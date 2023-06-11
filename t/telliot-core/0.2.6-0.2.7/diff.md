# Comparing `tmp/telliot_core-0.2.6.tar.gz` & `tmp/telliot_core-0.2.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "telliot_core-0.2.6.tar", last modified: Fri Apr 28 18:30:06 2023, max compression
+gzip compressed data, was "telliot_core-0.2.7.tar", last modified: Sun Jun 11 15:37:28 2023, max compression
```

## Comparing `telliot_core-0.2.6.tar` & `telliot_core-0.2.7.tar`

### file list

```diff
@@ -1,163 +1,163 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 18:30:06.381533 telliot_core-0.2.6/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 18:30:06.349531 telliot_core-0.2.6/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 18:30:06.361531 telliot_core-0.2.6/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      716 2023-04-28 18:29:54.000000 telliot_core-0.2.6/.github/workflows/docs.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1194 2023-04-28 18:29:54.000000 telliot_core-0.2.6/.github/workflows/py39.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1305 2023-04-28 18:29:54.000000 telliot_core-0.2.6/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (123)      715 2023-04-28 18:29:54.000000 telliot_core-0.2.6/.github/workflows/style.yml
--rw-r--r--   0 runner    (1001) docker     (123)      719 2023-04-28 18:29:54.000000 telliot_core-0.2.6/.github/workflows/typing.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2382 2023-04-28 18:29:54.000000 telliot_core-0.2.6/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1095 2023-04-28 18:29:54.000000 telliot_core-0.2.6/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      665 2023-04-28 18:29:54.000000 telliot_core-0.2.6/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2159 2023-04-28 18:29:54.000000 telliot_core-0.2.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1892 2023-04-28 18:30:06.381533 telliot_core-0.2.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      974 2023-04-28 18:29:54.000000 telliot_core-0.2.6/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-04-28 18:29:54.000000 telliot_core-0.2.6/brownie-config.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 18:30:06.361531 telliot_core-0.2.6/contracts/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 18:30:06.361531 telliot_core-0.2.6/contracts/Integrations/
--rw-r--r--   0 runner    (1001) docker     (123)      183 2023-04-28 18:29:54.000000 telliot_core-0.2.6/contracts/Integrations/DIVAOracleMock.sol
--rw-r--r--   0 runner    (1001) docker     (123)     4315 2023-04-28 18:29:54.000000 telliot_core-0.2.6/contracts/Integrations/DIVAProtocolMock.sol
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-04-28 18:29:54.000000 telliot_core-0.2.6/contracts/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 18:30:06.361531 telliot_core-0.2.6/contracts/TellorFlex/
--rw-r--r--   0 runner    (1001) docker     (123)      199 2023-04-28 18:29:54.000000 telliot_core-0.2.6/contracts/TellorFlex/AutopayMock.sol
--rw-r--r--   0 runner    (1001) docker     (123)    20244 2023-04-28 18:29:54.000000 telliot_core-0.2.6/contracts/TellorFlex/TellorFlex.sol
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 18:30:06.361531 telliot_core-0.2.6/contracts/TellorFlex/testing/
--rw-r--r--   0 runner    (1001) docker     (123)      317 2023-04-28 18:29:54.000000 telliot_core-0.2.6/contracts/TellorFlex/testing/StakingToken.sol
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 18:30:06.361531 telliot_core-0.2.6/contracts/TellorX/
--rw-r--r--   0 runner    (1001) docker     (123)      650 2023-04-28 18:29:54.000000 telliot_core-0.2.6/contracts/TellorX/TellorXMasterMock.sol
--rw-r--r--   0 runner    (1001) docker     (123)      949 2023-04-28 18:29:54.000000 telliot_core-0.2.6/contracts/TellorX/TellorXOracleMock.sol
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 18:30:06.365532 telliot_core-0.2.6/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      773 2023-04-28 18:29:54.000000 telliot_core-0.2.6/docs/add-chain.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 18:30:06.365532 telliot_core-0.2.6/docs/assets/
--rw-r--r--   0 runner    (1001) docker     (123)     1722 2023-04-28 18:29:54.000000 telliot_core-0.2.6/docs/assets/favicon-32x32.png
--rw-r--r--   0 runner    (1001) docker     (123)   160315 2023-04-28 18:29:54.000000 telliot_core-0.2.6/docs/assets/tellor_swoosh.png
--rw-r--r--   0 runner    (1001) docker     (123)     3134 2023-04-28 18:29:54.000000 telliot_core-0.2.6/docs/contributing.md
--rw-r--r--   0 runner    (1001) docker     (123)      693 2023-04-28 18:29:54.000000 telliot_core-0.2.6/docs/documentation.md
--rw-r--r--   0 runner    (1001) docker     (123)      219 2023-04-28 18:29:54.000000 telliot_core-0.2.6/docs/index.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 18:30:06.365532 telliot_core-0.2.6/interfaces/
--rw-r--r--   0 runner    (1001) docker     (123)      382 2023-04-28 18:29:54.000000 telliot_core-0.2.6/interfaces/IERC20.sol
--rw-r--r--   0 runner    (1001) docker     (123)     1561 2023-04-28 18:29:54.000000 telliot_core-0.2.6/mkdocs.yml
--rw-r--r--   0 runner    (1001) docker     (123)      377 2023-04-28 18:29:54.000000 telliot_core-0.2.6/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      152 2023-04-28 18:29:54.000000 telliot_core-0.2.6/requirements-dev.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 18:30:06.365532 telliot_core-0.2.6/scripts/
--rw-r--r--   0 runner    (1001) docker     (123)     1912 2023-04-28 18:29:54.000000 telliot_core-0.2.6/scripts/morphware_data_sizes.py
--rw-r--r--   0 runner    (1001) docker     (123)     7909 2023-04-28 18:29:54.000000 telliot_core-0.2.6/scripts/query_catalog.md
--rw-r--r--   0 runner    (1001) docker     (123)     2929 2023-04-28 18:29:54.000000 telliot_core-0.2.6/scripts/query_catalog.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1395 2023-04-28 18:30:06.385533 telliot_core-0.2.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-28 18:29:54.000000 telliot_core-0.2.6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 18:30:06.353531 telliot_core-0.2.6/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 18:30:06.365532 telliot_core-0.2.6/src/telliot_core/
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-28 18:29:54.000000 telliot_core-0.2.6/src/telliot_core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      146 2023-04-28 18:29:54.000000 telliot_core-0.2.6/src/telliot_core/api.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 18:30:06.369532 telliot_core-0.2.6/src/telliot_core/apps/
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-04-28 18:29:54.000000 telliot_core-0.2.6/src/telliot_core/apps/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1711 2023-04-28 18:29:54.000000 telliot_core-0.2.6/src/telliot_core/apps/app.py
--rw-r--r--   0 runner    (1001) docker     (123)     4328 2023-04-28 18:29:54.000000 telliot_core-0.2.6/src/telliot_core/apps/config.py
--rw-r--r--   0 runner    (1001) docker     (123)    11036 2023-04-28 18:29:54.000000 telliot_core-0.2.6/src/telliot_core/apps/core.py
--rw-r--r--   0 runner    (1001) docker     (123)     1700 2023-04-28 18:29:54.000000 telliot_core-0.2.6/src/telliot_core/apps/session_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     4398 2023-04-28 18:29:54.000000 telliot_core-0.2.6/src/telliot_core/apps/telliot_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-04-28 18:29:54.000000 telliot_core-0.2.6/src/telliot_core/asset_registry.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 18:30:06.369532 telliot_core-0.2.6/src/telliot_core/cli/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 18:29:54.000000 telliot_core-0.2.6/src/telliot_core/cli/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 18:30:06.369532 telliot_core-0.2.6/src/telliot_core/cli/commands/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 18:29:54.000000 telliot_core-0.2.6/src/telliot_core/cli/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1274 2023-04-28 18:29:54.000000 telliot_core-0.2.6/src/telliot_core/cli/commands/account.py
--rw-r--r--   0 runner    (1001) docker     (123)     1298 2023-04-28 18:29:54.000000 telliot_core-0.2.6/src/telliot_core/cli/commands/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     1532 2023-04-28 18:29:54.000000 telliot_core-0.2.6/src/telliot_core/cli/commands/listen.py
--rw-r--r--   0 runner    (1001) docker     (123)     2965 2023-04-28 18:29:54.000000 telliot_core-0.2.6/src/telliot_core/cli/commands/read.py
--rw-r--r--   0 runner    (1001) docker     (123)     1397 2023-04-28 18:29:54.000000 telliot_core-0.2.6/src/telliot_core/cli/main.py
--rw-r--r--   0 runner    (1001) docker     (123)     1195 2023-04-28 18:29:54.000000 telliot_core-0.2.6/src/telliot_core/cli/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 18:30:06.369532 telliot_core-0.2.6/src/telliot_core/contract/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 18:29:54.000000 telliot_core-0.2.6/src/telliot_core/contract/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8707 2023-04-28 18:29:54.000000 telliot_core-0.2.6/src/telliot_core/contract/contract.py
--rw-r--r--   0 runner    (1001) docker     (123)     9665 2023-04-28 18:29:54.000000 telliot_core-0.2.6/src/telliot_core/contract/listener.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 18:30:06.369532 telliot_core-0.2.6/src/telliot_core/data/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 18:29:54.000000 telliot_core-0.2.6/src/telliot_core/data/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 18:30:06.373532 telliot_core-0.2.6/src/telliot_core/data/abi/
--rw-r--r--   0 runner    (1001) docker     (123)     7513 2023-04-28 18:29:54.000000 telliot_core-0.2.6/src/telliot_core/data/abi/diva-oracle-tellor-abi.json
--rw-r--r--   0 runner    (1001) docker     (123)    28088 2023-04-28 18:29:54.000000 telliot_core-0.2.6/src/telliot_core/data/abi/diva-protocol-abi.json
--rw-r--r--   0 runner    (1001) docker     (123)     4935 2023-04-28 18:29:54.000000 telliot_core-0.2.6/src/telliot_core/data/abi/fuse-token-abi.json
--rw-r--r--   0 runner    (1001) docker     (123)    20737 2023-04-28 18:29:54.000000 telliot_core-0.2.6/src/telliot_core/data/abi/tellor-governance-abi.json
--rw-r--r--   0 runner    (1001) docker     (123)     4469 2023-04-28 18:29:54.000000 telliot_core-0.2.6/src/telliot_core/data/abi/tellor-mesosphere-abi.json
--rw-r--r--   0 runner    (1001) docker     (123)    35232 2023-04-28 18:29:54.000000 telliot_core-0.2.6/src/telliot_core/data/abi/tellor360-autopay-abi.json
--rw-r--r--   0 runner    (1001) docker     (123)    26675 2023-04-28 18:29:54.000000 telliot_core-0.2.6/src/telliot_core/data/abi/tellor360-oracle-abi.json
--rw-r--r--   0 runner    (1001) docker     (123)    21821 2023-04-28 18:29:54.000000 telliot_core-0.2.6/src/telliot_core/data/abi/tellor360-playground.json
--rw-r--r--   0 runner    (1001) docker     (123)    21041 2023-04-28 18:29:54.000000 telliot_core-0.2.6/src/telliot_core/data/abi/tellorflex-autopay-abi.json
--rw-r--r--   0 runner    (1001) docker     (123)    15025 2023-04-28 18:29:54.000000 telliot_core-0.2.6/src/telliot_core/data/abi/tellorflex-oracle-abi.json
--rw-r--r--   0 runner    (1001) docker     (123)    11824 2023-04-28 18:29:54.000000 telliot_core-0.2.6/src/telliot_core/data/abi/tellorx-governance-abi.json
--rw-r--r--   0 runner    (1001) docker     (123)     6670 2023-04-28 18:29:54.000000 telliot_core-0.2.6/src/telliot_core/data/abi/tellorx-lens-abi.json
--rw-r--r--   0 runner    (1001) docker     (123)    23746 2023-04-28 18:29:54.000000 telliot_core-0.2.6/src/telliot_core/data/abi/tellorx-master-abi.json
--rw-r--r--   0 runner    (1001) docker     (123)    11141 2023-04-28 18:29:54.000000 telliot_core-0.2.6/src/telliot_core/data/abi/tellorx-oracle-abi.json
--rw-r--r--   0 runner    (1001) docker     (123)     6681 2023-04-28 18:29:54.000000 telliot_core-0.2.6/src/telliot_core/data/abi/tellorx-treasury-abi.json
--rw-r--r--   0 runner    (1001) docker     (123)    13989 2023-04-28 18:29:54.000000 telliot_core-0.2.6/src/telliot_core/data/abi/trb-token-abi.json
--rw-r--r--   0 runner    (1001) docker     (123)     3274 2023-04-28 18:29:54.000000 telliot_core-0.2.6/src/telliot_core/data/assets.json
--rw-r--r--   0 runner    (1001) docker     (123)     9887 2023-04-28 18:29:54.000000 telliot_core-0.2.6/src/telliot_core/data/contract_directory.json
--rw-r--r--   0 runner    (1001) docker     (123)     5667 2023-04-28 18:29:54.000000 telliot_core-0.2.6/src/telliot_core/directory.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 18:30:06.373532 telliot_core-0.2.6/src/telliot_core/gas/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 18:29:54.000000 telliot_core-0.2.6/src/telliot_core/gas/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4547 2023-04-28 18:29:54.000000 telliot_core-0.2.6/src/telliot_core/gas/legacy_gas.py
--rw-r--r--   0 runner    (1001) docker     (123)     1384 2023-04-28 18:29:54.000000 telliot_core-0.2.6/src/telliot_core/logs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 18:30:06.373532 telliot_core-0.2.6/src/telliot_core/model/
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-04-28 18:29:54.000000 telliot_core-0.2.6/src/telliot_core/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1677 2023-04-28 18:29:54.000000 telliot_core-0.2.6/src/telliot_core/model/api_keys.py
--rw-r--r--   0 runner    (1001) docker     (123)      134 2023-04-28 18:29:54.000000 telliot_core-0.2.6/src/telliot_core/model/asset.py
--rw-r--r--   0 runner    (1001) docker     (123)      121 2023-04-28 18:29:54.000000 telliot_core-0.2.6/src/telliot_core/model/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     5006 2023-04-28 18:29:54.000000 telliot_core-0.2.6/src/telliot_core/model/chain.py
--rw-r--r--   0 runner    (1001) docker     (123)     8002 2023-04-28 18:29:54.000000 telliot_core-0.2.6/src/telliot_core/model/endpoints.py
--rw-r--r--   0 runner    (1001) docker     (123)      260 2023-04-28 18:29:54.000000 telliot_core-0.2.6/src/telliot_core/model/registry.py
--rw-r--r--   0 runner    (1001) docker     (123)     2086 2023-04-28 18:29:54.000000 telliot_core-0.2.6/src/telliot_core/model/tokens.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 18:30:06.373532 telliot_core-0.2.6/src/telliot_core/reporters/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 18:29:54.000000 telliot_core-0.2.6/src/telliot_core/reporters/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 18:30:06.373532 telliot_core-0.2.6/src/telliot_core/tellor/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 18:29:54.000000 telliot_core-0.2.6/src/telliot_core/tellor/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 18:30:06.373532 telliot_core-0.2.6/src/telliot_core/tellor/tellor360/
--rw-r--r--   0 runner    (1001) docker     (123)     1658 2023-04-28 18:29:54.000000 telliot_core-0.2.6/src/telliot_core/tellor/tellor360/autopay.py
--rw-r--r--   0 runner    (1001) docker     (123)     1344 2023-04-28 18:29:54.000000 telliot_core-0.2.6/src/telliot_core/tellor/tellor360/oracle.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 18:30:06.377532 telliot_core-0.2.6/src/telliot_core/tellor/tellorflex/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 18:29:54.000000 telliot_core-0.2.6/src/telliot_core/tellor/tellorflex/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2016 2023-04-28 18:29:54.000000 telliot_core-0.2.6/src/telliot_core/tellor/tellorflex/autopay.py
--rw-r--r--   0 runner    (1001) docker     (123)     3989 2023-04-28 18:29:54.000000 telliot_core-0.2.6/src/telliot_core/tellor/tellorflex/oracle.py
--rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-04-28 18:29:54.000000 telliot_core-0.2.6/src/telliot_core/tellor/tellorflex/token.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 18:30:06.377532 telliot_core-0.2.6/src/telliot_core/tellor/tellorx/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 18:29:54.000000 telliot_core-0.2.6/src/telliot_core/tellor/tellorx/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2591 2023-04-28 18:29:54.000000 telliot_core-0.2.6/src/telliot_core/tellor/tellorx/master.py
--rw-r--r--   0 runner    (1001) docker     (123)     4529 2023-04-28 18:29:54.000000 telliot_core-0.2.6/src/telliot_core/tellor/tellorx/oracle.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 18:30:06.377532 telliot_core-0.2.6/src/telliot_core/utils/
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-04-28 18:29:54.000000 telliot_core-0.2.6/src/telliot_core/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1248 2023-04-28 18:29:54.000000 telliot_core-0.2.6/src/telliot_core/utils/home.py
--rw-r--r--   0 runner    (1001) docker     (123)     1011 2023-04-28 18:29:54.000000 telliot_core-0.2.6/src/telliot_core/utils/key_helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)      222 2023-04-28 18:29:54.000000 telliot_core-0.2.6/src/telliot_core/utils/pyutils.py
--rw-r--r--   0 runner    (1001) docker     (123)      687 2023-04-28 18:29:54.000000 telliot_core-0.2.6/src/telliot_core/utils/response.py
--rw-r--r--   0 runner    (1001) docker     (123)     1094 2023-04-28 18:29:54.000000 telliot_core-0.2.6/src/telliot_core/utils/timestamp.py
--rw-r--r--   0 runner    (1001) docker     (123)      632 2023-04-28 18:29:54.000000 telliot_core-0.2.6/src/telliot_core/utils/versions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 18:30:06.365532 telliot_core-0.2.6/src/telliot_core.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1892 2023-04-28 18:30:06.000000 telliot_core-0.2.6/src/telliot_core.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4345 2023-04-28 18:30:06.000000 telliot_core-0.2.6/src/telliot_core.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-28 18:30:06.000000 telliot_core-0.2.6/src/telliot_core.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-04-28 18:30:06.000000 telliot_core-0.2.6/src/telliot_core.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-04-28 18:30:06.000000 telliot_core-0.2.6/src/telliot_core.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-04-28 18:30:06.000000 telliot_core-0.2.6/src/telliot_core.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 18:30:06.381533 telliot_core-0.2.6/tests/
--rw-r--r--   0 runner    (1001) docker     (123)       54 2023-04-28 18:29:54.000000 telliot_core-0.2.6/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4228 2023-04-28 18:29:54.000000 telliot_core-0.2.6/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)      505 2023-04-28 18:29:54.000000 telliot_core-0.2.6/tests/test_api_key.py
--rw-r--r--   0 runner    (1001) docker     (123)      471 2023-04-28 18:29:54.000000 telliot_core-0.2.6/tests/test_app.py
--rw-r--r--   0 runner    (1001) docker     (123)     1434 2023-04-28 18:29:54.000000 telliot_core-0.2.6/tests/test_app_core.py
--rw-r--r--   0 runner    (1001) docker     (123)      218 2023-04-28 18:29:54.000000 telliot_core-0.2.6/tests/test_asset_registry.py
--rw-r--r--   0 runner    (1001) docker     (123)      890 2023-04-28 18:29:54.000000 telliot_core-0.2.6/tests/test_autopay.py
--rw-r--r--   0 runner    (1001) docker     (123)     2216 2023-04-28 18:29:54.000000 telliot_core-0.2.6/tests/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     2012 2023-04-28 18:29:54.000000 telliot_core-0.2.6/tests/test_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     1253 2023-04-28 18:29:54.000000 telliot_core-0.2.6/tests/test_contract.py
--rw-r--r--   0 runner    (1001) docker     (123)     1979 2023-04-28 18:29:54.000000 telliot_core-0.2.6/tests/test_directory.py
--rw-r--r--   0 runner    (1001) docker     (123)     1601 2023-04-28 18:29:54.000000 telliot_core-0.2.6/tests/test_gas.py
--rw-r--r--   0 runner    (1001) docker     (123)      754 2023-04-28 18:29:54.000000 telliot_core-0.2.6/tests/test_listener.py
--rw-r--r--   0 runner    (1001) docker     (123)     1090 2023-04-28 18:29:54.000000 telliot_core-0.2.6/tests/test_master_read.py
--rw-r--r--   0 runner    (1001) docker     (123)      543 2023-04-28 18:29:54.000000 telliot_core-0.2.6/tests/test_model_chain.py
--rw-r--r--   0 runner    (1001) docker     (123)     5044 2023-04-28 18:29:54.000000 telliot_core-0.2.6/tests/test_oracle_read.py
--rw-r--r--   0 runner    (1001) docker     (123)     1442 2023-04-28 18:29:54.000000 telliot_core-0.2.6/tests/test_rpc_endpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2238 2023-04-28 18:29:54.000000 telliot_core-0.2.6/tests/test_session_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     1246 2023-04-28 18:29:54.000000 telliot_core-0.2.6/tests/test_telliot_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     2553 2023-04-28 18:29:54.000000 telliot_core-0.2.6/tests/test_tellorflex.py
--rw-r--r--   0 runner    (1001) docker     (123)      507 2023-04-28 18:29:54.000000 telliot_core-0.2.6/tests/test_timestamp.py
--rw-r--r--   0 runner    (1001) docker     (123)     1340 2023-04-28 18:29:54.000000 telliot_core-0.2.6/tests/test_token.py
--rw-r--r--   0 runner    (1001) docker     (123)      741 2023-04-28 18:29:54.000000 telliot_core-0.2.6/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 15:37:28.972586 telliot_core-0.2.7/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 15:37:28.900586 telliot_core-0.2.7/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 15:37:28.920586 telliot_core-0.2.7/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      716 2023-06-11 15:37:16.000000 telliot_core-0.2.7/.github/workflows/docs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1194 2023-06-11 15:37:16.000000 telliot_core-0.2.7/.github/workflows/py39.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1305 2023-06-11 15:37:16.000000 telliot_core-0.2.7/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      715 2023-06-11 15:37:16.000000 telliot_core-0.2.7/.github/workflows/style.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      719 2023-06-11 15:37:16.000000 telliot_core-0.2.7/.github/workflows/typing.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2401 2023-06-11 15:37:16.000000 telliot_core-0.2.7/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1095 2023-06-11 15:37:16.000000 telliot_core-0.2.7/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      665 2023-06-11 15:37:16.000000 telliot_core-0.2.7/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2159 2023-06-11 15:37:16.000000 telliot_core-0.2.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1892 2023-06-11 15:37:28.972586 telliot_core-0.2.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      974 2023-06-11 15:37:16.000000 telliot_core-0.2.7/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-06-11 15:37:16.000000 telliot_core-0.2.7/brownie-config.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 15:37:28.920586 telliot_core-0.2.7/contracts/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 15:37:28.920586 telliot_core-0.2.7/contracts/Integrations/
+-rw-r--r--   0 runner    (1001) docker     (123)      183 2023-06-11 15:37:16.000000 telliot_core-0.2.7/contracts/Integrations/DIVAOracleMock.sol
+-rw-r--r--   0 runner    (1001) docker     (123)     4315 2023-06-11 15:37:16.000000 telliot_core-0.2.7/contracts/Integrations/DIVAProtocolMock.sol
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-06-11 15:37:16.000000 telliot_core-0.2.7/contracts/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 15:37:28.920586 telliot_core-0.2.7/contracts/TellorFlex/
+-rw-r--r--   0 runner    (1001) docker     (123)      199 2023-06-11 15:37:16.000000 telliot_core-0.2.7/contracts/TellorFlex/AutopayMock.sol
+-rw-r--r--   0 runner    (1001) docker     (123)    20244 2023-06-11 15:37:16.000000 telliot_core-0.2.7/contracts/TellorFlex/TellorFlex.sol
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 15:37:28.924586 telliot_core-0.2.7/contracts/TellorFlex/testing/
+-rw-r--r--   0 runner    (1001) docker     (123)      317 2023-06-11 15:37:16.000000 telliot_core-0.2.7/contracts/TellorFlex/testing/StakingToken.sol
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 15:37:28.924586 telliot_core-0.2.7/contracts/TellorX/
+-rw-r--r--   0 runner    (1001) docker     (123)      650 2023-06-11 15:37:16.000000 telliot_core-0.2.7/contracts/TellorX/TellorXMasterMock.sol
+-rw-r--r--   0 runner    (1001) docker     (123)      949 2023-06-11 15:37:16.000000 telliot_core-0.2.7/contracts/TellorX/TellorXOracleMock.sol
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 15:37:28.924586 telliot_core-0.2.7/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      773 2023-06-11 15:37:16.000000 telliot_core-0.2.7/docs/add-chain.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 15:37:28.924586 telliot_core-0.2.7/docs/assets/
+-rw-r--r--   0 runner    (1001) docker     (123)     1722 2023-06-11 15:37:16.000000 telliot_core-0.2.7/docs/assets/favicon-32x32.png
+-rw-r--r--   0 runner    (1001) docker     (123)   160315 2023-06-11 15:37:16.000000 telliot_core-0.2.7/docs/assets/tellor_swoosh.png
+-rw-r--r--   0 runner    (1001) docker     (123)     3134 2023-06-11 15:37:16.000000 telliot_core-0.2.7/docs/contributing.md
+-rw-r--r--   0 runner    (1001) docker     (123)      693 2023-06-11 15:37:16.000000 telliot_core-0.2.7/docs/documentation.md
+-rw-r--r--   0 runner    (1001) docker     (123)      219 2023-06-11 15:37:16.000000 telliot_core-0.2.7/docs/index.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 15:37:28.928586 telliot_core-0.2.7/interfaces/
+-rw-r--r--   0 runner    (1001) docker     (123)      382 2023-06-11 15:37:16.000000 telliot_core-0.2.7/interfaces/IERC20.sol
+-rw-r--r--   0 runner    (1001) docker     (123)     1561 2023-06-11 15:37:16.000000 telliot_core-0.2.7/mkdocs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      377 2023-06-11 15:37:16.000000 telliot_core-0.2.7/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      152 2023-06-11 15:37:16.000000 telliot_core-0.2.7/requirements-dev.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 15:37:28.928586 telliot_core-0.2.7/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)     1912 2023-06-11 15:37:16.000000 telliot_core-0.2.7/scripts/morphware_data_sizes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7909 2023-06-11 15:37:16.000000 telliot_core-0.2.7/scripts/query_catalog.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2929 2023-06-11 15:37:16.000000 telliot_core-0.2.7/scripts/query_catalog.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1395 2023-06-11 15:37:28.976587 telliot_core-0.2.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-11 15:37:16.000000 telliot_core-0.2.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 15:37:28.904586 telliot_core-0.2.7/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 15:37:28.932587 telliot_core-0.2.7/src/telliot_core/
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-11 15:37:16.000000 telliot_core-0.2.7/src/telliot_core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      146 2023-06-11 15:37:16.000000 telliot_core-0.2.7/src/telliot_core/api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 15:37:28.936586 telliot_core-0.2.7/src/telliot_core/apps/
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-06-11 15:37:16.000000 telliot_core-0.2.7/src/telliot_core/apps/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1711 2023-06-11 15:37:16.000000 telliot_core-0.2.7/src/telliot_core/apps/app.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4328 2023-06-11 15:37:16.000000 telliot_core-0.2.7/src/telliot_core/apps/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11059 2023-06-11 15:37:16.000000 telliot_core-0.2.7/src/telliot_core/apps/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1700 2023-06-11 15:37:16.000000 telliot_core-0.2.7/src/telliot_core/apps/session_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4398 2023-06-11 15:37:16.000000 telliot_core-0.2.7/src/telliot_core/apps/telliot_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-06-11 15:37:16.000000 telliot_core-0.2.7/src/telliot_core/asset_registry.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 15:37:28.936586 telliot_core-0.2.7/src/telliot_core/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-11 15:37:16.000000 telliot_core-0.2.7/src/telliot_core/cli/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 15:37:28.940586 telliot_core-0.2.7/src/telliot_core/cli/commands/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-11 15:37:16.000000 telliot_core-0.2.7/src/telliot_core/cli/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1274 2023-06-11 15:37:16.000000 telliot_core-0.2.7/src/telliot_core/cli/commands/account.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1298 2023-06-11 15:37:16.000000 telliot_core-0.2.7/src/telliot_core/cli/commands/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1532 2023-06-11 15:37:16.000000 telliot_core-0.2.7/src/telliot_core/cli/commands/listen.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2965 2023-06-11 15:37:16.000000 telliot_core-0.2.7/src/telliot_core/cli/commands/read.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1397 2023-06-11 15:37:16.000000 telliot_core-0.2.7/src/telliot_core/cli/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1195 2023-06-11 15:37:16.000000 telliot_core-0.2.7/src/telliot_core/cli/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 15:37:28.940586 telliot_core-0.2.7/src/telliot_core/contract/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-11 15:37:16.000000 telliot_core-0.2.7/src/telliot_core/contract/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8707 2023-06-11 15:37:16.000000 telliot_core-0.2.7/src/telliot_core/contract/contract.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9665 2023-06-11 15:37:16.000000 telliot_core-0.2.7/src/telliot_core/contract/listener.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 15:37:28.944586 telliot_core-0.2.7/src/telliot_core/data/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-11 15:37:16.000000 telliot_core-0.2.7/src/telliot_core/data/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 15:37:28.952587 telliot_core-0.2.7/src/telliot_core/data/abi/
+-rw-r--r--   0 runner    (1001) docker     (123)     7513 2023-06-11 15:37:16.000000 telliot_core-0.2.7/src/telliot_core/data/abi/diva-oracle-tellor-abi.json
+-rw-r--r--   0 runner    (1001) docker     (123)    28088 2023-06-11 15:37:16.000000 telliot_core-0.2.7/src/telliot_core/data/abi/diva-protocol-abi.json
+-rw-r--r--   0 runner    (1001) docker     (123)     4935 2023-06-11 15:37:16.000000 telliot_core-0.2.7/src/telliot_core/data/abi/fuse-token-abi.json
+-rw-r--r--   0 runner    (1001) docker     (123)    20737 2023-06-11 15:37:16.000000 telliot_core-0.2.7/src/telliot_core/data/abi/tellor-governance-abi.json
+-rw-r--r--   0 runner    (1001) docker     (123)     4469 2023-06-11 15:37:16.000000 telliot_core-0.2.7/src/telliot_core/data/abi/tellor-mesosphere-abi.json
+-rw-r--r--   0 runner    (1001) docker     (123)    35232 2023-06-11 15:37:16.000000 telliot_core-0.2.7/src/telliot_core/data/abi/tellor360-autopay-abi.json
+-rw-r--r--   0 runner    (1001) docker     (123)    26675 2023-06-11 15:37:16.000000 telliot_core-0.2.7/src/telliot_core/data/abi/tellor360-oracle-abi.json
+-rw-r--r--   0 runner    (1001) docker     (123)    21821 2023-06-11 15:37:16.000000 telliot_core-0.2.7/src/telliot_core/data/abi/tellor360-playground.json
+-rw-r--r--   0 runner    (1001) docker     (123)    21041 2023-06-11 15:37:16.000000 telliot_core-0.2.7/src/telliot_core/data/abi/tellorflex-autopay-abi.json
+-rw-r--r--   0 runner    (1001) docker     (123)    15025 2023-06-11 15:37:16.000000 telliot_core-0.2.7/src/telliot_core/data/abi/tellorflex-oracle-abi.json
+-rw-r--r--   0 runner    (1001) docker     (123)    11824 2023-06-11 15:37:16.000000 telliot_core-0.2.7/src/telliot_core/data/abi/tellorx-governance-abi.json
+-rw-r--r--   0 runner    (1001) docker     (123)     6670 2023-06-11 15:37:16.000000 telliot_core-0.2.7/src/telliot_core/data/abi/tellorx-lens-abi.json
+-rw-r--r--   0 runner    (1001) docker     (123)    23746 2023-06-11 15:37:16.000000 telliot_core-0.2.7/src/telliot_core/data/abi/tellorx-master-abi.json
+-rw-r--r--   0 runner    (1001) docker     (123)    11141 2023-06-11 15:37:16.000000 telliot_core-0.2.7/src/telliot_core/data/abi/tellorx-oracle-abi.json
+-rw-r--r--   0 runner    (1001) docker     (123)     6681 2023-06-11 15:37:16.000000 telliot_core-0.2.7/src/telliot_core/data/abi/tellorx-treasury-abi.json
+-rw-r--r--   0 runner    (1001) docker     (123)    13989 2023-06-11 15:37:16.000000 telliot_core-0.2.7/src/telliot_core/data/abi/trb-token-abi.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3274 2023-06-11 15:37:16.000000 telliot_core-0.2.7/src/telliot_core/data/assets.json
+-rw-r--r--   0 runner    (1001) docker     (123)    10772 2023-06-11 15:37:16.000000 telliot_core-0.2.7/src/telliot_core/data/contract_directory.json
+-rw-r--r--   0 runner    (1001) docker     (123)     5667 2023-06-11 15:37:16.000000 telliot_core-0.2.7/src/telliot_core/directory.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 15:37:28.952587 telliot_core-0.2.7/src/telliot_core/gas/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-11 15:37:16.000000 telliot_core-0.2.7/src/telliot_core/gas/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4547 2023-06-11 15:37:16.000000 telliot_core-0.2.7/src/telliot_core/gas/legacy_gas.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1384 2023-06-11 15:37:16.000000 telliot_core-0.2.7/src/telliot_core/logs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 15:37:28.956586 telliot_core-0.2.7/src/telliot_core/model/
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-06-11 15:37:16.000000 telliot_core-0.2.7/src/telliot_core/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1677 2023-06-11 15:37:16.000000 telliot_core-0.2.7/src/telliot_core/model/api_keys.py
+-rw-r--r--   0 runner    (1001) docker     (123)      134 2023-06-11 15:37:16.000000 telliot_core-0.2.7/src/telliot_core/model/asset.py
+-rw-r--r--   0 runner    (1001) docker     (123)      121 2023-06-11 15:37:16.000000 telliot_core-0.2.7/src/telliot_core/model/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5217 2023-06-11 15:37:16.000000 telliot_core-0.2.7/src/telliot_core/model/chain.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8207 2023-06-11 15:37:16.000000 telliot_core-0.2.7/src/telliot_core/model/endpoints.py
+-rw-r--r--   0 runner    (1001) docker     (123)      260 2023-06-11 15:37:16.000000 telliot_core-0.2.7/src/telliot_core/model/registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2086 2023-06-11 15:37:16.000000 telliot_core-0.2.7/src/telliot_core/model/tokens.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 15:37:28.956586 telliot_core-0.2.7/src/telliot_core/reporters/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-11 15:37:16.000000 telliot_core-0.2.7/src/telliot_core/reporters/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 15:37:28.956586 telliot_core-0.2.7/src/telliot_core/tellor/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-11 15:37:16.000000 telliot_core-0.2.7/src/telliot_core/tellor/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 15:37:28.956586 telliot_core-0.2.7/src/telliot_core/tellor/tellor360/
+-rw-r--r--   0 runner    (1001) docker     (123)     1658 2023-06-11 15:37:16.000000 telliot_core-0.2.7/src/telliot_core/tellor/tellor360/autopay.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1344 2023-06-11 15:37:16.000000 telliot_core-0.2.7/src/telliot_core/tellor/tellor360/oracle.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 15:37:28.960587 telliot_core-0.2.7/src/telliot_core/tellor/tellorflex/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-11 15:37:16.000000 telliot_core-0.2.7/src/telliot_core/tellor/tellorflex/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2016 2023-06-11 15:37:16.000000 telliot_core-0.2.7/src/telliot_core/tellor/tellorflex/autopay.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3989 2023-06-11 15:37:16.000000 telliot_core-0.2.7/src/telliot_core/tellor/tellorflex/oracle.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-06-11 15:37:16.000000 telliot_core-0.2.7/src/telliot_core/tellor/tellorflex/token.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 15:37:28.960587 telliot_core-0.2.7/src/telliot_core/tellor/tellorx/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-11 15:37:16.000000 telliot_core-0.2.7/src/telliot_core/tellor/tellorx/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2591 2023-06-11 15:37:16.000000 telliot_core-0.2.7/src/telliot_core/tellor/tellorx/master.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4529 2023-06-11 15:37:16.000000 telliot_core-0.2.7/src/telliot_core/tellor/tellorx/oracle.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 15:37:28.964587 telliot_core-0.2.7/src/telliot_core/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-06-11 15:37:16.000000 telliot_core-0.2.7/src/telliot_core/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1248 2023-06-11 15:37:16.000000 telliot_core-0.2.7/src/telliot_core/utils/home.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1011 2023-06-11 15:37:16.000000 telliot_core-0.2.7/src/telliot_core/utils/key_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      222 2023-06-11 15:37:16.000000 telliot_core-0.2.7/src/telliot_core/utils/pyutils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      687 2023-06-11 15:37:16.000000 telliot_core-0.2.7/src/telliot_core/utils/response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1094 2023-06-11 15:37:16.000000 telliot_core-0.2.7/src/telliot_core/utils/timestamp.py
+-rw-r--r--   0 runner    (1001) docker     (123)      632 2023-06-11 15:37:16.000000 telliot_core-0.2.7/src/telliot_core/utils/versions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 15:37:28.932587 telliot_core-0.2.7/src/telliot_core.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1892 2023-06-11 15:37:28.000000 telliot_core-0.2.7/src/telliot_core.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4345 2023-06-11 15:37:28.000000 telliot_core-0.2.7/src/telliot_core.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-11 15:37:28.000000 telliot_core-0.2.7/src/telliot_core.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-06-11 15:37:28.000000 telliot_core-0.2.7/src/telliot_core.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-06-11 15:37:28.000000 telliot_core-0.2.7/src/telliot_core.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-11 15:37:28.000000 telliot_core-0.2.7/src/telliot_core.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 15:37:28.972586 telliot_core-0.2.7/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-06-11 15:37:16.000000 telliot_core-0.2.7/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3517 2023-06-11 15:37:16.000000 telliot_core-0.2.7/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      505 2023-06-11 15:37:16.000000 telliot_core-0.2.7/tests/test_api_key.py
+-rw-r--r--   0 runner    (1001) docker     (123)      471 2023-06-11 15:37:16.000000 telliot_core-0.2.7/tests/test_app.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1434 2023-06-11 15:37:16.000000 telliot_core-0.2.7/tests/test_app_core.py
+-rw-r--r--   0 runner    (1001) docker     (123)      218 2023-06-11 15:37:16.000000 telliot_core-0.2.7/tests/test_asset_registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)      890 2023-06-11 15:37:16.000000 telliot_core-0.2.7/tests/test_autopay.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2216 2023-06-11 15:37:16.000000 telliot_core-0.2.7/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2012 2023-06-11 15:37:16.000000 telliot_core-0.2.7/tests/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1253 2023-06-11 15:37:16.000000 telliot_core-0.2.7/tests/test_contract.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1979 2023-06-11 15:37:16.000000 telliot_core-0.2.7/tests/test_directory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1601 2023-06-11 15:37:16.000000 telliot_core-0.2.7/tests/test_gas.py
+-rw-r--r--   0 runner    (1001) docker     (123)      754 2023-06-11 15:37:16.000000 telliot_core-0.2.7/tests/test_listener.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1090 2023-06-11 15:37:16.000000 telliot_core-0.2.7/tests/test_master_read.py
+-rw-r--r--   0 runner    (1001) docker     (123)      543 2023-06-11 15:37:16.000000 telliot_core-0.2.7/tests/test_model_chain.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5044 2023-06-11 15:37:16.000000 telliot_core-0.2.7/tests/test_oracle_read.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1448 2023-06-11 15:37:16.000000 telliot_core-0.2.7/tests/test_rpc_endpoint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2238 2023-06-11 15:37:16.000000 telliot_core-0.2.7/tests/test_session_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1246 2023-06-11 15:37:16.000000 telliot_core-0.2.7/tests/test_telliot_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2553 2023-06-11 15:37:16.000000 telliot_core-0.2.7/tests/test_tellorflex.py
+-rw-r--r--   0 runner    (1001) docker     (123)      507 2023-06-11 15:37:16.000000 telliot_core-0.2.7/tests/test_timestamp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1340 2023-06-11 15:37:16.000000 telliot_core-0.2.7/tests/test_token.py
+-rw-r--r--   0 runner    (1001) docker     (123)      741 2023-06-11 15:37:16.000000 telliot_core-0.2.7/tox.ini
```

### Comparing `telliot_core-0.2.6/.github/workflows/docs.yml` & `telliot_core-0.2.7/.github/workflows/docs.yml`

 * *Files identical despite different names*

### Comparing `telliot_core-0.2.6/.github/workflows/py39.yml` & `telliot_core-0.2.7/.github/workflows/py39.yml`

 * *Files identical despite different names*

### Comparing `telliot_core-0.2.6/.github/workflows/release.yml` & `telliot_core-0.2.7/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `telliot_core-0.2.6/.github/workflows/style.yml` & `telliot_core-0.2.7/.github/workflows/style.yml`

 * *Files identical despite different names*

### Comparing `telliot_core-0.2.6/.github/workflows/typing.yml` & `telliot_core-0.2.7/.github/workflows/typing.yml`

 * *Files identical despite different names*

### Comparing `telliot_core-0.2.6/.gitignore` & `telliot_core-0.2.7/.gitignore`

 * *Files 1% similar despite different names*

```diff
@@ -160,7 +160,10 @@
 Pipfile
 Pipfile.lock
 
 # eth-brownie related files & dependencies
 package.json
 package-lock.json
 node_modules/
+
+# MacOS
+.DS_Store
```

### Comparing `telliot_core-0.2.6/.pre-commit-config.yaml` & `telliot_core-0.2.7/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `telliot_core-0.2.6/.readthedocs.yaml` & `telliot_core-0.2.7/.readthedocs.yaml`

 * *Files identical despite different names*

### Comparing `telliot_core-0.2.6/LICENSE` & `telliot_core-0.2.7/LICENSE`

 * *Files identical despite different names*

### Comparing `telliot_core-0.2.6/PKG-INFO` & `telliot_core-0.2.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: telliot_core
-Version: 0.2.6
+Version: 0.2.7
 Summary: Telliot is a Python framework for interacting with the decentralized TellorX network.
 Home-page: https://github.com/tellor-io/telliot-core
 Author: Tellor Development Community
 Author-email: info@tellor.io
 License: MIT
 Keywords: oracle,etherium,blockchain
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `telliot_core-0.2.6/README.md` & `telliot_core-0.2.7/README.md`

 * *Files identical despite different names*

### Comparing `telliot_core-0.2.6/contracts/Integrations/DIVAProtocolMock.sol` & `telliot_core-0.2.7/contracts/Integrations/DIVAProtocolMock.sol`

 * *Files identical despite different names*

### Comparing `telliot_core-0.2.6/contracts/TellorFlex/TellorFlex.sol` & `telliot_core-0.2.7/contracts/TellorFlex/TellorFlex.sol`

 * *Files identical despite different names*

### Comparing `telliot_core-0.2.6/contracts/TellorX/TellorXMasterMock.sol` & `telliot_core-0.2.7/contracts/TellorX/TellorXMasterMock.sol`

 * *Files identical despite different names*

### Comparing `telliot_core-0.2.6/contracts/TellorX/TellorXOracleMock.sol` & `telliot_core-0.2.7/contracts/TellorX/TellorXOracleMock.sol`

 * *Files identical despite different names*

### Comparing `telliot_core-0.2.6/docs/add-chain.md` & `telliot_core-0.2.7/docs/add-chain.md`

 * *Files identical despite different names*

### Comparing `telliot_core-0.2.6/docs/assets/favicon-32x32.png` & `telliot_core-0.2.7/docs/assets/favicon-32x32.png`

 * *Files identical despite different names*

### Comparing `telliot_core-0.2.6/docs/assets/tellor_swoosh.png` & `telliot_core-0.2.7/docs/assets/tellor_swoosh.png`

 * *Files identical despite different names*

### Comparing `telliot_core-0.2.6/docs/contributing.md` & `telliot_core-0.2.7/docs/contributing.md`

 * *Files identical despite different names*

### Comparing `telliot_core-0.2.6/docs/documentation.md` & `telliot_core-0.2.7/docs/documentation.md`

 * *Files identical despite different names*

### Comparing `telliot_core-0.2.6/mkdocs.yml` & `telliot_core-0.2.7/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `telliot_core-0.2.6/scripts/morphware_data_sizes.py` & `telliot_core-0.2.7/scripts/morphware_data_sizes.py`

 * *Files identical despite different names*

### Comparing `telliot_core-0.2.6/scripts/query_catalog.md` & `telliot_core-0.2.7/scripts/query_catalog.md`

 * *Files identical despite different names*

### Comparing `telliot_core-0.2.6/scripts/query_catalog.yaml` & `telliot_core-0.2.7/scripts/query_catalog.yaml`

 * *Files identical despite different names*

### Comparing `telliot_core-0.2.6/setup.cfg` & `telliot_core-0.2.7/setup.cfg`

 * *Files identical despite different names*

### Comparing `telliot_core-0.2.6/src/telliot_core/apps/app.py` & `telliot_core-0.2.7/src/telliot_core/apps/app.py`

 * *Files identical despite different names*

### Comparing `telliot_core-0.2.6/src/telliot_core/apps/config.py` & `telliot_core-0.2.7/src/telliot_core/apps/config.py`

 * *Files identical despite different names*

### Comparing `telliot_core-0.2.6/src/telliot_core/apps/core.py` & `telliot_core-0.2.7/src/telliot_core/apps/core.py`

 * *Files 1% similar despite different names*

```diff
@@ -37,24 +37,25 @@
     80001: "polygon-mumbai",
     122: "fuse-mainnet",
     69: "optimism-kovan",
     1666600000: "harmony-mainnet",
     1666700000: "harmony-testnet",
     421611: "arbitrum-rinkeby",
     421613: "arbitrum-goerli",
-    941: "pulsechain-testnet",
     42161: "arbitrum",
     1337: "brownie-local-network",
     10200: "chiado-testnet",
     100: "gnosis",
     10: "optimism",
     3141: "filecoin-hyperspace",
     314159: "filecoin-calibration",
     314: "filecoin",
     11155111: "sepolia",
+    369: "pulsechain",
+    943: "pulsechain-testnet",
 }
 
 LOGLEVEL_MAP = {
     "CRITICAL": logging.CRITICAL,
     "ERROR": logging.ERROR,
     "WARNING": logging.WARNING,
     "INFO": logging.INFO,
```

### Comparing `telliot_core-0.2.6/src/telliot_core/apps/session_manager.py` & `telliot_core-0.2.7/src/telliot_core/apps/session_manager.py`

 * *Files identical despite different names*

### Comparing `telliot_core-0.2.6/src/telliot_core/apps/telliot_config.py` & `telliot_core-0.2.7/src/telliot_core/apps/telliot_config.py`

 * *Files identical despite different names*

### Comparing `telliot_core-0.2.6/src/telliot_core/asset_registry.py` & `telliot_core-0.2.7/src/telliot_core/asset_registry.py`

 * *Files identical despite different names*

### Comparing `telliot_core-0.2.6/src/telliot_core/cli/commands/account.py` & `telliot_core-0.2.7/src/telliot_core/cli/commands/account.py`

 * *Files identical despite different names*

### Comparing `telliot_core-0.2.6/src/telliot_core/cli/commands/config.py` & `telliot_core-0.2.7/src/telliot_core/cli/commands/config.py`

 * *Files identical despite different names*

### Comparing `telliot_core-0.2.6/src/telliot_core/cli/commands/listen.py` & `telliot_core-0.2.7/src/telliot_core/cli/commands/listen.py`

 * *Files identical despite different names*

### Comparing `telliot_core-0.2.6/src/telliot_core/cli/commands/read.py` & `telliot_core-0.2.7/src/telliot_core/cli/commands/read.py`

 * *Files identical despite different names*

### Comparing `telliot_core-0.2.6/src/telliot_core/cli/main.py` & `telliot_core-0.2.7/src/telliot_core/cli/main.py`

 * *Files identical despite different names*

### Comparing `telliot_core-0.2.6/src/telliot_core/cli/utils.py` & `telliot_core-0.2.7/src/telliot_core/cli/utils.py`

 * *Files identical despite different names*

### Comparing `telliot_core-0.2.6/src/telliot_core/contract/contract.py` & `telliot_core-0.2.7/src/telliot_core/contract/contract.py`

 * *Files identical despite different names*

### Comparing `telliot_core-0.2.6/src/telliot_core/contract/listener.py` & `telliot_core-0.2.7/src/telliot_core/contract/listener.py`

 * *Files identical despite different names*

### Comparing `telliot_core-0.2.6/src/telliot_core/data/abi/diva-oracle-tellor-abi.json` & `telliot_core-0.2.7/src/telliot_core/data/abi/diva-oracle-tellor-abi.json`

 * *Files identical despite different names*

### Comparing `telliot_core-0.2.6/src/telliot_core/data/abi/diva-protocol-abi.json` & `telliot_core-0.2.7/src/telliot_core/data/abi/diva-protocol-abi.json`

 * *Files identical despite different names*

### Comparing `telliot_core-0.2.6/src/telliot_core/data/abi/fuse-token-abi.json` & `telliot_core-0.2.7/src/telliot_core/data/abi/fuse-token-abi.json`

 * *Files identical despite different names*

### Comparing `telliot_core-0.2.6/src/telliot_core/data/abi/tellor-governance-abi.json` & `telliot_core-0.2.7/src/telliot_core/data/abi/tellor-governance-abi.json`

 * *Files identical despite different names*

### Comparing `telliot_core-0.2.6/src/telliot_core/data/abi/tellor-mesosphere-abi.json` & `telliot_core-0.2.7/src/telliot_core/data/abi/tellor-mesosphere-abi.json`

 * *Files identical despite different names*

### Comparing `telliot_core-0.2.6/src/telliot_core/data/abi/tellor360-autopay-abi.json` & `telliot_core-0.2.7/src/telliot_core/data/abi/tellor360-autopay-abi.json`

 * *Files identical despite different names*

### Comparing `telliot_core-0.2.6/src/telliot_core/data/abi/tellor360-oracle-abi.json` & `telliot_core-0.2.7/src/telliot_core/data/abi/tellor360-oracle-abi.json`

 * *Files identical despite different names*

### Comparing `telliot_core-0.2.6/src/telliot_core/data/abi/tellor360-playground.json` & `telliot_core-0.2.7/src/telliot_core/data/abi/tellor360-playground.json`

 * *Files identical despite different names*

### Comparing `telliot_core-0.2.6/src/telliot_core/data/abi/tellorflex-autopay-abi.json` & `telliot_core-0.2.7/src/telliot_core/data/abi/tellorflex-autopay-abi.json`

 * *Files identical despite different names*

### Comparing `telliot_core-0.2.6/src/telliot_core/data/abi/tellorflex-oracle-abi.json` & `telliot_core-0.2.7/src/telliot_core/data/abi/tellorflex-oracle-abi.json`

 * *Files identical despite different names*

### Comparing `telliot_core-0.2.6/src/telliot_core/data/abi/tellorx-governance-abi.json` & `telliot_core-0.2.7/src/telliot_core/data/abi/tellorx-governance-abi.json`

 * *Files identical despite different names*

### Comparing `telliot_core-0.2.6/src/telliot_core/data/abi/tellorx-lens-abi.json` & `telliot_core-0.2.7/src/telliot_core/data/abi/tellorx-lens-abi.json`

 * *Files identical despite different names*

### Comparing `telliot_core-0.2.6/src/telliot_core/data/abi/tellorx-master-abi.json` & `telliot_core-0.2.7/src/telliot_core/data/abi/tellorx-master-abi.json`

 * *Files identical despite different names*

### Comparing `telliot_core-0.2.6/src/telliot_core/data/abi/tellorx-oracle-abi.json` & `telliot_core-0.2.7/src/telliot_core/data/abi/tellorx-oracle-abi.json`

 * *Files identical despite different names*

### Comparing `telliot_core-0.2.6/src/telliot_core/data/abi/tellorx-treasury-abi.json` & `telliot_core-0.2.7/src/telliot_core/data/abi/tellorx-treasury-abi.json`

 * *Files identical despite different names*

### Comparing `telliot_core-0.2.6/src/telliot_core/data/abi/trb-token-abi.json` & `telliot_core-0.2.7/src/telliot_core/data/abi/trb-token-abi.json`

 * *Files identical despite different names*

### Comparing `telliot_core-0.2.6/src/telliot_core/data/assets.json` & `telliot_core-0.2.7/src/telliot_core/data/assets.json`

 * *Files identical despite different names*

### Comparing `telliot_core-0.2.6/src/telliot_core/data/contract_directory.json` & `telliot_core-0.2.7/src/telliot_core/data/contract_directory.json`

 * *Files 4% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9858861158359746%*

 * *Differences: {'0': "{'address': {'369': '0x88dF592F8eb5D7Bd38bFeF7dEb0fBc02cf3778a0', '943': "*

 * *      "'0x88dF592F8eb5D7Bd38bFeF7dEb0fBc02cf3778a0'}}",*

 * * '1': "{'address': {'369': '0xf98624E9924CAA2cbD21cC6288215Ec2ef7cFE80', '943': "*

 * *      "'0xf98624E9924CAA2cbD21cC6288215Ec2ef7cFE80'}}",*

 * * '18': "{'address': {'369': '0x46038969D7DC0b17BC72137D07b4eDe43859DA45', '943': "*

 * *       "'0x46038969D7DC0b17BC72137D07b4eDe43859DA45'}}",*

 * * '2': "{'address': {'369': '0xe8218cACb0a5421BC6409e498d9f8CC8869945ea', '943': "*

 * *      "'0xe821 […]*

```diff
@@ -1,58 +1,68 @@
 [
     {
         "abi_file": "tellorx-master-abi.json",
         "address": {
             "1": "0x88dF592F8eb5D7Bd38bFeF7dEb0fBc02cf3778a0",
+            "369": "0x88dF592F8eb5D7Bd38bFeF7dEb0fBc02cf3778a0",
             "4": "0x88dF592F8eb5D7Bd38bFeF7dEb0fBc02cf3778a0",
-            "5": "0x51c59c6cAd28ce3693977F2feB4CfAebec30d8a2"
+            "5": "0x51c59c6cAd28ce3693977F2feB4CfAebec30d8a2",
+            "943": "0x88dF592F8eb5D7Bd38bFeF7dEb0fBc02cf3778a0"
         },
         "name": "tellorx-master",
         "org": "tellor",
         "type": "ContractInfo"
     },
     {
         "abi_file": null,
         "address": {
             "1": "0xf98624E9924CAA2cbD21cC6288215Ec2ef7cFE80",
+            "369": "0xf98624E9924CAA2cbD21cC6288215Ec2ef7cFE80",
             "4": "0x0f2b0a8fa0f60459f51e452273c879eb32555e91",
-            "5": "0xaF8797c5C113abC7338535581243e11168326082"
+            "5": "0xaF8797c5C113abC7338535581243e11168326082",
+            "943": "0xf98624E9924CAA2cbD21cC6288215Ec2ef7cFE80"
         },
         "name": "tellorx-controller",
         "org": "tellor",
         "type": "ContractInfo"
     },
     {
         "abi_file": "tellorx-oracle-abi.json",
         "address": {
             "1": "0xe8218cACb0a5421BC6409e498d9f8CC8869945ea",
+            "369": "0xe8218cACb0a5421BC6409e498d9f8CC8869945ea",
             "4": "0x18431fd88adF138e8b979A7246eb58EA7126ea16",
-            "5": "0x6732b279E7C975B39DfFedA7173e4E426aA9a40F"
+            "5": "0x6732b279E7C975B39DfFedA7173e4E426aA9a40F",
+            "943": "0xe8218cACb0a5421BC6409e498d9f8CC8869945ea"
         },
         "name": "tellorx-oracle",
         "org": "tellor",
         "type": "ContractInfo"
     },
     {
         "abi_file": "tellorx-governance-abi.json",
         "address": {
             "1": "0x51d4088d4EeE00Ae4c55f46E0673e9997121DB00",
+            "369": "0x51d4088d4EeE00Ae4c55f46E0673e9997121DB00",
             "4": "0xA64Bb0078eB80c97484f3f09Adb47b9B73CBcA00",
-            "5": "0x45B24bd85261210e1354d203682C7127cc3D44E6"
+            "5": "0x45B24bd85261210e1354d203682C7127cc3D44E6",
+            "943": "0x51d4088d4EeE00Ae4c55f46E0673e9997121DB00"
         },
         "name": "tellorx-governance",
         "org": "tellor",
         "type": "ContractInfo"
     },
     {
         "abi_file": "tellorx-treasury-abi.json",
         "address": {
             "1": "0x3b0f3eaEFaAc9f8F7FDe406919ecEb5270fE0607",
+            "369": "0x3b0f3eaEFaAc9f8F7FDe406919ecEb5270fE0607",
             "4": "0x2dB91443f2b562B8b2B2e8E4fC0A3EDD6c195147",
-            "5": "0x0a453872d73C3f4122aC26D03aD58285dAee6D6A"
+            "5": "0x0a453872d73C3f4122aC26D03aD58285dAee6D6A",
+            "943": "0x3b0f3eaEFaAc9f8F7FDe406919ecEb5270fE0607"
         },
         "name": "tellorx-treasury",
         "org": "tellor",
         "type": "ContractInfo"
     },
     {
         "abi_file": "tellorflex-oracle-abi.json",
@@ -62,16 +72,15 @@
             "1666600000": "0xb32e05DF1f11B1f0E1DE2A35F4D99393EB86FF8B",
             "1666700000": "0xbB97C038c338c3DcAF06D5be3B4A3e0B24835f9C",
             "3": "0x7B8AC044ebce66aCdF14197E8De38C1Cc802dB4A",
             "42161": "0x73B6715D9289bdfE5e758bB7ace782Cc7C933cfC",
             "421611": "0xbB97C038c338c3DcAF06D5be3B4A3e0B24835f9C",
             "5": "0x7B8AC044ebce66aCdF14197E8De38C1Cc802dB4A",
             "69": "0xa0013274d34a7c469952379646F26aA1C1237131",
-            "80001": "0x840c23e39F9D029fFa888F47069aA6864f0401D7",
-            "941": "0xB0A15Da1538D0968A32858273E64fcd0F9869283"
+            "80001": "0x840c23e39F9D029fFa888F47069aA6864f0401D7"
         },
         "name": "tellorflex-oracle",
         "org": "tellor",
         "type": "ContractInfo"
     },
     {
         "abi_file": "tellorflex-autopay-abi.json",
@@ -80,16 +89,15 @@
             "1666600000": "0xD789488E5ee48Ef8b0719843672Bc04c213b648c",
             "1666700000": "0x7B49420008BcA14782F2700547764AdAdD54F813",
             "3": "0x7B49420008BcA14782F2700547764AdAdD54F813",
             "42161": "0xd844B26dfAfB0776E70aF12C19189b740329A266",
             "421611": "0x7B49420008BcA14782F2700547764AdAdD54F813",
             "5": "0x7B49420008BcA14782F2700547764AdAdD54F813",
             "69": "0x7B49420008BcA14782F2700547764AdAdD54F813",
-            "80001": "0x7B49420008BcA14782F2700547764AdAdD54F813",
-            "941": "0xEea6D02cB52163119fDbD46c80617968079b5Af7"
+            "80001": "0x7B49420008BcA14782F2700547764AdAdD54F813"
         },
         "name": "tellorflex-autopay",
         "org": "tellor",
         "type": "ContractInfo"
     },
     {
         "abi_file": "tellor360-oracle-abi.json",
@@ -99,20 +107,22 @@
             "100": "0xD9157453E2668B2fc45b7A803D3FEF3642430cC0",
             "10200": "0xD9157453E2668B2fc45b7A803D3FEF3642430cC0",
             "11155111": "0x199839a4907ABeC8240D119B606C98c405Bb0B33",
             "137": "0xD9157453E2668B2fc45b7A803D3FEF3642430cC0",
             "314": "0xb2CB696fE5244fB9004877e58dcB680cB86Ba444",
             "3141": "0xb2CB696fE5244fB9004877e58dcB680cB86Ba444",
             "314159": "0xb2CB696fE5244fB9004877e58dcB680cB86Ba444",
+            "369": "0xD9157453E2668B2fc45b7A803D3FEF3642430cC0",
             "4": "0xDb7923FA7D8959A5aDCAA2B652508420f9E47541",
             "420": "0xD9157453E2668B2fc45b7A803D3FEF3642430cC0",
             "42161": "0xD9157453E2668B2fc45b7A803D3FEF3642430cC0",
             "421613": "0xb2CB696fE5244fB9004877e58dcB680cB86Ba444",
             "5": "0xD9157453E2668B2fc45b7A803D3FEF3642430cC0",
-            "80001": "0xD9157453E2668B2fc45b7A803D3FEF3642430cC0"
+            "80001": "0xD9157453E2668B2fc45b7A803D3FEF3642430cC0",
+            "943": "0xD9157453E2668B2fc45b7A803D3FEF3642430cC0"
         },
         "name": "tellor360-oracle",
         "org": "tellor",
         "type": "ContractInfo"
     },
     {
         "abi_file": "tellor360-autopay-abi.json",
@@ -122,20 +132,22 @@
             "100": "0x9BE9B0CFA89Ea800556C6efbA67b455D336db1D0",
             "10200": "0x9BE9B0CFA89Ea800556C6efbA67b455D336db1D0",
             "11155111": "0x7E7b96d13D75bc7DaF270A491e2f1e571147d4DA",
             "137": "0x9BE9B0CFA89Ea800556C6efbA67b455D336db1D0",
             "314": "0x60cBf3991F05a0671250e673Aa166e9D1A0C662E",
             "3141": "0x60cBf3991F05a0671250e673Aa166e9D1A0C662E",
             "314159": "0x60cBf3991F05a0671250e673Aa166e9D1A0C662E",
+            "369": "0x9BE9B0CFA89Ea800556C6efbA67b455D336db1D0",
             "4": "0xb4a418153039eECcaEE2d74D57766BF943aA8d53",
             "420": "0x9BE9B0CFA89Ea800556C6efbA67b455D336db1D0",
             "42161": "0x9BE9B0CFA89Ea800556C6efbA67b455D336db1D0",
             "421613": "0x60cBf3991F05a0671250e673Aa166e9D1A0C662E",
             "5": "0x9BE9B0CFA89Ea800556C6efbA67b455D336db1D0",
-            "80001": "0x9BE9B0CFA89Ea800556C6efbA67b455D336db1D0"
+            "80001": "0x9BE9B0CFA89Ea800556C6efbA67b455D336db1D0",
+            "943": "0x9BE9B0CFA89Ea800556C6efbA67b455D336db1D0"
         },
         "name": "tellor360-autopay",
         "org": "tellor",
         "type": "ContractInfo"
     },
     {
         "abi_file": "trb-token-abi.json",
@@ -148,23 +160,24 @@
             "137": "0xE3322702BEdaaEd36CdDAb233360B939775ae5f1",
             "1666600000": "0xd4b28ecb7b765C89F1e67dE3359d09A3520f794E",
             "1666700000": "0x7B8AC044ebce66aCdF14197E8De38C1Cc802dB4A",
             "3": "0x7B8AC044ebce66aCdF14197E8De38C1Cc802dB4A",
             "314": "0x045CE60839d108B43dF9e703d4b25402a6a28a0d",
             "3141": "0xe7147C5Ed14F545B4B17251992D1DB2bdfa26B6d",
             "314159": "0x15e6Cc0D69A162151Cadfba035aa10b82b12b970",
+            "369": "0x88dF592F8eb5D7Bd38bFeF7dEb0fBc02cf3778a0",
             "4": "0x88dF592F8eb5D7Bd38bFeF7dEb0fBc02cf3778a0",
             "420": "0xd71F72C18767083e4e3FE84F9c62b8038C1Ef4f6",
             "42161": "0xd58D345Fd9c82262E087d2D0607624B410D88242",
             "421611": "0x126f5C4802c10848Eb66ce2F74380B7ADeFF36Cb",
             "421613": "0x8d1bB5eDdFce08B92dD47c9871d1805211C3Eb3C",
             "5": "0x51c59c6cAd28ce3693977F2feB4CfAebec30d8a2",
             "69": "0x7B8AC044ebce66aCdF14197E8De38C1Cc802dB4A",
             "80001": "0xce4e32fe9d894f8185271aa990d2db425df3e6be",
-            "941": "0x08b193bC308eC1E60cE0064CB503c9D85A841347"
+            "943": "0x88dF592F8eb5D7Bd38bFeF7dEb0fBc02cf3778a0"
         },
         "name": "trb-token",
         "org": "tellor",
         "type": "ContractInfo"
     },
     {
         "abi_file": "tellorx-lens-abi.json",
@@ -253,18 +266,20 @@
             "100": "0x46038969D7DC0b17BC72137D07b4eDe43859DA45",
             "10200": "0x46038969D7DC0b17BC72137D07b4eDe43859DA45",
             "11155111": "0x8C9057FA16D3Debb703ADBac0A097d2E5577AA6b",
             "137": "0x46038969D7DC0b17BC72137D07b4eDe43859DA45",
             "314": "0xb55bB55f7D8b4F26Bd18198088C96488D95cab39",
             "3141": "0xb55bB55f7D8b4F26Bd18198088C96488D95cab39",
             "314159": "0xb55bB55f7D8b4F26Bd18198088C96488D95cab39",
+            "369": "0x46038969D7DC0b17BC72137D07b4eDe43859DA45",
             "420": "0x46038969D7DC0b17BC72137D07b4eDe43859DA45",
             "42161": "0x46038969D7DC0b17BC72137D07b4eDe43859DA45",
             "421613": "0xb55bB55f7D8b4F26Bd18198088C96488D95cab39",
             "5": "0x46038969D7DC0b17BC72137D07b4eDe43859DA45",
-            "80001": "0x46038969D7DC0b17BC72137D07b4eDe43859DA45"
+            "80001": "0x46038969D7DC0b17BC72137D07b4eDe43859DA45",
+            "943": "0x46038969D7DC0b17BC72137D07b4eDe43859DA45"
         },
         "name": "tellor-governance",
         "org": "tellor",
         "type": "ContractInfo"
     }
 ]
```

### Comparing `telliot_core-0.2.6/src/telliot_core/directory.py` & `telliot_core-0.2.7/src/telliot_core/directory.py`

 * *Files identical despite different names*

### Comparing `telliot_core-0.2.6/src/telliot_core/gas/legacy_gas.py` & `telliot_core-0.2.7/src/telliot_core/gas/legacy_gas.py`

 * *Files identical despite different names*

### Comparing `telliot_core-0.2.6/src/telliot_core/logs.py` & `telliot_core-0.2.7/src/telliot_core/logs.py`

 * *Files identical despite different names*

### Comparing `telliot_core-0.2.6/src/telliot_core/model/api_keys.py` & `telliot_core-0.2.7/src/telliot_core/model/api_keys.py`

 * *Files identical despite different names*

### Comparing `telliot_core-0.2.6/src/telliot_core/model/chain.py` & `telliot_core-0.2.7/src/telliot_core/model/chain.py`

 * *Files 1% similar despite different names*

```diff
@@ -84,21 +84,14 @@
         chain_id=421611,
         name="Arbitrum Rinkeby",
         chain="Arbitrum",
         network="testnet",
         currency=EVMCurrency(name="Ether", symbol="ETH", decimals=18),
     ),
     Chain(
-        chain_id=941,
-        name="Pulsechain Testnet",
-        chain="Pulechain",
-        network="testnet",
-        currency=EVMCurrency(name="Pulsechain tPLS", symbol="tPLS", decimals=18),
-    ),
-    Chain(
         chain_id=42161,
         name="Arbitrum One",
         chain="Arbitrum",
         network="mainnet",
         currency=EVMCurrency(name="Arbitrum Ether", symbol="ETH", decimals=18),
     ),
     Chain(
@@ -160,14 +153,28 @@
     Chain(
         chain_id=11155111,
         name="sepolia",
         chain="sepolia",
         network="testnet",
         currency=EVMCurrency(name="Ether", symbol="ETH", decimals=18),
     ),
+    Chain(
+        chain_id=369,
+        name="pulsechain",
+        chain="pulsechain",
+        network="mainnet",
+        currency=EVMCurrency(name="PulseChain PLS", symbol="PLS", decimals=18),
+    ),
+    Chain(
+        chain_id=943,
+        name="pulsechain-testnet",
+        chain="pulsechain-testnet",
+        network="testnet",
+        currency=EVMCurrency(name="PulseChain tPLS", symbol="tPLS", decimals=18),
+    ),
 ]
 
 
 @dataclass
 class ChainList(ConfigOptions):
     chains: List[Chain] = field(default_factory=lambda: default_chain_list)
```

### Comparing `telliot_core-0.2.6/src/telliot_core/model/endpoints.py` & `telliot_core-0.2.7/src/telliot_core/model/endpoints.py`

 * *Files 2% similar despite different names*

```diff
@@ -154,21 +154,14 @@
         chain_id=421611,
         provider="Infura",
         network="Arbitrum Rinkeby",
         url="https://arbitrum-rinkeby.infura.io/v3/{INFURA_API_KEY}",
         explorer="https://rinkeby-explorer.arbitrum.io/#/",
     ),
     RPCEndpoint(
-        chain_id=941,
-        provider="Pulsechain",
-        network="Pulsechain Testnet",
-        url="https://rpc.v2b.testnet.pulsechain.com",
-        explorer="https://scan.v2b.testnet.pulsechain.com",
-    ),
-    RPCEndpoint(
         chain_id=42161,
         provider="Infura",
         network="Arbitrum One",
         url="https://arbitrum-mainnet.infura.io/v3/{INFURA_API_KEY}",
         explorer="https://arbiscan.io",
     ),
     RPCEndpoint(
@@ -230,14 +223,28 @@
     RPCEndpoint(
         chain_id=11155111,
         provider="Sepolia",
         network="sepolia",
         url="https://sepolia.infura.io/v3/{INFURA_API_KEY}",
         explorer="https://sepolia.etherscan.io/",
     ),
+    RPCEndpoint(
+        chain_id=369,
+        provider="PulseChain",
+        network="pulsechain",
+        url="https://rpc.pulsechain.com",
+        explorer="https://scan.pulsechain.com/",
+    ),
+    RPCEndpoint(
+        chain_id=943,
+        provider="PulseChain Testnet",
+        network="pulsechain-testnet",
+        url="https://rpc.v4.testnet.pulsechain.com",
+        explorer="https://scan.v4.testnet.pulsechain.com/",
+    ),
 ]
 
 
 @dataclass
 class EndpointList(ConfigOptions):
     endpoints: List[RPCEndpoint] = field(default_factory=lambda: default_endpoint_list)
```

### Comparing `telliot_core-0.2.6/src/telliot_core/model/tokens.py` & `telliot_core-0.2.7/src/telliot_core/model/tokens.py`

 * *Files identical despite different names*

### Comparing `telliot_core-0.2.6/src/telliot_core/tellor/tellor360/autopay.py` & `telliot_core-0.2.7/src/telliot_core/tellor/tellor360/autopay.py`

 * *Files identical despite different names*

### Comparing `telliot_core-0.2.6/src/telliot_core/tellor/tellor360/oracle.py` & `telliot_core-0.2.7/src/telliot_core/tellor/tellor360/oracle.py`

 * *Files identical despite different names*

### Comparing `telliot_core-0.2.6/src/telliot_core/tellor/tellorflex/autopay.py` & `telliot_core-0.2.7/src/telliot_core/tellor/tellorflex/autopay.py`

 * *Files identical despite different names*

### Comparing `telliot_core-0.2.6/src/telliot_core/tellor/tellorflex/oracle.py` & `telliot_core-0.2.7/src/telliot_core/tellor/tellorflex/oracle.py`

 * *Files identical despite different names*

### Comparing `telliot_core-0.2.6/src/telliot_core/tellor/tellorflex/token.py` & `telliot_core-0.2.7/src/telliot_core/tellor/tellorflex/token.py`

 * *Files identical despite different names*

### Comparing `telliot_core-0.2.6/src/telliot_core/tellor/tellorx/master.py` & `telliot_core-0.2.7/src/telliot_core/tellor/tellorx/master.py`

 * *Files identical despite different names*

### Comparing `telliot_core-0.2.6/src/telliot_core/tellor/tellorx/oracle.py` & `telliot_core-0.2.7/src/telliot_core/tellor/tellorx/oracle.py`

 * *Files identical despite different names*

### Comparing `telliot_core-0.2.6/src/telliot_core/utils/home.py` & `telliot_core-0.2.7/src/telliot_core/utils/home.py`

 * *Files identical despite different names*

### Comparing `telliot_core-0.2.6/src/telliot_core/utils/key_helpers.py` & `telliot_core-0.2.7/src/telliot_core/utils/key_helpers.py`

 * *Files identical despite different names*

### Comparing `telliot_core-0.2.6/src/telliot_core/utils/response.py` & `telliot_core-0.2.7/src/telliot_core/utils/response.py`

 * *Files identical despite different names*

### Comparing `telliot_core-0.2.6/src/telliot_core/utils/timestamp.py` & `telliot_core-0.2.7/src/telliot_core/utils/timestamp.py`

 * *Files identical despite different names*

### Comparing `telliot_core-0.2.6/src/telliot_core/utils/versions.py` & `telliot_core-0.2.7/src/telliot_core/utils/versions.py`

 * *Files identical despite different names*

### Comparing `telliot_core-0.2.6/src/telliot_core.egg-info/PKG-INFO` & `telliot_core-0.2.7/src/telliot_core.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: telliot-core
-Version: 0.2.6
+Version: 0.2.7
 Summary: Telliot is a Python framework for interacting with the decentralized TellorX network.
 Home-page: https://github.com/tellor-io/telliot-core
 Author: Tellor Development Community
 Author-email: info@tellor.io
 License: MIT
 Keywords: oracle,etherium,blockchain
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `telliot_core-0.2.6/src/telliot_core.egg-info/SOURCES.txt` & `telliot_core-0.2.7/src/telliot_core.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `telliot_core-0.2.6/tests/conftest.py` & `telliot_core-0.2.7/tests/conftest.py`

 * *Files 8% similar despite different names*

```diff
@@ -115,30 +115,7 @@
 def mumbai_test_cfg(scope="session", autouse=True):
     return local_node_cfg(chain_id=80001)
 
 
 @pytest.fixture
 def rinkeby_test_cfg(scope="session", autouse=True):
     return local_node_cfg(chain_id=4)
-
-
-@pytest.fixture(scope="session", autouse=True)
-def fuse_cfg():
-    """Return a test telliot configuration for use on polygon-mumbai
-
-    If environment variables are defined, they will override the values in config files
-    """
-    cfg = TelliotConfig()
-
-    # Override configuration for fuse testnet
-    cfg.main.chain_id = 122
-
-    accounts = find_accounts(chain_id=122)
-    if not accounts:
-        # Create a test account using PRIVATE_KEY defined on github.
-        key = os.getenv("PRIVATE_KEY", None)
-        if key:
-            ChainedAccount.add("git-fuse-key", chains=122, key=os.environ["PRIVATE_KEY"], password="")
-        else:
-            raise Exception("Need a Fuse account")
-
-    return cfg
```

### Comparing `telliot_core-0.2.6/tests/test_app_core.py` & `telliot_core-0.2.7/tests/test_app_core.py`

 * *Files identical despite different names*

### Comparing `telliot_core-0.2.6/tests/test_autopay.py` & `telliot_core-0.2.7/tests/test_autopay.py`

 * *Files identical despite different names*

### Comparing `telliot_core-0.2.6/tests/test_cli.py` & `telliot_core-0.2.7/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `telliot_core-0.2.6/tests/test_config.py` & `telliot_core-0.2.7/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `telliot_core-0.2.6/tests/test_contract.py` & `telliot_core-0.2.7/tests/test_contract.py`

 * *Files identical despite different names*

### Comparing `telliot_core-0.2.6/tests/test_directory.py` & `telliot_core-0.2.7/tests/test_directory.py`

 * *Files identical despite different names*

### Comparing `telliot_core-0.2.6/tests/test_gas.py` & `telliot_core-0.2.7/tests/test_gas.py`

 * *Files identical despite different names*

### Comparing `telliot_core-0.2.6/tests/test_listener.py` & `telliot_core-0.2.7/tests/test_listener.py`

 * *Files identical despite different names*

### Comparing `telliot_core-0.2.6/tests/test_master_read.py` & `telliot_core-0.2.7/tests/test_master_read.py`

 * *Files identical despite different names*

### Comparing `telliot_core-0.2.6/tests/test_model_chain.py` & `telliot_core-0.2.7/tests/test_model_chain.py`

 * *Files identical despite different names*

### Comparing `telliot_core-0.2.6/tests/test_oracle_read.py` & `telliot_core-0.2.7/tests/test_oracle_read.py`

 * *Files identical despite different names*

### Comparing `telliot_core-0.2.6/tests/test_rpc_endpoint.py` & `telliot_core-0.2.7/tests/test_rpc_endpoint.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
 Tests covering Pytelliot rpc connection  utils.
 """
 import pytest
-import requests
 from brownie import chain
+from requests.exceptions import HTTPError
 
 from telliot_core.model.endpoints import EndpointList
 from telliot_core.model.endpoints import RPCEndpoint
 
 network = "mainnet"
 provider = "pokt"
 
@@ -32,15 +32,15 @@
 
 
 def test_incomplete_rpc_url():
     """an incomplete url will raise an exception in RPCEndpoint"""
     url = "https://eth-rinkeby.gateway.pokt.network/v1/lb/"
     endpt = RPCEndpoint(network=network, provider=provider, url=url)
     # expect bad url error from requests library
-    with pytest.raises(requests.exceptions.HTTPError):
+    with pytest.raises(HTTPError):
         _ = endpt.connect()
 
 
 def test_endpoint_list():
     sl = EndpointList()
     # print(json.dumps(sl.get_state(), indent=2))
     ep4 = sl.find(chain_id=4)[0]
```

### Comparing `telliot_core-0.2.6/tests/test_session_manager.py` & `telliot_core-0.2.7/tests/test_session_manager.py`

 * *Files identical despite different names*

### Comparing `telliot_core-0.2.6/tests/test_telliot_config.py` & `telliot_core-0.2.7/tests/test_telliot_config.py`

 * *Files identical despite different names*

### Comparing `telliot_core-0.2.6/tests/test_tellorflex.py` & `telliot_core-0.2.7/tests/test_tellorflex.py`

 * *Files identical despite different names*

### Comparing `telliot_core-0.2.6/tests/test_token.py` & `telliot_core-0.2.7/tests/test_token.py`

 * *Files identical despite different names*

### Comparing `telliot_core-0.2.6/tox.ini` & `telliot_core-0.2.7/tox.ini`

 * *Files identical despite different names*

