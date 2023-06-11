# Comparing `tmp/django_esteid-3.4b1.tar.gz` & `tmp/django_esteid-4.0b1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_esteid-3.4b1.tar", max compression
+gzip compressed data, was "django_esteid-4.0b1.tar", max compression
```

## Comparing `django_esteid-3.4b1.tar` & `django_esteid-4.0b1.tar`

### file list

```diff
@@ -1,82 +1,80 @@
--rw-r--r--   0        0        0      354 2021-11-09 11:26:25.693390 django_esteid-3.4b1/AUTHORS.md
--rw-r--r--   0        0        0     1477 2021-11-09 11:26:25.693390 django_esteid-3.4b1/LICENSE
--rw-r--r--   0        0        0     4901 2021-11-15 15:18:14.832376 django_esteid-3.4b1/README.md
--rw-r--r--   0        0        0       23 2023-06-02 10:09:24.263424 django_esteid-3.4b1/esteid/__init__.py
--rw-r--r--   0        0        0    16980 2023-06-02 09:57:48.736038 django_esteid-3.4b1/esteid/actions.py
--rw-r--r--   0        0        0     2685 2021-11-09 11:26:25.696724 django_esteid-3.4b1/esteid/authentication/README.md
--rw-r--r--   0        0        0      283 2021-11-09 11:26:25.696724 django_esteid-3.4b1/esteid/authentication/__init__.py
--rw-r--r--   0        0        0     6569 2021-11-09 11:26:25.696724 django_esteid-3.4b1/esteid/authentication/authenticator.py
--rw-r--r--   0        0        0      576 2021-11-09 11:26:25.696724 django_esteid-3.4b1/esteid/authentication/types.py
--rw-r--r--   0        0        0     3854 2021-11-09 11:26:25.696724 django_esteid-3.4b1/esteid/authentication/views.py
--rw-r--r--   0        0        0     6250 2021-11-15 12:09:45.735139 django_esteid-3.4b1/esteid/base_service.py
--rw-r--r--   0        0        0     1960 2021-11-09 11:26:25.696724 django_esteid-3.4b1/esteid/compat.py
--rw-r--r--   0        0        0     1912 2021-11-09 11:26:25.696724 django_esteid-3.4b1/esteid/constants.py
--rw-r--r--   0        0        0      410 2021-11-09 11:26:25.696724 django_esteid-3.4b1/esteid/context_processors.py
--rw-r--r--   0        0        0     5842 2021-11-09 11:26:25.696724 django_esteid-3.4b1/esteid/exceptions.py
--rw-r--r--   0        0        0       52 2021-11-09 11:26:25.696724 django_esteid-3.4b1/esteid/flowtest/README.md
--rw-r--r--   0        0        0        0 2021-11-09 11:26:25.696724 django_esteid-3.4b1/esteid/flowtest/__init__.py
--rw-r--r--   0        0        0     1155 2023-06-01 12:41:12.526823 django_esteid-3.4b1/esteid/flowtest/signer.py
--rw-r--r--   0        0        0     1475 2023-06-02 10:16:36.944478 django_esteid-3.4b1/esteid/flowtest/urls.py
--rw-r--r--   0        0        0     1938 2021-11-09 11:26:25.696724 django_esteid-3.4b1/esteid/flowtest/views.py
--rw-r--r--   0        0        0     1621 2021-11-09 11:26:25.696724 django_esteid-3.4b1/esteid/generic.py
--rw-r--r--   0        0        0     5336 2023-06-01 12:45:10.777134 django_esteid-3.4b1/esteid/idcard/README.md
--rw-r--r--   0        0        0      141 2021-11-09 11:26:25.696724 django_esteid-3.4b1/esteid/idcard/__init__.py
--rw-r--r--   0        0        0     3712 2023-06-01 13:16:41.695317 django_esteid-3.4b1/esteid/idcard/signer.py
--rw-r--r--   0        0        0      288 2021-11-09 11:26:25.696724 django_esteid-3.4b1/esteid/idcard/templates/iframe-error.html
--rw-r--r--   0        0        0      245 2021-11-09 11:26:25.696724 django_esteid-3.4b1/esteid/idcard/templates/iframe.html
--rw-r--r--   0        0        0     6413 2023-06-01 12:41:27.213305 django_esteid-3.4b1/esteid/idcard/views.py
--rw-r--r--   0        0        0      380 2021-11-09 11:26:25.696724 django_esteid-3.4b1/esteid/locale/en/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0     2049 2021-11-09 11:26:25.696724 django_esteid-3.4b1/esteid/locale/en/LC_MESSAGES/django.po
--rw-r--r--   0        0        0     1927 2021-11-09 11:26:25.696724 django_esteid-3.4b1/esteid/locale/et/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0     2743 2021-11-09 11:26:25.696724 django_esteid-3.4b1/esteid/locale/et/LC_MESSAGES/django.po
--rw-r--r--   0        0        0      511 2021-11-09 11:26:25.696724 django_esteid-3.4b1/esteid/locale/lt/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0     2186 2021-11-09 11:26:25.696724 django_esteid-3.4b1/esteid/locale/lt/LC_MESSAGES/django.po
--rw-r--r--   0        0        0     2688 2021-11-09 11:26:25.696724 django_esteid-3.4b1/esteid/locale/ru/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0     3363 2021-11-09 11:26:25.696724 django_esteid-3.4b1/esteid/locale/ru/LC_MESSAGES/django.po
--rw-r--r--   0        0        0     6627 2021-11-15 14:09:18.303071 django_esteid-3.4b1/esteid/middleware.py
--rw-r--r--   0        0        0     4682 2023-06-01 12:41:35.186538 django_esteid-3.4b1/esteid/mixins.py
--rw-r--r--   0        0        0     1329 2021-11-09 11:26:25.696724 django_esteid-3.4b1/esteid/mobileid/README.md
--rw-r--r--   0        0        0      210 2021-11-09 11:26:25.696724 django_esteid-3.4b1/esteid/mobileid/__init__.py
--rw-r--r--   0        0        0     2440 2021-11-09 11:26:25.696724 django_esteid-3.4b1/esteid/mobileid/authenticator.py
--rw-r--r--   0        0        0    11547 2021-11-15 12:09:45.738473 django_esteid-3.4b1/esteid/mobileid/base.py
--rw-r--r--   0        0        0      518 2021-11-09 11:26:25.696724 django_esteid-3.4b1/esteid/mobileid/constants.py
--rw-r--r--   0        0        0      960 2023-03-07 10:56:00.181576 django_esteid-3.4b1/esteid/mobileid/i18n.py
--rw-r--r--   0        0        0     3133 2021-11-09 11:26:25.696724 django_esteid-3.4b1/esteid/mobileid/signer.py
--rw-r--r--   0        0        0     2083 2021-11-09 11:26:25.696724 django_esteid-3.4b1/esteid/mobileid/types.py
--rw-r--r--   0        0        0      960 2021-11-15 12:09:45.738473 django_esteid-3.4b1/esteid/mobileid/utils.py
--rw-r--r--   0        0        0     2568 2023-03-07 11:40:15.776172 django_esteid-3.4b1/esteid/ocsp.py
--rw-r--r--   0        0        0     1981 2021-11-15 12:09:45.738473 django_esteid-3.4b1/esteid/session.py
--rw-r--r--   0        0        0     4932 2021-11-09 11:26:25.696724 django_esteid-3.4b1/esteid/settings.py
--rw-r--r--   0        0        0    13575 2021-11-09 11:26:25.696724 django_esteid-3.4b1/esteid/signing/README.md
--rw-r--r--   0        0        0      294 2021-11-09 11:26:25.696724 django_esteid-3.4b1/esteid/signing/__init__.py
--rw-r--r--   0        0        0     9874 2021-11-09 11:26:25.696724 django_esteid-3.4b1/esteid/signing/signer.py
--rw-r--r--   0        0        0     2579 2021-11-09 11:26:25.696724 django_esteid-3.4b1/esteid/signing/types.py
--rw-r--r--   0        0        0     5865 2021-11-09 11:26:25.696724 django_esteid-3.4b1/esteid/signing/views.py
--rw-r--r--   0        0        0     3498 2021-11-09 11:26:25.696724 django_esteid-3.4b1/esteid/smartid/README.md
--rw-r--r--   0        0        0      204 2021-11-09 11:26:25.696724 django_esteid-3.4b1/esteid/smartid/__init__.py
--rw-r--r--   0        0        0      183 2023-03-07 10:56:00.188243 django_esteid-3.4b1/esteid/smartid/apps.py
--rw-r--r--   0        0        0     2253 2021-11-09 11:26:25.696724 django_esteid-3.4b1/esteid/smartid/authenticator.py
--rw-r--r--   0        0        0    14593 2021-11-09 11:26:25.696724 django_esteid-3.4b1/esteid/smartid/base.py
--rw-r--r--   0        0        0      729 2021-11-09 11:26:25.696724 django_esteid-3.4b1/esteid/smartid/constants.py
--rw-r--r--   0        0        0      882 2023-03-07 10:56:00.191576 django_esteid-3.4b1/esteid/smartid/i18n.py
--rw-r--r--   0        0        0     2986 2021-11-09 11:26:25.696724 django_esteid-3.4b1/esteid/smartid/signer.py
--rw-r--r--   0        0        0     1612 2021-11-09 11:26:25.700057 django_esteid-3.4b1/esteid/smartid/types.py
--rw-r--r--   0        0        0      727 2021-11-15 12:09:45.738473 django_esteid-3.4b1/esteid/smartid/utils.py
--rw-r--r--   0        0        0    18710 2023-06-01 15:12:04.915485 django_esteid-3.4b1/esteid/static/esteid-helper/Esteid.main.web.js
--rw-r--r--   0        0        0     9450 2023-06-01 14:18:55.478528 django_esteid-3.4b1/esteid/static/esteid-helper/Esteid.main.web.min.js
--rw-r--r--   0        0        0    18301 2023-06-01 11:37:15.406641 django_esteid-3.4b1/esteid/static/esteid-helper/web-eid.js
--rw-r--r--   0        0        0     1449 2021-11-09 11:26:25.700057 django_esteid-3.4b1/esteid/static/images/esteid/id-kaart-logo.gif
--rw-r--r--   0        0        0     1472 2021-11-09 11:26:25.700057 django_esteid-3.4b1/esteid/static/images/esteid/mid-logo.gif
--rw-r--r--   0        0        0     2458 2021-11-09 11:26:25.700057 django_esteid-3.4b1/esteid/static/images/esteid/smartID-logo-btn.png
--rw-r--r--   0        0        0     6894 2021-11-09 11:26:25.700057 django_esteid-3.4b1/esteid/static/images/esteid/smartID-logo.png
--rw-r--r--   0        0        0    17701 2023-06-01 13:22:35.750760 django_esteid-3.4b1/esteid/templates/esteid/auth-new.html
--rw-r--r--   0        0        0      320 2021-11-09 11:26:25.700057 django_esteid-3.4b1/esteid/templates/esteid/authenticate.html
--rw-r--r--   0        0        0    19018 2023-06-01 12:12:54.665282 django_esteid-3.4b1/esteid/templates/esteid/test-new.html
--rw-r--r--   0        0        0    15435 2023-06-01 13:16:01.879157 django_esteid-3.4b1/esteid/templates/esteid/test.html
--rw-r--r--   0        0        0    10255 2023-03-07 12:58:53.501536 django_esteid-3.4b1/esteid/types.py
--rw-r--r--   0        0        0     1995 2023-06-02 10:16:24.981279 django_esteid-3.4b1/esteid/urls.py
--rw-r--r--   0        0        0     3477 2023-03-07 11:38:29.734360 django_esteid-3.4b1/esteid/util.py
--rw-r--r--   0        0        0     2305 2023-03-07 12:11:59.783677 django_esteid-3.4b1/esteid/validators.py
--rw-r--r--   0        0        0     6326 2023-06-01 12:48:23.157992 django_esteid-3.4b1/esteid/views.py
--rw-r--r--   0        0        0     2632 2023-06-02 10:09:33.583298 django_esteid-3.4b1/pyproject.toml
--rw-r--r--   0        0        0     6326 1970-01-01 00:00:00.000000 django_esteid-3.4b1/PKG-INFO
+-rw-r--r--   0        0        0      354 2021-11-09 11:26:25.693390 django_esteid-4.0b1/AUTHORS.md
+-rw-r--r--   0        0        0     1477 2021-11-09 11:26:25.693390 django_esteid-4.0b1/LICENSE
+-rw-r--r--   0        0        0     4901 2021-11-15 15:18:14.832376 django_esteid-4.0b1/README.md
+-rw-r--r--   0        0        0       23 2023-06-11 09:39:31.897250 django_esteid-4.0b1/esteid/__init__.py
+-rw-r--r--   0        0        0    16980 2023-06-02 09:57:48.736038 django_esteid-4.0b1/esteid/actions.py
+-rw-r--r--   0        0        0     2420 2023-06-11 09:36:46.476132 django_esteid-4.0b1/esteid/authentication/README.md
+-rw-r--r--   0        0        0      283 2021-11-09 11:26:25.696724 django_esteid-4.0b1/esteid/authentication/__init__.py
+-rw-r--r--   0        0        0     6684 2023-06-11 09:11:00.032889 django_esteid-4.0b1/esteid/authentication/authenticator.py
+-rw-r--r--   0        0        0      576 2021-11-09 11:26:25.696724 django_esteid-4.0b1/esteid/authentication/types.py
+-rw-r--r--   0        0        0     4024 2023-06-11 09:20:36.868440 django_esteid-4.0b1/esteid/authentication/views.py
+-rw-r--r--   0        0        0     6250 2021-11-15 12:09:45.735139 django_esteid-4.0b1/esteid/base_service.py
+-rw-r--r--   0        0        0     1960 2021-11-09 11:26:25.696724 django_esteid-4.0b1/esteid/compat.py
+-rw-r--r--   0        0        0     1912 2021-11-09 11:26:25.696724 django_esteid-4.0b1/esteid/constants.py
+-rw-r--r--   0        0        0      410 2021-11-09 11:26:25.696724 django_esteid-4.0b1/esteid/context_processors.py
+-rw-r--r--   0        0        0     5842 2021-11-09 11:26:25.696724 django_esteid-4.0b1/esteid/exceptions.py
+-rw-r--r--   0        0        0       52 2021-11-09 11:26:25.696724 django_esteid-4.0b1/esteid/flowtest/README.md
+-rw-r--r--   0        0        0        0 2021-11-09 11:26:25.696724 django_esteid-4.0b1/esteid/flowtest/__init__.py
+-rw-r--r--   0        0        0     1155 2023-06-01 12:41:12.526823 django_esteid-4.0b1/esteid/flowtest/signer.py
+-rw-r--r--   0        0        0     1387 2023-06-11 09:37:23.192308 django_esteid-4.0b1/esteid/flowtest/urls.py
+-rw-r--r--   0        0        0     1742 2023-06-11 09:37:22.982311 django_esteid-4.0b1/esteid/flowtest/views.py
+-rw-r--r--   0        0        0     1621 2021-11-09 11:26:25.696724 django_esteid-4.0b1/esteid/generic.py
+-rw-r--r--   0        0        0     3295 2023-06-11 09:31:54.576660 django_esteid-4.0b1/esteid/idcard/README.md
+-rw-r--r--   0        0        0      209 2023-06-11 09:33:43.105233 django_esteid-4.0b1/esteid/idcard/__init__.py
+-rw-r--r--   0        0        0     4397 2023-06-11 09:37:23.375639 django_esteid-4.0b1/esteid/idcard/authenticator.py
+-rw-r--r--   0        0        0     3712 2023-06-01 13:16:41.695317 django_esteid-4.0b1/esteid/idcard/signer.py
+-rw-r--r--   0        0        0     2891 2023-06-11 09:37:23.368973 django_esteid-4.0b1/esteid/idcard/types.py
+-rw-r--r--   0        0        0      380 2021-11-09 11:26:25.696724 django_esteid-4.0b1/esteid/locale/en/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0     2049 2021-11-09 11:26:25.696724 django_esteid-4.0b1/esteid/locale/en/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     1927 2021-11-09 11:26:25.696724 django_esteid-4.0b1/esteid/locale/et/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0     2743 2021-11-09 11:26:25.696724 django_esteid-4.0b1/esteid/locale/et/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0      511 2021-11-09 11:26:25.696724 django_esteid-4.0b1/esteid/locale/lt/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0     2186 2021-11-09 11:26:25.696724 django_esteid-4.0b1/esteid/locale/lt/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     2688 2021-11-09 11:26:25.696724 django_esteid-4.0b1/esteid/locale/ru/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0     3363 2021-11-09 11:26:25.696724 django_esteid-4.0b1/esteid/locale/ru/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     4682 2023-06-01 12:41:35.186538 django_esteid-4.0b1/esteid/mixins.py
+-rw-r--r--   0        0        0     1329 2021-11-09 11:26:25.696724 django_esteid-4.0b1/esteid/mobileid/README.md
+-rw-r--r--   0        0        0      210 2021-11-09 11:26:25.696724 django_esteid-4.0b1/esteid/mobileid/__init__.py
+-rw-r--r--   0        0        0     2440 2021-11-09 11:26:25.696724 django_esteid-4.0b1/esteid/mobileid/authenticator.py
+-rw-r--r--   0        0        0    11547 2021-11-15 12:09:45.738473 django_esteid-4.0b1/esteid/mobileid/base.py
+-rw-r--r--   0        0        0      518 2021-11-09 11:26:25.696724 django_esteid-4.0b1/esteid/mobileid/constants.py
+-rw-r--r--   0        0        0      960 2023-03-07 10:56:00.181576 django_esteid-4.0b1/esteid/mobileid/i18n.py
+-rw-r--r--   0        0        0     3133 2021-11-09 11:26:25.696724 django_esteid-4.0b1/esteid/mobileid/signer.py
+-rw-r--r--   0        0        0     2083 2021-11-09 11:26:25.696724 django_esteid-4.0b1/esteid/mobileid/types.py
+-rw-r--r--   0        0        0      960 2021-11-15 12:09:45.738473 django_esteid-4.0b1/esteid/mobileid/utils.py
+-rw-r--r--   0        0        0     2568 2023-03-07 11:40:15.776172 django_esteid-4.0b1/esteid/ocsp.py
+-rw-r--r--   0        0        0     1981 2021-11-15 12:09:45.738473 django_esteid-4.0b1/esteid/session.py
+-rw-r--r--   0        0        0     4735 2023-06-11 09:32:18.669678 django_esteid-4.0b1/esteid/settings.py
+-rw-r--r--   0        0        0    13575 2021-11-09 11:26:25.696724 django_esteid-4.0b1/esteid/signing/README.md
+-rw-r--r--   0        0        0      294 2021-11-09 11:26:25.696724 django_esteid-4.0b1/esteid/signing/__init__.py
+-rw-r--r--   0        0        0     9874 2021-11-09 11:26:25.696724 django_esteid-4.0b1/esteid/signing/signer.py
+-rw-r--r--   0        0        0     2579 2021-11-09 11:26:25.696724 django_esteid-4.0b1/esteid/signing/types.py
+-rw-r--r--   0        0        0     5865 2021-11-09 11:26:25.696724 django_esteid-4.0b1/esteid/signing/views.py
+-rw-r--r--   0        0        0     3498 2021-11-09 11:26:25.696724 django_esteid-4.0b1/esteid/smartid/README.md
+-rw-r--r--   0        0        0      204 2021-11-09 11:26:25.696724 django_esteid-4.0b1/esteid/smartid/__init__.py
+-rw-r--r--   0        0        0      183 2023-03-07 10:56:00.188243 django_esteid-4.0b1/esteid/smartid/apps.py
+-rw-r--r--   0        0        0     2253 2021-11-09 11:26:25.696724 django_esteid-4.0b1/esteid/smartid/authenticator.py
+-rw-r--r--   0        0        0    14593 2021-11-09 11:26:25.696724 django_esteid-4.0b1/esteid/smartid/base.py
+-rw-r--r--   0        0        0      729 2021-11-09 11:26:25.696724 django_esteid-4.0b1/esteid/smartid/constants.py
+-rw-r--r--   0        0        0      882 2023-03-07 10:56:00.191576 django_esteid-4.0b1/esteid/smartid/i18n.py
+-rw-r--r--   0        0        0     2986 2021-11-09 11:26:25.696724 django_esteid-4.0b1/esteid/smartid/signer.py
+-rw-r--r--   0        0        0     1612 2021-11-09 11:26:25.700057 django_esteid-4.0b1/esteid/smartid/types.py
+-rw-r--r--   0        0        0      727 2021-11-15 12:09:45.738473 django_esteid-4.0b1/esteid/smartid/utils.py
+-rw-r--r--   0        0        0    21878 2023-06-10 11:18:47.152496 django_esteid-4.0b1/esteid/static/esteid-helper/Esteid.main.web.js
+-rw-r--r--   0        0        0    10037 2023-06-10 11:18:47.449159 django_esteid-4.0b1/esteid/static/esteid-helper/Esteid.main.web.min.js
+-rw-r--r--   0        0        0    18301 2023-06-01 11:37:15.406641 django_esteid-4.0b1/esteid/static/esteid-helper/web-eid.js
+-rw-r--r--   0        0        0     1449 2021-11-09 11:26:25.700057 django_esteid-4.0b1/esteid/static/images/esteid/id-kaart-logo.gif
+-rw-r--r--   0        0        0     1472 2021-11-09 11:26:25.700057 django_esteid-4.0b1/esteid/static/images/esteid/mid-logo.gif
+-rw-r--r--   0        0        0     2458 2021-11-09 11:26:25.700057 django_esteid-4.0b1/esteid/static/images/esteid/smartID-logo-btn.png
+-rw-r--r--   0        0        0     6894 2021-11-09 11:26:25.700057 django_esteid-4.0b1/esteid/static/images/esteid/smartID-logo.png
+-rw-r--r--   0        0        0    15811 2023-06-10 11:21:23.187035 django_esteid-4.0b1/esteid/templates/esteid/auth-new.html
+-rw-r--r--   0        0        0      320 2021-11-09 11:26:25.700057 django_esteid-4.0b1/esteid/templates/esteid/authenticate.html
+-rw-r--r--   0        0        0    19018 2023-06-01 12:12:54.665282 django_esteid-4.0b1/esteid/templates/esteid/test-new.html
+-rw-r--r--   0        0        0    15435 2023-06-01 13:16:01.879157 django_esteid-4.0b1/esteid/templates/esteid/test.html
+-rw-r--r--   0        0        0    10342 2023-06-11 09:37:23.142309 django_esteid-4.0b1/esteid/types.py
+-rw-r--r--   0        0        0     1995 2023-06-02 10:16:24.981279 django_esteid-4.0b1/esteid/urls.py
+-rw-r--r--   0        0        0     3477 2023-03-07 11:38:29.734360 django_esteid-4.0b1/esteid/util.py
+-rw-r--r--   0        0        0     2305 2023-03-07 12:11:59.783677 django_esteid-4.0b1/esteid/validators.py
+-rw-r--r--   0        0        0     6326 2023-06-01 12:48:23.157992 django_esteid-4.0b1/esteid/views.py
+-rw-r--r--   0        0        0     2632 2023-06-11 09:39:20.670734 django_esteid-4.0b1/pyproject.toml
+-rw-r--r--   0        0        0     6326 1970-01-01 00:00:00.000000 django_esteid-4.0b1/PKG-INFO
```

### Comparing `django_esteid-3.4b1/LICENSE` & `django_esteid-4.0b1/LICENSE`

 * *Files identical despite different names*

### Comparing `django_esteid-3.4b1/README.md` & `django_esteid-4.0b1/README.md`

 * *Files identical despite different names*

### Comparing `django_esteid-3.4b1/esteid/actions.py` & `django_esteid-4.0b1/esteid/actions.py`

 * *Files identical despite different names*

### Comparing `django_esteid-3.4b1/esteid/authentication/README.md` & `django_esteid-4.0b1/esteid/authentication/README.md`

 * *Files 15% similar despite different names*

```diff
@@ -30,53 +30,41 @@
 from rest_framework.views import APIView
 from esteid.authentication import AuthenticationViewRestMixin
 
 class MyRestAuthView(MyAuthMixin, AuthenticationViewRestMixin, APIView):
     pass
 
 # urls.py
-from django.urls.conf import path, re_path
+from django.urls.conf import re_path
 
-from esteid.idcard import BaseIdCardAuthenticationView
+from esteid.idcard import IdCardAuthenticator
 from esteid.mobileid import MobileIdAuthenticator
 from esteid.smartid import SmartIdAuthenticator
 from .views import MyAuthView
-
-
-class MyIdCardAuthenticationView(MyAuthMixin, BaseIdCardAuthenticationView):
-    """A special view that handles ID Card authentication"""
     
 urlpatterns = [
     re_path(rf"^/authenticate/{auth_class.get_method_name()}/", 
             MyAuthView.as_view(authenticator=auth_class), 
             name=f"auth-{auth_class.get_method_name()}")
-    for auth_class in [MobileIdAuthenticator, SmartIdAuthenticator]
-]
-urlpatterns += [
-    path(rf"^/authenticate/id-card/", MyAuthView.as_view(), name=f"auth-idcard")
+    for auth_class in [IdCardAuthenticator, MobileIdAuthenticator, SmartIdAuthenticator]
 ]
 ```
 
 ## Testing Authentication with the Library
 
-To test SmartID and MobileID:
+To test IDCard, SmartID and MobileID:
 
 * Install, if necessary, and activate the library's virtualenv
 * Start the server locally: `./manage.py runserver 8765`
 * Open the [auth testing page](http://127.0.0.1:8765/new-auth/)
 
-To test ID card authentication, please refer to the [ID Card test app](../../idcard_auth_test). 
-
-## Implementation details
+To test ID card authentication you must use HTTPS as the browser extension
+refuses to work without HTTPS. Simple way to get https to work locally is to use
+ngrok. For example: `ngrok http 8000` will create an https proxy to the dev server
+running on your local machine. See [here](../../README.md#ngrok) for more info.
 
 ### Pluggable Authenticator
 
 The outline of the flow implementation is the Dependency Inversion pattern: 
 instead of the view explicitly calling an implementation, 
 the view interacts with an Authenticator class, which loads a pluggable implementation
 based on the method selected by user.
-
-### ID Card Authentication specific notes
-
-For ID Card, the authentication process is quite different from the SmartID/MobileID process.
-REST API can not be used. 
-See the corresponding [README](../idcard/README.md) for the details.
```

### Comparing `django_esteid-3.4b1/esteid/authentication/authenticator.py` & `django_esteid-4.0b1/esteid/authentication/authenticator.py`

 * *Files 6% similar despite different names*

```diff
@@ -48,15 +48,15 @@
         with the corresponding data such as verification code.
 
         Note: For a theoretical case when authentication happens immediately, we leave an opportunity
         that this method returns AuthenticationResult.
         """
         raise NotImplementedError
 
-    def poll(self) -> AuthenticationResult:
+    def poll(self, initial_data: dict = None) -> AuthenticationResult:
         """
         Polls status of the authentication process.
 
         If authentication succeeded, returns an AuthenticationResult.
         Otherwise, raises an ActionInProgress error with the corresponding data such as verification code.
         """
         raise NotImplementedError
@@ -94,15 +94,15 @@
             session_data = SessionData()
             self._cleanup_session(session)
 
         # Not doing session data validation here, because
         # an instance of another type may need different data
         return session_data
 
-    def __init__(self, session, initial=False):
+    def __init__(self, session, initial=False, origin=None):
         """
         Initializes the necessary session data.
 
         Takes a session object, e.g. django request.session,
         and a flag that tells whether to start new session or attempt to load an existing one
         """
         session_data = self.load_session_data(session)
@@ -131,36 +131,37 @@
                 raise SigningSessionDoesNotExist("Invalid authentication session") from e
 
             if time() > session_data.timestamp + self.SESSION_VALIDITY_TIMEOUT:
                 raise SigningSessionDoesNotExist("This authentication session has expired")
 
         self.session = session
         self.session_data = session_data
+        self.origin = origin
 
     def cleanup(self):
         """
         Cleans temporary authentication session data and files.
         """
         return self._cleanup_session(self.session)
 
     @classmethod
-    def start_session(cls, session, initial_data) -> "Authenticator":
+    def start_session(cls, session, initial_data, origin) -> "Authenticator":
         """
         Initializes a fresh authentication session.
         """
-        signer = cls(session, initial=True)
+        signer = cls(session, initial=True, origin=origin)
         signer.setup(initial_data)
         return signer
 
     @classmethod
-    def load_session(cls, session) -> "Authenticator":
+    def load_session(cls, session, origin) -> "Authenticator":
         """
         Continues (loads) an existing authentication session from the `session` object
         """
-        return cls(session, initial=False)
+        return cls(session, initial=False, origin=origin)
 
     @classmethod
     def _cleanup_session(cls, session):
         session.pop(cls._SESSION_KEY, None)
 
     # "Magic" registration of subclasses
```

### Comparing `django_esteid-3.4b1/esteid/authentication/types.py` & `django_esteid-4.0b1/esteid/authentication/types.py`

 * *Files identical despite different names*

### Comparing `django_esteid-3.4b1/esteid/authentication/views.py` & `django_esteid-4.0b1/esteid/authentication/views.py`

 * *Files 5% similar despite different names*

```diff
@@ -26,14 +26,20 @@
         session: base_session.AbstractBaseSession
         data: dict
 
 
 logger = logging.getLogger(__name__)
 
 
+def get_origin(request):
+    origin = f"{request.scheme}://{request.get_host()}"
+
+    return origin
+
+
 class AuthenticationViewMixin(SessionViewMixin):
     # these come from the `url()` definition as in `View.as_view(authentication_method='...')`, either one is enough
     authentication_method: str = None
     authenticator: Type[Authenticator] = None
 
     def on_auth_success(self, request, data: AuthenticationResult):
         """
@@ -54,15 +60,15 @@
 
     def start_session(self, request: "RequestType", *args, **kwargs):
         """
         Initiates an authentication session.
         """
 
         auth_class = self.select_authenticator_class()
-        authenticator = auth_class.start_session(request.session, request.data)
+        authenticator = auth_class.start_session(request.session, request.data, origin=get_origin(request))
 
         do_cleanup = True
 
         try:
             result = authenticator.authenticate()
 
         except ActionInProgress as e:
@@ -80,20 +86,20 @@
                 authenticator.cleanup()
 
     def finish_session(self, request: "RequestType", *args, **kwargs):
         """
         Checks the status of an authentication session
         """
         authenticator_class = self.select_authenticator_class()
-        authenticator = authenticator_class.load_session(request.session)
+        authenticator = authenticator_class.load_session(request.session, origin=get_origin(request))
 
         do_cleanup = True
 
         try:
-            result = authenticator.poll()
+            result = authenticator.poll(request.data)
 
         except ActionInProgress as e:
             do_cleanup = False
             return JsonResponse({"status": self.Status.PENDING, **e.data}, status=e.status)
 
         else:
             self.on_auth_success(request, result)
```

### Comparing `django_esteid-3.4b1/esteid/base_service.py` & `django_esteid-4.0b1/esteid/base_service.py`

 * *Files identical despite different names*

### Comparing `django_esteid-3.4b1/esteid/compat.py` & `django_esteid-4.0b1/esteid/compat.py`

 * *Files identical despite different names*

### Comparing `django_esteid-3.4b1/esteid/constants.py` & `django_esteid-4.0b1/esteid/constants.py`

 * *Files identical despite different names*

### Comparing `django_esteid-3.4b1/esteid/exceptions.py` & `django_esteid-4.0b1/esteid/exceptions.py`

 * *Files identical despite different names*

### Comparing `django_esteid-3.4b1/esteid/flowtest/signer.py` & `django_esteid-4.0b1/esteid/flowtest/signer.py`

 * *Files identical despite different names*

### Comparing `django_esteid-3.4b1/esteid/flowtest/urls.py` & `django_esteid-4.0b1/esteid/flowtest/urls.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,17 +1,20 @@
+from ..idcard.authenticator import IdCardAuthenticator
+
+
 try:
     from django.urls import re_path
 except ImportError:  # noqa
     from django.conf.urls import url as re_path
 
 from esteid.mobileid import MobileIdAuthenticator  # noqa
 from esteid.signing import Signer
 from esteid.smartid import SmartIdAuthenticator  # noqa
 
-from .views import AuthTestRestView, AuthTestView, IDCardAuthTestView, SigningTestRestView, SigningTestView
+from .views import AuthTestRestView, AuthTestView, SigningTestRestView, SigningTestView
 
 
 # Signing
 
 urlpatterns = [
     re_path(f"^sign/{method}/", SigningTestView.as_view(signing_method=method), name=f"sign-{method}")
     for method in Signer.SIGNING_METHODS
@@ -26,23 +29,18 @@
 
 urlpatterns += [
     re_path(
         f"^authenticate/{auth_class.get_method_name()}/",
         AuthTestView.as_view(authenticator=auth_class),
         name=f"auth-{auth_class.get_method_name()}",
     )
-    for auth_class in [MobileIdAuthenticator, SmartIdAuthenticator]
+    for auth_class in [IdCardAuthenticator, MobileIdAuthenticator, SmartIdAuthenticator]
 ]
 
 urlpatterns += [
     re_path(
         f"^authenticate-rest/{auth_class.get_method_name()}/",
         AuthTestRestView.as_view(authenticator=auth_class),
         name=f"auth-rest-{auth_class.get_method_name()}",
     )
-    for auth_class in [MobileIdAuthenticator, SmartIdAuthenticator]
-]
-
-urlpatterns += [
-    # See idcard/README.md as to why this view is special.
-    re_path("^authenticate-id-card/", IDCardAuthTestView.as_view(), name="auth-idcard")
+    for auth_class in [IdCardAuthenticator, MobileIdAuthenticator, SmartIdAuthenticator]
 ]
```

### Comparing `django_esteid-3.4b1/esteid/flowtest/views.py` & `django_esteid-4.0b1/esteid/flowtest/views.py`

 * *Files 15% similar despite different names*

```diff
@@ -8,15 +8,14 @@
 
 from esteid.authentication import AuthenticationViewDjangoMixin, AuthenticationViewRestMixin
 from esteid.signing import DataFile, SignViewDjangoMixin, SignViewRestMixin
 
 # Register our signers
 from ..authentication.types import AuthenticationResult
 from ..idcard import IdCardSigner  # noqa
-from ..idcard import BaseIdCardAuthenticationView
 from ..mobileid import MobileIdSigner  # noqa
 from ..smartid import SmartIdSigner  # noqa
 from .signer import MyPostSigner, MySigner  # noqa
 
 
 class BaseMethods:
     def get_files_to_sign(self, *args, **kwargs):
@@ -43,19 +42,14 @@
     pass
 
 
 class SigningTestRestView(BaseMethods, SignViewRestMixin, APIView):
     pass
 
 
-class IDCardAuthTestView(BaseIdCardAuthenticationView):
-    def on_auth_success(self, request, auth_result: AuthenticationResult):
-        pass
-
-
 class AuthTestView(AuthenticationViewDjangoMixin, View):
     def on_auth_success(self, request, data: AuthenticationResult):
         pass
 
 
 class AuthTestRestView(AuthenticationViewRestMixin, APIView):
     def on_auth_success(self, request, data: AuthenticationResult):
```

### Comparing `django_esteid-3.4b1/esteid/generic.py` & `django_esteid-4.0b1/esteid/generic.py`

 * *Files identical despite different names*

### Comparing `django_esteid-3.4b1/esteid/idcard/signer.py` & `django_esteid-4.0b1/esteid/idcard/signer.py`

 * *Files identical despite different names*

### Comparing `django_esteid-3.4b1/esteid/locale/en/LC_MESSAGES/django.po` & `django_esteid-4.0b1/esteid/locale/en/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django_esteid-3.4b1/esteid/locale/et/LC_MESSAGES/django.mo` & `django_esteid-4.0b1/esteid/locale/et/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django_esteid-3.4b1/esteid/locale/et/LC_MESSAGES/django.po` & `django_esteid-4.0b1/esteid/locale/et/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django_esteid-3.4b1/esteid/locale/lt/LC_MESSAGES/django.po` & `django_esteid-4.0b1/esteid/locale/lt/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django_esteid-3.4b1/esteid/locale/ru/LC_MESSAGES/django.mo` & `django_esteid-4.0b1/esteid/locale/ru/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django_esteid-3.4b1/esteid/locale/ru/LC_MESSAGES/django.po` & `django_esteid-4.0b1/esteid/locale/ru/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django_esteid-3.4b1/esteid/mixins.py` & `django_esteid-4.0b1/esteid/mixins.py`

 * *Files identical despite different names*

### Comparing `django_esteid-3.4b1/esteid/mobileid/README.md` & `django_esteid-4.0b1/esteid/mobileid/README.md`

 * *Files identical despite different names*

### Comparing `django_esteid-3.4b1/esteid/mobileid/authenticator.py` & `django_esteid-4.0b1/esteid/mobileid/authenticator.py`

 * *Files identical despite different names*

### Comparing `django_esteid-3.4b1/esteid/mobileid/base.py` & `django_esteid-4.0b1/esteid/mobileid/base.py`

 * *Files identical despite different names*

### Comparing `django_esteid-3.4b1/esteid/mobileid/constants.py` & `django_esteid-4.0b1/esteid/mobileid/constants.py`

 * *Files identical despite different names*

### Comparing `django_esteid-3.4b1/esteid/mobileid/i18n.py` & `django_esteid-4.0b1/esteid/mobileid/i18n.py`

 * *Files identical despite different names*

### Comparing `django_esteid-3.4b1/esteid/mobileid/signer.py` & `django_esteid-4.0b1/esteid/mobileid/signer.py`

 * *Files identical despite different names*

### Comparing `django_esteid-3.4b1/esteid/mobileid/types.py` & `django_esteid-4.0b1/esteid/mobileid/types.py`

 * *Files identical despite different names*

### Comparing `django_esteid-3.4b1/esteid/mobileid/utils.py` & `django_esteid-4.0b1/esteid/mobileid/utils.py`

 * *Files identical despite different names*

### Comparing `django_esteid-3.4b1/esteid/ocsp.py` & `django_esteid-4.0b1/esteid/ocsp.py`

 * *Files identical despite different names*

### Comparing `django_esteid-3.4b1/esteid/session.py` & `django_esteid-4.0b1/esteid/session.py`

 * *Files identical despite different names*

### Comparing `django_esteid-3.4b1/esteid/settings.py` & `django_esteid-4.0b1/esteid/settings.py`

 * *Files 4% similar despite different names*

```diff
@@ -14,17 +14,14 @@
 ESTEID_DEMO = getattr(settings, "ESTEID_DEMO", True)
 
 # *** ID Card ***
 
 # Whether to use the ID card signing method
 ID_CARD_ENABLED = getattr(settings, "ID_CARD_ENABLED", False)
 
-# For ID card authentication, this refers to the URLs which are allowed to open the auth iframe. '*' means any.
-ID_CARD_FRAME_TARGET_ORIGIN = getattr(settings, "ID_CARD_FRAME_TARGET_ORIGIN", "*")
-
 # *** Mobile ID ***
 
 MOBILE_ID_ENABLED = getattr(settings, "MOBILE_ID_ENABLED", False)
 # Whether to use demo services and credentials for Mobile ID. Default to global demo mode
 MOBILE_ID_TEST_MODE = getattr(settings, "MOBILE_ID_TEST_MODE", ESTEID_DEMO)
 # MobileID Relying party name and UUID, for DEMO they are always the same so no need to explicitly set them
 MOBILE_ID_SERVICE_NAME = getattr(settings, "MOBILE_ID_SERVICE_NAME", None)
```

### Comparing `django_esteid-3.4b1/esteid/signing/README.md` & `django_esteid-4.0b1/esteid/signing/README.md`

 * *Files identical despite different names*

### Comparing `django_esteid-3.4b1/esteid/signing/signer.py` & `django_esteid-4.0b1/esteid/signing/signer.py`

 * *Files identical despite different names*

### Comparing `django_esteid-3.4b1/esteid/signing/types.py` & `django_esteid-4.0b1/esteid/signing/types.py`

 * *Files identical despite different names*

### Comparing `django_esteid-3.4b1/esteid/signing/views.py` & `django_esteid-4.0b1/esteid/signing/views.py`

 * *Files identical despite different names*

### Comparing `django_esteid-3.4b1/esteid/smartid/README.md` & `django_esteid-4.0b1/esteid/smartid/README.md`

 * *Files identical despite different names*

### Comparing `django_esteid-3.4b1/esteid/smartid/authenticator.py` & `django_esteid-4.0b1/esteid/smartid/authenticator.py`

 * *Files identical despite different names*

### Comparing `django_esteid-3.4b1/esteid/smartid/base.py` & `django_esteid-4.0b1/esteid/smartid/base.py`

 * *Files identical despite different names*

### Comparing `django_esteid-3.4b1/esteid/smartid/constants.py` & `django_esteid-4.0b1/esteid/smartid/constants.py`

 * *Files identical despite different names*

### Comparing `django_esteid-3.4b1/esteid/smartid/i18n.py` & `django_esteid-4.0b1/esteid/smartid/i18n.py`

 * *Files identical despite different names*

### Comparing `django_esteid-3.4b1/esteid/smartid/signer.py` & `django_esteid-4.0b1/esteid/smartid/signer.py`

 * *Files identical despite different names*

### Comparing `django_esteid-3.4b1/esteid/smartid/types.py` & `django_esteid-4.0b1/esteid/smartid/types.py`

 * *Files identical despite different names*

### Comparing `django_esteid-3.4b1/esteid/smartid/utils.py` & `django_esteid-4.0b1/esteid/smartid/utils.py`

 * *Files identical despite different names*

### Comparing `django_esteid-3.4b1/esteid/static/esteid-helper/Esteid.main.web.js` & `django_esteid-4.0b1/esteid/static/esteid-helper/Esteid.main.web.js`

 * *Files 13% similar despite different names*

#### js-beautify {}

```diff
@@ -135,14 +135,64 @@
                     },
                     (err) => {
                         reject(err);
                     }
                 );
             });
         }
+        /**
+         * Requests the Web-eID browser extension to authenticate the user. The nonce must be recently retrieved
+         *  from the back end. The result contains the Web eID authentication token that must be sent to the
+         *  back end for validation.
+         *
+         * @param {string} nonce - base64 encoded nonce, generated by the back end, at least 256 bits of entropy
+         * @param {object} options
+         * @param {string} options.lang - ISO 639-1 two-letter language code to specify the Web-eID native application's user interface language
+         * @param {number} options.timeout - user interaction timeout in milliseconds. Default: 120000 (2 minutes)
+         * @returns {Promise<LibraryAuthenticateResponse>}
+         *
+         * Ref: https://github.com/web-eid/web-eid.js#authenticate-result
+         *
+         * interface LibraryAuthenticateResponse {
+         *     // base64-encoded DER encoded authentication certificate of the user
+         *     unverifiedCertificate: string;
+         *
+         *     // algorithm used to produce the authentication signature
+         *     algorithm:
+         *         | "ES256" | "ES384" | "ES512"  // ECDSA
+         *         | "PS256" | "PS384" | "PS512"  // RSASSA-PSS
+         *         | "RS256" | "RS384" | "RS512"; // RSASSA-PKCS1-v1_5
+         *
+         *     // base64-encoded signature of the token
+         *     signature: string;
+         *
+         *     // type identifier and version of the token format separated by a colon character.
+         *     //  example "web-eid:1.0"
+         *     format: string
+         *
+         *     // URL identifying the name and version of the application that issued the token
+         *     //  example "https://web-eid.eu/web-eid-app/releases/2.0.0+0"
+         *     appVersion: string;
+         */
+        authenticate(nonce, options) {
+            const authOptions = {
+                lang: this.language,
+                ...options
+            };
+            return new Promise((resolve, reject) => {
+                return window.webeid.authenticate(nonce, authOptions).then(
+                    (authResponse) => {
+                        resolve(authResponse);
+                    },
+                    (err) => {
+                        reject(err);
+                    }
+                );
+            });
+        }
         /* Language */
         get language() {
             return this._language;
         }
         set language(l) {
             if (LANGUAGES.indexOf(l) !== -1) {
                 this._language = l;
@@ -368,14 +418,53 @@
             });
         }
         smartidStatus() {
             return new Promise((resolve, reject) => {
                 this.checkStatus(this.smartIdUrl, resolve, reject);
             });
         }
+        authenticateWithIdCard(options) {
+            return new Promise((yay, nay) => {
+                request(
+                    this.idUrl, {
+                        csrfmiddlewaretoken: this.csrfToken
+                    },
+                    "POST"
+                ).then(({
+                    ok,
+                    data
+                }) => {
+                    if (ok && data.pending) {
+                        return this.idCardManager.initializeIdCard().then(() => {
+                            return this.idCardManager.authenticate(data.nonce, options || {}).then((result) => {
+                                return request(
+                                    this.idUrl, {
+                                        csrfmiddlewaretoken: this.csrfToken,
+                                        ...result
+                                    },
+                                    "PATCH"
+                                ).then(({
+                                    ok: ok2,
+                                    data: data2
+                                }) => {
+                                    if (ok2 && data2.success) {
+                                        yay(data2);
+                                    } else {
+                                        nay(data2);
+                                    }
+                                }, nay);
+                            }, nay);
+                        }, nay);
+                    } else {
+                        nay(data);
+                    }
+                });
+            });
+        }
+        LOLauthenticateIdCard(nonce, options) {}
         getError(err) {
             return this.idCardManager.getError(err);
         }
     };
     var IdentificationManager_default = IdentificationManager;
 
     // LegacyIdentificationManager.js
@@ -549,23 +638,24 @@
     };
     LegacyIdentificationManager.SIGN_ID = "id";
     LegacyIdentificationManager.SIGN_MOBILE = "mid";
     LegacyIdentificationManager.SIGN_SMARTID = "smartid";
     var LegacyIdentificationManager_default = LegacyIdentificationManager;
 
     // lib.js
+    var Languages = {
+        ET: LANGUAGE_ET,
+        EN: LANGUAGE_EN,
+        RU: LANGUAGE_RU,
+        LT: LANGUAGE_LT
+    };
     var lib_default = {
         IdentificationManager: IdentificationManager_default,
         LegacyIdentificationManager: LegacyIdentificationManager_default,
-        Languages: {
-            ET: LANGUAGE_ET,
-            EN: LANGUAGE_EN,
-            RU: LANGUAGE_RU,
-            LT: LANGUAGE_LT
-        }
+        Languages
     };
 
     // global.js
     var globalObject = typeof globalThis !== "undefined" ? globalThis : typeof self !== "undefined" ? self : typeof window !== "undefined" ? window : typeof global !== "undefined" ? global : {};
     globalObject.Esteid = lib_default;
     var global_default = lib_default;
 })();
```

### Comparing `django_esteid-3.4b1/esteid/static/esteid-helper/Esteid.main.web.min.js` & `django_esteid-4.0b1/esteid/static/esteid-helper/Esteid.main.web.min.js`

 * *Files 4% similar despite different names*

#### js-beautify {}

```diff
@@ -1,14 +1,14 @@
 (() => {
     var o = "EST",
         d = "ENG",
         l = "RUS",
         c = "LIT",
-        R = [o, d, l, c],
-        w = {
+        A = [o, d, l, c],
+        k = {
             user_cancel: {
                 [o]: "Allkirjastamine katkestati",
                 [d]: "Signing was cancelled",
                 [c]: "Pasira\u0161ymas nutrauktas",
                 [l]: "\u041F\u043E\u0434\u043F\u0438\u0441\u044C \u0431\u044B\u043B\u0430 \u043E\u0442\u043C\u0435\u043D\u0435\u043D\u0430"
             },
             no_certificates: {
@@ -59,40 +59,51 @@
             }
             getCertificate() {
                 return new Promise((e, t) => {
                     let i = {
                         lang: this.language
                     };
                     window.webeid.getSigningCertificate(i).then(({
-                        certificate: s,
-                        supportedSignatureAlgorithms: n
+                        certificate: n,
+                        supportedSignatureAlgorithms: s
                     }) => {
-                        this.certificate = s, this.supportedSignatureAlgorithms = n, e(s)
-                    }, s => {
-                        t(s)
+                        this.certificate = n, this.supportedSignatureAlgorithms = s, e(n)
+                    }, n => {
+                        t(n)
                     })
                 })
             }
             signHexData(e, t = "SHA-256") {
-                return new Promise((i, s) => {
-                    let n = {
+                return new Promise((i, n) => {
+                    let s = {
                         lang: this.language
                     };
-                    window.webeid.sign(this.certificate, e, t, n).then(r => {
+                    window.webeid.sign(this.certificate, e, t, s).then(r => {
                         this.signatureAlgorithm = r.signatureAlgorithm, i(r.signature)
                     }, r => {
-                        s(r)
+                        n(r)
                     })
                 })
             }
+            authenticate(e, t) {
+                let i = {
+                    lang: this.language,
+                    ...t
+                };
+                return new Promise((n, s) => window.webeid.authenticate(e, i).then(r => {
+                    n(r)
+                }, r => {
+                    s(r)
+                }))
+            }
             get language() {
                 return this._language
             }
             set language(e) {
-                R.indexOf(e) !== -1 && (this._language = e)
+                A.indexOf(e) !== -1 && (this._language = e)
             }
             getWebeidErrorMapping(e) {
                 switch ((e ? e.code : null) || null) {
                     case "ERR_WEBEID_CONTEXT_INSECURE":
                         return "not_allowed";
                     case "ERR_WEBEID_ACTION_TIMEOUT":
                         return "technical_error";
@@ -113,69 +124,69 @@
                     case "ERR_WEBEID_ACTION_PENDING":
                     case "ERR_WEBEID_MISSING_PARAMETER":
                         return "technical_error"
                 }
             }
             getError(e) {
                 let t;
-                return typeof w[e] > "u" ? t = this.getWebeidErrorMapping(e) || "technical_error" : t = e, {
+                return typeof k[e] > "u" ? t = this.getWebeidErrorMapping(e) || "technical_error" : t = e, {
                     error_code: t,
-                    message: w[t][this.language],
+                    message: k[t][this.language],
                     raw: e
                 }
             }
         },
-        f = m;
-    var g = async (h, e, t = "POST") => {
+        E = m;
+    var g = async (f, e, t = "POST") => {
         let i = {
                 "Content-Type": "application/json"
             },
-            s = null;
-        t !== "GET" && (i["X-CSRFToken"] = e.csrfmiddlewaretoken, s = JSON.stringify(e || {}));
+            n = null;
+        t !== "GET" && (i["X-CSRFToken"] = e.csrfmiddlewaretoken, n = JSON.stringify(e || {}));
         try {
-            let n = await fetch(h, {
+            let s = await fetch(f, {
                     method: t,
                     headers: i,
-                    body: s
+                    body: n
                 }),
-                r = await n.text();
+                r = await s.text();
             try {
                 let a = JSON.parse(r);
-                return a.success = a.status === "success", a.pending = `${n.status}` == "202", {
+                return a.success = a.status === "success", a.pending = `${s.status}` == "202", {
                     data: a,
-                    ok: n.ok
+                    ok: s.ok
                 }
             } catch {
                 return console.log("Failed to parse response as JSON", r), {}
             }
-        } catch (n) {
-            return console.log(n), {}
+        } catch (s) {
+            return console.log(s), {}
         }
     }, p = class {
         constructor({
             language: e,
             idUrl: t,
             mobileIdUrl: i,
-            smartIdUrl: s,
-            csrfToken: n,
+            smartIdUrl: n,
+            csrfToken: s,
             pollInterval: r
         }) {
-            this.idCardManager = new f(e), this.idUrl = t, this.mobileIdUrl = i, this.smartIdUrl = s, this.csrfToken = n, this.language = e, this.pollInterval = r || 3e3
+            this.idCardManager = new E(e), this.idUrl = t, this.mobileIdUrl = i, this.smartIdUrl = n, this.csrfToken = s, this.language = e, this.pollInterval = r || 3e3
         }
         checkStatus(e, t, i) {
-            let s = this.pollInterval,
-                n = this.csrfToken,
+            let n = this.pollInterval,
+                s = this.csrfToken,
                 r = () => {
                     g(e, {
-                        csrfmiddlewaretoken: n
+                        csrfmiddlewaretoken: s
                     }, "PATCH").then(({
                         ok: a,
-                        data: E
+                        data: h
                     }) => {
-                        a && E.pending ? setTimeout(() => r(), s) : a && E.success ? t(E) : i(E)
+                        a && h.pending ? setTimeout(() => r(), n) : a && h.success ? t(h) : i(h)
                     }).catch(a => {
                         console.log("Status error", a)
                     })
                 };
             return r()
         }
         signWithIdCard() {
@@ -183,103 +194,128 @@
                 this.__signHandleIdCard(e, t)
             })
         }
         signWithMobileId({
             idCode: e,
             phoneNumber: t
         }) {
-            return new Promise((i, s) => {
-                this.__signHandleMid(e, t, i, s)
+            return new Promise((i, n) => {
+                this.__signHandleMid(e, t, i, n)
             })
         }
         signWithSmartId({
             idCode: e,
             country: t
         }) {
-            return new Promise((i, s) => {
-                this.__signHandleSmartid(e, t, i, s)
+            return new Promise((i, n) => {
+                this.__signHandleSmartid(e, t, i, n)
             })
         }
         __signHandleIdCard(e, t) {
             this.idCardManager.initializeIdCard().then(() => {
                 this.idCardManager.getCertificate().then(i => {
                     g(this.idUrl, {
                         csrfmiddlewaretoken: this.csrfToken,
                         certificate: i
                     }).then(({
-                        ok: s,
-                        data: n
+                        ok: n,
+                        data: s
                     }) => {
-                        s && n.success ? this.__doSign(n.digest, e, t) : t(n)
+                        n && s.success ? this.__doSign(s.digest, e, t) : t(s)
                     })
                 }, t)
             }, t)
         }
         __doSign(e, t, i) {
-            this.idCardManager.signHexData(e).then(s => {
+            this.idCardManager.signHexData(e).then(n => {
                 g(this.idUrl, {
                     csrfmiddlewaretoken: this.csrfToken,
-                    signature_value: s
+                    signature_value: n
                 }, "PATCH").then(({
-                    ok: n,
+                    ok: s,
                     data: r
                 }) => {
-                    n && r.success ? t(r) : i(r)
+                    s && r.success ? t(r) : i(r)
                 })
             }, i)
         }
-        __signHandleMid(e, t, i, s) {
+        __signHandleMid(e, t, i, n) {
             g(this.mobileIdUrl, {
                 id_code: e,
                 phone_number: t,
                 language: this.language,
                 csrfmiddlewaretoken: this.csrfToken
             }).then(({
-                ok: n,
+                ok: s,
                 data: r
             }) => {
-                n && r.success ? i(r) : s(r)
+                s && r.success ? i(r) : n(r)
             })
         }
         midStatus() {
             return new Promise((e, t) => {
                 this.checkStatus(this.mobileIdUrl, e, t)
             })
         }
-        __signHandleSmartid(e, t, i, s) {
+        __signHandleSmartid(e, t, i, n) {
             g(this.smartIdUrl, {
                 id_code: e,
                 country: t,
                 csrfmiddlewaretoken: this.csrfToken
             }).then(({
-                ok: n,
+                ok: s,
                 data: r
             }) => {
-                n && r.success ? i(r) : s(r)
+                s && r.success ? i(r) : n(r)
             })
         }
         smartidStatus() {
             return new Promise((e, t) => {
                 this.checkStatus(this.smartIdUrl, e, t)
             })
         }
+        authenticateWithIdCard(e) {
+            return new Promise((t, i) => {
+                g(this.idUrl, {
+                    csrfmiddlewaretoken: this.csrfToken
+                }, "POST").then(({
+                    ok: n,
+                    data: s
+                }) => {
+                    if (n && s.pending) return this.idCardManager.initializeIdCard().then(() => this.idCardManager.authenticate(s.nonce, e || {}).then(r => g(this.idUrl, {
+                        csrfmiddlewaretoken: this.csrfToken,
+                        ...r
+                    }, "PATCH").then(({
+                        ok: a,
+                        data: h
+                    }) => {
+                        a && h.success ? t(h) : i(h)
+                    }, i), i), i);
+                    i(s)
+                })
+            })
+        }
+        LOLauthenticateIdCard(e, t) {}
         getError(e) {
             return this.idCardManager.getError(e)
         }
-    }, S = p;
+    }, I = p;
 
-    function _(h, e) {
-        let t = Object.entries(e).map(([i, s]) => `${encodeURIComponent(i)}=${encodeURIComponent(s)}`).join("&");
-        return fetch(h, {
+    function _(f, e) {
+        let t = Object.entries(e).map(([i, n]) => `${encodeURIComponent(i)}=${encodeURIComponent(n)}`).join("&");
+        return fetch(f, {
             method: "POST",
             headers: {
                 "Content-Type": "application/x-www-form-urlencoded"
             },
             body: t
-        }).then(i => i.json(), i => (console.log(i), {}))
+        }).then(i => i.json().then(n => ({
+            data: n,
+            ok: i.ok
+        })), i => (console.log(i), {}))
     }
     var u = class {
         constructor(e) {
             let t = {
                 language: null,
                 idEndpoints: {
                     start: null,
@@ -294,26 +330,26 @@
                 smartidEndpoints: {
                     start: null,
                     status: null,
                     finalize: null
                 },
                 ...e
             };
-            this.idCardManager = new f(t.language), this.idEndpoints = t.idEndpoints, this.midEndpoints = t.midEndpoints, this.smartidEndpoints = t.smartidEndpoints
+            this.idCardManager = new E(t.language), this.idEndpoints = t.idEndpoints, this.midEndpoints = t.midEndpoints, this.smartidEndpoints = t.smartidEndpoints
         }
-        checkStatus(e, t, i, s) {
-            let n = () => {
+        checkStatus(e, t, i, n) {
+            let s = () => {
                 _(e, t).then(({
                     ok: r,
                     data: a
                 }) => {
-                    r && a.pending ? setTimeout(() => n(), 1e3) : r && a.success ? i(a) : s(a)
+                    r && a.pending ? setTimeout(() => s(), 1e3) : r && a.success ? i(a) : n(a)
                 })
             };
-            return n
+            return s
         }
         signWithIdCard(e) {
             return new Promise((t, i) => {
                 this.__signHandleId(e, t, i)
             })
         }
         signWithMobileId(e) {
@@ -330,81 +366,82 @@
             if (e === u.SIGN_ID) return this.signWithIdCard(t);
             if (e === u.SIGN_MOBILE) return this.signWithMobileId(t);
             if (e === u.SIGN_SMARTID) return this.signWithSmartId(t);
             throw new TypeError("LegacyIdentificationManager: Bad signType")
         }
         __signHandleId(e, t, i) {
             this.idCardManager.initializeIdCard().then(() => {
-                this.idCardManager.getCertificate().then(s => {
+                this.idCardManager.getCertificate().then(n => {
                     _(this.idEndpoints.start, {
                         ...e,
-                        certificate: s
+                        certificate: n
                     }).then(({
-                        ok: n,
+                        ok: s,
                         data: r
                     }) => {
-                        n && r.success ? this.__doSign(r.digest, e, t, i) : i(r)
+                        s && r.success ? this.__doSign(r.digest, e, t, i) : i(r)
                     })
                 }, i)
             }, i)
         }
-        __doSign(e, t, i, s) {
-            this.idCardManager.signHexData(e).then(n => {
+        __doSign(e, t, i, n) {
+            this.idCardManager.signHexData(e).then(s => {
                 _(this.idEndpoints.finish, {
                     ...t,
-                    signature_value: n
+                    signature_value: s
                 }).then(({
                     ok: r,
                     data: a
                 }) => {
-                    r && a.success ? i(a) : s(a)
+                    r && a.success ? i(a) : n(a)
                 })
-            }, s)
+            }, n)
         }
         __signHandleMid(e, t, i) {
             _(this.midEndpoints.start, e).then(({
-                ok: s,
-                data: n
+                ok: n,
+                data: s
             }) => {
-                s && n.success ? t(n) : i(n)
+                n && s.success ? t(s) : i(s)
             })
         }
         midStatus(e) {
             return new Promise((t, i) => {
                 this.checkStatus(this.midEndpoints.status, e, t, i)()
             })
         }
         __signHandleSmartid(e, t, i) {
             _(this.smartidEndpoints.start, e).then(({
-                ok: s,
-                data: n
+                ok: n,
+                data: s
             }) => {
-                s && n.success ? t(n) : i(n)
+                n && s.success ? t(s) : i(s)
             })
         }
         smartidStatus(e) {
             return new Promise((t, i) => {
                 this.checkStatus(this.smartidEndpoints.status, e, t, i)()
             })
         }
         getError(e) {
             return this.idCardManager.getError(e)
         }
     };
     u.SIGN_ID = "id";
     u.SIGN_MOBILE = "mid";
     u.SIGN_SMARTID = "smartid";
-    var A = u;
-    var I = {
-        IdentificationManager: S,
-        LegacyIdentificationManager: A,
-        Languages: {
-            ET: o,
-            EN: d,
-            RU: l,
-            LT: c
-        }
+    var w = u;
+    var T = {
+        ET: o,
+        EN: d,
+        RU: l,
+        LT: c
+    };
+    var S = {
+        IdentificationManager: I,
+        LegacyIdentificationManager: w,
+        Languages: T
     };
-    var T = typeof globalThis < "u" ? globalThis : typeof self < "u" ? self : typeof window < "u" ? window : typeof global < "u" ? global : {};
-    T.Esteid = I;
-    var P = I;
+    var R = typeof globalThis < "u" ? globalThis : typeof self < "u" ? self : typeof window < "u" ? window : typeof global < "u" ? global : {};
+    R.Esteid = S;
+    var O = S;
 })();
```

### Comparing `django_esteid-3.4b1/esteid/static/esteid-helper/web-eid.js` & `django_esteid-4.0b1/esteid/static/esteid-helper/web-eid.js`

 * *Files identical despite different names*

### Comparing `django_esteid-3.4b1/esteid/static/images/esteid/id-kaart-logo.gif` & `django_esteid-4.0b1/esteid/static/images/esteid/id-kaart-logo.gif`

 * *Files identical despite different names*

### Comparing `django_esteid-3.4b1/esteid/static/images/esteid/mid-logo.gif` & `django_esteid-4.0b1/esteid/static/images/esteid/mid-logo.gif`

 * *Files identical despite different names*

### Comparing `django_esteid-3.4b1/esteid/static/images/esteid/smartID-logo-btn.png` & `django_esteid-4.0b1/esteid/static/images/esteid/smartID-logo-btn.png`

 * *Files identical despite different names*

### Comparing `django_esteid-3.4b1/esteid/static/images/esteid/smartID-logo.png` & `django_esteid-4.0b1/esteid/static/images/esteid/smartID-logo.png`

 * *Files identical despite different names*

### Comparing `django_esteid-3.4b1/esteid/templates/esteid/auth-new.html` & `django_esteid-4.0b1/esteid/templates/esteid/test-new.html`

 * *Files 10% similar despite different names*

```diff
@@ -38,91 +38,132 @@
         }
     </style>
 </head>
 
 <body>
 <div class="container">
     <h1>Esteid Test page</h1>
-    <p>
-        This is a test page for <b>digital authentication</b>.
+    <p style="font-size: larger">
+        This is a test page for digital signing of files via python.
     </p>
 
     <p style="font-size: larger">
-        To test out signing, please <a href="{% url "sk_test_new" %}">go to this page</a>.
+        To test out authentication, please <a href="{% url "sk_test_auth_new" %}">go to this page</a>.
     </p>
 
     <h4>Services settings</h4>
     <ul>
         <li><b>Use DEMO:</b> {{ ESTEID_DEMO|yesno }}</li>
         <li><b>ID Card:</b> {{ ID_CARD_ENABLED|yesno }}</li>
         <li><b>Mobile ID:</b> {{ MOBILE_ID_ENABLED|yesno }}, demo: {{ MOBILE_ID_TEST_MODE|yesno }}</li>
         <li><b>SMART ID:</b> {{ SMART_ID_ENABLED|yesno }}, demo: {{ SMART_ID_TEST_MODE|yesno }}</li>
     </ul>
 
     <h4>Notes on Services</h4>
     <ul>
         {% if MOBILE_ID_TEST_MODE %}
             <li>
-                Mobile ID authentication is done with Demo Mobile ID service, you can only use the
+                Mobile ID signing is done with Demo Mobile ID service, you can only use the
                 <a href="https://github.com/SK-EID/MID/wiki/Test-number-for-automated-testing-in-DEMO" target="_blank">demo
                     test numbers</a>.
+                The signatures will not be valid unless the test certificates are used to validate them.
             </li>
         {% endif %}
         {% if ESTEID_DEMO %}
             <li>
-                ID Card authentication can be done with real ID cards.
+                ID Card signing can be done with real ID cards, but such a signature can not be validated
+                unless you point the app to the live OCSP and TimeStamp services.
             </li>
         {% endif %}
         <li>
-            ID Card authentication requires the <b>chrome-token-signing</b> plugin for chrome or firefox.
+            ID Card signing requires the <b>chrome-token-signing</b> plugin for chrome or firefox.
         </li>
         <li>
-            ID Card authentication requires HTTPS. Please refer to the README.
+            ID Card signing requires HTTPS. Please refer to the README.
         </li>
         {% if SMART_ID_TEST_MODE %}
             <li>
-                Authentication with SmartID can be tested with the test ID codes found on the
+                Signing with SmartID can be tested with the test ID codes found on the
                 <a href="https://github.com/SK-EID/smart-id-documentation/wiki/Environment-technical-parameters"
                    target="_blank">SmartID wiki page</a>.
             </li>
             <li>
-                Authentication with <em>SmartID demo app</em> (where you can receive verification codes and enter PINs)
+                Signing with <em>SmartID demo app</em> (where you can receive verification codes and enter PINs)
                 requires setting up a demo SmartID account. Please refer to the README.
             </li>
         {% endif %}
     </ul>
 
     <hr />
 
-    <h3>Choose authentication method</h3>
+    <h3>Uploaded files</h3>
 
-    {% if ID_CARD_ENABLED %}
-        <a href="#" id="sign-id"><img alt="ID Card" src="{% static 'images/esteid/id-kaart-logo.gif' %}"></a>
-    {% endif %}
-    {% if MOBILE_ID_ENABLED %}
-        <a href="#" id="sign-mid"><img alt="Mobile ID" src="{% static 'images/esteid/mid-logo.gif' %}"></a>
-    {% endif %}
-    {% if SMART_ID_ENABLED %}
-        <a href="#" id="sign-smartid"><img alt="Smart ID"
-                                           src="{% static 'images/esteid/smartID-logo-btn.png' %}"></a>
+    {% if files %}
+        <ul class="list-group">
+            {% for file_name, file in files.items %}
+                <li class="list-group-item">
+                    <form method="post" class="pull-right">
+                        {% csrf_token %}
+
+                        <input name="action" type="hidden" value="remove_file" />
+                        <input name="file_name" type="hidden" value="{{ file_name }}" />
+
+                        <input type="submit" class="btn btn-xs btn-danger" value="X" />
+                    </form>
+                    <span class="badge">{{ file.size }} bytes</span>
+
+                    {{ file_name }}
+                </li>
+            {% endfor %}
+        </ul>
+
+        <hr />
+
+        <h3>Sign the files</h3>
+
+        {% if ID_CARD_ENABLED %}
+            <a href="#" id="sign-id"><img alt="ID Card" src="{% static 'images/esteid/id-kaart-logo.gif' %}"></a>
+        {% endif %}
+        {% if MOBILE_ID_ENABLED %}
+            <a href="#" id="sign-mid"><img alt="Mobile ID" src="{% static 'images/esteid/mid-logo.gif' %}"></a>
+        {% endif %}
+        {% if SMART_ID_ENABLED %}
+            <a href="#" id="sign-smartid"><img alt="Smart ID"
+                                               src="{% static 'images/esteid/smartID-logo-btn.png' %}"></a>
+        {% endif %}
+
+    {% else %}
+        <p>No files uploaded, to begin the signing process, please upload some files</p>
     {% endif %}
 
     <hr />
 
+    <h2>Upload files</h2>
+    <form method="POST" enctype="multipart/form-data">
+        {% csrf_token %}
+
+        <div class="form-group">
+            <label for="exampleInputFile">Select file</label>
+            <input type="file" id="exampleInputFile" name="the_file">
+        </div>
+
+        <button type="submit" class="btn btn-default">Submit</button>
+
+    </form>
 </div>
 
 <div class="modal fade" id="mid-modal">
     <div class="modal-dialog">
         <form name="mobileId">
             <div class="modal-content">
                 <div class="modal-header">
                     <button type="button" class="close" data-dismiss="modal" aria-label="Close"><span
                             aria-hidden="true">&times;</span>
                     </button>
-                    <h4 class="modal-title">Authentication with MobileID</h4>
+                    <h4 class="modal-title">Sign the files with MobileID</h4>
                 </div>
 
                 <div class="modal-body">
                     <div class="form-group">
                         <label for="phoneNrInput">Demo Phone nr:</label>
                         <input type="text" name="phone_nr" id="phoneNrInput" class="form-control"
                                value="{{ request.session.ddoc_test_phone_number | default:'+37200000766' }}" />
@@ -131,15 +172,15 @@
                         <label for="idCodeInput">Demo ID code:</label>
                         <input type="text" name="id_code" id="idCodeInput" class="form-control"
                                value="{{ request.session.ddoc_test_id_code | default:'60001019906' }}" />
                     </div>
                 </div>
 
                 <div class="modal-footer">
-                    <button type="submit" class="btn btn-primary">Authenticate</button>
+                    <button type="submit" class="btn btn-primary">Sign</button>
                     <div class="lds-dual-ring"></div>
                 </div>
             </div>
         </form>
     </div>
 </div>
 
@@ -160,50 +201,35 @@
     </div>
 </div>
 
 <div class="modal fade" id="id-modal">
     <div class="modal-dialog">
         <div class="modal-content">
             <div class="modal-header">
-                <h4 class="modal-title">Authentication with ID Card</h4>
+                <h4 class="modal-title">Signing with digital ID</h4>
             </div>
 
             <div class="modal-body">
                 <p>
-                    Please follow the instructions to complete the authentication process.
-                </p>
-                {# *** THIS IS NECESSARY ONLY FOR TESTING LOCALLY, BECAUSE OF THE SELF-SIGNED CERTIFICATE. *** #}
-                {# *** BEGIN *** #}
-                <hr>
-                <h3>Testing locally?</h3>
-                <p>
-                    If you haven't done it yet, open the link <br>
-                    <a href="#" id="auth-host"></a> <br>
-                    in a new tab and confirm security exception.
+                    Please follow the instructions to complete the signing process.
                 </p>
-                <p>
-                    <button onclick="securityException = true; authWithIDCard()">OK, DONE</button>
-                </p>
-                {# *** END ***  #}
             </div>
         </div>
     </div>
 </div>
 
-<div id="idCardAuthWrapper" />
-
 <div class="modal fade" id="smartid-modal">
     <div class="modal-dialog">
         <form name="smartId">
             <div class="modal-content">
                 <div class="modal-header">
                     <button type="button" class="close" data-dismiss="modal" aria-label="Close"><span
                             aria-hidden="true">&times;</span>
                     </button>
-                    <h4 class="modal-title">Authentication with SmartID</h4>
+                    <h4 class="modal-title">Sign the files with SmartID</h4>
                 </div>
 
                 <div class="modal-body">
                     <div class="form-group">
                         <label for="idCodeInput">Your ID code:</label>
                         <input type="text" name="id_code" id="idCodeInput" class="form-control"
                                value="{{ request.session.smartid_test_id_code | default:'30303039914' }}" />
@@ -216,15 +242,15 @@
                             <option value="LV">Latvia</option>
                             <option value="LT">Lithuania</option>
                         </select>
                     </div>
                 </div>
 
                 <div class="modal-footer">
-                    <button type="submit" class="btn btn-primary">Authenticate</button>
+                    <button type="submit" class="btn btn-primary">Sign</button>
                     <div class="lds-dual-ring"></div>
                 </div>
             </div>
         </form>
     </div>
 </div>
 
@@ -245,31 +271,34 @@
     </div>
 </div>
 
 <div class="modal fade" id="success-modal">
     <div class="modal-dialog">
         <div class="modal-content">
             <div class="modal-header">
-                <h4 class="modal-title">Authentication complete</h4>
+                <h4 class="modal-title">Signing complete</h4>
             </div>
 
             <div class="modal-body">
                 <p>
-                    Greetings, <i id="given-name"></i> <i id="surname"></i>!
+                    The uploaded files were successfully digitally signed, please click the following link
+                    to download the container and finish the signing process.
                 </p>
 
-                <a href="#" onclick="window.location.reload(); return false">OK</a>
+                <a href="#" id="get-document" target="_blank">Download file</a> &middot;
+                <a href="#" onclick="window.location.reload(); return false">Cancel</a>
             </div>
         </div>
     </div>
 </div>
 
 <script src="//ajax.googleapis.com/ajax/libs/jquery/1.11.1/jquery.min.js"></script>
 <script src="//maxcdn.bootstrapcdn.com/bootstrap/3.3.4/js/bootstrap.min.js"></script>
 
+
 <script type="text/javascript" src="{% static 'esteid-helper/web-eid.js' %}"></script>
 <script type="text/javascript" src="{% static 'esteid-helper/Esteid.main.web.js' %}"></script>
 
 <script type="text/javascript">
     function startSpinner(form) {
         $("button", form).hide()
         $(".lds-dual-ring", form).css("display", "inline-block")
@@ -277,104 +306,45 @@
 
     function stopSpinner(form) {
         $("button", form).show()
         $(".lds-dual-ring", form).css("display", "none")
     }
 
     function onError(res) {
-        $('#verification-code-modal').modal("hide")
-        $('#challenge-modal').modal('hide')
-
         console.log("Error:", res)
         if (res && res.message) {
             alert(res.message)
         } else {
             alert('Something went wrong, please try again')
         }
     }
 
-    {# *** TESTING ONLY *** #}
-    let securityException = false
-    {# *** In real apps, use some other algorithm to build the auth host name *** #}
-    const IFRAME_HOST = 'https://${RANDOM}.auth.127.0.0.1.xip.io:8443'.replace(
-        "${RANDOM}", Math.ceil(Number.MAX_SAFE_INTEGER * Math.random())
-    )
-
-    const idUrl = IFRAME_HOST + '{% url 'auth-idcard' %}'
-
-    const SITE_HOST = 'https://127.0.0.1.xip.io:8443'
-
-    function onAuthComplete(data) {
-        $('#success-modal').modal({
-            backdrop: 'static',
-            keyboard: false
-        })
-
-        $('#given-name').text(data.given_name)
-        $('#surname').text(data.surname)
-    }
-
-    function authWithIDCard (e) {
-        e && e.preventDefault()
-
-        $('#id-modal').modal({
-            backdrop: 'static',
-            keyboard: false
-        })
-
-        {# NECESSARY FOR TESTING ONLY #}
-        if (!securityException) { return }
-
-        var parentElement = document.getElementById('idCardAuthWrapper')
-
-        var idcardAuthFrame = document.createElement("iframe")
-        idcardAuthFrame.id = "idCardAuthFrame"
-        idcardAuthFrame.src = idUrl
-        idcardAuthFrame.width = 1
-        idcardAuthFrame.height = 1
-        idcardAuthFrame.onload = () => console.log("LOADED")
-        parentElement.appendChild(idcardAuthFrame)
-
-        function handleMessageFromIFrame(evt) {
-            if(evt.origin.startsWith(IFRAME_HOST) || evt.origin.startsWith(SITE_HOST)) {
-                console.log('idcardAuthFrame sent Data:', evt.data);
-                if (evt.data.error) {
-                    alert(evt.data.error + ": " + evt.data.message)
-                } else {
-                    onAuthComplete(evt.data)
-                }
-            } else {
-                console.error('Unexpected origin', evt.origin, 'Tried to send Data', evt.data);
-                alert("Something went wrong")
-            }
-            $('#id-modal').modal('hide')
-            parentElement.removeChild(idcardAuthFrame)
-            // remove the listener anyway.
-            window.removeEventListener('message', handleMessageFromIFrame, false)
-        }
-        window.addEventListener('message', handleMessageFromIFrame, false);
-    }
-
     $(function () {
-        var authHostLink = document.getElementById('auth-host')
-        authHostLink.innerText = IFRAME_HOST
-        authHostLink.setAttribute('href', IFRAME_HOST)
-
+        var downloadUrl = '{% url 'download_signed_container' %}'
         var manager = new Esteid.IdentificationManager({
             language: Esteid.Languages.ET,
 
-            idUrl, {# This is not used: Id Card authentication doesn't involve manager #}
+            idUrl: '{% url 'sign-idcard' %}',
 
-            mobileIdUrl: '{% url 'auth-mobileid' %}',
+            mobileIdUrl: '{% url 'sign-mobileid' %}',
 
-            smartIdUrl: '{% url 'auth-smartid' %}',
+            smartIdUrl: '{% url 'sign-smartid' %}',
 
             csrfToken: '{{ csrf_token }}'
         })
 
+        function onSigned() {
+            $('#get-document').attr('href', downloadUrl)
+
+            $('#success-modal').modal({
+                backdrop: 'static',
+                keyboard: false
+            })
+        }
+
         $('#sign-mid').on('click', function (e) {
             e.preventDefault()
 
             $('#mid-modal').modal()
         })
 
         var mobileIdForm = document.forms.mobileId
@@ -411,22 +381,30 @@
                         backdrop: 'static',
                         keyboard: false
                     })
 
                     $('#mid-modal').modal('hide')
 
                     manager.midStatus().then(
-                        function (data) {
+                        function () {
                             $('#challenge-modal').modal('hide')
-                            onAuthComplete(data)
+                            onSigned()
                         },
-                        onError
-                    ).finally(
-                        () => stopSpinner(mobileIdForm)
+
+                        function (res) {
+                            if (res.message) {
+                                alert(res.message)
+                            } else {
+                                alert('Something went wrong, please try again')
+                            }
+
+                            $('#challenge-modal').modal('hide')
+                        }
                     )
+
                 }, onError)
                 .finally(
                     () => stopSpinner(mobileIdForm)
                 )
         }
 
         $('#sign-smartid').on('click', function (e) {
@@ -436,40 +414,66 @@
         })
 
         var smartIdForm = document.forms.smartId
         smartIdForm.onsubmit = function (e) {
             console.log("Signing with Smart ID")
             var timeoutForVerificationCode = 3000  // delay polling to let user to enter verification code
 
-            function onAuthInitSuccess(response) {
+            /** Seems no longer necessary for signing. Kept here as it might be useful for authentication */
+            function onSuccessAuth(response) {
                 // Got a successful auth-start request...
                 console.log('SmartID: auth verification code', response.verification_code)
                 $('#verification-code-modal').modal({
                     backdrop: 'static',
                     keyboard: false
                 })
 
                 $('#smartid-step').text('Authentication')
                 $('#smartid-verification-code').text(response.verification_code)
 
                 // ...next phase: start signing
                 // we don't want to start polling immediately because user will need to enter verification code
                 setTimeout(function () {
                     manager.smartidStatus().then(
-                        (data) => {
-                            $('#smartid-modal').modal("hide")
-                            onAuthComplete(data)
-                        },
+                        onStartSign,
                         onError
                     ).finally(
                         () => stopSpinner(smartIdForm)
                     )
                 }, timeoutForVerificationCode)
             }
 
+            function onStartSign(response) {
+                // Got a successful sign-start request...
+                console.log('SmartID: Signing verification code', response.verification_code)
+
+                $('#smartid-modal').modal('hide')
+
+                $('#verification-code-modal').modal({
+                    backdrop: 'static',
+                    keyboard: false
+                })
+
+                $('#smartid-step').text('Signing')
+                $('#smartid-verification-code').text(response.verification_code)
+
+                // ...next phase: poll for status of signing
+                setTimeout(function () {
+                    manager.smartidStatus().then(
+                        onFinishSign,
+                        onError
+                    )
+                }, timeoutForVerificationCode)
+            }
+
+            function onFinishSign() {
+                $('#smartid-modal').modal("hide")
+                onSigned()
+            }
+
             e.preventDefault()
             var idCode = smartIdForm.id_code.value
             var country = smartIdForm.country.value
 
             if (!idCode) {
                 alert('Please enter an ID code')
                 return
@@ -479,22 +483,59 @@
 
             startSpinner(smartIdForm)
 
             manager.signWithSmartId({
                 idCode,
                 country,
             }).then(
-                onAuthInitSuccess,
+                // Start callback hell
+                onStartSign,
                 onError
             ).finally(
                 () => stopSpinner(smartIdForm)
             )
         }
 
-        $('#sign-id').on('click', authWithIDCard)
+        $('#sign-id').on('click', function (e) {
+            e.preventDefault()
+
+            $('#id-modal').modal({
+                backdrop: 'static',
+                keyboard: false
+            })
+
+            manager.signWithIdCard().then(
+                function () {
+                    $('#id-modal').modal('hide')
+                    onSigned()
+                },
+
+                function (res) {
+                    if (res instanceof Error) {
+                        console.log(res.message, res)
+                        res = manager.getError(res)
+
+                        alert(res.message)
+
+                        console.error('[Error code: ' + res.returnCode + '; Error: ' + res.message + ']')
+                        $('#id-modal').modal('hide')
+                    } else {
+                        if (typeof res === 'string' || res.error_code) {
+                            var msg = res.message !== undefined ? res.message : res
+
+                            alert(msg)
+                            $('#id-modal').modal('hide')
+                        } else {
+                            console.error(res.message !== undefined ? res.message : res)
+                            alert('Something went wrong, please refresh the page and try again')
+                        }
+                    }
+                }
+            )
+        })
 
         $('#get-document').on('click', function () {
             setTimeout(function () {
                 window.location.reload()
             }, 2000)
         })
     })
```

#### html2text {}

```diff
@@ -1,68 +1,77 @@
 {% load static %}
 
 
 ****** Esteid Test page ******
-This is a test page for digital authentication.
-To test out signing, please  %}">go to this page
+This is a test page for digital signing of files via python.
+To test out authentication, please  %}">go to this page
 .
 *** Services settings ***
     * Use DEMO: {{ ESTEID_DEMO|yesno }}
     * ID Card: {{ ID_CARD_ENABLED|yesno }}
     * Mobile ID: {{ MOBILE_ID_ENABLED|yesno }}, demo: {
       { MOBILE_ID_TEST_MODE|yesno }}
     * SMART ID: {{ SMART_ID_ENABLED|yesno }}, demo: {{ SMART_ID_TEST_MODE|yesno
       }}
 *** Notes on Services ***
     * {% if MOBILE_ID_TEST_MODE %}
-    * Mobile ID authentication is done with Demo Mobile ID service, you can
-      only use the demo_test_numbers.
+    * Mobile ID signing is done with Demo Mobile ID service, you can only use
+      the demo_test_numbers. The signatures will not be valid unless the test
+      certificates are used to validate them.
     * {% endif %} {% if ESTEID_DEMO %}
-    * ID Card authentication can be done with real ID cards.
+    * ID Card signing can be done with real ID cards, but such a signature can
+      not be validated unless you point the app to the live OCSP and TimeStamp
+      services.
     * {% endif %}
-    * ID Card authentication requires the chrome-token-signing plugin for
-      chrome or firefox.
-    * ID Card authentication requires HTTPS. Please refer to the README.
+    * ID Card signing requires the chrome-token-signing plugin for chrome or
+      firefox.
+    * ID Card signing requires HTTPS. Please refer to the README.
     * {% if SMART_ID_TEST_MODE %}
-    * Authentication with SmartID can be tested with the test ID codes found on
-      the SmartID_wiki_page.
-    * Authentication with SmartID demo app (where you can receive verification
-      codes and enter PINs) requires setting up a demo SmartID account. Please
-      refer to the README.
+    * Signing with SmartID can be tested with the test ID codes found on the
+      SmartID_wiki_page.
+    * Signing with SmartID demo app (where you can receive verification codes
+      and enter PINs) requires setting up a demo SmartID account. Please refer
+      to the README.
     * {% endif %}
 ===============================================================================
-**** Choose authentication method ****
+**** Uploaded files ****
+{% if files %}
+    * {% for file_name, file in files.items %}
+    * {% csrf_token %}   [X]
+      {{ file.size }} bytes {{ file_name }}
+    * {% endfor %}
+===============================================================================
+**** Sign the files ****
 {% if ID_CARD_ENABLED %} [ID_Card] {% endif %} {% if MOBILE_ID_ENABLED %}
-[Mobile_ID] {% endif %} {% if SMART_ID_ENABLED %} [Smart_ID] {% endif %}
+[Mobile_ID] {% endif %} {% if SMART_ID_ENABLED %} [Smart_ID] {% endif %} {%
+else %}
+No files uploaded, to begin the signing process, please upload some files
+{% endif %}
 ===============================================================================
+***** Upload files *****
+{% csrf_token %}
+Select file [File]
+Submit
 ×
-*** Authentication with MobileID ***
+*** Sign the files with MobileID ***
 Demo Phone nr: [{{ request.session.ddoc_test_phone_number | default:
 '+37200000766' }}]
 Demo ID code: [{{ request.session.ddoc_test_id_code | default:'60001019906' }}]
-Authenticate
+Sign
 *** MID Step 2 ***
 Please enter the following code into your mobile to proceed with the signing
 process: KOOD
-*** Authentication with ID Card ***
-Please follow the instructions to complete the authentication process.
-{# *** THIS IS NECESSARY ONLY FOR TESTING LOCALLY, BECAUSE OF THE SELF-SIGNED
-CERTIFICATE. *** #} {# *** BEGIN *** #}
-===============================================================================
-**** Testing locally? ****
-If you haven't done it yet, open the link
-
-in a new tab and confirm security exception.
-OK, DONE
-{# *** END *** #}
+*** Signing with digital ID ***
+Please follow the instructions to complete the signing process.
 ×
-*** Authentication with SmartID ***
+*** Sign the files with SmartID ***
 Your ID code: [{{ request.session.smartid_test_id_code | default:'30303039914'
 }}]
 Country: [One of: -- Not selected -- (defaults to Estonia)/Estonia/Latvia/
 Lithuania]
-Authenticate
+Sign
 *** Verification code ***
 Make sure you are seeing this verification code on your device: KOOD
-*** Authentication complete ***
-Greetings,  !
-OK
+*** Signing complete ***
+The uploaded files were successfully digitally signed, please click the
+following link to download the container and finish the signing process.
+Download_file · Cancel
```

### Comparing `django_esteid-3.4b1/esteid/templates/esteid/test-new.html` & `django_esteid-4.0b1/esteid/templates/esteid/test.html`

 * *Files 16% similar despite different names*

```diff
@@ -11,1179 +11,955 @@
 000000a0: 4353 5320 2d2d 3e0a 2020 2020 3c6c 696e  CSS -->.    <lin
 000000b0: 6b20 7265 6c3d 2273 7479 6c65 7368 6565  k rel="styleshee
 000000c0: 7422 2068 7265 663d 2268 7474 7073 3a2f  t" href="https:/
 000000d0: 2f6d 6178 6364 6e2e 626f 6f74 7374 7261  /maxcdn.bootstra
 000000e0: 7063 646e 2e63 6f6d 2f62 6f6f 7473 7472  pcdn.com/bootstr
 000000f0: 6170 2f33 2e33 2e34 2f63 7373 2f62 6f6f  ap/3.3.4/css/boo
 00000100: 7473 7472 6170 2e6d 696e 2e63 7373 223e  tstrap.min.css">
-00000110: 0a20 2020 203c 212d 2d20 7369 6d70 6c65  .    <!-- simple
-00000120: 2073 7069 6e6e 6572 2066 726f 6d20 6c6f   spinner from lo
-00000130: 6164 696e 672e 696f 202d 2d3e 0a20 2020  ading.io -->.   
-00000140: 203c 7374 796c 6520 7479 7065 3d22 7465   <style type="te
-00000150: 7874 2f63 7373 223e 0a20 2020 2020 2020  xt/css">.       
-00000160: 202e 6c64 732d 6475 616c 2d72 696e 6720   .lds-dual-ring 
-00000170: 7b0a 2020 2020 2020 2020 2020 2020 2f2a  {.            /*
-00000180: 2064 6973 706c 6179 3a20 696e 6c69 6e65   display: inline
-00000190: 2d62 6c6f 636b 3b20 2a2f 0a20 2020 2020  -block; */.     
-000001a0: 2020 2020 2020 2064 6973 706c 6179 3a20         display: 
-000001b0: 6e6f 6e65 3b0a 2020 2020 2020 2020 2020  none;.          
-000001c0: 2020 7769 6474 683a 2038 3070 783b 0a20    width: 80px;. 
-000001d0: 2020 2020 2020 2020 2020 2068 6569 6768             heigh
-000001e0: 743a 2038 3070 783b 0a20 2020 2020 2020  t: 80px;.       
-000001f0: 207d 0a0a 2020 2020 2020 2020 2e6c 6473   }..        .lds
-00000200: 2d64 7561 6c2d 7269 6e67 3a61 6674 6572  -dual-ring:after
-00000210: 207b 0a20 2020 2020 2020 2020 2020 2063   {.            c
-00000220: 6f6e 7465 6e74 3a20 2220 223b 0a20 2020  ontent: " ";.   
-00000230: 2020 2020 2020 2020 2064 6973 706c 6179           display
-00000240: 3a20 626c 6f63 6b3b 0a20 2020 2020 2020  : block;.       
-00000250: 2020 2020 2077 6964 7468 3a20 3634 7078       width: 64px
-00000260: 3b0a 2020 2020 2020 2020 2020 2020 6865  ;.            he
-00000270: 6967 6874 3a20 3634 7078 3b0a 2020 2020  ight: 64px;.    
-00000280: 2020 2020 2020 2020 6d61 7267 696e 3a20          margin: 
-00000290: 3870 783b 0a20 2020 2020 2020 2020 2020  8px;.           
-000002a0: 2062 6f72 6465 722d 7261 6469 7573 3a20   border-radius: 
-000002b0: 3530 253b 0a20 2020 2020 2020 2020 2020  50%;.           
-000002c0: 2062 6f72 6465 723a 2036 7078 2073 6f6c   border: 6px sol
-000002d0: 6964 2023 3333 3333 3333 3b0a 2020 2020  id #333333;.    
-000002e0: 2020 2020 2020 2020 626f 7264 6572 2d63          border-c
-000002f0: 6f6c 6f72 3a20 2333 3333 3333 3320 7472  olor: #333333 tr
-00000300: 616e 7370 6172 656e 7420 2333 3333 3333  ansparent #33333
-00000310: 3320 7472 616e 7370 6172 656e 743b 0a20  3 transparent;. 
-00000320: 2020 2020 2020 2020 2020 2061 6e69 6d61             anima
-00000330: 7469 6f6e 3a20 6c64 732d 6475 616c 2d72  tion: lds-dual-r
-00000340: 696e 6720 312e 3273 206c 696e 6561 7220  ing 1.2s linear 
-00000350: 696e 6669 6e69 7465 3b0a 2020 2020 2020  infinite;.      
-00000360: 2020 7d0a 0a20 2020 2020 2020 2040 6b65    }..        @ke
-00000370: 7966 7261 6d65 7320 6c64 732d 6475 616c  yframes lds-dual
-00000380: 2d72 696e 6720 7b0a 2020 2020 2020 2020  -ring {.        
-00000390: 2020 2020 3025 207b 0a20 2020 2020 2020      0% {.       
-000003a0: 2020 2020 2020 2020 2074 7261 6e73 666f           transfo
-000003b0: 726d 3a20 726f 7461 7465 2830 6465 6729  rm: rotate(0deg)
-000003c0: 3b0a 2020 2020 2020 2020 2020 2020 7d0a  ;.            }.
-000003d0: 2020 2020 2020 2020 2020 2020 3130 3025              100%
-000003e0: 207b 0a20 2020 2020 2020 2020 2020 2020   {.             
-000003f0: 2020 2074 7261 6e73 666f 726d 3a20 726f     transform: ro
-00000400: 7461 7465 2833 3630 6465 6729 3b0a 2020  tate(360deg);.  
-00000410: 2020 2020 2020 2020 2020 7d0a 2020 2020            }.    
-00000420: 2020 2020 7d0a 2020 2020 3c2f 7374 796c      }.    </styl
-00000430: 653e 0a3c 2f68 6561 643e 0a0a 3c62 6f64  e>.</head>..<bod
-00000440: 793e 0a3c 6469 7620 636c 6173 733d 2263  y>.<div class="c
-00000450: 6f6e 7461 696e 6572 223e 0a20 2020 203c  ontainer">.    <
-00000460: 6831 3e45 7374 6569 6420 5465 7374 2070  h1>Esteid Test p
-00000470: 6167 653c 2f68 313e 0a20 2020 203c 7020  age</h1>.    <p 
-00000480: 7374 796c 653d 2266 6f6e 742d 7369 7a65  style="font-size
-00000490: 3a20 6c61 7267 6572 223e 0a20 2020 2020  : larger">.     
-000004a0: 2020 2054 6869 7320 6973 2061 2074 6573     This is a tes
-000004b0: 7420 7061 6765 2066 6f72 2064 6967 6974  t page for digit
-000004c0: 616c 2073 6967 6e69 6e67 206f 6620 6669  al signing of fi
-000004d0: 6c65 7320 7669 6120 7079 7468 6f6e 2e0a  les via python..
-000004e0: 2020 2020 3c2f 703e 0a0a 2020 2020 3c70      </p>..    <p
-000004f0: 2073 7479 6c65 3d22 666f 6e74 2d73 697a   style="font-siz
-00000500: 653a 206c 6172 6765 7222 3e0a 2020 2020  e: larger">.    
-00000510: 2020 2020 546f 2074 6573 7420 6f75 7420      To test out 
-00000520: 6175 7468 656e 7469 6361 7469 6f6e 2c20  authentication, 
-00000530: 706c 6561 7365 203c 6120 6872 6566 3d22  please <a href="
-00000540: 7b25 2075 726c 2022 736b 5f74 6573 745f  {% url "sk_test_
-00000550: 6175 7468 5f6e 6577 2220 257d 223e 676f  auth_new" %}">go
-00000560: 2074 6f20 7468 6973 2070 6167 653c 2f61   to this page</a
-00000570: 3e2e 0a20 2020 203c 2f70 3e0a 0a20 2020  >..    </p>..   
-00000580: 203c 6834 3e53 6572 7669 6365 7320 7365   <h4>Services se
-00000590: 7474 696e 6773 3c2f 6834 3e0a 2020 2020  ttings</h4>.    
-000005a0: 3c75 6c3e 0a20 2020 2020 2020 203c 6c69  <ul>.        <li
-000005b0: 3e3c 623e 5573 6520 4445 4d4f 3a3c 2f62  ><b>Use DEMO:</b
-000005c0: 3e20 7b7b 2045 5354 4549 445f 4445 4d4f  > {{ ESTEID_DEMO
-000005d0: 7c79 6573 6e6f 207d 7d3c 2f6c 693e 0a20  |yesno }}</li>. 
-000005e0: 2020 2020 2020 203c 6c69 3e3c 623e 4944         <li><b>ID
-000005f0: 2043 6172 643a 3c2f 623e 207b 7b20 4944   Card:</b> {{ ID
-00000600: 5f43 4152 445f 454e 4142 4c45 447c 7965  _CARD_ENABLED|ye
-00000610: 736e 6f20 7d7d 3c2f 6c69 3e0a 2020 2020  sno }}</li>.    
-00000620: 2020 2020 3c6c 693e 3c62 3e4d 6f62 696c      <li><b>Mobil
-00000630: 6520 4944 3a3c 2f62 3e20 7b7b 204d 4f42  e ID:</b> {{ MOB
-00000640: 494c 455f 4944 5f45 4e41 424c 4544 7c79  ILE_ID_ENABLED|y
-00000650: 6573 6e6f 207d 7d2c 2064 656d 6f3a 207b  esno }}, demo: {
-00000660: 7b20 4d4f 4249 4c45 5f49 445f 5445 5354  { MOBILE_ID_TEST
-00000670: 5f4d 4f44 457c 7965 736e 6f20 7d7d 3c2f  _MODE|yesno }}</
-00000680: 6c69 3e0a 2020 2020 2020 2020 3c6c 693e  li>.        <li>
-00000690: 3c62 3e53 4d41 5254 2049 443a 3c2f 623e  <b>SMART ID:</b>
-000006a0: 207b 7b20 534d 4152 545f 4944 5f45 4e41   {{ SMART_ID_ENA
-000006b0: 424c 4544 7c79 6573 6e6f 207d 7d2c 2064  BLED|yesno }}, d
-000006c0: 656d 6f3a 207b 7b20 534d 4152 545f 4944  emo: {{ SMART_ID
-000006d0: 5f54 4553 545f 4d4f 4445 7c79 6573 6e6f  _TEST_MODE|yesno
-000006e0: 207d 7d3c 2f6c 693e 0a20 2020 203c 2f75   }}</li>.    </u
-000006f0: 6c3e 0a0a 2020 2020 3c68 343e 4e6f 7465  l>..    <h4>Note
-00000700: 7320 6f6e 2053 6572 7669 6365 733c 2f68  s on Services</h
-00000710: 343e 0a20 2020 203c 756c 3e0a 2020 2020  4>.    <ul>.    
-00000720: 2020 2020 7b25 2069 6620 4d4f 4249 4c45      {% if MOBILE
-00000730: 5f49 445f 5445 5354 5f4d 4f44 4520 257d  _ID_TEST_MODE %}
-00000740: 0a20 2020 2020 2020 2020 2020 203c 6c69  .            <li
-00000750: 3e0a 2020 2020 2020 2020 2020 2020 2020  >.              
-00000760: 2020 4d6f 6269 6c65 2049 4420 7369 676e    Mobile ID sign
-00000770: 696e 6720 6973 2064 6f6e 6520 7769 7468  ing is done with
-00000780: 2044 656d 6f20 4d6f 6269 6c65 2049 4420   Demo Mobile ID 
-00000790: 7365 7276 6963 652c 2079 6f75 2063 616e  service, you can
-000007a0: 206f 6e6c 7920 7573 6520 7468 650a 2020   only use the.  
-000007b0: 2020 2020 2020 2020 2020 2020 2020 3c61                <a
-000007c0: 2068 7265 663d 2268 7474 7073 3a2f 2f67   href="https://g
-000007d0: 6974 6875 622e 636f 6d2f 534b 2d45 4944  ithub.com/SK-EID
-000007e0: 2f4d 4944 2f77 696b 692f 5465 7374 2d6e  /MID/wiki/Test-n
-000007f0: 756d 6265 722d 666f 722d 6175 746f 6d61  umber-for-automa
-00000800: 7465 642d 7465 7374 696e 672d 696e 2d44  ted-testing-in-D
-00000810: 454d 4f22 2074 6172 6765 743d 225f 626c  EMO" target="_bl
-00000820: 616e 6b22 3e64 656d 6f0a 2020 2020 2020  ank">demo.      
-00000830: 2020 2020 2020 2020 2020 2020 2020 7465                te
-00000840: 7374 206e 756d 6265 7273 3c2f 613e 2e0a  st numbers</a>..
-00000850: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000860: 5468 6520 7369 676e 6174 7572 6573 2077  The signatures w
-00000870: 696c 6c20 6e6f 7420 6265 2076 616c 6964  ill not be valid
-00000880: 2075 6e6c 6573 7320 7468 6520 7465 7374   unless the test
-00000890: 2063 6572 7469 6669 6361 7465 7320 6172   certificates ar
-000008a0: 6520 7573 6564 2074 6f20 7661 6c69 6461  e used to valida
-000008b0: 7465 2074 6865 6d2e 0a20 2020 2020 2020  te them..       
-000008c0: 2020 2020 203c 2f6c 693e 0a20 2020 2020       </li>.     
-000008d0: 2020 207b 2520 656e 6469 6620 257d 0a20     {% endif %}. 
-000008e0: 2020 2020 2020 207b 2520 6966 2045 5354         {% if EST
-000008f0: 4549 445f 4445 4d4f 2025 7d0a 2020 2020  EID_DEMO %}.    
-00000900: 2020 2020 2020 2020 3c6c 693e 0a20 2020          <li>.   
-00000910: 2020 2020 2020 2020 2020 2020 2049 4420               ID 
-00000920: 4361 7264 2073 6967 6e69 6e67 2063 616e  Card signing can
-00000930: 2062 6520 646f 6e65 2077 6974 6820 7265   be done with re
-00000940: 616c 2049 4420 6361 7264 732c 2062 7574  al ID cards, but
-00000950: 2073 7563 6820 6120 7369 676e 6174 7572   such a signatur
-00000960: 6520 6361 6e20 6e6f 7420 6265 2076 616c  e can not be val
-00000970: 6964 6174 6564 0a20 2020 2020 2020 2020  idated.         
-00000980: 2020 2020 2020 2075 6e6c 6573 7320 796f         unless yo
-00000990: 7520 706f 696e 7420 7468 6520 6170 7020  u point the app 
-000009a0: 746f 2074 6865 206c 6976 6520 4f43 5350  to the live OCSP
-000009b0: 2061 6e64 2054 696d 6553 7461 6d70 2073   and TimeStamp s
-000009c0: 6572 7669 6365 732e 0a20 2020 2020 2020  ervices..       
-000009d0: 2020 2020 203c 2f6c 693e 0a20 2020 2020       </li>.     
-000009e0: 2020 207b 2520 656e 6469 6620 257d 0a20     {% endif %}. 
-000009f0: 2020 2020 2020 203c 6c69 3e0a 2020 2020         <li>.    
-00000a00: 2020 2020 2020 2020 4944 2043 6172 6420          ID Card 
-00000a10: 7369 676e 696e 6720 7265 7175 6972 6573  signing requires
-00000a20: 2074 6865 203c 623e 6368 726f 6d65 2d74   the <b>chrome-t
-00000a30: 6f6b 656e 2d73 6967 6e69 6e67 3c2f 623e  oken-signing</b>
-00000a40: 2070 6c75 6769 6e20 666f 7220 6368 726f   plugin for chro
-00000a50: 6d65 206f 7220 6669 7265 666f 782e 0a20  me or firefox.. 
-00000a60: 2020 2020 2020 203c 2f6c 693e 0a20 2020         </li>.   
-00000a70: 2020 2020 203c 6c69 3e0a 2020 2020 2020       <li>.      
-00000a80: 2020 2020 2020 4944 2043 6172 6420 7369        ID Card si
-00000a90: 676e 696e 6720 7265 7175 6972 6573 2048  gning requires H
-00000aa0: 5454 5053 2e20 506c 6561 7365 2072 6566  TTPS. Please ref
-00000ab0: 6572 2074 6f20 7468 6520 5245 4144 4d45  er to the README
-00000ac0: 2e0a 2020 2020 2020 2020 3c2f 6c69 3e0a  ..        </li>.
-00000ad0: 2020 2020 2020 2020 7b25 2069 6620 534d          {% if SM
-00000ae0: 4152 545f 4944 5f54 4553 545f 4d4f 4445  ART_ID_TEST_MODE
-00000af0: 2025 7d0a 2020 2020 2020 2020 2020 2020   %}.            
-00000b00: 3c6c 693e 0a20 2020 2020 2020 2020 2020  <li>.           
-00000b10: 2020 2020 2053 6967 6e69 6e67 2077 6974       Signing wit
-00000b20: 6820 536d 6172 7449 4420 6361 6e20 6265  h SmartID can be
-00000b30: 2074 6573 7465 6420 7769 7468 2074 6865   tested with the
-00000b40: 2074 6573 7420 4944 2063 6f64 6573 2066   test ID codes f
-00000b50: 6f75 6e64 206f 6e20 7468 650a 2020 2020  ound on the.    
-00000b60: 2020 2020 2020 2020 2020 2020 3c61 2068              <a h
-00000b70: 7265 663d 2268 7474 7073 3a2f 2f67 6974  ref="https://git
-00000b80: 6875 622e 636f 6d2f 534b 2d45 4944 2f73  hub.com/SK-EID/s
-00000b90: 6d61 7274 2d69 642d 646f 6375 6d65 6e74  mart-id-document
-00000ba0: 6174 696f 6e2f 7769 6b69 2f45 6e76 6972  ation/wiki/Envir
-00000bb0: 6f6e 6d65 6e74 2d74 6563 686e 6963 616c  onment-technical
-00000bc0: 2d70 6172 616d 6574 6572 7322 0a20 2020  -parameters".   
-00000bd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000be0: 7461 7267 6574 3d22 5f62 6c61 6e6b 223e  target="_blank">
-00000bf0: 536d 6172 7449 4420 7769 6b69 2070 6167  SmartID wiki pag
-00000c00: 653c 2f61 3e2e 0a20 2020 2020 2020 2020  e</a>..         
-00000c10: 2020 203c 2f6c 693e 0a20 2020 2020 2020     </li>.       
-00000c20: 2020 2020 203c 6c69 3e0a 2020 2020 2020       <li>.      
-00000c30: 2020 2020 2020 2020 2020 5369 676e 696e            Signin
-00000c40: 6720 7769 7468 203c 656d 3e53 6d61 7274  g with <em>Smart
-00000c50: 4944 2064 656d 6f20 6170 703c 2f65 6d3e  ID demo app</em>
-00000c60: 2028 7768 6572 6520 796f 7520 6361 6e20   (where you can 
-00000c70: 7265 6365 6976 6520 7665 7269 6669 6361  receive verifica
-00000c80: 7469 6f6e 2063 6f64 6573 2061 6e64 2065  tion codes and e
-00000c90: 6e74 6572 2050 494e 7329 0a20 2020 2020  nter PINs).     
-00000ca0: 2020 2020 2020 2020 2020 2072 6571 7569             requi
-00000cb0: 7265 7320 7365 7474 696e 6720 7570 2061  res setting up a
-00000cc0: 2064 656d 6f20 536d 6172 7449 4420 6163   demo SmartID ac
-00000cd0: 636f 756e 742e 2050 6c65 6173 6520 7265  count. Please re
-00000ce0: 6665 7220 746f 2074 6865 2052 4541 444d  fer to the READM
-00000cf0: 452e 0a20 2020 2020 2020 2020 2020 203c  E..            <
-00000d00: 2f6c 693e 0a20 2020 2020 2020 207b 2520  /li>.        {% 
-00000d10: 656e 6469 6620 257d 0a20 2020 203c 2f75  endif %}.    </u
-00000d20: 6c3e 0a0a 2020 2020 3c68 7220 2f3e 0a0a  l>..    <hr />..
-00000d30: 2020 2020 3c68 333e 5570 6c6f 6164 6564      <h3>Uploaded
-00000d40: 2066 696c 6573 3c2f 6833 3e0a 0a20 2020   files</h3>..   
-00000d50: 207b 2520 6966 2066 696c 6573 2025 7d0a   {% if files %}.
-00000d60: 2020 2020 2020 2020 3c75 6c20 636c 6173          <ul clas
-00000d70: 733d 226c 6973 742d 6772 6f75 7022 3e0a  s="list-group">.
-00000d80: 2020 2020 2020 2020 2020 2020 7b25 2066              {% f
-00000d90: 6f72 2066 696c 655f 6e61 6d65 2c20 6669  or file_name, fi
-00000da0: 6c65 2069 6e20 6669 6c65 732e 6974 656d  le in files.item
-00000db0: 7320 257d 0a20 2020 2020 2020 2020 2020  s %}.           
-00000dc0: 2020 2020 203c 6c69 2063 6c61 7373 3d22       <li class="
-00000dd0: 6c69 7374 2d67 726f 7570 2d69 7465 6d22  list-group-item"
-00000de0: 3e0a 2020 2020 2020 2020 2020 2020 2020  >.              
-00000df0: 2020 2020 2020 3c66 6f72 6d20 6d65 7468        <form meth
-00000e00: 6f64 3d22 706f 7374 2220 636c 6173 733d  od="post" class=
-00000e10: 2270 756c 6c2d 7269 6768 7422 3e0a 2020  "pull-right">.  
+00000110: 0a3c 2f68 6561 643e 0a0a 3c62 6f64 793e  .</head>..<body>
+00000120: 0a3c 6469 7620 636c 6173 733d 2263 6f6e  .<div class="con
+00000130: 7461 696e 6572 223e 0a20 2020 203c 6831  tainer">.    <h1
+00000140: 3e45 7374 6569 6420 5465 7374 2070 6167  >Esteid Test pag
+00000150: 653c 2f68 313e 0a20 2020 203c 7020 7374  e</h1>.    <p st
+00000160: 796c 653d 2266 6f6e 742d 7369 7a65 3a20  yle="font-size: 
+00000170: 782d 6c61 7267 6522 3e0a 2020 2020 2020  x-large">.      
+00000180: 2020 3c62 3e54 6869 7320 7465 7374 2070    <b>This test p
+00000190: 6167 6520 7573 6573 2074 6865 2064 6570  age uses the dep
+000001a0: 7265 6361 7465 6420 6163 7469 6f6e 7320  recated actions 
+000001b0: 4150 492e 2054 6f20 7465 7374 2074 6865  API. To test the
+000001c0: 206e 6577 2041 5049 2c0a 2020 2020 2020   new API,.      
+000001d0: 2020 2020 2020 3c61 2068 7265 663d 227b        <a href="{
+000001e0: 2520 7572 6c20 2773 6b5f 7465 7374 5f6e  % url 'sk_test_n
+000001f0: 6577 2720 257d 223e 706c 6561 7365 2067  ew' %}">please g
+00000200: 6f20 746f 2074 6869 7320 7061 6765 213c  o to this page!<
+00000210: 2f61 3e3c 2f62 3e0a 2020 2020 3c2f 703e  /a></b>.    </p>
+00000220: 0a20 2020 203c 703e 0a20 2020 2020 2020  .    <p>.       
+00000230: 2054 6869 7320 6973 2061 2074 6573 7420   This is a test 
+00000240: 7061 6765 2066 6f72 2064 6967 6974 616c  page for digital
+00000250: 2073 6967 6e69 6e67 206f 6620 6669 6c65   signing of file
+00000260: 7320 7669 6120 7079 7468 6f6e 2e0a 2020  s via python..  
+00000270: 2020 3c2f 703e 0a0a 2020 2020 3c75 6c3e    </p>..    <ul>
+00000280: 0a20 2020 2020 2020 203c 6c69 3e0a 2020  .        <li>.  
+00000290: 2020 2020 2020 2020 2020 4d6f 6269 6c65            Mobile
+000002a0: 2049 4420 7369 676e 696e 6720 6973 2064   ID signing is d
+000002b0: 6f6e 6520 7769 7468 2044 656d 6f20 4d6f  one with Demo Mo
+000002c0: 6269 6c65 2049 4420 7365 7276 6963 652c  bile ID service,
+000002d0: 2079 6f75 2063 616e 206f 6e6c 7920 7573   you can only us
+000002e0: 6520 7468 650a 2020 2020 2020 2020 2020  e the.          
+000002f0: 2020 3c61 2068 7265 663d 2268 7474 7073    <a href="https
+00000300: 3a2f 2f67 6974 6875 622e 636f 6d2f 534b  ://github.com/SK
+00000310: 2d45 4944 2f4d 4944 2f77 696b 692f 5465  -EID/MID/wiki/Te
+00000320: 7374 2d6e 756d 6265 722d 666f 722d 6175  st-number-for-au
+00000330: 746f 6d61 7465 642d 7465 7374 696e 672d  tomated-testing-
+00000340: 696e 2d44 454d 4f22 2074 6172 6765 743d  in-DEMO" target=
+00000350: 225f 626c 616e 6b22 3e64 656d 6f0a 2020  "_blank">demo.  
+00000360: 2020 2020 2020 2020 2020 2020 2020 7465                te
+00000370: 7374 206e 756d 6265 7273 3c2f 613e 2e0a  st numbers</a>..
+00000380: 2020 2020 2020 2020 2020 2020 5468 6520              The 
+00000390: 7369 676e 6174 7572 6573 2077 696c 6c20  signatures will 
+000003a0: 6e6f 7420 6265 2076 616c 6964 2075 6e6c  not be valid unl
+000003b0: 6573 7320 7468 6520 7465 7374 2063 6572  ess the test cer
+000003c0: 7469 6669 6361 7465 7320 6172 6520 7573  tificates are us
+000003d0: 6564 2074 6f20 7661 6c69 6461 7465 2074  ed to validate t
+000003e0: 6865 6d2e 0a20 2020 2020 2020 203c 2f6c  hem..        </l
+000003f0: 693e 0a20 2020 2020 2020 203c 6c69 3e0a  i>.        <li>.
+00000400: 2020 2020 2020 2020 2020 2020 4944 2043              ID C
+00000410: 6172 6420 7369 676e 696e 6720 6361 6e20  ard signing can 
+00000420: 6265 2064 6f6e 6520 7769 7468 2072 6561  be done with rea
+00000430: 6c20 4944 2063 6172 6473 2c20 6275 7420  l ID cards, but 
+00000440: 7375 6368 2061 2073 6967 6e61 7475 7265  such a signature
+00000450: 2063 616e 206e 6f74 2062 6520 7661 6c69   can not be vali
+00000460: 6461 7465 642e 0a20 2020 2020 2020 203c  dated..        <
+00000470: 2f6c 693e 0a20 2020 2020 2020 203c 6c69  /li>.        <li
+00000480: 3e0a 2020 2020 2020 2020 2020 2020 4944  >.            ID
+00000490: 2043 6172 6420 7369 676e 696e 6720 7265   Card signing re
+000004a0: 7175 6972 6573 2074 6865 2063 6872 6f6d  quires the chrom
+000004b0: 652d 746f 6b65 6e2d 7369 676e 696e 6720  e-token-signing 
+000004c0: 666f 7220 6368 726f 6d65 206f 7220 6669  for chrome or fi
+000004d0: 7265 666f 782e 0a20 2020 2020 2020 203c  refox..        <
+000004e0: 2f6c 693e 0a20 2020 2020 2020 203c 6c69  /li>.        <li
+000004f0: 3e0a 2020 2020 2020 2020 2020 2020 4944  >.            ID
+00000500: 2043 6172 6420 7369 676e 696e 6720 7265   Card signing re
+00000510: 7175 6972 6573 2048 5454 5053 2e20 506c  quires HTTPS. Pl
+00000520: 6561 7365 2072 6566 6572 2074 6f20 7468  ease refer to th
+00000530: 6520 5245 4144 4d45 2e0a 2020 2020 2020  e README..      
+00000540: 2020 3c2f 6c69 3e0a 2020 2020 2020 2020    </li>.        
+00000550: 3c6c 693e 0a20 2020 2020 2020 2020 2020  <li>.           
+00000560: 2053 6967 6e69 6e67 2077 6974 6820 536d   Signing with Sm
+00000570: 6172 7449 4420 7265 7175 6972 6573 2073  artID requires s
+00000580: 6574 7469 6e67 2075 7020 6120 6465 6d6f  etting up a demo
+00000590: 2053 6d61 7274 4944 2061 6363 6f75 6e74   SmartID account
+000005a0: 2e20 506c 6561 7365 2072 6566 6572 2074  . Please refer t
+000005b0: 6f20 7468 6520 5245 4144 4d45 2e0a 2020  o the README..  
+000005c0: 2020 2020 2020 3c2f 6c69 3e0a 2020 2020        </li>.    
+000005d0: 3c2f 756c 3e0a 0a20 2020 203c 6872 202f  </ul>..    <hr /
+000005e0: 3e0a 0a20 2020 203c 6833 3e55 706c 6f61  >..    <h3>Uploa
+000005f0: 6465 6420 6669 6c65 733c 2f68 333e 0a0a  ded files</h3>..
+00000600: 2020 2020 7b25 2069 6620 6669 6c65 7320      {% if files 
+00000610: 257d 0a20 2020 2020 2020 203c 756c 2063  %}.        <ul c
+00000620: 6c61 7373 3d22 6c69 7374 2d67 726f 7570  lass="list-group
+00000630: 223e 0a20 2020 2020 2020 2020 2020 207b  ">.            {
+00000640: 2520 666f 7220 6669 6c65 5f6e 616d 652c  % for file_name,
+00000650: 2066 696c 6520 696e 2066 696c 6573 2e69   file in files.i
+00000660: 7465 6d73 2025 7d0a 2020 2020 2020 2020  tems %}.        
+00000670: 2020 2020 2020 2020 3c6c 6920 636c 6173          <li clas
+00000680: 733d 226c 6973 742d 6772 6f75 702d 6974  s="list-group-it
+00000690: 656d 223e 0a20 2020 2020 2020 2020 2020  em">.           
+000006a0: 2020 2020 2020 2020 203c 666f 726d 206d           <form m
+000006b0: 6574 686f 643d 2270 6f73 7422 2063 6c61  ethod="post" cla
+000006c0: 7373 3d22 7075 6c6c 2d72 6967 6874 223e  ss="pull-right">
+000006d0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000006e0: 2020 2020 2020 2020 207b 2520 6373 7266           {% csrf
+000006f0: 5f74 6f6b 656e 2025 7d0a 0a20 2020 2020  _token %}..     
+00000700: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000710: 2020 203c 696e 7075 7420 6e61 6d65 3d22     <input name="
+00000720: 6163 7469 6f6e 2220 7479 7065 3d22 6869  action" type="hi
+00000730: 6464 656e 2220 7661 6c75 653d 2272 656d  dden" value="rem
+00000740: 6f76 655f 6669 6c65 2220 2f3e 0a20 2020  ove_file" />.   
+00000750: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000760: 2020 2020 203c 696e 7075 7420 6e61 6d65       <input name
+00000770: 3d22 6669 6c65 5f6e 616d 6522 2074 7970  ="file_name" typ
+00000780: 653d 2268 6964 6465 6e22 2076 616c 7565  e="hidden" value
+00000790: 3d22 7b7b 2066 696c 655f 6e61 6d65 207d  ="{{ file_name }
+000007a0: 7d22 202f 3e0a 0a20 2020 2020 2020 2020  }" />..         
+000007b0: 2020 2020 2020 2020 2020 2020 2020 203c                 <
+000007c0: 696e 7075 7420 7479 7065 3d22 7375 626d  input type="subm
+000007d0: 6974 2220 636c 6173 733d 2262 746e 2062  it" class="btn b
+000007e0: 746e 2d78 7320 6274 6e2d 6461 6e67 6572  tn-xs btn-danger
+000007f0: 2220 7661 6c75 653d 2258 2220 2f3e 0a20  " value="X" />. 
+00000800: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000810: 2020 203c 2f66 6f72 6d3e 0a20 2020 2020     </form>.     
+00000820: 2020 2020 2020 2020 2020 2020 2020 203c                 <
+00000830: 7370 616e 2063 6c61 7373 3d22 6261 6467  span class="badg
+00000840: 6522 3e7b 7b20 6669 6c65 2e73 697a 6520  e">{{ file.size 
+00000850: 7d7d 2062 7974 6573 3c2f 7370 616e 3e0a  }} bytes</span>.
+00000860: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00000870: 2020 2020 207b 7b20 6669 6c65 5f6e 616d       {{ file_nam
+00000880: 6520 7d7d 0a20 2020 2020 2020 2020 2020  e }}.           
+00000890: 2020 2020 203c 2f6c 693e 0a20 2020 2020       </li>.     
+000008a0: 2020 2020 2020 207b 2520 656e 6466 6f72         {% endfor
+000008b0: 2025 7d0a 2020 2020 2020 2020 3c2f 756c   %}.        </ul
+000008c0: 3e0a 0a20 2020 2020 2020 203c 6872 202f  >..        <hr /
+000008d0: 3e0a 0a20 2020 2020 2020 203c 6833 3e53  >..        <h3>S
+000008e0: 6967 6e20 7468 6520 6669 6c65 733c 2f68  ign the files</h
+000008f0: 333e 0a0a 2020 2020 2020 2020 3c61 2068  3>..        <a h
+00000900: 7265 663d 2223 2220 6964 3d22 7369 676e  ref="#" id="sign
+00000910: 2d69 6422 3e3c 696d 6720 616c 743d 2249  -id"><img alt="I
+00000920: 4420 4361 7264 2220 7372 633d 227b 2520  D Card" src="{% 
+00000930: 7374 6174 6963 2027 696d 6167 6573 2f65  static 'images/e
+00000940: 7374 6569 642f 6964 2d6b 6161 7274 2d6c  steid/id-kaart-l
+00000950: 6f67 6f2e 6769 6627 2025 7d22 3e3c 2f61  ogo.gif' %}"></a
+00000960: 3e0a 2020 2020 2020 2020 3c61 2068 7265  >.        <a hre
+00000970: 663d 2223 2220 6964 3d22 7369 676e 2d6d  f="#" id="sign-m
+00000980: 6964 223e 3c69 6d67 2061 6c74 3d22 4d6f  id"><img alt="Mo
+00000990: 6269 6c65 2049 4422 2073 7263 3d22 7b25  bile ID" src="{%
+000009a0: 2073 7461 7469 6320 2769 6d61 6765 732f   static 'images/
+000009b0: 6573 7465 6964 2f6d 6964 2d6c 6f67 6f2e  esteid/mid-logo.
+000009c0: 6769 6627 2025 7d22 3e3c 2f61 3e0a 2020  gif' %}"></a>.  
+000009d0: 2020 2020 2020 3c61 2068 7265 663d 2223        <a href="#
+000009e0: 2220 6964 3d22 7369 676e 2d73 6d61 7274  " id="sign-smart
+000009f0: 6964 223e 3c69 6d67 2061 6c74 3d22 536d  id"><img alt="Sm
+00000a00: 6172 7420 4944 2220 7372 633d 227b 2520  art ID" src="{% 
+00000a10: 7374 6174 6963 2027 696d 6167 6573 2f65  static 'images/e
+00000a20: 7374 6569 642f 736d 6172 7449 442d 6c6f  steid/smartID-lo
+00000a30: 676f 2d62 746e 2e70 6e67 2720 257d 223e  go-btn.png' %}">
+00000a40: 3c2f 613e 0a0a 2020 2020 7b25 2065 6c73  </a>..    {% els
+00000a50: 6520 257d 0a20 2020 2020 2020 203c 703e  e %}.        <p>
+00000a60: 4e6f 2066 696c 6573 2075 706c 6f61 6465  No files uploade
+00000a70: 642c 2074 6f20 6265 6769 6e20 7468 6520  d, to begin the 
+00000a80: 7369 676e 696e 6720 7072 6f63 6573 732c  signing process,
+00000a90: 2070 6c65 6173 6520 7570 6c6f 6164 2073   please upload s
+00000aa0: 6f6d 6520 6669 6c65 733c 2f70 3e0a 2020  ome files</p>.  
+00000ab0: 2020 7b25 2065 6e64 6966 2025 7d0a 0a20    {% endif %}.. 
+00000ac0: 2020 203c 6872 202f 3e0a 0a20 2020 203c     <hr />..    <
+00000ad0: 6832 3e55 706c 6f61 6420 6669 6c65 733c  h2>Upload files<
+00000ae0: 2f68 323e 0a20 2020 203c 666f 726d 206d  /h2>.    <form m
+00000af0: 6574 686f 643d 2250 4f53 5422 2065 6e63  ethod="POST" enc
+00000b00: 7479 7065 3d22 6d75 6c74 6970 6172 742f  type="multipart/
+00000b10: 666f 726d 2d64 6174 6122 3e0a 2020 2020  form-data">.    
+00000b20: 2020 2020 7b25 2063 7372 665f 746f 6b65      {% csrf_toke
+00000b30: 6e20 257d 0a0a 2020 2020 2020 2020 3c64  n %}..        <d
+00000b40: 6976 2063 6c61 7373 3d22 666f 726d 2d67  iv class="form-g
+00000b50: 726f 7570 223e 0a20 2020 2020 2020 2020  roup">.         
+00000b60: 2020 203c 6c61 6265 6c20 666f 723d 2265     <label for="e
+00000b70: 7861 6d70 6c65 496e 7075 7446 696c 6522  xampleInputFile"
+00000b80: 3e53 656c 6563 7420 6669 6c65 3c2f 6c61  >Select file</la
+00000b90: 6265 6c3e 0a20 2020 2020 2020 2020 2020  bel>.           
+00000ba0: 203c 696e 7075 7420 7479 7065 3d22 6669   <input type="fi
+00000bb0: 6c65 2220 6964 3d22 6578 616d 706c 6549  le" id="exampleI
+00000bc0: 6e70 7574 4669 6c65 2220 6e61 6d65 3d22  nputFile" name="
+00000bd0: 7468 655f 6669 6c65 223e 0a20 2020 2020  the_file">.     
+00000be0: 2020 203c 2f64 6976 3e0a 0a20 2020 2020     </div>..     
+00000bf0: 2020 203c 6275 7474 6f6e 2074 7970 653d     <button type=
+00000c00: 2273 7562 6d69 7422 2063 6c61 7373 3d22  "submit" class="
+00000c10: 6274 6e20 6274 6e2d 6465 6661 756c 7422  btn btn-default"
+00000c20: 3e53 7562 6d69 743c 2f62 7574 746f 6e3e  >Submit</button>
+00000c30: 0a0a 2020 2020 3c2f 666f 726d 3e0a 3c2f  ..    </form>.</
+00000c40: 6469 763e 0a0a 3c64 6976 2063 6c61 7373  div>..<div class
+00000c50: 3d22 6d6f 6461 6c20 6661 6465 2220 6964  ="modal fade" id
+00000c60: 3d22 6d69 642d 6d6f 6461 6c22 3e0a 2020  ="mid-modal">.  
+00000c70: 2020 3c64 6976 2063 6c61 7373 3d22 6d6f    <div class="mo
+00000c80: 6461 6c2d 6469 616c 6f67 223e 0a20 2020  dal-dialog">.   
+00000c90: 2020 2020 203c 6469 7620 636c 6173 733d       <div class=
+00000ca0: 226d 6f64 616c 2d63 6f6e 7465 6e74 223e  "modal-content">
+00000cb0: 0a20 2020 2020 2020 2020 2020 203c 6469  .            <di
+00000cc0: 7620 636c 6173 733d 226d 6f64 616c 2d68  v class="modal-h
+00000cd0: 6561 6465 7222 3e0a 2020 2020 2020 2020  eader">.        
+00000ce0: 2020 2020 2020 2020 3c62 7574 746f 6e20          <button 
+00000cf0: 7479 7065 3d22 6275 7474 6f6e 2220 636c  type="button" cl
+00000d00: 6173 733d 2263 6c6f 7365 2220 6461 7461  ass="close" data
+00000d10: 2d64 6973 6d69 7373 3d22 6d6f 6461 6c22  -dismiss="modal"
+00000d20: 2061 7269 612d 6c61 6265 6c3d 2243 6c6f   aria-label="Clo
+00000d30: 7365 223e 3c73 7061 6e20 6172 6961 2d68  se"><span aria-h
+00000d40: 6964 6465 6e3d 2274 7275 6522 3e26 7469  idden="true">&ti
+00000d50: 6d65 733b 3c2f 7370 616e 3e0a 2020 2020  mes;</span>.    
+00000d60: 2020 2020 2020 2020 2020 2020 3c2f 6275              </bu
+00000d70: 7474 6f6e 3e0a 2020 2020 2020 2020 2020  tton>.          
+00000d80: 2020 2020 2020 3c68 3420 636c 6173 733d        <h4 class=
+00000d90: 226d 6f64 616c 2d74 6974 6c65 223e 5369  "modal-title">Si
+00000da0: 676e 2074 6865 2066 696c 6573 2077 6974  gn the files wit
+00000db0: 6820 4d6f 6269 6c65 4944 3c2f 6834 3e0a  h MobileID</h4>.
+00000dc0: 2020 2020 2020 2020 2020 2020 3c2f 6469              </di
+00000dd0: 763e 0a0a 2020 2020 2020 2020 2020 2020  v>..            
+00000de0: 3c64 6976 2063 6c61 7373 3d22 6d6f 6461  <div class="moda
+00000df0: 6c2d 626f 6479 223e 0a20 2020 2020 2020  l-body">.       
+00000e00: 2020 2020 2020 2020 203c 666f 726d 206e           <form n
+00000e10: 616d 653d 226d 6f62 696c 6549 6422 3e0a  ame="mobileId">.
 00000e20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000e30: 2020 2020 2020 7b25 2063 7372 665f 746f        {% csrf_to
-00000e40: 6b65 6e20 257d 0a0a 2020 2020 2020 2020  ken %}..        
+00000e30: 2020 2020 3c64 6976 2063 6c61 7373 3d22      <div class="
+00000e40: 666f 726d 2d67 726f 7570 223e 0a20 2020  form-group">.   
 00000e50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000e60: 3c69 6e70 7574 206e 616d 653d 2261 6374  <input name="act
-00000e70: 696f 6e22 2074 7970 653d 2268 6964 6465  ion" type="hidde
-00000e80: 6e22 2076 616c 7565 3d22 7265 6d6f 7665  n" value="remove
-00000e90: 5f66 696c 6522 202f 3e0a 2020 2020 2020  _file" />.      
-00000ea0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000eb0: 2020 3c69 6e70 7574 206e 616d 653d 2266    <input name="f
-00000ec0: 696c 655f 6e61 6d65 2220 7479 7065 3d22  ile_name" type="
-00000ed0: 6869 6464 656e 2220 7661 6c75 653d 227b  hidden" value="{
-00000ee0: 7b20 6669 6c65 5f6e 616d 6520 7d7d 2220  { file_name }}" 
-00000ef0: 2f3e 0a0a 2020 2020 2020 2020 2020 2020  />..            
-00000f00: 2020 2020 2020 2020 2020 2020 3c69 6e70              <inp
-00000f10: 7574 2074 7970 653d 2273 7562 6d69 7422  ut type="submit"
-00000f20: 2063 6c61 7373 3d22 6274 6e20 6274 6e2d   class="btn btn-
-00000f30: 7873 2062 746e 2d64 616e 6765 7222 2076  xs btn-danger" v
-00000f40: 616c 7565 3d22 5822 202f 3e0a 2020 2020  alue="X" />.    
-00000f50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000f60: 3c2f 666f 726d 3e0a 2020 2020 2020 2020  </form>.        
-00000f70: 2020 2020 2020 2020 2020 2020 3c73 7061              <spa
-00000f80: 6e20 636c 6173 733d 2262 6164 6765 223e  n class="badge">
-00000f90: 7b7b 2066 696c 652e 7369 7a65 207d 7d20  {{ file.size }} 
-00000fa0: 6279 7465 733c 2f73 7061 6e3e 0a0a 2020  bytes</span>..  
+00000e60: 2020 2020 203c 6c61 6265 6c20 666f 723d       <label for=
+00000e70: 2270 686f 6e65 4e72 496e 7075 7422 3e44  "phoneNrInput">D
+00000e80: 656d 6f20 5068 6f6e 6520 6e72 3a3c 2f6c  emo Phone nr:</l
+00000e90: 6162 656c 3e0a 2020 2020 2020 2020 2020  abel>.          
+00000ea0: 2020 2020 2020 2020 2020 2020 2020 3c69                <i
+00000eb0: 6e70 7574 2074 7970 653d 2274 6578 7422  nput type="text"
+00000ec0: 206e 616d 653d 2270 686f 6e65 5f6e 7222   name="phone_nr"
+00000ed0: 2069 643d 2270 686f 6e65 4e72 496e 7075   id="phoneNrInpu
+00000ee0: 7422 2063 6c61 7373 3d22 666f 726d 2d63  t" class="form-c
+00000ef0: 6f6e 7472 6f6c 220a 2020 2020 2020 2020  ontrol".        
+00000f00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000f10: 2020 2020 2020 2076 616c 7565 3d22 7b7b         value="{{
+00000f20: 2072 6571 7565 7374 2e73 6573 7369 6f6e   request.session
+00000f30: 2e64 646f 635f 7465 7374 5f70 686f 6e65  .ddoc_test_phone
+00000f40: 5f6e 756d 6265 7220 7c20 6465 6661 756c  _number | defaul
+00000f50: 743a 272b 3337 3230 3030 3030 3736 3627  t:'+37200000766'
+00000f60: 207d 7d22 202f 3e0a 2020 2020 2020 2020   }}" />.        
+00000f70: 2020 2020 2020 2020 2020 2020 3c2f 6469              </di
+00000f80: 763e 0a20 2020 2020 2020 2020 2020 2020  v>.             
+00000f90: 2020 2020 2020 203c 6469 7620 636c 6173         <div clas
+00000fa0: 733d 2266 6f72 6d2d 6772 6f75 7022 3e0a  s="form-group">.
 00000fb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000fc0: 2020 7b7b 2066 696c 655f 6e61 6d65 207d    {{ file_name }
-00000fd0: 7d0a 2020 2020 2020 2020 2020 2020 2020  }.              
-00000fe0: 2020 3c2f 6c69 3e0a 2020 2020 2020 2020    </li>.        
-00000ff0: 2020 2020 7b25 2065 6e64 666f 7220 257d      {% endfor %}
-00001000: 0a20 2020 2020 2020 203c 2f75 6c3e 0a0a  .        </ul>..
-00001010: 2020 2020 2020 2020 3c68 7220 2f3e 0a0a          <hr />..
-00001020: 2020 2020 2020 2020 3c68 333e 5369 676e          <h3>Sign
-00001030: 2074 6865 2066 696c 6573 3c2f 6833 3e0a   the files</h3>.
-00001040: 0a20 2020 2020 2020 207b 2520 6966 2049  .        {% if I
-00001050: 445f 4341 5244 5f45 4e41 424c 4544 2025  D_CARD_ENABLED %
-00001060: 7d0a 2020 2020 2020 2020 2020 2020 3c61  }.            <a
-00001070: 2068 7265 663d 2223 2220 6964 3d22 7369   href="#" id="si
-00001080: 676e 2d69 6422 3e3c 696d 6720 616c 743d  gn-id"><img alt=
-00001090: 2249 4420 4361 7264 2220 7372 633d 227b  "ID Card" src="{
-000010a0: 2520 7374 6174 6963 2027 696d 6167 6573  % static 'images
-000010b0: 2f65 7374 6569 642f 6964 2d6b 6161 7274  /esteid/id-kaart
-000010c0: 2d6c 6f67 6f2e 6769 6627 2025 7d22 3e3c  -logo.gif' %}"><
-000010d0: 2f61 3e0a 2020 2020 2020 2020 7b25 2065  /a>.        {% e
-000010e0: 6e64 6966 2025 7d0a 2020 2020 2020 2020  ndif %}.        
-000010f0: 7b25 2069 6620 4d4f 4249 4c45 5f49 445f  {% if MOBILE_ID_
-00001100: 454e 4142 4c45 4420 257d 0a20 2020 2020  ENABLED %}.     
-00001110: 2020 2020 2020 203c 6120 6872 6566 3d22         <a href="
-00001120: 2322 2069 643d 2273 6967 6e2d 6d69 6422  #" id="sign-mid"
-00001130: 3e3c 696d 6720 616c 743d 224d 6f62 696c  ><img alt="Mobil
-00001140: 6520 4944 2220 7372 633d 227b 2520 7374  e ID" src="{% st
-00001150: 6174 6963 2027 696d 6167 6573 2f65 7374  atic 'images/est
-00001160: 6569 642f 6d69 642d 6c6f 676f 2e67 6966  eid/mid-logo.gif
-00001170: 2720 257d 223e 3c2f 613e 0a20 2020 2020  ' %}"></a>.     
-00001180: 2020 207b 2520 656e 6469 6620 257d 0a20     {% endif %}. 
-00001190: 2020 2020 2020 207b 2520 6966 2053 4d41         {% if SMA
-000011a0: 5254 5f49 445f 454e 4142 4c45 4420 257d  RT_ID_ENABLED %}
-000011b0: 0a20 2020 2020 2020 2020 2020 203c 6120  .            <a 
-000011c0: 6872 6566 3d22 2322 2069 643d 2273 6967  href="#" id="sig
-000011d0: 6e2d 736d 6172 7469 6422 3e3c 696d 6720  n-smartid"><img 
-000011e0: 616c 743d 2253 6d61 7274 2049 4422 0a20  alt="Smart ID". 
-000011f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001200: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001210: 2020 2020 2020 2020 2020 2020 2020 7372                sr
-00001220: 633d 227b 2520 7374 6174 6963 2027 696d  c="{% static 'im
-00001230: 6167 6573 2f65 7374 6569 642f 736d 6172  ages/esteid/smar
-00001240: 7449 442d 6c6f 676f 2d62 746e 2e70 6e67  tID-logo-btn.png
-00001250: 2720 257d 223e 3c2f 613e 0a20 2020 2020  ' %}"></a>.     
-00001260: 2020 207b 2520 656e 6469 6620 257d 0a0a     {% endif %}..
-00001270: 2020 2020 7b25 2065 6c73 6520 257d 0a20      {% else %}. 
-00001280: 2020 2020 2020 203c 703e 4e6f 2066 696c         <p>No fil
-00001290: 6573 2075 706c 6f61 6465 642c 2074 6f20  es uploaded, to 
-000012a0: 6265 6769 6e20 7468 6520 7369 676e 696e  begin the signin
-000012b0: 6720 7072 6f63 6573 732c 2070 6c65 6173  g process, pleas
-000012c0: 6520 7570 6c6f 6164 2073 6f6d 6520 6669  e upload some fi
-000012d0: 6c65 733c 2f70 3e0a 2020 2020 7b25 2065  les</p>.    {% e
-000012e0: 6e64 6966 2025 7d0a 0a20 2020 203c 6872  ndif %}..    <hr
-000012f0: 202f 3e0a 0a20 2020 203c 6832 3e55 706c   />..    <h2>Upl
-00001300: 6f61 6420 6669 6c65 733c 2f68 323e 0a20  oad files</h2>. 
-00001310: 2020 203c 666f 726d 206d 6574 686f 643d     <form method=
-00001320: 2250 4f53 5422 2065 6e63 7479 7065 3d22  "POST" enctype="
-00001330: 6d75 6c74 6970 6172 742f 666f 726d 2d64  multipart/form-d
-00001340: 6174 6122 3e0a 2020 2020 2020 2020 7b25  ata">.        {%
-00001350: 2063 7372 665f 746f 6b65 6e20 257d 0a0a   csrf_token %}..
-00001360: 2020 2020 2020 2020 3c64 6976 2063 6c61          <div cla
-00001370: 7373 3d22 666f 726d 2d67 726f 7570 223e  ss="form-group">
-00001380: 0a20 2020 2020 2020 2020 2020 203c 6c61  .            <la
-00001390: 6265 6c20 666f 723d 2265 7861 6d70 6c65  bel for="example
-000013a0: 496e 7075 7446 696c 6522 3e53 656c 6563  InputFile">Selec
-000013b0: 7420 6669 6c65 3c2f 6c61 6265 6c3e 0a20  t file</label>. 
-000013c0: 2020 2020 2020 2020 2020 203c 696e 7075             <inpu
-000013d0: 7420 7479 7065 3d22 6669 6c65 2220 6964  t type="file" id
-000013e0: 3d22 6578 616d 706c 6549 6e70 7574 4669  ="exampleInputFi
-000013f0: 6c65 2220 6e61 6d65 3d22 7468 655f 6669  le" name="the_fi
-00001400: 6c65 223e 0a20 2020 2020 2020 203c 2f64  le">.        </d
-00001410: 6976 3e0a 0a20 2020 2020 2020 203c 6275  iv>..        <bu
-00001420: 7474 6f6e 2074 7970 653d 2273 7562 6d69  tton type="submi
-00001430: 7422 2063 6c61 7373 3d22 6274 6e20 6274  t" class="btn bt
-00001440: 6e2d 6465 6661 756c 7422 3e53 7562 6d69  n-default">Submi
-00001450: 743c 2f62 7574 746f 6e3e 0a0a 2020 2020  t</button>..    
-00001460: 3c2f 666f 726d 3e0a 3c2f 6469 763e 0a0a  </form>.</div>..
-00001470: 3c64 6976 2063 6c61 7373 3d22 6d6f 6461  <div class="moda
-00001480: 6c20 6661 6465 2220 6964 3d22 6d69 642d  l fade" id="mid-
-00001490: 6d6f 6461 6c22 3e0a 2020 2020 3c64 6976  modal">.    <div
-000014a0: 2063 6c61 7373 3d22 6d6f 6461 6c2d 6469   class="modal-di
-000014b0: 616c 6f67 223e 0a20 2020 2020 2020 203c  alog">.        <
-000014c0: 666f 726d 206e 616d 653d 226d 6f62 696c  form name="mobil
-000014d0: 6549 6422 3e0a 2020 2020 2020 2020 2020  eId">.          
-000014e0: 2020 3c64 6976 2063 6c61 7373 3d22 6d6f    <div class="mo
-000014f0: 6461 6c2d 636f 6e74 656e 7422 3e0a 2020  dal-content">.  
-00001500: 2020 2020 2020 2020 2020 2020 2020 3c64                <d
-00001510: 6976 2063 6c61 7373 3d22 6d6f 6461 6c2d  iv class="modal-
-00001520: 6865 6164 6572 223e 0a20 2020 2020 2020  header">.       
-00001530: 2020 2020 2020 2020 2020 2020 203c 6275               <bu
-00001540: 7474 6f6e 2074 7970 653d 2262 7574 746f  tton type="butto
-00001550: 6e22 2063 6c61 7373 3d22 636c 6f73 6522  n" class="close"
-00001560: 2064 6174 612d 6469 736d 6973 733d 226d   data-dismiss="m
-00001570: 6f64 616c 2220 6172 6961 2d6c 6162 656c  odal" aria-label
-00001580: 3d22 436c 6f73 6522 3e3c 7370 616e 0a20  ="Close"><span. 
-00001590: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000015a0: 2020 2020 2020 2020 2020 2061 7269 612d             aria-
-000015b0: 6869 6464 656e 3d22 7472 7565 223e 2674  hidden="true">&t
-000015c0: 696d 6573 3b3c 2f73 7061 6e3e 0a20 2020  imes;</span>.   
-000015d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000015e0: 203c 2f62 7574 746f 6e3e 0a20 2020 2020   </button>.     
-000015f0: 2020 2020 2020 2020 2020 2020 2020 203c                 <
-00001600: 6834 2063 6c61 7373 3d22 6d6f 6461 6c2d  h4 class="modal-
-00001610: 7469 746c 6522 3e53 6967 6e20 7468 6520  title">Sign the 
-00001620: 6669 6c65 7320 7769 7468 204d 6f62 696c  files with Mobil
-00001630: 6549 443c 2f68 343e 0a20 2020 2020 2020  eID</h4>.       
-00001640: 2020 2020 2020 2020 203c 2f64 6976 3e0a           </div>.
-00001650: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00001660: 203c 6469 7620 636c 6173 733d 226d 6f64   <div class="mod
-00001670: 616c 2d62 6f64 7922 3e0a 2020 2020 2020  al-body">.      
-00001680: 2020 2020 2020 2020 2020 2020 2020 3c64                <d
-00001690: 6976 2063 6c61 7373 3d22 666f 726d 2d67  iv class="form-g
-000016a0: 726f 7570 223e 0a20 2020 2020 2020 2020  roup">.         
-000016b0: 2020 2020 2020 2020 2020 2020 2020 203c                 <
-000016c0: 6c61 6265 6c20 666f 723d 2270 686f 6e65  label for="phone
-000016d0: 4e72 496e 7075 7422 3e44 656d 6f20 5068  NrInput">Demo Ph
-000016e0: 6f6e 6520 6e72 3a3c 2f6c 6162 656c 3e0a  one nr:</label>.
-000016f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001700: 2020 2020 2020 2020 3c69 6e70 7574 2074          <input t
-00001710: 7970 653d 2274 6578 7422 206e 616d 653d  ype="text" name=
-00001720: 2270 686f 6e65 5f6e 7222 2069 643d 2270  "phone_nr" id="p
-00001730: 686f 6e65 4e72 496e 7075 7422 2063 6c61  honeNrInput" cla
-00001740: 7373 3d22 666f 726d 2d63 6f6e 7472 6f6c  ss="form-control
-00001750: 220a 2020 2020 2020 2020 2020 2020 2020  ".              
-00001760: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001770: 2076 616c 7565 3d22 7b7b 2072 6571 7565   value="{{ reque
-00001780: 7374 2e73 6573 7369 6f6e 2e64 646f 635f  st.session.ddoc_
-00001790: 7465 7374 5f70 686f 6e65 5f6e 756d 6265  test_phone_numbe
-000017a0: 7220 7c20 6465 6661 756c 743a 272b 3337  r | default:'+37
-000017b0: 3230 3030 3030 3736 3627 207d 7d22 202f  200000766' }}" /
-000017c0: 3e0a 2020 2020 2020 2020 2020 2020 2020  >.              
-000017d0: 2020 2020 2020 3c2f 6469 763e 0a20 2020        </div>.   
-000017e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000017f0: 203c 6469 7620 636c 6173 733d 2266 6f72   <div class="for
-00001800: 6d2d 6772 6f75 7022 3e0a 2020 2020 2020  m-group">.      
-00001810: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001820: 2020 3c6c 6162 656c 2066 6f72 3d22 6964    <label for="id
-00001830: 436f 6465 496e 7075 7422 3e44 656d 6f20  CodeInput">Demo 
-00001840: 4944 2063 6f64 653a 3c2f 6c61 6265 6c3e  ID code:</label>
-00001850: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00001860: 2020 2020 2020 2020 203c 696e 7075 7420           <input 
-00001870: 7479 7065 3d22 7465 7874 2220 6e61 6d65  type="text" name
-00001880: 3d22 6964 5f63 6f64 6522 2069 643d 2269  ="id_code" id="i
-00001890: 6443 6f64 6549 6e70 7574 2220 636c 6173  dCodeInput" clas
-000018a0: 733d 2266 6f72 6d2d 636f 6e74 726f 6c22  s="form-control"
-000018b0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000018c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000018d0: 7661 6c75 653d 227b 7b20 7265 7175 6573  value="{{ reques
-000018e0: 742e 7365 7373 696f 6e2e 6464 6f63 5f74  t.session.ddoc_t
-000018f0: 6573 745f 6964 5f63 6f64 6520 7c20 6465  est_id_code | de
-00001900: 6661 756c 743a 2736 3030 3031 3031 3939  fault:'600010199
-00001910: 3036 2720 7d7d 2220 2f3e 0a20 2020 2020  06' }}" />.     
-00001920: 2020 2020 2020 2020 2020 2020 2020 203c                 <
-00001930: 2f64 6976 3e0a 2020 2020 2020 2020 2020  /div>.          
-00001940: 2020 2020 2020 3c2f 6469 763e 0a0a 2020        </div>..  
-00001950: 2020 2020 2020 2020 2020 2020 2020 3c64                <d
-00001960: 6976 2063 6c61 7373 3d22 6d6f 6461 6c2d  iv class="modal-
-00001970: 666f 6f74 6572 223e 0a20 2020 2020 2020  footer">.       
-00001980: 2020 2020 2020 2020 2020 2020 203c 6275               <bu
-00001990: 7474 6f6e 2074 7970 653d 2273 7562 6d69  tton type="submi
-000019a0: 7422 2063 6c61 7373 3d22 6274 6e20 6274  t" class="btn bt
-000019b0: 6e2d 7072 696d 6172 7922 3e53 6967 6e3c  n-primary">Sign<
-000019c0: 2f62 7574 746f 6e3e 0a20 2020 2020 2020  /button>.       
-000019d0: 2020 2020 2020 2020 2020 2020 203c 6469               <di
-000019e0: 7620 636c 6173 733d 226c 6473 2d64 7561  v class="lds-dua
-000019f0: 6c2d 7269 6e67 223e 3c2f 6469 763e 0a20  l-ring"></div>. 
-00001a00: 2020 2020 2020 2020 2020 2020 2020 203c                 <
-00001a10: 2f64 6976 3e0a 2020 2020 2020 2020 2020  /div>.          
-00001a20: 2020 3c2f 6469 763e 0a20 2020 2020 2020    </div>.       
-00001a30: 203c 2f66 6f72 6d3e 0a20 2020 203c 2f64   </form>.    </d
-00001a40: 6976 3e0a 3c2f 6469 763e 0a0a 3c64 6976  iv>.</div>..<div
-00001a50: 2063 6c61 7373 3d22 6d6f 6461 6c20 6661   class="modal fa
-00001a60: 6465 2220 6964 3d22 6368 616c 6c65 6e67  de" id="challeng
-00001a70: 652d 6d6f 6461 6c22 3e0a 2020 2020 3c64  e-modal">.    <d
-00001a80: 6976 2063 6c61 7373 3d22 6d6f 6461 6c2d  iv class="modal-
-00001a90: 6469 616c 6f67 223e 0a20 2020 2020 2020  dialog">.       
-00001aa0: 203c 6469 7620 636c 6173 733d 226d 6f64   <div class="mod
-00001ab0: 616c 2d63 6f6e 7465 6e74 223e 0a20 2020  al-content">.   
-00001ac0: 2020 2020 2020 2020 203c 6469 7620 636c           <div cl
-00001ad0: 6173 733d 226d 6f64 616c 2d68 6561 6465  ass="modal-heade
-00001ae0: 7222 3e0a 2020 2020 2020 2020 2020 2020  r">.            
-00001af0: 2020 2020 3c68 3420 636c 6173 733d 226d      <h4 class="m
-00001b00: 6f64 616c 2d74 6974 6c65 223e 4d49 4420  odal-title">MID 
-00001b10: 5374 6570 2032 3c2f 6834 3e0a 2020 2020  Step 2</h4>.    
-00001b20: 2020 2020 2020 2020 3c2f 6469 763e 0a0a          </div>..
-00001b30: 2020 2020 2020 2020 2020 2020 3c64 6976              <div
-00001b40: 2063 6c61 7373 3d22 6d6f 6461 6c2d 626f   class="modal-bo
-00001b50: 6479 223e 0a20 2020 2020 2020 2020 2020  dy">.           
-00001b60: 2020 2020 203c 703e 0a20 2020 2020 2020       <p>.       
-00001b70: 2020 2020 2020 2020 2020 2020 2050 6c65               Ple
-00001b80: 6173 6520 656e 7465 7220 7468 6520 666f  ase enter the fo
-00001b90: 6c6c 6f77 696e 6720 636f 6465 2069 6e74  llowing code int
-00001ba0: 6f20 796f 7572 206d 6f62 696c 6520 746f  o your mobile to
-00001bb0: 2070 726f 6365 6564 2077 6974 680a 2020   proceed with.  
-00001bc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001bd0: 2020 7468 6520 7369 676e 696e 6720 7072    the signing pr
-00001be0: 6f63 6573 733a 203c 6220 6964 3d22 6368  ocess: <b id="ch
-00001bf0: 616c 6c65 6e67 652d 636f 6465 223e 4b4f  allenge-code">KO
-00001c00: 4f44 3c2f 623e 0a20 2020 2020 2020 2020  OD</b>.         
-00001c10: 2020 2020 2020 203c 2f70 3e0a 2020 2020         </p>.    
-00001c20: 2020 2020 2020 2020 3c2f 6469 763e 0a20          </div>. 
-00001c30: 2020 2020 2020 203c 2f64 6976 3e0a 2020         </div>.  
-00001c40: 2020 3c2f 6469 763e 0a3c 2f64 6976 3e0a    </div>.</div>.
-00001c50: 0a3c 6469 7620 636c 6173 733d 226d 6f64  .<div class="mod
-00001c60: 616c 2066 6164 6522 2069 643d 2269 642d  al fade" id="id-
-00001c70: 6d6f 6461 6c22 3e0a 2020 2020 3c64 6976  modal">.    <div
-00001c80: 2063 6c61 7373 3d22 6d6f 6461 6c2d 6469   class="modal-di
-00001c90: 616c 6f67 223e 0a20 2020 2020 2020 203c  alog">.        <
-00001ca0: 6469 7620 636c 6173 733d 226d 6f64 616c  div class="modal
-00001cb0: 2d63 6f6e 7465 6e74 223e 0a20 2020 2020  -content">.     
-00001cc0: 2020 2020 2020 203c 6469 7620 636c 6173         <div clas
-00001cd0: 733d 226d 6f64 616c 2d68 6561 6465 7222  s="modal-header"
-00001ce0: 3e0a 2020 2020 2020 2020 2020 2020 2020  >.              
-00001cf0: 2020 3c68 3420 636c 6173 733d 226d 6f64    <h4 class="mod
-00001d00: 616c 2d74 6974 6c65 223e 5369 676e 696e  al-title">Signin
-00001d10: 6720 7769 7468 2064 6967 6974 616c 2049  g with digital I
-00001d20: 443c 2f68 343e 0a20 2020 2020 2020 2020  D</h4>.         
-00001d30: 2020 203c 2f64 6976 3e0a 0a20 2020 2020     </div>..     
-00001d40: 2020 2020 2020 203c 6469 7620 636c 6173         <div clas
-00001d50: 733d 226d 6f64 616c 2d62 6f64 7922 3e0a  s="modal-body">.
-00001d60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001d70: 3c70 3e0a 2020 2020 2020 2020 2020 2020  <p>.            
-00001d80: 2020 2020 2020 2020 506c 6561 7365 2066          Please f
-00001d90: 6f6c 6c6f 7720 7468 6520 696e 7374 7275  ollow the instru
-00001da0: 6374 696f 6e73 2074 6f20 636f 6d70 6c65  ctions to comple
-00001db0: 7465 2074 6865 2073 6967 6e69 6e67 2070  te the signing p
-00001dc0: 726f 6365 7373 2e0a 2020 2020 2020 2020  rocess..        
-00001dd0: 2020 2020 2020 2020 3c2f 703e 0a20 2020          </p>.   
-00001de0: 2020 2020 2020 2020 203c 2f64 6976 3e0a           </div>.
-00001df0: 2020 2020 2020 2020 3c2f 6469 763e 0a20          </div>. 
-00001e00: 2020 203c 2f64 6976 3e0a 3c2f 6469 763e     </div>.</div>
-00001e10: 0a0a 3c64 6976 2063 6c61 7373 3d22 6d6f  ..<div class="mo
-00001e20: 6461 6c20 6661 6465 2220 6964 3d22 736d  dal fade" id="sm
-00001e30: 6172 7469 642d 6d6f 6461 6c22 3e0a 2020  artid-modal">.  
-00001e40: 2020 3c64 6976 2063 6c61 7373 3d22 6d6f    <div class="mo
-00001e50: 6461 6c2d 6469 616c 6f67 223e 0a20 2020  dal-dialog">.   
-00001e60: 2020 2020 203c 666f 726d 206e 616d 653d       <form name=
-00001e70: 2273 6d61 7274 4964 223e 0a20 2020 2020  "smartId">.     
-00001e80: 2020 2020 2020 203c 6469 7620 636c 6173         <div clas
-00001e90: 733d 226d 6f64 616c 2d63 6f6e 7465 6e74  s="modal-content
-00001ea0: 223e 0a20 2020 2020 2020 2020 2020 2020  ">.             
-00001eb0: 2020 203c 6469 7620 636c 6173 733d 226d     <div class="m
-00001ec0: 6f64 616c 2d68 6561 6465 7222 3e0a 2020  odal-header">.  
-00001ed0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001ee0: 2020 3c62 7574 746f 6e20 7479 7065 3d22    <button type="
-00001ef0: 6275 7474 6f6e 2220 636c 6173 733d 2263  button" class="c
-00001f00: 6c6f 7365 2220 6461 7461 2d64 6973 6d69  lose" data-dismi
-00001f10: 7373 3d22 6d6f 6461 6c22 2061 7269 612d  ss="modal" aria-
-00001f20: 6c61 6265 6c3d 2243 6c6f 7365 223e 3c73  label="Close"><s
-00001f30: 7061 6e0a 2020 2020 2020 2020 2020 2020  pan.            
-00001f40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001f50: 6172 6961 2d68 6964 6465 6e3d 2274 7275  aria-hidden="tru
-00001f60: 6522 3e26 7469 6d65 733b 3c2f 7370 616e  e">&times;</span
-00001f70: 3e0a 2020 2020 2020 2020 2020 2020 2020  >.              
-00001f80: 2020 2020 2020 3c2f 6275 7474 6f6e 3e0a        </button>.
-00001f90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001fa0: 2020 2020 3c68 3420 636c 6173 733d 226d      <h4 class="m
-00001fb0: 6f64 616c 2d74 6974 6c65 223e 5369 676e  odal-title">Sign
-00001fc0: 2074 6865 2066 696c 6573 2077 6974 6820   the files with 
-00001fd0: 536d 6172 7449 443c 2f68 343e 0a20 2020  SmartID</h4>.   
-00001fe0: 2020 2020 2020 2020 2020 2020 203c 2f64               </d
-00001ff0: 6976 3e0a 0a20 2020 2020 2020 2020 2020  iv>..           
-00002000: 2020 2020 203c 6469 7620 636c 6173 733d       <div class=
-00002010: 226d 6f64 616c 2d62 6f64 7922 3e0a 2020  "modal-body">.  
-00002020: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002030: 2020 3c64 6976 2063 6c61 7373 3d22 666f    <div class="fo
-00002040: 726d 2d67 726f 7570 223e 0a20 2020 2020  rm-group">.     
-00002050: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002060: 2020 203c 6c61 6265 6c20 666f 723d 2269     <label for="i
-00002070: 6443 6f64 6549 6e70 7574 223e 596f 7572  dCodeInput">Your
-00002080: 2049 4420 636f 6465 3a3c 2f6c 6162 656c   ID code:</label
-00002090: 3e0a 2020 2020 2020 2020 2020 2020 2020  >.              
-000020a0: 2020 2020 2020 2020 2020 3c69 6e70 7574            <input
-000020b0: 2074 7970 653d 2274 6578 7422 206e 616d   type="text" nam
-000020c0: 653d 2269 645f 636f 6465 2220 6964 3d22  e="id_code" id="
-000020d0: 6964 436f 6465 496e 7075 7422 2063 6c61  idCodeInput" cla
-000020e0: 7373 3d22 666f 726d 2d63 6f6e 7472 6f6c  ss="form-control
-000020f0: 220a 2020 2020 2020 2020 2020 2020 2020  ".              
-00002100: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002110: 2076 616c 7565 3d22 7b7b 2072 6571 7565   value="{{ reque
-00002120: 7374 2e73 6573 7369 6f6e 2e73 6d61 7274  st.session.smart
-00002130: 6964 5f74 6573 745f 6964 5f63 6f64 6520  id_test_id_code 
-00002140: 7c20 6465 6661 756c 743a 2733 3033 3033  | default:'30303
-00002150: 3033 3939 3134 2720 7d7d 2220 2f3e 0a20  039914' }}" />. 
-00002160: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002170: 2020 203c 2f64 6976 3e0a 2020 2020 2020     </div>.      
-00002180: 2020 2020 2020 2020 2020 2020 2020 3c64                <d
-00002190: 6976 2063 6c61 7373 3d22 666f 726d 2d67  iv class="form-g
-000021a0: 726f 7570 223e 0a20 2020 2020 2020 2020  roup">.         
-000021b0: 2020 2020 2020 2020 2020 2020 2020 203c                 <
-000021c0: 6c61 6265 6c20 666f 723d 2263 6f75 6e74  label for="count
-000021d0: 7279 496e 7075 7422 3e43 6f75 6e74 7279  ryInput">Country
-000021e0: 3a3c 2f6c 6162 656c 3e0a 2020 2020 2020  :</label>.      
-000021f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002200: 2020 3c73 656c 6563 7420 6e61 6d65 3d22    <select name="
-00002210: 636f 756e 7472 7922 2069 643d 2263 6f75  country" id="cou
-00002220: 6e74 7279 496e 7075 7422 2063 6c61 7373  ntryInput" class
-00002230: 3d22 666f 726d 2d63 6f6e 7472 6f6c 223e  ="form-control">
-00002240: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00002250: 2020 2020 2020 2020 2020 2020 203c 6f70               <op
-00002260: 7469 6f6e 2076 616c 7565 3d22 223e 2d2d  tion value="">--
-00002270: 204e 6f74 2073 656c 6563 7465 6420 2d2d   Not selected --
-00002280: 2028 6465 6661 756c 7473 2074 6f20 4573   (defaults to Es
-00002290: 746f 6e69 6129 3c2f 6f70 7469 6f6e 3e0a  tonia)</option>.
-000022a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000022b0: 2020 2020 2020 2020 2020 2020 3c6f 7074              <opt
-000022c0: 696f 6e20 7661 6c75 653d 2245 4522 3e45  ion value="EE">E
-000022d0: 7374 6f6e 6961 3c2f 6f70 7469 6f6e 3e0a  stonia</option>.
-000022e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000022f0: 2020 2020 2020 2020 2020 2020 3c6f 7074              <opt
-00002300: 696f 6e20 7661 6c75 653d 224c 5622 3e4c  ion value="LV">L
-00002310: 6174 7669 613c 2f6f 7074 696f 6e3e 0a20  atvia</option>. 
-00002320: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002330: 2020 2020 2020 2020 2020 203c 6f70 7469             <opti
-00002340: 6f6e 2076 616c 7565 3d22 4c54 223e 4c69  on value="LT">Li
-00002350: 7468 7561 6e69 613c 2f6f 7074 696f 6e3e  thuania</option>
-00002360: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00002370: 2020 2020 2020 2020 203c 2f73 656c 6563           </selec
-00002380: 743e 0a20 2020 2020 2020 2020 2020 2020  t>.             
-00002390: 2020 2020 2020 203c 2f64 6976 3e0a 2020         </div>.  
-000023a0: 2020 2020 2020 2020 2020 2020 2020 3c2f                </
-000023b0: 6469 763e 0a0a 2020 2020 2020 2020 2020  div>..          
-000023c0: 2020 2020 2020 3c64 6976 2063 6c61 7373        <div class
-000023d0: 3d22 6d6f 6461 6c2d 666f 6f74 6572 223e  ="modal-footer">
-000023e0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000023f0: 2020 2020 203c 6275 7474 6f6e 2074 7970       <button typ
-00002400: 653d 2273 7562 6d69 7422 2063 6c61 7373  e="submit" class
-00002410: 3d22 6274 6e20 6274 6e2d 7072 696d 6172  ="btn btn-primar
-00002420: 7922 3e53 6967 6e3c 2f62 7574 746f 6e3e  y">Sign</button>
-00002430: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00002440: 2020 2020 203c 6469 7620 636c 6173 733d       <div class=
-00002450: 226c 6473 2d64 7561 6c2d 7269 6e67 223e  "lds-dual-ring">
-00002460: 3c2f 6469 763e 0a20 2020 2020 2020 2020  </div>.         
-00002470: 2020 2020 2020 203c 2f64 6976 3e0a 2020         </div>.  
-00002480: 2020 2020 2020 2020 2020 3c2f 6469 763e            </div>
-00002490: 0a20 2020 2020 2020 203c 2f66 6f72 6d3e  .        </form>
-000024a0: 0a20 2020 203c 2f64 6976 3e0a 3c2f 6469  .    </div>.</di
-000024b0: 763e 0a0a 3c64 6976 2063 6c61 7373 3d22  v>..<div class="
-000024c0: 6d6f 6461 6c20 6661 6465 2220 6964 3d22  modal fade" id="
-000024d0: 7665 7269 6669 6361 7469 6f6e 2d63 6f64  verification-cod
-000024e0: 652d 6d6f 6461 6c22 3e0a 2020 2020 3c64  e-modal">.    <d
-000024f0: 6976 2063 6c61 7373 3d22 6d6f 6461 6c2d  iv class="modal-
-00002500: 6469 616c 6f67 223e 0a20 2020 2020 2020  dialog">.       
-00002510: 203c 6469 7620 636c 6173 733d 226d 6f64   <div class="mod
-00002520: 616c 2d63 6f6e 7465 6e74 223e 0a20 2020  al-content">.   
-00002530: 2020 2020 2020 2020 203c 6469 7620 636c           <div cl
-00002540: 6173 733d 226d 6f64 616c 2d68 6561 6465  ass="modal-heade
-00002550: 7222 3e0a 2020 2020 2020 2020 2020 2020  r">.            
-00002560: 2020 2020 3c68 3420 636c 6173 733d 226d      <h4 class="m
-00002570: 6f64 616c 2d74 6974 6c65 2220 6964 3d22  odal-title" id="
-00002580: 736d 6172 7469 642d 7374 6570 223e 5665  smartid-step">Ve
-00002590: 7269 6669 6361 7469 6f6e 2063 6f64 653c  rification code<
-000025a0: 2f68 343e 0a20 2020 2020 2020 2020 2020  /h4>.           
-000025b0: 203c 2f64 6976 3e0a 0a20 2020 2020 2020   </div>..       
-000025c0: 2020 2020 203c 6469 7620 636c 6173 733d       <div class=
-000025d0: 226d 6f64 616c 2d62 6f64 7922 3e0a 2020  "modal-body">.  
-000025e0: 2020 2020 2020 2020 2020 2020 2020 3c70                <p
-000025f0: 3e0a 2020 2020 2020 2020 2020 2020 2020  >.              
-00002600: 2020 2020 2020 4d61 6b65 2073 7572 6520        Make sure 
-00002610: 796f 7520 6172 6520 7365 6569 6e67 2074  you are seeing t
-00002620: 6869 7320 7665 7269 6669 6361 7469 6f6e  his verification
-00002630: 2063 6f64 6520 6f6e 2079 6f75 7220 6465   code on your de
-00002640: 7669 6365 3a0a 2020 2020 2020 2020 2020  vice:.          
-00002650: 2020 2020 2020 2020 2020 3c62 2069 643d            <b id=
-00002660: 2273 6d61 7274 6964 2d76 6572 6966 6963  "smartid-verific
-00002670: 6174 696f 6e2d 636f 6465 223e 4b4f 4f44  ation-code">KOOD
-00002680: 3c2f 623e 0a20 2020 2020 2020 2020 2020  </b>.           
-00002690: 2020 2020 203c 2f70 3e0a 2020 2020 2020       </p>.      
-000026a0: 2020 2020 2020 3c2f 6469 763e 0a20 2020        </div>.   
-000026b0: 2020 2020 203c 2f64 6976 3e0a 2020 2020       </div>.    
-000026c0: 3c2f 6469 763e 0a3c 2f64 6976 3e0a 0a3c  </div>.</div>..<
-000026d0: 6469 7620 636c 6173 733d 226d 6f64 616c  div class="modal
-000026e0: 2066 6164 6522 2069 643d 2273 7563 6365   fade" id="succe
-000026f0: 7373 2d6d 6f64 616c 223e 0a20 2020 203c  ss-modal">.    <
-00002700: 6469 7620 636c 6173 733d 226d 6f64 616c  div class="modal
-00002710: 2d64 6961 6c6f 6722 3e0a 2020 2020 2020  -dialog">.      
-00002720: 2020 3c64 6976 2063 6c61 7373 3d22 6d6f    <div class="mo
-00002730: 6461 6c2d 636f 6e74 656e 7422 3e0a 2020  dal-content">.  
-00002740: 2020 2020 2020 2020 2020 3c64 6976 2063            <div c
-00002750: 6c61 7373 3d22 6d6f 6461 6c2d 6865 6164  lass="modal-head
-00002760: 6572 223e 0a20 2020 2020 2020 2020 2020  er">.           
-00002770: 2020 2020 203c 6834 2063 6c61 7373 3d22       <h4 class="
-00002780: 6d6f 6461 6c2d 7469 746c 6522 3e53 6967  modal-title">Sig
-00002790: 6e69 6e67 2063 6f6d 706c 6574 653c 2f68  ning complete</h
-000027a0: 343e 0a20 2020 2020 2020 2020 2020 203c  4>.            <
-000027b0: 2f64 6976 3e0a 0a20 2020 2020 2020 2020  /div>..         
-000027c0: 2020 203c 6469 7620 636c 6173 733d 226d     <div class="m
-000027d0: 6f64 616c 2d62 6f64 7922 3e0a 2020 2020  odal-body">.    
-000027e0: 2020 2020 2020 2020 2020 2020 3c70 3e0a              <p>.
-000027f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002800: 2020 2020 5468 6520 7570 6c6f 6164 6564      The uploaded
-00002810: 2066 696c 6573 2077 6572 6520 7375 6363   files were succ
-00002820: 6573 7366 756c 6c79 2064 6967 6974 616c  essfully digital
-00002830: 6c79 2073 6967 6e65 642c 2070 6c65 6173  ly signed, pleas
-00002840: 6520 636c 6963 6b20 7468 6520 666f 6c6c  e click the foll
-00002850: 6f77 696e 6720 6c69 6e6b 0a20 2020 2020  owing link.     
-00002860: 2020 2020 2020 2020 2020 2020 2020 2074                 t
-00002870: 6f20 646f 776e 6c6f 6164 2074 6865 2063  o download the c
-00002880: 6f6e 7461 696e 6572 2061 6e64 2066 696e  ontainer and fin
-00002890: 6973 6820 7468 6520 7369 676e 696e 6720  ish the signing 
-000028a0: 7072 6f63 6573 732e 0a20 2020 2020 2020  process..       
-000028b0: 2020 2020 2020 2020 203c 2f70 3e0a 0a20           </p>.. 
-000028c0: 2020 2020 2020 2020 2020 2020 2020 203c                 <
-000028d0: 6120 6872 6566 3d22 2322 2069 643d 2267  a href="#" id="g
-000028e0: 6574 2d64 6f63 756d 656e 7422 2074 6172  et-document" tar
-000028f0: 6765 743d 225f 626c 616e 6b22 3e44 6f77  get="_blank">Dow
-00002900: 6e6c 6f61 6420 6669 6c65 3c2f 613e 2026  nload file</a> &
-00002910: 6d69 6464 6f74 3b0a 2020 2020 2020 2020  middot;.        
-00002920: 2020 2020 2020 2020 3c61 2068 7265 663d          <a href=
-00002930: 2223 2220 6f6e 636c 6963 6b3d 2277 696e  "#" onclick="win
-00002940: 646f 772e 6c6f 6361 7469 6f6e 2e72 656c  dow.location.rel
-00002950: 6f61 6428 293b 2072 6574 7572 6e20 6661  oad(); return fa
-00002960: 6c73 6522 3e43 616e 6365 6c3c 2f61 3e0a  lse">Cancel</a>.
-00002970: 2020 2020 2020 2020 2020 2020 3c2f 6469              </di
-00002980: 763e 0a20 2020 2020 2020 203c 2f64 6976  v>.        </div
-00002990: 3e0a 2020 2020 3c2f 6469 763e 0a3c 2f64  >.    </div>.</d
-000029a0: 6976 3e0a 0a3c 7363 7269 7074 2073 7263  iv>..<script src
-000029b0: 3d22 2f2f 616a 6178 2e67 6f6f 676c 6561  ="//ajax.googlea
-000029c0: 7069 732e 636f 6d2f 616a 6178 2f6c 6962  pis.com/ajax/lib
-000029d0: 732f 6a71 7565 7279 2f31 2e31 312e 312f  s/jquery/1.11.1/
-000029e0: 6a71 7565 7279 2e6d 696e 2e6a 7322 3e3c  jquery.min.js"><
-000029f0: 2f73 6372 6970 743e 0a3c 7363 7269 7074  /script>.<script
-00002a00: 2073 7263 3d22 2f2f 6d61 7863 646e 2e62   src="//maxcdn.b
-00002a10: 6f6f 7473 7472 6170 6364 6e2e 636f 6d2f  ootstrapcdn.com/
-00002a20: 626f 6f74 7374 7261 702f 332e 332e 342f  bootstrap/3.3.4/
-00002a30: 6a73 2f62 6f6f 7473 7472 6170 2e6d 696e  js/bootstrap.min
-00002a40: 2e6a 7322 3e3c 2f73 6372 6970 743e 0a0a  .js"></script>..
-00002a50: 0a3c 7363 7269 7074 2074 7970 653d 2274  .<script type="t
-00002a60: 6578 742f 6a61 7661 7363 7269 7074 2220  ext/javascript" 
-00002a70: 7372 633d 227b 2520 7374 6174 6963 2027  src="{% static '
-00002a80: 6573 7465 6964 2d68 656c 7065 722f 7765  esteid-helper/we
-00002a90: 622d 6569 642e 6a73 2720 257d 223e 3c2f  b-eid.js' %}"></
-00002aa0: 7363 7269 7074 3e0a 3c73 6372 6970 7420  script>.<script 
-00002ab0: 7479 7065 3d22 7465 7874 2f6a 6176 6173  type="text/javas
-00002ac0: 6372 6970 7422 2073 7263 3d22 7b25 2073  cript" src="{% s
-00002ad0: 7461 7469 6320 2765 7374 6569 642d 6865  tatic 'esteid-he
-00002ae0: 6c70 6572 2f45 7374 6569 642e 6d61 696e  lper/Esteid.main
-00002af0: 2e77 6562 2e6a 7327 2025 7d22 3e3c 2f73  .web.js' %}"></s
-00002b00: 6372 6970 743e 0a0a 3c73 6372 6970 7420  cript>..<script 
-00002b10: 7479 7065 3d22 7465 7874 2f6a 6176 6173  type="text/javas
-00002b20: 6372 6970 7422 3e0a 2020 2020 6675 6e63  cript">.    func
-00002b30: 7469 6f6e 2073 7461 7274 5370 696e 6e65  tion startSpinne
-00002b40: 7228 666f 726d 2920 7b0a 2020 2020 2020  r(form) {.      
-00002b50: 2020 2428 2262 7574 746f 6e22 2c20 666f    $("button", fo
-00002b60: 726d 292e 6869 6465 2829 0a20 2020 2020  rm).hide().     
-00002b70: 2020 2024 2822 2e6c 6473 2d64 7561 6c2d     $(".lds-dual-
-00002b80: 7269 6e67 222c 2066 6f72 6d29 2e63 7373  ring", form).css
-00002b90: 2822 6469 7370 6c61 7922 2c20 2269 6e6c  ("display", "inl
-00002ba0: 696e 652d 626c 6f63 6b22 290a 2020 2020  ine-block").    
-00002bb0: 7d0a 0a20 2020 2066 756e 6374 696f 6e20  }..    function 
-00002bc0: 7374 6f70 5370 696e 6e65 7228 666f 726d  stopSpinner(form
-00002bd0: 2920 7b0a 2020 2020 2020 2020 2428 2262  ) {.        $("b
-00002be0: 7574 746f 6e22 2c20 666f 726d 292e 7368  utton", form).sh
-00002bf0: 6f77 2829 0a20 2020 2020 2020 2024 2822  ow().        $("
-00002c00: 2e6c 6473 2d64 7561 6c2d 7269 6e67 222c  .lds-dual-ring",
-00002c10: 2066 6f72 6d29 2e63 7373 2822 6469 7370   form).css("disp
-00002c20: 6c61 7922 2c20 226e 6f6e 6522 290a 2020  lay", "none").  
-00002c30: 2020 7d0a 0a20 2020 2066 756e 6374 696f    }..    functio
-00002c40: 6e20 6f6e 4572 726f 7228 7265 7329 207b  n onError(res) {
-00002c50: 0a20 2020 2020 2020 2063 6f6e 736f 6c65  .        console
-00002c60: 2e6c 6f67 2822 4572 726f 723a 222c 2072  .log("Error:", r
-00002c70: 6573 290a 2020 2020 2020 2020 6966 2028  es).        if (
-00002c80: 7265 7320 2626 2072 6573 2e6d 6573 7361  res && res.messa
-00002c90: 6765 2920 7b0a 2020 2020 2020 2020 2020  ge) {.          
-00002ca0: 2020 616c 6572 7428 7265 732e 6d65 7373    alert(res.mess
-00002cb0: 6167 6529 0a20 2020 2020 2020 207d 2065  age).        } e
-00002cc0: 6c73 6520 7b0a 2020 2020 2020 2020 2020  lse {.          
-00002cd0: 2020 616c 6572 7428 2753 6f6d 6574 6869    alert('Somethi
-00002ce0: 6e67 2077 656e 7420 7772 6f6e 672c 2070  ng went wrong, p
-00002cf0: 6c65 6173 6520 7472 7920 6167 6169 6e27  lease try again'
-00002d00: 290a 2020 2020 2020 2020 7d0a 2020 2020  ).        }.    
-00002d10: 7d0a 0a20 2020 2024 2866 756e 6374 696f  }..    $(functio
-00002d20: 6e20 2829 207b 0a20 2020 2020 2020 2076  n () {.        v
-00002d30: 6172 2064 6f77 6e6c 6f61 6455 726c 203d  ar downloadUrl =
-00002d40: 2027 7b25 2075 726c 2027 646f 776e 6c6f   '{% url 'downlo
-00002d50: 6164 5f73 6967 6e65 645f 636f 6e74 6169  ad_signed_contai
-00002d60: 6e65 7227 2025 7d27 0a20 2020 2020 2020  ner' %}'.       
-00002d70: 2076 6172 206d 616e 6167 6572 203d 206e   var manager = n
-00002d80: 6577 2045 7374 6569 642e 4964 656e 7469  ew Esteid.Identi
-00002d90: 6669 6361 7469 6f6e 4d61 6e61 6765 7228  ficationManager(
-00002da0: 7b0a 2020 2020 2020 2020 2020 2020 6c61  {.            la
-00002db0: 6e67 7561 6765 3a20 4573 7465 6964 2e4c  nguage: Esteid.L
-00002dc0: 616e 6775 6167 6573 2e45 542c 0a0a 2020  anguages.ET,..  
-00002dd0: 2020 2020 2020 2020 2020 6964 5572 6c3a            idUrl:
-00002de0: 2027 7b25 2075 726c 2027 7369 676e 2d69   '{% url 'sign-i
-00002df0: 6463 6172 6427 2025 7d27 2c0a 0a20 2020  dcard' %}',..   
-00002e00: 2020 2020 2020 2020 206d 6f62 696c 6549           mobileI
-00002e10: 6455 726c 3a20 277b 2520 7572 6c20 2773  dUrl: '{% url 's
-00002e20: 6967 6e2d 6d6f 6269 6c65 6964 2720 257d  ign-mobileid' %}
-00002e30: 272c 0a0a 2020 2020 2020 2020 2020 2020  ',..            
-00002e40: 736d 6172 7449 6455 726c 3a20 277b 2520  smartIdUrl: '{% 
-00002e50: 7572 6c20 2773 6967 6e2d 736d 6172 7469  url 'sign-smarti
-00002e60: 6427 2025 7d27 2c0a 0a20 2020 2020 2020  d' %}',..       
-00002e70: 2020 2020 2063 7372 6654 6f6b 656e 3a20       csrfToken: 
-00002e80: 277b 7b20 6373 7266 5f74 6f6b 656e 207d  '{{ csrf_token }
-00002e90: 7d27 0a20 2020 2020 2020 207d 290a 0a20  }'.        }).. 
-00002ea0: 2020 2020 2020 2066 756e 6374 696f 6e20         function 
-00002eb0: 6f6e 5369 676e 6564 2829 207b 0a20 2020  onSigned() {.   
-00002ec0: 2020 2020 2020 2020 2024 2827 2367 6574           $('#get
-00002ed0: 2d64 6f63 756d 656e 7427 292e 6174 7472  -document').attr
-00002ee0: 2827 6872 6566 272c 2064 6f77 6e6c 6f61  ('href', downloa
-00002ef0: 6455 726c 290a 0a20 2020 2020 2020 2020  dUrl)..         
-00002f00: 2020 2024 2827 2373 7563 6365 7373 2d6d     $('#success-m
-00002f10: 6f64 616c 2729 2e6d 6f64 616c 287b 0a20  odal').modal({. 
-00002f20: 2020 2020 2020 2020 2020 2020 2020 2062                 b
-00002f30: 6163 6b64 726f 703a 2027 7374 6174 6963  ackdrop: 'static
-00002f40: 272c 0a20 2020 2020 2020 2020 2020 2020  ',.             
-00002f50: 2020 206b 6579 626f 6172 643a 2066 616c     keyboard: fal
-00002f60: 7365 0a20 2020 2020 2020 2020 2020 207d  se.            }
-00002f70: 290a 2020 2020 2020 2020 7d0a 0a20 2020  ).        }..   
-00002f80: 2020 2020 2024 2827 2373 6967 6e2d 6d69       $('#sign-mi
-00002f90: 6427 292e 6f6e 2827 636c 6963 6b27 2c20  d').on('click', 
-00002fa0: 6675 6e63 7469 6f6e 2028 6529 207b 0a20  function (e) {. 
-00002fb0: 2020 2020 2020 2020 2020 2065 2e70 7265             e.pre
-00002fc0: 7665 6e74 4465 6661 756c 7428 290a 0a20  ventDefault().. 
-00002fd0: 2020 2020 2020 2020 2020 2024 2827 236d             $('#m
-00002fe0: 6964 2d6d 6f64 616c 2729 2e6d 6f64 616c  id-modal').modal
-00002ff0: 2829 0a20 2020 2020 2020 207d 290a 0a20  ().        }).. 
-00003000: 2020 2020 2020 2076 6172 206d 6f62 696c         var mobil
-00003010: 6549 6446 6f72 6d20 3d20 646f 6375 6d65  eIdForm = docume
-00003020: 6e74 2e66 6f72 6d73 2e6d 6f62 696c 6549  nt.forms.mobileI
-00003030: 640a 2020 2020 2020 2020 6d6f 6269 6c65  d.        mobile
-00003040: 4964 466f 726d 2e6f 6e73 7562 6d69 7420  IdForm.onsubmit 
-00003050: 3d20 6675 6e63 7469 6f6e 2028 6529 207b  = function (e) {
-00003060: 0a20 2020 2020 2020 2020 2020 2065 2e70  .            e.p
-00003070: 7265 7665 6e74 4465 6661 756c 7428 290a  reventDefault().
-00003080: 2020 2020 2020 2020 2020 2020 7661 7220              var 
-00003090: 7068 6f6e 654e 7220 3d20 6d6f 6269 6c65  phoneNr = mobile
-000030a0: 4964 466f 726d 2e70 686f 6e65 5f6e 722e  IdForm.phone_nr.
-000030b0: 7661 6c75 650a 2020 2020 2020 2020 2020  value.          
-000030c0: 2020 7661 7220 6964 436f 6465 203d 206d    var idCode = m
-000030d0: 6f62 696c 6549 6446 6f72 6d2e 6964 5f63  obileIdForm.id_c
-000030e0: 6f64 652e 7661 6c75 650a 0a20 2020 2020  ode.value..     
-000030f0: 2020 2020 2020 2069 6620 2821 7068 6f6e         if (!phon
-00003100: 654e 7229 207b 0a20 2020 2020 2020 2020  eNr) {.         
-00003110: 2020 2020 2020 2061 6c65 7274 2827 506c         alert('Pl
-00003120: 6561 7365 2065 6e74 6572 2061 2070 686f  ease enter a pho
-00003130: 6e65 206e 756d 6265 7227 290a 2020 2020  ne number').    
-00003140: 2020 2020 2020 2020 2020 2020 7265 7475              retu
-00003150: 726e 0a20 2020 2020 2020 2020 2020 207d  rn.            }
-00003160: 0a20 2020 2020 2020 2020 2020 2069 6620  .            if 
-00003170: 2821 6964 436f 6465 2920 7b0a 2020 2020  (!idCode) {.    
-00003180: 2020 2020 2020 2020 2020 2020 616c 6572              aler
-00003190: 7428 2750 6c65 6173 6520 656e 7465 7220  t('Please enter 
-000031a0: 616e 2049 4420 636f 6465 2729 0a20 2020  an ID code').   
-000031b0: 2020 2020 2020 2020 2020 2020 2072 6574               ret
-000031c0: 7572 6e0a 2020 2020 2020 2020 2020 2020  urn.            
-000031d0: 7d0a 0a20 2020 2020 2020 2020 2020 2063  }..            c
-000031e0: 6f6e 736f 6c65 2e6c 6f67 2827 4d49 443a  onsole.log('MID:
-000031f0: 2073 6967 6e69 6e67 2077 6974 6820 7068   signing with ph
-00003200: 6f6e 654e 7227 2c20 7068 6f6e 654e 722c  oneNr', phoneNr,
-00003210: 2027 616e 6420 6964 2063 6f64 6527 2c20   'and id code', 
-00003220: 6964 436f 6465 290a 0a20 2020 2020 2020  idCode)..       
-00003230: 2020 2020 2073 7461 7274 5370 696e 6e65       startSpinne
-00003240: 7228 6d6f 6269 6c65 4964 466f 726d 290a  r(mobileIdForm).
-00003250: 0a20 2020 2020 2020 2020 2020 202f 2f20  .            // 
-00003260: 4361 6c6c 2049 6465 6e74 6966 6963 6174  Call Identificat
-00003270: 696f 6e4d 616e 6167 6572 2e73 6967 6e20  ionManager.sign 
-00003280: 7768 6963 6820 6361 6c6c 7320 7468 6520  which calls the 
-00003290: 6261 636b 656e 6420 656e 6470 6f69 6e74  backend endpoint
-000032a0: 2074 6f20 7374 6172 7420 6d6f 6269 6c65   to start mobile
-000032b0: 4964 2073 6967 6e69 6e67 2070 726f 6365  Id signing proce
-000032c0: 7373 0a20 2020 2020 2020 2020 2020 206d  ss.            m
-000032d0: 616e 6167 6572 2e73 6967 6e57 6974 684d  anager.signWithM
-000032e0: 6f62 696c 6549 6428 7b0a 2020 2020 2020  obileId({.      
-000032f0: 2020 2020 2020 2020 2020 7068 6f6e 654e            phoneN
-00003300: 756d 6265 723a 2070 686f 6e65 4e72 2c0a  umber: phoneNr,.
-00003310: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003320: 6964 436f 6465 3a20 6964 436f 6465 2c0a  idCode: idCode,.
-00003330: 2020 2020 2020 2020 2020 2020 7d29 0a0a              })..
-00003340: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003350: 2e74 6865 6e28 6675 6e63 7469 6f6e 2028  .then(function (
-00003360: 7265 7370 6f6e 7365 2920 7b0a 2020 2020  response) {.    
-00003370: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003380: 636f 6e73 6f6c 652e 6c6f 6728 274d 4944  console.log('MID
-00003390: 3a20 676f 7420 7665 7269 6669 6361 7469  : got verificati
-000033a0: 6f6e 2063 6f64 6527 2c20 7265 7370 6f6e  on code', respon
-000033b0: 7365 2e76 6572 6966 6963 6174 696f 6e5f  se.verification_
-000033c0: 636f 6465 290a 0a20 2020 2020 2020 2020  code)..         
-000033d0: 2020 2020 2020 2020 2020 202f 2f20 476f             // Go
-000033e0: 7420 7265 7370 6f6e 7365 2c20 7368 6f77  t response, show
-000033f0: 2063 6861 6c6c 656e 6765 206d 6f64 616c   challenge modal
-00003400: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00003410: 2020 2020 2024 2827 2363 6861 6c6c 656e       $('#challen
-00003420: 6765 2d63 6f64 6527 292e 7465 7874 2872  ge-code').text(r
-00003430: 6573 706f 6e73 652e 7665 7269 6669 6361  esponse.verifica
-00003440: 7469 6f6e 5f63 6f64 6529 0a20 2020 2020  tion_code).     
-00003450: 2020 2020 2020 2020 2020 2020 2020 2024                 $
-00003460: 2827 2363 6861 6c6c 656e 6765 2d6d 6f64  ('#challenge-mod
-00003470: 616c 2729 2e6d 6f64 616c 287b 0a20 2020  al').modal({.   
-00003480: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003490: 2020 2020 2062 6163 6b64 726f 703a 2027       backdrop: '
-000034a0: 7374 6174 6963 272c 0a20 2020 2020 2020  static',.       
-000034b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000034c0: 206b 6579 626f 6172 643a 2066 616c 7365   keyboard: false
-000034d0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000034e0: 2020 2020 207d 290a 0a20 2020 2020 2020       })..       
-000034f0: 2020 2020 2020 2020 2020 2020 2024 2827               $('
-00003500: 236d 6964 2d6d 6f64 616c 2729 2e6d 6f64  #mid-modal').mod
-00003510: 616c 2827 6869 6465 2729 0a0a 2020 2020  al('hide')..    
-00003520: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003530: 6d61 6e61 6765 722e 6d69 6453 7461 7475  manager.midStatu
-00003540: 7328 292e 7468 656e 280a 2020 2020 2020  s().then(.      
-00003550: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003560: 2020 6675 6e63 7469 6f6e 2028 2920 7b0a    function () {.
-00003570: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003580: 2020 2020 2020 2020 2020 2020 2428 2723              $('#
-00003590: 6368 616c 6c65 6e67 652d 6d6f 6461 6c27  challenge-modal'
-000035a0: 292e 6d6f 6461 6c28 2768 6964 6527 290a  ).modal('hide').
-000035b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000035c0: 2020 2020 2020 2020 2020 2020 6f6e 5369              onSi
-000035d0: 676e 6564 2829 0a20 2020 2020 2020 2020  gned().         
-000035e0: 2020 2020 2020 2020 2020 2020 2020 207d                 }
-000035f0: 2c0a 0a20 2020 2020 2020 2020 2020 2020  ,..             
-00003600: 2020 2020 2020 2020 2020 2066 756e 6374             funct
-00003610: 696f 6e20 2872 6573 2920 7b0a 2020 2020  ion (res) {.    
-00003620: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003630: 2020 2020 2020 2020 6966 2028 7265 732e          if (res.
-00003640: 6d65 7373 6167 6529 207b 0a20 2020 2020  message) {.     
-00003650: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003660: 2020 2020 2020 2020 2020 2061 6c65 7274             alert
-00003670: 2872 6573 2e6d 6573 7361 6765 290a 2020  (res.message).  
-00003680: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003690: 2020 2020 2020 2020 2020 7d20 656c 7365            } else
-000036a0: 207b 0a20 2020 2020 2020 2020 2020 2020   {.             
-000036b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000036c0: 2020 2061 6c65 7274 2827 536f 6d65 7468     alert('Someth
-000036d0: 696e 6720 7765 6e74 2077 726f 6e67 2c20  ing went wrong, 
-000036e0: 706c 6561 7365 2074 7279 2061 6761 696e  please try again
-000036f0: 2729 0a20 2020 2020 2020 2020 2020 2020  ').             
-00003700: 2020 2020 2020 2020 2020 2020 2020 207d                 }
-00003710: 0a0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00003720: 2020 2020 2020 2020 2020 2020 2020 2428                $(
-00003730: 2723 6368 616c 6c65 6e67 652d 6d6f 6461  '#challenge-moda
-00003740: 6c27 292e 6d6f 6461 6c28 2768 6964 6527  l').modal('hide'
-00003750: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
-00003760: 2020 2020 2020 2020 2020 7d0a 2020 2020            }.    
-00003770: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003780: 290a 0a20 2020 2020 2020 2020 2020 2020  )..             
-00003790: 2020 207d 2c20 6f6e 4572 726f 7229 0a20     }, onError). 
-000037a0: 2020 2020 2020 2020 2020 2020 2020 202e                 .
-000037b0: 6669 6e61 6c6c 7928 0a20 2020 2020 2020  finally(.       
-000037c0: 2020 2020 2020 2020 2020 2020 2028 2920               () 
-000037d0: 3d3e 2073 746f 7053 7069 6e6e 6572 286d  => stopSpinner(m
-000037e0: 6f62 696c 6549 6446 6f72 6d29 0a20 2020  obileIdForm).   
-000037f0: 2020 2020 2020 2020 2020 2020 2029 0a20               ). 
-00003800: 2020 2020 2020 207d 0a0a 2020 2020 2020         }..      
-00003810: 2020 2428 2723 7369 676e 2d73 6d61 7274    $('#sign-smart
-00003820: 6964 2729 2e6f 6e28 2763 6c69 636b 272c  id').on('click',
-00003830: 2066 756e 6374 696f 6e20 2865 2920 7b0a   function (e) {.
-00003840: 2020 2020 2020 2020 2020 2020 652e 7072              e.pr
-00003850: 6576 656e 7444 6566 6175 6c74 2829 0a0a  eventDefault()..
-00003860: 2020 2020 2020 2020 2020 2020 2428 2723              $('#
-00003870: 736d 6172 7469 642d 6d6f 6461 6c27 292e  smartid-modal').
-00003880: 6d6f 6461 6c28 290a 2020 2020 2020 2020  modal().        
-00003890: 7d29 0a0a 2020 2020 2020 2020 7661 7220  })..        var 
-000038a0: 736d 6172 7449 6446 6f72 6d20 3d20 646f  smartIdForm = do
-000038b0: 6375 6d65 6e74 2e66 6f72 6d73 2e73 6d61  cument.forms.sma
-000038c0: 7274 4964 0a20 2020 2020 2020 2073 6d61  rtId.        sma
-000038d0: 7274 4964 466f 726d 2e6f 6e73 7562 6d69  rtIdForm.onsubmi
-000038e0: 7420 3d20 6675 6e63 7469 6f6e 2028 6529  t = function (e)
-000038f0: 207b 0a20 2020 2020 2020 2020 2020 2063   {.            c
-00003900: 6f6e 736f 6c65 2e6c 6f67 2822 5369 676e  onsole.log("Sign
-00003910: 696e 6720 7769 7468 2053 6d61 7274 2049  ing with Smart I
-00003920: 4422 290a 2020 2020 2020 2020 2020 2020  D").            
-00003930: 7661 7220 7469 6d65 6f75 7446 6f72 5665  var timeoutForVe
-00003940: 7269 6669 6361 7469 6f6e 436f 6465 203d  rificationCode =
-00003950: 2033 3030 3020 202f 2f20 6465 6c61 7920   3000  // delay 
-00003960: 706f 6c6c 696e 6720 746f 206c 6574 2075  polling to let u
-00003970: 7365 7220 746f 2065 6e74 6572 2076 6572  ser to enter ver
-00003980: 6966 6963 6174 696f 6e20 636f 6465 0a0a  ification code..
-00003990: 2020 2020 2020 2020 2020 2020 2f2a 2a20              /** 
-000039a0: 5365 656d 7320 6e6f 206c 6f6e 6765 7220  Seems no longer 
-000039b0: 6e65 6365 7373 6172 7920 666f 7220 7369  necessary for si
-000039c0: 676e 696e 672e 204b 6570 7420 6865 7265  gning. Kept here
-000039d0: 2061 7320 6974 206d 6967 6874 2062 6520   as it might be 
-000039e0: 7573 6566 756c 2066 6f72 2061 7574 6865  useful for authe
-000039f0: 6e74 6963 6174 696f 6e20 2a2f 0a20 2020  ntication */.   
-00003a00: 2020 2020 2020 2020 2066 756e 6374 696f           functio
-00003a10: 6e20 6f6e 5375 6363 6573 7341 7574 6828  n onSuccessAuth(
-00003a20: 7265 7370 6f6e 7365 2920 7b0a 2020 2020  response) {.    
-00003a30: 2020 2020 2020 2020 2020 2020 2f2f 2047              // G
-00003a40: 6f74 2061 2073 7563 6365 7373 6675 6c20  ot a successful 
-00003a50: 6175 7468 2d73 7461 7274 2072 6571 7565  auth-start reque
-00003a60: 7374 2e2e 2e0a 2020 2020 2020 2020 2020  st....          
-00003a70: 2020 2020 2020 636f 6e73 6f6c 652e 6c6f        console.lo
-00003a80: 6728 2753 6d61 7274 4944 3a20 6175 7468  g('SmartID: auth
-00003a90: 2076 6572 6966 6963 6174 696f 6e20 636f   verification co
-00003aa0: 6465 272c 2072 6573 706f 6e73 652e 7665  de', response.ve
-00003ab0: 7269 6669 6361 7469 6f6e 5f63 6f64 6529  rification_code)
-00003ac0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00003ad0: 2024 2827 2376 6572 6966 6963 6174 696f   $('#verificatio
-00003ae0: 6e2d 636f 6465 2d6d 6f64 616c 2729 2e6d  n-code-modal').m
-00003af0: 6f64 616c 287b 0a20 2020 2020 2020 2020  odal({.         
-00003b00: 2020 2020 2020 2020 2020 2062 6163 6b64             backd
-00003b10: 726f 703a 2027 7374 6174 6963 272c 0a20  rop: 'static',. 
-00003b20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003b30: 2020 206b 6579 626f 6172 643a 2066 616c     keyboard: fal
-00003b40: 7365 0a20 2020 2020 2020 2020 2020 2020  se.             
-00003b50: 2020 207d 290a 0a20 2020 2020 2020 2020     })..         
-00003b60: 2020 2020 2020 2024 2827 2373 6d61 7274         $('#smart
-00003b70: 6964 2d73 7465 7027 292e 7465 7874 2827  id-step').text('
-00003b80: 4175 7468 656e 7469 6361 7469 6f6e 2729  Authentication')
-00003b90: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00003ba0: 2024 2827 2373 6d61 7274 6964 2d76 6572   $('#smartid-ver
-00003bb0: 6966 6963 6174 696f 6e2d 636f 6465 2729  ification-code')
-00003bc0: 2e74 6578 7428 7265 7370 6f6e 7365 2e76  .text(response.v
-00003bd0: 6572 6966 6963 6174 696f 6e5f 636f 6465  erification_code
-00003be0: 290a 0a20 2020 2020 2020 2020 2020 2020  )..             
-00003bf0: 2020 202f 2f20 2e2e 2e6e 6578 7420 7068     // ...next ph
-00003c00: 6173 653a 2073 7461 7274 2073 6967 6e69  ase: start signi
-00003c10: 6e67 0a20 2020 2020 2020 2020 2020 2020  ng.             
-00003c20: 2020 202f 2f20 7765 2064 6f6e 2774 2077     // we don't w
-00003c30: 616e 7420 746f 2073 7461 7274 2070 6f6c  ant to start pol
-00003c40: 6c69 6e67 2069 6d6d 6564 6961 7465 6c79  ling immediately
-00003c50: 2062 6563 6175 7365 2075 7365 7220 7769   because user wi
-00003c60: 6c6c 206e 6565 6420 746f 2065 6e74 6572  ll need to enter
-00003c70: 2076 6572 6966 6963 6174 696f 6e20 636f   verification co
-00003c80: 6465 0a20 2020 2020 2020 2020 2020 2020  de.             
-00003c90: 2020 2073 6574 5469 6d65 6f75 7428 6675     setTimeout(fu
-00003ca0: 6e63 7469 6f6e 2028 2920 7b0a 2020 2020  nction () {.    
-00003cb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003cc0: 6d61 6e61 6765 722e 736d 6172 7469 6453  manager.smartidS
-00003cd0: 7461 7475 7328 292e 7468 656e 280a 2020  tatus().then(.  
-00003ce0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003cf0: 2020 2020 2020 6f6e 5374 6172 7453 6967        onStartSig
-00003d00: 6e2c 0a20 2020 2020 2020 2020 2020 2020  n,.             
-00003d10: 2020 2020 2020 2020 2020 206f 6e45 7272             onErr
-00003d20: 6f72 0a20 2020 2020 2020 2020 2020 2020  or.             
-00003d30: 2020 2020 2020 2029 2e66 696e 616c 6c79         ).finally
-00003d40: 280a 2020 2020 2020 2020 2020 2020 2020  (.              
-00003d50: 2020 2020 2020 2020 2020 2829 203d 3e20            () => 
-00003d60: 7374 6f70 5370 696e 6e65 7228 736d 6172  stopSpinner(smar
-00003d70: 7449 6446 6f72 6d29 0a20 2020 2020 2020  tIdForm).       
-00003d80: 2020 2020 2020 2020 2020 2020 2029 0a20               ). 
-00003d90: 2020 2020 2020 2020 2020 2020 2020 207d                 }
-00003da0: 2c20 7469 6d65 6f75 7446 6f72 5665 7269  , timeoutForVeri
-00003db0: 6669 6361 7469 6f6e 436f 6465 290a 2020  ficationCode).  
-00003dc0: 2020 2020 2020 2020 2020 7d0a 0a20 2020            }..   
-00003dd0: 2020 2020 2020 2020 2066 756e 6374 696f           functio
-00003de0: 6e20 6f6e 5374 6172 7453 6967 6e28 7265  n onStartSign(re
-00003df0: 7370 6f6e 7365 2920 7b0a 2020 2020 2020  sponse) {.      
-00003e00: 2020 2020 2020 2020 2020 2f2f 2047 6f74            // Got
-00003e10: 2061 2073 7563 6365 7373 6675 6c20 7369   a successful si
-00003e20: 676e 2d73 7461 7274 2072 6571 7565 7374  gn-start request
-00003e30: 2e2e 2e0a 2020 2020 2020 2020 2020 2020  ....            
-00003e40: 2020 2020 636f 6e73 6f6c 652e 6c6f 6728      console.log(
-00003e50: 2753 6d61 7274 4944 3a20 5369 676e 696e  'SmartID: Signin
-00003e60: 6720 7665 7269 6669 6361 7469 6f6e 2063  g verification c
-00003e70: 6f64 6527 2c20 7265 7370 6f6e 7365 2e76  ode', response.v
-00003e80: 6572 6966 6963 6174 696f 6e5f 636f 6465  erification_code
-00003e90: 290a 0a20 2020 2020 2020 2020 2020 2020  )..             
-00003ea0: 2020 2024 2827 2373 6d61 7274 6964 2d6d     $('#smartid-m
-00003eb0: 6f64 616c 2729 2e6d 6f64 616c 2827 6869  odal').modal('hi
-00003ec0: 6465 2729 0a0a 2020 2020 2020 2020 2020  de')..          
-00003ed0: 2020 2020 2020 2428 2723 7665 7269 6669        $('#verifi
-00003ee0: 6361 7469 6f6e 2d63 6f64 652d 6d6f 6461  cation-code-moda
-00003ef0: 6c27 292e 6d6f 6461 6c28 7b0a 2020 2020  l').modal({.    
-00003f00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003f10: 6261 636b 6472 6f70 3a20 2773 7461 7469  backdrop: 'stati
-00003f20: 6327 2c0a 2020 2020 2020 2020 2020 2020  c',.            
-00003f30: 2020 2020 2020 2020 6b65 7962 6f61 7264          keyboard
-00003f40: 3a20 6661 6c73 650a 2020 2020 2020 2020  : false.        
-00003f50: 2020 2020 2020 2020 7d29 0a0a 2020 2020          })..    
-00003f60: 2020 2020 2020 2020 2020 2020 2428 2723              $('#
-00003f70: 736d 6172 7469 642d 7374 6570 2729 2e74  smartid-step').t
-00003f80: 6578 7428 2753 6967 6e69 6e67 2729 0a20  ext('Signing'). 
-00003f90: 2020 2020 2020 2020 2020 2020 2020 2024                 $
-00003fa0: 2827 2373 6d61 7274 6964 2d76 6572 6966  ('#smartid-verif
-00003fb0: 6963 6174 696f 6e2d 636f 6465 2729 2e74  ication-code').t
-00003fc0: 6578 7428 7265 7370 6f6e 7365 2e76 6572  ext(response.ver
-00003fd0: 6966 6963 6174 696f 6e5f 636f 6465 290a  ification_code).
-00003fe0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00003ff0: 202f 2f20 2e2e 2e6e 6578 7420 7068 6173   // ...next phas
-00004000: 653a 2070 6f6c 6c20 666f 7220 7374 6174  e: poll for stat
-00004010: 7573 206f 6620 7369 676e 696e 670a 2020  us of signing.  
-00004020: 2020 2020 2020 2020 2020 2020 2020 7365                se
-00004030: 7454 696d 656f 7574 2866 756e 6374 696f  tTimeout(functio
-00004040: 6e20 2829 207b 0a20 2020 2020 2020 2020  n () {.         
-00004050: 2020 2020 2020 2020 2020 206d 616e 6167             manag
-00004060: 6572 2e73 6d61 7274 6964 5374 6174 7573  er.smartidStatus
-00004070: 2829 2e74 6865 6e28 0a20 2020 2020 2020  ().then(.       
-00004080: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004090: 206f 6e46 696e 6973 6853 6967 6e2c 0a20   onFinishSign,. 
-000040a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000040b0: 2020 2020 2020 206f 6e45 7272 6f72 0a20         onError. 
-000040c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000040d0: 2020 2029 0a20 2020 2020 2020 2020 2020     ).           
-000040e0: 2020 2020 207d 2c20 7469 6d65 6f75 7446       }, timeoutF
-000040f0: 6f72 5665 7269 6669 6361 7469 6f6e 436f  orVerificationCo
-00004100: 6465 290a 2020 2020 2020 2020 2020 2020  de).            
-00004110: 7d0a 0a20 2020 2020 2020 2020 2020 2066  }..            f
-00004120: 756e 6374 696f 6e20 6f6e 4669 6e69 7368  unction onFinish
-00004130: 5369 676e 2829 207b 0a20 2020 2020 2020  Sign() {.       
-00004140: 2020 2020 2020 2020 2024 2827 2373 6d61           $('#sma
-00004150: 7274 6964 2d6d 6f64 616c 2729 2e6d 6f64  rtid-modal').mod
-00004160: 616c 2822 6869 6465 2229 0a20 2020 2020  al("hide").     
-00004170: 2020 2020 2020 2020 2020 206f 6e53 6967             onSig
-00004180: 6e65 6428 290a 2020 2020 2020 2020 2020  ned().          
-00004190: 2020 7d0a 0a20 2020 2020 2020 2020 2020    }..           
-000041a0: 2065 2e70 7265 7665 6e74 4465 6661 756c   e.preventDefaul
-000041b0: 7428 290a 2020 2020 2020 2020 2020 2020  t().            
-000041c0: 7661 7220 6964 436f 6465 203d 2073 6d61  var idCode = sma
-000041d0: 7274 4964 466f 726d 2e69 645f 636f 6465  rtIdForm.id_code
-000041e0: 2e76 616c 7565 0a20 2020 2020 2020 2020  .value.         
-000041f0: 2020 2076 6172 2063 6f75 6e74 7279 203d     var country =
-00004200: 2073 6d61 7274 4964 466f 726d 2e63 6f75   smartIdForm.cou
-00004210: 6e74 7279 2e76 616c 7565 0a0a 2020 2020  ntry.value..    
-00004220: 2020 2020 2020 2020 6966 2028 2169 6443          if (!idC
-00004230: 6f64 6529 207b 0a20 2020 2020 2020 2020  ode) {.         
-00004240: 2020 2020 2020 2061 6c65 7274 2827 506c         alert('Pl
-00004250: 6561 7365 2065 6e74 6572 2061 6e20 4944  ease enter an ID
-00004260: 2063 6f64 6527 290a 2020 2020 2020 2020   code').        
-00004270: 2020 2020 2020 2020 7265 7475 726e 0a20          return. 
-00004280: 2020 2020 2020 2020 2020 207d 0a0a 2020             }..  
-00004290: 2020 2020 2020 2020 2020 636f 6e73 6f6c            consol
-000042a0: 652e 6c6f 6728 2753 6d61 7274 4944 3a20  e.log('SmartID: 
-000042b0: 7369 676e 696e 6720 7769 7468 2069 6420  signing with id 
-000042c0: 636f 6465 272c 2069 6443 6f64 652c 2027  code', idCode, '
-000042d0: 616e 6420 636f 756e 7472 7927 2c20 636f  and country', co
-000042e0: 756e 7472 7929 0a0a 2020 2020 2020 2020  untry)..        
-000042f0: 2020 2020 7374 6172 7453 7069 6e6e 6572      startSpinner
-00004300: 2873 6d61 7274 4964 466f 726d 290a 0a20  (smartIdForm).. 
-00004310: 2020 2020 2020 2020 2020 206d 616e 6167             manag
-00004320: 6572 2e73 6967 6e57 6974 6853 6d61 7274  er.signWithSmart
-00004330: 4964 287b 0a20 2020 2020 2020 2020 2020  Id({.           
-00004340: 2020 2020 2069 6443 6f64 652c 0a20 2020       idCode,.   
-00004350: 2020 2020 2020 2020 2020 2020 2063 6f75               cou
-00004360: 6e74 7279 2c0a 2020 2020 2020 2020 2020  ntry,.          
-00004370: 2020 7d29 2e74 6865 6e28 0a20 2020 2020    }).then(.     
-00004380: 2020 2020 2020 2020 2020 202f 2f20 5374             // St
-00004390: 6172 7420 6361 6c6c 6261 636b 2068 656c  art callback hel
-000043a0: 6c0a 2020 2020 2020 2020 2020 2020 2020  l.              
-000043b0: 2020 6f6e 5374 6172 7453 6967 6e2c 0a20    onStartSign,. 
-000043c0: 2020 2020 2020 2020 2020 2020 2020 206f                 o
-000043d0: 6e45 7272 6f72 0a20 2020 2020 2020 2020  nError.         
-000043e0: 2020 2029 2e66 696e 616c 6c79 280a 2020     ).finally(.  
-000043f0: 2020 2020 2020 2020 2020 2020 2020 2829                ()
-00004400: 203d 3e20 7374 6f70 5370 696e 6e65 7228   => stopSpinner(
-00004410: 736d 6172 7449 6446 6f72 6d29 0a20 2020  smartIdForm).   
-00004420: 2020 2020 2020 2020 2029 0a20 2020 2020           ).     
-00004430: 2020 207d 0a0a 2020 2020 2020 2020 2428     }..        $(
-00004440: 2723 7369 676e 2d69 6427 292e 6f6e 2827  '#sign-id').on('
-00004450: 636c 6963 6b27 2c20 6675 6e63 7469 6f6e  click', function
-00004460: 2028 6529 207b 0a20 2020 2020 2020 2020   (e) {.         
-00004470: 2020 2065 2e70 7265 7665 6e74 4465 6661     e.preventDefa
-00004480: 756c 7428 290a 0a20 2020 2020 2020 2020  ult()..         
-00004490: 2020 2024 2827 2369 642d 6d6f 6461 6c27     $('#id-modal'
-000044a0: 292e 6d6f 6461 6c28 7b0a 2020 2020 2020  ).modal({.      
-000044b0: 2020 2020 2020 2020 2020 6261 636b 6472            backdr
-000044c0: 6f70 3a20 2773 7461 7469 6327 2c0a 2020  op: 'static',.  
-000044d0: 2020 2020 2020 2020 2020 2020 2020 6b65                ke
-000044e0: 7962 6f61 7264 3a20 6661 6c73 650a 2020  yboard: false.  
-000044f0: 2020 2020 2020 2020 2020 7d29 0a0a 2020            })..  
-00004500: 2020 2020 2020 2020 2020 6d61 6e61 6765            manage
-00004510: 722e 7369 676e 5769 7468 4964 4361 7264  r.signWithIdCard
-00004520: 2829 2e74 6865 6e28 0a20 2020 2020 2020  ().then(.       
-00004530: 2020 2020 2020 2020 2066 756e 6374 696f           functio
-00004540: 6e20 2829 207b 0a20 2020 2020 2020 2020  n () {.         
-00004550: 2020 2020 2020 2020 2020 2024 2827 2369             $('#i
-00004560: 642d 6d6f 6461 6c27 292e 6d6f 6461 6c28  d-modal').modal(
-00004570: 2768 6964 6527 290a 2020 2020 2020 2020  'hide').        
-00004580: 2020 2020 2020 2020 2020 2020 6f6e 5369              onSi
-00004590: 676e 6564 2829 0a20 2020 2020 2020 2020  gned().         
-000045a0: 2020 2020 2020 207d 2c0a 0a20 2020 2020         },..     
-000045b0: 2020 2020 2020 2020 2020 2066 756e 6374             funct
-000045c0: 696f 6e20 2872 6573 2920 7b0a 2020 2020  ion (res) {.    
-000045d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000045e0: 6966 2028 7265 7320 696e 7374 616e 6365  if (res instance
-000045f0: 6f66 2045 7272 6f72 2920 7b0a 2020 2020  of Error) {.    
-00004600: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004610: 2020 2020 636f 6e73 6f6c 652e 6c6f 6728      console.log(
-00004620: 7265 732e 6d65 7373 6167 652c 2072 6573  res.message, res
-00004630: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
-00004640: 2020 2020 2020 2020 2020 7265 7320 3d20            res = 
-00004650: 6d61 6e61 6765 722e 6765 7445 7272 6f72  manager.getError
-00004660: 2872 6573 290a 0a20 2020 2020 2020 2020  (res)..         
-00004670: 2020 2020 2020 2020 2020 2020 2020 2061                 a
-00004680: 6c65 7274 2872 6573 2e6d 6573 7361 6765  lert(res.message
-00004690: 290a 0a20 2020 2020 2020 2020 2020 2020  )..             
-000046a0: 2020 2020 2020 2020 2020 2063 6f6e 736f             conso
-000046b0: 6c65 2e65 7272 6f72 2827 5b45 7272 6f72  le.error('[Error
-000046c0: 2063 6f64 653a 2027 202b 2072 6573 2e72   code: ' + res.r
-000046d0: 6574 7572 6e43 6f64 6520 2b20 273b 2045  eturnCode + '; E
-000046e0: 7272 6f72 3a20 2720 2b20 7265 732e 6d65  rror: ' + res.me
-000046f0: 7373 6167 6520 2b20 275d 2729 0a20 2020  ssage + ']').   
-00004700: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004710: 2020 2020 2024 2827 2369 642d 6d6f 6461       $('#id-moda
-00004720: 6c27 292e 6d6f 6461 6c28 2768 6964 6527  l').modal('hide'
-00004730: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
-00004740: 2020 2020 2020 7d20 656c 7365 207b 0a20        } else {. 
-00004750: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004760: 2020 2020 2020 2069 6620 2874 7970 656f         if (typeo
-00004770: 6620 7265 7320 3d3d 3d20 2773 7472 696e  f res === 'strin
-00004780: 6727 207c 7c20 7265 732e 6572 726f 725f  g' || res.error_
-00004790: 636f 6465 2920 7b0a 2020 2020 2020 2020  code) {.        
-000047a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000047b0: 2020 2020 7661 7220 6d73 6720 3d20 7265      var msg = re
-000047c0: 732e 6d65 7373 6167 6520 213d 3d20 756e  s.message !== un
-000047d0: 6465 6669 6e65 6420 3f20 7265 732e 6d65  defined ? res.me
-000047e0: 7373 6167 6520 3a20 7265 730a 0a20 2020  ssage : res..   
-000047f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004800: 2020 2020 2020 2020 2061 6c65 7274 286d           alert(m
-00004810: 7367 290a 2020 2020 2020 2020 2020 2020  sg).            
-00004820: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004830: 2428 2723 6964 2d6d 6f64 616c 2729 2e6d  $('#id-modal').m
-00004840: 6f64 616c 2827 6869 6465 2729 0a20 2020  odal('hide').   
-00004850: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004860: 2020 2020 207d 2065 6c73 6520 7b0a 2020       } else {.  
-00004870: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004880: 2020 2020 2020 2020 2020 636f 6e73 6f6c            consol
-00004890: 652e 6572 726f 7228 7265 732e 6d65 7373  e.error(res.mess
-000048a0: 6167 6520 213d 3d20 756e 6465 6669 6e65  age !== undefine
-000048b0: 6420 3f20 7265 732e 6d65 7373 6167 6520  d ? res.message 
-000048c0: 3a20 7265 7329 0a20 2020 2020 2020 2020  : res).         
-000048d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000048e0: 2020 2061 6c65 7274 2827 536f 6d65 7468     alert('Someth
-000048f0: 696e 6720 7765 6e74 2077 726f 6e67 2c20  ing went wrong, 
-00004900: 706c 6561 7365 2072 6566 7265 7368 2074  please refresh t
-00004910: 6865 2070 6167 6520 616e 6420 7472 7920  he page and try 
-00004920: 6167 6169 6e27 290a 2020 2020 2020 2020  again').        
-00004930: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004940: 7d0a 2020 2020 2020 2020 2020 2020 2020  }.              
-00004950: 2020 2020 2020 7d0a 2020 2020 2020 2020        }.        
-00004960: 2020 2020 2020 2020 7d0a 2020 2020 2020          }.      
-00004970: 2020 2020 2020 290a 2020 2020 2020 2020        ).        
-00004980: 7d29 0a0a 2020 2020 2020 2020 2428 2723  })..        $('#
-00004990: 6765 742d 646f 6375 6d65 6e74 2729 2e6f  get-document').o
-000049a0: 6e28 2763 6c69 636b 272c 2066 756e 6374  n('click', funct
-000049b0: 696f 6e20 2829 207b 0a20 2020 2020 2020  ion () {.       
-000049c0: 2020 2020 2073 6574 5469 6d65 6f75 7428       setTimeout(
-000049d0: 6675 6e63 7469 6f6e 2028 2920 7b0a 2020  function () {.  
-000049e0: 2020 2020 2020 2020 2020 2020 2020 7769                wi
-000049f0: 6e64 6f77 2e6c 6f63 6174 696f 6e2e 7265  ndow.location.re
-00004a00: 6c6f 6164 2829 0a20 2020 2020 2020 2020  load().         
-00004a10: 2020 207d 2c20 3230 3030 290a 2020 2020     }, 2000).    
-00004a20: 2020 2020 7d29 0a20 2020 207d 290a 0a3c      }).    })..<
-00004a30: 2f73 6372 6970 743e 0a0a 3c2f 626f 6479  /script>..</body
-00004a40: 3e0a 3c2f 6874 6d6c 3e0a                 >.</html>.
+00000fc0: 2020 2020 2020 2020 3c6c 6162 656c 2066          <label f
+00000fd0: 6f72 3d22 6964 436f 6465 496e 7075 7422  or="idCodeInput"
+00000fe0: 3e44 656d 6f20 4944 2063 6f64 653a 3c2f  >Demo ID code:</
+00000ff0: 6c61 6265 6c3e 0a20 2020 2020 2020 2020  label>.         
+00001000: 2020 2020 2020 2020 2020 2020 2020 203c                 <
+00001010: 696e 7075 7420 7479 7065 3d22 7465 7874  input type="text
+00001020: 2220 6e61 6d65 3d22 6964 5f63 6f64 6522  " name="id_code"
+00001030: 2069 643d 2269 6443 6f64 6549 6e70 7574   id="idCodeInput
+00001040: 2220 636c 6173 733d 2266 6f72 6d2d 636f  " class="form-co
+00001050: 6e74 726f 6c22 0a20 2020 2020 2020 2020  ntrol".         
+00001060: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001070: 2020 2020 2020 7661 6c75 653d 227b 7b20        value="{{ 
+00001080: 7265 7175 6573 742e 7365 7373 696f 6e2e  request.session.
+00001090: 6464 6f63 5f74 6573 745f 6964 5f63 6f64  ddoc_test_id_cod
+000010a0: 6520 7c20 6465 6661 756c 743a 2736 3030  e | default:'600
+000010b0: 3031 3031 3939 3036 2720 7d7d 2220 2f3e  01019906' }}" />
+000010c0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000010d0: 2020 2020 203c 2f64 6976 3e0a 2020 2020       </div>.    
+000010e0: 2020 2020 2020 2020 2020 2020 3c2f 666f              </fo
+000010f0: 726d 3e0a 2020 2020 2020 2020 2020 2020  rm>.            
+00001100: 3c2f 6469 763e 0a0a 2020 2020 2020 2020  </div>..        
+00001110: 2020 2020 3c64 6976 2063 6c61 7373 3d22      <div class="
+00001120: 6d6f 6461 6c2d 666f 6f74 6572 223e 0a20  modal-footer">. 
+00001130: 2020 2020 2020 2020 2020 2020 2020 203c                 <
+00001140: 6275 7474 6f6e 2074 7970 653d 2262 7574  button type="but
+00001150: 746f 6e22 2063 6c61 7373 3d22 6274 6e20  ton" class="btn 
+00001160: 6274 6e2d 7072 696d 6172 7922 2069 643d  btn-primary" id=
+00001170: 2273 6967 6e4d 6f62 696c 6522 3e53 6967  "signMobile">Sig
+00001180: 6e3c 2f62 7574 746f 6e3e 0a20 2020 2020  n</button>.     
+00001190: 2020 2020 2020 203c 2f64 6976 3e0a 2020         </div>.  
+000011a0: 2020 2020 2020 3c2f 6469 763e 0a20 2020        </div>.   
+000011b0: 203c 2f64 6976 3e0a 3c2f 6469 763e 0a0a   </div>.</div>..
+000011c0: 3c64 6976 2063 6c61 7373 3d22 6d6f 6461  <div class="moda
+000011d0: 6c20 6661 6465 2220 6964 3d22 6368 616c  l fade" id="chal
+000011e0: 6c65 6e67 652d 6d6f 6461 6c22 3e0a 2020  lenge-modal">.  
+000011f0: 2020 3c64 6976 2063 6c61 7373 3d22 6d6f    <div class="mo
+00001200: 6461 6c2d 6469 616c 6f67 223e 0a20 2020  dal-dialog">.   
+00001210: 2020 2020 203c 6469 7620 636c 6173 733d       <div class=
+00001220: 226d 6f64 616c 2d63 6f6e 7465 6e74 223e  "modal-content">
+00001230: 0a20 2020 2020 2020 2020 2020 203c 6469  .            <di
+00001240: 7620 636c 6173 733d 226d 6f64 616c 2d68  v class="modal-h
+00001250: 6561 6465 7222 3e0a 2020 2020 2020 2020  eader">.        
+00001260: 2020 2020 2020 2020 3c68 3420 636c 6173          <h4 clas
+00001270: 733d 226d 6f64 616c 2d74 6974 6c65 223e  s="modal-title">
+00001280: 4d49 4420 5374 6570 2032 3c2f 6834 3e0a  MID Step 2</h4>.
+00001290: 2020 2020 2020 2020 2020 2020 3c2f 6469              </di
+000012a0: 763e 0a0a 2020 2020 2020 2020 2020 2020  v>..            
+000012b0: 3c64 6976 2063 6c61 7373 3d22 6d6f 6461  <div class="moda
+000012c0: 6c2d 626f 6479 223e 0a20 2020 2020 2020  l-body">.       
+000012d0: 2020 2020 2020 2020 203c 703e 0a20 2020           <p>.   
+000012e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000012f0: 2050 6c65 6173 6520 656e 7465 7220 7468   Please enter th
+00001300: 6520 666f 6c6c 6f77 696e 6720 636f 6465  e following code
+00001310: 2069 6e74 6f20 796f 7572 206d 6f62 696c   into your mobil
+00001320: 6520 746f 2070 726f 6365 6564 2077 6974  e to proceed wit
+00001330: 680a 2020 2020 2020 2020 2020 2020 2020  h.              
+00001340: 2020 2020 2020 7468 6520 7369 676e 696e        the signin
+00001350: 6720 7072 6f63 6573 733a 203c 6220 6964  g process: <b id
+00001360: 3d22 6368 616c 6c65 6e67 652d 636f 6465  ="challenge-code
+00001370: 223e 4b4f 4f44 3c2f 623e 0a20 2020 2020  ">KOOD</b>.     
+00001380: 2020 2020 2020 2020 2020 203c 2f70 3e0a             </p>.
+00001390: 2020 2020 2020 2020 2020 2020 3c2f 6469              </di
+000013a0: 763e 0a20 2020 2020 2020 203c 2f64 6976  v>.        </div
+000013b0: 3e0a 2020 2020 3c2f 6469 763e 0a3c 2f64  >.    </div>.</d
+000013c0: 6976 3e0a 0a3c 6469 7620 636c 6173 733d  iv>..<div class=
+000013d0: 226d 6f64 616c 2066 6164 6522 2069 643d  "modal fade" id=
+000013e0: 2269 642d 6d6f 6461 6c22 3e0a 2020 2020  "id-modal">.    
+000013f0: 3c64 6976 2063 6c61 7373 3d22 6d6f 6461  <div class="moda
+00001400: 6c2d 6469 616c 6f67 223e 0a20 2020 2020  l-dialog">.     
+00001410: 2020 203c 6469 7620 636c 6173 733d 226d     <div class="m
+00001420: 6f64 616c 2d63 6f6e 7465 6e74 223e 0a20  odal-content">. 
+00001430: 2020 2020 2020 2020 2020 203c 6469 7620             <div 
+00001440: 636c 6173 733d 226d 6f64 616c 2d68 6561  class="modal-hea
+00001450: 6465 7222 3e0a 2020 2020 2020 2020 2020  der">.          
+00001460: 2020 2020 2020 3c68 3420 636c 6173 733d        <h4 class=
+00001470: 226d 6f64 616c 2d74 6974 6c65 223e 5369  "modal-title">Si
+00001480: 676e 696e 6720 7769 7468 2064 6967 6974  gning with digit
+00001490: 616c 2049 443c 2f68 343e 0a20 2020 2020  al ID</h4>.     
+000014a0: 2020 2020 2020 203c 2f64 6976 3e0a 0a20         </div>.. 
+000014b0: 2020 2020 2020 2020 2020 203c 6469 7620             <div 
+000014c0: 636c 6173 733d 226d 6f64 616c 2d62 6f64  class="modal-bod
+000014d0: 7922 3e0a 2020 2020 2020 2020 2020 2020  y">.            
+000014e0: 2020 2020 3c70 3e0a 2020 2020 2020 2020      <p>.        
+000014f0: 2020 2020 2020 2020 2020 2020 506c 6561              Plea
+00001500: 7365 2066 6f6c 6c6f 7720 7468 6520 696e  se follow the in
+00001510: 7374 7275 6374 696f 6e73 2074 6f20 636f  structions to co
+00001520: 6d70 6c65 7465 2074 6865 2073 6967 6e69  mplete the signi
+00001530: 6e67 2070 726f 6365 7373 2e0a 2020 2020  ng process..    
+00001540: 2020 2020 2020 2020 2020 2020 3c2f 703e              </p>
+00001550: 0a20 2020 2020 2020 2020 2020 203c 2f64  .            </d
+00001560: 6976 3e0a 2020 2020 2020 2020 3c2f 6469  iv>.        </di
+00001570: 763e 0a20 2020 203c 2f64 6976 3e0a 3c2f  v>.    </div>.</
+00001580: 6469 763e 0a0a 3c64 6976 2063 6c61 7373  div>..<div class
+00001590: 3d22 6d6f 6461 6c20 6661 6465 2220 6964  ="modal fade" id
+000015a0: 3d22 736d 6172 7469 642d 6d6f 6461 6c22  ="smartid-modal"
+000015b0: 3e0a 2020 2020 3c64 6976 2063 6c61 7373  >.    <div class
+000015c0: 3d22 6d6f 6461 6c2d 6469 616c 6f67 223e  ="modal-dialog">
+000015d0: 0a20 2020 2020 2020 203c 6469 7620 636c  .        <div cl
+000015e0: 6173 733d 226d 6f64 616c 2d63 6f6e 7465  ass="modal-conte
+000015f0: 6e74 223e 0a20 2020 2020 2020 2020 2020  nt">.           
+00001600: 203c 6469 7620 636c 6173 733d 226d 6f64   <div class="mod
+00001610: 616c 2d68 6561 6465 7222 3e0a 2020 2020  al-header">.    
+00001620: 2020 2020 2020 2020 2020 2020 3c62 7574              <but
+00001630: 746f 6e20 7479 7065 3d22 6275 7474 6f6e  ton type="button
+00001640: 2220 636c 6173 733d 2263 6c6f 7365 2220  " class="close" 
+00001650: 6461 7461 2d64 6973 6d69 7373 3d22 6d6f  data-dismiss="mo
+00001660: 6461 6c22 2061 7269 612d 6c61 6265 6c3d  dal" aria-label=
+00001670: 2243 6c6f 7365 223e 3c73 7061 6e20 6172  "Close"><span ar
+00001680: 6961 2d68 6964 6465 6e3d 2274 7275 6522  ia-hidden="true"
+00001690: 3e26 7469 6d65 733b 3c2f 7370 616e 3e0a  >&times;</span>.
+000016a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000016b0: 3c2f 6275 7474 6f6e 3e0a 2020 2020 2020  </button>.      
+000016c0: 2020 2020 2020 2020 2020 3c68 3420 636c            <h4 cl
+000016d0: 6173 733d 226d 6f64 616c 2d74 6974 6c65  ass="modal-title
+000016e0: 223e 5369 676e 2074 6865 2066 696c 6573  ">Sign the files
+000016f0: 2077 6974 6820 536d 6172 7449 443c 2f68   with SmartID</h
+00001700: 343e 0a20 2020 2020 2020 2020 2020 203c  4>.            <
+00001710: 2f64 6976 3e0a 0a20 2020 2020 2020 2020  /div>..         
+00001720: 2020 203c 6469 7620 636c 6173 733d 226d     <div class="m
+00001730: 6f64 616c 2d62 6f64 7922 3e0a 2020 2020  odal-body">.    
+00001740: 2020 2020 2020 2020 2020 2020 3c66 6f72              <for
+00001750: 6d20 6e61 6d65 3d22 736d 6172 7449 6422  m name="smartId"
+00001760: 3e0a 2020 2020 2020 2020 2020 2020 2020  >.              
+00001770: 2020 2020 2020 3c64 6976 2063 6c61 7373        <div class
+00001780: 3d22 666f 726d 2d67 726f 7570 223e 0a20  ="form-group">. 
+00001790: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000017a0: 2020 2020 2020 203c 6c61 6265 6c20 666f         <label fo
+000017b0: 723d 2269 6443 6f64 6549 6e70 7574 223e  r="idCodeInput">
+000017c0: 596f 7572 2049 4420 636f 6465 3a3c 2f6c  Your ID code:</l
+000017d0: 6162 656c 3e0a 2020 2020 2020 2020 2020  abel>.          
+000017e0: 2020 2020 2020 2020 2020 2020 2020 3c69                <i
+000017f0: 6e70 7574 2074 7970 653d 2274 6578 7422  nput type="text"
+00001800: 206e 616d 653d 2269 645f 636f 6465 2220   name="id_code" 
+00001810: 6964 3d22 6964 436f 6465 496e 7075 7422  id="idCodeInput"
+00001820: 2063 6c61 7373 3d22 666f 726d 2d63 6f6e   class="form-con
+00001830: 7472 6f6c 220a 2020 2020 2020 2020 2020  trol".          
+00001840: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001850: 2020 2020 2076 616c 7565 3d22 7b7b 2072       value="{{ r
+00001860: 6571 7565 7374 2e73 6573 7369 6f6e 2e73  equest.session.s
+00001870: 6d61 7274 6964 5f74 6573 745f 6964 5f63  martid_test_id_c
+00001880: 6f64 6520 7c20 6465 6661 756c 743a 2733  ode | default:'3
+00001890: 3033 3033 3033 3939 3134 2720 7d7d 2220  0303039914' }}" 
+000018a0: 2f3e 0a20 2020 2020 2020 2020 2020 2020  />.             
+000018b0: 2020 2020 2020 203c 2f64 6976 3e0a 2020         </div>.  
+000018c0: 2020 2020 2020 2020 2020 2020 2020 3c2f                </
+000018d0: 666f 726d 3e0a 2020 2020 2020 2020 2020  form>.          
+000018e0: 2020 3c2f 6469 763e 0a0a 2020 2020 2020    </div>..      
+000018f0: 2020 2020 2020 3c64 6976 2063 6c61 7373        <div class
+00001900: 3d22 6d6f 6461 6c2d 666f 6f74 6572 223e  ="modal-footer">
+00001910: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00001920: 203c 6275 7474 6f6e 2074 7970 653d 2262   <button type="b
+00001930: 7574 746f 6e22 2063 6c61 7373 3d22 6274  utton" class="bt
+00001940: 6e20 6274 6e2d 7072 696d 6172 7922 2069  n btn-primary" i
+00001950: 643d 2273 6967 6e2d 736d 6172 7469 642d  d="sign-smartid-
+00001960: 6275 7474 6f6e 223e 5369 676e 3c2f 6275  button">Sign</bu
+00001970: 7474 6f6e 3e0a 2020 2020 2020 2020 2020  tton>.          
+00001980: 2020 3c2f 6469 763e 0a20 2020 2020 2020    </div>.       
+00001990: 203c 2f64 6976 3e0a 2020 2020 3c2f 6469   </div>.    </di
+000019a0: 763e 0a3c 2f64 6976 3e0a 0a3c 6469 7620  v>.</div>..<div 
+000019b0: 636c 6173 733d 226d 6f64 616c 2066 6164  class="modal fad
+000019c0: 6522 2069 643d 2276 6572 6966 6963 6174  e" id="verificat
+000019d0: 696f 6e2d 636f 6465 2d6d 6f64 616c 223e  ion-code-modal">
+000019e0: 0a20 2020 203c 6469 7620 636c 6173 733d  .    <div class=
+000019f0: 226d 6f64 616c 2d64 6961 6c6f 6722 3e0a  "modal-dialog">.
+00001a00: 2020 2020 2020 2020 3c64 6976 2063 6c61          <div cla
+00001a10: 7373 3d22 6d6f 6461 6c2d 636f 6e74 656e  ss="modal-conten
+00001a20: 7422 3e0a 2020 2020 2020 2020 2020 2020  t">.            
+00001a30: 3c64 6976 2063 6c61 7373 3d22 6d6f 6461  <div class="moda
+00001a40: 6c2d 6865 6164 6572 223e 0a20 2020 2020  l-header">.     
+00001a50: 2020 2020 2020 2020 2020 203c 6834 2063             <h4 c
+00001a60: 6c61 7373 3d22 6d6f 6461 6c2d 7469 746c  lass="modal-titl
+00001a70: 6522 3e56 6572 6966 6963 6174 696f 6e20  e">Verification 
+00001a80: 636f 6465 3c2f 6834 3e0a 2020 2020 2020  code</h4>.      
+00001a90: 2020 2020 2020 3c2f 6469 763e 0a0a 2020        </div>..  
+00001aa0: 2020 2020 2020 2020 2020 3c64 6976 2063            <div c
+00001ab0: 6c61 7373 3d22 6d6f 6461 6c2d 626f 6479  lass="modal-body
+00001ac0: 223e 0a20 2020 2020 2020 2020 2020 2020  ">.             
+00001ad0: 2020 203c 703e 0a20 2020 2020 2020 2020     <p>.         
+00001ae0: 2020 2020 2020 2020 2020 204d 616b 6520             Make 
+00001af0: 7375 7265 2079 6f75 2061 7265 2073 6565  sure you are see
+00001b00: 696e 6720 7468 6973 2076 6572 6966 6963  ing this verific
+00001b10: 6174 696f 6e20 636f 6465 206f 6e20 796f  ation code on yo
+00001b20: 7572 2064 6576 6963 653a 0a20 2020 2020  ur device:.     
+00001b30: 2020 2020 2020 2020 2020 2020 2020 203c                 <
+00001b40: 6220 6964 3d22 736d 6172 7469 642d 7665  b id="smartid-ve
+00001b50: 7269 6669 6361 7469 6f6e 2d63 6f64 6522  rification-code"
+00001b60: 3e4b 4f4f 443c 2f62 3e0a 2020 2020 2020  >KOOD</b>.      
+00001b70: 2020 2020 2020 2020 2020 3c2f 703e 0a20            </p>. 
+00001b80: 2020 2020 2020 2020 2020 203c 2f64 6976             </div
+00001b90: 3e0a 2020 2020 2020 2020 3c2f 6469 763e  >.        </div>
+00001ba0: 0a20 2020 203c 2f64 6976 3e0a 3c2f 6469  .    </div>.</di
+00001bb0: 763e 0a0a 3c64 6976 2063 6c61 7373 3d22  v>..<div class="
+00001bc0: 6d6f 6461 6c20 6661 6465 2220 6964 3d22  modal fade" id="
+00001bd0: 7375 6363 6573 732d 6d6f 6461 6c22 3e0a  success-modal">.
+00001be0: 2020 2020 3c64 6976 2063 6c61 7373 3d22      <div class="
+00001bf0: 6d6f 6461 6c2d 6469 616c 6f67 223e 0a20  modal-dialog">. 
+00001c00: 2020 2020 2020 203c 6469 7620 636c 6173         <div clas
+00001c10: 733d 226d 6f64 616c 2d63 6f6e 7465 6e74  s="modal-content
+00001c20: 223e 0a20 2020 2020 2020 2020 2020 203c  ">.            <
+00001c30: 6469 7620 636c 6173 733d 226d 6f64 616c  div class="modal
+00001c40: 2d68 6561 6465 7222 3e0a 2020 2020 2020  -header">.      
+00001c50: 2020 2020 2020 2020 2020 3c68 3420 636c            <h4 cl
+00001c60: 6173 733d 226d 6f64 616c 2d74 6974 6c65  ass="modal-title
+00001c70: 223e 5369 676e 696e 6720 636f 6d70 6c65  ">Signing comple
+00001c80: 7465 3c2f 6834 3e0a 2020 2020 2020 2020  te</h4>.        
+00001c90: 2020 2020 3c2f 6469 763e 0a0a 2020 2020      </div>..    
+00001ca0: 2020 2020 2020 2020 3c64 6976 2063 6c61          <div cla
+00001cb0: 7373 3d22 6d6f 6461 6c2d 626f 6479 223e  ss="modal-body">
+00001cc0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00001cd0: 203c 703e 0a20 2020 2020 2020 2020 2020   <p>.           
+00001ce0: 2020 2020 2020 2020 2054 6865 2075 706c           The upl
+00001cf0: 6f61 6465 6420 6669 6c65 7320 7765 7265  oaded files were
+00001d00: 2073 7563 6365 7373 6675 6c6c 7920 6469   successfully di
+00001d10: 6769 7461 6c6c 7920 7369 676e 6564 2c20  gitally signed, 
+00001d20: 706c 6561 7365 2063 6c69 636b 2074 6865  please click the
+00001d30: 2066 6f6c 6c6f 7769 6e67 206c 696e 6b0a   following link.
+00001d40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001d50: 2020 2020 746f 2064 6f77 6e6c 6f61 6420      to download 
+00001d60: 7468 6520 636f 6e74 6169 6e65 7220 616e  the container an
+00001d70: 6420 6669 6e69 7368 2074 6865 2073 6967  d finish the sig
+00001d80: 6e69 6e67 2070 726f 6365 7373 2e0a 2020  ning process..  
+00001d90: 2020 2020 2020 2020 2020 2020 2020 3c2f                </
+00001da0: 703e 0a0a 2020 2020 2020 2020 2020 2020  p>..            
+00001db0: 2020 2020 3c61 2068 7265 663d 2223 2220      <a href="#" 
+00001dc0: 6964 3d22 6765 742d 646f 6375 6d65 6e74  id="get-document
+00001dd0: 2220 7461 7267 6574 3d22 5f62 6c61 6e6b  " target="_blank
+00001de0: 223e 446f 776e 6c6f 6164 2066 696c 653c  ">Download file<
+00001df0: 2f61 3e0a 2020 2020 2020 2020 2020 2020  /a>.            
+00001e00: 3c2f 6469 763e 0a20 2020 2020 2020 203c  </div>.        <
+00001e10: 2f64 6976 3e0a 2020 2020 3c2f 6469 763e  /div>.    </div>
+00001e20: 0a3c 2f64 6976 3e0a 0a3c 7363 7269 7074  .</div>..<script
+00001e30: 2073 7263 3d22 2f2f 616a 6178 2e67 6f6f   src="//ajax.goo
+00001e40: 676c 6561 7069 732e 636f 6d2f 616a 6178  gleapis.com/ajax
+00001e50: 2f6c 6962 732f 6a71 7565 7279 2f31 2e31  /libs/jquery/1.1
+00001e60: 312e 312f 6a71 7565 7279 2e6d 696e 2e6a  1.1/jquery.min.j
+00001e70: 7322 3e3c 2f73 6372 6970 743e 0a3c 7363  s"></script>.<sc
+00001e80: 7269 7074 2073 7263 3d22 2f2f 6d61 7863  ript src="//maxc
+00001e90: 646e 2e62 6f6f 7473 7472 6170 6364 6e2e  dn.bootstrapcdn.
+00001ea0: 636f 6d2f 626f 6f74 7374 7261 702f 332e  com/bootstrap/3.
+00001eb0: 332e 342f 6a73 2f62 6f6f 7473 7472 6170  3.4/js/bootstrap
+00001ec0: 2e6d 696e 2e6a 7322 3e3c 2f73 6372 6970  .min.js"></scrip
+00001ed0: 743e 0a0a 3c73 6372 6970 7420 7479 7065  t>..<script type
+00001ee0: 3d22 7465 7874 2f6a 6176 6173 6372 6970  ="text/javascrip
+00001ef0: 7422 2073 7263 3d22 7b25 2073 7461 7469  t" src="{% stati
+00001f00: 6320 2765 7374 6569 642d 6865 6c70 6572  c 'esteid-helper
+00001f10: 2f77 6562 2d65 6964 2e6a 7327 2025 7d22  /web-eid.js' %}"
+00001f20: 3e3c 2f73 6372 6970 743e 0a3c 7363 7269  ></script>.<scri
+00001f30: 7074 2074 7970 653d 2274 6578 742f 6a61  pt type="text/ja
+00001f40: 7661 7363 7269 7074 2220 7372 633d 227b  vascript" src="{
+00001f50: 2520 7374 6174 6963 2027 6573 7465 6964  % static 'esteid
+00001f60: 2d68 656c 7065 722f 4573 7465 6964 2e6d  -helper/Esteid.m
+00001f70: 6169 6e2e 7765 622e 6a73 2720 257d 223e  ain.web.js' %}">
+00001f80: 3c2f 7363 7269 7074 3e0a 0a3c 7363 7269  </script>..<scri
+00001f90: 7074 2074 7970 653d 2274 6578 742f 6a61  pt type="text/ja
+00001fa0: 7661 7363 7269 7074 223e 0a20 2020 2024  vascript">.    $
+00001fb0: 2866 756e 6374 696f 6e20 2829 207b 0a20  (function () {. 
+00001fc0: 2020 2020 2020 2076 6172 2063 7372 665f         var csrf_
+00001fd0: 746f 6b65 6e20 3d20 277b 7b20 6373 7266  token = '{{ csrf
+00001fe0: 5f74 6f6b 656e 207d 7d27 0a20 2020 2020  _token }}'.     
+00001ff0: 2020 2076 6172 2064 6f77 6e6c 6f61 6455     var downloadU
+00002000: 726c 203d 2027 7b25 2075 726c 2027 646f  rl = '{% url 'do
+00002010: 776e 6c6f 6164 5f73 6967 6e65 645f 636f  wnload_signed_co
+00002020: 6e74 6169 6e65 7227 2025 7d27 0a20 2020  ntainer' %}'.   
+00002030: 2020 2020 2076 6172 206d 616e 6167 6572       var manager
+00002040: 203d 206e 6577 2045 7374 6569 642e 4c65   = new Esteid.Le
+00002050: 6761 6379 4964 656e 7469 6669 6361 7469  gacyIdentificati
+00002060: 6f6e 4d61 6e61 6765 7228 7b0a 2020 2020  onManager({.    
+00002070: 2020 2020 2020 2020 6c61 6e67 7561 6765          language
+00002080: 3a20 4573 7465 6964 2e4c 616e 6775 6167  : Esteid.Languag
+00002090: 6573 2e45 542c 0a0a 2020 2020 2020 2020  es.ET,..        
+000020a0: 2020 2020 6964 456e 6470 6f69 6e74 733a      idEndpoints:
+000020b0: 207b 0a20 2020 2020 2020 2020 2020 2020   {.             
+000020c0: 2020 2073 7461 7274 3a20 277b 2520 7572     start: '{% ur
+000020d0: 6c20 2774 6573 745f 6964 5f73 7461 7274  l 'test_id_start
+000020e0: 2720 257d 272c 0a20 2020 2020 2020 2020  ' %}',.         
+000020f0: 2020 2020 2020 2066 696e 6973 683a 2027         finish: '
+00002100: 7b25 2075 726c 2027 7465 7374 5f69 645f  {% url 'test_id_
+00002110: 6669 6e69 7368 2720 257d 272c 0a20 2020  finish' %}',.   
+00002120: 2020 2020 2020 2020 207d 2c0a 0a20 2020           },..   
+00002130: 2020 2020 2020 2020 206d 6964 456e 6470           midEndp
+00002140: 6f69 6e74 733a 207b 0a20 2020 2020 2020  oints: {.       
+00002150: 2020 2020 2020 2020 2073 7461 7274 3a20           start: 
+00002160: 277b 2520 7572 6c20 2774 6573 745f 6d69  '{% url 'test_mi
+00002170: 645f 7374 6172 7427 2025 7d27 2c0a 2020  d_start' %}',.  
+00002180: 2020 2020 2020 2020 2020 2020 2020 7374                st
+00002190: 6174 7573 3a20 277b 2520 7572 6c20 2774  atus: '{% url 't
+000021a0: 6573 745f 6d69 645f 7374 6174 7573 2720  est_mid_status' 
+000021b0: 257d 272c 0a20 2020 2020 2020 2020 2020  %}',.           
+000021c0: 207d 2c0a 0a20 2020 2020 2020 2020 2020   },..           
+000021d0: 2073 6d61 7274 6964 456e 6470 6f69 6e74   smartidEndpoint
+000021e0: 733a 207b 0a20 2020 2020 2020 2020 2020  s: {.           
+000021f0: 2020 2020 2073 7461 7274 3a20 277b 2520       start: '{% 
+00002200: 7572 6c20 2774 6573 745f 736d 6172 7469  url 'test_smarti
+00002210: 645f 7374 6172 7427 2025 7d27 2c0a 2020  d_start' %}',.  
+00002220: 2020 2020 2020 2020 2020 2020 2020 7374                st
+00002230: 6174 7573 3a20 277b 2520 7572 6c20 2774  atus: '{% url 't
+00002240: 6573 745f 736d 6172 7469 645f 7374 6174  est_smartid_stat
+00002250: 7573 2720 257d 272c 0a20 2020 2020 2020  us' %}',.       
+00002260: 2020 2020 207d 0a20 2020 2020 2020 207d       }.        }
+00002270: 290a 0a20 2020 2020 2020 2066 756e 6374  )..        funct
+00002280: 696f 6e20 6f6e 5369 676e 6564 2829 207b  ion onSigned() {
+00002290: 0a20 2020 2020 2020 2020 2020 2024 2827  .            $('
+000022a0: 2367 6574 2d64 6f63 756d 656e 7427 292e  #get-document').
+000022b0: 6174 7472 2827 6872 6566 272c 2064 6f77  attr('href', dow
+000022c0: 6e6c 6f61 6455 726c 290a 0a20 2020 2020  nloadUrl)..     
+000022d0: 2020 2020 2020 2024 2827 2373 7563 6365         $('#succe
+000022e0: 7373 2d6d 6f64 616c 2729 2e6d 6f64 616c  ss-modal').modal
+000022f0: 287b 0a20 2020 2020 2020 2020 2020 2020  ({.             
+00002300: 2020 2062 6163 6b64 726f 703a 2027 7374     backdrop: 'st
+00002310: 6174 6963 272c 0a20 2020 2020 2020 2020  atic',.         
+00002320: 2020 2020 2020 206b 6579 626f 6172 643a         keyboard:
+00002330: 2066 616c 7365 0a20 2020 2020 2020 2020   false.         
+00002340: 2020 207d 290a 2020 2020 2020 2020 7d0a     }).        }.
+00002350: 0a20 2020 2020 2020 2024 2827 2373 6967  .        $('#sig
+00002360: 6e2d 6d69 6427 292e 6f6e 2827 636c 6963  n-mid').on('clic
+00002370: 6b27 2c20 6675 6e63 7469 6f6e 2028 6529  k', function (e)
+00002380: 207b 0a20 2020 2020 2020 2020 2020 2065   {.            e
+00002390: 2e70 7265 7665 6e74 4465 6661 756c 7428  .preventDefault(
+000023a0: 290a 0a20 2020 2020 2020 2020 2020 2024  )..            $
+000023b0: 2827 236d 6964 2d6d 6f64 616c 2729 2e6d  ('#mid-modal').m
+000023c0: 6f64 616c 2829 0a20 2020 2020 2020 207d  odal().        }
+000023d0: 290a 0a20 2020 2020 2020 2066 756e 6374  )..        funct
+000023e0: 696f 6e20 7369 676e 4d6f 6269 6c65 4944  ion signMobileID
+000023f0: 2865 2920 7b0a 2020 2020 2020 2020 2020  (e) {.          
+00002400: 2020 652e 7072 6576 656e 7444 6566 6175    e.preventDefau
+00002410: 6c74 2829 0a20 2020 2020 2020 2020 2020  lt().           
+00002420: 2076 6172 206d 6f62 696c 6549 6446 6f72   var mobileIdFor
+00002430: 6d20 3d20 646f 6375 6d65 6e74 2e66 6f72  m = document.for
+00002440: 6d73 2e6d 6f62 696c 6549 640a 2020 2020  ms.mobileId.    
+00002450: 2020 2020 2020 2020 7661 7220 7068 6f6e          var phon
+00002460: 654e 7220 3d20 6d6f 6269 6c65 4964 466f  eNr = mobileIdFo
+00002470: 726d 2e70 686f 6e65 5f6e 722e 7661 6c75  rm.phone_nr.valu
+00002480: 650a 2020 2020 2020 2020 2020 2020 7661  e.            va
+00002490: 7220 6964 436f 6465 203d 206d 6f62 696c  r idCode = mobil
+000024a0: 6549 6446 6f72 6d2e 6964 5f63 6f64 652e  eIdForm.id_code.
+000024b0: 7661 6c75 650a 0a20 2020 2020 2020 2020  value..         
+000024c0: 2020 2069 6620 2821 7068 6f6e 654e 7229     if (!phoneNr)
+000024d0: 207b 0a20 2020 2020 2020 2020 2020 2020   {.             
+000024e0: 2020 2061 6c65 7274 2827 506c 6561 7365     alert('Please
+000024f0: 2065 6e74 6572 2061 2070 686f 6e65 206e   enter a phone n
+00002500: 756d 6265 7227 290a 2020 2020 2020 2020  umber').        
+00002510: 2020 2020 2020 2020 7265 7475 726e 0a20          return. 
+00002520: 2020 2020 2020 2020 2020 207d 0a20 2020             }.   
+00002530: 2020 2020 2020 2020 2069 6620 2821 6964           if (!id
+00002540: 436f 6465 2920 7b0a 2020 2020 2020 2020  Code) {.        
+00002550: 2020 2020 2020 2020 616c 6572 7428 2750          alert('P
+00002560: 6c65 6173 6520 656e 7465 7220 616e 2049  lease enter an I
+00002570: 4420 636f 6465 2729 0a20 2020 2020 2020  D code').       
+00002580: 2020 2020 2020 2020 2072 6574 7572 6e0a           return.
+00002590: 2020 2020 2020 2020 2020 2020 7d0a 0a20              }.. 
+000025a0: 2020 2020 2020 2020 2020 2063 6f6e 736f             conso
+000025b0: 6c65 2e6c 6f67 2827 4d49 443a 2073 6967  le.log('MID: sig
+000025c0: 6e69 6e67 2077 6974 6820 7068 6f6e 654e  ning with phoneN
+000025d0: 7227 2c20 7068 6f6e 654e 722c 2027 616e  r', phoneNr, 'an
+000025e0: 6420 6964 2063 6f64 6527 2c20 6964 436f  d id code', idCo
+000025f0: 6465 290a 0a20 2020 2020 2020 2020 2020  de)..           
+00002600: 202f 2f20 4361 6c6c 2049 6465 6e74 6966   // Call Identif
+00002610: 6963 6174 696f 6e4d 616e 6167 6572 2e73  icationManager.s
+00002620: 6967 6e20 7768 6963 6820 6361 6c6c 7320  ign which calls 
+00002630: 7468 6520 6261 636b 656e 6420 656e 6470  the backend endp
+00002640: 6f69 6e74 2074 6f20 7374 6172 7420 6d6f  oint to start mo
+00002650: 6269 6c65 4964 2073 6967 6e69 6e67 2070  bileId signing p
+00002660: 726f 6365 7373 0a20 2020 2020 2020 2020  rocess.         
+00002670: 2020 206d 616e 6167 6572 2e73 6967 6e57     manager.signW
+00002680: 6974 684d 6f62 696c 6549 6428 7b0a 2020  ithMobileId({.  
+00002690: 2020 2020 2020 2020 2020 2020 2020 7068                ph
+000026a0: 6f6e 655f 6e72 3a20 7068 6f6e 654e 722c  one_nr: phoneNr,
+000026b0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000026c0: 2069 645f 636f 6465 3a20 6964 436f 6465   id_code: idCode
+000026d0: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+000026e0: 2020 6373 7266 6d69 6464 6c65 7761 7265    csrfmiddleware
+000026f0: 746f 6b65 6e3a 2063 7372 665f 746f 6b65  token: csrf_toke
+00002700: 6e0a 2020 2020 2020 2020 2020 2020 7d29  n.            })
+00002710: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00002720: 202e 7468 656e 2866 756e 6374 696f 6e20   .then(function 
+00002730: 2872 6573 706f 6e73 6529 207b 0a20 2020  (response) {.   
+00002740: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002750: 2063 6f6e 736f 6c65 2e6c 6f67 2827 4d49   console.log('MI
+00002760: 443a 2067 6f74 2076 6572 6966 6963 6174  D: got verificat
+00002770: 696f 6e20 636f 6465 272c 2072 6573 706f  ion code', respo
+00002780: 6e73 652e 7665 7269 6669 6361 7469 6f6e  nse.verification
+00002790: 5f63 6f64 6529 0a0a 2020 2020 2020 2020  _code)..        
+000027a0: 2020 2020 2020 2020 2020 2020 2f2f 2047              // G
+000027b0: 6f74 2072 6573 706f 6e73 652c 2073 686f  ot response, sho
+000027c0: 7720 6368 616c 6c65 6e67 6520 6d6f 6461  w challenge moda
+000027d0: 6c0a 2020 2020 2020 2020 2020 2020 2020  l.              
+000027e0: 2020 2020 2020 2428 2723 6368 616c 6c65        $('#challe
+000027f0: 6e67 652d 636f 6465 2729 2e74 6578 7428  nge-code').text(
+00002800: 7265 7370 6f6e 7365 2e76 6572 6966 6963  response.verific
+00002810: 6174 696f 6e5f 636f 6465 290a 2020 2020  ation_code).    
+00002820: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002830: 2428 2723 6368 616c 6c65 6e67 652d 6d6f  $('#challenge-mo
+00002840: 6461 6c27 292e 6d6f 6461 6c28 7b0a 2020  dal').modal({.  
+00002850: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002860: 2020 2020 2020 6261 636b 6472 6f70 3a20        backdrop: 
+00002870: 2773 7461 7469 6327 2c0a 2020 2020 2020  'static',.      
+00002880: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002890: 2020 6b65 7962 6f61 7264 3a20 6661 6c73    keyboard: fals
+000028a0: 650a 2020 2020 2020 2020 2020 2020 2020  e.              
+000028b0: 2020 2020 2020 7d29 0a0a 2020 2020 2020        })..      
+000028c0: 2020 2020 2020 2020 2020 2020 2020 2428                $(
+000028d0: 2723 6d69 642d 6d6f 6461 6c27 292e 6d6f  '#mid-modal').mo
+000028e0: 6461 6c28 2768 6964 6527 290a 0a20 2020  dal('hide')..   
+000028f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002900: 206d 616e 6167 6572 2e6d 6964 5374 6174   manager.midStat
+00002910: 7573 287b 6373 7266 6d69 6464 6c65 7761  us({csrfmiddlewa
+00002920: 7265 746f 6b65 6e3a 2063 7372 665f 746f  retoken: csrf_to
+00002930: 6b65 6e7d 292e 7468 656e 280a 2020 2020  ken}).then(.    
+00002940: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002950: 2020 2020 6675 6e63 7469 6f6e 2028 2920      function () 
+00002960: 7b0a 2020 2020 2020 2020 2020 2020 2020  {.              
+00002970: 2020 2020 2020 2020 2020 2020 2020 2428                $(
+00002980: 2723 6368 616c 6c65 6e67 652d 6d6f 6461  '#challenge-moda
+00002990: 6c27 292e 6d6f 6461 6c28 2768 6964 6527  l').modal('hide'
+000029a0: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
+000029b0: 2020 2020 2020 2020 2020 2020 2020 6f6e                on
+000029c0: 5369 676e 6564 2829 0a20 2020 2020 2020  Signed().       
+000029d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000029e0: 207d 2c0a 0a20 2020 2020 2020 2020 2020   },..           
+000029f0: 2020 2020 2020 2020 2020 2020 2066 756e               fun
+00002a00: 6374 696f 6e20 2872 6573 2920 7b0a 2020  ction (res) {.  
+00002a10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002a20: 2020 2020 2020 2020 2020 6966 2028 7265            if (re
+00002a30: 732e 6d65 7373 6167 6529 207b 0a20 2020  s.message) {.   
+00002a40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002a50: 2020 2020 2020 2020 2020 2020 2061 6c65               ale
+00002a60: 7274 2872 6573 2e6d 6573 7361 6765 202b  rt(res.message +
+00002a70: 2027 2050 6c65 6173 6520 7472 7920 6167   ' Please try ag
+00002a80: 6169 6e27 290a 2020 2020 2020 2020 2020  ain').          
+00002a90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002aa0: 2020 7d20 656c 7365 207b 0a20 2020 2020    } else {.     
+00002ab0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002ac0: 2020 2020 2020 2020 2020 2061 6c65 7274             alert
+00002ad0: 2827 536f 6d65 7468 696e 6720 7765 6e74  ('Something went
+00002ae0: 2077 726f 6e67 2c20 706c 6561 7365 2074   wrong, please t
+00002af0: 7279 2061 6761 696e 2729 0a20 2020 2020  ry again').     
+00002b00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002b10: 2020 2020 2020 207d 0a0a 2020 2020 2020         }..      
+00002b20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002b30: 2020 2020 2020 2428 2723 6368 616c 6c65        $('#challe
+00002b40: 6e67 652d 6d6f 6461 6c27 292e 6d6f 6461  nge-modal').moda
+00002b50: 6c28 2768 6964 6527 290a 2020 2020 2020  l('hide').      
+00002b60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002b70: 2020 7d0a 2020 2020 2020 2020 2020 2020    }.            
+00002b80: 2020 2020 2020 2020 290a 0a20 2020 2020          )..     
+00002b90: 2020 2020 2020 2020 2020 207d 2c20 6675             }, fu
+00002ba0: 6e63 7469 6f6e 2028 7265 7329 207b 0a20  nction (res) {. 
+00002bb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002bc0: 2020 2069 6620 2872 6573 2026 2620 7265     if (res && re
+00002bd0: 732e 6d65 7373 6167 6529 207b 0a20 2020  s.message) {.   
+00002be0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002bf0: 2020 2020 2061 6c65 7274 2827 4d49 4420       alert('MID 
+00002c00: 5265 7370 6f6e 7365 5b27 202b 2072 6573  Response[' + res
+00002c10: 2e65 7272 6f72 5f63 6f64 6520 2b20 275d  .error_code + ']
+00002c20: 3a20 2720 2b20 7265 732e 6d65 7373 6167  : ' + res.messag
+00002c30: 6529 0a20 2020 2020 2020 2020 2020 2020  e).             
+00002c40: 2020 2020 2020 207d 2065 6c73 6520 7b0a         } else {.
+00002c50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002c60: 2020 2020 2020 2020 616c 6572 7428 2753          alert('S
+00002c70: 6f6d 6574 6869 6e67 2077 656e 7420 7772  omething went wr
+00002c80: 6f6e 672c 2070 6c65 6173 6520 7472 7920  ong, please try 
+00002c90: 6167 6169 6e27 290a 2020 2020 2020 2020  again').        
+00002ca0: 2020 2020 2020 2020 2020 2020 7d0a 2020              }.  
+00002cb0: 2020 2020 2020 2020 2020 2020 2020 7d29                })
+00002cc0: 0a20 2020 2020 2020 207d 0a0a 2020 2020  .        }..    
+00002cd0: 2020 2020 2428 2723 7369 676e 2d73 6d61      $('#sign-sma
+00002ce0: 7274 6964 2729 2e6f 6e28 2763 6c69 636b  rtid').on('click
+00002cf0: 272c 2066 756e 6374 696f 6e20 2865 2920  ', function (e) 
+00002d00: 7b0a 2020 2020 2020 2020 2020 2020 652e  {.            e.
+00002d10: 7072 6576 656e 7444 6566 6175 6c74 2829  preventDefault()
+00002d20: 0a0a 2020 2020 2020 2020 2020 2020 2428  ..            $(
+00002d30: 2723 736d 6172 7469 642d 6d6f 6461 6c27  '#smartid-modal'
+00002d40: 292e 6d6f 6461 6c28 290a 2020 2020 2020  ).modal().      
+00002d50: 2020 7d29 0a0a 2020 2020 2020 2020 6675    })..        fu
+00002d60: 6e63 7469 6f6e 206f 6e45 7272 6f72 2872  nction onError(r
+00002d70: 6573 2920 7b0a 2020 2020 2020 2020 2020  es) {.          
+00002d80: 2020 6966 2028 7265 7320 2626 2072 6573    if (res && res
+00002d90: 2e6d 6573 7361 6765 2920 7b0a 2020 2020  .message) {.    
+00002da0: 2020 2020 2020 2020 2020 2020 616c 6572              aler
+00002db0: 7428 2753 6d61 7274 4944 2052 6573 706f  t('SmartID Respo
+00002dc0: 6e73 655b 2720 2b20 2872 6573 2e65 7272  nse[' + (res.err
+00002dd0: 6f72 5f63 6f64 6520 7c7c 2027 756e 6b6e  or_code || 'unkn
+00002de0: 6f77 6e27 2920 2b20 275d 3a20 2720 2b20  own') + ']: ' + 
+00002df0: 7265 732e 6d65 7373 6167 6529 0a20 2020  res.message).   
+00002e00: 2020 2020 2020 2020 207d 2065 6c73 6520           } else 
+00002e10: 7b0a 2020 2020 2020 2020 2020 2020 2020  {.              
+00002e20: 2020 636f 6e73 6f6c 652e 6c6f 6728 2245    console.log("E
+00002e30: 7272 6f72 3a22 2c20 7265 7329 0a20 2020  rror:", res).   
+00002e40: 2020 2020 2020 2020 2020 2020 2061 6c65               ale
+00002e50: 7274 2827 536f 6d65 7468 696e 6720 7765  rt('Something we
+00002e60: 6e74 2077 726f 6e67 2c20 706c 6561 7365  nt wrong, please
+00002e70: 2074 7279 2061 6761 696e 2729 0a20 2020   try again').   
+00002e80: 2020 2020 2020 2020 207d 0a20 2020 2020           }.     
+00002e90: 2020 207d 0a0a 2020 2020 2020 2020 6675     }..        fu
+00002ea0: 6e63 7469 6f6e 2073 6967 6e53 6d61 7274  nction signSmart
+00002eb0: 4944 2865 2920 7b0a 2020 2020 2020 2020  ID(e) {.        
+00002ec0: 2020 2020 636f 6e73 6f6c 652e 6c6f 6728      console.log(
+00002ed0: 2253 6967 6e69 6e67 2077 6974 6820 536d  "Signing with Sm
+00002ee0: 6172 7420 4944 2229 0a20 2020 2020 2020  art ID").       
+00002ef0: 2020 2020 2065 2e70 7265 7665 6e74 4465       e.preventDe
+00002f00: 6661 756c 7428 290a 0a20 2020 2020 2020  fault()..       
+00002f10: 2020 2020 2076 6172 2074 696d 656f 7574       var timeout
+00002f20: 466f 7256 6572 6966 6963 6174 696f 6e43  ForVerificationC
+00002f30: 6f64 6520 3d20 3230 3030 2020 2f2f 2064  ode = 2000  // d
+00002f40: 656c 6179 2070 6f6c 6c69 6e67 2074 6f20  elay polling to 
+00002f50: 6c65 7420 7573 6572 2074 6f20 656e 7465  let user to ente
+00002f60: 7220 7665 7269 6669 6361 7469 6f6e 2063  r verification c
+00002f70: 6f64 650a 0a20 2020 2020 2020 2020 2020  ode..           
+00002f80: 2066 756e 6374 696f 6e20 6f6e 5374 6172   function onStar
+00002f90: 7453 6967 6e28 7265 7370 6f6e 7365 2920  tSign(response) 
+00002fa0: 7b0a 2020 2020 2020 2020 2020 2020 2020  {.              
+00002fb0: 2020 2f2f 2047 6f74 2061 2073 7563 6365    // Got a succe
+00002fc0: 7373 6675 6c20 7369 676e 2d73 7461 7274  ssful sign-start
+00002fd0: 2072 6571 7565 7374 2e2e 2e0a 2020 2020   request....    
+00002fe0: 2020 2020 2020 2020 2020 2020 636f 6e73              cons
+00002ff0: 6f6c 652e 6c6f 6728 2753 6d61 7274 4944  ole.log('SmartID
+00003000: 3a20 5369 676e 696e 6720 7665 7269 6669  : Signing verifi
+00003010: 6361 7469 6f6e 2063 6f64 6527 2c20 7265  cation code', re
+00003020: 7370 6f6e 7365 2e76 6572 6966 6963 6174  sponse.verificat
+00003030: 696f 6e5f 636f 6465 290a 0a20 2020 2020  ion_code)..     
+00003040: 2020 2020 2020 2020 2020 2024 2827 2376             $('#v
+00003050: 6572 6966 6963 6174 696f 6e2d 636f 6465  erification-code
+00003060: 2d6d 6f64 616c 2729 2e6d 6f64 616c 287b  -modal').modal({
+00003070: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00003080: 2020 2020 2062 6163 6b64 726f 703a 2027       backdrop: '
+00003090: 7374 6174 6963 272c 0a20 2020 2020 2020  static',.       
+000030a0: 2020 2020 2020 2020 2020 2020 206b 6579               key
+000030b0: 626f 6172 643a 2066 616c 7365 0a20 2020  board: false.   
+000030c0: 2020 2020 2020 2020 2020 2020 207d 290a               }).
+000030d0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000030e0: 2024 2827 2373 6d61 7274 6964 2d76 6572   $('#smartid-ver
+000030f0: 6966 6963 6174 696f 6e2d 636f 6465 2729  ification-code')
+00003100: 2e74 6578 7428 7265 7370 6f6e 7365 2e76  .text(response.v
+00003110: 6572 6966 6963 6174 696f 6e5f 636f 6465  erification_code
+00003120: 290a 0a20 2020 2020 2020 2020 2020 2020  )..             
+00003130: 2020 202f 2f20 2e2e 2e6e 6578 7420 7068     // ...next ph
+00003140: 6173 653a 2070 6f6c 6c20 666f 7220 7374  ase: poll for st
+00003150: 6174 7573 206f 6620 7369 676e 696e 670a  atus of signing.
+00003160: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003170: 7365 7454 696d 656f 7574 2866 756e 6374  setTimeout(funct
+00003180: 696f 6e20 2829 207b 0a20 2020 2020 2020  ion () {.       
+00003190: 2020 2020 2020 2020 2020 2020 206d 616e               man
+000031a0: 6167 6572 2e73 6d61 7274 6964 5374 6174  ager.smartidStat
+000031b0: 7573 287b 6373 7266 6d69 6464 6c65 7761  us({csrfmiddlewa
+000031c0: 7265 746f 6b65 6e3a 2063 7372 665f 746f  retoken: csrf_to
+000031d0: 6b65 6e7d 292e 7468 656e 280a 2020 2020  ken}).then(.    
+000031e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000031f0: 2020 2020 6f6e 4669 6e69 7368 5369 676e      onFinishSign
+00003200: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+00003210: 2020 2020 2020 2020 2020 6f6e 4572 726f            onErro
+00003220: 720a 2020 2020 2020 2020 2020 2020 2020  r.              
+00003230: 2020 2020 2020 290a 2020 2020 2020 2020        ).        
+00003240: 2020 2020 2020 2020 7d2c 2074 696d 656f          }, timeo
+00003250: 7574 466f 7256 6572 6966 6963 6174 696f  utForVerificatio
+00003260: 6e43 6f64 6529 0a20 2020 2020 2020 2020  nCode).         
+00003270: 2020 207d 0a0a 2020 2020 2020 2020 2020     }..          
+00003280: 2020 6675 6e63 7469 6f6e 206f 6e46 696e    function onFin
+00003290: 6973 6853 6967 6e28 2920 7b0a 2020 2020  ishSign() {.    
+000032a0: 2020 2020 2020 2020 2020 2020 2428 2723              $('#
+000032b0: 736d 6172 7469 642d 6d6f 6461 6c27 292e  smartid-modal').
+000032c0: 6d6f 6461 6c28 2268 6964 6522 290a 2020  modal("hide").  
+000032d0: 2020 2020 2020 2020 2020 2020 2020 6f6e                on
+000032e0: 5369 676e 6564 2829 0a20 2020 2020 2020  Signed().       
+000032f0: 2020 2020 207d 0a0a 0a20 2020 2020 2020       }...       
+00003300: 2020 2020 2076 6172 2066 6f72 6d20 3d20       var form = 
+00003310: 646f 6375 6d65 6e74 2e66 6f72 6d73 2e73  document.forms.s
+00003320: 6d61 7274 4964 0a20 2020 2020 2020 2020  martId.         
+00003330: 2020 2076 6172 2069 6443 6f64 6520 3d20     var idCode = 
+00003340: 666f 726d 2e69 645f 636f 6465 2e76 616c  form.id_code.val
+00003350: 7565 0a0a 2020 2020 2020 2020 2020 2020  ue..            
+00003360: 6966 2028 2169 6443 6f64 6529 207b 0a20  if (!idCode) {. 
+00003370: 2020 2020 2020 2020 2020 2020 2020 2061                 a
+00003380: 6c65 7274 2827 506c 6561 7365 2065 6e74  lert('Please ent
+00003390: 6572 2061 6e20 4944 2063 6f64 6527 290a  er an ID code').
+000033a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000033b0: 7265 7475 726e 0a20 2020 2020 2020 2020  return.         
+000033c0: 2020 207d 0a0a 2020 2020 2020 2020 2020     }..          
+000033d0: 2020 636f 6e73 6f6c 652e 6c6f 6728 2753    console.log('S
+000033e0: 6d61 7274 4944 3a20 7369 676e 696e 6720  martID: signing 
+000033f0: 7769 7468 2069 6420 636f 6465 272c 2069  with id code', i
+00003400: 6443 6f64 6529 0a0a 2020 2020 2020 2020  dCode)..        
+00003410: 2020 2020 6d61 6e61 6765 722e 7369 676e      manager.sign
+00003420: 5769 7468 536d 6172 7449 6428 7b0a 2020  WithSmartId({.  
+00003430: 2020 2020 2020 2020 2020 2020 2020 6964                id
+00003440: 5f63 6f64 653a 2069 6443 6f64 652c 0a20  _code: idCode,. 
+00003450: 2020 2020 2020 2020 2020 2020 2020 2063                 c
+00003460: 7372 666d 6964 646c 6577 6172 6574 6f6b  srfmiddlewaretok
+00003470: 656e 3a20 6373 7266 5f74 6f6b 656e 0a20  en: csrf_token. 
+00003480: 2020 2020 2020 2020 2020 207d 292e 7468             }).th
+00003490: 656e 280a 2020 2020 2020 2020 2020 2020  en(.            
+000034a0: 2020 2020 2f2f 2053 7461 7274 2063 616c      // Start cal
+000034b0: 6c62 6163 6b20 6865 6c6c 0a20 2020 2020  lback hell.     
+000034c0: 2020 2020 2020 2020 2020 206f 6e53 7461             onSta
+000034d0: 7274 5369 676e 2c0a 2020 2020 2020 2020  rtSign,.        
+000034e0: 2020 2020 2020 2020 6f6e 4572 726f 720a          onError.
+000034f0: 2020 2020 2020 2020 2020 2020 290a 2020              ).  
+00003500: 2020 2020 2020 7d0a 0a20 2020 2020 2020        }..       
+00003510: 2024 2827 2373 6967 6e2d 6964 2729 2e6f   $('#sign-id').o
+00003520: 6e28 2763 6c69 636b 272c 2066 756e 6374  n('click', funct
+00003530: 696f 6e20 2865 2920 7b0a 2020 2020 2020  ion (e) {.      
+00003540: 2020 2020 2020 652e 7072 6576 656e 7444        e.preventD
+00003550: 6566 6175 6c74 2829 0a0a 2020 2020 2020  efault()..      
+00003560: 2020 2020 2020 2428 2723 6964 2d6d 6f64        $('#id-mod
+00003570: 616c 2729 2e6d 6f64 616c 287b 0a20 2020  al').modal({.   
+00003580: 2020 2020 2020 2020 2020 2020 2062 6163               bac
+00003590: 6b64 726f 703a 2027 7374 6174 6963 272c  kdrop: 'static',
+000035a0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000035b0: 206b 6579 626f 6172 643a 2066 616c 7365   keyboard: false
+000035c0: 0a20 2020 2020 2020 2020 2020 207d 290a  .            }).
+000035d0: 0a20 2020 2020 2020 2020 2020 206d 616e  .            man
+000035e0: 6167 6572 2e73 6967 6e57 6974 6849 6443  ager.signWithIdC
+000035f0: 6172 6428 7b63 7372 666d 6964 646c 6577  ard({csrfmiddlew
+00003600: 6172 6574 6f6b 656e 3a20 6373 7266 5f74  aretoken: csrf_t
+00003610: 6f6b 656e 7d29 2e74 6865 6e28 0a20 2020  oken}).then(.   
+00003620: 2020 2020 2020 2020 2020 2020 2066 756e               fun
+00003630: 6374 696f 6e20 2829 207b 0a20 2020 2020  ction () {.     
+00003640: 2020 2020 2020 2020 2020 2020 2020 2024                 $
+00003650: 2827 2369 642d 6d6f 6461 6c27 292e 6d6f  ('#id-modal').mo
+00003660: 6461 6c28 2768 6964 6527 290a 2020 2020  dal('hide').    
+00003670: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003680: 6f6e 5369 676e 6564 2829 0a20 2020 2020  onSigned().     
+00003690: 2020 2020 2020 2020 2020 207d 2c0a 0a20             },.. 
+000036a0: 2020 2020 2020 2020 2020 2020 2020 2066                 f
+000036b0: 756e 6374 696f 6e20 2872 6573 2920 7b0a  unction (res) {.
+000036c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000036d0: 2020 2020 6966 2028 7265 7320 696e 7374      if (res inst
+000036e0: 616e 6365 6f66 2045 7272 6f72 2920 7b0a  anceof Error) {.
+000036f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003700: 2020 2020 2020 2020 636f 6e73 6f6c 652e          console.
+00003710: 6c6f 6728 7265 732e 6d65 7373 6167 652c  log(res.message,
+00003720: 2072 6573 290a 2020 2020 2020 2020 2020   res).          
+00003730: 2020 2020 2020 2020 2020 2020 2020 7265                re
+00003740: 7320 3d20 6d61 6e61 6765 722e 6765 7445  s = manager.getE
+00003750: 7272 6f72 2872 6573 290a 0a20 2020 2020  rror(res)..     
+00003760: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003770: 2020 2061 6c65 7274 2872 6573 2e6d 6573     alert(res.mes
+00003780: 7361 6765 290a 0a20 2020 2020 2020 2020  sage)..         
+00003790: 2020 2020 2020 2020 2020 2020 2020 2063                 c
+000037a0: 6f6e 736f 6c65 2e65 7272 6f72 2827 5b45  onsole.error('[E
+000037b0: 7272 6f72 2063 6f64 653a 2027 202b 2072  rror code: ' + r
+000037c0: 6573 2e72 6574 7572 6e43 6f64 6520 2b20  es.returnCode + 
+000037d0: 273b 2045 7272 6f72 3a20 2720 2b20 7265  '; Error: ' + re
+000037e0: 732e 6d65 7373 6167 6520 2b20 275d 2729  s.message + ']')
+000037f0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00003800: 2020 2020 2020 2020 2024 2827 2369 642d           $('#id-
+00003810: 6d6f 6461 6c27 292e 6d6f 6461 6c28 2768  modal').modal('h
+00003820: 6964 6527 290a 2020 2020 2020 2020 2020  ide').          
+00003830: 2020 2020 2020 2020 2020 7d20 656c 7365            } else
+00003840: 207b 0a20 2020 2020 2020 2020 2020 2020   {.             
+00003850: 2020 2020 2020 2020 2020 2069 6620 2874             if (t
+00003860: 7970 656f 6620 7265 7320 3d3d 3d20 2773  ypeof res === 's
+00003870: 7472 696e 6727 207c 7c20 2872 6573 2026  tring' || (res &
+00003880: 2620 7265 732e 6572 726f 725f 636f 6465  & res.error_code
+00003890: 2929 207b 0a20 2020 2020 2020 2020 2020  )) {.           
+000038a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000038b0: 2076 6172 206d 7367 203d 2072 6573 2026   var msg = res &
+000038c0: 2620 7265 732e 6d65 7373 6167 6520 213d  & res.message !=
+000038d0: 3d20 756e 6465 6669 6e65 6420 3f20 7265  = undefined ? re
+000038e0: 732e 6d65 7373 6167 6520 3a20 7265 730a  s.message : res.
+000038f0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00003900: 2020 2020 2020 2020 2020 2020 2061 6c65               ale
+00003910: 7274 286d 7367 202b 2027 2c20 706c 6561  rt(msg + ', plea
+00003920: 7365 2074 7279 2061 6761 696e 2729 0a20  se try again'). 
+00003930: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003940: 2020 2020 2020 2020 2020 2024 2827 2369             $('#i
+00003950: 642d 6d6f 6461 6c27 292e 6d6f 6461 6c28  d-modal').modal(
+00003960: 2768 6964 6527 290a 2020 2020 2020 2020  'hide').        
+00003970: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003980: 7d20 656c 7365 207b 0a20 2020 2020 2020  } else {.       
+00003990: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000039a0: 2020 2020 2063 6f6e 736f 6c65 2e65 7272       console.err
+000039b0: 6f72 2872 6573 2026 2620 7265 732e 6d65  or(res && res.me
+000039c0: 7373 6167 6520 213d 3d20 756e 6465 6669  ssage !== undefi
+000039d0: 6e65 6420 3f20 7265 732e 6d65 7373 6167  ned ? res.messag
+000039e0: 6520 3a20 7265 7329 0a20 2020 2020 2020  e : res).       
+000039f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003a00: 2020 2020 2061 6c65 7274 2827 536f 6d65       alert('Some
+00003a10: 7468 696e 6720 7765 6e74 2077 726f 6e67  thing went wrong
+00003a20: 2c20 706c 6561 7365 2072 6566 7265 7368  , please refresh
+00003a30: 2074 6865 2070 6167 6520 616e 6420 7472   the page and tr
+00003a40: 7920 6167 6169 6e27 290a 2020 2020 2020  y again').      
+00003a50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003a60: 2020 7d0a 2020 2020 2020 2020 2020 2020    }.            
+00003a70: 2020 2020 2020 2020 7d0a 2020 2020 2020          }.      
+00003a80: 2020 2020 2020 2020 2020 7d0a 2020 2020            }.    
+00003a90: 2020 2020 2020 2020 290a 2020 2020 2020          ).      
+00003aa0: 2020 7d29 0a0a 2020 2020 2020 2020 2428    })..        $(
+00003ab0: 2723 6765 742d 646f 6375 6d65 6e74 2729  '#get-document')
+00003ac0: 2e6f 6e28 2763 6c69 636b 272c 2066 756e  .on('click', fun
+00003ad0: 6374 696f 6e20 2829 207b 0a20 2020 2020  ction () {.     
+00003ae0: 2020 2020 2020 2073 6574 5469 6d65 6f75         setTimeou
+00003af0: 7428 6675 6e63 7469 6f6e 2028 2920 7b0a  t(function () {.
+00003b00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003b10: 7769 6e64 6f77 2e6c 6f63 6174 696f 6e2e  window.location.
+00003b20: 7265 6c6f 6164 2829 0a20 2020 2020 2020  reload().       
+00003b30: 2020 2020 207d 2c20 3230 3030 290a 2020       }, 2000).  
+00003b40: 2020 2020 2020 7d29 0a0a 2020 2020 2020        })..      
+00003b50: 2020 646f 6375 6d65 6e74 2e66 6f72 6d73    document.forms
+00003b60: 2e73 6d61 7274 4964 2e6f 6e73 7562 6d69  .smartId.onsubmi
+00003b70: 7420 3d20 7369 676e 536d 6172 7449 440a  t = signSmartID.
+00003b80: 2020 2020 2020 2020 2428 2723 7369 676e          $('#sign
+00003b90: 2d73 6d61 7274 6964 2d62 7574 746f 6e27  -smartid-button'
+00003ba0: 292e 6f6e 2827 636c 6963 6b27 2c20 7369  ).on('click', si
+00003bb0: 676e 536d 6172 7449 4429 0a0a 2020 2020  gnSmartID)..    
+00003bc0: 2020 2020 646f 6375 6d65 6e74 2e66 6f72      document.for
+00003bd0: 6d73 2e6d 6f62 696c 6549 642e 6f6e 7375  ms.mobileId.onsu
+00003be0: 626d 6974 203d 2073 6967 6e4d 6f62 696c  bmit = signMobil
+00003bf0: 6549 440a 2020 2020 2020 2020 2428 2723  eID.        $('#
+00003c00: 7369 676e 4d6f 6269 6c65 2729 2e6f 6e28  signMobile').on(
+00003c10: 2763 6c69 636b 272c 2073 6967 6e4d 6f62  'click', signMob
+00003c20: 696c 6549 4429 0a0a 2020 2020 7d29 0a0a  ileID)..    })..
+00003c30: 3c2f 7363 7269 7074 3e0a 0a3c 2f62 6f64  </script>..</bod
+00003c40: 793e 0a3c 2f68 746d 6c3e 0a              y>.</html>.
```

### Comparing `django_esteid-3.4b1/esteid/templates/esteid/test.html` & `django_esteid-4.0b1/esteid/templates/esteid/auth-new.html`

 * *Files 12% similar despite different names*

```diff
@@ -11,955 +11,979 @@
 000000a0: 4353 5320 2d2d 3e0a 2020 2020 3c6c 696e  CSS -->.    <lin
 000000b0: 6b20 7265 6c3d 2273 7479 6c65 7368 6565  k rel="styleshee
 000000c0: 7422 2068 7265 663d 2268 7474 7073 3a2f  t" href="https:/
 000000d0: 2f6d 6178 6364 6e2e 626f 6f74 7374 7261  /maxcdn.bootstra
 000000e0: 7063 646e 2e63 6f6d 2f62 6f6f 7473 7472  pcdn.com/bootstr
 000000f0: 6170 2f33 2e33 2e34 2f63 7373 2f62 6f6f  ap/3.3.4/css/boo
 00000100: 7473 7472 6170 2e6d 696e 2e63 7373 223e  tstrap.min.css">
-00000110: 0a3c 2f68 6561 643e 0a0a 3c62 6f64 793e  .</head>..<body>
-00000120: 0a3c 6469 7620 636c 6173 733d 2263 6f6e  .<div class="con
-00000130: 7461 696e 6572 223e 0a20 2020 203c 6831  tainer">.    <h1
-00000140: 3e45 7374 6569 6420 5465 7374 2070 6167  >Esteid Test pag
-00000150: 653c 2f68 313e 0a20 2020 203c 7020 7374  e</h1>.    <p st
-00000160: 796c 653d 2266 6f6e 742d 7369 7a65 3a20  yle="font-size: 
-00000170: 782d 6c61 7267 6522 3e0a 2020 2020 2020  x-large">.      
-00000180: 2020 3c62 3e54 6869 7320 7465 7374 2070    <b>This test p
-00000190: 6167 6520 7573 6573 2074 6865 2064 6570  age uses the dep
-000001a0: 7265 6361 7465 6420 6163 7469 6f6e 7320  recated actions 
-000001b0: 4150 492e 2054 6f20 7465 7374 2074 6865  API. To test the
-000001c0: 206e 6577 2041 5049 2c0a 2020 2020 2020   new API,.      
-000001d0: 2020 2020 2020 3c61 2068 7265 663d 227b        <a href="{
-000001e0: 2520 7572 6c20 2773 6b5f 7465 7374 5f6e  % url 'sk_test_n
-000001f0: 6577 2720 257d 223e 706c 6561 7365 2067  ew' %}">please g
-00000200: 6f20 746f 2074 6869 7320 7061 6765 213c  o to this page!<
-00000210: 2f61 3e3c 2f62 3e0a 2020 2020 3c2f 703e  /a></b>.    </p>
-00000220: 0a20 2020 203c 703e 0a20 2020 2020 2020  .    <p>.       
-00000230: 2054 6869 7320 6973 2061 2074 6573 7420   This is a test 
-00000240: 7061 6765 2066 6f72 2064 6967 6974 616c  page for digital
-00000250: 2073 6967 6e69 6e67 206f 6620 6669 6c65   signing of file
-00000260: 7320 7669 6120 7079 7468 6f6e 2e0a 2020  s via python..  
-00000270: 2020 3c2f 703e 0a0a 2020 2020 3c75 6c3e    </p>..    <ul>
-00000280: 0a20 2020 2020 2020 203c 6c69 3e0a 2020  .        <li>.  
-00000290: 2020 2020 2020 2020 2020 4d6f 6269 6c65            Mobile
-000002a0: 2049 4420 7369 676e 696e 6720 6973 2064   ID signing is d
-000002b0: 6f6e 6520 7769 7468 2044 656d 6f20 4d6f  one with Demo Mo
-000002c0: 6269 6c65 2049 4420 7365 7276 6963 652c  bile ID service,
-000002d0: 2079 6f75 2063 616e 206f 6e6c 7920 7573   you can only us
-000002e0: 6520 7468 650a 2020 2020 2020 2020 2020  e the.          
-000002f0: 2020 3c61 2068 7265 663d 2268 7474 7073    <a href="https
-00000300: 3a2f 2f67 6974 6875 622e 636f 6d2f 534b  ://github.com/SK
-00000310: 2d45 4944 2f4d 4944 2f77 696b 692f 5465  -EID/MID/wiki/Te
-00000320: 7374 2d6e 756d 6265 722d 666f 722d 6175  st-number-for-au
-00000330: 746f 6d61 7465 642d 7465 7374 696e 672d  tomated-testing-
-00000340: 696e 2d44 454d 4f22 2074 6172 6765 743d  in-DEMO" target=
-00000350: 225f 626c 616e 6b22 3e64 656d 6f0a 2020  "_blank">demo.  
-00000360: 2020 2020 2020 2020 2020 2020 2020 7465                te
-00000370: 7374 206e 756d 6265 7273 3c2f 613e 2e0a  st numbers</a>..
-00000380: 2020 2020 2020 2020 2020 2020 5468 6520              The 
-00000390: 7369 676e 6174 7572 6573 2077 696c 6c20  signatures will 
-000003a0: 6e6f 7420 6265 2076 616c 6964 2075 6e6c  not be valid unl
-000003b0: 6573 7320 7468 6520 7465 7374 2063 6572  ess the test cer
-000003c0: 7469 6669 6361 7465 7320 6172 6520 7573  tificates are us
-000003d0: 6564 2074 6f20 7661 6c69 6461 7465 2074  ed to validate t
-000003e0: 6865 6d2e 0a20 2020 2020 2020 203c 2f6c  hem..        </l
-000003f0: 693e 0a20 2020 2020 2020 203c 6c69 3e0a  i>.        <li>.
-00000400: 2020 2020 2020 2020 2020 2020 4944 2043              ID C
-00000410: 6172 6420 7369 676e 696e 6720 6361 6e20  ard signing can 
-00000420: 6265 2064 6f6e 6520 7769 7468 2072 6561  be done with rea
-00000430: 6c20 4944 2063 6172 6473 2c20 6275 7420  l ID cards, but 
-00000440: 7375 6368 2061 2073 6967 6e61 7475 7265  such a signature
-00000450: 2063 616e 206e 6f74 2062 6520 7661 6c69   can not be vali
-00000460: 6461 7465 642e 0a20 2020 2020 2020 203c  dated..        <
-00000470: 2f6c 693e 0a20 2020 2020 2020 203c 6c69  /li>.        <li
-00000480: 3e0a 2020 2020 2020 2020 2020 2020 4944  >.            ID
-00000490: 2043 6172 6420 7369 676e 696e 6720 7265   Card signing re
-000004a0: 7175 6972 6573 2074 6865 2063 6872 6f6d  quires the chrom
-000004b0: 652d 746f 6b65 6e2d 7369 676e 696e 6720  e-token-signing 
-000004c0: 666f 7220 6368 726f 6d65 206f 7220 6669  for chrome or fi
-000004d0: 7265 666f 782e 0a20 2020 2020 2020 203c  refox..        <
-000004e0: 2f6c 693e 0a20 2020 2020 2020 203c 6c69  /li>.        <li
-000004f0: 3e0a 2020 2020 2020 2020 2020 2020 4944  >.            ID
-00000500: 2043 6172 6420 7369 676e 696e 6720 7265   Card signing re
-00000510: 7175 6972 6573 2048 5454 5053 2e20 506c  quires HTTPS. Pl
-00000520: 6561 7365 2072 6566 6572 2074 6f20 7468  ease refer to th
-00000530: 6520 5245 4144 4d45 2e0a 2020 2020 2020  e README..      
-00000540: 2020 3c2f 6c69 3e0a 2020 2020 2020 2020    </li>.        
-00000550: 3c6c 693e 0a20 2020 2020 2020 2020 2020  <li>.           
-00000560: 2053 6967 6e69 6e67 2077 6974 6820 536d   Signing with Sm
-00000570: 6172 7449 4420 7265 7175 6972 6573 2073  artID requires s
-00000580: 6574 7469 6e67 2075 7020 6120 6465 6d6f  etting up a demo
-00000590: 2053 6d61 7274 4944 2061 6363 6f75 6e74   SmartID account
-000005a0: 2e20 506c 6561 7365 2072 6566 6572 2074  . Please refer t
-000005b0: 6f20 7468 6520 5245 4144 4d45 2e0a 2020  o the README..  
-000005c0: 2020 2020 2020 3c2f 6c69 3e0a 2020 2020        </li>.    
-000005d0: 3c2f 756c 3e0a 0a20 2020 203c 6872 202f  </ul>..    <hr /
-000005e0: 3e0a 0a20 2020 203c 6833 3e55 706c 6f61  >..    <h3>Uploa
-000005f0: 6465 6420 6669 6c65 733c 2f68 333e 0a0a  ded files</h3>..
-00000600: 2020 2020 7b25 2069 6620 6669 6c65 7320      {% if files 
-00000610: 257d 0a20 2020 2020 2020 203c 756c 2063  %}.        <ul c
-00000620: 6c61 7373 3d22 6c69 7374 2d67 726f 7570  lass="list-group
-00000630: 223e 0a20 2020 2020 2020 2020 2020 207b  ">.            {
-00000640: 2520 666f 7220 6669 6c65 5f6e 616d 652c  % for file_name,
-00000650: 2066 696c 6520 696e 2066 696c 6573 2e69   file in files.i
-00000660: 7465 6d73 2025 7d0a 2020 2020 2020 2020  tems %}.        
-00000670: 2020 2020 2020 2020 3c6c 6920 636c 6173          <li clas
-00000680: 733d 226c 6973 742d 6772 6f75 702d 6974  s="list-group-it
-00000690: 656d 223e 0a20 2020 2020 2020 2020 2020  em">.           
-000006a0: 2020 2020 2020 2020 203c 666f 726d 206d           <form m
-000006b0: 6574 686f 643d 2270 6f73 7422 2063 6c61  ethod="post" cla
-000006c0: 7373 3d22 7075 6c6c 2d72 6967 6874 223e  ss="pull-right">
-000006d0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000006e0: 2020 2020 2020 2020 207b 2520 6373 7266           {% csrf
-000006f0: 5f74 6f6b 656e 2025 7d0a 0a20 2020 2020  _token %}..     
-00000700: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000710: 2020 203c 696e 7075 7420 6e61 6d65 3d22     <input name="
-00000720: 6163 7469 6f6e 2220 7479 7065 3d22 6869  action" type="hi
-00000730: 6464 656e 2220 7661 6c75 653d 2272 656d  dden" value="rem
-00000740: 6f76 655f 6669 6c65 2220 2f3e 0a20 2020  ove_file" />.   
-00000750: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000760: 2020 2020 203c 696e 7075 7420 6e61 6d65       <input name
-00000770: 3d22 6669 6c65 5f6e 616d 6522 2074 7970  ="file_name" typ
-00000780: 653d 2268 6964 6465 6e22 2076 616c 7565  e="hidden" value
-00000790: 3d22 7b7b 2066 696c 655f 6e61 6d65 207d  ="{{ file_name }
-000007a0: 7d22 202f 3e0a 0a20 2020 2020 2020 2020  }" />..         
-000007b0: 2020 2020 2020 2020 2020 2020 2020 203c                 <
-000007c0: 696e 7075 7420 7479 7065 3d22 7375 626d  input type="subm
-000007d0: 6974 2220 636c 6173 733d 2262 746e 2062  it" class="btn b
-000007e0: 746e 2d78 7320 6274 6e2d 6461 6e67 6572  tn-xs btn-danger
-000007f0: 2220 7661 6c75 653d 2258 2220 2f3e 0a20  " value="X" />. 
-00000800: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000810: 2020 203c 2f66 6f72 6d3e 0a20 2020 2020     </form>.     
-00000820: 2020 2020 2020 2020 2020 2020 2020 203c                 <
-00000830: 7370 616e 2063 6c61 7373 3d22 6261 6467  span class="badg
-00000840: 6522 3e7b 7b20 6669 6c65 2e73 697a 6520  e">{{ file.size 
-00000850: 7d7d 2062 7974 6573 3c2f 7370 616e 3e0a  }} bytes</span>.
-00000860: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00000870: 2020 2020 207b 7b20 6669 6c65 5f6e 616d       {{ file_nam
-00000880: 6520 7d7d 0a20 2020 2020 2020 2020 2020  e }}.           
-00000890: 2020 2020 203c 2f6c 693e 0a20 2020 2020       </li>.     
-000008a0: 2020 2020 2020 207b 2520 656e 6466 6f72         {% endfor
-000008b0: 2025 7d0a 2020 2020 2020 2020 3c2f 756c   %}.        </ul
-000008c0: 3e0a 0a20 2020 2020 2020 203c 6872 202f  >..        <hr /
-000008d0: 3e0a 0a20 2020 2020 2020 203c 6833 3e53  >..        <h3>S
-000008e0: 6967 6e20 7468 6520 6669 6c65 733c 2f68  ign the files</h
-000008f0: 333e 0a0a 2020 2020 2020 2020 3c61 2068  3>..        <a h
-00000900: 7265 663d 2223 2220 6964 3d22 7369 676e  ref="#" id="sign
-00000910: 2d69 6422 3e3c 696d 6720 616c 743d 2249  -id"><img alt="I
-00000920: 4420 4361 7264 2220 7372 633d 227b 2520  D Card" src="{% 
-00000930: 7374 6174 6963 2027 696d 6167 6573 2f65  static 'images/e
-00000940: 7374 6569 642f 6964 2d6b 6161 7274 2d6c  steid/id-kaart-l
-00000950: 6f67 6f2e 6769 6627 2025 7d22 3e3c 2f61  ogo.gif' %}"></a
-00000960: 3e0a 2020 2020 2020 2020 3c61 2068 7265  >.        <a hre
-00000970: 663d 2223 2220 6964 3d22 7369 676e 2d6d  f="#" id="sign-m
-00000980: 6964 223e 3c69 6d67 2061 6c74 3d22 4d6f  id"><img alt="Mo
-00000990: 6269 6c65 2049 4422 2073 7263 3d22 7b25  bile ID" src="{%
-000009a0: 2073 7461 7469 6320 2769 6d61 6765 732f   static 'images/
-000009b0: 6573 7465 6964 2f6d 6964 2d6c 6f67 6f2e  esteid/mid-logo.
-000009c0: 6769 6627 2025 7d22 3e3c 2f61 3e0a 2020  gif' %}"></a>.  
-000009d0: 2020 2020 2020 3c61 2068 7265 663d 2223        <a href="#
-000009e0: 2220 6964 3d22 7369 676e 2d73 6d61 7274  " id="sign-smart
-000009f0: 6964 223e 3c69 6d67 2061 6c74 3d22 536d  id"><img alt="Sm
-00000a00: 6172 7420 4944 2220 7372 633d 227b 2520  art ID" src="{% 
-00000a10: 7374 6174 6963 2027 696d 6167 6573 2f65  static 'images/e
-00000a20: 7374 6569 642f 736d 6172 7449 442d 6c6f  steid/smartID-lo
-00000a30: 676f 2d62 746e 2e70 6e67 2720 257d 223e  go-btn.png' %}">
-00000a40: 3c2f 613e 0a0a 2020 2020 7b25 2065 6c73  </a>..    {% els
-00000a50: 6520 257d 0a20 2020 2020 2020 203c 703e  e %}.        <p>
-00000a60: 4e6f 2066 696c 6573 2075 706c 6f61 6465  No files uploade
-00000a70: 642c 2074 6f20 6265 6769 6e20 7468 6520  d, to begin the 
-00000a80: 7369 676e 696e 6720 7072 6f63 6573 732c  signing process,
-00000a90: 2070 6c65 6173 6520 7570 6c6f 6164 2073   please upload s
-00000aa0: 6f6d 6520 6669 6c65 733c 2f70 3e0a 2020  ome files</p>.  
-00000ab0: 2020 7b25 2065 6e64 6966 2025 7d0a 0a20    {% endif %}.. 
-00000ac0: 2020 203c 6872 202f 3e0a 0a20 2020 203c     <hr />..    <
-00000ad0: 6832 3e55 706c 6f61 6420 6669 6c65 733c  h2>Upload files<
-00000ae0: 2f68 323e 0a20 2020 203c 666f 726d 206d  /h2>.    <form m
-00000af0: 6574 686f 643d 2250 4f53 5422 2065 6e63  ethod="POST" enc
-00000b00: 7479 7065 3d22 6d75 6c74 6970 6172 742f  type="multipart/
-00000b10: 666f 726d 2d64 6174 6122 3e0a 2020 2020  form-data">.    
-00000b20: 2020 2020 7b25 2063 7372 665f 746f 6b65      {% csrf_toke
-00000b30: 6e20 257d 0a0a 2020 2020 2020 2020 3c64  n %}..        <d
-00000b40: 6976 2063 6c61 7373 3d22 666f 726d 2d67  iv class="form-g
-00000b50: 726f 7570 223e 0a20 2020 2020 2020 2020  roup">.         
-00000b60: 2020 203c 6c61 6265 6c20 666f 723d 2265     <label for="e
-00000b70: 7861 6d70 6c65 496e 7075 7446 696c 6522  xampleInputFile"
-00000b80: 3e53 656c 6563 7420 6669 6c65 3c2f 6c61  >Select file</la
-00000b90: 6265 6c3e 0a20 2020 2020 2020 2020 2020  bel>.           
-00000ba0: 203c 696e 7075 7420 7479 7065 3d22 6669   <input type="fi
-00000bb0: 6c65 2220 6964 3d22 6578 616d 706c 6549  le" id="exampleI
-00000bc0: 6e70 7574 4669 6c65 2220 6e61 6d65 3d22  nputFile" name="
-00000bd0: 7468 655f 6669 6c65 223e 0a20 2020 2020  the_file">.     
-00000be0: 2020 203c 2f64 6976 3e0a 0a20 2020 2020     </div>..     
-00000bf0: 2020 203c 6275 7474 6f6e 2074 7970 653d     <button type=
-00000c00: 2273 7562 6d69 7422 2063 6c61 7373 3d22  "submit" class="
-00000c10: 6274 6e20 6274 6e2d 6465 6661 756c 7422  btn btn-default"
-00000c20: 3e53 7562 6d69 743c 2f62 7574 746f 6e3e  >Submit</button>
-00000c30: 0a0a 2020 2020 3c2f 666f 726d 3e0a 3c2f  ..    </form>.</
-00000c40: 6469 763e 0a0a 3c64 6976 2063 6c61 7373  div>..<div class
-00000c50: 3d22 6d6f 6461 6c20 6661 6465 2220 6964  ="modal fade" id
-00000c60: 3d22 6d69 642d 6d6f 6461 6c22 3e0a 2020  ="mid-modal">.  
-00000c70: 2020 3c64 6976 2063 6c61 7373 3d22 6d6f    <div class="mo
-00000c80: 6461 6c2d 6469 616c 6f67 223e 0a20 2020  dal-dialog">.   
-00000c90: 2020 2020 203c 6469 7620 636c 6173 733d       <div class=
-00000ca0: 226d 6f64 616c 2d63 6f6e 7465 6e74 223e  "modal-content">
-00000cb0: 0a20 2020 2020 2020 2020 2020 203c 6469  .            <di
-00000cc0: 7620 636c 6173 733d 226d 6f64 616c 2d68  v class="modal-h
-00000cd0: 6561 6465 7222 3e0a 2020 2020 2020 2020  eader">.        
-00000ce0: 2020 2020 2020 2020 3c62 7574 746f 6e20          <button 
-00000cf0: 7479 7065 3d22 6275 7474 6f6e 2220 636c  type="button" cl
-00000d00: 6173 733d 2263 6c6f 7365 2220 6461 7461  ass="close" data
-00000d10: 2d64 6973 6d69 7373 3d22 6d6f 6461 6c22  -dismiss="modal"
-00000d20: 2061 7269 612d 6c61 6265 6c3d 2243 6c6f   aria-label="Clo
-00000d30: 7365 223e 3c73 7061 6e20 6172 6961 2d68  se"><span aria-h
-00000d40: 6964 6465 6e3d 2274 7275 6522 3e26 7469  idden="true">&ti
-00000d50: 6d65 733b 3c2f 7370 616e 3e0a 2020 2020  mes;</span>.    
-00000d60: 2020 2020 2020 2020 2020 2020 3c2f 6275              </bu
-00000d70: 7474 6f6e 3e0a 2020 2020 2020 2020 2020  tton>.          
-00000d80: 2020 2020 2020 3c68 3420 636c 6173 733d        <h4 class=
-00000d90: 226d 6f64 616c 2d74 6974 6c65 223e 5369  "modal-title">Si
-00000da0: 676e 2074 6865 2066 696c 6573 2077 6974  gn the files wit
-00000db0: 6820 4d6f 6269 6c65 4944 3c2f 6834 3e0a  h MobileID</h4>.
-00000dc0: 2020 2020 2020 2020 2020 2020 3c2f 6469              </di
-00000dd0: 763e 0a0a 2020 2020 2020 2020 2020 2020  v>..            
-00000de0: 3c64 6976 2063 6c61 7373 3d22 6d6f 6461  <div class="moda
-00000df0: 6c2d 626f 6479 223e 0a20 2020 2020 2020  l-body">.       
-00000e00: 2020 2020 2020 2020 203c 666f 726d 206e           <form n
-00000e10: 616d 653d 226d 6f62 696c 6549 6422 3e0a  ame="mobileId">.
-00000e20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000e30: 2020 2020 3c64 6976 2063 6c61 7373 3d22      <div class="
-00000e40: 666f 726d 2d67 726f 7570 223e 0a20 2020  form-group">.   
-00000e50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000e60: 2020 2020 203c 6c61 6265 6c20 666f 723d       <label for=
-00000e70: 2270 686f 6e65 4e72 496e 7075 7422 3e44  "phoneNrInput">D
-00000e80: 656d 6f20 5068 6f6e 6520 6e72 3a3c 2f6c  emo Phone nr:</l
-00000e90: 6162 656c 3e0a 2020 2020 2020 2020 2020  abel>.          
-00000ea0: 2020 2020 2020 2020 2020 2020 2020 3c69                <i
-00000eb0: 6e70 7574 2074 7970 653d 2274 6578 7422  nput type="text"
-00000ec0: 206e 616d 653d 2270 686f 6e65 5f6e 7222   name="phone_nr"
-00000ed0: 2069 643d 2270 686f 6e65 4e72 496e 7075   id="phoneNrInpu
-00000ee0: 7422 2063 6c61 7373 3d22 666f 726d 2d63  t" class="form-c
-00000ef0: 6f6e 7472 6f6c 220a 2020 2020 2020 2020  ontrol".        
-00000f00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000f10: 2020 2020 2020 2076 616c 7565 3d22 7b7b         value="{{
-00000f20: 2072 6571 7565 7374 2e73 6573 7369 6f6e   request.session
-00000f30: 2e64 646f 635f 7465 7374 5f70 686f 6e65  .ddoc_test_phone
-00000f40: 5f6e 756d 6265 7220 7c20 6465 6661 756c  _number | defaul
-00000f50: 743a 272b 3337 3230 3030 3030 3736 3627  t:'+37200000766'
-00000f60: 207d 7d22 202f 3e0a 2020 2020 2020 2020   }}" />.        
-00000f70: 2020 2020 2020 2020 2020 2020 3c2f 6469              </di
-00000f80: 763e 0a20 2020 2020 2020 2020 2020 2020  v>.             
-00000f90: 2020 2020 2020 203c 6469 7620 636c 6173         <div clas
-00000fa0: 733d 2266 6f72 6d2d 6772 6f75 7022 3e0a  s="form-group">.
+00000110: 0a20 2020 203c 212d 2d20 7369 6d70 6c65  .    <!-- simple
+00000120: 2073 7069 6e6e 6572 2066 726f 6d20 6c6f   spinner from lo
+00000130: 6164 696e 672e 696f 202d 2d3e 0a20 2020  ading.io -->.   
+00000140: 203c 7374 796c 6520 7479 7065 3d22 7465   <style type="te
+00000150: 7874 2f63 7373 223e 0a20 2020 2020 2020  xt/css">.       
+00000160: 202e 6c64 732d 6475 616c 2d72 696e 6720   .lds-dual-ring 
+00000170: 7b0a 2020 2020 2020 2020 2020 2020 2f2a  {.            /*
+00000180: 2064 6973 706c 6179 3a20 696e 6c69 6e65   display: inline
+00000190: 2d62 6c6f 636b 3b20 2a2f 0a20 2020 2020  -block; */.     
+000001a0: 2020 2020 2020 2064 6973 706c 6179 3a20         display: 
+000001b0: 6e6f 6e65 3b0a 2020 2020 2020 2020 2020  none;.          
+000001c0: 2020 7769 6474 683a 2038 3070 783b 0a20    width: 80px;. 
+000001d0: 2020 2020 2020 2020 2020 2068 6569 6768             heigh
+000001e0: 743a 2038 3070 783b 0a20 2020 2020 2020  t: 80px;.       
+000001f0: 207d 0a0a 2020 2020 2020 2020 2e6c 6473   }..        .lds
+00000200: 2d64 7561 6c2d 7269 6e67 3a61 6674 6572  -dual-ring:after
+00000210: 207b 0a20 2020 2020 2020 2020 2020 2063   {.            c
+00000220: 6f6e 7465 6e74 3a20 2220 223b 0a20 2020  ontent: " ";.   
+00000230: 2020 2020 2020 2020 2064 6973 706c 6179           display
+00000240: 3a20 626c 6f63 6b3b 0a20 2020 2020 2020  : block;.       
+00000250: 2020 2020 2077 6964 7468 3a20 3634 7078       width: 64px
+00000260: 3b0a 2020 2020 2020 2020 2020 2020 6865  ;.            he
+00000270: 6967 6874 3a20 3634 7078 3b0a 2020 2020  ight: 64px;.    
+00000280: 2020 2020 2020 2020 6d61 7267 696e 3a20          margin: 
+00000290: 3870 783b 0a20 2020 2020 2020 2020 2020  8px;.           
+000002a0: 2062 6f72 6465 722d 7261 6469 7573 3a20   border-radius: 
+000002b0: 3530 253b 0a20 2020 2020 2020 2020 2020  50%;.           
+000002c0: 2062 6f72 6465 723a 2036 7078 2073 6f6c   border: 6px sol
+000002d0: 6964 2023 3333 3333 3333 3b0a 2020 2020  id #333333;.    
+000002e0: 2020 2020 2020 2020 626f 7264 6572 2d63          border-c
+000002f0: 6f6c 6f72 3a20 2333 3333 3333 3320 7472  olor: #333333 tr
+00000300: 616e 7370 6172 656e 7420 2333 3333 3333  ansparent #33333
+00000310: 3320 7472 616e 7370 6172 656e 743b 0a20  3 transparent;. 
+00000320: 2020 2020 2020 2020 2020 2061 6e69 6d61             anima
+00000330: 7469 6f6e 3a20 6c64 732d 6475 616c 2d72  tion: lds-dual-r
+00000340: 696e 6720 312e 3273 206c 696e 6561 7220  ing 1.2s linear 
+00000350: 696e 6669 6e69 7465 3b0a 2020 2020 2020  infinite;.      
+00000360: 2020 7d0a 0a20 2020 2020 2020 2040 6b65    }..        @ke
+00000370: 7966 7261 6d65 7320 6c64 732d 6475 616c  yframes lds-dual
+00000380: 2d72 696e 6720 7b0a 2020 2020 2020 2020  -ring {.        
+00000390: 2020 2020 3025 207b 0a20 2020 2020 2020      0% {.       
+000003a0: 2020 2020 2020 2020 2074 7261 6e73 666f           transfo
+000003b0: 726d 3a20 726f 7461 7465 2830 6465 6729  rm: rotate(0deg)
+000003c0: 3b0a 2020 2020 2020 2020 2020 2020 7d0a  ;.            }.
+000003d0: 2020 2020 2020 2020 2020 2020 3130 3025              100%
+000003e0: 207b 0a20 2020 2020 2020 2020 2020 2020   {.             
+000003f0: 2020 2074 7261 6e73 666f 726d 3a20 726f     transform: ro
+00000400: 7461 7465 2833 3630 6465 6729 3b0a 2020  tate(360deg);.  
+00000410: 2020 2020 2020 2020 2020 7d0a 2020 2020            }.    
+00000420: 2020 2020 7d0a 2020 2020 3c2f 7374 796c      }.    </styl
+00000430: 653e 0a3c 2f68 6561 643e 0a0a 3c62 6f64  e>.</head>..<bod
+00000440: 793e 0a3c 6469 7620 636c 6173 733d 2263  y>.<div class="c
+00000450: 6f6e 7461 696e 6572 223e 0a20 2020 203c  ontainer">.    <
+00000460: 6831 3e45 7374 6569 6420 5465 7374 2070  h1>Esteid Test p
+00000470: 6167 653c 2f68 313e 0a20 2020 203c 703e  age</h1>.    <p>
+00000480: 0a20 2020 2020 2020 2054 6869 7320 6973  .        This is
+00000490: 2061 2074 6573 7420 7061 6765 2066 6f72   a test page for
+000004a0: 203c 623e 6469 6769 7461 6c20 6175 7468   <b>digital auth
+000004b0: 656e 7469 6361 7469 6f6e 3c2f 623e 2e0a  entication</b>..
+000004c0: 2020 2020 3c2f 703e 0a0a 2020 2020 3c70      </p>..    <p
+000004d0: 2073 7479 6c65 3d22 666f 6e74 2d73 697a   style="font-siz
+000004e0: 653a 206c 6172 6765 7222 3e0a 2020 2020  e: larger">.    
+000004f0: 2020 2020 546f 2074 6573 7420 6f75 7420      To test out 
+00000500: 7369 676e 696e 672c 2070 6c65 6173 6520  signing, please 
+00000510: 3c61 2068 7265 663d 227b 2520 7572 6c20  <a href="{% url 
+00000520: 2273 6b5f 7465 7374 5f6e 6577 2220 257d  "sk_test_new" %}
+00000530: 223e 676f 2074 6f20 7468 6973 2070 6167  ">go to this pag
+00000540: 653c 2f61 3e2e 0a20 2020 203c 2f70 3e0a  e</a>..    </p>.
+00000550: 0a20 2020 203c 6834 3e53 6572 7669 6365  .    <h4>Service
+00000560: 7320 7365 7474 696e 6773 3c2f 6834 3e0a  s settings</h4>.
+00000570: 2020 2020 3c75 6c3e 0a20 2020 2020 2020      <ul>.       
+00000580: 203c 6c69 3e3c 623e 5573 6520 4445 4d4f   <li><b>Use DEMO
+00000590: 3a3c 2f62 3e20 7b7b 2045 5354 4549 445f  :</b> {{ ESTEID_
+000005a0: 4445 4d4f 7c79 6573 6e6f 207d 7d3c 2f6c  DEMO|yesno }}</l
+000005b0: 693e 0a20 2020 2020 2020 203c 6c69 3e3c  i>.        <li><
+000005c0: 623e 4944 2043 6172 643a 3c2f 623e 207b  b>ID Card:</b> {
+000005d0: 7b20 4944 5f43 4152 445f 454e 4142 4c45  { ID_CARD_ENABLE
+000005e0: 447c 7965 736e 6f20 7d7d 3c2f 6c69 3e0a  D|yesno }}</li>.
+000005f0: 2020 2020 2020 2020 3c6c 693e 3c62 3e4d          <li><b>M
+00000600: 6f62 696c 6520 4944 3a3c 2f62 3e20 7b7b  obile ID:</b> {{
+00000610: 204d 4f42 494c 455f 4944 5f45 4e41 424c   MOBILE_ID_ENABL
+00000620: 4544 7c79 6573 6e6f 207d 7d2c 2064 656d  ED|yesno }}, dem
+00000630: 6f3a 207b 7b20 4d4f 4249 4c45 5f49 445f  o: {{ MOBILE_ID_
+00000640: 5445 5354 5f4d 4f44 457c 7965 736e 6f20  TEST_MODE|yesno 
+00000650: 7d7d 3c2f 6c69 3e0a 2020 2020 2020 2020  }}</li>.        
+00000660: 3c6c 693e 3c62 3e53 4d41 5254 2049 443a  <li><b>SMART ID:
+00000670: 3c2f 623e 207b 7b20 534d 4152 545f 4944  </b> {{ SMART_ID
+00000680: 5f45 4e41 424c 4544 7c79 6573 6e6f 207d  _ENABLED|yesno }
+00000690: 7d2c 2064 656d 6f3a 207b 7b20 534d 4152  }, demo: {{ SMAR
+000006a0: 545f 4944 5f54 4553 545f 4d4f 4445 7c79  T_ID_TEST_MODE|y
+000006b0: 6573 6e6f 207d 7d3c 2f6c 693e 0a20 2020  esno }}</li>.   
+000006c0: 203c 2f75 6c3e 0a0a 2020 2020 3c68 343e   </ul>..    <h4>
+000006d0: 4e6f 7465 7320 6f6e 2053 6572 7669 6365  Notes on Service
+000006e0: 733c 2f68 343e 0a20 2020 203c 756c 3e0a  s</h4>.    <ul>.
+000006f0: 2020 2020 2020 2020 7b25 2069 6620 4d4f          {% if MO
+00000700: 4249 4c45 5f49 445f 5445 5354 5f4d 4f44  BILE_ID_TEST_MOD
+00000710: 4520 257d 0a20 2020 2020 2020 2020 2020  E %}.           
+00000720: 203c 6c69 3e0a 2020 2020 2020 2020 2020   <li>.          
+00000730: 2020 2020 2020 4d6f 6269 6c65 2049 4420        Mobile ID 
+00000740: 6175 7468 656e 7469 6361 7469 6f6e 2069  authentication i
+00000750: 7320 646f 6e65 2077 6974 6820 4465 6d6f  s done with Demo
+00000760: 204d 6f62 696c 6520 4944 2073 6572 7669   Mobile ID servi
+00000770: 6365 2c20 796f 7520 6361 6e20 6f6e 6c79  ce, you can only
+00000780: 2075 7365 2074 6865 0a20 2020 2020 2020   use the.       
+00000790: 2020 2020 2020 2020 203c 6120 6872 6566           <a href
+000007a0: 3d22 6874 7470 733a 2f2f 6769 7468 7562  ="https://github
+000007b0: 2e63 6f6d 2f53 4b2d 4549 442f 4d49 442f  .com/SK-EID/MID/
+000007c0: 7769 6b69 2f54 6573 742d 6e75 6d62 6572  wiki/Test-number
+000007d0: 2d66 6f72 2d61 7574 6f6d 6174 6564 2d74  -for-automated-t
+000007e0: 6573 7469 6e67 2d69 6e2d 4445 4d4f 2220  esting-in-DEMO" 
+000007f0: 7461 7267 6574 3d22 5f62 6c61 6e6b 223e  target="_blank">
+00000800: 6465 6d6f 0a20 2020 2020 2020 2020 2020  demo.           
+00000810: 2020 2020 2020 2020 2074 6573 7420 6e75           test nu
+00000820: 6d62 6572 733c 2f61 3e2e 0a20 2020 2020  mbers</a>..     
+00000830: 2020 2020 2020 203c 2f6c 693e 0a20 2020         </li>.   
+00000840: 2020 2020 207b 2520 656e 6469 6620 257d       {% endif %}
+00000850: 0a20 2020 2020 2020 207b 2520 6966 2045  .        {% if E
+00000860: 5354 4549 445f 4445 4d4f 2025 7d0a 2020  STEID_DEMO %}.  
+00000870: 2020 2020 2020 2020 2020 3c6c 693e 0a20            <li>. 
+00000880: 2020 2020 2020 2020 2020 2020 2020 2049                 I
+00000890: 4420 4361 7264 2061 7574 6865 6e74 6963  D Card authentic
+000008a0: 6174 696f 6e20 6361 6e20 6265 2064 6f6e  ation can be don
+000008b0: 6520 7769 7468 2072 6561 6c20 4944 2063  e with real ID c
+000008c0: 6172 6473 2e0a 2020 2020 2020 2020 2020  ards..          
+000008d0: 2020 3c2f 6c69 3e0a 2020 2020 2020 2020    </li>.        
+000008e0: 7b25 2065 6e64 6966 2025 7d0a 2020 2020  {% endif %}.    
+000008f0: 2020 2020 3c6c 693e 0a20 2020 2020 2020      <li>.       
+00000900: 2020 2020 2049 4420 4361 7264 2061 7574       ID Card aut
+00000910: 6865 6e74 6963 6174 696f 6e20 7265 7175  hentication requ
+00000920: 6972 6573 2074 6865 203c 623e 6368 726f  ires the <b>chro
+00000930: 6d65 2d74 6f6b 656e 2d73 6967 6e69 6e67  me-token-signing
+00000940: 3c2f 623e 2070 6c75 6769 6e20 666f 7220  </b> plugin for 
+00000950: 6368 726f 6d65 206f 7220 6669 7265 666f  chrome or firefo
+00000960: 782e 0a20 2020 2020 2020 203c 2f6c 693e  x..        </li>
+00000970: 0a20 2020 2020 2020 203c 6c69 3e0a 2020  .        <li>.  
+00000980: 2020 2020 2020 2020 2020 4944 2043 6172            ID Car
+00000990: 6420 6175 7468 656e 7469 6361 7469 6f6e  d authentication
+000009a0: 2072 6571 7569 7265 7320 4854 5450 532e   requires HTTPS.
+000009b0: 2050 6c65 6173 6520 7265 6665 7220 746f   Please refer to
+000009c0: 2074 6865 2052 4541 444d 452e 0a20 2020   the README..   
+000009d0: 2020 2020 203c 2f6c 693e 0a20 2020 2020       </li>.     
+000009e0: 2020 207b 2520 6966 2053 4d41 5254 5f49     {% if SMART_I
+000009f0: 445f 5445 5354 5f4d 4f44 4520 257d 0a20  D_TEST_MODE %}. 
+00000a00: 2020 2020 2020 2020 2020 203c 6c69 3e0a             <li>.
+00000a10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000a20: 4175 7468 656e 7469 6361 7469 6f6e 2077  Authentication w
+00000a30: 6974 6820 536d 6172 7449 4420 6361 6e20  ith SmartID can 
+00000a40: 6265 2074 6573 7465 6420 7769 7468 2074  be tested with t
+00000a50: 6865 2074 6573 7420 4944 2063 6f64 6573  he test ID codes
+00000a60: 2066 6f75 6e64 206f 6e20 7468 650a 2020   found on the.  
+00000a70: 2020 2020 2020 2020 2020 2020 2020 3c61                <a
+00000a80: 2068 7265 663d 2268 7474 7073 3a2f 2f67   href="https://g
+00000a90: 6974 6875 622e 636f 6d2f 534b 2d45 4944  ithub.com/SK-EID
+00000aa0: 2f73 6d61 7274 2d69 642d 646f 6375 6d65  /smart-id-docume
+00000ab0: 6e74 6174 696f 6e2f 7769 6b69 2f45 6e76  ntation/wiki/Env
+00000ac0: 6972 6f6e 6d65 6e74 2d74 6563 686e 6963  ironment-technic
+00000ad0: 616c 2d70 6172 616d 6574 6572 7322 0a20  al-parameters". 
+00000ae0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000af0: 2020 7461 7267 6574 3d22 5f62 6c61 6e6b    target="_blank
+00000b00: 223e 536d 6172 7449 4420 7769 6b69 2070  ">SmartID wiki p
+00000b10: 6167 653c 2f61 3e2e 0a20 2020 2020 2020  age</a>..       
+00000b20: 2020 2020 203c 2f6c 693e 0a20 2020 2020       </li>.     
+00000b30: 2020 2020 2020 203c 6c69 3e0a 2020 2020         <li>.    
+00000b40: 2020 2020 2020 2020 2020 2020 4175 7468              Auth
+00000b50: 656e 7469 6361 7469 6f6e 2077 6974 6820  entication with 
+00000b60: 3c65 6d3e 536d 6172 7449 4420 6465 6d6f  <em>SmartID demo
+00000b70: 2061 7070 3c2f 656d 3e20 2877 6865 7265   app</em> (where
+00000b80: 2079 6f75 2063 616e 2072 6563 6569 7665   you can receive
+00000b90: 2076 6572 6966 6963 6174 696f 6e20 636f   verification co
+00000ba0: 6465 7320 616e 6420 656e 7465 7220 5049  des and enter PI
+00000bb0: 4e73 290a 2020 2020 2020 2020 2020 2020  Ns).            
+00000bc0: 2020 2020 7265 7175 6972 6573 2073 6574      requires set
+00000bd0: 7469 6e67 2075 7020 6120 6465 6d6f 2053  ting up a demo S
+00000be0: 6d61 7274 4944 2061 6363 6f75 6e74 2e20  martID account. 
+00000bf0: 506c 6561 7365 2072 6566 6572 2074 6f20  Please refer to 
+00000c00: 7468 6520 5245 4144 4d45 2e0a 2020 2020  the README..    
+00000c10: 2020 2020 2020 2020 3c2f 6c69 3e0a 2020          </li>.  
+00000c20: 2020 2020 2020 7b25 2065 6e64 6966 2025        {% endif %
+00000c30: 7d0a 2020 2020 3c2f 756c 3e0a 0a20 2020  }.    </ul>..   
+00000c40: 203c 6872 202f 3e0a 0a20 2020 203c 6833   <hr />..    <h3
+00000c50: 3e43 686f 6f73 6520 6175 7468 656e 7469  >Choose authenti
+00000c60: 6361 7469 6f6e 206d 6574 686f 643c 2f68  cation method</h
+00000c70: 333e 0a0a 2020 2020 7b25 2069 6620 4944  3>..    {% if ID
+00000c80: 5f43 4152 445f 454e 4142 4c45 4420 257d  _CARD_ENABLED %}
+00000c90: 0a20 2020 2020 2020 203c 6120 6872 6566  .        <a href
+00000ca0: 3d22 2322 2069 643d 2273 6967 6e2d 6964  ="#" id="sign-id
+00000cb0: 223e 3c69 6d67 2061 6c74 3d22 4944 2043  "><img alt="ID C
+00000cc0: 6172 6422 2073 7263 3d22 7b25 2073 7461  ard" src="{% sta
+00000cd0: 7469 6320 2769 6d61 6765 732f 6573 7465  tic 'images/este
+00000ce0: 6964 2f69 642d 6b61 6172 742d 6c6f 676f  id/id-kaart-logo
+00000cf0: 2e67 6966 2720 257d 223e 3c2f 613e 0a20  .gif' %}"></a>. 
+00000d00: 2020 207b 2520 656e 6469 6620 257d 0a20     {% endif %}. 
+00000d10: 2020 207b 2520 6966 204d 4f42 494c 455f     {% if MOBILE_
+00000d20: 4944 5f45 4e41 424c 4544 2025 7d0a 2020  ID_ENABLED %}.  
+00000d30: 2020 2020 2020 3c61 2068 7265 663d 2223        <a href="#
+00000d40: 2220 6964 3d22 7369 676e 2d6d 6964 223e  " id="sign-mid">
+00000d50: 3c69 6d67 2061 6c74 3d22 4d6f 6269 6c65  <img alt="Mobile
+00000d60: 2049 4422 2073 7263 3d22 7b25 2073 7461   ID" src="{% sta
+00000d70: 7469 6320 2769 6d61 6765 732f 6573 7465  tic 'images/este
+00000d80: 6964 2f6d 6964 2d6c 6f67 6f2e 6769 6627  id/mid-logo.gif'
+00000d90: 2025 7d22 3e3c 2f61 3e0a 2020 2020 7b25   %}"></a>.    {%
+00000da0: 2065 6e64 6966 2025 7d0a 2020 2020 7b25   endif %}.    {%
+00000db0: 2069 6620 534d 4152 545f 4944 5f45 4e41   if SMART_ID_ENA
+00000dc0: 424c 4544 2025 7d0a 2020 2020 2020 2020  BLED %}.        
+00000dd0: 3c61 2068 7265 663d 2223 2220 6964 3d22  <a href="#" id="
+00000de0: 7369 676e 2d73 6d61 7274 6964 223e 3c69  sign-smartid"><i
+00000df0: 6d67 2061 6c74 3d22 536d 6172 7420 4944  mg alt="Smart ID
+00000e00: 220a 2020 2020 2020 2020 2020 2020 2020  ".              
+00000e10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000e20: 2020 2020 2020 2020 2020 2020 2073 7263               src
+00000e30: 3d22 7b25 2073 7461 7469 6320 2769 6d61  ="{% static 'ima
+00000e40: 6765 732f 6573 7465 6964 2f73 6d61 7274  ges/esteid/smart
+00000e50: 4944 2d6c 6f67 6f2d 6274 6e2e 706e 6727  ID-logo-btn.png'
+00000e60: 2025 7d22 3e3c 2f61 3e0a 2020 2020 7b25   %}"></a>.    {%
+00000e70: 2065 6e64 6966 2025 7d0a 0a20 2020 203c   endif %}..    <
+00000e80: 6872 202f 3e0a 0a3c 2f64 6976 3e0a 0a3c  hr />..</div>..<
+00000e90: 6469 7620 636c 6173 733d 226d 6f64 616c  div class="modal
+00000ea0: 2066 6164 6522 2069 643d 226d 6964 2d6d   fade" id="mid-m
+00000eb0: 6f64 616c 223e 0a20 2020 203c 6469 7620  odal">.    <div 
+00000ec0: 636c 6173 733d 226d 6f64 616c 2d64 6961  class="modal-dia
+00000ed0: 6c6f 6722 3e0a 2020 2020 2020 2020 3c66  log">.        <f
+00000ee0: 6f72 6d20 6e61 6d65 3d22 6d6f 6269 6c65  orm name="mobile
+00000ef0: 4964 223e 0a20 2020 2020 2020 2020 2020  Id">.           
+00000f00: 203c 6469 7620 636c 6173 733d 226d 6f64   <div class="mod
+00000f10: 616c 2d63 6f6e 7465 6e74 223e 0a20 2020  al-content">.   
+00000f20: 2020 2020 2020 2020 2020 2020 203c 6469               <di
+00000f30: 7620 636c 6173 733d 226d 6f64 616c 2d68  v class="modal-h
+00000f40: 6561 6465 7222 3e0a 2020 2020 2020 2020  eader">.        
+00000f50: 2020 2020 2020 2020 2020 2020 3c62 7574              <but
+00000f60: 746f 6e20 7479 7065 3d22 6275 7474 6f6e  ton type="button
+00000f70: 2220 636c 6173 733d 2263 6c6f 7365 2220  " class="close" 
+00000f80: 6461 7461 2d64 6973 6d69 7373 3d22 6d6f  data-dismiss="mo
+00000f90: 6461 6c22 2061 7269 612d 6c61 6265 6c3d  dal" aria-label=
+00000fa0: 2243 6c6f 7365 223e 3c73 7061 6e0a 2020  "Close"><span.  
 00000fb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000fc0: 2020 2020 2020 2020 3c6c 6162 656c 2066          <label f
-00000fd0: 6f72 3d22 6964 436f 6465 496e 7075 7422  or="idCodeInput"
-00000fe0: 3e44 656d 6f20 4944 2063 6f64 653a 3c2f  >Demo ID code:</
-00000ff0: 6c61 6265 6c3e 0a20 2020 2020 2020 2020  label>.         
-00001000: 2020 2020 2020 2020 2020 2020 2020 203c                 <
-00001010: 696e 7075 7420 7479 7065 3d22 7465 7874  input type="text
-00001020: 2220 6e61 6d65 3d22 6964 5f63 6f64 6522  " name="id_code"
-00001030: 2069 643d 2269 6443 6f64 6549 6e70 7574   id="idCodeInput
-00001040: 2220 636c 6173 733d 2266 6f72 6d2d 636f  " class="form-co
-00001050: 6e74 726f 6c22 0a20 2020 2020 2020 2020  ntrol".         
-00001060: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001070: 2020 2020 2020 7661 6c75 653d 227b 7b20        value="{{ 
-00001080: 7265 7175 6573 742e 7365 7373 696f 6e2e  request.session.
-00001090: 6464 6f63 5f74 6573 745f 6964 5f63 6f64  ddoc_test_id_cod
-000010a0: 6520 7c20 6465 6661 756c 743a 2736 3030  e | default:'600
-000010b0: 3031 3031 3939 3036 2720 7d7d 2220 2f3e  01019906' }}" />
-000010c0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000010d0: 2020 2020 203c 2f64 6976 3e0a 2020 2020       </div>.    
-000010e0: 2020 2020 2020 2020 2020 2020 3c2f 666f              </fo
-000010f0: 726d 3e0a 2020 2020 2020 2020 2020 2020  rm>.            
-00001100: 3c2f 6469 763e 0a0a 2020 2020 2020 2020  </div>..        
-00001110: 2020 2020 3c64 6976 2063 6c61 7373 3d22      <div class="
-00001120: 6d6f 6461 6c2d 666f 6f74 6572 223e 0a20  modal-footer">. 
-00001130: 2020 2020 2020 2020 2020 2020 2020 203c                 <
-00001140: 6275 7474 6f6e 2074 7970 653d 2262 7574  button type="but
-00001150: 746f 6e22 2063 6c61 7373 3d22 6274 6e20  ton" class="btn 
-00001160: 6274 6e2d 7072 696d 6172 7922 2069 643d  btn-primary" id=
-00001170: 2273 6967 6e4d 6f62 696c 6522 3e53 6967  "signMobile">Sig
-00001180: 6e3c 2f62 7574 746f 6e3e 0a20 2020 2020  n</button>.     
-00001190: 2020 2020 2020 203c 2f64 6976 3e0a 2020         </div>.  
-000011a0: 2020 2020 2020 3c2f 6469 763e 0a20 2020        </div>.   
-000011b0: 203c 2f64 6976 3e0a 3c2f 6469 763e 0a0a   </div>.</div>..
-000011c0: 3c64 6976 2063 6c61 7373 3d22 6d6f 6461  <div class="moda
-000011d0: 6c20 6661 6465 2220 6964 3d22 6368 616c  l fade" id="chal
-000011e0: 6c65 6e67 652d 6d6f 6461 6c22 3e0a 2020  lenge-modal">.  
-000011f0: 2020 3c64 6976 2063 6c61 7373 3d22 6d6f    <div class="mo
-00001200: 6461 6c2d 6469 616c 6f67 223e 0a20 2020  dal-dialog">.   
-00001210: 2020 2020 203c 6469 7620 636c 6173 733d       <div class=
-00001220: 226d 6f64 616c 2d63 6f6e 7465 6e74 223e  "modal-content">
-00001230: 0a20 2020 2020 2020 2020 2020 203c 6469  .            <di
-00001240: 7620 636c 6173 733d 226d 6f64 616c 2d68  v class="modal-h
-00001250: 6561 6465 7222 3e0a 2020 2020 2020 2020  eader">.        
-00001260: 2020 2020 2020 2020 3c68 3420 636c 6173          <h4 clas
-00001270: 733d 226d 6f64 616c 2d74 6974 6c65 223e  s="modal-title">
-00001280: 4d49 4420 5374 6570 2032 3c2f 6834 3e0a  MID Step 2</h4>.
-00001290: 2020 2020 2020 2020 2020 2020 3c2f 6469              </di
-000012a0: 763e 0a0a 2020 2020 2020 2020 2020 2020  v>..            
-000012b0: 3c64 6976 2063 6c61 7373 3d22 6d6f 6461  <div class="moda
-000012c0: 6c2d 626f 6479 223e 0a20 2020 2020 2020  l-body">.       
-000012d0: 2020 2020 2020 2020 203c 703e 0a20 2020           <p>.   
-000012e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000012f0: 2050 6c65 6173 6520 656e 7465 7220 7468   Please enter th
-00001300: 6520 666f 6c6c 6f77 696e 6720 636f 6465  e following code
-00001310: 2069 6e74 6f20 796f 7572 206d 6f62 696c   into your mobil
-00001320: 6520 746f 2070 726f 6365 6564 2077 6974  e to proceed wit
-00001330: 680a 2020 2020 2020 2020 2020 2020 2020  h.              
-00001340: 2020 2020 2020 7468 6520 7369 676e 696e        the signin
-00001350: 6720 7072 6f63 6573 733a 203c 6220 6964  g process: <b id
-00001360: 3d22 6368 616c 6c65 6e67 652d 636f 6465  ="challenge-code
-00001370: 223e 4b4f 4f44 3c2f 623e 0a20 2020 2020  ">KOOD</b>.     
-00001380: 2020 2020 2020 2020 2020 203c 2f70 3e0a             </p>.
-00001390: 2020 2020 2020 2020 2020 2020 3c2f 6469              </di
-000013a0: 763e 0a20 2020 2020 2020 203c 2f64 6976  v>.        </div
-000013b0: 3e0a 2020 2020 3c2f 6469 763e 0a3c 2f64  >.    </div>.</d
-000013c0: 6976 3e0a 0a3c 6469 7620 636c 6173 733d  iv>..<div class=
-000013d0: 226d 6f64 616c 2066 6164 6522 2069 643d  "modal fade" id=
-000013e0: 2269 642d 6d6f 6461 6c22 3e0a 2020 2020  "id-modal">.    
-000013f0: 3c64 6976 2063 6c61 7373 3d22 6d6f 6461  <div class="moda
-00001400: 6c2d 6469 616c 6f67 223e 0a20 2020 2020  l-dialog">.     
-00001410: 2020 203c 6469 7620 636c 6173 733d 226d     <div class="m
-00001420: 6f64 616c 2d63 6f6e 7465 6e74 223e 0a20  odal-content">. 
-00001430: 2020 2020 2020 2020 2020 203c 6469 7620             <div 
-00001440: 636c 6173 733d 226d 6f64 616c 2d68 6561  class="modal-hea
-00001450: 6465 7222 3e0a 2020 2020 2020 2020 2020  der">.          
-00001460: 2020 2020 2020 3c68 3420 636c 6173 733d        <h4 class=
-00001470: 226d 6f64 616c 2d74 6974 6c65 223e 5369  "modal-title">Si
-00001480: 676e 696e 6720 7769 7468 2064 6967 6974  gning with digit
-00001490: 616c 2049 443c 2f68 343e 0a20 2020 2020  al ID</h4>.     
-000014a0: 2020 2020 2020 203c 2f64 6976 3e0a 0a20         </div>.. 
-000014b0: 2020 2020 2020 2020 2020 203c 6469 7620             <div 
-000014c0: 636c 6173 733d 226d 6f64 616c 2d62 6f64  class="modal-bod
-000014d0: 7922 3e0a 2020 2020 2020 2020 2020 2020  y">.            
-000014e0: 2020 2020 3c70 3e0a 2020 2020 2020 2020      <p>.        
-000014f0: 2020 2020 2020 2020 2020 2020 506c 6561              Plea
-00001500: 7365 2066 6f6c 6c6f 7720 7468 6520 696e  se follow the in
-00001510: 7374 7275 6374 696f 6e73 2074 6f20 636f  structions to co
-00001520: 6d70 6c65 7465 2074 6865 2073 6967 6e69  mplete the signi
-00001530: 6e67 2070 726f 6365 7373 2e0a 2020 2020  ng process..    
-00001540: 2020 2020 2020 2020 2020 2020 3c2f 703e              </p>
-00001550: 0a20 2020 2020 2020 2020 2020 203c 2f64  .            </d
-00001560: 6976 3e0a 2020 2020 2020 2020 3c2f 6469  iv>.        </di
-00001570: 763e 0a20 2020 203c 2f64 6976 3e0a 3c2f  v>.    </div>.</
-00001580: 6469 763e 0a0a 3c64 6976 2063 6c61 7373  div>..<div class
-00001590: 3d22 6d6f 6461 6c20 6661 6465 2220 6964  ="modal fade" id
-000015a0: 3d22 736d 6172 7469 642d 6d6f 6461 6c22  ="smartid-modal"
-000015b0: 3e0a 2020 2020 3c64 6976 2063 6c61 7373  >.    <div class
-000015c0: 3d22 6d6f 6461 6c2d 6469 616c 6f67 223e  ="modal-dialog">
-000015d0: 0a20 2020 2020 2020 203c 6469 7620 636c  .        <div cl
-000015e0: 6173 733d 226d 6f64 616c 2d63 6f6e 7465  ass="modal-conte
-000015f0: 6e74 223e 0a20 2020 2020 2020 2020 2020  nt">.           
-00001600: 203c 6469 7620 636c 6173 733d 226d 6f64   <div class="mod
-00001610: 616c 2d68 6561 6465 7222 3e0a 2020 2020  al-header">.    
-00001620: 2020 2020 2020 2020 2020 2020 3c62 7574              <but
-00001630: 746f 6e20 7479 7065 3d22 6275 7474 6f6e  ton type="button
-00001640: 2220 636c 6173 733d 2263 6c6f 7365 2220  " class="close" 
-00001650: 6461 7461 2d64 6973 6d69 7373 3d22 6d6f  data-dismiss="mo
-00001660: 6461 6c22 2061 7269 612d 6c61 6265 6c3d  dal" aria-label=
-00001670: 2243 6c6f 7365 223e 3c73 7061 6e20 6172  "Close"><span ar
-00001680: 6961 2d68 6964 6465 6e3d 2274 7275 6522  ia-hidden="true"
-00001690: 3e26 7469 6d65 733b 3c2f 7370 616e 3e0a  >&times;</span>.
-000016a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000016b0: 3c2f 6275 7474 6f6e 3e0a 2020 2020 2020  </button>.      
-000016c0: 2020 2020 2020 2020 2020 3c68 3420 636c            <h4 cl
-000016d0: 6173 733d 226d 6f64 616c 2d74 6974 6c65  ass="modal-title
-000016e0: 223e 5369 676e 2074 6865 2066 696c 6573  ">Sign the files
-000016f0: 2077 6974 6820 536d 6172 7449 443c 2f68   with SmartID</h
-00001700: 343e 0a20 2020 2020 2020 2020 2020 203c  4>.            <
-00001710: 2f64 6976 3e0a 0a20 2020 2020 2020 2020  /div>..         
-00001720: 2020 203c 6469 7620 636c 6173 733d 226d     <div class="m
-00001730: 6f64 616c 2d62 6f64 7922 3e0a 2020 2020  odal-body">.    
-00001740: 2020 2020 2020 2020 2020 2020 3c66 6f72              <for
-00001750: 6d20 6e61 6d65 3d22 736d 6172 7449 6422  m name="smartId"
-00001760: 3e0a 2020 2020 2020 2020 2020 2020 2020  >.              
-00001770: 2020 2020 2020 3c64 6976 2063 6c61 7373        <div class
-00001780: 3d22 666f 726d 2d67 726f 7570 223e 0a20  ="form-group">. 
-00001790: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000017a0: 2020 2020 2020 203c 6c61 6265 6c20 666f         <label fo
-000017b0: 723d 2269 6443 6f64 6549 6e70 7574 223e  r="idCodeInput">
-000017c0: 596f 7572 2049 4420 636f 6465 3a3c 2f6c  Your ID code:</l
-000017d0: 6162 656c 3e0a 2020 2020 2020 2020 2020  abel>.          
-000017e0: 2020 2020 2020 2020 2020 2020 2020 3c69                <i
-000017f0: 6e70 7574 2074 7970 653d 2274 6578 7422  nput type="text"
-00001800: 206e 616d 653d 2269 645f 636f 6465 2220   name="id_code" 
-00001810: 6964 3d22 6964 436f 6465 496e 7075 7422  id="idCodeInput"
-00001820: 2063 6c61 7373 3d22 666f 726d 2d63 6f6e   class="form-con
-00001830: 7472 6f6c 220a 2020 2020 2020 2020 2020  trol".          
-00001840: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001850: 2020 2020 2076 616c 7565 3d22 7b7b 2072       value="{{ r
-00001860: 6571 7565 7374 2e73 6573 7369 6f6e 2e73  equest.session.s
-00001870: 6d61 7274 6964 5f74 6573 745f 6964 5f63  martid_test_id_c
-00001880: 6f64 6520 7c20 6465 6661 756c 743a 2733  ode | default:'3
-00001890: 3033 3033 3033 3939 3134 2720 7d7d 2220  0303039914' }}" 
-000018a0: 2f3e 0a20 2020 2020 2020 2020 2020 2020  />.             
-000018b0: 2020 2020 2020 203c 2f64 6976 3e0a 2020         </div>.  
-000018c0: 2020 2020 2020 2020 2020 2020 2020 3c2f                </
-000018d0: 666f 726d 3e0a 2020 2020 2020 2020 2020  form>.          
-000018e0: 2020 3c2f 6469 763e 0a0a 2020 2020 2020    </div>..      
-000018f0: 2020 2020 2020 3c64 6976 2063 6c61 7373        <div class
-00001900: 3d22 6d6f 6461 6c2d 666f 6f74 6572 223e  ="modal-footer">
-00001910: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00001920: 203c 6275 7474 6f6e 2074 7970 653d 2262   <button type="b
-00001930: 7574 746f 6e22 2063 6c61 7373 3d22 6274  utton" class="bt
-00001940: 6e20 6274 6e2d 7072 696d 6172 7922 2069  n btn-primary" i
-00001950: 643d 2273 6967 6e2d 736d 6172 7469 642d  d="sign-smartid-
-00001960: 6275 7474 6f6e 223e 5369 676e 3c2f 6275  button">Sign</bu
-00001970: 7474 6f6e 3e0a 2020 2020 2020 2020 2020  tton>.          
-00001980: 2020 3c2f 6469 763e 0a20 2020 2020 2020    </div>.       
-00001990: 203c 2f64 6976 3e0a 2020 2020 3c2f 6469   </div>.    </di
-000019a0: 763e 0a3c 2f64 6976 3e0a 0a3c 6469 7620  v>.</div>..<div 
-000019b0: 636c 6173 733d 226d 6f64 616c 2066 6164  class="modal fad
-000019c0: 6522 2069 643d 2276 6572 6966 6963 6174  e" id="verificat
-000019d0: 696f 6e2d 636f 6465 2d6d 6f64 616c 223e  ion-code-modal">
-000019e0: 0a20 2020 203c 6469 7620 636c 6173 733d  .    <div class=
-000019f0: 226d 6f64 616c 2d64 6961 6c6f 6722 3e0a  "modal-dialog">.
-00001a00: 2020 2020 2020 2020 3c64 6976 2063 6c61          <div cla
-00001a10: 7373 3d22 6d6f 6461 6c2d 636f 6e74 656e  ss="modal-conten
-00001a20: 7422 3e0a 2020 2020 2020 2020 2020 2020  t">.            
-00001a30: 3c64 6976 2063 6c61 7373 3d22 6d6f 6461  <div class="moda
-00001a40: 6c2d 6865 6164 6572 223e 0a20 2020 2020  l-header">.     
-00001a50: 2020 2020 2020 2020 2020 203c 6834 2063             <h4 c
-00001a60: 6c61 7373 3d22 6d6f 6461 6c2d 7469 746c  lass="modal-titl
-00001a70: 6522 3e56 6572 6966 6963 6174 696f 6e20  e">Verification 
-00001a80: 636f 6465 3c2f 6834 3e0a 2020 2020 2020  code</h4>.      
-00001a90: 2020 2020 2020 3c2f 6469 763e 0a0a 2020        </div>..  
-00001aa0: 2020 2020 2020 2020 2020 3c64 6976 2063            <div c
-00001ab0: 6c61 7373 3d22 6d6f 6461 6c2d 626f 6479  lass="modal-body
-00001ac0: 223e 0a20 2020 2020 2020 2020 2020 2020  ">.             
-00001ad0: 2020 203c 703e 0a20 2020 2020 2020 2020     <p>.         
-00001ae0: 2020 2020 2020 2020 2020 204d 616b 6520             Make 
-00001af0: 7375 7265 2079 6f75 2061 7265 2073 6565  sure you are see
-00001b00: 696e 6720 7468 6973 2076 6572 6966 6963  ing this verific
-00001b10: 6174 696f 6e20 636f 6465 206f 6e20 796f  ation code on yo
-00001b20: 7572 2064 6576 6963 653a 0a20 2020 2020  ur device:.     
-00001b30: 2020 2020 2020 2020 2020 2020 2020 203c                 <
-00001b40: 6220 6964 3d22 736d 6172 7469 642d 7665  b id="smartid-ve
-00001b50: 7269 6669 6361 7469 6f6e 2d63 6f64 6522  rification-code"
-00001b60: 3e4b 4f4f 443c 2f62 3e0a 2020 2020 2020  >KOOD</b>.      
-00001b70: 2020 2020 2020 2020 2020 3c2f 703e 0a20            </p>. 
-00001b80: 2020 2020 2020 2020 2020 203c 2f64 6976             </div
-00001b90: 3e0a 2020 2020 2020 2020 3c2f 6469 763e  >.        </div>
-00001ba0: 0a20 2020 203c 2f64 6976 3e0a 3c2f 6469  .    </div>.</di
-00001bb0: 763e 0a0a 3c64 6976 2063 6c61 7373 3d22  v>..<div class="
-00001bc0: 6d6f 6461 6c20 6661 6465 2220 6964 3d22  modal fade" id="
-00001bd0: 7375 6363 6573 732d 6d6f 6461 6c22 3e0a  success-modal">.
-00001be0: 2020 2020 3c64 6976 2063 6c61 7373 3d22      <div class="
-00001bf0: 6d6f 6461 6c2d 6469 616c 6f67 223e 0a20  modal-dialog">. 
-00001c00: 2020 2020 2020 203c 6469 7620 636c 6173         <div clas
-00001c10: 733d 226d 6f64 616c 2d63 6f6e 7465 6e74  s="modal-content
-00001c20: 223e 0a20 2020 2020 2020 2020 2020 203c  ">.            <
-00001c30: 6469 7620 636c 6173 733d 226d 6f64 616c  div class="modal
-00001c40: 2d68 6561 6465 7222 3e0a 2020 2020 2020  -header">.      
-00001c50: 2020 2020 2020 2020 2020 3c68 3420 636c            <h4 cl
-00001c60: 6173 733d 226d 6f64 616c 2d74 6974 6c65  ass="modal-title
-00001c70: 223e 5369 676e 696e 6720 636f 6d70 6c65  ">Signing comple
-00001c80: 7465 3c2f 6834 3e0a 2020 2020 2020 2020  te</h4>.        
-00001c90: 2020 2020 3c2f 6469 763e 0a0a 2020 2020      </div>..    
-00001ca0: 2020 2020 2020 2020 3c64 6976 2063 6c61          <div cla
-00001cb0: 7373 3d22 6d6f 6461 6c2d 626f 6479 223e  ss="modal-body">
-00001cc0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00001cd0: 203c 703e 0a20 2020 2020 2020 2020 2020   <p>.           
-00001ce0: 2020 2020 2020 2020 2054 6865 2075 706c           The upl
-00001cf0: 6f61 6465 6420 6669 6c65 7320 7765 7265  oaded files were
-00001d00: 2073 7563 6365 7373 6675 6c6c 7920 6469   successfully di
-00001d10: 6769 7461 6c6c 7920 7369 676e 6564 2c20  gitally signed, 
-00001d20: 706c 6561 7365 2063 6c69 636b 2074 6865  please click the
-00001d30: 2066 6f6c 6c6f 7769 6e67 206c 696e 6b0a   following link.
-00001d40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001d50: 2020 2020 746f 2064 6f77 6e6c 6f61 6420      to download 
-00001d60: 7468 6520 636f 6e74 6169 6e65 7220 616e  the container an
-00001d70: 6420 6669 6e69 7368 2074 6865 2073 6967  d finish the sig
-00001d80: 6e69 6e67 2070 726f 6365 7373 2e0a 2020  ning process..  
-00001d90: 2020 2020 2020 2020 2020 2020 2020 3c2f                </
-00001da0: 703e 0a0a 2020 2020 2020 2020 2020 2020  p>..            
-00001db0: 2020 2020 3c61 2068 7265 663d 2223 2220      <a href="#" 
-00001dc0: 6964 3d22 6765 742d 646f 6375 6d65 6e74  id="get-document
-00001dd0: 2220 7461 7267 6574 3d22 5f62 6c61 6e6b  " target="_blank
-00001de0: 223e 446f 776e 6c6f 6164 2066 696c 653c  ">Download file<
-00001df0: 2f61 3e0a 2020 2020 2020 2020 2020 2020  /a>.            
-00001e00: 3c2f 6469 763e 0a20 2020 2020 2020 203c  </div>.        <
-00001e10: 2f64 6976 3e0a 2020 2020 3c2f 6469 763e  /div>.    </div>
-00001e20: 0a3c 2f64 6976 3e0a 0a3c 7363 7269 7074  .</div>..<script
-00001e30: 2073 7263 3d22 2f2f 616a 6178 2e67 6f6f   src="//ajax.goo
-00001e40: 676c 6561 7069 732e 636f 6d2f 616a 6178  gleapis.com/ajax
-00001e50: 2f6c 6962 732f 6a71 7565 7279 2f31 2e31  /libs/jquery/1.1
-00001e60: 312e 312f 6a71 7565 7279 2e6d 696e 2e6a  1.1/jquery.min.j
-00001e70: 7322 3e3c 2f73 6372 6970 743e 0a3c 7363  s"></script>.<sc
-00001e80: 7269 7074 2073 7263 3d22 2f2f 6d61 7863  ript src="//maxc
-00001e90: 646e 2e62 6f6f 7473 7472 6170 6364 6e2e  dn.bootstrapcdn.
-00001ea0: 636f 6d2f 626f 6f74 7374 7261 702f 332e  com/bootstrap/3.
-00001eb0: 332e 342f 6a73 2f62 6f6f 7473 7472 6170  3.4/js/bootstrap
-00001ec0: 2e6d 696e 2e6a 7322 3e3c 2f73 6372 6970  .min.js"></scrip
-00001ed0: 743e 0a0a 3c73 6372 6970 7420 7479 7065  t>..<script type
-00001ee0: 3d22 7465 7874 2f6a 6176 6173 6372 6970  ="text/javascrip
-00001ef0: 7422 2073 7263 3d22 7b25 2073 7461 7469  t" src="{% stati
-00001f00: 6320 2765 7374 6569 642d 6865 6c70 6572  c 'esteid-helper
-00001f10: 2f77 6562 2d65 6964 2e6a 7327 2025 7d22  /web-eid.js' %}"
-00001f20: 3e3c 2f73 6372 6970 743e 0a3c 7363 7269  ></script>.<scri
-00001f30: 7074 2074 7970 653d 2274 6578 742f 6a61  pt type="text/ja
-00001f40: 7661 7363 7269 7074 2220 7372 633d 227b  vascript" src="{
-00001f50: 2520 7374 6174 6963 2027 6573 7465 6964  % static 'esteid
-00001f60: 2d68 656c 7065 722f 4573 7465 6964 2e6d  -helper/Esteid.m
-00001f70: 6169 6e2e 7765 622e 6a73 2720 257d 223e  ain.web.js' %}">
-00001f80: 3c2f 7363 7269 7074 3e0a 0a3c 7363 7269  </script>..<scri
-00001f90: 7074 2074 7970 653d 2274 6578 742f 6a61  pt type="text/ja
-00001fa0: 7661 7363 7269 7074 223e 0a20 2020 2024  vascript">.    $
-00001fb0: 2866 756e 6374 696f 6e20 2829 207b 0a20  (function () {. 
-00001fc0: 2020 2020 2020 2076 6172 2063 7372 665f         var csrf_
-00001fd0: 746f 6b65 6e20 3d20 277b 7b20 6373 7266  token = '{{ csrf
-00001fe0: 5f74 6f6b 656e 207d 7d27 0a20 2020 2020  _token }}'.     
-00001ff0: 2020 2076 6172 2064 6f77 6e6c 6f61 6455     var downloadU
-00002000: 726c 203d 2027 7b25 2075 726c 2027 646f  rl = '{% url 'do
-00002010: 776e 6c6f 6164 5f73 6967 6e65 645f 636f  wnload_signed_co
-00002020: 6e74 6169 6e65 7227 2025 7d27 0a20 2020  ntainer' %}'.   
-00002030: 2020 2020 2076 6172 206d 616e 6167 6572       var manager
-00002040: 203d 206e 6577 2045 7374 6569 642e 4c65   = new Esteid.Le
-00002050: 6761 6379 4964 656e 7469 6669 6361 7469  gacyIdentificati
-00002060: 6f6e 4d61 6e61 6765 7228 7b0a 2020 2020  onManager({.    
-00002070: 2020 2020 2020 2020 6c61 6e67 7561 6765          language
-00002080: 3a20 4573 7465 6964 2e4c 616e 6775 6167  : Esteid.Languag
-00002090: 6573 2e45 542c 0a0a 2020 2020 2020 2020  es.ET,..        
-000020a0: 2020 2020 6964 456e 6470 6f69 6e74 733a      idEndpoints:
-000020b0: 207b 0a20 2020 2020 2020 2020 2020 2020   {.             
-000020c0: 2020 2073 7461 7274 3a20 277b 2520 7572     start: '{% ur
-000020d0: 6c20 2774 6573 745f 6964 5f73 7461 7274  l 'test_id_start
-000020e0: 2720 257d 272c 0a20 2020 2020 2020 2020  ' %}',.         
-000020f0: 2020 2020 2020 2066 696e 6973 683a 2027         finish: '
-00002100: 7b25 2075 726c 2027 7465 7374 5f69 645f  {% url 'test_id_
-00002110: 6669 6e69 7368 2720 257d 272c 0a20 2020  finish' %}',.   
-00002120: 2020 2020 2020 2020 207d 2c0a 0a20 2020           },..   
-00002130: 2020 2020 2020 2020 206d 6964 456e 6470           midEndp
-00002140: 6f69 6e74 733a 207b 0a20 2020 2020 2020  oints: {.       
-00002150: 2020 2020 2020 2020 2073 7461 7274 3a20           start: 
-00002160: 277b 2520 7572 6c20 2774 6573 745f 6d69  '{% url 'test_mi
-00002170: 645f 7374 6172 7427 2025 7d27 2c0a 2020  d_start' %}',.  
-00002180: 2020 2020 2020 2020 2020 2020 2020 7374                st
-00002190: 6174 7573 3a20 277b 2520 7572 6c20 2774  atus: '{% url 't
-000021a0: 6573 745f 6d69 645f 7374 6174 7573 2720  est_mid_status' 
-000021b0: 257d 272c 0a20 2020 2020 2020 2020 2020  %}',.           
-000021c0: 207d 2c0a 0a20 2020 2020 2020 2020 2020   },..           
-000021d0: 2073 6d61 7274 6964 456e 6470 6f69 6e74   smartidEndpoint
-000021e0: 733a 207b 0a20 2020 2020 2020 2020 2020  s: {.           
-000021f0: 2020 2020 2073 7461 7274 3a20 277b 2520       start: '{% 
-00002200: 7572 6c20 2774 6573 745f 736d 6172 7469  url 'test_smarti
-00002210: 645f 7374 6172 7427 2025 7d27 2c0a 2020  d_start' %}',.  
-00002220: 2020 2020 2020 2020 2020 2020 2020 7374                st
-00002230: 6174 7573 3a20 277b 2520 7572 6c20 2774  atus: '{% url 't
-00002240: 6573 745f 736d 6172 7469 645f 7374 6174  est_smartid_stat
-00002250: 7573 2720 257d 272c 0a20 2020 2020 2020  us' %}',.       
-00002260: 2020 2020 207d 0a20 2020 2020 2020 207d       }.        }
-00002270: 290a 0a20 2020 2020 2020 2066 756e 6374  )..        funct
-00002280: 696f 6e20 6f6e 5369 676e 6564 2829 207b  ion onSigned() {
-00002290: 0a20 2020 2020 2020 2020 2020 2024 2827  .            $('
-000022a0: 2367 6574 2d64 6f63 756d 656e 7427 292e  #get-document').
-000022b0: 6174 7472 2827 6872 6566 272c 2064 6f77  attr('href', dow
-000022c0: 6e6c 6f61 6455 726c 290a 0a20 2020 2020  nloadUrl)..     
-000022d0: 2020 2020 2020 2024 2827 2373 7563 6365         $('#succe
-000022e0: 7373 2d6d 6f64 616c 2729 2e6d 6f64 616c  ss-modal').modal
-000022f0: 287b 0a20 2020 2020 2020 2020 2020 2020  ({.             
-00002300: 2020 2062 6163 6b64 726f 703a 2027 7374     backdrop: 'st
-00002310: 6174 6963 272c 0a20 2020 2020 2020 2020  atic',.         
-00002320: 2020 2020 2020 206b 6579 626f 6172 643a         keyboard:
-00002330: 2066 616c 7365 0a20 2020 2020 2020 2020   false.         
-00002340: 2020 207d 290a 2020 2020 2020 2020 7d0a     }).        }.
-00002350: 0a20 2020 2020 2020 2024 2827 2373 6967  .        $('#sig
-00002360: 6e2d 6d69 6427 292e 6f6e 2827 636c 6963  n-mid').on('clic
-00002370: 6b27 2c20 6675 6e63 7469 6f6e 2028 6529  k', function (e)
-00002380: 207b 0a20 2020 2020 2020 2020 2020 2065   {.            e
-00002390: 2e70 7265 7665 6e74 4465 6661 756c 7428  .preventDefault(
-000023a0: 290a 0a20 2020 2020 2020 2020 2020 2024  )..            $
-000023b0: 2827 236d 6964 2d6d 6f64 616c 2729 2e6d  ('#mid-modal').m
-000023c0: 6f64 616c 2829 0a20 2020 2020 2020 207d  odal().        }
-000023d0: 290a 0a20 2020 2020 2020 2066 756e 6374  )..        funct
-000023e0: 696f 6e20 7369 676e 4d6f 6269 6c65 4944  ion signMobileID
-000023f0: 2865 2920 7b0a 2020 2020 2020 2020 2020  (e) {.          
-00002400: 2020 652e 7072 6576 656e 7444 6566 6175    e.preventDefau
-00002410: 6c74 2829 0a20 2020 2020 2020 2020 2020  lt().           
-00002420: 2076 6172 206d 6f62 696c 6549 6446 6f72   var mobileIdFor
-00002430: 6d20 3d20 646f 6375 6d65 6e74 2e66 6f72  m = document.for
-00002440: 6d73 2e6d 6f62 696c 6549 640a 2020 2020  ms.mobileId.    
-00002450: 2020 2020 2020 2020 7661 7220 7068 6f6e          var phon
-00002460: 654e 7220 3d20 6d6f 6269 6c65 4964 466f  eNr = mobileIdFo
-00002470: 726d 2e70 686f 6e65 5f6e 722e 7661 6c75  rm.phone_nr.valu
-00002480: 650a 2020 2020 2020 2020 2020 2020 7661  e.            va
-00002490: 7220 6964 436f 6465 203d 206d 6f62 696c  r idCode = mobil
-000024a0: 6549 6446 6f72 6d2e 6964 5f63 6f64 652e  eIdForm.id_code.
-000024b0: 7661 6c75 650a 0a20 2020 2020 2020 2020  value..         
-000024c0: 2020 2069 6620 2821 7068 6f6e 654e 7229     if (!phoneNr)
-000024d0: 207b 0a20 2020 2020 2020 2020 2020 2020   {.             
-000024e0: 2020 2061 6c65 7274 2827 506c 6561 7365     alert('Please
-000024f0: 2065 6e74 6572 2061 2070 686f 6e65 206e   enter a phone n
-00002500: 756d 6265 7227 290a 2020 2020 2020 2020  umber').        
-00002510: 2020 2020 2020 2020 7265 7475 726e 0a20          return. 
-00002520: 2020 2020 2020 2020 2020 207d 0a20 2020             }.   
-00002530: 2020 2020 2020 2020 2069 6620 2821 6964           if (!id
-00002540: 436f 6465 2920 7b0a 2020 2020 2020 2020  Code) {.        
-00002550: 2020 2020 2020 2020 616c 6572 7428 2750          alert('P
-00002560: 6c65 6173 6520 656e 7465 7220 616e 2049  lease enter an I
-00002570: 4420 636f 6465 2729 0a20 2020 2020 2020  D code').       
-00002580: 2020 2020 2020 2020 2072 6574 7572 6e0a           return.
-00002590: 2020 2020 2020 2020 2020 2020 7d0a 0a20              }.. 
-000025a0: 2020 2020 2020 2020 2020 2063 6f6e 736f             conso
-000025b0: 6c65 2e6c 6f67 2827 4d49 443a 2073 6967  le.log('MID: sig
-000025c0: 6e69 6e67 2077 6974 6820 7068 6f6e 654e  ning with phoneN
-000025d0: 7227 2c20 7068 6f6e 654e 722c 2027 616e  r', phoneNr, 'an
-000025e0: 6420 6964 2063 6f64 6527 2c20 6964 436f  d id code', idCo
-000025f0: 6465 290a 0a20 2020 2020 2020 2020 2020  de)..           
-00002600: 202f 2f20 4361 6c6c 2049 6465 6e74 6966   // Call Identif
-00002610: 6963 6174 696f 6e4d 616e 6167 6572 2e73  icationManager.s
-00002620: 6967 6e20 7768 6963 6820 6361 6c6c 7320  ign which calls 
-00002630: 7468 6520 6261 636b 656e 6420 656e 6470  the backend endp
-00002640: 6f69 6e74 2074 6f20 7374 6172 7420 6d6f  oint to start mo
-00002650: 6269 6c65 4964 2073 6967 6e69 6e67 2070  bileId signing p
-00002660: 726f 6365 7373 0a20 2020 2020 2020 2020  rocess.         
-00002670: 2020 206d 616e 6167 6572 2e73 6967 6e57     manager.signW
-00002680: 6974 684d 6f62 696c 6549 6428 7b0a 2020  ithMobileId({.  
-00002690: 2020 2020 2020 2020 2020 2020 2020 7068                ph
-000026a0: 6f6e 655f 6e72 3a20 7068 6f6e 654e 722c  one_nr: phoneNr,
-000026b0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000026c0: 2069 645f 636f 6465 3a20 6964 436f 6465   id_code: idCode
-000026d0: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-000026e0: 2020 6373 7266 6d69 6464 6c65 7761 7265    csrfmiddleware
-000026f0: 746f 6b65 6e3a 2063 7372 665f 746f 6b65  token: csrf_toke
-00002700: 6e0a 2020 2020 2020 2020 2020 2020 7d29  n.            })
-00002710: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00002720: 202e 7468 656e 2866 756e 6374 696f 6e20   .then(function 
-00002730: 2872 6573 706f 6e73 6529 207b 0a20 2020  (response) {.   
-00002740: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002750: 2063 6f6e 736f 6c65 2e6c 6f67 2827 4d49   console.log('MI
-00002760: 443a 2067 6f74 2076 6572 6966 6963 6174  D: got verificat
-00002770: 696f 6e20 636f 6465 272c 2072 6573 706f  ion code', respo
-00002780: 6e73 652e 7665 7269 6669 6361 7469 6f6e  nse.verification
-00002790: 5f63 6f64 6529 0a0a 2020 2020 2020 2020  _code)..        
-000027a0: 2020 2020 2020 2020 2020 2020 2f2f 2047              // G
-000027b0: 6f74 2072 6573 706f 6e73 652c 2073 686f  ot response, sho
-000027c0: 7720 6368 616c 6c65 6e67 6520 6d6f 6461  w challenge moda
-000027d0: 6c0a 2020 2020 2020 2020 2020 2020 2020  l.              
-000027e0: 2020 2020 2020 2428 2723 6368 616c 6c65        $('#challe
-000027f0: 6e67 652d 636f 6465 2729 2e74 6578 7428  nge-code').text(
-00002800: 7265 7370 6f6e 7365 2e76 6572 6966 6963  response.verific
-00002810: 6174 696f 6e5f 636f 6465 290a 2020 2020  ation_code).    
-00002820: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002830: 2428 2723 6368 616c 6c65 6e67 652d 6d6f  $('#challenge-mo
-00002840: 6461 6c27 292e 6d6f 6461 6c28 7b0a 2020  dal').modal({.  
-00002850: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002860: 2020 2020 2020 6261 636b 6472 6f70 3a20        backdrop: 
-00002870: 2773 7461 7469 6327 2c0a 2020 2020 2020  'static',.      
-00002880: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002890: 2020 6b65 7962 6f61 7264 3a20 6661 6c73    keyboard: fals
-000028a0: 650a 2020 2020 2020 2020 2020 2020 2020  e.              
-000028b0: 2020 2020 2020 7d29 0a0a 2020 2020 2020        })..      
-000028c0: 2020 2020 2020 2020 2020 2020 2020 2428                $(
-000028d0: 2723 6d69 642d 6d6f 6461 6c27 292e 6d6f  '#mid-modal').mo
-000028e0: 6461 6c28 2768 6964 6527 290a 0a20 2020  dal('hide')..   
-000028f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002900: 206d 616e 6167 6572 2e6d 6964 5374 6174   manager.midStat
-00002910: 7573 287b 6373 7266 6d69 6464 6c65 7761  us({csrfmiddlewa
-00002920: 7265 746f 6b65 6e3a 2063 7372 665f 746f  retoken: csrf_to
-00002930: 6b65 6e7d 292e 7468 656e 280a 2020 2020  ken}).then(.    
-00002940: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002950: 2020 2020 6675 6e63 7469 6f6e 2028 2920      function () 
-00002960: 7b0a 2020 2020 2020 2020 2020 2020 2020  {.              
-00002970: 2020 2020 2020 2020 2020 2020 2020 2428                $(
-00002980: 2723 6368 616c 6c65 6e67 652d 6d6f 6461  '#challenge-moda
-00002990: 6c27 292e 6d6f 6461 6c28 2768 6964 6527  l').modal('hide'
-000029a0: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
-000029b0: 2020 2020 2020 2020 2020 2020 2020 6f6e                on
-000029c0: 5369 676e 6564 2829 0a20 2020 2020 2020  Signed().       
-000029d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000029e0: 207d 2c0a 0a20 2020 2020 2020 2020 2020   },..           
-000029f0: 2020 2020 2020 2020 2020 2020 2066 756e               fun
-00002a00: 6374 696f 6e20 2872 6573 2920 7b0a 2020  ction (res) {.  
-00002a10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002a20: 2020 2020 2020 2020 2020 6966 2028 7265            if (re
-00002a30: 732e 6d65 7373 6167 6529 207b 0a20 2020  s.message) {.   
-00002a40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002a50: 2020 2020 2020 2020 2020 2020 2061 6c65               ale
-00002a60: 7274 2872 6573 2e6d 6573 7361 6765 202b  rt(res.message +
-00002a70: 2027 2050 6c65 6173 6520 7472 7920 6167   ' Please try ag
-00002a80: 6169 6e27 290a 2020 2020 2020 2020 2020  ain').          
-00002a90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002aa0: 2020 7d20 656c 7365 207b 0a20 2020 2020    } else {.     
-00002ab0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002ac0: 2020 2020 2020 2020 2020 2061 6c65 7274             alert
-00002ad0: 2827 536f 6d65 7468 696e 6720 7765 6e74  ('Something went
-00002ae0: 2077 726f 6e67 2c20 706c 6561 7365 2074   wrong, please t
-00002af0: 7279 2061 6761 696e 2729 0a20 2020 2020  ry again').     
-00002b00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002b10: 2020 2020 2020 207d 0a0a 2020 2020 2020         }..      
-00002b20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002b30: 2020 2020 2020 2428 2723 6368 616c 6c65        $('#challe
-00002b40: 6e67 652d 6d6f 6461 6c27 292e 6d6f 6461  nge-modal').moda
-00002b50: 6c28 2768 6964 6527 290a 2020 2020 2020  l('hide').      
-00002b60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002b70: 2020 7d0a 2020 2020 2020 2020 2020 2020    }.            
-00002b80: 2020 2020 2020 2020 290a 0a20 2020 2020          )..     
-00002b90: 2020 2020 2020 2020 2020 207d 2c20 6675             }, fu
-00002ba0: 6e63 7469 6f6e 2028 7265 7329 207b 0a20  nction (res) {. 
-00002bb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002bc0: 2020 2069 6620 2872 6573 2026 2620 7265     if (res && re
-00002bd0: 732e 6d65 7373 6167 6529 207b 0a20 2020  s.message) {.   
-00002be0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002bf0: 2020 2020 2061 6c65 7274 2827 4d49 4420       alert('MID 
-00002c00: 5265 7370 6f6e 7365 5b27 202b 2072 6573  Response[' + res
-00002c10: 2e65 7272 6f72 5f63 6f64 6520 2b20 275d  .error_code + ']
-00002c20: 3a20 2720 2b20 7265 732e 6d65 7373 6167  : ' + res.messag
-00002c30: 6529 0a20 2020 2020 2020 2020 2020 2020  e).             
-00002c40: 2020 2020 2020 207d 2065 6c73 6520 7b0a         } else {.
-00002c50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002c60: 2020 2020 2020 2020 616c 6572 7428 2753          alert('S
-00002c70: 6f6d 6574 6869 6e67 2077 656e 7420 7772  omething went wr
-00002c80: 6f6e 672c 2070 6c65 6173 6520 7472 7920  ong, please try 
-00002c90: 6167 6169 6e27 290a 2020 2020 2020 2020  again').        
-00002ca0: 2020 2020 2020 2020 2020 2020 7d0a 2020              }.  
-00002cb0: 2020 2020 2020 2020 2020 2020 2020 7d29                })
-00002cc0: 0a20 2020 2020 2020 207d 0a0a 2020 2020  .        }..    
-00002cd0: 2020 2020 2428 2723 7369 676e 2d73 6d61      $('#sign-sma
-00002ce0: 7274 6964 2729 2e6f 6e28 2763 6c69 636b  rtid').on('click
-00002cf0: 272c 2066 756e 6374 696f 6e20 2865 2920  ', function (e) 
-00002d00: 7b0a 2020 2020 2020 2020 2020 2020 652e  {.            e.
-00002d10: 7072 6576 656e 7444 6566 6175 6c74 2829  preventDefault()
-00002d20: 0a0a 2020 2020 2020 2020 2020 2020 2428  ..            $(
-00002d30: 2723 736d 6172 7469 642d 6d6f 6461 6c27  '#smartid-modal'
-00002d40: 292e 6d6f 6461 6c28 290a 2020 2020 2020  ).modal().      
-00002d50: 2020 7d29 0a0a 2020 2020 2020 2020 6675    })..        fu
-00002d60: 6e63 7469 6f6e 206f 6e45 7272 6f72 2872  nction onError(r
-00002d70: 6573 2920 7b0a 2020 2020 2020 2020 2020  es) {.          
-00002d80: 2020 6966 2028 7265 7320 2626 2072 6573    if (res && res
-00002d90: 2e6d 6573 7361 6765 2920 7b0a 2020 2020  .message) {.    
-00002da0: 2020 2020 2020 2020 2020 2020 616c 6572              aler
-00002db0: 7428 2753 6d61 7274 4944 2052 6573 706f  t('SmartID Respo
-00002dc0: 6e73 655b 2720 2b20 2872 6573 2e65 7272  nse[' + (res.err
-00002dd0: 6f72 5f63 6f64 6520 7c7c 2027 756e 6b6e  or_code || 'unkn
-00002de0: 6f77 6e27 2920 2b20 275d 3a20 2720 2b20  own') + ']: ' + 
-00002df0: 7265 732e 6d65 7373 6167 6529 0a20 2020  res.message).   
-00002e00: 2020 2020 2020 2020 207d 2065 6c73 6520           } else 
-00002e10: 7b0a 2020 2020 2020 2020 2020 2020 2020  {.              
-00002e20: 2020 636f 6e73 6f6c 652e 6c6f 6728 2245    console.log("E
-00002e30: 7272 6f72 3a22 2c20 7265 7329 0a20 2020  rror:", res).   
-00002e40: 2020 2020 2020 2020 2020 2020 2061 6c65               ale
-00002e50: 7274 2827 536f 6d65 7468 696e 6720 7765  rt('Something we
-00002e60: 6e74 2077 726f 6e67 2c20 706c 6561 7365  nt wrong, please
-00002e70: 2074 7279 2061 6761 696e 2729 0a20 2020   try again').   
-00002e80: 2020 2020 2020 2020 207d 0a20 2020 2020           }.     
-00002e90: 2020 207d 0a0a 2020 2020 2020 2020 6675     }..        fu
-00002ea0: 6e63 7469 6f6e 2073 6967 6e53 6d61 7274  nction signSmart
-00002eb0: 4944 2865 2920 7b0a 2020 2020 2020 2020  ID(e) {.        
-00002ec0: 2020 2020 636f 6e73 6f6c 652e 6c6f 6728      console.log(
-00002ed0: 2253 6967 6e69 6e67 2077 6974 6820 536d  "Signing with Sm
-00002ee0: 6172 7420 4944 2229 0a20 2020 2020 2020  art ID").       
-00002ef0: 2020 2020 2065 2e70 7265 7665 6e74 4465       e.preventDe
-00002f00: 6661 756c 7428 290a 0a20 2020 2020 2020  fault()..       
-00002f10: 2020 2020 2076 6172 2074 696d 656f 7574       var timeout
-00002f20: 466f 7256 6572 6966 6963 6174 696f 6e43  ForVerificationC
-00002f30: 6f64 6520 3d20 3230 3030 2020 2f2f 2064  ode = 2000  // d
-00002f40: 656c 6179 2070 6f6c 6c69 6e67 2074 6f20  elay polling to 
-00002f50: 6c65 7420 7573 6572 2074 6f20 656e 7465  let user to ente
-00002f60: 7220 7665 7269 6669 6361 7469 6f6e 2063  r verification c
-00002f70: 6f64 650a 0a20 2020 2020 2020 2020 2020  ode..           
-00002f80: 2066 756e 6374 696f 6e20 6f6e 5374 6172   function onStar
-00002f90: 7453 6967 6e28 7265 7370 6f6e 7365 2920  tSign(response) 
-00002fa0: 7b0a 2020 2020 2020 2020 2020 2020 2020  {.              
-00002fb0: 2020 2f2f 2047 6f74 2061 2073 7563 6365    // Got a succe
-00002fc0: 7373 6675 6c20 7369 676e 2d73 7461 7274  ssful sign-start
-00002fd0: 2072 6571 7565 7374 2e2e 2e0a 2020 2020   request....    
-00002fe0: 2020 2020 2020 2020 2020 2020 636f 6e73              cons
-00002ff0: 6f6c 652e 6c6f 6728 2753 6d61 7274 4944  ole.log('SmartID
-00003000: 3a20 5369 676e 696e 6720 7665 7269 6669  : Signing verifi
-00003010: 6361 7469 6f6e 2063 6f64 6527 2c20 7265  cation code', re
-00003020: 7370 6f6e 7365 2e76 6572 6966 6963 6174  sponse.verificat
-00003030: 696f 6e5f 636f 6465 290a 0a20 2020 2020  ion_code)..     
-00003040: 2020 2020 2020 2020 2020 2024 2827 2376             $('#v
-00003050: 6572 6966 6963 6174 696f 6e2d 636f 6465  erification-code
-00003060: 2d6d 6f64 616c 2729 2e6d 6f64 616c 287b  -modal').modal({
-00003070: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00003080: 2020 2020 2062 6163 6b64 726f 703a 2027       backdrop: '
-00003090: 7374 6174 6963 272c 0a20 2020 2020 2020  static',.       
-000030a0: 2020 2020 2020 2020 2020 2020 206b 6579               key
-000030b0: 626f 6172 643a 2066 616c 7365 0a20 2020  board: false.   
-000030c0: 2020 2020 2020 2020 2020 2020 207d 290a               }).
-000030d0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000030e0: 2024 2827 2373 6d61 7274 6964 2d76 6572   $('#smartid-ver
-000030f0: 6966 6963 6174 696f 6e2d 636f 6465 2729  ification-code')
-00003100: 2e74 6578 7428 7265 7370 6f6e 7365 2e76  .text(response.v
-00003110: 6572 6966 6963 6174 696f 6e5f 636f 6465  erification_code
-00003120: 290a 0a20 2020 2020 2020 2020 2020 2020  )..             
-00003130: 2020 202f 2f20 2e2e 2e6e 6578 7420 7068     // ...next ph
-00003140: 6173 653a 2070 6f6c 6c20 666f 7220 7374  ase: poll for st
-00003150: 6174 7573 206f 6620 7369 676e 696e 670a  atus of signing.
-00003160: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003170: 7365 7454 696d 656f 7574 2866 756e 6374  setTimeout(funct
-00003180: 696f 6e20 2829 207b 0a20 2020 2020 2020  ion () {.       
-00003190: 2020 2020 2020 2020 2020 2020 206d 616e               man
-000031a0: 6167 6572 2e73 6d61 7274 6964 5374 6174  ager.smartidStat
-000031b0: 7573 287b 6373 7266 6d69 6464 6c65 7761  us({csrfmiddlewa
-000031c0: 7265 746f 6b65 6e3a 2063 7372 665f 746f  retoken: csrf_to
-000031d0: 6b65 6e7d 292e 7468 656e 280a 2020 2020  ken}).then(.    
+00000fc0: 2020 2020 2020 2020 2020 6172 6961 2d68            aria-h
+00000fd0: 6964 6465 6e3d 2274 7275 6522 3e26 7469  idden="true">&ti
+00000fe0: 6d65 733b 3c2f 7370 616e 3e0a 2020 2020  mes;</span>.    
+00000ff0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001000: 3c2f 6275 7474 6f6e 3e0a 2020 2020 2020  </button>.      
+00001010: 2020 2020 2020 2020 2020 2020 2020 3c68                <h
+00001020: 3420 636c 6173 733d 226d 6f64 616c 2d74  4 class="modal-t
+00001030: 6974 6c65 223e 4175 7468 656e 7469 6361  itle">Authentica
+00001040: 7469 6f6e 2077 6974 6820 4d6f 6269 6c65  tion with Mobile
+00001050: 4944 3c2f 6834 3e0a 2020 2020 2020 2020  ID</h4>.        
+00001060: 2020 2020 2020 2020 3c2f 6469 763e 0a0a          </div>..
+00001070: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001080: 3c64 6976 2063 6c61 7373 3d22 6d6f 6461  <div class="moda
+00001090: 6c2d 626f 6479 223e 0a20 2020 2020 2020  l-body">.       
+000010a0: 2020 2020 2020 2020 2020 2020 203c 6469               <di
+000010b0: 7620 636c 6173 733d 2266 6f72 6d2d 6772  v class="form-gr
+000010c0: 6f75 7022 3e0a 2020 2020 2020 2020 2020  oup">.          
+000010d0: 2020 2020 2020 2020 2020 2020 2020 3c6c                <l
+000010e0: 6162 656c 2066 6f72 3d22 7068 6f6e 654e  abel for="phoneN
+000010f0: 7249 6e70 7574 223e 4465 6d6f 2050 686f  rInput">Demo Pho
+00001100: 6e65 206e 723a 3c2f 6c61 6265 6c3e 0a20  ne nr:</label>. 
+00001110: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001120: 2020 2020 2020 203c 696e 7075 7420 7479         <input ty
+00001130: 7065 3d22 7465 7874 2220 6e61 6d65 3d22  pe="text" name="
+00001140: 7068 6f6e 655f 6e72 2220 6964 3d22 7068  phone_nr" id="ph
+00001150: 6f6e 654e 7249 6e70 7574 2220 636c 6173  oneNrInput" clas
+00001160: 733d 2266 6f72 6d2d 636f 6e74 726f 6c22  s="form-control"
+00001170: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00001180: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001190: 7661 6c75 653d 227b 7b20 7265 7175 6573  value="{{ reques
+000011a0: 742e 7365 7373 696f 6e2e 6464 6f63 5f74  t.session.ddoc_t
+000011b0: 6573 745f 7068 6f6e 655f 6e75 6d62 6572  est_phone_number
+000011c0: 207c 2064 6566 6175 6c74 3a27 2b33 3732   | default:'+372
+000011d0: 3030 3030 3037 3636 2720 7d7d 2220 2f3e  00000766' }}" />
+000011e0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000011f0: 2020 2020 203c 2f64 6976 3e0a 2020 2020       </div>.    
+00001200: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001210: 3c64 6976 2063 6c61 7373 3d22 666f 726d  <div class="form
+00001220: 2d67 726f 7570 223e 0a20 2020 2020 2020  -group">.       
+00001230: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001240: 203c 6c61 6265 6c20 666f 723d 2269 6443   <label for="idC
+00001250: 6f64 6549 6e70 7574 223e 4465 6d6f 2049  odeInput">Demo I
+00001260: 4420 636f 6465 3a3c 2f6c 6162 656c 3e0a  D code:</label>.
+00001270: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001280: 2020 2020 2020 2020 3c69 6e70 7574 2074          <input t
+00001290: 7970 653d 2274 6578 7422 206e 616d 653d  ype="text" name=
+000012a0: 2269 645f 636f 6465 2220 6964 3d22 6964  "id_code" id="id
+000012b0: 436f 6465 496e 7075 7422 2063 6c61 7373  CodeInput" class
+000012c0: 3d22 666f 726d 2d63 6f6e 7472 6f6c 220a  ="form-control".
+000012d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000012e0: 2020 2020 2020 2020 2020 2020 2020 2076                 v
+000012f0: 616c 7565 3d22 7b7b 2072 6571 7565 7374  alue="{{ request
+00001300: 2e73 6573 7369 6f6e 2e64 646f 635f 7465  .session.ddoc_te
+00001310: 7374 5f69 645f 636f 6465 207c 2064 6566  st_id_code | def
+00001320: 6175 6c74 3a27 3630 3030 3130 3139 3930  ault:'6000101990
+00001330: 3627 207d 7d22 202f 3e0a 2020 2020 2020  6' }}" />.      
+00001340: 2020 2020 2020 2020 2020 2020 2020 3c2f                </
+00001350: 6469 763e 0a20 2020 2020 2020 2020 2020  div>.           
+00001360: 2020 2020 203c 2f64 6976 3e0a 0a20 2020       </div>..   
+00001370: 2020 2020 2020 2020 2020 2020 203c 6469               <di
+00001380: 7620 636c 6173 733d 226d 6f64 616c 2d66  v class="modal-f
+00001390: 6f6f 7465 7222 3e0a 2020 2020 2020 2020  ooter">.        
+000013a0: 2020 2020 2020 2020 2020 2020 3c62 7574              <but
+000013b0: 746f 6e20 7479 7065 3d22 7375 626d 6974  ton type="submit
+000013c0: 2220 636c 6173 733d 2262 746e 2062 746e  " class="btn btn
+000013d0: 2d70 7269 6d61 7279 223e 4175 7468 656e  -primary">Authen
+000013e0: 7469 6361 7465 3c2f 6275 7474 6f6e 3e0a  ticate</button>.
+000013f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001400: 2020 2020 3c64 6976 2063 6c61 7373 3d22      <div class="
+00001410: 6c64 732d 6475 616c 2d72 696e 6722 3e3c  lds-dual-ring"><
+00001420: 2f64 6976 3e0a 2020 2020 2020 2020 2020  /div>.          
+00001430: 2020 2020 2020 3c2f 6469 763e 0a20 2020        </div>.   
+00001440: 2020 2020 2020 2020 203c 2f64 6976 3e0a           </div>.
+00001450: 2020 2020 2020 2020 3c2f 666f 726d 3e0a          </form>.
+00001460: 2020 2020 3c2f 6469 763e 0a3c 2f64 6976      </div>.</div
+00001470: 3e0a 0a3c 6469 7620 636c 6173 733d 226d  >..<div class="m
+00001480: 6f64 616c 2066 6164 6522 2069 643d 2263  odal fade" id="c
+00001490: 6861 6c6c 656e 6765 2d6d 6f64 616c 223e  hallenge-modal">
+000014a0: 0a20 2020 203c 6469 7620 636c 6173 733d  .    <div class=
+000014b0: 226d 6f64 616c 2d64 6961 6c6f 6722 3e0a  "modal-dialog">.
+000014c0: 2020 2020 2020 2020 3c64 6976 2063 6c61          <div cla
+000014d0: 7373 3d22 6d6f 6461 6c2d 636f 6e74 656e  ss="modal-conten
+000014e0: 7422 3e0a 2020 2020 2020 2020 2020 2020  t">.            
+000014f0: 3c64 6976 2063 6c61 7373 3d22 6d6f 6461  <div class="moda
+00001500: 6c2d 6865 6164 6572 223e 0a20 2020 2020  l-header">.     
+00001510: 2020 2020 2020 2020 2020 203c 6834 2063             <h4 c
+00001520: 6c61 7373 3d22 6d6f 6461 6c2d 7469 746c  lass="modal-titl
+00001530: 6522 3e4d 4944 2053 7465 7020 323c 2f68  e">MID Step 2</h
+00001540: 343e 0a20 2020 2020 2020 2020 2020 203c  4>.            <
+00001550: 2f64 6976 3e0a 0a20 2020 2020 2020 2020  /div>..         
+00001560: 2020 203c 6469 7620 636c 6173 733d 226d     <div class="m
+00001570: 6f64 616c 2d62 6f64 7922 3e0a 2020 2020  odal-body">.    
+00001580: 2020 2020 2020 2020 2020 2020 3c70 3e0a              <p>.
+00001590: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000015a0: 2020 2020 506c 6561 7365 2065 6e74 6572      Please enter
+000015b0: 2074 6865 2066 6f6c 6c6f 7769 6e67 2063   the following c
+000015c0: 6f64 6520 696e 746f 2079 6f75 7220 6d6f  ode into your mo
+000015d0: 6269 6c65 2074 6f20 7072 6f63 6565 6420  bile to proceed 
+000015e0: 7769 7468 0a20 2020 2020 2020 2020 2020  with.           
+000015f0: 2020 2020 2020 2020 2074 6865 2073 6967           the sig
+00001600: 6e69 6e67 2070 726f 6365 7373 3a20 3c62  ning process: <b
+00001610: 2069 643d 2263 6861 6c6c 656e 6765 2d63   id="challenge-c
+00001620: 6f64 6522 3e4b 4f4f 443c 2f62 3e0a 2020  ode">KOOD</b>.  
+00001630: 2020 2020 2020 2020 2020 2020 2020 3c2f                </
+00001640: 703e 0a20 2020 2020 2020 2020 2020 203c  p>.            <
+00001650: 2f64 6976 3e0a 2020 2020 2020 2020 3c2f  /div>.        </
+00001660: 6469 763e 0a20 2020 203c 2f64 6976 3e0a  div>.    </div>.
+00001670: 3c2f 6469 763e 0a0a 3c64 6976 2063 6c61  </div>..<div cla
+00001680: 7373 3d22 6d6f 6461 6c20 6661 6465 2220  ss="modal fade" 
+00001690: 6964 3d22 6964 2d6d 6f64 616c 223e 0a20  id="id-modal">. 
+000016a0: 2020 203c 6469 7620 636c 6173 733d 226d     <div class="m
+000016b0: 6f64 616c 2d64 6961 6c6f 6722 3e0a 2020  odal-dialog">.  
+000016c0: 2020 2020 2020 3c64 6976 2063 6c61 7373        <div class
+000016d0: 3d22 6d6f 6461 6c2d 636f 6e74 656e 7422  ="modal-content"
+000016e0: 3e0a 2020 2020 2020 2020 2020 2020 3c64  >.            <d
+000016f0: 6976 2063 6c61 7373 3d22 6d6f 6461 6c2d  iv class="modal-
+00001700: 6865 6164 6572 223e 0a20 2020 2020 2020  header">.       
+00001710: 2020 2020 2020 2020 203c 6834 2063 6c61           <h4 cla
+00001720: 7373 3d22 6d6f 6461 6c2d 7469 746c 6522  ss="modal-title"
+00001730: 3e41 7574 6865 6e74 6963 6174 696f 6e20  >Authentication 
+00001740: 7769 7468 2049 4420 4361 7264 3c2f 6834  with ID Card</h4
+00001750: 3e0a 2020 2020 2020 2020 2020 2020 3c2f  >.            </
+00001760: 6469 763e 0a0a 2020 2020 2020 2020 2020  div>..          
+00001770: 2020 3c64 6976 2063 6c61 7373 3d22 6d6f    <div class="mo
+00001780: 6461 6c2d 626f 6479 223e 0a20 2020 2020  dal-body">.     
+00001790: 2020 2020 2020 2020 2020 203c 703e 0a20             <p>. 
+000017a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000017b0: 2020 2050 6c65 6173 6520 666f 6c6c 6f77     Please follow
+000017c0: 2074 6865 2069 6e73 7472 7563 7469 6f6e   the instruction
+000017d0: 7320 746f 2063 6f6d 706c 6574 6520 7468  s to complete th
+000017e0: 6520 6175 7468 656e 7469 6361 7469 6f6e  e authentication
+000017f0: 2070 726f 6365 7373 2e0a 2020 2020 2020   process..      
+00001800: 2020 2020 2020 2020 2020 3c2f 703e 0a20            </p>. 
+00001810: 2020 2020 2020 2020 2020 2020 2020 207b                 {
+00001820: 2320 2a2a 2a20 5448 4953 2049 5320 4e45  # *** THIS IS NE
+00001830: 4345 5353 4152 5920 4f4e 4c59 2046 4f52  CESSARY ONLY FOR
+00001840: 2054 4553 5449 4e47 204c 4f43 414c 4c59   TESTING LOCALLY
+00001850: 2c20 4245 4341 5553 4520 4f46 2054 4845  , BECAUSE OF THE
+00001860: 2053 454c 462d 5349 474e 4544 2043 4552   SELF-SIGNED CER
+00001870: 5449 4649 4341 5445 2e20 2a2a 2a20 237d  TIFICATE. *** #}
+00001880: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00001890: 207b 2320 2a2a 2a20 4245 4749 4e20 2a2a   {# *** BEGIN **
+000018a0: 2a20 237d 0a20 2020 2020 2020 2020 2020  * #}.           
+000018b0: 2020 2020 203c 6872 3e0a 2020 2020 2020       <hr>.      
+000018c0: 2020 2020 2020 2020 2020 3c68 333e 5465            <h3>Te
+000018d0: 7374 696e 6720 6c6f 6361 6c6c 793f 3c2f  sting locally?</
+000018e0: 6833 3e0a 2020 2020 2020 2020 2020 2020  h3>.            
+000018f0: 2020 2020 3c70 3e0a 2020 2020 2020 2020      <p>.        
+00001900: 2020 2020 2020 2020 2020 2020 4966 2079              If y
+00001910: 6f75 2068 6176 656e 2774 2064 6f6e 6520  ou haven't done 
+00001920: 6974 2079 6574 2c20 6f70 656e 2074 6865  it yet, open the
+00001930: 206c 696e 6b20 3c62 723e 0a20 2020 2020   link <br>.     
+00001940: 2020 2020 2020 2020 2020 2020 2020 203c                 <
+00001950: 6120 6872 6566 3d22 2322 2069 643d 2261  a href="#" id="a
+00001960: 7574 682d 686f 7374 223e 3c2f 613e 203c  uth-host"></a> <
+00001970: 6272 3e0a 2020 2020 2020 2020 2020 2020  br>.            
+00001980: 2020 2020 2020 2020 696e 2061 206e 6577          in a new
+00001990: 2074 6162 2061 6e64 2063 6f6e 6669 726d   tab and confirm
+000019a0: 2073 6563 7572 6974 7920 6578 6365 7074   security except
+000019b0: 696f 6e2e 0a20 2020 2020 2020 2020 2020  ion..           
+000019c0: 2020 2020 203c 2f70 3e0a 2020 2020 2020       </p>.      
+000019d0: 2020 2020 2020 2020 2020 3c70 3e0a 2020            <p>.  
+000019e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000019f0: 2020 3c62 7574 746f 6e20 6f6e 636c 6963    <button onclic
+00001a00: 6b3d 2273 6563 7572 6974 7945 7863 6570  k="securityExcep
+00001a10: 7469 6f6e 203d 2074 7275 653b 2061 7574  tion = true; aut
+00001a20: 6857 6974 6849 4443 6172 6428 2922 3e4f  hWithIDCard()">O
+00001a30: 4b2c 2044 4f4e 453c 2f62 7574 746f 6e3e  K, DONE</button>
+00001a40: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00001a50: 203c 2f70 3e0a 2020 2020 2020 2020 2020   </p>.          
+00001a60: 2020 2020 2020 7b23 202a 2a2a 2045 4e44        {# *** END
+00001a70: 202a 2a2a 2020 237d 0a20 2020 2020 2020   ***  #}.       
+00001a80: 2020 2020 203c 2f64 6976 3e0a 2020 2020       </div>.    
+00001a90: 2020 2020 3c2f 6469 763e 0a20 2020 203c      </div>.    <
+00001aa0: 2f64 6976 3e0a 3c2f 6469 763e 0a0a 3c64  /div>.</div>..<d
+00001ab0: 6976 2069 643d 2269 6443 6172 6441 7574  iv id="idCardAut
+00001ac0: 6857 7261 7070 6572 2220 2f3e 0a0a 3c64  hWrapper" />..<d
+00001ad0: 6976 2063 6c61 7373 3d22 6d6f 6461 6c20  iv class="modal 
+00001ae0: 6661 6465 2220 6964 3d22 736d 6172 7469  fade" id="smarti
+00001af0: 642d 6d6f 6461 6c22 3e0a 2020 2020 3c64  d-modal">.    <d
+00001b00: 6976 2063 6c61 7373 3d22 6d6f 6461 6c2d  iv class="modal-
+00001b10: 6469 616c 6f67 223e 0a20 2020 2020 2020  dialog">.       
+00001b20: 203c 666f 726d 206e 616d 653d 2273 6d61   <form name="sma
+00001b30: 7274 4964 223e 0a20 2020 2020 2020 2020  rtId">.         
+00001b40: 2020 203c 6469 7620 636c 6173 733d 226d     <div class="m
+00001b50: 6f64 616c 2d63 6f6e 7465 6e74 223e 0a20  odal-content">. 
+00001b60: 2020 2020 2020 2020 2020 2020 2020 203c                 <
+00001b70: 6469 7620 636c 6173 733d 226d 6f64 616c  div class="modal
+00001b80: 2d68 6561 6465 7222 3e0a 2020 2020 2020  -header">.      
+00001b90: 2020 2020 2020 2020 2020 2020 2020 3c62                <b
+00001ba0: 7574 746f 6e20 7479 7065 3d22 6275 7474  utton type="butt
+00001bb0: 6f6e 2220 636c 6173 733d 2263 6c6f 7365  on" class="close
+00001bc0: 2220 6461 7461 2d64 6973 6d69 7373 3d22  " data-dismiss="
+00001bd0: 6d6f 6461 6c22 2061 7269 612d 6c61 6265  modal" aria-labe
+00001be0: 6c3d 2243 6c6f 7365 223e 3c73 7061 6e0a  l="Close"><span.
+00001bf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001c00: 2020 2020 2020 2020 2020 2020 6172 6961              aria
+00001c10: 2d68 6964 6465 6e3d 2274 7275 6522 3e26  -hidden="true">&
+00001c20: 7469 6d65 733b 3c2f 7370 616e 3e0a 2020  times;</span>.  
+00001c30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001c40: 2020 3c2f 6275 7474 6f6e 3e0a 2020 2020    </button>.    
+00001c50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001c60: 3c68 3420 636c 6173 733d 226d 6f64 616c  <h4 class="modal
+00001c70: 2d74 6974 6c65 223e 4175 7468 656e 7469  -title">Authenti
+00001c80: 6361 7469 6f6e 2077 6974 6820 536d 6172  cation with Smar
+00001c90: 7449 443c 2f68 343e 0a20 2020 2020 2020  tID</h4>.       
+00001ca0: 2020 2020 2020 2020 203c 2f64 6976 3e0a           </div>.
+00001cb0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00001cc0: 203c 6469 7620 636c 6173 733d 226d 6f64   <div class="mod
+00001cd0: 616c 2d62 6f64 7922 3e0a 2020 2020 2020  al-body">.      
+00001ce0: 2020 2020 2020 2020 2020 2020 2020 3c64                <d
+00001cf0: 6976 2063 6c61 7373 3d22 666f 726d 2d67  iv class="form-g
+00001d00: 726f 7570 223e 0a20 2020 2020 2020 2020  roup">.         
+00001d10: 2020 2020 2020 2020 2020 2020 2020 203c                 <
+00001d20: 6c61 6265 6c20 666f 723d 2269 6443 6f64  label for="idCod
+00001d30: 6549 6e70 7574 223e 596f 7572 2049 4420  eInput">Your ID 
+00001d40: 636f 6465 3a3c 2f6c 6162 656c 3e0a 2020  code:</label>.  
+00001d50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001d60: 2020 2020 2020 3c69 6e70 7574 2074 7970        <input typ
+00001d70: 653d 2274 6578 7422 206e 616d 653d 2269  e="text" name="i
+00001d80: 645f 636f 6465 2220 6964 3d22 6964 436f  d_code" id="idCo
+00001d90: 6465 496e 7075 7422 2063 6c61 7373 3d22  deInput" class="
+00001da0: 666f 726d 2d63 6f6e 7472 6f6c 220a 2020  form-control".  
+00001db0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001dc0: 2020 2020 2020 2020 2020 2020 2076 616c               val
+00001dd0: 7565 3d22 7b7b 2072 6571 7565 7374 2e73  ue="{{ request.s
+00001de0: 6573 7369 6f6e 2e73 6d61 7274 6964 5f74  ession.smartid_t
+00001df0: 6573 745f 6964 5f63 6f64 6520 7c20 6465  est_id_code | de
+00001e00: 6661 756c 743a 2733 3033 3033 3033 3939  fault:'303030399
+00001e10: 3134 2720 7d7d 2220 2f3e 0a20 2020 2020  14' }}" />.     
+00001e20: 2020 2020 2020 2020 2020 2020 2020 203c                 <
+00001e30: 2f64 6976 3e0a 2020 2020 2020 2020 2020  /div>.          
+00001e40: 2020 2020 2020 2020 2020 3c64 6976 2063            <div c
+00001e50: 6c61 7373 3d22 666f 726d 2d67 726f 7570  lass="form-group
+00001e60: 223e 0a20 2020 2020 2020 2020 2020 2020  ">.             
+00001e70: 2020 2020 2020 2020 2020 203c 6c61 6265             <labe
+00001e80: 6c20 666f 723d 2263 6f75 6e74 7279 496e  l for="countryIn
+00001e90: 7075 7422 3e43 6f75 6e74 7279 3a3c 2f6c  put">Country:</l
+00001ea0: 6162 656c 3e0a 2020 2020 2020 2020 2020  abel>.          
+00001eb0: 2020 2020 2020 2020 2020 2020 2020 3c73                <s
+00001ec0: 656c 6563 7420 6e61 6d65 3d22 636f 756e  elect name="coun
+00001ed0: 7472 7922 2069 643d 2263 6f75 6e74 7279  try" id="country
+00001ee0: 496e 7075 7422 2063 6c61 7373 3d22 666f  Input" class="fo
+00001ef0: 726d 2d63 6f6e 7472 6f6c 223e 0a20 2020  rm-control">.   
+00001f00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001f10: 2020 2020 2020 2020 203c 6f70 7469 6f6e           <option
+00001f20: 2076 616c 7565 3d22 223e 2d2d 204e 6f74   value="">-- Not
+00001f30: 2073 656c 6563 7465 6420 2d2d 2028 6465   selected -- (de
+00001f40: 6661 756c 7473 2074 6f20 4573 746f 6e69  faults to Estoni
+00001f50: 6129 3c2f 6f70 7469 6f6e 3e0a 2020 2020  a)</option>.    
+00001f60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001f70: 2020 2020 2020 2020 3c6f 7074 696f 6e20          <option 
+00001f80: 7661 6c75 653d 2245 4522 3e45 7374 6f6e  value="EE">Eston
+00001f90: 6961 3c2f 6f70 7469 6f6e 3e0a 2020 2020  ia</option>.    
+00001fa0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001fb0: 2020 2020 2020 2020 3c6f 7074 696f 6e20          <option 
+00001fc0: 7661 6c75 653d 224c 5622 3e4c 6174 7669  value="LV">Latvi
+00001fd0: 613c 2f6f 7074 696f 6e3e 0a20 2020 2020  a</option>.     
+00001fe0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001ff0: 2020 2020 2020 203c 6f70 7469 6f6e 2076         <option v
+00002000: 616c 7565 3d22 4c54 223e 4c69 7468 7561  alue="LT">Lithua
+00002010: 6e69 613c 2f6f 7074 696f 6e3e 0a20 2020  nia</option>.   
+00002020: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002030: 2020 2020 203c 2f73 656c 6563 743e 0a20       </select>. 
+00002040: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002050: 2020 203c 2f64 6976 3e0a 2020 2020 2020     </div>.      
+00002060: 2020 2020 2020 2020 2020 3c2f 6469 763e            </div>
+00002070: 0a0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00002080: 2020 3c64 6976 2063 6c61 7373 3d22 6d6f    <div class="mo
+00002090: 6461 6c2d 666f 6f74 6572 223e 0a20 2020  dal-footer">.   
+000020a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000020b0: 203c 6275 7474 6f6e 2074 7970 653d 2273   <button type="s
+000020c0: 7562 6d69 7422 2063 6c61 7373 3d22 6274  ubmit" class="bt
+000020d0: 6e20 6274 6e2d 7072 696d 6172 7922 3e41  n btn-primary">A
+000020e0: 7574 6865 6e74 6963 6174 653c 2f62 7574  uthenticate</but
+000020f0: 746f 6e3e 0a20 2020 2020 2020 2020 2020  ton>.           
+00002100: 2020 2020 2020 2020 203c 6469 7620 636c           <div cl
+00002110: 6173 733d 226c 6473 2d64 7561 6c2d 7269  ass="lds-dual-ri
+00002120: 6e67 223e 3c2f 6469 763e 0a20 2020 2020  ng"></div>.     
+00002130: 2020 2020 2020 2020 2020 203c 2f64 6976             </div
+00002140: 3e0a 2020 2020 2020 2020 2020 2020 3c2f  >.            </
+00002150: 6469 763e 0a20 2020 2020 2020 203c 2f66  div>.        </f
+00002160: 6f72 6d3e 0a20 2020 203c 2f64 6976 3e0a  orm>.    </div>.
+00002170: 3c2f 6469 763e 0a0a 3c64 6976 2063 6c61  </div>..<div cla
+00002180: 7373 3d22 6d6f 6461 6c20 6661 6465 2220  ss="modal fade" 
+00002190: 6964 3d22 7665 7269 6669 6361 7469 6f6e  id="verification
+000021a0: 2d63 6f64 652d 6d6f 6461 6c22 3e0a 2020  -code-modal">.  
+000021b0: 2020 3c64 6976 2063 6c61 7373 3d22 6d6f    <div class="mo
+000021c0: 6461 6c2d 6469 616c 6f67 223e 0a20 2020  dal-dialog">.   
+000021d0: 2020 2020 203c 6469 7620 636c 6173 733d       <div class=
+000021e0: 226d 6f64 616c 2d63 6f6e 7465 6e74 223e  "modal-content">
+000021f0: 0a20 2020 2020 2020 2020 2020 203c 6469  .            <di
+00002200: 7620 636c 6173 733d 226d 6f64 616c 2d68  v class="modal-h
+00002210: 6561 6465 7222 3e0a 2020 2020 2020 2020  eader">.        
+00002220: 2020 2020 2020 2020 3c68 3420 636c 6173          <h4 clas
+00002230: 733d 226d 6f64 616c 2d74 6974 6c65 2220  s="modal-title" 
+00002240: 6964 3d22 736d 6172 7469 642d 7374 6570  id="smartid-step
+00002250: 223e 5665 7269 6669 6361 7469 6f6e 2063  ">Verification c
+00002260: 6f64 653c 2f68 343e 0a20 2020 2020 2020  ode</h4>.       
+00002270: 2020 2020 203c 2f64 6976 3e0a 0a20 2020       </div>..   
+00002280: 2020 2020 2020 2020 203c 6469 7620 636c           <div cl
+00002290: 6173 733d 226d 6f64 616c 2d62 6f64 7922  ass="modal-body"
+000022a0: 3e0a 2020 2020 2020 2020 2020 2020 2020  >.              
+000022b0: 2020 3c70 3e0a 2020 2020 2020 2020 2020    <p>.          
+000022c0: 2020 2020 2020 2020 2020 4d61 6b65 2073            Make s
+000022d0: 7572 6520 796f 7520 6172 6520 7365 6569  ure you are seei
+000022e0: 6e67 2074 6869 7320 7665 7269 6669 6361  ng this verifica
+000022f0: 7469 6f6e 2063 6f64 6520 6f6e 2079 6f75  tion code on you
+00002300: 7220 6465 7669 6365 3a0a 2020 2020 2020  r device:.      
+00002310: 2020 2020 2020 2020 2020 2020 2020 3c62                <b
+00002320: 2069 643d 2273 6d61 7274 6964 2d76 6572   id="smartid-ver
+00002330: 6966 6963 6174 696f 6e2d 636f 6465 223e  ification-code">
+00002340: 4b4f 4f44 3c2f 623e 0a20 2020 2020 2020  KOOD</b>.       
+00002350: 2020 2020 2020 2020 203c 2f70 3e0a 2020           </p>.  
+00002360: 2020 2020 2020 2020 2020 3c2f 6469 763e            </div>
+00002370: 0a20 2020 2020 2020 203c 2f64 6976 3e0a  .        </div>.
+00002380: 2020 2020 3c2f 6469 763e 0a3c 2f64 6976      </div>.</div
+00002390: 3e0a 0a3c 6469 7620 636c 6173 733d 226d  >..<div class="m
+000023a0: 6f64 616c 2066 6164 6522 2069 643d 2273  odal fade" id="s
+000023b0: 7563 6365 7373 2d6d 6f64 616c 223e 0a20  uccess-modal">. 
+000023c0: 2020 203c 6469 7620 636c 6173 733d 226d     <div class="m
+000023d0: 6f64 616c 2d64 6961 6c6f 6722 3e0a 2020  odal-dialog">.  
+000023e0: 2020 2020 2020 3c64 6976 2063 6c61 7373        <div class
+000023f0: 3d22 6d6f 6461 6c2d 636f 6e74 656e 7422  ="modal-content"
+00002400: 3e0a 2020 2020 2020 2020 2020 2020 3c64  >.            <d
+00002410: 6976 2063 6c61 7373 3d22 6d6f 6461 6c2d  iv class="modal-
+00002420: 6865 6164 6572 223e 0a20 2020 2020 2020  header">.       
+00002430: 2020 2020 2020 2020 203c 6834 2063 6c61           <h4 cla
+00002440: 7373 3d22 6d6f 6461 6c2d 7469 746c 6522  ss="modal-title"
+00002450: 3e41 7574 6865 6e74 6963 6174 696f 6e20  >Authentication 
+00002460: 636f 6d70 6c65 7465 3c2f 6834 3e0a 2020  complete</h4>.  
+00002470: 2020 2020 2020 2020 2020 3c2f 6469 763e            </div>
+00002480: 0a0a 2020 2020 2020 2020 2020 2020 3c64  ..            <d
+00002490: 6976 2063 6c61 7373 3d22 6d6f 6461 6c2d  iv class="modal-
+000024a0: 626f 6479 223e 0a20 2020 2020 2020 2020  body">.         
+000024b0: 2020 2020 2020 203c 703e 0a20 2020 2020         <p>.     
+000024c0: 2020 2020 2020 2020 2020 2020 2020 2047                 G
+000024d0: 7265 6574 696e 6773 2c20 3c69 2069 643d  reetings, <i id=
+000024e0: 2267 6976 656e 2d6e 616d 6522 3e3c 2f69  "given-name"></i
+000024f0: 3e20 3c69 2069 643d 2273 7572 6e61 6d65  > <i id="surname
+00002500: 223e 3c2f 693e 210a 2020 2020 2020 2020  "></i>!.        
+00002510: 2020 2020 2020 2020 3c2f 703e 0a0a 2020          </p>..  
+00002520: 2020 2020 2020 2020 2020 2020 2020 3c61                <a
+00002530: 2068 7265 663d 2223 2220 6f6e 636c 6963   href="#" onclic
+00002540: 6b3d 2277 696e 646f 772e 6c6f 6361 7469  k="window.locati
+00002550: 6f6e 2e72 656c 6f61 6428 293b 2072 6574  on.reload(); ret
+00002560: 7572 6e20 6661 6c73 6522 3e4f 4b3c 2f61  urn false">OK</a
+00002570: 3e0a 2020 2020 2020 2020 2020 2020 3c2f  >.            </
+00002580: 6469 763e 0a20 2020 2020 2020 203c 2f64  div>.        </d
+00002590: 6976 3e0a 2020 2020 3c2f 6469 763e 0a3c  iv>.    </div>.<
+000025a0: 2f64 6976 3e0a 0a3c 7363 7269 7074 2073  /div>..<script s
+000025b0: 7263 3d22 2f2f 616a 6178 2e67 6f6f 676c  rc="//ajax.googl
+000025c0: 6561 7069 732e 636f 6d2f 616a 6178 2f6c  eapis.com/ajax/l
+000025d0: 6962 732f 6a71 7565 7279 2f31 2e31 312e  ibs/jquery/1.11.
+000025e0: 312f 6a71 7565 7279 2e6d 696e 2e6a 7322  1/jquery.min.js"
+000025f0: 3e3c 2f73 6372 6970 743e 0a3c 7363 7269  ></script>.<scri
+00002600: 7074 2073 7263 3d22 2f2f 6d61 7863 646e  pt src="//maxcdn
+00002610: 2e62 6f6f 7473 7472 6170 6364 6e2e 636f  .bootstrapcdn.co
+00002620: 6d2f 626f 6f74 7374 7261 702f 332e 332e  m/bootstrap/3.3.
+00002630: 342f 6a73 2f62 6f6f 7473 7472 6170 2e6d  4/js/bootstrap.m
+00002640: 696e 2e6a 7322 3e3c 2f73 6372 6970 743e  in.js"></script>
+00002650: 0a0a 3c73 6372 6970 7420 7479 7065 3d22  ..<script type="
+00002660: 7465 7874 2f6a 6176 6173 6372 6970 7422  text/javascript"
+00002670: 2073 7263 3d22 7b25 2073 7461 7469 6320   src="{% static 
+00002680: 2765 7374 6569 642d 6865 6c70 6572 2f77  'esteid-helper/w
+00002690: 6562 2d65 6964 2e6a 7327 2025 7d22 3e3c  eb-eid.js' %}"><
+000026a0: 2f73 6372 6970 743e 0a3c 7363 7269 7074  /script>.<script
+000026b0: 2074 7970 653d 2274 6578 742f 6a61 7661   type="text/java
+000026c0: 7363 7269 7074 2220 7372 633d 227b 2520  script" src="{% 
+000026d0: 7374 6174 6963 2027 6573 7465 6964 2d68  static 'esteid-h
+000026e0: 656c 7065 722f 4573 7465 6964 2e6d 6169  elper/Esteid.mai
+000026f0: 6e2e 7765 622e 6a73 2720 257d 223e 3c2f  n.web.js' %}"></
+00002700: 7363 7269 7074 3e0a 0a3c 7363 7269 7074  script>..<script
+00002710: 2074 7970 653d 2274 6578 742f 6a61 7661   type="text/java
+00002720: 7363 7269 7074 223e 0a20 2020 2076 6172  script">.    var
+00002730: 206d 616e 6167 6572 3b0a 0a20 2020 2066   manager;..    f
+00002740: 756e 6374 696f 6e20 7374 6172 7453 7069  unction startSpi
+00002750: 6e6e 6572 2866 6f72 6d29 207b 0a20 2020  nner(form) {.   
+00002760: 2020 2020 2024 2822 6275 7474 6f6e 222c       $("button",
+00002770: 2066 6f72 6d29 2e68 6964 6528 290a 2020   form).hide().  
+00002780: 2020 2020 2020 2428 222e 6c64 732d 6475        $(".lds-du
+00002790: 616c 2d72 696e 6722 2c20 666f 726d 292e  al-ring", form).
+000027a0: 6373 7328 2264 6973 706c 6179 222c 2022  css("display", "
+000027b0: 696e 6c69 6e65 2d62 6c6f 636b 2229 0a20  inline-block"). 
+000027c0: 2020 207d 0a0a 2020 2020 6675 6e63 7469     }..    functi
+000027d0: 6f6e 2073 746f 7053 7069 6e6e 6572 2866  on stopSpinner(f
+000027e0: 6f72 6d29 207b 0a20 2020 2020 2020 2024  orm) {.        $
+000027f0: 2822 6275 7474 6f6e 222c 2066 6f72 6d29  ("button", form)
+00002800: 2e73 686f 7728 290a 2020 2020 2020 2020  .show().        
+00002810: 2428 222e 6c64 732d 6475 616c 2d72 696e  $(".lds-dual-rin
+00002820: 6722 2c20 666f 726d 292e 6373 7328 2264  g", form).css("d
+00002830: 6973 706c 6179 222c 2022 6e6f 6e65 2229  isplay", "none")
+00002840: 0a20 2020 207d 0a0a 2020 2020 6675 6e63  .    }..    func
+00002850: 7469 6f6e 206f 6e45 7272 6f72 2872 6573  tion onError(res
+00002860: 2920 7b0a 2020 2020 2020 2020 2428 2723  ) {.        $('#
+00002870: 7665 7269 6669 6361 7469 6f6e 2d63 6f64  verification-cod
+00002880: 652d 6d6f 6461 6c27 292e 6d6f 6461 6c28  e-modal').modal(
+00002890: 2268 6964 6522 290a 2020 2020 2020 2020  "hide").        
+000028a0: 2428 2723 6368 616c 6c65 6e67 652d 6d6f  $('#challenge-mo
+000028b0: 6461 6c27 292e 6d6f 6461 6c28 2768 6964  dal').modal('hid
+000028c0: 6527 290a 0a20 2020 2020 2020 2063 6f6e  e')..        con
+000028d0: 736f 6c65 2e6c 6f67 2822 4572 726f 723a  sole.log("Error:
+000028e0: 222c 2072 6573 290a 2020 2020 2020 2020  ", res).        
+000028f0: 6966 2028 7265 7320 2626 2072 6573 2e6d  if (res && res.m
+00002900: 6573 7361 6765 2920 7b0a 2020 2020 2020  essage) {.      
+00002910: 2020 2020 2020 616c 6572 7428 6d61 6e61        alert(mana
+00002920: 6765 722e 6765 7445 7272 6f72 2872 6573  ger.getError(res
+00002930: 292e 6d65 7373 6167 6520 2b20 275c 6e5c  ).message + '\n\
+00002940: 6e27 202b 2072 6573 2e6d 6573 7361 6765  n' + res.message
+00002950: 293b 0a20 2020 2020 2020 207d 2065 6c73  );.        } els
+00002960: 6520 7b0a 2020 2020 2020 2020 2020 2020  e {.            
+00002970: 616c 6572 7428 2753 6f6d 6574 6869 6e67  alert('Something
+00002980: 2077 656e 7420 7772 6f6e 672c 2070 6c65   went wrong, ple
+00002990: 6173 6520 7472 7920 6167 6169 6e27 290a  ase try again').
+000029a0: 2020 2020 2020 2020 7d0a 2020 2020 7d0a          }.    }.
+000029b0: 0a20 2020 2066 756e 6374 696f 6e20 6f6e  .    function on
+000029c0: 4175 7468 436f 6d70 6c65 7465 2864 6174  AuthComplete(dat
+000029d0: 6129 207b 0a20 2020 2020 2020 2024 2827  a) {.        $('
+000029e0: 2373 7563 6365 7373 2d6d 6f64 616c 2729  #success-modal')
+000029f0: 2e6d 6f64 616c 287b 0a20 2020 2020 2020  .modal({.       
+00002a00: 2020 2020 2062 6163 6b64 726f 703a 2027       backdrop: '
+00002a10: 7374 6174 6963 272c 0a20 2020 2020 2020  static',.       
+00002a20: 2020 2020 206b 6579 626f 6172 643a 2066       keyboard: f
+00002a30: 616c 7365 0a20 2020 2020 2020 207d 290a  alse.        }).
+00002a40: 0a20 2020 2020 2020 2024 2827 2367 6976  .        $('#giv
+00002a50: 656e 2d6e 616d 6527 292e 7465 7874 2864  en-name').text(d
+00002a60: 6174 612e 6769 7665 6e5f 6e61 6d65 290a  ata.given_name).
+00002a70: 2020 2020 2020 2020 2428 2723 7375 726e          $('#surn
+00002a80: 616d 6527 292e 7465 7874 2864 6174 612e  ame').text(data.
+00002a90: 7375 726e 616d 6529 0a20 2020 207d 0a0a  surname).    }..
+00002aa0: 2020 2020 2428 6675 6e63 7469 6f6e 2028      $(function (
+00002ab0: 2920 7b0a 2020 2020 2020 2020 6d61 6e61  ) {.        mana
+00002ac0: 6765 7220 3d20 6e65 7720 4573 7465 6964  ger = new Esteid
+00002ad0: 2e49 6465 6e74 6966 6963 6174 696f 6e4d  .IdentificationM
+00002ae0: 616e 6167 6572 287b 0a20 2020 2020 2020  anager({.       
+00002af0: 2020 2020 206c 616e 6775 6167 653a 2045       language: E
+00002b00: 7374 6569 642e 4c61 6e67 7561 6765 732e  steid.Languages.
+00002b10: 4554 2c0a 0a20 2020 2020 2020 2020 2020  ET,..           
+00002b20: 2069 6455 726c 3a20 277b 2520 7572 6c20   idUrl: '{% url 
+00002b30: 2761 7574 682d 6964 6361 7264 2720 257d  'auth-idcard' %}
+00002b40: 272c 0a20 2020 2020 2020 2020 2020 206d  ',.            m
+00002b50: 6f62 696c 6549 6455 726c 3a20 277b 2520  obileIdUrl: '{% 
+00002b60: 7572 6c20 2761 7574 682d 6d6f 6269 6c65  url 'auth-mobile
+00002b70: 6964 2720 257d 272c 0a0a 2020 2020 2020  id' %}',..      
+00002b80: 2020 2020 2020 736d 6172 7449 6455 726c        smartIdUrl
+00002b90: 3a20 277b 2520 7572 6c20 2761 7574 682d  : '{% url 'auth-
+00002ba0: 736d 6172 7469 6427 2025 7d27 2c0a 0a20  smartid' %}',.. 
+00002bb0: 2020 2020 2020 2020 2020 2063 7372 6654             csrfT
+00002bc0: 6f6b 656e 3a20 277b 7b20 6373 7266 5f74  oken: '{{ csrf_t
+00002bd0: 6f6b 656e 207d 7d27 0a20 2020 2020 2020  oken }}'.       
+00002be0: 207d 290a 0a20 2020 2020 2020 2024 2827   })..        $('
+00002bf0: 2373 6967 6e2d 6d69 6427 292e 6f6e 2827  #sign-mid').on('
+00002c00: 636c 6963 6b27 2c20 6675 6e63 7469 6f6e  click', function
+00002c10: 2028 6529 207b 0a20 2020 2020 2020 2020   (e) {.         
+00002c20: 2020 2065 2e70 7265 7665 6e74 4465 6661     e.preventDefa
+00002c30: 756c 7428 290a 0a20 2020 2020 2020 2020  ult()..         
+00002c40: 2020 2024 2827 236d 6964 2d6d 6f64 616c     $('#mid-modal
+00002c50: 2729 2e6d 6f64 616c 2829 0a20 2020 2020  ').modal().     
+00002c60: 2020 207d 290a 0a20 2020 2020 2020 2076     })..        v
+00002c70: 6172 206d 6f62 696c 6549 6446 6f72 6d20  ar mobileIdForm 
+00002c80: 3d20 646f 6375 6d65 6e74 2e66 6f72 6d73  = document.forms
+00002c90: 2e6d 6f62 696c 6549 640a 2020 2020 2020  .mobileId.      
+00002ca0: 2020 6d6f 6269 6c65 4964 466f 726d 2e6f    mobileIdForm.o
+00002cb0: 6e73 7562 6d69 7420 3d20 6675 6e63 7469  nsubmit = functi
+00002cc0: 6f6e 2028 6529 207b 0a20 2020 2020 2020  on (e) {.       
+00002cd0: 2020 2020 2065 2e70 7265 7665 6e74 4465       e.preventDe
+00002ce0: 6661 756c 7428 290a 2020 2020 2020 2020  fault().        
+00002cf0: 2020 2020 7661 7220 7068 6f6e 654e 7220      var phoneNr 
+00002d00: 3d20 6d6f 6269 6c65 4964 466f 726d 2e70  = mobileIdForm.p
+00002d10: 686f 6e65 5f6e 722e 7661 6c75 650a 2020  hone_nr.value.  
+00002d20: 2020 2020 2020 2020 2020 7661 7220 6964            var id
+00002d30: 436f 6465 203d 206d 6f62 696c 6549 6446  Code = mobileIdF
+00002d40: 6f72 6d2e 6964 5f63 6f64 652e 7661 6c75  orm.id_code.valu
+00002d50: 650a 0a20 2020 2020 2020 2020 2020 2069  e..            i
+00002d60: 6620 2821 7068 6f6e 654e 7229 207b 0a20  f (!phoneNr) {. 
+00002d70: 2020 2020 2020 2020 2020 2020 2020 2061                 a
+00002d80: 6c65 7274 2827 506c 6561 7365 2065 6e74  lert('Please ent
+00002d90: 6572 2061 2070 686f 6e65 206e 756d 6265  er a phone numbe
+00002da0: 7227 290a 2020 2020 2020 2020 2020 2020  r').            
+00002db0: 2020 2020 7265 7475 726e 0a20 2020 2020      return.     
+00002dc0: 2020 2020 2020 207d 0a20 2020 2020 2020         }.       
+00002dd0: 2020 2020 2069 6620 2821 6964 436f 6465       if (!idCode
+00002de0: 2920 7b0a 2020 2020 2020 2020 2020 2020  ) {.            
+00002df0: 2020 2020 616c 6572 7428 2750 6c65 6173      alert('Pleas
+00002e00: 6520 656e 7465 7220 616e 2049 4420 636f  e enter an ID co
+00002e10: 6465 2729 0a20 2020 2020 2020 2020 2020  de').           
+00002e20: 2020 2020 2072 6574 7572 6e0a 2020 2020       return.    
+00002e30: 2020 2020 2020 2020 7d0a 0a20 2020 2020          }..     
+00002e40: 2020 2020 2020 2063 6f6e 736f 6c65 2e6c         console.l
+00002e50: 6f67 2827 4d49 443a 2073 6967 6e69 6e67  og('MID: signing
+00002e60: 2077 6974 6820 7068 6f6e 654e 7227 2c20   with phoneNr', 
+00002e70: 7068 6f6e 654e 722c 2027 616e 6420 6964  phoneNr, 'and id
+00002e80: 2063 6f64 6527 2c20 6964 436f 6465 290a   code', idCode).
+00002e90: 0a20 2020 2020 2020 2020 2020 2073 7461  .            sta
+00002ea0: 7274 5370 696e 6e65 7228 6d6f 6269 6c65  rtSpinner(mobile
+00002eb0: 4964 466f 726d 290a 0a20 2020 2020 2020  IdForm)..       
+00002ec0: 2020 2020 202f 2f20 4361 6c6c 2049 6465       // Call Ide
+00002ed0: 6e74 6966 6963 6174 696f 6e4d 616e 6167  ntificationManag
+00002ee0: 6572 2e73 6967 6e20 7768 6963 6820 6361  er.sign which ca
+00002ef0: 6c6c 7320 7468 6520 6261 636b 656e 6420  lls the backend 
+00002f00: 656e 6470 6f69 6e74 2074 6f20 7374 6172  endpoint to star
+00002f10: 7420 6d6f 6269 6c65 4964 2073 6967 6e69  t mobileId signi
+00002f20: 6e67 2070 726f 6365 7373 0a20 2020 2020  ng process.     
+00002f30: 2020 2020 2020 206d 616e 6167 6572 2e73         manager.s
+00002f40: 6967 6e57 6974 684d 6f62 696c 6549 6428  ignWithMobileId(
+00002f50: 7b0a 2020 2020 2020 2020 2020 2020 2020  {.              
+00002f60: 2020 7068 6f6e 654e 756d 6265 723a 2070    phoneNumber: p
+00002f70: 686f 6e65 4e72 2c0a 2020 2020 2020 2020  honeNr,.        
+00002f80: 2020 2020 2020 2020 6964 436f 6465 3a20          idCode: 
+00002f90: 6964 436f 6465 2c0a 2020 2020 2020 2020  idCode,.        
+00002fa0: 2020 2020 7d29 0a0a 2020 2020 2020 2020      })..        
+00002fb0: 2020 2020 2020 2020 2e74 6865 6e28 6675          .then(fu
+00002fc0: 6e63 7469 6f6e 2028 7265 7370 6f6e 7365  nction (response
+00002fd0: 2920 7b0a 2020 2020 2020 2020 2020 2020  ) {.            
+00002fe0: 2020 2020 2020 2020 636f 6e73 6f6c 652e          console.
+00002ff0: 6c6f 6728 274d 4944 3a20 676f 7420 7665  log('MID: got ve
+00003000: 7269 6669 6361 7469 6f6e 2063 6f64 6527  rification code'
+00003010: 2c20 7265 7370 6f6e 7365 2e76 6572 6966  , response.verif
+00003020: 6963 6174 696f 6e5f 636f 6465 290a 0a20  ication_code).. 
+00003030: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003040: 2020 202f 2f20 476f 7420 7265 7370 6f6e     // Got respon
+00003050: 7365 2c20 7368 6f77 2063 6861 6c6c 656e  se, show challen
+00003060: 6765 206d 6f64 616c 0a20 2020 2020 2020  ge modal.       
+00003070: 2020 2020 2020 2020 2020 2020 2024 2827               $('
+00003080: 2363 6861 6c6c 656e 6765 2d63 6f64 6527  #challenge-code'
+00003090: 292e 7465 7874 2872 6573 706f 6e73 652e  ).text(response.
+000030a0: 7665 7269 6669 6361 7469 6f6e 5f63 6f64  verification_cod
+000030b0: 6529 0a20 2020 2020 2020 2020 2020 2020  e).             
+000030c0: 2020 2020 2020 2024 2827 2363 6861 6c6c         $('#chall
+000030d0: 656e 6765 2d6d 6f64 616c 2729 2e6d 6f64  enge-modal').mod
+000030e0: 616c 287b 0a20 2020 2020 2020 2020 2020  al({.           
+000030f0: 2020 2020 2020 2020 2020 2020 2062 6163               bac
+00003100: 6b64 726f 703a 2027 7374 6174 6963 272c  kdrop: 'static',
+00003110: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00003120: 2020 2020 2020 2020 206b 6579 626f 6172           keyboar
+00003130: 643a 2066 616c 7365 0a20 2020 2020 2020  d: false.       
+00003140: 2020 2020 2020 2020 2020 2020 207d 290a               }).
+00003150: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00003160: 2020 2020 2024 2827 236d 6964 2d6d 6f64       $('#mid-mod
+00003170: 616c 2729 2e6d 6f64 616c 2827 6869 6465  al').modal('hide
+00003180: 2729 0a0a 2020 2020 2020 2020 2020 2020  ')..            
+00003190: 2020 2020 2020 2020 6d61 6e61 6765 722e          manager.
+000031a0: 6d69 6453 7461 7475 7328 292e 7468 656e  midStatus().then
+000031b0: 280a 2020 2020 2020 2020 2020 2020 2020  (.              
+000031c0: 2020 2020 2020 2020 2020 6675 6e63 7469            functi
+000031d0: 6f6e 2028 6461 7461 2920 7b0a 2020 2020  on (data) {.    
 000031e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000031f0: 2020 2020 6f6e 4669 6e69 7368 5369 676e      onFinishSign
-00003200: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-00003210: 2020 2020 2020 2020 2020 6f6e 4572 726f            onErro
-00003220: 720a 2020 2020 2020 2020 2020 2020 2020  r.              
-00003230: 2020 2020 2020 290a 2020 2020 2020 2020        ).        
-00003240: 2020 2020 2020 2020 7d2c 2074 696d 656f          }, timeo
-00003250: 7574 466f 7256 6572 6966 6963 6174 696f  utForVerificatio
-00003260: 6e43 6f64 6529 0a20 2020 2020 2020 2020  nCode).         
-00003270: 2020 207d 0a0a 2020 2020 2020 2020 2020     }..          
-00003280: 2020 6675 6e63 7469 6f6e 206f 6e46 696e    function onFin
-00003290: 6973 6853 6967 6e28 2920 7b0a 2020 2020  ishSign() {.    
-000032a0: 2020 2020 2020 2020 2020 2020 2428 2723              $('#
-000032b0: 736d 6172 7469 642d 6d6f 6461 6c27 292e  smartid-modal').
-000032c0: 6d6f 6461 6c28 2268 6964 6522 290a 2020  modal("hide").  
-000032d0: 2020 2020 2020 2020 2020 2020 2020 6f6e                on
-000032e0: 5369 676e 6564 2829 0a20 2020 2020 2020  Signed().       
-000032f0: 2020 2020 207d 0a0a 0a20 2020 2020 2020       }...       
-00003300: 2020 2020 2076 6172 2066 6f72 6d20 3d20       var form = 
-00003310: 646f 6375 6d65 6e74 2e66 6f72 6d73 2e73  document.forms.s
-00003320: 6d61 7274 4964 0a20 2020 2020 2020 2020  martId.         
-00003330: 2020 2076 6172 2069 6443 6f64 6520 3d20     var idCode = 
-00003340: 666f 726d 2e69 645f 636f 6465 2e76 616c  form.id_code.val
-00003350: 7565 0a0a 2020 2020 2020 2020 2020 2020  ue..            
-00003360: 6966 2028 2169 6443 6f64 6529 207b 0a20  if (!idCode) {. 
-00003370: 2020 2020 2020 2020 2020 2020 2020 2061                 a
-00003380: 6c65 7274 2827 506c 6561 7365 2065 6e74  lert('Please ent
-00003390: 6572 2061 6e20 4944 2063 6f64 6527 290a  er an ID code').
-000033a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000033b0: 7265 7475 726e 0a20 2020 2020 2020 2020  return.         
-000033c0: 2020 207d 0a0a 2020 2020 2020 2020 2020     }..          
-000033d0: 2020 636f 6e73 6f6c 652e 6c6f 6728 2753    console.log('S
-000033e0: 6d61 7274 4944 3a20 7369 676e 696e 6720  martID: signing 
-000033f0: 7769 7468 2069 6420 636f 6465 272c 2069  with id code', i
-00003400: 6443 6f64 6529 0a0a 2020 2020 2020 2020  dCode)..        
-00003410: 2020 2020 6d61 6e61 6765 722e 7369 676e      manager.sign
-00003420: 5769 7468 536d 6172 7449 6428 7b0a 2020  WithSmartId({.  
-00003430: 2020 2020 2020 2020 2020 2020 2020 6964                id
-00003440: 5f63 6f64 653a 2069 6443 6f64 652c 0a20  _code: idCode,. 
-00003450: 2020 2020 2020 2020 2020 2020 2020 2063                 c
-00003460: 7372 666d 6964 646c 6577 6172 6574 6f6b  srfmiddlewaretok
-00003470: 656e 3a20 6373 7266 5f74 6f6b 656e 0a20  en: csrf_token. 
-00003480: 2020 2020 2020 2020 2020 207d 292e 7468             }).th
-00003490: 656e 280a 2020 2020 2020 2020 2020 2020  en(.            
-000034a0: 2020 2020 2f2f 2053 7461 7274 2063 616c      // Start cal
-000034b0: 6c62 6163 6b20 6865 6c6c 0a20 2020 2020  lback hell.     
-000034c0: 2020 2020 2020 2020 2020 206f 6e53 7461             onSta
-000034d0: 7274 5369 676e 2c0a 2020 2020 2020 2020  rtSign,.        
-000034e0: 2020 2020 2020 2020 6f6e 4572 726f 720a          onError.
-000034f0: 2020 2020 2020 2020 2020 2020 290a 2020              ).  
-00003500: 2020 2020 2020 7d0a 0a20 2020 2020 2020        }..       
-00003510: 2024 2827 2373 6967 6e2d 6964 2729 2e6f   $('#sign-id').o
-00003520: 6e28 2763 6c69 636b 272c 2066 756e 6374  n('click', funct
-00003530: 696f 6e20 2865 2920 7b0a 2020 2020 2020  ion (e) {.      
-00003540: 2020 2020 2020 652e 7072 6576 656e 7444        e.preventD
-00003550: 6566 6175 6c74 2829 0a0a 2020 2020 2020  efault()..      
-00003560: 2020 2020 2020 2428 2723 6964 2d6d 6f64        $('#id-mod
-00003570: 616c 2729 2e6d 6f64 616c 287b 0a20 2020  al').modal({.   
-00003580: 2020 2020 2020 2020 2020 2020 2062 6163               bac
-00003590: 6b64 726f 703a 2027 7374 6174 6963 272c  kdrop: 'static',
-000035a0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000035b0: 206b 6579 626f 6172 643a 2066 616c 7365   keyboard: false
-000035c0: 0a20 2020 2020 2020 2020 2020 207d 290a  .            }).
-000035d0: 0a20 2020 2020 2020 2020 2020 206d 616e  .            man
-000035e0: 6167 6572 2e73 6967 6e57 6974 6849 6443  ager.signWithIdC
-000035f0: 6172 6428 7b63 7372 666d 6964 646c 6577  ard({csrfmiddlew
-00003600: 6172 6574 6f6b 656e 3a20 6373 7266 5f74  aretoken: csrf_t
-00003610: 6f6b 656e 7d29 2e74 6865 6e28 0a20 2020  oken}).then(.   
-00003620: 2020 2020 2020 2020 2020 2020 2066 756e               fun
-00003630: 6374 696f 6e20 2829 207b 0a20 2020 2020  ction () {.     
-00003640: 2020 2020 2020 2020 2020 2020 2020 2024                 $
-00003650: 2827 2369 642d 6d6f 6461 6c27 292e 6d6f  ('#id-modal').mo
-00003660: 6461 6c28 2768 6964 6527 290a 2020 2020  dal('hide').    
-00003670: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003680: 6f6e 5369 676e 6564 2829 0a20 2020 2020  onSigned().     
-00003690: 2020 2020 2020 2020 2020 207d 2c0a 0a20             },.. 
-000036a0: 2020 2020 2020 2020 2020 2020 2020 2066                 f
-000036b0: 756e 6374 696f 6e20 2872 6573 2920 7b0a  unction (res) {.
-000036c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000036d0: 2020 2020 6966 2028 7265 7320 696e 7374      if (res inst
-000036e0: 616e 6365 6f66 2045 7272 6f72 2920 7b0a  anceof Error) {.
-000036f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003700: 2020 2020 2020 2020 636f 6e73 6f6c 652e          console.
-00003710: 6c6f 6728 7265 732e 6d65 7373 6167 652c  log(res.message,
-00003720: 2072 6573 290a 2020 2020 2020 2020 2020   res).          
-00003730: 2020 2020 2020 2020 2020 2020 2020 7265                re
-00003740: 7320 3d20 6d61 6e61 6765 722e 6765 7445  s = manager.getE
-00003750: 7272 6f72 2872 6573 290a 0a20 2020 2020  rror(res)..     
-00003760: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003770: 2020 2061 6c65 7274 2872 6573 2e6d 6573     alert(res.mes
-00003780: 7361 6765 290a 0a20 2020 2020 2020 2020  sage)..         
-00003790: 2020 2020 2020 2020 2020 2020 2020 2063                 c
-000037a0: 6f6e 736f 6c65 2e65 7272 6f72 2827 5b45  onsole.error('[E
-000037b0: 7272 6f72 2063 6f64 653a 2027 202b 2072  rror code: ' + r
-000037c0: 6573 2e72 6574 7572 6e43 6f64 6520 2b20  es.returnCode + 
-000037d0: 273b 2045 7272 6f72 3a20 2720 2b20 7265  '; Error: ' + re
-000037e0: 732e 6d65 7373 6167 6520 2b20 275d 2729  s.message + ']')
-000037f0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00003800: 2020 2020 2020 2020 2024 2827 2369 642d           $('#id-
-00003810: 6d6f 6461 6c27 292e 6d6f 6461 6c28 2768  modal').modal('h
-00003820: 6964 6527 290a 2020 2020 2020 2020 2020  ide').          
-00003830: 2020 2020 2020 2020 2020 7d20 656c 7365            } else
-00003840: 207b 0a20 2020 2020 2020 2020 2020 2020   {.             
-00003850: 2020 2020 2020 2020 2020 2069 6620 2874             if (t
-00003860: 7970 656f 6620 7265 7320 3d3d 3d20 2773  ypeof res === 's
-00003870: 7472 696e 6727 207c 7c20 2872 6573 2026  tring' || (res &
-00003880: 2620 7265 732e 6572 726f 725f 636f 6465  & res.error_code
-00003890: 2929 207b 0a20 2020 2020 2020 2020 2020  )) {.           
-000038a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000038b0: 2076 6172 206d 7367 203d 2072 6573 2026   var msg = res &
-000038c0: 2620 7265 732e 6d65 7373 6167 6520 213d  & res.message !=
-000038d0: 3d20 756e 6465 6669 6e65 6420 3f20 7265  = undefined ? re
-000038e0: 732e 6d65 7373 6167 6520 3a20 7265 730a  s.message : res.
-000038f0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00003900: 2020 2020 2020 2020 2020 2020 2061 6c65               ale
-00003910: 7274 286d 7367 202b 2027 2c20 706c 6561  rt(msg + ', plea
-00003920: 7365 2074 7279 2061 6761 696e 2729 0a20  se try again'). 
-00003930: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003940: 2020 2020 2020 2020 2020 2024 2827 2369             $('#i
-00003950: 642d 6d6f 6461 6c27 292e 6d6f 6461 6c28  d-modal').modal(
-00003960: 2768 6964 6527 290a 2020 2020 2020 2020  'hide').        
-00003970: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003980: 7d20 656c 7365 207b 0a20 2020 2020 2020  } else {.       
-00003990: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000039a0: 2020 2020 2063 6f6e 736f 6c65 2e65 7272       console.err
-000039b0: 6f72 2872 6573 2026 2620 7265 732e 6d65  or(res && res.me
-000039c0: 7373 6167 6520 213d 3d20 756e 6465 6669  ssage !== undefi
-000039d0: 6e65 6420 3f20 7265 732e 6d65 7373 6167  ned ? res.messag
-000039e0: 6520 3a20 7265 7329 0a20 2020 2020 2020  e : res).       
-000039f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003a00: 2020 2020 2061 6c65 7274 2827 536f 6d65       alert('Some
-00003a10: 7468 696e 6720 7765 6e74 2077 726f 6e67  thing went wrong
-00003a20: 2c20 706c 6561 7365 2072 6566 7265 7368  , please refresh
-00003a30: 2074 6865 2070 6167 6520 616e 6420 7472   the page and tr
-00003a40: 7920 6167 6169 6e27 290a 2020 2020 2020  y again').      
-00003a50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003a60: 2020 7d0a 2020 2020 2020 2020 2020 2020    }.            
-00003a70: 2020 2020 2020 2020 7d0a 2020 2020 2020          }.      
-00003a80: 2020 2020 2020 2020 2020 7d0a 2020 2020            }.    
-00003a90: 2020 2020 2020 2020 290a 2020 2020 2020          ).      
-00003aa0: 2020 7d29 0a0a 2020 2020 2020 2020 2428    })..        $(
-00003ab0: 2723 6765 742d 646f 6375 6d65 6e74 2729  '#get-document')
-00003ac0: 2e6f 6e28 2763 6c69 636b 272c 2066 756e  .on('click', fun
-00003ad0: 6374 696f 6e20 2829 207b 0a20 2020 2020  ction () {.     
-00003ae0: 2020 2020 2020 2073 6574 5469 6d65 6f75         setTimeou
-00003af0: 7428 6675 6e63 7469 6f6e 2028 2920 7b0a  t(function () {.
-00003b00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003b10: 7769 6e64 6f77 2e6c 6f63 6174 696f 6e2e  window.location.
-00003b20: 7265 6c6f 6164 2829 0a20 2020 2020 2020  reload().       
-00003b30: 2020 2020 207d 2c20 3230 3030 290a 2020       }, 2000).  
-00003b40: 2020 2020 2020 7d29 0a0a 2020 2020 2020        })..      
-00003b50: 2020 646f 6375 6d65 6e74 2e66 6f72 6d73    document.forms
-00003b60: 2e73 6d61 7274 4964 2e6f 6e73 7562 6d69  .smartId.onsubmi
-00003b70: 7420 3d20 7369 676e 536d 6172 7449 440a  t = signSmartID.
-00003b80: 2020 2020 2020 2020 2428 2723 7369 676e          $('#sign
-00003b90: 2d73 6d61 7274 6964 2d62 7574 746f 6e27  -smartid-button'
-00003ba0: 292e 6f6e 2827 636c 6963 6b27 2c20 7369  ).on('click', si
-00003bb0: 676e 536d 6172 7449 4429 0a0a 2020 2020  gnSmartID)..    
-00003bc0: 2020 2020 646f 6375 6d65 6e74 2e66 6f72      document.for
-00003bd0: 6d73 2e6d 6f62 696c 6549 642e 6f6e 7375  ms.mobileId.onsu
-00003be0: 626d 6974 203d 2073 6967 6e4d 6f62 696c  bmit = signMobil
-00003bf0: 6549 440a 2020 2020 2020 2020 2428 2723  eID.        $('#
-00003c00: 7369 676e 4d6f 6269 6c65 2729 2e6f 6e28  signMobile').on(
-00003c10: 2763 6c69 636b 272c 2073 6967 6e4d 6f62  'click', signMob
-00003c20: 696c 6549 4429 0a0a 2020 2020 7d29 0a0a  ileID)..    })..
-00003c30: 3c2f 7363 7269 7074 3e0a 0a3c 2f62 6f64  </script>..</bod
-00003c40: 793e 0a3c 2f68 746d 6c3e 0a              y>.</html>.
+000031f0: 2020 2020 2020 2020 2428 2723 6368 616c          $('#chal
+00003200: 6c65 6e67 652d 6d6f 6461 6c27 292e 6d6f  lenge-modal').mo
+00003210: 6461 6c28 2768 6964 6527 290a 2020 2020  dal('hide').    
+00003220: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003230: 2020 2020 2020 2020 6f6e 4175 7468 436f          onAuthCo
+00003240: 6d70 6c65 7465 2864 6174 6129 0a20 2020  mplete(data).   
+00003250: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003260: 2020 2020 207d 2c0a 2020 2020 2020 2020       },.        
+00003270: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003280: 6f6e 4572 726f 720a 2020 2020 2020 2020  onError.        
+00003290: 2020 2020 2020 2020 2020 2020 292e 6669              ).fi
+000032a0: 6e61 6c6c 7928 0a20 2020 2020 2020 2020  nally(.         
+000032b0: 2020 2020 2020 2020 2020 2020 2020 2028                 (
+000032c0: 2920 3d3e 2073 746f 7053 7069 6e6e 6572  ) => stopSpinner
+000032d0: 286d 6f62 696c 6549 6446 6f72 6d29 0a20  (mobileIdForm). 
+000032e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000032f0: 2020 2029 0a20 2020 2020 2020 2020 2020     ).           
+00003300: 2020 2020 207d 2c20 6f6e 4572 726f 7229       }, onError)
+00003310: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00003320: 202e 6669 6e61 6c6c 7928 0a20 2020 2020   .finally(.     
+00003330: 2020 2020 2020 2020 2020 2020 2020 2028                 (
+00003340: 2920 3d3e 2073 746f 7053 7069 6e6e 6572  ) => stopSpinner
+00003350: 286d 6f62 696c 6549 6446 6f72 6d29 0a20  (mobileIdForm). 
+00003360: 2020 2020 2020 2020 2020 2020 2020 2029                 )
+00003370: 0a20 2020 2020 2020 207d 0a0a 2020 2020  .        }..    
+00003380: 2020 2020 2428 2723 7369 676e 2d73 6d61      $('#sign-sma
+00003390: 7274 6964 2729 2e6f 6e28 2763 6c69 636b  rtid').on('click
+000033a0: 272c 2066 756e 6374 696f 6e20 2865 2920  ', function (e) 
+000033b0: 7b0a 2020 2020 2020 2020 2020 2020 652e  {.            e.
+000033c0: 7072 6576 656e 7444 6566 6175 6c74 2829  preventDefault()
+000033d0: 0a0a 2020 2020 2020 2020 2020 2020 2428  ..            $(
+000033e0: 2723 736d 6172 7469 642d 6d6f 6461 6c27  '#smartid-modal'
+000033f0: 292e 6d6f 6461 6c28 290a 2020 2020 2020  ).modal().      
+00003400: 2020 7d29 0a0a 2020 2020 2020 2020 7661    })..        va
+00003410: 7220 736d 6172 7449 6446 6f72 6d20 3d20  r smartIdForm = 
+00003420: 646f 6375 6d65 6e74 2e66 6f72 6d73 2e73  document.forms.s
+00003430: 6d61 7274 4964 0a20 2020 2020 2020 2073  martId.        s
+00003440: 6d61 7274 4964 466f 726d 2e6f 6e73 7562  martIdForm.onsub
+00003450: 6d69 7420 3d20 6675 6e63 7469 6f6e 2028  mit = function (
+00003460: 6529 207b 0a20 2020 2020 2020 2020 2020  e) {.           
+00003470: 2063 6f6e 736f 6c65 2e6c 6f67 2822 5369   console.log("Si
+00003480: 676e 696e 6720 7769 7468 2053 6d61 7274  gning with Smart
+00003490: 2049 4422 290a 2020 2020 2020 2020 2020   ID").          
+000034a0: 2020 7661 7220 7469 6d65 6f75 7446 6f72    var timeoutFor
+000034b0: 5665 7269 6669 6361 7469 6f6e 436f 6465  VerificationCode
+000034c0: 203d 2033 3030 3020 202f 2f20 6465 6c61   = 3000  // dela
+000034d0: 7920 706f 6c6c 696e 6720 746f 206c 6574  y polling to let
+000034e0: 2075 7365 7220 746f 2065 6e74 6572 2076   user to enter v
+000034f0: 6572 6966 6963 6174 696f 6e20 636f 6465  erification code
+00003500: 0a0a 2020 2020 2020 2020 2020 2020 6675  ..            fu
+00003510: 6e63 7469 6f6e 206f 6e41 7574 6849 6e69  nction onAuthIni
+00003520: 7453 7563 6365 7373 2872 6573 706f 6e73  tSuccess(respons
+00003530: 6529 207b 0a20 2020 2020 2020 2020 2020  e) {.           
+00003540: 2020 2020 202f 2f20 476f 7420 6120 7375       // Got a su
+00003550: 6363 6573 7366 756c 2061 7574 682d 7374  ccessful auth-st
+00003560: 6172 7420 7265 7175 6573 742e 2e2e 0a20  art request.... 
+00003570: 2020 2020 2020 2020 2020 2020 2020 2063                 c
+00003580: 6f6e 736f 6c65 2e6c 6f67 2827 536d 6172  onsole.log('Smar
+00003590: 7449 443a 2061 7574 6820 7665 7269 6669  tID: auth verifi
+000035a0: 6361 7469 6f6e 2063 6f64 6527 2c20 7265  cation code', re
+000035b0: 7370 6f6e 7365 2e76 6572 6966 6963 6174  sponse.verificat
+000035c0: 696f 6e5f 636f 6465 290a 2020 2020 2020  ion_code).      
+000035d0: 2020 2020 2020 2020 2020 2428 2723 7665            $('#ve
+000035e0: 7269 6669 6361 7469 6f6e 2d63 6f64 652d  rification-code-
+000035f0: 6d6f 6461 6c27 292e 6d6f 6461 6c28 7b0a  modal').modal({.
+00003600: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003610: 2020 2020 6261 636b 6472 6f70 3a20 2773      backdrop: 's
+00003620: 7461 7469 6327 2c0a 2020 2020 2020 2020  tatic',.        
+00003630: 2020 2020 2020 2020 2020 2020 6b65 7962              keyb
+00003640: 6f61 7264 3a20 6661 6c73 650a 2020 2020  oard: false.    
+00003650: 2020 2020 2020 2020 2020 2020 7d29 0a0a              })..
+00003660: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003670: 2428 2723 736d 6172 7469 642d 7374 6570  $('#smartid-step
+00003680: 2729 2e74 6578 7428 2741 7574 6865 6e74  ').text('Authent
+00003690: 6963 6174 696f 6e27 290a 2020 2020 2020  ication').      
+000036a0: 2020 2020 2020 2020 2020 2428 2723 736d            $('#sm
+000036b0: 6172 7469 642d 7665 7269 6669 6361 7469  artid-verificati
+000036c0: 6f6e 2d63 6f64 6527 292e 7465 7874 2872  on-code').text(r
+000036d0: 6573 706f 6e73 652e 7665 7269 6669 6361  esponse.verifica
+000036e0: 7469 6f6e 5f63 6f64 6529 0a0a 2020 2020  tion_code)..    
+000036f0: 2020 2020 2020 2020 2020 2020 2f2f 202e              // .
+00003700: 2e2e 6e65 7874 2070 6861 7365 3a20 7374  ..next phase: st
+00003710: 6172 7420 7369 676e 696e 670a 2020 2020  art signing.    
+00003720: 2020 2020 2020 2020 2020 2020 2f2f 2077              // w
+00003730: 6520 646f 6e27 7420 7761 6e74 2074 6f20  e don't want to 
+00003740: 7374 6172 7420 706f 6c6c 696e 6720 696d  start polling im
+00003750: 6d65 6469 6174 656c 7920 6265 6361 7573  mediately becaus
+00003760: 6520 7573 6572 2077 696c 6c20 6e65 6564  e user will need
+00003770: 2074 6f20 656e 7465 7220 7665 7269 6669   to enter verifi
+00003780: 6361 7469 6f6e 2063 6f64 650a 2020 2020  cation code.    
+00003790: 2020 2020 2020 2020 2020 2020 7365 7454              setT
+000037a0: 696d 656f 7574 2866 756e 6374 696f 6e20  imeout(function 
+000037b0: 2829 207b 0a20 2020 2020 2020 2020 2020  () {.           
+000037c0: 2020 2020 2020 2020 206d 616e 6167 6572           manager
+000037d0: 2e73 6d61 7274 6964 5374 6174 7573 2829  .smartidStatus()
+000037e0: 2e74 6865 6e28 0a20 2020 2020 2020 2020  .then(.         
+000037f0: 2020 2020 2020 2020 2020 2020 2020 2028                 (
+00003800: 6461 7461 2920 3d3e 207b 0a20 2020 2020  data) => {.     
+00003810: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003820: 2020 2020 2020 2024 2827 2373 6d61 7274         $('#smart
+00003830: 6964 2d6d 6f64 616c 2729 2e6d 6f64 616c  id-modal').modal
+00003840: 2822 6869 6465 2229 0a20 2020 2020 2020  ("hide").       
+00003850: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003860: 2020 2020 206f 6e41 7574 6843 6f6d 706c       onAuthCompl
+00003870: 6574 6528 6461 7461 290a 2020 2020 2020  ete(data).      
+00003880: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003890: 2020 7d2c 0a20 2020 2020 2020 2020 2020    },.           
+000038a0: 2020 2020 2020 2020 2020 2020 206f 6e45               onE
+000038b0: 7272 6f72 0a20 2020 2020 2020 2020 2020  rror.           
+000038c0: 2020 2020 2020 2020 2029 2e66 696e 616c           ).final
+000038d0: 6c79 280a 2020 2020 2020 2020 2020 2020  ly(.            
+000038e0: 2020 2020 2020 2020 2020 2020 2829 203d              () =
+000038f0: 3e20 7374 6f70 5370 696e 6e65 7228 736d  > stopSpinner(sm
+00003900: 6172 7449 6446 6f72 6d29 0a20 2020 2020  artIdForm).     
+00003910: 2020 2020 2020 2020 2020 2020 2020 2029                 )
+00003920: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00003930: 207d 2c20 7469 6d65 6f75 7446 6f72 5665   }, timeoutForVe
+00003940: 7269 6669 6361 7469 6f6e 436f 6465 290a  rificationCode).
+00003950: 2020 2020 2020 2020 2020 2020 7d0a 0a20              }.. 
+00003960: 2020 2020 2020 2020 2020 2065 2e70 7265             e.pre
+00003970: 7665 6e74 4465 6661 756c 7428 290a 2020  ventDefault().  
+00003980: 2020 2020 2020 2020 2020 7661 7220 6964            var id
+00003990: 436f 6465 203d 2073 6d61 7274 4964 466f  Code = smartIdFo
+000039a0: 726d 2e69 645f 636f 6465 2e76 616c 7565  rm.id_code.value
+000039b0: 0a20 2020 2020 2020 2020 2020 2076 6172  .            var
+000039c0: 2063 6f75 6e74 7279 203d 2073 6d61 7274   country = smart
+000039d0: 4964 466f 726d 2e63 6f75 6e74 7279 2e76  IdForm.country.v
+000039e0: 616c 7565 0a0a 2020 2020 2020 2020 2020  alue..          
+000039f0: 2020 6966 2028 2169 6443 6f64 6529 207b    if (!idCode) {
+00003a00: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00003a10: 2061 6c65 7274 2827 506c 6561 7365 2065   alert('Please e
+00003a20: 6e74 6572 2061 6e20 4944 2063 6f64 6527  nter an ID code'
+00003a30: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
+00003a40: 2020 7265 7475 726e 0a20 2020 2020 2020    return.       
+00003a50: 2020 2020 207d 0a0a 2020 2020 2020 2020       }..        
+00003a60: 2020 2020 636f 6e73 6f6c 652e 6c6f 6728      console.log(
+00003a70: 2753 6d61 7274 4944 3a20 7369 676e 696e  'SmartID: signin
+00003a80: 6720 7769 7468 2069 6420 636f 6465 272c  g with id code',
+00003a90: 2069 6443 6f64 652c 2027 616e 6420 636f   idCode, 'and co
+00003aa0: 756e 7472 7927 2c20 636f 756e 7472 7929  untry', country)
+00003ab0: 0a0a 2020 2020 2020 2020 2020 2020 7374  ..            st
+00003ac0: 6172 7453 7069 6e6e 6572 2873 6d61 7274  artSpinner(smart
+00003ad0: 4964 466f 726d 290a 0a20 2020 2020 2020  IdForm)..       
+00003ae0: 2020 2020 206d 616e 6167 6572 2e73 6967       manager.sig
+00003af0: 6e57 6974 6853 6d61 7274 4964 287b 0a20  nWithSmartId({. 
+00003b00: 2020 2020 2020 2020 2020 2020 2020 2069                 i
+00003b10: 6443 6f64 652c 0a20 2020 2020 2020 2020  dCode,.         
+00003b20: 2020 2020 2020 2063 6f75 6e74 7279 2c0a         country,.
+00003b30: 2020 2020 2020 2020 2020 2020 7d29 2e74              }).t
+00003b40: 6865 6e28 0a20 2020 2020 2020 2020 2020  hen(.           
+00003b50: 2020 2020 206f 6e41 7574 6849 6e69 7453       onAuthInitS
+00003b60: 7563 6365 7373 2c0a 2020 2020 2020 2020  uccess,.        
+00003b70: 2020 2020 2020 2020 6f6e 4572 726f 720a          onError.
+00003b80: 2020 2020 2020 2020 2020 2020 292e 6669              ).fi
+00003b90: 6e61 6c6c 7928 0a20 2020 2020 2020 2020  nally(.         
+00003ba0: 2020 2020 2020 2028 2920 3d3e 2073 746f         () => sto
+00003bb0: 7053 7069 6e6e 6572 2873 6d61 7274 4964  pSpinner(smartId
+00003bc0: 466f 726d 290a 2020 2020 2020 2020 2020  Form).          
+00003bd0: 2020 290a 2020 2020 2020 2020 7d0a 0a20    ).        }.. 
+00003be0: 2020 2020 2020 2024 2827 2373 6967 6e2d         $('#sign-
+00003bf0: 6964 2729 2e6f 6e28 2763 6c69 636b 272c  id').on('click',
+00003c00: 2066 756e 6374 696f 6e20 2865 2920 7b0a   function (e) {.
+00003c10: 2020 2020 2020 2020 2020 2020 652e 7072              e.pr
+00003c20: 6576 656e 7444 6566 6175 6c74 2829 0a0a  eventDefault()..
+00003c30: 2020 2020 2020 2020 2020 2020 2f2f 2053              // S
+00003c40: 7461 7274 2061 7574 6865 6e74 6963 6174  tart authenticat
+00003c50: 696f 6e20 7072 6f63 6573 7320 7669 6120  ion process via 
+00003c60: 4964 656e 7469 6669 6361 7469 6f4d 616e  IdentificatioMan
+00003c70: 6167 6572 0a20 2020 2020 2020 2020 2020  ager.           
+00003c80: 206d 616e 6167 6572 2e61 7574 6865 6e74   manager.authent
+00003c90: 6963 6174 6557 6974 6849 6443 6172 6428  icateWithIdCard(
+00003ca0: 292e 7468 656e 2828 6461 7461 2920 3d3e  ).then((data) =>
+00003cb0: 207b 0a20 2020 2020 2020 2020 2020 2020   {.             
+00003cc0: 2020 206f 6e41 7574 6843 6f6d 706c 6574     onAuthComplet
+00003cd0: 6528 6461 7461 290a 2020 2020 2020 2020  e(data).        
+00003ce0: 2020 2020 7d2c 206f 6e45 7272 6f72 293b      }, onError);
+00003cf0: 0a20 2020 2020 2020 207d 290a 0a20 2020  .        })..   
+00003d00: 2020 2020 2024 2827 2367 6574 2d64 6f63       $('#get-doc
+00003d10: 756d 656e 7427 292e 6f6e 2827 636c 6963  ument').on('clic
+00003d20: 6b27 2c20 6675 6e63 7469 6f6e 2028 2920  k', function () 
+00003d30: 7b0a 2020 2020 2020 2020 2020 2020 7365  {.            se
+00003d40: 7454 696d 656f 7574 2866 756e 6374 696f  tTimeout(functio
+00003d50: 6e20 2829 207b 0a20 2020 2020 2020 2020  n () {.         
+00003d60: 2020 2020 2020 2077 696e 646f 772e 6c6f         window.lo
+00003d70: 6361 7469 6f6e 2e72 656c 6f61 6428 290a  cation.reload().
+00003d80: 2020 2020 2020 2020 2020 2020 7d2c 2032              }, 2
+00003d90: 3030 3029 0a20 2020 2020 2020 207d 290a  000).        }).
+00003da0: 2020 2020 7d29 0a0a 3c2f 7363 7269 7074      })..</script
+00003db0: 3e0a 0a3c 2f62 6f64 793e 0a3c 2f68 746d  >..</body>.</htm
+00003dc0: 6c3e 0a                                  l>.
```

### Comparing `django_esteid-3.4b1/esteid/types.py` & `django_esteid-4.0b1/esteid/types.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from datetime import datetime
-from typing import List, TYPE_CHECKING, Union
+from typing import get_origin, List, Literal, TYPE_CHECKING, Union
 
 import attr
 import pytz
 from oscrypto.asymmetric import load_certificate
 
 
 if TYPE_CHECKING:
@@ -273,15 +273,15 @@
                     # Optional[T] == Union[T, NoneType]
                     continue
 
                 if not raise_exception:
                     return False
                 raise ValueError(f"Missing required key {attr_name}") from e
 
-            if type(val) not in valid_types:
+            if type(val) not in valid_types and not (get_origin(attr_type) == Literal and val in valid_types):
                 if not raise_exception:
                     return False
                 raise ValueError(f"Wrong type {type(val)} for key {attr_name}")
 
         return True
 
     @classmethod
```

### Comparing `django_esteid-3.4b1/esteid/urls.py` & `django_esteid-4.0b1/esteid/urls.py`

 * *Files identical despite different names*

### Comparing `django_esteid-3.4b1/esteid/util.py` & `django_esteid-4.0b1/esteid/util.py`

 * *Files identical despite different names*

### Comparing `django_esteid-3.4b1/esteid/validators.py` & `django_esteid-4.0b1/esteid/validators.py`

 * *Files identical despite different names*

### Comparing `django_esteid-3.4b1/esteid/views.py` & `django_esteid-4.0b1/esteid/views.py`

 * *Files identical despite different names*

### Comparing `django_esteid-3.4b1/pyproject.toml` & `django_esteid-4.0b1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "django-esteid"
-version = "3.4.b1"
+version = "4.0.b1"
 description = "Django-esteid is a package that provides Esteid based authentication for your Django applications."
 readme = "README.md"
 license = "BSD"
 authors = [
     "Thorgate <info@thorgate.eu>",
     "Jürno Ader <jyrno@thorgate.eu>",
     "Yuri Shatrov <yuriy@thorgate.eu>",
@@ -81,15 +81,15 @@
 djangorestframework = ">=3.9"
 django-sslserver = "*"
 black = "==23.1.0"
 coverage = ">=4.5.4"
 coveralls = ">=1.8.2"
 flake8 = "*"
 isort = "==5.12.*"
-pylint = "==2.16.*"
+pylint = "==2.17.*"
 pyopenssl = ">=18.0.0"
 pytest-cov = ">=2.8.1"
 pytest-django = ">=3.5.1"
 pytest = ">=4.6.5"
 requests-mock = "*"
 tox = ">=1.7.0"
```

### Comparing `django_esteid-3.4b1/PKG-INFO` & `django_esteid-4.0b1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-esteid
-Version: 3.4b1
+Version: 4.0b1
 Summary: Django-esteid is a package that provides Esteid based authentication for your Django applications.
 Home-page: https://github.com/thorgate/django-esteid
 License: BSD
 Keywords: esteid,django,smartid,mobile-id,idcard,asice
 Author: Thorgate
 Author-email: info@thorgate.eu
 Maintainer: Jyrno Ader
```

