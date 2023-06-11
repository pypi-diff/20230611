# Comparing `tmp/prompton-0.0.1.tar.gz` & `tmp/prompton-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "prompton-0.0.1.tar", max compression
+gzip compressed data, was "prompton-0.0.2.tar", max compression
```

## Comparing `prompton-0.0.1.tar` & `prompton-0.0.2.tar`

### file list

```diff
@@ -1,63 +1,63 @@
--rw-r--r--   0        0        0      100 2023-06-11 19:50:26.478999 prompton-0.0.1/README.md
--rw-r--r--   0        0        0     2214 2023-06-11 18:13:36.000000 prompton-0.0.1/prompton/__init__.py
--rw-r--r--   0        0        0     2307 2023-06-11 18:13:36.000000 prompton-0.0.1/prompton/client.py
--rw-r--r--   0        0        0      348 2023-06-11 18:13:36.000000 prompton-0.0.1/prompton/core/__init__.py
--rw-r--r--   0        0        0      426 2023-06-11 18:13:36.000000 prompton-0.0.1/prompton/core/api_error.py
--rw-r--r--   0        0        0     1047 2023-06-11 18:13:36.000000 prompton-0.0.1/prompton/core/datetime_utils.py
--rw-r--r--   0        0        0     3710 2023-06-11 18:13:36.000000 prompton-0.0.1/prompton/core/jsonable_encoder.py
--rw-r--r--   0        0        0      385 2023-06-11 18:13:36.000000 prompton-0.0.1/prompton/core/remove_none_from_headers.py
--rw-r--r--   0        0        0      367 2023-06-11 18:13:36.000000 prompton-0.0.1/prompton/errors/__init__.py
--rw-r--r--   0        0        0      248 2023-06-11 18:13:36.000000 prompton-0.0.1/prompton/errors/bad_request_error.py
--rw-r--r--   0        0        0      246 2023-06-11 18:13:36.000000 prompton-0.0.1/prompton/errors/not_found_error.py
--rw-r--r--   0        0        0      250 2023-06-11 18:13:36.000000 prompton-0.0.1/prompton/errors/unauthorized_error.py
--rw-r--r--   0        0        0      257 2023-06-11 18:13:36.000000 prompton-0.0.1/prompton/errors/unprocessable_entity_error.py
--rw-r--r--   0        0        0      268 2023-06-11 18:13:36.000000 prompton-0.0.1/prompton/resources/__init__.py
--rw-r--r--   0        0        0       65 2023-06-11 18:13:36.000000 prompton-0.0.1/prompton/resources/authentication/__init__.py
--rw-r--r--   0        0        0     6099 2023-06-11 18:13:36.000000 prompton-0.0.1/prompton/resources/authentication/client.py
--rw-r--r--   0        0        0       65 2023-06-11 18:13:36.000000 prompton-0.0.1/prompton/resources/inferences/__init__.py
--rw-r--r--   0        0        0    11315 2023-06-11 18:13:36.000000 prompton-0.0.1/prompton/resources/inferences/client.py
--rw-r--r--   0        0        0       65 2023-06-11 18:13:36.000000 prompton-0.0.1/prompton/resources/orgs/__init__.py
--rw-r--r--   0        0        0    14700 2023-06-11 18:13:36.000000 prompton-0.0.1/prompton/resources/orgs/client.py
--rw-r--r--   0        0        0       65 2023-06-11 18:13:36.000000 prompton-0.0.1/prompton/resources/prompt_versions/__init__.py
--rw-r--r--   0        0        0    16684 2023-06-11 18:13:36.000000 prompton-0.0.1/prompton/resources/prompt_versions/client.py
--rw-r--r--   0        0        0       65 2023-06-11 18:13:36.000000 prompton-0.0.1/prompton/resources/prompts/__init__.py
--rw-r--r--   0        0        0    15826 2023-06-11 18:13:36.000000 prompton-0.0.1/prompton/resources/prompts/client.py
--rw-r--r--   0        0        0       65 2023-06-11 18:13:36.000000 prompton-0.0.1/prompton/resources/server_status/__init__.py
--rw-r--r--   0        0        0     2307 2023-06-11 18:13:36.000000 prompton-0.0.1/prompton/resources/server_status/client.py
--rw-r--r--   0        0        0       65 2023-06-11 18:13:36.000000 prompton-0.0.1/prompton/resources/users/__init__.py
--rw-r--r--   0        0        0    13165 2023-06-11 18:13:36.000000 prompton-0.0.1/prompton/resources/users/client.py
--rw-r--r--   0        0        0     2747 2023-06-11 18:13:36.000000 prompton-0.0.1/prompton/types/__init__.py
--rw-r--r--   0        0        0      900 2023-06-11 18:13:36.000000 prompton-0.0.1/prompton/types/api_status_response.py
--rw-r--r--   0        0        0      936 2023-06-11 18:13:36.000000 prompton-0.0.1/prompton/types/body_get_access_token_extended_token_post.py
--rw-r--r--   0        0        0     1233 2023-06-11 18:13:36.000000 prompton-0.0.1/prompton/types/chat_gpt_chat_completition_config.py
--rw-r--r--   0        0        0      152 2023-06-11 18:13:36.000000 prompton-0.0.1/prompton/types/chat_gpt_chat_completition_config_stop.py
--rw-r--r--   0        0        0     1417 2023-06-11 18:13:36.000000 prompton-0.0.1/prompton/types/chat_gpt_chat_completition_request.py
--rw-r--r--   0        0        0      153 2023-06-11 18:13:36.000000 prompton-0.0.1/prompton/types/chat_gpt_chat_completition_request_stop.py
--rw-r--r--   0        0        0     1012 2023-06-11 18:13:36.000000 prompton-0.0.1/prompton/types/chat_gpt_chat_completition_response.py
--rw-r--r--   0        0        0      856 2023-06-11 18:13:36.000000 prompton-0.0.1/prompton/types/chat_gpt_completition_choice.py
--rw-r--r--   0        0        0      843 2023-06-11 18:13:36.000000 prompton-0.0.1/prompton/types/chat_gpt_message.py
--rw-r--r--   0        0        0      666 2023-06-11 18:13:36.000000 prompton-0.0.1/prompton/types/chat_gpt_role.py
--rw-r--r--   0        0        0      809 2023-06-11 18:13:36.000000 prompton-0.0.1/prompton/types/chat_gpt_token_usage.py
--rw-r--r--   0        0        0      773 2023-06-11 18:13:36.000000 prompton-0.0.1/prompton/types/db_status.py
--rw-r--r--   0        0        0      843 2023-06-11 18:13:36.000000 prompton-0.0.1/prompton/types/http_validation_error.py
--rw-r--r--   0        0        0      926 2023-06-11 18:13:36.000000 prompton-0.0.1/prompton/types/inference_post_response.py
--rw-r--r--   0        0        0      293 2023-06-11 18:13:36.000000 prompton-0.0.1/prompton/types/inference_post_response_response.py
--rw-r--r--   0        0        0     1687 2023-06-11 18:13:36.000000 prompton-0.0.1/prompton/types/inference_read.py
--rw-r--r--   0        0        0      285 2023-06-11 18:13:36.000000 prompton-0.0.1/prompton/types/inference_read_response.py
--rw-r--r--   0        0        0      965 2023-06-11 18:13:36.000000 prompton-0.0.1/prompton/types/inference_request_data.py
--rw-r--r--   0        0        0     1308 2023-06-11 18:13:36.000000 prompton-0.0.1/prompton/types/inference_response_data.py
--rw-r--r--   0        0        0     1051 2023-06-11 18:13:36.000000 prompton-0.0.1/prompton/types/inference_response_error.py
--rw-r--r--   0        0        0     1049 2023-06-11 18:13:36.000000 prompton-0.0.1/prompton/types/inference_response_status.py
--rw-r--r--   0        0        0     1076 2023-06-11 18:13:36.000000 prompton-0.0.1/prompton/types/org_read.py
--rw-r--r--   0        0        0     1143 2023-06-11 18:13:36.000000 prompton-0.0.1/prompton/types/prompt_read.py
--rw-r--r--   0        0        0      507 2023-06-11 18:13:36.000000 prompton-0.0.1/prompton/types/prompt_status.py
--rw-r--r--   0        0        0      411 2023-06-11 18:13:36.000000 prompton-0.0.1/prompton/types/prompt_version_providers.py
--rw-r--r--   0        0        0     1610 2023-06-11 18:13:36.000000 prompton-0.0.1/prompton/types/prompt_version_read.py
--rw-r--r--   0        0        0      837 2023-06-11 18:13:36.000000 prompton-0.0.1/prompton/types/prompt_version_status.py
--rw-r--r--   0        0        0      767 2023-06-11 18:13:36.000000 prompton-0.0.1/prompton/types/token.py
--rw-r--r--   0        0        0     1181 2023-06-11 18:13:36.000000 prompton-0.0.1/prompton/types/user_read.py
--rw-r--r--   0        0        0      686 2023-06-11 18:13:36.000000 prompton-0.0.1/prompton/types/user_roles.py
--rw-r--r--   0        0        0      869 2023-06-11 18:13:36.000000 prompton-0.0.1/prompton/types/validation_error.py
--rw-r--r--   0        0        0      128 2023-06-11 18:13:36.000000 prompton-0.0.1/prompton/types/validation_error_loc_item.py
--rw-r--r--   0        0        0      450 2023-06-11 19:36:43.562204 prompton-0.0.1/pyproject.toml
--rw-r--r--   0        0        0      526 1970-01-01 00:00:00.000000 prompton-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0      100 2023-06-11 19:50:26.478999 prompton-0.0.2/README.md
+-rw-r--r--   0        0        0     2214 2023-06-11 18:13:36.000000 prompton-0.0.2/prompton/__init__.py
+-rw-r--r--   0        0        0     2307 2023-06-11 18:13:36.000000 prompton-0.0.2/prompton/client.py
+-rw-r--r--   0        0        0      348 2023-06-11 18:13:36.000000 prompton-0.0.2/prompton/core/__init__.py
+-rw-r--r--   0        0        0      426 2023-06-11 18:13:36.000000 prompton-0.0.2/prompton/core/api_error.py
+-rw-r--r--   0        0        0     1047 2023-06-11 18:13:36.000000 prompton-0.0.2/prompton/core/datetime_utils.py
+-rw-r--r--   0        0        0     3710 2023-06-11 18:13:36.000000 prompton-0.0.2/prompton/core/jsonable_encoder.py
+-rw-r--r--   0        0        0      385 2023-06-11 18:13:36.000000 prompton-0.0.2/prompton/core/remove_none_from_headers.py
+-rw-r--r--   0        0        0      367 2023-06-11 18:13:36.000000 prompton-0.0.2/prompton/errors/__init__.py
+-rw-r--r--   0        0        0      248 2023-06-11 18:13:36.000000 prompton-0.0.2/prompton/errors/bad_request_error.py
+-rw-r--r--   0        0        0      246 2023-06-11 18:13:36.000000 prompton-0.0.2/prompton/errors/not_found_error.py
+-rw-r--r--   0        0        0      250 2023-06-11 18:13:36.000000 prompton-0.0.2/prompton/errors/unauthorized_error.py
+-rw-r--r--   0        0        0      257 2023-06-11 18:13:36.000000 prompton-0.0.2/prompton/errors/unprocessable_entity_error.py
+-rw-r--r--   0        0        0      268 2023-06-11 18:13:36.000000 prompton-0.0.2/prompton/resources/__init__.py
+-rw-r--r--   0        0        0       65 2023-06-11 18:13:36.000000 prompton-0.0.2/prompton/resources/authentication/__init__.py
+-rw-r--r--   0        0        0     6099 2023-06-11 18:13:36.000000 prompton-0.0.2/prompton/resources/authentication/client.py
+-rw-r--r--   0        0        0       65 2023-06-11 18:13:36.000000 prompton-0.0.2/prompton/resources/inferences/__init__.py
+-rw-r--r--   0        0        0    11315 2023-06-11 18:13:36.000000 prompton-0.0.2/prompton/resources/inferences/client.py
+-rw-r--r--   0        0        0       65 2023-06-11 18:13:36.000000 prompton-0.0.2/prompton/resources/orgs/__init__.py
+-rw-r--r--   0        0        0    14700 2023-06-11 18:13:36.000000 prompton-0.0.2/prompton/resources/orgs/client.py
+-rw-r--r--   0        0        0       65 2023-06-11 18:13:36.000000 prompton-0.0.2/prompton/resources/prompt_versions/__init__.py
+-rw-r--r--   0        0        0    16684 2023-06-11 18:13:36.000000 prompton-0.0.2/prompton/resources/prompt_versions/client.py
+-rw-r--r--   0        0        0       65 2023-06-11 18:13:36.000000 prompton-0.0.2/prompton/resources/prompts/__init__.py
+-rw-r--r--   0        0        0    15826 2023-06-11 18:13:36.000000 prompton-0.0.2/prompton/resources/prompts/client.py
+-rw-r--r--   0        0        0       65 2023-06-11 18:13:36.000000 prompton-0.0.2/prompton/resources/server_status/__init__.py
+-rw-r--r--   0        0        0     2307 2023-06-11 18:13:36.000000 prompton-0.0.2/prompton/resources/server_status/client.py
+-rw-r--r--   0        0        0       65 2023-06-11 18:13:36.000000 prompton-0.0.2/prompton/resources/users/__init__.py
+-rw-r--r--   0        0        0    13165 2023-06-11 18:13:36.000000 prompton-0.0.2/prompton/resources/users/client.py
+-rw-r--r--   0        0        0     2747 2023-06-11 18:13:36.000000 prompton-0.0.2/prompton/types/__init__.py
+-rw-r--r--   0        0        0      900 2023-06-11 18:13:36.000000 prompton-0.0.2/prompton/types/api_status_response.py
+-rw-r--r--   0        0        0      936 2023-06-11 18:13:36.000000 prompton-0.0.2/prompton/types/body_get_access_token_extended_token_post.py
+-rw-r--r--   0        0        0     1233 2023-06-11 18:13:36.000000 prompton-0.0.2/prompton/types/chat_gpt_chat_completition_config.py
+-rw-r--r--   0        0        0      152 2023-06-11 18:13:36.000000 prompton-0.0.2/prompton/types/chat_gpt_chat_completition_config_stop.py
+-rw-r--r--   0        0        0     1417 2023-06-11 18:13:36.000000 prompton-0.0.2/prompton/types/chat_gpt_chat_completition_request.py
+-rw-r--r--   0        0        0      153 2023-06-11 18:13:36.000000 prompton-0.0.2/prompton/types/chat_gpt_chat_completition_request_stop.py
+-rw-r--r--   0        0        0     1012 2023-06-11 18:13:36.000000 prompton-0.0.2/prompton/types/chat_gpt_chat_completition_response.py
+-rw-r--r--   0        0        0      856 2023-06-11 18:13:36.000000 prompton-0.0.2/prompton/types/chat_gpt_completition_choice.py
+-rw-r--r--   0        0        0      843 2023-06-11 18:13:36.000000 prompton-0.0.2/prompton/types/chat_gpt_message.py
+-rw-r--r--   0        0        0      666 2023-06-11 18:13:36.000000 prompton-0.0.2/prompton/types/chat_gpt_role.py
+-rw-r--r--   0        0        0      809 2023-06-11 18:13:36.000000 prompton-0.0.2/prompton/types/chat_gpt_token_usage.py
+-rw-r--r--   0        0        0      773 2023-06-11 18:13:36.000000 prompton-0.0.2/prompton/types/db_status.py
+-rw-r--r--   0        0        0      843 2023-06-11 18:13:36.000000 prompton-0.0.2/prompton/types/http_validation_error.py
+-rw-r--r--   0        0        0      926 2023-06-11 18:13:36.000000 prompton-0.0.2/prompton/types/inference_post_response.py
+-rw-r--r--   0        0        0      293 2023-06-11 18:13:36.000000 prompton-0.0.2/prompton/types/inference_post_response_response.py
+-rw-r--r--   0        0        0     1687 2023-06-11 18:13:36.000000 prompton-0.0.2/prompton/types/inference_read.py
+-rw-r--r--   0        0        0      285 2023-06-11 18:13:36.000000 prompton-0.0.2/prompton/types/inference_read_response.py
+-rw-r--r--   0        0        0      965 2023-06-11 18:13:36.000000 prompton-0.0.2/prompton/types/inference_request_data.py
+-rw-r--r--   0        0        0     1308 2023-06-11 18:13:36.000000 prompton-0.0.2/prompton/types/inference_response_data.py
+-rw-r--r--   0        0        0     1051 2023-06-11 18:13:36.000000 prompton-0.0.2/prompton/types/inference_response_error.py
+-rw-r--r--   0        0        0     1049 2023-06-11 18:13:36.000000 prompton-0.0.2/prompton/types/inference_response_status.py
+-rw-r--r--   0        0        0     1076 2023-06-11 18:13:36.000000 prompton-0.0.2/prompton/types/org_read.py
+-rw-r--r--   0        0        0     1143 2023-06-11 18:13:36.000000 prompton-0.0.2/prompton/types/prompt_read.py
+-rw-r--r--   0        0        0      507 2023-06-11 18:13:36.000000 prompton-0.0.2/prompton/types/prompt_status.py
+-rw-r--r--   0        0        0      411 2023-06-11 18:13:36.000000 prompton-0.0.2/prompton/types/prompt_version_providers.py
+-rw-r--r--   0        0        0     1610 2023-06-11 18:13:36.000000 prompton-0.0.2/prompton/types/prompt_version_read.py
+-rw-r--r--   0        0        0      837 2023-06-11 18:13:36.000000 prompton-0.0.2/prompton/types/prompt_version_status.py
+-rw-r--r--   0        0        0      767 2023-06-11 18:13:36.000000 prompton-0.0.2/prompton/types/token.py
+-rw-r--r--   0        0        0     1181 2023-06-11 18:13:36.000000 prompton-0.0.2/prompton/types/user_read.py
+-rw-r--r--   0        0        0      686 2023-06-11 18:13:36.000000 prompton-0.0.2/prompton/types/user_roles.py
+-rw-r--r--   0        0        0      869 2023-06-11 18:13:36.000000 prompton-0.0.2/prompton/types/validation_error.py
+-rw-r--r--   0        0        0      128 2023-06-11 18:13:36.000000 prompton-0.0.2/prompton/types/validation_error_loc_item.py
+-rw-r--r--   0        0        0      451 2023-06-11 20:06:50.881065 prompton-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0      572 1970-01-01 00:00:00.000000 prompton-0.0.2/PKG-INFO
```

### Comparing `prompton-0.0.1/prompton/__init__.py` & `prompton-0.0.2/prompton/__init__.py`

 * *Files identical despite different names*

### Comparing `prompton-0.0.1/prompton/client.py` & `prompton-0.0.2/prompton/client.py`

 * *Files identical despite different names*

### Comparing `prompton-0.0.1/prompton/core/datetime_utils.py` & `prompton-0.0.2/prompton/core/datetime_utils.py`

 * *Files identical despite different names*

### Comparing `prompton-0.0.1/prompton/core/jsonable_encoder.py` & `prompton-0.0.2/prompton/core/jsonable_encoder.py`

 * *Files identical despite different names*

### Comparing `prompton-0.0.1/prompton/resources/authentication/client.py` & `prompton-0.0.2/prompton/resources/authentication/client.py`

 * *Files identical despite different names*

### Comparing `prompton-0.0.1/prompton/resources/inferences/client.py` & `prompton-0.0.2/prompton/resources/inferences/client.py`

 * *Files identical despite different names*

### Comparing `prompton-0.0.1/prompton/resources/orgs/client.py` & `prompton-0.0.2/prompton/resources/orgs/client.py`

 * *Files identical despite different names*

### Comparing `prompton-0.0.1/prompton/resources/prompt_versions/client.py` & `prompton-0.0.2/prompton/resources/prompt_versions/client.py`

 * *Files identical despite different names*

### Comparing `prompton-0.0.1/prompton/resources/prompts/client.py` & `prompton-0.0.2/prompton/resources/prompts/client.py`

 * *Files identical despite different names*

### Comparing `prompton-0.0.1/prompton/resources/server_status/client.py` & `prompton-0.0.2/prompton/resources/server_status/client.py`

 * *Files identical despite different names*

### Comparing `prompton-0.0.1/prompton/resources/users/client.py` & `prompton-0.0.2/prompton/resources/users/client.py`

 * *Files identical despite different names*

### Comparing `prompton-0.0.1/prompton/types/__init__.py` & `prompton-0.0.2/prompton/types/__init__.py`

 * *Files identical despite different names*

### Comparing `prompton-0.0.1/prompton/types/api_status_response.py` & `prompton-0.0.2/prompton/types/api_status_response.py`

 * *Files identical despite different names*

### Comparing `prompton-0.0.1/prompton/types/body_get_access_token_extended_token_post.py` & `prompton-0.0.2/prompton/types/body_get_access_token_extended_token_post.py`

 * *Files identical despite different names*

### Comparing `prompton-0.0.1/prompton/types/chat_gpt_chat_completition_config.py` & `prompton-0.0.2/prompton/types/chat_gpt_chat_completition_config.py`

 * *Files identical despite different names*

### Comparing `prompton-0.0.1/prompton/types/chat_gpt_chat_completition_request.py` & `prompton-0.0.2/prompton/types/chat_gpt_chat_completition_request.py`

 * *Files identical despite different names*

### Comparing `prompton-0.0.1/prompton/types/chat_gpt_chat_completition_response.py` & `prompton-0.0.2/prompton/types/chat_gpt_chat_completition_response.py`

 * *Files identical despite different names*

### Comparing `prompton-0.0.1/prompton/types/chat_gpt_completition_choice.py` & `prompton-0.0.2/prompton/types/chat_gpt_completition_choice.py`

 * *Files identical despite different names*

### Comparing `prompton-0.0.1/prompton/types/chat_gpt_message.py` & `prompton-0.0.2/prompton/types/chat_gpt_message.py`

 * *Files identical despite different names*

### Comparing `prompton-0.0.1/prompton/types/chat_gpt_role.py` & `prompton-0.0.2/prompton/types/chat_gpt_role.py`

 * *Files identical despite different names*

### Comparing `prompton-0.0.1/prompton/types/chat_gpt_token_usage.py` & `prompton-0.0.2/prompton/types/chat_gpt_token_usage.py`

 * *Files identical despite different names*

### Comparing `prompton-0.0.1/prompton/types/db_status.py` & `prompton-0.0.2/prompton/types/db_status.py`

 * *Files identical despite different names*

### Comparing `prompton-0.0.1/prompton/types/http_validation_error.py` & `prompton-0.0.2/prompton/types/http_validation_error.py`

 * *Files identical despite different names*

### Comparing `prompton-0.0.1/prompton/types/inference_post_response.py` & `prompton-0.0.2/prompton/types/inference_post_response.py`

 * *Files identical despite different names*

### Comparing `prompton-0.0.1/prompton/types/inference_read.py` & `prompton-0.0.2/prompton/types/inference_read.py`

 * *Files identical despite different names*

### Comparing `prompton-0.0.1/prompton/types/inference_request_data.py` & `prompton-0.0.2/prompton/types/inference_request_data.py`

 * *Files identical despite different names*

### Comparing `prompton-0.0.1/prompton/types/inference_response_data.py` & `prompton-0.0.2/prompton/types/inference_response_data.py`

 * *Files identical despite different names*

### Comparing `prompton-0.0.1/prompton/types/inference_response_error.py` & `prompton-0.0.2/prompton/types/inference_response_error.py`

 * *Files identical despite different names*

### Comparing `prompton-0.0.1/prompton/types/inference_response_status.py` & `prompton-0.0.2/prompton/types/inference_response_status.py`

 * *Files identical despite different names*

### Comparing `prompton-0.0.1/prompton/types/org_read.py` & `prompton-0.0.2/prompton/types/org_read.py`

 * *Files identical despite different names*

### Comparing `prompton-0.0.1/prompton/types/prompt_read.py` & `prompton-0.0.2/prompton/types/prompt_read.py`

 * *Files identical despite different names*

### Comparing `prompton-0.0.1/prompton/types/prompt_version_read.py` & `prompton-0.0.2/prompton/types/prompt_version_read.py`

 * *Files identical despite different names*

### Comparing `prompton-0.0.1/prompton/types/prompt_version_status.py` & `prompton-0.0.2/prompton/types/prompt_version_status.py`

 * *Files identical despite different names*

### Comparing `prompton-0.0.1/prompton/types/token.py` & `prompton-0.0.2/prompton/types/token.py`

 * *Files identical despite different names*

### Comparing `prompton-0.0.1/prompton/types/user_read.py` & `prompton-0.0.2/prompton/types/user_read.py`

 * *Files identical despite different names*

### Comparing `prompton-0.0.1/prompton/types/user_roles.py` & `prompton-0.0.2/prompton/types/user_roles.py`

 * *Files identical despite different names*

### Comparing `prompton-0.0.1/prompton/types/validation_error.py` & `prompton-0.0.2/prompton/types/validation_error.py`

 * *Files identical despite different names*

### Comparing `prompton-0.0.1/PKG-INFO` & `prompton-0.0.2/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 Metadata-Version: 2.1
 Name: prompton
-Version: 0.0.1
+Version: 0.0.2
 Summary: Chat prompt template evaluation and inference monitoring
 Author: PromptOn
 Author-email: hello@prompton.ai
-Requires-Python: >=3.11,<4.0
+Requires-Python: >=3.10
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: httpx (>=0.24.1,<0.25.0)
 Requires-Dist: pydantic[email] (>=1.10.8,<2.0.0)
 Description-Content-Type: text/markdown
 
 # PromptOn API - Python client
```

