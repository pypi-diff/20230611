# Comparing `tmp/cycode-0.2.5.dev5.tar.gz` & `tmp/cycode-0.2.5.dev6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cycode-0.2.5.dev5.tar", max compression
+gzip compressed data, was "cycode-0.2.5.dev6.tar", max compression
```

## Comparing `cycode-0.2.5.dev5.tar` & `cycode-0.2.5.dev6.tar`

### file list

```diff
@@ -1,58 +1,58 @@
--rw-r--r--   0        0        0    32320 2023-06-11 18:40:19.306758 cycode-0.2.5.dev5/README.md
--rw-r--r--   0        0        0      115 2023-06-11 18:40:47.955126 cycode-0.2.5.dev5/cycode/__init__.py
--rw-r--r--   0        0        0        0 2023-06-11 18:40:19.306758 cycode-0.2.5.dev5/cycode/cli/__init__.py
--rw-r--r--   0        0        0        0 2023-06-11 18:40:19.306758 cycode-0.2.5.dev5/cycode/cli/auth/__init__.py
--rw-r--r--   0        0        0     2813 2023-06-11 18:40:19.306758 cycode-0.2.5.dev5/cycode/cli/auth/auth_command.py
--rw-r--r--   0        0        0     4761 2023-06-11 18:40:19.306758 cycode-0.2.5.dev5/cycode/cli/auth/auth_manager.py
--rw-r--r--   0        0        0     1652 2023-06-11 18:40:19.306758 cycode-0.2.5.dev5/cycode/cli/ci_integrations.py
--rw-r--r--   0        0        0    47480 2023-06-11 18:40:19.306758 cycode-0.2.5.dev5/cycode/cli/code_scanner.py
--rw-r--r--   0        0        0      453 2023-06-11 18:40:19.306758 cycode-0.2.5.dev5/cycode/cli/config.py
--rw-r--r--   0        0        0      387 2023-06-11 18:40:19.306758 cycode-0.2.5.dev5/cycode/cli/config.yaml
--rw-r--r--   0        0        0     5039 2023-06-11 18:40:19.306758 cycode-0.2.5.dev5/cycode/cli/consts.py
--rw-r--r--   0        0        0        0 2023-06-11 18:40:19.306758 cycode-0.2.5.dev5/cycode/cli/exceptions/__init__.py
--rw-r--r--   0        0        0     1698 2023-06-11 18:40:19.306758 cycode-0.2.5.dev5/cycode/cli/exceptions/custom_exceptions.py
--rw-r--r--   0        0        0        0 2023-06-11 18:40:19.306758 cycode-0.2.5.dev5/cycode/cli/helpers/__init__.py
--rw-r--r--   0        0        0        0 2023-06-11 18:40:19.306758 cycode-0.2.5.dev5/cycode/cli/helpers/maven/__init__.py
--rw-r--r--   0        0        0     2196 2023-06-11 18:40:19.306758 cycode-0.2.5.dev5/cycode/cli/helpers/maven/base_restore_maven_dependencies.py
--rw-r--r--   0        0        0      992 2023-06-11 18:40:19.306758 cycode-0.2.5.dev5/cycode/cli/helpers/maven/restore_gradle_dependencies.py
--rw-r--r--   0        0        0     2993 2023-06-11 18:40:19.306758 cycode-0.2.5.dev5/cycode/cli/helpers/maven/restore_maven_dependencies.py
--rw-r--r--   0        0        0     5835 2023-06-11 18:40:19.306758 cycode-0.2.5.dev5/cycode/cli/helpers/sca_code_scanner.py
--rw-r--r--   0        0        0     7213 2023-06-11 18:40:19.306758 cycode-0.2.5.dev5/cycode/cli/main.py
--rw-r--r--   0        0        0     1332 2023-06-11 18:40:19.306758 cycode-0.2.5.dev5/cycode/cli/models.py
--rw-r--r--   0        0        0       93 2023-06-11 18:40:19.306758 cycode-0.2.5.dev5/cycode/cli/printers/__init__.py
--rw-r--r--   0        0        0      564 2023-06-11 18:40:19.306758 cycode-0.2.5.dev5/cycode/cli/printers/base_printer.py
--rw-r--r--   0        0        0     1709 2023-06-11 18:40:19.306758 cycode-0.2.5.dev5/cycode/cli/printers/console_printer.py
--rw-r--r--   0        0        0     1537 2023-06-11 18:40:19.306758 cycode-0.2.5.dev5/cycode/cli/printers/json_printer.py
--rw-r--r--   0        0        0     6108 2023-06-11 18:40:19.306758 cycode-0.2.5.dev5/cycode/cli/printers/table_printer.py
--rw-r--r--   0        0        0     9166 2023-06-11 18:40:19.306758 cycode-0.2.5.dev5/cycode/cli/printers/text_printer.py
--rw-r--r--   0        0        0        0 2023-06-11 18:40:19.306758 cycode-0.2.5.dev5/cycode/cli/user_settings/__init__.py
--rw-r--r--   0        0        0      533 2023-06-11 18:40:19.306758 cycode-0.2.5.dev5/cycode/cli/user_settings/base_file_manager.py
--rw-r--r--   0        0        0     4821 2023-06-11 18:40:19.306758 cycode-0.2.5.dev5/cycode/cli/user_settings/config_file_manager.py
--rw-r--r--   0        0        0     6925 2023-06-11 18:40:19.306758 cycode-0.2.5.dev5/cycode/cli/user_settings/configuration_manager.py
--rw-r--r--   0        0        0     1908 2023-06-11 18:40:19.306758 cycode-0.2.5.dev5/cycode/cli/user_settings/credentials_manager.py
--rw-r--r--   0        0        0     6853 2023-06-11 18:40:19.306758 cycode-0.2.5.dev5/cycode/cli/user_settings/user_settings_commands.py
--rw-r--r--   0        0        0        0 2023-06-11 18:40:19.306758 cycode-0.2.5.dev5/cycode/cli/utils/__init__.py
--rw-r--r--   0        0        0     2162 2023-06-11 18:40:19.306758 cycode-0.2.5.dev5/cycode/cli/utils/path_utils.py
--rw-r--r--   0        0        0      195 2023-06-11 18:40:19.306758 cycode-0.2.5.dev5/cycode/cli/utils/scan_utils.py
--rw-r--r--   0        0        0      941 2023-06-11 18:40:19.306758 cycode-0.2.5.dev5/cycode/cli/utils/shell_executor.py
--rw-r--r--   0        0        0     1229 2023-06-11 18:40:19.306758 cycode-0.2.5.dev5/cycode/cli/utils/string_utils.py
--rw-r--r--   0        0        0     2700 2023-06-11 18:40:19.306758 cycode-0.2.5.dev5/cycode/cli/utils/task_timer.py
--rw-r--r--   0        0        0      815 2023-06-11 18:40:19.306758 cycode-0.2.5.dev5/cycode/cli/utils/yaml_utils.py
--rw-r--r--   0        0        0      929 2023-06-11 18:40:19.306758 cycode-0.2.5.dev5/cycode/cli/zip_file.py
--rw-r--r--   0        0        0       57 2023-06-11 18:40:19.306758 cycode-0.2.5.dev5/cycode/cyclient/__init__.py
--rw-r--r--   0        0        0     1708 2023-06-11 18:40:19.310758 cycode-0.2.5.dev5/cycode/cyclient/auth_client.py
--rw-r--r--   0        0        0     2458 2023-06-11 18:40:19.310758 cycode-0.2.5.dev5/cycode/cyclient/config.py
--rw-r--r--   0        0        0      126 2023-06-11 18:40:19.310758 cycode-0.2.5.dev5/cycode/cyclient/config.yaml
--rw-r--r--   0        0        0      119 2023-06-11 18:40:19.310758 cycode-0.2.5.dev5/cycode/cyclient/config_dev.py
--rw-r--r--   0        0        0      220 2023-06-11 18:40:19.310758 cycode-0.2.5.dev5/cycode/cyclient/cycode_client.py
--rw-r--r--   0        0        0     3617 2023-06-11 18:40:19.310758 cycode-0.2.5.dev5/cycode/cyclient/cycode_client_base.py
--rw-r--r--   0        0        0      543 2023-06-11 18:40:19.310758 cycode-0.2.5.dev5/cycode/cyclient/cycode_dev_based_client.py
--rw-r--r--   0        0        0     1705 2023-06-11 18:40:19.310758 cycode-0.2.5.dev5/cycode/cyclient/cycode_token_based_client.py
--rw-r--r--   0        0        0     9102 2023-06-11 18:40:19.310758 cycode-0.2.5.dev5/cycode/cyclient/models.py
--rw-r--r--   0        0        0     6222 2023-06-11 18:40:19.310758 cycode-0.2.5.dev5/cycode/cyclient/scan_client.py
--rw-r--r--   0        0        0        0 2023-06-11 18:40:19.310758 cycode-0.2.5.dev5/cycode/cyclient/scan_config/__init__.py
--rw-r--r--   0        0        0     1090 2023-06-11 18:40:19.310758 cycode-0.2.5.dev5/cycode/cyclient/scan_config/scan_config_base.py
--rw-r--r--   0        0        0     1021 2023-06-11 18:40:19.310758 cycode-0.2.5.dev5/cycode/cyclient/scan_config/scan_config_creator.py
--rw-r--r--   0        0        0      197 2023-06-11 18:40:19.310758 cycode-0.2.5.dev5/cycode/cyclient/utils.py
--rw-r--r--   0        0        0     2032 2023-06-11 18:40:47.955126 cycode-0.2.5.dev5/pyproject.toml
--rw-r--r--   0        0        0    33844 1970-01-01 00:00:00.000000 cycode-0.2.5.dev5/PKG-INFO
+-rw-r--r--   0        0        0    32320 2023-06-11 19:02:38.051877 cycode-0.2.5.dev6/README.md
+-rw-r--r--   0        0        0      115 2023-06-11 19:03:10.048696 cycode-0.2.5.dev6/cycode/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-11 19:02:38.051877 cycode-0.2.5.dev6/cycode/cli/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-11 19:02:38.051877 cycode-0.2.5.dev6/cycode/cli/auth/__init__.py
+-rw-r--r--   0        0        0     2813 2023-06-11 19:02:38.051877 cycode-0.2.5.dev6/cycode/cli/auth/auth_command.py
+-rw-r--r--   0        0        0     4761 2023-06-11 19:02:38.051877 cycode-0.2.5.dev6/cycode/cli/auth/auth_manager.py
+-rw-r--r--   0        0        0     1652 2023-06-11 19:02:38.051877 cycode-0.2.5.dev6/cycode/cli/ci_integrations.py
+-rw-r--r--   0        0        0    47480 2023-06-11 19:02:38.051877 cycode-0.2.5.dev6/cycode/cli/code_scanner.py
+-rw-r--r--   0        0        0      453 2023-06-11 19:02:38.051877 cycode-0.2.5.dev6/cycode/cli/config.py
+-rw-r--r--   0        0        0      387 2023-06-11 19:02:38.051877 cycode-0.2.5.dev6/cycode/cli/config.yaml
+-rw-r--r--   0        0        0     5039 2023-06-11 19:02:38.051877 cycode-0.2.5.dev6/cycode/cli/consts.py
+-rw-r--r--   0        0        0        0 2023-06-11 19:02:38.051877 cycode-0.2.5.dev6/cycode/cli/exceptions/__init__.py
+-rw-r--r--   0        0        0     1698 2023-06-11 19:02:38.051877 cycode-0.2.5.dev6/cycode/cli/exceptions/custom_exceptions.py
+-rw-r--r--   0        0        0        0 2023-06-11 19:02:38.051877 cycode-0.2.5.dev6/cycode/cli/helpers/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-11 19:02:38.051877 cycode-0.2.5.dev6/cycode/cli/helpers/maven/__init__.py
+-rw-r--r--   0        0        0     2196 2023-06-11 19:02:38.051877 cycode-0.2.5.dev6/cycode/cli/helpers/maven/base_restore_maven_dependencies.py
+-rw-r--r--   0        0        0      992 2023-06-11 19:02:38.051877 cycode-0.2.5.dev6/cycode/cli/helpers/maven/restore_gradle_dependencies.py
+-rw-r--r--   0        0        0     2993 2023-06-11 19:02:38.051877 cycode-0.2.5.dev6/cycode/cli/helpers/maven/restore_maven_dependencies.py
+-rw-r--r--   0        0        0     5835 2023-06-11 19:02:38.051877 cycode-0.2.5.dev6/cycode/cli/helpers/sca_code_scanner.py
+-rw-r--r--   0        0        0     7213 2023-06-11 19:02:38.051877 cycode-0.2.5.dev6/cycode/cli/main.py
+-rw-r--r--   0        0        0     1332 2023-06-11 19:02:38.051877 cycode-0.2.5.dev6/cycode/cli/models.py
+-rw-r--r--   0        0        0       93 2023-06-11 19:02:38.051877 cycode-0.2.5.dev6/cycode/cli/printers/__init__.py
+-rw-r--r--   0        0        0      564 2023-06-11 19:02:38.051877 cycode-0.2.5.dev6/cycode/cli/printers/base_printer.py
+-rw-r--r--   0        0        0     1709 2023-06-11 19:02:38.051877 cycode-0.2.5.dev6/cycode/cli/printers/console_printer.py
+-rw-r--r--   0        0        0     1537 2023-06-11 19:02:38.051877 cycode-0.2.5.dev6/cycode/cli/printers/json_printer.py
+-rw-r--r--   0        0        0     6108 2023-06-11 19:02:38.051877 cycode-0.2.5.dev6/cycode/cli/printers/table_printer.py
+-rw-r--r--   0        0        0     9166 2023-06-11 19:02:38.051877 cycode-0.2.5.dev6/cycode/cli/printers/text_printer.py
+-rw-r--r--   0        0        0        0 2023-06-11 19:02:38.051877 cycode-0.2.5.dev6/cycode/cli/user_settings/__init__.py
+-rw-r--r--   0        0        0      533 2023-06-11 19:02:38.051877 cycode-0.2.5.dev6/cycode/cli/user_settings/base_file_manager.py
+-rw-r--r--   0        0        0     4821 2023-06-11 19:02:38.051877 cycode-0.2.5.dev6/cycode/cli/user_settings/config_file_manager.py
+-rw-r--r--   0        0        0     6925 2023-06-11 19:02:38.051877 cycode-0.2.5.dev6/cycode/cli/user_settings/configuration_manager.py
+-rw-r--r--   0        0        0     1908 2023-06-11 19:02:38.051877 cycode-0.2.5.dev6/cycode/cli/user_settings/credentials_manager.py
+-rw-r--r--   0        0        0     6853 2023-06-11 19:02:38.051877 cycode-0.2.5.dev6/cycode/cli/user_settings/user_settings_commands.py
+-rw-r--r--   0        0        0        0 2023-06-11 19:02:38.051877 cycode-0.2.5.dev6/cycode/cli/utils/__init__.py
+-rw-r--r--   0        0        0     2162 2023-06-11 19:02:38.051877 cycode-0.2.5.dev6/cycode/cli/utils/path_utils.py
+-rw-r--r--   0        0        0      195 2023-06-11 19:02:38.051877 cycode-0.2.5.dev6/cycode/cli/utils/scan_utils.py
+-rw-r--r--   0        0        0      941 2023-06-11 19:02:38.051877 cycode-0.2.5.dev6/cycode/cli/utils/shell_executor.py
+-rw-r--r--   0        0        0     1229 2023-06-11 19:02:38.051877 cycode-0.2.5.dev6/cycode/cli/utils/string_utils.py
+-rw-r--r--   0        0        0     2700 2023-06-11 19:02:38.051877 cycode-0.2.5.dev6/cycode/cli/utils/task_timer.py
+-rw-r--r--   0        0        0      815 2023-06-11 19:02:38.051877 cycode-0.2.5.dev6/cycode/cli/utils/yaml_utils.py
+-rw-r--r--   0        0        0      929 2023-06-11 19:02:38.051877 cycode-0.2.5.dev6/cycode/cli/zip_file.py
+-rw-r--r--   0        0        0       57 2023-06-11 19:02:38.051877 cycode-0.2.5.dev6/cycode/cyclient/__init__.py
+-rw-r--r--   0        0        0     1708 2023-06-11 19:02:38.055878 cycode-0.2.5.dev6/cycode/cyclient/auth_client.py
+-rw-r--r--   0        0        0     2458 2023-06-11 19:02:38.055878 cycode-0.2.5.dev6/cycode/cyclient/config.py
+-rw-r--r--   0        0        0      126 2023-06-11 19:02:38.055878 cycode-0.2.5.dev6/cycode/cyclient/config.yaml
+-rw-r--r--   0        0        0      119 2023-06-11 19:02:38.055878 cycode-0.2.5.dev6/cycode/cyclient/config_dev.py
+-rw-r--r--   0        0        0      220 2023-06-11 19:02:38.055878 cycode-0.2.5.dev6/cycode/cyclient/cycode_client.py
+-rw-r--r--   0        0        0     3617 2023-06-11 19:02:38.055878 cycode-0.2.5.dev6/cycode/cyclient/cycode_client_base.py
+-rw-r--r--   0        0        0      543 2023-06-11 19:02:38.055878 cycode-0.2.5.dev6/cycode/cyclient/cycode_dev_based_client.py
+-rw-r--r--   0        0        0     1705 2023-06-11 19:02:38.055878 cycode-0.2.5.dev6/cycode/cyclient/cycode_token_based_client.py
+-rw-r--r--   0        0        0     9102 2023-06-11 19:02:38.055878 cycode-0.2.5.dev6/cycode/cyclient/models.py
+-rw-r--r--   0        0        0     6222 2023-06-11 19:02:38.055878 cycode-0.2.5.dev6/cycode/cyclient/scan_client.py
+-rw-r--r--   0        0        0        0 2023-06-11 19:02:38.055878 cycode-0.2.5.dev6/cycode/cyclient/scan_config/__init__.py
+-rw-r--r--   0        0        0     1090 2023-06-11 19:02:38.055878 cycode-0.2.5.dev6/cycode/cyclient/scan_config/scan_config_base.py
+-rw-r--r--   0        0        0     1021 2023-06-11 19:02:38.055878 cycode-0.2.5.dev6/cycode/cyclient/scan_config/scan_config_creator.py
+-rw-r--r--   0        0        0      197 2023-06-11 19:02:38.055878 cycode-0.2.5.dev6/cycode/cyclient/utils.py
+-rw-r--r--   0        0        0     2032 2023-06-11 19:03:10.048696 cycode-0.2.5.dev6/pyproject.toml
+-rw-r--r--   0        0        0    33844 1970-01-01 00:00:00.000000 cycode-0.2.5.dev6/PKG-INFO
```

### Comparing `cycode-0.2.5.dev5/README.md` & `cycode-0.2.5.dev6/README.md`

 * *Files identical despite different names*

### Comparing `cycode-0.2.5.dev5/cycode/cli/auth/auth_command.py` & `cycode-0.2.5.dev6/cycode/cli/auth/auth_command.py`

 * *Files identical despite different names*

### Comparing `cycode-0.2.5.dev5/cycode/cli/auth/auth_manager.py` & `cycode-0.2.5.dev6/cycode/cli/auth/auth_manager.py`

 * *Files identical despite different names*

### Comparing `cycode-0.2.5.dev5/cycode/cli/ci_integrations.py` & `cycode-0.2.5.dev6/cycode/cli/ci_integrations.py`

 * *Files identical despite different names*

### Comparing `cycode-0.2.5.dev5/cycode/cli/code_scanner.py` & `cycode-0.2.5.dev6/cycode/cli/code_scanner.py`

 * *Files identical despite different names*

### Comparing `cycode-0.2.5.dev5/cycode/cli/consts.py` & `cycode-0.2.5.dev6/cycode/cli/consts.py`

 * *Files identical despite different names*

### Comparing `cycode-0.2.5.dev5/cycode/cli/exceptions/custom_exceptions.py` & `cycode-0.2.5.dev6/cycode/cli/exceptions/custom_exceptions.py`

 * *Files identical despite different names*

### Comparing `cycode-0.2.5.dev5/cycode/cli/helpers/maven/base_restore_maven_dependencies.py` & `cycode-0.2.5.dev6/cycode/cli/helpers/maven/base_restore_maven_dependencies.py`

 * *Files identical despite different names*

### Comparing `cycode-0.2.5.dev5/cycode/cli/helpers/maven/restore_gradle_dependencies.py` & `cycode-0.2.5.dev6/cycode/cli/helpers/maven/restore_gradle_dependencies.py`

 * *Files identical despite different names*

### Comparing `cycode-0.2.5.dev5/cycode/cli/helpers/maven/restore_maven_dependencies.py` & `cycode-0.2.5.dev6/cycode/cli/helpers/maven/restore_maven_dependencies.py`

 * *Files identical despite different names*

### Comparing `cycode-0.2.5.dev5/cycode/cli/helpers/sca_code_scanner.py` & `cycode-0.2.5.dev6/cycode/cli/helpers/sca_code_scanner.py`

 * *Files identical despite different names*

### Comparing `cycode-0.2.5.dev5/cycode/cli/main.py` & `cycode-0.2.5.dev6/cycode/cli/main.py`

 * *Files identical despite different names*

### Comparing `cycode-0.2.5.dev5/cycode/cli/models.py` & `cycode-0.2.5.dev6/cycode/cli/models.py`

 * *Files identical despite different names*

### Comparing `cycode-0.2.5.dev5/cycode/cli/printers/base_printer.py` & `cycode-0.2.5.dev6/cycode/cli/printers/base_printer.py`

 * *Files identical despite different names*

### Comparing `cycode-0.2.5.dev5/cycode/cli/printers/console_printer.py` & `cycode-0.2.5.dev6/cycode/cli/printers/console_printer.py`

 * *Files identical despite different names*

### Comparing `cycode-0.2.5.dev5/cycode/cli/printers/json_printer.py` & `cycode-0.2.5.dev6/cycode/cli/printers/json_printer.py`

 * *Files identical despite different names*

### Comparing `cycode-0.2.5.dev5/cycode/cli/printers/table_printer.py` & `cycode-0.2.5.dev6/cycode/cli/printers/table_printer.py`

 * *Files identical despite different names*

### Comparing `cycode-0.2.5.dev5/cycode/cli/printers/text_printer.py` & `cycode-0.2.5.dev6/cycode/cli/printers/text_printer.py`

 * *Files identical despite different names*

### Comparing `cycode-0.2.5.dev5/cycode/cli/user_settings/base_file_manager.py` & `cycode-0.2.5.dev6/cycode/cli/user_settings/base_file_manager.py`

 * *Files identical despite different names*

### Comparing `cycode-0.2.5.dev5/cycode/cli/user_settings/config_file_manager.py` & `cycode-0.2.5.dev6/cycode/cli/user_settings/config_file_manager.py`

 * *Files identical despite different names*

### Comparing `cycode-0.2.5.dev5/cycode/cli/user_settings/configuration_manager.py` & `cycode-0.2.5.dev6/cycode/cli/user_settings/configuration_manager.py`

 * *Files identical despite different names*

### Comparing `cycode-0.2.5.dev5/cycode/cli/user_settings/credentials_manager.py` & `cycode-0.2.5.dev6/cycode/cli/user_settings/credentials_manager.py`

 * *Files identical despite different names*

### Comparing `cycode-0.2.5.dev5/cycode/cli/user_settings/user_settings_commands.py` & `cycode-0.2.5.dev6/cycode/cli/user_settings/user_settings_commands.py`

 * *Files identical despite different names*

### Comparing `cycode-0.2.5.dev5/cycode/cli/utils/path_utils.py` & `cycode-0.2.5.dev6/cycode/cli/utils/path_utils.py`

 * *Files identical despite different names*

### Comparing `cycode-0.2.5.dev5/cycode/cli/utils/shell_executor.py` & `cycode-0.2.5.dev6/cycode/cli/utils/shell_executor.py`

 * *Files identical despite different names*

### Comparing `cycode-0.2.5.dev5/cycode/cli/utils/string_utils.py` & `cycode-0.2.5.dev6/cycode/cli/utils/string_utils.py`

 * *Files identical despite different names*

### Comparing `cycode-0.2.5.dev5/cycode/cli/utils/task_timer.py` & `cycode-0.2.5.dev6/cycode/cli/utils/task_timer.py`

 * *Files identical despite different names*

### Comparing `cycode-0.2.5.dev5/cycode/cli/utils/yaml_utils.py` & `cycode-0.2.5.dev6/cycode/cli/utils/yaml_utils.py`

 * *Files identical despite different names*

### Comparing `cycode-0.2.5.dev5/cycode/cli/zip_file.py` & `cycode-0.2.5.dev6/cycode/cli/zip_file.py`

 * *Files identical despite different names*

### Comparing `cycode-0.2.5.dev5/cycode/cyclient/auth_client.py` & `cycode-0.2.5.dev6/cycode/cyclient/auth_client.py`

 * *Files identical despite different names*

### Comparing `cycode-0.2.5.dev5/cycode/cyclient/config.py` & `cycode-0.2.5.dev6/cycode/cyclient/config.py`

 * *Files identical despite different names*

### Comparing `cycode-0.2.5.dev5/cycode/cyclient/cycode_client_base.py` & `cycode-0.2.5.dev6/cycode/cyclient/cycode_client_base.py`

 * *Files identical despite different names*

### Comparing `cycode-0.2.5.dev5/cycode/cyclient/cycode_dev_based_client.py` & `cycode-0.2.5.dev6/cycode/cyclient/cycode_dev_based_client.py`

 * *Files identical despite different names*

### Comparing `cycode-0.2.5.dev5/cycode/cyclient/cycode_token_based_client.py` & `cycode-0.2.5.dev6/cycode/cyclient/cycode_token_based_client.py`

 * *Files identical despite different names*

### Comparing `cycode-0.2.5.dev5/cycode/cyclient/models.py` & `cycode-0.2.5.dev6/cycode/cyclient/models.py`

 * *Files identical despite different names*

### Comparing `cycode-0.2.5.dev5/cycode/cyclient/scan_client.py` & `cycode-0.2.5.dev6/cycode/cyclient/scan_client.py`

 * *Files identical despite different names*

### Comparing `cycode-0.2.5.dev5/cycode/cyclient/scan_config/scan_config_base.py` & `cycode-0.2.5.dev6/cycode/cyclient/scan_config/scan_config_base.py`

 * *Files identical despite different names*

### Comparing `cycode-0.2.5.dev5/cycode/cyclient/scan_config/scan_config_creator.py` & `cycode-0.2.5.dev6/cycode/cyclient/scan_config/scan_config_creator.py`

 * *Files identical despite different names*

### Comparing `cycode-0.2.5.dev5/pyproject.toml` & `cycode-0.2.5.dev6/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "cycode"
-version = "0.2.5.dev5" # DON'T TOUCH. Placeholder. Will be filled automatically on poetry build from Git Tag
+version = "0.2.5.dev6" # DON'T TOUCH. Placeholder. Will be filled automatically on poetry build from Git Tag
 description = "Perform secrets/iac scans for your sources using Cycode's engine"
 keywords=["secret-scan", "cycode", "devops", "token", "secret", "security", "cycode", "code"]
 authors = ["Cycode <support@cycode.com>"]
 license = "MIT"
 repository = "https://github.com/cycodehq-public/cycode-cli"
 readme = "README.md"
 classifiers = [
```

### Comparing `cycode-0.2.5.dev5/PKG-INFO` & `cycode-0.2.5.dev6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cycode
-Version: 0.2.5.dev5
+Version: 0.2.5.dev6
 Summary: Perform secrets/iac scans for your sources using Cycode's engine
 Home-page: https://github.com/cycodehq-public/cycode-cli
 License: MIT
 Keywords: secret-scan,cycode,devops,token,secret,security,cycode,code
 Author: Cycode
 Author-email: support@cycode.com
 Requires-Python: >=3.7,<3.12
```

