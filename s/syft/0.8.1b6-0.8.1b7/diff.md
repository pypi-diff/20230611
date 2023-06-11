# Comparing `tmp/syft-0.8.1b6.tar.gz` & `tmp/syft-0.8.1b7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "syft-0.8.1b6.tar", last modified: Sun Jun  4 12:44:27 2023, max compression
+gzip compressed data, was "syft-0.8.1b7.tar", last modified: Sun Jun 11 12:25:37 2023, max compression
```

## Comparing `syft-0.8.1b6.tar` & `syft-0.8.1b7.tar`

### file list

```diff
@@ -1,193 +1,194 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 12:44:27.013247 syft-0.8.1b6/
--rw-r--r--   0 runner    (1001) docker     (123)    11843 2023-06-04 12:42:01.000000 syft-0.8.1b6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       75 2023-06-04 12:42:01.000000 syft-0.8.1b6/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    15457 2023-06-04 12:44:27.013247 syft-0.8.1b6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    14801 2023-06-04 12:42:01.000000 syft-0.8.1b6/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      272 2023-06-04 12:42:01.000000 syft-0.8.1b6/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     3114 2023-06-04 12:44:27.017247 syft-0.8.1b6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      107 2023-06-04 12:42:01.000000 syft-0.8.1b6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 12:44:26.957247 syft-0.8.1b6/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 12:44:26.965247 syft-0.8.1b6/src/syft/
--rw-r--r--   0 runner    (1001) docker     (123)      580 2023-06-04 12:42:17.000000 syft-0.8.1b6/src/syft/VERSION
--rw-r--r--   0 runner    (1001) docker     (123)     4651 2023-06-04 12:42:17.000000 syft-0.8.1b6/src/syft/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      518 2023-06-04 12:42:01.000000 syft-0.8.1b6/src/syft/abstract_node.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 12:44:26.969246 syft-0.8.1b6/src/syft/capnp/
--rw-r--r--   0 runner    (1001) docker     (123)      270 2023-06-04 12:42:01.000000 syft-0.8.1b6/src/syft/capnp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       75 2023-06-04 12:42:01.000000 syft-0.8.1b6/src/syft/capnp/iterable.capnp
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-06-04 12:42:01.000000 syft-0.8.1b6/src/syft/capnp/kv_iterable.capnp
--rw-r--r--   0 runner    (1001) docker     (123)      186 2023-06-04 12:42:01.000000 syft-0.8.1b6/src/syft/capnp/recursive_serde.capnp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 12:44:26.973246 syft-0.8.1b6/src/syft/client/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-04 12:42:01.000000 syft-0.8.1b6/src/syft/client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    24407 2023-06-04 12:42:01.000000 syft-0.8.1b6/src/syft/client/api.py
--rw-r--r--   0 runner    (1001) docker     (123)    23619 2023-06-04 12:42:01.000000 syft-0.8.1b6/src/syft/client/client.py
--rw-r--r--   0 runner    (1001) docker     (123)      568 2023-06-04 12:42:01.000000 syft-0.8.1b6/src/syft/client/connection.py
--rw-r--r--   0 runner    (1001) docker     (123)      650 2023-06-04 12:42:01.000000 syft-0.8.1b6/src/syft/client/deploy.py
--rw-r--r--   0 runner    (1001) docker     (123)    10796 2023-06-04 12:42:01.000000 syft-0.8.1b6/src/syft/client/registry.py
--rw-r--r--   0 runner    (1001) docker     (123)     2623 2023-06-04 12:42:01.000000 syft-0.8.1b6/src/syft/client/search.py
--rw-r--r--   0 runner    (1001) docker     (123)      549 2023-06-04 12:42:01.000000 syft-0.8.1b6/src/syft/client/user_settings.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 12:44:26.973246 syft-0.8.1b6/src/syft/external/
--rw-r--r--   0 runner    (1001) docker     (123)     1735 2023-06-04 12:42:01.000000 syft-0.8.1b6/src/syft/external/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 12:44:26.977247 syft-0.8.1b6/src/syft/external/oblv/
--rw-r--r--   0 runner    (1001) docker     (123)      860 2023-06-04 12:42:01.000000 syft-0.8.1b6/src/syft/external/oblv/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      284 2023-06-04 12:42:01.000000 syft-0.8.1b6/src/syft/external/oblv/auth.py
--rw-r--r--   0 runner    (1001) docker     (123)      212 2023-06-04 12:42:01.000000 syft-0.8.1b6/src/syft/external/oblv/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     4835 2023-06-04 12:42:01.000000 syft-0.8.1b6/src/syft/external/oblv/deployment.py
--rw-r--r--   0 runner    (1001) docker     (123)    12360 2023-06-04 12:42:01.000000 syft-0.8.1b6/src/syft/external/oblv/deployment_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     1800 2023-06-04 12:42:01.000000 syft-0.8.1b6/src/syft/external/oblv/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)      489 2023-06-04 12:42:01.000000 syft-0.8.1b6/src/syft/external/oblv/oblv_keys.py
--rw-r--r--   0 runner    (1001) docker     (123)     2280 2023-06-04 12:42:01.000000 syft-0.8.1b6/src/syft/external/oblv/oblv_keys_stash.py
--rw-r--r--   0 runner    (1001) docker     (123)     7462 2023-06-04 12:42:01.000000 syft-0.8.1b6/src/syft/external/oblv/oblv_proxy.py
--rw-r--r--   0 runner    (1001) docker     (123)    15930 2023-06-04 12:42:01.000000 syft-0.8.1b6/src/syft/external/oblv/oblv_service.py
--rw-r--r--   0 runner    (1001) docker     (123)     1146 2023-06-04 12:42:01.000000 syft-0.8.1b6/src/syft/gevent_patch.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 12:44:26.981247 syft-0.8.1b6/src/syft/node/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-04 12:42:01.000000 syft-0.8.1b6/src/syft/node/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2641 2023-06-04 12:42:01.000000 syft-0.8.1b6/src/syft/node/credentials.py
--rw-r--r--   0 runner    (1001) docker     (123)      152 2023-06-04 12:42:01.000000 syft-0.8.1b6/src/syft/node/domain.py
--rw-r--r--   0 runner    (1001) docker     (123)      687 2023-06-04 12:42:01.000000 syft-0.8.1b6/src/syft/node/gateway.py
--rw-r--r--   0 runner    (1001) docker     (123)    28362 2023-06-04 12:42:01.000000 syft-0.8.1b6/src/syft/node/node.py
--rw-r--r--   0 runner    (1001) docker     (123)     6979 2023-06-04 12:42:01.000000 syft-0.8.1b6/src/syft/node/routes.py
--rw-r--r--   0 runner    (1001) docker     (123)     2064 2023-06-04 12:42:01.000000 syft-0.8.1b6/src/syft/node/run.py
--rw-r--r--   0 runner    (1001) docker     (123)     6180 2023-06-04 12:42:01.000000 syft-0.8.1b6/src/syft/node/server.py
--rw-r--r--   0 runner    (1001) docker     (123)      127 2023-06-04 12:42:01.000000 syft-0.8.1b6/src/syft/node/worker.py
--rw-r--r--   0 runner    (1001) docker     (123)     1001 2023-06-04 12:42:01.000000 syft-0.8.1b6/src/syft/node/worker_settings.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 12:44:26.985247 syft-0.8.1b6/src/syft/serde/
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-06-04 12:42:01.000000 syft-0.8.1b6/src/syft/serde/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3597 2023-06-04 12:42:01.000000 syft-0.8.1b6/src/syft/serde/array.py
--rw-r--r--   0 runner    (1001) docker     (123)     4099 2023-06-04 12:42:01.000000 syft-0.8.1b6/src/syft/serde/arrow.py
--rw-r--r--   0 runner    (1001) docker     (123)      298 2023-06-04 12:42:01.000000 syft-0.8.1b6/src/syft/serde/capnp.py
--rw-r--r--   0 runner    (1001) docker     (123)      722 2023-06-04 12:42:01.000000 syft-0.8.1b6/src/syft/serde/deserialize.py
--rw-r--r--   0 runner    (1001) docker     (123)     1230 2023-06-04 12:42:01.000000 syft-0.8.1b6/src/syft/serde/lib_permissions.py
--rw-r--r--   0 runner    (1001) docker     (123)    11663 2023-06-04 12:42:01.000000 syft-0.8.1b6/src/syft/serde/lib_service_registry.py
--rw-r--r--   0 runner    (1001) docker     (123)      875 2023-06-04 12:42:01.000000 syft-0.8.1b6/src/syft/serde/mock.py
--rw-r--r--   0 runner    (1001) docker     (123)    11484 2023-06-04 12:42:01.000000 syft-0.8.1b6/src/syft/serde/recursive.py
--rw-r--r--   0 runner    (1001) docker     (123)    10253 2023-06-04 12:42:01.000000 syft-0.8.1b6/src/syft/serde/recursive_primitives.py
--rw-r--r--   0 runner    (1001) docker     (123)     1822 2023-06-04 12:42:01.000000 syft-0.8.1b6/src/syft/serde/serializable.py
--rw-r--r--   0 runner    (1001) docker     (123)      369 2023-06-04 12:42:01.000000 syft-0.8.1b6/src/syft/serde/serialize.py
--rw-r--r--   0 runner    (1001) docker     (123)     4959 2023-06-04 12:42:01.000000 syft-0.8.1b6/src/syft/serde/signature.py
--rw-r--r--   0 runner    (1001) docker     (123)     4885 2023-06-04 12:42:01.000000 syft-0.8.1b6/src/syft/serde/third_party.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 12:44:26.985247 syft-0.8.1b6/src/syft/service/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-04 12:42:01.000000 syft-0.8.1b6/src/syft/service/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 12:44:26.989246 syft-0.8.1b6/src/syft/service/action/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-04 12:42:01.000000 syft-0.8.1b6/src/syft/service/action/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      703 2023-06-04 12:42:01.000000 syft-0.8.1b6/src/syft/service/action/action_data_empty.py
--rw-r--r--   0 runner    (1001) docker     (123)    16706 2023-06-04 12:42:01.000000 syft-0.8.1b6/src/syft/service/action/action_graph.py
--rw-r--r--   0 runner    (1001) docker     (123)     6874 2023-06-04 12:42:01.000000 syft-0.8.1b6/src/syft/service/action/action_graph_service.py
--rw-r--r--   0 runner    (1001) docker     (123)    46765 2023-06-04 12:42:01.000000 syft-0.8.1b6/src/syft/service/action/action_object.py
--rw-r--r--   0 runner    (1001) docker     (123)     2416 2023-06-04 12:42:01.000000 syft-0.8.1b6/src/syft/service/action/action_permissions.py
--rw-r--r--   0 runner    (1001) docker     (123)    26970 2023-06-04 12:42:01.000000 syft-0.8.1b6/src/syft/service/action/action_service.py
--rw-r--r--   0 runner    (1001) docker     (123)    10168 2023-06-04 12:42:01.000000 syft-0.8.1b6/src/syft/service/action/action_store.py
--rw-r--r--   0 runner    (1001) docker     (123)     1165 2023-06-04 12:42:01.000000 syft-0.8.1b6/src/syft/service/action/action_types.py
--rw-r--r--   0 runner    (1001) docker     (123)     3889 2023-06-04 12:42:01.000000 syft-0.8.1b6/src/syft/service/action/numpy.py
--rw-r--r--   0 runner    (1001) docker     (123)     2233 2023-06-04 12:42:01.000000 syft-0.8.1b6/src/syft/service/action/pandas.py
--rw-r--r--   0 runner    (1001) docker     (123)     2915 2023-06-04 12:42:01.000000 syft-0.8.1b6/src/syft/service/action/plan.py
--rw-r--r--   0 runner    (1001) docker     (123)     4951 2023-06-04 12:42:01.000000 syft-0.8.1b6/src/syft/service/action/verification.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 12:44:26.993247 syft-0.8.1b6/src/syft/service/code/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-04 12:42:01.000000 syft-0.8.1b6/src/syft/service/code/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      236 2023-06-04 12:42:01.000000 syft-0.8.1b6/src/syft/service/code/code_parse.py
--rw-r--r--   0 runner    (1001) docker     (123)      785 2023-06-04 12:42:01.000000 syft-0.8.1b6/src/syft/service/code/unparse.py
--rw-r--r--   0 runner    (1001) docker     (123)    22127 2023-06-04 12:42:01.000000 syft-0.8.1b6/src/syft/service/code/user_code.py
--rw-r--r--   0 runner    (1001) docker     (123)     1756 2023-06-04 12:42:01.000000 syft-0.8.1b6/src/syft/service/code/user_code_parse.py
--rw-r--r--   0 runner    (1001) docker     (123)     9272 2023-06-04 12:42:01.000000 syft-0.8.1b6/src/syft/service/code/user_code_service.py
--rw-r--r--   0 runner    (1001) docker     (123)     1446 2023-06-04 12:42:01.000000 syft-0.8.1b6/src/syft/service/code/user_code_stash.py
--rw-r--r--   0 runner    (1001) docker     (123)     1782 2023-06-04 12:42:01.000000 syft-0.8.1b6/src/syft/service/context.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 12:44:26.993247 syft-0.8.1b6/src/syft/service/data_subject/
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-06-04 12:42:01.000000 syft-0.8.1b6/src/syft/service/data_subject/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3669 2023-06-04 12:42:01.000000 syft-0.8.1b6/src/syft/service/data_subject/data_subject.py
--rw-r--r--   0 runner    (1001) docker     (123)      870 2023-06-04 12:42:01.000000 syft-0.8.1b6/src/syft/service/data_subject/data_subject_member.py
--rw-r--r--   0 runner    (1001) docker     (123)     3215 2023-06-04 12:42:01.000000 syft-0.8.1b6/src/syft/service/data_subject/data_subject_member_service.py
--rw-r--r--   0 runner    (1001) docker     (123)     5006 2023-06-04 12:42:01.000000 syft-0.8.1b6/src/syft/service/data_subject/data_subject_service.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 12:44:26.993247 syft-0.8.1b6/src/syft/service/dataset/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-04 12:42:01.000000 syft-0.8.1b6/src/syft/service/dataset/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13143 2023-06-04 12:42:01.000000 syft-0.8.1b6/src/syft/service/dataset/dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     5842 2023-06-04 12:42:01.000000 syft-0.8.1b6/src/syft/service/dataset/dataset_service.py
--rw-r--r--   0 runner    (1001) docker     (123)     1911 2023-06-04 12:42:01.000000 syft-0.8.1b6/src/syft/service/dataset/dataset_stash.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 12:44:26.997247 syft-0.8.1b6/src/syft/service/message/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-04 12:42:01.000000 syft-0.8.1b6/src/syft/service/message/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5450 2023-06-04 12:42:01.000000 syft-0.8.1b6/src/syft/service/message/message_service.py
--rw-r--r--   0 runner    (1001) docker     (123)     3951 2023-06-04 12:42:01.000000 syft-0.8.1b6/src/syft/service/message/message_stash.py
--rw-r--r--   0 runner    (1001) docker     (123)     2425 2023-06-04 12:42:01.000000 syft-0.8.1b6/src/syft/service/message/messages.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 12:44:26.997247 syft-0.8.1b6/src/syft/service/metadata/
--rw-r--r--   0 runner    (1001) docker     (123)     3525 2023-06-04 12:42:01.000000 syft-0.8.1b6/src/syft/service/metadata/node_metadata.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 12:44:26.997247 syft-0.8.1b6/src/syft/service/network/
--rw-r--r--   0 runner    (1001) docker     (123)    16364 2023-06-04 12:42:01.000000 syft-0.8.1b6/src/syft/service/network/network_service.py
--rw-r--r--   0 runner    (1001) docker     (123)     2638 2023-06-04 12:42:01.000000 syft-0.8.1b6/src/syft/service/network/node_peer.py
--rw-r--r--   0 runner    (1001) docker     (123)     4213 2023-06-04 12:42:01.000000 syft-0.8.1b6/src/syft/service/network/routes.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 12:44:26.997247 syft-0.8.1b6/src/syft/service/policy/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-04 12:42:01.000000 syft-0.8.1b6/src/syft/service/policy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    21242 2023-06-04 12:42:01.000000 syft-0.8.1b6/src/syft/service/policy/policy.py
--rw-r--r--   0 runner    (1001) docker     (123)     2081 2023-06-04 12:42:01.000000 syft-0.8.1b6/src/syft/service/policy/policy_service.py
--rw-r--r--   0 runner    (1001) docker     (123)     1077 2023-06-04 12:42:01.000000 syft-0.8.1b6/src/syft/service/policy/user_policy_stash.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 12:44:27.001247 syft-0.8.1b6/src/syft/service/project/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-04 12:42:01.000000 syft-0.8.1b6/src/syft/service/project/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    40512 2023-06-04 12:42:01.000000 syft-0.8.1b6/src/syft/service/project/project.py
--rw-r--r--   0 runner    (1001) docker     (123)    13261 2023-06-04 12:42:01.000000 syft-0.8.1b6/src/syft/service/project/project_service.py
--rw-r--r--   0 runner    (1001) docker     (123)     1703 2023-06-04 12:42:01.000000 syft-0.8.1b6/src/syft/service/project/project_stash.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 12:44:27.001247 syft-0.8.1b6/src/syft/service/queue/
--rw-r--r--   0 runner    (1001) docker     (123)     2044 2023-06-04 12:42:01.000000 syft-0.8.1b6/src/syft/service/queue/base_queue.py
--rw-r--r--   0 runner    (1001) docker     (123)     2992 2023-06-04 12:42:01.000000 syft-0.8.1b6/src/syft/service/queue/queue.py
--rw-r--r--   0 runner    (1001) docker     (123)     4765 2023-06-04 12:42:01.000000 syft-0.8.1b6/src/syft/service/queue/queue_stash.py
--rw-r--r--   0 runner    (1001) docker     (123)     7929 2023-06-04 12:42:01.000000 syft-0.8.1b6/src/syft/service/queue/zmq_queue.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 12:44:27.001247 syft-0.8.1b6/src/syft/service/request/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-04 12:42:01.000000 syft-0.8.1b6/src/syft/service/request/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16907 2023-06-04 12:42:01.000000 syft-0.8.1b6/src/syft/service/request/request.py
--rw-r--r--   0 runner    (1001) docker     (123)     4868 2023-06-04 12:42:01.000000 syft-0.8.1b6/src/syft/service/request/request_service.py
--rw-r--r--   0 runner    (1001) docker     (123)     1868 2023-06-04 12:42:01.000000 syft-0.8.1b6/src/syft/service/request/request_stash.py
--rw-r--r--   0 runner    (1001) docker     (123)     2850 2023-06-04 12:42:01.000000 syft-0.8.1b6/src/syft/service/response.py
--rw-r--r--   0 runner    (1001) docker     (123)    13188 2023-06-04 12:42:01.000000 syft-0.8.1b6/src/syft/service/service.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 12:44:27.001247 syft-0.8.1b6/src/syft/service/settings/
--rw-r--r--   0 runner    (1001) docker     (123)      773 2023-06-04 12:42:01.000000 syft-0.8.1b6/src/syft/service/settings/settings.py
--rw-r--r--   0 runner    (1001) docker     (123)     2600 2023-06-04 12:42:01.000000 syft-0.8.1b6/src/syft/service/settings/settings_service.py
--rw-r--r--   0 runner    (1001) docker     (123)     1711 2023-06-04 12:42:01.000000 syft-0.8.1b6/src/syft/service/settings/settings_stash.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 12:44:27.005246 syft-0.8.1b6/src/syft/service/user/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-04 12:42:01.000000 syft-0.8.1b6/src/syft/service/user/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      201 2023-06-04 12:42:01.000000 syft-0.8.1b6/src/syft/service/user/roles.py
--rw-r--r--   0 runner    (1001) docker     (123)     5368 2023-06-04 12:42:01.000000 syft-0.8.1b6/src/syft/service/user/user.py
--rw-r--r--   0 runner    (1001) docker     (123)     3337 2023-06-04 12:42:01.000000 syft-0.8.1b6/src/syft/service/user/user_roles.py
--rw-r--r--   0 runner    (1001) docker     (123)    13164 2023-06-04 12:42:01.000000 syft-0.8.1b6/src/syft/service/user/user_service.py
--rw-r--r--   0 runner    (1001) docker     (123)     4363 2023-06-04 12:42:01.000000 syft-0.8.1b6/src/syft/service/user/user_stash.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 12:44:27.005246 syft-0.8.1b6/src/syft/service/vpn/
--rw-r--r--   0 runner    (1001) docker     (123)     1809 2023-06-04 12:42:01.000000 syft-0.8.1b6/src/syft/service/vpn/headscale_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     6784 2023-06-04 12:42:01.000000 syft-0.8.1b6/src/syft/service/vpn/tailscale_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     5403 2023-06-04 12:42:01.000000 syft-0.8.1b6/src/syft/service/vpn/vpn.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 12:44:27.009246 syft-0.8.1b6/src/syft/store/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-04 12:42:01.000000 syft-0.8.1b6/src/syft/store/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3235 2023-06-04 12:42:01.000000 syft-0.8.1b6/src/syft/store/dict_document_store.py
--rw-r--r--   0 runner    (1001) docker     (123)    22993 2023-06-04 12:42:01.000000 syft-0.8.1b6/src/syft/store/document_store.py
--rw-r--r--   0 runner    (1001) docker     (123)    21837 2023-06-04 12:42:01.000000 syft-0.8.1b6/src/syft/store/kv_document_store.py
--rw-r--r--   0 runner    (1001) docker     (123)     4178 2023-06-04 12:42:01.000000 syft-0.8.1b6/src/syft/store/linked_obj.py
--rw-r--r--   0 runner    (1001) docker     (123)    11840 2023-06-04 12:42:01.000000 syft-0.8.1b6/src/syft/store/locks.py
--rw-r--r--   0 runner    (1001) docker     (123)     8768 2023-06-04 12:42:01.000000 syft-0.8.1b6/src/syft/store/mongo_client.py
--rw-r--r--   0 runner    (1001) docker     (123)      846 2023-06-04 12:42:01.000000 syft-0.8.1b6/src/syft/store/mongo_codecs.py
--rw-r--r--   0 runner    (1001) docker     (123)    14299 2023-06-04 12:42:01.000000 syft-0.8.1b6/src/syft/store/mongo_document_store.py
--rw-r--r--   0 runner    (1001) docker     (123)    13136 2023-06-04 12:42:01.000000 syft-0.8.1b6/src/syft/store/sqlite_document_store.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 12:44:27.009246 syft-0.8.1b6/src/syft/types/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-04 12:42:01.000000 syft-0.8.1b6/src/syft/types/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      136 2023-06-04 12:42:01.000000 syft-0.8.1b6/src/syft/types/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1091 2023-06-04 12:42:01.000000 syft-0.8.1b6/src/syft/types/datetime.py
--rw-r--r--   0 runner    (1001) docker     (123)     5100 2023-06-04 12:42:01.000000 syft-0.8.1b6/src/syft/types/grid_url.py
--rw-r--r--   0 runner    (1001) docker     (123)     4807 2023-06-04 12:42:01.000000 syft-0.8.1b6/src/syft/types/syft_metaclass.py
--rw-r--r--   0 runner    (1001) docker     (123)    19167 2023-06-04 12:42:01.000000 syft-0.8.1b6/src/syft/types/syft_object.py
--rw-r--r--   0 runner    (1001) docker     (123)     8113 2023-06-04 12:42:01.000000 syft-0.8.1b6/src/syft/types/transforms.py
--rw-r--r--   0 runner    (1001) docker     (123)     2029 2023-06-04 12:42:01.000000 syft-0.8.1b6/src/syft/types/twin_object.py
--rw-r--r--   0 runner    (1001) docker     (123)     8051 2023-06-04 12:42:01.000000 syft-0.8.1b6/src/syft/types/uid.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 12:44:27.013247 syft-0.8.1b6/src/syft/util/
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-06-04 12:42:01.000000 syft-0.8.1b6/src/syft/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      852 2023-06-04 12:42:01.000000 syft-0.8.1b6/src/syft/util/autoreload.py
--rw-r--r--   0 runner    (1001) docker     (123)     1514 2023-06-04 12:42:01.000000 syft-0.8.1b6/src/syft/util/decorators.py
--rw-r--r--   0 runner    (1001) docker     (123)     1265 2023-06-04 12:42:01.000000 syft-0.8.1b6/src/syft/util/experimental_flags.py
--rw-r--r--   0 runner    (1001) docker     (123)      654 2023-06-04 12:42:01.000000 syft-0.8.1b6/src/syft/util/filterwarnings.py
--rw-r--r--   0 runner    (1001) docker     (123)      153 2023-06-04 12:42:01.000000 syft-0.8.1b6/src/syft/util/jax_settings.py
--rw-r--r--   0 runner    (1001) docker     (123)     3779 2023-06-04 12:42:01.000000 syft-0.8.1b6/src/syft/util/logger.py
--rw-r--r--   0 runner    (1001) docker     (123)     5297 2023-06-04 12:42:01.000000 syft-0.8.1b6/src/syft/util/schema.py
--rw-r--r--   0 runner    (1001) docker     (123)     2502 2023-06-04 12:42:01.000000 syft-0.8.1b6/src/syft/util/telemetry.py
--rw-r--r--   0 runner    (1001) docker     (123)     6728 2023-06-04 12:42:01.000000 syft-0.8.1b6/src/syft/util/trace_decorator.py
--rw-r--r--   0 runner    (1001) docker     (123)    22652 2023-06-04 12:42:01.000000 syft-0.8.1b6/src/syft/util/util.py
--rw-r--r--   0 runner    (1001) docker     (123)     3123 2023-06-04 12:42:01.000000 syft-0.8.1b6/src/syft/util/version_compare.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 12:44:26.965247 syft-0.8.1b6/src/syft.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    15457 2023-06-04 12:44:26.000000 syft-0.8.1b6/src/syft.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5398 2023-06-04 12:44:26.000000 syft-0.8.1b6/src/syft.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-04 12:44:26.000000 syft-0.8.1b6/src/syft.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-06-04 12:44:26.000000 syft-0.8.1b6/src/syft.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-04 12:44:26.000000 syft-0.8.1b6/src/syft.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)     1271 2023-06-04 12:44:26.000000 syft-0.8.1b6/src/syft.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-06-04 12:44:26.000000 syft-0.8.1b6/src/syft.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 12:25:37.448962 syft-0.8.1b7/
+-rw-r--r--   0 runner    (1001) docker     (123)    11843 2023-06-11 12:23:10.000000 syft-0.8.1b7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       75 2023-06-11 12:23:10.000000 syft-0.8.1b7/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    15457 2023-06-11 12:25:37.448962 syft-0.8.1b7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    14801 2023-06-11 12:23:10.000000 syft-0.8.1b7/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      272 2023-06-11 12:23:10.000000 syft-0.8.1b7/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     3136 2023-06-11 12:25:37.448962 syft-0.8.1b7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      107 2023-06-11 12:23:10.000000 syft-0.8.1b7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 12:25:37.420961 syft-0.8.1b7/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 12:25:37.424961 syft-0.8.1b7/src/syft/
+-rw-r--r--   0 runner    (1001) docker     (123)      580 2023-06-11 12:23:22.000000 syft-0.8.1b7/src/syft/VERSION
+-rw-r--r--   0 runner    (1001) docker     (123)     4714 2023-06-11 12:23:22.000000 syft-0.8.1b7/src/syft/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      518 2023-06-11 12:23:10.000000 syft-0.8.1b7/src/syft/abstract_node.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 12:25:37.424961 syft-0.8.1b7/src/syft/capnp/
+-rw-r--r--   0 runner    (1001) docker     (123)      270 2023-06-11 12:23:10.000000 syft-0.8.1b7/src/syft/capnp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       75 2023-06-11 12:23:10.000000 syft-0.8.1b7/src/syft/capnp/iterable.capnp
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-06-11 12:23:10.000000 syft-0.8.1b7/src/syft/capnp/kv_iterable.capnp
+-rw-r--r--   0 runner    (1001) docker     (123)      186 2023-06-11 12:23:10.000000 syft-0.8.1b7/src/syft/capnp/recursive_serde.capnp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 12:25:37.424961 syft-0.8.1b7/src/syft/client/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-11 12:23:10.000000 syft-0.8.1b7/src/syft/client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24862 2023-06-11 12:23:10.000000 syft-0.8.1b7/src/syft/client/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24709 2023-06-11 12:23:10.000000 syft-0.8.1b7/src/syft/client/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)      568 2023-06-11 12:23:10.000000 syft-0.8.1b7/src/syft/client/connection.py
+-rw-r--r--   0 runner    (1001) docker     (123)      650 2023-06-11 12:23:10.000000 syft-0.8.1b7/src/syft/client/deploy.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10796 2023-06-11 12:23:10.000000 syft-0.8.1b7/src/syft/client/registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2623 2023-06-11 12:23:10.000000 syft-0.8.1b7/src/syft/client/search.py
+-rw-r--r--   0 runner    (1001) docker     (123)      549 2023-06-11 12:23:10.000000 syft-0.8.1b7/src/syft/client/user_settings.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 12:25:37.424961 syft-0.8.1b7/src/syft/external/
+-rw-r--r--   0 runner    (1001) docker     (123)     1735 2023-06-11 12:23:10.000000 syft-0.8.1b7/src/syft/external/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 12:25:37.428961 syft-0.8.1b7/src/syft/external/oblv/
+-rw-r--r--   0 runner    (1001) docker     (123)      860 2023-06-11 12:23:10.000000 syft-0.8.1b7/src/syft/external/oblv/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      284 2023-06-11 12:23:10.000000 syft-0.8.1b7/src/syft/external/oblv/auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)      212 2023-06-11 12:23:10.000000 syft-0.8.1b7/src/syft/external/oblv/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4835 2023-06-11 12:23:10.000000 syft-0.8.1b7/src/syft/external/oblv/deployment.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12347 2023-06-11 12:23:10.000000 syft-0.8.1b7/src/syft/external/oblv/deployment_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1800 2023-06-11 12:23:10.000000 syft-0.8.1b7/src/syft/external/oblv/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      489 2023-06-11 12:23:10.000000 syft-0.8.1b7/src/syft/external/oblv/oblv_keys.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2280 2023-06-11 12:23:10.000000 syft-0.8.1b7/src/syft/external/oblv/oblv_keys_stash.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7462 2023-06-11 12:23:10.000000 syft-0.8.1b7/src/syft/external/oblv/oblv_proxy.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15928 2023-06-11 12:23:10.000000 syft-0.8.1b7/src/syft/external/oblv/oblv_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1146 2023-06-11 12:23:10.000000 syft-0.8.1b7/src/syft/gevent_patch.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 12:25:37.428961 syft-0.8.1b7/src/syft/node/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-11 12:23:10.000000 syft-0.8.1b7/src/syft/node/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2631 2023-06-11 12:23:10.000000 syft-0.8.1b7/src/syft/node/credentials.py
+-rw-r--r--   0 runner    (1001) docker     (123)      152 2023-06-11 12:23:10.000000 syft-0.8.1b7/src/syft/node/domain.py
+-rw-r--r--   0 runner    (1001) docker     (123)      687 2023-06-11 12:23:10.000000 syft-0.8.1b7/src/syft/node/gateway.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28334 2023-06-11 12:23:10.000000 syft-0.8.1b7/src/syft/node/node.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6979 2023-06-11 12:23:10.000000 syft-0.8.1b7/src/syft/node/routes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2064 2023-06-11 12:23:10.000000 syft-0.8.1b7/src/syft/node/run.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6180 2023-06-11 12:23:10.000000 syft-0.8.1b7/src/syft/node/server.py
+-rw-r--r--   0 runner    (1001) docker     (123)      127 2023-06-11 12:23:10.000000 syft-0.8.1b7/src/syft/node/worker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1001 2023-06-11 12:23:10.000000 syft-0.8.1b7/src/syft/node/worker_settings.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 12:25:37.432961 syft-0.8.1b7/src/syft/serde/
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-06-11 12:23:10.000000 syft-0.8.1b7/src/syft/serde/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3597 2023-06-11 12:23:10.000000 syft-0.8.1b7/src/syft/serde/array.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4099 2023-06-11 12:23:10.000000 syft-0.8.1b7/src/syft/serde/arrow.py
+-rw-r--r--   0 runner    (1001) docker     (123)      298 2023-06-11 12:23:10.000000 syft-0.8.1b7/src/syft/serde/capnp.py
+-rw-r--r--   0 runner    (1001) docker     (123)      722 2023-06-11 12:23:10.000000 syft-0.8.1b7/src/syft/serde/deserialize.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1230 2023-06-11 12:23:10.000000 syft-0.8.1b7/src/syft/serde/lib_permissions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11663 2023-06-11 12:23:10.000000 syft-0.8.1b7/src/syft/serde/lib_service_registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)      875 2023-06-11 12:23:10.000000 syft-0.8.1b7/src/syft/serde/mock.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11639 2023-06-11 12:23:10.000000 syft-0.8.1b7/src/syft/serde/recursive.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10253 2023-06-11 12:23:10.000000 syft-0.8.1b7/src/syft/serde/recursive_primitives.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1822 2023-06-11 12:23:10.000000 syft-0.8.1b7/src/syft/serde/serializable.py
+-rw-r--r--   0 runner    (1001) docker     (123)      369 2023-06-11 12:23:10.000000 syft-0.8.1b7/src/syft/serde/serialize.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4959 2023-06-11 12:23:10.000000 syft-0.8.1b7/src/syft/serde/signature.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4885 2023-06-11 12:23:10.000000 syft-0.8.1b7/src/syft/serde/third_party.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 12:25:37.432961 syft-0.8.1b7/src/syft/service/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-11 12:23:10.000000 syft-0.8.1b7/src/syft/service/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 12:25:37.432961 syft-0.8.1b7/src/syft/service/action/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-11 12:23:10.000000 syft-0.8.1b7/src/syft/service/action/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      703 2023-06-11 12:23:10.000000 syft-0.8.1b7/src/syft/service/action/action_data_empty.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16706 2023-06-11 12:23:10.000000 syft-0.8.1b7/src/syft/service/action/action_graph.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6874 2023-06-11 12:23:10.000000 syft-0.8.1b7/src/syft/service/action/action_graph_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)    48110 2023-06-11 12:23:10.000000 syft-0.8.1b7/src/syft/service/action/action_object.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2416 2023-06-11 12:23:10.000000 syft-0.8.1b7/src/syft/service/action/action_permissions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27015 2023-06-11 12:23:10.000000 syft-0.8.1b7/src/syft/service/action/action_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10264 2023-06-11 12:23:10.000000 syft-0.8.1b7/src/syft/service/action/action_store.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1165 2023-06-11 12:23:10.000000 syft-0.8.1b7/src/syft/service/action/action_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3889 2023-06-11 12:23:10.000000 syft-0.8.1b7/src/syft/service/action/numpy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2233 2023-06-11 12:23:10.000000 syft-0.8.1b7/src/syft/service/action/pandas.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2915 2023-06-11 12:23:10.000000 syft-0.8.1b7/src/syft/service/action/plan.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4951 2023-06-11 12:23:10.000000 syft-0.8.1b7/src/syft/service/action/verification.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 12:25:37.436962 syft-0.8.1b7/src/syft/service/code/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-11 12:23:10.000000 syft-0.8.1b7/src/syft/service/code/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      236 2023-06-11 12:23:10.000000 syft-0.8.1b7/src/syft/service/code/code_parse.py
+-rw-r--r--   0 runner    (1001) docker     (123)      785 2023-06-11 12:23:10.000000 syft-0.8.1b7/src/syft/service/code/unparse.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22321 2023-06-11 12:23:10.000000 syft-0.8.1b7/src/syft/service/code/user_code.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1756 2023-06-11 12:23:10.000000 syft-0.8.1b7/src/syft/service/code/user_code_parse.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10072 2023-06-11 12:23:10.000000 syft-0.8.1b7/src/syft/service/code/user_code_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1446 2023-06-11 12:23:10.000000 syft-0.8.1b7/src/syft/service/code/user_code_stash.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1782 2023-06-11 12:23:10.000000 syft-0.8.1b7/src/syft/service/context.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 12:25:37.436962 syft-0.8.1b7/src/syft/service/data_subject/
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-06-11 12:23:10.000000 syft-0.8.1b7/src/syft/service/data_subject/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3749 2023-06-11 12:23:10.000000 syft-0.8.1b7/src/syft/service/data_subject/data_subject.py
+-rw-r--r--   0 runner    (1001) docker     (123)      870 2023-06-11 12:23:10.000000 syft-0.8.1b7/src/syft/service/data_subject/data_subject_member.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3215 2023-06-11 12:23:10.000000 syft-0.8.1b7/src/syft/service/data_subject/data_subject_member_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5006 2023-06-11 12:23:10.000000 syft-0.8.1b7/src/syft/service/data_subject/data_subject_service.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 12:25:37.436962 syft-0.8.1b7/src/syft/service/dataset/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-11 12:23:10.000000 syft-0.8.1b7/src/syft/service/dataset/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19446 2023-06-11 12:23:10.000000 syft-0.8.1b7/src/syft/service/dataset/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5842 2023-06-11 12:23:10.000000 syft-0.8.1b7/src/syft/service/dataset/dataset_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1911 2023-06-11 12:23:10.000000 syft-0.8.1b7/src/syft/service/dataset/dataset_stash.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 12:25:37.436962 syft-0.8.1b7/src/syft/service/message/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-11 12:23:10.000000 syft-0.8.1b7/src/syft/service/message/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6915 2023-06-11 12:23:10.000000 syft-0.8.1b7/src/syft/service/message/message_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3951 2023-06-11 12:23:10.000000 syft-0.8.1b7/src/syft/service/message/message_stash.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2826 2023-06-11 12:23:10.000000 syft-0.8.1b7/src/syft/service/message/messages.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 12:25:37.436962 syft-0.8.1b7/src/syft/service/metadata/
+-rw-r--r--   0 runner    (1001) docker     (123)     3527 2023-06-11 12:23:10.000000 syft-0.8.1b7/src/syft/service/metadata/node_metadata.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 12:25:37.436962 syft-0.8.1b7/src/syft/service/network/
+-rw-r--r--   0 runner    (1001) docker     (123)    16364 2023-06-11 12:23:10.000000 syft-0.8.1b7/src/syft/service/network/network_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2638 2023-06-11 12:23:10.000000 syft-0.8.1b7/src/syft/service/network/node_peer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4213 2023-06-11 12:23:10.000000 syft-0.8.1b7/src/syft/service/network/routes.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 12:25:37.440961 syft-0.8.1b7/src/syft/service/policy/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-11 12:23:10.000000 syft-0.8.1b7/src/syft/service/policy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21667 2023-06-11 12:23:10.000000 syft-0.8.1b7/src/syft/service/policy/policy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2081 2023-06-11 12:23:10.000000 syft-0.8.1b7/src/syft/service/policy/policy_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1077 2023-06-11 12:23:10.000000 syft-0.8.1b7/src/syft/service/policy/user_policy_stash.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 12:25:37.440961 syft-0.8.1b7/src/syft/service/project/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-11 12:23:10.000000 syft-0.8.1b7/src/syft/service/project/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    46382 2023-06-11 12:23:10.000000 syft-0.8.1b7/src/syft/service/project/project.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15336 2023-06-11 12:23:10.000000 syft-0.8.1b7/src/syft/service/project/project_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1908 2023-06-11 12:23:10.000000 syft-0.8.1b7/src/syft/service/project/project_stash.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 12:25:37.440961 syft-0.8.1b7/src/syft/service/queue/
+-rw-r--r--   0 runner    (1001) docker     (123)     2044 2023-06-11 12:23:10.000000 syft-0.8.1b7/src/syft/service/queue/base_queue.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2992 2023-06-11 12:23:10.000000 syft-0.8.1b7/src/syft/service/queue/queue.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4845 2023-06-11 12:23:10.000000 syft-0.8.1b7/src/syft/service/queue/queue_stash.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7929 2023-06-11 12:23:10.000000 syft-0.8.1b7/src/syft/service/queue/zmq_queue.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 12:25:37.440961 syft-0.8.1b7/src/syft/service/request/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-11 12:23:10.000000 syft-0.8.1b7/src/syft/service/request/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20654 2023-06-11 12:23:10.000000 syft-0.8.1b7/src/syft/service/request/request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7206 2023-06-11 12:23:10.000000 syft-0.8.1b7/src/syft/service/request/request_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1410 2023-06-11 12:23:10.000000 syft-0.8.1b7/src/syft/service/request/request_stash.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2850 2023-06-11 12:23:10.000000 syft-0.8.1b7/src/syft/service/response.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13653 2023-06-11 12:23:10.000000 syft-0.8.1b7/src/syft/service/service.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 12:25:37.440961 syft-0.8.1b7/src/syft/service/settings/
+-rw-r--r--   0 runner    (1001) docker     (123)      773 2023-06-11 12:23:10.000000 syft-0.8.1b7/src/syft/service/settings/settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2600 2023-06-11 12:23:10.000000 syft-0.8.1b7/src/syft/service/settings/settings_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1711 2023-06-11 12:23:10.000000 syft-0.8.1b7/src/syft/service/settings/settings_stash.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 12:25:37.440961 syft-0.8.1b7/src/syft/service/user/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-11 12:23:10.000000 syft-0.8.1b7/src/syft/service/user/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      201 2023-06-11 12:23:10.000000 syft-0.8.1b7/src/syft/service/user/roles.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5483 2023-06-11 12:23:10.000000 syft-0.8.1b7/src/syft/service/user/user.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3427 2023-06-11 12:23:10.000000 syft-0.8.1b7/src/syft/service/user/user_roles.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13662 2023-06-11 12:23:10.000000 syft-0.8.1b7/src/syft/service/user/user_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4363 2023-06-11 12:23:10.000000 syft-0.8.1b7/src/syft/service/user/user_stash.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 12:25:37.444962 syft-0.8.1b7/src/syft/service/vpn/
+-rw-r--r--   0 runner    (1001) docker     (123)     1809 2023-06-11 12:23:10.000000 syft-0.8.1b7/src/syft/service/vpn/headscale_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6784 2023-06-11 12:23:10.000000 syft-0.8.1b7/src/syft/service/vpn/tailscale_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5403 2023-06-11 12:23:10.000000 syft-0.8.1b7/src/syft/service/vpn/vpn.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 12:25:37.444962 syft-0.8.1b7/src/syft/store/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-11 12:23:10.000000 syft-0.8.1b7/src/syft/store/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3235 2023-06-11 12:23:10.000000 syft-0.8.1b7/src/syft/store/dict_document_store.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22993 2023-06-11 12:23:10.000000 syft-0.8.1b7/src/syft/store/document_store.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21837 2023-06-11 12:23:10.000000 syft-0.8.1b7/src/syft/store/kv_document_store.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4321 2023-06-11 12:23:10.000000 syft-0.8.1b7/src/syft/store/linked_obj.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11840 2023-06-11 12:23:10.000000 syft-0.8.1b7/src/syft/store/locks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8768 2023-06-11 12:23:10.000000 syft-0.8.1b7/src/syft/store/mongo_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)      846 2023-06-11 12:23:10.000000 syft-0.8.1b7/src/syft/store/mongo_codecs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14299 2023-06-11 12:23:10.000000 syft-0.8.1b7/src/syft/store/mongo_document_store.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13136 2023-06-11 12:23:10.000000 syft-0.8.1b7/src/syft/store/sqlite_document_store.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 12:25:37.444962 syft-0.8.1b7/src/syft/types/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-11 12:23:10.000000 syft-0.8.1b7/src/syft/types/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      136 2023-06-11 12:23:10.000000 syft-0.8.1b7/src/syft/types/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1091 2023-06-11 12:23:10.000000 syft-0.8.1b7/src/syft/types/datetime.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5100 2023-06-11 12:23:10.000000 syft-0.8.1b7/src/syft/types/grid_url.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4807 2023-06-11 12:23:10.000000 syft-0.8.1b7/src/syft/types/syft_metaclass.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25674 2023-06-11 12:23:10.000000 syft-0.8.1b7/src/syft/types/syft_object.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8113 2023-06-11 12:23:10.000000 syft-0.8.1b7/src/syft/types/transforms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2098 2023-06-11 12:23:10.000000 syft-0.8.1b7/src/syft/types/twin_object.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8038 2023-06-11 12:23:10.000000 syft-0.8.1b7/src/syft/types/uid.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 12:25:37.448962 syft-0.8.1b7/src/syft/util/
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-06-11 12:23:10.000000 syft-0.8.1b7/src/syft/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      852 2023-06-11 12:23:10.000000 syft-0.8.1b7/src/syft/util/autoreload.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1514 2023-06-11 12:23:10.000000 syft-0.8.1b7/src/syft/util/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1265 2023-06-11 12:23:10.000000 syft-0.8.1b7/src/syft/util/experimental_flags.py
+-rw-r--r--   0 runner    (1001) docker     (123)      654 2023-06-11 12:23:10.000000 syft-0.8.1b7/src/syft/util/filterwarnings.py
+-rw-r--r--   0 runner    (1001) docker     (123)      153 2023-06-11 12:23:10.000000 syft-0.8.1b7/src/syft/util/jax_settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3779 2023-06-11 12:23:10.000000 syft-0.8.1b7/src/syft/util/logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)      439 2023-06-11 12:23:10.000000 syft-0.8.1b7/src/syft/util/markdown.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5297 2023-06-11 12:23:10.000000 syft-0.8.1b7/src/syft/util/schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2502 2023-06-11 12:23:10.000000 syft-0.8.1b7/src/syft/util/telemetry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6728 2023-06-11 12:23:10.000000 syft-0.8.1b7/src/syft/util/trace_decorator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22652 2023-06-11 12:23:10.000000 syft-0.8.1b7/src/syft/util/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3123 2023-06-11 12:23:10.000000 syft-0.8.1b7/src/syft/util/version_compare.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 12:25:37.424961 syft-0.8.1b7/src/syft.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    15457 2023-06-11 12:25:37.000000 syft-0.8.1b7/src/syft.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5424 2023-06-11 12:25:37.000000 syft-0.8.1b7/src/syft.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-11 12:25:37.000000 syft-0.8.1b7/src/syft.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-06-11 12:25:37.000000 syft-0.8.1b7/src/syft.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-11 12:25:37.000000 syft-0.8.1b7/src/syft.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)     1296 2023-06-11 12:25:37.000000 syft-0.8.1b7/src/syft.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-06-11 12:25:37.000000 syft-0.8.1b7/src/syft.egg-info/top_level.txt
```

### Comparing `syft-0.8.1b6/LICENSE` & `syft-0.8.1b7/LICENSE`

 * *Files identical despite different names*

### Comparing `syft-0.8.1b6/PKG-INFO` & `syft-0.8.1b7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: syft
-Version: 0.8.1b6
+Version: 0.8.1b7
 Summary: Perform numpy-like analysis on data that remains in someone elses server
 Home-page: https://openmined.github.io/PySyft/
 Author: OpenMined
 Author-email: info@openmined.org
 License: Apache-2.0
 Project-URL: Source, https://github.com/OpenMined/PySyft
 Project-URL: Tracker, https://github.com/OpenMined/PySyft/issues
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: syft Version: 0.8.1b6 Summary: Perform numpy-like
+Metadata-Version: 2.1 Name: syft Version: 0.8.1b7 Summary: Perform numpy-like
 analysis on data that remains in someone elses server Home-page: https://
 openmined.github.io/PySyft/ Author: OpenMined Author-email: info@openmined.org
 License: Apache-2.0 Project-URL: Source, https://github.com/OpenMined/PySyft
 Project-URL: Tracker, https://github.com/OpenMined/PySyft/issues Platform: any
 Classifier: Development Status :: 4 - Beta Classifier: Programming Language ::
 Python Requires-Python: >=3.9 Description-Content-Type: text/markdown;
 charset=UTF-8; variant=GFM Provides-Extra: dev Provides-Extra: test_plugins
```

### Comparing `syft-0.8.1b6/README.md` & `syft-0.8.1b7/README.md`

 * *Files identical despite different names*

### Comparing `syft-0.8.1b6/setup.cfg` & `syft-0.8.1b7/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = syft
-version = attr: "0.8.1-beta.6"
+version = attr: "0.8.1-beta.7"
 description = Perform numpy-like analysis on data that remains in someone elses server
 author = OpenMined
 author_email = info@openmined.org
 license = Apache-2.0
 long_description = file: README.md
 long_description_content_type = text/markdown; charset=UTF-8; variant=GFM
 url = https://openmined.github.io/PySyft/
@@ -51,14 +51,15 @@
 	typing_extensions==4.5.0
 	sherlock[redis,filelock]==0.4.1
 	uvicorn[standard]==0.21.1
 	fastapi==0.95.1
 	hagrid>=0.3
 	matplotlib==3.7.1
 	dm-haiku==0.0.9
+	itables==1.5.2
 telemetry = 
 	opentelemetry-api==1.14.0
 	opentelemetry-sdk==1.14.0
 	opentelemetry-exporter-jaeger==1.14.0
 	opentelemetry-instrumentation==0.35b0
 	opentelemetry-instrumentation-requests==0.35b0
 install_requires = 
@@ -92,14 +93,15 @@
 	pytest_mock_resources
 	python_on_whales
 	pytest-lazy-fixture
 	pytest-rerunfailures
 	coverage
 	joblib
 	faker
+	lxml
 oblv = 
 	oblv-ctl==0.3.1
 
 [options.entry_points]
 console_scripts = 
 	syft=syft.node.run:run
```

### Comparing `syft-0.8.1b6/src/syft/VERSION` & `syft-0.8.1b7/src/syft/VERSION`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # Mono Repo Global Version
-__version__ = "0.8.1-beta.6"
+__version__ = "0.8.1-beta.7"
 # elsewhere we can call this file: `python VERSION` and simply take the stdout
 
 # stdlib
 import os
 import subprocess
 import sys
```

### Comparing `syft-0.8.1b6/src/syft/__init__.py` & `syft-0.8.1b7/src/syft/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = "0.8.1-beta.6"
+__version__ = "0.8.1-beta.7"
 
 # stdlib
 from pathlib import Path
 import sys
 from typing import Any
 from typing import Callable
 
@@ -32,14 +32,15 @@
 from .service.action.action_data_empty import ActionDataEmpty  # noqa: F401
 from .service.action.action_object import ActionObject  # noqa: F401
 from .service.action.plan import Plan  # noqa: F401
 from .service.action.plan import planify  # noqa: F401
 from .service.code.user_code import UserCodeStatus  # noqa: F401
 from .service.code.user_code import syft_function  # noqa: F401
 from .service.data_subject import DataSubjectCreate as DataSubject  # noqa: F401
+from .service.dataset.dataset import Contributor  # noqa: F401
 from .service.dataset.dataset import CreateAsset as Asset  # noqa: F401
 from .service.dataset.dataset import CreateDataset as Dataset  # noqa: F401
 from .service.message.messages import MessageStatus  # noqa: F401
 from .service.policy.policy import CustomInputPolicy  # noqa: F401
 from .service.policy.policy import CustomOutputPolicy  # noqa: F401
 from .service.policy.policy import ExactMatch  # noqa: F401
 from .service.policy.policy import SingleExecutionExactOutput  # noqa: F401
```

### Comparing `syft-0.8.1b6/src/syft/abstract_node.py` & `syft-0.8.1b7/src/syft/abstract_node.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.1b6/src/syft/client/api.py` & `syft-0.8.1b7/src/syft/client/api.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 from inspect import signature
 import types
 from typing import Any
 from typing import Callable
 from typing import Dict
 from typing import List
 from typing import Optional
+from typing import Tuple
 from typing import Union
 from typing import _GenericAlias
 
 # third party
 from nacl.exceptions import BadSignatureError
 from pydantic import BaseModel
 from pydantic import EmailStr
@@ -45,25 +46,37 @@
 from ..types.uid import UID
 from ..util.autoreload import autoreload_enabled
 from ..util.telemetry import instrument
 from .connection import NodeConnection
 
 
 class APIRegistry:
-    __api_registry__: Dict[str, SyftAPI] = {}
+    __api_registry__: Dict[Tuple, SyftAPI] = {}
 
     @classmethod
-    def set_api_for(cls, node_uid: Union[UID, str], api: SyftAPI) -> None:
+    def set_api_for(
+        cls,
+        node_uid: Union[UID, str],
+        user_verify_key: Union[SyftVerifyKey, str],
+        api: SyftAPI,
+    ) -> None:
         if isinstance(node_uid, str):
             node_uid = UID.from_string(node_uid)
-        cls.__api_registry__[node_uid] = api
+
+        if isinstance(user_verify_key, str):
+            user_verify_key = SyftVerifyKey.from_string(user_verify_key)
+
+        key = (node_uid, user_verify_key)
+
+        cls.__api_registry__[key] = api
 
     @classmethod
-    def api_for(cls, node_uid: UID) -> SyftAPI:
-        return cls.__api_registry__.get(node_uid, None)
+    def api_for(cls, node_uid: UID, user_verify_key: SyftVerifyKey) -> SyftAPI:
+        key = (node_uid, user_verify_key)
+        return cls.__api_registry__.get(key, None)
 
     @classmethod
     def get_all_api(cls) -> List[SyftAPI]:
         return list(cls.__api_registry__.values())
 
 
 @serializable()
@@ -395,15 +408,15 @@
                 doc_string=lib_config.doc_string,
                 signature=lib_config.signature,
                 has_self=False,
             )
             lib_endpoints[path] = endpoint
 
         # 🟡 TODO 35: fix root context
-        context = AuthedServiceContext(credentials=user_verify_key)
+        context = AuthedServiceContext(node=node, credentials=user_verify_key)
         method = node.get_method_with_context(UserCodeService.get_all_for_user, context)
         code_items = method()
 
         for code_item in code_items:
             path = "code.call"
             unique_path = f"code.call_{code_item.service_func_name}"
             endpoint = APIEndpoint(
@@ -520,14 +533,17 @@
 
     @property
     def lib(self) -> APIModule:
         if self.libs is None:
             self.generate_endpoints()
         return self.libs
 
+    def has_service(self, service_name: str) -> bool:
+        return hasattr(self.services, service_name)
+
     def __repr__(self) -> str:
         modules = self.services
         _repr_str = "client.api.services\n"
         for attr_name in modules._modules:
             module_or_func = getattr(modules, attr_name)
             module_path_str = f"client.api.services.{attr_name}"
             _repr_str += f"\n{module_path_str}\n\n"
```

### Comparing `syft-0.8.1b6/src/syft/client/client.py` & `syft-0.8.1b7/src/syft/client/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,24 @@
+# future
+from __future__ import annotations
+
 # stdlib
 from enum import Enum
 import hashlib
 import json
 from typing import Any
 from typing import Dict
 from typing import Optional
+from typing import TYPE_CHECKING
 from typing import Type
 from typing import Union
 from typing import cast
 
 # third party
+import pydantic
 import requests
 from requests import Response
 from requests import Session
 from requests.adapters import HTTPAdapter
 from requests.packages.urllib3.util.retry import Retry
 from tqdm import tqdm
 from typing_extensions import Self
@@ -50,59 +55,57 @@
 from .api import SyftAPICall
 from .connection import NodeConnection
 
 # use to enable mitm proxy
 # from syft.grid.connections.http_connection import HTTPConnection
 # HTTPConnection.proxies = {"http": "http://127.0.0.1:8080"}
 
+if TYPE_CHECKING:
+    # relative
+    from ..service.project.project import Project
+
 
 def upgrade_tls(url: GridURL, response: Response) -> GridURL:
     try:
         if response.url.startswith("https://") and url.protocol == "http":
             # we got redirected to https
             https_url = GridURL.from_url(response.url).with_path("")
             debug(f"GridURL Upgraded to HTTPS. {https_url}")
             return https_url
     except Exception as e:
         print(f"Failed to upgrade to HTTPS. {e}")
     return url
 
 
 API_PATH = "/api/v2"
+DEFAULT_PYGRID_PORT = 80
+DEFAULT_PYGRID_ADDRESS = f"http://localhost:{DEFAULT_PYGRID_PORT}"
 
 
 class Routes(Enum):
     ROUTE_METADATA = f"{API_PATH}/metadata"
     ROUTE_API = f"{API_PATH}/api"
     ROUTE_LOGIN = f"{API_PATH}/login"
     ROUTE_REGISTER = f"{API_PATH}/register"
     ROUTE_API_CALL = f"{API_PATH}/api_call"
 
 
-DEFAULT_PYGRID_PORT = 80
-DEFAULT_PYGRID_ADDRESS = f"http://localhost:{DEFAULT_PYGRID_PORT}"
-
-
 @serializable(attrs=["proxy_target_uid", "url"])
 class HTTPConnection(NodeConnection):
     __canonical_name__ = "HTTPConnection"
     __version__ = SYFT_OBJECT_VERSION_1
 
     proxy_target_uid: Optional[UID]
     url: GridURL
     routes: Type[Routes] = Routes
     session_cache: Optional[Session]
 
-    def __init__(
-        self, url: Union[GridURL, str], proxy_target_uid: Optional[UID] = None
-    ) -> None:
-        url = GridURL.from_url(url).as_container_host()
-
-        proxy_target_uid = proxy_target_uid
-        super().__init__(url=url, proxy_target_uid=proxy_target_uid)
+    @pydantic.validator("url", pre=True, always=True)
+    def make_url(cls, v: Union[GridURL, str]) -> GridURL:
+        return GridURL.from_url(v).as_container_host()
 
     def with_proxy(self, proxy_target_uid: UID) -> Self:
         return HTTPConnection(url=self.url, proxy_target_uid=proxy_target_uid)
 
     def get_cache_key(self) -> str:
         return str(self.url)
 
@@ -181,15 +184,15 @@
         obj = _deserialize(content, from_bytes=True)
         obj.connection = self
         obj.signing_key = credentials
         if self.proxy_target_uid:
             obj.node_uid = self.proxy_target_uid
         return cast(SyftAPI, obj)
 
-    def login(self, email: str, password: str) -> SyftSigningKey:
+    def login(self, email: str, password: str) -> Optional[SyftSigningKey]:
         credentials = {"email": email, "password": password}
         response = self._make_post(self.routes.ROUTE_LOGIN.value, credentials)
         obj = _deserialize(response, from_bytes=True)
         if isinstance(obj, UserPrivateKey):
             return obj.signing_key
         return None
 
@@ -300,14 +303,15 @@
 
 @instrument
 @serializable()
 class SyftClient:
     connection: NodeConnection
     metadata: Optional[NodeMetadataJSON]
     credentials: Optional[SyftSigningKey]
+    __logged_in_user: str = ""
 
     def __init__(
         self,
         connection: NodeConnection,
         metadata: Optional[NodeMetadataJSON] = None,
         credentials: Optional[SyftSigningKey] = None,
         api: Optional[SyftAPI] = None,
@@ -324,14 +328,18 @@
             self._fetch_node_metadata(self.credentials)
 
     @property
     def authed(self) -> bool:
         return bool(self.credentials)
 
     @property
+    def logged_in_user(self) -> Optional[str]:
+        return self.__logged_in_user
+
+    @property
     def verify_key(self) -> SyftVerifyKey:
         if self.credentials is None:
             raise ValueError("SigningKey not set on client")
         return self.credentials.verify_key
 
     @staticmethod
     def from_url(url: Union[str, GridURL]) -> Self:
@@ -351,27 +359,31 @@
 
     @property
     def icon(self) -> str:
         return "📡"
 
     @property
     def api(self) -> SyftAPI:
-        if self._api is None:
+        # invalidate API
+        if self._api is None or (self._api.signing_key != self.credentials):
             self._fetch_api(self.credentials)
 
         return self._api
 
     def guest(self) -> Self:
         self.credentials = SyftSigningKey.generate()
+        self.__logged_in_user = ""
         return self
 
     def upload_dataset(self, dataset: CreateDataset) -> Union[SyftSuccess, SyftError]:
         # relative
         from ..types.twin_object import TwinObject
 
+        dataset._check_asset_must_contain_mock()
+
         for asset in tqdm(dataset.asset_list):
             print(f"Uploading: {asset.name}")
             try:
                 twin = TwinObject(private_obj=asset.data, mock_obj=asset.mock)
             except Exception as e:
                 return SyftError(message=f"Failed to create twin. {e}")
             response = self.api.services.action.set(twin)
@@ -384,15 +396,15 @@
         if valid.ok():
             return self.api.services.dataset.add(dataset=dataset)
         else:
             if len(valid.err()) > 0:
                 return tuple(valid.err())
             return valid.err()
 
-    def exchange_route(self, client: Self) -> None:
+    def exchange_route(self, client: Self) -> Union[SyftSuccess, SyftError]:
         # relative
         from ..service.network.routes import connection_to_route
 
         self_node_route = connection_to_route(self.connection)
         remote_node_route = connection_to_route(client.connection)
 
         result = self.api.services.network.exchange_credentials_with(
@@ -404,57 +416,82 @@
         return result
 
     def apply_to_gateway(self, client: Self) -> None:
         return self.exchange_route(client)
 
     @property
     def data_subject_registry(self) -> Optional[APIModule]:
-        if self.api is not None and hasattr(self.api.services, "data_subject"):
+        if self.api is not None and self.api.has_service("data_subject"):
             return self.api.services.data_subject
         return None
 
     @property
     def users(self) -> Optional[APIModule]:
-        if self.api is not None and hasattr(self.api.services, "user"):
+        if self.api is not None and self.api.has_service("user"):
             return self.api.services.user
         return None
 
     @property
     def code(self) -> Optional[APIModule]:
-        if self.api is not None and hasattr(self.api.services, "code"):
+        if self.api is not None and self.api.has_service("code"):
             return self.api.services.code
 
     @property
     def requests(self) -> Optional[APIModule]:
-        if self.api is not None and hasattr(self.api.services, "request"):
+        if self.api is not None and self.api.has_service("request"):
             return self.api.services.request
         return None
 
     @property
     def datasets(self) -> Optional[APIModule]:
-        if self.api is not None and hasattr(self.api.services, "dataset"):
+        if self.api is not None and self.api.has_service("dataset"):
             return self.api.services.dataset
         return None
 
     @property
     def notifications(self) -> Optional[APIModule]:
-        if self.api is not None and hasattr(self.api.services, "messages"):
+        if self.api is not None and self.api.has_service("messages"):
             return self.api.services.messages
         return None
 
     @property
     def domains(self) -> Optional[APIModule]:
-        if self.api is not None and hasattr(self.api.services, "network"):
+        if self.api is not None and self.api.has_service("network"):
             return self.api.services.network.get_all_peers()
         return None
 
+    @property
+    def projects(self) -> Optional[APIModule]:
+        if self.api.has_service("project"):
+            return self.api.services.project
+        return None
+
+    def get_project(
+        self,
+        name: str = None,
+        uid: UID = None,
+    ) -> Optional[Project]:
+        """Get project by name or UID"""
+
+        if not self.api.has_service("project"):
+            return None
+
+        if name:
+            return self.api.services.project.get_by_name(name)
+
+        elif uid:
+            return self.api.services.project.get_by_uid(uid)
+
+        return self.api.services.project.get_all()
+
     def login(self, email: str, password: str, cache: bool = True) -> Self:
         signing_key = self.connection.login(email=email, password=password)
         if signing_key is not None:
             self.credentials = signing_key
+            self.__logged_in_user = email
             self._fetch_api(self.credentials)
             if cache:
                 SyftClientSessionCache.add_client(
                     email=email,
                     password=password,
                     connection=self.connection,
                     syft_client=self,
@@ -534,15 +571,15 @@
             hasattr(self, "api")
             and hasattr(self.api, "lib")
             and hasattr(self.api.lib, name)
         ):
             return getattr(self.api.lib, name)
         else:
             raise AttributeError(
-                f"{self.__class__.__name__} object has no attribute {name}"
+                f"{self.__class__.__name__} object has no attribute {name}."
             )
 
     def __hash__(self) -> int:
         return hash(self.id) + hash(self.connection)
 
     def __eq__(self, other: Any) -> bool:
         if not isinstance(other, SyftClient):
@@ -574,15 +611,19 @@
     def _fetch_api(self, credentials: SyftSigningKey):
         _api: SyftAPI = self.connection.get_api(credentials=credentials)
 
         def refresh_callback():
             return self._fetch_api(self.credentials)
 
         _api.refresh_api_callback = refresh_callback
-        APIRegistry.set_api_for(node_uid=self.id, api=_api)
+        APIRegistry.set_api_for(
+            node_uid=self.id,
+            user_verify_key=self.credentials.verify_key,
+            api=_api,
+        )
         self._api = _api
 
 
 @instrument
 def connect(
     url: Union[str, GridURL] = DEFAULT_PYGRID_ADDRESS,
     node: Optional[AbstractNode] = None,
@@ -682,15 +723,15 @@
         hash_key = str(node_uid) + str(verify_key)
         return cls.__client_cache__.get(hash_key, None)
 
     @classmethod
     def get_client(
         cls, email: str, password: str, connection: NodeConnection
     ) -> Optional[SyftClient]:
-        # we have some bugs here so lets disable until they are fixed
+        # we have some bugs here so lets disable until they are fixed.
         return None
         hash_key = cls._get_key(email, password, connection.get_cache_key())
         return cls.__credentials_store__.get(hash_key, None)
 
     @classmethod
     def get_client_for_node_uid(cls, node_uid: UID) -> Optional[SyftClient]:
         return cls.__client_cache__.get(node_uid, None)
```

### Comparing `syft-0.8.1b6/src/syft/client/connection.py` & `syft-0.8.1b7/src/syft/client/connection.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.1b6/src/syft/client/deploy.py` & `syft-0.8.1b7/src/syft/client/deploy.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.1b6/src/syft/client/registry.py` & `syft-0.8.1b7/src/syft/client/registry.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.1b6/src/syft/client/search.py` & `syft-0.8.1b7/src/syft/client/search.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.1b6/src/syft/client/user_settings.py` & `syft-0.8.1b7/src/syft/client/user_settings.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.1b6/src/syft/external/__init__.py` & `syft-0.8.1b7/src/syft/external/__init__.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.1b6/src/syft/external/oblv/__init__.py` & `syft-0.8.1b7/src/syft/external/oblv/__init__.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.1b6/src/syft/external/oblv/deployment.py` & `syft-0.8.1b7/src/syft/external/oblv/deployment.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.1b6/src/syft/external/oblv/deployment_client.py` & `syft-0.8.1b7/src/syft/external/oblv/deployment_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -304,15 +304,15 @@
         )
 
         code_id = UID()
         code.id = code_id
         code.enclave_metadata = enclave_metadata
 
         for domain_client in self.domain_clients:
-            domain_client.api.services.code.request_code_execution(code=code)
+            domain_client.code.request_code_execution(code=code)
 
         res = self.api.services.code.request_code_execution(code=code)
 
         return res
 
     @property
     def api(self) -> SyftAPI:
```

### Comparing `syft-0.8.1b6/src/syft/external/oblv/exceptions.py` & `syft-0.8.1b7/src/syft/external/oblv/exceptions.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.1b6/src/syft/external/oblv/oblv_keys_stash.py` & `syft-0.8.1b7/src/syft/external/oblv/oblv_keys_stash.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.1b6/src/syft/external/oblv/oblv_proxy.py` & `syft-0.8.1b7/src/syft/external/oblv/oblv_proxy.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.1b6/src/syft/external/oblv/oblv_service.py` & `syft-0.8.1b7/src/syft/external/oblv/oblv_service.py`

 * *Files 1% similar despite different names*

```diff
@@ -365,15 +365,15 @@
             oblv_key_name=worker_name,
             params=params,
         )
 
         obj = deserialize(req.content, from_bytes=True)
         # TODO 🟣 Retrieve of signing key of user after permission  is fully integrated
         obj.signing_key = signing_key
-        obj.connection = HTTPConnection(connection_string)
+        obj.connection = HTTPConnection(url=connection_string)
         return cast(SyftAPI, obj)
 
     @service_method(
         path="oblv.send_user_code_inputs_to_enclave",
         name="send_user_code_inputs_to_enclave",
         roles=GUEST_ROLE_LEVEL,
     )
@@ -409,29 +409,29 @@
         user_code_service.update_code_state(context=context, code_item=user_code)
 
         if not action_service.exists(context=context, obj_id=user_code_id):
             dict_object = DictObject(id=user_code_id)
             dict_object.base_dict[str(context.credentials)] = inputs
             action_service.store.set(
                 uid=user_code_id,
-                credentials=user_code.user_verify_key,
+                credentials=context.node.verify_key,
                 syft_object=dict_object,
                 has_result_read_permission=True,
             )
 
         else:
             res = action_service.store.get(
-                uid=user_code_id, credentials=user_code.user_verify_key
+                uid=user_code_id, credentials=context.node.verify_key
             )
             if res.is_ok():
                 dict_object = res.ok()
                 dict_object.base_dict[str(context.credentials)] = inputs
                 action_service.store.set(
                     uid=user_code_id,
-                    credentials=user_code.user_verify_key,
+                    credentials=context.node.verify_key,
                     syft_object=dict_object,
                 )
             else:
                 return res
 
         return Ok(Ok(True))
```

### Comparing `syft-0.8.1b6/src/syft/gevent_patch.py` & `syft-0.8.1b7/src/syft/gevent_patch.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.1b6/src/syft/node/credentials.py` & `syft-0.8.1b7/src/syft/node/credentials.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,27 +5,28 @@
 from typing import Any
 from typing import Union
 
 # third party
 from nacl.encoding import HexEncoder
 from nacl.signing import SigningKey
 from nacl.signing import VerifyKey
+import pydantic
 
 # relative
 from ..serde.serializable import serializable
 from ..types.base import SyftBaseModel
 
 SIGNING_KEY_FOR = "SigningKey for"
 
 
 @serializable()
 class SyftVerifyKey(SyftBaseModel):
     verify_key: VerifyKey
 
-    def __init__(self, verify_key: Union[str, VerifyKey]) -> None:
+    def __init__(self, verify_key: Union[str, VerifyKey]):
         if isinstance(verify_key, str):
             verify_key = VerifyKey(bytes.fromhex(verify_key))
         super().__init__(verify_key=verify_key)
 
     def __str__(self) -> str:
         return self.verify_key.encode(encoder=HexEncoder).decode("utf-8")
 
@@ -49,18 +50,17 @@
         return hash(self.verify_key)
 
 
 @serializable()
 class SyftSigningKey(SyftBaseModel):
     signing_key: SigningKey
 
-    def __init__(self, signing_key: Union[str, SigningKey]) -> None:
-        if isinstance(signing_key, str):
-            signing_key = SigningKey(bytes.fromhex(signing_key))
-        super().__init__(signing_key=signing_key)
+    @pydantic.validator("signing_key", pre=True, always=True)
+    def make_signing_key(cls, v: Union[str, SigningKey]) -> SigningKey:
+        return SigningKey(bytes.fromhex(v)) if isinstance(v, str) else v
 
     @property
     def verify_key(self) -> SyftVerifyKey:
         return SyftVerifyKey(verify_key=self.signing_key.verify_key)
 
     def __str__(self) -> str:
         return self.signing_key.encode(encoder=HexEncoder).decode("utf-8")
```

### Comparing `syft-0.8.1b6/src/syft/node/gateway.py` & `syft-0.8.1b7/src/syft/node/gateway.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.1b6/src/syft/node/node.py` & `syft-0.8.1b7/src/syft/node/node.py`

 * *Files 0% similar despite different names*

```diff
@@ -33,15 +33,14 @@
 from ..abstract_node import AbstractNode
 from ..abstract_node import NodeType
 from ..client.api import SignedSyftAPICall
 from ..client.api import SyftAPI
 from ..client.api import SyftAPICall
 from ..client.api import SyftAPIData
 from ..external import OBLV
-from ..serde import serialize
 from ..serde.deserialize import _deserialize
 from ..serde.serialize import _serialize
 from ..service.action.action_service import ActionService
 from ..service.action.action_store import DictActionStore
 from ..service.action.action_store import SQLiteActionStore
 from ..service.code.user_code_service import UserCodeService
 from ..service.context import AuthedServiceContext
@@ -273,15 +272,15 @@
             name_hash_uuid[6] & 0x0F
         ) | 0x40  # Set version to 4 (uuid4)
         name_hash_uuid[8] = (name_hash_uuid[8] & 0x3F) | 0x80  # Set variant to RFC 4122
         name_hash_string = binascii.hexlify(bytearray(name_hash_uuid)).decode("utf-8")
         if uuid.UUID(name_hash_string).version != 4:
             raise Exception(f"Invalid UID: {name_hash_string} for name: {name}")
         uid = UID(name_hash_string)
-        key = SyftSigningKey(SigningKey(name_hash))
+        key = SyftSigningKey(signing_key=SigningKey(name_hash))
         if reset:
             store_config = SQLiteStoreClientConfig()
             store_config.filename = f"{uid}.sqlite"
 
             # stdlib
             import sqlite3
 
@@ -617,15 +616,15 @@
             item = QueueItem(id=task_uid, node_uid=self.id)
             # 🟡 TODO 36: Needs distributed lock
             self.queue_stash.set_placeholder(self.verify_key, item)
 
             # Publisher system which pushes to a Queue
             worker_settings = WorkerSettings.from_node(node=self)
 
-            message_bytes = serialize._serialize(
+            message_bytes = _serialize(
                 [task_uid, api_call, worker_settings], to_bytes=True
             )
             self.queue_manager.send(message=message_bytes, queue_name="api_call")
 
             return item
         return result
```

### Comparing `syft-0.8.1b6/src/syft/node/routes.py` & `syft-0.8.1b7/src/syft/node/routes.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.1b6/src/syft/node/run.py` & `syft-0.8.1b7/src/syft/node/run.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.1b6/src/syft/node/server.py` & `syft-0.8.1b7/src/syft/node/server.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.1b6/src/syft/node/worker_settings.py` & `syft-0.8.1b7/src/syft/node/worker_settings.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.1b6/src/syft/serde/array.py` & `syft-0.8.1b7/src/syft/serde/array.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.1b6/src/syft/serde/arrow.py` & `syft-0.8.1b7/src/syft/serde/arrow.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.1b6/src/syft/serde/deserialize.py` & `syft-0.8.1b7/src/syft/serde/deserialize.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.1b6/src/syft/serde/lib_permissions.py` & `syft-0.8.1b7/src/syft/serde/lib_permissions.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.1b6/src/syft/serde/lib_service_registry.py` & `syft-0.8.1b7/src/syft/serde/lib_service_registry.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.1b6/src/syft/serde/mock.py` & `syft-0.8.1b7/src/syft/serde/mock.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.1b6/src/syft/serde/recursive.py` & `syft-0.8.1b7/src/syft/serde/recursive.py`

 * *Files 2% similar despite different names*

```diff
@@ -175,14 +175,17 @@
     bytes_value = b""
     for value in capnp_list:
         bytes_value += value
     return bytes_value
 
 
 def rs_object2proto(self: Any, for_hashing: bool = False) -> _DynamicStructBuilder:
+    # relative
+    from ..types.syft_object import DYNAMIC_SYFT_ATTRIBUTES
+
     is_type = False
     if isinstance(self, type):
         is_type = True
 
     msg = recursive_scheme.new_message()
     fqn = get_fully_qualified_name(self)
     if fqn not in TYPE_BANK:
@@ -209,17 +212,21 @@
             )
         chunk_bytes(serialize(self), "nonrecursiveBlob", msg)
         return msg
 
     if attribute_list is None:
         attribute_list = self.__dict__.keys()
 
-    hash_exclude_attrs = hash_exclude_attrs if for_hashing else []
+    hash_exclude_attrs_set = (
+        set(hash_exclude_attrs).union(set(DYNAMIC_SYFT_ATTRIBUTES))
+        if for_hashing
+        else set()
+    )
     attribute_list = (
-        set(attribute_list) - set(exclude_attrs_list) - set(hash_exclude_attrs)
+        set(attribute_list) - set(exclude_attrs_list) - hash_exclude_attrs_set
     )
 
     msg.init("fieldsName", len(attribute_list))
     msg.init("fieldsData", len(attribute_list))
 
     for idx, attr_name in enumerate(sorted(attribute_list)):
         if not hasattr(self, attr_name):
```

### Comparing `syft-0.8.1b6/src/syft/serde/recursive_primitives.py` & `syft-0.8.1b7/src/syft/serde/recursive_primitives.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.1b6/src/syft/serde/serializable.py` & `syft-0.8.1b7/src/syft/serde/serializable.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.1b6/src/syft/serde/signature.py` & `syft-0.8.1b7/src/syft/serde/signature.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.1b6/src/syft/serde/third_party.py` & `syft-0.8.1b7/src/syft/serde/third_party.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.1b6/src/syft/service/action/action_data_empty.py` & `syft-0.8.1b7/src/syft/service/action/action_data_empty.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.1b6/src/syft/service/action/action_graph.py` & `syft-0.8.1b7/src/syft/service/action/action_graph.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.1b6/src/syft/service/action/action_graph_service.py` & `syft-0.8.1b7/src/syft/service/action/action_graph_service.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.1b6/src/syft/service/action/action_object.py` & `syft-0.8.1b7/src/syft/service/action/action_object.py`

 * *Files 2% similar despite different names*

```diff
@@ -172,14 +172,15 @@
     "__version__",  # syft
     "__args__",  # pydantic
     "to_pointer",  # syft
     "to",  # syft
     "send",  # syft
     "_copy_and_set_values",  # pydantic
     "get_from",  # syft
+    "delete_data",  # syft
 ]
 dont_wrap_output_attrs = [
     "__repr__",
     "__str__",
     "_repr_html_",
     "_repr_markdown_",
     "_repr_latex_",
@@ -227,15 +228,15 @@
     result_id: Optional[Union[UID, LineageID]]
     result_twin_type: Optional[TwinMode]
     action: Optional[Action]
     action_type: Optional[ActionType]
 
 
 def make_action_side_effect(
-    context: PreHookContext, *args: List[Any, ...], **kwargs: Dict[str, Any]
+    context: PreHookContext, *args: Any, **kwargs: Any
 ) -> Result[Ok[Tuple[PreHookContext, Tuple[Any, ...], Dict[str, Any]]], Err[str]]:
     """Create a new action from context_op_name, and add it to the PreHookContext
 
     Parameters:
         context: PreHookContext
             PreHookContext object
         *args:
@@ -401,14 +402,15 @@
     "is_twin",
     "is_pointer",
     "request",
     "__repr__",
     "_repr_markdown_",
     "syft_twin_type",
     "_repr_debug_",
+    "as_empty",
 ]
 
 
 class ActionObject(SyftObject):
     """Action object for remote execution."""
 
     __canonical_name__ = "ActionObject"
@@ -505,15 +507,18 @@
         if self.syft_node_uid is None:
             raise SyftException("Pointers can't execute without a node_uid.")
 
         # relative
         from ...client.api import APIRegistry
         from ...client.api import SyftAPICall
 
-        api = APIRegistry.api_for(node_uid=self.syft_node_uid)
+        api = APIRegistry.api_for(
+            node_uid=self.syft_node_uid,
+            user_verify_key=self.syft_client_verify_key,
+        )
 
         kwargs = {"action": action}
         api_call = SyftAPICall(
             node_uid=self.syft_node_uid, path="action.execute", args=[], kwargs=kwargs
         )
         return api.make_call(api_call)
 
@@ -530,15 +535,15 @@
         submit_request = SubmitRequest(
             changes=[permission_change],
             requesting_user_verify_key=client.credentials.verify_key,
         )
         return client.api.services.request.submit(submit_request)
 
     def _syft_try_to_save_to_store(self, obj) -> None:
-        if self.syft_node_uid is None:
+        if self.syft_node_uid is None or self.syft_client_verify_key is None:
             return
         elif obj.syft_node_uid is not None:
             return
         # TODO fix: the APIRegistry often gets the wrong client
         # if you have 2 clients in memory
         # therefore the following happens if you call a method
         # with a pointer to a twin (mock version)
@@ -560,16 +565,18 @@
             create_object=obj,
         )
 
         if TraceResult._client is not None:
             api = TraceResult._client.api
             TraceResult.result += [action]
         else:
-            api = APIRegistry.api_for(node_uid=self.syft_node_uid)
-
+            api = APIRegistry.api_for(
+                node_uid=self.syft_node_uid,
+                user_verify_key=self.syft_client_verify_key,
+            )
         api.services.action.execute(action)
 
     def _syft_prepare_obj_uid(self, obj) -> LineageID:
         # We got the UID
         if isinstance(obj, (UID, LineageID)):
             return LineageID(obj.id)
 
@@ -718,14 +725,21 @@
         """Get the object from a Syft Client"""
         res = client.api.services.action.get(self.id)
         if not isinstance(res, ActionObject):
             return Err(res)
         else:
             return res.syft_action_data
 
+    def as_empty(self):
+        id = self.id
+        # TODO: fix
+        if isinstance(id, LineageID):
+            id = id.id
+        return ActionObject.empty(self.syft_internal_type, id, self.syft_lineage_id)
+
     @staticmethod
     def from_obj(
         syft_action_data: Any,
         id: Optional[UID] = None,
         syft_lineage_id: Optional[LineageID] = None,
     ) -> ActionObject:
         """Create an ActionObject from an existing object.
@@ -786,14 +800,18 @@
         empty = ActionDataEmpty(syft_internal_type=syft_internal_type)
         res = ActionObject.from_obj(
             syft_action_data=empty, id=id, syft_lineage_id=syft_lineage_id
         )
         res.__dict__["syft_internal_type"] = syft_internal_type
         return res
 
+    def delete_data(self):
+        empty = ActionDataEmpty(syft_internal_type=self.syft_internal_type)
+        self.syft_action_data = empty
+
     def __post_init__(self) -> None:
         """Add pre/post hooks."""
         if HOOK_ALWAYS not in self._syft_pre_hooks__:
             self._syft_pre_hooks__[HOOK_ALWAYS] = []
 
         if HOOK_ON_POINTERS not in self._syft_post_hooks__:
             self._syft_pre_hooks__[HOOK_ON_POINTERS] = []
@@ -941,14 +959,18 @@
         # Propagate History
         if context.action is not None:
             result.syft_history_hash = context.action.syft_history_hash
 
         # Propagate Syft Node UID
         result.syft_node_uid = context.node_uid
 
+        # Propogate Syft Node Location and Client Verify Key
+        result.syft_node_location = context.syft_node_location
+        result.syft_client_verify_key = context.syft_client_verify_key
+
         # Propagate Result ID
         if context.result_id is not None:
             result.id = context.result_id
 
         return result
 
     def _syft_wrap_attribute_for_bool_on_nonbools(self, name: str) -> Any:
@@ -960,15 +982,20 @@
 
         if hasattr(self.syft_action_data, "__bool__"):
             raise RuntimeError(
                 "[_wrap_attribute_for_bool_on_nonbools] self.syft_action_data already implements the bool operator"
             )
 
         debug("[__getattribute__] Handling bool on nonbools")
-        context = PreHookContext(obj=self, op_name=name)
+        context = PreHookContext(
+            obj=self,
+            op_name=name,
+            syft_node_location=self.syft_node_location,
+            syft_client_verify_key=self.syft_client_verify_key,
+        )
         context, _, _ = self._syft_run_pre_hooks__(context, name, (), {})
 
         # no input needs to propagate
         result = self._syft_run_post_hooks__(context, name, bool(self.syft_action_data))
         result = self._syft_attr_propagate_ids(context, name, result)
 
         def __wrapper__bool__() -> bool:
@@ -983,15 +1010,19 @@
         if not self.syft_is_property(context_self, name):
             raise RuntimeError(
                 "[_wrap_attribute_for_properties] Use this only on properties"
             )
         debug(f"[__getattribute__] Handling property {name} ")
 
         context = PreHookContext(
-            obj=self, op_name=name, action_type=ActionType.GETATTRIBUTE
+            obj=self,
+            op_name=name,
+            action_type=ActionType.GETATTRIBUTE,
+            syft_node_location=self.syft_node_location,
+            syft_client_verify_key=self.syft_client_verify_key,
         )
         context, _, _ = self._syft_run_pre_hooks__(context, name, (), {})
         # no input needs to propagate
         result = self._syft_run_post_hooks__(
             context, name, self.syft_get_property(context_self, name)
         )
 
@@ -1013,15 +1044,19 @@
         else:
             original_func = getattr(self.syft_action_data, name)
 
         debug_original_func(name, original_func)
 
         def _base_wrapper(*args: Any, **kwargs: Any) -> Any:
             context = PreHookContext(
-                obj=self, op_name=name, action_type=ActionType.METHOD
+                obj=self,
+                op_name=name,
+                action_type=ActionType.METHOD,
+                syft_node_location=self.syft_node_location,
+                syft_client_verify_key=self.syft_client_verify_key,
             )
             context, pre_hook_args, pre_hook_kwargs = self._syft_run_pre_hooks__(
                 context, name, args, kwargs
             )
 
             if has_action_data_empty(args=args, kwargs=kwargs):
                 result = fake_func(*args, **kwargs)
@@ -1075,15 +1110,19 @@
             args=args, kwargs=kwargs
         ):
             local_func = fake_func
         else:
             local_func = getattr(self.syft_action_data, op_name)
 
         context = PreHookContext(
-            obj=self, op_name=op_name, action_type=ActionType.SETATTRIBUTE
+            obj=self,
+            op_name=op_name,
+            action_type=ActionType.SETATTRIBUTE,
+            syft_node_location=self.syft_node_location,
+            syft_client_verify_key=self.syft_client_verify_key,
         )
         context, pre_hook_args, pre_hook_kwargs = self._syft_run_pre_hooks__(
             context, "__setattr__", args, kwargs
         )
 
         original_args, _ = debox_args_and_kwargs(pre_hook_args, pre_hook_kwargs)
         val = original_args[1]
@@ -1351,19 +1390,17 @@
     debug("inspect.isfunction", inspect.isfunction(func))
     debug("inspect.isbuiltin", inspect.isbuiltin(func))
     debug("inspect.ismethod", inspect.ismethod(func))
     debug("inspect.ismethoddescriptor", inspect.ismethoddescriptor(func))
 
 
 def is_action_data_empty(obj: Any) -> bool:
-    if hasattr(obj, "syft_action_data"):
-        obj = obj.syft_action_data
-    if isinstance(obj, ActionDataEmpty):
-        return True
-    return False
+    return isinstance(obj, AnyActionObject) and isinstance(
+        obj.syft_action_data, ActionDataEmpty
+    )
 
 
 def has_action_data_empty(args: Any, kwargs: Any) -> bool:
     for a in args:
         if is_action_data_empty(a):
             return True
```

### Comparing `syft-0.8.1b6/src/syft/service/action/action_permissions.py` & `syft-0.8.1b7/src/syft/service/action/action_permissions.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.1b6/src/syft/service/action/action_service.py` & `syft-0.8.1b7/src/syft/service/action/action_service.py`

 * *Files 0% similar despite different names*

```diff
@@ -199,14 +199,15 @@
         except Exception as e:
             return Err(f"_user_code_execute failed. {e}")
 
         set_result = self.store.set(
             uid=result_id,
             credentials=context.credentials,
             syft_object=result_action_object,
+            has_result_read_permission=True,
         )
         if set_result.is_err():
             return set_result.err()
         return Ok(result_action_object)
 
     def execute_plan(
         self, plan, context: AuthedServiceContext, plan_kwargs: Dict[str, ActionObject]
```

### Comparing `syft-0.8.1b6/src/syft/service/action/action_store.py` & `syft-0.8.1b7/src/syft/service/action/action_store.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,14 +19,15 @@
 from ...store.document_store import StoreConfig
 from ...types.syft_object import SyftObject
 from ...types.twin_object import TwinObject
 from ...types.uid import LineageID
 from ...types.uid import UID
 from ..response import SyftSuccess
 from .action_object import TwinMode
+from .action_object import is_action_data_empty
 from .action_permissions import ActionObjectEXECUTE
 from .action_permissions import ActionObjectOWNER
 from .action_permissions import ActionObjectPermission
 from .action_permissions import ActionObjectREAD
 from .action_permissions import ActionObjectWRITE
 from .action_permissions import ActionPermission
 
@@ -87,16 +88,17 @@
         uid = uid.id  # We only need the UID from LineageID or UID
 
         try:
             # 🟡 TODO 34: do we want pointer read permissions?
             if uid in self.data:
                 obj = self.data[uid]
                 if isinstance(obj, TwinObject):
-                    obj = obj.mock
-                    obj.syft_twin_type = TwinMode.MOCK
+                    obj = (
+                        obj.mock if not is_action_data_empty(obj.mock) else obj.private
+                    )
                     # we patch the real id on it so we can keep using the twin
                     obj.id = uid
                 else:
                     obj.syft_twin_type = TwinMode.NONE
                 obj.syft_point_to(node_uid)
                 return Ok(obj)
             # third party
```

### Comparing `syft-0.8.1b6/src/syft/service/action/action_types.py` & `syft-0.8.1b7/src/syft/service/action/action_types.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.1b6/src/syft/service/action/numpy.py` & `syft-0.8.1b7/src/syft/service/action/numpy.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.1b6/src/syft/service/action/pandas.py` & `syft-0.8.1b7/src/syft/service/action/pandas.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.1b6/src/syft/service/action/plan.py` & `syft-0.8.1b7/src/syft/service/action/plan.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.1b6/src/syft/service/action/verification.py` & `syft-0.8.1b7/src/syft/service/action/verification.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.1b6/src/syft/service/code/unparse.py` & `syft-0.8.1b7/src/syft/service/code/unparse.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.1b6/src/syft/service/code/user_code.py` & `syft-0.8.1b7/src/syft/service/code/user_code.py`

 * *Files 0% similar despite different names*

```diff
@@ -41,14 +41,15 @@
 from ..dataset.dataset import Asset
 from ..metadata.node_metadata import EnclaveMetadata
 from ..policy.policy import CustomInputPolicy
 from ..policy.policy import CustomOutputPolicy
 from ..policy.policy import InputPolicy
 from ..policy.policy import OutputPolicy
 from ..policy.policy import Policy
+from ..policy.policy import SingleExecutionExactOutput
 from ..policy.policy import SubmitUserPolicy
 from ..policy.policy import UserPolicy
 from ..policy.policy import init_policy
 from ..policy.policy import load_policy_code
 from ..policy.policy_service import PolicyService
 from ..response import SyftError
 from .code_parse import GlobalsVisitor
@@ -178,15 +179,15 @@
     signature: inspect.Signature
     status: UserCodeStatusContext
     input_kwargs: List[str]
     enclave_metadata: Optional[EnclaveMetadata] = None
 
     __attr_searchable__ = ["user_verify_key", "status", "service_func_name"]
     __attr_unique__ = ["code_hash", "user_unique_func_name"]
-    __attr_repr_cols__ = ["status", "service_func_name"]
+    __attr_repr_cols__ = ["status.approved", "service_func_name"]
 
     def __setattr__(self, key: str, value: Any) -> None:
         attr = getattr(type(self), key, None)
         if inspect.isdatadescriptor(attr):
             attr.fset(self, value)
         else:
             return super().__setattr__(key, value)
@@ -292,15 +293,15 @@
         return compile_byte_code(self.parsed_code)
 
     @property
     def assets(self) -> List[Asset]:
         # relative
         from ...client.api import APIRegistry
 
-        api = APIRegistry.api_for(self.node_uid)
+        api = APIRegistry.api_for(self.node_uid, self.syft_client_verify_key)
         if api is None:
             return SyftError(message=f"You must login to {self.node_uid}")
 
         node_view = NodeView(
             node_name=api.node_name, verify_key=api.signing_key.verify_key
         )
         inputs = self.input_policy_init_kwargs[node_view]
@@ -391,21 +392,24 @@
     if hasattr(deboxed_arg, "syft_action_data"):
         deboxed_arg = deboxed_arg.syft_action_data
     return deboxed_arg
 
 
 def syft_function(
     input_policy: Union[InputPolicy, UID],
-    output_policy: Union[OutputPolicy, UID],
+    output_policy: Optional[Union[OutputPolicy, UID]] = None,
 ) -> SubmitUserCode:
     if isinstance(input_policy, CustomInputPolicy):
         input_policy_type = SubmitUserPolicy.from_obj(input_policy)
     else:
         input_policy_type = type(input_policy)
 
+    if output_policy is None:
+        output_policy = SingleExecutionExactOutput()
+
     if isinstance(output_policy, CustomOutputPolicy):
         output_policy_type = SubmitUserPolicy.from_obj(output_policy)
     else:
         output_policy_type = type(output_policy)
 
     def decorator(f):
         return SubmitUserCode(
```

### Comparing `syft-0.8.1b6/src/syft/service/code/user_code_parse.py` & `syft-0.8.1b7/src/syft/service/code/user_code_parse.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.1b6/src/syft/service/code/user_code_service.py` & `syft-0.8.1b7/src/syft/service/code/user_code_service.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,23 +1,26 @@
 # stdlib
 from typing import Any
 from typing import Dict
 from typing import List
+from typing import Optional
 from typing import Union
 
 # third party
 from result import OkErr
+from result import Result
 
 # relative
 from ...serde.serializable import serializable
 from ...store.document_store import DocumentStore
 from ...store.linked_obj import LinkedObject
 from ...types.twin_object import TwinObject
 from ...types.uid import UID
 from ...util.telemetry import instrument
+from ..action.action_object import ActionObject
 from ..context import AuthedServiceContext
 from ..policy.policy import OutputHistory
 from ..request.request import SubmitRequest
 from ..request.request import UserCodeStatusChange
 from ..request.request_service import RequestService
 from ..response import SyftError
 from ..response import SyftNotReady
@@ -54,14 +57,15 @@
             return SyftError(message=str(result.err()))
         return SyftSuccess(message="User Code Submitted")
 
     def _code_execution(
         self,
         context: AuthedServiceContext,
         code: SubmitUserCode,
+        reason: Optional[str] = "",
     ):
         user_code = code.to(UserCode, context=context)
         result = self.stash.set(context.credentials, user_code)
         if result.is_err():
             return SyftError(message=str(result.err()))
 
         linked_obj = LinkedObject.from_obj(user_code, node_uid=context.node.id)
@@ -69,29 +73,32 @@
         CODE_EXECUTE = UserCodeStatusChange(
             value=UserCodeStatus.EXECUTE, linked_obj=linked_obj
         )
         changes = [CODE_EXECUTE]
 
         request = SubmitRequest(changes=changes)
         method = context.node.get_service_method(RequestService.submit)
-        result = method(context=context, request=request)
+        result = method(context=context, request=request, reason=reason)
 
         # The Request service already returns either a SyftSuccess or SyftError
         return result
 
     @service_method(
         path="code.request_code_execution",
         name="request_code_execution",
         roles=GUEST_ROLE_LEVEL,
     )
     def request_code_execution(
-        self, context: AuthedServiceContext, code: SubmitUserCode
+        self,
+        context: AuthedServiceContext,
+        code: SubmitUserCode,
+        reason: Optional[str] = "",
     ) -> Union[SyftSuccess, SyftError]:
         """Request Code execution on user code"""
-        return self._code_execution(context=context, code=code)
+        return self._code_execution(context=context, code=code, reason=reason)
 
     @service_method(path="code.get_all", name="get_all", roles=GUEST_ROLE_LEVEL)
     def get_all(
         self, context: AuthedServiceContext
     ) -> Union[List[UserCode], SyftError]:
         """Get a Dataset"""
         result = self.stash.get_all(context.credentials)
@@ -149,15 +156,25 @@
             if not result.is_ok():
                 return SyftError(message=result.err())
 
             # Unroll variables
             code_item = result.ok()
             status = code_item.status
 
-            # Check if we are allowed to execute the code
+            # Check if the user has permission to execute the code
+            # They can execute if they are root user or if they are the user who submitted the code
+            if not (
+                context.credentials == context.node.verify_key
+                or context.credentials == code_item.user_verify_key
+            ):
+                return SyftError(
+                    message=f"Code Execution Permission: {context.credentials} denied"
+                )
+
+            # Check if the code is approved
             if status.for_context(context) != UserCodeStatus.EXECUTE:
                 if status.for_context(context) == UserCodeStatus.SUBMITTED:
                     return SyftNotReady(
                         message=f"{type(code_item)} Your code is waiting for approval: {status}"
                     )
                 return SyftError(
                     message=f"{type(code_item)} Your code cannot be run: {status}"
@@ -168,38 +185,42 @@
                 raise Exception("Output policy not approved", code_item)
 
             # Check if the OutputPolicy is valid
             is_valid = output_policy.valid
 
             if not is_valid:
                 if len(output_policy.output_history) > 0:
-                    return get_outputs(
+                    result = get_outputs(
                         context=context,
                         output_history=output_policy.output_history[-1],
                     )
+                    return result.as_empty()
                 return is_valid
 
             # Execute the code item
             action_service = context.node.get_service("actionservice")
-            result = action_service._user_code_execute(
+            result: Result = action_service._user_code_execute(
                 context, code_item, filtered_kwargs
             )
             if isinstance(result, str):
                 return SyftError(message=result)
 
             # Apply Output Policy to the results and update the OutputPolicyState
-            final_results = result.ok()
-            output_policy.apply_output(context=context, outputs=final_results)
+            result: Union[ActionObject, TwinObject] = result.ok()
+            output_policy.apply_output(context=context, outputs=result)
             code_item.output_policy = output_policy
-            state_result = self.update_code_state(context=context, code_item=code_item)
-            if not state_result:
-                return state_result
-            if isinstance(final_results, TwinObject):
-                return final_results.private
-            return final_results
+            update_success = self.update_code_state(
+                context=context, code_item=code_item
+            )
+            if not update_success:
+                return update_success
+            if isinstance(result, TwinObject):
+                return result.mock
+            else:
+                return result.as_empty()
         except Exception as e:
             return SyftError(message=f"Failed to run. {e}")
 
 
 def get_outputs(context: AuthedServiceContext, output_history: OutputHistory) -> Any:
     # relative
     from ...service.action.action_object import TwinMode
```

### Comparing `syft-0.8.1b6/src/syft/service/code/user_code_stash.py` & `syft-0.8.1b7/src/syft/service/code/user_code_stash.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.1b6/src/syft/service/context.py` & `syft-0.8.1b7/src/syft/service/context.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.1b6/src/syft/service/data_subject/data_subject.py` & `syft-0.8.1b7/src/syft/service/data_subject/data_subject.py`

 * *Files 7% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 from ...types.syft_object import SYFT_OBJECT_VERSION_1
 from ...types.syft_object import SyftObject
 from ...types.transforms import TransformContext
 from ...types.transforms import add_node_uid_for_key
 from ...types.transforms import generate_id
 from ...types.transforms import transform
 from ...types.uid import UID
+from ...util.markdown import as_markdown_python_code
 from ..response import SyftError
 
 NamePartitionKey = PartitionKey(key="name", type_=str)
 
 
 @serializable()
 class DataSubject(SyftObject):
@@ -35,15 +36,15 @@
     aliases: List[str] = []
 
     @property
     def members(self) -> List:
         # relative
         from ...client.api import APIRegistry
 
-        api = APIRegistry.api_for(self.node_uid)
+        api = APIRegistry.api_for(self.node_uid, self.syft_client_verify_key)
         if api is None:
             return SyftError(message=f"You must login to {self.node_uid}")
         members = api.services.data_subject.members_for(self.name)
         return members
 
     __attr_searchable__ = ["name", "description"]
     __attr_unique__ = ["name"]
@@ -58,15 +59,15 @@
         return f"<DataSubject: {self.name}>"
 
     def _repr_markdown_(self) -> str:
         _repr_str = f"DataSubject: {self.name}\n"
         _repr_str += f"Description: {self.description}\n"
         _repr_str += f"Aliases: {self.aliases}\n"
         _repr_str += f"Members: {len(self.members)}\n"
-        return "```python\n" + _repr_str + "\n```"
+        return as_markdown_python_code(_repr_str)
 
 
 @serializable()
 class DataSubjectCreate(SyftObject):
     # version
     __canonical_name__ = "DataSubjectCreate"
     __version__ = SYFT_OBJECT_VERSION_1
@@ -104,15 +105,15 @@
         return f"<DataSubject: {self.name}>"
 
     def _repr_markdown_(self) -> str:
         _repr_str = f"DataSubject: {self.name}\n"
         _repr_str += f"Description: {self.description}\n"
         _repr_str += f"Aliases: {self.aliases}\n"
         _repr_str += f"Members: {len(self.members)}\n"
-        return "```python\n" + _repr_str + "\n```"
+        return as_markdown_python_code(_repr_str)
 
 
 def remove_members_list(context: TransformContext) -> TransformContext:
     context.output.pop("members", [])
     return context
```

### Comparing `syft-0.8.1b6/src/syft/service/data_subject/data_subject_member.py` & `syft-0.8.1b7/src/syft/service/data_subject/data_subject_member.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.1b6/src/syft/service/data_subject/data_subject_member_service.py` & `syft-0.8.1b7/src/syft/service/data_subject/data_subject_member_service.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.1b6/src/syft/service/data_subject/data_subject_service.py` & `syft-0.8.1b7/src/syft/service/data_subject/data_subject_service.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.1b6/src/syft/service/dataset/dataset.py` & `syft-0.8.1b7/src/syft/service/dataset/dataset.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,34 +1,43 @@
 # stdlib
 from collections import OrderedDict
 from datetime import datetime
 from enum import Enum
 import sys
 from typing import Any
 from typing import Callable
+from typing import Dict
 from typing import List
 from typing import Optional
 from typing import Tuple
 from typing import Union
 
 # third party
+import itables
+from pydantic import ValidationError
+from pydantic import root_validator
+from pydantic import validator
 from result import Err
 from result import Ok
 from result import Result
 
 # relative
 from ...serde.serializable import serializable
 from ...store.document_store import PartitionKey
+from ...types.datetime import DateTime
+from ...types.syft_object import SURFACE_DARK_BRIGHT
 from ...types.syft_object import SYFT_OBJECT_VERSION_1
 from ...types.syft_object import SyftObject
+from ...types.syft_object import itables_css
 from ...types.transforms import TransformContext
 from ...types.transforms import generate_id
 from ...types.transforms import transform
 from ...types.transforms import validate_url
 from ...types.uid import UID
+from ...util.markdown import as_markdown_python_code
 from ..data_subject.data_subject import DataSubject
 from ..data_subject.data_subject import DataSubjectCreate
 from ..data_subject.data_subject_service import DataSubjectService
 from ..response import SyftError
 from ..response import SyftException
 from ..response import SyftSuccess
 
@@ -68,82 +77,130 @@
     node_uid: UID
     name: str
     description: Optional[str]
     contributors: List[Contributor] = []
     data_subjects: List[DataSubject] = []
     mock_is_real: bool = False
     shape: Optional[Tuple]
+    created_at: DateTime = DateTime.now()
+
+    __attr_repr_cols__ = ["name", "shape"]
 
     # @property
     # def pointer(self) -> ActionObjectPointer:
     #     api = APIRegistry.api_for(node_uid=self.node_uid)
     #     obj_ptr = api.services.action.get_pointer(uid=self.action_id)
     #     return obj_ptr
 
+    def _repr_html_(self) -> Any:
+        # relative
+        from ...service.action.action_object import ActionObject
+
+        uploaded_by_line = ""
+        if len(self.contributors) > 0:
+            uploaded_by_line = (
+                f"<p><strong>Uploaded by: </strong>{self.contributors[0].name}</p>"
+            )
+        if isinstance(self.data, ActionObject):
+            data_table_line = itables.to_html_datatable(
+                df=self.data.syft_action_data, css=itables_css
+            )
+        else:
+            data_table_line = self.data
+        return (
+            f"""
+            <style>
+            .syft-asset {{color: {SURFACE_DARK_BRIGHT};}}
+            </style>
+            """
+            + '<div class="syft-asset">'
+            + f"<h3>{self.name}</h3>"
+            + f"<p>{self.description}</p>"
+            + f"<p><strong>Asset ID: </strong>{self.id}</p>"
+            + f"<p><strong>Action Object ID: </strong>{self.action_id}</p>"
+            + uploaded_by_line
+            + f"<p><strong>Created on: </strong>{self.created_at}</p>"
+            + "<p><strong>Data:</strong></p>"
+            + data_table_line
+            + "<p><strong>Mock Data:</strong></p>"
+            + itables.to_html_datatable(df=self.mock_data, css=itables_css)
+            + "</div>"
+        )
+
     def _repr_markdown_(self) -> str:
         _repr_str = f"Asset: {self.name}\n"
         _repr_str += f"Pointer Id: {self.action_id}\n"
         _repr_str += f"Description: {self.description}\n"
         _repr_str += f"Total Data Subjects: {len(self.data_subjects)}\n"
         _repr_str += f"Shape: {self.shape}\n"
         _repr_str += f"Contributors: {len(self.contributors)}\n"
         for contributor in self.contributors:
             _repr_str += f"\t{contributor.name}: {contributor.email}\n"
-        return "```python\n" + _repr_str + "\n```"
+        return as_markdown_python_code(_repr_str)
 
     @property
     def pointer(self) -> Any:
         # relative
         from ...client.api import APIRegistry
 
-        api = APIRegistry.api_for(node_uid=self.node_uid)
+        api = APIRegistry.api_for(
+            node_uid=self.node_uid,
+            user_verify_key=self.syft_client_verify_key,
+        )
         return api.services.action.get_pointer(self.action_id)
 
     @property
     def mock_data(self) -> Any:
         # relative
         from ...client.api import APIRegistry
 
-        api = APIRegistry.api_for(node_uid=self.node_uid)
+        api = APIRegistry.api_for(
+            node_uid=self.node_uid,
+            user_verify_key=self.syft_client_verify_key,
+        )
         return api.services.action.get_pointer(self.action_id).syft_action_data
 
     @property
     def mock(self) -> Any:
         # relative
         from ...client.api import APIRegistry
 
-        api = APIRegistry.api_for(node_uid=self.node_uid)
+        api = APIRegistry.api_for(
+            node_uid=self.node_uid,
+            user_verify_key=self.syft_client_verify_key,
+        )
         return api.services.action.get_pointer(self.action_id)
 
     @property
     def data(self) -> Any:
         # relative
         from ...client.api import APIRegistry
 
-        api = APIRegistry.api_for(node_uid=self.node_uid)
+        api = APIRegistry.api_for(
+            node_uid=self.node_uid,
+            user_verify_key=self.syft_client_verify_key,
+        )
         return api.services.action.get(self.action_id)
 
 
-def is_action_data_empty(mock: Any) -> bool:
+def _is_action_data_empty(obj: Any) -> bool:
+    # just a wrapper of action_object.is_action_data_empty
+    # to work around circular import error
+
     # relative
-    from ...service.action.action_data_empty import ActionDataEmpty
-    from ...service.action.action_object import AnyActionObject
+    from ...service.action.action_object import is_action_data_empty
 
-    if isinstance(mock, AnyActionObject) and isinstance(
-        mock.syft_action_data, ActionDataEmpty
-    ):
-        return True
-    return False
+    return is_action_data_empty(obj)
 
 
 def check_mock(data: Any, mock: Any) -> bool:
     if type(data) == type(mock):
         return True
 
-    return is_action_data_empty(mock)
+    return _is_action_data_empty(mock)
 
 
 @serializable()
 class CreateAsset(SyftObject):
     # version
     __canonical_name__ = "CreateAsset"
     __version__ = SYFT_OBJECT_VERSION_1
@@ -155,14 +212,36 @@
     data_subjects: List[DataSubjectCreate] = []
     node_uid: Optional[UID]
     action_id: Optional[UID]
     data: Optional[Any]
     mock: Optional[Any]
     shape: Optional[Tuple]
     mock_is_real: bool = False
+    created_at: Optional[DateTime]
+
+    class Config:
+        validate_assignment = True
+
+    @root_validator()
+    def __empty_mock_cannot_be_real(cls, values: dict[str, Any]) -> Dict:
+        """set mock_is_real to False whenever mock is None or empty"""
+
+        if (mock := values.get("mock")) is None or _is_action_data_empty(mock):
+            values["mock_is_real"] = False
+
+        return values
+
+    @validator("mock_is_real")
+    def __mock_is_real_for_empty_mock_must_be_false(
+        cls, v: bool, values: dict[str, Any], **kwargs: Any
+    ) -> bool:
+        if v and ((mock := values.get("mock")) is None or _is_action_data_empty(mock)):
+            raise ValueError("mock_is_real must be False if mock is not provided")
+
+        return v
 
     def add_data_subject(self, data_subject: DataSubject) -> None:
         self.data_subjects.append(data_subject)
 
     def add_contributor(
         self,
         name: str,
@@ -181,29 +260,42 @@
         self.description = description
 
     def set_obj(self, data: Any) -> None:
         if isinstance(data, SyftError):
             raise SyftException(data)
         self.data = data
 
-    def set_mock(self, mock_data: Any, mock_is_real: bool) -> Any:
+    def set_mock(self, mock_data: Any, mock_is_real: bool) -> None:
         if isinstance(mock_data, SyftError):
             raise SyftException(mock_data)
+
+        current_mock = self.mock
         self.mock = mock_data
-        self.mock_is_real = mock_is_real
+
+        try:
+            self.mock_is_real = mock_is_real
+        except ValidationError as e:
+            self.mock = current_mock
+            raise e
+
+    def no_mock(self) -> None:
+        # relative
+        from ..action.action_object import ActionObject
+
+        self.mock = ActionObject.empty()
 
     def set_shape(self, shape: Tuple) -> None:
         self.shape = shape
 
     def check(self) -> Union[SyftSuccess, SyftError]:
         if not check_mock(self.data, self.mock):
             return SyftError(
                 message=f"set_obj type {type(self.data)} must match set_mock type {type(self.mock)}"
             )
-        if not is_action_data_empty(self.mock):
+        if not _is_action_data_empty(self.mock):
             data_shape = get_shape_or_len(self.data)
             mock_shape = get_shape_or_len(self.mock)
             if data_shape != mock_shape:
                 return SyftError(
                     message=f"set_obj shape {data_shape} must match set_mock shape {mock_shape}"
                 )
 
@@ -234,67 +326,148 @@
     contributors: List[Contributor] = []
     citation: Optional[str]
     url: Optional[str]
     description: Optional[str]
     updated_at: Optional[str]
     requests: Optional[int] = 0
     mb_size: Optional[int]
+    created_at: DateTime = DateTime.now()
 
     __attr_searchable__ = ["name", "citation", "url", "description", "action_ids"]
     __attr_unique__ = ["name"]
     __attr_repr_cols__ = ["name", "url"]
 
+    def _repr_html_(self) -> Any:
+        uploaded_by_line = ""
+        if len(self.contributors) > 0:
+            uploaded_by_line = (
+                f"<p><strong>Uploaded by: </strong>{self.contributors[0].name}</p>"
+            )
+        return (
+            f"""
+            <style>
+            .syft-dataset {{color: {SURFACE_DARK_BRIGHT};}}
+            </style>
+            """
+            + "<div class='syft-dataset'>"
+            + f"<h3>{self.name}</h3>"
+            + f"<p>{self.description}</p>"
+            + uploaded_by_line
+            + f"<p><strong>Created on: </strong>{self.created_at}</p>"
+            + f'<p><strong>URL: </strong><a href="{self.url}">{self.url}</a></p>'
+            + "<p><strong>Contributors: </strong> to see full details call dataset.contributors</p>"
+            + self.asset_list._repr_html_()
+            + "</div>"
+        )
+
     def action_ids(self) -> List[UID]:
         data = []
         for asset in self.asset_list:
             if asset.action_id:
                 data.append(asset.action_id)
         return data
 
     @property
     def assets(self) -> TupleDict:
         data = TupleDict()
         for asset in self.asset_list:
             data[asset.name] = asset
         return data
 
-    def _repr_markdown_(self) -> str:
+    def _old_repr_markdown_(self) -> str:
         _repr_str = f"Syft Dataset: {self.name}\n"
         _repr_str += "Assets:\n"
         for asset in self.asset_list:
             _repr_str += f"\t{asset.name}: {asset.description}\n"
         if self.citation:
             _repr_str += f"Citation: {self.citation}\n"
         if self.url:
             _repr_str += f"URL: {self.url}\n"
         if self.description:
             _repr_str += f"Description: {self.description}\n"
-        return "```python\n" + _repr_str + "\n```"
+        return as_markdown_python_code(_repr_str)
+
+    def _repr_markdown_(self) -> str:
+        # return self._old_repr_markdown_()
+        return self._markdown_()
+
+    def _markdown_(self) -> str:
+        _repr_str = f"Syft Dataset: {self.name}\n\n"
+        _repr_str += "Assets:\n\n"
+        for asset in self.asset_list:
+            _repr_str += f"\t{asset.name}: {asset.description}\n\n"
+        if self.citation:
+            _repr_str += f"Citation: {self.citation}\n\n"
+        if self.url:
+            _repr_str += f"URL: {self.url}\n\n"
+        if self.description:
+            _repr_str += f"Description: \n\n{self.description}\n\n"
+        return _repr_str
 
     @property
     def client(self) -> Optional[Any]:
         # relative
         from ...client.client import SyftClientSessionCache
 
         client = SyftClientSessionCache.get_client_for_node_uid(self.node_uid)
         if client is None:
             return SyftError(
                 message=f"No clients for {self.node_uid} in memory. Please login with sy.login"
             )
         return client
 
 
+_ASSET_WITH_NONE_MOCK_ERROR_MESSAGE: str = "".join(
+    [
+        "To be included in a Dataset, an asset must either contain a mock, ",
+        "or have it explicitly set to be empty.\n",
+        "You can create an asset without a mock with `sy.Asset(..., mock=sy.ActionObject.empty())` or\n"
+        "set the mock of an existing asset to be empty with `asset.no_mock()` or ",
+        "`asset.mock = sy.ActionObject.empty()`.",
+    ]
+)
+
+
+def _check_asset_must_contain_mock(asset_list: List[CreateAsset]) -> None:
+    assets_without_mock = [asset.name for asset in asset_list if asset.mock is None]
+    if assets_without_mock:
+        raise ValueError(
+            "".join(
+                [
+                    "These assets do not contain a mock:\n",
+                    *[f"{asset}\n" for asset in assets_without_mock],
+                    "\n",
+                    _ASSET_WITH_NONE_MOCK_ERROR_MESSAGE,
+                ]
+            )
+        )
+
+
 @serializable()
 class CreateDataset(Dataset):
     # version
     __canonical_name__ = "CreateDataset"
     __version__ = SYFT_OBJECT_VERSION_1
     asset_list: List[CreateAsset] = []
 
     id: Optional[UID] = None
+    created_at: Optional[DateTime]
+
+    class Config:
+        validate_assignment = True
+
+    def _check_asset_must_contain_mock(self) -> None:
+        _check_asset_must_contain_mock(self.asset_list)
+
+    @validator("asset_list")
+    def __assets_must_contain_mock(
+        cls, asset_list: List[CreateAsset]
+    ) -> List[CreateAsset]:
+        _check_asset_must_contain_mock(asset_list)
+        return asset_list
 
     def set_description(self, description: str) -> None:
         self.description = description
 
     def add_citation(self, citation: str) -> None:
         self.citation = citation
 
@@ -312,14 +485,17 @@
         _role_str = role.value if isinstance(role, Enum) else role
         contributor = Contributor(
             name=name, role=_role_str, email=email, phone=phone, note=note
         )
         self.contributors.append(contributor)
 
     def add_asset(self, asset: CreateAsset) -> None:
+        if asset.mock is None:
+            raise ValueError(_ASSET_WITH_NONE_MOCK_ERROR_MESSAGE)
+
         self.asset_list.append(asset)
 
     def remove_asset(self, name: str) -> None:
         asset_to_remove = None
         for asset in self.asset_list:
             if asset.name == name:
                 asset_to_remove = asset
@@ -367,15 +543,15 @@
         private_obj = context.output.pop("data", None)
         mock_obj = context.output.pop("mock", None)
     return context
 
 
 def infer_shape(context: TransformContext) -> TransformContext:
     if context.output["shape"] is None:
-        if not is_action_data_empty(context.obj.mock):
+        if not _is_action_data_empty(context.obj.mock):
             context.output["shape"] = get_shape_or_len(context.obj.mock)
     return context
 
 
 def set_data_subjects(context: TransformContext) -> TransformContext:
     data_subjects = context.output["data_subjects"]
     get_data_subject = context.node.get_service_method(DataSubjectService.get_by_name)
@@ -386,17 +562,28 @@
         if isinstance(result, SyftError):
             return result
         resultant_data_subjects.append(result)
     context.output["data_subjects"] = resultant_data_subjects
     return context
 
 
+def add_msg_creation_time(context: TransformContext) -> TransformContext:
+    context.output["created_at"] = DateTime.now()
+    return context
+
+
 @transform(CreateAsset, Asset)
 def createasset_to_asset() -> List[Callable]:
-    return [generate_id, infer_shape, create_and_store_twin, set_data_subjects]
+    return [
+        generate_id,
+        add_msg_creation_time,
+        infer_shape,
+        create_and_store_twin,
+        set_data_subjects,
+    ]
 
 
 def convert_asset(context: TransformContext) -> TransformContext:
     assets = context.output.pop("asset_list", [])
     dataset_size = 0
     for idx, create_asset in enumerate(assets):
         dataset_size += sys.getsizeof(assets) / 1024
@@ -412,12 +599,18 @@
     formatted_date = current_date.strftime("%b %d, %Y")
     context.output["updated_at"] = formatted_date
     return context
 
 
 @transform(CreateDataset, Dataset)
 def createdataset_to_dataset() -> List[Callable]:
-    return [generate_id, validate_url, convert_asset, add_current_date]
+    return [
+        generate_id,
+        add_msg_creation_time,
+        validate_url,
+        convert_asset,
+        add_current_date,
+    ]
 
 
 class DatasetUpdate:
     pass
```

### Comparing `syft-0.8.1b6/src/syft/service/dataset/dataset_service.py` & `syft-0.8.1b7/src/syft/service/dataset/dataset_service.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.1b6/src/syft/service/dataset/dataset_stash.py` & `syft-0.8.1b7/src/syft/service/dataset/dataset_stash.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.1b6/src/syft/service/message/message_service.py` & `syft-0.8.1b7/src/syft/service/message/message_service.py`

 * *Files 14% similar despite different names*

```diff
@@ -11,19 +11,21 @@
 from ..response import SyftError
 from ..response import SyftSuccess
 from ..service import AbstractService
 from ..service import SERVICE_TO_TYPES
 from ..service import TYPE_TO_SERVICE
 from ..service import service_method
 from ..user.user_roles import DATA_SCIENTIST_ROLE_LEVEL
+from ..user.user_roles import GUEST_ROLE_LEVEL
 from .message_stash import MessageStash
 from .messages import CreateMessage
 from .messages import LinkedObject
 from .messages import Message
 from .messages import MessageStatus
+from .messages import ReplyMessage
 
 
 @instrument
 @serializable()
 class MessageService(AbstractService):
     store: DocumentStore
     stash: MessageStash
@@ -40,14 +42,37 @@
 
         new_message = message.to(Message, context=context)
         result = self.stash.set(context.credentials, new_message)
         if result.is_err():
             return SyftError(message=str(result.err()))
         return result.ok()
 
+    @service_method(path="messages.reply", name="reply", roles=GUEST_ROLE_LEVEL)
+    def reply(
+        self,
+        context: AuthedServiceContext,
+        reply: ReplyMessage,
+    ) -> Union[ReplyMessage, SyftError]:
+        msg = self.stash.get_by_uid(
+            credentials=context.credentials, uid=reply.target_msg
+        )
+        if msg.is_ok():
+            msg = msg.ok()
+            reply.from_user_verify_key = context.credentials
+            msg.replies.append(reply)
+            result = self.stash.update(credentials=context.credentials, obj=msg)
+            if result.is_ok():
+                return result.ok()
+            else:
+                SyftError(
+                    message="Couldn't add a new message reply in the target message."
+                )
+        else:
+            SyftError(message="The target message id {reply.target_msg} was not found!")
+
     @service_method(path="messages.get_all", name="get_all")
     def get_all(self, context: AuthedServiceContext) -> Union[List[Message], SyftError]:
         result = self.stash.get_all_inbox_for_verify_key(
             context.credentials, verify_key=context.credentials
         )
         if result.err():
             return SyftError(message=str(result.err()))
@@ -122,15 +147,19 @@
         result = self.stash.update_message_status(
             context.credentials, uid=uid, status=MessageStatus.UNREAD
         )
         if result.is_err():
             return SyftError(message=str(result.err()))
         return result.ok()
 
-    @service_method(path="messages.resolve_object", name="resolve_object")
+    @service_method(
+        path="messages.resolve_object",
+        name="resolve_object",
+        roles=GUEST_ROLE_LEVEL,
+    )
     def resolve_object(
         self, context: AuthedServiceContext, linked_obj: LinkedObject
     ) -> Union[Message, SyftError]:
         service = context.node.get_service(linked_obj.service_type)
         result = service.resolve_link(context=context, linked_obj=linked_obj)
         if result.is_err():
             return SyftError(message=str(result.err()))
@@ -141,10 +170,21 @@
         result = self.stash.delete_all_for_verify_key(
             credentials=context.credentials, verify_key=context.credentials
         )
         if result.is_ok():
             return SyftSuccess(message="All messages cleared !!")
         return SyftError(message=str(result.err()))
 
+    def filter_by_obj(
+        self, context: AuthedServiceContext, obj_uid: UID
+    ) -> Union[Message, SyftError]:
+        messages = self.stash.get_all(context.credentials)
+        if messages.is_ok():
+            for message in messages.ok():
+                if message.linked_obj and message.linked_obj.object_uid == obj_uid:
+                    return message
+        else:
+            return SyftError(message="Could not get messages!!")
+
 
 TYPE_TO_SERVICE[Message] = MessageService
 SERVICE_TO_TYPES[MessageService].update({Message})
```

### Comparing `syft-0.8.1b6/src/syft/service/message/message_stash.py` & `syft-0.8.1b7/src/syft/service/message/message_stash.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.1b6/src/syft/service/message/messages.py` & `syft-0.8.1b7/src/syft/service/message/messages.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 # stdlib
 from enum import Enum
+from typing import List
 from typing import Optional
 
 # relative
 from ...client.api import APIRegistry
 from ...node.credentials import SyftVerifyKey
 from ...serde.serializable import serializable
 from ...store.linked_obj import LinkedObject
@@ -26,25 +27,37 @@
 
 class MessageExpiryStatus(Enum):
     AUTO = 0
     NEVER = 1
 
 
 @serializable()
+class ReplyMessage(SyftObject):
+    __canonical_name__ = "ReplyMessage"
+    __version__ = SYFT_OBJECT_VERSION_1
+
+    text: str
+    target_msg: UID
+    id: Optional[UID]
+    from_user_verify_key: Optional[SyftVerifyKey]
+
+
+@serializable()
 class Message(SyftObject):
     __canonical_name__ = "Message"
     __version__ = SYFT_OBJECT_VERSION_1
 
     subject: str
     node_uid: UID
     from_user_verify_key: SyftVerifyKey
     to_user_verify_key: SyftVerifyKey
     created_at: DateTime
     status: MessageStatus = MessageStatus.UNREAD
     linked_obj: Optional[LinkedObject]
+    replies: Optional[List[ReplyMessage]] = []
 
     __attr_searchable__ = [
         "from_user_verify_key",
         "to_user_verify_key",
         "status",
     ]
     __attr_repr_cols__ = ["subject", "status", "created_at", "linked_obj"]
@@ -52,19 +65,22 @@
     @property
     def link(self) -> Optional[SyftObject]:
         if self.linked_obj:
             return self.linked_obj.resolve
         return None
 
     def mark_read(self) -> None:
-        api = APIRegistry.api_for(self.node_uid)
+        api = APIRegistry.api_for(self.node_uid, self.syft_client_verify_key)
         return api.services.messages.mark_as_read(uid=self.id)
 
     def mark_unread(self) -> None:
-        api = APIRegistry.api_for(self.node_uid)
+        api = APIRegistry.api_for(
+            self.node_uid,
+            self.syft_client_verify_key,
+        )
         return api.services.messages.mark_as_unread(uid=self.id)
 
 
 @serializable()
 class CreateMessage(Message):
     __canonical_name__ = "CreateMessage"
     __version__ = SYFT_OBJECT_VERSION_1
```

### Comparing `syft-0.8.1b6/src/syft/service/metadata/node_metadata.py` & `syft-0.8.1b7/src/syft/service/metadata/node_metadata.py`

 * *Files 0% similar despite different names*

```diff
@@ -104,15 +104,15 @@
             server_name=self.name,
         )
 
 
 @transform(NodeMetadata, NodeMetadataJSON)
 def metadata_to_json() -> List[Callable]:
     return [
-        drop("__canonical_name__"),
+        drop(["__canonical_name__"]),
         rename("__version__", "metadata_version"),
         convert_types(["id", "verify_key"], str),
     ]
 
 
 @transform(NodeMetadataJSON, NodeMetadata)
 def json_to_metadata() -> List[Callable]:
```

### Comparing `syft-0.8.1b6/src/syft/service/network/network_service.py` & `syft-0.8.1b7/src/syft/service/network/network_service.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.1b6/src/syft/service/network/node_peer.py` & `syft-0.8.1b7/src/syft/service/network/node_peer.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.1b6/src/syft/service/network/routes.py` & `syft-0.8.1b7/src/syft/service/network/routes.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.1b6/src/syft/service/policy/policy.py` & `syft-0.8.1b7/src/syft/service/policy/policy.py`

 * *Files 2% similar despite different names*

```diff
@@ -195,25 +195,33 @@
 ) -> Dict:
     # relative
     from ...service.action.action_object import TwinMode
 
     action_service = context.node.get_service("actionservice")
     code_inputs = {}
 
+    # When we are retrieving the code from the database, we need to use the node's
+    # verify key as the credentials. This is because when we approve the code, we
+    # we allow the private data to be used only for this specific code.
+    # but we are not modifying the permissions of the private data
+
+    root_context = AuthedServiceContext(
+        node=context.node, credentials=context.node.verify_key
+    )
     if context.node.node_type == NodeType.DOMAIN:
         for var_name, arg_id in allowed_inputs.items():
             kwarg_value = action_service.get(
-                context=context, uid=arg_id, twin_mode=TwinMode.NONE
+                context=root_context, uid=arg_id, twin_mode=TwinMode.NONE
             )
             if kwarg_value.is_err():
                 return kwarg_value
             code_inputs[var_name] = kwarg_value.ok()
 
     elif context.node.node_type == NodeType.ENCLAVE:
-        dict_object = action_service.get(context=context, uid=code_item_id)
+        dict_object = action_service.get(context=root_context, uid=code_item_id)
         if dict_object.is_err():
             return dict_object
         for value in dict_object.ok().base_dict.values():
             code_inputs.update(value)
 
     else:
         raise Exception(
```

### Comparing `syft-0.8.1b6/src/syft/service/policy/policy_service.py` & `syft-0.8.1b7/src/syft/service/policy/policy_service.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.1b6/src/syft/service/policy/user_policy_stash.py` & `syft-0.8.1b7/src/syft/service/policy/user_policy_stash.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.1b6/src/syft/service/project/project.py` & `syft-0.8.1b7/src/syft/service/project/project.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,45 +1,50 @@
 # future
 from __future__ import annotations
 
 # stdlib
 import copy
+import hashlib
 import textwrap
 import time
 from typing import Any
 from typing import Callable
 from typing import Dict
 from typing import Iterable
 from typing import List
 from typing import Optional
 from typing import Set
+from typing import Tuple
 from typing import Type
 from typing import Union
 
 # third party
 import pydantic
-from pydantic import root_validator
 from pydantic import validator
 from rich.progress import Progress
 from typing_extensions import Self
 
 # relative
 from ...client.client import SyftClient
 from ...client.client import SyftClientSessionCache
 from ...node.credentials import SyftSigningKey
 from ...node.credentials import SyftVerifyKey
 from ...serde.serializable import serializable
+from ...serde.serialize import _serialize
 from ...service.metadata.node_metadata import NodeMetadata
+from ...store.linked_obj import LinkedObject
 from ...types.datetime import DateTime
 from ...types.syft_object import SYFT_OBJECT_VERSION_1
 from ...types.syft_object import SyftObject
 from ...types.transforms import TransformContext
 from ...types.transforms import keep
 from ...types.transforms import transform
 from ...types.uid import UID
+from ...util.markdown import markdown_as_class_with_fields
+from ..code.user_code import SubmitUserCode
 from ..network.network_service import NodePeer
 from ..network.routes import NodeRoute
 from ..network.routes import connection_to_route
 from ..request.request import Request
 from ..response import SyftError
 from ..response import SyftException
 from ..response import SyftNotReady
@@ -58,16 +63,15 @@
     id: UID
     verify_key: SyftVerifyKey
 
     __attr_repr_cols__ = ["id", "verify_key"]
 
     def __repr__(self) -> str:
         verify_key_str = f"{self.verify_key}"
-        id_str = f"{self.id}"
-        return f"<🔑 {verify_key_str[0:8]} @ 🟢 {id_str[0:8]}>"
+        return f"<🔑 {verify_key_str[0:8]} @ 🟢 {self.id.short()}>"
 
     @classmethod
     def from_client(cls, client: SyftClient) -> Identity:
         return cls(id=client.id, verify_key=client.credentials.verify_key)
 
 
 @serializable()
@@ -92,18 +96,15 @@
     return [keep(["id", "verify_key"])]
 
 
 class ProjectEvent(SyftObject):
     __canonical_name__ = "ProjectEvent"
     __version__ = SYFT_OBJECT_VERSION_1
 
-    __hash_exclude_attrs__ = [
-        "event_hash",
-        "signature",
-    ]
+    __hash_exclude_attrs__ = ["event_hash", "signature"]
 
     # 1. Creation attrs
     id: UID
     timestamp: DateTime
     allowed_sub_types: Optional[List] = []
     # 2. Rebase attrs
     project_id: Optional[UID]
@@ -141,16 +142,15 @@
 
     @property
     def valid(self) -> Union[SyftSuccess, SyftError]:
         if self.signature is None:
             return SyftError(message="Sign event first")
         try:
             # Recompute hash
-            event_hash_bytes = self.__sha256__()
-            current_hash = event_hash_bytes.hex()
+            event_hash_bytes, current_hash = create_project_event_hash(self)
             if current_hash != self.event_hash:
                 raise Exception(
                     f"Event hash {current_hash} does not match {self.event_hash}"
                 )
 
             self.creator_verify_key.verify_key.verify(event_hash_bytes, self.signature)
             return SyftSuccess(message="Event signature is valid")
@@ -208,16 +208,16 @@
     def sign(self, signing_key: SyftSigningKey) -> None:
         if self.creator_verify_key != signing_key.verify_key:
             raise Exception(
                 f"creator_verify_key has changed from: {self.creator_verify_key} to "
                 f"{signing_key.verify_key}"
             )
         # Calculate Hash
-        event_hash_bytes = self.__sha256__()
-        self.event_hash = event_hash_bytes.hex()
+        event_hash_bytes, event_hash = create_project_event_hash(self)
+        self.event_hash = event_hash
 
         # Sign Hash
         signed_obj = signing_key.signing_key.sign(event_hash_bytes)
         self.signature = signed_obj._signature
 
     def publish(self, project: Project) -> Union[SyftSuccess, SyftError]:
         try:
@@ -282,23 +282,57 @@
 
 
 @serializable()
 class ProjectRequest(ProjectEventAddObject):
     __canonical_name__ = "ProjectRequest"
     __version__ = SYFT_OBJECT_VERSION_1
 
-    request: Request
+    linked_request: LinkedObject
     allowed_sub_types: List[Type] = [ProjectRequestResponse]
 
+    @validator("linked_request", pre=True)
+    def _validate_linked_request(cls, v):
+        if isinstance(v, Request):
+            linked_request = LinkedObject.from_obj(v, node_uid=v.node_uid)
+            return linked_request
+        elif isinstance(v, LinkedObject):
+            return v
+        else:
+            raise ValueError(
+                f"linked_request should be either Request or LinkedObject, got {type(v)}"
+            )
+
+    @property
+    def request(self):
+        return self.linked_request.resolve
+
+    __attr_repr_cols__ = [
+        "request.status",
+        "request.changes[-1].link.service_func_name",
+    ]
+
+    def _repr_markdown_(self) -> str:
+        func_name = None
+        if len(self.request.changes) > 0:
+            func_name = self.request.changes[-1].link.service_func_name
+        repr_dict = {
+            "request.status": self.request.status,
+            "request.changes[-1].link.service_func_name": func_name,
+        }
+        return markdown_as_class_with_fields(self, repr_dict)
+
     def approve(self) -> ProjectRequestResponse:
         result = self.request.approve()
         if isinstance(result, SyftError):
             return result
         return ProjectRequestResponse(response=True, parent_event_id=self.id)
 
+    def accept_by_depositing_result(self, result: Any, force: bool = False):
+        return self.request.accept_by_depositing_result(result=result, force=force)
+
     # TODO: To add deny requests, when deny functionality is added
 
     def status(self, project: Project) -> Union[Dict, SyftError]:
         """Returns the status of the request
 
         Args:
             project (Project): Project object to check the status
@@ -589,49 +623,100 @@
             return False
         return self.threshold == value.threshold
 
     def __hash__(self) -> int:
         return hash(self.threshold)
 
 
+def add_code_request_to_project(
+    project: Union[ProjectSubmit, Project],
+    code: SubmitUserCode,
+    client: SyftClient,
+    reason: Optional[str] = None,
+):
+    if not isinstance(code, SubmitUserCode):
+        return SyftError(
+            message=f"Currently we are  only support creating requests for SubmitUserCode: {type(code)}"
+        )
+
+    if not isinstance(client, SyftClient):
+        return SyftError(message="Client should be a valid SyftClient")
+
+    if reason is None:
+        reason = f"Code Request for Project: {project.name} has been submitted by {project.created_by}"
+
+    submitted_req = client.api.services.code.request_code_execution(
+        code=code, reason=reason
+    )
+    if isinstance(submitted_req, SyftError):
+        return submitted_req
+
+    request_event = ProjectRequest(linked_request=submitted_req)
+
+    if isinstance(project, ProjectSubmit):
+        project.bootstrap_events.append(request_event)
+    else:
+        result = project.add_event(request_event)
+        if isinstance(result, SyftError):
+            return result
+
+    return SyftSuccess(message="Request added successfully")
+
+
 @serializable()
 class Project(SyftObject):
     __canonical_name__ = "Project"
     __version__ = SYFT_OBJECT_VERSION_1
 
+    __attr_repr_cols__ = ["name", "description", "created_by", "events"]
+    __attr_unique__ = ["name"]
+
+    # TODO: re-add users, members, leader_node_peer
+    __hash_exclude_attrs__ = [
+        "user_signing_key",
+        "start_hash",
+        "users",
+        "members",
+        "leader_node_peer",
+        "event_id_hashmap",
+    ]
+
     id: Optional[UID]
     name: str
     description: Optional[str]
-    shareholders: List[NodeIdentity]
-    project_permissions: Set[str]
-    state_sync_leader: NodeIdentity
-    leader_node_peer: Optional[NodePeer]
-    consensus_model: ConsensusModel
-    store: Dict[UID, Dict[UID, SyftObject]] = {}
-    permissions: Dict[UID, Dict[UID, Set[str]]] = {}
-    events: List[ProjectEvent] = []
-    event_id_hashmap: Dict[UID, ProjectEvent] = {}
+    members: List[NodeIdentity]
+    users: List[UserIdentity] = []
+    created_by: str
     start_hash: Optional[str]
-    # WARNING:  Do not add it to hash keys , or print directly
+    # WARNING:  Do not add it to hash keys or print directly
     user_signing_key: Optional[SyftSigningKey] = None
-    user_email_address: Optional[str] = None
-    users: List[UserIdentity] = []
 
-    __attr_repr_cols__ = ["name", "shareholders", "state_sync_leader"]
-    __hash_exclude_attrs__ = ["user_signing_key", "start_hash"]
+    # Project events
+    events: List[ProjectEvent] = []
+    event_id_hashmap: Dict[UID, ProjectEvent] = {}
+
+    # Project sync
+    state_sync_leader: NodeIdentity
+    leader_node_peer: Optional[NodePeer]
+
+    # Unused
+    consensus_model: ConsensusModel
+    project_permissions: Set[str]
+    # store: Dict[UID, Dict[UID, SyftObject]] = {}
+    # permissions: Dict[UID, Dict[UID, Set[str]]] = {}
 
     def _broadcast_event(
         self, project_event: ProjectEvent
     ) -> Union[SyftSuccess, SyftError]:
         leader_client = self.get_leader_client(self.user_signing_key)
 
         return leader_client.api.services.project.broadcast_event(project_event)
 
     def get_all_identities(self) -> List[Identity]:
-        return [*self.shareholders, *self.users]
+        return [*self.members, *self.users]
 
     def key_in_project(self, verify_key: SyftVerifyKey) -> bool:
         project_verify_keys = [
             identity.verify_key for identity in self.get_all_identities()
         ]
 
         return verify_key in project_verify_keys
@@ -639,15 +724,15 @@
     def get_identity_from_key(
         self, verify_key: SyftVerifyKey
     ) -> List[Union[NodeIdentity, UserIdentity]]:
         identities: List[Identity] = self.get_all_identities()
         for identity in identities:
             if identity.verify_key == verify_key:
                 return identity
-        return SyftError(message=f"Shareholder with verify key: {verify_key} not found")
+        return SyftError(message=f"Member with verify key: {verify_key} not found")
 
     def get_leader_client(self, signing_key: SyftSigningKey) -> SyftClient:
         if self.leader_node_peer is None:
             raise Exception("Leader node peer is not set")
 
         if signing_key is None:
             raise Exception("Signing key is required to create leader client")
@@ -813,14 +898,24 @@
             if len(ids) == 0 or event.id in ids:
                 id_check = True
 
             if type_check and parent_check and id_check:
                 results.append(event)
         return results
 
+    def create_code_request(
+        self, obj: SubmitUserCode, client: SyftClient, reason: Optional[str] = None
+    ):
+        return add_code_request_to_project(
+            project=self,
+            code=obj,
+            client=client,
+            reason=reason,
+        )
+
     def get_messages(self) -> List[Union[ProjectMessage, ProjectThreadMessage]]:
         messages = []
         for event in self.events:
             if isinstance(event, (ProjectMessage, ProjectThreadMessage)):
                 messages.append(event)
         return messages
 
@@ -924,15 +1019,16 @@
             return SyftSuccess(message="Poll answered successfully")
         return result
 
     def add_request(
         self,
         request: Request,
     ):
-        request_event = ProjectRequest(request=request)
+        linked_request = LinkedObject.from_obj(request, node_uid=request.node_uid)
+        request_event = ProjectRequest(linked_request=linked_request)
         result = self.add_event(request_event)
 
         if isinstance(result, SyftSuccess):
             return SyftSuccess(message="Request created successfully")
         return result
 
     # Since currently we do not have the notion of denying a request
@@ -990,190 +1086,285 @@
                         f"[bold white]Syncing... {curr_val}/{len(unsynced_events)}"
                     )
                     progress.update(task1, advance=1)
                     self.events.append(event)
                     self.event_id_hashmap[event.id] = event
                     # for a fancy UI view , deliberately slowing the sync
                     if curr_val <= 7:
-                        time.sleep(0.2)
+                        time.sleep(0.1)
         else:
             for event in unsynced_events:
                 self.events.append(event)
                 self.event_id_hashmap[event.id] = event
 
         return SyftSuccess(message="Synced project  with Leader")
 
+    @property
+    def requests(self) -> List[Request]:
+        return [
+            event.request for event in self.events if isinstance(event, ProjectRequest)
+        ]
 
-@serializable()
+
+@serializable(without=["bootstrap_events", "clients"])
 class ProjectSubmit(SyftObject):
     __canonical_name__ = "ProjectSubmit"
     __version__ = SYFT_OBJECT_VERSION_1
 
-    id: Optional[UID]
+    __hash_exclude_attrs__ = [
+        "start_hash",
+        "users",
+        "members",
+        "clients",
+        "leader_node_route",
+        "bootstrap_events",
+    ]
+
+    # stash rules
+    __attr_repr_cols__ = ["name", "description", "created_by"]
+    __attr_unique__ = ["name"]
+
+    id: UID
+
+    # Init args
     name: str
     description: Optional[str]
-    shareholders: List[NodeIdentity]
-    project_permissions: Set[str] = set()
-    state_sync_leader: Optional[NodeIdentity]
-    consensus_model: ConsensusModel = DemocraticConsensusModel()
-    leader_node_route: Optional[NodeRoute]
-    user_email_address: Optional[str] = None
+    members: Union[List[SyftClient], List[NodeIdentity]]
+
+    # These will be automatically populated
     users: List[UserIdentity] = []
+    created_by: Optional[str] = None
+    clients: List[SyftClient] = []  # List of member clients
+    start_hash: str = ""
 
-    @root_validator(pre=True)
-    def make_shareholders_and_leader_route(cls, values) -> Dict:
-        clients = values["shareholders"]
+    # Project sync args
+    leader_node_route: Optional[NodeRoute]
+    state_sync_leader: Optional[NodeIdentity]
+    bootstrap_events: Optional[List[ProjectEvent]] = []
 
-        if not clients:
-            raise SyftException("Shareholders cannot be empty")
+    # Unused at the moment
+    project_permissions: Set[str] = set()
+    consensus_model: ConsensusModel = DemocraticConsensusModel()
 
-        shareholders = []
-        for client in clients:
-            if isinstance(client, NodeIdentity):
-                shareholders.append(client)
-            elif isinstance(client, SyftClient):
-                metadata = client.metadata.to(NodeMetadata)
-                node_identity = metadata.to(NodeIdentity)
-                shareholders.append(node_identity)
-            else:
-                raise Exception(
-                    f"Shareholders should be either SyftClient or NodeIdentity received: {type(client)}"
+    def __init__(self, *args, **kwargs):
+        super().__init__(*args, **kwargs)
+
+        # Preserve member SyftClients in a private variable clients
+        # self.members will be List[NodeIdentity] on the node i.e. self.clients = []
+        self.clients = self.get_syft_clients(self.members)
+
+        # If ProjectSubmit is being re-created at node side
+        if len(self.clients) == 0:
+            return
+
+        # Populate the created_by
+        self.created_by = self.clients[0].logged_in_user
+
+        # Extract information of logged in user from syft clients
+        self.users = [UserIdentity.from_client(client) for client in self.clients]
+
+        # Convert SyftClients to NodeIdentities
+        self.members = list(map(self.to_node_identity, self.members))
+
+    @validator("members", pre=True)
+    def verify_members(cls, val: Union[List[SyftClient], List[NodeIdentity]]):
+        # SyftClients must be logged in by the same emails
+        clients = cls.get_syft_clients(val)
+        if len(clients) > 0:
+            emails = set([client.logged_in_user for client in clients])
+            if len(emails) > 1:
+                raise SyftException(
+                    f"All clients must be logged in from the same account. Found multiple: {emails}"
                 )
-        if isinstance(clients[0], SyftClient):
-            route_exchange = cls.exchange_routes(clients)
-            if isinstance(route_exchange, SyftError):
-                raise SyftException(route_exchange)
+        return val
 
-            values["leader_node_route"] = connection_to_route(clients[0].connection)
+    @staticmethod
+    def get_syft_clients(vals: Union[List[SyftClient], List[NodeIdentity]]):
+        return [client for client in vals if isinstance(client, SyftClient)]
 
-        values["shareholders"] = shareholders
+    @staticmethod
+    def to_node_identity(val: Union[SyftClient, NodeIdentity]):
+        if isinstance(val, NodeIdentity):
+            return val
+        elif isinstance(val, SyftClient):
+            metadata = val.metadata.to(NodeMetadata)
+            return metadata.to(NodeIdentity)
+        else:
+            raise SyftException(
+                f"members must be SyftClient or NodeIdentity. Received: {type(val)}"
+            )
 
-        return values
+    def create_code_request(
+        self, obj: SubmitUserCode, client: SyftClient, reason: Optional[str] = None
+    ):
+        return add_code_request_to_project(
+            project=self,
+            code=obj,
+            client=client,
+            reason=reason,
+        )
 
-    @root_validator(pre=True)
-    def check_user_email_and_users(cls, values) -> Dict:
-        if values["user_email_address"] is not None:
-            users = values["users"]
-            if len(users) == 0:
-                raise SyftException(
-                    "Users cannot be empty if user email address is provided"
-                )
+    def start(self, return_all_projects=False) -> Project:
+        # Currently we are assuming that the first member is the leader
+        # This would be changed in our future leaderless approach
+        leader = self.clients[0]
+        followers = self.clients[1:]
 
-            share_holders = values["shareholders"]
-            if len(share_holders) != len(users):
-                raise SyftException(
-                    "Number of users should be equal to number of shareholders"
-                )
-            users_node_identity = []
-            for user in users:
-                if isinstance(user, SyftClient):
-                    users_node_identity.append(UserIdentity.from_client(user))
-                elif isinstance(user, UserIdentity):
-                    users_node_identity.append(user)
-                else:
-                    raise SyftException(
-                        "Users should be either SyftClient or UserIdentity"
-                    )
-            values["users"] = users_node_identity
+        try:
+            # Check for DS role across all members
+            self._pre_submit_checks(self.clients)
 
-        return values
+            # Exchange route between leaders and followers
+            self._exchange_routes(leader, followers)
 
-    @staticmethod
-    def exchange_routes(
-        shareholders: List[SyftClient],
-    ) -> Union[SyftSuccess, SyftError]:
+            # create project for each node
+            projects_map = self._create_projects(self.clients)
+
+            # bootstrap project with pending events on leader node's project
+            self._bootstrap_events(projects_map[leader])
+
+            if return_all_projects:
+                return list(projects_map.values())
+
+            return projects_map[leader]
+        except SyftException as exp:
+            return SyftError(message=str(exp))
+
+    def _pre_submit_checks(self, clients: List[SyftClient]):
+        try:
+            # Check if the user can create projects
+            for client in clients:
+                result = client.api.services.project.can_create_project()
+                if isinstance(result, SyftError):
+                    raise SyftException(result.message)
+        except Exception:
+            raise SyftException("Only Data Scientists can create projects")
+
+        return True
+
+    def _exchange_routes(self, leader: SyftClient, followers: List[SyftClient]):
         # Since we are implementing a leader based system
         # To be able to optimize exchanging routes.
-        # We require only the leader to exchange routes with all the shareholders
-        # Meaning if we could guarantee, that the leader node is able to reach the shareholders
-        # the project events could be broadcasted to all the shareholders
+        # We require only the leader to exchange routes with all the members
+        # Meaning if we could guarantee, that the leader node is able to reach the members
+        # the project events could be broadcasted to all the members
 
-        # Currently we are assuming that the first shareholder is the leader
-        # This would be changed in our future leaderless approach
-        leader_client = shareholders[0]
-
-        for follower_client in shareholders[1::]:
-            print()
-            print(
-                f"Exchanging Routes 📡: {leader_client.name} --- {follower_client.name}",
-                end="",
-            )
-            result = leader_client.exchange_route(follower_client)
+        for follower in followers:
+            result = leader.exchange_route(follower)
             if isinstance(result, SyftError):
-                return result
-            print(" ✅")
-            print()
+                raise SyftException(result.message)
 
-        return SyftSuccess(message="Successfully Exchaged Routes")
+        self.leader_node_route = connection_to_route(leader.connection)
 
-    def start(self) -> Project:
-        # Creating a new unique UID to be used by all shareholders
-        project_id = UID()
-        projects = []
-
-        if not self.users:
-            # If the Data Owner creates the project
-            node_identities = self.shareholders
-        else:
-            # If the Data Scientist creates the project
-            node_identities = self.users
-
-        for node_identity in node_identities:
-            client = SyftClientSessionCache.get_client_by_uid_and_verify_key(
-                verify_key=node_identity.verify_key, node_uid=node_identity.id
-            )
-            if client is None:
-                raise SyftException(
-                    f"Client not found for node_identity: {node_identity}"
-                    "Kindly login to the node"
-                )
+    def _create_projects(self, clients: List[SyftClient]):
+        projects: Dict[SyftClient, Project] = dict()
 
-            result = client.api.services.project.create_project(
-                project=self, project_id=project_id
-            )
+        for client in clients:
+            result = client.api.services.project.create_project(project=self)
             if isinstance(result, SyftError):
-                return result
-            else:
-                projects.append(result)
+                raise SyftException(result.message)
+            projects[client] = result
 
-        # as we currently assume that the first shareholder is the leader.
         return projects
 
-    __attr_repr_cols__ = ["name"]
+    def _bootstrap_events(self, leader_project: Project):
+        if not self.bootstrap_events:
+            return
+
+        while len(self.bootstrap_events) > 0:
+            event = self.bootstrap_events.pop(0)
+            result = leader_project.add_event(event)
+            if isinstance(result, SyftError):
+                raise SyftException(result.message)
 
 
-def add_shareholders_as_owners(shareholders: List[SyftVerifyKey]) -> Set[str]:
+def add_members_as_owners(members: List[SyftVerifyKey]) -> Set[str]:
     keys = set()
-    for shareholder in shareholders:
-        owner_key = f"OWNER_{shareholder.verify_key}"
+    for member in members:
+        owner_key = f"OWNER_{member.verify_key}"
         keys.add(owner_key)
     return keys
 
 
 def elect_leader(context: TransformContext) -> TransformContext:
-    if len(context.output["shareholders"]) == 0:
-        raise Exception("Project's require at least one shareholder")
+    if len(context.output["members"]) == 0:
+        raise Exception("Project's require at least one member")
 
-    context.output["state_sync_leader"] = context.output["shareholders"][0]
+    context.output["state_sync_leader"] = context.output["members"][0]
 
     return context
 
 
 def check_permissions(context: TransformContext) -> TransformContext:
-    if len(context.output["shareholders"]) > 1:
+    if len(context.output["members"]) > 1:
         # more than 1 node
         pass
 
     # check at least one owner
     if len(context.output["project_permissions"]) == 0:
         project_permissions = context.output["project_permissions"]
         project_permissions = project_permissions.union(
-            add_shareholders_as_owners(context.output["shareholders"])
+            add_members_as_owners(context.output["members"])
         )
         context.output["project_permissions"] = project_permissions
 
     return context
 
 
 @transform(ProjectSubmit, Project)
 def new_projectsubmit_to_project() -> List[Callable]:
     return [elect_leader, check_permissions]
+
+
+def hash_object(obj: Any) -> Tuple[bytes, str]:
+    """Hashes an object using sha256
+
+    Args:
+        obj (Any): Object to be hashed
+
+    Returns:
+        str: Hashed value of the object
+    """
+    hash_bytes = _serialize(obj, to_bytes=True, for_hashing=True)
+    hash = hashlib.sha256(hash_bytes)
+    return (hash.digest(), hash.hexdigest())
+
+
+def create_project_hash(project: Project) -> Tuple[bytes, str]:
+    # Creating a custom hash for the project
+    # as the recursive hash is yet to be revamped
+    # for primitives python types
+
+    # hashing is calculated based on the following attributes
+    # attrs = ["name", "description", "created_by", "members", "users"]
+
+    return hash_object(
+        [
+            project.name,
+            project.description,
+            project.created_by,
+            [hash_object(member) for member in project.members],
+            [hash_object(user) for user in project.users],
+        ]
+    )
+
+
+def create_project_event_hash(project_event: ProjectEvent) -> Tuple[bytes, str]:
+    # Creating a custom hash for the project
+    # as the recursive hash is yet to be revamped
+    # for primitives python types
+
+    # hashing is calculated based on the following attributes
+    # attrs = ["id", "project_id", "seq no",
+    #  "prev_event_uid", "prev_event_hash", "creator_verify_key"]
+
+    return hash_object(
+        [
+            project_event.id,
+            project_event.project_id,
+            project_event.seq_no,
+            project_event.prev_event_uid,
+            project_event.timestamp.utc_timestamp,
+            project_event.prev_event_hash,
+            hash_object(project_event.creator_verify_key)[1],
+        ]
+    )
```

### Comparing `syft-0.8.1b6/src/syft/service/project/project_service.py` & `syft-0.8.1b7/src/syft/service/project/project_service.py`

 * *Files 14% similar despite different names*

```diff
@@ -15,101 +15,123 @@
 from ..response import SyftNotReady
 from ..response import SyftSuccess
 from ..service import AbstractService
 from ..service import SERVICE_TO_TYPES
 from ..service import TYPE_TO_SERVICE
 from ..service import service_method
 from ..user.user_roles import GUEST_ROLE_LEVEL
-from ..user.user_service import UserService
+from ..user.user_roles import ONLY_DATA_SCIENTIST_ROLE_LEVEL
+from ..user.user_roles import ServiceRole
 from .project import Project
 from .project import ProjectEvent
 from .project import ProjectRequest
 from .project import ProjectSubmit
-from .project_stash import OrderByNamePartitionKey
+from .project import create_project_hash
 from .project_stash import ProjectStash
 
 
 @instrument
 @serializable()
 class ProjectService(AbstractService):
     store: DocumentStore
     stash: ProjectStash
 
     def __init__(self, store: DocumentStore) -> None:
         self.store = store
         self.stash = ProjectStash(store=store)
 
     @service_method(
-        path="project.create_project", name="create_project", roles=GUEST_ROLE_LEVEL
+        path="project.can_create_project",
+        name="can_create_project",
+        roles=ONLY_DATA_SCIENTIST_ROLE_LEVEL,
+    )
+    def can_create_project(
+        self, context: AuthedServiceContext
+    ) -> Union[bool, SyftError]:
+        user_service = context.node.get_service("userservice")
+        role = user_service.get_role_for_credentials(credentials=context.credentials)
+        if role == ServiceRole.DATA_SCIENTIST:
+            return True
+        return SyftError(message="User cannot create projects")
+
+    @service_method(
+        path="project.create_project",
+        name="create_project",
+        roles=ONLY_DATA_SCIENTIST_ROLE_LEVEL,
     )
     def create_project(
-        self,
-        context: AuthedServiceContext,
-        project: ProjectSubmit,
-        project_id: UID,
+        self, context: AuthedServiceContext, project: ProjectSubmit
     ) -> Union[SyftSuccess, SyftError]:
         """Start a Project"""
+
+        check_role = self.can_create_project(context)
+        if isinstance(check_role, SyftError):
+            return check_role
+
         try:
             # Check if the project with given id already exists
             project_id_check = self.stash.get_by_uid(
-                credentials=context.node.verify_key, uid=project_id
+                credentials=context.node.verify_key, uid=project.id
             )
 
             if project_id_check.is_err():
                 return SyftError(message=f"{project_id_check.err()}")
 
             if project_id_check.ok() is not None:
                 return SyftError(
-                    message=f"Project with id {project_id} already exists. Kindly use a different id"
+                    message=f"Project with id: {project.id} already exists."
                 )
 
-            project.id = project_id
             project_obj: Project = project.to(Project, context=context)
 
             # Updating the leader node route of the project object
             # In case the current node, is the leader, they would input their node route
             # For the followers, they would check if the leader is their node peer
             # using the leader's verify_key
             # If the follower do not have the leader as its peer in its routes
             # They would raise as error
             leader_node = project_obj.state_sync_leader
 
             # If the current node is a follower
             # For followers the leader node route is retrieved from its peer
-            if project_obj.state_sync_leader.verify_key != context.node.verify_key:
+            if leader_node.verify_key != context.node.verify_key:
                 network_service = context.node.get_service("networkservice")
                 peer = network_service.stash.get_for_verify_key(
                     credentials=context.node.verify_key,
                     verify_key=leader_node.verify_key,
                 )
                 if peer.is_err():
                     return SyftError(
-                        message=f"Node {context.node.name}-{str(context.node.id)[:6]} does not"
-                        + "leader node as peer. Kindly exchange routes with the leader node"
+                        message=(
+                            f"Leader Node(id={leader_node.id.short()}) is not a "
+                            f"peer of this Node(id={context.node.id.short()})"
+                        )
                     )
                 leader_node_peer = peer.ok()
             else:
                 # for the leader node, as it does not have route information to itself
                 # we rely on the data scientist to provide the route
                 # the route is then validated by the leader
                 leader_node_peer = project.leader_node_route.validate_with_context(
                     context=context
                 )
 
             project_obj.leader_node_peer = leader_node_peer
 
             # This should always be the last call before flushing to DB
-            project_obj.start_hash = project_obj.hash()
+            project_obj.start_hash = create_project_hash(project_obj)[1]
 
             result = self.stash.set(context.credentials, project_obj)
             if result.is_err():
                 return SyftError(message=str(result.err()))
 
             project_obj_store = result.ok()
-            project_obj_store = add_signing_key_to_project(context, project_obj_store)
+            project_obj_store = self.add_signing_key_to_project(
+                context, project_obj_store
+            )
 
             return project_obj_store
 
         except Exception as e:
             print("Failed to submit Project", e)
             raise e
 
@@ -139,15 +161,17 @@
                 return SyftError(
                     message="Only the leader of the project can add events"
                 )
 
             project.events.append(project_event)
             project.event_id_hashmap[project_event.id] = project_event
 
-            message_result = check_for_project_request(project, project_event, context)
+            message_result = self.check_for_project_request(
+                project, project_event, context
+            )
             if isinstance(message_result, SyftError):
                 return message_result
 
             # updating the project object using root verify key of node
             result = self.stash.update(context.node.verify_key, project)
 
             if result.is_err():
@@ -194,31 +218,31 @@
             return SyftNotReady(message="Project out of sync event")
         if project_event.seq_no > len(project.events) + 1:
             return SyftError(message="Project event out of order!")
 
         project.events.append(project_event)
         project.event_id_hashmap[project_event.id] = project_event
 
-        message_result = check_for_project_request(project, project_event, context)
+        message_result = self.check_for_project_request(project, project_event, context)
         if isinstance(message_result, SyftError):
             return message_result
 
         # Broadcast the event to all the members of the project
         network_service = context.node.get_service("networkservice")
-        for sharedholder in project.shareholders:
-            if sharedholder.verify_key != context.node.verify_key:
+        for member in project.members:
+            if member.verify_key != context.node.verify_key:
                 # Retrieving the NodePeer Object to communicate with the node
                 peer = network_service.stash.get_for_verify_key(
                     credentials=context.node.verify_key,
-                    verify_key=sharedholder.verify_key,
+                    verify_key=member.verify_key,
                 )
 
                 if peer.is_err():
                     return SyftError(
-                        message=f"Leader node does not have peer {sharedholder.name}-{sharedholder.id}"
+                        message=f"Leader node does not have peer {member.name}-{member.id.short()}"
                         + " Kindly exchange routes with the peer"
                     )
                 peer = peer.ok()
                 client = peer.client_with_context(context)
                 event_result = client.api.services.project.add_event(project_event)
                 if isinstance(event_result, SyftError):
                     return event_result
@@ -264,78 +288,110 @@
         if project_obj.is_err():
             return SyftError(message=str(project_obj.err()))
 
     @service_method(path="project.get_all", name="get_all", roles=GUEST_ROLE_LEVEL)
     def get_all(self, context: AuthedServiceContext) -> Union[List[Project], SyftError]:
         result = self.stash.get_all(
             context.credentials,
-            order_by=OrderByNamePartitionKey,
         )
         if result.is_err():
             return SyftError(message=str(result.err()))
 
         projects = result.ok()
 
         for idx, project in enumerate(projects):
-            result = add_signing_key_to_project(context, project)
+            result = self.add_signing_key_to_project(context, project)
             if isinstance(result, SyftError):
                 return result
             projects[idx] = result
 
         return projects
 
+    @service_method(
+        path="project.get_by_name",
+        name="get_by_name",
+        roles=GUEST_ROLE_LEVEL,
+    )
+    def get_by_name(
+        self, context: AuthedServiceContext, name: str
+    ) -> Union[Project, SyftError]:
+        result = self.stash.get_by_name(context.credentials, project_name=name)
+        if result.is_err():
+            return SyftError(message=str(result.err()))
+        elif result.ok():
+            project = result.ok()
+            return self.add_signing_key_to_project(context, project)
+        return SyftError(message=f'Project(name="{name}") does not exist')
 
-def add_signing_key_to_project(
-    context: AuthedServiceContext, project: Project
-) -> Union[Project, SyftError]:
-    # Automatically infuse signing key of user
-    # requesting get_all() or creating the project object
-
-    user_service = context.node.get_service(UserService)
-    user = user_service.stash.get_by_verify_key(
-        credentials=context.credentials, verify_key=context.credentials
+    @service_method(
+        path="project.get_by_uid",
+        name="get_by_uid",
+        roles=GUEST_ROLE_LEVEL,
     )
-    if user.is_err():
-        return SyftError(message=str(user.err()))
+    def get_by_uid(self, context: AuthedServiceContext, uid: UID):
+        result = self.stash.get_by_uid(
+            credentials=context.node.verify_key,
+            uid=uid,
+        )
+        if result.is_err():
+            return SyftError(message=str(result.err()))
+        elif result.ok():
+            return result.ok()
+        return SyftError(message=f'Project(id="{uid}") does not exist')
+
+    def add_signing_key_to_project(
+        self, context: AuthedServiceContext, project: Project
+    ) -> Union[Project, SyftError]:
+        # Automatically infuse signing key of user
+        # requesting get_all() or creating the project object
+
+        user_service = context.node.get_service("userservice")
+        user = user_service.stash.get_by_verify_key(
+            credentials=context.credentials, verify_key=context.credentials
+        )
+        if user.is_err():
+            return SyftError(message=str(user.err()))
+
+        user = user.ok()
+        if not user:
+            return SyftError(message="User not found! Kindly register user first")
+
+        project.user_signing_key = user.signing_key
+
+        return project
 
-    user = user.ok()
-    if not user:
-        return SyftError(message="User not found! Kindly register user first")
-
-    project.user_signing_key = user.signing_key
-
-    return project
-
-
-def check_for_project_request(
-    project: Project, project_event: ProjectEvent, context: AuthedServiceContext
-):
-    """To check for project request event and create a message for the root user
-
-    Args:
-        project (Project): Project object
-        project_event (ProjectEvent): Project event object
-        context (AuthedServiceContext): Context of the node
-
-    Returns:
-        Union[SyftSuccess, SyftError]: SyftSuccess if message is created else SyftError
-    """
-    if (
-        isinstance(project_event, ProjectRequest)
-        and project_event.request.node_uid == context.node.id
+    def check_for_project_request(
+        self,
+        project: Project,
+        project_event: ProjectEvent,
+        context: AuthedServiceContext,
     ):
-        link = LinkedObject.with_context(project, context=context)
-        message = CreateMessage(
-            subject="Project Approval",
-            from_user_verify_key=context.credentials,
-            to_user_verify_key=context.node.verify_key,
-            linked_obj=link,
-        )
-        method = context.node.get_service_method(MessageService.send)
-        result = method(context=context, message=message)
-        if isinstance(result, SyftError):
-            return result
-    return SyftSuccess(message="Successfully Validated Project Request")
+        """To check for project request event and create a message for the root user
+
+        Args:
+            project (Project): Project object
+            project_event (ProjectEvent): Project event object
+            context (AuthedServiceContext): Context of the node
+
+        Returns:
+            Union[SyftSuccess, SyftError]: SyftSuccess if message is created else SyftError
+        """
+        if (
+            isinstance(project_event, ProjectRequest)
+            and project_event.linked_request.node_uid == context.node.id
+        ):
+            link = LinkedObject.with_context(project, context=context)
+            message = CreateMessage(
+                subject=f"A new request has been added to the Project: {project.name}.",
+                from_user_verify_key=context.credentials,
+                to_user_verify_key=context.node.verify_key,
+                linked_obj=link,
+            )
+            method = context.node.get_service_method(MessageService.send)
+            result = method(context=context, message=message)
+            if isinstance(result, SyftError):
+                return result
+        return SyftSuccess(message="Successfully Validated Project Request")
 
 
 TYPE_TO_SERVICE[Project] = ProjectService
 SERVICE_TO_TYPES[ProjectService].update({Project})
```

### Comparing `syft-0.8.1b6/src/syft/service/project/project_stash.py` & `syft-0.8.1b7/src/syft/service/project/project_stash.py`

 * *Files 12% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 from ...types.uid import UID
 from ...util.telemetry import instrument
 from ..request.request import Request
 from ..response import SyftError
 from .project import Project
 
 VerifyKeyPartitionKey = PartitionKey(key="user_verify_key", type_=SyftVerifyKey)
-OrderByNamePartitionKey = PartitionKey(key="name", type_=str)
+NamePartitionKey = PartitionKey(key="name", type_=str)
 
 
 @instrument
 @serializable()
 class ProjectStash(BaseUIDStoreStash):
     object_type = Project
     settings: PartitionSettings = PartitionSettings(
@@ -36,15 +36,20 @@
     ) -> Result[List[Request], SyftError]:
         if isinstance(verify_key, str):
             verify_key = SyftVerifyKey.from_string(verify_key)
         qks = QueryKeys(qks=[VerifyKeyPartitionKey.with_obj(verify_key)])
         return self.query_all(
             credentials=credentials,
             qks=qks,
-            order_by=OrderByNamePartitionKey,
         )
 
     def get_by_uid(
         self, credentials: SyftVerifyKey, uid: UID
     ) -> Result[Optional[Project], str]:
         qks = QueryKeys(qks=[UIDPartitionKey.with_obj(uid)])
         return self.query_one(credentials=credentials, qks=qks)
+
+    def get_by_name(
+        self, credentials: SyftVerifyKey, project_name: str
+    ) -> Result[Optional[Project], str]:
+        qks = QueryKeys(qks=[NamePartitionKey.with_obj(project_name)])
+        return self.query_one(credentials=credentials, qks=qks)
```

### Comparing `syft-0.8.1b6/src/syft/service/queue/base_queue.py` & `syft-0.8.1b7/src/syft/service/queue/base_queue.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.1b6/src/syft/service/queue/queue.py` & `syft-0.8.1b7/src/syft/service/queue/queue.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.1b6/src/syft/service/queue/queue_stash.py` & `syft-0.8.1b7/src/syft/service/queue/queue_stash.py`

 * *Files 2% similar despite different names*

```diff
@@ -45,15 +45,18 @@
     id: UID
     node_uid: UID
     result: Optional[Any]
     resolved: bool = False
     status: Status = Status.CREATED
 
     def fetch(self) -> None:
-        api = APIRegistry.api_for(node_uid=self.node_uid)
+        api = APIRegistry.api_for(
+            node_uid=self.node_uid,
+            user_verify_key=self.syft_client_verify_key,
+        )
         call = SyftAPICall(
             node_uid=self.node_uid,
             path="queue",
             args=[],
             kwargs={"uid": self.id},
             blocking=True,
         )
```

### Comparing `syft-0.8.1b6/src/syft/service/queue/zmq_queue.py` & `syft-0.8.1b7/src/syft/service/queue/zmq_queue.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.1b6/src/syft/service/request/request.py` & `syft-0.8.1b7/src/syft/service/request/request.py`

 * *Files 16% similar despite different names*

```diff
@@ -27,24 +27,27 @@
 from ...types.syft_object import SyftObject
 from ...types.transforms import TransformContext
 from ...types.transforms import add_node_uid_for_key
 from ...types.transforms import generate_id
 from ...types.transforms import transform
 from ...types.uid import LineageID
 from ...types.uid import UID
+from ...util.markdown import markdown_as_class_with_fields
 from ..action.action_object import ActionObject
 from ..action.action_service import ActionService
 from ..action.action_store import ActionObjectPermission
 from ..action.action_store import ActionPermission
 from ..code.user_code import UserCode
 from ..code.user_code import UserCodeStatus
 from ..context import AuthedServiceContext
 from ..context import ChangeContext
+from ..message.messages import Message
 from ..response import SyftError
 from ..response import SyftSuccess
+from ..user.user import UserView
 
 
 @serializable()
 class RequestStatus(Enum):
     PENDING = 0
     REJECTED = 1
     APPROVED = 2
@@ -58,14 +61,28 @@
     linked_obj: Optional[LinkedObject]
 
     def is_type(self, type_: type) -> bool:
         return self.linked_obj and type_ == self.linked_obj.object_type
 
 
 @serializable()
+class ChangeStatus(SyftObject):
+    __canonical_name__ = "ChangeStatus"
+    __version__ = SYFT_OBJECT_VERSION_1
+
+    id: Optional[UID]
+    change_id: UID
+    applied: bool = False
+
+    @classmethod
+    def from_change(cls, change: Change, applied: bool) -> Self:
+        return cls(change_id=change.id, applied=applied)
+
+
+@serializable()
 class ActionStoreChange(Change):
     __canonical_name__ = "ActionStoreChange"
     __version__ = SYFT_OBJECT_VERSION_1
 
     linked_obj: LinkedObject
     apply_permission_type: ActionPermission
 
@@ -120,115 +137,197 @@
     __canonical_name__ = "Request"
     __version__ = SYFT_OBJECT_VERSION_1
 
     requesting_user_verify_key: SyftVerifyKey
     approving_user_verify_key: Optional[SyftVerifyKey]
     request_time: DateTime
     approval_time: Optional[DateTime]
-    status: RequestStatus = RequestStatus.PENDING
     node_uid: UID
     request_hash: str
     changes: List[Change]
+    history: List[ChangeStatus] = []
 
     __attr_searchable__ = [
         "requesting_user_verify_key",
         "approving_user_verify_key",
-        "status",
     ]
     __attr_unique__ = ["request_hash"]
-    __attr_repr_cols__ = ["request_time", "status", "changes"]
+    __attr_repr_cols__ = [
+        "request_time",
+        "approval_time",
+        "status",
+        "changes",
+        "requesting_user_verify_key",
+    ]
+
+    @property
+    def status(self) -> RequestStatus:
+        if len(self.history) == 0:
+            return RequestStatus.PENDING
+
+        change_applied_map = {}
+        for change_status in self.history:
+            # only store the last change
+            change_applied_map[change_status.id] = change_status.applied
+
+        all_changes_applied = all(change_applied_map.values()) and (
+            len(change_applied_map) == len(self.changes)
+        )
+
+        request_status = (
+            RequestStatus.APPROVED if all_changes_applied else RequestStatus.REJECTED
+        )
+
+        return request_status
 
     def approve(self):
-        api = APIRegistry.api_for(self.node_uid)
+        api = APIRegistry.api_for(
+            self.node_uid,
+            self.syft_client_verify_key,
+        )
         return api.services.request.apply(self.id)
 
     def approve_with_client(self, client):
         return client.api.services.request.apply(self.id)
 
     def apply(self, context: AuthedServiceContext) -> Result[SyftSuccess, SyftError]:
         change_context = ChangeContext.from_service(context)
         change_context.requesting_user_credentials = self.requesting_user_verify_key
         for change in self.changes:
+            # by default change status is not applied
+            change_status = ChangeStatus(change_id=change.id, applied=False)
             result = change.apply(context=change_context)
             if result.is_err():
+                # add to history and save history to request
+                self.history.append(change_status)
+                self.save(context=context)
                 return result
+
+            # If no error, then change successfully applied.
+            change_status.applied = True
+            self.history.append(change_status)
+
+        self.save(context=context)
         return Ok(SyftSuccess(message=f"Request {self.id} changes applied"))
 
+    def save(self, context: AuthedServiceContext) -> Result[SyftSuccess, SyftError]:
+        # relative
+        from .request_service import RequestService
+
+        save_method = context.node.get_service_method(RequestService.save)
+        return save_method(context=context, request=self)
+
     def revert(self, context: AuthedServiceContext) -> Result[SyftSuccess, SyftError]:
         change_context = ChangeContext.from_service(context)
         change_context.requesting_user_credentials = self.requesting_user_verify_key
         for change in self.changes:
             result = change.revert(context=change_context)
             if result.is_err():
                 return result
         return Ok(SyftSuccess(message=f"Request {self.id} changes reverted"))
 
-    def accept_by_depositing_result(self, result: Any):
+    def accept_by_depositing_result(self, result: Any, force: bool = False):
         # this code is extremely brittle because its a work around that relies on
         # the type of request being very specifically tied to code which needs approving
         change = self.changes[0]
         if not change.is_type(UserCode):
             raise Exception(
                 f"accept_by_depositing_result can only be run on {UserCode} not "
                 f"{change.linked_obj.object_type}"
             )
         if not type(change) == UserCodeStatusChange:
             raise Exception(
                 f"accept_by_depositing_result can only be run on {UserCodeStatusChange} not "
                 f"{type(change)}"
             )
 
-        api = APIRegistry.api_for(self.node_uid)
+        api = APIRegistry.api_for(self.node_uid, self.syft_client_verify_key)
         if not api:
             raise Exception(f"Login to {self.node_uid} first.")
 
-        action_object = ActionObject.from_obj(result)
-
-        result = api.services.action.save(action_object)
-        if not result:
-            return result
+        is_approved = change.approved
 
         permission_request = self.approve()
         if not permission_request:
             return permission_request
 
         code = change.linked_obj.resolve
         state = code.output_policy
-        ctx = AuthedServiceContext(credentials=api.signing_key.verify_key)
 
-        state.apply_output(context=ctx, outputs=action_object)
-        policy_state_mutation = ObjectMutation(
-            linked_obj=change.linked_obj,
-            attr_name="output_policy",
-            match_type=True,
-            value=state,
-        )
+        # This weird order is due to the fact that state is None before calling approve
+        # we could fix it in a future release
+        if is_approved:
+            if not force:
+                return SyftError(
+                    message="Already approved, if you want to force updating the result use force=True"
+                )
+            action_obj_id = state.output_history[0].outputs[0]
+            action_object = ActionObject.from_obj(result, id=action_obj_id)
+            result = api.services.action.save(action_object)
+            if not result:
+                return result
+            return SyftSuccess(message="Request submitted for updating result.")
+        else:
+            action_object = ActionObject.from_obj(result)
+            result = api.services.action.save(action_object)
+            if not result:
+                return result
+            ctx = AuthedServiceContext(credentials=api.signing_key.verify_key)
 
-        action_object_link = LinkedObject.from_obj(
-            action_object, node_uid=self.node_uid
-        )
-        permission_change = ActionStoreChange(
-            linked_obj=action_object_link, apply_permission_type=ActionPermission.READ
-        )
+            state.apply_output(context=ctx, outputs=action_object)
+            policy_state_mutation = ObjectMutation(
+                linked_obj=change.linked_obj,
+                attr_name="output_policy",
+                match_type=True,
+                value=state,
+            )
+
+            action_object_link = LinkedObject.from_obj(
+                action_object, node_uid=self.node_uid
+            )
+            permission_change = ActionStoreChange(
+                linked_obj=action_object_link,
+                apply_permission_type=ActionPermission.READ,
+            )
+
+            submit_request = SubmitRequest(
+                changes=[policy_state_mutation, permission_change],
+                requesting_user_verify_key=self.requesting_user_verify_key,
+            )
+
+            self.approve()
+
+            new_request = api.services.request.submit(submit_request)
+            if not new_request:
+                return new_request
+            new_request_result = api.services.request.apply(new_request.id)
+            if not new_request_result:
+                return new_request_result
+            result = api.services.request.apply(self.id)
+            return result
+
+
+@serializable()
+class RequestInfo(SyftObject):
+    # version
+    __canonical_name__ = "RequestInfo"
+    __version__ = SYFT_OBJECT_VERSION_1
+
+    user: UserView
+    request: Request
+    message: Message
 
-        submit_request = SubmitRequest(
-            changes=[policy_state_mutation, permission_change],
-            requesting_user_verify_key=self.requesting_user_verify_key,
-        )
 
-        self.status = RequestStatus.APPROVED
+@serializable()
+class RequestInfoFilter(SyftObject):
+    # version
+    __canonical_name__ = "RequestInfoFilter"
+    __version__ = SYFT_OBJECT_VERSION_1
 
-        new_request = api.services.request.submit(submit_request)
-        if not new_request:
-            return new_request
-        new_request_result = api.services.request.apply(new_request.id)
-        if not new_request_result:
-            return new_request_result
-        result = api.services.request.apply(self.id)
-        return result
+    name: Optional[str]
 
 
 @serializable()
 class SubmitRequest(SyftObject):
     __canonical_name__ = "SubmitRequest"
     __version__ = SYFT_OBJECT_VERSION_1
 
@@ -343,35 +442,14 @@
 
     enum_type: Type[Enum]
     value: Optional[Enum]
     match_type: bool = True
 
     __attr_repr_cols__ = ["linked_obj", "attr_name", "value"]
 
-    def __init__(
-        self,
-        attr_name: str,
-        enum_type: Type[Enum],
-        match_type: bool = True,
-        linked_obj: Optional[LinkedObject] = None,
-        value: Optional[Enum] = None,
-        id: Optional[UID] = None,
-    ) -> None:
-        if id is None:
-            id = UID()
-
-        super().__init__(
-            id=id,
-            linked_obj=linked_obj,
-            attr_name=attr_name,
-            value=value,
-            enum_type=enum_type,
-            match_type=match_type,
-        )
-
     @property
     def valid(self) -> Union[SyftSuccess, SyftError]:
         if self.match_type and not isinstance(self.value, self.enum_type):
             return SyftError(
                 message=f"{type(self.value)} must be of type: {self.enum_type}"
             )
         return SyftSuccess(message=f"{type(self)} valid")
@@ -428,14 +506,44 @@
 class UserCodeStatusChange(Change):
     __canonical_name__ = "UserCodeStatusChange"
     __version__ = SYFT_OBJECT_VERSION_1
 
     value: UserCodeStatus
     linked_obj: LinkedObject
     match_type: bool = True
+    __attr_repr_cols__ = [
+        "link.service_func_name",
+        "link.input_policy_type.__canonical_name__",
+        "link.output_policy_type.__canonical_name__",
+        "link.status.approved",
+    ]
+
+    def _repr_markdown_(self) -> str:
+        link = self.link
+        input_policy_type = (
+            link.input_policy_type.__canonical_name__
+            if link.input_policy_type is not None
+            else None
+        )
+        output_policy_type = (
+            link.output_policy_type.__canonical_name__
+            if link.output_policy_type is not None
+            else None
+        )
+        repr_dict = {
+            "function": link.service_func_name,
+            "input_policy_type": f"{input_policy_type}",
+            "output_policy_type": f"{output_policy_type}",
+            "approved": f"{link.status.approved}",
+        }
+        return markdown_as_class_with_fields(self, repr_dict)
+
+    @property
+    def approved(self) -> bool:
+        return self.linked_obj.resolve.status.approved
 
     @property
     def valid(self) -> Union[SyftSuccess, SyftError]:
         if self.match_type and not isinstance(self.value, UserCodeStatus):
             return SyftError(
                 message=f"{type(self.value)} must be of type: {UserCodeStatus}"
             )
```

### Comparing `syft-0.8.1b6/src/syft/service/request/request_stash.py` & `syft-0.8.1b7/src/syft/service/request/request_stash.py`

 * *Files 11% similar despite different names*

```diff
@@ -10,20 +10,18 @@
 from ...store.document_store import BaseUIDStoreStash
 from ...store.document_store import PartitionKey
 from ...store.document_store import PartitionSettings
 from ...store.document_store import QueryKeys
 from ...types.datetime import DateTime
 from ...util.telemetry import instrument
 from .request import Request
-from .request import RequestStatus
 
 RequestingUserVerifyKeyPartitionKey = PartitionKey(
     key="requesting_user_verify_key", type_=SyftVerifyKey
 )
-StatusPartitionKey = PartitionKey(key="status", type_=RequestStatus)
 
 OrderByRequestTimeStampPartitionKey = PartitionKey(key="request_time", type_=DateTime)
 
 
 @instrument
 @serializable()
 class RequestStash(BaseUIDStoreStash):
@@ -41,17 +39,7 @@
             verify_key = SyftVerifyKey.from_string(verify_key)
         qks = QueryKeys(qks=[RequestingUserVerifyKeyPartitionKey.with_obj(verify_key)])
         return self.query_all(
             credentials=credentials,
             qks=qks,
             order_by=OrderByRequestTimeStampPartitionKey,
         )
-
-    def get_all_for_status(
-        self, credentials: SyftVerifyKey, status: RequestStatus
-    ) -> Result[List[Request], str]:
-        qks = QueryKeys(qks=[StatusPartitionKey.with_obj(status)])
-        return self.query_all(
-            credentials=credentials,
-            qks=qks,
-            order_by=OrderByRequestTimeStampPartitionKey,
-        )
```

### Comparing `syft-0.8.1b6/src/syft/service/response.py` & `syft-0.8.1b7/src/syft/service/response.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.1b6/src/syft/service/service.py` & `syft-0.8.1b7/src/syft/service/service.py`

 * *Files 3% similar despite different names*

```diff
@@ -29,14 +29,15 @@
 from ..serde.serializable import serializable
 from ..serde.signature import Signature
 from ..serde.signature import signature_remove_context
 from ..serde.signature import signature_remove_self
 from ..store.linked_obj import LinkedObject
 from ..types.syft_object import SyftBaseObject
 from ..types.syft_object import SyftObject
+from ..types.syft_object import attach_attribute_to_syft_object
 from ..types.uid import UID
 from .context import AuthedServiceContext
 from .context import ChangeContext
 from .response import SyftError
 from .user.user_roles import DATA_OWNER_ROLE_LEVEL
 from .user.user_roles import ServiceRole
 
@@ -327,15 +328,24 @@
             if autosplat is not None and len(autosplat) > 0:
                 args, kwargs = reconstruct_args_kwargs(
                     signature=input_signature,
                     autosplat=autosplat,
                     args=args,
                     kwargs=kwargs,
                 )
-            return func(self, *args, **kwargs)
+            result = func(self, *args, **kwargs)
+            context = kwargs.get("context", None)
+            context = args[0] if context is None else context
+            attrs_to_attach = {
+                "syft_node_location": context.node.id,
+                "syft_client_verify_key": context.credentials,
+            }
+            return attach_attribute_to_syft_object(
+                result=result, attr_dict=attrs_to_attach
+            )
 
         if autosplat is not None and len(autosplat) > 0:
             signature = expand_signature(signature=input_signature, autosplat=autosplat)
 
         config = ServiceConfig(
             public_path=_path if path is None else path,
             private_path=_path,
```

### Comparing `syft-0.8.1b6/src/syft/service/settings/settings.py` & `syft-0.8.1b7/src/syft/service/settings/settings.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.1b6/src/syft/service/settings/settings_service.py` & `syft-0.8.1b7/src/syft/service/settings/settings_service.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.1b6/src/syft/service/settings/settings_stash.py` & `syft-0.8.1b7/src/syft/service/settings/settings_stash.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.1b6/src/syft/service/user/user.py` & `syft-0.8.1b7/src/syft/service/user/user.py`

 * *Files 3% similar despite different names*

```diff
@@ -169,15 +169,16 @@
 @transform(UserCreate, User)
 def user_create_to_user() -> List[Callable]:
     return [
         generate_id,
         validate_email,
         hash_password,
         generate_key,
-        default_role(ServiceRole.GUEST),
+        # TODO: Fix this by passing it from client & verifying it at server
+        default_role(ServiceRole.DATA_SCIENTIST),
         drop(["password", "password_verify"]),
     ]
 
 
 @transform(User, UserView)
 def user_to_view_user() -> List[Callable]:
     return [keep(["id", "email", "name", "role", "institution", "website"])]
@@ -186,12 +187,13 @@
 @serializable()
 class UserPrivateKey(SyftObject):
     __canonical_name__ = "UserPrivateKey"
     __version__ = SYFT_OBJECT_VERSION_1
 
     email: str
     signing_key: SyftSigningKey
+    role: ServiceRole
 
 
 @transform(User, UserPrivateKey)
 def user_to_user_verify() -> List[Callable]:
-    return [keep(["email", "signing_key", "id"])]
+    return [keep(["email", "signing_key", "id", "role"])]
```

### Comparing `syft-0.8.1b6/src/syft/service/user/user_roles.py` & `syft-0.8.1b7/src/syft/service/user/user_roles.py`

 * *Files 2% similar despite different names*

```diff
@@ -90,14 +90,16 @@
     + ServiceRole.ADMIN
 )
 
 DATA_SCIENTIST_ROLE_LEVEL = ServiceRole.roles_for_level(
     ServiceRole.DATA_SCIENTIST + ServiceRole.DATA_OWNER + ServiceRole.ADMIN
 )
 
+ONLY_DATA_SCIENTIST_ROLE_LEVEL = ServiceRole.roles_for_level(ServiceRole.DATA_SCIENTIST)
+
 DATA_OWNER_ROLE_LEVEL = ServiceRole.roles_for_level(
     ServiceRole.DATA_OWNER + ServiceRole.ADMIN
 )
 
 ADMIN_ROLE_LEVEL = ServiceRole.roles_for_level(ServiceRole.ADMIN)
 
 ROLE_TO_CAPABILITIES = {
```

### Comparing `syft-0.8.1b6/src/syft/service/user/user_service.py` & `syft-0.8.1b7/src/syft/service/user/user_service.py`

 * *Files 2% similar despite different names*

```diff
@@ -205,15 +205,15 @@
                 return SyftError(
                     message=f"As a {context.role}, you are not allowed to edit {user.role} to {user_update.role}"
                 )
 
         edits_non_role_attrs = any(
             [
                 getattr(user_update, attr) is not Empty
-                for attr in dict(user_update)
+                for attr in user_update.dict()
                 if attr != "role"
             ]
         )
 
         if (
             edits_non_role_attrs
             and user.verify_key != context.credentials
@@ -358,10 +358,22 @@
         # we are bypassing permissions here, so dont use to return a result directly to the user
         credentials = self.admin_verify_key()
         result = self.stash.get_by_email(credentials=credentials, email=email)
         if result.is_ok():
             return result.ok().verify_key
         return SyftError(message=f"No user with email: {email}")
 
+    def get_by_verify_key(
+        self, verify_key: SyftVerifyKey
+    ) -> Union[UserView, SyftError]:
+        # we are bypassing permissions here, so dont use to return a result directly to the user
+        credentials = self.admin_verify_key()
+        result = self.stash.get_by_verify_key(
+            credentials=credentials, verify_key=verify_key
+        )
+        if result.is_ok():
+            return result.ok()
+        return SyftError(message=f"No User with verify_key: {verify_key}")
+
 
 TYPE_TO_SERVICE[User] = UserService
 SERVICE_TO_TYPES[UserService].update({User})
```

### Comparing `syft-0.8.1b6/src/syft/service/user/user_stash.py` & `syft-0.8.1b7/src/syft/service/user/user_stash.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.1b6/src/syft/service/vpn/headscale_client.py` & `syft-0.8.1b7/src/syft/service/vpn/headscale_client.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.1b6/src/syft/service/vpn/tailscale_client.py` & `syft-0.8.1b7/src/syft/service/vpn/tailscale_client.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.1b6/src/syft/service/vpn/vpn.py` & `syft-0.8.1b7/src/syft/service/vpn/vpn.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.1b6/src/syft/store/dict_document_store.py` & `syft-0.8.1b7/src/syft/store/dict_document_store.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.1b6/src/syft/store/document_store.py` & `syft-0.8.1b7/src/syft/store/document_store.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.1b6/src/syft/store/kv_document_store.py` & `syft-0.8.1b7/src/syft/store/kv_document_store.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.1b6/src/syft/store/linked_obj.py` & `syft-0.8.1b7/src/syft/store/linked_obj.py`

 * *Files 5% similar despite different names*

```diff
@@ -33,15 +33,18 @@
         return f"<{self.object_type}: {self.object_uid}@<Node: {self.node_uid}>"
 
     @property
     def resolve(self) -> SyftObject:
         # relative
         from ..client.api import APIRegistry
 
-        api = APIRegistry.api_for(node_uid=self.node_uid)
+        api = APIRegistry.api_for(
+            node_uid=self.node_uid,
+            user_verify_key=self.syft_client_verify_key,
+        )
         return api.services.messages.resolve_object(self)
 
     def resolve_with_context(self, context: NodeServiceContext) -> Any:
         return context.node.get_service(self.service_type).resolve_link(
             context=context, linked_obj=self
         )
 
@@ -88,14 +91,15 @@
                 raise Exception(f"{cls} Requires an object UID")
 
         return LinkedObject(
             node_uid=node_uid,
             service_type=service_type,
             object_type=type(obj),
             object_uid=object_uid,
+            syft_client_verify_key=obj.syft_client_verify_key,
         )
 
     @classmethod
     def with_context(
         cls,
         obj: SyftObject,
         context: NodeServiceContext,
```

### Comparing `syft-0.8.1b6/src/syft/store/locks.py` & `syft-0.8.1b7/src/syft/store/locks.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.1b6/src/syft/store/mongo_client.py` & `syft-0.8.1b7/src/syft/store/mongo_client.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.1b6/src/syft/store/mongo_codecs.py` & `syft-0.8.1b7/src/syft/store/mongo_codecs.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.1b6/src/syft/store/mongo_document_store.py` & `syft-0.8.1b7/src/syft/store/mongo_document_store.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.1b6/src/syft/store/sqlite_document_store.py` & `syft-0.8.1b7/src/syft/store/sqlite_document_store.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.1b6/src/syft/types/datetime.py` & `syft-0.8.1b7/src/syft/types/datetime.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.1b6/src/syft/types/grid_url.py` & `syft-0.8.1b7/src/syft/types/grid_url.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.1b6/src/syft/types/syft_metaclass.py` & `syft-0.8.1b7/src/syft/types/syft_metaclass.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.1b6/src/syft/types/syft_object.py` & `syft-0.8.1b7/src/syft/types/syft_object.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,61 +1,113 @@
 # stdlib
 from collections import defaultdict
+from collections.abc import Set
 from hashlib import sha256
 import inspect
 from inspect import Signature
+import re
 import types
 from typing import Any
 from typing import Callable
 from typing import ClassVar
 from typing import Dict
 from typing import KeysView
 from typing import List
+from typing import Mapping
 from typing import Optional
 from typing import Sequence
 from typing import Tuple
 from typing import Type
+from typing import Union
 import warnings
 
 # third party
+import itables
 import pydantic
 from pydantic import BaseModel
 from pydantic import EmailStr
 from pydantic.fields import Undefined
+from result import OkErr
 from typeguard import check_type
 
 # relative
 from ..node.credentials import SyftVerifyKey
 from ..serde.deserialize import _deserialize as deserialize
 from ..serde.recursive_primitives import recursive_serde_register_type
 from ..serde.serialize import _serialize as serialize
 from ..util.autoreload import autoreload_enabled
+from ..util.markdown import as_markdown_python_code
 from ..util.util import aggressive_set_attr
 from ..util.util import full_name_with_qualname
 from ..util.util import get_qualname_for
 from .syft_metaclass import Empty
 from .syft_metaclass import PartialModelMetaclass
 from .uid import UID
 
+IntStr = Union[int, str]
+AbstractSetIntStr = Set[IntStr]
+MappingIntStrAny = Mapping[IntStr, Any]
+
+
 SYFT_OBJECT_VERSION_1 = 1
 SYFT_OBJECT_VERSION_2 = 2
 
 supported_object_versions = [SYFT_OBJECT_VERSION_1, SYFT_OBJECT_VERSION_2]
 
 HIGHEST_SYFT_OBJECT_VERSION = max(supported_object_versions)
 LOWEST_SYFT_OBJECT_VERSION = min(supported_object_versions)
 
 
-class SyftBaseObject(BaseModel):
+# These attributes are dynamically added based on node/client
+# that is interaction with the SyftObject
+DYNAMIC_SYFT_ATTRIBUTES = [
+    "syft_node_location",
+    "syft_client_verify_key",
+]
+
+SURFACE_DARK_BRIGHT = "#464158"
+SURFACE_SURFACE = "#2E2B3B"
+DK_ON_SURFACE_HIGHEST = "#534F64"
+
+# This can be customize however we want
+itables_css = f"""
+.itables table {{
+    margin: 0 auto;
+    float: left;
+    color: {DK_ON_SURFACE_HIGHEST};
+}}
+.itables table th {{color: {SURFACE_SURFACE};}}
+"""
+
+
+class SyftHashableObject:
+    __hash_exclude_attrs__ = []
+
+    def __hash__(self) -> int:
+        return int.from_bytes(self.__sha256__(), byteorder="big")
+
+    def __sha256__(self) -> bytes:
+        self.__hash_exclude_attrs__.extend(DYNAMIC_SYFT_ATTRIBUTES)
+        _bytes = serialize(self, to_bytes=True, for_hashing=True)
+        return sha256(_bytes).digest()
+
+    def hash(self) -> str:
+        return self.__sha256__().hex()
+
+
+class SyftBaseObject(BaseModel, SyftHashableObject):
     class Config:
         arbitrary_types_allowed = True
 
     __canonical_name__: str  # the name which doesn't change even when there are multiple classes
     __version__: int  # data is always versioned
 
+    syft_node_location: Optional[UID]
+    syft_client_verify_key: Optional[SyftVerifyKey]
+
 
 class Context(SyftBaseObject):
     pass
 
 
 class SyftObjectRegistry:
     __object_version_registry__: Dict[str, Type["SyftObject"]] = {}
@@ -136,29 +188,15 @@
             f"the registry: {cls.__object_transform_registry__.keys()}"
         )
 
 
 print_type_cache = defaultdict(list)
 
 
-class SyftHashableObject:
-    __hash_exclude_attrs__ = []
-
-    def __hash__(self) -> int:
-        return int.from_bytes(self.__sha256__(), byteorder="big")
-
-    def __sha256__(self) -> bytes:
-        _bytes = serialize(self, to_bytes=True, for_hashing=True)
-        return sha256(_bytes).digest()
-
-    def hash(self) -> str:
-        return self.__sha256__().hex()
-
-
-class SyftObject(SyftBaseObject, SyftObjectRegistry, SyftHashableObject):
+class SyftObject(SyftBaseObject, SyftObjectRegistry):
     __canonical_name__ = "SyftObject"
     __version__ = SYFT_OBJECT_VERSION_1
 
     class Config:
         arbitrary_types_allowed = True
 
     # all objects have a UID
@@ -179,14 +217,17 @@
     # the unique keys for the particular Collection the objects will be stored in
     __serde_overrides__: Dict[
         str, Sequence[Callable]
     ] = {}  # List of attributes names which require a serde override.
     __owner__: str
 
     __attr_repr_cols__: ClassVar[List[str]] = []  # show these in html repr collections
+    __attr_custom_repr__: ClassVar[
+        List[str]
+    ] = None  # show these in html repr of an object
 
     def to_mongo(self) -> Dict[str, Any]:
         warnings.warn(
             "`SyftObject.to_mongo` is deprecated and will be removed in a future version",
             PendingDeprecationWarning,
         )
 
@@ -237,43 +278,65 @@
         return self.__repr__()
 
     def _repr_debug_(self) -> str:
         class_name = get_qualname_for(type(self))
         _repr_str = f"class {class_name}:\n"
         fields = getattr(self, "__fields__", {})
         for attr in fields.keys():
+            if attr in DYNAMIC_SYFT_ATTRIBUTES:
+                continue
             value = getattr(self, attr, "<Missing>")
             value_type = full_name_with_qualname(type(attr))
             value_type = value_type.replace("builtins.", "")
             value = f'"{value}"' if isinstance(value, str) else value
             _repr_str += f"  {attr}: {value_type} = {value}\n"
         return _repr_str
 
-    def _repr_markdown_(self) -> str:
+    def _repr_markdown_(self, wrap_as_python=True, indent=0) -> str:
+        s_indent = " " * indent * 2
         class_name = get_qualname_for(type(self))
-        _repr_str = f"class {class_name}:\n"
-        fields = getattr(self, "__fields__", {})
-        for attr in fields.keys():
-            value = getattr(self, attr, "<Missing>")
+        if self.__attr_custom_repr__ is not None:
+            fields = self.__attr_custom_repr__
+        elif self.__attr_repr_cols__ is not None:
+            fields = self.__attr_repr_cols__
+        else:
+            fields = list(getattr(self, "__fields__", {}).keys())
+
+        if "id" not in fields:
+            fields = ["id"] + fields
+
+        dynam_attrs = set(DYNAMIC_SYFT_ATTRIBUTES)
+        fields = [x for x in fields if x not in dynam_attrs]
+        _repr_str = f"{s_indent}class {class_name}:\n"
+        for attr in fields:
+            value = self
+            if getattr(value, attr, None) is None:
+                value = getattr(value, attr, "<Missing>")
+            else:
+                for _attr in attr.split("."):  # if compound string
+                    value = getattr(value, _attr, "<Missing>")
             value_type = full_name_with_qualname(type(attr))
             value_type = value_type.replace("builtins.", "")
             value = f'"{value}"' if isinstance(value, str) else value
-            _repr_str += f"  {attr}: {value_type} = {value}\n"
+            _repr_str += f"{s_indent}  {attr}: {value_type} = {value}\n"
 
         # _repr_str += "\n"
         # fqn = full_name_with_qualname(type(self))
         # _repr_str += f'fqn = "{fqn}"\n'
         # _repr_str += f"mro = {[t.__name__ for t in type(self).mro()]}"
 
         # _repr_str += "\n\ncallables = [\n"
         # for func, sig in self.__syft_get_funcs__():
         #     _repr_str += f"  {func}{sig}: pass\n"
         # _repr_str += f"]"
         # return _repr_str
-        return "```python\n" + _repr_str + "\n```"
+        if wrap_as_python:
+            return as_markdown_python_code(_repr_str)
+        else:
+            return _repr_str
 
     @staticmethod
     def from_mongo(bson: Any) -> "SyftObject":
         warnings.warn(
             "`SyftObject.from_mongo` is deprecated and will be removed in a future version",
             PendingDeprecationWarning,
         )
@@ -323,24 +386,53 @@
     ) -> Dict[str, Any]:
         warnings.warn(
             "`SyftObject.to_dict` is deprecated and will be removed in a future version",
             PendingDeprecationWarning,
         )
         # 🟡 TODO 18: Remove to_dict and replace usage with transforms etc
         if not exclude_none and not exclude_empty:
-            return dict(self)
+            return self.dict()
         else:
             new_dict = {}
             for k, v in dict(self).items():
+                # exclude dynamically added syft attributes
+                if k in DYNAMIC_SYFT_ATTRIBUTES:
+                    continue
                 if exclude_empty and v is not Empty:
                     new_dict[k] = v
                 if exclude_none and v is not None:
                     new_dict[k] = v
             return new_dict
 
+    def dict(
+        self,
+        *,
+        include: Optional[Union["AbstractSetIntStr", "MappingIntStrAny"]] = None,
+        exclude: Optional[Union["AbstractSetIntStr", "MappingIntStrAny"]] = None,
+        by_alias: bool = False,
+        skip_defaults: Optional[bool] = None,
+        exclude_unset: bool = False,
+        exclude_defaults: bool = False,
+        exclude_none: bool = False,
+    ):
+        if exclude is None:
+            exclude = set()
+
+        for attr in DYNAMIC_SYFT_ATTRIBUTES:
+            exclude.add(attr)
+        return super().dict(
+            include=include,
+            exclude=exclude,
+            by_alias=by_alias,
+            skip_defaults=skip_defaults,
+            exclude_unset=exclude_unset,
+            exclude_defaults=exclude_defaults,
+            exclude_none=exclude_none,
+        )
+
     def __post_init__(self) -> None:
         pass
 
     def _syft_set_validate_private_attrs_(self, **kwargs):
         # Validate and set private attributes
         # https://github.com/pydantic/pydantic/issues/2105
         for attr, decl in self.__private_attributes__.items():
@@ -400,20 +492,42 @@
         return cls._syft_keys_types_dict("__attr_unique__")
 
     @classmethod
     def _syft_searchable_keys_dict(cls) -> Dict[str, type]:
         return cls._syft_keys_types_dict("__attr_searchable__")
 
 
+def short_qual_name(name: str) -> str:
+    # If the name is a qualname of formax a.b.c.d we will only get d
+    # otherwise this will leave it like it is
+    return name.split(".")[-1]
+
+
+def short_uid(uid: UID) -> str:
+    if uid is None:
+        return uid
+    else:
+        return str(uid)[:6] + "..."
+
+
 def list_dict_repr_html(self) -> str:
     try:
         max_check = 1
         items_checked = 0
         has_syft = False
         extra_fields = []
+        if isinstance(self, dict):
+            values = list(self.values())
+        else:
+            values = self
+
+        if len(values) == 0:
+            return self.__repr__()
+
+        is_homogenous = len(set([type(x) for x in values])) == 1
         for item in iter(self):
             items_checked += 1
             if items_checked > max_check:
                 break
             if isinstance(self, dict):
                 item = self.__getitem__(item)
 
@@ -429,39 +543,83 @@
                 extra_fields = getattr(item, "__attr_repr_cols__", [])
                 break
         if has_syft:
             # third party
             import pandas as pd
 
             cols = defaultdict(list)
-            max_lines = 5
+            # max_lines = 5
             line = 0
             for item in iter(self):
                 line += 1
-                if line > max_lines:
-                    break
+                # if line > max_lines:
+                #     break
                 if isinstance(self, dict):
                     cols["key"].append(item)
                     item = self.__getitem__(item)
 
+                # get id
+                id_ = getattr(item, "id", None)
+                if id is not None:
+                    id_ = f"{str(id_)[:4]}...{str(id_)[-3:]}"
+
                 if type(item) == type:
-                    cols["type"].append(full_name_with_qualname(item))
+                    t = full_name_with_qualname(item)
                 else:
-                    cols["type"].append(item.__repr__())
+                    try:
+                        t = item.__class__.__name__
+                    except Exception:
+                        t = item.__repr__()
+                cols["id"].append(id_)
+                if not is_homogenous:
+                    cols["type"].append(t)
 
-                cols["id"].append(getattr(item, "id", None))
                 for field in extra_fields:
-                    value = getattr(item, field, None)
+                    value = item
+                    try:
+                        attrs = field.split(".")
+                        for attr in attrs:
+                            # find indexing like abc[1]
+                            res = re.search("\[[+-]?\d+\]", attr)
+                            has_index = False
+                            if res:
+                                has_index = True
+                                index_str = res.group()
+                                index = int(index_str.replace("[", "").replace("]", ""))
+                                attr = attr.replace(index_str, "")
+
+                            value = getattr(value, attr, None)
+                            if isinstance(value, list) and has_index:
+                                value = value[index]
+                    except Exception as e:
+                        print(e)
+                        value = None
                     cols[field].append(value)
 
-            x = pd.DataFrame(cols)
-            collection_type = (
-                f"{type(self).__name__.capitalize()} - Size: {len(self)}\n"
-            )
-            return collection_type + x._repr_html_()
+            df = pd.DataFrame(cols)
+
+            if is_homogenous:
+                cls_name = values[0].__class__.__name__
+            else:
+                cls_name = ""
+
+            html_header = f"""
+                <style>
+                .collection-header {{color: {SURFACE_DARK_BRIGHT};}}
+                </style>
+                <div class='collection-header'>
+                    <h3>{cls_name} {self.__class__.__name__.capitalize()}</h3>
+                </div>
+                <br>
+                """
+
+            html_datatable = itables.to_html_datatable(df=df, css=itables_css)
+
+            return html_header + html_datatable
+            # return collection_type + df_styled._repr_html_()
     except Exception as e:
         print(e)
         pass
 
     # stdlib
     import html
 
@@ -524,7 +682,49 @@
 
         empty_fields = unset_fields - fields_with_default
         for field_name in empty_fields:
             self.__dict__[field_name] = Empty
 
 
 recursive_serde_register_type(PartialSyftObject)
+
+
+def attach_attribute_to_syft_object(result: Any, attr_dict: Dict[str, Any]) -> Any:
+    box_to_result_type = None
+
+    if type(result) in OkErr:
+        box_to_result_type = type(result)
+        result = result.value
+
+    single_entity = False
+    is_tuple = isinstance(result, tuple)
+
+    if isinstance(result, (list, tuple)):
+        iterable_keys = range(len(result))
+        result = list(result)
+    elif isinstance(result, dict):
+        iterable_keys = result.keys()
+    else:
+        iterable_keys = range(1)
+        result = [result]
+        single_entity = True
+
+    for key in iterable_keys:
+        _object = result[key]
+        # if object is SyftBaseObject,
+        # then attach the value to the attribute
+        # on the object
+        if isinstance(_object, SyftBaseObject):
+            for attr_name, attr_value in attr_dict.items():
+                setattr(_object, attr_name, attr_value)
+
+            for field_name, attr in _object.__dict__.items():
+                updated_attr = attach_attribute_to_syft_object(attr, attr_dict)
+                setattr(_object, field_name, updated_attr)
+        result[key] = _object
+
+    wrapped_result = result[0] if single_entity else result
+    wrapped_result = tuple(wrapped_result) if is_tuple else wrapped_result
+    if box_to_result_type is not None:
+        wrapped_result = box_to_result_type(wrapped_result)
+
+    return wrapped_result
```

### Comparing `syft-0.8.1b6/src/syft/types/transforms.py` & `syft-0.8.1b7/src/syft/types/transforms.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.1b6/src/syft/types/uid.py` & `syft-0.8.1b7/src/syft/types/uid.py`

 * *Files 2% similar despite different names*

```diff
@@ -169,22 +169,22 @@
             part, end = part[:-chunk], part[-chunk:]
             output.append(self.char_emoji(hex_chars=end))
         return "".join(output)
 
     def emoji(self) -> str:
         return f"<UID:{self.string_emoji(string=str(self.value), length=8, chunk=4)}>"
 
-    def repr_short(self) -> str:
+    def short(self) -> str:
         """Returns a SHORT human-readable version of the ID
 
         Return a SHORT human-readable version of the ID which
         makes it print nicer when embedded (often alongside other
         UID objects) within other object __repr__ methods."""
 
-        return f"..{str(self.value)[-5:]}"
+        return str(self.value)[:8]
 
     @property
     def id(self) -> "UID":
         return self
 
     @staticmethod
     def _check_or_convert(value: Union[str, "UID", uuid.UUID]) -> "UID":
```

### Comparing `syft-0.8.1b6/src/syft/util/autoreload.py` & `syft-0.8.1b7/src/syft/util/autoreload.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.1b6/src/syft/util/decorators.py` & `syft-0.8.1b7/src/syft/util/decorators.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.1b6/src/syft/util/experimental_flags.py` & `syft-0.8.1b7/src/syft/util/experimental_flags.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.1b6/src/syft/util/filterwarnings.py` & `syft-0.8.1b7/src/syft/util/filterwarnings.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.1b6/src/syft/util/logger.py` & `syft-0.8.1b7/src/syft/util/logger.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.1b6/src/syft/util/schema.py` & `syft-0.8.1b7/src/syft/util/schema.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.1b6/src/syft/util/telemetry.py` & `syft-0.8.1b7/src/syft/util/telemetry.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.1b6/src/syft/util/trace_decorator.py` & `syft-0.8.1b7/src/syft/util/trace_decorator.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.1b6/src/syft/util/util.py` & `syft-0.8.1b7/src/syft/util/util.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.1b6/src/syft/util/version_compare.py` & `syft-0.8.1b7/src/syft/util/version_compare.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.1b6/src/syft.egg-info/PKG-INFO` & `syft-0.8.1b7/src/syft.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: syft
-Version: 0.8.1b6
+Version: 0.8.1b7
 Summary: Perform numpy-like analysis on data that remains in someone elses server
 Home-page: https://openmined.github.io/PySyft/
 Author: OpenMined
 Author-email: info@openmined.org
 License: Apache-2.0
 Project-URL: Source, https://github.com/OpenMined/PySyft
 Project-URL: Tracker, https://github.com/OpenMined/PySyft/issues
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: syft Version: 0.8.1b6 Summary: Perform numpy-like
+Metadata-Version: 2.1 Name: syft Version: 0.8.1b7 Summary: Perform numpy-like
 analysis on data that remains in someone elses server Home-page: https://
 openmined.github.io/PySyft/ Author: OpenMined Author-email: info@openmined.org
 License: Apache-2.0 Project-URL: Source, https://github.com/OpenMined/PySyft
 Project-URL: Tracker, https://github.com/OpenMined/PySyft/issues Platform: any
 Classifier: Development Status :: 4 - Beta Classifier: Programming Language ::
 Python Requires-Python: >=3.9 Description-Content-Type: text/markdown;
 charset=UTF-8; variant=GFM Provides-Extra: dev Provides-Extra: test_plugins
```

### Comparing `syft-0.8.1b6/src/syft.egg-info/SOURCES.txt` & `syft-0.8.1b7/src/syft.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -153,12 +153,13 @@
 src/syft/util/__init__.py
 src/syft/util/autoreload.py
 src/syft/util/decorators.py
 src/syft/util/experimental_flags.py
 src/syft/util/filterwarnings.py
 src/syft/util/jax_settings.py
 src/syft/util/logger.py
+src/syft/util/markdown.py
 src/syft/util/schema.py
 src/syft/util/telemetry.py
 src/syft/util/trace_decorator.py
 src/syft/util/util.py
 src/syft/util/version_compare.py
```

### Comparing `syft-0.8.1b6/src/syft.egg-info/requires.txt` & `syft-0.8.1b7/src/syft.egg-info/requires.txt`

 * *Files 20% similar despite different names*

```diff
@@ -26,14 +26,15 @@
 typing_extensions==4.5.0
 sherlock[filelock,redis]==0.4.1
 uvicorn[standard]==0.21.1
 fastapi==0.95.1
 hagrid>=0.3
 matplotlib==3.7.1
 dm-haiku==0.0.9
+itables==1.5.2
 opentelemetry-api==1.14.0
 opentelemetry-sdk==1.14.0
 opentelemetry-exporter-jaeger==1.14.0
 opentelemetry-instrumentation==0.35b0
 opentelemetry-instrumentation-requests==0.35b0
 
 [dev]
@@ -47,14 +48,15 @@
 pytest_mock_resources
 python_on_whales
 pytest-lazy-fixture
 pytest-rerunfailures
 coverage
 joblib
 faker
+lxml
 bandit==1.7.5
 ruff==0.0.254
 importlib-metadata==6.0.0
 isort==5.12.0
 mypy==1.1.1
 pre-commit==3.1.1
 safety==2.3.5
@@ -73,7 +75,8 @@
 pytest_mock_resources
 python_on_whales
 pytest-lazy-fixture
 pytest-rerunfailures
 coverage
 joblib
 faker
+lxml
```

