# Comparing `tmp/wagtail-localize-1.5.tar.gz` & `tmp/wagtail-localize-1.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wagtail-localize-1.5.tar", last modified: Thu Feb 23 14:52:08 2023, max compression
+gzip compressed data, was "wagtail-localize-1.5.1.tar", last modified: Sun Jun 11 10:43:09 2023, max compression
```

## Comparing `wagtail-localize-1.5.tar` & `wagtail-localize-1.5.1.tar`

### file list

```diff
@@ -1,335 +1,335 @@
--rw-r--r--   0        0        0    11520 2023-02-23 14:17:49.011705 wagtail-localize-1.5/CHANGELOG.md
--rw-r--r--   0        0        0     1539 2022-07-01 10:57:34.575741 wagtail-localize-1.5/LICENSE
--rw-r--r--   0        0        0     3974 2023-02-15 19:30:42.625429 wagtail-localize-1.5/README.md
--rw-r--r--   0        0        0     2120 2023-02-15 19:30:42.625888 wagtail-localize-1.5/pyproject.toml
--rw-r--r--   0        0        0        4 2023-02-15 19:30:49.157059 wagtail-localize-1.5/runtime.txt
--rw-r--r--   0        0        0      384 2022-07-01 10:58:32.557727 wagtail-localize-1.5/setup.cfg
--rw-r--r--   0        0        0      154 2023-02-23 14:19:05.247523 wagtail-localize-1.5/wagtail_localize/__init__.py
--rw-r--r--   0        0        0      367 2022-07-01 10:57:34.552360 wagtail-localize-1.5/wagtail_localize/apps.py
--rw-r--r--   0        0        0      260 2023-02-15 19:30:42.626257 wagtail-localize-1.5/wagtail_localize/compat.py
--rw-r--r--   0        0        0     7001 2023-02-15 19:31:17.389647 wagtail-localize-1.5/wagtail_localize/components.py
--rw-r--r--   0        0        0    10830 2023-02-15 19:30:42.626478 wagtail-localize-1.5/wagtail_localize/fields.py
--rw-r--r--   0        0        0      355 2023-02-23 14:16:31.263856 wagtail-localize-1.5/wagtail_localize/locale/af/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0      452 2023-02-23 14:16:15.173853 wagtail-localize-1.5/wagtail_localize/locale/af/LC_MESSAGES/django.po
--rw-r--r--   0        0        0      332 2023-02-23 14:16:31.262091 wagtail-localize-1.5/wagtail_localize/locale/af/LC_MESSAGES/djangojs.mo
--rw-r--r--   0        0        0      380 2023-02-23 14:16:15.169157 wagtail-localize-1.5/wagtail_localize/locale/af/LC_MESSAGES/djangojs.po
--rw-r--r--   0        0        0      837 2023-02-23 14:16:31.190469 wagtail-localize-1.5/wagtail_localize/locale/ar/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0     1076 2023-02-23 14:16:15.109695 wagtail-localize-1.5/wagtail_localize/locale/ar/LC_MESSAGES/django.po
--rw-r--r--   0        0        0     1342 2023-02-23 14:16:31.187736 wagtail-localize-1.5/wagtail_localize/locale/ar/LC_MESSAGES/djangojs.mo
--rw-r--r--   0        0        0     1512 2023-02-23 14:16:15.104706 wagtail-localize-1.5/wagtail_localize/locale/ar/LC_MESSAGES/djangojs.po
--rw-r--r--   0        0        0      504 2023-02-23 14:16:31.284253 wagtail-localize-1.5/wagtail_localize/locale/az_AZ/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0      602 2023-02-23 14:16:14.857822 wagtail-localize-1.5/wagtail_localize/locale/az_AZ/LC_MESSAGES/django.po
--rw-r--r--   0        0        0      435 2023-02-23 14:16:31.283274 wagtail-localize-1.5/wagtail_localize/locale/az_AZ/LC_MESSAGES/djangojs.mo
--rw-r--r--   0        0        0      490 2023-02-23 14:16:14.851726 wagtail-localize-1.5/wagtail_localize/locale/az_AZ/LC_MESSAGES/djangojs.po
--rw-r--r--   0        0        0      794 2023-02-23 14:16:31.250377 wagtail-localize-1.5/wagtail_localize/locale/be/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0      883 2023-02-23 14:16:14.816557 wagtail-localize-1.5/wagtail_localize/locale/be/LC_MESSAGES/django.po
--rw-r--r--   0        0        0     1517 2023-02-23 14:16:31.248772 wagtail-localize-1.5/wagtail_localize/locale/be/LC_MESSAGES/djangojs.mo
--rw-r--r--   0        0        0     1546 2023-02-23 14:16:14.811362 wagtail-localize-1.5/wagtail_localize/locale/be/LC_MESSAGES/djangojs.po
--rw-r--r--   0        0        0      423 2023-02-23 14:16:31.253461 wagtail-localize-1.5/wagtail_localize/locale/bg/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0      568 2023-02-23 14:16:15.153850 wagtail-localize-1.5/wagtail_localize/locale/bg/LC_MESSAGES/django.po
--rw-r--r--   0        0        0      825 2023-02-23 14:16:31.251934 wagtail-localize-1.5/wagtail_localize/locale/bg/LC_MESSAGES/djangojs.mo
--rw-r--r--   0        0        0      901 2023-02-23 14:16:15.148547 wagtail-localize-1.5/wagtail_localize/locale/bg/LC_MESSAGES/djangojs.po
--rw-r--r--   0        0        0      541 2023-02-23 14:16:31.139558 wagtail-localize-1.5/wagtail_localize/locale/bn/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0      673 2023-02-23 14:16:15.164127 wagtail-localize-1.5/wagtail_localize/locale/bn/LC_MESSAGES/django.po
--rw-r--r--   0        0        0      723 2023-02-23 14:16:31.137592 wagtail-localize-1.5/wagtail_localize/locale/bn/LC_MESSAGES/djangojs.mo
--rw-r--r--   0        0        0      796 2023-02-23 14:16:15.159148 wagtail-localize-1.5/wagtail_localize/locale/bn/LC_MESSAGES/djangojs.po
--rw-r--r--   0        0        0     8727 2023-02-23 14:16:31.267472 wagtail-localize-1.5/wagtail_localize/locale/ca/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0     9246 2023-02-23 14:16:14.945443 wagtail-localize-1.5/wagtail_localize/locale/ca/LC_MESSAGES/django.po
--rw-r--r--   0        0        0     3330 2023-02-23 14:16:31.265678 wagtail-localize-1.5/wagtail_localize/locale/ca/LC_MESSAGES/djangojs.mo
--rw-r--r--   0        0        0     3257 2023-02-23 14:16:14.939802 wagtail-localize-1.5/wagtail_localize/locale/ca/LC_MESSAGES/djangojs.po
--rw-r--r--   0        0        0     5617 2023-02-23 14:16:31.192588 wagtail-localize-1.5/wagtail_localize/locale/cs/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0     5962 2023-02-23 14:16:14.956700 wagtail-localize-1.5/wagtail_localize/locale/cs/LC_MESSAGES/django.po
--rw-r--r--   0        0        0     2851 2023-02-23 14:16:31.191239 wagtail-localize-1.5/wagtail_localize/locale/cs/LC_MESSAGES/djangojs.mo
--rw-r--r--   0        0        0     2810 2023-02-23 14:16:14.950812 wagtail-localize-1.5/wagtail_localize/locale/cs/LC_MESSAGES/djangojs.po
--rw-r--r--   0        0        0     8527 2023-02-23 14:16:31.230188 wagtail-localize-1.5/wagtail_localize/locale/cy/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0     9068 2023-02-23 14:16:15.306817 wagtail-localize-1.5/wagtail_localize/locale/cy/LC_MESSAGES/django.po
--rw-r--r--   0        0        0     3265 2023-02-23 14:16:31.228886 wagtail-localize-1.5/wagtail_localize/locale/cy/LC_MESSAGES/djangojs.mo
--rw-r--r--   0        0        0     3167 2023-02-23 14:16:15.301245 wagtail-localize-1.5/wagtail_localize/locale/cy/LC_MESSAGES/djangojs.po
--rw-r--r--   0        0        0      498 2023-02-23 14:16:31.143000 wagtail-localize-1.5/wagtail_localize/locale/da/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0      574 2023-02-23 14:16:14.826574 wagtail-localize-1.5/wagtail_localize/locale/da/LC_MESSAGES/django.po
--rw-r--r--   0        0        0      876 2023-02-23 14:16:31.140963 wagtail-localize-1.5/wagtail_localize/locale/da/LC_MESSAGES/djangojs.mo
--rw-r--r--   0        0        0     1011 2023-02-23 14:16:14.821503 wagtail-localize-1.5/wagtail_localize/locale/da/LC_MESSAGES/djangojs.po
--rw-r--r--   0        0        0     8880 2023-02-23 14:16:31.274260 wagtail-localize-1.5/wagtail_localize/locale/de/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0     9632 2023-02-23 14:16:15.205779 wagtail-localize-1.5/wagtail_localize/locale/de/LC_MESSAGES/django.po
--rw-r--r--   0        0        0     3383 2023-02-23 14:16:31.272282 wagtail-localize-1.5/wagtail_localize/locale/de/LC_MESSAGES/djangojs.mo
--rw-r--r--   0        0        0     3404 2023-02-23 14:16:15.199951 wagtail-localize-1.5/wagtail_localize/locale/de/LC_MESSAGES/djangojs.po
--rw-r--r--   0        0        0      744 2023-02-23 14:16:31.185696 wagtail-localize-1.5/wagtail_localize/locale/el/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0     1022 2023-02-23 14:16:14.905561 wagtail-localize-1.5/wagtail_localize/locale/el/LC_MESSAGES/django.po
--rw-r--r--   0        0        0     1565 2023-02-23 14:16:31.183809 wagtail-localize-1.5/wagtail_localize/locale/el/LC_MESSAGES/djangojs.mo
--rw-r--r--   0        0        0     1701 2023-02-23 14:16:14.899134 wagtail-localize-1.5/wagtail_localize/locale/el/LC_MESSAGES/djangojs.po
--rw-r--r--   0        0        0      210 2023-02-23 14:16:31.203338 wagtail-localize-1.5/wagtail_localize/locale/en/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0     9124 2023-02-23 14:15:49.513297 wagtail-localize-1.5/wagtail_localize/locale/en/LC_MESSAGES/django.po
--rw-r--r--   0        0        0       98 2023-02-23 14:16:31.201470 wagtail-localize-1.5/wagtail_localize/locale/en/LC_MESSAGES/djangojs.mo
--rw-r--r--   0        0        0     6384 2023-02-23 14:15:48.812511 wagtail-localize-1.5/wagtail_localize/locale/en/LC_MESSAGES/djangojs.po
--rw-r--r--   0        0        0     8831 2023-02-23 14:16:31.305328 wagtail-localize-1.5/wagtail_localize/locale/es/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0     9558 2023-02-23 14:16:15.263656 wagtail-localize-1.5/wagtail_localize/locale/es/LC_MESSAGES/django.po
--rw-r--r--   0        0        0     3348 2023-02-23 14:16:31.303153 wagtail-localize-1.5/wagtail_localize/locale/es/LC_MESSAGES/djangojs.mo
--rw-r--r--   0        0        0     3295 2023-02-23 14:16:15.255437 wagtail-localize-1.5/wagtail_localize/locale/es/LC_MESSAGES/djangojs.po
--rw-r--r--   0        0        0      659 2023-02-23 14:16:31.220198 wagtail-localize-1.5/wagtail_localize/locale/et/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0      764 2023-02-23 14:16:15.273966 wagtail-localize-1.5/wagtail_localize/locale/et/LC_MESSAGES/django.po
--rw-r--r--   0        0        0     1214 2023-02-23 14:16:31.220144 wagtail-localize-1.5/wagtail_localize/locale/et/LC_MESSAGES/djangojs.mo
--rw-r--r--   0        0        0     1230 2023-02-23 14:16:15.268997 wagtail-localize-1.5/wagtail_localize/locale/et/LC_MESSAGES/djangojs.po
--rw-r--r--   0        0        0      425 2023-02-23 14:16:31.182085 wagtail-localize-1.5/wagtail_localize/locale/eu/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0      563 2023-02-23 14:16:15.317096 wagtail-localize-1.5/wagtail_localize/locale/eu/LC_MESSAGES/django.po
--rw-r--r--   0        0        0      518 2023-02-23 14:16:31.180723 wagtail-localize-1.5/wagtail_localize/locale/eu/LC_MESSAGES/djangojs.mo
--rw-r--r--   0        0        0      603 2023-02-23 14:16:15.311921 wagtail-localize-1.5/wagtail_localize/locale/eu/LC_MESSAGES/djangojs.po
--rw-r--r--   0        0        0      707 2023-02-23 14:16:31.280960 wagtail-localize-1.5/wagtail_localize/locale/fa/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0      888 2023-02-23 14:16:15.284949 wagtail-localize-1.5/wagtail_localize/locale/fa/LC_MESSAGES/django.po
--rw-r--r--   0        0        0     1652 2023-02-23 14:16:31.279105 wagtail-localize-1.5/wagtail_localize/locale/fa/LC_MESSAGES/djangojs.mo
--rw-r--r--   0        0        0     1753 2023-02-23 14:16:15.279330 wagtail-localize-1.5/wagtail_localize/locale/fa/LC_MESSAGES/djangojs.po
--rw-r--r--   0        0        0     2793 2023-02-23 14:16:31.277705 wagtail-localize-1.5/wagtail_localize/locale/fi/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0     2952 2023-02-23 14:16:15.238591 wagtail-localize-1.5/wagtail_localize/locale/fi/LC_MESSAGES/django.po
--rw-r--r--   0        0        0     2829 2023-02-23 14:16:31.276996 wagtail-localize-1.5/wagtail_localize/locale/fi/LC_MESSAGES/djangojs.mo
--rw-r--r--   0        0        0     2802 2023-02-23 14:16:15.233250 wagtail-localize-1.5/wagtail_localize/locale/fi/LC_MESSAGES/djangojs.po
--rw-r--r--   0        0        0     9166 2023-02-23 14:16:31.257640 wagtail-localize-1.5/wagtail_localize/locale/fr/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0     9733 2023-02-23 14:16:15.249549 wagtail-localize-1.5/wagtail_localize/locale/fr/LC_MESSAGES/django.po
--rw-r--r--   0        0        0     3519 2023-02-23 14:16:31.255694 wagtail-localize-1.5/wagtail_localize/locale/fr/LC_MESSAGES/djangojs.mo
--rw-r--r--   0        0        0     3408 2023-02-23 14:16:15.243731 wagtail-localize-1.5/wagtail_localize/locale/fr/LC_MESSAGES/djangojs.po
--rw-r--r--   0        0        0     8579 2023-02-23 14:16:31.243608 wagtail-localize-1.5/wagtail_localize/locale/gl/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0     9139 2023-02-23 14:16:15.121108 wagtail-localize-1.5/wagtail_localize/locale/gl/LC_MESSAGES/django.po
--rw-r--r--   0        0        0     3298 2023-02-23 14:16:31.241666 wagtail-localize-1.5/wagtail_localize/locale/gl/LC_MESSAGES/djangojs.mo
--rw-r--r--   0        0        0     3211 2023-02-23 14:16:15.115397 wagtail-localize-1.5/wagtail_localize/locale/gl/LC_MESSAGES/djangojs.po
--rw-r--r--   0        0        0      685 2023-02-23 14:16:31.295298 wagtail-localize-1.5/wagtail_localize/locale/he_IL/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0      880 2023-02-23 14:16:15.028561 wagtail-localize-1.5/wagtail_localize/locale/he_IL/LC_MESSAGES/django.po
--rw-r--r--   0        0        0     1091 2023-02-23 14:16:31.293398 wagtail-localize-1.5/wagtail_localize/locale/he_IL/LC_MESSAGES/djangojs.mo
--rw-r--r--   0        0        0     1155 2023-02-23 14:16:15.023030 wagtail-localize-1.5/wagtail_localize/locale/he_IL/LC_MESSAGES/djangojs.po
--rw-r--r--   0        0        0     1296 2023-02-23 14:16:31.287687 wagtail-localize-1.5/wagtail_localize/locale/hr_HR/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0     1373 2023-02-23 14:16:15.006502 wagtail-localize-1.5/wagtail_localize/locale/hr_HR/LC_MESSAGES/django.po
--rw-r--r--   0        0        0     1257 2023-02-23 14:16:31.285896 wagtail-localize-1.5/wagtail_localize/locale/hr_HR/LC_MESSAGES/djangojs.mo
--rw-r--r--   0        0        0     1293 2023-02-23 14:16:15.001057 wagtail-localize-1.5/wagtail_localize/locale/hr_HR/LC_MESSAGES/djangojs.po
--rw-r--r--   0        0        0      410 2023-02-23 14:16:31.166678 wagtail-localize-1.5/wagtail_localize/locale/ht/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0      501 2023-02-23 14:16:15.089432 wagtail-localize-1.5/wagtail_localize/locale/ht/LC_MESSAGES/django.po
--rw-r--r--   0        0        0      373 2023-02-23 14:16:31.163439 wagtail-localize-1.5/wagtail_localize/locale/ht/LC_MESSAGES/djangojs.mo
--rw-r--r--   0        0        0      415 2023-02-23 14:16:15.083959 wagtail-localize-1.5/wagtail_localize/locale/ht/LC_MESSAGES/djangojs.po
--rw-r--r--   0        0        0     8902 2023-02-23 14:16:31.165897 wagtail-localize-1.5/wagtail_localize/locale/hu/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0     9464 2023-02-23 14:16:15.131931 wagtail-localize-1.5/wagtail_localize/locale/hu/LC_MESSAGES/django.po
--rw-r--r--   0        0        0     3416 2023-02-23 14:16:31.161148 wagtail-localize-1.5/wagtail_localize/locale/hu/LC_MESSAGES/djangojs.mo
--rw-r--r--   0        0        0     3303 2023-02-23 14:16:15.126361 wagtail-localize-1.5/wagtail_localize/locale/hu/LC_MESSAGES/djangojs.po
--rw-r--r--   0        0        0      561 2023-02-23 14:16:31.236422 wagtail-localize-1.5/wagtail_localize/locale/id_ID/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0      737 2023-02-23 14:16:14.869572 wagtail-localize-1.5/wagtail_localize/locale/id_ID/LC_MESSAGES/django.po
--rw-r--r--   0        0        0     1213 2023-02-23 14:16:31.235350 wagtail-localize-1.5/wagtail_localize/locale/id_ID/LC_MESSAGES/djangojs.mo
--rw-r--r--   0        0        0     1398 2023-02-23 14:16:14.864093 wagtail-localize-1.5/wagtail_localize/locale/id_ID/LC_MESSAGES/djangojs.po
--rw-r--r--   0        0        0     8645 2023-02-23 14:16:31.322115 wagtail-localize-1.5/wagtail_localize/locale/is_IS/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0     9153 2023-02-23 14:16:15.227944 wagtail-localize-1.5/wagtail_localize/locale/is_IS/LC_MESSAGES/django.po
--rw-r--r--   0        0        0     3291 2023-02-23 14:16:31.320007 wagtail-localize-1.5/wagtail_localize/locale/is_IS/LC_MESSAGES/djangojs.mo
--rw-r--r--   0        0        0     3221 2023-02-23 14:16:15.221822 wagtail-localize-1.5/wagtail_localize/locale/is_IS/LC_MESSAGES/djangojs.po
--rw-r--r--   0        0        0     8269 2023-02-23 14:16:31.200738 wagtail-localize-1.5/wagtail_localize/locale/it/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0     8773 2023-02-23 14:16:14.933618 wagtail-localize-1.5/wagtail_localize/locale/it/LC_MESSAGES/django.po
--rw-r--r--   0        0        0     3360 2023-02-23 14:16:31.199137 wagtail-localize-1.5/wagtail_localize/locale/it/LC_MESSAGES/djangojs.mo
--rw-r--r--   0        0        0     3485 2023-02-23 14:16:14.927760 wagtail-localize-1.5/wagtail_localize/locale/it/LC_MESSAGES/djangojs.po
--rw-r--r--   0        0        0      741 2023-02-23 14:16:31.152616 wagtail-localize-1.5/wagtail_localize/locale/ja/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0      925 2023-02-23 14:16:14.893399 wagtail-localize-1.5/wagtail_localize/locale/ja/LC_MESSAGES/django.po
--rw-r--r--   0        0        0     1391 2023-02-23 14:16:31.151215 wagtail-localize-1.5/wagtail_localize/locale/ja/LC_MESSAGES/djangojs.mo
--rw-r--r--   0        0        0     1607 2023-02-23 14:16:14.887951 wagtail-localize-1.5/wagtail_localize/locale/ja/LC_MESSAGES/djangojs.po
--rw-r--r--   0        0        0      499 2023-02-23 14:16:31.223471 wagtail-localize-1.5/wagtail_localize/locale/ka/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0      581 2023-02-23 14:16:15.194568 wagtail-localize-1.5/wagtail_localize/locale/ka/LC_MESSAGES/django.po
--rw-r--r--   0        0        0      767 2023-02-23 14:16:31.221815 wagtail-localize-1.5/wagtail_localize/locale/ka/LC_MESSAGES/djangojs.mo
--rw-r--r--   0        0        0      788 2023-02-23 14:16:15.189633 wagtail-localize-1.5/wagtail_localize/locale/ka/LC_MESSAGES/djangojs.po
--rw-r--r--   0        0        0     1302 2023-02-23 14:16:31.206208 wagtail-localize-1.5/wagtail_localize/locale/ko/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0     1452 2023-02-23 14:16:15.216673 wagtail-localize-1.5/wagtail_localize/locale/ko/LC_MESSAGES/django.po
--rw-r--r--   0        0        0     1419 2023-02-23 14:16:31.205020 wagtail-localize-1.5/wagtail_localize/locale/ko/LC_MESSAGES/djangojs.mo
--rw-r--r--   0        0        0     1436 2023-02-23 14:16:15.211012 wagtail-localize-1.5/wagtail_localize/locale/ko/LC_MESSAGES/djangojs.po
--rw-r--r--   0        0        0     5586 2023-02-23 14:16:31.160015 wagtail-localize-1.5/wagtail_localize/locale/lt/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0     5943 2023-02-23 14:16:15.295612 wagtail-localize-1.5/wagtail_localize/locale/lt/LC_MESSAGES/django.po
--rw-r--r--   0        0        0     2911 2023-02-23 14:16:31.157744 wagtail-localize-1.5/wagtail_localize/locale/lt/LC_MESSAGES/djangojs.mo
--rw-r--r--   0        0        0     2842 2023-02-23 14:16:15.290176 wagtail-localize-1.5/wagtail_localize/locale/lt/LC_MESSAGES/djangojs.po
--rw-r--r--   0        0        0      637 2023-02-23 14:16:31.146249 wagtail-localize-1.5/wagtail_localize/locale/lv/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0      765 2023-02-23 14:16:14.920673 wagtail-localize-1.5/wagtail_localize/locale/lv/LC_MESSAGES/django.po
--rw-r--r--   0        0        0     1224 2023-02-23 14:16:31.144461 wagtail-localize-1.5/wagtail_localize/locale/lv/LC_MESSAGES/djangojs.mo
--rw-r--r--   0        0        0     1255 2023-02-23 14:16:14.914502 wagtail-localize-1.5/wagtail_localize/locale/lv/LC_MESSAGES/djangojs.po
--rw-r--r--   0        0        0     1016 2023-02-23 14:16:31.233238 wagtail-localize-1.5/wagtail_localize/locale/mi/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0     1112 2023-02-23 14:16:14.846462 wagtail-localize-1.5/wagtail_localize/locale/mi/LC_MESSAGES/django.po
--rw-r--r--   0        0        0      985 2023-02-23 14:16:31.231688 wagtail-localize-1.5/wagtail_localize/locale/mi/LC_MESSAGES/djangojs.mo
--rw-r--r--   0        0        0      975 2023-02-23 14:16:14.841536 wagtail-localize-1.5/wagtail_localize/locale/mi/LC_MESSAGES/djangojs.po
--rw-r--r--   0        0        0      786 2023-02-23 14:16:31.239556 wagtail-localize-1.5/wagtail_localize/locale/mn/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0      871 2023-02-23 14:16:14.836529 wagtail-localize-1.5/wagtail_localize/locale/mn/LC_MESSAGES/django.po
--rw-r--r--   0        0        0     1189 2023-02-23 14:16:31.237714 wagtail-localize-1.5/wagtail_localize/locale/mn/LC_MESSAGES/djangojs.mo
--rw-r--r--   0        0        0     1245 2023-02-23 14:16:14.831703 wagtail-localize-1.5/wagtail_localize/locale/mn/LC_MESSAGES/djangojs.po
--rw-r--r--   0        0        0      628 2023-02-23 14:16:31.325743 wagtail-localize-1.5/wagtail_localize/locale/my/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0      704 2023-02-23 14:16:15.099661 wagtail-localize-1.5/wagtail_localize/locale/my/LC_MESSAGES/django.po
--rw-r--r--   0        0        0      455 2023-02-23 14:16:31.323501 wagtail-localize-1.5/wagtail_localize/locale/my/LC_MESSAGES/djangojs.mo
--rw-r--r--   0        0        0      502 2023-02-23 14:16:15.094650 wagtail-localize-1.5/wagtail_localize/locale/my/LC_MESSAGES/djangojs.po
--rw-r--r--   0        0        0      653 2023-02-23 14:16:31.301397 wagtail-localize-1.5/wagtail_localize/locale/nb/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0      821 2023-02-23 14:16:15.184474 wagtail-localize-1.5/wagtail_localize/locale/nb/LC_MESSAGES/django.po
--rw-r--r--   0        0        0     1322 2023-02-23 14:16:31.300380 wagtail-localize-1.5/wagtail_localize/locale/nb/LC_MESSAGES/djangojs.mo
--rw-r--r--   0        0        0     1459 2023-02-23 14:16:15.178968 wagtail-localize-1.5/wagtail_localize/locale/nb/LC_MESSAGES/djangojs.po
--rw-r--r--   0        0        0     8728 2023-02-23 14:16:31.216755 wagtail-localize-1.5/wagtail_localize/locale/nl/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0     9421 2023-02-23 14:16:15.143497 wagtail-localize-1.5/wagtail_localize/locale/nl/LC_MESSAGES/django.po
--rw-r--r--   0        0        0     3309 2023-02-23 14:16:31.215611 wagtail-localize-1.5/wagtail_localize/locale/nl/LC_MESSAGES/djangojs.mo
--rw-r--r--   0        0        0     3311 2023-02-23 14:16:15.137909 wagtail-localize-1.5/wagtail_localize/locale/nl/LC_MESSAGES/djangojs.po
--rw-r--r--   0        0        0     5303 2022-07-01 10:57:34.469976 wagtail-localize-1.5/wagtail_localize/locale/nl_NL/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0     2838 2022-07-01 10:57:34.470220 wagtail-localize-1.5/wagtail_localize/locale/nl_NL/LC_MESSAGES/djangojs.mo
--rw-r--r--   0        0        0     6320 2023-02-23 14:16:31.299579 wagtail-localize-1.5/wagtail_localize/locale/pl/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0     6613 2023-02-23 14:16:14.774012 wagtail-localize-1.5/wagtail_localize/locale/pl/LC_MESSAGES/django.po
--rw-r--r--   0        0        0     3319 2023-02-23 14:16:31.296916 wagtail-localize-1.5/wagtail_localize/locale/pl/LC_MESSAGES/djangojs.mo
--rw-r--r--   0        0        0     3221 2023-02-23 14:16:14.766966 wagtail-localize-1.5/wagtail_localize/locale/pl/LC_MESSAGES/djangojs.po
--rw-r--r--   0        0        0     7506 2023-02-23 14:16:31.177083 wagtail-localize-1.5/wagtail_localize/locale/pt_BR/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0     8157 2023-02-23 14:16:14.881269 wagtail-localize-1.5/wagtail_localize/locale/pt_BR/LC_MESSAGES/django.po
--rw-r--r--   0        0        0     3384 2023-02-23 14:16:31.175667 wagtail-localize-1.5/wagtail_localize/locale/pt_BR/LC_MESSAGES/djangojs.mo
--rw-r--r--   0        0        0     3377 2023-02-23 14:16:14.875010 wagtail-localize-1.5/wagtail_localize/locale/pt_BR/LC_MESSAGES/djangojs.po
--rw-r--r--   0        0        0     8678 2023-02-23 14:16:31.149992 wagtail-localize-1.5/wagtail_localize/locale/pt_PT/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0     9281 2023-02-23 14:16:14.968390 wagtail-localize-1.5/wagtail_localize/locale/pt_PT/LC_MESSAGES/django.po
--rw-r--r--   0        0        0     3359 2023-02-23 14:16:31.147534 wagtail-localize-1.5/wagtail_localize/locale/pt_PT/LC_MESSAGES/djangojs.mo
--rw-r--r--   0        0        0     3289 2023-02-23 14:16:14.962480 wagtail-localize-1.5/wagtail_localize/locale/pt_PT/LC_MESSAGES/djangojs.po
--rw-r--r--   0        0        0     8593 2023-02-23 14:16:31.210743 wagtail-localize-1.5/wagtail_localize/locale/ro/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0     9029 2023-02-23 14:16:15.039590 wagtail-localize-1.5/wagtail_localize/locale/ro/LC_MESSAGES/django.po
--rw-r--r--   0        0        0     3349 2023-02-23 14:16:31.209331 wagtail-localize-1.5/wagtail_localize/locale/ro/LC_MESSAGES/djangojs.mo
--rw-r--r--   0        0        0     3202 2023-02-23 14:16:15.034017 wagtail-localize-1.5/wagtail_localize/locale/ro/LC_MESSAGES/djangojs.po
--rw-r--r--   0        0        0    10730 2023-02-23 14:16:31.197332 wagtail-localize-1.5/wagtail_localize/locale/ru/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0    11422 2023-02-23 14:16:14.994681 wagtail-localize-1.5/wagtail_localize/locale/ru/LC_MESSAGES/django.po
--rw-r--r--   0        0        0     4473 2023-02-23 14:16:31.194930 wagtail-localize-1.5/wagtail_localize/locale/ru/LC_MESSAGES/djangojs.mo
--rw-r--r--   0        0        0     4458 2023-02-23 14:16:14.987025 wagtail-localize-1.5/wagtail_localize/locale/ru/LC_MESSAGES/djangojs.po
--rw-r--r--   0        0        0      674 2023-02-23 14:16:31.173224 wagtail-localize-1.5/wagtail_localize/locale/sk_SK/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0      828 2023-02-23 14:16:14.795091 wagtail-localize-1.5/wagtail_localize/locale/sk_SK/LC_MESSAGES/django.po
--rw-r--r--   0        0        0     1176 2023-02-23 14:16:31.171596 wagtail-localize-1.5/wagtail_localize/locale/sk_SK/LC_MESSAGES/djangojs.mo
--rw-r--r--   0        0        0     1192 2023-02-23 14:16:14.789736 wagtail-localize-1.5/wagtail_localize/locale/sk_SK/LC_MESSAGES/djangojs.po
--rw-r--r--   0        0        0     6545 2023-02-23 14:16:31.226932 wagtail-localize-1.5/wagtail_localize/locale/sl/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0     6915 2023-02-23 14:16:14.760842 wagtail-localize-1.5/wagtail_localize/locale/sl/LC_MESSAGES/django.po
--rw-r--r--   0        0        0     3270 2023-02-23 14:16:31.225065 wagtail-localize-1.5/wagtail_localize/locale/sl/LC_MESSAGES/djangojs.mo
--rw-r--r--   0        0        0     3190 2023-02-23 14:16:14.754030 wagtail-localize-1.5/wagtail_localize/locale/sl/LC_MESSAGES/djangojs.po
--rw-r--r--   0        0        0      434 2023-02-23 14:16:31.178717 wagtail-localize-1.5/wagtail_localize/locale/sr/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0      527 2023-02-23 14:16:15.077681 wagtail-localize-1.5/wagtail_localize/locale/sr/LC_MESSAGES/django.po
--rw-r--r--   0        0        0     8613 2023-02-23 14:16:31.315760 wagtail-localize-1.5/wagtail_localize/locale/sv/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0     9230 2023-02-23 14:16:14.806087 wagtail-localize-1.5/wagtail_localize/locale/sv/LC_MESSAGES/django.po
--rw-r--r--   0        0        0     3237 2023-02-23 14:16:31.313629 wagtail-localize-1.5/wagtail_localize/locale/sv/LC_MESSAGES/djangojs.mo
--rw-r--r--   0        0        0     3215 2023-02-23 14:16:14.800532 wagtail-localize-1.5/wagtail_localize/locale/sv/LC_MESSAGES/djangojs.po
--rw-r--r--   0        0        0      433 2023-02-23 14:16:31.308933 wagtail-localize-1.5/wagtail_localize/locale/ta/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0      515 2023-02-23 14:16:15.327904 wagtail-localize-1.5/wagtail_localize/locale/ta/LC_MESSAGES/django.po
--rw-r--r--   0        0        0      343 2023-02-23 14:16:31.306752 wagtail-localize-1.5/wagtail_localize/locale/ta/LC_MESSAGES/djangojs.mo
--rw-r--r--   0        0        0      374 2023-02-23 14:16:15.322597 wagtail-localize-1.5/wagtail_localize/locale/ta/LC_MESSAGES/djangojs.po
--rw-r--r--   0        0        0      550 2023-02-23 14:16:31.156941 wagtail-localize-1.5/wagtail_localize/locale/tet/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0      717 2023-02-23 14:16:15.050588 wagtail-localize-1.5/wagtail_localize/locale/tet/LC_MESSAGES/django.po
--rw-r--r--   0        0        0      998 2023-02-23 14:16:31.154747 wagtail-localize-1.5/wagtail_localize/locale/tet/LC_MESSAGES/djangojs.mo
--rw-r--r--   0        0        0     1139 2023-02-23 14:16:15.045284 wagtail-localize-1.5/wagtail_localize/locale/tet/LC_MESSAGES/djangojs.po
--rw-r--r--   0        0        0      810 2023-02-23 14:16:31.318754 wagtail-localize-1.5/wagtail_localize/locale/th/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0      934 2023-02-23 14:16:15.338270 wagtail-localize-1.5/wagtail_localize/locale/th/LC_MESSAGES/django.po
--rw-r--r--   0        0        0     1429 2023-02-23 14:16:31.317263 wagtail-localize-1.5/wagtail_localize/locale/th/LC_MESSAGES/djangojs.mo
--rw-r--r--   0        0        0     1476 2023-02-23 14:16:15.333131 wagtail-localize-1.5/wagtail_localize/locale/th/LC_MESSAGES/djangojs.po
--rw-r--r--   0        0        0      583 2023-02-23 14:16:31.261237 wagtail-localize-1.5/wagtail_localize/locale/tr/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0      801 2023-02-23 14:16:15.349405 wagtail-localize-1.5/wagtail_localize/locale/tr/LC_MESSAGES/django.po
--rw-r--r--   0        0        0     1254 2023-02-23 14:16:31.258988 wagtail-localize-1.5/wagtail_localize/locale/tr/LC_MESSAGES/djangojs.mo
--rw-r--r--   0        0        0     1404 2023-02-23 14:16:15.343845 wagtail-localize-1.5/wagtail_localize/locale/tr/LC_MESSAGES/djangojs.po
--rw-r--r--   0        0        0      649 2023-02-23 14:16:31.169605 wagtail-localize-1.5/wagtail_localize/locale/tr_TR/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0      854 2023-02-23 14:16:15.359644 wagtail-localize-1.5/wagtail_localize/locale/tr_TR/LC_MESSAGES/django.po
--rw-r--r--   0        0        0     1213 2023-02-23 14:16:31.168140 wagtail-localize-1.5/wagtail_localize/locale/tr_TR/LC_MESSAGES/djangojs.mo
--rw-r--r--   0        0        0     1329 2023-02-23 14:16:15.354477 wagtail-localize-1.5/wagtail_localize/locale/tr_TR/LC_MESSAGES/djangojs.po
--rw-r--r--   0        0        0     9314 2023-02-23 14:16:31.214667 wagtail-localize-1.5/wagtail_localize/locale/uk/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0     9899 2023-02-23 14:16:15.072395 wagtail-localize-1.5/wagtail_localize/locale/uk/LC_MESSAGES/django.po
--rw-r--r--   0        0        0     4261 2023-02-23 14:16:31.211413 wagtail-localize-1.5/wagtail_localize/locale/uk/LC_MESSAGES/djangojs.mo
--rw-r--r--   0        0        0     4432 2023-02-23 14:16:15.066583 wagtail-localize-1.5/wagtail_localize/locale/uk/LC_MESSAGES/djangojs.po
--rw-r--r--   0        0        0      667 2023-02-23 14:16:31.270661 wagtail-localize-1.5/wagtail_localize/locale/vi/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0      852 2023-02-23 14:16:14.784668 wagtail-localize-1.5/wagtail_localize/locale/vi/LC_MESSAGES/django.po
--rw-r--r--   0        0        0     1550 2023-02-23 14:16:31.269147 wagtail-localize-1.5/wagtail_localize/locale/vi/LC_MESSAGES/djangojs.mo
--rw-r--r--   0        0        0     1582 2023-02-23 14:16:14.779407 wagtail-localize-1.5/wagtail_localize/locale/vi/LC_MESSAGES/djangojs.po
--rw-r--r--   0        0        0      495 2023-02-23 14:16:31.291239 wagtail-localize-1.5/wagtail_localize/locale/zh/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0      691 2023-02-23 14:16:15.060901 wagtail-localize-1.5/wagtail_localize/locale/zh/LC_MESSAGES/django.po
--rw-r--r--   0        0        0      765 2023-02-23 14:16:31.289811 wagtail-localize-1.5/wagtail_localize/locale/zh/LC_MESSAGES/djangojs.mo
--rw-r--r--   0        0        0      938 2023-02-23 14:16:15.055913 wagtail-localize-1.5/wagtail_localize/locale/zh/LC_MESSAGES/djangojs.po
--rw-r--r--   0        0        0     7010 2023-02-23 14:16:31.246962 wagtail-localize-1.5/wagtail_localize/locale/zh_Hans/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0     7554 2023-02-23 14:16:14.980894 wagtail-localize-1.5/wagtail_localize/locale/zh_Hans/LC_MESSAGES/django.po
--rw-r--r--   0        0        0     3102 2023-02-23 14:16:31.245225 wagtail-localize-1.5/wagtail_localize/locale/zh_Hans/LC_MESSAGES/djangojs.mo
--rw-r--r--   0        0        0     3132 2023-02-23 14:16:14.974330 wagtail-localize-1.5/wagtail_localize/locale/zh_Hans/LC_MESSAGES/djangojs.po
--rw-r--r--   0        0        0      793 2023-02-23 14:16:31.312028 wagtail-localize-1.5/wagtail_localize/locale/zh_Hant/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0      890 2023-02-23 14:16:15.017525 wagtail-localize-1.5/wagtail_localize/locale/zh_Hant/LC_MESSAGES/django.po
--rw-r--r--   0        0        0     1207 2023-02-23 14:16:31.310309 wagtail-localize-1.5/wagtail_localize/locale/zh_Hant/LC_MESSAGES/djangojs.mo
--rw-r--r--   0        0        0     1283 2023-02-23 14:16:15.012030 wagtail-localize-1.5/wagtail_localize/locale/zh_Hant/LC_MESSAGES/djangojs.po
--rw-r--r--   0        0        0        0 2022-09-23 10:15:38.922735 wagtail-localize-1.5/wagtail_localize/locales/__init__.py
--rw-r--r--   0        0        0      267 2022-07-01 10:57:34.513956 wagtail-localize-1.5/wagtail_localize/locales/apps.py
--rw-r--r--   0        0        0      917 2022-07-01 10:57:34.515898 wagtail-localize-1.5/wagtail_localize/locales/components.py
--rw-r--r--   0        0        0     1315 2023-02-15 19:30:42.626580 wagtail-localize-1.5/wagtail_localize/locales/forms.py
--rw-r--r--   0        0        0      337 2023-02-23 14:16:31.130439 wagtail-localize-1.5/wagtail_localize/locales/locale/en/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0     2436 2023-02-23 14:15:49.501551 wagtail-localize-1.5/wagtail_localize/locales/locale/en/LC_MESSAGES/django.po
--rw-r--r--   0        0        0      710 2022-07-01 10:57:34.510343 wagtail-localize-1.5/wagtail_localize/locales/locale/es/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0     1979 2022-07-01 10:57:34.509539 wagtail-localize-1.5/wagtail_localize/locales/locale/fi/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0     1981 2022-07-01 10:57:34.509928 wagtail-localize-1.5/wagtail_localize/locales/locale/fr/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0     2023 2022-07-01 10:57:34.507986 wagtail-localize-1.5/wagtail_localize/locales/locale/hr_HR/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0     2053 2022-07-01 10:57:34.509174 wagtail-localize-1.5/wagtail_localize/locales/locale/is_IS/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0     2010 2022-07-01 10:57:34.508810 wagtail-localize-1.5/wagtail_localize/locales/locale/nl_NL/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0     1986 2022-07-01 10:57:34.506765 wagtail-localize-1.5/wagtail_localize/locales/locale/pt_PT/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0     2453 2022-07-01 10:57:34.507498 wagtail-localize-1.5/wagtail_localize/locales/locale/ru/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0     2026 2022-07-01 10:57:34.506256 wagtail-localize-1.5/wagtail_localize/locales/locale/sv/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0     1927 2022-07-01 10:57:34.507136 wagtail-localize-1.5/wagtail_localize/locales/locale/zh_Hans/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0      559 2022-07-01 10:57:34.508337 wagtail-localize-1.5/wagtail_localize/locales/locale/zh_Hant/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0      917 2022-07-01 10:57:34.515715 wagtail-localize-1.5/wagtail_localize/locales/templates/wagtaillocales/confirm_delete.html
--rw-r--r--   0        0        0      207 2022-07-01 10:57:34.515314 wagtail-localize-1.5/wagtail_localize/locales/templates/wagtaillocales/create.html
--rw-r--r--   0        0        0     2762 2022-07-01 10:57:34.515505 wagtail-localize-1.5/wagtail_localize/locales/templates/wagtaillocales/edit.html
--rw-r--r--   0        0        0     2148 2022-07-01 10:57:34.515123 wagtail-localize-1.5/wagtail_localize/locales/templates/wagtaillocales/index.html
--rw-r--r--   0        0        0    13996 2023-02-15 19:30:42.626693 wagtail-localize-1.5/wagtail_localize/locales/tests.py
--rw-r--r--   0        0        0      462 2023-02-15 19:30:42.626782 wagtail-localize-1.5/wagtail_localize/locales/utils.py
--rw-r--r--   0        0        0     7259 2023-02-15 19:30:42.626895 wagtail-localize-1.5/wagtail_localize/locales/views.py
--rw-r--r--   0        0        0     1052 2023-02-15 19:30:42.626987 wagtail-localize-1.5/wagtail_localize/locales/wagtail_hooks.py
--rw-r--r--   0        0        0      385 2022-07-01 10:57:34.538728 wagtail-localize-1.5/wagtail_localize/machine_translators/__init__.py
--rw-r--r--   0        0        0      303 2022-09-12 13:15:14.646119 wagtail-localize-1.5/wagtail_localize/machine_translators/base.py
--rw-r--r--   0        0        0     1538 2022-09-12 13:15:14.646264 wagtail-localize-1.5/wagtail_localize/machine_translators/deepl.py
--rw-r--r--   0        0        0     1508 2022-07-01 10:57:34.540336 wagtail-localize-1.5/wagtail_localize/machine_translators/dummy.py
--rw-r--r--   0        0        0     1957 2023-01-22 13:17:54.447370 wagtail-localize-1.5/wagtail_localize/machine_translators/google.py
--rw-r--r--   0        0        0        0 2022-07-01 10:57:34.540801 wagtail-localize-1.5/wagtail_localize/management/__init__.py
--rw-r--r--   0        0        0        0 2022-07-01 10:57:34.541279 wagtail-localize-1.5/wagtail_localize/management/commands/__init__.py
--rw-r--r--   0        0        0      550 2022-07-01 10:57:34.541517 wagtail-localize-1.5/wagtail_localize/management/commands/sync_locale_trees.py
--rw-r--r--   0        0        0    14672 2022-11-04 12:29:12.963230 wagtail-localize-1.5/wagtail_localize/migrations/0001_initial.py
--rw-r--r--   0        0        0     2247 2022-07-01 10:57:34.432921 wagtail-localize-1.5/wagtail_localize/migrations/0002_translation.py
--rw-r--r--   0        0        0     1028 2022-07-01 10:57:34.427359 wagtail-localize-1.5/wagtail_localize/migrations/0003_delete_translation_sources.py
--rw-r--r--   0        0        0      860 2022-07-01 10:57:34.431933 wagtail-localize-1.5/wagtail_localize/migrations/0004_one_source_per_objectlocale.py
--rw-r--r--   0        0        0      553 2022-07-01 10:57:34.432415 wagtail-localize-1.5/wagtail_localize/migrations/0005_remove_translationsource_object.py
--rw-r--r--   0        0        0     1791 2022-07-01 10:57:34.432577 wagtail-localize-1.5/wagtail_localize/migrations/0006_create_submit_translation_permission.py
--rw-r--r--   0        0        0      783 2022-07-01 10:57:34.427737 wagtail-localize-1.5/wagtail_localize/migrations/0007_stringtranslation_type_and_tool_name.py
--rw-r--r--   0        0        0      764 2022-07-01 10:57:34.432114 wagtail-localize-1.5/wagtail_localize/migrations/0008_stringtranslation_last_translated_by.py
--rw-r--r--   0        0        0      592 2022-07-01 10:57:34.432267 wagtail-localize-1.5/wagtail_localize/migrations/0009_stringtranslation_errors.py
--rw-r--r--   0        0        0     1399 2022-07-01 10:57:34.427501 wagtail-localize-1.5/wagtail_localize/migrations/0010_overridablesegment.py
--rw-r--r--   0        0        0     2226 2022-07-01 10:57:34.431151 wagtail-localize-1.5/wagtail_localize/migrations/0011_segmentoverride.py
--rw-r--r--   0        0        0     1329 2022-07-01 10:57:34.431708 wagtail-localize-1.5/wagtail_localize/migrations/0012_localesynchronization.py
--rw-r--r--   0        0        0      428 2022-07-01 10:57:34.432763 wagtail-localize-1.5/wagtail_localize/migrations/0013_translationsource_schema_version.py
--rw-r--r--   0        0        0      372 2022-07-01 10:57:34.427137 wagtail-localize-1.5/wagtail_localize/migrations/0014_remove_translation_source_last_updated_at.py
--rw-r--r--   0        0        0      465 2022-07-01 10:57:34.431395 wagtail-localize-1.5/wagtail_localize/migrations/0015_translationcontext_field_path.py
--rw-r--r--   0        0        0        0 2022-07-01 10:57:34.427580 wagtail-localize-1.5/wagtail_localize/migrations/__init__.py
--rw-r--r--   0        0        0        0 2022-09-23 10:15:38.922854 wagtail-localize-1.5/wagtail_localize/modeladmin/__init__.py
--rw-r--r--   0        0        0      221 2022-07-01 10:57:34.554873 wagtail-localize-1.5/wagtail_localize/modeladmin/apps.py
--rw-r--r--   0        0        0     3138 2023-02-15 19:30:42.627204 wagtail-localize-1.5/wagtail_localize/modeladmin/helpers.py
--rw-r--r--   0        0        0     2223 2023-02-15 19:31:51.787872 wagtail-localize-1.5/wagtail_localize/modeladmin/options.py
--rw-r--r--   0        0        0      313 2022-07-01 10:57:34.555903 wagtail-localize-1.5/wagtail_localize/modeladmin/templates/wagtail_localize/modeladmin/includes/button.html
--rw-r--r--   0        0        0      162 2022-07-01 10:57:34.556094 wagtail-localize-1.5/wagtail_localize/modeladmin/templates/wagtail_localize/modeladmin/includes/header_with_breadcrumb.html
--rw-r--r--   0        0        0       46 2022-07-01 10:57:34.557049 wagtail-localize-1.5/wagtail_localize/modeladmin/templates/wagtail_localize/modeladmin/translatable_choose_parent.html
--rw-r--r--   0        0        0      309 2023-02-15 19:30:42.627410 wagtail-localize-1.5/wagtail_localize/modeladmin/templates/wagtail_localize/modeladmin/translatable_create.html
--rw-r--r--   0        0        0       39 2022-07-01 10:57:34.556233 wagtail-localize-1.5/wagtail_localize/modeladmin/templates/wagtail_localize/modeladmin/translatable_delete.html
--rw-r--r--   0        0        0     1151 2022-09-23 10:15:38.923251 wagtail-localize-1.5/wagtail_localize/modeladmin/templates/wagtail_localize/modeladmin/translatable_edit.html
--rw-r--r--   0        0        0       40 2022-07-01 10:57:34.556386 wagtail-localize-1.5/wagtail_localize/modeladmin/templates/wagtail_localize/modeladmin/translatable_history.html
--rw-r--r--   0        0        0     1065 2022-07-01 10:57:34.556547 wagtail-localize-1.5/wagtail_localize/modeladmin/templates/wagtail_localize/modeladmin/translatable_index.html
--rw-r--r--   0        0        0      245 2022-08-31 18:34:50.710573 wagtail-localize-1.5/wagtail_localize/modeladmin/templates/wagtail_localize/modeladmin/translatable_inspect.html
--rw-r--r--   0        0        0    27627 2023-02-15 19:30:42.627566 wagtail-localize-1.5/wagtail_localize/modeladmin/tests.py
--rw-r--r--   0        0        0     7471 2023-02-15 19:30:42.627688 wagtail-localize-1.5/wagtail_localize/modeladmin/views.py
--rw-r--r--   0        0        0      616 2023-02-15 19:30:42.627791 wagtail-localize-1.5/wagtail_localize/modeladmin/wagtail_hooks.py
--rw-r--r--   0        0        0    85122 2023-02-15 19:30:42.628116 wagtail-localize-1.5/wagtail_localize/models.py
--rw-r--r--   0        0        0     4620 2023-02-15 19:30:42.628255 wagtail-localize-1.5/wagtail_localize/operations.py
--rw-r--r--   0        0        0      141 2022-07-01 10:57:34.570543 wagtail-localize-1.5/wagtail_localize/segments/__init__.py
--rw-r--r--   0        0        0    13186 2023-02-15 19:30:42.628385 wagtail-localize-1.5/wagtail_localize/segments/extract.py
--rw-r--r--   0        0        0    12641 2023-02-15 19:30:42.628513 wagtail-localize-1.5/wagtail_localize/segments/ingest.py
--rw-r--r--   0        0        0    12328 2023-02-15 19:31:17.389809 wagtail-localize-1.5/wagtail_localize/segments/types.py
--rw-r--r--   0        0        0     1847 2023-02-15 19:30:42.628953 wagtail-localize-1.5/wagtail_localize/side_panels.py
--rw-r--r--   0        0        0      880 2023-02-23 14:50:54.142988 wagtail-localize-1.5/wagtail_localize/static/wagtail_localize/css/wagtail-localize-component-form.css
--rw-r--r--   0        0        0     1501 2023-02-23 14:50:54.142947 wagtail-localize-1.5/wagtail_localize/static/wagtail_localize/js/wagtail-localize-component-form.js
--rw-r--r--   0        0        0    84652 2023-02-23 14:50:54.142929 wagtail-localize-1.5/wagtail_localize/static/wagtail_localize/js/wagtail-localize.js
--rw-r--r--   0        0        0    14658 2023-02-15 19:31:17.389857 wagtail-localize-1.5/wagtail_localize/strings.py
--rw-r--r--   0        0        0     6973 2023-02-15 19:31:17.389902 wagtail-localize-1.5/wagtail_localize/synctree.py
--rw-r--r--   0        0        0     1377 2022-07-01 10:57:34.504798 wagtail-localize-1.5/wagtail_localize/tasks.py
--rw-r--r--   0        0        0     1273 2022-07-01 10:57:34.562536 wagtail-localize-1.5/wagtail_localize/templates/wagtail_localize/admin/_components.html
--rw-r--r--   0        0        0     1349 2022-07-01 10:57:34.560800 wagtail-localize-1.5/wagtail_localize/templates/wagtail_localize/admin/confirm_convert_to_alias.html
--rw-r--r--   0        0        0      893 2022-07-01 10:57:34.561400 wagtail-localize-1.5/wagtail_localize/templates/wagtail_localize/admin/edit_translatable_alias.html
--rw-r--r--   0        0        0     2298 2023-02-15 19:30:42.629292 wagtail-localize-1.5/wagtail_localize/templates/wagtail_localize/admin/edit_translation.html
--rw-r--r--   0        0        0      742 2022-09-13 08:26:04.349160 wagtail-localize-1.5/wagtail_localize/templates/wagtail_localize/admin/includes/generic_header.html
--rw-r--r--   0        0        0     2462 2022-07-01 10:57:34.561084 wagtail-localize-1.5/wagtail_localize/templates/wagtail_localize/admin/submit_translation.html
--rw-r--r--   0        0        0     1947 2022-07-01 10:57:34.562358 wagtail-localize-1.5/wagtail_localize/templates/wagtail_localize/admin/translations_report.html
--rw-r--r--   0        0        0     4225 2023-02-15 19:30:42.629398 wagtail-localize-1.5/wagtail_localize/templates/wagtail_localize/admin/update_translations.html
--rw-r--r--   0        0        0      501 2022-07-01 10:57:34.563064 wagtail-localize-1.5/wagtail_localize/templates/wagtail_localize/icons/wagtail-localize-convert.svg
--rw-r--r--   0        0        0      918 2022-10-12 20:12:40.316546 wagtail-localize-1.5/wagtail_localize/templates/wagtail_localize/icons/wagtail-localize-language.svg
--rw-r--r--   0        0        0        0 2022-07-01 10:57:34.425464 wagtail-localize-1.5/wagtail_localize/templatetags/__init__.py
--rw-r--r--   0        0        0      324 2022-07-01 10:57:34.426417 wagtail-localize-1.5/wagtail_localize/templatetags/wagtail_localize_admin_tags.py
--rw-r--r--   0        0        0     1232 2022-09-23 10:15:38.927745 wagtail-localize-1.5/wagtail_localize/version.py
--rw-r--r--   0        0        0        0 2022-07-01 10:57:34.565383 wagtail-localize-1.5/wagtail_localize/views/__init__.py
--rw-r--r--   0        0        0     6474 2023-02-15 19:30:42.632123 wagtail-localize-1.5/wagtail_localize/views/convert.py
--rw-r--r--   0        0        0    52453 2023-02-15 19:31:17.390082 wagtail-localize-1.5/wagtail_localize/views/edit_translation.py
--rw-r--r--   0        0        0     4250 2023-02-15 19:30:42.632454 wagtail-localize-1.5/wagtail_localize/views/report.py
--rw-r--r--   0        0        0     1350 2023-02-15 19:30:42.632653 wagtail-localize-1.5/wagtail_localize/views/snippets_api.py
--rw-r--r--   0        0        0     8968 2023-02-15 19:30:42.632802 wagtail-localize-1.5/wagtail_localize/views/submit_translations.py
--rw-r--r--   0        0        0     6591 2023-02-15 19:30:42.632929 wagtail-localize-1.5/wagtail_localize/views/update_translations.py
--rw-r--r--   0        0        0    15102 2023-02-15 19:30:42.633064 wagtail-localize-1.5/wagtail_localize/wagtail_hooks.py
--rw-r--r--   0        0        0     6013 1970-01-01 00:00:00.000000 wagtail-localize-1.5/PKG-INFO
+-rw-r--r--   0        0        0    12366 2023-06-11 10:42:27.019754 wagtail-localize-1.5.1/CHANGELOG.md
+-rw-r--r--   0        0        0     1539 2022-07-01 10:57:34.575741 wagtail-localize-1.5.1/LICENSE
+-rw-r--r--   0        0        0     3912 2023-06-02 22:09:08.195237 wagtail-localize-1.5.1/README.md
+-rw-r--r--   0        0        0     2273 2023-06-11 10:42:27.020191 wagtail-localize-1.5.1/pyproject.toml
+-rw-r--r--   0        0        0        4 2023-02-15 19:30:49.157059 wagtail-localize-1.5.1/runtime.txt
+-rw-r--r--   0        0        0      384 2022-07-01 10:58:32.557727 wagtail-localize-1.5.1/setup.cfg
+-rw-r--r--   0        0        0      154 2023-06-11 10:42:27.020464 wagtail-localize-1.5.1/wagtail_localize/__init__.py
+-rw-r--r--   0        0        0      367 2022-07-01 10:57:34.552360 wagtail-localize-1.5.1/wagtail_localize/apps.py
+-rw-r--r--   0        0        0      260 2023-02-15 19:30:42.626257 wagtail-localize-1.5.1/wagtail_localize/compat.py
+-rw-r--r--   0        0        0     7001 2023-02-15 19:31:17.389647 wagtail-localize-1.5.1/wagtail_localize/components.py
+-rw-r--r--   0        0        0    10830 2023-02-15 19:30:42.626478 wagtail-localize-1.5.1/wagtail_localize/fields.py
+-rw-r--r--   0        0        0      355 2023-06-11 10:42:27.020652 wagtail-localize-1.5.1/wagtail_localize/locale/af/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0      452 2023-06-11 10:42:27.020750 wagtail-localize-1.5.1/wagtail_localize/locale/af/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0      332 2023-06-11 10:42:27.020843 wagtail-localize-1.5.1/wagtail_localize/locale/af/LC_MESSAGES/djangojs.mo
+-rw-r--r--   0        0        0      380 2023-06-11 10:42:27.020945 wagtail-localize-1.5.1/wagtail_localize/locale/af/LC_MESSAGES/djangojs.po
+-rw-r--r--   0        0        0      837 2023-06-11 10:42:27.021041 wagtail-localize-1.5.1/wagtail_localize/locale/ar/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0     1076 2023-06-11 10:42:27.021158 wagtail-localize-1.5.1/wagtail_localize/locale/ar/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     1260 2023-06-11 10:42:27.021265 wagtail-localize-1.5.1/wagtail_localize/locale/ar/LC_MESSAGES/djangojs.mo
+-rw-r--r--   0        0        0     1400 2023-06-11 10:42:27.021381 wagtail-localize-1.5.1/wagtail_localize/locale/ar/LC_MESSAGES/djangojs.po
+-rw-r--r--   0        0        0      504 2023-06-11 10:42:27.021503 wagtail-localize-1.5.1/wagtail_localize/locale/az_AZ/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0      602 2023-06-11 10:42:27.021587 wagtail-localize-1.5.1/wagtail_localize/locale/az_AZ/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0      435 2023-06-11 10:42:27.021674 wagtail-localize-1.5.1/wagtail_localize/locale/az_AZ/LC_MESSAGES/djangojs.mo
+-rw-r--r--   0        0        0      490 2023-06-11 10:42:27.021853 wagtail-localize-1.5.1/wagtail_localize/locale/az_AZ/LC_MESSAGES/djangojs.po
+-rw-r--r--   0        0        0      794 2023-06-11 10:42:27.022045 wagtail-localize-1.5.1/wagtail_localize/locale/be/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0      883 2023-06-11 10:42:27.022202 wagtail-localize-1.5.1/wagtail_localize/locale/be/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     1360 2023-06-11 10:42:27.022338 wagtail-localize-1.5.1/wagtail_localize/locale/be/LC_MESSAGES/djangojs.mo
+-rw-r--r--   0        0        0     1407 2023-06-11 10:42:27.022461 wagtail-localize-1.5.1/wagtail_localize/locale/be/LC_MESSAGES/djangojs.po
+-rw-r--r--   0        0        0      423 2023-06-11 10:42:27.022582 wagtail-localize-1.5.1/wagtail_localize/locale/bg/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0      568 2023-06-11 10:42:27.022676 wagtail-localize-1.5.1/wagtail_localize/locale/bg/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0      825 2023-06-11 10:42:27.022776 wagtail-localize-1.5.1/wagtail_localize/locale/bg/LC_MESSAGES/djangojs.mo
+-rw-r--r--   0        0        0      901 2023-06-11 10:42:27.022875 wagtail-localize-1.5.1/wagtail_localize/locale/bg/LC_MESSAGES/djangojs.po
+-rw-r--r--   0        0        0      541 2023-06-11 10:42:27.022980 wagtail-localize-1.5.1/wagtail_localize/locale/bn/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0      673 2023-06-11 10:42:27.023069 wagtail-localize-1.5.1/wagtail_localize/locale/bn/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0      723 2023-06-11 10:42:27.023171 wagtail-localize-1.5.1/wagtail_localize/locale/bn/LC_MESSAGES/djangojs.mo
+-rw-r--r--   0        0        0      796 2023-06-11 10:42:27.023261 wagtail-localize-1.5.1/wagtail_localize/locale/bn/LC_MESSAGES/djangojs.po
+-rw-r--r--   0        0        0     8727 2023-06-11 10:42:27.023449 wagtail-localize-1.5.1/wagtail_localize/locale/ca/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0     9246 2023-06-11 10:42:27.023570 wagtail-localize-1.5.1/wagtail_localize/locale/ca/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     3131 2023-06-11 10:42:27.023712 wagtail-localize-1.5.1/wagtail_localize/locale/ca/LC_MESSAGES/djangojs.mo
+-rw-r--r--   0        0        0     3064 2023-06-11 10:42:27.023840 wagtail-localize-1.5.1/wagtail_localize/locale/ca/LC_MESSAGES/djangojs.po
+-rw-r--r--   0        0        0     5617 2023-06-11 10:42:27.023978 wagtail-localize-1.5.1/wagtail_localize/locale/cs/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0     5962 2023-06-11 10:42:27.024127 wagtail-localize-1.5.1/wagtail_localize/locale/cs/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     2628 2023-06-11 10:42:27.024253 wagtail-localize-1.5.1/wagtail_localize/locale/cs/LC_MESSAGES/djangojs.mo
+-rw-r--r--   0        0        0     2552 2023-06-11 10:42:27.024377 wagtail-localize-1.5.1/wagtail_localize/locale/cs/LC_MESSAGES/djangojs.po
+-rw-r--r--   0        0        0     8527 2023-06-11 10:42:27.024525 wagtail-localize-1.5.1/wagtail_localize/locale/cy/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0     9068 2023-06-11 10:42:27.024635 wagtail-localize-1.5.1/wagtail_localize/locale/cy/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     3066 2023-06-11 10:42:27.024794 wagtail-localize-1.5.1/wagtail_localize/locale/cy/LC_MESSAGES/djangojs.mo
+-rw-r--r--   0        0        0     2974 2023-06-11 10:42:27.024916 wagtail-localize-1.5.1/wagtail_localize/locale/cy/LC_MESSAGES/djangojs.po
+-rw-r--r--   0        0        0      498 2023-06-11 10:42:27.025031 wagtail-localize-1.5.1/wagtail_localize/locale/da/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0      574 2023-06-11 10:42:27.025127 wagtail-localize-1.5.1/wagtail_localize/locale/da/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0      797 2023-06-11 10:42:27.025231 wagtail-localize-1.5.1/wagtail_localize/locale/da/LC_MESSAGES/djangojs.mo
+-rw-r--r--   0        0        0      952 2023-06-11 10:42:27.025497 wagtail-localize-1.5.1/wagtail_localize/locale/da/LC_MESSAGES/djangojs.po
+-rw-r--r--   0        0        0     8880 2023-06-11 10:42:27.025631 wagtail-localize-1.5.1/wagtail_localize/locale/de/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0     9632 2023-06-11 10:42:27.025730 wagtail-localize-1.5.1/wagtail_localize/locale/de/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     3181 2023-06-11 10:42:27.025826 wagtail-localize-1.5.1/wagtail_localize/locale/de/LC_MESSAGES/djangojs.mo
+-rw-r--r--   0        0        0     3208 2023-06-11 10:42:27.025912 wagtail-localize-1.5.1/wagtail_localize/locale/de/LC_MESSAGES/djangojs.po
+-rw-r--r--   0        0        0      744 2023-06-11 10:42:27.026019 wagtail-localize-1.5.1/wagtail_localize/locale/el/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0     1022 2023-06-11 10:42:27.026123 wagtail-localize-1.5.1/wagtail_localize/locale/el/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     1460 2023-06-11 10:42:27.026237 wagtail-localize-1.5.1/wagtail_localize/locale/el/LC_MESSAGES/djangojs.mo
+-rw-r--r--   0        0        0     1590 2023-06-11 10:42:27.026330 wagtail-localize-1.5.1/wagtail_localize/locale/el/LC_MESSAGES/djangojs.po
+-rw-r--r--   0        0        0      210 2023-06-11 10:35:07.230803 wagtail-localize-1.5.1/wagtail_localize/locale/en/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0     9124 2023-06-11 10:42:27.026611 wagtail-localize-1.5.1/wagtail_localize/locale/en/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0       98 2023-06-11 10:35:07.229277 wagtail-localize-1.5.1/wagtail_localize/locale/en/LC_MESSAGES/djangojs.mo
+-rw-r--r--   0        0        0     6466 2023-06-11 10:42:27.026908 wagtail-localize-1.5.1/wagtail_localize/locale/en/LC_MESSAGES/djangojs.po
+-rw-r--r--   0        0        0     8831 2023-06-11 10:42:27.027054 wagtail-localize-1.5.1/wagtail_localize/locale/es/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0     9558 2023-06-11 10:42:27.027155 wagtail-localize-1.5.1/wagtail_localize/locale/es/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     3155 2023-06-11 10:42:27.027359 wagtail-localize-1.5.1/wagtail_localize/locale/es/LC_MESSAGES/djangojs.mo
+-rw-r--r--   0        0        0     3108 2023-06-11 10:42:27.027501 wagtail-localize-1.5.1/wagtail_localize/locale/es/LC_MESSAGES/djangojs.po
+-rw-r--r--   0        0        0      659 2023-06-11 10:42:27.027634 wagtail-localize-1.5.1/wagtail_localize/locale/et/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0      764 2023-06-11 10:42:27.027720 wagtail-localize-1.5.1/wagtail_localize/locale/et/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     1078 2023-06-11 10:42:27.027813 wagtail-localize-1.5.1/wagtail_localize/locale/et/LC_MESSAGES/djangojs.mo
+-rw-r--r--   0        0        0     1044 2023-06-11 10:42:27.027909 wagtail-localize-1.5.1/wagtail_localize/locale/et/LC_MESSAGES/djangojs.po
+-rw-r--r--   0        0        0      425 2023-06-11 10:42:27.028006 wagtail-localize-1.5.1/wagtail_localize/locale/eu/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0      563 2023-06-11 10:42:27.028115 wagtail-localize-1.5.1/wagtail_localize/locale/eu/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0      518 2023-06-11 10:42:27.028216 wagtail-localize-1.5.1/wagtail_localize/locale/eu/LC_MESSAGES/djangojs.mo
+-rw-r--r--   0        0        0      603 2023-06-11 10:42:27.028298 wagtail-localize-1.5.1/wagtail_localize/locale/eu/LC_MESSAGES/djangojs.po
+-rw-r--r--   0        0        0      707 2023-06-11 10:42:27.028429 wagtail-localize-1.5.1/wagtail_localize/locale/fa/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0      888 2023-06-11 10:42:27.028511 wagtail-localize-1.5.1/wagtail_localize/locale/fa/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     1509 2023-06-11 10:42:27.028609 wagtail-localize-1.5.1/wagtail_localize/locale/fa/LC_MESSAGES/djangojs.mo
+-rw-r--r--   0        0        0     1628 2023-06-11 10:42:27.028706 wagtail-localize-1.5.1/wagtail_localize/locale/fa/LC_MESSAGES/djangojs.po
+-rw-r--r--   0        0        0     2793 2023-06-11 10:42:27.028828 wagtail-localize-1.5.1/wagtail_localize/locale/fi/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0     2952 2023-06-11 10:42:27.028915 wagtail-localize-1.5.1/wagtail_localize/locale/fi/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     2646 2023-06-11 10:42:27.029034 wagtail-localize-1.5.1/wagtail_localize/locale/fi/LC_MESSAGES/djangojs.mo
+-rw-r--r--   0        0        0     2617 2023-06-11 10:42:27.029137 wagtail-localize-1.5.1/wagtail_localize/locale/fi/LC_MESSAGES/djangojs.po
+-rw-r--r--   0        0        0     9166 2023-06-11 10:42:27.029253 wagtail-localize-1.5.1/wagtail_localize/locale/fr/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0     9733 2023-06-11 10:42:27.029341 wagtail-localize-1.5.1/wagtail_localize/locale/fr/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     3318 2023-06-11 10:42:27.029425 wagtail-localize-1.5.1/wagtail_localize/locale/fr/LC_MESSAGES/djangojs.mo
+-rw-r--r--   0        0        0     3213 2023-06-11 10:42:27.029506 wagtail-localize-1.5.1/wagtail_localize/locale/fr/LC_MESSAGES/djangojs.po
+-rw-r--r--   0        0        0     8579 2023-06-11 10:42:27.029635 wagtail-localize-1.5.1/wagtail_localize/locale/gl/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0     9139 2023-06-11 10:42:27.029723 wagtail-localize-1.5.1/wagtail_localize/locale/gl/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     3105 2023-06-11 10:42:27.029831 wagtail-localize-1.5.1/wagtail_localize/locale/gl/LC_MESSAGES/djangojs.mo
+-rw-r--r--   0        0        0     3024 2023-06-11 10:42:27.030083 wagtail-localize-1.5.1/wagtail_localize/locale/gl/LC_MESSAGES/djangojs.po
+-rw-r--r--   0        0        0      685 2023-06-11 10:42:27.030254 wagtail-localize-1.5.1/wagtail_localize/locale/he_IL/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0      880 2023-06-11 10:42:27.030365 wagtail-localize-1.5.1/wagtail_localize/locale/he_IL/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     1008 2023-06-11 10:42:27.030467 wagtail-localize-1.5.1/wagtail_localize/locale/he_IL/LC_MESSAGES/djangojs.mo
+-rw-r--r--   0        0        0     1092 2023-06-11 10:42:27.030561 wagtail-localize-1.5.1/wagtail_localize/locale/he_IL/LC_MESSAGES/djangojs.po
+-rw-r--r--   0        0        0     1296 2023-06-11 10:42:27.030676 wagtail-localize-1.5.1/wagtail_localize/locale/hr_HR/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0     1373 2023-06-11 10:42:27.030768 wagtail-localize-1.5.1/wagtail_localize/locale/hr_HR/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     1164 2023-06-11 10:42:27.030867 wagtail-localize-1.5.1/wagtail_localize/locale/hr_HR/LC_MESSAGES/djangojs.mo
+-rw-r--r--   0        0        0     1194 2023-06-11 10:42:27.030969 wagtail-localize-1.5.1/wagtail_localize/locale/hr_HR/LC_MESSAGES/djangojs.po
+-rw-r--r--   0        0        0      410 2023-06-11 10:42:27.031085 wagtail-localize-1.5.1/wagtail_localize/locale/ht/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0      501 2023-06-11 10:42:27.031174 wagtail-localize-1.5.1/wagtail_localize/locale/ht/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0      373 2023-06-11 10:42:27.031273 wagtail-localize-1.5.1/wagtail_localize/locale/ht/LC_MESSAGES/djangojs.mo
+-rw-r--r--   0        0        0      415 2023-06-11 10:42:27.031372 wagtail-localize-1.5.1/wagtail_localize/locale/ht/LC_MESSAGES/djangojs.po
+-rw-r--r--   0        0        0     8902 2023-06-11 10:42:27.031512 wagtail-localize-1.5.1/wagtail_localize/locale/hu/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0     9464 2023-06-11 10:42:27.031615 wagtail-localize-1.5.1/wagtail_localize/locale/hu/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     3220 2023-06-11 10:42:27.031714 wagtail-localize-1.5.1/wagtail_localize/locale/hu/LC_MESSAGES/djangojs.mo
+-rw-r--r--   0        0        0     3113 2023-06-11 10:42:27.031828 wagtail-localize-1.5.1/wagtail_localize/locale/hu/LC_MESSAGES/djangojs.po
+-rw-r--r--   0        0        0      561 2023-06-11 10:42:27.031950 wagtail-localize-1.5.1/wagtail_localize/locale/id_ID/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0      737 2023-06-11 10:42:27.032039 wagtail-localize-1.5.1/wagtail_localize/locale/id_ID/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     1150 2023-06-11 10:42:27.032141 wagtail-localize-1.5.1/wagtail_localize/locale/id_ID/LC_MESSAGES/djangojs.mo
+-rw-r--r--   0        0        0     1331 2023-06-11 10:42:27.032241 wagtail-localize-1.5.1/wagtail_localize/locale/id_ID/LC_MESSAGES/djangojs.po
+-rw-r--r--   0        0        0     8645 2023-06-11 10:42:27.032366 wagtail-localize-1.5.1/wagtail_localize/locale/is_IS/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0     9153 2023-06-11 10:42:27.032466 wagtail-localize-1.5.1/wagtail_localize/locale/is_IS/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     3082 2023-06-11 10:42:27.032572 wagtail-localize-1.5.1/wagtail_localize/locale/is_IS/LC_MESSAGES/djangojs.mo
+-rw-r--r--   0        0        0     3018 2023-06-11 10:42:27.032674 wagtail-localize-1.5.1/wagtail_localize/locale/is_IS/LC_MESSAGES/djangojs.po
+-rw-r--r--   0        0        0     8269 2023-06-11 10:42:27.032819 wagtail-localize-1.5.1/wagtail_localize/locale/it/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0     8773 2023-06-11 10:42:27.032908 wagtail-localize-1.5.1/wagtail_localize/locale/it/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     3171 2023-06-11 10:42:27.033012 wagtail-localize-1.5.1/wagtail_localize/locale/it/LC_MESSAGES/djangojs.mo
+-rw-r--r--   0        0        0     3255 2023-06-11 10:42:27.033105 wagtail-localize-1.5.1/wagtail_localize/locale/it/LC_MESSAGES/djangojs.po
+-rw-r--r--   0        0        0      741 2023-06-11 10:42:27.033212 wagtail-localize-1.5.1/wagtail_localize/locale/ja/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0      925 2023-06-11 10:42:27.033308 wagtail-localize-1.5.1/wagtail_localize/locale/ja/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     1259 2023-06-11 10:42:27.033410 wagtail-localize-1.5.1/wagtail_localize/locale/ja/LC_MESSAGES/djangojs.mo
+-rw-r--r--   0        0        0     1448 2023-06-11 10:42:27.033508 wagtail-localize-1.5.1/wagtail_localize/locale/ja/LC_MESSAGES/djangojs.po
+-rw-r--r--   0        0        0      499 2023-06-11 10:42:27.033623 wagtail-localize-1.5.1/wagtail_localize/locale/ka/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0      581 2023-06-11 10:42:27.033756 wagtail-localize-1.5.1/wagtail_localize/locale/ka/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0      767 2023-06-11 10:42:27.033881 wagtail-localize-1.5.1/wagtail_localize/locale/ka/LC_MESSAGES/djangojs.mo
+-rw-r--r--   0        0        0      788 2023-06-11 10:42:27.033976 wagtail-localize-1.5.1/wagtail_localize/locale/ka/LC_MESSAGES/djangojs.po
+-rw-r--r--   0        0        0     1302 2023-06-11 10:42:27.034074 wagtail-localize-1.5.1/wagtail_localize/locale/ko/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0     1452 2023-06-11 10:42:27.034152 wagtail-localize-1.5.1/wagtail_localize/locale/ko/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     1248 2023-06-11 10:42:27.034242 wagtail-localize-1.5.1/wagtail_localize/locale/ko/LC_MESSAGES/djangojs.mo
+-rw-r--r--   0        0        0     1289 2023-06-11 10:42:27.034329 wagtail-localize-1.5.1/wagtail_localize/locale/ko/LC_MESSAGES/djangojs.po
+-rw-r--r--   0        0        0     5586 2023-06-11 10:42:27.034456 wagtail-localize-1.5.1/wagtail_localize/locale/lt/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0     5943 2023-06-11 10:42:27.034568 wagtail-localize-1.5.1/wagtail_localize/locale/lt/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     2690 2023-06-11 10:42:27.034702 wagtail-localize-1.5.1/wagtail_localize/locale/lt/LC_MESSAGES/djangojs.mo
+-rw-r--r--   0        0        0     2643 2023-06-11 10:42:27.034801 wagtail-localize-1.5.1/wagtail_localize/locale/lt/LC_MESSAGES/djangojs.po
+-rw-r--r--   0        0        0      637 2023-06-11 10:42:27.034922 wagtail-localize-1.5.1/wagtail_localize/locale/lv/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0      765 2023-06-11 10:42:27.035018 wagtail-localize-1.5.1/wagtail_localize/locale/lv/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     1162 2023-06-11 10:42:27.035129 wagtail-localize-1.5.1/wagtail_localize/locale/lv/LC_MESSAGES/djangojs.mo
+-rw-r--r--   0        0        0     1189 2023-06-11 10:42:27.035240 wagtail-localize-1.5.1/wagtail_localize/locale/lv/LC_MESSAGES/djangojs.po
+-rw-r--r--   0        0        0     1016 2023-06-11 10:42:27.035363 wagtail-localize-1.5.1/wagtail_localize/locale/mi/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0     1112 2023-06-11 10:42:27.035454 wagtail-localize-1.5.1/wagtail_localize/locale/mi/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0      985 2023-06-11 10:42:27.035559 wagtail-localize-1.5.1/wagtail_localize/locale/mi/LC_MESSAGES/djangojs.mo
+-rw-r--r--   0        0        0      975 2023-06-11 10:42:27.035662 wagtail-localize-1.5.1/wagtail_localize/locale/mi/LC_MESSAGES/djangojs.po
+-rw-r--r--   0        0        0      786 2023-06-11 10:42:27.035769 wagtail-localize-1.5.1/wagtail_localize/locale/mn/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0      871 2023-06-11 10:42:27.035866 wagtail-localize-1.5.1/wagtail_localize/locale/mn/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     1100 2023-06-11 10:42:27.035976 wagtail-localize-1.5.1/wagtail_localize/locale/mn/LC_MESSAGES/djangojs.mo
+-rw-r--r--   0        0        0     1176 2023-06-11 10:42:27.036067 wagtail-localize-1.5.1/wagtail_localize/locale/mn/LC_MESSAGES/djangojs.po
+-rw-r--r--   0        0        0      628 2023-06-11 10:42:27.036176 wagtail-localize-1.5.1/wagtail_localize/locale/my/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0      704 2023-06-11 10:42:27.036274 wagtail-localize-1.5.1/wagtail_localize/locale/my/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0      455 2023-06-11 10:42:27.036385 wagtail-localize-1.5.1/wagtail_localize/locale/my/LC_MESSAGES/djangojs.mo
+-rw-r--r--   0        0        0      502 2023-06-11 10:42:27.036485 wagtail-localize-1.5.1/wagtail_localize/locale/my/LC_MESSAGES/djangojs.po
+-rw-r--r--   0        0        0      653 2023-06-11 10:42:27.036597 wagtail-localize-1.5.1/wagtail_localize/locale/nb/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0      821 2023-06-11 10:42:27.036681 wagtail-localize-1.5.1/wagtail_localize/locale/nb/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     1216 2023-06-11 10:42:27.036776 wagtail-localize-1.5.1/wagtail_localize/locale/nb/LC_MESSAGES/djangojs.mo
+-rw-r--r--   0        0        0     1355 2023-06-11 10:42:27.036872 wagtail-localize-1.5.1/wagtail_localize/locale/nb/LC_MESSAGES/djangojs.po
+-rw-r--r--   0        0        0     8728 2023-06-11 10:42:27.037032 wagtail-localize-1.5.1/wagtail_localize/locale/nl/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0     9421 2023-06-11 10:42:27.037135 wagtail-localize-1.5.1/wagtail_localize/locale/nl/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     3124 2023-06-11 10:42:27.037254 wagtail-localize-1.5.1/wagtail_localize/locale/nl/LC_MESSAGES/djangojs.mo
+-rw-r--r--   0        0        0     3176 2023-06-11 10:42:27.037404 wagtail-localize-1.5.1/wagtail_localize/locale/nl/LC_MESSAGES/djangojs.po
+-rw-r--r--   0        0        0     5303 2022-07-01 10:57:34.469976 wagtail-localize-1.5.1/wagtail_localize/locale/nl_NL/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0     2838 2022-07-01 10:57:34.470220 wagtail-localize-1.5.1/wagtail_localize/locale/nl_NL/LC_MESSAGES/djangojs.mo
+-rw-r--r--   0        0        0     6320 2023-06-11 10:42:27.037548 wagtail-localize-1.5.1/wagtail_localize/locale/pl/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0     6613 2023-06-11 10:42:27.037645 wagtail-localize-1.5.1/wagtail_localize/locale/pl/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     3092 2023-06-11 10:42:27.037757 wagtail-localize-1.5.1/wagtail_localize/locale/pl/LC_MESSAGES/djangojs.mo
+-rw-r--r--   0        0        0     3024 2023-06-11 10:42:27.037875 wagtail-localize-1.5.1/wagtail_localize/locale/pl/LC_MESSAGES/djangojs.po
+-rw-r--r--   0        0        0     8197 2023-06-11 10:42:27.038084 wagtail-localize-1.5.1/wagtail_localize/locale/pt_BR/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0     8935 2023-06-11 10:42:27.038245 wagtail-localize-1.5.1/wagtail_localize/locale/pt_BR/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     3192 2023-06-11 10:42:27.038356 wagtail-localize-1.5.1/wagtail_localize/locale/pt_BR/LC_MESSAGES/djangojs.mo
+-rw-r--r--   0        0        0     3191 2023-06-11 10:42:27.038463 wagtail-localize-1.5.1/wagtail_localize/locale/pt_BR/LC_MESSAGES/djangojs.po
+-rw-r--r--   0        0        0     8678 2023-06-11 10:42:27.038619 wagtail-localize-1.5.1/wagtail_localize/locale/pt_PT/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0     9281 2023-06-11 10:42:27.038748 wagtail-localize-1.5.1/wagtail_localize/locale/pt_PT/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     3166 2023-06-11 10:42:27.038977 wagtail-localize-1.5.1/wagtail_localize/locale/pt_PT/LC_MESSAGES/djangojs.mo
+-rw-r--r--   0        0        0     3102 2023-06-11 10:42:27.039108 wagtail-localize-1.5.1/wagtail_localize/locale/pt_PT/LC_MESSAGES/djangojs.po
+-rw-r--r--   0        0        0     8676 2023-06-11 10:42:27.039392 wagtail-localize-1.5.1/wagtail_localize/locale/ro/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0     9151 2023-06-11 10:42:27.039614 wagtail-localize-1.5.1/wagtail_localize/locale/ro/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     3152 2023-06-11 10:42:27.039734 wagtail-localize-1.5.1/wagtail_localize/locale/ro/LC_MESSAGES/djangojs.mo
+-rw-r--r--   0        0        0     3011 2023-06-11 10:42:27.039845 wagtail-localize-1.5.1/wagtail_localize/locale/ro/LC_MESSAGES/djangojs.po
+-rw-r--r--   0        0        0    10730 2023-06-11 10:42:27.039994 wagtail-localize-1.5.1/wagtail_localize/locale/ru/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0    11422 2023-06-11 10:42:27.040110 wagtail-localize-1.5.1/wagtail_localize/locale/ru/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     4192 2023-06-11 10:42:27.040278 wagtail-localize-1.5.1/wagtail_localize/locale/ru/LC_MESSAGES/djangojs.mo
+-rw-r--r--   0        0        0     4183 2023-06-11 10:42:27.040409 wagtail-localize-1.5.1/wagtail_localize/locale/ru/LC_MESSAGES/djangojs.po
+-rw-r--r--   0        0        0      674 2023-06-11 10:42:27.040532 wagtail-localize-1.5.1/wagtail_localize/locale/sk_SK/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0      828 2023-06-11 10:42:27.040625 wagtail-localize-1.5.1/wagtail_localize/locale/sk_SK/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     1096 2023-06-11 10:42:27.040732 wagtail-localize-1.5.1/wagtail_localize/locale/sk_SK/LC_MESSAGES/djangojs.mo
+-rw-r--r--   0        0        0     1132 2023-06-11 10:42:27.040843 wagtail-localize-1.5.1/wagtail_localize/locale/sk_SK/LC_MESSAGES/djangojs.po
+-rw-r--r--   0        0        0     7117 2023-06-11 10:42:27.040992 wagtail-localize-1.5.1/wagtail_localize/locale/sl/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0     7542 2023-06-11 10:42:27.041129 wagtail-localize-1.5.1/wagtail_localize/locale/sl/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     3078 2023-06-11 10:42:27.041240 wagtail-localize-1.5.1/wagtail_localize/locale/sl/LC_MESSAGES/djangojs.mo
+-rw-r--r--   0        0        0     3004 2023-06-11 10:42:27.041362 wagtail-localize-1.5.1/wagtail_localize/locale/sl/LC_MESSAGES/djangojs.po
+-rw-r--r--   0        0        0      434 2023-06-11 10:42:27.041474 wagtail-localize-1.5.1/wagtail_localize/locale/sr/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0      527 2023-06-11 10:42:27.041574 wagtail-localize-1.5.1/wagtail_localize/locale/sr/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     8613 2023-06-11 10:42:27.041743 wagtail-localize-1.5.1/wagtail_localize/locale/sv/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0     9230 2023-06-11 10:42:27.041848 wagtail-localize-1.5.1/wagtail_localize/locale/sv/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     3031 2023-06-11 10:42:27.041960 wagtail-localize-1.5.1/wagtail_localize/locale/sv/LC_MESSAGES/djangojs.mo
+-rw-r--r--   0        0        0     3015 2023-06-11 10:42:27.042073 wagtail-localize-1.5.1/wagtail_localize/locale/sv/LC_MESSAGES/djangojs.po
+-rw-r--r--   0        0        0      433 2023-06-11 10:42:27.042178 wagtail-localize-1.5.1/wagtail_localize/locale/ta/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0      515 2023-06-11 10:42:27.042274 wagtail-localize-1.5.1/wagtail_localize/locale/ta/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0      343 2023-06-11 10:42:27.042363 wagtail-localize-1.5.1/wagtail_localize/locale/ta/LC_MESSAGES/djangojs.mo
+-rw-r--r--   0        0        0      374 2023-06-11 10:42:27.042466 wagtail-localize-1.5.1/wagtail_localize/locale/ta/LC_MESSAGES/djangojs.po
+-rw-r--r--   0        0        0      550 2023-06-11 10:42:27.042576 wagtail-localize-1.5.1/wagtail_localize/locale/tet/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0      717 2023-06-11 10:42:27.042668 wagtail-localize-1.5.1/wagtail_localize/locale/tet/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0      880 2023-06-11 10:42:27.042768 wagtail-localize-1.5.1/wagtail_localize/locale/tet/LC_MESSAGES/djangojs.mo
+-rw-r--r--   0        0        0     1031 2023-06-11 10:42:27.042871 wagtail-localize-1.5.1/wagtail_localize/locale/tet/LC_MESSAGES/djangojs.po
+-rw-r--r--   0        0        0      810 2023-06-11 10:42:27.042996 wagtail-localize-1.5.1/wagtail_localize/locale/th/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0      934 2023-06-11 10:42:27.043092 wagtail-localize-1.5.1/wagtail_localize/locale/th/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     1218 2023-06-11 10:42:27.043196 wagtail-localize-1.5.1/wagtail_localize/locale/th/LC_MESSAGES/djangojs.mo
+-rw-r--r--   0        0        0     1261 2023-06-11 10:42:27.043296 wagtail-localize-1.5.1/wagtail_localize/locale/th/LC_MESSAGES/djangojs.po
+-rw-r--r--   0        0        0      583 2023-06-11 10:42:27.043418 wagtail-localize-1.5.1/wagtail_localize/locale/tr/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0      801 2023-06-11 10:42:27.043506 wagtail-localize-1.5.1/wagtail_localize/locale/tr/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     1149 2023-06-11 10:42:27.043607 wagtail-localize-1.5.1/wagtail_localize/locale/tr/LC_MESSAGES/djangojs.mo
+-rw-r--r--   0        0        0     1293 2023-06-11 10:42:27.043710 wagtail-localize-1.5.1/wagtail_localize/locale/tr/LC_MESSAGES/djangojs.po
+-rw-r--r--   0        0        0      649 2023-06-11 10:42:27.043812 wagtail-localize-1.5.1/wagtail_localize/locale/tr_TR/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0      854 2023-06-11 10:42:27.043907 wagtail-localize-1.5.1/wagtail_localize/locale/tr_TR/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     1108 2023-06-11 10:42:27.044016 wagtail-localize-1.5.1/wagtail_localize/locale/tr_TR/LC_MESSAGES/djangojs.mo
+-rw-r--r--   0        0        0     1218 2023-06-11 10:42:27.044119 wagtail-localize-1.5.1/wagtail_localize/locale/tr_TR/LC_MESSAGES/djangojs.po
+-rw-r--r--   0        0        0     9314 2023-06-11 10:42:27.044276 wagtail-localize-1.5.1/wagtail_localize/locale/uk/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0     9899 2023-06-11 10:42:27.044366 wagtail-localize-1.5.1/wagtail_localize/locale/uk/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     3990 2023-06-11 10:42:27.044474 wagtail-localize-1.5.1/wagtail_localize/locale/uk/LC_MESSAGES/djangojs.mo
+-rw-r--r--   0        0        0     4175 2023-06-11 10:42:27.044581 wagtail-localize-1.5.1/wagtail_localize/locale/uk/LC_MESSAGES/djangojs.po
+-rw-r--r--   0        0        0      667 2023-06-11 10:42:27.044705 wagtail-localize-1.5.1/wagtail_localize/locale/vi/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0      852 2023-06-11 10:42:27.044813 wagtail-localize-1.5.1/wagtail_localize/locale/vi/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     1424 2023-06-11 10:42:27.044930 wagtail-localize-1.5.1/wagtail_localize/locale/vi/LC_MESSAGES/djangojs.mo
+-rw-r--r--   0        0        0     1450 2023-06-11 10:42:27.045033 wagtail-localize-1.5.1/wagtail_localize/locale/vi/LC_MESSAGES/djangojs.po
+-rw-r--r--   0        0        0      495 2023-06-11 10:42:27.045154 wagtail-localize-1.5.1/wagtail_localize/locale/zh/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0      691 2023-06-11 10:42:27.045238 wagtail-localize-1.5.1/wagtail_localize/locale/zh/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0      736 2023-06-11 10:42:27.045332 wagtail-localize-1.5.1/wagtail_localize/locale/zh/LC_MESSAGES/djangojs.mo
+-rw-r--r--   0        0        0      907 2023-06-11 10:42:27.045437 wagtail-localize-1.5.1/wagtail_localize/locale/zh/LC_MESSAGES/djangojs.po
+-rw-r--r--   0        0        0     7010 2023-06-11 10:42:27.045605 wagtail-localize-1.5.1/wagtail_localize/locale/zh_Hans/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0     7554 2023-06-11 10:42:27.045713 wagtail-localize-1.5.1/wagtail_localize/locale/zh_Hans/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     2916 2023-06-11 10:42:27.045839 wagtail-localize-1.5.1/wagtail_localize/locale/zh_Hans/LC_MESSAGES/djangojs.mo
+-rw-r--r--   0        0        0     2952 2023-06-11 10:42:27.046049 wagtail-localize-1.5.1/wagtail_localize/locale/zh_Hans/LC_MESSAGES/djangojs.po
+-rw-r--r--   0        0        0      793 2023-06-11 10:42:27.046156 wagtail-localize-1.5.1/wagtail_localize/locale/zh_Hant/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0      890 2023-06-11 10:42:27.046242 wagtail-localize-1.5.1/wagtail_localize/locale/zh_Hant/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     1114 2023-06-11 10:42:27.046353 wagtail-localize-1.5.1/wagtail_localize/locale/zh_Hant/LC_MESSAGES/djangojs.mo
+-rw-r--r--   0        0        0     1184 2023-06-11 10:42:27.046449 wagtail-localize-1.5.1/wagtail_localize/locale/zh_Hant/LC_MESSAGES/djangojs.po
+-rw-r--r--   0        0        0        0 2022-09-23 10:15:38.922735 wagtail-localize-1.5.1/wagtail_localize/locales/__init__.py
+-rw-r--r--   0        0        0      267 2022-07-01 10:57:34.513956 wagtail-localize-1.5.1/wagtail_localize/locales/apps.py
+-rw-r--r--   0        0        0      917 2022-07-01 10:57:34.515898 wagtail-localize-1.5.1/wagtail_localize/locales/components.py
+-rw-r--r--   0        0        0     1315 2023-02-15 19:30:42.626580 wagtail-localize-1.5.1/wagtail_localize/locales/forms.py
+-rw-r--r--   0        0        0      337 2023-06-11 10:35:07.029616 wagtail-localize-1.5.1/wagtail_localize/locales/locale/en/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0     2436 2023-06-11 10:42:27.046673 wagtail-localize-1.5.1/wagtail_localize/locales/locale/en/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0      710 2022-07-01 10:57:34.510343 wagtail-localize-1.5.1/wagtail_localize/locales/locale/es/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0     1979 2022-07-01 10:57:34.509539 wagtail-localize-1.5.1/wagtail_localize/locales/locale/fi/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0     1981 2022-07-01 10:57:34.509928 wagtail-localize-1.5.1/wagtail_localize/locales/locale/fr/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0     2023 2022-07-01 10:57:34.507986 wagtail-localize-1.5.1/wagtail_localize/locales/locale/hr_HR/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0     2053 2022-07-01 10:57:34.509174 wagtail-localize-1.5.1/wagtail_localize/locales/locale/is_IS/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0     2010 2022-07-01 10:57:34.508810 wagtail-localize-1.5.1/wagtail_localize/locales/locale/nl_NL/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0     1986 2022-07-01 10:57:34.506765 wagtail-localize-1.5.1/wagtail_localize/locales/locale/pt_PT/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0     2453 2022-07-01 10:57:34.507498 wagtail-localize-1.5.1/wagtail_localize/locales/locale/ru/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0     2026 2022-07-01 10:57:34.506256 wagtail-localize-1.5.1/wagtail_localize/locales/locale/sv/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0     1927 2022-07-01 10:57:34.507136 wagtail-localize-1.5.1/wagtail_localize/locales/locale/zh_Hans/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0      559 2022-07-01 10:57:34.508337 wagtail-localize-1.5.1/wagtail_localize/locales/locale/zh_Hant/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0      917 2022-07-01 10:57:34.515715 wagtail-localize-1.5.1/wagtail_localize/locales/templates/wagtaillocales/confirm_delete.html
+-rw-r--r--   0        0        0      207 2022-07-01 10:57:34.515314 wagtail-localize-1.5.1/wagtail_localize/locales/templates/wagtaillocales/create.html
+-rw-r--r--   0        0        0     2762 2022-07-01 10:57:34.515505 wagtail-localize-1.5.1/wagtail_localize/locales/templates/wagtaillocales/edit.html
+-rw-r--r--   0        0        0     2148 2022-07-01 10:57:34.515123 wagtail-localize-1.5.1/wagtail_localize/locales/templates/wagtaillocales/index.html
+-rw-r--r--   0        0        0    13996 2023-02-15 19:30:42.626693 wagtail-localize-1.5.1/wagtail_localize/locales/tests.py
+-rw-r--r--   0        0        0      462 2023-02-15 19:30:42.626782 wagtail-localize-1.5.1/wagtail_localize/locales/utils.py
+-rw-r--r--   0        0        0     6843 2023-06-02 22:09:08.221571 wagtail-localize-1.5.1/wagtail_localize/locales/views.py
+-rw-r--r--   0        0        0     1052 2023-02-15 19:30:42.626987 wagtail-localize-1.5.1/wagtail_localize/locales/wagtail_hooks.py
+-rw-r--r--   0        0        0      385 2022-07-01 10:57:34.538728 wagtail-localize-1.5.1/wagtail_localize/machine_translators/__init__.py
+-rw-r--r--   0        0        0      303 2022-09-12 13:15:14.646119 wagtail-localize-1.5.1/wagtail_localize/machine_translators/base.py
+-rw-r--r--   0        0        0     1538 2022-09-12 13:15:14.646264 wagtail-localize-1.5.1/wagtail_localize/machine_translators/deepl.py
+-rw-r--r--   0        0        0     1508 2022-07-01 10:57:34.540336 wagtail-localize-1.5.1/wagtail_localize/machine_translators/dummy.py
+-rw-r--r--   0        0        0     1957 2023-01-22 13:17:54.447370 wagtail-localize-1.5.1/wagtail_localize/machine_translators/google.py
+-rw-r--r--   0        0        0        0 2022-07-01 10:57:34.540801 wagtail-localize-1.5.1/wagtail_localize/management/__init__.py
+-rw-r--r--   0        0        0        0 2022-07-01 10:57:34.541279 wagtail-localize-1.5.1/wagtail_localize/management/commands/__init__.py
+-rw-r--r--   0        0        0      550 2022-07-01 10:57:34.541517 wagtail-localize-1.5.1/wagtail_localize/management/commands/sync_locale_trees.py
+-rw-r--r--   0        0        0    14672 2022-11-04 12:29:12.963230 wagtail-localize-1.5.1/wagtail_localize/migrations/0001_initial.py
+-rw-r--r--   0        0        0     2247 2022-07-01 10:57:34.432921 wagtail-localize-1.5.1/wagtail_localize/migrations/0002_translation.py
+-rw-r--r--   0        0        0     1028 2022-07-01 10:57:34.427359 wagtail-localize-1.5.1/wagtail_localize/migrations/0003_delete_translation_sources.py
+-rw-r--r--   0        0        0      860 2022-07-01 10:57:34.431933 wagtail-localize-1.5.1/wagtail_localize/migrations/0004_one_source_per_objectlocale.py
+-rw-r--r--   0        0        0      553 2022-07-01 10:57:34.432415 wagtail-localize-1.5.1/wagtail_localize/migrations/0005_remove_translationsource_object.py
+-rw-r--r--   0        0        0     1791 2022-07-01 10:57:34.432577 wagtail-localize-1.5.1/wagtail_localize/migrations/0006_create_submit_translation_permission.py
+-rw-r--r--   0        0        0      783 2022-07-01 10:57:34.427737 wagtail-localize-1.5.1/wagtail_localize/migrations/0007_stringtranslation_type_and_tool_name.py
+-rw-r--r--   0        0        0      764 2022-07-01 10:57:34.432114 wagtail-localize-1.5.1/wagtail_localize/migrations/0008_stringtranslation_last_translated_by.py
+-rw-r--r--   0        0        0      592 2022-07-01 10:57:34.432267 wagtail-localize-1.5.1/wagtail_localize/migrations/0009_stringtranslation_errors.py
+-rw-r--r--   0        0        0     1399 2022-07-01 10:57:34.427501 wagtail-localize-1.5.1/wagtail_localize/migrations/0010_overridablesegment.py
+-rw-r--r--   0        0        0     2226 2022-07-01 10:57:34.431151 wagtail-localize-1.5.1/wagtail_localize/migrations/0011_segmentoverride.py
+-rw-r--r--   0        0        0     1329 2022-07-01 10:57:34.431708 wagtail-localize-1.5.1/wagtail_localize/migrations/0012_localesynchronization.py
+-rw-r--r--   0        0        0      428 2022-07-01 10:57:34.432763 wagtail-localize-1.5.1/wagtail_localize/migrations/0013_translationsource_schema_version.py
+-rw-r--r--   0        0        0      372 2022-07-01 10:57:34.427137 wagtail-localize-1.5.1/wagtail_localize/migrations/0014_remove_translation_source_last_updated_at.py
+-rw-r--r--   0        0        0      465 2022-07-01 10:57:34.431395 wagtail-localize-1.5.1/wagtail_localize/migrations/0015_translationcontext_field_path.py
+-rw-r--r--   0        0        0        0 2022-07-01 10:57:34.427580 wagtail-localize-1.5.1/wagtail_localize/migrations/__init__.py
+-rw-r--r--   0        0        0        0 2022-09-23 10:15:38.922854 wagtail-localize-1.5.1/wagtail_localize/modeladmin/__init__.py
+-rw-r--r--   0        0        0      221 2022-07-01 10:57:34.554873 wagtail-localize-1.5.1/wagtail_localize/modeladmin/apps.py
+-rw-r--r--   0        0        0     3138 2023-02-15 19:30:42.627204 wagtail-localize-1.5.1/wagtail_localize/modeladmin/helpers.py
+-rw-r--r--   0        0        0     2223 2023-02-15 19:31:51.787872 wagtail-localize-1.5.1/wagtail_localize/modeladmin/options.py
+-rw-r--r--   0        0        0      313 2022-07-01 10:57:34.555903 wagtail-localize-1.5.1/wagtail_localize/modeladmin/templates/wagtail_localize/modeladmin/includes/button.html
+-rw-r--r--   0        0        0      162 2022-07-01 10:57:34.556094 wagtail-localize-1.5.1/wagtail_localize/modeladmin/templates/wagtail_localize/modeladmin/includes/header_with_breadcrumb.html
+-rw-r--r--   0        0        0       46 2022-07-01 10:57:34.557049 wagtail-localize-1.5.1/wagtail_localize/modeladmin/templates/wagtail_localize/modeladmin/translatable_choose_parent.html
+-rw-r--r--   0        0        0      309 2023-02-15 19:30:42.627410 wagtail-localize-1.5.1/wagtail_localize/modeladmin/templates/wagtail_localize/modeladmin/translatable_create.html
+-rw-r--r--   0        0        0       39 2022-07-01 10:57:34.556233 wagtail-localize-1.5.1/wagtail_localize/modeladmin/templates/wagtail_localize/modeladmin/translatable_delete.html
+-rw-r--r--   0        0        0     1347 2023-06-02 22:09:08.221764 wagtail-localize-1.5.1/wagtail_localize/modeladmin/templates/wagtail_localize/modeladmin/translatable_edit.html
+-rw-r--r--   0        0        0       40 2022-07-01 10:57:34.556386 wagtail-localize-1.5.1/wagtail_localize/modeladmin/templates/wagtail_localize/modeladmin/translatable_history.html
+-rw-r--r--   0        0        0     1065 2022-07-01 10:57:34.556547 wagtail-localize-1.5.1/wagtail_localize/modeladmin/templates/wagtail_localize/modeladmin/translatable_index.html
+-rw-r--r--   0        0        0      245 2022-08-31 18:34:50.710573 wagtail-localize-1.5.1/wagtail_localize/modeladmin/templates/wagtail_localize/modeladmin/translatable_inspect.html
+-rw-r--r--   0        0        0    27627 2023-02-15 19:30:42.627566 wagtail-localize-1.5.1/wagtail_localize/modeladmin/tests.py
+-rw-r--r--   0        0        0     7471 2023-02-15 19:30:42.627688 wagtail-localize-1.5.1/wagtail_localize/modeladmin/views.py
+-rw-r--r--   0        0        0      616 2023-02-15 19:30:42.627791 wagtail-localize-1.5.1/wagtail_localize/modeladmin/wagtail_hooks.py
+-rw-r--r--   0        0        0    85122 2023-02-15 19:30:42.628116 wagtail-localize-1.5.1/wagtail_localize/models.py
+-rw-r--r--   0        0        0     4620 2023-02-15 19:30:42.628255 wagtail-localize-1.5.1/wagtail_localize/operations.py
+-rw-r--r--   0        0        0      141 2022-07-01 10:57:34.570543 wagtail-localize-1.5.1/wagtail_localize/segments/__init__.py
+-rw-r--r--   0        0        0    13186 2023-02-15 19:30:42.628385 wagtail-localize-1.5.1/wagtail_localize/segments/extract.py
+-rw-r--r--   0        0        0    12641 2023-02-15 19:30:42.628513 wagtail-localize-1.5.1/wagtail_localize/segments/ingest.py
+-rw-r--r--   0        0        0    12328 2023-02-15 19:31:17.389809 wagtail-localize-1.5.1/wagtail_localize/segments/types.py
+-rw-r--r--   0        0        0     1847 2023-02-15 19:30:42.628953 wagtail-localize-1.5.1/wagtail_localize/side_panels.py
+-rw-r--r--   0        0        0      880 2023-06-11 10:43:03.594211 wagtail-localize-1.5.1/wagtail_localize/static/wagtail_localize/css/wagtail-localize-component-form.css
+-rw-r--r--   0        0        0     1501 2023-06-11 10:43:03.593997 wagtail-localize-1.5.1/wagtail_localize/static/wagtail_localize/js/wagtail-localize-component-form.js
+-rw-r--r--   0        0        0    86331 2023-06-11 10:43:03.595076 wagtail-localize-1.5.1/wagtail_localize/static/wagtail_localize/js/wagtail-localize.js
+-rw-r--r--   0        0        0    14658 2023-02-15 19:31:17.389857 wagtail-localize-1.5.1/wagtail_localize/strings.py
+-rw-r--r--   0        0        0     6973 2023-02-15 19:31:17.389902 wagtail-localize-1.5.1/wagtail_localize/synctree.py
+-rw-r--r--   0        0        0     1377 2022-07-01 10:57:34.504798 wagtail-localize-1.5.1/wagtail_localize/tasks.py
+-rw-r--r--   0        0        0     1273 2022-07-01 10:57:34.562536 wagtail-localize-1.5.1/wagtail_localize/templates/wagtail_localize/admin/_components.html
+-rw-r--r--   0        0        0     1349 2022-07-01 10:57:34.560800 wagtail-localize-1.5.1/wagtail_localize/templates/wagtail_localize/admin/confirm_convert_to_alias.html
+-rw-r--r--   0        0        0      893 2022-07-01 10:57:34.561400 wagtail-localize-1.5.1/wagtail_localize/templates/wagtail_localize/admin/edit_translatable_alias.html
+-rw-r--r--   0        0        0     2298 2023-02-15 19:30:42.629292 wagtail-localize-1.5.1/wagtail_localize/templates/wagtail_localize/admin/edit_translation.html
+-rw-r--r--   0        0        0      742 2022-09-13 08:26:04.349160 wagtail-localize-1.5.1/wagtail_localize/templates/wagtail_localize/admin/includes/generic_header.html
+-rw-r--r--   0        0        0     2462 2022-07-01 10:57:34.561084 wagtail-localize-1.5.1/wagtail_localize/templates/wagtail_localize/admin/submit_translation.html
+-rw-r--r--   0        0        0     1947 2022-07-01 10:57:34.562358 wagtail-localize-1.5.1/wagtail_localize/templates/wagtail_localize/admin/translations_report.html
+-rw-r--r--   0        0        0     4225 2023-02-15 19:30:42.629398 wagtail-localize-1.5.1/wagtail_localize/templates/wagtail_localize/admin/update_translations.html
+-rw-r--r--   0        0        0      501 2022-07-01 10:57:34.563064 wagtail-localize-1.5.1/wagtail_localize/templates/wagtail_localize/icons/wagtail-localize-convert.svg
+-rw-r--r--   0        0        0      918 2022-10-12 20:12:40.316546 wagtail-localize-1.5.1/wagtail_localize/templates/wagtail_localize/icons/wagtail-localize-language.svg
+-rw-r--r--   0        0        0        0 2022-07-01 10:57:34.425464 wagtail-localize-1.5.1/wagtail_localize/templatetags/__init__.py
+-rw-r--r--   0        0        0      324 2022-07-01 10:57:34.426417 wagtail-localize-1.5.1/wagtail_localize/templatetags/wagtail_localize_admin_tags.py
+-rw-r--r--   0        0        0     1232 2022-09-23 10:15:38.927745 wagtail-localize-1.5.1/wagtail_localize/version.py
+-rw-r--r--   0        0        0        0 2022-07-01 10:57:34.565383 wagtail-localize-1.5.1/wagtail_localize/views/__init__.py
+-rw-r--r--   0        0        0     6474 2023-02-15 19:30:42.632123 wagtail-localize-1.5.1/wagtail_localize/views/convert.py
+-rw-r--r--   0        0        0    52453 2023-02-15 19:31:17.390082 wagtail-localize-1.5.1/wagtail_localize/views/edit_translation.py
+-rw-r--r--   0        0        0     4250 2023-02-15 19:30:42.632454 wagtail-localize-1.5.1/wagtail_localize/views/report.py
+-rw-r--r--   0        0        0     1350 2023-02-15 19:30:42.632653 wagtail-localize-1.5.1/wagtail_localize/views/snippets_api.py
+-rw-r--r--   0        0        0     8968 2023-02-15 19:30:42.632802 wagtail-localize-1.5.1/wagtail_localize/views/submit_translations.py
+-rw-r--r--   0        0        0     6591 2023-02-15 19:30:42.632929 wagtail-localize-1.5.1/wagtail_localize/views/update_translations.py
+-rw-r--r--   0        0        0    15106 2023-06-02 22:09:08.224615 wagtail-localize-1.5.1/wagtail_localize/wagtail_hooks.py
+-rw-r--r--   0        0        0     6123 1970-01-01 00:00:00.000000 wagtail-localize-1.5.1/PKG-INFO
```

### Comparing `wagtail-localize-1.5/CHANGELOG.md` & `wagtail-localize-1.5.1/CHANGELOG.md`

 * *Files 2% similar despite different names*

```diff
@@ -3,14 +3,31 @@
 All notable changes to this project will be documented in this file.
 
 The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
 and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).
 
 ## [Unreleased]
 
+## [1.5.1] - 2023-06-11
+
+### Added
+
+- [Support for Django 4.2](https://github.com/wagtail/wagtail-localize/pull/692) @kmtracey
+- [Official Wagtail 5.0 support](https://github.com/wagtail/wagtail-localize/pull/699) @nickmoreton, @zerolab
+
+### Changed
+
+- [Updated prettier version and delegated linting to pre-commit](https://github.com/wagtail/wagtail-localize/pull/694) @PeteCoward
+- [Updated documentation dependencies and fix build errors](https://github.com/wagtail/wagtail-localize/pull/700) @zerolab
+- [Updated colour declarations for dark-mode compatibility](https://github.com/wagtail/wagtail-localize/pull/701) @spikennm, @zerolab
+
+### Removed
+
+- [Python 3.7, pre Wagtail 4.1 logic](https://github.com/wagtail/wagtail-localize/pull/699) @nickmoreton, @zerolab
+
 ## [1.5] - 2023-02-23
 
 ### Changed
 
 - [Updated tests to include Wagtail 4.2](https://github.com/wagtail/wagtail-localize/pull/673) @katdom13
 
 ### Removed
@@ -217,15 +234,16 @@
 - [Support for Wagtail 2.14](https://github.com/wagtail/wagtail-localize/pull/440)
 - [`overridable` keyword argument for `SynchronizedField`](https://github.com/wagtail/wagtail-localize/pull/438)
 
 ### Fixed
 
 - [Make sure field level validation runs when translating snippets](https://github.com/wagtail/wagtail-localize/pull/427)
 
-[unreleased]: https://github.com/wagtail/wagtail-localize/compare/v1.5...HEAD
+[unreleased]: https://github.com/wagtail/wagtail-localize/compare/v1.5.1...HEAD
+[1.5.1]: https://github.com/wagtail/wagtail-localize/compare/v1.5...v1.5.1
 [1.5]: https://github.com/wagtail/wagtail-localize/compare/v1.4...v1.5
 [1.4]: https://github.com/wagtail/wagtail-localize/compare/v1.3.3...v1.4
 [1.3.2]: https://github.com/wagtail/wagtail-localize/compare/v1.3.2...v1.3.3
 [1.3.2]: https://github.com/wagtail/wagtail-localize/compare/v1.3.1...v1.3.2
 [1.3.1]: https://github.com/wagtail/wagtail-localize/compare/v1.3...v1.3.1
 [1.3]: https://github.com/wagtail/wagtail-localize/compare/v1.3.0-alpha.3...v1.3
 [1.3alpha1]: https://github.com/wagtail/wagtail-localize/compare/v1.3.0-alpha.1...v1.3.0-alpha.3
```

### Comparing `wagtail-localize-1.5/LICENSE` & `wagtail-localize-1.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `wagtail-localize-1.5/README.md` & `wagtail-localize-1.5.1/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -14,17 +14,17 @@
 [Documentation](https://www.wagtail-localize.org)
 [Changelog](https://github.com/wagtail/wagtail-localize/blob/main/CHANGELOG.md)
 
 ## Requirements
 
 Wagtail Localize requires the following:
 
-- Python (3.7, 3.8, 3.9, 3.10, 3.11)
-- Django (3.2, 4.0, 4.1)
-- Wagtail (4.1, 4.2) with [internationalisation enabled](https://docs.wagtail.org/en/stable/advanced_topics/i18n.html#configuration)
+- Python (3.8, 3.9, 3.10, 3.11)
+- Django (3.2, 4.1, 4.2)
+- Wagtail (4.1, 4.2, 5.0) with [internationalisation enabled](https://docs.wagtail.org/en/stable/advanced_topics/i18n.html#configuration)
 
 ## Installation
 
 Install using `pip`:
 
 ```shell
 pip install wagtail-localize
@@ -62,31 +62,29 @@
 
 With your preferred virtualenv activated, install testing dependencies:
 
 #### Using pip
 
 ```sh
 pip install pip>=21.3
-pip install -e .[testing] -U
+pip install -e '.[testing]' -U
 ```
 
 #### Using flit
 
 ```sh
 pip install "flit>=3.8.0"
 flit install
 ```
 
 ### pre-commit
 
 Note that this project uses [pre-commit](https://github.com/pre-commit/pre-commit). To set up locally:
 
 ```shell
-# if you don't have it yet, globally
-$ pip install pre-commit
 # go to the project directory
 $ cd wagtail-localize
 # initialize pre-commit
 $ pre-commit install
 
 # Optional, run all checks once for this, then the checks will run only on the changed files
 $ pre-commit run --all-files
@@ -103,14 +101,14 @@
 or, you can run them for a specific environment `tox -e python3.8-django3.2-wagtail4.1` or specific test
 `tox -e python3.9-django3.2-wagtail4.1-sqlite wagtail_localize.tests.test_edit_translation.TestGetEditTranslationView`
 
 To run the test app interactively, use `tox -e interactive`, visit `http://127.0.0.1:8020/admin/` and log in with `admin`/`changeme`.
 
 ## Support
 
-For support, please use [GitHub Discussions](https://github.com/wagtail/wagtail-localize/discussions) or ask a question on the `#multi-language` channel on [Wagtail's Slack instance](`https://wagtail.org/slack/`).
+For support, please use [GitHub Discussions](https://github.com/wagtail/wagtail-localize/discussions) or ask a question on the `#multi-language` channel on [Wagtail's Slack instance](https://wagtail.org/slack/).
 
 ## Thanks
 
 Many thanks to all of our supporters, contributors, and early adopters who helped with the initial release. In particular, to The Mozilla Foundation and Torchbox who sponsored the majority of the initial development and Wagtail core's internationalisation support.
 
 <!--content-end-->
```

### Comparing `wagtail-localize-1.5/pyproject.toml` & `wagtail-localize-1.5.1/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 [build-system]
 requires = ["flit_core >=3.2,<4"]
 build-backend = "flit_core.buildapi"
 
 [project]
 name = "wagtail-localize"
 authors = [{name = "Karl Hobley", email = "karl@torchbox.com"}]
+maintainers = [{name = "Dan Braghis", email="dan.braghis@torchbox.com"}]
 description = "Translation plugin for Wagtail CMS"
 readme = "README.md"
 license = {file = "LICENSE"}
 classifiers = [
     "Development Status :: 4 - Beta",
     "Intended Audience :: Developers",
     "License :: OSI Approved :: BSD License",
@@ -18,42 +19,44 @@
     "Programming Language :: Python :: 3.7",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
     "Framework :: Django",
     "Framework :: Django :: 3.2",
-    "Framework :: Django :: 4.0",
     "Framework :: Django :: 4.1",
+    "Framework :: Django :: 4.2",
     "Framework :: Wagtail",
-    "Framework :: Wagtail :: 4"
+    "Framework :: Wagtail :: 4",
+    "Framework :: Wagtail :: 5"
 ]
 dynamic = ["version"]
-requires-python = ">=3.7"
+requires-python = ">=3.8"
 dependencies = [
-    "Django>=3.2,<4.2",
+    "Django>=3.2,<5.0",
     "Wagtail>=4.1",
     "polib>=1.1,<2.0",
     "typing_extensions>=4.0"
 ]
 
 [project.optional-dependencies]
 testing = [
     "dj-database-url==0.5.0",
     "freezegun==1.1.0",
     "django-rq>=2.5,<3.0",
-    "google-cloud-translate>=3.0.0"
+    "google-cloud-translate>=3.0.0",
+    "pre-commit>=2.21.0,<3.0"
 ]
 documentation = [
-    "mkdocs==1.1.2",
-    "mkdocs-material==6.2.8",
-    "mkdocs-mermaid2-plugin==0.5.1",
-    "mkdocstrings==0.14.0",
-    "mkdocs-include-markdown-plugin==2.8.0",
-    "pygments==2.11.2"
+    "mkdocs==1.4.3",
+    "mkdocs-material>=9.1,<10",
+    "mkdocstrings[python]==0.22.0",
+    "mkdocs-autorefs>=0.4.0,<0.5",
+    "mkdocs-include-markdown-plugin>=4.0.4,<5",
+    "pygments>=2.15,<2.16",
 ]
 google = [
     "google-cloud-translate>=3.0.0"
 ]
 
 [project.urls]
 Home = "https://www.wagtail-localize.org"
```

### Comparing `wagtail-localize-1.5/wagtail_localize/components.py` & `wagtail-localize-1.5.1/wagtail_localize/components.py`

 * *Files identical despite different names*

### Comparing `wagtail-localize-1.5/wagtail_localize/fields.py` & `wagtail-localize-1.5.1/wagtail_localize/fields.py`

 * *Files identical despite different names*

### Comparing `wagtail-localize-1.5/wagtail_localize/locale/ar/LC_MESSAGES/django.mo` & `wagtail-localize-1.5.1/wagtail_localize/locale/ar/LC_MESSAGES/django.mo`

 * *Files 16% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,12 +1,12 @@
 msgid ""
 msgstr ""
 "Report-Msgid-Bugs-To: \n"
 "Last-Translator: Younes Oumakhou, 2022\n"
-"Language-Team: Arabic (https://www.transifex.com/torchbox/teams/8009/ar/)\n"
+"Language-Team: Arabic (https://app.transifex.com/torchbox/teams/8009/ar/)\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Language: ar\n"
 "Plural-Forms: nplurals=6; plural=n==0 ? 0 : n==1 ? 1 : n==2 ? 2 : n%100>=3 "
 "&& n%100<=10 ? 3 : n%100>=11 && n%100<=99 ? 4 : 5;\n"
 
 msgid "Content"
 msgstr "محتوى"
```

### Comparing `wagtail-localize-1.5/wagtail_localize/locale/ar/LC_MESSAGES/django.po` & `wagtail-localize-1.5.1/wagtail_localize/locale/ar/LC_MESSAGES/django.po`

 * *Files 13% similar despite different names*

```diff
@@ -5,17 +5,17 @@
 # Ahmad Kiswani <kiswani.ahmad@gmail.com>, 2022
 # ultraify media <ultraify@gmail.com>, 2022
 # Younes Oumakhou, 2022
 #
 msgid ""
 msgstr ""
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2022-10-17 21:00+0000\n"
+"POT-Creation-Date: 2023-02-23 14:15+0000\n"
 "Last-Translator: Younes Oumakhou, 2022\n"
-"Language-Team: Arabic (https://www.transifex.com/torchbox/teams/8009/ar/)\n"
+"Language-Team: Arabic (https://app.transifex.com/torchbox/teams/8009/ar/)\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Language: ar\n"
 "Plural-Forms: nplurals=6; plural=n==0 ? 0 : n==1 ? 1 : n==2 ? 2 : n%100>=3 "
 "&& n%100<=10 ? 3 : n%100>=11 && n%100<=99 ? 4 : 5;\n"
 
 msgid "Saving…"
 msgstr "يتم الحفظ…"
```

### Comparing `wagtail-localize-1.5/wagtail_localize/locale/ar/LC_MESSAGES/djangojs.mo` & `wagtail-localize-1.5.1/wagtail_localize/locale/ar/LC_MESSAGES/djangojs.mo`

 * *Files 20% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,11 +1,11 @@
 msgid ""
 msgstr ""
-"Last-Translator: Younes Oumakhou, 2022\n"
-"Language-Team: Arabic (https://www.transifex.com/torchbox/teams/8009/ar/)\n"
+"Last-Translator: abdulaziz alfuhigi <abajall@gmail.com>, 2021\n"
+"Language-Team: Arabic (https://app.transifex.com/torchbox/teams/8009/ar/)\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Language: ar\n"
 "Plural-Forms: nplurals=6; plural=n==0 ? 0 : n==1 ? 1 : n==2 ? 2 : n%100>=3 "
 "&& n%100<=10 ? 3 : n%100>=11 && n%100<=99 ? 4 : 5;\n"
 
 msgid "Change image"
 msgstr "تغير الصورة"
@@ -18,17 +18,14 @@
 
 msgid "Choose an image"
 msgstr "اختر صورة"
 
 msgid "Delete"
 msgstr "حذف"
 
-msgid "Draft"
-msgstr "مسودة"
-
 msgid "Edit"
 msgstr "تحرير"
 
 msgid "Edit this %s"
 msgstr "تحرير هذا %s"
 
 msgid "Edit this document"
@@ -36,26 +33,20 @@
 
 msgid "Edit this image"
 msgstr "حرر هذه الصورة"
 
 msgid "Edit this page"
 msgstr "حرر هذه الصفحة"
 
-msgid "Live"
-msgstr "مباشر"
-
 msgid "Lock"
 msgstr "قفل"
 
 msgid "Preview"
 msgstr "نظر مقدم"
 
-msgid "Published"
-msgstr "تم نشره"
-
 msgid "Publishing..."
 msgstr "يتم النشر..."
 
 msgid "Save"
 msgstr "حفظ"
 
 msgid "Saving..."
```

### Comparing `wagtail-localize-1.5/wagtail_localize/locale/ar/LC_MESSAGES/djangojs.po` & `wagtail-localize-1.5.1/wagtail_localize/locale/ar/LC_MESSAGES/djangojs.po`

 * *Files 7% similar despite different names*

```diff
@@ -1,19 +1,18 @@
 #
 # Translators:
 # ROGER MICHAEL ASHLEY ALLEN <rogermaallen@gmail.com>, 2021
 # Ahmad Kiswani <kiswani.ahmad@gmail.com>, 2021
 # Ahmed Miske Sidi Med <boutien321@gmail.com>, 2021
 # abdulaziz alfuhigi <abajall@gmail.com>, 2021
-# Younes Oumakhou, 2022
 #
 msgid ""
 msgstr ""
-"Last-Translator: Younes Oumakhou, 2022\n"
-"Language-Team: Arabic (https://www.transifex.com/torchbox/teams/8009/ar/)\n"
+"Last-Translator: abdulaziz alfuhigi <abajall@gmail.com>, 2021\n"
+"Language-Team: Arabic (https://app.transifex.com/torchbox/teams/8009/ar/)\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Language: ar\n"
 "Plural-Forms: nplurals=6; plural=n==0 ? 0 : n==1 ? 1 : n==2 ? 2 : n%100>=3 "
 "&& n%100<=10 ? 3 : n%100>=11 && n%100<=99 ? 4 : 5;\n"
 
 msgid "Change image"
 msgstr "تغير الصورة"
@@ -26,17 +25,14 @@
 
 msgid "Choose an image"
 msgstr "اختر صورة"
 
 msgid "Delete"
 msgstr "حذف"
 
-msgid "Draft"
-msgstr "مسودة"
-
 msgid "Edit"
 msgstr "تحرير"
 
 msgid "Edit this %s"
 msgstr "تحرير هذا %s"
 
 msgid "Edit this document"
@@ -44,26 +40,20 @@
 
 msgid "Edit this image"
 msgstr "حرر هذه الصورة"
 
 msgid "Edit this page"
 msgstr "حرر هذه الصفحة"
 
-msgid "Live"
-msgstr "مباشر"
-
 msgid "Lock"
 msgstr "قفل"
 
 msgid "Preview"
 msgstr "نظر مقدم"
 
-msgid "Published"
-msgstr "تم نشره"
-
 msgid "Publishing..."
 msgstr "يتم النشر..."
 
 msgid "Save"
 msgstr "حفظ"
 
 msgid "Saving..."
```

### Comparing `wagtail-localize-1.5/wagtail_localize/locale/az_AZ/LC_MESSAGES/django.po` & `wagtail-localize-1.5.1/wagtail_localize/locale/az_AZ/LC_MESSAGES/django.po`

 * *Files 23% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 #
 # Translators:
 # Mirza Iskandarov <mirza.iskandarov@gmail.com>, 2022
 #
 msgid ""
 msgstr ""
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2022-10-17 21:00+0000\n"
+"POT-Creation-Date: 2023-02-23 14:15+0000\n"
 "Last-Translator: Mirza Iskandarov <mirza.iskandarov@gmail.com>, 2022\n"
-"Language-Team: Azerbaijani (Azerbaijan) (https://www.transifex.com/torchbox/"
+"Language-Team: Azerbaijani (Azerbaijan) (https://app.transifex.com/torchbox/"
 "teams/8009/az_AZ/)\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Language: az_AZ\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
 
 msgid "Saving…"
 msgstr "Yadda saxlanılır..."
```

### Comparing `wagtail-localize-1.5/wagtail_localize/locale/be/LC_MESSAGES/django.mo` & `wagtail-localize-1.5.1/wagtail_localize/locale/be/LC_MESSAGES/django.mo`

 * *Files 20% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,12 +1,12 @@
 msgid ""
 msgstr ""
 "Report-Msgid-Bugs-To: \n"
 "Last-Translator: Tatsiana Tsygan <art.tatsiana@gmail.com>, 2022\n"
-"Language-Team: Belarusian (https://www.transifex.com/torchbox/teams/8009/"
+"Language-Team: Belarusian (https://app.transifex.com/torchbox/teams/8009/"
 "be/)\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Language: be\n"
 "Plural-Forms: nplurals=4; plural=(n%10==1 && n%100!=11 ? 0 : n%10>=2 && "
 "n%10<=4 && (n%100<12 || n%100>14) ? 1 : n%10==0 || (n%10>=5 && n%10<=9) || "
 "(n%100>=11 && n%100<=14)? 2 : 3);\n"
```

### Comparing `wagtail-localize-1.5/wagtail_localize/locale/be/LC_MESSAGES/django.po` & `wagtail-localize-1.5.1/wagtail_localize/locale/be/LC_MESSAGES/django.po`

 * *Files 3% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 #
 # Translators:
 # Tatsiana Tsygan <art.tatsiana@gmail.com>, 2022
 #
 msgid ""
 msgstr ""
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2022-10-17 21:00+0000\n"
+"POT-Creation-Date: 2023-02-23 14:15+0000\n"
 "Last-Translator: Tatsiana Tsygan <art.tatsiana@gmail.com>, 2022\n"
-"Language-Team: Belarusian (https://www.transifex.com/torchbox/teams/8009/"
+"Language-Team: Belarusian (https://app.transifex.com/torchbox/teams/8009/"
 "be/)\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Language: be\n"
 "Plural-Forms: nplurals=4; plural=(n%10==1 && n%100!=11 ? 0 : n%10>=2 && "
 "n%10<=4 && (n%100<12 || n%100>14) ? 1 : n%10==0 || (n%10>=5 && n%10<=9) || "
 "(n%100>=11 && n%100<=14)? 2 : 3);\n"
```

### Comparing `wagtail-localize-1.5/wagtail_localize/locale/be/LC_MESSAGES/djangojs.mo` & `wagtail-localize-1.5.1/wagtail_localize/locale/be/LC_MESSAGES/djangojs.mo`

 * *Files 14% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,51 +1,42 @@
 msgid ""
 msgstr ""
 "Last-Translator: Tatsiana Tsygan <art.tatsiana@gmail.com>, 2021\n"
-"Language-Team: Belarusian (https://www.transifex.com/torchbox/teams/8009/"
+"Language-Team: Belarusian (https://app.transifex.com/torchbox/teams/8009/"
 "be/)\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Language: be\n"
 "Plural-Forms: nplurals=4; plural=(n%10==1 && n%100!=11 ? 0 : n%10>=2 && "
 "n%10<=4 && (n%100<12 || n%100>14) ? 1 : n%10==0 || (n%10>=5 && n%10<=9) || "
 "(n%100>=11 && n%100<=14)? 2 : 3);\n"
 
 msgid "Apply editor lock"
 msgstr "Заблакаваць рэдактар"
 
-msgid "Breadcrumb"
-msgstr "Шлях па сайту"
-
 msgid "Choose a document"
 msgstr "Абраць дакумент"
 
 msgid "Choose a page"
 msgstr "Выбраць старонку"
 
 msgid "Delete"
 msgstr "Выдаліць"
 
-msgid "Draft"
-msgstr "Чарнавік"
-
 msgid "Edit"
 msgstr "Рэдагаваць"
 
 msgid "Edit this %s"
 msgstr "Рэдактаваць гэта %s"
 
 msgid "Edit this document"
 msgstr "Рэдагаваць гэты дакумент"
 
 msgid "Edit this page"
 msgstr "Змяніць гэтую старонку"
 
-msgid "Live"
-msgstr "Размешчана"
-
 msgid "Lock"
 msgstr "Заблакаваць"
 
 msgid "Preview"
 msgstr "Папярэдні прагляд"
 
 msgid "Remove editor lock"
```

### Comparing `wagtail-localize-1.5/wagtail_localize/locale/be/LC_MESSAGES/djangojs.po` & `wagtail-localize-1.5.1/wagtail_localize/locale/be/LC_MESSAGES/djangojs.po`

 * *Files 8% similar despite different names*

```diff
@@ -2,55 +2,46 @@
 # Translators:
 # Stas Rudakou <stas@garage22.net>, 2021
 # Tatsiana Tsygan <art.tatsiana@gmail.com>, 2021
 #
 msgid ""
 msgstr ""
 "Last-Translator: Tatsiana Tsygan <art.tatsiana@gmail.com>, 2021\n"
-"Language-Team: Belarusian (https://www.transifex.com/torchbox/teams/8009/"
+"Language-Team: Belarusian (https://app.transifex.com/torchbox/teams/8009/"
 "be/)\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Language: be\n"
 "Plural-Forms: nplurals=4; plural=(n%10==1 && n%100!=11 ? 0 : n%10>=2 && "
 "n%10<=4 && (n%100<12 || n%100>14) ? 1 : n%10==0 || (n%10>=5 && n%10<=9) || "
 "(n%100>=11 && n%100<=14)? 2 : 3);\n"
 
 msgid "Apply editor lock"
 msgstr "Заблакаваць рэдактар"
 
-msgid "Breadcrumb"
-msgstr "Шлях па сайту"
-
 msgid "Choose a document"
 msgstr "Абраць дакумент"
 
 msgid "Choose a page"
 msgstr "Выбраць старонку"
 
 msgid "Delete"
 msgstr "Выдаліць"
 
-msgid "Draft"
-msgstr "Чарнавік"
-
 msgid "Edit"
 msgstr "Рэдагаваць"
 
 msgid "Edit this %s"
 msgstr "Рэдактаваць гэта %s"
 
 msgid "Edit this document"
 msgstr "Рэдагаваць гэты дакумент"
 
 msgid "Edit this page"
 msgstr "Змяніць гэтую старонку"
 
-msgid "Live"
-msgstr "Размешчана"
-
 msgid "Lock"
 msgstr "Заблакаваць"
 
 msgid "Preview"
 msgstr "Папярэдні прагляд"
 
 msgid "Remove editor lock"
```

### Comparing `wagtail-localize-1.5/wagtail_localize/locale/bg/LC_MESSAGES/django.po` & `wagtail-localize-1.5.1/wagtail_localize/locale/bg/LC_MESSAGES/django.po`

 * *Files 20% similar despite different names*

```diff
@@ -2,17 +2,17 @@
 # Translators:
 # Lyuboslav  Petrov <petrov.lyuboslav@gmail.com>, 2021
 # Karl Hobley <karl@torchbox.com>, 2022
 #
 msgid ""
 msgstr ""
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2022-10-17 21:00+0000\n"
+"POT-Creation-Date: 2023-02-23 14:15+0000\n"
 "Last-Translator: Karl Hobley <karl@torchbox.com>, 2022\n"
-"Language-Team: Bulgarian (https://www.transifex.com/torchbox/teams/8009/"
+"Language-Team: Bulgarian (https://app.transifex.com/torchbox/teams/8009/"
 "bg/)\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Language: bg\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
 
 msgid "Save"
 msgstr "Запази"
```

### Comparing `wagtail-localize-1.5/wagtail_localize/locale/bg/LC_MESSAGES/djangojs.mo` & `wagtail-localize-1.5.1/wagtail_localize/locale/bg/LC_MESSAGES/djangojs.mo`

 * *Files 16% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,11 +1,11 @@
 msgid ""
 msgstr ""
 "Last-Translator: Karl Hobley <karl@torchbox.com>, 2021\n"
-"Language-Team: Bulgarian (https://www.transifex.com/torchbox/teams/8009/"
+"Language-Team: Bulgarian (https://app.transifex.com/torchbox/teams/8009/"
 "bg/)\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Language: bg\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
 
 msgid "Choose a document"
 msgstr "Изберете документ"
```

### Comparing `wagtail-localize-1.5/wagtail_localize/locale/bg/LC_MESSAGES/djangojs.po` & `wagtail-localize-1.5.1/wagtail_localize/locale/bg/LC_MESSAGES/djangojs.po`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # Translators:
 # Lyuboslav  Petrov <petrov.lyuboslav@gmail.com>, 2021
 # Karl Hobley <karl@torchbox.com>, 2021
 #
 msgid ""
 msgstr ""
 "Last-Translator: Karl Hobley <karl@torchbox.com>, 2021\n"
-"Language-Team: Bulgarian (https://www.transifex.com/torchbox/teams/8009/"
+"Language-Team: Bulgarian (https://app.transifex.com/torchbox/teams/8009/"
 "bg/)\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Language: bg\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
 
 msgid "Choose a document"
 msgstr "Изберете документ"
```

### Comparing `wagtail-localize-1.5/wagtail_localize/locale/bn/LC_MESSAGES/django.mo` & `wagtail-localize-1.5.1/wagtail_localize/locale/bn/LC_MESSAGES/django.mo`

 * *Files 27% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,12 +1,12 @@
 msgid ""
 msgstr ""
 "Report-Msgid-Bugs-To: \n"
 "Last-Translator: MA Rahman <ugikot@gmail.com>, 2022\n"
-"Language-Team: Bengali (https://www.transifex.com/torchbox/teams/8009/bn/)\n"
+"Language-Team: Bengali (https://app.transifex.com/torchbox/teams/8009/bn/)\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Language: bn\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
 
 msgid "Content"
 msgstr "বিষয়বস্তু"
```

### Comparing `wagtail-localize-1.5/wagtail_localize/locale/bn/LC_MESSAGES/django.po` & `wagtail-localize-1.5.1/wagtail_localize/locale/bn/LC_MESSAGES/django.po`

 * *Files 2% similar despite different names*

```diff
@@ -2,17 +2,17 @@
 # Translators:
 # Mahmud Abdur Rahman <clanlord.ikot@gmail.com>, 2021
 # MA Rahman <ugikot@gmail.com>, 2022
 #
 msgid ""
 msgstr ""
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2022-10-17 21:00+0000\n"
+"POT-Creation-Date: 2023-02-23 14:15+0000\n"
 "Last-Translator: MA Rahman <ugikot@gmail.com>, 2022\n"
-"Language-Team: Bengali (https://www.transifex.com/torchbox/teams/8009/bn/)\n"
+"Language-Team: Bengali (https://app.transifex.com/torchbox/teams/8009/bn/)\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Language: bn\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
 
 msgid "Saving…"
 msgstr "সংরক্ষিত হচ্ছে..."
```

### Comparing `wagtail-localize-1.5/wagtail_localize/locale/bn/LC_MESSAGES/djangojs.mo` & `wagtail-localize-1.5.1/wagtail_localize/locale/bn/LC_MESSAGES/djangojs.mo`

 * *Files 18% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,11 +1,11 @@
 msgid ""
 msgstr ""
 "Last-Translator: Mahmud Abdur Rahman <clanlord.ikot@gmail.com>, 2021\n"
-"Language-Team: Bengali (https://www.transifex.com/torchbox/teams/8009/bn/)\n"
+"Language-Team: Bengali (https://app.transifex.com/torchbox/teams/8009/bn/)\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Language: bn\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
 
 msgid "Apply editor lock"
 msgstr "এডিটর লক প্রয়োগ করুন"
```

### Comparing `wagtail-localize-1.5/wagtail_localize/locale/bn/LC_MESSAGES/djangojs.po` & `wagtail-localize-1.5.1/wagtail_localize/locale/bn/LC_MESSAGES/djangojs.po`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # Translators:
 # MA Rahman <ugikot@gmail.com>, 2021
 # Mahmud Abdur Rahman <clanlord.ikot@gmail.com>, 2021
 #
 msgid ""
 msgstr ""
 "Last-Translator: Mahmud Abdur Rahman <clanlord.ikot@gmail.com>, 2021\n"
-"Language-Team: Bengali (https://www.transifex.com/torchbox/teams/8009/bn/)\n"
+"Language-Team: Bengali (https://app.transifex.com/torchbox/teams/8009/bn/)\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Language: bn\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
 
 msgid "Apply editor lock"
 msgstr "এডিটর লক প্রয়োগ করুন"
```

### Comparing `wagtail-localize-1.5/wagtail_localize/locale/ca/LC_MESSAGES/django.mo` & `wagtail-localize-1.5.1/wagtail_localize/locale/ca/LC_MESSAGES/django.mo`

 * *Files 1% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,12 +1,12 @@
 msgid ""
 msgstr ""
 "Report-Msgid-Bugs-To: \n"
 "Last-Translator: Roger Pons <rogerpons@gmail.com>, 2023\n"
-"Language-Team: Catalan (https://www.transifex.com/torchbox/teams/8009/ca/)\n"
+"Language-Team: Catalan (https://app.transifex.com/torchbox/teams/8009/ca/)\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Language: ca\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
 
 msgid ""
 "<{}> tag is not allowed. Strings can only contain standard HTML inline tags "
 "(such as <b>, <a>)"
```

### Comparing `wagtail-localize-1.5/wagtail_localize/locale/ca/LC_MESSAGES/django.po` & `wagtail-localize-1.5.1/wagtail_localize/locale/ca/LC_MESSAGES/django.po`

 * *Files 0% similar despite different names*

```diff
@@ -2,17 +2,17 @@
 # Translators:
 # Antoni Aloy <aaloy@apsl.net>, 2021
 # Roger Pons <rogerpons@gmail.com>, 2023
 #
 msgid ""
 msgstr ""
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2022-10-17 21:00+0000\n"
+"POT-Creation-Date: 2023-02-23 14:15+0000\n"
 "Last-Translator: Roger Pons <rogerpons@gmail.com>, 2023\n"
-"Language-Team: Catalan (https://www.transifex.com/torchbox/teams/8009/ca/)\n"
+"Language-Team: Catalan (https://app.transifex.com/torchbox/teams/8009/ca/)\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Language: ca\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
 
 msgid "Disable"
 msgstr "Desactivar"
```

### Comparing `wagtail-localize-1.5/wagtail_localize/locale/ca/LC_MESSAGES/djangojs.mo` & `wagtail-localize-1.5.1/wagtail_localize/locale/es/LC_MESSAGES/djangojs.mo`

 * *Files 16% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,160 +1,147 @@
 msgid ""
 msgstr ""
-"Last-Translator: Roger Pons <rogerpons@gmail.com>, 2023\n"
-"Language-Team: Catalan (https://www.transifex.com/torchbox/teams/8009/ca/)\n"
+"Last-Translator: Amós Oviedo <amos.oviedo@gmail.com>, 2022\n"
+"Language-Team: Spanish (https://app.transifex.com/torchbox/teams/8009/es/)\n"
 "Content-Type: text/plain; charset=UTF-8\n"
-"Language: ca\n"
-"Plural-Forms: nplurals=2; plural=(n != 1);\n"
+"Language: es\n"
+"Plural-Forms: nplurals=3; plural=n == 1 ? 0 : n != 0 && n % 1000000 == 0 ? "
+"1 : 2;\n"
 
 msgid "Apply editor lock"
-msgstr "Aplica bloqueig d'editor"
-
-msgid "Breadcrumb"
-msgstr "Ruta de navegació"
+msgstr "Aplicar bloqueo del editor"
 
 msgid "Cancel"
-msgstr "Cancel·lar"
+msgstr "Cancelar"
 
 msgid "Change %s"
-msgstr "Canviar %s"
+msgstr "Cambiar %s"
 
 msgid "Change document"
-msgstr "Canviar document"
+msgstr "Cambiar documento"
 
 msgid "Change image"
-msgstr "Substituir imatge"
+msgstr "Cambiar imagen"
 
 msgid "Change page"
-msgstr "Canviar pàgina"
+msgstr "Cambiar página"
 
 msgid "Changed"
-msgstr "Canviat/da"
+msgstr "Cambiado"
 
 msgid "Choose a %s"
-msgstr "Triar un/a %s"
+msgstr "Seleccionar un %s"
 
 msgid "Choose a document"
-msgstr "Escull un document"
+msgstr "Seleccionar un documento"
 
 msgid "Choose a page"
-msgstr "Escull una pàgina"
+msgstr "Seleccionar una página"
 
 msgid "Choose an image"
-msgstr "Escull una imatge"
+msgstr "Seleccionar una imagen"
 
 msgid "Convert to alias page"
-msgstr "Convertir a àlies de pàgina"
+msgstr "Convertir a alias de página"
 
 msgid "Delete"
 msgstr "Eliminar"
 
 msgid "Download PO file"
-msgstr "Baixar fitxer PO"
+msgstr "Descargar archivo PO"
 
 msgid "Download PO file and input translations offline"
-msgstr "Baixar fitxer PO i introduir traduccions fora de línia"
-
-msgid "Draft"
-msgstr "Esborrany"
+msgstr "Descargar archivo PO y traducir desconectado"
 
 msgid "Edit"
 msgstr "Editar"
 
 msgid "Edit this %s"
-msgstr "Editar aquest %s"
+msgstr "Editar este %s"
 
 msgid "Edit this document"
-msgstr "Editar aquest document"
+msgstr "Editar este docuemento"
 
 msgid "Edit this image"
-msgstr "Editar aquesta imatge"
+msgstr "Editar esta imagen"
 
 msgid "Edit this page"
-msgstr "Editar aquesta plana"
+msgstr "Editar esta página"
 
 msgid "Fetching %s information..."
-msgstr "Recol·lectant %s informació..."
+msgstr "Obtebiendo información %s..."
 
 msgid "Fetching document information..."
-msgstr "Recol·lectant informació del document..."
+msgstr "Obteniendo información del documento..."
 
 msgid "Fetching image information..."
-msgstr "Recol·lectant informació de la imatge..."
+msgstr "Obteniendo información de la imagen..."
 
 msgid "Fetching page information..."
-msgstr "Recol·lectant informació de la pàgina..."
-
-msgid "Live"
-msgstr "En viu"
+msgstr "Obteniendo información de la página..."
 
 msgid "Lock"
-msgstr "Bloqueja"
+msgstr "Bloquear"
 
 msgid "Not translated"
-msgstr "Sense traducció"
+msgstr "Sin traducir"
 
 msgid "Preview"
-msgstr "Previsualització"
+msgstr "Vista previa"
 
 msgid "Publish in "
-msgstr "Publicar a"
-
-msgid "Published"
-msgstr "Publicada"
-
-msgid "Published on "
-msgstr "Publicat a"
+msgstr "Publicar en"
 
 msgid "Publishing..."
-msgstr "Publicant..."
+msgstr "Publicando..."
 
 msgid "Remove editor lock"
-msgstr "Esborrar bloqueig d'editor"
+msgstr "Eliminar bloqueo del editor"
 
 msgid "Revert to %s version"
-msgstr "Revertir a la versió %s"
+msgstr "Revertir a versión %s"
 
 msgid "Save"
-msgstr "Desar"
+msgstr "Guardar"
 
 msgid "Saving..."
-msgstr "Desant..."
+msgstr "Guardando..."
 
 msgid "Server error"
-msgstr "Error de servidor"
+msgstr "Error del servidor"
 
 msgid "Stop Synced translation"
-msgstr "Aturar Traducció sincronitzada"
+msgstr "Parar traducción sincronizada"
 
 msgid "There are unsaved segments. Please save or cancel them before leaving."
-msgstr "Hi ha segments no desats. Deseu-los o cancel·leu-los abans de sortir."
+msgstr ""
+"Hay segmentos sin guardar. Por favor, guárdalos o cancélalos antes de salir."
 
 msgid "Translate"
-msgstr "Traduir"
+msgstr "Traducir"
 
 msgid "Translate all missing strings with "
-msgstr "Traduir totes les cadenes de caràcters que falten amb"
+msgstr "Traducir todas las cadenas faltantes con"
 
 msgid "Translate with "
-msgstr "Traduir amb"
+msgstr "Traducir con"
 
 msgid "Unlock"
-msgstr "Desbloquejar"
+msgstr "Desbloquear"
 
 msgid "Unpublish"
 msgstr "Despublicar"
 
 msgid "Upload PO file"
-msgstr "Pujar fitxer PO"
+msgstr "Cargar archivo PO"
 
 msgid "Upload translated PO file to submit translations"
-msgstr "Pujar fitxer PO traduït per enviar les traduccions"
+msgstr "Cargar archivo PO traducido para enviar traducciones"
 
 msgid "Uses %s version"
-msgstr "Utilitza la versió %s"
+msgstr "Usa versión %s"
 
 msgid "[DELETED]"
-msgstr "[ESBORRAT]"
+msgstr "[ELIMINADO]"
 
 msgid "segments translated"
-msgstr "segments traduïts"
+msgstr "segmentos traducidos"
```

### Comparing `wagtail-localize-1.5/wagtail_localize/locale/ca/LC_MESSAGES/djangojs.po` & `wagtail-localize-1.5.1/wagtail_localize/locale/ca/LC_MESSAGES/djangojs.po`

 * *Files 12% similar despite different names*

```diff
@@ -3,28 +3,25 @@
 # Antoni Aloy <aaloy@apsl.net>, 2021
 # David Llop, 2021
 # Roger Pons <rogerpons@gmail.com>, 2023
 #
 msgid ""
 msgstr ""
 "Last-Translator: Roger Pons <rogerpons@gmail.com>, 2023\n"
-"Language-Team: Catalan (https://www.transifex.com/torchbox/teams/8009/ca/)\n"
+"Language-Team: Catalan (https://app.transifex.com/torchbox/teams/8009/ca/)\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Language: ca\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
 
 msgid "[DELETED]"
 msgstr "[ESBORRAT]"
 
 msgid "Apply editor lock"
 msgstr "Aplica bloqueig d'editor"
 
-msgid "Breadcrumb"
-msgstr "Ruta de navegació"
-
 msgid "Cancel"
 msgstr "Cancel·lar"
 
 msgid "Change %s"
 msgstr "Canviar %s"
 
 msgid "Change document"
@@ -59,17 +56,14 @@
 
 msgid "Download PO file"
 msgstr "Baixar fitxer PO"
 
 msgid "Download PO file and input translations offline"
 msgstr "Baixar fitxer PO i introduir traduccions fora de línia"
 
-msgid "Draft"
-msgstr "Esborrany"
-
 msgid "Edit"
 msgstr "Editar"
 
 msgid "Edit this %s"
 msgstr "Editar aquest %s"
 
 msgid "Edit this document"
@@ -89,35 +83,26 @@
 
 msgid "Fetching image information..."
 msgstr "Recol·lectant informació de la imatge..."
 
 msgid "Fetching page information..."
 msgstr "Recol·lectant informació de la pàgina..."
 
-msgid "Live"
-msgstr "En viu"
-
 msgid "Lock"
 msgstr "Bloqueja"
 
 msgid "Not translated"
 msgstr "Sense traducció"
 
 msgid "Preview"
 msgstr "Previsualització"
 
 msgid "Publish in "
 msgstr "Publicar a"
 
-msgid "Published"
-msgstr "Publicada"
-
-msgid "Published on "
-msgstr "Publicat a"
-
 msgid "Publishing..."
 msgstr "Publicant..."
 
 msgid "Remove editor lock"
 msgstr "Esborrar bloqueig d'editor"
 
 msgid "Revert to %s version"
```

### Comparing `wagtail-localize-1.5/wagtail_localize/locale/cs/LC_MESSAGES/django.mo` & `wagtail-localize-1.5.1/wagtail_localize/locale/cs/LC_MESSAGES/django.mo`

 * *Files 0% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,12 +1,12 @@
 msgid ""
 msgstr ""
 "Report-Msgid-Bugs-To: \n"
 "Last-Translator: Mirek Zvolský <zvolsky@seznam.cz>, 2022\n"
-"Language-Team: Czech (https://www.transifex.com/torchbox/teams/8009/cs/)\n"
+"Language-Team: Czech (https://app.transifex.com/torchbox/teams/8009/cs/)\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Language: cs\n"
 "Plural-Forms: nplurals=4; plural=(n == 1 && n % 1 == 0) ? 0 : (n >= 2 && n "
 "<= 4 && n % 1 == 0) ? 1: (n % 1 != 0 ) ? 2 : 3;\n"
 
 msgid ""
 "<{}> tag is not allowed. Strings can only contain standard HTML inline tags "
```

### Comparing `wagtail-localize-1.5/wagtail_localize/locale/cs/LC_MESSAGES/django.po` & `wagtail-localize-1.5.1/wagtail_localize/locale/cs/LC_MESSAGES/django.po`

 * *Files 1% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 #
 # Translators:
 # Mirek Zvolský <zvolsky@seznam.cz>, 2022
 #
 msgid ""
 msgstr ""
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2022-10-17 21:00+0000\n"
+"POT-Creation-Date: 2023-02-23 14:15+0000\n"
 "Last-Translator: Mirek Zvolský <zvolsky@seznam.cz>, 2022\n"
-"Language-Team: Czech (https://www.transifex.com/torchbox/teams/8009/cs/)\n"
+"Language-Team: Czech (https://app.transifex.com/torchbox/teams/8009/cs/)\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Language: cs\n"
 "Plural-Forms: nplurals=4; plural=(n == 1 && n % 1 == 0) ? 0 : (n >= 2 && n "
 "<= 4 && n % 1 == 0) ? 1: (n % 1 != 0 ) ? 2 : 3;\n"
 
 msgid "Disable"
 msgstr "Zakázat"
```

### Comparing `wagtail-localize-1.5/wagtail_localize/locale/cs/LC_MESSAGES/djangojs.mo` & `wagtail-localize-1.5.1/wagtail_localize/locale/cs/LC_MESSAGES/djangojs.mo`

 * *Files 22% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,22 +1,19 @@
 msgid ""
 msgstr ""
 "Last-Translator: Mirek Zvolský <zvolsky@seznam.cz>, 2021\n"
-"Language-Team: Czech (https://www.transifex.com/torchbox/teams/8009/cs/)\n"
+"Language-Team: Czech (https://app.transifex.com/torchbox/teams/8009/cs/)\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Language: cs\n"
 "Plural-Forms: nplurals=4; plural=(n == 1 && n % 1 == 0) ? 0 : (n >= 2 && n "
 "<= 4 && n % 1 == 0) ? 1: (n % 1 != 0 ) ? 2 : 3;\n"
 
 msgid "Apply editor lock"
 msgstr "Uzamknout pro úpravy"
 
-msgid "Breadcrumb"
-msgstr "Navigace stránek"
-
 msgid "Cancel"
 msgstr "Storno"
 
 msgid "Change document"
 msgstr "Změnit dokument"
 
 msgid "Change image"
@@ -42,17 +39,14 @@
 
 msgid "Download PO file"
 msgstr "Stáhnout PO soubor"
 
 msgid "Download PO file and input translations offline"
 msgstr "Stáhnout PO soubor a zadat překlady offline"
 
-msgid "Draft"
-msgstr "Koncept"
-
 msgid "Edit"
 msgstr "Upravit"
 
 msgid "Edit this %s"
 msgstr "Edituj %s"
 
 msgid "Edit this document"
@@ -69,35 +63,26 @@
 
 msgid "Fetching image information..."
 msgstr "Získávají se informace o obrázku..."
 
 msgid "Fetching page information..."
 msgstr "Získávají se informace o stránce..."
 
-msgid "Live"
-msgstr "Publikováno"
-
 msgid "Lock"
 msgstr "Uzamknout"
 
 msgid "Not translated"
 msgstr "Není přeloženo"
 
 msgid "Preview"
 msgstr "Náhled"
 
 msgid "Publish in "
 msgstr "Publikovat"
 
-msgid "Published"
-msgstr "Publikováno"
-
-msgid "Published on "
-msgstr "Publikováno"
-
 msgid "Publishing..."
 msgstr "Publikování..."
 
 msgid "Remove editor lock"
 msgstr "Zrušit uzamčení pro úpravy"
 
 msgid "Save"
```

### Comparing `wagtail-localize-1.5/wagtail_localize/locale/cs/LC_MESSAGES/djangojs.po` & `wagtail-localize-1.5.1/wagtail_localize/locale/cs/LC_MESSAGES/djangojs.po`

 * *Files 10% similar despite different names*

```diff
@@ -1,30 +1,26 @@
 #
 # Translators:
-# Kryštof Pilnáček <krystof.pilnacek@rossum.ai>, 2020
 # Mirek Zvolský <zvolsky@seznam.cz>, 2021
 #
 msgid ""
 msgstr ""
 "Last-Translator: Mirek Zvolský <zvolsky@seznam.cz>, 2021\n"
-"Language-Team: Czech (https://www.transifex.com/torchbox/teams/8009/cs/)\n"
+"Language-Team: Czech (https://app.transifex.com/torchbox/teams/8009/cs/)\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Language: cs\n"
 "Plural-Forms: nplurals=4; plural=(n == 1 && n % 1 == 0) ? 0 : (n >= 2 && n "
 "<= 4 && n % 1 == 0) ? 1: (n % 1 != 0 ) ? 2 : 3;\n"
 
 msgid "[DELETED]"
 msgstr "[ZRUŠENO]"
 
 msgid "Apply editor lock"
 msgstr "Uzamknout pro úpravy"
 
-msgid "Breadcrumb"
-msgstr "Navigace stránek"
-
 msgid "Cancel"
 msgstr "Storno"
 
 msgid "Change document"
 msgstr "Změnit dokument"
 
 msgid "Change image"
@@ -50,17 +46,14 @@
 
 msgid "Download PO file"
 msgstr "Stáhnout PO soubor"
 
 msgid "Download PO file and input translations offline"
 msgstr "Stáhnout PO soubor a zadat překlady offline"
 
-msgid "Draft"
-msgstr "Koncept"
-
 msgid "Edit"
 msgstr "Upravit"
 
 msgid "Edit this %s"
 msgstr "Edituj %s"
 
 msgid "Edit this document"
@@ -77,35 +70,26 @@
 
 msgid "Fetching image information..."
 msgstr "Získávají se informace o obrázku..."
 
 msgid "Fetching page information..."
 msgstr "Získávají se informace o stránce..."
 
-msgid "Live"
-msgstr "Publikováno"
-
 msgid "Lock"
 msgstr "Uzamknout"
 
 msgid "Not translated"
 msgstr "Není přeloženo"
 
 msgid "Preview"
 msgstr "Náhled"
 
 msgid "Publish in "
 msgstr "Publikovat"
 
-msgid "Published"
-msgstr "Publikováno"
-
-msgid "Published on "
-msgstr "Publikováno"
-
 msgid "Publishing..."
 msgstr "Publikování..."
 
 msgid "Remove editor lock"
 msgstr "Zrušit uzamčení pro úpravy"
 
 msgid "Save"
```

### Comparing `wagtail-localize-1.5/wagtail_localize/locale/cy/LC_MESSAGES/django.mo` & `wagtail-localize-1.5.1/wagtail_localize/locale/cy/LC_MESSAGES/django.mo`

 * *Files 0% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,12 +1,12 @@
 msgid ""
 msgstr ""
 "Report-Msgid-Bugs-To: \n"
 "Last-Translator: Matt Westcott <matthew@torchbox.com>, 2022\n"
-"Language-Team: Welsh (https://www.transifex.com/torchbox/teams/8009/cy/)\n"
+"Language-Team: Welsh (https://app.transifex.com/torchbox/teams/8009/cy/)\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Language: cy\n"
 "Plural-Forms: nplurals=4; plural=(n==1) ? 0 : (n==2) ? 1 : (n != 8 && n != "
 "11) ? 2 : 3;\n"
 
 msgid ""
 "<{}> tag is not allowed. Strings can only contain standard HTML inline tags "
```

### Comparing `wagtail-localize-1.5/wagtail_localize/locale/cy/LC_MESSAGES/django.po` & `wagtail-localize-1.5.1/wagtail_localize/locale/cy/LC_MESSAGES/django.po`

 * *Files 1% similar despite different names*

```diff
@@ -3,17 +3,17 @@
 # Philip Crisp, 2022
 # Adam Hughes <adamhughes31@gmail.com>, 2022
 # Matt Westcott <matthew@torchbox.com>, 2022
 #
 msgid ""
 msgstr ""
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2022-10-17 21:00+0000\n"
+"POT-Creation-Date: 2023-02-23 14:15+0000\n"
 "Last-Translator: Matt Westcott <matthew@torchbox.com>, 2022\n"
-"Language-Team: Welsh (https://www.transifex.com/torchbox/teams/8009/cy/)\n"
+"Language-Team: Welsh (https://app.transifex.com/torchbox/teams/8009/cy/)\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Language: cy\n"
 "Plural-Forms: nplurals=4; plural=(n==1) ? 0 : (n==2) ? 1 : (n != 8 && n != "
 "11) ? 2 : 3;\n"
 
 msgid "Disable"
 msgstr "Analluogi"
```

### Comparing `wagtail-localize-1.5/wagtail_localize/locale/cy/LC_MESSAGES/djangojs.mo` & `wagtail-localize-1.5.1/wagtail_localize/locale/cy/LC_MESSAGES/djangojs.mo`

 * *Files 13% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,22 +1,19 @@
 msgid ""
 msgstr ""
 "Last-Translator: Philip Crisp, 2022\n"
-"Language-Team: Welsh (https://www.transifex.com/torchbox/teams/8009/cy/)\n"
+"Language-Team: Welsh (https://app.transifex.com/torchbox/teams/8009/cy/)\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Language: cy\n"
 "Plural-Forms: nplurals=4; plural=(n==1) ? 0 : (n==2) ? 1 : (n != 8 && n != "
 "11) ? 2 : 3;\n"
 
 msgid "Apply editor lock"
 msgstr "Cymhwyso clo golygydd"
 
-msgid "Breadcrumb"
-msgstr "Briwsion Bara"
-
 msgid "Cancel"
 msgstr "Canslo"
 
 msgid "Change %s"
 msgstr "Newid %s"
 
 msgid "Change document"
@@ -51,17 +48,14 @@
 
 msgid "Download PO file"
 msgstr "Lawrlwythwch ffeil PO"
 
 msgid "Download PO file and input translations offline"
 msgstr "Dadlwythwch ffeil PO a mewnbynnu cyfieithiadau all-lein"
 
-msgid "Draft"
-msgstr "Drafft"
-
 msgid "Edit"
 msgstr "Golygu"
 
 msgid "Edit this %s"
 msgstr "Golygu %s"
 
 msgid "Edit this document"
@@ -81,35 +75,26 @@
 
 msgid "Fetching image information..."
 msgstr "Wrthi'n nôl gwybodaeth llun..."
 
 msgid "Fetching page information..."
 msgstr "Wrthi'n nôl gwybodaeth tudalen..."
 
-msgid "Live"
-msgstr "Yn fyw"
-
 msgid "Lock"
 msgstr "Clo"
 
 msgid "Not translated"
 msgstr "Heb ei gyfieithu"
 
 msgid "Preview"
 msgstr "Rhagolwg"
 
 msgid "Publish in "
 msgstr "Cyhoeddi yn "
 
-msgid "Published"
-msgstr "Wedi cyhoeddi"
-
-msgid "Published on "
-msgstr "Cyhoeddwyd ar "
-
 msgid "Publishing..."
 msgstr "Wrthi'n cyhoeddi..."
 
 msgid "Remove editor lock"
 msgstr "Dileu clo'r golygydd"
 
 msgid "Revert to %s version"
```

### Comparing `wagtail-localize-1.5/wagtail_localize/locale/cy/LC_MESSAGES/djangojs.po` & `wagtail-localize-1.5.1/wagtail_localize/locale/cy/LC_MESSAGES/djangojs.po`

 * *Files 3% similar despite different names*

```diff
@@ -2,29 +2,26 @@
 # Translators:
 # Adam Hughes <adamhughes31@gmail.com>, 2021
 # Philip Crisp, 2022
 #
 msgid ""
 msgstr ""
 "Last-Translator: Philip Crisp, 2022\n"
-"Language-Team: Welsh (https://www.transifex.com/torchbox/teams/8009/cy/)\n"
+"Language-Team: Welsh (https://app.transifex.com/torchbox/teams/8009/cy/)\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Language: cy\n"
 "Plural-Forms: nplurals=4; plural=(n==1) ? 0 : (n==2) ? 1 : (n != 8 && n != "
 "11) ? 2 : 3;\n"
 
 msgid "[DELETED]"
 msgstr "[WEDI'I DILEU]"
 
 msgid "Apply editor lock"
 msgstr "Cymhwyso clo golygydd"
 
-msgid "Breadcrumb"
-msgstr "Briwsion Bara"
-
 msgid "Cancel"
 msgstr "Canslo"
 
 msgid "Change %s"
 msgstr "Newid %s"
 
 msgid "Change document"
@@ -59,17 +56,14 @@
 
 msgid "Download PO file"
 msgstr "Lawrlwythwch ffeil PO"
 
 msgid "Download PO file and input translations offline"
 msgstr "Dadlwythwch ffeil PO a mewnbynnu cyfieithiadau all-lein"
 
-msgid "Draft"
-msgstr "Drafft"
-
 msgid "Edit"
 msgstr "Golygu"
 
 msgid "Edit this %s"
 msgstr "Golygu %s"
 
 msgid "Edit this document"
@@ -89,35 +83,26 @@
 
 msgid "Fetching image information..."
 msgstr "Wrthi'n nôl gwybodaeth llun..."
 
 msgid "Fetching page information..."
 msgstr "Wrthi'n nôl gwybodaeth tudalen..."
 
-msgid "Live"
-msgstr "Yn fyw"
-
 msgid "Lock"
 msgstr "Clo"
 
 msgid "Not translated"
 msgstr "Heb ei gyfieithu"
 
 msgid "Preview"
 msgstr "Rhagolwg"
 
 msgid "Publish in "
 msgstr "Cyhoeddi yn "
 
-msgid "Published"
-msgstr "Wedi cyhoeddi"
-
-msgid "Published on "
-msgstr "Cyhoeddwyd ar "
-
 msgid "Publishing..."
 msgstr "Wrthi'n cyhoeddi..."
 
 msgid "Remove editor lock"
 msgstr "Dileu clo'r golygydd"
 
 msgid "Revert to %s version"
```

### Comparing `wagtail-localize-1.5/wagtail_localize/locale/da/LC_MESSAGES/django.po` & `wagtail-localize-1.5.1/wagtail_localize/locale/da/LC_MESSAGES/django.po`

 * *Files 20% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 #
 # Translators:
 # Mads Kronborg <madskronborg99@gmail.com>, 2022
 #
 msgid ""
 msgstr ""
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2022-10-17 21:00+0000\n"
+"POT-Creation-Date: 2023-02-23 14:15+0000\n"
 "Last-Translator: Mads Kronborg <madskronborg99@gmail.com>, 2022\n"
-"Language-Team: Danish (https://www.transifex.com/torchbox/teams/8009/da/)\n"
+"Language-Team: Danish (https://app.transifex.com/torchbox/teams/8009/da/)\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Language: da\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
 
 msgid "Saving…"
 msgstr "Gemmer..."
```

### Comparing `wagtail-localize-1.5/wagtail_localize/locale/da/LC_MESSAGES/djangojs.mo` & `wagtail-localize-1.5.1/wagtail_localize/locale/tr_TR/LC_MESSAGES/djangojs.mo`

 * *Files 26% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,49 +1,59 @@
 msgid ""
 msgstr ""
-"Last-Translator: Benjamin Bach <benjaoming@gmail.com>, 2022\n"
-"Language-Team: Danish (https://www.transifex.com/torchbox/teams/8009/da/)\n"
+"Last-Translator: Py Data Geek <pydatageek@gmail.com>, 2021\n"
+"Language-Team: Turkish (Turkey) (https://app.transifex.com/torchbox/"
+"teams/8009/tr_TR/)\n"
 "Content-Type: text/plain; charset=UTF-8\n"
-"Language: da\n"
-"Plural-Forms: nplurals=2; plural=(n != 1);\n"
+"Language: tr_TR\n"
+"Plural-Forms: nplurals=2; plural=(n > 1);\n"
 
-msgid "Apply editor lock"
-msgstr "Aktivér redaktør-lås"
+msgid "Change image"
+msgstr "Resmi değiştir"
 
 msgid "Choose a document"
-msgstr "Vælg et dokument"
+msgstr "Belge seç"
 
 msgid "Choose a page"
-msgstr "Vælg en side"
+msgstr "Bir sayfa seç"
 
-msgid "Delete"
-msgstr "Slet"
+msgid "Choose an image"
+msgstr "Bir resim seç"
 
-msgid "Draft"
-msgstr "Skitse"
+msgid "Delete"
+msgstr "Sil"
 
 msgid "Edit"
-msgstr "Rediger"
+msgstr "Düzenle"
 
-msgid "Edit this page"
-msgstr "Rediger denne side"
+msgid "Edit this %s"
+msgstr "%s düzenle"
+
+msgid "Edit this document"
+msgstr "Belgeyi düzenle"
 
-msgid "Live"
-msgstr "Live"
+msgid "Edit this image"
+msgstr "Resmi düzenle"
+
+msgid "Edit this page"
+msgstr "Sayfayı düzenle"
 
 msgid "Lock"
-msgstr "Lås"
+msgstr "Kilitle"
 
 msgid "Preview"
-msgstr "Forhåndsvis"
+msgstr "Önizleme"
+
+msgid "Remove editor lock"
+msgstr "Editör kilidini kaldır"
 
 msgid "Save"
-msgstr "Gem"
+msgstr "Kaydet"
 
 msgid "Saving..."
-msgstr "Gemmer..."
+msgstr "Kaydediyor..."
 
 msgid "Unlock"
-msgstr "Lås op"
+msgstr "Kilidi kaldır"
 
 msgid "Unpublish"
-msgstr "Afpublicer"
+msgstr "Yayından Kaldır"
```

### Comparing `wagtail-localize-1.5/wagtail_localize/locale/da/LC_MESSAGES/djangojs.po` & `wagtail-localize-1.5.1/wagtail_localize/locale/da/LC_MESSAGES/djangojs.po`

 * *Files 7% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 # Asger Sørensen <asger.soerensen@live.com>, 2021
 # Mads Kronborg <madskronborg99@gmail.com>, 2021
 # Benjamin Bach <benjaoming@gmail.com>, 2022
 #
 msgid ""
 msgstr ""
 "Last-Translator: Benjamin Bach <benjaoming@gmail.com>, 2022\n"
-"Language-Team: Danish (https://www.transifex.com/torchbox/teams/8009/da/)\n"
+"Language-Team: Danish (https://app.transifex.com/torchbox/teams/8009/da/)\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Language: da\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
 
 msgid "Apply editor lock"
 msgstr "Aktivér redaktør-lås"
 
@@ -21,26 +21,20 @@
 
 msgid "Choose a page"
 msgstr "Vælg en side"
 
 msgid "Delete"
 msgstr "Slet"
 
-msgid "Draft"
-msgstr "Skitse"
-
 msgid "Edit"
 msgstr "Rediger"
 
 msgid "Edit this page"
 msgstr "Rediger denne side"
 
-msgid "Live"
-msgstr "Live"
-
 msgid "Lock"
 msgstr "Lås"
 
 msgid "Preview"
 msgstr "Forhåndsvis"
 
 msgid "Save"
```

### Comparing `wagtail-localize-1.5/wagtail_localize/locale/de/LC_MESSAGES/django.mo` & `wagtail-localize-1.5.1/wagtail_localize/locale/de/LC_MESSAGES/django.mo`

 * *Files 2% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,12 +1,12 @@
 msgid ""
 msgstr ""
 "Report-Msgid-Bugs-To: \n"
 "Last-Translator: Stefan Hammer <stefan@hammerworxx.com>, 2022\n"
-"Language-Team: German (https://www.transifex.com/torchbox/teams/8009/de/)\n"
+"Language-Team: German (https://app.transifex.com/torchbox/teams/8009/de/)\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Language: de\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
 
 msgid ""
 "<{}> tag is not allowed. Strings can only contain standard HTML inline tags "
 "(such as <b>, <a>)"
```

### Comparing `wagtail-localize-1.5/wagtail_localize/locale/de/LC_MESSAGES/django.po` & `wagtail-localize-1.5.1/wagtail_localize/locale/de/LC_MESSAGES/django.po`

 * *Files 1% similar despite different names*

```diff
@@ -7,17 +7,17 @@
 # Oliver Engel <codeangel@posteo.de>, 2022
 # Moritz Pfeiffer <moritz@alp-phone.ch>, 2022
 # Stefan Hammer <stefan@hammerworxx.com>, 2022
 #
 msgid ""
 msgstr ""
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2022-10-17 21:00+0000\n"
+"POT-Creation-Date: 2023-02-23 14:15+0000\n"
 "Last-Translator: Stefan Hammer <stefan@hammerworxx.com>, 2022\n"
-"Language-Team: German (https://www.transifex.com/torchbox/teams/8009/de/)\n"
+"Language-Team: German (https://app.transifex.com/torchbox/teams/8009/de/)\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Language: de\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
 
 msgid "Disable"
 msgstr "Deaktivieren"
```

### Comparing `wagtail-localize-1.5/wagtail_localize/locale/de/LC_MESSAGES/djangojs.mo` & `wagtail-localize-1.5.1/wagtail_localize/locale/de/LC_MESSAGES/djangojs.mo`

 * *Files 9% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,21 +1,18 @@
 msgid ""
 msgstr ""
 "Last-Translator: Stefan Hammer <stefan@hammerworxx.com>, 2022\n"
-"Language-Team: German (https://www.transifex.com/torchbox/teams/8009/de/)\n"
+"Language-Team: German (https://app.transifex.com/torchbox/teams/8009/de/)\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Language: de\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
 
 msgid "Apply editor lock"
 msgstr "Editor-Sperre anwenden"
 
-msgid "Breadcrumb"
-msgstr "Breadcrumb"
-
 msgid "Cancel"
 msgstr "Abbrechen"
 
 msgid "Change %s"
 msgstr "Ändere %s"
 
 msgid "Change document"
@@ -50,17 +47,14 @@
 
 msgid "Download PO file"
 msgstr "PO Datei herunterladen"
 
 msgid "Download PO file and input translations offline"
 msgstr "Lade PO Datei herunter und füge Übersetzungen offline hinzu"
 
-msgid "Draft"
-msgstr "Entwurf"
-
 msgid "Edit"
 msgstr "Bearbeiten"
 
 msgid "Edit this %s"
 msgstr "%s bearbeiten"
 
 msgid "Edit this document"
@@ -80,35 +74,26 @@
 
 msgid "Fetching image information..."
 msgstr "Bildinformationen werden gesammelt…"
 
 msgid "Fetching page information..."
 msgstr "Seiteninformationen werden gesammelt…"
 
-msgid "Live"
-msgstr "Live"
-
 msgid "Lock"
 msgstr "Sperren"
 
 msgid "Not translated"
 msgstr "Nicht übersetzt"
 
 msgid "Preview"
 msgstr "Vorschau"
 
 msgid "Publish in "
 msgstr "Veröffentlichen in "
 
-msgid "Published"
-msgstr "Veröffentlicht"
-
-msgid "Published on "
-msgstr "Veröffentlicht am "
-
 msgid "Publishing..."
 msgstr "Veröffentlichen..."
 
 msgid "Remove editor lock"
 msgstr "Editor-Sperre aufheben"
 
 msgid "Revert to %s version"
```

### Comparing `wagtail-localize-1.5/wagtail_localize/locale/de/LC_MESSAGES/djangojs.po` & `wagtail-localize-1.5.1/wagtail_localize/locale/de/LC_MESSAGES/djangojs.po`

 * *Files 4% similar despite different names*

```diff
@@ -4,28 +4,25 @@
 # Oliver Engel <codeangel@posteo.de>, 2021
 # Krzysztof Jeziorny <github@jeziorny.net>, 2021
 # Stefan Hammer <stefan@hammerworxx.com>, 2022
 #
 msgid ""
 msgstr ""
 "Last-Translator: Stefan Hammer <stefan@hammerworxx.com>, 2022\n"
-"Language-Team: German (https://www.transifex.com/torchbox/teams/8009/de/)\n"
+"Language-Team: German (https://app.transifex.com/torchbox/teams/8009/de/)\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Language: de\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
 
 msgid "[DELETED]"
 msgstr "[GELÖSCHT]"
 
 msgid "Apply editor lock"
 msgstr "Editor-Sperre anwenden"
 
-msgid "Breadcrumb"
-msgstr "Breadcrumb"
-
 msgid "Cancel"
 msgstr "Abbrechen"
 
 msgid "Change %s"
 msgstr "Ändere %s"
 
 msgid "Change document"
@@ -60,17 +57,14 @@
 
 msgid "Download PO file"
 msgstr "PO Datei herunterladen"
 
 msgid "Download PO file and input translations offline"
 msgstr "Lade PO Datei herunter und füge Übersetzungen offline hinzu"
 
-msgid "Draft"
-msgstr "Entwurf"
-
 msgid "Edit"
 msgstr "Bearbeiten"
 
 msgid "Edit this %s"
 msgstr "%s bearbeiten"
 
 msgid "Edit this document"
@@ -90,35 +84,26 @@
 
 msgid "Fetching image information..."
 msgstr "Bildinformationen werden gesammelt…"
 
 msgid "Fetching page information..."
 msgstr "Seiteninformationen werden gesammelt…"
 
-msgid "Live"
-msgstr "Live"
-
 msgid "Lock"
 msgstr "Sperren"
 
 msgid "Not translated"
 msgstr "Nicht übersetzt"
 
 msgid "Preview"
 msgstr "Vorschau"
 
 msgid "Publish in "
 msgstr "Veröffentlichen in "
 
-msgid "Published"
-msgstr "Veröffentlicht"
-
-msgid "Published on "
-msgstr "Veröffentlicht am "
-
 msgid "Publishing..."
 msgstr "Veröffentlichen..."
 
 msgid "Remove editor lock"
 msgstr "Editor-Sperre aufheben"
 
 msgid "Revert to %s version"
```

### Comparing `wagtail-localize-1.5/wagtail_localize/locale/el/LC_MESSAGES/django.mo` & `wagtail-localize-1.5.1/wagtail_localize/locale/el/LC_MESSAGES/django.mo`

 * *Files 2% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,12 +1,12 @@
 msgid ""
 msgstr ""
 "Report-Msgid-Bugs-To: \n"
 "Last-Translator: Matt Westcott <matthew@torchbox.com>, 2022\n"
-"Language-Team: Greek (https://www.transifex.com/torchbox/teams/8009/el/)\n"
+"Language-Team: Greek (https://app.transifex.com/torchbox/teams/8009/el/)\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Language: el\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
 
 msgid "Content"
 msgstr "Περιεχομενο"
```

### Comparing `wagtail-localize-1.5/wagtail_localize/locale/el/LC_MESSAGES/django.po` & `wagtail-localize-1.5.1/wagtail_localize/locale/el/LC_MESSAGES/django.po`

 * *Files 12% similar despite different names*

```diff
@@ -6,17 +6,17 @@
 # Nick Mavrakis <mavrakis.n@gmail.com>, 2022
 # Yiannis Inglessis <negtheone@gmail.com>, 2022
 # Matt Westcott <matthew@torchbox.com>, 2022
 #
 msgid ""
 msgstr ""
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2022-10-17 21:00+0000\n"
+"POT-Creation-Date: 2023-02-23 14:15+0000\n"
 "Last-Translator: Matt Westcott <matthew@torchbox.com>, 2022\n"
-"Language-Team: Greek (https://www.transifex.com/torchbox/teams/8009/el/)\n"
+"Language-Team: Greek (https://app.transifex.com/torchbox/teams/8009/el/)\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Language: el\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
 
 msgid "Saving…"
 msgstr "Γίνεται αποθήκευση…"
```

### Comparing `wagtail-localize-1.5/wagtail_localize/locale/el/LC_MESSAGES/djangojs.mo` & `wagtail-localize-1.5.1/wagtail_localize/locale/el/LC_MESSAGES/djangojs.mo`

 * *Files 13% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,11 +1,11 @@
 msgid ""
 msgstr ""
 "Last-Translator: fekioh, 2022\n"
-"Language-Team: Greek (https://www.transifex.com/torchbox/teams/8009/el/)\n"
+"Language-Team: Greek (https://app.transifex.com/torchbox/teams/8009/el/)\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Language: el\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
 
 msgid "Apply editor lock"
 msgstr "Κλείδωμα επεξεργαστή κειμένου"
 
@@ -20,17 +20,14 @@
 
 msgid "Choose an image"
 msgstr "Επιλέξατε εικόνα"
 
 msgid "Delete"
 msgstr "Διαγραφή"
 
-msgid "Draft"
-msgstr "Draft"
-
 msgid "Edit"
 msgstr "Επεξεργασία"
 
 msgid "Edit this %s"
 msgstr "Επεξεργαστείτε το %s"
 
 msgid "Edit this document"
@@ -38,26 +35,20 @@
 
 msgid "Edit this image"
 msgstr "Επεξεργασία αυτής της εικόνας"
 
 msgid "Edit this page"
 msgstr "Επεξεργασία αυτής της σελίδας"
 
-msgid "Live"
-msgstr "Live"
-
 msgid "Lock"
 msgstr "Κλείδωμα"
 
 msgid "Preview"
 msgstr "Προεπισκόπηση"
 
-msgid "Published"
-msgstr "Δημοσιεύθηκε"
-
 msgid "Publishing..."
 msgstr "Γίνεται δημοσίευση..."
 
 msgid "Save"
 msgstr "Αποθηκευση"
 
 msgid "Saving..."
```

### Comparing `wagtail-localize-1.5/wagtail_localize/locale/el/LC_MESSAGES/djangojs.po` & `wagtail-localize-1.5.1/wagtail_localize/locale/el/LC_MESSAGES/djangojs.po`

 * *Files 9% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 # Nick Mavrakis <mavrakis.n@gmail.com>, 2021
 # Yiannis Inglessis <negtheone@gmail.com>, 2021
 # fekioh, 2022
 #
 msgid ""
 msgstr ""
 "Last-Translator: fekioh, 2022\n"
-"Language-Team: Greek (https://www.transifex.com/torchbox/teams/8009/el/)\n"
+"Language-Team: Greek (https://app.transifex.com/torchbox/teams/8009/el/)\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Language: el\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
 
 msgid "Apply editor lock"
 msgstr "Κλείδωμα επεξεργαστή κειμένου"
 
@@ -28,17 +28,14 @@
 
 msgid "Choose an image"
 msgstr "Επιλέξατε εικόνα"
 
 msgid "Delete"
 msgstr "Διαγραφή"
 
-msgid "Draft"
-msgstr "Draft"
-
 msgid "Edit"
 msgstr "Επεξεργασία"
 
 msgid "Edit this %s"
 msgstr "Επεξεργαστείτε το %s"
 
 msgid "Edit this document"
@@ -46,26 +43,20 @@
 
 msgid "Edit this image"
 msgstr "Επεξεργασία αυτής της εικόνας"
 
 msgid "Edit this page"
 msgstr "Επεξεργασία αυτής της σελίδας"
 
-msgid "Live"
-msgstr "Live"
-
 msgid "Lock"
 msgstr "Κλείδωμα"
 
 msgid "Preview"
 msgstr "Προεπισκόπηση"
 
-msgid "Published"
-msgstr "Δημοσιεύθηκε"
-
 msgid "Publishing..."
 msgstr "Γίνεται δημοσίευση..."
 
 msgid "Save"
 msgstr "Αποθηκευση"
 
 msgid "Saving..."
```

### Comparing `wagtail-localize-1.5/wagtail_localize/locale/en/LC_MESSAGES/django.po` & `wagtail-localize-1.5.1/wagtail_localize/locale/en/LC_MESSAGES/django.po`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 #
 msgid ""
 msgstr ""
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2023-02-23 14:15+0000\n"
+"POT-Creation-Date: 2023-06-11 10:34+0000\n"
 "Language: en\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "#-#-#-#-#  messages-js.pot  #-#-#-#-#\n"
 "#-#-#-#-#  messages-py.pot  #-#-#-#-#\n"
 
 #: components.py:30 templates/wagtail_localize/admin/_components.html:17
 msgid "Disable"
@@ -22,28 +22,28 @@
 msgstr ""
 
 #: modeladmin/helpers.py:75 modeladmin/helpers.py:78
 #, python-format
 msgid "Sync translated %(model_name)s"
 msgstr ""
 
-#: modeladmin/templates/wagtail_localize/modeladmin/translatable_edit.html:10
+#: modeladmin/templates/wagtail_localize/modeladmin/translatable_edit.html:11
 msgid "Saving…"
 msgstr ""
 
-#: modeladmin/templates/wagtail_localize/modeladmin/translatable_edit.html:11
+#: modeladmin/templates/wagtail_localize/modeladmin/translatable_edit.html:12
 msgid "Save"
 msgstr ""
 
-#: modeladmin/templates/wagtail_localize/modeladmin/translatable_edit.html:21
+#: modeladmin/templates/wagtail_localize/modeladmin/translatable_edit.html:22
 #: wagtail_hooks.py:258 wagtail_hooks.py:345
 msgid "Start Synced translation"
 msgstr ""
 
-#: modeladmin/templates/wagtail_localize/modeladmin/translatable_edit.html:25
+#: modeladmin/templates/wagtail_localize/modeladmin/translatable_edit.html:26
 msgid "Delete"
 msgstr ""
 
 #: modeladmin/templates/wagtail_localize/modeladmin/translatable_index.html:16
 msgid "Download XLSX"
 msgstr ""
```

### Comparing `wagtail-localize-1.5/wagtail_localize/locale/en/LC_MESSAGES/djangojs.po` & `wagtail-localize-1.5.1/wagtail_localize/locale/en/LC_MESSAGES/djangojs.po`

 * *Files 2% similar despite different names*

```diff
@@ -1,37 +1,37 @@
 msgid ""
 msgstr ""
 "Content-Type: text/plain; charset=UTF-8\n"
 
-#: wagtail_localize/static_src/editor/components/TranslationEditor/segments.tsx:859
+#: wagtail_localize/static_src/editor/components/TranslationEditor/segments.tsx:870
 msgid "[DELETED]"
 msgstr ""
 
 #: wagtail_localize/static_src/editor/components/TranslationEditor/footer.tsx:72
 msgid "Apply editor lock"
 msgstr ""
 
-#: wagtail_localize/static_src/editor/components/TranslationEditor/segments.tsx:428
-#: wagtail_localize/static_src/editor/components/TranslationEditor/segments.tsx:601
+#: wagtail_localize/static_src/editor/components/TranslationEditor/segments.tsx:439
+#: wagtail_localize/static_src/editor/components/TranslationEditor/segments.tsx:612
 msgid "Cancel"
 msgstr ""
 
-#: wagtail_localize/static_src/editor/components/TranslationEditor/segments.tsx:743
+#: wagtail_localize/static_src/editor/components/TranslationEditor/segments.tsx:754
 msgid "Change %s"
 msgstr ""
 
-#: wagtail_localize/static_src/editor/components/TranslationEditor/segments.tsx:712
+#: wagtail_localize/static_src/editor/components/TranslationEditor/segments.tsx:723
 msgid "Change document"
 msgstr ""
 
-#: wagtail_localize/static_src/editor/components/TranslationEditor/segments.tsx:681
+#: wagtail_localize/static_src/editor/components/TranslationEditor/segments.tsx:692
 msgid "Change image"
 msgstr ""
 
-#: wagtail_localize/static_src/editor/components/TranslationEditor/segments.tsx:650
+#: wagtail_localize/static_src/editor/components/TranslationEditor/segments.tsx:661
 msgid "Change page"
 msgstr ""
 
 #: wagtail_localize/static_src/editor/components/TranslationEditor/index.tsx:215
 #: wagtail_localize/static_src/editor/components/TranslationEditor/reducer.ts:159
 #: wagtail_localize/static_src/editor/components/TranslationEditor/reducer.ts:181
 msgid "Changed"
@@ -58,25 +58,25 @@
 msgid "Convert to alias page"
 msgstr ""
 
 #: wagtail_localize/static_src/editor/components/TranslationEditor/footer.tsx:54
 msgid "Delete"
 msgstr ""
 
-#: wagtail_localize/static_src/editor/components/TranslationEditor/toolbox.tsx:90
+#: wagtail_localize/static_src/editor/components/TranslationEditor/toolbox.tsx:91
 msgid "Download PO file"
 msgstr ""
 
-#: wagtail_localize/static_src/editor/components/TranslationEditor/toolbox.tsx:83
+#: wagtail_localize/static_src/editor/components/TranslationEditor/toolbox.tsx:84
 msgid "Download PO file and input translations offline"
 msgstr ""
 
-#: wagtail_localize/static_src/editor/components/TranslationEditor/segments.tsx:491
-#: wagtail_localize/static_src/editor/components/TranslationEditor/segments.tsx:625
-#: wagtail_localize/static_src/editor/components/TranslationEditor/segments.tsx:867
+#: wagtail_localize/static_src/editor/components/TranslationEditor/segments.tsx:502
+#: wagtail_localize/static_src/editor/components/TranslationEditor/segments.tsx:636
+#: wagtail_localize/static_src/editor/components/TranslationEditor/segments.tsx:878
 msgid "Edit"
 msgstr ""
 
 #: wagtail_localize/static_src/common/components/SnippetChooser/index.tsx:59
 msgid "Edit this %s"
 msgstr ""
 
@@ -108,50 +108,51 @@
 msgid "Fetching page information..."
 msgstr ""
 
 #: wagtail_localize/static_src/editor/components/TranslationEditor/footer.tsx:75
 msgid "Lock"
 msgstr ""
 
-#: wagtail_localize/static_src/editor/components/TranslationEditor/segments.tsx:842
+#: wagtail_localize/static_src/editor/components/TranslationEditor/segments.tsx:853
 msgid "Not translated"
 msgstr ""
 
 #: wagtail_localize/static_src/common/components/ActionMenu/index.tsx:118
 #: wagtail_localize/static_src/common/components/ActionMenu/index.tsx:139
 msgid "Preview"
 msgstr ""
 
-#: wagtail_localize/static_src/editor/components/TranslationEditor/footer.tsx:134
+#: wagtail_localize/static_src/editor/components/TranslationEditor/footer.tsx:137
 msgid "Publish in "
 msgstr ""
 
 #: wagtail_localize/static_src/editor/components/TranslationEditor/footer.tsx:127
+#: wagtail_localize/static_src/editor/components/TranslationEditor/footer.tsx:130
 msgid "Publishing..."
 msgstr ""
 
 #: wagtail_localize/static_src/editor/components/TranslationEditor/footer.tsx:94
 msgid "Remove editor lock"
 msgstr ""
 
-#: wagtail_localize/static_src/editor/components/TranslationEditor/segments.tsx:768
+#: wagtail_localize/static_src/editor/components/TranslationEditor/segments.tsx:779
 msgid "Revert to %s version"
 msgstr ""
 
-#: wagtail_localize/static_src/editor/components/TranslationEditor/segments.tsx:433
-#: wagtail_localize/static_src/editor/components/TranslationEditor/segments.tsx:604
+#: wagtail_localize/static_src/editor/components/TranslationEditor/segments.tsx:444
+#: wagtail_localize/static_src/editor/components/TranslationEditor/segments.tsx:615
 msgid "Save"
 msgstr ""
 
 #: wagtail_localize/static_src/editor/components/TranslationEditor/reducer.ts:115
-#: wagtail_localize/static_src/editor/components/TranslationEditor/segments.tsx:449
+#: wagtail_localize/static_src/editor/components/TranslationEditor/segments.tsx:460
 msgid "Saving..."
 msgstr ""
 
-#: wagtail_localize/static_src/editor/components/TranslationEditor/segments.tsx:827
+#: wagtail_localize/static_src/editor/components/TranslationEditor/segments.tsx:838
 msgid "segments translated"
 msgstr ""
 
 #: wagtail_localize/static_src/editor/components/TranslationEditor/reducer.ts:145
 msgid "Server error"
 msgstr ""
 
@@ -160,39 +161,39 @@
 msgid "Stop Synced translation"
 msgstr ""
 
 #: wagtail_localize/static_src/editor/components/TranslationEditor/index.tsx:232
 msgid "There are unsaved segments. Please save or cancel them before leaving."
 msgstr ""
 
-#: wagtail_localize/static_src/editor/components/TranslationEditor/segments.tsx:491
-#: wagtail_localize/static_src/editor/components/TranslationEditor/segments.tsx:876
+#: wagtail_localize/static_src/editor/components/TranslationEditor/segments.tsx:502
+#: wagtail_localize/static_src/editor/components/TranslationEditor/segments.tsx:887
 msgid "Translate"
 msgstr ""
 
-#: wagtail_localize/static_src/editor/components/TranslationEditor/toolbox.tsx:134
+#: wagtail_localize/static_src/editor/components/TranslationEditor/toolbox.tsx:135
 msgid "Translate all missing strings with "
 msgstr ""
 
-#: wagtail_localize/static_src/editor/components/TranslationEditor/toolbox.tsx:158
+#: wagtail_localize/static_src/editor/components/TranslationEditor/toolbox.tsx:159
 msgid "Translate with "
 msgstr ""
 
 #: wagtail_localize/static_src/editor/components/TranslationEditor/footer.tsx:97
 msgid "Unlock"
 msgstr ""
 
 #: wagtail_localize/static_src/editor/components/TranslationEditor/footer.tsx:107
 msgid "Unpublish"
 msgstr ""
 
-#: wagtail_localize/static_src/editor/components/TranslationEditor/toolbox.tsx:104
+#: wagtail_localize/static_src/editor/components/TranslationEditor/toolbox.tsx:105
 msgid "Upload PO file"
 msgstr ""
 
-#: wagtail_localize/static_src/editor/components/TranslationEditor/toolbox.tsx:96
+#: wagtail_localize/static_src/editor/components/TranslationEditor/toolbox.tsx:97
 msgid "Upload translated PO file to submit translations"
 msgstr ""
 
-#: wagtail_localize/static_src/editor/components/TranslationEditor/segments.tsx:574
+#: wagtail_localize/static_src/editor/components/TranslationEditor/segments.tsx:585
 msgid "Uses %s version"
 msgstr ""
```

### Comparing `wagtail-localize-1.5/wagtail_localize/locale/es/LC_MESSAGES/django.mo` & `wagtail-localize-1.5.1/wagtail_localize/locale/es/LC_MESSAGES/django.mo`

 * *Files 0% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,12 +1,12 @@
 msgid ""
 msgstr ""
 "Report-Msgid-Bugs-To: \n"
 "Last-Translator: Antoni Aloy <aaloy@apsl.net>, 2022\n"
-"Language-Team: Spanish (https://www.transifex.com/torchbox/teams/8009/es/)\n"
+"Language-Team: Spanish (https://app.transifex.com/torchbox/teams/8009/es/)\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Language: es\n"
 "Plural-Forms: nplurals=3; plural=n == 1 ? 0 : n != 0 && n % 1000000 == 0 ? "
 "1 : 2;\n"
 
 msgid ""
 "<{}> tag is not allowed. Strings can only contain standard HTML inline tags "
```

### Comparing `wagtail-localize-1.5/wagtail_localize/locale/es/LC_MESSAGES/django.po` & `wagtail-localize-1.5.1/wagtail_localize/locale/es/LC_MESSAGES/django.po`

 * *Files 1% similar despite different names*

```diff
@@ -7,17 +7,17 @@
 # José Luis <alagunajs@gmail.com>, 2022
 # X Bello <xbello@gmail.com>, 2022
 # Antoni Aloy <aaloy@apsl.net>, 2022
 #
 msgid ""
 msgstr ""
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2022-10-17 21:00+0000\n"
+"POT-Creation-Date: 2023-02-23 14:15+0000\n"
 "Last-Translator: Antoni Aloy <aaloy@apsl.net>, 2022\n"
-"Language-Team: Spanish (https://www.transifex.com/torchbox/teams/8009/es/)\n"
+"Language-Team: Spanish (https://app.transifex.com/torchbox/teams/8009/es/)\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Language: es\n"
 "Plural-Forms: nplurals=3; plural=n == 1 ? 0 : n != 0 && n % 1000000 == 0 ? "
 "1 : 2;\n"
 
 msgid "Disable"
 msgstr "Deshabilitar"
```

### Comparing `wagtail-localize-1.5/wagtail_localize/locale/es/LC_MESSAGES/djangojs.mo` & `wagtail-localize-1.5.1/wagtail_localize/locale/pt_PT/LC_MESSAGES/djangojs.mo`

 * *Files 20% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,162 +1,147 @@
 msgid ""
 msgstr ""
-"Last-Translator: Amós Oviedo <amos.oviedo@gmail.com>, 2022\n"
-"Language-Team: Spanish (https://www.transifex.com/torchbox/teams/8009/es/)\n"
+"Last-Translator: Tiago Henriques <trinosauro@gmail.com>, 2022\n"
+"Language-Team: Portuguese (Portugal) (https://app.transifex.com/torchbox/"
+"teams/8009/pt_PT/)\n"
 "Content-Type: text/plain; charset=UTF-8\n"
-"Language: es\n"
-"Plural-Forms: nplurals=3; plural=n == 1 ? 0 : n != 0 && n % 1000000 == 0 ? "
-"1 : 2;\n"
+"Language: pt_PT\n"
+"Plural-Forms: nplurals=3; plural=(n == 0 || n == 1) ? 0 : n != 0 && n % "
+"1000000 == 0 ? 1 : 2;\n"
 
 msgid "Apply editor lock"
-msgstr "Aplicar bloqueo del editor"
-
-msgid "Breadcrumb"
-msgstr "Breadcrumb"
+msgstr "Aplicar bloqueio de editor"
 
 msgid "Cancel"
 msgstr "Cancelar"
 
 msgid "Change %s"
-msgstr "Cambiar %s"
+msgstr "Mudar %s"
 
 msgid "Change document"
-msgstr "Cambiar documento"
+msgstr "Mudar documento"
 
 msgid "Change image"
-msgstr "Cambiar imagen"
+msgstr "Mudar imagem"
 
 msgid "Change page"
-msgstr "Cambiar página"
+msgstr "Mudar página"
 
 msgid "Changed"
-msgstr "Cambiado"
+msgstr "Mudado"
 
 msgid "Choose a %s"
-msgstr "Seleccionar un %s"
+msgstr "Escolher um %s"
 
 msgid "Choose a document"
-msgstr "Seleccionar un documento"
+msgstr "Escolher um documento"
 
 msgid "Choose a page"
-msgstr "Seleccionar una página"
+msgstr "Escolher uma página"
 
 msgid "Choose an image"
-msgstr "Seleccionar una imagen"
+msgstr "Escolher uma imagem"
 
 msgid "Convert to alias page"
-msgstr "Convertir a alias de página"
+msgstr "Converter em página de atalho"
 
 msgid "Delete"
-msgstr "Eliminar"
+msgstr "Apagar"
 
 msgid "Download PO file"
-msgstr "Descargar archivo PO"
+msgstr "Descarregar ficheiro PO"
 
 msgid "Download PO file and input translations offline"
-msgstr "Descargar archivo PO y traducir desconectado"
-
-msgid "Draft"
-msgstr "Borrador"
+msgstr "Descarregar ficheiro PO e introduzir traduções em offline"
 
 msgid "Edit"
-msgstr "Editar"
+msgstr "Alterar"
 
 msgid "Edit this %s"
-msgstr "Editar este %s"
+msgstr "Alterar este %s"
 
 msgid "Edit this document"
-msgstr "Editar este docuemento"
+msgstr "Alterar este documento"
 
 msgid "Edit this image"
-msgstr "Editar esta imagen"
+msgstr "Alterar esta imagem"
 
 msgid "Edit this page"
-msgstr "Editar esta página"
+msgstr "Alterar esta página"
 
 msgid "Fetching %s information..."
-msgstr "Obtebiendo información %s..."
+msgstr "A obter informação %s..."
 
 msgid "Fetching document information..."
-msgstr "Obteniendo información del documento..."
+msgstr "A obter informação do documento..."
 
 msgid "Fetching image information..."
-msgstr "Obteniendo información de la imagen..."
+msgstr "A obter informação da imagem..."
 
 msgid "Fetching page information..."
-msgstr "Obteniendo información de la página..."
-
-msgid "Live"
-msgstr "En vivo"
+msgstr "A obter informação da página..."
 
 msgid "Lock"
 msgstr "Bloquear"
 
 msgid "Not translated"
-msgstr "Sin traducir"
+msgstr "Por traduzir"
 
 msgid "Preview"
-msgstr "Vista previa"
+msgstr "Visualizar"
 
 msgid "Publish in "
-msgstr "Publicar en"
-
-msgid "Published"
-msgstr "Publicado"
-
-msgid "Published on "
-msgstr "Publicado en"
+msgstr "Publicar em"
 
 msgid "Publishing..."
-msgstr "Publicando..."
+msgstr "A publicar..."
 
 msgid "Remove editor lock"
-msgstr "Eliminar bloqueo del editor"
+msgstr "Retirar bloqueio de editor"
 
 msgid "Revert to %s version"
-msgstr "Revertir a versión %s"
+msgstr "Reverter à versão %s "
 
 msgid "Save"
-msgstr "Guardar"
+msgstr "Gravar"
 
 msgid "Saving..."
-msgstr "Guardando..."
+msgstr "A gravar..."
 
 msgid "Server error"
-msgstr "Error del servidor"
+msgstr "Erro de servidor"
 
 msgid "Stop Synced translation"
-msgstr "Parar traducción sincronizada"
+msgstr "Parar tradução Sincronizada"
 
 msgid "There are unsaved segments. Please save or cancel them before leaving."
-msgstr ""
-"Hay segmentos sin guardar. Por favor, guárdalos o cancélalos antes de salir."
+msgstr "Existem segmentos por gravar. Grave ou cancele-os antes de sair."
 
 msgid "Translate"
-msgstr "Traducir"
+msgstr "Traduzir"
 
 msgid "Translate all missing strings with "
-msgstr "Traducir todas las cadenas faltantes con"
+msgstr "Traduzir todos os segmentos de texto em falta com"
 
 msgid "Translate with "
-msgstr "Traducir con"
+msgstr "Traduzir com"
 
 msgid "Unlock"
 msgstr "Desbloquear"
 
 msgid "Unpublish"
 msgstr "Despublicar"
 
 msgid "Upload PO file"
-msgstr "Cargar archivo PO"
+msgstr "Carregar ficheiro PO"
 
 msgid "Upload translated PO file to submit translations"
-msgstr "Cargar archivo PO traducido para enviar traducciones"
+msgstr "Carregar ficheiro PO traduzido para enviar traduções"
 
 msgid "Uses %s version"
-msgstr "Usa versión %s"
+msgstr "Utiliza a versão %s"
 
 msgid "[DELETED]"
-msgstr "[ELIMINADO]"
+msgstr "[APAGADO]"
 
 msgid "segments translated"
-msgstr "segmentos traducidos"
+msgstr "segmentos traduzidos"
```

### Comparing `wagtail-localize-1.5/wagtail_localize/locale/es/LC_MESSAGES/djangojs.po` & `wagtail-localize-1.5.1/wagtail_localize/locale/es/LC_MESSAGES/djangojs.po`

 * *Files 9% similar despite different names*

```diff
@@ -3,29 +3,26 @@
 # José Luis <alagunajs@gmail.com>, 2021
 # Kevin Gutiérrez, 2021
 # Amós Oviedo <amos.oviedo@gmail.com>, 2022
 #
 msgid ""
 msgstr ""
 "Last-Translator: Amós Oviedo <amos.oviedo@gmail.com>, 2022\n"
-"Language-Team: Spanish (https://www.transifex.com/torchbox/teams/8009/es/)\n"
+"Language-Team: Spanish (https://app.transifex.com/torchbox/teams/8009/es/)\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Language: es\n"
 "Plural-Forms: nplurals=3; plural=n == 1 ? 0 : n != 0 && n % 1000000 == 0 ? "
 "1 : 2;\n"
 
 msgid "[DELETED]"
 msgstr "[ELIMINADO]"
 
 msgid "Apply editor lock"
 msgstr "Aplicar bloqueo del editor"
 
-msgid "Breadcrumb"
-msgstr "Breadcrumb"
-
 msgid "Cancel"
 msgstr "Cancelar"
 
 msgid "Change %s"
 msgstr "Cambiar %s"
 
 msgid "Change document"
@@ -60,17 +57,14 @@
 
 msgid "Download PO file"
 msgstr "Descargar archivo PO"
 
 msgid "Download PO file and input translations offline"
 msgstr "Descargar archivo PO y traducir desconectado"
 
-msgid "Draft"
-msgstr "Borrador"
-
 msgid "Edit"
 msgstr "Editar"
 
 msgid "Edit this %s"
 msgstr "Editar este %s"
 
 msgid "Edit this document"
@@ -90,35 +84,26 @@
 
 msgid "Fetching image information..."
 msgstr "Obteniendo información de la imagen..."
 
 msgid "Fetching page information..."
 msgstr "Obteniendo información de la página..."
 
-msgid "Live"
-msgstr "En vivo"
-
 msgid "Lock"
 msgstr "Bloquear"
 
 msgid "Not translated"
 msgstr "Sin traducir"
 
 msgid "Preview"
 msgstr "Vista previa"
 
 msgid "Publish in "
 msgstr "Publicar en"
 
-msgid "Published"
-msgstr "Publicado"
-
-msgid "Published on "
-msgstr "Publicado en"
-
 msgid "Publishing..."
 msgstr "Publicando..."
 
 msgid "Remove editor lock"
 msgstr "Eliminar bloqueo del editor"
 
 msgid "Revert to %s version"
```

### Comparing `wagtail-localize-1.5/wagtail_localize/locale/et/LC_MESSAGES/django.mo` & `wagtail-localize-1.5.1/wagtail_localize/locale/et/LC_MESSAGES/django.mo`

 * *Files 2% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,12 +1,12 @@
 msgid ""
 msgstr ""
 "Report-Msgid-Bugs-To: \n"
 "Last-Translator: Erlend <debcf78e@opayq.com>, 2022\n"
-"Language-Team: Estonian (https://www.transifex.com/torchbox/teams/8009/et/)\n"
+"Language-Team: Estonian (https://app.transifex.com/torchbox/teams/8009/et/)\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Language: et\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
 
 msgid "Content"
 msgstr "Sisu"
```

### Comparing `wagtail-localize-1.5/wagtail_localize/locale/et/LC_MESSAGES/django.po` & `wagtail-localize-1.5.1/wagtail_localize/locale/et/LC_MESSAGES/django.po`

 * *Files 4% similar despite different names*

```diff
@@ -2,17 +2,17 @@
 # Translators:
 # Ragnar Rebase <rrebase@gmail.com>, 2021
 # Erlend <debcf78e@opayq.com>, 2022
 #
 msgid ""
 msgstr ""
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2022-10-17 21:00+0000\n"
+"POT-Creation-Date: 2023-02-23 14:15+0000\n"
 "Last-Translator: Erlend <debcf78e@opayq.com>, 2022\n"
-"Language-Team: Estonian (https://www.transifex.com/torchbox/teams/8009/et/)\n"
+"Language-Team: Estonian (https://app.transifex.com/torchbox/teams/8009/et/)\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Language: et\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
 
 msgid "Disable"
 msgstr "Keela"
```

### Comparing `wagtail-localize-1.5/wagtail_localize/locale/et/LC_MESSAGES/djangojs.mo` & `wagtail-localize-1.5.1/wagtail_localize/locale/vi/LC_MESSAGES/djangojs.mo`

 * *Files 24% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,70 +1,80 @@
 msgid ""
 msgstr ""
-"Last-Translator: Erlend <debcf78e@opayq.com>, 2021\n"
-"Language-Team: Estonian (https://www.transifex.com/torchbox/teams/8009/et/)\n"
+"Last-Translator: Vu Pham, 2022\n"
+"Language-Team: Vietnamese (https://app.transifex.com/torchbox/teams/8009/"
+"vi/)\n"
 "Content-Type: text/plain; charset=UTF-8\n"
-"Language: et\n"
-"Plural-Forms: nplurals=2; plural=(n != 1);\n"
+"Language: vi\n"
+"Plural-Forms: nplurals=1; plural=0;\n"
 
-msgid "Apply editor lock"
-msgstr "Rakenda redaktori lukustus"
+msgid "Cancel"
+msgstr "Hủy bỏ"
 
-msgid "Breadcrumb"
-msgstr "Riivsai"
+msgid "Change %s"
+msgstr "Thay đổi %s"
 
-msgid "Cancel"
-msgstr "Tühista"
+msgid "Change document"
+msgstr "Thay đổi văn bản"
 
 msgid "Change image"
-msgstr "Muuda pilti"
+msgstr "Thay đổi hình ảnh"
+
+msgid "Change page"
+msgstr "Thay đổi trang"
+
+msgid "Changed"
+msgstr "Đã thay đổi"
+
+msgid "Choose a %s"
+msgstr "Chọn một %s"
 
 msgid "Choose a document"
-msgstr "Valige dokument"
+msgstr "Chọn một văn bản"
 
 msgid "Choose a page"
-msgstr "Valige leht"
+msgstr "Chọn một trang"
 
 msgid "Choose an image"
-msgstr "Valige pilt"
+msgstr "Chọn một hình ảnh"
 
 msgid "Delete"
-msgstr "Kustuta"
-
-msgid "Draft"
-msgstr "Mustand"
+msgstr "Xoá"
 
 msgid "Edit"
-msgstr "Muuda"
+msgstr "Biên tập"
 
 msgid "Edit this %s"
-msgstr "Muutke seda %s"
+msgstr "Biên tập %s này"
 
 msgid "Edit this document"
-msgstr "Muutke seda dokumenti"
-
-msgid "Edit this image"
-msgstr "Muutke seda pilti"
-
-msgid "Edit this page"
-msgstr "Muutke seda lehte"
-
-msgid "Live"
-msgstr "Otseülekanne"
+msgstr "Biên tập văn bản này"
 
 msgid "Lock"
-msgstr "Lukusta"
+msgstr "Khóa"
 
 msgid "Preview"
-msgstr "Eelvaade"
+msgstr "Xem trước"
 
-msgid "Published"
-msgstr "Avaldatud"
+msgid "Publishing..."
+msgstr "Đang xuất bản..."
 
 msgid "Save"
-msgstr "Salvesta"
+msgstr "Lưu"
+
+msgid "Saving..."
+msgstr "Đang lưu..."
+
+msgid "Translate"
+msgstr "Dịch"
+
+msgid "Translate with "
+msgstr "Dịch với"
 
 msgid "Unlock"
-msgstr "Ava"
+msgstr "Mở khóa"
 
 msgid "Unpublish"
-msgstr "Tühista avaldamine"
+msgstr "Thu hồi xuất bản"
+
+msgid "[DELETED]"
+msgstr "[ĐÃ XÓA]"
```

### Comparing `wagtail-localize-1.5/wagtail_localize/locale/et/LC_MESSAGES/djangojs.po` & `wagtail-localize-1.5.1/wagtail_localize/locale/et/LC_MESSAGES/djangojs.po`

 * *Files 12% similar despite different names*

```diff
@@ -1,26 +1,22 @@
 #
 # Translators:
-# Ragnar Rebase <rrebase@gmail.com>, 2021
 # Erlend <debcf78e@opayq.com>, 2021
 #
 msgid ""
 msgstr ""
 "Last-Translator: Erlend <debcf78e@opayq.com>, 2021\n"
-"Language-Team: Estonian (https://www.transifex.com/torchbox/teams/8009/et/)\n"
+"Language-Team: Estonian (https://app.transifex.com/torchbox/teams/8009/et/)\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Language: et\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
 
 msgid "Apply editor lock"
 msgstr "Rakenda redaktori lukustus"
 
-msgid "Breadcrumb"
-msgstr "Riivsai"
-
 msgid "Cancel"
 msgstr "Tühista"
 
 msgid "Change image"
 msgstr "Muuda pilti"
 
 msgid "Choose a document"
@@ -31,17 +27,14 @@
 
 msgid "Choose an image"
 msgstr "Valige pilt"
 
 msgid "Delete"
 msgstr "Kustuta"
 
-msgid "Draft"
-msgstr "Mustand"
-
 msgid "Edit"
 msgstr "Muuda"
 
 msgid "Edit this %s"
 msgstr "Muutke seda %s"
 
 msgid "Edit this document"
@@ -49,26 +42,20 @@
 
 msgid "Edit this image"
 msgstr "Muutke seda pilti"
 
 msgid "Edit this page"
 msgstr "Muutke seda lehte"
 
-msgid "Live"
-msgstr "Otseülekanne"
-
 msgid "Lock"
 msgstr "Lukusta"
 
 msgid "Preview"
 msgstr "Eelvaade"
 
-msgid "Published"
-msgstr "Avaldatud"
-
 msgid "Save"
 msgstr "Salvesta"
 
 msgid "Unlock"
 msgstr "Ava"
 
 msgid "Unpublish"
```

### Comparing `wagtail-localize-1.5/wagtail_localize/locale/eu/LC_MESSAGES/django.po` & `wagtail-localize-1.5.1/wagtail_localize/locale/eu/LC_MESSAGES/django.po`

 * *Files 5% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 #
 # Translators:
 # 67feb0cba3962a6c9f09eb0e43697461_528661a <cbde1c637170da616adcdde6daca673c_96059>, 2022
 #
 msgid ""
 msgstr ""
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2022-10-17 21:00+0000\n"
+"POT-Creation-Date: 2023-02-23 14:15+0000\n"
 "Last-Translator: 67feb0cba3962a6c9f09eb0e43697461_528661a "
 "<cbde1c637170da616adcdde6daca673c_96059>, 2022\n"
-"Language-Team: Basque (https://www.transifex.com/torchbox/teams/8009/eu/)\n"
+"Language-Team: Basque (https://app.transifex.com/torchbox/teams/8009/eu/)\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Language: eu\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
 
 msgid "Delete"
 msgstr "Ezabatu"
```

### Comparing `wagtail-localize-1.5/wagtail_localize/locale/eu/LC_MESSAGES/djangojs.mo` & `wagtail-localize-1.5.1/wagtail_localize/locale/eu/LC_MESSAGES/djangojs.mo`

 * *Files 2% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,12 +1,12 @@
 msgid ""
 msgstr ""
 "Last-Translator: 67feb0cba3962a6c9f09eb0e43697461_528661a "
 "<cbde1c637170da616adcdde6daca673c_96059>, 2021\n"
-"Language-Team: Basque (https://www.transifex.com/torchbox/teams/8009/eu/)\n"
+"Language-Team: Basque (https://app.transifex.com/torchbox/teams/8009/eu/)\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Language: eu\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
 
 msgid "Choose a page"
 msgstr "Orrialde bat aukeratu"
```

### Comparing `wagtail-localize-1.5/wagtail_localize/locale/eu/LC_MESSAGES/djangojs.po` & `wagtail-localize-1.5.1/wagtail_localize/locale/eu/LC_MESSAGES/djangojs.po`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # Translators:
 # 67feb0cba3962a6c9f09eb0e43697461_528661a <cbde1c637170da616adcdde6daca673c_96059>, 2021
 #
 msgid ""
 msgstr ""
 "Last-Translator: 67feb0cba3962a6c9f09eb0e43697461_528661a "
 "<cbde1c637170da616adcdde6daca673c_96059>, 2021\n"
-"Language-Team: Basque (https://www.transifex.com/torchbox/teams/8009/eu/)\n"
+"Language-Team: Basque (https://app.transifex.com/torchbox/teams/8009/eu/)\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Language: eu\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
 
 msgid "Choose a page"
 msgstr "Orrialde bat aukeratu"
```

### Comparing `wagtail-localize-1.5/wagtail_localize/locale/fa/LC_MESSAGES/django.mo` & `wagtail-localize-1.5.1/wagtail_localize/locale/fa/LC_MESSAGES/django.mo`

 * *Files 2% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,12 +1,12 @@
 msgid ""
 msgstr ""
 "Report-Msgid-Bugs-To: \n"
 "Last-Translator: Amir Mahmoodi, 2023\n"
-"Language-Team: Persian (https://www.transifex.com/torchbox/teams/8009/fa/)\n"
+"Language-Team: Persian (https://app.transifex.com/torchbox/teams/8009/fa/)\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Language: fa\n"
 "Plural-Forms: nplurals=2; plural=(n > 1);\n"
 
 msgid "Content"
 msgstr "محتوا"
```

### Comparing `wagtail-localize-1.5/wagtail_localize/locale/fa/LC_MESSAGES/django.po` & `wagtail-localize-1.5.1/wagtail_localize/locale/fa/LC_MESSAGES/django.po`

 * *Files 13% similar despite different names*

```diff
@@ -4,17 +4,17 @@
 # Mostafa Heidarian <tabvar@gmail.com>, 2022
 # Ehsan jahanbakhsh <man207ej@gmail.com>, 2022
 # Amir Mahmoodi, 2023
 #
 msgid ""
 msgstr ""
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2022-10-17 21:00+0000\n"
+"POT-Creation-Date: 2023-02-23 14:15+0000\n"
 "Last-Translator: Amir Mahmoodi, 2023\n"
-"Language-Team: Persian (https://www.transifex.com/torchbox/teams/8009/fa/)\n"
+"Language-Team: Persian (https://app.transifex.com/torchbox/teams/8009/fa/)\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Language: fa\n"
 "Plural-Forms: nplurals=2; plural=(n > 1);\n"
 
 msgid "Saving…"
 msgstr "در حال ذخیره سازی"
```

### Comparing `wagtail-localize-1.5/wagtail_localize/locale/fa/LC_MESSAGES/djangojs.mo` & `wagtail-localize-1.5.1/wagtail_localize/locale/fa/LC_MESSAGES/djangojs.mo`

 * *Files 15% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,21 +1,18 @@
 msgid ""
 msgstr ""
 "Last-Translator: pyzenberg <pyzenberg@gmail.com>, 2021\n"
-"Language-Team: Persian (https://www.transifex.com/torchbox/teams/8009/fa/)\n"
+"Language-Team: Persian (https://app.transifex.com/torchbox/teams/8009/fa/)\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Language: fa\n"
 "Plural-Forms: nplurals=2; plural=(n > 1);\n"
 
 msgid "Apply editor lock"
 msgstr "گذاشتن قفل ویراستاری"
 
-msgid "Breadcrumb"
-msgstr "خرده نان"
-
 msgid "Cancel"
 msgstr "انصراف"
 
 msgid "Change image"
 msgstr "تغییر تصویر"
 
 msgid "Changed"
@@ -29,17 +26,14 @@
 
 msgid "Choose an image"
 msgstr "تصویر را انتخاب کنید"
 
 msgid "Delete"
 msgstr "حذف"
 
-msgid "Draft"
-msgstr "پیشنویس"
-
 msgid "Edit"
 msgstr "ویرایش"
 
 msgid "Edit this %s"
 msgstr "ویرایش این %s"
 
 msgid "Edit this document"
@@ -47,17 +41,14 @@
 
 msgid "Edit this image"
 msgstr "ویرایش این تصویر"
 
 msgid "Edit this page"
 msgstr "ویرایش این صفحه"
 
-msgid "Live"
-msgstr "منتشر شده"
-
 msgid "Lock"
 msgstr "قفل"
 
 msgid "Preview"
 msgstr "پیش‌نمایش"
 
 msgid "Publishing..."
```

### Comparing `wagtail-localize-1.5/wagtail_localize/locale/fa/LC_MESSAGES/djangojs.po` & `wagtail-localize-1.5.1/wagtail_localize/locale/fa/LC_MESSAGES/djangojs.po`

 * *Files 21% similar despite different names*

```diff
@@ -4,28 +4,25 @@
 # Mohammad Hossein Mojtahedi <Mhm5000@gmail.com>, 2021
 # Ehsan jahanbakhsh <man207ej@gmail.com>, 2021
 # pyzenberg <pyzenberg@gmail.com>, 2021
 #
 msgid ""
 msgstr ""
 "Last-Translator: pyzenberg <pyzenberg@gmail.com>, 2021\n"
-"Language-Team: Persian (https://www.transifex.com/torchbox/teams/8009/fa/)\n"
+"Language-Team: Persian (https://app.transifex.com/torchbox/teams/8009/fa/)\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Language: fa\n"
 "Plural-Forms: nplurals=2; plural=(n > 1);\n"
 
 msgid "[DELETED]"
 msgstr "[حذف شده]"
 
 msgid "Apply editor lock"
 msgstr "گذاشتن قفل ویراستاری"
 
-msgid "Breadcrumb"
-msgstr "خرده نان"
-
 msgid "Cancel"
 msgstr "انصراف"
 
 msgid "Change image"
 msgstr "تغییر تصویر"
 
 msgid "Changed"
@@ -39,17 +36,14 @@
 
 msgid "Choose an image"
 msgstr "تصویر را انتخاب کنید"
 
 msgid "Delete"
 msgstr "حذف"
 
-msgid "Draft"
-msgstr "پیشنویس"
-
 msgid "Edit"
 msgstr "ویرایش"
 
 msgid "Edit this %s"
 msgstr "ویرایش این %s"
 
 msgid "Edit this document"
@@ -57,17 +51,14 @@
 
 msgid "Edit this image"
 msgstr "ویرایش این تصویر"
 
 msgid "Edit this page"
 msgstr "ویرایش این صفحه"
 
-msgid "Live"
-msgstr "منتشر شده"
-
 msgid "Lock"
 msgstr "قفل"
 
 msgid "Preview"
 msgstr "پیش‌نمایش"
 
 msgid "Publishing..."
```

### Comparing `wagtail-localize-1.5/wagtail_localize/locale/fi/LC_MESSAGES/django.mo` & `wagtail-localize-1.5.1/wagtail_localize/locale/fi/LC_MESSAGES/django.mo`

 * *Files 3% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,12 +1,12 @@
 msgid ""
 msgstr ""
 "Report-Msgid-Bugs-To: \n"
 "Last-Translator: Jiri Grönroos <jiri.gronroos@iki.fi>, 2022\n"
-"Language-Team: Finnish (https://www.transifex.com/torchbox/teams/8009/fi/)\n"
+"Language-Team: Finnish (https://app.transifex.com/torchbox/teams/8009/fi/)\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Language: fi\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
 
 msgid "All child pages will be created."
 msgstr "Kaikki lapsisivut luodaan."
```

### Comparing `wagtail-localize-1.5/wagtail_localize/locale/fi/LC_MESSAGES/django.po` & `wagtail-localize-1.5.1/wagtail_localize/locale/fi/LC_MESSAGES/django.po`

 * *Files 1% similar despite different names*

```diff
@@ -4,17 +4,17 @@
 # Glen Somerville <glen.somerville@gmail.com>, 2021
 # Valter Maasalo <vmaasalo@gmail.com>, 2022
 # Jiri Grönroos <jiri.gronroos@iki.fi>, 2022
 #
 msgid ""
 msgstr ""
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2022-10-17 21:00+0000\n"
+"POT-Creation-Date: 2023-02-23 14:15+0000\n"
 "Last-Translator: Jiri Grönroos <jiri.gronroos@iki.fi>, 2022\n"
-"Language-Team: Finnish (https://www.transifex.com/torchbox/teams/8009/fi/)\n"
+"Language-Team: Finnish (https://app.transifex.com/torchbox/teams/8009/fi/)\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Language: fi\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
 
 msgid "Disable"
 msgstr "Poista käytöstä"
```

### Comparing `wagtail-localize-1.5/wagtail_localize/locale/fi/LC_MESSAGES/djangojs.mo` & `wagtail-localize-1.5.1/wagtail_localize/locale/nl_NL/LC_MESSAGES/djangojs.mo`

 * *Files 20% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,143 +1,143 @@
 msgid ""
 msgstr ""
-"Last-Translator: Jiri Grönroos <jiri.gronroos@iki.fi>, 2022\n"
-"Language-Team: Finnish (https://www.transifex.com/torchbox/teams/8009/fi/)\n"
+"Last-Translator: Coen van der Kamp <cvanderkamp@gmail.com>, 2021\n"
+"Language-Team: Dutch (Netherlands) (https://www.transifex.com/torchbox/"
+"teams/8009/nl_NL/)\n"
 "Content-Type: text/plain; charset=UTF-8\n"
-"Language: fi\n"
+"Language: nl_NL\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
 
 msgid "Apply editor lock"
-msgstr "Toteuta editorin lukitus"
+msgstr "Pas bewerkingsblokkade toe"
 
 msgid "Breadcrumb"
-msgstr "Linkkipolku"
+msgstr "Broodkruimel"
 
 msgid "Cancel"
-msgstr "Peruuta"
-
-msgid "Change %s"
-msgstr "Vaihda %s"
+msgstr "Annuleren"
 
 msgid "Change document"
-msgstr "Vaihda dokumentti"
+msgstr "Wijzig document"
 
 msgid "Change image"
-msgstr "Vaihda kuva"
+msgstr "Wijzig afbeelding"
 
 msgid "Change page"
-msgstr "Vaihda sivu"
+msgstr "Wijzig pagina"
 
 msgid "Changed"
-msgstr "Vaihdettu"
-
-msgid "Choose a %s"
-msgstr "Valitse %s"
+msgstr "Gewijzigd"
 
 msgid "Choose a document"
-msgstr "Valitse dokumentti"
+msgstr "Kies een document"
 
 msgid "Choose a page"
-msgstr "Valitse sivu"
+msgstr "Kies een pagina"
 
 msgid "Choose an image"
-msgstr "Valitse kuva"
-
-msgid "Convert to alias page"
-msgstr "Muunna aliassivuksi"
+msgstr "Kies een afbeelding"
 
 msgid "Delete"
-msgstr "Poista"
+msgstr "Verwijderen"
 
 msgid "Download PO file"
-msgstr "Lataa PO-tiedosto"
+msgstr "Download PO-bestand"
 
 msgid "Download PO file and input translations offline"
-msgstr "Lataa PO-tiedosto ja syötä käännökset offline-tilassa"
+msgstr "Download PO-bestand en voer offline vertalingen in"
 
 msgid "Draft"
-msgstr "Luonnos"
+msgstr "Concept"
 
 msgid "Edit"
-msgstr "Muokkaa"
+msgstr "Bewerk"
 
 msgid "Edit this %s"
-msgstr "Muokkaa %s-kohdetta"
+msgstr "Wijzig %s"
 
 msgid "Edit this document"
-msgstr "Muokkaa tätä dokumenttia"
+msgstr "Bewerk dit document"
 
 msgid "Edit this image"
-msgstr "Muokkaa tätä kuvaa"
+msgstr "Bewerk deze afbeelding"
 
 msgid "Edit this page"
-msgstr "Muokkaa tätä sivua"
+msgstr "Bewerk deze pagina"
 
 msgid "Fetching document information..."
-msgstr "Noudetaan dokumentin tietoja..."
+msgstr "Bezig met ophalen van documentgegevens..."
 
 msgid "Fetching image information..."
-msgstr "Noudetaan kuvan tietoja..."
+msgstr "Bezig met ophalen van afbeeldingsgegevens..."
 
 msgid "Fetching page information..."
-msgstr "Noudetaan sivun tietoja..."
+msgstr "Bezig met ophalen van paginagegevens..."
 
 msgid "Live"
-msgstr "Julkinen"
+msgstr "Openbaar"
 
 msgid "Lock"
-msgstr "Lukitse"
+msgstr "Vergrendel"
 
 msgid "Not translated"
-msgstr "Ei käännetty"
+msgstr "Niet vertaald"
 
 msgid "Preview"
-msgstr "Esikatsele"
+msgstr "Voorvertoning"
+
+msgid "Publish in "
+msgstr "Publiceer in"
 
 msgid "Published"
-msgstr "Julkaistu"
+msgstr "Gepubliceerd"
 
 msgid "Published on "
-msgstr "Julkaistu"
+msgstr "Gepubliceerd op"
 
 msgid "Publishing..."
-msgstr "Julkaistaan..."
+msgstr "Bezig met publiceren..."
 
 msgid "Remove editor lock"
-msgstr "Poista editorin lukitus"
+msgstr "Verwijder bewerkingsblokkade"
 
 msgid "Save"
-msgstr "Tallenna"
+msgstr "Opslaan"
 
 msgid "Saving..."
-msgstr "Tallennetaan..."
+msgstr "Bezig met opslaan..."
 
 msgid "Server error"
-msgstr "Palvelinvirhe"
+msgstr "Server error"
 
-msgid "There are unsaved segments. Please save or cancel them before leaving."
-msgstr ""
-"Tallentamattomia segmenttejä. Tallenna ne tai peruuta ennen poistumista."
+msgid "Stop translation"
+msgstr "Stop vertaling"
 
 msgid "Translate"
-msgstr "Käännä"
+msgstr "Vertaal"
+
+msgid "Translate all missing strings with "
+msgstr "Vertaal alle ontbrekende teksten met"
 
 msgid "Translate with "
-msgstr "Käännä käyttäen"
+msgstr "Vertaal met"
 
 msgid "Unlock"
-msgstr "Avaa lukitus"
+msgstr "Ontgrendelen"
 
 msgid "Unpublish"
-msgstr "Piilota"
+msgstr "Depubliceren"
 
 msgid "Upload PO file"
-msgstr "Lähetä PO-tiedosto"
+msgstr "Upload PO-bestand"
 
 msgid "Upload translated PO file to submit translations"
-msgstr "Lähetä käännetty PO-tiedosto lähettääksesi käännökset"
+msgstr "Upload vertaald PO-bestand om vertalingen te verzenden"
+
+msgid "Uses %s version"
+msgstr "Gebruikt %s versie"
 
 msgid "[DELETED]"
-msgstr "[POISTETTU]"
+msgstr "[VERWIJDERD]"
 
 msgid "segments translated"
-msgstr "segmenttiä käännetty"
+msgstr "vertaalde segmenten"
```

### Comparing `wagtail-localize-1.5/wagtail_localize/locale/fi/LC_MESSAGES/djangojs.po` & `wagtail-localize-1.5.1/wagtail_localize/locale/sv/LC_MESSAGES/djangojs.po`

 * *Files 22% similar despite different names*

```diff
@@ -1,149 +1,153 @@
 #
 # Translators:
-# Valter Maasalo <vmaasalo@gmail.com>, 2021
-# Aarni Koskela, 2021
-# Jiri Grönroos <jiri.gronroos@iki.fi>, 2022
+# Martin Sandström <martin@marteinn.se>, 2021
+# Thomas Kunambi <kunambi@gmail.com>, 2021
+# Philip Andersen <renegadevi@codeofmagi.net>, 2022
 #
 msgid ""
 msgstr ""
-"Last-Translator: Jiri Grönroos <jiri.gronroos@iki.fi>, 2022\n"
-"Language-Team: Finnish (https://www.transifex.com/torchbox/teams/8009/fi/)\n"
+"Last-Translator: Philip Andersen <renegadevi@codeofmagi.net>, 2022\n"
+"Language-Team: Swedish (https://app.transifex.com/torchbox/teams/8009/sv/)\n"
 "Content-Type: text/plain; charset=UTF-8\n"
-"Language: fi\n"
+"Language: sv\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
 
 msgid "[DELETED]"
-msgstr "[POISTETTU]"
+msgstr "[RADERAD]"
 
 msgid "Apply editor lock"
-msgstr "Toteuta editorin lukitus"
-
-msgid "Breadcrumb"
-msgstr "Linkkipolku"
+msgstr "Tillämpa redaktörslås"
 
 msgid "Cancel"
-msgstr "Peruuta"
+msgstr "Avbryt"
 
 msgid "Change %s"
-msgstr "Vaihda %s"
+msgstr "Ändra %s"
 
 msgid "Change document"
-msgstr "Vaihda dokumentti"
+msgstr "Ändra dokument"
 
 msgid "Change image"
-msgstr "Vaihda kuva"
+msgstr "Ändra bild"
 
 msgid "Change page"
-msgstr "Vaihda sivu"
+msgstr "Ändra sida"
 
 msgid "Changed"
-msgstr "Vaihdettu"
+msgstr "Ändrad"
 
 msgid "Choose a %s"
-msgstr "Valitse %s"
+msgstr "Välj en %s"
 
 msgid "Choose a document"
-msgstr "Valitse dokumentti"
+msgstr "Välj ett dokument"
 
 msgid "Choose a page"
-msgstr "Valitse sivu"
+msgstr "Välj en sida"
 
 msgid "Choose an image"
-msgstr "Valitse kuva"
+msgstr "Välj en bild"
 
 msgid "Convert to alias page"
-msgstr "Muunna aliassivuksi"
+msgstr "Konvertera till alias"
 
 msgid "Delete"
-msgstr "Poista"
+msgstr "Radera"
 
 msgid "Download PO file"
-msgstr "Lataa PO-tiedosto"
+msgstr "Ladda ner PO fil"
 
 msgid "Download PO file and input translations offline"
-msgstr "Lataa PO-tiedosto ja syötä käännökset offline-tilassa"
-
-msgid "Draft"
-msgstr "Luonnos"
+msgstr "Ladda ner PO fil och uppdatera översättningar offline"
 
 msgid "Edit"
-msgstr "Muokkaa"
+msgstr "Redigera"
 
 msgid "Edit this %s"
-msgstr "Muokkaa %s-kohdetta"
+msgstr "Redigera %s"
 
 msgid "Edit this document"
-msgstr "Muokkaa tätä dokumenttia"
+msgstr "Redigera detta dokument"
 
 msgid "Edit this image"
-msgstr "Muokkaa tätä kuvaa"
+msgstr "Redigera denna bild"
 
 msgid "Edit this page"
-msgstr "Muokkaa tätä sivua"
+msgstr "Redigera denna sida"
+
+msgid "Fetching %s information..."
+msgstr "Hämtar %s information..."
 
 msgid "Fetching document information..."
-msgstr "Noudetaan dokumentin tietoja..."
+msgstr "Hämtar dokumentinformation"
 
 msgid "Fetching image information..."
-msgstr "Noudetaan kuvan tietoja..."
+msgstr "Hämtar bildinformation"
 
 msgid "Fetching page information..."
-msgstr "Noudetaan sivun tietoja..."
-
-msgid "Live"
-msgstr "Julkinen"
+msgstr "Hämtar sidoinformation"
 
 msgid "Lock"
-msgstr "Lukitse"
+msgstr "Lås"
 
 msgid "Not translated"
-msgstr "Ei käännetty"
+msgstr "Inte översatt"
 
 msgid "Preview"
-msgstr "Esikatsele"
-
-msgid "Published"
-msgstr "Julkaistu"
+msgstr "Förhandsgranska"
 
-msgid "Published on "
-msgstr "Julkaistu"
+msgid "Publish in "
+msgstr "Publicera på"
 
 msgid "Publishing..."
-msgstr "Julkaistaan..."
+msgstr "Publicerar..."
 
 msgid "Remove editor lock"
-msgstr "Poista editorin lukitus"
+msgstr "Ta bort redaktörslås"
+
+msgid "Revert to %s version"
+msgstr "Återställ till %s version"
 
 msgid "Save"
-msgstr "Tallenna"
+msgstr "Spara"
 
 msgid "Saving..."
-msgstr "Tallennetaan..."
+msgstr "Sparar..."
 
 msgid "segments translated"
-msgstr "segmenttiä käännetty"
+msgstr "segment översatta"
 
 msgid "Server error"
-msgstr "Palvelinvirhe"
+msgstr "Serverfel"
+
+msgid "Stop Synced translation"
+msgstr "Stoppa synkroniserad översättning"
 
 msgid "There are unsaved segments. Please save or cancel them before leaving."
 msgstr ""
-"Tallentamattomia segmenttejä. Tallenna ne tai peruuta ennen poistumista."
+"Det finns osparade segment. Vänligen spara eller återställ dem innan du "
+"lämnar."
 
 msgid "Translate"
-msgstr "Käännä"
+msgstr "Översätt"
+
+msgid "Translate all missing strings with "
+msgstr "Översätt alla saknade strängar med"
 
 msgid "Translate with "
-msgstr "Käännä käyttäen"
+msgstr "Översätt med"
 
 msgid "Unlock"
-msgstr "Avaa lukitus"
+msgstr "Lås upp"
 
 msgid "Unpublish"
-msgstr "Piilota"
+msgstr "Avpublicera"
 
 msgid "Upload PO file"
-msgstr "Lähetä PO-tiedosto"
+msgstr "Ladda upp PO fil"
 
 msgid "Upload translated PO file to submit translations"
-msgstr "Lähetä käännetty PO-tiedosto lähettääksesi käännökset"
+msgstr "Ladda upp översatt PO-fil för att spara översättningar"
+
+msgid "Uses %s version"
+msgstr "Använder version %s "
```

### Comparing `wagtail-localize-1.5/wagtail_localize/locale/fr/LC_MESSAGES/django.mo` & `wagtail-localize-1.5.1/wagtail_localize/locale/fr/LC_MESSAGES/django.mo`

 * *Files 0% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,12 +1,12 @@
 msgid ""
 msgstr ""
 "Report-Msgid-Bugs-To: \n"
 "Last-Translator: Loic Teixeira, 2022\n"
-"Language-Team: French (https://www.transifex.com/torchbox/teams/8009/fr/)\n"
+"Language-Team: French (https://app.transifex.com/torchbox/teams/8009/fr/)\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Language: fr\n"
 "Plural-Forms: nplurals=3; plural=(n == 0 || n == 1) ? 0 : n != 0 && n % "
 "1000000 == 0 ? 1 : 2;\n"
 
 msgid ""
 "<{}> tag is not allowed. Strings can only contain standard HTML inline tags "
```

### Comparing `wagtail-localize-1.5/wagtail_localize/locale/fr/LC_MESSAGES/django.po` & `wagtail-localize-1.5.1/wagtail_localize/locale/fr/LC_MESSAGES/django.po`

 * *Files 1% similar despite different names*

```diff
@@ -3,17 +3,17 @@
 # Karl Hobley <karl@torchbox.com>, 2021
 # Benoît Bar <bar.benoit@gmail.com>, 2021
 # Loic Teixeira, 2022
 #
 msgid ""
 msgstr ""
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2022-10-17 21:00+0000\n"
+"POT-Creation-Date: 2023-02-23 14:15+0000\n"
 "Last-Translator: Loic Teixeira, 2022\n"
-"Language-Team: French (https://www.transifex.com/torchbox/teams/8009/fr/)\n"
+"Language-Team: French (https://app.transifex.com/torchbox/teams/8009/fr/)\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Language: fr\n"
 "Plural-Forms: nplurals=3; plural=(n == 0 || n == 1) ? 0 : n != 0 && n % "
 "1000000 == 0 ? 1 : 2;\n"
 
 msgid "Disable"
 msgstr "Désactiver"
```

### Comparing `wagtail-localize-1.5/wagtail_localize/locale/fr/LC_MESSAGES/djangojs.mo` & `wagtail-localize-1.5.1/wagtail_localize/locale/fr/LC_MESSAGES/djangojs.mo`

 * *Files 11% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,22 +1,19 @@
 msgid ""
 msgstr ""
 "Last-Translator: Loic Teixeira, 2022\n"
-"Language-Team: French (https://www.transifex.com/torchbox/teams/8009/fr/)\n"
+"Language-Team: French (https://app.transifex.com/torchbox/teams/8009/fr/)\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Language: fr\n"
 "Plural-Forms: nplurals=3; plural=(n == 0 || n == 1) ? 0 : n != 0 && n % "
 "1000000 == 0 ? 1 : 2;\n"
 
 msgid "Apply editor lock"
 msgstr "Ajouter un verrou éditeur"
 
-msgid "Breadcrumb"
-msgstr "Fil d'Ariane"
-
 msgid "Cancel"
 msgstr "Annuler"
 
 msgid "Change %s"
 msgstr "Modifier %s"
 
 msgid "Change document"
@@ -51,17 +48,14 @@
 
 msgid "Download PO file"
 msgstr "Télécharger un fichier PO"
 
 msgid "Download PO file and input translations offline"
 msgstr "Télécharger un fichier PO et effectuer les traductions hors-ligne"
 
-msgid "Draft"
-msgstr "Brouillon"
-
 msgid "Edit"
 msgstr "Modifier"
 
 msgid "Edit this %s"
 msgstr "Modifier ce/cette %s"
 
 msgid "Edit this document"
@@ -81,35 +75,26 @@
 
 msgid "Fetching image information..."
 msgstr "Récupération des informations de l'image en cours."
 
 msgid "Fetching page information..."
 msgstr "Récupération des informations de la page en cours."
 
-msgid "Live"
-msgstr "Publié(e)"
-
 msgid "Lock"
 msgstr "Verrouiller"
 
 msgid "Not translated"
 msgstr "Pas traduit"
 
 msgid "Preview"
 msgstr "Prévisualiser"
 
 msgid "Publish in "
 msgstr "Publier dans"
 
-msgid "Published"
-msgstr "Publié(e)"
-
-msgid "Published on "
-msgstr "Publié(e) le"
-
 msgid "Publishing..."
 msgstr "Publication..."
 
 msgid "Remove editor lock"
 msgstr "Supprimer un verrou éditeur"
 
 msgid "Revert to %s version"
```

### Comparing `wagtail-localize-1.5/wagtail_localize/locale/fr/LC_MESSAGES/djangojs.po` & `wagtail-localize-1.5.1/wagtail_localize/locale/pt_PT/LC_MESSAGES/djangojs.po`

 * *Files 13% similar despite different names*

```diff
@@ -1,168 +1,152 @@
 #
 # Translators:
-# Léo <leo@naeka.fr>, 2021
-# Loic Teixeira, 2022
+# Luís Tiago Favas <traducoes@favas.eu>, 2020
+# Tiago Henriques <trinosauro@gmail.com>, 2022
 #
 msgid ""
 msgstr ""
-"Last-Translator: Loic Teixeira, 2022\n"
-"Language-Team: French (https://www.transifex.com/torchbox/teams/8009/fr/)\n"
+"Last-Translator: Tiago Henriques <trinosauro@gmail.com>, 2022\n"
+"Language-Team: Portuguese (Portugal) (https://app.transifex.com/torchbox/"
+"teams/8009/pt_PT/)\n"
 "Content-Type: text/plain; charset=UTF-8\n"
-"Language: fr\n"
+"Language: pt_PT\n"
 "Plural-Forms: nplurals=3; plural=(n == 0 || n == 1) ? 0 : n != 0 && n % "
 "1000000 == 0 ? 1 : 2;\n"
 
 msgid "[DELETED]"
-msgstr "[SUPPRIMÉ(E)]"
+msgstr "[APAGADO]"
 
 msgid "Apply editor lock"
-msgstr "Ajouter un verrou éditeur"
-
-msgid "Breadcrumb"
-msgstr "Fil d'Ariane"
+msgstr "Aplicar bloqueio de editor"
 
 msgid "Cancel"
-msgstr "Annuler"
+msgstr "Cancelar"
 
 msgid "Change %s"
-msgstr "Modifier %s"
+msgstr "Mudar %s"
 
 msgid "Change document"
-msgstr "Changer le document"
+msgstr "Mudar documento"
 
 msgid "Change image"
-msgstr "Changer l'image"
+msgstr "Mudar imagem"
 
 msgid "Change page"
-msgstr "Changer la page"
+msgstr "Mudar página"
 
 msgid "Changed"
-msgstr "Modifié(e)(s)"
+msgstr "Mudado"
 
 msgid "Choose a %s"
-msgstr "Choisir un(e) %s"
+msgstr "Escolher um %s"
 
 msgid "Choose a document"
-msgstr "Choisir un document"
+msgstr "Escolher um documento"
 
 msgid "Choose a page"
-msgstr "Choisir une page"
+msgstr "Escolher uma página"
 
 msgid "Choose an image"
-msgstr "Choisir une image"
+msgstr "Escolher uma imagem"
 
 msgid "Convert to alias page"
-msgstr "Convertir en alias de page"
+msgstr "Converter em página de atalho"
 
 msgid "Delete"
-msgstr "Supprimer"
+msgstr "Apagar"
 
 msgid "Download PO file"
-msgstr "Télécharger un fichier PO"
+msgstr "Descarregar ficheiro PO"
 
 msgid "Download PO file and input translations offline"
-msgstr "Télécharger un fichier PO et effectuer les traductions hors-ligne"
-
-msgid "Draft"
-msgstr "Brouillon"
+msgstr "Descarregar ficheiro PO e introduzir traduções em offline"
 
 msgid "Edit"
-msgstr "Modifier"
+msgstr "Alterar"
 
 msgid "Edit this %s"
-msgstr "Modifier ce/cette %s"
+msgstr "Alterar este %s"
 
 msgid "Edit this document"
-msgstr "Modifier ce document"
+msgstr "Alterar este documento"
 
 msgid "Edit this image"
-msgstr "Modifier cette image"
+msgstr "Alterar esta imagem"
 
 msgid "Edit this page"
-msgstr "Modifier cette page"
+msgstr "Alterar esta página"
 
 msgid "Fetching %s information..."
-msgstr "Récupération des informations de %s en cours."
+msgstr "A obter informação %s..."
 
 msgid "Fetching document information..."
-msgstr "Récupération des informations du document en cours."
+msgstr "A obter informação do documento..."
 
 msgid "Fetching image information..."
-msgstr "Récupération des informations de l'image en cours."
+msgstr "A obter informação da imagem..."
 
 msgid "Fetching page information..."
-msgstr "Récupération des informations de la page en cours."
-
-msgid "Live"
-msgstr "Publié(e)"
+msgstr "A obter informação da página..."
 
 msgid "Lock"
-msgstr "Verrouiller"
+msgstr "Bloquear"
 
 msgid "Not translated"
-msgstr "Pas traduit"
+msgstr "Por traduzir"
 
 msgid "Preview"
-msgstr "Prévisualiser"
+msgstr "Visualizar"
 
 msgid "Publish in "
-msgstr "Publier dans"
-
-msgid "Published"
-msgstr "Publié(e)"
-
-msgid "Published on "
-msgstr "Publié(e) le"
+msgstr "Publicar em"
 
 msgid "Publishing..."
-msgstr "Publication..."
+msgstr "A publicar..."
 
 msgid "Remove editor lock"
-msgstr "Supprimer un verrou éditeur"
+msgstr "Retirar bloqueio de editor"
 
 msgid "Revert to %s version"
-msgstr "Revenir à la version %s"
+msgstr "Reverter à versão %s "
 
 msgid "Save"
-msgstr "Enregistrer"
+msgstr "Gravar"
 
 msgid "Saving..."
-msgstr "Enregistrement…"
+msgstr "A gravar..."
 
 msgid "segments translated"
-msgstr "segments traduits"
+msgstr "segmentos traduzidos"
 
 msgid "Server error"
-msgstr "Erreur du serveur"
+msgstr "Erro de servidor"
 
 msgid "Stop Synced translation"
-msgstr "Arrêter la synchronisation des traductions"
+msgstr "Parar tradução Sincronizada"
 
 msgid "There are unsaved segments. Please save or cancel them before leaving."
-msgstr ""
-"Il y a des segments non enregistrés. Veuillez les enregistrer ou les annuler "
-"avant de quitter."
+msgstr "Existem segmentos por gravar. Grave ou cancele-os antes de sair."
 
 msgid "Translate"
-msgstr "Traduire"
+msgstr "Traduzir"
 
 msgid "Translate all missing strings with "
-msgstr "Traduire toutes les chaînes manquantes avec "
+msgstr "Traduzir todos os segmentos de texto em falta com"
 
 msgid "Translate with "
-msgstr "Traduire avec "
+msgstr "Traduzir com"
 
 msgid "Unlock"
-msgstr "Déverrouiller"
+msgstr "Desbloquear"
 
 msgid "Unpublish"
-msgstr "Dépublier"
+msgstr "Despublicar"
 
 msgid "Upload PO file"
-msgstr "Transférer un fichier PO"
+msgstr "Carregar ficheiro PO"
 
 msgid "Upload translated PO file to submit translations"
-msgstr "Transférer un fichier PO traduit afin de mettre à jour les traductions"
+msgstr "Carregar ficheiro PO traduzido para enviar traduções"
 
 msgid "Uses %s version"
-msgstr "Utiliser la version %s"
+msgstr "Utiliza a versão %s"
```

### Comparing `wagtail-localize-1.5/wagtail_localize/locale/gl/LC_MESSAGES/django.mo` & `wagtail-localize-1.5.1/wagtail_localize/locale/gl/LC_MESSAGES/django.mo`

 * *Files 0% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,12 +1,12 @@
 msgid ""
 msgstr ""
 "Report-Msgid-Bugs-To: \n"
 "Last-Translator: X Bello <xbello@gmail.com>, 2022\n"
-"Language-Team: Galician (https://www.transifex.com/torchbox/teams/8009/gl/)\n"
+"Language-Team: Galician (https://app.transifex.com/torchbox/teams/8009/gl/)\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Language: gl\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
 
 msgid ""
 "<{}> tag is not allowed. Strings can only contain standard HTML inline tags "
 "(such as <b>, <a>)"
```

### Comparing `wagtail-localize-1.5/wagtail_localize/locale/gl/LC_MESSAGES/django.po` & `wagtail-localize-1.5.1/wagtail_localize/locale/gl/LC_MESSAGES/django.po`

 * *Files 1% similar despite different names*

```diff
@@ -3,17 +3,17 @@
 # Amós Oviedo <amos.oviedo@gmail.com>, 2022
 # Matt Westcott <matthew@torchbox.com>, 2022
 # X Bello <xbello@gmail.com>, 2022
 #
 msgid ""
 msgstr ""
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2022-10-17 21:00+0000\n"
+"POT-Creation-Date: 2023-02-23 14:15+0000\n"
 "Last-Translator: X Bello <xbello@gmail.com>, 2022\n"
-"Language-Team: Galician (https://www.transifex.com/torchbox/teams/8009/gl/)\n"
+"Language-Team: Galician (https://app.transifex.com/torchbox/teams/8009/gl/)\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Language: gl\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
 
 msgid "Disable"
 msgstr "Deshabilitar"
```

### Comparing `wagtail-localize-1.5/wagtail_localize/locale/gl/LC_MESSAGES/djangojs.mo` & `wagtail-localize-1.5.1/wagtail_localize/locale/pt_BR/LC_MESSAGES/djangojs.mo`

 * *Files 18% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,161 +1,148 @@
 msgid ""
 msgstr ""
-"Last-Translator: X Bello <xbello@gmail.com>, 2022\n"
-"Language-Team: Galician (https://www.transifex.com/torchbox/teams/8009/gl/)\n"
+"Last-Translator: Rodrigo de Almeida Sottomaior Macedo "
+"<rmsolucoeseminformatica@protonmail.com>, 2022\n"
+"Language-Team: Portuguese (Brazil) (https://app.transifex.com/torchbox/"
+"teams/8009/pt_BR/)\n"
 "Content-Type: text/plain; charset=UTF-8\n"
-"Language: gl\n"
-"Plural-Forms: nplurals=2; plural=(n != 1);\n"
+"Language: pt_BR\n"
+"Plural-Forms: nplurals=3; plural=(n == 0 || n == 1) ? 0 : n != 0 && n % "
+"1000000 == 0 ? 1 : 2;\n"
 
 msgid "Apply editor lock"
-msgstr "Aplicar bloqueo de editor"
-
-msgid "Breadcrumb"
-msgstr "Miga de pan"
+msgstr "Aplicar bloqueio do editor"
 
 msgid "Cancel"
 msgstr "Cancelar"
 
 msgid "Change %s"
-msgstr "Cambia %s"
+msgstr "Alterar %s"
 
 msgid "Change document"
-msgstr "Cambiar documento"
+msgstr "Alterar documento"
 
 msgid "Change image"
-msgstr "Cambiar imaxe"
+msgstr "Alterar imagem"
 
 msgid "Change page"
-msgstr "Cambiar páxina"
+msgstr "Alterar página"
 
 msgid "Changed"
-msgstr "Cambiado"
+msgstr "Alterado"
 
 msgid "Choose a %s"
-msgstr "Elixe un %s"
+msgstr "Escolha um %s"
 
 msgid "Choose a document"
-msgstr "Seleccionar un documento"
+msgstr "Escolha um documento"
 
 msgid "Choose a page"
-msgstr "Selecciona unha páxina"
+msgstr "Escolha uma página"
 
 msgid "Choose an image"
-msgstr "Seleccionar unha imaxe"
+msgstr "Escolha uma imagem"
 
 msgid "Convert to alias page"
-msgstr "Converter en páxina alias"
+msgstr "Converter em página de atalho"
 
 msgid "Delete"
-msgstr "Eliminar"
+msgstr "Excluir"
 
 msgid "Download PO file"
-msgstr "Descargar arquivo PO"
+msgstr "Baixar arquivo PO"
 
 msgid "Download PO file and input translations offline"
-msgstr "Descargar arquivo PO e introducir traduccións sen conexión"
-
-msgid "Draft"
-msgstr "Borrador"
+msgstr "Baixe o arquivo PO e insira traduções offline"
 
 msgid "Edit"
 msgstr "Editar"
 
 msgid "Edit this %s"
 msgstr "Editar este %s"
 
 msgid "Edit this document"
 msgstr "Editar este documento"
 
 msgid "Edit this image"
-msgstr "Editar esta imaxe"
+msgstr "Editar esta imagem"
 
 msgid "Edit this page"
-msgstr "Editar esta páxina"
+msgstr "Editar esta página"
 
 msgid "Fetching %s information..."
-msgstr "Recopilando información de %s..."
+msgstr "Buscando %s informação..."
 
 msgid "Fetching document information..."
-msgstr "Recopilando información do documento..."
+msgstr "Buscando informações do documento..."
 
 msgid "Fetching image information..."
-msgstr "Recopilar información da imaxe..."
+msgstr "Buscando informações da imagem..."
 
 msgid "Fetching page information..."
-msgstr "Recopilando información da páxina..."
-
-msgid "Live"
-msgstr "En vivo"
+msgstr "Buscando informações da página..."
 
 msgid "Lock"
-msgstr "Bloquear"
+msgstr "Travar"
 
 msgid "Not translated"
-msgstr "Non traducido"
+msgstr "Não traduzido"
 
 msgid "Preview"
-msgstr "Previsualizar"
+msgstr "Pré-visualizar"
 
 msgid "Publish in "
-msgstr "Publicar en "
-
-msgid "Published"
-msgstr "Publicada"
-
-msgid "Published on "
-msgstr "Publicar en"
+msgstr "Publicar em"
 
 msgid "Publishing..."
 msgstr "Publicando..."
 
 msgid "Remove editor lock"
-msgstr "Quitar bloqueo do editor"
+msgstr "Remover bloqueio do editor"
 
 msgid "Revert to %s version"
-msgstr "Reverter á versión %s"
+msgstr "Reverter para %s versão"
 
 msgid "Save"
-msgstr "Gardar"
+msgstr "Salvar"
 
 msgid "Saving..."
-msgstr "Gardando..."
+msgstr "Salvando..."
 
 msgid "Server error"
-msgstr "Erro do servidor"
+msgstr "Erro de servidor"
 
 msgid "Stop Synced translation"
-msgstr "Deter traducción Sincronizada"
+msgstr "Parar tradução sincronizada"
 
 msgid "There are unsaved segments. Please save or cancel them before leaving."
-msgstr ""
-"Hai segmentos sen gardar. Por favor, gárdaos ou cancélaos antes de sair."
+msgstr "Existem segmentos não salvos. Salve ou cancele-os antes de sair."
 
 msgid "Translate"
-msgstr "Traducir"
+msgstr "Traduzir"
 
 msgid "Translate all missing strings with "
-msgstr "Traducir tódolos textos faltantes con"
+msgstr "Traduzir todas as frases ausentes com"
 
 msgid "Translate with "
-msgstr "Traducir con"
+msgstr "Traduzir com"
 
 msgid "Unlock"
 msgstr "Desbloquear"
 
 msgid "Unpublish"
-msgstr "Cancelar publicación"
+msgstr "Despublicar"
 
 msgid "Upload PO file"
-msgstr "Subir arquivo PO"
+msgstr "Carregar arquivo PO"
 
 msgid "Upload translated PO file to submit translations"
-msgstr "Subir arquivo PO traducido para enviar traduccións"
+msgstr "Faça upload do arquivo PO traduzido para enviar traduções"
 
 msgid "Uses %s version"
-msgstr "Usa a versión %s"
+msgstr "Use a versão %s "
 
 msgid "[DELETED]"
-msgstr "[ELIMINADO]"
+msgstr "[REMOVIDO]"
 
 msgid "segments translated"
-msgstr "anacos traducidos"
+msgstr "segmentos traduzidos"
```

### Comparing `wagtail-localize-1.5/wagtail_localize/locale/gl/LC_MESSAGES/djangojs.po` & `wagtail-localize-1.5.1/wagtail_localize/locale/gl/LC_MESSAGES/djangojs.po`

 * *Files 4% similar despite different names*

```diff
@@ -2,28 +2,25 @@
 # Translators:
 # Amós Oviedo <amos.oviedo@gmail.com>, 2021
 # X Bello <xbello@gmail.com>, 2022
 #
 msgid ""
 msgstr ""
 "Last-Translator: X Bello <xbello@gmail.com>, 2022\n"
-"Language-Team: Galician (https://www.transifex.com/torchbox/teams/8009/gl/)\n"
+"Language-Team: Galician (https://app.transifex.com/torchbox/teams/8009/gl/)\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Language: gl\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
 
 msgid "[DELETED]"
 msgstr "[ELIMINADO]"
 
 msgid "Apply editor lock"
 msgstr "Aplicar bloqueo de editor"
 
-msgid "Breadcrumb"
-msgstr "Miga de pan"
-
 msgid "Cancel"
 msgstr "Cancelar"
 
 msgid "Change %s"
 msgstr "Cambia %s"
 
 msgid "Change document"
@@ -58,17 +55,14 @@
 
 msgid "Download PO file"
 msgstr "Descargar arquivo PO"
 
 msgid "Download PO file and input translations offline"
 msgstr "Descargar arquivo PO e introducir traduccións sen conexión"
 
-msgid "Draft"
-msgstr "Borrador"
-
 msgid "Edit"
 msgstr "Editar"
 
 msgid "Edit this %s"
 msgstr "Editar este %s"
 
 msgid "Edit this document"
@@ -88,35 +82,26 @@
 
 msgid "Fetching image information..."
 msgstr "Recopilar información da imaxe..."
 
 msgid "Fetching page information..."
 msgstr "Recopilando información da páxina..."
 
-msgid "Live"
-msgstr "En vivo"
-
 msgid "Lock"
 msgstr "Bloquear"
 
 msgid "Not translated"
 msgstr "Non traducido"
 
 msgid "Preview"
 msgstr "Previsualizar"
 
 msgid "Publish in "
 msgstr "Publicar en "
 
-msgid "Published"
-msgstr "Publicada"
-
-msgid "Published on "
-msgstr "Publicar en"
-
 msgid "Publishing..."
 msgstr "Publicando..."
 
 msgid "Remove editor lock"
 msgstr "Quitar bloqueo do editor"
 
 msgid "Revert to %s version"
```

### Comparing `wagtail-localize-1.5/wagtail_localize/locale/he_IL/LC_MESSAGES/django.mo` & `wagtail-localize-1.5.1/wagtail_localize/locale/he_IL/LC_MESSAGES/django.mo`

 * *Files 1% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,12 +1,12 @@
 msgid ""
 msgstr ""
 "Report-Msgid-Bugs-To: \n"
 "Last-Translator: Adi Ron <adi@bnop.co>, 2022\n"
-"Language-Team: Hebrew (Israel) (https://www.transifex.com/torchbox/"
+"Language-Team: Hebrew (Israel) (https://app.transifex.com/torchbox/"
 "teams/8009/he_IL/)\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Language: he_IL\n"
 "Plural-Forms: nplurals=4; plural=(n == 1 && n % 1 == 0) ? 0 : (n == 2 && n % "
 "1 == 0) ? 1: (n % 10 == 0 && n % 1 == 0 && n > 10) ? 2 : 3;\n"
 
 msgid "Content"
```

### Comparing `wagtail-localize-1.5/wagtail_localize/locale/he_IL/LC_MESSAGES/django.po` & `wagtail-localize-1.5.1/wagtail_localize/locale/he_IL/LC_MESSAGES/django.po`

 * *Files 15% similar despite different names*

```diff
@@ -3,17 +3,17 @@
 # 2ba49a64a97dc0c30b67cbb6522d98c8_d0a1309 <5628a6f4d3ab86b48aef276247790766_814>, 2021
 # lior abazon <abazon@v15.org.il>, 2022
 # Adi Ron <adi@bnop.co>, 2022
 #
 msgid ""
 msgstr ""
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2022-10-17 21:00+0000\n"
+"POT-Creation-Date: 2023-02-23 14:15+0000\n"
 "Last-Translator: Adi Ron <adi@bnop.co>, 2022\n"
-"Language-Team: Hebrew (Israel) (https://www.transifex.com/torchbox/"
+"Language-Team: Hebrew (Israel) (https://app.transifex.com/torchbox/"
 "teams/8009/he_IL/)\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Language: he_IL\n"
 "Plural-Forms: nplurals=4; plural=(n == 1 && n % 1 == 0) ? 0 : (n == 2 && n % "
 "1 == 0) ? 1: (n % 10 == 0 && n % 1 == 0 && n > 10) ? 2 : 3;\n"
 
 msgid "Saving…"
```

### Comparing `wagtail-localize-1.5/wagtail_localize/locale/he_IL/LC_MESSAGES/djangojs.po` & `wagtail-localize-1.5.1/wagtail_localize/locale/he_IL/LC_MESSAGES/djangojs.po`

 * *Files 16% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 # Karl Hobley <karl@torchbox.com>, 2021
 # Adi Ron <adi@bnop.co>, 2021
 # lior abazon <abazon@v15.org.il>, 2021
 #
 msgid ""
 msgstr ""
 "Last-Translator: lior abazon <abazon@v15.org.il>, 2021\n"
-"Language-Team: Hebrew (Israel) (https://www.transifex.com/torchbox/"
+"Language-Team: Hebrew (Israel) (https://app.transifex.com/torchbox/"
 "teams/8009/he_IL/)\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Language: he_IL\n"
 "Plural-Forms: nplurals=4; plural=(n == 1 && n % 1 == 0) ? 0 : (n == 2 && n % "
 "1 == 0) ? 1: (n % 10 == 0 && n % 1 == 0 && n > 10) ? 2 : 3;\n"
 
 msgid "Choose a document"
@@ -22,17 +22,14 @@
 
 msgid "Choose an image"
 msgstr "בחרו תמונה"
 
 msgid "Delete"
 msgstr "מחק"
 
-msgid "Draft"
-msgstr "טיוטה"
-
 msgid "Edit"
 msgstr "ערוך"
 
 msgid "Edit this %s"
 msgstr "ערוך את %s זה"
 
 msgid "Edit this document"
@@ -40,17 +37,14 @@
 
 msgid "Edit this image"
 msgstr "ערוך תמונה זו "
 
 msgid "Edit this page"
 msgstr "ערוך עמוד זה"
 
-msgid "Live"
-msgstr "חי"
-
 msgid "Preview"
 msgstr "תצוגה מקדימה "
 
 msgid "Save"
 msgstr "שמור"
 
 msgid "Unpublish"
```

### Comparing `wagtail-localize-1.5/wagtail_localize/locale/hr_HR/LC_MESSAGES/django.mo` & `wagtail-localize-1.5.1/wagtail_localize/locale/hr_HR/LC_MESSAGES/django.mo`

 * *Files 2% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,12 +1,12 @@
 msgid ""
 msgstr ""
 "Report-Msgid-Bugs-To: \n"
 "Last-Translator: Dino Aljević <dino8890@protonmail.com>, 2022\n"
-"Language-Team: Croatian (Croatia) (https://www.transifex.com/torchbox/"
+"Language-Team: Croatian (Croatia) (https://app.transifex.com/torchbox/"
 "teams/8009/hr_HR/)\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Language: hr_HR\n"
 "Plural-Forms: nplurals=3; plural=n%10==1 && n%100!=11 ? 0 : n%10>=2 && "
 "n%10<=4 && (n%100<10 || n%100>=20) ? 1 : 2;\n"
 
 msgid "All child pages will be created."
```

### Comparing `wagtail-localize-1.5/wagtail_localize/locale/hr_HR/LC_MESSAGES/django.po` & `wagtail-localize-1.5.1/wagtail_localize/locale/hr_HR/LC_MESSAGES/django.po`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 #
 # Translators:
 # Dino Aljević <dino8890@protonmail.com>, 2022
 #
 msgid ""
 msgstr ""
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2022-10-17 21:00+0000\n"
+"POT-Creation-Date: 2023-02-23 14:15+0000\n"
 "Last-Translator: Dino Aljević <dino8890@protonmail.com>, 2022\n"
-"Language-Team: Croatian (Croatia) (https://www.transifex.com/torchbox/"
+"Language-Team: Croatian (Croatia) (https://app.transifex.com/torchbox/"
 "teams/8009/hr_HR/)\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Language: hr_HR\n"
 "Plural-Forms: nplurals=3; plural=n%10==1 && n%100!=11 ? 0 : n%10>=2 && "
 "n%10<=4 && (n%100<10 || n%100>=20) ? 1 : 2;\n"
 
 msgid "Disable"
```

### Comparing `wagtail-localize-1.5/wagtail_localize/locale/hr_HR/LC_MESSAGES/djangojs.mo` & `wagtail-localize-1.5.1/wagtail_localize/locale/hr_HR/LC_MESSAGES/djangojs.mo`

 * *Files 20% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,11 +1,11 @@
 msgid ""
 msgstr ""
 "Last-Translator: Dino Aljević <dino8890@protonmail.com>, 2022\n"
-"Language-Team: Croatian (Croatia) (https://www.transifex.com/torchbox/"
+"Language-Team: Croatian (Croatia) (https://app.transifex.com/torchbox/"
 "teams/8009/hr_HR/)\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Language: hr_HR\n"
 "Plural-Forms: nplurals=3; plural=n%10==1 && n%100!=11 ? 0 : n%10>=2 && "
 "n%10<=4 && (n%100<10 || n%100>=20) ? 1 : 2;\n"
 
 msgid "Cancel"
@@ -22,17 +22,14 @@
 
 msgid "Choose an image"
 msgstr "Odaberi sliku"
 
 msgid "Delete"
 msgstr "Izbriši"
 
-msgid "Draft"
-msgstr "Skica"
-
 msgid "Edit"
 msgstr "Uredi"
 
 msgid "Edit this %s"
 msgstr "Uredi ovaj %s"
 
 msgid "Edit this document"
@@ -40,26 +37,20 @@
 
 msgid "Edit this image"
 msgstr "Uredi ovu sliku"
 
 msgid "Edit this page"
 msgstr "Uredi ovu stranicu"
 
-msgid "Live"
-msgstr "Uživo"
-
 msgid "Lock"
 msgstr "Zaključavanje"
 
 msgid "Preview"
 msgstr "Pregled"
 
-msgid "Published"
-msgstr "Objavljeno"
-
 msgid "Save"
 msgstr "Spremi"
 
 msgid "Translate"
 msgstr "Prevedi"
 
 msgid "Unlock"
```

### Comparing `wagtail-localize-1.5/wagtail_localize/locale/hr_HR/LC_MESSAGES/djangojs.po` & `wagtail-localize-1.5.1/wagtail_localize/locale/mi/LC_MESSAGES/djangojs.po`

 * *Files 22% similar despite different names*

```diff
@@ -1,74 +1,53 @@
 #
 # Translators:
-# Luka Matijević <lumatijev@gmail.com>, 2021
-# Dino Aljević <dino8890@protonmail.com>, 2022
+# Awatea Randall <awatea@octave.nz>, 2021
 #
 msgid ""
 msgstr ""
-"Last-Translator: Dino Aljević <dino8890@protonmail.com>, 2022\n"
-"Language-Team: Croatian (Croatia) (https://www.transifex.com/torchbox/"
-"teams/8009/hr_HR/)\n"
+"Last-Translator: Awatea Randall <awatea@octave.nz>, 2021\n"
+"Language-Team: Maori (https://app.transifex.com/torchbox/teams/8009/mi/)\n"
 "Content-Type: text/plain; charset=UTF-8\n"
-"Language: hr_HR\n"
-"Plural-Forms: nplurals=3; plural=n%10==1 && n%100!=11 ? 0 : n%10>=2 && "
-"n%10<=4 && (n%100<10 || n%100>=20) ? 1 : 2;\n"
+"Language: mi\n"
+"Plural-Forms: nplurals=2; plural=(n > 1);\n"
 
-msgid "Cancel"
-msgstr "Odustani"
-
-msgid "Change image"
-msgstr "Promijeni sliku"
+msgid "Apply editor lock"
+msgstr "Purua he raka ētita"
 
 msgid "Choose a document"
-msgstr "Odaberi dokument"
+msgstr "Kōhiti he pukapuka"
 
 msgid "Choose a page"
-msgstr "Odaberite stranicu"
+msgstr "Kōhiti he whārangi"
 
 msgid "Choose an image"
-msgstr "Odaberi sliku"
+msgstr "Kōhiti he whakaahua"
 
 msgid "Delete"
-msgstr "Izbriši"
-
-msgid "Draft"
-msgstr "Skica"
+msgstr "Muku"
 
 msgid "Edit"
-msgstr "Uredi"
+msgstr "Whakarerekē"
 
 msgid "Edit this %s"
-msgstr "Uredi ovaj %s"
+msgstr "Whakarerekē i tēnei %s"
 
 msgid "Edit this document"
-msgstr "Uredi ovaj dokument"
-
-msgid "Edit this image"
-msgstr "Uredi ovu sliku"
+msgstr "Whakarerekē i tēnei pukapuka"
 
 msgid "Edit this page"
-msgstr "Uredi ovu stranicu"
-
-msgid "Live"
-msgstr "Uživo"
+msgstr "Whakarerekē i tēnei whārangi"
 
 msgid "Lock"
-msgstr "Zaključavanje"
+msgstr "Raka"
 
 msgid "Preview"
-msgstr "Pregled"
-
-msgid "Published"
-msgstr "Objavljeno"
+msgstr "Titiro"
 
 msgid "Save"
-msgstr "Spremi"
-
-msgid "Translate"
-msgstr "Prevedi"
+msgstr "Puritia"
 
 msgid "Unlock"
-msgstr "Otključavanje"
+msgstr "Iriti"
 
 msgid "Unpublish"
-msgstr "Odjavi"
+msgstr "whakakore te whakaputa"
```

### Comparing `wagtail-localize-1.5/wagtail_localize/locale/hu/LC_MESSAGES/django.mo` & `wagtail-localize-1.5.1/wagtail_localize/locale/hu/LC_MESSAGES/django.mo`

 * *Files 0% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,12 +1,12 @@
 msgid ""
 msgstr ""
 "Report-Msgid-Bugs-To: \n"
 "Last-Translator: Istvan Farkas <istvan.farkas@gmail.com>, 2022\n"
-"Language-Team: Hungarian (https://www.transifex.com/torchbox/teams/8009/"
+"Language-Team: Hungarian (https://app.transifex.com/torchbox/teams/8009/"
 "hu/)\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Language: hu\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
 
 msgid ""
 "<{}> tag is not allowed. Strings can only contain standard HTML inline tags "
```

### Comparing `wagtail-localize-1.5/wagtail_localize/locale/hu/LC_MESSAGES/django.po` & `wagtail-localize-1.5.1/wagtail_localize/locale/hu/LC_MESSAGES/django.po`

 * *Files 2% similar despite different names*

```diff
@@ -3,17 +3,17 @@
 # Laszlo Molnar <lazlowmiller@gmail.com>, 2021
 # Dan Braghis, 2022
 # Istvan Farkas <istvan.farkas@gmail.com>, 2022
 #
 msgid ""
 msgstr ""
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2022-10-17 21:00+0000\n"
+"POT-Creation-Date: 2023-02-23 14:15+0000\n"
 "Last-Translator: Istvan Farkas <istvan.farkas@gmail.com>, 2022\n"
-"Language-Team: Hungarian (https://www.transifex.com/torchbox/teams/8009/"
+"Language-Team: Hungarian (https://app.transifex.com/torchbox/teams/8009/"
 "hu/)\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Language: hu\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
 
 msgid "Disable"
 msgstr "Kikapcsol"
```

### Comparing `wagtail-localize-1.5/wagtail_localize/locale/hu/LC_MESSAGES/djangojs.mo` & `wagtail-localize-1.5.1/wagtail_localize/locale/hu/LC_MESSAGES/djangojs.mo`

 * *Files 11% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,22 +1,19 @@
 msgid ""
 msgstr ""
 "Last-Translator: Istvan Farkas <istvan.farkas@gmail.com>, 2022\n"
-"Language-Team: Hungarian (https://www.transifex.com/torchbox/teams/8009/"
+"Language-Team: Hungarian (https://app.transifex.com/torchbox/teams/8009/"
 "hu/)\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Language: hu\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
 
 msgid "Apply editor lock"
 msgstr "Szerkesztési zárolás"
 
-msgid "Breadcrumb"
-msgstr "Morzsamenü"
-
 msgid "Cancel"
 msgstr "Mégsem"
 
 msgid "Change %s"
 msgstr "%s megváltoztatása"
 
 msgid "Change document"
@@ -51,17 +48,14 @@
 
 msgid "Download PO file"
 msgstr "PO fájl letöltése"
 
 msgid "Download PO file and input translations offline"
 msgstr "PO fájl letöltése, és a fordítások kitöltése külön"
 
-msgid "Draft"
-msgstr "Vázlat"
-
 msgid "Edit"
 msgstr "Szerkesztés"
 
 msgid "Edit this %s"
 msgstr "%s szerkesztése"
 
 msgid "Edit this document"
@@ -81,35 +75,26 @@
 
 msgid "Fetching image information..."
 msgstr "Kép információinak lekérése..."
 
 msgid "Fetching page information..."
 msgstr "Oldal információinak lekérése"
 
-msgid "Live"
-msgstr "Élő"
-
 msgid "Lock"
 msgstr "Lezár"
 
 msgid "Not translated"
 msgstr "Nincs lefordítva"
 
 msgid "Preview"
 msgstr "Előnézet"
 
 msgid "Publish in "
 msgstr "Közzététel: "
 
-msgid "Published"
-msgstr "Élő"
-
-msgid "Published on "
-msgstr "Közzététel ideje: "
-
 msgid "Publishing..."
 msgstr "Közzététel..."
 
 msgid "Remove editor lock"
 msgstr "Szerkesztési zár feloldása"
 
 msgid "Revert to %s version"
```

### Comparing `wagtail-localize-1.5/wagtail_localize/locale/hu/LC_MESSAGES/djangojs.po` & `wagtail-localize-1.5.1/wagtail_localize/locale/hu/LC_MESSAGES/djangojs.po`

 * *Files 5% similar despite different names*

```diff
@@ -1,29 +1,26 @@
 #
 # Translators:
 # Istvan Farkas <istvan.farkas@gmail.com>, 2022
 #
 msgid ""
 msgstr ""
 "Last-Translator: Istvan Farkas <istvan.farkas@gmail.com>, 2022\n"
-"Language-Team: Hungarian (https://www.transifex.com/torchbox/teams/8009/"
+"Language-Team: Hungarian (https://app.transifex.com/torchbox/teams/8009/"
 "hu/)\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Language: hu\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
 
 msgid "[DELETED]"
 msgstr "[TÖRÖLT]"
 
 msgid "Apply editor lock"
 msgstr "Szerkesztési zárolás"
 
-msgid "Breadcrumb"
-msgstr "Morzsamenü"
-
 msgid "Cancel"
 msgstr "Mégsem"
 
 msgid "Change %s"
 msgstr "%s megváltoztatása"
 
 msgid "Change document"
@@ -58,17 +55,14 @@
 
 msgid "Download PO file"
 msgstr "PO fájl letöltése"
 
 msgid "Download PO file and input translations offline"
 msgstr "PO fájl letöltése, és a fordítások kitöltése külön"
 
-msgid "Draft"
-msgstr "Vázlat"
-
 msgid "Edit"
 msgstr "Szerkesztés"
 
 msgid "Edit this %s"
 msgstr "%s szerkesztése"
 
 msgid "Edit this document"
@@ -88,35 +82,26 @@
 
 msgid "Fetching image information..."
 msgstr "Kép információinak lekérése..."
 
 msgid "Fetching page information..."
 msgstr "Oldal információinak lekérése"
 
-msgid "Live"
-msgstr "Élő"
-
 msgid "Lock"
 msgstr "Lezár"
 
 msgid "Not translated"
 msgstr "Nincs lefordítva"
 
 msgid "Preview"
 msgstr "Előnézet"
 
 msgid "Publish in "
 msgstr "Közzététel: "
 
-msgid "Published"
-msgstr "Élő"
-
-msgid "Published on "
-msgstr "Közzététel ideje: "
-
 msgid "Publishing..."
 msgstr "Közzététel..."
 
 msgid "Remove editor lock"
 msgstr "Szerkesztési zár feloldása"
 
 msgid "Revert to %s version"
```

### Comparing `wagtail-localize-1.5/wagtail_localize/locale/id_ID/LC_MESSAGES/django.mo` & `wagtail-localize-1.5.1/wagtail_localize/locale/id_ID/LC_MESSAGES/django.mo`

 * *Files 3% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,12 +1,12 @@
 msgid ""
 msgstr ""
 "Report-Msgid-Bugs-To: \n"
 "Last-Translator: M. Febrian Ramadhana <febrian@ramadhana.me>, 2022\n"
-"Language-Team: Indonesian (Indonesia) (https://www.transifex.com/torchbox/"
+"Language-Team: Indonesian (Indonesia) (https://app.transifex.com/torchbox/"
 "teams/8009/id_ID/)\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Language: id_ID\n"
 "Plural-Forms: nplurals=1; plural=0;\n"
 
 msgid "Content"
 msgstr "Konten"
```

### Comparing `wagtail-localize-1.5/wagtail_localize/locale/id_ID/LC_MESSAGES/django.po` & `wagtail-localize-1.5.1/wagtail_localize/locale/id_ID/LC_MESSAGES/django.po`

 * *Files 12% similar despite different names*

```diff
@@ -3,17 +3,17 @@
 # Ronggo Radityo <radityo3000@yahoo.com>, 2021
 # Sutrisno Efendi <kangfend@gmail.com>, 2021
 # M. Febrian Ramadhana <febrian@ramadhana.me>, 2022
 #
 msgid ""
 msgstr ""
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2022-10-17 21:00+0000\n"
+"POT-Creation-Date: 2023-02-23 14:15+0000\n"
 "Last-Translator: M. Febrian Ramadhana <febrian@ramadhana.me>, 2022\n"
-"Language-Team: Indonesian (Indonesia) (https://www.transifex.com/torchbox/"
+"Language-Team: Indonesian (Indonesia) (https://app.transifex.com/torchbox/"
 "teams/8009/id_ID/)\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Language: id_ID\n"
 "Plural-Forms: nplurals=1; plural=0;\n"
 
 msgid "Saving…"
 msgstr "Menyimpan..."
```

### Comparing `wagtail-localize-1.5/wagtail_localize/locale/id_ID/LC_MESSAGES/djangojs.mo` & `wagtail-localize-1.5.1/wagtail_localize/locale/id_ID/LC_MESSAGES/djangojs.mo`

 * *Files 12% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,11 +1,11 @@
 msgid ""
 msgstr ""
 "Last-Translator: M. Febrian Ramadhana <febrian@ramadhana.me>, 2021\n"
-"Language-Team: Indonesian (Indonesia) (https://www.transifex.com/torchbox/"
+"Language-Team: Indonesian (Indonesia) (https://app.transifex.com/torchbox/"
 "teams/8009/id_ID/)\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Language: id_ID\n"
 "Plural-Forms: nplurals=1; plural=0;\n"
 
 msgid "Apply editor lock"
 msgstr "Terapkan kunci editor"
@@ -21,17 +21,14 @@
 
 msgid "Choose an image"
 msgstr "Pilih sebuah gambar"
 
 msgid "Delete"
 msgstr "Hapus"
 
-msgid "Draft"
-msgstr "Konsep"
-
 msgid "Edit"
 msgstr "Ubah"
 
 msgid "Edit this %s"
 msgstr "Ubah %s ini"
 
 msgid "Edit this document"
@@ -39,17 +36,14 @@
 
 msgid "Edit this image"
 msgstr "Ubah gambar ini"
 
 msgid "Edit this page"
 msgstr "Ubah halaman ini"
 
-msgid "Live"
-msgstr "Terpublikasi"
-
 msgid "Lock"
 msgstr "Kunci"
 
 msgid "Preview"
 msgstr "Pratinjau"
 
 msgid "Publishing..."
```

### Comparing `wagtail-localize-1.5/wagtail_localize/locale/id_ID/LC_MESSAGES/djangojs.po` & `wagtail-localize-1.5.1/wagtail_localize/locale/id_ID/LC_MESSAGES/djangojs.po`

 * *Files 10% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 # Ronggo Radityo <radityo3000@yahoo.com>, 2021
 # Andry Widya Putra UN <andrywidyaputra@gmail.com>, 2021
 # M. Febrian Ramadhana <febrian@ramadhana.me>, 2021
 #
 msgid ""
 msgstr ""
 "Last-Translator: M. Febrian Ramadhana <febrian@ramadhana.me>, 2021\n"
-"Language-Team: Indonesian (Indonesia) (https://www.transifex.com/torchbox/"
+"Language-Team: Indonesian (Indonesia) (https://app.transifex.com/torchbox/"
 "teams/8009/id_ID/)\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Language: id_ID\n"
 "Plural-Forms: nplurals=1; plural=0;\n"
 
 msgid "Apply editor lock"
 msgstr "Terapkan kunci editor"
@@ -29,17 +29,14 @@
 
 msgid "Choose an image"
 msgstr "Pilih sebuah gambar"
 
 msgid "Delete"
 msgstr "Hapus"
 
-msgid "Draft"
-msgstr "Konsep"
-
 msgid "Edit"
 msgstr "Ubah"
 
 msgid "Edit this %s"
 msgstr "Ubah %s ini"
 
 msgid "Edit this document"
@@ -47,17 +44,14 @@
 
 msgid "Edit this image"
 msgstr "Ubah gambar ini"
 
 msgid "Edit this page"
 msgstr "Ubah halaman ini"
 
-msgid "Live"
-msgstr "Terpublikasi"
-
 msgid "Lock"
 msgstr "Kunci"
 
 msgid "Preview"
 msgstr "Pratinjau"
 
 msgid "Publishing..."
```

### Comparing `wagtail-localize-1.5/wagtail_localize/locale/is_IS/LC_MESSAGES/django.mo` & `wagtail-localize-1.5.1/wagtail_localize/locale/is_IS/LC_MESSAGES/django.mo`

 * *Files 0% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,12 +1,12 @@
 msgid ""
 msgstr ""
 "Report-Msgid-Bugs-To: \n"
 "Last-Translator: Arnar Tumi Þorsteinsson <arnartumi@gmail.com>, 2022\n"
-"Language-Team: Icelandic (Iceland) (https://www.transifex.com/torchbox/"
+"Language-Team: Icelandic (Iceland) (https://app.transifex.com/torchbox/"
 "teams/8009/is_IS/)\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Language: is_IS\n"
 "Plural-Forms: nplurals=2; plural=(n % 10 != 1 || n % 100 == 11);\n"
 
 msgid ""
 "<{}> tag is not allowed. Strings can only contain standard HTML inline tags "
```

### Comparing `wagtail-localize-1.5/wagtail_localize/locale/is_IS/LC_MESSAGES/django.po` & `wagtail-localize-1.5.1/wagtail_localize/locale/is_IS/LC_MESSAGES/django.po`

 * *Files 1% similar despite different names*

```diff
@@ -2,17 +2,17 @@
 # Translators:
 # saevarom <saevar@saevar.is>, 2022
 # Arnar Tumi Þorsteinsson <arnartumi@gmail.com>, 2022
 #
 msgid ""
 msgstr ""
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2022-10-17 21:00+0000\n"
+"POT-Creation-Date: 2023-02-23 14:15+0000\n"
 "Last-Translator: Arnar Tumi Þorsteinsson <arnartumi@gmail.com>, 2022\n"
-"Language-Team: Icelandic (Iceland) (https://www.transifex.com/torchbox/"
+"Language-Team: Icelandic (Iceland) (https://app.transifex.com/torchbox/"
 "teams/8009/is_IS/)\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Language: is_IS\n"
 "Plural-Forms: nplurals=2; plural=(n % 10 != 1 || n % 100 == 11);\n"
 
 msgid "Disable"
 msgstr "Afvirkja"
```

### Comparing `wagtail-localize-1.5/wagtail_localize/locale/is_IS/LC_MESSAGES/djangojs.mo` & `wagtail-localize-1.5.1/wagtail_localize/locale/is_IS/LC_MESSAGES/djangojs.mo`

 * *Files 16% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,22 +1,19 @@
 msgid ""
 msgstr ""
 "Last-Translator: Arnar Tumi Þorsteinsson <arnartumi@gmail.com>, 2022\n"
-"Language-Team: Icelandic (Iceland) (https://www.transifex.com/torchbox/"
+"Language-Team: Icelandic (Iceland) (https://app.transifex.com/torchbox/"
 "teams/8009/is_IS/)\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Language: is_IS\n"
 "Plural-Forms: nplurals=2; plural=(n % 10 != 1 || n % 100 == 11);\n"
 
 msgid "Apply editor lock"
 msgstr "Kveikja á skriflás"
 
-msgid "Breadcrumb"
-msgstr "Brauðmolar"
-
 msgid "Cancel"
 msgstr "Hætta við"
 
 msgid "Change %s"
 msgstr "Breyta %s"
 
 msgid "Change document"
@@ -51,17 +48,14 @@
 
 msgid "Download PO file"
 msgstr "Hlaða niður PO skrá"
 
 msgid "Download PO file and input translations offline"
 msgstr "Hlaða niður PO skrá og þýða utan nets"
 
-msgid "Draft"
-msgstr "Uppkast"
-
 msgid "Edit"
 msgstr "Breyta"
 
 msgid "Edit this %s"
 msgstr "Breyta þessu %s"
 
 msgid "Edit this document"
@@ -81,35 +75,26 @@
 
 msgid "Fetching image information..."
 msgstr "Sæki upplýsingar um mynd..."
 
 msgid "Fetching page information..."
 msgstr "Sæki upplýsingar um síðu..."
 
-msgid "Live"
-msgstr "Í birtingu"
-
 msgid "Lock"
 msgstr "Læsa"
 
 msgid "Not translated"
 msgstr "Ekki þýtt"
 
 msgid "Preview"
 msgstr "Forskoða"
 
 msgid "Publish in "
 msgstr "Birta í"
 
-msgid "Published"
-msgstr "Sett í birtingu"
-
-msgid "Published on "
-msgstr "Sett í birtingu "
-
 msgid "Publishing..."
 msgstr "Set í birtingu..."
 
 msgid "Remove editor lock"
 msgstr "Fjarlægja skriflás"
 
 msgid "Revert to %s version"
```

### Comparing `wagtail-localize-1.5/wagtail_localize/locale/is_IS/LC_MESSAGES/djangojs.po` & `wagtail-localize-1.5.1/wagtail_localize/locale/is_IS/LC_MESSAGES/djangojs.po`

 * *Files 11% similar despite different names*

```diff
@@ -2,29 +2,26 @@
 # Translators:
 # saevarom <saevar@saevar.is>, 2022
 # Arnar Tumi Þorsteinsson <arnartumi@gmail.com>, 2022
 #
 msgid ""
 msgstr ""
 "Last-Translator: Arnar Tumi Þorsteinsson <arnartumi@gmail.com>, 2022\n"
-"Language-Team: Icelandic (Iceland) (https://www.transifex.com/torchbox/"
+"Language-Team: Icelandic (Iceland) (https://app.transifex.com/torchbox/"
 "teams/8009/is_IS/)\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Language: is_IS\n"
 "Plural-Forms: nplurals=2; plural=(n % 10 != 1 || n % 100 == 11);\n"
 
 msgid "[DELETED]"
 msgstr "[EYDD]"
 
 msgid "Apply editor lock"
 msgstr "Kveikja á skriflás"
 
-msgid "Breadcrumb"
-msgstr "Brauðmolar"
-
 msgid "Cancel"
 msgstr "Hætta við"
 
 msgid "Change %s"
 msgstr "Breyta %s"
 
 msgid "Change document"
@@ -59,17 +56,14 @@
 
 msgid "Download PO file"
 msgstr "Hlaða niður PO skrá"
 
 msgid "Download PO file and input translations offline"
 msgstr "Hlaða niður PO skrá og þýða utan nets"
 
-msgid "Draft"
-msgstr "Uppkast"
-
 msgid "Edit"
 msgstr "Breyta"
 
 msgid "Edit this %s"
 msgstr "Breyta þessu %s"
 
 msgid "Edit this document"
@@ -89,35 +83,26 @@
 
 msgid "Fetching image information..."
 msgstr "Sæki upplýsingar um mynd..."
 
 msgid "Fetching page information..."
 msgstr "Sæki upplýsingar um síðu..."
 
-msgid "Live"
-msgstr "Í birtingu"
-
 msgid "Lock"
 msgstr "Læsa"
 
 msgid "Not translated"
 msgstr "Ekki þýtt"
 
 msgid "Preview"
 msgstr "Forskoða"
 
 msgid "Publish in "
 msgstr "Birta í"
 
-msgid "Published"
-msgstr "Sett í birtingu"
-
-msgid "Published on "
-msgstr "Sett í birtingu "
-
 msgid "Publishing..."
 msgstr "Set í birtingu..."
 
 msgid "Remove editor lock"
 msgstr "Fjarlægja skriflás"
 
 msgid "Revert to %s version"
```

### Comparing `wagtail-localize-1.5/wagtail_localize/locale/it/LC_MESSAGES/django.mo` & `wagtail-localize-1.5.1/wagtail_localize/locale/it/LC_MESSAGES/django.mo`

 * *Files 0% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,12 +1,12 @@
 msgid ""
 msgstr ""
 "Report-Msgid-Bugs-To: \n"
 "Last-Translator: Marco Badan <marco.badan@gmail.com>, 2022\n"
-"Language-Team: Italian (https://www.transifex.com/torchbox/teams/8009/it/)\n"
+"Language-Team: Italian (https://app.transifex.com/torchbox/teams/8009/it/)\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Language: it\n"
 "Plural-Forms: nplurals=3; plural=n == 1 ? 0 : n != 0 && n % 1000000 == 0 ? "
 "1 : 2;\n"
 
 msgid ""
 "<{}> tag is not allowed. Strings can only contain standard HTML inline tags "
```

### Comparing `wagtail-localize-1.5/wagtail_localize/locale/it/LC_MESSAGES/django.po` & `wagtail-localize-1.5.1/wagtail_localize/locale/it/LC_MESSAGES/django.po`

 * *Files 1% similar despite different names*

```diff
@@ -2,17 +2,17 @@
 # Translators:
 # Giacomo Ghizzani <giacomo.ghz@gmail.com>, 2022
 # Marco Badan <marco.badan@gmail.com>, 2022
 #
 msgid ""
 msgstr ""
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2022-10-17 21:00+0000\n"
+"POT-Creation-Date: 2023-02-23 14:15+0000\n"
 "Last-Translator: Marco Badan <marco.badan@gmail.com>, 2022\n"
-"Language-Team: Italian (https://www.transifex.com/torchbox/teams/8009/it/)\n"
+"Language-Team: Italian (https://app.transifex.com/torchbox/teams/8009/it/)\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Language: it\n"
 "Plural-Forms: nplurals=3; plural=n == 1 ? 0 : n != 0 && n % 1000000 == 0 ? "
 "1 : 2;\n"
 
 msgid "Disable"
 msgstr "Disabilita"
```

### Comparing `wagtail-localize-1.5/wagtail_localize/locale/it/LC_MESSAGES/djangojs.mo` & `wagtail-localize-1.5.1/wagtail_localize/locale/it/LC_MESSAGES/djangojs.mo`

 * *Files 12% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,22 +1,19 @@
 msgid ""
 msgstr ""
 "Last-Translator: Marco Badan <marco.badan@gmail.com>, 2022\n"
-"Language-Team: Italian (https://www.transifex.com/torchbox/teams/8009/it/)\n"
+"Language-Team: Italian (https://app.transifex.com/torchbox/teams/8009/it/)\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Language: it\n"
 "Plural-Forms: nplurals=3; plural=n == 1 ? 0 : n != 0 && n % 1000000 == 0 ? "
 "1 : 2;\n"
 
 msgid "Apply editor lock"
 msgstr "Applica il blocco dell'editor"
 
-msgid "Breadcrumb"
-msgstr "Breadcrumb"
-
 msgid "Cancel"
 msgstr "Annulla"
 
 msgid "Change %s"
 msgstr "Cambia %s"
 
 msgid "Change document"
@@ -51,17 +48,14 @@
 
 msgid "Download PO file"
 msgstr "Scarica file PO"
 
 msgid "Download PO file and input translations offline"
 msgstr "Scarica file PO e inserisci le traduzioni offline"
 
-msgid "Draft"
-msgstr "Bozza"
-
 msgid "Edit"
 msgstr "Modifica"
 
 msgid "Edit this %s"
 msgstr "Modifica questo %s"
 
 msgid "Edit this document"
@@ -81,35 +75,26 @@
 
 msgid "Fetching image information..."
 msgstr "Raccolta informazioni immagine in corso..."
 
 msgid "Fetching page information..."
 msgstr "Raccolta informazioni pagina in corso..."
 
-msgid "Live"
-msgstr "Live"
-
 msgid "Lock"
 msgstr "Blocca"
 
 msgid "Not translated"
 msgstr "Non tradotto"
 
 msgid "Preview"
 msgstr "Anteprima"
 
 msgid "Publish in "
 msgstr "Pubblicata in"
 
-msgid "Published"
-msgstr "Pubblicata"
-
-msgid "Published on "
-msgstr "Pubblicata il"
-
 msgid "Publishing..."
 msgstr "Pubblicazione in corso..."
 
 msgid "Remove editor lock"
 msgstr "Rimuovi blocco editor"
 
 msgid "Revert to %s version"
```

### Comparing `wagtail-localize-1.5/wagtail_localize/locale/it/LC_MESSAGES/djangojs.po` & `wagtail-localize-1.5.1/wagtail_localize/locale/it/LC_MESSAGES/djangojs.po`

 * *Files 10% similar despite different names*

```diff
@@ -1,34 +1,30 @@
 #
 # Translators:
 # Marco Lerco <marcolerco@gmail.com>, 2021
 # andrea tagliazucchi <andreatagliazucchi@gmail.com>, 2021
-# Alessio Di Stasio <aledista@gmail.com>, 2021
 # Stefano Marchetto <airbatum@gmail.com>, 2021
 # Giacomo Ghizzani <giacomo.ghz@gmail.com>, 2021
 # Marco Badan <marco.badan@gmail.com>, 2022
 #
 msgid ""
 msgstr ""
 "Last-Translator: Marco Badan <marco.badan@gmail.com>, 2022\n"
-"Language-Team: Italian (https://www.transifex.com/torchbox/teams/8009/it/)\n"
+"Language-Team: Italian (https://app.transifex.com/torchbox/teams/8009/it/)\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Language: it\n"
 "Plural-Forms: nplurals=3; plural=n == 1 ? 0 : n != 0 && n % 1000000 == 0 ? "
 "1 : 2;\n"
 
 msgid "[DELETED]"
 msgstr "[DELETED]"
 
 msgid "Apply editor lock"
 msgstr "Applica il blocco dell'editor"
 
-msgid "Breadcrumb"
-msgstr "Breadcrumb"
-
 msgid "Cancel"
 msgstr "Annulla"
 
 msgid "Change %s"
 msgstr "Cambia %s"
 
 msgid "Change document"
@@ -63,17 +59,14 @@
 
 msgid "Download PO file"
 msgstr "Scarica file PO"
 
 msgid "Download PO file and input translations offline"
 msgstr "Scarica file PO e inserisci le traduzioni offline"
 
-msgid "Draft"
-msgstr "Bozza"
-
 msgid "Edit"
 msgstr "Modifica"
 
 msgid "Edit this %s"
 msgstr "Modifica questo %s"
 
 msgid "Edit this document"
@@ -93,35 +86,26 @@
 
 msgid "Fetching image information..."
 msgstr "Raccolta informazioni immagine in corso..."
 
 msgid "Fetching page information..."
 msgstr "Raccolta informazioni pagina in corso..."
 
-msgid "Live"
-msgstr "Live"
-
 msgid "Lock"
 msgstr "Blocca"
 
 msgid "Not translated"
 msgstr "Non tradotto"
 
 msgid "Preview"
 msgstr "Anteprima"
 
 msgid "Publish in "
 msgstr "Pubblicata in"
 
-msgid "Published"
-msgstr "Pubblicata"
-
-msgid "Published on "
-msgstr "Pubblicata il"
-
 msgid "Publishing..."
 msgstr "Pubblicazione in corso..."
 
 msgid "Remove editor lock"
 msgstr "Rimuovi blocco editor"
 
 msgid "Revert to %s version"
```

### Comparing `wagtail-localize-1.5/wagtail_localize/locale/ja/LC_MESSAGES/django.mo` & `wagtail-localize-1.5.1/wagtail_localize/locale/ja/LC_MESSAGES/django.mo`

 * *Files 1% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,12 +1,12 @@
 msgid ""
 msgstr ""
 "Report-Msgid-Bugs-To: \n"
 "Last-Translator: shuhei hirota, 2022\n"
-"Language-Team: Japanese (https://www.transifex.com/torchbox/teams/8009/ja/)\n"
+"Language-Team: Japanese (https://app.transifex.com/torchbox/teams/8009/ja/)\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Language: ja\n"
 "Plural-Forms: nplurals=1; plural=0;\n"
 
 msgid "Content"
 msgstr "コンテンツ"
```

### Comparing `wagtail-localize-1.5/wagtail_localize/locale/ja/LC_MESSAGES/django.po` & `wagtail-localize-1.5.1/wagtail_localize/locale/ja/LC_MESSAGES/django.po`

 * *Files 16% similar despite different names*

```diff
@@ -5,17 +5,17 @@
 # Daigo Shitara <stain.witness@gmail.com>, 2022
 # Hiroki Sawano, 2022
 # shuhei hirota, 2022
 #
 msgid ""
 msgstr ""
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2022-10-17 21:00+0000\n"
+"POT-Creation-Date: 2023-02-23 14:15+0000\n"
 "Last-Translator: shuhei hirota, 2022\n"
-"Language-Team: Japanese (https://www.transifex.com/torchbox/teams/8009/ja/)\n"
+"Language-Team: Japanese (https://app.transifex.com/torchbox/teams/8009/ja/)\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Language: ja\n"
 "Plural-Forms: nplurals=1; plural=0;\n"
 
 msgid "Saving…"
 msgstr "保存中..."
```

### Comparing `wagtail-localize-1.5/wagtail_localize/locale/ja/LC_MESSAGES/djangojs.po` & `wagtail-localize-1.5.1/wagtail_localize/locale/ja/LC_MESSAGES/djangojs.po`

 * *Files 5% similar despite different names*

```diff
@@ -1,31 +1,27 @@
 #
 # Translators:
 # Tetsuya Morimoto <tetsuya.morimoto@gmail.com>, 2021
 # Daigo Shitara <stain.witness@gmail.com>, 2021
 # 石田秀 <ishidashu@gmail.com>, 2021
-# 山本 卓也 <takuya.miraidenshi@gmail.com>, 2021
 # Yudai Kobayashi <yudai.kobayashi.miraidenshi@gmail.com>, 2021
 # shuhei hirota, 2021
 # kojikojikojikoji, 2021
 #
 msgid ""
 msgstr ""
 "Last-Translator: kojikojikojikoji, 2021\n"
-"Language-Team: Japanese (https://www.transifex.com/torchbox/teams/8009/ja/)\n"
+"Language-Team: Japanese (https://app.transifex.com/torchbox/teams/8009/ja/)\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Language: ja\n"
 "Plural-Forms: nplurals=1; plural=0;\n"
 
 msgid "Apply editor lock"
 msgstr "エディターロック機能を適用する"
 
-msgid "Breadcrumb"
-msgstr "パンくず"
-
 msgid "Cancel"
 msgstr "キャンセル"
 
 msgid "Change image"
 msgstr "画像を変更"
 
 msgid "Change page"
@@ -39,17 +35,14 @@
 
 msgid "Choose an image"
 msgstr "画像を選択"
 
 msgid "Delete"
 msgstr "削除"
 
-msgid "Draft"
-msgstr "下書き"
-
 msgid "Edit"
 msgstr "編集"
 
 msgid "Edit this %s"
 msgstr "%sを編集"
 
 msgid "Edit this document"
@@ -57,17 +50,14 @@
 
 msgid "Edit this image"
 msgstr "画像を編集"
 
 msgid "Edit this page"
 msgstr "ページを編集"
 
-msgid "Live"
-msgstr "公開"
-
 msgid "Lock"
 msgstr "ロックする"
 
 msgid "Preview"
 msgstr "プレビュー"
 
 msgid "Publishing..."
```

### Comparing `wagtail-localize-1.5/wagtail_localize/locale/ka/LC_MESSAGES/django.po` & `wagtail-localize-1.5.1/wagtail_localize/locale/ka/LC_MESSAGES/django.po`

 * *Files 5% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 #
 # Translators:
 # André Bouatchidzé <a@anbz.net>, 2022
 #
 msgid ""
 msgstr ""
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2022-10-17 21:00+0000\n"
+"POT-Creation-Date: 2023-02-23 14:15+0000\n"
 "Last-Translator: André Bouatchidzé <a@anbz.net>, 2022\n"
-"Language-Team: Georgian (https://www.transifex.com/torchbox/teams/8009/ka/)\n"
+"Language-Team: Georgian (https://app.transifex.com/torchbox/teams/8009/ka/)\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Language: ka\n"
 "Plural-Forms: nplurals=2; plural=(n!=1);\n"
 
 msgid "Save"
 msgstr "შენახვა"
```

### Comparing `wagtail-localize-1.5/wagtail_localize/locale/ka/LC_MESSAGES/djangojs.mo` & `wagtail-localize-1.5.1/wagtail_localize/locale/ka/LC_MESSAGES/djangojs.mo`

 * *Files 13% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,11 +1,11 @@
 msgid ""
 msgstr ""
 "Last-Translator: André Bouatchidzé <a@anbz.net>, 2021\n"
-"Language-Team: Georgian (https://www.transifex.com/torchbox/teams/8009/ka/)\n"
+"Language-Team: Georgian (https://app.transifex.com/torchbox/teams/8009/ka/)\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Language: ka\n"
 "Plural-Forms: nplurals=2; plural=(n!=1);\n"
 
 msgid "Delete"
 msgstr "წაშლა"
```

### Comparing `wagtail-localize-1.5/wagtail_localize/locale/ka/LC_MESSAGES/djangojs.po` & `wagtail-localize-1.5.1/wagtail_localize/locale/ka/LC_MESSAGES/djangojs.po`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 #
 # Translators:
 # André Bouatchidzé <a@anbz.net>, 2021
 #
 msgid ""
 msgstr ""
 "Last-Translator: André Bouatchidzé <a@anbz.net>, 2021\n"
-"Language-Team: Georgian (https://www.transifex.com/torchbox/teams/8009/ka/)\n"
+"Language-Team: Georgian (https://app.transifex.com/torchbox/teams/8009/ka/)\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Language: ka\n"
 "Plural-Forms: nplurals=2; plural=(n!=1);\n"
 
 msgid "Delete"
 msgstr "წაშლა"
```

### Comparing `wagtail-localize-1.5/wagtail_localize/locale/ko/LC_MESSAGES/django.mo` & `wagtail-localize-1.5.1/wagtail_localize/locale/ko/LC_MESSAGES/django.mo`

 * *Files 1% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,12 +1,12 @@
 msgid ""
 msgstr ""
 "Report-Msgid-Bugs-To: \n"
 "Last-Translator: Kyungil Choi <hanpama@gmail.com>, 2022\n"
-"Language-Team: Korean (https://www.transifex.com/torchbox/teams/8009/ko/)\n"
+"Language-Team: Korean (https://app.transifex.com/torchbox/teams/8009/ko/)\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Language: ko\n"
 "Plural-Forms: nplurals=1; plural=0;\n"
 
 msgid "All child pages will be created."
 msgstr "모든 하위 페이지가 생성될 것"
```

### Comparing `wagtail-localize-1.5/wagtail_localize/locale/ko/LC_MESSAGES/django.po` & `wagtail-localize-1.5.1/wagtail_localize/locale/ko/LC_MESSAGES/django.po`

 * *Files 2% similar despite different names*

```diff
@@ -4,17 +4,17 @@
 # Kyu Choi, 2022
 # Dan Braghis, 2022
 # Kyungil Choi <hanpama@gmail.com>, 2022
 #
 msgid ""
 msgstr ""
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2022-10-17 21:00+0000\n"
+"POT-Creation-Date: 2023-02-23 14:15+0000\n"
 "Last-Translator: Kyungil Choi <hanpama@gmail.com>, 2022\n"
-"Language-Team: Korean (https://www.transifex.com/torchbox/teams/8009/ko/)\n"
+"Language-Team: Korean (https://app.transifex.com/torchbox/teams/8009/ko/)\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Language: ko\n"
 "Plural-Forms: nplurals=1; plural=0;\n"
 
 msgid "Disable"
 msgstr "불가한"
```

### Comparing `wagtail-localize-1.5/wagtail_localize/locale/ko/LC_MESSAGES/djangojs.mo` & `wagtail-localize-1.5.1/wagtail_localize/locale/ko/LC_MESSAGES/djangojs.mo`

 * *Files 22% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,21 +1,18 @@
 msgid ""
 msgstr ""
 "Last-Translator: Kyu Choi, 2022\n"
-"Language-Team: Korean (https://www.transifex.com/torchbox/teams/8009/ko/)\n"
+"Language-Team: Korean (https://app.transifex.com/torchbox/teams/8009/ko/)\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Language: ko\n"
 "Plural-Forms: nplurals=1; plural=0;\n"
 
 msgid "Apply editor lock"
 msgstr "편집자 잠금 적용"
 
-msgid "Breadcrumb"
-msgstr "브레드크럼"
-
 msgid "Cancel"
 msgstr "취소"
 
 msgid "Change image"
 msgstr "이미지 변경"
 
 msgid "Choose a document"
@@ -26,17 +23,14 @@
 
 msgid "Choose an image"
 msgstr "이미지 선택"
 
 msgid "Delete"
 msgstr "삭제"
 
-msgid "Draft"
-msgstr "초안"
-
 msgid "Edit"
 msgstr "수정"
 
 msgid "Edit this %s"
 msgstr "이 %s 수정하기"
 
 msgid "Edit this document"
@@ -44,26 +38,20 @@
 
 msgid "Edit this image"
 msgstr "이 이미지 수정"
 
 msgid "Edit this page"
 msgstr "페이지 변경"
 
-msgid "Live"
-msgstr "라이브"
-
 msgid "Lock"
 msgstr "잠금"
 
 msgid "Preview"
 msgstr "미리보기"
 
-msgid "Published"
-msgstr "출시된"
-
 msgid "Publishing..."
 msgstr "게시 중..."
 
 msgid "Remove editor lock"
 msgstr "편집자 잠금 제거"
 
 msgid "Save"
```

### Comparing `wagtail-localize-1.5/wagtail_localize/locale/ko/LC_MESSAGES/djangojs.po` & `wagtail-localize-1.5.1/wagtail_localize/locale/ko/LC_MESSAGES/djangojs.po`

 * *Files 18% similar despite different names*

```diff
@@ -3,25 +3,22 @@
 # Jihan Chung <jihanchung20@gmail.com>, 2021
 # Kyungil Choi <hanpama@gmail.com>, 2021
 # Kyu Choi, 2022
 #
 msgid ""
 msgstr ""
 "Last-Translator: Kyu Choi, 2022\n"
-"Language-Team: Korean (https://www.transifex.com/torchbox/teams/8009/ko/)\n"
+"Language-Team: Korean (https://app.transifex.com/torchbox/teams/8009/ko/)\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Language: ko\n"
 "Plural-Forms: nplurals=1; plural=0;\n"
 
 msgid "Apply editor lock"
 msgstr "편집자 잠금 적용"
 
-msgid "Breadcrumb"
-msgstr "브레드크럼"
-
 msgid "Cancel"
 msgstr "취소"
 
 msgid "Change image"
 msgstr "이미지 변경"
 
 msgid "Choose a document"
@@ -32,17 +29,14 @@
 
 msgid "Choose an image"
 msgstr "이미지 선택"
 
 msgid "Delete"
 msgstr "삭제"
 
-msgid "Draft"
-msgstr "초안"
-
 msgid "Edit"
 msgstr "수정"
 
 msgid "Edit this %s"
 msgstr "이 %s 수정하기"
 
 msgid "Edit this document"
@@ -50,26 +44,20 @@
 
 msgid "Edit this image"
 msgstr "이 이미지 수정"
 
 msgid "Edit this page"
 msgstr "페이지 변경"
 
-msgid "Live"
-msgstr "라이브"
-
 msgid "Lock"
 msgstr "잠금"
 
 msgid "Preview"
 msgstr "미리보기"
 
-msgid "Published"
-msgstr "출시된"
-
 msgid "Publishing..."
 msgstr "게시 중..."
 
 msgid "Remove editor lock"
 msgstr "편집자 잠금 제거"
 
 msgid "Save"
```

### Comparing `wagtail-localize-1.5/wagtail_localize/locale/lt/LC_MESSAGES/django.mo` & `wagtail-localize-1.5.1/wagtail_localize/locale/lt/LC_MESSAGES/django.mo`

 * *Files 0% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,12 +1,12 @@
 msgid ""
 msgstr ""
 "Report-Msgid-Bugs-To: \n"
 "Last-Translator: Matas Dailyda <matas@dailyda.com>, 2022\n"
-"Language-Team: Lithuanian (https://www.transifex.com/torchbox/teams/8009/"
+"Language-Team: Lithuanian (https://app.transifex.com/torchbox/teams/8009/"
 "lt/)\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Language: lt\n"
 "Plural-Forms: nplurals=4; plural=(n % 10 == 1 && (n % 100 > 19 || n % 100 < "
 "11) ? 0 : (n % 10 >= 2 && n % 10 <=9) && (n % 100 > 19 || n % 100 < 11) ? "
 "1 : n % 1 != 0 ? 2: 3);\n"
```

### Comparing `wagtail-localize-1.5/wagtail_localize/locale/lt/LC_MESSAGES/django.po` & `wagtail-localize-1.5.1/wagtail_localize/locale/lt/LC_MESSAGES/django.po`

 * *Files 1% similar despite different names*

```diff
@@ -2,17 +2,17 @@
 # Translators:
 # Naglis Jonaitis, 2022
 # Matas Dailyda <matas@dailyda.com>, 2022
 #
 msgid ""
 msgstr ""
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2022-10-17 21:00+0000\n"
+"POT-Creation-Date: 2023-02-23 14:15+0000\n"
 "Last-Translator: Matas Dailyda <matas@dailyda.com>, 2022\n"
-"Language-Team: Lithuanian (https://www.transifex.com/torchbox/teams/8009/"
+"Language-Team: Lithuanian (https://app.transifex.com/torchbox/teams/8009/"
 "lt/)\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Language: lt\n"
 "Plural-Forms: nplurals=4; plural=(n % 10 == 1 && (n % 100 > 19 || n % 100 < "
 "11) ? 0 : (n % 10 >= 2 && n % 10 <=9) && (n % 100 > 19 || n % 100 < 11) ? "
 "1 : n % 1 != 0 ? 2: 3);\n"
```

### Comparing `wagtail-localize-1.5/wagtail_localize/locale/lt/LC_MESSAGES/djangojs.mo` & `wagtail-localize-1.5.1/wagtail_localize/locale/lt/LC_MESSAGES/djangojs.mo`

 * *Files 10% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,24 +1,21 @@
 msgid ""
 msgstr ""
 "Last-Translator: Naglis Jonaitis, 2022\n"
-"Language-Team: Lithuanian (https://www.transifex.com/torchbox/teams/8009/"
+"Language-Team: Lithuanian (https://app.transifex.com/torchbox/teams/8009/"
 "lt/)\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Language: lt\n"
 "Plural-Forms: nplurals=4; plural=(n % 10 == 1 && (n % 100 > 19 || n % 100 < "
 "11) ? 0 : (n % 10 >= 2 && n % 10 <=9) && (n % 100 > 19 || n % 100 < 11) ? "
 "1 : n % 1 != 0 ? 2: 3);\n"
 
 msgid "Apply editor lock"
 msgstr "Taikyti redaktoriaus užraktą"
 
-msgid "Breadcrumb"
-msgstr "Naršymo kelias"
-
 msgid "Cancel"
 msgstr "Atšaukti"
 
 msgid "Change document"
 msgstr "Keisti dokumentą"
 
 msgid "Change image"
@@ -44,17 +41,14 @@
 
 msgid "Download PO file"
 msgstr "Parsisiųsti PO failą"
 
 msgid "Download PO file and input translations offline"
 msgstr "Parsisiųskite PO failą ir verskite atsijungę"
 
-msgid "Draft"
-msgstr "Juodraštis"
-
 msgid "Edit"
 msgstr "Redaguoti"
 
 msgid "Edit this %s"
 msgstr "Redaguoti šį %s"
 
 msgid "Edit this document"
@@ -71,35 +65,26 @@
 
 msgid "Fetching image information..."
 msgstr "Gaunama paveikslėlio informacija..."
 
 msgid "Fetching page information..."
 msgstr "Gaunama puslapio informacija..."
 
-msgid "Live"
-msgstr "Veikiantis"
-
 msgid "Lock"
 msgstr "Užrakinti"
 
 msgid "Not translated"
 msgstr "Neišversta"
 
 msgid "Preview"
 msgstr "Peržiūrėti"
 
 msgid "Publish in "
 msgstr "Publikuoti "
 
-msgid "Published"
-msgstr "Publikuotas"
-
-msgid "Published on "
-msgstr "Publikuotas"
-
 msgid "Publishing..."
 msgstr "Publikuojama..."
 
 msgid "Remove editor lock"
 msgstr "Pašalinti redaktoriaus užraktą"
 
 msgid "Save"
```

### Comparing `wagtail-localize-1.5/wagtail_localize/locale/lt/LC_MESSAGES/djangojs.po` & `wagtail-localize-1.5.1/wagtail_localize/locale/lt/LC_MESSAGES/djangojs.po`

 * *Files 8% similar despite different names*

```diff
@@ -2,31 +2,28 @@
 # Translators:
 # Matas Dailyda <matas@dailyda.com>, 2021
 # Naglis Jonaitis, 2022
 #
 msgid ""
 msgstr ""
 "Last-Translator: Naglis Jonaitis, 2022\n"
-"Language-Team: Lithuanian (https://www.transifex.com/torchbox/teams/8009/"
+"Language-Team: Lithuanian (https://app.transifex.com/torchbox/teams/8009/"
 "lt/)\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Language: lt\n"
 "Plural-Forms: nplurals=4; plural=(n % 10 == 1 && (n % 100 > 19 || n % 100 < "
 "11) ? 0 : (n % 10 >= 2 && n % 10 <=9) && (n % 100 > 19 || n % 100 < 11) ? "
 "1 : n % 1 != 0 ? 2: 3);\n"
 
 msgid "[DELETED]"
 msgstr "[IŠTRINTA]"
 
 msgid "Apply editor lock"
 msgstr "Taikyti redaktoriaus užraktą"
 
-msgid "Breadcrumb"
-msgstr "Naršymo kelias"
-
 msgid "Cancel"
 msgstr "Atšaukti"
 
 msgid "Change document"
 msgstr "Keisti dokumentą"
 
 msgid "Change image"
@@ -52,17 +49,14 @@
 
 msgid "Download PO file"
 msgstr "Parsisiųsti PO failą"
 
 msgid "Download PO file and input translations offline"
 msgstr "Parsisiųskite PO failą ir verskite atsijungę"
 
-msgid "Draft"
-msgstr "Juodraštis"
-
 msgid "Edit"
 msgstr "Redaguoti"
 
 msgid "Edit this %s"
 msgstr "Redaguoti šį %s"
 
 msgid "Edit this document"
@@ -79,35 +73,26 @@
 
 msgid "Fetching image information..."
 msgstr "Gaunama paveikslėlio informacija..."
 
 msgid "Fetching page information..."
 msgstr "Gaunama puslapio informacija..."
 
-msgid "Live"
-msgstr "Veikiantis"
-
 msgid "Lock"
 msgstr "Užrakinti"
 
 msgid "Not translated"
 msgstr "Neišversta"
 
 msgid "Preview"
 msgstr "Peržiūrėti"
 
 msgid "Publish in "
 msgstr "Publikuoti "
 
-msgid "Published"
-msgstr "Publikuotas"
-
-msgid "Published on "
-msgstr "Publikuotas"
-
 msgid "Publishing..."
 msgstr "Publikuojama..."
 
 msgid "Remove editor lock"
 msgstr "Pašalinti redaktoriaus užraktą"
 
 msgid "Save"
```

### Comparing `wagtail-localize-1.5/wagtail_localize/locale/lv/LC_MESSAGES/django.mo` & `wagtail-localize-1.5.1/wagtail_localize/locale/lv/LC_MESSAGES/django.mo`

 * *Files 2% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,12 +1,12 @@
 msgid ""
 msgstr ""
 "Report-Msgid-Bugs-To: \n"
 "Last-Translator: Reinis Rozenbergs <reinisr@gmail.com>, 2022\n"
-"Language-Team: Latvian (https://www.transifex.com/torchbox/teams/8009/lv/)\n"
+"Language-Team: Latvian (https://app.transifex.com/torchbox/teams/8009/lv/)\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Language: lv\n"
 "Plural-Forms: nplurals=3; plural=(n%10==1 && n%100!=11 ? 0 : n != 0 ? 1 : "
 "2);\n"
 
 msgid "Content"
 msgstr "Saturs"
```

### Comparing `wagtail-localize-1.5/wagtail_localize/locale/lv/LC_MESSAGES/django.po` & `wagtail-localize-1.5.1/wagtail_localize/locale/lv/LC_MESSAGES/django.po`

 * *Files 4% similar despite different names*

```diff
@@ -2,17 +2,17 @@
 # Translators:
 # Maris Serzans <maris.serzans@gmail.com>, 2022
 # Reinis Rozenbergs <reinisr@gmail.com>, 2022
 #
 msgid ""
 msgstr ""
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2022-10-17 21:00+0000\n"
+"POT-Creation-Date: 2023-02-23 14:15+0000\n"
 "Last-Translator: Reinis Rozenbergs <reinisr@gmail.com>, 2022\n"
-"Language-Team: Latvian (https://www.transifex.com/torchbox/teams/8009/lv/)\n"
+"Language-Team: Latvian (https://app.transifex.com/torchbox/teams/8009/lv/)\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Language: lv\n"
 "Plural-Forms: nplurals=3; plural=(n%10==1 && n%100!=11 ? 0 : n != 0 ? 1 : "
 "2);\n"
 
 msgid "Saving…"
 msgstr "Saglabā..."
```

### Comparing `wagtail-localize-1.5/wagtail_localize/locale/lv/LC_MESSAGES/djangojs.mo` & `wagtail-localize-1.5.1/wagtail_localize/locale/lv/LC_MESSAGES/djangojs.mo`

 * *Files 13% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,11 +1,11 @@
 msgid ""
 msgstr ""
 "Last-Translator: Maris Serzans <maris.serzans@gmail.com>, 2021\n"
-"Language-Team: Latvian (https://www.transifex.com/torchbox/teams/8009/lv/)\n"
+"Language-Team: Latvian (https://app.transifex.com/torchbox/teams/8009/lv/)\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Language: lv\n"
 "Plural-Forms: nplurals=3; plural=(n%10==1 && n%100!=11 ? 0 : n != 0 ? 1 : "
 "2);\n"
 
 msgid "Apply editor lock"
 msgstr "Pielietot redaktora slēgšanu"
@@ -18,17 +18,14 @@
 
 msgid "Choose an image"
 msgstr "Izvēlēties attēlu"
 
 msgid "Delete"
 msgstr "Dzēst"
 
-msgid "Draft"
-msgstr "Melnraksts"
-
 msgid "Edit"
 msgstr "Labot"
 
 msgid "Edit this %s"
 msgstr "Labot šo %s"
 
 msgid "Edit this document"
@@ -36,17 +33,14 @@
 
 msgid "Edit this image"
 msgstr "Labot šo attēlu"
 
 msgid "Edit this page"
 msgstr "Labot šo lapu"
 
-msgid "Live"
-msgstr "Aktīva"
-
 msgid "Lock"
 msgstr "Slēgt"
 
 msgid "Preview"
 msgstr "Priekšskatīt"
 
 msgid "Publishing..."
```

### Comparing `wagtail-localize-1.5/wagtail_localize/locale/lv/LC_MESSAGES/djangojs.po` & `wagtail-localize-1.5.1/wagtail_localize/locale/lv/LC_MESSAGES/djangojs.po`

 * *Files 10% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # Translators:
 # Reinis Rozenbergs <reinisr@gmail.com>, 2021
 # Maris Serzans <maris.serzans@gmail.com>, 2021
 #
 msgid ""
 msgstr ""
 "Last-Translator: Maris Serzans <maris.serzans@gmail.com>, 2021\n"
-"Language-Team: Latvian (https://www.transifex.com/torchbox/teams/8009/lv/)\n"
+"Language-Team: Latvian (https://app.transifex.com/torchbox/teams/8009/lv/)\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Language: lv\n"
 "Plural-Forms: nplurals=3; plural=(n%10==1 && n%100!=11 ? 0 : n != 0 ? 1 : "
 "2);\n"
 
 msgid "Apply editor lock"
 msgstr "Pielietot redaktora slēgšanu"
@@ -23,17 +23,14 @@
 
 msgid "Choose an image"
 msgstr "Izvēlēties attēlu"
 
 msgid "Delete"
 msgstr "Dzēst"
 
-msgid "Draft"
-msgstr "Melnraksts"
-
 msgid "Edit"
 msgstr "Labot"
 
 msgid "Edit this %s"
 msgstr "Labot šo %s"
 
 msgid "Edit this document"
@@ -41,17 +38,14 @@
 
 msgid "Edit this image"
 msgstr "Labot šo attēlu"
 
 msgid "Edit this page"
 msgstr "Labot šo lapu"
 
-msgid "Live"
-msgstr "Aktīva"
-
 msgid "Lock"
 msgstr "Slēgt"
 
 msgid "Preview"
 msgstr "Priekšskatīt"
 
 msgid "Publishing..."
```

### Comparing `wagtail-localize-1.5/wagtail_localize/locale/mi/LC_MESSAGES/django.mo` & `wagtail-localize-1.5.1/wagtail_localize/locale/mi/LC_MESSAGES/django.mo`

 * *Files 2% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,12 +1,12 @@
 msgid ""
 msgstr ""
 "Report-Msgid-Bugs-To: \n"
 "Last-Translator: Awatea Randall <awatea@octave.nz>, 2022\n"
-"Language-Team: Maori (https://www.transifex.com/torchbox/teams/8009/mi/)\n"
+"Language-Team: Maori (https://app.transifex.com/torchbox/teams/8009/mi/)\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Language: mi\n"
 "Plural-Forms: nplurals=2; plural=(n > 1);\n"
 
 msgid "Content"
 msgstr "Rārangi take"
```

### Comparing `wagtail-localize-1.5/wagtail_localize/locale/mi/LC_MESSAGES/django.po` & `wagtail-localize-1.5.1/wagtail_localize/locale/mi/LC_MESSAGES/django.po`

 * *Files 3% similar despite different names*

```diff
@@ -2,17 +2,17 @@
 # Translators:
 # Dan Braghis, 2022
 # Awatea Randall <awatea@octave.nz>, 2022
 #
 msgid ""
 msgstr ""
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2022-10-17 21:00+0000\n"
+"POT-Creation-Date: 2023-02-23 14:15+0000\n"
 "Last-Translator: Awatea Randall <awatea@octave.nz>, 2022\n"
-"Language-Team: Maori (https://www.transifex.com/torchbox/teams/8009/mi/)\n"
+"Language-Team: Maori (https://app.transifex.com/torchbox/teams/8009/mi/)\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Language: mi\n"
 "Plural-Forms: nplurals=2; plural=(n > 1);\n"
 
 msgid "Dummy translator"
 msgstr "Tohipa whakamāori"
```

### Comparing `wagtail-localize-1.5/wagtail_localize/locale/mn/LC_MESSAGES/django.mo` & `wagtail-localize-1.5.1/wagtail_localize/locale/mn/LC_MESSAGES/django.mo`

 * *Files 2% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,12 +1,12 @@
 msgid ""
 msgstr ""
 "Report-Msgid-Bugs-To: \n"
 "Last-Translator: visual, 2022\n"
-"Language-Team: Mongolian (https://www.transifex.com/torchbox/teams/8009/"
+"Language-Team: Mongolian (https://app.transifex.com/torchbox/teams/8009/"
 "mn/)\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Language: mn\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
 
 msgid "Content"
 msgstr "Контент"
```

### Comparing `wagtail-localize-1.5/wagtail_localize/locale/mn/LC_MESSAGES/django.po` & `wagtail-localize-1.5.1/wagtail_localize/locale/mn/LC_MESSAGES/django.po`

 * *Files 16% similar despite different names*

```diff
@@ -2,17 +2,17 @@
 # Translators:
 # Myagmarjav Enkhbileg <miigaa.lucky@gmail.com>, 2022
 # visual, 2022
 #
 msgid ""
 msgstr ""
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2022-10-17 21:00+0000\n"
+"POT-Creation-Date: 2023-02-23 14:15+0000\n"
 "Last-Translator: visual, 2022\n"
-"Language-Team: Mongolian (https://www.transifex.com/torchbox/teams/8009/"
+"Language-Team: Mongolian (https://app.transifex.com/torchbox/teams/8009/"
 "mn/)\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Language: mn\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
 
 msgid "Saving…"
 msgstr "Хадгалж байна..."
```

### Comparing `wagtail-localize-1.5/wagtail_localize/locale/mn/LC_MESSAGES/djangojs.mo` & `wagtail-localize-1.5.1/wagtail_localize/locale/mn/LC_MESSAGES/djangojs.mo`

 * *Files 12% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,11 +1,11 @@
 msgid ""
 msgstr ""
 "Last-Translator: visual, 2022\n"
-"Language-Team: Mongolian (https://www.transifex.com/torchbox/teams/8009/"
+"Language-Team: Mongolian (https://app.transifex.com/torchbox/teams/8009/"
 "mn/)\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Language: mn\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
 
 msgid "Change image"
 msgstr "Зураг солих"
@@ -18,17 +18,14 @@
 
 msgid "Choose an image"
 msgstr "Зургаа сонгоно уу"
 
 msgid "Delete"
 msgstr "Устгах"
 
-msgid "Draft"
-msgstr "Ноорог"
-
 msgid "Edit"
 msgstr "Засах"
 
 msgid "Edit this %s"
 msgstr "%s-г засах"
 
 msgid "Edit this document"
@@ -36,17 +33,14 @@
 
 msgid "Edit this image"
 msgstr "Энэ зургийг засах"
 
 msgid "Edit this page"
 msgstr "Энэ хуудсыг засах"
 
-msgid "Live"
-msgstr "Шууд"
-
 msgid "Lock"
 msgstr "Түгжих"
 
 msgid "Preview"
 msgstr "Урдчилж харах"
 
 msgid "Save"
```

### Comparing `wagtail-localize-1.5/wagtail_localize/locale/mn/LC_MESSAGES/djangojs.po` & `wagtail-localize-1.5.1/wagtail_localize/locale/mn/LC_MESSAGES/djangojs.po`

 * *Files 10% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 # Delgermurun Purevkhuuu <info@delgermurun.com>, 2021
 # Myagmarjav Enkhbileg <miigaa.lucky@gmail.com>, 2021
 # visual, 2022
 #
 msgid ""
 msgstr ""
 "Last-Translator: visual, 2022\n"
-"Language-Team: Mongolian (https://www.transifex.com/torchbox/teams/8009/"
+"Language-Team: Mongolian (https://app.transifex.com/torchbox/teams/8009/"
 "mn/)\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Language: mn\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
 
 msgid "Change image"
 msgstr "Зураг солих"
@@ -24,17 +24,14 @@
 
 msgid "Choose an image"
 msgstr "Зургаа сонгоно уу"
 
 msgid "Delete"
 msgstr "Устгах"
 
-msgid "Draft"
-msgstr "Ноорог"
-
 msgid "Edit"
 msgstr "Засах"
 
 msgid "Edit this %s"
 msgstr "%s-г засах"
 
 msgid "Edit this document"
@@ -42,17 +39,14 @@
 
 msgid "Edit this image"
 msgstr "Энэ зургийг засах"
 
 msgid "Edit this page"
 msgstr "Энэ хуудсыг засах"
 
-msgid "Live"
-msgstr "Шууд"
-
 msgid "Lock"
 msgstr "Түгжих"
 
 msgid "Preview"
 msgstr "Урдчилж харах"
 
 msgid "Save"
```

### Comparing `wagtail-localize-1.5/wagtail_localize/locale/my/LC_MESSAGES/django.mo` & `wagtail-localize-1.5.1/wagtail_localize/locale/my/LC_MESSAGES/django.mo`

 * *Files 2% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,12 +1,12 @@
 msgid ""
 msgstr ""
 "Report-Msgid-Bugs-To: \n"
 "Last-Translator: ime11 <pmh.yourworstnightmare@gmail.com>, 2022\n"
-"Language-Team: Burmese (https://www.transifex.com/torchbox/teams/8009/my/)\n"
+"Language-Team: Burmese (https://app.transifex.com/torchbox/teams/8009/my/)\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Language: my\n"
 "Plural-Forms: nplurals=1; plural=0;\n"
 
 msgid "Delete"
 msgstr "ဖျက်သိမ်းပါ"
```

### Comparing `wagtail-localize-1.5/wagtail_localize/locale/my/LC_MESSAGES/django.po` & `wagtail-localize-1.5.1/wagtail_localize/locale/my/LC_MESSAGES/django.po`

 * *Files 4% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 #
 # Translators:
 # ime11 <pmh.yourworstnightmare@gmail.com>, 2022
 #
 msgid ""
 msgstr ""
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2022-10-17 21:00+0000\n"
+"POT-Creation-Date: 2023-02-23 14:15+0000\n"
 "Last-Translator: ime11 <pmh.yourworstnightmare@gmail.com>, 2022\n"
-"Language-Team: Burmese (https://www.transifex.com/torchbox/teams/8009/my/)\n"
+"Language-Team: Burmese (https://app.transifex.com/torchbox/teams/8009/my/)\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Language: my\n"
 "Plural-Forms: nplurals=1; plural=0;\n"
 
 msgid "Saving…"
 msgstr "သိမ်းဆည်းနေသည်..."
```

### Comparing `wagtail-localize-1.5/wagtail_localize/locale/nb/LC_MESSAGES/django.mo` & `wagtail-localize-1.5.1/wagtail_localize/locale/nb/LC_MESSAGES/django.mo`

 * *Files 2% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,12 +1,12 @@
 msgid ""
 msgstr ""
 "Report-Msgid-Bugs-To: \n"
 "Last-Translator: Stein Strindhaug <stein.strindhaug@gmail.com>, 2022\n"
-"Language-Team: Norwegian Bokmål (https://www.transifex.com/torchbox/"
+"Language-Team: Norwegian Bokmål (https://app.transifex.com/torchbox/"
 "teams/8009/nb/)\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Language: nb\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
 
 msgid "Content"
 msgstr "Innhold"
```

### Comparing `wagtail-localize-1.5/wagtail_localize/locale/nb/LC_MESSAGES/django.po` & `wagtail-localize-1.5.1/wagtail_localize/locale/nb/LC_MESSAGES/django.po`

 * *Files 16% similar despite different names*

```diff
@@ -3,17 +3,17 @@
 # Eirik Krogstad <eirikkr@gmail.com>, 2021
 # Ole Kristian Losvik <ole@losol.no>, 2022
 # Stein Strindhaug <stein.strindhaug@gmail.com>, 2022
 #
 msgid ""
 msgstr ""
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2022-10-17 21:00+0000\n"
+"POT-Creation-Date: 2023-02-23 14:15+0000\n"
 "Last-Translator: Stein Strindhaug <stein.strindhaug@gmail.com>, 2022\n"
-"Language-Team: Norwegian Bokmål (https://www.transifex.com/torchbox/"
+"Language-Team: Norwegian Bokmål (https://app.transifex.com/torchbox/"
 "teams/8009/nb/)\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Language: nb\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
 
 msgid "Saving…"
 msgstr "Lagrer..."
```

### Comparing `wagtail-localize-1.5/wagtail_localize/locale/nb/LC_MESSAGES/djangojs.mo` & `wagtail-localize-1.5.1/wagtail_localize/locale/nb/LC_MESSAGES/djangojs.mo`

 * *Files 27% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,22 +1,19 @@
 msgid ""
 msgstr ""
 "Last-Translator: Stein Strindhaug <stein.strindhaug@gmail.com>, 2021\n"
-"Language-Team: Norwegian Bokmål (https://www.transifex.com/torchbox/"
+"Language-Team: Norwegian Bokmål (https://app.transifex.com/torchbox/"
 "teams/8009/nb/)\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Language: nb\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
 
 msgid "Apply editor lock"
 msgstr "Slå på redigeringslås"
 
-msgid "Breadcrumb"
-msgstr "Brødsmuler"
-
 msgid "Change image"
 msgstr "Velg et annet bilde"
 
 msgid "Choose a document"
 msgstr "Velg et dokument"
 
 msgid "Choose a page"
@@ -24,17 +21,14 @@
 
 msgid "Choose an image"
 msgstr "Velg et bilde"
 
 msgid "Delete"
 msgstr "Slett"
 
-msgid "Draft"
-msgstr "Kladd"
-
 msgid "Edit"
 msgstr "Rediger"
 
 msgid "Edit this %s"
 msgstr "Endre %s"
 
 msgid "Edit this document"
@@ -42,17 +36,14 @@
 
 msgid "Edit this image"
 msgstr "Rediger dette bildet"
 
 msgid "Edit this page"
 msgstr "Redigér denne siden"
 
-msgid "Live"
-msgstr "Publisert"
-
 msgid "Lock"
 msgstr "Lås"
 
 msgid "Preview"
 msgstr "Forhåndsvis"
 
 msgid "Publishing..."
```

### Comparing `wagtail-localize-1.5/wagtail_localize/locale/nb/LC_MESSAGES/djangojs.po` & `wagtail-localize-1.5.1/wagtail_localize/locale/nb/LC_MESSAGES/djangojs.po`

 * *Files 4% similar despite different names*

```diff
@@ -4,26 +4,23 @@
 # Robin Skahjem-Eriksen <robinds@student.matnat.uio.no>, 2021
 # Ole Kristian Losvik <ole@losol.no>, 2021
 # Stein Strindhaug <stein.strindhaug@gmail.com>, 2021
 #
 msgid ""
 msgstr ""
 "Last-Translator: Stein Strindhaug <stein.strindhaug@gmail.com>, 2021\n"
-"Language-Team: Norwegian Bokmål (https://www.transifex.com/torchbox/"
+"Language-Team: Norwegian Bokmål (https://app.transifex.com/torchbox/"
 "teams/8009/nb/)\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Language: nb\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
 
 msgid "Apply editor lock"
 msgstr "Slå på redigeringslås"
 
-msgid "Breadcrumb"
-msgstr "Brødsmuler"
-
 msgid "Change image"
 msgstr "Velg et annet bilde"
 
 msgid "Choose a document"
 msgstr "Velg et dokument"
 
 msgid "Choose a page"
@@ -31,17 +28,14 @@
 
 msgid "Choose an image"
 msgstr "Velg et bilde"
 
 msgid "Delete"
 msgstr "Slett"
 
-msgid "Draft"
-msgstr "Kladd"
-
 msgid "Edit"
 msgstr "Rediger"
 
 msgid "Edit this %s"
 msgstr "Endre %s"
 
 msgid "Edit this document"
@@ -49,17 +43,14 @@
 
 msgid "Edit this image"
 msgstr "Rediger dette bildet"
 
 msgid "Edit this page"
 msgstr "Redigér denne siden"
 
-msgid "Live"
-msgstr "Publisert"
-
 msgid "Lock"
 msgstr "Lås"
 
 msgid "Preview"
 msgstr "Forhåndsvis"
 
 msgid "Publishing..."
```

### Comparing `wagtail-localize-1.5/wagtail_localize/locale/nl/LC_MESSAGES/django.mo` & `wagtail-localize-1.5.1/wagtail_localize/locale/nl/LC_MESSAGES/django.mo`

 * *Files 0% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,12 +1,12 @@
 msgid ""
 msgstr ""
 "Report-Msgid-Bugs-To: \n"
 "Last-Translator: Storm Heg <storm@stormbase.digital>, 2022\n"
-"Language-Team: Dutch (https://www.transifex.com/torchbox/teams/8009/nl/)\n"
+"Language-Team: Dutch (https://app.transifex.com/torchbox/teams/8009/nl/)\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Language: nl\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
 
 msgid ""
 "<{}> tag is not allowed. Strings can only contain standard HTML inline tags "
 "(such as <b>, <a>)"
```

### Comparing `wagtail-localize-1.5/wagtail_localize/locale/nl/LC_MESSAGES/django.po` & `wagtail-localize-1.5.1/wagtail_localize/locale/nl/LC_MESSAGES/django.po`

 * *Files 1% similar despite different names*

```diff
@@ -6,17 +6,17 @@
 # Thijs Kramer <thijskramer@gmail.com>, 2022
 # Loic Teixeira, 2022
 # Storm Heg <storm@stormbase.digital>, 2022
 #
 msgid ""
 msgstr ""
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2022-10-17 21:00+0000\n"
+"POT-Creation-Date: 2023-02-23 14:15+0000\n"
 "Last-Translator: Storm Heg <storm@stormbase.digital>, 2022\n"
-"Language-Team: Dutch (https://www.transifex.com/torchbox/teams/8009/nl/)\n"
+"Language-Team: Dutch (https://app.transifex.com/torchbox/teams/8009/nl/)\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Language: nl\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
 
 msgid "Disable"
 msgstr "Uitschakelen"
```

### Comparing `wagtail-localize-1.5/wagtail_localize/locale/nl/LC_MESSAGES/djangojs.mo` & `wagtail-localize-1.5.1/wagtail_localize/locale/nl/LC_MESSAGES/djangojs.mo`

 * *Files 10% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,20 +1,17 @@
 msgid ""
 msgstr ""
-"Last-Translator: Thijs Kramer <thijskramer@gmail.com>, 2022\n"
-"Language-Team: Dutch (https://www.transifex.com/torchbox/teams/8009/nl/)\n"
+"Last-Translator: Storm Heg <storm@stormbase.digital>, 2023\n"
+"Language-Team: Dutch (https://app.transifex.com/torchbox/teams/8009/nl/)\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Language: nl\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
 
 msgid "Apply editor lock"
-msgstr "Pas bewerkingsblokkade toe"
-
-msgid "Breadcrumb"
-msgstr "Broodkruimel"
+msgstr "Bewerkingsvergrendeling inschakelen"
 
 msgid "Cancel"
 msgstr "Annuleren"
 
 msgid "Change %s"
 msgstr "Wijzig %s"
 
@@ -50,17 +47,14 @@
 
 msgid "Download PO file"
 msgstr "Download PO-bestand"
 
 msgid "Download PO file and input translations offline"
 msgstr "Download PO-bestand en voer offline vertalingen in"
 
-msgid "Draft"
-msgstr "Concept"
-
 msgid "Edit"
 msgstr "Bewerk"
 
 msgid "Edit this %s"
 msgstr "Wijzig %s"
 
 msgid "Edit this document"
@@ -80,35 +74,26 @@
 
 msgid "Fetching image information..."
 msgstr "Bezig met ophalen van afbeeldingsgegevens..."
 
 msgid "Fetching page information..."
 msgstr "Bezig met ophalen van paginagegevens..."
 
-msgid "Live"
-msgstr "Openbaar"
-
 msgid "Lock"
 msgstr "Vergrendel"
 
 msgid "Not translated"
 msgstr "Niet vertaald"
 
 msgid "Preview"
 msgstr "Voorvertoning"
 
 msgid "Publish in "
 msgstr "Publiceer in"
 
-msgid "Published"
-msgstr "Gepubliceerd"
-
-msgid "Published on "
-msgstr "Gepubliceerd op"
-
 msgid "Publishing..."
 msgstr "Bezig met publiceren..."
 
 msgid "Remove editor lock"
 msgstr "Verwijder bewerkingsblokkade"
 
 msgid "Revert to %s version"
@@ -139,15 +124,15 @@
 msgid "Translate with "
 msgstr "Vertaal met"
 
 msgid "Unlock"
 msgstr "Ontgrendelen"
 
 msgid "Unpublish"
-msgstr "Depubliceren"
+msgstr "Publicatie intrekken"
 
 msgid "Upload PO file"
 msgstr "Upload PO-bestand"
 
 msgid "Upload translated PO file to submit translations"
 msgstr "Upload vertaald PO-bestand om vertalingen te verzenden"
```

### Comparing `wagtail-localize-1.5/wagtail_localize/locale/nl/LC_MESSAGES/djangojs.po` & `wagtail-localize-1.5.1/wagtail_localize/locale/nl/LC_MESSAGES/djangojs.po`

 * *Files 19% similar despite different names*

```diff
@@ -1,31 +1,29 @@
 #
 # Translators:
 # benny_AT_it_digin.com <benny@it-digin.com>, 2021
 # mahulst, 2021
 # Rob Moorman <rob@moori.nl>, 2021
 # Loic Teixeira, 2021
 # Thijs Kramer <thijskramer@gmail.com>, 2022
+# Storm Heg <storm@stormbase.digital>, 2023
 #
 msgid ""
 msgstr ""
-"Last-Translator: Thijs Kramer <thijskramer@gmail.com>, 2022\n"
-"Language-Team: Dutch (https://www.transifex.com/torchbox/teams/8009/nl/)\n"
+"Last-Translator: Storm Heg <storm@stormbase.digital>, 2023\n"
+"Language-Team: Dutch (https://app.transifex.com/torchbox/teams/8009/nl/)\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Language: nl\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
 
 msgid "[DELETED]"
 msgstr "[VERWIJDERD]"
 
 msgid "Apply editor lock"
-msgstr "Pas bewerkingsblokkade toe"
-
-msgid "Breadcrumb"
-msgstr "Broodkruimel"
+msgstr "Bewerkingsvergrendeling inschakelen"
 
 msgid "Cancel"
 msgstr "Annuleren"
 
 msgid "Change %s"
 msgstr "Wijzig %s"
 
@@ -61,17 +59,14 @@
 
 msgid "Download PO file"
 msgstr "Download PO-bestand"
 
 msgid "Download PO file and input translations offline"
 msgstr "Download PO-bestand en voer offline vertalingen in"
 
-msgid "Draft"
-msgstr "Concept"
-
 msgid "Edit"
 msgstr "Bewerk"
 
 msgid "Edit this %s"
 msgstr "Wijzig %s"
 
 msgid "Edit this document"
@@ -91,35 +86,26 @@
 
 msgid "Fetching image information..."
 msgstr "Bezig met ophalen van afbeeldingsgegevens..."
 
 msgid "Fetching page information..."
 msgstr "Bezig met ophalen van paginagegevens..."
 
-msgid "Live"
-msgstr "Openbaar"
-
 msgid "Lock"
 msgstr "Vergrendel"
 
 msgid "Not translated"
 msgstr "Niet vertaald"
 
 msgid "Preview"
 msgstr "Voorvertoning"
 
 msgid "Publish in "
 msgstr "Publiceer in"
 
-msgid "Published"
-msgstr "Gepubliceerd"
-
-msgid "Published on "
-msgstr "Gepubliceerd op"
-
 msgid "Publishing..."
 msgstr "Bezig met publiceren..."
 
 msgid "Remove editor lock"
 msgstr "Verwijder bewerkingsblokkade"
 
 msgid "Revert to %s version"
@@ -153,15 +139,15 @@
 msgid "Translate with "
 msgstr "Vertaal met"
 
 msgid "Unlock"
 msgstr "Ontgrendelen"
 
 msgid "Unpublish"
-msgstr "Depubliceren"
+msgstr "Publicatie intrekken"
 
 msgid "Upload PO file"
 msgstr "Upload PO-bestand"
 
 msgid "Upload translated PO file to submit translations"
 msgstr "Upload vertaald PO-bestand om vertalingen te verzenden"
```

### Comparing `wagtail-localize-1.5/wagtail_localize/locale/nl_NL/LC_MESSAGES/django.mo` & `wagtail-localize-1.5.1/wagtail_localize/locale/nl_NL/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `wagtail-localize-1.5/wagtail_localize/locale/nl_NL/LC_MESSAGES/djangojs.mo` & `wagtail-localize-1.5.1/wagtail_localize/locale/sv/LC_MESSAGES/djangojs.mo`

 * *Files 21% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,143 +1,147 @@
 msgid ""
 msgstr ""
-"Last-Translator: Coen van der Kamp <cvanderkamp@gmail.com>, 2021\n"
-"Language-Team: Dutch (Netherlands) (https://www.transifex.com/torchbox/"
-"teams/8009/nl_NL/)\n"
+"Last-Translator: Philip Andersen <renegadevi@codeofmagi.net>, 2022\n"
+"Language-Team: Swedish (https://app.transifex.com/torchbox/teams/8009/sv/)\n"
 "Content-Type: text/plain; charset=UTF-8\n"
-"Language: nl_NL\n"
+"Language: sv\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
 
 msgid "Apply editor lock"
-msgstr "Pas bewerkingsblokkade toe"
-
-msgid "Breadcrumb"
-msgstr "Broodkruimel"
+msgstr "Tillämpa redaktörslås"
 
 msgid "Cancel"
-msgstr "Annuleren"
+msgstr "Avbryt"
+
+msgid "Change %s"
+msgstr "Ändra %s"
 
 msgid "Change document"
-msgstr "Wijzig document"
+msgstr "Ändra dokument"
 
 msgid "Change image"
-msgstr "Wijzig afbeelding"
+msgstr "Ändra bild"
 
 msgid "Change page"
-msgstr "Wijzig pagina"
+msgstr "Ändra sida"
 
 msgid "Changed"
-msgstr "Gewijzigd"
+msgstr "Ändrad"
+
+msgid "Choose a %s"
+msgstr "Välj en %s"
 
 msgid "Choose a document"
-msgstr "Kies een document"
+msgstr "Välj ett dokument"
 
 msgid "Choose a page"
-msgstr "Kies een pagina"
+msgstr "Välj en sida"
 
 msgid "Choose an image"
-msgstr "Kies een afbeelding"
+msgstr "Välj en bild"
+
+msgid "Convert to alias page"
+msgstr "Konvertera till alias"
 
 msgid "Delete"
-msgstr "Verwijderen"
+msgstr "Radera"
 
 msgid "Download PO file"
-msgstr "Download PO-bestand"
+msgstr "Ladda ner PO fil"
 
 msgid "Download PO file and input translations offline"
-msgstr "Download PO-bestand en voer offline vertalingen in"
-
-msgid "Draft"
-msgstr "Concept"
+msgstr "Ladda ner PO fil och uppdatera översättningar offline"
 
 msgid "Edit"
-msgstr "Bewerk"
+msgstr "Redigera"
 
 msgid "Edit this %s"
-msgstr "Wijzig %s"
+msgstr "Redigera %s"
 
 msgid "Edit this document"
-msgstr "Bewerk dit document"
+msgstr "Redigera detta dokument"
 
 msgid "Edit this image"
-msgstr "Bewerk deze afbeelding"
+msgstr "Redigera denna bild"
 
 msgid "Edit this page"
-msgstr "Bewerk deze pagina"
+msgstr "Redigera denna sida"
+
+msgid "Fetching %s information..."
+msgstr "Hämtar %s information..."
 
 msgid "Fetching document information..."
-msgstr "Bezig met ophalen van documentgegevens..."
+msgstr "Hämtar dokumentinformation"
 
 msgid "Fetching image information..."
-msgstr "Bezig met ophalen van afbeeldingsgegevens..."
+msgstr "Hämtar bildinformation"
 
 msgid "Fetching page information..."
-msgstr "Bezig met ophalen van paginagegevens..."
-
-msgid "Live"
-msgstr "Openbaar"
+msgstr "Hämtar sidoinformation"
 
 msgid "Lock"
-msgstr "Vergrendel"
+msgstr "Lås"
 
 msgid "Not translated"
-msgstr "Niet vertaald"
+msgstr "Inte översatt"
 
 msgid "Preview"
-msgstr "Voorvertoning"
+msgstr "Förhandsgranska"
 
 msgid "Publish in "
-msgstr "Publiceer in"
-
-msgid "Published"
-msgstr "Gepubliceerd"
-
-msgid "Published on "
-msgstr "Gepubliceerd op"
+msgstr "Publicera på"
 
 msgid "Publishing..."
-msgstr "Bezig met publiceren..."
+msgstr "Publicerar..."
 
 msgid "Remove editor lock"
-msgstr "Verwijder bewerkingsblokkade"
+msgstr "Ta bort redaktörslås"
+
+msgid "Revert to %s version"
+msgstr "Återställ till %s version"
 
 msgid "Save"
-msgstr "Opslaan"
+msgstr "Spara"
 
 msgid "Saving..."
-msgstr "Bezig met opslaan..."
+msgstr "Sparar..."
 
 msgid "Server error"
-msgstr "Server error"
+msgstr "Serverfel"
+
+msgid "Stop Synced translation"
+msgstr "Stoppa synkroniserad översättning"
 
-msgid "Stop translation"
-msgstr "Stop vertaling"
+msgid "There are unsaved segments. Please save or cancel them before leaving."
+msgstr ""
+"Det finns osparade segment. Vänligen spara eller återställ dem innan du "
+"lämnar."
 
 msgid "Translate"
-msgstr "Vertaal"
+msgstr "Översätt"
 
 msgid "Translate all missing strings with "
-msgstr "Vertaal alle ontbrekende teksten met"
+msgstr "Översätt alla saknade strängar med"
 
 msgid "Translate with "
-msgstr "Vertaal met"
+msgstr "Översätt med"
 
 msgid "Unlock"
-msgstr "Ontgrendelen"
+msgstr "Lås upp"
 
 msgid "Unpublish"
-msgstr "Depubliceren"
+msgstr "Avpublicera"
 
 msgid "Upload PO file"
-msgstr "Upload PO-bestand"
+msgstr "Ladda upp PO fil"
 
 msgid "Upload translated PO file to submit translations"
-msgstr "Upload vertaald PO-bestand om vertalingen te verzenden"
+msgstr "Ladda upp översatt PO-fil för att spara översättningar"
 
 msgid "Uses %s version"
-msgstr "Gebruikt %s versie"
+msgstr "Använder version %s "
 
 msgid "[DELETED]"
-msgstr "[VERWIJDERD]"
+msgstr "[RADERAD]"
 
 msgid "segments translated"
-msgstr "vertaalde segmenten"
+msgstr "segment översatta"
```

### Comparing `wagtail-localize-1.5/wagtail_localize/locale/pl/LC_MESSAGES/django.mo` & `wagtail-localize-1.5.1/wagtail_localize/locale/pl/LC_MESSAGES/django.mo`

 * *Files 2% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,12 +1,12 @@
 msgid ""
 msgstr ""
 "Report-Msgid-Bugs-To: \n"
 "Last-Translator: Miłosz Miśkiewicz, 2023\n"
-"Language-Team: Polish (https://www.transifex.com/torchbox/teams/8009/pl/)\n"
+"Language-Team: Polish (https://app.transifex.com/torchbox/teams/8009/pl/)\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Language: pl\n"
 "Plural-Forms: nplurals=4; plural=(n==1 ? 0 : (n%10>=2 && n%10<=4) && "
 "(n%100<12 || n%100>14) ? 1 : n!=1 && (n%10>=0 && n%10<=1) || (n%10>=5 && "
 "n%10<=9) || (n%100>=12 && n%100<=14) ? 2 : 3);\n"
 
 msgid ""
```

### Comparing `wagtail-localize-1.5/wagtail_localize/locale/pl/LC_MESSAGES/django.po` & `wagtail-localize-1.5.1/wagtail_localize/locale/pl/LC_MESSAGES/django.po`

 * *Files 1% similar despite different names*

```diff
@@ -4,17 +4,17 @@
 # Łukasz Bołdys (Lukasz Boldys), 2021
 # Dominik Lech, 2022
 # Miłosz Miśkiewicz, 2023
 #
 msgid ""
 msgstr ""
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2022-10-17 21:00+0000\n"
+"POT-Creation-Date: 2023-02-23 14:15+0000\n"
 "Last-Translator: Miłosz Miśkiewicz, 2023\n"
-"Language-Team: Polish (https://www.transifex.com/torchbox/teams/8009/pl/)\n"
+"Language-Team: Polish (https://app.transifex.com/torchbox/teams/8009/pl/)\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Language: pl\n"
 "Plural-Forms: nplurals=4; plural=(n==1 ? 0 : (n%10>=2 && n%10<=4) && "
 "(n%100<12 || n%100>14) ? 1 : n!=1 && (n%10>=0 && n%10<=1) || (n%10>=5 && "
 "n%10<=9) || (n%100>=12 && n%100<=14) ? 2 : 3);\n"
 
 msgid "Disable"
```

### Comparing `wagtail-localize-1.5/wagtail_localize/locale/pl/LC_MESSAGES/djangojs.mo` & `wagtail-localize-1.5.1/wagtail_localize/locale/pl/LC_MESSAGES/djangojs.mo`

 * *Files 15% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,23 +1,20 @@
 msgid ""
 msgstr ""
 "Last-Translator: Miłosz Miśkiewicz, 2023\n"
-"Language-Team: Polish (https://www.transifex.com/torchbox/teams/8009/pl/)\n"
+"Language-Team: Polish (https://app.transifex.com/torchbox/teams/8009/pl/)\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Language: pl\n"
 "Plural-Forms: nplurals=4; plural=(n==1 ? 0 : (n%10>=2 && n%10<=4) && "
 "(n%100<12 || n%100>14) ? 1 : n!=1 && (n%10>=0 && n%10<=1) || (n%10>=5 && "
 "n%10<=9) || (n%100>=12 && n%100<=14) ? 2 : 3);\n"
 
 msgid "Apply editor lock"
 msgstr "Zastosuj blokadę edytorską"
 
-msgid "Breadcrumb"
-msgstr "Breadcrumb"
-
 msgid "Cancel"
 msgstr "Anuluj"
 
 msgid "Change %s"
 msgstr "Zmień %s"
 
 msgid "Change document"
@@ -52,17 +49,14 @@
 
 msgid "Download PO file"
 msgstr "Pobierz plik PO"
 
 msgid "Download PO file and input translations offline"
 msgstr "Pobierz plik PO i wprowadź tłumaczenia offline"
 
-msgid "Draft"
-msgstr "Szkic"
-
 msgid "Edit"
 msgstr "Edytuj"
 
 msgid "Edit this %s"
 msgstr "Edytuj ten %s"
 
 msgid "Edit this document"
@@ -82,35 +76,26 @@
 
 msgid "Fetching image information..."
 msgstr "Pobieranie informacji na temat obrazu"
 
 msgid "Fetching page information..."
 msgstr "Pobieranie informacji na temat strony..."
 
-msgid "Live"
-msgstr "Opublikowana"
-
 msgid "Lock"
 msgstr "Zablokuj"
 
 msgid "Not translated"
 msgstr "Nie przetłumaczone"
 
 msgid "Preview"
 msgstr "Podgląd"
 
 msgid "Publish in "
 msgstr "Opublikuj w"
 
-msgid "Published"
-msgstr "Opublikowano"
-
-msgid "Published on "
-msgstr "Opublikowano dnia"
-
 msgid "Publishing..."
 msgstr "Publikowanie..."
 
 msgid "Remove editor lock"
 msgstr "Usuń blokadę edytorską"
 
 msgid "Revert to %s version"
```

### Comparing `wagtail-localize-1.5/wagtail_localize/locale/pl/LC_MESSAGES/djangojs.po` & `wagtail-localize-1.5.1/wagtail_localize/locale/pl/LC_MESSAGES/djangojs.po`

 * *Files 4% similar despite different names*

```diff
@@ -2,30 +2,27 @@
 # Translators:
 # Łukasz Bołdys (Lukasz Boldys), 2021
 # Miłosz Miśkiewicz, 2023
 #
 msgid ""
 msgstr ""
 "Last-Translator: Miłosz Miśkiewicz, 2023\n"
-"Language-Team: Polish (https://www.transifex.com/torchbox/teams/8009/pl/)\n"
+"Language-Team: Polish (https://app.transifex.com/torchbox/teams/8009/pl/)\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Language: pl\n"
 "Plural-Forms: nplurals=4; plural=(n==1 ? 0 : (n%10>=2 && n%10<=4) && "
 "(n%100<12 || n%100>14) ? 1 : n!=1 && (n%10>=0 && n%10<=1) || (n%10>=5 && "
 "n%10<=9) || (n%100>=12 && n%100<=14) ? 2 : 3);\n"
 
 msgid "[DELETED]"
 msgstr "[USUNIĘTE]"
 
 msgid "Apply editor lock"
 msgstr "Zastosuj blokadę edytorską"
 
-msgid "Breadcrumb"
-msgstr "Breadcrumb"
-
 msgid "Cancel"
 msgstr "Anuluj"
 
 msgid "Change %s"
 msgstr "Zmień %s"
 
 msgid "Change document"
@@ -60,17 +57,14 @@
 
 msgid "Download PO file"
 msgstr "Pobierz plik PO"
 
 msgid "Download PO file and input translations offline"
 msgstr "Pobierz plik PO i wprowadź tłumaczenia offline"
 
-msgid "Draft"
-msgstr "Szkic"
-
 msgid "Edit"
 msgstr "Edytuj"
 
 msgid "Edit this %s"
 msgstr "Edytuj ten %s"
 
 msgid "Edit this document"
@@ -90,35 +84,26 @@
 
 msgid "Fetching image information..."
 msgstr "Pobieranie informacji na temat obrazu"
 
 msgid "Fetching page information..."
 msgstr "Pobieranie informacji na temat strony..."
 
-msgid "Live"
-msgstr "Opublikowana"
-
 msgid "Lock"
 msgstr "Zablokuj"
 
 msgid "Not translated"
 msgstr "Nie przetłumaczone"
 
 msgid "Preview"
 msgstr "Podgląd"
 
 msgid "Publish in "
 msgstr "Opublikuj w"
 
-msgid "Published"
-msgstr "Opublikowano"
-
-msgid "Published on "
-msgstr "Opublikowano dnia"
-
 msgid "Publishing..."
 msgstr "Publikowanie..."
 
 msgid "Remove editor lock"
 msgstr "Usuń blokadę edytorską"
 
 msgid "Revert to %s version"
```

### Comparing `wagtail-localize-1.5/wagtail_localize/locale/pt_BR/LC_MESSAGES/django.mo` & `wagtail-localize-1.5.1/wagtail_localize/locale/pt_BR/LC_MESSAGES/django.mo`

 * *Files 12% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,13 +1,12 @@
 msgid ""
 msgstr ""
 "Report-Msgid-Bugs-To: \n"
-"Last-Translator: Rodrigo de Almeida Sottomaior Macedo "
-"<rmsolucoeseminformatica@protonmail.com>, 2022\n"
-"Language-Team: Portuguese (Brazil) (https://www.transifex.com/torchbox/"
+"Last-Translator: Fabio Santos <f4bio.sa@gmail.com>, 2023\n"
+"Language-Team: Portuguese (Brazil) (https://app.transifex.com/torchbox/"
 "teams/8009/pt_BR/)\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Language: pt_BR\n"
 "Plural-Forms: nplurals=3; plural=(n == 0 || n == 1) ? 0 : n != 0 && n % "
 "1000000 == 0 ? 1 : 2;\n"
 
 msgid ""
@@ -16,14 +15,23 @@
 msgstr ""
 "Tag <{}> não é permitida. O texto pode conter apenas HTML com tags "
 "\"inline\" (tais como <b>,<a>) "
 
 msgid "All child pages will be created."
 msgstr "Todas páginas filho serão criadas"
 
+msgid ""
+"Are you sure you want to convert this page into an alias? This will "
+"overwrite the content of the page with the content of "
+"'%(source_page_title)s' (%(source_page_locale)s)"
+msgstr ""
+"Tem certeza de que deseja converter esta página em um alias? Isso "
+"substituirá o conteúdo da página pelo conteúdo de "
+"'%(source_page_title)s' (%(source_page_locale)s)"
+
 msgid "Cannot import PO file that was created for a different translation."
 msgstr ""
 "Não é possível importar o arquivo PO criado para uma tradução diferente."
 
 msgid ""
 "Changes are not automatically applied between translated pages. Syncing will "
 "add new content for translation and remove deleted content."
@@ -41,14 +49,23 @@
 
 msgid "Content"
 msgstr "Conteúdo"
 
 msgid "Content type"
 msgstr "Tipo de conteúdo"
 
+msgid "Convert page to alias"
+msgstr "Converter página em alias"
+
+msgid "Convert to alias"
+msgstr "Converter em alias"
+
+msgid "Convert to alias %(title)s"
+msgstr "Converter alias para %(title)s"
+
 msgid "Convert to alias page"
 msgstr "Converter em página de atalho"
 
 msgid "Delete"
 msgstr "Excluir"
 
 msgid "Disable"
@@ -94,14 +111,20 @@
 "Novos erros de validação foram encontrados ao publicar o '{object}' em "
 "{locale}. Por favor revise os erros ou clique em publicar outra vez para "
 "ignorar essas traduções por agora."
 
 msgid "No translations found."
 msgstr "Nenhuma tradução foi encontrada."
 
+msgid "No, leave it as a page"
+msgstr "Não, deixe como uma página"
+
+msgid "Page '{}' has been converted into an alias."
+msgstr "A página '{}' foi convertida em um alias."
+
 msgid "Please upload a valid PO file."
 msgstr "Por favor faça o upload de um arquivo PO válido."
 
 msgid "Publish immediately"
 msgstr "Publicar imediatamente"
 
 msgid "Published '{object}' in {locale} with missing translations - see below."
```

### Comparing `wagtail-localize-1.5/wagtail_localize/locale/pt_BR/LC_MESSAGES/django.po` & `wagtail-localize-1.5.1/wagtail_localize/locale/pt_BR/LC_MESSAGES/django.po`

 * *Files 8% similar despite different names*

```diff
@@ -2,22 +2,22 @@
 # Translators:
 # Ed Wurch <ewurch@gmail.com>, 2021
 # Claudemiro Alves Feitosa Neto <dimiro1@gmail.com>, 2021
 # Éder Brito <britoederr@gmail.com>, 2021
 # Iuri L. Machado, 2021
 # Luiz Boaretto <lboaretto@gmail.com>, 2022
 # Rodrigo de Almeida Sottomaior Macedo <rmsolucoeseminformatica@protonmail.com>, 2022
+# Fabio Santos <f4bio.sa@gmail.com>, 2023
 #
 msgid ""
 msgstr ""
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2022-10-17 21:00+0000\n"
-"Last-Translator: Rodrigo de Almeida Sottomaior Macedo "
-"<rmsolucoeseminformatica@protonmail.com>, 2022\n"
-"Language-Team: Portuguese (Brazil) (https://www.transifex.com/torchbox/"
+"POT-Creation-Date: 2023-02-23 14:15+0000\n"
+"Last-Translator: Fabio Santos <f4bio.sa@gmail.com>, 2023\n"
+"Language-Team: Portuguese (Brazil) (https://app.transifex.com/torchbox/"
 "teams/8009/pt_BR/)\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Language: pt_BR\n"
 "Plural-Forms: nplurals=3; plural=(n == 0 || n == 1) ? 0 : n != 0 && n % "
 "1000000 == 0 ? 1 : 2;\n"
 
 msgid "Disable"
@@ -112,17 +112,37 @@
 
 msgid "Unrecognised id found in an <a> tag: {}"
 msgstr "Id não reconhecido encontrado na tag <a>: {}"
 
 msgid "Enable"
 msgstr "Habilitar"
 
+#, python-format
+msgid "Convert to alias %(title)s"
+msgstr "Converter alias para %(title)s"
+
+msgid "Convert to alias"
+msgstr "Converter em alias"
+
+#, python-format
+msgid ""
+"Are you sure you want to convert this page into an alias? This will "
+"overwrite the content of the page with the content of "
+"'%(source_page_title)s' (%(source_page_locale)s)"
+msgstr ""
+"Tem certeza de que deseja converter esta página em um alias? Isso "
+"substituirá o conteúdo da página pelo conteúdo de "
+"'%(source_page_title)s' (%(source_page_locale)s)"
+
 msgid "Yes, convert it"
 msgstr "Sim, converta"
 
+msgid "No, leave it as a page"
+msgstr "Não, deixe como uma página"
+
 #, python-format
 msgid ""
 "This page hasn't been translated yet. It is mirroring the <a "
 "href=\"%(edit_original_page_url)s\" target=\"_blank\">%(original_locale)s "
 "page</a>."
 msgstr ""
 "Esta página ainda não foi traduzida. Ela é um espelhamento da <a "
@@ -171,14 +191,17 @@
 msgid ""
 "The last sync date was %(last_sync_date)s. You are about to sync the "
 "following:"
 msgstr ""
 "A última sincronização foi a %(last_sync_date)s. Você irá sincronizar o "
 "seguinte:"
 
+msgid "Page '{}' has been converted into an alias."
+msgstr "A página '{}' foi convertida em um alias."
+
 msgid "Content"
 msgstr "Conteúdo"
 
 #, python-brace-format
 msgid ""
 "New validation errors were found when publishing '{object}' in {locale}. "
 "Please fix them or click publish again to ignore these translations for now."
@@ -291,7 +314,10 @@
 
 #, python-format
 msgid "Sync translations of '%(title)s'"
 msgstr "Sincronizar traduções de '%(title)s'"
 
 msgid "Convert to alias page"
 msgstr "Converter em página de atalho"
+
+msgid "Convert page to alias"
+msgstr "Converter página em alias"
```

### Comparing `wagtail-localize-1.5/wagtail_localize/locale/pt_BR/LC_MESSAGES/djangojs.mo` & `wagtail-localize-1.5.1/wagtail_localize/locale/sl/LC_MESSAGES/djangojs.mo`

 * *Files 25% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,163 +1,148 @@
 msgid ""
 msgstr ""
-"Last-Translator: Rodrigo de Almeida Sottomaior Macedo "
-"<rmsolucoeseminformatica@protonmail.com>, 2022\n"
-"Language-Team: Portuguese (Brazil) (https://www.transifex.com/torchbox/"
-"teams/8009/pt_BR/)\n"
+"Last-Translator: Andrej Marsetič, 2023\n"
+"Language-Team: Slovenian (https://app.transifex.com/torchbox/teams/8009/"
+"sl/)\n"
 "Content-Type: text/plain; charset=UTF-8\n"
-"Language: pt_BR\n"
-"Plural-Forms: nplurals=3; plural=(n == 0 || n == 1) ? 0 : n != 0 && n % "
-"1000000 == 0 ? 1 : 2;\n"
+"Language: sl\n"
+"Plural-Forms: nplurals=4; plural=(n%100==1 ? 0 : n%100==2 ? 1 : n%100==3 || "
+"n%100==4 ? 2 : 3);\n"
 
 msgid "Apply editor lock"
-msgstr "Aplicar bloqueio do editor"
-
-msgid "Breadcrumb"
-msgstr "Breadcrumb"
+msgstr "Uporabi zaklepanje urejevalnika"
 
 msgid "Cancel"
-msgstr "Cancelar"
+msgstr "Prekliči"
 
 msgid "Change %s"
-msgstr "Alterar %s"
+msgstr "Spremeni %s"
 
 msgid "Change document"
-msgstr "Alterar documento"
+msgstr "Spremeni dokument"
 
 msgid "Change image"
-msgstr "Alterar imagem"
+msgstr "Spremeni sliko"
 
 msgid "Change page"
-msgstr "Alterar página"
+msgstr "Spremeni stran"
 
 msgid "Changed"
-msgstr "Alterado"
+msgstr "Spremenjeno"
 
 msgid "Choose a %s"
-msgstr "Escolha um %s"
+msgstr "Izberite %s"
 
 msgid "Choose a document"
-msgstr "Escolha um documento"
+msgstr "Izberite dokument"
 
 msgid "Choose a page"
-msgstr "Escolha uma página"
+msgstr "Izberite stran"
 
 msgid "Choose an image"
-msgstr "Escolha uma imagem"
+msgstr "Izberi sliko"
 
 msgid "Convert to alias page"
-msgstr "Converter em página de atalho"
+msgstr "Pretvori v vzdevek strani"
 
 msgid "Delete"
-msgstr "Excluir"
+msgstr "Izbriši"
 
 msgid "Download PO file"
-msgstr "Baixar arquivo PO"
+msgstr "Prenesi PO datoteko"
 
 msgid "Download PO file and input translations offline"
-msgstr "Baixe o arquivo PO e insira traduções offline"
-
-msgid "Draft"
-msgstr "Rascunho"
+msgstr "Prenesite datoteko PO in vnesite prevode brez povezave"
 
 msgid "Edit"
-msgstr "Editar"
+msgstr "Uredi"
 
 msgid "Edit this %s"
-msgstr "Editar este %s"
+msgstr "Uredi %s"
 
 msgid "Edit this document"
-msgstr "Editar este documento"
+msgstr "Uredi dokument"
 
 msgid "Edit this image"
-msgstr "Editar esta imagem"
+msgstr "Uredi sliko"
 
 msgid "Edit this page"
-msgstr "Editar esta página"
+msgstr "Uredi stran"
 
 msgid "Fetching %s information..."
-msgstr "Buscando %s informação..."
+msgstr "Pridobivanje podatkov %s ..."
 
 msgid "Fetching document information..."
-msgstr "Buscando informações do documento..."
+msgstr "Pridobivanje informacij o dokumentu ..."
 
 msgid "Fetching image information..."
-msgstr "Buscando informações da imagem..."
+msgstr "Pridobivanje informacij o sliki ..."
 
 msgid "Fetching page information..."
-msgstr "Buscando informações da página..."
-
-msgid "Live"
-msgstr "Online"
+msgstr "Pridobivanje informacij o strani ..."
 
 msgid "Lock"
-msgstr "Travar"
+msgstr "Zakleni"
 
 msgid "Not translated"
-msgstr "Não traduzido"
+msgstr "Ni prevedeno"
 
 msgid "Preview"
-msgstr "Pré-visualizar"
+msgstr "Predogled"
 
 msgid "Publish in "
-msgstr "Publicar em"
-
-msgid "Published"
-msgstr "Publicado"
-
-msgid "Published on "
-msgstr "Publicado em"
+msgstr "Objavi v "
 
 msgid "Publishing..."
-msgstr "Publicando..."
+msgstr "Objava..."
 
 msgid "Remove editor lock"
-msgstr "Remover bloqueio do editor"
+msgstr "Odstranite zaklep urejevalnika"
 
 msgid "Revert to %s version"
-msgstr "Reverter para %s versão"
+msgstr "Povrni na različico %s"
 
 msgid "Save"
-msgstr "Salvar"
+msgstr "Shrani"
 
 msgid "Saving..."
-msgstr "Salvando..."
+msgstr "Shranjevanje..."
 
 msgid "Server error"
-msgstr "Erro de servidor"
+msgstr "Napaka strežnika"
 
 msgid "Stop Synced translation"
-msgstr "Parar tradução sincronizada"
+msgstr "Ustavi sinhroniziran prevod"
 
 msgid "There are unsaved segments. Please save or cancel them before leaving."
-msgstr "Existem segmentos não salvos. Salve ou cancele-os antes de sair."
+msgstr ""
+"Obstajajo neshranjeni segmenti. Pred odhodom jih shranite ali prekličite."
 
 msgid "Translate"
-msgstr "Traduzir"
+msgstr "Prevedi"
 
 msgid "Translate all missing strings with "
-msgstr "Traduzir todas as frases ausentes com"
+msgstr "prevedite vse manjkajoče nize z"
 
 msgid "Translate with "
-msgstr "Traduzir com"
+msgstr "Prevedi z"
 
 msgid "Unlock"
-msgstr "Desbloquear"
+msgstr "Odkleni"
 
 msgid "Unpublish"
-msgstr "Despublicar"
+msgstr "Umakni iz objave"
 
 msgid "Upload PO file"
-msgstr "Carregar arquivo PO"
+msgstr "Naložite PO datoteko"
 
 msgid "Upload translated PO file to submit translations"
-msgstr "Faça upload do arquivo PO traduzido para enviar traduções"
+msgstr "Naložite prevedeno datoteko PO, da objavite prevode"
 
 msgid "Uses %s version"
-msgstr "Use a versão %s "
+msgstr "Uporabi %s različico"
 
 msgid "[DELETED]"
-msgstr "[REMOVIDO]"
+msgstr "[IZBRISANO]"
 
 msgid "segments translated"
-msgstr "segmentos traduzidos"
+msgstr "segmenti prevedeni"
```

### Comparing `wagtail-localize-1.5/wagtail_localize/locale/pt_BR/LC_MESSAGES/djangojs.po` & `wagtail-localize-1.5.1/wagtail_localize/locale/pt_BR/LC_MESSAGES/djangojs.po`

 * *Files 12% similar despite different names*

```diff
@@ -4,30 +4,27 @@
 # Iuri L. Machado, 2021
 # Rodrigo de Almeida Sottomaior Macedo <rmsolucoeseminformatica@protonmail.com>, 2022
 #
 msgid ""
 msgstr ""
 "Last-Translator: Rodrigo de Almeida Sottomaior Macedo "
 "<rmsolucoeseminformatica@protonmail.com>, 2022\n"
-"Language-Team: Portuguese (Brazil) (https://www.transifex.com/torchbox/"
+"Language-Team: Portuguese (Brazil) (https://app.transifex.com/torchbox/"
 "teams/8009/pt_BR/)\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Language: pt_BR\n"
 "Plural-Forms: nplurals=3; plural=(n == 0 || n == 1) ? 0 : n != 0 && n % "
 "1000000 == 0 ? 1 : 2;\n"
 
 msgid "[DELETED]"
 msgstr "[REMOVIDO]"
 
 msgid "Apply editor lock"
 msgstr "Aplicar bloqueio do editor"
 
-msgid "Breadcrumb"
-msgstr "Breadcrumb"
-
 msgid "Cancel"
 msgstr "Cancelar"
 
 msgid "Change %s"
 msgstr "Alterar %s"
 
 msgid "Change document"
@@ -62,17 +59,14 @@
 
 msgid "Download PO file"
 msgstr "Baixar arquivo PO"
 
 msgid "Download PO file and input translations offline"
 msgstr "Baixe o arquivo PO e insira traduções offline"
 
-msgid "Draft"
-msgstr "Rascunho"
-
 msgid "Edit"
 msgstr "Editar"
 
 msgid "Edit this %s"
 msgstr "Editar este %s"
 
 msgid "Edit this document"
@@ -92,35 +86,26 @@
 
 msgid "Fetching image information..."
 msgstr "Buscando informações da imagem..."
 
 msgid "Fetching page information..."
 msgstr "Buscando informações da página..."
 
-msgid "Live"
-msgstr "Online"
-
 msgid "Lock"
 msgstr "Travar"
 
 msgid "Not translated"
 msgstr "Não traduzido"
 
 msgid "Preview"
 msgstr "Pré-visualizar"
 
 msgid "Publish in "
 msgstr "Publicar em"
 
-msgid "Published"
-msgstr "Publicado"
-
-msgid "Published on "
-msgstr "Publicado em"
-
 msgid "Publishing..."
 msgstr "Publicando..."
 
 msgid "Remove editor lock"
 msgstr "Remover bloqueio do editor"
 
 msgid "Revert to %s version"
```

### Comparing `wagtail-localize-1.5/wagtail_localize/locale/pt_PT/LC_MESSAGES/django.mo` & `wagtail-localize-1.5.1/wagtail_localize/locale/pt_PT/LC_MESSAGES/django.mo`

 * *Files 0% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,12 +1,12 @@
 msgid ""
 msgstr ""
 "Report-Msgid-Bugs-To: \n"
 "Last-Translator: Tiago Henriques <trinosauro@gmail.com>, 2022\n"
-"Language-Team: Portuguese (Portugal) (https://www.transifex.com/torchbox/"
+"Language-Team: Portuguese (Portugal) (https://app.transifex.com/torchbox/"
 "teams/8009/pt_PT/)\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Language: pt_PT\n"
 "Plural-Forms: nplurals=3; plural=(n == 0 || n == 1) ? 0 : n != 0 && n % "
 "1000000 == 0 ? 1 : 2;\n"
 
 msgid ""
```

### Comparing `wagtail-localize-1.5/wagtail_localize/locale/pt_PT/LC_MESSAGES/django.po` & `wagtail-localize-1.5.1/wagtail_localize/locale/pt_PT/LC_MESSAGES/django.po`

 * *Files 1% similar despite different names*

```diff
@@ -4,17 +4,17 @@
 # Diogo Silva <diogo_silva30@hotmail.com>, 2021
 # Luís Tiago Favas <traducoes@favas.eu>, 2022
 # Tiago Henriques <trinosauro@gmail.com>, 2022
 #
 msgid ""
 msgstr ""
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2022-10-17 21:00+0000\n"
+"POT-Creation-Date: 2023-02-23 14:15+0000\n"
 "Last-Translator: Tiago Henriques <trinosauro@gmail.com>, 2022\n"
-"Language-Team: Portuguese (Portugal) (https://www.transifex.com/torchbox/"
+"Language-Team: Portuguese (Portugal) (https://app.transifex.com/torchbox/"
 "teams/8009/pt_PT/)\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Language: pt_PT\n"
 "Plural-Forms: nplurals=3; plural=(n == 0 || n == 1) ? 0 : n != 0 && n % "
 "1000000 == 0 ? 1 : 2;\n"
 
 msgid "Disable"
```

### Comparing `wagtail-localize-1.5/wagtail_localize/locale/pt_PT/LC_MESSAGES/djangojs.mo` & `wagtail-localize-1.5.1/wagtail_localize/locale/zh_Hans/LC_MESSAGES/djangojs.mo`

 * *Files 26% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,162 +1,146 @@
 msgid ""
 msgstr ""
-"Last-Translator: Tiago Henriques <trinosauro@gmail.com>, 2022\n"
-"Language-Team: Portuguese (Portugal) (https://www.transifex.com/torchbox/"
-"teams/8009/pt_PT/)\n"
+"Last-Translator: Ford Guo <agile.guo@gmail.com>, 2023\n"
+"Language-Team: Chinese (China) (https://app.transifex.com/torchbox/"
+"teams/8009/zh_CN/)\n"
 "Content-Type: text/plain; charset=UTF-8\n"
-"Language: pt_PT\n"
-"Plural-Forms: nplurals=3; plural=(n == 0 || n == 1) ? 0 : n != 0 && n % "
-"1000000 == 0 ? 1 : 2;\n"
+"Language: zh_CN\n"
+"Plural-Forms: nplurals=1; plural=0;\n"
 
 msgid "Apply editor lock"
-msgstr "Aplicar bloqueio de editor"
-
-msgid "Breadcrumb"
-msgstr "Percurso"
+msgstr "应用锁编辑"
 
 msgid "Cancel"
-msgstr "Cancelar"
+msgstr "取消"
 
 msgid "Change %s"
-msgstr "Mudar %s"
+msgstr "更改 %s"
 
 msgid "Change document"
-msgstr "Mudar documento"
+msgstr "修改文档"
 
 msgid "Change image"
-msgstr "Mudar imagem"
+msgstr "修改图片"
 
 msgid "Change page"
-msgstr "Mudar página"
+msgstr "修改页面"
 
 msgid "Changed"
-msgstr "Mudado"
+msgstr "修改"
 
 msgid "Choose a %s"
-msgstr "Escolher um %s"
+msgstr "选择一个 %s"
 
 msgid "Choose a document"
-msgstr "Escolher um documento"
+msgstr "选择一个文档"
 
 msgid "Choose a page"
-msgstr "Escolher uma página"
+msgstr "选择一个页面"
 
 msgid "Choose an image"
-msgstr "Escolher uma imagem"
+msgstr "选择一个图片"
 
 msgid "Convert to alias page"
-msgstr "Converter em página de atalho"
+msgstr "转换成页面别名"
 
 msgid "Delete"
-msgstr "Apagar"
+msgstr "删除"
 
 msgid "Download PO file"
-msgstr "Descarregar ficheiro PO"
+msgstr "下载 PO 文件"
 
 msgid "Download PO file and input translations offline"
-msgstr "Descarregar ficheiro PO e introduzir traduções em offline"
-
-msgid "Draft"
-msgstr "Rascunho"
+msgstr "下载 PO 文件并且线下翻译"
 
 msgid "Edit"
-msgstr "Alterar"
+msgstr "编辑"
 
 msgid "Edit this %s"
-msgstr "Alterar este %s"
+msgstr "编辑这个 %s"
 
 msgid "Edit this document"
-msgstr "Alterar este documento"
+msgstr "编辑此文档"
 
 msgid "Edit this image"
-msgstr "Alterar esta imagem"
+msgstr "编辑此图片"
 
 msgid "Edit this page"
-msgstr "Alterar esta página"
+msgstr "编辑此页面"
 
 msgid "Fetching %s information..."
-msgstr "A obter informação %s..."
+msgstr "正在获取 %s 信息..."
 
 msgid "Fetching document information..."
-msgstr "A obter informação do documento..."
+msgstr "正在获取文档信息..."
 
 msgid "Fetching image information..."
-msgstr "A obter informação da imagem..."
+msgstr "正在获取图片信息..."
 
 msgid "Fetching page information..."
-msgstr "A obter informação da página..."
-
-msgid "Live"
-msgstr "Publicado"
+msgstr "正在获取页面信息..."
 
 msgid "Lock"
-msgstr "Bloquear"
+msgstr "锁定"
 
 msgid "Not translated"
-msgstr "Por traduzir"
+msgstr "未翻译"
 
 msgid "Preview"
-msgstr "Visualizar"
+msgstr "预览"
 
 msgid "Publish in "
-msgstr "Publicar em"
-
-msgid "Published"
-msgstr "Publicado"
-
-msgid "Published on "
-msgstr "Publicado em"
+msgstr "发布在"
 
 msgid "Publishing..."
-msgstr "A publicar..."
+msgstr "正在发布……"
 
 msgid "Remove editor lock"
-msgstr "Retirar bloqueio de editor"
+msgstr "移除编辑锁定"
 
 msgid "Revert to %s version"
-msgstr "Reverter à versão %s "
+msgstr "回滚至 %s 版本"
 
 msgid "Save"
-msgstr "Gravar"
+msgstr "保存"
 
 msgid "Saving..."
-msgstr "A gravar..."
+msgstr "正在保存……"
 
 msgid "Server error"
-msgstr "Erro de servidor"
+msgstr "服务器错误"
 
 msgid "Stop Synced translation"
-msgstr "Parar tradução Sincronizada"
+msgstr "停止同步翻译"
 
 msgid "There are unsaved segments. Please save or cancel them before leaving."
-msgstr "Existem segmentos por gravar. Grave ou cancele-os antes de sair."
+msgstr "存在未保存的部分。请保存或取消修改后再离开。"
 
 msgid "Translate"
-msgstr "Traduzir"
+msgstr "翻译"
 
 msgid "Translate all missing strings with "
-msgstr "Traduzir todos os segmentos de texto em falta com"
+msgstr "翻译所有缺失的字符串"
 
 msgid "Translate with "
-msgstr "Traduzir com"
+msgstr "翻译"
 
 msgid "Unlock"
-msgstr "Desbloquear"
+msgstr "解锁"
 
 msgid "Unpublish"
-msgstr "Despublicar"
+msgstr "取消发布"
 
 msgid "Upload PO file"
-msgstr "Carregar ficheiro PO"
+msgstr "上传 PO 文件"
 
 msgid "Upload translated PO file to submit translations"
-msgstr "Carregar ficheiro PO traduzido para enviar traduções"
+msgstr "上传翻译好的 PO 文件来提交翻译"
 
 msgid "Uses %s version"
-msgstr "Utiliza a versão %s"
+msgstr "使用%s版本"
 
 msgid "[DELETED]"
-msgstr "[APAGADO]"
+msgstr "[已删除]"
 
 msgid "segments translated"
-msgstr "segmentos traduzidos"
+msgstr "片段已翻译"
```

### Comparing `wagtail-localize-1.5/wagtail_localize/locale/pt_PT/LC_MESSAGES/djangojs.po` & `wagtail-localize-1.5.1/wagtail_localize/locale/sl/LC_MESSAGES/djangojs.po`

 * *Files 20% similar despite different names*

```diff
@@ -1,167 +1,154 @@
 #
 # Translators:
-# Luís Tiago Favas <traducoes@favas.eu>, 2020
-# Tiago Henriques <trinosauro@gmail.com>, 2022
+# Mitja Pagon <mitja.pagon@inueni.com>, 2021
+# UP, 2021
+# Andrej Marsetič, 2023
 #
 msgid ""
 msgstr ""
-"Last-Translator: Tiago Henriques <trinosauro@gmail.com>, 2022\n"
-"Language-Team: Portuguese (Portugal) (https://www.transifex.com/torchbox/"
-"teams/8009/pt_PT/)\n"
+"Last-Translator: Andrej Marsetič, 2023\n"
+"Language-Team: Slovenian (https://app.transifex.com/torchbox/teams/8009/"
+"sl/)\n"
 "Content-Type: text/plain; charset=UTF-8\n"
-"Language: pt_PT\n"
-"Plural-Forms: nplurals=3; plural=(n == 0 || n == 1) ? 0 : n != 0 && n % "
-"1000000 == 0 ? 1 : 2;\n"
+"Language: sl\n"
+"Plural-Forms: nplurals=4; plural=(n%100==1 ? 0 : n%100==2 ? 1 : n%100==3 || "
+"n%100==4 ? 2 : 3);\n"
 
 msgid "[DELETED]"
-msgstr "[APAGADO]"
+msgstr "[IZBRISANO]"
 
 msgid "Apply editor lock"
-msgstr "Aplicar bloqueio de editor"
-
-msgid "Breadcrumb"
-msgstr "Percurso"
+msgstr "Uporabi zaklepanje urejevalnika"
 
 msgid "Cancel"
-msgstr "Cancelar"
+msgstr "Prekliči"
 
 msgid "Change %s"
-msgstr "Mudar %s"
+msgstr "Spremeni %s"
 
 msgid "Change document"
-msgstr "Mudar documento"
+msgstr "Spremeni dokument"
 
 msgid "Change image"
-msgstr "Mudar imagem"
+msgstr "Spremeni sliko"
 
 msgid "Change page"
-msgstr "Mudar página"
+msgstr "Spremeni stran"
 
 msgid "Changed"
-msgstr "Mudado"
+msgstr "Spremenjeno"
 
 msgid "Choose a %s"
-msgstr "Escolher um %s"
+msgstr "Izberite %s"
 
 msgid "Choose a document"
-msgstr "Escolher um documento"
+msgstr "Izberite dokument"
 
 msgid "Choose a page"
-msgstr "Escolher uma página"
+msgstr "Izberite stran"
 
 msgid "Choose an image"
-msgstr "Escolher uma imagem"
+msgstr "Izberi sliko"
 
 msgid "Convert to alias page"
-msgstr "Converter em página de atalho"
+msgstr "Pretvori v vzdevek strani"
 
 msgid "Delete"
-msgstr "Apagar"
+msgstr "Izbriši"
 
 msgid "Download PO file"
-msgstr "Descarregar ficheiro PO"
+msgstr "Prenesi PO datoteko"
 
 msgid "Download PO file and input translations offline"
-msgstr "Descarregar ficheiro PO e introduzir traduções em offline"
-
-msgid "Draft"
-msgstr "Rascunho"
+msgstr "Prenesite datoteko PO in vnesite prevode brez povezave"
 
 msgid "Edit"
-msgstr "Alterar"
+msgstr "Uredi"
 
 msgid "Edit this %s"
-msgstr "Alterar este %s"
+msgstr "Uredi %s"
 
 msgid "Edit this document"
-msgstr "Alterar este documento"
+msgstr "Uredi dokument"
 
 msgid "Edit this image"
-msgstr "Alterar esta imagem"
+msgstr "Uredi sliko"
 
 msgid "Edit this page"
-msgstr "Alterar esta página"
+msgstr "Uredi stran"
 
 msgid "Fetching %s information..."
-msgstr "A obter informação %s..."
+msgstr "Pridobivanje podatkov %s ..."
 
 msgid "Fetching document information..."
-msgstr "A obter informação do documento..."
+msgstr "Pridobivanje informacij o dokumentu ..."
 
 msgid "Fetching image information..."
-msgstr "A obter informação da imagem..."
+msgstr "Pridobivanje informacij o sliki ..."
 
 msgid "Fetching page information..."
-msgstr "A obter informação da página..."
-
-msgid "Live"
-msgstr "Publicado"
+msgstr "Pridobivanje informacij o strani ..."
 
 msgid "Lock"
-msgstr "Bloquear"
+msgstr "Zakleni"
 
 msgid "Not translated"
-msgstr "Por traduzir"
+msgstr "Ni prevedeno"
 
 msgid "Preview"
-msgstr "Visualizar"
+msgstr "Predogled"
 
 msgid "Publish in "
-msgstr "Publicar em"
-
-msgid "Published"
-msgstr "Publicado"
-
-msgid "Published on "
-msgstr "Publicado em"
+msgstr "Objavi v "
 
 msgid "Publishing..."
-msgstr "A publicar..."
+msgstr "Objava..."
 
 msgid "Remove editor lock"
-msgstr "Retirar bloqueio de editor"
+msgstr "Odstranite zaklep urejevalnika"
 
 msgid "Revert to %s version"
-msgstr "Reverter à versão %s "
+msgstr "Povrni na različico %s"
 
 msgid "Save"
-msgstr "Gravar"
+msgstr "Shrani"
 
 msgid "Saving..."
-msgstr "A gravar..."
+msgstr "Shranjevanje..."
 
 msgid "segments translated"
-msgstr "segmentos traduzidos"
+msgstr "segmenti prevedeni"
 
 msgid "Server error"
-msgstr "Erro de servidor"
+msgstr "Napaka strežnika"
 
 msgid "Stop Synced translation"
-msgstr "Parar tradução Sincronizada"
+msgstr "Ustavi sinhroniziran prevod"
 
 msgid "There are unsaved segments. Please save or cancel them before leaving."
-msgstr "Existem segmentos por gravar. Grave ou cancele-os antes de sair."
+msgstr ""
+"Obstajajo neshranjeni segmenti. Pred odhodom jih shranite ali prekličite."
 
 msgid "Translate"
-msgstr "Traduzir"
+msgstr "Prevedi"
 
 msgid "Translate all missing strings with "
-msgstr "Traduzir todos os segmentos de texto em falta com"
+msgstr "prevedite vse manjkajoče nize z"
 
 msgid "Translate with "
-msgstr "Traduzir com"
+msgstr "Prevedi z"
 
 msgid "Unlock"
-msgstr "Desbloquear"
+msgstr "Odkleni"
 
 msgid "Unpublish"
-msgstr "Despublicar"
+msgstr "Umakni iz objave"
 
 msgid "Upload PO file"
-msgstr "Carregar ficheiro PO"
+msgstr "Naložite PO datoteko"
 
 msgid "Upload translated PO file to submit translations"
-msgstr "Carregar ficheiro PO traduzido para enviar traduções"
+msgstr "Naložite prevedeno datoteko PO, da objavite prevode"
 
 msgid "Uses %s version"
-msgstr "Utiliza a versão %s"
+msgstr "Uporabi %s različico"
```

### Comparing `wagtail-localize-1.5/wagtail_localize/locale/ro/LC_MESSAGES/django.mo` & `wagtail-localize-1.5.1/wagtail_localize/locale/ro/LC_MESSAGES/django.mo`

 * *Files 5% similar despite different names*

```diff
@@ -1,538 +1,543 @@
-00000000: de12 0495 0000 0000 4f00 0000 1c00 0000  ........O.......
-00000010: 9402 0000 6b00 0000 0c05 0000 0000 0000  ....k...........
-00000020: b806 0000 5e00 0000 b906 0000 2000 0000  ....^....... ...
-00000030: 1807 0000 aa00 0000 3907 0000 4300 0000  ........9...C...
-00000040: e407 0000 8800 0000 2808 0000 9600 0000  ........(.......
-00000050: b108 0000 0700 0000 4809 0000 0c00 0000  ........H.......
-00000060: 5009 0000 1500 0000 5d09 0000 1000 0000  P.......].......
-00000070: 7309 0000 1a00 0000 8409 0000 1500 0000  s...............
-00000080: 9f09 0000 5800 0000 b509 0000 3900 0000  ....X.......9...
-00000090: 0e0a 0000 0600 0000 480a 0000 0700 0000  ........H.......
-000000a0: 4f0a 0000 0c00 0000 570a 0000 0d00 0000  O.......W.......
-000000b0: 640a 0000 1000 0000 720a 0000 0600 0000  d.......r.......
-000000c0: 830a 0000 0700 0000 8a0a 0000 3400 0000  ............4...
-000000d0: 920a 0000 0700 0000 c70a 0000 0700 0000  ................
-000000e0: cf0a 0000 1c00 0000 d70a 0000 0600 0000  ................
-000000f0: f40a 0000 9500 0000 fb0a 0000 1600 0000  ................
-00000100: 910b 0000 1600 0000 a80b 0000 2b00 0000  ............+...
-00000110: bf0b 0000 1e00 0000 eb0b 0000 1300 0000  ................
-00000120: 0a0c 0000 4700 0000 1e0c 0000 2100 0000  ....G.......!...
-00000130: 660c 0000 0400 0000 880c 0000 0900 0000  f...............
-00000140: 8d0c 0000 0a00 0000 970c 0000 0600 0000  ................
-00000150: a20c 0000 0c00 0000 a90c 0000 1800 0000  ................
-00000160: b60c 0000 0600 0000 cf0c 0000 4f00 0000  ............O...
-00000170: d60c 0000 0600 0000 260d 0000 3000 0000  ........&...0...
-00000180: 2d0d 0000 2000 0000 5e0d 0000 3000 0000  -... ...^...0...
-00000190: 7f0d 0000 1e00 0000 b00d 0000 1500 0000  ................
-000001a0: cf0d 0000 1800 0000 e50d 0000 2000 0000  ............ ...
-000001b0: fe0d 0000 2700 0000 1f0e 0000 0600 0000  ....'...........
-000001c0: 470e 0000 b900 0000 4e0e 0000 4f00 0000  G.......N...O...
-000001d0: 080f 0000 5100 0000 580f 0000 5500 0000  ....Q...X...U...
-000001e0: aa0f 0000 2700 0000 0010 0000 2900 0000  ....'.......)...
-000001f0: 2810 0000 8c00 0000 5210 0000 5800 0000  (.......R...X...
-00000200: df10 0000 0900 0000 3811 0000 1500 0000  ........8.......
-00000210: 4211 0000 0e00 0000 5811 0000 1300 0000  B.......X.......
-00000220: 6711 0000 1600 0000 7b11 0000 1d00 0000  g.......{.......
-00000230: 9211 0000 2500 0000 b011 0000 1f00 0000  ....%...........
-00000240: d611 0000 1d00 0000 f611 0000 2b00 0000  ............+...
-00000250: 1412 0000 0c00 0000 4012 0000 2700 0000  ........@...'...
-00000260: 4d12 0000 0a00 0000 7512 0000 1c00 0000  M.......u.......
-00000270: 8012 0000 1800 0000 9d12 0000 1900 0000  ................
-00000280: b612 0000 0f00 0000 d012 0000 0a00 0000  ................
-00000290: e012 0000 0f01 0000 eb12 0000 7000 0000  ............p...
-000002a0: fb13 0000 2800 0000 6c14 0000 ae00 0000  ....(...l.......
-000002b0: 9514 0000 4400 0000 4415 0000 8a00 0000  ....D...D.......
-000002c0: 8915 0000 a800 0000 1416 0000 0900 0000  ................
-000002d0: bd16 0000 1000 0000 c716 0000 2500 0000  ............%...
-000002e0: d816 0000 1600 0000 fe16 0000 2000 0000  ............ ...
-000002f0: 1517 0000 1e00 0000 3617 0000 5f00 0000  ........6..._...
-00000300: 5517 0000 4000 0000 b517 0000 0700 0000  U...@...........
-00000310: f617 0000 0d00 0000 fe17 0000 0d00 0000  ................
-00000320: 0c18 0000 0e00 0000 1a18 0000 1000 0000  ................
-00000330: 2918 0000 0a00 0000 3a18 0000 0700 0000  ).......:.......
-00000340: 4518 0000 7500 0000 4d18 0000 0b00 0000  E...u...M.......
-00000350: c318 0000 0700 0000 cf18 0000 1800 0000  ................
-00000360: d718 0000 0600 0000 f018 0000 bd00 0000  ................
-00000370: f718 0000 1900 0000 b519 0000 1a00 0000  ................
-00000380: cf19 0000 2900 0000 ea19 0000 1e00 0000  ....)...........
-00000390: 141a 0000 1400 0000 331a 0000 4800 0000  ........3...H...
-000003a0: 481a 0000 2300 0000 911a 0000 0900 0000  H...#...........
-000003b0: b51a 0000 1600 0000 bf1a 0000 1100 0000  ................
-000003c0: d61a 0000 0600 0000 e81a 0000 0c00 0000  ................
-000003d0: ef1a 0000 1f00 0000 fc1a 0000 0600 0000  ................
-000003e0: 1c1b 0000 6500 0000 231b 0000 0700 0000  ....e...#.......
-000003f0: 891b 0000 3700 0000 911b 0000 1a00 0000  ....7...........
-00000400: c91b 0000 3100 0000 e41b 0000 2800 0000  ....1.......(...
-00000410: 161c 0000 1d00 0000 3f1c 0000 2000 0000  ........?... ...
-00000420: 5d1c 0000 2d00 0000 7e1c 0000 2d00 0000  ]...-...~...-...
-00000430: ac1c 0000 0700 0000 da1c 0000 d100 0000  ................
-00000440: e21c 0000 6200 0000 b41d 0000 4400 0000  ....b.......D...
-00000450: 171e 0000 4800 0000 5c1e 0000 1c00 0000  ....H...\.......
-00000460: a51e 0000 3700 0000 c21e 0000 8400 0000  ....7...........
-00000470: fa1e 0000 5800 0000 7f1f 0000 0a00 0000  ....X...........
-00000480: d81f 0000 1300 0000 e31f 0000 0f00 0000  ................
-00000490: f71f 0000 1b00 0000 0720 0000 1400 0000  ......... ......
-000004a0: 2320 0000 1700 0000 3820 0000 2700 0000  # ......8 ..'...
-000004b0: 5020 0000 1f00 0000 7820 0000 1a00 0000  P ......x ......
-000004c0: 9820 0000 2600 0000 b320 0000 0900 0000  . ..&.... ......
-000004d0: da20 0000 2c00 0000 e420 0000 0a00 0000  . ..,.... ......
-000004e0: 1121 0000 2100 0000 1c21 0000 1100 0000  .!..!....!......
-000004f0: 3e21 0000 2000 0000 5021 0000 1000 0000  >!.. ...P!......
-00000500: 7121 0000 0e00 0000 8221 0000 0100 0000  q!.......!......
-00000510: 4d00 0000 2100 0000 0000 0000 0d00 0000  M...!...........
-00000520: 1000 0000 2a00 0000 0000 0000 0000 0000  ....*...........
-00000530: 1c00 0000 4000 0000 3c00 0000 0200 0000  ....@...<.......
-00000540: 2300 0000 1d00 0000 4800 0000 1b00 0000  #.......H.......
-00000550: 3400 0000 2e00 0000 1700 0000 3800 0000  4...........8...
-00000560: 0000 0000 0000 0000 3100 0000 4500 0000  ........1...E...
-00000570: 0000 0000 1e00 0000 0000 0000 2c00 0000  ............,...
-00000580: 0000 0000 0000 0000 1300 0000 2900 0000  ............)...
-00000590: 1a00 0000 3d00 0000 1200 0000 1100 0000  ....=...........
-000005a0: 4300 0000 4a00 0000 0000 0000 0500 0000  C...J...........
-000005b0: 4400 0000 4e00 0000 3900 0000 0000 0000  D...N...9.......
-000005c0: 0000 0000 2500 0000 1900 0000 0000 0000  ....%...........
-000005d0: 2800 0000 0000 0000 4900 0000 1600 0000  (.......I.......
-000005e0: 0000 0000 0300 0000 3e00 0000 1f00 0000  ........>.......
-000005f0: 0000 0000 3b00 0000 0700 0000 0000 0000  ....;...........
-00000600: 3300 0000 4100 0000 3700 0000 0400 0000  3...A...7.......
-00000610: 4700 0000 3500 0000 2700 0000 2b00 0000  G...5...'...+...
-00000620: 0c00 0000 0e00 0000 3a00 0000 1400 0000  ........:.......
-00000630: 3000 0000 0000 0000 0b00 0000 0000 0000  0...............
-00000640: 3200 0000 4c00 0000 1500 0000 0a00 0000  2...L...........
-00000650: 0f00 0000 2600 0000 4b00 0000 2200 0000  ....&...K..."...
-00000660: 0600 0000 0000 0000 0000 0000 4200 0000  ............B...
-00000670: 0000 0000 0000 0000 2d00 0000 0000 0000  ........-.......
-00000680: 2000 0000 0900 0000 1800 0000 0800 0000   ...............
-00000690: 0000 0000 3600 0000 0000 0000 2400 0000  ....6.......$...
-000006a0: 4600 0000 0000 0000 2f00 0000 0000 0000  F......./.......
-000006b0: 3f00 0000 4f00 0000 003c 7b7d 3e20 7461  ?...O....<{}> ta
-000006c0: 6720 6973 206e 6f74 2061 6c6c 6f77 6564  g is not allowed
-000006d0: 2e20 5374 7269 6e67 7320 6361 6e20 6f6e  . Strings can on
-000006e0: 6c79 2063 6f6e 7461 696e 2073 7461 6e64  ly contain stand
-000006f0: 6172 6420 4854 4d4c 2069 6e6c 696e 6520  ard HTML inline 
-00000700: 7461 6773 2028 7375 6368 2061 7320 3c62  tags (such as <b
-00000710: 3e2c 203c 613e 2900 416c 6c20 6368 696c  >, <a>).All chil
-00000720: 6420 7061 6765 7320 7769 6c6c 2062 6520  d pages will be 
-00000730: 6372 6561 7465 642e 0041 7265 2079 6f75  created..Are you
-00000740: 2073 7572 6520 796f 7520 7761 6e74 2074   sure you want t
-00000750: 6f20 636f 6e76 6572 7420 7468 6973 2070  o convert this p
-00000760: 6167 6520 696e 746f 2061 6e20 616c 6961  age into an alia
-00000770: 733f 2054 6869 7320 7769 6c6c 206f 7665  s? This will ove
-00000780: 7277 7269 7465 2074 6865 2063 6f6e 7465  rwrite the conte
-00000790: 6e74 206f 6620 7468 6520 7061 6765 2077  nt of the page w
-000007a0: 6974 6820 7468 6520 636f 6e74 656e 7420  ith the content 
-000007b0: 6f66 2027 2528 736f 7572 6365 5f70 6167  of '%(source_pag
-000007c0: 655f 7469 746c 6529 7327 2028 2528 736f  e_title)s' (%(so
-000007d0: 7572 6365 5f70 6167 655f 6c6f 6361 6c65  urce_page_locale
-000007e0: 2973 2900 4361 6e6e 6f74 2069 6d70 6f72  )s).Cannot impor
-000007f0: 7420 504f 2066 696c 6520 7468 6174 2077  t PO file that w
-00000800: 6173 2063 7265 6174 6564 2066 6f72 2061  as created for a
-00000810: 2064 6966 6665 7265 6e74 2074 7261 6e73   different trans
-00000820: 6c61 7469 6f6e 2e00 4368 616e 6765 7320  lation..Changes 
-00000830: 6172 6520 6e6f 7420 6175 746f 6d61 7469  are not automati
-00000840: 6361 6c6c 7920 6170 706c 6965 6420 6265  cally applied be
-00000850: 7477 6565 6e20 7472 616e 736c 6174 6564  tween translated
-00000860: 2070 6167 6573 2e20 5379 6e63 696e 6720   pages. Syncing 
-00000870: 7769 6c6c 2061 6464 206e 6577 2063 6f6e  will add new con
-00000880: 7465 6e74 2066 6f72 2074 7261 6e73 6c61  tent for transla
-00000890: 7469 6f6e 2061 6e64 2072 656d 6f76 6520  tion and remove 
-000008a0: 6465 6c65 7465 6420 636f 6e74 656e 742e  deleted content.
-000008b0: 0043 686f 6f73 6520 6120 6c6f 6361 6c65  .Choose a locale
-000008c0: 2074 6f20 7379 6e63 6872 6f6e 6973 6520   to synchronise 
-000008d0: 636f 6e74 656e 7420 6672 6f6d 2e20 416e  content from. An
-000008e0: 7920 6578 6973 7469 6e67 2061 6e64 2066  y existing and f
-000008f0: 7574 7572 6520 636f 6e74 656e 7420 6175  uture content au
-00000900: 7468 6f72 6564 2069 6e20 7468 6520 7365  thored in the se
-00000910: 6c65 6374 6564 206c 6f63 616c 6520 7769  lected locale wi
-00000920: 6c6c 2062 6520 6175 746f 6d61 7469 6361  ll be automatica
-00000930: 6c6c 7920 636f 7069 6564 2074 6f20 7468  lly copied to th
-00000940: 6973 206f 6e65 2e00 436f 6e74 656e 7400  is one..Content.
-00000950: 436f 6e74 656e 7420 7479 7065 0043 6f6e  Content type.Con
-00000960: 7665 7274 2070 6167 6520 746f 2061 6c69  vert page to ali
-00000970: 6173 0043 6f6e 7665 7274 2074 6f20 616c  as.Convert to al
-00000980: 6961 7300 436f 6e76 6572 7420 746f 2061  ias.Convert to a
-00000990: 6c69 6173 2025 2874 6974 6c65 2973 0043  lias %(title)s.C
-000009a0: 6f6e 7665 7274 2074 6f20 616c 6961 7320  onvert to alias 
-000009b0: 7061 6765 0043 6f6e 7665 7274 6564 2070  page.Converted p
-000009c0: 6167 6520 2725 2874 6974 6c65 2973 2720  age '%(title)s' 
-000009d0: 746f 2061 6e20 616c 6961 7320 6f66 2074  to an alias of t
-000009e0: 6865 2074 7261 6e73 6c61 7469 6f6e 2073  he translation s
-000009f0: 6f75 7263 6520 7061 6765 2027 2528 736f  ource page '%(so
-00000a00: 7572 6365 5f74 6974 6c65 2973 2700 436f  urce_title)s'.Co
-00000a10: 6e76 6572 7465 6420 7061 6765 2074 6f20  nverted page to 
-00000a20: 616e 2061 6c69 6173 206f 6620 7468 6520  an alias of the 
-00000a30: 7472 616e 736c 6174 696f 6e20 736f 7572  translation sour
-00000a40: 6365 2070 6167 6500 4465 6c65 7465 0044  ce page.Delete.D
-00000a50: 6973 6162 6c65 0044 6f77 6e6c 6f61 6420  isable.Download 
-00000a60: 4353 5600 446f 776e 6c6f 6164 2058 4c53  CSV.Download XLS
-00000a70: 5800 4475 6d6d 7920 7472 616e 736c 6174  X.Dummy translat
-00000a80: 6f72 0045 6e61 626c 6500 476f 2062 6163  or.Enable.Go bac
-00000a90: 6b00 496e 636c 7564 6520 7375 6274 7265  k.Include subtre
-00000aa0: 6520 287b 7d20 7061 6765 2900 496e 636c  e ({} page).Incl
-00000ab0: 7564 6520 7375 6274 7265 6520 287b 7d20  ude subtree ({} 
-00000ac0: 7061 6765 7329 004c 6f63 616c 6573 004d  pages).Locales.M
-00000ad0: 6163 6869 6e65 004d 6163 6869 6e65 2074  achine.Machine t
-00000ae0: 7261 6e73 6c61 7465 6420 6f6e 207b 6461  ranslated on {da
-00000af0: 7465 7d00 4d61 6e75 616c 004e 6577 2076  te}.Manual.New v
-00000b00: 616c 6964 6174 696f 6e20 6572 726f 7273  alidation errors
-00000b10: 2077 6572 6520 666f 756e 6420 7768 656e   were found when
-00000b20: 2070 7562 6c69 7368 696e 6720 277b 6f62   publishing '{ob
-00000b30: 6a65 6374 7d27 2069 6e20 7b6c 6f63 616c  ject}' in {local
-00000b40: 657d 2e20 506c 6561 7365 2066 6978 2074  e}. Please fix t
-00000b50: 6865 6d20 6f72 2063 6c69 636b 2070 7562  hem or click pub
-00000b60: 6c69 7368 2061 6761 696e 2074 6f20 6967  lish again to ig
-00000b70: 6e6f 7265 2074 6865 7365 2074 7261 6e73  nore these trans
-00000b80: 6c61 7469 6f6e 7320 666f 7220 6e6f 772e  lations for now.
-00000b90: 004e 6f20 7472 616e 736c 6174 696f 6e73  .No translations
-00000ba0: 2066 6f75 6e64 2e00 4e6f 2c20 6c65 6176   found..No, leav
-00000bb0: 6520 6974 2061 7320 6120 7061 6765 0050  e it as a page.P
-00000bc0: 6167 6520 277b 7d27 2068 6173 2062 6565  age '{}' has bee
-00000bd0: 6e20 636f 6e76 6572 7465 6420 696e 746f  n converted into
-00000be0: 2061 6e20 616c 6961 732e 0050 6c65 6173   an alias..Pleas
-00000bf0: 6520 7570 6c6f 6164 2061 2076 616c 6964  e upload a valid
-00000c00: 2050 4f20 6669 6c65 2e00 5075 626c 6973   PO file..Publis
-00000c10: 6820 696d 6d65 6469 6174 656c 7900 5075  h immediately.Pu
-00000c20: 626c 6973 6865 6420 277b 6f62 6a65 6374  blished '{object
-00000c30: 7d27 2069 6e20 7b6c 6f63 616c 657d 2077  }' in {locale} w
-00000c40: 6974 6820 6d69 7373 696e 6720 7472 616e  ith missing tran
-00000c50: 736c 6174 696f 6e73 202d 2073 6565 2062  slations - see b
-00000c60: 656c 6f77 2e00 5075 626c 6973 6865 6420  elow..Published 
-00000c70: 277b 6f62 6a65 6374 7d27 2069 6e20 7b6c  '{object}' in {l
-00000c80: 6f63 616c 657d 2e00 5361 7665 0053 6176  ocale}..Save.Sav
-00000c90: 696e 67e2 80a6 0053 656c 6563 7420 616c  ing....Select al
-00000ca0: 6c00 536f 7572 6365 0053 6f75 7263 6520  l.Source.Source 
-00000cb0: 7469 746c 6500 5374 6172 7420 5379 6e63  title.Start Sync
-00000cc0: 6564 2074 7261 6e73 6c61 7469 6f6e 0053  ed translation.S
-00000cd0: 7461 7475 7300 5374 7269 6e67 7320 6361  tatus.Strings ca
-00000ce0: 6e6e 6f74 2068 6176 6520 616e 7920 4854  nnot have any HT
-00000cf0: 4d4c 2074 6167 7320 7769 7468 2061 7474  ML tags with att
-00000d00: 7269 6275 7465 7320 2865 7863 6570 7420  ributes (except 
-00000d10: 666f 7220 2769 6427 2069 6e20 3c61 3e20  for 'id' in <a> 
-00000d20: 7461 6773 2900 5375 626d 6974 0053 7563  tags).Submit.Suc
-00000d30: 6365 7373 6675 6c6c 7920 696d 706f 7274  cessfully import
-00000d40: 6564 2074 7261 6e73 6c61 7469 6f6e 7320  ed translations 
-00000d50: 6672 6f6d 2050 4f20 4669 6c65 2e00 5375  from PO File..Su
-00000d60: 6363 6573 7366 756c 6c79 2074 7261 6e73  ccessfully trans
-00000d70: 6c61 7465 6420 7769 7468 207b 7d2e 0053  lated with {}..S
-00000d80: 7563 6365 7373 6675 6c6c 7920 7570 6461  uccessfully upda
-00000d90: 7465 6420 7472 616e 736c 6174 696f 6e73  ted translations
-00000da0: 2066 6f72 2027 7b6f 626a 6563 747d 2700   for '{object}'.
-00000db0: 5379 6e63 2074 7261 6e73 6c61 7465 6420  Sync translated 
-00000dc0: 2528 6d6f 6465 6c5f 6e61 6d65 2973 0053  %(model_name)s.S
-00000dd0: 796e 6320 7472 616e 736c 6174 6564 2070  ync translated p
-00000de0: 6167 6573 0053 796e 6320 7472 616e 736c  ages.Sync transl
-00000df0: 6174 6564 2073 6e69 7070 6574 7300 5379  ated snippets.Sy
-00000e00: 6e63 2074 7261 6e73 6c61 7469 6f6e 7320  nc translations 
-00000e10: 6f66 2027 2528 7469 746c 6529 7327 0053  of '%(title)s'.S
-00000e20: 796e 6368 726f 6e69 7365 2063 6f6e 7465  ynchronise conte
-00000e30: 6e74 2066 726f 6d20 616e 6f74 6865 7220  nt from another 
-00000e40: 6c6f 6361 6c65 0054 6172 6765 7400 5468  locale.Target.Th
-00000e50: 6520 6461 7461 206d 6f64 656c 2066 6f72  e data model for
-00000e60: 2027 7b6d 6f64 656c 5f6e 616d 657d 2720   '{model_name}' 
-00000e70: 6861 7320 6265 656e 2063 6861 6e67 6564  has been changed
-00000e80: 2073 696e 6365 2074 6865 206c 6173 7420   since the last 
-00000e90: 7472 616e 736c 6174 696f 6e20 7379 6e63  translation sync
-00000ea0: 2e20 4966 2061 6e79 206e 6577 2066 6965  . If any new fie
-00000eb0: 6c64 7320 6861 7665 2062 6565 6e20 6164  lds have been ad
-00000ec0: 6465 6420 7265 6365 6e74 6c79 2c20 7468  ded recently, th
-00000ed0: 6573 6520 6d61 7920 6e6f 7420 6265 2076  ese may not be v
-00000ee0: 6973 6962 6c65 2075 6e74 696c 2074 6865  isible until the
-00000ef0: 206e 6578 7420 7472 616e 736c 6174 696f   next translatio
-00000f00: 6e20 7379 6e63 2e00 5468 6520 6c61 7374  n sync..The last
-00000f10: 2073 796e 6320 6461 7465 2077 6173 2025   sync date was %
-00000f20: 286c 6173 745f 7379 6e63 5f64 6174 6529  (last_sync_date)
-00000f30: 732e 2059 6f75 2061 7265 2061 626f 7574  s. You are about
-00000f40: 2074 6f20 7379 6e63 2074 6865 2066 6f6c   to sync the fol
-00000f50: 6c6f 7769 6e67 3a00 5468 6520 7061 6765  lowing:.The page
-00000f60: 2027 7b70 6167 655f 7469 746c 657d 2720   '{page_title}' 
-00000f70: 7761 7320 7375 6363 6573 7366 756c 6c79  was successfully
-00000f80: 2073 7562 6d69 7474 6564 2066 6f72 2074   submitted for t
-00000f90: 7261 6e73 6c61 7469 6f6e 2069 6e74 6f20  ranslation into 
-00000fa0: 7b6c 6f63 616c 6573 7d00 5468 6520 7b6d  {locales}.The {m
-00000fb0: 6f64 656c 5f6e 616d 657d 2027 7b6f 626a  odel_name} '{obj
-00000fc0: 6563 747d 2720 7761 7320 7375 6363 6573  ect}' was succes
-00000fd0: 7366 756c 6c79 2073 7562 6d69 7474 6564  sfully submitted
-00000fe0: 2066 6f72 2074 7261 6e73 6c61 7469 6f6e   for translation
-00000ff0: 2069 6e74 6f20 7b6c 6f63 616c 6573 7d00   into {locales}.
-00001000: 5468 6572 6520 6973 6e27 7420 616e 7974  There isn't anyt
-00001010: 6869 6e67 206c 6566 7420 746f 2074 7261  hing left to tra
-00001020: 6e73 6c61 7465 2e00 5468 6973 206c 6f63  nslate..This loc
-00001030: 616c 6520 6361 6e6e 6f74 2062 6520 7379  ale cannot be sy
-00001040: 6e63 6564 2069 6e74 6f20 6974 7365 6c66  nced into itself
-00001050: 2e00 5468 6973 2070 6167 6520 6861 736e  ..This page hasn
-00001060: 2774 2062 6565 6e20 7472 616e 736c 6174  't been translat
-00001070: 6564 2079 6574 2e20 4974 2069 7320 6d69  ed yet. It is mi
-00001080: 7272 6f72 696e 6720 7468 6520 3c61 2068  rroring the <a h
-00001090: 7265 663d 2225 2865 6469 745f 6f72 6967  ref="%(edit_orig
-000010a0: 696e 616c 5f70 6167 655f 7572 6c29 7322  inal_page_url)s"
-000010b0: 2074 6172 6765 743d 225f 626c 616e 6b22   target="_blank"
-000010c0: 3e25 286f 7269 6769 6e61 6c5f 6c6f 6361  >%(original_loca
-000010d0: 6c65 2973 2070 6167 653c 2f61 3e2e 0054  le)s page</a>..T
-000010e0: 6869 7320 7769 6c6c 2061 7070 6c79 2074  his will apply t
-000010f0: 6865 2075 7064 6174 6573 2061 6e64 2070  he updates and p
-00001100: 7562 6c69 7368 2069 6d6d 6564 6961 7465  ublish immediate
-00001110: 6c79 2c20 6265 666f 7265 2061 6e79 206e  ly, before any n
-00001120: 6577 2074 7261 6e73 6c61 7469 6f6e 7320  ew translations 
-00001130: 6861 7070 656e 2e00 5472 616e 736c 6174  happen..Translat
-00001140: 6500 5472 616e 736c 6174 6520 2725 2874  e.Translate '%(t
-00001150: 6974 6c65 2973 2700 5472 616e 736c 6174  itle)s'.Translat
-00001160: 6520 7061 6765 0054 7261 6e73 6c61 7465  e page.Translate
-00001170: 2074 6869 7320 7061 6765 0054 7261 6e73   this page.Trans
-00001180: 6c61 7465 207b 6d6f 6465 6c5f 6e61 6d65  late {model_name
-00001190: 7d00 5472 616e 736c 6174 6564 206d 616e  }.Translated man
-000011a0: 7561 6c6c 7920 6f6e 207b 6461 7465 7d00  ually on {date}.
-000011b0: 5472 616e 736c 6174 6564 2077 6974 6820  Translated with 
-000011c0: 7b74 6f6f 6c5f 6e61 6d65 7d20 6f6e 207b  {tool_name} on {
-000011d0: 6461 7465 7d00 5472 616e 736c 6174 696f  date}.Translatio
-000011e0: 6e20 6861 7320 6265 656e 2072 6573 7461  n has been resta
-000011f0: 7274 6564 2e00 5472 616e 736c 6174 696f  rted..Translatio
-00001200: 6e20 6861 7320 6265 656e 2073 746f 7070  n has been stopp
-00001210: 6564 2e00 5472 616e 736c 6174 696f 6e20  ed..Translation 
-00001220: 6f66 2025 2869 6e73 7461 6e63 6529 7320  of %(instance)s 
-00001230: 696e 746f 2025 286c 6f63 616c 6529 7300  into %(locale)s.
-00001240: 5472 616e 736c 6174 696f 6e73 0055 6e72  Translations.Unr
-00001250: 6563 6f67 6e69 7365 6420 6964 2066 6f75  ecognised id fou
-00001260: 6e64 2069 6e20 616e 203c 613e 2074 6167  nd in an <a> tag
-00001270: 3a20 7b7d 0055 7020 746f 2064 6174 6500  : {}.Up to date.
-00001280: 5570 6461 7465 2065 7869 7374 696e 6720  Update existing 
-00001290: 7472 616e 736c 6174 696f 6e73 0057 6169  translations.Wai
-000012a0: 7469 6e67 2066 6f72 2074 7261 6e73 6c61  ting for transla
-000012b0: 7469 6f6e 7300 5768 7920 776f 756c 6420  tions.Why would 
-000012c0: 4920 7379 6e63 206d 7920 7061 6765 3f00  I sync my page?.
-000012d0: 5965 732c 2063 6f6e 7665 7274 2069 7400  Yes, convert it.
-000012e0: 7b7d 206c 6f63 616c 6573 0052 6570 6f72  {} locales.Repor
-000012f0: 742d 4d73 6769 642d 4275 6773 2d54 6f3a  t-Msgid-Bugs-To:
-00001300: 200a 4c61 7374 2d54 7261 6e73 6c61 746f   .Last-Translato
-00001310: 723a 2044 616e 2042 7261 6768 6973 2c20  r: Dan Braghis, 
-00001320: 3230 3232 0a4c 616e 6775 6167 652d 5465  2022.Language-Te
-00001330: 616d 3a20 526f 6d61 6e69 616e 2028 6874  am: Romanian (ht
-00001340: 7470 733a 2f2f 7777 772e 7472 616e 7369  tps://www.transi
-00001350: 6665 782e 636f 6d2f 746f 7263 6862 6f78  fex.com/torchbox
-00001360: 2f74 6561 6d73 2f38 3030 392f 726f 2f29  /teams/8009/ro/)
-00001370: 0a43 6f6e 7465 6e74 2d54 7970 653a 2074  .Content-Type: t
-00001380: 6578 742f 706c 6169 6e3b 2063 6861 7273  ext/plain; chars
-00001390: 6574 3d55 5446 2d38 0a4c 616e 6775 6167  et=UTF-8.Languag
-000013a0: 653a 2072 6f0a 506c 7572 616c 2d46 6f72  e: ro.Plural-For
-000013b0: 6d73 3a20 6e70 6c75 7261 6c73 3d33 3b20  ms: nplurals=3; 
-000013c0: 706c 7572 616c 3d28 6e3d 3d31 3f30 3a28  plural=(n==1?0:(
-000013d0: 2828 6e25 3130 303e 3139 297c 7c28 286e  ((n%100>19)||((n
-000013e0: 2531 3030 3d3d 3029 2626 286e 213d 3029  %100==0)&&(n!=0)
-000013f0: 2929 3f32 3a31 2929 3b0a 0045 7469 6368  ))?2:1));..Etich
-00001400: 6574 6120 3c7b 7d3e 206e 7520 6573 7465  eta <{}> nu este
-00001410: 2070 6572 6d69 73c4 832e 20c8 9869 7275   permis... ..iru
-00001420: 7269 6c65 2064 6520 7465 7874 2070 6f74  rile de text pot
-00001430: 2073 c483 2063 6f6e c89b 696e c483 206e   s.. con..in.. n
-00001440: 756d 6169 2065 7469 6368 6574 6520 696e  umai etichete in
-00001450: 6c69 6e65 2048 544d 4c20 2870 7265 6375  line HTML (precu
-00001460: 6d20 3c62 3e2c 203c 613e 2900 546f 6174  m <b>, <a>).Toat
-00001470: 6520 7061 6769 6e69 6c65 2064 6573 6365  e paginile desce
-00001480: 6e64 6574 6520 766f 7220 6669 2063 7265  ndete vor fi cre
-00001490: 6174 652e 0053 6967 7572 2064 6f72 69c8  ate..Sigur dori.
-000014a0: 9b69 2073 c483 2063 6f6e 7665 7274 69c8  .i s.. converti.
-000014b0: 9b69 2061 6365 6173 74c4 8320 7061 6769  .i aceast.. pagi
-000014c0: 6ec4 8320 c3ae 6e74 7275 2d75 6e20 616c  n.. ..ntru-un al
-000014d0: 6961 733f 2041 6365 6173 74c4 8320 6163  ias? Aceast.. ac
-000014e0: c89b 6975 6e65 2076 6120 7375 7072 6173  ..iune va supras
-000014f0: 6372 6965 2063 6f6e c89b 696e 7574 756c  crie con..inutul
-00001500: 2070 6167 696e 6969 2063 7520 6365 6c20   paginii cu cel 
-00001510: 616c 2027 2528 736f 7572 6365 5f70 6167  al '%(source_pag
-00001520: 655f 7469 746c 6529 7327 2028 2528 736f  e_title)s' (%(so
-00001530: 7572 6365 5f70 6167 655f 6c6f 6361 6c65  urce_page_locale
-00001540: 2973 2900 4669 c899 6965 7275 6c20 504f  )s).Fi..ierul PO
-00001550: 2063 7265 6174 2070 656e 7472 7520 6f20   creat pentru o 
-00001560: 7472 6164 7563 6572 6520 6469 6665 7269  traducere diferi
-00001570: 7461 206e 7520 706f 6174 6520 6669 2069  ta nu poate fi i
-00001580: 6d70 6f72 7461 742e 004d 6f64 6966 6963  mportat..Modific
-00001590: c483 7269 6c65 206e 7520 7375 6e74 2061  ..rile nu sunt a
-000015a0: 706c 6963 6174 6520 6175 746f 6d61 7465  plicate automate
-000015b0: 20c3 ae6e 7472 6520 7061 6769 6e69 2074   ..ntre pagini t
-000015c0: 7261 6475 7365 2e20 5369 6e63 726f 6e69  raduse. Sincroni
-000015d0: 7a61 7265 6120 7661 2061 64c4 8375 6761  zarea va ad..uga
-000015e0: 2063 6f6e c89b 696e 7574 756c 206e 6f69   con..inutul noi
-000015f0: 20c8 9969 2076 6120 656c 696d 696e 6120   ..i va elimina 
-00001600: 636f 6ec8 9b69 6e75 7475 6c20 c899 7465  con..inutul ..te
-00001610: 7273 2e00 416c 6567 6520 6f20 6c6f 6361  rs..Alege o loca
-00001620: 6c69 7a61 7265 2070 656e 7472 7520 6120  lizare pentru a 
-00001630: 7369 6e63 726f 6e69 7a61 2063 6f6e c89b  sincroniza con..
-00001640: 696e 7574 2e20 4f72 6963 6520 636f 6ec8  inut. Orice con.
-00001650: 9b69 6e75 7420 6375 7265 6e74 2073 6175  .inut curent sau
-00001660: 2063 6f6e c89b 696e 7574 2063 7265 6174   con..inut creat
-00001670: 20c3 ae6e 206c 6f63 616c 697a 6172 6561   ..n localizarea
-00001680: 2073 656c 6563 7461 74c4 8320 7661 2066   selectat.. va f
-00001690: 6920 636f 7069 6174 2061 7574 6f6d 6174  i copiat automat
-000016a0: 20c3 ae6e 206c 6f63 616c 697a 6172 6561   ..n localizarea
-000016b0: 2073 656c 6563 7461 74c4 832e 0043 6f6e   selectat....Con
-000016c0: c89b 696e 7574 0054 6970 2064 6520 636f  ..inut.Tip de co
-000016d0: 6ec8 9b69 6e75 7400 436f 6e76 6572 7465  n..inut.Converte
-000016e0: 617a c483 2070 6167 696e 6120 c3ae 6e20  az.. pagina ..n 
-000016f0: 7061 6769 6ec4 8320 616c 6961 7300 436f  pagin.. alias.Co
-00001700: 6e76 6572 7465 617a c483 20c3 ae6e 2061  nverteaz.. ..n a
-00001710: 6c69 6173 0043 6f6e 7665 7274 6561 7ac4  lias.Converteaz.
-00001720: 8320 c3ae 6e20 616c 6961 7320 2528 7469  . ..n alias %(ti
-00001730: 746c 6529 7300 436f 6e76 6572 7465 617a  tle)s.Converteaz
-00001740: c483 20c3 ae6e 2070 6167 696e c483 2061  .. ..n pagin.. a
-00001750: 6c69 6173 0041 2063 6f6e 7665 7274 6974  lias.A convertit
-00001760: 2070 6167 696e 6120 2725 2874 6974 6c65   pagina '%(title
-00001770: 2973 2720 c3ae 6e74 722d 756e 2061 6c69  )s' ..ntr-un ali
-00001780: 6173 2061 6c20 7061 6769 6e69 6920 7375  as al paginii su
-00001790: 7273 c483 2027 2528 736f 7572 6365 5f74  rs.. '%(source_t
-000017a0: 6974 6c65 2973 2720 6120 7472 6164 7563  itle)s' a traduc
-000017b0: 6572 6969 0041 2063 6f6e 7665 7274 6974  erii.A convertit
-000017c0: 2070 6167 696e 6120 c3ae 6e74 722d 756e   pagina ..ntr-un
-000017d0: 2061 6c69 6173 2061 6c20 7061 6769 6e69   alias al pagini
-000017e0: 6920 7375 7273 c483 2061 2074 7261 6475  i surs.. a tradu
-000017f0: 6365 7269 6900 c898 7465 7267 6500 4465  cerii...terge.De
-00001800: 7a61 6374 6976 6561 7ac4 8300 4465 7363  zactiveaz...Desc
-00001810: 6172 63c4 8320 4353 5600 4465 7363 6172  arc.. CSV.Descar
-00001820: 63c4 8320 584c 5358 0054 7261 6475 63c4  c.. XLSX.Traduc.
-00001830: 8374 6f72 2066 616c 7300 4163 7469 7665  .tor fals.Active
-00001840: 617a c483 00c3 8e6e 6170 6f69 0049 6e63  az.....napoi.Inc
-00001850: 6c75 6465 2070 6167 696e 6920 6465 7363  lude pagini desc
-00001860: 656e 6465 6e74 6520 287b 7d20 7061 6769  endente ({} pagi
-00001870: 6ec4 8329 0049 6e63 6c75 6465 2070 6167  n..).Include pag
-00001880: 696e 6920 6465 7363 656e 6465 6e74 6520  ini descendente 
-00001890: 287b 7d20 7061 6769 6e69 2900 496e 636c  ({} pagini).Incl
-000018a0: 7564 6520 7061 6769 6e69 2064 6573 6365  ude pagini desce
-000018b0: 6e64 656e 7465 2028 7b7d 2070 6167 696e  ndente ({} pagin
-000018c0: 6929 004c 6f63 616c 697a c483 7269 0041  i).Localiz..ri.A
-000018d0: 7574 6f6d 6174 0054 7261 6475 7320 6175  utomat.Tradus au
-000018e0: 746f 6d61 7420 6c61 207b 6461 7465 7d00  tomat la {date}.
-000018f0: 4d61 6e75 616c 0045 726f 7269 2064 6520  Manual.Erori de 
-00001900: 7661 6c69 6461 7265 206e 6f69 2061 7520  validare noi au 
-00001910: 666f 7374 20c3 ae6e 7469 6c6e 6974 6520  fost ..ntilnite 
-00001920: 6c61 2070 7562 6c69 6361 7265 6120 277b  la publicarea '{
-00001930: 6f62 6a65 6374 7d27 20c3 ae6e 207b 6c6f  object}' ..n {lo
-00001940: 6361 6c65 7d2e 2056 c483 2072 7567 c483  cale}. V.. rug..
-00001950: 6d20 73c4 8320 6c65 2072 656d 6564 6961  m s.. le remedia
-00001960: c89b 692c 2073 6175 2061 70c4 8373 61c8  ..i, sau ap..sa.
-00001970: 9b69 2070 7562 6c69 6361 7265 2064 696e  .i publicare din
-00001980: 206e 6f75 2070 656e 7472 7520 6120 6967   nou pentru a ig
-00001990: 6e6f 7265 2061 6365 7374 6520 7472 6164  nore aceste trad
-000019a0: 7563 6572 6920 7065 6e74 7275 206d 6f6d  uceri pentru mom
-000019b0: 656e 742e 004e 7520 732d 6175 2067 c483  ent..Nu s-au g..
-000019c0: 7369 7420 7472 6164 7563 6572 692e 004e  sit traduceri..N
-000019d0: 752c 2070 c483 7374 7265 617a c483 2063  u, p..streaz.. c
-000019e0: 6120 7061 6769 6ec4 8300 5061 6769 6e61  a pagin...Pagina
-000019f0: 2027 7b7d 2720 6120 666f 7374 2063 6f6e   '{}' a fost con
-00001a00: 7665 7274 6974 c483 20c3 ae6e 2061 6c69  vertit.. ..n ali
-00001a10: 6173 2e00 c38e 6e63 c483 7263 61c8 9b69  as....nc..rca..i
-00001a20: 2066 69c8 9969 6572 2050 4f20 7661 6c69   fi..ier PO vali
-00001a30: 642e 0050 7562 6c69 6368 6561 7ac4 8320  d..Publicheaz.. 
-00001a40: 696d 6564 6961 7400 277b 6f62 6a65 6374  imediat.'{object
-00001a50: 7d27 2070 7562 6c69 6361 7428 c483 2920  }' publicat(..) 
-00001a60: c3ae 6e20 7b6c 6f63 616c 657d 2063 7520  ..n {locale} cu 
-00001a70: 7472 6164 7563 6572 6920 6c69 7073 c483  traduceri lips..
-00001a80: 202d 2076 657a 6920 6d61 6920 6a6f 732e   - vezi mai jos.
-00001a90: 0041 2070 7562 6c69 6361 7420 277b 6f62  .A publicat '{ob
-00001aa0: 6a65 6374 7d27 20c3 ae6e 207b 6c6f 6361  ject}' ..n {loca
-00001ab0: 6c65 7d2e 0053 616c 7665 617a c483 00c3  le}..Salveaz....
-00001ac0: 8e6e 2063 7572 7320 6465 2073 616c 7661  .n curs de salva
-00001ad0: 7265 2e2e 2e00 5365 6c65 6374 6561 7ac4  re....Selecteaz.
-00001ae0: 8320 746f 6174 6500 5375 7273 c483 0054  . toate.Surs...T
-00001af0: 6974 6c75 2073 7572 73c4 8300 c38e 6e63  itlu surs.....nc
-00001b00: 6570 6520 7472 6164 7563 6572 6520 7369  epe traducere si
-00001b10: 6e63 726f 6e69 7a61 74c4 8300 5374 6174  ncronizat...Stat
-00001b20: 7573 00c8 9869 7275 7269 6c65 2064 6520  us...irurile de 
-00001b30: 7465 7874 206e 7520 706f 7420 73c4 8320  text nu pot s.. 
-00001b40: 636f 6ec8 9b69 6ec4 8320 6574 6963 6865  con..in.. etiche
-00001b50: 7465 2048 544d 4c20 6375 2061 7472 6962  te HTML cu atrib
-00001b60: 7574 6520 6375 2065 7863 6570 c89b 6961  ute cu excep..ia
-00001b70: 2027 6964 2720 c3ae 6e20 6574 6963 6865   'id' ..n etiche
-00001b80: 7465 6c65 203c 613e 0054 7269 6d69 7465  tele <a>.Trimite
-00001b90: 0054 7261 6475 6365 7269 6c65 2064 696e  .Traducerile din
-00001ba0: 2066 69c8 9969 6572 2050 4f20 6175 2066   fi..ier PO au f
-00001bb0: 6f73 7420 696d 706f 7274 6174 6520 6375  ost importate cu
-00001bc0: 2073 7563 6365 732e 0054 7261 6475 6365   succes..Traduce
-00001bd0: 7265 2064 6520 7375 6363 6573 2063 7520  re de succes cu 
-00001be0: 7b7d 2e00 5472 6164 7563 6572 696c 6520  {}..Traducerile 
-00001bf0: 7065 6e74 7275 2027 7b6f 626a 6563 747d  pentru '{object}
-00001c00: 2720 6175 2066 6f73 7420 6163 7475 616c  ' au fost actual
-00001c10: 697a 6174 6500 5369 6e63 726f 6e69 7a65  izate.Sincronize
-00001c20: 617a c483 2025 286d 6f64 656c 5f6e 616d  az.. %(model_nam
-00001c30: 6529 7320 7472 6164 7573 28c4 8329 0053  e)s tradus(..).S
-00001c40: 696e 6372 6f6e 697a 6561 7ac4 8320 7061  incronizeaz.. pa
-00001c50: 6769 6e69 2074 7261 6475 7365 0053 696e  gini traduse.Sin
-00001c60: 6372 6f6e 697a 6561 7ac4 8320 6672 6167  cronizeaz.. frag
-00001c70: 6d65 6e74 6520 7472 6164 7573 6500 5369  mente traduse.Si
-00001c80: 6e63 726f 6e69 7a65 617a c483 2074 7261  ncronizeaz.. tra
-00001c90: 6475 6365 7269 6c65 2070 656e 7472 7520  ducerile pentru 
-00001ca0: 2725 2874 6974 6c65 2973 2700 5369 6e63  '%(title)s'.Sinc
-00001cb0: 726f 6e69 7a65 617a c483 2063 6f6e c89b  ronizeaz.. con..
-00001cc0: 696e 7574 2064 696e 2061 6c74 c483 206c  inut din alt.. l
-00001cd0: 6f63 616c 697a 6172 6500 c5a2 696e 74c4  ocalizare...int.
-00001ce0: 8300 4d6f 6465 6c75 6c20 6465 2064 6174  ..Modelul de dat
-00001cf0: 6520 7065 6e74 7275 2027 7b6d 6f64 656c  e pentru '{model
-00001d00: 5f6e 616d 657d 2720 6120 666f 7374 2073  _name}' a fost s
-00001d10: 6368 696d 6261 7420 6465 206c 6120 756c  chimbat de la ul
-00001d20: 7469 6d61 2073 696e 6372 6f6e 697a 6172  tima sincronizar
-00001d30: 6520 6465 2074 7261 6475 6365 7269 2e20  e de traduceri. 
-00001d40: 4461 63c4 8320 6175 2066 6f73 7420 6164  Dac.. au fost ad
-00001d50: c483 6761 7465 2063 c3a2 6d70 7572 6920  ..gate c..mpuri 
-00001d60: 6e6f 692c 2073 2d61 7220 7075 7465 6120  noi, s-ar putea 
-00001d70: 73c4 8320 6e75 2066 6965 2076 697a 6962  s.. nu fie vizib
-00001d80: 6c65 2070 c3a2 6ec4 8320 6c61 2075 726d  le p..n.. la urm
-00001d90: c483 746f 6172 6561 2073 696e 6372 6f6e  ..toarea sincron
-00001da0: 697a 6172 6520 6465 2074 7261 6475 6365  izare de traduce
-00001db0: 7269 2e00 556c 7469 6d61 2073 696e 6372  ri..Ultima sincr
-00001dc0: 6f6e 697a 6172 6520 6120 666f 7374 2070  onizare a fost p
-00001dd0: 6520 2528 6c61 7374 5f73 796e 635f 6461  e %(last_sync_da
-00001de0: 7465 2973 2e20 5375 6e74 65c8 9b69 2070  te)s. Sunte..i p
-00001df0: 6520 6361 6c65 2073 c483 2073 696e 6372  e cale s.. sincr
-00001e00: 6f6e 697a 61c8 9b69 2075 726d c483 746f  oniza..i urm..to
-00001e10: 6172 656c 653a 0050 6167 696e 6120 277b  arele:.Pagina '{
-00001e20: 7061 6765 5f74 6974 6c65 7d27 2061 2066  page_title}' a f
-00001e30: 6f73 7420 7472 696d 6973 c483 2070 656e  ost trimis.. pen
-00001e40: 7472 7520 7472 6164 7563 6572 6520 c3ae  tru traducere ..
-00001e50: 6e20 7b6c 6f63 616c 6573 7d00 7b6d 6f64  n {locales}.{mod
-00001e60: 656c 5f6e 616d 657d 2027 7b6f 626a 6563  el_name} '{objec
-00001e70: 747d 2720 6120 666f 7374 2074 7269 6d69  t}' a fost trimi
-00001e80: 7328 c483 2920 7065 6e74 7275 2074 7261  s(..) pentru tra
-00001e90: 6475 6365 7265 20c3 ae6e 207b 6c6f 6361  ducere ..n {loca
-00001ea0: 6c65 737d 004e 7520 6d61 6920 6573 7465  les}.Nu mai este
-00001eb0: 206e 696d 6963 2064 6520 7472 6164 7573   nimic de tradus
-00001ec0: 2e00 4163 6561 7374 c483 206c 6f63 616c  ..Aceast.. local
-00001ed0: 697a 6172 6520 6e75 2070 6f61 7465 2066  izare nu poate f
-00001ee0: 6920 7369 6e63 726f 6e69 7a61 74c4 8320  i sincronizat.. 
-00001ef0: c3ae 6e20 7369 6e65 2e00 4163 6561 74c4  ..n sine..Aceat.
-00001f00: 8320 7061 6769 6ec4 8320 6e2d 6120 666f  . pagin.. n-a fo
-00001f10: 7374 2074 7261 6475 73c4 8320 c899 6920  st tradus.. ..i 
-00001f20: 7265 666c 6563 74c4 8320 3c61 2068 7265  reflect.. <a hre
-00001f30: 663d 2225 2865 6469 745f 6f72 6967 696e  f="%(edit_origin
-00001f40: 616c 5f70 6167 655f 7572 6c29 7322 2074  al_page_url)s" t
-00001f50: 6172 6765 743d 225f 626c 616e 6b22 3e70  arget="_blank">p
-00001f60: 6167 696e 6120 2528 6f72 6967 696e 616c  agina %(original
-00001f70: 5f6c 6f63 616c 6529 733c 2f61 3e2e 0041  _locale)s</a>..A
-00001f80: 6365 6173 7461 2076 6120 6170 6c69 6361  ceasta va aplica
-00001f90: 206d 6f64 6966 6963 c483 7269 6c65 20c8   modific..rile .
-00001fa0: 9969 2076 6120 7075 626c 6963 6120 696d  .i va publica im
-00001fb0: 6564 6961 742c 20c3 ae6e 6169 6e74 6520  ediat, ..nainte 
-00001fc0: 6465 206f 7269 6365 2074 7261 6475 6365  de orice traduce
-00001fd0: 7269 206e 6f69 2e00 5472 6164 7563 65c8  ri noi..Traduce.
-00001fe0: 9b69 0054 7261 6475 6365 2027 2528 7469  .i.Traduce '%(ti
-00001ff0: 746c 6529 7327 0054 7261 6475 6365 2070  tle)s'.Traduce p
-00002000: 6167 696e c483 0054 7261 6475 6365 c89b  agin...Traduce..
-00002010: 6920 6163 6561 7374 c483 2070 6167 696e  i aceast.. pagin
-00002020: c483 0054 7261 6475 6365 207b 6d6f 6465  ...Traduce {mode
-00002030: 6c5f 6e61 6d65 7d00 5472 6164 7573 206d  l_name}.Tradus m
-00002040: 616e 7561 6c20 6c61 207b 6461 7465 7d00  anual la {date}.
-00002050: 5472 6164 7573 2063 7520 7b74 6f6f 6c5f  Tradus cu {tool_
-00002060: 6e61 6d65 7d20 6c61 2064 6174 6120 6465  name} la data de
-00002070: 207b 6461 7465 7d00 5472 6164 7563 6572   {date}.Traducer
-00002080: 6561 2061 2066 6f73 7420 7265 c3ae 6e63  ea a fost re..nc
-00002090: 6570 7574 c483 2e00 5472 6164 7563 6572  eput....Traducer
-000020a0: 6561 2061 2066 6f73 7420 6f70 7269 74c4  ea a fost oprit.
-000020b0: 832e 0054 7261 6475 6365 7265 6120 2528  ...Traducerea %(
-000020c0: 696e 7374 616e 6365 2973 20c3 ae6e 2025  instance)s ..n %
-000020d0: 286c 6f63 616c 6529 7300 5472 6164 7563  (locale)s.Traduc
-000020e0: 6572 6900 4964 206e 6572 6563 756e 6f73  eri.Id nerecunos
-000020f0: 6375 7420 67c4 8373 6974 20c3 ae6e 7472  cut g..sit ..ntr
-00002100: 752d 756e 2074 6167 203c 613e 3a20 7b7d  u-un tag <a>: {}
-00002110: 0041 6374 7561 6c69 7a61 7400 4163 7475  .Actualizat.Actu
-00002120: 616c 697a 6561 7ac4 8320 7472 6164 7563  alizeaz.. traduc
-00002130: 6572 6920 6578 6973 7465 6e74 6500 41c8  eri existente.A.
-00002140: 9974 6570 7420 7472 6164 7563 6572 6900  .tept traduceri.
-00002150: 4465 2063 6520 73c4 832d 6d69 2073 696e  De ce s..-mi sin
-00002160: 6372 6f6e 697a 657a 2070 6167 696e 613f  cronizez pagina?
-00002170: 0044 612c 2063 6f6e 7665 7274 6561 7ac4  .Da, converteaz.
-00002180: 8300 7b7d 206c 6f63 616c 697a c483 7269  ..{} localiz..ri
-00002190: 00                                       .
+00000000: de12 0495 0000 0000 5000 0000 1c00 0000  ........P.......
+00000010: 9c02 0000 6b00 0000 1c05 0000 0000 0000  ....k...........
+00000020: c806 0000 5e00 0000 c906 0000 2000 0000  ....^....... ...
+00000030: 2807 0000 aa00 0000 4907 0000 4300 0000  (.......I...C...
+00000040: f407 0000 8800 0000 3808 0000 9600 0000  ........8.......
+00000050: c108 0000 0700 0000 5809 0000 0c00 0000  ........X.......
+00000060: 6009 0000 1500 0000 6d09 0000 1000 0000  `.......m.......
+00000070: 8309 0000 1a00 0000 9409 0000 1500 0000  ................
+00000080: af09 0000 5800 0000 c509 0000 3900 0000  ....X.......9...
+00000090: 1e0a 0000 0600 0000 580a 0000 0700 0000  ........X.......
+000000a0: 5f0a 0000 0c00 0000 670a 0000 0d00 0000  _.......g.......
+000000b0: 740a 0000 1000 0000 820a 0000 2100 0000  t...........!...
+000000c0: 930a 0000 0600 0000 b50a 0000 0700 0000  ................
+000000d0: bc0a 0000 3400 0000 c40a 0000 0700 0000  ....4...........
+000000e0: f90a 0000 0700 0000 010b 0000 1c00 0000  ................
+000000f0: 090b 0000 0600 0000 260b 0000 9500 0000  ........&.......
+00000100: 2d0b 0000 1600 0000 c30b 0000 1600 0000  -...............
+00000110: da0b 0000 2b00 0000 f10b 0000 1e00 0000  ....+...........
+00000120: 1d0c 0000 1300 0000 3c0c 0000 4700 0000  ........<...G...
+00000130: 500c 0000 2100 0000 980c 0000 0400 0000  P...!...........
+00000140: ba0c 0000 0900 0000 bf0c 0000 0a00 0000  ................
+00000150: c90c 0000 0600 0000 d40c 0000 0c00 0000  ................
+00000160: db0c 0000 1800 0000 e80c 0000 0600 0000  ................
+00000170: 010d 0000 4f00 0000 080d 0000 0600 0000  ....O...........
+00000180: 580d 0000 3000 0000 5f0d 0000 2000 0000  X...0..._... ...
+00000190: 900d 0000 3000 0000 b10d 0000 1e00 0000  ....0...........
+000001a0: e20d 0000 1500 0000 010e 0000 1800 0000  ................
+000001b0: 170e 0000 2000 0000 300e 0000 2700 0000  .... ...0...'...
+000001c0: 510e 0000 0600 0000 790e 0000 b900 0000  Q.......y.......
+000001d0: 800e 0000 4f00 0000 3a0f 0000 5100 0000  ....O...:...Q...
+000001e0: 8a0f 0000 5500 0000 dc0f 0000 2700 0000  ....U.......'...
+000001f0: 3210 0000 2900 0000 5a10 0000 8c00 0000  2...)...Z.......
+00000200: 8410 0000 5800 0000 1111 0000 0900 0000  ....X...........
+00000210: 6a11 0000 1500 0000 7411 0000 0e00 0000  j.......t.......
+00000220: 8a11 0000 1300 0000 9911 0000 1600 0000  ................
+00000230: ad11 0000 1d00 0000 c411 0000 2500 0000  ............%...
+00000240: e211 0000 1f00 0000 0812 0000 1d00 0000  ................
+00000250: 2812 0000 2b00 0000 4612 0000 0c00 0000  (...+...F.......
+00000260: 7212 0000 2700 0000 7f12 0000 0a00 0000  r...'...........
+00000270: a712 0000 1c00 0000 b212 0000 1800 0000  ................
+00000280: cf12 0000 1900 0000 e812 0000 0f00 0000  ................
+00000290: 0213 0000 0a00 0000 1213 0000 0f01 0000  ................
+000002a0: 1d13 0000 7000 0000 2d14 0000 2900 0000  ....p...-...)...
+000002b0: 9e14 0000 ae00 0000 c814 0000 4400 0000  ............D...
+000002c0: 7715 0000 8a00 0000 bc15 0000 a800 0000  w...............
+000002d0: 4716 0000 0900 0000 f016 0000 1000 0000  G...............
+000002e0: fa16 0000 2500 0000 0b17 0000 1600 0000  ....%...........
+000002f0: 3117 0000 2000 0000 4817 0000 1e00 0000  1... ...H.......
+00000300: 6917 0000 5f00 0000 8817 0000 4000 0000  i..._.......@...
+00000310: e817 0000 0700 0000 2918 0000 0d00 0000  ........).......
+00000320: 3118 0000 0d00 0000 3f18 0000 0e00 0000  1.......?.......
+00000330: 4d18 0000 1000 0000 5c18 0000 2100 0000  M.......\...!...
+00000340: 6d18 0000 0a00 0000 8f18 0000 0700 0000  m...............
+00000350: 9a18 0000 7500 0000 a218 0000 0b00 0000  ....u...........
+00000360: 1819 0000 0700 0000 2419 0000 1800 0000  ........$.......
+00000370: 2c19 0000 0600 0000 4519 0000 bd00 0000  ,.......E.......
+00000380: 4c19 0000 1900 0000 0a1a 0000 1a00 0000  L...............
+00000390: 241a 0000 2900 0000 3f1a 0000 1e00 0000  $...)...?.......
+000003a0: 691a 0000 1400 0000 881a 0000 4800 0000  i...........H...
+000003b0: 9d1a 0000 2300 0000 e61a 0000 0900 0000  ....#...........
+000003c0: 0a1b 0000 1600 0000 141b 0000 1100 0000  ................
+000003d0: 2b1b 0000 0600 0000 3d1b 0000 0c00 0000  +.......=.......
+000003e0: 441b 0000 1f00 0000 511b 0000 0600 0000  D.......Q.......
+000003f0: 711b 0000 6500 0000 781b 0000 0700 0000  q...e...x.......
+00000400: de1b 0000 3700 0000 e61b 0000 1a00 0000  ....7...........
+00000410: 1e1c 0000 3100 0000 391c 0000 2800 0000  ....1...9...(...
+00000420: 6b1c 0000 1d00 0000 941c 0000 2000 0000  k........... ...
+00000430: b21c 0000 2d00 0000 d31c 0000 2d00 0000  ....-.......-...
+00000440: 011d 0000 0700 0000 2f1d 0000 d100 0000  ......../.......
+00000450: 371d 0000 6200 0000 091e 0000 4400 0000  7...b.......D...
+00000460: 6c1e 0000 4800 0000 b11e 0000 1c00 0000  l...H...........
+00000470: fa1e 0000 3700 0000 171f 0000 8400 0000  ....7...........
+00000480: 4f1f 0000 5800 0000 d41f 0000 0a00 0000  O...X...........
+00000490: 2d20 0000 1300 0000 3820 0000 0f00 0000  - ......8 ......
+000004a0: 4c20 0000 1b00 0000 5c20 0000 1200 0000  L ......\ ......
+000004b0: 7820 0000 1700 0000 8b20 0000 2700 0000  x ....... ..'...
+000004c0: a320 0000 1f00 0000 cb20 0000 1a00 0000  . ....... ......
+000004d0: eb20 0000 2600 0000 0621 0000 0900 0000  . ..&....!......
+000004e0: 2d21 0000 2c00 0000 3721 0000 0a00 0000  -!..,...7!......
+000004f0: 6421 0000 2100 0000 6f21 0000 1100 0000  d!..!...o!......
+00000500: 9121 0000 2000 0000 a321 0000 1000 0000  .!.. ....!......
+00000510: c421 0000 0e00 0000 d521 0000 0100 0000  .!.......!......
+00000520: 4e00 0000 2200 0000 0000 0000 0d00 0000  N..."...........
+00000530: 1000 0000 2b00 0000 0000 0000 0000 0000  ....+...........
+00000540: 1d00 0000 4100 0000 3d00 0000 0200 0000  ....A...=.......
+00000550: 2400 0000 1e00 0000 4900 0000 1c00 0000  $.......I.......
+00000560: 3500 0000 2f00 0000 1800 0000 3900 0000  5.../.......9...
+00000570: 0000 0000 0000 0000 3200 0000 4600 0000  ........2...F...
+00000580: 0000 0000 1f00 0000 0000 0000 2d00 0000  ............-...
+00000590: 0000 0000 0000 0000 1300 0000 2a00 0000  ............*...
+000005a0: 1b00 0000 3e00 0000 1200 0000 1100 0000  ....>...........
+000005b0: 4400 0000 4b00 0000 0000 0000 0500 0000  D...K...........
+000005c0: 4500 0000 4f00 0000 3a00 0000 0000 0000  E...O...:.......
+000005d0: 1500 0000 2600 0000 1a00 0000 0000 0000  ....&...........
+000005e0: 2900 0000 0000 0000 4a00 0000 1700 0000  ).......J.......
+000005f0: 0000 0000 0300 0000 3f00 0000 2000 0000  ........?... ...
+00000600: 0000 0000 3c00 0000 0700 0000 0000 0000  ....<...........
+00000610: 3400 0000 4200 0000 3800 0000 0400 0000  4...B...8.......
+00000620: 4800 0000 3600 0000 2800 0000 2c00 0000  H...6...(...,...
+00000630: 0c00 0000 0e00 0000 3b00 0000 1400 0000  ........;.......
+00000640: 3100 0000 0000 0000 0b00 0000 0000 0000  1...............
+00000650: 3300 0000 4d00 0000 1600 0000 0a00 0000  3...M...........
+00000660: 0f00 0000 2700 0000 4c00 0000 2300 0000  ....'...L...#...
+00000670: 0600 0000 0000 0000 0000 0000 4300 0000  ............C...
+00000680: 0000 0000 0000 0000 2e00 0000 0000 0000  ................
+00000690: 2100 0000 0900 0000 1900 0000 0800 0000  !...............
+000006a0: 0000 0000 3700 0000 0000 0000 2500 0000  ....7.......%...
+000006b0: 4700 0000 0000 0000 3000 0000 0000 0000  G.......0.......
+000006c0: 4000 0000 5000 0000 003c 7b7d 3e20 7461  @...P....<{}> ta
+000006d0: 6720 6973 206e 6f74 2061 6c6c 6f77 6564  g is not allowed
+000006e0: 2e20 5374 7269 6e67 7320 6361 6e20 6f6e  . Strings can on
+000006f0: 6c79 2063 6f6e 7461 696e 2073 7461 6e64  ly contain stand
+00000700: 6172 6420 4854 4d4c 2069 6e6c 696e 6520  ard HTML inline 
+00000710: 7461 6773 2028 7375 6368 2061 7320 3c62  tags (such as <b
+00000720: 3e2c 203c 613e 2900 416c 6c20 6368 696c  >, <a>).All chil
+00000730: 6420 7061 6765 7320 7769 6c6c 2062 6520  d pages will be 
+00000740: 6372 6561 7465 642e 0041 7265 2079 6f75  created..Are you
+00000750: 2073 7572 6520 796f 7520 7761 6e74 2074   sure you want t
+00000760: 6f20 636f 6e76 6572 7420 7468 6973 2070  o convert this p
+00000770: 6167 6520 696e 746f 2061 6e20 616c 6961  age into an alia
+00000780: 733f 2054 6869 7320 7769 6c6c 206f 7665  s? This will ove
+00000790: 7277 7269 7465 2074 6865 2063 6f6e 7465  rwrite the conte
+000007a0: 6e74 206f 6620 7468 6520 7061 6765 2077  nt of the page w
+000007b0: 6974 6820 7468 6520 636f 6e74 656e 7420  ith the content 
+000007c0: 6f66 2027 2528 736f 7572 6365 5f70 6167  of '%(source_pag
+000007d0: 655f 7469 746c 6529 7327 2028 2528 736f  e_title)s' (%(so
+000007e0: 7572 6365 5f70 6167 655f 6c6f 6361 6c65  urce_page_locale
+000007f0: 2973 2900 4361 6e6e 6f74 2069 6d70 6f72  )s).Cannot impor
+00000800: 7420 504f 2066 696c 6520 7468 6174 2077  t PO file that w
+00000810: 6173 2063 7265 6174 6564 2066 6f72 2061  as created for a
+00000820: 2064 6966 6665 7265 6e74 2074 7261 6e73   different trans
+00000830: 6c61 7469 6f6e 2e00 4368 616e 6765 7320  lation..Changes 
+00000840: 6172 6520 6e6f 7420 6175 746f 6d61 7469  are not automati
+00000850: 6361 6c6c 7920 6170 706c 6965 6420 6265  cally applied be
+00000860: 7477 6565 6e20 7472 616e 736c 6174 6564  tween translated
+00000870: 2070 6167 6573 2e20 5379 6e63 696e 6720   pages. Syncing 
+00000880: 7769 6c6c 2061 6464 206e 6577 2063 6f6e  will add new con
+00000890: 7465 6e74 2066 6f72 2074 7261 6e73 6c61  tent for transla
+000008a0: 7469 6f6e 2061 6e64 2072 656d 6f76 6520  tion and remove 
+000008b0: 6465 6c65 7465 6420 636f 6e74 656e 742e  deleted content.
+000008c0: 0043 686f 6f73 6520 6120 6c6f 6361 6c65  .Choose a locale
+000008d0: 2074 6f20 7379 6e63 6872 6f6e 6973 6520   to synchronise 
+000008e0: 636f 6e74 656e 7420 6672 6f6d 2e20 416e  content from. An
+000008f0: 7920 6578 6973 7469 6e67 2061 6e64 2066  y existing and f
+00000900: 7574 7572 6520 636f 6e74 656e 7420 6175  uture content au
+00000910: 7468 6f72 6564 2069 6e20 7468 6520 7365  thored in the se
+00000920: 6c65 6374 6564 206c 6f63 616c 6520 7769  lected locale wi
+00000930: 6c6c 2062 6520 6175 746f 6d61 7469 6361  ll be automatica
+00000940: 6c6c 7920 636f 7069 6564 2074 6f20 7468  lly copied to th
+00000950: 6973 206f 6e65 2e00 436f 6e74 656e 7400  is one..Content.
+00000960: 436f 6e74 656e 7420 7479 7065 0043 6f6e  Content type.Con
+00000970: 7665 7274 2070 6167 6520 746f 2061 6c69  vert page to ali
+00000980: 6173 0043 6f6e 7665 7274 2074 6f20 616c  as.Convert to al
+00000990: 6961 7300 436f 6e76 6572 7420 746f 2061  ias.Convert to a
+000009a0: 6c69 6173 2025 2874 6974 6c65 2973 0043  lias %(title)s.C
+000009b0: 6f6e 7665 7274 2074 6f20 616c 6961 7320  onvert to alias 
+000009c0: 7061 6765 0043 6f6e 7665 7274 6564 2070  page.Converted p
+000009d0: 6167 6520 2725 2874 6974 6c65 2973 2720  age '%(title)s' 
+000009e0: 746f 2061 6e20 616c 6961 7320 6f66 2074  to an alias of t
+000009f0: 6865 2074 7261 6e73 6c61 7469 6f6e 2073  he translation s
+00000a00: 6f75 7263 6520 7061 6765 2027 2528 736f  ource page '%(so
+00000a10: 7572 6365 5f74 6974 6c65 2973 2700 436f  urce_title)s'.Co
+00000a20: 6e76 6572 7465 6420 7061 6765 2074 6f20  nverted page to 
+00000a30: 616e 2061 6c69 6173 206f 6620 7468 6520  an alias of the 
+00000a40: 7472 616e 736c 6174 696f 6e20 736f 7572  translation sour
+00000a50: 6365 2070 6167 6500 4465 6c65 7465 0044  ce page.Delete.D
+00000a60: 6973 6162 6c65 0044 6f77 6e6c 6f61 6420  isable.Download 
+00000a70: 4353 5600 446f 776e 6c6f 6164 2058 4c53  CSV.Download XLS
+00000a80: 5800 4475 6d6d 7920 7472 616e 736c 6174  X.Dummy translat
+00000a90: 6f72 0045 6469 7469 6e67 2025 286f 626a  or.Editing %(obj
+00000aa0: 6563 745f 7479 7065 2973 2025 2874 6974  ect_type)s %(tit
+00000ab0: 6c65 2973 0045 6e61 626c 6500 476f 2062  le)s.Enable.Go b
+00000ac0: 6163 6b00 496e 636c 7564 6520 7375 6274  ack.Include subt
+00000ad0: 7265 6520 287b 7d20 7061 6765 2900 496e  ree ({} page).In
+00000ae0: 636c 7564 6520 7375 6274 7265 6520 287b  clude subtree ({
+00000af0: 7d20 7061 6765 7329 004c 6f63 616c 6573  } pages).Locales
+00000b00: 004d 6163 6869 6e65 004d 6163 6869 6e65  .Machine.Machine
+00000b10: 2074 7261 6e73 6c61 7465 6420 6f6e 207b   translated on {
+00000b20: 6461 7465 7d00 4d61 6e75 616c 004e 6577  date}.Manual.New
+00000b30: 2076 616c 6964 6174 696f 6e20 6572 726f   validation erro
+00000b40: 7273 2077 6572 6520 666f 756e 6420 7768  rs were found wh
+00000b50: 656e 2070 7562 6c69 7368 696e 6720 277b  en publishing '{
+00000b60: 6f62 6a65 6374 7d27 2069 6e20 7b6c 6f63  object}' in {loc
+00000b70: 616c 657d 2e20 506c 6561 7365 2066 6978  ale}. Please fix
+00000b80: 2074 6865 6d20 6f72 2063 6c69 636b 2070   them or click p
+00000b90: 7562 6c69 7368 2061 6761 696e 2074 6f20  ublish again to 
+00000ba0: 6967 6e6f 7265 2074 6865 7365 2074 7261  ignore these tra
+00000bb0: 6e73 6c61 7469 6f6e 7320 666f 7220 6e6f  nslations for no
+00000bc0: 772e 004e 6f20 7472 616e 736c 6174 696f  w..No translatio
+00000bd0: 6e73 2066 6f75 6e64 2e00 4e6f 2c20 6c65  ns found..No, le
+00000be0: 6176 6520 6974 2061 7320 6120 7061 6765  ave it as a page
+00000bf0: 0050 6167 6520 277b 7d27 2068 6173 2062  .Page '{}' has b
+00000c00: 6565 6e20 636f 6e76 6572 7465 6420 696e  een converted in
+00000c10: 746f 2061 6e20 616c 6961 732e 0050 6c65  to an alias..Ple
+00000c20: 6173 6520 7570 6c6f 6164 2061 2076 616c  ase upload a val
+00000c30: 6964 2050 4f20 6669 6c65 2e00 5075 626c  id PO file..Publ
+00000c40: 6973 6820 696d 6d65 6469 6174 656c 7900  ish immediately.
+00000c50: 5075 626c 6973 6865 6420 277b 6f62 6a65  Published '{obje
+00000c60: 6374 7d27 2069 6e20 7b6c 6f63 616c 657d  ct}' in {locale}
+00000c70: 2077 6974 6820 6d69 7373 696e 6720 7472   with missing tr
+00000c80: 616e 736c 6174 696f 6e73 202d 2073 6565  anslations - see
+00000c90: 2062 656c 6f77 2e00 5075 626c 6973 6865   below..Publishe
+00000ca0: 6420 277b 6f62 6a65 6374 7d27 2069 6e20  d '{object}' in 
+00000cb0: 7b6c 6f63 616c 657d 2e00 5361 7665 0053  {locale}..Save.S
+00000cc0: 6176 696e 67e2 80a6 0053 656c 6563 7420  aving....Select 
+00000cd0: 616c 6c00 536f 7572 6365 0053 6f75 7263  all.Source.Sourc
+00000ce0: 6520 7469 746c 6500 5374 6172 7420 5379  e title.Start Sy
+00000cf0: 6e63 6564 2074 7261 6e73 6c61 7469 6f6e  nced translation
+00000d00: 0053 7461 7475 7300 5374 7269 6e67 7320  .Status.Strings 
+00000d10: 6361 6e6e 6f74 2068 6176 6520 616e 7920  cannot have any 
+00000d20: 4854 4d4c 2074 6167 7320 7769 7468 2061  HTML tags with a
+00000d30: 7474 7269 6275 7465 7320 2865 7863 6570  ttributes (excep
+00000d40: 7420 666f 7220 2769 6427 2069 6e20 3c61  t for 'id' in <a
+00000d50: 3e20 7461 6773 2900 5375 626d 6974 0053  > tags).Submit.S
+00000d60: 7563 6365 7373 6675 6c6c 7920 696d 706f  uccessfully impo
+00000d70: 7274 6564 2074 7261 6e73 6c61 7469 6f6e  rted translation
+00000d80: 7320 6672 6f6d 2050 4f20 4669 6c65 2e00  s from PO File..
+00000d90: 5375 6363 6573 7366 756c 6c79 2074 7261  Successfully tra
+00000da0: 6e73 6c61 7465 6420 7769 7468 207b 7d2e  nslated with {}.
+00000db0: 0053 7563 6365 7373 6675 6c6c 7920 7570  .Successfully up
+00000dc0: 6461 7465 6420 7472 616e 736c 6174 696f  dated translatio
+00000dd0: 6e73 2066 6f72 2027 7b6f 626a 6563 747d  ns for '{object}
+00000de0: 2700 5379 6e63 2074 7261 6e73 6c61 7465  '.Sync translate
+00000df0: 6420 2528 6d6f 6465 6c5f 6e61 6d65 2973  d %(model_name)s
+00000e00: 0053 796e 6320 7472 616e 736c 6174 6564  .Sync translated
+00000e10: 2070 6167 6573 0053 796e 6320 7472 616e   pages.Sync tran
+00000e20: 736c 6174 6564 2073 6e69 7070 6574 7300  slated snippets.
+00000e30: 5379 6e63 2074 7261 6e73 6c61 7469 6f6e  Sync translation
+00000e40: 7320 6f66 2027 2528 7469 746c 6529 7327  s of '%(title)s'
+00000e50: 0053 796e 6368 726f 6e69 7365 2063 6f6e  .Synchronise con
+00000e60: 7465 6e74 2066 726f 6d20 616e 6f74 6865  tent from anothe
+00000e70: 7220 6c6f 6361 6c65 0054 6172 6765 7400  r locale.Target.
+00000e80: 5468 6520 6461 7461 206d 6f64 656c 2066  The data model f
+00000e90: 6f72 2027 7b6d 6f64 656c 5f6e 616d 657d  or '{model_name}
+00000ea0: 2720 6861 7320 6265 656e 2063 6861 6e67  ' has been chang
+00000eb0: 6564 2073 696e 6365 2074 6865 206c 6173  ed since the las
+00000ec0: 7420 7472 616e 736c 6174 696f 6e20 7379  t translation sy
+00000ed0: 6e63 2e20 4966 2061 6e79 206e 6577 2066  nc. If any new f
+00000ee0: 6965 6c64 7320 6861 7665 2062 6565 6e20  ields have been 
+00000ef0: 6164 6465 6420 7265 6365 6e74 6c79 2c20  added recently, 
+00000f00: 7468 6573 6520 6d61 7920 6e6f 7420 6265  these may not be
+00000f10: 2076 6973 6962 6c65 2075 6e74 696c 2074   visible until t
+00000f20: 6865 206e 6578 7420 7472 616e 736c 6174  he next translat
+00000f30: 696f 6e20 7379 6e63 2e00 5468 6520 6c61  ion sync..The la
+00000f40: 7374 2073 796e 6320 6461 7465 2077 6173  st sync date was
+00000f50: 2025 286c 6173 745f 7379 6e63 5f64 6174   %(last_sync_dat
+00000f60: 6529 732e 2059 6f75 2061 7265 2061 626f  e)s. You are abo
+00000f70: 7574 2074 6f20 7379 6e63 2074 6865 2066  ut to sync the f
+00000f80: 6f6c 6c6f 7769 6e67 3a00 5468 6520 7061  ollowing:.The pa
+00000f90: 6765 2027 7b70 6167 655f 7469 746c 657d  ge '{page_title}
+00000fa0: 2720 7761 7320 7375 6363 6573 7366 756c  ' was successful
+00000fb0: 6c79 2073 7562 6d69 7474 6564 2066 6f72  ly submitted for
+00000fc0: 2074 7261 6e73 6c61 7469 6f6e 2069 6e74   translation int
+00000fd0: 6f20 7b6c 6f63 616c 6573 7d00 5468 6520  o {locales}.The 
+00000fe0: 7b6d 6f64 656c 5f6e 616d 657d 2027 7b6f  {model_name} '{o
+00000ff0: 626a 6563 747d 2720 7761 7320 7375 6363  bject}' was succ
+00001000: 6573 7366 756c 6c79 2073 7562 6d69 7474  essfully submitt
+00001010: 6564 2066 6f72 2074 7261 6e73 6c61 7469  ed for translati
+00001020: 6f6e 2069 6e74 6f20 7b6c 6f63 616c 6573  on into {locales
+00001030: 7d00 5468 6572 6520 6973 6e27 7420 616e  }.There isn't an
+00001040: 7974 6869 6e67 206c 6566 7420 746f 2074  ything left to t
+00001050: 7261 6e73 6c61 7465 2e00 5468 6973 206c  ranslate..This l
+00001060: 6f63 616c 6520 6361 6e6e 6f74 2062 6520  ocale cannot be 
+00001070: 7379 6e63 6564 2069 6e74 6f20 6974 7365  synced into itse
+00001080: 6c66 2e00 5468 6973 2070 6167 6520 6861  lf..This page ha
+00001090: 736e 2774 2062 6565 6e20 7472 616e 736c  sn't been transl
+000010a0: 6174 6564 2079 6574 2e20 4974 2069 7320  ated yet. It is 
+000010b0: 6d69 7272 6f72 696e 6720 7468 6520 3c61  mirroring the <a
+000010c0: 2068 7265 663d 2225 2865 6469 745f 6f72   href="%(edit_or
+000010d0: 6967 696e 616c 5f70 6167 655f 7572 6c29  iginal_page_url)
+000010e0: 7322 2074 6172 6765 743d 225f 626c 616e  s" target="_blan
+000010f0: 6b22 3e25 286f 7269 6769 6e61 6c5f 6c6f  k">%(original_lo
+00001100: 6361 6c65 2973 2070 6167 653c 2f61 3e2e  cale)s page</a>.
+00001110: 0054 6869 7320 7769 6c6c 2061 7070 6c79  .This will apply
+00001120: 2074 6865 2075 7064 6174 6573 2061 6e64   the updates and
+00001130: 2070 7562 6c69 7368 2069 6d6d 6564 6961   publish immedia
+00001140: 7465 6c79 2c20 6265 666f 7265 2061 6e79  tely, before any
+00001150: 206e 6577 2074 7261 6e73 6c61 7469 6f6e   new translation
+00001160: 7320 6861 7070 656e 2e00 5472 616e 736c  s happen..Transl
+00001170: 6174 6500 5472 616e 736c 6174 6520 2725  ate.Translate '%
+00001180: 2874 6974 6c65 2973 2700 5472 616e 736c  (title)s'.Transl
+00001190: 6174 6520 7061 6765 0054 7261 6e73 6c61  ate page.Transla
+000011a0: 7465 2074 6869 7320 7061 6765 0054 7261  te this page.Tra
+000011b0: 6e73 6c61 7465 207b 6d6f 6465 6c5f 6e61  nslate {model_na
+000011c0: 6d65 7d00 5472 616e 736c 6174 6564 206d  me}.Translated m
+000011d0: 616e 7561 6c6c 7920 6f6e 207b 6461 7465  anually on {date
+000011e0: 7d00 5472 616e 736c 6174 6564 2077 6974  }.Translated wit
+000011f0: 6820 7b74 6f6f 6c5f 6e61 6d65 7d20 6f6e  h {tool_name} on
+00001200: 207b 6461 7465 7d00 5472 616e 736c 6174   {date}.Translat
+00001210: 696f 6e20 6861 7320 6265 656e 2072 6573  ion has been res
+00001220: 7461 7274 6564 2e00 5472 616e 736c 6174  tarted..Translat
+00001230: 696f 6e20 6861 7320 6265 656e 2073 746f  ion has been sto
+00001240: 7070 6564 2e00 5472 616e 736c 6174 696f  pped..Translatio
+00001250: 6e20 6f66 2025 2869 6e73 7461 6e63 6529  n of %(instance)
+00001260: 7320 696e 746f 2025 286c 6f63 616c 6529  s into %(locale)
+00001270: 7300 5472 616e 736c 6174 696f 6e73 0055  s.Translations.U
+00001280: 6e72 6563 6f67 6e69 7365 6420 6964 2066  nrecognised id f
+00001290: 6f75 6e64 2069 6e20 616e 203c 613e 2074  ound in an <a> t
+000012a0: 6167 3a20 7b7d 0055 7020 746f 2064 6174  ag: {}.Up to dat
+000012b0: 6500 5570 6461 7465 2065 7869 7374 696e  e.Update existin
+000012c0: 6720 7472 616e 736c 6174 696f 6e73 0057  g translations.W
+000012d0: 6169 7469 6e67 2066 6f72 2074 7261 6e73  aiting for trans
+000012e0: 6c61 7469 6f6e 7300 5768 7920 776f 756c  lations.Why woul
+000012f0: 6420 4920 7379 6e63 206d 7920 7061 6765  d I sync my page
+00001300: 3f00 5965 732c 2063 6f6e 7665 7274 2069  ?.Yes, convert i
+00001310: 7400 7b7d 206c 6f63 616c 6573 0052 6570  t.{} locales.Rep
+00001320: 6f72 742d 4d73 6769 642d 4275 6773 2d54  ort-Msgid-Bugs-T
+00001330: 6f3a 200a 4c61 7374 2d54 7261 6e73 6c61  o: .Last-Transla
+00001340: 746f 723a 2041 6c65 7820 4d6f 7265 6761  tor: Alex Morega
+00001350: 2c20 3230 3233 0a4c 616e 6775 6167 652d  , 2023.Language-
+00001360: 5465 616d 3a20 526f 6d61 6e69 616e 2028  Team: Romanian (
+00001370: 6874 7470 733a 2f2f 6170 702e 7472 616e  https://app.tran
+00001380: 7369 6665 782e 636f 6d2f 746f 7263 6862  sifex.com/torchb
+00001390: 6f78 2f74 6561 6d73 2f38 3030 392f 726f  ox/teams/8009/ro
+000013a0: 2f29 0a43 6f6e 7465 6e74 2d54 7970 653a  /).Content-Type:
+000013b0: 2074 6578 742f 706c 6169 6e3b 2063 6861   text/plain; cha
+000013c0: 7273 6574 3d55 5446 2d38 0a4c 616e 6775  rset=UTF-8.Langu
+000013d0: 6167 653a 2072 6f0a 506c 7572 616c 2d46  age: ro.Plural-F
+000013e0: 6f72 6d73 3a20 6e70 6c75 7261 6c73 3d33  orms: nplurals=3
+000013f0: 3b20 706c 7572 616c 3d28 6e3d 3d31 3f30  ; plural=(n==1?0
+00001400: 3a28 2828 6e25 3130 303e 3139 297c 7c28  :(((n%100>19)||(
+00001410: 286e 2531 3030 3d3d 3029 2626 286e 213d  (n%100==0)&&(n!=
+00001420: 3029 2929 3f32 3a31 2929 3b0a 0045 7469  0)))?2:1));..Eti
+00001430: 6368 6574 6120 3c7b 7d3e 206e 7520 6573  cheta <{}> nu es
+00001440: 7465 2070 6572 6d69 73c4 832e 20c8 9869  te permis... ..i
+00001450: 7275 7269 6c65 2064 6520 7465 7874 2070  rurile de text p
+00001460: 6f74 2073 c483 2063 6f6e c89b 696e c483  ot s.. con..in..
+00001470: 206e 756d 6169 2065 7469 6368 6574 6520   numai etichete 
+00001480: 696e 6c69 6e65 2048 544d 4c20 2870 7265  inline HTML (pre
+00001490: 6375 6d20 3c62 3e2c 203c 613e 2900 546f  cum <b>, <a>).To
+000014a0: 6174 6520 7061 6769 6e69 6c65 2064 6573  ate paginile des
+000014b0: 6365 6e64 656e 7465 2076 6f72 2066 6920  cendente vor fi 
+000014c0: 6372 6561 7465 2e00 5369 6775 7220 646f  create..Sigur do
+000014d0: 7269 c89b 6920 73c4 8320 636f 6e76 6572  ri..i s.. conver
+000014e0: 7469 c89b 6920 6163 6561 7374 c483 2070  ti..i aceast.. p
+000014f0: 6167 696e c483 20c3 ae6e 7472 752d 756e  agin.. ..ntru-un
+00001500: 2061 6c69 6173 3f20 4163 6561 7374 c483   alias? Aceast..
+00001510: 2061 63c8 9b69 756e 6520 7661 2073 7570   ac..iune va sup
+00001520: 7261 7363 7269 6520 636f 6ec8 9b69 6e75  rascrie con..inu
+00001530: 7475 6c20 7061 6769 6e69 6920 6375 2063  tul paginii cu c
+00001540: 656c 2061 6c20 2725 2873 6f75 7263 655f  el al '%(source_
+00001550: 7061 6765 5f74 6974 6c65 2973 2720 2825  page_title)s' (%
+00001560: 2873 6f75 7263 655f 7061 6765 5f6c 6f63  (source_page_loc
+00001570: 616c 6529 7329 0046 69c8 9969 6572 756c  ale)s).Fi..ierul
+00001580: 2050 4f20 6372 6561 7420 7065 6e74 7275   PO creat pentru
+00001590: 206f 2074 7261 6475 6365 7265 2064 6966   o traducere dif
+000015a0: 6572 6974 6120 6e75 2070 6f61 7465 2066  erita nu poate f
+000015b0: 6920 696d 706f 7274 6174 2e00 4d6f 6469  i importat..Modi
+000015c0: 6669 63c4 8372 696c 6520 6e75 2073 756e  fic..rile nu sun
+000015d0: 7420 6170 6c69 6361 7465 2061 7574 6f6d  t aplicate autom
+000015e0: 6174 6520 c3ae 6e74 7265 2070 6167 696e  ate ..ntre pagin
+000015f0: 6920 7472 6164 7573 652e 2053 696e 6372  i traduse. Sincr
+00001600: 6f6e 697a 6172 6561 2076 6120 6164 c483  onizarea va ad..
+00001610: 7567 6120 636f 6ec8 9b69 6e75 7475 6c20  uga con..inutul 
+00001620: 6e6f 6920 c899 6920 7661 2065 6c69 6d69  noi ..i va elimi
+00001630: 6e61 2063 6f6e c89b 696e 7574 756c 20c8  na con..inutul .
+00001640: 9974 6572 732e 0041 6c65 6765 206f 206c  .ters..Alege o l
+00001650: 6f63 616c 697a 6172 6520 7065 6e74 7275  ocalizare pentru
+00001660: 2061 2073 696e 6372 6f6e 697a 6120 636f   a sincroniza co
+00001670: 6ec8 9b69 6e75 742e 204f 7269 6365 2063  n..inut. Orice c
+00001680: 6f6e c89b 696e 7574 2063 7572 656e 7420  on..inut curent 
+00001690: 7361 7520 636f 6ec8 9b69 6e75 7420 6372  sau con..inut cr
+000016a0: 6561 7420 c3ae 6e20 6c6f 6361 6c69 7a61  eat ..n localiza
+000016b0: 7265 6120 7365 6c65 6374 6174 c483 2076  rea selectat.. v
+000016c0: 6120 6669 2063 6f70 6961 7420 6175 746f  a fi copiat auto
+000016d0: 6d61 7420 c3ae 6e20 6c6f 6361 6c69 7a61  mat ..n localiza
+000016e0: 7265 6120 7365 6c65 6374 6174 c483 2e00  rea selectat....
+000016f0: 436f 6ec8 9b69 6e75 7400 5469 7020 6465  Con..inut.Tip de
+00001700: 2063 6f6e c89b 696e 7574 0043 6f6e 7665   con..inut.Conve
+00001710: 7274 6561 7ac4 8320 7061 6769 6e61 20c3  rteaz.. pagina .
+00001720: ae6e 2070 6167 696e c483 2061 6c69 6173  .n pagin.. alias
+00001730: 0043 6f6e 7665 7274 6561 7ac4 8320 c3ae  .Converteaz.. ..
+00001740: 6e20 616c 6961 7300 436f 6e76 6572 7465  n alias.Converte
+00001750: 617a c483 20c3 ae6e 2061 6c69 6173 2025  az.. ..n alias %
+00001760: 2874 6974 6c65 2973 0043 6f6e 7665 7274  (title)s.Convert
+00001770: 6561 7ac4 8320 c3ae 6e20 7061 6769 6ec4  eaz.. ..n pagin.
+00001780: 8320 616c 6961 7300 4120 636f 6e76 6572  . alias.A conver
+00001790: 7469 7420 7061 6769 6e61 2027 2528 7469  tit pagina '%(ti
+000017a0: 746c 6529 7327 20c3 ae6e 7472 2d75 6e20  tle)s' ..ntr-un 
+000017b0: 616c 6961 7320 616c 2070 6167 696e 6969  alias al paginii
+000017c0: 2073 7572 73c4 8320 2725 2873 6f75 7263   surs.. '%(sourc
+000017d0: 655f 7469 746c 6529 7327 2061 2074 7261  e_title)s' a tra
+000017e0: 6475 6365 7269 6900 4120 636f 6e76 6572  ducerii.A conver
+000017f0: 7469 7420 7061 6769 6e61 20c3 ae6e 7472  tit pagina ..ntr
+00001800: 2d75 6e20 616c 6961 7320 616c 2070 6167  -un alias al pag
+00001810: 696e 6969 2073 7572 73c4 8320 6120 7472  inii surs.. a tr
+00001820: 6164 7563 6572 6969 00c8 9874 6572 6765  aducerii...terge
+00001830: 0044 657a 6163 7469 7665 617a c483 0044  .Dezactiveaz...D
+00001840: 6573 6361 7263 c483 2043 5356 0044 6573  escarc.. CSV.Des
+00001850: 6361 7263 c483 2058 4c53 5800 5472 6164  carc.. XLSX.Trad
+00001860: 7563 c483 746f 7220 6661 6c73 0045 6469  uc..tor fals.Edi
+00001870: 7461 7265 2025 286f 626a 6563 745f 7479  tare %(object_ty
+00001880: 7065 2973 2025 2874 6974 6c65 2973 0041  pe)s %(title)s.A
+00001890: 6374 6976 6561 7ac4 8300 c38e 6e61 706f  ctiveaz.....napo
+000018a0: 6900 496e 636c 7564 6520 7061 6769 6e69  i.Include pagini
+000018b0: 2064 6573 6365 6e64 656e 7465 2028 7b7d   descendente ({}
+000018c0: 2070 6167 696e c483 2900 496e 636c 7564   pagin..).Includ
+000018d0: 6520 7061 6769 6e69 2064 6573 6365 6e64  e pagini descend
+000018e0: 656e 7465 2028 7b7d 2070 6167 696e 6929  ente ({} pagini)
+000018f0: 0049 6e63 6c75 6465 2070 6167 696e 6920  .Include pagini 
+00001900: 6465 7363 656e 6465 6e74 6520 287b 7d20  descendente ({} 
+00001910: 7061 6769 6e69 2900 4c6f 6361 6c69 7ac4  pagini).Localiz.
+00001920: 8372 6900 4175 746f 6d61 7400 5472 6164  .ri.Automat.Trad
+00001930: 7573 2061 7574 6f6d 6174 206c 6120 7b64  us automat la {d
+00001940: 6174 657d 004d 616e 7561 6c00 4572 6f72  ate}.Manual.Eror
+00001950: 6920 6465 2076 616c 6964 6172 6520 6e6f  i de validare no
+00001960: 6920 6175 2066 6f73 7420 c3ae 6e74 696c  i au fost ..ntil
+00001970: 6e69 7465 206c 6120 7075 626c 6963 6172  nite la publicar
+00001980: 6561 2027 7b6f 626a 6563 747d 2720 c3ae  ea '{object}' ..
+00001990: 6e20 7b6c 6f63 616c 657d 2e20 56c4 8320  n {locale}. V.. 
+000019a0: 7275 67c4 836d 2073 c483 206c 6520 7265  rug..m s.. le re
+000019b0: 6d65 6469 61c8 9b69 2c20 7361 7520 6170  media..i, sau ap
+000019c0: c483 7361 c89b 6920 7075 626c 6963 6172  ..sa..i publicar
+000019d0: 6520 6469 6e20 6e6f 7520 7065 6e74 7275  e din nou pentru
+000019e0: 2061 2069 676e 6f72 6520 6163 6573 7465   a ignore aceste
+000019f0: 2074 7261 6475 6365 7269 2070 656e 7472   traduceri pentr
+00001a00: 7520 6d6f 6d65 6e74 2e00 4e75 2073 2d61  u moment..Nu s-a
+00001a10: 7520 67c4 8373 6974 2074 7261 6475 6365  u g..sit traduce
+00001a20: 7269 2e00 4e75 2c20 70c4 8373 7472 6561  ri..Nu, p..strea
+00001a30: 7ac4 8320 6361 2070 6167 696e c483 0050  z.. ca pagin...P
+00001a40: 6167 696e 6120 277b 7d27 2061 2066 6f73  agina '{}' a fos
+00001a50: 7420 636f 6e76 6572 7469 74c4 8320 c3ae  t convertit.. ..
+00001a60: 6e20 616c 6961 732e 00c3 8e6e 63c4 8372  n alias....nc..r
+00001a70: 6361 c89b 6920 6669 c899 6965 7220 504f  ca..i fi..ier PO
+00001a80: 2076 616c 6964 2e00 5075 626c 6963 6865   valid..Publiche
+00001a90: 617a c483 2069 6d65 6469 6174 0027 7b6f  az.. imediat.'{o
+00001aa0: 626a 6563 747d 2720 7075 626c 6963 6174  bject}' publicat
+00001ab0: 28c4 8329 20c3 ae6e 207b 6c6f 6361 6c65  (..) ..n {locale
+00001ac0: 7d20 6375 2074 7261 6475 6365 7269 206c  } cu traduceri l
+00001ad0: 6970 73c4 8320 2d20 7665 7a69 206d 6169  ips.. - vezi mai
+00001ae0: 206a 6f73 2e00 4120 7075 626c 6963 6174   jos..A publicat
+00001af0: 2027 7b6f 626a 6563 747d 2720 c3ae 6e20   '{object}' ..n 
+00001b00: 7b6c 6f63 616c 657d 2e00 5361 6c76 6561  {locale}..Salvea
+00001b10: 7ac4 8300 c38e 6e20 6375 7273 2064 6520  z.....n curs de 
+00001b20: 7361 6c76 6172 652e 2e2e 0053 656c 6563  salvare....Selec
+00001b30: 7465 617a c483 2074 6f61 7465 0053 7572  teaz.. toate.Sur
+00001b40: 73c4 8300 5469 746c 7520 7375 7273 c483  s...Titlu surs..
+00001b50: 00c3 8e6e 6365 7065 2074 7261 6475 6365  ...ncepe traduce
+00001b60: 7265 2073 696e 6372 6f6e 697a 6174 c483  re sincronizat..
+00001b70: 0053 7461 7475 7300 c898 6972 7572 696c  .Status...iruril
+00001b80: 6520 6465 2074 6578 7420 6e75 2070 6f74  e de text nu pot
+00001b90: 2073 c483 2063 6f6e c89b 696e c483 2065   s.. con..in.. e
+00001ba0: 7469 6368 6574 6520 4854 4d4c 2063 7520  tichete HTML cu 
+00001bb0: 6174 7269 6275 7465 2063 7520 6578 6365  atribute cu exce
+00001bc0: 70c8 9b69 6120 2769 6427 20c3 ae6e 2065  p..ia 'id' ..n e
+00001bd0: 7469 6368 6574 656c 6520 3c61 3e00 5472  tichetele <a>.Tr
+00001be0: 696d 6974 6500 5472 6164 7563 6572 696c  imite.Traduceril
+00001bf0: 6520 6469 6e20 6669 c899 6965 7220 504f  e din fi..ier PO
+00001c00: 2061 7520 666f 7374 2069 6d70 6f72 7461   au fost importa
+00001c10: 7465 2063 7520 7375 6363 6573 2e00 5472  te cu succes..Tr
+00001c20: 6164 7563 6572 6520 6465 2073 7563 6365  aducere de succe
+00001c30: 7320 6375 207b 7d2e 0054 7261 6475 6365  s cu {}..Traduce
+00001c40: 7269 6c65 2070 656e 7472 7520 277b 6f62  rile pentru '{ob
+00001c50: 6a65 6374 7d27 2061 7520 666f 7374 2061  ject}' au fost a
+00001c60: 6374 7561 6c69 7a61 7465 0053 696e 6372  ctualizate.Sincr
+00001c70: 6f6e 697a 6561 7ac4 8320 2528 6d6f 6465  onizeaz.. %(mode
+00001c80: 6c5f 6e61 6d65 2973 2074 7261 6475 7328  l_name)s tradus(
+00001c90: c483 2900 5369 6e63 726f 6e69 7a65 617a  ..).Sincronizeaz
+00001ca0: c483 2070 6167 696e 6920 7472 6164 7573  .. pagini tradus
+00001cb0: 6500 5369 6e63 726f 6e69 7a65 617a c483  e.Sincronizeaz..
+00001cc0: 2066 7261 676d 656e 7465 2074 7261 6475   fragmente tradu
+00001cd0: 7365 0053 696e 6372 6f6e 697a 6561 7ac4  se.Sincronizeaz.
+00001ce0: 8320 7472 6164 7563 6572 696c 6520 7065  . traducerile pe
+00001cf0: 6e74 7275 2027 2528 7469 746c 6529 7327  ntru '%(title)s'
+00001d00: 0053 696e 6372 6f6e 697a 6561 7ac4 8320  .Sincronizeaz.. 
+00001d10: 636f 6ec8 9b69 6e75 7420 6469 6e20 616c  con..inut din al
+00001d20: 74c4 8320 6c6f 6361 6c69 7a61 7265 00c5  t.. localizare..
+00001d30: a269 6e74 c483 004d 6f64 656c 756c 2064  .int...Modelul d
+00001d40: 6520 6461 7465 2070 656e 7472 7520 277b  e date pentru '{
+00001d50: 6d6f 6465 6c5f 6e61 6d65 7d27 2061 2066  model_name}' a f
+00001d60: 6f73 7420 7363 6869 6d62 6174 2064 6520  ost schimbat de 
+00001d70: 6c61 2075 6c74 696d 6120 7369 6e63 726f  la ultima sincro
+00001d80: 6e69 7a61 7265 2064 6520 7472 6164 7563  nizare de traduc
+00001d90: 6572 692e 2044 6163 c483 2061 7520 666f  eri. Dac.. au fo
+00001da0: 7374 2061 64c4 8367 6174 6520 63c3 a26d  st ad..gate c..m
+00001db0: 7075 7269 206e 6f69 2c20 732d 6172 2070  puri noi, s-ar p
+00001dc0: 7574 6561 2073 c483 206e 7520 6669 6520  utea s.. nu fie 
+00001dd0: 7669 7a69 626c 6520 70c3 a26e c483 206c  vizible p..n.. l
+00001de0: 6120 7572 6dc4 8374 6f61 7265 6120 7369  a urm..toarea si
+00001df0: 6e63 726f 6e69 7a61 7265 2064 6520 7472  ncronizare de tr
+00001e00: 6164 7563 6572 692e 0055 6c74 696d 6120  aduceri..Ultima 
+00001e10: 7369 6e63 726f 6e69 7a61 7265 2061 2066  sincronizare a f
+00001e20: 6f73 7420 7065 2025 286c 6173 745f 7379  ost pe %(last_sy
+00001e30: 6e63 5f64 6174 6529 732e 2053 756e 7465  nc_date)s. Sunte
+00001e40: c89b 6920 7065 2063 616c 6520 73c4 8320  ..i pe cale s.. 
+00001e50: 7369 6e63 726f 6e69 7a61 c89b 6920 7572  sincroniza..i ur
+00001e60: 6dc4 8374 6f61 7265 6c65 3a00 5061 6769  m..toarele:.Pagi
+00001e70: 6e61 2027 7b70 6167 655f 7469 746c 657d  na '{page_title}
+00001e80: 2720 6120 666f 7374 2074 7269 6d69 73c4  ' a fost trimis.
+00001e90: 8320 7065 6e74 7275 2074 7261 6475 6365  . pentru traduce
+00001ea0: 7265 20c3 ae6e 207b 6c6f 6361 6c65 737d  re ..n {locales}
+00001eb0: 007b 6d6f 6465 6c5f 6e61 6d65 7d20 277b  .{model_name} '{
+00001ec0: 6f62 6a65 6374 7d27 2061 2066 6f73 7420  object}' a fost 
+00001ed0: 7472 696d 6973 28c4 8329 2070 656e 7472  trimis(..) pentr
+00001ee0: 7520 7472 6164 7563 6572 6520 c3ae 6e20  u traducere ..n 
+00001ef0: 7b6c 6f63 616c 6573 7d00 4e75 206d 6169  {locales}.Nu mai
+00001f00: 2065 7374 6520 6e69 6d69 6320 6465 2074   este nimic de t
+00001f10: 7261 6475 732e 0041 6365 6173 74c4 8320  radus..Aceast.. 
+00001f20: 6c6f 6361 6c69 7a61 7265 206e 7520 706f  localizare nu po
+00001f30: 6174 6520 6669 2073 696e 6372 6f6e 697a  ate fi sincroniz
+00001f40: 6174 c483 20c3 ae6e 2073 696e 652e 0041  at.. ..n sine..A
+00001f50: 6365 6174 c483 2070 6167 696e c483 206e  ceat.. pagin.. n
+00001f60: 2d61 2066 6f73 7420 7472 6164 7573 c483  -a fost tradus..
+00001f70: 20c8 9969 2072 6566 6c65 6374 c483 203c   ..i reflect.. <
+00001f80: 6120 6872 6566 3d22 2528 6564 6974 5f6f  a href="%(edit_o
+00001f90: 7269 6769 6e61 6c5f 7061 6765 5f75 726c  riginal_page_url
+00001fa0: 2973 2220 7461 7267 6574 3d22 5f62 6c61  )s" target="_bla
+00001fb0: 6e6b 223e 7061 6769 6e61 2025 286f 7269  nk">pagina %(ori
+00001fc0: 6769 6e61 6c5f 6c6f 6361 6c65 2973 3c2f  ginal_locale)s</
+00001fd0: 613e 2e00 4163 6561 7374 6120 7661 2061  a>..Aceasta va a
+00001fe0: 706c 6963 6120 6d6f 6469 6669 63c4 8372  plica modific..r
+00001ff0: 696c 6520 c899 6920 7661 2070 7562 6c69  ile ..i va publi
+00002000: 6361 2069 6d65 6469 6174 2c20 c3ae 6e61  ca imediat, ..na
+00002010: 696e 7465 2064 6520 6f72 6963 6520 7472  inte de orice tr
+00002020: 6164 7563 6572 6920 6e6f 692e 0054 7261  aduceri noi..Tra
+00002030: 6475 6365 c89b 6900 5472 6164 7563 6520  duce..i.Traduce 
+00002040: 2725 2874 6974 6c65 2973 2700 5472 6164  '%(title)s'.Trad
+00002050: 7563 6520 7061 6769 6ec4 8300 5472 6164  uce pagin...Trad
+00002060: 7563 65c8 9b69 2061 6365 6173 74c4 8320  uce..i aceast.. 
+00002070: 7061 6769 6ec4 8300 5472 6164 7520 7b6d  pagin...Tradu {m
+00002080: 6f64 656c 5f6e 616d 657d 0054 7261 6475  odel_name}.Tradu
+00002090: 7320 6d61 6e75 616c 206c 6120 7b64 6174  s manual la {dat
+000020a0: 657d 0054 7261 6475 7320 6375 207b 746f  e}.Tradus cu {to
+000020b0: 6f6c 5f6e 616d 657d 206c 6120 6461 7461  ol_name} la data
+000020c0: 2064 6520 7b64 6174 657d 0054 7261 6475   de {date}.Tradu
+000020d0: 6365 7265 6120 6120 666f 7374 2072 65c3  cerea a fost re.
+000020e0: ae6e 6365 7075 74c4 832e 0054 7261 6475  .nceput....Tradu
+000020f0: 6365 7265 6120 6120 666f 7374 206f 7072  cerea a fost opr
+00002100: 6974 c483 2e00 5472 6164 7563 6572 6561  it....Traducerea
+00002110: 2025 2869 6e73 7461 6e63 6529 7320 c3ae   %(instance)s ..
+00002120: 6e20 2528 6c6f 6361 6c65 2973 0054 7261  n %(locale)s.Tra
+00002130: 6475 6365 7269 0049 6420 6e65 7265 6375  duceri.Id nerecu
+00002140: 6e6f 7363 7574 2067 c483 7369 7420 c3ae  noscut g..sit ..
+00002150: 6e74 7275 2d75 6e20 7461 6720 3c61 3e3a  ntru-un tag <a>:
+00002160: 207b 7d00 4163 7475 616c 697a 6174 0041   {}.Actualizat.A
+00002170: 6374 7561 6c69 7a65 617a c483 2074 7261  ctualizeaz.. tra
+00002180: 6475 6365 7269 2065 7869 7374 656e 7465  duceri existente
+00002190: 0041 c899 7465 7074 2074 7261 6475 6365  .A..tept traduce
+000021a0: 7269 0044 6520 6365 2073 c483 2d6d 6920  ri.De ce s..-mi 
+000021b0: 7369 6e63 726f 6e69 7a65 7a20 7061 6769  sincronizez pagi
+000021c0: 6e61 3f00 4461 2c20 636f 6e76 6572 7465  na?.Da, converte
+000021d0: 617a c483 007b 7d20 6c6f 6361 6c69 7ac4  az...{} localiz.
+000021e0: 8372 6900                                .ri.
```

### Comparing `wagtail-localize-1.5/wagtail_localize/locale/ro/LC_MESSAGES/django.po` & `wagtail-localize-1.5.1/wagtail_localize/locale/ro/LC_MESSAGES/django.po`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 #
 # Translators:
 # Dan Braghis, 2022
+# Alex Morega, 2023
 #
 msgid ""
 msgstr ""
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2022-10-17 21:00+0000\n"
-"Last-Translator: Dan Braghis, 2022\n"
-"Language-Team: Romanian (https://www.transifex.com/torchbox/teams/8009/ro/)\n"
+"POT-Creation-Date: 2023-02-23 14:15+0000\n"
+"Last-Translator: Alex Morega, 2023\n"
+"Language-Team: Romanian (https://app.transifex.com/torchbox/teams/8009/ro/)\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Language: ro\n"
 "Plural-Forms: nplurals=3; plural=(n==1?0:(((n%100>19)||((n%100==0)&&(n!=0)))?"
 "2:1));\n"
 
 msgid "Disable"
 msgstr "Dezactivează"
@@ -42,15 +43,15 @@
 msgstr "Descarcă XLSX"
 
 msgid "Download CSV"
 msgstr "Descarcă CSV"
 
 #, python-brace-format
 msgid "Translate {model_name}"
-msgstr "Traduce {model_name}"
+msgstr "Tradu {model_name}"
 
 #, python-brace-format
 msgid ""
 "The {model_name} '{object}' was successfully submitted for translation into "
 "{locales}"
 msgstr "{model_name} '{object}' a fost trimis(ă) pentru traducere în {locales}"
 
@@ -148,14 +149,18 @@
 msgid "Translate this page"
 msgstr "Traduceți această pagină"
 
 #, python-format
 msgid "Translation of %(instance)s into %(locale)s"
 msgstr "Traducerea %(instance)s în %(locale)s"
 
+#, python-format
+msgid "Editing %(object_type)s %(title)s"
+msgstr "Editare %(object_type)s %(title)s"
+
 msgid "Submit"
 msgstr "Trimite"
 
 msgid "Go back"
 msgstr "Înapoi"
 
 msgid "Content type"
@@ -254,15 +259,15 @@
 msgid "Select all"
 msgstr "Selectează toate"
 
 msgid "Locales"
 msgstr "Localizări"
 
 msgid "All child pages will be created."
-msgstr "Toate paginile descendete vor fi create."
+msgstr "Toate paginile descendente vor fi create."
 
 msgid "Include subtree ({} page)"
 msgid_plural "Include subtree ({} pages)"
 msgstr[0] "Include pagini descendente ({} pagină)"
 msgstr[1] "Include pagini descendente ({} pagini)"
 msgstr[2] "Include pagini descendente ({} pagini)"
```

### Comparing `wagtail-localize-1.5/wagtail_localize/locale/ro/LC_MESSAGES/djangojs.mo` & `wagtail-localize-1.5.1/wagtail_localize/locale/ro/LC_MESSAGES/djangojs.mo`

 * *Files 16% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,22 +1,19 @@
 msgid ""
 msgstr ""
 "Last-Translator: Dan Braghis, 2022\n"
-"Language-Team: Romanian (https://www.transifex.com/torchbox/teams/8009/ro/)\n"
+"Language-Team: Romanian (https://app.transifex.com/torchbox/teams/8009/ro/)\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Language: ro\n"
 "Plural-Forms: nplurals=3; plural=(n==1?0:(((n%100>19)||((n%100==0)&&(n!=0)))?"
 "2:1));\n"
 
 msgid "Apply editor lock"
 msgstr "Aplică blocaj editorial"
 
-msgid "Breadcrumb"
-msgstr "Traseu navigare"
-
 msgid "Cancel"
 msgstr "Anulează"
 
 msgid "Change %s"
 msgstr "Modifică %s"
 
 msgid "Change document"
@@ -51,17 +48,14 @@
 
 msgid "Download PO file"
 msgstr "Descarcă fișier PO"
 
 msgid "Download PO file and input translations offline"
 msgstr "Descarcă fișier PO și adaugă traduceri offline"
 
-msgid "Draft"
-msgstr "Ciornă"
-
 msgid "Edit"
 msgstr "Editează"
 
 msgid "Edit this %s"
 msgstr "Editează %s"
 
 msgid "Edit this document"
@@ -81,35 +75,26 @@
 
 msgid "Fetching image information..."
 msgstr "Preluare informație despre imagine..."
 
 msgid "Fetching page information..."
 msgstr "Preluare informație despre pagină..."
 
-msgid "Live"
-msgstr "Activată"
-
 msgid "Lock"
 msgstr "Încuie"
 
 msgid "Not translated"
 msgstr "Netradus"
 
 msgid "Preview"
 msgstr "Examinare"
 
 msgid "Publish in "
 msgstr "Publică în"
 
-msgid "Published"
-msgstr "Publicat"
-
-msgid "Published on "
-msgstr "Publicat pe"
-
 msgid "Publishing..."
 msgstr "Publicare..."
 
 msgid "Remove editor lock"
 msgstr "Elimină blocaj editorial"
 
 msgid "Revert to %s version"
```

### Comparing `wagtail-localize-1.5/wagtail_localize/locale/ro/LC_MESSAGES/djangojs.po` & `wagtail-localize-1.5.1/wagtail_localize/locale/ro/LC_MESSAGES/djangojs.po`

 * *Files 5% similar despite different names*

```diff
@@ -1,29 +1,26 @@
 #
 # Translators:
 # Dan Braghis, 2022
 #
 msgid ""
 msgstr ""
 "Last-Translator: Dan Braghis, 2022\n"
-"Language-Team: Romanian (https://www.transifex.com/torchbox/teams/8009/ro/)\n"
+"Language-Team: Romanian (https://app.transifex.com/torchbox/teams/8009/ro/)\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Language: ro\n"
 "Plural-Forms: nplurals=3; plural=(n==1?0:(((n%100>19)||((n%100==0)&&(n!=0)))?"
 "2:1));\n"
 
 msgid "[DELETED]"
 msgstr "[ȘTERS]"
 
 msgid "Apply editor lock"
 msgstr "Aplică blocaj editorial"
 
-msgid "Breadcrumb"
-msgstr "Traseu navigare"
-
 msgid "Cancel"
 msgstr "Anulează"
 
 msgid "Change %s"
 msgstr "Modifică %s"
 
 msgid "Change document"
@@ -58,17 +55,14 @@
 
 msgid "Download PO file"
 msgstr "Descarcă fișier PO"
 
 msgid "Download PO file and input translations offline"
 msgstr "Descarcă fișier PO și adaugă traduceri offline"
 
-msgid "Draft"
-msgstr "Ciornă"
-
 msgid "Edit"
 msgstr "Editează"
 
 msgid "Edit this %s"
 msgstr "Editează %s"
 
 msgid "Edit this document"
@@ -88,35 +82,26 @@
 
 msgid "Fetching image information..."
 msgstr "Preluare informație despre imagine..."
 
 msgid "Fetching page information..."
 msgstr "Preluare informație despre pagină..."
 
-msgid "Live"
-msgstr "Activată"
-
 msgid "Lock"
 msgstr "Încuie"
 
 msgid "Not translated"
 msgstr "Netradus"
 
 msgid "Preview"
 msgstr "Examinare"
 
 msgid "Publish in "
 msgstr "Publică în"
 
-msgid "Published"
-msgstr "Publicat"
-
-msgid "Published on "
-msgstr "Publicat pe"
-
 msgid "Publishing..."
 msgstr "Publicare..."
 
 msgid "Remove editor lock"
 msgstr "Elimină blocaj editorial"
 
 msgid "Revert to %s version"
```

### Comparing `wagtail-localize-1.5/wagtail_localize/locale/ru/LC_MESSAGES/django.mo` & `wagtail-localize-1.5.1/wagtail_localize/locale/ru/LC_MESSAGES/django.mo`

 * *Files 2% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,12 +1,12 @@
 msgid ""
 msgstr ""
 "Report-Msgid-Bugs-To: \n"
 "Last-Translator: Влад <integration.into.society@gmail.com>, 2022\n"
-"Language-Team: Russian (https://www.transifex.com/torchbox/teams/8009/ru/)\n"
+"Language-Team: Russian (https://app.transifex.com/torchbox/teams/8009/ru/)\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Language: ru\n"
 "Plural-Forms: nplurals=4; plural=(n%10==1 && n%100!=11 ? 0 : n%10>=2 && "
 "n%10<=4 && (n%100<12 || n%100>14) ? 1 : n%10==0 || (n%10>=5 && n%10<=9) || "
 "(n%100>=11 && n%100<=14)? 2 : 3);\n"
 
 msgid ""
```

### Comparing `wagtail-localize-1.5/wagtail_localize/locale/ru/LC_MESSAGES/django.po` & `wagtail-localize-1.5.1/wagtail_localize/locale/ru/LC_MESSAGES/django.po`

 * *Files 1% similar despite different names*

```diff
@@ -6,17 +6,17 @@
 # Sergey Mazanov <mvver@outlook.com>, 2022
 # Tatsiana Tsygan <art.tatsiana@gmail.com>, 2022
 # Влад <integration.into.society@gmail.com>, 2022
 #
 msgid ""
 msgstr ""
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2022-10-17 21:00+0000\n"
+"POT-Creation-Date: 2023-02-23 14:15+0000\n"
 "Last-Translator: Влад <integration.into.society@gmail.com>, 2022\n"
-"Language-Team: Russian (https://www.transifex.com/torchbox/teams/8009/ru/)\n"
+"Language-Team: Russian (https://app.transifex.com/torchbox/teams/8009/ru/)\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Language: ru\n"
 "Plural-Forms: nplurals=4; plural=(n%10==1 && n%100!=11 ? 0 : n%10>=2 && "
 "n%10<=4 && (n%100<12 || n%100>14) ? 1 : n%10==0 || (n%10>=5 && n%10<=9) || "
 "(n%100>=11 && n%100<=14)? 2 : 3);\n"
 
 msgid "Disable"
```

### Comparing `wagtail-localize-1.5/wagtail_localize/locale/ru/LC_MESSAGES/djangojs.mo` & `wagtail-localize-1.5.1/wagtail_localize/locale/ru/LC_MESSAGES/djangojs.mo`

 * *Files 20% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,23 +1,20 @@
 msgid ""
 msgstr ""
 "Last-Translator: Влад <integration.into.society@gmail.com>, 2022\n"
-"Language-Team: Russian (https://www.transifex.com/torchbox/teams/8009/ru/)\n"
+"Language-Team: Russian (https://app.transifex.com/torchbox/teams/8009/ru/)\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Language: ru\n"
 "Plural-Forms: nplurals=4; plural=(n%10==1 && n%100!=11 ? 0 : n%10>=2 && "
 "n%10<=4 && (n%100<12 || n%100>14) ? 1 : n%10==0 || (n%10>=5 && n%10<=9) || "
 "(n%100>=11 && n%100<=14)? 2 : 3);\n"
 
 msgid "Apply editor lock"
 msgstr "Применить блокировку редактора"
 
-msgid "Breadcrumb"
-msgstr "Навигационная цепочка"
-
 msgid "Cancel"
 msgstr "Отменить"
 
 msgid "Change %s"
 msgstr "Изменить %s"
 
 msgid "Change document"
@@ -52,17 +49,14 @@
 
 msgid "Download PO file"
 msgstr "Загрузить PO файл"
 
 msgid "Download PO file and input translations offline"
 msgstr "Скачать PO-файл и вводить переводы в автономном режиме"
 
-msgid "Draft"
-msgstr "Черновик"
-
 msgid "Edit"
 msgstr "Редактировать"
 
 msgid "Edit this %s"
 msgstr "Править %s"
 
 msgid "Edit this document"
@@ -82,35 +76,26 @@
 
 msgid "Fetching image information..."
 msgstr "Получение информации об изображении..."
 
 msgid "Fetching page information..."
 msgstr "Получение информации о странице..."
 
-msgid "Live"
-msgstr "Опубликовано"
-
 msgid "Lock"
 msgstr "Блокировка"
 
 msgid "Not translated"
 msgstr "Не переведено"
 
 msgid "Preview"
 msgstr "Предварительный просмотр"
 
 msgid "Publish in "
 msgstr "Опубликовать в"
 
-msgid "Published"
-msgstr "Опубликовано"
-
-msgid "Published on "
-msgstr "Опубликовано на"
-
 msgid "Publishing..."
 msgstr "Публикация..."
 
 msgid "Remove editor lock"
 msgstr "Убрать блокировку редактора"
 
 msgid "Revert to %s version"
```

### Comparing `wagtail-localize-1.5/wagtail_localize/locale/ru/LC_MESSAGES/djangojs.po` & `wagtail-localize-1.5.1/wagtail_localize/locale/ru/LC_MESSAGES/djangojs.po`

 * *Files 13% similar despite different names*

```diff
@@ -3,30 +3,27 @@
 # Sergey Mazanov <mvver@outlook.com>, 2021
 # Mikalai Radchuk <radchuk.m@gmail.com>, 2021
 # Влад <integration.into.society@gmail.com>, 2022
 #
 msgid ""
 msgstr ""
 "Last-Translator: Влад <integration.into.society@gmail.com>, 2022\n"
-"Language-Team: Russian (https://www.transifex.com/torchbox/teams/8009/ru/)\n"
+"Language-Team: Russian (https://app.transifex.com/torchbox/teams/8009/ru/)\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Language: ru\n"
 "Plural-Forms: nplurals=4; plural=(n%10==1 && n%100!=11 ? 0 : n%10>=2 && "
 "n%10<=4 && (n%100<12 || n%100>14) ? 1 : n%10==0 || (n%10>=5 && n%10<=9) || "
 "(n%100>=11 && n%100<=14)? 2 : 3);\n"
 
 msgid "[DELETED]"
 msgstr "[УДАЛЕНО]"
 
 msgid "Apply editor lock"
 msgstr "Применить блокировку редактора"
 
-msgid "Breadcrumb"
-msgstr "Навигационная цепочка"
-
 msgid "Cancel"
 msgstr "Отменить"
 
 msgid "Change %s"
 msgstr "Изменить %s"
 
 msgid "Change document"
@@ -61,17 +58,14 @@
 
 msgid "Download PO file"
 msgstr "Загрузить PO файл"
 
 msgid "Download PO file and input translations offline"
 msgstr "Скачать PO-файл и вводить переводы в автономном режиме"
 
-msgid "Draft"
-msgstr "Черновик"
-
 msgid "Edit"
 msgstr "Редактировать"
 
 msgid "Edit this %s"
 msgstr "Править %s"
 
 msgid "Edit this document"
@@ -91,35 +85,26 @@
 
 msgid "Fetching image information..."
 msgstr "Получение информации об изображении..."
 
 msgid "Fetching page information..."
 msgstr "Получение информации о странице..."
 
-msgid "Live"
-msgstr "Опубликовано"
-
 msgid "Lock"
 msgstr "Блокировка"
 
 msgid "Not translated"
 msgstr "Не переведено"
 
 msgid "Preview"
 msgstr "Предварительный просмотр"
 
 msgid "Publish in "
 msgstr "Опубликовать в"
 
-msgid "Published"
-msgstr "Опубликовано"
-
-msgid "Published on "
-msgstr "Опубликовано на"
-
 msgid "Publishing..."
 msgstr "Публикация..."
 
 msgid "Remove editor lock"
 msgstr "Убрать блокировку редактора"
 
 msgid "Revert to %s version"
```

### Comparing `wagtail-localize-1.5/wagtail_localize/locale/sk_SK/LC_MESSAGES/django.mo` & `wagtail-localize-1.5.1/wagtail_localize/locale/sk_SK/LC_MESSAGES/django.mo`

 * *Files 19% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,12 +1,12 @@
 msgid ""
 msgstr ""
 "Report-Msgid-Bugs-To: \n"
 "Last-Translator: Jozef Gáborík <hi@jozo.io>, 2022\n"
-"Language-Team: Slovak (Slovakia) (https://www.transifex.com/torchbox/"
+"Language-Team: Slovak (Slovakia) (https://app.transifex.com/torchbox/"
 "teams/8009/sk_SK/)\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Language: sk_SK\n"
 "Plural-Forms: nplurals=4; plural=(n % 1 == 0 && n == 1 ? 0 : n % 1 == 0 && n "
 ">= 2 && n <= 4 ? 1 : n % 1 != 0 ? 2: 3);\n"
 
 msgid "Content"
```

### Comparing `wagtail-localize-1.5/wagtail_localize/locale/sk_SK/LC_MESSAGES/django.po` & `wagtail-localize-1.5.1/wagtail_localize/locale/sk_SK/LC_MESSAGES/django.po`

 * *Files 4% similar despite different names*

```diff
@@ -3,17 +3,17 @@
 # dellax <michalnebbia@gmail.com>, 2022
 # Martin Janšto <mato@jansto.sk>, 2022
 # Jozef Gáborík <hi@jozo.io>, 2022
 #
 msgid ""
 msgstr ""
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2022-10-17 21:00+0000\n"
+"POT-Creation-Date: 2023-02-23 14:15+0000\n"
 "Last-Translator: Jozef Gáborík <hi@jozo.io>, 2022\n"
-"Language-Team: Slovak (Slovakia) (https://www.transifex.com/torchbox/"
+"Language-Team: Slovak (Slovakia) (https://app.transifex.com/torchbox/"
 "teams/8009/sk_SK/)\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Language: sk_SK\n"
 "Plural-Forms: nplurals=4; plural=(n % 1 == 0 && n == 1 ? 0 : n % 1 == 0 && n "
 ">= 2 && n <= 4 ? 1 : n % 1 != 0 ? 2: 3);\n"
 
 msgid "Saving…"
```

### Comparing `wagtail-localize-1.5/wagtail_localize/locale/sk_SK/LC_MESSAGES/djangojs.mo` & `wagtail-localize-1.5.1/wagtail_localize/locale/sk_SK/LC_MESSAGES/djangojs.mo`

 * *Files 12% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,11 +1,11 @@
 msgid ""
 msgstr ""
 "Last-Translator: Martin Janšto <mato@jansto.sk>, 2021\n"
-"Language-Team: Slovak (Slovakia) (https://www.transifex.com/torchbox/"
+"Language-Team: Slovak (Slovakia) (https://app.transifex.com/torchbox/"
 "teams/8009/sk_SK/)\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Language: sk_SK\n"
 "Plural-Forms: nplurals=4; plural=(n % 1 == 0 && n == 1 ? 0 : n % 1 == 0 && n "
 ">= 2 && n <= 4 ? 1 : n % 1 != 0 ? 2: 3);\n"
 
 msgid "Choose a document"
@@ -16,17 +16,14 @@
 
 msgid "Choose an image"
 msgstr "Vybrať obrázok"
 
 msgid "Delete"
 msgstr "Vymazať"
 
-msgid "Draft"
-msgstr "Koncept"
-
 msgid "Edit"
 msgstr "Upraviť"
 
 msgid "Edit this %s"
 msgstr "Upraviť toto %s"
 
 msgid "Edit this document"
@@ -34,17 +31,14 @@
 
 msgid "Edit this image"
 msgstr "Upraviť tento obrázok"
 
 msgid "Edit this page"
 msgstr "Upraviť túto stránku"
 
-msgid "Live"
-msgstr "Live"
-
 msgid "Lock"
 msgstr "Zamknúť"
 
 msgid "Preview"
 msgstr "Náhľad"
 
 msgid "Publishing..."
```

### Comparing `wagtail-localize-1.5/wagtail_localize/locale/sk_SK/LC_MESSAGES/djangojs.po` & `wagtail-localize-1.5.1/wagtail_localize/locale/sk_SK/LC_MESSAGES/djangojs.po`

 * *Files 16% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # Translators:
 # dellax <michalnebbia@gmail.com>, 2021
 # Martin Janšto <mato@jansto.sk>, 2021
 #
 msgid ""
 msgstr ""
 "Last-Translator: Martin Janšto <mato@jansto.sk>, 2021\n"
-"Language-Team: Slovak (Slovakia) (https://www.transifex.com/torchbox/"
+"Language-Team: Slovak (Slovakia) (https://app.transifex.com/torchbox/"
 "teams/8009/sk_SK/)\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Language: sk_SK\n"
 "Plural-Forms: nplurals=4; plural=(n % 1 == 0 && n == 1 ? 0 : n % 1 == 0 && n "
 ">= 2 && n <= 4 ? 1 : n % 1 != 0 ? 2: 3);\n"
 
 msgid "Choose a document"
@@ -21,17 +21,14 @@
 
 msgid "Choose an image"
 msgstr "Vybrať obrázok"
 
 msgid "Delete"
 msgstr "Vymazať"
 
-msgid "Draft"
-msgstr "Koncept"
-
 msgid "Edit"
 msgstr "Upraviť"
 
 msgid "Edit this %s"
 msgstr "Upraviť toto %s"
 
 msgid "Edit this document"
@@ -39,17 +36,14 @@
 
 msgid "Edit this image"
 msgstr "Upraviť tento obrázok"
 
 msgid "Edit this page"
 msgstr "Upraviť túto stránku"
 
-msgid "Live"
-msgstr "Live"
-
 msgid "Lock"
 msgstr "Zamknúť"
 
 msgid "Preview"
 msgstr "Náhľad"
 
 msgid "Publishing..."
```

### Comparing `wagtail-localize-1.5/wagtail_localize/locale/sl/LC_MESSAGES/django.mo` & `wagtail-localize-1.5.1/wagtail_localize/locale/sl/LC_MESSAGES/django.mo`

 * *Files 8% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,12 +1,12 @@
 msgid ""
 msgstr ""
 "Report-Msgid-Bugs-To: \n"
 "Last-Translator: Andrej Marsetič, 2023\n"
-"Language-Team: Slovenian (https://www.transifex.com/torchbox/teams/8009/"
+"Language-Team: Slovenian (https://app.transifex.com/torchbox/teams/8009/"
 "sl/)\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Language: sl\n"
 "Plural-Forms: nplurals=4; plural=(n%100==1 ? 0 : n%100==2 ? 1 : n%100==3 || "
 "n%100==4 ? 2 : 3);\n"
 
 msgid ""
@@ -51,14 +51,17 @@
 
 msgid "Convert to alias %(title)s"
 msgstr "Pretvori v vzdevek %(title)s"
 
 msgid "Convert to alias page"
 msgstr "Pretvori v vzdevek strani"
 
+msgid "Converted page to an alias of the translation source page"
+msgstr "Stran pretvorjena v vzdevek izvorne strani prevoda"
+
 msgid "Delete"
 msgstr "Izbriši"
 
 msgid "Disable"
 msgstr "Onemogoči"
 
 msgid "Download CSV"
@@ -135,14 +138,19 @@
 
 msgid "Start Synced translation"
 msgstr "Začnite sinhronizirani prevod"
 
 msgid "Status"
 msgstr "Status"
 
+msgid ""
+"Strings cannot have any HTML tags with attributes (except for 'id' in <a> "
+"tags)"
+msgstr "Nizi ne smejo imeti oznak HTML z atributi (razen 'id' <a> v oznakah)"
+
 msgid "Submit"
 msgstr "Pošlji"
 
 msgid "Successfully imported translations from PO File."
 msgstr "Prevodi so bili uspešno uvoženi iz datoteke PO."
 
 msgid "Successfully translated with {}."
@@ -183,14 +191,23 @@
 msgid "There isn't anything left to translate."
 msgstr "Nič več ni za prevesti."
 
 msgid "This locale cannot be synced into itself."
 msgstr "Tega jezika ni mogoče sinhronizirati samega s seboj."
 
 msgid ""
+"This page hasn't been translated yet. It is mirroring the <a "
+"href=\"%(edit_original_page_url)s\" target=\"_blank\">%(original_locale)s "
+"page</a>."
+msgstr ""
+"Ta stran še ni bila prevedena in zrcali <a "
+"href=\"%(edit_original_page_url)s\" target=\"_blank\">%(original_locale)s "
+"stran</a>."
+
+msgid ""
 "This will apply the updates and publish immediately, before any new "
 "translations happen."
 msgstr ""
 "S tem bodo posodobitve uporabljene in objavljene takoj, preden pride do "
 "novih prevodov."
 
 msgid "Translate"
```

### Comparing `wagtail-localize-1.5/wagtail_localize/locale/sl/LC_MESSAGES/django.po` & `wagtail-localize-1.5.1/wagtail_localize/locale/sl/LC_MESSAGES/django.po`

 * *Files 9% similar despite different names*

```diff
@@ -4,17 +4,17 @@
 # Matej Stavanja <matej.stavanja@zfm.si>, 2022
 # andrej55 <andrej.marsetic@gmail.com>, 2022
 # Andrej Marsetič, 2023
 #
 msgid ""
 msgstr ""
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2022-10-17 21:00+0000\n"
+"POT-Creation-Date: 2023-02-23 14:15+0000\n"
 "Last-Translator: Andrej Marsetič, 2023\n"
-"Language-Team: Slovenian (https://www.transifex.com/torchbox/teams/8009/"
+"Language-Team: Slovenian (https://app.transifex.com/torchbox/teams/8009/"
 "sl/)\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Language: sl\n"
 "Plural-Forms: nplurals=4; plural=(n%100==1 ? 0 : n%100==2 ? 1 : n%100==3 || "
 "n%100==4 ? 2 : 3);\n"
 
 msgid "Disable"
@@ -95,14 +95,19 @@
 msgid ""
 "<{}> tag is not allowed. Strings can only contain standard HTML inline tags "
 "(such as <b>, <a>)"
 msgstr ""
 "Oznaka <{}> ni dovoljena. Nizi lahko vsebujejo samo standardne oznake HTML v "
 "vrstici (kot so <b>, <a>)"
 
+msgid ""
+"Strings cannot have any HTML tags with attributes (except for 'id' in <a> "
+"tags)"
+msgstr "Nizi ne smejo imeti oznak HTML z atributi (razen 'id' <a> v oznakah)"
+
 msgid "Unrecognised id found in an <a> tag: {}"
 msgstr "V oznaki <a> je bil najden neprepoznan ID: {}"
 
 msgid "Enable"
 msgstr "Omogoči"
 
 #, python-format
@@ -114,14 +119,24 @@
 
 msgid "Yes, convert it"
 msgstr "Da, pretvori ga"
 
 msgid "No, leave it as a page"
 msgstr "Ne, pustite to kot stran"
 
+#, python-format
+msgid ""
+"This page hasn't been translated yet. It is mirroring the <a "
+"href=\"%(edit_original_page_url)s\" target=\"_blank\">%(original_locale)s "
+"page</a>."
+msgstr ""
+"Ta stran še ni bila prevedena in zrcali <a "
+"href=\"%(edit_original_page_url)s\" target=\"_blank\">%(original_locale)s "
+"stran</a>."
+
 msgid "Translate this page"
 msgstr "Prevedi to stran"
 
 #, python-format
 msgid "Translation of %(instance)s into %(locale)s"
 msgstr "Prevod od %(instance)s v%(locale)s"
 
@@ -264,7 +279,10 @@
 msgstr "Sinhroniziraj prevod  '%(title)s'"
 
 msgid "Convert to alias page"
 msgstr "Pretvori v vzdevek strani"
 
 msgid "Convert page to alias"
 msgstr "Pretvori stran v vzdevek"
+
+msgid "Converted page to an alias of the translation source page"
+msgstr "Stran pretvorjena v vzdevek izvorne strani prevoda"
```

### Comparing `wagtail-localize-1.5/wagtail_localize/locale/sl/LC_MESSAGES/djangojs.mo` & `wagtail-localize-1.5.1/wagtail_localize/locale/gl/LC_MESSAGES/djangojs.mo`

 * *Files 22% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,163 +1,146 @@
 msgid ""
 msgstr ""
-"Last-Translator: Andrej Marsetič, 2023\n"
-"Language-Team: Slovenian (https://www.transifex.com/torchbox/teams/8009/"
-"sl/)\n"
+"Last-Translator: X Bello <xbello@gmail.com>, 2022\n"
+"Language-Team: Galician (https://app.transifex.com/torchbox/teams/8009/gl/)\n"
 "Content-Type: text/plain; charset=UTF-8\n"
-"Language: sl\n"
-"Plural-Forms: nplurals=4; plural=(n%100==1 ? 0 : n%100==2 ? 1 : n%100==3 || "
-"n%100==4 ? 2 : 3);\n"
+"Language: gl\n"
+"Plural-Forms: nplurals=2; plural=(n != 1);\n"
 
 msgid "Apply editor lock"
-msgstr "Uporabi zaklepanje urejevalnika"
-
-msgid "Breadcrumb"
-msgstr "Drobtina"
+msgstr "Aplicar bloqueo de editor"
 
 msgid "Cancel"
-msgstr "Prekliči"
+msgstr "Cancelar"
 
 msgid "Change %s"
-msgstr "Spremeni %s"
+msgstr "Cambia %s"
 
 msgid "Change document"
-msgstr "Spremeni dokument"
+msgstr "Cambiar documento"
 
 msgid "Change image"
-msgstr "Spremeni sliko"
+msgstr "Cambiar imaxe"
 
 msgid "Change page"
-msgstr "Spremeni stran"
+msgstr "Cambiar páxina"
 
 msgid "Changed"
-msgstr "Spremenjeno"
+msgstr "Cambiado"
 
 msgid "Choose a %s"
-msgstr "Izberite %s"
+msgstr "Elixe un %s"
 
 msgid "Choose a document"
-msgstr "Izberite dokument"
+msgstr "Seleccionar un documento"
 
 msgid "Choose a page"
-msgstr "Izberite stran"
+msgstr "Selecciona unha páxina"
 
 msgid "Choose an image"
-msgstr "Izberi sliko"
+msgstr "Seleccionar unha imaxe"
 
 msgid "Convert to alias page"
-msgstr "Pretvori v vzdevek strani"
+msgstr "Converter en páxina alias"
 
 msgid "Delete"
-msgstr "Izbriši"
+msgstr "Eliminar"
 
 msgid "Download PO file"
-msgstr "Prenesi PO datoteko"
+msgstr "Descargar arquivo PO"
 
 msgid "Download PO file and input translations offline"
-msgstr "Prenesite datoteko PO in vnesite prevode brez povezave"
-
-msgid "Draft"
-msgstr "Osnutek"
+msgstr "Descargar arquivo PO e introducir traduccións sen conexión"
 
 msgid "Edit"
-msgstr "Uredi"
+msgstr "Editar"
 
 msgid "Edit this %s"
-msgstr "Uredi %s"
+msgstr "Editar este %s"
 
 msgid "Edit this document"
-msgstr "Uredi dokument"
+msgstr "Editar este documento"
 
 msgid "Edit this image"
-msgstr "Uredi sliko"
+msgstr "Editar esta imaxe"
 
 msgid "Edit this page"
-msgstr "Uredi stran"
+msgstr "Editar esta páxina"
 
 msgid "Fetching %s information..."
-msgstr "Pridobivanje podatkov %s ..."
+msgstr "Recopilando información de %s..."
 
 msgid "Fetching document information..."
-msgstr "Pridobivanje informacij o dokumentu ..."
+msgstr "Recopilando información do documento..."
 
 msgid "Fetching image information..."
-msgstr "Pridobivanje informacij o sliki ..."
+msgstr "Recopilar información da imaxe..."
 
 msgid "Fetching page information..."
-msgstr "Pridobivanje informacij o strani ..."
-
-msgid "Live"
-msgstr "V živo"
+msgstr "Recopilando información da páxina..."
 
 msgid "Lock"
-msgstr "Zakleni"
+msgstr "Bloquear"
 
 msgid "Not translated"
-msgstr "Ni prevedeno"
+msgstr "Non traducido"
 
 msgid "Preview"
-msgstr "Predogled"
+msgstr "Previsualizar"
 
 msgid "Publish in "
-msgstr "Objavi v"
-
-msgid "Published"
-msgstr "Objavljeno"
-
-msgid "Published on "
-msgstr "Objavljeno dne"
+msgstr "Publicar en "
 
 msgid "Publishing..."
-msgstr "Objava..."
+msgstr "Publicando..."
 
 msgid "Remove editor lock"
-msgstr "Odstranite zaklep urejevalnika"
+msgstr "Quitar bloqueo do editor"
 
 msgid "Revert to %s version"
-msgstr "Povrni na različico %s"
+msgstr "Reverter á versión %s"
 
 msgid "Save"
-msgstr "Shrani"
+msgstr "Gardar"
 
 msgid "Saving..."
-msgstr "Shranjevanje..."
+msgstr "Gardando..."
 
 msgid "Server error"
-msgstr "Napaka strežnika"
+msgstr "Erro do servidor"
 
 msgid "Stop Synced translation"
-msgstr "Ustavi sinhroniziran prevod"
+msgstr "Deter traducción Sincronizada"
 
 msgid "There are unsaved segments. Please save or cancel them before leaving."
 msgstr ""
-"Obstajajo neshranjeni segmenti. Pred odhodom jih shranite ali prekličite."
+"Hai segmentos sen gardar. Por favor, gárdaos ou cancélaos antes de sair."
 
 msgid "Translate"
-msgstr "Prevedi"
+msgstr "Traducir"
 
 msgid "Translate all missing strings with "
-msgstr "prevedite vse manjkajoče nize z"
+msgstr "Traducir tódolos textos faltantes con"
 
 msgid "Translate with "
-msgstr "Prevedi z"
+msgstr "Traducir con"
 
 msgid "Unlock"
-msgstr "Odkleni"
+msgstr "Desbloquear"
 
 msgid "Unpublish"
-msgstr "Umakni iz objave"
+msgstr "Cancelar publicación"
 
 msgid "Upload PO file"
-msgstr "Naložite PO datoteko"
+msgstr "Subir arquivo PO"
 
 msgid "Upload translated PO file to submit translations"
-msgstr "Naložite prevedeno datoteko PO, da objavite prevode"
+msgstr "Subir arquivo PO traducido para enviar traduccións"
 
 msgid "Uses %s version"
-msgstr "Uporabi %s različico"
+msgstr "Usa a versión %s"
 
 msgid "[DELETED]"
-msgstr "[IZBRISANO]"
+msgstr "[ELIMINADO]"
 
 msgid "segments translated"
-msgstr "segmenti prevedeni"
+msgstr "anacos traducidos"
```

### Comparing `wagtail-localize-1.5/wagtail_localize/locale/sl/LC_MESSAGES/djangojs.po` & `wagtail-localize-1.5.1/wagtail_localize/locale/fi/LC_MESSAGES/djangojs.po`

 * *Files 16% similar despite different names*

```diff
@@ -1,169 +1,134 @@
 #
 # Translators:
-# Mitja Pagon <mitja.pagon@inueni.com>, 2021
-# UP, 2021
-# Andrej Marsetič, 2023
+# Valter Maasalo <vmaasalo@gmail.com>, 2021
+# Aarni Koskela, 2021
+# Jiri Grönroos <jiri.gronroos@iki.fi>, 2022
 #
 msgid ""
 msgstr ""
-"Last-Translator: Andrej Marsetič, 2023\n"
-"Language-Team: Slovenian (https://www.transifex.com/torchbox/teams/8009/"
-"sl/)\n"
+"Last-Translator: Jiri Grönroos <jiri.gronroos@iki.fi>, 2022\n"
+"Language-Team: Finnish (https://app.transifex.com/torchbox/teams/8009/fi/)\n"
 "Content-Type: text/plain; charset=UTF-8\n"
-"Language: sl\n"
-"Plural-Forms: nplurals=4; plural=(n%100==1 ? 0 : n%100==2 ? 1 : n%100==3 || "
-"n%100==4 ? 2 : 3);\n"
+"Language: fi\n"
+"Plural-Forms: nplurals=2; plural=(n != 1);\n"
 
 msgid "[DELETED]"
-msgstr "[IZBRISANO]"
+msgstr "[POISTETTU]"
 
 msgid "Apply editor lock"
-msgstr "Uporabi zaklepanje urejevalnika"
-
-msgid "Breadcrumb"
-msgstr "Drobtina"
+msgstr "Toteuta editorin lukitus"
 
 msgid "Cancel"
-msgstr "Prekliči"
+msgstr "Peruuta"
 
 msgid "Change %s"
-msgstr "Spremeni %s"
+msgstr "Vaihda %s"
 
 msgid "Change document"
-msgstr "Spremeni dokument"
+msgstr "Vaihda dokumentti"
 
 msgid "Change image"
-msgstr "Spremeni sliko"
+msgstr "Vaihda kuva"
 
 msgid "Change page"
-msgstr "Spremeni stran"
+msgstr "Vaihda sivu"
 
 msgid "Changed"
-msgstr "Spremenjeno"
+msgstr "Vaihdettu"
 
 msgid "Choose a %s"
-msgstr "Izberite %s"
+msgstr "Valitse %s"
 
 msgid "Choose a document"
-msgstr "Izberite dokument"
+msgstr "Valitse dokumentti"
 
 msgid "Choose a page"
-msgstr "Izberite stran"
+msgstr "Valitse sivu"
 
 msgid "Choose an image"
-msgstr "Izberi sliko"
+msgstr "Valitse kuva"
 
 msgid "Convert to alias page"
-msgstr "Pretvori v vzdevek strani"
+msgstr "Muunna aliassivuksi"
 
 msgid "Delete"
-msgstr "Izbriši"
+msgstr "Poista"
 
 msgid "Download PO file"
-msgstr "Prenesi PO datoteko"
+msgstr "Lataa PO-tiedosto"
 
 msgid "Download PO file and input translations offline"
-msgstr "Prenesite datoteko PO in vnesite prevode brez povezave"
-
-msgid "Draft"
-msgstr "Osnutek"
+msgstr "Lataa PO-tiedosto ja syötä käännökset offline-tilassa"
 
 msgid "Edit"
-msgstr "Uredi"
+msgstr "Muokkaa"
 
 msgid "Edit this %s"
-msgstr "Uredi %s"
+msgstr "Muokkaa %s-kohdetta"
 
 msgid "Edit this document"
-msgstr "Uredi dokument"
+msgstr "Muokkaa tätä dokumenttia"
 
 msgid "Edit this image"
-msgstr "Uredi sliko"
+msgstr "Muokkaa tätä kuvaa"
 
 msgid "Edit this page"
-msgstr "Uredi stran"
-
-msgid "Fetching %s information..."
-msgstr "Pridobivanje podatkov %s ..."
+msgstr "Muokkaa tätä sivua"
 
 msgid "Fetching document information..."
-msgstr "Pridobivanje informacij o dokumentu ..."
+msgstr "Noudetaan dokumentin tietoja..."
 
 msgid "Fetching image information..."
-msgstr "Pridobivanje informacij o sliki ..."
+msgstr "Noudetaan kuvan tietoja..."
 
 msgid "Fetching page information..."
-msgstr "Pridobivanje informacij o strani ..."
-
-msgid "Live"
-msgstr "V živo"
+msgstr "Noudetaan sivun tietoja..."
 
 msgid "Lock"
-msgstr "Zakleni"
+msgstr "Lukitse"
 
 msgid "Not translated"
-msgstr "Ni prevedeno"
+msgstr "Ei käännetty"
 
 msgid "Preview"
-msgstr "Predogled"
-
-msgid "Publish in "
-msgstr "Objavi v"
-
-msgid "Published"
-msgstr "Objavljeno"
-
-msgid "Published on "
-msgstr "Objavljeno dne"
+msgstr "Esikatsele"
 
 msgid "Publishing..."
-msgstr "Objava..."
+msgstr "Julkaistaan..."
 
 msgid "Remove editor lock"
-msgstr "Odstranite zaklep urejevalnika"
-
-msgid "Revert to %s version"
-msgstr "Povrni na različico %s"
+msgstr "Poista editorin lukitus"
 
 msgid "Save"
-msgstr "Shrani"
+msgstr "Tallenna"
 
 msgid "Saving..."
-msgstr "Shranjevanje..."
+msgstr "Tallennetaan..."
 
 msgid "segments translated"
-msgstr "segmenti prevedeni"
+msgstr "segmenttiä käännetty"
 
 msgid "Server error"
-msgstr "Napaka strežnika"
-
-msgid "Stop Synced translation"
-msgstr "Ustavi sinhroniziran prevod"
+msgstr "Palvelinvirhe"
 
 msgid "There are unsaved segments. Please save or cancel them before leaving."
 msgstr ""
-"Obstajajo neshranjeni segmenti. Pred odhodom jih shranite ali prekličite."
+"Tallentamattomia segmenttejä. Tallenna ne tai peruuta ennen poistumista."
 
 msgid "Translate"
-msgstr "Prevedi"
-
-msgid "Translate all missing strings with "
-msgstr "prevedite vse manjkajoče nize z"
+msgstr "Käännä"
 
 msgid "Translate with "
-msgstr "Prevedi z"
+msgstr "Käännä käyttäen"
 
 msgid "Unlock"
-msgstr "Odkleni"
+msgstr "Avaa lukitus"
 
 msgid "Unpublish"
-msgstr "Umakni iz objave"
+msgstr "Piilota"
 
 msgid "Upload PO file"
-msgstr "Naložite PO datoteko"
+msgstr "Lähetä PO-tiedosto"
 
 msgid "Upload translated PO file to submit translations"
-msgstr "Naložite prevedeno datoteko PO, da objavite prevode"
-
-msgid "Uses %s version"
-msgstr "Uporabi %s različico"
+msgstr "Lähetä käännetty PO-tiedosto lähettääksesi käännökset"
```

### Comparing `wagtail-localize-1.5/wagtail_localize/locale/sr/LC_MESSAGES/django.po` & `wagtail-localize-1.5.1/wagtail_localize/locale/sr/LC_MESSAGES/django.po`

 * *Files 5% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 #
 # Translators:
 # Nikola Kadić <kadicnikola3@gmail.com>, 2022
 #
 msgid ""
 msgstr ""
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2022-10-17 21:00+0000\n"
+"POT-Creation-Date: 2023-02-23 14:15+0000\n"
 "Last-Translator: Nikola Kadić <kadicnikola3@gmail.com>, 2022\n"
-"Language-Team: Serbian (https://www.transifex.com/torchbox/teams/8009/sr/)\n"
+"Language-Team: Serbian (https://app.transifex.com/torchbox/teams/8009/sr/)\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Language: sr\n"
 "Plural-Forms: nplurals=3; plural=(n%10==1 && n%100!=11 ? 0 : n%10>=2 && "
 "n%10<=4 && (n%100<10 || n%100>=20) ? 1 : 2);\n"
 
 msgid "Saving…"
 msgstr "Čuvanje..."
```

### Comparing `wagtail-localize-1.5/wagtail_localize/locale/sv/LC_MESSAGES/django.mo` & `wagtail-localize-1.5.1/wagtail_localize/locale/sv/LC_MESSAGES/django.mo`

 * *Files 0% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,12 +1,12 @@
 msgid ""
 msgstr ""
 "Report-Msgid-Bugs-To: \n"
 "Last-Translator: Thomas Kunambi <kunambi@gmail.com>, 2022\n"
-"Language-Team: Swedish (https://www.transifex.com/torchbox/teams/8009/sv/)\n"
+"Language-Team: Swedish (https://app.transifex.com/torchbox/teams/8009/sv/)\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Language: sv\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
 
 msgid ""
 "<{}> tag is not allowed. Strings can only contain standard HTML inline tags "
 "(such as <b>, <a>)"
```

### Comparing `wagtail-localize-1.5/wagtail_localize/locale/sv/LC_MESSAGES/django.po` & `wagtail-localize-1.5.1/wagtail_localize/locale/sv/LC_MESSAGES/django.po`

 * *Files 1% similar despite different names*

```diff
@@ -4,17 +4,17 @@
 # Philip Andersen <renegadevi@codeofmagi.net>, 2022
 # Andreas Lans <andreas.lans@gmail.com>, 2022
 # Thomas Kunambi <kunambi@gmail.com>, 2022
 #
 msgid ""
 msgstr ""
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2022-10-17 21:00+0000\n"
+"POT-Creation-Date: 2023-02-23 14:15+0000\n"
 "Last-Translator: Thomas Kunambi <kunambi@gmail.com>, 2022\n"
-"Language-Team: Swedish (https://www.transifex.com/torchbox/teams/8009/sv/)\n"
+"Language-Team: Swedish (https://app.transifex.com/torchbox/teams/8009/sv/)\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Language: sv\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
 
 msgid "Disable"
 msgstr "Inaktivera"
```

### Comparing `wagtail-localize-1.5/wagtail_localize/locale/ta/LC_MESSAGES/django.po` & `wagtail-localize-1.5.1/wagtail_localize/locale/ta/LC_MESSAGES/django.po`

 * *Files 5% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 #
 # Translators:
 # Ramakrishnan Sathyanarayanan, 2022
 #
 msgid ""
 msgstr ""
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2022-10-17 21:00+0000\n"
+"POT-Creation-Date: 2023-02-23 14:15+0000\n"
 "Last-Translator: Ramakrishnan Sathyanarayanan, 2022\n"
-"Language-Team: Tamil (https://www.transifex.com/torchbox/teams/8009/ta/)\n"
+"Language-Team: Tamil (https://app.transifex.com/torchbox/teams/8009/ta/)\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Language: ta\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
 
 msgid "Saving…"
 msgstr "சேமிக்கின்றது "
```

### Comparing `wagtail-localize-1.5/wagtail_localize/locale/tet/LC_MESSAGES/django.mo` & `wagtail-localize-1.5.1/wagtail_localize/locale/tet/LC_MESSAGES/django.mo`

 * *Files 26% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,12 +1,12 @@
 msgid ""
 msgstr ""
 "Report-Msgid-Bugs-To: \n"
 "Last-Translator: Mariano de Deus <dedeus_mariano@yahoo.com>, 2022\n"
-"Language-Team: Tetum (Tetun) (https://www.transifex.com/torchbox/teams/8009/"
+"Language-Team: Tetum (Tetun) (https://app.transifex.com/torchbox/teams/8009/"
 "tet/)\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Language: tet\n"
 "Plural-Forms: nplurals=1; plural=0;\n"
 
 msgid "Content"
 msgstr "Konteudu"
```

### Comparing `wagtail-localize-1.5/wagtail_localize/locale/tet/LC_MESSAGES/django.po` & `wagtail-localize-1.5.1/wagtail_localize/locale/tet/LC_MESSAGES/django.po`

 * *Files 21% similar despite different names*

```diff
@@ -3,17 +3,17 @@
 # Peter Coward <peter@catalpa.io>, 2021
 # Joanico Barros <joanico@catalpa.io>, 2022
 # Mariano de Deus <dedeus_mariano@yahoo.com>, 2022
 #
 msgid ""
 msgstr ""
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2022-10-17 21:00+0000\n"
+"POT-Creation-Date: 2023-02-23 14:15+0000\n"
 "Last-Translator: Mariano de Deus <dedeus_mariano@yahoo.com>, 2022\n"
-"Language-Team: Tetum (Tetun) (https://www.transifex.com/torchbox/teams/8009/"
+"Language-Team: Tetum (Tetun) (https://app.transifex.com/torchbox/teams/8009/"
 "tet/)\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Language: tet\n"
 "Plural-Forms: nplurals=1; plural=0;\n"
 
 msgid "Saving…"
 msgstr "Rai tiha ona"
```

### Comparing `wagtail-localize-1.5/wagtail_localize/locale/tet/LC_MESSAGES/djangojs.mo` & `wagtail-localize-1.5.1/wagtail_localize/locale/tr/LC_MESSAGES/djangojs.mo`

 * *Files 26% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,56 +1,61 @@
 msgid ""
 msgstr ""
-"Last-Translator: Mariano de Deus <dedeus_mariano@yahoo.com>, 2021\n"
-"Language-Team: Tetum (Tetun) (https://www.transifex.com/torchbox/teams/8009/"
-"tet/)\n"
+"Last-Translator: Py Data Geek <pydatageek@gmail.com>, 2021\n"
+"Language-Team: Turkish (https://app.transifex.com/torchbox/teams/8009/tr/)\n"
 "Content-Type: text/plain; charset=UTF-8\n"
-"Language: tet\n"
-"Plural-Forms: nplurals=1; plural=0;\n"
+"Language: tr\n"
+"Plural-Forms: nplurals=2; plural=(n > 1);\n"
 
-msgid "Breadcrumb"
-msgstr "Hatudu dalan korta"
+msgid "Apply editor lock"
+msgstr "Editör kilidini kaldır"
 
 msgid "Change image"
-msgstr "Troka imajen"
+msgstr "Resmi değiştir"
+
+msgid "Choose a document"
+msgstr "Belge seç"
 
 msgid "Choose a page"
-msgstr "Hili pajina ida"
+msgstr "Bir sayfa seç"
 
 msgid "Choose an image"
-msgstr "Hili imagen ida"
+msgstr "Bir resim seç"
 
 msgid "Delete"
-msgstr "Hamoos"
-
-msgid "Draft"
-msgstr "Esbosu"
+msgstr "Sil"
 
 msgid "Edit"
-msgstr "Hadia"
+msgstr "Düzenle"
 
 msgid "Edit this %s"
-msgstr "hadia iha %s"
+msgstr "%s düzenle"
 
 msgid "Edit this document"
-msgstr "Hadia dokumentu nee"
+msgstr "Belgeyi düzenle"
 
 msgid "Edit this image"
-msgstr "Hadia imajen ne'e"
+msgstr "Resmi düzenle"
 
 msgid "Edit this page"
-msgstr "Hadia pajina nee"
-
-msgid "Live"
-msgstr "Ativu"
+msgstr "Sayfayı düzenle"
 
 msgid "Lock"
-msgstr "Xavi"
+msgstr "Kilitle"
 
 msgid "Preview"
-msgstr "Pré-visualizasaun"
+msgstr "Önizleme"
+
+msgid "Remove editor lock"
+msgstr "Editör kilidini kaldır"
 
 msgid "Save"
-msgstr "Rai"
+msgstr "Kaydet"
+
+msgid "Saving..."
+msgstr "Kaydediliyor"
+
+msgid "Unlock"
+msgstr "Kilidini aç"
 
 msgid "Unpublish"
-msgstr "La publika "
+msgstr "Yayından kaldır"
```

### Comparing `wagtail-localize-1.5/wagtail_localize/locale/tet/LC_MESSAGES/djangojs.po` & `wagtail-localize-1.5.1/wagtail_localize/locale/tet/LC_MESSAGES/djangojs.po`

 * *Files 5% similar despite different names*

```diff
@@ -4,38 +4,32 @@
 # Onorio de Jesus Afonso <onorio@catalpa.io>, 2021
 # Joanico Barros <joanico@catalpa.io>, 2021
 # Mariano de Deus <dedeus_mariano@yahoo.com>, 2021
 #
 msgid ""
 msgstr ""
 "Last-Translator: Mariano de Deus <dedeus_mariano@yahoo.com>, 2021\n"
-"Language-Team: Tetum (Tetun) (https://www.transifex.com/torchbox/teams/8009/"
+"Language-Team: Tetum (Tetun) (https://app.transifex.com/torchbox/teams/8009/"
 "tet/)\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Language: tet\n"
 "Plural-Forms: nplurals=1; plural=0;\n"
 
-msgid "Breadcrumb"
-msgstr "Hatudu dalan korta"
-
 msgid "Change image"
 msgstr "Troka imajen"
 
 msgid "Choose a page"
 msgstr "Hili pajina ida"
 
 msgid "Choose an image"
 msgstr "Hili imagen ida"
 
 msgid "Delete"
 msgstr "Hamoos"
 
-msgid "Draft"
-msgstr "Esbosu"
-
 msgid "Edit"
 msgstr "Hadia"
 
 msgid "Edit this %s"
 msgstr "hadia iha %s"
 
 msgid "Edit this document"
@@ -43,17 +37,14 @@
 
 msgid "Edit this image"
 msgstr "Hadia imajen ne'e"
 
 msgid "Edit this page"
 msgstr "Hadia pajina nee"
 
-msgid "Live"
-msgstr "Ativu"
-
 msgid "Lock"
 msgstr "Xavi"
 
 msgid "Preview"
 msgstr "Pré-visualizasaun"
 
 msgid "Save"
```

### Comparing `wagtail-localize-1.5/wagtail_localize/locale/th/LC_MESSAGES/django.mo` & `wagtail-localize-1.5.1/wagtail_localize/locale/th/LC_MESSAGES/django.mo`

 * *Files 18% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,12 +1,12 @@
 msgid ""
 msgstr ""
 "Report-Msgid-Bugs-To: \n"
 "Last-Translator: Walaksawan Vervoort <nula_wala@yahoo.com>, 2022\n"
-"Language-Team: Thai (https://www.transifex.com/torchbox/teams/8009/th/)\n"
+"Language-Team: Thai (https://app.transifex.com/torchbox/teams/8009/th/)\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Language: th\n"
 "Plural-Forms: nplurals=1; plural=0;\n"
 
 msgid "Content"
 msgstr "เนื้อหา"
```

### Comparing `wagtail-localize-1.5/wagtail_localize/locale/th/LC_MESSAGES/django.po` & `wagtail-localize-1.5.1/wagtail_localize/locale/th/LC_MESSAGES/django.po`

 * *Files 18% similar despite different names*

```diff
@@ -2,17 +2,17 @@
 # Translators:
 # Amawalee Combe <dang@getsalebox.com>, 2021
 # Walaksawan Vervoort <nula_wala@yahoo.com>, 2022
 #
 msgid ""
 msgstr ""
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2022-10-17 21:00+0000\n"
+"POT-Creation-Date: 2023-02-23 14:15+0000\n"
 "Last-Translator: Walaksawan Vervoort <nula_wala@yahoo.com>, 2022\n"
-"Language-Team: Thai (https://www.transifex.com/torchbox/teams/8009/th/)\n"
+"Language-Team: Thai (https://app.transifex.com/torchbox/teams/8009/th/)\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Language: th\n"
 "Plural-Forms: nplurals=1; plural=0;\n"
 
 msgid "Saving…"
 msgstr "กำลังเซฟ...,กำลังเก็บข้อมูล"
```

### Comparing `wagtail-localize-1.5/wagtail_localize/locale/th/LC_MESSAGES/djangojs.mo` & `wagtail-localize-1.5.1/wagtail_localize/locale/th/LC_MESSAGES/djangojs.mo`

 * *Files 20% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,11 +1,11 @@
 msgid ""
 msgstr ""
 "Last-Translator: Walaksawan Vervoort <nula_wala@yahoo.com>, 2021\n"
-"Language-Team: Thai (https://www.transifex.com/torchbox/teams/8009/th/)\n"
+"Language-Team: Thai (https://app.transifex.com/torchbox/teams/8009/th/)\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Language: th\n"
 "Plural-Forms: nplurals=1; plural=0;\n"
 
 msgid "Change image"
 msgstr "เปลี่ยนรูปภาพ"
 
@@ -17,17 +17,14 @@
 
 msgid "Choose an image"
 msgstr "เลือกรูปภาพ"
 
 msgid "Delete"
 msgstr "ลบ,ลบทิ้ง"
 
-msgid "Draft"
-msgstr "ร่าง , ข้อความที่เก็บเอาไว้ทำใหม่"
-
 msgid "Edit"
 msgstr "แก้ไข"
 
 msgid "Edit this %s"
 msgstr "แก้ไขสิ่งนี้ %s"
 
 msgid "Edit this document"
@@ -35,17 +32,14 @@
 
 msgid "Edit this image"
 msgstr "แก้ไขรูปภาพนี้"
 
 msgid "Edit this page"
 msgstr "แก้ไขหน้านี้"
 
-msgid "Live"
-msgstr "กำลังแสดงสดอยู่,ถ่ายทอดสด"
-
 msgid "Lock"
 msgstr "ล็อค"
 
 msgid "Preview"
 msgstr "ภาพตัวอย่าง"
 
 msgid "Save"
```

### Comparing `wagtail-localize-1.5/wagtail_localize/locale/th/LC_MESSAGES/djangojs.po` & `wagtail-localize-1.5.1/wagtail_localize/locale/th/LC_MESSAGES/djangojs.po`

 * *Files 8% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # Translators:
 # Amawalee Combe <dang@getsalebox.com>, 2021
 # Walaksawan Vervoort <nula_wala@yahoo.com>, 2021
 #
 msgid ""
 msgstr ""
 "Last-Translator: Walaksawan Vervoort <nula_wala@yahoo.com>, 2021\n"
-"Language-Team: Thai (https://www.transifex.com/torchbox/teams/8009/th/)\n"
+"Language-Team: Thai (https://app.transifex.com/torchbox/teams/8009/th/)\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Language: th\n"
 "Plural-Forms: nplurals=1; plural=0;\n"
 
 msgid "Change image"
 msgstr "เปลี่ยนรูปภาพ"
 
@@ -22,17 +22,14 @@
 
 msgid "Choose an image"
 msgstr "เลือกรูปภาพ"
 
 msgid "Delete"
 msgstr "ลบ,ลบทิ้ง"
 
-msgid "Draft"
-msgstr "ร่าง , ข้อความที่เก็บเอาไว้ทำใหม่"
-
 msgid "Edit"
 msgstr "แก้ไข"
 
 msgid "Edit this %s"
 msgstr "แก้ไขสิ่งนี้ %s"
 
 msgid "Edit this document"
@@ -40,17 +37,14 @@
 
 msgid "Edit this image"
 msgstr "แก้ไขรูปภาพนี้"
 
 msgid "Edit this page"
 msgstr "แก้ไขหน้านี้"
 
-msgid "Live"
-msgstr "กำลังแสดงสดอยู่,ถ่ายทอดสด"
-
 msgid "Lock"
 msgstr "ล็อค"
 
 msgid "Preview"
 msgstr "ภาพตัวอย่าง"
 
 msgid "Save"
```

### Comparing `wagtail-localize-1.5/wagtail_localize/locale/tr/LC_MESSAGES/django.mo` & `wagtail-localize-1.5.1/wagtail_localize/locale/tr/LC_MESSAGES/django.mo`

 * *Files 24% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,12 +1,12 @@
 msgid ""
 msgstr ""
 "Report-Msgid-Bugs-To: \n"
 "Last-Translator: Py Data Geek <pydatageek@gmail.com>, 2022\n"
-"Language-Team: Turkish (https://www.transifex.com/torchbox/teams/8009/tr/)\n"
+"Language-Team: Turkish (https://app.transifex.com/torchbox/teams/8009/tr/)\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Language: tr\n"
 "Plural-Forms: nplurals=2; plural=(n > 1);\n"
 
 msgid "Content"
 msgstr "İçerik"
```

### Comparing `wagtail-localize-1.5/wagtail_localize/locale/tr/LC_MESSAGES/django.po` & `wagtail-localize-1.5.1/wagtail_localize/locale/tr/LC_MESSAGES/django.po`

 * *Files 3% similar despite different names*

```diff
@@ -4,17 +4,17 @@
 # Halim Turan <halim_turan_61@hotmail.com>, 2022
 # Ragıp Ünal <ragip@ragipunal.com>, 2022
 # Py Data Geek <pydatageek@gmail.com>, 2022
 #
 msgid ""
 msgstr ""
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2022-10-17 21:00+0000\n"
+"POT-Creation-Date: 2023-02-23 14:15+0000\n"
 "Last-Translator: Py Data Geek <pydatageek@gmail.com>, 2022\n"
-"Language-Team: Turkish (https://www.transifex.com/torchbox/teams/8009/tr/)\n"
+"Language-Team: Turkish (https://app.transifex.com/torchbox/teams/8009/tr/)\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Language: tr\n"
 "Plural-Forms: nplurals=2; plural=(n > 1);\n"
 
 msgid "Saving…"
 msgstr "Kaydediliyor…"
```

### Comparing `wagtail-localize-1.5/wagtail_localize/locale/tr/LC_MESSAGES/djangojs.po` & `wagtail-localize-1.5.1/wagtail_localize/locale/tr/LC_MESSAGES/djangojs.po`

 * *Files 7% similar despite different names*

```diff
@@ -5,25 +5,22 @@
 # Halim Turan <halim_turan_61@hotmail.com>, 2021
 # Basitlik İyidir, 2021
 # Py Data Geek <pydatageek@gmail.com>, 2021
 #
 msgid ""
 msgstr ""
 "Last-Translator: Py Data Geek <pydatageek@gmail.com>, 2021\n"
-"Language-Team: Turkish (https://www.transifex.com/torchbox/teams/8009/tr/)\n"
+"Language-Team: Turkish (https://app.transifex.com/torchbox/teams/8009/tr/)\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Language: tr\n"
 "Plural-Forms: nplurals=2; plural=(n > 1);\n"
 
 msgid "Apply editor lock"
 msgstr "Editör kilidini kaldır"
 
-msgid "Breadcrumb"
-msgstr "İçerik haritası"
-
 msgid "Change image"
 msgstr "Resmi değiştir"
 
 msgid "Choose a document"
 msgstr "Belge seç"
 
 msgid "Choose a page"
@@ -31,17 +28,14 @@
 
 msgid "Choose an image"
 msgstr "Bir resim seç"
 
 msgid "Delete"
 msgstr "Sil"
 
-msgid "Draft"
-msgstr "Taslak"
-
 msgid "Edit"
 msgstr "Düzenle"
 
 msgid "Edit this %s"
 msgstr "%s düzenle"
 
 msgid "Edit this document"
@@ -49,17 +43,14 @@
 
 msgid "Edit this image"
 msgstr "Resmi düzenle"
 
 msgid "Edit this page"
 msgstr "Sayfayı düzenle"
 
-msgid "Live"
-msgstr "Yayında"
-
 msgid "Lock"
 msgstr "Kilitle"
 
 msgid "Preview"
 msgstr "Önizleme"
 
 msgid "Remove editor lock"
```

### Comparing `wagtail-localize-1.5/wagtail_localize/locale/tr_TR/LC_MESSAGES/django.mo` & `wagtail-localize-1.5.1/wagtail_localize/locale/tr_TR/LC_MESSAGES/django.mo`

 * *Files 2% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,12 +1,12 @@
 msgid ""
 msgstr ""
 "Report-Msgid-Bugs-To: \n"
 "Last-Translator: Py Data Geek <pydatageek@gmail.com>, 2022\n"
-"Language-Team: Turkish (Turkey) (https://www.transifex.com/torchbox/"
+"Language-Team: Turkish (Turkey) (https://app.transifex.com/torchbox/"
 "teams/8009/tr_TR/)\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Language: tr_TR\n"
 "Plural-Forms: nplurals=2; plural=(n > 1);\n"
 
 msgid "Content"
 msgstr "İçerik"
```

### Comparing `wagtail-localize-1.5/wagtail_localize/locale/tr_TR/LC_MESSAGES/django.po` & `wagtail-localize-1.5.1/wagtail_localize/locale/tr_TR/LC_MESSAGES/django.po`

 * *Files 15% similar despite different names*

```diff
@@ -4,17 +4,17 @@
 # Halim Turan <halim_turan_61@hotmail.com>, 2022
 # José Luis <alagunajs@gmail.com>, 2022
 # Py Data Geek <pydatageek@gmail.com>, 2022
 #
 msgid ""
 msgstr ""
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2022-10-17 21:00+0000\n"
+"POT-Creation-Date: 2023-02-23 14:15+0000\n"
 "Last-Translator: Py Data Geek <pydatageek@gmail.com>, 2022\n"
-"Language-Team: Turkish (Turkey) (https://www.transifex.com/torchbox/"
+"Language-Team: Turkish (Turkey) (https://app.transifex.com/torchbox/"
 "teams/8009/tr_TR/)\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Language: tr_TR\n"
 "Plural-Forms: nplurals=2; plural=(n > 1);\n"
 
 msgid "Saving…"
 msgstr "Kaydediliyor…"
```

### Comparing `wagtail-localize-1.5/wagtail_localize/locale/tr_TR/LC_MESSAGES/djangojs.mo` & `wagtail-localize-1.5.1/wagtail_localize/locale/et/LC_MESSAGES/djangojs.mo`

 * *Files 27% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,68 +1,58 @@
 msgid ""
 msgstr ""
-"Last-Translator: Py Data Geek <pydatageek@gmail.com>, 2021\n"
-"Language-Team: Turkish (Turkey) (https://www.transifex.com/torchbox/"
-"teams/8009/tr_TR/)\n"
+"Last-Translator: Erlend <debcf78e@opayq.com>, 2021\n"
+"Language-Team: Estonian (https://app.transifex.com/torchbox/teams/8009/et/)\n"
 "Content-Type: text/plain; charset=UTF-8\n"
-"Language: tr_TR\n"
-"Plural-Forms: nplurals=2; plural=(n > 1);\n"
+"Language: et\n"
+"Plural-Forms: nplurals=2; plural=(n != 1);\n"
 
-msgid "Breadcrumb"
-msgstr "İçerik haritası"
+msgid "Apply editor lock"
+msgstr "Rakenda redaktori lukustus"
+
+msgid "Cancel"
+msgstr "Tühista"
 
 msgid "Change image"
-msgstr "Resmi değiştir"
+msgstr "Muuda pilti"
 
 msgid "Choose a document"
-msgstr "Belge seç"
+msgstr "Valige dokument"
 
 msgid "Choose a page"
-msgstr "Bir sayfa seç"
+msgstr "Valige leht"
 
 msgid "Choose an image"
-msgstr "Bir resim seç"
+msgstr "Valige pilt"
 
 msgid "Delete"
-msgstr "Sil"
-
-msgid "Draft"
-msgstr "Taslak"
+msgstr "Kustuta"
 
 msgid "Edit"
-msgstr "Düzenle"
+msgstr "Muuda"
 
 msgid "Edit this %s"
-msgstr "%s düzenle"
+msgstr "Muutke seda %s"
 
 msgid "Edit this document"
-msgstr "Belgeyi düzenle"
+msgstr "Muutke seda dokumenti"
 
 msgid "Edit this image"
-msgstr "Resmi düzenle"
+msgstr "Muutke seda pilti"
 
 msgid "Edit this page"
-msgstr "Sayfayı düzenle"
-
-msgid "Live"
-msgstr "Yayında"
+msgstr "Muutke seda lehte"
 
 msgid "Lock"
-msgstr "Kilitle"
+msgstr "Lukusta"
 
 msgid "Preview"
-msgstr "Önizleme"
-
-msgid "Remove editor lock"
-msgstr "Editör kilidini kaldır"
+msgstr "Eelvaade"
 
 msgid "Save"
-msgstr "Kaydet"
-
-msgid "Saving..."
-msgstr "Kaydediyor..."
+msgstr "Salvesta"
 
 msgid "Unlock"
-msgstr "Kilidi kaldır"
+msgstr "Ava"
 
 msgid "Unpublish"
-msgstr "Yayından Kaldır"
+msgstr "Tühista avaldamine"
```

### Comparing `wagtail-localize-1.5/wagtail_localize/locale/tr_TR/LC_MESSAGES/djangojs.po` & `wagtail-localize-1.5.1/wagtail_localize/locale/tr_TR/LC_MESSAGES/djangojs.po`

 * *Files 5% similar despite different names*

```diff
@@ -4,23 +4,20 @@
 # Ragıp Ünal <ragip@ragipunal.com>, 2021
 # Halim Turan <halim_turan_61@hotmail.com>, 2021
 # Py Data Geek <pydatageek@gmail.com>, 2021
 #
 msgid ""
 msgstr ""
 "Last-Translator: Py Data Geek <pydatageek@gmail.com>, 2021\n"
-"Language-Team: Turkish (Turkey) (https://www.transifex.com/torchbox/"
+"Language-Team: Turkish (Turkey) (https://app.transifex.com/torchbox/"
 "teams/8009/tr_TR/)\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Language: tr_TR\n"
 "Plural-Forms: nplurals=2; plural=(n > 1);\n"
 
-msgid "Breadcrumb"
-msgstr "İçerik haritası"
-
 msgid "Change image"
 msgstr "Resmi değiştir"
 
 msgid "Choose a document"
 msgstr "Belge seç"
 
 msgid "Choose a page"
@@ -28,17 +25,14 @@
 
 msgid "Choose an image"
 msgstr "Bir resim seç"
 
 msgid "Delete"
 msgstr "Sil"
 
-msgid "Draft"
-msgstr "Taslak"
-
 msgid "Edit"
 msgstr "Düzenle"
 
 msgid "Edit this %s"
 msgstr "%s düzenle"
 
 msgid "Edit this document"
@@ -46,17 +40,14 @@
 
 msgid "Edit this image"
 msgstr "Resmi düzenle"
 
 msgid "Edit this page"
 msgstr "Sayfayı düzenle"
 
-msgid "Live"
-msgstr "Yayında"
-
 msgid "Lock"
 msgstr "Kilitle"
 
 msgid "Preview"
 msgstr "Önizleme"
 
 msgid "Remove editor lock"
```

### Comparing `wagtail-localize-1.5/wagtail_localize/locale/uk/LC_MESSAGES/django.mo` & `wagtail-localize-1.5.1/wagtail_localize/locale/uk/LC_MESSAGES/django.mo`

 * *Files 0% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,12 +1,12 @@
 msgid ""
 msgstr ""
 "Report-Msgid-Bugs-To: \n"
 "Last-Translator: Sergiy Shkodenko <shkodenkosergiy@gmail.com>, 2022\n"
-"Language-Team: Ukrainian (https://www.transifex.com/torchbox/teams/8009/"
+"Language-Team: Ukrainian (https://app.transifex.com/torchbox/teams/8009/"
 "uk/)\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Language: uk\n"
 "Plural-Forms: nplurals=4; plural=(n % 1 == 0 && n % 10 == 1 && n % 100 != "
 "11 ? 0 : n % 1 == 0 && n % 10 >= 2 && n % 10 <= 4 && (n % 100 < 12 || n % "
 "100 > 14) ? 1 : n % 1 == 0 && (n % 10 ==0 || (n % 10 >=5 && n % 10 <=9) || "
 "(n % 100 >=11 && n % 100 <=14 )) ? 2: 3);\n"
```

### Comparing `wagtail-localize-1.5/wagtail_localize/locale/uk/LC_MESSAGES/django.po` & `wagtail-localize-1.5.1/wagtail_localize/locale/uk/LC_MESSAGES/django.po`

 * *Files 0% similar despite different names*

```diff
@@ -4,17 +4,17 @@
 # Anastasiia La, 2021
 # d55ee35323c0c760f088259cd23b1b6d_9e8a7d1 <5459f3ae99ecdd5ed0be0220acd46004_1019581>, 2022
 # Sergiy Shkodenko <shkodenkosergiy@gmail.com>, 2022
 #
 msgid ""
 msgstr ""
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2022-10-17 21:00+0000\n"
+"POT-Creation-Date: 2023-02-23 14:15+0000\n"
 "Last-Translator: Sergiy Shkodenko <shkodenkosergiy@gmail.com>, 2022\n"
-"Language-Team: Ukrainian (https://www.transifex.com/torchbox/teams/8009/"
+"Language-Team: Ukrainian (https://app.transifex.com/torchbox/teams/8009/"
 "uk/)\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Language: uk\n"
 "Plural-Forms: nplurals=4; plural=(n % 1 == 0 && n % 10 == 1 && n % 100 != "
 "11 ? 0 : n % 1 == 0 && n % 10 >= 2 && n % 10 <= 4 && (n % 100 < 12 || n % "
 "100 > 14) ? 1 : n % 1 == 0 && (n % 10 ==0 || (n % 10 >=5 && n % 10 <=9) || "
 "(n % 100 >=11 && n % 100 <=14 )) ? 2: 3);\n"
```

### Comparing `wagtail-localize-1.5/wagtail_localize/locale/uk/LC_MESSAGES/djangojs.mo` & `wagtail-localize-1.5.1/wagtail_localize/locale/uk/LC_MESSAGES/djangojs.mo`

 * *Files 14% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,25 +1,22 @@
 msgid ""
 msgstr ""
 "Last-Translator: Anastasiia La, 2021\n"
-"Language-Team: Ukrainian (https://www.transifex.com/torchbox/teams/8009/"
+"Language-Team: Ukrainian (https://app.transifex.com/torchbox/teams/8009/"
 "uk/)\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Language: uk\n"
 "Plural-Forms: nplurals=4; plural=(n % 1 == 0 && n % 10 == 1 && n % 100 != "
 "11 ? 0 : n % 1 == 0 && n % 10 >= 2 && n % 10 <= 4 && (n % 100 < 12 || n % "
 "100 > 14) ? 1 : n % 1 == 0 && (n % 10 ==0 || (n % 10 >=5 && n % 10 <=9) || "
 "(n % 100 >=11 && n % 100 <=14 )) ? 2: 3);\n"
 
 msgid "Apply editor lock"
 msgstr "Застосувати редакторське блокування"
 
-msgid "Breadcrumb"
-msgstr "Ланцюжок навігації"
-
 msgid "Cancel"
 msgstr "Скасувати"
 
 msgid "Change %s"
 msgstr "Змінено %s"
 
 msgid "Change document"
@@ -51,17 +48,14 @@
 
 msgid "Download PO file"
 msgstr "Завантажити PO-файл"
 
 msgid "Download PO file and input translations offline"
 msgstr "Завантажити PO-файл і ввести переклад офлайн"
 
-msgid "Draft"
-msgstr "Чернетка"
-
 msgid "Edit"
 msgstr "Редагувати"
 
 msgid "Edit this %s"
 msgstr "Редагувати %s"
 
 msgid "Edit this document"
@@ -81,35 +75,26 @@
 
 msgid "Fetching image information..."
 msgstr "Вилучення інформації про зображення"
 
 msgid "Fetching page information..."
 msgstr "Виручення інформації про сторінку"
 
-msgid "Live"
-msgstr "Наживо"
-
 msgid "Lock"
 msgstr "Блокувати"
 
 msgid "Not translated"
 msgstr "Не перекладено"
 
 msgid "Preview"
 msgstr "Попередній перегляд"
 
 msgid "Publish in "
 msgstr "Опублікувати в"
 
-msgid "Published"
-msgstr "Опубліковано"
-
-msgid "Published on "
-msgstr "Опублікувати на"
-
 msgid "Publishing..."
 msgstr "Публікація..."
 
 msgid "Remove editor lock"
 msgstr "Зняти блокування редактора"
 
 msgid "Revert to %s version"
```

### Comparing `wagtail-localize-1.5/wagtail_localize/locale/uk/LC_MESSAGES/djangojs.po` & `wagtail-localize-1.5.1/wagtail_localize/locale/uk/LC_MESSAGES/djangojs.po`

 * *Files 4% similar despite different names*

```diff
@@ -6,32 +6,29 @@
 # Sergiy Shkodenko <shkodenkosergiy@gmail.com>, 2021
 # d55ee35323c0c760f088259cd23b1b6d_9e8a7d1 <5459f3ae99ecdd5ed0be0220acd46004_1019581>, 2021
 # Anastasiia La, 2021
 #
 msgid ""
 msgstr ""
 "Last-Translator: Anastasiia La, 2021\n"
-"Language-Team: Ukrainian (https://www.transifex.com/torchbox/teams/8009/"
+"Language-Team: Ukrainian (https://app.transifex.com/torchbox/teams/8009/"
 "uk/)\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Language: uk\n"
 "Plural-Forms: nplurals=4; plural=(n % 1 == 0 && n % 10 == 1 && n % 100 != "
 "11 ? 0 : n % 1 == 0 && n % 10 >= 2 && n % 10 <= 4 && (n % 100 < 12 || n % "
 "100 > 14) ? 1 : n % 1 == 0 && (n % 10 ==0 || (n % 10 >=5 && n % 10 <=9) || "
 "(n % 100 >=11 && n % 100 <=14 )) ? 2: 3);\n"
 
 msgid "[DELETED]"
 msgstr "[Видалено]"
 
 msgid "Apply editor lock"
 msgstr "Застосувати редакторське блокування"
 
-msgid "Breadcrumb"
-msgstr "Ланцюжок навігації"
-
 msgid "Cancel"
 msgstr "Скасувати"
 
 msgid "Change %s"
 msgstr "Змінено %s"
 
 msgid "Change document"
@@ -63,17 +60,14 @@
 
 msgid "Download PO file"
 msgstr "Завантажити PO-файл"
 
 msgid "Download PO file and input translations offline"
 msgstr "Завантажити PO-файл і ввести переклад офлайн"
 
-msgid "Draft"
-msgstr "Чернетка"
-
 msgid "Edit"
 msgstr "Редагувати"
 
 msgid "Edit this %s"
 msgstr "Редагувати %s"
 
 msgid "Edit this document"
@@ -93,35 +87,26 @@
 
 msgid "Fetching image information..."
 msgstr "Вилучення інформації про зображення"
 
 msgid "Fetching page information..."
 msgstr "Виручення інформації про сторінку"
 
-msgid "Live"
-msgstr "Наживо"
-
 msgid "Lock"
 msgstr "Блокувати"
 
 msgid "Not translated"
 msgstr "Не перекладено"
 
 msgid "Preview"
 msgstr "Попередній перегляд"
 
 msgid "Publish in "
 msgstr "Опублікувати в"
 
-msgid "Published"
-msgstr "Опубліковано"
-
-msgid "Published on "
-msgstr "Опублікувати на"
-
 msgid "Publishing..."
 msgstr "Публікація..."
 
 msgid "Remove editor lock"
 msgstr "Зняти блокування редактора"
 
 msgid "Revert to %s version"
```

### Comparing `wagtail-localize-1.5/wagtail_localize/locale/vi/LC_MESSAGES/django.mo` & `wagtail-localize-1.5.1/wagtail_localize/locale/vi/LC_MESSAGES/django.mo`

 * *Files 1% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,12 +1,12 @@
 msgid ""
 msgstr ""
 "Report-Msgid-Bugs-To: \n"
 "Last-Translator: Duc Huynh <duchuynhthoai@gmail.com>, 2022\n"
-"Language-Team: Vietnamese (https://www.transifex.com/torchbox/teams/8009/"
+"Language-Team: Vietnamese (https://app.transifex.com/torchbox/teams/8009/"
 "vi/)\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Language: vi\n"
 "Plural-Forms: nplurals=1; plural=0;\n"
 
 msgid "Delete"
 msgstr "Xoá"
```

### Comparing `wagtail-localize-1.5/wagtail_localize/locale/vi/LC_MESSAGES/django.po` & `wagtail-localize-1.5.1/wagtail_localize/locale/vi/LC_MESSAGES/django.po`

 * *Files 12% similar despite different names*

```diff
@@ -4,17 +4,17 @@
 # Vu Pham, 2022
 # Luan Nguyen <lihavim@gmail.com>, 2022
 # Duc Huynh <duchuynhthoai@gmail.com>, 2022
 #
 msgid ""
 msgstr ""
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2022-10-17 21:00+0000\n"
+"POT-Creation-Date: 2023-02-23 14:15+0000\n"
 "Last-Translator: Duc Huynh <duchuynhthoai@gmail.com>, 2022\n"
-"Language-Team: Vietnamese (https://www.transifex.com/torchbox/teams/8009/"
+"Language-Team: Vietnamese (https://app.transifex.com/torchbox/teams/8009/"
 "vi/)\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Language: vi\n"
 "Plural-Forms: nplurals=1; plural=0;\n"
 
 msgid "Translate"
 msgstr "Dịch"
```

### Comparing `wagtail-localize-1.5/wagtail_localize/locale/vi/LC_MESSAGES/djangojs.po` & `wagtail-localize-1.5.1/wagtail_localize/locale/vi/LC_MESSAGES/djangojs.po`

 * *Files 4% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 # Hồng Quân Nguyễn <ng.hong.quan@gmail.com>, 2021
 # Luan Nguyen <lihavim@gmail.com>, 2021
 # Vu Pham, 2022
 #
 msgid ""
 msgstr ""
 "Last-Translator: Vu Pham, 2022\n"
-"Language-Team: Vietnamese (https://www.transifex.com/torchbox/teams/8009/"
+"Language-Team: Vietnamese (https://app.transifex.com/torchbox/teams/8009/"
 "vi/)\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Language: vi\n"
 "Plural-Forms: nplurals=1; plural=0;\n"
 
 msgid "[DELETED]"
 msgstr "[ĐÃ XÓA]"
@@ -45,17 +45,14 @@
 
 msgid "Choose an image"
 msgstr "Chọn một hình ảnh"
 
 msgid "Delete"
 msgstr "Xoá"
 
-msgid "Draft"
-msgstr "Bản nháp"
-
 msgid "Edit"
 msgstr "Biên tập"
 
 msgid "Edit this %s"
 msgstr "Biên tập %s này"
 
 msgid "Edit this document"
@@ -63,20 +60,14 @@
 
 msgid "Lock"
 msgstr "Khóa"
 
 msgid "Preview"
 msgstr "Xem trước"
 
-msgid "Published"
-msgstr "Đã xuất bản"
-
-msgid "Published on "
-msgstr "Xuất bản vào"
-
 msgid "Publishing..."
 msgstr "Đang xuất bản..."
 
 msgid "Save"
 msgstr "Lưu"
 
 msgid "Saving..."
```

### Comparing `wagtail-localize-1.5/wagtail_localize/locale/zh/LC_MESSAGES/django.po` & `wagtail-localize-1.5.1/wagtail_localize/locale/zh/LC_MESSAGES/django.po`

 * *Files 18% similar despite different names*

```diff
@@ -4,17 +4,17 @@
 # Orangle Liu <orangleliu@gmail.com>, 2022
 # Karl Hobley <karl@torchbox.com>, 2022
 # Matt Westcott <matthew@torchbox.com>, 2022
 #
 msgid ""
 msgstr ""
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2022-10-17 21:00+0000\n"
+"POT-Creation-Date: 2023-02-23 14:15+0000\n"
 "Last-Translator: Matt Westcott <matthew@torchbox.com>, 2022\n"
-"Language-Team: Chinese (https://www.transifex.com/torchbox/teams/8009/zh/)\n"
+"Language-Team: Chinese (https://app.transifex.com/torchbox/teams/8009/zh/)\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Language: zh\n"
 "Plural-Forms: nplurals=1; plural=0;\n"
 
 msgid "Saving…"
 msgstr "正在保存"
```

### Comparing `wagtail-localize-1.5/wagtail_localize/locale/zh/LC_MESSAGES/djangojs.po` & `wagtail-localize-1.5.1/wagtail_localize/locale/zh/LC_MESSAGES/djangojs.po`

 * *Files 12% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 # serafeim <serafeim@torchbox.com>, 2021
 # Karl Hobley <karl@torchbox.com>, 2021
 # shengsheng gz <gzshengsheng@139.com>, 2021
 #
 msgid ""
 msgstr ""
 "Last-Translator: shengsheng gz <gzshengsheng@139.com>, 2021\n"
-"Language-Team: Chinese (https://www.transifex.com/torchbox/teams/8009/zh/)\n"
+"Language-Team: Chinese (https://app.transifex.com/torchbox/teams/8009/zh/)\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Language: zh\n"
 "Plural-Forms: nplurals=1; plural=0;\n"
 
 msgid "Choose a document"
 msgstr "选择一个文档"
 
@@ -22,17 +22,14 @@
 
 msgid "Choose an image"
 msgstr "选择一个图片"
 
 msgid "Delete"
 msgstr "删除"
 
-msgid "Draft"
-msgstr "草稿"
-
 msgid "Edit"
 msgstr "编辑"
 
 msgid "Edit this page"
 msgstr "编辑这个页面"
 
 msgid "Preview"
```

### Comparing `wagtail-localize-1.5/wagtail_localize/locale/zh_Hans/LC_MESSAGES/django.mo` & `wagtail-localize-1.5.1/wagtail_localize/locale/zh_Hans/LC_MESSAGES/django.mo`

 * *Files 1% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,12 +1,12 @@
 msgid ""
 msgstr ""
 "Report-Msgid-Bugs-To: \n"
 "Last-Translator: Ford Guo <agile.guo@gmail.com>, 2023\n"
-"Language-Team: Chinese (China) (https://www.transifex.com/torchbox/"
+"Language-Team: Chinese (China) (https://app.transifex.com/torchbox/"
 "teams/8009/zh_CN/)\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Language: zh_CN\n"
 "Plural-Forms: nplurals=1; plural=0;\n"
 
 msgid ""
 "<{}> tag is not allowed. Strings can only contain standard HTML inline tags "
```

### Comparing `wagtail-localize-1.5/wagtail_localize/locale/zh_Hans/LC_MESSAGES/django.po` & `wagtail-localize-1.5.1/wagtail_localize/locale/zh_Hans/LC_MESSAGES/django.po`

 * *Files 1% similar despite different names*

```diff
@@ -6,17 +6,17 @@
 # Yin Guanhao <sopium@mysterious.site>, 2022
 # Vincent Zhao <zhaopu2008@gmail.com>, 2022
 # Ford Guo <agile.guo@gmail.com>, 2023
 #
 msgid ""
 msgstr ""
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2022-10-17 21:00+0000\n"
+"POT-Creation-Date: 2023-02-23 14:15+0000\n"
 "Last-Translator: Ford Guo <agile.guo@gmail.com>, 2023\n"
-"Language-Team: Chinese (China) (https://www.transifex.com/torchbox/"
+"Language-Team: Chinese (China) (https://app.transifex.com/torchbox/"
 "teams/8009/zh_CN/)\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Language: zh_CN\n"
 "Plural-Forms: nplurals=1; plural=0;\n"
 
 msgid "Disable"
 msgstr "禁用"
```

### Comparing `wagtail-localize-1.5/wagtail_localize/locale/zh_Hans/LC_MESSAGES/djangojs.po` & `wagtail-localize-1.5.1/wagtail_localize/locale/zh_Hans/LC_MESSAGES/djangojs.po`

 * *Files 9% similar despite different names*

```diff
@@ -5,29 +5,26 @@
 # Favo Yang <favoyang@gmail.com>, 2021
 # 汇民 王 <whuim@qq.com>, 2021
 # Ford Guo <agile.guo@gmail.com>, 2023
 #
 msgid ""
 msgstr ""
 "Last-Translator: Ford Guo <agile.guo@gmail.com>, 2023\n"
-"Language-Team: Chinese (China) (https://www.transifex.com/torchbox/"
+"Language-Team: Chinese (China) (https://app.transifex.com/torchbox/"
 "teams/8009/zh_CN/)\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Language: zh_CN\n"
 "Plural-Forms: nplurals=1; plural=0;\n"
 
 msgid "[DELETED]"
 msgstr "[已删除]"
 
 msgid "Apply editor lock"
 msgstr "应用锁编辑"
 
-msgid "Breadcrumb"
-msgstr "面包屑"
-
 msgid "Cancel"
 msgstr "取消"
 
 msgid "Change %s"
 msgstr "更改 %s"
 
 msgid "Change document"
@@ -62,17 +59,14 @@
 
 msgid "Download PO file"
 msgstr "下载 PO 文件"
 
 msgid "Download PO file and input translations offline"
 msgstr "下载 PO 文件并且线下翻译"
 
-msgid "Draft"
-msgstr "草稿"
-
 msgid "Edit"
 msgstr "编辑"
 
 msgid "Edit this %s"
 msgstr "编辑这个 %s"
 
 msgid "Edit this document"
@@ -92,35 +86,26 @@
 
 msgid "Fetching image information..."
 msgstr "正在获取图片信息..."
 
 msgid "Fetching page information..."
 msgstr "正在获取页面信息..."
 
-msgid "Live"
-msgstr "发布"
-
 msgid "Lock"
 msgstr "锁定"
 
 msgid "Not translated"
 msgstr "未翻译"
 
 msgid "Preview"
 msgstr "预览"
 
 msgid "Publish in "
 msgstr "发布在"
 
-msgid "Published"
-msgstr "已发布"
-
-msgid "Published on "
-msgstr "发布在"
-
 msgid "Publishing..."
 msgstr "正在发布……"
 
 msgid "Remove editor lock"
 msgstr "移除编辑锁定"
 
 msgid "Revert to %s version"
```

### Comparing `wagtail-localize-1.5/wagtail_localize/locale/zh_Hant/LC_MESSAGES/django.mo` & `wagtail-localize-1.5.1/wagtail_localize/locale/zh_Hant/LC_MESSAGES/django.mo`

 * *Files 16% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,12 +1,12 @@
 msgid ""
 msgstr ""
 "Report-Msgid-Bugs-To: \n"
 "Last-Translator: Chih Wang <ihcgno@icloud.com>, 2022\n"
-"Language-Team: Chinese Traditional (https://www.transifex.com/torchbox/"
+"Language-Team: Chinese Traditional (https://app.transifex.com/torchbox/"
 "teams/8009/zh-Hant/)\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Language: zh-Hant\n"
 "Plural-Forms: nplurals=1; plural=0;\n"
 
 msgid "Content"
 msgstr "內容"
```

### Comparing `wagtail-localize-1.5/wagtail_localize/locale/zh_Hant/LC_MESSAGES/django.po` & `wagtail-localize-1.5.1/wagtail_localize/locale/zh_Hant/LC_MESSAGES/django.po`

 * *Files 14% similar despite different names*

```diff
@@ -2,17 +2,17 @@
 # Translators:
 # Yeh Yen-Ke <yyken@outlook.com>, 2022
 # Chih Wang <ihcgno@icloud.com>, 2022
 #
 msgid ""
 msgstr ""
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2022-10-17 21:00+0000\n"
+"POT-Creation-Date: 2023-02-23 14:15+0000\n"
 "Last-Translator: Chih Wang <ihcgno@icloud.com>, 2022\n"
-"Language-Team: Chinese Traditional (https://www.transifex.com/torchbox/"
+"Language-Team: Chinese Traditional (https://app.transifex.com/torchbox/"
 "teams/8009/zh-Hant/)\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Language: zh-Hant\n"
 "Plural-Forms: nplurals=1; plural=0;\n"
 
 msgid "Disable"
 msgstr "禁用"
```

### Comparing `wagtail-localize-1.5/wagtail_localize/locale/zh_Hant/LC_MESSAGES/djangojs.mo` & `wagtail-localize-1.5.1/wagtail_localize/locale/zh_Hant/LC_MESSAGES/djangojs.mo`

 * *Files 24% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,11 +1,11 @@
 msgid ""
 msgstr ""
 "Last-Translator: Chih Wang <ihcgno@icloud.com>, 2021\n"
-"Language-Team: Chinese Traditional (https://www.transifex.com/torchbox/"
+"Language-Team: Chinese Traditional (https://app.transifex.com/torchbox/"
 "teams/8009/zh-Hant/)\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Language: zh-Hant\n"
 "Plural-Forms: nplurals=1; plural=0;\n"
 
 msgid "Apply editor lock"
 msgstr "套用編輯鎖定"
@@ -24,17 +24,14 @@
 
 msgid "Choose an image"
 msgstr "選擇一個圖片"
 
 msgid "Delete"
 msgstr "刪除"
 
-msgid "Draft"
-msgstr "草稿"
-
 msgid "Edit"
 msgstr "編輯"
 
 msgid "Edit this %s"
 msgstr "編輯此 %s"
 
 msgid "Edit this document"
@@ -42,26 +39,20 @@
 
 msgid "Edit this image"
 msgstr "編輯此圖片"
 
 msgid "Edit this page"
 msgstr "編輯此頁面"
 
-msgid "Live"
-msgstr "上線"
-
 msgid "Lock"
 msgstr "鎖定"
 
 msgid "Preview"
 msgstr "預覽"
 
-msgid "Published"
-msgstr "已發佈"
-
 msgid "Save"
 msgstr "儲存"
 
 msgid "Saving..."
 msgstr "儲存中..."
 
 msgid "Unlock"
```

### Comparing `wagtail-localize-1.5/wagtail_localize/locale/zh_Hant/LC_MESSAGES/djangojs.po` & `wagtail-localize-1.5.1/wagtail_localize/locale/zh_Hant/LC_MESSAGES/djangojs.po`

 * *Files 4% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 # Andy Kong <worminfo@gmail.com>, 2021
 # Yeh Yen-Ke <yyken@outlook.com>, 2021
 # Chih Wang <ihcgno@icloud.com>, 2021
 #
 msgid ""
 msgstr ""
 "Last-Translator: Chih Wang <ihcgno@icloud.com>, 2021\n"
-"Language-Team: Chinese Traditional (https://www.transifex.com/torchbox/"
+"Language-Team: Chinese Traditional (https://app.transifex.com/torchbox/"
 "teams/8009/zh-Hant/)\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Language: zh-Hant\n"
 "Plural-Forms: nplurals=1; plural=0;\n"
 
 msgid "Apply editor lock"
 msgstr "套用編輯鎖定"
@@ -31,17 +31,14 @@
 
 msgid "Choose an image"
 msgstr "選擇一個圖片"
 
 msgid "Delete"
 msgstr "刪除"
 
-msgid "Draft"
-msgstr "草稿"
-
 msgid "Edit"
 msgstr "編輯"
 
 msgid "Edit this %s"
 msgstr "編輯此 %s"
 
 msgid "Edit this document"
@@ -49,26 +46,20 @@
 
 msgid "Edit this image"
 msgstr "編輯此圖片"
 
 msgid "Edit this page"
 msgstr "編輯此頁面"
 
-msgid "Live"
-msgstr "上線"
-
 msgid "Lock"
 msgstr "鎖定"
 
 msgid "Preview"
 msgstr "預覽"
 
-msgid "Published"
-msgstr "已發佈"
-
 msgid "Save"
 msgstr "儲存"
 
 msgid "Saving..."
 msgstr "儲存中..."
 
 msgid "Unlock"
```

### Comparing `wagtail-localize-1.5/wagtail_localize/locales/components.py` & `wagtail-localize-1.5.1/wagtail_localize/locales/components.py`

 * *Files identical despite different names*

### Comparing `wagtail-localize-1.5/wagtail_localize/locales/forms.py` & `wagtail-localize-1.5.1/wagtail_localize/locales/forms.py`

 * *Files identical despite different names*

### Comparing `wagtail-localize-1.5/wagtail_localize/locales/locale/en/LC_MESSAGES/django.po` & `wagtail-localize-1.5.1/wagtail_localize/locales/locale/en/LC_MESSAGES/django.po`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 # FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
 #
 #, fuzzy
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2023-02-23 14:15+0000\n"
+"POT-Creation-Date: 2023-06-11 10:34+0000\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language-Team: LANGUAGE <LL@li.org>\n"
 "Language: \n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
@@ -54,51 +54,51 @@
 msgid "Usage"
 msgstr ""
 
 #: locales/templates/wagtaillocales/index.html:31
 msgid "This locale's language code is not supported"
 msgstr ""
 
-#: locales/views.py:77 locales/wagtail_hooks.py:26
+#: locales/views.py:76 locales/wagtail_hooks.py:26
 msgid "Locales"
 msgstr ""
 
-#: locales/views.py:78
+#: locales/views.py:77
 msgid "Add a locale"
 msgstr ""
 
-#: locales/views.py:92
+#: locales/views.py:91
 msgid "Add locale"
 msgstr ""
 
-#: locales/views.py:93
+#: locales/views.py:92
 #, python-brace-format
 msgid "Locale '{0}' created."
 msgstr ""
 
-#: locales/views.py:127
+#: locales/views.py:126
 #, python-brace-format
 msgid "Locale '{0}' updated."
 msgstr ""
 
-#: locales/views.py:128
+#: locales/views.py:127
 msgid "The locale could not be saved due to errors."
 msgstr ""
 
-#: locales/views.py:129 locales/views.py:171
+#: locales/views.py:128 locales/views.py:170
 msgid "Delete locale"
 msgstr ""
 
-#: locales/views.py:167
+#: locales/views.py:166
 #, python-brace-format
 msgid "Locale '{0}' deleted."
 msgstr ""
 
-#: locales/views.py:169
+#: locales/views.py:168
 msgid ""
 "This locale cannot be deleted because there are pages and/or other objects "
 "using it."
 msgstr ""
 
-#: locales/views.py:172
+#: locales/views.py:171
 msgid "Are you sure you want to delete this locale?"
 msgstr ""
```

### Comparing `wagtail-localize-1.5/wagtail_localize/locales/locale/es/LC_MESSAGES/django.mo` & `wagtail-localize-1.5.1/wagtail_localize/locales/locale/es/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `wagtail-localize-1.5/wagtail_localize/locales/locale/fi/LC_MESSAGES/django.mo` & `wagtail-localize-1.5.1/wagtail_localize/locales/locale/fi/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `wagtail-localize-1.5/wagtail_localize/locales/locale/fr/LC_MESSAGES/django.mo` & `wagtail-localize-1.5.1/wagtail_localize/locales/locale/fr/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `wagtail-localize-1.5/wagtail_localize/locales/locale/hr_HR/LC_MESSAGES/django.mo` & `wagtail-localize-1.5.1/wagtail_localize/locales/locale/hr_HR/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `wagtail-localize-1.5/wagtail_localize/locales/locale/is_IS/LC_MESSAGES/django.mo` & `wagtail-localize-1.5.1/wagtail_localize/locales/locale/is_IS/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `wagtail-localize-1.5/wagtail_localize/locales/locale/nl_NL/LC_MESSAGES/django.mo` & `wagtail-localize-1.5.1/wagtail_localize/locales/locale/nl_NL/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `wagtail-localize-1.5/wagtail_localize/locales/locale/pt_PT/LC_MESSAGES/django.mo` & `wagtail-localize-1.5.1/wagtail_localize/locales/locale/pt_PT/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `wagtail-localize-1.5/wagtail_localize/locales/locale/ru/LC_MESSAGES/django.mo` & `wagtail-localize-1.5.1/wagtail_localize/locales/locale/ru/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `wagtail-localize-1.5/wagtail_localize/locales/locale/sv/LC_MESSAGES/django.mo` & `wagtail-localize-1.5.1/wagtail_localize/locales/locale/sv/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `wagtail-localize-1.5/wagtail_localize/locales/locale/zh_Hans/LC_MESSAGES/django.mo` & `wagtail-localize-1.5.1/wagtail_localize/locales/locale/zh_Hans/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `wagtail-localize-1.5/wagtail_localize/locales/locale/zh_Hant/LC_MESSAGES/django.mo` & `wagtail-localize-1.5.1/wagtail_localize/locales/locale/zh_Hant/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `wagtail-localize-1.5/wagtail_localize/locales/templates/wagtaillocales/confirm_delete.html` & `wagtail-localize-1.5.1/wagtail_localize/locales/templates/wagtaillocales/confirm_delete.html`

 * *Files identical despite different names*

### Comparing `wagtail-localize-1.5/wagtail_localize/locales/templates/wagtaillocales/edit.html` & `wagtail-localize-1.5.1/wagtail_localize/locales/templates/wagtaillocales/edit.html`

 * *Files identical despite different names*

### Comparing `wagtail-localize-1.5/wagtail_localize/locales/templates/wagtaillocales/index.html` & `wagtail-localize-1.5.1/wagtail_localize/locales/templates/wagtaillocales/index.html`

 * *Files identical despite different names*

### Comparing `wagtail-localize-1.5/wagtail_localize/locales/tests.py` & `wagtail-localize-1.5.1/wagtail_localize/locales/tests.py`

 * *Files identical despite different names*

### Comparing `wagtail-localize-1.5/wagtail_localize/locales/views.py` & `wagtail-localize-1.5.1/wagtail_localize/locales/views.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 import functools
 
 from django.core.exceptions import ValidationError
 from django.db import transaction
 from django.utils.translation import gettext_lazy
-from wagtail import VERSION as WAGTAIL_VERSION
 from wagtail.admin import messages
 from wagtail.admin.panels import ObjectList, extract_panel_definitions_from_model_class
 from wagtail.admin.views import generic
 from wagtail.admin.viewsets.model import ModelViewSet
 from wagtail.models import Locale
 from wagtail.permissions import locale_permission_policy
 
@@ -177,31 +176,20 @@
         return get_locale_usage(locale) == (0, 0)
 
     def get_context_data(self, object=None):
         context = super().get_context_data()
         context["can_delete"] = self.can_delete(object)
         return context
 
-    if WAGTAIL_VERSION >= (2, 16):
-
-        def form_valid(self, form):
-            if self.can_delete(self.get_object()):
-                return super().form_valid(form)
-            else:
-                messages.error(self.request, self.cannot_delete_message)
-                return super().get(self.request)
-
-    else:
-
-        def delete(self, request, *args, **kwargs):
-            if self.can_delete(self.get_object()):
-                return super().delete(request, *args, **kwargs)
-            else:
-                messages.error(request, self.cannot_delete_message)
-                return super().get(request)
+    def form_valid(self, form):
+        if self.can_delete(self.get_object()):
+            return super().form_valid(form)
+        else:
+            messages.error(self.request, self.cannot_delete_message)
+            return super().get(self.request)
 
 
 class LocaleViewSet(ModelViewSet):
     icon = "site"
     model = Locale
     permission_policy = locale_permission_policy
```

### Comparing `wagtail-localize-1.5/wagtail_localize/locales/wagtail_hooks.py` & `wagtail-localize-1.5.1/wagtail_localize/locales/wagtail_hooks.py`

 * *Files identical despite different names*

### Comparing `wagtail-localize-1.5/wagtail_localize/machine_translators/deepl.py` & `wagtail-localize-1.5.1/wagtail_localize/machine_translators/deepl.py`

 * *Files identical despite different names*

### Comparing `wagtail-localize-1.5/wagtail_localize/machine_translators/dummy.py` & `wagtail-localize-1.5.1/wagtail_localize/machine_translators/dummy.py`

 * *Files identical despite different names*

### Comparing `wagtail-localize-1.5/wagtail_localize/machine_translators/google.py` & `wagtail-localize-1.5.1/wagtail_localize/machine_translators/google.py`

 * *Files identical despite different names*

### Comparing `wagtail-localize-1.5/wagtail_localize/management/commands/sync_locale_trees.py` & `wagtail-localize-1.5.1/wagtail_localize/management/commands/sync_locale_trees.py`

 * *Files identical despite different names*

### Comparing `wagtail-localize-1.5/wagtail_localize/migrations/0001_initial.py` & `wagtail-localize-1.5.1/wagtail_localize/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `wagtail-localize-1.5/wagtail_localize/migrations/0002_translation.py` & `wagtail-localize-1.5.1/wagtail_localize/migrations/0002_translation.py`

 * *Files identical despite different names*

### Comparing `wagtail-localize-1.5/wagtail_localize/migrations/0003_delete_translation_sources.py` & `wagtail-localize-1.5.1/wagtail_localize/migrations/0003_delete_translation_sources.py`

 * *Files identical despite different names*

### Comparing `wagtail-localize-1.5/wagtail_localize/migrations/0004_one_source_per_objectlocale.py` & `wagtail-localize-1.5.1/wagtail_localize/migrations/0004_one_source_per_objectlocale.py`

 * *Files identical despite different names*

### Comparing `wagtail-localize-1.5/wagtail_localize/migrations/0005_remove_translationsource_object.py` & `wagtail-localize-1.5.1/wagtail_localize/migrations/0005_remove_translationsource_object.py`

 * *Files identical despite different names*

### Comparing `wagtail-localize-1.5/wagtail_localize/migrations/0006_create_submit_translation_permission.py` & `wagtail-localize-1.5.1/wagtail_localize/migrations/0006_create_submit_translation_permission.py`

 * *Files identical despite different names*

### Comparing `wagtail-localize-1.5/wagtail_localize/migrations/0007_stringtranslation_type_and_tool_name.py` & `wagtail-localize-1.5.1/wagtail_localize/migrations/0007_stringtranslation_type_and_tool_name.py`

 * *Files identical despite different names*

### Comparing `wagtail-localize-1.5/wagtail_localize/migrations/0008_stringtranslation_last_translated_by.py` & `wagtail-localize-1.5.1/wagtail_localize/migrations/0008_stringtranslation_last_translated_by.py`

 * *Files identical despite different names*

### Comparing `wagtail-localize-1.5/wagtail_localize/migrations/0009_stringtranslation_errors.py` & `wagtail-localize-1.5.1/wagtail_localize/migrations/0009_stringtranslation_errors.py`

 * *Files identical despite different names*

### Comparing `wagtail-localize-1.5/wagtail_localize/migrations/0010_overridablesegment.py` & `wagtail-localize-1.5.1/wagtail_localize/migrations/0010_overridablesegment.py`

 * *Files identical despite different names*

### Comparing `wagtail-localize-1.5/wagtail_localize/migrations/0011_segmentoverride.py` & `wagtail-localize-1.5.1/wagtail_localize/migrations/0011_segmentoverride.py`

 * *Files identical despite different names*

### Comparing `wagtail-localize-1.5/wagtail_localize/migrations/0012_localesynchronization.py` & `wagtail-localize-1.5.1/wagtail_localize/migrations/0012_localesynchronization.py`

 * *Files identical despite different names*

### Comparing `wagtail-localize-1.5/wagtail_localize/modeladmin/helpers.py` & `wagtail-localize-1.5.1/wagtail_localize/modeladmin/helpers.py`

 * *Files identical despite different names*

### Comparing `wagtail-localize-1.5/wagtail_localize/modeladmin/options.py` & `wagtail-localize-1.5.1/wagtail_localize/modeladmin/options.py`

 * *Files identical despite different names*

### Comparing `wagtail-localize-1.5/wagtail_localize/modeladmin/templates/wagtail_localize/modeladmin/translatable_edit.html` & `wagtail-localize-1.5.1/wagtail_localize/modeladmin/templates/wagtail_localize/modeladmin/translatable_edit.html`

 * *Files 16% similar despite different names*

```diff
@@ -3,15 +3,16 @@
 
 {% block header %}
     {% include "modeladmin/includes/header_with_history.html" with title=view.get_page_title subtitle=view.get_page_subtitle icon=view.header_icon tabbed=1 merged=1 latest_log_entry=latest_log_entry history_url=history_url %}
 {% endblock %}
 
 {% block form_actions %}
   <div class="dropdown dropup dropdown-button match-width">
-    <button type="submit" class="button action-save button-longrunning" data-clicked-text="{% trans 'Saving…' %}">
+    {# TODO: remove data-clicked-text once we drop support for Wagtail 4.x #}
+    <button type="submit" class="button action-save button-longrunning" data-clicked-text="{% trans 'Saving…' %}" data-controller="w-progress" data-action="w-progress#activate" data-w-progress-active-value="{% trans 'Saving…' %}">
       {% icon name="spinner" %}<em>{% trans "Save" %}</em>
     </button>
 
     {% if user_can_delete %}
       <div class="dropdown-toggle">{% icon name="arrow-up" %}</div>
       <ul>
         {% if translation %}
```

#### html2text {}

```diff
@@ -1,13 +1,14 @@
 {% extends "modeladmin/edit.html" %} {% load i18n wagtailadmin_tags %} {% block
 header %} {% include "modeladmin/includes/header_with_history.html" with
 title=view.get_page_title subtitle=view.get_page_subtitle icon=view.header_icon
 tabbed=1 merged=1 latest_log_entry=latest_log_entry history_url=history_url %}
 {% endblock %} {% block form_actions %}
- {% icon name="spinner" %}{% trans "Save" %}  {% if user_can_delete %}
+{# TODO: remove data-clicked-text once we drop support for Wagtail 4.x #}  {%
+icon name="spinner" %}{% trans "Save" %}  {% if user_can_delete %}
 {% icon name="arrow-up" %}
     * {% if translation %}
     *  {% trans "Start Synced translation" %}
     * {% endif %}
     * {%_trans_"Delete"_%}
 {% endif %}
 {% endblock %}
```

### Comparing `wagtail-localize-1.5/wagtail_localize/modeladmin/templates/wagtail_localize/modeladmin/translatable_index.html` & `wagtail-localize-1.5.1/wagtail_localize/modeladmin/templates/wagtail_localize/modeladmin/translatable_index.html`

 * *Files identical despite different names*

### Comparing `wagtail-localize-1.5/wagtail_localize/modeladmin/tests.py` & `wagtail-localize-1.5.1/wagtail_localize/modeladmin/tests.py`

 * *Files identical despite different names*

### Comparing `wagtail-localize-1.5/wagtail_localize/modeladmin/views.py` & `wagtail-localize-1.5.1/wagtail_localize/modeladmin/views.py`

 * *Files identical despite different names*

### Comparing `wagtail-localize-1.5/wagtail_localize/modeladmin/wagtail_hooks.py` & `wagtail-localize-1.5.1/wagtail_localize/modeladmin/wagtail_hooks.py`

 * *Files identical despite different names*

### Comparing `wagtail-localize-1.5/wagtail_localize/models.py` & `wagtail-localize-1.5.1/wagtail_localize/models.py`

 * *Files identical despite different names*

### Comparing `wagtail-localize-1.5/wagtail_localize/operations.py` & `wagtail-localize-1.5.1/wagtail_localize/operations.py`

 * *Files identical despite different names*

### Comparing `wagtail-localize-1.5/wagtail_localize/segments/extract.py` & `wagtail-localize-1.5.1/wagtail_localize/segments/extract.py`

 * *Files identical despite different names*

### Comparing `wagtail-localize-1.5/wagtail_localize/segments/ingest.py` & `wagtail-localize-1.5.1/wagtail_localize/segments/ingest.py`

 * *Files identical despite different names*

### Comparing `wagtail-localize-1.5/wagtail_localize/segments/types.py` & `wagtail-localize-1.5.1/wagtail_localize/segments/types.py`

 * *Files identical despite different names*

### Comparing `wagtail-localize-1.5/wagtail_localize/side_panels.py` & `wagtail-localize-1.5.1/wagtail_localize/side_panels.py`

 * *Files identical despite different names*

### Comparing `wagtail-localize-1.5/wagtail_localize/static/wagtail_localize/css/wagtail-localize-component-form.css` & `wagtail-localize-1.5.1/wagtail_localize/static/wagtail_localize/css/wagtail-localize-component-form.css`

 * *Files identical despite different names*

### Comparing `wagtail-localize-1.5/wagtail_localize/static/wagtail_localize/js/wagtail-localize-component-form.js` & `wagtail-localize-1.5.1/wagtail_localize/static/wagtail_localize/js/wagtail-localize-component-form.js`

 * *Files identical despite different names*

### Comparing `wagtail-localize-1.5/wagtail_localize/static/wagtail_localize/js/wagtail-localize.js` & `wagtail-localize-1.5.1/wagtail_localize/static/wagtail_localize/js/wagtail-localize.js`

 * *Files 3% similar despite different names*

#### js-beautify {}

```diff
@@ -76,29 +76,29 @@
             n.d(t, "ServerStyleSheet", (function() {
                 return Ue
             })), n.d(t, "StyleSheetConsumer", (function() {
                 return ae
             })), n.d(t, "StyleSheetContext", (function() {
                 return re
             })), n.d(t, "StyleSheetManager", (function() {
-                return ce
+                return ue
             })), n.d(t, "ThemeConsumer", (function() {
                 return Ne
             })), n.d(t, "ThemeContext", (function() {
                 return Re
             })), n.d(t, "ThemeProvider", (function() {
                 return Ie
             })), n.d(t, "__PRIVATE__", (function() {
                 return $e
             })), n.d(t, "createGlobalStyle", (function() {
                 return Le
             })), n.d(t, "css", (function() {
-                return Ee
+                return ye
             })), n.d(t, "isStyledComponent", (function() {
-                return y
+                return E
             })), n.d(t, "keyframes", (function() {
                 return Fe
             })), n.d(t, "useTheme", (function() {
                 return ze
             })), n.d(t, "version", (function() {
                 return _
             })), n.d(t, "withTheme", (function() {
@@ -106,16 +106,16 @@
             }));
             var r = n(4),
                 a = n(0),
                 o = n.n(a),
                 l = n(8),
                 i = n.n(l),
                 s = n(9),
-                u = n(10),
-                c = n(6),
+                c = n(10),
+                u = n(6),
                 d = n(5),
                 f = n.n(d);
 
             function m() {
                 return (m = Object.assign || function(e) {
                     for (var t = 1; t < arguments.length; t++) {
                         var n = arguments[t];
@@ -134,19 +134,19 @@
                 g = Object.freeze([]),
                 v = Object.freeze({});
 
             function b(e) {
                 return "function" == typeof e
             }
 
-            function E(e) {
+            function y(e) {
                 return e.displayName || e.name || "Component"
             }
 
-            function y(e) {
+            function E(e) {
                 return e && "string" == typeof e.styledComponentId
             }
             var w = void 0 !== e && (e.env.REACT_APP_SC_ATTR || e.env.SC_ATTR) || "data-styled",
                 _ = "5.3.0",
                 S = "undefined" != typeof window && "HTMLElement" in window,
                 k = Boolean("boolean" == typeof SC_DISABLE_SPEEDY ? SC_DISABLE_SPEEDY : void 0 !== e && void 0 !== e.env.REACT_APP_SC_DISABLE_SPEEDY && "" !== e.env.REACT_APP_SC_DISABLE_SPEEDY ? "false" !== e.env.REACT_APP_SC_DISABLE_SPEEDY && e.env.REACT_APP_SC_DISABLE_SPEEDY : void 0 !== e && void 0 !== e.env.SC_DISABLE_SPEEDY && "" !== e.env.SC_DISABLE_SPEEDY && ("false" !== e.env.SC_DISABLE_SPEEDY && e.env.SC_DISABLE_SPEEDY)),
                 x = {};
@@ -208,16 +208,16 @@
                 L = function(e, t) {
                     for (var n = t.innerHTML.split("/*!sc*/\n"), r = [], a = 0, o = n.length; a < o; a++) {
                         var l = n[a].trim();
                         if (l) {
                             var i = l.match(j);
                             if (i) {
                                 var s = 0 | parseInt(i[1], 10),
-                                    u = i[2];
-                                0 !== s && (D(u, s), M(e, u, i[3]), e.getTag().insertRules(s, r)), r.length = 0
+                                    c = i[2];
+                                0 !== s && (D(c, s), M(e, c, i[3]), e.getTag().insertRules(s, r)), r.length = 0
                             } else r.push(l)
                         }
                     }
                 },
                 F = function() {
                     return "undefined" != typeof window && void 0 !== window.__webpack_nonce__ ? window.__webpack_nonce__ : null
                 },
@@ -340,18 +340,18 @@
                             for (var t = e.getTag(), n = t.length, r = "", a = 0; a < n; a++) {
                                 var o = I(a);
                                 if (void 0 !== o) {
                                     var l = e.names.get(o),
                                         i = t.getGroup(a);
                                     if (void 0 !== l && 0 !== i.length) {
                                         var s = w + ".g" + a + '[id="' + o + '"]',
-                                            u = "";
+                                            c = "";
                                         void 0 !== l && l.forEach((function(e) {
-                                            e.length > 0 && (u += e + ",")
-                                        })), r += "" + i + s + '{content:"' + u + '"}/*!sc*/\n'
+                                            e.length > 0 && (c += e + ",")
+                                        })), r += "" + i + s + '{content:"' + c + '"}/*!sc*/\n'
                                     }
                                 }
                             }
                             return r
                         }(this)
                     }, e
                 }(),
@@ -372,15 +372,15 @@
                 J = function(e) {
                     return X(5381, e)
                 };
 
             function Z(e) {
                 for (var t = 0; t < e.length; t += 1) {
                     var n = e[t];
-                    if (b(n) && !y(n)) return !1
+                    if (b(n) && !E(n)) return !1
                 }
                 return !0
             }
             var K = J("5.3.0"),
                 Q = function() {
                     function e(e, t, n) {
                         this.rules = e, this.staticRulesId = "", this.isStatic = (void 0 === n || n.isStatic) && Z(e), this.componentId = t, this.baseHash = X(K, t), this.baseStyle = n, G.registerId(t)
@@ -396,27 +396,27 @@
                                 if (!t.hasNameForId(r, l)) {
                                     var i = n(o, "." + l, void 0, r);
                                     t.insertRules(r, l, i)
                                 }
                                 a.push(l), this.staticRulesId = l
                             }
                         else {
-                            for (var s = this.rules.length, u = X(this.baseHash, n.hash), c = "", d = 0; d < s; d++) {
+                            for (var s = this.rules.length, c = X(this.baseHash, n.hash), u = "", d = 0; d < s; d++) {
                                 var f = this.rules[d];
-                                if ("string" == typeof f) c += f;
+                                if ("string" == typeof f) u += f;
                                 else if (f) {
                                     var m = be(f, e, t, n),
                                         p = Array.isArray(m) ? m.join("") : m;
-                                    u = X(u, p + d), c += p
+                                    c = X(c, p + d), u += p
                                 }
                             }
-                            if (c) {
-                                var h = Y(u >>> 0);
+                            if (u) {
+                                var h = Y(c >>> 0);
                                 if (!t.hasNameForId(r, h)) {
-                                    var g = n(c, "." + h, void 0, r);
+                                    var g = n(u, "." + h, void 0, r);
                                     t.insertRules(r, h, g)
                                 }
                                 a.push(h)
                             }
                         }
                         return a.join(" ")
                     }, e
@@ -424,34 +424,34 @@
                 ee = /^\s*\/\/.*$/gm,
                 te = [":", "[", ".", "#"];
 
             function ne(e) {
                 var t, n, r, a, o = void 0 === e ? v : e,
                     l = o.options,
                     i = void 0 === l ? v : l,
-                    u = o.plugins,
-                    c = void 0 === u ? g : u,
+                    c = o.plugins,
+                    u = void 0 === c ? g : c,
                     d = new s.a(i),
                     f = [],
                     m = function(e) {
                         function t(t) {
                             if (t) try {
                                 e(t + "}")
                             } catch (e) {}
                         }
-                        return function(n, r, a, o, l, i, s, u, c, d) {
+                        return function(n, r, a, o, l, i, s, c, u, d) {
                             switch (n) {
                                 case 1:
-                                    if (0 === c && 64 === r.charCodeAt(0)) return e(r + ";"), "";
+                                    if (0 === u && 64 === r.charCodeAt(0)) return e(r + ";"), "";
                                     break;
                                 case 2:
-                                    if (0 === u) return r + "/*|*/";
+                                    if (0 === c) return r + "/*|*/";
                                     break;
                                 case 3:
-                                    switch (u) {
+                                    switch (c) {
                                         case 102:
                                         case 112:
                                             return e(a[0] + r), "";
                                         default:
                                             return r + (0 === d ? "/*|*/" : "")
                                     }
                                 case -2:
@@ -464,69 +464,69 @@
                     p = function(e, r, o) {
                         return 0 === r && -1 !== te.indexOf(o[n.length]) || o.match(a) ? e : "." + t
                     };
 
                 function h(e, o, l, i) {
                     void 0 === i && (i = "&");
                     var s = e.replace(ee, ""),
-                        u = o && l ? l + " " + o + " { " + s + " }" : s;
-                    return t = i, n = o, r = new RegExp("\\" + n + "\\b", "g"), a = new RegExp("(\\" + n + "\\b){2,}"), d(l || !o ? "" : o, u)
+                        c = o && l ? l + " " + o + " { " + s + " }" : s;
+                    return t = i, n = o, r = new RegExp("\\" + n + "\\b", "g"), a = new RegExp("(\\" + n + "\\b){2,}"), d(l || !o ? "" : o, c)
                 }
-                return d.use([].concat(c, [function(e, t, a) {
+                return d.use([].concat(u, [function(e, t, a) {
                     2 === e && a.length && a[0].lastIndexOf(n) > 0 && (a[0] = a[0].replace(r, p))
                 }, m, function(e) {
                     if (-2 === e) {
                         var t = f;
                         return f = [], t
                     }
-                }])), h.hash = c.length ? c.reduce((function(e, t) {
+                }])), h.hash = u.length ? u.reduce((function(e, t) {
                     return t.name || O(15), X(e, t.name)
                 }), 5381).toString() : "", h
             }
             var re = o.a.createContext(),
                 ae = re.Consumer,
                 oe = o.a.createContext(),
                 le = (oe.Consumer, new G),
                 ie = ne();
 
             function se() {
                 return Object(a.useContext)(re) || le
             }
 
-            function ue() {
+            function ce() {
                 return Object(a.useContext)(oe) || ie
             }
 
-            function ce(e) {
+            function ue(e) {
                 var t = Object(a.useState)(e.stylisPlugins),
                     n = t[0],
                     r = t[1],
                     l = se(),
                     s = Object(a.useMemo)((function() {
                         var t = l;
                         return e.sheet ? t = e.sheet : e.target && (t = t.reconstructWithOptions({
                             target: e.target
                         }, !1)), e.disableCSSOMInjection && (t = t.reconstructWithOptions({
                             useCSSOMInjection: !1
                         })), t
                     }), [e.disableCSSOMInjection, e.sheet, e.target]),
-                    u = Object(a.useMemo)((function() {
+                    c = Object(a.useMemo)((function() {
                         return ne({
                             options: {
                                 prefix: !e.disableVendorPrefixes
                             },
                             plugins: n
                         })
                     }), [e.disableVendorPrefixes, n]);
                 return Object(a.useEffect)((function() {
                     i()(n, e.stylisPlugins) || r(e.stylisPlugins)
                 }), [e.stylisPlugins]), o.a.createElement(re.Provider, {
                     value: s
                 }, o.a.createElement(oe.Provider, {
-                    value: u
+                    value: c
                 }, e.children))
             }
             var de = function() {
                     function e(e, t) {
                         var n = this;
                         this.inject = function(e, t) {
                             void 0 === t && (t = ie);
@@ -555,28 +555,28 @@
             };
 
             function be(e, t, n, r) {
                 if (Array.isArray(e)) {
                     for (var a, o = [], l = 0, i = e.length; l < i; l += 1) "" !== (a = be(e[l], t, n, r)) && (Array.isArray(a) ? o.push.apply(o, a) : o.push(a));
                     return o
                 }
-                return ve(e) ? "" : y(e) ? "." + e.styledComponentId : b(e) ? "function" != typeof(s = e) || s.prototype && s.prototype.isReactComponent || !t ? e : be(e(t), t, n, r) : e instanceof de ? n ? (e.inject(n, r), e.getName(r)) : e : h(e) ? function e(t, n) {
+                return ve(e) ? "" : E(e) ? "." + e.styledComponentId : b(e) ? "function" != typeof(s = e) || s.prototype && s.prototype.isReactComponent || !t ? e : be(e(t), t, n, r) : e instanceof de ? n ? (e.inject(n, r), e.getName(r)) : e : h(e) ? function e(t, n) {
                     var r, a, o = [];
-                    for (var l in t) t.hasOwnProperty(l) && !ve(t[l]) && (h(t[l]) ? o.push.apply(o, e(t[l], l)) : b(t[l]) ? o.push(ge(l) + ":", t[l], ";") : o.push(ge(l) + ": " + (r = l, (null == (a = t[l]) || "boolean" == typeof a || "" === a ? "" : "number" != typeof a || 0 === a || r in u.a ? String(a).trim() : a + "px") + ";")));
+                    for (var l in t) t.hasOwnProperty(l) && !ve(t[l]) && (h(t[l]) ? o.push.apply(o, e(t[l], l)) : b(t[l]) ? o.push(ge(l) + ":", t[l], ";") : o.push(ge(l) + ": " + (r = l, (null == (a = t[l]) || "boolean" == typeof a || "" === a ? "" : "number" != typeof a || 0 === a || r in c.a ? String(a).trim() : a + "px") + ";")));
                     return n ? [n + " {"].concat(o, ["}"]) : o
                 }(e) : e.toString();
                 var s
             }
 
-            function Ee(e) {
+            function ye(e) {
                 for (var t = arguments.length, n = new Array(t > 1 ? t - 1 : 0), r = 1; r < t; r++) n[r - 1] = arguments[r];
                 return b(e) || h(e) ? be(p(g, [e].concat(n))) : 0 === n.length && 1 === e.length && "string" == typeof e[0] ? e : be(p(e, n))
             }
             new Set;
-            var ye = function(e, t, n) {
+            var Ee = function(e, t, n) {
                     return void 0 === n && (n = v), e.theme !== n.theme && e.theme || t || n.theme
                 },
                 we = /[!"#$%&'()*+,./:;<=>?@[\\\]^`{|}~-]+/g,
                 _e = /(^-|-$)/g;
 
             function Se(e) {
                 return e.replace(we, "-").replace(_e, "")
@@ -622,28 +622,28 @@
                 return e.children ? o.a.createElement(Re.Provider, {
                     value: n
                 }, e.children) : null
             }
             var De = {};
 
             function Pe(e, t, n) {
-                var r = y(e),
+                var r = E(e),
                     l = !xe(e),
                     i = t.attrs,
                     s = void 0 === i ? g : i,
-                    u = t.componentId,
-                    d = void 0 === u ? function(e, t) {
+                    c = t.componentId,
+                    d = void 0 === c ? function(e, t) {
                         var n = "string" != typeof e ? "sc" : Se(e);
                         De[n] = (De[n] || 0) + 1;
                         var r = n + "-" + ke("5.3.0" + n + De[n]);
                         return t ? t + "-" + r : r
-                    }(t.displayName, t.parentComponentId) : u,
+                    }(t.displayName, t.parentComponentId) : c,
                     p = t.displayName,
                     h = void 0 === p ? function(e) {
-                        return xe(e) ? "styled." + e : "Styled(" + E(e) + ")"
+                        return xe(e) ? "styled." + e : "Styled(" + y(e) + ")"
                     }(e) : p,
                     w = t.displayName && t.componentId ? Se(t.displayName) + "-" + t.componentId : t.componentId || d,
                     _ = r && e.attrs ? Array.prototype.concat(e.attrs, s).filter(Boolean) : s,
                     S = t.shouldForwardProp;
                 r && e.shouldForwardProp && (S = t.shouldForwardProp ? function(n, r, a) {
                     return e.shouldForwardProp(n, r, a) && t.shouldForwardProp(n, r, a)
                 } : e.shouldForwardProp);
@@ -651,54 +651,54 @@
                     O = x.isStatic && 0 === s.length,
                     A = function(e, t) {
                         return function(e, t, n, r) {
                             var o = e.attrs,
                                 l = e.componentStyle,
                                 i = e.defaultProps,
                                 s = e.foldedComponentIds,
-                                u = e.shouldForwardProp,
+                                c = e.shouldForwardProp,
                                 d = e.styledComponentId,
                                 f = e.target,
                                 p = function(e, t, n) {
                                     void 0 === e && (e = v);
                                     var r = m({}, t, {
                                             theme: e
                                         }),
                                         a = {};
                                     return n.forEach((function(e) {
                                         var t, n, o, l = e;
                                         for (t in b(l) && (l = l(r)), l) r[t] = a[t] = "className" === t ? (n = a[t], o = l[t], n && o ? n + " " + o : n || o) : l[t]
                                     })), [r, a]
-                                }(ye(t, Object(a.useContext)(Re), i) || v, t, o),
+                                }(Ee(t, Object(a.useContext)(Re), i) || v, t, o),
                                 h = p[0],
                                 g = p[1],
-                                E = function(e, t, n, r) {
+                                y = function(e, t, n, r) {
                                     var a = se(),
-                                        o = ue();
+                                        o = ce();
                                     return t ? e.generateAndInjectStyles(v, a, o) : e.generateAndInjectStyles(n, a, o)
                                 }(l, r, h),
-                                y = n,
+                                E = n,
                                 w = g.$as || t.$as || g.as || t.as || f,
                                 _ = xe(w),
                                 S = g !== t ? m({}, t, {}, g) : t,
                                 k = {};
-                            for (var x in S) "$" !== x[0] && "as" !== x && ("forwardedAs" === x ? k.as = S[x] : (u ? u(x, c.a, w) : !_ || Object(c.a)(x)) && (k[x] = S[x]));
-                            return t.style && g.style !== t.style && (k.style = m({}, t.style, {}, g.style)), k.className = Array.prototype.concat(s, d, E !== d ? E : null, t.className, g.className).filter(Boolean).join(" "), k.ref = y, Object(a.createElement)(w, k)
+                            for (var x in S) "$" !== x[0] && "as" !== x && ("forwardedAs" === x ? k.as = S[x] : (c ? c(x, u.a, w) : !_ || Object(u.a)(x)) && (k[x] = S[x]));
+                            return t.style && g.style !== t.style && (k.style = m({}, t.style, {}, g.style)), k.className = Array.prototype.concat(s, d, y !== d ? y : null, t.className, g.className).filter(Boolean).join(" "), k.ref = E, Object(a.createElement)(w, k)
                         }(k, e, t, O)
                     };
                 return A.displayName = h, (k = o.a.forwardRef(A)).attrs = _, k.componentStyle = x, k.displayName = h, k.shouldForwardProp = S, k.foldedComponentIds = r ? Array.prototype.concat(e.foldedComponentIds, e.styledComponentId) : g, k.styledComponentId = w, k.target = r ? e.target : e, k.withComponent = function(e) {
                     var r = t.componentId,
                         a = function(e, t) {
                             if (null == e) return {};
                             var n, r, a = {},
                                 o = Object.keys(e);
                             for (r = 0; r < o.length; r++) n = o[r], t.indexOf(n) >= 0 || (a[n] = e[n]);
                             return a
                         }(t, ["componentId"]),
-                        o = r && r + "-" + (xe(e) ? e : Se(E(e)));
+                        o = r && r + "-" + (xe(e) ? e : Se(y(e)));
                     return Pe(e, m({}, a, {
                         attrs: _,
                         componentId: o
                     }), n)
                 }, Object.defineProperty(k, "defaultProps", {
                     get: function() {
                         return this._foldedDefaultProps
@@ -719,15 +719,15 @@
                     withComponent: !0
                 }), k
             }
             var je = function(e) {
                 return function e(t, n, a) {
                     if (void 0 === a && (a = v), !Object(r.isValidElementType)(n)) return O(1, String(n));
                     var o = function() {
-                        return t(n, a, Ee.apply(void 0, arguments))
+                        return t(n, a, ye.apply(void 0, arguments))
                     };
                     return o.withConfig = function(r) {
                         return e(t, n, m({}, a, {}, r))
                     }, o.attrs = function(r) {
                         return e(t, n, m({}, a, {
                             attrs: Array.prototype.concat(a.attrs, r).filter(Boolean)
                         }))
@@ -751,46 +751,46 @@
                 }, t.renderStyles = function(e, t, n, r) {
                     e > 2 && G.registerId(this.componentId + e), this.removeStyles(e, n), this.createStyles(e, t, n, r)
                 }, e
             }();
 
             function Le(e) {
                 for (var t = arguments.length, n = new Array(t > 1 ? t - 1 : 0), r = 1; r < t; r++) n[r - 1] = arguments[r];
-                var l = Ee.apply(void 0, [e].concat(n)),
+                var l = ye.apply(void 0, [e].concat(n)),
                     i = "sc-global-" + ke(JSON.stringify(l)),
                     s = new Me(l, i);
 
-                function u(e) {
+                function c(e) {
                     var t = se(),
-                        n = ue(),
+                        n = ce(),
                         r = Object(a.useContext)(Re),
                         o = Object(a.useRef)(t.allocateGSInstance(i)).current;
                     return Object(a.useLayoutEffect)((function() {
-                        return c(o, e, t, r, n),
+                        return u(o, e, t, r, n),
                             function() {
                                 return s.removeStyles(o, t)
                             }
                     }), [o, e, t, r, n]), null
                 }
 
-                function c(e, t, n, r, a) {
+                function u(e, t, n, r, a) {
                     if (s.isStatic) s.renderStyles(e, x, n, a);
                     else {
                         var o = m({}, t, {
-                            theme: ye(t, r, u.defaultProps)
+                            theme: Ee(t, r, c.defaultProps)
                         });
                         s.renderStyles(e, o, n, a)
                     }
                 }
-                return o.a.memo(u)
+                return o.a.memo(c)
             }
 
             function Fe(e) {
                 for (var t = arguments.length, n = new Array(t > 1 ? t - 1 : 0), r = 1; r < t; r++) n[r - 1] = arguments[r];
-                var a = Ee.apply(void 0, [e].concat(n)).join(""),
+                var a = ye.apply(void 0, [e].concat(n)).join(""),
                     o = ke(a);
                 return new de(o, a)
             }
             var Ue = function() {
                     function e() {
                         var e = this;
                         this._emitSheetCSS = function() {
@@ -813,32 +813,32 @@
                             e.sealed = !0
                         }, this.instance = new G({
                             isServer: !0
                         }), this.sealed = !1
                     }
                     var t = e.prototype;
                     return t.collectStyles = function(e) {
-                        return this.sealed ? O(2) : o.a.createElement(ce, {
+                        return this.sealed ? O(2) : o.a.createElement(ue, {
                             sheet: this.instance
                         }, e)
                     }, t.interleaveWithNodeStream = function(e) {
                         return O(3)
                     }, e
                 }(),
                 Ve = function(e) {
                     var t = o.a.forwardRef((function(t, n) {
                         var r = Object(a.useContext)(Re),
                             l = e.defaultProps,
-                            i = ye(t, r, l);
+                            i = Ee(t, r, l);
                         return o.a.createElement(e, m({}, t, {
                             theme: i,
                             ref: n
                         }))
                     }));
-                    return f()(t, e), t.displayName = "WithTheme(" + E(e) + ")", t
+                    return f()(t, e), t.displayName = "WithTheme(" + y(e) + ")", t
                 },
                 ze = function() {
                     return Object(a.useContext)(Re)
                 },
                 $e = {
                     StyleSheet: G,
                     masterSheet: le
@@ -889,34 +889,34 @@
     i[r.ForwardRef] = {
         $$typeof: !0,
         render: !0,
         defaultProps: !0,
         displayName: !0,
         propTypes: !0
     }, i[r.Memo] = l;
-    var u = Object.defineProperty,
-        c = Object.getOwnPropertyNames,
+    var c = Object.defineProperty,
+        u = Object.getOwnPropertyNames,
         d = Object.getOwnPropertySymbols,
         f = Object.getOwnPropertyDescriptor,
         m = Object.getPrototypeOf,
         p = Object.prototype;
     e.exports = function e(t, n, r) {
         if ("string" != typeof n) {
             if (p) {
                 var a = m(n);
                 a && a !== p && e(t, a, r)
             }
-            var l = c(n);
+            var l = u(n);
             d && (l = l.concat(d(n)));
             for (var i = s(t), h = s(n), g = 0; g < l.length; ++g) {
                 var v = l[g];
                 if (!(o[v] || r && r[v] || h && h[v] || i && i[v])) {
                     var b = f(n, v);
                     try {
-                        u(t, v, b)
+                        c(t, v, b)
                     } catch (e) {}
                 }
             }
         }
         return t
     }
 }, function(e, t, n) {
@@ -1019,19 +1019,19 @@
         if (void 0 !== a) return !!a;
         if (e === t) return !0;
         if ("object" != typeof e || !e || "object" != typeof t || !t) return !1;
         var o = Object.keys(e),
             l = Object.keys(t);
         if (o.length !== l.length) return !1;
         for (var i = Object.prototype.hasOwnProperty.bind(t), s = 0; s < o.length; s++) {
-            var u = o[s];
-            if (!i(u)) return !1;
-            var c = e[u],
-                d = t[u];
-            if (!1 === (a = n ? n.call(r, c, d, u) : void 0) || void 0 === a && c !== d) return !1
+            var c = o[s];
+            if (!i(c)) return !1;
+            var u = e[c],
+                d = t[c];
+            if (!1 === (a = n ? n.call(r, u, d, c) : void 0) || void 0 === a && u !== d) return !1
         }
         return !0
     }
 }, function(e, t, n) {
     "use strict";
     t.a = function(e) {
         function t(e, t, r) {
@@ -1044,15 +1044,15 @@
                 case 1:
                     var i = 0;
                     for (e = 0 === l ? "" : e[0] + " "; i < o; ++i) t[i] = n(e, t[i], r).trim();
                     break;
                 default:
                     var s = i = 0;
                     for (t = []; i < o; ++i)
-                        for (var u = 0; u < l; ++u) t[s++] = n(e[u] + " ", a[i], r).trim()
+                        for (var c = 0; c < l; ++c) t[s++] = n(e[c] + " ", a[i], r).trim()
             }
             return t
         }
 
         function n(e, t, n) {
             var r = t.charCodeAt(0);
             switch (33 > r && (r = (t = t.trim()).charCodeAt(0)), r) {
@@ -1112,21 +1112,21 @@
                     if (99 !== l.charCodeAt(8)) break;
                     return "-webkit-box-pack" + (s = l.substring(l.indexOf(":", 15)).replace("flex-", "").replace("space-between", "justify")) + "-webkit-" + l + "-ms-flex-pack" + s + l;
                 case 1005:
                     return f.test(l) ? l.replace(d, ":-webkit-") + l.replace(d, ":-moz-") + l : l;
                 case 1e3:
                     switch (t = (s = l.substring(13).trim()).indexOf("-") + 1, s.charCodeAt(0) + s.charCodeAt(t)) {
                         case 226:
-                            s = l.replace(E, "tb");
+                            s = l.replace(y, "tb");
                             break;
                         case 232:
-                            s = l.replace(E, "tb-rl");
+                            s = l.replace(y, "tb-rl");
                             break;
                         case 220:
-                            s = l.replace(E, "lr");
+                            s = l.replace(y, "lr");
                             break;
                         default:
                             return l
                     }
                     return "-webkit-" + l + "-ms-" + s + l;
                 case 1017:
                     if (-1 === l.indexOf("sticky", 9)) break;
@@ -1172,16 +1172,16 @@
         }
 
         function o(e, t) {
             var n = r(t, t.charCodeAt(0), t.charCodeAt(1), t.charCodeAt(2));
             return n !== t + ";" ? n.replace(w, " or ($1)").substring(4) : "(" + t + ")"
         }
 
-        function l(e, t, n, r, a, o, l, i, u, c) {
-            for (var d, f = 0, m = t; f < I; ++f) switch (d = N[f].call(s, e, m, n, r, a, o, l, i, u, c)) {
+        function l(e, t, n, r, a, o, l, i, c, u) {
+            for (var d, f = 0, m = t; f < I; ++f) switch (d = N[f].call(s, e, m, n, r, a, o, l, i, c, u)) {
                 case void 0:
                 case !1:
                 case !0:
                 case null:
                     break;
                 default:
                     m = d
@@ -1196,17 +1196,17 @@
         function s(e, n) {
             var i = e;
             if (33 > i.charCodeAt(0) && (i = i.trim()), i = [i], 0 < I) {
                 var s = l(-1, n, i, i, A, O, 0, 0, 0, 0);
                 void 0 !== s && "string" == typeof s && (n = s)
             }
             var d = function e(n, i, s, d, f) {
-                for (var m, p, h, E, w, _ = 0, S = 0, k = 0, x = 0, N = 0, D = 0, j = h = m = 0, M = 0, L = 0, F = 0, U = 0, V = s.length, z = V - 1, $ = "", B = "", H = "", G = ""; M < V;) {
+                for (var m, p, h, y, w, _ = 0, S = 0, k = 0, x = 0, N = 0, D = 0, j = h = m = 0, M = 0, L = 0, F = 0, U = 0, V = s.length, z = V - 1, $ = "", B = "", H = "", G = ""; M < V;) {
                     if (p = s.charCodeAt(M), M === z && 0 !== S + x + k + _ && (0 !== S && (p = 47 === S ? 10 : 47), x = k = _ = 0, V++, z++), 0 === S + x + k + _) {
-                        if (M === z && (0 < L && ($ = $.replace(c, "")), 0 < $.trim().length)) {
+                        if (M === z && (0 < L && ($ = $.replace(u, "")), 0 < $.trim().length)) {
                             switch (p) {
                                 case 32:
                                 case 9:
                                 case 59:
                                 case 13:
                                 case 10:
                                     break;
@@ -1254,29 +1254,29 @@
                                         case 34:
                                         case 39:
                                             for (; M++ < z && s.charCodeAt(M) !== p;);
                                     }
                                     if (0 === h) break;
                                     M++
                                 }
-                                switch (h = s.substring(U, M), 0 === m && (m = ($ = $.replace(u, "").trim()).charCodeAt(0)), m) {
+                                switch (h = s.substring(U, M), 0 === m && (m = ($ = $.replace(c, "").trim()).charCodeAt(0)), m) {
                                     case 64:
-                                        switch (0 < L && ($ = $.replace(c, "")), p = $.charCodeAt(1)) {
+                                        switch (0 < L && ($ = $.replace(u, "")), p = $.charCodeAt(1)) {
                                             case 100:
                                             case 109:
                                             case 115:
                                             case 45:
                                                 L = i;
                                                 break;
                                             default:
                                                 L = R
                                         }
                                         if (U = (h = e(i, L, h, p, f + 1)).length, 0 < I && (w = l(3, h, L = t(R, $, F), i, A, O, U, p, f, d), $ = L.join(""), void 0 !== w && 0 === (U = (h = w.trim()).length) && (p = 0, h = "")), 0 < U) switch (p) {
                                             case 115:
-                                                $ = $.replace(y, o);
+                                                $ = $.replace(E, o);
                                             case 100:
                                             case 109:
                                             case 45:
                                                 h = $ + "{" + h + "}";
                                                 break;
                                             case 107:
                                                 h = ($ = $.replace(g, "$1 $2")) + "{" + h + "}", h = 1 === T || 2 === T && a("@" + h, 3) ? "@-webkit-" + h + "@" + h : "@" + h;
@@ -1288,15 +1288,15 @@
                                     default:
                                         h = e(i, t(i, $, F), h, d, f + 1)
                                 }
                                 H += h, h = F = L = j = m = 0, $ = "", p = s.charCodeAt(++M);
                                 break;
                             case 125:
                             case 59:
-                                if (1 < (U = ($ = (0 < L ? $.replace(c, "") : $).trim()).length)) switch (0 === j && (m = $.charCodeAt(0), 45 === m || 96 < m && 123 > m) && (U = ($ = $.replace(" ", ":")).length), 0 < I && void 0 !== (w = l(1, $, i, n, A, O, B.length, d, f, d)) && 0 === (U = ($ = w.trim()).length) && ($ = "\0\0"), m = $.charCodeAt(0), p = $.charCodeAt(1), m) {
+                                if (1 < (U = ($ = (0 < L ? $.replace(u, "") : $).trim()).length)) switch (0 === j && (m = $.charCodeAt(0), 45 === m || 96 < m && 123 > m) && (U = ($ = $.replace(" ", ":")).length), 0 < I && void 0 !== (w = l(1, $, i, n, A, O, B.length, d, f, d)) && 0 === (U = ($ = w.trim()).length) && ($ = "\0\0"), m = $.charCodeAt(0), p = $.charCodeAt(1), m) {
                                     case 0:
                                         break;
                                     case 64:
                                         if (105 === p || 99 === p) {
                                             G += $ + s.charAt(M);
                                             break
                                         }
@@ -1314,53 +1314,53 @@
                         case 59:
                         case 125:
                             if (0 === S + x + k + _) {
                                 O++;
                                 break
                             }
                         default:
-                            switch (O++, E = s.charAt(M), p) {
+                            switch (O++, y = s.charAt(M), p) {
                                 case 9:
                                 case 32:
                                     if (0 === x + _ + S) switch (N) {
                                         case 44:
                                         case 58:
                                         case 9:
                                         case 32:
-                                            E = "";
+                                            y = "";
                                             break;
                                         default:
-                                            32 !== p && (E = " ")
+                                            32 !== p && (y = " ")
                                     }
                                     break;
                                 case 0:
-                                    E = "\\0";
+                                    y = "\\0";
                                     break;
                                 case 12:
-                                    E = "\\f";
+                                    y = "\\f";
                                     break;
                                 case 11:
-                                    E = "\\v";
+                                    y = "\\v";
                                     break;
                                 case 38:
-                                    0 === x + S + _ && (L = F = 1, E = "\f" + E);
+                                    0 === x + S + _ && (L = F = 1, y = "\f" + y);
                                     break;
                                 case 108:
                                     if (0 === x + S + _ + C && 0 < j) switch (M - j) {
                                         case 2:
                                             112 === N && 58 === s.charCodeAt(M - 3) && (C = N);
                                         case 8:
                                             111 === D && (C = D)
                                     }
                                     break;
                                 case 58:
                                     0 === x + S + _ && (j = M);
                                     break;
                                 case 44:
-                                    0 === S + k + x + _ && (L = 1, E += "\r");
+                                    0 === S + k + x + _ && (L = 1, y += "\r");
                                     break;
                                 case 34:
                                 case 39:
                                     0 === S && (x = x === p ? 0 : 0 === x ? p : x);
                                     break;
                                 case 91:
                                     0 === x + S + k && _++;
@@ -1394,18 +1394,18 @@
                                                     S = 47;
                                                     break;
                                                 case 220:
                                                     U = M, S = 42
                                             }
                                             break;
                                         case 42:
-                                            47 === p && 42 === N && U + 2 !== M && (33 === s.charCodeAt(U + 2) && (B += s.substring(U, M + 1)), E = "", S = 0)
+                                            47 === p && 42 === N && U + 2 !== M && (33 === s.charCodeAt(U + 2) && (B += s.substring(U, M + 1)), y = "", S = 0)
                                     }
                             }
-                            0 === S && ($ += E)
+                            0 === S && ($ += y)
                     }
                     D = N, N = p, M++
                 }
                 if (0 < (U = B.length)) {
                     if (L = i, 0 < I && (void 0 !== (w = l(2, B, L, n, A, O, U, d, f, d)) && 0 === (B = w).length)) return G + B + H;
                     if (B = L.join(",") + "{" + B + "}", 0 != T * C) {
                         switch (2 !== T || a(B, 2) || (C = 0), C) {
@@ -1418,26 +1418,26 @@
                         C = 0
                     }
                 }
                 return G + B + H
             }(R, i, n, 0, 0);
             return 0 < I && (void 0 !== (s = l(-2, d, i, i, A, O, d.length, 0, 0, 0)) && (d = s)), "", C = 0, O = A = 1, d
         }
-        var u = /^\0+/g,
-            c = /[\0\r\f]/g,
+        var c = /^\0+/g,
+            u = /[\0\r\f]/g,
             d = /: */g,
             f = /zoo|gra/,
             m = /([,: ])(transform)/g,
             p = /,\r+?/g,
             h = /([\t\r\n ])*\f?&/g,
             g = /@(k\w+)\s*(\S*)\s*/,
             v = /::(place)/g,
             b = /:(read-only)/g,
-            E = /[svh]\w+-[tblr]{2}/,
-            y = /\(\s*(.*)\s*\)/g,
+            y = /[svh]\w+-[tblr]{2}/,
+            E = /\(\s*(.*)\s*\)/g,
             w = /([\s\S]*?);/g,
             _ = /-self|flex-/g,
             S = /[^]*?(:[rp][el]a[\w-]+)[^]*/,
             k = /stretch|:\s*\w+\-(?:conte|avail)/,
             x = /([^-])(image-set\()/,
             O = 1,
             A = 1,
@@ -1630,20 +1630,20 @@
             return e && e.__esModule ? e : {
                 default: e
             }
         };
     t.__esModule = !0;
     var i = l(n(0)),
         s = l(n(13)),
-        u = l(n(14));
+        c = l(n(14));
     document.addEventListener("DOMContentLoaded", (function() {
         return a(void 0, void 0, void 0, (function() {
             var e, t, n, a, l;
             return o(this, (function(o) {
-                return (e = document.querySelector(".js-translation-editor")) instanceof HTMLElement && e.dataset.props && ((t = e.querySelector('[name="csrfmiddlewaretoken"]')) instanceof HTMLInputElement ? (n = t.value, a = JSON.parse(e.dataset.props), l = u.default, s.default.render(i.default.createElement(l, r({
+                return (e = document.querySelector(".js-translation-editor")) instanceof HTMLElement && e.dataset.props && ((t = e.querySelector('[name="csrfmiddlewaretoken"]')) instanceof HTMLInputElement ? (n = t.value, a = JSON.parse(e.dataset.props), l = c.default, s.default.render(i.default.createElement(l, r({
                     csrfToken: n
                 }, a)), e)) : console.error("Not starting translation editor because I couldn't find the CSRF token element!")), [2]
             }))
         }))
     }))
 }, function(e, t) {
     e.exports = ReactDOM
@@ -1684,16 +1684,16 @@
         i = this && this.__importDefault || function(e) {
             return e && e.__esModule ? e : {
                 default: e
             }
         };
     t.__esModule = !0;
     var s = l(n(0)),
-        u = i(n(15)),
-        c = n(18),
+        c = i(n(15)),
+        u = n(18),
         d = n(7),
         f = i(n(19)),
         m = i(n(20)),
         p = i(n(22)),
         h = i(n(28)),
         g = i(n(1));
     t.default = function(e) {
@@ -1749,35 +1749,39 @@
                     })).length,
                     segments: n
                 }, t)
             })).filter((function(e) {
                 return e.segments.length > 0
             })),
             b = s.default.createElement(s.default.Fragment, null);
-        return b = v.length > 1 ? s.default.createElement(c.Tabs, {
+        return b = v.length > 1 ? s.default.createElement(u.Tabs, {
             tabs: v
         }, v.map((function(t) {
-            return s.default.createElement(c.TabContent, r({
+            return s.default.createElement(u.TabContent, r({
                 key: t.slug
             }, t), s.default.createElement(h.default, r({}, e, l, {
                 dispatch: i
-            })), s.default.createElement(u.default, {
+            })), s.default.createElement(c.default, {
                 title: e.sourceLocale.displayName + " to " + e.locale.displayName + " translation"
             }, s.default.createElement(p.default, r({}, e, {
                 segments: t.segments
             }, l, {
                 dispatch: i
             }))))
-        }))) : s.default.createElement(s.default.Fragment, null, s.default.createElement(h.default, r({}, e, l, {
+        }))) : s.default.createElement("div", {
+            className: "w-tabs"
+        }, s.default.createElement("div", {
+            className: "tab-content"
+        }, s.default.createElement(h.default, r({}, e, l, {
             dispatch: i
-        })), s.default.createElement(u.default, {
+        })), s.default.createElement(c.default, {
             title: e.sourceLocale.displayName + " to " + e.locale.displayName + " translation"
         }, s.default.createElement(p.default, r({}, e, l, {
             dispatch: i
-        })))), s.default.createElement(s.default.Fragment, null, s.default.createElement(f.default, r({}, e, l)), b, s.default.createElement(m.default, r({}, e)))
+        }))))), s.default.createElement(s.default.Fragment, null, s.default.createElement(f.default, r({}, e, l)), b, s.default.createElement(m.default, r({}, e)))
     }
 }, function(e, t, n) {
     "use strict";
     var r = this && this.__makeTemplateObject || function(e, t) {
             return Object.defineProperty ? Object.defineProperty(e, "raw", {
                 value: t
             }) : e.raw = t, e
@@ -1785,15 +1789,15 @@
         a = this && this.__importDefault || function(e) {
             return e && e.__esModule ? e : {
                 default: e
             }
         };
     t.__esModule = !0;
     var o, l = a(n(0)),
-        i = a(n(3)).default.div(o || (o = r(["\n    box-sizing: border-box;\n    height: 40px;\n    -webkit-font-smoothing: auto;\n    background-color: var(--w-color-secondary-50);\n    color: var(--w-color-secondary);\n    padding: 0.9em 0 0.9em 95px;\n    font-size: 0.95em;\n    margin: 0;\n    line-height: 1.5em;\n    font-weight: 400;\n    overflow: hidden;\n    position: relative;\n\n    > h3 {\n        display: inline;\n        text-transform: inherit;\n        font-weight: inherit;\n        float: none;\n        color: inherit;\n        font-size: inherit;\n    }\n"], ["\n    box-sizing: border-box;\n    height: 40px;\n    -webkit-font-smoothing: auto;\n    background-color: var(--w-color-secondary-50);\n    color: var(--w-color-secondary);\n    padding: 0.9em 0 0.9em 95px;\n    font-size: 0.95em;\n    margin: 0;\n    line-height: 1.5em;\n    font-weight: 400;\n    overflow: hidden;\n    position: relative;\n\n    > h3 {\n        display: inline;\n        text-transform: inherit;\n        font-weight: inherit;\n        float: none;\n        color: inherit;\n        font-size: inherit;\n    }\n"])));
+        i = a(n(3)).default.div(o || (o = r(["\n    box-sizing: border-box;\n    height: 40px;\n    -webkit-font-smoothing: auto;\n    background-color: var(\n        --w-color-surface-panel-information,\n        var(--w-color-secondary-50)\n    );\n    color: var(--w-text-surface-panel-information, var(--w-color-secondary));\n    padding: 1em 0 1em 1.5em;\n    font-size: 0.95em;\n    margin: 0;\n    line-height: 1.5em;\n    font-weight: 400;\n    overflow: hidden;\n    position: relative;\n\n    > h3 {\n        display: inline;\n        text-transform: inherit;\n        font-weight: inherit;\n        float: none;\n        color: inherit;\n        font-size: inherit;\n    }\n"], ["\n    box-sizing: border-box;\n    height: 40px;\n    -webkit-font-smoothing: auto;\n    background-color: var(\n        --w-color-surface-panel-information,\n        var(--w-color-secondary-50)\n    );\n    color: var(--w-text-surface-panel-information, var(--w-color-secondary));\n    padding: 1em 0 1em 1.5em;\n    font-size: 0.95em;\n    margin: 0;\n    line-height: 1.5em;\n    font-weight: 400;\n    overflow: hidden;\n    position: relative;\n\n    > h3 {\n        display: inline;\n        text-transform: inherit;\n        font-weight: inherit;\n        float: none;\n        color: inherit;\n        font-size: inherit;\n    }\n"])));
     t.default = function(e) {
         var t = e.title,
             n = e.children;
         return l.default.createElement("section", null, l.default.createElement(i, null, l.default.createElement("h3", null, t)), n)
     }
 }, function(e, t) {
     var n, r, a = e.exports = {};
@@ -1826,31 +1830,31 @@
         }
         try {
             r = "function" == typeof clearTimeout ? clearTimeout : l
         } catch (e) {
             r = l
         }
     }();
-    var s, u = [],
-        c = !1,
+    var s, c = [],
+        u = !1,
         d = -1;
 
     function f() {
-        c && s && (c = !1, s.length ? u = s.concat(u) : d = -1, u.length && m())
+        u && s && (u = !1, s.length ? c = s.concat(c) : d = -1, c.length && m())
     }
 
     function m() {
-        if (!c) {
+        if (!u) {
             var e = i(f);
-            c = !0;
-            for (var t = u.length; t;) {
-                for (s = u, u = []; ++d < t;) s && s[d].run();
-                d = -1, t = u.length
+            u = !0;
+            for (var t = c.length; t;) {
+                for (s = c, c = []; ++d < t;) s && s[d].run();
+                d = -1, t = c.length
             }
-            s = null, c = !1,
+            s = null, u = !1,
                 function(e) {
                     if (r === clearTimeout) return clearTimeout(e);
                     if ((r === l || !r) && clearTimeout) return r = clearTimeout, clearTimeout(e);
                     try {
                         r(e)
                     } catch (t) {
                         try {
@@ -1868,15 +1872,15 @@
     }
 
     function h() {}
     a.nextTick = function(e) {
         var t = new Array(arguments.length - 1);
         if (arguments.length > 1)
             for (var n = 1; n < arguments.length; n++) t[n - 1] = arguments[n];
-        u.push(new p(e, t)), 1 !== u.length || c || i(m)
+        c.push(new p(e, t)), 1 !== c.length || u || i(m)
     }, p.prototype.run = function() {
         this.fun.apply(null, this.array)
     }, a.title = "browser", a.browser = !0, a.env = {}, a.argv = [], a.version = "", a.versions = {}, a.on = h, a.addListener = h, a.once = h, a.off = h, a.removeListener = h, a.removeAllListeners = h, a.emit = h, a.prependListener = h, a.prependOnceListener = h, a.listeners = function(e) {
         return []
     }, a.binding = function(e) {
         throw new Error("process.binding is not supported")
     }, a.cwd = function() {
@@ -1898,26 +1902,26 @@
      */
     var r = "function" == typeof Symbol && Symbol.for,
         a = r ? Symbol.for("react.element") : 60103,
         o = r ? Symbol.for("react.portal") : 60106,
         l = r ? Symbol.for("react.fragment") : 60107,
         i = r ? Symbol.for("react.strict_mode") : 60108,
         s = r ? Symbol.for("react.profiler") : 60114,
-        u = r ? Symbol.for("react.provider") : 60109,
-        c = r ? Symbol.for("react.context") : 60110,
+        c = r ? Symbol.for("react.provider") : 60109,
+        u = r ? Symbol.for("react.context") : 60110,
         d = r ? Symbol.for("react.async_mode") : 60111,
         f = r ? Symbol.for("react.concurrent_mode") : 60111,
         m = r ? Symbol.for("react.forward_ref") : 60112,
         p = r ? Symbol.for("react.suspense") : 60113,
         h = r ? Symbol.for("react.suspense_list") : 60120,
         g = r ? Symbol.for("react.memo") : 60115,
         v = r ? Symbol.for("react.lazy") : 60116,
         b = r ? Symbol.for("react.block") : 60121,
-        E = r ? Symbol.for("react.fundamental") : 60117,
-        y = r ? Symbol.for("react.responder") : 60118,
+        y = r ? Symbol.for("react.fundamental") : 60117,
+        E = r ? Symbol.for("react.responder") : 60118,
         w = r ? Symbol.for("react.scope") : 60119;
 
     function _(e) {
         if ("object" == typeof e && null !== e) {
             var t = e.$$typeof;
             switch (t) {
                 case a:
@@ -1927,39 +1931,39 @@
                         case l:
                         case s:
                         case i:
                         case p:
                             return e;
                         default:
                             switch (e = e && e.$$typeof) {
-                                case c:
+                                case u:
                                 case m:
                                 case v:
                                 case g:
-                                case u:
+                                case c:
                                     return e;
                                 default:
                                     return t
                             }
                     }
                 case o:
                     return t
             }
         }
     }
 
     function S(e) {
         return _(e) === f
     }
-    t.AsyncMode = d, t.ConcurrentMode = f, t.ContextConsumer = c, t.ContextProvider = u, t.Element = a, t.ForwardRef = m, t.Fragment = l, t.Lazy = v, t.Memo = g, t.Portal = o, t.Profiler = s, t.StrictMode = i, t.Suspense = p, t.isAsyncMode = function(e) {
+    t.AsyncMode = d, t.ConcurrentMode = f, t.ContextConsumer = u, t.ContextProvider = c, t.Element = a, t.ForwardRef = m, t.Fragment = l, t.Lazy = v, t.Memo = g, t.Portal = o, t.Profiler = s, t.StrictMode = i, t.Suspense = p, t.isAsyncMode = function(e) {
         return S(e) || _(e) === d
     }, t.isConcurrentMode = S, t.isContextConsumer = function(e) {
-        return _(e) === c
-    }, t.isContextProvider = function(e) {
         return _(e) === u
+    }, t.isContextProvider = function(e) {
+        return _(e) === c
     }, t.isElement = function(e) {
         return "object" == typeof e && null !== e && e.$$typeof === a
     }, t.isForwardRef = function(e) {
         return _(e) === m
     }, t.isFragment = function(e) {
         return _(e) === l
     }, t.isLazy = function(e) {
@@ -1971,15 +1975,15 @@
     }, t.isProfiler = function(e) {
         return _(e) === s
     }, t.isStrictMode = function(e) {
         return _(e) === i
     }, t.isSuspense = function(e) {
         return _(e) === p
     }, t.isValidElementType = function(e) {
-        return "string" == typeof e || "function" == typeof e || e === l || e === f || e === s || e === i || e === p || e === h || "object" == typeof e && null !== e && (e.$$typeof === v || e.$$typeof === g || e.$$typeof === u || e.$$typeof === c || e.$$typeof === m || e.$$typeof === E || e.$$typeof === y || e.$$typeof === w || e.$$typeof === b)
+        return "string" == typeof e || "function" == typeof e || e === l || e === f || e === s || e === i || e === p || e === h || "object" == typeof e && null !== e && (e.$$typeof === v || e.$$typeof === g || e.$$typeof === c || e.$$typeof === u || e.$$typeof === m || e.$$typeof === y || e.$$typeof === E || e.$$typeof === w || e.$$typeof === b)
     }, t.typeOf = _
 }, function(e, t, n) {
     "use strict";
     var r = this && this.__makeTemplateObject || function(e, t) {
             return Object.defineProperty ? Object.defineProperty(e, "raw", {
                 value: t
             }) : e.raw = t, e
@@ -2026,20 +2030,20 @@
             value: a
         }, o.default.createElement("section", {
             "aria-labelledby": "tab-label-" + a,
             id: "tab-" + a,
             role: "tabpanel"
         }, n))))
     };
-    var s, u = l.default.section(s || (s = r(["\n    padding-top: 0 !important;\n"], ["\n    padding-top: 0 !important;\n"])));
+    var s, c = l.default.section(s || (s = r(["\n    padding-top: 0 !important;\n"], ["\n    padding-top: 0 !important;\n"])));
     t.TabContent = function(e) {
         var t = e.slug,
             n = e.children,
             r = o.default.useContext(i);
-        return o.default.createElement(u, {
+        return o.default.createElement(c, {
             id: "tab-" + t,
             className: t === r ? "active" : "",
             hidden: t !== r
         }, n)
     }
 }, function(e, t, n) {
     "use strict";
@@ -2058,38 +2062,38 @@
                 l = e.targetLocale,
                 i = n.filter((function(e) {
                     return e.locale.code == r.code
                 })).pop(),
                 s = i && i.editUrl ? a.default.createElement("a", {
                     href: i.editUrl
                 }, r.displayName) : a.default.createElement(a.default.Fragment, null, r.displayName),
-                u = a.default.createElement(a.default.Fragment, null),
-                c = n.filter((function(e) {
+                c = a.default.createElement(a.default.Fragment, null),
+                u = n.filter((function(e) {
                     return e.locale.code != r.code
                 })).map((function(e) {
                     var t = e.locale,
                         n = e.editUrl;
                     return {
                         label: t.displayName,
                         href: n
                     }
                 }));
-            if (c.length > 0) {
-                var d = c.map((function(e) {
+            if (u.length > 0) {
+                var d = u.map((function(e) {
                     var t = e.label,
                         n = e.href;
                     return a.default.createElement("li", {
                         className: "c-dropdown__item "
                     }, a.default.createElement("a", {
                         href: n,
                         "aria-label": "",
                         className: "u-link is-live"
                     }, t))
                 }));
-                u = a.default.createElement("div", {
+                c = a.default.createElement("div", {
                     className: "c-dropdown t-inverted",
                     "data-dropdown": "",
                     style: {
                         display: "inline-block"
                     }
                 }, a.default.createElement("a", {
                     href: "javascript:void(0)",
@@ -2105,32 +2109,32 @@
                 }), a.default.createElement(o.default, {
                     name: "arrow-up"
                 }))), a.default.createElement("div", {
                     className: "t-dark"
                 }, a.default.createElement("ul", {
                     className: "c-dropdown__menu u-toggle  u-arrow u-arrow--tl u-background"
                 }, d)))
-            } else u = a.default.createElement(a.default.Fragment, null, l.displayName);
+            } else c = a.default.createElement(a.default.Fragment, null, l.displayName);
             return a.default.createElement("div", {
                 className: "w-p-4 header-meta--" + t + " w-flex w-flex-row w-items-center"
             }, s, a.default.createElement("svg", {
                 "aria-hidden": "true",
                 className: "icon icon-arrow-right w-w-4 w-h-4"
             }, a.default.createElement("use", {
                 href: "#icon-arrow-right"
-            })), u)
+            })), c)
         };
     t.default = function(e) {
         var t = e.sourceLocale,
             n = e.locale,
             r = e.translations;
         return a.default.createElement("header", {
-            className: "w-flex w-flex-col sm:w-flex-row w-items-center w-justify-between w-bg-grey-50 w-border-b w-border-grey-100 w-px-0 w-py-0 w-mb-0 w-relative w-top-0 sm:w-sticky w-min-h-slim-header"
+            className: "w-flex w-flex-col sm:w-flex-row w-items-center w-justify-between w-bg-surface-header w-border-b w-border-border-furniture w-px-0 w-py-0 w-mb-0 w-relative w-top-0 sm:w-sticky w-min-h-slim-header"
         }, a.default.createElement("div", {
-            className: "w-pl-slim-header w-min-h-slim-header sm:w-pl-0 sm:w-pr-2 w-w-full w-flex-1 w-overflow-x-auto w-box-border"
+            className: "w-pl-slim-header w-min-h-slim-header sm:w-pl-5 sm:w-pr-2 w-w-full w-flex-1 w-overflow-x-auto w-box-border"
         }, a.default.createElement("div", {
             className: "w-flex w-flex-1 w-items-center w-overflow-hidden w-h-slim-header"
         }, a.default.createElement(l, {
             key: "locales",
             name: "locales",
             translations: r,
             sourceLocale: t,
@@ -2150,16 +2154,16 @@
         l = r(n(2)),
         i = r(n(21));
     t.default = function(e) {
         var t = e.csrfToken,
             n = e.object.isLocked,
             r = e.perms,
             s = e.links,
-            u = e.previewModes,
-            c = e.locale,
+            c = e.previewModes,
+            u = e.locale,
             d = [a.default.createElement("form", {
                 method: "POST",
                 action: s.stopTranslationUrl
             }, a.default.createElement("input", {
                 type: "hidden",
                 name: "csrfmiddlewaretoken",
                 value: t
@@ -2226,15 +2230,15 @@
             "aria-label": o.default("Remove editor lock")
         }, a.default.createElement(l.default, {
             name: "lock-open"
         }), o.default("Unlock")))), r.canUnpublish && d.push(a.default.createElement("a", {
             className: "button action-secondary",
             href: s.unpublishUrl
         }, a.default.createElement(l.default, {
-            name: "download-alt"
+            name: "download"
         }), o.default("Unpublish"))), r.canPublish && d.push(a.default.createElement("form", {
             method: "POST"
         }, a.default.createElement("input", {
             type: "hidden",
             name: "csrfmiddlewaretoken",
             value: t
         }), a.default.createElement("input", {
@@ -2242,30 +2246,33 @@
             name: "next",
             value: window.location.href
         }), a.default.createElement("button", {
             type: "submit",
             name: "action",
             value: "publish",
             className: "button button-longrunning ",
-            "data-clicked-text": o.default("Publishing...")
+            "data-clicked-text": o.default("Publishing..."),
+            "data-controller": "w-progress",
+            "data-action": "w-progress#activate",
+            "data-w-progress-active-value": o.default("Publishing...")
         }, a.default.createElement(l.default, {
             name: "upload",
             className: "button-longrunning__icon"
         }), a.default.createElement(l.default, {
             name: "spinner"
-        }), a.default.createElement("em", null, o.default("Publish in ") + c.displayName))));
+        }), a.default.createElement("em", null, o.default("Publish in ") + u.displayName))));
         var f = d.pop();
         return a.default.createElement("footer", {
             className: "footer"
         }, a.default.createElement("ul", null, a.default.createElement("li", {
             className: "footer__container"
         }, a.default.createElement(i.default, {
             defaultAction: f,
             actions: d,
-            previewModes: u
+            previewModes: c
         }))))
     }
 }, function(e, t, n) {
     "use strict";
     var r = this && this.__importDefault || function(e) {
         return e && e.__esModule ? e : {
             default: e
@@ -2384,16 +2391,16 @@
             }
         };
     t.__esModule = !0, t.BlockLabel = void 0;
     var o = a(n(0)),
         l = a(n(3)),
         i = a(n(1)),
         s = a(n(2)),
-        u = a(n(23)),
-        c = a(n(24)),
+        c = a(n(23)),
+        u = a(n(24)),
         d = a(n(25)),
         f = a(n(26)),
         m = a(n(27)),
         p = n(7);
 
     function h(e, t, n, r) {
         r({
@@ -2444,38 +2451,38 @@
                 },
                 onKeyDown: function(e) {
                     "Enter" == e.key && r && (e.preventDefault(), r())
                 },
                 value: t
             })
         };
-    t.BlockLabel = l.default.h3(E || (E = r(["\n    color: var(--w-color-secondary-100);\n    border: 1px solid #f5f5f5;\n    padding-left: 11px;\n    padding-right: 11px;\n    padding-top: 7px;\n    padding-bottom: 9px;\n    display: inline-block;\n    margin-bottom: 0;\n    font-weight: bold;\n"], ["\n    color: var(--w-color-secondary-100);\n    border: 1px solid #f5f5f5;\n    padding-left: 11px;\n    padding-right: 11px;\n    padding-top: 7px;\n    padding-bottom: 9px;\n    display: inline-block;\n    margin-bottom: 0;\n    font-weight: bold;\n"])));
-    var b, E, y, w, _, S, k, x, O, A = l.default.ul(y || (y = r(["\n    list-style-type: none;\n    border: 1px solid #eeeeee;\n    background-color: #f1f1f1;\n    padding: 0;\n    margin: 0;\n\n    > li {\n        &.errored {\n            background-color: #fee7e8;\n            // !important required to override the border-bottom rule just below\n            border: 1px solid var(--w-color-critical-100) !important;\n        }\n\n        &.incomplete {\n            // !important required to override the border-bottom rule just below\n            border-left: 5px solid var(--w-color-warning-100) !important;\n        }\n\n        &.complete {\n            // !important required to override the border-bottom rule just below\n            border-left: 5px solid var(--w-color-positive-100) !important;\n        }\n\n        &:not(:last-child) {\n            border-bottom: 1px solid #eaeaea;\n        }\n\n        &:after {\n            content: '';\n            display: table;\n            clear: both;\n        }\n    }\n"], ["\n    list-style-type: none;\n    border: 1px solid #eeeeee;\n    background-color: #f1f1f1;\n    padding: 0;\n    margin: 0;\n\n    > li {\n        &.errored {\n            background-color: #fee7e8;\n            // !important required to override the border-bottom rule just below\n            border: 1px solid var(--w-color-critical-100) !important;\n        }\n\n        &.incomplete {\n            // !important required to override the border-bottom rule just below\n            border-left: 5px solid var(--w-color-warning-100) !important;\n        }\n\n        &.complete {\n            // !important required to override the border-bottom rule just below\n            border-left: 5px solid var(--w-color-positive-100) !important;\n        }\n\n        &:not(:last-child) {\n            border-bottom: 1px solid #eaeaea;\n        }\n\n        &:after {\n            content: '';\n            display: table;\n            clear: both;\n        }\n    }\n"]))),
-        C = l.default.h4(w || (w = r(["\n    margin: 0;\n    padding: 15px 20px;\n    background-color: var(--w-color-secondary-50);\n    font-style: normal;\n    font-weight: bold;\n    padding-left: 20px;\n"], ["\n    margin: 0;\n    padding: 15px 20px;\n    background-color: var(--w-color-secondary-50);\n    font-style: normal;\n    font-weight: bold;\n    padding-left: 20px;\n"]))),
-        T = l.default.p(_ || (_ = r(["\n    padding: 15px 20px;\n    font-style: italic;\n\n    &.title {\n        color: var(--w-color-grey-600);\n        font-size: 1.875rem;\n        font-weight: 800;\n        line-height: 1.3;\n    }\n"], ["\n    padding: 15px 20px;\n    font-style: italic;\n\n    &.title {\n        color: var(--w-color-grey-600);\n        font-size: 1.875rem;\n        font-weight: 800;\n        line-height: 1.3;\n    }\n"]))),
+    t.BlockLabel = l.default.h3(y || (y = r(["\n    border: 1px solid\n        var(--w-color-border-furniture, var(--w-color-secondary-100));\n    border-bottom: none;\n    color: var(\n        --w-color-surface-alert-information,\n        var(--w-color-secondary-100)\n    );\n    padding-left: 11px;\n    padding-right: 11px;\n    padding-top: 7px;\n    padding-bottom: 9px;\n    display: inline-block;\n    margin-bottom: 0;\n    font-weight: bold;\n"], ["\n    border: 1px solid\n        var(--w-color-border-furniture, var(--w-color-secondary-100));\n    border-bottom: none;\n    color: var(\n        --w-color-surface-alert-information,\n        var(--w-color-secondary-100)\n    );\n    padding-left: 11px;\n    padding-right: 11px;\n    padding-top: 7px;\n    padding-bottom: 9px;\n    display: inline-block;\n    margin-bottom: 0;\n    font-weight: bold;\n"])));
+    var b, y, E, w, _, S, k, x, O, A = l.default.ul(E || (E = r(["\n    list-style-type: none;\n    border: 1px solid var(--w-color-border-furniture, var(--w-color-grey-100));\n    background-color: var(--w-color-surface-header, var(--w-color-grey-50));\n    padding: 0;\n    margin: 0;\n\n    > li {\n        &.errored {\n            background-color: var(--w-color-critical-50, #fee7e8);\n            color: var(--w-color-text-error, var(--w-color-grey-600));\n            // !important required to override the border-bottom rule just below\n            border: 1px solid var(--w-color-critical-100) !important;\n            border-left-width: 5px !important;\n        }\n\n        &.incomplete {\n            // !important required to override the border-bottom rule just below\n            border-left: 5px solid var(--w-color-warning-100) !important;\n        }\n\n        &.complete {\n            // !important required to override the border-bottom rule just below\n            border-left: 5px solid var(--w-color-positive-100) !important;\n        }\n\n        &:not(:last-child) {\n            border-bottom: 1px solid var(--w-color-border-furniture, #eeeeee);\n        }\n\n        &:after {\n            content: '';\n            display: table;\n            clear: both;\n        }\n    }\n"], ["\n    list-style-type: none;\n    border: 1px solid var(--w-color-border-furniture, var(--w-color-grey-100));\n    background-color: var(--w-color-surface-header, var(--w-color-grey-50));\n    padding: 0;\n    margin: 0;\n\n    > li {\n        &.errored {\n            background-color: var(--w-color-critical-50, #fee7e8);\n            color: var(--w-color-text-error, var(--w-color-grey-600));\n            // !important required to override the border-bottom rule just below\n            border: 1px solid var(--w-color-critical-100) !important;\n            border-left-width: 5px !important;\n        }\n\n        &.incomplete {\n            // !important required to override the border-bottom rule just below\n            border-left: 5px solid var(--w-color-warning-100) !important;\n        }\n\n        &.complete {\n            // !important required to override the border-bottom rule just below\n            border-left: 5px solid var(--w-color-positive-100) !important;\n        }\n\n        &:not(:last-child) {\n            border-bottom: 1px solid var(--w-color-border-furniture, #eeeeee);\n        }\n\n        &:after {\n            content: '';\n            display: table;\n            clear: both;\n        }\n    }\n"]))),
+        C = l.default.h4(w || (w = r(["\n    margin: 0;\n    padding: 15px 20px;\n    background-color: var(\n        --w-color-surface-panel-information,\n        var(--w-color-secondary-50)\n    );\n    color: var(--w-text-surface-panel-information, var(--w-color-secondary));\n    font-style: normal;\n    font-weight: bold;\n    padding-left: 20px;\n"], ["\n    margin: 0;\n    padding: 15px 20px;\n    background-color: var(\n        --w-color-surface-panel-information,\n        var(--w-color-secondary-50)\n    );\n    color: var(--w-text-surface-panel-information, var(--w-color-secondary));\n    font-style: normal;\n    font-weight: bold;\n    padding-left: 20px;\n"]))),
+        T = l.default.p(_ || (_ = r(["\n    padding: 15px 20px;\n    font-style: italic;\n\n    &.title {\n        font-size: 1.875rem;\n        font-weight: 800;\n        line-height: 1.3;\n    }\n"], ["\n    padding: 15px 20px;\n    font-style: italic;\n\n    &.title {\n        font-size: 1.875rem;\n        font-weight: 800;\n        line-height: 1.3;\n    }\n"]))),
         R = l.default.div(S || (S = r(["\n    padding: 0.9em 1.2em;\n\n    > p,\n    > ", " {\n        font-size: 1.2em;\n        font-style: italic;\n        line-height: 1.5em;\n        font-style: italic;\n        font-weight: 600;\n    }\n"], ["\n    padding: 0.9em 1.2em;\n\n    > p,\n    > ", " {\n        font-size: 1.2em;\n        font-style: italic;\n        line-height: 1.5em;\n        font-style: italic;\n        font-weight: 600;\n    }\n"])), g),
-        N = l.default.button(k || (k = r(["\n    font-size: 0.8em;\n    font-weight: bold;\n    color: var(--w-color-secondary);\n    background-color: var(--w-color-secondary-50);\n    border: 2px solid var(--w-color-secondary-100);\n    border-radius: 2px;\n    padding: 5px 10px;\n\n    &:hover {\n        background-color: var(--w-color-secondary-75);\n    }\n"], ["\n    font-size: 0.8em;\n    font-weight: bold;\n    color: var(--w-color-secondary);\n    background-color: var(--w-color-secondary-50);\n    border: 2px solid var(--w-color-secondary-100);\n    border-radius: 2px;\n    padding: 5px 10px;\n\n    &:hover {\n        background-color: var(--w-color-secondary-75);\n    }\n"]))),
+        N = l.default.button(k || (k = r(["\n    font-size: 0.8em;\n    font-weight: bold;\n    color: var(--w-color-text-button, var(--w-color-secondary));\n    background-color: var(\n        --w-color-surface-button-default,\n        var(--w-color-secondary-50)\n    );\n    border: 1px solid\n        var(--w-color-surface-button-default, var(--w-color-secondary-100));\n    border-radius: 2px;\n    padding: 5px 10px;\n\n    &:hover {\n        background-color: var(\n            --w-color-surface-button-hover,\n            var(--w-color-secondary-75)\n        );\n    }\n"], ["\n    font-size: 0.8em;\n    font-weight: bold;\n    color: var(--w-color-text-button, var(--w-color-secondary));\n    background-color: var(\n        --w-color-surface-button-default,\n        var(--w-color-secondary-50)\n    );\n    border: 1px solid\n        var(--w-color-surface-button-default, var(--w-color-secondary-100));\n    border-radius: 2px;\n    padding: 5px 10px;\n\n    &:hover {\n        background-color: var(\n            --w-color-surface-button-hover,\n            var(--w-color-secondary-75)\n        );\n    }\n"]))),
         I = l.default.ul(x || (x = r(["\n    box-sizing: border-box;\n    width: 100%;\n    text-align: right;\n    padding: 10px;\n    margin: 0;\n\n    > li {\n        display: inline-block;\n\n        &:not(:first-child) {\n            margin-left: 15px;\n        }\n    }\n\n    .icon {\n        width: 1.3em;\n        height: 1.3em;\n        vertical-align: text-bottom;\n        margin-left: 10px;\n\n        &--green {\n            color: #15704d;\n        }\n\n        &--red {\n            color: #cd3239;\n        }\n    }\n"], ["\n    box-sizing: border-box;\n    width: 100%;\n    text-align: right;\n    padding: 10px;\n    margin: 0;\n\n    > li {\n        display: inline-block;\n\n        &:not(:first-child) {\n            margin-left: 15px;\n        }\n    }\n\n    .icon {\n        width: 1.3em;\n        height: 1.3em;\n        vertical-align: text-bottom;\n        margin-left: 10px;\n\n        &--green {\n            color: #15704d;\n        }\n\n        &--red {\n            color: #cd3239;\n        }\n    }\n"]))),
-        D = l.default.ul(O || (O = r(["\n    list-style-type: none;\n    max-width: 1200px;\n    padding-left: 20px;\n    padding-right: 20px;\n\n    @media screen and (min-width: 800px) {\n        padding-left: 80px;\n        padding-right: 80px;\n    }\n"], ["\n    list-style-type: none;\n    max-width: 1200px;\n    padding-left: 20px;\n    padding-right: 20px;\n\n    @media screen and (min-width: 800px) {\n        padding-left: 80px;\n        padding-right: 80px;\n    }\n"]))),
+        D = l.default.ul(O || (O = r(["\n    list-style-type: none;\n    max-width: 1200px;\n    padding-left: 0;\n"], ["\n    list-style-type: none;\n    max-width: 1200px;\n    padding-left: 0;\n"]))),
         P = function(e) {
             var t = e.segment,
                 n = e.translation,
                 r = e.isLocked,
                 a = e.isEditing,
                 l = e.setIsEditing,
-                c = e.dispatch,
+                u = e.dispatch,
                 d = e.csrfToken,
                 f = o.default.useState(n && n.value || ""),
                 m = f[0],
                 h = f[1],
                 g = o.default.createElement(o.default.Fragment, null),
                 b = [],
-                E = o.default.createElement(o.default.Fragment, null);
+                y = o.default.createElement(o.default.Fragment, null);
             if (a && !r) {
-                var y = function() {
+                var E = function() {
                     l(!1),
                         function(e, t, n, r) {
                             if (r({
                                     type: p.EDIT_STRING_TRANSLATION,
                                     segmentId: e.id,
                                     value: t
                                 }), t) {
@@ -2513,95 +2520,95 @@
                                     type: p.TRANSLATION_DELETED,
                                     segmentId: e.id
                                 }) : r({
                                     type: p.TRANSLATION_SAVE_SERVER_ERROR,
                                     segmentId: e.id
                                 })
                             }))
-                        }(t, m, d, c)
+                        }(t, m, d, u)
                 };
                 b = [o.default.createElement("li", {
                     key: "cancel"
                 }, o.default.createElement(N, {
                     onClick: function() {
                         l(!1)
                     }
                 }, i.default("Cancel"))), o.default.createElement("li", {
                     key: "save"
                 }, o.default.createElement(N, {
-                    onClick: y
-                }, i.default("Save")))], E = o.default.createElement(v, {
+                    onClick: E
+                }, i.default("Save")))], y = o.default.createElement(v, {
                     onChange: h,
-                    onHitEnter: y,
+                    onHitEnter: E,
                     value: m,
                     focusOnMount: !0
                 })
             } else if (n && n.isSaving) g = o.default.createElement(o.default.Fragment, null, i.default("Saving..."), " ", o.default.createElement(s.default, {
                 name: "spinner"
-            })), E = o.default.createElement("p", null, n && n.value);
+            })), y = o.default.createElement("p", null, n && n.value);
             else {
                 n && n.comment && (g = o.default.createElement(o.default.Fragment, null, n.comment, n.isErrored ? o.default.createElement(s.default, {
                     name: "warning",
                     className: "icon--red"
                 }) : o.default.createElement(s.default, {
-                    name: "tick",
+                    name: "check",
                     className: "icon--green"
-                })), n.translatedBy && n.translatedBy.avatar_url && (g = o.default.createElement(o.default.Fragment, null, o.default.createElement(u.default, {
+                })), n.translatedBy && n.translatedBy.avatar_url && (g = o.default.createElement(o.default.Fragment, null, o.default.createElement(c.default, {
                     username: n.translatedBy.full_name,
                     avatarUrl: n.translatedBy.avatar_url
                 }), g))), r || b.push(o.default.createElement("li", {
                     key: "edit"
                 }, o.default.createElement(N, {
                     onClick: function() {
                         l(!0), h(n && n.value || "")
                     }
-                }, n ? i.default("Edit") : i.default("Translate")))), E = o.default.createElement("p", null, n && n.value)
+                }, n ? i.default("Edit") : i.default("Translate")))), y = o.default.createElement("p", null, n && n.value)
             }
             var w = "complete";
             n ? n.isErrored && (w = "errored") : w = "incomplete";
             var _ = "";
             return "title" === t.contentPath && (_ = "title"), o.default.createElement("li", {
                 className: w
             }, t.location.subField && o.default.createElement(C, null, t.location.subField), o.default.createElement(T, {
                 className: _
-            }, t.source), o.default.createElement(R, null, E), o.default.createElement(I, null, o.default.createElement("li", {
+            }, t.source), o.default.createElement(R, null, y), o.default.createElement(I, null, o.default.createElement("li", {
                 key: "comment"
             }, g), b))
         },
         j = function(e) {
             var t = e.adminBaseUrl,
                 n = e.segment,
                 r = e.override,
                 a = e.sourceLocale,
                 l = e.isLocked,
-                u = e.isEditing,
+                c = e.isEditing,
                 g = e.setIsEditing,
                 b = e.dispatch,
-                E = e.csrfToken,
-                y = o.default.createElement(o.default.Fragment, null),
+                y = e.csrfToken,
+                E = o.default.createElement(o.default.Fragment, null),
                 w = [],
                 _ = o.default.createElement(o.default.Fragment, null);
-            y = r ? o.default.createElement(o.default.Fragment, null, r.comment, r.isErrored ? o.default.createElement(s.default, {
+            E = r ? o.default.createElement(o.default.Fragment, null, r.comment, r.isErrored ? o.default.createElement(s.default, {
                 name: "warning",
                 className: "icon--red"
             }) : o.default.createElement(s.default, {
-                name: "tick",
+                name: "check",
                 className: "icon--green"
             })) : o.default.createElement(o.default.Fragment, null, i.default("Uses %s version").replace("%s", a.displayName), " ", o.default.createElement(s.default, {
-                name: "tick",
+                name: "check",
                 className: "icon--green"
             }));
             var S = n.location.widget;
             if ("text" == S.type) {
                 var k = o.default.useState(r && r.value || n.value),
                     x = k[0],
                     O = k[1];
-                if (u && !l) {
+                if (c && !l) {
                     var A = function() {
-                        g(!1), h(n, x, E, b)
+                        g(!1), h(n, x, y, b)
                     };
                     w = [o.default.createElement(N, {
                         onClick: function() {
                             g(!1)
                         }
                     }, i.default("Cancel")), o.default.createElement(N, {
                         onClick: A
@@ -2625,32 +2632,32 @@
                             url: window.chooserUrls.pageChooser,
                             urlParams: {
                                 page_type: S.allowed_page_types.join(",")
                             },
                             onload: window.PAGE_CHOOSER_MODAL_ONLOAD_HANDLERS,
                             responses: {
                                 pageChosen: function(e) {
-                                    h(n, e.id, E, b)
+                                    h(n, e.id, y, b)
                                 }
                             }
                         })
                     }
-                }, i.default("Change page"))), _ = o.default.createElement(c.default, {
+                }, i.default("Change page"))), _ = o.default.createElement(u.default, {
                     adminBaseUrl: t,
                     pageId: r && r.value || n.value
                 })
             } else if ("image_chooser" == S.type) {
                 l || w.push(o.default.createElement(N, {
                     onClick: function() {
                         window.ModalWorkflow({
                             url: window.chooserUrls.imageChooser,
                             onload: window.IMAGE_CHOOSER_MODAL_ONLOAD_HANDLERS,
                             responses: {
                                 chosen: function(e) {
-                                    h(n, e.id, E, b)
+                                    h(n, e.id, y, b)
                                 }
                             }
                         })
                     }
                 }, i.default("Change image"))), _ = o.default.createElement(d.default, {
                     adminBaseUrl: t,
                     imageId: r && r.value || n.value
@@ -2659,15 +2666,15 @@
                 l || w.push(o.default.createElement(N, {
                     onClick: function() {
                         window.ModalWorkflow({
                             url: window.chooserUrls.documentChooser,
                             onload: window.DOCUMENT_CHOOSER_MODAL_ONLOAD_HANDLERS,
                             responses: {
                                 chosen: function(e) {
-                                    h(n, e.id, E, b)
+                                    h(n, e.id, y, b)
                                 }
                             }
                         })
                     }
                 }, i.default("Change document"))), _ = o.default.createElement(f.default, {
                     adminBaseUrl: t,
                     documentId: r && r.value || n.value
@@ -2676,15 +2683,15 @@
                 l || w.push(o.default.createElement(N, {
                     onClick: function() {
                         window.ModalWorkflow({
                             url: S.chooser_url,
                             onload: window.SNIPPET_CHOOSER_MODAL_ONLOAD_HANDLERS,
                             responses: {
                                 snippetChosen: function(e) {
-                                    h(n, e.id, E, b)
+                                    h(n, e.id, y, b)
                                 }
                             }
                         })
                     }
                 }, i.default("Change %s").replace("%s", S.snippet_model.verbose_name))), _ = o.default.createElement(m.default, {
                     adminBaseUrl: t,
                     snippetModel: S.snippet_model,
@@ -2709,33 +2716,33 @@
                                     type: p.OVERRIDE_DELETED,
                                     segmentId: e.id
                                 }) : n({
                                     type: p.OVERRIDE_SAVE_SERVER_ERROR,
                                     segmentId: e.id
                                 })
                             }))
-                        }(n, E, b)
+                        }(n, y, b)
                     }
                 }, i.default("Revert to %s version").replace("%s", a.displayName)))
             }
             var T = "";
             return r && r.isErrored && (T = "errored"), o.default.createElement("li", {
                 className: T
-            }, n.location.subField && o.default.createElement(C, null, n.location.subField), o.default.createElement(R, null, _), o.default.createElement(I, null, o.default.createElement("li", null, y), w.map((function(e) {
+            }, n.location.subField && o.default.createElement(C, null, n.location.subField), o.default.createElement(R, null, _), o.default.createElement(I, null, o.default.createElement("li", null, E), w.map((function(e) {
                 return o.default.createElement("li", null, e)
             }))))
         },
         M = function(e) {
             var t = e.segment,
                 n = o.default.createElement(o.default.Fragment, null);
             return n = t.dest ? null !== t.translationProgress ? o.default.createElement(o.default.Fragment, null, t.translationProgress.translatedSegments, " /", " ", t.translationProgress.totalSegments, " ", i.default("segments translated"), t.translationProgress.translatedSegments == t.translationProgress.totalSegments && o.default.createElement(s.default, {
-                name: "tick",
+                name: "check",
                 className: "icon--green"
             })) : o.default.createElement(s.default, {
-                name: "tick",
+                name: "check",
                 className: "icon--green"
             }) : o.default.createElement(o.default.Fragment, null, i.default("Not translated"), " ", o.default.createElement(s.default, {
                 name: "warning",
                 className: "icon--red"
             })), o.default.createElement("li", null, t.location.subField && o.default.createElement(C, null, t.location.subField), o.default.createElement(R, null, o.default.createElement("p", null, t.source ? t.source.title : i.default("[DELETED]"))), o.default.createElement(I, null, o.default.createElement("li", null, n), o.default.createElement("li", null, t.dest && t.dest.editUrl && o.default.createElement(N, {
                 onClick: function() {
                     t.dest && window.open(t.dest.editUrl)
@@ -2749,60 +2756,60 @@
     t.default = function(e) {
         var n = e.adminBaseUrl,
             r = e.object.isLocked,
             a = e.sourceLocale,
             l = e.segments,
             i = e.stringTranslations,
             s = e.segmentOverrides,
-            u = e.editingSegments,
-            c = e.dispatch,
+            c = e.editingSegments,
+            u = e.dispatch,
             d = e.csrfToken,
             f = new Map;
         l.forEach((function(e) {
             var t = e.location.field + "/" + (e.location.blockId || "null"),
                 n = f.get(t);
             n || (n = [], f.set(t, n)), n.push(e)
         }));
         var m = Array.from(f.entries()).map((function(e) {
             var l = e[0],
                 f = e[1],
                 m = function(e, t) {
-                    c({
+                    u({
                         type: "set-editing-mode",
                         segmentId: e,
                         editing: t
                     })
                 },
                 p = f.map((function(e) {
                     switch (e.type) {
                         case "string":
                             return o.default.createElement(P, {
                                 key: e.id,
                                 segment: e,
                                 translation: i.get(e.id),
                                 isLocked: r,
-                                isEditing: u.has(e.id),
+                                isEditing: c.has(e.id),
                                 setIsEditing: function(t) {
                                     return m(e.id, t)
                                 },
-                                dispatch: c,
+                                dispatch: u,
                                 csrfToken: d
                             });
                         case "synchronised_value":
                             return o.default.createElement(j, {
                                 adminBaseUrl: n,
                                 segment: e,
                                 override: s.get(e.id),
                                 sourceLocale: a,
                                 isLocked: r,
-                                isEditing: u.has(e.id),
+                                isEditing: c.has(e.id),
                                 setIsEditing: function(t) {
                                     return m(e.id, t)
                                 },
-                                dispatch: c,
+                                dispatch: u,
                                 csrfToken: d
                             });
                         case "related_object":
                             return o.default.createElement(M, {
                                 segment: e
                             })
                     }
@@ -2860,36 +2867,36 @@
             l = r[0],
             i = r[1];
         a.default.useEffect((function() {
             i(null), n && fetch(t + "api/main/pages/" + n + "/").then((function(e) {
                 return e.json()
             })).then(i)
         }), [n]);
-        var s, u = ["chooser", "page-chooser"];
+        var s, c = ["chooser", "page-chooser"];
         return n ? s = l ? a.default.createElement("div", {
             className: "chosen"
         }, a.default.createElement("span", {
             className: "title"
         }, l.title), a.default.createElement("ul", {
             className: "actions",
             style: {
                 listStyleType: "none"
             }
         }, a.default.createElement("li", null, a.default.createElement("a", {
             href: t + "pages/" + l.id + "/edit/",
             className: "edit-link button button-small button-secondary",
             target: "_blank",
             rel: "noopener noreferrer"
-        }, o.default("Edit this page"))))) : a.default.createElement("p", null, o.default("Fetching page information...")) : (u.push("blank"), s = a.default.createElement("div", {
+        }, o.default("Edit this page"))))) : a.default.createElement("p", null, o.default("Fetching page information...")) : (c.push("blank"), s = a.default.createElement("div", {
             className: "unchosen"
         }, a.default.createElement("button", {
             type: "button",
             className: "button action-choose button-small button-secondary"
         }, o.default("Choose a page")))), a.default.createElement("div", {
-            className: u.join(" ")
+            className: c.join(" ")
         }, s)
     }
 }, function(e, t, n) {
     "use strict";
     var r = this && this.__importDefault || function(e) {
         return e && e.__esModule ? e : {
             default: e
@@ -2905,15 +2912,15 @@
             l = r[0],
             i = r[1];
         a.default.useEffect((function() {
             i(null), n && fetch(t + "api/main/images/" + n + "/").then((function(e) {
                 return e.json()
             })).then(i)
         }), [n]);
-        var s, u = ["chooser", "image-chooser"];
+        var s, c = ["chooser", "image-chooser"];
         return n ? s = l ? a.default.createElement("div", {
             className: "chosen"
         }, a.default.createElement("div", {
             className: "preview-image"
         }, a.default.createElement("img", {
             alt: l.title,
             className: "show-transparency",
@@ -2927,21 +2934,21 @@
                 listStyleType: "none"
             }
         }, a.default.createElement("li", null, a.default.createElement("a", {
             href: t + "images/" + l.id + "/",
             className: "edit-link button button-small button-secondary",
             target: "_blank",
             rel: "noopener noreferrer"
-        }, o.default("Edit this image"))))) : a.default.createElement("p", null, o.default("Fetching image information...")) : (u.push("blank"), s = a.default.createElement("div", {
+        }, o.default("Edit this image"))))) : a.default.createElement("p", null, o.default("Fetching image information...")) : (c.push("blank"), s = a.default.createElement("div", {
             className: "unchosen"
         }, a.default.createElement("button", {
             type: "button",
             className: "button action-choose button-small button-secondary"
         }, o.default("Choose an image")))), a.default.createElement("div", {
-            className: u.join(" ")
+            className: c.join(" ")
         }, s)
     }
 }, function(e, t, n) {
     "use strict";
     var r = this && this.__importDefault || function(e) {
         return e && e.__esModule ? e : {
             default: e
@@ -2957,36 +2964,36 @@
             l = r[0],
             i = r[1];
         a.default.useEffect((function() {
             i(null), n && fetch(t + "api/main/documents/" + n + "/").then((function(e) {
                 return e.json()
             })).then(i)
         }), [n]);
-        var s, u = ["chooser", "document-chooser"];
+        var s, c = ["chooser", "document-chooser"];
         return n ? s = l ? a.default.createElement("div", {
             className: "chosen"
         }, a.default.createElement("span", {
             className: "title"
         }, l.title), a.default.createElement("ul", {
             className: "actions",
             style: {
                 listStyleType: "none"
             }
         }, a.default.createElement("li", null, a.default.createElement("a", {
             href: t + "documents/edit/" + l.id + "/",
             className: "edit-link button button-small button-secondary",
             target: "_blank",
             rel: "noopener noreferrer"
-        }, o.default("Edit this document"))))) : a.default.createElement("p", null, o.default("Fetching document information...")) : (u.push("blank"), s = a.default.createElement("div", {
+        }, o.default("Edit this document"))))) : a.default.createElement("p", null, o.default("Fetching document information...")) : (c.push("blank"), s = a.default.createElement("div", {
             className: "unchosen"
         }, a.default.createElement("button", {
             type: "button",
             className: "button action-choose button-small button-secondary"
         }, o.default("Choose a document")))), a.default.createElement("div", {
-            className: u.join(" ")
+            className: c.join(" ")
         }, s)
     }
 }, function(e, t, n) {
     "use strict";
     var r = this && this.__importDefault || function(e) {
         return e && e.__esModule ? e : {
             default: e
@@ -3003,127 +3010,127 @@
             i = l[0],
             s = l[1];
         a.default.useEffect((function() {
             s(null), r && fetch(t + "localize/api/snippets/" + n.app_label + "/" + n.model_name + "/" + r + "/").then((function(e) {
                 return e.json()
             })).then(s)
         }), [r]);
-        var u, c = ["chooser", "snippet-chooser"];
-        return r ? u = i ? a.default.createElement("div", {
+        var c, u = ["chooser", "snippet-chooser"];
+        return r ? c = i ? a.default.createElement("div", {
             className: "chosen"
         }, a.default.createElement("span", {
             className: "title"
         }, i.title), a.default.createElement("ul", {
             className: "actions",
             style: {
                 listStyleType: "none"
             }
         }, a.default.createElement("li", null, a.default.createElement("a", {
             href: i.edit_url,
             className: "edit-link button button-small button-secondary",
             target: "_blank",
             rel: "noopener noreferrer"
-        }, o.default("Edit this %s").replace("%s", n.verbose_name))))) : a.default.createElement("p", null, o.default("Fetching %s information...").replace("%s", n.verbose_name)) : (c.push("blank"), u = a.default.createElement("div", {
+        }, o.default("Edit this %s").replace("%s", n.verbose_name))))) : a.default.createElement("p", null, o.default("Fetching %s information...").replace("%s", n.verbose_name)) : (u.push("blank"), c = a.default.createElement("div", {
             className: "unchosen"
         }, a.default.createElement("button", {
             type: "button",
             className: "button action-choose button-small button-secondary"
         }, o.default("Choose a %s").replace("%s", n.verbose_name)))), a.default.createElement("div", {
-            className: c.join(" ")
-        }, u)
+            className: u.join(" ")
+        }, c)
     }
 }, function(e, t, n) {
     "use strict";
     var r = this && this.__makeTemplateObject || function(e, t) {
             return Object.defineProperty ? Object.defineProperty(e, "raw", {
                 value: t
             }) : e.raw = t, e
         },
         a = this && this.__importDefault || function(e) {
             return e && e.__esModule ? e : {
                 default: e
             }
         };
     t.__esModule = !0;
-    var o, l, i, s, u = a(n(0)),
-        c = a(n(3)),
+    var o, l, i, s, c = a(n(0)),
+        u = a(n(3)),
         d = a(n(1)),
         f = a(n(2)),
         m = a(n(29)),
-        p = c.default.div(o || (o = r(["\n    &:after {\n        content: '';\n        display: table;\n        clear: both;\n    }\n"], ["\n    &:after {\n        content: '';\n        display: table;\n        clear: both;\n    }\n"]))),
-        h = c.default.div(l || (l = r(["\n    float: left;\n    margin-bottom: 40px;\n"], ["\n    float: left;\n    margin-bottom: 40px;\n"]))),
-        g = c.default.input(i || (i = r(["\n    border: 0;\n    clip: rect(0 0 0 0);\n    height: 1px;\n    margin: -1px;\n    overflow: hidden;\n    padding: 0;\n    position: absolute;\n    width: 1px;\n"], ["\n    border: 0;\n    clip: rect(0 0 0 0);\n    height: 1px;\n    margin: -1px;\n    overflow: hidden;\n    padding: 0;\n    position: absolute;\n    width: 1px;\n"]))),
-        v = c.default(m.default)(s || (s = r(["\n    width: 1.5em;\n    height: 1.5em;\n    vertical-align: text-top;\n"], ["\n    width: 1.5em;\n    height: 1.5em;\n    vertical-align: text-top;\n"])));
+        p = u.default.div(o || (o = r(["\n    &:after {\n        content: '';\n        display: table;\n        clear: both;\n    }\n"], ["\n    &:after {\n        content: '';\n        display: table;\n        clear: both;\n    }\n"]))),
+        h = u.default.div(l || (l = r(["\n    float: left;\n    margin-bottom: 40px;\n    margin-right: 2em;\n"], ["\n    float: left;\n    margin-bottom: 40px;\n    margin-right: 2em;\n"]))),
+        g = u.default.input(i || (i = r(["\n    border: 0;\n    clip: rect(0 0 0 0);\n    height: 1px;\n    margin: -1px;\n    overflow: hidden;\n    padding: 0;\n    position: absolute;\n    width: 1px;\n"], ["\n    border: 0;\n    clip: rect(0 0 0 0);\n    height: 1px;\n    margin: -1px;\n    overflow: hidden;\n    padding: 0;\n    position: absolute;\n    width: 1px;\n"]))),
+        v = u.default(m.default)(s || (s = r(["\n    width: 1.5em;\n    height: 1.5em;\n    vertical-align: text-top;\n"], ["\n    width: 1.5em;\n    height: 1.5em;\n    vertical-align: text-top;\n"])));
     t.default = function(e) {
         var t = e.object.isLocked,
             n = e.links,
             r = e.machineTranslator,
             a = e.csrfToken,
             o = e.stringTranslations,
             l = e.segments;
-        if (t) return u.default.createElement(u.default.Fragment, null);
+        if (t) return c.default.createElement(c.default.Fragment, null);
         var i = Array.from(o.keys()).length < l.length,
-            s = u.default.useRef(null),
-            c = u.default.useRef(null);
-        return u.default.createElement(p, {
+            s = c.default.useRef(null),
+            u = c.default.useRef(null);
+        return c.default.createElement(p, {
             className: "w-mt-4"
-        }, u.default.createElement(h, {
+        }, c.default.createElement(h, {
             className: "w-tabs__panel"
-        }, u.default.createElement("p", null, d.default("Download PO file and input translations offline")), u.default.createElement("a", {
+        }, c.default.createElement("p", null, d.default("Download PO file and input translations offline")), c.default.createElement("a", {
             className: "button button-primary button--icon",
             href: n.downloadPofile,
             download: !0
-        }, u.default.createElement(f.default, {
+        }, c.default.createElement(f.default, {
             name: "download"
-        }), " ", d.default("Download PO file"))), u.default.createElement(h, {
+        }), " ", d.default("Download PO file"))), c.default.createElement(h, {
             className: "w-tabs__panel"
-        }, u.default.createElement("p", null, d.default("Upload translated PO file to submit translations")), u.default.createElement("button", {
+        }, c.default.createElement("p", null, d.default("Upload translated PO file to submit translations")), c.default.createElement("button", {
             className: "button button-primary button--icon",
             onClick: function() {
-                c.current && c.current.click()
+                u.current && u.current.click()
             }
-        }, u.default.createElement(f.default, {
+        }, c.default.createElement(f.default, {
             name: "upload"
-        }), " ", d.default("Upload PO file")), u.default.createElement("form", {
+        }), " ", d.default("Upload PO file")), c.default.createElement("form", {
             ref: s,
             action: n.uploadPofile,
             method: "post",
             encType: "multipart/form-data"
-        }, u.default.createElement("input", {
+        }, c.default.createElement("input", {
             type: "hidden",
             name: "csrfmiddlewaretoken",
             value: a
-        }), u.default.createElement("input", {
+        }), c.default.createElement("input", {
             type: "hidden",
             name: "next",
             value: window.location.href
-        }), u.default.createElement(g, {
-            ref: c,
+        }), c.default.createElement(g, {
+            ref: u,
             onChange: function(e) {
                 e.preventDefault(), s.current && s.current.submit()
             },
             type: "file",
             name: "file"
-        }))), r && u.default.createElement(h, null, u.default.createElement("p", null, d.default("Translate all missing strings with ") + r.name), u.default.createElement("form", {
+        }))), r && c.default.createElement(h, null, c.default.createElement("p", null, d.default("Translate all missing strings with ") + r.name), c.default.createElement("form", {
             action: r.url,
             method: "post",
             encType: "multipart/form-data"
-        }, u.default.createElement("input", {
+        }, c.default.createElement("input", {
             type: "hidden",
             name: "csrfmiddlewaretoken",
             value: a
-        }), u.default.createElement("input", {
+        }), c.default.createElement("input", {
             type: "hidden",
             name: "next",
             value: window.location.href
-        }), u.default.createElement("button", {
+        }), c.default.createElement("button", {
             type: "submit",
             className: "button button-primary button--icon",
             disabled: !i
-        }, u.default.createElement(v, null), " ", d.default("Translate with ") + r.name))))
+        }, c.default.createElement(v, null), " ", d.default("Translate with ") + r.name))))
     }
 }, function(e, t, n) {
     "use strict";
     n.r(t);
     var r, a = n(0);
 
     function o() {
```

### Comparing `wagtail-localize-1.5/wagtail_localize/strings.py` & `wagtail-localize-1.5.1/wagtail_localize/strings.py`

 * *Files identical despite different names*

### Comparing `wagtail-localize-1.5/wagtail_localize/synctree.py` & `wagtail-localize-1.5.1/wagtail_localize/synctree.py`

 * *Files identical despite different names*

### Comparing `wagtail-localize-1.5/wagtail_localize/tasks.py` & `wagtail-localize-1.5.1/wagtail_localize/tasks.py`

 * *Files identical despite different names*

### Comparing `wagtail-localize-1.5/wagtail_localize/templates/wagtail_localize/admin/_components.html` & `wagtail-localize-1.5.1/wagtail_localize/templates/wagtail_localize/admin/_components.html`

 * *Files identical despite different names*

### Comparing `wagtail-localize-1.5/wagtail_localize/templates/wagtail_localize/admin/confirm_convert_to_alias.html` & `wagtail-localize-1.5.1/wagtail_localize/templates/wagtail_localize/admin/confirm_convert_to_alias.html`

 * *Files identical despite different names*

### Comparing `wagtail-localize-1.5/wagtail_localize/templates/wagtail_localize/admin/edit_translatable_alias.html` & `wagtail-localize-1.5.1/wagtail_localize/templates/wagtail_localize/admin/edit_translatable_alias.html`

 * *Files identical despite different names*

### Comparing `wagtail-localize-1.5/wagtail_localize/templates/wagtail_localize/admin/edit_translation.html` & `wagtail-localize-1.5.1/wagtail_localize/templates/wagtail_localize/admin/edit_translation.html`

 * *Files identical despite different names*

### Comparing `wagtail-localize-1.5/wagtail_localize/templates/wagtail_localize/admin/includes/generic_header.html` & `wagtail-localize-1.5.1/wagtail_localize/templates/wagtail_localize/admin/includes/generic_header.html`

 * *Files identical despite different names*

### Comparing `wagtail-localize-1.5/wagtail_localize/templates/wagtail_localize/admin/submit_translation.html` & `wagtail-localize-1.5.1/wagtail_localize/templates/wagtail_localize/admin/submit_translation.html`

 * *Files identical despite different names*

### Comparing `wagtail-localize-1.5/wagtail_localize/templates/wagtail_localize/admin/translations_report.html` & `wagtail-localize-1.5.1/wagtail_localize/templates/wagtail_localize/admin/translations_report.html`

 * *Files identical despite different names*

### Comparing `wagtail-localize-1.5/wagtail_localize/templates/wagtail_localize/admin/update_translations.html` & `wagtail-localize-1.5.1/wagtail_localize/templates/wagtail_localize/admin/update_translations.html`

 * *Files identical despite different names*

### Comparing `wagtail-localize-1.5/wagtail_localize/templates/wagtail_localize/icons/wagtail-localize-language.svg` & `wagtail-localize-1.5.1/wagtail_localize/templates/wagtail_localize/icons/wagtail-localize-language.svg`

 * *Files identical despite different names*

### Comparing `wagtail-localize-1.5/wagtail_localize/version.py` & `wagtail-localize-1.5.1/wagtail_localize/version.py`

 * *Files identical despite different names*

### Comparing `wagtail-localize-1.5/wagtail_localize/views/convert.py` & `wagtail-localize-1.5.1/wagtail_localize/views/convert.py`

 * *Files identical despite different names*

### Comparing `wagtail-localize-1.5/wagtail_localize/views/edit_translation.py` & `wagtail-localize-1.5.1/wagtail_localize/views/edit_translation.py`

 * *Files identical despite different names*

### Comparing `wagtail-localize-1.5/wagtail_localize/views/report.py` & `wagtail-localize-1.5.1/wagtail_localize/views/report.py`

 * *Files identical despite different names*

### Comparing `wagtail-localize-1.5/wagtail_localize/views/snippets_api.py` & `wagtail-localize-1.5.1/wagtail_localize/views/snippets_api.py`

 * *Files identical despite different names*

### Comparing `wagtail-localize-1.5/wagtail_localize/views/submit_translations.py` & `wagtail-localize-1.5.1/wagtail_localize/views/submit_translations.py`

 * *Files identical despite different names*

### Comparing `wagtail-localize-1.5/wagtail_localize/views/update_translations.py` & `wagtail-localize-1.5.1/wagtail_localize/views/update_translations.py`

 * *Files identical despite different names*

### Comparing `wagtail-localize-1.5/wagtail_localize/wagtail_hooks.py` & `wagtail-localize-1.5.1/wagtail_localize/wagtail_hooks.py`

 * *Files 0% similar despite different names*

```diff
@@ -253,15 +253,15 @@
     except Translation.DoesNotExist:
         pass
 
 
 class RestartTranslationPageActionMenuItem(PageActionMenuItem):
     label = gettext_lazy("Start Synced translation")
     name = "localize-restart-translation"
-    icon_name = "undo"
+    icon_name = "rotate"
     classname = "action-secondary"
 
     def is_shown(self, context):
         # Only show this menu item on the edit view where there was a previous translation record
         if context["view"] != "edit":
             return False
 
@@ -340,15 +340,15 @@
         except Translation.DoesNotExist:
             pass
 
 
 class RestartTranslationSnippetActionMenuItem(SnippetActionMenuItem):
     label = gettext_lazy("Start Synced translation")
     name = "localize-restart-translation"
-    icon_name = "undo"
+    icon_name = "rotate"
     classname = "action-secondary"
 
     def is_shown(self, context):
         # Only show this menu item on the edit view where there was a previous translation record
         if context["view"] != "edit":
             return False
```

### Comparing `wagtail-localize-1.5/PKG-INFO` & `wagtail-localize-1.5.1/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,46 +1,49 @@
 Metadata-Version: 2.1
 Name: wagtail-localize
-Version: 1.5
+Version: 1.5.1
 Summary: Translation plugin for Wagtail CMS
 Author-email: Karl Hobley <karl@torchbox.com>
-Requires-Python: >=3.7
+Maintainer-email: Dan Braghis <dan.braghis@torchbox.com>
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Framework :: Django
 Classifier: Framework :: Django :: 3.2
-Classifier: Framework :: Django :: 4.0
 Classifier: Framework :: Django :: 4.1
+Classifier: Framework :: Django :: 4.2
 Classifier: Framework :: Wagtail
 Classifier: Framework :: Wagtail :: 4
-Requires-Dist: Django>=3.2,<4.2
+Classifier: Framework :: Wagtail :: 5
+Requires-Dist: Django>=3.2,<5.0
 Requires-Dist: Wagtail>=4.1
 Requires-Dist: polib>=1.1,<2.0
 Requires-Dist: typing_extensions>=4.0
-Requires-Dist: mkdocs==1.1.2 ; extra == "documentation"
-Requires-Dist: mkdocs-material==6.2.8 ; extra == "documentation"
-Requires-Dist: mkdocs-mermaid2-plugin==0.5.1 ; extra == "documentation"
-Requires-Dist: mkdocstrings==0.14.0 ; extra == "documentation"
-Requires-Dist: mkdocs-include-markdown-plugin==2.8.0 ; extra == "documentation"
-Requires-Dist: pygments==2.11.2 ; extra == "documentation"
+Requires-Dist: mkdocs==1.4.3 ; extra == "documentation"
+Requires-Dist: mkdocs-material>=9.1,<10 ; extra == "documentation"
+Requires-Dist: mkdocstrings[python]==0.22.0 ; extra == "documentation"
+Requires-Dist: mkdocs-autorefs>=0.4.0,<0.5 ; extra == "documentation"
+Requires-Dist: mkdocs-include-markdown-plugin>=4.0.4,<5 ; extra == "documentation"
+Requires-Dist: pygments>=2.15,<2.16 ; extra == "documentation"
 Requires-Dist: google-cloud-translate>=3.0.0 ; extra == "google"
 Requires-Dist: dj-database-url==0.5.0 ; extra == "testing"
 Requires-Dist: freezegun==1.1.0 ; extra == "testing"
 Requires-Dist: django-rq>=2.5,<3.0 ; extra == "testing"
 Requires-Dist: google-cloud-translate>=3.0.0 ; extra == "testing"
+Requires-Dist: pre-commit>=2.21.0,<3.0 ; extra == "testing"
 Project-URL: Documentation, https://www.wagtail-localize.org
 Project-URL: Home, https://www.wagtail-localize.org
 Project-URL: Source, https://github.com/wagtail/wagtail-localize
 Provides-Extra: documentation
 Provides-Extra: google
 Provides-Extra: testing
 
@@ -60,17 +63,17 @@
 [Documentation](https://www.wagtail-localize.org)
 [Changelog](https://github.com/wagtail/wagtail-localize/blob/main/CHANGELOG.md)
 
 ## Requirements
 
 Wagtail Localize requires the following:
 
-- Python (3.7, 3.8, 3.9, 3.10, 3.11)
-- Django (3.2, 4.0, 4.1)
-- Wagtail (4.1, 4.2) with [internationalisation enabled](https://docs.wagtail.org/en/stable/advanced_topics/i18n.html#configuration)
+- Python (3.8, 3.9, 3.10, 3.11)
+- Django (3.2, 4.1, 4.2)
+- Wagtail (4.1, 4.2, 5.0) with [internationalisation enabled](https://docs.wagtail.org/en/stable/advanced_topics/i18n.html#configuration)
 
 ## Installation
 
 Install using `pip`:
 
 ```shell
 pip install wagtail-localize
@@ -108,31 +111,29 @@
 
 With your preferred virtualenv activated, install testing dependencies:
 
 #### Using pip
 
 ```sh
 pip install pip>=21.3
-pip install -e .[testing] -U
+pip install -e '.[testing]' -U
 ```
 
 #### Using flit
 
 ```sh
 pip install "flit>=3.8.0"
 flit install
 ```
 
 ### pre-commit
 
 Note that this project uses [pre-commit](https://github.com/pre-commit/pre-commit). To set up locally:
 
 ```shell
-# if you don't have it yet, globally
-$ pip install pre-commit
 # go to the project directory
 $ cd wagtail-localize
 # initialize pre-commit
 $ pre-commit install
 
 # Optional, run all checks once for this, then the checks will run only on the changed files
 $ pre-commit run --all-files
@@ -149,15 +150,15 @@
 or, you can run them for a specific environment `tox -e python3.8-django3.2-wagtail4.1` or specific test
 `tox -e python3.9-django3.2-wagtail4.1-sqlite wagtail_localize.tests.test_edit_translation.TestGetEditTranslationView`
 
 To run the test app interactively, use `tox -e interactive`, visit `http://127.0.0.1:8020/admin/` and log in with `admin`/`changeme`.
 
 ## Support
 
-For support, please use [GitHub Discussions](https://github.com/wagtail/wagtail-localize/discussions) or ask a question on the `#multi-language` channel on [Wagtail's Slack instance](`https://wagtail.org/slack/`).
+For support, please use [GitHub Discussions](https://github.com/wagtail/wagtail-localize/discussions) or ask a question on the `#multi-language` channel on [Wagtail's Slack instance](https://wagtail.org/slack/).
 
 ## Thanks
 
 Many thanks to all of our supporters, contributors, and early adopters who helped with the initial release. In particular, to The Mozilla Foundation and Torchbox who sponsored the majority of the initial development and Wagtail core's internationalisation support.
 
 <!--content-end-->
```

