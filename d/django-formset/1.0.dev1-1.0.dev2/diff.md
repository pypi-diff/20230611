# Comparing `tmp/django-formset-1.0.dev1.tar.gz` & `tmp/django-formset-1.0.dev2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-formset-1.0.dev1.tar", last modified: Fri Jun  9 12:44:35 2023, max compression
+gzip compressed data, was "django-formset-1.0.dev2.tar", last modified: Sun Jun 11 11:07:28 2023, max compression
```

## Comparing `django-formset-1.0.dev1.tar` & `django-formset-1.0.dev2.tar`

### file list

```diff
@@ -1,260 +1,261 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 12:44:35.765094 django-formset-1.0.dev1/
--rw-r--r--   0 runner    (1001) docker     (123)     1079 2023-06-09 12:43:32.000000 django-formset-1.0.dev1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      244 2023-06-09 12:43:32.000000 django-formset-1.0.dev1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    14240 2023-06-09 12:44:35.765094 django-formset-1.0.dev1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    13295 2023-06-09 12:43:32.000000 django-formset-1.0.dev1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 12:44:35.713094 django-formset-1.0.dev1/django_formset.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    14240 2023-06-09 12:44:35.000000 django-formset-1.0.dev1/django_formset.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    10168 2023-06-09 12:44:35.000000 django-formset-1.0.dev1/django_formset.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-09 12:44:35.000000 django-formset-1.0.dev1/django_formset.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-09 12:44:35.000000 django-formset-1.0.dev1/django_formset.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-09 12:44:35.000000 django-formset-1.0.dev1/django_formset.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-06-09 12:44:35.000000 django-formset-1.0.dev1/django_formset.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 12:44:35.717094 django-formset-1.0.dev1/formset/
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-06-09 12:43:32.000000 django-formset-1.0.dev1/formset/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8860 2023-06-09 12:43:32.000000 django-formset-1.0.dev1/formset/boundfield.py
--rw-r--r--   0 runner    (1001) docker     (123)     7637 2023-06-09 12:43:32.000000 django-formset-1.0.dev1/formset/calendar.py
--rw-r--r--   0 runner    (1001) docker     (123)    20763 2023-06-09 12:43:32.000000 django-formset-1.0.dev1/formset/collection.py
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-06-09 12:43:32.000000 django-formset-1.0.dev1/formset/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2913 2023-06-09 12:43:32.000000 django-formset-1.0.dev1/formset/fields.py
--rw-r--r--   0 runner    (1001) docker     (123)     2098 2023-06-09 12:43:32.000000 django-formset-1.0.dev1/formset/fieldset.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 12:44:35.705093 django-formset-1.0.dev1/formset/locale/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 12:44:35.705093 django-formset-1.0.dev1/formset/locale/de/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 12:44:35.717094 django-formset-1.0.dev1/formset/locale/de/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)     3444 2023-06-09 12:44:26.000000 django-formset-1.0.dev1/formset/locale/de/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (123)     7554 2023-06-09 12:43:32.000000 django-formset-1.0.dev1/formset/locale/de/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 12:44:35.717094 django-formset-1.0.dev1/formset/renderers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-09 12:43:32.000000 django-formset-1.0.dev1/formset/renderers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4271 2023-06-09 12:43:32.000000 django-formset-1.0.dev1/formset/renderers/bootstrap.py
--rw-r--r--   0 runner    (1001) docker     (123)     3302 2023-06-09 12:43:32.000000 django-formset-1.0.dev1/formset/renderers/bulma.py
--rw-r--r--   0 runner    (1001) docker     (123)     5684 2023-06-09 12:43:32.000000 django-formset-1.0.dev1/formset/renderers/default.py
--rw-r--r--   0 runner    (1001) docker     (123)     1964 2023-06-09 12:43:32.000000 django-formset-1.0.dev1/formset/renderers/foundation.py
--rw-r--r--   0 runner    (1001) docker     (123)     5111 2023-06-09 12:43:32.000000 django-formset-1.0.dev1/formset/renderers/tailwind.py
--rw-r--r--   0 runner    (1001) docker     (123)     2851 2023-06-09 12:43:32.000000 django-formset-1.0.dev1/formset/renderers/uikit.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 12:44:35.721094 django-formset-1.0.dev1/formset/richtext/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-09 12:43:32.000000 django-formset-1.0.dev1/formset/richtext/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7278 2023-06-09 12:43:32.000000 django-formset-1.0.dev1/formset/richtext/controls.py
--rw-r--r--   0 runner    (1001) docker     (123)     1456 2023-06-09 12:43:32.000000 django-formset-1.0.dev1/formset/richtext/dialogs.py
--rw-r--r--   0 runner    (1001) docker     (123)      353 2023-06-09 12:43:32.000000 django-formset-1.0.dev1/formset/richtext/fields.py
--rw-r--r--   0 runner    (1001) docker     (123)     1950 2023-06-09 12:43:32.000000 django-formset-1.0.dev1/formset/richtext/widgets.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 12:44:35.705093 django-formset-1.0.dev1/formset/static/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 12:44:35.709094 django-formset-1.0.dev1/formset/static/formset/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 12:44:35.721094 django-formset-1.0.dev1/formset/static/formset/css/
--rw-r--r--   0 runner    (1001) docker     (123)     1895 2023-06-09 12:44:23.000000 django-formset-1.0.dev1/formset/static/formset/css/bootstrap5-extra.css
--rw-r--r--   0 runner    (1001) docker     (123)      567 2023-06-09 12:44:23.000000 django-formset-1.0.dev1/formset/static/formset/css/bootstrap5-extra.css.map
--rw-r--r--   0 runner    (1001) docker     (123)     1830 2023-06-09 12:44:23.000000 django-formset-1.0.dev1/formset/static/formset/css/collections.css
--rw-r--r--   0 runner    (1001) docker     (123)      354 2023-06-09 12:44:23.000000 django-formset-1.0.dev1/formset/static/formset/css/collections.css.map
--rw-r--r--   0 runner    (1001) docker     (123)    35875 2023-06-09 12:44:25.000000 django-formset-1.0.dev1/formset/static/formset/css/tailwind.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 12:44:35.721094 django-formset-1.0.dev1/formset/static/formset/icons/
--rw-r--r--   0 runner    (1001) docker     (123)     1516 2023-06-09 12:43:32.000000 django-formset-1.0.dev1/formset/static/formset/icons/file-audio.svg
--rw-r--r--   0 runner    (1001) docker     (123)      637 2023-06-09 12:43:32.000000 django-formset-1.0.dev1/formset/static/formset/icons/file-empty.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1258 2023-06-09 12:43:32.000000 django-formset-1.0.dev1/formset/static/formset/icons/file-font.svg
--rw-r--r--   0 runner    (1001) docker     (123)     3181 2023-06-09 12:43:32.000000 django-formset-1.0.dev1/formset/static/formset/icons/file-missing.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1958 2023-06-09 12:43:32.000000 django-formset-1.0.dev1/formset/static/formset/icons/file-pdf.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1031 2023-06-09 12:43:32.000000 django-formset-1.0.dev1/formset/static/formset/icons/file-picture.svg
--rw-r--r--   0 runner    (1001) docker     (123)     2071 2023-06-09 12:43:32.000000 django-formset-1.0.dev1/formset/static/formset/icons/file-unknown.svg
--rw-r--r--   0 runner    (1001) docker     (123)     2911 2023-06-09 12:43:32.000000 django-formset-1.0.dev1/formset/static/formset/icons/file-video.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1838 2023-06-09 12:43:32.000000 django-formset-1.0.dev1/formset/static/formset/icons/file-zip.svg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 12:44:35.725094 django-formset-1.0.dev1/formset/static/formset/js/
--rw-r--r--   0 runner    (1001) docker     (123)    37792 2023-06-09 12:44:26.000000 django-formset-1.0.dev1/formset/static/formset/js/DateTimePicker-IUQQAZGS.js
--rw-r--r--   0 runner    (1001) docker     (123)    55721 2023-06-09 12:44:26.000000 django-formset-1.0.dev1/formset/static/formset/js/DjangoSelectize-D5OZV3VC.js
--rw-r--r--   0 runner    (1001) docker     (123)    11534 2023-06-09 12:44:26.000000 django-formset-1.0.dev1/formset/static/formset/js/DjangoSlug-226MVQ6E.js
--rw-r--r--   0 runner    (1001) docker     (123)    12352 2023-06-09 12:44:26.000000 django-formset-1.0.dev1/formset/static/formset/js/DualSelector-WKVUCHIG.js
--rw-r--r--   0 runner    (1001) docker     (123)   338568 2023-06-09 12:44:26.000000 django-formset-1.0.dev1/formset/static/formset/js/RichtextArea-XF7D5LDW.js
--rw-r--r--   0 runner    (1001) docker     (123)      196 2023-06-09 12:44:26.000000 django-formset-1.0.dev1/formset/static/formset/js/SortableSelect-7KQVPUF2.js
--rw-r--r--   0 runner    (1001) docker     (123)     3967 2023-06-09 12:44:26.000000 django-formset-1.0.dev1/formset/static/formset/js/chunk-A6DNWD2B.js
--rw-r--r--   0 runner    (1001) docker     (123)     1713 2023-06-09 12:44:26.000000 django-formset-1.0.dev1/formset/static/formset/js/chunk-AELXO3WZ.js
--rw-r--r--   0 runner    (1001) docker     (123)    43947 2023-06-09 12:44:26.000000 django-formset-1.0.dev1/formset/static/formset/js/chunk-APVD22ED.js
--rw-r--r--   0 runner    (1001) docker     (123)     9669 2023-06-09 12:44:26.000000 django-formset-1.0.dev1/formset/static/formset/js/chunk-KDP4ZIAK.js
--rw-r--r--   0 runner    (1001) docker     (123)      544 2023-06-09 12:44:26.000000 django-formset-1.0.dev1/formset/static/formset/js/chunk-NLMHZ7JJ.js
--rw-r--r--   0 runner    (1001) docker     (123)     1850 2023-06-09 12:44:26.000000 django-formset-1.0.dev1/formset/static/formset/js/chunk-O5UGFU32.js
--rw-r--r--   0 runner    (1001) docker     (123)   106347 2023-06-09 12:44:26.000000 django-formset-1.0.dev1/formset/static/formset/js/django-formset.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 12:44:35.725094 django-formset-1.0.dev1/formset/static/formset/scss/
--rw-r--r--   0 runner    (1001) docker     (123)     2091 2023-06-09 12:43:32.000000 django-formset-1.0.dev1/formset/static/formset/scss/bootstrap5-extra.scss
--rw-r--r--   0 runner    (1001) docker     (123)     1497 2023-06-09 12:43:32.000000 django-formset-1.0.dev1/formset/static/formset/scss/collections.scss
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 12:44:35.713094 django-formset-1.0.dev1/formset/templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 12:44:35.709094 django-formset-1.0.dev1/formset/templates/admin/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 12:44:35.725094 django-formset-1.0.dev1/formset/templates/admin/formset/
--rw-r--r--   0 runner    (1001) docker     (123)      344 2023-06-09 12:43:32.000000 django-formset-1.0.dev1/formset/templates/admin/formset/change_form.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 12:44:35.729094 django-formset-1.0.dev1/formset/templates/calendar/
--rw-r--r--   0 runner    (1001) docker     (123)     1360 2023-06-09 12:43:32.000000 django-formset-1.0.dev1/formset/templates/calendar/hours.html
--rw-r--r--   0 runner    (1001) docker     (123)     1176 2023-06-09 12:43:32.000000 django-formset-1.0.dev1/formset/templates/calendar/months.html
--rw-r--r--   0 runner    (1001) docker     (123)     1208 2023-06-09 12:43:32.000000 django-formset-1.0.dev1/formset/templates/calendar/weeks.html
--rw-r--r--   0 runner    (1001) docker     (123)     1132 2023-06-09 12:43:32.000000 django-formset-1.0.dev1/formset/templates/calendar/years.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 12:44:35.729094 django-formset-1.0.dev1/formset/templates/formset/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 12:44:35.729094 django-formset-1.0.dev1/formset/templates/formset/bootstrap/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 12:44:35.729094 django-formset-1.0.dev1/formset/templates/formset/bootstrap/buttons/
--rw-r--r--   0 runner    (1001) docker     (123)      176 2023-06-09 12:43:32.000000 django-formset-1.0.dev1/formset/templates/formset/bootstrap/buttons/add_collection.html
--rw-r--r--   0 runner    (1001) docker     (123)      134 2023-06-09 12:43:32.000000 django-formset-1.0.dev1/formset/templates/formset/bootstrap/buttons/remove_collection.html
--rw-r--r--   0 runner    (1001) docker     (123)      194 2023-06-09 12:43:32.000000 django-formset-1.0.dev1/formset/templates/formset/bootstrap/buttons/richtext_align.html
--rw-r--r--   0 runner    (1001) docker     (123)      194 2023-06-09 12:43:32.000000 django-formset-1.0.dev1/formset/templates/formset/bootstrap/buttons/richtext_color.html
--rw-r--r--   0 runner    (1001) docker     (123)      196 2023-06-09 12:43:32.000000 django-formset-1.0.dev1/formset/templates/formset/bootstrap/buttons/richtext_heading.html
--rw-r--r--   0 runner    (1001) docker     (123)      511 2023-06-09 12:43:32.000000 django-formset-1.0.dev1/formset/templates/formset/bootstrap/field_group.html
--rw-r--r--   0 runner    (1001) docker     (123)      254 2023-06-09 12:43:32.000000 django-formset-1.0.dev1/formset/templates/formset/bootstrap/form.html
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-06-09 12:43:32.000000 django-formset-1.0.dev1/formset/templates/formset/bootstrap/help_text.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 12:44:35.729094 django-formset-1.0.dev1/formset/templates/formset/bootstrap/widgets/
--rw-r--r--   0 runner    (1001) docker     (123)      181 2023-06-09 12:43:32.000000 django-formset-1.0.dev1/formset/templates/formset/bootstrap/widgets/checkbox.html
--rw-r--r--   0 runner    (1001) docker     (123)      918 2023-06-09 12:43:32.000000 django-formset-1.0.dev1/formset/templates/formset/bootstrap/widgets/dual_selector.html
--rw-r--r--   0 runner    (1001) docker     (123)      637 2023-06-09 12:43:32.000000 django-formset-1.0.dev1/formset/templates/formset/bootstrap/widgets/file.html
--rw-r--r--   0 runner    (1001) docker     (123)      169 2023-06-09 12:43:32.000000 django-formset-1.0.dev1/formset/templates/formset/bootstrap/widgets/input_option.html
--rw-r--r--   0 runner    (1001) docker     (123)      468 2023-06-09 12:43:32.000000 django-formset-1.0.dev1/formset/templates/formset/bootstrap/widgets/multiple_input.html
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-06-09 12:43:32.000000 django-formset-1.0.dev1/formset/templates/formset/bootstrap/widgets/richtextarea.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 12:44:35.733094 django-formset-1.0.dev1/formset/templates/formset/bulma/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 12:44:35.733094 django-formset-1.0.dev1/formset/templates/formset/bulma/buttons/
--rw-r--r--   0 runner    (1001) docker     (123)      124 2023-06-09 12:43:32.000000 django-formset-1.0.dev1/formset/templates/formset/bulma/buttons/add_collection.html
--rw-r--r--   0 runner    (1001) docker     (123)      122 2023-06-09 12:43:32.000000 django-formset-1.0.dev1/formset/templates/formset/bulma/buttons/remove_collection.html
--rw-r--r--   0 runner    (1001) docker     (123)      364 2023-06-09 12:43:32.000000 django-formset-1.0.dev1/formset/templates/formset/bulma/field_group.html
--rw-r--r--   0 runner    (1001) docker     (123)      253 2023-06-09 12:43:32.000000 django-formset-1.0.dev1/formset/templates/formset/bulma/form.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 12:44:35.733094 django-formset-1.0.dev1/formset/templates/formset/bulma/widgets/
--rw-r--r--   0 runner    (1001) docker     (123)      141 2023-06-09 12:43:32.000000 django-formset-1.0.dev1/formset/templates/formset/bulma/widgets/checkbox.html
--rw-r--r--   0 runner    (1001) docker     (123)     1260 2023-06-09 12:43:32.000000 django-formset-1.0.dev1/formset/templates/formset/bulma/widgets/dual_selector.html
--rw-r--r--   0 runner    (1001) docker     (123)      669 2023-06-09 12:43:32.000000 django-formset-1.0.dev1/formset/templates/formset/bulma/widgets/file.html
--rw-r--r--   0 runner    (1001) docker     (123)      183 2023-06-09 12:43:32.000000 django-formset-1.0.dev1/formset/templates/formset/bulma/widgets/input_option.html
--rw-r--r--   0 runner    (1001) docker     (123)      396 2023-06-09 12:43:32.000000 django-formset-1.0.dev1/formset/templates/formset/bulma/widgets/multiple_input.html
--rw-r--r--   0 runner    (1001) docker     (123)      113 2023-06-09 12:43:32.000000 django-formset-1.0.dev1/formset/templates/formset/bulma/widgets/select.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 12:44:35.733094 django-formset-1.0.dev1/formset/templates/formset/default/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 12:44:35.737094 django-formset-1.0.dev1/formset/templates/formset/default/buttons/
--rw-r--r--   0 runner    (1001) docker     (123)      361 2023-06-09 12:43:32.000000 django-formset-1.0.dev1/formset/templates/formset/default/buttons/add_collection.html
--rw-r--r--   0 runner    (1001) docker     (123)      204 2023-06-09 12:43:32.000000 django-formset-1.0.dev1/formset/templates/formset/default/buttons/move_all_left.html
--rw-r--r--   0 runner    (1001) docker     (123)      207 2023-06-09 12:43:32.000000 django-formset-1.0.dev1/formset/templates/formset/default/buttons/move_all_right.html
--rw-r--r--   0 runner    (1001) docker     (123)      207 2023-06-09 12:43:32.000000 django-formset-1.0.dev1/formset/templates/formset/default/buttons/move_selected_left.html
--rw-r--r--   0 runner    (1001) docker     (123)      210 2023-06-09 12:43:32.000000 django-formset-1.0.dev1/formset/templates/formset/default/buttons/move_selected_right.html
--rw-r--r--   0 runner    (1001) docker     (123)      189 2023-06-09 12:43:32.000000 django-formset-1.0.dev1/formset/templates/formset/default/buttons/redo_selected.html
--rw-r--r--   0 runner    (1001) docker     (123)      233 2023-06-09 12:43:32.000000 django-formset-1.0.dev1/formset/templates/formset/default/buttons/remove_collection.html
--rw-r--r--   0 runner    (1001) docker     (123)      959 2023-06-09 12:43:32.000000 django-formset-1.0.dev1/formset/templates/formset/default/buttons/richtext_align.html
--rw-r--r--   0 runner    (1001) docker     (123)      692 2023-06-09 12:43:32.000000 django-formset-1.0.dev1/formset/templates/formset/default/buttons/richtext_color.html
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-06-09 12:43:32.000000 django-formset-1.0.dev1/formset/templates/formset/default/buttons/richtext_control.html
--rw-r--r--   0 runner    (1001) docker     (123)      843 2023-06-09 12:43:32.000000 django-formset-1.0.dev1/formset/templates/formset/default/buttons/richtext_heading.html
--rw-r--r--   0 runner    (1001) docker     (123)       92 2023-06-09 12:43:32.000000 django-formset-1.0.dev1/formset/templates/formset/default/buttons/richtext_separator.html
--rw-r--r--   0 runner    (1001) docker     (123)      189 2023-06-09 12:43:32.000000 django-formset-1.0.dev1/formset/templates/formset/default/buttons/undo_selected.html
--rw-r--r--   0 runner    (1001) docker     (123)     1504 2023-06-09 12:43:32.000000 django-formset-1.0.dev1/formset/templates/formset/default/collection.html
--rw-r--r--   0 runner    (1001) docker     (123)      864 2023-06-09 12:43:32.000000 django-formset-1.0.dev1/formset/templates/formset/default/dialog_form.html
--rw-r--r--   0 runner    (1001) docker     (123)      300 2023-06-09 12:43:32.000000 django-formset-1.0.dev1/formset/templates/formset/default/field_errors.html
--rw-r--r--   0 runner    (1001) docker     (123)      407 2023-06-09 12:43:32.000000 django-formset-1.0.dev1/formset/templates/formset/default/field_group.html
--rw-r--r--   0 runner    (1001) docker     (123)      677 2023-06-09 12:43:32.000000 django-formset-1.0.dev1/formset/templates/formset/default/fieldset.html
--rw-r--r--   0 runner    (1001) docker     (123)      415 2023-06-09 12:43:32.000000 django-formset-1.0.dev1/formset/templates/formset/default/form.html
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-06-09 12:43:32.000000 django-formset-1.0.dev1/formset/templates/formset/default/help_text.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 12:44:35.741094 django-formset-1.0.dev1/formset/templates/formset/default/widgets/
--rw-r--r--   0 runner    (1001) docker     (123)      149 2023-06-09 12:43:32.000000 django-formset-1.0.dev1/formset/templates/formset/default/widgets/datetimepicker.html
--rw-r--r--   0 runner    (1001) docker     (123)     2416 2023-06-09 12:43:32.000000 django-formset-1.0.dev1/formset/templates/formset/default/widgets/dual_selector.html
--rw-r--r--   0 runner    (1001) docker     (123)     1407 2023-06-09 12:43:32.000000 django-formset-1.0.dev1/formset/templates/formset/default/widgets/file.html
--rw-r--r--   0 runner    (1001) docker     (123)      454 2023-06-09 12:43:32.000000 django-formset-1.0.dev1/formset/templates/formset/default/widgets/multiple_input.html
--rw-r--r--   0 runner    (1001) docker     (123)      446 2023-06-09 12:43:32.000000 django-formset-1.0.dev1/formset/templates/formset/default/widgets/richtextarea.html
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-06-09 12:43:32.000000 django-formset-1.0.dev1/formset/templates/formset/default/widgets/select.html
--rw-r--r--   0 runner    (1001) docker     (123)     1048 2023-06-09 12:43:32.000000 django-formset-1.0.dev1/formset/templates/formset/default/widgets/selectize.html
--rw-r--r--   0 runner    (1001) docker     (123)      216 2023-06-09 12:43:32.000000 django-formset-1.0.dev1/formset/templates/formset/form_attrs.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 12:44:35.741094 django-formset-1.0.dev1/formset/templates/formset/foundation/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 12:44:35.741094 django-formset-1.0.dev1/formset/templates/formset/foundation/buttons/
--rw-r--r--   0 runner    (1001) docker     (123)      132 2023-06-09 12:43:32.000000 django-formset-1.0.dev1/formset/templates/formset/foundation/buttons/add_collection.html
--rw-r--r--   0 runner    (1001) docker     (123)      128 2023-06-09 12:43:32.000000 django-formset-1.0.dev1/formset/templates/formset/foundation/buttons/remove_collection.html
--rw-r--r--   0 runner    (1001) docker     (123)      390 2023-06-09 12:43:32.000000 django-formset-1.0.dev1/formset/templates/formset/foundation/field_group.html
--rw-r--r--   0 runner    (1001) docker     (123)      258 2023-06-09 12:43:32.000000 django-formset-1.0.dev1/formset/templates/formset/foundation/form.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 12:44:35.741094 django-formset-1.0.dev1/formset/templates/formset/foundation/widgets/
--rw-r--r--   0 runner    (1001) docker     (123)      123 2023-06-09 12:43:32.000000 django-formset-1.0.dev1/formset/templates/formset/foundation/widgets/checkbox.html
--rw-r--r--   0 runner    (1001) docker     (123)      835 2023-06-09 12:43:32.000000 django-formset-1.0.dev1/formset/templates/formset/foundation/widgets/dual_selector.html
--rw-r--r--   0 runner    (1001) docker     (123)      654 2023-06-09 12:43:32.000000 django-formset-1.0.dev1/formset/templates/formset/foundation/widgets/file.html
--rw-r--r--   0 runner    (1001) docker     (123)      145 2023-06-09 12:43:32.000000 django-formset-1.0.dev1/formset/templates/formset/foundation/widgets/inlined_input_option.html
--rw-r--r--   0 runner    (1001) docker     (123)      340 2023-06-09 12:43:32.000000 django-formset-1.0.dev1/formset/templates/formset/foundation/widgets/multiple_input.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 12:44:35.753094 django-formset-1.0.dev1/formset/templates/formset/icons/
--rw-r--r--   0 runner    (1001) docker     (123)      196 2023-06-09 12:43:32.000000 django-formset-1.0.dev1/formset/templates/formset/icons/add-fill.svg
--rw-r--r--   0 runner    (1001) docker     (123)      193 2023-06-09 12:43:32.000000 django-formset-1.0.dev1/formset/templates/formset/icons/align-center.svg
--rw-r--r--   0 runner    (1001) docker     (123)      193 2023-06-09 12:43:32.000000 django-formset-1.0.dev1/formset/templates/formset/icons/align-justify.svg
--rw-r--r--   0 runner    (1001) docker     (123)      193 2023-06-09 12:43:32.000000 django-formset-1.0.dev1/formset/templates/formset/icons/align-left.svg
--rw-r--r--   0 runner    (1001) docker     (123)      193 2023-06-09 12:43:32.000000 django-formset-1.0.dev1/formset/templates/formset/icons/align-right.svg
--rw-r--r--   0 runner    (1001) docker     (123)      237 2023-06-09 12:43:32.000000 django-formset-1.0.dev1/formset/templates/formset/icons/arrow-left.svg
--rw-r--r--   0 runner    (1001) docker     (123)      245 2023-06-09 12:43:32.000000 django-formset-1.0.dev1/formset/templates/formset/icons/arrow-right.svg
--rw-r--r--   0 runner    (1001) docker     (123)      248 2023-06-09 12:43:32.000000 django-formset-1.0.dev1/formset/templates/formset/icons/arrow-up.svg
--rw-r--r--   0 runner    (1001) docker     (123)      792 2023-06-09 12:43:32.000000 django-formset-1.0.dev1/formset/templates/formset/icons/blockquote.svg
--rw-r--r--   0 runner    (1001) docker     (123)      408 2023-06-09 12:43:32.000000 django-formset-1.0.dev1/formset/templates/formset/icons/bold.svg
--rw-r--r--   0 runner    (1001) docker     (123)      252 2023-06-09 12:43:32.000000 django-formset-1.0.dev1/formset/templates/formset/icons/bulletlist.svg
--rw-r--r--   0 runner    (1001) docker     (123)      463 2023-06-09 12:43:32.000000 django-formset-1.0.dev1/formset/templates/formset/icons/calendar-today.svg
--rw-r--r--   0 runner    (1001) docker     (123)      318 2023-06-09 12:43:32.000000 django-formset-1.0.dev1/formset/templates/formset/icons/chevron-double-left.svg
--rw-r--r--   0 runner    (1001) docker     (123)      312 2023-06-09 12:43:32.000000 django-formset-1.0.dev1/formset/templates/formset/icons/chevron-double-right.svg
--rw-r--r--   0 runner    (1001) docker     (123)      225 2023-06-09 12:43:32.000000 django-formset-1.0.dev1/formset/templates/formset/icons/chevron-left.svg
--rw-r--r--   0 runner    (1001) docker     (123)      228 2023-06-09 12:43:32.000000 django-formset-1.0.dev1/formset/templates/formset/icons/chevron-right.svg
--rw-r--r--   0 runner    (1001) docker     (123)      329 2023-06-09 12:43:32.000000 django-formset-1.0.dev1/formset/templates/formset/icons/clearformat.svg
--rw-r--r--   0 runner    (1001) docker     (123)      359 2023-06-09 12:43:32.000000 django-formset-1.0.dev1/formset/templates/formset/icons/codeblock.svg
--rw-r--r--   0 runner    (1001) docker     (123)      219 2023-06-09 12:43:32.000000 django-formset-1.0.dev1/formset/templates/formset/icons/decreasemargin.svg
--rw-r--r--   0 runner    (1001) docker     (123)      467 2023-06-09 12:43:32.000000 django-formset-1.0.dev1/formset/templates/formset/icons/delete-back.svg
--rw-r--r--   0 runner    (1001) docker     (123)      456 2023-06-09 12:43:32.000000 django-formset-1.0.dev1/formset/templates/formset/icons/double-chevron-left.svg
--rw-r--r--   0 runner    (1001) docker     (123)      463 2023-06-09 12:43:32.000000 django-formset-1.0.dev1/formset/templates/formset/icons/double-chevron-right.svg
--rw-r--r--   0 runner    (1001) docker     (123)      323 2023-06-09 12:43:32.000000 django-formset-1.0.dev1/formset/templates/formset/icons/hardbreak.svg
--rw-r--r--   0 runner    (1001) docker     (123)      195 2023-06-09 12:43:32.000000 django-formset-1.0.dev1/formset/templates/formset/icons/heading.svg
--rw-r--r--   0 runner    (1001) docker     (123)      239 2023-06-09 12:43:32.000000 django-formset-1.0.dev1/formset/templates/formset/icons/heading1.svg
--rw-r--r--   0 runner    (1001) docker     (123)      429 2023-06-09 12:43:32.000000 django-formset-1.0.dev1/formset/templates/formset/icons/heading2.svg
--rw-r--r--   0 runner    (1001) docker     (123)      457 2023-06-09 12:43:32.000000 django-formset-1.0.dev1/formset/templates/formset/icons/heading3.svg
--rw-r--r--   0 runner    (1001) docker     (123)      272 2023-06-09 12:43:32.000000 django-formset-1.0.dev1/formset/templates/formset/icons/heading4.svg
--rw-r--r--   0 runner    (1001) docker     (123)      431 2023-06-09 12:43:32.000000 django-formset-1.0.dev1/formset/templates/formset/icons/heading5.svg
--rw-r--r--   0 runner    (1001) docker     (123)      371 2023-06-09 12:43:32.000000 django-formset-1.0.dev1/formset/templates/formset/icons/heading6.svg
--rw-r--r--   0 runner    (1001) docker     (123)      182 2023-06-09 12:43:32.000000 django-formset-1.0.dev1/formset/templates/formset/icons/horizontalrule.svg
--rw-r--r--   0 runner    (1001) docker     (123)      397 2023-06-09 12:43:32.000000 django-formset-1.0.dev1/formset/templates/formset/icons/image.svg
--rw-r--r--   0 runner    (1001) docker     (123)      219 2023-06-09 12:43:32.000000 django-formset-1.0.dev1/formset/templates/formset/icons/increasemargin.svg
--rw-r--r--   0 runner    (1001) docker     (123)      214 2023-06-09 12:43:32.000000 django-formset-1.0.dev1/formset/templates/formset/icons/indentfirstline.svg
--rw-r--r--   0 runner    (1001) docker     (123)      218 2023-06-09 12:43:32.000000 django-formset-1.0.dev1/formset/templates/formset/icons/italic.svg
--rw-r--r--   0 runner    (1001) docker     (123)      632 2023-06-09 12:43:32.000000 django-formset-1.0.dev1/formset/templates/formset/icons/letters.svg
--rw-r--r--   0 runner    (1001) docker     (123)      475 2023-06-09 12:43:32.000000 django-formset-1.0.dev1/formset/templates/formset/icons/link.svg
--rw-r--r--   0 runner    (1001) docker     (123)      308 2023-06-09 12:43:32.000000 django-formset-1.0.dev1/formset/templates/formset/icons/orderedlist.svg
--rw-r--r--   0 runner    (1001) docker     (123)      214 2023-06-09 12:43:32.000000 django-formset-1.0.dev1/formset/templates/formset/icons/outdentfirstline.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1226 2023-06-09 12:43:32.000000 django-formset-1.0.dev1/formset/templates/formset/icons/placeholder.svg
--rw-r--r--   0 runner    (1001) docker     (123)      529 2023-06-09 12:43:32.000000 django-formset-1.0.dev1/formset/templates/formset/icons/questionmark.svg
--rw-r--r--   0 runner    (1001) docker     (123)      280 2023-06-09 12:43:32.000000 django-formset-1.0.dev1/formset/templates/formset/icons/redo.svg
--rw-r--r--   0 runner    (1001) docker     (123)      457 2023-06-09 12:43:32.000000 django-formset-1.0.dev1/formset/templates/formset/icons/send.svg
--rw-r--r--   0 runner    (1001) docker     (123)      200 2023-06-09 12:43:32.000000 django-formset-1.0.dev1/formset/templates/formset/icons/separator.svg
--rw-r--r--   0 runner    (1001) docker     (123)      514 2023-06-09 12:43:32.000000 django-formset-1.0.dev1/formset/templates/formset/icons/subscript.svg
--rw-r--r--   0 runner    (1001) docker     (123)      501 2023-06-09 12:43:32.000000 django-formset-1.0.dev1/formset/templates/formset/icons/superscript.svg
--rw-r--r--   0 runner    (1001) docker     (123)      274 2023-06-09 12:43:32.000000 django-formset-1.0.dev1/formset/templates/formset/icons/textcolor.svg
--rw-r--r--   0 runner    (1001) docker     (123)      309 2023-06-09 12:43:32.000000 django-formset-1.0.dev1/formset/templates/formset/icons/trash.svg
--rw-r--r--   0 runner    (1001) docker     (123)      225 2023-06-09 12:43:32.000000 django-formset-1.0.dev1/formset/templates/formset/icons/underline.svg
--rw-r--r--   0 runner    (1001) docker     (123)      275 2023-06-09 12:43:32.000000 django-formset-1.0.dev1/formset/templates/formset/icons/undo.svg
--rw-r--r--   0 runner    (1001) docker     (123)      513 2023-06-09 12:43:32.000000 django-formset-1.0.dev1/formset/templates/formset/icons/unlink.svg
--rw-r--r--   0 runner    (1001) docker     (123)      109 2023-06-09 12:43:32.000000 django-formset-1.0.dev1/formset/templates/formset/non_field_errors.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 12:44:35.757094 django-formset-1.0.dev1/formset/templates/formset/tailwind/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 12:44:35.757094 django-formset-1.0.dev1/formset/templates/formset/tailwind/buttons/
--rw-r--r--   0 runner    (1001) docker     (123)      309 2023-06-09 12:43:32.000000 django-formset-1.0.dev1/formset/templates/formset/tailwind/buttons/add_collection.html
--rw-r--r--   0 runner    (1001) docker     (123)      262 2023-06-09 12:43:32.000000 django-formset-1.0.dev1/formset/templates/formset/tailwind/buttons/remove_collection.html
--rw-r--r--   0 runner    (1001) docker     (123)      376 2023-06-09 12:43:32.000000 django-formset-1.0.dev1/formset/templates/formset/tailwind/field_group.html
--rw-r--r--   0 runner    (1001) docker     (123)      256 2023-06-09 12:43:32.000000 django-formset-1.0.dev1/formset/templates/formset/tailwind/form.html
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-06-09 12:43:32.000000 django-formset-1.0.dev1/formset/templates/formset/tailwind/help_text.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 12:44:35.757094 django-formset-1.0.dev1/formset/templates/formset/tailwind/widgets/
--rw-r--r--   0 runner    (1001) docker     (123)      124 2023-06-09 12:43:32.000000 django-formset-1.0.dev1/formset/templates/formset/tailwind/widgets/checkbox.html
--rw-r--r--   0 runner    (1001) docker     (123)      884 2023-06-09 12:43:32.000000 django-formset-1.0.dev1/formset/templates/formset/tailwind/widgets/dual_selector.html
--rw-r--r--   0 runner    (1001) docker     (123)      611 2023-06-09 12:43:32.000000 django-formset-1.0.dev1/formset/templates/formset/tailwind/widgets/file.html
--rw-r--r--   0 runner    (1001) docker     (123)      144 2023-06-09 12:43:32.000000 django-formset-1.0.dev1/formset/templates/formset/tailwind/widgets/input_option.html
--rw-r--r--   0 runner    (1001) docker     (123)      454 2023-06-09 12:43:32.000000 django-formset-1.0.dev1/formset/templates/formset/tailwind/widgets/multiple_input.html
--rw-r--r--   0 runner    (1001) docker     (123)      449 2023-06-09 12:43:32.000000 django-formset-1.0.dev1/formset/templates/formset/tailwind/widgets/radio.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 12:44:35.757094 django-formset-1.0.dev1/formset/templates/formset/uikit/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 12:44:35.757094 django-formset-1.0.dev1/formset/templates/formset/uikit/buttons/
--rw-r--r--   0 runner    (1001) docker     (123)      113 2023-06-09 12:43:32.000000 django-formset-1.0.dev1/formset/templates/formset/uikit/buttons/add_collection.html
--rw-r--r--   0 runner    (1001) docker     (123)      116 2023-06-09 12:43:32.000000 django-formset-1.0.dev1/formset/templates/formset/uikit/buttons/remove_collection.html
--rw-r--r--   0 runner    (1001) docker     (123)      377 2023-06-09 12:43:32.000000 django-formset-1.0.dev1/formset/templates/formset/uikit/field_group.html
--rw-r--r--   0 runner    (1001) docker     (123)      253 2023-06-09 12:43:32.000000 django-formset-1.0.dev1/formset/templates/formset/uikit/form.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 12:44:35.761094 django-formset-1.0.dev1/formset/templates/formset/uikit/widgets/
--rw-r--r--   0 runner    (1001) docker     (123)      125 2023-06-09 12:43:32.000000 django-formset-1.0.dev1/formset/templates/formset/uikit/widgets/checkbox.html
--rw-r--r--   0 runner    (1001) docker     (123)      681 2023-06-09 12:43:32.000000 django-formset-1.0.dev1/formset/templates/formset/uikit/widgets/file.html
--rw-r--r--   0 runner    (1001) docker     (123)      227 2023-06-09 12:43:32.000000 django-formset-1.0.dev1/formset/templates/formset/uikit/widgets/input_option.html
--rw-r--r--   0 runner    (1001) docker     (123)      464 2023-06-09 12:43:32.000000 django-formset-1.0.dev1/formset/templates/formset/uikit/widgets/multiple_input.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 12:44:35.761094 django-formset-1.0.dev1/formset/templates/richtext/
--rw-r--r--   0 runner    (1001) docker     (123)      234 2023-06-09 12:43:32.000000 django-formset-1.0.dev1/formset/templates/richtext/bulletlist.html
--rw-r--r--   0 runner    (1001) docker     (123)      195 2023-06-09 12:43:32.000000 django-formset-1.0.dev1/formset/templates/richtext/doc.html
--rw-r--r--   0 runner    (1001) docker     (123)      272 2023-06-09 12:43:32.000000 django-formset-1.0.dev1/formset/templates/richtext/heading.html
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-06-09 12:43:32.000000 django-formset-1.0.dev1/formset/templates/richtext/horizontalrule.html
--rw-r--r--   0 runner    (1001) docker     (123)      201 2023-06-09 12:43:32.000000 django-formset-1.0.dev1/formset/templates/richtext/listitem.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 12:44:35.761094 django-formset-1.0.dev1/formset/templates/richtext/marks/
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-06-09 12:43:32.000000 django-formset-1.0.dev1/formset/templates/richtext/marks/bold.html
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-06-09 12:43:32.000000 django-formset-1.0.dev1/formset/templates/richtext/marks/code.html
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-06-09 12:43:32.000000 django-formset-1.0.dev1/formset/templates/richtext/marks/italic.html
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-06-09 12:43:32.000000 django-formset-1.0.dev1/formset/templates/richtext/marks/link.html
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-06-09 12:43:32.000000 django-formset-1.0.dev1/formset/templates/richtext/marks/underline.html
--rw-r--r--   0 runner    (1001) docker     (123)      201 2023-06-09 12:43:32.000000 django-formset-1.0.dev1/formset/templates/richtext/orderedlist.html
--rw-r--r--   0 runner    (1001) docker     (123)      204 2023-06-09 12:43:32.000000 django-formset-1.0.dev1/formset/templates/richtext/paragraph.html
--rw-r--r--   0 runner    (1001) docker     (123)      205 2023-06-09 12:43:32.000000 django-formset-1.0.dev1/formset/templates/richtext/text.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 12:44:35.765094 django-formset-1.0.dev1/formset/templatetags/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-09 12:43:32.000000 django-formset-1.0.dev1/formset/templatetags/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2428 2023-06-09 12:43:32.000000 django-formset-1.0.dev1/formset/templatetags/formsetify.py
--rw-r--r--   0 runner    (1001) docker     (123)      502 2023-06-09 12:43:32.000000 django-formset-1.0.dev1/formset/templatetags/richtext.py
--rw-r--r--   0 runner    (1001) docker     (123)     5703 2023-06-09 12:43:32.000000 django-formset-1.0.dev1/formset/upload.py
--rw-r--r--   0 runner    (1001) docker     (123)     5477 2023-06-09 12:43:32.000000 django-formset-1.0.dev1/formset/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    11553 2023-06-09 12:43:32.000000 django-formset-1.0.dev1/formset/views.py
--rw-r--r--   0 runner    (1001) docker     (123)    15216 2023-06-09 12:43:32.000000 django-formset-1.0.dev1/formset/widgets.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-09 12:44:35.765094 django-formset-1.0.dev1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1390 2023-06-09 12:43:32.000000 django-formset-1.0.dev1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 11:07:28.344778 django-formset-1.0.dev2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1079 2023-06-11 11:06:18.000000 django-formset-1.0.dev2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      244 2023-06-11 11:06:18.000000 django-formset-1.0.dev2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    14240 2023-06-11 11:07:28.344778 django-formset-1.0.dev2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    13295 2023-06-11 11:06:18.000000 django-formset-1.0.dev2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 11:07:28.308778 django-formset-1.0.dev2/django_formset.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    14240 2023-06-11 11:07:28.000000 django-formset-1.0.dev2/django_formset.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    10212 2023-06-11 11:07:28.000000 django-formset-1.0.dev2/django_formset.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-11 11:07:28.000000 django-formset-1.0.dev2/django_formset.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-11 11:07:28.000000 django-formset-1.0.dev2/django_formset.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-11 11:07:28.000000 django-formset-1.0.dev2/django_formset.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-06-11 11:07:28.000000 django-formset-1.0.dev2/django_formset.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 11:07:28.308778 django-formset-1.0.dev2/formset/
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-06-11 11:06:18.000000 django-formset-1.0.dev2/formset/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8860 2023-06-11 11:06:18.000000 django-formset-1.0.dev2/formset/boundfield.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7637 2023-06-11 11:06:18.000000 django-formset-1.0.dev2/formset/calendar.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20763 2023-06-11 11:06:18.000000 django-formset-1.0.dev2/formset/collection.py
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-06-11 11:06:18.000000 django-formset-1.0.dev2/formset/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2913 2023-06-11 11:06:18.000000 django-formset-1.0.dev2/formset/fields.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2098 2023-06-11 11:06:18.000000 django-formset-1.0.dev2/formset/fieldset.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 11:07:28.304777 django-formset-1.0.dev2/formset/locale/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 11:07:28.304777 django-formset-1.0.dev2/formset/locale/de/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 11:07:28.308778 django-formset-1.0.dev2/formset/locale/de/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)     3444 2023-06-11 11:07:21.000000 django-formset-1.0.dev2/formset/locale/de/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (123)     7554 2023-06-11 11:06:18.000000 django-formset-1.0.dev2/formset/locale/de/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 11:07:28.312778 django-formset-1.0.dev2/formset/renderers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-11 11:06:18.000000 django-formset-1.0.dev2/formset/renderers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4271 2023-06-11 11:06:18.000000 django-formset-1.0.dev2/formset/renderers/bootstrap.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3302 2023-06-11 11:06:18.000000 django-formset-1.0.dev2/formset/renderers/bulma.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5684 2023-06-11 11:06:18.000000 django-formset-1.0.dev2/formset/renderers/default.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1964 2023-06-11 11:06:18.000000 django-formset-1.0.dev2/formset/renderers/foundation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5111 2023-06-11 11:06:18.000000 django-formset-1.0.dev2/formset/renderers/tailwind.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2851 2023-06-11 11:06:18.000000 django-formset-1.0.dev2/formset/renderers/uikit.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 11:07:28.312778 django-formset-1.0.dev2/formset/richtext/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-11 11:06:18.000000 django-formset-1.0.dev2/formset/richtext/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7308 2023-06-11 11:06:18.000000 django-formset-1.0.dev2/formset/richtext/controls.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1456 2023-06-11 11:06:18.000000 django-formset-1.0.dev2/formset/richtext/dialogs.py
+-rw-r--r--   0 runner    (1001) docker     (123)      353 2023-06-11 11:06:18.000000 django-formset-1.0.dev2/formset/richtext/fields.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2043 2023-06-11 11:06:18.000000 django-formset-1.0.dev2/formset/richtext/widgets.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 11:07:28.304777 django-formset-1.0.dev2/formset/static/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 11:07:28.304777 django-formset-1.0.dev2/formset/static/formset/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 11:07:28.312778 django-formset-1.0.dev2/formset/static/formset/css/
+-rw-r--r--   0 runner    (1001) docker     (123)     1895 2023-06-11 11:07:18.000000 django-formset-1.0.dev2/formset/static/formset/css/bootstrap5-extra.css
+-rw-r--r--   0 runner    (1001) docker     (123)      567 2023-06-11 11:07:18.000000 django-formset-1.0.dev2/formset/static/formset/css/bootstrap5-extra.css.map
+-rw-r--r--   0 runner    (1001) docker     (123)     1830 2023-06-11 11:07:18.000000 django-formset-1.0.dev2/formset/static/formset/css/collections.css
+-rw-r--r--   0 runner    (1001) docker     (123)      354 2023-06-11 11:07:18.000000 django-formset-1.0.dev2/formset/static/formset/css/collections.css.map
+-rw-r--r--   0 runner    (1001) docker     (123)    35875 2023-06-11 11:07:19.000000 django-formset-1.0.dev2/formset/static/formset/css/tailwind.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 11:07:28.312778 django-formset-1.0.dev2/formset/static/formset/icons/
+-rw-r--r--   0 runner    (1001) docker     (123)     1516 2023-06-11 11:06:18.000000 django-formset-1.0.dev2/formset/static/formset/icons/file-audio.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      637 2023-06-11 11:06:18.000000 django-formset-1.0.dev2/formset/static/formset/icons/file-empty.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1258 2023-06-11 11:06:18.000000 django-formset-1.0.dev2/formset/static/formset/icons/file-font.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     3181 2023-06-11 11:06:18.000000 django-formset-1.0.dev2/formset/static/formset/icons/file-missing.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1958 2023-06-11 11:06:18.000000 django-formset-1.0.dev2/formset/static/formset/icons/file-pdf.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1031 2023-06-11 11:06:18.000000 django-formset-1.0.dev2/formset/static/formset/icons/file-picture.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     2071 2023-06-11 11:06:18.000000 django-formset-1.0.dev2/formset/static/formset/icons/file-unknown.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     2911 2023-06-11 11:06:18.000000 django-formset-1.0.dev2/formset/static/formset/icons/file-video.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1838 2023-06-11 11:06:18.000000 django-formset-1.0.dev2/formset/static/formset/icons/file-zip.svg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 11:07:28.316778 django-formset-1.0.dev2/formset/static/formset/js/
+-rw-r--r--   0 runner    (1001) docker     (123)    25407 2023-06-11 11:07:20.000000 django-formset-1.0.dev2/formset/static/formset/js/DateTimePicker-64ONYNKG.js
+-rw-r--r--   0 runner    (1001) docker     (123)    55721 2023-06-11 11:07:20.000000 django-formset-1.0.dev2/formset/static/formset/js/DjangoSelectize-MICJ4DHH.js
+-rw-r--r--   0 runner    (1001) docker     (123)    11534 2023-06-11 11:07:20.000000 django-formset-1.0.dev2/formset/static/formset/js/DjangoSlug-226MVQ6E.js
+-rw-r--r--   0 runner    (1001) docker     (123)    12352 2023-06-11 11:07:20.000000 django-formset-1.0.dev2/formset/static/formset/js/DualSelector-XYVC5VWO.js
+-rw-r--r--   0 runner    (1001) docker     (123)   316764 2023-06-11 11:07:20.000000 django-formset-1.0.dev2/formset/static/formset/js/RichtextArea-63COGKXW.js
+-rw-r--r--   0 runner    (1001) docker     (123)      196 2023-06-11 11:07:20.000000 django-formset-1.0.dev2/formset/static/formset/js/SortableSelect-WBJL5XGS.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1713 2023-06-11 11:07:20.000000 django-formset-1.0.dev2/formset/static/formset/js/chunk-AELXO3WZ.js
+-rw-r--r--   0 runner    (1001) docker     (123)    43947 2023-06-11 11:07:20.000000 django-formset-1.0.dev2/formset/static/formset/js/chunk-APVD22ED.js
+-rw-r--r--   0 runner    (1001) docker     (123)    12466 2023-06-11 11:07:20.000000 django-formset-1.0.dev2/formset/static/formset/js/chunk-ISEEQP4V.js
+-rw-r--r--   0 runner    (1001) docker     (123)     3967 2023-06-11 11:07:20.000000 django-formset-1.0.dev2/formset/static/formset/js/chunk-JSQHGMDY.js
+-rw-r--r--   0 runner    (1001) docker     (123)     9669 2023-06-11 11:07:20.000000 django-formset-1.0.dev2/formset/static/formset/js/chunk-KDP4ZIAK.js
+-rw-r--r--   0 runner    (1001) docker     (123)      544 2023-06-11 11:07:20.000000 django-formset-1.0.dev2/formset/static/formset/js/chunk-NLMHZ7JJ.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1850 2023-06-11 11:07:20.000000 django-formset-1.0.dev2/formset/static/formset/js/chunk-O5UGFU32.js
+-rw-r--r--   0 runner    (1001) docker     (123)   106347 2023-06-11 11:07:20.000000 django-formset-1.0.dev2/formset/static/formset/js/django-formset.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 11:07:28.316778 django-formset-1.0.dev2/formset/static/formset/scss/
+-rw-r--r--   0 runner    (1001) docker     (123)     2091 2023-06-11 11:06:18.000000 django-formset-1.0.dev2/formset/static/formset/scss/bootstrap5-extra.scss
+-rw-r--r--   0 runner    (1001) docker     (123)     1497 2023-06-11 11:06:18.000000 django-formset-1.0.dev2/formset/static/formset/scss/collections.scss
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 11:07:28.304777 django-formset-1.0.dev2/formset/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 11:07:28.304777 django-formset-1.0.dev2/formset/templates/admin/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 11:07:28.316778 django-formset-1.0.dev2/formset/templates/admin/formset/
+-rw-r--r--   0 runner    (1001) docker     (123)      344 2023-06-11 11:06:18.000000 django-formset-1.0.dev2/formset/templates/admin/formset/change_form.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 11:07:28.316778 django-formset-1.0.dev2/formset/templates/calendar/
+-rw-r--r--   0 runner    (1001) docker     (123)     1360 2023-06-11 11:06:18.000000 django-formset-1.0.dev2/formset/templates/calendar/hours.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1176 2023-06-11 11:06:18.000000 django-formset-1.0.dev2/formset/templates/calendar/months.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1208 2023-06-11 11:06:18.000000 django-formset-1.0.dev2/formset/templates/calendar/weeks.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1132 2023-06-11 11:06:18.000000 django-formset-1.0.dev2/formset/templates/calendar/years.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 11:07:28.320778 django-formset-1.0.dev2/formset/templates/formset/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 11:07:28.320778 django-formset-1.0.dev2/formset/templates/formset/bootstrap/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 11:07:28.320778 django-formset-1.0.dev2/formset/templates/formset/bootstrap/buttons/
+-rw-r--r--   0 runner    (1001) docker     (123)      176 2023-06-11 11:06:18.000000 django-formset-1.0.dev2/formset/templates/formset/bootstrap/buttons/add_collection.html
+-rw-r--r--   0 runner    (1001) docker     (123)      134 2023-06-11 11:06:18.000000 django-formset-1.0.dev2/formset/templates/formset/bootstrap/buttons/remove_collection.html
+-rw-r--r--   0 runner    (1001) docker     (123)      194 2023-06-11 11:06:18.000000 django-formset-1.0.dev2/formset/templates/formset/bootstrap/buttons/richtext_align.html
+-rw-r--r--   0 runner    (1001) docker     (123)      194 2023-06-11 11:06:18.000000 django-formset-1.0.dev2/formset/templates/formset/bootstrap/buttons/richtext_color.html
+-rw-r--r--   0 runner    (1001) docker     (123)      196 2023-06-11 11:06:18.000000 django-formset-1.0.dev2/formset/templates/formset/bootstrap/buttons/richtext_heading.html
+-rw-r--r--   0 runner    (1001) docker     (123)      511 2023-06-11 11:06:18.000000 django-formset-1.0.dev2/formset/templates/formset/bootstrap/field_group.html
+-rw-r--r--   0 runner    (1001) docker     (123)      254 2023-06-11 11:06:18.000000 django-formset-1.0.dev2/formset/templates/formset/bootstrap/form.html
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-06-11 11:06:18.000000 django-formset-1.0.dev2/formset/templates/formset/bootstrap/help_text.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 11:07:28.320778 django-formset-1.0.dev2/formset/templates/formset/bootstrap/widgets/
+-rw-r--r--   0 runner    (1001) docker     (123)      181 2023-06-11 11:06:18.000000 django-formset-1.0.dev2/formset/templates/formset/bootstrap/widgets/checkbox.html
+-rw-r--r--   0 runner    (1001) docker     (123)      918 2023-06-11 11:06:18.000000 django-formset-1.0.dev2/formset/templates/formset/bootstrap/widgets/dual_selector.html
+-rw-r--r--   0 runner    (1001) docker     (123)      637 2023-06-11 11:06:18.000000 django-formset-1.0.dev2/formset/templates/formset/bootstrap/widgets/file.html
+-rw-r--r--   0 runner    (1001) docker     (123)      169 2023-06-11 11:06:18.000000 django-formset-1.0.dev2/formset/templates/formset/bootstrap/widgets/input_option.html
+-rw-r--r--   0 runner    (1001) docker     (123)      468 2023-06-11 11:06:18.000000 django-formset-1.0.dev2/formset/templates/formset/bootstrap/widgets/multiple_input.html
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-06-11 11:06:18.000000 django-formset-1.0.dev2/formset/templates/formset/bootstrap/widgets/richtextarea.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 11:07:28.320778 django-formset-1.0.dev2/formset/templates/formset/bulma/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 11:07:28.320778 django-formset-1.0.dev2/formset/templates/formset/bulma/buttons/
+-rw-r--r--   0 runner    (1001) docker     (123)      124 2023-06-11 11:06:18.000000 django-formset-1.0.dev2/formset/templates/formset/bulma/buttons/add_collection.html
+-rw-r--r--   0 runner    (1001) docker     (123)      122 2023-06-11 11:06:18.000000 django-formset-1.0.dev2/formset/templates/formset/bulma/buttons/remove_collection.html
+-rw-r--r--   0 runner    (1001) docker     (123)      364 2023-06-11 11:06:18.000000 django-formset-1.0.dev2/formset/templates/formset/bulma/field_group.html
+-rw-r--r--   0 runner    (1001) docker     (123)      253 2023-06-11 11:06:18.000000 django-formset-1.0.dev2/formset/templates/formset/bulma/form.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 11:07:28.324778 django-formset-1.0.dev2/formset/templates/formset/bulma/widgets/
+-rw-r--r--   0 runner    (1001) docker     (123)      141 2023-06-11 11:06:18.000000 django-formset-1.0.dev2/formset/templates/formset/bulma/widgets/checkbox.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1260 2023-06-11 11:06:18.000000 django-formset-1.0.dev2/formset/templates/formset/bulma/widgets/dual_selector.html
+-rw-r--r--   0 runner    (1001) docker     (123)      669 2023-06-11 11:06:18.000000 django-formset-1.0.dev2/formset/templates/formset/bulma/widgets/file.html
+-rw-r--r--   0 runner    (1001) docker     (123)      183 2023-06-11 11:06:18.000000 django-formset-1.0.dev2/formset/templates/formset/bulma/widgets/input_option.html
+-rw-r--r--   0 runner    (1001) docker     (123)      396 2023-06-11 11:06:18.000000 django-formset-1.0.dev2/formset/templates/formset/bulma/widgets/multiple_input.html
+-rw-r--r--   0 runner    (1001) docker     (123)      113 2023-06-11 11:06:18.000000 django-formset-1.0.dev2/formset/templates/formset/bulma/widgets/select.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 11:07:28.324778 django-formset-1.0.dev2/formset/templates/formset/default/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 11:07:28.324778 django-formset-1.0.dev2/formset/templates/formset/default/buttons/
+-rw-r--r--   0 runner    (1001) docker     (123)      361 2023-06-11 11:06:18.000000 django-formset-1.0.dev2/formset/templates/formset/default/buttons/add_collection.html
+-rw-r--r--   0 runner    (1001) docker     (123)      204 2023-06-11 11:06:18.000000 django-formset-1.0.dev2/formset/templates/formset/default/buttons/move_all_left.html
+-rw-r--r--   0 runner    (1001) docker     (123)      207 2023-06-11 11:06:18.000000 django-formset-1.0.dev2/formset/templates/formset/default/buttons/move_all_right.html
+-rw-r--r--   0 runner    (1001) docker     (123)      207 2023-06-11 11:06:18.000000 django-formset-1.0.dev2/formset/templates/formset/default/buttons/move_selected_left.html
+-rw-r--r--   0 runner    (1001) docker     (123)      210 2023-06-11 11:06:18.000000 django-formset-1.0.dev2/formset/templates/formset/default/buttons/move_selected_right.html
+-rw-r--r--   0 runner    (1001) docker     (123)      189 2023-06-11 11:06:18.000000 django-formset-1.0.dev2/formset/templates/formset/default/buttons/redo_selected.html
+-rw-r--r--   0 runner    (1001) docker     (123)      233 2023-06-11 11:06:18.000000 django-formset-1.0.dev2/formset/templates/formset/default/buttons/remove_collection.html
+-rw-r--r--   0 runner    (1001) docker     (123)      959 2023-06-11 11:06:18.000000 django-formset-1.0.dev2/formset/templates/formset/default/buttons/richtext_align.html
+-rw-r--r--   0 runner    (1001) docker     (123)      692 2023-06-11 11:06:18.000000 django-formset-1.0.dev2/formset/templates/formset/default/buttons/richtext_color.html
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-06-11 11:06:18.000000 django-formset-1.0.dev2/formset/templates/formset/default/buttons/richtext_control.html
+-rw-r--r--   0 runner    (1001) docker     (123)      843 2023-06-11 11:06:18.000000 django-formset-1.0.dev2/formset/templates/formset/default/buttons/richtext_heading.html
+-rw-r--r--   0 runner    (1001) docker     (123)       92 2023-06-11 11:06:18.000000 django-formset-1.0.dev2/formset/templates/formset/default/buttons/richtext_separator.html
+-rw-r--r--   0 runner    (1001) docker     (123)      189 2023-06-11 11:06:18.000000 django-formset-1.0.dev2/formset/templates/formset/default/buttons/undo_selected.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1504 2023-06-11 11:06:18.000000 django-formset-1.0.dev2/formset/templates/formset/default/collection.html
+-rw-r--r--   0 runner    (1001) docker     (123)      864 2023-06-11 11:06:18.000000 django-formset-1.0.dev2/formset/templates/formset/default/dialog_form.html
+-rw-r--r--   0 runner    (1001) docker     (123)      300 2023-06-11 11:06:18.000000 django-formset-1.0.dev2/formset/templates/formset/default/field_errors.html
+-rw-r--r--   0 runner    (1001) docker     (123)      407 2023-06-11 11:06:18.000000 django-formset-1.0.dev2/formset/templates/formset/default/field_group.html
+-rw-r--r--   0 runner    (1001) docker     (123)      677 2023-06-11 11:06:18.000000 django-formset-1.0.dev2/formset/templates/formset/default/fieldset.html
+-rw-r--r--   0 runner    (1001) docker     (123)      415 2023-06-11 11:06:18.000000 django-formset-1.0.dev2/formset/templates/formset/default/form.html
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-06-11 11:06:18.000000 django-formset-1.0.dev2/formset/templates/formset/default/help_text.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 11:07:28.328778 django-formset-1.0.dev2/formset/templates/formset/default/widgets/
+-rw-r--r--   0 runner    (1001) docker     (123)      149 2023-06-11 11:06:18.000000 django-formset-1.0.dev2/formset/templates/formset/default/widgets/datetimepicker.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2416 2023-06-11 11:06:18.000000 django-formset-1.0.dev2/formset/templates/formset/default/widgets/dual_selector.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1407 2023-06-11 11:06:18.000000 django-formset-1.0.dev2/formset/templates/formset/default/widgets/file.html
+-rw-r--r--   0 runner    (1001) docker     (123)      454 2023-06-11 11:06:18.000000 django-formset-1.0.dev2/formset/templates/formset/default/widgets/multiple_input.html
+-rw-r--r--   0 runner    (1001) docker     (123)      446 2023-06-11 11:06:18.000000 django-formset-1.0.dev2/formset/templates/formset/default/widgets/richtextarea.html
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-06-11 11:06:18.000000 django-formset-1.0.dev2/formset/templates/formset/default/widgets/select.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1048 2023-06-11 11:06:18.000000 django-formset-1.0.dev2/formset/templates/formset/default/widgets/selectize.html
+-rw-r--r--   0 runner    (1001) docker     (123)      216 2023-06-11 11:06:18.000000 django-formset-1.0.dev2/formset/templates/formset/form_attrs.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 11:07:28.328778 django-formset-1.0.dev2/formset/templates/formset/foundation/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 11:07:28.328778 django-formset-1.0.dev2/formset/templates/formset/foundation/buttons/
+-rw-r--r--   0 runner    (1001) docker     (123)      132 2023-06-11 11:06:18.000000 django-formset-1.0.dev2/formset/templates/formset/foundation/buttons/add_collection.html
+-rw-r--r--   0 runner    (1001) docker     (123)      128 2023-06-11 11:06:18.000000 django-formset-1.0.dev2/formset/templates/formset/foundation/buttons/remove_collection.html
+-rw-r--r--   0 runner    (1001) docker     (123)      390 2023-06-11 11:06:18.000000 django-formset-1.0.dev2/formset/templates/formset/foundation/field_group.html
+-rw-r--r--   0 runner    (1001) docker     (123)      258 2023-06-11 11:06:18.000000 django-formset-1.0.dev2/formset/templates/formset/foundation/form.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 11:07:28.328778 django-formset-1.0.dev2/formset/templates/formset/foundation/widgets/
+-rw-r--r--   0 runner    (1001) docker     (123)      123 2023-06-11 11:06:18.000000 django-formset-1.0.dev2/formset/templates/formset/foundation/widgets/checkbox.html
+-rw-r--r--   0 runner    (1001) docker     (123)      835 2023-06-11 11:06:18.000000 django-formset-1.0.dev2/formset/templates/formset/foundation/widgets/dual_selector.html
+-rw-r--r--   0 runner    (1001) docker     (123)      654 2023-06-11 11:06:18.000000 django-formset-1.0.dev2/formset/templates/formset/foundation/widgets/file.html
+-rw-r--r--   0 runner    (1001) docker     (123)      145 2023-06-11 11:06:18.000000 django-formset-1.0.dev2/formset/templates/formset/foundation/widgets/inlined_input_option.html
+-rw-r--r--   0 runner    (1001) docker     (123)      340 2023-06-11 11:06:18.000000 django-formset-1.0.dev2/formset/templates/formset/foundation/widgets/multiple_input.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 11:07:28.336778 django-formset-1.0.dev2/formset/templates/formset/icons/
+-rw-r--r--   0 runner    (1001) docker     (123)      196 2023-06-11 11:06:18.000000 django-formset-1.0.dev2/formset/templates/formset/icons/add-fill.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      193 2023-06-11 11:06:18.000000 django-formset-1.0.dev2/formset/templates/formset/icons/align-center.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      193 2023-06-11 11:06:18.000000 django-formset-1.0.dev2/formset/templates/formset/icons/align-justify.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      193 2023-06-11 11:06:18.000000 django-formset-1.0.dev2/formset/templates/formset/icons/align-left.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      193 2023-06-11 11:06:18.000000 django-formset-1.0.dev2/formset/templates/formset/icons/align-right.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      237 2023-06-11 11:06:18.000000 django-formset-1.0.dev2/formset/templates/formset/icons/arrow-left.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      245 2023-06-11 11:06:18.000000 django-formset-1.0.dev2/formset/templates/formset/icons/arrow-right.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      248 2023-06-11 11:06:18.000000 django-formset-1.0.dev2/formset/templates/formset/icons/arrow-up.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      792 2023-06-11 11:06:18.000000 django-formset-1.0.dev2/formset/templates/formset/icons/blockquote.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      408 2023-06-11 11:06:18.000000 django-formset-1.0.dev2/formset/templates/formset/icons/bold.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      252 2023-06-11 11:06:18.000000 django-formset-1.0.dev2/formset/templates/formset/icons/bulletlist.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      463 2023-06-11 11:06:18.000000 django-formset-1.0.dev2/formset/templates/formset/icons/calendar-today.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      318 2023-06-11 11:06:18.000000 django-formset-1.0.dev2/formset/templates/formset/icons/chevron-double-left.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      312 2023-06-11 11:06:18.000000 django-formset-1.0.dev2/formset/templates/formset/icons/chevron-double-right.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      225 2023-06-11 11:06:18.000000 django-formset-1.0.dev2/formset/templates/formset/icons/chevron-left.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      228 2023-06-11 11:06:18.000000 django-formset-1.0.dev2/formset/templates/formset/icons/chevron-right.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      329 2023-06-11 11:06:18.000000 django-formset-1.0.dev2/formset/templates/formset/icons/clearformat.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      359 2023-06-11 11:06:18.000000 django-formset-1.0.dev2/formset/templates/formset/icons/codeblock.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      219 2023-06-11 11:06:18.000000 django-formset-1.0.dev2/formset/templates/formset/icons/decreasemargin.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      467 2023-06-11 11:06:18.000000 django-formset-1.0.dev2/formset/templates/formset/icons/delete-back.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      456 2023-06-11 11:06:18.000000 django-formset-1.0.dev2/formset/templates/formset/icons/double-chevron-left.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      463 2023-06-11 11:06:18.000000 django-formset-1.0.dev2/formset/templates/formset/icons/double-chevron-right.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      323 2023-06-11 11:06:18.000000 django-formset-1.0.dev2/formset/templates/formset/icons/hardbreak.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      195 2023-06-11 11:06:18.000000 django-formset-1.0.dev2/formset/templates/formset/icons/heading.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      239 2023-06-11 11:06:18.000000 django-formset-1.0.dev2/formset/templates/formset/icons/heading1.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      429 2023-06-11 11:06:18.000000 django-formset-1.0.dev2/formset/templates/formset/icons/heading2.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      457 2023-06-11 11:06:18.000000 django-formset-1.0.dev2/formset/templates/formset/icons/heading3.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      272 2023-06-11 11:06:18.000000 django-formset-1.0.dev2/formset/templates/formset/icons/heading4.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      431 2023-06-11 11:06:18.000000 django-formset-1.0.dev2/formset/templates/formset/icons/heading5.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      371 2023-06-11 11:06:18.000000 django-formset-1.0.dev2/formset/templates/formset/icons/heading6.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      182 2023-06-11 11:06:18.000000 django-formset-1.0.dev2/formset/templates/formset/icons/horizontalrule.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      397 2023-06-11 11:06:18.000000 django-formset-1.0.dev2/formset/templates/formset/icons/image.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      219 2023-06-11 11:06:18.000000 django-formset-1.0.dev2/formset/templates/formset/icons/increasemargin.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      214 2023-06-11 11:06:18.000000 django-formset-1.0.dev2/formset/templates/formset/icons/indentfirstline.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      218 2023-06-11 11:06:18.000000 django-formset-1.0.dev2/formset/templates/formset/icons/italic.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      632 2023-06-11 11:06:18.000000 django-formset-1.0.dev2/formset/templates/formset/icons/letters.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      475 2023-06-11 11:06:18.000000 django-formset-1.0.dev2/formset/templates/formset/icons/link.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      308 2023-06-11 11:06:18.000000 django-formset-1.0.dev2/formset/templates/formset/icons/orderedlist.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      214 2023-06-11 11:06:18.000000 django-formset-1.0.dev2/formset/templates/formset/icons/outdentfirstline.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1226 2023-06-11 11:06:18.000000 django-formset-1.0.dev2/formset/templates/formset/icons/placeholder.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      529 2023-06-11 11:06:18.000000 django-formset-1.0.dev2/formset/templates/formset/icons/questionmark.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      280 2023-06-11 11:06:18.000000 django-formset-1.0.dev2/formset/templates/formset/icons/redo.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      457 2023-06-11 11:06:18.000000 django-formset-1.0.dev2/formset/templates/formset/icons/send.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      200 2023-06-11 11:06:18.000000 django-formset-1.0.dev2/formset/templates/formset/icons/separator.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      514 2023-06-11 11:06:18.000000 django-formset-1.0.dev2/formset/templates/formset/icons/subscript.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      501 2023-06-11 11:06:18.000000 django-formset-1.0.dev2/formset/templates/formset/icons/superscript.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      274 2023-06-11 11:06:18.000000 django-formset-1.0.dev2/formset/templates/formset/icons/textcolor.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      309 2023-06-11 11:06:18.000000 django-formset-1.0.dev2/formset/templates/formset/icons/trash.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      225 2023-06-11 11:06:18.000000 django-formset-1.0.dev2/formset/templates/formset/icons/underline.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      275 2023-06-11 11:06:18.000000 django-formset-1.0.dev2/formset/templates/formset/icons/undo.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      513 2023-06-11 11:06:18.000000 django-formset-1.0.dev2/formset/templates/formset/icons/unlink.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      109 2023-06-11 11:06:18.000000 django-formset-1.0.dev2/formset/templates/formset/non_field_errors.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 11:07:28.336778 django-formset-1.0.dev2/formset/templates/formset/tailwind/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 11:07:28.336778 django-formset-1.0.dev2/formset/templates/formset/tailwind/buttons/
+-rw-r--r--   0 runner    (1001) docker     (123)      309 2023-06-11 11:06:18.000000 django-formset-1.0.dev2/formset/templates/formset/tailwind/buttons/add_collection.html
+-rw-r--r--   0 runner    (1001) docker     (123)      262 2023-06-11 11:06:18.000000 django-formset-1.0.dev2/formset/templates/formset/tailwind/buttons/remove_collection.html
+-rw-r--r--   0 runner    (1001) docker     (123)      376 2023-06-11 11:06:18.000000 django-formset-1.0.dev2/formset/templates/formset/tailwind/field_group.html
+-rw-r--r--   0 runner    (1001) docker     (123)      256 2023-06-11 11:06:18.000000 django-formset-1.0.dev2/formset/templates/formset/tailwind/form.html
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-06-11 11:06:18.000000 django-formset-1.0.dev2/formset/templates/formset/tailwind/help_text.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 11:07:28.340778 django-formset-1.0.dev2/formset/templates/formset/tailwind/widgets/
+-rw-r--r--   0 runner    (1001) docker     (123)      124 2023-06-11 11:06:18.000000 django-formset-1.0.dev2/formset/templates/formset/tailwind/widgets/checkbox.html
+-rw-r--r--   0 runner    (1001) docker     (123)      884 2023-06-11 11:06:18.000000 django-formset-1.0.dev2/formset/templates/formset/tailwind/widgets/dual_selector.html
+-rw-r--r--   0 runner    (1001) docker     (123)      611 2023-06-11 11:06:18.000000 django-formset-1.0.dev2/formset/templates/formset/tailwind/widgets/file.html
+-rw-r--r--   0 runner    (1001) docker     (123)      144 2023-06-11 11:06:18.000000 django-formset-1.0.dev2/formset/templates/formset/tailwind/widgets/input_option.html
+-rw-r--r--   0 runner    (1001) docker     (123)      454 2023-06-11 11:06:18.000000 django-formset-1.0.dev2/formset/templates/formset/tailwind/widgets/multiple_input.html
+-rw-r--r--   0 runner    (1001) docker     (123)      449 2023-06-11 11:06:18.000000 django-formset-1.0.dev2/formset/templates/formset/tailwind/widgets/radio.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 11:07:28.340778 django-formset-1.0.dev2/formset/templates/formset/uikit/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 11:07:28.340778 django-formset-1.0.dev2/formset/templates/formset/uikit/buttons/
+-rw-r--r--   0 runner    (1001) docker     (123)      113 2023-06-11 11:06:18.000000 django-formset-1.0.dev2/formset/templates/formset/uikit/buttons/add_collection.html
+-rw-r--r--   0 runner    (1001) docker     (123)      116 2023-06-11 11:06:18.000000 django-formset-1.0.dev2/formset/templates/formset/uikit/buttons/remove_collection.html
+-rw-r--r--   0 runner    (1001) docker     (123)      377 2023-06-11 11:06:18.000000 django-formset-1.0.dev2/formset/templates/formset/uikit/field_group.html
+-rw-r--r--   0 runner    (1001) docker     (123)      253 2023-06-11 11:06:18.000000 django-formset-1.0.dev2/formset/templates/formset/uikit/form.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 11:07:28.340778 django-formset-1.0.dev2/formset/templates/formset/uikit/widgets/
+-rw-r--r--   0 runner    (1001) docker     (123)      125 2023-06-11 11:06:18.000000 django-formset-1.0.dev2/formset/templates/formset/uikit/widgets/checkbox.html
+-rw-r--r--   0 runner    (1001) docker     (123)      681 2023-06-11 11:06:18.000000 django-formset-1.0.dev2/formset/templates/formset/uikit/widgets/file.html
+-rw-r--r--   0 runner    (1001) docker     (123)      227 2023-06-11 11:06:18.000000 django-formset-1.0.dev2/formset/templates/formset/uikit/widgets/input_option.html
+-rw-r--r--   0 runner    (1001) docker     (123)      464 2023-06-11 11:06:18.000000 django-formset-1.0.dev2/formset/templates/formset/uikit/widgets/multiple_input.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 11:07:28.340778 django-formset-1.0.dev2/formset/templates/richtext/
+-rw-r--r--   0 runner    (1001) docker     (123)      234 2023-06-11 11:06:18.000000 django-formset-1.0.dev2/formset/templates/richtext/bulletlist.html
+-rw-r--r--   0 runner    (1001) docker     (123)      195 2023-06-11 11:06:18.000000 django-formset-1.0.dev2/formset/templates/richtext/doc.html
+-rw-r--r--   0 runner    (1001) docker     (123)      272 2023-06-11 11:06:18.000000 django-formset-1.0.dev2/formset/templates/richtext/heading.html
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-06-11 11:06:18.000000 django-formset-1.0.dev2/formset/templates/richtext/horizontalrule.html
+-rw-r--r--   0 runner    (1001) docker     (123)      201 2023-06-11 11:06:18.000000 django-formset-1.0.dev2/formset/templates/richtext/listitem.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 11:07:28.340778 django-formset-1.0.dev2/formset/templates/richtext/marks/
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-06-11 11:06:18.000000 django-formset-1.0.dev2/formset/templates/richtext/marks/bold.html
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-06-11 11:06:18.000000 django-formset-1.0.dev2/formset/templates/richtext/marks/code.html
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-06-11 11:06:18.000000 django-formset-1.0.dev2/formset/templates/richtext/marks/italic.html
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-06-11 11:06:18.000000 django-formset-1.0.dev2/formset/templates/richtext/marks/link.html
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-06-11 11:06:18.000000 django-formset-1.0.dev2/formset/templates/richtext/marks/underline.html
+-rw-r--r--   0 runner    (1001) docker     (123)      201 2023-06-11 11:06:18.000000 django-formset-1.0.dev2/formset/templates/richtext/orderedlist.html
+-rw-r--r--   0 runner    (1001) docker     (123)      204 2023-06-11 11:06:18.000000 django-formset-1.0.dev2/formset/templates/richtext/paragraph.html
+-rw-r--r--   0 runner    (1001) docker     (123)      205 2023-06-11 11:06:18.000000 django-formset-1.0.dev2/formset/templates/richtext/text.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 11:07:28.340778 django-formset-1.0.dev2/formset/templatetags/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-11 11:06:18.000000 django-formset-1.0.dev2/formset/templatetags/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2428 2023-06-11 11:06:18.000000 django-formset-1.0.dev2/formset/templatetags/formsetify.py
+-rw-r--r--   0 runner    (1001) docker     (123)      502 2023-06-11 11:06:18.000000 django-formset-1.0.dev2/formset/templatetags/richtext.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5703 2023-06-11 11:06:18.000000 django-formset-1.0.dev2/formset/upload.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5477 2023-06-11 11:06:18.000000 django-formset-1.0.dev2/formset/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11553 2023-06-11 11:06:18.000000 django-formset-1.0.dev2/formset/views.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15216 2023-06-11 11:06:18.000000 django-formset-1.0.dev2/formset/widgets.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-11 11:07:28.344778 django-formset-1.0.dev2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1390 2023-06-11 11:06:18.000000 django-formset-1.0.dev2/setup.py
```

### Comparing `django-formset-1.0.dev1/LICENSE` & `django-formset-1.0.dev2/LICENSE`

 * *Files identical despite different names*

### Comparing `django-formset-1.0.dev1/PKG-INFO` & `django-formset-1.0.dev2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-formset
-Version: 1.0.dev1
+Version: 1.0.dev2
 Summary: Prevalidate Django Forms in the browser
 Home-page: https://github.com/jrief/django-formset
 Author: Jacob Rief
 Author-email: jacob.rief@gmail.com
 License: MIT
 Keywords: Django Forms,webcomponent
 Platform: OS Independent
```

### Comparing `django-formset-1.0.dev1/README.md` & `django-formset-1.0.dev2/README.md`

 * *Files identical despite different names*

### Comparing `django-formset-1.0.dev1/django_formset.egg-info/PKG-INFO` & `django-formset-1.0.dev2/django_formset.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-formset
-Version: 1.0.dev1
+Version: 1.0.dev2
 Summary: Prevalidate Django Forms in the browser
 Home-page: https://github.com/jrief/django-formset
 Author: Jacob Rief
 Author-email: jacob.rief@gmail.com
 License: MIT
 Keywords: Django Forms,webcomponent
 Platform: OS Independent
```

### Comparing `django-formset-1.0.dev1/django_formset.egg-info/SOURCES.txt` & `django-formset-1.0.dev2/django_formset.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -43,23 +43,24 @@
 formset/static/formset/icons/file-font.svg
 formset/static/formset/icons/file-missing.svg
 formset/static/formset/icons/file-pdf.svg
 formset/static/formset/icons/file-picture.svg
 formset/static/formset/icons/file-unknown.svg
 formset/static/formset/icons/file-video.svg
 formset/static/formset/icons/file-zip.svg
-formset/static/formset/js/DateTimePicker-IUQQAZGS.js
-formset/static/formset/js/DjangoSelectize-D5OZV3VC.js
+formset/static/formset/js/DateTimePicker-64ONYNKG.js
+formset/static/formset/js/DjangoSelectize-MICJ4DHH.js
 formset/static/formset/js/DjangoSlug-226MVQ6E.js
-formset/static/formset/js/DualSelector-WKVUCHIG.js
-formset/static/formset/js/RichtextArea-XF7D5LDW.js
-formset/static/formset/js/SortableSelect-7KQVPUF2.js
-formset/static/formset/js/chunk-A6DNWD2B.js
+formset/static/formset/js/DualSelector-XYVC5VWO.js
+formset/static/formset/js/RichtextArea-63COGKXW.js
+formset/static/formset/js/SortableSelect-WBJL5XGS.js
 formset/static/formset/js/chunk-AELXO3WZ.js
 formset/static/formset/js/chunk-APVD22ED.js
+formset/static/formset/js/chunk-ISEEQP4V.js
+formset/static/formset/js/chunk-JSQHGMDY.js
 formset/static/formset/js/chunk-KDP4ZIAK.js
 formset/static/formset/js/chunk-NLMHZ7JJ.js
 formset/static/formset/js/chunk-O5UGFU32.js
 formset/static/formset/js/django-formset.js
 formset/static/formset/scss/bootstrap5-extra.scss
 formset/static/formset/scss/collections.scss
 formset/templates/admin/formset/change_form.html
```

### Comparing `django-formset-1.0.dev1/formset/boundfield.py` & `django-formset-1.0.dev2/formset/boundfield.py`

 * *Files identical despite different names*

### Comparing `django-formset-1.0.dev1/formset/calendar.py` & `django-formset-1.0.dev2/formset/calendar.py`

 * *Files identical despite different names*

### Comparing `django-formset-1.0.dev1/formset/collection.py` & `django-formset-1.0.dev2/formset/collection.py`

 * *Files identical despite different names*

### Comparing `django-formset-1.0.dev1/formset/fields.py` & `django-formset-1.0.dev2/formset/fields.py`

 * *Files identical despite different names*

### Comparing `django-formset-1.0.dev1/formset/fieldset.py` & `django-formset-1.0.dev2/formset/fieldset.py`

 * *Files identical despite different names*

### Comparing `django-formset-1.0.dev1/formset/locale/de/LC_MESSAGES/django.mo` & `django-formset-1.0.dev2/formset/locale/de/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-formset-1.0.dev1/formset/locale/de/LC_MESSAGES/django.po` & `django-formset-1.0.dev2/formset/locale/de/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-formset-1.0.dev1/formset/renderers/bootstrap.py` & `django-formset-1.0.dev2/formset/renderers/bootstrap.py`

 * *Files identical despite different names*

### Comparing `django-formset-1.0.dev1/formset/renderers/bulma.py` & `django-formset-1.0.dev2/formset/renderers/bulma.py`

 * *Files identical despite different names*

### Comparing `django-formset-1.0.dev1/formset/renderers/default.py` & `django-formset-1.0.dev2/formset/renderers/default.py`

 * *Files identical despite different names*

### Comparing `django-formset-1.0.dev1/formset/renderers/foundation.py` & `django-formset-1.0.dev2/formset/renderers/foundation.py`

 * *Files identical despite different names*

### Comparing `django-formset-1.0.dev1/formset/renderers/tailwind.py` & `django-formset-1.0.dev2/formset/renderers/tailwind.py`

 * *Files identical despite different names*

### Comparing `django-formset-1.0.dev1/formset/renderers/uikit.py` & `django-formset-1.0.dev2/formset/renderers/uikit.py`

 * *Files identical despite different names*

### Comparing `django-formset-1.0.dev1/formset/richtext/controls.py` & `django-formset-1.0.dev2/formset/richtext/controls.py`

 * *Files 1% similar despite different names*

```diff
@@ -91,15 +91,14 @@
         })
 
 
 class TextColor(ControlElement):
     name = 'textColor'
     label = _("Text Color")
     template_name = 'formset/{framework}/buttons/richtext_color.html'
-    colors = [None]
     class_based = None
 
     def __init__(self, colors):
         if not isinstance(colors, (list, tuple)) or len(colors) == 0:
             raise ImproperlyConfigured("TextColor() requires a list with at least one color")
         rgb_pattern = re.compile(r'^rgb\(\d{1,3}, \d{1,3}, \d{1,3}\)$')
         class_pattern = re.compile(r'^-?[_a-zA-Z]+[_a-zA-Z0-9-]*$')
@@ -108,14 +107,15 @@
                 if self.class_based is True:
                     raise ImproperlyConfigured(f"Given color {color} is not in format rgb(r, g, b)")
                 self.class_based = False
             elif re.match(class_pattern, color):
                 if self.class_based is False:
                     raise ImproperlyConfigured(f"Given color {color} does not look like a valid CSS class name")
                 self.class_based = True
+        self.colors = [None]  # the default color
         self.colors.extend(colors)
 
     def render(self, renderer):
         template = self.get_template(renderer)
         return template.render({
             'colors': self.colors,
             'class_based': self.class_based,
```

### Comparing `django-formset-1.0.dev1/formset/richtext/dialogs.py` & `django-formset-1.0.dev2/formset/richtext/dialogs.py`

 * *Files identical despite different names*

### Comparing `django-formset-1.0.dev1/formset/richtext/widgets.py` & `django-formset-1.0.dev2/formset/richtext/widgets.py`

 * *Files 11% similar despite different names*

```diff
@@ -37,16 +37,18 @@
         context['use_json'] = attrs.get('use_json', False)
         context['widget']['attrs'].pop('use_json', None)
         return context
 
     def render(self, name, value, attrs=None, renderer=None):
         context = self.get_context(name, value, attrs)
         control_panel = format_html_join('', '{0}', ((elm.render(renderer),) for elm in self.control_elements))
+        auto_id = '{id}_dialog_%s'.format(**attrs)
         modal_dialogs = format_html_join('\n', '{0}', (
-            (format_html('<dialog richtext-opener="{0}">{1}</dialog>', elm.name, elm.dialog_class(renderer=renderer)),)
+            (format_html('<dialog richtext-opener="{0}">{1}</dialog>',
+                         elm.name, elm.dialog_class(renderer=renderer, auto_id=auto_id)),)
             for elm in self.control_elements if getattr(elm, 'dialog_class', None))
         )
         context.update(
             control_panel=control_panel,
             modal_dialogs=modal_dialogs,
         )
         return self._render(self.template_name, context, renderer)
```

### Comparing `django-formset-1.0.dev1/formset/static/formset/css/bootstrap5-extra.css` & `django-formset-1.0.dev2/formset/static/formset/css/bootstrap5-extra.css`

 * *Files identical despite different names*

### Comparing `django-formset-1.0.dev1/formset/static/formset/css/bootstrap5-extra.css.map` & `django-formset-1.0.dev2/formset/static/formset/css/bootstrap5-extra.css.map`

 * *Files identical despite different names*

### Comparing `django-formset-1.0.dev1/formset/static/formset/css/collections.css` & `django-formset-1.0.dev2/formset/static/formset/css/collections.css`

 * *Files identical despite different names*

### Comparing `django-formset-1.0.dev1/formset/static/formset/css/tailwind.css` & `django-formset-1.0.dev2/formset/static/formset/css/tailwind.css`

 * *Files identical despite different names*

### Comparing `django-formset-1.0.dev1/formset/static/formset/icons/file-audio.svg` & `django-formset-1.0.dev2/formset/static/formset/icons/file-audio.svg`

 * *Files identical despite different names*

### Comparing `django-formset-1.0.dev1/formset/static/formset/icons/file-empty.svg` & `django-formset-1.0.dev2/formset/static/formset/icons/file-empty.svg`

 * *Files identical despite different names*

### Comparing `django-formset-1.0.dev1/formset/static/formset/icons/file-font.svg` & `django-formset-1.0.dev2/formset/static/formset/icons/file-font.svg`

 * *Files identical despite different names*

### Comparing `django-formset-1.0.dev1/formset/static/formset/icons/file-missing.svg` & `django-formset-1.0.dev2/formset/static/formset/icons/file-missing.svg`

 * *Files identical despite different names*

### Comparing `django-formset-1.0.dev1/formset/static/formset/icons/file-pdf.svg` & `django-formset-1.0.dev2/formset/static/formset/icons/file-pdf.svg`

 * *Files identical despite different names*

### Comparing `django-formset-1.0.dev1/formset/static/formset/icons/file-picture.svg` & `django-formset-1.0.dev2/formset/static/formset/icons/file-picture.svg`

 * *Files identical despite different names*

### Comparing `django-formset-1.0.dev1/formset/static/formset/icons/file-unknown.svg` & `django-formset-1.0.dev2/formset/static/formset/icons/file-unknown.svg`

 * *Files identical despite different names*

### Comparing `django-formset-1.0.dev1/formset/static/formset/icons/file-video.svg` & `django-formset-1.0.dev2/formset/static/formset/icons/file-video.svg`

 * *Files identical despite different names*

### Comparing `django-formset-1.0.dev1/formset/static/formset/icons/file-zip.svg` & `django-formset-1.0.dev2/formset/static/formset/icons/file-zip.svg`

 * *Files identical despite different names*

### Comparing `django-formset-1.0.dev1/formset/static/formset/js/DjangoSelectize-D5OZV3VC.js` & `django-formset-1.0.dev2/formset/static/formset/js/DjangoSelectize-MICJ4DHH.js`

 * *Files identical despite different names*

### Comparing `django-formset-1.0.dev1/formset/static/formset/js/DjangoSlug-226MVQ6E.js` & `django-formset-1.0.dev2/formset/static/formset/js/DjangoSlug-226MVQ6E.js`

 * *Files identical despite different names*

### Comparing `django-formset-1.0.dev1/formset/static/formset/js/DualSelector-WKVUCHIG.js` & `django-formset-1.0.dev2/formset/static/formset/js/DualSelector-XYVC5VWO.js`

 * *Files 1% similar despite different names*

#### js-beautify {}

```diff
@@ -1,14 +1,14 @@
 import {
     a as d
 } from "./chunk-AELXO3WZ.js";
 import {
     a as u,
     b as p
-} from "./chunk-A6DNWD2B.js";
+} from "./chunk-JSQHGMDY.js";
 import "./chunk-APVD22ED.js";
 import {
     a as g
 } from "./chunk-KDP4ZIAK.js";
 import {
     a as r
 } from "./chunk-O5UGFU32.js";
```

### Comparing `django-formset-1.0.dev1/formset/static/formset/js/RichtextArea-XF7D5LDW.js` & `django-formset-1.0.dev2/formset/static/formset/js/RichtextArea-63COGKXW.js`

 * *Files 3% similar despite different names*

#### js-beautify {}

```diff
@@ -1,1442 +1,212 @@
 import {
-    a as hd
+    a as bc
 } from "./chunk-KDP4ZIAK.js";
 import {
-    a as wt
+    d as Vs
+} from "./chunk-ISEEQP4V.js";
+import {
+    a as Ue
 } from "./chunk-O5UGFU32.js";
 import {
-    b as pd
+    b as yc
 } from "./chunk-NLMHZ7JJ.js";
-var pl = '.dj-richtext-wrapper{--button-active: rgba(0, 0, 0, 0.1);--button-opacity: 0.5;position:relative;overflow:auto}.dj-richtext-wrapper [role=menubar]{border:none;position:absolute;inset:0 0 auto 0;padding:.125rem .25rem}.dj-richtext-wrapper [role=menubar] [role=separator]{display:inline-block;padding:.25rem 0;vertical-align:middle}.dj-richtext-wrapper [role=menubar] button{display:inline-block;text-align:center;text-decoration:none;vertical-align:middle;cursor:pointer;-webkit-user-select:none;-moz-user-select:none;user-select:none;border:none;border-radius:.25rem;padding:.25rem;background-color:inherit;opacity:var(--button-opacity)}.dj-richtext-wrapper [role=menubar] button:hover{opacity:1}.dj-richtext-wrapper [role=menubar] button.active{opacity:1;background-color:var(--button-active)}.dj-richtext-wrapper [role=menubar] button[aria-haspopup=true]:after{border-bottom:0;border-left:.3em solid rgba(0,0,0,0);border-right:.3em solid rgba(0,0,0,0);border-top:.3em solid;margin-right:.125rem;content:"";display:inline-block;transition:transform 250ms ease-in-out}.dj-richtext-wrapper [role=menubar] button[aria-haspopup=true][aria-expanded=true]:after{transform:scaleY(-1)}.dj-richtext-wrapper [role=menubar] button[aria-haspopup=true]+ul[role=menu]{display:none;padding:inherit;list-style:none;background-color:inherit;border-color:#000}.dj-richtext-wrapper [role=menubar] button[aria-haspopup=true]+ul[role=menu]>li{background-color:inherit;opacity:var(--button-opacity)}.dj-richtext-wrapper [role=menubar] button[aria-haspopup=true]+ul[role=menu]>li:hover{opacity:1}.dj-richtext-wrapper [role=menubar] button[aria-haspopup=true]+ul[role=menu]>li.active{color:inherit;opacity:1;background-color:var(--button-active)}.dj-richtext-wrapper [role=menubar] button[aria-haspopup=true][aria-expanded=true]+ul[role=menu]{display:block}.dj-richtext-wrapper [role=menubar] button>svg{vertical-align:middle;display:inline}.dj-richtext-wrapper .character-count{position:absolute;bottom:3px;right:6px;color:rgba(0,0,0,.2)}.dj-richtext-wrapper .ProseMirror{border:none;position:absolute;left:0;right:0;bottom:0;word-wrap:break-word;white-space:break-spaces;font-variant-ligatures:none;font-feature-settings:"liga" 0;overflow:hidden}.dj-richtext-wrapper .ProseMirror[contenteditable=false]{white-space:normal}.dj-richtext-wrapper .ProseMirror p{margin-bottom:.5rem}.dj-richtext-wrapper .ProseMirror p.is-editor-empty:first-child::before{color:rgba(0,0,0,.2);content:attr(data-placeholder);float:left;height:0;pointer-events:none}.dj-richtext-wrapper .ProseMirror p[data-text=indent]{text-indent:3em}.dj-richtext-wrapper .ProseMirror p[data-text=outdent]{text-indent:-3em;padding-left:3em}.dj-richtext-wrapper .ProseMirror p[data-text-indent="1"]{margin-left:2em}.dj-richtext-wrapper .ProseMirror p[data-text-indent="2"]{margin-left:4em}.dj-richtext-wrapper .ProseMirror p[data-text-indent="3"]{margin-left:6em}.dj-richtext-wrapper .ProseMirror p[data-text-indent="4"]{margin-left:8em}.dj-richtext-wrapper .ProseMirror p[data-text-indent="5"]{margin-left:10em}.dj-richtext-wrapper .ProseMirror p[data-text-indent="6"]{margin-left:12em}.dj-richtext-wrapper .ProseMirror p[data-text-indent="7"]{margin-left:14em}.dj-richtext-wrapper .ProseMirror p[data-text-indent="8"]{margin-left:16em}.dj-richtext-wrapper .ProseMirror p[data-text-indent="9"]{margin-left:18em}.dj-richtext-wrapper .ProseMirror p[data-text-indent="10"]{margin-left:20em}.dj-richtext-wrapper .ProseMirror li>p{margin:0}.dj-richtext-wrapper .ProseMirror:focus-visible{outline:none}.dj-richtext-wrapper .ProseMirror blockquote{border-left:3px solid rgba(0,0,0,.2);padding-left:1rem}.dj-richtext-wrapper .ProseMirror output[role=placeholder]{background-color:rgba(0,0,0,.03);box-shadow:inset 0 0 5px rgba(0,0,0,.7)}.dj-richtext-wrapper .ProseMirror pre{padding:.5rem 1rem;background-color:rgba(0,0,0,.03);font-family:monospace}.dj-richtext-wrapper .ProseMirror pre{white-space:pre-wrap}.dj-richtext-wrapper.focused{opacity:1}.dj-submitted .dj-richtext-wrapper.focused.invalid{opacity:1}.dj-richtext-wrapper:not(.focused).invalid{border-color:var(--django-formset-color-invalid)}.dj-richtext-wrapper:not(.focused).valid{border-color:var(--django-formset-color-valid)}';
-var _ = "top",
-    oe = "bottom",
-    ne = "right",
-    Y = "left",
-    Pr = "auto",
-    Tt = [_, oe, ne, Y],
-    dt = "start",
-    Kt = "end",
-    hl = "clippingParents",
-    Rr = "viewport",
-    Mn = "popper",
-    ml = "reference",
-    Ji = Tt.reduce(function(n, e) {
-        return n.concat([e + "-" + dt, e + "-" + Kt])
-    }, []),
-    Br = [].concat(Tt, [Pr]).reduce(function(n, e) {
-        return n.concat([e, e + "-" + dt, e + "-" + Kt])
-    }, []),
-    gd = "beforeRead",
-    yd = "read",
-    xd = "afterRead",
-    bd = "beforeMain",
-    kd = "main",
-    vd = "afterMain",
-    Md = "beforeWrite",
-    Ed = "write",
-    Sd = "afterWrite",
-    gl = [gd, yd, xd, bd, kd, vd, Md, Ed, Sd];
-
-function le(n) {
-    return n ? (n.nodeName || "").toLowerCase() : null
-}
-
-function $(n) {
-    if (n == null) return window;
-    if (n.toString() !== "[object Window]") {
-        var e = n.ownerDocument;
-        return e && e.defaultView || window
-    }
-    return n
-}
-
-function Le(n) {
-    var e = $(n).Element;
-    return n instanceof e || n instanceof Element
-}
-
-function se(n) {
-    var e = $(n).HTMLElement;
-    return n instanceof e || n instanceof HTMLElement
-}
-
-function En(n) {
-    if (typeof ShadowRoot > "u") return !1;
-    var e = $(n).ShadowRoot;
-    return n instanceof e || n instanceof ShadowRoot
-}
-
-function wd(n) {
-    var e = n.state;
-    Object.keys(e.elements).forEach(function(t) {
-        var r = e.styles[t] || {},
-            i = e.attributes[t] || {},
-            o = e.elements[t];
-        !se(o) || !le(o) || (Object.assign(o.style, r), Object.keys(i).forEach(function(s) {
-            var l = i[s];
-            l === !1 ? o.removeAttribute(s) : o.setAttribute(s, l === !0 ? "" : l)
-        }))
-    })
-}
-
-function Td(n) {
-    var e = n.state,
-        t = {
-            popper: {
-                position: e.options.strategy,
-                left: "0",
-                top: "0",
-                margin: "0"
-            },
-            arrow: {
-                position: "absolute"
-            },
-            reference: {}
-        };
-    return Object.assign(e.elements.popper.style, t.popper), e.styles = t, e.elements.arrow && Object.assign(e.elements.arrow.style, t.arrow),
-        function() {
-            Object.keys(e.elements).forEach(function(r) {
-                var i = e.elements[r],
-                    o = e.attributes[r] || {},
-                    s = Object.keys(e.styles.hasOwnProperty(r) ? e.styles[r] : t[r]),
-                    l = s.reduce(function(a, c) {
-                        return a[c] = "", a
-                    }, {});
-                !se(i) || !le(i) || (Object.assign(i.style, l), Object.keys(o).forEach(function(a) {
-                    i.removeAttribute(a)
-                }))
-            })
-        }
-}
-var yl = {
-    name: "applyStyles",
-    enabled: !0,
-    phase: "write",
-    fn: wd,
-    effect: Td,
-    requires: ["computeStyles"]
-};
-
-function ae(n) {
-    return n.split("-")[0]
-}
-var We = Math.max,
-    Ut = Math.min,
-    ft = Math.round;
-
-function Sn() {
-    var n = navigator.userAgentData;
-    return n != null && n.brands && Array.isArray(n.brands) ? n.brands.map(function(e) {
-        return e.brand + "/" + e.version
-    }).join(" ") : navigator.userAgent
-}
-
-function er() {
-    return !/^((?!chrome|android).)*safari/i.test(Sn())
-}
-
-function Pe(n, e, t) {
-    e === void 0 && (e = !1), t === void 0 && (t = !1);
-    var r = n.getBoundingClientRect(),
-        i = 1,
-        o = 1;
-    e && se(n) && (i = n.offsetWidth > 0 && ft(r.width) / n.offsetWidth || 1, o = n.offsetHeight > 0 && ft(r.height) / n.offsetHeight || 1);
-    var s = Le(n) ? $(n) : window,
-        l = s.visualViewport,
-        a = !er() && t,
-        c = (r.left + (a && l ? l.offsetLeft : 0)) / i,
-        u = (r.top + (a && l ? l.offsetTop : 0)) / o,
-        d = r.width / i,
-        f = r.height / o;
-    return {
-        width: d,
-        height: f,
-        top: u,
-        right: c + d,
-        bottom: u + f,
-        left: c,
-        x: c,
-        y: u
-    }
-}
-
-function _t(n) {
-    var e = Pe(n),
-        t = n.offsetWidth,
-        r = n.offsetHeight;
-    return Math.abs(e.width - t) <= 1 && (t = e.width), Math.abs(e.height - r) <= 1 && (r = e.height), {
-        x: n.offsetLeft,
-        y: n.offsetTop,
-        width: t,
-        height: r
-    }
-}
-
-function tr(n, e) {
-    var t = e.getRootNode && e.getRootNode();
-    if (n.contains(e)) return !0;
-    if (t && En(t)) {
-        var r = e;
-        do {
-            if (r && n.isSameNode(r)) return !0;
-            r = r.parentNode || r.host
-        } while (r)
-    }
-    return !1
-}
-
-function be(n) {
-    return $(n).getComputedStyle(n)
-}
-
-function Ki(n) {
-    return ["table", "td", "th"].indexOf(le(n)) >= 0
-}
-
-function de(n) {
-    return ((Le(n) ? n.ownerDocument : n.document) || window.document).documentElement
-}
-
-function pt(n) {
-    return le(n) === "html" ? n : n.assignedSlot || n.parentNode || (En(n) ? n.host : null) || de(n)
-}
-
-function xl(n) {
-    return !se(n) || be(n).position === "fixed" ? null : n.offsetParent
-}
-
-function Cd(n) {
-    var e = /firefox/i.test(Sn()),
-        t = /Trident/i.test(Sn());
-    if (t && se(n)) {
-        var r = be(n);
-        if (r.position === "fixed") return null
-    }
-    var i = pt(n);
-    for (En(i) && (i = i.host); se(i) && ["html", "body"].indexOf(le(i)) < 0;) {
-        var o = be(i);
-        if (o.transform !== "none" || o.perspective !== "none" || o.contain === "paint" || ["transform", "perspective"].indexOf(o.willChange) !== -1 || e && o.willChange === "filter" || e && o.filter && o.filter !== "none") return i;
-        i = i.parentNode
-    }
-    return null
-}
-
-function qe(n) {
-    for (var e = $(n), t = xl(n); t && Ki(t) && be(t).position === "static";) t = xl(t);
-    return t && (le(t) === "html" || le(t) === "body" && be(t).position === "static") ? e : t || Cd(n) || e
-}
-
-function Gt(n) {
-    return ["top", "bottom"].indexOf(n) >= 0 ? "x" : "y"
-}
-
-function Yt(n, e, t) {
-    return We(n, Ut(e, t))
-}
-
-function bl(n, e, t) {
-    var r = Yt(n, e, t);
-    return r > t ? t : r
-}
-
-function nr() {
-    return {
-        top: 0,
-        right: 0,
-        bottom: 0,
-        left: 0
-    }
-}
-
-function rr(n) {
-    return Object.assign({}, nr(), n)
-}
-
-function ir(n, e) {
-    return e.reduce(function(t, r) {
-        return t[r] = n, t
-    }, {})
-}
-var Od = function(e, t) {
-    return e = typeof e == "function" ? e(Object.assign({}, t.rects, {
-        placement: t.placement
-    })) : e, rr(typeof e != "number" ? e : ir(e, Tt))
-};
-
-function Ad(n) {
-    var e, t = n.state,
-        r = n.name,
-        i = n.options,
-        o = t.elements.arrow,
-        s = t.modifiersData.popperOffsets,
-        l = ae(t.placement),
-        a = Gt(l),
-        c = [Y, ne].indexOf(l) >= 0,
-        u = c ? "height" : "width";
-    if (!(!o || !s)) {
-        var d = Od(i.padding, t),
-            f = _t(o),
-            p = a === "y" ? _ : Y,
-            h = a === "y" ? oe : ne,
-            m = t.rects.reference[u] + t.rects.reference[a] - s[a] - t.rects.popper[u],
-            b = s[a] - t.rects.reference[a],
-            k = qe(o),
-            S = k ? a === "y" ? k.clientHeight || 0 : k.clientWidth || 0 : 0,
-            C = m / 2 - b / 2,
-            T = d[p],
-            E = S - f[u] - d[h],
-            g = S / 2 - f[u] / 2 + C,
-            x = Yt(T, g, E),
-            y = a;
-        t.modifiersData[r] = (e = {}, e[y] = x, e.centerOffset = x - g, e)
-    }
-}
-
-function Nd(n) {
-    var e = n.state,
-        t = n.options,
-        r = t.element,
-        i = r === void 0 ? "[data-popper-arrow]" : r;
-    i != null && (typeof i == "string" && (i = e.elements.popper.querySelector(i), !i) || tr(e.elements.popper, i) && (e.elements.arrow = i))
-}
-var kl = {
-    name: "arrow",
-    enabled: !0,
-    phase: "main",
-    fn: Ad,
-    effect: Nd,
-    requires: ["popperOffsets"],
-    requiresIfExists: ["preventOverflow"]
-};
-
-function Re(n) {
-    return n.split("-")[1]
-}
-var Id = {
-    top: "auto",
-    right: "auto",
-    bottom: "auto",
-    left: "auto"
-};
-
-function Dd(n, e) {
-    var t = n.x,
-        r = n.y,
-        i = e.devicePixelRatio || 1;
-    return {
-        x: ft(t * i) / i || 0,
-        y: ft(r * i) / i || 0
-    }
-}
-
-function vl(n) {
-    var e, t = n.popper,
-        r = n.popperRect,
-        i = n.placement,
-        o = n.variation,
-        s = n.offsets,
-        l = n.position,
-        a = n.gpuAcceleration,
-        c = n.adaptive,
-        u = n.roundOffsets,
-        d = n.isFixed,
-        f = s.x,
-        p = f === void 0 ? 0 : f,
-        h = s.y,
-        m = h === void 0 ? 0 : h,
-        b = typeof u == "function" ? u({
-            x: p,
-            y: m
-        }) : {
-            x: p,
-            y: m
-        };
-    p = b.x, m = b.y;
-    var k = s.hasOwnProperty("x"),
-        S = s.hasOwnProperty("y"),
-        C = Y,
-        T = _,
-        E = window;
-    if (c) {
-        var g = qe(t),
-            x = "clientHeight",
-            y = "clientWidth";
-        if (g === $(t) && (g = de(t), be(g).position !== "static" && l === "absolute" && (x = "scrollHeight", y = "scrollWidth")), g = g, i === _ || (i === Y || i === ne) && o === Kt) {
-            T = oe;
-            var O = d && g === E && E.visualViewport ? E.visualViewport.height : g[x];
-            m -= O - r.height, m *= a ? 1 : -1
-        }
-        if (i === Y || (i === _ || i === oe) && o === Kt) {
-            C = ne;
-            var I = d && g === E && E.visualViewport ? E.visualViewport.width : g[y];
-            p -= I - r.width, p *= a ? 1 : -1
-        }
-    }
-    var L = Object.assign({
-            position: l
-        }, c && Id),
-        j = u === !0 ? Dd({
-            x: p,
-            y: m
-        }, $(t)) : {
-            x: p,
-            y: m
-        };
-    if (p = j.x, m = j.y, a) {
-        var ee;
-        return Object.assign({}, L, (ee = {}, ee[T] = S ? "0" : "", ee[C] = k ? "0" : "", ee.transform = (E.devicePixelRatio || 1) <= 1 ? "translate(" + p + "px, " + m + "px)" : "translate3d(" + p + "px, " + m + "px, 0)", ee))
-    }
-    return Object.assign({}, L, (e = {}, e[T] = S ? m + "px" : "", e[C] = k ? p + "px" : "", e.transform = "", e))
-}
-
-function Ld(n) {
-    var e = n.state,
-        t = n.options,
-        r = t.gpuAcceleration,
-        i = r === void 0 ? !0 : r,
-        o = t.adaptive,
-        s = o === void 0 ? !0 : o,
-        l = t.roundOffsets,
-        a = l === void 0 ? !0 : l;
-    if (!1) var c;
-    var u = {
-        placement: ae(e.placement),
-        variation: Re(e.placement),
-        popper: e.elements.popper,
-        popperRect: e.rects.popper,
-        gpuAcceleration: i,
-        isFixed: e.options.strategy === "fixed"
-    };
-    e.modifiersData.popperOffsets != null && (e.styles.popper = Object.assign({}, e.styles.popper, vl(Object.assign({}, u, {
-        offsets: e.modifiersData.popperOffsets,
-        position: e.options.strategy,
-        adaptive: s,
-        roundOffsets: a
-    })))), e.modifiersData.arrow != null && (e.styles.arrow = Object.assign({}, e.styles.arrow, vl(Object.assign({}, u, {
-        offsets: e.modifiersData.arrow,
-        position: "absolute",
-        adaptive: !1,
-        roundOffsets: a
-    })))), e.attributes.popper = Object.assign({}, e.attributes.popper, {
-        "data-popper-placement": e.placement
-    })
-}
-var Ml = {
-    name: "computeStyles",
-    enabled: !0,
-    phase: "beforeWrite",
-    fn: Ld,
-    data: {}
-};
-var zr = {
-    passive: !0
-};
-
-function Pd(n) {
-    var e = n.state,
-        t = n.instance,
-        r = n.options,
-        i = r.scroll,
-        o = i === void 0 ? !0 : i,
-        s = r.resize,
-        l = s === void 0 ? !0 : s,
-        a = $(e.elements.popper),
-        c = [].concat(e.scrollParents.reference, e.scrollParents.popper);
-    return o && c.forEach(function(u) {
-            u.addEventListener("scroll", t.update, zr)
-        }), l && a.addEventListener("resize", t.update, zr),
-        function() {
-            o && c.forEach(function(u) {
-                u.removeEventListener("scroll", t.update, zr)
-            }), l && a.removeEventListener("resize", t.update, zr)
-        }
-}
-var El = {
-    name: "eventListeners",
-    enabled: !0,
-    phase: "write",
-    fn: function() {},
-    effect: Pd,
-    data: {}
-};
-var Rd = {
-    left: "right",
-    right: "left",
-    bottom: "top",
-    top: "bottom"
-};
-
-function wn(n) {
-    return n.replace(/left|right|bottom|top/g, function(e) {
-        return Rd[e]
-    })
-}
-var Bd = {
-    start: "end",
-    end: "start"
-};
-
-function Hr(n) {
-    return n.replace(/start|end/g, function(e) {
-        return Bd[e]
-    })
-}
-
-function Qt(n) {
-    var e = $(n),
-        t = e.pageXOffset,
-        r = e.pageYOffset;
-    return {
-        scrollLeft: t,
-        scrollTop: r
-    }
-}
-
-function Xt(n) {
-    return Pe(de(n)).left + Qt(n).scrollLeft
-}
-
-function Ui(n, e) {
-    var t = $(n),
-        r = de(n),
-        i = t.visualViewport,
-        o = r.clientWidth,
-        s = r.clientHeight,
-        l = 0,
-        a = 0;
-    if (i) {
-        o = i.width, s = i.height;
-        var c = er();
-        (c || !c && e === "fixed") && (l = i.offsetLeft, a = i.offsetTop)
-    }
-    return {
-        width: o,
-        height: s,
-        x: l + Xt(n),
-        y: a
-    }
-}
-
-function _i(n) {
-    var e, t = de(n),
-        r = Qt(n),
-        i = (e = n.ownerDocument) == null ? void 0 : e.body,
-        o = We(t.scrollWidth, t.clientWidth, i ? i.scrollWidth : 0, i ? i.clientWidth : 0),
-        s = We(t.scrollHeight, t.clientHeight, i ? i.scrollHeight : 0, i ? i.clientHeight : 0),
-        l = -r.scrollLeft + Xt(n),
-        a = -r.scrollTop;
-    return be(i || t).direction === "rtl" && (l += We(t.clientWidth, i ? i.clientWidth : 0) - o), {
-        width: o,
-        height: s,
-        x: l,
-        y: a
-    }
-}
-
-function Zt(n) {
-    var e = be(n),
-        t = e.overflow,
-        r = e.overflowX,
-        i = e.overflowY;
-    return /auto|scroll|overlay|hidden/.test(t + i + r)
-}
-
-function Fr(n) {
-    return ["html", "body", "#document"].indexOf(le(n)) >= 0 ? n.ownerDocument.body : se(n) && Zt(n) ? n : Fr(pt(n))
-}
-
-function Ct(n, e) {
-    var t;
-    e === void 0 && (e = []);
-    var r = Fr(n),
-        i = r === ((t = n.ownerDocument) == null ? void 0 : t.body),
-        o = $(r),
-        s = i ? [o].concat(o.visualViewport || [], Zt(r) ? r : []) : r,
-        l = e.concat(s);
-    return i ? l : l.concat(Ct(pt(s)))
-}
-
-function Tn(n) {
-    return Object.assign({}, n, {
-        left: n.x,
-        top: n.y,
-        right: n.x + n.width,
-        bottom: n.y + n.height
-    })
-}
+var Js = '.dj-richtext-wrapper{--button-active: rgba(0, 0, 0, 0.1);--button-opacity: 0.5;position:relative;overflow:auto}.dj-richtext-wrapper [role=menubar]{border:none;position:absolute;inset:0 0 auto 0;padding:.125rem .25rem}.dj-richtext-wrapper [role=menubar] [role=separator]{display:inline-block;padding:.25rem 0;vertical-align:middle}.dj-richtext-wrapper [role=menubar] button{display:inline-block;text-align:center;text-decoration:none;vertical-align:middle;cursor:pointer;-webkit-user-select:none;-moz-user-select:none;user-select:none;border:none;border-radius:.25rem;padding:.25rem;background-color:inherit;opacity:var(--button-opacity)}.dj-richtext-wrapper [role=menubar] button:hover{opacity:1}.dj-richtext-wrapper [role=menubar] button.active{opacity:1;background-color:var(--button-active)}.dj-richtext-wrapper [role=menubar] button[aria-haspopup=true]:after{border-bottom:0;border-left:.3em solid rgba(0,0,0,0);border-right:.3em solid rgba(0,0,0,0);border-top:.3em solid;margin-right:.125rem;content:"";display:inline-block;transition:transform 250ms ease-in-out}.dj-richtext-wrapper [role=menubar] button[aria-haspopup=true][aria-expanded=true]:after{transform:scaleY(-1)}.dj-richtext-wrapper [role=menubar] button[aria-haspopup=true]+ul[role=menu]{display:none;position:absolute;width:max-content;top:0;left:0;padding:inherit;list-style:none;background-color:inherit;border-color:#000}.dj-richtext-wrapper [role=menubar] button[aria-haspopup=true]+ul[role=menu]>li{background-color:inherit;opacity:var(--button-opacity)}.dj-richtext-wrapper [role=menubar] button[aria-haspopup=true]+ul[role=menu]>li:hover{opacity:1}.dj-richtext-wrapper [role=menubar] button[aria-haspopup=true]+ul[role=menu]>li.active{color:inherit;opacity:1;background-color:var(--button-active)}.dj-richtext-wrapper [role=menubar] button[aria-haspopup=true][aria-expanded=true]+ul[role=menu]{display:block}.dj-richtext-wrapper [role=menubar] button>svg{vertical-align:middle;display:inline}.dj-richtext-wrapper .character-count{position:absolute;bottom:3px;right:6px;color:rgba(0,0,0,.2)}.dj-richtext-wrapper .ProseMirror{border:none;position:absolute;left:0;right:0;bottom:0;word-wrap:break-word;white-space:break-spaces;font-variant-ligatures:none;font-feature-settings:"liga" 0;overflow:hidden}.dj-richtext-wrapper .ProseMirror[contenteditable=false]{white-space:normal}.dj-richtext-wrapper .ProseMirror p{margin-bottom:.5rem}.dj-richtext-wrapper .ProseMirror p.is-editor-empty:first-child::before{color:rgba(0,0,0,.2);content:attr(data-placeholder);float:left;height:0;pointer-events:none}.dj-richtext-wrapper .ProseMirror p[data-text=indent]{text-indent:3em}.dj-richtext-wrapper .ProseMirror p[data-text=outdent]{text-indent:-3em;padding-left:3em}.dj-richtext-wrapper .ProseMirror p[data-text-indent="1"]{margin-left:2em}.dj-richtext-wrapper .ProseMirror p[data-text-indent="2"]{margin-left:4em}.dj-richtext-wrapper .ProseMirror p[data-text-indent="3"]{margin-left:6em}.dj-richtext-wrapper .ProseMirror p[data-text-indent="4"]{margin-left:8em}.dj-richtext-wrapper .ProseMirror p[data-text-indent="5"]{margin-left:10em}.dj-richtext-wrapper .ProseMirror p[data-text-indent="6"]{margin-left:12em}.dj-richtext-wrapper .ProseMirror p[data-text-indent="7"]{margin-left:14em}.dj-richtext-wrapper .ProseMirror p[data-text-indent="8"]{margin-left:16em}.dj-richtext-wrapper .ProseMirror p[data-text-indent="9"]{margin-left:18em}.dj-richtext-wrapper .ProseMirror p[data-text-indent="10"]{margin-left:20em}.dj-richtext-wrapper .ProseMirror li>p{margin:0}.dj-richtext-wrapper .ProseMirror:focus-visible{outline:none}.dj-richtext-wrapper .ProseMirror blockquote{border-left:3px solid rgba(0,0,0,.2);padding-left:1rem}.dj-richtext-wrapper .ProseMirror output[role=placeholder]{background-color:rgba(0,0,0,.03);box-shadow:inset 0 0 5px rgba(0,0,0,.7)}.dj-richtext-wrapper .ProseMirror pre{padding:.5rem 1rem;background-color:rgba(0,0,0,.03);font-family:monospace}.dj-richtext-wrapper .ProseMirror pre{white-space:pre-wrap}.dj-richtext-wrapper.focused{opacity:1}.dj-submitted .dj-richtext-wrapper.focused.invalid{opacity:1}.dj-richtext-wrapper:not(.focused).invalid{border-color:var(--django-formset-color-invalid)}.dj-richtext-wrapper:not(.focused).valid{border-color:var(--django-formset-color-valid)}';
 
-function zd(n, e) {
-    var t = Pe(n, !1, e === "fixed");
-    return t.top = t.top + n.clientTop, t.left = t.left + n.clientLeft, t.bottom = t.top + n.clientHeight, t.right = t.left + n.clientWidth, t.width = n.clientWidth, t.height = n.clientHeight, t.x = t.left, t.y = t.top, t
-}
-
-function Sl(n, e, t) {
-    return e === Rr ? Tn(Ui(n, t)) : Le(e) ? zd(e, t) : Tn(_i(de(n)))
-}
-
-function Hd(n) {
-    var e = Ct(pt(n)),
-        t = ["absolute", "fixed"].indexOf(be(n).position) >= 0,
-        r = t && se(n) ? qe(n) : n;
-    return Le(r) ? e.filter(function(i) {
-        return Le(i) && tr(i, r) && le(i) !== "body"
-    }) : []
-}
-
-function Gi(n, e, t, r) {
-    var i = e === "clippingParents" ? Hd(n) : [].concat(e),
-        o = [].concat(i, [t]),
-        s = o[0],
-        l = o.reduce(function(a, c) {
-            var u = Sl(n, c, r);
-            return a.top = We(u.top, a.top), a.right = Ut(u.right, a.right), a.bottom = Ut(u.bottom, a.bottom), a.left = We(u.left, a.left), a
-        }, Sl(n, s, r));
-    return l.width = l.right - l.left, l.height = l.bottom - l.top, l.x = l.left, l.y = l.top, l
-}
-
-function or(n) {
-    var e = n.reference,
-        t = n.element,
-        r = n.placement,
-        i = r ? ae(r) : null,
-        o = r ? Re(r) : null,
-        s = e.x + e.width / 2 - t.width / 2,
-        l = e.y + e.height / 2 - t.height / 2,
-        a;
-    switch (i) {
-        case _:
-            a = {
-                x: s,
-                y: e.y - t.height
-            };
-            break;
-        case oe:
-            a = {
-                x: s,
-                y: e.y + e.height
-            };
-            break;
-        case ne:
-            a = {
-                x: e.x + e.width,
-                y: l
-            };
-            break;
-        case Y:
-            a = {
-                x: e.x - t.width,
-                y: l
-            };
-            break;
-        default:
-            a = {
-                x: e.x,
-                y: e.y
-            }
-    }
-    var c = i ? Gt(i) : null;
-    if (c != null) {
-        var u = c === "y" ? "height" : "width";
-        switch (o) {
-            case dt:
-                a[c] = a[c] - (e[u] / 2 - t[u] / 2);
-                break;
-            case Kt:
-                a[c] = a[c] + (e[u] / 2 - t[u] / 2);
-                break;
-            default:
-        }
-    }
-    return a
-}
-
-function Je(n, e) {
-    e === void 0 && (e = {});
-    var t = e,
-        r = t.placement,
-        i = r === void 0 ? n.placement : r,
-        o = t.strategy,
-        s = o === void 0 ? n.strategy : o,
-        l = t.boundary,
-        a = l === void 0 ? hl : l,
-        c = t.rootBoundary,
-        u = c === void 0 ? Rr : c,
-        d = t.elementContext,
-        f = d === void 0 ? Mn : d,
-        p = t.altBoundary,
-        h = p === void 0 ? !1 : p,
-        m = t.padding,
-        b = m === void 0 ? 0 : m,
-        k = rr(typeof b != "number" ? b : ir(b, Tt)),
-        S = f === Mn ? ml : Mn,
-        C = n.rects.popper,
-        T = n.elements[h ? S : f],
-        E = Gi(Le(T) ? T : T.contextElement || de(n.elements.popper), a, u, s),
-        g = Pe(n.elements.reference),
-        x = or({
-            reference: g,
-            element: C,
-            strategy: "absolute",
-            placement: i
-        }),
-        y = Tn(Object.assign({}, C, x)),
-        O = f === Mn ? y : g,
-        I = {
-            top: E.top - O.top + k.top,
-            bottom: O.bottom - E.bottom + k.bottom,
-            left: E.left - O.left + k.left,
-            right: O.right - E.right + k.right
-        },
-        L = n.modifiersData.offset;
-    if (f === Mn && L) {
-        var j = L[i];
-        Object.keys(I).forEach(function(ee) {
-            var Ne = [ne, oe].indexOf(ee) >= 0 ? 1 : -1,
-                Ie = [_, oe].indexOf(ee) >= 0 ? "y" : "x";
-            I[ee] += j[Ie] * Ne
-        })
-    }
-    return I
-}
-
-function Yi(n, e) {
-    e === void 0 && (e = {});
-    var t = e,
-        r = t.placement,
-        i = t.boundary,
-        o = t.rootBoundary,
-        s = t.padding,
-        l = t.flipVariations,
-        a = t.allowedAutoPlacements,
-        c = a === void 0 ? Br : a,
-        u = Re(r),
-        d = u ? l ? Ji : Ji.filter(function(h) {
-            return Re(h) === u
-        }) : Tt,
-        f = d.filter(function(h) {
-            return c.indexOf(h) >= 0
-        });
-    f.length === 0 && (f = d);
-    var p = f.reduce(function(h, m) {
-        return h[m] = Je(n, {
-            placement: m,
-            boundary: i,
-            rootBoundary: o,
-            padding: s
-        })[ae(m)], h
-    }, {});
-    return Object.keys(p).sort(function(h, m) {
-        return p[h] - p[m]
-    })
-}
-
-function Fd(n) {
-    if (ae(n) === Pr) return [];
-    var e = wn(n);
-    return [Hr(n), e, Hr(e)]
-}
-
-function jd(n) {
-    var e = n.state,
-        t = n.options,
-        r = n.name;
-    if (!e.modifiersData[r]._skip) {
-        for (var i = t.mainAxis, o = i === void 0 ? !0 : i, s = t.altAxis, l = s === void 0 ? !0 : s, a = t.fallbackPlacements, c = t.padding, u = t.boundary, d = t.rootBoundary, f = t.altBoundary, p = t.flipVariations, h = p === void 0 ? !0 : p, m = t.allowedAutoPlacements, b = e.options.placement, k = ae(b), S = k === b, C = a || (S || !h ? [wn(b)] : Fd(b)), T = [b].concat(C).reduce(function(vn, St) {
-                return vn.concat(ae(St) === Pr ? Yi(e, {
-                    placement: St,
-                    boundary: u,
-                    rootBoundary: d,
-                    padding: c,
-                    flipVariations: h,
-                    allowedAutoPlacements: m
-                }) : St)
-            }, []), E = e.rects.reference, g = e.rects.popper, x = new Map, y = !0, O = T[0], I = 0; I < T.length; I++) {
-            var L = T[I],
-                j = ae(L),
-                ee = Re(L) === dt,
-                Ne = [_, oe].indexOf(j) >= 0,
-                Ie = Ne ? "width" : "height",
-                te = Je(e, {
-                    placement: L,
-                    boundary: u,
-                    rootBoundary: d,
-                    altBoundary: f,
-                    padding: c
-                }),
-                ie = Ne ? ee ? ne : Y : ee ? oe : _;
-            E[Ie] > g[Ie] && (ie = wn(ie));
-            var De = wn(ie),
-                xe = [];
-            if (o && xe.push(te[j] <= 0), l && xe.push(te[ie] <= 0, te[De] <= 0), xe.every(function(vn) {
-                    return vn
-                })) {
-                O = L, y = !1;
-                break
-            }
-            x.set(L, xe)
-        }
-        if (y)
-            for (var Ge = h ? 3 : 1, Et = function(St) {
-                    var Zn = T.find(function(Dr) {
-                        var qt = x.get(Dr);
-                        if (qt) return qt.slice(0, St).every(function($i) {
-                            return $i
-                        })
-                    });
-                    if (Zn) return O = Zn, "break"
-                }, Ye = Ge; Ye > 0; Ye--) {
-                var ut = Et(Ye);
-                if (ut === "break") break
-            }
-        e.placement !== O && (e.modifiersData[r]._skip = !0, e.placement = O, e.reset = !0)
-    }
-}
-var wl = {
-    name: "flip",
-    enabled: !0,
-    phase: "main",
-    fn: jd,
-    requiresIfExists: ["offset"],
-    data: {
-        _skip: !1
-    }
-};
-
-function Tl(n, e, t) {
-    return t === void 0 && (t = {
-        x: 0,
-        y: 0
-    }), {
-        top: n.top - e.height - t.y,
-        right: n.right - e.width + t.x,
-        bottom: n.bottom - e.height + t.y,
-        left: n.left - e.width - t.x
-    }
-}
-
-function Cl(n) {
-    return [_, ne, oe, Y].some(function(e) {
-        return n[e] >= 0
-    })
-}
-
-function Vd(n) {
-    var e = n.state,
-        t = n.name,
-        r = e.rects.reference,
-        i = e.rects.popper,
-        o = e.modifiersData.preventOverflow,
-        s = Je(e, {
-            elementContext: "reference"
-        }),
-        l = Je(e, {
-            altBoundary: !0
-        }),
-        a = Tl(s, r),
-        c = Tl(l, i, o),
-        u = Cl(a),
-        d = Cl(c);
-    e.modifiersData[t] = {
-        referenceClippingOffsets: a,
-        popperEscapeOffsets: c,
-        isReferenceHidden: u,
-        hasPopperEscaped: d
-    }, e.attributes.popper = Object.assign({}, e.attributes.popper, {
-        "data-popper-reference-hidden": u,
-        "data-popper-escaped": d
-    })
-}
-var Ol = {
-    name: "hide",
-    enabled: !0,
-    phase: "main",
-    requiresIfExists: ["preventOverflow"],
-    fn: Vd
-};
-
-function $d(n, e, t) {
-    var r = ae(n),
-        i = [Y, _].indexOf(r) >= 0 ? -1 : 1,
-        o = typeof t == "function" ? t(Object.assign({}, e, {
-            placement: n
-        })) : t,
-        s = o[0],
-        l = o[1];
-    return s = s || 0, l = (l || 0) * i, [Y, ne].indexOf(r) >= 0 ? {
-        x: l,
-        y: s
-    } : {
-        x: s,
-        y: l
-    }
-}
-
-function Wd(n) {
-    var e = n.state,
-        t = n.options,
-        r = n.name,
-        i = t.offset,
-        o = i === void 0 ? [0, 0] : i,
-        s = Br.reduce(function(u, d) {
-            return u[d] = $d(d, e.rects, o), u
-        }, {}),
-        l = s[e.placement],
-        a = l.x,
-        c = l.y;
-    e.modifiersData.popperOffsets != null && (e.modifiersData.popperOffsets.x += a, e.modifiersData.popperOffsets.y += c), e.modifiersData[r] = s
-}
-var Al = {
-    name: "offset",
-    enabled: !0,
-    phase: "main",
-    requires: ["popperOffsets"],
-    fn: Wd
-};
-
-function qd(n) {
-    var e = n.state,
-        t = n.name;
-    e.modifiersData[t] = or({
-        reference: e.rects.reference,
-        element: e.rects.popper,
-        strategy: "absolute",
-        placement: e.placement
-    })
-}
-var Nl = {
-    name: "popperOffsets",
-    enabled: !0,
-    phase: "read",
-    fn: qd,
-    data: {}
-};
-
-function Qi(n) {
-    return n === "x" ? "y" : "x"
-}
-
-function Jd(n) {
-    var e = n.state,
-        t = n.options,
-        r = n.name,
-        i = t.mainAxis,
-        o = i === void 0 ? !0 : i,
-        s = t.altAxis,
-        l = s === void 0 ? !1 : s,
-        a = t.boundary,
-        c = t.rootBoundary,
-        u = t.altBoundary,
-        d = t.padding,
-        f = t.tether,
-        p = f === void 0 ? !0 : f,
-        h = t.tetherOffset,
-        m = h === void 0 ? 0 : h,
-        b = Je(e, {
-            boundary: a,
-            rootBoundary: c,
-            padding: d,
-            altBoundary: u
-        }),
-        k = ae(e.placement),
-        S = Re(e.placement),
-        C = !S,
-        T = Gt(k),
-        E = Qi(T),
-        g = e.modifiersData.popperOffsets,
-        x = e.rects.reference,
-        y = e.rects.popper,
-        O = typeof m == "function" ? m(Object.assign({}, e.rects, {
-            placement: e.placement
-        })) : m,
-        I = typeof O == "number" ? {
-            mainAxis: O,
-            altAxis: O
-        } : Object.assign({
-            mainAxis: 0,
-            altAxis: 0
-        }, O),
-        L = e.modifiersData.offset ? e.modifiersData.offset[e.placement] : null,
-        j = {
-            x: 0,
-            y: 0
-        };
-    if (g) {
-        if (o) {
-            var ee, Ne = T === "y" ? _ : Y,
-                Ie = T === "y" ? oe : ne,
-                te = T === "y" ? "height" : "width",
-                ie = g[T],
-                De = ie + b[Ne],
-                xe = ie - b[Ie],
-                Ge = p ? -y[te] / 2 : 0,
-                Et = S === dt ? x[te] : y[te],
-                Ye = S === dt ? -y[te] : -x[te],
-                ut = e.elements.arrow,
-                vn = p && ut ? _t(ut) : {
-                    width: 0,
-                    height: 0
-                },
-                St = e.modifiersData["arrow#persistent"] ? e.modifiersData["arrow#persistent"].padding : nr(),
-                Zn = St[Ne],
-                Dr = St[Ie],
-                qt = Yt(0, x[te], vn[te]),
-                $i = C ? x[te] / 2 - Ge - qt - Zn - I.mainAxis : Et - qt - Zn - I.mainAxis,
-                ld = C ? -x[te] / 2 + Ge + qt + Dr + I.mainAxis : Ye + qt + Dr + I.mainAxis,
-                Wi = e.elements.arrow && qe(e.elements.arrow),
-                ad = Wi ? T === "y" ? Wi.clientTop || 0 : Wi.clientLeft || 0 : 0,
-                il = (ee = L == null ? void 0 : L[T]) != null ? ee : 0,
-                cd = ie + $i - il - ad,
-                ud = ie + ld - il,
-                ol = Yt(p ? Ut(De, cd) : De, ie, p ? We(xe, ud) : xe);
-            g[T] = ol, j[T] = ol - ie
-        }
-        if (l) {
-            var sl, dd = T === "x" ? _ : Y,
-                fd = T === "x" ? oe : ne,
-                Jt = g[E],
-                Lr = E === "y" ? "height" : "width",
-                ll = Jt + b[dd],
-                al = Jt - b[fd],
-                qi = [_, Y].indexOf(k) !== -1,
-                cl = (sl = L == null ? void 0 : L[E]) != null ? sl : 0,
-                ul = qi ? ll : Jt - x[Lr] - y[Lr] - cl + I.altAxis,
-                dl = qi ? Jt + x[Lr] + y[Lr] - cl - I.altAxis : al,
-                fl = p && qi ? bl(ul, Jt, dl) : Yt(p ? ul : ll, Jt, p ? dl : al);
-            g[E] = fl, j[E] = fl - Jt
-        }
-        e.modifiersData[r] = j
-    }
-}
-var Il = {
-    name: "preventOverflow",
-    enabled: !0,
-    phase: "main",
-    fn: Jd,
-    requiresIfExists: ["offset"]
-};
-
-function Xi(n) {
-    return {
-        scrollLeft: n.scrollLeft,
-        scrollTop: n.scrollTop
-    }
-}
-
-function Zi(n) {
-    return n === $(n) || !se(n) ? Qt(n) : Xi(n)
-}
-
-function Kd(n) {
-    var e = n.getBoundingClientRect(),
-        t = ft(e.width) / n.offsetWidth || 1,
-        r = ft(e.height) / n.offsetHeight || 1;
-    return t !== 1 || r !== 1
-}
-
-function eo(n, e, t) {
-    t === void 0 && (t = !1);
-    var r = se(e),
-        i = se(e) && Kd(e),
-        o = de(e),
-        s = Pe(n, i, t),
-        l = {
-            scrollLeft: 0,
-            scrollTop: 0
-        },
-        a = {
-            x: 0,
-            y: 0
-        };
-    return (r || !r && !t) && ((le(e) !== "body" || Zt(o)) && (l = Zi(e)), se(e) ? (a = Pe(e, !0), a.x += e.clientLeft, a.y += e.clientTop) : o && (a.x = Xt(o))), {
-        x: s.left + l.scrollLeft - a.x,
-        y: s.top + l.scrollTop - a.y,
-        width: s.width,
-        height: s.height
-    }
-}
-
-function Ud(n) {
-    var e = new Map,
-        t = new Set,
-        r = [];
-    n.forEach(function(o) {
-        e.set(o.name, o)
-    });
-
-    function i(o) {
-        t.add(o.name);
-        var s = [].concat(o.requires || [], o.requiresIfExists || []);
-        s.forEach(function(l) {
-            if (!t.has(l)) {
-                var a = e.get(l);
-                a && i(a)
-            }
-        }), r.push(o)
-    }
-    return n.forEach(function(o) {
-        t.has(o.name) || i(o)
-    }), r
-}
-
-function to(n) {
-    var e = Ud(n);
-    return gl.reduce(function(t, r) {
-        return t.concat(e.filter(function(i) {
-            return i.phase === r
-        }))
-    }, [])
-}
-
-function no(n) {
-    var e;
-    return function() {
-        return e || (e = new Promise(function(t) {
-            Promise.resolve().then(function() {
-                e = void 0, t(n())
-            })
-        })), e
-    }
-}
-
-function ro(n) {
-    var e = n.reduce(function(t, r) {
-        var i = t[r.name];
-        return t[r.name] = i ? Object.assign({}, i, r, {
-            options: Object.assign({}, i.options, r.options),
-            data: Object.assign({}, i.data, r.data)
-        }) : r, t
-    }, {});
-    return Object.keys(e).map(function(t) {
-        return e[t]
-    })
-}
-var Dl = {
-    placement: "bottom",
-    modifiers: [],
-    strategy: "absolute"
-};
-
-function Ll() {
-    for (var n = arguments.length, e = new Array(n), t = 0; t < n; t++) e[t] = arguments[t];
-    return !e.some(function(r) {
-        return !(r && typeof r.getBoundingClientRect == "function")
-    })
-}
-
-function Pl(n) {
-    n === void 0 && (n = {});
-    var e = n,
-        t = e.defaultModifiers,
-        r = t === void 0 ? [] : t,
-        i = e.defaultOptions,
-        o = i === void 0 ? Dl : i;
-    return function(l, a, c) {
-        c === void 0 && (c = o);
-        var u = {
-                placement: "bottom",
-                orderedModifiers: [],
-                options: Object.assign({}, Dl, o),
-                modifiersData: {},
-                elements: {
-                    reference: l,
-                    popper: a
-                },
-                attributes: {},
-                styles: {}
-            },
-            d = [],
-            f = !1,
-            p = {
-                state: u,
-                setOptions: function(k) {
-                    var S = typeof k == "function" ? k(u.options) : k;
-                    m(), u.options = Object.assign({}, o, u.options, S), u.scrollParents = {
-                        reference: Le(l) ? Ct(l) : l.contextElement ? Ct(l.contextElement) : [],
-                        popper: Ct(a)
-                    };
-                    var C = to(ro([].concat(r, u.options.modifiers)));
-                    if (u.orderedModifiers = C.filter(function(L) {
-                            return L.enabled
-                        }), !1) {
-                        var T;
-                        if (getBasePlacement(u.options.placement) === auto) var E;
-                        var g, x, y, O, I
-                    }
-                    return h(), p.update()
-                },
-                forceUpdate: function() {
-                    if (!f) {
-                        var k = u.elements,
-                            S = k.reference,
-                            C = k.popper;
-                        if (Ll(S, C)) {
-                            u.rects = {
-                                reference: eo(S, qe(C), u.options.strategy === "fixed"),
-                                popper: _t(C)
-                            }, u.reset = !1, u.placement = u.options.placement, u.orderedModifiers.forEach(function(L) {
-                                return u.modifiersData[L.name] = Object.assign({}, L.data)
-                            });
-                            for (var T = 0, E = 0; E < u.orderedModifiers.length; E++) {
-                                if (u.reset === !0) {
-                                    u.reset = !1, E = -1;
-                                    continue
-                                }
-                                var g = u.orderedModifiers[E],
-                                    x = g.fn,
-                                    y = g.options,
-                                    O = y === void 0 ? {} : y,
-                                    I = g.name;
-                                typeof x == "function" && (u = x({
-                                    state: u,
-                                    options: O,
-                                    name: I,
-                                    instance: p
-                                }) || u)
-                            }
-                        }
-                    }
-                },
-                update: no(function() {
-                    return new Promise(function(b) {
-                        p.forceUpdate(), b(u)
-                    })
-                }),
-                destroy: function() {
-                    m(), f = !0
-                }
-            };
-        if (!Ll(l, a)) return p;
-        p.setOptions(c).then(function(b) {
-            !f && c.onFirstUpdate && c.onFirstUpdate(b)
-        });
-
-        function h() {
-            u.orderedModifiers.forEach(function(b) {
-                var k = b.name,
-                    S = b.options,
-                    C = S === void 0 ? {} : S,
-                    T = b.effect;
-                if (typeof T == "function") {
-                    var E = T({
-                            state: u,
-                            name: k,
-                            instance: p,
-                            options: C
-                        }),
-                        g = function() {};
-                    d.push(E || g)
-                }
-            })
-        }
-
-        function m() {
-            d.forEach(function(b) {
-                return b()
-            }), d = []
-        }
-        return p
-    }
-}
-var _d = [El, Nl, Ml, yl, Al, wl, Il, kl, Ol],
-    sr = Pl({
-        defaultModifiers: _d
-    });
-
-function he(n) {
+function te(n) {
     this.content = n
 }
-he.prototype = {
-    constructor: he,
+te.prototype = {
+    constructor: te,
     find: function(n) {
         for (var e = 0; e < this.content.length; e += 2)
             if (this.content[e] === n) return e;
         return -1
     },
     get: function(n) {
         var e = this.find(n);
         return e == -1 ? void 0 : this.content[e + 1]
     },
     update: function(n, e, t) {
         var r = t && t != n ? this.remove(t) : this,
             i = r.find(n),
-            o = r.content.slice();
-        return i == -1 ? o.push(t || n, e) : (o[i + 1] = e, t && (o[i] = t)), new he(o)
+            s = r.content.slice();
+        return i == -1 ? s.push(t || n, e) : (s[i + 1] = e, t && (s[i] = t)), new te(s)
     },
     remove: function(n) {
         var e = this.find(n);
         if (e == -1) return this;
         var t = this.content.slice();
-        return t.splice(e, 2), new he(t)
+        return t.splice(e, 2), new te(t)
     },
     addToStart: function(n, e) {
-        return new he([n, e].concat(this.remove(n).content))
+        return new te([n, e].concat(this.remove(n).content))
     },
     addToEnd: function(n, e) {
         var t = this.remove(n).content.slice();
-        return t.push(n, e), new he(t)
+        return t.push(n, e), new te(t)
     },
     addBefore: function(n, e, t) {
         var r = this.remove(e),
             i = r.content.slice(),
-            o = r.find(n);
-        return i.splice(o == -1 ? i.length : o, 0, e, t), new he(i)
+            s = r.find(n);
+        return i.splice(s == -1 ? i.length : s, 0, e, t), new te(i)
     },
     forEach: function(n) {
         for (var e = 0; e < this.content.length; e += 2) n(this.content[e], this.content[e + 1])
     },
     prepend: function(n) {
-        return n = he.from(n), n.size ? new he(n.content.concat(this.subtract(n).content)) : this
+        return n = te.from(n), n.size ? new te(n.content.concat(this.subtract(n).content)) : this
     },
     append: function(n) {
-        return n = he.from(n), n.size ? new he(this.subtract(n).content.concat(n.content)) : this
+        return n = te.from(n), n.size ? new te(this.subtract(n).content.concat(n.content)) : this
     },
     subtract: function(n) {
         var e = this;
-        n = he.from(n);
+        n = te.from(n);
         for (var t = 0; t < n.content.length; t += 2) e = e.remove(n.content[t]);
         return e
     },
     toObject: function() {
         var n = {};
         return this.forEach(function(e, t) {
             n[e] = t
         }), n
     },
     get size() {
         return this.content.length >> 1
     }
 };
-he.from = function(n) {
-    if (n instanceof he) return n;
+te.from = function(n) {
+    if (n instanceof te) return n;
     var e = [];
     if (n)
         for (var t in n) e.push(t, n[t]);
-    return new he(e)
+    return new te(e)
 };
-var io = he;
+var Jr = te;
 
-function Vl(n, e, t) {
+function Qs(n, e, t) {
     for (let r = 0;; r++) {
         if (r == n.childCount || r == e.childCount) return n.childCount == e.childCount ? null : t;
         let i = n.child(r),
-            o = e.child(r);
-        if (i == o) {
+            s = e.child(r);
+        if (i == s) {
             t += i.nodeSize;
             continue
         }
-        if (!i.sameMarkup(o)) return t;
-        if (i.isText && i.text != o.text) {
-            for (let s = 0; i.text[s] == o.text[s]; s++) t++;
+        if (!i.sameMarkup(s)) return t;
+        if (i.isText && i.text != s.text) {
+            for (let o = 0; i.text[o] == s.text[o]; o++) t++;
             return t
         }
-        if (i.content.size || o.content.size) {
-            let s = Vl(i.content, o.content, t + 1);
-            if (s != null) return s
+        if (i.content.size || s.content.size) {
+            let o = Qs(i.content, s.content, t + 1);
+            if (o != null) return o
         }
         t += i.nodeSize
     }
 }
 
-function $l(n, e, t, r) {
-    for (let i = n.childCount, o = e.childCount;;) {
-        if (i == 0 || o == 0) return i == o ? null : {
+function Ys(n, e, t, r) {
+    for (let i = n.childCount, s = e.childCount;;) {
+        if (i == 0 || s == 0) return i == s ? null : {
             a: t,
             b: r
         };
-        let s = n.child(--i),
-            l = e.child(--o),
-            a = s.nodeSize;
-        if (s == l) {
+        let o = n.child(--i),
+            l = e.child(--s),
+            a = o.nodeSize;
+        if (o == l) {
             t -= a, r -= a;
             continue
         }
-        if (!s.sameMarkup(l)) return {
+        if (!o.sameMarkup(l)) return {
             a: t,
             b: r
         };
-        if (s.isText && s.text != l.text) {
+        if (o.isText && o.text != l.text) {
             let c = 0,
-                u = Math.min(s.text.length, l.text.length);
-            for (; c < u && s.text[s.text.length - c - 1] == l.text[l.text.length - c - 1];) c++, t--, r--;
+                u = Math.min(o.text.length, l.text.length);
+            for (; c < u && o.text[o.text.length - c - 1] == l.text[l.text.length - c - 1];) c++, t--, r--;
             return {
                 a: t,
                 b: r
             }
         }
-        if (s.content.size || l.content.size) {
-            let c = $l(s.content, l.content, t - 1, r - 1);
+        if (o.content.size || l.content.size) {
+            let c = Ys(o.content, l.content, t - 1, r - 1);
             if (c) return c
         }
         t -= a, r -= a
     }
 }
-var v = class {
+var x = class {
     constructor(e, t) {
         if (this.content = e, this.size = t || 0, t == null)
             for (let r = 0; r < e.length; r++) this.size += e[r].nodeSize
     }
-    nodesBetween(e, t, r, i = 0, o) {
-        for (let s = 0, l = 0; l < t; s++) {
-            let a = this.content[s],
+    nodesBetween(e, t, r, i = 0, s) {
+        for (let o = 0, l = 0; l < t; o++) {
+            let a = this.content[o],
                 c = l + a.nodeSize;
-            if (c > e && r(a, i + l, o || null, s) !== !1 && a.content.size) {
+            if (c > e && r(a, i + l, s || null, o) !== !1 && a.content.size) {
                 let u = l + 1;
                 a.nodesBetween(Math.max(0, e - u), Math.min(a.content.size, t - u), r, i + u)
             }
             l = c
         }
     }
     descendants(e) {
         this.nodesBetween(0, this.size, e)
     }
     textBetween(e, t, r, i) {
-        let o = "",
-            s = !0;
+        let s = "",
+            o = !0;
         return this.nodesBetween(e, t, (l, a) => {
-            l.isText ? (o += l.text.slice(Math.max(e, a) - a, t - a), s = !r) : l.isLeaf ? (i ? o += typeof i == "function" ? i(l) : i : l.type.spec.leafText && (o += l.type.spec.leafText(l)), s = !r) : !s && l.isBlock && (o += r, s = !0)
-        }, 0), o
+            l.isText ? (s += l.text.slice(Math.max(e, a) - a, t - a), o = !r) : l.isLeaf ? (i ? s += typeof i == "function" ? i(l) : i : l.type.spec.leafText && (s += l.type.spec.leafText(l)), o = !r) : !o && l.isBlock && (s += r, o = !0)
+        }, 0), s
     }
     append(e) {
         if (!e.size) return this;
         if (!this.size) return e;
         let t = this.lastChild,
             r = e.firstChild,
             i = this.content.slice(),
-            o = 0;
-        for (t.isText && t.sameMarkup(r) && (i[i.length - 1] = t.withText(t.text + r.text), o = 1); o < e.content.length; o++) i.push(e.content[o]);
-        return new v(i, this.size + e.size)
+            s = 0;
+        for (t.isText && t.sameMarkup(r) && (i[i.length - 1] = t.withText(t.text + r.text), s = 1); s < e.content.length; s++) i.push(e.content[s]);
+        return new x(i, this.size + e.size)
     }
     cut(e, t = this.size) {
         if (e == 0 && t == this.size) return this;
         let r = [],
             i = 0;
         if (t > e)
-            for (let o = 0, s = 0; s < t; o++) {
-                let l = this.content[o],
-                    a = s + l.nodeSize;
-                a > e && ((s < e || a > t) && (l.isText ? l = l.cut(Math.max(0, e - s), Math.min(l.text.length, t - s)) : l = l.cut(Math.max(0, e - s - 1), Math.min(l.content.size, t - s - 1))), r.push(l), i += l.nodeSize), s = a
+            for (let s = 0, o = 0; o < t; s++) {
+                let l = this.content[s],
+                    a = o + l.nodeSize;
+                a > e && ((o < e || a > t) && (l.isText ? l = l.cut(Math.max(0, e - o), Math.min(l.text.length, t - o)) : l = l.cut(Math.max(0, e - o - 1), Math.min(l.content.size, t - o - 1))), r.push(l), i += l.nodeSize), o = a
             }
-        return new v(r, i)
+        return new x(r, i)
     }
     cutByIndex(e, t) {
-        return e == t ? v.empty : e == 0 && t == this.content.length ? this : new v(this.content.slice(e, t))
+        return e == t ? x.empty : e == 0 && t == this.content.length ? this : new x(this.content.slice(e, t))
     }
     replaceChild(e, t) {
         let r = this.content[e];
         if (r == t) return this;
         let i = this.content.slice(),
-            o = this.size + t.nodeSize - r.nodeSize;
-        return i[e] = t, new v(i, o)
+            s = this.size + t.nodeSize - r.nodeSize;
+        return i[e] = t, new x(i, s)
     }
     addToStart(e) {
-        return new v([e].concat(this.content), this.size + e.nodeSize)
+        return new x([e].concat(this.content), this.size + e.nodeSize)
     }
     addToEnd(e) {
-        return new v(this.content.concat(e), this.size + e.nodeSize)
+        return new x(this.content.concat(e), this.size + e.nodeSize)
     }
     eq(e) {
         if (this.content.length != e.content.length) return !1;
         for (let t = 0; t < this.content.length; t++)
             if (!this.content[t].eq(e.content[t])) return !1;
         return !0
     }
@@ -1460,101 +230,101 @@
     forEach(e) {
         for (let t = 0, r = 0; t < this.content.length; t++) {
             let i = this.content[t];
             e(i, r, t), r += i.nodeSize
         }
     }
     findDiffStart(e, t = 0) {
-        return Vl(this, e, t)
+        return Qs(this, e, t)
     }
     findDiffEnd(e, t = this.size, r = e.size) {
-        return $l(this, e, t, r)
+        return Ys(this, e, t, r)
     }
     findIndex(e, t = -1) {
-        if (e == 0) return jr(0, e);
-        if (e == this.size) return jr(this.content.length, e);
+        if (e == 0) return $n(0, e);
+        if (e == this.size) return $n(this.content.length, e);
         if (e > this.size || e < 0) throw new RangeError(`Position ${e} outside of fragment (${this})`);
         for (let r = 0, i = 0;; r++) {
-            let o = this.child(r),
-                s = i + o.nodeSize;
-            if (s >= e) return s == e || t > 0 ? jr(r + 1, s) : jr(r, i);
-            i = s
+            let s = this.child(r),
+                o = i + s.nodeSize;
+            if (o >= e) return o == e || t > 0 ? $n(r + 1, o) : $n(r, i);
+            i = o
         }
     }
     toString() {
         return "<" + this.toStringInner() + ">"
     }
     toStringInner() {
         return this.content.join(", ")
     }
     toJSON() {
         return this.content.length ? this.content.map(e => e.toJSON()) : null
     }
     static fromJSON(e, t) {
-        if (!t) return v.empty;
+        if (!t) return x.empty;
         if (!Array.isArray(t)) throw new RangeError("Invalid input for Fragment.fromJSON");
-        return new v(t.map(e.nodeFromJSON))
+        return new x(t.map(e.nodeFromJSON))
     }
     static fromArray(e) {
-        if (!e.length) return v.empty;
+        if (!e.length) return x.empty;
         let t, r = 0;
         for (let i = 0; i < e.length; i++) {
-            let o = e[i];
-            r += o.nodeSize, i && o.isText && e[i - 1].sameMarkup(o) ? (t || (t = e.slice(0, i)), t[t.length - 1] = o.withText(t[t.length - 1].text + o.text)) : t && t.push(o)
+            let s = e[i];
+            r += s.nodeSize, i && s.isText && e[i - 1].sameMarkup(s) ? (t || (t = e.slice(0, i)), t[t.length - 1] = s.withText(t[t.length - 1].text + s.text)) : t && t.push(s)
         }
-        return new v(t || e, r)
+        return new x(t || e, r)
     }
     static from(e) {
-        if (!e) return v.empty;
-        if (e instanceof v) return e;
+        if (!e) return x.empty;
+        if (e instanceof x) return e;
         if (Array.isArray(e)) return this.fromArray(e);
-        if (e.attrs) return new v([e], e.nodeSize);
+        if (e.attrs) return new x([e], e.nodeSize);
         throw new RangeError("Can not convert " + e + " to a Fragment" + (e.nodesBetween ? " (looks like multiple versions of prosemirror-model were loaded)" : ""))
     }
 };
-v.empty = new v([], 0);
-var oo = {
+x.empty = new x([], 0);
+var Wr = {
     index: 0,
     offset: 0
 };
 
-function jr(n, e) {
-    return oo.index = n, oo.offset = e, oo
+function $n(n, e) {
+    return Wr.index = n, Wr.offset = e, Wr
 }
 
-function Vr(n, e) {
+function Vn(n, e) {
     if (n === e) return !0;
     if (!(n && typeof n == "object") || !(e && typeof e == "object")) return !1;
     let t = Array.isArray(n);
     if (Array.isArray(e) != t) return !1;
     if (t) {
         if (n.length != e.length) return !1;
         for (let r = 0; r < n.length; r++)
-            if (!Vr(n[r], e[r])) return !1
+            if (!Vn(n[r], e[r])) return !1
     } else {
         for (let r in n)
-            if (!(r in e) || !Vr(n[r], e[r])) return !1;
+            if (!(r in e) || !Vn(n[r], e[r])) return !1;
         for (let r in e)
             if (!(r in n)) return !1
     }
     return !0
 }
-var H = class {
+var B = class {
     constructor(e, t) {
         this.type = e, this.attrs = t
     }
     addToSet(e) {
         let t, r = !1;
         for (let i = 0; i < e.length; i++) {
-            let o = e[i];
-            if (this.eq(o)) return e;
-            if (this.type.excludes(o.type)) t || (t = e.slice(0, i));
+            let s = e[i];
+            if (this.eq(s)) return e;
+            if (this.type.excludes(s.type)) t || (t = e.slice(0, i));
             else {
-                if (o.type.excludes(this.type)) return e;
-                !r && o.type.rank > this.type.rank && (t || (t = e.slice(0, i)), t.push(this), r = !0), t && t.push(o)
+                if (s.type.excludes(this.type)) return e;
+                !r && s.type.rank > this.type.rank && (t || (t = e.slice(0, i)), t.push(this), r = !0), t && t.push(s)
             }
         }
         return t || (t = e.slice()), r || t.push(this), t
     }
     removeFromSet(e) {
         for (let t = 0; t < e.length; t++)
             if (this.eq(e[t])) return e.slice(0, t).concat(e.slice(t + 1));
@@ -1562,15 +332,15 @@
     }
     isInSet(e) {
         for (let t = 0; t < e.length; t++)
             if (this.eq(e[t])) return !0;
         return !1
     }
     eq(e) {
-        return this == e || this.type == e.type && Vr(this.attrs, e.attrs)
+        return this == e || this.type == e.type && Vn(this.attrs, e.attrs)
     }
     toJSON() {
         let e = {
             type: this.type.name
         };
         for (let t in this.attrs) {
             e.attrs = this.attrs;
@@ -1588,35 +358,35 @@
         if (e == t) return !0;
         if (e.length != t.length) return !1;
         for (let r = 0; r < e.length; r++)
             if (!e[r].eq(t[r])) return !1;
         return !0
     }
     static setFrom(e) {
-        if (!e || Array.isArray(e) && e.length == 0) return H.none;
-        if (e instanceof H) return [e];
+        if (!e || Array.isArray(e) && e.length == 0) return B.none;
+        if (e instanceof B) return [e];
         let t = e.slice();
         return t.sort((r, i) => r.type.rank - i.type.rank), t
     }
 };
-H.none = [];
-var nn = class extends Error {},
-    w = class {
+B.none = [];
+var mt = class extends Error {},
+    E = class {
         constructor(e, t, r) {
             this.content = e, this.openStart = t, this.openEnd = r
         }
         get size() {
             return this.content.size - this.openStart - this.openEnd
         }
         insertAt(e, t) {
-            let r = ql(this.content, e + this.openStart, t);
-            return r && new w(r, this.openStart, this.openEnd)
+            let r = Zs(this.content, e + this.openStart, t);
+            return r && new E(r, this.openStart, this.openEnd)
         }
         removeBetween(e, t) {
-            return new w(Wl(this.content, e + this.openStart, t + this.openStart), this.openStart, this.openEnd)
+            return new E(Xs(this.content, e + this.openStart, t + this.openStart), this.openStart, this.openEnd)
         }
         eq(e) {
             return this.content.eq(e.content) && this.openStart == e.openStart && this.openEnd == e.openEnd
         }
         toString() {
             return this.content + "(" + this.openStart + "," + this.openEnd + ")"
         }
@@ -1624,136 +394,136 @@
             if (!this.content.size) return null;
             let e = {
                 content: this.content.toJSON()
             };
             return this.openStart > 0 && (e.openStart = this.openStart), this.openEnd > 0 && (e.openEnd = this.openEnd), e
         }
         static fromJSON(e, t) {
-            if (!t) return w.empty;
+            if (!t) return E.empty;
             let r = t.openStart || 0,
                 i = t.openEnd || 0;
             if (typeof r != "number" || typeof i != "number") throw new RangeError("Invalid input for Slice.fromJSON");
-            return new w(v.fromJSON(e, t.content), r, i)
+            return new E(x.fromJSON(e, t.content), r, i)
         }
         static maxOpen(e, t = !0) {
             let r = 0,
                 i = 0;
-            for (let o = e.firstChild; o && !o.isLeaf && (t || !o.type.spec.isolating); o = o.firstChild) r++;
-            for (let o = e.lastChild; o && !o.isLeaf && (t || !o.type.spec.isolating); o = o.lastChild) i++;
-            return new w(e, r, i)
+            for (let s = e.firstChild; s && !s.isLeaf && (t || !s.type.spec.isolating); s = s.firstChild) r++;
+            for (let s = e.lastChild; s && !s.isLeaf && (t || !s.type.spec.isolating); s = s.lastChild) i++;
+            return new E(e, r, i)
         }
     };
-w.empty = new w(v.empty, 0, 0);
+E.empty = new E(x.empty, 0, 0);
 
-function Wl(n, e, t) {
+function Xs(n, e, t) {
     let {
         index: r,
         offset: i
-    } = n.findIndex(e), o = n.maybeChild(r), {
-        index: s,
+    } = n.findIndex(e), s = n.maybeChild(r), {
+        index: o,
         offset: l
     } = n.findIndex(t);
-    if (i == e || o.isText) {
-        if (l != t && !n.child(s).isText) throw new RangeError("Removing non-flat range");
+    if (i == e || s.isText) {
+        if (l != t && !n.child(o).isText) throw new RangeError("Removing non-flat range");
         return n.cut(0, e).append(n.cut(t))
     }
-    if (r != s) throw new RangeError("Removing non-flat range");
-    return n.replaceChild(r, o.copy(Wl(o.content, e - i - 1, t - i - 1)))
+    if (r != o) throw new RangeError("Removing non-flat range");
+    return n.replaceChild(r, s.copy(Xs(s.content, e - i - 1, t - i - 1)))
 }
 
-function ql(n, e, t, r) {
+function Zs(n, e, t, r) {
     let {
         index: i,
-        offset: o
-    } = n.findIndex(e), s = n.maybeChild(i);
-    if (o == e || s.isText) return r && !r.canReplace(i, i, t) ? null : n.cut(0, e).append(t).append(n.cut(e));
-    let l = ql(s.content, e - o - 1, t);
-    return l && n.replaceChild(i, s.copy(l))
+        offset: s
+    } = n.findIndex(e), o = n.maybeChild(i);
+    if (s == e || o.isText) return r && !r.canReplace(i, i, t) ? null : n.cut(0, e).append(t).append(n.cut(e));
+    let l = Zs(o.content, e - s - 1, t);
+    return l && n.replaceChild(i, o.copy(l))
 }
 
-function Gd(n, e, t) {
-    if (t.openStart > n.depth) throw new nn("Inserted content deeper than insertion position");
-    if (n.depth - t.openStart != e.depth - t.openEnd) throw new nn("Inconsistent open depths");
-    return Jl(n, e, t, 0)
+function kc(n, e, t) {
+    if (t.openStart > n.depth) throw new mt("Inserted content deeper than insertion position");
+    if (n.depth - t.openStart != e.depth - t.openEnd) throw new mt("Inconsistent open depths");
+    return eo(n, e, t, 0)
 }
 
-function Jl(n, e, t, r) {
+function eo(n, e, t, r) {
     let i = n.index(r),
-        o = n.node(r);
+        s = n.node(r);
     if (i == e.index(r) && r < n.depth - t.openStart) {
-        let s = Jl(n, e, t, r + 1);
-        return o.copy(o.content.replaceChild(i, s))
+        let o = eo(n, e, t, r + 1);
+        return s.copy(s.content.replaceChild(i, o))
     } else if (t.content.size)
         if (!t.openStart && !t.openEnd && n.depth == r && e.depth == r) {
-            let s = n.parent,
-                l = s.content;
-            return tn(s, l.cut(0, n.parentOffset).append(t.content).append(l.cut(e.parentOffset)))
+            let o = n.parent,
+                l = o.content;
+            return pt(o, l.cut(0, n.parentOffset).append(t.content).append(l.cut(e.parentOffset)))
         } else {
             let {
-                start: s,
+                start: o,
                 end: l
-            } = Yd(t, n);
-            return tn(o, Ul(n, s, l, e, r))
+            } = Mc(t, n);
+            return pt(s, no(n, o, l, e, r))
         }
-    else return tn(o, $r(n, e, r))
+    else return pt(s, Jn(n, e, r))
 }
 
-function Kl(n, e) {
-    if (!e.type.compatibleContent(n.type)) throw new nn("Cannot join " + e.type.name + " onto " + n.type.name)
+function to(n, e) {
+    if (!e.type.compatibleContent(n.type)) throw new mt("Cannot join " + e.type.name + " onto " + n.type.name)
 }
 
-function co(n, e, t) {
+function _r(n, e, t) {
     let r = n.node(t);
-    return Kl(r, e.node(t)), r
+    return to(r, e.node(t)), r
 }
 
-function en(n, e) {
+function ht(n, e) {
     let t = e.length - 1;
     t >= 0 && n.isText && n.sameMarkup(e[t]) ? e[t] = n.withText(e[t].text + n.text) : e.push(n)
 }
 
-function lr(n, e, t, r) {
+function cn(n, e, t, r) {
     let i = (e || n).node(t),
-        o = 0,
-        s = e ? e.index(t) : i.childCount;
-    n && (o = n.index(t), n.depth > t ? o++ : n.textOffset && (en(n.nodeAfter, r), o++));
-    for (let l = o; l < s; l++) en(i.child(l), r);
-    e && e.depth == t && e.textOffset && en(e.nodeBefore, r)
+        s = 0,
+        o = e ? e.index(t) : i.childCount;
+    n && (s = n.index(t), n.depth > t ? s++ : n.textOffset && (ht(n.nodeAfter, r), s++));
+    for (let l = s; l < o; l++) ht(i.child(l), r);
+    e && e.depth == t && e.textOffset && ht(e.nodeBefore, r)
 }
 
-function tn(n, e) {
+function pt(n, e) {
     return n.type.checkContent(e), n.copy(e)
 }
 
-function Ul(n, e, t, r, i) {
-    let o = n.depth > i && co(n, e, i + 1),
-        s = r.depth > i && co(t, r, i + 1),
+function no(n, e, t, r, i) {
+    let s = n.depth > i && _r(n, e, i + 1),
+        o = r.depth > i && _r(t, r, i + 1),
         l = [];
-    return lr(null, n, i, l), o && s && e.index(i) == t.index(i) ? (Kl(o, s), en(tn(o, Ul(n, e, t, r, i + 1)), l)) : (o && en(tn(o, $r(n, e, i + 1)), l), lr(e, t, i, l), s && en(tn(s, $r(t, r, i + 1)), l)), lr(r, null, i, l), new v(l)
+    return cn(null, n, i, l), s && o && e.index(i) == t.index(i) ? (to(s, o), ht(pt(s, no(n, e, t, r, i + 1)), l)) : (s && ht(pt(s, Jn(n, e, i + 1)), l), cn(e, t, i, l), o && ht(pt(o, Jn(t, r, i + 1)), l)), cn(r, null, i, l), new x(l)
 }
 
-function $r(n, e, t) {
+function Jn(n, e, t) {
     let r = [];
-    if (lr(null, n, t, r), n.depth > t) {
-        let i = co(n, e, t + 1);
-        en(tn(i, $r(n, e, t + 1)), r)
+    if (cn(null, n, t, r), n.depth > t) {
+        let i = _r(n, e, t + 1);
+        ht(pt(i, Jn(n, e, t + 1)), r)
     }
-    return lr(e, null, t, r), new v(r)
+    return cn(e, null, t, r), new x(r)
 }
 
-function Yd(n, e) {
+function Mc(n, e) {
     let t = e.depth - n.openStart,
         i = e.node(t).copy(n.content);
-    for (let o = t - 1; o >= 0; o--) i = e.node(o).copy(v.from(i));
+    for (let s = t - 1; s >= 0; s--) i = e.node(s).copy(x.from(i));
     return {
         start: i.resolveNoCache(n.openStart + t),
         end: i.resolveNoCache(i.content.size - n.openEnd - t)
     }
 }
-var rn = class {
+var gt = class {
         constructor(e, t, r) {
             this.pos = e, this.path = t, this.parentOffset = r, this.depth = t.length / 3 - 1
         }
         resolveDepth(e) {
             return e == null ? this.depth : e < 0 ? this.depth + e : e
         }
         get parent() {
@@ -1801,49 +571,49 @@
                 t = this.pos - this.path[this.path.length - 1];
             return t ? this.parent.child(e).cut(0, t) : e == 0 ? null : this.parent.child(e - 1)
         }
         posAtIndex(e, t) {
             t = this.resolveDepth(t);
             let r = this.path[t * 3],
                 i = t == 0 ? 0 : this.path[t * 3 - 1] + 1;
-            for (let o = 0; o < e; o++) i += r.child(o).nodeSize;
+            for (let s = 0; s < e; s++) i += r.child(s).nodeSize;
             return i
         }
         marks() {
             let e = this.parent,
                 t = this.index();
-            if (e.content.size == 0) return H.none;
+            if (e.content.size == 0) return B.none;
             if (this.textOffset) return e.child(t).marks;
             let r = e.maybeChild(t - 1),
                 i = e.maybeChild(t);
             if (!r) {
                 let l = r;
                 r = i, i = l
             }
-            let o = r.marks;
-            for (var s = 0; s < o.length; s++) o[s].type.spec.inclusive === !1 && (!i || !o[s].isInSet(i.marks)) && (o = o[s--].removeFromSet(o));
-            return o
+            let s = r.marks;
+            for (var o = 0; o < s.length; o++) s[o].type.spec.inclusive === !1 && (!i || !s[o].isInSet(i.marks)) && (s = s[o--].removeFromSet(s));
+            return s
         }
         marksAcross(e) {
             let t = this.parent.maybeChild(this.index());
             if (!t || !t.isInline) return null;
             let r = t.marks,
                 i = e.parent.maybeChild(e.index());
-            for (var o = 0; o < r.length; o++) r[o].type.spec.inclusive === !1 && (!i || !r[o].isInSet(i.marks)) && (r = r[o--].removeFromSet(r));
+            for (var s = 0; s < r.length; s++) r[s].type.spec.inclusive === !1 && (!i || !r[s].isInSet(i.marks)) && (r = r[s--].removeFromSet(r));
             return r
         }
         sharedDepth(e) {
             for (let t = this.depth; t > 0; t--)
                 if (this.start(t) <= e && this.end(t) >= e) return t;
             return 0
         }
         blockRange(e = this, t) {
             if (e.pos < this.pos) return e.blockRange(this);
             for (let r = this.depth - (this.parent.inlineContent || this.pos == e.pos ? 1 : 0); r >= 0; r--)
-                if (e.pos <= this.end(r) && (!t || t(this.node(r)))) return new on(this, e, r);
+                if (e.pos <= this.end(r) && (!t || t(this.node(r)))) return new yt(this, e, r);
             return null
         }
         sameParent(e) {
             return this.pos - this.parentOffset == e.pos - e.parentOffset
         }
         max(e) {
             return e.pos > this.pos ? e : this
@@ -1856,38 +626,38 @@
             for (let t = 1; t <= this.depth; t++) e += (e ? "/" : "") + this.node(t).type.name + "_" + this.index(t - 1);
             return e + ":" + this.parentOffset
         }
         static resolve(e, t) {
             if (!(t >= 0 && t <= e.content.size)) throw new RangeError("Position " + t + " out of range");
             let r = [],
                 i = 0,
-                o = t;
-            for (let s = e;;) {
+                s = t;
+            for (let o = e;;) {
                 let {
                     index: l,
                     offset: a
-                } = s.content.findIndex(o), c = o - a;
-                if (r.push(s, l, i + a), !c || (s = s.child(l), s.isText)) break;
-                o = c - 1, i += a + 1
+                } = o.content.findIndex(s), c = s - a;
+                if (r.push(o, l, i + a), !c || (o = o.child(l), o.isText)) break;
+                s = c - 1, i += a + 1
             }
-            return new rn(t, r, o)
+            return new gt(t, r, s)
         }
         static resolveCached(e, t) {
-            for (let i = 0; i < so.length; i++) {
-                let o = so[i];
-                if (o.pos == t && o.doc == e) return o
-            }
-            let r = so[lo] = rn.resolve(e, t);
-            return lo = (lo + 1) % Qd, r
+            for (let i = 0; i < qr.length; i++) {
+                let s = qr[i];
+                if (s.pos == t && s.doc == e) return s
+            }
+            let r = qr[Kr] = gt.resolve(e, t);
+            return Kr = (Kr + 1) % Sc, r
         }
     },
-    so = [],
-    lo = 0,
-    Qd = 12,
-    on = class {
+    qr = [],
+    Kr = 0,
+    Sc = 12,
+    yt = class {
         constructor(e, t, r) {
             this.$from = e, this.$to = t, this.depth = r
         }
         get start() {
             return this.$from.before(this.depth + 1)
         }
         get end() {
@@ -1899,18 +669,18 @@
         get startIndex() {
             return this.$from.index(this.depth)
         }
         get endIndex() {
             return this.$to.indexAfter(this.depth)
         }
     },
-    Xd = Object.create(null),
-    we = class {
-        constructor(e, t, r, i = H.none) {
-            this.type = e, this.attrs = t, this.marks = i, this.content = r || v.empty
+    Ec = Object.create(null),
+    ue = class {
+        constructor(e, t, r, i = B.none) {
+            this.type = e, this.attrs = t, this.marks = i, this.content = r || x.empty
         }
         get nodeSize() {
             return this.isLeaf ? 1 : 2 + this.content.size
         }
         get childCount() {
             return this.content.childCount
         }
@@ -1944,36 +714,36 @@
         eq(e) {
             return this == e || this.sameMarkup(e) && this.content.eq(e.content)
         }
         sameMarkup(e) {
             return this.hasMarkup(e.type, e.attrs, e.marks)
         }
         hasMarkup(e, t, r) {
-            return this.type == e && Vr(this.attrs, t || e.defaultAttrs || Xd) && H.sameSet(this.marks, r || H.none)
+            return this.type == e && Vn(this.attrs, t || e.defaultAttrs || Ec) && B.sameSet(this.marks, r || B.none)
         }
         copy(e = null) {
-            return e == this.content ? this : new we(this.type, this.attrs, e, this.marks)
+            return e == this.content ? this : new ue(this.type, this.attrs, e, this.marks)
         }
         mark(e) {
-            return e == this.marks ? this : new we(this.type, this.attrs, this.content, e)
+            return e == this.marks ? this : new ue(this.type, this.attrs, this.content, e)
         }
         cut(e, t = this.content.size) {
             return e == 0 && t == this.content.size ? this : this.copy(this.content.cut(e, t))
         }
         slice(e, t = this.content.size, r = !1) {
-            if (e == t) return w.empty;
+            if (e == t) return E.empty;
             let i = this.resolve(e),
-                o = this.resolve(t),
-                s = r ? 0 : i.sharedDepth(t),
-                l = i.start(s),
-                c = i.node(s).content.cut(i.pos - l, o.pos - l);
-            return new w(c, i.depth - s, o.depth - s)
+                s = this.resolve(t),
+                o = r ? 0 : i.sharedDepth(t),
+                l = i.start(o),
+                c = i.node(o).content.cut(i.pos - l, s.pos - l);
+            return new E(c, i.depth - o, s.depth - o)
         }
         replace(e, t, r) {
-            return Gd(this.resolve(e), this.resolve(t), r)
+            return kc(this.resolve(e), this.resolve(t), r)
         }
         nodeAt(e) {
             for (let t = this;;) {
                 let {
                     index: r,
                     offset: i
                 } = t.content.findIndex(e);
@@ -2012,22 +782,22 @@
             return {
                 node: i,
                 index: t - 1,
                 offset: r - i.nodeSize
             }
         }
         resolve(e) {
-            return rn.resolveCached(this, e)
+            return gt.resolveCached(this, e)
         }
         resolveNoCache(e) {
-            return rn.resolve(this, e)
+            return gt.resolve(this, e)
         }
         rangeHasMark(e, t, r) {
             let i = !1;
-            return t > e && this.nodesBetween(e, t, o => (r.isInSet(o.marks) && (i = !0), !i)), i
+            return t > e && this.nodesBetween(e, t, s => (r.isInSet(s.marks) && (i = !0), !i)), i
         }
         get isBlock() {
             return this.type.isBlock
         }
         get isTextblock() {
             return this.type.isTextblock
         }
@@ -2045,43 +815,43 @@
         }
         get isAtom() {
             return this.type.isAtom
         }
         toString() {
             if (this.type.spec.toDebugString) return this.type.spec.toDebugString(this);
             let e = this.type.name;
-            return this.content.size && (e += "(" + this.content.toStringInner() + ")"), _l(this.marks, e)
+            return this.content.size && (e += "(" + this.content.toStringInner() + ")"), ro(this.marks, e)
         }
         contentMatchAt(e) {
             let t = this.type.contentMatch.matchFragment(this.content, 0, e);
             if (!t) throw new Error("Called contentMatchAt on a node with invalid content");
             return t
         }
-        canReplace(e, t, r = v.empty, i = 0, o = r.childCount) {
-            let s = this.contentMatchAt(e).matchFragment(r, i, o),
-                l = s && s.matchFragment(this.content, t);
+        canReplace(e, t, r = x.empty, i = 0, s = r.childCount) {
+            let o = this.contentMatchAt(e).matchFragment(r, i, s),
+                l = o && o.matchFragment(this.content, t);
             if (!l || !l.validEnd) return !1;
-            for (let a = i; a < o; a++)
+            for (let a = i; a < s; a++)
                 if (!this.type.allowsMarks(r.child(a).marks)) return !1;
             return !0
         }
         canReplaceWith(e, t, r, i) {
             if (i && !this.type.allowsMarks(i)) return !1;
-            let o = this.contentMatchAt(e).matchType(r),
-                s = o && o.matchFragment(this.content, t);
-            return s ? s.validEnd : !1
+            let s = this.contentMatchAt(e).matchType(r),
+                o = s && s.matchFragment(this.content, t);
+            return o ? o.validEnd : !1
         }
         canAppend(e) {
             return e.content.size ? this.canReplace(this.childCount, this.childCount, e.content) : this.type.compatibleContent(e.type)
         }
         check() {
             this.type.checkContent(this.content);
-            let e = H.none;
+            let e = B.none;
             for (let t = 0; t < this.marks.length; t++) e = this.marks[t].addToSet(e);
-            if (!H.sameSet(e, this.marks)) throw new RangeError(`Invalid collection of marks for node ${this.type.name}: ${this.marks.map(t=>t.type.name)}`);
+            if (!B.sameSet(e, this.marks)) throw new RangeError(`Invalid collection of marks for node ${this.type.name}: ${this.marks.map(t=>t.type.name)}`);
             this.content.forEach(t => t.check())
         }
         toJSON() {
             let e = {
                 type: this.type.name
             };
             for (let t in this.attrs) {
@@ -2097,78 +867,78 @@
                 if (!Array.isArray(t.marks)) throw new RangeError("Invalid mark data for Node.fromJSON");
                 r = t.marks.map(e.markFromJSON)
             }
             if (t.type == "text") {
                 if (typeof t.text != "string") throw new RangeError("Invalid text node in JSON");
                 return e.text(t.text, r)
             }
-            let i = v.fromJSON(e, t.content);
+            let i = x.fromJSON(e, t.content);
             return e.nodeType(t.type).create(t.attrs, i, r)
         }
     };
-we.prototype.text = void 0;
-var On = class extends we {
+ue.prototype.text = void 0;
+var Pt = class extends ue {
     constructor(e, t, r, i) {
         if (super(e, t, null, i), !r) throw new RangeError("Empty text nodes are not allowed");
         this.text = r
     }
     toString() {
-        return this.type.spec.toDebugString ? this.type.spec.toDebugString(this) : _l(this.marks, JSON.stringify(this.text))
+        return this.type.spec.toDebugString ? this.type.spec.toDebugString(this) : ro(this.marks, JSON.stringify(this.text))
     }
     get textContent() {
         return this.text
     }
     textBetween(e, t) {
         return this.text.slice(e, t)
     }
     get nodeSize() {
         return this.text.length
     }
     mark(e) {
-        return e == this.marks ? this : new On(this.type, this.attrs, this.text, e)
+        return e == this.marks ? this : new Pt(this.type, this.attrs, this.text, e)
     }
     withText(e) {
-        return e == this.text ? this : new On(this.type, this.attrs, e, this.marks)
+        return e == this.text ? this : new Pt(this.type, this.attrs, e, this.marks)
     }
     cut(e = 0, t = this.text.length) {
         return e == 0 && t == this.text.length ? this : this.withText(this.text.slice(e, t))
     }
     eq(e) {
         return this.sameMarkup(e) && this.text == e.text
     }
     toJSON() {
         let e = super.toJSON();
         return e.text = this.text, e
     }
 };
 
-function _l(n, e) {
+function ro(n, e) {
     for (let t = n.length - 1; t >= 0; t--) e = n[t].type.name + "(" + e + ")";
     return e
 }
-var ht = class {
+var He = class {
     constructor(e) {
         this.validEnd = e, this.next = [], this.wrapCache = []
     }
     static parse(e, t) {
-        let r = new uo(e, t);
-        if (r.next == null) return ht.empty;
-        let i = Gl(r);
+        let r = new Gr(e, t);
+        if (r.next == null) return He.empty;
+        let i = io(r);
         r.next && r.err("Unexpected trailing text");
-        let o = sf(of(i));
-        return lf(o, r), o
+        let s = Nc(vc(i));
+        return Ic(s, r), s
     }
     matchType(e) {
         for (let t = 0; t < this.next.length; t++)
             if (this.next[t].type == e) return this.next[t].next;
         return null
     }
     matchFragment(e, t = 0, r = e.childCount) {
         let i = this;
-        for (let o = t; i && o < r; o++) i = i.matchType(e.child(o).type);
+        for (let s = t; i && s < r; s++) i = i.matchType(e.child(s).type);
         return i
     }
     get inlineContent() {
         return this.next.length != 0 && this.next[0].type.isInline
     }
     get defaultType() {
         for (let e = 0; e < this.next.length; e++) {
@@ -2184,31 +954,31 @@
             for (let r = 0; r < e.next.length; r++)
                 if (this.next[t].type == e.next[r].type) return !0;
         return !1
     }
     fillBefore(e, t = !1, r = 0) {
         let i = [this];
 
-        function o(s, l) {
-            let a = s.matchFragment(e, r);
-            if (a && (!t || a.validEnd)) return v.from(l.map(c => c.createAndFill()));
-            for (let c = 0; c < s.next.length; c++) {
+        function s(o, l) {
+            let a = o.matchFragment(e, r);
+            if (a && (!t || a.validEnd)) return x.from(l.map(c => c.createAndFill()));
+            for (let c = 0; c < o.next.length; c++) {
                 let {
                     type: u,
                     next: d
-                } = s.next[c];
+                } = o.next[c];
                 if (!(u.isText || u.hasRequiredAttrs()) && i.indexOf(d) == -1) {
                     i.push(d);
-                    let f = o(d, l.concat(u));
+                    let f = s(d, l.concat(u));
                     if (f) return f
                 }
             }
             return null
         }
-        return o(this, [])
+        return s(this, [])
     }
     findWrapping(e) {
         for (let r = 0; r < this.wrapCache.length; r += 2)
             if (this.wrapCache[r] == e) return this.wrapCache[r + 1];
         let t = this.computeWrapping(e);
         return this.wrapCache.push(e, t), t
     }
@@ -2217,25 +987,25 @@
             r = [{
                 match: this,
                 type: null,
                 via: null
             }];
         for (; r.length;) {
             let i = r.shift(),
-                o = i.match;
-            if (o.matchType(e)) {
-                let s = [];
-                for (let l = i; l.type; l = l.via) s.push(l.type);
-                return s.reverse()
+                s = i.match;
+            if (s.matchType(e)) {
+                let o = [];
+                for (let l = i; l.type; l = l.via) o.push(l.type);
+                return o.reverse()
             }
-            for (let s = 0; s < o.next.length; s++) {
+            for (let o = 0; o < s.next.length; o++) {
                 let {
                     type: l,
                     next: a
-                } = o.next[s];
+                } = s.next[o];
                 !l.isLeaf && !l.hasRequiredAttrs() && !(l.name in t) && (!i.type || a.validEnd) && (r.push({
                     match: l.contentMatch,
                     type: l,
                     via: i
                 }), t[l.name] = !0)
             }
         }
@@ -2252,290 +1022,290 @@
         let e = [];
 
         function t(r) {
             e.push(r);
             for (let i = 0; i < r.next.length; i++) e.indexOf(r.next[i].next) == -1 && t(r.next[i].next)
         }
         return t(this), e.map((r, i) => {
-            let o = i + (r.validEnd ? "*" : " ") + " ";
-            for (let s = 0; s < r.next.length; s++) o += (s ? ", " : "") + r.next[s].type.name + "->" + e.indexOf(r.next[s].next);
-            return o
+            let s = i + (r.validEnd ? "*" : " ") + " ";
+            for (let o = 0; o < r.next.length; o++) s += (o ? ", " : "") + r.next[o].type.name + "->" + e.indexOf(r.next[o].next);
+            return s
         }).join(`
 `)
     }
 };
-ht.empty = new ht(!0);
-var uo = class {
+He.empty = new He(!0);
+var Gr = class {
     constructor(e, t) {
         this.string = e, this.nodeTypes = t, this.inline = null, this.pos = 0, this.tokens = e.split(/\s*(?=\b|\W|$)/), this.tokens[this.tokens.length - 1] == "" && this.tokens.pop(), this.tokens[0] == "" && this.tokens.shift()
     }
     get next() {
         return this.tokens[this.pos]
     }
     eat(e) {
         return this.next == e && (this.pos++ || !0)
     }
     err(e) {
         throw new SyntaxError(e + " (in content expression '" + this.string + "')")
     }
 };
 
-function Gl(n) {
+function io(n) {
     let e = [];
-    do e.push(Zd(n)); while (n.eat("|"));
+    do e.push(wc(n)); while (n.eat("|"));
     return e.length == 1 ? e[0] : {
         type: "choice",
         exprs: e
     }
 }
 
-function Zd(n) {
+function wc(n) {
     let e = [];
-    do e.push(ef(n)); while (n.next && n.next != ")" && n.next != "|");
+    do e.push(Tc(n)); while (n.next && n.next != ")" && n.next != "|");
     return e.length == 1 ? e[0] : {
         type: "seq",
         exprs: e
     }
 }
 
-function ef(n) {
-    let e = rf(n);
+function Tc(n) {
+    let e = Oc(n);
     for (;;)
         if (n.eat("+")) e = {
             type: "plus",
             expr: e
         };
         else if (n.eat("*")) e = {
         type: "star",
         expr: e
     };
     else if (n.eat("?")) e = {
         type: "opt",
         expr: e
     };
-    else if (n.eat("{")) e = tf(n, e);
+    else if (n.eat("{")) e = Cc(n, e);
     else break;
     return e
 }
 
-function Rl(n) {
+function Ws(n) {
     /\D/.test(n.next) && n.err("Expected number, got '" + n.next + "'");
     let e = Number(n.next);
     return n.pos++, e
 }
 
-function tf(n, e) {
-    let t = Rl(n),
+function Cc(n, e) {
+    let t = Ws(n),
         r = t;
-    return n.eat(",") && (n.next != "}" ? r = Rl(n) : r = -1), n.eat("}") || n.err("Unclosed braced range"), {
+    return n.eat(",") && (n.next != "}" ? r = Ws(n) : r = -1), n.eat("}") || n.err("Unclosed braced range"), {
         type: "range",
         min: t,
         max: r,
         expr: e
     }
 }
 
-function nf(n, e) {
+function Ac(n, e) {
     let t = n.nodeTypes,
         r = t[e];
     if (r) return [r];
     let i = [];
-    for (let o in t) {
-        let s = t[o];
-        s.groups.indexOf(e) > -1 && i.push(s)
+    for (let s in t) {
+        let o = t[s];
+        o.groups.indexOf(e) > -1 && i.push(o)
     }
     return i.length == 0 && n.err("No node type or group '" + e + "' found"), i
 }
 
-function rf(n) {
+function Oc(n) {
     if (n.eat("(")) {
-        let e = Gl(n);
+        let e = io(n);
         return n.eat(")") || n.err("Missing closing paren"), e
     } else if (/\W/.test(n.next)) n.err("Unexpected token '" + n.next + "'");
     else {
-        let e = nf(n, n.next).map(t => (n.inline == null ? n.inline = t.isInline : n.inline != t.isInline && n.err("Mixing inline and block content"), {
+        let e = Ac(n, n.next).map(t => (n.inline == null ? n.inline = t.isInline : n.inline != t.isInline && n.err("Mixing inline and block content"), {
             type: "name",
             value: t
         }));
         return n.pos++, e.length == 1 ? e[0] : {
             type: "choice",
             exprs: e
         }
     }
 }
 
-function of(n) {
+function vc(n) {
     let e = [
         []
     ];
-    return i(o(n, 0), t()), e;
+    return i(s(n, 0), t()), e;
 
     function t() {
         return e.push([]) - 1
     }
 
-    function r(s, l, a) {
+    function r(o, l, a) {
         let c = {
             term: a,
             to: l
         };
-        return e[s].push(c), c
+        return e[o].push(c), c
     }
 
-    function i(s, l) {
-        s.forEach(a => a.to = l)
+    function i(o, l) {
+        o.forEach(a => a.to = l)
     }
 
-    function o(s, l) {
-        if (s.type == "choice") return s.exprs.reduce((a, c) => a.concat(o(c, l)), []);
-        if (s.type == "seq")
+    function s(o, l) {
+        if (o.type == "choice") return o.exprs.reduce((a, c) => a.concat(s(c, l)), []);
+        if (o.type == "seq")
             for (let a = 0;; a++) {
-                let c = o(s.exprs[a], l);
-                if (a == s.exprs.length - 1) return c;
+                let c = s(o.exprs[a], l);
+                if (a == o.exprs.length - 1) return c;
                 i(c, l = t())
-            } else if (s.type == "star") {
+            } else if (o.type == "star") {
                 let a = t();
-                return r(l, a), i(o(s.expr, a), a), [r(a)]
-            } else if (s.type == "plus") {
+                return r(l, a), i(s(o.expr, a), a), [r(a)]
+            } else if (o.type == "plus") {
             let a = t();
-            return i(o(s.expr, l), a), i(o(s.expr, a), a), [r(a)]
+            return i(s(o.expr, l), a), i(s(o.expr, a), a), [r(a)]
         } else {
-            if (s.type == "opt") return [r(l)].concat(o(s.expr, l));
-            if (s.type == "range") {
+            if (o.type == "opt") return [r(l)].concat(s(o.expr, l));
+            if (o.type == "range") {
                 let a = l;
-                for (let c = 0; c < s.min; c++) {
+                for (let c = 0; c < o.min; c++) {
                     let u = t();
-                    i(o(s.expr, a), u), a = u
+                    i(s(o.expr, a), u), a = u
                 }
-                if (s.max == -1) i(o(s.expr, a), a);
+                if (o.max == -1) i(s(o.expr, a), a);
                 else
-                    for (let c = s.min; c < s.max; c++) {
+                    for (let c = o.min; c < o.max; c++) {
                         let u = t();
-                        r(a, u), i(o(s.expr, a), u), a = u
+                        r(a, u), i(s(o.expr, a), u), a = u
                     }
                 return [r(a)]
             } else {
-                if (s.type == "name") return [r(l, void 0, s.value)];
+                if (o.type == "name") return [r(l, void 0, o.value)];
                 throw new Error("Unknown expr type")
             }
         }
     }
 }
 
-function Yl(n, e) {
+function so(n, e) {
     return e - n
 }
 
-function Bl(n, e) {
+function qs(n, e) {
     let t = [];
-    return r(e), t.sort(Yl);
+    return r(e), t.sort(so);
 
     function r(i) {
-        let o = n[i];
-        if (o.length == 1 && !o[0].term) return r(o[0].to);
+        let s = n[i];
+        if (s.length == 1 && !s[0].term) return r(s[0].to);
         t.push(i);
-        for (let s = 0; s < o.length; s++) {
+        for (let o = 0; o < s.length; o++) {
             let {
                 term: l,
                 to: a
-            } = o[s];
+            } = s[o];
             !l && t.indexOf(a) == -1 && r(a)
         }
     }
 }
 
-function sf(n) {
+function Nc(n) {
     let e = Object.create(null);
-    return t(Bl(n, 0));
+    return t(qs(n, 0));
 
     function t(r) {
         let i = [];
-        r.forEach(s => {
-            n[s].forEach(({
+        r.forEach(o => {
+            n[o].forEach(({
                 term: l,
                 to: a
             }) => {
                 if (!l) return;
                 let c;
                 for (let u = 0; u < i.length; u++) i[u][0] == l && (c = i[u][1]);
-                Bl(n, a).forEach(u => {
+                qs(n, a).forEach(u => {
                     c || i.push([l, c = []]), c.indexOf(u) == -1 && c.push(u)
                 })
             })
         });
-        let o = e[r.join(",")] = new ht(r.indexOf(n.length - 1) > -1);
-        for (let s = 0; s < i.length; s++) {
-            let l = i[s][1].sort(Yl);
-            o.next.push({
-                type: i[s][0],
+        let s = e[r.join(",")] = new He(r.indexOf(n.length - 1) > -1);
+        for (let o = 0; o < i.length; o++) {
+            let l = i[o][1].sort(so);
+            s.next.push({
+                type: i[o][0],
                 next: e[l.join(",")] || t(l)
             })
         }
-        return o
+        return s
     }
 }
 
-function lf(n, e) {
+function Ic(n, e) {
     for (let t = 0, r = [n]; t < r.length; t++) {
         let i = r[t],
-            o = !i.validEnd,
-            s = [];
+            s = !i.validEnd,
+            o = [];
         for (let l = 0; l < i.next.length; l++) {
             let {
                 type: a,
                 next: c
             } = i.next[l];
-            s.push(a.name), o && !(a.isText || a.hasRequiredAttrs()) && (o = !1), r.indexOf(c) == -1 && r.push(c)
+            o.push(a.name), s && !(a.isText || a.hasRequiredAttrs()) && (s = !1), r.indexOf(c) == -1 && r.push(c)
         }
-        o && e.err("Only non-generatable nodes (" + s.join(", ") + ") in a required position (see https://prosemirror.net/docs/guide/#generatable)")
+        s && e.err("Only non-generatable nodes (" + o.join(", ") + ") in a required position (see https://prosemirror.net/docs/guide/#generatable)")
     }
 }
 
-function Ql(n) {
+function oo(n) {
     let e = Object.create(null);
     for (let t in n) {
         let r = n[t];
         if (!r.hasDefault) return null;
         e[t] = r.default
     }
     return e
 }
 
-function Xl(n, e) {
+function lo(n, e) {
     let t = Object.create(null);
     for (let r in n) {
         let i = e && e[r];
         if (i === void 0) {
-            let o = n[r];
-            if (o.hasDefault) i = o.default;
+            let s = n[r];
+            if (s.hasDefault) i = s.default;
             else throw new RangeError("No value supplied for attribute " + r)
         }
         t[r] = i
     }
     return t
 }
 
-function Zl(n) {
+function ao(n) {
     let e = Object.create(null);
     if (n)
-        for (let t in n) e[t] = new fo(n[t]);
+        for (let t in n) e[t] = new Qr(n[t]);
     return e
 }
-var An = class {
+var Bt = class {
         constructor(e, t, r) {
-            this.name = e, this.schema = t, this.spec = r, this.markSet = null, this.groups = r.group ? r.group.split(" ") : [], this.attrs = Zl(r.attrs), this.defaultAttrs = Ql(this.attrs), this.contentMatch = null, this.inlineContent = null, this.isBlock = !(r.inline || e == "text"), this.isText = e == "text"
+            this.name = e, this.schema = t, this.spec = r, this.markSet = null, this.groups = r.group ? r.group.split(" ") : [], this.attrs = ao(r.attrs), this.defaultAttrs = oo(this.attrs), this.contentMatch = null, this.inlineContent = null, this.isBlock = !(r.inline || e == "text"), this.isText = e == "text"
         }
         get isInline() {
             return !this.isBlock
         }
         get isTextblock() {
             return this.isBlock && this.inlineContent
         }
         get isLeaf() {
-            return this.contentMatch == ht.empty
+            return this.contentMatch == He.empty
         }
         get isAtom() {
             return this.isLeaf || !!this.spec.atom
         }
         get whitespace() {
             return this.spec.whitespace || (this.spec.code ? "pre" : "normal")
         }
@@ -2544,32 +1314,32 @@
                 if (this.attrs[e].isRequired) return !0;
             return !1
         }
         compatibleContent(e) {
             return this == e || this.contentMatch.compatible(e.contentMatch)
         }
         computeAttrs(e) {
-            return !e && this.defaultAttrs ? this.defaultAttrs : Xl(this.attrs, e)
+            return !e && this.defaultAttrs ? this.defaultAttrs : lo(this.attrs, e)
         }
         create(e = null, t, r) {
             if (this.isText) throw new Error("NodeType.create can't construct text nodes");
-            return new we(this, this.computeAttrs(e), v.from(t), H.setFrom(r))
+            return new ue(this, this.computeAttrs(e), x.from(t), B.setFrom(r))
         }
         createChecked(e = null, t, r) {
-            return t = v.from(t), this.checkContent(t), new we(this, this.computeAttrs(e), t, H.setFrom(r))
+            return t = x.from(t), this.checkContent(t), new ue(this, this.computeAttrs(e), t, B.setFrom(r))
         }
         createAndFill(e = null, t, r) {
-            if (e = this.computeAttrs(e), t = v.from(t), t.size) {
-                let s = this.contentMatch.fillBefore(t);
-                if (!s) return null;
-                t = s.append(t)
+            if (e = this.computeAttrs(e), t = x.from(t), t.size) {
+                let o = this.contentMatch.fillBefore(t);
+                if (!o) return null;
+                t = o.append(t)
             }
             let i = this.contentMatch.matchFragment(t),
-                o = i && i.fillBefore(v.empty, !0);
-            return o ? new we(this, e, t.append(o), H.setFrom(r)) : null
+                s = i && i.fillBefore(x.empty, !0);
+            return s ? new ue(this, e, t.append(s), B.setFrom(r)) : null
         }
         validContent(e) {
             let t = this.contentMatch.matchFragment(e);
             if (!t || !t.validEnd) return !1;
             for (let r = 0; r < e.childCount; r++)
                 if (!this.allowsMarks(e.child(r).marks)) return !1;
             return !0
@@ -2586,200 +1356,200 @@
                 if (!this.allowsMarkType(e[t].type)) return !1;
             return !0
         }
         allowedMarks(e) {
             if (this.markSet == null) return e;
             let t;
             for (let r = 0; r < e.length; r++) this.allowsMarkType(e[r].type) ? t && t.push(e[r]) : t || (t = e.slice(0, r));
-            return t ? t.length ? t : H.none : e
+            return t ? t.length ? t : B.none : e
         }
         static compile(e, t) {
             let r = Object.create(null);
-            e.forEach((o, s) => r[o] = new An(o, t, s));
+            e.forEach((s, o) => r[s] = new Bt(s, t, o));
             let i = t.spec.topNode || "doc";
             if (!r[i]) throw new RangeError("Schema is missing its top node type ('" + i + "')");
             if (!r.text) throw new RangeError("Every schema needs a 'text' type");
-            for (let o in r.text.attrs) throw new RangeError("The text node type should not have attributes");
+            for (let s in r.text.attrs) throw new RangeError("The text node type should not have attributes");
             return r
         }
     },
-    fo = class {
+    Qr = class {
         constructor(e) {
             this.hasDefault = Object.prototype.hasOwnProperty.call(e, "default"), this.default = e.default
         }
         get isRequired() {
             return !this.hasDefault
         }
     },
-    sn = class {
+    bt = class {
         constructor(e, t, r, i) {
-            this.name = e, this.rank = t, this.schema = r, this.spec = i, this.attrs = Zl(i.attrs), this.excluded = null;
-            let o = Ql(this.attrs);
-            this.instance = o ? new H(this, o) : null
+            this.name = e, this.rank = t, this.schema = r, this.spec = i, this.attrs = ao(i.attrs), this.excluded = null;
+            let s = oo(this.attrs);
+            this.instance = s ? new B(this, s) : null
         }
         create(e = null) {
-            return !e && this.instance ? this.instance : new H(this, Xl(this.attrs, e))
+            return !e && this.instance ? this.instance : new B(this, lo(this.attrs, e))
         }
         static compile(e, t) {
             let r = Object.create(null),
                 i = 0;
-            return e.forEach((o, s) => r[o] = new sn(o, i++, t, s)), r
+            return e.forEach((s, o) => r[s] = new bt(s, i++, t, o)), r
         }
         removeFromSet(e) {
             for (var t = 0; t < e.length; t++) e[t].type == this && (e = e.slice(0, t).concat(e.slice(t + 1)), t--);
             return e
         }
         isInSet(e) {
             for (let t = 0; t < e.length; t++)
                 if (e[t].type == this) return e[t]
         }
         excludes(e) {
             return this.excluded.indexOf(e) > -1
         }
     },
-    Wr = class {
+    Wn = class {
         constructor(e) {
             this.cached = Object.create(null);
             let t = this.spec = {};
             for (let i in e) t[i] = e[i];
-            t.nodes = io.from(e.nodes), t.marks = io.from(e.marks || {}), this.nodes = An.compile(this.spec.nodes, this), this.marks = sn.compile(this.spec.marks, this);
+            t.nodes = Jr.from(e.nodes), t.marks = Jr.from(e.marks || {}), this.nodes = Bt.compile(this.spec.nodes, this), this.marks = bt.compile(this.spec.marks, this);
             let r = Object.create(null);
             for (let i in this.nodes) {
                 if (i in this.marks) throw new RangeError(i + " can not be both a node and a mark");
-                let o = this.nodes[i],
-                    s = o.spec.content || "",
-                    l = o.spec.marks;
-                o.contentMatch = r[s] || (r[s] = ht.parse(s, this.nodes)), o.inlineContent = o.contentMatch.inlineContent, o.markSet = l == "_" ? null : l ? zl(this, l.split(" ")) : l == "" || !o.inlineContent ? [] : null
+                let s = this.nodes[i],
+                    o = s.spec.content || "",
+                    l = s.spec.marks;
+                s.contentMatch = r[o] || (r[o] = He.parse(o, this.nodes)), s.inlineContent = s.contentMatch.inlineContent, s.markSet = l == "_" ? null : l ? Ks(this, l.split(" ")) : l == "" || !s.inlineContent ? [] : null
             }
             for (let i in this.marks) {
-                let o = this.marks[i],
-                    s = o.spec.excludes;
-                o.excluded = s == null ? [o] : s == "" ? [] : zl(this, s.split(" "))
+                let s = this.marks[i],
+                    o = s.spec.excludes;
+                s.excluded = o == null ? [s] : o == "" ? [] : Ks(this, o.split(" "))
             }
             this.nodeFromJSON = this.nodeFromJSON.bind(this), this.markFromJSON = this.markFromJSON.bind(this), this.topNodeType = this.nodes[this.spec.topNode || "doc"], this.cached.wrappings = Object.create(null)
         }
         node(e, t = null, r, i) {
             if (typeof e == "string") e = this.nodeType(e);
-            else if (e instanceof An) {
+            else if (e instanceof Bt) {
                 if (e.schema != this) throw new RangeError("Node type from different schema used (" + e.name + ")")
             } else throw new RangeError("Invalid node type: " + e);
             return e.createChecked(t, r, i)
         }
         text(e, t) {
             let r = this.nodes.text;
-            return new On(r, r.defaultAttrs, e, H.setFrom(t))
+            return new Pt(r, r.defaultAttrs, e, B.setFrom(t))
         }
         mark(e, t) {
             return typeof e == "string" && (e = this.marks[e]), e.create(t)
         }
         nodeFromJSON(e) {
-            return we.fromJSON(this, e)
+            return ue.fromJSON(this, e)
         }
         markFromJSON(e) {
-            return H.fromJSON(this, e)
+            return B.fromJSON(this, e)
         }
         nodeType(e) {
             let t = this.nodes[e];
             if (!t) throw new RangeError("Unknown node type: " + e);
             return t
         }
     };
 
-function zl(n, e) {
+function Ks(n, e) {
     let t = [];
     for (let r = 0; r < e.length; r++) {
         let i = e[r],
-            o = n.marks[i],
-            s = o;
-        if (o) t.push(o);
+            s = n.marks[i],
+            o = s;
+        if (s) t.push(s);
         else
             for (let l in n.marks) {
                 let a = n.marks[l];
-                (i == "_" || a.spec.group && a.spec.group.split(" ").indexOf(i) > -1) && t.push(s = a)
+                (i == "_" || a.spec.group && a.spec.group.split(" ").indexOf(i) > -1) && t.push(o = a)
             }
-        if (!s) throw new SyntaxError("Unknown mark type: '" + e[r] + "'")
+        if (!o) throw new SyntaxError("Unknown mark type: '" + e[r] + "'")
     }
     return t
 }
-var Qe = class {
+var Te = class {
         constructor(e, t) {
             this.schema = e, this.rules = t, this.tags = [], this.styles = [], t.forEach(r => {
                 r.tag ? this.tags.push(r) : r.style && this.styles.push(r)
             }), this.normalizeLists = !this.tags.some(r => {
                 if (!/^(ul|ol)\b/.test(r.tag) || !r.node) return !1;
                 let i = e.nodes[r.node];
                 return i.contentMatch.matchType(i)
             })
         }
         parse(e, t = {}) {
-            let r = new Kr(this, t, !1);
+            let r = new Un(this, t, !1);
             return r.addAll(e, t.from, t.to), r.finish()
         }
         parseSlice(e, t = {}) {
-            let r = new Kr(this, t, !0);
-            return r.addAll(e, t.from, t.to), w.maxOpen(r.finish())
+            let r = new Un(this, t, !0);
+            return r.addAll(e, t.from, t.to), E.maxOpen(r.finish())
         }
         matchTag(e, t, r) {
             for (let i = r ? this.tags.indexOf(r) + 1 : 0; i < this.tags.length; i++) {
-                let o = this.tags[i];
-                if (uf(e, o.tag) && (o.namespace === void 0 || e.namespaceURI == o.namespace) && (!o.context || t.matchesContext(o.context))) {
-                    if (o.getAttrs) {
-                        let s = o.getAttrs(e);
-                        if (s === !1) continue;
-                        o.attrs = s || void 0
+                let s = this.tags[i];
+                if (Rc(e, s.tag) && (s.namespace === void 0 || e.namespaceURI == s.namespace) && (!s.context || t.matchesContext(s.context))) {
+                    if (s.getAttrs) {
+                        let o = s.getAttrs(e);
+                        if (o === !1) continue;
+                        s.attrs = o || void 0
                     }
-                    return o
+                    return s
                 }
             }
         }
         matchStyle(e, t, r, i) {
-            for (let o = i ? this.styles.indexOf(i) + 1 : 0; o < this.styles.length; o++) {
-                let s = this.styles[o],
-                    l = s.style;
-                if (!(l.indexOf(e) != 0 || s.context && !r.matchesContext(s.context) || l.length > e.length && (l.charCodeAt(e.length) != 61 || l.slice(e.length + 1) != t))) {
-                    if (s.getAttrs) {
-                        let a = s.getAttrs(t);
+            for (let s = i ? this.styles.indexOf(i) + 1 : 0; s < this.styles.length; s++) {
+                let o = this.styles[s],
+                    l = o.style;
+                if (!(l.indexOf(e) != 0 || o.context && !r.matchesContext(o.context) || l.length > e.length && (l.charCodeAt(e.length) != 61 || l.slice(e.length + 1) != t))) {
+                    if (o.getAttrs) {
+                        let a = o.getAttrs(t);
                         if (a === !1) continue;
-                        s.attrs = a || void 0
+                        o.attrs = a || void 0
                     }
-                    return s
+                    return o
                 }
             }
         }
         static schemaRules(e) {
             let t = [];
 
             function r(i) {
-                let o = i.priority == null ? 50 : i.priority,
-                    s = 0;
-                for (; s < t.length; s++) {
-                    let l = t[s];
-                    if ((l.priority == null ? 50 : l.priority) < o) break
+                let s = i.priority == null ? 50 : i.priority,
+                    o = 0;
+                for (; o < t.length; o++) {
+                    let l = t[o];
+                    if ((l.priority == null ? 50 : l.priority) < s) break
                 }
-                t.splice(s, 0, i)
+                t.splice(o, 0, i)
             }
             for (let i in e.marks) {
-                let o = e.marks[i].spec.parseDOM;
-                o && o.forEach(s => {
-                    r(s = Fl(s)), s.mark || s.ignore || s.clearMark || (s.mark = i)
+                let s = e.marks[i].spec.parseDOM;
+                s && s.forEach(o => {
+                    r(o = _s(o)), o.mark || o.ignore || o.clearMark || (o.mark = i)
                 })
             }
             for (let i in e.nodes) {
-                let o = e.nodes[i].spec.parseDOM;
-                o && o.forEach(s => {
-                    r(s = Fl(s)), s.node || s.ignore || s.mark || (s.node = i)
+                let s = e.nodes[i].spec.parseDOM;
+                s && s.forEach(o => {
+                    r(o = _s(o)), o.node || o.ignore || o.mark || (o.node = i)
                 })
             }
             return t
         }
         static fromSchema(e) {
-            return e.cached.domParser || (e.cached.domParser = new Qe(e, Qe.schemaRules(e)))
+            return e.cached.domParser || (e.cached.domParser = new Te(e, Te.schemaRules(e)))
         }
     },
-    ea = {
+    co = {
         address: !0,
         article: !0,
         aside: !0,
         blockquote: !0,
         canvas: !0,
         dd: !0,
         div: !0,
@@ -2805,181 +1575,181 @@
         p: !0,
         pre: !0,
         section: !0,
         table: !0,
         tfoot: !0,
         ul: !0
     },
-    af = {
+    Dc = {
         head: !0,
         noscript: !0,
         object: !0,
         script: !0,
         style: !0,
         title: !0
     },
-    ta = {
+    uo = {
         ol: !0,
         ul: !0
     },
-    qr = 1,
-    Jr = 2,
-    ar = 4;
-
-function Hl(n, e, t) {
-    return e != null ? (e ? qr : 0) | (e === "full" ? Jr : 0) : n && n.whitespace == "pre" ? qr | Jr : t & ~ar
-}
-var Cn = class {
-        constructor(e, t, r, i, o, s, l) {
-            this.type = e, this.attrs = t, this.marks = r, this.pendingMarks = i, this.solid = o, this.options = l, this.content = [], this.activeMarks = H.none, this.stashMarks = [], this.match = s || (l & ar ? null : e.contentMatch)
+    qn = 1,
+    Kn = 2,
+    un = 4;
+
+function Us(n, e, t) {
+    return e != null ? (e ? qn : 0) | (e === "full" ? Kn : 0) : n && n.whitespace == "pre" ? qn | Kn : t & ~un
+}
+var Rt = class {
+        constructor(e, t, r, i, s, o, l) {
+            this.type = e, this.attrs = t, this.marks = r, this.pendingMarks = i, this.solid = s, this.options = l, this.content = [], this.activeMarks = B.none, this.stashMarks = [], this.match = o || (l & un ? null : e.contentMatch)
         }
         findWrapping(e) {
             if (!this.match) {
                 if (!this.type) return [];
-                let t = this.type.contentMatch.fillBefore(v.from(e));
+                let t = this.type.contentMatch.fillBefore(x.from(e));
                 if (t) this.match = this.type.contentMatch.matchFragment(t);
                 else {
                     let r = this.type.contentMatch,
                         i;
                     return (i = r.findWrapping(e.type)) ? (this.match = r, i) : null
                 }
             }
             return this.match.findWrapping(e.type)
         }
         finish(e) {
-            if (!(this.options & qr)) {
+            if (!(this.options & qn)) {
                 let r = this.content[this.content.length - 1],
                     i;
                 if (r && r.isText && (i = /[ \t\r\n\u000c]+$/.exec(r.text))) {
-                    let o = r;
-                    r.text.length == i[0].length ? this.content.pop() : this.content[this.content.length - 1] = o.withText(o.text.slice(0, o.text.length - i[0].length))
+                    let s = r;
+                    r.text.length == i[0].length ? this.content.pop() : this.content[this.content.length - 1] = s.withText(s.text.slice(0, s.text.length - i[0].length))
                 }
             }
-            let t = v.from(this.content);
-            return !e && this.match && (t = t.append(this.match.fillBefore(v.empty, !0))), this.type ? this.type.create(this.attrs, t, this.marks) : t
+            let t = x.from(this.content);
+            return !e && this.match && (t = t.append(this.match.fillBefore(x.empty, !0))), this.type ? this.type.create(this.attrs, t, this.marks) : t
         }
         popFromStashMark(e) {
             for (let t = this.stashMarks.length - 1; t >= 0; t--)
                 if (e.eq(this.stashMarks[t])) return this.stashMarks.splice(t, 1)[0]
         }
         applyPending(e) {
             for (let t = 0, r = this.pendingMarks; t < r.length; t++) {
                 let i = r[t];
-                (this.type ? this.type.allowsMarkType(i.type) : ff(i.type, e)) && !i.isInSet(this.activeMarks) && (this.activeMarks = i.addToSet(this.activeMarks), this.pendingMarks = i.removeFromSet(this.pendingMarks))
+                (this.type ? this.type.allowsMarkType(i.type) : Bc(i.type, e)) && !i.isInSet(this.activeMarks) && (this.activeMarks = i.addToSet(this.activeMarks), this.pendingMarks = i.removeFromSet(this.pendingMarks))
             }
         }
         inlineContext(e) {
-            return this.type ? this.type.inlineContent : this.content.length ? this.content[0].isInline : e.parentNode && !ea.hasOwnProperty(e.parentNode.nodeName.toLowerCase())
+            return this.type ? this.type.inlineContent : this.content.length ? this.content[0].isInline : e.parentNode && !co.hasOwnProperty(e.parentNode.nodeName.toLowerCase())
         }
     },
-    Kr = class {
+    Un = class {
         constructor(e, t, r) {
             this.parser = e, this.options = t, this.isOpen = r, this.open = 0;
             let i = t.topNode,
-                o, s = Hl(null, t.preserveWhitespace, 0) | (r ? ar : 0);
-            i ? o = new Cn(i.type, i.attrs, H.none, H.none, !0, t.topMatch || i.type.contentMatch, s) : r ? o = new Cn(null, null, H.none, H.none, !0, null, s) : o = new Cn(e.schema.topNodeType, null, H.none, H.none, !0, null, s), this.nodes = [o], this.find = t.findPositions, this.needsBlock = !1
+                s, o = Us(null, t.preserveWhitespace, 0) | (r ? un : 0);
+            i ? s = new Rt(i.type, i.attrs, B.none, B.none, !0, t.topMatch || i.type.contentMatch, o) : r ? s = new Rt(null, null, B.none, B.none, !0, null, o) : s = new Rt(e.schema.topNodeType, null, B.none, B.none, !0, null, o), this.nodes = [s], this.find = t.findPositions, this.needsBlock = !1
         }
         get top() {
             return this.nodes[this.open]
         }
         addDOM(e) {
             if (e.nodeType == 3) this.addTextNode(e);
             else if (e.nodeType == 1) {
                 let t = e.getAttribute("style");
                 if (!t) this.addElement(e);
                 else {
-                    let r = this.readStyles(df(t));
+                    let r = this.readStyles(Pc(t));
                     if (!r) return;
-                    let [i, o] = r, s = this.top;
-                    for (let l = 0; l < o.length; l++) this.removePendingMark(o[l], s);
+                    let [i, s] = r, o = this.top;
+                    for (let l = 0; l < s.length; l++) this.removePendingMark(s[l], o);
                     for (let l = 0; l < i.length; l++) this.addPendingMark(i[l]);
                     this.addElement(e);
-                    for (let l = 0; l < i.length; l++) this.removePendingMark(i[l], s);
-                    for (let l = 0; l < o.length; l++) this.addPendingMark(o[l])
+                    for (let l = 0; l < i.length; l++) this.removePendingMark(i[l], o);
+                    for (let l = 0; l < s.length; l++) this.addPendingMark(s[l])
                 }
             }
         }
         addTextNode(e) {
             let t = e.nodeValue,
                 r = this.top;
-            if (r.options & Jr || r.inlineContext(e) || /[^ \t\r\n\u000c]/.test(t)) {
-                if (r.options & qr) r.options & Jr ? t = t.replace(/\r\n?/g, `
+            if (r.options & Kn || r.inlineContext(e) || /[^ \t\r\n\u000c]/.test(t)) {
+                if (r.options & qn) r.options & Kn ? t = t.replace(/\r\n?/g, `
 `) : t = t.replace(/\r?\n|\r/g, " ");
                 else if (t = t.replace(/[ \t\r\n\u000c]+/g, " "), /^[ \t\r\n\u000c]/.test(t) && this.open == this.nodes.length - 1) {
                     let i = r.content[r.content.length - 1],
-                        o = e.previousSibling;
-                    (!i || o && o.nodeName == "BR" || i.isText && /[ \t\r\n\u000c]$/.test(i.text)) && (t = t.slice(1))
+                        s = e.previousSibling;
+                    (!i || s && s.nodeName == "BR" || i.isText && /[ \t\r\n\u000c]$/.test(i.text)) && (t = t.slice(1))
                 }
                 t && this.insertNode(this.parser.schema.text(t)), this.findInText(e)
             } else this.findInside(e)
         }
         addElement(e, t) {
             let r = e.nodeName.toLowerCase(),
                 i;
-            ta.hasOwnProperty(r) && this.parser.normalizeLists && cf(e);
-            let o = this.options.ruleFromNode && this.options.ruleFromNode(e) || (i = this.parser.matchTag(e, this, t));
-            if (o ? o.ignore : af.hasOwnProperty(r)) this.findInside(e), this.ignoreFallback(e);
-            else if (!o || o.skip || o.closeParent) {
-                o && o.closeParent ? this.open = Math.max(0, this.open - 1) : o && o.skip.nodeType && (e = o.skip);
-                let s, l = this.top,
+            uo.hasOwnProperty(r) && this.parser.normalizeLists && Lc(e);
+            let s = this.options.ruleFromNode && this.options.ruleFromNode(e) || (i = this.parser.matchTag(e, this, t));
+            if (s ? s.ignore : Dc.hasOwnProperty(r)) this.findInside(e), this.ignoreFallback(e);
+            else if (!s || s.skip || s.closeParent) {
+                s && s.closeParent ? this.open = Math.max(0, this.open - 1) : s && s.skip.nodeType && (e = s.skip);
+                let o, l = this.top,
                     a = this.needsBlock;
-                if (ea.hasOwnProperty(r)) l.content.length && l.content[0].isInline && this.open && (this.open--, l = this.top), s = !0, l.type || (this.needsBlock = !0);
+                if (co.hasOwnProperty(r)) l.content.length && l.content[0].isInline && this.open && (this.open--, l = this.top), o = !0, l.type || (this.needsBlock = !0);
                 else if (!e.firstChild) {
                     this.leafFallback(e);
                     return
                 }
-                this.addAll(e), s && this.sync(l), this.needsBlock = a
-            } else this.addElementByRule(e, o, o.consuming === !1 ? i : void 0)
+                this.addAll(e), o && this.sync(l), this.needsBlock = a
+            } else this.addElementByRule(e, s, s.consuming === !1 ? i : void 0)
         }
         leafFallback(e) {
             e.nodeName == "BR" && this.top.type && this.top.type.inlineContent && this.addTextNode(e.ownerDocument.createTextNode(`
 `))
         }
         ignoreFallback(e) {
             e.nodeName == "BR" && (!this.top.type || !this.top.type.inlineContent) && this.findPlace(this.parser.schema.text("-"))
         }
         readStyles(e) {
-            let t = H.none,
-                r = H.none;
+            let t = B.none,
+                r = B.none;
             for (let i = 0; i < e.length; i += 2)
-                for (let o = void 0;;) {
-                    let s = this.parser.matchStyle(e[i], e[i + 1], this, o);
-                    if (!s) break;
-                    if (s.ignore) return null;
-                    if (s.clearMark ? this.top.pendingMarks.concat(this.top.activeMarks).forEach(l => {
-                            s.clearMark(l) && (r = l.addToSet(r))
-                        }) : t = this.parser.schema.marks[s.mark].create(s.attrs).addToSet(t), s.consuming === !1) o = s;
+                for (let s = void 0;;) {
+                    let o = this.parser.matchStyle(e[i], e[i + 1], this, s);
+                    if (!o) break;
+                    if (o.ignore) return null;
+                    if (o.clearMark ? this.top.pendingMarks.concat(this.top.activeMarks).forEach(l => {
+                            o.clearMark(l) && (r = l.addToSet(r))
+                        }) : t = this.parser.schema.marks[o.mark].create(o.attrs).addToSet(t), o.consuming === !1) s = o;
                     else break
                 }
             return [t, r]
         }
         addElementByRule(e, t, r) {
-            let i, o, s;
-            t.node ? (o = this.parser.schema.nodes[t.node], o.isLeaf ? this.insertNode(o.create(t.attrs)) || this.leafFallback(e) : i = this.enter(o, t.attrs || null, t.preserveWhitespace)) : (s = this.parser.schema.marks[t.mark].create(t.attrs), this.addPendingMark(s));
+            let i, s, o;
+            t.node ? (s = this.parser.schema.nodes[t.node], s.isLeaf ? this.insertNode(s.create(t.attrs)) || this.leafFallback(e) : i = this.enter(s, t.attrs || null, t.preserveWhitespace)) : (o = this.parser.schema.marks[t.mark].create(t.attrs), this.addPendingMark(o));
             let l = this.top;
-            if (o && o.isLeaf) this.findInside(e);
+            if (s && s.isLeaf) this.findInside(e);
             else if (r) this.addElement(e, r);
             else if (t.getContent) this.findInside(e), t.getContent(e, this.parser.schema).forEach(a => this.insertNode(a));
             else {
                 let a = e;
                 typeof t.contentElement == "string" ? a = e.querySelector(t.contentElement) : typeof t.contentElement == "function" ? a = t.contentElement(e) : t.contentElement && (a = t.contentElement), this.findAround(e, a, !0), this.addAll(a)
             }
-            i && this.sync(l) && this.open--, s && this.removePendingMark(s, l)
+            i && this.sync(l) && this.open--, o && this.removePendingMark(o, l)
         }
         addAll(e, t, r) {
             let i = t || 0;
-            for (let o = t ? e.childNodes[t] : e.firstChild, s = r == null ? null : e.childNodes[r]; o != s; o = o.nextSibling, ++i) this.findAtPoint(e, i), this.addDOM(o);
+            for (let s = t ? e.childNodes[t] : e.firstChild, o = r == null ? null : e.childNodes[r]; s != o; s = s.nextSibling, ++i) this.findAtPoint(e, i), this.addDOM(s);
             this.findAtPoint(e, i)
         }
         findPlace(e) {
             let t, r;
             for (let i = this.open; i >= 0; i--) {
-                let o = this.nodes[i],
-                    s = o.findWrapping(e);
-                if (s && (!t || t.length > s.length) && (t = s, r = o, !s.length) || o.solid) break
+                let s = this.nodes[i],
+                    o = s.findWrapping(e);
+                if (o && (!t || t.length > o.length) && (t = o, r = s, !o.length) || s.solid) break
             }
             if (!t) return !1;
             this.sync(r);
             for (let i = 0; i < t.length; i++) this.enterInner(t[i], null, !1);
             return !0
         }
         insertNode(e) {
@@ -2999,18 +1769,18 @@
         }
         enter(e, t, r) {
             let i = this.findPlace(e.create(t));
             return i && this.enterInner(e, t, !0, r), i
         }
         enterInner(e, t = null, r = !1, i) {
             this.closeExtra();
-            let o = this.top;
-            o.applyPending(e), o.match = o.match && o.match.matchType(e);
-            let s = Hl(e, i, o.options);
-            o.options & ar && o.content.length == 0 && (s |= ar), this.nodes.push(new Cn(e, t, o.activeMarks, o.pendingMarks, r, null, s)), this.open++
+            let s = this.top;
+            s.applyPending(e), s.match = s.match && s.match.matchType(e);
+            let o = Us(e, i, s.options);
+            s.options & un && s.content.length == 0 && (o |= un), this.nodes.push(new Rt(e, t, s.activeMarks, s.pendingMarks, r, null, o)), this.open++
         }
         closeExtra(e = !1) {
             let t = this.nodes.length - 1;
             if (t > this.open) {
                 for (; t > this.open; t--) this.nodes[t - 1].content.push(this.nodes[t].finish(e));
                 this.nodes.length = this.open + 1
             }
@@ -3050,177 +1820,177 @@
                 for (let t = 0; t < this.find.length; t++) this.find[t].node == e && (this.find[t].pos = this.currentPos - (e.nodeValue.length - this.find[t].offset))
         }
         matchesContext(e) {
             if (e.indexOf("|") > -1) return e.split(/\s*\|\s*/).some(this.matchesContext, this);
             let t = e.split("/"),
                 r = this.options.context,
                 i = !this.isOpen && (!r || r.parent.type == this.nodes[0].type),
-                o = -(r ? r.depth + 1 : 0) + (i ? 0 : 1),
-                s = (l, a) => {
+                s = -(r ? r.depth + 1 : 0) + (i ? 0 : 1),
+                o = (l, a) => {
                     for (; l >= 0; l--) {
                         let c = t[l];
                         if (c == "") {
                             if (l == t.length - 1 || l == 0) continue;
-                            for (; a >= o; a--)
-                                if (s(l - 1, a)) return !0;
+                            for (; a >= s; a--)
+                                if (o(l - 1, a)) return !0;
                             return !1
                         } else {
-                            let u = a > 0 || a == 0 && i ? this.nodes[a].type : r && a >= o ? r.node(a - o).type : null;
+                            let u = a > 0 || a == 0 && i ? this.nodes[a].type : r && a >= s ? r.node(a - s).type : null;
                             if (!u || u.name != c && u.groups.indexOf(c) == -1) return !1;
                             a--
                         }
                     }
                     return !0
                 };
-            return s(t.length - 1, this.open)
+            return o(t.length - 1, this.open)
         }
         textblockFromContext() {
             let e = this.options.context;
             if (e)
                 for (let t = e.depth; t >= 0; t--) {
                     let r = e.node(t).contentMatchAt(e.indexAfter(t)).defaultType;
                     if (r && r.isTextblock && r.defaultAttrs) return r
                 }
             for (let t in this.parser.schema.nodes) {
                 let r = this.parser.schema.nodes[t];
                 if (r.isTextblock && r.defaultAttrs) return r
             }
         }
         addPendingMark(e) {
-            let t = pf(e, this.top.pendingMarks);
+            let t = zc(e, this.top.pendingMarks);
             t && this.top.stashMarks.push(t), this.top.pendingMarks = e.addToSet(this.top.pendingMarks)
         }
         removePendingMark(e, t) {
             for (let r = this.open; r >= 0; r--) {
                 let i = this.nodes[r];
                 if (i.pendingMarks.lastIndexOf(e) > -1) i.pendingMarks = e.removeFromSet(i.pendingMarks);
                 else {
                     i.activeMarks = e.removeFromSet(i.activeMarks);
-                    let s = i.popFromStashMark(e);
-                    s && i.type && i.type.allowsMarkType(s.type) && (i.activeMarks = s.addToSet(i.activeMarks))
+                    let o = i.popFromStashMark(e);
+                    o && i.type && i.type.allowsMarkType(o.type) && (i.activeMarks = o.addToSet(i.activeMarks))
                 }
                 if (i == t) break
             }
         }
     };
 
-function cf(n) {
+function Lc(n) {
     for (let e = n.firstChild, t = null; e; e = e.nextSibling) {
         let r = e.nodeType == 1 ? e.nodeName.toLowerCase() : null;
-        r && ta.hasOwnProperty(r) && t ? (t.appendChild(e), e = t) : r == "li" ? t = e : r && (t = null)
+        r && uo.hasOwnProperty(r) && t ? (t.appendChild(e), e = t) : r == "li" ? t = e : r && (t = null)
     }
 }
 
-function uf(n, e) {
+function Rc(n, e) {
     return (n.matches || n.msMatchesSelector || n.webkitMatchesSelector || n.mozMatchesSelector).call(n, e)
 }
 
-function df(n) {
+function Pc(n) {
     let e = /\s*([\w-]+)\s*:\s*([^;]+)/g,
         t, r = [];
     for (; t = e.exec(n);) r.push(t[1], t[2].trim());
     return r
 }
 
-function Fl(n) {
+function _s(n) {
     let e = {};
     for (let t in n) e[t] = n[t];
     return e
 }
 
-function ff(n, e) {
+function Bc(n, e) {
     let t = e.schema.nodes;
     for (let r in t) {
         let i = t[r];
         if (!i.allowsMarkType(n)) continue;
-        let o = [],
-            s = l => {
-                o.push(l);
+        let s = [],
+            o = l => {
+                s.push(l);
                 for (let a = 0; a < l.edgeCount; a++) {
                     let {
                         type: c,
                         next: u
                     } = l.edge(a);
-                    if (c == e || o.indexOf(u) < 0 && s(u)) return !0
+                    if (c == e || s.indexOf(u) < 0 && o(u)) return !0
                 }
             };
-        if (s(i.contentMatch)) return !0
+        if (o(i.contentMatch)) return !0
     }
 }
 
-function pf(n, e) {
+function zc(n, e) {
     for (let t = 0; t < e.length; t++)
         if (n.eq(e[t])) return e[t]
 }
-var Se = class {
+var ce = class {
     constructor(e, t) {
         this.nodes = e, this.marks = t
     }
     serializeFragment(e, t = {}, r) {
-        r || (r = ao(t).createDocumentFragment());
+        r || (r = Ur(t).createDocumentFragment());
         let i = r,
-            o = [];
-        return e.forEach(s => {
-            if (o.length || s.marks.length) {
+            s = [];
+        return e.forEach(o => {
+            if (s.length || o.marks.length) {
                 let l = 0,
                     a = 0;
-                for (; l < o.length && a < s.marks.length;) {
-                    let c = s.marks[a];
+                for (; l < s.length && a < o.marks.length;) {
+                    let c = o.marks[a];
                     if (!this.marks[c.type.name]) {
                         a++;
                         continue
                     }
-                    if (!c.eq(o[l][0]) || c.type.spec.spanning === !1) break;
+                    if (!c.eq(s[l][0]) || c.type.spec.spanning === !1) break;
                     l++, a++
                 }
-                for (; l < o.length;) i = o.pop()[1];
-                for (; a < s.marks.length;) {
-                    let c = s.marks[a++],
-                        u = this.serializeMark(c, s.isInline, t);
-                    u && (o.push([c, i]), i.appendChild(u.dom), i = u.contentDOM || u.dom)
+                for (; l < s.length;) i = s.pop()[1];
+                for (; a < o.marks.length;) {
+                    let c = o.marks[a++],
+                        u = this.serializeMark(c, o.isInline, t);
+                    u && (s.push([c, i]), i.appendChild(u.dom), i = u.contentDOM || u.dom)
                 }
             }
-            i.appendChild(this.serializeNodeInner(s, t))
+            i.appendChild(this.serializeNodeInner(o, t))
         }), r
     }
     serializeNodeInner(e, t) {
         let {
             dom: r,
             contentDOM: i
-        } = Se.renderSpec(ao(t), this.nodes[e.type.name](e));
+        } = ce.renderSpec(Ur(t), this.nodes[e.type.name](e));
         if (i) {
             if (e.isLeaf) throw new RangeError("Content hole not allowed in a leaf node spec");
             this.serializeFragment(e.content, t, i)
         }
         return r
     }
     serializeNode(e, t = {}) {
         let r = this.serializeNodeInner(e, t);
         for (let i = e.marks.length - 1; i >= 0; i--) {
-            let o = this.serializeMark(e.marks[i], e.isInline, t);
-            o && ((o.contentDOM || o.dom).appendChild(r), r = o.dom)
+            let s = this.serializeMark(e.marks[i], e.isInline, t);
+            s && ((s.contentDOM || s.dom).appendChild(r), r = s.dom)
         }
         return r
     }
     serializeMark(e, t, r = {}) {
         let i = this.marks[e.type.name];
-        return i && Se.renderSpec(ao(r), i(e, t))
+        return i && ce.renderSpec(Ur(r), i(e, t))
     }
     static renderSpec(e, t, r = null) {
         if (typeof t == "string") return {
             dom: e.createTextNode(t)
         };
         if (t.nodeType != null) return {
             dom: t
         };
         if (t.dom && t.dom.nodeType != null) return t;
         let i = t[0],
-            o = i.indexOf(" ");
-        o > 0 && (r = i.slice(0, o), i = i.slice(o + 1));
-        let s, l = r ? e.createElementNS(r, i) : e.createElement(i),
+            s = i.indexOf(" ");
+        s > 0 && (r = i.slice(0, s), i = i.slice(s + 1));
+        let o, l = r ? e.createElementNS(r, i) : e.createElement(i),
             a = t[1],
             c = 1;
         if (a && typeof a == "object" && a.nodeType == null && !Array.isArray(a)) {
             c = 2;
             for (let u in a)
                 if (a[u] != null) {
                     let d = u.indexOf(" ");
@@ -3234,172 +2004,172 @@
                 return {
                     dom: l,
                     contentDOM: l
                 }
             } else {
                 let {
                     dom: f,
-                    contentDOM: p
-                } = Se.renderSpec(e, d, r);
-                if (l.appendChild(f), p) {
-                    if (s) throw new RangeError("Multiple content holes");
-                    s = p
+                    contentDOM: h
+                } = ce.renderSpec(e, d, r);
+                if (l.appendChild(f), h) {
+                    if (o) throw new RangeError("Multiple content holes");
+                    o = h
                 }
             }
         }
         return {
             dom: l,
-            contentDOM: s
+            contentDOM: o
         }
     }
     static fromSchema(e) {
-        return e.cached.domSerializer || (e.cached.domSerializer = new Se(this.nodesFromSchema(e), this.marksFromSchema(e)))
+        return e.cached.domSerializer || (e.cached.domSerializer = new ce(this.nodesFromSchema(e), this.marksFromSchema(e)))
     }
     static nodesFromSchema(e) {
-        let t = jl(e.nodes);
+        let t = Gs(e.nodes);
         return t.text || (t.text = r => r.text), t
     }
     static marksFromSchema(e) {
-        return jl(e.marks)
+        return Gs(e.marks)
     }
 };
 
-function jl(n) {
+function Gs(n) {
     let e = {};
     for (let t in n) {
         let r = n[t].spec.toDOM;
         r && (e[t] = r)
     }
     return e
 }
 
-function ao(n) {
+function Ur(n) {
     return n.document || window.document
 }
-var ia = 65535,
-    oa = Math.pow(2, 16);
+var po = 65535,
+    mo = Math.pow(2, 16);
 
-function hf(n, e) {
-    return n + e * oa
+function Hc(n, e) {
+    return n + e * mo
 }
 
-function na(n) {
-    return n & ia
+function fo(n) {
+    return n & po
 }
 
-function mf(n) {
-    return (n - (n & ia)) / oa
+function Fc(n) {
+    return (n - (n & po)) / mo
 }
-var sa = 1,
-    la = 2,
-    Ur = 4,
-    aa = 8,
-    dr = class {
+var go = 1,
+    yo = 2,
+    _n = 4,
+    bo = 8,
+    hn = class {
         constructor(e, t, r) {
             this.pos = e, this.delInfo = t, this.recover = r
         }
         get deleted() {
-            return (this.delInfo & aa) > 0
+            return (this.delInfo & bo) > 0
         }
         get deletedBefore() {
-            return (this.delInfo & (sa | Ur)) > 0
+            return (this.delInfo & (go | _n)) > 0
         }
         get deletedAfter() {
-            return (this.delInfo & (la | Ur)) > 0
+            return (this.delInfo & (yo | _n)) > 0
         }
         get deletedAcross() {
-            return (this.delInfo & Ur) > 0
+            return (this.delInfo & _n) > 0
         }
     },
-    Te = class {
+    de = class {
         constructor(e, t = !1) {
-            if (this.ranges = e, this.inverted = t, !e.length && Te.empty) return Te.empty
+            if (this.ranges = e, this.inverted = t, !e.length && de.empty) return de.empty
         }
         recover(e) {
             let t = 0,
-                r = na(e);
+                r = fo(e);
             if (!this.inverted)
                 for (let i = 0; i < r; i++) t += this.ranges[i * 3 + 2] - this.ranges[i * 3 + 1];
-            return this.ranges[r * 3] + t + mf(e)
+            return this.ranges[r * 3] + t + Fc(e)
         }
         mapResult(e, t = 1) {
             return this._map(e, t, !1)
         }
         map(e, t = 1) {
             return this._map(e, t, !0)
         }
         _map(e, t, r) {
             let i = 0,
-                o = this.inverted ? 2 : 1,
-                s = this.inverted ? 1 : 2;
+                s = this.inverted ? 2 : 1,
+                o = this.inverted ? 1 : 2;
             for (let l = 0; l < this.ranges.length; l += 3) {
                 let a = this.ranges[l] - (this.inverted ? i : 0);
                 if (a > e) break;
-                let c = this.ranges[l + o],
-                    u = this.ranges[l + s],
+                let c = this.ranges[l + s],
+                    u = this.ranges[l + o],
                     d = a + c;
                 if (e <= d) {
                     let f = c ? e == a ? -1 : e == d ? 1 : t : t,
-                        p = a + i + (f < 0 ? 0 : u);
-                    if (r) return p;
-                    let h = e == (t < 0 ? a : d) ? null : hf(l / 3, e - a),
-                        m = e == a ? la : e == d ? sa : Ur;
-                    return (t < 0 ? e != a : e != d) && (m |= aa), new dr(p, m, h)
+                        h = a + i + (f < 0 ? 0 : u);
+                    if (r) return h;
+                    let p = e == (t < 0 ? a : d) ? null : Hc(l / 3, e - a),
+                        m = e == a ? yo : e == d ? go : _n;
+                    return (t < 0 ? e != a : e != d) && (m |= bo), new hn(h, m, p)
                 }
                 i += u - c
             }
-            return r ? e + i : new dr(e + i, 0, null)
+            return r ? e + i : new hn(e + i, 0, null)
         }
         touches(e, t) {
             let r = 0,
-                i = na(t),
-                o = this.inverted ? 2 : 1,
-                s = this.inverted ? 1 : 2;
+                i = fo(t),
+                s = this.inverted ? 2 : 1,
+                o = this.inverted ? 1 : 2;
             for (let l = 0; l < this.ranges.length; l += 3) {
                 let a = this.ranges[l] - (this.inverted ? r : 0);
                 if (a > e) break;
-                let c = this.ranges[l + o],
+                let c = this.ranges[l + s],
                     u = a + c;
                 if (e <= u && l == i * 3) return !0;
-                r += this.ranges[l + s] - c
+                r += this.ranges[l + o] - c
             }
             return !1
         }
         forEach(e) {
             let t = this.inverted ? 2 : 1,
                 r = this.inverted ? 1 : 2;
-            for (let i = 0, o = 0; i < this.ranges.length; i += 3) {
-                let s = this.ranges[i],
-                    l = s - (this.inverted ? o : 0),
-                    a = s + (this.inverted ? 0 : o),
+            for (let i = 0, s = 0; i < this.ranges.length; i += 3) {
+                let o = this.ranges[i],
+                    l = o - (this.inverted ? s : 0),
+                    a = o + (this.inverted ? 0 : s),
                     c = this.ranges[i + t],
                     u = this.ranges[i + r];
-                e(l, l + c, a, a + u), o += u - c
+                e(l, l + c, a, a + u), s += u - c
             }
         }
         invert() {
-            return new Te(this.ranges, !this.inverted)
+            return new de(this.ranges, !this.inverted)
         }
         toString() {
             return (this.inverted ? "-" : "") + JSON.stringify(this.ranges)
         }
         static offset(e) {
-            return e == 0 ? Te.empty : new Te(e < 0 ? [0, -e, 0] : [0, 0, e])
+            return e == 0 ? de.empty : new de(e < 0 ? [0, -e, 0] : [0, 0, e])
         }
     };
-Te.empty = new Te([]);
-var mt = class {
+de.empty = new de([]);
+var Fe = class {
         constructor(e = [], t, r = 0, i = e.length) {
             this.maps = e, this.mirror = t, this.from = r, this.to = i
         }
         slice(e = 0, t = this.maps.length) {
-            return new mt(this.maps, this.mirror, e, t)
+            return new Fe(this.maps, this.mirror, e, t)
         }
         copy() {
-            return new mt(this.maps.slice(), this.mirror && this.mirror.slice(), this.from, this.to)
+            return new Fe(this.maps.slice(), this.mirror && this.mirror.slice(), this.from, this.to)
         }
         appendMap(e, t) {
             this.to = this.maps.push(e), t != null && this.setMirror(this.maps.length - 1, t)
         }
         appendMapping(e) {
             for (let t = 0, r = this.maps.length; t < e.maps.length; t++) {
                 let i = e.getMirror(t);
@@ -3418,1068 +2188,1068 @@
         appendMappingInverted(e) {
             for (let t = e.maps.length - 1, r = this.maps.length + e.maps.length; t >= 0; t--) {
                 let i = e.getMirror(t);
                 this.appendMap(e.maps[t].invert(), i != null && i > t ? r - i - 1 : void 0)
             }
         }
         invert() {
-            let e = new mt;
+            let e = new Fe;
             return e.appendMappingInverted(this), e
         }
         map(e, t = 1) {
             if (this.mirror) return this._map(e, t, !0);
             for (let r = this.from; r < this.to; r++) e = this.maps[r].map(e, t);
             return e
         }
         mapResult(e, t = 1) {
             return this._map(e, t, !1)
         }
         _map(e, t, r) {
             let i = 0;
-            for (let o = this.from; o < this.to; o++) {
-                let s = this.maps[o],
-                    l = s.mapResult(e, t);
+            for (let s = this.from; s < this.to; s++) {
+                let o = this.maps[s],
+                    l = o.mapResult(e, t);
                 if (l.recover != null) {
-                    let a = this.getMirror(o);
-                    if (a != null && a > o && a < this.to) {
-                        o = a, e = this.maps[a].recover(l.recover);
+                    let a = this.getMirror(s);
+                    if (a != null && a > s && a < this.to) {
+                        s = a, e = this.maps[a].recover(l.recover);
                         continue
                     }
                 }
                 i |= l.delInfo, e = l.pos
             }
-            return r ? e : new dr(e, i, null)
+            return r ? e : new hn(e, i, null)
         }
     },
-    po = Object.create(null),
-    me = class {
+    Yr = Object.create(null),
+    ne = class {
         getMap() {
-            return Te.empty
+            return de.empty
         }
         merge(e) {
             return null
         }
         static fromJSON(e, t) {
             if (!t || !t.stepType) throw new RangeError("Invalid input for Step.fromJSON");
-            let r = po[t.stepType];
+            let r = Yr[t.stepType];
             if (!r) throw new RangeError(`No step type ${t.stepType} defined`);
             return r.fromJSON(e, t)
         }
         static jsonID(e, t) {
-            if (e in po) throw new RangeError("Duplicate use of step JSON ID " + e);
-            return po[e] = t, t.prototype.jsonID = e, t
+            if (e in Yr) throw new RangeError("Duplicate use of step JSON ID " + e);
+            return Yr[e] = t, t.prototype.jsonID = e, t
         }
     },
-    X = class {
+    K = class {
         constructor(e, t) {
             this.doc = e, this.failed = t
         }
         static ok(e) {
-            return new X(e, null)
+            return new K(e, null)
         }
         static fail(e) {
-            return new X(null, e)
+            return new K(null, e)
         }
         static fromReplace(e, t, r, i) {
             try {
-                return X.ok(e.replace(t, r, i))
-            } catch (o) {
-                if (o instanceof nn) return X.fail(o.message);
-                throw o
+                return K.ok(e.replace(t, r, i))
+            } catch (s) {
+                if (s instanceof mt) return K.fail(s.message);
+                throw s
             }
         }
     };
 
-function xo(n, e, t) {
+function ni(n, e, t) {
     let r = [];
     for (let i = 0; i < n.childCount; i++) {
-        let o = n.child(i);
-        o.content.size && (o = o.copy(xo(o.content, e, o))), o.isInline && (o = e(o, t, i)), r.push(o)
+        let s = n.child(i);
+        s.content.size && (s = s.copy(ni(s.content, e, s))), s.isInline && (s = e(s, t, i)), r.push(s)
     }
-    return v.fromArray(r)
+    return x.fromArray(r)
 }
-var Xe = class extends me {
+var Ce = class extends ne {
     constructor(e, t, r) {
         super(), this.from = e, this.to = t, this.mark = r
     }
     apply(e) {
         let t = e.slice(this.from, this.to),
             r = e.resolve(this.from),
             i = r.node(r.sharedDepth(this.to)),
-            o = new w(xo(t.content, (s, l) => !s.isAtom || !l.type.allowsMarkType(this.mark.type) ? s : s.mark(this.mark.addToSet(s.marks)), i), t.openStart, t.openEnd);
-        return X.fromReplace(e, this.from, this.to, o)
+            s = new E(ni(t.content, (o, l) => !o.isAtom || !l.type.allowsMarkType(this.mark.type) ? o : o.mark(this.mark.addToSet(o.marks)), i), t.openStart, t.openEnd);
+        return K.fromReplace(e, this.from, this.to, s)
     }
     invert() {
-        return new Be(this.from, this.to, this.mark)
+        return new me(this.from, this.to, this.mark)
     }
     map(e) {
         let t = e.mapResult(this.from, 1),
             r = e.mapResult(this.to, -1);
-        return t.deleted && r.deleted || t.pos >= r.pos ? null : new Xe(t.pos, r.pos, this.mark)
+        return t.deleted && r.deleted || t.pos >= r.pos ? null : new Ce(t.pos, r.pos, this.mark)
     }
     merge(e) {
-        return e instanceof Xe && e.mark.eq(this.mark) && this.from <= e.to && this.to >= e.from ? new Xe(Math.min(this.from, e.from), Math.max(this.to, e.to), this.mark) : null
+        return e instanceof Ce && e.mark.eq(this.mark) && this.from <= e.to && this.to >= e.from ? new Ce(Math.min(this.from, e.from), Math.max(this.to, e.to), this.mark) : null
     }
     toJSON() {
         return {
             stepType: "addMark",
             mark: this.mark.toJSON(),
             from: this.from,
             to: this.to
         }
     }
     static fromJSON(e, t) {
         if (typeof t.from != "number" || typeof t.to != "number") throw new RangeError("Invalid input for AddMarkStep.fromJSON");
-        return new Xe(t.from, t.to, e.markFromJSON(t.mark))
+        return new Ce(t.from, t.to, e.markFromJSON(t.mark))
     }
 };
-me.jsonID("addMark", Xe);
-var Be = class extends me {
+ne.jsonID("addMark", Ce);
+var me = class extends ne {
     constructor(e, t, r) {
         super(), this.from = e, this.to = t, this.mark = r
     }
     apply(e) {
         let t = e.slice(this.from, this.to),
-            r = new w(xo(t.content, i => i.mark(this.mark.removeFromSet(i.marks)), e), t.openStart, t.openEnd);
-        return X.fromReplace(e, this.from, this.to, r)
+            r = new E(ni(t.content, i => i.mark(this.mark.removeFromSet(i.marks)), e), t.openStart, t.openEnd);
+        return K.fromReplace(e, this.from, this.to, r)
     }
     invert() {
-        return new Xe(this.from, this.to, this.mark)
+        return new Ce(this.from, this.to, this.mark)
     }
     map(e) {
         let t = e.mapResult(this.from, 1),
             r = e.mapResult(this.to, -1);
-        return t.deleted && r.deleted || t.pos >= r.pos ? null : new Be(t.pos, r.pos, this.mark)
+        return t.deleted && r.deleted || t.pos >= r.pos ? null : new me(t.pos, r.pos, this.mark)
     }
     merge(e) {
-        return e instanceof Be && e.mark.eq(this.mark) && this.from <= e.to && this.to >= e.from ? new Be(Math.min(this.from, e.from), Math.max(this.to, e.to), this.mark) : null
+        return e instanceof me && e.mark.eq(this.mark) && this.from <= e.to && this.to >= e.from ? new me(Math.min(this.from, e.from), Math.max(this.to, e.to), this.mark) : null
     }
     toJSON() {
         return {
             stepType: "removeMark",
             mark: this.mark.toJSON(),
             from: this.from,
             to: this.to
         }
     }
     static fromJSON(e, t) {
         if (typeof t.from != "number" || typeof t.to != "number") throw new RangeError("Invalid input for RemoveMarkStep.fromJSON");
-        return new Be(t.from, t.to, e.markFromJSON(t.mark))
+        return new me(t.from, t.to, e.markFromJSON(t.mark))
     }
 };
-me.jsonID("removeMark", Be);
-var Ze = class extends me {
+ne.jsonID("removeMark", me);
+var Ae = class extends ne {
     constructor(e, t) {
         super(), this.pos = e, this.mark = t
     }
     apply(e) {
         let t = e.nodeAt(this.pos);
-        if (!t) return X.fail("No node at mark step's position");
+        if (!t) return K.fail("No node at mark step's position");
         let r = t.type.create(t.attrs, null, this.mark.addToSet(t.marks));
-        return X.fromReplace(e, this.pos, this.pos + 1, new w(v.from(r), 0, t.isLeaf ? 0 : 1))
+        return K.fromReplace(e, this.pos, this.pos + 1, new E(x.from(r), 0, t.isLeaf ? 0 : 1))
     }
     invert(e) {
         let t = e.nodeAt(this.pos);
         if (t) {
             let r = this.mark.addToSet(t.marks);
             if (r.length == t.marks.length) {
                 for (let i = 0; i < t.marks.length; i++)
-                    if (!t.marks[i].isInSet(r)) return new Ze(this.pos, t.marks[i]);
-                return new Ze(this.pos, this.mark)
+                    if (!t.marks[i].isInSet(r)) return new Ae(this.pos, t.marks[i]);
+                return new Ae(this.pos, this.mark)
             }
         }
-        return new At(this.pos, this.mark)
+        return new Ge(this.pos, this.mark)
     }
     map(e) {
         let t = e.mapResult(this.pos, 1);
-        return t.deletedAfter ? null : new Ze(t.pos, this.mark)
+        return t.deletedAfter ? null : new Ae(t.pos, this.mark)
     }
     toJSON() {
         return {
             stepType: "addNodeMark",
             pos: this.pos,
             mark: this.mark.toJSON()
         }
     }
     static fromJSON(e, t) {
         if (typeof t.pos != "number") throw new RangeError("Invalid input for AddNodeMarkStep.fromJSON");
-        return new Ze(t.pos, e.markFromJSON(t.mark))
+        return new Ae(t.pos, e.markFromJSON(t.mark))
     }
 };
-me.jsonID("addNodeMark", Ze);
-var At = class extends me {
+ne.jsonID("addNodeMark", Ae);
+var Ge = class extends ne {
     constructor(e, t) {
         super(), this.pos = e, this.mark = t
     }
     apply(e) {
         let t = e.nodeAt(this.pos);
-        if (!t) return X.fail("No node at mark step's position");
+        if (!t) return K.fail("No node at mark step's position");
         let r = t.type.create(t.attrs, null, this.mark.removeFromSet(t.marks));
-        return X.fromReplace(e, this.pos, this.pos + 1, new w(v.from(r), 0, t.isLeaf ? 0 : 1))
+        return K.fromReplace(e, this.pos, this.pos + 1, new E(x.from(r), 0, t.isLeaf ? 0 : 1))
     }
     invert(e) {
         let t = e.nodeAt(this.pos);
-        return !t || !this.mark.isInSet(t.marks) ? this : new Ze(this.pos, this.mark)
+        return !t || !this.mark.isInSet(t.marks) ? this : new Ae(this.pos, this.mark)
     }
     map(e) {
         let t = e.mapResult(this.pos, 1);
-        return t.deletedAfter ? null : new At(t.pos, this.mark)
+        return t.deletedAfter ? null : new Ge(t.pos, this.mark)
     }
     toJSON() {
         return {
             stepType: "removeNodeMark",
             pos: this.pos,
             mark: this.mark.toJSON()
         }
     }
     static fromJSON(e, t) {
         if (typeof t.pos != "number") throw new RangeError("Invalid input for RemoveNodeMarkStep.fromJSON");
-        return new At(t.pos, e.markFromJSON(t.mark))
+        return new Ge(t.pos, e.markFromJSON(t.mark))
     }
 };
-me.jsonID("removeNodeMark", At);
-var Q = class extends me {
+ne.jsonID("removeNodeMark", Ge);
+var q = class extends ne {
     constructor(e, t, r, i = !1) {
         super(), this.from = e, this.to = t, this.slice = r, this.structure = i
     }
     apply(e) {
-        return this.structure && go(e, this.from, this.to) ? X.fail("Structure replace would overwrite content") : X.fromReplace(e, this.from, this.to, this.slice)
+        return this.structure && ei(e, this.from, this.to) ? K.fail("Structure replace would overwrite content") : K.fromReplace(e, this.from, this.to, this.slice)
     }
     getMap() {
-        return new Te([this.from, this.to - this.from, this.slice.size])
+        return new de([this.from, this.to - this.from, this.slice.size])
     }
     invert(e) {
-        return new Q(this.from, this.from + this.slice.size, e.slice(this.from, this.to))
+        return new q(this.from, this.from + this.slice.size, e.slice(this.from, this.to))
     }
     map(e) {
         let t = e.mapResult(this.from, 1),
             r = e.mapResult(this.to, -1);
-        return t.deletedAcross && r.deletedAcross ? null : new Q(t.pos, Math.max(t.pos, r.pos), this.slice)
+        return t.deletedAcross && r.deletedAcross ? null : new q(t.pos, Math.max(t.pos, r.pos), this.slice)
     }
     merge(e) {
-        if (!(e instanceof Q) || e.structure || this.structure) return null;
+        if (!(e instanceof q) || e.structure || this.structure) return null;
         if (this.from + this.slice.size == e.from && !this.slice.openEnd && !e.slice.openStart) {
-            let t = this.slice.size + e.slice.size == 0 ? w.empty : new w(this.slice.content.append(e.slice.content), this.slice.openStart, e.slice.openEnd);
-            return new Q(this.from, this.to + (e.to - e.from), t, this.structure)
+            let t = this.slice.size + e.slice.size == 0 ? E.empty : new E(this.slice.content.append(e.slice.content), this.slice.openStart, e.slice.openEnd);
+            return new q(this.from, this.to + (e.to - e.from), t, this.structure)
         } else if (e.to == this.from && !this.slice.openStart && !e.slice.openEnd) {
-            let t = this.slice.size + e.slice.size == 0 ? w.empty : new w(e.slice.content.append(this.slice.content), e.slice.openStart, this.slice.openEnd);
-            return new Q(e.from, this.to, t, this.structure)
+            let t = this.slice.size + e.slice.size == 0 ? E.empty : new E(e.slice.content.append(this.slice.content), e.slice.openStart, this.slice.openEnd);
+            return new q(e.from, this.to, t, this.structure)
         } else return null
     }
     toJSON() {
         let e = {
             stepType: "replace",
             from: this.from,
             to: this.to
         };
         return this.slice.size && (e.slice = this.slice.toJSON()), this.structure && (e.structure = !0), e
     }
     static fromJSON(e, t) {
         if (typeof t.from != "number" || typeof t.to != "number") throw new RangeError("Invalid input for ReplaceStep.fromJSON");
-        return new Q(t.from, t.to, w.fromJSON(e, t.slice), !!t.structure)
+        return new q(t.from, t.to, E.fromJSON(e, t.slice), !!t.structure)
     }
 };
-me.jsonID("replace", Q);
-var W = class extends me {
-    constructor(e, t, r, i, o, s, l = !1) {
-        super(), this.from = e, this.to = t, this.gapFrom = r, this.gapTo = i, this.slice = o, this.insert = s, this.structure = l
+ne.jsonID("replace", q);
+var j = class extends ne {
+    constructor(e, t, r, i, s, o, l = !1) {
+        super(), this.from = e, this.to = t, this.gapFrom = r, this.gapTo = i, this.slice = s, this.insert = o, this.structure = l
     }
     apply(e) {
-        if (this.structure && (go(e, this.from, this.gapFrom) || go(e, this.gapTo, this.to))) return X.fail("Structure gap-replace would overwrite content");
+        if (this.structure && (ei(e, this.from, this.gapFrom) || ei(e, this.gapTo, this.to))) return K.fail("Structure gap-replace would overwrite content");
         let t = e.slice(this.gapFrom, this.gapTo);
-        if (t.openStart || t.openEnd) return X.fail("Gap is not a flat range");
+        if (t.openStart || t.openEnd) return K.fail("Gap is not a flat range");
         let r = this.slice.insertAt(this.insert, t.content);
-        return r ? X.fromReplace(e, this.from, this.to, r) : X.fail("Content does not fit in gap")
+        return r ? K.fromReplace(e, this.from, this.to, r) : K.fail("Content does not fit in gap")
     }
     getMap() {
-        return new Te([this.from, this.gapFrom - this.from, this.insert, this.gapTo, this.to - this.gapTo, this.slice.size - this.insert])
+        return new de([this.from, this.gapFrom - this.from, this.insert, this.gapTo, this.to - this.gapTo, this.slice.size - this.insert])
     }
     invert(e) {
         let t = this.gapTo - this.gapFrom;
-        return new W(this.from, this.from + this.slice.size + t, this.from + this.insert, this.from + this.insert + t, e.slice(this.from, this.to).removeBetween(this.gapFrom - this.from, this.gapTo - this.from), this.gapFrom - this.from, this.structure)
+        return new j(this.from, this.from + this.slice.size + t, this.from + this.insert, this.from + this.insert + t, e.slice(this.from, this.to).removeBetween(this.gapFrom - this.from, this.gapTo - this.from), this.gapFrom - this.from, this.structure)
     }
     map(e) {
         let t = e.mapResult(this.from, 1),
             r = e.mapResult(this.to, -1),
             i = e.map(this.gapFrom, -1),
-            o = e.map(this.gapTo, 1);
-        return t.deletedAcross && r.deletedAcross || i < t.pos || o > r.pos ? null : new W(t.pos, r.pos, i, o, this.slice, this.insert, this.structure)
+            s = e.map(this.gapTo, 1);
+        return t.deletedAcross && r.deletedAcross || i < t.pos || s > r.pos ? null : new j(t.pos, r.pos, i, s, this.slice, this.insert, this.structure)
     }
     toJSON() {
         let e = {
             stepType: "replaceAround",
             from: this.from,
             to: this.to,
             gapFrom: this.gapFrom,
             gapTo: this.gapTo,
             insert: this.insert
         };
         return this.slice.size && (e.slice = this.slice.toJSON()), this.structure && (e.structure = !0), e
     }
     static fromJSON(e, t) {
         if (typeof t.from != "number" || typeof t.to != "number" || typeof t.gapFrom != "number" || typeof t.gapTo != "number" || typeof t.insert != "number") throw new RangeError("Invalid input for ReplaceAroundStep.fromJSON");
-        return new W(t.from, t.to, t.gapFrom, t.gapTo, w.fromJSON(e, t.slice), t.insert, !!t.structure)
+        return new j(t.from, t.to, t.gapFrom, t.gapTo, E.fromJSON(e, t.slice), t.insert, !!t.structure)
     }
 };
-me.jsonID("replaceAround", W);
+ne.jsonID("replaceAround", j);
 
-function go(n, e, t) {
+function ei(n, e, t) {
     let r = n.resolve(e),
         i = t - e,
-        o = r.depth;
-    for (; i > 0 && o > 0 && r.indexAfter(o) == r.node(o).childCount;) o--, i--;
+        s = r.depth;
+    for (; i > 0 && s > 0 && r.indexAfter(s) == r.node(s).childCount;) s--, i--;
     if (i > 0) {
-        let s = r.node(o).maybeChild(r.indexAfter(o));
+        let o = r.node(s).maybeChild(r.indexAfter(s));
         for (; i > 0;) {
-            if (!s || s.isLeaf) return !0;
-            s = s.firstChild, i--
+            if (!o || o.isLeaf) return !0;
+            o = o.firstChild, i--
         }
     }
     return !1
 }
 
-function gf(n, e, t, r) {
+function jc(n, e, t, r) {
     let i = [],
-        o = [],
-        s, l;
+        s = [],
+        o, l;
     n.doc.nodesBetween(e, t, (a, c, u) => {
         if (!a.isInline) return;
         let d = a.marks;
         if (!r.isInSet(d) && u.type.allowsMarkType(r.type)) {
             let f = Math.max(c, e),
-                p = Math.min(c + a.nodeSize, t),
-                h = r.addToSet(d);
-            for (let m = 0; m < d.length; m++) d[m].isInSet(h) || (s && s.to == f && s.mark.eq(d[m]) ? s.to = p : i.push(s = new Be(f, p, d[m])));
-            l && l.to == f ? l.to = p : o.push(l = new Xe(f, p, r))
+                h = Math.min(c + a.nodeSize, t),
+                p = r.addToSet(d);
+            for (let m = 0; m < d.length; m++) d[m].isInSet(p) || (o && o.to == f && o.mark.eq(d[m]) ? o.to = h : i.push(o = new me(f, h, d[m])));
+            l && l.to == f ? l.to = h : s.push(l = new Ce(f, h, r))
         }
-    }), i.forEach(a => n.step(a)), o.forEach(a => n.step(a))
+    }), i.forEach(a => n.step(a)), s.forEach(a => n.step(a))
 }
 
-function yf(n, e, t, r) {
+function $c(n, e, t, r) {
     let i = [],
-        o = 0;
-    n.doc.nodesBetween(e, t, (s, l) => {
-        if (!s.isInline) return;
-        o++;
+        s = 0;
+    n.doc.nodesBetween(e, t, (o, l) => {
+        if (!o.isInline) return;
+        s++;
         let a = null;
-        if (r instanceof sn) {
-            let c = s.marks,
+        if (r instanceof bt) {
+            let c = o.marks,
                 u;
             for (; u = r.isInSet(c);)(a || (a = [])).push(u), c = u.removeFromSet(c)
-        } else r ? r.isInSet(s.marks) && (a = [r]) : a = s.marks;
+        } else r ? r.isInSet(o.marks) && (a = [r]) : a = o.marks;
         if (a && a.length) {
-            let c = Math.min(l + s.nodeSize, t);
+            let c = Math.min(l + o.nodeSize, t);
             for (let u = 0; u < a.length; u++) {
                 let d = a[u],
                     f;
-                for (let p = 0; p < i.length; p++) {
-                    let h = i[p];
-                    h.step == o - 1 && d.eq(i[p].style) && (f = h)
+                for (let h = 0; h < i.length; h++) {
+                    let p = i[h];
+                    p.step == s - 1 && d.eq(i[h].style) && (f = p)
                 }
-                f ? (f.to = c, f.step = o) : i.push({
+                f ? (f.to = c, f.step = s) : i.push({
                     style: d,
                     from: Math.max(l, e),
                     to: c,
-                    step: o
+                    step: s
                 })
             }
         }
-    }), i.forEach(s => n.step(new Be(s.from, s.to, s.style)))
+    }), i.forEach(o => n.step(new me(o.from, o.to, o.style)))
 }
 
-function xf(n, e, t, r = t.contentMatch) {
+function Vc(n, e, t, r = t.contentMatch) {
     let i = n.doc.nodeAt(e),
-        o = [],
-        s = e + 1;
+        s = [],
+        o = e + 1;
     for (let l = 0; l < i.childCount; l++) {
         let a = i.child(l),
-            c = s + a.nodeSize,
+            c = o + a.nodeSize,
             u = r.matchType(a.type);
-        if (!u) o.push(new Q(s, c, w.empty));
+        if (!u) s.push(new q(o, c, E.empty));
         else {
             r = u;
-            for (let d = 0; d < a.marks.length; d++) t.allowsMarkType(a.marks[d].type) || n.step(new Be(s, c, a.marks[d]))
+            for (let d = 0; d < a.marks.length; d++) t.allowsMarkType(a.marks[d].type) || n.step(new me(o, c, a.marks[d]))
         }
-        s = c
+        o = c
     }
     if (!r.validEnd) {
-        let l = r.fillBefore(v.empty, !0);
-        n.replace(s, s, new w(l, 0, 0))
+        let l = r.fillBefore(x.empty, !0);
+        n.replace(o, o, new E(l, 0, 0))
     }
-    for (let l = o.length - 1; l >= 0; l--) n.step(o[l])
+    for (let l = s.length - 1; l >= 0; l--) n.step(s[l])
 }
 
-function bf(n, e, t) {
+function Jc(n, e, t) {
     return (e == 0 || n.canReplace(e, n.childCount)) && (t == n.childCount || n.canReplace(0, t))
 }
 
-function gt(n) {
+function je(n) {
     let t = n.parent.content.cutByIndex(n.startIndex, n.endIndex);
     for (let r = n.depth;; --r) {
         let i = n.$from.node(r),
-            o = n.$from.index(r),
-            s = n.$to.indexAfter(r);
-        if (r < n.depth && i.canReplace(o, s, t)) return r;
-        if (r == 0 || i.type.spec.isolating || !bf(i, o, s)) break
+            s = n.$from.index(r),
+            o = n.$to.indexAfter(r);
+        if (r < n.depth && i.canReplace(s, o, t)) return r;
+        if (r == 0 || i.type.spec.isolating || !Jc(i, s, o)) break
     }
     return null
 }
 
-function kf(n, e, t) {
+function Wc(n, e, t) {
     let {
         $from: r,
         $to: i,
-        depth: o
-    } = e, s = r.before(o + 1), l = i.after(o + 1), a = s, c = l, u = v.empty, d = 0;
-    for (let h = o, m = !1; h > t; h--) m || r.index(h) > 0 ? (m = !0, u = v.from(r.node(h).copy(u)), d++) : a--;
-    let f = v.empty,
-        p = 0;
-    for (let h = o, m = !1; h > t; h--) m || i.after(h + 1) < i.end(h) ? (m = !0, f = v.from(i.node(h).copy(f)), p++) : c++;
-    n.step(new W(a, c, s, l, new w(u.append(f), d, p), u.size - d, !0))
+        depth: s
+    } = e, o = r.before(s + 1), l = i.after(s + 1), a = o, c = l, u = x.empty, d = 0;
+    for (let p = s, m = !1; p > t; p--) m || r.index(p) > 0 ? (m = !0, u = x.from(r.node(p).copy(u)), d++) : a--;
+    let f = x.empty,
+        h = 0;
+    for (let p = s, m = !1; p > t; p--) m || i.after(p + 1) < i.end(p) ? (m = !0, f = x.from(i.node(p).copy(f)), h++) : c++;
+    n.step(new j(a, c, o, l, new E(u.append(f), d, h), u.size - d, !0))
 }
 
-function Dn(n, e, t = null, r = n) {
-    let i = vf(n, e),
-        o = i && Mf(r, e);
-    return o ? i.map(ra).concat({
+function Ft(n, e, t = null, r = n) {
+    let i = qc(n, e),
+        s = i && Kc(r, e);
+    return s ? i.map(ho).concat({
         type: e,
         attrs: t
-    }).concat(o.map(ra)) : null
+    }).concat(s.map(ho)) : null
 }
 
-function ra(n) {
+function ho(n) {
     return {
         type: n,
         attrs: null
     }
 }
 
-function vf(n, e) {
+function qc(n, e) {
     let {
         parent: t,
         startIndex: r,
         endIndex: i
-    } = n, o = t.contentMatchAt(r).findWrapping(e);
-    if (!o) return null;
-    let s = o.length ? o[0] : e;
-    return t.canReplaceWith(r, i, s) ? o : null
+    } = n, s = t.contentMatchAt(r).findWrapping(e);
+    if (!s) return null;
+    let o = s.length ? s[0] : e;
+    return t.canReplaceWith(r, i, o) ? s : null
 }
 
-function Mf(n, e) {
+function Kc(n, e) {
     let {
         parent: t,
         startIndex: r,
         endIndex: i
-    } = n, o = t.child(r), s = e.contentMatch.findWrapping(o.type);
-    if (!s) return null;
-    let a = (s.length ? s[s.length - 1] : e).contentMatch;
+    } = n, s = t.child(r), o = e.contentMatch.findWrapping(s.type);
+    if (!o) return null;
+    let a = (o.length ? o[o.length - 1] : e).contentMatch;
     for (let c = r; a && c < i; c++) a = a.matchType(t.child(c).type);
-    return !a || !a.validEnd ? null : s
+    return !a || !a.validEnd ? null : o
 }
 
-function Ef(n, e, t) {
-    let r = v.empty;
-    for (let s = t.length - 1; s >= 0; s--) {
+function Uc(n, e, t) {
+    let r = x.empty;
+    for (let o = t.length - 1; o >= 0; o--) {
         if (r.size) {
-            let l = t[s].type.contentMatch.matchFragment(r);
+            let l = t[o].type.contentMatch.matchFragment(r);
             if (!l || !l.validEnd) throw new RangeError("Wrapper type given to Transform.wrap does not form valid content of its parent wrapper")
         }
-        r = v.from(t[s].type.create(t[s].attrs, r))
+        r = x.from(t[o].type.create(t[o].attrs, r))
     }
     let i = e.start,
-        o = e.end;
-    n.step(new W(i, o, i, o, new w(r, 0, 0), t.length, !0))
+        s = e.end;
+    n.step(new j(i, s, i, s, new E(r, 0, 0), t.length, !0))
 }
 
-function Sf(n, e, t, r, i) {
+function _c(n, e, t, r, i) {
     if (!r.isTextblock) throw new RangeError("Type given to setBlockType should be a textblock");
-    let o = n.steps.length;
-    n.doc.nodesBetween(e, t, (s, l) => {
-        if (s.isTextblock && !s.hasMarkup(r, i) && wf(n.doc, n.mapping.slice(o).map(l), r)) {
-            n.clearIncompatible(n.mapping.slice(o).map(l, 1), r);
-            let a = n.mapping.slice(o),
+    let s = n.steps.length;
+    n.doc.nodesBetween(e, t, (o, l) => {
+        if (o.isTextblock && !o.hasMarkup(r, i) && Gc(n.doc, n.mapping.slice(s).map(l), r)) {
+            n.clearIncompatible(n.mapping.slice(s).map(l, 1), r);
+            let a = n.mapping.slice(s),
                 c = a.map(l, 1),
-                u = a.map(l + s.nodeSize, 1);
-            return n.step(new W(c, u, c + 1, u - 1, new w(v.from(r.create(i, null, s.marks)), 0, 0), 1, !0)), !1
+                u = a.map(l + o.nodeSize, 1);
+            return n.step(new j(c, u, c + 1, u - 1, new E(x.from(r.create(i, null, o.marks)), 0, 0), 1, !0)), !1
         }
     })
 }
 
-function wf(n, e, t) {
+function Gc(n, e, t) {
     let r = n.resolve(e),
         i = r.index();
     return r.parent.canReplaceWith(i, i + 1, t)
 }
 
-function Tf(n, e, t, r, i) {
-    let o = n.doc.nodeAt(e);
-    if (!o) throw new RangeError("No node at given position");
-    t || (t = o.type);
-    let s = t.create(r, null, i || o.marks);
-    if (o.isLeaf) return n.replaceWith(e, e + o.nodeSize, s);
-    if (!t.validContent(o.content)) throw new RangeError("Invalid content for node type " + t.name);
-    n.step(new W(e, e + o.nodeSize, e + 1, e + o.nodeSize - 1, new w(v.from(s), 0, 0), 1, !0))
+function Qc(n, e, t, r, i) {
+    let s = n.doc.nodeAt(e);
+    if (!s) throw new RangeError("No node at given position");
+    t || (t = s.type);
+    let o = t.create(r, null, i || s.marks);
+    if (s.isLeaf) return n.replaceWith(e, e + s.nodeSize, o);
+    if (!t.validContent(s.content)) throw new RangeError("Invalid content for node type " + t.name);
+    n.step(new j(e, e + s.nodeSize, e + 1, e + s.nodeSize - 1, new E(x.from(o), 0, 0), 1, !0))
 }
 
-function ze(n, e, t = 1, r) {
+function ge(n, e, t = 1, r) {
     let i = n.resolve(e),
-        o = i.depth - t,
-        s = r && r[r.length - 1] || i.parent;
-    if (o < 0 || i.parent.type.spec.isolating || !i.parent.canReplace(i.index(), i.parent.childCount) || !s.type.validContent(i.parent.content.cutByIndex(i.index(), i.parent.childCount))) return !1;
-    for (let c = i.depth - 1, u = t - 2; c > o; c--, u--) {
+        s = i.depth - t,
+        o = r && r[r.length - 1] || i.parent;
+    if (s < 0 || i.parent.type.spec.isolating || !i.parent.canReplace(i.index(), i.parent.childCount) || !o.type.validContent(i.parent.content.cutByIndex(i.index(), i.parent.childCount))) return !1;
+    for (let c = i.depth - 1, u = t - 2; c > s; c--, u--) {
         let d = i.node(c),
             f = i.index(c);
         if (d.type.spec.isolating) return !1;
-        let p = d.content.cutByIndex(f, d.childCount),
-            h = r && r[u] || d;
-        if (h != d && (p = p.replaceChild(0, h.type.create(h.attrs))), !d.canReplace(f + 1, d.childCount) || !h.type.validContent(p)) return !1
+        let h = d.content.cutByIndex(f, d.childCount),
+            p = r && r[u] || d;
+        if (p != d && (h = h.replaceChild(0, p.type.create(p.attrs))), !d.canReplace(f + 1, d.childCount) || !p.type.validContent(h)) return !1
     }
-    let l = i.indexAfter(o),
+    let l = i.indexAfter(s),
         a = r && r[0];
-    return i.node(o).canReplaceWith(l, l, a ? a.type : i.node(o + 1).type)
+    return i.node(s).canReplaceWith(l, l, a ? a.type : i.node(s + 1).type)
 }
 
-function Cf(n, e, t = 1, r) {
+function Yc(n, e, t = 1, r) {
     let i = n.doc.resolve(e),
-        o = v.empty,
-        s = v.empty;
+        s = x.empty,
+        o = x.empty;
     for (let l = i.depth, a = i.depth - t, c = t - 1; l > a; l--, c--) {
-        o = v.from(i.node(l).copy(o));
+        s = x.from(i.node(l).copy(s));
         let u = r && r[c];
-        s = v.from(u ? u.type.create(u.attrs, s) : i.node(l).copy(s))
+        o = x.from(u ? u.type.create(u.attrs, o) : i.node(l).copy(o))
     }
-    n.step(new Q(e, e, new w(o.append(s), t, t), !0))
+    n.step(new q(e, e, new E(s.append(o), t, t), !0))
 }
 
-function Ke(n, e) {
+function Se(n, e) {
     let t = n.resolve(e),
         r = t.index();
-    return ca(t.nodeBefore, t.nodeAfter) && t.parent.canReplace(r, r + 1)
+    return xo(t.nodeBefore, t.nodeAfter) && t.parent.canReplace(r, r + 1)
 }
 
-function ca(n, e) {
+function xo(n, e) {
     return !!(n && e && !n.isLeaf && n.canAppend(e))
 }
 
-function bo(n, e, t = -1) {
+function ri(n, e, t = -1) {
     let r = n.resolve(e);
     for (let i = r.depth;; i--) {
-        let o, s, l = r.index(i);
-        if (i == r.depth ? (o = r.nodeBefore, s = r.nodeAfter) : t > 0 ? (o = r.node(i + 1), l++, s = r.node(i).maybeChild(l)) : (o = r.node(i).maybeChild(l - 1), s = r.node(i + 1)), o && !o.isTextblock && ca(o, s) && r.node(i).canReplace(l, l + 1)) return e;
+        let s, o, l = r.index(i);
+        if (i == r.depth ? (s = r.nodeBefore, o = r.nodeAfter) : t > 0 ? (s = r.node(i + 1), l++, o = r.node(i).maybeChild(l)) : (s = r.node(i).maybeChild(l - 1), o = r.node(i + 1)), s && !s.isTextblock && xo(s, o) && r.node(i).canReplace(l, l + 1)) return e;
         if (i == 0) break;
         e = t < 0 ? r.before(i) : r.after(i)
     }
 }
 
-function Of(n, e, t) {
-    let r = new Q(e - t, e + t, w.empty, !0);
+function Xc(n, e, t) {
+    let r = new q(e - t, e + t, E.empty, !0);
     n.step(r)
 }
 
-function Af(n, e, t) {
+function Zc(n, e, t) {
     let r = n.resolve(e);
     if (r.parent.canReplaceWith(r.index(), r.index(), t)) return e;
     if (r.parentOffset == 0)
         for (let i = r.depth - 1; i >= 0; i--) {
-            let o = r.index(i);
-            if (r.node(i).canReplaceWith(o, o, t)) return r.before(i + 1);
-            if (o > 0) return null
+            let s = r.index(i);
+            if (r.node(i).canReplaceWith(s, s, t)) return r.before(i + 1);
+            if (s > 0) return null
         }
     if (r.parentOffset == r.parent.content.size)
         for (let i = r.depth - 1; i >= 0; i--) {
-            let o = r.indexAfter(i);
-            if (r.node(i).canReplaceWith(o, o, t)) return r.after(i + 1);
-            if (o < r.node(i).childCount) return null
+            let s = r.indexAfter(i);
+            if (r.node(i).canReplaceWith(s, s, t)) return r.after(i + 1);
+            if (s < r.node(i).childCount) return null
         }
     return null
 }
 
-function ua(n, e, t) {
+function ko(n, e, t) {
     let r = n.resolve(e);
     if (!t.content.size) return e;
     let i = t.content;
-    for (let o = 0; o < t.openStart; o++) i = i.firstChild.content;
-    for (let o = 1; o <= (t.openStart == 0 && t.size ? 2 : 1); o++)
-        for (let s = r.depth; s >= 0; s--) {
-            let l = s == r.depth ? 0 : r.pos <= (r.start(s + 1) + r.end(s + 1)) / 2 ? -1 : 1,
-                a = r.index(s) + (l > 0 ? 1 : 0),
-                c = r.node(s),
+    for (let s = 0; s < t.openStart; s++) i = i.firstChild.content;
+    for (let s = 1; s <= (t.openStart == 0 && t.size ? 2 : 1); s++)
+        for (let o = r.depth; o >= 0; o--) {
+            let l = o == r.depth ? 0 : r.pos <= (r.start(o + 1) + r.end(o + 1)) / 2 ? -1 : 1,
+                a = r.index(o) + (l > 0 ? 1 : 0),
+                c = r.node(o),
                 u = !1;
-            if (o == 1) u = c.canReplace(a, a, i);
+            if (s == 1) u = c.canReplace(a, a, i);
             else {
                 let d = c.contentMatchAt(a).findWrapping(i.firstChild.type);
                 u = d && c.canReplaceWith(a, a, d[0])
             }
-            if (u) return l == 0 ? r.pos : l < 0 ? r.before(s + 1) : r.after(s + 1)
+            if (u) return l == 0 ? r.pos : l < 0 ? r.before(o + 1) : r.after(o + 1)
         }
     return null
 }
 
-function _r(n, e, t = e, r = w.empty) {
+function Gn(n, e, t = e, r = E.empty) {
     if (e == t && !r.size) return null;
     let i = n.resolve(e),
-        o = n.resolve(t);
-    return da(i, o, r) ? new Q(e, t, r) : new yo(i, o, r).fit()
+        s = n.resolve(t);
+    return Mo(i, s, r) ? new q(e, t, r) : new ti(i, s, r).fit()
 }
 
-function da(n, e, t) {
+function Mo(n, e, t) {
     return !t.openStart && !t.openEnd && n.start() == e.start() && n.parent.canReplace(n.index(), e.index(), t.content)
 }
-var yo = class {
+var ti = class {
     constructor(e, t, r) {
-        this.$from = e, this.$to = t, this.unplaced = r, this.frontier = [], this.placed = v.empty;
+        this.$from = e, this.$to = t, this.unplaced = r, this.frontier = [], this.placed = x.empty;
         for (let i = 0; i <= e.depth; i++) {
-            let o = e.node(i);
+            let s = e.node(i);
             this.frontier.push({
-                type: o.type,
-                match: o.contentMatchAt(e.indexAfter(i))
+                type: s.type,
+                match: s.contentMatchAt(e.indexAfter(i))
             })
         }
-        for (let i = e.depth; i > 0; i--) this.placed = v.from(e.node(i).copy(this.placed))
+        for (let i = e.depth; i > 0; i--) this.placed = x.from(e.node(i).copy(this.placed))
     }
     get depth() {
         return this.frontier.length - 1
     }
     fit() {
         for (; this.unplaced.size;) {
             let c = this.findFittable();
             c ? this.placeNodes(c) : this.openMore() || this.dropNode()
         }
         let e = this.mustMoveInline(),
             t = this.placed.size - this.depth - this.$from.depth,
             r = this.$from,
             i = this.close(e < 0 ? this.$to : r.doc.resolve(e));
         if (!i) return null;
-        let o = this.placed,
-            s = r.depth,
+        let s = this.placed,
+            o = r.depth,
             l = i.depth;
-        for (; s && l && o.childCount == 1;) o = o.firstChild.content, s--, l--;
-        let a = new w(o, s, l);
-        return e > -1 ? new W(r.pos, e, this.$to.pos, this.$to.end(), a, t) : a.size || r.pos != this.$to.pos ? new Q(r.pos, i.pos, a) : null
+        for (; o && l && s.childCount == 1;) s = s.firstChild.content, o--, l--;
+        let a = new E(s, o, l);
+        return e > -1 ? new j(r.pos, e, this.$to.pos, this.$to.end(), a, t) : a.size || r.pos != this.$to.pos ? new q(r.pos, i.pos, a) : null
     }
     findFittable() {
         let e = this.unplaced.openStart;
         for (let t = this.unplaced.content, r = 0, i = this.unplaced.openEnd; r < e; r++) {
-            let o = t.firstChild;
-            if (t.childCount > 1 && (i = 0), o.type.spec.isolating && i <= r) {
+            let s = t.firstChild;
+            if (t.childCount > 1 && (i = 0), s.type.spec.isolating && i <= r) {
                 e = r;
                 break
             }
-            t = o.content
+            t = s.content
         }
         for (let t = 1; t <= 2; t++)
             for (let r = t == 1 ? e : this.unplaced.openStart; r >= 0; r--) {
-                let i, o = null;
-                r ? (o = ho(this.unplaced.content, r - 1).firstChild, i = o.content) : i = this.unplaced.content;
-                let s = i.firstChild;
+                let i, s = null;
+                r ? (s = Xr(this.unplaced.content, r - 1).firstChild, i = s.content) : i = this.unplaced.content;
+                let o = i.firstChild;
                 for (let l = this.depth; l >= 0; l--) {
                     let {
                         type: a,
                         match: c
                     } = this.frontier[l], u, d = null;
-                    if (t == 1 && (s ? c.matchType(s.type) || (d = c.fillBefore(v.from(s), !1)) : o && a.compatibleContent(o.type))) return {
+                    if (t == 1 && (o ? c.matchType(o.type) || (d = c.fillBefore(x.from(o), !1)) : s && a.compatibleContent(s.type))) return {
                         sliceDepth: r,
                         frontierDepth: l,
-                        parent: o,
+                        parent: s,
                         inject: d
                     };
-                    if (t == 2 && s && (u = c.findWrapping(s.type))) return {
+                    if (t == 2 && o && (u = c.findWrapping(o.type))) return {
                         sliceDepth: r,
                         frontierDepth: l,
-                        parent: o,
+                        parent: s,
                         wrap: u
                     };
-                    if (o && c.matchType(o.type)) break
+                    if (s && c.matchType(s.type)) break
                 }
             }
     }
     openMore() {
         let {
             content: e,
             openStart: t,
             openEnd: r
-        } = this.unplaced, i = ho(e, t);
-        return !i.childCount || i.firstChild.isLeaf ? !1 : (this.unplaced = new w(e, t + 1, Math.max(r, i.size + t >= e.size - r ? t + 1 : 0)), !0)
+        } = this.unplaced, i = Xr(e, t);
+        return !i.childCount || i.firstChild.isLeaf ? !1 : (this.unplaced = new E(e, t + 1, Math.max(r, i.size + t >= e.size - r ? t + 1 : 0)), !0)
     }
     dropNode() {
         let {
             content: e,
             openStart: t,
             openEnd: r
-        } = this.unplaced, i = ho(e, t);
+        } = this.unplaced, i = Xr(e, t);
         if (i.childCount <= 1 && t > 0) {
-            let o = e.size - t <= t + i.size;
-            this.unplaced = new w(cr(e, t - 1, 1), t - 1, o ? t - 1 : r)
-        } else this.unplaced = new w(cr(e, t, 1), t, r)
+            let s = e.size - t <= t + i.size;
+            this.unplaced = new E(dn(e, t - 1, 1), t - 1, s ? t - 1 : r)
+        } else this.unplaced = new E(dn(e, t, 1), t, r)
     }
     placeNodes({
         sliceDepth: e,
         frontierDepth: t,
         parent: r,
         inject: i,
-        wrap: o
+        wrap: s
     }) {
         for (; this.depth > t;) this.closeFrontierNode();
-        if (o)
-            for (let m = 0; m < o.length; m++) this.openFrontierNode(o[m]);
-        let s = this.unplaced,
-            l = r ? r.content : s.content,
-            a = s.openStart - e,
+        if (s)
+            for (let m = 0; m < s.length; m++) this.openFrontierNode(s[m]);
+        let o = this.unplaced,
+            l = r ? r.content : o.content,
+            a = o.openStart - e,
             c = 0,
             u = [],
             {
                 match: d,
                 type: f
             } = this.frontier[t];
         if (i) {
             for (let m = 0; m < i.childCount; m++) u.push(i.child(m));
             d = d.matchFragment(i)
         }
-        let p = l.size + e - (s.content.size - s.openEnd);
+        let h = l.size + e - (o.content.size - o.openEnd);
         for (; c < l.childCount;) {
             let m = l.child(c),
                 b = d.matchType(m.type);
             if (!b) break;
-            c++, (c > 1 || a == 0 || m.content.size) && (d = b, u.push(fa(m.mark(f.allowedMarks(m.marks)), c == 1 ? a : 0, c == l.childCount ? p : -1)))
+            c++, (c > 1 || a == 0 || m.content.size) && (d = b, u.push(So(m.mark(f.allowedMarks(m.marks)), c == 1 ? a : 0, c == l.childCount ? h : -1)))
         }
-        let h = c == l.childCount;
-        h || (p = -1), this.placed = ur(this.placed, t, v.from(u)), this.frontier[t].match = d, h && p < 0 && r && r.type == this.frontier[this.depth].type && this.frontier.length > 1 && this.closeFrontierNode();
-        for (let m = 0, b = l; m < p; m++) {
-            let k = b.lastChild;
+        let p = c == l.childCount;
+        p || (h = -1), this.placed = fn(this.placed, t, x.from(u)), this.frontier[t].match = d, p && h < 0 && r && r.type == this.frontier[this.depth].type && this.frontier.length > 1 && this.closeFrontierNode();
+        for (let m = 0, b = l; m < h; m++) {
+            let M = b.lastChild;
             this.frontier.push({
-                type: k.type,
-                match: k.contentMatchAt(k.childCount)
-            }), b = k.content
+                type: M.type,
+                match: M.contentMatchAt(M.childCount)
+            }), b = M.content
         }
-        this.unplaced = h ? e == 0 ? w.empty : new w(cr(s.content, e - 1, 1), e - 1, p < 0 ? s.openEnd : e - 1) : new w(cr(s.content, e, c), s.openStart, s.openEnd)
+        this.unplaced = p ? e == 0 ? E.empty : new E(dn(o.content, e - 1, 1), e - 1, h < 0 ? o.openEnd : e - 1) : new E(dn(o.content, e, c), o.openStart, o.openEnd)
     }
     mustMoveInline() {
         if (!this.$to.parent.isTextblock) return -1;
         let e = this.frontier[this.depth],
             t;
-        if (!e.type.isTextblock || !mo(this.$to, this.$to.depth, e.type, e.match, !1) || this.$to.depth == this.depth && (t = this.findCloseLevel(this.$to)) && t.depth == this.depth) return -1;
+        if (!e.type.isTextblock || !Zr(this.$to, this.$to.depth, e.type, e.match, !1) || this.$to.depth == this.depth && (t = this.findCloseLevel(this.$to)) && t.depth == this.depth) return -1;
         let {
             depth: r
         } = this.$to, i = this.$to.after(r);
         for (; r > 1 && i == this.$to.end(--r);) ++i;
         return i
     }
     findCloseLevel(e) {
         e: for (let t = Math.min(this.depth, e.depth); t >= 0; t--) {
             let {
                 match: r,
                 type: i
-            } = this.frontier[t], o = t < e.depth && e.end(t + 1) == e.pos + (e.depth - (t + 1)), s = mo(e, t, i, r, o);
-            if (s) {
+            } = this.frontier[t], s = t < e.depth && e.end(t + 1) == e.pos + (e.depth - (t + 1)), o = Zr(e, t, i, r, s);
+            if (o) {
                 for (let l = t - 1; l >= 0; l--) {
                     let {
                         match: a,
                         type: c
-                    } = this.frontier[l], u = mo(e, l, c, a, !0);
+                    } = this.frontier[l], u = Zr(e, l, c, a, !0);
                     if (!u || u.childCount) continue e
                 }
                 return {
                     depth: t,
-                    fit: s,
-                    move: o ? e.doc.resolve(e.after(t + 1)) : e
+                    fit: o,
+                    move: s ? e.doc.resolve(e.after(t + 1)) : e
                 }
             }
         }
     }
     close(e) {
         let t = this.findCloseLevel(e);
         if (!t) return null;
         for (; this.depth > t.depth;) this.closeFrontierNode();
-        t.fit.childCount && (this.placed = ur(this.placed, t.depth, t.fit)), e = t.move;
+        t.fit.childCount && (this.placed = fn(this.placed, t.depth, t.fit)), e = t.move;
         for (let r = t.depth + 1; r <= e.depth; r++) {
             let i = e.node(r),
-                o = i.type.contentMatch.fillBefore(i.content, !0, e.index(r));
-            this.openFrontierNode(i.type, i.attrs, o)
+                s = i.type.contentMatch.fillBefore(i.content, !0, e.index(r));
+            this.openFrontierNode(i.type, i.attrs, s)
         }
         return e
     }
     openFrontierNode(e, t = null, r) {
         let i = this.frontier[this.depth];
-        i.match = i.match.matchType(e), this.placed = ur(this.placed, this.depth, v.from(e.create(t, r))), this.frontier.push({
+        i.match = i.match.matchType(e), this.placed = fn(this.placed, this.depth, x.from(e.create(t, r))), this.frontier.push({
             type: e,
             match: e.contentMatch
         })
     }
     closeFrontierNode() {
-        let t = this.frontier.pop().match.fillBefore(v.empty, !0);
-        t.childCount && (this.placed = ur(this.placed, this.frontier.length, t))
+        let t = this.frontier.pop().match.fillBefore(x.empty, !0);
+        t.childCount && (this.placed = fn(this.placed, this.frontier.length, t))
     }
 };
 
-function cr(n, e, t) {
-    return e == 0 ? n.cutByIndex(t, n.childCount) : n.replaceChild(0, n.firstChild.copy(cr(n.firstChild.content, e - 1, t)))
+function dn(n, e, t) {
+    return e == 0 ? n.cutByIndex(t, n.childCount) : n.replaceChild(0, n.firstChild.copy(dn(n.firstChild.content, e - 1, t)))
 }
 
-function ur(n, e, t) {
-    return e == 0 ? n.append(t) : n.replaceChild(n.childCount - 1, n.lastChild.copy(ur(n.lastChild.content, e - 1, t)))
+function fn(n, e, t) {
+    return e == 0 ? n.append(t) : n.replaceChild(n.childCount - 1, n.lastChild.copy(fn(n.lastChild.content, e - 1, t)))
 }
 
-function ho(n, e) {
+function Xr(n, e) {
     for (let t = 0; t < e; t++) n = n.firstChild.content;
     return n
 }
 
-function fa(n, e, t) {
+function So(n, e, t) {
     if (e <= 0) return n;
     let r = n.content;
-    return e > 1 && (r = r.replaceChild(0, fa(r.firstChild, e - 1, r.childCount == 1 ? t - 1 : 0))), e > 0 && (r = n.type.contentMatch.fillBefore(r).append(r), t <= 0 && (r = r.append(n.type.contentMatch.matchFragment(r).fillBefore(v.empty, !0)))), n.copy(r)
+    return e > 1 && (r = r.replaceChild(0, So(r.firstChild, e - 1, r.childCount == 1 ? t - 1 : 0))), e > 0 && (r = n.type.contentMatch.fillBefore(r).append(r), t <= 0 && (r = r.append(n.type.contentMatch.matchFragment(r).fillBefore(x.empty, !0)))), n.copy(r)
 }
 
-function mo(n, e, t, r, i) {
-    let o = n.node(e),
-        s = i ? n.indexAfter(e) : n.index(e);
-    if (s == o.childCount && !t.compatibleContent(o.type)) return null;
-    let l = r.fillBefore(o.content, !0, s);
-    return l && !Nf(t, o.content, s) ? l : null
+function Zr(n, e, t, r, i) {
+    let s = n.node(e),
+        o = i ? n.indexAfter(e) : n.index(e);
+    if (o == s.childCount && !t.compatibleContent(s.type)) return null;
+    let l = r.fillBefore(s.content, !0, o);
+    return l && !eu(t, s.content, o) ? l : null
 }
 
-function Nf(n, e, t) {
+function eu(n, e, t) {
     for (let r = t; r < e.childCount; r++)
         if (!n.allowsMarks(e.child(r).marks)) return !0;
     return !1
 }
 
-function If(n) {
+function tu(n) {
     return n.spec.defining || n.spec.definingForContent
 }
 
-function Df(n, e, t, r) {
+function nu(n, e, t, r) {
     if (!r.size) return n.deleteRange(e, t);
     let i = n.doc.resolve(e),
-        o = n.doc.resolve(t);
-    if (da(i, o, r)) return n.step(new Q(e, t, r));
-    let s = ha(i, n.doc.resolve(t));
-    s[s.length - 1] == 0 && s.pop();
+        s = n.doc.resolve(t);
+    if (Mo(i, s, r)) return n.step(new q(e, t, r));
+    let o = wo(i, n.doc.resolve(t));
+    o[o.length - 1] == 0 && o.pop();
     let l = -(i.depth + 1);
-    s.unshift(l);
-    for (let f = i.depth, p = i.pos - 1; f > 0; f--, p--) {
-        let h = i.node(f).type.spec;
-        if (h.defining || h.definingAsContext || h.isolating) break;
-        s.indexOf(f) > -1 ? l = f : i.before(f) == p && s.splice(1, 0, -f)
+    o.unshift(l);
+    for (let f = i.depth, h = i.pos - 1; f > 0; f--, h--) {
+        let p = i.node(f).type.spec;
+        if (p.defining || p.definingAsContext || p.isolating) break;
+        o.indexOf(f) > -1 ? l = f : i.before(f) == h && o.splice(1, 0, -f)
     }
-    let a = s.indexOf(l),
+    let a = o.indexOf(l),
         c = [],
         u = r.openStart;
-    for (let f = r.content, p = 0;; p++) {
-        let h = f.firstChild;
-        if (c.push(h), p == r.openStart) break;
-        f = h.content
+    for (let f = r.content, h = 0;; h++) {
+        let p = f.firstChild;
+        if (c.push(p), h == r.openStart) break;
+        f = p.content
     }
     for (let f = u - 1; f >= 0; f--) {
-        let p = c[f].type,
-            h = If(p);
-        if (h && i.node(a).type != p) u = f;
-        else if (h || !p.isTextblock) break
+        let h = c[f].type,
+            p = tu(h);
+        if (p && i.node(a).type != h) u = f;
+        else if (p || !h.isTextblock) break
     }
     for (let f = r.openStart; f >= 0; f--) {
-        let p = (f + u + 1) % (r.openStart + 1),
-            h = c[p];
-        if (h)
-            for (let m = 0; m < s.length; m++) {
-                let b = s[(m + a) % s.length],
-                    k = !0;
-                b < 0 && (k = !1, b = -b);
-                let S = i.node(b - 1),
-                    C = i.index(b - 1);
-                if (S.canReplaceWith(C, C, h.type, h.marks)) return n.replace(i.before(b), k ? o.after(b) : t, new w(pa(r.content, 0, r.openStart, p), p, r.openEnd))
+        let h = (f + u + 1) % (r.openStart + 1),
+            p = c[h];
+        if (p)
+            for (let m = 0; m < o.length; m++) {
+                let b = o[(m + a) % o.length],
+                    M = !0;
+                b < 0 && (M = !1, b = -b);
+                let w = i.node(b - 1),
+                    v = i.index(b - 1);
+                if (w.canReplaceWith(v, v, p.type, p.marks)) return n.replace(i.before(b), M ? s.after(b) : t, new E(Eo(r.content, 0, r.openStart, h), h, r.openEnd))
             }
     }
     let d = n.steps.length;
-    for (let f = s.length - 1; f >= 0 && (n.replace(e, t, r), !(n.steps.length > d)); f--) {
-        let p = s[f];
-        p < 0 || (e = i.before(p), t = o.after(p))
+    for (let f = o.length - 1; f >= 0 && (n.replace(e, t, r), !(n.steps.length > d)); f--) {
+        let h = o[f];
+        h < 0 || (e = i.before(h), t = s.after(h))
     }
 }
 
-function pa(n, e, t, r, i) {
+function Eo(n, e, t, r, i) {
     if (e < t) {
-        let o = n.firstChild;
-        n = n.replaceChild(0, o.copy(pa(o.content, e + 1, t, r, o)))
+        let s = n.firstChild;
+        n = n.replaceChild(0, s.copy(Eo(s.content, e + 1, t, r, s)))
     }
     if (e > r) {
-        let o = i.contentMatchAt(0),
-            s = o.fillBefore(n).append(n);
-        n = s.append(o.matchFragment(s).fillBefore(v.empty, !0))
+        let s = i.contentMatchAt(0),
+            o = s.fillBefore(n).append(n);
+        n = o.append(s.matchFragment(o).fillBefore(x.empty, !0))
     }
     return n
 }
 
-function Lf(n, e, t, r) {
+function ru(n, e, t, r) {
     if (!r.isInline && e == t && n.doc.resolve(e).parent.content.size) {
-        let i = Af(n.doc, e, r.type);
+        let i = Zc(n.doc, e, r.type);
         i != null && (e = t = i)
     }
-    n.replaceRange(e, t, new w(v.from(r), 0, 0))
+    n.replaceRange(e, t, new E(x.from(r), 0, 0))
 }
 
-function Pf(n, e, t) {
+function iu(n, e, t) {
     let r = n.doc.resolve(e),
         i = n.doc.resolve(t),
-        o = ha(r, i);
-    for (let s = 0; s < o.length; s++) {
-        let l = o[s],
-            a = s == o.length - 1;
+        s = wo(r, i);
+    for (let o = 0; o < s.length; o++) {
+        let l = s[o],
+            a = o == s.length - 1;
         if (a && l == 0 || r.node(l).type.contentMatch.validEnd) return n.delete(r.start(l), i.end(l));
         if (l > 0 && (a || r.node(l - 1).canReplace(r.index(l - 1), i.indexAfter(l - 1)))) return n.delete(r.before(l), i.after(l))
     }
-    for (let s = 1; s <= r.depth && s <= i.depth; s++)
-        if (e - r.start(s) == r.depth - s && t > r.end(s) && i.end(s) - t != i.depth - s) return n.delete(r.before(s), t);
+    for (let o = 1; o <= r.depth && o <= i.depth; o++)
+        if (e - r.start(o) == r.depth - o && t > r.end(o) && i.end(o) - t != i.depth - o) return n.delete(r.before(o), t);
     n.delete(e, t)
 }
 
-function ha(n, e) {
+function wo(n, e) {
     let t = [],
         r = Math.min(n.depth, e.depth);
     for (let i = r; i >= 0; i--) {
-        let o = n.start(i);
-        if (o < n.pos - (n.depth - i) || e.end(i) > e.pos + (e.depth - i) || n.node(i).type.spec.isolating || e.node(i).type.spec.isolating) break;
-        (o == e.start(i) || i == n.depth && i == e.depth && n.parent.inlineContent && e.parent.inlineContent && i && e.start(i - 1) == o - 1) && t.push(i)
+        let s = n.start(i);
+        if (s < n.pos - (n.depth - i) || e.end(i) > e.pos + (e.depth - i) || n.node(i).type.spec.isolating || e.node(i).type.spec.isolating) break;
+        (s == e.start(i) || i == n.depth && i == e.depth && n.parent.inlineContent && e.parent.inlineContent && i && e.start(i - 1) == s - 1) && t.push(i)
     }
     return t
 }
-var Ot = class extends me {
+var _e = class extends ne {
     constructor(e, t, r) {
         super(), this.pos = e, this.attr = t, this.value = r
     }
     apply(e) {
         let t = e.nodeAt(this.pos);
-        if (!t) return X.fail("No node at attribute step's position");
+        if (!t) return K.fail("No node at attribute step's position");
         let r = Object.create(null);
-        for (let o in t.attrs) r[o] = t.attrs[o];
+        for (let s in t.attrs) r[s] = t.attrs[s];
         r[this.attr] = this.value;
         let i = t.type.create(r, null, t.marks);
-        return X.fromReplace(e, this.pos, this.pos + 1, new w(v.from(i), 0, t.isLeaf ? 0 : 1))
+        return K.fromReplace(e, this.pos, this.pos + 1, new E(x.from(i), 0, t.isLeaf ? 0 : 1))
     }
     getMap() {
-        return Te.empty
+        return de.empty
     }
     invert(e) {
-        return new Ot(this.pos, this.attr, e.nodeAt(this.pos).attrs[this.attr])
+        return new _e(this.pos, this.attr, e.nodeAt(this.pos).attrs[this.attr])
     }
     map(e) {
         let t = e.mapResult(this.pos, 1);
-        return t.deletedAfter ? null : new Ot(t.pos, this.attr, this.value)
+        return t.deletedAfter ? null : new _e(t.pos, this.attr, this.value)
     }
     toJSON() {
         return {
             stepType: "attr",
             pos: this.pos,
             attr: this.attr,
             value: this.value
         }
     }
     static fromJSON(e, t) {
         if (typeof t.pos != "number" || typeof t.attr != "string") throw new RangeError("Invalid input for AttrStep.fromJSON");
-        return new Ot(t.pos, t.attr, t.value)
+        return new _e(t.pos, t.attr, t.value)
     }
 };
-me.jsonID("attr", Ot);
-var Nn = class extends Error {};
-Nn = function n(e) {
+ne.jsonID("attr", _e);
+var zt = class extends Error {};
+zt = function n(e) {
     let t = Error.call(this, e);
     return t.__proto__ = n.prototype, t
 };
-Nn.prototype = Object.create(Error.prototype);
-Nn.prototype.constructor = Nn;
-Nn.prototype.name = "TransformError";
-var In = class {
+zt.prototype = Object.create(Error.prototype);
+zt.prototype.constructor = zt;
+zt.prototype.name = "TransformError";
+var Ht = class {
     constructor(e) {
-        this.doc = e, this.steps = [], this.docs = [], this.mapping = new mt
+        this.doc = e, this.steps = [], this.docs = [], this.mapping = new Fe
     }
     get before() {
         return this.docs.length ? this.docs[0] : this.doc
     }
     step(e) {
         let t = this.maybeStep(e);
-        if (t.failed) throw new Nn(t.failed);
+        if (t.failed) throw new zt(t.failed);
         return this
     }
     maybeStep(e) {
         let t = e.apply(this.doc);
         return t.failed || this.addStep(e, t.doc), t
     }
     get docChanged() {
         return this.steps.length > 0
     }
     addStep(e, t) {
         this.docs.push(this.doc), this.steps.push(e), this.mapping.appendMap(e.getMap()), this.doc = t
     }
-    replace(e, t = e, r = w.empty) {
-        let i = _r(this.doc, e, t, r);
+    replace(e, t = e, r = E.empty) {
+        let i = Gn(this.doc, e, t, r);
         return i && this.step(i), this
     }
     replaceWith(e, t, r) {
-        return this.replace(e, t, new w(v.from(r), 0, 0))
+        return this.replace(e, t, new E(x.from(r), 0, 0))
     }
     delete(e, t) {
-        return this.replace(e, t, w.empty)
+        return this.replace(e, t, E.empty)
     }
     insert(e, t) {
         return this.replaceWith(e, e, t)
     }
     replaceRange(e, t, r) {
-        return Df(this, e, t, r), this
+        return nu(this, e, t, r), this
     }
     replaceRangeWith(e, t, r) {
-        return Lf(this, e, t, r), this
+        return ru(this, e, t, r), this
     }
     deleteRange(e, t) {
-        return Pf(this, e, t), this
+        return iu(this, e, t), this
     }
     lift(e, t) {
-        return kf(this, e, t), this
+        return Wc(this, e, t), this
     }
     join(e, t = 1) {
-        return Of(this, e, t), this
+        return Xc(this, e, t), this
     }
     wrap(e, t) {
-        return Ef(this, e, t), this
+        return Uc(this, e, t), this
     }
     setBlockType(e, t = e, r, i = null) {
-        return Sf(this, e, t, r, i), this
+        return _c(this, e, t, r, i), this
     }
     setNodeMarkup(e, t, r = null, i) {
-        return Tf(this, e, t, r, i), this
+        return Qc(this, e, t, r, i), this
     }
     setNodeAttribute(e, t, r) {
-        return this.step(new Ot(e, t, r)), this
+        return this.step(new _e(e, t, r)), this
     }
     addNodeMark(e, t) {
-        return this.step(new Ze(e, t)), this
+        return this.step(new Ae(e, t)), this
     }
     removeNodeMark(e, t) {
-        if (!(t instanceof H)) {
+        if (!(t instanceof B)) {
             let r = this.doc.nodeAt(e);
             if (!r) throw new RangeError("No node at position " + e);
             if (t = t.isInSet(r.marks), !t) return this
         }
-        return this.step(new At(e, t)), this
+        return this.step(new Ge(e, t)), this
     }
     split(e, t = 1, r) {
-        return Cf(this, e, t, r), this
+        return Yc(this, e, t, r), this
     }
     addMark(e, t, r) {
-        return gf(this, e, t, r), this
+        return jc(this, e, t, r), this
     }
     removeMark(e, t, r) {
-        return yf(this, e, t, r), this
+        return $c(this, e, t, r), this
     }
     clearIncompatible(e, t, r) {
-        return xf(this, e, t, r), this
+        return Vc(this, e, t, r), this
     }
 };
-var ko = Object.create(null),
-    R = class {
+var ii = Object.create(null),
+    L = class {
         constructor(e, t, r) {
-            this.$anchor = e, this.$head = t, this.ranges = r || [new Mo(e.min(t), e.max(t))]
+            this.$anchor = e, this.$head = t, this.ranges = r || [new oi(e.min(t), e.max(t))]
         }
         get anchor() {
             return this.$anchor.pos
         }
         get head() {
             return this.$head.pos
         }
@@ -4500,391 +3270,391 @@
             for (let t = 0; t < e.length; t++)
                 if (e[t].$from.pos != e[t].$to.pos) return !1;
             return !0
         }
         content() {
             return this.$from.doc.slice(this.from, this.to, !0)
         }
-        replace(e, t = w.empty) {
+        replace(e, t = E.empty) {
             let r = t.content.lastChild,
                 i = null;
             for (let l = 0; l < t.openEnd; l++) i = r, r = r.lastChild;
-            let o = e.steps.length,
-                s = this.ranges;
-            for (let l = 0; l < s.length; l++) {
+            let s = e.steps.length,
+                o = this.ranges;
+            for (let l = 0; l < o.length; l++) {
                 let {
                     $from: a,
                     $to: c
-                } = s[l], u = e.mapping.slice(o);
-                e.replaceRange(u.map(a.pos), u.map(c.pos), l ? w.empty : t), l == 0 && ya(e, o, (r ? r.isInline : i && i.isTextblock) ? -1 : 1)
+                } = o[l], u = e.mapping.slice(s);
+                e.replaceRange(u.map(a.pos), u.map(c.pos), l ? E.empty : t), l == 0 && Ao(e, s, (r ? r.isInline : i && i.isTextblock) ? -1 : 1)
             }
         }
         replaceWith(e, t) {
             let r = e.steps.length,
                 i = this.ranges;
-            for (let o = 0; o < i.length; o++) {
+            for (let s = 0; s < i.length; s++) {
                 let {
-                    $from: s,
+                    $from: o,
                     $to: l
-                } = i[o], a = e.mapping.slice(r), c = a.map(s.pos), u = a.map(l.pos);
-                o ? e.deleteRange(c, u) : (e.replaceRangeWith(c, u, t), ya(e, r, t.isInline ? -1 : 1))
+                } = i[s], a = e.mapping.slice(r), c = a.map(o.pos), u = a.map(l.pos);
+                s ? e.deleteRange(c, u) : (e.replaceRangeWith(c, u, t), Ao(e, r, t.isInline ? -1 : 1))
             }
         }
         static findFrom(e, t, r = !1) {
-            let i = e.parent.inlineContent ? new P(e) : Ln(e.node(0), e.parent, e.pos, e.index(), t, r);
+            let i = e.parent.inlineContent ? new I(e) : jt(e.node(0), e.parent, e.pos, e.index(), t, r);
             if (i) return i;
-            for (let o = e.depth - 1; o >= 0; o--) {
-                let s = t < 0 ? Ln(e.node(0), e.node(o), e.before(o + 1), e.index(o), t, r) : Ln(e.node(0), e.node(o), e.after(o + 1), e.index(o) + 1, t, r);
-                if (s) return s
+            for (let s = e.depth - 1; s >= 0; s--) {
+                let o = t < 0 ? jt(e.node(0), e.node(s), e.before(s + 1), e.index(s), t, r) : jt(e.node(0), e.node(s), e.after(s + 1), e.index(s) + 1, t, r);
+                if (o) return o
             }
             return null
         }
         static near(e, t = 1) {
-            return this.findFrom(e, t) || this.findFrom(e, -t) || new fe(e.node(0))
+            return this.findFrom(e, t) || this.findFrom(e, -t) || new Z(e.node(0))
         }
         static atStart(e) {
-            return Ln(e, e, 0, 0, 1) || new fe(e)
+            return jt(e, e, 0, 0, 1) || new Z(e)
         }
         static atEnd(e) {
-            return Ln(e, e, e.content.size, e.childCount, -1) || new fe(e)
+            return jt(e, e, e.content.size, e.childCount, -1) || new Z(e)
         }
         static fromJSON(e, t) {
             if (!t || !t.type) throw new RangeError("Invalid input for Selection.fromJSON");
-            let r = ko[t.type];
+            let r = ii[t.type];
             if (!r) throw new RangeError(`No selection type ${t.type} defined`);
             return r.fromJSON(e, t)
         }
         static jsonID(e, t) {
-            if (e in ko) throw new RangeError("Duplicate use of selection JSON ID " + e);
-            return ko[e] = t, t.prototype.jsonID = e, t
+            if (e in ii) throw new RangeError("Duplicate use of selection JSON ID " + e);
+            return ii[e] = t, t.prototype.jsonID = e, t
         }
         getBookmark() {
-            return P.between(this.$anchor, this.$head).getBookmark()
+            return I.between(this.$anchor, this.$head).getBookmark()
         }
     };
-R.prototype.visible = !0;
-var Mo = class {
+L.prototype.visible = !0;
+var oi = class {
         constructor(e, t) {
             this.$from = e, this.$to = t
         }
     },
-    ma = !1;
+    To = !1;
 
-function ga(n) {
-    !ma && !n.parent.inlineContent && (ma = !0, console.warn("TextSelection endpoint not pointing into a node with inline content (" + n.parent.type.name + ")"))
+function Co(n) {
+    !To && !n.parent.inlineContent && (To = !0, console.warn("TextSelection endpoint not pointing into a node with inline content (" + n.parent.type.name + ")"))
 }
-var P = class extends R {
+var I = class extends L {
     constructor(e, t = e) {
-        ga(e), ga(t), super(e, t)
+        Co(e), Co(t), super(e, t)
     }
     get $cursor() {
         return this.$anchor.pos == this.$head.pos ? this.$head : null
     }
     map(e, t) {
         let r = e.resolve(t.map(this.head));
-        if (!r.parent.inlineContent) return R.near(r);
+        if (!r.parent.inlineContent) return L.near(r);
         let i = e.resolve(t.map(this.anchor));
-        return new P(i.parent.inlineContent ? i : r, r)
+        return new I(i.parent.inlineContent ? i : r, r)
     }
-    replace(e, t = w.empty) {
-        if (super.replace(e, t), t == w.empty) {
+    replace(e, t = E.empty) {
+        if (super.replace(e, t), t == E.empty) {
             let r = this.$from.marksAcross(this.$to);
             r && e.ensureMarks(r)
         }
     }
     eq(e) {
-        return e instanceof P && e.anchor == this.anchor && e.head == this.head
+        return e instanceof I && e.anchor == this.anchor && e.head == this.head
     }
     getBookmark() {
-        return new Pn(this.anchor, this.head)
+        return new $t(this.anchor, this.head)
     }
     toJSON() {
         return {
             type: "text",
             anchor: this.anchor,
             head: this.head
         }
     }
     static fromJSON(e, t) {
         if (typeof t.anchor != "number" || typeof t.head != "number") throw new RangeError("Invalid input for TextSelection.fromJSON");
-        return new P(e.resolve(t.anchor), e.resolve(t.head))
+        return new I(e.resolve(t.anchor), e.resolve(t.head))
     }
     static create(e, t, r = t) {
         let i = e.resolve(t);
         return new this(i, r == t ? i : e.resolve(r))
     }
     static between(e, t, r) {
         let i = e.pos - t.pos;
         if ((!r || i) && (r = i >= 0 ? 1 : -1), !t.parent.inlineContent) {
-            let o = R.findFrom(t, r, !0) || R.findFrom(t, -r, !0);
-            if (o) t = o.$head;
-            else return R.near(t, r)
+            let s = L.findFrom(t, r, !0) || L.findFrom(t, -r, !0);
+            if (s) t = s.$head;
+            else return L.near(t, r)
         }
-        return e.parent.inlineContent || (i == 0 ? e = t : (e = (R.findFrom(e, -r, !0) || R.findFrom(e, r, !0)).$anchor, e.pos < t.pos != i < 0 && (e = t))), new P(e, t)
+        return e.parent.inlineContent || (i == 0 ? e = t : (e = (L.findFrom(e, -r, !0) || L.findFrom(e, r, !0)).$anchor, e.pos < t.pos != i < 0 && (e = t))), new I(e, t)
     }
 };
-R.jsonID("text", P);
-var Pn = class {
+L.jsonID("text", I);
+var $t = class {
         constructor(e, t) {
             this.anchor = e, this.head = t
         }
         map(e) {
-            return new Pn(e.map(this.anchor), e.map(this.head))
+            return new $t(e.map(this.anchor), e.map(this.head))
         }
         resolve(e) {
-            return P.between(e.resolve(this.anchor), e.resolve(this.head))
+            return I.between(e.resolve(this.anchor), e.resolve(this.head))
         }
     },
-    D = class extends R {
+    O = class extends L {
         constructor(e) {
             let t = e.nodeAfter,
                 r = e.node(0).resolve(e.pos + t.nodeSize);
             super(e, r), this.node = t
         }
         map(e, t) {
             let {
                 deleted: r,
                 pos: i
-            } = t.mapResult(this.anchor), o = e.resolve(i);
-            return r ? R.near(o) : new D(o)
+            } = t.mapResult(this.anchor), s = e.resolve(i);
+            return r ? L.near(s) : new O(s)
         }
         content() {
-            return new w(v.from(this.node), 0, 0)
+            return new E(x.from(this.node), 0, 0)
         }
         eq(e) {
-            return e instanceof D && e.anchor == this.anchor
+            return e instanceof O && e.anchor == this.anchor
         }
         toJSON() {
             return {
                 type: "node",
                 anchor: this.anchor
             }
         }
         getBookmark() {
-            return new pr(this.anchor)
+            return new mn(this.anchor)
         }
         static fromJSON(e, t) {
             if (typeof t.anchor != "number") throw new RangeError("Invalid input for NodeSelection.fromJSON");
-            return new D(e.resolve(t.anchor))
+            return new O(e.resolve(t.anchor))
         }
         static create(e, t) {
-            return new D(e.resolve(t))
+            return new O(e.resolve(t))
         }
         static isSelectable(e) {
             return !e.isText && e.type.spec.selectable !== !1
         }
     };
-D.prototype.visible = !1;
-R.jsonID("node", D);
-var pr = class {
+O.prototype.visible = !1;
+L.jsonID("node", O);
+var mn = class {
         constructor(e) {
             this.anchor = e
         }
         map(e) {
             let {
                 deleted: t,
                 pos: r
             } = e.mapResult(this.anchor);
-            return t ? new Pn(r, r) : new pr(r)
+            return t ? new $t(r, r) : new mn(r)
         }
         resolve(e) {
             let t = e.resolve(this.anchor),
                 r = t.nodeAfter;
-            return r && D.isSelectable(r) ? new D(t) : R.near(t)
+            return r && O.isSelectable(r) ? new O(t) : L.near(t)
         }
     },
-    fe = class extends R {
+    Z = class extends L {
         constructor(e) {
             super(e.resolve(0), e.resolve(e.content.size))
         }
-        replace(e, t = w.empty) {
-            if (t == w.empty) {
+        replace(e, t = E.empty) {
+            if (t == E.empty) {
                 e.delete(0, e.doc.content.size);
-                let r = R.atStart(e.doc);
+                let r = L.atStart(e.doc);
                 r.eq(e.selection) || e.setSelection(r)
             } else super.replace(e, t)
         }
         toJSON() {
             return {
                 type: "all"
             }
         }
         static fromJSON(e) {
-            return new fe(e)
+            return new Z(e)
         }
         map(e) {
-            return new fe(e)
+            return new Z(e)
         }
         eq(e) {
-            return e instanceof fe
+            return e instanceof Z
         }
         getBookmark() {
-            return Rf
+            return su
         }
     };
-R.jsonID("all", fe);
-var Rf = {
+L.jsonID("all", Z);
+var su = {
     map() {
         return this
     },
     resolve(n) {
-        return new fe(n)
+        return new Z(n)
     }
 };
 
-function Ln(n, e, t, r, i, o = !1) {
-    if (e.inlineContent) return P.create(n, t);
-    for (let s = r - (i > 0 ? 0 : 1); i > 0 ? s < e.childCount : s >= 0; s += i) {
-        let l = e.child(s);
+function jt(n, e, t, r, i, s = !1) {
+    if (e.inlineContent) return I.create(n, t);
+    for (let o = r - (i > 0 ? 0 : 1); i > 0 ? o < e.childCount : o >= 0; o += i) {
+        let l = e.child(o);
         if (l.isAtom) {
-            if (!o && D.isSelectable(l)) return D.create(n, t - (i < 0 ? l.nodeSize : 0))
+            if (!s && O.isSelectable(l)) return O.create(n, t - (i < 0 ? l.nodeSize : 0))
         } else {
-            let a = Ln(n, l, t + i, i < 0 ? l.childCount : 0, i, o);
+            let a = jt(n, l, t + i, i < 0 ? l.childCount : 0, i, s);
             if (a) return a
         }
         t += l.nodeSize * i
     }
     return null
 }
 
-function ya(n, e, t) {
+function Ao(n, e, t) {
     let r = n.steps.length - 1;
     if (r < e) return;
     let i = n.steps[r];
-    if (!(i instanceof Q || i instanceof W)) return;
-    let o = n.mapping.maps[r],
-        s;
-    o.forEach((l, a, c, u) => {
-        s == null && (s = u)
-    }), n.setSelection(R.near(n.doc.resolve(s), t))
-}
-var xa = 1,
-    Gr = 2,
-    ba = 4,
-    Eo = class extends In {
+    if (!(i instanceof q || i instanceof j)) return;
+    let s = n.mapping.maps[r],
+        o;
+    s.forEach((l, a, c, u) => {
+        o == null && (o = u)
+    }), n.setSelection(L.near(n.doc.resolve(o), t))
+}
+var Oo = 1,
+    Qn = 2,
+    vo = 4,
+    li = class extends Ht {
         constructor(e) {
             super(e.doc), this.curSelectionFor = 0, this.updated = 0, this.meta = Object.create(null), this.time = Date.now(), this.curSelection = e.selection, this.storedMarks = e.storedMarks
         }
         get selection() {
             return this.curSelectionFor < this.steps.length && (this.curSelection = this.curSelection.map(this.doc, this.mapping.slice(this.curSelectionFor)), this.curSelectionFor = this.steps.length), this.curSelection
         }
         setSelection(e) {
             if (e.$from.doc != this.doc) throw new RangeError("Selection passed to setSelection must point at the current document");
-            return this.curSelection = e, this.curSelectionFor = this.steps.length, this.updated = (this.updated | xa) & ~Gr, this.storedMarks = null, this
+            return this.curSelection = e, this.curSelectionFor = this.steps.length, this.updated = (this.updated | Oo) & ~Qn, this.storedMarks = null, this
         }
         get selectionSet() {
-            return (this.updated & xa) > 0
+            return (this.updated & Oo) > 0
         }
         setStoredMarks(e) {
-            return this.storedMarks = e, this.updated |= Gr, this
+            return this.storedMarks = e, this.updated |= Qn, this
         }
         ensureMarks(e) {
-            return H.sameSet(this.storedMarks || this.selection.$from.marks(), e) || this.setStoredMarks(e), this
+            return B.sameSet(this.storedMarks || this.selection.$from.marks(), e) || this.setStoredMarks(e), this
         }
         addStoredMark(e) {
             return this.ensureMarks(e.addToSet(this.storedMarks || this.selection.$head.marks()))
         }
         removeStoredMark(e) {
             return this.ensureMarks(e.removeFromSet(this.storedMarks || this.selection.$head.marks()))
         }
         get storedMarksSet() {
-            return (this.updated & Gr) > 0
+            return (this.updated & Qn) > 0
         }
         addStep(e, t) {
-            super.addStep(e, t), this.updated = this.updated & ~Gr, this.storedMarks = null
+            super.addStep(e, t), this.updated = this.updated & ~Qn, this.storedMarks = null
         }
         setTime(e) {
             return this.time = e, this
         }
         replaceSelection(e) {
             return this.selection.replace(this, e), this
         }
         replaceSelectionWith(e, t = !0) {
             let r = this.selection;
-            return t && (e = e.mark(this.storedMarks || (r.empty ? r.$from.marks() : r.$from.marksAcross(r.$to) || H.none))), r.replaceWith(this, e), this
+            return t && (e = e.mark(this.storedMarks || (r.empty ? r.$from.marks() : r.$from.marksAcross(r.$to) || B.none))), r.replaceWith(this, e), this
         }
         deleteSelection() {
             return this.selection.replace(this), this
         }
         insertText(e, t, r) {
             let i = this.doc.type.schema;
             if (t == null) return e ? this.replaceSelectionWith(i.text(e), !0) : this.deleteSelection(); {
                 if (r == null && (r = t), r = r ?? t, !e) return this.deleteRange(t, r);
-                let o = this.storedMarks;
-                if (!o) {
-                    let s = this.doc.resolve(t);
-                    o = r == t ? s.marks() : s.marksAcross(this.doc.resolve(r))
+                let s = this.storedMarks;
+                if (!s) {
+                    let o = this.doc.resolve(t);
+                    s = r == t ? o.marks() : o.marksAcross(this.doc.resolve(r))
                 }
-                return this.replaceRangeWith(t, r, i.text(e, o)), this.selection.empty || this.setSelection(R.near(this.selection.$to)), this
+                return this.replaceRangeWith(t, r, i.text(e, s)), this.selection.empty || this.setSelection(L.near(this.selection.$to)), this
             }
         }
         setMeta(e, t) {
             return this.meta[typeof e == "string" ? e : e.key] = t, this
         }
         getMeta(e) {
             return this.meta[typeof e == "string" ? e : e.key]
         }
         get isGeneric() {
             for (let e in this.meta) return !1;
             return !0
         }
         scrollIntoView() {
-            return this.updated |= ba, this
+            return this.updated |= vo, this
         }
         get scrolledIntoView() {
-            return (this.updated & ba) > 0
+            return (this.updated & vo) > 0
         }
     };
 
-function ka(n, e) {
+function No(n, e) {
     return !e || !n ? n : n.bind(e)
 }
-var ln = class {
+var xt = class {
         constructor(e, t, r) {
-            this.name = e, this.init = ka(t.init, r), this.apply = ka(t.apply, r)
+            this.name = e, this.init = No(t.init, r), this.apply = No(t.apply, r)
         }
     },
-    Bf = [new ln("doc", {
+    ou = [new xt("doc", {
         init(n) {
             return n.doc || n.schema.topNodeType.createAndFill()
         },
         apply(n) {
             return n.doc
         }
-    }), new ln("selection", {
+    }), new xt("selection", {
         init(n, e) {
-            return n.selection || R.atStart(e.doc)
+            return n.selection || L.atStart(e.doc)
         },
         apply(n) {
             return n.selection
         }
-    }), new ln("storedMarks", {
+    }), new xt("storedMarks", {
         init(n) {
             return n.storedMarks || null
         },
         apply(n, e, t, r) {
             return r.selection.$cursor ? n.storedMarks : null
         }
-    }), new ln("scrollToSelection", {
+    }), new xt("scrollToSelection", {
         init() {
             return 0
         },
         apply(n, e) {
             return n.scrolledIntoView ? e + 1 : e
         }
     })],
-    fr = class {
+    pn = class {
         constructor(e, t) {
-            this.schema = e, this.plugins = [], this.pluginsByKey = Object.create(null), this.fields = Bf.slice(), t && t.forEach(r => {
+            this.schema = e, this.plugins = [], this.pluginsByKey = Object.create(null), this.fields = ou.slice(), t && t.forEach(r => {
                 if (this.pluginsByKey[r.key]) throw new RangeError("Adding different instances of a keyed plugin (" + r.key + ")");
-                this.plugins.push(r), this.pluginsByKey[r.key] = r, r.spec.state && this.fields.push(new ln(r.key, r.spec.state, r))
+                this.plugins.push(r), this.pluginsByKey[r.key] = r, r.spec.state && this.fields.push(new xt(r.key, r.spec.state, r))
             })
         }
     },
-    yt = class {
+    $e = class {
         constructor(e) {
             this.config = e
         }
         get schema() {
             return this.config.schema
         }
         get plugins() {
@@ -4905,211 +3675,211 @@
                 state: this,
                 transactions: []
             };
             let t = [e],
                 r = this.applyInner(e),
                 i = null;
             for (;;) {
-                let o = !1;
-                for (let s = 0; s < this.config.plugins.length; s++) {
-                    let l = this.config.plugins[s];
+                let s = !1;
+                for (let o = 0; o < this.config.plugins.length; o++) {
+                    let l = this.config.plugins[o];
                     if (l.spec.appendTransaction) {
-                        let a = i ? i[s].n : 0,
-                            c = i ? i[s].state : this,
+                        let a = i ? i[o].n : 0,
+                            c = i ? i[o].state : this,
                             u = a < t.length && l.spec.appendTransaction.call(l, a ? t.slice(a) : t, c, r);
-                        if (u && r.filterTransaction(u, s)) {
+                        if (u && r.filterTransaction(u, o)) {
                             if (u.setMeta("appendedTransaction", e), !i) {
                                 i = [];
-                                for (let d = 0; d < this.config.plugins.length; d++) i.push(d < s ? {
+                                for (let d = 0; d < this.config.plugins.length; d++) i.push(d < o ? {
                                     state: r,
                                     n: t.length
                                 } : {
                                     state: this,
                                     n: 0
                                 })
                             }
-                            t.push(u), r = r.applyInner(u), o = !0
+                            t.push(u), r = r.applyInner(u), s = !0
                         }
-                        i && (i[s] = {
+                        i && (i[o] = {
                             state: r,
                             n: t.length
                         })
                     }
                 }
-                if (!o) return {
+                if (!s) return {
                     state: r,
                     transactions: t
                 }
             }
         }
         applyInner(e) {
             if (!e.before.eq(this.doc)) throw new RangeError("Applying a mismatched transaction");
-            let t = new yt(this.config),
+            let t = new $e(this.config),
                 r = this.config.fields;
             for (let i = 0; i < r.length; i++) {
-                let o = r[i];
-                t[o.name] = o.apply(e, this[o.name], this, t)
+                let s = r[i];
+                t[s.name] = s.apply(e, this[s.name], this, t)
             }
             return t
         }
         get tr() {
-            return new Eo(this)
+            return new li(this)
         }
         static create(e) {
-            let t = new fr(e.doc ? e.doc.type.schema : e.schema, e.plugins),
-                r = new yt(t);
+            let t = new pn(e.doc ? e.doc.type.schema : e.schema, e.plugins),
+                r = new $e(t);
             for (let i = 0; i < t.fields.length; i++) r[t.fields[i].name] = t.fields[i].init(e, r);
             return r
         }
         reconfigure(e) {
-            let t = new fr(this.schema, e.plugins),
+            let t = new pn(this.schema, e.plugins),
                 r = t.fields,
-                i = new yt(t);
-            for (let o = 0; o < r.length; o++) {
-                let s = r[o].name;
-                i[s] = this.hasOwnProperty(s) ? this[s] : r[o].init(e, i)
+                i = new $e(t);
+            for (let s = 0; s < r.length; s++) {
+                let o = r[s].name;
+                i[o] = this.hasOwnProperty(o) ? this[o] : r[s].init(e, i)
             }
             return i
         }
         toJSON(e) {
             let t = {
                 doc: this.doc.toJSON(),
                 selection: this.selection.toJSON()
             };
             if (this.storedMarks && (t.storedMarks = this.storedMarks.map(r => r.toJSON())), e && typeof e == "object")
                 for (let r in e) {
                     if (r == "doc" || r == "selection") throw new RangeError("The JSON fields `doc` and `selection` are reserved");
                     let i = e[r],
-                        o = i.spec.state;
-                    o && o.toJSON && (t[r] = o.toJSON.call(i, this[i.key]))
+                        s = i.spec.state;
+                    s && s.toJSON && (t[r] = s.toJSON.call(i, this[i.key]))
                 }
             return t
         }
         static fromJSON(e, t, r) {
             if (!t) throw new RangeError("Invalid input for EditorState.fromJSON");
             if (!e.schema) throw new RangeError("Required config field 'schema' missing");
-            let i = new fr(e.schema, e.plugins),
-                o = new yt(i);
-            return i.fields.forEach(s => {
-                if (s.name == "doc") o.doc = we.fromJSON(e.schema, t.doc);
-                else if (s.name == "selection") o.selection = R.fromJSON(o.doc, t.selection);
-                else if (s.name == "storedMarks") t.storedMarks && (o.storedMarks = t.storedMarks.map(e.schema.markFromJSON));
+            let i = new pn(e.schema, e.plugins),
+                s = new $e(i);
+            return i.fields.forEach(o => {
+                if (o.name == "doc") s.doc = ue.fromJSON(e.schema, t.doc);
+                else if (o.name == "selection") s.selection = L.fromJSON(s.doc, t.selection);
+                else if (o.name == "storedMarks") t.storedMarks && (s.storedMarks = t.storedMarks.map(e.schema.markFromJSON));
                 else {
                     if (r)
                         for (let l in r) {
                             let a = r[l],
                                 c = a.spec.state;
-                            if (a.key == s.name && c && c.fromJSON && Object.prototype.hasOwnProperty.call(t, l)) {
-                                o[s.name] = c.fromJSON.call(a, e, t[l], o);
+                            if (a.key == o.name && c && c.fromJSON && Object.prototype.hasOwnProperty.call(t, l)) {
+                                s[o.name] = c.fromJSON.call(a, e, t[l], s);
                                 return
                             }
                         }
-                    o[s.name] = s.init(e, o)
+                    s[o.name] = o.init(e, s)
                 }
-            }), o
+            }), s
         }
     };
 
-function va(n, e, t) {
+function Io(n, e, t) {
     for (let r in n) {
         let i = n[r];
-        i instanceof Function ? i = i.bind(e) : r == "handleDOMEvents" && (i = va(i, e, {})), t[r] = i
+        i instanceof Function ? i = i.bind(e) : r == "handleDOMEvents" && (i = Io(i, e, {})), t[r] = i
     }
     return t
 }
-var q = class {
+var $ = class {
         constructor(e) {
-            this.spec = e, this.props = {}, e.props && va(e.props, this, this.props), this.key = e.key ? e.key.key : Ma("plugin")
+            this.spec = e, this.props = {}, e.props && Io(e.props, this, this.props), this.key = e.key ? e.key.key : Do("plugin")
         }
         getState(e) {
             return e[this.key]
         }
     },
-    vo = Object.create(null);
+    si = Object.create(null);
 
-function Ma(n) {
-    return n in vo ? n + "$" + ++vo[n] : (vo[n] = 0, n + "$")
+function Do(n) {
+    return n in si ? n + "$" + ++si[n] : (si[n] = 0, n + "$")
 }
-var Z = class {
+var U = class {
     constructor(e = "key") {
-        this.key = Ma(e)
+        this.key = Do(e)
     }
     get(e) {
         return e.config.pluginsByKey[this.key]
     }
     getState(e) {
         return e[this.key]
     }
 };
-var Fe = function(n) {
+var be = function(n) {
         for (var e = 0;; e++)
             if (n = n.previousSibling, !n) return e
     },
-    xr = function(n) {
+    kn = function(n) {
         let e = n.assignedSlot || n.parentNode;
         return e && e.nodeType == 11 ? e.host : e
     },
-    Ea = null,
-    xt = function(n, e, t) {
-        let r = Ea || (Ea = document.createRange());
+    Lo = null,
+    Ve = function(n, e, t) {
+        let r = Lo || (Lo = document.createRange());
         return r.setEnd(n, t ?? n.nodeValue.length), r.setStart(n, e || 0), r
     },
-    hn = function(n, e, t, r) {
-        return t && (Sa(n, e, t, r, -1) || Sa(n, e, t, r, 1))
+    Ct = function(n, e, t, r) {
+        return t && (Ro(n, e, t, r, -1) || Ro(n, e, t, r, 1))
     },
-    zf = /^(img|br|input|textarea|hr)$/i;
+    lu = /^(img|br|input|textarea|hr)$/i;
 
-function Sa(n, e, t, r, i) {
+function Ro(n, e, t, r, i) {
     for (;;) {
         if (n == t && e == r) return !0;
-        if (e == (i < 0 ? 0 : et(n))) {
-            let o = n.parentNode;
-            if (!o || o.nodeType != 1 || Ff(n) || zf.test(n.nodeName) || n.contentEditable == "false") return !1;
-            e = Fe(n) + (i < 0 ? 0 : 1), n = o
+        if (e == (i < 0 ? 0 : Oe(n))) {
+            let s = n.parentNode;
+            if (!s || s.nodeType != 1 || cu(n) || lu.test(n.nodeName) || n.contentEditable == "false") return !1;
+            e = be(n) + (i < 0 ? 0 : 1), n = s
         } else if (n.nodeType == 1) {
             if (n = n.childNodes[e + (i < 0 ? -1 : 0)], n.contentEditable == "false") return !1;
-            e = i < 0 ? et(n) : 0
+            e = i < 0 ? Oe(n) : 0
         } else return !1
     }
 }
 
-function et(n) {
+function Oe(n) {
     return n.nodeType == 3 ? n.nodeValue.length : n.childNodes.length
 }
 
-function Hf(n, e, t) {
-    for (let r = e == 0, i = e == et(n); r || i;) {
+function au(n, e, t) {
+    for (let r = e == 0, i = e == Oe(n); r || i;) {
         if (n == t) return !0;
-        let o = Fe(n);
+        let s = be(n);
         if (n = n.parentNode, !n) return !1;
-        r = r && o == 0, i = i && o == et(n)
+        r = r && s == 0, i = i && s == Oe(n)
     }
 }
 
-function Ff(n) {
+function cu(n) {
     let e;
     for (let t = n; t && !(e = t.pmViewDesc); t = t.parentNode);
     return e && e.node && e.node.isBlock && (e.dom == n || e.contentDOM == n)
 }
-var ni = function(n) {
-    return n.focusNode && hn(n.focusNode, n.focusOffset, n.anchorNode, n.anchorOffset)
+var rr = function(n) {
+    return n.focusNode && Ct(n.focusNode, n.focusOffset, n.anchorNode, n.anchorOffset)
 };
 
-function an(n, e) {
+function kt(n, e) {
     let t = document.createEvent("Event");
     return t.initEvent("keydown", !0, !0), t.keyCode = n, t.key = t.code = e, t
 }
 
-function jf(n) {
+function uu(n) {
     let e = n.activeElement;
     for (; e && e.shadowRoot;) e = e.shadowRoot.activeElement;
     return e
 }
 
-function Vf(n, e, t) {
+function du(n, e, t) {
     if (n.caretPositionFromPoint) try {
         let r = n.caretPositionFromPoint(e, t);
         if (r) return {
             node: r.offsetNode,
             offset: r.offset
         }
     } catch {}
@@ -5117,460 +3887,460 @@
         let r = n.caretRangeFromPoint(e, t);
         if (r) return {
             node: r.startContainer,
             offset: r.startOffset
         }
     }
 }
-var it = typeof navigator < "u" ? navigator : null,
-    wa = typeof document < "u" ? document : null,
-    Pt = it && it.userAgent || "",
-    Oo = /Edge\/(\d+)/.exec(Pt),
-    tc = /MSIE \d/.exec(Pt),
-    Ao = /Trident\/(?:[7-9]|\d{2,})\..*rv:(\d+)/.exec(Pt),
-    Ce = !!(tc || Ao || Oo),
-    Lt = tc ? document.documentMode : Ao ? +Ao[1] : Oo ? +Oo[1] : 0,
-    _e = !Ce && /gecko\/(\d+)/i.test(Pt);
-_e && +(/Firefox\/(\d+)/.exec(Pt) || [0, 0])[1];
-var No = !Ce && /Chrome\/(\d+)/.exec(Pt),
-    ye = !!No,
-    $f = No ? +No[1] : 0,
-    ve = !Ce && !!it && /Apple Computer/.test(it.vendor),
-    Hn = ve && (/Mobile\/\w+/.test(Pt) || !!it && it.maxTouchPoints > 2),
-    He = Hn || (it ? /Mac/.test(it.platform) : !1),
-    Wf = it ? /Win/.test(it.platform) : !1,
-    Ue = /Android \d/.test(Pt),
-    ri = !!wa && "webkitFontSmoothing" in wa.documentElement.style,
-    qf = ri ? +(/\bAppleWebKit\/(\d+)/.exec(navigator.userAgent) || [0, 0])[1] : 0;
+var De = typeof navigator < "u" ? navigator : null,
+    Po = typeof document < "u" ? document : null,
+    et = De && De.userAgent || "",
+    fi = /Edge\/(\d+)/.exec(et),
+    dl = /MSIE \d/.exec(et),
+    hi = /Trident\/(?:[7-9]|\d{2,})\..*rv:(\d+)/.exec(et),
+    fe = !!(dl || hi || fi),
+    Ze = dl ? document.documentMode : hi ? +hi[1] : fi ? +fi[1] : 0,
+    we = !fe && /gecko\/(\d+)/i.test(et);
+we && +(/Firefox\/(\d+)/.exec(et) || [0, 0])[1];
+var pi = !fe && /Chrome\/(\d+)/.exec(et),
+    ie = !!pi,
+    fu = pi ? +pi[1] : 0,
+    oe = !fe && !!De && /Apple Computer/.test(De.vendor),
+    qt = oe && (/Mobile\/\w+/.test(et) || !!De && De.maxTouchPoints > 2),
+    ye = qt || (De ? /Mac/.test(De.platform) : !1),
+    hu = De ? /Win/.test(De.platform) : !1,
+    Ee = /Android \d/.test(et),
+    ir = !!Po && "webkitFontSmoothing" in Po.documentElement.style,
+    pu = ir ? +(/\bAppleWebKit\/(\d+)/.exec(navigator.userAgent) || [0, 0])[1] : 0;
 
-function Jf(n) {
+function mu(n) {
     return {
         left: 0,
         right: n.documentElement.clientWidth,
         top: 0,
         bottom: n.documentElement.clientHeight
     }
 }
 
-function Nt(n, e) {
+function Qe(n, e) {
     return typeof n == "number" ? n : n[e]
 }
 
-function Kf(n) {
+function gu(n) {
     let e = n.getBoundingClientRect(),
         t = e.width / n.offsetWidth || 1,
         r = e.height / n.offsetHeight || 1;
     return {
         left: e.left,
         right: e.left + n.clientWidth * t,
         top: e.top,
         bottom: e.top + n.clientHeight * r
     }
 }
 
-function Ta(n, e, t) {
+function Bo(n, e, t) {
     let r = n.someProp("scrollThreshold") || 0,
         i = n.someProp("scrollMargin") || 5,
-        o = n.dom.ownerDocument;
-    for (let s = t || n.dom; s; s = xr(s)) {
-        if (s.nodeType != 1) continue;
-        let l = s,
-            a = l == o.body,
-            c = a ? Jf(o) : Kf(l),
+        s = n.dom.ownerDocument;
+    for (let o = t || n.dom; o; o = kn(o)) {
+        if (o.nodeType != 1) continue;
+        let l = o,
+            a = l == s.body,
+            c = a ? mu(s) : gu(l),
             u = 0,
             d = 0;
-        if (e.top < c.top + Nt(r, "top") ? d = -(c.top - e.top + Nt(i, "top")) : e.bottom > c.bottom - Nt(r, "bottom") && (d = e.bottom - c.bottom + Nt(i, "bottom")), e.left < c.left + Nt(r, "left") ? u = -(c.left - e.left + Nt(i, "left")) : e.right > c.right - Nt(r, "right") && (u = e.right - c.right + Nt(i, "right")), u || d)
-            if (a) o.defaultView.scrollBy(u, d);
+        if (e.top < c.top + Qe(r, "top") ? d = -(c.top - e.top + Qe(i, "top")) : e.bottom > c.bottom - Qe(r, "bottom") && (d = e.bottom - c.bottom + Qe(i, "bottom")), e.left < c.left + Qe(r, "left") ? u = -(c.left - e.left + Qe(i, "left")) : e.right > c.right - Qe(r, "right") && (u = e.right - c.right + Qe(i, "right")), u || d)
+            if (a) s.defaultView.scrollBy(u, d);
             else {
                 let f = l.scrollLeft,
-                    p = l.scrollTop;
+                    h = l.scrollTop;
                 d && (l.scrollTop += d), u && (l.scrollLeft += u);
-                let h = l.scrollLeft - f,
-                    m = l.scrollTop - p;
+                let p = l.scrollLeft - f,
+                    m = l.scrollTop - h;
                 e = {
-                    left: e.left - h,
+                    left: e.left - p,
                     top: e.top - m,
-                    right: e.right - h,
+                    right: e.right - p,
                     bottom: e.bottom - m
                 }
             } if (a) break
     }
 }
 
-function Uf(n) {
+function yu(n) {
     let e = n.dom.getBoundingClientRect(),
         t = Math.max(0, e.top),
         r, i;
-    for (let o = (e.left + e.right) / 2, s = t + 1; s < Math.min(innerHeight, e.bottom); s += 5) {
-        let l = n.root.elementFromPoint(o, s);
+    for (let s = (e.left + e.right) / 2, o = t + 1; o < Math.min(innerHeight, e.bottom); o += 5) {
+        let l = n.root.elementFromPoint(s, o);
         if (!l || l == n.dom || !n.dom.contains(l)) continue;
         let a = l.getBoundingClientRect();
         if (a.top >= t - 20) {
             r = l, i = a.top;
             break
         }
     }
     return {
         refDOM: r,
         refTop: i,
-        stack: nc(n.dom)
+        stack: fl(n.dom)
     }
 }
 
-function nc(n) {
+function fl(n) {
     let e = [],
         t = n.ownerDocument;
     for (let r = n; r && (e.push({
             dom: r,
             top: r.scrollTop,
             left: r.scrollLeft
-        }), n != t); r = xr(r));
+        }), n != t); r = kn(r));
     return e
 }
 
-function _f({
+function bu({
     refDOM: n,
     refTop: e,
     stack: t
 }) {
     let r = n ? n.getBoundingClientRect().top : 0;
-    rc(t, r == 0 ? 0 : r - e)
+    hl(t, r == 0 ? 0 : r - e)
 }
 
-function rc(n, e) {
+function hl(n, e) {
     for (let t = 0; t < n.length; t++) {
         let {
             dom: r,
             top: i,
-            left: o
+            left: s
         } = n[t];
-        r.scrollTop != i + e && (r.scrollTop = i + e), r.scrollLeft != o && (r.scrollLeft = o)
+        r.scrollTop != i + e && (r.scrollTop = i + e), r.scrollLeft != s && (r.scrollLeft = s)
     }
 }
-var Rn = null;
+var Vt = null;
 
-function Gf(n) {
+function xu(n) {
     if (n.setActive) return n.setActive();
-    if (Rn) return n.focus(Rn);
-    let e = nc(n);
-    n.focus(Rn == null ? {
+    if (Vt) return n.focus(Vt);
+    let e = fl(n);
+    n.focus(Vt == null ? {
         get preventScroll() {
-            return Rn = {
+            return Vt = {
                 preventScroll: !0
             }, !0
         }
-    } : void 0), Rn || (Rn = !1, rc(e, 0))
+    } : void 0), Vt || (Vt = !1, hl(e, 0))
 }
 
-function ic(n, e) {
+function pl(n, e) {
     let t, r = 2e8,
-        i, o = 0,
-        s = e.top,
+        i, s = 0,
+        o = e.top,
         l = e.top,
         a, c;
     for (let u = n.firstChild, d = 0; u; u = u.nextSibling, d++) {
         let f;
         if (u.nodeType == 1) f = u.getClientRects();
-        else if (u.nodeType == 3) f = xt(u).getClientRects();
+        else if (u.nodeType == 3) f = Ve(u).getClientRects();
         else continue;
-        for (let p = 0; p < f.length; p++) {
-            let h = f[p];
-            if (h.top <= s && h.bottom >= l) {
-                s = Math.max(h.bottom, s), l = Math.min(h.top, l);
-                let m = h.left > e.left ? h.left - e.left : h.right < e.left ? e.left - h.right : 0;
+        for (let h = 0; h < f.length; h++) {
+            let p = f[h];
+            if (p.top <= o && p.bottom >= l) {
+                o = Math.max(p.bottom, o), l = Math.min(p.top, l);
+                let m = p.left > e.left ? p.left - e.left : p.right < e.left ? e.left - p.right : 0;
                 if (m < r) {
                     t = u, r = m, i = m && t.nodeType == 3 ? {
-                        left: h.right < e.left ? h.right : h.left,
+                        left: p.right < e.left ? p.right : p.left,
                         top: e.top
-                    } : e, u.nodeType == 1 && m && (o = d + (e.left >= (h.left + h.right) / 2 ? 1 : 0));
+                    } : e, u.nodeType == 1 && m && (s = d + (e.left >= (p.left + p.right) / 2 ? 1 : 0));
                     continue
                 }
-            } else h.top > e.top && !a && h.left <= e.left && h.right >= e.left && (a = u, c = {
-                left: Math.max(h.left, Math.min(h.right, e.left)),
-                top: h.top
+            } else p.top > e.top && !a && p.left <= e.left && p.right >= e.left && (a = u, c = {
+                left: Math.max(p.left, Math.min(p.right, e.left)),
+                top: p.top
             });
-            !t && (e.left >= h.right && e.top >= h.top || e.left >= h.left && e.top >= h.bottom) && (o = d + 1)
+            !t && (e.left >= p.right && e.top >= p.top || e.left >= p.left && e.top >= p.bottom) && (s = d + 1)
         }
     }
-    return !t && a && (t = a, i = c, r = 0), t && t.nodeType == 3 ? Yf(t, i) : !t || r && t.nodeType == 1 ? {
+    return !t && a && (t = a, i = c, r = 0), t && t.nodeType == 3 ? ku(t, i) : !t || r && t.nodeType == 1 ? {
         node: n,
-        offset: o
-    } : ic(t, i)
+        offset: s
+    } : pl(t, i)
 }
 
-function Yf(n, e) {
+function ku(n, e) {
     let t = n.nodeValue.length,
         r = document.createRange();
     for (let i = 0; i < t; i++) {
         r.setEnd(n, i + 1), r.setStart(n, i);
-        let o = It(r, 1);
-        if (o.top != o.bottom && Ko(e, o)) return {
+        let s = Ye(r, 1);
+        if (s.top != s.bottom && Ni(e, s)) return {
             node: n,
-            offset: i + (e.left >= (o.left + o.right) / 2 ? 1 : 0)
+            offset: i + (e.left >= (s.left + s.right) / 2 ? 1 : 0)
         }
     }
     return {
         node: n,
         offset: 0
     }
 }
 
-function Ko(n, e) {
+function Ni(n, e) {
     return n.left >= e.left - 1 && n.left <= e.right + 1 && n.top >= e.top - 1 && n.top <= e.bottom + 1
 }
 
-function Qf(n, e) {
+function Mu(n, e) {
     let t = n.parentNode;
     return t && /^li$/i.test(t.nodeName) && e.left < n.getBoundingClientRect().left ? t : n
 }
 
-function Xf(n, e, t) {
+function Su(n, e, t) {
     let {
         node: r,
         offset: i
-    } = ic(e, t), o = -1;
+    } = pl(e, t), s = -1;
     if (r.nodeType == 1 && !r.firstChild) {
-        let s = r.getBoundingClientRect();
-        o = s.left != s.right && t.left > (s.left + s.right) / 2 ? 1 : -1
+        let o = r.getBoundingClientRect();
+        s = o.left != o.right && t.left > (o.left + o.right) / 2 ? 1 : -1
     }
-    return n.docView.posFromDOM(r, i, o)
+    return n.docView.posFromDOM(r, i, s)
 }
 
-function Zf(n, e, t, r) {
+function Eu(n, e, t, r) {
     let i = -1;
-    for (let o = e, s = !1; o != n.dom;) {
-        let l = n.docView.nearestDesc(o, !0);
+    for (let s = e, o = !1; s != n.dom;) {
+        let l = n.docView.nearestDesc(s, !0);
         if (!l) return null;
-        if (l.dom.nodeType == 1 && (l.node.isBlock && l.parent && !s || !l.contentDOM)) {
+        if (l.dom.nodeType == 1 && (l.node.isBlock && l.parent && !o || !l.contentDOM)) {
             let a = l.dom.getBoundingClientRect();
-            if (l.node.isBlock && l.parent && !s && (s = !0, a.left > r.left || a.top > r.top ? i = l.posBefore : (a.right < r.left || a.bottom < r.top) && (i = l.posAfter)), !l.contentDOM && i < 0) return (l.node.isBlock ? r.top < (a.top + a.bottom) / 2 : r.left < (a.left + a.right) / 2) ? l.posBefore : l.posAfter
+            if (l.node.isBlock && l.parent && !o && (o = !0, a.left > r.left || a.top > r.top ? i = l.posBefore : (a.right < r.left || a.bottom < r.top) && (i = l.posAfter)), !l.contentDOM && i < 0) return (l.node.isBlock ? r.top < (a.top + a.bottom) / 2 : r.left < (a.left + a.right) / 2) ? l.posBefore : l.posAfter
         }
-        o = l.dom.parentNode
+        s = l.dom.parentNode
     }
     return i > -1 ? i : n.docView.posFromDOM(e, t, -1)
 }
 
-function oc(n, e, t) {
+function ml(n, e, t) {
     let r = n.childNodes.length;
     if (r && t.top < t.bottom)
-        for (let i = Math.max(0, Math.min(r - 1, Math.floor(r * (e.top - t.top) / (t.bottom - t.top)) - 2)), o = i;;) {
-            let s = n.childNodes[o];
-            if (s.nodeType == 1) {
-                let l = s.getClientRects();
+        for (let i = Math.max(0, Math.min(r - 1, Math.floor(r * (e.top - t.top) / (t.bottom - t.top)) - 2)), s = i;;) {
+            let o = n.childNodes[s];
+            if (o.nodeType == 1) {
+                let l = o.getClientRects();
                 for (let a = 0; a < l.length; a++) {
                     let c = l[a];
-                    if (Ko(e, c)) return oc(s, e, c)
+                    if (Ni(e, c)) return ml(o, e, c)
                 }
             }
-            if ((o = (o + 1) % r) == i) break
+            if ((s = (s + 1) % r) == i) break
         }
     return n
 }
 
-function ep(n, e) {
+function wu(n, e) {
     let t = n.dom.ownerDocument,
         r, i = 0,
-        o = Vf(t, e.left, e.top);
-    o && ({
+        s = du(t, e.left, e.top);
+    s && ({
         node: r,
         offset: i
-    } = o);
-    let s = (n.root.elementFromPoint ? n.root : t).elementFromPoint(e.left, e.top),
+    } = s);
+    let o = (n.root.elementFromPoint ? n.root : t).elementFromPoint(e.left, e.top),
         l;
-    if (!s || !n.dom.contains(s.nodeType != 1 ? s.parentNode : s)) {
+    if (!o || !n.dom.contains(o.nodeType != 1 ? o.parentNode : o)) {
         let c = n.dom.getBoundingClientRect();
-        if (!Ko(e, c) || (s = oc(n.dom, e, c), !s)) return null
+        if (!Ni(e, c) || (o = ml(n.dom, e, c), !o)) return null
     }
-    if (ve)
-        for (let c = s; r && c; c = xr(c)) c.draggable && (r = void 0);
-    if (s = Qf(s, e), r) {
-        if (_e && r.nodeType == 1 && (i = Math.min(i, r.childNodes.length), i < r.childNodes.length)) {
+    if (oe)
+        for (let c = o; r && c; c = kn(c)) c.draggable && (r = void 0);
+    if (o = Mu(o, e), r) {
+        if (we && r.nodeType == 1 && (i = Math.min(i, r.childNodes.length), i < r.childNodes.length)) {
             let c = r.childNodes[i],
                 u;
             c.nodeName == "IMG" && (u = c.getBoundingClientRect()).right <= e.left && u.bottom > e.top && i++
         }
-        r == n.dom && i == r.childNodes.length - 1 && r.lastChild.nodeType == 1 && e.top > r.lastChild.getBoundingClientRect().bottom ? l = n.state.doc.content.size : (i == 0 || r.nodeType != 1 || r.childNodes[i - 1].nodeName != "BR") && (l = Zf(n, r, i, e))
+        r == n.dom && i == r.childNodes.length - 1 && r.lastChild.nodeType == 1 && e.top > r.lastChild.getBoundingClientRect().bottom ? l = n.state.doc.content.size : (i == 0 || r.nodeType != 1 || r.childNodes[i - 1].nodeName != "BR") && (l = Eu(n, r, i, e))
     }
-    l == null && (l = Xf(n, s, e));
-    let a = n.docView.nearestDesc(s, !0);
+    l == null && (l = Su(n, o, e));
+    let a = n.docView.nearestDesc(o, !0);
     return {
         pos: l,
         inside: a ? a.posAtStart - a.border : -1
     }
 }
 
-function Ca(n) {
+function zo(n) {
     return n.top < n.bottom || n.left < n.right
 }
 
-function It(n, e) {
+function Ye(n, e) {
     let t = n.getClientRects();
     if (t.length) {
         let r = t[e < 0 ? 0 : t.length - 1];
-        if (Ca(r)) return r
+        if (zo(r)) return r
     }
-    return Array.prototype.find.call(t, Ca) || n.getBoundingClientRect()
+    return Array.prototype.find.call(t, zo) || n.getBoundingClientRect()
 }
-var tp = /[\u0590-\u05f4\u0600-\u06ff\u0700-\u08ac]/;
+var Tu = /[\u0590-\u05f4\u0600-\u06ff\u0700-\u08ac]/;
 
-function sc(n, e, t) {
+function gl(n, e, t) {
     let {
         node: r,
         offset: i,
-        atom: o
-    } = n.docView.domFromPos(e, t < 0 ? -1 : 1), s = ri || _e;
+        atom: s
+    } = n.docView.domFromPos(e, t < 0 ? -1 : 1), o = ir || we;
     if (r.nodeType == 3)
-        if (s && (tp.test(r.nodeValue) || (t < 0 ? !i : i == r.nodeValue.length))) {
-            let a = It(xt(r, i, i), t);
-            if (_e && i && /\s/.test(r.nodeValue[i - 1]) && i < r.nodeValue.length) {
-                let c = It(xt(r, i - 1, i - 1), -1);
+        if (o && (Tu.test(r.nodeValue) || (t < 0 ? !i : i == r.nodeValue.length))) {
+            let a = Ye(Ve(r, i, i), t);
+            if (we && i && /\s/.test(r.nodeValue[i - 1]) && i < r.nodeValue.length) {
+                let c = Ye(Ve(r, i - 1, i - 1), -1);
                 if (c.top == a.top) {
-                    let u = It(xt(r, i, i + 1), -1);
-                    if (u.top != a.top) return hr(u, u.left < c.left)
+                    let u = Ye(Ve(r, i, i + 1), -1);
+                    if (u.top != a.top) return gn(u, u.left < c.left)
                 }
             }
             return a
         } else {
             let a = i,
                 c = i,
                 u = t < 0 ? 1 : -1;
-            return t < 0 && !i ? (c++, u = -1) : t >= 0 && i == r.nodeValue.length ? (a--, u = 1) : t < 0 ? a-- : c++, hr(It(xt(r, a, c), u), u < 0)
-        } if (!n.state.doc.resolve(e - (o || 0)).parent.inlineContent) {
-        if (o == null && i && (t < 0 || i == et(r))) {
+            return t < 0 && !i ? (c++, u = -1) : t >= 0 && i == r.nodeValue.length ? (a--, u = 1) : t < 0 ? a-- : c++, gn(Ye(Ve(r, a, c), u), u < 0)
+        } if (!n.state.doc.resolve(e - (s || 0)).parent.inlineContent) {
+        if (s == null && i && (t < 0 || i == Oe(r))) {
             let a = r.childNodes[i - 1];
-            if (a.nodeType == 1) return So(a.getBoundingClientRect(), !1)
+            if (a.nodeType == 1) return ai(a.getBoundingClientRect(), !1)
         }
-        if (o == null && i < et(r)) {
+        if (s == null && i < Oe(r)) {
             let a = r.childNodes[i];
-            if (a.nodeType == 1) return So(a.getBoundingClientRect(), !0)
+            if (a.nodeType == 1) return ai(a.getBoundingClientRect(), !0)
         }
-        return So(r.getBoundingClientRect(), t >= 0)
+        return ai(r.getBoundingClientRect(), t >= 0)
     }
-    if (o == null && i && (t < 0 || i == et(r))) {
+    if (s == null && i && (t < 0 || i == Oe(r))) {
         let a = r.childNodes[i - 1],
-            c = a.nodeType == 3 ? xt(a, et(a) - (s ? 0 : 1)) : a.nodeType == 1 && (a.nodeName != "BR" || !a.nextSibling) ? a : null;
-        if (c) return hr(It(c, 1), !1)
+            c = a.nodeType == 3 ? Ve(a, Oe(a) - (o ? 0 : 1)) : a.nodeType == 1 && (a.nodeName != "BR" || !a.nextSibling) ? a : null;
+        if (c) return gn(Ye(c, 1), !1)
     }
-    if (o == null && i < et(r)) {
+    if (s == null && i < Oe(r)) {
         let a = r.childNodes[i];
         for (; a.pmViewDesc && a.pmViewDesc.ignoreForCoords;) a = a.nextSibling;
-        let c = a ? a.nodeType == 3 ? xt(a, 0, s ? 0 : 1) : a.nodeType == 1 ? a : null : null;
-        if (c) return hr(It(c, -1), !0)
+        let c = a ? a.nodeType == 3 ? Ve(a, 0, o ? 0 : 1) : a.nodeType == 1 ? a : null : null;
+        if (c) return gn(Ye(c, -1), !0)
     }
-    return hr(It(r.nodeType == 3 ? xt(r) : r, -t), t >= 0)
+    return gn(Ye(r.nodeType == 3 ? Ve(r) : r, -t), t >= 0)
 }
 
-function hr(n, e) {
+function gn(n, e) {
     if (n.width == 0) return n;
     let t = e ? n.left : n.right;
     return {
         top: n.top,
         bottom: n.bottom,
         left: t,
         right: t
     }
 }
 
-function So(n, e) {
+function ai(n, e) {
     if (n.height == 0) return n;
     let t = e ? n.top : n.bottom;
     return {
         top: t,
         bottom: t,
         left: n.left,
         right: n.right
     }
 }
 
-function lc(n, e, t) {
+function yl(n, e, t) {
     let r = n.state,
         i = n.root.activeElement;
     r != e && n.updateState(e), i != n.dom && n.focus();
     try {
         return t()
     } finally {
         r != e && n.updateState(r), i != n.dom && i && i.focus()
     }
 }
 
-function np(n, e, t) {
+function Cu(n, e, t) {
     let r = e.selection,
         i = t == "up" ? r.$from : r.$to;
-    return lc(n, e, () => {
+    return yl(n, e, () => {
         let {
-            node: o
+            node: s
         } = n.docView.domFromPos(i.pos, t == "up" ? -1 : 1);
         for (;;) {
-            let l = n.docView.nearestDesc(o, !0);
+            let l = n.docView.nearestDesc(s, !0);
             if (!l) break;
             if (l.node.isBlock) {
-                o = l.contentDOM || l.dom;
+                s = l.contentDOM || l.dom;
                 break
             }
-            o = l.dom.parentNode
+            s = l.dom.parentNode
         }
-        let s = sc(n, i.pos, 1);
-        for (let l = o.firstChild; l; l = l.nextSibling) {
+        let o = gl(n, i.pos, 1);
+        for (let l = s.firstChild; l; l = l.nextSibling) {
             let a;
             if (l.nodeType == 1) a = l.getClientRects();
-            else if (l.nodeType == 3) a = xt(l, 0, l.nodeValue.length).getClientRects();
+            else if (l.nodeType == 3) a = Ve(l, 0, l.nodeValue.length).getClientRects();
             else continue;
             for (let c = 0; c < a.length; c++) {
                 let u = a[c];
-                if (u.bottom > u.top + 1 && (t == "up" ? s.top - u.top > (u.bottom - s.top) * 2 : u.bottom - s.bottom > (s.bottom - u.top) * 2)) return !1
+                if (u.bottom > u.top + 1 && (t == "up" ? o.top - u.top > (u.bottom - o.top) * 2 : u.bottom - o.bottom > (o.bottom - u.top) * 2)) return !1
             }
         }
         return !0
     })
 }
-var rp = /[\u0590-\u08ac]/;
+var Au = /[\u0590-\u08ac]/;
 
-function ip(n, e, t) {
+function Ou(n, e, t) {
     let {
         $head: r
     } = e.selection;
     if (!r.parent.isTextblock) return !1;
     let i = r.parentOffset,
-        o = !i,
-        s = i == r.parent.content.size,
+        s = !i,
+        o = i == r.parent.content.size,
         l = n.domSelection();
-    return !rp.test(r.parent.textContent) || !l.modify ? t == "left" || t == "backward" ? o : s : lc(n, e, () => {
+    return !Au.test(r.parent.textContent) || !l.modify ? t == "left" || t == "backward" ? s : o : yl(n, e, () => {
         let {
             focusNode: a,
             focusOffset: c,
             anchorNode: u,
             anchorOffset: d
         } = n.domSelectionRange(), f = l.caretBidiLevel;
         l.modify("move", t, "character");
-        let p = r.depth ? n.docView.domAfterPos(r.before()) : n.dom,
+        let h = r.depth ? n.docView.domAfterPos(r.before()) : n.dom,
             {
-                focusNode: h,
+                focusNode: p,
                 focusOffset: m
             } = n.domSelectionRange(),
-            b = h && !p.contains(h.nodeType == 1 ? h : h.parentNode) || a == h && c == m;
+            b = p && !h.contains(p.nodeType == 1 ? p : p.parentNode) || a == p && c == m;
         try {
             l.collapse(u, d), a && (a != u || c != d) && l.extend && l.extend(a, c)
         } catch {}
         return f != null && (l.caretBidiLevel = f), b
     })
 }
-var Oa = null,
-    Aa = null,
-    Na = !1;
-
-function op(n, e, t) {
-    return Oa == e && Aa == t ? Na : (Oa = e, Aa = t, Na = t == "up" || t == "down" ? np(n, e, t) : ip(n, e, t))
-}
-var je = 0,
-    Ia = 1,
-    un = 2,
-    ot = 3,
-    mn = class {
+var Ho = null,
+    Fo = null,
+    jo = !1;
+
+function vu(n, e, t) {
+    return Ho == e && Fo == t ? jo : (Ho = e, Fo = t, jo = t == "up" || t == "down" ? Cu(n, e, t) : Ou(n, e, t))
+}
+var xe = 0,
+    $o = 1,
+    St = 2,
+    Le = 3,
+    At = class {
         constructor(e, t, r, i) {
-            this.parent = e, this.children = t, this.dom = r, this.contentDOM = i, this.dirty = je, r.pmViewDesc = this
+            this.parent = e, this.children = t, this.dom = r, this.contentDOM = i, this.dirty = xe, r.pmViewDesc = this
         }
         matchesWidget(e) {
             return !1
         }
         matchesMark(e) {
             return !1
         }
@@ -5616,170 +4386,170 @@
         }
         get posAtEnd() {
             return this.posAtStart + this.size - 2 * this.border
         }
         localPosFromDOM(e, t, r) {
             if (this.contentDOM && this.contentDOM.contains(e.nodeType == 1 ? e : e.parentNode))
                 if (r < 0) {
-                    let o, s;
-                    if (e == this.contentDOM) o = e.childNodes[t - 1];
+                    let s, o;
+                    if (e == this.contentDOM) s = e.childNodes[t - 1];
                     else {
                         for (; e.parentNode != this.contentDOM;) e = e.parentNode;
-                        o = e.previousSibling
+                        s = e.previousSibling
                     }
-                    for (; o && !((s = o.pmViewDesc) && s.parent == this);) o = o.previousSibling;
-                    return o ? this.posBeforeChild(s) + s.size : this.posAtStart
+                    for (; s && !((o = s.pmViewDesc) && o.parent == this);) s = s.previousSibling;
+                    return s ? this.posBeforeChild(o) + o.size : this.posAtStart
                 } else {
-                    let o, s;
-                    if (e == this.contentDOM) o = e.childNodes[t];
+                    let s, o;
+                    if (e == this.contentDOM) s = e.childNodes[t];
                     else {
                         for (; e.parentNode != this.contentDOM;) e = e.parentNode;
-                        o = e.nextSibling
+                        s = e.nextSibling
                     }
-                    for (; o && !((s = o.pmViewDesc) && s.parent == this);) o = o.nextSibling;
-                    return o ? this.posBeforeChild(s) : this.posAtEnd
+                    for (; s && !((o = s.pmViewDesc) && o.parent == this);) s = s.nextSibling;
+                    return s ? this.posBeforeChild(o) : this.posAtEnd
                 } let i;
-            if (e == this.dom && this.contentDOM) i = t > Fe(this.contentDOM);
+            if (e == this.dom && this.contentDOM) i = t > be(this.contentDOM);
             else if (this.contentDOM && this.contentDOM != this.dom && this.dom.contains(this.contentDOM)) i = e.compareDocumentPosition(this.contentDOM) & 2;
             else if (this.dom.firstChild) {
                 if (t == 0)
-                    for (let o = e;; o = o.parentNode) {
-                        if (o == this.dom) {
+                    for (let s = e;; s = s.parentNode) {
+                        if (s == this.dom) {
                             i = !1;
                             break
                         }
-                        if (o.previousSibling) break
+                        if (s.previousSibling) break
                     }
                 if (i == null && t == e.childNodes.length)
-                    for (let o = e;; o = o.parentNode) {
-                        if (o == this.dom) {
+                    for (let s = e;; s = s.parentNode) {
+                        if (s == this.dom) {
                             i = !0;
                             break
                         }
-                        if (o.nextSibling) break
+                        if (s.nextSibling) break
                     }
             }
             return i ?? r > 0 ? this.posAtEnd : this.posAtStart
         }
         nearestDesc(e, t = !1) {
             for (let r = !0, i = e; i; i = i.parentNode) {
-                let o = this.getDesc(i),
-                    s;
-                if (o && (!t || o.node))
-                    if (r && (s = o.nodeDOM) && !(s.nodeType == 1 ? s.contains(e.nodeType == 1 ? e : e.parentNode) : s == e)) r = !1;
-                    else return o
+                let s = this.getDesc(i),
+                    o;
+                if (s && (!t || s.node))
+                    if (r && (o = s.nodeDOM) && !(o.nodeType == 1 ? o.contains(e.nodeType == 1 ? e : e.parentNode) : o == e)) r = !1;
+                    else return s
             }
         }
         getDesc(e) {
             let t = e.pmViewDesc;
             for (let r = t; r; r = r.parent)
                 if (r == this) return t
         }
         posFromDOM(e, t, r) {
             for (let i = e; i; i = i.parentNode) {
-                let o = this.getDesc(i);
-                if (o) return o.localPosFromDOM(e, t, r)
+                let s = this.getDesc(i);
+                if (s) return s.localPosFromDOM(e, t, r)
             }
             return -1
         }
         descAt(e) {
             for (let t = 0, r = 0; t < this.children.length; t++) {
                 let i = this.children[t],
-                    o = r + i.size;
-                if (r == e && o != r) {
+                    s = r + i.size;
+                if (r == e && s != r) {
                     for (; !i.border && i.children.length;) i = i.children[0];
                     return i
                 }
-                if (e < o) return i.descAt(e - r - i.border);
-                r = o
+                if (e < s) return i.descAt(e - r - i.border);
+                r = s
             }
         }
         domFromPos(e, t) {
             if (!this.contentDOM) return {
                 node: this.dom,
                 offset: 0,
                 atom: e + 1
             };
             let r = 0,
                 i = 0;
-            for (let o = 0; r < this.children.length; r++) {
-                let s = this.children[r],
-                    l = o + s.size;
-                if (l > e || s instanceof Qr) {
-                    i = e - o;
+            for (let s = 0; r < this.children.length; r++) {
+                let o = this.children[r],
+                    l = s + o.size;
+                if (l > e || o instanceof Xn) {
+                    i = e - s;
                     break
                 }
-                o = l
+                s = l
             }
             if (i) return this.children[r].domFromPos(i - this.children[r].border, t);
-            for (let o; r && !(o = this.children[r - 1]).size && o instanceof Yr && o.side >= 0; r--);
+            for (let s; r && !(s = this.children[r - 1]).size && s instanceof Yn && s.side >= 0; r--);
             if (t <= 0) {
-                let o, s = !0;
-                for (; o = r ? this.children[r - 1] : null, !(!o || o.dom.parentNode == this.contentDOM); r--, s = !1);
-                return o && t && s && !o.border && !o.domAtom ? o.domFromPos(o.size, t) : {
+                let s, o = !0;
+                for (; s = r ? this.children[r - 1] : null, !(!s || s.dom.parentNode == this.contentDOM); r--, o = !1);
+                return s && t && o && !s.border && !s.domAtom ? s.domFromPos(s.size, t) : {
                     node: this.contentDOM,
-                    offset: o ? Fe(o.dom) + 1 : 0
+                    offset: s ? be(s.dom) + 1 : 0
                 }
             } else {
-                let o, s = !0;
-                for (; o = r < this.children.length ? this.children[r] : null, !(!o || o.dom.parentNode == this.contentDOM); r++, s = !1);
-                return o && s && !o.border && !o.domAtom ? o.domFromPos(0, t) : {
+                let s, o = !0;
+                for (; s = r < this.children.length ? this.children[r] : null, !(!s || s.dom.parentNode == this.contentDOM); r++, o = !1);
+                return s && o && !s.border && !s.domAtom ? s.domFromPos(0, t) : {
                     node: this.contentDOM,
-                    offset: o ? Fe(o.dom) : this.contentDOM.childNodes.length
+                    offset: s ? be(s.dom) : this.contentDOM.childNodes.length
                 }
             }
         }
         parseRange(e, t, r = 0) {
             if (this.children.length == 0) return {
                 node: this.contentDOM,
                 from: e,
                 to: t,
                 fromOffset: 0,
                 toOffset: this.contentDOM.childNodes.length
             };
             let i = -1,
-                o = -1;
-            for (let s = r, l = 0;; l++) {
+                s = -1;
+            for (let o = r, l = 0;; l++) {
                 let a = this.children[l],
-                    c = s + a.size;
+                    c = o + a.size;
                 if (i == -1 && e <= c) {
-                    let u = s + a.border;
+                    let u = o + a.border;
                     if (e >= u && t <= c - a.border && a.node && a.contentDOM && this.contentDOM.contains(a.contentDOM)) return a.parseRange(e, t, u);
-                    e = s;
+                    e = o;
                     for (let d = l; d > 0; d--) {
                         let f = this.children[d - 1];
                         if (f.size && f.dom.parentNode == this.contentDOM && !f.emptyChildAt(1)) {
-                            i = Fe(f.dom) + 1;
+                            i = be(f.dom) + 1;
                             break
                         }
                         e -= f.size
                     }
                     i == -1 && (i = 0)
                 }
                 if (i > -1 && (c > t || l == this.children.length - 1)) {
                     t = c;
                     for (let u = l + 1; u < this.children.length; u++) {
                         let d = this.children[u];
                         if (d.size && d.dom.parentNode == this.contentDOM && !d.emptyChildAt(-1)) {
-                            o = Fe(d.dom);
+                            s = be(d.dom);
                             break
                         }
                         t += d.size
                     }
-                    o == -1 && (o = this.contentDOM.childNodes.length);
+                    s == -1 && (s = this.contentDOM.childNodes.length);
                     break
                 }
-                s = c
+                o = c
             }
             return {
                 node: this.contentDOM,
                 from: e,
                 to: t,
                 fromOffset: i,
-                toOffset: o
+                toOffset: s
             }
         }
         emptyChildAt(e) {
             if (this.border || !this.contentDOM || !this.children.length) return !1;
             let t = this.children[e < 0 ? 0 : this.children.length - 1];
             return t.size == 0 || t.emptyChildAt(e)
         }
@@ -5788,112 +4558,112 @@
                 node: t,
                 offset: r
             } = this.domFromPos(e, 0);
             if (t.nodeType != 1 || r == t.childNodes.length) throw new RangeError("No node after pos " + e);
             return t.childNodes[r]
         }
         setSelection(e, t, r, i = !1) {
-            let o = Math.min(e, t),
-                s = Math.max(e, t);
-            for (let f = 0, p = 0; f < this.children.length; f++) {
-                let h = this.children[f],
-                    m = p + h.size;
-                if (o > p && s < m) return h.setSelection(e - p - h.border, t - p - h.border, r, i);
-                p = m
+            let s = Math.min(e, t),
+                o = Math.max(e, t);
+            for (let f = 0, h = 0; f < this.children.length; f++) {
+                let p = this.children[f],
+                    m = h + p.size;
+                if (s > h && o < m) return p.setSelection(e - h - p.border, t - h - p.border, r, i);
+                h = m
             }
             let l = this.domFromPos(e, e ? -1 : 1),
                 a = t == e ? l : this.domFromPos(t, t ? -1 : 1),
                 c = r.getSelection(),
                 u = !1;
-            if ((_e || ve) && e == t) {
+            if ((we || oe) && e == t) {
                 let {
                     node: f,
-                    offset: p
+                    offset: h
                 } = l;
-                if (f.nodeType == 3) u = !!(p && f.nodeValue[p - 1] == `
+                if (f.nodeType == 3) u = !!(h && f.nodeValue[h - 1] == `
 `);
                 else {
-                    let h = f.childNodes[p - 1];
-                    u = h && (h.nodeName == "BR" || h.contentEditable == "false")
+                    let p = f.childNodes[h - 1];
+                    u = p && (p.nodeName == "BR" || p.contentEditable == "false")
                 }
             }
-            if (_e && c.focusNode && c.focusNode != a.node && c.focusNode.nodeType == 1) {
+            if (we && c.focusNode && c.focusNode != a.node && c.focusNode.nodeType == 1) {
                 let f = c.focusNode.childNodes[c.focusOffset];
                 f && f.contentEditable == "false" && (i = !0)
             }
-            if (!(i || u && ve) && hn(l.node, l.offset, c.anchorNode, c.anchorOffset) && hn(a.node, a.offset, c.focusNode, c.focusOffset)) return;
+            if (!(i || u && oe) && Ct(l.node, l.offset, c.anchorNode, c.anchorOffset) && Ct(a.node, a.offset, c.focusNode, c.focusOffset)) return;
             let d = !1;
             if ((c.extend || e == t) && !u) {
                 c.collapse(l.node, l.offset);
                 try {
                     e != t && c.extend(a.node, a.offset), d = !0
                 } catch {}
             }
             if (!d) {
                 if (e > t) {
-                    let p = l;
-                    l = a, a = p
+                    let h = l;
+                    l = a, a = h
                 }
                 let f = document.createRange();
                 f.setEnd(a.node, a.offset), f.setStart(l.node, l.offset), c.removeAllRanges(), c.addRange(f)
             }
         }
         ignoreMutation(e) {
             return !this.contentDOM && e.type != "selection"
         }
         get contentLost() {
             return this.contentDOM && this.contentDOM != this.dom && !this.dom.contains(this.contentDOM)
         }
         markDirty(e, t) {
             for (let r = 0, i = 0; i < this.children.length; i++) {
-                let o = this.children[i],
-                    s = r + o.size;
-                if (r == s ? e <= s && t >= r : e < s && t > r) {
-                    let l = r + o.border,
-                        a = s - o.border;
+                let s = this.children[i],
+                    o = r + s.size;
+                if (r == o ? e <= o && t >= r : e < o && t > r) {
+                    let l = r + s.border,
+                        a = o - s.border;
                     if (e >= l && t <= a) {
-                        this.dirty = e == r || t == s ? un : Ia, e == l && t == a && (o.contentLost || o.dom.parentNode != this.contentDOM) ? o.dirty = ot : o.markDirty(e - l, t - l);
+                        this.dirty = e == r || t == o ? St : $o, e == l && t == a && (s.contentLost || s.dom.parentNode != this.contentDOM) ? s.dirty = Le : s.markDirty(e - l, t - l);
                         return
-                    } else o.dirty = o.dom == o.contentDOM && o.dom.parentNode == this.contentDOM && !o.children.length ? un : ot
+                    } else s.dirty = s.dom == s.contentDOM && s.dom.parentNode == this.contentDOM && !s.children.length ? St : Le
                 }
-                r = s
+                r = o
             }
-            this.dirty = un
+            this.dirty = St
         }
         markParentsDirty() {
             let e = 1;
             for (let t = this.parent; t; t = t.parent, e++) {
-                let r = e == 1 ? un : Ia;
+                let r = e == 1 ? St : $o;
                 t.dirty < r && (t.dirty = r)
             }
         }
         get domAtom() {
             return !1
         }
         get ignoreForCoords() {
             return !1
         }
     },
-    Yr = class extends mn {
+    Yn = class extends At {
         constructor(e, t, r, i) {
-            let o, s = t.type.toDOM;
-            if (typeof s == "function" && (s = s(r, () => {
-                    if (!o) return i;
-                    if (o.parent) return o.parent.posBeforeChild(o)
+            let s, o = t.type.toDOM;
+            if (typeof o == "function" && (o = o(r, () => {
+                    if (!s) return i;
+                    if (s.parent) return s.parent.posBeforeChild(s)
                 })), !t.type.spec.raw) {
-                if (s.nodeType != 1) {
+                if (o.nodeType != 1) {
                     let l = document.createElement("span");
-                    l.appendChild(s), s = l
+                    l.appendChild(o), o = l
                 }
-                s.contentEditable = "false", s.classList.add("ProseMirror-widget")
+                o.contentEditable = "false", o.classList.add("ProseMirror-widget")
             }
-            super(e, [], s, null), this.widget = t, this.widget = t, o = this
+            super(e, [], o, null), this.widget = t, this.widget = t, s = this
         }
         matchesWidget(e) {
-            return this.dirty == je && e.type.eq(this.widget.type)
+            return this.dirty == xe && e.type.eq(this.widget.type)
         }
         parseRule() {
             return {
                 ignore: !0
             }
         }
         stopEvent(e) {
@@ -5909,15 +4679,15 @@
         get domAtom() {
             return !0
         }
         get side() {
             return this.widget.type.side
         }
     },
-    Io = class extends mn {
+    mi = class extends At {
         constructor(e, t, r, i) {
             super(e, [], t, null), this.textDOM = r, this.text = i
         }
         get size() {
             return this.text.length
         }
         localPosFromDOM(e, t) {
@@ -5929,71 +4699,71 @@
                 offset: e
             }
         }
         ignoreMutation(e) {
             return e.type === "characterData" && e.target.nodeValue == e.oldValue
         }
     },
-    kt = class extends mn {
+    We = class extends At {
         constructor(e, t, r, i) {
             super(e, [], r, i), this.mark = t
         }
         static create(e, t, r, i) {
-            let o = i.nodeViews[t.type.name],
-                s = o && o(t, i, r);
-            return (!s || !s.dom) && (s = Se.renderSpec(document, t.type.spec.toDOM(t, r))), new kt(e, t, s.dom, s.contentDOM || s.dom)
+            let s = i.nodeViews[t.type.name],
+                o = s && s(t, i, r);
+            return (!o || !o.dom) && (o = ce.renderSpec(document, t.type.spec.toDOM(t, r))), new We(e, t, o.dom, o.contentDOM || o.dom)
         }
         parseRule() {
-            return this.dirty & ot || this.mark.type.spec.reparseInView ? null : {
+            return this.dirty & Le || this.mark.type.spec.reparseInView ? null : {
                 mark: this.mark.type.name,
                 attrs: this.mark.attrs,
                 contentElement: this.contentDOM || void 0
             }
         }
         matchesMark(e) {
-            return this.dirty != ot && this.mark.eq(e)
+            return this.dirty != Le && this.mark.eq(e)
         }
         markDirty(e, t) {
-            if (super.markDirty(e, t), this.dirty != je) {
+            if (super.markDirty(e, t), this.dirty != xe) {
                 let r = this.parent;
                 for (; !r.node;) r = r.parent;
-                r.dirty < this.dirty && (r.dirty = this.dirty), this.dirty = je
+                r.dirty < this.dirty && (r.dirty = this.dirty), this.dirty = xe
             }
         }
         slice(e, t, r) {
-            let i = kt.create(this.parent, this.mark, !0, r),
-                o = this.children,
-                s = this.size;
-            t < s && (o = Bo(o, t, s, r)), e > 0 && (o = Bo(o, 0, e, r));
-            for (let l = 0; l < o.length; l++) o[l].parent = i;
-            return i.children = o, i
-        }
-    },
-    nt = class extends mn {
-        constructor(e, t, r, i, o, s, l, a, c) {
-            super(e, [], o, s), this.node = t, this.outerDeco = r, this.innerDeco = i, this.nodeDOM = l
-        }
-        static create(e, t, r, i, o, s) {
-            let l = o.nodeViews[t.type.name],
-                a, c = l && l(t, o, () => {
-                    if (!a) return s;
+            let i = We.create(this.parent, this.mark, !0, r),
+                s = this.children,
+                o = this.size;
+            t < o && (s = ki(s, t, o, r)), e > 0 && (s = ki(s, 0, e, r));
+            for (let l = 0; l < s.length; l++) s[l].parent = i;
+            return i.children = s, i
+        }
+    },
+    Ne = class extends At {
+        constructor(e, t, r, i, s, o, l, a, c) {
+            super(e, [], s, o), this.node = t, this.outerDeco = r, this.innerDeco = i, this.nodeDOM = l
+        }
+        static create(e, t, r, i, s, o) {
+            let l = s.nodeViews[t.type.name],
+                a, c = l && l(t, s, () => {
+                    if (!a) return o;
                     if (a.parent) return a.parent.posBeforeChild(a)
                 }, r, i),
                 u = c && c.dom,
                 d = c && c.contentDOM;
             if (t.isText) {
                 if (!u) u = document.createTextNode(t.text);
                 else if (u.nodeType != 3) throw new RangeError("Text must be rendered as a DOM text node")
             } else u || ({
                 dom: u,
                 contentDOM: d
-            } = Se.renderSpec(document, t.type.spec.toDOM(t)));
+            } = ce.renderSpec(document, t.type.spec.toDOM(t)));
             !d && !t.isText && u.nodeName != "BR" && (u.hasAttribute("contenteditable") || (u.contentEditable = "false"), t.type.spec.draggable && (u.draggable = !0));
             let f = u;
-            return u = uc(u, r, t), c ? a = new Do(e, t, r, i, u, d || null, f, c, o, s + 1) : t.isText ? new Fn(e, t, r, i, u, f, o) : new nt(e, t, r, i, u, d || null, f, o, s + 1)
+            return u = kl(u, r, t), c ? a = new gi(e, t, r, i, u, d || null, f, c, s, o + 1) : t.isText ? new Kt(e, t, r, i, u, f, s) : new Ne(e, t, r, i, u, d || null, f, s, o + 1)
         }
         parseRule() {
             if (this.node.type.spec.reparseInView) return null;
             let e = {
                 node: this.node.type.name,
                 attrs: this.node.attrs
             };
@@ -6003,121 +4773,121 @@
                 for (let t = this.children.length - 1; t >= 0; t--) {
                     let r = this.children[t];
                     if (this.dom.contains(r.dom.parentNode)) {
                         e.contentElement = r.dom.parentNode;
                         break
                     }
                 }
-                e.contentElement || (e.getContent = () => v.empty)
+                e.contentElement || (e.getContent = () => x.empty)
             }
             return e
         }
         matchesNode(e, t, r) {
-            return this.dirty == je && e.eq(this.node) && Po(t, this.outerDeco) && r.eq(this.innerDeco)
+            return this.dirty == xe && e.eq(this.node) && bi(t, this.outerDeco) && r.eq(this.innerDeco)
         }
         get size() {
             return this.node.nodeSize
         }
         get border() {
             return this.node.isLeaf ? 0 : 1
         }
         updateChildren(e, t) {
             let r = this.node.inlineContent,
                 i = t,
-                o = e.composing ? this.localCompositionInfo(e, t) : null,
-                s = o && o.pos > -1 ? o : null,
-                l = o && o.pos < 0,
-                a = new Ro(this, s && s.node, e);
-            cp(this.node, this.innerDeco, (c, u, d) => {
-                c.spec.marks ? a.syncToMarks(c.spec.marks, r, e) : c.type.side >= 0 && !d && a.syncToMarks(u == this.node.childCount ? H.none : this.node.child(u).marks, r, e), a.placeWidget(c, e, i)
+                s = e.composing ? this.localCompositionInfo(e, t) : null,
+                o = s && s.pos > -1 ? s : null,
+                l = s && s.pos < 0,
+                a = new xi(this, o && o.node, e);
+            Lu(this.node, this.innerDeco, (c, u, d) => {
+                c.spec.marks ? a.syncToMarks(c.spec.marks, r, e) : c.type.side >= 0 && !d && a.syncToMarks(u == this.node.childCount ? B.none : this.node.child(u).marks, r, e), a.placeWidget(c, e, i)
             }, (c, u, d, f) => {
                 a.syncToMarks(c.marks, r, e);
-                let p;
-                a.findNodeMatch(c, u, d, f) || l && e.state.selection.from > i && e.state.selection.to < i + c.nodeSize && (p = a.findIndexWithChild(o.node)) > -1 && a.updateNodeAt(c, u, d, p, e) || a.updateNextNode(c, u, d, e, f, i) || a.addNode(c, u, d, e, i), i += c.nodeSize
-            }), a.syncToMarks([], r, e), this.node.isTextblock && a.addTextblockHacks(), a.destroyRest(), (a.changed || this.dirty == un) && (s && this.protectLocalComposition(e, s), ac(this.contentDOM, this.children, e), Hn && up(this.dom))
+                let h;
+                a.findNodeMatch(c, u, d, f) || l && e.state.selection.from > i && e.state.selection.to < i + c.nodeSize && (h = a.findIndexWithChild(s.node)) > -1 && a.updateNodeAt(c, u, d, h, e) || a.updateNextNode(c, u, d, e, f, i) || a.addNode(c, u, d, e, i), i += c.nodeSize
+            }), a.syncToMarks([], r, e), this.node.isTextblock && a.addTextblockHacks(), a.destroyRest(), (a.changed || this.dirty == St) && (o && this.protectLocalComposition(e, o), bl(this.contentDOM, this.children, e), qt && Ru(this.dom))
         }
         localCompositionInfo(e, t) {
             let {
                 from: r,
                 to: i
             } = e.state.selection;
-            if (!(e.state.selection instanceof P) || r < t || i > t + this.node.content.size) return null;
-            let o = e.domSelectionRange(),
-                s = dp(o.focusNode, o.focusOffset);
-            if (!s || !this.dom.contains(s.parentNode)) return null;
+            if (!(e.state.selection instanceof I) || r < t || i > t + this.node.content.size) return null;
+            let s = e.domSelectionRange(),
+                o = Pu(s.focusNode, s.focusOffset);
+            if (!o || !this.dom.contains(o.parentNode)) return null;
             if (this.node.inlineContent) {
-                let l = s.nodeValue,
-                    a = fp(this.node.content, l, r - t, i - t);
+                let l = o.nodeValue,
+                    a = Bu(this.node.content, l, r - t, i - t);
                 return a < 0 ? null : {
-                    node: s,
+                    node: o,
                     pos: a,
                     text: l
                 }
             } else return {
-                node: s,
+                node: o,
                 pos: -1,
                 text: ""
             }
         }
         protectLocalComposition(e, {
             node: t,
             pos: r,
             text: i
         }) {
             if (this.getDesc(t)) return;
-            let o = t;
-            for (; o.parentNode != this.contentDOM; o = o.parentNode) {
-                for (; o.previousSibling;) o.parentNode.removeChild(o.previousSibling);
-                for (; o.nextSibling;) o.parentNode.removeChild(o.nextSibling);
-                o.pmViewDesc && (o.pmViewDesc = void 0)
+            let s = t;
+            for (; s.parentNode != this.contentDOM; s = s.parentNode) {
+                for (; s.previousSibling;) s.parentNode.removeChild(s.previousSibling);
+                for (; s.nextSibling;) s.parentNode.removeChild(s.nextSibling);
+                s.pmViewDesc && (s.pmViewDesc = void 0)
             }
-            let s = new Io(this, o, t, i);
-            e.input.compositionNodes.push(s), this.children = Bo(this.children, r, r + i.length, e, s)
+            let o = new mi(this, s, t, i);
+            e.input.compositionNodes.push(o), this.children = ki(this.children, r, r + i.length, e, o)
         }
         update(e, t, r, i) {
-            return this.dirty == ot || !e.sameMarkup(this.node) ? !1 : (this.updateInner(e, t, r, i), !0)
+            return this.dirty == Le || !e.sameMarkup(this.node) ? !1 : (this.updateInner(e, t, r, i), !0)
         }
         updateInner(e, t, r, i) {
-            this.updateOuterDeco(t), this.node = e, this.innerDeco = r, this.contentDOM && this.updateChildren(i, this.posAtStart), this.dirty = je
+            this.updateOuterDeco(t), this.node = e, this.innerDeco = r, this.contentDOM && this.updateChildren(i, this.posAtStart), this.dirty = xe
         }
         updateOuterDeco(e) {
-            if (Po(e, this.outerDeco)) return;
+            if (bi(e, this.outerDeco)) return;
             let t = this.nodeDOM.nodeType != 1,
                 r = this.dom;
-            this.dom = cc(this.dom, this.nodeDOM, Lo(this.outerDeco, this.node, t), Lo(e, this.node, t)), this.dom != r && (r.pmViewDesc = void 0, this.dom.pmViewDesc = this), this.outerDeco = e
+            this.dom = xl(this.dom, this.nodeDOM, yi(this.outerDeco, this.node, t), yi(e, this.node, t)), this.dom != r && (r.pmViewDesc = void 0, this.dom.pmViewDesc = this), this.outerDeco = e
         }
         selectNode() {
             this.nodeDOM.nodeType == 1 && this.nodeDOM.classList.add("ProseMirror-selectednode"), (this.contentDOM || !this.node.type.spec.draggable) && (this.dom.draggable = !0)
         }
         deselectNode() {
             this.nodeDOM.nodeType == 1 && this.nodeDOM.classList.remove("ProseMirror-selectednode"), (this.contentDOM || !this.node.type.spec.draggable) && this.dom.removeAttribute("draggable")
         }
         get domAtom() {
             return this.node.isAtom
         }
     };
 
-function Da(n, e, t, r, i) {
-    uc(r, e, n);
-    let o = new nt(void 0, n, e, t, r, r, r, i, 0);
-    return o.contentDOM && o.updateChildren(i, 0), o
-}
-var Fn = class extends nt {
-        constructor(e, t, r, i, o, s, l) {
-            super(e, t, r, i, o, null, s, l, 0)
+function Vo(n, e, t, r, i) {
+    kl(r, e, n);
+    let s = new Ne(void 0, n, e, t, r, r, r, i, 0);
+    return s.contentDOM && s.updateChildren(i, 0), s
+}
+var Kt = class extends Ne {
+        constructor(e, t, r, i, s, o, l) {
+            super(e, t, r, i, s, null, o, l, 0)
         }
         parseRule() {
             let e = this.nodeDOM.parentNode;
             for (; e && e != this.dom && !e.pmIsDeco;) e = e.parentNode;
             return {
                 skip: e || !0
             }
         }
         update(e, t, r, i) {
-            return this.dirty == ot || this.dirty != je && !this.inParent() || !e.sameMarkup(this.node) ? !1 : (this.updateOuterDeco(t), (this.dirty != je || e.text != this.node.text) && e.text != this.nodeDOM.nodeValue && (this.nodeDOM.nodeValue = e.text, i.trackWrites == this.nodeDOM && (i.trackWrites = null)), this.node = e, this.dirty = je, !0)
+            return this.dirty == Le || this.dirty != xe && !this.inParent() || !e.sameMarkup(this.node) ? !1 : (this.updateOuterDeco(t), (this.dirty != xe || e.text != this.node.text) && e.text != this.nodeDOM.nodeValue && (this.nodeDOM.nodeValue = e.text, i.trackWrites == this.nodeDOM && (i.trackWrites = null)), this.node = e, this.dirty = xe, !0)
         }
         inParent() {
             let e = this.parent.contentDOM;
             for (let t = this.nodeDOM; t; t = t.parentNode)
                 if (t == e) return !0;
             return !1
         }
@@ -6131,49 +4901,49 @@
             return e == this.nodeDOM ? this.posAtStart + Math.min(t, this.node.text.length) : super.localPosFromDOM(e, t, r)
         }
         ignoreMutation(e) {
             return e.type != "characterData" && e.type != "selection"
         }
         slice(e, t, r) {
             let i = this.node.cut(e, t),
-                o = document.createTextNode(i.text);
-            return new Fn(this.parent, i, this.outerDeco, this.innerDeco, o, o, r)
+                s = document.createTextNode(i.text);
+            return new Kt(this.parent, i, this.outerDeco, this.innerDeco, s, s, r)
         }
         markDirty(e, t) {
-            super.markDirty(e, t), this.dom != this.nodeDOM && (e == 0 || t == this.nodeDOM.nodeValue.length) && (this.dirty = ot)
+            super.markDirty(e, t), this.dom != this.nodeDOM && (e == 0 || t == this.nodeDOM.nodeValue.length) && (this.dirty = Le)
         }
         get domAtom() {
             return !1
         }
     },
-    Qr = class extends mn {
+    Xn = class extends At {
         parseRule() {
             return {
                 ignore: !0
             }
         }
         matchesHack(e) {
-            return this.dirty == je && this.dom.nodeName == e
+            return this.dirty == xe && this.dom.nodeName == e
         }
         get domAtom() {
             return !0
         }
         get ignoreForCoords() {
             return this.dom.nodeName == "IMG"
         }
     },
-    Do = class extends nt {
-        constructor(e, t, r, i, o, s, l, a, c, u) {
-            super(e, t, r, i, o, s, l, c, u), this.spec = a
+    gi = class extends Ne {
+        constructor(e, t, r, i, s, o, l, a, c, u) {
+            super(e, t, r, i, s, o, l, c, u), this.spec = a
         }
         update(e, t, r, i) {
-            if (this.dirty == ot) return !1;
+            if (this.dirty == Le) return !1;
             if (this.spec.update) {
-                let o = this.spec.update(e, t, r);
-                return o && this.updateInner(e, t, r, i), o
+                let s = this.spec.update(e, t, r);
+                return s && this.updateInner(e, t, r, i), s
             } else return !this.contentDOM && !e.isLeaf ? !1 : super.update(e, t, r, i)
         }
         selectNode() {
             this.spec.selectNode ? this.spec.selectNode() : super.selectNode()
         }
         deselectNode() {
             this.spec.deselectNode ? this.spec.deselectNode() : super.deselectNode()
@@ -6188,159 +4958,159 @@
             return this.spec.stopEvent ? this.spec.stopEvent(e) : !1
         }
         ignoreMutation(e) {
             return this.spec.ignoreMutation ? this.spec.ignoreMutation(e) : super.ignoreMutation(e)
         }
     };
 
-function ac(n, e, t) {
+function bl(n, e, t) {
     let r = n.firstChild,
         i = !1;
-    for (let o = 0; o < e.length; o++) {
-        let s = e[o],
-            l = s.dom;
+    for (let s = 0; s < e.length; s++) {
+        let o = e[s],
+            l = o.dom;
         if (l.parentNode == n) {
-            for (; l != r;) r = La(r), i = !0;
+            for (; l != r;) r = Jo(r), i = !0;
             r = r.nextSibling
         } else i = !0, n.insertBefore(l, r);
-        if (s instanceof kt) {
+        if (o instanceof We) {
             let a = r ? r.previousSibling : n.lastChild;
-            ac(s.contentDOM, s.children, t), r = a ? a.nextSibling : n.firstChild
+            bl(o.contentDOM, o.children, t), r = a ? a.nextSibling : n.firstChild
         }
     }
-    for (; r;) r = La(r), i = !0;
+    for (; r;) r = Jo(r), i = !0;
     i && t.trackWrites == n && (t.trackWrites = null)
 }
-var gr = function(n) {
+var bn = function(n) {
     n && (this.nodeName = n)
 };
-gr.prototype = Object.create(null);
-var dn = [new gr];
+bn.prototype = Object.create(null);
+var Et = [new bn];
 
-function Lo(n, e, t) {
-    if (n.length == 0) return dn;
-    let r = t ? dn[0] : new gr,
+function yi(n, e, t) {
+    if (n.length == 0) return Et;
+    let r = t ? Et[0] : new bn,
         i = [r];
-    for (let o = 0; o < n.length; o++) {
-        let s = n[o].type.attrs;
-        if (s) {
-            s.nodeName && i.push(r = new gr(s.nodeName));
-            for (let l in s) {
-                let a = s[l];
-                a != null && (t && i.length == 1 && i.push(r = new gr(e.isInline ? "span" : "div")), l == "class" ? r.class = (r.class ? r.class + " " : "") + a : l == "style" ? r.style = (r.style ? r.style + ";" : "") + a : l != "nodeName" && (r[l] = a))
+    for (let s = 0; s < n.length; s++) {
+        let o = n[s].type.attrs;
+        if (o) {
+            o.nodeName && i.push(r = new bn(o.nodeName));
+            for (let l in o) {
+                let a = o[l];
+                a != null && (t && i.length == 1 && i.push(r = new bn(e.isInline ? "span" : "div")), l == "class" ? r.class = (r.class ? r.class + " " : "") + a : l == "style" ? r.style = (r.style ? r.style + ";" : "") + a : l != "nodeName" && (r[l] = a))
             }
         }
     }
     return i
 }
 
-function cc(n, e, t, r) {
-    if (t == dn && r == dn) return e;
+function xl(n, e, t, r) {
+    if (t == Et && r == Et) return e;
     let i = e;
-    for (let o = 0; o < r.length; o++) {
-        let s = r[o],
-            l = t[o];
-        if (o) {
+    for (let s = 0; s < r.length; s++) {
+        let o = r[s],
+            l = t[s];
+        if (s) {
             let a;
-            l && l.nodeName == s.nodeName && i != n && (a = i.parentNode) && a.nodeName.toLowerCase() == s.nodeName || (a = document.createElement(s.nodeName), a.pmIsDeco = !0, a.appendChild(i), l = dn[0]), i = a
+            l && l.nodeName == o.nodeName && i != n && (a = i.parentNode) && a.nodeName.toLowerCase() == o.nodeName || (a = document.createElement(o.nodeName), a.pmIsDeco = !0, a.appendChild(i), l = Et[0]), i = a
         }
-        sp(i, l || dn[0], s)
+        Nu(i, l || Et[0], o)
     }
     return i
 }
 
-function sp(n, e, t) {
+function Nu(n, e, t) {
     for (let r in e) r != "class" && r != "style" && r != "nodeName" && !(r in t) && n.removeAttribute(r);
     for (let r in t) r != "class" && r != "style" && r != "nodeName" && t[r] != e[r] && n.setAttribute(r, t[r]);
     if (e.class != t.class) {
         let r = e.class ? e.class.split(" ").filter(Boolean) : [],
             i = t.class ? t.class.split(" ").filter(Boolean) : [];
-        for (let o = 0; o < r.length; o++) i.indexOf(r[o]) == -1 && n.classList.remove(r[o]);
-        for (let o = 0; o < i.length; o++) r.indexOf(i[o]) == -1 && n.classList.add(i[o]);
+        for (let s = 0; s < r.length; s++) i.indexOf(r[s]) == -1 && n.classList.remove(r[s]);
+        for (let s = 0; s < i.length; s++) r.indexOf(i[s]) == -1 && n.classList.add(i[s]);
         n.classList.length == 0 && n.removeAttribute("class")
     }
     if (e.style != t.style) {
         if (e.style) {
             let r = /\s*([\w\-\xa1-\uffff]+)\s*:(?:"(?:\\.|[^"])*"|'(?:\\.|[^'])*'|\(.*?\)|[^;])*/g,
                 i;
             for (; i = r.exec(e.style);) n.style.removeProperty(i[1])
         }
         t.style && (n.style.cssText += t.style)
     }
 }
 
-function uc(n, e, t) {
-    return cc(n, n, dn, Lo(e, t, n.nodeType != 1))
+function kl(n, e, t) {
+    return xl(n, n, Et, yi(e, t, n.nodeType != 1))
 }
 
-function Po(n, e) {
+function bi(n, e) {
     if (n.length != e.length) return !1;
     for (let t = 0; t < n.length; t++)
         if (!n[t].type.eq(e[t].type)) return !1;
     return !0
 }
 
-function La(n) {
+function Jo(n) {
     let e = n.nextSibling;
     return n.parentNode.removeChild(n), e
 }
-var Ro = class {
+var xi = class {
     constructor(e, t, r) {
-        this.lock = t, this.view = r, this.index = 0, this.stack = [], this.changed = !1, this.top = e, this.preMatch = lp(e.node.content, e)
+        this.lock = t, this.view = r, this.index = 0, this.stack = [], this.changed = !1, this.top = e, this.preMatch = Iu(e.node.content, e)
     }
     destroyBetween(e, t) {
         if (e != t) {
             for (let r = e; r < t; r++) this.top.children[r].destroy();
             this.top.children.splice(e, t - e), this.changed = !0
         }
     }
     destroyRest() {
         this.destroyBetween(this.index, this.top.children.length)
     }
     syncToMarks(e, t, r) {
         let i = 0,
-            o = this.stack.length >> 1,
-            s = Math.min(o, e.length);
-        for (; i < s && (i == o - 1 ? this.top : this.stack[i + 1 << 1]).matchesMark(e[i]) && e[i].type.spec.spanning !== !1;) i++;
-        for (; i < o;) this.destroyRest(), this.top.dirty = je, this.index = this.stack.pop(), this.top = this.stack.pop(), o--;
-        for (; o < e.length;) {
+            s = this.stack.length >> 1,
+            o = Math.min(s, e.length);
+        for (; i < o && (i == s - 1 ? this.top : this.stack[i + 1 << 1]).matchesMark(e[i]) && e[i].type.spec.spanning !== !1;) i++;
+        for (; i < s;) this.destroyRest(), this.top.dirty = xe, this.index = this.stack.pop(), this.top = this.stack.pop(), s--;
+        for (; s < e.length;) {
             this.stack.push(this.top, this.index + 1);
             let l = -1;
             for (let a = this.index; a < Math.min(this.index + 3, this.top.children.length); a++) {
                 let c = this.top.children[a];
-                if (c.matchesMark(e[o]) && !this.isLocked(c.dom)) {
+                if (c.matchesMark(e[s]) && !this.isLocked(c.dom)) {
                     l = a;
                     break
                 }
             }
             if (l > -1) l > this.index && (this.changed = !0, this.destroyBetween(this.index, l)), this.top = this.top.children[this.index];
             else {
-                let a = kt.create(this.top, e[o], t, r);
+                let a = We.create(this.top, e[s], t, r);
                 this.top.children.splice(this.index, 0, a), this.top = a, this.changed = !0
             }
-            this.index = 0, o++
+            this.index = 0, s++
         }
     }
     findNodeMatch(e, t, r, i) {
-        let o = -1,
-            s;
-        if (i >= this.preMatch.index && (s = this.preMatch.matches[i - this.preMatch.index]).parent == this.top && s.matchesNode(e, t, r)) o = this.top.children.indexOf(s, this.index);
+        let s = -1,
+            o;
+        if (i >= this.preMatch.index && (o = this.preMatch.matches[i - this.preMatch.index]).parent == this.top && o.matchesNode(e, t, r)) s = this.top.children.indexOf(o, this.index);
         else
             for (let l = this.index, a = Math.min(this.top.children.length, l + 5); l < a; l++) {
                 let c = this.top.children[l];
                 if (c.matchesNode(e, t, r) && !this.preMatch.matched.has(c)) {
-                    o = l;
+                    s = l;
                     break
                 }
             }
-        return o < 0 ? !1 : (this.destroyBetween(this.index, o), this.index++, !0)
+        return s < 0 ? !1 : (this.destroyBetween(this.index, s), this.index++, !0)
     }
-    updateNodeAt(e, t, r, i, o) {
-        let s = this.top.children[i];
-        return s.dirty == ot && s.dom == s.contentDOM && (s.dirty = un), s.update(e, t, r, o) ? (this.destroyBetween(this.index, i), this.index++, !0) : !1
+    updateNodeAt(e, t, r, i, s) {
+        let o = this.top.children[i];
+        return o.dirty == Le && o.dom == o.contentDOM && (o.dirty = St), o.update(e, t, r, s) ? (this.destroyBetween(this.index, i), this.index++, !0) : !1
     }
     findIndexWithChild(e) {
         for (;;) {
             let t = e.parentNode;
             if (!t) return -1;
             if (t == this.top.contentDOM) {
                 let r = e.pmViewDesc;
@@ -6349,1620 +5119,1620 @@
                         if (this.top.children[i] == r) return i
                 }
                 return -1
             }
             e = t
         }
     }
-    updateNextNode(e, t, r, i, o, s) {
+    updateNextNode(e, t, r, i, s, o) {
         for (let l = this.index; l < this.top.children.length; l++) {
             let a = this.top.children[l];
-            if (a instanceof nt) {
+            if (a instanceof Ne) {
                 let c = this.preMatch.matched.get(a);
-                if (c != null && c != o) return !1;
+                if (c != null && c != s) return !1;
                 let u = a.dom,
-                    d, f = this.isLocked(u) && !(e.isText && a.node && a.node.isText && a.nodeDOM.nodeValue == e.text && a.dirty != ot && Po(t, a.outerDeco));
+                    d, f = this.isLocked(u) && !(e.isText && a.node && a.node.isText && a.nodeDOM.nodeValue == e.text && a.dirty != Le && bi(t, a.outerDeco));
                 if (!f && a.update(e, t, r, i)) return this.destroyBetween(this.index, l), a.dom != u && (this.changed = !0), this.index++, !0;
-                if (!f && (d = this.recreateWrapper(a, e, t, r, i, s))) return this.top.children[this.index] = d, d.dirty = un, d.updateChildren(i, s + 1), d.dirty = je, this.changed = !0, this.index++, !0;
+                if (!f && (d = this.recreateWrapper(a, e, t, r, i, o))) return this.top.children[this.index] = d, d.dirty = St, d.updateChildren(i, o + 1), d.dirty = xe, this.changed = !0, this.index++, !0;
                 break
             }
         }
         return !1
     }
-    recreateWrapper(e, t, r, i, o, s) {
+    recreateWrapper(e, t, r, i, s, o) {
         if (e.dirty || t.isAtom || !e.children.length || !e.node.content.eq(t.content)) return null;
-        let l = nt.create(this.top, t, r, i, o, s);
+        let l = Ne.create(this.top, t, r, i, s, o);
         if (!l.contentDOM) return null;
         l.children = e.children, e.children = [];
         for (let a of l.children) a.parent = l;
         return l
     }
-    addNode(e, t, r, i, o) {
-        let s = nt.create(this.top, e, t, r, i, o);
-        s.contentDOM && s.updateChildren(i, o + 1), this.top.children.splice(this.index++, 0, s), this.changed = !0
+    addNode(e, t, r, i, s) {
+        let o = Ne.create(this.top, e, t, r, i, s);
+        o.contentDOM && o.updateChildren(i, s + 1), this.top.children.splice(this.index++, 0, o), this.changed = !0
     }
     placeWidget(e, t, r) {
         let i = this.index < this.top.children.length ? this.top.children[this.index] : null;
         if (i && i.matchesWidget(e) && (e == i.widget || !i.widget.type.toDOM.parentNode)) this.index++;
         else {
-            let o = new Yr(this.top, e, t, r);
-            this.top.children.splice(this.index++, 0, o), this.changed = !0
+            let s = new Yn(this.top, e, t, r);
+            this.top.children.splice(this.index++, 0, s), this.changed = !0
         }
     }
     addTextblockHacks() {
         let e = this.top.children[this.index - 1],
             t = this.top;
-        for (; e instanceof kt;) t = e, e = t.children[t.children.length - 1];
-        (!e || !(e instanceof Fn) || /\n$/.test(e.node.text) || this.view.requiresGeckoHackNode && /\s$/.test(e.node.text)) && ((ve || ye) && e && e.dom.contentEditable == "false" && this.addHackNode("IMG", t), this.addHackNode("BR", this.top))
+        for (; e instanceof We;) t = e, e = t.children[t.children.length - 1];
+        (!e || !(e instanceof Kt) || /\n$/.test(e.node.text) || this.view.requiresGeckoHackNode && /\s$/.test(e.node.text)) && ((oe || ie) && e && e.dom.contentEditable == "false" && this.addHackNode("IMG", t), this.addHackNode("BR", this.top))
     }
     addHackNode(e, t) {
         if (t == this.top && this.index < t.children.length && t.children[this.index].matchesHack(e)) this.index++;
         else {
             let r = document.createElement(e);
             e == "IMG" && (r.className = "ProseMirror-separator", r.alt = ""), e == "BR" && (r.className = "ProseMirror-trailingBreak");
-            let i = new Qr(this.top, [], r, null);
+            let i = new Xn(this.top, [], r, null);
             t != this.top ? t.children.push(i) : t.children.splice(this.index++, 0, i), this.changed = !0
         }
     }
     isLocked(e) {
         return this.lock && (e == this.lock || e.nodeType == 1 && e.contains(this.lock.parentNode))
     }
 };
 
-function lp(n, e) {
+function Iu(n, e) {
     let t = e,
         r = t.children.length,
         i = n.childCount,
-        o = new Map,
-        s = [];
+        s = new Map,
+        o = [];
     e: for (; i > 0;) {
         let l;
         for (;;)
             if (r) {
                 let c = t.children[r - 1];
-                if (c instanceof kt) t = c, r = c.children.length;
+                if (c instanceof We) t = c, r = c.children.length;
                 else {
                     l = c, r--;
                     break
                 }
             } else {
                 if (t == e) break e;
                 r = t.parent.children.indexOf(t), t = t.parent
             } let a = l.node;
         if (a) {
             if (a != n.child(i - 1)) break;
-            --i, o.set(l, i), s.push(l)
+            --i, s.set(l, i), o.push(l)
         }
     }
     return {
         index: i,
-        matched: o,
-        matches: s.reverse()
+        matched: s,
+        matches: o.reverse()
     }
 }
 
-function ap(n, e) {
+function Du(n, e) {
     return n.type.side - e.type.side
 }
 
-function cp(n, e, t, r) {
+function Lu(n, e, t, r) {
     let i = e.locals(n),
-        o = 0;
+        s = 0;
     if (i.length == 0) {
         for (let c = 0; c < n.childCount; c++) {
             let u = n.child(c);
-            r(u, i, e.forChild(o, u), c), o += u.nodeSize
+            r(u, i, e.forChild(s, u), c), s += u.nodeSize
         }
         return
     }
-    let s = 0,
+    let o = 0,
         l = [],
         a = null;
     for (let c = 0;;) {
-        if (s < i.length && i[s].to == o) {
-            let h = i[s++],
+        if (o < i.length && i[o].to == s) {
+            let p = i[o++],
                 m;
-            for (; s < i.length && i[s].to == o;)(m || (m = [h])).push(i[s++]);
+            for (; o < i.length && i[o].to == s;)(m || (m = [p])).push(i[o++]);
             if (m) {
-                m.sort(ap);
+                m.sort(Du);
                 for (let b = 0; b < m.length; b++) t(m[b], c, !!a)
-            } else t(h, c, !!a)
+            } else t(p, c, !!a)
         }
         let u, d;
         if (a) d = -1, u = a, a = null;
         else if (c < n.childCount) d = c, u = n.child(c++);
         else break;
-        for (let h = 0; h < l.length; h++) l[h].to <= o && l.splice(h--, 1);
-        for (; s < i.length && i[s].from <= o && i[s].to > o;) l.push(i[s++]);
-        let f = o + u.nodeSize;
+        for (let p = 0; p < l.length; p++) l[p].to <= s && l.splice(p--, 1);
+        for (; o < i.length && i[o].from <= s && i[o].to > s;) l.push(i[o++]);
+        let f = s + u.nodeSize;
         if (u.isText) {
-            let h = f;
-            s < i.length && i[s].from < h && (h = i[s].from);
-            for (let m = 0; m < l.length; m++) l[m].to < h && (h = l[m].to);
-            h < f && (a = u.cut(h - o), u = u.cut(0, h - o), f = h, d = -1)
+            let p = f;
+            o < i.length && i[o].from < p && (p = i[o].from);
+            for (let m = 0; m < l.length; m++) l[m].to < p && (p = l[m].to);
+            p < f && (a = u.cut(p - s), u = u.cut(0, p - s), f = p, d = -1)
         }
-        let p = u.isInline && !u.isLeaf ? l.filter(h => !h.inline) : l.slice();
-        r(u, p, e.forChild(o, u), d), o = f
+        let h = u.isInline && !u.isLeaf ? l.filter(p => !p.inline) : l.slice();
+        r(u, h, e.forChild(s, u), d), s = f
     }
 }
 
-function up(n) {
+function Ru(n) {
     if (n.nodeName == "UL" || n.nodeName == "OL") {
         let e = n.style.cssText;
         n.style.cssText = e + "; list-style: square !important", window.getComputedStyle(n).listStyle, n.style.cssText = e
     }
 }
 
-function dp(n, e) {
+function Pu(n, e) {
     for (;;) {
         if (n.nodeType == 3) return n;
         if (n.nodeType == 1 && e > 0) {
             if (n.childNodes.length > e && n.childNodes[e].nodeType == 3) return n.childNodes[e];
-            n = n.childNodes[e - 1], e = et(n)
+            n = n.childNodes[e - 1], e = Oe(n)
         } else if (n.nodeType == 1 && e < n.childNodes.length) n = n.childNodes[e], e = 0;
         else return null
     }
 }
 
-function fp(n, e, t, r) {
-    for (let i = 0, o = 0; i < n.childCount && o <= r;) {
-        let s = n.child(i++),
-            l = o;
-        if (o += s.nodeSize, !s.isText) continue;
-        let a = s.text;
+function Bu(n, e, t, r) {
+    for (let i = 0, s = 0; i < n.childCount && s <= r;) {
+        let o = n.child(i++),
+            l = s;
+        if (s += o.nodeSize, !o.isText) continue;
+        let a = o.text;
         for (; i < n.childCount;) {
             let c = n.child(i++);
-            if (o += c.nodeSize, !c.isText) break;
+            if (s += c.nodeSize, !c.isText) break;
             a += c.text
         }
-        if (o >= t) {
+        if (s >= t) {
             let c = l < r ? a.lastIndexOf(e, r - l - 1) : -1;
             if (c >= 0 && c + e.length + l >= t) return l + c;
             if (t == r && a.length >= r + e.length - l && a.slice(r - l, r - l + e.length) == e) return r
         }
     }
     return -1
 }
 
-function Bo(n, e, t, r, i) {
-    let o = [];
-    for (let s = 0, l = 0; s < n.length; s++) {
-        let a = n[s],
+function ki(n, e, t, r, i) {
+    let s = [];
+    for (let o = 0, l = 0; o < n.length; o++) {
+        let a = n[o],
             c = l,
             u = l += a.size;
-        c >= t || u <= e ? o.push(a) : (c < e && o.push(a.slice(0, e - c, r)), i && (o.push(i), i = void 0), u > t && o.push(a.slice(t - c, a.size, r)))
+        c >= t || u <= e ? s.push(a) : (c < e && s.push(a.slice(0, e - c, r)), i && (s.push(i), i = void 0), u > t && s.push(a.slice(t - c, a.size, r)))
     }
-    return o
+    return s
 }
 
-function Uo(n, e = null) {
+function Ii(n, e = null) {
     let t = n.domSelectionRange(),
         r = n.state.doc;
     if (!t.focusNode) return null;
     let i = n.docView.nearestDesc(t.focusNode),
-        o = i && i.size == 0,
-        s = n.docView.posFromDOM(t.focusNode, t.focusOffset, 1);
-    if (s < 0) return null;
-    let l = r.resolve(s),
+        s = i && i.size == 0,
+        o = n.docView.posFromDOM(t.focusNode, t.focusOffset, 1);
+    if (o < 0) return null;
+    let l = r.resolve(o),
         a, c;
-    if (ni(t)) {
+    if (rr(t)) {
         for (a = l; i && !i.node;) i = i.parent;
         let u = i.node;
-        if (i && u.isAtom && D.isSelectable(u) && i.parent && !(u.isInline && Hf(t.focusNode, t.focusOffset, i.dom))) {
+        if (i && u.isAtom && O.isSelectable(u) && i.parent && !(u.isInline && au(t.focusNode, t.focusOffset, i.dom))) {
             let d = i.posBefore;
-            c = new D(s == d ? l : r.resolve(d))
+            c = new O(o == d ? l : r.resolve(d))
         }
     } else {
         let u = n.docView.posFromDOM(t.anchorNode, t.anchorOffset, 1);
         if (u < 0) return null;
         a = r.resolve(u)
     }
     if (!c) {
-        let u = e == "pointer" || n.state.selection.head < l.pos && !o ? 1 : -1;
-        c = _o(n, a, l, u)
+        let u = e == "pointer" || n.state.selection.head < l.pos && !s ? 1 : -1;
+        c = Di(n, a, l, u)
     }
     return c
 }
 
-function dc(n) {
-    return n.editable ? n.hasFocus() : pc(n) && document.activeElement && document.activeElement.contains(n.dom)
+function Ml(n) {
+    return n.editable ? n.hasFocus() : El(n) && document.activeElement && document.activeElement.contains(n.dom)
 }
 
-function bt(n, e = !1) {
+function Je(n, e = !1) {
     let t = n.state.selection;
-    if (fc(n, t), !!dc(n)) {
-        if (!e && n.input.mouseDown && n.input.mouseDown.allowDefault && ye) {
+    if (Sl(n, t), !!Ml(n)) {
+        if (!e && n.input.mouseDown && n.input.mouseDown.allowDefault && ie) {
             let r = n.domSelectionRange(),
                 i = n.domObserver.currentSelection;
-            if (r.anchorNode && i.anchorNode && hn(r.anchorNode, r.anchorOffset, i.anchorNode, i.anchorOffset)) {
+            if (r.anchorNode && i.anchorNode && Ct(r.anchorNode, r.anchorOffset, i.anchorNode, i.anchorOffset)) {
                 n.input.mouseDown.delayedSelectionSync = !0, n.domObserver.setCurSelection();
                 return
             }
         }
-        if (n.domObserver.disconnectSelection(), n.cursorWrapper) hp(n);
+        if (n.domObserver.disconnectSelection(), n.cursorWrapper) Hu(n);
         else {
             let {
                 anchor: r,
                 head: i
-            } = t, o, s;
-            Pa && !(t instanceof P) && (t.$from.parent.inlineContent || (o = Ra(n, t.from)), !t.empty && !t.$from.parent.inlineContent && (s = Ra(n, t.to))), n.docView.setSelection(r, i, n.root, e), Pa && (o && Ba(o), s && Ba(s)), t.visible ? n.dom.classList.remove("ProseMirror-hideselection") : (n.dom.classList.add("ProseMirror-hideselection"), "onselectionchange" in document && pp(n))
+            } = t, s, o;
+            Wo && !(t instanceof I) && (t.$from.parent.inlineContent || (s = qo(n, t.from)), !t.empty && !t.$from.parent.inlineContent && (o = qo(n, t.to))), n.docView.setSelection(r, i, n.root, e), Wo && (s && Ko(s), o && Ko(o)), t.visible ? n.dom.classList.remove("ProseMirror-hideselection") : (n.dom.classList.add("ProseMirror-hideselection"), "onselectionchange" in document && zu(n))
         }
         n.domObserver.setCurSelection(), n.domObserver.connectSelection()
     }
 }
-var Pa = ve || ye && $f < 63;
+var Wo = oe || ie && fu < 63;
 
-function Ra(n, e) {
+function qo(n, e) {
     let {
         node: t,
         offset: r
-    } = n.docView.domFromPos(e, 0), i = r < t.childNodes.length ? t.childNodes[r] : null, o = r ? t.childNodes[r - 1] : null;
-    if (ve && i && i.contentEditable == "false") return wo(i);
-    if ((!i || i.contentEditable == "false") && (!o || o.contentEditable == "false")) {
-        if (i) return wo(i);
-        if (o) return wo(o)
+    } = n.docView.domFromPos(e, 0), i = r < t.childNodes.length ? t.childNodes[r] : null, s = r ? t.childNodes[r - 1] : null;
+    if (oe && i && i.contentEditable == "false") return ci(i);
+    if ((!i || i.contentEditable == "false") && (!s || s.contentEditable == "false")) {
+        if (i) return ci(i);
+        if (s) return ci(s)
     }
 }
 
-function wo(n) {
-    return n.contentEditable = "true", ve && n.draggable && (n.draggable = !1, n.wasDraggable = !0), n
+function ci(n) {
+    return n.contentEditable = "true", oe && n.draggable && (n.draggable = !1, n.wasDraggable = !0), n
 }
 
-function Ba(n) {
+function Ko(n) {
     n.contentEditable = "false", n.wasDraggable && (n.draggable = !0, n.wasDraggable = null)
 }
 
-function pp(n) {
+function zu(n) {
     let e = n.dom.ownerDocument;
     e.removeEventListener("selectionchange", n.input.hideSelectionGuard);
     let t = n.domSelectionRange(),
         r = t.anchorNode,
         i = t.anchorOffset;
     e.addEventListener("selectionchange", n.input.hideSelectionGuard = () => {
         (t.anchorNode != r || t.anchorOffset != i) && (e.removeEventListener("selectionchange", n.input.hideSelectionGuard), setTimeout(() => {
-            (!dc(n) || n.state.selection.visible) && n.dom.classList.remove("ProseMirror-hideselection")
+            (!Ml(n) || n.state.selection.visible) && n.dom.classList.remove("ProseMirror-hideselection")
         }, 20))
     })
 }
 
-function hp(n) {
+function Hu(n) {
     let e = n.domSelection(),
         t = document.createRange(),
         r = n.cursorWrapper.dom,
         i = r.nodeName == "IMG";
-    i ? t.setEnd(r.parentNode, Fe(r) + 1) : t.setEnd(r, 0), t.collapse(!1), e.removeAllRanges(), e.addRange(t), !i && !n.state.selection.visible && Ce && Lt <= 11 && (r.disabled = !0, r.disabled = !1)
+    i ? t.setEnd(r.parentNode, be(r) + 1) : t.setEnd(r, 0), t.collapse(!1), e.removeAllRanges(), e.addRange(t), !i && !n.state.selection.visible && fe && Ze <= 11 && (r.disabled = !0, r.disabled = !1)
 }
 
-function fc(n, e) {
-    if (e instanceof D) {
+function Sl(n, e) {
+    if (e instanceof O) {
         let t = n.docView.descAt(e.from);
-        t != n.lastSelectedViewDesc && (za(n), t && t.selectNode(), n.lastSelectedViewDesc = t)
-    } else za(n)
+        t != n.lastSelectedViewDesc && (Uo(n), t && t.selectNode(), n.lastSelectedViewDesc = t)
+    } else Uo(n)
 }
 
-function za(n) {
+function Uo(n) {
     n.lastSelectedViewDesc && (n.lastSelectedViewDesc.parent && n.lastSelectedViewDesc.deselectNode(), n.lastSelectedViewDesc = void 0)
 }
 
-function _o(n, e, t, r) {
-    return n.someProp("createSelectionBetween", i => i(n, e, t)) || P.between(e, t, r)
+function Di(n, e, t, r) {
+    return n.someProp("createSelectionBetween", i => i(n, e, t)) || I.between(e, t, r)
 }
 
-function Ha(n) {
-    return n.editable && !n.hasFocus() ? !1 : pc(n)
+function _o(n) {
+    return n.editable && !n.hasFocus() ? !1 : El(n)
 }
 
-function pc(n) {
+function El(n) {
     let e = n.domSelectionRange();
     if (!e.anchorNode) return !1;
     try {
         return n.dom.contains(e.anchorNode.nodeType == 3 ? e.anchorNode.parentNode : e.anchorNode) && (n.editable || n.dom.contains(e.focusNode.nodeType == 3 ? e.focusNode.parentNode : e.focusNode))
     } catch {
         return !1
     }
 }
 
-function mp(n) {
+function Fu(n) {
     let e = n.docView.domFromPos(n.state.selection.anchor, 0),
         t = n.domSelectionRange();
-    return hn(e.node, e.offset, t.anchorNode, t.anchorOffset)
+    return Ct(e.node, e.offset, t.anchorNode, t.anchorOffset)
 }
 
-function zo(n, e) {
+function Mi(n, e) {
     let {
         $anchor: t,
         $head: r
-    } = n.selection, i = e > 0 ? t.max(r) : t.min(r), o = i.parent.inlineContent ? i.depth ? n.doc.resolve(e > 0 ? i.after() : i.before()) : null : i;
-    return o && R.findFrom(o, e)
+    } = n.selection, i = e > 0 ? t.max(r) : t.min(r), s = i.parent.inlineContent ? i.depth ? n.doc.resolve(e > 0 ? i.after() : i.before()) : null : i;
+    return s && L.findFrom(s, e)
 }
 
-function cn(n, e) {
+function Mt(n, e) {
     return n.dispatch(n.state.tr.setSelection(e).scrollIntoView()), !0
 }
 
-function Fa(n, e, t) {
+function Go(n, e, t) {
     let r = n.state.selection;
-    if (r instanceof P) {
+    if (r instanceof I) {
         if (!r.empty || t.indexOf("s") > -1) return !1;
         if (n.endOfTextblock(e > 0 ? "forward" : "backward")) {
-            let i = zo(n.state, e);
-            return i && i instanceof D ? cn(n, i) : !1
-        } else if (!(He && t.indexOf("m") > -1)) {
+            let i = Mi(n.state, e);
+            return i && i instanceof O ? Mt(n, i) : !1
+        } else if (!(ye && t.indexOf("m") > -1)) {
             let i = r.$head,
-                o = i.textOffset ? null : e < 0 ? i.nodeBefore : i.nodeAfter,
-                s;
-            if (!o || o.isText) return !1;
-            let l = e < 0 ? i.pos - o.nodeSize : i.pos;
-            return o.isAtom || (s = n.docView.descAt(l)) && !s.contentDOM ? D.isSelectable(o) ? cn(n, new D(e < 0 ? n.state.doc.resolve(i.pos - o.nodeSize) : i)) : ri ? cn(n, new P(n.state.doc.resolve(e < 0 ? l : l + o.nodeSize))) : !1 : !1
+                s = i.textOffset ? null : e < 0 ? i.nodeBefore : i.nodeAfter,
+                o;
+            if (!s || s.isText) return !1;
+            let l = e < 0 ? i.pos - s.nodeSize : i.pos;
+            return s.isAtom || (o = n.docView.descAt(l)) && !o.contentDOM ? O.isSelectable(s) ? Mt(n, new O(e < 0 ? n.state.doc.resolve(i.pos - s.nodeSize) : i)) : ir ? Mt(n, new I(n.state.doc.resolve(e < 0 ? l : l + s.nodeSize))) : !1 : !1
         }
     } else {
-        if (r instanceof D && r.node.isInline) return cn(n, new P(e > 0 ? r.$to : r.$from)); {
-            let i = zo(n.state, e);
-            return i ? cn(n, i) : !1
+        if (r instanceof O && r.node.isInline) return Mt(n, new I(e > 0 ? r.$to : r.$from)); {
+            let i = Mi(n.state, e);
+            return i ? Mt(n, i) : !1
         }
     }
 }
 
-function Xr(n) {
+function Zn(n) {
     return n.nodeType == 3 ? n.nodeValue.length : n.childNodes.length
 }
 
-function yr(n) {
+function xn(n) {
     let e = n.pmViewDesc;
     return e && e.size == 0 && (n.nextSibling || n.nodeName != "BR")
 }
 
-function mr(n, e) {
-    return e < 0 ? gp(n) : hc(n)
+function yn(n, e) {
+    return e < 0 ? ju(n) : wl(n)
 }
 
-function gp(n) {
+function ju(n) {
     let e = n.domSelectionRange(),
         t = e.focusNode,
         r = e.focusOffset;
     if (!t) return;
-    let i, o, s = !1;
-    for (_e && t.nodeType == 1 && r < Xr(t) && yr(t.childNodes[r]) && (s = !0);;)
+    let i, s, o = !1;
+    for (we && t.nodeType == 1 && r < Zn(t) && xn(t.childNodes[r]) && (o = !0);;)
         if (r > 0) {
             if (t.nodeType != 1) break; {
                 let l = t.childNodes[r - 1];
-                if (yr(l)) i = t, o = --r;
+                if (xn(l)) i = t, s = --r;
                 else if (l.nodeType == 3) t = l, r = t.nodeValue.length;
                 else break
             }
         } else {
-            if (mc(t)) break; {
+            if (Tl(t)) break; {
                 let l = t.previousSibling;
-                for (; l && yr(l);) i = t.parentNode, o = Fe(l), l = l.previousSibling;
-                if (l) t = l, r = Xr(t);
+                for (; l && xn(l);) i = t.parentNode, s = be(l), l = l.previousSibling;
+                if (l) t = l, r = Zn(t);
                 else {
                     if (t = t.parentNode, t == n.dom) break;
                     r = 0
                 }
             }
-        } s ? Ho(n, t, r) : i && Ho(n, i, o)
+        } o ? Si(n, t, r) : i && Si(n, i, s)
 }
 
-function hc(n) {
+function wl(n) {
     let e = n.domSelectionRange(),
         t = e.focusNode,
         r = e.focusOffset;
     if (!t) return;
-    let i = Xr(t),
-        o, s;
+    let i = Zn(t),
+        s, o;
     for (;;)
         if (r < i) {
             if (t.nodeType != 1) break;
             let l = t.childNodes[r];
-            if (yr(l)) o = t, s = ++r;
+            if (xn(l)) s = t, o = ++r;
             else break
         } else {
-            if (mc(t)) break; {
+            if (Tl(t)) break; {
                 let l = t.nextSibling;
-                for (; l && yr(l);) o = l.parentNode, s = Fe(l) + 1, l = l.nextSibling;
-                if (l) t = l, r = 0, i = Xr(t);
+                for (; l && xn(l);) s = l.parentNode, o = be(l) + 1, l = l.nextSibling;
+                if (l) t = l, r = 0, i = Zn(t);
                 else {
                     if (t = t.parentNode, t == n.dom) break;
                     r = i = 0
                 }
             }
-        } o && Ho(n, o, s)
+        } s && Si(n, s, o)
 }
 
-function mc(n) {
+function Tl(n) {
     let e = n.pmViewDesc;
     return e && e.node && e.node.isBlock
 }
 
-function Ho(n, e, t) {
+function Si(n, e, t) {
     let r = n.domSelection();
-    if (ni(r)) {
-        let o = document.createRange();
-        o.setEnd(e, t), o.setStart(e, t), r.removeAllRanges(), r.addRange(o)
+    if (rr(r)) {
+        let s = document.createRange();
+        s.setEnd(e, t), s.setStart(e, t), r.removeAllRanges(), r.addRange(s)
     } else r.extend && r.extend(e, t);
     n.domObserver.setCurSelection();
     let {
         state: i
     } = n;
     setTimeout(() => {
-        n.state == i && bt(n)
+        n.state == i && Je(n)
     }, 50)
 }
 
-function ja(n, e) {
+function Qo(n, e) {
     let t = n.state.doc.resolve(e);
-    if (!(ye || Wf) && t.parent.inlineContent) {
+    if (!(ie || hu) && t.parent.inlineContent) {
         let i = n.coordsAtPos(e);
         if (e > t.start()) {
-            let o = n.coordsAtPos(e - 1),
-                s = (o.top + o.bottom) / 2;
-            if (s > i.top && s < i.bottom && Math.abs(o.left - i.left) > 1) return o.left < i.left ? "ltr" : "rtl"
+            let s = n.coordsAtPos(e - 1),
+                o = (s.top + s.bottom) / 2;
+            if (o > i.top && o < i.bottom && Math.abs(s.left - i.left) > 1) return s.left < i.left ? "ltr" : "rtl"
         }
         if (e < t.end()) {
-            let o = n.coordsAtPos(e + 1),
-                s = (o.top + o.bottom) / 2;
-            if (s > i.top && s < i.bottom && Math.abs(o.left - i.left) > 1) return o.left > i.left ? "ltr" : "rtl"
+            let s = n.coordsAtPos(e + 1),
+                o = (s.top + s.bottom) / 2;
+            if (o > i.top && o < i.bottom && Math.abs(s.left - i.left) > 1) return s.left > i.left ? "ltr" : "rtl"
         }
     }
     return getComputedStyle(n.dom).direction == "rtl" ? "rtl" : "ltr"
 }
 
-function Va(n, e, t) {
+function Yo(n, e, t) {
     let r = n.state.selection;
-    if (r instanceof P && !r.empty || t.indexOf("s") > -1 || He && t.indexOf("m") > -1) return !1;
+    if (r instanceof I && !r.empty || t.indexOf("s") > -1 || ye && t.indexOf("m") > -1) return !1;
     let {
         $from: i,
-        $to: o
+        $to: s
     } = r;
     if (!i.parent.inlineContent || n.endOfTextblock(e < 0 ? "up" : "down")) {
-        let s = zo(n.state, e);
-        if (s && s instanceof D) return cn(n, s)
+        let o = Mi(n.state, e);
+        if (o && o instanceof O) return Mt(n, o)
     }
     if (!i.parent.inlineContent) {
-        let s = e < 0 ? i : o,
-            l = r instanceof fe ? R.near(s, e) : R.findFrom(s, e);
-        return l ? cn(n, l) : !1
+        let o = e < 0 ? i : s,
+            l = r instanceof Z ? L.near(o, e) : L.findFrom(o, e);
+        return l ? Mt(n, l) : !1
     }
     return !1
 }
 
-function $a(n, e) {
-    if (!(n.state.selection instanceof P)) return !0;
+function Xo(n, e) {
+    if (!(n.state.selection instanceof I)) return !0;
     let {
         $head: t,
         $anchor: r,
         empty: i
     } = n.state.selection;
     if (!t.sameParent(r)) return !0;
     if (!i) return !1;
     if (n.endOfTextblock(e > 0 ? "forward" : "backward")) return !0;
-    let o = !t.textOffset && (e < 0 ? t.nodeBefore : t.nodeAfter);
-    if (o && !o.isText) {
-        let s = n.state.tr;
-        return e < 0 ? s.delete(t.pos - o.nodeSize, t.pos) : s.delete(t.pos, t.pos + o.nodeSize), n.dispatch(s), !0
+    let s = !t.textOffset && (e < 0 ? t.nodeBefore : t.nodeAfter);
+    if (s && !s.isText) {
+        let o = n.state.tr;
+        return e < 0 ? o.delete(t.pos - s.nodeSize, t.pos) : o.delete(t.pos, t.pos + s.nodeSize), n.dispatch(o), !0
     }
     return !1
 }
 
-function Wa(n, e, t) {
+function Zo(n, e, t) {
     n.domObserver.stop(), e.contentEditable = t, n.domObserver.start()
 }
 
-function yp(n) {
-    if (!ve || n.state.selection.$head.parentOffset > 0) return !1;
+function $u(n) {
+    if (!oe || n.state.selection.$head.parentOffset > 0) return !1;
     let {
         focusNode: e,
         focusOffset: t
     } = n.domSelectionRange();
     if (e && e.nodeType == 1 && t == 0 && e.firstChild && e.firstChild.contentEditable == "false") {
         let r = e.firstChild;
-        Wa(n, r, "true"), setTimeout(() => Wa(n, r, "false"), 20)
+        Zo(n, r, "true"), setTimeout(() => Zo(n, r, "false"), 20)
     }
     return !1
 }
 
-function xp(n) {
+function Vu(n) {
     let e = "";
     return n.ctrlKey && (e += "c"), n.metaKey && (e += "m"), n.altKey && (e += "a"), n.shiftKey && (e += "s"), e
 }
 
-function bp(n, e) {
+function Ju(n, e) {
     let t = e.keyCode,
-        r = xp(e);
-    if (t == 8 || He && t == 72 && r == "c") return $a(n, -1) || mr(n, -1);
-    if (t == 46 || He && t == 68 && r == "c") return $a(n, 1) || mr(n, 1);
+        r = Vu(e);
+    if (t == 8 || ye && t == 72 && r == "c") return Xo(n, -1) || yn(n, -1);
+    if (t == 46 || ye && t == 68 && r == "c") return Xo(n, 1) || yn(n, 1);
     if (t == 13 || t == 27) return !0;
-    if (t == 37 || He && t == 66 && r == "c") {
-        let i = t == 37 ? ja(n, n.state.selection.from) == "ltr" ? -1 : 1 : -1;
-        return Fa(n, i, r) || mr(n, i)
-    } else if (t == 39 || He && t == 70 && r == "c") {
-        let i = t == 39 ? ja(n, n.state.selection.from) == "ltr" ? 1 : -1 : 1;
-        return Fa(n, i, r) || mr(n, i)
+    if (t == 37 || ye && t == 66 && r == "c") {
+        let i = t == 37 ? Qo(n, n.state.selection.from) == "ltr" ? -1 : 1 : -1;
+        return Go(n, i, r) || yn(n, i)
+    } else if (t == 39 || ye && t == 70 && r == "c") {
+        let i = t == 39 ? Qo(n, n.state.selection.from) == "ltr" ? 1 : -1 : 1;
+        return Go(n, i, r) || yn(n, i)
     } else {
-        if (t == 38 || He && t == 80 && r == "c") return Va(n, -1, r) || mr(n, -1);
-        if (t == 40 || He && t == 78 && r == "c") return yp(n) || Va(n, 1, r) || hc(n);
-        if (r == (He ? "m" : "c") && (t == 66 || t == 73 || t == 89 || t == 90)) return !0
+        if (t == 38 || ye && t == 80 && r == "c") return Yo(n, -1, r) || yn(n, -1);
+        if (t == 40 || ye && t == 78 && r == "c") return $u(n) || Yo(n, 1, r) || wl(n);
+        if (r == (ye ? "m" : "c") && (t == 66 || t == 73 || t == 89 || t == 90)) return !0
     }
     return !1
 }
 
-function gc(n, e) {
-    n.someProp("transformCopied", p => {
-        e = p(e, n)
+function Cl(n, e) {
+    n.someProp("transformCopied", h => {
+        e = h(e, n)
     });
     let t = [],
         {
             content: r,
             openStart: i,
-            openEnd: o
+            openEnd: s
         } = e;
-    for (; i > 1 && o > 1 && r.childCount == 1 && r.firstChild.childCount == 1;) {
-        i--, o--;
-        let p = r.firstChild;
-        t.push(p.type.name, p.attrs != p.type.defaultAttrs ? p.attrs : null), r = p.content
+    for (; i > 1 && s > 1 && r.childCount == 1 && r.firstChild.childCount == 1;) {
+        i--, s--;
+        let h = r.firstChild;
+        t.push(h.type.name, h.attrs != h.type.defaultAttrs ? h.attrs : null), r = h.content
     }
-    let s = n.someProp("clipboardSerializer") || Se.fromSchema(n.state.schema),
-        l = Mc(),
+    let o = n.someProp("clipboardSerializer") || ce.fromSchema(n.state.schema),
+        l = Dl(),
         a = l.createElement("div");
-    a.appendChild(s.serializeFragment(r, {
+    a.appendChild(o.serializeFragment(r, {
         document: l
     }));
     let c = a.firstChild,
         u, d = 0;
-    for (; c && c.nodeType == 1 && (u = vc[c.nodeName.toLowerCase()]);) {
-        for (let p = u.length - 1; p >= 0; p--) {
-            let h = l.createElement(u[p]);
-            for (; a.firstChild;) h.appendChild(a.firstChild);
-            a.appendChild(h), d++
+    for (; c && c.nodeType == 1 && (u = Il[c.nodeName.toLowerCase()]);) {
+        for (let h = u.length - 1; h >= 0; h--) {
+            let p = l.createElement(u[h]);
+            for (; a.firstChild;) p.appendChild(a.firstChild);
+            a.appendChild(p), d++
         }
         c = a.firstChild
     }
-    c && c.nodeType == 1 && c.setAttribute("data-pm-slice", `${i} ${o}${d?` -${d}`:""} ${JSON.stringify(t)}`);
-    let f = n.someProp("clipboardTextSerializer", p => p(e, n)) || e.content.textBetween(0, e.content.size, `
+    c && c.nodeType == 1 && c.setAttribute("data-pm-slice", `${i} ${s}${d?` -${d}`:""} ${JSON.stringify(t)}`);
+    let f = n.someProp("clipboardTextSerializer", h => h(e, n)) || e.content.textBetween(0, e.content.size, `
 
 `);
     return {
         dom: a,
         text: f
     }
 }
 
-function yc(n, e, t, r, i) {
-    let o = i.parent.type.spec.code,
-        s, l;
+function Al(n, e, t, r, i) {
+    let s = i.parent.type.spec.code,
+        o, l;
     if (!t && !e) return null;
-    let a = e && (r || o || !t);
+    let a = e && (r || s || !t);
     if (a) {
         if (n.someProp("transformPastedText", f => {
-                e = f(e, o || r, n)
-            }), o) return e ? new w(v.from(n.state.schema.text(e.replace(/\r\n?/g, `
-`))), 0, 0) : w.empty;
+                e = f(e, s || r, n)
+            }), s) return e ? new E(x.from(n.state.schema.text(e.replace(/\r\n?/g, `
+`))), 0, 0) : E.empty;
         let d = n.someProp("clipboardTextParser", f => f(e, i, r, n));
         if (d) l = d;
         else {
             let f = i.marks(),
                 {
-                    schema: p
+                    schema: h
                 } = n.state,
-                h = Se.fromSchema(p);
-            s = document.createElement("div"), e.split(/(?:\r\n?|\n)+/).forEach(m => {
-                let b = s.appendChild(document.createElement("p"));
-                m && b.appendChild(h.serializeNode(p.text(m, f)))
+                p = ce.fromSchema(h);
+            o = document.createElement("div"), e.split(/(?:\r\n?|\n)+/).forEach(m => {
+                let b = o.appendChild(document.createElement("p"));
+                m && b.appendChild(p.serializeNode(h.text(m, f)))
             })
         }
     } else n.someProp("transformPastedHTML", d => {
         t = d(t, n)
-    }), s = Mp(t), ri && Ep(s);
-    let c = s && s.querySelector("[data-pm-slice]"),
+    }), o = Ku(t), ir && Uu(o);
+    let c = o && o.querySelector("[data-pm-slice]"),
         u = c && /^(\d+) (\d+)(?: -(\d+))? (.*)/.exec(c.getAttribute("data-pm-slice") || "");
     if (u && u[3])
         for (let d = +u[3]; d > 0; d--) {
-            let f = s.firstChild;
+            let f = o.firstChild;
             for (; f && f.nodeType != 1;) f = f.nextSibling;
             if (!f) break;
-            s = f
+            o = f
         }
-    if (l || (l = (n.someProp("clipboardParser") || n.someProp("domParser") || Qe.fromSchema(n.state.schema)).parseSlice(s, {
+    if (l || (l = (n.someProp("clipboardParser") || n.someProp("domParser") || Te.fromSchema(n.state.schema)).parseSlice(o, {
             preserveWhitespace: !!(a || u),
             context: i,
             ruleFromNode(f) {
-                return f.nodeName == "BR" && !f.nextSibling && f.parentNode && !kp.test(f.parentNode.nodeName) ? {
+                return f.nodeName == "BR" && !f.nextSibling && f.parentNode && !Wu.test(f.parentNode.nodeName) ? {
                     ignore: !0
                 } : null
             }
-        })), u) l = Sp(qa(l, +u[1], +u[2]), u[4]);
-    else if (l = w.maxOpen(vp(l.content, i), !0), l.openStart || l.openEnd) {
+        })), u) l = _u(el(l, +u[1], +u[2]), u[4]);
+    else if (l = E.maxOpen(qu(l.content, i), !0), l.openStart || l.openEnd) {
         let d = 0,
             f = 0;
-        for (let p = l.content.firstChild; d < l.openStart && !p.type.spec.isolating; d++, p = p.firstChild);
-        for (let p = l.content.lastChild; f < l.openEnd && !p.type.spec.isolating; f++, p = p.lastChild);
-        l = qa(l, d, f)
+        for (let h = l.content.firstChild; d < l.openStart && !h.type.spec.isolating; d++, h = h.firstChild);
+        for (let h = l.content.lastChild; f < l.openEnd && !h.type.spec.isolating; f++, h = h.lastChild);
+        l = el(l, d, f)
     }
     return n.someProp("transformPasted", d => {
         l = d(l, n)
     }), l
 }
-var kp = /^(a|abbr|acronym|b|cite|code|del|em|i|ins|kbd|label|output|q|ruby|s|samp|span|strong|sub|sup|time|u|tt|var)$/i;
+var Wu = /^(a|abbr|acronym|b|cite|code|del|em|i|ins|kbd|label|output|q|ruby|s|samp|span|strong|sub|sup|time|u|tt|var)$/i;
 
-function vp(n, e) {
+function qu(n, e) {
     if (n.childCount < 2) return n;
     for (let t = e.depth; t >= 0; t--) {
         let i = e.node(t).contentMatchAt(e.index(t)),
-            o, s = [];
+            s, o = [];
         if (n.forEach(l => {
-                if (!s) return;
+                if (!o) return;
                 let a = i.findWrapping(l.type),
                     c;
-                if (!a) return s = null;
-                if (c = s.length && o.length && bc(a, o, l, s[s.length - 1], 0)) s[s.length - 1] = c;
+                if (!a) return o = null;
+                if (c = o.length && s.length && vl(a, s, l, o[o.length - 1], 0)) o[o.length - 1] = c;
                 else {
-                    s.length && (s[s.length - 1] = kc(s[s.length - 1], o.length));
-                    let u = xc(l, a);
-                    s.push(u), i = i.matchType(u.type), o = a
+                    o.length && (o[o.length - 1] = Nl(o[o.length - 1], s.length));
+                    let u = Ol(l, a);
+                    o.push(u), i = i.matchType(u.type), s = a
                 }
-            }), s) return v.from(s)
+            }), o) return x.from(o)
     }
     return n
 }
 
-function xc(n, e, t = 0) {
-    for (let r = e.length - 1; r >= t; r--) n = e[r].create(null, v.from(n));
+function Ol(n, e, t = 0) {
+    for (let r = e.length - 1; r >= t; r--) n = e[r].create(null, x.from(n));
     return n
 }
 
-function bc(n, e, t, r, i) {
+function vl(n, e, t, r, i) {
     if (i < n.length && i < e.length && n[i] == e[i]) {
-        let o = bc(n, e, t, r.lastChild, i + 1);
-        if (o) return r.copy(r.content.replaceChild(r.childCount - 1, o));
-        if (r.contentMatchAt(r.childCount).matchType(i == n.length - 1 ? t.type : n[i + 1])) return r.copy(r.content.append(v.from(xc(t, n, i + 1))))
+        let s = vl(n, e, t, r.lastChild, i + 1);
+        if (s) return r.copy(r.content.replaceChild(r.childCount - 1, s));
+        if (r.contentMatchAt(r.childCount).matchType(i == n.length - 1 ? t.type : n[i + 1])) return r.copy(r.content.append(x.from(Ol(t, n, i + 1))))
     }
 }
 
-function kc(n, e) {
+function Nl(n, e) {
     if (e == 0) return n;
-    let t = n.content.replaceChild(n.childCount - 1, kc(n.lastChild, e - 1)),
-        r = n.contentMatchAt(n.childCount).fillBefore(v.empty, !0);
+    let t = n.content.replaceChild(n.childCount - 1, Nl(n.lastChild, e - 1)),
+        r = n.contentMatchAt(n.childCount).fillBefore(x.empty, !0);
     return n.copy(t.append(r))
 }
 
-function Fo(n, e, t, r, i, o) {
-    let s = e < 0 ? n.firstChild : n.lastChild,
-        l = s.content;
-    return n.childCount > 1 && (o = 0), i < r - 1 && (l = Fo(l, e, t, r, i + 1, o)), i >= t && (l = e < 0 ? s.contentMatchAt(0).fillBefore(l, o <= i).append(l) : l.append(s.contentMatchAt(s.childCount).fillBefore(v.empty, !0))), n.replaceChild(e < 0 ? 0 : n.childCount - 1, s.copy(l))
+function Ei(n, e, t, r, i, s) {
+    let o = e < 0 ? n.firstChild : n.lastChild,
+        l = o.content;
+    return n.childCount > 1 && (s = 0), i < r - 1 && (l = Ei(l, e, t, r, i + 1, s)), i >= t && (l = e < 0 ? o.contentMatchAt(0).fillBefore(l, s <= i).append(l) : l.append(o.contentMatchAt(o.childCount).fillBefore(x.empty, !0))), n.replaceChild(e < 0 ? 0 : n.childCount - 1, o.copy(l))
 }
 
-function qa(n, e, t) {
-    return e < n.openStart && (n = new w(Fo(n.content, -1, e, n.openStart, 0, n.openEnd), e, n.openEnd)), t < n.openEnd && (n = new w(Fo(n.content, 1, t, n.openEnd, 0, 0), n.openStart, t)), n
+function el(n, e, t) {
+    return e < n.openStart && (n = new E(Ei(n.content, -1, e, n.openStart, 0, n.openEnd), e, n.openEnd)), t < n.openEnd && (n = new E(Ei(n.content, 1, t, n.openEnd, 0, 0), n.openStart, t)), n
 }
-var vc = {
+var Il = {
         thead: ["table"],
         tbody: ["table"],
         tfoot: ["table"],
         caption: ["table"],
         colgroup: ["table"],
         col: ["table", "colgroup"],
         tr: ["table", "tbody"],
         td: ["table", "tbody", "tr"],
         th: ["table", "tbody", "tr"]
     },
-    Ja = null;
+    tl = null;
 
-function Mc() {
-    return Ja || (Ja = document.implementation.createHTMLDocument("title"))
+function Dl() {
+    return tl || (tl = document.implementation.createHTMLDocument("title"))
 }
 
-function Mp(n) {
+function Ku(n) {
     let e = /^(\s*<meta [^>]*>)*/.exec(n);
     e && (n = n.slice(e[0].length));
-    let t = Mc().createElement("div"),
+    let t = Dl().createElement("div"),
         r = /<([a-z][^>\s]+)/i.exec(n),
         i;
-    if ((i = r && vc[r[1].toLowerCase()]) && (n = i.map(o => "<" + o + ">").join("") + n + i.map(o => "</" + o + ">").reverse().join("")), t.innerHTML = n, i)
-        for (let o = 0; o < i.length; o++) t = t.querySelector(i[o]) || t;
+    if ((i = r && Il[r[1].toLowerCase()]) && (n = i.map(s => "<" + s + ">").join("") + n + i.map(s => "</" + s + ">").reverse().join("")), t.innerHTML = n, i)
+        for (let s = 0; s < i.length; s++) t = t.querySelector(i[s]) || t;
     return t
 }
 
-function Ep(n) {
-    let e = n.querySelectorAll(ye ? "span:not([class]):not([style])" : "span.Apple-converted-space");
+function Uu(n) {
+    let e = n.querySelectorAll(ie ? "span:not([class]):not([style])" : "span.Apple-converted-space");
     for (let t = 0; t < e.length; t++) {
         let r = e[t];
         r.childNodes.length == 1 && r.textContent == "\xA0" && r.parentNode && r.parentNode.replaceChild(n.ownerDocument.createTextNode(" "), r)
     }
 }
 
-function Sp(n, e) {
+function _u(n, e) {
     if (!n.size) return n;
     let t = n.content.firstChild.type.schema,
         r;
     try {
         r = JSON.parse(e)
     } catch {
         return n
     }
     let {
         content: i,
-        openStart: o,
-        openEnd: s
+        openStart: s,
+        openEnd: o
     } = n;
     for (let l = r.length - 2; l >= 0; l -= 2) {
         let a = t.nodes[r[l]];
         if (!a || a.hasRequiredAttrs()) break;
-        i = v.from(a.create(r[l + 1], i)), o++, s++
+        i = x.from(a.create(r[l + 1], i)), s++, o++
     }
-    return new w(i, o, s)
+    return new E(i, s, o)
 }
-var Me = {},
-    Ee = {},
-    wp = {
+var le = {},
+    ae = {},
+    Gu = {
         touchstart: !0,
         touchmove: !0
     },
-    jo = class {
+    wi = class {
         constructor() {
             this.shiftKey = !1, this.mouseDown = null, this.lastKeyCode = null, this.lastKeyCodeTime = 0, this.lastClick = {
                 time: 0,
                 x: 0,
                 y: 0,
                 type: ""
             }, this.lastSelectionOrigin = null, this.lastSelectionTime = 0, this.lastIOSEnter = 0, this.lastIOSEnterFallbackTimeout = -1, this.lastFocus = 0, this.lastTouch = 0, this.lastAndroidDelete = 0, this.composing = !1, this.composingTimeout = -1, this.compositionNodes = [], this.compositionEndedAt = -2e8, this.compositionID = 1, this.domChangeCount = 0, this.eventHandlers = Object.create(null), this.hideSelectionGuard = null
         }
     };
 
-function Tp(n) {
-    for (let e in Me) {
-        let t = Me[e];
+function Qu(n) {
+    for (let e in le) {
+        let t = le[e];
         n.dom.addEventListener(e, n.input.eventHandlers[e] = r => {
-            Op(n, r) && !Go(n, r) && (n.editable || !(r.type in Ee)) && t(n, r)
-        }, wp[e] ? {
+            Xu(n, r) && !Li(n, r) && (n.editable || !(r.type in ae)) && t(n, r)
+        }, Gu[e] ? {
             passive: !0
         } : void 0)
     }
-    ve && n.dom.addEventListener("input", () => null), Vo(n)
+    oe && n.dom.addEventListener("input", () => null), Ti(n)
 }
 
-function Dt(n, e) {
+function Xe(n, e) {
     n.input.lastSelectionOrigin = e, n.input.lastSelectionTime = Date.now()
 }
 
-function Cp(n) {
+function Yu(n) {
     n.domObserver.stop();
     for (let e in n.input.eventHandlers) n.dom.removeEventListener(e, n.input.eventHandlers[e]);
     clearTimeout(n.input.composingTimeout), clearTimeout(n.input.lastIOSEnterFallbackTimeout)
 }
 
-function Vo(n) {
+function Ti(n) {
     n.someProp("handleDOMEvents", e => {
-        for (let t in e) n.input.eventHandlers[t] || n.dom.addEventListener(t, n.input.eventHandlers[t] = r => Go(n, r))
+        for (let t in e) n.input.eventHandlers[t] || n.dom.addEventListener(t, n.input.eventHandlers[t] = r => Li(n, r))
     })
 }
 
-function Go(n, e) {
+function Li(n, e) {
     return n.someProp("handleDOMEvents", t => {
         let r = t[e.type];
         return r ? r(n, e) || e.defaultPrevented : !1
     })
 }
 
-function Op(n, e) {
+function Xu(n, e) {
     if (!e.bubbles) return !0;
     if (e.defaultPrevented) return !1;
     for (let t = e.target; t != n.dom; t = t.parentNode)
         if (!t || t.nodeType == 11 || t.pmViewDesc && t.pmViewDesc.stopEvent(e)) return !1;
     return !0
 }
 
-function Ap(n, e) {
-    !Go(n, e) && Me[e.type] && (n.editable || !(e.type in Ee)) && Me[e.type](n, e)
+function Zu(n, e) {
+    !Li(n, e) && le[e.type] && (n.editable || !(e.type in ae)) && le[e.type](n, e)
 }
-Ee.keydown = (n, e) => {
+ae.keydown = (n, e) => {
     let t = e;
-    if (n.input.shiftKey = t.keyCode == 16 || t.shiftKey, !Sc(n, t) && (n.input.lastKeyCode = t.keyCode, n.input.lastKeyCodeTime = Date.now(), !(Ue && ye && t.keyCode == 13)))
-        if (t.keyCode != 229 && n.domObserver.forceFlush(), Hn && t.keyCode == 13 && !t.ctrlKey && !t.altKey && !t.metaKey) {
+    if (n.input.shiftKey = t.keyCode == 16 || t.shiftKey, !Rl(n, t) && (n.input.lastKeyCode = t.keyCode, n.input.lastKeyCodeTime = Date.now(), !(Ee && ie && t.keyCode == 13)))
+        if (t.keyCode != 229 && n.domObserver.forceFlush(), qt && t.keyCode == 13 && !t.ctrlKey && !t.altKey && !t.metaKey) {
             let r = Date.now();
             n.input.lastIOSEnter = r, n.input.lastIOSEnterFallbackTimeout = setTimeout(() => {
-                n.input.lastIOSEnter == r && (n.someProp("handleKeyDown", i => i(n, an(13, "Enter"))), n.input.lastIOSEnter = 0)
+                n.input.lastIOSEnter == r && (n.someProp("handleKeyDown", i => i(n, kt(13, "Enter"))), n.input.lastIOSEnter = 0)
             }, 200)
-        } else n.someProp("handleKeyDown", r => r(n, t)) || bp(n, t) ? t.preventDefault() : Dt(n, "key")
+        } else n.someProp("handleKeyDown", r => r(n, t)) || Ju(n, t) ? t.preventDefault() : Xe(n, "key")
 };
-Ee.keyup = (n, e) => {
+ae.keyup = (n, e) => {
     e.keyCode == 16 && (n.input.shiftKey = !1)
 };
-Ee.keypress = (n, e) => {
+ae.keypress = (n, e) => {
     let t = e;
-    if (Sc(n, t) || !t.charCode || t.ctrlKey && !t.altKey || He && t.metaKey) return;
+    if (Rl(n, t) || !t.charCode || t.ctrlKey && !t.altKey || ye && t.metaKey) return;
     if (n.someProp("handleKeyPress", i => i(n, t))) {
         t.preventDefault();
         return
     }
     let r = n.state.selection;
-    if (!(r instanceof P) || !r.$from.sameParent(r.$to)) {
+    if (!(r instanceof I) || !r.$from.sameParent(r.$to)) {
         let i = String.fromCharCode(t.charCode);
-        !/[\r\n]/.test(i) && !n.someProp("handleTextInput", o => o(n, r.$from.pos, r.$to.pos, i)) && n.dispatch(n.state.tr.insertText(i).scrollIntoView()), t.preventDefault()
+        !/[\r\n]/.test(i) && !n.someProp("handleTextInput", s => s(n, r.$from.pos, r.$to.pos, i)) && n.dispatch(n.state.tr.insertText(i).scrollIntoView()), t.preventDefault()
     }
 };
 
-function ii(n) {
+function sr(n) {
     return {
         left: n.clientX,
         top: n.clientY
     }
 }
 
-function Np(n, e) {
+function ed(n, e) {
     let t = e.x - n.clientX,
         r = e.y - n.clientY;
     return t * t + r * r < 100
 }
 
-function Yo(n, e, t, r, i) {
+function Ri(n, e, t, r, i) {
     if (r == -1) return !1;
-    let o = n.state.doc.resolve(r);
-    for (let s = o.depth + 1; s > 0; s--)
-        if (n.someProp(e, l => s > o.depth ? l(n, t, o.nodeAfter, o.before(s), i, !0) : l(n, t, o.node(s), o.before(s), i, !1))) return !0;
+    let s = n.state.doc.resolve(r);
+    for (let o = s.depth + 1; o > 0; o--)
+        if (n.someProp(e, l => o > s.depth ? l(n, t, s.nodeAfter, s.before(o), i, !0) : l(n, t, s.node(o), s.before(o), i, !1))) return !0;
     return !1
 }
 
-function zn(n, e, t) {
+function Wt(n, e, t) {
     n.focused || n.focus();
     let r = n.state.tr.setSelection(e);
     t == "pointer" && r.setMeta("pointer", !0), n.dispatch(r)
 }
 
-function Ip(n, e) {
+function td(n, e) {
     if (e == -1) return !1;
     let t = n.state.doc.resolve(e),
         r = t.nodeAfter;
-    return r && r.isAtom && D.isSelectable(r) ? (zn(n, new D(t), "pointer"), !0) : !1
+    return r && r.isAtom && O.isSelectable(r) ? (Wt(n, new O(t), "pointer"), !0) : !1
 }
 
-function Dp(n, e) {
+function nd(n, e) {
     if (e == -1) return !1;
     let t = n.state.selection,
         r, i;
-    t instanceof D && (r = t.node);
-    let o = n.state.doc.resolve(e);
-    for (let s = o.depth + 1; s > 0; s--) {
-        let l = s > o.depth ? o.nodeAfter : o.node(s);
-        if (D.isSelectable(l)) {
-            r && t.$from.depth > 0 && s >= t.$from.depth && o.before(t.$from.depth + 1) == t.$from.pos ? i = o.before(t.$from.depth) : i = o.before(s);
+    t instanceof O && (r = t.node);
+    let s = n.state.doc.resolve(e);
+    for (let o = s.depth + 1; o > 0; o--) {
+        let l = o > s.depth ? s.nodeAfter : s.node(o);
+        if (O.isSelectable(l)) {
+            r && t.$from.depth > 0 && o >= t.$from.depth && s.before(t.$from.depth + 1) == t.$from.pos ? i = s.before(t.$from.depth) : i = s.before(o);
             break
         }
     }
-    return i != null ? (zn(n, D.create(n.state.doc, i), "pointer"), !0) : !1
+    return i != null ? (Wt(n, O.create(n.state.doc, i), "pointer"), !0) : !1
 }
 
-function Lp(n, e, t, r, i) {
-    return Yo(n, "handleClickOn", e, t, r) || n.someProp("handleClick", o => o(n, e, r)) || (i ? Dp(n, t) : Ip(n, t))
+function rd(n, e, t, r, i) {
+    return Ri(n, "handleClickOn", e, t, r) || n.someProp("handleClick", s => s(n, e, r)) || (i ? nd(n, t) : td(n, t))
 }
 
-function Pp(n, e, t, r) {
-    return Yo(n, "handleDoubleClickOn", e, t, r) || n.someProp("handleDoubleClick", i => i(n, e, r))
+function id(n, e, t, r) {
+    return Ri(n, "handleDoubleClickOn", e, t, r) || n.someProp("handleDoubleClick", i => i(n, e, r))
 }
 
-function Rp(n, e, t, r) {
-    return Yo(n, "handleTripleClickOn", e, t, r) || n.someProp("handleTripleClick", i => i(n, e, r)) || Bp(n, t, r)
+function sd(n, e, t, r) {
+    return Ri(n, "handleTripleClickOn", e, t, r) || n.someProp("handleTripleClick", i => i(n, e, r)) || od(n, t, r)
 }
 
-function Bp(n, e, t) {
+function od(n, e, t) {
     if (t.button != 0) return !1;
     let r = n.state.doc;
-    if (e == -1) return r.inlineContent ? (zn(n, P.create(r, 0, r.content.size), "pointer"), !0) : !1;
+    if (e == -1) return r.inlineContent ? (Wt(n, I.create(r, 0, r.content.size), "pointer"), !0) : !1;
     let i = r.resolve(e);
-    for (let o = i.depth + 1; o > 0; o--) {
-        let s = o > i.depth ? i.nodeAfter : i.node(o),
-            l = i.before(o);
-        if (s.inlineContent) zn(n, P.create(r, l + 1, l + 1 + s.content.size), "pointer");
-        else if (D.isSelectable(s)) zn(n, D.create(r, l), "pointer");
+    for (let s = i.depth + 1; s > 0; s--) {
+        let o = s > i.depth ? i.nodeAfter : i.node(s),
+            l = i.before(s);
+        if (o.inlineContent) Wt(n, I.create(r, l + 1, l + 1 + o.content.size), "pointer");
+        else if (O.isSelectable(o)) Wt(n, O.create(r, l), "pointer");
         else continue;
         return !0
     }
 }
 
-function Qo(n) {
-    return Zr(n)
+function Pi(n) {
+    return er(n)
 }
-var Ec = He ? "metaKey" : "ctrlKey";
-Me.mousedown = (n, e) => {
+var Ll = ye ? "metaKey" : "ctrlKey";
+le.mousedown = (n, e) => {
     let t = e;
     n.input.shiftKey = t.shiftKey;
-    let r = Qo(n),
+    let r = Pi(n),
         i = Date.now(),
-        o = "singleClick";
-    i - n.input.lastClick.time < 500 && Np(t, n.input.lastClick) && !t[Ec] && (n.input.lastClick.type == "singleClick" ? o = "doubleClick" : n.input.lastClick.type == "doubleClick" && (o = "tripleClick")), n.input.lastClick = {
+        s = "singleClick";
+    i - n.input.lastClick.time < 500 && ed(t, n.input.lastClick) && !t[Ll] && (n.input.lastClick.type == "singleClick" ? s = "doubleClick" : n.input.lastClick.type == "doubleClick" && (s = "tripleClick")), n.input.lastClick = {
         time: i,
         x: t.clientX,
         y: t.clientY,
-        type: o
+        type: s
     };
-    let s = n.posAtCoords(ii(t));
-    s && (o == "singleClick" ? (n.input.mouseDown && n.input.mouseDown.done(), n.input.mouseDown = new $o(n, s, t, !!r)) : (o == "doubleClick" ? Pp : Rp)(n, s.pos, s.inside, t) ? t.preventDefault() : Dt(n, "pointer"))
+    let o = n.posAtCoords(sr(t));
+    o && (s == "singleClick" ? (n.input.mouseDown && n.input.mouseDown.done(), n.input.mouseDown = new Ci(n, o, t, !!r)) : (s == "doubleClick" ? id : sd)(n, o.pos, o.inside, t) ? t.preventDefault() : Xe(n, "pointer"))
 };
-var $o = class {
+var Ci = class {
     constructor(e, t, r, i) {
-        this.view = e, this.pos = t, this.event = r, this.flushed = i, this.delayedSelectionSync = !1, this.mightDrag = null, this.startDoc = e.state.doc, this.selectNode = !!r[Ec], this.allowDefault = r.shiftKey;
-        let o, s;
-        if (t.inside > -1) o = e.state.doc.nodeAt(t.inside), s = t.inside;
+        this.view = e, this.pos = t, this.event = r, this.flushed = i, this.delayedSelectionSync = !1, this.mightDrag = null, this.startDoc = e.state.doc, this.selectNode = !!r[Ll], this.allowDefault = r.shiftKey;
+        let s, o;
+        if (t.inside > -1) s = e.state.doc.nodeAt(t.inside), o = t.inside;
         else {
             let u = e.state.doc.resolve(t.pos);
-            o = u.parent, s = u.depth ? u.before() : 0
+            s = u.parent, o = u.depth ? u.before() : 0
         }
         let l = i ? null : r.target,
             a = l ? e.docView.nearestDesc(l, !0) : null;
         this.target = a ? a.dom : null;
         let {
             selection: c
         } = e.state;
-        (r.button == 0 && o.type.spec.draggable && o.type.spec.selectable !== !1 || c instanceof D && c.from <= s && c.to > s) && (this.mightDrag = {
-            node: o,
-            pos: s,
+        (r.button == 0 && s.type.spec.draggable && s.type.spec.selectable !== !1 || c instanceof O && c.from <= o && c.to > o) && (this.mightDrag = {
+            node: s,
+            pos: o,
             addAttr: !!(this.target && !this.target.draggable),
-            setUneditable: !!(this.target && _e && !this.target.hasAttribute("contentEditable"))
+            setUneditable: !!(this.target && we && !this.target.hasAttribute("contentEditable"))
         }), this.target && this.mightDrag && (this.mightDrag.addAttr || this.mightDrag.setUneditable) && (this.view.domObserver.stop(), this.mightDrag.addAttr && (this.target.draggable = !0), this.mightDrag.setUneditable && setTimeout(() => {
             this.view.input.mouseDown == this && this.target.setAttribute("contentEditable", "false")
-        }, 20), this.view.domObserver.start()), e.root.addEventListener("mouseup", this.up = this.up.bind(this)), e.root.addEventListener("mousemove", this.move = this.move.bind(this)), Dt(e, "pointer")
+        }, 20), this.view.domObserver.start()), e.root.addEventListener("mouseup", this.up = this.up.bind(this)), e.root.addEventListener("mousemove", this.move = this.move.bind(this)), Xe(e, "pointer")
     }
     done() {
-        this.view.root.removeEventListener("mouseup", this.up), this.view.root.removeEventListener("mousemove", this.move), this.mightDrag && this.target && (this.view.domObserver.stop(), this.mightDrag.addAttr && this.target.removeAttribute("draggable"), this.mightDrag.setUneditable && this.target.removeAttribute("contentEditable"), this.view.domObserver.start()), this.delayedSelectionSync && setTimeout(() => bt(this.view)), this.view.input.mouseDown = null
+        this.view.root.removeEventListener("mouseup", this.up), this.view.root.removeEventListener("mousemove", this.move), this.mightDrag && this.target && (this.view.domObserver.stop(), this.mightDrag.addAttr && this.target.removeAttribute("draggable"), this.mightDrag.setUneditable && this.target.removeAttribute("contentEditable"), this.view.domObserver.start()), this.delayedSelectionSync && setTimeout(() => Je(this.view)), this.view.input.mouseDown = null
     }
     up(e) {
         if (this.done(), !this.view.dom.contains(e.target)) return;
         let t = this.pos;
-        this.view.state.doc != this.startDoc && (t = this.view.posAtCoords(ii(e))), this.updateAllowDefault(e), this.allowDefault || !t ? Dt(this.view, "pointer") : Lp(this.view, t.pos, t.inside, e, this.selectNode) ? e.preventDefault() : e.button == 0 && (this.flushed || ve && this.mightDrag && !this.mightDrag.node.isAtom || ye && !this.view.state.selection.visible && Math.min(Math.abs(t.pos - this.view.state.selection.from), Math.abs(t.pos - this.view.state.selection.to)) <= 2) ? (zn(this.view, R.near(this.view.state.doc.resolve(t.pos)), "pointer"), e.preventDefault()) : Dt(this.view, "pointer")
+        this.view.state.doc != this.startDoc && (t = this.view.posAtCoords(sr(e))), this.updateAllowDefault(e), this.allowDefault || !t ? Xe(this.view, "pointer") : rd(this.view, t.pos, t.inside, e, this.selectNode) ? e.preventDefault() : e.button == 0 && (this.flushed || oe && this.mightDrag && !this.mightDrag.node.isAtom || ie && !this.view.state.selection.visible && Math.min(Math.abs(t.pos - this.view.state.selection.from), Math.abs(t.pos - this.view.state.selection.to)) <= 2) ? (Wt(this.view, L.near(this.view.state.doc.resolve(t.pos)), "pointer"), e.preventDefault()) : Xe(this.view, "pointer")
     }
     move(e) {
-        this.updateAllowDefault(e), Dt(this.view, "pointer"), e.buttons == 0 && this.done()
+        this.updateAllowDefault(e), Xe(this.view, "pointer"), e.buttons == 0 && this.done()
     }
     updateAllowDefault(e) {
         !this.allowDefault && (Math.abs(this.event.x - e.clientX) > 4 || Math.abs(this.event.y - e.clientY) > 4) && (this.allowDefault = !0)
     }
 };
-Me.touchstart = n => {
-    n.input.lastTouch = Date.now(), Qo(n), Dt(n, "pointer")
+le.touchstart = n => {
+    n.input.lastTouch = Date.now(), Pi(n), Xe(n, "pointer")
 };
-Me.touchmove = n => {
-    n.input.lastTouch = Date.now(), Dt(n, "pointer")
+le.touchmove = n => {
+    n.input.lastTouch = Date.now(), Xe(n, "pointer")
 };
-Me.contextmenu = n => Qo(n);
+le.contextmenu = n => Pi(n);
 
-function Sc(n, e) {
-    return n.composing ? !0 : ve && Math.abs(e.timeStamp - n.input.compositionEndedAt) < 500 ? (n.input.compositionEndedAt = -2e8, !0) : !1
+function Rl(n, e) {
+    return n.composing ? !0 : oe && Math.abs(e.timeStamp - n.input.compositionEndedAt) < 500 ? (n.input.compositionEndedAt = -2e8, !0) : !1
 }
-var zp = Ue ? 5e3 : -1;
-Ee.compositionstart = Ee.compositionupdate = n => {
+var ld = Ee ? 5e3 : -1;
+ae.compositionstart = ae.compositionupdate = n => {
     if (!n.composing) {
         n.domObserver.flush();
         let {
             state: e
         } = n, t = e.selection.$from;
-        if (e.selection.empty && (e.storedMarks || !t.textOffset && t.parentOffset && t.nodeBefore.marks.some(r => r.type.spec.inclusive === !1))) n.markCursor = n.state.storedMarks || t.marks(), Zr(n, !0), n.markCursor = null;
-        else if (Zr(n), _e && e.selection.empty && t.parentOffset && !t.textOffset && t.nodeBefore.marks.length) {
+        if (e.selection.empty && (e.storedMarks || !t.textOffset && t.parentOffset && t.nodeBefore.marks.some(r => r.type.spec.inclusive === !1))) n.markCursor = n.state.storedMarks || t.marks(), er(n, !0), n.markCursor = null;
+        else if (er(n), we && e.selection.empty && t.parentOffset && !t.textOffset && t.nodeBefore.marks.length) {
             let r = n.domSelectionRange();
-            for (let i = r.focusNode, o = r.focusOffset; i && i.nodeType == 1 && o != 0;) {
-                let s = o < 0 ? i.lastChild : i.childNodes[o - 1];
-                if (!s) break;
-                if (s.nodeType == 3) {
-                    n.domSelection().collapse(s, s.nodeValue.length);
+            for (let i = r.focusNode, s = r.focusOffset; i && i.nodeType == 1 && s != 0;) {
+                let o = s < 0 ? i.lastChild : i.childNodes[s - 1];
+                if (!o) break;
+                if (o.nodeType == 3) {
+                    n.domSelection().collapse(o, o.nodeValue.length);
                     break
-                } else i = s, o = -1
+                } else i = o, s = -1
             }
         }
         n.input.composing = !0
     }
-    wc(n, zp)
+    Pl(n, ld)
 };
-Ee.compositionend = (n, e) => {
-    n.composing && (n.input.composing = !1, n.input.compositionEndedAt = e.timeStamp, n.input.compositionID++, wc(n, 20))
+ae.compositionend = (n, e) => {
+    n.composing && (n.input.composing = !1, n.input.compositionEndedAt = e.timeStamp, n.input.compositionID++, Pl(n, 20))
 };
 
-function wc(n, e) {
-    clearTimeout(n.input.composingTimeout), e > -1 && (n.input.composingTimeout = setTimeout(() => Zr(n), e))
+function Pl(n, e) {
+    clearTimeout(n.input.composingTimeout), e > -1 && (n.input.composingTimeout = setTimeout(() => er(n), e))
 }
 
-function Tc(n) {
-    for (n.composing && (n.input.composing = !1, n.input.compositionEndedAt = Hp()); n.input.compositionNodes.length > 0;) n.input.compositionNodes.pop().markParentsDirty()
+function Bl(n) {
+    for (n.composing && (n.input.composing = !1, n.input.compositionEndedAt = ad()); n.input.compositionNodes.length > 0;) n.input.compositionNodes.pop().markParentsDirty()
 }
 
-function Hp() {
+function ad() {
     let n = document.createEvent("Event");
     return n.initEvent("event", !0, !0), n.timeStamp
 }
 
-function Zr(n, e = !1) {
-    if (!(Ue && n.domObserver.flushingSoon >= 0)) {
-        if (n.domObserver.forceFlush(), Tc(n), e || n.docView && n.docView.dirty) {
-            let t = Uo(n);
+function er(n, e = !1) {
+    if (!(Ee && n.domObserver.flushingSoon >= 0)) {
+        if (n.domObserver.forceFlush(), Bl(n), e || n.docView && n.docView.dirty) {
+            let t = Ii(n);
             return t && !t.eq(n.state.selection) ? n.dispatch(n.state.tr.setSelection(t)) : n.updateState(n.state), !0
         }
         return !1
     }
 }
 
-function Fp(n, e) {
+function cd(n, e) {
     if (!n.dom.parentNode) return;
     let t = n.dom.parentNode.appendChild(document.createElement("div"));
     t.appendChild(e), t.style.cssText = "position: fixed; left: -10000px; top: 10px";
     let r = getSelection(),
         i = document.createRange();
     i.selectNodeContents(e), n.dom.blur(), r.removeAllRanges(), r.addRange(i), setTimeout(() => {
         t.parentNode && t.parentNode.removeChild(t), n.focus()
     }, 50)
 }
-var jn = Ce && Lt < 15 || Hn && qf < 604;
-Me.copy = Ee.cut = (n, e) => {
+var Ut = fe && Ze < 15 || qt && pu < 604;
+le.copy = ae.cut = (n, e) => {
     let t = e,
         r = n.state.selection,
         i = t.type == "cut";
     if (r.empty) return;
-    let o = jn ? null : t.clipboardData,
-        s = r.content(),
+    let s = Ut ? null : t.clipboardData,
+        o = r.content(),
         {
             dom: l,
             text: a
-        } = gc(n, s);
-    o ? (t.preventDefault(), o.clearData(), o.setData("text/html", l.innerHTML), o.setData("text/plain", a)) : Fp(n, l), i && n.dispatch(n.state.tr.deleteSelection().scrollIntoView().setMeta("uiEvent", "cut"))
+        } = Cl(n, o);
+    s ? (t.preventDefault(), s.clearData(), s.setData("text/html", l.innerHTML), s.setData("text/plain", a)) : cd(n, l), i && n.dispatch(n.state.tr.deleteSelection().scrollIntoView().setMeta("uiEvent", "cut"))
 };
 
-function jp(n) {
+function ud(n) {
     return n.openStart == 0 && n.openEnd == 0 && n.content.childCount == 1 ? n.content.firstChild : null
 }
 
-function Vp(n, e) {
+function dd(n, e) {
     if (!n.dom.parentNode) return;
     let t = n.input.shiftKey || n.state.selection.$from.parent.type.spec.code,
         r = n.dom.parentNode.appendChild(document.createElement(t ? "textarea" : "div"));
     t || (r.contentEditable = "true"), r.style.cssText = "position: fixed; left: -10000px; top: 10px", r.focus(), setTimeout(() => {
-        n.focus(), r.parentNode && r.parentNode.removeChild(r), t ? br(n, r.value, null, n.input.shiftKey, e) : br(n, r.textContent, r.innerHTML, n.input.shiftKey, e)
+        n.focus(), r.parentNode && r.parentNode.removeChild(r), t ? Mn(n, r.value, null, n.input.shiftKey, e) : Mn(n, r.textContent, r.innerHTML, n.input.shiftKey, e)
     }, 50)
 }
 
-function br(n, e, t, r, i) {
-    let o = yc(n, e, t, r, n.state.selection.$from);
-    if (n.someProp("handlePaste", a => a(n, i, o || w.empty))) return !0;
-    if (!o) return !1;
-    let s = jp(o),
-        l = s ? n.state.tr.replaceSelectionWith(s, n.input.shiftKey) : n.state.tr.replaceSelection(o);
+function Mn(n, e, t, r, i) {
+    let s = Al(n, e, t, r, n.state.selection.$from);
+    if (n.someProp("handlePaste", a => a(n, i, s || E.empty))) return !0;
+    if (!s) return !1;
+    let o = ud(s),
+        l = o ? n.state.tr.replaceSelectionWith(o, n.input.shiftKey) : n.state.tr.replaceSelection(s);
     return n.dispatch(l.scrollIntoView().setMeta("paste", !0).setMeta("uiEvent", "paste")), !0
 }
-Ee.paste = (n, e) => {
+ae.paste = (n, e) => {
     let t = e;
-    if (n.composing && !Ue) return;
-    let r = jn ? null : t.clipboardData;
-    r && br(n, r.getData("text/plain"), r.getData("text/html"), n.input.shiftKey, t) ? t.preventDefault() : Vp(n, t)
+    if (n.composing && !Ee) return;
+    let r = Ut ? null : t.clipboardData;
+    r && Mn(n, r.getData("text/plain"), r.getData("text/html"), n.input.shiftKey, t) ? t.preventDefault() : dd(n, t)
 };
-var Wo = class {
+var Ai = class {
         constructor(e, t) {
             this.slice = e, this.move = t
         }
     },
-    Cc = He ? "altKey" : "ctrlKey";
-Me.dragstart = (n, e) => {
+    zl = ye ? "altKey" : "ctrlKey";
+le.dragstart = (n, e) => {
     let t = e,
         r = n.input.mouseDown;
     if (r && r.done(), !t.dataTransfer) return;
     let i = n.state.selection,
-        o = i.empty ? null : n.posAtCoords(ii(t));
-    if (!(o && o.pos >= i.from && o.pos <= (i instanceof D ? i.to - 1 : i.to))) {
-        if (r && r.mightDrag) n.dispatch(n.state.tr.setSelection(D.create(n.state.doc, r.mightDrag.pos)));
+        s = i.empty ? null : n.posAtCoords(sr(t));
+    if (!(s && s.pos >= i.from && s.pos <= (i instanceof O ? i.to - 1 : i.to))) {
+        if (r && r.mightDrag) n.dispatch(n.state.tr.setSelection(O.create(n.state.doc, r.mightDrag.pos)));
         else if (t.target && t.target.nodeType == 1) {
             let c = n.docView.nearestDesc(t.target, !0);
-            c && c.node.type.spec.draggable && c != n.docView && n.dispatch(n.state.tr.setSelection(D.create(n.state.doc, c.posBefore)))
+            c && c.node.type.spec.draggable && c != n.docView && n.dispatch(n.state.tr.setSelection(O.create(n.state.doc, c.posBefore)))
         }
     }
-    let s = n.state.selection.content(),
+    let o = n.state.selection.content(),
         {
             dom: l,
             text: a
-        } = gc(n, s);
-    t.dataTransfer.clearData(), t.dataTransfer.setData(jn ? "Text" : "text/html", l.innerHTML), t.dataTransfer.effectAllowed = "copyMove", jn || t.dataTransfer.setData("text/plain", a), n.dragging = new Wo(s, !t[Cc])
+        } = Cl(n, o);
+    t.dataTransfer.clearData(), t.dataTransfer.setData(Ut ? "Text" : "text/html", l.innerHTML), t.dataTransfer.effectAllowed = "copyMove", Ut || t.dataTransfer.setData("text/plain", a), n.dragging = new Ai(o, !t[zl])
 };
-Me.dragend = n => {
+le.dragend = n => {
     let e = n.dragging;
     window.setTimeout(() => {
         n.dragging == e && (n.dragging = null)
     }, 50)
 };
-Ee.dragover = Ee.dragenter = (n, e) => e.preventDefault();
-Ee.drop = (n, e) => {
+ae.dragover = ae.dragenter = (n, e) => e.preventDefault();
+ae.drop = (n, e) => {
     let t = e,
         r = n.dragging;
     if (n.dragging = null, !t.dataTransfer) return;
-    let i = n.posAtCoords(ii(t));
+    let i = n.posAtCoords(sr(t));
     if (!i) return;
-    let o = n.state.doc.resolve(i.pos),
-        s = r && r.slice;
-    s ? n.someProp("transformPasted", h => {
-        s = h(s, n)
-    }) : s = yc(n, t.dataTransfer.getData(jn ? "Text" : "text/plain"), jn ? null : t.dataTransfer.getData("text/html"), !1, o);
-    let l = !!(r && !t[Cc]);
-    if (n.someProp("handleDrop", h => h(n, t, s || w.empty, l))) {
+    let s = n.state.doc.resolve(i.pos),
+        o = r && r.slice;
+    o ? n.someProp("transformPasted", p => {
+        o = p(o, n)
+    }) : o = Al(n, t.dataTransfer.getData(Ut ? "Text" : "text/plain"), Ut ? null : t.dataTransfer.getData("text/html"), !1, s);
+    let l = !!(r && !t[zl]);
+    if (n.someProp("handleDrop", p => p(n, t, o || E.empty, l))) {
         t.preventDefault();
         return
     }
-    if (!s) return;
+    if (!o) return;
     t.preventDefault();
-    let a = s ? ua(n.state.doc, o.pos, s) : o.pos;
-    a == null && (a = o.pos);
+    let a = o ? ko(n.state.doc, s.pos, o) : s.pos;
+    a == null && (a = s.pos);
     let c = n.state.tr;
     l && c.deleteSelection();
     let u = c.mapping.map(a),
-        d = s.openStart == 0 && s.openEnd == 0 && s.content.childCount == 1,
+        d = o.openStart == 0 && o.openEnd == 0 && o.content.childCount == 1,
         f = c.doc;
-    if (d ? c.replaceRangeWith(u, u, s.content.firstChild) : c.replaceRange(u, u, s), c.doc.eq(f)) return;
-    let p = c.doc.resolve(u);
-    if (d && D.isSelectable(s.content.firstChild) && p.nodeAfter && p.nodeAfter.sameMarkup(s.content.firstChild)) c.setSelection(new D(p));
+    if (d ? c.replaceRangeWith(u, u, o.content.firstChild) : c.replaceRange(u, u, o), c.doc.eq(f)) return;
+    let h = c.doc.resolve(u);
+    if (d && O.isSelectable(o.content.firstChild) && h.nodeAfter && h.nodeAfter.sameMarkup(o.content.firstChild)) c.setSelection(new O(h));
     else {
-        let h = c.mapping.map(a);
-        c.mapping.maps[c.mapping.maps.length - 1].forEach((m, b, k, S) => h = S), c.setSelection(_o(n, p, c.doc.resolve(h)))
+        let p = c.mapping.map(a);
+        c.mapping.maps[c.mapping.maps.length - 1].forEach((m, b, M, w) => p = w), c.setSelection(Di(n, h, c.doc.resolve(p)))
     }
     n.focus(), n.dispatch(c.setMeta("uiEvent", "drop"))
 };
-Me.focus = n => {
+le.focus = n => {
     n.input.lastFocus = Date.now(), n.focused || (n.domObserver.stop(), n.dom.classList.add("ProseMirror-focused"), n.domObserver.start(), n.focused = !0, setTimeout(() => {
-        n.docView && n.hasFocus() && !n.domObserver.currentSelection.eq(n.domSelectionRange()) && bt(n)
+        n.docView && n.hasFocus() && !n.domObserver.currentSelection.eq(n.domSelectionRange()) && Je(n)
     }, 20))
 };
-Me.blur = (n, e) => {
+le.blur = (n, e) => {
     let t = e;
     n.focused && (n.domObserver.stop(), n.dom.classList.remove("ProseMirror-focused"), n.domObserver.start(), t.relatedTarget && n.dom.contains(t.relatedTarget) && n.domObserver.currentSelection.clear(), n.focused = !1)
 };
-Me.beforeinput = (n, e) => {
-    if (ye && Ue && e.inputType == "deleteContentBackward") {
+le.beforeinput = (n, e) => {
+    if (ie && Ee && e.inputType == "deleteContentBackward") {
         n.domObserver.flushSoon();
         let {
             domChangeCount: r
         } = n.input;
         setTimeout(() => {
-            if (n.input.domChangeCount != r || (n.dom.blur(), n.focus(), n.someProp("handleKeyDown", o => o(n, an(8, "Backspace"))))) return;
+            if (n.input.domChangeCount != r || (n.dom.blur(), n.focus(), n.someProp("handleKeyDown", s => s(n, kt(8, "Backspace"))))) return;
             let {
                 $cursor: i
             } = n.state.selection;
             i && i.pos > 0 && n.dispatch(n.state.tr.delete(i.pos - 1, i.pos).scrollIntoView())
         }, 50)
     }
 };
-for (let n in Ee) Me[n] = Ee[n];
+for (let n in ae) le[n] = ae[n];
 
-function kr(n, e) {
+function Sn(n, e) {
     if (n == e) return !0;
     for (let t in n)
         if (n[t] !== e[t]) return !1;
     for (let t in e)
         if (!(t in n)) return !1;
     return !0
 }
-var vr = class {
+var En = class {
         constructor(e, t) {
-            this.toDOM = e, this.spec = t || fn, this.side = this.spec.side || 0
+            this.toDOM = e, this.spec = t || wt, this.side = this.spec.side || 0
         }
         map(e, t, r, i) {
             let {
-                pos: o,
-                deleted: s
+                pos: s,
+                deleted: o
             } = e.mapResult(t.from + i, this.side < 0 ? -1 : 1);
-            return s ? null : new ke(o - r, o - r, this)
+            return o ? null : new se(s - r, s - r, this)
         }
         valid() {
             return !0
         }
         eq(e) {
-            return this == e || e instanceof vr && (this.spec.key && this.spec.key == e.spec.key || this.toDOM == e.toDOM && kr(this.spec, e.spec))
+            return this == e || e instanceof En && (this.spec.key && this.spec.key == e.spec.key || this.toDOM == e.toDOM && Sn(this.spec, e.spec))
         }
         destroy(e) {
             this.spec.destroy && this.spec.destroy(e)
         }
     },
-    rt = class {
+    Ie = class {
         constructor(e, t) {
-            this.attrs = e, this.spec = t || fn
+            this.attrs = e, this.spec = t || wt
         }
         map(e, t, r, i) {
-            let o = e.map(t.from + i, this.spec.inclusiveStart ? -1 : 1) - r,
-                s = e.map(t.to + i, this.spec.inclusiveEnd ? 1 : -1) - r;
-            return o >= s ? null : new ke(o, s, this)
+            let s = e.map(t.from + i, this.spec.inclusiveStart ? -1 : 1) - r,
+                o = e.map(t.to + i, this.spec.inclusiveEnd ? 1 : -1) - r;
+            return s >= o ? null : new se(s, o, this)
         }
         valid(e, t) {
             return t.from < t.to
         }
         eq(e) {
-            return this == e || e instanceof rt && kr(this.attrs, e.attrs) && kr(this.spec, e.spec)
+            return this == e || e instanceof Ie && Sn(this.attrs, e.attrs) && Sn(this.spec, e.spec)
         }
         static is(e) {
-            return e.type instanceof rt
+            return e.type instanceof Ie
         }
         destroy() {}
     },
-    Mr = class {
+    wn = class {
         constructor(e, t) {
-            this.attrs = e, this.spec = t || fn
+            this.attrs = e, this.spec = t || wt
         }
         map(e, t, r, i) {
-            let o = e.mapResult(t.from + i, 1);
-            if (o.deleted) return null;
-            let s = e.mapResult(t.to + i, -1);
-            return s.deleted || s.pos <= o.pos ? null : new ke(o.pos - r, s.pos - r, this)
+            let s = e.mapResult(t.from + i, 1);
+            if (s.deleted) return null;
+            let o = e.mapResult(t.to + i, -1);
+            return o.deleted || o.pos <= s.pos ? null : new se(s.pos - r, o.pos - r, this)
         }
         valid(e, t) {
             let {
                 index: r,
                 offset: i
-            } = e.content.findIndex(t.from), o;
-            return i == t.from && !(o = e.child(r)).isText && i + o.nodeSize == t.to
+            } = e.content.findIndex(t.from), s;
+            return i == t.from && !(s = e.child(r)).isText && i + s.nodeSize == t.to
         }
         eq(e) {
-            return this == e || e instanceof Mr && kr(this.attrs, e.attrs) && kr(this.spec, e.spec)
+            return this == e || e instanceof wn && Sn(this.attrs, e.attrs) && Sn(this.spec, e.spec)
         }
         destroy() {}
     },
-    ke = class {
+    se = class {
         constructor(e, t, r) {
             this.from = e, this.to = t, this.type = r
         }
         copy(e, t) {
-            return new ke(e, t, this.type)
+            return new se(e, t, this.type)
         }
         eq(e, t = 0) {
             return this.type.eq(e.type) && this.from + t == e.from && this.to + t == e.to
         }
         map(e, t, r) {
             return this.type.map(e, this, t, r)
         }
         static widget(e, t, r) {
-            return new ke(e, e, new vr(t, r))
+            return new se(e, e, new En(t, r))
         }
         static inline(e, t, r, i) {
-            return new ke(e, t, new rt(r, i))
+            return new se(e, t, new Ie(r, i))
         }
         static node(e, t, r, i) {
-            return new ke(e, t, new Mr(r, i))
+            return new se(e, t, new wn(r, i))
         }
         get spec() {
             return this.type.spec
         }
         get inline() {
-            return this.type instanceof rt
+            return this.type instanceof Ie
         }
     },
-    Bn = [],
-    fn = {},
-    G = class {
+    Jt = [],
+    wt = {},
+    W = class {
         constructor(e, t) {
-            this.local = e.length ? e : Bn, this.children = t.length ? t : Bn
+            this.local = e.length ? e : Jt, this.children = t.length ? t : Jt
         }
         static create(e, t) {
-            return t.length ? ei(t, e, 0, fn) : ge
+            return t.length ? tr(t, e, 0, wt) : re
         }
         find(e, t, r) {
             let i = [];
             return this.findInner(e ?? 0, t ?? 1e9, i, 0, r), i
         }
-        findInner(e, t, r, i, o) {
-            for (let s = 0; s < this.local.length; s++) {
-                let l = this.local[s];
-                l.from <= t && l.to >= e && (!o || o(l.spec)) && r.push(l.copy(l.from + i, l.to + i))
-            }
-            for (let s = 0; s < this.children.length; s += 3)
-                if (this.children[s] < t && this.children[s + 1] > e) {
-                    let l = this.children[s] + 1;
-                    this.children[s + 2].findInner(e - l, t - l, r, i + l, o)
+        findInner(e, t, r, i, s) {
+            for (let o = 0; o < this.local.length; o++) {
+                let l = this.local[o];
+                l.from <= t && l.to >= e && (!s || s(l.spec)) && r.push(l.copy(l.from + i, l.to + i))
+            }
+            for (let o = 0; o < this.children.length; o += 3)
+                if (this.children[o] < t && this.children[o + 1] > e) {
+                    let l = this.children[o] + 1;
+                    this.children[o + 2].findInner(e - l, t - l, r, i + l, s)
                 }
         }
         map(e, t, r) {
-            return this == ge || e.maps.length == 0 ? this : this.mapInner(e, t, 0, 0, r || fn)
+            return this == re || e.maps.length == 0 ? this : this.mapInner(e, t, 0, 0, r || wt)
         }
-        mapInner(e, t, r, i, o) {
-            let s;
+        mapInner(e, t, r, i, s) {
+            let o;
             for (let l = 0; l < this.local.length; l++) {
                 let a = this.local[l].map(e, r, i);
-                a && a.type.valid(t, a) ? (s || (s = [])).push(a) : o.onRemove && o.onRemove(this.local[l].spec)
+                a && a.type.valid(t, a) ? (o || (o = [])).push(a) : s.onRemove && s.onRemove(this.local[l].spec)
             }
-            return this.children.length ? $p(this.children, s || [], e, t, r, i, o) : s ? new G(s.sort(pn), Bn) : ge
+            return this.children.length ? fd(this.children, o || [], e, t, r, i, s) : o ? new W(o.sort(Tt), Jt) : re
         }
         add(e, t) {
-            return t.length ? this == ge ? G.create(e, t) : this.addInner(e, t, 0) : this
+            return t.length ? this == re ? W.create(e, t) : this.addInner(e, t, 0) : this
         }
         addInner(e, t, r) {
-            let i, o = 0;
+            let i, s = 0;
             e.forEach((l, a) => {
                 let c = a + r,
                     u;
-                if (u = Ac(t, l, c)) {
-                    for (i || (i = this.children.slice()); o < i.length && i[o] < a;) o += 3;
-                    i[o] == a ? i[o + 2] = i[o + 2].addInner(l, u, c + 1) : i.splice(o, 0, a, a + l.nodeSize, ei(u, l, c + 1, fn)), o += 3
+                if (u = Fl(t, l, c)) {
+                    for (i || (i = this.children.slice()); s < i.length && i[s] < a;) s += 3;
+                    i[s] == a ? i[s + 2] = i[s + 2].addInner(l, u, c + 1) : i.splice(s, 0, a, a + l.nodeSize, tr(u, l, c + 1, wt)), s += 3
                 }
             });
-            let s = Oc(o ? Nc(t) : t, -r);
-            for (let l = 0; l < s.length; l++) s[l].type.valid(e, s[l]) || s.splice(l--, 1);
-            return new G(s.length ? this.local.concat(s).sort(pn) : this.local, i || this.children)
+            let o = Hl(s ? jl(t) : t, -r);
+            for (let l = 0; l < o.length; l++) o[l].type.valid(e, o[l]) || o.splice(l--, 1);
+            return new W(o.length ? this.local.concat(o).sort(Tt) : this.local, i || this.children)
         }
         remove(e) {
-            return e.length == 0 || this == ge ? this : this.removeInner(e, 0)
+            return e.length == 0 || this == re ? this : this.removeInner(e, 0)
         }
         removeInner(e, t) {
             let r = this.children,
                 i = this.local;
-            for (let o = 0; o < r.length; o += 3) {
-                let s, l = r[o] + t,
-                    a = r[o + 1] + t;
-                for (let u = 0, d; u < e.length; u++)(d = e[u]) && d.from > l && d.to < a && (e[u] = null, (s || (s = [])).push(d));
-                if (!s) continue;
+            for (let s = 0; s < r.length; s += 3) {
+                let o, l = r[s] + t,
+                    a = r[s + 1] + t;
+                for (let u = 0, d; u < e.length; u++)(d = e[u]) && d.from > l && d.to < a && (e[u] = null, (o || (o = [])).push(d));
+                if (!o) continue;
                 r == this.children && (r = this.children.slice());
-                let c = r[o + 2].removeInner(s, l + 1);
-                c != ge ? r[o + 2] = c : (r.splice(o, 3), o -= 3)
+                let c = r[s + 2].removeInner(o, l + 1);
+                c != re ? r[s + 2] = c : (r.splice(s, 3), s -= 3)
             }
             if (i.length) {
-                for (let o = 0, s; o < e.length; o++)
-                    if (s = e[o])
-                        for (let l = 0; l < i.length; l++) i[l].eq(s, t) && (i == this.local && (i = this.local.slice()), i.splice(l--, 1))
+                for (let s = 0, o; s < e.length; s++)
+                    if (o = e[s])
+                        for (let l = 0; l < i.length; l++) i[l].eq(o, t) && (i == this.local && (i = this.local.slice()), i.splice(l--, 1))
             }
-            return r == this.children && i == this.local ? this : i.length || r.length ? new G(i, r) : ge
+            return r == this.children && i == this.local ? this : i.length || r.length ? new W(i, r) : re
         }
         forChild(e, t) {
-            if (this == ge) return this;
-            if (t.isLeaf) return G.empty;
+            if (this == re) return this;
+            if (t.isLeaf) return W.empty;
             let r, i;
             for (let l = 0; l < this.children.length; l += 3)
                 if (this.children[l] >= e) {
                     this.children[l] == e && (r = this.children[l + 2]);
                     break
-                } let o = e + 1,
-                s = o + t.content.size;
+                } let s = e + 1,
+                o = s + t.content.size;
             for (let l = 0; l < this.local.length; l++) {
                 let a = this.local[l];
-                if (a.from < s && a.to > o && a.type instanceof rt) {
-                    let c = Math.max(o, a.from) - o,
-                        u = Math.min(s, a.to) - o;
+                if (a.from < o && a.to > s && a.type instanceof Ie) {
+                    let c = Math.max(s, a.from) - s,
+                        u = Math.min(o, a.to) - s;
                     c < u && (i || (i = [])).push(a.copy(c, u))
                 }
             }
             if (i) {
-                let l = new G(i.sort(pn), Bn);
-                return r ? new tt([l, r]) : l
+                let l = new W(i.sort(Tt), Jt);
+                return r ? new ve([l, r]) : l
             }
-            return r || ge
+            return r || re
         }
         eq(e) {
             if (this == e) return !0;
-            if (!(e instanceof G) || this.local.length != e.local.length || this.children.length != e.children.length) return !1;
+            if (!(e instanceof W) || this.local.length != e.local.length || this.children.length != e.children.length) return !1;
             for (let t = 0; t < this.local.length; t++)
                 if (!this.local[t].eq(e.local[t])) return !1;
             for (let t = 0; t < this.children.length; t += 3)
                 if (this.children[t] != e.children[t] || this.children[t + 1] != e.children[t + 1] || !this.children[t + 2].eq(e.children[t + 2])) return !1;
             return !0
         }
         locals(e) {
-            return Xo(this.localsInner(e))
+            return Bi(this.localsInner(e))
         }
         localsInner(e) {
-            if (this == ge) return Bn;
-            if (e.inlineContent || !this.local.some(rt.is)) return this.local;
+            if (this == re) return Jt;
+            if (e.inlineContent || !this.local.some(Ie.is)) return this.local;
             let t = [];
-            for (let r = 0; r < this.local.length; r++) this.local[r].type instanceof rt || t.push(this.local[r]);
+            for (let r = 0; r < this.local.length; r++) this.local[r].type instanceof Ie || t.push(this.local[r]);
             return t
         }
     };
-G.empty = new G([], []);
-G.removeOverlap = Xo;
-var ge = G.empty,
-    tt = class {
+W.empty = new W([], []);
+W.removeOverlap = Bi;
+var re = W.empty,
+    ve = class {
         constructor(e) {
             this.members = e
         }
         map(e, t) {
-            let r = this.members.map(i => i.map(e, t, fn));
-            return tt.from(r)
+            let r = this.members.map(i => i.map(e, t, wt));
+            return ve.from(r)
         }
         forChild(e, t) {
-            if (t.isLeaf) return G.empty;
+            if (t.isLeaf) return W.empty;
             let r = [];
             for (let i = 0; i < this.members.length; i++) {
-                let o = this.members[i].forChild(e, t);
-                o != ge && (o instanceof tt ? r = r.concat(o.members) : r.push(o))
+                let s = this.members[i].forChild(e, t);
+                s != re && (s instanceof ve ? r = r.concat(s.members) : r.push(s))
             }
-            return tt.from(r)
+            return ve.from(r)
         }
         eq(e) {
-            if (!(e instanceof tt) || e.members.length != this.members.length) return !1;
+            if (!(e instanceof ve) || e.members.length != this.members.length) return !1;
             for (let t = 0; t < this.members.length; t++)
                 if (!this.members[t].eq(e.members[t])) return !1;
             return !0
         }
         locals(e) {
             let t, r = !0;
             for (let i = 0; i < this.members.length; i++) {
-                let o = this.members[i].localsInner(e);
-                if (o.length)
-                    if (!t) t = o;
+                let s = this.members[i].localsInner(e);
+                if (s.length)
+                    if (!t) t = s;
                     else {
                         r && (t = t.slice(), r = !1);
-                        for (let s = 0; s < o.length; s++) t.push(o[s])
+                        for (let o = 0; o < s.length; o++) t.push(s[o])
                     }
             }
-            return t ? Xo(r ? t : t.sort(pn)) : Bn
+            return t ? Bi(r ? t : t.sort(Tt)) : Jt
         }
         static from(e) {
             switch (e.length) {
                 case 0:
-                    return ge;
+                    return re;
                 case 1:
                     return e[0];
                 default:
-                    return new tt(e.every(t => t instanceof G) ? e : e.reduce((t, r) => t.concat(r instanceof G ? r : r.members), []))
+                    return new ve(e.every(t => t instanceof W) ? e : e.reduce((t, r) => t.concat(r instanceof W ? r : r.members), []))
             }
         }
     };
 
-function $p(n, e, t, r, i, o, s) {
+function fd(n, e, t, r, i, s, o) {
     let l = n.slice();
-    for (let c = 0, u = o; c < t.maps.length; c++) {
+    for (let c = 0, u = s; c < t.maps.length; c++) {
         let d = 0;
-        t.maps[c].forEach((f, p, h, m) => {
-            let b = m - h - (p - f);
-            for (let k = 0; k < l.length; k += 3) {
-                let S = l[k + 1];
-                if (S < 0 || f > S + u - d) continue;
-                let C = l[k] + u - d;
-                p >= C ? l[k + 1] = f <= C ? -2 : -1 : h >= i && b && (l[k] += b, l[k + 1] += b)
+        t.maps[c].forEach((f, h, p, m) => {
+            let b = m - p - (h - f);
+            for (let M = 0; M < l.length; M += 3) {
+                let w = l[M + 1];
+                if (w < 0 || f > w + u - d) continue;
+                let v = l[M] + u - d;
+                h >= v ? l[M + 1] = f <= v ? -2 : -1 : p >= i && b && (l[M] += b, l[M + 1] += b)
             }
             d += b
         }), u = t.maps[c].map(u, -1)
     }
     let a = !1;
     for (let c = 0; c < l.length; c += 3)
         if (l[c + 1] < 0) {
             if (l[c + 1] == -2) {
                 a = !0, l[c + 1] = -1;
                 continue
             }
-            let u = t.map(n[c] + o),
+            let u = t.map(n[c] + s),
                 d = u - i;
             if (d < 0 || d >= r.content.size) {
                 a = !0;
                 continue
             }
-            let f = t.map(n[c + 1] + o, -1),
-                p = f - i,
+            let f = t.map(n[c + 1] + s, -1),
+                h = f - i,
                 {
-                    index: h,
+                    index: p,
                     offset: m
                 } = r.content.findIndex(d),
-                b = r.maybeChild(h);
-            if (b && m == d && m + b.nodeSize == p) {
-                let k = l[c + 2].mapInner(t, b, u + 1, n[c] + o + 1, s);
-                k != ge ? (l[c] = d, l[c + 1] = p, l[c + 2] = k) : (l[c + 1] = -2, a = !0)
+                b = r.maybeChild(p);
+            if (b && m == d && m + b.nodeSize == h) {
+                let M = l[c + 2].mapInner(t, b, u + 1, n[c] + s + 1, o);
+                M != re ? (l[c] = d, l[c + 1] = h, l[c + 2] = M) : (l[c + 1] = -2, a = !0)
             } else a = !0
         } if (a) {
-        let c = Wp(l, n, e, t, i, o, s),
-            u = ei(c, r, 0, s);
+        let c = hd(l, n, e, t, i, s, o),
+            u = tr(c, r, 0, o);
         e = u.local;
         for (let d = 0; d < l.length; d += 3) l[d + 1] < 0 && (l.splice(d, 3), d -= 3);
         for (let d = 0, f = 0; d < u.children.length; d += 3) {
-            let p = u.children[d];
-            for (; f < l.length && l[f] < p;) f += 3;
+            let h = u.children[d];
+            for (; f < l.length && l[f] < h;) f += 3;
             l.splice(f, 0, u.children[d], u.children[d + 1], u.children[d + 2])
         }
     }
-    return new G(e.sort(pn), l)
+    return new W(e.sort(Tt), l)
 }
 
-function Oc(n, e) {
+function Hl(n, e) {
     if (!e || !n.length) return n;
     let t = [];
     for (let r = 0; r < n.length; r++) {
         let i = n[r];
-        t.push(new ke(i.from + e, i.to + e, i.type))
+        t.push(new se(i.from + e, i.to + e, i.type))
     }
     return t
 }
 
-function Wp(n, e, t, r, i, o, s) {
+function hd(n, e, t, r, i, s, o) {
     function l(a, c) {
         for (let u = 0; u < a.local.length; u++) {
             let d = a.local[u].map(r, i, c);
-            d ? t.push(d) : s.onRemove && s.onRemove(a.local[u].spec)
+            d ? t.push(d) : o.onRemove && o.onRemove(a.local[u].spec)
         }
         for (let u = 0; u < a.children.length; u += 3) l(a.children[u + 2], a.children[u] + c + 1)
     }
-    for (let a = 0; a < n.length; a += 3) n[a + 1] == -1 && l(n[a + 2], e[a] + o + 1);
+    for (let a = 0; a < n.length; a += 3) n[a + 1] == -1 && l(n[a + 2], e[a] + s + 1);
     return t
 }
 
-function Ac(n, e, t) {
+function Fl(n, e, t) {
     if (e.isLeaf) return null;
     let r = t + e.nodeSize,
         i = null;
-    for (let o = 0, s; o < n.length; o++)(s = n[o]) && s.from > t && s.to < r && ((i || (i = [])).push(s), n[o] = null);
+    for (let s = 0, o; s < n.length; s++)(o = n[s]) && o.from > t && o.to < r && ((i || (i = [])).push(o), n[s] = null);
     return i
 }
 
-function Nc(n) {
+function jl(n) {
     let e = [];
     for (let t = 0; t < n.length; t++) n[t] != null && e.push(n[t]);
     return e
 }
 
-function ei(n, e, t, r) {
+function tr(n, e, t, r) {
     let i = [],
-        o = !1;
+        s = !1;
     e.forEach((l, a) => {
-        let c = Ac(n, l, a + t);
+        let c = Fl(n, l, a + t);
         if (c) {
-            o = !0;
-            let u = ei(c, l, t + a + 1, r);
-            u != ge && i.push(a, a + l.nodeSize, u)
+            s = !0;
+            let u = tr(c, l, t + a + 1, r);
+            u != re && i.push(a, a + l.nodeSize, u)
         }
     });
-    let s = Oc(o ? Nc(n) : n, -t).sort(pn);
-    for (let l = 0; l < s.length; l++) s[l].type.valid(e, s[l]) || (r.onRemove && r.onRemove(s[l].spec), s.splice(l--, 1));
-    return s.length || i.length ? new G(s, i) : ge
+    let o = Hl(s ? jl(n) : n, -t).sort(Tt);
+    for (let l = 0; l < o.length; l++) o[l].type.valid(e, o[l]) || (r.onRemove && r.onRemove(o[l].spec), o.splice(l--, 1));
+    return o.length || i.length ? new W(o, i) : re
 }
 
-function pn(n, e) {
+function Tt(n, e) {
     return n.from - e.from || n.to - e.to
 }
 
-function Xo(n) {
+function Bi(n) {
     let e = n;
     for (let t = 0; t < e.length - 1; t++) {
         let r = e[t];
         if (r.from != r.to)
             for (let i = t + 1; i < e.length; i++) {
-                let o = e[i];
-                if (o.from == r.from) {
-                    o.to != r.to && (e == n && (e = n.slice()), e[i] = o.copy(o.from, r.to), Ka(e, i + 1, o.copy(r.to, o.to)));
+                let s = e[i];
+                if (s.from == r.from) {
+                    s.to != r.to && (e == n && (e = n.slice()), e[i] = s.copy(s.from, r.to), nl(e, i + 1, s.copy(r.to, s.to)));
                     continue
                 } else {
-                    o.from < r.to && (e == n && (e = n.slice()), e[t] = r.copy(r.from, o.from), Ka(e, i, r.copy(o.from, r.to)));
+                    s.from < r.to && (e == n && (e = n.slice()), e[t] = r.copy(r.from, s.from), nl(e, i, r.copy(s.from, r.to)));
                     break
                 }
             }
     }
     return e
 }
 
-function Ka(n, e, t) {
-    for (; e < n.length && pn(t, n[e]) > 0;) e++;
+function nl(n, e, t) {
+    for (; e < n.length && Tt(t, n[e]) > 0;) e++;
     n.splice(e, 0, t)
 }
 
-function To(n) {
+function ui(n) {
     let e = [];
     return n.someProp("decorations", t => {
         let r = t(n.state);
-        r && r != ge && e.push(r)
-    }), n.cursorWrapper && e.push(G.create(n.state.doc, [n.cursorWrapper.deco])), tt.from(e)
+        r && r != re && e.push(r)
+    }), n.cursorWrapper && e.push(W.create(n.state.doc, [n.cursorWrapper.deco])), ve.from(e)
 }
-var qp = {
+var pd = {
         childList: !0,
         characterData: !0,
         characterDataOldValue: !0,
         attributes: !0,
         attributeOldValue: !0,
         subtree: !0
     },
-    Jp = Ce && Lt <= 11,
-    qo = class {
+    md = fe && Ze <= 11,
+    Oi = class {
         constructor() {
             this.anchorNode = null, this.anchorOffset = 0, this.focusNode = null, this.focusOffset = 0
         }
         set(e) {
             this.anchorNode = e.anchorNode, this.anchorOffset = e.anchorOffset, this.focusNode = e.focusNode, this.focusOffset = e.focusOffset
         }
         clear() {
             this.anchorNode = this.focusNode = null
         }
         eq(e) {
             return e.anchorNode == this.anchorNode && e.anchorOffset == this.anchorOffset && e.focusNode == this.focusNode && e.focusOffset == this.focusOffset
         }
     },
-    Jo = class {
+    vi = class {
         constructor(e, t) {
-            this.view = e, this.handleDOMChange = t, this.queue = [], this.flushingSoon = -1, this.observer = null, this.currentSelection = new qo, this.onCharData = null, this.suppressingSelectionUpdates = !1, this.observer = window.MutationObserver && new window.MutationObserver(r => {
+            this.view = e, this.handleDOMChange = t, this.queue = [], this.flushingSoon = -1, this.observer = null, this.currentSelection = new Oi, this.onCharData = null, this.suppressingSelectionUpdates = !1, this.observer = window.MutationObserver && new window.MutationObserver(r => {
                 for (let i = 0; i < r.length; i++) this.queue.push(r[i]);
-                Ce && Lt <= 11 && r.some(i => i.type == "childList" && i.removedNodes.length || i.type == "characterData" && i.oldValue.length > i.target.nodeValue.length) ? this.flushSoon() : this.flush()
-            }), Jp && (this.onCharData = r => {
+                fe && Ze <= 11 && r.some(i => i.type == "childList" && i.removedNodes.length || i.type == "characterData" && i.oldValue.length > i.target.nodeValue.length) ? this.flushSoon() : this.flush()
+            }), md && (this.onCharData = r => {
                 this.queue.push({
                     target: r.target,
                     type: "characterData",
                     oldValue: r.prevValue
                 }), this.flushSoon()
             }), this.onSelectionChange = this.onSelectionChange.bind(this)
         }
@@ -7971,15 +6741,15 @@
                 this.flushingSoon = -1, this.flush()
             }, 20))
         }
         forceFlush() {
             this.flushingSoon > -1 && (window.clearTimeout(this.flushingSoon), this.flushingSoon = -1, this.flush())
         }
         start() {
-            this.observer && (this.observer.takeRecords(), this.observer.observe(this.view.dom, qp)), this.onCharData && this.view.dom.addEventListener("DOMCharacterDataModified", this.onCharData), this.connectSelection()
+            this.observer && (this.observer.takeRecords(), this.observer.observe(this.view.dom, pd)), this.onCharData && this.view.dom.addEventListener("DOMCharacterDataModified", this.onCharData), this.connectSelection()
         }
         stop() {
             if (this.observer) {
                 let e = this.observer.takeRecords();
                 if (e.length) {
                     for (let t = 0; t < e.length; t++) this.queue.push(e[t]);
                     window.setTimeout(() => this.flush(), 20)
@@ -7994,34 +6764,34 @@
         disconnectSelection() {
             this.view.dom.ownerDocument.removeEventListener("selectionchange", this.onSelectionChange)
         }
         suppressSelectionUpdates() {
             this.suppressingSelectionUpdates = !0, setTimeout(() => this.suppressingSelectionUpdates = !1, 50)
         }
         onSelectionChange() {
-            if (Ha(this.view)) {
-                if (this.suppressingSelectionUpdates) return bt(this.view);
-                if (Ce && Lt <= 11 && !this.view.state.selection.empty) {
+            if (_o(this.view)) {
+                if (this.suppressingSelectionUpdates) return Je(this.view);
+                if (fe && Ze <= 11 && !this.view.state.selection.empty) {
                     let e = this.view.domSelectionRange();
-                    if (e.focusNode && hn(e.focusNode, e.focusOffset, e.anchorNode, e.anchorOffset)) return this.flushSoon()
+                    if (e.focusNode && Ct(e.focusNode, e.focusOffset, e.anchorNode, e.anchorOffset)) return this.flushSoon()
                 }
                 this.flush()
             }
         }
         setCurSelection() {
             this.currentSelection.set(this.view.domSelectionRange())
         }
         ignoreSelectionChange(e) {
             if (!e.focusNode) return !0;
             let t = new Set,
                 r;
-            for (let o = e.focusNode; o; o = xr(o)) t.add(o);
-            for (let o = e.anchorNode; o; o = xr(o))
-                if (t.has(o)) {
-                    r = o;
+            for (let s = e.focusNode; s; s = kn(s)) t.add(s);
+            for (let s = e.anchorNode; s; s = kn(s))
+                if (t.has(s)) {
+                    r = s;
                     break
                 } let i = r && this.view.docView.nearestDesc(r);
             if (i && i.ignoreMutation({
                     type: "selection",
                     target: r.nodeType == 3 ? r.parentNode : r
                 })) return this.setCurSelection(), !0
         }
@@ -8029,58 +6799,58 @@
             let {
                 view: e
             } = this;
             if (!e.docView || this.flushingSoon > -1) return;
             let t = this.observer ? this.observer.takeRecords() : [];
             this.queue.length && (t = this.queue.concat(t), this.queue.length = 0);
             let r = e.domSelectionRange(),
-                i = !this.suppressingSelectionUpdates && !this.currentSelection.eq(r) && Ha(e) && !this.ignoreSelectionChange(r),
-                o = -1,
+                i = !this.suppressingSelectionUpdates && !this.currentSelection.eq(r) && _o(e) && !this.ignoreSelectionChange(r),
                 s = -1,
+                o = -1,
                 l = !1,
                 a = [];
             if (e.editable)
                 for (let u = 0; u < t.length; u++) {
                     let d = this.registerMutation(t[u], a);
-                    d && (o = o < 0 ? d.from : Math.min(d.from, o), s = s < 0 ? d.to : Math.max(d.to, s), d.typeOver && (l = !0))
+                    d && (s = s < 0 ? d.from : Math.min(d.from, s), o = o < 0 ? d.to : Math.max(d.to, o), d.typeOver && (l = !0))
                 }
-            if (_e && a.length > 1) {
+            if (we && a.length > 1) {
                 let u = a.filter(d => d.nodeName == "BR");
                 if (u.length == 2) {
                     let d = u[0],
                         f = u[1];
                     d.parentNode && d.parentNode.parentNode == f.parentNode ? f.remove() : d.remove()
                 }
             }
             let c = null;
-            o < 0 && i && e.input.lastFocus > Date.now() - 200 && Math.max(e.input.lastTouch, e.input.lastClick.time) < Date.now() - 300 && ni(r) && (c = Uo(e)) && c.eq(R.near(e.state.doc.resolve(0), 1)) ? (e.input.lastFocus = 0, bt(e), this.currentSelection.set(r), e.scrollToSelection()) : (o > -1 || i) && (o > -1 && (e.docView.markDirty(o, s), Kp(e)), this.handleDOMChange(o, s, l, a), e.docView && e.docView.dirty ? e.updateState(e.state) : this.currentSelection.eq(r) || bt(e), this.currentSelection.set(r))
+            s < 0 && i && e.input.lastFocus > Date.now() - 200 && Math.max(e.input.lastTouch, e.input.lastClick.time) < Date.now() - 300 && rr(r) && (c = Ii(e)) && c.eq(L.near(e.state.doc.resolve(0), 1)) ? (e.input.lastFocus = 0, Je(e), this.currentSelection.set(r), e.scrollToSelection()) : (s > -1 || i) && (s > -1 && (e.docView.markDirty(s, o), gd(e)), this.handleDOMChange(s, o, l, a), e.docView && e.docView.dirty ? e.updateState(e.state) : this.currentSelection.eq(r) || Je(e), this.currentSelection.set(r))
         }
         registerMutation(e, t) {
             if (t.indexOf(e.target) > -1) return null;
             let r = this.view.docView.nearestDesc(e.target);
             if (e.type == "attributes" && (r == this.view.docView || e.attributeName == "contenteditable" || e.attributeName == "style" && !e.oldValue && !e.target.getAttribute("style")) || !r || r.ignoreMutation(e)) return null;
             if (e.type == "childList") {
                 for (let u = 0; u < e.addedNodes.length; u++) t.push(e.addedNodes[u]);
                 if (r.contentDOM && r.contentDOM != r.dom && !r.contentDOM.contains(e.target)) return {
                     from: r.posBefore,
                     to: r.posAfter
                 };
                 let i = e.previousSibling,
-                    o = e.nextSibling;
-                if (Ce && Lt <= 11 && e.addedNodes.length)
+                    s = e.nextSibling;
+                if (fe && Ze <= 11 && e.addedNodes.length)
                     for (let u = 0; u < e.addedNodes.length; u++) {
                         let {
                             previousSibling: d,
                             nextSibling: f
                         } = e.addedNodes[u];
-                        (!d || Array.prototype.indexOf.call(e.addedNodes, d) < 0) && (i = d), (!f || Array.prototype.indexOf.call(e.addedNodes, f) < 0) && (o = f)
+                        (!d || Array.prototype.indexOf.call(e.addedNodes, d) < 0) && (i = d), (!f || Array.prototype.indexOf.call(e.addedNodes, f) < 0) && (s = f)
                     }
-                let s = i && i.parentNode == e.target ? Fe(i) + 1 : 0,
-                    l = r.localPosFromDOM(e.target, s, -1),
-                    a = o && o.parentNode == e.target ? Fe(o) : e.target.childNodes.length,
+                let o = i && i.parentNode == e.target ? be(i) + 1 : 0,
+                    l = r.localPosFromDOM(e.target, o, -1),
+                    a = s && s.parentNode == e.target ? be(s) : e.target.childNodes.length,
                     c = r.localPosFromDOM(e.target, a, 1);
                 return {
                     from: l,
                     to: c
                 }
             } else return e.type == "attributes" ? {
                 from: r.posAtStart - r.border,
@@ -8088,334 +6858,334 @@
             } : {
                 from: r.posAtStart,
                 to: r.posAtEnd,
                 typeOver: e.target.nodeValue == e.oldValue
             }
         }
     },
-    Ua = new WeakMap,
-    _a = !1;
+    rl = new WeakMap,
+    il = !1;
 
-function Kp(n) {
-    if (!Ua.has(n) && (Ua.set(n, null), ["normal", "nowrap", "pre-line"].indexOf(getComputedStyle(n.dom).whiteSpace) !== -1)) {
-        if (n.requiresGeckoHackNode = _e, _a) return;
-        console.warn("ProseMirror expects the CSS white-space property to be set, preferably to 'pre-wrap'. It is recommended to load style/prosemirror.css from the prosemirror-view package."), _a = !0
+function gd(n) {
+    if (!rl.has(n) && (rl.set(n, null), ["normal", "nowrap", "pre-line"].indexOf(getComputedStyle(n.dom).whiteSpace) !== -1)) {
+        if (n.requiresGeckoHackNode = we, il) return;
+        console.warn("ProseMirror expects the CSS white-space property to be set, preferably to 'pre-wrap'. It is recommended to load style/prosemirror.css from the prosemirror-view package."), il = !0
     }
 }
 
-function Up(n) {
+function yd(n) {
     let e;
 
     function t(a) {
         a.preventDefault(), a.stopImmediatePropagation(), e = a.getTargetRanges()[0]
     }
     n.dom.addEventListener("beforeinput", t, !0), document.execCommand("indent"), n.dom.removeEventListener("beforeinput", t, !0);
     let r = e.startContainer,
         i = e.startOffset,
-        o = e.endContainer,
-        s = e.endOffset,
+        s = e.endContainer,
+        o = e.endOffset,
         l = n.domAtPos(n.state.selection.anchor);
-    return hn(l.node, l.offset, o, s) && ([r, i, o, s] = [o, s, r, i]), {
+    return Ct(l.node, l.offset, s, o) && ([r, i, s, o] = [s, o, r, i]), {
         anchorNode: r,
         anchorOffset: i,
-        focusNode: o,
-        focusOffset: s
+        focusNode: s,
+        focusOffset: o
     }
 }
 
-function _p(n, e, t) {
+function bd(n, e, t) {
     let {
         node: r,
         fromOffset: i,
-        toOffset: o,
-        from: s,
+        toOffset: s,
+        from: o,
         to: l
     } = n.docView.parseRange(e, t), a = n.domSelectionRange(), c, u = a.anchorNode;
     if (u && n.dom.contains(u.nodeType == 1 ? u : u.parentNode) && (c = [{
             node: u,
             offset: a.anchorOffset
-        }], ni(a) || c.push({
+        }], rr(a) || c.push({
             node: a.focusNode,
             offset: a.focusOffset
-        })), ye && n.input.lastKeyCode === 8)
-        for (let b = o; b > i; b--) {
-            let k = r.childNodes[b - 1],
-                S = k.pmViewDesc;
-            if (k.nodeName == "BR" && !S) {
-                o = b;
+        })), ie && n.input.lastKeyCode === 8)
+        for (let b = s; b > i; b--) {
+            let M = r.childNodes[b - 1],
+                w = M.pmViewDesc;
+            if (M.nodeName == "BR" && !w) {
+                s = b;
                 break
             }
-            if (!S || S.size) break
+            if (!w || w.size) break
         }
     let d = n.state.doc,
-        f = n.someProp("domParser") || Qe.fromSchema(n.state.schema),
-        p = d.resolve(s),
-        h = null,
+        f = n.someProp("domParser") || Te.fromSchema(n.state.schema),
+        h = d.resolve(o),
+        p = null,
         m = f.parse(r, {
-            topNode: p.parent,
-            topMatch: p.parent.contentMatchAt(p.index()),
+            topNode: h.parent,
+            topMatch: h.parent.contentMatchAt(h.index()),
             topOpen: !0,
             from: i,
-            to: o,
-            preserveWhitespace: p.parent.type.whitespace == "pre" ? "full" : !0,
+            to: s,
+            preserveWhitespace: h.parent.type.whitespace == "pre" ? "full" : !0,
             findPositions: c,
-            ruleFromNode: Gp,
-            context: p
+            ruleFromNode: xd,
+            context: h
         });
     if (c && c[0].pos != null) {
         let b = c[0].pos,
-            k = c[1] && c[1].pos;
-        k == null && (k = b), h = {
-            anchor: b + s,
-            head: k + s
+            M = c[1] && c[1].pos;
+        M == null && (M = b), p = {
+            anchor: b + o,
+            head: M + o
         }
     }
     return {
         doc: m,
-        sel: h,
-        from: s,
+        sel: p,
+        from: o,
         to: l
     }
 }
 
-function Gp(n) {
+function xd(n) {
     let e = n.pmViewDesc;
     if (e) return e.parseRule();
     if (n.nodeName == "BR" && n.parentNode) {
-        if (ve && /^(ul|ol)$/i.test(n.parentNode.nodeName)) {
+        if (oe && /^(ul|ol)$/i.test(n.parentNode.nodeName)) {
             let t = document.createElement("div");
             return t.appendChild(document.createElement("li")), {
                 skip: t
             }
-        } else if (n.parentNode.lastChild == n || ve && /^(tr|table)$/i.test(n.parentNode.nodeName)) return {
+        } else if (n.parentNode.lastChild == n || oe && /^(tr|table)$/i.test(n.parentNode.nodeName)) return {
             ignore: !0
         }
     } else if (n.nodeName == "IMG" && n.getAttribute("mark-placeholder")) return {
         ignore: !0
     };
     return null
 }
-var Yp = /^(a|abbr|acronym|b|bd[io]|big|br|button|cite|code|data(list)?|del|dfn|em|i|ins|kbd|label|map|mark|meter|output|q|ruby|s|samp|small|span|strong|su[bp]|time|u|tt|var)$/i;
+var kd = /^(a|abbr|acronym|b|bd[io]|big|br|button|cite|code|data(list)?|del|dfn|em|i|ins|kbd|label|map|mark|meter|output|q|ruby|s|samp|small|span|strong|su[bp]|time|u|tt|var)$/i;
 
-function Qp(n, e, t, r, i) {
+function Md(n, e, t, r, i) {
     if (e < 0) {
         let y = n.input.lastSelectionTime > Date.now() - 50 ? n.input.lastSelectionOrigin : null,
-            O = Uo(n, y);
-        if (O && !n.state.selection.eq(O)) {
-            if (ye && Ue && n.input.lastKeyCode === 13 && Date.now() - 100 < n.input.lastKeyCodeTime && n.someProp("handleKeyDown", L => L(n, an(13, "Enter")))) return;
-            let I = n.state.tr.setSelection(O);
-            y == "pointer" ? I.setMeta("pointer", !0) : y == "key" && I.scrollIntoView(), n.composing && I.setMeta("composition", n.input.compositionID), n.dispatch(I)
+            N = Ii(n, y);
+        if (N && !n.state.selection.eq(N)) {
+            if (ie && Ee && n.input.lastKeyCode === 13 && Date.now() - 100 < n.input.lastKeyCodeTime && n.someProp("handleKeyDown", Q => Q(n, kt(13, "Enter")))) return;
+            let z = n.state.tr.setSelection(N);
+            y == "pointer" ? z.setMeta("pointer", !0) : y == "key" && z.scrollIntoView(), n.composing && z.setMeta("composition", n.input.compositionID), n.dispatch(z)
         }
         return
     }
-    let o = n.state.doc.resolve(e),
-        s = o.sharedDepth(t);
-    e = o.before(s + 1), t = n.state.doc.resolve(t).after(s + 1);
+    let s = n.state.doc.resolve(e),
+        o = s.sharedDepth(t);
+    e = s.before(o + 1), t = n.state.doc.resolve(t).after(o + 1);
     let l = n.state.selection,
-        a = _p(n, e, t),
+        a = bd(n, e, t),
         c = n.state.doc,
         u = c.slice(a.from, a.to),
         d, f;
     n.input.lastKeyCode === 8 && Date.now() - 100 < n.input.lastKeyCodeTime ? (d = n.state.selection.to, f = "end") : (d = n.state.selection.from, f = "start"), n.input.lastKeyCode = null;
-    let p = eh(u.content, a.doc.content, a.from, d, f);
-    if ((Hn && n.input.lastIOSEnter > Date.now() - 225 || Ue) && i.some(y => y.nodeType == 1 && !Yp.test(y.nodeName)) && (!p || p.endA >= p.endB) && n.someProp("handleKeyDown", y => y(n, an(13, "Enter")))) {
+    let h = wd(u.content, a.doc.content, a.from, d, f);
+    if ((qt && n.input.lastIOSEnter > Date.now() - 225 || Ee) && i.some(y => y.nodeType == 1 && !kd.test(y.nodeName)) && (!h || h.endA >= h.endB) && n.someProp("handleKeyDown", y => y(n, kt(13, "Enter")))) {
         n.input.lastIOSEnter = 0;
         return
     }
-    if (!p)
-        if (r && l instanceof P && !l.empty && l.$head.sameParent(l.$anchor) && !n.composing && !(a.sel && a.sel.anchor != a.sel.head)) p = {
+    if (!h)
+        if (r && l instanceof I && !l.empty && l.$head.sameParent(l.$anchor) && !n.composing && !(a.sel && a.sel.anchor != a.sel.head)) h = {
             start: l.from,
             endA: l.to,
             endB: l.to
         };
         else {
             if (a.sel) {
-                let y = Ga(n, n.state.doc, a.sel);
+                let y = sl(n, n.state.doc, a.sel);
                 if (y && !y.eq(n.state.selection)) {
-                    let O = n.state.tr.setSelection(y);
-                    n.composing && O.setMeta("composition", n.input.compositionID), n.dispatch(O)
+                    let N = n.state.tr.setSelection(y);
+                    n.composing && N.setMeta("composition", n.input.compositionID), n.dispatch(N)
                 }
             }
             return
-        } if (ye && n.cursorWrapper && a.sel && a.sel.anchor == n.cursorWrapper.deco.from && a.sel.head == a.sel.anchor) {
-        let y = p.endB - p.start;
+        } if (ie && n.cursorWrapper && a.sel && a.sel.anchor == n.cursorWrapper.deco.from && a.sel.head == a.sel.anchor) {
+        let y = h.endB - h.start;
         a.sel = {
             anchor: a.sel.anchor + y,
             head: a.sel.anchor + y
         }
     }
-    n.input.domChangeCount++, n.state.selection.from < n.state.selection.to && p.start == p.endB && n.state.selection instanceof P && (p.start > n.state.selection.from && p.start <= n.state.selection.from + 2 && n.state.selection.from >= a.from ? p.start = n.state.selection.from : p.endA < n.state.selection.to && p.endA >= n.state.selection.to - 2 && n.state.selection.to <= a.to && (p.endB += n.state.selection.to - p.endA, p.endA = n.state.selection.to)), Ce && Lt <= 11 && p.endB == p.start + 1 && p.endA == p.start && p.start > a.from && a.doc.textBetween(p.start - a.from - 1, p.start - a.from + 1) == " \xA0" && (p.start--, p.endA--, p.endB--);
-    let h = a.doc.resolveNoCache(p.start - a.from),
-        m = a.doc.resolveNoCache(p.endB - a.from),
-        b = c.resolve(p.start),
-        k = h.sameParent(m) && h.parent.inlineContent && b.end() >= p.endA,
-        S;
-    if ((Hn && n.input.lastIOSEnter > Date.now() - 225 && (!k || i.some(y => y.nodeName == "DIV" || y.nodeName == "P")) || !k && h.pos < a.doc.content.size && (S = R.findFrom(a.doc.resolve(h.pos + 1), 1, !0)) && S.head == m.pos) && n.someProp("handleKeyDown", y => y(n, an(13, "Enter")))) {
+    n.input.domChangeCount++, n.state.selection.from < n.state.selection.to && h.start == h.endB && n.state.selection instanceof I && (h.start > n.state.selection.from && h.start <= n.state.selection.from + 2 && n.state.selection.from >= a.from ? h.start = n.state.selection.from : h.endA < n.state.selection.to && h.endA >= n.state.selection.to - 2 && n.state.selection.to <= a.to && (h.endB += n.state.selection.to - h.endA, h.endA = n.state.selection.to)), fe && Ze <= 11 && h.endB == h.start + 1 && h.endA == h.start && h.start > a.from && a.doc.textBetween(h.start - a.from - 1, h.start - a.from + 1) == " \xA0" && (h.start--, h.endA--, h.endB--);
+    let p = a.doc.resolveNoCache(h.start - a.from),
+        m = a.doc.resolveNoCache(h.endB - a.from),
+        b = c.resolve(h.start),
+        M = p.sameParent(m) && p.parent.inlineContent && b.end() >= h.endA,
+        w;
+    if ((qt && n.input.lastIOSEnter > Date.now() - 225 && (!M || i.some(y => y.nodeName == "DIV" || y.nodeName == "P")) || !M && p.pos < a.doc.content.size && (w = L.findFrom(a.doc.resolve(p.pos + 1), 1, !0)) && w.head == m.pos) && n.someProp("handleKeyDown", y => y(n, kt(13, "Enter")))) {
         n.input.lastIOSEnter = 0;
         return
     }
-    if (n.state.selection.anchor > p.start && Zp(c, p.start, p.endA, h, m) && n.someProp("handleKeyDown", y => y(n, an(8, "Backspace")))) {
-        Ue && ye && n.domObserver.suppressSelectionUpdates();
+    if (n.state.selection.anchor > h.start && Ed(c, h.start, h.endA, p, m) && n.someProp("handleKeyDown", y => y(n, kt(8, "Backspace")))) {
+        Ee && ie && n.domObserver.suppressSelectionUpdates();
         return
     }
-    ye && Ue && p.endB == p.start && (n.input.lastAndroidDelete = Date.now()), Ue && !k && h.start() != m.start() && m.parentOffset == 0 && h.depth == m.depth && a.sel && a.sel.anchor == a.sel.head && a.sel.head == p.endA && (p.endB -= 2, m = a.doc.resolveNoCache(p.endB - a.from), setTimeout(() => {
+    ie && Ee && h.endB == h.start && (n.input.lastAndroidDelete = Date.now()), Ee && !M && p.start() != m.start() && m.parentOffset == 0 && p.depth == m.depth && a.sel && a.sel.anchor == a.sel.head && a.sel.head == h.endA && (h.endB -= 2, m = a.doc.resolveNoCache(h.endB - a.from), setTimeout(() => {
         n.someProp("handleKeyDown", function(y) {
-            return y(n, an(13, "Enter"))
+            return y(n, kt(13, "Enter"))
         })
     }, 20));
-    let C = p.start,
-        T = p.endA,
-        E, g, x;
-    if (k) {
-        if (h.pos == m.pos) Ce && Lt <= 11 && h.parentOffset == 0 && (n.domObserver.suppressSelectionUpdates(), setTimeout(() => bt(n), 20)), E = n.state.tr.delete(C, T), g = c.resolve(p.start).marksAcross(c.resolve(p.endA));
-        else if (p.endA == p.endB && (x = Xp(h.parent.content.cut(h.parentOffset, m.parentOffset), b.parent.content.cut(b.parentOffset, p.endA - b.start())))) E = n.state.tr, x.type == "add" ? E.addMark(C, T, x.mark) : E.removeMark(C, T, x.mark);
-        else if (h.parent.child(h.index()).isText && h.index() == m.index() - (m.textOffset ? 0 : 1)) {
-            let y = h.parent.textBetween(h.parentOffset, m.parentOffset);
-            if (n.someProp("handleTextInput", O => O(n, C, T, y))) return;
-            E = n.state.tr.insertText(y, C, T)
+    let v = h.start,
+        D = h.endA,
+        A, g, k;
+    if (M) {
+        if (p.pos == m.pos) fe && Ze <= 11 && p.parentOffset == 0 && (n.domObserver.suppressSelectionUpdates(), setTimeout(() => Je(n), 20)), A = n.state.tr.delete(v, D), g = c.resolve(h.start).marksAcross(c.resolve(h.endA));
+        else if (h.endA == h.endB && (k = Sd(p.parent.content.cut(p.parentOffset, m.parentOffset), b.parent.content.cut(b.parentOffset, h.endA - b.start())))) A = n.state.tr, k.type == "add" ? A.addMark(v, D, k.mark) : A.removeMark(v, D, k.mark);
+        else if (p.parent.child(p.index()).isText && p.index() == m.index() - (m.textOffset ? 0 : 1)) {
+            let y = p.parent.textBetween(p.parentOffset, m.parentOffset);
+            if (n.someProp("handleTextInput", N => N(n, v, D, y))) return;
+            A = n.state.tr.insertText(y, v, D)
         }
     }
-    if (E || (E = n.state.tr.replace(C, T, a.doc.slice(p.start - a.from, p.endB - a.from))), a.sel) {
-        let y = Ga(n, E.doc, a.sel);
-        y && !(ye && Ue && n.composing && y.empty && (p.start != p.endB || n.input.lastAndroidDelete < Date.now() - 100) && (y.head == C || y.head == E.mapping.map(T) - 1) || Ce && y.empty && y.head == C) && E.setSelection(y)
+    if (A || (A = n.state.tr.replace(v, D, a.doc.slice(h.start - a.from, h.endB - a.from))), a.sel) {
+        let y = sl(n, A.doc, a.sel);
+        y && !(ie && Ee && n.composing && y.empty && (h.start != h.endB || n.input.lastAndroidDelete < Date.now() - 100) && (y.head == v || y.head == A.mapping.map(D) - 1) || fe && y.empty && y.head == v) && A.setSelection(y)
     }
-    g && E.ensureMarks(g), n.composing && E.setMeta("composition", n.input.compositionID), n.dispatch(E.scrollIntoView())
+    g && A.ensureMarks(g), n.composing && A.setMeta("composition", n.input.compositionID), n.dispatch(A.scrollIntoView())
 }
 
-function Ga(n, e, t) {
-    return Math.max(t.anchor, t.head) > e.content.size ? null : _o(n, e.resolve(t.anchor), e.resolve(t.head))
+function sl(n, e, t) {
+    return Math.max(t.anchor, t.head) > e.content.size ? null : Di(n, e.resolve(t.anchor), e.resolve(t.head))
 }
 
-function Xp(n, e) {
+function Sd(n, e) {
     let t = n.firstChild.marks,
         r = e.firstChild.marks,
         i = t,
-        o = r,
-        s, l, a;
+        s = r,
+        o, l, a;
     for (let u = 0; u < r.length; u++) i = r[u].removeFromSet(i);
-    for (let u = 0; u < t.length; u++) o = t[u].removeFromSet(o);
-    if (i.length == 1 && o.length == 0) l = i[0], s = "add", a = u => u.mark(l.addToSet(u.marks));
-    else if (i.length == 0 && o.length == 1) l = o[0], s = "remove", a = u => u.mark(l.removeFromSet(u.marks));
+    for (let u = 0; u < t.length; u++) s = t[u].removeFromSet(s);
+    if (i.length == 1 && s.length == 0) l = i[0], o = "add", a = u => u.mark(l.addToSet(u.marks));
+    else if (i.length == 0 && s.length == 1) l = s[0], o = "remove", a = u => u.mark(l.removeFromSet(u.marks));
     else return null;
     let c = [];
     for (let u = 0; u < e.childCount; u++) c.push(a(e.child(u)));
-    if (v.from(c).eq(n)) return {
+    if (x.from(c).eq(n)) return {
         mark: l,
-        type: s
+        type: o
     }
 }
 
-function Zp(n, e, t, r, i) {
-    if (!r.parent.isTextblock || t - e <= i.pos - r.pos || Co(r, !0, !1) < i.pos) return !1;
-    let o = n.resolve(e);
-    if (o.parentOffset < o.parent.content.size || !o.parent.isTextblock) return !1;
-    let s = n.resolve(Co(o, !0, !0));
-    return !s.parent.isTextblock || s.pos > t || Co(s, !0, !1) < t ? !1 : r.parent.content.cut(r.parentOffset).eq(s.parent.content)
+function Ed(n, e, t, r, i) {
+    if (!r.parent.isTextblock || t - e <= i.pos - r.pos || di(r, !0, !1) < i.pos) return !1;
+    let s = n.resolve(e);
+    if (s.parentOffset < s.parent.content.size || !s.parent.isTextblock) return !1;
+    let o = n.resolve(di(s, !0, !0));
+    return !o.parent.isTextblock || o.pos > t || di(o, !0, !1) < t ? !1 : r.parent.content.cut(r.parentOffset).eq(o.parent.content)
 }
 
-function Co(n, e, t) {
+function di(n, e, t) {
     let r = n.depth,
         i = e ? n.end() : n.pos;
     for (; r > 0 && (e || n.indexAfter(r) == n.node(r).childCount);) r--, i++, e = !1;
     if (t) {
-        let o = n.node(r).maybeChild(n.indexAfter(r));
-        for (; o && !o.isLeaf;) o = o.firstChild, i++
+        let s = n.node(r).maybeChild(n.indexAfter(r));
+        for (; s && !s.isLeaf;) s = s.firstChild, i++
     }
     return i
 }
 
-function eh(n, e, t, r, i) {
-    let o = n.findDiffStart(e, t);
-    if (o == null) return null;
+function wd(n, e, t, r, i) {
+    let s = n.findDiffStart(e, t);
+    if (s == null) return null;
     let {
-        a: s,
+        a: o,
         b: l
     } = n.findDiffEnd(e, t + n.size, t + e.size);
     if (i == "end") {
-        let a = Math.max(0, o - Math.min(s, l));
-        r -= s + a - o
+        let a = Math.max(0, s - Math.min(o, l));
+        r -= o + a - s
     }
-    if (s < o && n.size < e.size) {
-        let a = r <= o && r >= s ? o - r : 0;
-        o -= a, l = o + (l - s), s = o
-    } else if (l < o) {
-        let a = r <= o && r >= l ? o - r : 0;
-        o -= a, s = o + (s - l), l = o
+    if (o < s && n.size < e.size) {
+        let a = r <= s && r >= o ? s - r : 0;
+        s -= a, l = s + (l - o), o = s
+    } else if (l < s) {
+        let a = r <= s && r >= l ? s - r : 0;
+        s -= a, o = s + (o - l), l = s
     }
     return {
-        start: o,
-        endA: s,
+        start: s,
+        endA: o,
         endB: l
     }
 }
-var ti = class {
+var nr = class {
     constructor(e, t) {
-        this._root = null, this.focused = !1, this.trackWrites = null, this.mounted = !1, this.markCursor = null, this.cursorWrapper = null, this.lastSelectedViewDesc = void 0, this.input = new jo, this.prevDirectPlugins = [], this.pluginViews = [], this.requiresGeckoHackNode = !1, this.dragging = null, this._props = t, this.state = t.state, this.directPlugins = t.plugins || [], this.directPlugins.forEach(ec), this.dispatch = this.dispatch.bind(this), this.dom = e && e.mount || document.createElement("div"), e && (e.appendChild ? e.appendChild(this.dom) : typeof e == "function" ? e(this.dom) : e.mount && (this.mounted = !0)), this.editable = Xa(this), Qa(this), this.nodeViews = Za(this), this.docView = Da(this.state.doc, Ya(this), To(this), this.dom, this), this.domObserver = new Jo(this, (r, i, o, s) => Qp(this, r, i, o, s)), this.domObserver.start(), Tp(this), this.updatePluginViews()
+        this._root = null, this.focused = !1, this.trackWrites = null, this.mounted = !1, this.markCursor = null, this.cursorWrapper = null, this.lastSelectedViewDesc = void 0, this.input = new wi, this.prevDirectPlugins = [], this.pluginViews = [], this.requiresGeckoHackNode = !1, this.dragging = null, this._props = t, this.state = t.state, this.directPlugins = t.plugins || [], this.directPlugins.forEach(ul), this.dispatch = this.dispatch.bind(this), this.dom = e && e.mount || document.createElement("div"), e && (e.appendChild ? e.appendChild(this.dom) : typeof e == "function" ? e(this.dom) : e.mount && (this.mounted = !0)), this.editable = al(this), ll(this), this.nodeViews = cl(this), this.docView = Vo(this.state.doc, ol(this), ui(this), this.dom, this), this.domObserver = new vi(this, (r, i, s, o) => Md(this, r, i, s, o)), this.domObserver.start(), Qu(this), this.updatePluginViews()
     }
     get composing() {
         return this.input.composing
     }
     get props() {
         if (this._props.state != this.state) {
             let e = this._props;
             this._props = {};
             for (let t in e) this._props[t] = e[t];
             this._props.state = this.state
         }
         return this._props
     }
     update(e) {
-        e.handleDOMEvents != this._props.handleDOMEvents && Vo(this);
+        e.handleDOMEvents != this._props.handleDOMEvents && Ti(this);
         let t = this._props;
-        this._props = e, e.plugins && (e.plugins.forEach(ec), this.directPlugins = e.plugins), this.updateStateInner(e.state, t)
+        this._props = e, e.plugins && (e.plugins.forEach(ul), this.directPlugins = e.plugins), this.updateStateInner(e.state, t)
     }
     setProps(e) {
         let t = {};
         for (let r in this._props) t[r] = this._props[r];
         t.state = this.state;
         for (let r in e) t[r] = e[r];
         this.update(t)
     }
     updateState(e) {
         this.updateStateInner(e, this._props)
     }
     updateStateInner(e, t) {
         let r = this.state,
             i = !1,
-            o = !1;
-        e.storedMarks && this.composing && (Tc(this), o = !0), this.state = e;
-        let s = r.plugins != e.plugins || this._props.plugins != t.plugins;
-        if (s || this._props.plugins != t.plugins || this._props.nodeViews != t.nodeViews) {
-            let f = Za(this);
-            nh(f, this.nodeViews) && (this.nodeViews = f, i = !0)
-        }(s || t.handleDOMEvents != this._props.handleDOMEvents) && Vo(this), this.editable = Xa(this), Qa(this);
-        let l = To(this),
-            a = Ya(this),
+            s = !1;
+        e.storedMarks && this.composing && (Bl(this), s = !0), this.state = e;
+        let o = r.plugins != e.plugins || this._props.plugins != t.plugins;
+        if (o || this._props.plugins != t.plugins || this._props.nodeViews != t.nodeViews) {
+            let f = cl(this);
+            Cd(f, this.nodeViews) && (this.nodeViews = f, i = !0)
+        }(o || t.handleDOMEvents != this._props.handleDOMEvents) && Ti(this), this.editable = al(this), ll(this);
+        let l = ui(this),
+            a = ol(this),
             c = r.plugins != e.plugins && !r.doc.eq(e.doc) ? "reset" : e.scrollToSelection > r.scrollToSelection ? "to selection" : "preserve",
             u = i || !this.docView.matchesNode(e.doc, a, l);
-        (u || !e.selection.eq(r.selection)) && (o = !0);
-        let d = c == "preserve" && o && this.dom.style.overflowAnchor == null && Uf(this);
-        if (o) {
+        (u || !e.selection.eq(r.selection)) && (s = !0);
+        let d = c == "preserve" && s && this.dom.style.overflowAnchor == null && yu(this);
+        if (s) {
             this.domObserver.stop();
-            let f = u && (Ce || ye) && !this.composing && !r.selection.empty && !e.selection.empty && th(r.selection, e.selection);
+            let f = u && (fe || ie) && !this.composing && !r.selection.empty && !e.selection.empty && Td(r.selection, e.selection);
             if (u) {
-                let p = ye ? this.trackWrites = this.domSelectionRange().focusNode : null;
-                (i || !this.docView.update(e.doc, a, l, this)) && (this.docView.updateOuterDeco([]), this.docView.destroy(), this.docView = Da(e.doc, a, l, this.dom, this)), p && !this.trackWrites && (f = !0)
+                let h = ie ? this.trackWrites = this.domSelectionRange().focusNode : null;
+                (i || !this.docView.update(e.doc, a, l, this)) && (this.docView.updateOuterDeco([]), this.docView.destroy(), this.docView = Vo(e.doc, a, l, this.dom, this)), h && !this.trackWrites && (f = !0)
             }
-            f || !(this.input.mouseDown && this.domObserver.currentSelection.eq(this.domSelectionRange()) && mp(this)) ? bt(this, f) : (fc(this, e.selection), this.domObserver.setCurSelection()), this.domObserver.start()
+            f || !(this.input.mouseDown && this.domObserver.currentSelection.eq(this.domSelectionRange()) && Fu(this)) ? Je(this, f) : (Sl(this, e.selection), this.domObserver.setCurSelection()), this.domObserver.start()
         }
-        this.updatePluginViews(r), c == "reset" ? this.dom.scrollTop = 0 : c == "to selection" ? this.scrollToSelection() : d && _f(d)
+        this.updatePluginViews(r), c == "reset" ? this.dom.scrollTop = 0 : c == "to selection" ? this.scrollToSelection() : d && bu(d)
     }
     scrollToSelection() {
         let e = this.domSelectionRange().focusNode;
         if (!this.someProp("handleScrollToSelection", t => t(this)))
-            if (this.state.selection instanceof D) {
+            if (this.state.selection instanceof O) {
                 let t = this.docView.domAfterPos(this.state.selection.from);
-                t.nodeType == 1 && Ta(this, t.getBoundingClientRect(), e)
-            } else Ta(this, this.coordsAtPos(this.state.selection.head, 1), e)
+                t.nodeType == 1 && Bo(this, t.getBoundingClientRect(), e)
+            } else Bo(this, this.coordsAtPos(this.state.selection.head, 1), e)
     }
     destroyPluginViews() {
         let e;
         for (; e = this.pluginViews.pop();) e.destroy && e.destroy()
     }
     updatePluginViews(e) {
         if (!e || e.plugins != this.state.plugins || this.directPlugins != this.prevDirectPlugins) {
@@ -8434,151 +7204,151 @@
                 r.update && r.update(this, e)
             }
     }
     someProp(e, t) {
         let r = this._props && this._props[e],
             i;
         if (r != null && (i = t ? t(r) : r)) return i;
-        for (let s = 0; s < this.directPlugins.length; s++) {
-            let l = this.directPlugins[s].props[e];
+        for (let o = 0; o < this.directPlugins.length; o++) {
+            let l = this.directPlugins[o].props[e];
             if (l != null && (i = t ? t(l) : l)) return i
         }
-        let o = this.state.plugins;
-        if (o)
-            for (let s = 0; s < o.length; s++) {
-                let l = o[s].props[e];
+        let s = this.state.plugins;
+        if (s)
+            for (let o = 0; o < s.length; o++) {
+                let l = s[o].props[e];
                 if (l != null && (i = t ? t(l) : l)) return i
             }
     }
     hasFocus() {
-        if (Ce) {
+        if (fe) {
             let e = this.root.activeElement;
             if (e == this.dom) return !0;
             if (!e || !this.dom.contains(e)) return !1;
             for (; e && this.dom != e && this.dom.contains(e);) {
                 if (e.contentEditable == "false") return !1;
                 e = e.parentElement
             }
             return !0
         }
         return this.root.activeElement == this.dom
     }
     focus() {
-        this.domObserver.stop(), this.editable && Gf(this.dom), bt(this), this.domObserver.start()
+        this.domObserver.stop(), this.editable && xu(this.dom), Je(this), this.domObserver.start()
     }
     get root() {
         let e = this._root;
         if (e == null) {
             for (let t = this.dom.parentNode; t; t = t.parentNode)
                 if (t.nodeType == 9 || t.nodeType == 11 && t.host) return t.getSelection || (Object.getPrototypeOf(t).getSelection = () => t.ownerDocument.getSelection()), this._root = t
         }
         return e || document
     }
     posAtCoords(e) {
-        return ep(this, e)
+        return wu(this, e)
     }
     coordsAtPos(e, t = 1) {
-        return sc(this, e, t)
+        return gl(this, e, t)
     }
     domAtPos(e, t = 0) {
         return this.docView.domFromPos(e, t)
     }
     nodeDOM(e) {
         let t = this.docView.descAt(e);
         return t ? t.nodeDOM : null
     }
     posAtDOM(e, t, r = -1) {
         let i = this.docView.posFromDOM(e, t, r);
         if (i == null) throw new RangeError("DOM position not inside the editor");
         return i
     }
     endOfTextblock(e, t) {
-        return op(this, t || this.state, e)
+        return vu(this, t || this.state, e)
     }
     pasteHTML(e, t) {
-        return br(this, "", e, !1, t || new ClipboardEvent("paste"))
+        return Mn(this, "", e, !1, t || new ClipboardEvent("paste"))
     }
     pasteText(e, t) {
-        return br(this, e, null, !0, t || new ClipboardEvent("paste"))
+        return Mn(this, e, null, !0, t || new ClipboardEvent("paste"))
     }
     destroy() {
-        this.docView && (Cp(this), this.destroyPluginViews(), this.mounted ? (this.docView.update(this.state.doc, [], To(this), this), this.dom.textContent = "") : this.dom.parentNode && this.dom.parentNode.removeChild(this.dom), this.docView.destroy(), this.docView = null)
+        this.docView && (Yu(this), this.destroyPluginViews(), this.mounted ? (this.docView.update(this.state.doc, [], ui(this), this), this.dom.textContent = "") : this.dom.parentNode && this.dom.parentNode.removeChild(this.dom), this.docView.destroy(), this.docView = null)
     }
     get isDestroyed() {
         return this.docView == null
     }
     dispatchEvent(e) {
-        return Ap(this, e)
+        return Zu(this, e)
     }
     dispatch(e) {
         let t = this._props.dispatchTransaction;
         t ? t.call(this, e) : this.updateState(this.state.apply(e))
     }
     domSelectionRange() {
-        return ve && this.root.nodeType === 11 && jf(this.dom.ownerDocument) == this.dom ? Up(this) : this.domSelection()
+        return oe && this.root.nodeType === 11 && uu(this.dom.ownerDocument) == this.dom ? yd(this) : this.domSelection()
     }
     domSelection() {
         return this.root.getSelection()
     }
 };
 
-function Ya(n) {
+function ol(n) {
     let e = Object.create(null);
     return e.class = "ProseMirror", e.contenteditable = String(n.editable), n.someProp("attributes", t => {
         if (typeof t == "function" && (t = t(n.state)), t)
             for (let r in t) r == "class" ? e.class += " " + t[r] : r == "style" ? e.style = (e.style ? e.style + ";" : "") + t[r] : !e[r] && r != "contenteditable" && r != "nodeName" && (e[r] = String(t[r]))
-    }), e.translate || (e.translate = "no"), [ke.node(0, n.state.doc.content.size, e)]
+    }), e.translate || (e.translate = "no"), [se.node(0, n.state.doc.content.size, e)]
 }
 
-function Qa(n) {
+function ll(n) {
     if (n.markCursor) {
         let e = document.createElement("img");
         e.className = "ProseMirror-separator", e.setAttribute("mark-placeholder", "true"), e.setAttribute("alt", ""), n.cursorWrapper = {
             dom: e,
-            deco: ke.widget(n.state.selection.head, e, {
+            deco: se.widget(n.state.selection.head, e, {
                 raw: !0,
                 marks: n.markCursor
             })
         }
     } else n.cursorWrapper = null
 }
 
-function Xa(n) {
+function al(n) {
     return !n.someProp("editable", e => e(n.state) === !1)
 }
 
-function th(n, e) {
+function Td(n, e) {
     let t = Math.min(n.$anchor.sharedDepth(n.head), e.$anchor.sharedDepth(e.head));
     return n.$anchor.start(t) != e.$anchor.start(t)
 }
 
-function Za(n) {
+function cl(n) {
     let e = Object.create(null);
 
     function t(r) {
         for (let i in r) Object.prototype.hasOwnProperty.call(e, i) || (e[i] = r[i])
     }
     return n.someProp("nodeViews", t), n.someProp("markViews", t), e
 }
 
-function nh(n, e) {
+function Cd(n, e) {
     let t = 0,
         r = 0;
     for (let i in n) {
         if (n[i] != e[i]) return !0;
         t++
     }
     for (let i in e) r++;
     return t != r
 }
 
-function ec(n) {
+function ul(n) {
     if (n.spec.state || n.spec.filterTransaction || n.spec.appendTransaction) throw new RangeError("Plugins passed directly to the view must not have a state component")
 }
-var vt = {
+var qe = {
         8: "Backspace",
         9: "Tab",
         10: "Enter",
         12: "NumLock",
         13: "Enter",
         16: "Shift",
         17: "Control",
@@ -8624,15 +7394,15 @@
         191: "/",
         192: "`",
         219: "[",
         220: "\\",
         221: "]",
         222: "'"
     },
-    si = {
+    lr = {
         48: ")",
         49: "!",
         50: "@",
         51: "#",
         52: "$",
         53: "%",
         54: "^",
@@ -8650,614 +7420,614 @@
         191: "?",
         192: "~",
         219: "{",
         220: "|",
         221: "}",
         222: '"'
     },
-    Ic = typeof navigator < "u" && /Chrome\/(\d+)/.exec(navigator.userAgent),
-    Zb = typeof navigator < "u" && /Gecko\/\d+/.test(navigator.userAgent),
-    rh = typeof navigator < "u" && /Mac/.test(navigator.platform),
-    ih = typeof navigator < "u" && /MSIE \d|Trident\/(?:[7-9]|\d{2,})\..*rv:(\d+)/.exec(navigator.userAgent),
-    oh = rh || Ic && +Ic[1] < 57;
-for (re = 0; re < 10; re++) vt[48 + re] = vt[96 + re] = String(re);
-var re;
-for (re = 1; re <= 24; re++) vt[re + 111] = "F" + re;
-var re;
-for (re = 65; re <= 90; re++) vt[re] = String.fromCharCode(re + 32), si[re] = String.fromCharCode(re);
-var re;
-for (oi in vt) si.hasOwnProperty(oi) || (si[oi] = vt[oi]);
-var oi;
-
-function Dc(n) {
-    var e = oh && (n.ctrlKey || n.altKey || n.metaKey) || ih && n.shiftKey && n.key && n.key.length == 1 || n.key == "Unidentified",
-        t = !e && n.key || (n.shiftKey ? si : vt)[n.keyCode] || n.key || "Unidentified";
+    $l = typeof navigator < "u" && /Chrome\/(\d+)/.exec(navigator.userAgent),
+    Ip = typeof navigator < "u" && /Gecko\/\d+/.test(navigator.userAgent),
+    Ad = typeof navigator < "u" && /Mac/.test(navigator.platform),
+    Od = typeof navigator < "u" && /MSIE \d|Trident\/(?:[7-9]|\d{2,})\..*rv:(\d+)/.exec(navigator.userAgent),
+    vd = Ad || $l && +$l[1] < 57;
+for (G = 0; G < 10; G++) qe[48 + G] = qe[96 + G] = String(G);
+var G;
+for (G = 1; G <= 24; G++) qe[G + 111] = "F" + G;
+var G;
+for (G = 65; G <= 90; G++) qe[G] = String.fromCharCode(G + 32), lr[G] = String.fromCharCode(G);
+var G;
+for (or in qe) lr.hasOwnProperty(or) || (lr[or] = qe[or]);
+var or;
+
+function Vl(n) {
+    var e = vd && (n.ctrlKey || n.altKey || n.metaKey) || Od && n.shiftKey && n.key && n.key.length == 1 || n.key == "Unidentified",
+        t = !e && n.key || (n.shiftKey ? lr : qe)[n.keyCode] || n.key || "Unidentified";
     return t == "Esc" && (t = "Escape"), t == "Del" && (t = "Delete"), t == "Left" && (t = "ArrowLeft"), t == "Up" && (t = "ArrowUp"), t == "Right" && (t = "ArrowRight"), t == "Down" && (t = "ArrowDown"), t
 }
-var sh = typeof navigator < "u" ? /Mac|iP(hone|[oa]d)/.test(navigator.platform) : !1;
+var Nd = typeof navigator < "u" ? /Mac|iP(hone|[oa]d)/.test(navigator.platform) : !1;
 
-function lh(n) {
+function Id(n) {
     let e = n.split(/-(?!$)/),
         t = e[e.length - 1];
     t == "Space" && (t = " ");
-    let r, i, o, s;
+    let r, i, s, o;
     for (let l = 0; l < e.length - 1; l++) {
         let a = e[l];
-        if (/^(cmd|meta|m)$/i.test(a)) s = !0;
+        if (/^(cmd|meta|m)$/i.test(a)) o = !0;
         else if (/^a(lt)?$/i.test(a)) r = !0;
         else if (/^(c|ctrl|control)$/i.test(a)) i = !0;
-        else if (/^s(hift)?$/i.test(a)) o = !0;
-        else if (/^mod$/i.test(a)) sh ? s = !0 : i = !0;
+        else if (/^s(hift)?$/i.test(a)) s = !0;
+        else if (/^mod$/i.test(a)) Nd ? o = !0 : i = !0;
         else throw new Error("Unrecognized modifier name: " + a)
     }
-    return r && (t = "Alt-" + t), i && (t = "Ctrl-" + t), s && (t = "Meta-" + t), o && (t = "Shift-" + t), t
+    return r && (t = "Alt-" + t), i && (t = "Ctrl-" + t), o && (t = "Meta-" + t), s && (t = "Shift-" + t), t
 }
 
-function ah(n) {
+function Dd(n) {
     let e = Object.create(null);
-    for (let t in n) e[lh(t)] = n[t];
+    for (let t in n) e[Id(t)] = n[t];
     return e
 }
 
-function Zo(n, e, t = !0) {
+function zi(n, e, t = !0) {
     return e.altKey && (n = "Alt-" + n), e.ctrlKey && (n = "Ctrl-" + n), e.metaKey && (n = "Meta-" + n), t && e.shiftKey && (n = "Shift-" + n), n
 }
 
-function Lc(n) {
-    return new q({
+function Jl(n) {
+    return new $({
         props: {
-            handleKeyDown: ch(n)
+            handleKeyDown: Ld(n)
         }
     })
 }
 
-function ch(n) {
-    let e = ah(n);
+function Ld(n) {
+    let e = Dd(n);
     return function(t, r) {
-        let i = Dc(r),
-            o, s = e[Zo(i, r)];
-        if (s && s(t.state, t.dispatch, t)) return !0;
+        let i = Vl(r),
+            s, o = e[zi(i, r)];
+        if (o && o(t.state, t.dispatch, t)) return !0;
         if (i.length == 1 && i != " ") {
             if (r.shiftKey) {
-                let l = e[Zo(i, r, !1)];
+                let l = e[zi(i, r, !1)];
                 if (l && l(t.state, t.dispatch, t)) return !0
             }
-            if ((r.shiftKey || r.altKey || r.metaKey || i.charCodeAt(0) > 127) && (o = vt[r.keyCode]) && o != i) {
-                let l = e[Zo(o, r)];
+            if ((r.shiftKey || r.altKey || r.metaKey || i.charCodeAt(0) > 127) && (s = qe[r.keyCode]) && s != i) {
+                let l = e[zi(s, r)];
                 if (l && l(t.state, t.dispatch, t)) return !0
             }
         }
         return !1
     }
 }
-var li = (n, e) => n.selection.empty ? !1 : (e && e(n.tr.deleteSelection().scrollIntoView()), !0);
+var ar = (n, e) => n.selection.empty ? !1 : (e && e(n.tr.deleteSelection().scrollIntoView()), !0);
 
-function uh(n, e) {
+function Rd(n, e) {
     let {
         $cursor: t
     } = n.selection;
     return !t || (e ? !e.endOfTextblock("backward", n) : t.parentOffset > 0) ? null : t
 }
-var ts = (n, e, t) => {
-    let r = uh(n, t);
+var Fi = (n, e, t) => {
+    let r = Rd(n, t);
     if (!r) return !1;
-    let i = Rc(r);
+    let i = ql(r);
     if (!i) {
-        let s = r.blockRange(),
-            l = s && gt(s);
-        return l == null ? !1 : (e && e(n.tr.lift(s, l).scrollIntoView()), !0)
-    }
-    let o = i.nodeBefore;
-    if (!o.type.spec.isolating && Vc(n, i, e)) return !0;
-    if (r.parent.content.size == 0 && (Vn(o, "end") || D.isSelectable(o))) {
-        let s = _r(n.doc, r.before(), r.after(), w.empty);
-        if (s && s.slice.size < s.to - s.from) {
+        let o = r.blockRange(),
+            l = o && je(o);
+        return l == null ? !1 : (e && e(n.tr.lift(o, l).scrollIntoView()), !0)
+    }
+    let s = i.nodeBefore;
+    if (!s.type.spec.isolating && Yl(n, i, e)) return !0;
+    if (r.parent.content.size == 0 && (_t(s, "end") || O.isSelectable(s))) {
+        let o = Gn(n.doc, r.before(), r.after(), E.empty);
+        if (o && o.slice.size < o.to - o.from) {
             if (e) {
-                let l = n.tr.step(s);
-                l.setSelection(Vn(o, "end") ? R.findFrom(l.doc.resolve(l.mapping.map(i.pos, -1)), -1) : D.create(l.doc, i.pos - o.nodeSize)), e(l.scrollIntoView())
+                let l = n.tr.step(o);
+                l.setSelection(_t(s, "end") ? L.findFrom(l.doc.resolve(l.mapping.map(i.pos, -1)), -1) : O.create(l.doc, i.pos - s.nodeSize)), e(l.scrollIntoView())
             }
             return !0
         }
     }
-    return o.isAtom && i.depth == r.depth - 1 ? (e && e(n.tr.delete(i.pos - o.nodeSize, i.pos).scrollIntoView()), !0) : !1
+    return s.isAtom && i.depth == r.depth - 1 ? (e && e(n.tr.delete(i.pos - s.nodeSize, i.pos).scrollIntoView()), !0) : !1
 };
 
-function Vn(n, e, t = !1) {
+function _t(n, e, t = !1) {
     for (let r = n; r; r = e == "start" ? r.firstChild : r.lastChild) {
         if (r.isTextblock) return !0;
         if (t && r.childCount != 1) return !1
     }
     return !1
 }
-var ns = (n, e, t) => {
+var ji = (n, e, t) => {
     let {
         $head: r,
         empty: i
-    } = n.selection, o = r;
+    } = n.selection, s = r;
     if (!i) return !1;
     if (r.parent.isTextblock) {
         if (t ? !t.endOfTextblock("backward", n) : r.parentOffset > 0) return !1;
-        o = Rc(r)
+        s = ql(r)
     }
-    let s = o && o.nodeBefore;
-    return !s || !D.isSelectable(s) ? !1 : (e && e(n.tr.setSelection(D.create(n.doc, o.pos - s.nodeSize)).scrollIntoView()), !0)
+    let o = s && s.nodeBefore;
+    return !o || !O.isSelectable(o) ? !1 : (e && e(n.tr.setSelection(O.create(n.doc, s.pos - o.nodeSize)).scrollIntoView()), !0)
 };
 
-function Rc(n) {
+function ql(n) {
     if (!n.parent.type.spec.isolating)
         for (let e = n.depth - 1; e >= 0; e--) {
             if (n.index(e) > 0) return n.doc.resolve(n.before(e + 1));
             if (n.node(e).type.spec.isolating) break
         }
     return null
 }
 
-function dh(n, e) {
+function Pd(n, e) {
     let {
         $cursor: t
     } = n.selection;
     return !t || (e ? !e.endOfTextblock("forward", n) : t.parentOffset < t.parent.content.size) ? null : t
 }
-var rs = (n, e, t) => {
-        let r = dh(n, t);
+var $i = (n, e, t) => {
+        let r = Pd(n, t);
         if (!r) return !1;
-        let i = Bc(r);
+        let i = Kl(r);
         if (!i) return !1;
-        let o = i.nodeAfter;
-        if (Vc(n, i, e)) return !0;
-        if (r.parent.content.size == 0 && (Vn(o, "start") || D.isSelectable(o))) {
-            let s = _r(n.doc, r.before(), r.after(), w.empty);
-            if (s && s.slice.size < s.to - s.from) {
+        let s = i.nodeAfter;
+        if (Yl(n, i, e)) return !0;
+        if (r.parent.content.size == 0 && (_t(s, "start") || O.isSelectable(s))) {
+            let o = Gn(n.doc, r.before(), r.after(), E.empty);
+            if (o && o.slice.size < o.to - o.from) {
                 if (e) {
-                    let l = n.tr.step(s);
-                    l.setSelection(Vn(o, "start") ? R.findFrom(l.doc.resolve(l.mapping.map(i.pos)), 1) : D.create(l.doc, l.mapping.map(i.pos))), e(l.scrollIntoView())
+                    let l = n.tr.step(o);
+                    l.setSelection(_t(s, "start") ? L.findFrom(l.doc.resolve(l.mapping.map(i.pos)), 1) : O.create(l.doc, l.mapping.map(i.pos))), e(l.scrollIntoView())
                 }
                 return !0
             }
         }
-        return o.isAtom && i.depth == r.depth - 1 ? (e && e(n.tr.delete(i.pos, i.pos + o.nodeSize).scrollIntoView()), !0) : !1
+        return s.isAtom && i.depth == r.depth - 1 ? (e && e(n.tr.delete(i.pos, i.pos + s.nodeSize).scrollIntoView()), !0) : !1
     },
-    is = (n, e, t) => {
+    Vi = (n, e, t) => {
         let {
             $head: r,
             empty: i
-        } = n.selection, o = r;
+        } = n.selection, s = r;
         if (!i) return !1;
         if (r.parent.isTextblock) {
             if (t ? !t.endOfTextblock("forward", n) : r.parentOffset < r.parent.content.size) return !1;
-            o = Bc(r)
+            s = Kl(r)
         }
-        let s = o && o.nodeAfter;
-        return !s || !D.isSelectable(s) ? !1 : (e && e(n.tr.setSelection(D.create(n.doc, o.pos)).scrollIntoView()), !0)
+        let o = s && s.nodeAfter;
+        return !o || !O.isSelectable(o) ? !1 : (e && e(n.tr.setSelection(O.create(n.doc, s.pos)).scrollIntoView()), !0)
     };
 
-function Bc(n) {
+function Kl(n) {
     if (!n.parent.type.spec.isolating)
         for (let e = n.depth - 1; e >= 0; e--) {
             let t = n.node(e);
             if (n.index(e) + 1 < t.childCount) return n.doc.resolve(n.after(e + 1));
             if (t.type.spec.isolating) break
         }
     return null
 }
-var zc = (n, e) => {
+var Ul = (n, e) => {
         let t = n.selection,
-            r = t instanceof D,
+            r = t instanceof O,
             i;
         if (r) {
-            if (t.node.isTextblock || !Ke(n.doc, t.from)) return !1;
+            if (t.node.isTextblock || !Se(n.doc, t.from)) return !1;
             i = t.from
-        } else if (i = bo(n.doc, t.from, -1), i == null) return !1;
+        } else if (i = ri(n.doc, t.from, -1), i == null) return !1;
         if (e) {
-            let o = n.tr.join(i);
-            r && o.setSelection(D.create(o.doc, i - n.doc.resolve(i).nodeBefore.nodeSize)), e(o.scrollIntoView())
+            let s = n.tr.join(i);
+            r && s.setSelection(O.create(s.doc, i - n.doc.resolve(i).nodeBefore.nodeSize)), e(s.scrollIntoView())
         }
         return !0
     },
-    Hc = (n, e) => {
+    _l = (n, e) => {
         let t = n.selection,
             r;
-        if (t instanceof D) {
-            if (t.node.isTextblock || !Ke(n.doc, t.to)) return !1;
+        if (t instanceof O) {
+            if (t.node.isTextblock || !Se(n.doc, t.to)) return !1;
             r = t.to
-        } else if (r = bo(n.doc, t.to, 1), r == null) return !1;
+        } else if (r = ri(n.doc, t.to, 1), r == null) return !1;
         return e && e(n.tr.join(r).scrollIntoView()), !0
     },
-    Fc = (n, e) => {
+    Gl = (n, e) => {
         let {
             $from: t,
             $to: r
-        } = n.selection, i = t.blockRange(r), o = i && gt(i);
-        return o == null ? !1 : (e && e(n.tr.lift(i, o).scrollIntoView()), !0)
+        } = n.selection, i = t.blockRange(r), s = i && je(i);
+        return s == null ? !1 : (e && e(n.tr.lift(i, s).scrollIntoView()), !0)
     },
-    ss = (n, e) => {
+    Ji = (n, e) => {
         let {
             $head: t,
             $anchor: r
         } = n.selection;
         return !t.parent.type.spec.code || !t.sameParent(r) ? !1 : (e && e(n.tr.insertText(`
 `).scrollIntoView()), !0)
     };
 
-function ls(n) {
+function Wi(n) {
     for (let e = 0; e < n.edgeCount; e++) {
         let {
             type: t
         } = n.edge(e);
         if (t.isTextblock && !t.hasRequiredAttrs()) return t
     }
     return null
 }
-var as = (n, e) => {
+var qi = (n, e) => {
         let {
             $head: t,
             $anchor: r
         } = n.selection;
         if (!t.parent.type.spec.code || !t.sameParent(r)) return !1;
         let i = t.node(-1),
-            o = t.indexAfter(-1),
-            s = ls(i.contentMatchAt(o));
-        if (!s || !i.canReplaceWith(o, o, s)) return !1;
+            s = t.indexAfter(-1),
+            o = Wi(i.contentMatchAt(s));
+        if (!o || !i.canReplaceWith(s, s, o)) return !1;
         if (e) {
             let l = t.after(),
-                a = n.tr.replaceWith(l, l, s.createAndFill());
-            a.setSelection(R.near(a.doc.resolve(l), 1)), e(a.scrollIntoView())
+                a = n.tr.replaceWith(l, l, o.createAndFill());
+            a.setSelection(L.near(a.doc.resolve(l), 1)), e(a.scrollIntoView())
         }
         return !0
     },
-    cs = (n, e) => {
+    Ki = (n, e) => {
         let t = n.selection,
             {
                 $from: r,
                 $to: i
             } = t;
-        if (t instanceof fe || r.parent.inlineContent || i.parent.inlineContent) return !1;
-        let o = ls(i.parent.contentMatchAt(i.indexAfter()));
-        if (!o || !o.isTextblock) return !1;
+        if (t instanceof Z || r.parent.inlineContent || i.parent.inlineContent) return !1;
+        let s = Wi(i.parent.contentMatchAt(i.indexAfter()));
+        if (!s || !s.isTextblock) return !1;
         if (e) {
-            let s = (!r.parentOffset && i.index() < i.parent.childCount ? r : i).pos,
-                l = n.tr.insert(s, o.createAndFill());
-            l.setSelection(P.create(l.doc, s + 1)), e(l.scrollIntoView())
+            let o = (!r.parentOffset && i.index() < i.parent.childCount ? r : i).pos,
+                l = n.tr.insert(o, s.createAndFill());
+            l.setSelection(I.create(l.doc, o + 1)), e(l.scrollIntoView())
         }
         return !0
     },
-    us = (n, e) => {
+    Ui = (n, e) => {
         let {
             $cursor: t
         } = n.selection;
         if (!t || t.parent.content.size) return !1;
         if (t.depth > 1 && t.after() != t.end(-1)) {
-            let o = t.before();
-            if (ze(n.doc, o)) return e && e(n.tr.split(o).scrollIntoView()), !0
+            let s = t.before();
+            if (ge(n.doc, s)) return e && e(n.tr.split(s).scrollIntoView()), !0
         }
         let r = t.blockRange(),
-            i = r && gt(r);
+            i = r && je(r);
         return i == null ? !1 : (e && e(n.tr.lift(r, i).scrollIntoView()), !0)
     };
 
-function fh(n) {
+function Bd(n) {
     return (e, t) => {
         let {
             $from: r,
             $to: i
         } = e.selection;
-        if (e.selection instanceof D && e.selection.node.isBlock) return !r.parentOffset || !ze(e.doc, r.pos) ? !1 : (t && t(e.tr.split(r.pos).scrollIntoView()), !0);
+        if (e.selection instanceof O && e.selection.node.isBlock) return !r.parentOffset || !ge(e.doc, r.pos) ? !1 : (t && t(e.tr.split(r.pos).scrollIntoView()), !0);
         if (!r.parent.isBlock) return !1;
         if (t) {
-            let o = i.parentOffset == i.parent.content.size,
-                s = e.tr;
-            (e.selection instanceof P || e.selection instanceof fe) && s.deleteSelection();
-            let l = r.depth == 0 ? null : ls(r.node(-1).contentMatchAt(r.indexAfter(-1))),
-                a = n && n(i.parent, o),
-                c = a ? [a] : o && l ? [{
+            let s = i.parentOffset == i.parent.content.size,
+                o = e.tr;
+            (e.selection instanceof I || e.selection instanceof Z) && o.deleteSelection();
+            let l = r.depth == 0 ? null : Wi(r.node(-1).contentMatchAt(r.indexAfter(-1))),
+                a = n && n(i.parent, s),
+                c = a ? [a] : s && l ? [{
                     type: l
                 }] : void 0,
-                u = ze(s.doc, s.mapping.map(r.pos), 1, c);
-            if (!c && !u && ze(s.doc, s.mapping.map(r.pos), 1, l ? [{
+                u = ge(o.doc, o.mapping.map(r.pos), 1, c);
+            if (!c && !u && ge(o.doc, o.mapping.map(r.pos), 1, l ? [{
                     type: l
                 }] : void 0) && (l && (c = [{
                     type: l
-                }]), u = !0), u && (s.split(s.mapping.map(r.pos), 1, c), !o && !r.parentOffset && r.parent.type != l)) {
-                let d = s.mapping.map(r.before()),
-                    f = s.doc.resolve(d);
-                l && r.node(-1).canReplaceWith(f.index(), f.index() + 1, l) && s.setNodeMarkup(s.mapping.map(r.before()), l)
+                }]), u = !0), u && (o.split(o.mapping.map(r.pos), 1, c), !s && !r.parentOffset && r.parent.type != l)) {
+                let d = o.mapping.map(r.before()),
+                    f = o.doc.resolve(d);
+                l && r.node(-1).canReplaceWith(f.index(), f.index() + 1, l) && o.setNodeMarkup(o.mapping.map(r.before()), l)
             }
-            t(s.scrollIntoView())
+            t(o.scrollIntoView())
         }
         return !0
     }
 }
-var ph = fh();
-var jc = (n, e) => {
+var zd = Bd();
+var Ql = (n, e) => {
         let {
             $from: t,
             to: r
-        } = n.selection, i, o = t.sharedDepth(r);
-        return o == 0 ? !1 : (i = t.before(o), e && e(n.tr.setSelection(D.create(n.doc, i))), !0)
+        } = n.selection, i, s = t.sharedDepth(r);
+        return s == 0 ? !1 : (i = t.before(s), e && e(n.tr.setSelection(O.create(n.doc, i))), !0)
     },
-    hh = (n, e) => (e && e(n.tr.setSelection(new fe(n.doc))), !0);
+    Hd = (n, e) => (e && e(n.tr.setSelection(new Z(n.doc))), !0);
 
-function mh(n, e, t) {
+function Fd(n, e, t) {
     let r = e.nodeBefore,
         i = e.nodeAfter,
-        o = e.index();
-    return !r || !i || !r.type.compatibleContent(i.type) ? !1 : !r.content.size && e.parent.canReplace(o - 1, o) ? (t && t(n.tr.delete(e.pos - r.nodeSize, e.pos).scrollIntoView()), !0) : !e.parent.canReplace(o, o + 1) || !(i.isTextblock || Ke(n.doc, e.pos)) ? !1 : (t && t(n.tr.clearIncompatible(e.pos, r.type, r.contentMatchAt(r.childCount)).join(e.pos).scrollIntoView()), !0)
+        s = e.index();
+    return !r || !i || !r.type.compatibleContent(i.type) ? !1 : !r.content.size && e.parent.canReplace(s - 1, s) ? (t && t(n.tr.delete(e.pos - r.nodeSize, e.pos).scrollIntoView()), !0) : !e.parent.canReplace(s, s + 1) || !(i.isTextblock || Se(n.doc, e.pos)) ? !1 : (t && t(n.tr.clearIncompatible(e.pos, r.type, r.contentMatchAt(r.childCount)).join(e.pos).scrollIntoView()), !0)
 }
 
-function Vc(n, e, t) {
+function Yl(n, e, t) {
     let r = e.nodeBefore,
         i = e.nodeAfter,
-        o, s;
+        s, o;
     if (r.type.spec.isolating || i.type.spec.isolating) return !1;
-    if (mh(n, e, t)) return !0;
+    if (Fd(n, e, t)) return !0;
     let l = e.parent.canReplace(e.index(), e.index() + 1);
-    if (l && (o = (s = r.contentMatchAt(r.childCount)).findWrapping(i.type)) && s.matchType(o[0] || i.type).validEnd) {
+    if (l && (s = (o = r.contentMatchAt(r.childCount)).findWrapping(i.type)) && o.matchType(s[0] || i.type).validEnd) {
         if (t) {
             let d = e.pos + i.nodeSize,
-                f = v.empty;
-            for (let m = o.length - 1; m >= 0; m--) f = v.from(o[m].create(null, f));
-            f = v.from(r.copy(f));
-            let p = n.tr.step(new W(e.pos - 1, d, e.pos, d, new w(f, 1, 0), o.length, !0)),
-                h = d + 2 * o.length;
-            Ke(p.doc, h) && p.join(h), t(p.scrollIntoView())
+                f = x.empty;
+            for (let m = s.length - 1; m >= 0; m--) f = x.from(s[m].create(null, f));
+            f = x.from(r.copy(f));
+            let h = n.tr.step(new j(e.pos - 1, d, e.pos, d, new E(f, 1, 0), s.length, !0)),
+                p = d + 2 * s.length;
+            Se(h.doc, p) && h.join(p), t(h.scrollIntoView())
         }
         return !0
     }
-    let a = R.findFrom(e, 1),
+    let a = L.findFrom(e, 1),
         c = a && a.$from.blockRange(a.$to),
-        u = c && gt(c);
+        u = c && je(c);
     if (u != null && u >= e.depth) return t && t(n.tr.lift(c, u).scrollIntoView()), !0;
-    if (l && Vn(i, "start", !0) && Vn(r, "end")) {
+    if (l && _t(i, "start", !0) && _t(r, "end")) {
         let d = r,
             f = [];
         for (; f.push(d), !d.isTextblock;) d = d.lastChild;
-        let p = i,
-            h = 1;
-        for (; !p.isTextblock; p = p.firstChild) h++;
-        if (d.canReplace(d.childCount, d.childCount, p.content)) {
+        let h = i,
+            p = 1;
+        for (; !h.isTextblock; h = h.firstChild) p++;
+        if (d.canReplace(d.childCount, d.childCount, h.content)) {
             if (t) {
-                let m = v.empty;
-                for (let k = f.length - 1; k >= 0; k--) m = v.from(f[k].copy(m));
-                let b = n.tr.step(new W(e.pos - f.length, e.pos + i.nodeSize, e.pos + h, e.pos + i.nodeSize - h, new w(m, f.length, 0), 0, !0));
+                let m = x.empty;
+                for (let M = f.length - 1; M >= 0; M--) m = x.from(f[M].copy(m));
+                let b = n.tr.step(new j(e.pos - f.length, e.pos + i.nodeSize, e.pos + p, e.pos + i.nodeSize - p, new E(m, f.length, 0), 0, !0));
                 t(b.scrollIntoView())
             }
             return !0
         }
     }
     return !1
 }
 
-function $c(n) {
+function Xl(n) {
     return function(e, t) {
         let r = e.selection,
             i = n < 0 ? r.$from : r.$to,
-            o = i.depth;
-        for (; i.node(o).isInline;) {
-            if (!o) return !1;
-            o--
+            s = i.depth;
+        for (; i.node(s).isInline;) {
+            if (!s) return !1;
+            s--
         }
-        return i.node(o).isTextblock ? (t && t(e.tr.setSelection(P.create(e.doc, n < 0 ? i.start(o) : i.end(o)))), !0) : !1
+        return i.node(s).isTextblock ? (t && t(e.tr.setSelection(I.create(e.doc, n < 0 ? i.start(s) : i.end(s)))), !0) : !1
     }
 }
-var ds = $c(-1),
-    fs = $c(1);
+var _i = Xl(-1),
+    Gi = Xl(1);
 
-function Wc(n, e = null) {
+function Zl(n, e = null) {
     return function(t, r) {
         let {
             $from: i,
-            $to: o
-        } = t.selection, s = i.blockRange(o), l = s && Dn(s, n, e);
-        return l ? (r && r(t.tr.wrap(s, l).scrollIntoView()), !0) : !1
+            $to: s
+        } = t.selection, o = i.blockRange(s), l = o && Ft(o, n, e);
+        return l ? (r && r(t.tr.wrap(o, l).scrollIntoView()), !0) : !1
     }
 }
 
-function ps(n, e = null) {
+function Qi(n, e = null) {
     return function(t, r) {
         let i = !1;
-        for (let o = 0; o < t.selection.ranges.length && !i; o++) {
+        for (let s = 0; s < t.selection.ranges.length && !i; s++) {
             let {
                 $from: {
-                    pos: s
+                    pos: o
                 },
                 $to: {
                     pos: l
                 }
-            } = t.selection.ranges[o];
-            t.doc.nodesBetween(s, l, (a, c) => {
+            } = t.selection.ranges[s];
+            t.doc.nodesBetween(o, l, (a, c) => {
                 if (i) return !1;
                 if (!(!a.isTextblock || a.hasMarkup(n, e)))
                     if (a.type == n) i = !0;
                     else {
                         let u = t.doc.resolve(c),
                             d = u.index();
                         i = u.parent.canReplaceWith(d, d + 1, n)
                     }
             })
         }
         if (!i) return !1;
         if (r) {
-            let o = t.tr;
-            for (let s = 0; s < t.selection.ranges.length; s++) {
+            let s = t.tr;
+            for (let o = 0; o < t.selection.ranges.length; o++) {
                 let {
                     $from: {
                         pos: l
                     },
                     $to: {
                         pos: a
                     }
-                } = t.selection.ranges[s];
-                o.setBlockType(l, a, n, e)
+                } = t.selection.ranges[o];
+                s.setBlockType(l, a, n, e)
             }
-            r(o.scrollIntoView())
+            r(s.scrollIntoView())
         }
         return !0
     }
 }
 
-function hs(...n) {
+function Yi(...n) {
     return function(e, t, r) {
         for (let i = 0; i < n.length; i++)
             if (n[i](e, t, r)) return !0;
         return !1
     }
 }
-var es = hs(li, ts, ns),
-    Pc = hs(li, rs, is),
-    Rt = {
-        Enter: hs(ss, cs, us, ph),
-        "Mod-Enter": as,
-        Backspace: es,
-        "Mod-Backspace": es,
-        "Shift-Backspace": es,
-        Delete: Pc,
-        "Mod-Delete": Pc,
-        "Mod-a": hh
-    },
-    gh = {
-        "Ctrl-h": Rt.Backspace,
-        "Alt-Backspace": Rt["Mod-Backspace"],
-        "Ctrl-d": Rt.Delete,
-        "Ctrl-Alt-Backspace": Rt["Mod-Delete"],
-        "Alt-Delete": Rt["Mod-Delete"],
-        "Alt-d": Rt["Mod-Delete"],
-        "Ctrl-a": ds,
-        "Ctrl-e": fs
+var Hi = Yi(ar, Fi, ji),
+    Wl = Yi(ar, $i, Vi),
+    tt = {
+        Enter: Yi(Ji, Ki, Ui, zd),
+        "Mod-Enter": qi,
+        Backspace: Hi,
+        "Mod-Backspace": Hi,
+        "Shift-Backspace": Hi,
+        Delete: Wl,
+        "Mod-Delete": Wl,
+        "Mod-a": Hd
+    },
+    jd = {
+        "Ctrl-h": tt.Backspace,
+        "Alt-Backspace": tt["Mod-Backspace"],
+        "Ctrl-d": tt.Delete,
+        "Ctrl-Alt-Backspace": tt["Mod-Delete"],
+        "Alt-Delete": tt["Mod-Delete"],
+        "Alt-d": tt["Mod-Delete"],
+        "Ctrl-a": _i,
+        "Ctrl-e": Gi
     };
-for (let n in Rt) gh[n] = Rt[n];
-var pk = typeof navigator < "u" ? /Mac|iP(hone|[oa]d)/.test(navigator.platform) : typeof os < "u" && os.platform ? os.platform() == "darwin" : !1;
+for (let n in tt) jd[n] = tt[n];
+var qp = typeof navigator < "u" ? /Mac|iP(hone|[oa]d)/.test(navigator.platform) : typeof os < "u" && os.platform ? os.platform() == "darwin" : !1;
 
-function qc(n, e = null) {
+function ea(n, e = null) {
     return function(t, r) {
         let {
             $from: i,
-            $to: o
-        } = t.selection, s = i.blockRange(o), l = !1, a = s;
-        if (!s) return !1;
-        if (s.depth >= 2 && i.node(s.depth - 1).type.compatibleContent(n) && s.startIndex == 0) {
-            if (i.index(s.depth - 1) == 0) return !1;
-            let u = t.doc.resolve(s.start - 2);
-            a = new on(u, u, s.depth), s.endIndex < s.parent.childCount && (s = new on(i, t.doc.resolve(o.end(s.depth)), s.depth)), l = !0
-        }
-        let c = Dn(a, n, e, s);
-        return c ? (r && r(yh(t.tr, s, c, l, n).scrollIntoView()), !0) : !1
+            $to: s
+        } = t.selection, o = i.blockRange(s), l = !1, a = o;
+        if (!o) return !1;
+        if (o.depth >= 2 && i.node(o.depth - 1).type.compatibleContent(n) && o.startIndex == 0) {
+            if (i.index(o.depth - 1) == 0) return !1;
+            let u = t.doc.resolve(o.start - 2);
+            a = new yt(u, u, o.depth), o.endIndex < o.parent.childCount && (o = new yt(i, t.doc.resolve(s.end(o.depth)), o.depth)), l = !0
+        }
+        let c = Ft(a, n, e, o);
+        return c ? (r && r($d(t.tr, o, c, l, n).scrollIntoView()), !0) : !1
     }
 }
 
-function yh(n, e, t, r, i) {
-    let o = v.empty;
-    for (let u = t.length - 1; u >= 0; u--) o = v.from(t[u].type.create(t[u].attrs, o));
-    n.step(new W(e.start - (r ? 2 : 0), e.end, e.start, e.end, new w(o, 0, 0), t.length, !0));
-    let s = 0;
-    for (let u = 0; u < t.length; u++) t[u].type == i && (s = u + 1);
-    let l = t.length - s,
+function $d(n, e, t, r, i) {
+    let s = x.empty;
+    for (let u = t.length - 1; u >= 0; u--) s = x.from(t[u].type.create(t[u].attrs, s));
+    n.step(new j(e.start - (r ? 2 : 0), e.end, e.start, e.end, new E(s, 0, 0), t.length, !0));
+    let o = 0;
+    for (let u = 0; u < t.length; u++) t[u].type == i && (o = u + 1);
+    let l = t.length - o,
         a = e.start + t.length - (r ? 2 : 0),
         c = e.parent;
-    for (let u = e.startIndex, d = e.endIndex, f = !0; u < d; u++, f = !1) !f && ze(n.doc, a, l) && (n.split(a, l), a += 2 * l), a += c.child(u).nodeSize;
+    for (let u = e.startIndex, d = e.endIndex, f = !0; u < d; u++, f = !1) !f && ge(n.doc, a, l) && (n.split(a, l), a += 2 * l), a += c.child(u).nodeSize;
     return n
 }
 
-function Jc(n) {
+function ta(n) {
     return function(e, t) {
         let {
             $from: r,
             $to: i
-        } = e.selection, o = r.blockRange(i, s => s.childCount > 0 && s.firstChild.type == n);
-        return o ? t ? r.node(o.depth - 1).type == n ? xh(e, t, n, o) : bh(e, t, o) : !0 : !1
+        } = e.selection, s = r.blockRange(i, o => o.childCount > 0 && o.firstChild.type == n);
+        return s ? t ? r.node(s.depth - 1).type == n ? Vd(e, t, n, s) : Jd(e, t, s) : !0 : !1
     }
 }
 
-function xh(n, e, t, r) {
+function Vd(n, e, t, r) {
     let i = n.tr,
-        o = r.end,
-        s = r.$to.end(r.depth);
-    o < s && (i.step(new W(o - 1, s, o, s, new w(v.from(t.create(null, r.parent.copy())), 1, 0), 1, !0)), r = new on(i.doc.resolve(r.$from.pos), i.doc.resolve(s), r.depth));
-    let l = gt(r);
+        s = r.end,
+        o = r.$to.end(r.depth);
+    s < o && (i.step(new j(s - 1, o, s, o, new E(x.from(t.create(null, r.parent.copy())), 1, 0), 1, !0)), r = new yt(i.doc.resolve(r.$from.pos), i.doc.resolve(o), r.depth));
+    let l = je(r);
     if (l == null) return !1;
     i.lift(r, l);
-    let a = i.mapping.map(o, -1) - 1;
-    return Ke(i.doc, a) && i.join(a), e(i.scrollIntoView()), !0
+    let a = i.mapping.map(s, -1) - 1;
+    return Se(i.doc, a) && i.join(a), e(i.scrollIntoView()), !0
 }
 
-function bh(n, e, t) {
+function Jd(n, e, t) {
     let r = n.tr,
         i = t.parent;
-    for (let p = t.end, h = t.endIndex - 1, m = t.startIndex; h > m; h--) p -= i.child(h).nodeSize, r.delete(p - 1, p + 1);
-    let o = r.doc.resolve(t.start),
-        s = o.nodeAfter;
-    if (r.mapping.map(t.end) != t.start + o.nodeAfter.nodeSize) return !1;
+    for (let h = t.end, p = t.endIndex - 1, m = t.startIndex; p > m; p--) h -= i.child(p).nodeSize, r.delete(h - 1, h + 1);
+    let s = r.doc.resolve(t.start),
+        o = s.nodeAfter;
+    if (r.mapping.map(t.end) != t.start + s.nodeAfter.nodeSize) return !1;
     let l = t.startIndex == 0,
         a = t.endIndex == i.childCount,
-        c = o.node(-1),
-        u = o.index(-1);
-    if (!c.canReplace(u + (l ? 0 : 1), u + 1, s.content.append(a ? v.empty : v.from(i)))) return !1;
-    let d = o.pos,
-        f = d + s.nodeSize;
-    return r.step(new W(d - (l ? 1 : 0), f + (a ? 1 : 0), d + 1, f - 1, new w((l ? v.empty : v.from(i.copy(v.empty))).append(a ? v.empty : v.from(i.copy(v.empty))), l ? 0 : 1, a ? 0 : 1), l ? 0 : 1)), e(r.scrollIntoView()), !0
+        c = s.node(-1),
+        u = s.index(-1);
+    if (!c.canReplace(u + (l ? 0 : 1), u + 1, o.content.append(a ? x.empty : x.from(i)))) return !1;
+    let d = s.pos,
+        f = d + o.nodeSize;
+    return r.step(new j(d - (l ? 1 : 0), f + (a ? 1 : 0), d + 1, f - 1, new E((l ? x.empty : x.from(i.copy(x.empty))).append(a ? x.empty : x.from(i.copy(x.empty))), l ? 0 : 1, a ? 0 : 1), l ? 0 : 1)), e(r.scrollIntoView()), !0
 }
 
-function Kc(n) {
+function na(n) {
     return function(e, t) {
         let {
             $from: r,
             $to: i
-        } = e.selection, o = r.blockRange(i, c => c.childCount > 0 && c.firstChild.type == n);
-        if (!o) return !1;
-        let s = o.startIndex;
-        if (s == 0) return !1;
-        let l = o.parent,
-            a = l.child(s - 1);
+        } = e.selection, s = r.blockRange(i, c => c.childCount > 0 && c.firstChild.type == n);
+        if (!s) return !1;
+        let o = s.startIndex;
+        if (o == 0) return !1;
+        let l = s.parent,
+            a = l.child(o - 1);
         if (a.type != n) return !1;
         if (t) {
             let c = a.lastChild && a.lastChild.type == l.type,
-                u = v.from(c ? n.create() : null),
-                d = new w(v.from(n.create(null, v.from(l.type.create(null, u)))), c ? 3 : 1, 0),
-                f = o.start,
-                p = o.end;
-            t(e.tr.step(new W(f - (c ? 3 : 1), p, f, p, d, 1, !0)).scrollIntoView())
+                u = x.from(c ? n.create() : null),
+                d = new E(x.from(n.create(null, x.from(l.type.create(null, u)))), c ? 3 : 1, 0),
+                f = s.start,
+                h = s.end;
+            t(e.tr.step(new j(f - (c ? 3 : 1), h, f, h, d, 1, !0)).scrollIntoView())
         }
         return !0
     }
 }
 
-function fi(n) {
+function hr(n) {
     let {
         state: e,
         transaction: t
     } = n, {
         selection: r
     } = t, {
         doc: i
     } = t, {
-        storedMarks: o
+        storedMarks: s
     } = t;
     return {
         ...e,
         apply: e.apply.bind(e),
         applyTransaction: e.applyTransaction.bind(e),
         filterTransaction: e.filterTransaction,
         plugins: e.plugins,
         schema: e.schema,
         reconfigure: e.reconfigure.bind(e),
         toJSON: e.toJSON.bind(e),
         get storedMarks() {
-            return o
+            return s
         },
         get selection() {
             return r
         },
         get doc() {
             return i
         },
         get tr() {
-            return r = t.selection, i = t.doc, o = t.storedMarks, t
+            return r = t.selection, i = t.doc, s = t.storedMarks, t
         }
     }
 }
-var $n = class {
+var Gt = class {
         constructor(e) {
             this.editor = e.editor, this.rawCommands = this.editor.extensionManager.commands, this.customState = e.state
         }
         get hasCustomState() {
             return !!this.customState
         }
         get state() {
@@ -9267,85 +8037,85 @@
             let {
                 rawCommands: e,
                 editor: t,
                 state: r
             } = this, {
                 view: i
             } = t, {
-                tr: o
-            } = r, s = this.buildProps(o);
+                tr: s
+            } = r, o = this.buildProps(s);
             return Object.fromEntries(Object.entries(e).map(([l, a]) => [l, (...u) => {
-                let d = a(...u)(s);
-                return !o.getMeta("preventDispatch") && !this.hasCustomState && i.dispatch(o), d
+                let d = a(...u)(o);
+                return !s.getMeta("preventDispatch") && !this.hasCustomState && i.dispatch(s), d
             }]))
         }
         get chain() {
             return () => this.createChain()
         }
         get can() {
             return () => this.createCan()
         }
         createChain(e, t = !0) {
             let {
                 rawCommands: r,
                 editor: i,
-                state: o
+                state: s
             } = this, {
-                view: s
-            } = i, l = [], a = !!e, c = e || o.tr, u = () => (!a && t && !c.getMeta("preventDispatch") && !this.hasCustomState && s.dispatch(c), l.every(f => f === !0)), d = {
-                ...Object.fromEntries(Object.entries(r).map(([f, p]) => [f, (...m) => {
+                view: o
+            } = i, l = [], a = !!e, c = e || s.tr, u = () => (!a && t && !c.getMeta("preventDispatch") && !this.hasCustomState && o.dispatch(c), l.every(f => f === !0)), d = {
+                ...Object.fromEntries(Object.entries(r).map(([f, h]) => [f, (...m) => {
                     let b = this.buildProps(c, t),
-                        k = p(...m)(b);
-                    return l.push(k), d
+                        M = h(...m)(b);
+                    return l.push(M), d
                 }])),
                 run: u
             };
             return d
         }
         createCan(e) {
             let {
                 rawCommands: t,
                 state: r
-            } = this, i = !1, o = e || r.tr, s = this.buildProps(o, i);
+            } = this, i = !1, s = e || r.tr, o = this.buildProps(s, i);
             return {
                 ...Object.fromEntries(Object.entries(t).map(([a, c]) => [a, (...u) => c(...u)({
-                    ...s,
+                    ...o,
                     dispatch: void 0
                 })])),
-                chain: () => this.createChain(o, i)
+                chain: () => this.createChain(s, i)
             }
         }
         buildProps(e, t = !0) {
             let {
                 rawCommands: r,
                 editor: i,
-                state: o
+                state: s
             } = this, {
-                view: s
+                view: o
             } = i;
-            o.storedMarks && e.setStoredMarks(o.storedMarks);
+            s.storedMarks && e.setStoredMarks(s.storedMarks);
             let l = {
                 tr: e,
                 editor: i,
-                view: s,
-                state: fi({
-                    state: o,
+                view: o,
+                state: hr({
+                    state: s,
                     transaction: e
                 }),
                 dispatch: t ? () => {} : void 0,
                 chain: () => this.createChain(e),
                 can: () => this.createCan(e),
                 get commands() {
                     return Object.fromEntries(Object.entries(r).map(([a, c]) => [a, (...u) => c(...u)(l)]))
                 }
             };
             return l
         }
     },
-    ks = class {
+    rs = class {
         constructor() {
             this.callbacks = {}
         }
         on(e, t) {
             return this.callbacks[e] || (this.callbacks[e] = []), this.callbacks[e].push(t), this
         }
         emit(e, ...t) {
@@ -9357,2002 +8127,2002 @@
             return r && (t ? this.callbacks[e] = r.filter(i => i !== t) : delete this.callbacks[e]), this
         }
         removeAllListeners() {
             this.callbacks = {}
         }
     };
 
-function A(n, e, t) {
-    return n.config[e] === void 0 && n.parent ? A(n.parent, e, t) : typeof n.config[e] == "function" ? n.config[e].bind({
+function T(n, e, t) {
+    return n.config[e] === void 0 && n.parent ? T(n.parent, e, t) : typeof n.config[e] == "function" ? n.config[e].bind({
         ...t,
-        parent: n.parent ? A(n.parent, e, t) : null
+        parent: n.parent ? T(n.parent, e, t) : null
     }) : n.config[e]
 }
 
-function pi(n) {
+function pr(n) {
     let e = n.filter(i => i.type === "extension"),
         t = n.filter(i => i.type === "node"),
         r = n.filter(i => i.type === "mark");
     return {
         baseExtensions: e,
         nodeExtensions: t,
         markExtensions: r
     }
 }
 
-function eu(n) {
+function ua(n) {
     let e = [],
         {
             nodeExtensions: t,
             markExtensions: r
-        } = pi(n),
+        } = pr(n),
         i = [...t, ...r],
-        o = {
+        s = {
             default: null,
             rendered: !0,
             renderHTML: null,
             parseHTML: null,
             keepOnSplit: !0,
             isRequired: !1
         };
-    return n.forEach(s => {
+    return n.forEach(o => {
         let l = {
-                name: s.name,
-                options: s.options,
-                storage: s.storage
+                name: o.name,
+                options: o.options,
+                storage: o.storage
             },
-            a = A(s, "addGlobalAttributes", l);
+            a = T(o, "addGlobalAttributes", l);
         if (!a) return;
         a().forEach(u => {
             u.types.forEach(d => {
-                Object.entries(u.attributes).forEach(([f, p]) => {
+                Object.entries(u.attributes).forEach(([f, h]) => {
                     e.push({
                         type: d,
                         name: f,
                         attribute: {
-                            ...o,
-                            ...p
+                            ...s,
+                            ...h
                         }
                     })
                 })
             })
         })
-    }), i.forEach(s => {
+    }), i.forEach(o => {
         let l = {
-                name: s.name,
-                options: s.options,
-                storage: s.storage
+                name: o.name,
+                options: o.options,
+                storage: o.storage
             },
-            a = A(s, "addAttributes", l);
+            a = T(o, "addAttributes", l);
         if (!a) return;
         let c = a();
         Object.entries(c).forEach(([u, d]) => {
             let f = {
-                ...o,
+                ...s,
                 ...d
             };
             typeof(f == null ? void 0 : f.default) == "function" && (f.default = f.default()), f != null && f.isRequired && (f == null ? void 0 : f.default) === void 0 && delete f.default, e.push({
-                type: s.name,
+                type: o.name,
                 name: u,
                 attribute: f
             })
         })
     }), e
 }
 
-function ce(n, e) {
+function Y(n, e) {
     if (typeof n == "string") {
         if (!e.nodes[n]) throw Error(`There is no node type named '${n}'. Maybe you forgot to add the extension?`);
         return e.nodes[n]
     }
     return n
 }
 
-function z(...n) {
+function P(...n) {
     return n.filter(e => !!e).reduce((e, t) => {
         let r = {
             ...e
         };
-        return Object.entries(t).forEach(([i, o]) => {
+        return Object.entries(t).forEach(([i, s]) => {
             if (!r[i]) {
-                r[i] = o;
+                r[i] = s;
                 return
             }
-            i === "class" ? r[i] = [r[i], o].join(" ") : i === "style" ? r[i] = [r[i], o].join("; ") : r[i] = o
+            i === "class" ? r[i] = [r[i], s].join(" ") : i === "style" ? r[i] = [r[i], s].join("; ") : r[i] = s
         }), r
     }, {})
 }
 
-function vs(n, e) {
+function is(n, e) {
     return e.filter(t => t.attribute.rendered).map(t => t.attribute.renderHTML ? t.attribute.renderHTML(n.attrs) || {} : {
         [t.name]: n.attrs[t.name]
-    }).reduce((t, r) => z(t, r), {})
+    }).reduce((t, r) => P(t, r), {})
 }
 
-function tu(n) {
+function da(n) {
     return typeof n == "function"
 }
 
-function B(n, e = void 0, ...t) {
-    return tu(n) ? e ? n.bind(e)(...t) : n(...t) : n
+function R(n, e = void 0, ...t) {
+    return da(n) ? e ? n.bind(e)(...t) : n(...t) : n
 }
 
-function kh(n = {}) {
+function Wd(n = {}) {
     return Object.keys(n).length === 0 && n.constructor === Object
 }
 
-function vh(n) {
+function qd(n) {
     return typeof n != "string" ? n : n.match(/^[+-]?(?:\d*\.)?\d+$/) ? Number(n) : n === "true" ? !0 : n === "false" ? !1 : n
 }
 
-function Uc(n, e) {
+function ra(n, e) {
     return n.style ? n : {
         ...n,
         getAttrs: t => {
             let r = n.getAttrs ? n.getAttrs(t) : n.attrs;
             if (r === !1) return !1;
-            let i = e.reduce((o, s) => {
-                let l = s.attribute.parseHTML ? s.attribute.parseHTML(t) : vh(t.getAttribute(s.name));
-                return l == null ? o : {
-                    ...o,
-                    [s.name]: l
+            let i = e.reduce((s, o) => {
+                let l = o.attribute.parseHTML ? o.attribute.parseHTML(t) : qd(t.getAttribute(o.name));
+                return l == null ? s : {
+                    ...s,
+                    [o.name]: l
                 }
             }, {});
             return {
                 ...r,
                 ...i
             }
         }
     }
 }
 
-function _c(n) {
-    return Object.fromEntries(Object.entries(n).filter(([e, t]) => e === "attrs" && kh(t) ? !1 : t != null))
+function ia(n) {
+    return Object.fromEntries(Object.entries(n).filter(([e, t]) => e === "attrs" && Wd(t) ? !1 : t != null))
 }
 
-function Mh(n, e) {
+function Kd(n, e) {
     var t;
-    let r = eu(n),
+    let r = ua(n),
         {
             nodeExtensions: i,
-            markExtensions: o
-        } = pi(n),
-        s = (t = i.find(c => A(c, "topNode"))) === null || t === void 0 ? void 0 : t.name,
+            markExtensions: s
+        } = pr(n),
+        o = (t = i.find(c => T(c, "topNode"))) === null || t === void 0 ? void 0 : t.name,
         l = Object.fromEntries(i.map(c => {
-            let u = r.filter(k => k.type === c.name),
+            let u = r.filter(M => M.type === c.name),
                 d = {
                     name: c.name,
                     options: c.options,
                     storage: c.storage,
                     editor: e
                 },
-                f = n.reduce((k, S) => {
-                    let C = A(S, "extendNodeSchema", d);
+                f = n.reduce((M, w) => {
+                    let v = T(w, "extendNodeSchema", d);
                     return {
-                        ...k,
-                        ...C ? C(c) : {}
+                        ...M,
+                        ...v ? v(c) : {}
                     }
                 }, {}),
-                p = _c({
+                h = ia({
                     ...f,
-                    content: B(A(c, "content", d)),
-                    marks: B(A(c, "marks", d)),
-                    group: B(A(c, "group", d)),
-                    inline: B(A(c, "inline", d)),
-                    atom: B(A(c, "atom", d)),
-                    selectable: B(A(c, "selectable", d)),
-                    draggable: B(A(c, "draggable", d)),
-                    code: B(A(c, "code", d)),
-                    defining: B(A(c, "defining", d)),
-                    isolating: B(A(c, "isolating", d)),
-                    attrs: Object.fromEntries(u.map(k => {
-                        var S;
-                        return [k.name, {
-                            default: (S = k == null ? void 0 : k.attribute) === null || S === void 0 ? void 0 : S.default
+                    content: R(T(c, "content", d)),
+                    marks: R(T(c, "marks", d)),
+                    group: R(T(c, "group", d)),
+                    inline: R(T(c, "inline", d)),
+                    atom: R(T(c, "atom", d)),
+                    selectable: R(T(c, "selectable", d)),
+                    draggable: R(T(c, "draggable", d)),
+                    code: R(T(c, "code", d)),
+                    defining: R(T(c, "defining", d)),
+                    isolating: R(T(c, "isolating", d)),
+                    attrs: Object.fromEntries(u.map(M => {
+                        var w;
+                        return [M.name, {
+                            default: (w = M == null ? void 0 : M.attribute) === null || w === void 0 ? void 0 : w.default
                         }]
                     }))
                 }),
-                h = B(A(c, "parseHTML", d));
-            h && (p.parseDOM = h.map(k => Uc(k, u)));
-            let m = A(c, "renderHTML", d);
-            m && (p.toDOM = k => m({
-                node: k,
-                HTMLAttributes: vs(k, u)
+                p = R(T(c, "parseHTML", d));
+            p && (h.parseDOM = p.map(M => ra(M, u)));
+            let m = T(c, "renderHTML", d);
+            m && (h.toDOM = M => m({
+                node: M,
+                HTMLAttributes: is(M, u)
             }));
-            let b = A(c, "renderText", d);
-            return b && (p.toText = b), [c.name, p]
+            let b = T(c, "renderText", d);
+            return b && (h.toText = b), [c.name, h]
         })),
-        a = Object.fromEntries(o.map(c => {
+        a = Object.fromEntries(s.map(c => {
             let u = r.filter(b => b.type === c.name),
                 d = {
                     name: c.name,
                     options: c.options,
                     storage: c.storage,
                     editor: e
                 },
-                f = n.reduce((b, k) => {
-                    let S = A(k, "extendMarkSchema", d);
+                f = n.reduce((b, M) => {
+                    let w = T(M, "extendMarkSchema", d);
                     return {
                         ...b,
-                        ...S ? S(c) : {}
+                        ...w ? w(c) : {}
                     }
                 }, {}),
-                p = _c({
+                h = ia({
                     ...f,
-                    inclusive: B(A(c, "inclusive", d)),
-                    excludes: B(A(c, "excludes", d)),
-                    group: B(A(c, "group", d)),
-                    spanning: B(A(c, "spanning", d)),
-                    code: B(A(c, "code", d)),
+                    inclusive: R(T(c, "inclusive", d)),
+                    excludes: R(T(c, "excludes", d)),
+                    group: R(T(c, "group", d)),
+                    spanning: R(T(c, "spanning", d)),
+                    code: R(T(c, "code", d)),
                     attrs: Object.fromEntries(u.map(b => {
-                        var k;
+                        var M;
                         return [b.name, {
-                            default: (k = b == null ? void 0 : b.attribute) === null || k === void 0 ? void 0 : k.default
+                            default: (M = b == null ? void 0 : b.attribute) === null || M === void 0 ? void 0 : M.default
                         }]
                     }))
                 }),
-                h = B(A(c, "parseHTML", d));
-            h && (p.parseDOM = h.map(b => Uc(b, u)));
-            let m = A(c, "renderHTML", d);
-            return m && (p.toDOM = b => m({
+                p = R(T(c, "parseHTML", d));
+            p && (h.parseDOM = p.map(b => ra(b, u)));
+            let m = T(c, "renderHTML", d);
+            return m && (h.toDOM = b => m({
                 mark: b,
-                HTMLAttributes: vs(b, u)
-            })), [c.name, p]
+                HTMLAttributes: is(b, u)
+            })), [c.name, h]
         }));
-    return new Wr({
-        topNode: s,
+    return new Wn({
+        topNode: o,
         nodes: l,
         marks: a
     })
 }
 
-function ms(n, e) {
+function Xi(n, e) {
     return e.nodes[n] || e.marks[n] || null
 }
 
-function Gc(n, e) {
+function sa(n, e) {
     return Array.isArray(e) ? e.some(t => (typeof t == "string" ? t : t.name) === n.name) : e
 }
-var Eh = (n, e = 500) => {
+var Ud = (n, e = 500) => {
     let t = "",
         r = n.parentOffset;
-    return n.parent.nodesBetween(Math.max(0, r - e), r, (i, o, s, l) => {
+    return n.parent.nodesBetween(Math.max(0, r - e), r, (i, s, o, l) => {
         var a, c;
         let u = ((c = (a = i.type.spec).toText) === null || c === void 0 ? void 0 : c.call(a, {
             node: i,
-            pos: o,
-            parent: s,
+            pos: s,
+            parent: o,
             index: l
         })) || i.textContent || "%leaf%";
-        t += u.slice(0, Math.max(0, r - o))
+        t += u.slice(0, Math.max(0, r - s))
     }), t
 };
 
-function ws(n) {
+function cs(n) {
     return Object.prototype.toString.call(n) === "[object RegExp]"
 }
-var Wn = class {
+var Qt = class {
         constructor(e) {
             this.find = e.find, this.handler = e.handler
         }
     },
-    Sh = (n, e) => {
-        if (ws(e)) return e.exec(n);
+    _d = (n, e) => {
+        if (cs(e)) return e.exec(n);
         let t = e(n);
         if (!t) return null;
         let r = [t.text];
         return r.index = t.index, r.input = n, r.data = t.data, t.replaceWith && (t.text.includes(t.replaceWith) || console.warn('[tiptap warn]: "inputRuleMatch.replaceWith" must be part of "inputRuleMatch.text".'), r.push(t.replaceWith)), r
     };
 
-function gs(n) {
+function Zi(n) {
     var e;
     let {
         editor: t,
         from: r,
         to: i,
-        text: o,
-        rules: s,
+        text: s,
+        rules: o,
         plugin: l
     } = n, {
         view: a
     } = t;
     if (a.composing) return !1;
     let c = a.state.doc.resolve(r);
     if (c.parent.type.spec.code || !((e = c.nodeBefore || c.nodeAfter) === null || e === void 0) && e.marks.find(f => f.type.spec.code)) return !1;
     let u = !1,
-        d = Eh(c) + o;
-    return s.forEach(f => {
+        d = Ud(c) + s;
+    return o.forEach(f => {
         if (u) return;
-        let p = Sh(d, f.find);
-        if (!p) return;
-        let h = a.state.tr,
-            m = fi({
+        let h = _d(d, f.find);
+        if (!h) return;
+        let p = a.state.tr,
+            m = hr({
                 state: a.state,
-                transaction: h
+                transaction: p
             }),
             b = {
-                from: r - (p[0].length - o.length),
+                from: r - (h[0].length - s.length),
                 to: i
             },
             {
-                commands: k,
-                chain: S,
-                can: C
-            } = new $n({
+                commands: M,
+                chain: w,
+                can: v
+            } = new Gt({
                 editor: t,
                 state: m
             });
         f.handler({
             state: m,
             range: b,
-            match: p,
-            commands: k,
-            chain: S,
-            can: C
-        }) === null || !h.steps.length || (h.setMeta(l, {
-            transform: h,
+            match: h,
+            commands: M,
+            chain: w,
+            can: v
+        }) === null || !p.steps.length || (p.setMeta(l, {
+            transform: p,
             from: r,
             to: i,
-            text: o
-        }), a.dispatch(h), u = !0)
+            text: s
+        }), a.dispatch(p), u = !0)
     }), u
 }
 
-function wh(n) {
+function Gd(n) {
     let {
         editor: e,
         rules: t
-    } = n, r = new q({
+    } = n, r = new $({
         state: {
             init() {
                 return null
             },
-            apply(i, o) {
-                let s = i.getMeta(r);
-                return s || (i.selectionSet || i.docChanged ? null : o)
+            apply(i, s) {
+                let o = i.getMeta(r);
+                return o || (i.selectionSet || i.docChanged ? null : s)
             }
         },
         props: {
-            handleTextInput(i, o, s, l) {
-                return gs({
+            handleTextInput(i, s, o, l) {
+                return Zi({
                     editor: e,
-                    from: o,
-                    to: s,
+                    from: s,
+                    to: o,
                     text: l,
                     rules: t,
                     plugin: r
                 })
             },
             handleDOMEvents: {
                 compositionend: i => (setTimeout(() => {
                     let {
-                        $cursor: o
+                        $cursor: s
                     } = i.state.selection;
-                    o && gs({
+                    s && Zi({
                         editor: e,
-                        from: o.pos,
-                        to: o.pos,
+                        from: s.pos,
+                        to: s.pos,
                         text: "",
                         rules: t,
                         plugin: r
                     })
                 }), !1)
             },
-            handleKeyDown(i, o) {
-                if (o.key !== "Enter") return !1;
+            handleKeyDown(i, s) {
+                if (s.key !== "Enter") return !1;
                 let {
-                    $cursor: s
+                    $cursor: o
                 } = i.state.selection;
-                return s ? gs({
+                return o ? Zi({
                     editor: e,
-                    from: s.pos,
-                    to: s.pos,
+                    from: o.pos,
+                    to: o.pos,
                     text: `
 `,
                     rules: t,
                     plugin: r
                 }) : !1
             }
         },
         isInputRules: !0
     });
     return r
 }
 
-function Th(n) {
+function Qd(n) {
     return typeof n == "number"
 }
-var Ms = class {
+var ss = class {
         constructor(e) {
             this.find = e.find, this.handler = e.handler
         }
     },
-    Ch = (n, e) => {
-        if (ws(e)) return [...n.matchAll(e)];
+    Yd = (n, e) => {
+        if (cs(e)) return [...n.matchAll(e)];
         let t = e(n);
         return t ? t.map(r => {
             let i = [r.text];
             return i.index = r.index, i.input = n, i.data = r.data, r.replaceWith && (r.text.includes(r.replaceWith) || console.warn('[tiptap warn]: "pasteRuleMatch.replaceWith" must be part of "pasteRuleMatch.text".'), i.push(r.replaceWith)), i
         }) : []
     };
 
-function Oh(n) {
+function Xd(n) {
     let {
         editor: e,
         state: t,
         from: r,
         to: i,
-        rule: o
+        rule: s
     } = n, {
-        commands: s,
+        commands: o,
         chain: l,
         can: a
-    } = new $n({
+    } = new Gt({
         editor: e,
         state: t
     }), c = [];
     return t.doc.nodesBetween(r, i, (d, f) => {
         if (!d.isTextblock || d.type.spec.code) return;
-        let p = Math.max(r, f),
-            h = Math.min(i, f + d.content.size),
-            m = d.textBetween(p - f, h - f, void 0, "\uFFFC");
-        Ch(m, o.find).forEach(k => {
-            if (k.index === void 0) return;
-            let S = p + k.index + 1,
-                C = S + k[0].length,
-                T = {
-                    from: t.tr.mapping.map(S),
-                    to: t.tr.mapping.map(C)
+        let h = Math.max(r, f),
+            p = Math.min(i, f + d.content.size),
+            m = d.textBetween(h - f, p - f, void 0, "\uFFFC");
+        Yd(m, s.find).forEach(M => {
+            if (M.index === void 0) return;
+            let w = h + M.index + 1,
+                v = w + M[0].length,
+                D = {
+                    from: t.tr.mapping.map(w),
+                    to: t.tr.mapping.map(v)
                 },
-                E = o.handler({
+                A = s.handler({
                     state: t,
-                    range: T,
-                    match: k,
-                    commands: s,
+                    range: D,
+                    match: M,
+                    commands: o,
                     chain: l,
                     can: a
                 });
-            c.push(E)
+            c.push(A)
         })
     }), c.every(d => d !== null)
 }
 
-function Ah(n) {
+function Zd(n) {
     let {
         editor: e,
         rules: t
-    } = n, r = null, i = !1, o = !1;
-    return t.map(l => new q({
+    } = n, r = null, i = !1, s = !1;
+    return t.map(l => new $({
         view(a) {
             let c = u => {
                 var d;
                 r = !((d = a.dom.parentElement) === null || d === void 0) && d.contains(u.target) ? a.dom.parentElement : null
             };
             return window.addEventListener("dragstart", c), {
                 destroy() {
                     window.removeEventListener("dragstart", c)
                 }
             }
         },
         props: {
             handleDOMEvents: {
-                drop: a => (o = r === a.dom.parentElement, !1),
+                drop: a => (s = r === a.dom.parentElement, !1),
                 paste: (a, c) => {
                     var u;
                     let d = (u = c.clipboardData) === null || u === void 0 ? void 0 : u.getData("text/html");
                     return i = !!(d != null && d.includes("data-pm-slice")), !1
                 }
             }
         },
         appendTransaction: (a, c, u) => {
             let d = a[0],
                 f = d.getMeta("uiEvent") === "paste" && !i,
-                p = d.getMeta("uiEvent") === "drop" && !o;
-            if (!f && !p) return;
-            let h = c.doc.content.findDiffStart(u.doc.content),
+                h = d.getMeta("uiEvent") === "drop" && !s;
+            if (!f && !h) return;
+            let p = c.doc.content.findDiffStart(u.doc.content),
                 m = c.doc.content.findDiffEnd(u.doc.content);
-            if (!Th(h) || !m || h === m.b) return;
+            if (!Qd(p) || !m || p === m.b) return;
             let b = u.tr,
-                k = fi({
+                M = hr({
                     state: u,
                     transaction: b
                 });
-            if (!(!Oh({
+            if (!(!Xd({
                     editor: e,
-                    state: k,
-                    from: Math.max(h - 1, 0),
+                    state: M,
+                    from: Math.max(p - 1, 0),
                     to: m.b - 1,
                     rule: l
                 }) || !b.steps.length)) return b
         }
     }))
 }
 
-function Nh(n) {
+function ef(n) {
     let e = n.filter((t, r) => n.indexOf(t) !== r);
     return [...new Set(e)]
 }
-var Bt = class {
+var nt = class {
     constructor(e, t) {
-        this.splittableMarks = [], this.editor = t, this.extensions = Bt.resolve(e), this.schema = Mh(this.extensions, t), this.extensions.forEach(r => {
+        this.splittableMarks = [], this.editor = t, this.extensions = nt.resolve(e), this.schema = Kd(this.extensions, t), this.extensions.forEach(r => {
             var i;
             this.editor.extensionStorage[r.name] = r.storage;
-            let o = {
+            let s = {
                 name: r.name,
                 options: r.options,
                 storage: r.storage,
                 editor: this.editor,
-                type: ms(r.name, this.schema)
+                type: Xi(r.name, this.schema)
             };
-            r.type === "mark" && (!((i = B(A(r, "keepOnSplit", o))) !== null && i !== void 0) || i) && this.splittableMarks.push(r.name);
-            let s = A(r, "onBeforeCreate", o);
-            s && this.editor.on("beforeCreate", s);
-            let l = A(r, "onCreate", o);
+            r.type === "mark" && (!((i = R(T(r, "keepOnSplit", s))) !== null && i !== void 0) || i) && this.splittableMarks.push(r.name);
+            let o = T(r, "onBeforeCreate", s);
+            o && this.editor.on("beforeCreate", o);
+            let l = T(r, "onCreate", s);
             l && this.editor.on("create", l);
-            let a = A(r, "onUpdate", o);
+            let a = T(r, "onUpdate", s);
             a && this.editor.on("update", a);
-            let c = A(r, "onSelectionUpdate", o);
+            let c = T(r, "onSelectionUpdate", s);
             c && this.editor.on("selectionUpdate", c);
-            let u = A(r, "onTransaction", o);
+            let u = T(r, "onTransaction", s);
             u && this.editor.on("transaction", u);
-            let d = A(r, "onFocus", o);
+            let d = T(r, "onFocus", s);
             d && this.editor.on("focus", d);
-            let f = A(r, "onBlur", o);
+            let f = T(r, "onBlur", s);
             f && this.editor.on("blur", f);
-            let p = A(r, "onDestroy", o);
-            p && this.editor.on("destroy", p)
+            let h = T(r, "onDestroy", s);
+            h && this.editor.on("destroy", h)
         })
     }
     static resolve(e) {
-        let t = Bt.sort(Bt.flatten(e)),
-            r = Nh(t.map(i => i.name));
+        let t = nt.sort(nt.flatten(e)),
+            r = ef(t.map(i => i.name));
         return r.length && console.warn(`[tiptap warn]: Duplicate extension names found: [${r.map(i=>`'${i}'`).join(", ")}]. This can lead to issues.`), t
     }
     static flatten(e) {
         return e.map(t => {
             let r = {
                     name: t.name,
                     options: t.options,
                     storage: t.storage
                 },
-                i = A(t, "addExtensions", r);
+                i = T(t, "addExtensions", r);
             return i ? [t, ...this.flatten(i())] : t
         }).flat(10)
     }
     static sort(e) {
         return e.sort((r, i) => {
-            let o = A(r, "priority") || 100,
-                s = A(i, "priority") || 100;
-            return o > s ? -1 : o < s ? 1 : 0
+            let s = T(r, "priority") || 100,
+                o = T(i, "priority") || 100;
+            return s > o ? -1 : s < o ? 1 : 0
         })
     }
     get commands() {
         return this.extensions.reduce((e, t) => {
             let r = {
                     name: t.name,
                     options: t.options,
                     storage: t.storage,
                     editor: this.editor,
-                    type: ms(t.name, this.schema)
+                    type: Xi(t.name, this.schema)
                 },
-                i = A(t, "addCommands", r);
+                i = T(t, "addCommands", r);
             return i ? {
                 ...e,
                 ...i()
             } : e
         }, {})
     }
     get plugins() {
         let {
             editor: e
-        } = this, t = Bt.sort([...this.extensions].reverse()), r = [], i = [], o = t.map(s => {
+        } = this, t = nt.sort([...this.extensions].reverse()), r = [], i = [], s = t.map(o => {
             let l = {
-                    name: s.name,
-                    options: s.options,
-                    storage: s.storage,
+                    name: o.name,
+                    options: o.options,
+                    storage: o.storage,
                     editor: e,
-                    type: ms(s.name, this.schema)
+                    type: Xi(o.name, this.schema)
                 },
                 a = [],
-                c = A(s, "addKeyboardShortcuts", l),
+                c = T(o, "addKeyboardShortcuts", l),
                 u = {};
-            if (s.type === "mark" && s.config.exitable && (u.ArrowRight = () => V.handleExit({
+            if (o.type === "mark" && o.config.exitable && (u.ArrowRight = () => F.handleExit({
                     editor: e,
-                    mark: s
+                    mark: o
                 })), c) {
-                let m = Object.fromEntries(Object.entries(c()).map(([b, k]) => [b, () => k({
+                let m = Object.fromEntries(Object.entries(c()).map(([b, M]) => [b, () => M({
                     editor: e
                 })]));
                 u = {
                     ...u,
                     ...m
                 }
             }
-            let d = Lc(u);
+            let d = Jl(u);
             a.push(d);
-            let f = A(s, "addInputRules", l);
-            Gc(s, e.options.enableInputRules) && f && r.push(...f());
-            let p = A(s, "addPasteRules", l);
-            Gc(s, e.options.enablePasteRules) && p && i.push(...p());
-            let h = A(s, "addProseMirrorPlugins", l);
-            if (h) {
-                let m = h();
+            let f = T(o, "addInputRules", l);
+            sa(o, e.options.enableInputRules) && f && r.push(...f());
+            let h = T(o, "addPasteRules", l);
+            sa(o, e.options.enablePasteRules) && h && i.push(...h());
+            let p = T(o, "addProseMirrorPlugins", l);
+            if (p) {
+                let m = p();
                 a.push(...m)
             }
             return a
         }).flat();
-        return [wh({
+        return [Gd({
             editor: e,
             rules: r
-        }), ...Ah({
+        }), ...Zd({
             editor: e,
             rules: i
-        }), ...o]
+        }), ...s]
     }
     get attributes() {
-        return eu(this.extensions)
+        return ua(this.extensions)
     }
     get nodeViews() {
         let {
             editor: e
         } = this, {
             nodeExtensions: t
-        } = pi(this.extensions);
-        return Object.fromEntries(t.filter(r => !!A(r, "addNodeView")).map(r => {
+        } = pr(this.extensions);
+        return Object.fromEntries(t.filter(r => !!T(r, "addNodeView")).map(r => {
             let i = this.attributes.filter(a => a.type === r.name),
-                o = {
+                s = {
                     name: r.name,
                     options: r.options,
                     storage: r.storage,
                     editor: e,
-                    type: ce(r.name, this.schema)
+                    type: Y(r.name, this.schema)
                 },
-                s = A(r, "addNodeView", o);
-            if (!s) return [];
+                o = T(r, "addNodeView", s);
+            if (!o) return [];
             let l = (a, c, u, d) => {
-                let f = vs(a, i);
-                return s()({
+                let f = is(a, i);
+                return o()({
                     editor: e,
                     node: a,
                     getPos: u,
                     decorations: d,
                     HTMLAttributes: f,
                     extension: r
                 })
             };
             return [r.name, l]
         }))
     }
 };
 
-function Ih(n) {
+function tf(n) {
     return Object.prototype.toString.call(n).slice(8, -1)
 }
 
-function ys(n) {
-    return Ih(n) !== "Object" ? !1 : n.constructor === Object && Object.getPrototypeOf(n) === Object.prototype
+function es(n) {
+    return tf(n) !== "Object" ? !1 : n.constructor === Object && Object.getPrototypeOf(n) === Object.prototype
 }
 
-function hi(n, e) {
+function mr(n, e) {
     let t = {
         ...n
     };
-    return ys(n) && ys(e) && Object.keys(e).forEach(r => {
-        ys(e[r]) ? r in n ? t[r] = hi(n[r], e[r]) : Object.assign(t, {
+    return es(n) && es(e) && Object.keys(e).forEach(r => {
+        es(e[r]) ? r in n ? t[r] = mr(n[r], e[r]) : Object.assign(t, {
             [r]: e[r]
         }) : Object.assign(t, {
             [r]: e[r]
         })
     }), t
 }
-var J = class {
+var V = class {
     constructor(e = {}) {
         this.type = "extension", this.name = "extension", this.parent = null, this.child = null, this.config = {
             name: this.name,
             defaultOptions: {}
         }, this.config = {
             ...this.config,
             ...e
-        }, this.name = this.config.name, e.defaultOptions && console.warn(`[tiptap warn]: BREAKING CHANGE: "defaultOptions" is deprecated. Please use "addOptions" instead. Found in extension: "${this.name}".`), this.options = this.config.defaultOptions, this.config.addOptions && (this.options = B(A(this, "addOptions", {
+        }, this.name = this.config.name, e.defaultOptions && console.warn(`[tiptap warn]: BREAKING CHANGE: "defaultOptions" is deprecated. Please use "addOptions" instead. Found in extension: "${this.name}".`), this.options = this.config.defaultOptions, this.config.addOptions && (this.options = R(T(this, "addOptions", {
             name: this.name
-        }))), this.storage = B(A(this, "addStorage", {
+        }))), this.storage = R(T(this, "addStorage", {
             name: this.name,
             options: this.options
         })) || {}
     }
     static create(e = {}) {
-        return new J(e)
+        return new V(e)
     }
     configure(e = {}) {
         let t = this.extend();
-        return t.options = hi(this.options, e), t.storage = B(A(t, "addStorage", {
+        return t.options = mr(this.options, e), t.storage = R(T(t, "addStorage", {
             name: t.name,
             options: t.options
         })), t
     }
     extend(e = {}) {
-        let t = new J(e);
-        return t.parent = this, this.child = t, t.name = e.name ? e.name : t.parent.name, e.defaultOptions && console.warn(`[tiptap warn]: BREAKING CHANGE: "defaultOptions" is deprecated. Please use "addOptions" instead. Found in extension: "${t.name}".`), t.options = B(A(t, "addOptions", {
+        let t = new V(e);
+        return t.parent = this, this.child = t, t.name = e.name ? e.name : t.parent.name, e.defaultOptions && console.warn(`[tiptap warn]: BREAKING CHANGE: "defaultOptions" is deprecated. Please use "addOptions" instead. Found in extension: "${t.name}".`), t.options = R(T(t, "addOptions", {
             name: t.name
-        })), t.storage = B(A(t, "addStorage", {
+        })), t.storage = R(T(t, "addStorage", {
             name: t.name,
             options: t.options
         })), t
     }
 };
 
-function nu(n, e, t) {
+function fa(n, e, t) {
     let {
         from: r,
         to: i
     } = e, {
-        blockSeparator: o = `
+        blockSeparator: s = `
 
 `,
-        textSerializers: s = {}
+        textSerializers: o = {}
     } = t || {}, l = "", a = !0;
     return n.nodesBetween(r, i, (c, u, d, f) => {
-        var p;
-        let h = s == null ? void 0 : s[c.type.name];
-        h ? (c.isBlock && !a && (l += o, a = !0), d && (l += h({
+        var h;
+        let p = o == null ? void 0 : o[c.type.name];
+        p ? (c.isBlock && !a && (l += s, a = !0), d && (l += p({
             node: c,
             pos: u,
             parent: d,
             index: f,
             range: e
-        }))) : c.isText ? (l += (p = c == null ? void 0 : c.text) === null || p === void 0 ? void 0 : p.slice(Math.max(r, u) - u, i - u), a = !1) : c.isBlock && !a && (l += o, a = !0)
+        }))) : c.isText ? (l += (h = c == null ? void 0 : c.text) === null || h === void 0 ? void 0 : h.slice(Math.max(r, u) - u, i - u), a = !1) : c.isBlock && !a && (l += s, a = !0)
     }), l
 }
 
-function ru(n) {
+function ha(n) {
     return Object.fromEntries(Object.entries(n.nodes).filter(([, e]) => e.spec.toText).map(([e, t]) => [e, t.spec.toText]))
 }
-var Dh = J.create({
+var nf = V.create({
         name: "clipboardTextSerializer",
         addProseMirrorPlugins() {
-            return [new q({
-                key: new Z("clipboardTextSerializer"),
+            return [new $({
+                key: new U("clipboardTextSerializer"),
                 props: {
                     clipboardTextSerializer: () => {
                         let {
                             editor: n
                         } = this, {
                             state: e,
                             schema: t
                         } = n, {
                             doc: r,
                             selection: i
                         } = e, {
-                            ranges: o
-                        } = i, s = Math.min(...o.map(u => u.$from.pos)), l = Math.max(...o.map(u => u.$to.pos)), a = ru(t);
-                        return nu(r, {
-                            from: s,
+                            ranges: s
+                        } = i, o = Math.min(...s.map(u => u.$from.pos)), l = Math.max(...s.map(u => u.$to.pos)), a = ha(t);
+                        return fa(r, {
+                            from: o,
                             to: l
                         }, {
                             textSerializers: a
                         })
                     }
                 }
             })]
         }
     }),
-    Lh = () => ({
+    rf = () => ({
         editor: n,
         view: e
     }) => (requestAnimationFrame(() => {
         var t;
         n.isDestroyed || (e.dom.blur(), (t = window == null ? void 0 : window.getSelection()) === null || t === void 0 || t.removeAllRanges())
     }), !0),
-    Ph = (n = !1) => ({
+    sf = (n = !1) => ({
         commands: e
     }) => e.setContent("", n),
-    Rh = () => ({
+    of = () => ({
         state: n,
         tr: e,
         dispatch: t
     }) => {
         let {
             selection: r
         } = e, {
             ranges: i
         } = r;
         return t && i.forEach(({
-            $from: o,
-            $to: s
+            $from: s,
+            $to: o
         }) => {
-            n.doc.nodesBetween(o.pos, s.pos, (l, a) => {
+            n.doc.nodesBetween(s.pos, o.pos, (l, a) => {
                 if (l.type.isText) return;
                 let {
                     doc: c,
                     mapping: u
-                } = e, d = c.resolve(u.map(a)), f = c.resolve(u.map(a + l.nodeSize)), p = d.blockRange(f);
-                if (!p) return;
-                let h = gt(p);
+                } = e, d = c.resolve(u.map(a)), f = c.resolve(u.map(a + l.nodeSize)), h = d.blockRange(f);
+                if (!h) return;
+                let p = je(h);
                 if (l.type.isTextblock) {
                     let {
                         defaultType: m
                     } = d.parent.contentMatchAt(d.index());
-                    e.setNodeMarkup(p.start, m)
-                }(h || h === 0) && e.lift(p, h)
+                    e.setNodeMarkup(h.start, m)
+                }(p || p === 0) && e.lift(h, p)
             })
         }), !0
     },
-    Bh = n => e => n(e),
-    zh = () => ({
+    lf = n => e => n(e),
+    af = () => ({
         state: n,
         dispatch: e
-    }) => cs(n, e),
-    Hh = () => ({
+    }) => Ki(n, e),
+    cf = () => ({
         tr: n,
         dispatch: e
     }) => {
         let {
             selection: t
         } = n, r = t.$anchor.node();
         if (r.content.size > 0) return !1;
         let i = n.selection.$anchor;
-        for (let o = i.depth; o > 0; o -= 1)
-            if (i.node(o).type === r.type) {
+        for (let s = i.depth; s > 0; s -= 1)
+            if (i.node(s).type === r.type) {
                 if (e) {
-                    let l = i.before(o),
-                        a = i.after(o);
+                    let l = i.before(s),
+                        a = i.after(s);
                     n.delete(l, a).scrollIntoView()
                 }
                 return !0
             } return !1
     },
-    Fh = n => ({
+    uf = n => ({
         tr: e,
         state: t,
         dispatch: r
     }) => {
-        let i = ce(n, t.schema),
-            o = e.selection.$anchor;
-        for (let s = o.depth; s > 0; s -= 1)
-            if (o.node(s).type === i) {
+        let i = Y(n, t.schema),
+            s = e.selection.$anchor;
+        for (let o = s.depth; o > 0; o -= 1)
+            if (s.node(o).type === i) {
                 if (r) {
-                    let a = o.before(s),
-                        c = o.after(s);
+                    let a = s.before(o),
+                        c = s.after(o);
                     e.delete(a, c).scrollIntoView()
                 }
                 return !0
             } return !1
     },
-    jh = n => ({
+    df = n => ({
         tr: e,
         dispatch: t
     }) => {
         let {
             from: r,
             to: i
         } = n;
         return t && e.delete(r, i), !0
     },
-    Vh = () => ({
+    ff = () => ({
         state: n,
         dispatch: e
-    }) => li(n, e),
-    $h = () => ({
+    }) => ar(n, e),
+    hf = () => ({
         commands: n
     }) => n.keyboardShortcut("Enter"),
-    Wh = () => ({
+    pf = () => ({
         state: n,
         dispatch: e
-    }) => as(n, e);
+    }) => qi(n, e);
 
-function ci(n, e, t = {
+function ur(n, e, t = {
     strict: !0
 }) {
     let r = Object.keys(e);
-    return r.length ? r.every(i => t.strict ? e[i] === n[i] : ws(e[i]) ? e[i].test(n[i]) : e[i] === n[i]) : !0
+    return r.length ? r.every(i => t.strict ? e[i] === n[i] : cs(e[i]) ? e[i].test(n[i]) : e[i] === n[i]) : !0
 }
 
-function Es(n, e, t = {}) {
-    return n.find(r => r.type === e && ci(r.attrs, t))
+function ls(n, e, t = {}) {
+    return n.find(r => r.type === e && ur(r.attrs, t))
 }
 
-function qh(n, e, t = {}) {
-    return !!Es(n, e, t)
+function mf(n, e, t = {}) {
+    return !!ls(n, e, t)
 }
 
-function Ts(n, e, t = {}) {
+function us(n, e, t = {}) {
     if (!n || !e) return;
     let r = n.parent.childAfter(n.parentOffset);
     if (n.parentOffset === r.offset && r.offset !== 0 && (r = n.parent.childBefore(n.parentOffset)), !r.node) return;
-    let i = Es([...r.node.marks], e, t);
+    let i = ls([...r.node.marks], e, t);
     if (!i) return;
-    let o = r.index,
-        s = n.start() + r.offset,
-        l = o + 1,
-        a = s + r.node.nodeSize;
-    for (Es([...r.node.marks], e, t); o > 0 && i.isInSet(n.parent.child(o - 1).marks);) o -= 1, s -= n.parent.child(o).nodeSize;
-    for (; l < n.parent.childCount && qh([...n.parent.child(l).marks], e, t);) a += n.parent.child(l).nodeSize, l += 1;
+    let s = r.index,
+        o = n.start() + r.offset,
+        l = s + 1,
+        a = o + r.node.nodeSize;
+    for (ls([...r.node.marks], e, t); s > 0 && i.isInSet(n.parent.child(s - 1).marks);) s -= 1, o -= n.parent.child(s).nodeSize;
+    for (; l < n.parent.childCount && mf([...n.parent.child(l).marks], e, t);) a += n.parent.child(l).nodeSize, l += 1;
     return {
-        from: s,
+        from: o,
         to: a
     }
 }
 
-function zt(n, e) {
+function rt(n, e) {
     if (typeof n == "string") {
         if (!e.marks[n]) throw Error(`There is no mark type named '${n}'. Maybe you forgot to add the extension?`);
         return e.marks[n]
     }
     return n
 }
-var Jh = (n, e = {}) => ({
+var gf = (n, e = {}) => ({
         tr: t,
         state: r,
         dispatch: i
     }) => {
-        let o = zt(n, r.schema),
+        let s = rt(n, r.schema),
             {
-                doc: s,
+                doc: o,
                 selection: l
             } = t,
             {
                 $from: a,
                 from: c,
                 to: u
             } = l;
         if (i) {
-            let d = Ts(a, o, e);
+            let d = us(a, s, e);
             if (d && d.from <= c && d.to >= u) {
-                let f = P.create(s, d.from, d.to);
+                let f = I.create(o, d.from, d.to);
                 t.setSelection(f)
             }
         }
         return !0
     },
-    Kh = n => e => {
+    yf = n => e => {
         let t = typeof n == "function" ? n(e) : n;
         for (let r = 0; r < t.length; r += 1)
             if (t[r](e)) return !0;
         return !1
     };
 
-function iu(n) {
-    return n instanceof P
+function pa(n) {
+    return n instanceof I
 }
 
-function gn(n = 0, e = 0, t = 0) {
+function Ot(n = 0, e = 0, t = 0) {
     return Math.min(Math.max(n, e), t)
 }
 
-function ou(n, e = null) {
+function ma(n, e = null) {
     if (!e) return null;
-    let t = R.atStart(n),
-        r = R.atEnd(n);
+    let t = L.atStart(n),
+        r = L.atEnd(n);
     if (e === "start" || e === !0) return t;
     if (e === "end") return r;
     let i = t.from,
-        o = r.to;
-    return e === "all" ? P.create(n, gn(0, i, o), gn(n.content.size, i, o)) : P.create(n, gn(e, i, o), gn(e, i, o))
+        s = r.to;
+    return e === "all" ? I.create(n, Ot(0, i, s), Ot(n.content.size, i, s)) : I.create(n, Ot(e, i, s), Ot(e, i, s))
 }
 
-function Cs() {
+function ds() {
     return ["iPad Simulator", "iPhone Simulator", "iPod Simulator", "iPad", "iPhone", "iPod"].includes(navigator.platform) || navigator.userAgent.includes("Mac") && "ontouchend" in document
 }
-var Uh = (n = null, e = {}) => ({
+var bf = (n = null, e = {}) => ({
         editor: t,
         view: r,
         tr: i,
-        dispatch: o
+        dispatch: s
     }) => {
         e = {
             scrollIntoView: !0,
             ...e
         };
-        let s = () => {
-            Cs() && r.dom.focus(), requestAnimationFrame(() => {
+        let o = () => {
+            ds() && r.dom.focus(), requestAnimationFrame(() => {
                 t.isDestroyed || (r.focus(), e != null && e.scrollIntoView && t.commands.scrollIntoView())
             })
         };
         if (r.hasFocus() && n === null || n === !1) return !0;
-        if (o && n === null && !iu(t.state.selection)) return s(), !0;
-        let l = ou(i.doc, n) || t.state.selection,
+        if (s && n === null && !pa(t.state.selection)) return o(), !0;
+        let l = ma(i.doc, n) || t.state.selection,
             a = t.state.selection.eq(l);
-        return o && (a || i.setSelection(l), a && i.storedMarks && i.setStoredMarks(i.storedMarks), s()), !0
+        return s && (a || i.setSelection(l), a && i.storedMarks && i.setStoredMarks(i.storedMarks), o()), !0
     },
-    _h = (n, e) => t => n.every((r, i) => e(r, {
+    xf = (n, e) => t => n.every((r, i) => e(r, {
         ...t,
         index: i
     })),
-    Gh = (n, e) => ({
+    kf = (n, e) => ({
         tr: t,
         commands: r
     }) => r.insertContentAt({
         from: t.selection.from,
         to: t.selection.to
     }, n, e);
 
-function Yc(n) {
+function oa(n) {
     let e = `<body>${n}</body>`;
     return new window.DOMParser().parseFromString(e, "text/html").body
 }
 
-function ui(n, e, t) {
+function dr(n, e, t) {
     if (t = {
             slice: !0,
             parseOptions: {},
             ...t
         }, typeof n == "object" && n !== null) try {
-        return Array.isArray(n) && n.length > 0 ? v.fromArray(n.map(r => e.nodeFromJSON(r))) : e.nodeFromJSON(n)
+        return Array.isArray(n) && n.length > 0 ? x.fromArray(n.map(r => e.nodeFromJSON(r))) : e.nodeFromJSON(n)
     } catch (r) {
-        return console.warn("[tiptap warn]: Invalid content.", "Passed value:", n, "Error:", r), ui("", e, t)
+        return console.warn("[tiptap warn]: Invalid content.", "Passed value:", n, "Error:", r), dr("", e, t)
     }
     if (typeof n == "string") {
-        let r = Qe.fromSchema(e);
-        return t.slice ? r.parseSlice(Yc(n), t.parseOptions).content : r.parse(Yc(n), t.parseOptions)
+        let r = Te.fromSchema(e);
+        return t.slice ? r.parseSlice(oa(n), t.parseOptions).content : r.parse(oa(n), t.parseOptions)
     }
-    return ui("", e, t)
+    return dr("", e, t)
 }
 
-function Yh(n, e, t) {
+function Mf(n, e, t) {
     let r = n.steps.length - 1;
     if (r < e) return;
     let i = n.steps[r];
-    if (!(i instanceof Q || i instanceof W)) return;
-    let o = n.mapping.maps[r],
-        s = 0;
-    o.forEach((l, a, c, u) => {
-        s === 0 && (s = u)
-    }), n.setSelection(R.near(n.doc.resolve(s), t))
+    if (!(i instanceof q || i instanceof j)) return;
+    let s = n.mapping.maps[r],
+        o = 0;
+    s.forEach((l, a, c, u) => {
+        o === 0 && (o = u)
+    }), n.setSelection(L.near(n.doc.resolve(o), t))
 }
-var Qh = n => n.toString().startsWith("<"),
-    Xh = (n, e, t) => ({
+var Sf = n => n.toString().startsWith("<"),
+    Ef = (n, e, t) => ({
         tr: r,
         dispatch: i,
-        editor: o
+        editor: s
     }) => {
         if (i) {
             t = {
                 parseOptions: {},
                 updateSelection: !0,
                 ...t
             };
-            let s = ui(e, o.schema, {
+            let o = dr(e, s.schema, {
                 parseOptions: {
                     preserveWhitespace: "full",
                     ...t.parseOptions
                 }
             });
-            if (s.toString() === "<>") return !0;
+            if (o.toString() === "<>") return !0;
             let {
                 from: l,
                 to: a
             } = typeof n == "number" ? {
                 from: n,
                 to: n
             } : n, c = !0, u = !0;
-            if ((Qh(s) ? s : [s]).forEach(f => {
+            if ((Sf(o) ? o : [o]).forEach(f => {
                     f.check(), c = c ? f.isText && f.marks.length === 0 : !1, u = u ? f.isBlock : !1
                 }), l === a && u) {
                 let {
                     parent: f
                 } = r.doc.resolve(l);
                 f.isTextblock && !f.type.spec.code && !f.childCount && (l -= 1, a += 1)
             }
-            c ? Array.isArray(e) ? r.insertText(e.map(f => f.text || "").join(""), l, a) : typeof e == "object" && e && e.text ? r.insertText(e.text, l, a) : r.insertText(e, l, a) : r.replaceWith(l, a, s), t.updateSelection && Yh(r, r.steps.length - 1, -1)
+            c ? Array.isArray(e) ? r.insertText(e.map(f => f.text || "").join(""), l, a) : typeof e == "object" && e && e.text ? r.insertText(e.text, l, a) : r.insertText(e, l, a) : r.replaceWith(l, a, o), t.updateSelection && Mf(r, r.steps.length - 1, -1)
         }
         return !0
     },
-    Zh = () => ({
+    wf = () => ({
         state: n,
         dispatch: e
-    }) => zc(n, e),
-    em = () => ({
+    }) => Ul(n, e),
+    Tf = () => ({
         state: n,
         dispatch: e
-    }) => Hc(n, e),
-    tm = () => ({
+    }) => _l(n, e),
+    Cf = () => ({
         state: n,
         dispatch: e
-    }) => ts(n, e),
-    nm = () => ({
+    }) => Fi(n, e),
+    Af = () => ({
         state: n,
         dispatch: e
-    }) => rs(n, e);
+    }) => $i(n, e);
 
-function su() {
+function ga() {
     return typeof navigator < "u" ? /Mac/.test(navigator.platform) : !1
 }
 
-function rm(n) {
+function Of(n) {
     let e = n.split(/-(?!$)/),
         t = e[e.length - 1];
     t === "Space" && (t = " ");
-    let r, i, o, s;
+    let r, i, s, o;
     for (let l = 0; l < e.length - 1; l += 1) {
         let a = e[l];
-        if (/^(cmd|meta|m)$/i.test(a)) s = !0;
+        if (/^(cmd|meta|m)$/i.test(a)) o = !0;
         else if (/^a(lt)?$/i.test(a)) r = !0;
         else if (/^(c|ctrl|control)$/i.test(a)) i = !0;
-        else if (/^s(hift)?$/i.test(a)) o = !0;
-        else if (/^mod$/i.test(a)) Cs() || su() ? s = !0 : i = !0;
+        else if (/^s(hift)?$/i.test(a)) s = !0;
+        else if (/^mod$/i.test(a)) ds() || ga() ? o = !0 : i = !0;
         else throw new Error(`Unrecognized modifier name: ${a}`)
     }
-    return r && (t = `Alt-${t}`), i && (t = `Ctrl-${t}`), s && (t = `Meta-${t}`), o && (t = `Shift-${t}`), t
+    return r && (t = `Alt-${t}`), i && (t = `Ctrl-${t}`), o && (t = `Meta-${t}`), s && (t = `Shift-${t}`), t
 }
-var im = n => ({
+var vf = n => ({
     editor: e,
     view: t,
     tr: r,
     dispatch: i
 }) => {
-    let o = rm(n).split(/-(?!$)/),
-        s = o.find(c => !["Alt", "Ctrl", "Meta", "Shift"].includes(c)),
+    let s = Of(n).split(/-(?!$)/),
+        o = s.find(c => !["Alt", "Ctrl", "Meta", "Shift"].includes(c)),
         l = new KeyboardEvent("keydown", {
-            key: s === "Space" ? " " : s,
-            altKey: o.includes("Alt"),
-            ctrlKey: o.includes("Ctrl"),
-            metaKey: o.includes("Meta"),
-            shiftKey: o.includes("Shift"),
+            key: o === "Space" ? " " : o,
+            altKey: s.includes("Alt"),
+            ctrlKey: s.includes("Ctrl"),
+            metaKey: s.includes("Meta"),
+            shiftKey: s.includes("Shift"),
             bubbles: !0,
             cancelable: !0
         }),
         a = e.captureTransaction(() => {
             t.someProp("handleKeyDown", c => c(t, l))
         });
     return a == null || a.steps.forEach(c => {
         let u = c.map(r.mapping);
         u && i && r.maybeStep(u)
     }), !0
 };
 
-function Er(n, e, t = {}) {
+function Tn(n, e, t = {}) {
     let {
         from: r,
         to: i,
-        empty: o
-    } = n.selection, s = e ? ce(e, n.schema) : null, l = [];
+        empty: s
+    } = n.selection, o = e ? Y(e, n.schema) : null, l = [];
     n.doc.nodesBetween(r, i, (d, f) => {
         if (d.isText) return;
-        let p = Math.max(r, f),
-            h = Math.min(i, f + d.nodeSize);
+        let h = Math.max(r, f),
+            p = Math.min(i, f + d.nodeSize);
         l.push({
             node: d,
-            from: p,
-            to: h
+            from: h,
+            to: p
         })
     });
     let a = i - r,
-        c = l.filter(d => s ? s.name === d.node.type.name : !0).filter(d => ci(d.node.attrs, t, {
+        c = l.filter(d => o ? o.name === d.node.type.name : !0).filter(d => ur(d.node.attrs, t, {
             strict: !1
         }));
-    return o ? !!c.length : c.reduce((d, f) => d + f.to - f.from, 0) >= a
+    return s ? !!c.length : c.reduce((d, f) => d + f.to - f.from, 0) >= a
 }
-var om = (n, e = {}) => ({
+var Nf = (n, e = {}) => ({
         state: t,
         dispatch: r
     }) => {
-        let i = ce(n, t.schema);
-        return Er(t, i, e) ? Fc(t, r) : !1
+        let i = Y(n, t.schema);
+        return Tn(t, i, e) ? Gl(t, r) : !1
     },
-    sm = () => ({
+    If = () => ({
         state: n,
         dispatch: e
-    }) => us(n, e),
-    lm = n => ({
+    }) => Ui(n, e),
+    Df = n => ({
         state: e,
         dispatch: t
     }) => {
-        let r = ce(n, e.schema);
-        return Jc(r)(e, t)
+        let r = Y(n, e.schema);
+        return ta(r)(e, t)
     },
-    am = () => ({
+    Lf = () => ({
         state: n,
         dispatch: e
-    }) => ss(n, e);
+    }) => Ji(n, e);
 
-function mi(n, e) {
+function gr(n, e) {
     return e.nodes[n] ? "node" : e.marks[n] ? "mark" : null
 }
 
-function Qc(n, e) {
+function la(n, e) {
     let t = typeof e == "string" ? [e] : e;
     return Object.keys(n).reduce((r, i) => (t.includes(i) || (r[i] = n[i]), r), {})
 }
-var cm = (n, e) => ({
+var Rf = (n, e) => ({
         tr: t,
         state: r,
         dispatch: i
     }) => {
-        let o = null,
-            s = null,
-            l = mi(typeof n == "string" ? n : n.name, r.schema);
-        return l ? (l === "node" && (o = ce(n, r.schema)), l === "mark" && (s = zt(n, r.schema)), i && t.selection.ranges.forEach(a => {
+        let s = null,
+            o = null,
+            l = gr(typeof n == "string" ? n : n.name, r.schema);
+        return l ? (l === "node" && (s = Y(n, r.schema)), l === "mark" && (o = rt(n, r.schema)), i && t.selection.ranges.forEach(a => {
             r.doc.nodesBetween(a.$from.pos, a.$to.pos, (c, u) => {
-                o && o === c.type && t.setNodeMarkup(u, void 0, Qc(c.attrs, e)), s && c.marks.length && c.marks.forEach(d => {
-                    s === d.type && t.addMark(u, u + c.nodeSize, s.create(Qc(d.attrs, e)))
+                s && s === c.type && t.setNodeMarkup(u, void 0, la(c.attrs, e)), o && c.marks.length && c.marks.forEach(d => {
+                    o === d.type && t.addMark(u, u + c.nodeSize, o.create(la(d.attrs, e)))
                 })
             })
         }), !0) : !1
     },
-    um = () => ({
+    Pf = () => ({
         tr: n,
         dispatch: e
     }) => (e && n.scrollIntoView(), !0),
-    dm = () => ({
+    Bf = () => ({
         tr: n,
         commands: e
     }) => e.setTextSelection({
         from: 0,
         to: n.doc.content.size
     }),
-    fm = () => ({
+    zf = () => ({
         state: n,
         dispatch: e
-    }) => ns(n, e),
-    pm = () => ({
+    }) => ji(n, e),
+    Hf = () => ({
         state: n,
         dispatch: e
-    }) => is(n, e),
-    hm = () => ({
+    }) => Vi(n, e),
+    Ff = () => ({
         state: n,
         dispatch: e
-    }) => jc(n, e),
-    mm = () => ({
+    }) => Ql(n, e),
+    jf = () => ({
         state: n,
         dispatch: e
-    }) => fs(n, e),
-    gm = () => ({
+    }) => Gi(n, e),
+    $f = () => ({
         state: n,
         dispatch: e
-    }) => ds(n, e);
+    }) => _i(n, e);
 
-function lu(n, e, t = {}) {
-    return ui(n, e, {
+function ya(n, e, t = {}) {
+    return dr(n, e, {
         slice: !1,
         parseOptions: t
     })
 }
-var ym = (n, e = !1, t = {}) => ({
+var Vf = (n, e = !1, t = {}) => ({
     tr: r,
     editor: i,
-    dispatch: o
+    dispatch: s
 }) => {
     let {
-        doc: s
-    } = r, l = lu(n, i.schema, t);
-    return o && r.replaceWith(0, s.content.size, l).setMeta("preventUpdate", !e), !0
+        doc: o
+    } = r, l = ya(n, i.schema, t);
+    return s && r.replaceWith(0, o.content.size, l).setMeta("preventUpdate", !e), !0
 };
 
-function au(n, e) {
-    let t = new In(n);
+function ba(n, e) {
+    let t = new Ht(n);
     return e.forEach(r => {
         r.steps.forEach(i => {
             t.step(i)
         })
     }), t
 }
 
-function xm(n) {
+function Jf(n) {
     for (let e = 0; e < n.edgeCount; e += 1) {
         let {
             type: t
         } = n.edge(e);
         if (t.isTextblock && !t.hasRequiredAttrs()) return t
     }
     return null
 }
 
-function cu(n, e, t) {
+function xa(n, e, t) {
     let r = [];
-    return n.nodesBetween(e.from, e.to, (i, o) => {
+    return n.nodesBetween(e.from, e.to, (i, s) => {
         t(i) && r.push({
             node: i,
-            pos: o
+            pos: s
         })
     }), r
 }
 
-function bm(n, e) {
+function Wf(n, e) {
     for (let t = n.depth; t > 0; t -= 1) {
         let r = n.node(t);
         if (e(r)) return {
             pos: t > 0 ? n.before(t) : 0,
             start: n.start(t),
             depth: t,
             node: r
         }
     }
 }
 
-function Os(n) {
-    return e => bm(e.$from, n)
+function fs(n) {
+    return e => Wf(e.$from, n)
 }
 
-function km(n, e) {
-    let t = Se.fromSchema(e).serializeFragment(n),
+function qf(n, e) {
+    let t = ce.fromSchema(e).serializeFragment(n),
         i = document.implementation.createHTMLDocument().createElement("div");
     return i.appendChild(t), i.innerHTML
 }
 
-function vm(n, e) {
+function Kf(n, e) {
     let t = {
         from: 0,
         to: n.content.size
     };
-    return nu(n, t, e)
+    return fa(n, t, e)
 }
 
-function qn(n, e) {
-    let t = zt(e, n.schema),
+function Yt(n, e) {
+    let t = rt(e, n.schema),
         {
             from: r,
             to: i,
-            empty: o
+            empty: s
         } = n.selection,
-        s = [];
-    o ? (n.storedMarks && s.push(...n.storedMarks), s.push(...n.selection.$head.marks())) : n.doc.nodesBetween(r, i, a => {
-        s.push(...a.marks)
+        o = [];
+    s ? (n.storedMarks && o.push(...n.storedMarks), o.push(...n.selection.$head.marks())) : n.doc.nodesBetween(r, i, a => {
+        o.push(...a.marks)
     });
-    let l = s.find(a => a.type.name === t.name);
+    let l = o.find(a => a.type.name === t.name);
     return l ? {
         ...l.attrs
     } : {}
 }
 
-function Mm(n, e) {
-    let t = ce(e, n.schema),
+function Uf(n, e) {
+    let t = Y(e, n.schema),
         {
             from: r,
             to: i
         } = n.selection,
-        o = [];
+        s = [];
     n.doc.nodesBetween(r, i, l => {
-        o.push(l)
+        s.push(l)
     });
-    let s = o.reverse().find(l => l.type.name === t.name);
-    return s ? {
-        ...s.attrs
+    let o = s.reverse().find(l => l.type.name === t.name);
+    return o ? {
+        ...o.attrs
     } : {}
 }
 
-function As(n, e) {
-    let t = mi(typeof e == "string" ? e : e.name, n.schema);
-    return t === "node" ? Mm(n, e) : t === "mark" ? qn(n, e) : {}
+function hs(n, e) {
+    let t = gr(typeof e == "string" ? e : e.name, n.schema);
+    return t === "node" ? Uf(n, e) : t === "mark" ? Yt(n, e) : {}
 }
 
-function Em(n, e = JSON.stringify) {
+function _f(n, e = JSON.stringify) {
     let t = {};
     return n.filter(r => {
         let i = e(r);
         return Object.prototype.hasOwnProperty.call(t, i) ? !1 : t[i] = !0
     })
 }
 
-function Sm(n) {
-    let e = Em(n);
-    return e.length === 1 ? e : e.filter((t, r) => !e.filter((o, s) => s !== r).some(o => t.oldRange.from >= o.oldRange.from && t.oldRange.to <= o.oldRange.to && t.newRange.from >= o.newRange.from && t.newRange.to <= o.newRange.to))
+function Gf(n) {
+    let e = _f(n);
+    return e.length === 1 ? e : e.filter((t, r) => !e.filter((s, o) => o !== r).some(s => t.oldRange.from >= s.oldRange.from && t.oldRange.to <= s.oldRange.to && t.newRange.from >= s.newRange.from && t.newRange.to <= s.newRange.to))
 }
 
-function uu(n) {
+function ka(n) {
     let {
         mapping: e,
         steps: t
     } = n, r = [];
-    return e.maps.forEach((i, o) => {
-        let s = [];
+    return e.maps.forEach((i, s) => {
+        let o = [];
         if (i.ranges.length) i.forEach((l, a) => {
-            s.push({
+            o.push({
                 from: l,
                 to: a
             })
         });
         else {
             let {
                 from: l,
                 to: a
-            } = t[o];
+            } = t[s];
             if (l === void 0 || a === void 0) return;
-            s.push({
+            o.push({
                 from: l,
                 to: a
             })
         }
-        s.forEach(({
+        o.forEach(({
             from: l,
             to: a
         }) => {
-            let c = e.slice(o).map(l, -1),
-                u = e.slice(o).map(a),
+            let c = e.slice(s).map(l, -1),
+                u = e.slice(s).map(a),
                 d = e.invert().map(c, -1),
                 f = e.invert().map(u);
             r.push({
                 oldRange: {
                     from: d,
                     to: f
                 },
                 newRange: {
                     from: c,
                     to: u
                 }
             })
         })
-    }), Sm(r)
+    }), Gf(r)
 }
 
-function Sr(n, e, t) {
+function Cn(n, e, t) {
     let r = [];
     return n === e ? t.resolve(n).marks().forEach(i => {
-        let o = t.resolve(n - 1),
-            s = Ts(o, i.type);
-        s && r.push({
+        let s = t.resolve(n - 1),
+            o = us(s, i.type);
+        o && r.push({
             mark: i,
-            ...s
+            ...o
         })
-    }) : t.nodesBetween(n, e, (i, o) => {
-        r.push(...i.marks.map(s => ({
-            from: o,
-            to: o + i.nodeSize,
-            mark: s
+    }) : t.nodesBetween(n, e, (i, s) => {
+        r.push(...i.marks.map(o => ({
+            from: s,
+            to: s + i.nodeSize,
+            mark: o
         })))
     }), r
 }
 
-function ai(n, e, t) {
+function cr(n, e, t) {
     return Object.fromEntries(Object.entries(t).filter(([r]) => {
-        let i = n.find(o => o.type === e && o.name === r);
+        let i = n.find(s => s.type === e && s.name === r);
         return i ? i.attribute.keepOnSplit : !1
     }))
 }
 
-function Ss(n, e, t = {}) {
+function as(n, e, t = {}) {
     let {
         empty: r,
         ranges: i
-    } = n.selection, o = e ? zt(e, n.schema) : null;
-    if (r) return !!(n.storedMarks || n.selection.$from.marks()).filter(d => o ? o.name === d.type.name : !0).find(d => ci(d.attrs, t, {
+    } = n.selection, s = e ? rt(e, n.schema) : null;
+    if (r) return !!(n.storedMarks || n.selection.$from.marks()).filter(d => s ? s.name === d.type.name : !0).find(d => ur(d.attrs, t, {
         strict: !1
     }));
-    let s = 0,
+    let o = 0,
         l = [];
     if (i.forEach(({
             $from: d,
             $to: f
         }) => {
-            let p = d.pos,
-                h = f.pos;
-            n.doc.nodesBetween(p, h, (m, b) => {
+            let h = d.pos,
+                p = f.pos;
+            n.doc.nodesBetween(h, p, (m, b) => {
                 if (!m.isText && !m.marks.length) return;
-                let k = Math.max(p, b),
-                    S = Math.min(h, b + m.nodeSize),
-                    C = S - k;
-                s += C, l.push(...m.marks.map(T => ({
-                    mark: T,
-                    from: k,
-                    to: S
+                let M = Math.max(h, b),
+                    w = Math.min(p, b + m.nodeSize),
+                    v = w - M;
+                o += v, l.push(...m.marks.map(D => ({
+                    mark: D,
+                    from: M,
+                    to: w
                 })))
             })
-        }), s === 0) return !1;
-    let a = l.filter(d => o ? o.name === d.mark.type.name : !0).filter(d => ci(d.mark.attrs, t, {
+        }), o === 0) return !1;
+    let a = l.filter(d => s ? s.name === d.mark.type.name : !0).filter(d => ur(d.mark.attrs, t, {
             strict: !1
         })).reduce((d, f) => d + f.to - f.from, 0),
-        c = l.filter(d => o ? d.mark.type !== o && d.mark.type.excludes(o) : !0).reduce((d, f) => d + f.to - f.from, 0);
-    return (a > 0 ? a + c : a) >= s
+        c = l.filter(d => s ? d.mark.type !== s && d.mark.type.excludes(s) : !0).reduce((d, f) => d + f.to - f.from, 0);
+    return (a > 0 ? a + c : a) >= o
 }
 
-function wm(n, e, t = {}) {
-    if (!e) return Er(n, null, t) || Ss(n, null, t);
-    let r = mi(e, n.schema);
-    return r === "node" ? Er(n, e, t) : r === "mark" ? Ss(n, e, t) : !1
+function Qf(n, e, t = {}) {
+    if (!e) return Tn(n, null, t) || as(n, null, t);
+    let r = gr(e, n.schema);
+    return r === "node" ? Tn(n, e, t) : r === "mark" ? as(n, e, t) : !1
 }
 
-function Xc(n, e) {
+function aa(n, e) {
     let {
         nodeExtensions: t
-    } = pi(e), r = t.find(s => s.name === n);
+    } = pr(e), r = t.find(o => o.name === n);
     if (!r) return !1;
     let i = {
             name: r.name,
             options: r.options,
             storage: r.storage
         },
-        o = B(A(r, "group", i));
-    return typeof o != "string" ? !1 : o.split(" ").includes("list")
+        s = R(T(r, "group", i));
+    return typeof s != "string" ? !1 : s.split(" ").includes("list")
 }
 
-function Tm(n) {
+function Yf(n) {
     var e;
     let t = (e = n.type.createAndFill()) === null || e === void 0 ? void 0 : e.toJSON(),
         r = n.toJSON();
     return JSON.stringify(t) === JSON.stringify(r)
 }
 
-function Cm(n, e, t) {
+function Xf(n, e, t) {
     var r;
     let {
         selection: i
-    } = e, o = null;
-    if (iu(i) && (o = i.$cursor), o) {
-        let l = (r = n.storedMarks) !== null && r !== void 0 ? r : o.marks();
+    } = e, s = null;
+    if (pa(i) && (s = i.$cursor), s) {
+        let l = (r = n.storedMarks) !== null && r !== void 0 ? r : s.marks();
         return !!t.isInSet(l) || !l.some(a => a.type.excludes(t))
     }
     let {
-        ranges: s
+        ranges: o
     } = i;
-    return s.some(({
+    return o.some(({
         $from: l,
         $to: a
     }) => {
         let c = l.depth === 0 ? n.doc.inlineContent && n.doc.type.allowsMarkType(t) : !1;
         return n.doc.nodesBetween(l.pos, a.pos, (u, d, f) => {
             if (c) return !1;
             if (u.isInline) {
-                let p = !f || f.type.allowsMarkType(t),
-                    h = !!t.isInSet(u.marks) || !u.marks.some(m => m.type.excludes(t));
-                c = p && h
+                let h = !f || f.type.allowsMarkType(t),
+                    p = !!t.isInSet(u.marks) || !u.marks.some(m => m.type.excludes(t));
+                c = h && p
             }
             return !c
         }), c
     })
 }
-var Om = (n, e = {}) => ({
+var Zf = (n, e = {}) => ({
         tr: t,
         state: r,
         dispatch: i
     }) => {
         let {
-            selection: o
+            selection: s
         } = t, {
-            empty: s,
+            empty: o,
             ranges: l
-        } = o, a = zt(n, r.schema);
+        } = s, a = rt(n, r.schema);
         if (i)
-            if (s) {
-                let c = qn(r, a);
+            if (o) {
+                let c = Yt(r, a);
                 t.addStoredMark(a.create({
                     ...c,
                     ...e
                 }))
             } else l.forEach(c => {
                 let u = c.$from.pos,
                     d = c.$to.pos;
-                r.doc.nodesBetween(u, d, (f, p) => {
-                    let h = Math.max(p, u),
-                        m = Math.min(p + f.nodeSize, d);
-                    f.marks.find(k => k.type === a) ? f.marks.forEach(k => {
-                        a === k.type && t.addMark(h, m, a.create({
-                            ...k.attrs,
+                r.doc.nodesBetween(u, d, (f, h) => {
+                    let p = Math.max(h, u),
+                        m = Math.min(h + f.nodeSize, d);
+                    f.marks.find(M => M.type === a) ? f.marks.forEach(M => {
+                        a === M.type && t.addMark(p, m, a.create({
+                            ...M.attrs,
                             ...e
                         }))
-                    }) : t.addMark(h, m, a.create(e))
+                    }) : t.addMark(p, m, a.create(e))
                 })
             });
-        return Cm(r, t, a)
+        return Xf(r, t, a)
     },
-    Am = (n, e) => ({
+    eh = (n, e) => ({
         tr: t
     }) => (t.setMeta(n, e), !0),
-    Nm = (n, e = {}) => ({
+    th = (n, e = {}) => ({
         state: t,
         dispatch: r,
         chain: i
     }) => {
-        let o = ce(n, t.schema);
-        return o.isTextblock ? i().command(({
-            commands: s
-        }) => ps(o, e)(t) ? !0 : s.clearNodes()).command(({
-            state: s
-        }) => ps(o, e)(s, r)).run() : (console.warn('[tiptap warn]: Currently "setNode()" only supports text block nodes.'), !1)
+        let s = Y(n, t.schema);
+        return s.isTextblock ? i().command(({
+            commands: o
+        }) => Qi(s, e)(t) ? !0 : o.clearNodes()).command(({
+            state: o
+        }) => Qi(s, e)(o, r)).run() : (console.warn('[tiptap warn]: Currently "setNode()" only supports text block nodes.'), !1)
     },
-    Im = n => ({
+    nh = n => ({
         tr: e,
         dispatch: t
     }) => {
         if (t) {
             let {
                 doc: r
-            } = e, i = gn(n, 0, r.content.size), o = D.create(r, i);
-            e.setSelection(o)
+            } = e, i = Ot(n, 0, r.content.size), s = O.create(r, i);
+            e.setSelection(s)
         }
         return !0
     },
-    Dm = n => ({
+    rh = n => ({
         tr: e,
         dispatch: t
     }) => {
         if (t) {
             let {
                 doc: r
             } = e, {
                 from: i,
-                to: o
+                to: s
             } = typeof n == "number" ? {
                 from: n,
                 to: n
-            } : n, s = P.atStart(r).from, l = P.atEnd(r).to, a = gn(i, s, l), c = gn(o, s, l), u = P.create(r, a, c);
+            } : n, o = I.atStart(r).from, l = I.atEnd(r).to, a = Ot(i, o, l), c = Ot(s, o, l), u = I.create(r, a, c);
             e.setSelection(u)
         }
         return !0
     },
-    Lm = n => ({
+    ih = n => ({
         state: e,
         dispatch: t
     }) => {
-        let r = ce(n, e.schema);
-        return Kc(r)(e, t)
+        let r = Y(n, e.schema);
+        return na(r)(e, t)
     };
 
-function Zc(n, e) {
+function ca(n, e) {
     let t = n.storedMarks || n.selection.$to.parentOffset && n.selection.$from.marks();
     if (t) {
         let r = t.filter(i => e == null ? void 0 : e.includes(i.type.name));
         n.tr.ensureMarks(r)
     }
 }
-var Pm = ({
+var sh = ({
         keepMarks: n = !0
     } = {}) => ({
         tr: e,
         state: t,
         dispatch: r,
         editor: i
     }) => {
         let {
-            selection: o,
-            doc: s
+            selection: s,
+            doc: o
         } = e, {
             $from: l,
             $to: a
-        } = o, c = i.extensionManager.attributes, u = ai(c, l.node().type.name, l.node().attrs);
-        if (o instanceof D && o.node.isBlock) return !l.parentOffset || !ze(s, l.pos) ? !1 : (r && (n && Zc(t, i.extensionManager.splittableMarks), e.split(l.pos).scrollIntoView()), !0);
+        } = s, c = i.extensionManager.attributes, u = cr(c, l.node().type.name, l.node().attrs);
+        if (s instanceof O && s.node.isBlock) return !l.parentOffset || !ge(o, l.pos) ? !1 : (r && (n && ca(t, i.extensionManager.splittableMarks), e.split(l.pos).scrollIntoView()), !0);
         if (!l.parent.isBlock) return !1;
         if (r) {
             let d = a.parentOffset === a.parent.content.size;
-            o instanceof P && e.deleteSelection();
-            let f = l.depth === 0 ? void 0 : xm(l.node(-1).contentMatchAt(l.indexAfter(-1))),
-                p = d && f ? [{
+            s instanceof I && e.deleteSelection();
+            let f = l.depth === 0 ? void 0 : Jf(l.node(-1).contentMatchAt(l.indexAfter(-1))),
+                h = d && f ? [{
                     type: f,
                     attrs: u
                 }] : void 0,
-                h = ze(e.doc, e.mapping.map(l.pos), 1, p);
-            if (!p && !h && ze(e.doc, e.mapping.map(l.pos), 1, f ? [{
+                p = ge(e.doc, e.mapping.map(l.pos), 1, h);
+            if (!h && !p && ge(e.doc, e.mapping.map(l.pos), 1, f ? [{
                     type: f
-                }] : void 0) && (h = !0, p = f ? [{
+                }] : void 0) && (p = !0, h = f ? [{
                     type: f,
                     attrs: u
-                }] : void 0), h && (e.split(e.mapping.map(l.pos), 1, p), f && !d && !l.parentOffset && l.parent.type !== f)) {
+                }] : void 0), p && (e.split(e.mapping.map(l.pos), 1, h), f && !d && !l.parentOffset && l.parent.type !== f)) {
                 let m = e.mapping.map(l.before()),
                     b = e.doc.resolve(m);
                 l.node(-1).canReplaceWith(b.index(), b.index() + 1, f) && e.setNodeMarkup(e.mapping.map(l.before()), f)
             }
-            n && Zc(t, i.extensionManager.splittableMarks), e.scrollIntoView()
+            n && ca(t, i.extensionManager.splittableMarks), e.scrollIntoView()
         }
         return !0
     },
-    Rm = n => ({
+    oh = n => ({
         tr: e,
         state: t,
         dispatch: r,
         editor: i
     }) => {
-        var o;
-        let s = ce(n, t.schema),
+        var s;
+        let o = Y(n, t.schema),
             {
                 $from: l,
                 $to: a
             } = t.selection,
             c = t.selection.node;
         if (c && c.isBlock || l.depth < 2 || !l.sameParent(a)) return !1;
         let u = l.node(-1);
-        if (u.type !== s) return !1;
+        if (u.type !== o) return !1;
         let d = i.extensionManager.attributes;
         if (l.parent.content.size === 0 && l.node(-1).childCount === l.indexAfter(-1)) {
-            if (l.depth === 2 || l.node(-3).type !== s || l.index(-2) !== l.node(-2).childCount - 1) return !1;
+            if (l.depth === 2 || l.node(-3).type !== o || l.index(-2) !== l.node(-2).childCount - 1) return !1;
             if (r) {
-                let b = v.empty,
-                    k = l.index(-1) ? 1 : l.index(-2) ? 2 : 3;
-                for (let x = l.depth - k; x >= l.depth - 3; x -= 1) b = v.from(l.node(x).copy(b));
-                let S = l.indexAfter(-1) < l.node(-2).childCount ? 1 : l.indexAfter(-2) < l.node(-3).childCount ? 2 : 3,
-                    C = ai(d, l.node().type.name, l.node().attrs),
-                    T = ((o = s.contentMatch.defaultType) === null || o === void 0 ? void 0 : o.createAndFill(C)) || void 0;
-                b = b.append(v.from(s.createAndFill(null, T) || void 0));
-                let E = l.before(l.depth - (k - 1));
-                e.replace(E, l.after(-S), new w(b, 4 - k, 0));
+                let b = x.empty,
+                    M = l.index(-1) ? 1 : l.index(-2) ? 2 : 3;
+                for (let k = l.depth - M; k >= l.depth - 3; k -= 1) b = x.from(l.node(k).copy(b));
+                let w = l.indexAfter(-1) < l.node(-2).childCount ? 1 : l.indexAfter(-2) < l.node(-3).childCount ? 2 : 3,
+                    v = cr(d, l.node().type.name, l.node().attrs),
+                    D = ((s = o.contentMatch.defaultType) === null || s === void 0 ? void 0 : s.createAndFill(v)) || void 0;
+                b = b.append(x.from(o.createAndFill(null, D) || void 0));
+                let A = l.before(l.depth - (M - 1));
+                e.replace(A, l.after(-w), new E(b, 4 - M, 0));
                 let g = -1;
-                e.doc.nodesBetween(E, e.doc.content.size, (x, y) => {
+                e.doc.nodesBetween(A, e.doc.content.size, (k, y) => {
                     if (g > -1) return !1;
-                    x.isTextblock && x.content.size === 0 && (g = y + 1)
-                }), g > -1 && e.setSelection(P.near(e.doc.resolve(g))), e.scrollIntoView()
+                    k.isTextblock && k.content.size === 0 && (g = y + 1)
+                }), g > -1 && e.setSelection(I.near(e.doc.resolve(g))), e.scrollIntoView()
             }
             return !0
         }
         let f = a.pos === l.end() ? u.contentMatchAt(0).defaultType : null,
-            p = ai(d, u.type.name, u.attrs),
-            h = ai(d, l.node().type.name, l.node().attrs);
+            h = cr(d, u.type.name, u.attrs),
+            p = cr(d, l.node().type.name, l.node().attrs);
         e.delete(l.pos, a.pos);
         let m = f ? [{
-            type: s,
-            attrs: p
+            type: o,
+            attrs: h
         }, {
             type: f,
-            attrs: h
-        }] : [{
-            type: s,
             attrs: p
+        }] : [{
+            type: o,
+            attrs: h
         }];
-        if (!ze(e.doc, l.pos, 2)) return !1;
+        if (!ge(e.doc, l.pos, 2)) return !1;
         if (r) {
             let {
                 selection: b,
-                storedMarks: k
+                storedMarks: M
             } = t, {
-                splittableMarks: S
-            } = i.extensionManager, C = k || b.$to.parentOffset && b.$from.marks();
-            if (e.split(l.pos, 2, m).scrollIntoView(), !C || !r) return !0;
-            let T = C.filter(E => S.includes(E.type.name));
-            e.ensureMarks(T)
+                splittableMarks: w
+            } = i.extensionManager, v = M || b.$to.parentOffset && b.$from.marks();
+            if (e.split(l.pos, 2, m).scrollIntoView(), !v || !r) return !0;
+            let D = v.filter(A => w.includes(A.type.name));
+            e.ensureMarks(D)
         }
         return !0
     },
-    xs = (n, e) => {
-        let t = Os(s => s.type === e)(n.selection);
+    ts = (n, e) => {
+        let t = fs(o => o.type === e)(n.selection);
         if (!t) return !0;
         let r = n.doc.resolve(Math.max(0, t.pos - 1)).before(t.depth);
         if (r === void 0) return !0;
         let i = n.doc.nodeAt(r);
-        return t.node.type === (i == null ? void 0 : i.type) && Ke(n.doc, t.pos) && n.join(t.pos), !0
+        return t.node.type === (i == null ? void 0 : i.type) && Se(n.doc, t.pos) && n.join(t.pos), !0
     },
-    bs = (n, e) => {
-        let t = Os(s => s.type === e)(n.selection);
+    ns = (n, e) => {
+        let t = fs(o => o.type === e)(n.selection);
         if (!t) return !0;
         let r = n.doc.resolve(t.start).after(t.depth);
         if (r === void 0) return !0;
         let i = n.doc.nodeAt(r);
-        return t.node.type === (i == null ? void 0 : i.type) && Ke(n.doc, r) && n.join(r), !0
+        return t.node.type === (i == null ? void 0 : i.type) && Se(n.doc, r) && n.join(r), !0
     },
-    Bm = (n, e, t, r = {}) => ({
+    lh = (n, e, t, r = {}) => ({
         editor: i,
-        tr: o,
-        state: s,
+        tr: s,
+        state: o,
         dispatch: l,
         chain: a,
         commands: c,
         can: u
     }) => {
         let {
             extensions: d,
             splittableMarks: f
-        } = i.extensionManager, p = ce(n, s.schema), h = ce(e, s.schema), {
+        } = i.extensionManager, h = Y(n, o.schema), p = Y(e, o.schema), {
             selection: m,
             storedMarks: b
-        } = s, {
-            $from: k,
-            $to: S
-        } = m, C = k.blockRange(S), T = b || m.$to.parentOffset && m.$from.marks();
-        if (!C) return !1;
-        let E = Os(g => Xc(g.type.name, d))(m);
-        if (C.depth >= 1 && E && C.depth - E.depth <= 1) {
-            if (E.node.type === p) return c.liftListItem(h);
-            if (Xc(E.node.type.name, d) && p.validContent(E.node.content) && l) return a().command(() => (o.setNodeMarkup(E.pos, p), !0)).command(() => xs(o, p)).command(() => bs(o, p)).run()
-        }
-        return !t || !T || !l ? a().command(() => u().wrapInList(p, r) ? !0 : c.clearNodes()).wrapInList(p, r).command(() => xs(o, p)).command(() => bs(o, p)).run() : a().command(() => {
-            let g = u().wrapInList(p, r),
-                x = T.filter(y => f.includes(y.type.name));
-            return o.ensureMarks(x), g ? !0 : c.clearNodes()
-        }).wrapInList(p, r).command(() => xs(o, p)).command(() => bs(o, p)).run()
+        } = o, {
+            $from: M,
+            $to: w
+        } = m, v = M.blockRange(w), D = b || m.$to.parentOffset && m.$from.marks();
+        if (!v) return !1;
+        let A = fs(g => aa(g.type.name, d))(m);
+        if (v.depth >= 1 && A && v.depth - A.depth <= 1) {
+            if (A.node.type === h) return c.liftListItem(p);
+            if (aa(A.node.type.name, d) && h.validContent(A.node.content) && l) return a().command(() => (s.setNodeMarkup(A.pos, h), !0)).command(() => ts(s, h)).command(() => ns(s, h)).run()
+        }
+        return !t || !D || !l ? a().command(() => u().wrapInList(h, r) ? !0 : c.clearNodes()).wrapInList(h, r).command(() => ts(s, h)).command(() => ns(s, h)).run() : a().command(() => {
+            let g = u().wrapInList(h, r),
+                k = D.filter(y => f.includes(y.type.name));
+            return s.ensureMarks(k), g ? !0 : c.clearNodes()
+        }).wrapInList(h, r).command(() => ts(s, h)).command(() => ns(s, h)).run()
     },
-    zm = (n, e = {}, t = {}) => ({
+    ah = (n, e = {}, t = {}) => ({
         state: r,
         commands: i
     }) => {
         let {
-            extendEmptyMarkRange: o = !1
-        } = t, s = zt(n, r.schema);
-        return Ss(r, s, e) ? i.unsetMark(s, {
-            extendEmptyMarkRange: o
-        }) : i.setMark(s, e)
+            extendEmptyMarkRange: s = !1
+        } = t, o = rt(n, r.schema);
+        return as(r, o, e) ? i.unsetMark(o, {
+            extendEmptyMarkRange: s
+        }) : i.setMark(o, e)
     },
-    Hm = (n, e, t = {}) => ({
+    ch = (n, e, t = {}) => ({
         state: r,
         commands: i
     }) => {
-        let o = ce(n, r.schema),
-            s = ce(e, r.schema);
-        return Er(r, o, t) ? i.setNode(s) : i.setNode(o, t)
+        let s = Y(n, r.schema),
+            o = Y(e, r.schema);
+        return Tn(r, s, t) ? i.setNode(o) : i.setNode(s, t)
     },
-    Fm = (n, e = {}) => ({
+    uh = (n, e = {}) => ({
         state: t,
         commands: r
     }) => {
-        let i = ce(n, t.schema);
-        return Er(t, i, e) ? r.lift(i) : r.wrapIn(i, e)
+        let i = Y(n, t.schema);
+        return Tn(t, i, e) ? r.lift(i) : r.wrapIn(i, e)
     },
-    jm = () => ({
+    dh = () => ({
         state: n,
         dispatch: e
     }) => {
         let t = n.plugins;
         for (let r = 0; r < t.length; r += 1) {
             let i = t[r],
-                o;
-            if (i.spec.isInputRules && (o = i.getState(n))) {
+                s;
+            if (i.spec.isInputRules && (s = i.getState(n))) {
                 if (e) {
-                    let s = n.tr,
-                        l = o.transform;
-                    for (let a = l.steps.length - 1; a >= 0; a -= 1) s.step(l.steps[a].invert(l.docs[a]));
-                    if (o.text) {
-                        let a = s.doc.resolve(o.from).marks();
-                        s.replaceWith(o.from, o.to, n.schema.text(o.text, a))
-                    } else s.delete(o.from, o.to)
+                    let o = n.tr,
+                        l = s.transform;
+                    for (let a = l.steps.length - 1; a >= 0; a -= 1) o.step(l.steps[a].invert(l.docs[a]));
+                    if (s.text) {
+                        let a = o.doc.resolve(s.from).marks();
+                        o.replaceWith(s.from, s.to, n.schema.text(s.text, a))
+                    } else o.delete(s.from, s.to)
                 }
                 return !0
             }
         }
         return !1
     },
-    Vm = () => ({
+    fh = () => ({
         tr: n,
         dispatch: e
     }) => {
         let {
             selection: t
         } = n, {
             empty: r,
             ranges: i
         } = t;
-        return r || e && i.forEach(o => {
-            n.removeMark(o.$from.pos, o.$to.pos)
+        return r || e && i.forEach(s => {
+            n.removeMark(s.$from.pos, s.$to.pos)
         }), !0
     },
-    $m = (n, e = {}) => ({
+    hh = (n, e = {}) => ({
         tr: t,
         state: r,
         dispatch: i
     }) => {
-        var o;
+        var s;
         let {
-            extendEmptyMarkRange: s = !1
+            extendEmptyMarkRange: o = !1
         } = e, {
             selection: l
-        } = t, a = zt(n, r.schema), {
+        } = t, a = rt(n, r.schema), {
             $from: c,
             empty: u,
             ranges: d
         } = l;
         if (!i) return !0;
-        if (u && s) {
+        if (u && o) {
             let {
                 from: f,
-                to: p
-            } = l, h = (o = c.marks().find(b => b.type === a)) === null || o === void 0 ? void 0 : o.attrs, m = Ts(c, a, h);
-            m && (f = m.from, p = m.to), t.removeMark(f, p, a)
+                to: h
+            } = l, p = (s = c.marks().find(b => b.type === a)) === null || s === void 0 ? void 0 : s.attrs, m = us(c, a, p);
+            m && (f = m.from, h = m.to), t.removeMark(f, h, a)
         } else d.forEach(f => {
             t.removeMark(f.$from.pos, f.$to.pos, a)
         });
         return t.removeStoredMark(a), !0
     },
-    Wm = (n, e = {}) => ({
+    ph = (n, e = {}) => ({
         tr: t,
         state: r,
         dispatch: i
     }) => {
-        let o = null,
-            s = null,
-            l = mi(typeof n == "string" ? n : n.name, r.schema);
-        return l ? (l === "node" && (o = ce(n, r.schema)), l === "mark" && (s = zt(n, r.schema)), i && t.selection.ranges.forEach(a => {
+        let s = null,
+            o = null,
+            l = gr(typeof n == "string" ? n : n.name, r.schema);
+        return l ? (l === "node" && (s = Y(n, r.schema)), l === "mark" && (o = rt(n, r.schema)), i && t.selection.ranges.forEach(a => {
             let c = a.$from.pos,
                 u = a.$to.pos;
             r.doc.nodesBetween(c, u, (d, f) => {
-                o && o === d.type && t.setNodeMarkup(f, void 0, {
+                s && s === d.type && t.setNodeMarkup(f, void 0, {
                     ...d.attrs,
                     ...e
-                }), s && d.marks.length && d.marks.forEach(p => {
-                    if (s === p.type) {
-                        let h = Math.max(f, c),
+                }), o && d.marks.length && d.marks.forEach(h => {
+                    if (o === h.type) {
+                        let p = Math.max(f, c),
                             m = Math.min(f + d.nodeSize, u);
-                        t.addMark(h, m, s.create({
-                            ...p.attrs,
+                        t.addMark(p, m, o.create({
+                            ...h.attrs,
                             ...e
                         }))
                     }
                 })
             })
         }), !0) : !1
     },
-    qm = (n, e = {}) => ({
+    mh = (n, e = {}) => ({
         state: t,
         dispatch: r
     }) => {
-        let i = ce(n, t.schema);
-        return Wc(i, e)(t, r)
+        let i = Y(n, t.schema);
+        return Zl(i, e)(t, r)
     },
-    Jm = (n, e = {}) => ({
+    gh = (n, e = {}) => ({
         state: t,
         dispatch: r
     }) => {
-        let i = ce(n, t.schema);
-        return qc(i, e)(t, r)
+        let i = Y(n, t.schema);
+        return ea(i, e)(t, r)
     },
-    Km = Object.freeze({
+    yh = Object.freeze({
         __proto__: null,
-        blur: Lh,
-        clearContent: Ph,
-        clearNodes: Rh,
-        command: Bh,
-        createParagraphNear: zh,
-        deleteCurrentNode: Hh,
-        deleteNode: Fh,
-        deleteRange: jh,
-        deleteSelection: Vh,
-        enter: $h,
-        exitCode: Wh,
-        extendMarkRange: Jh,
-        first: Kh,
-        focus: Uh,
-        forEach: _h,
-        insertContent: Gh,
-        insertContentAt: Xh,
-        joinUp: Zh,
-        joinDown: em,
-        joinBackward: tm,
-        joinForward: nm,
-        keyboardShortcut: im,
-        lift: om,
-        liftEmptyBlock: sm,
-        liftListItem: lm,
-        newlineInCode: am,
-        resetAttributes: cm,
-        scrollIntoView: um,
-        selectAll: dm,
-        selectNodeBackward: fm,
-        selectNodeForward: pm,
-        selectParentNode: hm,
-        selectTextblockEnd: mm,
-        selectTextblockStart: gm,
-        setContent: ym,
-        setMark: Om,
-        setMeta: Am,
-        setNode: Nm,
-        setNodeSelection: Im,
-        setTextSelection: Dm,
-        sinkListItem: Lm,
-        splitBlock: Pm,
-        splitListItem: Rm,
-        toggleList: Bm,
-        toggleMark: zm,
-        toggleNode: Hm,
-        toggleWrap: Fm,
-        undoInputRule: jm,
-        unsetAllMarks: Vm,
-        unsetMark: $m,
-        updateAttributes: Wm,
-        wrapIn: qm,
-        wrapInList: Jm
+        blur: rf,
+        clearContent: sf,
+        clearNodes: of,
+        command: lf,
+        createParagraphNear: af,
+        deleteCurrentNode: cf,
+        deleteNode: uf,
+        deleteRange: df,
+        deleteSelection: ff,
+        enter: hf,
+        exitCode: pf,
+        extendMarkRange: gf,
+        first: yf,
+        focus: bf,
+        forEach: xf,
+        insertContent: kf,
+        insertContentAt: Ef,
+        joinUp: wf,
+        joinDown: Tf,
+        joinBackward: Cf,
+        joinForward: Af,
+        keyboardShortcut: vf,
+        lift: Nf,
+        liftEmptyBlock: If,
+        liftListItem: Df,
+        newlineInCode: Lf,
+        resetAttributes: Rf,
+        scrollIntoView: Pf,
+        selectAll: Bf,
+        selectNodeBackward: zf,
+        selectNodeForward: Hf,
+        selectParentNode: Ff,
+        selectTextblockEnd: jf,
+        selectTextblockStart: $f,
+        setContent: Vf,
+        setMark: Zf,
+        setMeta: eh,
+        setNode: th,
+        setNodeSelection: nh,
+        setTextSelection: rh,
+        sinkListItem: ih,
+        splitBlock: sh,
+        splitListItem: oh,
+        toggleList: lh,
+        toggleMark: ah,
+        toggleNode: ch,
+        toggleWrap: uh,
+        undoInputRule: dh,
+        unsetAllMarks: fh,
+        unsetMark: hh,
+        updateAttributes: ph,
+        wrapIn: mh,
+        wrapInList: gh
     }),
-    Um = J.create({
+    bh = V.create({
         name: "commands",
         addCommands() {
             return {
-                ...Km
+                ...yh
             }
         }
     }),
-    _m = J.create({
+    xh = V.create({
         name: "editable",
         addProseMirrorPlugins() {
-            return [new q({
-                key: new Z("editable"),
+            return [new $({
+                key: new U("editable"),
                 props: {
                     editable: () => this.editor.options.editable
                 }
             })]
         }
     }),
-    Gm = J.create({
+    kh = V.create({
         name: "focusEvents",
         addProseMirrorPlugins() {
             let {
                 editor: n
             } = this;
-            return [new q({
-                key: new Z("focusEvents"),
+            return [new $({
+                key: new U("focusEvents"),
                 props: {
                     handleDOMEvents: {
                         focus: (e, t) => {
                             n.isFocused = !0;
                             let r = n.state.tr.setMeta("focus", {
                                 event: t
                             }).setMeta("addToHistory", !1);
@@ -11366,115 +10136,115 @@
                             return e.dispatch(r), !1
                         }
                     }
                 }
             })]
         }
     }),
-    Ym = J.create({
+    Mh = V.create({
         name: "keymap",
         addKeyboardShortcuts() {
             let n = () => this.editor.commands.first(({
-                    commands: s
-                }) => [() => s.undoInputRule(), () => s.command(({
+                    commands: o
+                }) => [() => o.undoInputRule(), () => o.command(({
                     tr: l
                 }) => {
                     let {
                         selection: a,
                         doc: c
                     } = l, {
                         empty: u,
                         $anchor: d
                     } = a, {
                         pos: f,
-                        parent: p
-                    } = d, h = R.atStart(c).from === f;
-                    return !u || !h || !p.type.isTextblock || p.textContent.length ? !1 : s.clearNodes()
-                }), () => s.deleteSelection(), () => s.joinBackward(), () => s.selectNodeBackward()]),
+                        parent: h
+                    } = d, p = L.atStart(c).from === f;
+                    return !u || !p || !h.type.isTextblock || h.textContent.length ? !1 : o.clearNodes()
+                }), () => o.deleteSelection(), () => o.joinBackward(), () => o.selectNodeBackward()]),
                 e = () => this.editor.commands.first(({
-                    commands: s
-                }) => [() => s.deleteSelection(), () => s.deleteCurrentNode(), () => s.joinForward(), () => s.selectNodeForward()]),
+                    commands: o
+                }) => [() => o.deleteSelection(), () => o.deleteCurrentNode(), () => o.joinForward(), () => o.selectNodeForward()]),
                 r = {
                     Enter: () => this.editor.commands.first(({
-                        commands: s
-                    }) => [() => s.newlineInCode(), () => s.createParagraphNear(), () => s.liftEmptyBlock(), () => s.splitBlock()]),
+                        commands: o
+                    }) => [() => o.newlineInCode(), () => o.createParagraphNear(), () => o.liftEmptyBlock(), () => o.splitBlock()]),
                     "Mod-Enter": () => this.editor.commands.exitCode(),
                     Backspace: n,
                     "Mod-Backspace": n,
                     "Shift-Backspace": n,
                     Delete: e,
                     "Mod-Delete": e,
                     "Mod-a": () => this.editor.commands.selectAll()
                 },
                 i = {
                     ...r
                 },
-                o = {
+                s = {
                     ...r,
                     "Ctrl-h": n,
                     "Alt-Backspace": n,
                     "Ctrl-d": e,
                     "Ctrl-Alt-Backspace": e,
                     "Alt-Delete": e,
                     "Alt-d": e,
                     "Ctrl-a": () => this.editor.commands.selectTextblockStart(),
                     "Ctrl-e": () => this.editor.commands.selectTextblockEnd()
                 };
-            return Cs() || su() ? o : i
+            return ds() || ga() ? s : i
         },
         addProseMirrorPlugins() {
-            return [new q({
-                key: new Z("clearDocument"),
+            return [new $({
+                key: new U("clearDocument"),
                 appendTransaction: (n, e, t) => {
-                    if (!(n.some(h => h.docChanged) && !e.doc.eq(t.doc))) return;
+                    if (!(n.some(p => p.docChanged) && !e.doc.eq(t.doc))) return;
                     let {
                         empty: i,
-                        from: o,
-                        to: s
-                    } = e.selection, l = R.atStart(e.doc).from, a = R.atEnd(e.doc).to;
-                    if (i || !(o === l && s === a) || !(t.doc.textBetween(0, t.doc.content.size, " ", " ").length === 0)) return;
+                        from: s,
+                        to: o
+                    } = e.selection, l = L.atStart(e.doc).from, a = L.atEnd(e.doc).to;
+                    if (i || !(s === l && o === a) || !(t.doc.textBetween(0, t.doc.content.size, " ", " ").length === 0)) return;
                     let d = t.tr,
-                        f = fi({
+                        f = hr({
                             state: t,
                             transaction: d
                         }),
                         {
-                            commands: p
-                        } = new $n({
+                            commands: h
+                        } = new Gt({
                             editor: this.editor,
                             state: f
                         });
-                    if (p.clearNodes(), !!d.steps.length) return d
+                    if (h.clearNodes(), !!d.steps.length) return d
                 }
             })]
         }
     }),
-    Qm = J.create({
+    Sh = V.create({
         name: "tabindex",
         addProseMirrorPlugins() {
-            return [new q({
-                key: new Z("tabindex"),
+            return [new $({
+                key: new U("tabindex"),
                 props: {
                     attributes: this.editor.isEditable ? {
                         tabindex: "0"
                     } : {}
                 }
             })]
         }
     }),
-    Xm = Object.freeze({
+    Eh = Object.freeze({
         __proto__: null,
-        ClipboardTextSerializer: Dh,
-        Commands: Um,
-        Editable: _m,
-        FocusEvents: Gm,
-        Keymap: Ym,
-        Tabindex: Qm
+        ClipboardTextSerializer: nf,
+        Commands: bh,
+        Editable: xh,
+        FocusEvents: kh,
+        Keymap: Mh,
+        Tabindex: Sh
     }),
-    Zm = `.ProseMirror {
+    wh = `.ProseMirror {
   position: relative;
 }
 
 .ProseMirror {
   word-wrap: break-word;
   white-space: pre-wrap;
   white-space: break-spaces;
@@ -11542,21 +10312,21 @@
   display: block;
 }
 
 .tippy-box[data-animation=fade][data-state=hidden] {
   opacity: 0
 }`;
 
-function eg(n, e) {
+function Th(n, e) {
     let t = document.querySelector("style[data-tiptap-style]");
     if (t !== null) return t;
     let r = document.createElement("style");
     return e && r.setAttribute("nonce", e), r.setAttribute("data-tiptap-style", ""), r.innerHTML = n, document.getElementsByTagName("head")[0].appendChild(r), r
 }
-var di = class extends ks {
+var fr = class extends rs {
     constructor(e = {}) {
         super(), this.isFocused = !1, this.extensionStorage = {}, this.options = {
             element: document.createElement("div"),
             content: "",
             injectCSS: !0,
             injectNonce: void 0,
             extensions: [],
@@ -11592,15 +10362,15 @@
     chain() {
         return this.commandManager.chain()
     }
     can() {
         return this.commandManager.can()
     }
     injectCSS() {
-        this.options.injectCSS && document && (this.css = eg(Zm, this.options.injectNonce))
+        this.options.injectCSS && document && (this.css = Th(wh, this.options.injectNonce))
     }
     setOptions(e = {}) {
         this.options = {
             ...this.options,
             ...e
         }, !(!this.view || !this.state || this.isDestroyed) && (this.options.editorProps && this.view.setProps(this.options.editorProps), this.view.updateState(this.state))
     }
@@ -11615,47 +10385,47 @@
     get isEditable() {
         return this.options.editable && this.view && this.view.editable
     }
     get state() {
         return this.view.state
     }
     registerPlugin(e, t) {
-        let r = tu(t) ? t(e, [...this.state.plugins]) : [...this.state.plugins, e],
+        let r = da(t) ? t(e, [...this.state.plugins]) : [...this.state.plugins, e],
             i = this.state.reconfigure({
                 plugins: r
             });
         this.view.updateState(i)
     }
     unregisterPlugin(e) {
         if (this.isDestroyed) return;
         let t = typeof e == "string" ? `${e}$` : e.key,
             r = this.state.reconfigure({
                 plugins: this.state.plugins.filter(i => !i.key.startsWith(t))
             });
         this.view.updateState(r)
     }
     createExtensionManager() {
-        let t = [...this.options.enableCoreExtensions ? Object.values(Xm) : [], ...this.options.extensions].filter(r => ["extension", "node", "mark"].includes(r == null ? void 0 : r.type));
-        this.extensionManager = new Bt(t, this)
+        let t = [...this.options.enableCoreExtensions ? Object.values(Eh) : [], ...this.options.extensions].filter(r => ["extension", "node", "mark"].includes(r == null ? void 0 : r.type));
+        this.extensionManager = new nt(t, this)
     }
     createCommandManager() {
-        this.commandManager = new $n({
+        this.commandManager = new Gt({
             editor: this
         })
     }
     createSchema() {
         this.schema = this.extensionManager.schema
     }
     createView() {
-        let e = lu(this.options.content, this.schema, this.options.parseOptions),
-            t = ou(e, this.options.autofocus);
-        this.view = new ti(this.options.element, {
+        let e = ya(this.options.content, this.schema, this.options.parseOptions),
+            t = ma(e, this.options.autofocus);
+        this.view = new nr(this.options.element, {
             ...this.options.editorProps,
             dispatchTransaction: this.dispatchTransaction.bind(this),
-            state: yt.create({
+            state: $e.create({
                 doc: e,
                 selection: t || void 0
             })
         });
         let r = this.state.reconfigure({
             plugins: this.extensionManager.plugins
         });
@@ -11676,299 +10446,299 @@
     dispatchTransaction(e) {
         if (this.view.isDestroyed) return;
         if (this.isCapturingTransaction) {
             if (!this.capturedTransaction) {
                 this.capturedTransaction = e;
                 return
             }
-            e.steps.forEach(s => {
+            e.steps.forEach(o => {
                 var l;
-                return (l = this.capturedTransaction) === null || l === void 0 ? void 0 : l.step(s)
+                return (l = this.capturedTransaction) === null || l === void 0 ? void 0 : l.step(o)
             });
             return
         }
         let t = this.state.apply(e),
             r = !this.state.selection.eq(t.selection);
         this.view.updateState(t), this.emit("transaction", {
             editor: this,
             transaction: e
         }), r && this.emit("selectionUpdate", {
             editor: this,
             transaction: e
         });
         let i = e.getMeta("focus"),
-            o = e.getMeta("blur");
+            s = e.getMeta("blur");
         i && this.emit("focus", {
             editor: this,
             event: i.event,
             transaction: e
-        }), o && this.emit("blur", {
+        }), s && this.emit("blur", {
             editor: this,
-            event: o.event,
+            event: s.event,
             transaction: e
         }), !(!e.docChanged || e.getMeta("preventUpdate")) && this.emit("update", {
             editor: this,
             transaction: e
         })
     }
     getAttributes(e) {
-        return As(this.state, e)
+        return hs(this.state, e)
     }
     isActive(e, t) {
         let r = typeof e == "string" ? e : null,
             i = typeof e == "string" ? t : e;
-        return wm(this.state, r, i)
+        return Qf(this.state, r, i)
     }
     getJSON() {
         return this.state.doc.toJSON()
     }
     getHTML() {
-        return km(this.state.doc.content, this.schema)
+        return qf(this.state.doc.content, this.schema)
     }
     getText(e) {
         let {
             blockSeparator: t = `
 
 `,
             textSerializers: r = {}
         } = e || {};
-        return vm(this.state.doc, {
+        return Kf(this.state.doc, {
             blockSeparator: t,
             textSerializers: {
-                ...ru(this.schema),
+                ...ha(this.schema),
                 ...r
             }
         })
     }
     get isEmpty() {
-        return Tm(this.state.doc)
+        return Yf(this.state.doc)
     }
     getCharacterCount() {
         return console.warn('[tiptap warn]: "editor.getCharacterCount()" is deprecated. Please use "editor.storage.characterCount.characters()" instead.'), this.state.doc.content.size - 2
     }
     destroy() {
         this.emit("destroy"), this.view && this.view.destroy(), this.removeAllListeners()
     }
     get isDestroyed() {
         var e;
         return !(!((e = this.view) === null || e === void 0) && e.docView)
     }
 };
 
-function Jn(n) {
-    return new Wn({
+function Xt(n) {
+    return new Qt({
         find: n.find,
         handler: ({
             state: e,
             range: t,
             match: r
         }) => {
-            let i = B(n.getAttributes, void 0, r);
+            let i = R(n.getAttributes, void 0, r);
             if (i === !1 || i === null) return null;
             let {
-                tr: o
-            } = e, s = r[r.length - 1], l = r[0], a = t.to;
-            if (s) {
+                tr: s
+            } = e, o = r[r.length - 1], l = r[0], a = t.to;
+            if (o) {
                 let c = l.search(/\S/),
-                    u = t.from + l.indexOf(s),
-                    d = u + s.length;
-                if (Sr(t.from, t.to, e.doc).filter(p => p.mark.type.excluded.find(m => m === n.type && m !== p.mark.type)).filter(p => p.to > u).length) return null;
-                d < t.to && o.delete(d, t.to), u > t.from && o.delete(t.from + c, u), a = t.from + c + s.length, o.addMark(t.from + c, a, n.type.create(i || {})), o.removeStoredMark(n.type)
+                    u = t.from + l.indexOf(o),
+                    d = u + o.length;
+                if (Cn(t.from, t.to, e.doc).filter(h => h.mark.type.excluded.find(m => m === n.type && m !== h.mark.type)).filter(h => h.to > u).length) return null;
+                d < t.to && s.delete(d, t.to), u > t.from && s.delete(t.from + c, u), a = t.from + c + o.length, s.addMark(t.from + c, a, n.type.create(i || {})), s.removeStoredMark(n.type)
             }
         }
     })
 }
 
-function gi(n) {
-    return new Wn({
+function yr(n) {
+    return new Qt({
         find: n.find,
         handler: ({
             state: e,
             range: t,
             match: r
         }) => {
-            let i = B(n.getAttributes, void 0, r) || {},
+            let i = R(n.getAttributes, void 0, r) || {},
                 {
-                    tr: o
+                    tr: s
                 } = e,
-                s = t.from,
+                o = t.from,
                 l = t.to;
             if (r[1]) {
                 let a = r[0].lastIndexOf(r[1]),
-                    c = s + a;
+                    c = o + a;
                 c > l ? c = l : l = c + r[1].length;
                 let u = r[0][r[0].length - 1];
-                o.insertText(u, s + r[0].length - 1), o.replaceWith(c, l, n.type.create(i))
-            } else r[0] && o.replaceWith(s, l, n.type.create(i))
+                s.insertText(u, o + r[0].length - 1), s.replaceWith(c, l, n.type.create(i))
+            } else r[0] && s.replaceWith(o, l, n.type.create(i))
         }
     })
 }
 
-function wr(n) {
-    return new Wn({
+function An(n) {
+    return new Qt({
         find: n.find,
         handler: ({
             state: e,
             range: t,
             match: r
         }) => {
             let i = e.doc.resolve(t.from),
-                o = B(n.getAttributes, void 0, r) || {};
+                s = R(n.getAttributes, void 0, r) || {};
             if (!i.node(-1).canReplaceWith(i.index(-1), i.indexAfter(-1), n.type)) return null;
-            e.tr.delete(t.from, t.to).setBlockType(t.from, t.from, n.type, o)
+            e.tr.delete(t.from, t.to).setBlockType(t.from, t.from, n.type, s)
         }
     })
 }
 
-function Ht(n) {
-    return new Wn({
+function it(n) {
+    return new Qt({
         find: n.find,
         handler: ({
             state: e,
             range: t,
             match: r,
             chain: i
         }) => {
-            let o = B(n.getAttributes, void 0, r) || {},
-                s = e.tr.delete(t.from, t.to),
-                a = s.doc.resolve(t.from).blockRange(),
-                c = a && Dn(a, n.type, o);
+            let s = R(n.getAttributes, void 0, r) || {},
+                o = e.tr.delete(t.from, t.to),
+                a = o.doc.resolve(t.from).blockRange(),
+                c = a && Ft(a, n.type, s);
             if (!c) return null;
-            if (s.wrap(a, c), n.keepMarks && n.editor) {
+            if (o.wrap(a, c), n.keepMarks && n.editor) {
                 let {
                     selection: d,
                     storedMarks: f
                 } = e, {
-                    splittableMarks: p
-                } = n.editor.extensionManager, h = f || d.$to.parentOffset && d.$from.marks();
-                if (h) {
-                    let m = h.filter(b => p.includes(b.type.name));
-                    s.ensureMarks(m)
+                    splittableMarks: h
+                } = n.editor.extensionManager, p = f || d.$to.parentOffset && d.$from.marks();
+                if (p) {
+                    let m = p.filter(b => h.includes(b.type.name));
+                    o.ensureMarks(m)
                 }
             }
             if (n.keepAttributes) {
                 let d = n.type.name === "bulletList" || n.type.name === "orderedList" ? "listItem" : "taskList";
-                i().updateAttributes(d, o).run()
+                i().updateAttributes(d, s).run()
             }
-            let u = s.doc.resolve(t.from - 1).nodeBefore;
-            u && u.type === n.type && Ke(s.doc, t.from - 1) && (!n.joinPredicate || n.joinPredicate(r, u)) && s.join(t.from - 1)
+            let u = o.doc.resolve(t.from - 1).nodeBefore;
+            u && u.type === n.type && Se(o.doc, t.from - 1) && (!n.joinPredicate || n.joinPredicate(r, u)) && o.join(t.from - 1)
         }
     })
 }
-var V = class {
+var F = class {
         constructor(e = {}) {
             this.type = "mark", this.name = "mark", this.parent = null, this.child = null, this.config = {
                 name: this.name,
                 defaultOptions: {}
             }, this.config = {
                 ...this.config,
                 ...e
-            }, this.name = this.config.name, e.defaultOptions && console.warn(`[tiptap warn]: BREAKING CHANGE: "defaultOptions" is deprecated. Please use "addOptions" instead. Found in extension: "${this.name}".`), this.options = this.config.defaultOptions, this.config.addOptions && (this.options = B(A(this, "addOptions", {
+            }, this.name = this.config.name, e.defaultOptions && console.warn(`[tiptap warn]: BREAKING CHANGE: "defaultOptions" is deprecated. Please use "addOptions" instead. Found in extension: "${this.name}".`), this.options = this.config.defaultOptions, this.config.addOptions && (this.options = R(T(this, "addOptions", {
                 name: this.name
-            }))), this.storage = B(A(this, "addStorage", {
+            }))), this.storage = R(T(this, "addStorage", {
                 name: this.name,
                 options: this.options
             })) || {}
         }
         static create(e = {}) {
-            return new V(e)
+            return new F(e)
         }
         configure(e = {}) {
             let t = this.extend();
-            return t.options = hi(this.options, e), t.storage = B(A(t, "addStorage", {
+            return t.options = mr(this.options, e), t.storage = R(T(t, "addStorage", {
                 name: t.name,
                 options: t.options
             })), t
         }
         extend(e = {}) {
-            let t = new V(e);
-            return t.parent = this, this.child = t, t.name = e.name ? e.name : t.parent.name, e.defaultOptions && console.warn(`[tiptap warn]: BREAKING CHANGE: "defaultOptions" is deprecated. Please use "addOptions" instead. Found in extension: "${t.name}".`), t.options = B(A(t, "addOptions", {
+            let t = new F(e);
+            return t.parent = this, this.child = t, t.name = e.name ? e.name : t.parent.name, e.defaultOptions && console.warn(`[tiptap warn]: BREAKING CHANGE: "defaultOptions" is deprecated. Please use "addOptions" instead. Found in extension: "${t.name}".`), t.options = R(T(t, "addOptions", {
                 name: t.name
-            })), t.storage = B(A(t, "addStorage", {
+            })), t.storage = R(T(t, "addStorage", {
                 name: t.name,
                 options: t.options
             })), t
         }
         static handleExit({
             editor: e,
             mark: t
         }) {
             let {
                 tr: r
             } = e.state, i = e.state.selection.$from;
             if (i.pos === i.end()) {
-                let s = i.marks();
-                if (!!!s.find(c => (c == null ? void 0 : c.type.name) === t.name)) return !1;
-                let a = s.find(c => (c == null ? void 0 : c.type.name) === t.name);
+                let o = i.marks();
+                if (!!!o.find(c => (c == null ? void 0 : c.type.name) === t.name)) return !1;
+                let a = o.find(c => (c == null ? void 0 : c.type.name) === t.name);
                 return a && r.removeStoredMark(a), r.insertText(" ", i.pos), e.view.dispatch(r), !0
             }
             return !1
         }
     },
-    F = class {
+    H = class {
         constructor(e = {}) {
             this.type = "node", this.name = "node", this.parent = null, this.child = null, this.config = {
                 name: this.name,
                 defaultOptions: {}
             }, this.config = {
                 ...this.config,
                 ...e
-            }, this.name = this.config.name, e.defaultOptions && console.warn(`[tiptap warn]: BREAKING CHANGE: "defaultOptions" is deprecated. Please use "addOptions" instead. Found in extension: "${this.name}".`), this.options = this.config.defaultOptions, this.config.addOptions && (this.options = B(A(this, "addOptions", {
+            }, this.name = this.config.name, e.defaultOptions && console.warn(`[tiptap warn]: BREAKING CHANGE: "defaultOptions" is deprecated. Please use "addOptions" instead. Found in extension: "${this.name}".`), this.options = this.config.defaultOptions, this.config.addOptions && (this.options = R(T(this, "addOptions", {
                 name: this.name
-            }))), this.storage = B(A(this, "addStorage", {
+            }))), this.storage = R(T(this, "addStorage", {
                 name: this.name,
                 options: this.options
             })) || {}
         }
         static create(e = {}) {
-            return new F(e)
+            return new H(e)
         }
         configure(e = {}) {
             let t = this.extend();
-            return t.options = hi(this.options, e), t.storage = B(A(t, "addStorage", {
+            return t.options = mr(this.options, e), t.storage = R(T(t, "addStorage", {
                 name: t.name,
                 options: t.options
             })), t
         }
         extend(e = {}) {
-            let t = new F(e);
-            return t.parent = this, this.child = t, t.name = e.name ? e.name : t.parent.name, e.defaultOptions && console.warn(`[tiptap warn]: BREAKING CHANGE: "defaultOptions" is deprecated. Please use "addOptions" instead. Found in extension: "${t.name}".`), t.options = B(A(t, "addOptions", {
+            let t = new H(e);
+            return t.parent = this, this.child = t, t.name = e.name ? e.name : t.parent.name, e.defaultOptions && console.warn(`[tiptap warn]: BREAKING CHANGE: "defaultOptions" is deprecated. Please use "addOptions" instead. Found in extension: "${t.name}".`), t.options = R(T(t, "addOptions", {
                 name: t.name
-            })), t.storage = B(A(t, "addStorage", {
+            })), t.storage = R(T(t, "addStorage", {
                 name: t.name,
                 options: t.options
             })), t
         }
     };
 
-function Ft(n) {
-    return new Ms({
+function st(n) {
+    return new ss({
         find: n.find,
         handler: ({
             state: e,
             range: t,
             match: r
         }) => {
-            let i = B(n.getAttributes, void 0, r);
+            let i = R(n.getAttributes, void 0, r);
             if (i === !1 || i === null) return null;
             let {
-                tr: o
-            } = e, s = r[r.length - 1], l = r[0], a = t.to;
-            if (s) {
+                tr: s
+            } = e, o = r[r.length - 1], l = r[0], a = t.to;
+            if (o) {
                 let c = l.search(/\S/),
-                    u = t.from + l.indexOf(s),
-                    d = u + s.length;
-                if (Sr(t.from, t.to, e.doc).filter(p => p.mark.type.excluded.find(m => m === n.type && m !== p.mark.type)).filter(p => p.to > u).length) return null;
-                d < t.to && o.delete(d, t.to), u > t.from && o.delete(t.from + c, u), a = t.from + c + s.length, o.addMark(t.from + c, a, n.type.create(i || {})), o.removeStoredMark(n.type)
+                    u = t.from + l.indexOf(o),
+                    d = u + o.length;
+                if (Cn(t.from, t.to, e.doc).filter(h => h.mark.type.excluded.find(m => m === n.type && m !== h.mark.type)).filter(h => h.to > u).length) return null;
+                d < t.to && s.delete(d, t.to), u > t.from && s.delete(t.from + c, u), a = t.from + c + o.length, s.addMark(t.from + c, a, n.type.create(i || {})), s.removeStoredMark(n.type)
             }
         }
     })
 }
-var tg = /^\s*>\s$/,
-    du = F.create({
+var Ch = /^\s*>\s$/,
+    Ma = H.create({
         name: "blockquote",
         addOptions() {
             return {
                 HTMLAttributes: {}
             }
         },
         content: "block+",
@@ -11978,15 +10748,15 @@
             return [{
                 tag: "blockquote"
             }]
         },
         renderHTML({
             HTMLAttributes: n
         }) {
-            return ["blockquote", z(this.options.HTMLAttributes, n), 0]
+            return ["blockquote", P(this.options.HTMLAttributes, n), 0]
         },
         addCommands() {
             return {
                 setBlockquote: () => ({
                     commands: n
                 }) => n.wrapIn(this.name),
                 toggleBlockquote: () => ({
@@ -11999,25 +10769,25 @@
         },
         addKeyboardShortcuts() {
             return {
                 "Mod-Shift-b": () => this.editor.commands.toggleBlockquote()
             }
         },
         addInputRules() {
-            return [Ht({
-                find: tg,
+            return [it({
+                find: Ch,
                 type: this.type
             })]
         }
     });
-var ng = /(?:^|\s)((?:\*\*)((?:[^*]+))(?:\*\*))$/,
-    rg = /(?:^|\s)((?:\*\*)((?:[^*]+))(?:\*\*))/g,
-    ig = /(?:^|\s)((?:__)((?:[^__]+))(?:__))$/,
-    og = /(?:^|\s)((?:__)((?:[^__]+))(?:__))/g,
-    fu = V.create({
+var Ah = /(?:^|\s)((?:\*\*)((?:[^*]+))(?:\*\*))$/,
+    Oh = /(?:^|\s)((?:\*\*)((?:[^*]+))(?:\*\*))/g,
+    vh = /(?:^|\s)((?:__)((?:[^__]+))(?:__))$/,
+    Nh = /(?:^|\s)((?:__)((?:[^__]+))(?:__))/g,
+    Sa = F.create({
         name: "bold",
         addOptions() {
             return {
                 HTMLAttributes: {}
             }
         },
         parseHTML() {
@@ -12030,15 +10800,15 @@
                 style: "font-weight",
                 getAttrs: n => /^(bold(er)?|[5-9]\d{2,})$/.test(n) && null
             }]
         },
         renderHTML({
             HTMLAttributes: n
         }) {
-            return ["strong", z(this.options.HTMLAttributes, n), 0]
+            return ["strong", P(this.options.HTMLAttributes, n), 0]
         },
         addCommands() {
             return {
                 setBold: () => ({
                     commands: n
                 }) => n.setMark(this.name),
                 toggleBold: () => ({
@@ -12052,33 +10822,33 @@
         addKeyboardShortcuts() {
             return {
                 "Mod-b": () => this.editor.commands.toggleBold(),
                 "Mod-B": () => this.editor.commands.toggleBold()
             }
         },
         addInputRules() {
-            return [Jn({
-                find: ng,
+            return [Xt({
+                find: Ah,
                 type: this.type
-            }), Jn({
-                find: ig,
+            }), Xt({
+                find: vh,
                 type: this.type
             })]
         },
         addPasteRules() {
-            return [Ft({
-                find: rg,
+            return [st({
+                find: Oh,
                 type: this.type
-            }), Ft({
-                find: og,
+            }), st({
+                find: Nh,
                 type: this.type
             })]
         }
     });
-var sg = F.create({
+var Ih = H.create({
         name: "listItem",
         addOptions() {
             return {
                 HTMLAttributes: {}
             }
         },
         content: "paragraph block*",
@@ -12087,25 +10857,25 @@
             return [{
                 tag: "li"
             }]
         },
         renderHTML({
             HTMLAttributes: n
         }) {
-            return ["li", z(this.options.HTMLAttributes, n), 0]
+            return ["li", P(this.options.HTMLAttributes, n), 0]
         },
         addKeyboardShortcuts() {
             return {
                 Enter: () => this.editor.commands.splitListItem(this.name),
                 Tab: () => this.editor.commands.sinkListItem(this.name),
                 "Shift-Tab": () => this.editor.commands.liftListItem(this.name)
             }
         }
     }),
-    pu = V.create({
+    Ea = F.create({
         name: "textStyle",
         addOptions() {
             return {
                 HTMLAttributes: {}
             }
         },
         parseHTML() {
@@ -12113,30 +10883,30 @@
                 tag: "span",
                 getAttrs: n => n.hasAttribute("style") ? {} : !1
             }]
         },
         renderHTML({
             HTMLAttributes: n
         }) {
-            return ["span", z(this.options.HTMLAttributes, n), 0]
+            return ["span", P(this.options.HTMLAttributes, n), 0]
         },
         addCommands() {
             return {
                 removeEmptyTextStyle: () => ({
                     state: n,
                     commands: e
                 }) => {
-                    let t = qn(n, this.type);
+                    let t = Yt(n, this.type);
                     return Object.entries(t).some(([, i]) => !!i) ? !0 : e.unsetMark(this.name)
                 }
             }
         }
     }),
-    hu = /^\s*([-+*])\s$/,
-    mu = F.create({
+    wa = /^\s*([-+*])\s$/,
+    Ta = H.create({
         name: "bulletList",
         addOptions() {
             return {
                 itemTypeName: "listItem",
                 HTMLAttributes: {},
                 keepMarks: !1,
                 keepAttributes: !1
@@ -12150,45 +10920,45 @@
             return [{
                 tag: "ul"
             }]
         },
         renderHTML({
             HTMLAttributes: n
         }) {
-            return ["ul", z(this.options.HTMLAttributes, n), 0]
+            return ["ul", P(this.options.HTMLAttributes, n), 0]
         },
         addCommands() {
             return {
                 toggleBulletList: () => ({
                     commands: n,
                     chain: e
-                }) => this.options.keepAttributes ? e().toggleList(this.name, this.options.itemTypeName, this.options.keepMarks).updateAttributes(sg.name, this.editor.getAttributes(pu.name)).run() : n.toggleList(this.name, this.options.itemTypeName, this.options.keepMarks)
+                }) => this.options.keepAttributes ? e().toggleList(this.name, this.options.itemTypeName, this.options.keepMarks).updateAttributes(Ih.name, this.editor.getAttributes(Ea.name)).run() : n.toggleList(this.name, this.options.itemTypeName, this.options.keepMarks)
             }
         },
         addKeyboardShortcuts() {
             return {
                 "Mod-Shift-8": () => this.editor.commands.toggleBulletList()
             }
         },
         addInputRules() {
-            let n = Ht({
-                find: hu,
+            let n = it({
+                find: wa,
                 type: this.type
             });
-            return (this.options.keepMarks || this.options.keepAttributes) && (n = Ht({
-                find: hu,
+            return (this.options.keepMarks || this.options.keepAttributes) && (n = it({
+                find: wa,
                 type: this.type,
                 keepMarks: this.options.keepMarks,
                 keepAttributes: this.options.keepAttributes,
-                getAttributes: () => this.editor.getAttributes(pu.name),
+                getAttributes: () => this.editor.getAttributes(Ea.name),
                 editor: this.editor
             })), [n]
         }
     });
-var gu = J.create({
+var Ca = V.create({
     name: "characterCount",
     addOptions() {
         return {
             limit: null,
             mode: "textSize"
         }
     },
@@ -12204,41 +10974,41 @@
             return ((n == null ? void 0 : n.mode) || this.options.mode) === "textSize" ? e.textBetween(0, e.content.size, void 0, " ").length : e.nodeSize
         }, this.storage.words = n => {
             let e = (n == null ? void 0 : n.node) || this.editor.state.doc;
             return e.textBetween(0, e.content.size, " ", " ").split(" ").filter(i => i !== "").length
         }
     },
     addProseMirrorPlugins() {
-        return [new q({
-            key: new Z("characterCount"),
+        return [new $({
+            key: new U("characterCount"),
             filterTransaction: (n, e) => {
                 let t = this.options.limit;
                 if (!n.docChanged || t === 0 || t === null || t === void 0) return !0;
                 let r = this.storage.characters({
                         node: e.doc
                     }),
                     i = this.storage.characters({
                         node: n.doc
                     });
                 if (i <= t || r > t && i > t && i <= r) return !0;
                 if (r > t && i > t && i > r || !n.getMeta("paste")) return !1;
-                let s = n.selection.$head.pos,
+                let o = n.selection.$head.pos,
                     l = i - t,
-                    a = s - l,
-                    c = s;
+                    a = o - l,
+                    c = o;
                 return n.deleteRange(a, c), !(this.storage.characters({
                     node: n.doc
                 }) > t)
             }
         })]
     }
 });
-var lg = /^```([a-z]+)?[\s\n]$/,
-    ag = /^~~~([a-z]+)?[\s\n]$/,
-    yu = F.create({
+var Dh = /^```([a-z]+)?[\s\n]$/,
+    Lh = /^~~~([a-z]+)?[\s\n]$/,
+    Aa = H.create({
         name: "codeBlock",
         addOptions() {
             return {
                 languageClassPrefix: "language-",
                 exitOnTripleEnter: !0,
                 exitOnArrowDown: !0,
                 HTMLAttributes: {}
@@ -12253,16 +11023,16 @@
             return {
                 language: {
                     default: null,
                     parseHTML: n => {
                         var e;
                         let {
                             languageClassPrefix: t
-                        } = this.options, o = [...((e = n.firstElementChild) === null || e === void 0 ? void 0 : e.classList) || []].filter(s => s.startsWith(t)).map(s => s.replace(t, ""))[0];
-                        return o || null
+                        } = this.options, s = [...((e = n.firstElementChild) === null || e === void 0 ? void 0 : e.classList) || []].filter(o => o.startsWith(t)).map(o => o.replace(t, ""))[0];
+                        return s || null
                     },
                     rendered: !1
                 }
             }
         },
         parseHTML() {
             return [{
@@ -12270,15 +11040,15 @@
                 preserveWhitespace: "full"
             }]
         },
         renderHTML({
             node: n,
             HTMLAttributes: e
         }) {
-            return ["pre", z(this.options.HTMLAttributes, e), ["code", {
+            return ["pre", P(this.options.HTMLAttributes, e), ["code", {
                 class: n.attrs.language ? this.options.languageClassPrefix + n.attrs.language : null
             }, 0]]
         },
         addCommands() {
             return {
                 setCodeBlock: n => ({
                     commands: e
@@ -12307,85 +11077,85 @@
                     } = n, {
                         selection: t
                     } = e, {
                         $from: r,
                         empty: i
                     } = t;
                     if (!i || r.parent.type !== this.type) return !1;
-                    let o = r.parentOffset === r.parent.nodeSize - 2,
-                        s = r.parent.textContent.endsWith(`
+                    let s = r.parentOffset === r.parent.nodeSize - 2,
+                        o = r.parent.textContent.endsWith(`
 
 `);
-                    return !o || !s ? !1 : n.chain().command(({
+                    return !s || !o ? !1 : n.chain().command(({
                         tr: l
                     }) => (l.delete(r.pos - 2, r.pos), !0)).exitCode().run()
                 },
                 ArrowDown: ({
                     editor: n
                 }) => {
                     if (!this.options.exitOnArrowDown) return !1;
                     let {
                         state: e
                     } = n, {
                         selection: t,
                         doc: r
                     } = e, {
                         $from: i,
-                        empty: o
+                        empty: s
                     } = t;
-                    if (!o || i.parent.type !== this.type || !(i.parentOffset === i.parent.nodeSize - 2)) return !1;
+                    if (!s || i.parent.type !== this.type || !(i.parentOffset === i.parent.nodeSize - 2)) return !1;
                     let l = i.after();
                     return l === void 0 || r.nodeAt(l) ? !1 : n.commands.exitCode()
                 }
             }
         },
         addInputRules() {
-            return [wr({
-                find: lg,
+            return [An({
+                find: Dh,
                 type: this.type,
                 getAttributes: n => ({
                     language: n[1]
                 })
-            }), wr({
-                find: ag,
+            }), An({
+                find: Lh,
                 type: this.type,
                 getAttributes: n => ({
                     language: n[1]
                 })
             })]
         },
         addProseMirrorPlugins() {
-            return [new q({
-                key: new Z("codeBlockVSCodeHandler"),
+            return [new $({
+                key: new U("codeBlockVSCodeHandler"),
                 props: {
                     handlePaste: (n, e) => {
                         if (!e.clipboardData || this.editor.isActive(this.type.name)) return !1;
                         let t = e.clipboardData.getData("text/plain"),
                             r = e.clipboardData.getData("vscode-editor-data"),
                             i = r ? JSON.parse(r) : void 0,
-                            o = i == null ? void 0 : i.mode;
-                        if (!t || !o) return !1;
+                            s = i == null ? void 0 : i.mode;
+                        if (!t || !s) return !1;
                         let {
-                            tr: s
+                            tr: o
                         } = n.state;
-                        return s.replaceSelectionWith(this.type.create({
-                            language: o
-                        })), s.setSelection(P.near(s.doc.resolve(Math.max(0, s.selection.from - 2)))), s.insertText(t.replace(/\r\n?/g, `
-`)), s.setMeta("paste", !0), n.dispatch(s), !0
+                        return o.replaceSelectionWith(this.type.create({
+                            language: s
+                        })), o.setSelection(I.near(o.doc.resolve(Math.max(0, o.selection.from - 2)))), o.insertText(t.replace(/\r\n?/g, `
+`)), o.setMeta("paste", !0), n.dispatch(o), !0
                     }
                 }
             })]
         }
     });
-var xu = F.create({
+var Oa = H.create({
     name: "doc",
     topNode: !0,
     content: "block+"
 });
-var bu = F.create({
+var va = H.create({
     name: "hardBreak",
     addOptions() {
         return {
             keepMarks: !0,
             HTMLAttributes: {}
         }
     },
@@ -12396,15 +11166,15 @@
         return [{
             tag: "br"
         }]
     },
     renderHTML({
         HTMLAttributes: n
     }) {
-        return ["br", z(this.options.HTMLAttributes, n)]
+        return ["br", P(this.options.HTMLAttributes, n)]
     },
     renderText() {
         return `
 `
     },
     addCommands() {
         return {
@@ -12412,29 +11182,29 @@
                 commands: n,
                 chain: e,
                 state: t,
                 editor: r
             }) => n.first([() => n.exitCode(), () => n.command(() => {
                 let {
                     selection: i,
-                    storedMarks: o
+                    storedMarks: s
                 } = t;
                 if (i.$from.parent.type.spec.isolating) return !1;
                 let {
-                    keepMarks: s
+                    keepMarks: o
                 } = this.options, {
                     splittableMarks: l
-                } = r.extensionManager, a = o || i.$to.parentOffset && i.$from.marks();
+                } = r.extensionManager, a = s || i.$to.parentOffset && i.$from.marks();
                 return e().insertContent({
                     type: this.name
                 }).command(({
                     tr: c,
                     dispatch: u
                 }) => {
-                    if (u && a && s) {
+                    if (u && a && o) {
                         let d = a.filter(f => l.includes(f.type.name));
                         c.ensureMarks(d)
                     }
                     return !0
                 }).run()
             })])
         }
@@ -12442,15 +11212,15 @@
     addKeyboardShortcuts() {
         return {
             "Mod-Enter": () => this.editor.commands.setHardBreak(),
             "Shift-Enter": () => this.editor.commands.setHardBreak()
         }
     }
 });
-var ku = F.create({
+var Na = H.create({
     name: "heading",
     addOptions() {
         return {
             levels: [1, 2, 3, 4, 5, 6],
             HTMLAttributes: {}
         }
     },
@@ -12473,15 +11243,15 @@
             }
         }))
     },
     renderHTML({
         node: n,
         HTMLAttributes: e
     }) {
-        return [`h${this.options.levels.includes(n.attrs.level)?n.attrs.level:this.options.levels[0]}`, z(this.options.HTMLAttributes, e), 0]
+        return [`h${this.options.levels.includes(n.attrs.level)?n.attrs.level:this.options.levels[0]}`, P(this.options.HTMLAttributes, e), 0]
     },
     addCommands() {
         return {
             setHeading: n => ({
                 commands: e
             }) => this.options.levels.includes(n.level) ? e.setNode(this.name, n) : !1,
             toggleHeading: n => ({
@@ -12494,398 +11264,398 @@
             ...n,
             [`Mod-Alt-${e}`]: () => this.editor.commands.toggleHeading({
                 level: e
             })
         }), {})
     },
     addInputRules() {
-        return this.options.levels.map(n => wr({
+        return this.options.levels.map(n => An({
             find: new RegExp(`^(#{1,${n}})\\s$`),
             type: this.type,
             getAttributes: {
                 level: n
             }
         }))
     }
 });
-var yi = 200,
-    pe = function() {};
-pe.prototype.append = function(e) {
-    return e.length ? (e = pe.from(e), !this.length && e || e.length < yi && this.leafAppend(e) || this.length < yi && e.leafPrepend(this) || this.appendInner(e)) : this
+var br = 200,
+    ee = function() {};
+ee.prototype.append = function(e) {
+    return e.length ? (e = ee.from(e), !this.length && e || e.length < br && this.leafAppend(e) || this.length < br && e.leafPrepend(this) || this.appendInner(e)) : this
 };
-pe.prototype.prepend = function(e) {
-    return e.length ? pe.from(e).append(this) : this
+ee.prototype.prepend = function(e) {
+    return e.length ? ee.from(e).append(this) : this
 };
-pe.prototype.appendInner = function(e) {
-    return new cg(this, e)
+ee.prototype.appendInner = function(e) {
+    return new Rh(this, e)
 };
-pe.prototype.slice = function(e, t) {
-    return e === void 0 && (e = 0), t === void 0 && (t = this.length), e >= t ? pe.empty : this.sliceInner(Math.max(0, e), Math.min(this.length, t))
+ee.prototype.slice = function(e, t) {
+    return e === void 0 && (e = 0), t === void 0 && (t = this.length), e >= t ? ee.empty : this.sliceInner(Math.max(0, e), Math.min(this.length, t))
 };
-pe.prototype.get = function(e) {
+ee.prototype.get = function(e) {
     if (!(e < 0 || e >= this.length)) return this.getInner(e)
 };
-pe.prototype.forEach = function(e, t, r) {
+ee.prototype.forEach = function(e, t, r) {
     t === void 0 && (t = 0), r === void 0 && (r = this.length), t <= r ? this.forEachInner(e, t, r, 0) : this.forEachInvertedInner(e, t, r, 0)
 };
-pe.prototype.map = function(e, t, r) {
+ee.prototype.map = function(e, t, r) {
     t === void 0 && (t = 0), r === void 0 && (r = this.length);
     var i = [];
-    return this.forEach(function(o, s) {
-        return i.push(e(o, s))
+    return this.forEach(function(s, o) {
+        return i.push(e(s, o))
     }, t, r), i
 };
-pe.from = function(e) {
-    return e instanceof pe ? e : e && e.length ? new vu(e) : pe.empty
+ee.from = function(e) {
+    return e instanceof ee ? e : e && e.length ? new Ia(e) : ee.empty
 };
-var vu = function(n) {
+var Ia = function(n) {
     function e(r) {
         n.call(this), this.values = r
     }
     n && (e.__proto__ = n), e.prototype = Object.create(n && n.prototype), e.prototype.constructor = e;
     var t = {
         length: {
             configurable: !0
         },
         depth: {
             configurable: !0
         }
     };
     return e.prototype.flatten = function() {
         return this.values
-    }, e.prototype.sliceInner = function(i, o) {
-        return i == 0 && o == this.length ? this : new e(this.values.slice(i, o))
+    }, e.prototype.sliceInner = function(i, s) {
+        return i == 0 && s == this.length ? this : new e(this.values.slice(i, s))
     }, e.prototype.getInner = function(i) {
         return this.values[i]
-    }, e.prototype.forEachInner = function(i, o, s, l) {
-        for (var a = o; a < s; a++)
+    }, e.prototype.forEachInner = function(i, s, o, l) {
+        for (var a = s; a < o; a++)
             if (i(this.values[a], l + a) === !1) return !1
-    }, e.prototype.forEachInvertedInner = function(i, o, s, l) {
-        for (var a = o - 1; a >= s; a--)
+    }, e.prototype.forEachInvertedInner = function(i, s, o, l) {
+        for (var a = s - 1; a >= o; a--)
             if (i(this.values[a], l + a) === !1) return !1
     }, e.prototype.leafAppend = function(i) {
-        if (this.length + i.length <= yi) return new e(this.values.concat(i.flatten()))
+        if (this.length + i.length <= br) return new e(this.values.concat(i.flatten()))
     }, e.prototype.leafPrepend = function(i) {
-        if (this.length + i.length <= yi) return new e(i.flatten().concat(this.values))
+        if (this.length + i.length <= br) return new e(i.flatten().concat(this.values))
     }, t.length.get = function() {
         return this.values.length
     }, t.depth.get = function() {
         return 0
     }, Object.defineProperties(e.prototype, t), e
-}(pe);
-pe.empty = new vu([]);
-var cg = function(n) {
+}(ee);
+ee.empty = new Ia([]);
+var Rh = function(n) {
         function e(t, r) {
             n.call(this), this.left = t, this.right = r, this.length = t.length + r.length, this.depth = Math.max(t.depth, r.depth) + 1
         }
         return n && (e.__proto__ = n), e.prototype = Object.create(n && n.prototype), e.prototype.constructor = e, e.prototype.flatten = function() {
             return this.left.flatten().concat(this.right.flatten())
         }, e.prototype.getInner = function(r) {
             return r < this.left.length ? this.left.get(r) : this.right.get(r - this.left.length)
-        }, e.prototype.forEachInner = function(r, i, o, s) {
+        }, e.prototype.forEachInner = function(r, i, s, o) {
             var l = this.left.length;
-            if (i < l && this.left.forEachInner(r, i, Math.min(o, l), s) === !1 || o > l && this.right.forEachInner(r, Math.max(i - l, 0), Math.min(this.length, o) - l, s + l) === !1) return !1
-        }, e.prototype.forEachInvertedInner = function(r, i, o, s) {
+            if (i < l && this.left.forEachInner(r, i, Math.min(s, l), o) === !1 || s > l && this.right.forEachInner(r, Math.max(i - l, 0), Math.min(this.length, s) - l, o + l) === !1) return !1
+        }, e.prototype.forEachInvertedInner = function(r, i, s, o) {
             var l = this.left.length;
-            if (i > l && this.right.forEachInvertedInner(r, i - l, Math.max(o, l) - l, s + l) === !1 || o < l && this.left.forEachInvertedInner(r, Math.min(i, l), o, s) === !1) return !1
+            if (i > l && this.right.forEachInvertedInner(r, i - l, Math.max(s, l) - l, o + l) === !1 || s < l && this.left.forEachInvertedInner(r, Math.min(i, l), s, o) === !1) return !1
         }, e.prototype.sliceInner = function(r, i) {
             if (r == 0 && i == this.length) return this;
-            var o = this.left.length;
-            return i <= o ? this.left.slice(r, i) : r >= o ? this.right.slice(r - o, i - o) : this.left.slice(r, o).append(this.right.slice(0, i - o))
+            var s = this.left.length;
+            return i <= s ? this.left.slice(r, i) : r >= s ? this.right.slice(r - s, i - s) : this.left.slice(r, s).append(this.right.slice(0, i - s))
         }, e.prototype.leafAppend = function(r) {
             var i = this.right.leafAppend(r);
             if (i) return new e(this.left, i)
         }, e.prototype.leafPrepend = function(r) {
             var i = this.left.leafPrepend(r);
             if (i) return new e(i, this.right)
         }, e.prototype.appendInner = function(r) {
             return this.left.depth >= Math.max(this.right.depth, r.depth) + 1 ? new e(this.left, new e(this.right, r)) : new e(this, r)
         }, e
-    }(pe),
-    Ns = pe;
-var ug = 500,
-    Ae = class {
+    }(ee),
+    ps = ee;
+var Ph = 500,
+    pe = class {
         constructor(e, t) {
             this.items = e, this.eventCount = t
         }
         popEvent(e, t) {
             if (this.eventCount == 0) return null;
             let r = this.items.length;
             for (;; r--)
                 if (this.items.get(r - 1).selection) {
                     --r;
                     break
-                } let i, o;
-            t && (i = this.remapping(r, this.items.length), o = i.maps.length);
-            let s = e.tr,
+                } let i, s;
+            t && (i = this.remapping(r, this.items.length), s = i.maps.length);
+            let o = e.tr,
                 l, a, c = [],
                 u = [];
             return this.items.forEach((d, f) => {
                 if (!d.step) {
-                    i || (i = this.remapping(r, f + 1), o = i.maps.length), o--, u.push(d);
+                    i || (i = this.remapping(r, f + 1), s = i.maps.length), s--, u.push(d);
                     return
                 }
                 if (i) {
-                    u.push(new Ve(d.map));
-                    let p = d.step.map(i.slice(o)),
-                        h;
-                    p && s.maybeStep(p).doc && (h = s.mapping.maps[s.mapping.maps.length - 1], c.push(new Ve(h, void 0, void 0, c.length + u.length))), o--, h && i.appendMap(h, o)
-                } else s.maybeStep(d.step);
-                if (d.selection) return l = i ? d.selection.map(i.slice(o)) : d.selection, a = new Ae(this.items.slice(0, r).append(u.reverse().concat(c)), this.eventCount - 1), !1
+                    u.push(new ke(d.map));
+                    let h = d.step.map(i.slice(s)),
+                        p;
+                    h && o.maybeStep(h).doc && (p = o.mapping.maps[o.mapping.maps.length - 1], c.push(new ke(p, void 0, void 0, c.length + u.length))), s--, p && i.appendMap(p, s)
+                } else o.maybeStep(d.step);
+                if (d.selection) return l = i ? d.selection.map(i.slice(s)) : d.selection, a = new pe(this.items.slice(0, r).append(u.reverse().concat(c)), this.eventCount - 1), !1
             }, this.items.length, 0), {
                 remaining: a,
-                transform: s,
+                transform: o,
                 selection: l
             }
         }
         addTransform(e, t, r, i) {
-            let o = [],
-                s = this.eventCount,
+            let s = [],
+                o = this.eventCount,
                 l = this.items,
                 a = !i && l.length ? l.get(l.length - 1) : null;
             for (let u = 0; u < e.steps.length; u++) {
                 let d = e.steps[u].invert(e.docs[u]),
-                    f = new Ve(e.mapping.maps[u], d, t),
-                    p;
-                (p = a && a.merge(f)) && (f = p, u ? o.pop() : l = l.slice(0, l.length - 1)), o.push(f), t && (s++, t = void 0), i || (a = f)
+                    f = new ke(e.mapping.maps[u], d, t),
+                    h;
+                (h = a && a.merge(f)) && (f = h, u ? s.pop() : l = l.slice(0, l.length - 1)), s.push(f), t && (o++, t = void 0), i || (a = f)
             }
-            let c = s - r.depth;
-            return c > fg && (l = dg(l, c), s -= c), new Ae(l.append(o), s)
+            let c = o - r.depth;
+            return c > zh && (l = Bh(l, c), o -= c), new pe(l.append(s), o)
         }
         remapping(e, t) {
-            let r = new mt;
-            return this.items.forEach((i, o) => {
-                let s = i.mirrorOffset != null && o - i.mirrorOffset >= e ? r.maps.length - i.mirrorOffset : void 0;
-                r.appendMap(i.map, s)
+            let r = new Fe;
+            return this.items.forEach((i, s) => {
+                let o = i.mirrorOffset != null && s - i.mirrorOffset >= e ? r.maps.length - i.mirrorOffset : void 0;
+                r.appendMap(i.map, o)
             }, e, t), r
         }
         addMaps(e) {
-            return this.eventCount == 0 ? this : new Ae(this.items.append(e.map(t => new Ve(t))), this.eventCount)
+            return this.eventCount == 0 ? this : new pe(this.items.append(e.map(t => new ke(t))), this.eventCount)
         }
         rebased(e, t) {
             if (!this.eventCount) return this;
             let r = [],
                 i = Math.max(0, this.items.length - t),
-                o = e.mapping,
-                s = e.steps.length,
+                s = e.mapping,
+                o = e.steps.length,
                 l = this.eventCount;
             this.items.forEach(f => {
                 f.selection && l--
             }, i);
             let a = t;
             this.items.forEach(f => {
-                let p = o.getMirror(--a);
-                if (p == null) return;
-                s = Math.min(s, p);
-                let h = o.maps[p];
+                let h = s.getMirror(--a);
+                if (h == null) return;
+                o = Math.min(o, h);
+                let p = s.maps[h];
                 if (f.step) {
-                    let m = e.steps[p].invert(e.docs[p]),
-                        b = f.selection && f.selection.map(o.slice(a + 1, p));
-                    b && l++, r.push(new Ve(h, m, b))
-                } else r.push(new Ve(h))
+                    let m = e.steps[h].invert(e.docs[h]),
+                        b = f.selection && f.selection.map(s.slice(a + 1, h));
+                    b && l++, r.push(new ke(p, m, b))
+                } else r.push(new ke(p))
             }, i);
             let c = [];
-            for (let f = t; f < s; f++) c.push(new Ve(o.maps[f]));
+            for (let f = t; f < o; f++) c.push(new ke(s.maps[f]));
             let u = this.items.slice(0, i).append(c).append(r),
-                d = new Ae(u, l);
-            return d.emptyItemCount() > ug && (d = d.compress(this.items.length - r.length)), d
+                d = new pe(u, l);
+            return d.emptyItemCount() > Ph && (d = d.compress(this.items.length - r.length)), d
         }
         emptyItemCount() {
             let e = 0;
             return this.items.forEach(t => {
                 t.step || e++
             }), e
         }
         compress(e = this.items.length) {
             let t = this.remapping(0, e),
                 r = t.maps.length,
                 i = [],
-                o = 0;
-            return this.items.forEach((s, l) => {
-                if (l >= e) i.push(s), s.selection && o++;
-                else if (s.step) {
-                    let a = s.step.map(t.slice(r)),
+                s = 0;
+            return this.items.forEach((o, l) => {
+                if (l >= e) i.push(o), o.selection && s++;
+                else if (o.step) {
+                    let a = o.step.map(t.slice(r)),
                         c = a && a.getMap();
                     if (r--, c && t.appendMap(c, r), a) {
-                        let u = s.selection && s.selection.map(t.slice(r));
-                        u && o++;
-                        let d = new Ve(c.invert(), a, u),
-                            f, p = i.length - 1;
-                        (f = i.length && i[p].merge(d)) ? i[p] = f: i.push(d)
+                        let u = o.selection && o.selection.map(t.slice(r));
+                        u && s++;
+                        let d = new ke(c.invert(), a, u),
+                            f, h = i.length - 1;
+                        (f = i.length && i[h].merge(d)) ? i[h] = f: i.push(d)
                     }
-                } else s.map && r--
-            }, this.items.length, 0), new Ae(Ns.from(i.reverse()), o)
+                } else o.map && r--
+            }, this.items.length, 0), new pe(ps.from(i.reverse()), s)
         }
     };
-Ae.empty = new Ae(Ns.empty, 0);
+pe.empty = new pe(ps.empty, 0);
 
-function dg(n, e) {
+function Bh(n, e) {
     let t;
     return n.forEach((r, i) => {
         if (r.selection && e-- == 0) return t = i, !1
     }), n.slice(t)
 }
-var Ve = class {
+var ke = class {
         constructor(e, t, r, i) {
             this.map = e, this.step = t, this.selection = r, this.mirrorOffset = i
         }
         merge(e) {
             if (this.step && e.step && !e.selection) {
                 let t = e.step.merge(this.step);
-                if (t) return new Ve(t.getMap().invert(), t, this.selection)
+                if (t) return new ke(t.getMap().invert(), t, this.selection)
             }
         }
     },
-    st = class {
-        constructor(e, t, r, i, o) {
-            this.done = e, this.undone = t, this.prevRanges = r, this.prevTime = i, this.prevComposition = o
+    Re = class {
+        constructor(e, t, r, i, s) {
+            this.done = e, this.undone = t, this.prevRanges = r, this.prevTime = i, this.prevComposition = s
         }
     },
-    fg = 20;
+    zh = 20;
 
-function pg(n, e, t, r) {
-    let i = t.getMeta(jt),
-        o;
+function Hh(n, e, t, r) {
+    let i = t.getMeta(ot),
+        s;
     if (i) return i.historyState;
-    t.getMeta(mg) && (n = new st(n.done, n.undone, null, 0, -1));
-    let s = t.getMeta("appendedTransaction");
+    t.getMeta(jh) && (n = new Re(n.done, n.undone, null, 0, -1));
+    let o = t.getMeta("appendedTransaction");
     if (t.steps.length == 0) return n;
-    if (s && s.getMeta(jt)) return s.getMeta(jt).redo ? new st(n.done.addTransform(t, void 0, r, xi(e)), n.undone, Mu(t.mapping.maps[t.steps.length - 1]), n.prevTime, n.prevComposition) : new st(n.done, n.undone.addTransform(t, void 0, r, xi(e)), null, n.prevTime, n.prevComposition);
-    if (t.getMeta("addToHistory") !== !1 && !(s && s.getMeta("addToHistory") === !1)) {
+    if (o && o.getMeta(ot)) return o.getMeta(ot).redo ? new Re(n.done.addTransform(t, void 0, r, xr(e)), n.undone, Da(t.mapping.maps[t.steps.length - 1]), n.prevTime, n.prevComposition) : new Re(n.done, n.undone.addTransform(t, void 0, r, xr(e)), null, n.prevTime, n.prevComposition);
+    if (t.getMeta("addToHistory") !== !1 && !(o && o.getMeta("addToHistory") === !1)) {
         let l = t.getMeta("composition"),
-            a = n.prevTime == 0 || !s && n.prevComposition != l && (n.prevTime < (t.time || 0) - r.newGroupDelay || !hg(t, n.prevRanges)),
-            c = s ? Is(n.prevRanges, t.mapping) : Mu(t.mapping.maps[t.steps.length - 1]);
-        return new st(n.done.addTransform(t, a ? e.selection.getBookmark() : void 0, r, xi(e)), Ae.empty, c, t.time, l ?? n.prevComposition)
-    } else return (o = t.getMeta("rebased")) ? new st(n.done.rebased(t, o), n.undone.rebased(t, o), Is(n.prevRanges, t.mapping), n.prevTime, n.prevComposition) : new st(n.done.addMaps(t.mapping.maps), n.undone.addMaps(t.mapping.maps), Is(n.prevRanges, t.mapping), n.prevTime, n.prevComposition)
+            a = n.prevTime == 0 || !o && n.prevComposition != l && (n.prevTime < (t.time || 0) - r.newGroupDelay || !Fh(t, n.prevRanges)),
+            c = o ? ms(n.prevRanges, t.mapping) : Da(t.mapping.maps[t.steps.length - 1]);
+        return new Re(n.done.addTransform(t, a ? e.selection.getBookmark() : void 0, r, xr(e)), pe.empty, c, t.time, l ?? n.prevComposition)
+    } else return (s = t.getMeta("rebased")) ? new Re(n.done.rebased(t, s), n.undone.rebased(t, s), ms(n.prevRanges, t.mapping), n.prevTime, n.prevComposition) : new Re(n.done.addMaps(t.mapping.maps), n.undone.addMaps(t.mapping.maps), ms(n.prevRanges, t.mapping), n.prevTime, n.prevComposition)
 }
 
-function hg(n, e) {
+function Fh(n, e) {
     if (!e) return !1;
     if (!n.docChanged) return !0;
     let t = !1;
     return n.mapping.maps[0].forEach((r, i) => {
-        for (let o = 0; o < e.length; o += 2) r <= e[o + 1] && i >= e[o] && (t = !0)
+        for (let s = 0; s < e.length; s += 2) r <= e[s + 1] && i >= e[s] && (t = !0)
     }), t
 }
 
-function Mu(n) {
+function Da(n) {
     let e = [];
-    return n.forEach((t, r, i, o) => e.push(i, o)), e
+    return n.forEach((t, r, i, s) => e.push(i, s)), e
 }
 
-function Is(n, e) {
+function ms(n, e) {
     if (!n) return null;
     let t = [];
     for (let r = 0; r < n.length; r += 2) {
         let i = e.map(n[r], 1),
-            o = e.map(n[r + 1], -1);
-        i <= o && t.push(i, o)
+            s = e.map(n[r + 1], -1);
+        i <= s && t.push(i, s)
     }
     return t
 }
 
-function Su(n, e, t, r) {
-    let i = xi(e),
-        o = jt.get(e).spec.config,
-        s = (r ? n.undone : n.done).popEvent(e, i);
-    if (!s) return;
-    let l = s.selection.resolve(s.transform.doc),
-        a = (r ? n.done : n.undone).addTransform(s.transform, e.selection.getBookmark(), o, i),
-        c = new st(r ? a : s.remaining, r ? s.remaining : a, null, 0, -1);
-    t(s.transform.setSelection(l).setMeta(jt, {
+function Ra(n, e, t, r) {
+    let i = xr(e),
+        s = ot.get(e).spec.config,
+        o = (r ? n.undone : n.done).popEvent(e, i);
+    if (!o) return;
+    let l = o.selection.resolve(o.transform.doc),
+        a = (r ? n.done : n.undone).addTransform(o.transform, e.selection.getBookmark(), s, i),
+        c = new Re(r ? a : o.remaining, r ? o.remaining : a, null, 0, -1);
+    t(o.transform.setSelection(l).setMeta(ot, {
         redo: r,
         historyState: c
     }).scrollIntoView())
 }
-var Ds = !1,
-    Eu = null;
+var gs = !1,
+    La = null;
 
-function xi(n) {
+function xr(n) {
     let e = n.plugins;
-    if (Eu != e) {
-        Ds = !1, Eu = e;
+    if (La != e) {
+        gs = !1, La = e;
         for (let t = 0; t < e.length; t++)
             if (e[t].spec.historyPreserveItems) {
-                Ds = !0;
+                gs = !0;
                 break
             }
     }
-    return Ds
+    return gs
 }
-var jt = new Z("history"),
-    mg = new Z("closeHistory");
+var ot = new U("history"),
+    jh = new U("closeHistory");
 
-function wu(n = {}) {
+function Pa(n = {}) {
     return n = {
         depth: n.depth || 100,
         newGroupDelay: n.newGroupDelay || 500
-    }, new q({
-        key: jt,
+    }, new $({
+        key: ot,
         state: {
             init() {
-                return new st(Ae.empty, Ae.empty, null, 0, -1)
+                return new Re(pe.empty, pe.empty, null, 0, -1)
             },
             apply(e, t, r) {
-                return pg(t, r, e, n)
+                return Hh(t, r, e, n)
             }
         },
         config: n,
         props: {
             handleDOMEvents: {
                 beforeinput(e, t) {
                     let r = t.inputType,
-                        i = r == "historyUndo" ? Ls : r == "historyRedo" ? Ps : null;
+                        i = r == "historyUndo" ? ys : r == "historyRedo" ? bs : null;
                     return i ? (t.preventDefault(), i(e.state, e.dispatch)) : !1
                 }
             }
         }
     })
 }
-var Ls = (n, e) => {
-        let t = jt.getState(n);
-        return !t || t.done.eventCount == 0 ? !1 : (e && Su(t, n, e, !1), !0)
-    },
-    Ps = (n, e) => {
-        let t = jt.getState(n);
-        return !t || t.undone.eventCount == 0 ? !1 : (e && Su(t, n, e, !0), !0)
+var ys = (n, e) => {
+        let t = ot.getState(n);
+        return !t || t.done.eventCount == 0 ? !1 : (e && Ra(t, n, e, !1), !0)
+    },
+    bs = (n, e) => {
+        let t = ot.getState(n);
+        return !t || t.undone.eventCount == 0 ? !1 : (e && Ra(t, n, e, !0), !0)
     };
-var Rs = J.create({
+var xs = V.create({
     name: "history",
     addOptions() {
         return {
             depth: 100,
             newGroupDelay: 500
         }
     },
     addCommands() {
         return {
             undo: () => ({
                 state: n,
                 dispatch: e
-            }) => Ls(n, e),
+            }) => ys(n, e),
             redo: () => ({
                 state: n,
                 dispatch: e
-            }) => Ps(n, e)
+            }) => bs(n, e)
         }
     },
     addProseMirrorPlugins() {
-        return [wu(this.options)]
+        return [Pa(this.options)]
     },
     addKeyboardShortcuts() {
         return {
             "Mod-z": () => this.editor.commands.undo(),
             "Mod-y": () => this.editor.commands.redo(),
             "Shift-Mod-z": () => this.editor.commands.redo(),
             "Mod-\u044F": () => this.editor.commands.undo(),
             "Shift-Mod-\u044F": () => this.editor.commands.redo()
         }
     }
 });
-var Tu = F.create({
+var Ba = H.create({
     name: "horizontalRule",
     addOptions() {
         return {
             HTMLAttributes: {}
         }
     },
     group: "block",
@@ -12893,15 +11663,15 @@
         return [{
             tag: "hr"
         }]
     },
     renderHTML({
         HTMLAttributes: n
     }) {
-        return ["hr", z(this.options.HTMLAttributes, n)]
+        return ["hr", P(this.options.HTMLAttributes, n)]
     },
     addCommands() {
         return {
             setHorizontalRule: () => ({
                 chain: n
             }) => n().insertContent({
                 type: this.name
@@ -12909,35 +11679,35 @@
                 tr: e,
                 dispatch: t
             }) => {
                 var r;
                 if (t) {
                     let {
                         $to: i
-                    } = e.selection, o = i.end();
-                    if (i.nodeAfter) e.setSelection(P.create(e.doc, i.pos));
+                    } = e.selection, s = i.end();
+                    if (i.nodeAfter) e.setSelection(I.create(e.doc, i.pos));
                     else {
-                        let s = (r = i.parent.type.contentMatch.defaultType) === null || r === void 0 ? void 0 : r.create();
-                        s && (e.insert(o, s), e.setSelection(P.create(e.doc, o)))
+                        let o = (r = i.parent.type.contentMatch.defaultType) === null || r === void 0 ? void 0 : r.create();
+                        o && (e.insert(s, o), e.setSelection(I.create(e.doc, s)))
                     }
                     e.scrollIntoView()
                 }
                 return !0
             }).run()
         }
     },
     addInputRules() {
-        return [gi({
+        return [yr({
             find: /^(?:---|—-|___\s|\*\*\*\s)$/,
             type: this.type
         })]
     }
 });
-var gg = /(?:^|\s)(!\[(.+|:?)]\((\S+)(?:(?:\s+)["'](\S+)["'])?\))$/,
-    Cu = F.create({
+var $h = /(?:^|\s)(!\[(.+|:?)]\((\S+)(?:(?:\s+)["'](\S+)["'])?\))$/,
+    za = H.create({
         name: "image",
         addOptions() {
             return {
                 inline: !1,
                 allowBase64: !1,
                 HTMLAttributes: {}
             }
@@ -12966,46 +11736,46 @@
             return [{
                 tag: this.options.allowBase64 ? "img[src]" : 'img[src]:not([src^="data:"])'
             }]
         },
         renderHTML({
             HTMLAttributes: n
         }) {
-            return ["img", z(this.options.HTMLAttributes, n)]
+            return ["img", P(this.options.HTMLAttributes, n)]
         },
         addCommands() {
             return {
                 setImage: n => ({
                     commands: e
                 }) => e.insertContent({
                     type: this.name,
                     attrs: n
                 })
             }
         },
         addInputRules() {
-            return [gi({
-                find: gg,
+            return [yr({
+                find: $h,
                 type: this.type,
                 getAttributes: n => {
                     let [, , e, t, r] = n;
                     return {
                         src: t,
                         alt: e,
                         title: r
                     }
                 }
             })]
         }
     });
-var yg = /(?:^|\s)((?:\*)((?:[^*]+))(?:\*))$/,
-    xg = /(?:^|\s)((?:\*)((?:[^*]+))(?:\*))/g,
-    bg = /(?:^|\s)((?:_)((?:[^_]+))(?:_))$/,
-    kg = /(?:^|\s)((?:_)((?:[^_]+))(?:_))/g,
-    Ou = V.create({
+var Vh = /(?:^|\s)((?:\*)((?:[^*]+))(?:\*))$/,
+    Jh = /(?:^|\s)((?:\*)((?:[^*]+))(?:\*))/g,
+    Wh = /(?:^|\s)((?:_)((?:[^_]+))(?:_))$/,
+    qh = /(?:^|\s)((?:_)((?:[^_]+))(?:_))/g,
+    Ha = F.create({
         name: "italic",
         addOptions() {
             return {
                 HTMLAttributes: {}
             }
         },
         parseHTML() {
@@ -13017,15 +11787,15 @@
             }, {
                 style: "font-style=italic"
             }]
         },
         renderHTML({
             HTMLAttributes: n
         }) {
-            return ["em", z(this.options.HTMLAttributes, n), 0]
+            return ["em", P(this.options.HTMLAttributes, n), 0]
         },
         addCommands() {
             return {
                 setItalic: () => ({
                     commands: n
                 }) => n.setMark(this.name),
                 toggleItalic: () => ({
@@ -13039,418 +11809,418 @@
         addKeyboardShortcuts() {
             return {
                 "Mod-i": () => this.editor.commands.toggleItalic(),
                 "Mod-I": () => this.editor.commands.toggleItalic()
             }
         },
         addInputRules() {
-            return [Jn({
-                find: yg,
+            return [Xt({
+                find: Vh,
                 type: this.type
-            }), Jn({
-                find: bg,
+            }), Xt({
+                find: Wh,
                 type: this.type
             })]
         },
         addPasteRules() {
-            return [Ft({
-                find: xg,
+            return [st({
+                find: Jh,
                 type: this.type
-            }), Ft({
-                find: kg,
+            }), st({
+                find: qh,
                 type: this.type
             })]
         }
     });
-var vg = "aaa1rp3barth4b0ott3vie4c1le2ogado5udhabi7c0ademy5centure6ountant0s9o1tor4d0s1ult4e0g1ro2tna4f0l1rica5g0akhan5ency5i0g1rbus3force5tel5kdn3l0faromeo7ibaba4pay4lfinanz6state5y2sace3tom5m0azon4ericanexpress7family11x2fam3ica3sterdam8nalytics7droid5quan4z2o0l2partments8p0le4q0uarelle8r0ab1mco4chi3my2pa2t0e3s0da2ia2sociates9t0hleta5torney7u0ction5di0ble3o3spost5thor3o0s4vianca6w0s2x0a2z0ure5ba0by2idu3namex3narepublic11d1k2r0celona5laycard4s5efoot5gains6seball5ketball8uhaus5yern5b0c1t1va3cg1n2d1e0ats2uty4er2ntley5rlin4st0buy5t2f1g1h0arti5i0ble3d1ke2ng0o3o1z2j1lack0friday9ockbuster8g1omberg7ue3m0s1w2n0pparibas9o0ats3ehringer8fa2m1nd2o0k0ing5sch2tik2on4t1utique6x2r0adesco6idgestone9oadway5ker3ther5ussels7s1t1uild0ers6siness6y1zz3v1w1y1z0h3ca0b1fe2l0l1vinklein9m0era3p2non3petown5ital0one8r0avan4ds2e0er0s4s2sa1e1h1ino4t0ering5holic7ba1n1re2s2c1d1enter4o1rn3f0a1d2g1h0anel2nel4rity4se2t2eap3intai5ristmas6ome4urch5i0priani6rcle4sco3tadel4i0c2y0eats7k1l0aims4eaning6ick2nic1que6othing5ud3ub0med6m1n1o0ach3des3ffee4llege4ogne5m0cast4mbank4unity6pany2re3uter5sec4ndos3struction8ulting7tact3ractors9oking0channel11l1p2rsica5untry4pon0s4rses6pa2r0edit0card4union9icket5own3s1uise0s6u0isinella9v1w1x1y0mru3ou3z2dabur3d1nce3ta1e1ing3sun4y2clk3ds2e0al0er2s3gree4livery5l1oitte5ta3mocrat6ntal2ist5si0gn4v2hl2iamonds6et2gital5rect0ory7scount3ver5h2y2j1k1m1np2o0cs1tor4g1mains5t1wnload7rive4tv2ubai3nlop4pont4rban5vag2r2z2earth3t2c0o2deka3u0cation8e1g1mail3erck5nergy4gineer0ing9terprises10pson4quipment8r0icsson6ni3s0q1tate5t0isalat7u0rovision8s2vents5xchange6pert3osed4ress5traspace10fage2il1rwinds6th3mily4n0s2rm0ers5shion4t3edex3edback6rrari3ero6i0at2delity5o2lm2nal1nce1ial7re0stone6mdale6sh0ing5t0ness6j1k1lickr3ghts4r2orist4wers5y2m1o0o0d0network8tball6rd1ex2sale4um3undation8x2r0ee1senius7l1ogans4ntdoor4ier7tr2ujitsu5n0d2rniture7tbol5yi3ga0l0lery3o1up4me0s3p1rden4y2b0iz3d0n2e0a1nt0ing5orge5f1g0ee3h1i0ft0s3ves2ing5l0ass3e1obal2o4m0ail3bh2o1x2n1odaddy5ld0point6f2o0dyear5g0le4p1t1v2p1q1r0ainger5phics5tis4een3ipe3ocery4up4s1t1u0ardian6cci3ge2ide2tars5ru3w1y2hair2mburg5ngout5us3bo2dfc0bank7ealth0care8lp1sinki6re1mes5gtv3iphop4samitsu7tachi5v2k0t2m1n1ockey4ldings5iday5medepot5goods5s0ense7nda3rse3spital5t0ing5t0eles2s3mail5use3w2r1sbc3t1u0ghes5yatt3undai7ibm2cbc2e1u2d1e0ee3fm2kano4l1m0amat4db2mo0bilien9n0c1dustries8finiti5o2g1k1stitute6urance4e4t0ernational10uit4vestments10o1piranga7q1r0ish4s0maili5t0anbul7t0au2v3jaguar4va3cb2e0ep2tzt3welry6io2ll2m0p2nj2o0bs1urg4t1y2p0morgan6rs3uegos4niper7kaufen5ddi3e0rryhotels6logistics9properties14fh2g1h1i0a1ds2m1nder2le4tchen5wi3m1n1oeln3matsu5sher5p0mg2n2r0d1ed3uokgroup8w1y0oto4z2la0caixa5mborghini8er3ncaster5ia3d0rover6xess5salle5t0ino3robe5w0yer5b1c1ds2ease3clerc5frak4gal2o2xus4gbt3i0dl2fe0insurance9style7ghting6ke2lly3mited4o2ncoln4de2k2psy3ve1ing5k1lc1p2oan0s3cker3us3l1ndon4tte1o3ve3pl0financial11r1s1t0d0a3u0ndbeck6xe1ury5v1y2ma0cys3drid4if1son4keup4n0agement7go3p1rket0ing3s4riott5shalls7serati6ttel5ba2c0kinsey7d1e0d0ia3et2lbourne7me1orial6n0u2rckmsd7g1h1iami3crosoft7l1ni1t2t0subishi9k1l0b1s2m0a2n1o0bi0le4da2e1i1m1nash3ey2ster5rmon3tgage6scow4to0rcycles9v0ie4p1q1r1s0d2t0n1r2u0seum3ic3tual5v1w1x1y1z2na0b1goya4me2tura4vy3ba2c1e0c1t0bank4flix4work5ustar5w0s2xt0direct7us4f0l2g0o2hk2i0co2ke1on3nja3ssan1y5l1o0kia3rthwesternmutual14on4w0ruz3tv4p1r0a1w2tt2u1yc2z2obi1server7ffice5kinawa6layan0group9dnavy5lo3m0ega4ne1g1l0ine5oo2pen3racle3nge4g0anic5igins6saka4tsuka4t2vh3pa0ge2nasonic7ris2s1tners4s1y3ssagens7y2ccw3e0t2f0izer5g1h0armacy6d1ilips5one2to0graphy6s4ysio5ics1tet2ures6d1n0g1k2oneer5zza4k1l0ace2y0station9umbing5s3m1n0c2ohl2ker3litie5rn2st3r0america6xi3ess3ime3o0d0uctions8f1gressive8mo2perties3y5tection8u0dential9s1t1ub2w0c2y2qa1pon3uebec3st5racing4dio4e0ad1lestate6tor2y4cipes5d0stone5umbrella9hab3ise0n3t2liance6n0t0als5pair3ort3ublican8st0aurant8view0s5xroth6ich0ardli6oh3l1o1p2o0cher3ks3deo3gers4om3s0vp3u0gby3hr2n2w0e2yukyu6sa0arland6fe0ty4kura4le1on3msclub4ung5ndvik0coromant12ofi4p1rl2s1ve2xo3b0i1s2c0a1b1haeffler7midt4olarships8ol3ule3warz5ience5ot3d1e0arch3t2cure1ity6ek2lect4ner3rvices6ven3w1x0y3fr2g1h0angrila6rp2w2ell3ia1ksha5oes2p0ping5uji3w0time7i0lk2na1gles5te3j1k0i0n2y0pe4l0ing4m0art3ile4n0cf3o0ccer3ial4ftbank4ware6hu2lar2utions7ng1y2y2pa0ce3ort2t3r0l2s1t0ada2ples4r1tebank4farm7c0group6ockholm6rage3e3ream4udio2y3yle4u0cks3pplies3y2ort5rf1gery5zuki5v1watch4iss4x1y0dney4stems6z2tab1ipei4lk2obao4rget4tamotors6r2too4x0i3c0i2d0k2eam2ch0nology8l1masek5nnis4va3f1g1h0d1eater2re6iaa2ckets5enda4ffany5ps2res2ol4j0maxx4x2k0maxx5l1m0all4n1o0day3kyo3ols3p1ray3shiba5tal3urs3wn2yota3s3r0ade1ing4ining5vel0channel7ers0insurance16ust3v2t1ube2i1nes3shu4v0s2w1z2ua1bank3s2g1k1nicom3versity8o2ol2ps2s1y1z2va0cations7na1guard7c1e0gas3ntures6risign5m\xF6gensberater2ung14sicherung10t2g1i0ajes4deo3g1king4llas4n1p1rgin4sa1ion4va1o3laanderen9n1odka3lkswagen7vo3te1ing3o2yage5u0elos6wales2mart4ter4ng0gou5tch0es6eather0channel12bcam3er2site5d0ding5ibo2r3f1hoswho6ien2ki2lliamhill9n0dows4e1ners6me2olterskluwer11odside6rk0s2ld3w2s1tc1f3xbox3erox4finity6ihuan4n2xx2yz3yachts4hoo3maxun5ndex5e1odobashi7ga2kohama6u0tube6t1un3za0ppos4ra3ero3ip2m1one3uerich6w2",
-    Mg = "\u03B5\u03BB1\u03C52\u0431\u04331\u0435\u043B3\u0434\u0435\u0442\u04384\u0435\u044E2\u043A\u0430\u0442\u043E\u043B\u0438\u043A6\u043E\u043C3\u043C\u043A\u04342\u043E\u043D1\u0441\u043A\u0432\u04306\u043E\u043D\u043B\u0430\u0439\u043D5\u0440\u04333\u0440\u0443\u04412\u04442\u0441\u0430\u0439\u04423\u0440\u04313\u0443\u043A\u04403\u049B\u0430\u04373\u0570\u0561\u05753\u05D9\u05E9\u05E8\u05D0\u05DC5\u05E7\u05D5\u05DD3\u0627\u0628\u0648\u0638\u0628\u064A5\u062A\u0635\u0627\u0644\u0627\u062A6\u0631\u0627\u0645\u0643\u06485\u0644\u0627\u0631\u062F\u06464\u0628\u062D\u0631\u064A\u06465\u062C\u0632\u0627\u0626\u06315\u0633\u0639\u0648\u062F\u064A\u06296\u0639\u0644\u064A\u0627\u06465\u0645\u063A\u0631\u06285\u0645\u0627\u0631\u0627\u062A5\u06CC\u0631\u0627\u06465\u0628\u0627\u0631\u062A2\u0632\u0627\u06314\u064A\u062A\u06433\u06BE\u0627\u0631\u062A5\u062A\u0648\u0646\u06334\u0633\u0648\u062F\u0627\u06463\u0631\u064A\u06295\u0634\u0628\u0643\u06294\u0639\u0631\u0627\u06422\u06282\u0645\u0627\u06464\u0641\u0644\u0633\u0637\u064A\u06466\u0642\u0637\u06313\u0643\u0627\u062B\u0648\u0644\u064A\u06436\u0648\u06453\u0645\u0635\u06312\u0644\u064A\u0633\u064A\u06275\u0648\u0631\u064A\u062A\u0627\u0646\u064A\u06277\u0642\u06394\u0647\u0645\u0631\u0627\u06475\u067E\u0627\u06A9\u0633\u062A\u0627\u06467\u0680\u0627\u0631\u062A4\u0915\u0949\u092E3\u0928\u0947\u091F3\u092D\u093E\u0930\u09240\u092E\u094D3\u094B\u09245\u0938\u0902\u0917\u0920\u09285\u09AC\u09BE\u0982\u09B2\u09BE5\u09AD\u09BE\u09B0\u09A42\u09F0\u09A44\u0A2D\u0A3E\u0A30\u0A244\u0AAD\u0ABE\u0AB0\u0AA44\u0B2D\u0B3E\u0B30\u0B244\u0B87\u0BA8\u0BCD\u0BA4\u0BBF\u0BAF\u0BBE6\u0BB2\u0B99\u0BCD\u0B95\u0BC86\u0B9A\u0BBF\u0B99\u0BCD\u0B95\u0BAA\u0BCD\u0BAA\u0BC2\u0BB0\u0BCD11\u0C2D\u0C3E\u0C30\u0C24\u0C4D5\u0CAD\u0CBE\u0CB0\u0CA44\u0D2D\u0D3E\u0D30\u0D24\u0D025\u0DBD\u0D82\u0D9A\u0DCF4\u0E04\u0E2D\u0E213\u0E44\u0E17\u0E223\u0EA5\u0EB2\u0EA73\u10D2\u10D42\u307F\u3093\u306A3\u30A2\u30DE\u30BE\u30F34\u30AF\u30E9\u30A6\u30C94\u30B0\u30FC\u30B0\u30EB4\u30B3\u30E02\u30B9\u30C8\u30A23\u30BB\u30FC\u30EB3\u30D5\u30A1\u30C3\u30B7\u30E7\u30F36\u30DD\u30A4\u30F3\u30C84\u4E16\u754C2\u4E2D\u4FE11\u56FD1\u570B1\u6587\u7F513\u4E9A\u9A6C\u900A3\u4F01\u4E1A2\u4F5B\u5C712\u4FE1\u606F2\u5065\u5EB72\u516B\u53662\u516C\u53F81\u76CA2\u53F0\u6E7E1\u70632\u5546\u57CE1\u5E971\u68072\u5609\u91CC0\u5927\u9152\u5E975\u5728\u7EBF2\u5927\u62FF2\u5929\u4E3B\u65593\u5A31\u4E502\u5BB6\u96FB2\u5E7F\u4E1C2\u5FAE\u535A2\u6148\u55842\u6211\u7231\u4F603\u624B\u673A2\u62DB\u80582\u653F\u52A11\u5E9C2\u65B0\u52A0\u57612\u95FB2\u65F6\u5C1A2\u66F8\u7C4D2\u673A\u67842\u6DE1\u9A6C\u95213\u6E38\u620F2\u6FB3\u95802\u70B9\u770B2\u79FB\u52A82\u7EC4\u7EC7\u673A\u67844\u7F51\u57401\u5E971\u7AD91\u7EDC2\u8054\u901A2\u8C37\u6B4C2\u8D2D\u72692\u901A\u8CA92\u96C6\u56E22\u96FB\u8A0A\u76C8\u79D14\u98DE\u5229\u6D663\u98DF\u54C12\u9910\u53852\u9999\u683C\u91CC\u62C93\u6E2F2\uB2F7\uB1371\uCEF42\uC0BC\uC1312\uD55C\uAD6D2",
-    Qn = (n, e) => {
+var Kh = "aaa1rp3barth4b0ott3vie4c1le2ogado5udhabi7c0ademy5centure6ountant0s9o1tor4d0s1ult4e0g1ro2tna4f0l1rica5g0akhan5ency5i0g1rbus3force5tel5kdn3l0faromeo7ibaba4pay4lfinanz6state5y2sace3tom5m0azon4ericanexpress7family11x2fam3ica3sterdam8nalytics7droid5quan4z2o0l2partments8p0le4q0uarelle8r0ab1mco4chi3my2pa2t0e3s0da2ia2sociates9t0hleta5torney7u0ction5di0ble3o3spost5thor3o0s4vianca6w0s2x0a2z0ure5ba0by2idu3namex3narepublic11d1k2r0celona5laycard4s5efoot5gains6seball5ketball8uhaus5yern5b0c1t1va3cg1n2d1e0ats2uty4er2ntley5rlin4st0buy5t2f1g1h0arti5i0ble3d1ke2ng0o3o1z2j1lack0friday9ockbuster8g1omberg7ue3m0s1w2n0pparibas9o0ats3ehringer8fa2m1nd2o0k0ing5sch2tik2on4t1utique6x2r0adesco6idgestone9oadway5ker3ther5ussels7s1t1uild0ers6siness6y1zz3v1w1y1z0h3ca0b1fe2l0l1vinklein9m0era3p2non3petown5ital0one8r0avan4ds2e0er0s4s2sa1e1h1ino4t0ering5holic7ba1n1re2s2c1d1enter4o1rn3f0a1d2g1h0anel2nel4rity4se2t2eap3intai5ristmas6ome4urch5i0priani6rcle4sco3tadel4i0c2y0eats7k1l0aims4eaning6ick2nic1que6othing5ud3ub0med6m1n1o0ach3des3ffee4llege4ogne5m0cast4mbank4unity6pany2re3uter5sec4ndos3struction8ulting7tact3ractors9oking0channel11l1p2rsica5untry4pon0s4rses6pa2r0edit0card4union9icket5own3s1uise0s6u0isinella9v1w1x1y0mru3ou3z2dabur3d1nce3ta1e1ing3sun4y2clk3ds2e0al0er2s3gree4livery5l1oitte5ta3mocrat6ntal2ist5si0gn4v2hl2iamonds6et2gital5rect0ory7scount3ver5h2y2j1k1m1np2o0cs1tor4g1mains5t1wnload7rive4tv2ubai3nlop4pont4rban5vag2r2z2earth3t2c0o2deka3u0cation8e1g1mail3erck5nergy4gineer0ing9terprises10pson4quipment8r0icsson6ni3s0q1tate5t0isalat7u0rovision8s2vents5xchange6pert3osed4ress5traspace10fage2il1rwinds6th3mily4n0s2rm0ers5shion4t3edex3edback6rrari3ero6i0at2delity5o2lm2nal1nce1ial7re0stone6mdale6sh0ing5t0ness6j1k1lickr3ghts4r2orist4wers5y2m1o0o0d0network8tball6rd1ex2sale4um3undation8x2r0ee1senius7l1ogans4ntdoor4ier7tr2ujitsu5n0d2rniture7tbol5yi3ga0l0lery3o1up4me0s3p1rden4y2b0iz3d0n2e0a1nt0ing5orge5f1g0ee3h1i0ft0s3ves2ing5l0ass3e1obal2o4m0ail3bh2o1x2n1odaddy5ld0point6f2o0dyear5g0le4p1t1v2p1q1r0ainger5phics5tis4een3ipe3ocery4up4s1t1u0ardian6cci3ge2ide2tars5ru3w1y2hair2mburg5ngout5us3bo2dfc0bank7ealth0care8lp1sinki6re1mes5gtv3iphop4samitsu7tachi5v2k0t2m1n1ockey4ldings5iday5medepot5goods5s0ense7nda3rse3spital5t0ing5t0eles2s3mail5use3w2r1sbc3t1u0ghes5yatt3undai7ibm2cbc2e1u2d1e0ee3fm2kano4l1m0amat4db2mo0bilien9n0c1dustries8finiti5o2g1k1stitute6urance4e4t0ernational10uit4vestments10o1piranga7q1r0ish4s0maili5t0anbul7t0au2v3jaguar4va3cb2e0ep2tzt3welry6io2ll2m0p2nj2o0bs1urg4t1y2p0morgan6rs3uegos4niper7kaufen5ddi3e0rryhotels6logistics9properties14fh2g1h1i0a1ds2m1nder2le4tchen5wi3m1n1oeln3matsu5sher5p0mg2n2r0d1ed3uokgroup8w1y0oto4z2la0caixa5mborghini8er3ncaster5ia3d0rover6xess5salle5t0ino3robe5w0yer5b1c1ds2ease3clerc5frak4gal2o2xus4gbt3i0dl2fe0insurance9style7ghting6ke2lly3mited4o2ncoln4de2k2psy3ve1ing5k1lc1p2oan0s3cker3us3l1ndon4tte1o3ve3pl0financial11r1s1t0d0a3u0ndbeck6xe1ury5v1y2ma0cys3drid4if1son4keup4n0agement7go3p1rket0ing3s4riott5shalls7serati6ttel5ba2c0kinsey7d1e0d0ia3et2lbourne7me1orial6n0u2rckmsd7g1h1iami3crosoft7l1ni1t2t0subishi9k1l0b1s2m0a2n1o0bi0le4da2e1i1m1nash3ey2ster5rmon3tgage6scow4to0rcycles9v0ie4p1q1r1s0d2t0n1r2u0seum3ic3tual5v1w1x1y1z2na0b1goya4me2tura4vy3ba2c1e0c1t0bank4flix4work5ustar5w0s2xt0direct7us4f0l2g0o2hk2i0co2ke1on3nja3ssan1y5l1o0kia3rthwesternmutual14on4w0ruz3tv4p1r0a1w2tt2u1yc2z2obi1server7ffice5kinawa6layan0group9dnavy5lo3m0ega4ne1g1l0ine5oo2pen3racle3nge4g0anic5igins6saka4tsuka4t2vh3pa0ge2nasonic7ris2s1tners4s1y3ssagens7y2ccw3e0t2f0izer5g1h0armacy6d1ilips5one2to0graphy6s4ysio5ics1tet2ures6d1n0g1k2oneer5zza4k1l0ace2y0station9umbing5s3m1n0c2ohl2ker3litie5rn2st3r0america6xi3ess3ime3o0d0uctions8f1gressive8mo2perties3y5tection8u0dential9s1t1ub2w0c2y2qa1pon3uebec3st5racing4dio4e0ad1lestate6tor2y4cipes5d0stone5umbrella9hab3ise0n3t2liance6n0t0als5pair3ort3ublican8st0aurant8view0s5xroth6ich0ardli6oh3l1o1p2o0cher3ks3deo3gers4om3s0vp3u0gby3hr2n2w0e2yukyu6sa0arland6fe0ty4kura4le1on3msclub4ung5ndvik0coromant12ofi4p1rl2s1ve2xo3b0i1s2c0a1b1haeffler7midt4olarships8ol3ule3warz5ience5ot3d1e0arch3t2cure1ity6ek2lect4ner3rvices6ven3w1x0y3fr2g1h0angrila6rp2w2ell3ia1ksha5oes2p0ping5uji3w0time7i0lk2na1gles5te3j1k0i0n2y0pe4l0ing4m0art3ile4n0cf3o0ccer3ial4ftbank4ware6hu2lar2utions7ng1y2y2pa0ce3ort2t3r0l2s1t0ada2ples4r1tebank4farm7c0group6ockholm6rage3e3ream4udio2y3yle4u0cks3pplies3y2ort5rf1gery5zuki5v1watch4iss4x1y0dney4stems6z2tab1ipei4lk2obao4rget4tamotors6r2too4x0i3c0i2d0k2eam2ch0nology8l1masek5nnis4va3f1g1h0d1eater2re6iaa2ckets5enda4ffany5ps2res2ol4j0maxx4x2k0maxx5l1m0all4n1o0day3kyo3ols3p1ray3shiba5tal3urs3wn2yota3s3r0ade1ing4ining5vel0channel7ers0insurance16ust3v2t1ube2i1nes3shu4v0s2w1z2ua1bank3s2g1k1nicom3versity8o2ol2ps2s1y1z2va0cations7na1guard7c1e0gas3ntures6risign5m\xF6gensberater2ung14sicherung10t2g1i0ajes4deo3g1king4llas4n1p1rgin4sa1ion4va1o3laanderen9n1odka3lkswagen7vo3te1ing3o2yage5u0elos6wales2mart4ter4ng0gou5tch0es6eather0channel12bcam3er2site5d0ding5ibo2r3f1hoswho6ien2ki2lliamhill9n0dows4e1ners6me2olterskluwer11odside6rk0s2ld3w2s1tc1f3xbox3erox4finity6ihuan4n2xx2yz3yachts4hoo3maxun5ndex5e1odobashi7ga2kohama6u0tube6t1un3za0ppos4ra3ero3ip2m1one3uerich6w2",
+    Uh = "\u03B5\u03BB1\u03C52\u0431\u04331\u0435\u043B3\u0434\u0435\u0442\u04384\u0435\u044E2\u043A\u0430\u0442\u043E\u043B\u0438\u043A6\u043E\u043C3\u043C\u043A\u04342\u043E\u043D1\u0441\u043A\u0432\u04306\u043E\u043D\u043B\u0430\u0439\u043D5\u0440\u04333\u0440\u0443\u04412\u04442\u0441\u0430\u0439\u04423\u0440\u04313\u0443\u043A\u04403\u049B\u0430\u04373\u0570\u0561\u05753\u05D9\u05E9\u05E8\u05D0\u05DC5\u05E7\u05D5\u05DD3\u0627\u0628\u0648\u0638\u0628\u064A5\u062A\u0635\u0627\u0644\u0627\u062A6\u0631\u0627\u0645\u0643\u06485\u0644\u0627\u0631\u062F\u06464\u0628\u062D\u0631\u064A\u06465\u062C\u0632\u0627\u0626\u06315\u0633\u0639\u0648\u062F\u064A\u06296\u0639\u0644\u064A\u0627\u06465\u0645\u063A\u0631\u06285\u0645\u0627\u0631\u0627\u062A5\u06CC\u0631\u0627\u06465\u0628\u0627\u0631\u062A2\u0632\u0627\u06314\u064A\u062A\u06433\u06BE\u0627\u0631\u062A5\u062A\u0648\u0646\u06334\u0633\u0648\u062F\u0627\u06463\u0631\u064A\u06295\u0634\u0628\u0643\u06294\u0639\u0631\u0627\u06422\u06282\u0645\u0627\u06464\u0641\u0644\u0633\u0637\u064A\u06466\u0642\u0637\u06313\u0643\u0627\u062B\u0648\u0644\u064A\u06436\u0648\u06453\u0645\u0635\u06312\u0644\u064A\u0633\u064A\u06275\u0648\u0631\u064A\u062A\u0627\u0646\u064A\u06277\u0642\u06394\u0647\u0645\u0631\u0627\u06475\u067E\u0627\u06A9\u0633\u062A\u0627\u06467\u0680\u0627\u0631\u062A4\u0915\u0949\u092E3\u0928\u0947\u091F3\u092D\u093E\u0930\u09240\u092E\u094D3\u094B\u09245\u0938\u0902\u0917\u0920\u09285\u09AC\u09BE\u0982\u09B2\u09BE5\u09AD\u09BE\u09B0\u09A42\u09F0\u09A44\u0A2D\u0A3E\u0A30\u0A244\u0AAD\u0ABE\u0AB0\u0AA44\u0B2D\u0B3E\u0B30\u0B244\u0B87\u0BA8\u0BCD\u0BA4\u0BBF\u0BAF\u0BBE6\u0BB2\u0B99\u0BCD\u0B95\u0BC86\u0B9A\u0BBF\u0B99\u0BCD\u0B95\u0BAA\u0BCD\u0BAA\u0BC2\u0BB0\u0BCD11\u0C2D\u0C3E\u0C30\u0C24\u0C4D5\u0CAD\u0CBE\u0CB0\u0CA44\u0D2D\u0D3E\u0D30\u0D24\u0D025\u0DBD\u0D82\u0D9A\u0DCF4\u0E04\u0E2D\u0E213\u0E44\u0E17\u0E223\u0EA5\u0EB2\u0EA73\u10D2\u10D42\u307F\u3093\u306A3\u30A2\u30DE\u30BE\u30F34\u30AF\u30E9\u30A6\u30C94\u30B0\u30FC\u30B0\u30EB4\u30B3\u30E02\u30B9\u30C8\u30A23\u30BB\u30FC\u30EB3\u30D5\u30A1\u30C3\u30B7\u30E7\u30F36\u30DD\u30A4\u30F3\u30C84\u4E16\u754C2\u4E2D\u4FE11\u56FD1\u570B1\u6587\u7F513\u4E9A\u9A6C\u900A3\u4F01\u4E1A2\u4F5B\u5C712\u4FE1\u606F2\u5065\u5EB72\u516B\u53662\u516C\u53F81\u76CA2\u53F0\u6E7E1\u70632\u5546\u57CE1\u5E971\u68072\u5609\u91CC0\u5927\u9152\u5E975\u5728\u7EBF2\u5927\u62FF2\u5929\u4E3B\u65593\u5A31\u4E502\u5BB6\u96FB2\u5E7F\u4E1C2\u5FAE\u535A2\u6148\u55842\u6211\u7231\u4F603\u624B\u673A2\u62DB\u80582\u653F\u52A11\u5E9C2\u65B0\u52A0\u57612\u95FB2\u65F6\u5C1A2\u66F8\u7C4D2\u673A\u67842\u6DE1\u9A6C\u95213\u6E38\u620F2\u6FB3\u95802\u70B9\u770B2\u79FB\u52A82\u7EC4\u7EC7\u673A\u67844\u7F51\u57401\u5E971\u7AD91\u7EDC2\u8054\u901A2\u8C37\u6B4C2\u8D2D\u72692\u901A\u8CA92\u96C6\u56E22\u96FB\u8A0A\u76C8\u79D14\u98DE\u5229\u6D663\u98DF\u54C12\u9910\u53852\u9999\u683C\u91CC\u62C93\u6E2F2\uB2F7\uB1371\uCEF42\uC0BC\uC1312\uD55C\uAD6D2",
+    sn = (n, e) => {
         for (let t in e) n[t] = e[t];
         return n
     },
-    js = "numeric",
-    Vs = "ascii",
-    $s = "alpha",
-    Mi = "asciinumeric",
-    bi = "alphanumeric",
-    Ws = "domain",
-    zu = "emoji",
-    Eg = "scheme",
-    Sg = "slashscheme",
-    Au = "whitespace";
+    ws = "numeric",
+    Ts = "ascii",
+    Cs = "alpha",
+    Er = "asciinumeric",
+    kr = "alphanumeric",
+    As = "domain",
+    Ua = "emoji",
+    _h = "scheme",
+    Gh = "slashscheme",
+    Fa = "whitespace";
 
-function wg(n, e) {
+function Qh(n, e) {
     return n in e || (e[n] = []), e[n]
 }
 
-function kn(n, e, t) {
-    e[js] && (e[Mi] = !0, e[bi] = !0), e[Vs] && (e[Mi] = !0, e[$s] = !0), e[Mi] && (e[bi] = !0), e[$s] && (e[bi] = !0), e[bi] && (e[Ws] = !0), e[zu] && (e[Ws] = !0);
+function Dt(n, e, t) {
+    e[ws] && (e[Er] = !0, e[kr] = !0), e[Ts] && (e[Er] = !0, e[Cs] = !0), e[Er] && (e[kr] = !0), e[Cs] && (e[kr] = !0), e[kr] && (e[As] = !0), e[Ua] && (e[As] = !0);
     for (let r in e) {
-        let i = wg(r, t);
+        let i = Qh(r, t);
         i.indexOf(n) < 0 && i.push(n)
     }
 }
 
-function Tg(n, e) {
+function Yh(n, e) {
     let t = {};
     for (let r in e) e[r].indexOf(n) >= 0 && (t[r] = !0);
     return t
 }
 
-function Oe(n) {
+function he(n) {
     n === void 0 && (n = null), this.j = {}, this.jr = [], this.jd = null, this.t = n
 }
-Oe.groups = {};
-Oe.prototype = {
+he.groups = {};
+he.prototype = {
     accepts() {
         return !!this.t
     },
     go(n) {
         let e = this,
             t = e.j[n];
         if (t) return t;
         for (let r = 0; r < e.jr.length; r++) {
             let i = e.jr[r][0],
-                o = e.jr[r][1];
-            if (o && i.test(n)) return o
+                s = e.jr[r][1];
+            if (s && i.test(n)) return s
         }
         return e.jd
     },
     has(n, e) {
         return e === void 0 && (e = !1), e ? n in this.j : !!this.go(n)
     },
     ta(n, e, t, r) {
         for (let i = 0; i < n.length; i++) this.tt(n[i], e, t, r)
     },
     tr(n, e, t, r) {
-        r = r || Oe.groups;
+        r = r || he.groups;
         let i;
-        return e && e.j ? i = e : (i = new Oe(e), t && r && kn(e, t, r)), this.jr.push([n, i]), i
+        return e && e.j ? i = e : (i = new he(e), t && r && Dt(e, t, r)), this.jr.push([n, i]), i
     },
     ts(n, e, t, r) {
         let i = this,
-            o = n.length;
-        if (!o) return i;
-        for (let s = 0; s < o - 1; s++) i = i.tt(n[s]);
-        return i.tt(n[o - 1], e, t, r)
+            s = n.length;
+        if (!s) return i;
+        for (let o = 0; o < s - 1; o++) i = i.tt(n[o]);
+        return i.tt(n[s - 1], e, t, r)
     },
     tt(n, e, t, r) {
-        r = r || Oe.groups;
+        r = r || he.groups;
         let i = this;
         if (e && e.j) return i.j[n] = e, e;
-        let o = e,
-            s, l = i.go(n);
-        if (l ? (s = new Oe, Qn(s.j, l.j), s.jr.push.apply(s.jr, l.jr), s.jd = l.jd, s.t = l.t) : s = new Oe, o) {
+        let s = e,
+            o, l = i.go(n);
+        if (l ? (o = new he, sn(o.j, l.j), o.jr.push.apply(o.jr, l.jr), o.jd = l.jd, o.t = l.t) : o = new he, s) {
             if (r)
-                if (s.t && typeof s.t == "string") {
-                    let a = Qn(Tg(s.t, r), t);
-                    kn(o, a, r)
-                } else t && kn(o, t, r);
-            s.t = o
-        }
-        return i.j[n] = s, s
-    }
-};
-var N = (n, e, t, r, i) => n.ta(e, t, r, i),
-    $e = (n, e, t, r, i) => n.tr(e, t, r, i),
-    Nu = (n, e, t, r, i) => n.ts(e, t, r, i),
-    M = (n, e, t, r, i) => n.tt(e, t, r, i),
-    Mt = "WORD",
-    qs = "UWORD",
-    Nr = "LOCALHOST",
-    Js = "TLD",
-    Ks = "UTLD",
-    Ei = "SCHEME",
-    Un = "SLASH_SCHEME",
-    Us = "NUM",
-    Hu = "WS",
-    _s = "NL",
-    _n = "OPENBRACE",
-    Tr = "OPENBRACKET",
-    Cr = "OPENANGLEBRACKET",
-    Or = "OPENPAREN",
-    xn = "CLOSEBRACE",
-    Gn = "CLOSEBRACKET",
-    Yn = "CLOSEANGLEBRACKET",
-    bn = "CLOSEPAREN",
-    Si = "AMPERSAND",
-    wi = "APOSTROPHE",
-    Ti = "ASTERISK",
-    $t = "AT",
-    Ci = "BACKSLASH",
-    Oi = "BACKTICK",
-    Ai = "CARET",
-    Wt = "COLON",
-    Gs = "COMMA",
-    Ni = "DOLLAR",
-    lt = "DOT",
-    Ii = "EQUALS",
-    Ys = "EXCLAMATION",
-    at = "HYPHEN",
-    Di = "PERCENT",
-    Li = "PIPE",
-    Pi = "PLUS",
-    Ri = "POUND",
-    Bi = "QUERY",
-    Qs = "QUOTE",
-    Xs = "SEMI",
-    ct = "SLASH",
-    Ar = "TILDE",
-    zi = "UNDERSCORE",
-    Fu = "EMOJI",
-    Hi = "SYM",
-    ju = Object.freeze({
+                if (o.t && typeof o.t == "string") {
+                    let a = sn(Yh(o.t, r), t);
+                    Dt(s, a, r)
+                } else t && Dt(s, t, r);
+            o.t = s
+        }
+        return i.j[n] = o, o
+    }
+};
+var C = (n, e, t, r, i) => n.ta(e, t, r, i),
+    Me = (n, e, t, r, i) => n.tr(e, t, r, i),
+    ja = (n, e, t, r, i) => n.ts(e, t, r, i),
+    S = (n, e, t, r, i) => n.tt(e, t, r, i),
+    Ke = "WORD",
+    Os = "UWORD",
+    Dn = "LOCALHOST",
+    vs = "TLD",
+    Ns = "UTLD",
+    wr = "SCHEME",
+    en = "SLASH_SCHEME",
+    Is = "NUM",
+    _a = "WS",
+    Ds = "NL",
+    tn = "OPENBRACE",
+    On = "OPENBRACKET",
+    vn = "OPENANGLEBRACKET",
+    Nn = "OPENPAREN",
+    Nt = "CLOSEBRACE",
+    nn = "CLOSEBRACKET",
+    rn = "CLOSEANGLEBRACKET",
+    It = "CLOSEPAREN",
+    Tr = "AMPERSAND",
+    Cr = "APOSTROPHE",
+    Ar = "ASTERISK",
+    at = "AT",
+    Or = "BACKSLASH",
+    vr = "BACKTICK",
+    Nr = "CARET",
+    ct = "COLON",
+    Ls = "COMMA",
+    Ir = "DOLLAR",
+    Pe = "DOT",
+    Dr = "EQUALS",
+    Rs = "EXCLAMATION",
+    Be = "HYPHEN",
+    Lr = "PERCENT",
+    Rr = "PIPE",
+    Pr = "PLUS",
+    Br = "POUND",
+    zr = "QUERY",
+    Ps = "QUOTE",
+    Bs = "SEMI",
+    ze = "SLASH",
+    In = "TILDE",
+    Hr = "UNDERSCORE",
+    Ga = "EMOJI",
+    Fr = "SYM",
+    Qa = Object.freeze({
         __proto__: null,
-        WORD: Mt,
-        UWORD: qs,
-        LOCALHOST: Nr,
-        TLD: Js,
-        UTLD: Ks,
-        SCHEME: Ei,
-        SLASH_SCHEME: Un,
-        NUM: Us,
-        WS: Hu,
-        NL: _s,
-        OPENBRACE: _n,
-        OPENBRACKET: Tr,
-        OPENANGLEBRACKET: Cr,
-        OPENPAREN: Or,
-        CLOSEBRACE: xn,
-        CLOSEBRACKET: Gn,
-        CLOSEANGLEBRACKET: Yn,
-        CLOSEPAREN: bn,
-        AMPERSAND: Si,
-        APOSTROPHE: wi,
-        ASTERISK: Ti,
-        AT: $t,
-        BACKSLASH: Ci,
-        BACKTICK: Oi,
-        CARET: Ai,
-        COLON: Wt,
-        COMMA: Gs,
-        DOLLAR: Ni,
-        DOT: lt,
-        EQUALS: Ii,
-        EXCLAMATION: Ys,
-        HYPHEN: at,
-        PERCENT: Di,
-        PIPE: Li,
-        PLUS: Pi,
-        POUND: Ri,
-        QUERY: Bi,
-        QUOTE: Qs,
-        SEMI: Xs,
-        SLASH: ct,
-        TILDE: Ar,
-        UNDERSCORE: zi,
-        EMOJI: Fu,
-        SYM: Hi
+        WORD: Ke,
+        UWORD: Os,
+        LOCALHOST: Dn,
+        TLD: vs,
+        UTLD: Ns,
+        SCHEME: wr,
+        SLASH_SCHEME: en,
+        NUM: Is,
+        WS: _a,
+        NL: Ds,
+        OPENBRACE: tn,
+        OPENBRACKET: On,
+        OPENANGLEBRACKET: vn,
+        OPENPAREN: Nn,
+        CLOSEBRACE: Nt,
+        CLOSEBRACKET: nn,
+        CLOSEANGLEBRACKET: rn,
+        CLOSEPAREN: It,
+        AMPERSAND: Tr,
+        APOSTROPHE: Cr,
+        ASTERISK: Ar,
+        AT: at,
+        BACKSLASH: Or,
+        BACKTICK: vr,
+        CARET: Nr,
+        COLON: ct,
+        COMMA: Ls,
+        DOLLAR: Ir,
+        DOT: Pe,
+        EQUALS: Dr,
+        EXCLAMATION: Rs,
+        HYPHEN: Be,
+        PERCENT: Lr,
+        PIPE: Rr,
+        PLUS: Pr,
+        POUND: Br,
+        QUERY: zr,
+        QUOTE: Ps,
+        SEMI: Bs,
+        SLASH: ze,
+        TILDE: In,
+        UNDERSCORE: Hr,
+        EMOJI: Ga,
+        SYM: Fr
     }),
-    Kn = /[a-z]/,
-    Bs = /\p{L}/u,
-    zs = /\p{Emoji}/u;
-var Hs = /\d/,
-    Iu = /\s/;
-var Du = `
+    Zt = /[a-z]/,
+    ks = /\p{L}/u,
+    Ms = /\p{Emoji}/u;
+var Ss = /\d/,
+    $a = /\s/;
+var Va = `
 `,
-    Cg = "\uFE0F",
-    Og = "\u200D",
-    ki = null,
-    vi = null;
+    Xh = "\uFE0F",
+    Zh = "\u200D",
+    Mr = null,
+    Sr = null;
 
-function Ag(n) {
+function ep(n) {
     n === void 0 && (n = []);
     let e = {};
-    Oe.groups = e;
-    let t = new Oe;
-    ki == null && (ki = Lu(vg)), vi == null && (vi = Lu(Mg)), M(t, "'", wi), M(t, "{", _n), M(t, "[", Tr), M(t, "<", Cr), M(t, "(", Or), M(t, "}", xn), M(t, "]", Gn), M(t, ">", Yn), M(t, ")", bn), M(t, "&", Si), M(t, "*", Ti), M(t, "@", $t), M(t, "`", Oi), M(t, "^", Ai), M(t, ":", Wt), M(t, ",", Gs), M(t, "$", Ni), M(t, ".", lt), M(t, "=", Ii), M(t, "!", Ys), M(t, "-", at), M(t, "%", Di), M(t, "|", Li), M(t, "+", Pi), M(t, "#", Ri), M(t, "?", Bi), M(t, '"', Qs), M(t, "/", ct), M(t, ";", Xs), M(t, "~", Ar), M(t, "_", zi), M(t, "\\", Ci);
-    let r = $e(t, Hs, Us, {
-        [js]: !0
+    he.groups = e;
+    let t = new he;
+    Mr == null && (Mr = Ja(Kh)), Sr == null && (Sr = Ja(Uh)), S(t, "'", Cr), S(t, "{", tn), S(t, "[", On), S(t, "<", vn), S(t, "(", Nn), S(t, "}", Nt), S(t, "]", nn), S(t, ">", rn), S(t, ")", It), S(t, "&", Tr), S(t, "*", Ar), S(t, "@", at), S(t, "`", vr), S(t, "^", Nr), S(t, ":", ct), S(t, ",", Ls), S(t, "$", Ir), S(t, ".", Pe), S(t, "=", Dr), S(t, "!", Rs), S(t, "-", Be), S(t, "%", Lr), S(t, "|", Rr), S(t, "+", Pr), S(t, "#", Br), S(t, "?", zr), S(t, '"', Ps), S(t, "/", ze), S(t, ";", Bs), S(t, "~", In), S(t, "_", Hr), S(t, "\\", Or);
+    let r = Me(t, Ss, Is, {
+        [ws]: !0
     });
-    $e(r, Hs, r);
-    let i = $e(t, Kn, Mt, {
-        [Vs]: !0
+    Me(r, Ss, r);
+    let i = Me(t, Zt, Ke, {
+        [Ts]: !0
     });
-    $e(i, Kn, i);
-    let o = $e(t, Bs, qs, {
-        [$s]: !0
+    Me(i, Zt, i);
+    let s = Me(t, ks, Os, {
+        [Cs]: !0
     });
-    $e(o, Kn), $e(o, Bs, o);
-    let s = $e(t, Iu, Hu, {
-        [Au]: !0
+    Me(s, Zt), Me(s, ks, s);
+    let o = Me(t, $a, _a, {
+        [Fa]: !0
     });
-    M(t, Du, _s, {
-        [Au]: !0
-    }), M(s, Du), $e(s, Iu, s);
-    let l = $e(t, zs, Fu, {
-        [zu]: !0
+    S(t, Va, Ds, {
+        [Fa]: !0
+    }), S(o, Va), Me(o, $a, o);
+    let l = Me(t, Ms, Ga, {
+        [Ua]: !0
     });
-    $e(l, zs, l), M(l, Cg, l);
-    let a = M(l, Og);
-    $e(a, zs, l);
+    Me(l, Ms, l), S(l, Xh, l);
+    let a = S(l, Zh);
+    Me(a, Ms, l);
     let c = [
-            [Kn, i]
+            [Zt, i]
         ],
         u = [
-            [Kn, null],
-            [Bs, o]
+            [Zt, null],
+            [ks, s]
         ];
-    for (let d = 0; d < ki.length; d++) Vt(t, ki[d], Js, Mt, c);
-    for (let d = 0; d < vi.length; d++) Vt(t, vi[d], Ks, qs, u);
-    kn(Js, {
+    for (let d = 0; d < Mr.length; d++) lt(t, Mr[d], vs, Ke, c);
+    for (let d = 0; d < Sr.length; d++) lt(t, Sr[d], Ns, Os, u);
+    Dt(vs, {
         tld: !0,
         ascii: !0
-    }, e), kn(Ks, {
+    }, e), Dt(Ns, {
         utld: !0,
         alpha: !0
-    }, e), Vt(t, "file", Ei, Mt, c), Vt(t, "mailto", Ei, Mt, c), Vt(t, "http", Un, Mt, c), Vt(t, "https", Un, Mt, c), Vt(t, "ftp", Un, Mt, c), Vt(t, "ftps", Un, Mt, c), kn(Ei, {
+    }, e), lt(t, "file", wr, Ke, c), lt(t, "mailto", wr, Ke, c), lt(t, "http", en, Ke, c), lt(t, "https", en, Ke, c), lt(t, "ftp", en, Ke, c), lt(t, "ftps", en, Ke, c), Dt(wr, {
         scheme: !0,
         ascii: !0
-    }, e), kn(Un, {
+    }, e), Dt(en, {
         slashscheme: !0,
         ascii: !0
     }, e), n = n.sort((d, f) => d[0] > f[0] ? 1 : -1);
     for (let d = 0; d < n.length; d++) {
         let f = n[d][0],
-            h = n[d][1] ? {
-                [Eg]: !0
+            p = n[d][1] ? {
+                [_h]: !0
             } : {
-                [Sg]: !0
+                [Gh]: !0
             };
-        f.indexOf("-") >= 0 ? h[Ws] = !0 : Kn.test(f) ? Hs.test(f) ? h[Mi] = !0 : h[Vs] = !0 : h[js] = !0, Nu(t, f, f, h)
+        f.indexOf("-") >= 0 ? p[As] = !0 : Zt.test(f) ? Ss.test(f) ? p[Er] = !0 : p[Ts] = !0 : p[ws] = !0, ja(t, f, f, p)
     }
-    return Nu(t, "localhost", Nr, {
+    return ja(t, "localhost", Dn, {
         ascii: !0
-    }), t.jd = new Oe(Hi), {
+    }), t.jd = new he(Fr), {
         start: t,
-        tokens: Qn({
+        tokens: sn({
             groups: e
-        }, ju)
+        }, Qa)
     }
 }
 
-function Ng(n, e) {
-    let t = Ig(e.replace(/[A-Z]/g, l => l.toLowerCase())),
+function tp(n, e) {
+    let t = np(e.replace(/[A-Z]/g, l => l.toLowerCase())),
         r = t.length,
         i = [],
-        o = 0,
-        s = 0;
-    for (; s < r;) {
+        s = 0,
+        o = 0;
+    for (; o < r;) {
         let l = n,
             a = null,
             c = 0,
             u = null,
             d = -1,
             f = -1;
-        for (; s < r && (a = l.go(t[s]));) l = a, l.accepts() ? (d = 0, f = 0, u = l) : d >= 0 && (d += t[s].length, f++), c += t[s].length, o += t[s].length, s++;
-        o -= d, s -= f, c -= d, i.push({
+        for (; o < r && (a = l.go(t[o]));) l = a, l.accepts() ? (d = 0, f = 0, u = l) : d >= 0 && (d += t[o].length, f++), c += t[o].length, s += t[o].length, o++;
+        s -= d, o -= f, c -= d, i.push({
             t: u.t,
-            v: e.slice(o - c, o),
-            s: o - c,
-            e: o
+            v: e.slice(s - c, s),
+            s: s - c,
+            e: s
         })
     }
     return i
 }
 
-function Ig(n) {
+function np(n) {
     let e = [],
         t = n.length,
         r = 0;
     for (; r < t;) {
         let i = n.charCodeAt(r),
-            o, s = i < 55296 || i > 56319 || r + 1 === t || (o = n.charCodeAt(r + 1)) < 56320 || o > 57343 ? n[r] : n.slice(r, r + 2);
-        e.push(s), r += s.length
+            s, o = i < 55296 || i > 56319 || r + 1 === t || (s = n.charCodeAt(r + 1)) < 56320 || s > 57343 ? n[r] : n.slice(r, r + 2);
+        e.push(o), r += o.length
     }
     return e
 }
 
-function Vt(n, e, t, r, i) {
-    let o, s = e.length;
-    for (let l = 0; l < s - 1; l++) {
+function lt(n, e, t, r, i) {
+    let s, o = e.length;
+    for (let l = 0; l < o - 1; l++) {
         let a = e[l];
-        n.j[a] ? o = n.j[a] : (o = new Oe(r), o.jr = i.slice(), n.j[a] = o), n = o
+        n.j[a] ? s = n.j[a] : (s = new he(r), s.jr = i.slice(), n.j[a] = s), n = s
     }
-    return o = new Oe(t), o.jr = i.slice(), n.j[e[s - 1]] = o, o
+    return s = new he(t), s.jr = i.slice(), n.j[e[o - 1]] = s, s
 }
 
-function Lu(n) {
+function Ja(n) {
     let e = [],
         t = [],
         r = 0,
         i = "0123456789";
     for (; r < n.length;) {
-        let o = 0;
-        for (; i.indexOf(n[r + o]) >= 0;) o++;
-        if (o > 0) {
+        let s = 0;
+        for (; i.indexOf(n[r + s]) >= 0;) s++;
+        if (s > 0) {
             e.push(t.join(""));
-            for (let s = parseInt(n.substring(r, r + o), 10); s > 0; s--) t.pop();
-            r += o
+            for (let o = parseInt(n.substring(r, r + s), 10); o > 0; o--) t.pop();
+            r += s
         } else t.push(n[r]), r++
     }
     return e
 }
-var Ir = {
+var Ln = {
     defaultProtocol: "http",
     events: null,
-    format: Pu,
-    formatHref: Pu,
+    format: Wa,
+    formatHref: Wa,
     nl2br: !1,
     tagName: "a",
     target: null,
     rel: null,
     validate: !0,
     truncate: 1 / 0,
     className: null,
     attributes: null,
     ignoreTags: [],
     render: null
 };
 
-function Zs(n, e) {
+function zs(n, e) {
     e === void 0 && (e = null);
-    let t = Qn({}, Ir);
-    n && (t = Qn(t, n instanceof Zs ? n.o : n));
+    let t = sn({}, Ln);
+    n && (t = sn(t, n instanceof zs ? n.o : n));
     let r = t.ignoreTags,
         i = [];
-    for (let o = 0; o < r.length; o++) i.push(r[o].toUpperCase());
+    for (let s = 0; s < r.length; s++) i.push(r[s].toUpperCase());
     this.o = t, e && (this.defaultRender = e), this.ignoreTags = i
 }
-Zs.prototype = {
-    o: Ir,
+zs.prototype = {
+    o: Ln,
     ignoreTags: [],
     defaultRender(n) {
         return n
     },
     check(n) {
         return this.get("validate", n.toString(), n)
     },
     get(n, e, t) {
         let r = e != null,
             i = this.o[n];
-        return i && (typeof i == "object" ? (i = t.t in i ? i[t.t] : Ir[n], typeof i == "function" && r && (i = i(e, t))) : typeof i == "function" && r && (i = i(e, t.t, t)), i)
+        return i && (typeof i == "object" ? (i = t.t in i ? i[t.t] : Ln[n], typeof i == "function" && r && (i = i(e, t))) : typeof i == "function" && r && (i = i(e, t.t, t)), i)
     },
     getObj(n, e, t) {
         let r = this.o[n];
         return typeof r == "function" && e != null && (r = r(e, t.t, t)), r
     },
     render(n) {
         let e = n.render(this);
         return (this.get("render", null, n) || this.defaultRender)(e, n.t, n)
     }
 };
 
-function Pu(n) {
+function Wa(n) {
     return n
 }
 
-function Vu(n, e) {
+function Ya(n, e) {
     this.t = "token", this.v = n, this.tk = e
 }
-Vu.prototype = {
+Ya.prototype = {
     isLink: !1,
     toString() {
         return this.v
     },
     toHref(n) {
         return this.toString()
     },
@@ -13466,15 +12236,15 @@
     startIndex() {
         return this.tk[0].s
     },
     endIndex() {
         return this.tk[this.tk.length - 1].e
     },
     toObject(n) {
-        return n === void 0 && (n = Ir.defaultProtocol), {
+        return n === void 0 && (n = Ln.defaultProtocol), {
             type: this.t,
             value: this.toString(),
             isLink: this.isLink,
             href: this.toHref(n),
             start: this.startIndex(),
             end: this.endIndex()
         }
@@ -13493,318 +12263,318 @@
         return n.get("validate", this.toString(), this)
     },
     render(n) {
         let e = this,
             t = this.toHref(n.get("defaultProtocol")),
             r = n.get("formatHref", t, this),
             i = n.get("tagName", t, e),
-            o = this.toFormattedString(n),
-            s = {},
+            s = this.toFormattedString(n),
+            o = {},
             l = n.get("className", t, e),
             a = n.get("target", t, e),
             c = n.get("rel", t, e),
             u = n.getObj("attributes", t, e),
             d = n.getObj("events", t, e);
-        return s.href = r, l && (s.class = l), a && (s.target = a), c && (s.rel = c), u && Qn(s, u), {
+        return o.href = r, l && (o.class = l), a && (o.target = a), c && (o.rel = c), u && sn(o, u), {
             tagName: i,
-            attributes: s,
-            content: o,
+            attributes: o,
+            content: s,
             eventListeners: d
         }
     }
 };
 
-function Fi(n, e) {
-    class t extends Vu {
-        constructor(i, o) {
-            super(i, o), this.t = n
+function jr(n, e) {
+    class t extends Ya {
+        constructor(i, s) {
+            super(i, s), this.t = n
         }
     }
     for (let r in e) t.prototype[r] = e[r];
     return t.t = n, t
 }
-var Ru = Fi("email", {
+var qa = jr("email", {
         isLink: !0,
         toHref() {
             return "mailto:" + this.toString()
         }
     }),
-    Bu = Fi("text"),
-    Dg = Fi("nl"),
-    yn = Fi("url", {
+    Ka = jr("text"),
+    rp = jr("nl"),
+    vt = jr("url", {
         isLink: !0,
         toHref(n) {
-            return n === void 0 && (n = Ir.defaultProtocol), this.hasProtocol() ? this.v : `${n}://${this.v}`
+            return n === void 0 && (n = Ln.defaultProtocol), this.hasProtocol() ? this.v : `${n}://${this.v}`
         },
         hasProtocol() {
             let n = this.tk;
-            return n.length >= 2 && n[0].t !== Nr && n[1].t === Wt
+            return n.length >= 2 && n[0].t !== Dn && n[1].t === ct
         }
     });
-var ue = n => new Oe(n);
+var X = n => new he(n);
 
-function Lg(n) {
+function ip(n) {
     let {
         groups: e
-    } = n, t = e.domain.concat([Si, Ti, $t, Ci, Oi, Ai, Ni, Ii, at, Us, Di, Li, Pi, Ri, ct, Hi, Ar, zi]), r = [wi, Yn, xn, Gn, bn, Wt, Gs, lt, Ys, Cr, _n, Tr, Or, Bi, Qs, Xs], i = [Si, wi, Ti, Ci, Oi, Ai, xn, Ni, Ii, at, _n, Di, Li, Pi, Ri, Bi, ct, Hi, Ar, zi], o = ue(), s = M(o, Ar);
-    N(s, i, s), N(s, e.domain, s);
-    let l = ue(),
-        a = ue(),
-        c = ue();
-    N(o, e.domain, l), N(o, e.scheme, a), N(o, e.slashscheme, c), N(l, i, s), N(l, e.domain, l);
-    let u = M(l, $t);
-    M(s, $t, u), M(a, $t, u), M(c, $t, u);
-    let d = M(s, lt);
-    N(d, i, s), N(d, e.domain, s);
-    let f = ue();
-    N(u, e.domain, f), N(f, e.domain, f);
-    let p = M(f, lt);
-    N(p, e.domain, f);
-    let h = ue(Ru);
-    N(p, e.tld, h), N(p, e.utld, h), M(u, Nr, h);
-    let m = M(f, at);
-    N(m, e.domain, f), N(h, e.domain, f), M(h, lt, p), M(h, at, m);
-    let b = M(h, Wt);
-    N(b, e.numeric, Ru);
-    let k = M(l, at),
-        S = M(l, lt);
-    N(k, e.domain, l), N(S, i, s), N(S, e.domain, l);
-    let C = ue(yn);
-    N(S, e.tld, C), N(S, e.utld, C), N(C, e.domain, l), N(C, i, s), M(C, lt, S), M(C, at, k), M(C, $t, u);
-    let T = M(C, Wt),
-        E = ue(yn);
-    N(T, e.numeric, E);
-    let g = ue(yn),
-        x = ue();
-    N(g, t, g), N(g, r, x), N(x, t, g), N(x, r, x), M(C, ct, g), M(E, ct, g);
-    let y = M(a, Wt),
-        O = M(c, Wt),
-        I = M(O, ct),
-        L = M(I, ct);
-    N(a, e.domain, l), M(a, lt, S), M(a, at, k), N(c, e.domain, l), M(c, lt, S), M(c, at, k), N(y, e.domain, g), M(y, ct, g), N(L, e.domain, g), N(L, t, g), M(L, ct, g);
-    let j = M(g, _n),
-        ee = M(g, Tr),
-        Ne = M(g, Cr),
-        Ie = M(g, Or);
-    M(x, _n, j), M(x, Tr, ee), M(x, Cr, Ne), M(x, Or, Ie), M(j, xn, g), M(ee, Gn, g), M(Ne, Yn, g), M(Ie, bn, g), M(j, xn, g);
-    let te = ue(yn),
-        ie = ue(yn),
-        De = ue(yn),
-        xe = ue(yn);
-    N(j, t, te), N(ee, t, ie), N(Ne, t, De), N(Ie, t, xe);
-    let Ge = ue(),
-        Et = ue(),
-        Ye = ue(),
-        ut = ue();
-    return N(j, r), N(ee, r), N(Ne, r), N(Ie, r), N(te, t, te), N(ie, t, ie), N(De, t, De), N(xe, t, xe), N(te, r, te), N(ie, r, ie), N(De, r, De), N(xe, r, xe), N(Ge, t, Ge), N(Et, t, ie), N(Ye, t, De), N(ut, t, xe), N(Ge, r, Ge), N(Et, r, Et), N(Ye, r, Ye), N(ut, r, ut), M(ie, Gn, g), M(De, Yn, g), M(xe, bn, g), M(te, xn, g), M(Et, Gn, g), M(Ye, Yn, g), M(ut, bn, g), M(Ge, bn, g), M(o, Nr, C), M(o, _s, Dg), {
-        start: o,
-        tokens: ju
+    } = n, t = e.domain.concat([Tr, Ar, at, Or, vr, Nr, Ir, Dr, Be, Is, Lr, Rr, Pr, Br, ze, Fr, In, Hr]), r = [Cr, rn, Nt, nn, It, ct, Ls, Pe, Rs, vn, tn, On, Nn, zr, Ps, Bs], i = [Tr, Cr, Ar, Or, vr, Nr, Nt, Ir, Dr, Be, tn, Lr, Rr, Pr, Br, zr, ze, Fr, In, Hr], s = X(), o = S(s, In);
+    C(o, i, o), C(o, e.domain, o);
+    let l = X(),
+        a = X(),
+        c = X();
+    C(s, e.domain, l), C(s, e.scheme, a), C(s, e.slashscheme, c), C(l, i, o), C(l, e.domain, l);
+    let u = S(l, at);
+    S(o, at, u), S(a, at, u), S(c, at, u);
+    let d = S(o, Pe);
+    C(d, i, o), C(d, e.domain, o);
+    let f = X();
+    C(u, e.domain, f), C(f, e.domain, f);
+    let h = S(f, Pe);
+    C(h, e.domain, f);
+    let p = X(qa);
+    C(h, e.tld, p), C(h, e.utld, p), S(u, Dn, p);
+    let m = S(f, Be);
+    C(m, e.domain, f), C(p, e.domain, f), S(p, Pe, h), S(p, Be, m);
+    let b = S(p, ct);
+    C(b, e.numeric, qa);
+    let M = S(l, Be),
+        w = S(l, Pe);
+    C(M, e.domain, l), C(w, i, o), C(w, e.domain, l);
+    let v = X(vt);
+    C(w, e.tld, v), C(w, e.utld, v), C(v, e.domain, l), C(v, i, o), S(v, Pe, w), S(v, Be, M), S(v, at, u);
+    let D = S(v, ct),
+        A = X(vt);
+    C(D, e.numeric, A);
+    let g = X(vt),
+        k = X();
+    C(g, t, g), C(g, r, k), C(k, t, g), C(k, r, k), S(v, ze, g), S(A, ze, g);
+    let y = S(a, ct),
+        N = S(c, ct),
+        z = S(N, ze),
+        Q = S(z, ze);
+    C(a, e.domain, l), S(a, Pe, w), S(a, Be, M), C(c, e.domain, l), S(c, Pe, w), S(c, Be, M), C(y, e.domain, g), S(y, ze, g), C(Q, e.domain, g), C(Q, t, g), S(Q, ze, g);
+    let ln = S(g, tn),
+        Pn = S(g, On),
+        Bn = S(g, vn),
+        zn = S(g, Nn);
+    S(k, tn, ln), S(k, On, Pn), S(k, vn, Bn), S(k, Nn, zn), S(ln, Nt, g), S(Pn, nn, g), S(Bn, rn, g), S(zn, It, g), S(ln, Nt, g);
+    let Lt = X(vt),
+        ut = X(vt),
+        dt = X(vt),
+        ft = X(vt);
+    C(ln, t, Lt), C(Pn, t, ut), C(Bn, t, dt), C(zn, t, ft);
+    let an = X(),
+        Hn = X(),
+        Fn = X(),
+        jn = X();
+    return C(ln, r), C(Pn, r), C(Bn, r), C(zn, r), C(Lt, t, Lt), C(ut, t, ut), C(dt, t, dt), C(ft, t, ft), C(Lt, r, Lt), C(ut, r, ut), C(dt, r, dt), C(ft, r, ft), C(an, t, an), C(Hn, t, ut), C(Fn, t, dt), C(jn, t, ft), C(an, r, an), C(Hn, r, Hn), C(Fn, r, Fn), C(jn, r, jn), S(ut, nn, g), S(dt, rn, g), S(ft, It, g), S(Lt, Nt, g), S(Hn, nn, g), S(Fn, rn, g), S(jn, It, g), S(an, It, g), S(s, Dn, v), S(s, Ds, rp), {
+        start: s,
+        tokens: Qa
     }
 }
 
-function Pg(n, e, t) {
+function sp(n, e, t) {
     let r = t.length,
         i = 0,
-        o = [],
-        s = [];
+        s = [],
+        o = [];
     for (; i < r;) {
         let l = n,
             a = null,
             c = null,
             u = 0,
             d = null,
             f = -1;
-        for (; i < r && !(a = l.go(t[i].t));) s.push(t[i++]);
+        for (; i < r && !(a = l.go(t[i].t));) o.push(t[i++]);
         for (; i < r && (c = a || l.go(t[i].t));) a = null, l = c, l.accepts() ? (f = 0, d = l) : f >= 0 && f++, i++, u++;
-        if (f < 0) i -= u, i < r && (s.push(t[i]), i++);
+        if (f < 0) i -= u, i < r && (o.push(t[i]), i++);
         else {
-            s.length > 0 && (o.push(Fs(Bu, e, s)), s = []), i -= f, u -= f;
-            let p = d.t,
-                h = t.slice(i - u, i);
-            o.push(Fs(p, e, h))
+            o.length > 0 && (s.push(Es(Ka, e, o)), o = []), i -= f, u -= f;
+            let h = d.t,
+                p = t.slice(i - u, i);
+            s.push(Es(h, e, p))
         }
     }
-    return s.length > 0 && o.push(Fs(Bu, e, s)), o
+    return o.length > 0 && s.push(Es(Ka, e, o)), s
 }
 
-function Fs(n, e, t) {
+function Es(n, e, t) {
     let r = t[0].s,
         i = t[t.length - 1].e,
-        o = e.slice(r, i);
-    return new n(o, t)
+        s = e.slice(r, i);
+    return new n(s, t)
 }
-var Rg = typeof console < "u" && console && console.warn || (() => {}),
-    Bg = "until manual call of linkify.init(). Register all schemes and plugins before invoking linkify the first time.",
-    K = {
+var op = typeof console < "u" && console && console.warn || (() => {}),
+    lp = "until manual call of linkify.init(). Register all schemes and plugins before invoking linkify the first time.",
+    J = {
         scanner: null,
         parser: null,
         tokenQueue: [],
         pluginQueue: [],
         customSchemes: [],
         initialized: !1
     };
 
-function $u() {
-    Oe.groups = {}, K.scanner = null, K.parser = null, K.tokenQueue = [], K.pluginQueue = [], K.customSchemes = [], K.initialized = !1
+function Xa() {
+    he.groups = {}, J.scanner = null, J.parser = null, J.tokenQueue = [], J.pluginQueue = [], J.customSchemes = [], J.initialized = !1
 }
 
-function el(n, e) {
-    if (e === void 0 && (e = !1), K.initialized && Rg(`linkifyjs: already initialized - will not register custom scheme "${n}" ${Bg}`), !/^[0-9a-z]+(-[0-9a-z]+)*$/.test(n)) throw new Error(`linkifyjs: incorrect scheme format.
+function Hs(n, e) {
+    if (e === void 0 && (e = !1), J.initialized && op(`linkifyjs: already initialized - will not register custom scheme "${n}" ${lp}`), !/^[0-9a-z]+(-[0-9a-z]+)*$/.test(n)) throw new Error(`linkifyjs: incorrect scheme format.
  1. Must only contain digits, lowercase ASCII letters or "-"
  2. Cannot start or end with "-"
  3. "-" cannot repeat`);
-    K.customSchemes.push([n, e])
+    J.customSchemes.push([n, e])
 }
 
-function zg() {
-    K.scanner = Ag(K.customSchemes);
-    for (let n = 0; n < K.tokenQueue.length; n++) K.tokenQueue[n][1]({
-        scanner: K.scanner
+function ap() {
+    J.scanner = ep(J.customSchemes);
+    for (let n = 0; n < J.tokenQueue.length; n++) J.tokenQueue[n][1]({
+        scanner: J.scanner
     });
-    K.parser = Lg(K.scanner.tokens);
-    for (let n = 0; n < K.pluginQueue.length; n++) K.pluginQueue[n][1]({
-        scanner: K.scanner,
-        parser: K.parser
+    J.parser = ip(J.scanner.tokens);
+    for (let n = 0; n < J.pluginQueue.length; n++) J.pluginQueue[n][1]({
+        scanner: J.scanner,
+        parser: J.parser
     });
-    K.initialized = !0
+    J.initialized = !0
 }
 
-function Wu(n) {
-    return K.initialized || zg(), Pg(K.parser.start, n, Ng(K.scanner.start, n))
+function Za(n) {
+    return J.initialized || ap(), sp(J.parser.start, n, tp(J.scanner.start, n))
 }
 
-function ji(n, e, t) {
+function $r(n, e, t) {
     if (e === void 0 && (e = null), t === void 0 && (t = null), e && typeof e == "object") {
         if (t) throw Error(`linkifyjs: Invalid link type ${e}; must be a string`);
         t = e, e = null
     }
-    let r = new Zs(t),
-        i = Wu(n),
-        o = [];
-    for (let s = 0; s < i.length; s++) {
-        let l = i[s];
-        l.isLink && (!e || l.t === e) && o.push(l.toFormattedObject(r))
+    let r = new zs(t),
+        i = Za(n),
+        s = [];
+    for (let o = 0; o < i.length; o++) {
+        let l = i[o];
+        l.isLink && (!e || l.t === e) && s.push(l.toFormattedObject(r))
     }
-    return o
+    return s
 }
 
-function tl(n, e) {
+function Fs(n, e) {
     e === void 0 && (e = null);
-    let t = Wu(n);
+    let t = Za(n);
     return t.length === 1 && t[0].isLink && (!e || t[0].t === e)
 }
 
-function Hg(n) {
-    return new q({
-        key: new Z("autolink"),
+function cp(n) {
+    return new $({
+        key: new U("autolink"),
         appendTransaction: (e, t, r) => {
             let i = e.some(u => u.docChanged) && !t.doc.eq(r.doc),
-                o = e.some(u => u.getMeta("preventAutolink"));
-            if (!i || o) return;
+                s = e.some(u => u.getMeta("preventAutolink"));
+            if (!i || s) return;
             let {
-                tr: s
-            } = r, l = au(t.doc, [...e]), {
+                tr: o
+            } = r, l = ba(t.doc, [...e]), {
                 mapping: a
             } = l;
-            if (uu(l).forEach(({
+            if (ka(l).forEach(({
                     oldRange: u,
                     newRange: d
                 }) => {
-                    Sr(u.from, u.to, t.doc).filter(m => m.mark.type === n.type).forEach(m => {
+                    Cn(u.from, u.to, t.doc).filter(m => m.mark.type === n.type).forEach(m => {
                         let b = a.map(m.from),
-                            k = a.map(m.to),
-                            S = Sr(b, k, r.doc).filter(y => y.mark.type === n.type);
-                        if (!S.length) return;
-                        let C = S[0],
-                            T = t.doc.textBetween(m.from, m.to, void 0, " "),
-                            E = r.doc.textBetween(C.from, C.to, void 0, " "),
-                            g = tl(T),
-                            x = tl(E);
-                        g && !x && s.removeMark(C.from, C.to, n.type)
+                            M = a.map(m.to),
+                            w = Cn(b, M, r.doc).filter(y => y.mark.type === n.type);
+                        if (!w.length) return;
+                        let v = w[0],
+                            D = t.doc.textBetween(m.from, m.to, void 0, " "),
+                            A = r.doc.textBetween(v.from, v.to, void 0, " "),
+                            g = Fs(D),
+                            k = Fs(A);
+                        g && !k && o.removeMark(v.from, v.to, n.type)
                     });
-                    let f = cu(r.doc, d, m => m.isTextblock),
-                        p, h;
-                    if (f.length > 1 ? (p = f[0], h = r.doc.textBetween(p.pos, p.pos + p.node.nodeSize, void 0, " ")) : f.length && r.doc.textBetween(d.from, d.to, " ", " ").endsWith(" ") && (p = f[0], h = r.doc.textBetween(p.pos, d.to, void 0, " ")), p && h) {
-                        let m = h.split(" ").filter(S => S !== "");
+                    let f = xa(r.doc, d, m => m.isTextblock),
+                        h, p;
+                    if (f.length > 1 ? (h = f[0], p = r.doc.textBetween(h.pos, h.pos + h.node.nodeSize, void 0, " ")) : f.length && r.doc.textBetween(d.from, d.to, " ", " ").endsWith(" ") && (h = f[0], p = r.doc.textBetween(h.pos, d.to, void 0, " ")), h && p) {
+                        let m = p.split(" ").filter(w => w !== "");
                         if (m.length <= 0) return !1;
                         let b = m[m.length - 1],
-                            k = p.pos + h.lastIndexOf(b);
+                            M = h.pos + p.lastIndexOf(b);
                         if (!b) return !1;
-                        ji(b).filter(S => S.isLink).filter(S => n.validate ? n.validate(S.value) : !0).map(S => ({
-                            ...S,
-                            from: k + S.start + 1,
-                            to: k + S.end + 1
-                        })).forEach(S => {
-                            s.addMark(S.from, S.to, n.type.create({
-                                href: S.href
+                        $r(b).filter(w => w.isLink).filter(w => n.validate ? n.validate(w.value) : !0).map(w => ({
+                            ...w,
+                            from: M + w.start + 1,
+                            to: M + w.end + 1
+                        })).forEach(w => {
+                            o.addMark(w.from, w.to, n.type.create({
+                                href: w.href
                             }))
                         })
                     }
-                }), !!s.steps.length) return s
+                }), !!o.steps.length) return o
         }
     })
 }
 
-function Fg(n) {
-    return new q({
-        key: new Z("handleClickLink"),
+function up(n) {
+    return new $({
+        key: new U("handleClickLink"),
         props: {
             handleClick: (e, t, r) => {
-                var i, o, s;
+                var i, s, o;
                 if (r.button !== 0) return !1;
-                let l = As(e.state, n.type.name),
+                let l = hs(e.state, n.type.name),
                     a = (i = r.target) === null || i === void 0 ? void 0 : i.closest("a"),
-                    c = (o = a == null ? void 0 : a.href) !== null && o !== void 0 ? o : l.href,
-                    u = (s = a == null ? void 0 : a.target) !== null && s !== void 0 ? s : l.target;
+                    c = (s = a == null ? void 0 : a.href) !== null && s !== void 0 ? s : l.href,
+                    u = (o = a == null ? void 0 : a.target) !== null && o !== void 0 ? o : l.target;
                 return a && c ? (window.open(c, u), !0) : !1
             }
         }
     })
 }
 
-function jg(n) {
-    return new q({
-        key: new Z("handlePasteLink"),
+function dp(n) {
+    return new $({
+        key: new U("handlePasteLink"),
         props: {
             handlePaste: (e, t, r) => {
                 let {
                     state: i
                 } = e, {
-                    selection: o
+                    selection: s
                 } = i, {
-                    empty: s
-                } = o;
-                if (s) return !1;
+                    empty: o
+                } = s;
+                if (o) return !1;
                 let l = "";
                 r.content.forEach(c => {
                     l += c.textContent
                 });
-                let a = ji(l).find(c => c.isLink && c.value === l);
+                let a = $r(l).find(c => c.isLink && c.value === l);
                 return !l || !a ? !1 : (n.editor.commands.setMark(n.type, {
                     href: a.href
                 }), !0)
             }
         }
     })
 }
-var qu = V.create({
+var ec = F.create({
     name: "link",
     priority: 1e3,
     keepOnSplit: !1,
     onCreate() {
         this.options.protocols.forEach(n => {
             if (typeof n == "string") {
-                el(n);
+                Hs(n);
                 return
             }
-            el(n.scheme, n.optionalSlashes)
+            Hs(n.scheme, n.optionalSlashes)
         })
     },
     onDestroy() {
-        $u()
+        Xa()
     },
     inclusive() {
         return this.options.autolink
     },
     addOptions() {
         return {
             openOnClick: !0,
@@ -13836,15 +12606,15 @@
         return [{
             tag: 'a[href]:not([href *= "javascript:" i])'
         }]
     },
     renderHTML({
         HTMLAttributes: n
     }) {
-        return ["a", z(this.options.HTMLAttributes, n), 0]
+        return ["a", P(this.options.HTMLAttributes, n), 0]
     },
     addCommands() {
         return {
             setLink: n => ({
                 chain: e
             }) => e().setMark(this.name, n).setMeta("preventAutolink", !0).run(),
             toggleLink: n => ({
@@ -13856,16 +12626,16 @@
                 chain: n
             }) => n().unsetMark(this.name, {
                 extendEmptyMarkRange: !0
             }).setMeta("preventAutolink", !0).run()
         }
     },
     addPasteRules() {
-        return [Ft({
-            find: n => ji(n).filter(e => this.options.validate ? this.options.validate(e.value) : !0).filter(e => e.isLink).map(e => ({
+        return [st({
+            find: n => $r(n).filter(e => this.options.validate ? this.options.validate(e.value) : !0).filter(e => e.isLink).map(e => ({
                 text: e.value,
                 index: e.start,
                 data: e
             })),
             type: this.type,
             getAttributes: n => {
                 var e;
@@ -13873,26 +12643,26 @@
                     href: (e = n.data) === null || e === void 0 ? void 0 : e.href
                 }
             }
         })]
     },
     addProseMirrorPlugins() {
         let n = [];
-        return this.options.autolink && n.push(Hg({
+        return this.options.autolink && n.push(cp({
             type: this.type,
             validate: this.options.validate
-        })), this.options.openOnClick && n.push(Fg({
+        })), this.options.openOnClick && n.push(up({
             type: this.type
-        })), this.options.linkOnPaste && n.push(jg({
+        })), this.options.linkOnPaste && n.push(dp({
             editor: this.editor,
             type: this.type
         })), n
     }
 });
-var nl = F.create({
+var js = H.create({
     name: "listItem",
     addOptions() {
         return {
             HTMLAttributes: {}
         }
     },
     content: "paragraph block*",
@@ -13901,25 +12671,25 @@
         return [{
             tag: "li"
         }]
     },
     renderHTML({
         HTMLAttributes: n
     }) {
-        return ["li", z(this.options.HTMLAttributes, n), 0]
+        return ["li", P(this.options.HTMLAttributes, n), 0]
     },
     addKeyboardShortcuts() {
         return {
             Enter: () => this.editor.commands.splitListItem(this.name),
             Tab: () => this.editor.commands.sinkListItem(this.name),
             "Shift-Tab": () => this.editor.commands.liftListItem(this.name)
         }
     }
 });
-var Vg = F.create({
+var fp = H.create({
         name: "listItem",
         addOptions() {
             return {
                 HTMLAttributes: {}
             }
         },
         content: "paragraph block*",
@@ -13928,25 +12698,25 @@
             return [{
                 tag: "li"
             }]
         },
         renderHTML({
             HTMLAttributes: n
         }) {
-            return ["li", z(this.options.HTMLAttributes, n), 0]
+            return ["li", P(this.options.HTMLAttributes, n), 0]
         },
         addKeyboardShortcuts() {
             return {
                 Enter: () => this.editor.commands.splitListItem(this.name),
                 Tab: () => this.editor.commands.sinkListItem(this.name),
                 "Shift-Tab": () => this.editor.commands.liftListItem(this.name)
             }
         }
     }),
-    Ju = V.create({
+    tc = F.create({
         name: "textStyle",
         addOptions() {
             return {
                 HTMLAttributes: {}
             }
         },
         parseHTML() {
@@ -13954,30 +12724,30 @@
                 tag: "span",
                 getAttrs: n => n.hasAttribute("style") ? {} : !1
             }]
         },
         renderHTML({
             HTMLAttributes: n
         }) {
-            return ["span", z(this.options.HTMLAttributes, n), 0]
+            return ["span", P(this.options.HTMLAttributes, n), 0]
         },
         addCommands() {
             return {
                 removeEmptyTextStyle: () => ({
                     state: n,
                     commands: e
                 }) => {
-                    let t = qn(n, this.type);
+                    let t = Yt(n, this.type);
                     return Object.entries(t).some(([, i]) => !!i) ? !0 : e.unsetMark(this.name)
                 }
             }
         }
     }),
-    Ku = /^(\d+)\.\s$/,
-    Uu = F.create({
+    nc = /^(\d+)\.\s$/,
+    rc = H.create({
         name: "orderedList",
         addOptions() {
             return {
                 itemTypeName: "listItem",
                 HTMLAttributes: {},
                 keepMarks: !1,
                 keepAttributes: !1
@@ -14003,53 +12773,53 @@
         renderHTML({
             HTMLAttributes: n
         }) {
             let {
                 start: e,
                 ...t
             } = n;
-            return e === 1 ? ["ol", z(this.options.HTMLAttributes, t), 0] : ["ol", z(this.options.HTMLAttributes, n), 0]
+            return e === 1 ? ["ol", P(this.options.HTMLAttributes, t), 0] : ["ol", P(this.options.HTMLAttributes, n), 0]
         },
         addCommands() {
             return {
                 toggleOrderedList: () => ({
                     commands: n,
                     chain: e
-                }) => this.options.keepAttributes ? e().toggleList(this.name, this.options.itemTypeName, this.options.keepMarks).updateAttributes(Vg.name, this.editor.getAttributes(Ju.name)).run() : n.toggleList(this.name, this.options.itemTypeName, this.options.keepMarks)
+                }) => this.options.keepAttributes ? e().toggleList(this.name, this.options.itemTypeName, this.options.keepMarks).updateAttributes(fp.name, this.editor.getAttributes(tc.name)).run() : n.toggleList(this.name, this.options.itemTypeName, this.options.keepMarks)
             }
         },
         addKeyboardShortcuts() {
             return {
                 "Mod-Shift-7": () => this.editor.commands.toggleOrderedList()
             }
         },
         addInputRules() {
-            let n = Ht({
-                find: Ku,
+            let n = it({
+                find: nc,
                 type: this.type,
                 getAttributes: e => ({
                     start: +e[1]
                 }),
                 joinPredicate: (e, t) => t.childCount + t.attrs.start === +e[1]
             });
-            return (this.options.keepMarks || this.options.keepAttributes) && (n = Ht({
-                find: Ku,
+            return (this.options.keepMarks || this.options.keepAttributes) && (n = it({
+                find: nc,
                 type: this.type,
                 keepMarks: this.options.keepMarks,
                 keepAttributes: this.options.keepAttributes,
                 getAttributes: e => ({
                     start: +e[1],
-                    ...this.editor.getAttributes(Ju.name)
+                    ...this.editor.getAttributes(tc.name)
                 }),
                 joinPredicate: (e, t) => t.childCount + t.attrs.start === +e[1],
                 editor: this.editor
             })), [n]
         }
     });
-var _u = F.create({
+var ic = H.create({
     name: "paragraph",
     priority: 1e3,
     addOptions() {
         return {
             HTMLAttributes: {}
         }
     },
@@ -14059,82 +12829,82 @@
         return [{
             tag: "p"
         }]
     },
     renderHTML({
         HTMLAttributes: n
     }) {
-        return ["p", z(this.options.HTMLAttributes, n), 0]
+        return ["p", P(this.options.HTMLAttributes, n), 0]
     },
     addCommands() {
         return {
             setParagraph: () => ({
                 commands: n
             }) => n.setNode(this.name)
         }
     },
     addKeyboardShortcuts() {
         return {
             "Mod-Alt-0": () => this.editor.commands.setParagraph()
         }
     }
 });
-var Gu = J.create({
+var sc = V.create({
     name: "placeholder",
     addOptions() {
         return {
             emptyEditorClass: "is-editor-empty",
             emptyNodeClass: "is-empty",
             placeholder: "Write something \u2026",
             showOnlyWhenEditable: !0,
             showOnlyCurrent: !0,
             includeChildren: !1
         }
     },
     addProseMirrorPlugins() {
-        return [new q({
-            key: new Z("placeholder"),
+        return [new $({
+            key: new U("placeholder"),
             props: {
                 decorations: ({
                     doc: n,
                     selection: e
                 }) => {
                     let t = this.editor.isEditable || !this.options.showOnlyWhenEditable,
                         {
                             anchor: r
                         } = e,
                         i = [];
                     if (!t) return null;
-                    let o = n.type.createAndFill(),
-                        s = (o == null ? void 0 : o.sameMarkup(n)) && o.content.findDiffStart(n.content) === null;
+                    let s = n.type.createAndFill(),
+                        o = (s == null ? void 0 : s.sameMarkup(n)) && s.content.findDiffStart(n.content) === null;
                     return n.descendants((l, a) => {
                         let c = r >= a && r <= a + l.nodeSize,
                             u = !l.isLeaf && !l.childCount;
                         if ((c || !this.options.showOnlyCurrent) && u) {
                             let d = [this.options.emptyNodeClass];
-                            s && d.push(this.options.emptyEditorClass);
-                            let f = ke.node(a, a + l.nodeSize, {
+                            o && d.push(this.options.emptyEditorClass);
+                            let f = se.node(a, a + l.nodeSize, {
                                 class: d.join(" "),
                                 "data-placeholder": typeof this.options.placeholder == "function" ? this.options.placeholder({
                                     editor: this.editor,
                                     node: l,
                                     pos: a,
                                     hasAnchor: c
                                 }) : this.options.placeholder
                             });
                             i.push(f)
                         }
                         return this.options.includeChildren
-                    }), G.create(n, i)
+                    }), W.create(n, i)
                 }
             }
         })]
     }
 });
-var Yu = V.create({
+var oc = F.create({
     name: "subscript",
     addOptions() {
         return {
             HTMLAttributes: {}
         }
     },
     parseHTML() {
@@ -14146,15 +12916,15 @@
                 return n !== "sub" ? !1 : null
             }
         }]
     },
     renderHTML({
         HTMLAttributes: n
     }) {
-        return ["sub", z(this.options.HTMLAttributes, n), 0]
+        return ["sub", P(this.options.HTMLAttributes, n), 0]
     },
     addCommands() {
         return {
             setSubscript: () => ({
                 commands: n
             }) => n.setMark(this.name),
             toggleSubscript: () => ({
@@ -14167,15 +12937,15 @@
     },
     addKeyboardShortcuts() {
         return {
             "Mod-,": () => this.editor.commands.toggleSubscript()
         }
     }
 });
-var Qu = V.create({
+var lc = F.create({
     name: "superscript",
     addOptions() {
         return {
             HTMLAttributes: {}
         }
     },
     parseHTML() {
@@ -14187,15 +12957,15 @@
                 return n !== "super" ? !1 : null
             }
         }]
     },
     renderHTML({
         HTMLAttributes: n
     }) {
-        return ["sup", z(this.options.HTMLAttributes, n), 0]
+        return ["sup", P(this.options.HTMLAttributes, n), 0]
     },
     addCommands() {
         return {
             setSuperscript: () => ({
                 commands: n
             }) => n.setMark(this.name),
             toggleSuperscript: () => ({
@@ -14208,19 +12978,19 @@
     },
     addKeyboardShortcuts() {
         return {
             "Mod-.": () => this.editor.commands.toggleSuperscript()
         }
     }
 });
-var Xu = F.create({
+var ac = H.create({
     name: "text",
     group: "inline"
 });
-var Zu = J.create({
+var cc = V.create({
     name: "textAlign",
     addOptions() {
         return {
             types: [],
             alignments: ["left", "center", "right", "justify"],
             defaultAlignment: "left"
         }
@@ -14256,15 +13026,15 @@
             "Mod-Shift-l": () => this.editor.commands.setTextAlign("left"),
             "Mod-Shift-e": () => this.editor.commands.setTextAlign("center"),
             "Mod-Shift-r": () => this.editor.commands.setTextAlign("right"),
             "Mod-Shift-j": () => this.editor.commands.setTextAlign("justify")
         }
     }
 });
-var ed = J.create({
+var uc = V.create({
     name: "textIndent",
     addOptions() {
         return {
             types: []
         }
     },
     addGlobalAttributes() {
@@ -14290,15 +13060,15 @@
             })),
             unsetTextIndent: () => ({
                 commands: n
             }) => this.options.types.every(e => n.resetAttributes(e, ["textIndent"]))
         }
     }
 });
-var td = J.create({
+var dc = V.create({
     name: "textMargin",
     addOptions() {
         return {
             types: [],
             maxIndentLevel: 8
         }
     },
@@ -14336,15 +13106,15 @@
             },
             unsetTextMargin: () => ({
                 commands: n
             }) => this.options.types.every(e => n.resetAttributes(e, ["textMargin"]))
         }
     }
 });
-var nd = V.create({
+var fc = F.create({
     name: "textColor",
     addOptions() {
         return {
             allowedClasses: []
         }
     },
     addAttributes() {
@@ -14391,15 +13161,15 @@
             }),
             unsetColor: () => ({
                 commands: n
             }) => n.unsetMark(this.name)
         }
     }
 });
-var rd = V.create({
+var hc = F.create({
     name: "procurator",
     keepOnSplit: !1,
     addOptions() {
         return {
             HTMLAttributes: {
                 role: "placeholder"
             }
@@ -14435,15 +13205,15 @@
                 chain: n
             }) => n().unsetMark(this.name, {
                 extendEmptyMarkRange: !0
             }).run()
         }
     }
 });
-var id = V.create({
+var pc = F.create({
     name: "underline",
     addOptions() {
         return {
             HTMLAttributes: {}
         }
     },
     parseHTML() {
@@ -14454,15 +13224,15 @@
             consuming: !1,
             getAttrs: n => n.includes("underline") ? {} : !1
         }]
     },
     renderHTML({
         HTMLAttributes: n
     }) {
-        return ["u", z(this.options.HTMLAttributes, n), 0]
+        return ["u", P(this.options.HTMLAttributes, n), 0]
     },
     addCommands() {
         return {
             setUnderline: () => ({
                 commands: n
             }) => n.setMark(this.name),
             toggleUnderline: () => ({
@@ -14476,16 +13246,16 @@
     addKeyboardShortcuts() {
         return {
             "Mod-u": () => this.editor.commands.toggleUnderline(),
             "Mod-U": () => this.editor.commands.toggleUnderline()
         }
     }
 });
-var sd = pd(hd()),
-    U = class {
+var gc = yc(bc()),
+    _ = class {
         constructor(e, t, r) {
             this.extensions = [];
             this.name = t, this.button = r
         }
         installEventHandler(e) {
             this.button.addEventListener("click", () => this.clicked(e))
         }
@@ -14497,445 +13267,429 @@
         }
         extendExtensions(e) {
             this.extensions.forEach(t => {
                 e.includes(t) || e.push(t)
             })
         }
     },
-    Xn;
-(C => {
-    class n extends U {
+    Rn = class extends _ {
+        constructor(t, r, i, s) {
+            super(t, r, i);
+            this.dropdownItems = [];
+            this.button.nextElementSibling instanceof HTMLUListElement && this.button.nextElementSibling.role === "menu" ? (this.dropdownMenu = this.button.nextElementSibling, this.dropdownItems = this.dropdownMenu.querySelectorAll(s)) : this.dropdownMenu = null
+        }
+        installEventHandler(t) {
+            this.dropdownMenu ? (this.button.addEventListener("click", () => this.toggleMenu(t)), this.dropdownMenu.addEventListener("click", r => this.toggleItem(r, t)), document.addEventListener("click", r => {
+                let i = r.target instanceof Element ? r.target : null;
+                for (; i;) {
+                    if (i.isSameNode(this.button) || i.isSameNode(this.dropdownMenu)) return;
+                    i = i.parentElement
+                }
+                this.toggleMenu(t, !1)
+            })) : this.button.addEventListener("click", r => this.toggleItem(r, t))
+        }
+        toggleMenu(t, r) {
+            if (this.dropdownMenu) {
+                let i = r !== !1 && this.button.ariaExpanded === "false";
+                this.button.ariaExpanded = i ? "true" : "false", Vs(this.button, this.dropdownMenu).then(({
+                    x: s,
+                    y: o
+                }) => Object.assign(this.dropdownMenu.style, {
+                    left: `${s}px`,
+                    top: `${o}px`
+                }))
+            }
+        }
+    },
+    on;
+(v => {
+    class n extends _ {
         constructor() {
             super(...arguments);
-            this.extensions = [fu]
+            this.extensions = [Sa]
         }
         clicked(g) {
             g.chain().focus().toggleBold().run(), this.activate(g)
         }
     }
-    C.BoldAction = n;
-    class e extends U {
+    v.BoldAction = n;
+    class e extends _ {
         constructor() {
             super(...arguments);
-            this.extensions = [Ou]
+            this.extensions = [Ha]
         }
         clicked(g) {
             g.chain().focus().toggleItalic().run(), this.activate(g)
         }
     }
-    C.ItalicAction = e;
-    class t extends U {
+    v.ItalicAction = e;
+    class t extends _ {
         constructor() {
             super(...arguments);
-            this.extensions = [Yu]
+            this.extensions = [oc]
         }
         clicked(g) {
             g.chain().focus().unsetSuperscript().run(), g.chain().focus().toggleSubscript().run(), this.activate(g)
         }
     }
-    C.SubscriptAction = t;
-    class r extends U {
+    v.SubscriptAction = t;
+    class r extends _ {
         constructor() {
             super(...arguments);
-            this.extensions = [Qu]
+            this.extensions = [lc]
         }
         clicked(g) {
             g.chain().focus().unsetSubscript().run(), g.chain().focus().toggleSuperscript().run(), this.activate(g)
         }
     }
-    C.SuperscriptAction = r;
-    class i extends U {
+    v.SuperscriptAction = r;
+    class i extends _ {
         constructor() {
             super(...arguments);
-            this.extensions = [id]
+            this.extensions = [pc]
         }
         clicked(g) {
             g.chain().focus().toggleUnderline().run(), this.activate(g)
         }
     }
-    C.UnderlineAction = i;
-    class o extends U {
+    v.UnderlineAction = i;
+    class s extends _ {
         constructor() {
             super(...arguments);
-            this.extensions = [mu, nl]
+            this.extensions = [Ta, js]
         }
         clicked(g) {
             g.chain().focus().toggleBulletList().run(), this.activate(g)
         }
     }
-    C.BulletListAction = o;
-    class s extends U {
+    v.BulletListAction = s;
+    class o extends _ {
         constructor() {
             super(...arguments);
-            this.extensions = [du]
+            this.extensions = [Ma]
         }
         clicked(g) {
             g.chain().focus().toggleBlockquote().run(), this.activate(g)
         }
     }
-    C.BlockquoteAction = s;
-    class l extends U {
+    v.BlockquoteAction = o;
+    class l extends _ {
         constructor() {
             super(...arguments);
-            this.extensions = [yu]
+            this.extensions = [Aa]
         }
         clicked(g) {
             g.chain().focus().toggleCodeBlock().run(), this.activate(g)
         }
     }
-    C.CodeBlockAction = l;
-    class a extends U {
-        clicked(E) {
-            E.chain().focus().setHardBreak().run(), this.activate(E)
+    v.CodeBlockAction = l;
+    class a extends _ {
+        clicked(A) {
+            A.chain().focus().setHardBreak().run(), this.activate(A)
         }
     }
-    C.HardBreakAction = a;
-    class c extends U {
-        constructor(g, x, y) {
-            super(g, x, y);
-            this.dropdownItems = [];
+    v.HardBreakAction = a;
+    class c extends Rn {
+        constructor(g, k, y) {
+            super(g, k, y, '[richtext-click^="color:"]');
             this.colors = [];
             this.allowedClasses = [];
             if (!(y.nextElementSibling instanceof HTMLUListElement) || y.nextElementSibling.role !== "menu") throw new Error('Text color requires a sibling element <ul role="menu">\u2026</ul>');
-            this.dropdownMenu = y.nextElementSibling, this.dropdownInstance = sr(this.button, this.dropdownMenu, {
-                placement: "bottom-start"
-            }), this.dropdownItems = this.dropdownMenu.querySelectorAll('[richtext-click^="color:"]'), this.collecColors()
+            this.collecColors()
         }
         collecColors() {
             this.dropdownItems.forEach(g => {
-                let x = this.extractColor(g);
-                if (x)
-                    if (/^rgb\(\d{1,3}, \d{1,3}, \d{1,3}\)$/.test(x)) {
+                let k = this.extractColor(g);
+                if (k)
+                    if (/^rgb\(\d{1,3}, \d{1,3}, \d{1,3}\)$/.test(k)) {
                         if (this.allowedClasses.length !== 0) throw new Error(`In element ${g} can not mix class based with style based colors.`);
-                        this.colors.push(x)
-                    } else if (/^-?[_a-zA-Z]+[_a-zA-Z0-9-]*$/.test(x)) this.allowedClasses.push(x);
-                else throw new Error(`${x} is not a valid color.`)
+                        this.colors.push(k)
+                    } else if (/^-?[_a-zA-Z]+[_a-zA-Z0-9-]*$/.test(k)) this.allowedClasses.push(k);
+                else throw new Error(`${k} is not a valid color.`)
             })
         }
         extractColor(g) {
             var y;
-            let x = ((y = g.getAttribute("richtext-click")) == null ? void 0 : y.split(":")) ?? [];
-            if (x.length !== 2) throw new Error(`Element ${g} requires attribute 'richtext-click'.`);
-            return x[1] === "null" ? null : x[1]
-        }
-        installEventHandler(g) {
-            this.dropdownMenu ? (this.button.addEventListener("click", () => this.toggleMenu(g)), this.dropdownMenu.addEventListener("click", x => this.toggleItem(x, g)), document.addEventListener("click", x => {
-                let y = x.target instanceof Element ? x.target : null;
-                for (; y;) {
-                    if (y.isSameNode(this.button) || y.isSameNode(this.dropdownMenu)) return;
-                    y = y.parentElement
-                }
-                this.toggleMenu(g, !1)
-            })) : this.button.addEventListener("click", x => this.toggleItem(x, g))
+            let k = ((y = g.getAttribute("richtext-click")) == null ? void 0 : y.split(":")) ?? [];
+            if (k.length !== 2) throw new Error(`Element ${g} requires attribute 'richtext-click'.`);
+            return k[1] === "null" ? null : k[1]
         }
         clicked() {}
         activate(g) {
-            let x = !1,
+            let k = !1,
                 y = this.button.querySelector("svg > rect");
-            this.dropdownItems.forEach(O => {
-                let I = this.extractColor(O);
-                I && g.isActive({
-                    textColor: I
-                }) && (this.allowedClasses.length === 0 ? y == null || y.setAttribute("fill", I) : (y == null || y.classList.forEach(L => y.classList.remove(L)), y == null || y.classList.add(I)), x = !0)
-            }), this.button.classList.toggle("active", x), x || (this.allowedClasses.length === 0 ? y == null || y.removeAttribute("fill") : y == null || y.classList.forEach(O => y.classList.remove(O)))
+            this.dropdownItems.forEach(N => {
+                let z = this.extractColor(N);
+                z && g.isActive({
+                    textColor: z
+                }) && (this.allowedClasses.length === 0 ? y == null || y.setAttribute("fill", z) : (y == null || y.classList.forEach(Q => y.classList.remove(Q)), y == null || y.classList.add(z)), k = !0)
+            }), this.button.classList.toggle("active", k), k || (this.allowedClasses.length === 0 ? y == null || y.removeAttribute("fill") : y == null || y.classList.forEach(N => y.classList.remove(N)))
         }
         extendExtensions(g) {
-            let x = !0;
+            let k = !0;
             g.forEach(y => {
                 if (y.name === "textColor") throw new Error("RichtextArea allows only one control element with 'textColor'.")
-            }), g.push(nd.configure({
+            }), g.push(fc.configure({
                 allowedClasses: this.allowedClasses
             }))
         }
-        toggleMenu(g, x) {
-            var O;
-            let y = x !== !1 && this.button.ariaExpanded === "false";
-            this.button.ariaExpanded = y ? "true" : "false", this.dropdownItems.forEach(I => {
-                var j;
-                let L = this.extractColor(I);
-                (j = I.parentElement) == null || j.classList.toggle("active", g.isActive({
-                    textColor: L
+        toggleMenu(g, k) {
+            super.toggleMenu(g, k), this.dropdownItems.forEach(y => {
+                var z;
+                let N = this.extractColor(y);
+                (z = y.parentElement) == null || z.classList.toggle("active", g.isActive({
+                    textColor: N
                 }))
-            }), (O = this.dropdownInstance) == null || O.update()
+            })
         }
-        toggleItem(g, x) {
+        toggleItem(g, k) {
             let y = g.target instanceof Element ? g.target : null;
             for (; y;) {
                 if (y instanceof HTMLAnchorElement) {
-                    let O = this.extractColor(y);
-                    O ? x.chain().focus().setColor(O).run() : x.chain().focus().unsetColor().run(), this.activate(x), this.toggleMenu(x, !1);
+                    let N = this.extractColor(y);
+                    N ? k.chain().focus().setColor(N).run() : k.chain().focus().unsetColor().run(), this.activate(k), this.toggleMenu(k, !1);
                     break
                 }
                 y = y.parentElement
             }
         }
     }
-    C.TextColorAction = c;
-    class u extends U {
-        constructor(g, x, y) {
-            super(g, x, y);
+    v.TextColorAction = c;
+    class u extends _ {
+        constructor(g, k, y) {
+            super(g, k, y);
             this.options = {
                 types: ["heading", "paragraph"]
             };
-            let O = x.split(":");
-            this.indent = O[1] ?? ""
+            let N = k.split(":");
+            this.indent = N[1] ?? ""
         }
         clicked(g) {
             g.isActive({
                 textIndent: this.indent
             }) ? g.chain().focus().unsetTextIndent().run() : g.chain().focus().setTextIndent(this.indent).run(), this.activate(g)
         }
         activate(g) {
             this.button.classList.toggle("active", g.isActive({
                 textIndent: this.indent
             }))
         }
         extendExtensions(g) {
-            g.filter(x => x.name === "textIndent").length || g.push(ed.configure(this.options))
+            g.filter(k => k.name === "textIndent").length || g.push(uc.configure(this.options))
         }
     }
-    C.TextIndentAction = u;
-    class d extends U {
-        constructor(g, x, y) {
-            super(g, x, y);
+    v.TextIndentAction = u;
+    class d extends _ {
+        constructor(g, k, y) {
+            super(g, k, y);
             this.options = {
                 types: ["heading", "paragraph"],
                 maxIndentLevel: 5
             };
-            let O = x.split(":");
-            this.indent = O[1] ?? ""
+            let N = k.split(":");
+            this.indent = N[1] ?? ""
         }
         clicked(g) {
             this.indent === "increase" ? g.chain().focus().increaseTextMargin().run() : this.indent === "decrease" ? g.chain().focus().decreaseTextMargin().run() : g.chain().focus().unsetTextMargin().run(), this.activate(g)
         }
         activate(g) {
             this.button.classList.toggle("active", g.isActive({
                 textMargin: this.indent
             }))
         }
         extendExtensions(g) {
-            g.filter(x => x.name === "textMargin").length || g.push(td.configure(this.options))
+            g.filter(k => k.name === "textMargin").length || g.push(dc.configure(this.options))
         }
     }
-    C.TextMarginAction = d;
-    class f extends U {
+    v.TextMarginAction = d;
+    class f extends _ {
         constructor() {
             super(...arguments);
-            this.extensions = [Uu, nl]
+            this.extensions = [rc, js]
         }
         clicked(g) {
             g.chain().focus().toggleOrderedList().run(), this.activate(g)
         }
     }
-    C.OrderedListAction = f;
-    class p extends U {
+    v.OrderedListAction = f;
+    class h extends _ {
         constructor() {
             super(...arguments);
-            this.extensions = [Tu]
+            this.extensions = [Ba]
         }
         clicked(g) {
             g.chain().focus().setHorizontalRule().run()
         }
     }
-    C.HorizontalRuleAction = p;
-    class h extends U {
-        clicked(E) {
-            E.chain().focus().clearNodes().unsetAllMarks().run(), this.activate(E)
+    v.HorizontalRuleAction = h;
+    class p extends _ {
+        clicked(A) {
+            A.chain().focus().clearNodes().unsetAllMarks().run(), this.activate(A)
         }
     }
-    C.ClearFormatAction = h;
-    class m extends U {
+    v.ClearFormatAction = p;
+    class m extends _ {
         constructor() {
             super(...arguments);
-            this.extensions = [Rs]
+            this.extensions = [xs]
         }
         clicked(g) {
             g.commands.undo()
         }
     }
-    C.UndoAction = m;
-    class b extends U {
+    v.UndoAction = m;
+    class b extends _ {
         constructor() {
             super(...arguments);
-            this.extensions = [Rs]
+            this.extensions = [xs]
         }
         clicked(g) {
             g.commands.redo()
         }
     }
-    C.RedoAction = b;
-    class k extends U {
-        constructor(g, x, y) {
-            var O;
-            super(g, x, y);
-            this.dropdownItems = [];
+    v.RedoAction = b;
+    class M extends Rn {
+        constructor(g, k, y) {
+            var N;
+            super(g, k, y, '[richtext-click^="heading:"]');
             this.levels = [];
-            this.dropdownMenu = y.nextElementSibling instanceof HTMLUListElement && y.nextElementSibling.role === "menu" ? y.nextElementSibling : null, this.dropdownMenu ? (this.dropdownInstance = sr(this.button, this.dropdownMenu, {
-                placement: "bottom-start"
-            }), this.dropdownItems = this.dropdownMenu.querySelectorAll('[richtext-click^="heading:"]'), this.dropdownItems.forEach(I => this.levels.push(this.extractLevel(I)))) : this.levels.push(this.extractLevel(this.button)), this.defaultIcon = (O = this.button.querySelector("svg")) == null ? void 0 : O.cloneNode(!0)
+            this.dropdownMenu ? this.dropdownItems.forEach(z => this.levels.push(this.extractLevel(z))) : this.levels.push(this.extractLevel(this.button)), this.defaultIcon = (N = this.button.querySelector("svg")) == null ? void 0 : N.cloneNode(!0)
         }
         extractLevel(g) {
-            var O;
-            let x = ((O = g.getAttribute("richtext-click")) == null ? void 0 : O.split(":")) ?? [];
-            if (x.length !== 2) throw new Error(`Element ${g} requires attribute 'richtext-click'.`);
-            return parseInt(x[1])
-        }
-        installEventHandler(g) {
-            this.dropdownMenu ? (this.button.addEventListener("click", () => this.toggleMenu(g)), this.dropdownMenu.addEventListener("click", x => this.toggleItem(x, g)), document.addEventListener("click", x => {
-                let y = x.target instanceof Element ? x.target : null;
-                for (; y;) {
-                    if (y.isSameNode(this.button) || y.isSameNode(this.dropdownMenu)) return;
-                    y = y.parentElement
-                }
-                this.toggleMenu(g, !1)
-            })) : this.button.addEventListener("click", x => this.toggleItem(x, g))
+            var N;
+            let k = ((N = g.getAttribute("richtext-click")) == null ? void 0 : N.split(":")) ?? [];
+            if (k.length !== 2) throw new Error(`Element ${g} requires attribute 'richtext-click'.`);
+            return parseInt(k[1])
         }
         clicked() {}
         activate(g) {
             if (this.dropdownMenu) {
-                let x = !1;
+                let k = !1;
                 this.dropdownItems.forEach(y => {
-                    var L;
-                    let O = this.extractLevel(y),
-                        I = (L = y.querySelector("svg")) == null ? void 0 : L.cloneNode(!0);
+                    var Q;
+                    let N = this.extractLevel(y),
+                        z = (Q = y.querySelector("svg")) == null ? void 0 : Q.cloneNode(!0);
                     g.isActive("heading", {
-                        level: O
-                    }) && I && (this.button.replaceChildren(I), x = !0)
-                }), this.button.classList.toggle("active", x), x || this.button.replaceChildren(this.defaultIcon)
+                        level: N
+                    }) && z && (this.button.replaceChildren(z), k = !0)
+                }), this.button.classList.toggle("active", k), k || this.button.replaceChildren(this.defaultIcon)
             } else {
-                let x = this.extractLevel(this.button);
+                let k = this.extractLevel(this.button);
                 this.button.classList.toggle("active", g.isActive("heading", {
-                    level: x
+                    level: k
                 }))
             }
         }
         extendExtensions(g) {
-            let x = !0;
+            let k = !0;
             g.forEach(y => {
-                y.name === "heading" && (y.options.levels.push(...this.levels), x = !1)
-            }), x && g.push(ku.configure({
+                y.name === "heading" && (y.options.levels.push(...this.levels), k = !1)
+            }), k && g.push(Na.configure({
                 levels: this.levels
             }))
         }
-        toggleMenu(g, x) {
-            var O;
-            let y = x !== !1 && this.button.ariaExpanded === "false";
-            this.button.ariaExpanded = y ? "true" : "false", this.dropdownItems.forEach(I => {
-                var j;
-                let L = this.extractLevel(I);
-                (j = I.parentElement) == null || j.classList.toggle("active", g.isActive("heading", {
-                    level: L
+        toggleMenu(g, k) {
+            super.toggleMenu(g, k), this.dropdownItems.forEach(y => {
+                var z;
+                let N = this.extractLevel(y);
+                (z = y.parentElement) == null || z.classList.toggle("active", g.isActive("heading", {
+                    level: N
                 }))
-            }), (O = this.dropdownInstance) == null || O.update()
+            })
         }
-        toggleItem(g, x) {
-            var O;
+        toggleItem(g, k) {
+            var N;
             let y = g.target instanceof Element ? g.target : null;
             for (; y;) {
                 if (y instanceof HTMLButtonElement || y instanceof HTMLAnchorElement) {
-                    let I = this.extractLevel(y);
-                    x.chain().focus().setHeading({
-                        level: I
-                    }).run(), this.activate(x), this.toggleMenu(x, !1);
-                    let L = (O = y.querySelector("svg")) == null ? void 0 : O.cloneNode(!0);
-                    L && this.button.replaceChildren(L);
+                    let z = this.extractLevel(y);
+                    k.chain().focus().setHeading({
+                        level: z
+                    }).run(), this.activate(k), this.toggleMenu(k, !1);
+                    let Q = (N = y.querySelector("svg")) == null ? void 0 : N.cloneNode(!0);
+                    Q && this.button.replaceChildren(Q);
                     break
                 }
                 y = y.parentElement
             }
         }
     }
-    C.HeadingAction = k;
-    class S extends U {
-        constructor(g, x, y) {
-            var O;
-            super(g, x, y);
-            this.dropdownItems = [];
+    v.HeadingAction = M;
+    class w extends Rn {
+        constructor(g, k, y) {
+            var N;
+            super(g, k, y, '[richtext-click^="alignment:"]');
             this.options = {
                 types: ["heading", "paragraph"],
                 alignments: [],
                 defaultAlignment: ""
             };
-            this.dropdownMenu = y.nextElementSibling instanceof HTMLUListElement && y.nextElementSibling.role === "menu" ? y.nextElementSibling : null, this.dropdownMenu ? (this.dropdownInstance = sr(this.button, this.dropdownMenu, {
-                placement: "bottom-start"
-            }), this.dropdownItems = this.dropdownMenu.querySelectorAll('[richtext-click^="alignment:"]'), this.dropdownItems.forEach(I => {
-                this.options.alignments.push(this.extractAlignment(I))
-            })) : this.options.alignments.push(this.extractAlignment(this.button)), this.defaultIcon = (O = this.button.querySelector("svg")) == null ? void 0 : O.cloneNode(!0)
+            this.dropdownMenu ? this.dropdownItems.forEach(z => {
+                this.options.alignments.push(this.extractAlignment(z))
+            }) : this.options.alignments.push(this.extractAlignment(this.button)), this.defaultIcon = (N = this.button.querySelector("svg")) == null ? void 0 : N.cloneNode(!0)
         }
         extractAlignment(g) {
             var y;
-            let x = ((y = g.getAttribute("richtext-click")) == null ? void 0 : y.split(":")) ?? [];
-            if (x.length !== 2) throw new Error(`Element ${g} requires attribute 'richtext-click'.`);
-            return x[1]
-        }
-        installEventHandler(g) {
-            this.dropdownMenu ? (this.button.addEventListener("click", () => this.toggleMenu(g)), this.dropdownMenu.addEventListener("click", x => this.toggleItem(x, g)), document.addEventListener("click", x => {
-                let y = x.target instanceof Element ? x.target : null;
-                for (; y;) {
-                    if (y.isSameNode(this.button) || y.isSameNode(this.dropdownMenu)) return;
-                    y = y.parentElement
-                }
-                this.toggleMenu(g, !1)
-            })) : this.button.addEventListener("click", x => this.toggleItem(x, g))
+            let k = ((y = g.getAttribute("richtext-click")) == null ? void 0 : y.split(":")) ?? [];
+            if (k.length !== 2) throw new Error(`Element ${g} requires attribute 'richtext-click'.`);
+            return k[1]
         }
         clicked() {}
         activate(g) {
             if (this.dropdownMenu) {
-                let x = !1;
+                let k = !1;
                 this.dropdownItems.forEach(y => {
-                    var L;
-                    let O = this.extractAlignment(y),
-                        I = (L = y.querySelector("svg")) == null ? void 0 : L.cloneNode(!0);
+                    var Q;
+                    let N = this.extractAlignment(y),
+                        z = (Q = y.querySelector("svg")) == null ? void 0 : Q.cloneNode(!0);
                     g.isActive({
-                        textAlign: O
-                    }) && I && (this.button.replaceChildren(I), x = !0)
-                }), x || this.button.replaceChildren(this.defaultIcon)
+                        textAlign: N
+                    }) && z && (this.button.replaceChildren(z), k = !0)
+                }), k || this.button.replaceChildren(this.defaultIcon)
             } else {
-                let x = this.extractAlignment(this.button);
+                let k = this.extractAlignment(this.button);
                 this.button.classList.toggle("active", g.isActive({
-                    textAlign: x
+                    textAlign: k
                 }))
             }
         }
         extendExtensions(g) {
-            let x = !0;
+            let k = !0;
             g.forEach(y => {
-                y.name === "textAlign" && (y.options.alignments.push(...this.options.alignments), x = !1)
-            }), x && g.push(Zu.configure(this.options))
+                y.name === "textAlign" && (y.options.alignments.push(...this.options.alignments), k = !1)
+            }), k && g.push(cc.configure(this.options))
         }
-        toggleMenu(g, x) {
-            var O;
-            let y = x !== !1 && this.button.ariaExpanded === "false";
-            this.button.ariaExpanded = y ? "true" : "false", this.dropdownItems.forEach(I => {
-                var j;
-                let L = this.extractAlignment(I);
-                (j = I.parentElement) == null || j.classList.toggle("active", g.isActive({
-                    textAlign: L
+        toggleMenu(g, k) {
+            super.toggleMenu(g, k), this.dropdownItems.forEach(y => {
+                var z;
+                let N = this.extractAlignment(y);
+                (z = y.parentElement) == null || z.classList.toggle("active", g.isActive({
+                    textAlign: N
                 }))
-            }), (O = this.dropdownInstance) == null || O.update()
+            })
         }
-        toggleItem(g, x) {
-            var O;
+        toggleItem(g, k) {
+            var N;
             let y = g.target instanceof Element ? g.target : null;
             for (; y;) {
                 if (y instanceof HTMLButtonElement || y instanceof HTMLAnchorElement) {
-                    let I = this.extractAlignment(y);
-                    x.chain().focus().setTextAlign(I).run(), this.activate(x), this.toggleMenu(x, !1);
-                    let L = (O = y.querySelector("svg")) == null ? void 0 : O.cloneNode(!0);
-                    L && this.button.replaceChildren(L);
+                    let z = this.extractAlignment(y);
+                    k.chain().focus().setTextAlign(z).run(), this.activate(k), this.toggleMenu(k, !1);
+                    let Q = (N = y.querySelector("svg")) == null ? void 0 : N.cloneNode(!0);
+                    Q && this.button.replaceChildren(Q);
                     break
                 }
                 y = y.parentElement
             }
         }
     }
-    C.TextAlignAction = S
-})(Xn || (Xn = {}));
+    v.TextAlignAction = w
+})(on || (on = {}));
 (i => {
-    class n extends U {
+    class n extends _ {
         constructor(l, a, c) {
             super(l, a, c);
             this.clicked = l => this.openDialog(l);
             let u = c.getAttribute("richtext-click") ?? "";
             this.modalDialogElement = l.querySelector(`dialog[richtext-opener="${u}"]`), this.formElement = this.modalDialogElement.querySelector('form[method="dialog"]')
         }
         initialize() {
@@ -14966,15 +13720,15 @@
                 once: !0
             })
         }
     }
     class e extends n {
         constructor(l, a, c) {
             super(l, a, c);
-            this.extensions = [qu.configure({
+            this.extensions = [ec.configure({
                 openOnClick: !1
             })];
             this.textInputElement = this.formElement.elements.namedItem("text"), this.urlInputElement = this.formElement.elements.namedItem("url"), this.initialize()
         }
         initialize() {
             if (super.initialize(), !(this.textInputElement instanceof HTMLInputElement)) throw new Error('<form method="dialog"> requires field <input name="text">');
             if (!(this.urlInputElement instanceof HTMLInputElement)) throw new Error('<form method="dialog"> requires field <input name="url">')
@@ -15000,15 +13754,15 @@
             this.formElement.reset()
         }
     }
     i.LinkAction = e;
     class t extends n {
         constructor(l, a, c) {
             super(l, a, c);
-            this.extensions = [rd.configure()];
+            this.extensions = [hc.configure()];
             this.variableInputElement = this.formElement.elements.namedItem("variable"), this.sampleInputElement = this.formElement.elements.namedItem("sample"), this.initialize()
         }
         initialize() {
             if (super.initialize(), !(this.variableInputElement instanceof HTMLInputElement)) throw new Error('<form method="dialog"> requires field <input name="variable">');
             if (!(this.sampleInputElement instanceof HTMLInputElement)) throw new Error('<form method="dialog"> requires field <input name="sample">')
         }
         activate(l) {
@@ -15036,15 +13790,15 @@
             this.formElement.reset()
         }
     }
     i.PlaceholderAction = t;
     class r extends n {
         constructor(l, a, c) {
             super(l, a, c);
-            this.extensions = [Cu.configure({
+            this.extensions = [za.configure({
                 inline: !1
             })];
             this.fileInputElement = this.formElement.elements.namedItem("image"), this.initialize()
         }
         initialize() {
             if (super.initialize(), !(this.fileInputElement instanceof HTMLInputElement)) throw new Error('<form method="dialog"> requires field <input name="text">')
         }
@@ -15060,16 +13814,16 @@
                 l.chain().focus().setImage({
                     src: c.src
                 }).run()
             } else a === "remove" && l.chain().focus().extendMarkRange("link").unsetLink().run()
         }
     }
     i.ImageAction = r
-})(Xn || (Xn = {}));
-var rl = class {
+})(on || (on = {}));
+var $s = class {
         constructor(e, t) {
             this.registeredActions = new Array;
             this.useJson = !1;
             this.charaterCountDiv = null;
             this.focused = () => {
                 this.wrapperElement.classList.add("focused"), this.textAreaElement.dispatchEvent(new Event("focus"))
             };
@@ -15090,119 +13844,119 @@
             this.selectionUpdate = () => {
                 this.registeredActions.forEach(e => e.activate(this.editor))
             };
             this.formResetted = () => {
                 this.editor.chain().clearContent().insertContent(this.initialValue).run()
             };
             this.formSubmitted = () => {};
-            this.wrapperElement = e, this.textAreaElement = t, this.menubarElement = e.querySelector('[role="menubar"]'), this.declaredStyles = document.createElement("style"), this.declaredStyles.innerText = pl, document.head.appendChild(this.declaredStyles);
+            this.wrapperElement = e, this.textAreaElement = t, this.menubarElement = e.querySelector('[role="menubar"]'), this.declaredStyles = document.createElement("style"), this.declaredStyles.innerText = Js, document.head.appendChild(this.declaredStyles);
             let r = e.querySelector("textarea + script");
             if (r instanceof HTMLScriptElement && r.type === "application/json") {
                 this.useJson = !0;
                 let i = r.textContent ? JSON.parse(r.textContent) : "";
                 this.editor = this.createEditor(e, i), r.remove()
             } else this.useJson = !1, this.editor = this.createEditor(e, t.textContent);
             this.initialValue = this.getValue(), this.transferStyles(), this.concealTextArea(e), this.textAreaElement.innerHTML = this.editor.getHTML(), this.contentUpdate(), this.installEventHandlers()
         }
         createEditor(e, t) {
-            let r = new Array(xu, _u, Xu, bu);
-            return this.registerControlActions(r), this.registerPlaceholder(r), this.registerCharaterCount(r), new di({
+            let r = new Array(Oa, ic, ac, va);
+            return this.registerControlActions(r), this.registerPlaceholder(r), this.registerCharaterCount(r), new fr({
                 element: e,
                 extensions: r,
                 content: t,
                 autofocus: !1,
                 editable: !this.textAreaElement.disabled,
                 injectCSS: !1
             })
         }
         registerControlActions(e) {
             var t;
             return (t = this.menubarElement) == null || t.querySelectorAll("button[richtext-click]").forEach(r => {
                 if (!(r instanceof HTMLButtonElement)) return;
                 let i = r.getAttribute("richtext-click");
                 if (!i) throw new Error("Missing attribute 'richtext-click' on action button");
-                let o = i.split(":"),
-                    s = `${o[0].charAt(0).toUpperCase()}${o[0].slice(1)}Action`,
-                    l = Xn[s];
-                if (!((l == null ? void 0 : l.prototype) instanceof U)) throw new Error(`Unknown action class '${s}'.`);
+                let s = i.split(":"),
+                    o = `${s[0].charAt(0).toUpperCase()}${s[0].slice(1)}Action`,
+                    l = on[o];
+                if (!((l == null ? void 0 : l.prototype) instanceof _)) throw new Error(`Unknown action class '${o}'.`);
                 let a = new l(this.wrapperElement, i, r);
                 this.registeredActions.push(a), a.extendExtensions(e)
             }), e
         }
         registerPlaceholder(e) {
             let t = this.textAreaElement.getAttribute("placeholder");
-            t && e.push(Gu.configure({
+            t && e.push(sc.configure({
                 placeholder: t
             }))
         }
         registerCharaterCount(e) {
             let t = parseInt(this.textAreaElement.getAttribute("maxlength") ?? "");
-            t > 0 && (e.push(gu.configure({
+            t > 0 && (e.push(Ca.configure({
                 limit: t
-            })), this.charaterCountTemplate = (0, sd.default)(`\${count}/${t}`), this.charaterCountDiv = document.createElement("div"), this.charaterCountDiv.classList.add("character-count"), this.wrapperElement.insertAdjacentElement("beforeend", this.charaterCountDiv))
+            })), this.charaterCountTemplate = (0, gc.default)(`\${count}/${t}`), this.charaterCountDiv = document.createElement("div"), this.charaterCountDiv.classList.add("character-count"), this.wrapperElement.insertAdjacentElement("beforeend", this.charaterCountDiv))
         }
         installEventHandlers() {
             this.editor.on("focus", this.focused), this.editor.on("update", this.updated), this.editor.on("blur", this.blurred), this.editor.on("update", this.contentUpdate), this.editor.on("selectionUpdate", this.selectionUpdate);
             let e = this.textAreaElement.form;
             e.addEventListener("reset", this.formResetted), e.addEventListener("submitted", this.formSubmitted), this.registeredActions.forEach(t => t.installEventHandler(this.editor))
         }
         concealTextArea(e) {
             e.insertAdjacentElement("afterend", this.textAreaElement), this.textAreaElement.classList.add("dj-concealed")
         }
         transferStyles() {
             var r;
             let e = ((r = this.menubarElement) == null ? void 0 : r.getBoundingClientRect().height) ?? 0,
                 t = this.declaredStyles.sheet;
             for (let i = 0; t && i < t.cssRules.length; i++) {
-                let o = t.cssRules.item(i),
-                    s;
-                switch (o.selectorText) {
+                let s = t.cssRules.item(i),
+                    o;
+                switch (s.selectorText) {
                     case ".dj-richtext-wrapper":
-                        s = wt.extractStyles(this.textAreaElement, ["height", "background-image", "border", "border-radius", "box-shadow", "outline", "resize"]), s = s.concat(`min-height:${e*2}px;`), t.insertRule(`${o.selectorText}{${s}}`, ++i);
+                        o = Ue.extractStyles(this.textAreaElement, ["height", "background-image", "border", "border-radius", "box-shadow", "outline", "resize"]), o = o.concat(`min-height:${e*2}px;`), t.insertRule(`${s.selectorText}{${o}}`, ++i);
                         break;
                     case ".dj-richtext-wrapper.focused":
-                        this.textAreaElement.style.transition = "none", this.textAreaElement.focus(), s = wt.extractStyles(this.textAreaElement, ["border", "box-shadow", "outline"]), this.textAreaElement.blur(), t.insertRule(`${o.selectorText}{${s}}`, ++i), this.textAreaElement.style.transition = "";
+                        this.textAreaElement.style.transition = "none", this.textAreaElement.focus(), o = Ue.extractStyles(this.textAreaElement, ["border", "box-shadow", "outline"]), this.textAreaElement.blur(), t.insertRule(`${s.selectorText}{${o}}`, ++i), this.textAreaElement.style.transition = "";
                         break;
                     case ".dj-submitted .dj-richtext-wrapper.focused.invalid":
-                        this.textAreaElement.style.transition = "none", this.textAreaElement.classList.add("-focus-", "-invalid-", "is-invalid"), s = wt.extractStyles(this.textAreaElement, ["border", "box-shadow", "outline"]), this.textAreaElement.classList.remove("-focus-", "-invalid-", "is-invalid"), t.insertRule(`${o.selectorText}{${s}}`, ++i), this.textAreaElement.style.transition = "";
+                        this.textAreaElement.style.transition = "none", this.textAreaElement.classList.add("-focus-", "-invalid-", "is-invalid"), o = Ue.extractStyles(this.textAreaElement, ["border", "box-shadow", "outline"]), this.textAreaElement.classList.remove("-focus-", "-invalid-", "is-invalid"), t.insertRule(`${s.selectorText}{${o}}`, ++i), this.textAreaElement.style.transition = "";
                         break;
                     case ".dj-richtext-wrapper .ProseMirror":
-                        s = wt.extractStyles(this.textAreaElement, ["font-family", "font-size", "font-strech", "font-style", "font-weight", "letter-spacing", "white-space", "line-height", "overflow", "padding"]), s = s.concat(`top:${e+1}px;`), t.insertRule(`${o.selectorText}{${s}}`, ++i);
+                        o = Ue.extractStyles(this.textAreaElement, ["font-family", "font-size", "font-strech", "font-style", "font-weight", "letter-spacing", "white-space", "line-height", "overflow", "padding"]), o = o.concat(`top:${e+1}px;`), t.insertRule(`${s.selectorText}{${o}}`, ++i);
                         break;
                     case '.dj-richtext-wrapper [role="menubar"]':
-                        s = wt.extractStyles(this.textAreaElement, ["border-bottom"]), t.insertRule(`${o.selectorText}{${s}}`, ++i);
+                        o = Ue.extractStyles(this.textAreaElement, ["border-bottom"]), t.insertRule(`${s.selectorText}{${o}}`, ++i);
                         break;
                     case '.dj-richtext-wrapper [role="menubar"] button[aria-haspopup="true"] + ul[role="menu"]':
-                        s = wt.extractStyles(this.textAreaElement, ["border", "z-index"]);
+                        o = Ue.extractStyles(this.textAreaElement, ["border", "z-index"]);
                         let l = new RegExp("z-index:(\\d+);"),
-                            a = s.match(l);
-                        a ? s = s.replace(l, `z-index:${parseInt(a[1])+1}`) : s = s.replace("z-index:auto;", "z-index:1;"), t.insertRule(`${o.selectorText}{${s}}`, ++i), this.menubarElement && (s = wt.extractStyles(document.documentElement, ["background-color"]), s === "background-color:rgba(0, 0, 0, 0); " && (s = "background-color:rgb(255, 255, 255);"), t.insertRule(`${o.selectorText}{${s}}`, ++i));
+                            a = o.match(l);
+                        a ? o = o.replace(l, `z-index:${parseInt(a[1])+1}`) : o = o.replace("z-index:auto;", "z-index:1;"), t.insertRule(`${s.selectorText}{${o}}`, ++i), this.menubarElement && (o = Ue.extractStyles(document.documentElement, ["background-color"]), o === "background-color:rgba(0, 0, 0, 0); " && (o = "background-color:rgb(255, 255, 255);"), t.insertRule(`${s.selectorText}{${o}}`, ++i));
                         break;
                     default:
                         break
                 }
             }
         }
         disconnect() {}
         getValue() {
             return this.editor.isEmpty ? "" : this.useJson ? this.editor.getJSON() : this.editor.getHTML()
         }
     },
-    Vi = Symbol("RichtextArea"),
-    od = class extends HTMLTextAreaElement {
+    Vr = Symbol("RichtextArea"),
+    mc = class extends HTMLTextAreaElement {
         connectedCallback() {
             let t = this.closest(".dj-richtext-wrapper");
-            t instanceof HTMLElement && (this[Vi] = new rl(t, this))
+            t instanceof HTMLElement && (this[Vr] = new $s(t, this))
         }
         disconnectCallback() {
             var t;
-            (t = this[Vi]) == null || t.disconnect()
+            (t = this[Vr]) == null || t.disconnect()
         }
         get value() {
             var t;
-            return (t = this[Vi]) == null ? void 0 : t.getValue()
+            return (t = this[Vr]) == null ? void 0 : t.getValue()
         }
     };
-Vi;
+Vr;
 export {
-    od as RichTextAreaElement
+    mc as RichTextAreaElement
 };
```

### Comparing `django-formset-1.0.dev1/formset/static/formset/js/chunk-A6DNWD2B.js` & `django-formset-1.0.dev2/formset/static/formset/js/chunk-JSQHGMDY.js`

 * *Files identical despite different names*

### Comparing `django-formset-1.0.dev1/formset/static/formset/js/chunk-AELXO3WZ.js` & `django-formset-1.0.dev2/formset/static/formset/js/chunk-AELXO3WZ.js`

 * *Files identical despite different names*

### Comparing `django-formset-1.0.dev1/formset/static/formset/js/chunk-APVD22ED.js` & `django-formset-1.0.dev2/formset/static/formset/js/chunk-APVD22ED.js`

 * *Files identical despite different names*

### Comparing `django-formset-1.0.dev1/formset/static/formset/js/chunk-KDP4ZIAK.js` & `django-formset-1.0.dev2/formset/static/formset/js/chunk-KDP4ZIAK.js`

 * *Files identical despite different names*

### Comparing `django-formset-1.0.dev1/formset/static/formset/js/chunk-NLMHZ7JJ.js` & `django-formset-1.0.dev2/formset/static/formset/js/chunk-NLMHZ7JJ.js`

 * *Files identical despite different names*

### Comparing `django-formset-1.0.dev1/formset/static/formset/js/chunk-O5UGFU32.js` & `django-formset-1.0.dev2/formset/static/formset/js/chunk-O5UGFU32.js`

 * *Files identical despite different names*

### Comparing `django-formset-1.0.dev1/formset/static/formset/js/django-formset.js` & `django-formset-1.0.dev2/formset/static/formset/js/django-formset.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -3173,43 +3173,43 @@
 
     function n(s, u, f, d = void 0) {
         customElements.get(u) instanceof Function ? s() : (window.customElements.define(u, f, d), window.customElements.whenDefined(u).then(() => s()))
     }
 
     function i(s) {
         s.querySelector('select[is="django-selectize"]') && r.push(new Promise((u, f) => {
-            import("./DjangoSelectize-D5OZV3VC.js").then(({
+            import("./DjangoSelectize-MICJ4DHH.js").then(({
                 DjangoSelectizeElement: d
             }) => {
                 n(u, "django-selectize", d, {
                     extends: "select"
                 })
             }).catch(d => f(d))
         })), s.querySelector("django-sortable-select") ? r.push(new Promise((u, f) => {
-            import("./SortableSelect-7KQVPUF2.js").then(({
+            import("./SortableSelect-WBJL5XGS.js").then(({
                 SortableSelectElement: d
             }) => {
-                customElements.get("django-sortable-select") instanceof Function ? u() : window.customElements.define("django-sortable-select", d), import("./DualSelector-WKVUCHIG.js").then(({
+                customElements.get("django-sortable-select") instanceof Function ? u() : window.customElements.define("django-sortable-select", d), import("./DualSelector-XYVC5VWO.js").then(({
                     DualSelectorElement: h
                 }) => {
                     customElements.get("django-dual-selector") instanceof Function ? u() : (window.customElements.define("django-dual-selector", h, {
                         extends: "select"
                     }), Promise.all([window.customElements.whenDefined("django-sortable-select"), window.customElements.whenDefined("django-dual-selector")]).then(() => u()))
                 }).catch(h => f(h))
             }).catch(d => f(d))
         })) : s.querySelector('select[is="django-dual-selector"]') && r.push(new Promise((u, f) => {
-            import("./DualSelector-WKVUCHIG.js").then(({
+            import("./DualSelector-XYVC5VWO.js").then(({
                 DualSelectorElement: d
             }) => {
                 n(u, "django-dual-selector", d, {
                     extends: "select"
                 })
             }).catch(d => f(d))
         })), s.querySelector('textarea[is="django-richtext"]') && r.push(new Promise((u, f) => {
-            import("./RichtextArea-XF7D5LDW.js").then(({
+            import("./RichtextArea-63COGKXW.js").then(({
                 RichTextAreaElement: d
             }) => {
                 n(u, "django-richtext", d, {
                     extends: "textarea"
                 })
             }).catch(d => f(d))
         })), s.querySelector('input[is="django-slug"]') && r.push(new Promise((u, f) => {
@@ -3217,23 +3217,23 @@
                 DjangoSlugElement: d
             }) => {
                 n(u, "django-slug", d, {
                     extends: "input"
                 })
             }).catch(d => f(d))
         })), s.querySelector('input[is="django-datepicker"]') && r.push(new Promise((u, f) => {
-            import("./DateTimePicker-IUQQAZGS.js").then(({
+            import("./DateTimePicker-64ONYNKG.js").then(({
                 DatePickerElement: d
             }) => {
                 n(u, "django-datepicker", d, {
                     extends: "input"
                 })
             }).catch(d => f(d))
         })), s.querySelector('input[is="django-datetimepicker"]') && r.push(new Promise((u, f) => {
-            import("./DateTimePicker-IUQQAZGS.js").then(({
+            import("./DateTimePicker-64ONYNKG.js").then(({
                 DateTimePickerElement: d
             }) => {
                 n(u, "django-datetimepicker", d, {
                     extends: "input"
                 })
             }).catch(d => f(d))
         }))
```

### Comparing `django-formset-1.0.dev1/formset/static/formset/scss/bootstrap5-extra.scss` & `django-formset-1.0.dev2/formset/static/formset/scss/bootstrap5-extra.scss`

 * *Files identical despite different names*

### Comparing `django-formset-1.0.dev1/formset/static/formset/scss/collections.scss` & `django-formset-1.0.dev2/formset/static/formset/scss/collections.scss`

 * *Files identical despite different names*

### Comparing `django-formset-1.0.dev1/formset/templates/calendar/hours.html` & `django-formset-1.0.dev2/formset/templates/calendar/hours.html`

 * *Files identical despite different names*

### Comparing `django-formset-1.0.dev1/formset/templates/calendar/months.html` & `django-formset-1.0.dev2/formset/templates/calendar/months.html`

 * *Files identical despite different names*

### Comparing `django-formset-1.0.dev1/formset/templates/calendar/weeks.html` & `django-formset-1.0.dev2/formset/templates/calendar/weeks.html`

 * *Files identical despite different names*

### Comparing `django-formset-1.0.dev1/formset/templates/calendar/years.html` & `django-formset-1.0.dev2/formset/templates/calendar/years.html`

 * *Files identical despite different names*

### Comparing `django-formset-1.0.dev1/formset/templates/formset/bootstrap/widgets/dual_selector.html` & `django-formset-1.0.dev2/formset/templates/formset/bootstrap/widgets/dual_selector.html`

 * *Files identical despite different names*

### Comparing `django-formset-1.0.dev1/formset/templates/formset/bootstrap/widgets/file.html` & `django-formset-1.0.dev2/formset/templates/formset/bootstrap/widgets/file.html`

 * *Files identical despite different names*

### Comparing `django-formset-1.0.dev1/formset/templates/formset/bulma/widgets/dual_selector.html` & `django-formset-1.0.dev2/formset/templates/formset/bulma/widgets/dual_selector.html`

 * *Files identical despite different names*

### Comparing `django-formset-1.0.dev1/formset/templates/formset/bulma/widgets/file.html` & `django-formset-1.0.dev2/formset/templates/formset/bulma/widgets/file.html`

 * *Files identical despite different names*

### Comparing `django-formset-1.0.dev1/formset/templates/formset/default/buttons/richtext_align.html` & `django-formset-1.0.dev2/formset/templates/formset/default/buttons/richtext_align.html`

 * *Files identical despite different names*

### Comparing `django-formset-1.0.dev1/formset/templates/formset/default/buttons/richtext_color.html` & `django-formset-1.0.dev2/formset/templates/formset/default/buttons/richtext_color.html`

 * *Files identical despite different names*

### Comparing `django-formset-1.0.dev1/formset/templates/formset/default/buttons/richtext_heading.html` & `django-formset-1.0.dev2/formset/templates/formset/default/buttons/richtext_heading.html`

 * *Files identical despite different names*

### Comparing `django-formset-1.0.dev1/formset/templates/formset/default/collection.html` & `django-formset-1.0.dev2/formset/templates/formset/default/collection.html`

 * *Files identical despite different names*

### Comparing `django-formset-1.0.dev1/formset/templates/formset/default/dialog_form.html` & `django-formset-1.0.dev2/formset/templates/formset/default/dialog_form.html`

 * *Files identical despite different names*

### Comparing `django-formset-1.0.dev1/formset/templates/formset/default/fieldset.html` & `django-formset-1.0.dev2/formset/templates/formset/default/fieldset.html`

 * *Files identical despite different names*

### Comparing `django-formset-1.0.dev1/formset/templates/formset/default/widgets/dual_selector.html` & `django-formset-1.0.dev2/formset/templates/formset/default/widgets/dual_selector.html`

 * *Files identical despite different names*

### Comparing `django-formset-1.0.dev1/formset/templates/formset/default/widgets/file.html` & `django-formset-1.0.dev2/formset/templates/formset/default/widgets/file.html`

 * *Files identical despite different names*

### Comparing `django-formset-1.0.dev1/formset/templates/formset/default/widgets/selectize.html` & `django-formset-1.0.dev2/formset/templates/formset/default/widgets/selectize.html`

 * *Files identical despite different names*

### Comparing `django-formset-1.0.dev1/formset/templates/formset/foundation/widgets/dual_selector.html` & `django-formset-1.0.dev2/formset/templates/formset/foundation/widgets/dual_selector.html`

 * *Files identical despite different names*

### Comparing `django-formset-1.0.dev1/formset/templates/formset/foundation/widgets/file.html` & `django-formset-1.0.dev2/formset/templates/formset/foundation/widgets/file.html`

 * *Files identical despite different names*

### Comparing `django-formset-1.0.dev1/formset/templates/formset/icons/blockquote.svg` & `django-formset-1.0.dev2/formset/templates/formset/icons/blockquote.svg`

 * *Files identical despite different names*

### Comparing `django-formset-1.0.dev1/formset/templates/formset/icons/letters.svg` & `django-formset-1.0.dev2/formset/templates/formset/icons/letters.svg`

 * *Files identical despite different names*

### Comparing `django-formset-1.0.dev1/formset/templates/formset/icons/placeholder.svg` & `django-formset-1.0.dev2/formset/templates/formset/icons/placeholder.svg`

 * *Files identical despite different names*

### Comparing `django-formset-1.0.dev1/formset/templates/formset/icons/questionmark.svg` & `django-formset-1.0.dev2/formset/templates/formset/icons/questionmark.svg`

 * *Files identical despite different names*

### Comparing `django-formset-1.0.dev1/formset/templates/formset/icons/subscript.svg` & `django-formset-1.0.dev2/formset/templates/formset/icons/subscript.svg`

 * *Files identical despite different names*

### Comparing `django-formset-1.0.dev1/formset/templates/formset/icons/unlink.svg` & `django-formset-1.0.dev2/formset/templates/formset/icons/unlink.svg`

 * *Files identical despite different names*

### Comparing `django-formset-1.0.dev1/formset/templates/formset/tailwind/widgets/dual_selector.html` & `django-formset-1.0.dev2/formset/templates/formset/tailwind/widgets/dual_selector.html`

 * *Files identical despite different names*

### Comparing `django-formset-1.0.dev1/formset/templates/formset/tailwind/widgets/file.html` & `django-formset-1.0.dev2/formset/templates/formset/tailwind/widgets/file.html`

 * *Files identical despite different names*

### Comparing `django-formset-1.0.dev1/formset/templates/formset/uikit/widgets/file.html` & `django-formset-1.0.dev2/formset/templates/formset/uikit/widgets/file.html`

 * *Files identical despite different names*

### Comparing `django-formset-1.0.dev1/formset/templatetags/formsetify.py` & `django-formset-1.0.dev2/formset/templatetags/formsetify.py`

 * *Files identical despite different names*

### Comparing `django-formset-1.0.dev1/formset/upload.py` & `django-formset-1.0.dev2/formset/upload.py`

 * *Files identical despite different names*

### Comparing `django-formset-1.0.dev1/formset/utils.py` & `django-formset-1.0.dev2/formset/utils.py`

 * *Files identical despite different names*

### Comparing `django-formset-1.0.dev1/formset/views.py` & `django-formset-1.0.dev2/formset/views.py`

 * *Files identical despite different names*

### Comparing `django-formset-1.0.dev1/formset/widgets.py` & `django-formset-1.0.dev2/formset/widgets.py`

 * *Files identical despite different names*

### Comparing `django-formset-1.0.dev1/setup.py` & `django-formset-1.0.dev2/setup.py`

 * *Files identical despite different names*

