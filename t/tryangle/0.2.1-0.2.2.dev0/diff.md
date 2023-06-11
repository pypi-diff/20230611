# Comparing `tmp/tryangle-0.2.1.tar.gz` & `tmp/tryangle-0.2.2.dev0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tryangle-0.2.1.tar", last modified: Wed Apr 20 08:35:45 2022, max compression
+gzip compressed data, was "tryangle-0.2.2.dev0.tar", last modified: Sun Jun 11 17:56:33 2023, max compression
```

## Comparing `tryangle-0.2.1.tar` & `tryangle-0.2.2.dev0.tar`

### file list

```diff
@@ -1,43 +1,49 @@
-drwxrwxrwx   0        0        0        0 2022-04-20 08:35:45.990283 tryangle-0.2.1/
--rw-rw-rw-   0        0        0    17096 2022-04-19 12:54:43.000000 tryangle-0.2.1/LICENSE
--rw-rw-rw-   0        0        0      345 2022-04-19 12:54:43.000000 tryangle-0.2.1/MANIFEST.in
--rw-rw-rw-   0        0        0     3374 2022-04-20 08:35:45.989284 tryangle-0.2.1/PKG-INFO
--rw-rw-rw-   0        0        0     2624 2022-04-20 08:33:11.000000 tryangle-0.2.1/README.rst
--rw-rw-rw-   0        0        0       53 2022-04-20 08:32:20.000000 tryangle-0.2.1/requirements.txt
--rw-rw-rw-   0        0        0       42 2022-04-20 08:35:45.990283 tryangle-0.2.1/setup.cfg
--rw-rw-rw-   0        0        0     1574 2022-04-20 08:31:32.000000 tryangle-0.2.1/setup.py
-drwxrwxrwx   0        0        0        0 2022-04-20 08:35:45.954286 tryangle-0.2.1/src/
-drwxrwxrwx   0        0        0        0 2022-04-20 08:35:45.961285 tryangle-0.2.1/src/tryangle/
--rw-rw-rw-   0        0        0      333 2022-04-20 08:29:33.000000 tryangle-0.2.1/src/tryangle/__init__.py
-drwxrwxrwx   0        0        0        0 2022-04-20 08:35:45.974287 tryangle-0.2.1/src/tryangle/core/
--rw-rw-rw-   0        0        0      597 2022-04-20 08:29:14.000000 tryangle-0.2.1/src/tryangle/core/__init__.py
--rw-rw-rw-   0        0        0     2200 2022-04-20 08:30:19.000000 tryangle-0.2.1/src/tryangle/core/base.py
--rw-rw-rw-   0        0        0     5623 2022-04-20 08:12:22.000000 tryangle-0.2.1/src/tryangle/core/methods.py
-drwxrwxrwx   0        0        0        0 2022-04-20 08:35:45.978284 tryangle-0.2.1/src/tryangle/ensemble/
--rw-rw-rw-   0        0        0      615 2022-04-20 08:29:14.000000 tryangle-0.2.1/src/tryangle/ensemble/__init__.py
--rw-rw-rw-   0        0        0    16515 2022-04-19 13:26:21.000000 tryangle-0.2.1/src/tryangle/ensemble/base.py
--rw-rw-rw-   0        0        0      840 2022-04-20 08:29:14.000000 tryangle-0.2.1/src/tryangle/ensemble/losses.py
--rw-rw-rw-   0        0        0     8312 2022-04-20 08:29:14.000000 tryangle-0.2.1/src/tryangle/ensemble/optimizers.py
-drwxrwxrwx   0        0        0        0 2022-04-20 08:35:45.980286 tryangle-0.2.1/src/tryangle/metrics/
--rw-rw-rw-   0        0        0      551 2022-04-20 08:29:14.000000 tryangle-0.2.1/src/tryangle/metrics/__init__.py
--rw-rw-rw-   0        0        0     1405 2022-04-20 08:29:14.000000 tryangle-0.2.1/src/tryangle/metrics/base.py
--rw-rw-rw-   0        0        0     3027 2022-04-20 08:29:14.000000 tryangle-0.2.1/src/tryangle/metrics/score.py
-drwxrwxrwx   0        0        0        0 2022-04-20 08:35:45.982284 tryangle-0.2.1/src/tryangle/model_selection/
--rw-rw-rw-   0        0        0      400 2022-04-20 08:29:14.000000 tryangle-0.2.1/src/tryangle/model_selection/__init__.py
--rw-rw-rw-   0        0        0     1576 2022-04-19 12:54:43.000000 tryangle-0.2.1/src/tryangle/model_selection/split.py
-drwxrwxrwx   0        0        0        0 2022-04-20 08:35:45.983284 tryangle-0.2.1/src/tryangle/utils/
--rw-rw-rw-   0        0        0      279 2022-04-19 12:54:43.000000 tryangle-0.2.1/src/tryangle/utils/__init__.py
-drwxrwxrwx   0        0        0        0 2022-04-20 08:35:45.988284 tryangle-0.2.1/src/tryangle/utils/data/
--rw-rw-rw-   0        0        0     8372 2022-04-19 12:54:43.000000 tryangle-0.2.1/src/tryangle/utils/data/cas_test.csv
--rw-rw-rw-   0        0        0    10154 2022-04-19 12:54:43.000000 tryangle-0.2.1/src/tryangle/utils/data/cas_train.csv
--rw-rw-rw-   0        0        0     8388 2022-04-19 12:54:43.000000 tryangle-0.2.1/src/tryangle/utils/data/sme_test.csv
--rw-rw-rw-   0        0        0    10370 2022-04-19 12:54:43.000000 tryangle-0.2.1/src/tryangle/utils/data/sme_train.csv
--rw-rw-rw-   0        0        0     8473 2022-04-19 12:54:43.000000 tryangle-0.2.1/src/tryangle/utils/data/swiss_test.csv
--rw-rw-rw-   0        0        0     4793 2022-04-19 12:54:43.000000 tryangle-0.2.1/src/tryangle/utils/data/swiss_train.csv
--rw-rw-rw-   0        0        0     2613 2022-04-20 08:21:23.000000 tryangle-0.2.1/src/tryangle/utils/datasets.py
-drwxrwxrwx   0        0        0        0 2022-04-20 08:35:45.972284 tryangle-0.2.1/src/tryangle.egg-info/
--rw-rw-rw-   0        0        0     3374 2022-04-20 08:35:45.000000 tryangle-0.2.1/src/tryangle.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      939 2022-04-20 08:35:45.000000 tryangle-0.2.1/src/tryangle.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-04-20 08:35:45.000000 tryangle-0.2.1/src/tryangle.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       52 2022-04-20 08:35:45.000000 tryangle-0.2.1/src/tryangle.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2022-04-20 08:35:45.000000 tryangle-0.2.1/src/tryangle.egg-info/top_level.txt
+drwxr-xr-x   0 cb        (1000) cb        (1000)        0 2023-06-11 17:56:33.047664 tryangle-0.2.2.dev0/
+-rw-r--r--   0 cb        (1000) cb        (1000)    16724 2023-06-10 18:49:01.000000 tryangle-0.2.2.dev0/LICENSE
+-rw-r--r--   0 cb        (1000) cb        (1000)      336 2023-06-10 18:49:01.000000 tryangle-0.2.2.dev0/MANIFEST.in
+-rw-r--r--   0 cb        (1000) cb        (1000)     3148 2023-06-11 17:56:33.047664 tryangle-0.2.2.dev0/PKG-INFO
+-rw-r--r--   0 cb        (1000) cb        (1000)     2385 2023-06-10 19:52:36.000000 tryangle-0.2.2.dev0/README.md
+-rw-r--r--   0 cb        (1000) cb        (1000)      991 2023-06-11 17:56:21.000000 tryangle-0.2.2.dev0/pyproject.toml
+-rw-r--r--   0 cb        (1000) cb        (1000)     1355 2023-06-11 17:32:19.000000 tryangle-0.2.2.dev0/requirements.txt
+-rw-r--r--   0 cb        (1000) cb        (1000)       38 2023-06-11 17:56:33.047664 tryangle-0.2.2.dev0/setup.cfg
+drwxr-xr-x   0 cb        (1000) cb        (1000)        0 2023-06-11 17:56:33.037664 tryangle-0.2.2.dev0/src/
+drwxr-xr-x   0 cb        (1000) cb        (1000)        0 2023-06-11 17:56:33.037664 tryangle-0.2.2.dev0/src/tryangle/
+-rw-r--r--   0 cb        (1000) cb        (1000)      330 2023-06-11 17:56:26.000000 tryangle-0.2.2.dev0/src/tryangle/__init__.py
+drwxr-xr-x   0 cb        (1000) cb        (1000)        0 2023-06-11 17:56:33.047664 tryangle-0.2.2.dev0/src/tryangle/core/
+-rw-r--r--   0 cb        (1000) cb        (1000)      581 2023-06-10 18:49:01.000000 tryangle-0.2.2.dev0/src/tryangle/core/__init__.py
+-rw-r--r--   0 cb        (1000) cb        (1000)     2146 2023-06-10 18:49:01.000000 tryangle-0.2.2.dev0/src/tryangle/core/base.py
+-rw-r--r--   0 cb        (1000) cb        (1000)     5435 2023-06-10 18:49:01.000000 tryangle-0.2.2.dev0/src/tryangle/core/methods.py
+drwxr-xr-x   0 cb        (1000) cb        (1000)        0 2023-06-11 17:56:33.047664 tryangle-0.2.2.dev0/src/tryangle/ensemble/
+-rw-r--r--   0 cb        (1000) cb        (1000)      596 2023-06-10 18:49:01.000000 tryangle-0.2.2.dev0/src/tryangle/ensemble/__init__.py
+-rw-r--r--   0 cb        (1000) cb        (1000)    16047 2023-06-10 18:49:01.000000 tryangle-0.2.2.dev0/src/tryangle/ensemble/base.py
+-rw-r--r--   0 cb        (1000) cb        (1000)      810 2023-06-10 18:49:01.000000 tryangle-0.2.2.dev0/src/tryangle/ensemble/losses.py
+-rw-r--r--   0 cb        (1000) cb        (1000)     8055 2023-06-10 18:49:01.000000 tryangle-0.2.2.dev0/src/tryangle/ensemble/optimizers.py
+drwxr-xr-x   0 cb        (1000) cb        (1000)        0 2023-06-11 17:56:33.047664 tryangle-0.2.2.dev0/src/tryangle/metrics/
+-rw-r--r--   0 cb        (1000) cb        (1000)      536 2023-06-10 18:49:01.000000 tryangle-0.2.2.dev0/src/tryangle/metrics/__init__.py
+-rw-r--r--   0 cb        (1000) cb        (1000)     1362 2023-06-10 18:49:01.000000 tryangle-0.2.2.dev0/src/tryangle/metrics/base.py
+-rw-r--r--   0 cb        (1000) cb        (1000)     2946 2023-06-10 18:49:01.000000 tryangle-0.2.2.dev0/src/tryangle/metrics/score.py
+drwxr-xr-x   0 cb        (1000) cb        (1000)        0 2023-06-11 17:56:33.047664 tryangle-0.2.2.dev0/src/tryangle/model_selection/
+-rw-r--r--   0 cb        (1000) cb        (1000)      391 2023-06-10 18:49:01.000000 tryangle-0.2.2.dev0/src/tryangle/model_selection/__init__.py
+-rw-r--r--   0 cb        (1000) cb        (1000)     1543 2023-06-10 18:49:01.000000 tryangle-0.2.2.dev0/src/tryangle/model_selection/split.py
+drwxr-xr-x   0 cb        (1000) cb        (1000)        0 2023-06-11 17:56:33.047664 tryangle-0.2.2.dev0/src/tryangle/utils/
+-rw-r--r--   0 cb        (1000) cb        (1000)      272 2023-06-10 18:49:01.000000 tryangle-0.2.2.dev0/src/tryangle/utils/__init__.py
+drwxr-xr-x   0 cb        (1000) cb        (1000)        0 2023-06-11 17:56:33.047664 tryangle-0.2.2.dev0/src/tryangle/utils/data/
+-rw-r--r--   0 cb        (1000) cb        (1000)     8161 2023-06-10 18:49:01.000000 tryangle-0.2.2.dev0/src/tryangle/utils/data/cas_test.csv
+-rw-r--r--   0 cb        (1000) cb        (1000)     9943 2023-06-10 18:49:01.000000 tryangle-0.2.2.dev0/src/tryangle/utils/data/cas_train.csv
+-rw-r--r--   0 cb        (1000) cb        (1000)     8177 2023-06-10 18:49:01.000000 tryangle-0.2.2.dev0/src/tryangle/utils/data/sme_test.csv
+-rw-r--r--   0 cb        (1000) cb        (1000)    10159 2023-06-10 18:49:01.000000 tryangle-0.2.2.dev0/src/tryangle/utils/data/sme_train.csv
+-rw-r--r--   0 cb        (1000) cb        (1000)     8082 2023-06-10 18:49:01.000000 tryangle-0.2.2.dev0/src/tryangle/utils/data/swiss_test.csv
+-rw-r--r--   0 cb        (1000) cb        (1000)     4602 2023-06-10 18:49:01.000000 tryangle-0.2.2.dev0/src/tryangle/utils/data/swiss_train.csv
+-rw-r--r--   0 cb        (1000) cb        (1000)     2521 2023-06-10 18:49:01.000000 tryangle-0.2.2.dev0/src/tryangle/utils/datasets.py
+drwxr-xr-x   0 cb        (1000) cb        (1000)        0 2023-06-11 17:56:33.047664 tryangle-0.2.2.dev0/src/tryangle.egg-info/
+-rw-r--r--   0 cb        (1000) cb        (1000)     3148 2023-06-11 17:56:33.000000 tryangle-0.2.2.dev0/src/tryangle.egg-info/PKG-INFO
+-rw-r--r--   0 cb        (1000) cb        (1000)     1052 2023-06-11 17:56:33.000000 tryangle-0.2.2.dev0/src/tryangle.egg-info/SOURCES.txt
+-rw-r--r--   0 cb        (1000) cb        (1000)        1 2023-06-11 17:56:33.000000 tryangle-0.2.2.dev0/src/tryangle.egg-info/dependency_links.txt
+-rw-r--r--   0 cb        (1000) cb        (1000)       89 2023-06-11 17:56:33.000000 tryangle-0.2.2.dev0/src/tryangle.egg-info/requires.txt
+-rw-r--r--   0 cb        (1000) cb        (1000)        9 2023-06-11 17:56:33.000000 tryangle-0.2.2.dev0/src/tryangle.egg-info/top_level.txt
+drwxr-xr-x   0 cb        (1000) cb        (1000)        0 2023-06-11 17:56:33.047664 tryangle-0.2.2.dev0/tests/
+-rw-r--r--   0 cb        (1000) cb        (1000)     1610 2023-06-10 18:49:01.000000 tryangle-0.2.2.dev0/tests/test_datasets.py
+-rw-r--r--   0 cb        (1000) cb        (1000)     2714 2023-06-10 18:49:01.000000 tryangle-0.2.2.dev0/tests/test_ensemble.py
+-rw-r--r--   0 cb        (1000) cb        (1000)     1853 2023-06-10 18:49:01.000000 tryangle-0.2.2.dev0/tests/test_methods.py
+-rw-r--r--   0 cb        (1000) cb        (1000)      876 2023-06-10 18:49:01.000000 tryangle-0.2.2.dev0/tests/test_score.py
+-rw-r--r--   0 cb        (1000) cb        (1000)     1444 2023-06-10 18:49:01.000000 tryangle-0.2.2.dev0/tests/test_split.py
```

### Comparing `tryangle-0.2.1/LICENSE` & `tryangle-0.2.2.dev0/LICENSE`

 * *Ordering differences only*

 * *Files 7% similar despite different names*

```diff
@@ -1,373 +1,373 @@
-Mozilla Public License Version 2.0
-==================================
-
-1. Definitions
---------------
-
-1.1. "Contributor"
-    means each individual or legal entity that creates, contributes to
-    the creation of, or owns Covered Software.
-
-1.2. "Contributor Version"
-    means the combination of the Contributions of others (if any) used
-    by a Contributor and that particular Contributor's Contribution.
-
-1.3. "Contribution"
-    means Covered Software of a particular Contributor.
-
-1.4. "Covered Software"
-    means Source Code Form to which the initial Contributor has attached
-    the notice in Exhibit A, the Executable Form of such Source Code
-    Form, and Modifications of such Source Code Form, in each case
-    including portions thereof.
-
-1.5. "Incompatible With Secondary Licenses"
-    means
-
-    (a) that the initial Contributor has attached the notice described
-        in Exhibit B to the Covered Software; or
-
-    (b) that the Covered Software was made available under the terms of
-        version 1.1 or earlier of the License, but not also under the
-        terms of a Secondary License.
-
-1.6. "Executable Form"
-    means any form of the work other than Source Code Form.
-
-1.7. "Larger Work"
-    means a work that combines Covered Software with other material, in
-    a separate file or files, that is not Covered Software.
-
-1.8. "License"
-    means this document.
-
-1.9. "Licensable"
-    means having the right to grant, to the maximum extent possible,
-    whether at the time of the initial grant or subsequently, any and
-    all of the rights conveyed by this License.
-
-1.10. "Modifications"
-    means any of the following:
-
-    (a) any file in Source Code Form that results from an addition to,
-        deletion from, or modification of the contents of Covered
-        Software; or
-
-    (b) any new file in Source Code Form that contains any Covered
-        Software.
-
-1.11. "Patent Claims" of a Contributor
-    means any patent claim(s), including without limitation, method,
-    process, and apparatus claims, in any patent Licensable by such
-    Contributor that would be infringed, but for the grant of the
-    License, by the making, using, selling, offering for sale, having
-    made, import, or transfer of either its Contributions or its
-    Contributor Version.
-
-1.12. "Secondary License"
-    means either the GNU General Public License, Version 2.0, the GNU
-    Lesser General Public License, Version 2.1, the GNU Affero General
-    Public License, Version 3.0, or any later versions of those
-    licenses.
-
-1.13. "Source Code Form"
-    means the form of the work preferred for making modifications.
-
-1.14. "You" (or "Your")
-    means an individual or a legal entity exercising rights under this
-    License. For legal entities, "You" includes any entity that
-    controls, is controlled by, or is under common control with You. For
-    purposes of this definition, "control" means (a) the power, direct
-    or indirect, to cause the direction or management of such entity,
-    whether by contract or otherwise, or (b) ownership of more than
-    fifty percent (50%) of the outstanding shares or beneficial
-    ownership of such entity.
-
-2. License Grants and Conditions
---------------------------------
-
-2.1. Grants
-
-Each Contributor hereby grants You a world-wide, royalty-free,
-non-exclusive license:
-
-(a) under intellectual property rights (other than patent or trademark)
-    Licensable by such Contributor to use, reproduce, make available,
-    modify, display, perform, distribute, and otherwise exploit its
-    Contributions, either on an unmodified basis, with Modifications, or
-    as part of a Larger Work; and
-
-(b) under Patent Claims of such Contributor to make, use, sell, offer
-    for sale, have made, import, and otherwise transfer either its
-    Contributions or its Contributor Version.
-
-2.2. Effective Date
-
-The licenses granted in Section 2.1 with respect to any Contribution
-become effective for each Contribution on the date the Contributor first
-distributes such Contribution.
-
-2.3. Limitations on Grant Scope
-
-The licenses granted in this Section 2 are the only rights granted under
-this License. No additional rights or licenses will be implied from the
-distribution or licensing of Covered Software under this License.
-Notwithstanding Section 2.1(b) above, no patent license is granted by a
-Contributor:
-
-(a) for any code that a Contributor has removed from Covered Software;
-    or
-
-(b) for infringements caused by: (i) Your and any other third party's
-    modifications of Covered Software, or (ii) the combination of its
-    Contributions with other software (except as part of its Contributor
-    Version); or
-
-(c) under Patent Claims infringed by Covered Software in the absence of
-    its Contributions.
-
-This License does not grant any rights in the trademarks, service marks,
-or logos of any Contributor (except as may be necessary to comply with
-the notice requirements in Section 3.4).
-
-2.4. Subsequent Licenses
-
-No Contributor makes additional grants as a result of Your choice to
-distribute the Covered Software under a subsequent version of this
-License (see Section 10.2) or under the terms of a Secondary License (if
-permitted under the terms of Section 3.3).
-
-2.5. Representation
-
-Each Contributor represents that the Contributor believes its
-Contributions are its original creation(s) or it has sufficient rights
-to grant the rights to its Contributions conveyed by this License.
-
-2.6. Fair Use
-
-This License is not intended to limit any rights You have under
-applicable copyright doctrines of fair use, fair dealing, or other
-equivalents.
-
-2.7. Conditions
-
-Sections 3.1, 3.2, 3.3, and 3.4 are conditions of the licenses granted
-in Section 2.1.
-
-3. Responsibilities
--------------------
-
-3.1. Distribution of Source Form
-
-All distribution of Covered Software in Source Code Form, including any
-Modifications that You create or to which You contribute, must be under
-the terms of this License. You must inform recipients that the Source
-Code Form of the Covered Software is governed by the terms of this
-License, and how they can obtain a copy of this License. You may not
-attempt to alter or restrict the recipients' rights in the Source Code
-Form.
-
-3.2. Distribution of Executable Form
-
-If You distribute Covered Software in Executable Form then:
-
-(a) such Covered Software must also be made available in Source Code
-    Form, as described in Section 3.1, and You must inform recipients of
-    the Executable Form how they can obtain a copy of such Source Code
-    Form by reasonable means in a timely manner, at a charge no more
-    than the cost of distribution to the recipient; and
-
-(b) You may distribute such Executable Form under the terms of this
-    License, or sublicense it under different terms, provided that the
-    license for the Executable Form does not attempt to limit or alter
-    the recipients' rights in the Source Code Form under this License.
-
-3.3. Distribution of a Larger Work
-
-You may create and distribute a Larger Work under terms of Your choice,
-provided that You also comply with the requirements of this License for
-the Covered Software. If the Larger Work is a combination of Covered
-Software with a work governed by one or more Secondary Licenses, and the
-Covered Software is not Incompatible With Secondary Licenses, this
-License permits You to additionally distribute such Covered Software
-under the terms of such Secondary License(s), so that the recipient of
-the Larger Work may, at their option, further distribute the Covered
-Software under the terms of either this License or such Secondary
-License(s).
-
-3.4. Notices
-
-You may not remove or alter the substance of any license notices
-(including copyright notices, patent notices, disclaimers of warranty,
-or limitations of liability) contained within the Source Code Form of
-the Covered Software, except that You may alter any license notices to
-the extent required to remedy known factual inaccuracies.
-
-3.5. Application of Additional Terms
-
-You may choose to offer, and to charge a fee for, warranty, support,
-indemnity or liability obligations to one or more recipients of Covered
-Software. However, You may do so only on Your own behalf, and not on
-behalf of any Contributor. You must make it absolutely clear that any
-such warranty, support, indemnity, or liability obligation is offered by
-You alone, and You hereby agree to indemnify every Contributor for any
-liability incurred by such Contributor as a result of warranty, support,
-indemnity or liability terms You offer. You may include additional
-disclaimers of warranty and limitations of liability specific to any
-jurisdiction.
-
-4. Inability to Comply Due to Statute or Regulation
----------------------------------------------------
-
-If it is impossible for You to comply with any of the terms of this
-License with respect to some or all of the Covered Software due to
-statute, judicial order, or regulation then You must: (a) comply with
-the terms of this License to the maximum extent possible; and (b)
-describe the limitations and the code they affect. Such description must
-be placed in a text file included with all distributions of the Covered
-Software under this License. Except to the extent prohibited by statute
-or regulation, such description must be sufficiently detailed for a
-recipient of ordinary skill to be able to understand it.
-
-5. Termination
---------------
-
-5.1. The rights granted under this License will terminate automatically
-if You fail to comply with any of its terms. However, if You become
-compliant, then the rights granted under this License from a particular
-Contributor are reinstated (a) provisionally, unless and until such
-Contributor explicitly and finally terminates Your grants, and (b) on an
-ongoing basis, if such Contributor fails to notify You of the
-non-compliance by some reasonable means prior to 60 days after You have
-come back into compliance. Moreover, Your grants from a particular
-Contributor are reinstated on an ongoing basis if such Contributor
-notifies You of the non-compliance by some reasonable means, this is the
-first time You have received notice of non-compliance with this License
-from such Contributor, and You become compliant prior to 30 days after
-Your receipt of the notice.
-
-5.2. If You initiate litigation against any entity by asserting a patent
-infringement claim (excluding declaratory judgment actions,
-counter-claims, and cross-claims) alleging that a Contributor Version
-directly or indirectly infringes any patent, then the rights granted to
-You by any and all Contributors for the Covered Software under Section
-2.1 of this License shall terminate.
-
-5.3. In the event of termination under Sections 5.1 or 5.2 above, all
-end user license agreements (excluding distributors and resellers) which
-have been validly granted by You or Your distributors under this License
-prior to termination shall survive termination.
-
-************************************************************************
-*                                                                      *
-*  6. Disclaimer of Warranty                                           *
-*  -------------------------                                           *
-*                                                                      *
-*  Covered Software is provided under this License on an "as is"       *
-*  basis, without warranty of any kind, either expressed, implied, or  *
-*  statutory, including, without limitation, warranties that the       *
-*  Covered Software is free of defects, merchantable, fit for a        *
-*  particular purpose or non-infringing. The entire risk as to the     *
-*  quality and performance of the Covered Software is with You.        *
-*  Should any Covered Software prove defective in any respect, You     *
-*  (not any Contributor) assume the cost of any necessary servicing,   *
-*  repair, or correction. This disclaimer of warranty constitutes an   *
-*  essential part of this License. No use of any Covered Software is   *
-*  authorized under this License except under this disclaimer.         *
-*                                                                      *
-************************************************************************
-
-************************************************************************
-*                                                                      *
-*  7. Limitation of Liability                                          *
-*  --------------------------                                          *
-*                                                                      *
-*  Under no circumstances and under no legal theory, whether tort      *
-*  (including negligence), contract, or otherwise, shall any           *
-*  Contributor, or anyone who distributes Covered Software as          *
-*  permitted above, be liable to You for any direct, indirect,         *
-*  special, incidental, or consequential damages of any character      *
-*  including, without limitation, damages for lost profits, loss of    *
-*  goodwill, work stoppage, computer failure or malfunction, or any    *
-*  and all other commercial damages or losses, even if such party      *
-*  shall have been informed of the possibility of such damages. This   *
-*  limitation of liability shall not apply to liability for death or   *
-*  personal injury resulting from such party's negligence to the       *
-*  extent applicable law prohibits such limitation. Some               *
-*  jurisdictions do not allow the exclusion or limitation of           *
-*  incidental or consequential damages, so this exclusion and          *
-*  limitation may not apply to You.                                    *
-*                                                                      *
-************************************************************************
-
-8. Litigation
--------------
-
-Any litigation relating to this License may be brought only in the
-courts of a jurisdiction where the defendant maintains its principal
-place of business and such litigation shall be governed by laws of that
-jurisdiction, without reference to its conflict-of-law provisions.
-Nothing in this Section shall prevent a party's ability to bring
-cross-claims or counter-claims.
-
-9. Miscellaneous
-----------------
-
-This License represents the complete agreement concerning the subject
-matter hereof. If any provision of this License is held to be
-unenforceable, such provision shall be reformed only to the extent
-necessary to make it enforceable. Any law or regulation which provides
-that the language of a contract shall be construed against the drafter
-shall not be used to construe this License against a Contributor.
-
-10. Versions of the License
----------------------------
-
-10.1. New Versions
-
-Mozilla Foundation is the license steward. Except as provided in Section
-10.3, no one other than the license steward has the right to modify or
-publish new versions of this License. Each version will be given a
-distinguishing version number.
-
-10.2. Effect of New Versions
-
-You may distribute the Covered Software under the terms of the version
-of the License under which You originally received the Covered Software,
-or under the terms of any subsequent version published by the license
-steward.
-
-10.3. Modified Versions
-
-If you create software not governed by this License, and you want to
-create a new license for such software, you may create and use a
-modified version of this License if you rename the license and remove
-any references to the name of the license steward (except to note that
-such modified license differs from this License).
-
-10.4. Distributing Source Code Form that is Incompatible With Secondary
-Licenses
-
-If You choose to distribute Source Code Form that is Incompatible With
-Secondary Licenses under the terms of this version of the License, the
-notice described in Exhibit B of this License must be attached.
-
-Exhibit A - Source Code Form License Notice
--------------------------------------------
-
-  This Source Code Form is subject to the terms of the Mozilla Public
-  License, v. 2.0. If a copy of the MPL was not distributed with this
-  file, You can obtain one at http://mozilla.org/MPL/2.0/.
-
-If it is not possible or desirable to put the notice in a particular
-file, then You may include the notice in a location (such as a LICENSE
-file in a relevant directory) where a recipient would be likely to look
-for such a notice.
-
-You may add additional accurate notices of copyright ownership.
-
-Exhibit B - "Incompatible With Secondary Licenses" Notice
----------------------------------------------------------
-
-  This Source Code Form is "Incompatible With Secondary Licenses", as
+Mozilla Public License Version 2.0
+==================================
+
+1. Definitions
+--------------
+
+1.1. "Contributor"
+    means each individual or legal entity that creates, contributes to
+    the creation of, or owns Covered Software.
+
+1.2. "Contributor Version"
+    means the combination of the Contributions of others (if any) used
+    by a Contributor and that particular Contributor's Contribution.
+
+1.3. "Contribution"
+    means Covered Software of a particular Contributor.
+
+1.4. "Covered Software"
+    means Source Code Form to which the initial Contributor has attached
+    the notice in Exhibit A, the Executable Form of such Source Code
+    Form, and Modifications of such Source Code Form, in each case
+    including portions thereof.
+
+1.5. "Incompatible With Secondary Licenses"
+    means
+
+    (a) that the initial Contributor has attached the notice described
+        in Exhibit B to the Covered Software; or
+
+    (b) that the Covered Software was made available under the terms of
+        version 1.1 or earlier of the License, but not also under the
+        terms of a Secondary License.
+
+1.6. "Executable Form"
+    means any form of the work other than Source Code Form.
+
+1.7. "Larger Work"
+    means a work that combines Covered Software with other material, in
+    a separate file or files, that is not Covered Software.
+
+1.8. "License"
+    means this document.
+
+1.9. "Licensable"
+    means having the right to grant, to the maximum extent possible,
+    whether at the time of the initial grant or subsequently, any and
+    all of the rights conveyed by this License.
+
+1.10. "Modifications"
+    means any of the following:
+
+    (a) any file in Source Code Form that results from an addition to,
+        deletion from, or modification of the contents of Covered
+        Software; or
+
+    (b) any new file in Source Code Form that contains any Covered
+        Software.
+
+1.11. "Patent Claims" of a Contributor
+    means any patent claim(s), including without limitation, method,
+    process, and apparatus claims, in any patent Licensable by such
+    Contributor that would be infringed, but for the grant of the
+    License, by the making, using, selling, offering for sale, having
+    made, import, or transfer of either its Contributions or its
+    Contributor Version.
+
+1.12. "Secondary License"
+    means either the GNU General Public License, Version 2.0, the GNU
+    Lesser General Public License, Version 2.1, the GNU Affero General
+    Public License, Version 3.0, or any later versions of those
+    licenses.
+
+1.13. "Source Code Form"
+    means the form of the work preferred for making modifications.
+
+1.14. "You" (or "Your")
+    means an individual or a legal entity exercising rights under this
+    License. For legal entities, "You" includes any entity that
+    controls, is controlled by, or is under common control with You. For
+    purposes of this definition, "control" means (a) the power, direct
+    or indirect, to cause the direction or management of such entity,
+    whether by contract or otherwise, or (b) ownership of more than
+    fifty percent (50%) of the outstanding shares or beneficial
+    ownership of such entity.
+
+2. License Grants and Conditions
+--------------------------------
+
+2.1. Grants
+
+Each Contributor hereby grants You a world-wide, royalty-free,
+non-exclusive license:
+
+(a) under intellectual property rights (other than patent or trademark)
+    Licensable by such Contributor to use, reproduce, make available,
+    modify, display, perform, distribute, and otherwise exploit its
+    Contributions, either on an unmodified basis, with Modifications, or
+    as part of a Larger Work; and
+
+(b) under Patent Claims of such Contributor to make, use, sell, offer
+    for sale, have made, import, and otherwise transfer either its
+    Contributions or its Contributor Version.
+
+2.2. Effective Date
+
+The licenses granted in Section 2.1 with respect to any Contribution
+become effective for each Contribution on the date the Contributor first
+distributes such Contribution.
+
+2.3. Limitations on Grant Scope
+
+The licenses granted in this Section 2 are the only rights granted under
+this License. No additional rights or licenses will be implied from the
+distribution or licensing of Covered Software under this License.
+Notwithstanding Section 2.1(b) above, no patent license is granted by a
+Contributor:
+
+(a) for any code that a Contributor has removed from Covered Software;
+    or
+
+(b) for infringements caused by: (i) Your and any other third party's
+    modifications of Covered Software, or (ii) the combination of its
+    Contributions with other software (except as part of its Contributor
+    Version); or
+
+(c) under Patent Claims infringed by Covered Software in the absence of
+    its Contributions.
+
+This License does not grant any rights in the trademarks, service marks,
+or logos of any Contributor (except as may be necessary to comply with
+the notice requirements in Section 3.4).
+
+2.4. Subsequent Licenses
+
+No Contributor makes additional grants as a result of Your choice to
+distribute the Covered Software under a subsequent version of this
+License (see Section 10.2) or under the terms of a Secondary License (if
+permitted under the terms of Section 3.3).
+
+2.5. Representation
+
+Each Contributor represents that the Contributor believes its
+Contributions are its original creation(s) or it has sufficient rights
+to grant the rights to its Contributions conveyed by this License.
+
+2.6. Fair Use
+
+This License is not intended to limit any rights You have under
+applicable copyright doctrines of fair use, fair dealing, or other
+equivalents.
+
+2.7. Conditions
+
+Sections 3.1, 3.2, 3.3, and 3.4 are conditions of the licenses granted
+in Section 2.1.
+
+3. Responsibilities
+-------------------
+
+3.1. Distribution of Source Form
+
+All distribution of Covered Software in Source Code Form, including any
+Modifications that You create or to which You contribute, must be under
+the terms of this License. You must inform recipients that the Source
+Code Form of the Covered Software is governed by the terms of this
+License, and how they can obtain a copy of this License. You may not
+attempt to alter or restrict the recipients' rights in the Source Code
+Form.
+
+3.2. Distribution of Executable Form
+
+If You distribute Covered Software in Executable Form then:
+
+(a) such Covered Software must also be made available in Source Code
+    Form, as described in Section 3.1, and You must inform recipients of
+    the Executable Form how they can obtain a copy of such Source Code
+    Form by reasonable means in a timely manner, at a charge no more
+    than the cost of distribution to the recipient; and
+
+(b) You may distribute such Executable Form under the terms of this
+    License, or sublicense it under different terms, provided that the
+    license for the Executable Form does not attempt to limit or alter
+    the recipients' rights in the Source Code Form under this License.
+
+3.3. Distribution of a Larger Work
+
+You may create and distribute a Larger Work under terms of Your choice,
+provided that You also comply with the requirements of this License for
+the Covered Software. If the Larger Work is a combination of Covered
+Software with a work governed by one or more Secondary Licenses, and the
+Covered Software is not Incompatible With Secondary Licenses, this
+License permits You to additionally distribute such Covered Software
+under the terms of such Secondary License(s), so that the recipient of
+the Larger Work may, at their option, further distribute the Covered
+Software under the terms of either this License or such Secondary
+License(s).
+
+3.4. Notices
+
+You may not remove or alter the substance of any license notices
+(including copyright notices, patent notices, disclaimers of warranty,
+or limitations of liability) contained within the Source Code Form of
+the Covered Software, except that You may alter any license notices to
+the extent required to remedy known factual inaccuracies.
+
+3.5. Application of Additional Terms
+
+You may choose to offer, and to charge a fee for, warranty, support,
+indemnity or liability obligations to one or more recipients of Covered
+Software. However, You may do so only on Your own behalf, and not on
+behalf of any Contributor. You must make it absolutely clear that any
+such warranty, support, indemnity, or liability obligation is offered by
+You alone, and You hereby agree to indemnify every Contributor for any
+liability incurred by such Contributor as a result of warranty, support,
+indemnity or liability terms You offer. You may include additional
+disclaimers of warranty and limitations of liability specific to any
+jurisdiction.
+
+4. Inability to Comply Due to Statute or Regulation
+---------------------------------------------------
+
+If it is impossible for You to comply with any of the terms of this
+License with respect to some or all of the Covered Software due to
+statute, judicial order, or regulation then You must: (a) comply with
+the terms of this License to the maximum extent possible; and (b)
+describe the limitations and the code they affect. Such description must
+be placed in a text file included with all distributions of the Covered
+Software under this License. Except to the extent prohibited by statute
+or regulation, such description must be sufficiently detailed for a
+recipient of ordinary skill to be able to understand it.
+
+5. Termination
+--------------
+
+5.1. The rights granted under this License will terminate automatically
+if You fail to comply with any of its terms. However, if You become
+compliant, then the rights granted under this License from a particular
+Contributor are reinstated (a) provisionally, unless and until such
+Contributor explicitly and finally terminates Your grants, and (b) on an
+ongoing basis, if such Contributor fails to notify You of the
+non-compliance by some reasonable means prior to 60 days after You have
+come back into compliance. Moreover, Your grants from a particular
+Contributor are reinstated on an ongoing basis if such Contributor
+notifies You of the non-compliance by some reasonable means, this is the
+first time You have received notice of non-compliance with this License
+from such Contributor, and You become compliant prior to 30 days after
+Your receipt of the notice.
+
+5.2. If You initiate litigation against any entity by asserting a patent
+infringement claim (excluding declaratory judgment actions,
+counter-claims, and cross-claims) alleging that a Contributor Version
+directly or indirectly infringes any patent, then the rights granted to
+You by any and all Contributors for the Covered Software under Section
+2.1 of this License shall terminate.
+
+5.3. In the event of termination under Sections 5.1 or 5.2 above, all
+end user license agreements (excluding distributors and resellers) which
+have been validly granted by You or Your distributors under this License
+prior to termination shall survive termination.
+
+************************************************************************
+*                                                                      *
+*  6. Disclaimer of Warranty                                           *
+*  -------------------------                                           *
+*                                                                      *
+*  Covered Software is provided under this License on an "as is"       *
+*  basis, without warranty of any kind, either expressed, implied, or  *
+*  statutory, including, without limitation, warranties that the       *
+*  Covered Software is free of defects, merchantable, fit for a        *
+*  particular purpose or non-infringing. The entire risk as to the     *
+*  quality and performance of the Covered Software is with You.        *
+*  Should any Covered Software prove defective in any respect, You     *
+*  (not any Contributor) assume the cost of any necessary servicing,   *
+*  repair, or correction. This disclaimer of warranty constitutes an   *
+*  essential part of this License. No use of any Covered Software is   *
+*  authorized under this License except under this disclaimer.         *
+*                                                                      *
+************************************************************************
+
+************************************************************************
+*                                                                      *
+*  7. Limitation of Liability                                          *
+*  --------------------------                                          *
+*                                                                      *
+*  Under no circumstances and under no legal theory, whether tort      *
+*  (including negligence), contract, or otherwise, shall any           *
+*  Contributor, or anyone who distributes Covered Software as          *
+*  permitted above, be liable to You for any direct, indirect,         *
+*  special, incidental, or consequential damages of any character      *
+*  including, without limitation, damages for lost profits, loss of    *
+*  goodwill, work stoppage, computer failure or malfunction, or any    *
+*  and all other commercial damages or losses, even if such party      *
+*  shall have been informed of the possibility of such damages. This   *
+*  limitation of liability shall not apply to liability for death or   *
+*  personal injury resulting from such party's negligence to the       *
+*  extent applicable law prohibits such limitation. Some               *
+*  jurisdictions do not allow the exclusion or limitation of           *
+*  incidental or consequential damages, so this exclusion and          *
+*  limitation may not apply to You.                                    *
+*                                                                      *
+************************************************************************
+
+8. Litigation
+-------------
+
+Any litigation relating to this License may be brought only in the
+courts of a jurisdiction where the defendant maintains its principal
+place of business and such litigation shall be governed by laws of that
+jurisdiction, without reference to its conflict-of-law provisions.
+Nothing in this Section shall prevent a party's ability to bring
+cross-claims or counter-claims.
+
+9. Miscellaneous
+----------------
+
+This License represents the complete agreement concerning the subject
+matter hereof. If any provision of this License is held to be
+unenforceable, such provision shall be reformed only to the extent
+necessary to make it enforceable. Any law or regulation which provides
+that the language of a contract shall be construed against the drafter
+shall not be used to construe this License against a Contributor.
+
+10. Versions of the License
+---------------------------
+
+10.1. New Versions
+
+Mozilla Foundation is the license steward. Except as provided in Section
+10.3, no one other than the license steward has the right to modify or
+publish new versions of this License. Each version will be given a
+distinguishing version number.
+
+10.2. Effect of New Versions
+
+You may distribute the Covered Software under the terms of the version
+of the License under which You originally received the Covered Software,
+or under the terms of any subsequent version published by the license
+steward.
+
+10.3. Modified Versions
+
+If you create software not governed by this License, and you want to
+create a new license for such software, you may create and use a
+modified version of this License if you rename the license and remove
+any references to the name of the license steward (except to note that
+such modified license differs from this License).
+
+10.4. Distributing Source Code Form that is Incompatible With Secondary
+Licenses
+
+If You choose to distribute Source Code Form that is Incompatible With
+Secondary Licenses under the terms of this version of the License, the
+notice described in Exhibit B of this License must be attached.
+
+Exhibit A - Source Code Form License Notice
+-------------------------------------------
+
+  This Source Code Form is subject to the terms of the Mozilla Public
+  License, v. 2.0. If a copy of the MPL was not distributed with this
+  file, You can obtain one at http://mozilla.org/MPL/2.0/.
+
+If it is not possible or desirable to put the notice in a particular
+file, then You may include the notice in a location (such as a LICENSE
+file in a relevant directory) where a recipient would be likely to look
+for such a notice.
+
+You may add additional accurate notices of copyright ownership.
+
+Exhibit B - "Incompatible With Secondary Licenses" Notice
+---------------------------------------------------------
+
+  This Source Code Form is "Incompatible With Secondary Licenses", as
   defined by the Mozilla Public License, v. 2.0.
```

### Comparing `tryangle-0.2.1/src/tryangle/core/base.py` & `tryangle-0.2.2.dev0/src/tryangle/core/base.py`

 * *Ordering differences only*

 * *Files 19% similar despite different names*

```diff
@@ -1,54 +1,54 @@
-# This Source Code Form is subject to the terms of the Mozilla Public
-# License, v. 2.0. If a copy of the MPL was not distributed with this
-# file, You can obtain one at https://mozilla.org/MPL/2.0/.
-
-import numpy as np
-
-
-class TryangleData:
-    """
-    TryangleData is an internal data structure used by Tryangle which is built
-    to work with optimization libraries to allow hyperparameter optimization
-    and parallel processing.
-
-    TryangleData can only hold chainladder ``Triangle``'s that are singular in
-    the first and second axis. That is, the shape of the ``Triangle`` must be
-    (1, 1, n_origin, n_development). The sample_weight must also be singular
-    in its development axis, i.e. a shape of (1, 1, n_origin, 1).
-
-    Parameters
-    ----------
-    triangle : chainladder ``Triangle`` object of shape (1, 1, n_origin, n_development)
-        The loss triangle to be reserved.
-
-    sample_weight : chainladder ``Triangle`` object of shape (1, 1, n_origin, 1), default=None
-        The exposure data for exposure based methods.
-    """
-
-    def __init__(self, triangle, sample_weight=None):
-        self.triangle = triangle
-        self.sample_weight = sample_weight
-        self.shape = self.triangle.shape[2] * self.triangle.shape[3], 1
-        self.latest_diagonal = triangle.cum_to_incr().latest_diagonal
-        if self.latest_diagonal.shape != ():
-            self.actual = self.latest_diagonal[
-                self.latest_diagonal.origin < self.latest_diagonal.origin[-1]
-            ]
-
-    def __getitem__(self, x):
-        indices = np.full((self.shape[0],), False)
-        indices[x] = True
-        spliced_triangle = self.triangle[indices]
-        if self.sample_weight is not None:
-            sample_weight_indices = np.array(
-                [
-                    origin in spliced_triangle.origin
-                    for origin in self.sample_weight.origin
-                ]
-            )
-            return TryangleData(
-                self.triangle[indices],
-                self.sample_weight[sample_weight_indices],
-            )
-        else:
-            return TryangleData(self.triangle[indices], None)
+# This Source Code Form is subject to the terms of the Mozilla Public
+# License, v. 2.0. If a copy of the MPL was not distributed with this
+# file, You can obtain one at https://mozilla.org/MPL/2.0/.
+
+import numpy as np
+
+
+class TryangleData:
+    """
+    TryangleData is an internal data structure used by Tryangle which is built
+    to work with optimization libraries to allow hyperparameter optimization
+    and parallel processing.
+
+    TryangleData can only hold chainladder ``Triangle``'s that are singular in
+    the first and second axis. That is, the shape of the ``Triangle`` must be
+    (1, 1, n_origin, n_development). The sample_weight must also be singular
+    in its development axis, i.e. a shape of (1, 1, n_origin, 1).
+
+    Parameters
+    ----------
+    triangle : chainladder ``Triangle`` object of shape (1, 1, n_origin, n_development)
+        The loss triangle to be reserved.
+
+    sample_weight : chainladder ``Triangle`` object of shape (1, 1, n_origin, 1), default=None
+        The exposure data for exposure based methods.
+    """
+
+    def __init__(self, triangle, sample_weight=None):
+        self.triangle = triangle
+        self.sample_weight = sample_weight
+        self.shape = self.triangle.shape[2] * self.triangle.shape[3], 1
+        self.latest_diagonal = triangle.cum_to_incr().latest_diagonal
+        if self.latest_diagonal.shape != ():
+            self.actual = self.latest_diagonal[
+                self.latest_diagonal.origin < self.latest_diagonal.origin[-1]
+            ]
+
+    def __getitem__(self, x):
+        indices = np.full((self.shape[0],), False)
+        indices[x] = True
+        spliced_triangle = self.triangle[indices]
+        if self.sample_weight is not None:
+            sample_weight_indices = np.array(
+                [
+                    origin in spliced_triangle.origin
+                    for origin in self.sample_weight.origin
+                ]
+            )
+            return TryangleData(
+                self.triangle[indices],
+                self.sample_weight[sample_weight_indices],
+            )
+        else:
+            return TryangleData(self.triangle[indices], None)
```

### Comparing `tryangle-0.2.1/src/tryangle/core/methods.py` & `tryangle-0.2.2.dev0/src/tryangle/core/methods.py`

 * *Ordering differences only*

 * *Files 21% similar despite different names*

```diff
@@ -1,188 +1,188 @@
-# This Source Code Form is subject to the terms of the Mozilla Public
-# License, v. 2.0. If a copy of the MPL was not distributed with this
-# file, You can obtain one at https://mozilla.org/MPL/2.0/.
-
-from chainladder.development.clark import ClarkLDF as _cl_ClarkLDF
-from chainladder.development.constant import (
-    DevelopmentConstant as _cl_DevelopmentConstant,
-)
-from chainladder.development.development import Development as _cl_Development
-from chainladder.development.incremental import (
-    IncrementalAdditive as _cl_IncrementalAdditive,
-)
-from chainladder.methods.benktander import Benktander as _cl_Benktander
-from chainladder.methods.bornferg import BornhuetterFerguson as _cl_BornhuetterFerguson
-from chainladder.methods.capecod import CapeCod as _cl_CapeCod
-from chainladder.methods.chainladder import Chainladder as _cl_Chainladder
-from chainladder.methods.mack import MackChainladder as _cl_MackChainladder
-from chainladder.workflow.voting import VotingChainladder as _cl_VotingChainladder
-from tryangle.core.base import TryangleData
-
-
-class EstimatorMixin:
-    """
-    Fit and predict a chainladder estimator
-    """
-
-    def fit(self, X, y=None, sample_weight=None):
-        return super().fit(X.triangle, y=None, sample_weight=X.sample_weight)
-
-    def predict(self, X, sample_weight=None):
-        return super().predict(X.triangle, sample_weight=X.sample_weight)
-
-    def fit_predict(self, X, sample_weight=None):
-        self.fit(X)
-        return self.predict(X)
-
-
-class TransformerMixin:
-    """
-    Fit and transform a chainladder transfomer
-    """
-
-    def fit(self, X, y=None, sample_weight=None):
-        return super().fit(X.triangle, y=None, sample_weight=X.sample_weight)
-
-    def transform(self, X):
-        return TryangleData(super().transform(X.triangle), X.sample_weight)
-
-
-class Development(TransformerMixin, _cl_Development):
-    __doc__ = _cl_Development.__doc__
-
-    def __init__(
-        self,
-        n_periods=-1,
-        average="volume",
-        sigma_interpolation="log-linear",
-        drop=None,
-        drop_high=None,
-        drop_low=None,
-        drop_valuation=None,
-        fillna=None,
-    ):
-        super().__init__(
-            n_periods=n_periods,
-            average=average,
-            sigma_interpolation=sigma_interpolation,
-            drop=drop,
-            drop_high=drop_high,
-            drop_low=drop_low,
-            drop_valuation=drop_valuation,
-            fillna=fillna,
-        )
-
-
-class DevelopmentConstant(TransformerMixin, _cl_DevelopmentConstant):
-    __doc__ = _cl_DevelopmentConstant.__doc__
-
-    def __init__(
-        self,
-        patterns=None,
-        style="ldf",
-        callable_axis=0,
-    ):
-        super().__init__(
-            patterns=patterns,
-            style=style,
-            callable_axis=callable_axis,
-        )
-
-
-class IncrementalAdditive(TransformerMixin, _cl_IncrementalAdditive):
-    __doc__ = _cl_IncrementalAdditive.__doc__
-
-    def __init__(
-        self,
-        trend=0.0,
-        n_periods=-1,
-        average="volume",
-        future_trend=0,
-        drop=None,
-        drop_high=None,
-        drop_low=None,
-        drop_valuation=None,
-    ):
-        super().__init__(
-            trend=trend,
-            n_periods=n_periods,
-            average=average,
-            future_trend=future_trend,
-            drop=drop,
-            drop_high=drop_high,
-            drop_low=drop_low,
-            drop_valuation=drop_valuation,
-        )
-
-
-class ClarkLDF(TransformerMixin, _cl_ClarkLDF):
-    __doc__ = _cl_ClarkLDF.__doc__
-
-    def __init__(self, growth="loglogistic"):
-        super().__init__(
-            growth=growth,
-        )
-
-
-class Chainladder(EstimatorMixin, _cl_Chainladder):
-    __doc__ = _cl_Chainladder.__doc__
-
-
-class MackChainladder(EstimatorMixin, _cl_MackChainladder):
-    __doc__ = _cl_MackChainladder.__doc__
-
-
-class BornhuetterFerguson(EstimatorMixin, _cl_BornhuetterFerguson):
-    __doc__ = _cl_BornhuetterFerguson.__doc__
-
-    def __init__(self, apriori=1.0, apriori_sigma=0.0, random_state=None):
-        super().__init__(
-            apriori=apriori, apriori_sigma=apriori_sigma, random_state=random_state
-        )
-
-
-class CapeCod(EstimatorMixin, _cl_CapeCod):
-    __doc__ = _cl_CapeCod.__doc__
-
-    def __init__(self, trend=0, decay=1):
-        super().__init__(trend=trend, decay=decay)
-
-
-class Benktander(EstimatorMixin, _cl_Benktander):
-    __doc__ = _cl_Benktander.__doc__
-
-    def __init__(self, apriori=1.0, n_iters=1, apriori_sigma=0, random_state=None):
-        super().__init__(
-            apriori=apriori,
-            n_iters=n_iters,
-            apriori_sigma=apriori_sigma,
-            random_state=random_state,
-        )
-
-
-class VotingChainladder(EstimatorMixin, _cl_VotingChainladder):
-    __doc__ = _cl_VotingChainladder.__doc__
-
-    def __init__(
-        self,
-        estimators,
-        weights=None,
-        default_weighting=None,
-        n_jobs=None,
-        verbose=False,
-    ):
-        # Convert tryangle estimators to chainladder estimators
-        estimators = [
-            (
-                name,
-                globals()["_cl_" + estimator.__class__.__name__](**estimator.__dict__),
-            )
-            for name, estimator in estimators
-        ]
-        super().__init__(
-            estimators=estimators,
-            weights=weights,
-            default_weighting=default_weighting,
-            n_jobs=n_jobs,
-            verbose=verbose,
-        )
+# This Source Code Form is subject to the terms of the Mozilla Public
+# License, v. 2.0. If a copy of the MPL was not distributed with this
+# file, You can obtain one at https://mozilla.org/MPL/2.0/.
+
+from chainladder.development.clark import ClarkLDF as _cl_ClarkLDF
+from chainladder.development.constant import (
+    DevelopmentConstant as _cl_DevelopmentConstant,
+)
+from chainladder.development.development import Development as _cl_Development
+from chainladder.development.incremental import (
+    IncrementalAdditive as _cl_IncrementalAdditive,
+)
+from chainladder.methods.benktander import Benktander as _cl_Benktander
+from chainladder.methods.bornferg import BornhuetterFerguson as _cl_BornhuetterFerguson
+from chainladder.methods.capecod import CapeCod as _cl_CapeCod
+from chainladder.methods.chainladder import Chainladder as _cl_Chainladder
+from chainladder.methods.mack import MackChainladder as _cl_MackChainladder
+from chainladder.workflow.voting import VotingChainladder as _cl_VotingChainladder
+from tryangle.core.base import TryangleData
+
+
+class EstimatorMixin:
+    """
+    Fit and predict a chainladder estimator
+    """
+
+    def fit(self, X, y=None, sample_weight=None):
+        return super().fit(X.triangle, y=None, sample_weight=X.sample_weight)
+
+    def predict(self, X, sample_weight=None):
+        return super().predict(X.triangle, sample_weight=X.sample_weight)
+
+    def fit_predict(self, X, sample_weight=None):
+        self.fit(X)
+        return self.predict(X)
+
+
+class TransformerMixin:
+    """
+    Fit and transform a chainladder transfomer
+    """
+
+    def fit(self, X, y=None, sample_weight=None):
+        return super().fit(X.triangle, y=None, sample_weight=X.sample_weight)
+
+    def transform(self, X):
+        return TryangleData(super().transform(X.triangle), X.sample_weight)
+
+
+class Development(TransformerMixin, _cl_Development):
+    __doc__ = _cl_Development.__doc__
+
+    def __init__(
+        self,
+        n_periods=-1,
+        average="volume",
+        sigma_interpolation="log-linear",
+        drop=None,
+        drop_high=None,
+        drop_low=None,
+        drop_valuation=None,
+        fillna=None,
+    ):
+        super().__init__(
+            n_periods=n_periods,
+            average=average,
+            sigma_interpolation=sigma_interpolation,
+            drop=drop,
+            drop_high=drop_high,
+            drop_low=drop_low,
+            drop_valuation=drop_valuation,
+            fillna=fillna,
+        )
+
+
+class DevelopmentConstant(TransformerMixin, _cl_DevelopmentConstant):
+    __doc__ = _cl_DevelopmentConstant.__doc__
+
+    def __init__(
+        self,
+        patterns=None,
+        style="ldf",
+        callable_axis=0,
+    ):
+        super().__init__(
+            patterns=patterns,
+            style=style,
+            callable_axis=callable_axis,
+        )
+
+
+class IncrementalAdditive(TransformerMixin, _cl_IncrementalAdditive):
+    __doc__ = _cl_IncrementalAdditive.__doc__
+
+    def __init__(
+        self,
+        trend=0.0,
+        n_periods=-1,
+        average="volume",
+        future_trend=0,
+        drop=None,
+        drop_high=None,
+        drop_low=None,
+        drop_valuation=None,
+    ):
+        super().__init__(
+            trend=trend,
+            n_periods=n_periods,
+            average=average,
+            future_trend=future_trend,
+            drop=drop,
+            drop_high=drop_high,
+            drop_low=drop_low,
+            drop_valuation=drop_valuation,
+        )
+
+
+class ClarkLDF(TransformerMixin, _cl_ClarkLDF):
+    __doc__ = _cl_ClarkLDF.__doc__
+
+    def __init__(self, growth="loglogistic"):
+        super().__init__(
+            growth=growth,
+        )
+
+
+class Chainladder(EstimatorMixin, _cl_Chainladder):
+    __doc__ = _cl_Chainladder.__doc__
+
+
+class MackChainladder(EstimatorMixin, _cl_MackChainladder):
+    __doc__ = _cl_MackChainladder.__doc__
+
+
+class BornhuetterFerguson(EstimatorMixin, _cl_BornhuetterFerguson):
+    __doc__ = _cl_BornhuetterFerguson.__doc__
+
+    def __init__(self, apriori=1.0, apriori_sigma=0.0, random_state=None):
+        super().__init__(
+            apriori=apriori, apriori_sigma=apriori_sigma, random_state=random_state
+        )
+
+
+class CapeCod(EstimatorMixin, _cl_CapeCod):
+    __doc__ = _cl_CapeCod.__doc__
+
+    def __init__(self, trend=0, decay=1):
+        super().__init__(trend=trend, decay=decay)
+
+
+class Benktander(EstimatorMixin, _cl_Benktander):
+    __doc__ = _cl_Benktander.__doc__
+
+    def __init__(self, apriori=1.0, n_iters=1, apriori_sigma=0, random_state=None):
+        super().__init__(
+            apriori=apriori,
+            n_iters=n_iters,
+            apriori_sigma=apriori_sigma,
+            random_state=random_state,
+        )
+
+
+class VotingChainladder(EstimatorMixin, _cl_VotingChainladder):
+    __doc__ = _cl_VotingChainladder.__doc__
+
+    def __init__(
+        self,
+        estimators,
+        weights=None,
+        default_weighting=None,
+        n_jobs=None,
+        verbose=False,
+    ):
+        # Convert tryangle estimators to chainladder estimators
+        estimators = [
+            (
+                name,
+                globals()["_cl_" + estimator.__class__.__name__](**estimator.__dict__),
+            )
+            for name, estimator in estimators
+        ]
+        super().__init__(
+            estimators=estimators,
+            weights=weights,
+            default_weighting=default_weighting,
+            n_jobs=n_jobs,
+            verbose=verbose,
+        )
```

### Comparing `tryangle-0.2.1/src/tryangle/ensemble/base.py` & `tryangle-0.2.2.dev0/src/tryangle/ensemble/base.py`

 * *Ordering differences only*

 * *Files 22% similar despite different names*

```diff
@@ -1,468 +1,468 @@
-# This Source Code Form is subject to the terms of the Mozilla Public
-# License, v. 2.0. If a copy of the MPL was not distributed with this
-# file, You can obtain one at https://mozilla.org/MPL/2.0/.
-
-import numpy as np
-from chainladder.workflow.voting import _BaseTriangleEnsemble
-from sklearn.base import clone
-from sklearn.ensemble._base import _fit_single_estimator
-from sklearn.utils.validation import _deprecate_positional_args
-from tryangle.ensemble.optimizers import Adam
-from tryangle.metrics.base import get_expected
-from tryangle.ensemble.losses import LOSS_FUNCTIONS
-
-
-class AutoEnsemble(_BaseTriangleEnsemble):
-    """Automated ensembling of chainladder methods
-
-    `AutoEnsemble` uses a neural network to find optimal weights
-    to ensemble multiple chainladder methods.
-
-    Read more in the :ref:`User Guide <autoensemble>`
-
-    .. versionadded:: 0.1.0
-
-    Parameters
-    ----------
-    estimators : list of (str, estimator) tuples
-        Invoking the ``fit`` method on the ``AutoEnsemble`` will fit clones
-        of those original estimators across the cv folds of the triangle and
-        store the expected incremental claims for the next diagonal for each
-        of the folds.
-
-    cv : `TriangleSplit` cross-validation generator
-        Determines the number of cross-validation folds
-        over which to fit. Must be an instance of `TriangleSplit`
-
-        Refer :ref:`User Guide <cross_validation>`
-
-    max_iter : int, default=1000
-        Maximum number of iterations (or epochs) used to train the neural
-        network. Currently the optimizers use all iterations.
-
-    optimizer : optimizer object, default=Adam()
-        The optimization method to find optimal weights and biases.
-
-    initial_weight : ndarray of shape (1, num_estimators), default=None
-        Force the initial weights instead of using a random initialization
-
-    initial_bias : ndarray of shape (1, num_estimators), default=None
-        Force the initial biases instead of using a random initialization
-
-    weight_function : 'linear', 'poly(n)', or None, default='linear'
-        Specify a function to constrain the voting weights.
-        ``poly(n)`` will fit an n-term polynomial:
-        t^n * w + t^(n-1) * w + ... + t^(2) * w + t * w + b
-        where t is the origin period, w is the weight, and b is the bias
-        ``linear`` is equivalent to ``poly(1)``
-        ``None`` will not constrain the weights meaning each origin period
-        will have its own vector of weights.
-
-    random_state : int or None, default=None
-        Specify the seed for random weight and bias initialization.
-
-    n_jobs : int, default=None
-        Number of jobs to run in parallel
-        ``None`` means 1.
-        ``-1`` means using all processors.
-        Currently only the compilation step is run in parallel. Optimization
-        is not.
-
-    verbose : int, default=False
-        Controls the verbosity: the higher, the more messages.
-
-    dropout : float, default=False
-        Randomly sets incremental claim amounts equal to 0 equivalently for
-        actual and expected. That is, the same incremental claims set to
-        zero for actual are set to zero for expected. Parameter is given as
-        a proportion of number of incremental claims data points.
-
-    broad_dropout : float, default=False
-        Randomly sets entire folds to zero equivalently for actual and expected.
-        Parameter is given as a proportion of the number of folds and rounded to
-        the nearest integer.
-
-    Attributes
-    ----------
-
-    actual_ : ndarray
-        The actual incremental claims for each fold.
-
-    expected_ : ndarray
-        The expected incremental claims for each estimator for each fold.
-
-    weights_ : ndarray
-        The optimal weights found to ensemble the estimators.
-
-    Notes
-    -----
-
-    ``AutoEnsemble`` is still experimental and may change with future versions.
-    """
-
-    @_deprecate_positional_args
-    def __init__(
-        self,
-        estimators,
-        cv,
-        max_iter=1000,
-        optimizer=Adam(),
-        initial_weight=None,
-        initial_bias=None,
-        weight_function="linear",
-        loss="mse",
-        random_state=None,
-        n_jobs=None,
-        verbose=False,
-        dropout=False,
-        broad_dropout=False,
-    ):
-        self.estimators = estimators
-        self.cv = cv
-        self.max_iter = max_iter
-        self.optimizer = optimizer
-        self.initial_weight = initial_weight
-        self.initial_bias = initial_bias
-        self.weight_function = weight_function
-        self.loss = loss
-        self.random_state = random_state
-        self.n_jobs = n_jobs
-        self.verbose = verbose
-        self.dropout = dropout
-        self.broad_dropout = broad_dropout
-
-    def _log_message(self, name, idx, total):
-        if self.verbose < 2:
-            return None
-        return "(%d of %d) Processing %s" % (idx, total, name)
-
-    def initialize_weights(self):
-        if self.weight_function is None:
-            weight_dim = self.origin_dim
-        elif self.weight_function == "linear":
-            weight_dim = 1
-        elif "poly" in self.weight_function:
-            self.weight_polynomial = int(
-                self.weight_function[
-                    self.weight_function.find("(") + 1 : self.weight_function.find(")")
-                ]
-            )
-            weight_dim = 1
-        else:
-            raise Exception(
-                "Unknown weight function provided. Options are None, linear, or poly(n)."
-            )
-
-        if self.initial_weight is None:
-            np.random.seed(self.random_state)
-            self.weights = np.random.normal(
-                0,
-                np.sqrt(2 / (2 * len(self.estimators))),
-                size=(weight_dim, len(self.estimators)),
-            )
-        else:
-            self.weights = self.initial_weight
-        if self.initial_bias is None:
-            np.random.seed(self.random_state)
-            self.biases = np.zeros((weight_dim, len(self.estimators)))
-        else:
-            self.biases = self.initial_bias
-
-    def preprocess(self, X, y=None, sample_weight=None):
-        """
-        In order to find optimal weights, the actual incremental claims
-        and expected incremental claims for each estimator is required.
-        This method also returns the `t` array.
-        """
-
-        names, clfs = self._validate_estimators()
-
-        actual = X.latest_diagonal.to_frame().fillna(0).to_numpy()[:-1]
-        actual = actual[np.newaxis, ...]
-        expected = np.array(
-            [
-                get_expected(
-                    _fit_single_estimator(
-                        clone(clf),
-                        X,
-                        X,
-                        sample_weight=None,
-                        message_clsname=f"Preprocessing - {names[idx]}_expected",
-                        message=self._log_message(names[idx], idx + 1, len(clfs)),
-                    ),
-                    X,
-                )
-                for idx, clf in enumerate(clfs)
-            ]
-        )
-
-        t = (
-            np.arange(1, actual.shape[1] + 1).reshape(-1, 1)[np.newaxis, ...]
-            / actual.shape[1]
-        )
-
-        return actual, expected, t
-
-    def compile(self, X, y=None, sample_weight=None):
-        """
-        Obtain the actual, expected, and t, arrays for each estimator
-        for each fold and reshape for input to the neural network.
-        """
-        # Fit individual estimators
-        if self.verbose > 1:
-            print("\n[Compiling]\n")
-
-        names, clfs = self._validate_estimators()
-
-        self.actual_ = []
-        self.expected_ = []
-
-        # Preprocessing for each fold
-        for fold, (train, _) in enumerate(self.cv.split(X)):
-
-            zeros_to_pad = self.cv.n_splits - fold
-
-            fold_actual, fold_expected, _ = self.preprocess(X[train])
-
-            # Pad actuals to have same shape
-            fold_actual = np.pad(
-                fold_actual,
-                [
-                    [0, 0],
-                    [zeros_to_pad, 0],
-                    [0, 0],
-                ],
-            )
-
-            self.actual_.append(fold_actual)
-
-            # Pad expecteds to have same shape
-            fold_expected = np.pad(
-                fold_expected,
-                [
-                    [0, 0],
-                    [zeros_to_pad, 0],
-                    [0, 0],
-                ],
-            )
-
-            self.expected_.append(fold_expected)
-
-        self.actual_ = np.concatenate(self.actual_, axis=0)
-        self.expected_ = np.concatenate(self.expected_, axis=2).T
-        self.t_ = (
-            np.repeat(
-                np.arange(1, self.actual_.shape[1] + 1).reshape(-1, 1)[np.newaxis, ...],
-                self.cv.n_splits,
-                axis=0,
-            )
-            / self.actual_.shape[1]
-        )
-        self._output = np.zeros(self.actual_.shape)
-        self.origin_dim = self.actual_.shape[1]
-
-        if self.verbose:
-            print()
-
-        return self
-
-    def _softmax(self, x):
-        return np.exp(x) / np.exp(x).sum(axis=2, keepdims=True)
-
-    def _softmax_gradient(self, x):
-        identity = np.repeat(
-            np.repeat(np.eye(x.shape[2])[np.newaxis, ...], x.shape[1], axis=0)[
-                np.newaxis, ...
-            ],
-            x.shape[0],
-            axis=0,
-        )
-        lhs_jacobian = identity * self._softmax(x)[..., np.newaxis]
-        rhs_jacobian = np.einsum("fij,kif->fijk", self._softmax(x), self._softmax(x).T)
-        return lhs_jacobian - rhs_jacobian
-
-    def dense(self, t):
-        if self.weight_function is None:
-            return t * self.weights + self.biases
-        elif self.weight_function == "linear":
-            return np.matmul(t, self.weights) + self.biases
-        elif self.weight_function[:4] == "poly":
-            return (
-                sum(
-                    [t ** (n + 1) * self.weights for n in range(self.weight_polynomial)]
-                )
-                + self.biases
-            )
-        else:
-            raise Exception(
-                "Unknown weight function provided. Options are None, linear, or poly(n)."
-            )
-
-    def _dense_gradient(self, t):
-        if self.weight_function is None:
-            return t
-        elif self.weight_function == "linear":
-            return t
-        elif self.weight_function[:4] == "poly":
-            return sum([(n + 1) * t ** (n) for n in range(self.weight_polynomial)])
-        else:
-            raise Exception(
-                "Unknown weight function provided. Options are None, linear, or poly(n)."
-            )
-
-    def activation(self, x):
-        return self._softmax(x)
-
-    def output(self, expected, activation):
-        return (expected * activation).sum(axis=2, keepdims=True)
-
-    def compute_loss(self, output, actual):
-        return self.Loss()._loss(output, actual)
-
-    def forward_pass(self, actual, expected, t, text_file=None):
-        if self.verbose > 2:
-            print("Starting weights: ", self.weights, " ", self.biases, file=text_file)
-        self._dense = self.dense(t)
-        self._activation = self.activation(self._dense)
-        self._output = self.output(expected, self._activation)
-        self._compute_loss = self.compute_loss(self._output, actual)
-        if self.verbose > 2:
-            print("Loss: ", self._compute_loss, file=text_file)
-
-        return self
-
-    def backward_pass(self, actual, expected, t, epoch, text_file):
-        dLdy = self.Loss()._loss_gradient(self._output, actual)
-        dyds = expected
-        dsdd = self._softmax_gradient(self._dense)
-        dddw = self._dense_gradient(t)
-        dddb = np.ones(t.shape)
-
-        dLdd = np.einsum("fkij,fkj->fki", dsdd, dLdy * dyds)
-
-        self._w_grad = (dLdd * dddw).mean(axis=(0, 1))
-        self._b_grad = (dLdd * dddb).mean(axis=(0, 1))
-
-        self.optimizer.pre_update_params(epoch)
-        self.optimizer.update_params(self, epoch)
-
-        if self.verbose > 2:
-            print(
-                "[EPOCH: ",
-                epoch,
-                "]: cust_w_grad: ",
-                self._w_grad,
-                ", cust_b_grad: ",
-                self._b_grad,
-                file=text_file,
-            )
-
-        return self
-
-    def _log_epoch(self, epoch):
-        if not epoch % 10:
-            print(
-                f"[Epoch {epoch}/{self.max_iter}] "
-                + f"loss: {self._loss:.4f} "
-                + f"lr: {self.optimizer._learning_rate:.8f}"
-            )
-
-    def fit(self, X, y=None, sample_weight=None, loss="mse", text_file=None):
-
-        self.compile(X, y, sample_weight)
-        self.Loss = LOSS_FUNCTIONS[self.loss]
-
-        if self.verbose:
-            print("[Training]\n")
-
-        num_folds = self.actual_.shape[0]
-
-        weights = []
-        biases = []
-        eval_losses = []
-
-        for p in range(num_folds):
-
-            actual_train = np.delete(self.actual_, p, axis=0)
-            expected_train = np.delete(self.expected_, p, axis=0)
-            t_train = np.delete(self.t_, p, axis=0)
-
-            actual_test = self.actual_[np.newaxis, p, :, :]
-            expected_test = self.expected_[np.newaxis, p, :, :]
-            t_test = self.t_[np.newaxis, p, :, :]
-
-            self.initialize_weights()
-            self.optimizer.reset(self)
-
-            for epoch in range(self.max_iter + 1):
-                _actual_train = actual_train
-                _expected_train = expected_train
-                _t_train = t_train
-
-                if self.dropout:
-                    drop_mask = np.ones_like(
-                        _actual_train.reshape(-1, _actual_train.shape[-1])
-                    )
-                    choices = list(range(drop_mask.shape[0]))
-                    drop_idx = np.random.choice(
-                        choices, int(len(choices) * self.dropout)
-                    )
-                    drop_mask[drop_idx] = 0
-                    drop_mask = drop_mask.reshape(_actual_train.shape)
-
-                    _actual_train = _actual_train * drop_mask
-                    _expected_train = _expected_train * drop_mask
-
-                if self.broad_dropout:
-                    choices = list(range(_actual_train.shape[0]))
-                    drop_idx = np.random.choice(
-                        choices, int(len(choices) * self.broad_dropout)
-                    )
-                    drop_mask = np.ones_like(_actual_train)
-                    drop_mask[drop_idx, :, :] = 0
-
-                    _actual_train = _actual_train * drop_mask
-                    _expected_train = _expected_train * drop_mask
-
-                self.forward_pass(_actual_train, _expected_train, _t_train, text_file)
-                self.backward_pass(
-                    _actual_train, _expected_train, _t_train, epoch, text_file
-                )
-
-                if self.verbose:
-                    self._log_epoch(epoch)
-
-            weights.append(self.weights)
-            biases.append(self.biases)
-
-            eval_loss = self.compute_loss(
-                self._predict(expected_test, t_test), actual_test
-            )
-            eval_loss = eval_loss / actual_test.mean()
-            eval_losses.append(eval_loss)
-
-        self.weights = np.average(np.stack(weights, axis=1), axis=1)
-        self.biases = np.average(np.stack(biases, axis=1), axis=1)
-
-        self.weights_ = self._activation[-1]
-
-        print()
-        if self.verbose:
-            print("\n")
-
-        return self
-
-    def _predict(self, expected, t):
-        dense = self.dense(t)
-        activation = self.activation(dense)
-        output = self.output(expected, activation)
-        return output
-
-    def predict(self, X, y=None, sample_weight=None):
-        _, expected, t = self.preprocess(X, y, sample_weight)
-        return self._predict(expected, t)
-
-    def evaluate(self, X, y=None, sample_weight=None):
-        actual, expected, t = self.preprocess(X, y, sample_weight)
-        output = self._predict(expected, t)
-        return self.compute_loss(output, actual)
+# This Source Code Form is subject to the terms of the Mozilla Public
+# License, v. 2.0. If a copy of the MPL was not distributed with this
+# file, You can obtain one at https://mozilla.org/MPL/2.0/.
+
+import numpy as np
+from chainladder.workflow.voting import _BaseTriangleEnsemble
+from sklearn.base import clone
+from sklearn.ensemble._base import _fit_single_estimator
+from sklearn.utils.validation import _deprecate_positional_args
+from tryangle.ensemble.optimizers import Adam
+from tryangle.metrics.base import get_expected
+from tryangle.ensemble.losses import LOSS_FUNCTIONS
+
+
+class AutoEnsemble(_BaseTriangleEnsemble):
+    """Automated ensembling of chainladder methods
+
+    `AutoEnsemble` uses a neural network to find optimal weights
+    to ensemble multiple chainladder methods.
+
+    Read more in the :ref:`User Guide <autoensemble>`
+
+    .. versionadded:: 0.1.0
+
+    Parameters
+    ----------
+    estimators : list of (str, estimator) tuples
+        Invoking the ``fit`` method on the ``AutoEnsemble`` will fit clones
+        of those original estimators across the cv folds of the triangle and
+        store the expected incremental claims for the next diagonal for each
+        of the folds.
+
+    cv : `TriangleSplit` cross-validation generator
+        Determines the number of cross-validation folds
+        over which to fit. Must be an instance of `TriangleSplit`
+
+        Refer :ref:`User Guide <cross_validation>`
+
+    max_iter : int, default=1000
+        Maximum number of iterations (or epochs) used to train the neural
+        network. Currently the optimizers use all iterations.
+
+    optimizer : optimizer object, default=Adam()
+        The optimization method to find optimal weights and biases.
+
+    initial_weight : ndarray of shape (1, num_estimators), default=None
+        Force the initial weights instead of using a random initialization
+
+    initial_bias : ndarray of shape (1, num_estimators), default=None
+        Force the initial biases instead of using a random initialization
+
+    weight_function : 'linear', 'poly(n)', or None, default='linear'
+        Specify a function to constrain the voting weights.
+        ``poly(n)`` will fit an n-term polynomial:
+        t^n * w + t^(n-1) * w + ... + t^(2) * w + t * w + b
+        where t is the origin period, w is the weight, and b is the bias
+        ``linear`` is equivalent to ``poly(1)``
+        ``None`` will not constrain the weights meaning each origin period
+        will have its own vector of weights.
+
+    random_state : int or None, default=None
+        Specify the seed for random weight and bias initialization.
+
+    n_jobs : int, default=None
+        Number of jobs to run in parallel
+        ``None`` means 1.
+        ``-1`` means using all processors.
+        Currently only the compilation step is run in parallel. Optimization
+        is not.
+
+    verbose : int, default=False
+        Controls the verbosity: the higher, the more messages.
+
+    dropout : float, default=False
+        Randomly sets incremental claim amounts equal to 0 equivalently for
+        actual and expected. That is, the same incremental claims set to
+        zero for actual are set to zero for expected. Parameter is given as
+        a proportion of number of incremental claims data points.
+
+    broad_dropout : float, default=False
+        Randomly sets entire folds to zero equivalently for actual and expected.
+        Parameter is given as a proportion of the number of folds and rounded to
+        the nearest integer.
+
+    Attributes
+    ----------
+
+    actual_ : ndarray
+        The actual incremental claims for each fold.
+
+    expected_ : ndarray
+        The expected incremental claims for each estimator for each fold.
+
+    weights_ : ndarray
+        The optimal weights found to ensemble the estimators.
+
+    Notes
+    -----
+
+    ``AutoEnsemble`` is still experimental and may change with future versions.
+    """
+
+    @_deprecate_positional_args
+    def __init__(
+        self,
+        estimators,
+        cv,
+        max_iter=1000,
+        optimizer=Adam(),
+        initial_weight=None,
+        initial_bias=None,
+        weight_function="linear",
+        loss="mse",
+        random_state=None,
+        n_jobs=None,
+        verbose=False,
+        dropout=False,
+        broad_dropout=False,
+    ):
+        self.estimators = estimators
+        self.cv = cv
+        self.max_iter = max_iter
+        self.optimizer = optimizer
+        self.initial_weight = initial_weight
+        self.initial_bias = initial_bias
+        self.weight_function = weight_function
+        self.loss = loss
+        self.random_state = random_state
+        self.n_jobs = n_jobs
+        self.verbose = verbose
+        self.dropout = dropout
+        self.broad_dropout = broad_dropout
+
+    def _log_message(self, name, idx, total):
+        if self.verbose < 2:
+            return None
+        return "(%d of %d) Processing %s" % (idx, total, name)
+
+    def initialize_weights(self):
+        if self.weight_function is None:
+            weight_dim = self.origin_dim
+        elif self.weight_function == "linear":
+            weight_dim = 1
+        elif "poly" in self.weight_function:
+            self.weight_polynomial = int(
+                self.weight_function[
+                    self.weight_function.find("(") + 1 : self.weight_function.find(")")
+                ]
+            )
+            weight_dim = 1
+        else:
+            raise Exception(
+                "Unknown weight function provided. Options are None, linear, or poly(n)."
+            )
+
+        if self.initial_weight is None:
+            np.random.seed(self.random_state)
+            self.weights = np.random.normal(
+                0,
+                np.sqrt(2 / (2 * len(self.estimators))),
+                size=(weight_dim, len(self.estimators)),
+            )
+        else:
+            self.weights = self.initial_weight
+        if self.initial_bias is None:
+            np.random.seed(self.random_state)
+            self.biases = np.zeros((weight_dim, len(self.estimators)))
+        else:
+            self.biases = self.initial_bias
+
+    def preprocess(self, X, y=None, sample_weight=None):
+        """
+        In order to find optimal weights, the actual incremental claims
+        and expected incremental claims for each estimator is required.
+        This method also returns the `t` array.
+        """
+
+        names, clfs = self._validate_estimators()
+
+        actual = X.latest_diagonal.to_frame().fillna(0).to_numpy()[:-1]
+        actual = actual[np.newaxis, ...]
+        expected = np.array(
+            [
+                get_expected(
+                    _fit_single_estimator(
+                        clone(clf),
+                        X,
+                        X,
+                        sample_weight=None,
+                        message_clsname=f"Preprocessing - {names[idx]}_expected",
+                        message=self._log_message(names[idx], idx + 1, len(clfs)),
+                    ),
+                    X,
+                )
+                for idx, clf in enumerate(clfs)
+            ]
+        )
+
+        t = (
+            np.arange(1, actual.shape[1] + 1).reshape(-1, 1)[np.newaxis, ...]
+            / actual.shape[1]
+        )
+
+        return actual, expected, t
+
+    def compile(self, X, y=None, sample_weight=None):
+        """
+        Obtain the actual, expected, and t, arrays for each estimator
+        for each fold and reshape for input to the neural network.
+        """
+        # Fit individual estimators
+        if self.verbose > 1:
+            print("\n[Compiling]\n")
+
+        names, clfs = self._validate_estimators()
+
+        self.actual_ = []
+        self.expected_ = []
+
+        # Preprocessing for each fold
+        for fold, (train, _) in enumerate(self.cv.split(X)):
+
+            zeros_to_pad = self.cv.n_splits - fold
+
+            fold_actual, fold_expected, _ = self.preprocess(X[train])
+
+            # Pad actuals to have same shape
+            fold_actual = np.pad(
+                fold_actual,
+                [
+                    [0, 0],
+                    [zeros_to_pad, 0],
+                    [0, 0],
+                ],
+            )
+
+            self.actual_.append(fold_actual)
+
+            # Pad expecteds to have same shape
+            fold_expected = np.pad(
+                fold_expected,
+                [
+                    [0, 0],
+                    [zeros_to_pad, 0],
+                    [0, 0],
+                ],
+            )
+
+            self.expected_.append(fold_expected)
+
+        self.actual_ = np.concatenate(self.actual_, axis=0)
+        self.expected_ = np.concatenate(self.expected_, axis=2).T
+        self.t_ = (
+            np.repeat(
+                np.arange(1, self.actual_.shape[1] + 1).reshape(-1, 1)[np.newaxis, ...],
+                self.cv.n_splits,
+                axis=0,
+            )
+            / self.actual_.shape[1]
+        )
+        self._output = np.zeros(self.actual_.shape)
+        self.origin_dim = self.actual_.shape[1]
+
+        if self.verbose:
+            print()
+
+        return self
+
+    def _softmax(self, x):
+        return np.exp(x) / np.exp(x).sum(axis=2, keepdims=True)
+
+    def _softmax_gradient(self, x):
+        identity = np.repeat(
+            np.repeat(np.eye(x.shape[2])[np.newaxis, ...], x.shape[1], axis=0)[
+                np.newaxis, ...
+            ],
+            x.shape[0],
+            axis=0,
+        )
+        lhs_jacobian = identity * self._softmax(x)[..., np.newaxis]
+        rhs_jacobian = np.einsum("fij,kif->fijk", self._softmax(x), self._softmax(x).T)
+        return lhs_jacobian - rhs_jacobian
+
+    def dense(self, t):
+        if self.weight_function is None:
+            return t * self.weights + self.biases
+        elif self.weight_function == "linear":
+            return np.matmul(t, self.weights) + self.biases
+        elif self.weight_function[:4] == "poly":
+            return (
+                sum(
+                    [t ** (n + 1) * self.weights for n in range(self.weight_polynomial)]
+                )
+                + self.biases
+            )
+        else:
+            raise Exception(
+                "Unknown weight function provided. Options are None, linear, or poly(n)."
+            )
+
+    def _dense_gradient(self, t):
+        if self.weight_function is None:
+            return t
+        elif self.weight_function == "linear":
+            return t
+        elif self.weight_function[:4] == "poly":
+            return sum([(n + 1) * t ** (n) for n in range(self.weight_polynomial)])
+        else:
+            raise Exception(
+                "Unknown weight function provided. Options are None, linear, or poly(n)."
+            )
+
+    def activation(self, x):
+        return self._softmax(x)
+
+    def output(self, expected, activation):
+        return (expected * activation).sum(axis=2, keepdims=True)
+
+    def compute_loss(self, output, actual):
+        return self.Loss()._loss(output, actual)
+
+    def forward_pass(self, actual, expected, t, text_file=None):
+        if self.verbose > 2:
+            print("Starting weights: ", self.weights, " ", self.biases, file=text_file)
+        self._dense = self.dense(t)
+        self._activation = self.activation(self._dense)
+        self._output = self.output(expected, self._activation)
+        self._compute_loss = self.compute_loss(self._output, actual)
+        if self.verbose > 2:
+            print("Loss: ", self._compute_loss, file=text_file)
+
+        return self
+
+    def backward_pass(self, actual, expected, t, epoch, text_file):
+        dLdy = self.Loss()._loss_gradient(self._output, actual)
+        dyds = expected
+        dsdd = self._softmax_gradient(self._dense)
+        dddw = self._dense_gradient(t)
+        dddb = np.ones(t.shape)
+
+        dLdd = np.einsum("fkij,fkj->fki", dsdd, dLdy * dyds)
+
+        self._w_grad = (dLdd * dddw).mean(axis=(0, 1))
+        self._b_grad = (dLdd * dddb).mean(axis=(0, 1))
+
+        self.optimizer.pre_update_params(epoch)
+        self.optimizer.update_params(self, epoch)
+
+        if self.verbose > 2:
+            print(
+                "[EPOCH: ",
+                epoch,
+                "]: cust_w_grad: ",
+                self._w_grad,
+                ", cust_b_grad: ",
+                self._b_grad,
+                file=text_file,
+            )
+
+        return self
+
+    def _log_epoch(self, epoch):
+        if not epoch % 10:
+            print(
+                f"[Epoch {epoch}/{self.max_iter}] "
+                + f"loss: {self._loss:.4f} "
+                + f"lr: {self.optimizer._learning_rate:.8f}"
+            )
+
+    def fit(self, X, y=None, sample_weight=None, loss="mse", text_file=None):
+
+        self.compile(X, y, sample_weight)
+        self.Loss = LOSS_FUNCTIONS[self.loss]
+
+        if self.verbose:
+            print("[Training]\n")
+
+        num_folds = self.actual_.shape[0]
+
+        weights = []
+        biases = []
+        eval_losses = []
+
+        for p in range(num_folds):
+
+            actual_train = np.delete(self.actual_, p, axis=0)
+            expected_train = np.delete(self.expected_, p, axis=0)
+            t_train = np.delete(self.t_, p, axis=0)
+
+            actual_test = self.actual_[np.newaxis, p, :, :]
+            expected_test = self.expected_[np.newaxis, p, :, :]
+            t_test = self.t_[np.newaxis, p, :, :]
+
+            self.initialize_weights()
+            self.optimizer.reset(self)
+
+            for epoch in range(self.max_iter + 1):
+                _actual_train = actual_train
+                _expected_train = expected_train
+                _t_train = t_train
+
+                if self.dropout:
+                    drop_mask = np.ones_like(
+                        _actual_train.reshape(-1, _actual_train.shape[-1])
+                    )
+                    choices = list(range(drop_mask.shape[0]))
+                    drop_idx = np.random.choice(
+                        choices, int(len(choices) * self.dropout)
+                    )
+                    drop_mask[drop_idx] = 0
+                    drop_mask = drop_mask.reshape(_actual_train.shape)
+
+                    _actual_train = _actual_train * drop_mask
+                    _expected_train = _expected_train * drop_mask
+
+                if self.broad_dropout:
+                    choices = list(range(_actual_train.shape[0]))
+                    drop_idx = np.random.choice(
+                        choices, int(len(choices) * self.broad_dropout)
+                    )
+                    drop_mask = np.ones_like(_actual_train)
+                    drop_mask[drop_idx, :, :] = 0
+
+                    _actual_train = _actual_train * drop_mask
+                    _expected_train = _expected_train * drop_mask
+
+                self.forward_pass(_actual_train, _expected_train, _t_train, text_file)
+                self.backward_pass(
+                    _actual_train, _expected_train, _t_train, epoch, text_file
+                )
+
+                if self.verbose:
+                    self._log_epoch(epoch)
+
+            weights.append(self.weights)
+            biases.append(self.biases)
+
+            eval_loss = self.compute_loss(
+                self._predict(expected_test, t_test), actual_test
+            )
+            eval_loss = eval_loss / actual_test.mean()
+            eval_losses.append(eval_loss)
+
+        self.weights = np.average(np.stack(weights, axis=1), axis=1)
+        self.biases = np.average(np.stack(biases, axis=1), axis=1)
+
+        self.weights_ = self._activation[-1]
+
+        print()
+        if self.verbose:
+            print("\n")
+
+        return self
+
+    def _predict(self, expected, t):
+        dense = self.dense(t)
+        activation = self.activation(dense)
+        output = self.output(expected, activation)
+        return output
+
+    def predict(self, X, y=None, sample_weight=None):
+        _, expected, t = self.preprocess(X, y, sample_weight)
+        return self._predict(expected, t)
+
+    def evaluate(self, X, y=None, sample_weight=None):
+        actual, expected, t = self.preprocess(X, y, sample_weight)
+        output = self._predict(expected, t)
+        return self.compute_loss(output, actual)
```

### Comparing `tryangle-0.2.1/src/tryangle/ensemble/optimizers.py` & `tryangle-0.2.2.dev0/src/tryangle/ensemble/optimizers.py`

 * *Ordering differences only*

 * *Files 12% similar despite different names*

```diff
@@ -1,257 +1,257 @@
-# This Source Code Form is subject to the terms of the Mozilla Public
-# License, v. 2.0. If a copy of the MPL was not distributed with this
-# file, You can obtain one at https://mozilla.org/MPL/2.0/.
-
-import numpy as np
-
-
-class SGD:
-    """
-    Stochastic Gradient Descent optimizer with decay and momentum
-
-    Parameters
-    ----------
-    learning_rate : float, default=0.0001
-        The initial learning rate used. It controls the step-size used
-        in updating the weights and biases.
-
-    decay : float, default=0.0
-        The learning rate decay over epochs.
-
-    momentum : float, default=0.0
-        The value of momentum used. Must be larger than or equal to 0.
-    """
-
-    def __init__(self, learning_rate=0.0001, decay=0.0, momentum=0.0):
-        self.learning_rate = learning_rate
-        self._learning_rate = learning_rate
-        self.decay = decay
-        self.momentum = momentum
-
-    def reset(self, model):
-        model.weight_momentums = np.zeros_like(model.initial_weight)
-        model.bias_momentums = np.zeros_like(model.initial_bias)
-
-    def pre_update_params(self, epoch):
-        if self.decay:
-            self._learning_rate = self.learning_rate * (
-                1.0 / (1.0 + self.decay * epoch)
-            )
-
-    def update_params(self, model, epoch):
-        if self.momentum:
-            if not hasattr(model, "weight_momentums"):
-                self.reset(model)
-
-            weight_updates = (
-                self.momentum * model.weight_momentums
-                - self._learning_rate * model._w_grad
-            )
-            model.weight_momentums = weight_updates
-
-            bias_updates = (
-                self.momentum * model.bias_momentums
-                - self._learning_rate * model._b_grad
-            )
-            model.bias_momentums = bias_updates
-        else:
-            weight_updates = -self._learning_rate * model._w_grad
-            bias_updates = -self._learning_rate * model._b_grad
-
-        model.weights = model.weights + weight_updates
-        model.biases = model.biases + bias_updates
-
-
-class AdaGrad:
-    """
-    Adaptive Gradient Algorithm with decay
-
-    Parameters
-    ----------
-    learning_rate : float, default=0.0001
-        The initial learning rate used. It controls the step-size used
-        in updating the weights and biases.
-
-    decay : float, default=0.0
-        The learning rate decay over epochs.
-
-    epsilon : float, default=1e-7
-        A small constant for numerical stability.
-    """
-
-    def __init__(self, learning_rate=0.0001, decay=0.0, epsilon=1e-7):
-        self.learning_rate = learning_rate
-        self._learning_rate = learning_rate
-        self.decay = decay
-        self.epsilon = epsilon
-
-    def pre_update_params(self, epoch):
-        if self.decay:
-            self._learning_rate = self.learning_rate * (
-                1.0 / (1.0 + self.decay * epoch)
-            )
-
-    def update_params(self, model, epoch):
-        if not hasattr(model, "weight_cache"):
-            model.weight_cache = np.zeros_like(model.weights)
-            model.bias_cache = np.zeros_like(model.biases)
-
-        model.weight_cache += model._w_grad**2
-        model.bias_cache += model._b_grad**2
-
-        model.weights += (
-            -model.optimizer._learning_rate
-            * model._w_grad
-            / (np.sqrt(model.weight_cache) + self.epsilon)
-        )
-        model.biases += (
-            -model.optimizer._learning_rate
-            * model._w_grad
-            / (np.sqrt(model.bias_cache) + self.epsilon)
-        )
-
-
-class RMSProp:
-    """
-    RMSProp with decay
-
-    Parameters
-    ----------
-    learning_rate : float, default=0.0001
-        The initial learning rate used. It controls the step-size used
-        in updating the weights and biases.
-
-    decay : float, default=0.0
-        The learning rate decay over epochs.
-
-    epsilon : float, default=1e-7
-        A small constant for numerical stability.
-
-    rho : float, default=0.9
-        Discounting factor for the history/coming gradient.
-    """
-
-    def __init__(self, learning_rate=0.0001, decay=0.0, epsilon=1e-7, rho=0.9):
-        self.learning_rate = learning_rate
-        self._learning_rate = learning_rate
-        self.decay = decay
-        self.epsilon = epsilon
-        self.rho = rho
-
-    def reset(self, model):
-        model.weight_cache = np.zeros_like(model.weights)
-        model.bias_cache = np.zeros_like(model.biases)
-
-    def pre_update_params(self, epoch):
-        if self.decay:
-            self._learning_rate = self.learning_rate * (
-                1.0 / (1.0 + self.decay * epoch)
-            )
-
-    def update_params(self, model, epoch):
-        if not hasattr(model, "weight_cache"):
-            self.reset(model)
-
-        model.weight_cache += (
-            self.rho * model.weight_cache + (1 - self.rho) * model._w_grad**2
-        )
-        model.bias_cache += (
-            self.rho * model.bias_cache + (1 - self.rho) * model._b_grad**2
-        )
-
-        model.weights += (
-            -model.optimizer._learning_rate
-            * model._w_grad
-            / (np.sqrt(model.weight_cache) + self.epsilon)
-        )
-        model.biases += (
-            -model.optimizer._learning_rate
-            * model._w_grad
-            / (np.sqrt(model.bias_cache) + self.epsilon)
-        )
-
-
-class Adam:
-    """
-    Adam optimizer with decay
-
-    Parameters
-    ----------
-    learning_rate : float, default=0.0001
-        The initial learning rate used. It controls the step-size used
-        in updating the weights and biases.
-
-    decay : float, default=0.0
-        The learning rate decay over epochs.
-
-    epsilon : float, default=1e-7
-        A small constant for numerical stability.
-
-    beta_1 : float, default=0.9
-        Exponential decay rate for the 1st moment estimates.
-
-    beta_2 : float, default=0.999
-        Exponential decay rate for the 2nd moment estimates.
-    """
-
-    def __init__(
-        self, learning_rate=0.0001, decay=0.0, epsilon=1e-7, beta_1=0.9, beta_2=0.999
-    ):
-
-        self.learning_rate = learning_rate
-        self._learning_rate = learning_rate
-        self.decay = decay
-        self.epsilon = epsilon
-        self.beta_1 = beta_1
-        self.beta_2 = beta_2
-
-    def reset(self, model):
-        model.weight_momentums = np.zeros_like(model.weights)
-        model.weight_cache = np.zeros_like(model.weights)
-        model.bias_momentums = np.zeros_like(model.biases)
-        model.bias_cache = np.zeros_like(model.biases)
-
-    def pre_update_params(self, epoch):
-        if self.decay:
-            self._learning_rate = self.learning_rate * (
-                1.0 / (1.0 + self.decay * epoch)
-            )
-
-    def update_params(self, model, epoch):
-        if not hasattr(model, "weight_cache"):
-            self.reset(model)
-
-        model.weight_momentums = (
-            self.beta_1 * model.weight_momentums + (1 - self.beta_1) * model._w_grad
-        )
-        model.bias_momentums = (
-            self.beta_1 * model.bias_momentums + (1 - self.beta_1) * model._b_grad
-        )
-
-        weight_momentums_corrected = model.weight_momentums / (
-            1 - self.beta_1 ** (epoch + 1)
-        )
-        bias_momentums_corrected = model.bias_momentums / (
-            1 - self.beta_1 ** (epoch + 1)
-        )
-
-        model.weight_cache += (
-            self.beta_2 * model.weight_cache + (1 - self.beta_2) * model._w_grad**2
-        )
-        model.bias_cache += (
-            self.beta_2 * model.bias_cache + (1 - self.beta_2) * model._b_grad**2
-        )
-
-        weight_cache_corrected = model.weight_cache / (1 - self.beta_2 ** (epoch + 1))
-        bias_cache_corrected = model.bias_cache / (1 - self.beta_2 ** (epoch + 1))
-
-        model.weights += (
-            -model.optimizer._learning_rate
-            * weight_momentums_corrected
-            / (np.sqrt(weight_cache_corrected) + self.epsilon)
-        )
-        model.biases += (
-            -model.optimizer._learning_rate
-            * bias_momentums_corrected
-            / (np.sqrt(bias_cache_corrected) + self.epsilon)
-        )
+# This Source Code Form is subject to the terms of the Mozilla Public
+# License, v. 2.0. If a copy of the MPL was not distributed with this
+# file, You can obtain one at https://mozilla.org/MPL/2.0/.
+
+import numpy as np
+
+
+class SGD:
+    """
+    Stochastic Gradient Descent optimizer with decay and momentum
+
+    Parameters
+    ----------
+    learning_rate : float, default=0.0001
+        The initial learning rate used. It controls the step-size used
+        in updating the weights and biases.
+
+    decay : float, default=0.0
+        The learning rate decay over epochs.
+
+    momentum : float, default=0.0
+        The value of momentum used. Must be larger than or equal to 0.
+    """
+
+    def __init__(self, learning_rate=0.0001, decay=0.0, momentum=0.0):
+        self.learning_rate = learning_rate
+        self._learning_rate = learning_rate
+        self.decay = decay
+        self.momentum = momentum
+
+    def reset(self, model):
+        model.weight_momentums = np.zeros_like(model.initial_weight)
+        model.bias_momentums = np.zeros_like(model.initial_bias)
+
+    def pre_update_params(self, epoch):
+        if self.decay:
+            self._learning_rate = self.learning_rate * (
+                1.0 / (1.0 + self.decay * epoch)
+            )
+
+    def update_params(self, model, epoch):
+        if self.momentum:
+            if not hasattr(model, "weight_momentums"):
+                self.reset(model)
+
+            weight_updates = (
+                self.momentum * model.weight_momentums
+                - self._learning_rate * model._w_grad
+            )
+            model.weight_momentums = weight_updates
+
+            bias_updates = (
+                self.momentum * model.bias_momentums
+                - self._learning_rate * model._b_grad
+            )
+            model.bias_momentums = bias_updates
+        else:
+            weight_updates = -self._learning_rate * model._w_grad
+            bias_updates = -self._learning_rate * model._b_grad
+
+        model.weights = model.weights + weight_updates
+        model.biases = model.biases + bias_updates
+
+
+class AdaGrad:
+    """
+    Adaptive Gradient Algorithm with decay
+
+    Parameters
+    ----------
+    learning_rate : float, default=0.0001
+        The initial learning rate used. It controls the step-size used
+        in updating the weights and biases.
+
+    decay : float, default=0.0
+        The learning rate decay over epochs.
+
+    epsilon : float, default=1e-7
+        A small constant for numerical stability.
+    """
+
+    def __init__(self, learning_rate=0.0001, decay=0.0, epsilon=1e-7):
+        self.learning_rate = learning_rate
+        self._learning_rate = learning_rate
+        self.decay = decay
+        self.epsilon = epsilon
+
+    def pre_update_params(self, epoch):
+        if self.decay:
+            self._learning_rate = self.learning_rate * (
+                1.0 / (1.0 + self.decay * epoch)
+            )
+
+    def update_params(self, model, epoch):
+        if not hasattr(model, "weight_cache"):
+            model.weight_cache = np.zeros_like(model.weights)
+            model.bias_cache = np.zeros_like(model.biases)
+
+        model.weight_cache += model._w_grad**2
+        model.bias_cache += model._b_grad**2
+
+        model.weights += (
+            -model.optimizer._learning_rate
+            * model._w_grad
+            / (np.sqrt(model.weight_cache) + self.epsilon)
+        )
+        model.biases += (
+            -model.optimizer._learning_rate
+            * model._w_grad
+            / (np.sqrt(model.bias_cache) + self.epsilon)
+        )
+
+
+class RMSProp:
+    """
+    RMSProp with decay
+
+    Parameters
+    ----------
+    learning_rate : float, default=0.0001
+        The initial learning rate used. It controls the step-size used
+        in updating the weights and biases.
+
+    decay : float, default=0.0
+        The learning rate decay over epochs.
+
+    epsilon : float, default=1e-7
+        A small constant for numerical stability.
+
+    rho : float, default=0.9
+        Discounting factor for the history/coming gradient.
+    """
+
+    def __init__(self, learning_rate=0.0001, decay=0.0, epsilon=1e-7, rho=0.9):
+        self.learning_rate = learning_rate
+        self._learning_rate = learning_rate
+        self.decay = decay
+        self.epsilon = epsilon
+        self.rho = rho
+
+    def reset(self, model):
+        model.weight_cache = np.zeros_like(model.weights)
+        model.bias_cache = np.zeros_like(model.biases)
+
+    def pre_update_params(self, epoch):
+        if self.decay:
+            self._learning_rate = self.learning_rate * (
+                1.0 / (1.0 + self.decay * epoch)
+            )
+
+    def update_params(self, model, epoch):
+        if not hasattr(model, "weight_cache"):
+            self.reset(model)
+
+        model.weight_cache += (
+            self.rho * model.weight_cache + (1 - self.rho) * model._w_grad**2
+        )
+        model.bias_cache += (
+            self.rho * model.bias_cache + (1 - self.rho) * model._b_grad**2
+        )
+
+        model.weights += (
+            -model.optimizer._learning_rate
+            * model._w_grad
+            / (np.sqrt(model.weight_cache) + self.epsilon)
+        )
+        model.biases += (
+            -model.optimizer._learning_rate
+            * model._w_grad
+            / (np.sqrt(model.bias_cache) + self.epsilon)
+        )
+
+
+class Adam:
+    """
+    Adam optimizer with decay
+
+    Parameters
+    ----------
+    learning_rate : float, default=0.0001
+        The initial learning rate used. It controls the step-size used
+        in updating the weights and biases.
+
+    decay : float, default=0.0
+        The learning rate decay over epochs.
+
+    epsilon : float, default=1e-7
+        A small constant for numerical stability.
+
+    beta_1 : float, default=0.9
+        Exponential decay rate for the 1st moment estimates.
+
+    beta_2 : float, default=0.999
+        Exponential decay rate for the 2nd moment estimates.
+    """
+
+    def __init__(
+        self, learning_rate=0.0001, decay=0.0, epsilon=1e-7, beta_1=0.9, beta_2=0.999
+    ):
+
+        self.learning_rate = learning_rate
+        self._learning_rate = learning_rate
+        self.decay = decay
+        self.epsilon = epsilon
+        self.beta_1 = beta_1
+        self.beta_2 = beta_2
+
+    def reset(self, model):
+        model.weight_momentums = np.zeros_like(model.weights)
+        model.weight_cache = np.zeros_like(model.weights)
+        model.bias_momentums = np.zeros_like(model.biases)
+        model.bias_cache = np.zeros_like(model.biases)
+
+    def pre_update_params(self, epoch):
+        if self.decay:
+            self._learning_rate = self.learning_rate * (
+                1.0 / (1.0 + self.decay * epoch)
+            )
+
+    def update_params(self, model, epoch):
+        if not hasattr(model, "weight_cache"):
+            self.reset(model)
+
+        model.weight_momentums = (
+            self.beta_1 * model.weight_momentums + (1 - self.beta_1) * model._w_grad
+        )
+        model.bias_momentums = (
+            self.beta_1 * model.bias_momentums + (1 - self.beta_1) * model._b_grad
+        )
+
+        weight_momentums_corrected = model.weight_momentums / (
+            1 - self.beta_1 ** (epoch + 1)
+        )
+        bias_momentums_corrected = model.bias_momentums / (
+            1 - self.beta_1 ** (epoch + 1)
+        )
+
+        model.weight_cache += (
+            self.beta_2 * model.weight_cache + (1 - self.beta_2) * model._w_grad**2
+        )
+        model.bias_cache += (
+            self.beta_2 * model.bias_cache + (1 - self.beta_2) * model._b_grad**2
+        )
+
+        weight_cache_corrected = model.weight_cache / (1 - self.beta_2 ** (epoch + 1))
+        bias_cache_corrected = model.bias_cache / (1 - self.beta_2 ** (epoch + 1))
+
+        model.weights += (
+            -model.optimizer._learning_rate
+            * weight_momentums_corrected
+            / (np.sqrt(weight_cache_corrected) + self.epsilon)
+        )
+        model.biases += (
+            -model.optimizer._learning_rate
+            * bias_momentums_corrected
+            / (np.sqrt(bias_cache_corrected) + self.epsilon)
+        )
```

### Comparing `tryangle-0.2.1/src/tryangle/metrics/__init__.py` & `tryangle-0.2.2.dev0/src/tryangle/metrics/__init__.py`

 * *Ordering differences only*

 * *Files 14% similar despite different names*

```diff
@@ -1,15 +1,15 @@
-# This Source Code Form is subject to the terms of the Mozilla Public
-# License, v. 2.0. If a copy of the MPL was not distributed with this
-# file, You can obtain one at https://mozilla.org/MPL/2.0/.
-
-"""
-The :mod:`tryangle.metrics` module includes scoring metrics used
-when finding the optimal reserving parameters.
-"""
-from tryangle.metrics.base import *  # noqa (API Import)
-from tryangle.metrics.score import (  # noqa (API Import)
-    neg_ave_scorer,
-    neg_cdr_scorer,
-    neg_weighted_ave_scorer,
-    neg_weighted_cdr_scorer,
-)
+# This Source Code Form is subject to the terms of the Mozilla Public
+# License, v. 2.0. If a copy of the MPL was not distributed with this
+# file, You can obtain one at https://mozilla.org/MPL/2.0/.
+
+"""
+The :mod:`tryangle.metrics` module includes scoring metrics used
+when finding the optimal reserving parameters.
+"""
+from tryangle.metrics.base import *  # noqa (API Import)
+from tryangle.metrics.score import (  # noqa (API Import)
+    neg_ave_scorer,
+    neg_cdr_scorer,
+    neg_weighted_ave_scorer,
+    neg_weighted_cdr_scorer,
+)
```

### Comparing `tryangle-0.2.1/src/tryangle/metrics/score.py` & `tryangle-0.2.2.dev0/src/tryangle/metrics/score.py`

 * *Ordering differences only*

 * *Files 15% similar despite different names*

```diff
@@ -1,81 +1,81 @@
-# This Source Code Form is subject to the terms of the Mozilla Public
-# License, v. 2.0. If a copy of the MPL was not distributed with this
-# file, You can obtain one at https://mozilla.org/MPL/2.0/.
-
-import numpy as np
-
-from tryangle.metrics.base import get_actual_expected
-
-from sklearn.metrics._scorer import _BaseScorer
-from sklearn.metrics import mean_squared_error
-
-
-class AVEScore(_BaseScorer):
-    """Base AvE scoring class"""
-
-    def __init__(
-        self,
-        score_func=mean_squared_error,
-        sign=-1,
-        kwargs={"squared": False},
-        weighted=False,
-    ):
-        self.weighted = weighted
-        super().__init__(score_func, sign, kwargs)
-
-    def _sample_weight(self, X, valuation_date):
-        X_prior = X[X.triangle.valuation < valuation_date]
-        return np.abs(
-            X.triangle.latest_diagonal.to_frame().to_numpy()[:-1]
-            - X_prior.triangle.latest_diagonal.to_frame().to_numpy()
-        )
-
-    def _score(self, method_caller, estimator, X, y_true=None, sample_weight=None):
-        """Evaluate predicted target values for X relative to y_true."""  # TODO: Update docstring
-
-        valuation_date = X.triangle.cum_to_incr().latest_diagonal.valuation[0]
-        actual, expected = get_actual_expected(estimator, X)
-
-        if self.weighted:
-            sample_weight = self._sample_weight(X, valuation_date)
-            return self._sign * self._score_func(
-                actual, expected, sample_weight=sample_weight, **self._kwargs
-            )
-        else:
-            return self._sign * self._score_func(actual, expected, **self._kwargs)
-
-
-class CDRScore(AVEScore):
-    """Base CDR scoring class"""
-
-    def _score(self, method_caller, estimator, X, y_true, sample_weight=None):
-        """Evaluate predicted target values for X relative to y_true."""  # TODO: Update docstring
-
-        valuation_date = y_true.triangle.latest_diagonal.valuation[0]
-        X_k = X[X.triangle.valuation < valuation_date]
-        X_k_1 = X
-
-        # We only need actual as the expected will be in ibnr_k
-        actual, _ = get_actual_expected(estimator, X)
-
-        # ! TODO: Rewrite a better method that avoids fillna(0) as this could mask some error
-        ibnr_k = estimator.fit_predict(X_k).ibnr_.to_frame().fillna(0).to_numpy()
-        ibnr_k_1 = (
-            estimator.fit_predict(X_k_1).ibnr_.to_frame().fillna(0).to_numpy()[:-1]
-        )
-
-        if self.weighted:
-            sample_weight = super()._sample_weight(X, valuation_date)
-            return self._sign * self._score_func(
-                actual + ibnr_k_1, ibnr_k, sample_weight=sample_weight, **self._kwargs
-            )
-        else:
-            return self._sign * self._score_func(
-                actual + ibnr_k_1, ibnr_k, **self._kwargs
-            )
-
-
-neg_ave_scorer = AVEScore()
-neg_weighted_ave_scorer = AVEScore(weighted=True)
-neg_cdr_scorer = CDRScore()
-neg_weighted_cdr_scorer = CDRScore(weighted=True)
+# This Source Code Form is subject to the terms of the Mozilla Public
+# License, v. 2.0. If a copy of the MPL was not distributed with this
+# file, You can obtain one at https://mozilla.org/MPL/2.0/.
+
+import numpy as np
+
+from tryangle.metrics.base import get_actual_expected
+
+from sklearn.metrics._scorer import _BaseScorer
+from sklearn.metrics import mean_squared_error
+
+
+class AVEScore(_BaseScorer):
+    """Base AvE scoring class"""
+
+    def __init__(
+        self,
+        score_func=mean_squared_error,
+        sign=-1,
+        kwargs={"squared": False},
+        weighted=False,
+    ):
+        self.weighted = weighted
+        super().__init__(score_func, sign, kwargs)
+
+    def _sample_weight(self, X, valuation_date):
+        X_prior = X[X.triangle.valuation < valuation_date]
+        return np.abs(
+            X.triangle.latest_diagonal.to_frame().to_numpy()[:-1]
+            - X_prior.triangle.latest_diagonal.to_frame().to_numpy()
+        )
+
+    def _score(self, method_caller, estimator, X, y_true=None, sample_weight=None):
+        """Evaluate predicted target values for X relative to y_true."""  # TODO: Update docstring
+
+        valuation_date = X.triangle.cum_to_incr().latest_diagonal.valuation[0]
+        actual, expected = get_actual_expected(estimator, X)
+
+        if self.weighted:
+            sample_weight = self._sample_weight(X, valuation_date)
+            return self._sign * self._score_func(
+                actual, expected, sample_weight=sample_weight, **self._kwargs
+            )
+        else:
+            return self._sign * self._score_func(actual, expected, **self._kwargs)
+
+
+class CDRScore(AVEScore):
+    """Base CDR scoring class"""
+
+    def _score(self, method_caller, estimator, X, y_true, sample_weight=None):
+        """Evaluate predicted target values for X relative to y_true."""  # TODO: Update docstring
+
+        valuation_date = y_true.triangle.latest_diagonal.valuation[0]
+        X_k = X[X.triangle.valuation < valuation_date]
+        X_k_1 = X
+
+        # We only need actual as the expected will be in ibnr_k
+        actual, _ = get_actual_expected(estimator, X)
+
+        # ! TODO: Rewrite a better method that avoids fillna(0) as this could mask some error
+        ibnr_k = estimator.fit_predict(X_k).ibnr_.to_frame().fillna(0).to_numpy()
+        ibnr_k_1 = (
+            estimator.fit_predict(X_k_1).ibnr_.to_frame().fillna(0).to_numpy()[:-1]
+        )
+
+        if self.weighted:
+            sample_weight = super()._sample_weight(X, valuation_date)
+            return self._sign * self._score_func(
+                actual + ibnr_k_1, ibnr_k, sample_weight=sample_weight, **self._kwargs
+            )
+        else:
+            return self._sign * self._score_func(
+                actual + ibnr_k_1, ibnr_k, **self._kwargs
+            )
+
+
+neg_ave_scorer = AVEScore()
+neg_weighted_ave_scorer = AVEScore(weighted=True)
+neg_cdr_scorer = CDRScore()
+neg_weighted_cdr_scorer = CDRScore(weighted=True)
```

### Comparing `tryangle-0.2.1/src/tryangle/model_selection/split.py` & `tryangle-0.2.2.dev0/src/tryangle/model_selection/split.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,40 +1,40 @@
-# This Source Code Form is subject to the terms of the Mozilla Public
-# License, v. 2.0. If a copy of the MPL was not distributed with this
-# file, You can obtain one at https://mozilla.org/MPL/2.0/.
-
-import numpy as np
-from sklearn.model_selection._split import TimeSeriesSplit
-
-
-class TriangleSplit(TimeSeriesSplit):
-    """Triangle cross-validation across calendar periods
-
-    Splits a ``TryangleData`` instance into k sub-triangles or folds
-    over the latest k calendar periods or diagonals. Thus, successive
-    folds are supersets of previous folds.
-
-    Parameters
-    ----------
-    n_splits : int, default=5
-        Number of splits, must be at least 2.
-    """
-
-    def __init__(self, n_splits=5, *, max_train_size=None, test_size=None, gap=0):
-        super().__init__(n_splits=n_splits, max_train_size=None, test_size=1, gap=0)
-
-    def split(self, X, y=None, groups=None):
-        valuation_date = X.triangle.latest_diagonal.valuation[0]
-        valuation_dates = np.array(
-            [
-                date
-                for date in X.triangle.valuation.drop_duplicates().sort_values()
-                if date.date() <= valuation_date
-            ]
-        )
-        for train, test in super().split(valuation_dates):
-            indices = np.arange(X.triangle.shape[2] * X.triangle.shape[3])
-            test_start = test[0]
-            yield (
-                indices[X.triangle.valuation <= valuation_dates[test_start]],
-                indices[X.triangle.valuation <= valuation_dates[test_start]],
-            )
+# This Source Code Form is subject to the terms of the Mozilla Public
+# License, v. 2.0. If a copy of the MPL was not distributed with this
+# file, You can obtain one at https://mozilla.org/MPL/2.0/.
+
+import numpy as np
+from sklearn.model_selection._split import TimeSeriesSplit
+
+
+class TriangleSplit(TimeSeriesSplit):
+    """Triangle cross-validation across calendar periods
+
+    Splits a ``TryangleData`` instance into k sub-triangles or folds
+    over the latest k calendar periods or diagonals. Thus, successive
+    folds are supersets of previous folds.
+
+    Parameters
+    ----------
+    n_splits : int, default=5
+        Number of splits, must be at least 2.
+    """
+
+    def __init__(self, n_splits=5, *, max_train_size=None, test_size=None, gap=0):
+        super().__init__(n_splits=n_splits, max_train_size=None, test_size=1, gap=0)
+
+    def split(self, X, y=None, groups=None):
+        valuation_date = X.triangle.latest_diagonal.valuation[0]
+        valuation_dates = np.array(
+            [
+                date
+                for date in X.triangle.valuation.drop_duplicates().sort_values()
+                if date.date() <= valuation_date.date()
+            ]
+        )
+        for train, test in super().split(valuation_dates):
+            indices = np.arange(X.triangle.shape[2] * X.triangle.shape[3])
+            test_start = test[0]
+            yield (
+                indices[X.triangle.valuation <= valuation_dates[test_start]],
+                indices[X.triangle.valuation <= valuation_dates[test_start]],
+            )
```

### Comparing `tryangle-0.2.1/src/tryangle/utils/data/cas_test.csv` & `tryangle-0.2.2.dev0/src/tryangle/utils/data/cas_test.csv`

 * *Ordering differences only*

 * *Files 23% similar despite different names*

```diff
@@ -1,211 +1,211 @@
-﻿origin,development,lag,claim,premium
-2010/03/31,2015/03/31,20,9455.582936,0
-2010/06/30,2015/03/31,19,5807.656259,0
-2010/06/30,2015/06/30,20,5802.727068,0
-2010/09/30,2015/03/31,18,7821.904961,0
-2010/09/30,2015/06/30,19,7821.405067,0
-2010/09/30,2015/09/30,20,8155.834385,0
-2010/12/31,2015/03/31,17,5920.818388,0
-2010/12/31,2015/06/30,18,6165.941,0
-2010/12/31,2015/09/30,19,6196.027664,0
-2010/12/31,2015/12/31,20,6026.017085,0
-2011/03/31,2015/03/31,16,8708.868662,0
-2011/03/31,2015/06/30,17,9367.636407,0
-2011/03/31,2015/09/30,18,9670.723512,0
-2011/03/31,2015/12/31,19,10318.90047,0
-2011/03/31,2016/03/31,20,10078.6838,0
-2011/06/30,2015/03/31,15,7050.81212,0
-2011/06/30,2015/06/30,16,6987.592923,0
-2011/06/30,2015/09/30,17,7024.759487,0
-2011/06/30,2015/12/31,18,7182.156453,0
-2011/06/30,2016/03/31,19,6672.333972,0
-2011/06/30,2016/06/30,20,6675.705353,0
-2011/09/30,2015/03/31,14,8560.597674,0
-2011/09/30,2015/06/30,15,8368.7545,0
-2011/09/30,2015/09/30,16,8322.810722,0
-2011/09/30,2015/12/31,17,8495.471904,0
-2011/09/30,2016/03/31,18,8286.097551,0
-2011/09/30,2016/06/30,19,8254.976221,0
-2011/09/30,2016/09/30,20,8536.265608,0
-2011/12/31,2015/03/31,13,9206.937813,0
-2011/12/31,2015/06/30,14,9792.186212,0
-2011/12/31,2015/09/30,15,9953.245195,0
-2011/12/31,2015/12/31,16,10001.54894,0
-2011/12/31,2016/03/31,17,9407.197813,0
-2011/12/31,2016/06/30,18,9451.769788,0
-2011/12/31,2016/09/30,19,8273.228178,0
-2011/12/31,2016/12/31,20,8370.95171,0
-2012/03/31,2015/03/31,12,2504.505551,0
-2012/03/31,2015/06/30,13,2677.771256,0
-2012/03/31,2015/09/30,14,2594.393529,0
-2012/03/31,2015/12/31,15,2648.196111,0
-2012/03/31,2016/03/31,16,2660.832975,0
-2012/03/31,2016/06/30,17,2521.048566,0
-2012/03/31,2016/09/30,18,2529.395639,0
-2012/03/31,2016/12/31,19,2370.231604,0
-2012/03/31,2017/03/31,20,2370.231604,0
-2012/06/30,2015/03/31,11,4719.5839,0
-2012/06/30,2015/06/30,12,5136.530661,0
-2012/06/30,2015/09/30,13,5207.515658,0
-2012/06/30,2015/12/31,14,5588.958295,0
-2012/06/30,2016/03/31,15,6253.538765,0
-2012/06/30,2016/06/30,16,6507.101453,0
-2012/06/30,2016/09/30,17,6507.101453,0
-2012/06/30,2016/12/31,18,6593.048404,0
-2012/06/30,2017/03/31,19,6603.650814,0
-2012/06/30,2017/06/30,20,6659.034458,0
-2012/09/30,2015/03/31,10,7024.701359,0
-2012/09/30,2015/06/30,11,7046.092187,0
-2012/09/30,2015/09/30,12,7394.181408,0
-2012/09/30,2015/12/31,13,10204.44792,0
-2012/09/30,2016/03/31,14,9914.892836,0
-2012/09/30,2016/06/30,15,9643.392079,0
-2012/09/30,2016/09/30,16,9928.971256,0
-2012/09/30,2016/12/31,17,10268.88779,0
-2012/09/30,2017/03/31,18,10221.3397,0
-2012/09/30,2017/06/30,19,10808.43654,0
-2012/09/30,2017/09/30,20,10913.05397,0
-2012/12/31,2015/03/31,9,4983.900129,0
-2012/12/31,2015/06/30,10,4971.553901,0
-2012/12/31,2015/09/30,11,5328.397086,0
-2012/12/31,2015/12/31,12,5752.481874,0
-2012/12/31,2016/03/31,13,5802.343428,0
-2012/12/31,2016/06/30,14,5553.616928,0
-2012/12/31,2016/09/30,15,6082.888786,0
-2012/12/31,2016/12/31,16,6529.6432,0
-2012/12/31,2017/03/31,17,6522.784185,0
-2012/12/31,2017/06/30,18,6564.868313,0
-2012/12/31,2017/09/30,19,6569.704501,0
-2012/12/31,2017/12/31,20,6519.645313,0
-2013/03/31,2015/03/31,8,4766.701849,0
-2013/03/31,2015/06/30,9,5146.912188,0
-2013/03/31,2015/09/30,10,5977.108817,0
-2013/03/31,2015/12/31,11,5955.415727,0
-2013/03/31,2016/03/31,12,6004.498377,0
-2013/03/31,2016/06/30,13,6077.296944,0
-2013/03/31,2016/09/30,14,6227.974401,0
-2013/03/31,2016/12/31,15,6501.928128,0
-2013/03/31,2017/03/31,16,6590.22342,0
-2013/03/31,2017/06/30,17,6602.709153,0
-2013/03/31,2017/09/30,18,7606.764385,0
-2013/03/31,2017/12/31,19,7754.256468,0
-2013/03/31,2018/03/31,20,7754.256468,0
-2013/06/30,2015/03/31,7,10614.36128,0
-2013/06/30,2015/06/30,8,11270.87369,0
-2013/06/30,2015/09/30,9,11901.05445,0
-2013/06/30,2015/12/31,10,11493.18717,0
-2013/06/30,2016/03/31,11,11492.57102,0
-2013/06/30,2016/06/30,12,11778.18507,0
-2013/06/30,2016/09/30,13,11795.65812,0
-2013/06/30,2016/12/31,14,11238.04342,0
-2013/06/30,2017/03/31,15,11358.48308,0
-2013/06/30,2017/06/30,16,11098.73565,0
-2013/06/30,2017/09/30,17,11107.0711,0
-2013/06/30,2017/12/31,18,11450.11487,0
-2013/06/30,2018/03/31,19,11413.3087,0
-2013/06/30,2018/06/30,20,11607.40721,0
-2013/09/30,2015/03/31,6,4882.154192,0
-2013/09/30,2015/06/30,7,4970.077469,0
-2013/09/30,2015/09/30,8,4877.07387,0
-2013/09/30,2015/12/31,9,5969.377893,0
-2013/09/30,2016/03/31,10,6023.157224,0
-2013/09/30,2016/06/30,11,6167.719694,0
-2013/09/30,2016/09/30,12,6383.557797,0
-2013/09/30,2016/12/31,13,7814.511175,0
-2013/09/30,2017/03/31,14,7804.362157,0
-2013/09/30,2017/06/30,15,7262.162799,0
-2013/09/30,2017/09/30,16,8047.078301,0
-2013/09/30,2017/12/31,17,8041.846848,0
-2013/09/30,2018/03/31,18,8288.318012,0
-2013/09/30,2018/06/30,19,8340.237271,0
-2013/09/30,2018/09/30,20,8329.809243,0
-2013/12/31,2015/03/31,5,7356.631205,0
-2013/12/31,2015/06/30,6,7117.693333,0
-2013/12/31,2015/09/30,7,7671.250756,0
-2013/12/31,2015/12/31,8,7983.905606,0
-2013/12/31,2016/03/31,9,8775.831254,0
-2013/12/31,2016/06/30,10,9575.278568,0
-2013/12/31,2016/09/30,11,9614.851599,0
-2013/12/31,2016/12/31,12,9884.143521,0
-2013/12/31,2017/03/31,13,9907.88269,0
-2013/12/31,2017/06/30,14,7871.127116,0
-2013/12/31,2017/09/30,15,8005.029048,0
-2013/12/31,2017/12/31,16,7982.185039,0
-2013/12/31,2018/03/31,17,7897.8424,0
-2013/12/31,2018/06/30,18,7899.597843,0
-2013/12/31,2018/09/30,19,7894.447769,0
-2013/12/31,2018/12/31,20,7732.237866,0
-2014/03/31,2015/03/31,4,5070.777116,0
-2014/03/31,2015/06/30,5,5653.839931,0
-2014/03/31,2015/09/30,6,6389.265893,0
-2014/03/31,2015/12/31,7,7468.130895,0
-2014/03/31,2016/03/31,8,7458.226012,0
-2014/03/31,2016/06/30,9,7303.293641,0
-2014/03/31,2016/09/30,10,7229.983554,0
-2014/03/31,2016/12/31,11,7365.826936,0
-2014/03/31,2017/03/31,12,7498.264061,0
-2014/03/31,2017/06/30,13,8081.245498,0
-2014/03/31,2017/09/30,14,8312.684955,0
-2014/03/31,2017/12/31,15,8778.70274,0
-2014/03/31,2018/03/31,16,8854.465797,0
-2014/03/31,2018/06/30,17,9395.583989,0
-2014/03/31,2018/09/30,18,9567.431389,0
-2014/03/31,2018/12/31,19,10067.05835,0
-2014/03/31,2019/03/31,20,10907.65976,0
-2014/06/30,2015/03/31,3,10026.34602,0
-2014/06/30,2015/06/30,4,10224.50182,0
-2014/06/30,2015/09/30,5,10712.86372,0
-2014/06/30,2015/12/31,6,11673.96291,0
-2014/06/30,2016/03/31,7,11833.42921,0
-2014/06/30,2016/06/30,8,11639.13306,0
-2014/06/30,2016/09/30,9,12485.36119,0
-2014/06/30,2016/12/31,10,12278.86995,0
-2014/06/30,2017/03/31,11,12327.17369,0
-2014/06/30,2017/06/30,12,11754.22502,0
-2014/06/30,2017/09/30,13,11808.58562,0
-2014/06/30,2017/12/31,14,11776.18549,0
-2014/06/30,2018/03/31,15,11853.77375,0
-2014/06/30,2018/06/30,16,11686.86716,0
-2014/06/30,2018/09/30,17,11708.78114,0
-2014/06/30,2018/12/31,18,11364.81895,0
-2014/06/30,2019/03/31,19,11469.4945,0
-2014/06/30,2019/06/30,20,10940.32727,0
-2014/09/30,2015/03/31,2,6178.124471,0
-2014/09/30,2015/06/30,3,8651.020424,0
-2014/09/30,2015/09/30,4,10214.28305,0
-2014/09/30,2015/12/31,5,11282.7084,0
-2014/09/30,2016/03/31,6,11203.48095,0
-2014/09/30,2016/06/30,7,11551.5818,0
-2014/09/30,2016/09/30,8,12697.20014,0
-2014/09/30,2016/12/31,9,12468.06252,0
-2014/09/30,2017/03/31,10,12828.07945,0
-2014/09/30,2017/06/30,11,14162.85548,0
-2014/09/30,2017/09/30,12,13961.60732,0
-2014/09/30,2017/12/31,13,14113.86584,0
-2014/09/30,2018/03/31,14,14931.72786,0
-2014/09/30,2018/06/30,15,16580.93744,0
-2014/09/30,2018/09/30,16,16279.29189,0
-2014/09/30,2018/12/31,17,15667.74672,0
-2014/09/30,2019/03/31,18,15625.05807,0
-2014/09/30,2019/06/30,19,17347.31035,0
-2014/09/30,2019/09/30,20,17165.33718,0
-2014/12/31,2015/03/31,1,4341.617273,0
-2014/12/31,2015/06/30,2,4786.546492,0
-2014/12/31,2015/09/30,3,6309.515306,0
-2014/12/31,2015/12/31,4,7942.635259,0
-2014/12/31,2016/03/31,5,8481.951506,0
-2014/12/31,2016/06/30,6,8669.772274,0
-2014/12/31,2016/09/30,7,8747.348902,0
-2014/12/31,2016/12/31,8,9149.728974,0
-2014/12/31,2017/03/31,9,9373.867648,0
-2014/12/31,2017/06/30,10,9823.168036,0
-2014/12/31,2017/09/30,11,10711.74767,0
-2014/12/31,2017/12/31,12,11521.55326,0
-2014/12/31,2018/03/31,13,11241.58918,0
-2014/12/31,2018/06/30,14,12279.20709,0
-2014/12/31,2018/09/30,15,13806.30294,0
-2014/12/31,2018/12/31,16,13720.93726,0
-2014/12/31,2019/03/31,17,13857.64092,0
-2014/12/31,2019/06/30,18,14243.54773,0
-2014/12/31,2019/09/30,19,16558.00043,0
-2014/12/31,2019/12/31,20,16405.61403,0
+﻿origin,development,lag,claim,premium
+2010/03/31,2015/03/31,20,9455.582936,0
+2010/06/30,2015/03/31,19,5807.656259,0
+2010/06/30,2015/06/30,20,5802.727068,0
+2010/09/30,2015/03/31,18,7821.904961,0
+2010/09/30,2015/06/30,19,7821.405067,0
+2010/09/30,2015/09/30,20,8155.834385,0
+2010/12/31,2015/03/31,17,5920.818388,0
+2010/12/31,2015/06/30,18,6165.941,0
+2010/12/31,2015/09/30,19,6196.027664,0
+2010/12/31,2015/12/31,20,6026.017085,0
+2011/03/31,2015/03/31,16,8708.868662,0
+2011/03/31,2015/06/30,17,9367.636407,0
+2011/03/31,2015/09/30,18,9670.723512,0
+2011/03/31,2015/12/31,19,10318.90047,0
+2011/03/31,2016/03/31,20,10078.6838,0
+2011/06/30,2015/03/31,15,7050.81212,0
+2011/06/30,2015/06/30,16,6987.592923,0
+2011/06/30,2015/09/30,17,7024.759487,0
+2011/06/30,2015/12/31,18,7182.156453,0
+2011/06/30,2016/03/31,19,6672.333972,0
+2011/06/30,2016/06/30,20,6675.705353,0
+2011/09/30,2015/03/31,14,8560.597674,0
+2011/09/30,2015/06/30,15,8368.7545,0
+2011/09/30,2015/09/30,16,8322.810722,0
+2011/09/30,2015/12/31,17,8495.471904,0
+2011/09/30,2016/03/31,18,8286.097551,0
+2011/09/30,2016/06/30,19,8254.976221,0
+2011/09/30,2016/09/30,20,8536.265608,0
+2011/12/31,2015/03/31,13,9206.937813,0
+2011/12/31,2015/06/30,14,9792.186212,0
+2011/12/31,2015/09/30,15,9953.245195,0
+2011/12/31,2015/12/31,16,10001.54894,0
+2011/12/31,2016/03/31,17,9407.197813,0
+2011/12/31,2016/06/30,18,9451.769788,0
+2011/12/31,2016/09/30,19,8273.228178,0
+2011/12/31,2016/12/31,20,8370.95171,0
+2012/03/31,2015/03/31,12,2504.505551,0
+2012/03/31,2015/06/30,13,2677.771256,0
+2012/03/31,2015/09/30,14,2594.393529,0
+2012/03/31,2015/12/31,15,2648.196111,0
+2012/03/31,2016/03/31,16,2660.832975,0
+2012/03/31,2016/06/30,17,2521.048566,0
+2012/03/31,2016/09/30,18,2529.395639,0
+2012/03/31,2016/12/31,19,2370.231604,0
+2012/03/31,2017/03/31,20,2370.231604,0
+2012/06/30,2015/03/31,11,4719.5839,0
+2012/06/30,2015/06/30,12,5136.530661,0
+2012/06/30,2015/09/30,13,5207.515658,0
+2012/06/30,2015/12/31,14,5588.958295,0
+2012/06/30,2016/03/31,15,6253.538765,0
+2012/06/30,2016/06/30,16,6507.101453,0
+2012/06/30,2016/09/30,17,6507.101453,0
+2012/06/30,2016/12/31,18,6593.048404,0
+2012/06/30,2017/03/31,19,6603.650814,0
+2012/06/30,2017/06/30,20,6659.034458,0
+2012/09/30,2015/03/31,10,7024.701359,0
+2012/09/30,2015/06/30,11,7046.092187,0
+2012/09/30,2015/09/30,12,7394.181408,0
+2012/09/30,2015/12/31,13,10204.44792,0
+2012/09/30,2016/03/31,14,9914.892836,0
+2012/09/30,2016/06/30,15,9643.392079,0
+2012/09/30,2016/09/30,16,9928.971256,0
+2012/09/30,2016/12/31,17,10268.88779,0
+2012/09/30,2017/03/31,18,10221.3397,0
+2012/09/30,2017/06/30,19,10808.43654,0
+2012/09/30,2017/09/30,20,10913.05397,0
+2012/12/31,2015/03/31,9,4983.900129,0
+2012/12/31,2015/06/30,10,4971.553901,0
+2012/12/31,2015/09/30,11,5328.397086,0
+2012/12/31,2015/12/31,12,5752.481874,0
+2012/12/31,2016/03/31,13,5802.343428,0
+2012/12/31,2016/06/30,14,5553.616928,0
+2012/12/31,2016/09/30,15,6082.888786,0
+2012/12/31,2016/12/31,16,6529.6432,0
+2012/12/31,2017/03/31,17,6522.784185,0
+2012/12/31,2017/06/30,18,6564.868313,0
+2012/12/31,2017/09/30,19,6569.704501,0
+2012/12/31,2017/12/31,20,6519.645313,0
+2013/03/31,2015/03/31,8,4766.701849,0
+2013/03/31,2015/06/30,9,5146.912188,0
+2013/03/31,2015/09/30,10,5977.108817,0
+2013/03/31,2015/12/31,11,5955.415727,0
+2013/03/31,2016/03/31,12,6004.498377,0
+2013/03/31,2016/06/30,13,6077.296944,0
+2013/03/31,2016/09/30,14,6227.974401,0
+2013/03/31,2016/12/31,15,6501.928128,0
+2013/03/31,2017/03/31,16,6590.22342,0
+2013/03/31,2017/06/30,17,6602.709153,0
+2013/03/31,2017/09/30,18,7606.764385,0
+2013/03/31,2017/12/31,19,7754.256468,0
+2013/03/31,2018/03/31,20,7754.256468,0
+2013/06/30,2015/03/31,7,10614.36128,0
+2013/06/30,2015/06/30,8,11270.87369,0
+2013/06/30,2015/09/30,9,11901.05445,0
+2013/06/30,2015/12/31,10,11493.18717,0
+2013/06/30,2016/03/31,11,11492.57102,0
+2013/06/30,2016/06/30,12,11778.18507,0
+2013/06/30,2016/09/30,13,11795.65812,0
+2013/06/30,2016/12/31,14,11238.04342,0
+2013/06/30,2017/03/31,15,11358.48308,0
+2013/06/30,2017/06/30,16,11098.73565,0
+2013/06/30,2017/09/30,17,11107.0711,0
+2013/06/30,2017/12/31,18,11450.11487,0
+2013/06/30,2018/03/31,19,11413.3087,0
+2013/06/30,2018/06/30,20,11607.40721,0
+2013/09/30,2015/03/31,6,4882.154192,0
+2013/09/30,2015/06/30,7,4970.077469,0
+2013/09/30,2015/09/30,8,4877.07387,0
+2013/09/30,2015/12/31,9,5969.377893,0
+2013/09/30,2016/03/31,10,6023.157224,0
+2013/09/30,2016/06/30,11,6167.719694,0
+2013/09/30,2016/09/30,12,6383.557797,0
+2013/09/30,2016/12/31,13,7814.511175,0
+2013/09/30,2017/03/31,14,7804.362157,0
+2013/09/30,2017/06/30,15,7262.162799,0
+2013/09/30,2017/09/30,16,8047.078301,0
+2013/09/30,2017/12/31,17,8041.846848,0
+2013/09/30,2018/03/31,18,8288.318012,0
+2013/09/30,2018/06/30,19,8340.237271,0
+2013/09/30,2018/09/30,20,8329.809243,0
+2013/12/31,2015/03/31,5,7356.631205,0
+2013/12/31,2015/06/30,6,7117.693333,0
+2013/12/31,2015/09/30,7,7671.250756,0
+2013/12/31,2015/12/31,8,7983.905606,0
+2013/12/31,2016/03/31,9,8775.831254,0
+2013/12/31,2016/06/30,10,9575.278568,0
+2013/12/31,2016/09/30,11,9614.851599,0
+2013/12/31,2016/12/31,12,9884.143521,0
+2013/12/31,2017/03/31,13,9907.88269,0
+2013/12/31,2017/06/30,14,7871.127116,0
+2013/12/31,2017/09/30,15,8005.029048,0
+2013/12/31,2017/12/31,16,7982.185039,0
+2013/12/31,2018/03/31,17,7897.8424,0
+2013/12/31,2018/06/30,18,7899.597843,0
+2013/12/31,2018/09/30,19,7894.447769,0
+2013/12/31,2018/12/31,20,7732.237866,0
+2014/03/31,2015/03/31,4,5070.777116,0
+2014/03/31,2015/06/30,5,5653.839931,0
+2014/03/31,2015/09/30,6,6389.265893,0
+2014/03/31,2015/12/31,7,7468.130895,0
+2014/03/31,2016/03/31,8,7458.226012,0
+2014/03/31,2016/06/30,9,7303.293641,0
+2014/03/31,2016/09/30,10,7229.983554,0
+2014/03/31,2016/12/31,11,7365.826936,0
+2014/03/31,2017/03/31,12,7498.264061,0
+2014/03/31,2017/06/30,13,8081.245498,0
+2014/03/31,2017/09/30,14,8312.684955,0
+2014/03/31,2017/12/31,15,8778.70274,0
+2014/03/31,2018/03/31,16,8854.465797,0
+2014/03/31,2018/06/30,17,9395.583989,0
+2014/03/31,2018/09/30,18,9567.431389,0
+2014/03/31,2018/12/31,19,10067.05835,0
+2014/03/31,2019/03/31,20,10907.65976,0
+2014/06/30,2015/03/31,3,10026.34602,0
+2014/06/30,2015/06/30,4,10224.50182,0
+2014/06/30,2015/09/30,5,10712.86372,0
+2014/06/30,2015/12/31,6,11673.96291,0
+2014/06/30,2016/03/31,7,11833.42921,0
+2014/06/30,2016/06/30,8,11639.13306,0
+2014/06/30,2016/09/30,9,12485.36119,0
+2014/06/30,2016/12/31,10,12278.86995,0
+2014/06/30,2017/03/31,11,12327.17369,0
+2014/06/30,2017/06/30,12,11754.22502,0
+2014/06/30,2017/09/30,13,11808.58562,0
+2014/06/30,2017/12/31,14,11776.18549,0
+2014/06/30,2018/03/31,15,11853.77375,0
+2014/06/30,2018/06/30,16,11686.86716,0
+2014/06/30,2018/09/30,17,11708.78114,0
+2014/06/30,2018/12/31,18,11364.81895,0
+2014/06/30,2019/03/31,19,11469.4945,0
+2014/06/30,2019/06/30,20,10940.32727,0
+2014/09/30,2015/03/31,2,6178.124471,0
+2014/09/30,2015/06/30,3,8651.020424,0
+2014/09/30,2015/09/30,4,10214.28305,0
+2014/09/30,2015/12/31,5,11282.7084,0
+2014/09/30,2016/03/31,6,11203.48095,0
+2014/09/30,2016/06/30,7,11551.5818,0
+2014/09/30,2016/09/30,8,12697.20014,0
+2014/09/30,2016/12/31,9,12468.06252,0
+2014/09/30,2017/03/31,10,12828.07945,0
+2014/09/30,2017/06/30,11,14162.85548,0
+2014/09/30,2017/09/30,12,13961.60732,0
+2014/09/30,2017/12/31,13,14113.86584,0
+2014/09/30,2018/03/31,14,14931.72786,0
+2014/09/30,2018/06/30,15,16580.93744,0
+2014/09/30,2018/09/30,16,16279.29189,0
+2014/09/30,2018/12/31,17,15667.74672,0
+2014/09/30,2019/03/31,18,15625.05807,0
+2014/09/30,2019/06/30,19,17347.31035,0
+2014/09/30,2019/09/30,20,17165.33718,0
+2014/12/31,2015/03/31,1,4341.617273,0
+2014/12/31,2015/06/30,2,4786.546492,0
+2014/12/31,2015/09/30,3,6309.515306,0
+2014/12/31,2015/12/31,4,7942.635259,0
+2014/12/31,2016/03/31,5,8481.951506,0
+2014/12/31,2016/06/30,6,8669.772274,0
+2014/12/31,2016/09/30,7,8747.348902,0
+2014/12/31,2016/12/31,8,9149.728974,0
+2014/12/31,2017/03/31,9,9373.867648,0
+2014/12/31,2017/06/30,10,9823.168036,0
+2014/12/31,2017/09/30,11,10711.74767,0
+2014/12/31,2017/12/31,12,11521.55326,0
+2014/12/31,2018/03/31,13,11241.58918,0
+2014/12/31,2018/06/30,14,12279.20709,0
+2014/12/31,2018/09/30,15,13806.30294,0
+2014/12/31,2018/12/31,16,13720.93726,0
+2014/12/31,2019/03/31,17,13857.64092,0
+2014/12/31,2019/06/30,18,14243.54773,0
+2014/12/31,2019/09/30,19,16558.00043,0
+2014/12/31,2019/12/31,20,16405.61403,0
```

### Comparing `tryangle-0.2.1/src/tryangle/utils/data/cas_train.csv` & `tryangle-0.2.2.dev0/src/tryangle/utils/data/sme_train.csv`

 * *Files 23% similar despite different names*

```diff
@@ -1,211 +1,211 @@
-origin,development,lag,claim,premium
-2010/03/31,2010/03/31,0,2013.946441,25728.2402
-2010/03/31,2010/06/30,1,3924.798392,25728.2402
-2010/03/31,2010/09/30,2,6027.319135,25728.2402
-2010/03/31,2010/12/31,3,6476.875283,25728.2402
-2010/03/31,2011/03/31,4,5624.078779,25728.2402
-2010/03/31,2011/06/30,5,5159.316543,25728.2402
-2010/03/31,2011/09/30,6,5213.851529,25728.2402
-2010/03/31,2011/12/31,7,6240.692643,25728.2402
-2010/03/31,2012/03/31,8,6705.35025,25728.2402
-2010/03/31,2012/06/30,9,6716.243297,25728.2402
-2010/03/31,2012/09/30,10,7373.267224,25728.2402
-2010/03/31,2012/12/31,11,7695.745579,25728.2402
-2010/03/31,2013/03/31,12,9011.246614,25728.2402
-2010/03/31,2013/06/30,13,9229.502811,25728.2402
-2010/03/31,2013/09/30,14,8408.513538,25728.2402
-2010/03/31,2013/12/31,15,8448.179574,25728.2402
-2010/03/31,2014/03/31,16,8824.216376,25728.2402
-2010/03/31,2014/06/30,17,9202.496891,25728.2402
-2010/03/31,2014/09/30,18,9388.457588,25728.2402
-2010/03/31,2014/12/31,19,9349.686712,25728.2402
-2010/06/30,2010/06/30,0,2531.220834,25975.3502
-2010/06/30,2010/09/30,1,4102.412015,25975.3502
-2010/06/30,2010/12/31,2,3674.700088,25975.3502
-2010/06/30,2011/03/31,3,3868.18245,25975.3502
-2010/06/30,2011/06/30,4,4796.172364,25975.3502
-2010/06/30,2011/09/30,5,6866.351106,25975.3502
-2010/06/30,2011/12/31,6,6072.077117,25975.3502
-2010/06/30,2012/03/31,7,6013.984744,25975.3502
-2010/06/30,2012/06/30,8,5986.455679,25975.3502
-2010/06/30,2012/09/30,9,5787.881369,25975.3502
-2010/06/30,2012/12/31,10,5951.207315,25975.3502
-2010/06/30,2013/03/31,11,5957.566436,25975.3502
-2010/06/30,2013/06/30,12,6047.884556,25975.3502
-2010/06/30,2013/09/30,13,6064.741458,25975.3502
-2010/06/30,2013/12/31,14,5876.618428,25975.3502
-2010/06/30,2014/03/31,15,5969.354642,25975.3502
-2010/06/30,2014/06/30,16,5986.537057,25975.3502
-2010/06/30,2014/09/30,17,5997.383602,25975.3502
-2010/06/30,2014/12/31,18,5766.676548,25975.3502
-2010/09/30,2010/09/30,0,2373.056588,24954.4902
-2010/09/30,2010/12/31,1,4426.390053,24954.4902
-2010/09/30,2011/03/31,2,7274.148638,24954.4902
-2010/09/30,2011/06/30,3,6513.62333,24954.4902
-2010/09/30,2011/09/30,4,6699.130635,24954.4902
-2010/09/30,2011/12/31,5,7062.867711,24954.4902
-2010/09/30,2012/03/31,6,7602.893111,24954.4902
-2010/09/30,2012/06/30,7,7727.29705,24954.4902
-2010/09/30,2012/09/30,8,7130.492953,24954.4902
-2010/09/30,2012/12/31,9,7655.498271,24954.4902
-2010/09/30,2013/03/31,10,7948.796747,24954.4902
-2010/09/30,2013/06/30,11,8586.568929,24954.4902
-2010/09/30,2013/09/30,12,9113.050679,24954.4902
-2010/09/30,2013/12/31,13,7730.296416,24954.4902
-2010/09/30,2014/03/31,14,7925.092455,24954.4902
-2010/09/30,2014/06/30,15,8275.576519,24954.4902
-2010/09/30,2014/09/30,16,8179.631681,24954.4902
-2010/09/30,2014/12/31,17,7820.881922,24954.4902
-2010/12/31,2010/12/31,0,3664.585946,24478.1902
-2010/12/31,2011/03/31,1,6028.330549,24478.1902
-2010/12/31,2011/06/30,2,5679.334543,24478.1902
-2010/12/31,2011/09/30,3,5792.775683,24478.1902
-2010/12/31,2011/12/31,4,5157.665729,24478.1902
-2010/12/31,2012/03/31,5,5202.586468,24478.1902
-2010/12/31,2012/06/30,6,4824.10832,24478.1902
-2010/12/31,2012/09/30,7,4749.066041,24478.1902
-2010/12/31,2012/12/31,8,5152.469153,24478.1902
-2010/12/31,2013/03/31,9,5240.392431,24478.1902
-2010/12/31,2013/06/30,10,5260.829972,24478.1902
-2010/12/31,2013/09/30,11,5360.622834,24478.1902
-2010/12/31,2013/12/31,12,5261.911138,24478.1902
-2010/12/31,2014/03/31,13,5605.582689,24478.1902
-2010/12/31,2014/06/30,14,5472.92468,24478.1902
-2010/12/31,2014/09/30,15,5358.541878,24478.1902
-2010/12/31,2014/12/31,16,6050.686289,24478.1902
-2011/03/31,2011/03/31,0,3685.244371,23899.4402
-2011/03/31,2011/06/30,1,6009.229935,23899.4402
-2011/03/31,2011/09/30,2,6655.209685,23899.4402
-2011/03/31,2011/12/31,3,5535.06271,23899.4402
-2011/03/31,2012/03/31,4,6291.728368,23899.4402
-2011/03/31,2012/06/30,5,6971.88694,23899.4402
-2011/03/31,2012/09/30,6,6792.68063,23899.4402
-2011/03/31,2012/12/31,7,6362.015838,23899.4402
-2011/03/31,2013/03/31,8,6510.12407,23899.4402
-2011/03/31,2013/06/30,9,6456.658626,23899.4402
-2011/03/31,2013/09/30,10,6734.030235,23899.4402
-2011/03/31,2013/12/31,11,6836.148187,23899.4402
-2011/03/31,2014/03/31,12,7816.882767,23899.4402
-2011/03/31,2014/06/30,13,8117.493651,23899.4402
-2011/03/31,2014/09/30,14,8601.71689,23899.4402
-2011/03/31,2014/12/31,15,8508.050641,23899.4402
-2011/06/30,2011/06/30,0,5623.509132,21730.2502
-2011/06/30,2011/09/30,1,9330.190833,21730.2502
-2011/06/30,2011/12/31,2,8640.313384,21730.2502
-2011/06/30,2012/03/31,3,7675.807932,21730.2502
-2011/06/30,2012/06/30,4,7066.06471,21730.2502
-2011/06/30,2012/09/30,5,6535.025784,21730.2502
-2011/06/30,2012/12/31,6,7004.298695,21730.2502
-2011/06/30,2013/03/31,7,6964.644285,21730.2502
-2011/06/30,2013/06/30,8,7006.577283,21730.2502
-2011/06/30,2013/09/30,9,7243.748086,21730.2502
-2011/06/30,2013/12/31,10,7123.773443,21730.2502
-2011/06/30,2014/03/31,11,7118.960507,21730.2502
-2011/06/30,2014/06/30,12,7294.074659,21730.2502
-2011/06/30,2014/09/30,13,7250.979116,21730.2502
-2011/06/30,2014/12/31,14,6981.222177,21730.2502
-2011/09/30,2011/09/30,0,6359.527992,15231.7602
-2011/09/30,2011/12/31,1,8484.695112,15231.7602
-2011/09/30,2012/03/31,2,9147.194626,15231.7602
-2011/09/30,2012/06/30,3,6628.157263,15231.7602
-2011/09/30,2012/09/30,4,6883.138256,15231.7602
-2011/09/30,2012/12/31,5,6989.906388,15231.7602
-2011/09/30,2013/03/31,6,7416.58365,15231.7602
-2011/09/30,2013/06/30,7,7768.218634,15231.7602
-2011/09/30,2013/09/30,8,8116.935629,15231.7602
-2011/09/30,2013/12/31,9,7775.496165,15231.7602
-2011/09/30,2014/03/31,10,7907.968167,15231.7602
-2011/09/30,2014/06/30,11,7946.192646,15231.7602
-2011/09/30,2014/09/30,12,7905.085056,15231.7602
-2011/09/30,2014/12/31,13,7503.623394,15231.7602
-2011/12/31,2011/12/31,0,3654.86707,11990.0202
-2011/12/31,2012/03/31,1,4337.501863,11990.0202
-2011/12/31,2012/06/30,2,3999.759293,11990.0202
-2011/12/31,2012/09/30,3,4567.848528,11990.0202
-2011/12/31,2012/12/31,4,6659.162338,11990.0202
-2011/12/31,2013/03/31,5,6570.506657,11990.0202
-2011/12/31,2013/06/30,6,6598.896005,11990.0202
-2011/12/31,2013/09/30,7,6949.194062,11990.0202
-2011/12/31,2013/12/31,8,7302.991379,11990.0202
-2011/12/31,2014/03/31,9,7384.113769,11990.0202
-2011/12/31,2014/06/30,10,8192.291796,11990.0202
-2011/12/31,2014/09/30,11,8634.616914,11990.0202
-2011/12/31,2014/12/31,12,8644.114906,11990.0202
-2012/03/31,2012/03/31,0,1202.803924,11731.1402
-2012/03/31,2012/06/30,1,2897.120245,11731.1402
-2012/03/31,2012/09/30,2,3288.560769,11731.1402
-2012/03/31,2012/12/31,3,2418.360967,11731.1402
-2012/03/31,2013/03/31,4,2197.326288,11731.1402
-2012/03/31,2013/06/30,5,3144.428441,11731.1402
-2012/03/31,2013/09/30,6,3153.228906,11731.1402
-2012/03/31,2013/12/31,7,3073.071429,11731.1402
-2012/03/31,2014/03/31,8,3108.656931,11731.1402
-2012/03/31,2014/06/30,9,2366.918351,11731.1402
-2012/03/31,2014/09/30,10,1991.509322,11731.1402
-2012/03/31,2014/12/31,11,2082.80398,11731.1402
-2012/06/30,2012/06/30,0,1110.253717,11502.8702
-2012/06/30,2012/09/30,1,2110.96082,11502.8702
-2012/06/30,2012/12/31,2,3328.017546,11502.8702
-2012/06/30,2013/03/31,3,5474.017472,11502.8702
-2012/06/30,2013/06/30,4,5593.375966,11502.8702
-2012/06/30,2013/09/30,5,5660.38506,11502.8702
-2012/06/30,2013/12/31,6,4710.016155,11502.8702
-2012/06/30,2014/03/31,7,4873.516482,11502.8702
-2012/06/30,2014/06/30,8,4568.569306,11502.8702
-2012/06/30,2014/09/30,9,4547.131976,11502.8702
-2012/06/30,2014/12/31,10,4600.667173,11502.8702
-2012/09/30,2012/09/30,0,775.7081453,13316.5402
-2012/09/30,2012/12/31,1,3290.351088,13316.5402
-2012/09/30,2013/03/31,2,6314.549126,13316.5402
-2012/09/30,2013/06/30,3,7099.383249,13316.5402
-2012/09/30,2013/09/30,4,7206.38389,13316.5402
-2012/09/30,2013/12/31,5,6951.123887,13316.5402
-2012/09/30,2014/03/31,6,6910.562692,13316.5402
-2012/09/30,2014/06/30,7,6848.320033,13316.5402
-2012/09/30,2014/09/30,8,6906.168272,13316.5402
-2012/09/30,2014/12/31,9,6825.708533,13316.5402
-2012/12/31,2012/12/31,0,1857.653892,14269.7402
-2012/12/31,2013/03/31,1,3064.352342,14269.7402
-2012/12/31,2013/06/30,2,3964.894568,14269.7402
-2012/12/31,2013/09/30,3,3906.174421,14269.7402
-2012/12/31,2013/12/31,4,4058.235306,14269.7402
-2012/12/31,2014/03/31,5,4269.934748,14269.7402
-2012/12/31,2014/06/30,6,4018.813405,14269.7402
-2012/12/31,2014/09/30,7,3867.275665,14269.7402
-2012/12/31,2014/12/31,8,5107.385658,14269.7402
-2013/03/31,2013/03/31,0,1607.706719,15193.1202
-2013/03/31,2013/06/30,1,4000.340565,15193.1202
-2013/03/31,2013/09/30,2,4989.08508,15193.1202
-2013/03/31,2013/12/31,3,4800.183144,15193.1202
-2013/03/31,2014/03/31,4,4794.533176,15193.1202
-2013/03/31,2014/06/30,5,5481.643767,15193.1202
-2013/03/31,2014/09/30,6,4777.978535,15193.1202
-2013/03/31,2014/12/31,7,4847.149962,15193.1202
-2013/06/30,2013/06/30,0,3120.317258,15076.7802
-2013/06/30,2013/09/30,1,3906.220923,15076.7802
-2013/06/30,2013/12/31,2,7001.938728,15076.7802
-2013/06/30,2014/03/31,3,9182.175605,15076.7802
-2013/06/30,2014/06/30,4,9679.802988,15076.7802
-2013/06/30,2014/09/30,5,7915.826971,15076.7802
-2013/06/30,2014/12/31,6,10125.44136,15076.7802
-2013/09/30,2013/09/30,0,1186.749178,18804.4802
-2013/09/30,2013/12/31,1,1948.716041,18804.4802
-2013/09/30,2014/03/31,2,3061.969125,18804.4802
-2013/09/30,2014/06/30,3,4515.324745,18804.4802
-2013/09/30,2014/09/30,4,4628.405496,18804.4802
-2013/09/30,2014/12/31,5,4755.134526,18804.4802
-2013/12/31,2013/12/31,0,508.1251647,17929.9502
-2013/12/31,2014/03/31,1,1844.156745,17929.9502
-2013/12/31,2014/06/30,2,4444.653635,17929.9502
-2013/12/31,2014/09/30,3,6455.914597,17929.9502
-2013/12/31,2014/12/31,4,7419.199377,17929.9502
-2014/03/31,2014/03/31,0,631.9129553,18824.7102
-2014/03/31,2014/06/30,1,1950.552862,18824.7102
-2014/03/31,2014/09/30,2,2235.318258,18824.7102
-2014/03/31,2014/12/31,3,4024.533126,18824.7102
-2014/06/30,2014/06/30,0,575.9015377,20181.3402
-2014/06/30,2014/09/30,1,3531.009527,20181.3402
-2014/06/30,2014/12/31,2,8147.766322,20181.3402
-2014/09/30,2014/09/30,0,1548.602932,20891.3602
-2014/09/30,2014/12/31,1,4806.751524,20891.3602
-2014/12/31,2014/12/31,0,1877.010266,23653.9902
+origin,development,lag,claim,premium
+2010/03/31,2010/03/31,0,15885.64381,51346.66641
+2010/03/31,2010/06/30,1,25177.51136,51346.66641
+2010/03/31,2010/09/30,2,26571.78973,51346.66641
+2010/03/31,2010/12/31,3,25520.48766,51346.66641
+2010/03/31,2011/03/31,4,25047.47172,51346.66641
+2010/03/31,2011/06/30,5,25025.26462,51346.66641
+2010/03/31,2011/09/30,6,24961.98862,51346.66641
+2010/03/31,2011/12/31,7,24447.97496,51346.66641
+2010/03/31,2012/03/31,8,24411.81725,51346.66641
+2010/03/31,2012/06/30,9,24305.19471,51346.66641
+2010/03/31,2012/09/30,10,24305.07608,51346.66641
+2010/03/31,2012/12/31,11,24285.31271,51346.66641
+2010/03/31,2013/03/31,12,24201.01589,51346.66641
+2010/03/31,2013/06/30,13,24159.40131,51346.66641
+2010/03/31,2013/09/30,14,24170.83702,51346.66641
+2010/03/31,2013/12/31,15,24108.41514,51346.66641
+2010/03/31,2014/03/31,16,24096.95571,51346.66641
+2010/03/31,2014/06/30,17,24096.95571,51346.66641
+2010/03/31,2014/09/30,18,24096.95571,51346.66641
+2010/03/31,2014/12/31,19,24096.95571,51346.66641
+2010/06/30,2010/06/30,0,18399.93339,53877.27641
+2010/06/30,2010/09/30,1,24209.50963,53877.27641
+2010/06/30,2010/12/31,2,22952.86308,53877.27641
+2010/06/30,2011/03/31,3,22781.44611,53877.27641
+2010/06/30,2011/06/30,4,22709.81873,53877.27641
+2010/06/30,2011/09/30,5,22939.48188,53877.27641
+2010/06/30,2011/12/31,6,22276.51933,53877.27641
+2010/06/30,2012/03/31,7,22394.64875,53877.27641
+2010/06/30,2012/06/30,8,22331.79982,53877.27641
+2010/06/30,2012/09/30,9,22614.84542,53877.27641
+2010/06/30,2012/12/31,10,22614.84542,53877.27641
+2010/06/30,2013/03/31,11,22614.75052,53877.27641
+2010/06/30,2013/06/30,12,22614.75052,53877.27641
+2010/06/30,2013/09/30,13,22614.75052,53877.27641
+2010/06/30,2013/12/31,14,22593.94322,53877.27641
+2010/06/30,2014/03/31,15,22590.24204,53877.27641
+2010/06/30,2014/06/30,16,22592.40107,53877.27641
+2010/06/30,2014/09/30,17,22592.40107,53877.27641
+2010/06/30,2014/12/31,18,22592.40107,53877.27641
+2010/09/30,2010/09/30,0,15765.26046,54577.09641
+2010/09/30,2010/12/31,1,18859.94774,54577.09641
+2010/09/30,2011/03/31,2,17972.3044,54577.09641
+2010/09/30,2011/06/30,3,18029.22195,54577.09641
+2010/09/30,2011/09/30,4,18099.71051,54577.09641
+2010/09/30,2011/12/31,5,17914.79371,54577.09641
+2010/09/30,2012/03/31,6,17918.92195,54577.09641
+2010/09/30,2012/06/30,7,17802.40586,54577.09641
+2010/09/30,2012/09/30,8,17854.41223,54577.09641
+2010/09/30,2012/12/31,9,17854.3885,54577.09641
+2010/09/30,2013/03/31,10,17867.88833,54577.09641
+2010/09/30,2013/06/30,11,17843.83064,54577.09641
+2010/09/30,2013/09/30,12,17828.90728,54577.09641
+2010/09/30,2013/12/31,13,17828.90728,54577.09641
+2010/09/30,2014/03/31,14,17762.30971,54577.09641
+2010/09/30,2014/06/30,15,17762.30971,54577.09641
+2010/09/30,2014/09/30,16,17754.29048,54577.09641
+2010/09/30,2014/12/31,17,17754.29048,54577.09641
+2010/12/31,2010/12/31,0,18049.1514,55527.48641
+2010/12/31,2011/03/31,1,24586.08129,55527.48641
+2010/12/31,2011/06/30,2,24557.61065,55527.48641
+2010/12/31,2011/09/30,3,24341.73203,55527.48641
+2010/12/31,2011/12/31,4,23850.18645,55527.48641
+2010/12/31,2012/03/31,5,23923.40344,55527.48641
+2010/12/31,2012/06/30,6,23912.37107,55527.48641
+2010/12/31,2012/09/30,7,23959.22899,55527.48641
+2010/12/31,2012/12/31,8,23949.21682,55527.48641
+2010/12/31,2013/03/31,9,23823.18679,55527.48641
+2010/12/31,2013/06/30,10,23921.38677,55527.48641
+2010/12/31,2013/09/30,11,23836.0223,55527.48641
+2010/12/31,2013/12/31,12,23862.87961,55527.48641
+2010/12/31,2014/03/31,13,23862.85588,55527.48641
+2010/12/31,2014/06/30,14,23853.15214,55527.48641
+2010/12/31,2014/09/30,15,23829.94857,55527.48641
+2010/12/31,2014/12/31,16,23829.94857,55527.48641
+2011/03/31,2011/03/31,0,22716.20089,56767.61641
+2011/03/31,2011/06/30,1,28799.4986,56767.61641
+2011/03/31,2011/09/30,2,28139.21703,56767.61641
+2011/03/31,2011/12/31,3,26890.42363,56767.61641
+2011/03/31,2012/03/31,4,27203.1736,56767.61641
+2011/03/31,2012/06/30,5,27014.27091,56767.61641
+2011/03/31,2012/09/30,6,26813.00722,56767.61641
+2011/03/31,2012/12/31,7,26542.22772,56767.61641
+2011/03/31,2013/03/31,8,26363.69308,56767.61641
+2011/03/31,2013/06/30,9,26522.72533,56767.61641
+2011/03/31,2013/09/30,10,26259.32447,56767.61641
+2011/03/31,2013/12/31,11,26256.54858,56767.61641
+2011/03/31,2014/03/31,12,26050.51605,56767.61641
+2011/03/31,2014/06/30,13,26000.57381,56767.61641
+2011/03/31,2014/09/30,14,26000.57381,56767.61641
+2011/03/31,2014/12/31,15,26000.57381,56767.61641
+2011/06/30,2011/06/30,0,17629.56535,57243.72641
+2011/06/30,2011/09/30,1,24164.4074,57243.72641
+2011/06/30,2011/12/31,2,23772.50905,57243.72641
+2011/06/30,2012/03/31,3,23060.50582,57243.72641
+2011/06/30,2012/06/30,4,22775.34865,57243.72641
+2011/06/30,2012/09/30,5,22658.66648,57243.72641
+2011/06/30,2012/12/31,6,22348.52632,57243.72641
+2011/06/30,2013/03/31,7,22241.50044,57243.72641
+2011/06/30,2013/06/30,8,22254.90537,57243.72641
+2011/06/30,2013/09/30,9,22228.85473,57243.72641
+2011/06/30,2013/12/31,10,22228.85473,57243.72641
+2011/06/30,2014/03/31,11,22197.63193,57243.72641
+2011/06/30,2014/06/30,12,22114.45021,57243.72641
+2011/06/30,2014/09/30,13,22062.42012,57243.72641
+2011/06/30,2014/12/31,14,22062.42012,57243.72641
+2011/09/30,2011/09/30,0,20852.10953,58405.12641
+2011/09/30,2011/12/31,1,28044.43353,58405.12641
+2011/09/30,2012/03/31,2,27322.34695,58405.12641
+2011/09/30,2012/06/30,3,27051.21156,58405.12641
+2011/09/30,2012/09/30,4,26749.75495,58405.12641
+2011/09/30,2012/12/31,5,26292.91982,58405.12641
+2011/09/30,2013/03/31,6,26136.59229,58405.12641
+2011/09/30,2013/06/30,7,26133.00973,58405.12641
+2011/09/30,2013/09/30,8,26309.78867,58405.12641
+2011/09/30,2013/12/31,9,26223.90225,58405.12641
+2011/09/30,2014/03/31,10,25942.89704,58405.12641
+2011/09/30,2014/06/30,11,25952.4347,58405.12641
+2011/09/30,2014/09/30,12,25941.99547,58405.12641
+2011/09/30,2014/12/31,13,25940.09743,58405.12641
+2011/12/31,2011/12/31,0,21489.49596,59911.59641
+2011/12/31,2012/03/31,1,32918.53575,59911.59641
+2011/12/31,2012/06/30,2,32872.43704,59911.59641
+2011/12/31,2012/09/30,3,32830.06324,59911.59641
+2011/12/31,2012/12/31,4,32575.06122,59911.59641
+2011/12/31,2013/03/31,5,32552.94902,59911.59641
+2011/12/31,2013/06/30,6,32536.26997,59911.59641
+2011/12/31,2013/09/30,7,32443.52686,59911.59641
+2011/12/31,2013/12/31,8,32453.46786,59911.59641
+2011/12/31,2014/03/31,9,32324.49587,59911.59641
+2011/12/31,2014/06/30,10,32324.49587,59911.59641
+2011/12/31,2014/09/30,11,32495.50951,59911.59641
+2011/12/31,2014/12/31,12,32474.15653,59911.59641
+2012/03/31,2012/03/31,0,18254.16372,60339.49641
+2012/03/31,2012/06/30,1,29871.29953,60339.49641
+2012/03/31,2012/09/30,2,30149.22042,60339.49641
+2012/03/31,2012/12/31,3,29904.39665,60339.49641
+2012/03/31,2013/03/31,4,30122.22077,60339.49641
+2012/03/31,2013/06/30,5,30281.72752,60339.49641
+2012/03/31,2013/09/30,6,30003.61683,60339.49641
+2012/03/31,2013/12/31,7,30047.31926,60339.49641
+2012/03/31,2014/03/31,8,29792.98155,60339.49641
+2012/03/31,2014/06/30,9,29747.97422,60339.49641
+2012/03/31,2014/09/30,10,29722.30319,60339.49641
+2012/03/31,2014/12/31,11,29755.30541,60339.49641
+2012/06/30,2012/06/30,0,21811.61752,61308.49641
+2012/06/30,2012/09/30,1,29825.69906,61308.49641
+2012/06/30,2012/12/31,2,28046.97216,61308.49641
+2012/06/30,2013/03/31,3,27959.59103,61308.49641
+2012/06/30,2013/06/30,4,28009.27229,61308.49641
+2012/06/30,2013/09/30,5,27812.51645,61308.49641
+2012/06/30,2013/12/31,6,27604.58588,61308.49641
+2012/06/30,2014/03/31,7,27430.53538,61308.49641
+2012/06/30,2014/06/30,8,27502.7559,61308.49641
+2012/06/30,2014/09/30,9,27206.96969,61308.49641
+2012/06/30,2014/12/31,10,27183.78984,61308.49641
+2012/09/30,2012/09/30,0,25062.3239,60262.30641
+2012/09/30,2012/12/31,1,35858.55629,60262.30641
+2012/09/30,2013/03/31,2,36143.49993,60262.30641
+2012/09/30,2013/06/30,3,35174.40683,60262.30641
+2012/09/30,2013/09/30,4,34845.02526,60262.30641
+2012/09/30,2013/12/31,5,34032.33087,60262.30641
+2012/09/30,2014/03/31,6,33252.09301,60262.30641
+2012/09/30,2014/06/30,7,33128.10338,60262.30641
+2012/09/30,2014/09/30,8,32078.79425,60262.30641
+2012/09/30,2014/12/31,9,32282.07462,60262.30641
+2012/12/31,2012/12/31,0,27478.65076,60512.84641
+2012/12/31,2013/03/31,1,41905.36413,60512.84641
+2012/12/31,2013/06/30,2,42866.65153,60512.84641
+2012/12/31,2013/09/30,3,42488.20556,60512.84641
+2012/12/31,2013/12/31,4,42368.36789,60512.84641
+2012/12/31,2014/03/31,5,41576.12491,60512.84641
+2012/12/31,2014/06/30,6,41451.42351,60512.84641
+2012/12/31,2014/09/30,7,40987.37582,60512.84641
+2012/12/31,2014/12/31,8,41403.85382,60512.84641
+2013/03/31,2013/03/31,0,26771.0842,62668.15641
+2013/03/31,2013/06/30,1,40483.56414,62668.15641
+2013/03/31,2013/09/30,2,39967.65244,62668.15641
+2013/03/31,2013/12/31,3,40057.5722,62668.15641
+2013/03/31,2014/03/31,4,40010.85663,62668.15641
+2013/03/31,2014/06/30,5,38822.58706,62668.15641
+2013/03/31,2014/09/30,6,38480.74959,62668.15641
+2013/03/31,2014/12/31,7,38506.08846,62668.15641
+2013/06/30,2013/06/30,0,20361.60787,63109.32641
+2013/06/30,2013/09/30,1,26804.96426,63109.32641
+2013/06/30,2013/12/31,2,26388.29646,63109.32641
+2013/06/30,2014/03/31,3,26454.27717,63109.32641
+2013/06/30,2014/06/30,4,26380.03998,63109.32641
+2013/06/30,2014/09/30,5,26321.22438,63109.32641
+2013/06/30,2014/12/31,6,26310.42926,63109.32641
+2013/09/30,2013/09/30,0,19766.45289,62933.52641
+2013/09/30,2013/12/31,1,29064.96359,62933.52641
+2013/09/30,2014/03/31,2,28266.90785,62933.52641
+2013/09/30,2014/06/30,3,27855.69692,62933.52641
+2013/09/30,2014/09/30,4,27475.28173,62933.52641
+2013/09/30,2014/12/31,5,27402.4918,62933.52641
+2013/12/31,2013/12/31,0,27034.74604,63694.44641
+2013/12/31,2014/03/31,1,43552.72275,63694.44641
+2013/12/31,2014/06/30,2,45623.39232,63694.44641
+2013/12/31,2014/09/30,3,45858.20392,63694.44641
+2013/12/31,2014/12/31,4,45471.02695,63694.44641
+2014/03/31,2014/03/31,0,19600.13691,64467.46641
+2014/03/31,2014/06/30,1,35431.71023,64467.46641
+2014/03/31,2014/09/30,2,37810.95408,64467.46641
+2014/03/31,2014/12/31,3,38378.89588,64467.46641
+2014/06/30,2014/06/30,0,22220.45589,66842.73641
+2014/06/30,2014/09/30,1,35361.36403,66842.73641
+2014/06/30,2014/12/31,2,38685.95172,66842.73641
+2014/09/30,2014/09/30,0,22583.36164,68593.77641
+2014/09/30,2014/12/31,1,34819.30679,68593.77641
+2014/12/31,2014/12/31,0,25472.84679,69620.50641
```

### Comparing `tryangle-0.2.1/src/tryangle/utils/data/sme_test.csv` & `tryangle-0.2.2.dev0/src/tryangle/utils/data/sme_test.csv`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,211 +1,211 @@
-﻿origin,development,lag,claim,premium
-2010/03/31,2015/03/31,20,24096.95571,0
-2010/06/30,2015/03/31,19,22592.40107,0
-2010/06/30,2015/06/30,20,22589.88616,0
-2010/09/30,2015/03/31,18,17754.29048,0
-2010/09/30,2015/06/30,19,17754.29048,0
-2010/09/30,2015/09/30,20,17754.29048,0
-2010/12/31,2015/03/31,17,23829.94857,0
-2010/12/31,2015/06/30,18,23829.94857,0
-2010/12/31,2015/09/30,19,23828.50131,0
-2010/12/31,2015/12/31,20,23774.35964,0
-2011/03/31,2015/03/31,16,26000.57381,0
-2011/03/31,2015/06/30,17,26000.57381,0
-2011/03/31,2015/09/30,18,26000.57381,0
-2011/03/31,2015/12/31,19,26000.57381,0
-2011/03/31,2016/03/31,20,26000.57381,0
-2011/06/30,2015/03/31,15,22062.42012,0
-2011/06/30,2015/06/30,16,22062.42012,0
-2011/06/30,2015/09/30,17,22062.42012,0
-2011/06/30,2015/12/31,18,22062.42012,0
-2011/06/30,2016/03/31,19,22062.42012,0
-2011/06/30,2016/06/30,20,22062.42012,0
-2011/09/30,2015/03/31,14,25940.09743,0
-2011/09/30,2015/06/30,15,25940.09743,0
-2011/09/30,2015/09/30,16,25940.09743,0
-2011/09/30,2015/12/31,17,25940.09743,0
-2011/09/30,2016/03/31,18,25927.68897,0
-2011/09/30,2016/06/30,19,25921.44916,0
-2011/09/30,2016/09/30,20,25931.95957,0
-2011/12/31,2015/03/31,13,32463.95455,0
-2011/12/31,2015/06/30,14,32463.95455,0
-2011/12/31,2015/09/30,15,32463.95455,0
-2011/12/31,2015/12/31,16,32463.95455,0
-2011/12/31,2016/03/31,17,32463.95455,0
-2011/12/31,2016/06/30,18,32463.95455,0
-2011/12/31,2016/09/30,19,32463.95455,0
-2011/12/31,2016/12/31,20,32463.95455,0
-2012/03/31,2015/03/31,12,29765.69719,0
-2012/03/31,2015/06/30,13,29764.65326,0
-2012/03/31,2015/09/30,14,29763.63307,0
-2012/03/31,2015/12/31,15,29763.63307,0
-2012/03/31,2016/03/31,16,29763.63307,0
-2012/03/31,2016/06/30,17,29763.63307,0
-2012/03/31,2016/09/30,18,29759.90816,0
-2012/03/31,2016/12/31,19,29759.90816,0
-2012/03/31,2017/03/31,20,29759.90816,0
-2012/06/30,2015/03/31,11,27184.00337,0
-2012/06/30,2015/06/30,12,27184.00337,0
-2012/06/30,2015/09/30,13,27184.00337,0
-2012/06/30,2015/12/31,14,27043.73802,0
-2012/06/30,2016/03/31,15,27043.73802,0
-2012/06/30,2016/06/30,16,27043.73802,0
-2012/06/30,2016/09/30,17,27043.73802,0
-2012/06/30,2016/12/31,18,27043.73802,0
-2012/06/30,2017/03/31,19,27043.73802,0
-2012/06/30,2017/06/30,20,27043.73802,0
-2012/09/30,2015/03/31,10,32479.8032,0
-2012/09/30,2015/06/30,11,32317.23586,0
-2012/09/30,2015/09/30,12,32441.72372,0
-2012/09/30,2015/12/31,13,32413.25309,0
-2012/09/30,2016/03/31,14,32454.13218,0
-2012/09/30,2016/06/30,15,32454.13218,0
-2012/09/30,2016/09/30,16,32560.84962,0
-2012/09/30,2016/12/31,17,32564.50335,0
-2012/09/30,2017/03/31,18,32564.50335,0
-2012/09/30,2017/06/30,19,32560.56492,0
-2012/09/30,2017/09/30,20,32560.56492,0
-2012/12/31,2015/03/31,9,41486.03907,0
-2012/12/31,2015/06/30,10,41475.59983,0
-2012/12/31,2015/09/30,11,41551.30801,0
-2012/12/31,2015/12/31,12,41551.30801,0
-2012/12/31,2016/03/31,13,41551.30801,0
-2012/12/31,2016/06/30,14,41551.30801,0
-2012/12/31,2016/09/30,15,41583.40865,0
-2012/12/31,2016/12/31,16,41583.40865,0
-2012/12/31,2017/03/31,17,41583.40865,0
-2012/12/31,2017/06/30,18,41255.9963,0
-2012/12/31,2017/09/30,19,41214.38172,0
-2012/12/31,2017/12/31,20,41214.38172,0
-2013/03/31,2015/03/31,8,38508.0814,0
-2013/03/31,2015/06/30,9,38516.29044,0
-2013/03/31,2015/09/30,10,38526.65849,0
-2013/03/31,2015/12/31,11,38510.71494,0
-2013/03/31,2016/03/31,12,38510.71494,0
-2013/03/31,2016/06/30,13,38510.71494,0
-2013/03/31,2016/09/30,14,38776.89169,0
-2013/03/31,2016/12/31,15,38729.01356,0
-2013/03/31,2017/03/31,16,38726.64101,0
-2013/03/31,2017/06/30,17,38726.64101,0
-2013/03/31,2017/09/30,18,38726.64101,0
-2013/03/31,2017/12/31,19,38726.64101,0
-2013/03/31,2018/03/31,20,38737.05652,0
-2013/06/30,2015/03/31,7,26322.95634,0
-2013/06/30,2015/06/30,8,26318.30614,0
-2013/06/30,2015/09/30,9,26309.00573,0
-2013/06/30,2015/12/31,10,26621.18629,0
-2013/06/30,2016/03/31,11,26621.18629,0
-2013/06/30,2016/06/30,12,26639.73965,0
-2013/06/30,2016/09/30,13,26639.73965,0
-2013/06/30,2016/12/31,14,26624.34178,0
-2013/06/30,2017/03/31,15,26624.34178,0
-2013/06/30,2017/06/30,16,26623.63002,0
-2013/06/30,2017/09/30,17,26623.63002,0
-2013/06/30,2017/12/31,18,26623.63002,0
-2013/06/30,2018/03/31,19,26623.63002,0
-2013/06/30,2018/06/30,20,26623.63002,0
-2013/09/30,2015/03/31,6,27364.72075,0
-2013/09/30,2015/06/30,7,27262.70096,0
-2013/09/30,2015/09/30,8,27243.91034,0
-2013/09/30,2015/12/31,9,27246.16426,0
-2013/09/30,2016/03/31,10,27256.55605,0
-2013/09/30,2016/06/30,11,27246.14054,0
-2013/09/30,2016/09/30,12,27246.14054,0
-2013/09/30,2016/12/31,13,27258.64389,0
-2013/09/30,2017/03/31,14,27258.64389,0
-2013/09/30,2017/06/30,15,27258.64389,0
-2013/09/30,2017/09/30,16,27258.64389,0
-2013/09/30,2017/12/31,17,27258.64389,0
-2013/09/30,2018/03/31,18,27258.64389,0
-2013/09/30,2018/06/30,19,27258.66762,0
-2013/09/30,2018/09/30,20,27258.64389,0
-2013/12/31,2015/03/31,5,45806.36363,0
-2013/12/31,2015/06/30,6,44432.8451,0
-2013/12/31,2015/09/30,7,44633.70546,0
-2013/12/31,2015/12/31,8,44637.71508,0
-2013/12/31,2016/03/31,9,44694.01577,0
-2013/12/31,2016/06/30,10,44694.01577,0
-2013/12/31,2016/09/30,11,44683.57653,0
-2013/12/31,2016/12/31,12,44481.43499,0
-2013/12/31,2017/03/31,13,44528.71998,0
-2013/12/31,2017/06/30,14,44567.20279,0
-2013/12/31,2017/09/30,15,44675.6522,0
-2013/12/31,2017/12/31,16,44707.04108,0
-2013/12/31,2018/03/31,17,44790.29398,0
-2013/12/31,2018/06/30,18,44837.1519,0
-2013/12/31,2018/09/30,19,44883.06081,0
-2013/12/31,2018/12/31,20,44814.47029,0
-2014/03/31,2015/03/31,4,37946.52177,0
-2014/03/31,2015/06/30,5,37692.44505,0
-2014/03/31,2015/09/30,6,37686.37131,0
-2014/03/31,2015/12/31,7,37629.2165,0
-2014/03/31,2016/03/31,8,37634.19886,0
-2014/03/31,2016/06/30,9,37634.19886,0
-2014/03/31,2016/09/30,10,37612.44255,0
-2014/03/31,2016/12/31,11,37612.44255,0
-2014/03/31,2017/03/31,12,37599.79684,0
-2014/03/31,2017/06/30,13,37599.79684,0
-2014/03/31,2017/09/30,14,37599.79684,0
-2014/03/31,2017/12/31,15,37599.79684,0
-2014/03/31,2018/03/31,16,37599.79684,0
-2014/03/31,2018/06/30,17,37599.82057,0
-2014/03/31,2018/09/30,18,37599.82057,0
-2014/03/31,2018/12/31,19,37599.79684,0
-2014/03/31,2019/03/31,20,37599.82057,0
-2014/06/30,2015/03/31,3,38611.97551,0
-2014/06/30,2015/06/30,4,37948.23001,0
-2014/06/30,2015/09/30,5,38007.56757,0
-2014/06/30,2015/12/31,6,38109.23148,0
-2014/06/30,2016/03/31,7,38098.74479,0
-2014/06/30,2016/06/30,8,38210.08871,0
-2014/06/30,2016/09/30,9,38178.84219,0
-2014/06/30,2016/12/31,10,38178.84219,0
-2014/06/30,2017/03/31,11,38177.65591,0
-2014/06/30,2017/06/30,12,38177.65591,0
-2014/06/30,2017/09/30,13,38177.65591,0
-2014/06/30,2017/12/31,14,38177.65591,0
-2014/06/30,2018/03/31,15,38177.65591,0
-2014/06/30,2018/06/30,16,38177.65591,0
-2014/06/30,2018/09/30,17,38177.65591,0
-2014/06/30,2018/12/31,18,38175.40199,0
-2014/06/30,2019/03/31,19,38175.40199,0
-2014/06/30,2019/06/30,20,38185.72259,0
-2014/09/30,2015/03/31,2,35282.14447,0
-2014/09/30,2015/06/30,3,34872.14355,0
-2014/09/30,2015/09/30,4,35780.52301,0
-2014/09/30,2015/12/31,5,35467.41716,0
-2014/09/30,2016/03/31,6,35473.39599,0
-2014/09/30,2016/06/30,7,35477.31071,0
-2014/09/30,2016/09/30,8,35450.19242,0
-2014/09/30,2016/12/31,9,35662.91555,0
-2014/09/30,2017/03/31,10,35628.34744,0
-2014/09/30,2017/06/30,11,35557.69281,0
-2014/09/30,2017/09/30,12,35557.69281,0
-2014/09/30,2017/12/31,13,35563.69537,0
-2014/09/30,2018/03/31,14,35563.69537,0
-2014/09/30,2018/06/30,15,35576.12755,0
-2014/09/30,2018/09/30,16,35576.12755,0
-2014/09/30,2018/12/31,17,35570.88421,0
-2014/09/30,2019/03/31,18,35570.88421,0
-2014/09/30,2019/06/30,19,35568.91499,0
-2014/09/30,2019/09/30,20,35555.58124,0
-2014/12/31,2015/03/31,1,35454.98498,0
-2014/12/31,2015/06/30,2,36729.97137,0
-2014/12/31,2015/09/30,3,37065.5453,0
-2014/12/31,2015/12/31,4,36676.58892,0
-2014/12/31,2016/03/31,5,36631.46296,0
-2014/12/31,2016/06/30,6,36391.88253,0
-2014/12/31,2016/09/30,7,36360.65973,0
-2014/12/31,2016/12/31,8,36376.36603,0
-2014/12/31,2017/03/31,9,36386.78154,0
-2014/12/31,2017/06/30,10,36420.49552,0
-2014/12/31,2017/09/30,11,36420.49552,0
-2014/12/31,2017/12/31,12,36430.91103,0
-2014/12/31,2018/03/31,13,36445.02772,0
-2014/12/31,2018/06/30,14,36449.70165,0
-2014/12/31,2018/09/30,15,36449.86773,0
-2014/12/31,2018/12/31,16,36436.98477,0
-2014/12/31,2019/03/31,17,36436.98477,0
-2014/12/31,2019/06/30,18,36436.98477,0
-2014/12/31,2019/09/30,19,36436.98477,0
-2014/12/31,2019/12/31,20,36436.98477,0
+﻿origin,development,lag,claim,premium
+2010/03/31,2015/03/31,20,24096.95571,0
+2010/06/30,2015/03/31,19,22592.40107,0
+2010/06/30,2015/06/30,20,22589.88616,0
+2010/09/30,2015/03/31,18,17754.29048,0
+2010/09/30,2015/06/30,19,17754.29048,0
+2010/09/30,2015/09/30,20,17754.29048,0
+2010/12/31,2015/03/31,17,23829.94857,0
+2010/12/31,2015/06/30,18,23829.94857,0
+2010/12/31,2015/09/30,19,23828.50131,0
+2010/12/31,2015/12/31,20,23774.35964,0
+2011/03/31,2015/03/31,16,26000.57381,0
+2011/03/31,2015/06/30,17,26000.57381,0
+2011/03/31,2015/09/30,18,26000.57381,0
+2011/03/31,2015/12/31,19,26000.57381,0
+2011/03/31,2016/03/31,20,26000.57381,0
+2011/06/30,2015/03/31,15,22062.42012,0
+2011/06/30,2015/06/30,16,22062.42012,0
+2011/06/30,2015/09/30,17,22062.42012,0
+2011/06/30,2015/12/31,18,22062.42012,0
+2011/06/30,2016/03/31,19,22062.42012,0
+2011/06/30,2016/06/30,20,22062.42012,0
+2011/09/30,2015/03/31,14,25940.09743,0
+2011/09/30,2015/06/30,15,25940.09743,0
+2011/09/30,2015/09/30,16,25940.09743,0
+2011/09/30,2015/12/31,17,25940.09743,0
+2011/09/30,2016/03/31,18,25927.68897,0
+2011/09/30,2016/06/30,19,25921.44916,0
+2011/09/30,2016/09/30,20,25931.95957,0
+2011/12/31,2015/03/31,13,32463.95455,0
+2011/12/31,2015/06/30,14,32463.95455,0
+2011/12/31,2015/09/30,15,32463.95455,0
+2011/12/31,2015/12/31,16,32463.95455,0
+2011/12/31,2016/03/31,17,32463.95455,0
+2011/12/31,2016/06/30,18,32463.95455,0
+2011/12/31,2016/09/30,19,32463.95455,0
+2011/12/31,2016/12/31,20,32463.95455,0
+2012/03/31,2015/03/31,12,29765.69719,0
+2012/03/31,2015/06/30,13,29764.65326,0
+2012/03/31,2015/09/30,14,29763.63307,0
+2012/03/31,2015/12/31,15,29763.63307,0
+2012/03/31,2016/03/31,16,29763.63307,0
+2012/03/31,2016/06/30,17,29763.63307,0
+2012/03/31,2016/09/30,18,29759.90816,0
+2012/03/31,2016/12/31,19,29759.90816,0
+2012/03/31,2017/03/31,20,29759.90816,0
+2012/06/30,2015/03/31,11,27184.00337,0
+2012/06/30,2015/06/30,12,27184.00337,0
+2012/06/30,2015/09/30,13,27184.00337,0
+2012/06/30,2015/12/31,14,27043.73802,0
+2012/06/30,2016/03/31,15,27043.73802,0
+2012/06/30,2016/06/30,16,27043.73802,0
+2012/06/30,2016/09/30,17,27043.73802,0
+2012/06/30,2016/12/31,18,27043.73802,0
+2012/06/30,2017/03/31,19,27043.73802,0
+2012/06/30,2017/06/30,20,27043.73802,0
+2012/09/30,2015/03/31,10,32479.8032,0
+2012/09/30,2015/06/30,11,32317.23586,0
+2012/09/30,2015/09/30,12,32441.72372,0
+2012/09/30,2015/12/31,13,32413.25309,0
+2012/09/30,2016/03/31,14,32454.13218,0
+2012/09/30,2016/06/30,15,32454.13218,0
+2012/09/30,2016/09/30,16,32560.84962,0
+2012/09/30,2016/12/31,17,32564.50335,0
+2012/09/30,2017/03/31,18,32564.50335,0
+2012/09/30,2017/06/30,19,32560.56492,0
+2012/09/30,2017/09/30,20,32560.56492,0
+2012/12/31,2015/03/31,9,41486.03907,0
+2012/12/31,2015/06/30,10,41475.59983,0
+2012/12/31,2015/09/30,11,41551.30801,0
+2012/12/31,2015/12/31,12,41551.30801,0
+2012/12/31,2016/03/31,13,41551.30801,0
+2012/12/31,2016/06/30,14,41551.30801,0
+2012/12/31,2016/09/30,15,41583.40865,0
+2012/12/31,2016/12/31,16,41583.40865,0
+2012/12/31,2017/03/31,17,41583.40865,0
+2012/12/31,2017/06/30,18,41255.9963,0
+2012/12/31,2017/09/30,19,41214.38172,0
+2012/12/31,2017/12/31,20,41214.38172,0
+2013/03/31,2015/03/31,8,38508.0814,0
+2013/03/31,2015/06/30,9,38516.29044,0
+2013/03/31,2015/09/30,10,38526.65849,0
+2013/03/31,2015/12/31,11,38510.71494,0
+2013/03/31,2016/03/31,12,38510.71494,0
+2013/03/31,2016/06/30,13,38510.71494,0
+2013/03/31,2016/09/30,14,38776.89169,0
+2013/03/31,2016/12/31,15,38729.01356,0
+2013/03/31,2017/03/31,16,38726.64101,0
+2013/03/31,2017/06/30,17,38726.64101,0
+2013/03/31,2017/09/30,18,38726.64101,0
+2013/03/31,2017/12/31,19,38726.64101,0
+2013/03/31,2018/03/31,20,38737.05652,0
+2013/06/30,2015/03/31,7,26322.95634,0
+2013/06/30,2015/06/30,8,26318.30614,0
+2013/06/30,2015/09/30,9,26309.00573,0
+2013/06/30,2015/12/31,10,26621.18629,0
+2013/06/30,2016/03/31,11,26621.18629,0
+2013/06/30,2016/06/30,12,26639.73965,0
+2013/06/30,2016/09/30,13,26639.73965,0
+2013/06/30,2016/12/31,14,26624.34178,0
+2013/06/30,2017/03/31,15,26624.34178,0
+2013/06/30,2017/06/30,16,26623.63002,0
+2013/06/30,2017/09/30,17,26623.63002,0
+2013/06/30,2017/12/31,18,26623.63002,0
+2013/06/30,2018/03/31,19,26623.63002,0
+2013/06/30,2018/06/30,20,26623.63002,0
+2013/09/30,2015/03/31,6,27364.72075,0
+2013/09/30,2015/06/30,7,27262.70096,0
+2013/09/30,2015/09/30,8,27243.91034,0
+2013/09/30,2015/12/31,9,27246.16426,0
+2013/09/30,2016/03/31,10,27256.55605,0
+2013/09/30,2016/06/30,11,27246.14054,0
+2013/09/30,2016/09/30,12,27246.14054,0
+2013/09/30,2016/12/31,13,27258.64389,0
+2013/09/30,2017/03/31,14,27258.64389,0
+2013/09/30,2017/06/30,15,27258.64389,0
+2013/09/30,2017/09/30,16,27258.64389,0
+2013/09/30,2017/12/31,17,27258.64389,0
+2013/09/30,2018/03/31,18,27258.64389,0
+2013/09/30,2018/06/30,19,27258.66762,0
+2013/09/30,2018/09/30,20,27258.64389,0
+2013/12/31,2015/03/31,5,45806.36363,0
+2013/12/31,2015/06/30,6,44432.8451,0
+2013/12/31,2015/09/30,7,44633.70546,0
+2013/12/31,2015/12/31,8,44637.71508,0
+2013/12/31,2016/03/31,9,44694.01577,0
+2013/12/31,2016/06/30,10,44694.01577,0
+2013/12/31,2016/09/30,11,44683.57653,0
+2013/12/31,2016/12/31,12,44481.43499,0
+2013/12/31,2017/03/31,13,44528.71998,0
+2013/12/31,2017/06/30,14,44567.20279,0
+2013/12/31,2017/09/30,15,44675.6522,0
+2013/12/31,2017/12/31,16,44707.04108,0
+2013/12/31,2018/03/31,17,44790.29398,0
+2013/12/31,2018/06/30,18,44837.1519,0
+2013/12/31,2018/09/30,19,44883.06081,0
+2013/12/31,2018/12/31,20,44814.47029,0
+2014/03/31,2015/03/31,4,37946.52177,0
+2014/03/31,2015/06/30,5,37692.44505,0
+2014/03/31,2015/09/30,6,37686.37131,0
+2014/03/31,2015/12/31,7,37629.2165,0
+2014/03/31,2016/03/31,8,37634.19886,0
+2014/03/31,2016/06/30,9,37634.19886,0
+2014/03/31,2016/09/30,10,37612.44255,0
+2014/03/31,2016/12/31,11,37612.44255,0
+2014/03/31,2017/03/31,12,37599.79684,0
+2014/03/31,2017/06/30,13,37599.79684,0
+2014/03/31,2017/09/30,14,37599.79684,0
+2014/03/31,2017/12/31,15,37599.79684,0
+2014/03/31,2018/03/31,16,37599.79684,0
+2014/03/31,2018/06/30,17,37599.82057,0
+2014/03/31,2018/09/30,18,37599.82057,0
+2014/03/31,2018/12/31,19,37599.79684,0
+2014/03/31,2019/03/31,20,37599.82057,0
+2014/06/30,2015/03/31,3,38611.97551,0
+2014/06/30,2015/06/30,4,37948.23001,0
+2014/06/30,2015/09/30,5,38007.56757,0
+2014/06/30,2015/12/31,6,38109.23148,0
+2014/06/30,2016/03/31,7,38098.74479,0
+2014/06/30,2016/06/30,8,38210.08871,0
+2014/06/30,2016/09/30,9,38178.84219,0
+2014/06/30,2016/12/31,10,38178.84219,0
+2014/06/30,2017/03/31,11,38177.65591,0
+2014/06/30,2017/06/30,12,38177.65591,0
+2014/06/30,2017/09/30,13,38177.65591,0
+2014/06/30,2017/12/31,14,38177.65591,0
+2014/06/30,2018/03/31,15,38177.65591,0
+2014/06/30,2018/06/30,16,38177.65591,0
+2014/06/30,2018/09/30,17,38177.65591,0
+2014/06/30,2018/12/31,18,38175.40199,0
+2014/06/30,2019/03/31,19,38175.40199,0
+2014/06/30,2019/06/30,20,38185.72259,0
+2014/09/30,2015/03/31,2,35282.14447,0
+2014/09/30,2015/06/30,3,34872.14355,0
+2014/09/30,2015/09/30,4,35780.52301,0
+2014/09/30,2015/12/31,5,35467.41716,0
+2014/09/30,2016/03/31,6,35473.39599,0
+2014/09/30,2016/06/30,7,35477.31071,0
+2014/09/30,2016/09/30,8,35450.19242,0
+2014/09/30,2016/12/31,9,35662.91555,0
+2014/09/30,2017/03/31,10,35628.34744,0
+2014/09/30,2017/06/30,11,35557.69281,0
+2014/09/30,2017/09/30,12,35557.69281,0
+2014/09/30,2017/12/31,13,35563.69537,0
+2014/09/30,2018/03/31,14,35563.69537,0
+2014/09/30,2018/06/30,15,35576.12755,0
+2014/09/30,2018/09/30,16,35576.12755,0
+2014/09/30,2018/12/31,17,35570.88421,0
+2014/09/30,2019/03/31,18,35570.88421,0
+2014/09/30,2019/06/30,19,35568.91499,0
+2014/09/30,2019/09/30,20,35555.58124,0
+2014/12/31,2015/03/31,1,35454.98498,0
+2014/12/31,2015/06/30,2,36729.97137,0
+2014/12/31,2015/09/30,3,37065.5453,0
+2014/12/31,2015/12/31,4,36676.58892,0
+2014/12/31,2016/03/31,5,36631.46296,0
+2014/12/31,2016/06/30,6,36391.88253,0
+2014/12/31,2016/09/30,7,36360.65973,0
+2014/12/31,2016/12/31,8,36376.36603,0
+2014/12/31,2017/03/31,9,36386.78154,0
+2014/12/31,2017/06/30,10,36420.49552,0
+2014/12/31,2017/09/30,11,36420.49552,0
+2014/12/31,2017/12/31,12,36430.91103,0
+2014/12/31,2018/03/31,13,36445.02772,0
+2014/12/31,2018/06/30,14,36449.70165,0
+2014/12/31,2018/09/30,15,36449.86773,0
+2014/12/31,2018/12/31,16,36436.98477,0
+2014/12/31,2019/03/31,17,36436.98477,0
+2014/12/31,2019/06/30,18,36436.98477,0
+2014/12/31,2019/09/30,19,36436.98477,0
+2014/12/31,2019/12/31,20,36436.98477,0
```

### Comparing `tryangle-0.2.1/src/tryangle/utils/data/swiss_test.csv` & `tryangle-0.2.2.dev0/src/tryangle/utils/data/swiss_test.csv`

 * *Ordering differences only*

 * *Files 24% similar despite different names*

```diff
@@ -1,391 +1,391 @@
-﻿origin,development,lag,claim,premium
-1979,1998,19,8051,0
-1980,1998,18,9749,0
-1980,1999,19,9749,0
-1981,1998,17,12666,0
-1981,1999,18,12711,0
-1981,2000,19,12713,0
-1982,1998,16,14141,0
-1982,1999,17,14145,0
-1982,2000,18,14166,0
-1982,2001,19,14167,0
-1983,1998,15,16619,0
-1983,1999,16,16681,0
-1983,2000,17,16681,0
-1983,2001,18,16687,0
-1983,2002,19,16711,0
-1984,1998,14,17298,0
-1984,1999,15,17307,0
-1984,2000,16,17308,0
-1984,2001,17,17308,0
-1984,2002,18,17309,0
-1984,2003,19,17310,0
-1985,1998,13,16426,0
-1985,1999,14,16480,0
-1985,2000,15,16480,0
-1985,2001,16,16480,0
-1985,2002,17,16480,0
-1985,2003,18,16482,0
-1985,2004,19,16482,0
-1986,1998,12,17706,0
-1986,1999,13,17706,0
-1986,2000,14,17712,0
-1986,2001,15,17713,0
-1986,2002,16,17718,0
-1986,2003,17,17719,0
-1986,2004,18,17719,0
-1986,2005,19,17719,0
-1987,1998,11,18689,0
-1987,1999,12,18746,0
-1987,2000,13,18772,0
-1987,2001,14,18774,0
-1987,2002,15,18804,0
-1987,2003,16,18804,0
-1987,2004,17,18804,0
-1987,2005,18,18806,0
-1987,2006,19,18806,0
-1988,1998,10,20611,0
-1988,1999,11,21250,0
-1988,2000,12,21257,0
-1988,2001,13,22505,0
-1988,2002,14,22509,0
-1988,2003,15,22516,0
-1988,2004,16,22518,0
-1988,2005,17,22522,0
-1988,2006,18,22523,0
-1988,2007,19,22527,0
-1989,1998,9,20415,0
-1989,1999,10,20510,0
-1989,2000,11,20594,0
-1989,2001,12,20657,0
-1989,2002,13,20752,0
-1989,2003,14,20823,0
-1989,2004,15,20899,0
-1989,2005,16,20983,0
-1989,2006,17,21124,0
-1989,2007,18,21622,0
-1989,2008,19,21627,0
-1990,1998,8,23888,0
-1990,1999,9,24061,0
-1990,2000,10,24096,0
-1990,2001,11,24301,0
-1990,2002,12,24356,0
-1990,2003,13,24389,0
-1990,2004,14,24391,0
-1990,2005,15,24784,0
-1990,2006,16,24784,0
-1990,2007,17,24794,0
-1990,2008,18,24894,0
-1990,2009,19,24900,0
-1991,1998,7,24410,0
-1991,1999,8,24884,0
-1991,2000,9,24896,0
-1991,2001,10,24968,0
-1991,2002,11,25031,0
-1991,2003,12,25172,0
-1991,2004,13,25459,0
-1991,2005,14,25460,0
-1991,2006,15,25470,0
-1991,2007,16,25734,0
-1991,2008,17,25774,0
-1991,2009,18,25877,0
-1991,2010,19,25883,0
-1992,1998,6,26129,0
-1992,1999,7,26149,0
-1992,2000,8,26166,0
-1992,2001,9,26231,0
-1992,2002,10,26328,0
-1992,2003,11,26743,0
-1992,2004,12,27023,0
-1992,2005,13,27048,0
-1992,2006,14,27075,0
-1992,2007,15,27168,0
-1992,2008,16,27234,0
-1992,2009,17,27276,0
-1992,2010,18,27386,0
-1992,2011,19,27392,0
-1993,1998,5,27120,0
-1993,1999,6,27164,0
-1993,2000,7,27183,0
-1993,2001,8,27250,0
-1993,2002,9,27490,0
-1993,2003,10,27497,0
-1993,2004,11,27561,0
-1993,2005,12,27565,0
-1993,2006,13,27582,0
-1993,2007,14,27706,0
-1993,2008,15,27787,0
-1993,2009,16,27855,0
-1993,2010,17,27898,0
-1993,2011,18,28010,0
-1993,2012,19,28017,0
-1994,1998,4,27568,0
-1994,1999,5,27637,0
-1994,2000,6,27805,0
-1994,2001,7,28003,0
-1994,2002,8,28223,0
-1994,2003,9,28240,0
-1994,2004,10,28245,0
-1994,2005,11,28250,0
-1994,2006,12,28257,0
-1994,2007,13,28297,0
-1994,2008,14,28347,0
-1994,2009,15,28430,0
-1994,2010,16,28499,0
-1994,2011,17,28543,0
-1994,2012,18,28658,0
-1994,2013,19,28665,0
-1995,1998,3,27043,0
-1995,1999,4,27866,0
-1995,2000,5,27882,0
-1995,2001,6,27903,0
-1995,2002,7,27933,0
-1995,2003,8,28492,0
-1995,2004,9,28545,0
-1995,2005,10,28564,0
-1995,2006,11,28686,0
-1995,2007,12,28695,0
-1995,2008,13,28897,0
-1995,2009,14,28948,0
-1995,2010,15,29033,0
-1995,2011,16,29104,0
-1995,2012,17,29149,0
-1995,2013,18,29266,0
-1995,2014,19,29273,0
-1996,1998,2,23909,0
-1996,1999,3,24690,0
-1996,2000,4,26083,0
-1996,2001,5,26525,0
-1996,2002,6,26567,0
-1996,2003,7,26640,0
-1996,2004,8,26695,0
-1996,2005,9,26801,0
-1996,2006,10,26814,0
-1996,2007,11,27018,0
-1996,2008,12,27078,0
-1996,2009,13,27269,0
-1996,2010,14,27317,0
-1996,2011,15,27397,0
-1996,2012,16,27463,0
-1996,2013,17,27506,0
-1996,2014,18,27616,0
-1996,2015,19,27623,0
-1997,1998,1,26918,0
-1997,1999,2,28256,0
-1997,2000,3,28569,0
-1997,2001,4,28964,0
-1997,2002,5,29268,0
-1997,2003,6,29344,0
-1997,2004,7,29393,0
-1997,2005,8,30159,0
-1997,2006,9,30936,0
-1997,2007,10,30966,0
-1997,2008,11,31122,0
-1997,2009,12,31190,0
-1997,2010,13,31410,0
-1997,2011,14,31466,0
-1997,2012,15,31558,0
-1997,2013,16,31635,0
-1997,2014,17,31684,0
-1997,2015,18,31811,0
-1997,2016,19,31819,0
-1998,1998,0,17655,0
-1998,1999,1,26241,0
-1998,2000,2,27369,0
-1998,2001,3,28063,0
-1998,2002,4,28346,0
-1998,2003,5,28780,0
-1998,2004,6,29024,0
-1998,2005,7,29180,0
-1998,2006,8,29250,0
-1998,2007,9,29575,0
-1998,2008,10,29660,0
-1998,2009,11,29809,0
-1998,2010,12,29875,0
-1998,2011,13,30085,0
-1998,2012,14,30138,0
-1998,2013,15,30227,0
-1998,2014,16,30300,0
-1998,2015,17,30347,0
-1998,2016,18,30469,0
-1998,2017,19,30476,0
-1999,1999,0,16789,0
-1999,2000,1,25547,0
-1999,2001,2,27099,0
-1999,2002,3,27801,0
-1999,2003,4,27919,0
-1999,2004,5,28052,0
-1999,2005,6,30020,0
-1999,2006,7,30035,0
-1999,2007,8,30456,0
-1999,2008,9,30663,0
-1999,2009,10,30750,0
-1999,2010,11,30905,0
-1999,2011,12,30973,0
-1999,2012,13,31192,0
-1999,2013,14,31247,0
-1999,2014,15,31338,0
-1999,2015,16,31415,0
-1999,2016,17,31463,0
-1999,2017,18,31590,0
-1999,2018,19,31597,0
-2000,2000,0,15538,0
-2000,2001,1,23830,0
-2000,2002,2,25202,0
-2000,2003,3,26462,0
-2000,2004,4,27056,0
-2000,2005,5,27480,0
-2000,2006,6,27564,0
-2000,2007,7,27612,0
-2000,2008,8,27873,0
-2000,2009,9,28062,0
-2000,2010,10,28143,0
-2000,2011,11,28284,0
-2000,2012,12,28347,0
-2000,2013,13,28546,0
-2000,2014,14,28597,0
-2000,2015,15,28681,0
-2000,2016,16,28751,0
-2000,2017,17,28795,0
-2000,2018,18,28911,0
-2000,2019,19,28917,0
-2001,2001,0,15113,0
-2001,2002,1,23405,0
-2001,2003,2,26822,0
-2001,2004,3,27711,0
-2001,2005,4,28080,0
-2001,2006,5,29203,0
-2001,2007,6,29647,0
-2001,2008,7,29751,0
-2001,2009,8,30032,0
-2001,2010,9,30236,0
-2001,2011,10,30323,0
-2001,2012,11,30475,0
-2001,2013,12,30542,0
-2001,2014,13,30758,0
-2001,2015,14,30812,0
-2001,2016,15,30903,0
-2001,2017,16,30978,0
-2001,2018,17,31025,0
-2001,2019,18,31150,0
-2001,2020,19,31157,0
-2002,2002,0,14543,0
-2002,2003,1,22674,0
-2002,2004,2,23603,0
-2002,2005,3,24159,0
-2002,2006,4,24242,0
-2002,2007,5,24425,0
-2002,2008,6,24767,0
-2002,2009,7,24854,0
-2002,2010,8,25089,0
-2002,2011,9,25260,0
-2002,2012,10,25332,0
-2002,2013,11,25459,0
-2002,2014,12,25515,0
-2002,2015,13,25695,0
-2002,2016,14,25741,0
-2002,2017,15,25816,0
-2002,2018,16,25879,0
-2002,2019,17,25919,0
-2002,2020,18,26023,0
-2002,2021,19,26029,0
-2003,2003,0,14590,0
-2003,2004,1,22337,0
-2003,2005,2,23442,0
-2003,2006,3,24031,0
-2003,2007,4,24665,0
-2003,2008,5,24942,0
-2003,2009,6,25292,0
-2003,2010,7,25380,0
-2003,2011,8,25621,0
-2003,2012,9,25794,0
-2003,2013,10,25868,0
-2003,2014,11,25998,0
-2003,2015,12,26056,0
-2003,2016,13,26239,0
-2003,2017,14,26286,0
-2003,2018,15,26363,0
-2003,2019,16,26427,0
-2003,2020,17,26468,0
-2003,2021,18,26574,0
-2003,2022,19,26580,0
-2004,2004,0,13976,0
-2004,2005,1,21527,0
-2004,2006,2,22615,0
-2004,2007,3,23242,0
-2004,2008,4,23653,0
-2004,2009,5,23918,0
-2004,2010,6,24254,0
-2004,2011,7,24339,0
-2004,2012,8,24569,0
-2004,2013,9,24736,0
-2004,2014,10,24806,0
-2004,2015,11,24931,0
-2004,2016,12,24986,0
-2004,2017,13,25162,0
-2004,2018,14,25207,0
-2004,2019,15,25281,0
-2004,2020,16,25342,0
-2004,2021,17,25381,0
-2004,2022,18,25483,0
-2004,2023,19,25489,0
-2005,2005,0,12932,0
-2005,2006,1,20118,0
-2005,2007,2,21309,0
-2005,2008,3,21824,0
-2005,2009,4,22209,0
-2005,2010,5,22459,0
-2005,2011,6,22774,0
-2005,2012,7,22853,0
-2005,2013,8,23070,0
-2005,2014,9,23226,0
-2005,2015,10,23293,0
-2005,2016,11,23410,0
-2005,2017,12,23462,0
-2005,2018,13,23627,0
-2005,2019,14,23669,0
-2005,2020,15,23738,0
-2005,2021,16,23796,0
-2005,2022,17,23832,0
-2005,2023,18,23928,0
-2005,2024,19,23934,0
-2006,2006,0,12538,0
-2006,2007,1,20357,0
-2006,2008,2,21435,0
-2006,2009,3,21953,0
-2006,2010,4,22341,0
-2006,2011,5,22592,0
-2006,2012,6,22909,0
-2006,2013,7,22989,0
-2006,2014,8,23206,0
-2006,2015,9,23364,0
-2006,2016,10,23431,0
-2006,2017,11,23548,0
-2006,2018,12,23600,0
-2006,2019,13,23767,0
-2006,2020,14,23809,0
-2006,2021,15,23879,0
-2006,2022,16,23937,0
-2006,2023,17,23974,0
-2006,2024,18,24070,0
-2006,2025,19,24076,0
-2007,2007,0,12888,0
-2007,2008,1,19413,0
-2007,2009,2,20441,0
-2007,2010,3,20935,0
-2007,2011,4,21304,0
-2007,2012,5,21544,0
-2007,2013,6,21846,0
-2007,2014,7,21922,0
-2007,2015,8,22130,0
-2007,2016,9,22280,0
-2007,2017,10,22344,0
-2007,2018,11,22456,0
-2007,2019,12,22506,0
-2007,2020,13,22664,0
-2007,2021,14,22704,0
-2007,2022,15,22771,0
-2007,2023,16,22826,0
-2007,2024,17,22861,0
-2007,2025,18,22953,0
-2007,2026,19,22959,0
+﻿origin,development,lag,claim,premium
+1979,1998,19,8051,0
+1980,1998,18,9749,0
+1980,1999,19,9749,0
+1981,1998,17,12666,0
+1981,1999,18,12711,0
+1981,2000,19,12713,0
+1982,1998,16,14141,0
+1982,1999,17,14145,0
+1982,2000,18,14166,0
+1982,2001,19,14167,0
+1983,1998,15,16619,0
+1983,1999,16,16681,0
+1983,2000,17,16681,0
+1983,2001,18,16687,0
+1983,2002,19,16711,0
+1984,1998,14,17298,0
+1984,1999,15,17307,0
+1984,2000,16,17308,0
+1984,2001,17,17308,0
+1984,2002,18,17309,0
+1984,2003,19,17310,0
+1985,1998,13,16426,0
+1985,1999,14,16480,0
+1985,2000,15,16480,0
+1985,2001,16,16480,0
+1985,2002,17,16480,0
+1985,2003,18,16482,0
+1985,2004,19,16482,0
+1986,1998,12,17706,0
+1986,1999,13,17706,0
+1986,2000,14,17712,0
+1986,2001,15,17713,0
+1986,2002,16,17718,0
+1986,2003,17,17719,0
+1986,2004,18,17719,0
+1986,2005,19,17719,0
+1987,1998,11,18689,0
+1987,1999,12,18746,0
+1987,2000,13,18772,0
+1987,2001,14,18774,0
+1987,2002,15,18804,0
+1987,2003,16,18804,0
+1987,2004,17,18804,0
+1987,2005,18,18806,0
+1987,2006,19,18806,0
+1988,1998,10,20611,0
+1988,1999,11,21250,0
+1988,2000,12,21257,0
+1988,2001,13,22505,0
+1988,2002,14,22509,0
+1988,2003,15,22516,0
+1988,2004,16,22518,0
+1988,2005,17,22522,0
+1988,2006,18,22523,0
+1988,2007,19,22527,0
+1989,1998,9,20415,0
+1989,1999,10,20510,0
+1989,2000,11,20594,0
+1989,2001,12,20657,0
+1989,2002,13,20752,0
+1989,2003,14,20823,0
+1989,2004,15,20899,0
+1989,2005,16,20983,0
+1989,2006,17,21124,0
+1989,2007,18,21622,0
+1989,2008,19,21627,0
+1990,1998,8,23888,0
+1990,1999,9,24061,0
+1990,2000,10,24096,0
+1990,2001,11,24301,0
+1990,2002,12,24356,0
+1990,2003,13,24389,0
+1990,2004,14,24391,0
+1990,2005,15,24784,0
+1990,2006,16,24784,0
+1990,2007,17,24794,0
+1990,2008,18,24894,0
+1990,2009,19,24900,0
+1991,1998,7,24410,0
+1991,1999,8,24884,0
+1991,2000,9,24896,0
+1991,2001,10,24968,0
+1991,2002,11,25031,0
+1991,2003,12,25172,0
+1991,2004,13,25459,0
+1991,2005,14,25460,0
+1991,2006,15,25470,0
+1991,2007,16,25734,0
+1991,2008,17,25774,0
+1991,2009,18,25877,0
+1991,2010,19,25883,0
+1992,1998,6,26129,0
+1992,1999,7,26149,0
+1992,2000,8,26166,0
+1992,2001,9,26231,0
+1992,2002,10,26328,0
+1992,2003,11,26743,0
+1992,2004,12,27023,0
+1992,2005,13,27048,0
+1992,2006,14,27075,0
+1992,2007,15,27168,0
+1992,2008,16,27234,0
+1992,2009,17,27276,0
+1992,2010,18,27386,0
+1992,2011,19,27392,0
+1993,1998,5,27120,0
+1993,1999,6,27164,0
+1993,2000,7,27183,0
+1993,2001,8,27250,0
+1993,2002,9,27490,0
+1993,2003,10,27497,0
+1993,2004,11,27561,0
+1993,2005,12,27565,0
+1993,2006,13,27582,0
+1993,2007,14,27706,0
+1993,2008,15,27787,0
+1993,2009,16,27855,0
+1993,2010,17,27898,0
+1993,2011,18,28010,0
+1993,2012,19,28017,0
+1994,1998,4,27568,0
+1994,1999,5,27637,0
+1994,2000,6,27805,0
+1994,2001,7,28003,0
+1994,2002,8,28223,0
+1994,2003,9,28240,0
+1994,2004,10,28245,0
+1994,2005,11,28250,0
+1994,2006,12,28257,0
+1994,2007,13,28297,0
+1994,2008,14,28347,0
+1994,2009,15,28430,0
+1994,2010,16,28499,0
+1994,2011,17,28543,0
+1994,2012,18,28658,0
+1994,2013,19,28665,0
+1995,1998,3,27043,0
+1995,1999,4,27866,0
+1995,2000,5,27882,0
+1995,2001,6,27903,0
+1995,2002,7,27933,0
+1995,2003,8,28492,0
+1995,2004,9,28545,0
+1995,2005,10,28564,0
+1995,2006,11,28686,0
+1995,2007,12,28695,0
+1995,2008,13,28897,0
+1995,2009,14,28948,0
+1995,2010,15,29033,0
+1995,2011,16,29104,0
+1995,2012,17,29149,0
+1995,2013,18,29266,0
+1995,2014,19,29273,0
+1996,1998,2,23909,0
+1996,1999,3,24690,0
+1996,2000,4,26083,0
+1996,2001,5,26525,0
+1996,2002,6,26567,0
+1996,2003,7,26640,0
+1996,2004,8,26695,0
+1996,2005,9,26801,0
+1996,2006,10,26814,0
+1996,2007,11,27018,0
+1996,2008,12,27078,0
+1996,2009,13,27269,0
+1996,2010,14,27317,0
+1996,2011,15,27397,0
+1996,2012,16,27463,0
+1996,2013,17,27506,0
+1996,2014,18,27616,0
+1996,2015,19,27623,0
+1997,1998,1,26918,0
+1997,1999,2,28256,0
+1997,2000,3,28569,0
+1997,2001,4,28964,0
+1997,2002,5,29268,0
+1997,2003,6,29344,0
+1997,2004,7,29393,0
+1997,2005,8,30159,0
+1997,2006,9,30936,0
+1997,2007,10,30966,0
+1997,2008,11,31122,0
+1997,2009,12,31190,0
+1997,2010,13,31410,0
+1997,2011,14,31466,0
+1997,2012,15,31558,0
+1997,2013,16,31635,0
+1997,2014,17,31684,0
+1997,2015,18,31811,0
+1997,2016,19,31819,0
+1998,1998,0,17655,0
+1998,1999,1,26241,0
+1998,2000,2,27369,0
+1998,2001,3,28063,0
+1998,2002,4,28346,0
+1998,2003,5,28780,0
+1998,2004,6,29024,0
+1998,2005,7,29180,0
+1998,2006,8,29250,0
+1998,2007,9,29575,0
+1998,2008,10,29660,0
+1998,2009,11,29809,0
+1998,2010,12,29875,0
+1998,2011,13,30085,0
+1998,2012,14,30138,0
+1998,2013,15,30227,0
+1998,2014,16,30300,0
+1998,2015,17,30347,0
+1998,2016,18,30469,0
+1998,2017,19,30476,0
+1999,1999,0,16789,0
+1999,2000,1,25547,0
+1999,2001,2,27099,0
+1999,2002,3,27801,0
+1999,2003,4,27919,0
+1999,2004,5,28052,0
+1999,2005,6,30020,0
+1999,2006,7,30035,0
+1999,2007,8,30456,0
+1999,2008,9,30663,0
+1999,2009,10,30750,0
+1999,2010,11,30905,0
+1999,2011,12,30973,0
+1999,2012,13,31192,0
+1999,2013,14,31247,0
+1999,2014,15,31338,0
+1999,2015,16,31415,0
+1999,2016,17,31463,0
+1999,2017,18,31590,0
+1999,2018,19,31597,0
+2000,2000,0,15538,0
+2000,2001,1,23830,0
+2000,2002,2,25202,0
+2000,2003,3,26462,0
+2000,2004,4,27056,0
+2000,2005,5,27480,0
+2000,2006,6,27564,0
+2000,2007,7,27612,0
+2000,2008,8,27873,0
+2000,2009,9,28062,0
+2000,2010,10,28143,0
+2000,2011,11,28284,0
+2000,2012,12,28347,0
+2000,2013,13,28546,0
+2000,2014,14,28597,0
+2000,2015,15,28681,0
+2000,2016,16,28751,0
+2000,2017,17,28795,0
+2000,2018,18,28911,0
+2000,2019,19,28917,0
+2001,2001,0,15113,0
+2001,2002,1,23405,0
+2001,2003,2,26822,0
+2001,2004,3,27711,0
+2001,2005,4,28080,0
+2001,2006,5,29203,0
+2001,2007,6,29647,0
+2001,2008,7,29751,0
+2001,2009,8,30032,0
+2001,2010,9,30236,0
+2001,2011,10,30323,0
+2001,2012,11,30475,0
+2001,2013,12,30542,0
+2001,2014,13,30758,0
+2001,2015,14,30812,0
+2001,2016,15,30903,0
+2001,2017,16,30978,0
+2001,2018,17,31025,0
+2001,2019,18,31150,0
+2001,2020,19,31157,0
+2002,2002,0,14543,0
+2002,2003,1,22674,0
+2002,2004,2,23603,0
+2002,2005,3,24159,0
+2002,2006,4,24242,0
+2002,2007,5,24425,0
+2002,2008,6,24767,0
+2002,2009,7,24854,0
+2002,2010,8,25089,0
+2002,2011,9,25260,0
+2002,2012,10,25332,0
+2002,2013,11,25459,0
+2002,2014,12,25515,0
+2002,2015,13,25695,0
+2002,2016,14,25741,0
+2002,2017,15,25816,0
+2002,2018,16,25879,0
+2002,2019,17,25919,0
+2002,2020,18,26023,0
+2002,2021,19,26029,0
+2003,2003,0,14590,0
+2003,2004,1,22337,0
+2003,2005,2,23442,0
+2003,2006,3,24031,0
+2003,2007,4,24665,0
+2003,2008,5,24942,0
+2003,2009,6,25292,0
+2003,2010,7,25380,0
+2003,2011,8,25621,0
+2003,2012,9,25794,0
+2003,2013,10,25868,0
+2003,2014,11,25998,0
+2003,2015,12,26056,0
+2003,2016,13,26239,0
+2003,2017,14,26286,0
+2003,2018,15,26363,0
+2003,2019,16,26427,0
+2003,2020,17,26468,0
+2003,2021,18,26574,0
+2003,2022,19,26580,0
+2004,2004,0,13976,0
+2004,2005,1,21527,0
+2004,2006,2,22615,0
+2004,2007,3,23242,0
+2004,2008,4,23653,0
+2004,2009,5,23918,0
+2004,2010,6,24254,0
+2004,2011,7,24339,0
+2004,2012,8,24569,0
+2004,2013,9,24736,0
+2004,2014,10,24806,0
+2004,2015,11,24931,0
+2004,2016,12,24986,0
+2004,2017,13,25162,0
+2004,2018,14,25207,0
+2004,2019,15,25281,0
+2004,2020,16,25342,0
+2004,2021,17,25381,0
+2004,2022,18,25483,0
+2004,2023,19,25489,0
+2005,2005,0,12932,0
+2005,2006,1,20118,0
+2005,2007,2,21309,0
+2005,2008,3,21824,0
+2005,2009,4,22209,0
+2005,2010,5,22459,0
+2005,2011,6,22774,0
+2005,2012,7,22853,0
+2005,2013,8,23070,0
+2005,2014,9,23226,0
+2005,2015,10,23293,0
+2005,2016,11,23410,0
+2005,2017,12,23462,0
+2005,2018,13,23627,0
+2005,2019,14,23669,0
+2005,2020,15,23738,0
+2005,2021,16,23796,0
+2005,2022,17,23832,0
+2005,2023,18,23928,0
+2005,2024,19,23934,0
+2006,2006,0,12538,0
+2006,2007,1,20357,0
+2006,2008,2,21435,0
+2006,2009,3,21953,0
+2006,2010,4,22341,0
+2006,2011,5,22592,0
+2006,2012,6,22909,0
+2006,2013,7,22989,0
+2006,2014,8,23206,0
+2006,2015,9,23364,0
+2006,2016,10,23431,0
+2006,2017,11,23548,0
+2006,2018,12,23600,0
+2006,2019,13,23767,0
+2006,2020,14,23809,0
+2006,2021,15,23879,0
+2006,2022,16,23937,0
+2006,2023,17,23974,0
+2006,2024,18,24070,0
+2006,2025,19,24076,0
+2007,2007,0,12888,0
+2007,2008,1,19413,0
+2007,2009,2,20441,0
+2007,2010,3,20935,0
+2007,2011,4,21304,0
+2007,2012,5,21544,0
+2007,2013,6,21846,0
+2007,2014,7,21922,0
+2007,2015,8,22130,0
+2007,2016,9,22280,0
+2007,2017,10,22344,0
+2007,2018,11,22456,0
+2007,2019,12,22506,0
+2007,2020,13,22664,0
+2007,2021,14,22704,0
+2007,2022,15,22771,0
+2007,2023,16,22826,0
+2007,2024,17,22861,0
+2007,2025,18,22953,0
+2007,2026,19,22959,0
```

### Comparing `tryangle-0.2.1/src/tryangle/utils/data/swiss_train.csv` & `tryangle-0.2.2.dev0/src/tryangle/utils/data/swiss_train.csv`

 * *Ordering differences only*

 * *Files 21% similar despite different names*

```diff
@@ -1,191 +1,191 @@
-origin,development,lag,claim,premium
-1979,1979,0,3670,17684
-1979,1980,1,5817,17684
-1979,1981,2,6462,17684
-1979,1982,3,6671,17684
-1979,1983,4,6775,17684
-1979,1984,5,7002,17684
-1979,1985,6,7034,17684
-1979,1986,7,7096,17684
-1979,1987,8,7204,17684
-1979,1988,9,7326,17684
-1979,1989,10,7395,17684
-1979,1990,11,7438,17684
-1979,1991,12,7468,17684
-1979,1992,13,7541,17684
-1979,1993,14,7580,17684
-1979,1994,15,7677,17684
-1979,1995,16,7794,17684
-1979,1996,17,7919,17684
-1979,1997,18,8047,17684
-1980,1980,0,4827,18762
-1980,1981,1,7600,18762
-1980,1982,2,8274,18762
-1980,1983,3,8412,18762
-1980,1984,4,9059,18762
-1980,1985,5,9197,18762
-1980,1986,6,9230,18762
-1980,1987,7,9277,18762
-1980,1988,8,9331,18762
-1980,1989,9,9435,18762
-1980,1990,10,9864,18762
-1980,1991,11,9621,18762
-1980,1992,12,9654,18762
-1980,1993,13,9704,18762
-1980,1994,14,9743,18762
-1980,1995,15,9745,18762
-1980,1996,16,9745,18762
-1980,1997,17,9748,18762
-1981,1981,0,7130,22056
-1981,1982,1,10852,22056
-1981,1983,2,11422,22056
-1981,1984,3,12024,22056
-1981,1985,4,12320,22056
-1981,1986,5,12346,22056
-1981,1987,6,12379,22056
-1981,1988,7,12426,22056
-1981,1989,8,12460,22056
-1981,1990,9,12500,22056
-1981,1991,10,12508,22056
-1981,1992,11,12547,22056
-1981,1993,12,12557,22056
-1981,1994,13,12624,22056
-1981,1995,14,12639,22056
-1981,1996,15,12644,22056
-1981,1997,16,12647,22056
-1982,1982,0,9244,25489
-1982,1983,1,13340,25489
-1982,1984,2,13758,25489
-1982,1985,3,13853,25489
-1982,1986,4,13894,25489
-1982,1987,5,13942,25489
-1982,1988,6,13980,25489
-1982,1989,7,14001,25489
-1982,1990,8,14012,25489
-1982,1991,9,14070,25489
-1982,1992,10,14085,25489
-1982,1993,11,14098,25489
-1982,1994,12,14111,25489
-1982,1995,13,14118,25489
-1982,1996,14,14120,25489
-1982,1997,15,14133,25489
-1983,1983,0,10019,24819
-1983,1984,1,14223,24819
-1983,1985,2,15403,24819
-1983,1986,3,15579,24819
-1983,1987,4,15732,24819
-1983,1988,5,15921,24819
-1983,1989,6,16187,24819
-1983,1990,7,16420,24819
-1983,1991,8,16531,24819
-1983,1992,9,16559,24819
-1983,1993,10,16568,24819
-1983,1994,11,16585,24819
-1983,1995,12,16597,24819
-1983,1996,13,16614,24819
-1983,1997,14,16617,24819
-1984,1984,0,9966,26887
-1984,1985,1,14599,26887
-1984,1986,2,15181,26887
-1984,1987,3,15431,26887
-1984,1988,4,15506,26887
-1984,1989,5,15538,26887
-1984,1990,6,15906,26887
-1984,1991,7,16014,26887
-1984,1992,8,16537,26887
-1984,1993,9,16833,26887
-1984,1994,10,16951,26887
-1984,1995,11,17038,26887
-1984,1996,12,17040,26887
-1984,1997,13,17195,26887
-1985,1985,0,10441,31782
-1985,1986,1,15043,31782
-1985,1987,2,15577,31782
-1985,1988,3,15784,31782
-1985,1989,4,15926,31782
-1985,1990,5,16054,31782
-1985,1991,6,16087,31782
-1985,1992,7,16107,31782
-1985,1993,8,16311,31782
-1985,1994,9,16366,31782
-1985,1995,10,16396,31782
-1985,1996,11,16414,31782
-1985,1997,12,16419,31782
-1986,1986,0,10578,32585
-1986,1987,1,15657,32585
-1986,1988,2,16352,32585
-1986,1989,3,16714,32585
-1986,1990,4,17048,32585
-1986,1991,5,17289,32585
-1986,1992,6,17632,32585
-1986,1993,7,17646,32585
-1986,1994,8,17662,32585
-1986,1995,9,17678,32585
-1986,1996,10,17693,32585
-1986,1997,11,17700,32585
-1987,1987,0,11214,32726
-1987,1988,1,16482,32726
-1987,1989,2,17197,32726
-1987,1990,3,17518,32726
-1987,1991,4,18345,32726
-1987,1992,5,18480,32726
-1987,1993,6,18505,32726
-1987,1994,7,18520,32726
-1987,1995,8,18578,32726
-1987,1996,9,18633,32726
-1987,1997,10,18671,32726
-1988,1988,0,11442,36372
-1988,1989,1,17621,36372
-1988,1990,2,18465,36372
-1988,1991,3,18693,36372
-1988,1992,4,18882,36372
-1988,1993,5,18965,36372
-1988,1994,6,20464,36372
-1988,1995,7,20522,36372
-1988,1996,8,20558,36372
-1988,1997,9,20607,36372
-1989,1989,0,11720,36873
-1989,1990,1,17779,36873
-1989,1991,2,18655,36873
-1989,1992,3,18940,36873
-1989,1993,4,19098,36873
-1989,1994,5,19368,36873
-1989,1995,6,19970,36873
-1989,1996,7,20162,36873
-1989,1997,8,20195,36873
-1990,1990,0,13293,38938
-1990,1991,1,20689,38938
-1990,1992,2,21696,38938
-1990,1993,3,22439,38938
-1990,1994,4,22798,38938
-1990,1995,5,23054,38938
-1990,1996,6,23394,38938
-1990,1997,7,23554,38938
-1991,1991,0,15063,42109
-1991,1992,1,22917,42109
-1991,1993,2,23543,42109
-1991,1994,3,24032,42109
-1991,1995,4,24156,42109
-1991,1996,5,24232,42109
-1991,1997,6,24360,42109
-1992,1992,0,16986,40818
-1992,1993,1,23958,40818
-1992,1994,2,25090,40818
-1992,1995,3,25392,40818
-1992,1996,4,25546,40818
-1992,1997,5,26099,40818
-1993,1993,0,16681,43180
-1993,1994,1,24867,43180
-1993,1995,2,25871,43180
-1993,1996,3,26463,43180
-1993,1997,4,26941,43180
-1994,1994,0,17595,47061
-1994,1995,1,25152,47061
-1994,1996,2,26140,47061
-1994,1997,3,27090,47061
-1995,1995,0,16547,48428
-1995,1996,1,25396,48428
-1995,1997,2,26506,48428
-1996,1996,0,15449,52565
-1996,1997,1,22702,52565
-1997,1997,0,18043,52728
+origin,development,lag,claim,premium
+1979,1979,0,3670,17684
+1979,1980,1,5817,17684
+1979,1981,2,6462,17684
+1979,1982,3,6671,17684
+1979,1983,4,6775,17684
+1979,1984,5,7002,17684
+1979,1985,6,7034,17684
+1979,1986,7,7096,17684
+1979,1987,8,7204,17684
+1979,1988,9,7326,17684
+1979,1989,10,7395,17684
+1979,1990,11,7438,17684
+1979,1991,12,7468,17684
+1979,1992,13,7541,17684
+1979,1993,14,7580,17684
+1979,1994,15,7677,17684
+1979,1995,16,7794,17684
+1979,1996,17,7919,17684
+1979,1997,18,8047,17684
+1980,1980,0,4827,18762
+1980,1981,1,7600,18762
+1980,1982,2,8274,18762
+1980,1983,3,8412,18762
+1980,1984,4,9059,18762
+1980,1985,5,9197,18762
+1980,1986,6,9230,18762
+1980,1987,7,9277,18762
+1980,1988,8,9331,18762
+1980,1989,9,9435,18762
+1980,1990,10,9864,18762
+1980,1991,11,9621,18762
+1980,1992,12,9654,18762
+1980,1993,13,9704,18762
+1980,1994,14,9743,18762
+1980,1995,15,9745,18762
+1980,1996,16,9745,18762
+1980,1997,17,9748,18762
+1981,1981,0,7130,22056
+1981,1982,1,10852,22056
+1981,1983,2,11422,22056
+1981,1984,3,12024,22056
+1981,1985,4,12320,22056
+1981,1986,5,12346,22056
+1981,1987,6,12379,22056
+1981,1988,7,12426,22056
+1981,1989,8,12460,22056
+1981,1990,9,12500,22056
+1981,1991,10,12508,22056
+1981,1992,11,12547,22056
+1981,1993,12,12557,22056
+1981,1994,13,12624,22056
+1981,1995,14,12639,22056
+1981,1996,15,12644,22056
+1981,1997,16,12647,22056
+1982,1982,0,9244,25489
+1982,1983,1,13340,25489
+1982,1984,2,13758,25489
+1982,1985,3,13853,25489
+1982,1986,4,13894,25489
+1982,1987,5,13942,25489
+1982,1988,6,13980,25489
+1982,1989,7,14001,25489
+1982,1990,8,14012,25489
+1982,1991,9,14070,25489
+1982,1992,10,14085,25489
+1982,1993,11,14098,25489
+1982,1994,12,14111,25489
+1982,1995,13,14118,25489
+1982,1996,14,14120,25489
+1982,1997,15,14133,25489
+1983,1983,0,10019,24819
+1983,1984,1,14223,24819
+1983,1985,2,15403,24819
+1983,1986,3,15579,24819
+1983,1987,4,15732,24819
+1983,1988,5,15921,24819
+1983,1989,6,16187,24819
+1983,1990,7,16420,24819
+1983,1991,8,16531,24819
+1983,1992,9,16559,24819
+1983,1993,10,16568,24819
+1983,1994,11,16585,24819
+1983,1995,12,16597,24819
+1983,1996,13,16614,24819
+1983,1997,14,16617,24819
+1984,1984,0,9966,26887
+1984,1985,1,14599,26887
+1984,1986,2,15181,26887
+1984,1987,3,15431,26887
+1984,1988,4,15506,26887
+1984,1989,5,15538,26887
+1984,1990,6,15906,26887
+1984,1991,7,16014,26887
+1984,1992,8,16537,26887
+1984,1993,9,16833,26887
+1984,1994,10,16951,26887
+1984,1995,11,17038,26887
+1984,1996,12,17040,26887
+1984,1997,13,17195,26887
+1985,1985,0,10441,31782
+1985,1986,1,15043,31782
+1985,1987,2,15577,31782
+1985,1988,3,15784,31782
+1985,1989,4,15926,31782
+1985,1990,5,16054,31782
+1985,1991,6,16087,31782
+1985,1992,7,16107,31782
+1985,1993,8,16311,31782
+1985,1994,9,16366,31782
+1985,1995,10,16396,31782
+1985,1996,11,16414,31782
+1985,1997,12,16419,31782
+1986,1986,0,10578,32585
+1986,1987,1,15657,32585
+1986,1988,2,16352,32585
+1986,1989,3,16714,32585
+1986,1990,4,17048,32585
+1986,1991,5,17289,32585
+1986,1992,6,17632,32585
+1986,1993,7,17646,32585
+1986,1994,8,17662,32585
+1986,1995,9,17678,32585
+1986,1996,10,17693,32585
+1986,1997,11,17700,32585
+1987,1987,0,11214,32726
+1987,1988,1,16482,32726
+1987,1989,2,17197,32726
+1987,1990,3,17518,32726
+1987,1991,4,18345,32726
+1987,1992,5,18480,32726
+1987,1993,6,18505,32726
+1987,1994,7,18520,32726
+1987,1995,8,18578,32726
+1987,1996,9,18633,32726
+1987,1997,10,18671,32726
+1988,1988,0,11442,36372
+1988,1989,1,17621,36372
+1988,1990,2,18465,36372
+1988,1991,3,18693,36372
+1988,1992,4,18882,36372
+1988,1993,5,18965,36372
+1988,1994,6,20464,36372
+1988,1995,7,20522,36372
+1988,1996,8,20558,36372
+1988,1997,9,20607,36372
+1989,1989,0,11720,36873
+1989,1990,1,17779,36873
+1989,1991,2,18655,36873
+1989,1992,3,18940,36873
+1989,1993,4,19098,36873
+1989,1994,5,19368,36873
+1989,1995,6,19970,36873
+1989,1996,7,20162,36873
+1989,1997,8,20195,36873
+1990,1990,0,13293,38938
+1990,1991,1,20689,38938
+1990,1992,2,21696,38938
+1990,1993,3,22439,38938
+1990,1994,4,22798,38938
+1990,1995,5,23054,38938
+1990,1996,6,23394,38938
+1990,1997,7,23554,38938
+1991,1991,0,15063,42109
+1991,1992,1,22917,42109
+1991,1993,2,23543,42109
+1991,1994,3,24032,42109
+1991,1995,4,24156,42109
+1991,1996,5,24232,42109
+1991,1997,6,24360,42109
+1992,1992,0,16986,40818
+1992,1993,1,23958,40818
+1992,1994,2,25090,40818
+1992,1995,3,25392,40818
+1992,1996,4,25546,40818
+1992,1997,5,26099,40818
+1993,1993,0,16681,43180
+1993,1994,1,24867,43180
+1993,1995,2,25871,43180
+1993,1996,3,26463,43180
+1993,1997,4,26941,43180
+1994,1994,0,17595,47061
+1994,1995,1,25152,47061
+1994,1996,2,26140,47061
+1994,1997,3,27090,47061
+1995,1995,0,16547,48428
+1995,1996,1,25396,48428
+1995,1997,2,26506,48428
+1996,1996,0,15449,52565
+1996,1997,1,22702,52565
+1997,1997,0,18043,52728
```

### Comparing `tryangle-0.2.1/src/tryangle/utils/datasets.py` & `tryangle-0.2.2.dev0/src/tryangle/utils/datasets.py`

 * *Ordering differences only*

 * *Files 14% similar despite different names*

```diff
@@ -1,92 +1,92 @@
-# This Source Code Form is subject to the terms of the Mozilla Public
-# License, v. 2.0. If a copy of the MPL was not distributed with this
-# file, You can obtain one at https://mozilla.org/MPL/2.0/.
-
-import os
-import pandas as pd
-from chainladder.core.triangle import Triangle
-from tryangle.core import TryangleData
-
-
-def load_sample(key, *args, **kwargs):
-    """Function to load training datasets included in the tryangle package.
-
-    Args:
-        key (str): Key to identify dataset
-
-    Returns:
-        [TryangleData]: TryangleData object of the loaded dataset.
-    """
-    path = os.path.dirname(os.path.abspath(__file__))
-
-    if key in ["swiss", "cas", "sme"]:
-        df = pd.read_csv(os.path.join(path, "data", key.lower() + "_train.csv"))
-        sample_weight = df[["origin", "premium", "development"]].drop_duplicates()
-        columns = ["claim"]
-    else:
-        raise KeyError(
-            "No such dataset exists. Available datasets are 'swiss', 'cas' and 'sme'."
-        )
-
-    claim = Triangle(
-        df,
-        origin="origin",
-        development="development",
-        index=None,
-        columns=columns,
-        cumulative=True,
-        *args,
-        **kwargs
-    )
-    sample_weight = Triangle(
-        sample_weight,
-        origin="origin",
-        index=None,
-        development="development",
-        columns=["premium"],
-        cumulative=True,
-        *args,
-        **kwargs
-    ).latest_diagonal
-
-    return TryangleData(claim, sample_weight)
-
-
-def load_test_sample(key, *args, **kwargs):
-    """Function to load test datasets included in the tryangle package.
-
-    Args:
-        key (str): Key to identify dataset
-
-    Returns:
-        [TryangleData]: TryangleData object of the loaded dataset.
-    """
-    path = os.path.dirname(os.path.abspath(__file__))
-
-    df = pd.read_csv(os.path.join(path, "data", key.lower() + "_test.csv"))
-
-    claim = Triangle(
-        df,
-        origin="origin",
-        development="development",
-        index=None,
-        columns=["claim"],
-        cumulative=True,
-        *args,
-        **kwargs
-    )
-
-    if key.lower() in ["swiss"]:
-        claim = claim[claim.development <= 240]
-        claim = claim[claim.origin.year <= 1997]
-        claim = claim[claim.valuation.year > 1997]
-    elif key.lower() in ["cas", "sme"]:
-        claim = claim[claim.development <= 63]
-        claim = claim[claim.origin.year <= 2014]
-        claim = claim[claim.valuation.year > 2014]
-
-    return TryangleData(claim)
-
-
-if __name__ == "__main__":
-    pass
+# This Source Code Form is subject to the terms of the Mozilla Public
+# License, v. 2.0. If a copy of the MPL was not distributed with this
+# file, You can obtain one at https://mozilla.org/MPL/2.0/.
+
+import os
+import pandas as pd
+from chainladder.core.triangle import Triangle
+from tryangle.core import TryangleData
+
+
+def load_sample(key, *args, **kwargs):
+    """Function to load training datasets included in the tryangle package.
+
+    Args:
+        key (str): Key to identify dataset
+
+    Returns:
+        [TryangleData]: TryangleData object of the loaded dataset.
+    """
+    path = os.path.dirname(os.path.abspath(__file__))
+
+    if key in ["swiss", "cas", "sme"]:
+        df = pd.read_csv(os.path.join(path, "data", key.lower() + "_train.csv"))
+        sample_weight = df[["origin", "premium", "development"]].drop_duplicates()
+        columns = ["claim"]
+    else:
+        raise KeyError(
+            "No such dataset exists. Available datasets are 'swiss', 'cas' and 'sme'."
+        )
+
+    claim = Triangle(
+        df,
+        origin="origin",
+        development="development",
+        index=None,
+        columns=columns,
+        cumulative=True,
+        *args,
+        **kwargs
+    )
+    sample_weight = Triangle(
+        sample_weight,
+        origin="origin",
+        index=None,
+        development="development",
+        columns=["premium"],
+        cumulative=True,
+        *args,
+        **kwargs
+    ).latest_diagonal
+
+    return TryangleData(claim, sample_weight)
+
+
+def load_test_sample(key, *args, **kwargs):
+    """Function to load test datasets included in the tryangle package.
+
+    Args:
+        key (str): Key to identify dataset
+
+    Returns:
+        [TryangleData]: TryangleData object of the loaded dataset.
+    """
+    path = os.path.dirname(os.path.abspath(__file__))
+
+    df = pd.read_csv(os.path.join(path, "data", key.lower() + "_test.csv"))
+
+    claim = Triangle(
+        df,
+        origin="origin",
+        development="development",
+        index=None,
+        columns=["claim"],
+        cumulative=True,
+        *args,
+        **kwargs
+    )
+
+    if key.lower() in ["swiss"]:
+        claim = claim[claim.development <= 240]
+        claim = claim[claim.origin.year <= 1997]
+        claim = claim[claim.valuation.year > 1997]
+    elif key.lower() in ["cas", "sme"]:
+        claim = claim[claim.development <= 63]
+        claim = claim[claim.origin.year <= 2014]
+        claim = claim[claim.valuation.year > 2014]
+
+    return TryangleData(claim)
+
+
+if __name__ == "__main__":
+    pass
```

### Comparing `tryangle-0.2.1/src/tryangle.egg-info/SOURCES.txt` & `tryangle-0.2.2.dev0/src/tryangle.egg-info/SOURCES.txt`

 * *Files 18% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 LICENSE
 MANIFEST.in
-README.rst
+README.md
+pyproject.toml
 requirements.txt
-setup.py
 src/tryangle/__init__.py
 src/tryangle.egg-info/PKG-INFO
 src/tryangle.egg-info/SOURCES.txt
 src/tryangle.egg-info/dependency_links.txt
 src/tryangle.egg-info/requires.txt
 src/tryangle.egg-info/top_level.txt
 src/tryangle/core/__init__.py
@@ -24,8 +24,13 @@
 src/tryangle/utils/__init__.py
 src/tryangle/utils/datasets.py
 src/tryangle/utils/data/cas_test.csv
 src/tryangle/utils/data/cas_train.csv
 src/tryangle/utils/data/sme_test.csv
 src/tryangle/utils/data/sme_train.csv
 src/tryangle/utils/data/swiss_test.csv
-src/tryangle/utils/data/swiss_train.csv
+src/tryangle/utils/data/swiss_train.csv
+tests/test_datasets.py
+tests/test_ensemble.py
+tests/test_methods.py
+tests/test_score.py
+tests/test_split.py
```

