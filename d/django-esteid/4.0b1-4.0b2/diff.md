# Comparing `tmp/django_esteid-4.0b1.tar.gz` & `tmp/django_esteid-4.0b2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_esteid-4.0b1.tar", max compression
+gzip compressed data, was "django_esteid-4.0b2.tar", max compression
```

## Comparing `django_esteid-4.0b1.tar` & `django_esteid-4.0b2.tar`

### file list

```diff
@@ -1,80 +1,80 @@
--rw-r--r--   0        0        0      354 2021-11-09 11:26:25.693390 django_esteid-4.0b1/AUTHORS.md
--rw-r--r--   0        0        0     1477 2021-11-09 11:26:25.693390 django_esteid-4.0b1/LICENSE
--rw-r--r--   0        0        0     4901 2021-11-15 15:18:14.832376 django_esteid-4.0b1/README.md
--rw-r--r--   0        0        0       23 2023-06-11 09:39:31.897250 django_esteid-4.0b1/esteid/__init__.py
--rw-r--r--   0        0        0    16980 2023-06-02 09:57:48.736038 django_esteid-4.0b1/esteid/actions.py
--rw-r--r--   0        0        0     2420 2023-06-11 09:36:46.476132 django_esteid-4.0b1/esteid/authentication/README.md
--rw-r--r--   0        0        0      283 2021-11-09 11:26:25.696724 django_esteid-4.0b1/esteid/authentication/__init__.py
--rw-r--r--   0        0        0     6684 2023-06-11 09:11:00.032889 django_esteid-4.0b1/esteid/authentication/authenticator.py
--rw-r--r--   0        0        0      576 2021-11-09 11:26:25.696724 django_esteid-4.0b1/esteid/authentication/types.py
--rw-r--r--   0        0        0     4024 2023-06-11 09:20:36.868440 django_esteid-4.0b1/esteid/authentication/views.py
--rw-r--r--   0        0        0     6250 2021-11-15 12:09:45.735139 django_esteid-4.0b1/esteid/base_service.py
--rw-r--r--   0        0        0     1960 2021-11-09 11:26:25.696724 django_esteid-4.0b1/esteid/compat.py
--rw-r--r--   0        0        0     1912 2021-11-09 11:26:25.696724 django_esteid-4.0b1/esteid/constants.py
--rw-r--r--   0        0        0      410 2021-11-09 11:26:25.696724 django_esteid-4.0b1/esteid/context_processors.py
--rw-r--r--   0        0        0     5842 2021-11-09 11:26:25.696724 django_esteid-4.0b1/esteid/exceptions.py
--rw-r--r--   0        0        0       52 2021-11-09 11:26:25.696724 django_esteid-4.0b1/esteid/flowtest/README.md
--rw-r--r--   0        0        0        0 2021-11-09 11:26:25.696724 django_esteid-4.0b1/esteid/flowtest/__init__.py
--rw-r--r--   0        0        0     1155 2023-06-01 12:41:12.526823 django_esteid-4.0b1/esteid/flowtest/signer.py
--rw-r--r--   0        0        0     1387 2023-06-11 09:37:23.192308 django_esteid-4.0b1/esteid/flowtest/urls.py
--rw-r--r--   0        0        0     1742 2023-06-11 09:37:22.982311 django_esteid-4.0b1/esteid/flowtest/views.py
--rw-r--r--   0        0        0     1621 2021-11-09 11:26:25.696724 django_esteid-4.0b1/esteid/generic.py
--rw-r--r--   0        0        0     3295 2023-06-11 09:31:54.576660 django_esteid-4.0b1/esteid/idcard/README.md
--rw-r--r--   0        0        0      209 2023-06-11 09:33:43.105233 django_esteid-4.0b1/esteid/idcard/__init__.py
--rw-r--r--   0        0        0     4397 2023-06-11 09:37:23.375639 django_esteid-4.0b1/esteid/idcard/authenticator.py
--rw-r--r--   0        0        0     3712 2023-06-01 13:16:41.695317 django_esteid-4.0b1/esteid/idcard/signer.py
--rw-r--r--   0        0        0     2891 2023-06-11 09:37:23.368973 django_esteid-4.0b1/esteid/idcard/types.py
--rw-r--r--   0        0        0      380 2021-11-09 11:26:25.696724 django_esteid-4.0b1/esteid/locale/en/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0     2049 2021-11-09 11:26:25.696724 django_esteid-4.0b1/esteid/locale/en/LC_MESSAGES/django.po
--rw-r--r--   0        0        0     1927 2021-11-09 11:26:25.696724 django_esteid-4.0b1/esteid/locale/et/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0     2743 2021-11-09 11:26:25.696724 django_esteid-4.0b1/esteid/locale/et/LC_MESSAGES/django.po
--rw-r--r--   0        0        0      511 2021-11-09 11:26:25.696724 django_esteid-4.0b1/esteid/locale/lt/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0     2186 2021-11-09 11:26:25.696724 django_esteid-4.0b1/esteid/locale/lt/LC_MESSAGES/django.po
--rw-r--r--   0        0        0     2688 2021-11-09 11:26:25.696724 django_esteid-4.0b1/esteid/locale/ru/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0     3363 2021-11-09 11:26:25.696724 django_esteid-4.0b1/esteid/locale/ru/LC_MESSAGES/django.po
--rw-r--r--   0        0        0     4682 2023-06-01 12:41:35.186538 django_esteid-4.0b1/esteid/mixins.py
--rw-r--r--   0        0        0     1329 2021-11-09 11:26:25.696724 django_esteid-4.0b1/esteid/mobileid/README.md
--rw-r--r--   0        0        0      210 2021-11-09 11:26:25.696724 django_esteid-4.0b1/esteid/mobileid/__init__.py
--rw-r--r--   0        0        0     2440 2021-11-09 11:26:25.696724 django_esteid-4.0b1/esteid/mobileid/authenticator.py
--rw-r--r--   0        0        0    11547 2021-11-15 12:09:45.738473 django_esteid-4.0b1/esteid/mobileid/base.py
--rw-r--r--   0        0        0      518 2021-11-09 11:26:25.696724 django_esteid-4.0b1/esteid/mobileid/constants.py
--rw-r--r--   0        0        0      960 2023-03-07 10:56:00.181576 django_esteid-4.0b1/esteid/mobileid/i18n.py
--rw-r--r--   0        0        0     3133 2021-11-09 11:26:25.696724 django_esteid-4.0b1/esteid/mobileid/signer.py
--rw-r--r--   0        0        0     2083 2021-11-09 11:26:25.696724 django_esteid-4.0b1/esteid/mobileid/types.py
--rw-r--r--   0        0        0      960 2021-11-15 12:09:45.738473 django_esteid-4.0b1/esteid/mobileid/utils.py
--rw-r--r--   0        0        0     2568 2023-03-07 11:40:15.776172 django_esteid-4.0b1/esteid/ocsp.py
--rw-r--r--   0        0        0     1981 2021-11-15 12:09:45.738473 django_esteid-4.0b1/esteid/session.py
--rw-r--r--   0        0        0     4735 2023-06-11 09:32:18.669678 django_esteid-4.0b1/esteid/settings.py
--rw-r--r--   0        0        0    13575 2021-11-09 11:26:25.696724 django_esteid-4.0b1/esteid/signing/README.md
--rw-r--r--   0        0        0      294 2021-11-09 11:26:25.696724 django_esteid-4.0b1/esteid/signing/__init__.py
--rw-r--r--   0        0        0     9874 2021-11-09 11:26:25.696724 django_esteid-4.0b1/esteid/signing/signer.py
--rw-r--r--   0        0        0     2579 2021-11-09 11:26:25.696724 django_esteid-4.0b1/esteid/signing/types.py
--rw-r--r--   0        0        0     5865 2021-11-09 11:26:25.696724 django_esteid-4.0b1/esteid/signing/views.py
--rw-r--r--   0        0        0     3498 2021-11-09 11:26:25.696724 django_esteid-4.0b1/esteid/smartid/README.md
--rw-r--r--   0        0        0      204 2021-11-09 11:26:25.696724 django_esteid-4.0b1/esteid/smartid/__init__.py
--rw-r--r--   0        0        0      183 2023-03-07 10:56:00.188243 django_esteid-4.0b1/esteid/smartid/apps.py
--rw-r--r--   0        0        0     2253 2021-11-09 11:26:25.696724 django_esteid-4.0b1/esteid/smartid/authenticator.py
--rw-r--r--   0        0        0    14593 2021-11-09 11:26:25.696724 django_esteid-4.0b1/esteid/smartid/base.py
--rw-r--r--   0        0        0      729 2021-11-09 11:26:25.696724 django_esteid-4.0b1/esteid/smartid/constants.py
--rw-r--r--   0        0        0      882 2023-03-07 10:56:00.191576 django_esteid-4.0b1/esteid/smartid/i18n.py
--rw-r--r--   0        0        0     2986 2021-11-09 11:26:25.696724 django_esteid-4.0b1/esteid/smartid/signer.py
--rw-r--r--   0        0        0     1612 2021-11-09 11:26:25.700057 django_esteid-4.0b1/esteid/smartid/types.py
--rw-r--r--   0        0        0      727 2021-11-15 12:09:45.738473 django_esteid-4.0b1/esteid/smartid/utils.py
--rw-r--r--   0        0        0    21878 2023-06-10 11:18:47.152496 django_esteid-4.0b1/esteid/static/esteid-helper/Esteid.main.web.js
--rw-r--r--   0        0        0    10037 2023-06-10 11:18:47.449159 django_esteid-4.0b1/esteid/static/esteid-helper/Esteid.main.web.min.js
--rw-r--r--   0        0        0    18301 2023-06-01 11:37:15.406641 django_esteid-4.0b1/esteid/static/esteid-helper/web-eid.js
--rw-r--r--   0        0        0     1449 2021-11-09 11:26:25.700057 django_esteid-4.0b1/esteid/static/images/esteid/id-kaart-logo.gif
--rw-r--r--   0        0        0     1472 2021-11-09 11:26:25.700057 django_esteid-4.0b1/esteid/static/images/esteid/mid-logo.gif
--rw-r--r--   0        0        0     2458 2021-11-09 11:26:25.700057 django_esteid-4.0b1/esteid/static/images/esteid/smartID-logo-btn.png
--rw-r--r--   0        0        0     6894 2021-11-09 11:26:25.700057 django_esteid-4.0b1/esteid/static/images/esteid/smartID-logo.png
--rw-r--r--   0        0        0    15811 2023-06-10 11:21:23.187035 django_esteid-4.0b1/esteid/templates/esteid/auth-new.html
--rw-r--r--   0        0        0      320 2021-11-09 11:26:25.700057 django_esteid-4.0b1/esteid/templates/esteid/authenticate.html
--rw-r--r--   0        0        0    19018 2023-06-01 12:12:54.665282 django_esteid-4.0b1/esteid/templates/esteid/test-new.html
--rw-r--r--   0        0        0    15435 2023-06-01 13:16:01.879157 django_esteid-4.0b1/esteid/templates/esteid/test.html
--rw-r--r--   0        0        0    10342 2023-06-11 09:37:23.142309 django_esteid-4.0b1/esteid/types.py
--rw-r--r--   0        0        0     1995 2023-06-02 10:16:24.981279 django_esteid-4.0b1/esteid/urls.py
--rw-r--r--   0        0        0     3477 2023-03-07 11:38:29.734360 django_esteid-4.0b1/esteid/util.py
--rw-r--r--   0        0        0     2305 2023-03-07 12:11:59.783677 django_esteid-4.0b1/esteid/validators.py
--rw-r--r--   0        0        0     6326 2023-06-01 12:48:23.157992 django_esteid-4.0b1/esteid/views.py
--rw-r--r--   0        0        0     2632 2023-06-11 09:39:20.670734 django_esteid-4.0b1/pyproject.toml
--rw-r--r--   0        0        0     6326 1970-01-01 00:00:00.000000 django_esteid-4.0b1/PKG-INFO
+-rw-r--r--   0        0        0      354 2021-11-09 11:26:25.693390 django_esteid-4.0b2/AUTHORS.md
+-rw-r--r--   0        0        0     1477 2021-11-09 11:26:25.693390 django_esteid-4.0b2/LICENSE
+-rw-r--r--   0        0        0     4901 2021-11-15 15:18:14.832376 django_esteid-4.0b2/README.md
+-rw-r--r--   0        0        0       22 2023-06-11 11:03:27.329573 django_esteid-4.0b2/esteid/__init__.py
+-rw-r--r--   0        0        0    16980 2023-06-02 09:57:48.736038 django_esteid-4.0b2/esteid/actions.py
+-rw-r--r--   0        0        0     2420 2023-06-11 09:36:46.476132 django_esteid-4.0b2/esteid/authentication/README.md
+-rw-r--r--   0        0        0      283 2021-11-09 11:26:25.696724 django_esteid-4.0b2/esteid/authentication/__init__.py
+-rw-r--r--   0        0        0     6684 2023-06-11 09:11:00.032889 django_esteid-4.0b2/esteid/authentication/authenticator.py
+-rw-r--r--   0        0        0      576 2021-11-09 11:26:25.696724 django_esteid-4.0b2/esteid/authentication/types.py
+-rw-r--r--   0        0        0     4024 2023-06-11 09:20:36.868440 django_esteid-4.0b2/esteid/authentication/views.py
+-rw-r--r--   0        0        0     6250 2021-11-15 12:09:45.735139 django_esteid-4.0b2/esteid/base_service.py
+-rw-r--r--   0        0        0     1960 2021-11-09 11:26:25.696724 django_esteid-4.0b2/esteid/compat.py
+-rw-r--r--   0        0        0     1912 2021-11-09 11:26:25.696724 django_esteid-4.0b2/esteid/constants.py
+-rw-r--r--   0        0        0      410 2021-11-09 11:26:25.696724 django_esteid-4.0b2/esteid/context_processors.py
+-rw-r--r--   0        0        0     5842 2021-11-09 11:26:25.696724 django_esteid-4.0b2/esteid/exceptions.py
+-rw-r--r--   0        0        0       52 2021-11-09 11:26:25.696724 django_esteid-4.0b2/esteid/flowtest/README.md
+-rw-r--r--   0        0        0        0 2021-11-09 11:26:25.696724 django_esteid-4.0b2/esteid/flowtest/__init__.py
+-rw-r--r--   0        0        0     1155 2023-06-01 12:41:12.526823 django_esteid-4.0b2/esteid/flowtest/signer.py
+-rw-r--r--   0        0        0     1387 2023-06-11 09:37:23.192308 django_esteid-4.0b2/esteid/flowtest/urls.py
+-rw-r--r--   0        0        0     1742 2023-06-11 09:37:22.982311 django_esteid-4.0b2/esteid/flowtest/views.py
+-rw-r--r--   0        0        0     1621 2021-11-09 11:26:25.696724 django_esteid-4.0b2/esteid/generic.py
+-rw-r--r--   0        0        0     3295 2023-06-11 09:31:54.576660 django_esteid-4.0b2/esteid/idcard/README.md
+-rw-r--r--   0        0        0      209 2023-06-11 09:33:43.105233 django_esteid-4.0b2/esteid/idcard/__init__.py
+-rw-r--r--   0        0        0     4335 2023-06-11 09:56:34.133232 django_esteid-4.0b2/esteid/idcard/authenticator.py
+-rw-r--r--   0        0        0     3712 2023-06-01 13:16:41.695317 django_esteid-4.0b2/esteid/idcard/signer.py
+-rw-r--r--   0        0        0     2902 2023-06-11 09:57:49.932200 django_esteid-4.0b2/esteid/idcard/types.py
+-rw-r--r--   0        0        0      380 2021-11-09 11:26:25.696724 django_esteid-4.0b2/esteid/locale/en/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0     2049 2021-11-09 11:26:25.696724 django_esteid-4.0b2/esteid/locale/en/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     1927 2021-11-09 11:26:25.696724 django_esteid-4.0b2/esteid/locale/et/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0     2743 2021-11-09 11:26:25.696724 django_esteid-4.0b2/esteid/locale/et/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0      511 2021-11-09 11:26:25.696724 django_esteid-4.0b2/esteid/locale/lt/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0     2186 2021-11-09 11:26:25.696724 django_esteid-4.0b2/esteid/locale/lt/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     2688 2021-11-09 11:26:25.696724 django_esteid-4.0b2/esteid/locale/ru/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0     3363 2021-11-09 11:26:25.696724 django_esteid-4.0b2/esteid/locale/ru/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     4682 2023-06-01 12:41:35.186538 django_esteid-4.0b2/esteid/mixins.py
+-rw-r--r--   0        0        0     1329 2021-11-09 11:26:25.696724 django_esteid-4.0b2/esteid/mobileid/README.md
+-rw-r--r--   0        0        0      210 2021-11-09 11:26:25.696724 django_esteid-4.0b2/esteid/mobileid/__init__.py
+-rw-r--r--   0        0        0     2467 2023-06-11 09:56:28.863304 django_esteid-4.0b2/esteid/mobileid/authenticator.py
+-rw-r--r--   0        0        0    11547 2021-11-15 12:09:45.738473 django_esteid-4.0b2/esteid/mobileid/base.py
+-rw-r--r--   0        0        0      518 2021-11-09 11:26:25.696724 django_esteid-4.0b2/esteid/mobileid/constants.py
+-rw-r--r--   0        0        0      960 2023-03-07 10:56:00.181576 django_esteid-4.0b2/esteid/mobileid/i18n.py
+-rw-r--r--   0        0        0     3133 2021-11-09 11:26:25.696724 django_esteid-4.0b2/esteid/mobileid/signer.py
+-rw-r--r--   0        0        0     2083 2021-11-09 11:26:25.696724 django_esteid-4.0b2/esteid/mobileid/types.py
+-rw-r--r--   0        0        0      960 2021-11-15 12:09:45.738473 django_esteid-4.0b2/esteid/mobileid/utils.py
+-rw-r--r--   0        0        0     2568 2023-03-07 11:40:15.776172 django_esteid-4.0b2/esteid/ocsp.py
+-rw-r--r--   0        0        0     1981 2021-11-15 12:09:45.738473 django_esteid-4.0b2/esteid/session.py
+-rw-r--r--   0        0        0     4735 2023-06-11 09:32:18.669678 django_esteid-4.0b2/esteid/settings.py
+-rw-r--r--   0        0        0    13575 2021-11-09 11:26:25.696724 django_esteid-4.0b2/esteid/signing/README.md
+-rw-r--r--   0        0        0      294 2021-11-09 11:26:25.696724 django_esteid-4.0b2/esteid/signing/__init__.py
+-rw-r--r--   0        0        0     9874 2021-11-09 11:26:25.696724 django_esteid-4.0b2/esteid/signing/signer.py
+-rw-r--r--   0        0        0     2579 2021-11-09 11:26:25.696724 django_esteid-4.0b2/esteid/signing/types.py
+-rw-r--r--   0        0        0     5865 2021-11-09 11:26:25.696724 django_esteid-4.0b2/esteid/signing/views.py
+-rw-r--r--   0        0        0     3498 2021-11-09 11:26:25.696724 django_esteid-4.0b2/esteid/smartid/README.md
+-rw-r--r--   0        0        0      204 2021-11-09 11:26:25.696724 django_esteid-4.0b2/esteid/smartid/__init__.py
+-rw-r--r--   0        0        0      183 2023-03-07 10:56:00.188243 django_esteid-4.0b2/esteid/smartid/apps.py
+-rw-r--r--   0        0        0     2280 2023-06-11 09:56:44.663088 django_esteid-4.0b2/esteid/smartid/authenticator.py
+-rw-r--r--   0        0        0    14593 2021-11-09 11:26:25.696724 django_esteid-4.0b2/esteid/smartid/base.py
+-rw-r--r--   0        0        0      729 2021-11-09 11:26:25.696724 django_esteid-4.0b2/esteid/smartid/constants.py
+-rw-r--r--   0        0        0      882 2023-03-07 10:56:00.191576 django_esteid-4.0b2/esteid/smartid/i18n.py
+-rw-r--r--   0        0        0     2986 2021-11-09 11:26:25.696724 django_esteid-4.0b2/esteid/smartid/signer.py
+-rw-r--r--   0        0        0     1612 2021-11-09 11:26:25.700057 django_esteid-4.0b2/esteid/smartid/types.py
+-rw-r--r--   0        0        0      727 2021-11-15 12:09:45.738473 django_esteid-4.0b2/esteid/smartid/utils.py
+-rw-r--r--   0        0        0    21878 2023-06-10 11:18:47.152496 django_esteid-4.0b2/esteid/static/esteid-helper/Esteid.main.web.js
+-rw-r--r--   0        0        0    10037 2023-06-10 11:18:47.449159 django_esteid-4.0b2/esteid/static/esteid-helper/Esteid.main.web.min.js
+-rw-r--r--   0        0        0    18301 2023-06-01 11:37:15.406641 django_esteid-4.0b2/esteid/static/esteid-helper/web-eid.js
+-rw-r--r--   0        0        0     1449 2021-11-09 11:26:25.700057 django_esteid-4.0b2/esteid/static/images/esteid/id-kaart-logo.gif
+-rw-r--r--   0        0        0     1472 2021-11-09 11:26:25.700057 django_esteid-4.0b2/esteid/static/images/esteid/mid-logo.gif
+-rw-r--r--   0        0        0     2458 2021-11-09 11:26:25.700057 django_esteid-4.0b2/esteid/static/images/esteid/smartID-logo-btn.png
+-rw-r--r--   0        0        0     6894 2021-11-09 11:26:25.700057 django_esteid-4.0b2/esteid/static/images/esteid/smartID-logo.png
+-rw-r--r--   0        0        0    15811 2023-06-10 11:21:23.187035 django_esteid-4.0b2/esteid/templates/esteid/auth-new.html
+-rw-r--r--   0        0        0      320 2021-11-09 11:26:25.700057 django_esteid-4.0b2/esteid/templates/esteid/authenticate.html
+-rw-r--r--   0        0        0    19018 2023-06-01 12:12:54.665282 django_esteid-4.0b2/esteid/templates/esteid/test-new.html
+-rw-r--r--   0        0        0    15435 2023-06-01 13:16:01.879157 django_esteid-4.0b2/esteid/templates/esteid/test.html
+-rw-r--r--   0        0        0    10484 2023-06-11 09:59:16.147692 django_esteid-4.0b2/esteid/types.py
+-rw-r--r--   0        0        0     1995 2023-06-02 10:16:24.981279 django_esteid-4.0b2/esteid/urls.py
+-rw-r--r--   0        0        0     3477 2023-03-07 11:38:29.734360 django_esteid-4.0b2/esteid/util.py
+-rw-r--r--   0        0        0     2305 2023-03-07 12:11:59.783677 django_esteid-4.0b2/esteid/validators.py
+-rw-r--r--   0        0        0     6326 2023-06-01 12:48:23.157992 django_esteid-4.0b2/esteid/views.py
+-rw-r--r--   0        0        0     2631 2023-06-11 11:03:32.216174 django_esteid-4.0b2/pyproject.toml
+-rw-r--r--   0        0        0     6326 1970-01-01 00:00:00.000000 django_esteid-4.0b2/PKG-INFO
```

### Comparing `django_esteid-4.0b1/LICENSE` & `django_esteid-4.0b2/LICENSE`

 * *Files identical despite different names*

### Comparing `django_esteid-4.0b1/README.md` & `django_esteid-4.0b2/README.md`

 * *Files identical despite different names*

### Comparing `django_esteid-4.0b1/esteid/actions.py` & `django_esteid-4.0b2/esteid/actions.py`

 * *Files identical despite different names*

### Comparing `django_esteid-4.0b1/esteid/authentication/README.md` & `django_esteid-4.0b2/esteid/authentication/README.md`

 * *Files identical despite different names*

### Comparing `django_esteid-4.0b1/esteid/authentication/authenticator.py` & `django_esteid-4.0b2/esteid/authentication/authenticator.py`

 * *Files identical despite different names*

### Comparing `django_esteid-4.0b1/esteid/authentication/types.py` & `django_esteid-4.0b2/esteid/authentication/types.py`

 * *Files identical despite different names*

### Comparing `django_esteid-4.0b1/esteid/authentication/views.py` & `django_esteid-4.0b2/esteid/authentication/views.py`

 * *Files identical despite different names*

### Comparing `django_esteid-4.0b1/esteid/base_service.py` & `django_esteid-4.0b2/esteid/base_service.py`

 * *Files identical despite different names*

### Comparing `django_esteid-4.0b1/esteid/compat.py` & `django_esteid-4.0b2/esteid/compat.py`

 * *Files identical despite different names*

### Comparing `django_esteid-4.0b1/esteid/constants.py` & `django_esteid-4.0b2/esteid/constants.py`

 * *Files identical despite different names*

### Comparing `django_esteid-4.0b1/esteid/exceptions.py` & `django_esteid-4.0b2/esteid/exceptions.py`

 * *Files identical despite different names*

### Comparing `django_esteid-4.0b1/esteid/flowtest/signer.py` & `django_esteid-4.0b2/esteid/flowtest/signer.py`

 * *Files identical despite different names*

### Comparing `django_esteid-4.0b1/esteid/flowtest/urls.py` & `django_esteid-4.0b2/esteid/flowtest/urls.py`

 * *Files identical despite different names*

### Comparing `django_esteid-4.0b1/esteid/flowtest/views.py` & `django_esteid-4.0b2/esteid/flowtest/views.py`

 * *Files identical despite different names*

### Comparing `django_esteid-4.0b1/esteid/generic.py` & `django_esteid-4.0b2/esteid/generic.py`

 * *Files identical despite different names*

### Comparing `django_esteid-4.0b1/esteid/idcard/README.md` & `django_esteid-4.0b2/esteid/idcard/README.md`

 * *Files identical despite different names*

### Comparing `django_esteid-4.0b1/esteid/idcard/authenticator.py` & `django_esteid-4.0b2/esteid/idcard/authenticator.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,32 +1,28 @@
 import base64
-import binascii
 import logging
 import uuid
 
 from cryptography.hazmat.backends import default_backend
 from cryptography.x509 import load_der_x509_certificate, NameOID
 from esteid_certificates import get_certificate
-from oscrypto.asymmetric import load_certificate
+from oscrypto.asymmetric import Certificate as OsCryptoCertificate
 
 from pyasice.ocsp import OCSP
 
 from .. import settings
 from ..authentication import Authenticator
 from ..authentication.types import AuthenticationResult
 from ..constants import HASH_SHA256
 from ..exceptions import ActionInProgress, InvalidIdCode, InvalidParameter, InvalidParameters
 from ..types import CertificateHolderInfo
 from ..util import generate_hash, secure_random
 from .types import LibraryAuthenticateResponse
 
 
-# from .types import UserInput
-
-
 logger = logging.getLogger(__name__)
 
 
 class IdCardAuthenticator(Authenticator):
     certificate: bytes
 
     hash_type: str
@@ -57,15 +53,15 @@
 
         raise ActionInProgress(
             data={
                 "nonce": hash_value_b64,
             }
         )
 
-    def poll(self, initial_data: dict) -> AuthenticationResult:
+    def poll(self, initial_data: dict = None) -> AuthenticationResult:
         hash_value_b64 = self.session_data.hash_value_b64
 
         if not isinstance(initial_data, dict):
             raise InvalidParameters("Missing required parameters")
 
         auth_response = LibraryAuthenticateResponse(**initial_data)
 
@@ -75,16 +71,14 @@
             # Just to be explicit
             raise
         except ValueError as e:
             raise InvalidParameters("Invalid parameters") from e
 
         certificate = load_der_x509_certificate(auth_response.certificate_bytes, default_backend())
 
-        print("origin", self.origin)
-
         # This method:
         #
         # - validates the signature matches the certificate and the original nonce
         # - indirectly validates the certificate (by loading it with cryptography)
         auth_response.validate_signature(certificate, self.origin, hash_value_b64.encode())
 
         # Now we verify the certificate validity via OCSP. This ensures we comply with the following parts of the spec:
```

### Comparing `django_esteid-4.0b1/esteid/idcard/signer.py` & `django_esteid-4.0b2/esteid/idcard/signer.py`

 * *Files identical despite different names*

### Comparing `django_esteid-4.0b1/esteid/idcard/types.py` & `django_esteid-4.0b2/esteid/idcard/types.py`

 * *Files 0% similar despite different names*

```diff
@@ -72,19 +72,18 @@
     def certificate_bytes(self):
         return base64.b64decode(self.unverifiedCertificate)
 
     @property
     def signature_bytes(self):
         return base64.b64decode(self.signature)
 
-    """
-    Validates that the signature of the authentication token is valid
-    """
-
     def validate_signature(self, certificate, origin: str, challenge_nonce: bytes):
+        """
+        Validates that the signature of the authentication token is valid
+        """
         require_not_empty(challenge_nonce, "challenge_nonce")
 
         hash_algorithm = HASH_ALGORITHM_MAPPING[self.algorithm]
 
         origin_hash = generate_hash(hash_algorithm, origin.encode())
         nonce_hash = generate_hash(hash_algorithm, challenge_nonce)
         hash_value = origin_hash + nonce_hash
```

### Comparing `django_esteid-4.0b1/esteid/locale/en/LC_MESSAGES/django.po` & `django_esteid-4.0b2/esteid/locale/en/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django_esteid-4.0b1/esteid/locale/et/LC_MESSAGES/django.mo` & `django_esteid-4.0b2/esteid/locale/et/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django_esteid-4.0b1/esteid/locale/et/LC_MESSAGES/django.po` & `django_esteid-4.0b2/esteid/locale/et/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django_esteid-4.0b1/esteid/locale/lt/LC_MESSAGES/django.po` & `django_esteid-4.0b2/esteid/locale/lt/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django_esteid-4.0b1/esteid/locale/ru/LC_MESSAGES/django.mo` & `django_esteid-4.0b2/esteid/locale/ru/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django_esteid-4.0b1/esteid/locale/ru/LC_MESSAGES/django.po` & `django_esteid-4.0b2/esteid/locale/ru/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django_esteid-4.0b1/esteid/mixins.py` & `django_esteid-4.0b2/esteid/mixins.py`

 * *Files identical despite different names*

### Comparing `django_esteid-4.0b1/esteid/mobileid/README.md` & `django_esteid-4.0b2/esteid/mobileid/README.md`

 * *Files identical despite different names*

### Comparing `django_esteid-4.0b1/esteid/mobileid/authenticator.py` & `django_esteid-4.0b2/esteid/mobileid/authenticator.py`

 * *Files 3% similar despite different names*

```diff
@@ -50,15 +50,15 @@
 
         raise ActionInProgress(
             data={
                 "verification_code": auth_initial_result.verification_code,
             }
         )
 
-    def poll(self) -> AuthenticationResult:
+    def poll(self, initial_data: dict = None) -> AuthenticationResult:
         session_id = self.session_data.session_id
         hash_value_b64 = self.session_data.hash_value_b64
 
         service = TranslatedMobileIDService.get_instance()
 
         # raises ActionInProgress if not received a final result
         auth_result = service.status(session_id, hash_value=base64.b64decode(hash_value_b64))
```

### Comparing `django_esteid-4.0b1/esteid/mobileid/base.py` & `django_esteid-4.0b2/esteid/mobileid/base.py`

 * *Files identical despite different names*

### Comparing `django_esteid-4.0b1/esteid/mobileid/constants.py` & `django_esteid-4.0b2/esteid/mobileid/constants.py`

 * *Files identical despite different names*

### Comparing `django_esteid-4.0b1/esteid/mobileid/i18n.py` & `django_esteid-4.0b2/esteid/mobileid/i18n.py`

 * *Files identical despite different names*

### Comparing `django_esteid-4.0b1/esteid/mobileid/signer.py` & `django_esteid-4.0b2/esteid/mobileid/signer.py`

 * *Files identical despite different names*

### Comparing `django_esteid-4.0b1/esteid/mobileid/types.py` & `django_esteid-4.0b2/esteid/mobileid/types.py`

 * *Files identical despite different names*

### Comparing `django_esteid-4.0b1/esteid/mobileid/utils.py` & `django_esteid-4.0b2/esteid/mobileid/utils.py`

 * *Files identical despite different names*

### Comparing `django_esteid-4.0b1/esteid/ocsp.py` & `django_esteid-4.0b2/esteid/ocsp.py`

 * *Files identical despite different names*

### Comparing `django_esteid-4.0b1/esteid/session.py` & `django_esteid-4.0b2/esteid/session.py`

 * *Files identical despite different names*

### Comparing `django_esteid-4.0b1/esteid/settings.py` & `django_esteid-4.0b2/esteid/settings.py`

 * *Files identical despite different names*

### Comparing `django_esteid-4.0b1/esteid/signing/README.md` & `django_esteid-4.0b2/esteid/signing/README.md`

 * *Files identical despite different names*

### Comparing `django_esteid-4.0b1/esteid/signing/signer.py` & `django_esteid-4.0b2/esteid/signing/signer.py`

 * *Files identical despite different names*

### Comparing `django_esteid-4.0b1/esteid/signing/types.py` & `django_esteid-4.0b2/esteid/signing/types.py`

 * *Files identical despite different names*

### Comparing `django_esteid-4.0b1/esteid/signing/views.py` & `django_esteid-4.0b2/esteid/signing/views.py`

 * *Files identical despite different names*

### Comparing `django_esteid-4.0b1/esteid/smartid/README.md` & `django_esteid-4.0b2/esteid/smartid/README.md`

 * *Files identical despite different names*

### Comparing `django_esteid-4.0b1/esteid/smartid/authenticator.py` & `django_esteid-4.0b2/esteid/smartid/authenticator.py`

 * *Files 4% similar despite different names*

```diff
@@ -48,15 +48,15 @@
 
         raise ActionInProgress(
             data={
                 "verification_code": auth_initial_result.verification_code,
             }
         )
 
-    def poll(self) -> AuthenticationResult:
+    def poll(self, initial_data: dict = None) -> AuthenticationResult:
         session_id = self.session_data.session_id
         hash_value_b64 = self.session_data.hash_value_b64
 
         service = TranslatedSmartIDService.get_instance()
 
         # raises ActionInProgress if not received a final result
         auth_result = service.status(session_id, hash_value=base64.b64decode(hash_value_b64))
```

### Comparing `django_esteid-4.0b1/esteid/smartid/base.py` & `django_esteid-4.0b2/esteid/smartid/base.py`

 * *Files identical despite different names*

### Comparing `django_esteid-4.0b1/esteid/smartid/constants.py` & `django_esteid-4.0b2/esteid/smartid/constants.py`

 * *Files identical despite different names*

### Comparing `django_esteid-4.0b1/esteid/smartid/i18n.py` & `django_esteid-4.0b2/esteid/smartid/i18n.py`

 * *Files identical despite different names*

### Comparing `django_esteid-4.0b1/esteid/smartid/signer.py` & `django_esteid-4.0b2/esteid/smartid/signer.py`

 * *Files identical despite different names*

### Comparing `django_esteid-4.0b1/esteid/smartid/types.py` & `django_esteid-4.0b2/esteid/smartid/types.py`

 * *Files identical despite different names*

### Comparing `django_esteid-4.0b1/esteid/smartid/utils.py` & `django_esteid-4.0b2/esteid/smartid/utils.py`

 * *Files identical despite different names*

### Comparing `django_esteid-4.0b1/esteid/static/esteid-helper/Esteid.main.web.js` & `django_esteid-4.0b2/esteid/static/esteid-helper/Esteid.main.web.js`

 * *Files identical despite different names*

### Comparing `django_esteid-4.0b1/esteid/static/esteid-helper/Esteid.main.web.min.js` & `django_esteid-4.0b2/esteid/static/esteid-helper/Esteid.main.web.min.js`

 * *Files identical despite different names*

### Comparing `django_esteid-4.0b1/esteid/static/esteid-helper/web-eid.js` & `django_esteid-4.0b2/esteid/static/esteid-helper/web-eid.js`

 * *Files identical despite different names*

### Comparing `django_esteid-4.0b1/esteid/static/images/esteid/id-kaart-logo.gif` & `django_esteid-4.0b2/esteid/static/images/esteid/id-kaart-logo.gif`

 * *Files identical despite different names*

### Comparing `django_esteid-4.0b1/esteid/static/images/esteid/mid-logo.gif` & `django_esteid-4.0b2/esteid/static/images/esteid/mid-logo.gif`

 * *Files identical despite different names*

### Comparing `django_esteid-4.0b1/esteid/static/images/esteid/smartID-logo-btn.png` & `django_esteid-4.0b2/esteid/static/images/esteid/smartID-logo-btn.png`

 * *Files identical despite different names*

### Comparing `django_esteid-4.0b1/esteid/static/images/esteid/smartID-logo.png` & `django_esteid-4.0b2/esteid/static/images/esteid/smartID-logo.png`

 * *Files identical despite different names*

### Comparing `django_esteid-4.0b1/esteid/templates/esteid/auth-new.html` & `django_esteid-4.0b2/esteid/templates/esteid/auth-new.html`

 * *Files identical despite different names*

### Comparing `django_esteid-4.0b1/esteid/templates/esteid/test-new.html` & `django_esteid-4.0b2/esteid/templates/esteid/test-new.html`

 * *Files identical despite different names*

### Comparing `django_esteid-4.0b1/esteid/templates/esteid/test.html` & `django_esteid-4.0b2/esteid/templates/esteid/test.html`

 * *Files identical despite different names*

### Comparing `django_esteid-4.0b1/esteid/types.py` & `django_esteid-4.0b2/esteid/types.py`

 * *Files 1% similar despite different names*

```diff
@@ -273,15 +273,19 @@
                     # Optional[T] == Union[T, NoneType]
                     continue
 
                 if not raise_exception:
                     return False
                 raise ValueError(f"Missing required key {attr_name}") from e
 
-            if type(val) not in valid_types and not (get_origin(attr_type) == Literal and val in valid_types):
+            if type(val) not in valid_types:
+                if get_origin(attr_type) == Literal and val in valid_types:  # pylint: disable=comparison-with-callable
+                    # literal type needs special handling
+                    continue
+
                 if not raise_exception:
                     return False
                 raise ValueError(f"Wrong type {type(val)} for key {attr_name}")
 
         return True
 
     @classmethod
```

### Comparing `django_esteid-4.0b1/esteid/urls.py` & `django_esteid-4.0b2/esteid/urls.py`

 * *Files identical despite different names*

### Comparing `django_esteid-4.0b1/esteid/util.py` & `django_esteid-4.0b2/esteid/util.py`

 * *Files identical despite different names*

### Comparing `django_esteid-4.0b1/esteid/validators.py` & `django_esteid-4.0b2/esteid/validators.py`

 * *Files identical despite different names*

### Comparing `django_esteid-4.0b1/esteid/views.py` & `django_esteid-4.0b2/esteid/views.py`

 * *Files identical despite different names*

### Comparing `django_esteid-4.0b1/pyproject.toml` & `django_esteid-4.0b2/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "django-esteid"
-version = "4.0.b1"
+version = "4.0b2"
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
-pylint = "==2.17.*"
+pylint = "==2.16.*"
 pyopenssl = ">=18.0.0"
 pytest-cov = ">=2.8.1"
 pytest-django = ">=3.5.1"
 pytest = ">=4.6.5"
 requests-mock = "*"
 tox = ">=1.7.0"
```

### Comparing `django_esteid-4.0b1/PKG-INFO` & `django_esteid-4.0b2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-esteid
-Version: 4.0b1
+Version: 4.0b2
 Summary: Django-esteid is a package that provides Esteid based authentication for your Django applications.
 Home-page: https://github.com/thorgate/django-esteid
 License: BSD
 Keywords: esteid,django,smartid,mobile-id,idcard,asice
 Author: Thorgate
 Author-email: info@thorgate.eu
 Maintainer: Jyrno Ader
```

