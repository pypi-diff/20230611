# Comparing `tmp/miepython-2.3.2.tar.gz` & `tmp/miepython-2.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "miepython-2.3.2.tar", last modified: Thu May 18 22:25:29 2023, max compression
+gzip compressed data, was "miepython-2.4.0.tar", last modified: Sat Jun 10 22:07:22 2023, max compression
```

## Comparing `miepython-2.3.2.tar` & `miepython-2.4.0.tar`

### file list

```diff
@@ -1,61 +1,61 @@
-drwxr-xr-x   0 prahl      (502) staff       (20)        0 2023-05-18 22:25:29.628378 miepython-2.3.2/
-drwxr-xr-x   0 prahl      (502) staff       (20)        0 2023-05-18 22:25:29.397087 miepython-2.3.2/.github/
-drwxr-xr-x   0 prahl      (502) staff       (20)        0 2023-05-18 22:25:29.404818 miepython-2.3.2/.github/workflows/
--rw-r--r--   0 prahl      (502) staff       (20)      713 2022-01-26 22:36:27.000000 miepython-2.3.2/.github/workflows/test.yml
--rw-r--r--   0 prahl      (502) staff       (20)      164 2022-01-26 22:27:48.000000 miepython-2.3.2/.gitignore
--rw-r--r--   0 prahl      (502) staff       (20)      398 2021-11-17 18:49:05.000000 miepython-2.3.2/.readthedocs.yaml
--rw-r--r--   0 prahl      (502) staff       (20)       48 2022-01-25 19:27:23.000000 miepython-2.3.2/.testignore
--rw-r--r--   0 prahl      (502) staff       (20)     5500 2023-05-18 22:21:25.000000 miepython-2.3.2/CHANGELOG.rst
--rw-r--r--   0 prahl      (502) staff       (20)     1098 2023-05-18 22:23:49.000000 miepython-2.3.2/CITATION.cff
--rw-r--r--   0 prahl      (502) staff       (20)     1055 2021-11-17 18:49:05.000000 miepython-2.3.2/LICENSE.txt
--rw-r--r--   0 prahl      (502) staff       (20)      161 2023-05-18 22:09:45.000000 miepython-2.3.2/MANIFEST.in
--rw-r--r--   0 prahl      (502) staff       (20)     1797 2022-07-05 18:09:58.000000 miepython-2.3.2/Makefile
--rw-r--r--   0 prahl      (502) staff       (20)     4364 2023-05-18 22:25:29.628605 miepython-2.3.2/PKG-INFO
--rw-r--r--   0 prahl      (502) staff       (20)     3584 2023-05-18 22:03:55.000000 miepython-2.3.2/README.rst
-drwxr-xr-x   0 prahl      (502) staff       (20)        0 2023-05-18 22:25:29.555198 miepython-2.3.2/docs/
--rw-r--r--   0 prahl      (502) staff       (20)   190191 2022-07-27 18:07:30.000000 miepython-2.3.2/docs/01_basics.ipynb
--rw-r--r--   0 prahl      (502) staff       (20)    34904 2021-11-17 18:49:05.000000 miepython-2.3.2/docs/01_plot.png
--rw-r--r--   0 prahl      (502) staff       (20)   123686 2022-08-03 16:28:32.000000 miepython-2.3.2/docs/02_efficiencies.ipynb
--rw-r--r--   0 prahl      (502) staff       (20)    47794 2021-11-17 18:49:05.000000 miepython-2.3.2/docs/02_plot.png
--rw-r--r--   0 prahl      (502) staff       (20)   478393 2022-01-31 19:21:59.000000 miepython-2.3.2/docs/03_angular_scattering.ipynb
--rw-r--r--   0 prahl      (502) staff       (20)    34095 2021-11-17 18:49:05.000000 miepython-2.3.2/docs/03_plot.png
--rw-r--r--   0 prahl      (502) staff       (20)   165954 2022-07-27 19:14:22.000000 miepython-2.3.2/docs/03a_normalization.ipynb
--rw-r--r--   0 prahl      (502) staff       (20)    54959 2022-07-05 18:09:58.000000 miepython-2.3.2/docs/04_plot.png
--rw-r--r--   0 prahl      (502) staff       (20)   133775 2021-11-17 18:49:05.000000 miepython-2.3.2/docs/04_rayleigh.ipynb
--rw-r--r--   0 prahl      (502) staff       (20)   264354 2022-01-26 21:48:56.000000 miepython-2.3.2/docs/05_fog.ipynb
--rw-r--r--   0 prahl      (502) staff       (20)    88000 2021-11-17 18:49:06.000000 miepython-2.3.2/docs/06_random_deviates.ipynb
--rw-r--r--   0 prahl      (502) staff       (20)    43928 2022-01-25 19:22:34.000000 miepython-2.3.2/docs/07_algorithm.ipynb
--rw-r--r--   0 prahl      (502) staff       (20)   565045 2021-11-17 18:49:06.000000 miepython-2.3.2/docs/08_large_spheres.ipynb
--rw-r--r--   0 prahl      (502) staff       (20)    33297 2021-11-17 18:49:06.000000 miepython-2.3.2/docs/09_backscattering.ipynb
--rw-r--r--   0 prahl      (502) staff       (20)    21271 2021-11-17 18:49:06.000000 miepython-2.3.2/docs/10_basic_tests.ipynb
--rw-r--r--   0 prahl      (502) staff       (20)   111396 2021-11-17 18:49:06.000000 miepython-2.3.2/docs/11_performance.ipynb
--rw-r--r--   0 prahl      (502) staff       (20)       29 2021-11-17 18:49:06.000000 miepython-2.3.2/docs/changelog.rst
--rw-r--r--   0 prahl      (502) staff       (20)     1953 2022-07-05 18:09:58.000000 miepython-2.3.2/docs/conf.py
--rw-r--r--   0 prahl      (502) staff       (20)     3407 2022-07-27 18:48:20.000000 miepython-2.3.2/docs/index.rst
--rw-r--r--   0 prahl      (502) staff       (20)      136 2022-01-28 00:11:47.000000 miepython-2.3.2/docs/miepython.rst
--rw-r--r--   0 prahl      (502) staff       (20)       76 2022-07-05 18:09:58.000000 miepython-2.3.2/docs/requirements.txt
-drwxr-xr-x   0 prahl      (502) staff       (20)        0 2023-05-18 22:25:29.557592 miepython-2.3.2/miepython/
--rw-r--r--   0 prahl      (502) staff       (20)     1432 2023-05-18 22:21:35.000000 miepython-2.3.2/miepython/__init__.py
-drwxr-xr-x   0 prahl      (502) staff       (20)        0 2023-05-18 22:25:29.607507 miepython-2.3.2/miepython/data/
--rw-r--r--   0 prahl      (502) staff       (20)     1337 2022-01-26 18:53:40.000000 miepython-2.3.2/miepython/data/Johnson.txt
--rw-r--r--   0 prahl      (502) staff       (20)     1337 2022-01-26 20:40:40.000000 miepython-2.3.2/miepython/data/ag-Johnson.txt
--rw-r--r--   0 prahl      (502) staff       (20)    36719 2017-08-05 17:05:42.000000 miepython-2.3.2/miepython/data/segelstein81_index.txt
-drwxr-xr-x   0 prahl      (502) staff       (20)        0 2023-05-18 22:25:29.627297 miepython-2.3.2/miepython/examples/
--rwxr-xr-x   0 prahl      (502) staff       (20)      684 2021-11-17 18:49:06.000000 miepython-2.3.2/miepython/examples/01_dielectric.py
--rwxr-xr-x   0 prahl      (502) staff       (20)      804 2021-11-17 18:49:06.000000 miepython-2.3.2/miepython/examples/02_glass.py
--rwxr-xr-x   0 prahl      (502) staff       (20)      921 2021-11-17 18:49:06.000000 miepython-2.3.2/miepython/examples/03_droplets.py
--rwxr-xr-x   0 prahl      (502) staff       (20)     2717 2022-07-05 18:09:58.000000 miepython-2.3.2/miepython/examples/04_gold.py
--rw-r--r--   0 prahl      (502) staff       (20)    26737 2022-07-26 20:03:48.000000 miepython-2.3.2/miepython/miepython.py
--rw-r--r--   0 prahl      (502) staff       (20)    24387 2022-07-05 18:09:58.000000 miepython-2.3.2/miepython/miepython_nojit.py
-drwxr-xr-x   0 prahl      (502) staff       (20)        0 2023-05-18 22:25:29.560825 miepython-2.3.2/miepython.egg-info/
--rw-r--r--   0 prahl      (502) staff       (20)     4364 2023-05-18 22:25:29.000000 miepython-2.3.2/miepython.egg-info/PKG-INFO
--rw-r--r--   0 prahl      (502) staff       (20)     1156 2023-05-18 22:25:29.000000 miepython-2.3.2/miepython.egg-info/SOURCES.txt
--rw-r--r--   0 prahl      (502) staff       (20)        1 2023-05-18 22:25:29.000000 miepython-2.3.2/miepython.egg-info/dependency_links.txt
--rw-r--r--   0 prahl      (502) staff       (20)       23 2023-05-18 22:25:29.000000 miepython-2.3.2/miepython.egg-info/requires.txt
--rw-r--r--   0 prahl      (502) staff       (20)       10 2023-05-18 22:25:29.000000 miepython-2.3.2/miepython.egg-info/top_level.txt
--rw-r--r--   0 prahl      (502) staff       (20)      569 2022-07-05 18:09:58.000000 miepython-2.3.2/pyproject.toml
--rw-r--r--   0 prahl      (502) staff       (20)      602 2022-03-11 18:19:27.000000 miepython-2.3.2/release.txt
--rw-r--r--   0 prahl      (502) staff       (20)      182 2022-01-26 22:23:15.000000 miepython-2.3.2/requirements-dev.txt
--rw-r--r--   0 prahl      (502) staff       (20)       22 2022-01-26 22:23:09.000000 miepython-2.3.2/requirements.txt
--rw-r--r--   0 prahl      (502) staff       (20)      986 2023-05-18 22:25:29.629541 miepython-2.3.2/setup.cfg
--rw-r--r--   0 prahl      (502) staff       (20)     1095 2022-07-05 18:09:58.000000 miepython-2.3.2/setup.py
+drwxr-xr-x   0 prahl      (501) staff       (20)        0 2023-06-10 22:07:22.939050 miepython-2.4.0/
+drwxr-xr-x   0 prahl      (501) staff       (20)        0 2023-06-10 22:07:22.876983 miepython-2.4.0/.github/
+drwxr-xr-x   0 prahl      (501) staff       (20)        0 2023-06-10 22:07:22.887274 miepython-2.4.0/.github/workflows/
+-rw-r--r--   0 prahl      (501) staff       (20)      713 2022-01-27 02:10:04.000000 miepython-2.4.0/.github/workflows/test.yml
+-rw-r--r--   0 prahl      (501) staff       (20)      164 2022-01-27 02:10:04.000000 miepython-2.4.0/.gitignore
+-rw-r--r--   0 prahl      (501) staff       (20)      398 2021-08-16 19:03:47.000000 miepython-2.4.0/.readthedocs.yaml
+-rw-r--r--   0 prahl      (501) staff       (20)       48 2022-01-26 16:03:16.000000 miepython-2.4.0/.testignore
+-rw-r--r--   0 prahl      (501) staff       (20)     5608 2023-06-10 21:51:59.000000 miepython-2.4.0/CHANGELOG.rst
+-rw-r--r--   0 prahl      (501) staff       (20)      328 2023-05-26 22:17:36.000000 miepython-2.4.0/CITATION.cff
+-rw-r--r--   0 prahl      (501) staff       (20)     1055 2021-03-21 17:45:57.000000 miepython-2.4.0/LICENSE.txt
+-rw-r--r--   0 prahl      (501) staff       (20)      161 2023-05-26 22:17:36.000000 miepython-2.4.0/MANIFEST.in
+-rw-r--r--   0 prahl      (501) staff       (20)     1767 2023-06-10 21:55:43.000000 miepython-2.4.0/Makefile
+-rw-r--r--   0 prahl      (501) staff       (20)     4094 2023-06-10 22:07:22.939377 miepython-2.4.0/PKG-INFO
+-rw-r--r--   0 prahl      (501) staff       (20)     3314 2023-05-26 22:17:36.000000 miepython-2.4.0/README.rst
+drwxr-xr-x   0 prahl      (501) staff       (20)        0 2023-06-10 22:07:22.923510 miepython-2.4.0/docs/
+-rw-r--r--   0 prahl      (501) staff       (20)   190191 2023-05-26 22:17:36.000000 miepython-2.4.0/docs/01_basics.ipynb
+-rw-r--r--   0 prahl      (501) staff       (20)    34904 2021-01-18 22:54:10.000000 miepython-2.4.0/docs/01_plot.png
+-rw-r--r--   0 prahl      (501) staff       (20)   123686 2023-05-26 22:17:36.000000 miepython-2.4.0/docs/02_efficiencies.ipynb
+-rw-r--r--   0 prahl      (501) staff       (20)    47794 2021-01-18 22:55:06.000000 miepython-2.4.0/docs/02_plot.png
+-rw-r--r--   0 prahl      (501) staff       (20)   478393 2022-01-30 19:54:28.000000 miepython-2.4.0/docs/03_angular_scattering.ipynb
+-rw-r--r--   0 prahl      (501) staff       (20)    34095 2021-01-18 22:55:36.000000 miepython-2.4.0/docs/03_plot.png
+-rw-r--r--   0 prahl      (501) staff       (20)   165954 2023-05-26 22:17:36.000000 miepython-2.4.0/docs/03a_normalization.ipynb
+-rw-r--r--   0 prahl      (501) staff       (20)    54959 2022-03-13 17:44:50.000000 miepython-2.4.0/docs/04_plot.png
+-rw-r--r--   0 prahl      (501) staff       (20)   133775 2021-04-25 22:33:21.000000 miepython-2.4.0/docs/04_rayleigh.ipynb
+-rw-r--r--   0 prahl      (501) staff       (20)   264354 2021-04-25 22:33:21.000000 miepython-2.4.0/docs/05_fog.ipynb
+-rw-r--r--   0 prahl      (501) staff       (20)    88000 2021-04-25 22:33:21.000000 miepython-2.4.0/docs/06_random_deviates.ipynb
+-rw-r--r--   0 prahl      (501) staff       (20)    43928 2022-01-26 16:03:16.000000 miepython-2.4.0/docs/07_algorithm.ipynb
+-rw-r--r--   0 prahl      (501) staff       (20)   565045 2021-04-25 22:33:21.000000 miepython-2.4.0/docs/08_large_spheres.ipynb
+-rw-r--r--   0 prahl      (501) staff       (20)    33297 2021-04-25 22:33:21.000000 miepython-2.4.0/docs/09_backscattering.ipynb
+-rw-r--r--   0 prahl      (501) staff       (20)    21271 2021-05-22 14:24:13.000000 miepython-2.4.0/docs/10_basic_tests.ipynb
+-rw-r--r--   0 prahl      (501) staff       (20)   111396 2021-04-25 22:33:21.000000 miepython-2.4.0/docs/11_performance.ipynb
+-rw-r--r--   0 prahl      (501) staff       (20)       29 2020-03-30 16:00:58.000000 miepython-2.4.0/docs/changelog.rst
+-rw-r--r--   0 prahl      (501) staff       (20)     1953 2022-07-05 15:41:23.000000 miepython-2.4.0/docs/conf.py
+-rw-r--r--   0 prahl      (501) staff       (20)     3113 2023-05-26 22:17:36.000000 miepython-2.4.0/docs/index.rst
+-rw-r--r--   0 prahl      (501) staff       (20)      136 2022-01-27 02:10:43.000000 miepython-2.4.0/docs/miepython.rst
+-rw-r--r--   0 prahl      (501) staff       (20)       76 2022-07-05 15:42:07.000000 miepython-2.4.0/docs/requirements.txt
+drwxr-xr-x   0 prahl      (501) staff       (20)        0 2023-06-10 22:07:22.927018 miepython-2.4.0/miepython/
+-rw-r--r--   0 prahl      (501) staff       (20)     1498 2023-06-10 21:47:39.000000 miepython-2.4.0/miepython/__init__.py
+drwxr-xr-x   0 prahl      (501) staff       (20)        0 2023-06-10 22:07:22.933208 miepython-2.4.0/miepython/data/
+-rw-r--r--   0 prahl      (501) staff       (20)     1337 2022-01-27 02:10:04.000000 miepython-2.4.0/miepython/data/Johnson.txt
+-rw-r--r--   0 prahl      (501) staff       (20)     1337 2022-01-27 02:10:04.000000 miepython-2.4.0/miepython/data/ag-Johnson.txt
+-rw-r--r--   0 prahl      (501) staff       (20)    36719 2022-01-27 02:10:04.000000 miepython-2.4.0/miepython/data/segelstein81_index.txt
+drwxr-xr-x   0 prahl      (501) staff       (20)        0 2023-06-10 22:07:22.937851 miepython-2.4.0/miepython/examples/
+-rwxr-xr-x   0 prahl      (501) staff       (20)      684 2021-07-09 19:31:22.000000 miepython-2.4.0/miepython/examples/01_dielectric.py
+-rwxr-xr-x   0 prahl      (501) staff       (20)      804 2021-07-09 19:33:51.000000 miepython-2.4.0/miepython/examples/02_glass.py
+-rwxr-xr-x   0 prahl      (501) staff       (20)      921 2021-07-09 19:46:36.000000 miepython-2.4.0/miepython/examples/03_droplets.py
+-rwxr-xr-x   0 prahl      (501) staff       (20)     2717 2022-03-12 23:14:57.000000 miepython-2.4.0/miepython/examples/04_gold.py
+-rw-r--r--   0 prahl      (501) staff       (20)    28173 2023-06-10 21:52:43.000000 miepython-2.4.0/miepython/miepython.py
+-rw-r--r--   0 prahl      (501) staff       (20)    25822 2023-06-10 21:52:20.000000 miepython-2.4.0/miepython/miepython_nojit.py
+drwxr-xr-x   0 prahl      (501) staff       (20)        0 2023-06-10 22:07:22.930642 miepython-2.4.0/miepython.egg-info/
+-rw-r--r--   0 prahl      (501) staff       (20)     4094 2023-06-10 22:07:22.000000 miepython-2.4.0/miepython.egg-info/PKG-INFO
+-rw-r--r--   0 prahl      (501) staff       (20)     1156 2023-06-10 22:07:22.000000 miepython-2.4.0/miepython.egg-info/SOURCES.txt
+-rw-r--r--   0 prahl      (501) staff       (20)        1 2023-06-10 22:07:22.000000 miepython-2.4.0/miepython.egg-info/dependency_links.txt
+-rw-r--r--   0 prahl      (501) staff       (20)       23 2023-06-10 22:07:22.000000 miepython-2.4.0/miepython.egg-info/requires.txt
+-rw-r--r--   0 prahl      (501) staff       (20)       10 2023-06-10 22:07:22.000000 miepython-2.4.0/miepython.egg-info/top_level.txt
+-rw-r--r--   0 prahl      (501) staff       (20)      569 2022-07-05 15:56:06.000000 miepython-2.4.0/pyproject.toml
+-rw-r--r--   0 prahl      (501) staff       (20)      602 2022-03-12 18:25:05.000000 miepython-2.4.0/release.txt
+-rw-r--r--   0 prahl      (501) staff       (20)      182 2021-05-22 21:35:05.000000 miepython-2.4.0/requirements-dev.txt
+-rw-r--r--   0 prahl      (501) staff       (20)       22 2021-04-25 22:33:21.000000 miepython-2.4.0/requirements.txt
+-rw-r--r--   0 prahl      (501) staff       (20)      986 2023-06-10 22:07:22.940582 miepython-2.4.0/setup.cfg
+-rw-r--r--   0 prahl      (501) staff       (20)     1095 2022-03-12 23:40:23.000000 miepython-2.4.0/setup.py
```

### Comparing `miepython-2.3.2/.github/workflows/test.yml` & `miepython-2.4.0/.github/workflows/test.yml`

 * *Files identical despite different names*

### Comparing `miepython-2.3.2/CHANGELOG.rst` & `miepython-2.4.0/CHANGELOG.rst`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,14 @@
 Changelog
 =========
 
+v2.4.0 (6/10/2023)
+-------------------
+*   add mie_phase_matrix() to calculate scattering (Mueller) matrix
+
 v2.3.2
 -------------------
 *   fix typo in README.rst that prevented pypi upload
 *   add CITATION.cff to base level of miepython repository
 
 v2.3.1
 -------------------
```

### Comparing `miepython-2.3.2/LICENSE.txt` & `miepython-2.4.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `miepython-2.3.2/Makefile` & `miepython-2.4.0/Makefile`

 * *Files 2% similar despite different names*

```diff
@@ -22,92 +22,90 @@
 00000150: 6b73 2e70 790a 0972 6d20 2d72 6620 5f5f  ks.py..rm -rf __
 00000160: 7079 6361 6368 655f 5f0a 0a72 7374 6368  pycache__..rstch
 00000170: 6563 6b3a 0a09 2d72 7374 6368 6563 6b20  eck:..-rstcheck 
 00000180: 5245 4144 4d45 2e72 7374 0a09 2d72 7374  README.rst..-rst
 00000190: 6368 6563 6b20 4348 414e 4745 4c4f 472e  check CHANGELOG.
 000001a0: 7273 740a 092d 7273 7463 6865 636b 2064  rst..-rstcheck d
 000001b0: 6f63 732f 696e 6465 782e 7273 740a 092d  ocs/index.rst..-
-000001c0: 7273 7463 6865 636b 2064 6f63 732f 6368  rstcheck docs/ch
-000001d0: 616e 6765 6c6f 672e 7273 740a 092d 7273  angelog.rst..-rs
-000001e0: 7463 6865 636b 202d 2d69 676e 6f72 652d  tcheck --ignore-
-000001f0: 6469 7265 6374 6976 6573 2061 7574 6f6d  directives autom
-00000200: 6f64 6170 6920 646f 6373 2f6d 6965 7079  odapi docs/miepy
-00000210: 7468 6f6e 2e72 7374 0a0a 6c69 6e74 6368  thon.rst..lintch
-00000220: 6563 6b3a 0a09 2d70 796c 696e 7420 6d69  eck:..-pylint mi
-00000230: 6570 7974 686f 6e2f 6d69 6570 7974 686f  epython/miepytho
-00000240: 6e2e 7079 0a09 2d70 796c 696e 7420 6d69  n.py..-pylint mi
-00000250: 6570 7974 686f 6e2f 6d69 6570 7974 686f  epython/miepytho
-00000260: 6e5f 6e6f 6a69 742e 7079 0a09 2d70 796c  n_nojit.py..-pyl
-00000270: 696e 7420 6d69 6570 7974 686f 6e2f 5f5f  int miepython/__
-00000280: 696e 6974 5f5f 2e70 790a 092d 7079 6c69  init__.py..-pyli
-00000290: 6e74 2074 6573 7473 2f74 6573 745f 616c  nt tests/test_al
-000002a0: 6c5f 6578 616d 706c 6573 2e70 790a 092d  l_examples.py..-
-000002b0: 7079 6c69 6e74 2074 6573 7473 2f74 6573  pylint tests/tes
-000002c0: 745f 616c 6c5f 6e6f 7465 626f 6f6b 732e  t_all_notebooks.
-000002d0: 7079 0a09 2d70 796c 696e 7420 7465 7374  py..-pylint test
-000002e0: 732f 7465 7374 5f6a 6974 2e70 790a 092d  s/test_jit.py..-
-000002f0: 7079 6c69 6e74 2074 6573 7473 2f74 6573  pylint tests/tes
-00000300: 745f 6e6f 6a69 742e 7079 0a09 2d70 796c  t_nojit.py..-pyl
-00000310: 696e 7420 646f 6373 2f63 6f6e 662e 7079  int docs/conf.py
-00000320: 0a0a 646f 6363 6865 636b 3a0a 092d 7079  ..doccheck:..-py
-00000330: 646f 6373 7479 6c65 206d 6965 7079 7468  docstyle miepyth
-00000340: 6f6e 2f6d 6965 7079 7468 6f6e 2e70 790a  on/miepython.py.
-00000350: 092d 7079 646f 6373 7479 6c65 206d 6965  .-pydocstyle mie
-00000360: 7079 7468 6f6e 2f6d 6965 7079 7468 6f6e  python/miepython
-00000370: 5f6e 6f6a 6974 2e70 790a 092d 7079 646f  _nojit.py..-pydo
-00000380: 6373 7479 6c65 206d 6965 7079 7468 6f6e  cstyle miepython
-00000390: 2f5f 5f69 6e69 745f 5f2e 7079 0a09 2d70  /__init__.py..-p
-000003a0: 7964 6f63 7374 796c 6520 7465 7374 732f  ydocstyle tests/
-000003b0: 7465 7374 5f61 6c6c 5f65 7861 6d70 6c65  test_all_example
-000003c0: 732e 7079 0a09 2d70 7964 6f63 7374 796c  s.py..-pydocstyl
-000003d0: 6520 7465 7374 732f 7465 7374 5f61 6c6c  e tests/test_all
-000003e0: 5f6e 6f74 6562 6f6f 6b73 2e70 790a 092d  _notebooks.py..-
-000003f0: 7079 646f 6373 7479 6c65 202d 2d69 676e  pydocstyle --ign
-00000400: 6f72 6520 4431 3030 2c44 3130 312c 4431  ore D100,D101,D1
-00000410: 3032 2074 6573 7473 2f74 6573 745f 6a69  02 tests/test_ji
-00000420: 742e 7079 0a09 2d70 7964 6f63 7374 796c  t.py..-pydocstyl
-00000430: 6520 2d2d 6967 6e6f 7265 2044 3130 302c  e --ignore D100,
-00000440: 4431 3031 2c44 3130 3220 7465 7374 732f  D101,D102 tests/
-00000450: 7465 7374 5f6e 6f6a 6974 2e70 790a 0a72  test_nojit.py..r
-00000460: 6368 6563 6b3a 0a09 6d61 6b65 206e 6f74  check:..make not
-00000470: 6563 6865 636b 0a09 6d61 6b65 2072 7374  echeck..make rst
-00000480: 6368 6563 6b0a 096d 616b 6520 6c69 6e74  check..make lint
-00000490: 6368 6563 6b0a 096d 616b 6520 646f 6363  check..make docc
-000004a0: 6865 636b 0a09 2d20 666c 616b 6538 202e  heck..- flake8 .
-000004b0: 0a09 7079 726f 6d61 202d 6420 2e0a 0963  ..pyroma -d ...c
-000004c0: 6865 636b 2d6d 616e 6966 6573 740a 096d  heck-manifest..m
-000004d0: 616b 6520 6874 6d6c 0a09 6d61 6b65 206a  ake html..make j
-000004e0: 6974 7465 7374 0a0a 6a69 7474 6573 743a  ittest..jittest:
-000004f0: 0a09 7079 7468 6f6e 3320 2d6d 2070 7974  ..python3 -m pyt
-00000500: 6573 7420 7465 7374 732f 7465 7374 5f6e  est tests/test_n
-00000510: 6f6a 6974 2e70 790a 0970 7974 686f 6e33  ojit.py..python3
-00000520: 202d 6d20 7079 7465 7374 2074 6573 7473   -m pytest tests
-00000530: 2f74 6573 745f 6a69 742e 7079 0a0a 7465  /test_jit.py..te
-00000540: 7374 3a0a 0974 6f78 0a0a 636c 6561 6e3a  st:..tox..clean:
-00000550: 0a09 726d 202d 7266 2064 6973 740a 0972  ..rm -rf dist..r
-00000560: 6d20 2d72 6620 6d69 6570 7974 686f 6e2e  m -rf miepython.
-00000570: 6567 672d 696e 666f 0a09 726d 202d 7266  egg-info..rm -rf
-00000580: 206d 6965 7079 7468 6f6e 2f5f 5f70 7963   miepython/__pyc
-00000590: 6163 6865 5f5f 0a09 726d 202d 7266 206d  ache__..rm -rf m
-000005a0: 6965 7079 7468 6f6e 2f65 7861 6d70 6c65  iepython/example
-000005b0: 732f 5f5f 7079 6361 6368 655f 5f0a 0972  s/__pycache__..r
-000005c0: 6d20 2d72 6620 646f 6373 2f2e 4453 5f53  m -rf docs/.DS_S
-000005d0: 746f 7265 0a09 726d 202d 7266 2064 6f63  tore..rm -rf doc
-000005e0: 732f 6170 690a 0972 6d20 2d72 6620 646f  s/api..rm -rf do
-000005f0: 6373 2f5f 6275 696c 640a 0972 6d20 2d72  cs/_build..rm -r
-00000600: 6620 646f 6373 2f2e 6970 796e 625f 6368  f docs/.ipynb_ch
-00000610: 6563 6b70 6f69 6e74 730a 0972 6d20 2d72  eckpoints..rm -r
-00000620: 6620 646f 6373 2f2e 7079 7465 7374 5f63  f docs/.pytest_c
-00000630: 6163 6865 0a09 726d 202d 7266 2074 6573  ache..rm -rf tes
-00000640: 7473 2f5f 5f70 7963 6163 6865 5f5f 0a09  ts/__pycache__..
-00000650: 726d 202d 7266 202e 746f 780a 0972 6d20  rm -rf .tox..rm 
-00000660: 2d72 6620 3034 5f70 6c6f 742e 706e 670a  -rf 04_plot.png.
-00000670: 0972 6d20 2d72 6620 2e70 7974 6573 745f  .rm -rf .pytest_
-00000680: 6361 6368 650a 0972 6d20 2d72 6620 6275  cache..rm -rf bu
-00000690: 696c 640a 0a72 6561 6c63 6c65 616e 3a0a  ild..realclean:.
-000006a0: 096d 616b 6520 636c 6561 6e0a 0a2e 5048  .make clean...PH
-000006b0: 4f4e 593a 2063 6c65 616e 2068 746d 6c20  ONY: clean html 
-000006c0: 7465 7374 2072 6561 6c63 6c65 616e 205c  test realclean \
-000006d0: 0a20 2020 2020 2020 2072 6368 6563 6b20  .        rcheck 
-000006e0: 646f 6363 6865 636b 206c 696e 7463 6865  doccheck lintche
-000006f0: 636b 2072 7374 6368 6563 6b20 6e6f 7465  ck rstcheck note
-00000700: 6368 6563 6b                             check
+000001c0: 7273 7463 6865 636b 202d 2d69 676e 6f72  rstcheck --ignor
+000001d0: 652d 6469 7265 6374 6976 6573 2061 7574  e-directives aut
+000001e0: 6f6d 6f64 6170 6920 646f 6373 2f6d 6965  omodapi docs/mie
+000001f0: 7079 7468 6f6e 2e72 7374 0a0a 6c69 6e74  python.rst..lint
+00000200: 6368 6563 6b3a 0a09 2d70 796c 696e 7420  check:..-pylint 
+00000210: 6d69 6570 7974 686f 6e2f 6d69 6570 7974  miepython/miepyt
+00000220: 686f 6e2e 7079 0a09 2d70 796c 696e 7420  hon.py..-pylint 
+00000230: 6d69 6570 7974 686f 6e2f 6d69 6570 7974  miepython/miepyt
+00000240: 686f 6e5f 6e6f 6a69 742e 7079 0a09 2d70  hon_nojit.py..-p
+00000250: 796c 696e 7420 6d69 6570 7974 686f 6e2f  ylint miepython/
+00000260: 5f5f 696e 6974 5f5f 2e70 790a 092d 7079  __init__.py..-py
+00000270: 6c69 6e74 2074 6573 7473 2f74 6573 745f  lint tests/test_
+00000280: 616c 6c5f 6578 616d 706c 6573 2e70 790a  all_examples.py.
+00000290: 092d 7079 6c69 6e74 2074 6573 7473 2f74  .-pylint tests/t
+000002a0: 6573 745f 616c 6c5f 6e6f 7465 626f 6f6b  est_all_notebook
+000002b0: 732e 7079 0a09 2d70 796c 696e 7420 7465  s.py..-pylint te
+000002c0: 7374 732f 7465 7374 5f6a 6974 2e70 790a  sts/test_jit.py.
+000002d0: 092d 7079 6c69 6e74 2074 6573 7473 2f74  .-pylint tests/t
+000002e0: 6573 745f 6e6f 6a69 742e 7079 0a09 2d70  est_nojit.py..-p
+000002f0: 796c 696e 7420 646f 6373 2f63 6f6e 662e  ylint docs/conf.
+00000300: 7079 0a0a 646f 6363 6865 636b 3a0a 092d  py..doccheck:..-
+00000310: 7079 646f 6373 7479 6c65 206d 6965 7079  pydocstyle miepy
+00000320: 7468 6f6e 2f6d 6965 7079 7468 6f6e 2e70  thon/miepython.p
+00000330: 790a 092d 7079 646f 6373 7479 6c65 206d  y..-pydocstyle m
+00000340: 6965 7079 7468 6f6e 2f6d 6965 7079 7468  iepython/miepyth
+00000350: 6f6e 5f6e 6f6a 6974 2e70 790a 092d 7079  on_nojit.py..-py
+00000360: 646f 6373 7479 6c65 206d 6965 7079 7468  docstyle miepyth
+00000370: 6f6e 2f5f 5f69 6e69 745f 5f2e 7079 0a09  on/__init__.py..
+00000380: 2d70 7964 6f63 7374 796c 6520 7465 7374  -pydocstyle test
+00000390: 732f 7465 7374 5f61 6c6c 5f65 7861 6d70  s/test_all_examp
+000003a0: 6c65 732e 7079 0a09 2d70 7964 6f63 7374  les.py..-pydocst
+000003b0: 796c 6520 7465 7374 732f 7465 7374 5f61  yle tests/test_a
+000003c0: 6c6c 5f6e 6f74 6562 6f6f 6b73 2e70 790a  ll_notebooks.py.
+000003d0: 092d 7079 646f 6373 7479 6c65 202d 2d69  .-pydocstyle --i
+000003e0: 676e 6f72 6520 4431 3030 2c44 3130 312c  gnore D100,D101,
+000003f0: 4431 3032 2074 6573 7473 2f74 6573 745f  D102 tests/test_
+00000400: 6a69 742e 7079 0a09 2d70 7964 6f63 7374  jit.py..-pydocst
+00000410: 796c 6520 2d2d 6967 6e6f 7265 2044 3130  yle --ignore D10
+00000420: 302c 4431 3031 2c44 3130 3220 7465 7374  0,D101,D102 test
+00000430: 732f 7465 7374 5f6e 6f6a 6974 2e70 790a  s/test_nojit.py.
+00000440: 0a72 6368 6563 6b3a 0a09 6d61 6b65 206e  .rcheck:..make n
+00000450: 6f74 6563 6865 636b 0a09 6d61 6b65 2072  otecheck..make r
+00000460: 7374 6368 6563 6b0a 096d 616b 6520 6c69  stcheck..make li
+00000470: 6e74 6368 6563 6b0a 096d 616b 6520 646f  ntcheck..make do
+00000480: 6363 6865 636b 0a09 2d20 666c 616b 6538  ccheck..- flake8
+00000490: 202e 0a09 7079 726f 6d61 202d 6420 2e0a   ...pyroma -d ..
+000004a0: 0963 6865 636b 2d6d 616e 6966 6573 740a  .check-manifest.
+000004b0: 096d 616b 6520 6874 6d6c 0a09 6d61 6b65  .make html..make
+000004c0: 206a 6974 7465 7374 0a0a 6a69 7474 6573   jittest..jittes
+000004d0: 743a 0a09 7079 7468 6f6e 3320 2d6d 2070  t:..python3 -m p
+000004e0: 7974 6573 7420 7465 7374 732f 7465 7374  ytest tests/test
+000004f0: 5f6e 6f6a 6974 2e70 790a 0970 7974 686f  _nojit.py..pytho
+00000500: 6e33 202d 6d20 7079 7465 7374 2074 6573  n3 -m pytest tes
+00000510: 7473 2f74 6573 745f 6a69 742e 7079 0a0a  ts/test_jit.py..
+00000520: 7465 7374 3a0a 0974 6f78 0a0a 636c 6561  test:..tox..clea
+00000530: 6e3a 0a09 726d 202d 7266 2064 6973 740a  n:..rm -rf dist.
+00000540: 0972 6d20 2d72 6620 6d69 6570 7974 686f  .rm -rf miepytho
+00000550: 6e2e 6567 672d 696e 666f 0a09 726d 202d  n.egg-info..rm -
+00000560: 7266 206d 6965 7079 7468 6f6e 2f5f 5f70  rf miepython/__p
+00000570: 7963 6163 6865 5f5f 0a09 726d 202d 7266  ycache__..rm -rf
+00000580: 206d 6965 7079 7468 6f6e 2f65 7861 6d70   miepython/examp
+00000590: 6c65 732f 5f5f 7079 6361 6368 655f 5f0a  les/__pycache__.
+000005a0: 0972 6d20 2d72 6620 646f 6373 2f2e 4453  .rm -rf docs/.DS
+000005b0: 5f53 746f 7265 0a09 726d 202d 7266 2064  _Store..rm -rf d
+000005c0: 6f63 732f 6170 690a 0972 6d20 2d72 6620  ocs/api..rm -rf 
+000005d0: 646f 6373 2f5f 6275 696c 640a 0972 6d20  docs/_build..rm 
+000005e0: 2d72 6620 646f 6373 2f2e 6970 796e 625f  -rf docs/.ipynb_
+000005f0: 6368 6563 6b70 6f69 6e74 730a 0972 6d20  checkpoints..rm 
+00000600: 2d72 6620 646f 6373 2f2e 7079 7465 7374  -rf docs/.pytest
+00000610: 5f63 6163 6865 0a09 726d 202d 7266 2074  _cache..rm -rf t
+00000620: 6573 7473 2f5f 5f70 7963 6163 6865 5f5f  ests/__pycache__
+00000630: 0a09 726d 202d 7266 202e 746f 780a 0972  ..rm -rf .tox..r
+00000640: 6d20 2d72 6620 3034 5f70 6c6f 742e 706e  m -rf 04_plot.pn
+00000650: 670a 0972 6d20 2d72 6620 2e70 7974 6573  g..rm -rf .pytes
+00000660: 745f 6361 6368 650a 0972 6d20 2d72 6620  t_cache..rm -rf 
+00000670: 6275 696c 640a 0a72 6561 6c63 6c65 616e  build..realclean
+00000680: 3a0a 096d 616b 6520 636c 6561 6e0a 0a2e  :..make clean...
+00000690: 5048 4f4e 593a 2063 6c65 616e 2068 746d  PHONY: clean htm
+000006a0: 6c20 7465 7374 2072 6561 6c63 6c65 616e  l test realclean
+000006b0: 205c 0a20 2020 2020 2020 2072 6368 6563   \.        rchec
+000006c0: 6b20 646f 6363 6865 636b 206c 696e 7463  k doccheck lintc
+000006d0: 6865 636b 2072 7374 6368 6563 6b20 6e6f  heck rstcheck no
+000006e0: 7465 6368 6563 6b                        techeck
```

### Comparing `miepython-2.3.2/PKG-INFO` & `miepython-2.4.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: miepython
-Version: 2.3.2
+Version: 2.4.0
 Summary: Mie scattering of a plane wave by a sphere
 Home-page: https://github.com/scottprahl/miepython.git
 Author: Scott Prahl
 Author-email: scott.prahl@oit.edu
 License: MIT
 Keywords: mie,scattering,rainbow,droplet,backscatter,sphere,nanoparticle,sphere,cloud,phase function,efficiency,rayleigh,backscattering
 Classifier: Development Status :: 5 - Production/Stable
@@ -21,23 +21,17 @@
 =========
 
 by Scott Prahl
 
 .. image:: https://img.shields.io/pypi/v/miepython.svg
    :target: https://pypi.org/project/miepython/
 
-.. image:: https://colab.research.google.com/assets/colab-badge.svg
-   :target: https://colab.research.google.com/github/scottprahl/miepython/blob/master
-
 .. image:: https://img.shields.io/badge/readthedocs-latest-blue.svg
    :target: https://miepython.readthedocs.io
 
-.. image:: https://img.shields.io/badge/github-code-green.svg
-   :target: https://github.com/scottprahl/miepython
-
 .. image:: https://img.shields.io/badge/MIT-license-yellow.svg
    :target: https://github.com/scottprahl/miepython/blob/master/LICENSE.txt
 
 .. image:: https://github.com/scottprahl/miepython/actions/workflows/test.yml/badge.svg
    :target: https://github.com/scottprahl/miepython/actions/workflows/test.yml
 
 .. image:: https://zenodo.org/badge/99259684.svg
```

### Comparing `miepython-2.3.2/README.rst` & `miepython-2.4.0/README.rst`

 * *Files 10% similar despite different names*

```diff
@@ -2,23 +2,17 @@
 =========
 
 by Scott Prahl
 
 .. image:: https://img.shields.io/pypi/v/miepython.svg
    :target: https://pypi.org/project/miepython/
 
-.. image:: https://colab.research.google.com/assets/colab-badge.svg
-   :target: https://colab.research.google.com/github/scottprahl/miepython/blob/master
-
 .. image:: https://img.shields.io/badge/readthedocs-latest-blue.svg
    :target: https://miepython.readthedocs.io
 
-.. image:: https://img.shields.io/badge/github-code-green.svg
-   :target: https://github.com/scottprahl/miepython
-
 .. image:: https://img.shields.io/badge/MIT-license-yellow.svg
    :target: https://github.com/scottprahl/miepython/blob/master/LICENSE.txt
 
 .. image:: https://github.com/scottprahl/miepython/actions/workflows/test.yml/badge.svg
    :target: https://github.com/scottprahl/miepython/actions/workflows/test.yml
 
 .. image:: https://zenodo.org/badge/99259684.svg
```

### Comparing `miepython-2.3.2/docs/01_basics.ipynb` & `miepython-2.4.0/docs/01_basics.ipynb`

 * *Files identical despite different names*

### Comparing `miepython-2.3.2/docs/01_plot.png` & `miepython-2.4.0/docs/01_plot.png`

 * *Files identical despite different names*

### Comparing `miepython-2.3.2/docs/02_efficiencies.ipynb` & `miepython-2.4.0/docs/02_efficiencies.ipynb`

 * *Files identical despite different names*

### Comparing `miepython-2.3.2/docs/02_plot.png` & `miepython-2.4.0/docs/02_plot.png`

 * *Files identical despite different names*

### Comparing `miepython-2.3.2/docs/03_angular_scattering.ipynb` & `miepython-2.4.0/docs/03_angular_scattering.ipynb`

 * *Files identical despite different names*

### Comparing `miepython-2.3.2/docs/03_plot.png` & `miepython-2.4.0/docs/03_plot.png`

 * *Files identical despite different names*

### Comparing `miepython-2.3.2/docs/03a_normalization.ipynb` & `miepython-2.4.0/docs/03a_normalization.ipynb`

 * *Files identical despite different names*

### Comparing `miepython-2.3.2/docs/04_plot.png` & `miepython-2.4.0/docs/04_plot.png`

 * *Files identical despite different names*

### Comparing `miepython-2.3.2/docs/04_rayleigh.ipynb` & `miepython-2.4.0/docs/04_rayleigh.ipynb`

 * *Files identical despite different names*

### Comparing `miepython-2.3.2/docs/05_fog.ipynb` & `miepython-2.4.0/docs/05_fog.ipynb`

 * *Files identical despite different names*

### Comparing `miepython-2.3.2/docs/06_random_deviates.ipynb` & `miepython-2.4.0/docs/06_random_deviates.ipynb`

 * *Files identical despite different names*

### Comparing `miepython-2.3.2/docs/07_algorithm.ipynb` & `miepython-2.4.0/docs/07_algorithm.ipynb`

 * *Files identical despite different names*

### Comparing `miepython-2.3.2/docs/08_large_spheres.ipynb` & `miepython-2.4.0/docs/08_large_spheres.ipynb`

 * *Files identical despite different names*

### Comparing `miepython-2.3.2/docs/09_backscattering.ipynb` & `miepython-2.4.0/docs/09_backscattering.ipynb`

 * *Files identical despite different names*

### Comparing `miepython-2.3.2/docs/10_basic_tests.ipynb` & `miepython-2.4.0/docs/10_basic_tests.ipynb`

 * *Files identical despite different names*

### Comparing `miepython-2.3.2/docs/11_performance.ipynb` & `miepython-2.4.0/docs/11_performance.ipynb`

 * *Files identical despite different names*

### Comparing `miepython-2.3.2/docs/conf.py` & `miepython-2.4.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `miepython-2.3.2/docs/index.rst` & `miepython-2.4.0/docs/index.rst`

 * *Files 8% similar despite different names*

```diff
@@ -1,28 +1,24 @@
 miepython
 =========
 
+by Scott Prahl
+
 .. image:: https://img.shields.io/pypi/v/miepython.svg
    :target: https://pypi.org/project/miepython/
 
-.. image:: https://colab.research.google.com/assets/colab-badge.svg
-   :target: https://colab.research.google.com/github/scottprahl/miepython/blob/master
-
-.. image:: https://img.shields.io/badge/readthedocs-latest-blue.svg
-   :target: https://miepython.readthedocs.io
-
 .. image:: https://img.shields.io/badge/github-code-green.svg
    :target: https://github.com/scottprahl/miepython
 
-.. image:: https://img.shields.io/badge/MIT-license-yellow.svg
-   :target: https://github.com/scottprahl/miepython/blob/master/LICENSE.txt
-
 .. image:: https://github.com/scottprahl/miepython/actions/workflows/test.yml/badge.svg
    :target: https://github.com/scottprahl/miepython/actions/workflows/test.yml
 
+.. image:: https://zenodo.org/badge/99259684.svg
+   :target: https://zenodo.org/badge/latestdoi/99259684
+
 ----
 
 ``miepython`` is a pure Python module to calculate light scattering by
 non-absorbing, partially-absorbing, or perfectly conducting spheres. Mie
 theory is used, following `the procedure described by Wiscombe
 <http://opensky.ucar.edu/islandora/object/technotes:232>`_. This code has
 been validated against his results. 
@@ -43,15 +39,15 @@
 * the scattering phase function is normalized so it equals the *single scattering albedo* when integrated over 4π steradians by default.  As of version 2.3, this can be changed (see the normalization notebook for details).
 
 Using miepython
 ---------------
 
 1. You can install locally using pip::
     
-    pip install --user miepython
+    pip install miepython
 
 2. or `run this code in the cloud using Google Collaboratory <https://colab.research.google.com/github/scottprahl/miepython/blob/master>`_ by selecting the Jupyter notebook that interests you.
 
 Script Examples for those that don't do Jupyter
 -----------------------------------------------
 
 Simple Dielectric
```

### Comparing `miepython-2.3.2/miepython/__init__.py` & `miepython-2.4.0/miepython/__init__.py`

 * *Files 23% similar despite different names*

```diff
@@ -32,16 +32,21 @@
     miepython.i_unpolarized(m, x, mu)
 
 Mie scattering intensities normalized to one when integrated over all angles::
 
     miepython.i_per(m, x, mu, norm='one')
     miepython.i_par(m, x, mu, norm='one')
     miepython.i_unpolarized(m, x, mu, norm='one')
+
+The scattering matrix
+
+    miepython.mie_phase_matrix(m, x, mu)
+
 """
-__version__ = '2.3.2'
+__version__ = '2.4.0'
 __author__ = 'Scott Prahl'
 __email__ = 'scott.prahl@oit.edu'
 __copyright__ = 'Copyright 2017-23, Scott Prahl'
 __license__ = 'MIT'
 __url__ = 'https://github.com/scottprahl/miepython.git'
 
 from .miepython import *
```

### Comparing `miepython-2.3.2/miepython/data/Johnson.txt` & `miepython-2.4.0/miepython/data/Johnson.txt`

 * *Files identical despite different names*

### Comparing `miepython-2.3.2/miepython/data/ag-Johnson.txt` & `miepython-2.4.0/miepython/data/ag-Johnson.txt`

 * *Files identical despite different names*

### Comparing `miepython-2.3.2/miepython/data/segelstein81_index.txt` & `miepython-2.4.0/miepython/data/segelstein81_index.txt`

 * *Files identical despite different names*

### Comparing `miepython-2.3.2/miepython/examples/01_dielectric.py` & `miepython-2.4.0/miepython/examples/01_dielectric.py`

 * *Files identical despite different names*

### Comparing `miepython-2.3.2/miepython/examples/02_glass.py` & `miepython-2.4.0/miepython/examples/02_glass.py`

 * *Files identical despite different names*

### Comparing `miepython-2.3.2/miepython/examples/03_droplets.py` & `miepython-2.4.0/miepython/examples/03_droplets.py`

 * *Files identical despite different names*

### Comparing `miepython-2.3.2/miepython/examples/04_gold.py` & `miepython-2.4.0/miepython/examples/04_gold.py`

 * *Files identical despite different names*

### Comparing `miepython-2.3.2/miepython/miepython.py` & `miepython-2.4.0/miepython/miepython.py`

 * *Files 2% similar despite different names*

```diff
@@ -46,14 +46,15 @@
 __all__ = ('ez_mie',
            'ez_intensities',
            'i_par',
            'i_per',
            'i_unpolarized',
            'mie',
            'mie_S1_S2',
+           'mie_phase_matrix',
            'mie_cdf',
            'mie_mu_with_uniform_cdf',
            'generate_mie_costheta',
            )
 
 
 @njit((complex128, int32), cache=True)
@@ -638,14 +639,60 @@
         mu_array = np.array([mu], dtype=float)
         s1, s2 = _mie_S1_S2(m, x, mu_array, norm_int)
         return s1[0], s2[0]
 
     return _mie_S1_S2(m, x, mu, norm_int)
 
 
+def mie_phase_matrix(m, x, mu, norm='albedo'):
+    """
+    Calculate the scattering (Mueller) matrix.
+
+    If mu has length N, then the returned matrix is 4x4xN.  If mu is a scalar
+    then the matrix is 4x4
+
+    The phase scattering matrix is computed from the scattering amplitude
+    functions, according to equations 5.2.105-6 in K. N. Liou (**2002**) -
+    *An Introduction to Atmospheric Radiation*, Second Edition.
+
+    or
+
+    Bohren and Huffman, *Absorption and Scattering of Light by Small Particles*,
+    JOHN WILEY & SONS, page 112, (1983).
+
+    Args:
+        m: the complex index of refraction of the sphere
+        x: the size parameter of the sphere
+        mu: the angles, cos(theta), for the phase scattering matrix
+
+    Returns:
+        p: the phase scattering matrix [sr**(-1.0)]
+    """
+    s1, s2 = mie_S1_S2(m=m, x=x, mu=mu, norm=norm)
+
+    mu = np.atleast_1d(mu)
+    s1_star = np.conjugate(s1)
+    s2_star = np.conjugate(s2)
+    m1 = (s1 * s1_star).real
+    m2 = (s2 * s2_star).real
+    s21 = (0.5 * (s1 * s2_star + s2 * s1_star)).real
+    d21 = (-0.5j * (s1 * s2_star - s2 * s1_star)).real
+    phase = np.zeros(shape=(4, 4, mu.size))
+    phase[0, 0] = 0.5 * (m2 + m1)
+    phase[0, 1] = 0.5 * (m2 - m1)
+    phase[1, 0] = phase[0, 1]
+    phase[1, 1] = phase[0, 0]
+    phase[2, 2] = s21
+    phase[2, 3] = -d21
+    phase[3, 2] = d21
+    phase[3, 3] = s21
+
+    return phase.squeeze()
+
+
 def mie_cdf(m, x, num, norm='albedo'):
     """
     Create a CDF for unpolarized scattering uniformly spaced in cos(theta).
 
     The CDF covers scattered (exit) angles ranging from 180 to 0 degrees.
     (The cosines are uniformly distributed over -1 to 1.) Because the angles
     are uniformly distributed in cos(theta), the scattering function is not
```

### Comparing `miepython-2.3.2/miepython/miepython_nojit.py` & `miepython-2.4.0/miepython/miepython_nojit.py`

 * *Files 4% similar despite different names*

```diff
@@ -45,14 +45,15 @@
 __all__ = ('ez_mie',
            'ez_intensities',
            'i_par',
            'i_per',
            'i_unpolarized',
            'mie',
            'mie_S1_S2',
+           'mie_phase_matrix',
            'mie_cdf',
            'mie_mu_with_uniform_cdf',
            'generate_mie_costheta',
            )
 
 
 def _Lentz_Dn(z, N):
@@ -552,14 +553,60 @@
 
     S1 /= normalization
     S2 /= normalization
 
     return [S1, S2]
 
 
+def mie_phase_matrix(m, x, mu, norm='albedo'):
+    """
+    Calculate the scattering (Mueller) matrix.
+
+    If mu has length N, then the returned matrix is 4x4xN.  If mu is a scalar
+    then the matrix is 4x4
+
+    The phase scattering matrix is computed from the scattering amplitude
+    functions, according to equations 5.2.105-6 in K. N. Liou (**2002**) -
+    *An Introduction to Atmospheric Radiation*, Second Edition.
+
+    or
+
+    Bohren and Huffman, *Absorption and Scattering of Light by Small Particles*,
+    JOHN WILEY & SONS, page 112, (1983).
+
+    Args:
+        m: the complex index of refraction of the sphere
+        x: the size parameter of the sphere
+        mu: the angles, cos(theta), of the phase scattering matrix
+
+    Returns:
+        p: the phase scattering matrix [sr**(-1.0)]
+    """
+    mu = np.atleast_1d(mu)
+    s1, s2 = mie_S1_S2(m=m, x=x, mu=mu, norm=norm)
+
+    s1_star = np.conjugate(s1)
+    s2_star = np.conjugate(s2)
+    m1 = (s1 * s1_star).real
+    m2 = (s2 * s2_star).real
+    s21 = (0.5 * (s1 * s2_star + s2 * s1_star)).real
+    d21 = (-0.5j * (s1 * s2_star - s2 * s1_star)).real
+    phase = np.zeros(shape=(4, 4, mu.size))
+    phase[0, 0] = 0.5 * (m2 + m1)
+    phase[0, 1] = 0.5 * (m2 - m1)
+    phase[1, 0] = phase[0, 1]
+    phase[1, 1] = phase[0, 0]
+    phase[2, 2] = s21
+    phase[2, 3] = -d21
+    phase[3, 2] = d21
+    phase[3, 3] = s21
+
+    return phase.squeeze()
+
+
 def mie_cdf(m, x, num, norm='albedo'):
     """
     Create a CDF for unpolarized scattering uniformly spaced in cos(theta).
 
     The CDF covers scattered (exit) angles ranging from 180 to 0 degrees.
     (The cosines are uniformly distributed over -1 to 1.) Because the angles
     are uniformly distributed in cos(theta), the scattering function is not
```

### Comparing `miepython-2.3.2/miepython.egg-info/PKG-INFO` & `miepython-2.4.0/miepython.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: miepython
-Version: 2.3.2
+Version: 2.4.0
 Summary: Mie scattering of a plane wave by a sphere
 Home-page: https://github.com/scottprahl/miepython.git
 Author: Scott Prahl
 Author-email: scott.prahl@oit.edu
 License: MIT
 Keywords: mie,scattering,rainbow,droplet,backscatter,sphere,nanoparticle,sphere,cloud,phase function,efficiency,rayleigh,backscattering
 Classifier: Development Status :: 5 - Production/Stable
@@ -21,23 +21,17 @@
 =========
 
 by Scott Prahl
 
 .. image:: https://img.shields.io/pypi/v/miepython.svg
    :target: https://pypi.org/project/miepython/
 
-.. image:: https://colab.research.google.com/assets/colab-badge.svg
-   :target: https://colab.research.google.com/github/scottprahl/miepython/blob/master
-
 .. image:: https://img.shields.io/badge/readthedocs-latest-blue.svg
    :target: https://miepython.readthedocs.io
 
-.. image:: https://img.shields.io/badge/github-code-green.svg
-   :target: https://github.com/scottprahl/miepython
-
 .. image:: https://img.shields.io/badge/MIT-license-yellow.svg
    :target: https://github.com/scottprahl/miepython/blob/master/LICENSE.txt
 
 .. image:: https://github.com/scottprahl/miepython/actions/workflows/test.yml/badge.svg
    :target: https://github.com/scottprahl/miepython/actions/workflows/test.yml
 
 .. image:: https://zenodo.org/badge/99259684.svg
```

### Comparing `miepython-2.3.2/miepython.egg-info/SOURCES.txt` & `miepython-2.4.0/miepython.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `miepython-2.3.2/pyproject.toml` & `miepython-2.4.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `miepython-2.3.2/release.txt` & `miepython-2.4.0/release.txt`

 * *Files identical despite different names*

### Comparing `miepython-2.3.2/setup.cfg` & `miepython-2.4.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `miepython-2.3.2/setup.py` & `miepython-2.4.0/setup.py`

 * *Files identical despite different names*

