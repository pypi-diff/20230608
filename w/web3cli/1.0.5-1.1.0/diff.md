# Comparing `tmp/web3cli-1.0.5.tar.gz` & `tmp/web3cli-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "web3cli-1.0.5.tar", last modified: Wed Jun  7 17:20:13 2023, max compression
+gzip compressed data, was "web3cli-1.1.0.tar", last modified: Thu Jun  8 18:16:53 2023, max compression
```

## Comparing `web3cli-1.0.5.tar` & `web3cli-1.1.0.tar`

### file list

```diff
@@ -1,170 +1,171 @@
--rw-r--r--   0        0        0     1069 2022-10-24 15:49:55.999119 web3cli-1.0.5/LICENSE
--rw-r--r--   0        0        0    11246 2023-06-07 17:19:26.093594 web3cli-1.0.5/README.md
--rw-r--r--   0        0        0     3891 2023-06-07 17:20:01.229192 web3cli-1.0.5/pyproject.toml
--rw-r--r--   0        0        0     6148 2022-11-13 07:56:22.807127 web3cli-1.0.5/src/web3cli/.DS_Store
--rw-r--r--   0        0        0        0 2022-11-18 22:32:14.016225 web3cli-1.0.5/src/web3cli/__init__.py
--rw-r--r--   0        0        0        0 2022-10-24 15:34:40.198985 web3cli-1.0.5/src/web3cli/controllers/__init__.py
--rw-r--r--   0        0        0     4699 2023-05-20 18:26:40.921508 web3cli-1.0.5/src/web3cli/controllers/abi_controller.py
--rw-r--r--   0        0        0     2005 2023-05-17 11:19:52.195517 web3cli-1.0.5/src/web3cli/controllers/app_key_controller.py
--rw-r--r--   0        0        0     1171 2023-05-20 18:17:47.037441 web3cli-1.0.5/src/web3cli/controllers/base_controller.py
--rw-r--r--   0        0        0     3116 2023-05-20 18:17:47.038161 web3cli-1.0.5/src/web3cli/controllers/call_controller.py
--rw-r--r--   0        0        0     2372 2023-05-20 18:17:47.039146 web3cli-1.0.5/src/web3cli/controllers/config_controller.py
--rw-r--r--   0        0        0     1109 2022-12-17 18:21:46.704206 web3cli-1.0.5/src/web3cli/controllers/controller.py
--rw-r--r--   0        0        0        0 2023-03-25 21:06:13.922427 web3cli-1.0.5/src/web3cli/controllers/crud/__init__.py
--rw-r--r--   0        0        0     2540 2023-05-20 18:17:47.040161 web3cli-1.0.5/src/web3cli/controllers/crud/address_controller.py
--rw-r--r--   0        0        0     4421 2023-05-26 15:30:25.886766 web3cli-1.0.5/src/web3cli/controllers/crud/chain_controller.py
--rw-r--r--   0        0        0     4795 2023-05-31 08:43:28.096742 web3cli-1.0.5/src/web3cli/controllers/crud/contract_controller.py
--rw-r--r--   0        0        0     3052 2023-05-20 18:17:47.042307 web3cli-1.0.5/src/web3cli/controllers/crud/history_controller.py
--rw-r--r--   0        0        0     2958 2023-05-20 18:17:47.043048 web3cli-1.0.5/src/web3cli/controllers/crud/rpc_controller.py
--rw-r--r--   0        0        0     5286 2023-05-20 18:17:47.043661 web3cli-1.0.5/src/web3cli/controllers/crud/signer_controller.py
--rw-r--r--   0        0        0     1346 2023-04-30 17:34:17.185968 web3cli-1.0.5/src/web3cli/controllers/db_controller.py
--rw-r--r--   0        0        0     1433 2023-05-18 10:41:28.547083 web3cli-1.0.5/src/web3cli/controllers/keyfile_controller.py
--rw-r--r--   0        0        0     4330 2023-05-31 11:18:25.258680 web3cli-1.0.5/src/web3cli/controllers/misc_controller.py
--rw-r--r--   0        0        0     4191 2023-06-07 17:09:12.321376 web3cli-1.0.5/src/web3cli/controllers/replay_controller.py
--rw-r--r--   0        0        0     2359 2023-05-20 18:17:47.045353 web3cli-1.0.5/src/web3cli/controllers/send_controller.py
--rw-r--r--   0        0        0     6878 2023-05-20 18:17:47.046015 web3cli-1.0.5/src/web3cli/controllers/swap_controller.py
--rw-r--r--   0        0        0     6759 2023-05-31 08:57:39.106511 web3cli-1.0.5/src/web3cli/controllers/token_controller.py
--rw-r--r--   0        0        0     2862 2023-05-20 18:17:47.047364 web3cli-1.0.5/src/web3cli/controllers/transact_controller.py
--rw-r--r--   0        0        0     1408 2023-06-07 17:07:38.026919 web3cli-1.0.5/src/web3cli/controllers/tx_controller.py
--rw-r--r--   0        0        0      341 2023-05-20 18:17:47.049010 web3cli-1.0.5/src/web3cli/exceptions.py
--rw-r--r--   0        0        0        0 2022-10-24 15:34:40.191413 web3cli-1.0.5/src/web3cli/helpers/__init__.py
--rw-r--r--   0        0        0    15889 2023-05-20 18:17:47.050167 web3cli-1.0.5/src/web3cli/helpers/args.py
--rw-r--r--   0        0        0     2198 2023-05-20 18:17:47.051274 web3cli-1.0.5/src/web3cli/helpers/client_factory.py
--rw-r--r--   0        0        0     1252 2022-12-28 16:44:58.644508 web3cli-1.0.5/src/web3cli/helpers/config.py
--rw-r--r--   0        0        0     2092 2023-05-18 11:14:15.678582 web3cli-1.0.5/src/web3cli/helpers/crypto.py
--rw-r--r--   0        0        0     1228 2023-02-11 17:24:24.959766 web3cli-1.0.5/src/web3cli/helpers/database.py
--rw-r--r--   0        0        0     1704 2023-06-07 16:28:34.402212 web3cli-1.0.5/src/web3cli/helpers/render.py
--rw-r--r--   0        0        0     4548 2023-06-07 12:09:20.814550 web3cli-1.0.5/src/web3cli/helpers/send.py
--rw-r--r--   0        0        0     2178 2023-05-20 18:17:47.053233 web3cli-1.0.5/src/web3cli/helpers/signer.py
--rw-r--r--   0        0        0     2132 2023-06-07 12:22:03.729729 web3cli-1.0.5/src/web3cli/helpers/tx.py
--rw-r--r--   0        0        0      435 2023-06-07 17:19:55.986398 web3cli-1.0.5/src/web3cli/helpers/version.py
--rw-r--r--   0        0        0     2595 2023-02-12 21:33:06.910919 web3cli-1.0.5/src/web3cli/hooks.py
--rw-r--r--   0        0        0     7221 2023-06-07 17:09:36.844399 web3cli-1.0.5/src/web3cli/main.py
--rw-r--r--   0        0        0        0 2023-01-29 11:30:42.897043 web3cli-1.0.5/src/web3cli/templates/__init__.py
--rw-r--r--   0        0        0      243 2023-01-29 11:41:03.173746 web3cli-1.0.5/src/web3cli/templates/balance.jinja2
--rw-r--r--   0        0        0      120 2022-11-03 17:39:28.958124 web3cli-1.0.5/src/web3core/__init__.py
--rw-r--r--   0        0        0       72 2023-02-19 11:02:13.393953 web3cli-1.0.5/src/web3core/constants.py
--rw-r--r--   0        0        0       90 2023-01-18 19:29:57.558367 web3cli-1.0.5/src/web3core/db.py
--rw-r--r--   0        0        0     1762 2023-01-18 20:41:45.295870 web3cli-1.0.5/src/web3core/exceptions.py
--rw-r--r--   0        0        0        0 2022-11-03 17:39:28.958845 web3cli-1.0.5/src/web3core/helpers/__init__.py
--rw-r--r--   0        0        0     9448 2023-04-07 18:14:01.618698 web3cli-1.0.5/src/web3core/helpers/abi.py
--rw-r--r--   0        0        0     1148 2023-05-17 09:47:21.910041 web3cli-1.0.5/src/web3core/helpers/blocks.py
--rw-r--r--   0        0        0     3405 2023-05-20 18:17:47.055119 web3cli-1.0.5/src/web3core/helpers/client_factory.py
--rw-r--r--   0        0        0     1060 2022-12-17 18:21:46.707584 web3cli-1.0.5/src/web3core/helpers/crypto.py
--rw-r--r--   0        0        0      714 2023-02-11 17:32:11.986925 web3cli-1.0.5/src/web3core/helpers/database.py
--rw-r--r--   0        0        0     1582 2023-04-07 18:14:01.619156 web3cli-1.0.5/src/web3core/helpers/dex.py
--rw-r--r--   0        0        0      434 2022-12-19 20:01:36.985004 web3cli-1.0.5/src/web3core/helpers/format.py
--rw-r--r--   0        0        0     2413 2023-05-18 08:42:25.689036 web3cli-1.0.5/src/web3core/helpers/misc.py
--rw-r--r--   0        0        0      532 2022-12-16 06:48:29.391730 web3cli-1.0.5/src/web3core/helpers/os.py
--rw-r--r--   0        0        0     1790 2023-04-07 18:14:01.619658 web3cli-1.0.5/src/web3core/helpers/resolve.py
--rw-r--r--   0        0        0      515 2022-12-17 18:21:46.708465 web3cli-1.0.5/src/web3core/helpers/rpc.py
--rw-r--r--   0        0        0     2158 2023-01-14 21:27:16.459461 web3cli-1.0.5/src/web3core/helpers/seed.py
--rw-r--r--   0        0        0     4697 2023-04-07 18:14:01.620145 web3cli-1.0.5/src/web3core/helpers/tx.py
--rw-r--r--   0        0        0      345 2023-01-29 18:12:45.184768 web3cli-1.0.5/src/web3core/helpers/validation.py
--rw-r--r--   0        0        0     1207 2022-12-28 16:44:58.644659 web3cli-1.0.5/src/web3core/helpers/yaml.py
--rw-r--r--   0        0        0      424 2023-01-18 19:29:57.562778 web3cli-1.0.5/src/web3core/models/__init__.py
--rw-r--r--   0        0        0     1790 2023-01-18 19:29:57.563744 web3cli-1.0.5/src/web3core/models/address.py
--rw-r--r--   0        0        0     3433 2023-05-20 18:17:47.055757 web3cli-1.0.5/src/web3core/models/base_model.py
--rw-r--r--   0        0        0     4923 2023-03-25 21:22:51.453293 web3cli-1.0.5/src/web3core/models/chain.py
--rw-r--r--   0        0        0     4262 2023-05-31 08:53:51.850966 web3cli-1.0.5/src/web3core/models/contract.py
--rw-r--r--   0        0        0     1405 2023-05-18 09:25:11.305140 web3cli-1.0.5/src/web3core/models/signer.py
--rw-r--r--   0        0        0     1054 2022-12-28 16:44:59.161817 web3cli-1.0.5/src/web3core/models/timestamps_model.py
--rw-r--r--   0        0        0     2550 2022-12-28 16:44:59.162568 web3cli-1.0.5/src/web3core/models/tx.py
--rw-r--r--   0        0        0     1449 2023-01-18 19:29:57.566552 web3cli-1.0.5/src/web3core/models/types.py
--rw-r--r--   0        0        0       48 2022-11-18 22:43:37.360850 web3cli-1.0.5/src/web3core/seeds/__init__.py
--rw-r--r--   0        0        0     3071 2023-05-26 15:12:06.303278 web3cli-1.0.5/src/web3core/seeds/chain_seeds.py
--rw-r--r--   0        0        0      466 2023-05-26 15:26:11.248665 web3cli-1.0.5/src/web3core/seeds/contract_seeds.py
--rw-r--r--   0        0        0    49489 2023-02-19 09:09:21.024661 web3cli-1.0.5/src/web3core/seeds/contract_type_seeds.py
--rw-r--r--   0        0        0     9720 2023-02-27 16:48:07.675984 web3cli-1.0.5/src/web3core/seeds/contracts/arb_contract_seeds.py
--rw-r--r--   0        0        0     1881 2023-02-27 19:24:54.136969 web3cli-1.0.5/src/web3core/seeds/contracts/avax_contract_seeds.py
--rw-r--r--   0        0        0      480 2023-02-27 16:48:16.132079 web3cli-1.0.5/src/web3core/seeds/contracts/bnb_contract_seeds.py
--rw-r--r--   0        0        0      611 2023-05-25 15:43:35.647237 web3cli-1.0.5/src/web3core/seeds/contracts/era_contract_seeds.py
--rw-r--r--   0        0        0     1579 2023-02-27 16:48:24.467166 web3cli-1.0.5/src/web3core/seeds/contracts/eth_contract_seeds.py
--rw-r--r--   0        0        0     1183 2023-05-26 15:20:05.535496 web3cli-1.0.5/src/web3core/seeds/contracts/gno_contract_seeds.py
--rw-r--r--   0        0        0     1448 2023-02-19 10:37:03.165028 web3cli-1.0.5/src/web3core/types.py
--rw-r--r--   0        0        0     6148 2023-02-28 16:18:46.901853 web3cli-1.0.5/tests/.DS_Store
--rw-r--r--   0        0        0        0 2022-11-10 21:50:51.296564 web3cli-1.0.5/tests/__init__.py
--rw-r--r--   0        0        0    10244 2023-02-28 16:18:44.627516 web3cli-1.0.5/tests/ape/.DS_Store
--rw-r--r--   0        0        0     2609 2023-04-06 17:43:03.934034 web3cli-1.0.5/tests/ape/.build/Factory_IERC20.json
--rw-r--r--   0        0        0      536 2023-04-06 17:43:03.934442 web3cli-1.0.5/tests/ape/.build/Factory_IUniswapV2Callee.json
--rw-r--r--   0        0        0     3605 2023-04-06 17:43:03.935802 web3cli-1.0.5/tests/ape/.build/Factory_IUniswapV2ERC20.json
--rw-r--r--   0        0        0     2026 2023-04-06 17:43:03.936651 web3cli-1.0.5/tests/ape/.build/Factory_IUniswapV2Factory.json
--rw-r--r--   0        0        0     7527 2023-04-06 17:43:03.938968 web3cli-1.0.5/tests/ape/.build/Factory_IUniswapV2Pair.json
--rw-r--r--   0        0        0      862 2023-04-06 17:43:03.939241 web3cli-1.0.5/tests/ape/.build/Factory_Math.json
--rw-r--r--   0        0        0      866 2023-04-06 17:43:03.939527 web3cli-1.0.5/tests/ape/.build/Factory_SafeMath.json
--rw-r--r--   0        0        0      867 2023-04-06 17:43:03.939780 web3cli-1.0.5/tests/ape/.build/Factory_UQ112x112.json
--rw-r--r--   0        0        0     2609 2023-04-06 17:43:03.916870 web3cli-1.0.5/tests/ape/.build/Router_IERC20.json
--rw-r--r--   0        0        0     2026 2023-04-06 17:43:03.917744 web3cli-1.0.5/tests/ape/.build/Router_IUniswapV2Factory.json
--rw-r--r--   0        0        0     7527 2023-04-06 17:43:03.920204 web3cli-1.0.5/tests/ape/.build/Router_IUniswapV2Pair.json
--rw-r--r--   0        0        0     9213 2023-04-06 17:43:03.922797 web3cli-1.0.5/tests/ape/.build/Router_IUniswapV2Router01.json
--rw-r--r--   0        0        0    11845 2023-04-06 17:43:03.926066 web3cli-1.0.5/tests/ape/.build/Router_IUniswapV2Router02.json
--rw-r--r--   0        0        0      683 2023-04-06 17:43:03.926558 web3cli-1.0.5/tests/ape/.build/Router_IWETH.json
--rw-r--r--   0        0        0      872 2023-04-06 17:43:03.926867 web3cli-1.0.5/tests/ape/.build/Router_SafeMath.json
--rw-r--r--   0        0        0      879 2023-04-06 17:43:03.927162 web3cli-1.0.5/tests/ape/.build/Router_TransferHelper.json
--rw-r--r--   0        0        0      881 2023-04-06 17:43:03.927462 web3cli-1.0.5/tests/ape/.build/Router_UniswapV2Library.json
--rw-r--r--   0        0        0    14895 2023-04-06 17:43:03.932635 web3cli-1.0.5/tests/ape/.build/Token.json
--rw-r--r--   0        0        0      791 2023-04-06 17:43:03.932974 web3cli-1.0.5/tests/ape/.build/Token_SafeMath.json
--rw-r--r--   0        0        0    14014 2023-04-06 17:43:03.941015 web3cli-1.0.5/tests/ape/.build/UniswapV2ERC20.json
--rw-r--r--   0        0        0    46097 2023-04-06 17:43:03.942289 web3cli-1.0.5/tests/ape/.build/UniswapV2Factory.json
--rw-r--r--   0        0        0    44784 2023-04-06 17:43:03.944616 web3cli-1.0.5/tests/ape/.build/UniswapV2Pair.json
--rw-r--r--   0        0        0    85730 2023-04-06 17:43:03.931232 web3cli-1.0.5/tests/ape/.build/UniswapV2Router02.json
--rw-r--r--   0        0        0   324962 2023-06-07 17:20:01.143842 web3cli-1.0.5/tests/ape/.build/__local__.json
--rw-r--r--   0        0        0        0 2023-04-07 18:14:01.620721 web3cli-1.0.5/tests/ape/__init__.py
--rw-r--r--   0        0        0     6148 2023-02-28 16:18:44.554061 web3cli-1.0.5/tests/ape/contracts/.DS_Store
--rw-r--r--   0        0        0     4101 2023-04-07 18:14:01.621230 web3cli-1.0.5/tests/ape/contracts/token/Token.sol
--rw-r--r--   0        0        0      646 2023-04-07 18:14:01.621775 web3cli-1.0.5/tests/ape/contracts/token/Token_SafeMath.sol
--rw-r--r--   0        0        0     6148 2023-02-28 15:31:57.501753 web3cli-1.0.5/tests/ape/contracts/uniswap/.DS_Store
--rw-r--r--   0        0        0    21725 2023-04-07 18:14:01.622322 web3cli-1.0.5/tests/ape/contracts/uniswap/UniswapV2Factory.sol
--rw-r--r--   0        0        0    34078 2023-04-07 18:14:01.622848 web3cli-1.0.5/tests/ape/contracts/uniswap/UniswapV2Router02.sol
--rw-r--r--   0        0        0      236 2023-04-07 18:14:01.623357 web3cli-1.0.5/tests/ape/scripts/__init__.py
--rw-r--r--   0        0        0      347 2023-04-07 18:14:01.623719 web3cli-1.0.5/tests/ape/scripts/db.py
--rw-r--r--   0        0        0      200 2023-04-07 18:14:01.624050 web3cli-1.0.5/tests/ape/scripts/token.py
--rw-r--r--   0        0        0        0 2023-04-07 18:14:01.624201 web3cli-1.0.5/tests/ape/tests/__init__.py
--rw-r--r--   0        0        0    13902 2023-04-07 18:14:01.624793 web3cli-1.0.5/tests/ape/tests/fixtures.py
--rw-r--r--   0        0        0        0 2023-04-07 18:14:01.624997 web3cli-1.0.5/tests/ape/tests/helpers/__init__.py
--rw-r--r--   0        0        0      371 2023-04-07 18:14:01.625481 web3cli-1.0.5/tests/ape/tests/helpers/ape.py
--rw-r--r--   0        0        0      881 2023-04-07 18:14:01.625860 web3cli-1.0.5/tests/ape/tests/helpers/token.py
--rw-r--r--   0        0        0     3790 2023-04-07 18:14:01.626436 web3cli-1.0.5/tests/ape/tests/helpers/uniswap.py
--rw-r--r--   0        0        0        0 2023-04-07 18:14:01.626729 web3cli-1.0.5/tests/ape/tests/token/__init__.py
--rw-r--r--   0        0        0     1983 2023-04-07 18:14:01.627373 web3cli-1.0.5/tests/ape/tests/token/test_token_approve.py
--rw-r--r--   0        0        0     2876 2023-04-07 18:14:01.627765 web3cli-1.0.5/tests/ape/tests/token/test_token_transfer.py
--rw-r--r--   0        0        0     6467 2023-04-07 18:14:01.628071 web3cli-1.0.5/tests/ape/tests/token/test_token_transferFrom.py
--rw-r--r--   0        0        0        0 2023-04-07 18:14:01.628193 web3cli-1.0.5/tests/ape/tests/uniswap/__init__.py
--rw-r--r--   0        0        0     4193 2023-04-07 18:14:01.628531 web3cli-1.0.5/tests/ape/tests/uniswap/test_v2_add_liquidity.py
--rw-r--r--   0        0        0      794 2023-04-07 18:14:01.628890 web3cli-1.0.5/tests/ape/tests/uniswap/test_v2_create_pair.py
--rw-r--r--   0        0        0      487 2023-04-07 18:14:01.629400 web3cli-1.0.5/tests/conftest.py
--rw-r--r--   0        0        0     1130 2023-04-07 12:55:47.114434 web3cli-1.0.5/tests/helper.py
--rw-r--r--   0        0        0     3240 2023-04-07 18:14:01.629815 web3cli-1.0.5/tests/seed.py
--rw-r--r--   0        0        0        0 2022-12-28 17:01:25.438908 web3cli-1.0.5/tests/web3cli/__init__.py
--rw-r--r--   0        0        0        0 2022-11-10 21:50:51.297637 web3cli-1.0.5/tests/web3cli/controllers/__init__.py
--rw-r--r--   0        0        0     3754 2023-05-20 18:17:47.056601 web3cli-1.0.5/tests/web3cli/controllers/crud/test_address_controller.py
--rw-r--r--   0        0        0     3517 2023-05-20 18:17:47.057300 web3cli-1.0.5/tests/web3cli/controllers/crud/test_chain_controller.py
--rw-r--r--   0        0        0     8222 2023-05-20 18:17:47.058165 web3cli-1.0.5/tests/web3cli/controllers/crud/test_contract_controller.py
--rw-r--r--   0        0        0     2870 2023-05-20 18:17:47.058996 web3cli-1.0.5/tests/web3cli/controllers/crud/test_history_controller.py
--rw-r--r--   0        0        0     3762 2023-05-20 18:17:47.059822 web3cli-1.0.5/tests/web3cli/controllers/crud/test_rpc_controller.py
--rw-r--r--   0        0        0     4933 2023-05-20 18:17:47.060483 web3cli-1.0.5/tests/web3cli/controllers/crud/test_signer_controller.py
--rw-r--r--   0        0        0     3235 2023-05-31 09:02:25.228686 web3cli-1.0.5/tests/web3cli/controllers/crud/test_token_controller.py
--rw-r--r--   0        0        0     1848 2023-05-18 10:32:19.351291 web3cli-1.0.5/tests/web3cli/controllers/test_appkey_controller.py
--rw-r--r--   0        0        0     6339 2023-05-20 18:17:47.061301 web3cli-1.0.5/tests/web3cli/controllers/test_call_controller.py
--rw-r--r--   0        0        0     1041 2023-03-25 21:24:05.581746 web3cli-1.0.5/tests/web3cli/controllers/test_db_controller.py
--rw-r--r--   0        0        0     1702 2023-05-18 11:14:40.025134 web3cli-1.0.5/tests/web3cli/controllers/test_keyfile_controller.py
--rw-r--r--   0        0        0     6099 2023-05-31 11:22:03.092128 web3cli-1.0.5/tests/web3cli/controllers/test_misc_controller.py
--rw-r--r--   0        0        0     1210 2023-06-07 17:12:04.381111 web3cli-1.0.5/tests/web3cli/controllers/test_replay_controller.py
--rw-r--r--   0        0        0     3415 2023-05-20 18:17:47.063638 web3cli-1.0.5/tests/web3cli/controllers/test_send_controller.py
--rw-r--r--   0        0        0     9593 2023-05-20 18:17:47.064509 web3cli-1.0.5/tests/web3cli/controllers/test_transact_controller.py
--rw-r--r--   0        0        0     1265 2023-06-07 17:10:04.508480 web3cli-1.0.5/tests/web3cli/controllers/test_tx_controller.py
--rw-r--r--   0        0        0     1293 2023-04-07 18:14:01.632176 web3cli-1.0.5/tests/web3cli/fixtures.py
--rw-r--r--   0        0        0        0 2022-11-10 21:50:51.303802 web3cli-1.0.5/tests/web3cli/helpers/__init__.py
--rw-r--r--   0        0        0      684 2022-12-28 17:00:06.651527 web3cli-1.0.5/tests/web3cli/helpers/test_crypto_helper.py
--rw-r--r--   0        0        0     1455 2023-02-12 12:11:39.416778 web3cli-1.0.5/tests/web3cli/main.py
--rw-r--r--   0        0        0     1171 2023-02-11 18:15:39.713968 web3cli-1.0.5/tests/web3cli/test_db.py
--rw-r--r--   0        0        0      393 2023-02-11 18:16:36.584225 web3cli-1.0.5/tests/web3cli/test_main.py
--rw-r--r--   0        0        0        0 2022-11-10 21:50:51.301380 web3cli-1.0.5/tests/web3core/__init__.py
--rw-r--r--   0        0        0     5362 2023-05-18 11:01:18.894137 web3cli-1.0.5/tests/web3core/fixtures.py
--rw-r--r--   0        0        0        0 2022-11-10 21:50:51.301610 web3cli-1.0.5/tests/web3core/helpers/__init__.py
--rw-r--r--   0        0        0     8923 2023-01-28 12:36:51.002666 web3cli-1.0.5/tests/web3core/helpers/test_abi_helper.py
--rw-r--r--   0        0        0      528 2022-12-28 16:44:57.745951 web3cli-1.0.5/tests/web3core/helpers/test_crypto_helper.py
--rw-r--r--   0        0        0     4807 2023-02-19 09:09:21.027684 web3cli-1.0.5/tests/web3core/helpers/test_resolve_address_helper.py
--rw-r--r--   0        0        0     1022 2023-01-29 17:56:31.054122 web3cli-1.0.5/tests/web3core/helpers/test_validation_helper.py
--rw-r--r--   0        0        0     1783 2023-01-14 21:27:16.475375 web3cli-1.0.5/tests/web3core/models/test_contract_model.py
--rw-r--r--   0        0        0    11703 1970-01-01 00:00:00.000000 web3cli-1.0.5/PKG-INFO
+-rw-r--r--   0        0        0     1069 2022-10-24 15:49:55.999119 web3cli-1.1.0/LICENSE
+-rw-r--r--   0        0        0    11240 2023-06-07 17:21:32.607065 web3cli-1.1.0/README.md
+-rw-r--r--   0        0        0     4026 2023-06-08 18:16:41.983226 web3cli-1.1.0/pyproject.toml
+-rw-r--r--   0        0        0     6148 2022-11-13 07:56:22.807127 web3cli-1.1.0/src/web3cli/.DS_Store
+-rw-r--r--   0        0        0        0 2022-11-18 22:32:14.016225 web3cli-1.1.0/src/web3cli/__init__.py
+-rw-r--r--   0        0        0        0 2022-10-24 15:34:40.198985 web3cli-1.1.0/src/web3cli/controllers/__init__.py
+-rw-r--r--   0        0        0     4699 2023-05-20 18:26:40.921508 web3cli-1.1.0/src/web3cli/controllers/abi_controller.py
+-rw-r--r--   0        0        0     2005 2023-05-17 11:19:52.195517 web3cli-1.1.0/src/web3cli/controllers/app_key_controller.py
+-rw-r--r--   0        0        0     1171 2023-05-20 18:17:47.037441 web3cli-1.1.0/src/web3cli/controllers/base_controller.py
+-rw-r--r--   0        0        0     3116 2023-05-20 18:17:47.038161 web3cli-1.1.0/src/web3cli/controllers/call_controller.py
+-rw-r--r--   0        0        0     2372 2023-05-20 18:17:47.039146 web3cli-1.1.0/src/web3cli/controllers/config_controller.py
+-rw-r--r--   0        0        0     1109 2022-12-17 18:21:46.704206 web3cli-1.1.0/src/web3cli/controllers/controller.py
+-rw-r--r--   0        0        0        0 2023-03-25 21:06:13.922427 web3cli-1.1.0/src/web3cli/controllers/crud/__init__.py
+-rw-r--r--   0        0        0     2540 2023-05-20 18:17:47.040161 web3cli-1.1.0/src/web3cli/controllers/crud/address_controller.py
+-rw-r--r--   0        0        0     4421 2023-05-26 15:30:25.886766 web3cli-1.1.0/src/web3cli/controllers/crud/chain_controller.py
+-rw-r--r--   0        0        0     4795 2023-05-31 08:43:28.096742 web3cli-1.1.0/src/web3cli/controllers/crud/contract_controller.py
+-rw-r--r--   0        0        0     3052 2023-05-20 18:17:47.042307 web3cli-1.1.0/src/web3cli/controllers/crud/history_controller.py
+-rw-r--r--   0        0        0     2958 2023-05-20 18:17:47.043048 web3cli-1.1.0/src/web3cli/controllers/crud/rpc_controller.py
+-rw-r--r--   0        0        0     5286 2023-05-20 18:17:47.043661 web3cli-1.1.0/src/web3cli/controllers/crud/signer_controller.py
+-rw-r--r--   0        0        0     1346 2023-04-30 17:34:17.185968 web3cli-1.1.0/src/web3cli/controllers/db_controller.py
+-rw-r--r--   0        0        0     1433 2023-05-18 10:41:28.547083 web3cli-1.1.0/src/web3cli/controllers/keyfile_controller.py
+-rw-r--r--   0        0        0     4330 2023-05-31 11:18:25.258680 web3cli-1.1.0/src/web3cli/controllers/misc_controller.py
+-rw-r--r--   0        0        0     4461 2023-06-08 17:37:43.908413 web3cli-1.1.0/src/web3cli/controllers/replay_controller.py
+-rw-r--r--   0        0        0     2359 2023-05-20 18:17:47.045353 web3cli-1.1.0/src/web3cli/controllers/send_controller.py
+-rw-r--r--   0        0        0     6878 2023-05-20 18:17:47.046015 web3cli-1.1.0/src/web3cli/controllers/swap_controller.py
+-rw-r--r--   0        0        0     7872 2023-06-08 18:14:50.319839 web3cli-1.1.0/src/web3cli/controllers/token_controller.py
+-rw-r--r--   0        0        0     2862 2023-05-20 18:17:47.047364 web3cli-1.1.0/src/web3cli/controllers/transact_controller.py
+-rw-r--r--   0        0        0     1408 2023-06-07 17:07:38.026919 web3cli-1.1.0/src/web3cli/controllers/tx_controller.py
+-rw-r--r--   0        0        0      341 2023-05-20 18:17:47.049010 web3cli-1.1.0/src/web3cli/exceptions.py
+-rw-r--r--   0        0        0        0 2022-10-24 15:34:40.191413 web3cli-1.1.0/src/web3cli/helpers/__init__.py
+-rw-r--r--   0        0        0    15889 2023-05-20 18:17:47.050167 web3cli-1.1.0/src/web3cli/helpers/args.py
+-rw-r--r--   0        0        0     2198 2023-05-20 18:17:47.051274 web3cli-1.1.0/src/web3cli/helpers/client_factory.py
+-rw-r--r--   0        0        0     1252 2022-12-28 16:44:58.644508 web3cli-1.1.0/src/web3cli/helpers/config.py
+-rw-r--r--   0        0        0     2092 2023-05-18 11:14:15.678582 web3cli-1.1.0/src/web3cli/helpers/crypto.py
+-rw-r--r--   0        0        0     1228 2023-02-11 17:24:24.959766 web3cli-1.1.0/src/web3cli/helpers/database.py
+-rw-r--r--   0        0        0     1774 2023-06-08 18:15:33.914193 web3cli-1.1.0/src/web3cli/helpers/render.py
+-rw-r--r--   0        0        0     4548 2023-06-07 12:09:20.814550 web3cli-1.1.0/src/web3cli/helpers/send.py
+-rw-r--r--   0        0        0     2178 2023-05-20 18:17:47.053233 web3cli-1.1.0/src/web3cli/helpers/signer.py
+-rw-r--r--   0        0        0     2132 2023-06-07 12:22:03.729729 web3cli-1.1.0/src/web3cli/helpers/tx.py
+-rw-r--r--   0        0        0      435 2023-06-08 18:16:07.880013 web3cli-1.1.0/src/web3cli/helpers/version.py
+-rw-r--r--   0        0        0     2595 2023-02-12 21:33:06.910919 web3cli-1.1.0/src/web3cli/hooks.py
+-rw-r--r--   0        0        0     7358 2023-06-08 14:37:45.655105 web3cli-1.1.0/src/web3cli/main.py
+-rw-r--r--   0        0        0        0 2023-01-29 11:30:42.897043 web3cli-1.1.0/src/web3cli/templates/__init__.py
+-rw-r--r--   0        0        0      243 2023-01-29 11:41:03.173746 web3cli-1.1.0/src/web3cli/templates/balance.jinja2
+-rw-r--r--   0        0        0      120 2022-11-03 17:39:28.958124 web3cli-1.1.0/src/web3core/__init__.py
+-rw-r--r--   0        0        0       72 2023-02-19 11:02:13.393953 web3cli-1.1.0/src/web3core/constants.py
+-rw-r--r--   0        0        0       90 2023-01-18 19:29:57.558367 web3cli-1.1.0/src/web3core/db.py
+-rw-r--r--   0        0        0     1762 2023-01-18 20:41:45.295870 web3cli-1.1.0/src/web3core/exceptions.py
+-rw-r--r--   0        0        0        0 2022-11-03 17:39:28.958845 web3cli-1.1.0/src/web3core/helpers/__init__.py
+-rw-r--r--   0        0        0     9448 2023-04-07 18:14:01.618698 web3cli-1.1.0/src/web3core/helpers/abi.py
+-rw-r--r--   0        0        0     1148 2023-05-17 09:47:21.910041 web3cli-1.1.0/src/web3core/helpers/blocks.py
+-rw-r--r--   0        0        0     3405 2023-05-20 18:17:47.055119 web3cli-1.1.0/src/web3core/helpers/client_factory.py
+-rw-r--r--   0        0        0     1060 2022-12-17 18:21:46.707584 web3cli-1.1.0/src/web3core/helpers/crypto.py
+-rw-r--r--   0        0        0      714 2023-02-11 17:32:11.986925 web3cli-1.1.0/src/web3core/helpers/database.py
+-rw-r--r--   0        0        0     1582 2023-04-07 18:14:01.619156 web3cli-1.1.0/src/web3core/helpers/dex.py
+-rw-r--r--   0        0        0      434 2022-12-19 20:01:36.985004 web3cli-1.1.0/src/web3core/helpers/format.py
+-rw-r--r--   0        0        0     2413 2023-05-18 08:42:25.689036 web3cli-1.1.0/src/web3core/helpers/misc.py
+-rw-r--r--   0        0        0      532 2022-12-16 06:48:29.391730 web3cli-1.1.0/src/web3core/helpers/os.py
+-rw-r--r--   0        0        0     1790 2023-04-07 18:14:01.619658 web3cli-1.1.0/src/web3core/helpers/resolve.py
+-rw-r--r--   0        0        0      515 2022-12-17 18:21:46.708465 web3cli-1.1.0/src/web3core/helpers/rpc.py
+-rw-r--r--   0        0        0     2158 2023-01-14 21:27:16.459461 web3cli-1.1.0/src/web3core/helpers/seed.py
+-rw-r--r--   0        0        0     4697 2023-04-07 18:14:01.620145 web3cli-1.1.0/src/web3core/helpers/tx.py
+-rw-r--r--   0        0        0      345 2023-01-29 18:12:45.184768 web3cli-1.1.0/src/web3core/helpers/validation.py
+-rw-r--r--   0        0        0     1207 2022-12-28 16:44:58.644659 web3cli-1.1.0/src/web3core/helpers/yaml.py
+-rw-r--r--   0        0        0      424 2023-01-18 19:29:57.562778 web3cli-1.1.0/src/web3core/models/__init__.py
+-rw-r--r--   0        0        0     1790 2023-01-18 19:29:57.563744 web3cli-1.1.0/src/web3core/models/address.py
+-rw-r--r--   0        0        0     3433 2023-05-20 18:17:47.055757 web3cli-1.1.0/src/web3core/models/base_model.py
+-rw-r--r--   0        0        0     4923 2023-03-25 21:22:51.453293 web3cli-1.1.0/src/web3core/models/chain.py
+-rw-r--r--   0        0        0     4262 2023-05-31 08:53:51.850966 web3cli-1.1.0/src/web3core/models/contract.py
+-rw-r--r--   0        0        0     1405 2023-05-18 09:25:11.305140 web3cli-1.1.0/src/web3core/models/signer.py
+-rw-r--r--   0        0        0     1054 2022-12-28 16:44:59.161817 web3cli-1.1.0/src/web3core/models/timestamps_model.py
+-rw-r--r--   0        0        0     2550 2022-12-28 16:44:59.162568 web3cli-1.1.0/src/web3core/models/tx.py
+-rw-r--r--   0        0        0     1449 2023-01-18 19:29:57.566552 web3cli-1.1.0/src/web3core/models/types.py
+-rw-r--r--   0        0        0       48 2022-11-18 22:43:37.360850 web3cli-1.1.0/src/web3core/seeds/__init__.py
+-rw-r--r--   0        0        0     3164 2023-06-08 14:39:52.689918 web3cli-1.1.0/src/web3core/seeds/chain_seeds.py
+-rw-r--r--   0        0        0      521 2023-06-08 14:37:27.133219 web3cli-1.1.0/src/web3core/seeds/contract_seeds.py
+-rw-r--r--   0        0        0    49489 2023-02-19 09:09:21.024661 web3cli-1.1.0/src/web3core/seeds/contract_type_seeds.py
+-rw-r--r--   0        0        0     9720 2023-02-27 16:48:07.675984 web3cli-1.1.0/src/web3core/seeds/contracts/arb_contract_seeds.py
+-rw-r--r--   0        0        0     1881 2023-02-27 19:24:54.136969 web3cli-1.1.0/src/web3core/seeds/contracts/avax_contract_seeds.py
+-rw-r--r--   0        0        0      480 2023-02-27 16:48:16.132079 web3cli-1.1.0/src/web3core/seeds/contracts/bnb_contract_seeds.py
+-rw-r--r--   0        0        0      611 2023-05-25 15:43:35.647237 web3cli-1.1.0/src/web3core/seeds/contracts/era_contract_seeds.py
+-rw-r--r--   0        0        0      997 2023-06-08 14:37:20.947238 web3cli-1.1.0/src/web3core/seeds/contracts/erat_contract_seeds.py
+-rw-r--r--   0        0        0     1579 2023-02-27 16:48:24.467166 web3cli-1.1.0/src/web3core/seeds/contracts/eth_contract_seeds.py
+-rw-r--r--   0        0        0     1183 2023-05-26 15:20:05.535496 web3cli-1.1.0/src/web3core/seeds/contracts/gno_contract_seeds.py
+-rw-r--r--   0        0        0     1448 2023-02-19 10:37:03.165028 web3cli-1.1.0/src/web3core/types.py
+-rw-r--r--   0        0        0     6148 2023-02-28 16:18:46.901853 web3cli-1.1.0/tests/.DS_Store
+-rw-r--r--   0        0        0        0 2022-11-10 21:50:51.296564 web3cli-1.1.0/tests/__init__.py
+-rw-r--r--   0        0        0    10244 2023-02-28 16:18:44.627516 web3cli-1.1.0/tests/ape/.DS_Store
+-rw-r--r--   0        0        0     2609 2023-04-06 17:43:03.934034 web3cli-1.1.0/tests/ape/.build/Factory_IERC20.json
+-rw-r--r--   0        0        0      536 2023-04-06 17:43:03.934442 web3cli-1.1.0/tests/ape/.build/Factory_IUniswapV2Callee.json
+-rw-r--r--   0        0        0     3605 2023-04-06 17:43:03.935802 web3cli-1.1.0/tests/ape/.build/Factory_IUniswapV2ERC20.json
+-rw-r--r--   0        0        0     2026 2023-04-06 17:43:03.936651 web3cli-1.1.0/tests/ape/.build/Factory_IUniswapV2Factory.json
+-rw-r--r--   0        0        0     7527 2023-04-06 17:43:03.938968 web3cli-1.1.0/tests/ape/.build/Factory_IUniswapV2Pair.json
+-rw-r--r--   0        0        0      862 2023-04-06 17:43:03.939241 web3cli-1.1.0/tests/ape/.build/Factory_Math.json
+-rw-r--r--   0        0        0      866 2023-04-06 17:43:03.939527 web3cli-1.1.0/tests/ape/.build/Factory_SafeMath.json
+-rw-r--r--   0        0        0      867 2023-04-06 17:43:03.939780 web3cli-1.1.0/tests/ape/.build/Factory_UQ112x112.json
+-rw-r--r--   0        0        0     2609 2023-04-06 17:43:03.916870 web3cli-1.1.0/tests/ape/.build/Router_IERC20.json
+-rw-r--r--   0        0        0     2026 2023-04-06 17:43:03.917744 web3cli-1.1.0/tests/ape/.build/Router_IUniswapV2Factory.json
+-rw-r--r--   0        0        0     7527 2023-04-06 17:43:03.920204 web3cli-1.1.0/tests/ape/.build/Router_IUniswapV2Pair.json
+-rw-r--r--   0        0        0     9213 2023-04-06 17:43:03.922797 web3cli-1.1.0/tests/ape/.build/Router_IUniswapV2Router01.json
+-rw-r--r--   0        0        0    11845 2023-04-06 17:43:03.926066 web3cli-1.1.0/tests/ape/.build/Router_IUniswapV2Router02.json
+-rw-r--r--   0        0        0      683 2023-04-06 17:43:03.926558 web3cli-1.1.0/tests/ape/.build/Router_IWETH.json
+-rw-r--r--   0        0        0      872 2023-04-06 17:43:03.926867 web3cli-1.1.0/tests/ape/.build/Router_SafeMath.json
+-rw-r--r--   0        0        0      879 2023-04-06 17:43:03.927162 web3cli-1.1.0/tests/ape/.build/Router_TransferHelper.json
+-rw-r--r--   0        0        0      881 2023-04-06 17:43:03.927462 web3cli-1.1.0/tests/ape/.build/Router_UniswapV2Library.json
+-rw-r--r--   0        0        0    14895 2023-04-06 17:43:03.932635 web3cli-1.1.0/tests/ape/.build/Token.json
+-rw-r--r--   0        0        0      791 2023-04-06 17:43:03.932974 web3cli-1.1.0/tests/ape/.build/Token_SafeMath.json
+-rw-r--r--   0        0        0    14014 2023-04-06 17:43:03.941015 web3cli-1.1.0/tests/ape/.build/UniswapV2ERC20.json
+-rw-r--r--   0        0        0    46097 2023-04-06 17:43:03.942289 web3cli-1.1.0/tests/ape/.build/UniswapV2Factory.json
+-rw-r--r--   0        0        0    44784 2023-04-06 17:43:03.944616 web3cli-1.1.0/tests/ape/.build/UniswapV2Pair.json
+-rw-r--r--   0        0        0    85730 2023-04-06 17:43:03.931232 web3cli-1.1.0/tests/ape/.build/UniswapV2Router02.json
+-rw-r--r--   0        0        0   324962 2023-06-08 18:16:46.405077 web3cli-1.1.0/tests/ape/.build/__local__.json
+-rw-r--r--   0        0        0        0 2023-04-07 18:14:01.620721 web3cli-1.1.0/tests/ape/__init__.py
+-rw-r--r--   0        0        0     6148 2023-02-28 16:18:44.554061 web3cli-1.1.0/tests/ape/contracts/.DS_Store
+-rw-r--r--   0        0        0     4101 2023-04-07 18:14:01.621230 web3cli-1.1.0/tests/ape/contracts/token/Token.sol
+-rw-r--r--   0        0        0      646 2023-04-07 18:14:01.621775 web3cli-1.1.0/tests/ape/contracts/token/Token_SafeMath.sol
+-rw-r--r--   0        0        0     6148 2023-02-28 15:31:57.501753 web3cli-1.1.0/tests/ape/contracts/uniswap/.DS_Store
+-rw-r--r--   0        0        0    21725 2023-04-07 18:14:01.622322 web3cli-1.1.0/tests/ape/contracts/uniswap/UniswapV2Factory.sol
+-rw-r--r--   0        0        0    34078 2023-04-07 18:14:01.622848 web3cli-1.1.0/tests/ape/contracts/uniswap/UniswapV2Router02.sol
+-rw-r--r--   0        0        0      236 2023-04-07 18:14:01.623357 web3cli-1.1.0/tests/ape/scripts/__init__.py
+-rw-r--r--   0        0        0      347 2023-04-07 18:14:01.623719 web3cli-1.1.0/tests/ape/scripts/db.py
+-rw-r--r--   0        0        0      200 2023-04-07 18:14:01.624050 web3cli-1.1.0/tests/ape/scripts/token.py
+-rw-r--r--   0        0        0        0 2023-04-07 18:14:01.624201 web3cli-1.1.0/tests/ape/tests/__init__.py
+-rw-r--r--   0        0        0    13902 2023-04-07 18:14:01.624793 web3cli-1.1.0/tests/ape/tests/fixtures.py
+-rw-r--r--   0        0        0        0 2023-04-07 18:14:01.624997 web3cli-1.1.0/tests/ape/tests/helpers/__init__.py
+-rw-r--r--   0        0        0      371 2023-04-07 18:14:01.625481 web3cli-1.1.0/tests/ape/tests/helpers/ape.py
+-rw-r--r--   0        0        0      881 2023-04-07 18:14:01.625860 web3cli-1.1.0/tests/ape/tests/helpers/token.py
+-rw-r--r--   0        0        0     3790 2023-04-07 18:14:01.626436 web3cli-1.1.0/tests/ape/tests/helpers/uniswap.py
+-rw-r--r--   0        0        0        0 2023-04-07 18:14:01.626729 web3cli-1.1.0/tests/ape/tests/token/__init__.py
+-rw-r--r--   0        0        0     1983 2023-04-07 18:14:01.627373 web3cli-1.1.0/tests/ape/tests/token/test_ape_token_approve.py
+-rw-r--r--   0        0        0     2876 2023-04-07 18:14:01.627765 web3cli-1.1.0/tests/ape/tests/token/test_ape_token_transfer.py
+-rw-r--r--   0        0        0     6467 2023-04-07 18:14:01.628071 web3cli-1.1.0/tests/ape/tests/token/test_ape_token_transferFrom.py
+-rw-r--r--   0        0        0        0 2023-04-07 18:14:01.628193 web3cli-1.1.0/tests/ape/tests/uniswap/__init__.py
+-rw-r--r--   0        0        0     4193 2023-04-07 18:14:01.628531 web3cli-1.1.0/tests/ape/tests/uniswap/test_ape_uniswap_v2_add_liquidity.py
+-rw-r--r--   0        0        0      794 2023-04-07 18:14:01.628890 web3cli-1.1.0/tests/ape/tests/uniswap/test_ape_uniswap_v2_create_pair.py
+-rw-r--r--   0        0        0      487 2023-04-07 18:14:01.629400 web3cli-1.1.0/tests/conftest.py
+-rw-r--r--   0        0        0     1130 2023-04-07 12:55:47.114434 web3cli-1.1.0/tests/helper.py
+-rw-r--r--   0        0        0     3240 2023-06-08 17:29:54.142209 web3cli-1.1.0/tests/seed.py
+-rw-r--r--   0        0        0        0 2022-12-28 17:01:25.438908 web3cli-1.1.0/tests/web3cli/__init__.py
+-rw-r--r--   0        0        0        0 2022-11-10 21:50:51.297637 web3cli-1.1.0/tests/web3cli/controllers/__init__.py
+-rw-r--r--   0        0        0     3754 2023-05-20 18:17:47.056601 web3cli-1.1.0/tests/web3cli/controllers/crud/test_address_controller.py
+-rw-r--r--   0        0        0     3517 2023-05-20 18:17:47.057300 web3cli-1.1.0/tests/web3cli/controllers/crud/test_chain_controller.py
+-rw-r--r--   0        0        0     8222 2023-05-20 18:17:47.058165 web3cli-1.1.0/tests/web3cli/controllers/crud/test_contract_controller.py
+-rw-r--r--   0        0        0     2870 2023-05-20 18:17:47.058996 web3cli-1.1.0/tests/web3cli/controllers/crud/test_history_controller.py
+-rw-r--r--   0        0        0     3762 2023-05-20 18:17:47.059822 web3cli-1.1.0/tests/web3cli/controllers/crud/test_rpc_controller.py
+-rw-r--r--   0        0        0     4933 2023-05-20 18:17:47.060483 web3cli-1.1.0/tests/web3cli/controllers/crud/test_signer_controller.py
+-rw-r--r--   0        0        0     6446 2023-06-08 18:14:50.320112 web3cli-1.1.0/tests/web3cli/controllers/crud/test_token_controller.py
+-rw-r--r--   0        0        0     1848 2023-05-18 10:32:19.351291 web3cli-1.1.0/tests/web3cli/controllers/test_appkey_controller.py
+-rw-r--r--   0        0        0     6339 2023-05-20 18:17:47.061301 web3cli-1.1.0/tests/web3cli/controllers/test_call_controller.py
+-rw-r--r--   0        0        0     1041 2023-03-25 21:24:05.581746 web3cli-1.1.0/tests/web3cli/controllers/test_db_controller.py
+-rw-r--r--   0        0        0     1702 2023-05-18 11:14:40.025134 web3cli-1.1.0/tests/web3cli/controllers/test_keyfile_controller.py
+-rw-r--r--   0        0        0     6099 2023-05-31 11:22:03.092128 web3cli-1.1.0/tests/web3cli/controllers/test_misc_controller.py
+-rw-r--r--   0        0        0     1210 2023-06-07 17:12:04.381111 web3cli-1.1.0/tests/web3cli/controllers/test_replay_controller.py
+-rw-r--r--   0        0        0     3415 2023-05-20 18:17:47.063638 web3cli-1.1.0/tests/web3cli/controllers/test_send_controller.py
+-rw-r--r--   0        0        0     9593 2023-05-20 18:17:47.064509 web3cli-1.1.0/tests/web3cli/controllers/test_transact_controller.py
+-rw-r--r--   0        0        0     1265 2023-06-07 17:10:04.508480 web3cli-1.1.0/tests/web3cli/controllers/test_tx_controller.py
+-rw-r--r--   0        0        0     1293 2023-04-07 18:14:01.632176 web3cli-1.1.0/tests/web3cli/fixtures.py
+-rw-r--r--   0        0        0        0 2022-11-10 21:50:51.303802 web3cli-1.1.0/tests/web3cli/helpers/__init__.py
+-rw-r--r--   0        0        0      684 2022-12-28 17:00:06.651527 web3cli-1.1.0/tests/web3cli/helpers/test_crypto_helper.py
+-rw-r--r--   0        0        0     1455 2023-02-12 12:11:39.416778 web3cli-1.1.0/tests/web3cli/main.py
+-rw-r--r--   0        0        0     1171 2023-02-11 18:15:39.713968 web3cli-1.1.0/tests/web3cli/test_db.py
+-rw-r--r--   0        0        0      393 2023-02-11 18:16:36.584225 web3cli-1.1.0/tests/web3cli/test_main.py
+-rw-r--r--   0        0        0        0 2022-11-10 21:50:51.301380 web3cli-1.1.0/tests/web3core/__init__.py
+-rw-r--r--   0        0        0     5362 2023-05-18 11:01:18.894137 web3cli-1.1.0/tests/web3core/fixtures.py
+-rw-r--r--   0        0        0        0 2022-11-10 21:50:51.301610 web3cli-1.1.0/tests/web3core/helpers/__init__.py
+-rw-r--r--   0        0        0     8923 2023-01-28 12:36:51.002666 web3cli-1.1.0/tests/web3core/helpers/test_abi_helper.py
+-rw-r--r--   0        0        0      528 2022-12-28 16:44:57.745951 web3cli-1.1.0/tests/web3core/helpers/test_crypto_helper.py
+-rw-r--r--   0        0        0     4807 2023-02-19 09:09:21.027684 web3cli-1.1.0/tests/web3core/helpers/test_resolve_address_helper.py
+-rw-r--r--   0        0        0     1022 2023-01-29 17:56:31.054122 web3cli-1.1.0/tests/web3core/helpers/test_validation_helper.py
+-rw-r--r--   0        0        0     1783 2023-01-14 21:27:16.475375 web3cli-1.1.0/tests/web3core/models/test_contract_model.py
+-rw-r--r--   0        0        0    11697 1970-01-01 00:00:00.000000 web3cli-1.1.0/PKG-INFO
```

### Comparing `web3cli-1.0.5/LICENSE` & `web3cli-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `web3cli-1.0.5/README.md` & `web3cli-1.1.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -114,16 +114,16 @@
    ```
    w3 swap uniswap_v2 1 usdc usdt     # swap 1 USDC for USDT on Uniswap
    w3avax swap traderjoe 1 usdc wavax # swap 1 USDC for WAVAX on TraderJoe
    ```
 
 - Replay a given transactions on the blockchain:
    ```
-   tx=`w3arb send unicef 1 USDC --force` # send 1 USDC to Unicef
-   w3 replay $tx                         # re-send 1 USDC to Unicef
+   tx=`w3 send unicef 1 USDC --force` # send 1 USDC to Unicef
+   w3 replay $tx                      # re-send 1 USDC to Unicef
    ```
 
 # Smart Contract support
 
 `web3cli` comes preloaded with some popular smart contracts, including ERC20 tokens and Uniswap clones.
 
 See the available contracts with `w3 contract list`:
```

#### html2text {}

```diff
@@ -40,28 +40,28 @@
 Output-processing)): ```bash w3 block latest | jq -r '.baseFeePerGas' ``` -
 Sign messages: ```bash w3 sign 'Hello world!' ``` # Advanced examples - Send
 coins or tokens to any address: ``` w3 send unicef 1 ETH # send 1 ETH, ask for
 confirmation w3 send unicef 1 ETH gwei # send 1 gwei, ask for confirmation w3
 send unicef 1 usdc # send 1 USDC ``` - Swap tokens on a DEX: ``` w3 swap
 uniswap_v2 1 usdc usdt # swap 1 USDC for USDT on Uniswap w3avax swap traderjoe
 1 usdc wavax # swap 1 USDC for WAVAX on TraderJoe ``` - Replay a given
-transactions on the blockchain: ``` tx=`w3arb send unicef 1 USDC --force` #
-send 1 USDC to Unicef w3 replay $tx # re-send 1 USDC to Unicef ``` # Smart
-Contract support `web3cli` comes preloaded with some popular smart contracts,
-including ERC20 tokens and Uniswap clones. See the available contracts with `w3
-contract list`: ``` w3 contract list # contracts on Ethereum w3 contract list -
--chain bnb # contracts on BNB chain w3 contract list --type erc20 # tokens on
-Ethereum ``` You can also add custom contracts with `w3 contract add`: ``` w3
-contract add weth 0xC02aaA39b223FE8D0A0e5C4F27eAD9083C756Cc2 --type erc20 w3
-contract add sushi 0xd9e1cE17f2641f24aE83637ab66a2cca9C378B9F --type uniswap_v2
-``` To add or list new tokens, you can use the `w3 token` shorthand: ``` w3
-token add weth 0xC02aaA39b223FE8D0A0e5C4F27eAD9083C756Cc2 w3 token list w3
-token delete weth ``` See available functions and events on a contract with `w3
-abi functions` and `w3 abi events`: ``` w3 abi fns weth # functions on WETH
-token w3 abi evs uniswap_v2 # events on Uniswap V2 w3 abi fns --abi abi.json #
+transactions on the blockchain: ``` tx=`w3 send unicef 1 USDC --force` # send 1
+USDC to Unicef w3 replay $tx # re-send 1 USDC to Unicef ``` # Smart Contract
+support `web3cli` comes preloaded with some popular smart contracts, including
+ERC20 tokens and Uniswap clones. See the available contracts with `w3 contract
+list`: ``` w3 contract list # contracts on Ethereum w3 contract list --chain
+bnb # contracts on BNB chain w3 contract list --type erc20 # tokens on Ethereum
+``` You can also add custom contracts with `w3 contract add`: ``` w3 contract
+add weth 0xC02aaA39b223FE8D0A0e5C4F27eAD9083C756Cc2 --type erc20 w3 contract
+add sushi 0xd9e1cE17f2641f24aE83637ab66a2cca9C378B9F --type uniswap_v2 ``` To
+add or list new tokens, you can use the `w3 token` shorthand: ``` w3 token add
+weth 0xC02aaA39b223FE8D0A0e5C4F27eAD9083C756Cc2 w3 token list w3 token delete
+weth ``` See available functions and events on a contract with `w3 abi
+functions` and `w3 abi events`: ``` w3 abi fns weth # functions on WETH token
+w3 abi evs uniswap_v2 # events on Uniswap V2 w3 abi fns --abi abi.json #
 functions of an arbitrary ABI ``` ### Read from a smart contract To read from a
 smart contract, use `w3 call`. For example, to get the total supply of the WETH
 token, run: ``` w3 call weth totalSupply ``` Function arguments are parsed
 automatically, so you can call `balanceOf` with: ``` w3 call weth balanceOf
 0xA59B29d7dbC9794d1e7f45123C48b2b8d0a34636 ``` You can also do more complex
 stuff like: ```bash # get the amount of USDT you get for 100 USDC w3 call
 uniswap_v2 getAmountsOut 100e6 usdc,usdt | jq -r '.[1]' ``` ### Send a
```

### Comparing `web3cli-1.0.5/pyproject.toml` & `web3cli-1.1.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "web3cli"
-version = "1.0.5"
+version = "1.1.0"
 description = "Interact with blockchains and smart contracts using the command line"
 authors = [
     { name = "coccoinomane", email = "coccoinomane@gmail.com" },
 ]
 readme = "README.md"
 keywords = [
     "web3",
@@ -40,14 +40,15 @@
 w3eth = "web3cli.main:w3eth"
 w3bnb = "web3cli.main:w3bnb"
 w3avax = "web3cli.main:w3avax"
 w3matic = "web3cli.main:w3matic"
 w3cro = "web3cli.main:w3cro"
 w3arb = "web3cli.main:w3arb"
 w3era = "web3cli.main:w3era"
+w3erat = "web3cli.main:w3erat"
 w3gno = "web3cli.main:w3gno"
 
 [project.urls]
 homepage = "https://github.com/coccoinomane/web3cli"
 repository = "https://github.com/coccoinomane/web3cli"
 
 [tool.pdm.dev-dependencies]
@@ -98,14 +99,18 @@
 cmd = "w3arb"
 help = "Run the CLI in dev mode, on Arbitrum One chain"
 
 [tool.pdm.scripts.w3era]
 cmd = "w3era"
 help = "Run the CLI in dev mode, on zkSync Era chain"
 
+[tool.pdm.scripts.w3erat]
+cmd = "w3erat"
+help = "Run the CLI in dev mode, on zkSync Era testnet chain"
+
 [tool.pdm.scripts.w3gno]
 cmd = "w3gno"
 help = "Run the CLI in dev mode, on Gnosis (xDAI) chain"
 
 [tool.pdm.build]
 includes = [
     "src",
```

### Comparing `web3cli-1.0.5/src/web3cli/.DS_Store` & `web3cli-1.1.0/src/web3cli/.DS_Store`

 * *Files identical despite different names*

### Comparing `web3cli-1.0.5/src/web3cli/controllers/abi_controller.py` & `web3cli-1.1.0/src/web3cli/controllers/abi_controller.py`

 * *Files identical despite different names*

### Comparing `web3cli-1.0.5/src/web3cli/controllers/app_key_controller.py` & `web3cli-1.1.0/src/web3cli/controllers/app_key_controller.py`

 * *Files identical despite different names*

### Comparing `web3cli-1.0.5/src/web3cli/controllers/base_controller.py` & `web3cli-1.1.0/src/web3cli/controllers/base_controller.py`

 * *Files identical despite different names*

### Comparing `web3cli-1.0.5/src/web3cli/controllers/call_controller.py` & `web3cli-1.1.0/src/web3cli/controllers/call_controller.py`

 * *Files identical despite different names*

### Comparing `web3cli-1.0.5/src/web3cli/controllers/config_controller.py` & `web3cli-1.1.0/src/web3cli/controllers/config_controller.py`

 * *Files identical despite different names*

### Comparing `web3cli-1.0.5/src/web3cli/controllers/controller.py` & `web3cli-1.1.0/src/web3cli/controllers/controller.py`

 * *Files identical despite different names*

### Comparing `web3cli-1.0.5/src/web3cli/controllers/crud/address_controller.py` & `web3cli-1.1.0/src/web3cli/controllers/crud/address_controller.py`

 * *Files identical despite different names*

### Comparing `web3cli-1.0.5/src/web3cli/controllers/crud/chain_controller.py` & `web3cli-1.1.0/src/web3cli/controllers/crud/chain_controller.py`

 * *Files identical despite different names*

### Comparing `web3cli-1.0.5/src/web3cli/controllers/crud/contract_controller.py` & `web3cli-1.1.0/src/web3cli/controllers/crud/contract_controller.py`

 * *Files identical despite different names*

### Comparing `web3cli-1.0.5/src/web3cli/controllers/crud/history_controller.py` & `web3cli-1.1.0/src/web3cli/controllers/crud/history_controller.py`

 * *Files identical despite different names*

### Comparing `web3cli-1.0.5/src/web3cli/controllers/crud/rpc_controller.py` & `web3cli-1.1.0/src/web3cli/controllers/crud/rpc_controller.py`

 * *Files identical despite different names*

### Comparing `web3cli-1.0.5/src/web3cli/controllers/crud/signer_controller.py` & `web3cli-1.1.0/src/web3cli/controllers/crud/signer_controller.py`

 * *Files identical despite different names*

### Comparing `web3cli-1.0.5/src/web3cli/controllers/db_controller.py` & `web3cli-1.1.0/src/web3cli/controllers/db_controller.py`

 * *Files identical despite different names*

### Comparing `web3cli-1.0.5/src/web3cli/controllers/keyfile_controller.py` & `web3cli-1.1.0/src/web3cli/controllers/keyfile_controller.py`

 * *Files identical despite different names*

### Comparing `web3cli-1.0.5/src/web3cli/controllers/misc_controller.py` & `web3cli-1.1.0/src/web3cli/controllers/misc_controller.py`

 * *Files identical despite different names*

### Comparing `web3cli-1.0.5/src/web3cli/controllers/replay_controller.py` & `web3cli-1.1.0/src/web3cli/controllers/replay_controller.py`

 * *Files 3% similar despite different names*

```diff
@@ -39,14 +39,18 @@
                     "type": float,
                 },
             ),
             (
                 ["--type"],
                 {"help": "Override the type of the original tx", "type": int},
             ),
+            (
+                ["--data", "--input"],
+                {"help": "Override the input data of the original tx"},
+            ),
             args.force(),
         ],
     )
     def replay(self) -> None:
         original_tx = make_client(self.app).get_tx(self.app.pargs.hash)
         # Build replay transaction
         signer = make_wallet(self.app)
@@ -83,14 +87,17 @@
         ):
             tx["gasPrice"] = int(
                 original_tx["gasPrice"] * self.app.pargs.fee_multiplier
             )
         # Optionally override type field
         if self.app.pargs.type is not None:
             tx["type"] = self.app.pargs.type
+        # Optionally override data field
+        if self.app.pargs.data is not None:
+            tx["data"] = self.app.pargs.data
         # Ask for confirmation
         if not self.app.pargs.force:
             self.app.log.info(f"Replaying the following transaction:")
             render_web3py(self.app, original_tx)
             print("\n")
             self.app.log.info(f"Transaction that will be sent:")
             render_web3py(self.app, tx)
```

### Comparing `web3cli-1.0.5/src/web3cli/controllers/send_controller.py` & `web3cli-1.1.0/src/web3cli/controllers/send_controller.py`

 * *Files identical despite different names*

### Comparing `web3cli-1.0.5/src/web3cli/controllers/swap_controller.py` & `web3cli-1.1.0/src/web3cli/controllers/swap_controller.py`

 * *Files identical despite different names*

### Comparing `web3cli-1.0.5/src/web3cli/controllers/token_controller.py` & `web3cli-1.1.0/src/web3cli/controllers/token_controller.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 import argparse
-import decimal
 
 from cement import ex
 
 from web3cli.controllers.controller import Controller
 from web3cli.exceptions import Web3CliError
 from web3cli.helpers import args
 from web3cli.helpers.client_factory import make_contract_client, make_contract_wallet
@@ -27,23 +26,23 @@
         help="Approve the given spender to spend the given amount of tokens",
         arguments=[
             (["token"], {"help": "Token to approve"}),
             (["spender"], {"help": "Address or name of the spender to be approved"}),
             (
                 ["amount"],
                 {
-                    "help": "Amount of tokens to approve, in wei. Leave empty to approve the maximum amount",
-                    "type": int,
+                    "help": "Amount of tokens to approve. Leave empty to approve the maximum amount",
+                    "type": float,
                     "nargs": "?",
                 },
             ),
             (
                 ["--check"],
                 {
-                    "help": "Do nothing if the spender already has enough allowance",
+                    "help": "Whether to stop if the spender already has enough allowance",
                     "action": argparse.BooleanOptionalAction,
                     "default": True,
                 },
             ),
             args.tx_return(),
             args.tx_dry_run(),
             args.tx_call(),
@@ -53,68 +52,91 @@
             args.force(),
         ],
     )
     def approve(self) -> None:
         # Parse arguments
         spender = resolve_address(self.app.pargs.spender, chain=self.app.chain.name)
         # Initialize client
-        client = make_contract_wallet(self.app, self.app.pargs.token)
+        signer = make_contract_wallet(self.app, self.app.pargs.token)
         # Compute amount in
         if not self.app.pargs.amount:
-            amount = 2**256 - 1
+            amount_in_wei = 2**256 - 1
         else:
-            amount_token_units = decimal.Decimal(self.app.pargs.amount)
-            decimals = client.functions["decimals"]().call()
-            amount = int(amount_token_units * 10**decimals)
+            decimals = signer.functions["decimals"]().call()
+            amount_in_wei = int(self.app.pargs.amount * 10**decimals)
         # Approve
         if self.app.pargs.check:
             self.app.log.debug("Checking token allowance...")
-            allowance = client.functions["allowance"](
+            allowance = signer.functions["allowance"](
                 self.app.signer.address, spender
             ).call()
             # If allowance is not sufficient, approve
-            if allowance >= amount:
+            if allowance >= amount_in_wei:
                 self.app.log.info(
-                    "Not approving: token allowance is already sufficient"
+                    f"Token allowance already sufficient {allowance} >= {amount_in_wei}"
                 )
                 return
         # Confirm
         if not self.app.pargs.force:
             what = (
                 (str(self.app.pargs.amount) if self.app.pargs.amount else "infinite")
                 + " "
                 + self.app.pargs.token
             )
             print(
-                f"You are about to approve {self.app.pargs.spender} on chain {self.app.chain.name} to spend {what} in your name"
+                f"You are about to approve {spender} on chain {self.app.chain.name} to spend {what} on behalf of {signer.user_address}"
             )
             yes_or_exit(logger=self.app.log.info)
         self.app.log.debug("Approving DEX spender spend token...")
         output = send_contract_tx(
             self.app,
-            client,
-            client.functions["approve"](spender, amount),
+            signer,
+            signer.functions["approve"](spender, amount_in_wei),
         )
         # Print output
         render_web3py(self.app, output)
 
     @ex(
         help="Show the balance of the given token for the given address",
         arguments=[
             (["token"], {"help": "Token to check, by name"}),
             (["address"], {"help": "Address or name of the account to check"}),
+            (["--wei"], {"help": "Print the output in wei", "action": "store_true"}),
             *args.chain_and_rpc(),
         ],
     )
     def balance(self) -> None:
         address = resolve_address(self.app.pargs.address, chain=self.app.chain.name)
         client = make_contract_client(self.app, self.app.pargs.token)
         balance_in_wei = client.functions["balanceOf"](address).call()
-        balance = balance_in_wei / 10 ** client.functions["decimals"]().call()
-        render_number(self.app, balance)
+        if self.app.pargs.wei:
+            render_number(self.app, balance_in_wei)
+        else:
+            balance = balance_in_wei / 10 ** client.functions["decimals"]().call()
+            render_number(self.app, balance)
+
+    @ex(
+        help="Return the allowance of the given spender to spend the given token for the given address",
+        arguments=[
+            (["token"], {"help": "Token to check, by name"}),
+            (["owner"], {"help": "Address or name of the account to check"}),
+            (["spender"], {"help": "Address or name of the spender to check"}),
+            *args.chain_and_rpc(),
+        ],
+    )
+    def allowance(self) -> None:
+        # Parse arguments
+        spender = resolve_address(self.app.pargs.spender, chain=self.app.chain.name)
+        owner = resolve_address(self.app.pargs.owner, chain=self.app.chain.name)
+        # Initialize client
+        client = make_contract_client(self.app, self.app.pargs.token)
+        decimals = client.functions["decimals"]().call()
+        allowance_in_wei = client.functions["allowance"](owner, spender).call()
+        allowance = allowance_in_wei / 10**decimals
+        self.app.print(str(allowance))
 
     #    ____                      _
     #   / ___|  _ __   _   _    __| |
     #  | |     | '__| | | | |  / _` |
     #  | |___  | |    | |_| | | (_| |
     #   \____| |_|     \__,_|  \__,_|
```

### Comparing `web3cli-1.0.5/src/web3cli/controllers/transact_controller.py` & `web3cli-1.1.0/src/web3cli/controllers/transact_controller.py`

 * *Files identical despite different names*

### Comparing `web3cli-1.0.5/src/web3cli/controllers/tx_controller.py` & `web3cli-1.1.0/src/web3cli/controllers/tx_controller.py`

 * *Files identical despite different names*

### Comparing `web3cli-1.0.5/src/web3cli/helpers/args.py` & `web3cli-1.1.0/src/web3cli/helpers/args.py`

 * *Files identical despite different names*

### Comparing `web3cli-1.0.5/src/web3cli/helpers/client_factory.py` & `web3cli-1.1.0/src/web3cli/helpers/client_factory.py`

 * *Files identical despite different names*

### Comparing `web3cli-1.0.5/src/web3cli/helpers/config.py` & `web3cli-1.1.0/src/web3cli/helpers/config.py`

 * *Files identical despite different names*

### Comparing `web3cli-1.0.5/src/web3cli/helpers/crypto.py` & `web3cli-1.1.0/src/web3cli/helpers/crypto.py`

 * *Files identical despite different names*

### Comparing `web3cli-1.0.5/src/web3cli/helpers/database.py` & `web3cli-1.1.0/src/web3cli/helpers/database.py`

 * *Files identical despite different names*

### Comparing `web3cli-1.0.5/src/web3cli/helpers/render.py` & `web3cli-1.1.0/src/web3cli/helpers/render.py`

 * *Files 4% similar despite different names*

```diff
@@ -60,8 +60,11 @@
         "balance.jinja2",
         handler="jinja2",
     )
 
 
 def render_number(app: App, n: Union[int, float]) -> None:
     """Print a number"""
-    app.print(f"{n:g}")
+    if isinstance(n, int):
+        app.print(f"{n}")
+    else:
+        app.print(f"{n:.18g}")
```

### Comparing `web3cli-1.0.5/src/web3cli/helpers/send.py` & `web3cli-1.1.0/src/web3cli/helpers/send.py`

 * *Files identical despite different names*

### Comparing `web3cli-1.0.5/src/web3cli/helpers/signer.py` & `web3cli-1.1.0/src/web3cli/helpers/signer.py`

 * *Files identical despite different names*

### Comparing `web3cli-1.0.5/src/web3cli/helpers/tx.py` & `web3cli-1.1.0/src/web3cli/helpers/tx.py`

 * *Files identical despite different names*

### Comparing `web3cli-1.0.5/src/web3cli/hooks.py` & `web3cli-1.1.0/src/web3cli/hooks.py`

 * *Files identical despite different names*

### Comparing `web3cli-1.0.5/src/web3cli/main.py` & `web3cli-1.1.0/src/web3cli/main.py`

 * *Files 1% similar despite different names*

```diff
@@ -222,10 +222,15 @@
 
 
 def w3era() -> None:
     """Shorthand command to use zkSync Era chain"""
     main(lambda a: override_arg(a, "chain", "era"))
 
 
+def w3erat() -> None:
+    """Shorthand command to use zkSync Era testnet chain"""
+    main(lambda a: override_arg(a, "chain", "erat"))
+
+
 def w3gno() -> None:
     """Shorthand command to use gnosis chain"""
     main(lambda a: override_arg(a, "chain", "gno"))
```

### Comparing `web3cli-1.0.5/src/web3core/exceptions.py` & `web3cli-1.1.0/src/web3core/exceptions.py`

 * *Files identical despite different names*

### Comparing `web3cli-1.0.5/src/web3core/helpers/abi.py` & `web3cli-1.1.0/src/web3core/helpers/abi.py`

 * *Files identical despite different names*

### Comparing `web3cli-1.0.5/src/web3core/helpers/blocks.py` & `web3cli-1.1.0/src/web3core/helpers/blocks.py`

 * *Files identical despite different names*

### Comparing `web3cli-1.0.5/src/web3core/helpers/client_factory.py` & `web3cli-1.1.0/src/web3core/helpers/client_factory.py`

 * *Files identical despite different names*

### Comparing `web3cli-1.0.5/src/web3core/helpers/crypto.py` & `web3cli-1.1.0/src/web3core/helpers/crypto.py`

 * *Files identical despite different names*

### Comparing `web3cli-1.0.5/src/web3core/helpers/database.py` & `web3cli-1.1.0/src/web3core/helpers/database.py`

 * *Files identical despite different names*

### Comparing `web3cli-1.0.5/src/web3core/helpers/dex.py` & `web3cli-1.1.0/src/web3core/helpers/dex.py`

 * *Files identical despite different names*

### Comparing `web3cli-1.0.5/src/web3core/helpers/misc.py` & `web3cli-1.1.0/src/web3core/helpers/misc.py`

 * *Files identical despite different names*

### Comparing `web3cli-1.0.5/src/web3core/helpers/os.py` & `web3cli-1.1.0/src/web3core/helpers/os.py`

 * *Files identical despite different names*

### Comparing `web3cli-1.0.5/src/web3core/helpers/resolve.py` & `web3cli-1.1.0/src/web3core/helpers/resolve.py`

 * *Files identical despite different names*

### Comparing `web3cli-1.0.5/src/web3core/helpers/rpc.py` & `web3cli-1.1.0/src/web3core/helpers/rpc.py`

 * *Files identical despite different names*

### Comparing `web3cli-1.0.5/src/web3core/helpers/seed.py` & `web3cli-1.1.0/src/web3core/helpers/seed.py`

 * *Files identical despite different names*

### Comparing `web3cli-1.0.5/src/web3core/helpers/tx.py` & `web3cli-1.1.0/src/web3core/helpers/tx.py`

 * *Files identical despite different names*

### Comparing `web3cli-1.0.5/src/web3core/helpers/yaml.py` & `web3cli-1.1.0/src/web3core/helpers/yaml.py`

 * *Files identical despite different names*

### Comparing `web3cli-1.0.5/src/web3core/models/address.py` & `web3cli-1.1.0/src/web3core/models/address.py`

 * *Files identical despite different names*

### Comparing `web3cli-1.0.5/src/web3core/models/base_model.py` & `web3cli-1.1.0/src/web3core/models/base_model.py`

 * *Files identical despite different names*

### Comparing `web3cli-1.0.5/src/web3core/models/chain.py` & `web3cli-1.1.0/src/web3core/models/chain.py`

 * *Files identical despite different names*

### Comparing `web3cli-1.0.5/src/web3core/models/contract.py` & `web3cli-1.1.0/src/web3core/models/contract.py`

 * *Files identical despite different names*

### Comparing `web3cli-1.0.5/src/web3core/models/signer.py` & `web3cli-1.1.0/src/web3core/models/signer.py`

 * *Files identical despite different names*

### Comparing `web3cli-1.0.5/src/web3core/models/timestamps_model.py` & `web3cli-1.1.0/src/web3core/models/timestamps_model.py`

 * *Files identical despite different names*

### Comparing `web3cli-1.0.5/src/web3core/models/tx.py` & `web3cli-1.1.0/src/web3core/models/tx.py`

 * *Files identical despite different names*

### Comparing `web3cli-1.0.5/src/web3core/models/types.py` & `web3cli-1.1.0/src/web3core/models/types.py`

 * *Files identical despite different names*

### Comparing `web3cli-1.0.5/src/web3core/seeds/chain_seeds.py` & `web3cli-1.1.0/src/web3core/seeds/chain_seeds.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,117 +1,124 @@
 from typing import List
 
 from web3core.models.types import ChainFields
 
-# Ethereum
 eth: ChainFields = {
     "name": "eth",
     "desc": "Ethereum Mainnet",
     "chain_id": 1,
     "coin": "ETH",
     "tx_type": 2,
     "middlewares": "",
     "rpcs": [
         {
             "url": "https://cloudflare-eth.com",
         },
     ],
 }
 
-# BNB Chain
 bnb: ChainFields = {
     "name": "bnb",
     "desc": "Binance Smart Chain Mainnet",
     "chain_id": 56,
     "coin": "BNB",
     "tx_type": 1,
     "middlewares": "geth_poa_middleware",
     "rpcs": [
         {
             "url": "https://bsc-dataseed.binance.org/",
         }
     ],
 }
 
-# Avalanche C Chian
 avax: ChainFields = {
     "name": "avax",
     "desc": "Avalanche C-Chain",
     "chain_id": 43114,
     "coin": "AVAX",
     "tx_type": 2,
     "middlewares": "geth_poa_middleware",
     "rpcs": [
         {
             "url": "https://api.avax.network/ext/bc/C/rpc",
         }
     ],
 }
 
-# Polygon chain
 matic: ChainFields = {
     "name": "matic",
     "desc": "Polygon Mainnet",
     "chain_id": 137,
     "coin": "MATIC",
     "tx_type": 1,
     "middlewares": "geth_poa_middleware",
     "rpcs": [
         {
             "url": "https://polygon-rpc.com/",
         }
     ],
 }
 
-# Cronos chain
 cro: ChainFields = {
     "name": "cro",
     "desc": "Cronos Mainnet Beta",
     "chain_id": 25,
     "coin": "CRO",
     "tx_type": 2,
     "middlewares": "",
     "rpcs": [
         {
             "url": "https://evm.cronos.org",
         }
     ],
 }
 
-# Arbitrum One chain
 arb: ChainFields = {
     "name": "arb",
     "desc": "Arbitrum One",
     "chain_id": 42161,
     "coin": "ETH",
     "tx_type": 2,
     "middlewares": "",
     "rpcs": [
         {
             "url": "https://arb1.arbitrum.io/rpc",
         },
     ],
 }
 
-# Arbitrum One chain
 era: ChainFields = {
     "name": "era",
     "desc": "zkSync Era",
     "chain_id": 324,
     "coin": "ETH",
     "tx_type": 2,
     "middlewares": "",
     "rpcs": [
         {
             "url": "https://mainnet.era.zksync.io",
         },
     ],
 }
 
-# Gnosis chain
+erat: ChainFields = {
+    "name": "erat",
+    "desc": "zkSync Era Testnet",
+    "chain_id": 280,
+    "coin": "ETH",
+    "tx_type": 2,
+    "middlewares": "",
+    "rpcs": [
+        {
+            "url": "https://testnet.era.zksync.dev",
+        },
+    ],
+}
+
+
 gno: ChainFields = {
     "name": "gno",
     "desc": "Gnosis",
     "chain_id": 100,
     "coin": "xDAI",
     "tx_type": 2,
     "middlewares": "",
@@ -125,30 +132,28 @@
         {
             "url": "https://rpc.ankr.com/gnosis",
         },
     ],
 }
 
 
-# Ganache local chain
 ganache: ChainFields = {
     "name": "ganache",
     "desc": "Ganache local chain",
     "chain_id": 1337,
     "coin": "ETH",
     "tx_type": 1,
     "middlewares": "",
     "rpcs": [
         {
             "url": "http://127.0.0.1:8545",
         }
     ],
 }
 
-# Anvil local chain
 anvil: ChainFields = {
     "name": "anvil",
     "desc": "Anvil local chain",
     "chain_id": 31337,
     "coin": "ETH",
     "tx_type": 2,
     "middlewares": "",
@@ -163,11 +168,12 @@
     eth,
     bnb,
     avax,
     matic,
     cro,
     arb,
     era,
+    erat,
     gno,
     ganache,
     anvil,
 ]
```

### Comparing `web3cli-1.0.5/src/web3core/seeds/contract_type_seeds.py` & `web3cli-1.1.0/src/web3core/seeds/contract_type_seeds.py`

 * *Files identical despite different names*

### Comparing `web3cli-1.0.5/src/web3core/seeds/contracts/arb_contract_seeds.py` & `web3cli-1.1.0/src/web3core/seeds/contracts/arb_contract_seeds.py`

 * *Files identical despite different names*

### Comparing `web3cli-1.0.5/src/web3core/seeds/contracts/avax_contract_seeds.py` & `web3cli-1.1.0/src/web3core/seeds/contracts/avax_contract_seeds.py`

 * *Files identical despite different names*

### Comparing `web3cli-1.0.5/src/web3core/seeds/contracts/era_contract_seeds.py` & `web3cli-1.1.0/src/web3core/seeds/contracts/era_contract_seeds.py`

 * *Files identical despite different names*

### Comparing `web3cli-1.0.5/src/web3core/seeds/contracts/eth_contract_seeds.py` & `web3cli-1.1.0/src/web3core/seeds/contracts/eth_contract_seeds.py`

 * *Files identical despite different names*

### Comparing `web3cli-1.0.5/src/web3core/seeds/contracts/gno_contract_seeds.py` & `web3cli-1.1.0/src/web3core/seeds/contracts/gno_contract_seeds.py`

 * *Files identical despite different names*

### Comparing `web3cli-1.0.5/src/web3core/types.py` & `web3cli-1.1.0/src/web3core/types.py`

 * *Files identical despite different names*

### Comparing `web3cli-1.0.5/tests/.DS_Store` & `web3cli-1.1.0/tests/.DS_Store`

 * *Files identical despite different names*

### Comparing `web3cli-1.0.5/tests/ape/.DS_Store` & `web3cli-1.1.0/tests/ape/.DS_Store`

 * *Files identical despite different names*

### Comparing `web3cli-1.0.5/tests/ape/.build/Factory_IERC20.json` & `web3cli-1.1.0/tests/ape/.build/Factory_IERC20.json`

 * *Files identical despite different names*

### Comparing `web3cli-1.0.5/tests/ape/.build/Factory_IUniswapV2Callee.json` & `web3cli-1.1.0/tests/ape/.build/Factory_IUniswapV2Callee.json`

 * *Files identical despite different names*

### Comparing `web3cli-1.0.5/tests/ape/.build/Factory_IUniswapV2ERC20.json` & `web3cli-1.1.0/tests/ape/.build/Factory_IUniswapV2ERC20.json`

 * *Files identical despite different names*

### Comparing `web3cli-1.0.5/tests/ape/.build/Factory_IUniswapV2Factory.json` & `web3cli-1.1.0/tests/ape/.build/Factory_IUniswapV2Factory.json`

 * *Files identical despite different names*

### Comparing `web3cli-1.0.5/tests/ape/.build/Factory_IUniswapV2Pair.json` & `web3cli-1.1.0/tests/ape/.build/Factory_IUniswapV2Pair.json`

 * *Files identical despite different names*

### Comparing `web3cli-1.0.5/tests/ape/.build/Factory_Math.json` & `web3cli-1.1.0/tests/ape/.build/Factory_Math.json`

 * *Files identical despite different names*

### Comparing `web3cli-1.0.5/tests/ape/.build/Factory_SafeMath.json` & `web3cli-1.1.0/tests/ape/.build/Factory_SafeMath.json`

 * *Files identical despite different names*

### Comparing `web3cli-1.0.5/tests/ape/.build/Factory_UQ112x112.json` & `web3cli-1.1.0/tests/ape/.build/Factory_UQ112x112.json`

 * *Files identical despite different names*

### Comparing `web3cli-1.0.5/tests/ape/.build/Router_IERC20.json` & `web3cli-1.1.0/tests/ape/.build/Router_IERC20.json`

 * *Files identical despite different names*

### Comparing `web3cli-1.0.5/tests/ape/.build/Router_IUniswapV2Factory.json` & `web3cli-1.1.0/tests/ape/.build/Router_IUniswapV2Factory.json`

 * *Files identical despite different names*

### Comparing `web3cli-1.0.5/tests/ape/.build/Router_IUniswapV2Pair.json` & `web3cli-1.1.0/tests/ape/.build/Router_IUniswapV2Pair.json`

 * *Files identical despite different names*

### Comparing `web3cli-1.0.5/tests/ape/.build/Router_IUniswapV2Router01.json` & `web3cli-1.1.0/tests/ape/.build/Router_IUniswapV2Router01.json`

 * *Files identical despite different names*

### Comparing `web3cli-1.0.5/tests/ape/.build/Router_IUniswapV2Router02.json` & `web3cli-1.1.0/tests/ape/.build/Router_IUniswapV2Router02.json`

 * *Files identical despite different names*

### Comparing `web3cli-1.0.5/tests/ape/.build/Router_IWETH.json` & `web3cli-1.1.0/tests/ape/.build/Router_IWETH.json`

 * *Files identical despite different names*

### Comparing `web3cli-1.0.5/tests/ape/.build/Router_SafeMath.json` & `web3cli-1.1.0/tests/ape/.build/Router_SafeMath.json`

 * *Files identical despite different names*

### Comparing `web3cli-1.0.5/tests/ape/.build/Router_TransferHelper.json` & `web3cli-1.1.0/tests/ape/.build/Router_TransferHelper.json`

 * *Files identical despite different names*

### Comparing `web3cli-1.0.5/tests/ape/.build/Router_UniswapV2Library.json` & `web3cli-1.1.0/tests/ape/.build/Router_UniswapV2Library.json`

 * *Files identical despite different names*

### Comparing `web3cli-1.0.5/tests/ape/.build/Token.json` & `web3cli-1.1.0/tests/ape/.build/Token.json`

 * *Files identical despite different names*

### Comparing `web3cli-1.0.5/tests/ape/.build/Token_SafeMath.json` & `web3cli-1.1.0/tests/ape/.build/Token_SafeMath.json`

 * *Files identical despite different names*

### Comparing `web3cli-1.0.5/tests/ape/.build/UniswapV2ERC20.json` & `web3cli-1.1.0/tests/ape/.build/UniswapV2ERC20.json`

 * *Files identical despite different names*

### Comparing `web3cli-1.0.5/tests/ape/.build/UniswapV2Factory.json` & `web3cli-1.1.0/tests/ape/.build/UniswapV2Factory.json`

 * *Files identical despite different names*

### Comparing `web3cli-1.0.5/tests/ape/.build/UniswapV2Pair.json` & `web3cli-1.1.0/tests/ape/.build/UniswapV2Pair.json`

 * *Files identical despite different names*

### Comparing `web3cli-1.0.5/tests/ape/.build/UniswapV2Router02.json` & `web3cli-1.1.0/tests/ape/.build/UniswapV2Router02.json`

 * *Files identical despite different names*

### Comparing `web3cli-1.0.5/tests/ape/.build/__local__.json` & `web3cli-1.1.0/tests/ape/.build/__local__.json`

 * *Files identical despite different names*

### Comparing `web3cli-1.0.5/tests/ape/contracts/.DS_Store` & `web3cli-1.1.0/tests/ape/contracts/.DS_Store`

 * *Files identical despite different names*

### Comparing `web3cli-1.0.5/tests/ape/contracts/token/Token.sol` & `web3cli-1.1.0/tests/ape/contracts/token/Token.sol`

 * *Files identical despite different names*

### Comparing `web3cli-1.0.5/tests/ape/contracts/token/Token_SafeMath.sol` & `web3cli-1.1.0/tests/ape/contracts/token/Token_SafeMath.sol`

 * *Files identical despite different names*

### Comparing `web3cli-1.0.5/tests/ape/contracts/uniswap/.DS_Store` & `web3cli-1.1.0/tests/ape/contracts/uniswap/.DS_Store`

 * *Files identical despite different names*

### Comparing `web3cli-1.0.5/tests/ape/contracts/uniswap/UniswapV2Factory.sol` & `web3cli-1.1.0/tests/ape/contracts/uniswap/UniswapV2Factory.sol`

 * *Files identical despite different names*

### Comparing `web3cli-1.0.5/tests/ape/contracts/uniswap/UniswapV2Router02.sol` & `web3cli-1.1.0/tests/ape/contracts/uniswap/UniswapV2Router02.sol`

 * *Files identical despite different names*

### Comparing `web3cli-1.0.5/tests/ape/tests/fixtures.py` & `web3cli-1.1.0/tests/ape/tests/fixtures.py`

 * *Files identical despite different names*

### Comparing `web3cli-1.0.5/tests/ape/tests/helpers/token.py` & `web3cli-1.1.0/tests/ape/tests/helpers/token.py`

 * *Files identical despite different names*

### Comparing `web3cli-1.0.5/tests/ape/tests/helpers/uniswap.py` & `web3cli-1.1.0/tests/ape/tests/helpers/uniswap.py`

 * *Files identical despite different names*

### Comparing `web3cli-1.0.5/tests/ape/tests/token/test_token_approve.py` & `web3cli-1.1.0/tests/ape/tests/token/test_ape_token_approve.py`

 * *Files identical despite different names*

### Comparing `web3cli-1.0.5/tests/ape/tests/token/test_token_transfer.py` & `web3cli-1.1.0/tests/ape/tests/token/test_ape_token_transfer.py`

 * *Files identical despite different names*

### Comparing `web3cli-1.0.5/tests/ape/tests/token/test_token_transferFrom.py` & `web3cli-1.1.0/tests/ape/tests/token/test_ape_token_transferFrom.py`

 * *Files identical despite different names*

### Comparing `web3cli-1.0.5/tests/ape/tests/uniswap/test_v2_add_liquidity.py` & `web3cli-1.1.0/tests/ape/tests/uniswap/test_ape_uniswap_v2_add_liquidity.py`

 * *Files identical despite different names*

### Comparing `web3cli-1.0.5/tests/ape/tests/uniswap/test_v2_create_pair.py` & `web3cli-1.1.0/tests/ape/tests/uniswap/test_ape_uniswap_v2_create_pair.py`

 * *Files identical despite different names*

### Comparing `web3cli-1.0.5/tests/helper.py` & `web3cli-1.1.0/tests/helper.py`

 * *Files identical despite different names*

### Comparing `web3cli-1.0.5/tests/seed.py` & `web3cli-1.1.0/tests/seed.py`

 * *Files identical despite different names*

### Comparing `web3cli-1.0.5/tests/web3cli/controllers/crud/test_address_controller.py` & `web3cli-1.1.0/tests/web3cli/controllers/crud/test_address_controller.py`

 * *Files identical despite different names*

### Comparing `web3cli-1.0.5/tests/web3cli/controllers/crud/test_chain_controller.py` & `web3cli-1.1.0/tests/web3cli/controllers/crud/test_chain_controller.py`

 * *Files identical despite different names*

### Comparing `web3cli-1.0.5/tests/web3cli/controllers/crud/test_contract_controller.py` & `web3cli-1.1.0/tests/web3cli/controllers/crud/test_contract_controller.py`

 * *Files identical despite different names*

### Comparing `web3cli-1.0.5/tests/web3cli/controllers/crud/test_history_controller.py` & `web3cli-1.1.0/tests/web3cli/controllers/crud/test_history_controller.py`

 * *Files identical despite different names*

### Comparing `web3cli-1.0.5/tests/web3cli/controllers/crud/test_rpc_controller.py` & `web3cli-1.1.0/tests/web3cli/controllers/crud/test_rpc_controller.py`

 * *Files identical despite different names*

### Comparing `web3cli-1.0.5/tests/web3cli/controllers/crud/test_signer_controller.py` & `web3cli-1.1.0/tests/web3cli/controllers/crud/test_signer_controller.py`

 * *Files identical despite different names*

### Comparing `web3cli-1.0.5/tests/web3cli/controllers/test_appkey_controller.py` & `web3cli-1.1.0/tests/web3cli/controllers/test_appkey_controller.py`

 * *Files identical despite different names*

### Comparing `web3cli-1.0.5/tests/web3cli/controllers/test_call_controller.py` & `web3cli-1.1.0/tests/web3cli/controllers/test_call_controller.py`

 * *Files identical despite different names*

### Comparing `web3cli-1.0.5/tests/web3cli/controllers/test_db_controller.py` & `web3cli-1.1.0/tests/web3cli/controllers/test_db_controller.py`

 * *Files identical despite different names*

### Comparing `web3cli-1.0.5/tests/web3cli/controllers/test_keyfile_controller.py` & `web3cli-1.1.0/tests/web3cli/controllers/test_keyfile_controller.py`

 * *Files identical despite different names*

### Comparing `web3cli-1.0.5/tests/web3cli/controllers/test_misc_controller.py` & `web3cli-1.1.0/tests/web3cli/controllers/test_misc_controller.py`

 * *Files identical despite different names*

### Comparing `web3cli-1.0.5/tests/web3cli/controllers/test_replay_controller.py` & `web3cli-1.1.0/tests/web3cli/controllers/test_replay_controller.py`

 * *Files identical despite different names*

### Comparing `web3cli-1.0.5/tests/web3cli/controllers/test_send_controller.py` & `web3cli-1.1.0/tests/web3cli/controllers/test_send_controller.py`

 * *Files identical despite different names*

### Comparing `web3cli-1.0.5/tests/web3cli/controllers/test_transact_controller.py` & `web3cli-1.1.0/tests/web3cli/controllers/test_transact_controller.py`

 * *Files identical despite different names*

### Comparing `web3cli-1.0.5/tests/web3cli/controllers/test_tx_controller.py` & `web3cli-1.1.0/tests/web3cli/controllers/test_tx_controller.py`

 * *Files identical despite different names*

### Comparing `web3cli-1.0.5/tests/web3cli/fixtures.py` & `web3cli-1.1.0/tests/web3cli/fixtures.py`

 * *Files identical despite different names*

### Comparing `web3cli-1.0.5/tests/web3cli/helpers/test_crypto_helper.py` & `web3cli-1.1.0/tests/web3cli/helpers/test_crypto_helper.py`

 * *Files identical despite different names*

### Comparing `web3cli-1.0.5/tests/web3cli/main.py` & `web3cli-1.1.0/tests/web3cli/main.py`

 * *Files identical despite different names*

### Comparing `web3cli-1.0.5/tests/web3cli/test_db.py` & `web3cli-1.1.0/tests/web3cli/test_db.py`

 * *Files identical despite different names*

### Comparing `web3cli-1.0.5/tests/web3core/fixtures.py` & `web3cli-1.1.0/tests/web3core/fixtures.py`

 * *Files identical despite different names*

### Comparing `web3cli-1.0.5/tests/web3core/helpers/test_abi_helper.py` & `web3cli-1.1.0/tests/web3core/helpers/test_abi_helper.py`

 * *Files identical despite different names*

### Comparing `web3cli-1.0.5/tests/web3core/helpers/test_crypto_helper.py` & `web3cli-1.1.0/tests/web3core/helpers/test_crypto_helper.py`

 * *Files identical despite different names*

### Comparing `web3cli-1.0.5/tests/web3core/helpers/test_resolve_address_helper.py` & `web3cli-1.1.0/tests/web3core/helpers/test_resolve_address_helper.py`

 * *Files identical despite different names*

### Comparing `web3cli-1.0.5/tests/web3core/helpers/test_validation_helper.py` & `web3cli-1.1.0/tests/web3core/helpers/test_validation_helper.py`

 * *Files identical despite different names*

### Comparing `web3cli-1.0.5/tests/web3core/models/test_contract_model.py` & `web3cli-1.1.0/tests/web3core/models/test_contract_model.py`

 * *Files identical despite different names*

### Comparing `web3cli-1.0.5/PKG-INFO` & `web3cli-1.1.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: web3cli
-Version: 1.0.5
+Version: 1.1.0
 Summary: Interact with blockchains and smart contracts using the command line
 License: MIT
 Keywords: web3,w3,cli,evm,blockchain,ethereum,binance,avalanche
 Author-email: coccoinomane <coccoinomane@gmail.com>
 Requires-Python: >=3.9,<3.11
 Project-URL: homepage, https://github.com/coccoinomane/web3cli
 Project-URL: repository, https://github.com/coccoinomane/web3cli
@@ -126,16 +126,16 @@
    ```
    w3 swap uniswap_v2 1 usdc usdt     # swap 1 USDC for USDT on Uniswap
    w3avax swap traderjoe 1 usdc wavax # swap 1 USDC for WAVAX on TraderJoe
    ```
 
 - Replay a given transactions on the blockchain:
    ```
-   tx=`w3arb send unicef 1 USDC --force` # send 1 USDC to Unicef
-   w3 replay $tx                         # re-send 1 USDC to Unicef
+   tx=`w3 send unicef 1 USDC --force` # send 1 USDC to Unicef
+   w3 replay $tx                      # re-send 1 USDC to Unicef
    ```
 
 # Smart Contract support
 
 `web3cli` comes preloaded with some popular smart contracts, including ERC20 tokens and Uniswap clones.
 
 See the available contracts with `w3 contract list`:
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: web3cli Version: 1.0.5 Summary: Interact with
+Metadata-Version: 2.1 Name: web3cli Version: 1.1.0 Summary: Interact with
 blockchains and smart contracts using the command line License: MIT Keywords:
 web3,w3,cli,evm,blockchain,ethereum,binance,avalanche Author-email:
 coccoinomane
 gmail.com> Requires-Python: >=3.9,<3.11 Project-URL: homepage, https://
 github.com/coccoinomane/web3cli Project-URL: repository, https://github.com/
 coccoinomane/web3cli Description-Content-Type: text/markdown
 [https://img.shields.io/github/commit-activity/m/badges/shields?color=009051]
@@ -47,28 +47,28 @@
 Output-processing)): ```bash w3 block latest | jq -r '.baseFeePerGas' ``` -
 Sign messages: ```bash w3 sign 'Hello world!' ``` # Advanced examples - Send
 coins or tokens to any address: ``` w3 send unicef 1 ETH # send 1 ETH, ask for
 confirmation w3 send unicef 1 ETH gwei # send 1 gwei, ask for confirmation w3
 send unicef 1 usdc # send 1 USDC ``` - Swap tokens on a DEX: ``` w3 swap
 uniswap_v2 1 usdc usdt # swap 1 USDC for USDT on Uniswap w3avax swap traderjoe
 1 usdc wavax # swap 1 USDC for WAVAX on TraderJoe ``` - Replay a given
-transactions on the blockchain: ``` tx=`w3arb send unicef 1 USDC --force` #
-send 1 USDC to Unicef w3 replay $tx # re-send 1 USDC to Unicef ``` # Smart
-Contract support `web3cli` comes preloaded with some popular smart contracts,
-including ERC20 tokens and Uniswap clones. See the available contracts with `w3
-contract list`: ``` w3 contract list # contracts on Ethereum w3 contract list -
--chain bnb # contracts on BNB chain w3 contract list --type erc20 # tokens on
-Ethereum ``` You can also add custom contracts with `w3 contract add`: ``` w3
-contract add weth 0xC02aaA39b223FE8D0A0e5C4F27eAD9083C756Cc2 --type erc20 w3
-contract add sushi 0xd9e1cE17f2641f24aE83637ab66a2cca9C378B9F --type uniswap_v2
-``` To add or list new tokens, you can use the `w3 token` shorthand: ``` w3
-token add weth 0xC02aaA39b223FE8D0A0e5C4F27eAD9083C756Cc2 w3 token list w3
-token delete weth ``` See available functions and events on a contract with `w3
-abi functions` and `w3 abi events`: ``` w3 abi fns weth # functions on WETH
-token w3 abi evs uniswap_v2 # events on Uniswap V2 w3 abi fns --abi abi.json #
+transactions on the blockchain: ``` tx=`w3 send unicef 1 USDC --force` # send 1
+USDC to Unicef w3 replay $tx # re-send 1 USDC to Unicef ``` # Smart Contract
+support `web3cli` comes preloaded with some popular smart contracts, including
+ERC20 tokens and Uniswap clones. See the available contracts with `w3 contract
+list`: ``` w3 contract list # contracts on Ethereum w3 contract list --chain
+bnb # contracts on BNB chain w3 contract list --type erc20 # tokens on Ethereum
+``` You can also add custom contracts with `w3 contract add`: ``` w3 contract
+add weth 0xC02aaA39b223FE8D0A0e5C4F27eAD9083C756Cc2 --type erc20 w3 contract
+add sushi 0xd9e1cE17f2641f24aE83637ab66a2cca9C378B9F --type uniswap_v2 ``` To
+add or list new tokens, you can use the `w3 token` shorthand: ``` w3 token add
+weth 0xC02aaA39b223FE8D0A0e5C4F27eAD9083C756Cc2 w3 token list w3 token delete
+weth ``` See available functions and events on a contract with `w3 abi
+functions` and `w3 abi events`: ``` w3 abi fns weth # functions on WETH token
+w3 abi evs uniswap_v2 # events on Uniswap V2 w3 abi fns --abi abi.json #
 functions of an arbitrary ABI ``` ### Read from a smart contract To read from a
 smart contract, use `w3 call`. For example, to get the total supply of the WETH
 token, run: ``` w3 call weth totalSupply ``` Function arguments are parsed
 automatically, so you can call `balanceOf` with: ``` w3 call weth balanceOf
 0xA59B29d7dbC9794d1e7f45123C48b2b8d0a34636 ``` You can also do more complex
 stuff like: ```bash # get the amount of USDT you get for 100 USDC w3 call
 uniswap_v2 getAmountsOut 100e6 usdc,usdt | jq -r '.[1]' ``` ### Send a
```

