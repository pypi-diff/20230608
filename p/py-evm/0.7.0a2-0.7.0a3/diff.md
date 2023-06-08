# Comparing `tmp/py-evm-0.7.0a2.tar.gz` & `tmp/py-evm-0.7.0a3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py-evm-0.7.0a2.tar", last modified: Thu May 11 21:31:06 2023, max compression
+gzip compressed data, was "py-evm-0.7.0a3.tar", last modified: Thu Jun  8 20:25:34 2023, max compression
```

## Comparing `py-evm-0.7.0a2.tar` & `py-evm-0.7.0a3.tar`

### file list

```diff
@@ -1,337 +1,337 @@
-drwxr-xr-x   0 fselmo     (501) staff       (20)        0 2023-05-11 21:31:06.470517 py-evm-0.7.0a2/
--rw-r--r--   0 fselmo     (501) staff       (20)     1095 2023-04-28 21:58:38.000000 py-evm-0.7.0a2/LICENSE
--rw-r--r--   0 fselmo     (501) staff       (20)      141 2023-04-28 21:58:38.000000 py-evm-0.7.0a2/MANIFEST.in
--rw-r--r--   0 fselmo     (501) staff       (20)     2976 2023-05-11 21:31:06.469745 py-evm-0.7.0a2/PKG-INFO
--rw-r--r--   0 fselmo     (501) staff       (20)     2157 2023-04-28 21:58:38.000000 py-evm-0.7.0a2/README.md
-drwxr-xr-x   0 fselmo     (501) staff       (20)        0 2023-05-11 21:31:06.132414 py-evm-0.7.0a2/eth/
--rw-r--r--   0 fselmo     (501) staff       (20)      368 2021-10-11 18:18:14.000000 py-evm-0.7.0a2/eth/__init__.py
-drwxr-xr-x   0 fselmo     (501) staff       (20)        0 2023-05-11 21:31:06.142130 py-evm-0.7.0a2/eth/_utils/
--rw-r--r--   0 fselmo     (501) staff       (20)        0 2021-10-11 18:18:14.000000 py-evm-0.7.0a2/eth/_utils/__init__.py
--rw-r--r--   0 fselmo     (501) staff       (20)      687 2023-05-11 21:18:28.000000 py-evm-0.7.0a2/eth/_utils/address.py
-drwxr-xr-x   0 fselmo     (501) staff       (20)        0 2023-05-11 21:31:06.144715 py-evm-0.7.0a2/eth/_utils/blake2/
--rw-r--r--   0 fselmo     (501) staff       (20)        0 2021-10-11 18:18:14.000000 py-evm-0.7.0a2/eth/_utils/blake2/__init__.py
--rw-r--r--   0 fselmo     (501) staff       (20)     1841 2023-05-11 21:18:28.000000 py-evm-0.7.0a2/eth/_utils/blake2/coders.py
--rwxr-xr-x   0 fselmo     (501) staff       (20)     5793 2023-05-11 21:18:28.000000 py-evm-0.7.0a2/eth/_utils/blake2/compression.py
--rw-r--r--   0 fselmo     (501) staff       (20)      980 2023-05-11 21:18:28.000000 py-evm-0.7.0a2/eth/_utils/bn128.py
--rw-r--r--   0 fselmo     (501) staff       (20)     3924 2023-05-11 21:18:28.000000 py-evm-0.7.0a2/eth/_utils/datatypes.py
--rw-r--r--   0 fselmo     (501) staff       (20)     1013 2023-05-11 21:18:28.000000 py-evm-0.7.0a2/eth/_utils/db.py
--rw-r--r--   0 fselmo     (501) staff       (20)       40 2021-10-11 18:18:14.000000 py-evm-0.7.0a2/eth/_utils/empty.py
--rw-r--r--   0 fselmo     (501) staff       (20)     8124 2023-05-11 21:18:28.000000 py-evm-0.7.0a2/eth/_utils/env.py
--rw-r--r--   0 fselmo     (501) staff       (20)      612 2023-05-11 21:18:28.000000 py-evm-0.7.0a2/eth/_utils/generator.py
--rw-r--r--   0 fselmo     (501) staff       (20)     5024 2023-05-11 21:18:28.000000 py-evm-0.7.0a2/eth/_utils/headers.py
--rw-r--r--   0 fselmo     (501) staff       (20)        0 2021-10-11 18:18:14.000000 py-evm-0.7.0a2/eth/_utils/logging.py
--rw-r--r--   0 fselmo     (501) staff       (20)     1540 2023-05-11 21:18:28.000000 py-evm-0.7.0a2/eth/_utils/module_loading.py
--rw-r--r--   0 fselmo     (501) staff       (20)     2671 2023-05-11 21:18:28.000000 py-evm-0.7.0a2/eth/_utils/numeric.py
--rw-r--r--   0 fselmo     (501) staff       (20)      337 2023-05-11 21:18:28.000000 py-evm-0.7.0a2/eth/_utils/padding.py
--rw-r--r--   0 fselmo     (501) staff       (20)     3284 2023-05-11 21:18:28.000000 py-evm-0.7.0a2/eth/_utils/rlp.py
--rw-r--r--   0 fselmo     (501) staff       (20)     1749 2023-05-11 21:18:28.000000 py-evm-0.7.0a2/eth/_utils/spoof.py
--rw-r--r--   0 fselmo     (501) staff       (20)     1343 2023-05-11 21:18:28.000000 py-evm-0.7.0a2/eth/_utils/state.py
--rw-r--r--   0 fselmo     (501) staff       (20)     3379 2023-05-11 21:18:28.000000 py-evm-0.7.0a2/eth/_utils/transactions.py
--rw-r--r--   0 fselmo     (501) staff       (20)      385 2023-05-11 21:18:28.000000 py-evm-0.7.0a2/eth/_utils/version.py
--rw-r--r--   0 fselmo     (501) staff       (20)      364 2023-05-11 21:18:28.000000 py-evm-0.7.0a2/eth/_warnings.py
--rw-r--r--   0 fselmo     (501) staff       (20)   117125 2023-05-11 21:18:28.000000 py-evm-0.7.0a2/eth/abc.py
-drwxr-xr-x   0 fselmo     (501) staff       (20)        0 2023-05-11 21:31:06.146869 py-evm-0.7.0a2/eth/chains/
--rw-r--r--   0 fselmo     (501) staff       (20)      223 2021-10-11 18:18:14.000000 py-evm-0.7.0a2/eth/chains/__init__.py
--rw-r--r--   0 fselmo     (501) staff       (20)    25965 2023-05-11 21:18:28.000000 py-evm-0.7.0a2/eth/chains/base.py
-drwxr-xr-x   0 fselmo     (501) staff       (20)        0 2023-05-11 21:31:06.148085 py-evm-0.7.0a2/eth/chains/goerli/
--rw-r--r--   0 fselmo     (501) staff       (20)     1305 2023-05-11 21:18:28.000000 py-evm-0.7.0a2/eth/chains/goerli/__init__.py
--rw-r--r--   0 fselmo     (501) staff       (20)      270 2023-05-11 21:18:28.000000 py-evm-0.7.0a2/eth/chains/goerli/constants.py
--rw-r--r--   0 fselmo     (501) staff       (20)     2554 2023-05-11 21:18:28.000000 py-evm-0.7.0a2/eth/chains/header.py
-drwxr-xr-x   0 fselmo     (501) staff       (20)        0 2023-05-11 21:31:06.149533 py-evm-0.7.0a2/eth/chains/mainnet/
--rw-r--r--   0 fselmo     (501) staff       (20)     4409 2023-05-11 21:18:28.000000 py-evm-0.7.0a2/eth/chains/mainnet/__init__.py
--rw-r--r--   0 fselmo     (501) staff       (20)     1199 2023-05-11 21:18:28.000000 py-evm-0.7.0a2/eth/chains/mainnet/constants.py
-drwxr-xr-x   0 fselmo     (501) staff       (20)        0 2023-05-11 21:31:06.150947 py-evm-0.7.0a2/eth/chains/ropsten/
--rw-r--r--   0 fselmo     (501) staff       (20)     2131 2023-05-11 21:18:28.000000 py-evm-0.7.0a2/eth/chains/ropsten/__init__.py
--rw-r--r--   0 fselmo     (501) staff       (20)      847 2023-05-11 21:18:28.000000 py-evm-0.7.0a2/eth/chains/ropsten/constants.py
-drwxr-xr-x   0 fselmo     (501) staff       (20)        0 2023-05-11 21:31:06.151666 py-evm-0.7.0a2/eth/chains/tester/
--rw-r--r--   0 fselmo     (501) staff       (20)     5919 2023-05-11 21:18:28.000000 py-evm-0.7.0a2/eth/chains/tester/__init__.py
-drwxr-xr-x   0 fselmo     (501) staff       (20)        0 2023-05-11 21:31:06.155213 py-evm-0.7.0a2/eth/consensus/
--rw-r--r--   0 fselmo     (501) staff       (20)      313 2022-06-06 17:44:51.000000 py-evm-0.7.0a2/eth/consensus/__init__.py
--rw-r--r--   0 fselmo     (501) staff       (20)      968 2023-05-11 21:18:28.000000 py-evm-0.7.0a2/eth/consensus/applier.py
-drwxr-xr-x   0 fselmo     (501) staff       (20)        0 2023-05-11 21:31:06.159710 py-evm-0.7.0a2/eth/consensus/clique/
--rw-r--r--   0 fselmo     (501) staff       (20)      271 2023-05-11 21:18:28.000000 py-evm-0.7.0a2/eth/consensus/clique/__init__.py
--rw-r--r--   0 fselmo     (501) staff       (20)     5208 2023-05-11 21:18:28.000000 py-evm-0.7.0a2/eth/consensus/clique/_utils.py
--rw-r--r--   0 fselmo     (501) staff       (20)     5383 2023-05-11 21:18:28.000000 py-evm-0.7.0a2/eth/consensus/clique/clique.py
--rw-r--r--   0 fselmo     (501) staff       (20)      486 2023-05-11 21:18:28.000000 py-evm-0.7.0a2/eth/consensus/clique/constants.py
--rw-r--r--   0 fselmo     (501) staff       (20)     3368 2023-05-11 21:18:28.000000 py-evm-0.7.0a2/eth/consensus/clique/datatypes.py
--rw-r--r--   0 fselmo     (501) staff       (20)     2949 2023-05-11 21:18:28.000000 py-evm-0.7.0a2/eth/consensus/clique/encoding.py
--rw-r--r--   0 fselmo     (501) staff       (20)      158 2023-05-11 21:18:28.000000 py-evm-0.7.0a2/eth/consensus/clique/exceptions.py
--rw-r--r--   0 fselmo     (501) staff       (20)    11157 2023-05-11 21:18:28.000000 py-evm-0.7.0a2/eth/consensus/clique/snapshot_manager.py
--rw-r--r--   0 fselmo     (501) staff       (20)      187 2023-05-11 21:18:28.000000 py-evm-0.7.0a2/eth/consensus/context.py
--rw-r--r--   0 fselmo     (501) staff       (20)      683 2023-05-11 21:18:28.000000 py-evm-0.7.0a2/eth/consensus/noproof.py
--rw-r--r--   0 fselmo     (501) staff       (20)      819 2023-05-11 21:18:28.000000 py-evm-0.7.0a2/eth/consensus/pos.py
--rw-r--r--   0 fselmo     (501) staff       (20)     4024 2023-05-11 21:18:28.000000 py-evm-0.7.0a2/eth/consensus/pow.py
--rw-r--r--   0 fselmo     (501) staff       (20)     3921 2023-05-11 21:18:28.000000 py-evm-0.7.0a2/eth/constants.py
-drwxr-xr-x   0 fselmo     (501) staff       (20)        0 2023-05-11 21:31:06.172356 py-evm-0.7.0a2/eth/db/
--rw-r--r--   0 fselmo     (501) staff       (20)      730 2023-05-11 21:18:28.000000 py-evm-0.7.0a2/eth/db/__init__.py
--rw-r--r--   0 fselmo     (501) staff       (20)     3460 2023-05-11 21:18:28.000000 py-evm-0.7.0a2/eth/db/accesslog.py
--rw-r--r--   0 fselmo     (501) staff       (20)    24391 2023-05-11 21:18:28.000000 py-evm-0.7.0a2/eth/db/account.py
--rw-r--r--   0 fselmo     (501) staff       (20)     4277 2023-05-11 21:18:28.000000 py-evm-0.7.0a2/eth/db/atomic.py
-drwxr-xr-x   0 fselmo     (501) staff       (20)        0 2023-05-11 21:31:06.174356 py-evm-0.7.0a2/eth/db/backends/
--rw-r--r--   0 fselmo     (501) staff       (20)        0 2021-10-11 18:18:14.000000 py-evm-0.7.0a2/eth/db/backends/__init__.py
--rw-r--r--   0 fselmo     (501) staff       (20)     2513 2023-05-11 21:18:28.000000 py-evm-0.7.0a2/eth/db/backends/base.py
--rw-r--r--   0 fselmo     (501) staff       (20)     4496 2023-05-11 21:18:28.000000 py-evm-0.7.0a2/eth/db/backends/level.py
--rw-r--r--   0 fselmo     (501) staff       (20)      890 2021-10-11 18:18:14.000000 py-evm-0.7.0a2/eth/db/backends/memory.py
--rw-r--r--   0 fselmo     (501) staff       (20)     2874 2023-05-11 21:18:28.000000 py-evm-0.7.0a2/eth/db/batch.py
--rw-r--r--   0 fselmo     (501) staff       (20)      971 2023-05-11 21:18:28.000000 py-evm-0.7.0a2/eth/db/cache.py
--rw-r--r--   0 fselmo     (501) staff       (20)    19178 2023-05-11 21:18:28.000000 py-evm-0.7.0a2/eth/db/chain.py
--rw-r--r--   0 fselmo     (501) staff       (20)     5873 2023-05-11 21:18:28.000000 py-evm-0.7.0a2/eth/db/chain_gaps.py
--rw-r--r--   0 fselmo     (501) staff       (20)     7394 2023-05-11 21:18:28.000000 py-evm-0.7.0a2/eth/db/diff.py
--rw-r--r--   0 fselmo     (501) staff       (20)      506 2023-05-11 21:18:28.000000 py-evm-0.7.0a2/eth/db/hash_trie.py
--rw-r--r--   0 fselmo     (501) staff       (20)    24129 2023-05-11 21:18:28.000000 py-evm-0.7.0a2/eth/db/header.py
--rw-r--r--   0 fselmo     (501) staff       (20)    17008 2023-05-11 21:18:28.000000 py-evm-0.7.0a2/eth/db/journal.py
--rw-r--r--   0 fselmo     (501) staff       (20)     1306 2023-05-11 21:18:28.000000 py-evm-0.7.0a2/eth/db/keymap.py
--rw-r--r--   0 fselmo     (501) staff       (20)     1354 2023-05-11 21:18:28.000000 py-evm-0.7.0a2/eth/db/schema.py
--rw-r--r--   0 fselmo     (501) staff       (20)    16562 2023-05-11 21:18:28.000000 py-evm-0.7.0a2/eth/db/slow_journal.py
--rw-r--r--   0 fselmo     (501) staff       (20)    16442 2023-05-11 21:18:28.000000 py-evm-0.7.0a2/eth/db/storage.py
--rw-r--r--   0 fselmo     (501) staff       (20)     1393 2023-05-11 21:18:28.000000 py-evm-0.7.0a2/eth/db/trie.py
--rw-r--r--   0 fselmo     (501) staff       (20)     1660 2023-05-11 21:18:28.000000 py-evm-0.7.0a2/eth/db/witness.py
-drwxr-xr-x   0 fselmo     (501) staff       (20)        0 2023-05-11 21:31:06.175706 py-evm-0.7.0a2/eth/estimators/
--rw-r--r--   0 fselmo     (501) staff       (20)      514 2023-05-11 21:18:28.000000 py-evm-0.7.0a2/eth/estimators/__init__.py
--rw-r--r--   0 fselmo     (501) staff       (20)     3427 2023-05-11 21:18:28.000000 py-evm-0.7.0a2/eth/estimators/gas.py
--rw-r--r--   0 fselmo     (501) staff       (20)     4115 2023-05-11 21:18:28.000000 py-evm-0.7.0a2/eth/exceptions.py
-drwxr-xr-x   0 fselmo     (501) staff       (20)        0 2023-05-11 21:31:06.181870 py-evm-0.7.0a2/eth/precompiles/
--rw-r--r--   0 fselmo     (501) staff       (20)      398 2021-10-11 18:18:14.000000 py-evm-0.7.0a2/eth/precompiles/__init__.py
--rw-r--r--   0 fselmo     (501) staff       (20)      962 2023-05-11 21:18:28.000000 py-evm-0.7.0a2/eth/precompiles/blake2.py
--rw-r--r--   0 fselmo     (501) staff       (20)     1502 2023-05-11 21:18:28.000000 py-evm-0.7.0a2/eth/precompiles/ecadd.py
--rw-r--r--   0 fselmo     (501) staff       (20)     1390 2023-05-11 21:18:28.000000 py-evm-0.7.0a2/eth/precompiles/ecmul.py
--rw-r--r--   0 fselmo     (501) staff       (20)     3257 2023-05-11 21:18:28.000000 py-evm-0.7.0a2/eth/precompiles/ecpairing.py
--rw-r--r--   0 fselmo     (501) staff       (20)     1512 2023-05-11 21:18:28.000000 py-evm-0.7.0a2/eth/precompiles/ecrecover.py
--rw-r--r--   0 fselmo     (501) staff       (20)      472 2023-05-11 21:18:28.000000 py-evm-0.7.0a2/eth/precompiles/identity.py
--rw-r--r--   0 fselmo     (501) staff       (20)     3934 2023-05-11 21:18:28.000000 py-evm-0.7.0a2/eth/precompiles/modexp.py
--rw-r--r--   0 fselmo     (501) staff       (20)      670 2023-05-11 21:18:28.000000 py-evm-0.7.0a2/eth/precompiles/ripemd160.py
--rw-r--r--   0 fselmo     (501) staff       (20)      541 2023-05-11 21:18:28.000000 py-evm-0.7.0a2/eth/precompiles/sha256.py
--rw-r--r--   0 fselmo     (501) staff       (20)        0 2021-10-11 18:18:14.000000 py-evm-0.7.0a2/eth/py.typed
-drwxr-xr-x   0 fselmo     (501) staff       (20)        0 2023-05-11 21:31:06.189931 py-evm-0.7.0a2/eth/rlp/
--rw-r--r--   0 fselmo     (501) staff       (20)        0 2021-10-11 18:18:14.000000 py-evm-0.7.0a2/eth/rlp/__init__.py
--rw-r--r--   0 fselmo     (501) staff       (20)     1022 2023-05-11 21:18:28.000000 py-evm-0.7.0a2/eth/rlp/accounts.py
--rw-r--r--   0 fselmo     (501) staff       (20)      904 2023-05-11 21:18:28.000000 py-evm-0.7.0a2/eth/rlp/blocks.py
--rw-r--r--   0 fselmo     (501) staff       (20)     5417 2023-05-11 21:18:28.000000 py-evm-0.7.0a2/eth/rlp/headers.py
--rw-r--r--   0 fselmo     (501) staff       (20)      603 2023-05-11 21:18:28.000000 py-evm-0.7.0a2/eth/rlp/logs.py
--rw-r--r--   0 fselmo     (501) staff       (20)     1285 2023-05-11 21:18:28.000000 py-evm-0.7.0a2/eth/rlp/receipts.py
--rw-r--r--   0 fselmo     (501) staff       (20)      387 2023-05-11 21:18:28.000000 py-evm-0.7.0a2/eth/rlp/sedes.py
--rw-r--r--   0 fselmo     (501) staff       (20)     3611 2023-05-11 21:18:28.000000 py-evm-0.7.0a2/eth/rlp/transactions.py
-drwxr-xr-x   0 fselmo     (501) staff       (20)        0 2023-05-11 21:31:06.192185 py-evm-0.7.0a2/eth/tools/
--rw-r--r--   0 fselmo     (501) staff       (20)        0 2021-10-11 18:18:14.000000 py-evm-0.7.0a2/eth/tools/__init__.py
-drwxr-xr-x   0 fselmo     (501) staff       (20)        0 2023-05-11 21:31:06.199164 py-evm-0.7.0a2/eth/tools/_utils/
--rw-r--r--   0 fselmo     (501) staff       (20)        0 2021-10-11 18:18:14.000000 py-evm-0.7.0a2/eth/tools/_utils/__init__.py
--rw-r--r--   0 fselmo     (501) staff       (20)      636 2023-05-11 21:18:28.000000 py-evm-0.7.0a2/eth/tools/_utils/deprecation.py
--rw-r--r--   0 fselmo     (501) staff       (20)      190 2023-05-11 21:18:28.000000 py-evm-0.7.0a2/eth/tools/_utils/git.py
--rw-r--r--   0 fselmo     (501) staff       (20)      556 2023-05-11 21:18:28.000000 py-evm-0.7.0a2/eth/tools/_utils/hashing.py
--rw-r--r--   0 fselmo     (501) staff       (20)     1564 2023-05-11 21:18:28.000000 py-evm-0.7.0a2/eth/tools/_utils/mappings.py
--rw-r--r--   0 fselmo     (501) staff       (20)    18084 2023-05-11 21:18:28.000000 py-evm-0.7.0a2/eth/tools/_utils/normalization.py
--rw-r--r--   0 fselmo     (501) staff       (20)     4410 2023-05-11 21:18:28.000000 py-evm-0.7.0a2/eth/tools/_utils/slow_code_stream.py
--rw-r--r--   0 fselmo     (501) staff       (20)      903 2023-05-11 21:18:28.000000 py-evm-0.7.0a2/eth/tools/_utils/vyper.py
-drwxr-xr-x   0 fselmo     (501) staff       (20)        0 2023-05-11 21:31:06.200084 py-evm-0.7.0a2/eth/tools/builder/
--rw-r--r--   0 fselmo     (501) staff       (20)        0 2021-10-11 18:18:14.000000 py-evm-0.7.0a2/eth/tools/builder/__init__.py
-drwxr-xr-x   0 fselmo     (501) staff       (20)        0 2023-05-11 21:31:06.203230 py-evm-0.7.0a2/eth/tools/builder/chain/
--rw-r--r--   0 fselmo     (501) staff       (20)     2936 2023-04-17 23:21:54.000000 py-evm-0.7.0a2/eth/tools/builder/chain/__init__.py
--rw-r--r--   0 fselmo     (501) staff       (20)    15254 2023-05-11 21:18:28.000000 py-evm-0.7.0a2/eth/tools/builder/chain/builders.py
-drwxr-xr-x   0 fselmo     (501) staff       (20)        0 2023-05-11 21:31:06.205942 py-evm-0.7.0a2/eth/tools/db/
--rw-r--r--   0 fselmo     (501) staff       (20)        0 2021-10-11 18:18:14.000000 py-evm-0.7.0a2/eth/tools/db/__init__.py
--rw-r--r--   0 fselmo     (501) staff       (20)     5184 2023-05-11 21:18:28.000000 py-evm-0.7.0a2/eth/tools/db/atomic.py
--rw-r--r--   0 fselmo     (501) staff       (20)     2269 2023-05-11 21:18:28.000000 py-evm-0.7.0a2/eth/tools/db/base.py
-drwxr-xr-x   0 fselmo     (501) staff       (20)        0 2023-05-11 21:31:06.211823 py-evm-0.7.0a2/eth/tools/fixtures/
--rw-r--r--   0 fselmo     (501) staff       (20)      615 2021-10-11 18:18:14.000000 py-evm-0.7.0a2/eth/tools/fixtures/__init__.py
--rw-r--r--   0 fselmo     (501) staff       (20)      887 2023-05-11 21:18:28.000000 py-evm-0.7.0a2/eth/tools/fixtures/_utils.py
-drwxr-xr-x   0 fselmo     (501) staff       (20)        0 2023-05-11 21:31:06.221591 py-evm-0.7.0a2/eth/tools/fixtures/fillers/
--rw-r--r--   0 fselmo     (501) staff       (20)      282 2021-10-11 18:18:14.000000 py-evm-0.7.0a2/eth/tools/fixtures/fillers/__init__.py
--rw-r--r--   0 fselmo     (501) staff       (20)     2456 2023-05-11 21:18:28.000000 py-evm-0.7.0a2/eth/tools/fixtures/fillers/_utils.py
--rw-r--r--   0 fselmo     (501) staff       (20)    12732 2023-05-11 21:18:28.000000 py-evm-0.7.0a2/eth/tools/fixtures/fillers/common.py
--rw-r--r--   0 fselmo     (501) staff       (20)     3461 2023-05-11 21:18:28.000000 py-evm-0.7.0a2/eth/tools/fixtures/fillers/formatters.py
--rw-r--r--   0 fselmo     (501) staff       (20)     1307 2023-05-11 21:18:28.000000 py-evm-0.7.0a2/eth/tools/fixtures/fillers/main.py
--rw-r--r--   0 fselmo     (501) staff       (20)     2758 2023-05-11 21:18:28.000000 py-evm-0.7.0a2/eth/tools/fixtures/fillers/state.py
--rw-r--r--   0 fselmo     (501) staff       (20)     1737 2023-05-11 21:18:28.000000 py-evm-0.7.0a2/eth/tools/fixtures/fillers/vm.py
--rw-r--r--   0 fselmo     (501) staff       (20)     2079 2023-05-11 21:18:28.000000 py-evm-0.7.0a2/eth/tools/fixtures/generation.py
--rw-r--r--   0 fselmo     (501) staff       (20)     9361 2023-05-11 21:18:28.000000 py-evm-0.7.0a2/eth/tools/fixtures/helpers.py
--rw-r--r--   0 fselmo     (501) staff       (20)     3068 2023-05-11 21:18:28.000000 py-evm-0.7.0a2/eth/tools/fixtures/loading.py
--rw-r--r--   0 fselmo     (501) staff       (20)      791 2023-05-11 21:18:28.000000 py-evm-0.7.0a2/eth/tools/mining.py
--rw-r--r--   0 fselmo     (501) staff       (20)      476 2023-05-11 21:18:28.000000 py-evm-0.7.0a2/eth/tools/rlp.py
--rw-r--r--   0 fselmo     (501) staff       (20)     2693 2023-05-11 21:18:28.000000 py-evm-0.7.0a2/eth/typing.py
--rw-r--r--   0 fselmo     (501) staff       (20)     8548 2023-05-11 21:18:28.000000 py-evm-0.7.0a2/eth/validation.py
-drwxr-xr-x   0 fselmo     (501) staff       (20)        0 2023-05-11 21:31:06.243609 py-evm-0.7.0a2/eth/vm/
--rw-r--r--   0 fselmo     (501) staff       (20)        0 2021-10-11 18:18:14.000000 py-evm-0.7.0a2/eth/vm/__init__.py
--rw-r--r--   0 fselmo     (501) staff       (20)    26238 2023-05-11 21:18:28.000000 py-evm-0.7.0a2/eth/vm/base.py
--rw-r--r--   0 fselmo     (501) staff       (20)      632 2023-05-11 21:18:28.000000 py-evm-0.7.0a2/eth/vm/chain_context.py
--rw-r--r--   0 fselmo     (501) staff       (20)     4408 2023-05-11 21:18:28.000000 py-evm-0.7.0a2/eth/vm/code_stream.py
--rw-r--r--   0 fselmo     (501) staff       (20)    19222 2023-05-11 21:18:28.000000 py-evm-0.7.0a2/eth/vm/computation.py
--rw-r--r--   0 fselmo     (501) staff       (20)     2124 2023-05-11 21:18:28.000000 py-evm-0.7.0a2/eth/vm/execution_context.py
-drwxr-xr-x   0 fselmo     (501) staff       (20)        0 2023-05-11 21:31:06.244467 py-evm-0.7.0a2/eth/vm/forks/
--rw-r--r--   0 fselmo     (501) staff       (20)      899 2023-05-04 19:22:49.000000 py-evm-0.7.0a2/eth/vm/forks/__init__.py
-drwxr-xr-x   0 fselmo     (501) staff       (20)        0 2023-05-11 21:31:06.253170 py-evm-0.7.0a2/eth/vm/forks/arrow_glacier/
--rw-r--r--   0 fselmo     (501) staff       (20)      856 2023-05-11 21:18:28.000000 py-evm-0.7.0a2/eth/vm/forks/arrow_glacier/__init__.py
--rw-r--r--   0 fselmo     (501) staff       (20)      993 2023-05-11 21:18:28.000000 py-evm-0.7.0a2/eth/vm/forks/arrow_glacier/blocks.py
--rw-r--r--   0 fselmo     (501) staff       (20)      287 2023-05-11 21:18:28.000000 py-evm-0.7.0a2/eth/vm/forks/arrow_glacier/computation.py
--rw-r--r--   0 fselmo     (501) staff       (20)     1084 2023-05-11 21:18:28.000000 py-evm-0.7.0a2/eth/vm/forks/arrow_glacier/headers.py
--rw-r--r--   0 fselmo     (501) staff       (20)      523 2023-05-11 21:18:28.000000 py-evm-0.7.0a2/eth/vm/forks/arrow_glacier/state.py
--rw-r--r--   0 fselmo     (501) staff       (20)     1134 2023-05-11 21:18:28.000000 py-evm-0.7.0a2/eth/vm/forks/arrow_glacier/transactions.py
-drwxr-xr-x   0 fselmo     (501) staff       (20)        0 2023-05-11 21:31:06.270170 py-evm-0.7.0a2/eth/vm/forks/berlin/
--rw-r--r--   0 fselmo     (501) staff       (20)      772 2023-05-11 21:18:28.000000 py-evm-0.7.0a2/eth/vm/forks/berlin/__init__.py
--rw-r--r--   0 fselmo     (501) staff       (20)      784 2023-05-11 21:18:28.000000 py-evm-0.7.0a2/eth/vm/forks/berlin/blocks.py
--rw-r--r--   0 fselmo     (501) staff       (20)     2441 2023-05-11 21:18:28.000000 py-evm-0.7.0a2/eth/vm/forks/berlin/computation.py
--rw-r--r--   0 fselmo     (501) staff       (20)      327 2021-10-11 18:18:14.000000 py-evm-0.7.0a2/eth/vm/forks/berlin/constants.py
--rw-r--r--   0 fselmo     (501) staff       (20)      374 2023-05-11 21:18:28.000000 py-evm-0.7.0a2/eth/vm/forks/berlin/headers.py
--rw-r--r--   0 fselmo     (501) staff       (20)     6417 2023-05-11 21:18:28.000000 py-evm-0.7.0a2/eth/vm/forks/berlin/logic.py
--rw-r--r--   0 fselmo     (501) staff       (20)     2922 2023-05-11 21:18:28.000000 py-evm-0.7.0a2/eth/vm/forks/berlin/opcodes.py
--rw-r--r--   0 fselmo     (501) staff       (20)     4606 2023-05-11 21:18:28.000000 py-evm-0.7.0a2/eth/vm/forks/berlin/receipts.py
--rw-r--r--   0 fselmo     (501) staff       (20)     1187 2023-05-11 21:18:28.000000 py-evm-0.7.0a2/eth/vm/forks/berlin/state.py
--rw-r--r--   0 fselmo     (501) staff       (20)    15375 2023-05-11 21:18:28.000000 py-evm-0.7.0a2/eth/vm/forks/berlin/transactions.py
-drwxr-xr-x   0 fselmo     (501) staff       (20)        0 2023-05-11 21:31:06.296825 py-evm-0.7.0a2/eth/vm/forks/byzantium/
--rw-r--r--   0 fselmo     (501) staff       (20)     3584 2023-05-11 21:18:28.000000 py-evm-0.7.0a2/eth/vm/forks/byzantium/__init__.py
--rw-r--r--   0 fselmo     (501) staff       (20)      485 2023-05-11 21:18:28.000000 py-evm-0.7.0a2/eth/vm/forks/byzantium/blocks.py
--rw-r--r--   0 fselmo     (501) staff       (20)     1016 2023-05-11 21:18:28.000000 py-evm-0.7.0a2/eth/vm/forks/byzantium/computation.py
--rw-r--r--   0 fselmo     (501) staff       (20)      235 2023-05-11 21:18:28.000000 py-evm-0.7.0a2/eth/vm/forks/byzantium/constants.py
--rw-r--r--   0 fselmo     (501) staff       (20)     3368 2023-05-11 21:18:28.000000 py-evm-0.7.0a2/eth/vm/forks/byzantium/headers.py
--rw-r--r--   0 fselmo     (501) staff       (20)     3526 2023-05-11 21:18:28.000000 py-evm-0.7.0a2/eth/vm/forks/byzantium/opcodes.py
--rw-r--r--   0 fselmo     (501) staff       (20)      222 2023-05-11 21:18:28.000000 py-evm-0.7.0a2/eth/vm/forks/byzantium/state.py
--rw-r--r--   0 fselmo     (501) staff       (20)     1231 2023-05-11 21:18:28.000000 py-evm-0.7.0a2/eth/vm/forks/byzantium/transactions.py
-drwxr-xr-x   0 fselmo     (501) staff       (20)        0 2023-05-11 21:31:06.328039 py-evm-0.7.0a2/eth/vm/forks/constantinople/
--rw-r--r--   0 fselmo     (501) staff       (20)     1106 2023-05-11 21:18:28.000000 py-evm-0.7.0a2/eth/vm/forks/constantinople/__init__.py
--rw-r--r--   0 fselmo     (501) staff       (20)      484 2023-05-11 21:18:28.000000 py-evm-0.7.0a2/eth/vm/forks/constantinople/blocks.py
--rw-r--r--   0 fselmo     (501) staff       (20)      757 2023-05-11 21:18:28.000000 py-evm-0.7.0a2/eth/vm/forks/constantinople/computation.py
--rw-r--r--   0 fselmo     (501) staff       (20)      329 2023-05-11 21:18:28.000000 py-evm-0.7.0a2/eth/vm/forks/constantinople/constants.py
--rw-r--r--   0 fselmo     (501) staff       (20)      406 2023-05-11 21:18:28.000000 py-evm-0.7.0a2/eth/vm/forks/constantinople/headers.py
--rw-r--r--   0 fselmo     (501) staff       (20)     1574 2023-05-11 21:18:28.000000 py-evm-0.7.0a2/eth/vm/forks/constantinople/opcodes.py
--rw-r--r--   0 fselmo     (501) staff       (20)      221 2023-05-11 21:18:28.000000 py-evm-0.7.0a2/eth/vm/forks/constantinople/state.py
--rw-r--r--   0 fselmo     (501) staff       (20)      334 2023-05-11 21:18:28.000000 py-evm-0.7.0a2/eth/vm/forks/constantinople/storage.py
--rw-r--r--   0 fselmo     (501) staff       (20)     1235 2023-05-11 21:18:28.000000 py-evm-0.7.0a2/eth/vm/forks/constantinople/transactions.py
-drwxr-xr-x   0 fselmo     (501) staff       (20)        0 2023-05-11 21:31:06.354068 py-evm-0.7.0a2/eth/vm/forks/frontier/
--rw-r--r--   0 fselmo     (501) staff       (20)     3732 2023-05-11 21:18:28.000000 py-evm-0.7.0a2/eth/vm/forks/frontier/__init__.py
--rw-r--r--   0 fselmo     (501) staff       (20)     3412 2023-05-11 21:18:28.000000 py-evm-0.7.0a2/eth/vm/forks/frontier/blocks.py
--rw-r--r--   0 fselmo     (501) staff       (20)     3715 2023-05-11 21:18:28.000000 py-evm-0.7.0a2/eth/vm/forks/frontier/computation.py
--rw-r--r--   0 fselmo     (501) staff       (20)       96 2021-10-11 18:18:14.000000 py-evm-0.7.0a2/eth/vm/forks/frontier/constants.py
--rw-r--r--   0 fselmo     (501) staff       (20)     3529 2023-05-11 21:18:28.000000 py-evm-0.7.0a2/eth/vm/forks/frontier/headers.py
--rw-r--r--   0 fselmo     (501) staff       (20)    20228 2023-05-11 21:18:28.000000 py-evm-0.7.0a2/eth/vm/forks/frontier/opcodes.py
--rw-r--r--   0 fselmo     (501) staff       (20)     7686 2023-05-11 21:18:28.000000 py-evm-0.7.0a2/eth/vm/forks/frontier/state.py
--rw-r--r--   0 fselmo     (501) staff       (20)      140 2023-05-11 21:18:28.000000 py-evm-0.7.0a2/eth/vm/forks/frontier/transaction_context.py
--rw-r--r--   0 fselmo     (501) staff       (20)     5849 2023-05-11 21:18:28.000000 py-evm-0.7.0a2/eth/vm/forks/frontier/transactions.py
--rw-r--r--   0 fselmo     (501) staff       (20)     1603 2023-05-11 21:18:28.000000 py-evm-0.7.0a2/eth/vm/forks/frontier/validation.py
-drwxr-xr-x   0 fselmo     (501) staff       (20)        0 2023-05-11 21:31:06.360109 py-evm-0.7.0a2/eth/vm/forks/gray_glacier/
--rw-r--r--   0 fselmo     (501) staff       (20)      855 2023-05-11 21:18:28.000000 py-evm-0.7.0a2/eth/vm/forks/gray_glacier/__init__.py
--rw-r--r--   0 fselmo     (501) staff       (20)     1068 2023-05-11 21:18:28.000000 py-evm-0.7.0a2/eth/vm/forks/gray_glacier/blocks.py
--rw-r--r--   0 fselmo     (501) staff       (20)      317 2023-05-11 21:18:28.000000 py-evm-0.7.0a2/eth/vm/forks/gray_glacier/computation.py
--rw-r--r--   0 fselmo     (501) staff       (20)     1119 2023-05-11 21:18:28.000000 py-evm-0.7.0a2/eth/vm/forks/gray_glacier/headers.py
--rw-r--r--   0 fselmo     (501) staff       (20)      556 2023-05-11 21:18:28.000000 py-evm-0.7.0a2/eth/vm/forks/gray_glacier/state.py
--rw-r--r--   0 fselmo     (501) staff       (20)     1170 2023-05-11 21:18:28.000000 py-evm-0.7.0a2/eth/vm/forks/gray_glacier/transactions.py
-drwxr-xr-x   0 fselmo     (501) staff       (20)        0 2023-05-11 21:31:06.369439 py-evm-0.7.0a2/eth/vm/forks/homestead/
--rw-r--r--   0 fselmo     (501) staff       (20)     1250 2023-05-11 21:18:28.000000 py-evm-0.7.0a2/eth/vm/forks/homestead/__init__.py
--rw-r--r--   0 fselmo     (501) staff       (20)      466 2023-05-11 21:18:28.000000 py-evm-0.7.0a2/eth/vm/forks/homestead/blocks.py
--rw-r--r--   0 fselmo     (501) staff       (20)     2289 2023-05-11 21:18:28.000000 py-evm-0.7.0a2/eth/vm/forks/homestead/computation.py
--rw-r--r--   0 fselmo     (501) staff       (20)       61 2021-10-11 18:18:14.000000 py-evm-0.7.0a2/eth/vm/forks/homestead/constants.py
--rw-r--r--   0 fselmo     (501) staff       (20)     9656 2023-05-11 21:18:28.000000 py-evm-0.7.0a2/eth/vm/forks/homestead/headers.py
--rw-r--r--   0 fselmo     (501) staff       (20)      637 2023-05-11 21:18:28.000000 py-evm-0.7.0a2/eth/vm/forks/homestead/opcodes.py
--rw-r--r--   0 fselmo     (501) staff       (20)      640 2023-05-11 21:18:28.000000 py-evm-0.7.0a2/eth/vm/forks/homestead/state.py
--rw-r--r--   0 fselmo     (501) staff       (20)     2197 2023-05-11 21:18:28.000000 py-evm-0.7.0a2/eth/vm/forks/homestead/transactions.py
--rw-r--r--   0 fselmo     (501) staff       (20)      518 2023-05-11 21:18:28.000000 py-evm-0.7.0a2/eth/vm/forks/homestead/validation.py
-drwxr-xr-x   0 fselmo     (501) staff       (20)        0 2023-05-11 21:31:06.378364 py-evm-0.7.0a2/eth/vm/forks/istanbul/
--rw-r--r--   0 fselmo     (501) staff       (20)      817 2023-05-11 21:18:28.000000 py-evm-0.7.0a2/eth/vm/forks/istanbul/__init__.py
--rw-r--r--   0 fselmo     (501) staff       (20)      469 2023-05-11 21:18:28.000000 py-evm-0.7.0a2/eth/vm/forks/istanbul/blocks.py
--rw-r--r--   0 fselmo     (501) staff       (20)     1421 2023-05-11 21:18:28.000000 py-evm-0.7.0a2/eth/vm/forks/istanbul/computation.py
--rw-r--r--   0 fselmo     (501) staff       (20)      316 2021-10-11 18:18:14.000000 py-evm-0.7.0a2/eth/vm/forks/istanbul/constants.py
--rw-r--r--   0 fselmo     (501) staff       (20)      384 2023-05-11 21:18:28.000000 py-evm-0.7.0a2/eth/vm/forks/istanbul/headers.py
--rw-r--r--   0 fselmo     (501) staff       (20)     1664 2023-05-11 21:18:28.000000 py-evm-0.7.0a2/eth/vm/forks/istanbul/opcodes.py
--rw-r--r--   0 fselmo     (501) staff       (20)      206 2023-05-11 21:18:28.000000 py-evm-0.7.0a2/eth/vm/forks/istanbul/state.py
--rw-r--r--   0 fselmo     (501) staff       (20)      909 2023-05-11 21:18:28.000000 py-evm-0.7.0a2/eth/vm/forks/istanbul/storage.py
--rw-r--r--   0 fselmo     (501) staff       (20)     1798 2023-05-11 21:18:28.000000 py-evm-0.7.0a2/eth/vm/forks/istanbul/transactions.py
-drwxr-xr-x   0 fselmo     (501) staff       (20)        0 2023-05-11 21:31:06.390946 py-evm-0.7.0a2/eth/vm/forks/london/
--rw-r--r--   0 fselmo     (501) staff       (20)     2260 2023-05-11 21:18:28.000000 py-evm-0.7.0a2/eth/vm/forks/london/__init__.py
--rw-r--r--   0 fselmo     (501) staff       (20)     5828 2023-05-11 21:18:28.000000 py-evm-0.7.0a2/eth/vm/forks/london/blocks.py
--rw-r--r--   0 fselmo     (501) staff       (20)      810 2023-05-11 21:18:28.000000 py-evm-0.7.0a2/eth/vm/forks/london/computation.py
--rw-r--r--   0 fselmo     (501) staff       (20)      470 2023-05-11 21:18:28.000000 py-evm-0.7.0a2/eth/vm/forks/london/constants.py
--rw-r--r--   0 fselmo     (501) staff       (20)     5618 2023-05-11 21:18:28.000000 py-evm-0.7.0a2/eth/vm/forks/london/headers.py
--rw-r--r--   0 fselmo     (501) staff       (20)      895 2023-05-11 21:18:28.000000 py-evm-0.7.0a2/eth/vm/forks/london/opcodes.py
--rw-r--r--   0 fselmo     (501) staff       (20)      629 2023-05-11 21:18:28.000000 py-evm-0.7.0a2/eth/vm/forks/london/receipts.py
--rw-r--r--   0 fselmo     (501) staff       (20)     4881 2023-05-11 21:18:28.000000 py-evm-0.7.0a2/eth/vm/forks/london/state.py
--rw-r--r--   0 fselmo     (501) staff       (20)      544 2023-05-11 21:18:28.000000 py-evm-0.7.0a2/eth/vm/forks/london/storage.py
--rw-r--r--   0 fselmo     (501) staff       (20)     9466 2023-05-11 21:18:28.000000 py-evm-0.7.0a2/eth/vm/forks/london/transactions.py
--rw-r--r--   0 fselmo     (501) staff       (20)      855 2023-05-11 21:18:28.000000 py-evm-0.7.0a2/eth/vm/forks/london/validation.py
-drwxr-xr-x   0 fselmo     (501) staff       (20)        0 2023-05-11 21:31:06.399860 py-evm-0.7.0a2/eth/vm/forks/muir_glacier/
--rw-r--r--   0 fselmo     (501) staff       (20)      842 2023-05-11 21:18:28.000000 py-evm-0.7.0a2/eth/vm/forks/muir_glacier/__init__.py
--rw-r--r--   0 fselmo     (501) staff       (20)      472 2023-05-11 21:18:28.000000 py-evm-0.7.0a2/eth/vm/forks/muir_glacier/blocks.py
--rw-r--r--   0 fselmo     (501) staff       (20)      537 2023-05-11 21:18:28.000000 py-evm-0.7.0a2/eth/vm/forks/muir_glacier/computation.py
--rw-r--r--   0 fselmo     (501) staff       (20)      443 2023-05-11 21:18:28.000000 py-evm-0.7.0a2/eth/vm/forks/muir_glacier/headers.py
--rw-r--r--   0 fselmo     (501) staff       (20)      137 2023-05-11 21:18:28.000000 py-evm-0.7.0a2/eth/vm/forks/muir_glacier/opcodes.py
--rw-r--r--   0 fselmo     (501) staff       (20)      209 2023-05-11 21:18:28.000000 py-evm-0.7.0a2/eth/vm/forks/muir_glacier/state.py
--rw-r--r--   0 fselmo     (501) staff       (20)     1212 2023-05-11 21:18:28.000000 py-evm-0.7.0a2/eth/vm/forks/muir_glacier/transactions.py
-drwxr-xr-x   0 fselmo     (501) staff       (20)        0 2023-05-11 21:31:06.406971 py-evm-0.7.0a2/eth/vm/forks/paris/
--rw-r--r--   0 fselmo     (501) staff       (20)     2117 2023-05-11 21:18:28.000000 py-evm-0.7.0a2/eth/vm/forks/paris/__init__.py
--rw-r--r--   0 fselmo     (501) staff       (20)     1039 2023-05-11 21:18:28.000000 py-evm-0.7.0a2/eth/vm/forks/paris/blocks.py
--rw-r--r--   0 fselmo     (501) staff       (20)      379 2023-05-11 21:18:28.000000 py-evm-0.7.0a2/eth/vm/forks/paris/computation.py
--rw-r--r--   0 fselmo     (501) staff       (20)     2284 2023-05-11 21:18:28.000000 py-evm-0.7.0a2/eth/vm/forks/paris/headers.py
--rw-r--r--   0 fselmo     (501) staff       (20)      686 2023-05-11 21:18:28.000000 py-evm-0.7.0a2/eth/vm/forks/paris/opcodes.py
--rw-r--r--   0 fselmo     (501) staff       (20)      666 2023-05-11 21:18:28.000000 py-evm-0.7.0a2/eth/vm/forks/paris/state.py
--rw-r--r--   0 fselmo     (501) staff       (20)     1121 2023-05-11 21:18:28.000000 py-evm-0.7.0a2/eth/vm/forks/paris/transactions.py
-drwxr-xr-x   0 fselmo     (501) staff       (20)        0 2023-05-11 21:31:06.416338 py-evm-0.7.0a2/eth/vm/forks/petersburg/
--rw-r--r--   0 fselmo     (501) staff       (20)     1036 2023-05-11 21:18:28.000000 py-evm-0.7.0a2/eth/vm/forks/petersburg/__init__.py
--rw-r--r--   0 fselmo     (501) staff       (20)      472 2023-05-11 21:18:28.000000 py-evm-0.7.0a2/eth/vm/forks/petersburg/blocks.py
--rw-r--r--   0 fselmo     (501) staff       (20)      531 2023-05-11 21:18:28.000000 py-evm-0.7.0a2/eth/vm/forks/petersburg/computation.py
--rw-r--r--   0 fselmo     (501) staff       (20)      110 2023-05-11 21:18:28.000000 py-evm-0.7.0a2/eth/vm/forks/petersburg/constants.py
--rw-r--r--   0 fselmo     (501) staff       (20)      386 2023-05-11 21:18:28.000000 py-evm-0.7.0a2/eth/vm/forks/petersburg/headers.py
--rw-r--r--   0 fselmo     (501) staff       (20)     1399 2023-05-11 21:18:28.000000 py-evm-0.7.0a2/eth/vm/forks/petersburg/opcodes.py
--rw-r--r--   0 fselmo     (501) staff       (20)      209 2023-05-11 21:18:28.000000 py-evm-0.7.0a2/eth/vm/forks/petersburg/state.py
--rw-r--r--   0 fselmo     (501) staff       (20)     1211 2023-05-11 21:18:28.000000 py-evm-0.7.0a2/eth/vm/forks/petersburg/transactions.py
-drwxr-xr-x   0 fselmo     (501) staff       (20)        0 2023-05-11 21:31:06.428399 py-evm-0.7.0a2/eth/vm/forks/shanghai/
--rw-r--r--   0 fselmo     (501) staff       (20)      667 2023-05-11 21:18:28.000000 py-evm-0.7.0a2/eth/vm/forks/shanghai/__init__.py
--rw-r--r--   0 fselmo     (501) staff       (20)     9048 2023-05-11 21:18:28.000000 py-evm-0.7.0a2/eth/vm/forks/shanghai/blocks.py
--rw-r--r--   0 fselmo     (501) staff       (20)     1655 2023-05-11 21:18:28.000000 py-evm-0.7.0a2/eth/vm/forks/shanghai/computation.py
--rw-r--r--   0 fselmo     (501) staff       (20)      196 2023-05-11 21:18:28.000000 py-evm-0.7.0a2/eth/vm/forks/shanghai/constants.py
--rw-r--r--   0 fselmo     (501) staff       (20)      824 2023-05-11 21:18:28.000000 py-evm-0.7.0a2/eth/vm/forks/shanghai/headers.py
--rw-r--r--   0 fselmo     (501) staff       (20)      821 2023-05-11 21:18:28.000000 py-evm-0.7.0a2/eth/vm/forks/shanghai/logic.py
--rw-r--r--   0 fselmo     (501) staff       (20)     1531 2023-05-11 21:18:28.000000 py-evm-0.7.0a2/eth/vm/forks/shanghai/opcodes.py
--rw-r--r--   0 fselmo     (501) staff       (20)      751 2023-05-11 21:18:28.000000 py-evm-0.7.0a2/eth/vm/forks/shanghai/state.py
--rw-r--r--   0 fselmo     (501) staff       (20)     1099 2023-05-11 21:18:28.000000 py-evm-0.7.0a2/eth/vm/forks/shanghai/transactions.py
--rw-r--r--   0 fselmo     (501) staff       (20)     1515 2023-05-11 21:18:28.000000 py-evm-0.7.0a2/eth/vm/forks/shanghai/withdrawals.py
-drwxr-xr-x   0 fselmo     (501) staff       (20)        0 2023-05-11 21:31:06.438268 py-evm-0.7.0a2/eth/vm/forks/spurious_dragon/
--rw-r--r--   0 fselmo     (501) staff       (20)      429 2023-05-11 21:18:28.000000 py-evm-0.7.0a2/eth/vm/forks/spurious_dragon/__init__.py
--rw-r--r--   0 fselmo     (501) staff       (20)     2145 2023-05-11 21:18:28.000000 py-evm-0.7.0a2/eth/vm/forks/spurious_dragon/_utils.py
--rw-r--r--   0 fselmo     (501) staff       (20)      484 2023-05-11 21:18:28.000000 py-evm-0.7.0a2/eth/vm/forks/spurious_dragon/blocks.py
--rw-r--r--   0 fselmo     (501) staff       (20)     3322 2023-05-11 21:18:28.000000 py-evm-0.7.0a2/eth/vm/forks/spurious_dragon/computation.py
--rw-r--r--   0 fselmo     (501) staff       (20)      169 2023-04-17 23:21:54.000000 py-evm-0.7.0a2/eth/vm/forks/spurious_dragon/constants.py
--rw-r--r--   0 fselmo     (501) staff       (20)     1221 2023-05-11 21:18:28.000000 py-evm-0.7.0a2/eth/vm/forks/spurious_dragon/opcodes.py
--rw-r--r--   0 fselmo     (501) staff       (20)     1465 2023-05-11 21:18:28.000000 py-evm-0.7.0a2/eth/vm/forks/spurious_dragon/state.py
--rw-r--r--   0 fselmo     (501) staff       (20)     2866 2023-05-11 21:18:28.000000 py-evm-0.7.0a2/eth/vm/forks/spurious_dragon/transactions.py
-drwxr-xr-x   0 fselmo     (501) staff       (20)        0 2023-05-11 21:31:06.446334 py-evm-0.7.0a2/eth/vm/forks/tangerine_whistle/
--rw-r--r--   0 fselmo     (501) staff       (20)      469 2023-05-11 21:18:28.000000 py-evm-0.7.0a2/eth/vm/forks/tangerine_whistle/__init__.py
--rw-r--r--   0 fselmo     (501) staff       (20)      428 2023-05-11 21:18:28.000000 py-evm-0.7.0a2/eth/vm/forks/tangerine_whistle/computation.py
--rw-r--r--   0 fselmo     (501) staff       (20)      225 2021-10-11 18:18:14.000000 py-evm-0.7.0a2/eth/vm/forks/tangerine_whistle/constants.py
--rw-r--r--   0 fselmo     (501) staff       (20)     2106 2023-05-11 21:18:28.000000 py-evm-0.7.0a2/eth/vm/forks/tangerine_whistle/opcodes.py
--rw-r--r--   0 fselmo     (501) staff       (20)      227 2023-05-11 21:18:28.000000 py-evm-0.7.0a2/eth/vm/forks/tangerine_whistle/state.py
--rw-r--r--   0 fselmo     (501) staff       (20)     2626 2023-05-11 21:18:28.000000 py-evm-0.7.0a2/eth/vm/gas_meter.py
--rw-r--r--   0 fselmo     (501) staff       (20)      540 2023-05-11 21:18:28.000000 py-evm-0.7.0a2/eth/vm/header.py
--rw-r--r--   0 fselmo     (501) staff       (20)     3425 2023-05-11 21:18:28.000000 py-evm-0.7.0a2/eth/vm/interrupt.py
-drwxr-xr-x   0 fselmo     (501) staff       (20)        0 2023-05-11 21:31:06.463876 py-evm-0.7.0a2/eth/vm/logic/
--rw-r--r--   0 fselmo     (501) staff       (20)        0 2021-10-11 18:18:14.000000 py-evm-0.7.0a2/eth/vm/logic/__init__.py
--rw-r--r--   0 fselmo     (501) staff       (20)     4805 2023-05-11 21:18:28.000000 py-evm-0.7.0a2/eth/vm/logic/arithmetic.py
--rw-r--r--   0 fselmo     (501) staff       (20)     1113 2023-05-11 21:18:28.000000 py-evm-0.7.0a2/eth/vm/logic/block.py
--rw-r--r--   0 fselmo     (501) staff       (20)    13394 2023-05-11 21:18:28.000000 py-evm-0.7.0a2/eth/vm/logic/call.py
--rw-r--r--   0 fselmo     (501) staff       (20)     2824 2023-05-11 21:18:28.000000 py-evm-0.7.0a2/eth/vm/logic/comparison.py
--rw-r--r--   0 fselmo     (501) staff       (20)     6418 2023-05-11 21:18:28.000000 py-evm-0.7.0a2/eth/vm/logic/context.py
--rw-r--r--   0 fselmo     (501) staff       (20)      944 2023-05-11 21:18:28.000000 py-evm-0.7.0a2/eth/vm/logic/duplication.py
--rw-r--r--   0 fselmo     (501) staff       (20)     1508 2023-05-11 21:18:28.000000 py-evm-0.7.0a2/eth/vm/logic/flow.py
--rw-r--r--   0 fselmo     (501) staff       (20)      507 2023-05-11 21:18:28.000000 py-evm-0.7.0a2/eth/vm/logic/invalid.py
--rw-r--r--   0 fselmo     (501) staff       (20)     1355 2023-05-11 21:18:28.000000 py-evm-0.7.0a2/eth/vm/logic/logging.py
--rw-r--r--   0 fselmo     (501) staff       (20)     1102 2023-05-11 21:18:28.000000 py-evm-0.7.0a2/eth/vm/logic/memory.py
--rw-r--r--   0 fselmo     (501) staff       (20)      640 2023-05-11 21:18:28.000000 py-evm-0.7.0a2/eth/vm/logic/sha3.py
--rw-r--r--   0 fselmo     (501) staff       (20)     2176 2023-05-11 21:18:28.000000 py-evm-0.7.0a2/eth/vm/logic/stack.py
--rw-r--r--   0 fselmo     (501) staff       (20)     3939 2023-05-11 21:18:28.000000 py-evm-0.7.0a2/eth/vm/logic/storage.py
--rw-r--r--   0 fselmo     (501) staff       (20)      974 2023-05-11 21:18:28.000000 py-evm-0.7.0a2/eth/vm/logic/swap.py
--rw-r--r--   0 fselmo     (501) staff       (20)     9518 2023-05-11 21:18:28.000000 py-evm-0.7.0a2/eth/vm/logic/system.py
--rw-r--r--   0 fselmo     (501) staff       (20)     2134 2023-05-11 21:18:28.000000 py-evm-0.7.0a2/eth/vm/memory.py
--rw-r--r--   0 fselmo     (501) staff       (20)     3214 2023-05-11 21:18:28.000000 py-evm-0.7.0a2/eth/vm/message.py
--rw-r--r--   0 fselmo     (501) staff       (20)     2785 2023-05-11 21:18:28.000000 py-evm-0.7.0a2/eth/vm/mnemonics.py
--rw-r--r--   0 fselmo     (501) staff       (20)     1864 2023-05-11 21:18:28.000000 py-evm-0.7.0a2/eth/vm/opcode.py
--rw-r--r--   0 fselmo     (501) staff       (20)     2432 2023-05-11 21:18:28.000000 py-evm-0.7.0a2/eth/vm/opcode_values.py
--rw-r--r--   0 fselmo     (501) staff       (20)      416 2023-05-11 21:18:28.000000 py-evm-0.7.0a2/eth/vm/spoof.py
--rw-r--r--   0 fselmo     (501) staff       (20)     7713 2023-05-11 21:18:28.000000 py-evm-0.7.0a2/eth/vm/stack.py
--rw-r--r--   0 fselmo     (501) staff       (20)    10406 2023-05-11 21:18:28.000000 py-evm-0.7.0a2/eth/vm/state.py
--rw-r--r--   0 fselmo     (501) staff       (20)      875 2023-05-11 21:18:28.000000 py-evm-0.7.0a2/eth/vm/transaction_context.py
-drwxr-xr-x   0 fselmo     (501) staff       (20)        0 2023-05-11 21:31:06.468847 py-evm-0.7.0a2/py_evm.egg-info/
--rw-r--r--   0 fselmo     (501) staff       (20)     2976 2023-05-11 21:31:02.000000 py-evm-0.7.0a2/py_evm.egg-info/PKG-INFO
--rw-r--r--   0 fselmo     (501) staff       (20)     8485 2023-05-11 21:31:06.000000 py-evm-0.7.0a2/py_evm.egg-info/SOURCES.txt
--rw-r--r--   0 fselmo     (501) staff       (20)        1 2023-05-11 21:31:02.000000 py-evm-0.7.0a2/py_evm.egg-info/dependency_links.txt
--rw-r--r--   0 fselmo     (501) staff       (20)        1 2021-11-19 17:48:51.000000 py-evm-0.7.0a2/py_evm.egg-info/not-zip-safe
--rw-r--r--   0 fselmo     (501) staff       (20)     2141 2023-05-11 21:31:02.000000 py-evm-0.7.0a2/py_evm.egg-info/requires.txt
--rw-r--r--   0 fselmo     (501) staff       (20)        4 2023-05-11 21:31:02.000000 py-evm-0.7.0a2/py_evm.egg-info/top_level.txt
--rw-r--r--   0 fselmo     (501) staff       (20)     1116 2023-04-28 21:58:38.000000 py-evm-0.7.0a2/pyproject.toml
--rw-r--r--   0 fselmo     (501) staff       (20)       38 2023-05-11 21:31:06.470806 py-evm-0.7.0a2/setup.cfg
--rw-r--r--   0 fselmo     (501) staff       (20)     3724 2023-05-11 21:30:18.000000 py-evm-0.7.0a2/setup.py
+drwxr-xr-x   0 eve        (501) staff       (20)        0 2023-06-08 20:25:34.271456 py-evm-0.7.0a3/
+-rw-r--r--   0 eve        (501) staff       (20)     1095 2023-05-01 17:23:48.000000 py-evm-0.7.0a3/LICENSE
+-rw-r--r--   0 eve        (501) staff       (20)      141 2023-05-01 17:23:48.000000 py-evm-0.7.0a3/MANIFEST.in
+-rw-r--r--   0 eve        (501) staff       (20)     2977 2023-06-08 20:25:34.271158 py-evm-0.7.0a3/PKG-INFO
+-rw-r--r--   0 eve        (501) staff       (20)     2157 2023-05-01 17:23:48.000000 py-evm-0.7.0a3/README.md
+drwxr-xr-x   0 eve        (501) staff       (20)        0 2023-06-08 20:25:34.239643 py-evm-0.7.0a3/eth/
+-rw-r--r--   0 eve        (501) staff       (20)      368 2021-02-22 21:36:31.000000 py-evm-0.7.0a3/eth/__init__.py
+drwxr-xr-x   0 eve        (501) staff       (20)        0 2023-06-08 20:25:34.241667 py-evm-0.7.0a3/eth/_utils/
+-rw-r--r--   0 eve        (501) staff       (20)        0 2021-02-22 21:36:31.000000 py-evm-0.7.0a3/eth/_utils/__init__.py
+-rw-r--r--   0 eve        (501) staff       (20)      687 2023-06-02 21:07:53.000000 py-evm-0.7.0a3/eth/_utils/address.py
+drwxr-xr-x   0 eve        (501) staff       (20)        0 2023-06-08 20:25:34.242049 py-evm-0.7.0a3/eth/_utils/blake2/
+-rw-r--r--   0 eve        (501) staff       (20)        0 2022-12-07 18:37:56.000000 py-evm-0.7.0a3/eth/_utils/blake2/__init__.py
+-rw-r--r--   0 eve        (501) staff       (20)     1841 2023-06-02 21:07:53.000000 py-evm-0.7.0a3/eth/_utils/blake2/coders.py
+-rwxr-xr-x   0 eve        (501) staff       (20)     5793 2023-06-02 21:07:53.000000 py-evm-0.7.0a3/eth/_utils/blake2/compression.py
+-rw-r--r--   0 eve        (501) staff       (20)      980 2023-06-02 21:07:53.000000 py-evm-0.7.0a3/eth/_utils/bn128.py
+-rw-r--r--   0 eve        (501) staff       (20)     3924 2023-06-02 21:07:53.000000 py-evm-0.7.0a3/eth/_utils/datatypes.py
+-rw-r--r--   0 eve        (501) staff       (20)     1013 2023-06-02 21:07:53.000000 py-evm-0.7.0a3/eth/_utils/db.py
+-rw-r--r--   0 eve        (501) staff       (20)       40 2021-02-22 21:36:31.000000 py-evm-0.7.0a3/eth/_utils/empty.py
+-rw-r--r--   0 eve        (501) staff       (20)     8124 2023-06-02 21:07:53.000000 py-evm-0.7.0a3/eth/_utils/env.py
+-rw-r--r--   0 eve        (501) staff       (20)      612 2023-06-02 21:07:53.000000 py-evm-0.7.0a3/eth/_utils/generator.py
+-rw-r--r--   0 eve        (501) staff       (20)     5024 2023-06-02 21:07:53.000000 py-evm-0.7.0a3/eth/_utils/headers.py
+-rw-r--r--   0 eve        (501) staff       (20)        0 2022-12-07 18:37:56.000000 py-evm-0.7.0a3/eth/_utils/logging.py
+-rw-r--r--   0 eve        (501) staff       (20)     1540 2023-06-02 21:07:53.000000 py-evm-0.7.0a3/eth/_utils/module_loading.py
+-rw-r--r--   0 eve        (501) staff       (20)     2671 2023-06-02 21:07:53.000000 py-evm-0.7.0a3/eth/_utils/numeric.py
+-rw-r--r--   0 eve        (501) staff       (20)      337 2023-06-02 21:07:53.000000 py-evm-0.7.0a3/eth/_utils/padding.py
+-rw-r--r--   0 eve        (501) staff       (20)     3284 2023-06-02 21:07:53.000000 py-evm-0.7.0a3/eth/_utils/rlp.py
+-rw-r--r--   0 eve        (501) staff       (20)     1749 2023-06-02 21:07:53.000000 py-evm-0.7.0a3/eth/_utils/spoof.py
+-rw-r--r--   0 eve        (501) staff       (20)     1343 2023-06-02 21:07:53.000000 py-evm-0.7.0a3/eth/_utils/state.py
+-rw-r--r--   0 eve        (501) staff       (20)     3379 2023-06-02 21:07:53.000000 py-evm-0.7.0a3/eth/_utils/transactions.py
+-rw-r--r--   0 eve        (501) staff       (20)      385 2023-06-02 21:07:53.000000 py-evm-0.7.0a3/eth/_utils/version.py
+-rw-r--r--   0 eve        (501) staff       (20)      364 2023-06-02 21:07:53.000000 py-evm-0.7.0a3/eth/_warnings.py
+-rw-r--r--   0 eve        (501) staff       (20)   117181 2023-06-08 20:21:10.000000 py-evm-0.7.0a3/eth/abc.py
+drwxr-xr-x   0 eve        (501) staff       (20)        0 2023-06-08 20:25:34.242397 py-evm-0.7.0a3/eth/chains/
+-rw-r--r--   0 eve        (501) staff       (20)      223 2021-02-22 21:36:31.000000 py-evm-0.7.0a3/eth/chains/__init__.py
+-rw-r--r--   0 eve        (501) staff       (20)    25965 2023-06-02 21:07:53.000000 py-evm-0.7.0a3/eth/chains/base.py
+drwxr-xr-x   0 eve        (501) staff       (20)        0 2023-06-08 20:25:34.242652 py-evm-0.7.0a3/eth/chains/goerli/
+-rw-r--r--   0 eve        (501) staff       (20)     1305 2023-06-02 21:07:53.000000 py-evm-0.7.0a3/eth/chains/goerli/__init__.py
+-rw-r--r--   0 eve        (501) staff       (20)      270 2023-06-02 21:07:53.000000 py-evm-0.7.0a3/eth/chains/goerli/constants.py
+-rw-r--r--   0 eve        (501) staff       (20)     2554 2023-06-02 21:07:53.000000 py-evm-0.7.0a3/eth/chains/header.py
+drwxr-xr-x   0 eve        (501) staff       (20)        0 2023-06-08 20:25:34.242876 py-evm-0.7.0a3/eth/chains/mainnet/
+-rw-r--r--   0 eve        (501) staff       (20)     4409 2023-06-02 21:07:53.000000 py-evm-0.7.0a3/eth/chains/mainnet/__init__.py
+-rw-r--r--   0 eve        (501) staff       (20)     1199 2023-06-02 21:07:53.000000 py-evm-0.7.0a3/eth/chains/mainnet/constants.py
+drwxr-xr-x   0 eve        (501) staff       (20)        0 2023-06-08 20:25:34.243084 py-evm-0.7.0a3/eth/chains/ropsten/
+-rw-r--r--   0 eve        (501) staff       (20)     2131 2023-06-02 21:07:53.000000 py-evm-0.7.0a3/eth/chains/ropsten/__init__.py
+-rw-r--r--   0 eve        (501) staff       (20)      847 2023-06-02 21:07:53.000000 py-evm-0.7.0a3/eth/chains/ropsten/constants.py
+drwxr-xr-x   0 eve        (501) staff       (20)        0 2023-06-08 20:25:34.243193 py-evm-0.7.0a3/eth/chains/tester/
+-rw-r--r--   0 eve        (501) staff       (20)     5919 2023-06-02 21:07:53.000000 py-evm-0.7.0a3/eth/chains/tester/__init__.py
+drwxr-xr-x   0 eve        (501) staff       (20)        0 2023-06-08 20:25:34.243864 py-evm-0.7.0a3/eth/consensus/
+-rw-r--r--   0 eve        (501) staff       (20)      313 2021-02-22 21:36:31.000000 py-evm-0.7.0a3/eth/consensus/__init__.py
+-rw-r--r--   0 eve        (501) staff       (20)      968 2023-06-02 21:07:53.000000 py-evm-0.7.0a3/eth/consensus/applier.py
+drwxr-xr-x   0 eve        (501) staff       (20)        0 2023-06-08 20:25:34.244690 py-evm-0.7.0a3/eth/consensus/clique/
+-rw-r--r--   0 eve        (501) staff       (20)      271 2023-06-02 21:07:53.000000 py-evm-0.7.0a3/eth/consensus/clique/__init__.py
+-rw-r--r--   0 eve        (501) staff       (20)     5208 2023-06-02 21:07:53.000000 py-evm-0.7.0a3/eth/consensus/clique/_utils.py
+-rw-r--r--   0 eve        (501) staff       (20)     5383 2023-06-02 21:07:53.000000 py-evm-0.7.0a3/eth/consensus/clique/clique.py
+-rw-r--r--   0 eve        (501) staff       (20)      486 2023-06-02 21:07:53.000000 py-evm-0.7.0a3/eth/consensus/clique/constants.py
+-rw-r--r--   0 eve        (501) staff       (20)     3368 2023-06-02 21:07:53.000000 py-evm-0.7.0a3/eth/consensus/clique/datatypes.py
+-rw-r--r--   0 eve        (501) staff       (20)     2949 2023-06-02 21:07:53.000000 py-evm-0.7.0a3/eth/consensus/clique/encoding.py
+-rw-r--r--   0 eve        (501) staff       (20)      158 2023-06-02 21:07:53.000000 py-evm-0.7.0a3/eth/consensus/clique/exceptions.py
+-rw-r--r--   0 eve        (501) staff       (20)    11157 2023-06-02 21:07:53.000000 py-evm-0.7.0a3/eth/consensus/clique/snapshot_manager.py
+-rw-r--r--   0 eve        (501) staff       (20)      187 2023-06-02 21:07:53.000000 py-evm-0.7.0a3/eth/consensus/context.py
+-rw-r--r--   0 eve        (501) staff       (20)      683 2023-06-02 21:07:53.000000 py-evm-0.7.0a3/eth/consensus/noproof.py
+-rw-r--r--   0 eve        (501) staff       (20)      819 2023-06-02 21:07:53.000000 py-evm-0.7.0a3/eth/consensus/pos.py
+-rw-r--r--   0 eve        (501) staff       (20)     4024 2023-06-02 21:07:53.000000 py-evm-0.7.0a3/eth/consensus/pow.py
+-rw-r--r--   0 eve        (501) staff       (20)     3921 2023-06-02 21:07:53.000000 py-evm-0.7.0a3/eth/constants.py
+drwxr-xr-x   0 eve        (501) staff       (20)        0 2023-06-08 20:25:34.246821 py-evm-0.7.0a3/eth/db/
+-rw-r--r--   0 eve        (501) staff       (20)      714 2023-06-08 20:21:10.000000 py-evm-0.7.0a3/eth/db/__init__.py
+-rw-r--r--   0 eve        (501) staff       (20)     3460 2023-06-02 21:07:53.000000 py-evm-0.7.0a3/eth/db/accesslog.py
+-rw-r--r--   0 eve        (501) staff       (20)    24411 2023-06-02 21:07:53.000000 py-evm-0.7.0a3/eth/db/account.py
+-rw-r--r--   0 eve        (501) staff       (20)     4277 2023-06-02 21:07:53.000000 py-evm-0.7.0a3/eth/db/atomic.py
+drwxr-xr-x   0 eve        (501) staff       (20)        0 2023-06-08 20:25:34.247220 py-evm-0.7.0a3/eth/db/backends/
+-rw-r--r--   0 eve        (501) staff       (20)        0 2021-02-22 21:36:31.000000 py-evm-0.7.0a3/eth/db/backends/__init__.py
+-rw-r--r--   0 eve        (501) staff       (20)     2513 2023-06-02 21:07:53.000000 py-evm-0.7.0a3/eth/db/backends/base.py
+-rw-r--r--   0 eve        (501) staff       (20)     4496 2023-06-02 21:07:53.000000 py-evm-0.7.0a3/eth/db/backends/level.py
+-rw-r--r--   0 eve        (501) staff       (20)      890 2021-02-22 21:36:31.000000 py-evm-0.7.0a3/eth/db/backends/memory.py
+-rw-r--r--   0 eve        (501) staff       (20)     2874 2023-06-02 21:07:53.000000 py-evm-0.7.0a3/eth/db/batch.py
+-rw-r--r--   0 eve        (501) staff       (20)      971 2023-06-02 21:07:53.000000 py-evm-0.7.0a3/eth/db/cache.py
+-rw-r--r--   0 eve        (501) staff       (20)    19206 2023-06-08 20:21:10.000000 py-evm-0.7.0a3/eth/db/chain.py
+-rw-r--r--   0 eve        (501) staff       (20)     5873 2023-06-02 21:07:53.000000 py-evm-0.7.0a3/eth/db/chain_gaps.py
+-rw-r--r--   0 eve        (501) staff       (20)     7394 2023-06-02 21:07:53.000000 py-evm-0.7.0a3/eth/db/diff.py
+-rw-r--r--   0 eve        (501) staff       (20)      506 2023-06-02 21:07:53.000000 py-evm-0.7.0a3/eth/db/hash_trie.py
+-rw-r--r--   0 eve        (501) staff       (20)    24129 2023-06-02 21:07:53.000000 py-evm-0.7.0a3/eth/db/header.py
+-rw-r--r--   0 eve        (501) staff       (20)    17008 2023-06-02 21:07:53.000000 py-evm-0.7.0a3/eth/db/journal.py
+-rw-r--r--   0 eve        (501) staff       (20)     1306 2023-06-02 21:07:53.000000 py-evm-0.7.0a3/eth/db/keymap.py
+-rw-r--r--   0 eve        (501) staff       (20)     1354 2023-06-02 21:07:53.000000 py-evm-0.7.0a3/eth/db/schema.py
+-rw-r--r--   0 eve        (501) staff       (20)    16562 2023-06-02 21:07:53.000000 py-evm-0.7.0a3/eth/db/slow_journal.py
+-rw-r--r--   0 eve        (501) staff       (20)    16442 2023-06-02 21:07:53.000000 py-evm-0.7.0a3/eth/db/storage.py
+-rw-r--r--   0 eve        (501) staff       (20)     1393 2023-06-02 21:07:53.000000 py-evm-0.7.0a3/eth/db/trie.py
+-rw-r--r--   0 eve        (501) staff       (20)     1660 2023-06-02 21:07:53.000000 py-evm-0.7.0a3/eth/db/witness.py
+drwxr-xr-x   0 eve        (501) staff       (20)        0 2023-06-08 20:25:34.247428 py-evm-0.7.0a3/eth/estimators/
+-rw-r--r--   0 eve        (501) staff       (20)      514 2023-06-02 21:07:53.000000 py-evm-0.7.0a3/eth/estimators/__init__.py
+-rw-r--r--   0 eve        (501) staff       (20)     3427 2023-06-02 21:07:53.000000 py-evm-0.7.0a3/eth/estimators/gas.py
+-rw-r--r--   0 eve        (501) staff       (20)     4115 2023-06-02 21:07:53.000000 py-evm-0.7.0a3/eth/exceptions.py
+drwxr-xr-x   0 eve        (501) staff       (20)        0 2023-06-08 20:25:34.248574 py-evm-0.7.0a3/eth/precompiles/
+-rw-r--r--   0 eve        (501) staff       (20)      398 2021-02-26 19:54:17.000000 py-evm-0.7.0a3/eth/precompiles/__init__.py
+-rw-r--r--   0 eve        (501) staff       (20)      962 2023-06-02 21:07:53.000000 py-evm-0.7.0a3/eth/precompiles/blake2.py
+-rw-r--r--   0 eve        (501) staff       (20)     1502 2023-06-02 21:07:53.000000 py-evm-0.7.0a3/eth/precompiles/ecadd.py
+-rw-r--r--   0 eve        (501) staff       (20)     1390 2023-06-02 21:07:53.000000 py-evm-0.7.0a3/eth/precompiles/ecmul.py
+-rw-r--r--   0 eve        (501) staff       (20)     3257 2023-06-02 21:07:53.000000 py-evm-0.7.0a3/eth/precompiles/ecpairing.py
+-rw-r--r--   0 eve        (501) staff       (20)     1512 2023-06-02 21:07:53.000000 py-evm-0.7.0a3/eth/precompiles/ecrecover.py
+-rw-r--r--   0 eve        (501) staff       (20)      472 2023-06-02 21:07:53.000000 py-evm-0.7.0a3/eth/precompiles/identity.py
+-rw-r--r--   0 eve        (501) staff       (20)     3934 2023-06-02 21:07:53.000000 py-evm-0.7.0a3/eth/precompiles/modexp.py
+-rw-r--r--   0 eve        (501) staff       (20)      670 2023-06-02 21:07:53.000000 py-evm-0.7.0a3/eth/precompiles/ripemd160.py
+-rw-r--r--   0 eve        (501) staff       (20)      541 2023-06-02 21:07:53.000000 py-evm-0.7.0a3/eth/precompiles/sha256.py
+-rw-r--r--   0 eve        (501) staff       (20)        0 2021-02-22 21:36:31.000000 py-evm-0.7.0a3/eth/py.typed
+drwxr-xr-x   0 eve        (501) staff       (20)        0 2023-06-08 20:25:34.249432 py-evm-0.7.0a3/eth/rlp/
+-rw-r--r--   0 eve        (501) staff       (20)        0 2021-02-22 21:36:31.000000 py-evm-0.7.0a3/eth/rlp/__init__.py
+-rw-r--r--   0 eve        (501) staff       (20)     1022 2023-06-02 21:07:53.000000 py-evm-0.7.0a3/eth/rlp/accounts.py
+-rw-r--r--   0 eve        (501) staff       (20)      904 2023-06-02 21:07:53.000000 py-evm-0.7.0a3/eth/rlp/blocks.py
+-rw-r--r--   0 eve        (501) staff       (20)     5417 2023-06-02 21:07:53.000000 py-evm-0.7.0a3/eth/rlp/headers.py
+-rw-r--r--   0 eve        (501) staff       (20)      603 2023-06-02 21:07:53.000000 py-evm-0.7.0a3/eth/rlp/logs.py
+-rw-r--r--   0 eve        (501) staff       (20)     1285 2023-06-02 21:07:53.000000 py-evm-0.7.0a3/eth/rlp/receipts.py
+-rw-r--r--   0 eve        (501) staff       (20)      387 2023-06-02 21:07:53.000000 py-evm-0.7.0a3/eth/rlp/sedes.py
+-rw-r--r--   0 eve        (501) staff       (20)     3611 2023-06-02 21:07:53.000000 py-evm-0.7.0a3/eth/rlp/transactions.py
+drwxr-xr-x   0 eve        (501) staff       (20)        0 2023-06-08 20:25:34.249735 py-evm-0.7.0a3/eth/tools/
+-rw-r--r--   0 eve        (501) staff       (20)        0 2021-02-22 21:36:31.000000 py-evm-0.7.0a3/eth/tools/__init__.py
+drwxr-xr-x   0 eve        (501) staff       (20)        0 2023-06-08 20:25:34.250875 py-evm-0.7.0a3/eth/tools/_utils/
+-rw-r--r--   0 eve        (501) staff       (20)        0 2021-02-22 21:36:31.000000 py-evm-0.7.0a3/eth/tools/_utils/__init__.py
+-rw-r--r--   0 eve        (501) staff       (20)      662 2023-06-08 20:21:10.000000 py-evm-0.7.0a3/eth/tools/_utils/deprecation.py
+-rw-r--r--   0 eve        (501) staff       (20)      190 2023-06-02 21:07:53.000000 py-evm-0.7.0a3/eth/tools/_utils/git.py
+-rw-r--r--   0 eve        (501) staff       (20)      556 2023-06-02 21:07:53.000000 py-evm-0.7.0a3/eth/tools/_utils/hashing.py
+-rw-r--r--   0 eve        (501) staff       (20)     1564 2023-06-02 21:07:53.000000 py-evm-0.7.0a3/eth/tools/_utils/mappings.py
+-rw-r--r--   0 eve        (501) staff       (20)    18084 2023-06-02 21:07:53.000000 py-evm-0.7.0a3/eth/tools/_utils/normalization.py
+-rw-r--r--   0 eve        (501) staff       (20)     4410 2023-06-02 21:07:53.000000 py-evm-0.7.0a3/eth/tools/_utils/slow_code_stream.py
+-rw-r--r--   0 eve        (501) staff       (20)      903 2023-06-02 21:07:53.000000 py-evm-0.7.0a3/eth/tools/_utils/vyper.py
+drwxr-xr-x   0 eve        (501) staff       (20)        0 2023-06-08 20:25:34.250983 py-evm-0.7.0a3/eth/tools/builder/
+-rw-r--r--   0 eve        (501) staff       (20)        0 2021-02-22 21:36:31.000000 py-evm-0.7.0a3/eth/tools/builder/__init__.py
+drwxr-xr-x   0 eve        (501) staff       (20)        0 2023-06-08 20:25:34.251175 py-evm-0.7.0a3/eth/tools/builder/chain/
+-rw-r--r--   0 eve        (501) staff       (20)     2936 2023-04-28 21:07:47.000000 py-evm-0.7.0a3/eth/tools/builder/chain/__init__.py
+-rw-r--r--   0 eve        (501) staff       (20)    15254 2023-06-02 21:07:53.000000 py-evm-0.7.0a3/eth/tools/builder/chain/builders.py
+drwxr-xr-x   0 eve        (501) staff       (20)        0 2023-06-08 20:25:34.251502 py-evm-0.7.0a3/eth/tools/db/
+-rw-r--r--   0 eve        (501) staff       (20)        0 2021-02-22 21:36:31.000000 py-evm-0.7.0a3/eth/tools/db/__init__.py
+-rw-r--r--   0 eve        (501) staff       (20)     5191 2023-06-08 20:21:10.000000 py-evm-0.7.0a3/eth/tools/db/atomic.py
+-rw-r--r--   0 eve        (501) staff       (20)     2269 2023-06-02 21:07:53.000000 py-evm-0.7.0a3/eth/tools/db/base.py
+drwxr-xr-x   0 eve        (501) staff       (20)        0 2023-06-08 20:25:34.252087 py-evm-0.7.0a3/eth/tools/fixtures/
+-rw-r--r--   0 eve        (501) staff       (20)      615 2021-08-19 20:42:01.000000 py-evm-0.7.0a3/eth/tools/fixtures/__init__.py
+-rw-r--r--   0 eve        (501) staff       (20)      887 2023-06-02 21:07:53.000000 py-evm-0.7.0a3/eth/tools/fixtures/_utils.py
+drwxr-xr-x   0 eve        (501) staff       (20)        0 2023-06-08 20:25:34.252838 py-evm-0.7.0a3/eth/tools/fixtures/fillers/
+-rw-r--r--   0 eve        (501) staff       (20)      282 2021-02-22 21:36:31.000000 py-evm-0.7.0a3/eth/tools/fixtures/fillers/__init__.py
+-rw-r--r--   0 eve        (501) staff       (20)     2456 2023-06-02 21:07:53.000000 py-evm-0.7.0a3/eth/tools/fixtures/fillers/_utils.py
+-rw-r--r--   0 eve        (501) staff       (20)    12716 2023-06-08 20:21:10.000000 py-evm-0.7.0a3/eth/tools/fixtures/fillers/common.py
+-rw-r--r--   0 eve        (501) staff       (20)     3461 2023-06-02 21:07:53.000000 py-evm-0.7.0a3/eth/tools/fixtures/fillers/formatters.py
+-rw-r--r--   0 eve        (501) staff       (20)     1307 2023-06-02 21:07:53.000000 py-evm-0.7.0a3/eth/tools/fixtures/fillers/main.py
+-rw-r--r--   0 eve        (501) staff       (20)     2758 2023-06-02 21:07:53.000000 py-evm-0.7.0a3/eth/tools/fixtures/fillers/state.py
+-rw-r--r--   0 eve        (501) staff       (20)     1737 2023-06-02 21:07:53.000000 py-evm-0.7.0a3/eth/tools/fixtures/fillers/vm.py
+-rw-r--r--   0 eve        (501) staff       (20)     2079 2023-06-02 21:07:53.000000 py-evm-0.7.0a3/eth/tools/fixtures/generation.py
+-rw-r--r--   0 eve        (501) staff       (20)     9361 2023-06-02 21:07:53.000000 py-evm-0.7.0a3/eth/tools/fixtures/helpers.py
+-rw-r--r--   0 eve        (501) staff       (20)     3068 2023-06-02 21:07:53.000000 py-evm-0.7.0a3/eth/tools/fixtures/loading.py
+-rw-r--r--   0 eve        (501) staff       (20)      791 2023-06-02 21:07:53.000000 py-evm-0.7.0a3/eth/tools/mining.py
+-rw-r--r--   0 eve        (501) staff       (20)      476 2023-06-02 21:07:53.000000 py-evm-0.7.0a3/eth/tools/rlp.py
+-rw-r--r--   0 eve        (501) staff       (20)     2693 2023-06-02 21:07:53.000000 py-evm-0.7.0a3/eth/typing.py
+-rw-r--r--   0 eve        (501) staff       (20)     8548 2023-06-02 21:07:53.000000 py-evm-0.7.0a3/eth/validation.py
+drwxr-xr-x   0 eve        (501) staff       (20)        0 2023-06-08 20:25:34.254784 py-evm-0.7.0a3/eth/vm/
+-rw-r--r--   0 eve        (501) staff       (20)        0 2021-02-22 21:36:31.000000 py-evm-0.7.0a3/eth/vm/__init__.py
+-rw-r--r--   0 eve        (501) staff       (20)    26238 2023-06-02 21:07:53.000000 py-evm-0.7.0a3/eth/vm/base.py
+-rw-r--r--   0 eve        (501) staff       (20)      632 2023-06-02 21:07:53.000000 py-evm-0.7.0a3/eth/vm/chain_context.py
+-rw-r--r--   0 eve        (501) staff       (20)     4438 2023-06-08 20:21:10.000000 py-evm-0.7.0a3/eth/vm/code_stream.py
+-rw-r--r--   0 eve        (501) staff       (20)    19222 2023-06-02 21:07:53.000000 py-evm-0.7.0a3/eth/vm/computation.py
+-rw-r--r--   0 eve        (501) staff       (20)     2124 2023-06-02 21:07:53.000000 py-evm-0.7.0a3/eth/vm/execution_context.py
+drwxr-xr-x   0 eve        (501) staff       (20)        0 2023-06-08 20:25:34.254878 py-evm-0.7.0a3/eth/vm/forks/
+-rw-r--r--   0 eve        (501) staff       (20)      899 2023-04-28 21:07:47.000000 py-evm-0.7.0a3/eth/vm/forks/__init__.py
+drwxr-xr-x   0 eve        (501) staff       (20)        0 2023-06-08 20:25:34.255545 py-evm-0.7.0a3/eth/vm/forks/arrow_glacier/
+-rw-r--r--   0 eve        (501) staff       (20)      856 2023-06-02 21:07:53.000000 py-evm-0.7.0a3/eth/vm/forks/arrow_glacier/__init__.py
+-rw-r--r--   0 eve        (501) staff       (20)      993 2023-06-02 21:07:53.000000 py-evm-0.7.0a3/eth/vm/forks/arrow_glacier/blocks.py
+-rw-r--r--   0 eve        (501) staff       (20)      287 2023-06-02 21:07:53.000000 py-evm-0.7.0a3/eth/vm/forks/arrow_glacier/computation.py
+-rw-r--r--   0 eve        (501) staff       (20)     1084 2023-06-02 21:07:53.000000 py-evm-0.7.0a3/eth/vm/forks/arrow_glacier/headers.py
+-rw-r--r--   0 eve        (501) staff       (20)      523 2023-06-02 21:07:53.000000 py-evm-0.7.0a3/eth/vm/forks/arrow_glacier/state.py
+-rw-r--r--   0 eve        (501) staff       (20)     1134 2023-06-02 21:07:53.000000 py-evm-0.7.0a3/eth/vm/forks/arrow_glacier/transactions.py
+drwxr-xr-x   0 eve        (501) staff       (20)        0 2023-06-08 20:25:34.256618 py-evm-0.7.0a3/eth/vm/forks/berlin/
+-rw-r--r--   0 eve        (501) staff       (20)      772 2023-06-02 21:07:53.000000 py-evm-0.7.0a3/eth/vm/forks/berlin/__init__.py
+-rw-r--r--   0 eve        (501) staff       (20)      784 2023-06-02 21:07:53.000000 py-evm-0.7.0a3/eth/vm/forks/berlin/blocks.py
+-rw-r--r--   0 eve        (501) staff       (20)     2441 2023-06-02 21:07:53.000000 py-evm-0.7.0a3/eth/vm/forks/berlin/computation.py
+-rw-r--r--   0 eve        (501) staff       (20)      327 2021-08-30 21:22:29.000000 py-evm-0.7.0a3/eth/vm/forks/berlin/constants.py
+-rw-r--r--   0 eve        (501) staff       (20)      374 2023-06-02 21:07:53.000000 py-evm-0.7.0a3/eth/vm/forks/berlin/headers.py
+-rw-r--r--   0 eve        (501) staff       (20)     6417 2023-06-02 21:07:53.000000 py-evm-0.7.0a3/eth/vm/forks/berlin/logic.py
+-rw-r--r--   0 eve        (501) staff       (20)     2922 2023-06-02 21:07:53.000000 py-evm-0.7.0a3/eth/vm/forks/berlin/opcodes.py
+-rw-r--r--   0 eve        (501) staff       (20)     4606 2023-06-02 21:07:53.000000 py-evm-0.7.0a3/eth/vm/forks/berlin/receipts.py
+-rw-r--r--   0 eve        (501) staff       (20)     1187 2023-06-02 21:07:53.000000 py-evm-0.7.0a3/eth/vm/forks/berlin/state.py
+-rw-r--r--   0 eve        (501) staff       (20)    15395 2023-06-02 21:07:53.000000 py-evm-0.7.0a3/eth/vm/forks/berlin/transactions.py
+drwxr-xr-x   0 eve        (501) staff       (20)        0 2023-06-08 20:25:34.257581 py-evm-0.7.0a3/eth/vm/forks/byzantium/
+-rw-r--r--   0 eve        (501) staff       (20)     3584 2023-06-02 21:07:53.000000 py-evm-0.7.0a3/eth/vm/forks/byzantium/__init__.py
+-rw-r--r--   0 eve        (501) staff       (20)      485 2023-06-02 21:07:53.000000 py-evm-0.7.0a3/eth/vm/forks/byzantium/blocks.py
+-rw-r--r--   0 eve        (501) staff       (20)     1016 2023-06-02 21:07:53.000000 py-evm-0.7.0a3/eth/vm/forks/byzantium/computation.py
+-rw-r--r--   0 eve        (501) staff       (20)      235 2023-06-02 21:07:53.000000 py-evm-0.7.0a3/eth/vm/forks/byzantium/constants.py
+-rw-r--r--   0 eve        (501) staff       (20)     3368 2023-06-02 21:07:53.000000 py-evm-0.7.0a3/eth/vm/forks/byzantium/headers.py
+-rw-r--r--   0 eve        (501) staff       (20)     3526 2023-06-02 21:07:53.000000 py-evm-0.7.0a3/eth/vm/forks/byzantium/opcodes.py
+-rw-r--r--   0 eve        (501) staff       (20)      222 2023-06-02 21:07:53.000000 py-evm-0.7.0a3/eth/vm/forks/byzantium/state.py
+-rw-r--r--   0 eve        (501) staff       (20)     1231 2023-06-02 21:07:53.000000 py-evm-0.7.0a3/eth/vm/forks/byzantium/transactions.py
+drwxr-xr-x   0 eve        (501) staff       (20)        0 2023-06-08 20:25:34.258580 py-evm-0.7.0a3/eth/vm/forks/constantinople/
+-rw-r--r--   0 eve        (501) staff       (20)     1106 2023-06-02 21:07:53.000000 py-evm-0.7.0a3/eth/vm/forks/constantinople/__init__.py
+-rw-r--r--   0 eve        (501) staff       (20)      484 2023-06-02 21:07:53.000000 py-evm-0.7.0a3/eth/vm/forks/constantinople/blocks.py
+-rw-r--r--   0 eve        (501) staff       (20)      757 2023-06-02 21:07:53.000000 py-evm-0.7.0a3/eth/vm/forks/constantinople/computation.py
+-rw-r--r--   0 eve        (501) staff       (20)      329 2023-06-02 21:07:53.000000 py-evm-0.7.0a3/eth/vm/forks/constantinople/constants.py
+-rw-r--r--   0 eve        (501) staff       (20)      406 2023-06-02 21:07:53.000000 py-evm-0.7.0a3/eth/vm/forks/constantinople/headers.py
+-rw-r--r--   0 eve        (501) staff       (20)     1574 2023-06-02 21:07:53.000000 py-evm-0.7.0a3/eth/vm/forks/constantinople/opcodes.py
+-rw-r--r--   0 eve        (501) staff       (20)      221 2023-06-02 21:07:53.000000 py-evm-0.7.0a3/eth/vm/forks/constantinople/state.py
+-rw-r--r--   0 eve        (501) staff       (20)      334 2023-06-02 21:07:53.000000 py-evm-0.7.0a3/eth/vm/forks/constantinople/storage.py
+-rw-r--r--   0 eve        (501) staff       (20)     1235 2023-06-02 21:07:53.000000 py-evm-0.7.0a3/eth/vm/forks/constantinople/transactions.py
+drwxr-xr-x   0 eve        (501) staff       (20)        0 2023-06-08 20:25:34.259676 py-evm-0.7.0a3/eth/vm/forks/frontier/
+-rw-r--r--   0 eve        (501) staff       (20)     3732 2023-06-02 21:07:53.000000 py-evm-0.7.0a3/eth/vm/forks/frontier/__init__.py
+-rw-r--r--   0 eve        (501) staff       (20)     3412 2023-06-02 21:07:53.000000 py-evm-0.7.0a3/eth/vm/forks/frontier/blocks.py
+-rw-r--r--   0 eve        (501) staff       (20)     3715 2023-06-02 21:07:53.000000 py-evm-0.7.0a3/eth/vm/forks/frontier/computation.py
+-rw-r--r--   0 eve        (501) staff       (20)       96 2021-09-20 20:47:49.000000 py-evm-0.7.0a3/eth/vm/forks/frontier/constants.py
+-rw-r--r--   0 eve        (501) staff       (20)     3529 2023-06-02 21:07:53.000000 py-evm-0.7.0a3/eth/vm/forks/frontier/headers.py
+-rw-r--r--   0 eve        (501) staff       (20)    20228 2023-06-02 21:07:53.000000 py-evm-0.7.0a3/eth/vm/forks/frontier/opcodes.py
+-rw-r--r--   0 eve        (501) staff       (20)     7686 2023-06-02 21:07:53.000000 py-evm-0.7.0a3/eth/vm/forks/frontier/state.py
+-rw-r--r--   0 eve        (501) staff       (20)      140 2023-06-02 21:07:53.000000 py-evm-0.7.0a3/eth/vm/forks/frontier/transaction_context.py
+-rw-r--r--   0 eve        (501) staff       (20)     5868 2023-06-02 21:07:53.000000 py-evm-0.7.0a3/eth/vm/forks/frontier/transactions.py
+-rw-r--r--   0 eve        (501) staff       (20)     1603 2023-06-02 21:07:53.000000 py-evm-0.7.0a3/eth/vm/forks/frontier/validation.py
+drwxr-xr-x   0 eve        (501) staff       (20)        0 2023-06-08 20:25:34.260335 py-evm-0.7.0a3/eth/vm/forks/gray_glacier/
+-rw-r--r--   0 eve        (501) staff       (20)      855 2023-06-02 21:07:53.000000 py-evm-0.7.0a3/eth/vm/forks/gray_glacier/__init__.py
+-rw-r--r--   0 eve        (501) staff       (20)     1068 2023-06-02 21:07:53.000000 py-evm-0.7.0a3/eth/vm/forks/gray_glacier/blocks.py
+-rw-r--r--   0 eve        (501) staff       (20)      317 2023-06-02 21:07:53.000000 py-evm-0.7.0a3/eth/vm/forks/gray_glacier/computation.py
+-rw-r--r--   0 eve        (501) staff       (20)     1119 2023-06-02 21:07:53.000000 py-evm-0.7.0a3/eth/vm/forks/gray_glacier/headers.py
+-rw-r--r--   0 eve        (501) staff       (20)      556 2023-06-02 21:07:53.000000 py-evm-0.7.0a3/eth/vm/forks/gray_glacier/state.py
+-rw-r--r--   0 eve        (501) staff       (20)     1170 2023-06-02 21:07:53.000000 py-evm-0.7.0a3/eth/vm/forks/gray_glacier/transactions.py
+drwxr-xr-x   0 eve        (501) staff       (20)        0 2023-06-08 20:25:34.261524 py-evm-0.7.0a3/eth/vm/forks/homestead/
+-rw-r--r--   0 eve        (501) staff       (20)     1250 2023-06-02 21:07:53.000000 py-evm-0.7.0a3/eth/vm/forks/homestead/__init__.py
+-rw-r--r--   0 eve        (501) staff       (20)      466 2023-06-02 21:07:53.000000 py-evm-0.7.0a3/eth/vm/forks/homestead/blocks.py
+-rw-r--r--   0 eve        (501) staff       (20)     2289 2023-06-02 21:07:53.000000 py-evm-0.7.0a3/eth/vm/forks/homestead/computation.py
+-rw-r--r--   0 eve        (501) staff       (20)       61 2021-09-03 20:35:50.000000 py-evm-0.7.0a3/eth/vm/forks/homestead/constants.py
+-rw-r--r--   0 eve        (501) staff       (20)     9656 2023-06-02 21:07:53.000000 py-evm-0.7.0a3/eth/vm/forks/homestead/headers.py
+-rw-r--r--   0 eve        (501) staff       (20)      637 2023-06-02 21:07:53.000000 py-evm-0.7.0a3/eth/vm/forks/homestead/opcodes.py
+-rw-r--r--   0 eve        (501) staff       (20)      640 2023-06-02 21:07:53.000000 py-evm-0.7.0a3/eth/vm/forks/homestead/state.py
+-rw-r--r--   0 eve        (501) staff       (20)     2197 2023-06-02 21:07:53.000000 py-evm-0.7.0a3/eth/vm/forks/homestead/transactions.py
+-rw-r--r--   0 eve        (501) staff       (20)      518 2023-06-02 21:07:53.000000 py-evm-0.7.0a3/eth/vm/forks/homestead/validation.py
+drwxr-xr-x   0 eve        (501) staff       (20)        0 2023-06-08 20:25:34.262617 py-evm-0.7.0a3/eth/vm/forks/istanbul/
+-rw-r--r--   0 eve        (501) staff       (20)      817 2023-06-02 21:07:53.000000 py-evm-0.7.0a3/eth/vm/forks/istanbul/__init__.py
+-rw-r--r--   0 eve        (501) staff       (20)      469 2023-06-02 21:07:53.000000 py-evm-0.7.0a3/eth/vm/forks/istanbul/blocks.py
+-rw-r--r--   0 eve        (501) staff       (20)     1421 2023-06-02 21:07:53.000000 py-evm-0.7.0a3/eth/vm/forks/istanbul/computation.py
+-rw-r--r--   0 eve        (501) staff       (20)      316 2021-02-22 21:36:31.000000 py-evm-0.7.0a3/eth/vm/forks/istanbul/constants.py
+-rw-r--r--   0 eve        (501) staff       (20)      384 2023-06-02 21:07:53.000000 py-evm-0.7.0a3/eth/vm/forks/istanbul/headers.py
+-rw-r--r--   0 eve        (501) staff       (20)     1664 2023-06-02 21:07:53.000000 py-evm-0.7.0a3/eth/vm/forks/istanbul/opcodes.py
+-rw-r--r--   0 eve        (501) staff       (20)      206 2023-06-02 21:07:53.000000 py-evm-0.7.0a3/eth/vm/forks/istanbul/state.py
+-rw-r--r--   0 eve        (501) staff       (20)      909 2023-06-02 21:07:53.000000 py-evm-0.7.0a3/eth/vm/forks/istanbul/storage.py
+-rw-r--r--   0 eve        (501) staff       (20)     1798 2023-06-02 21:07:53.000000 py-evm-0.7.0a3/eth/vm/forks/istanbul/transactions.py
+drwxr-xr-x   0 eve        (501) staff       (20)        0 2023-06-08 20:25:34.263788 py-evm-0.7.0a3/eth/vm/forks/london/
+-rw-r--r--   0 eve        (501) staff       (20)     2260 2023-06-02 21:07:53.000000 py-evm-0.7.0a3/eth/vm/forks/london/__init__.py
+-rw-r--r--   0 eve        (501) staff       (20)     5828 2023-06-02 21:07:53.000000 py-evm-0.7.0a3/eth/vm/forks/london/blocks.py
+-rw-r--r--   0 eve        (501) staff       (20)      810 2023-06-02 21:07:53.000000 py-evm-0.7.0a3/eth/vm/forks/london/computation.py
+-rw-r--r--   0 eve        (501) staff       (20)      470 2023-06-02 21:07:53.000000 py-evm-0.7.0a3/eth/vm/forks/london/constants.py
+-rw-r--r--   0 eve        (501) staff       (20)     5618 2023-06-02 21:07:53.000000 py-evm-0.7.0a3/eth/vm/forks/london/headers.py
+-rw-r--r--   0 eve        (501) staff       (20)      895 2023-06-02 21:07:53.000000 py-evm-0.7.0a3/eth/vm/forks/london/opcodes.py
+-rw-r--r--   0 eve        (501) staff       (20)      629 2023-06-02 21:07:53.000000 py-evm-0.7.0a3/eth/vm/forks/london/receipts.py
+-rw-r--r--   0 eve        (501) staff       (20)     4881 2023-06-02 21:07:53.000000 py-evm-0.7.0a3/eth/vm/forks/london/state.py
+-rw-r--r--   0 eve        (501) staff       (20)      544 2023-06-02 21:07:53.000000 py-evm-0.7.0a3/eth/vm/forks/london/storage.py
+-rw-r--r--   0 eve        (501) staff       (20)     9486 2023-06-02 21:07:53.000000 py-evm-0.7.0a3/eth/vm/forks/london/transactions.py
+-rw-r--r--   0 eve        (501) staff       (20)      855 2023-06-02 21:07:53.000000 py-evm-0.7.0a3/eth/vm/forks/london/validation.py
+drwxr-xr-x   0 eve        (501) staff       (20)        0 2023-06-08 20:25:34.264476 py-evm-0.7.0a3/eth/vm/forks/muir_glacier/
+-rw-r--r--   0 eve        (501) staff       (20)      842 2023-06-02 21:07:53.000000 py-evm-0.7.0a3/eth/vm/forks/muir_glacier/__init__.py
+-rw-r--r--   0 eve        (501) staff       (20)      472 2023-06-02 21:07:53.000000 py-evm-0.7.0a3/eth/vm/forks/muir_glacier/blocks.py
+-rw-r--r--   0 eve        (501) staff       (20)      537 2023-06-02 21:07:53.000000 py-evm-0.7.0a3/eth/vm/forks/muir_glacier/computation.py
+-rw-r--r--   0 eve        (501) staff       (20)      443 2023-06-02 21:07:53.000000 py-evm-0.7.0a3/eth/vm/forks/muir_glacier/headers.py
+-rw-r--r--   0 eve        (501) staff       (20)      137 2023-06-02 21:07:53.000000 py-evm-0.7.0a3/eth/vm/forks/muir_glacier/opcodes.py
+-rw-r--r--   0 eve        (501) staff       (20)      209 2023-06-02 21:07:53.000000 py-evm-0.7.0a3/eth/vm/forks/muir_glacier/state.py
+-rw-r--r--   0 eve        (501) staff       (20)     1212 2023-06-02 21:07:53.000000 py-evm-0.7.0a3/eth/vm/forks/muir_glacier/transactions.py
+drwxr-xr-x   0 eve        (501) staff       (20)        0 2023-06-08 20:25:34.265183 py-evm-0.7.0a3/eth/vm/forks/paris/
+-rw-r--r--   0 eve        (501) staff       (20)     2117 2023-06-02 21:07:53.000000 py-evm-0.7.0a3/eth/vm/forks/paris/__init__.py
+-rw-r--r--   0 eve        (501) staff       (20)     1039 2023-06-02 21:07:53.000000 py-evm-0.7.0a3/eth/vm/forks/paris/blocks.py
+-rw-r--r--   0 eve        (501) staff       (20)      379 2023-06-02 21:07:53.000000 py-evm-0.7.0a3/eth/vm/forks/paris/computation.py
+-rw-r--r--   0 eve        (501) staff       (20)     2284 2023-06-02 21:07:53.000000 py-evm-0.7.0a3/eth/vm/forks/paris/headers.py
+-rw-r--r--   0 eve        (501) staff       (20)      686 2023-06-02 21:07:53.000000 py-evm-0.7.0a3/eth/vm/forks/paris/opcodes.py
+-rw-r--r--   0 eve        (501) staff       (20)      666 2023-06-02 21:07:53.000000 py-evm-0.7.0a3/eth/vm/forks/paris/state.py
+-rw-r--r--   0 eve        (501) staff       (20)     1121 2023-06-02 21:07:53.000000 py-evm-0.7.0a3/eth/vm/forks/paris/transactions.py
+drwxr-xr-x   0 eve        (501) staff       (20)        0 2023-06-08 20:25:34.265991 py-evm-0.7.0a3/eth/vm/forks/petersburg/
+-rw-r--r--   0 eve        (501) staff       (20)     1036 2023-06-02 21:07:53.000000 py-evm-0.7.0a3/eth/vm/forks/petersburg/__init__.py
+-rw-r--r--   0 eve        (501) staff       (20)      472 2023-06-02 21:07:53.000000 py-evm-0.7.0a3/eth/vm/forks/petersburg/blocks.py
+-rw-r--r--   0 eve        (501) staff       (20)      531 2023-06-02 21:07:53.000000 py-evm-0.7.0a3/eth/vm/forks/petersburg/computation.py
+-rw-r--r--   0 eve        (501) staff       (20)      110 2023-06-02 21:07:53.000000 py-evm-0.7.0a3/eth/vm/forks/petersburg/constants.py
+-rw-r--r--   0 eve        (501) staff       (20)      386 2023-06-02 21:07:53.000000 py-evm-0.7.0a3/eth/vm/forks/petersburg/headers.py
+-rw-r--r--   0 eve        (501) staff       (20)     1399 2023-06-02 21:07:53.000000 py-evm-0.7.0a3/eth/vm/forks/petersburg/opcodes.py
+-rw-r--r--   0 eve        (501) staff       (20)      209 2023-06-02 21:07:53.000000 py-evm-0.7.0a3/eth/vm/forks/petersburg/state.py
+-rw-r--r--   0 eve        (501) staff       (20)     1211 2023-06-02 21:07:53.000000 py-evm-0.7.0a3/eth/vm/forks/petersburg/transactions.py
+drwxr-xr-x   0 eve        (501) staff       (20)        0 2023-06-08 20:25:34.267033 py-evm-0.7.0a3/eth/vm/forks/shanghai/
+-rw-r--r--   0 eve        (501) staff       (20)      667 2023-06-02 21:07:53.000000 py-evm-0.7.0a3/eth/vm/forks/shanghai/__init__.py
+-rw-r--r--   0 eve        (501) staff       (20)     9048 2023-06-02 21:07:53.000000 py-evm-0.7.0a3/eth/vm/forks/shanghai/blocks.py
+-rw-r--r--   0 eve        (501) staff       (20)     1655 2023-06-02 21:07:53.000000 py-evm-0.7.0a3/eth/vm/forks/shanghai/computation.py
+-rw-r--r--   0 eve        (501) staff       (20)      196 2023-06-02 21:07:53.000000 py-evm-0.7.0a3/eth/vm/forks/shanghai/constants.py
+-rw-r--r--   0 eve        (501) staff       (20)      824 2023-06-02 21:07:53.000000 py-evm-0.7.0a3/eth/vm/forks/shanghai/headers.py
+-rw-r--r--   0 eve        (501) staff       (20)      821 2023-06-02 21:07:53.000000 py-evm-0.7.0a3/eth/vm/forks/shanghai/logic.py
+-rw-r--r--   0 eve        (501) staff       (20)     1531 2023-06-02 21:07:53.000000 py-evm-0.7.0a3/eth/vm/forks/shanghai/opcodes.py
+-rw-r--r--   0 eve        (501) staff       (20)      751 2023-06-02 21:07:53.000000 py-evm-0.7.0a3/eth/vm/forks/shanghai/state.py
+-rw-r--r--   0 eve        (501) staff       (20)     1099 2023-06-02 21:07:53.000000 py-evm-0.7.0a3/eth/vm/forks/shanghai/transactions.py
+-rw-r--r--   0 eve        (501) staff       (20)     1515 2023-06-02 21:07:53.000000 py-evm-0.7.0a3/eth/vm/forks/shanghai/withdrawals.py
+drwxr-xr-x   0 eve        (501) staff       (20)        0 2023-06-08 20:25:34.267886 py-evm-0.7.0a3/eth/vm/forks/spurious_dragon/
+-rw-r--r--   0 eve        (501) staff       (20)      429 2023-06-02 21:07:53.000000 py-evm-0.7.0a3/eth/vm/forks/spurious_dragon/__init__.py
+-rw-r--r--   0 eve        (501) staff       (20)     2145 2023-06-02 21:07:53.000000 py-evm-0.7.0a3/eth/vm/forks/spurious_dragon/_utils.py
+-rw-r--r--   0 eve        (501) staff       (20)      484 2023-06-02 21:07:53.000000 py-evm-0.7.0a3/eth/vm/forks/spurious_dragon/blocks.py
+-rw-r--r--   0 eve        (501) staff       (20)     3322 2023-06-02 21:07:53.000000 py-evm-0.7.0a3/eth/vm/forks/spurious_dragon/computation.py
+-rw-r--r--   0 eve        (501) staff       (20)      169 2023-04-28 21:07:47.000000 py-evm-0.7.0a3/eth/vm/forks/spurious_dragon/constants.py
+-rw-r--r--   0 eve        (501) staff       (20)     1221 2023-06-02 21:07:53.000000 py-evm-0.7.0a3/eth/vm/forks/spurious_dragon/opcodes.py
+-rw-r--r--   0 eve        (501) staff       (20)     1465 2023-06-02 21:07:53.000000 py-evm-0.7.0a3/eth/vm/forks/spurious_dragon/state.py
+-rw-r--r--   0 eve        (501) staff       (20)     2866 2023-06-02 21:07:53.000000 py-evm-0.7.0a3/eth/vm/forks/spurious_dragon/transactions.py
+drwxr-xr-x   0 eve        (501) staff       (20)        0 2023-06-08 20:25:34.268364 py-evm-0.7.0a3/eth/vm/forks/tangerine_whistle/
+-rw-r--r--   0 eve        (501) staff       (20)      469 2023-06-02 21:07:53.000000 py-evm-0.7.0a3/eth/vm/forks/tangerine_whistle/__init__.py
+-rw-r--r--   0 eve        (501) staff       (20)      428 2023-06-02 21:07:53.000000 py-evm-0.7.0a3/eth/vm/forks/tangerine_whistle/computation.py
+-rw-r--r--   0 eve        (501) staff       (20)      225 2021-02-22 21:36:31.000000 py-evm-0.7.0a3/eth/vm/forks/tangerine_whistle/constants.py
+-rw-r--r--   0 eve        (501) staff       (20)     2106 2023-06-02 21:07:53.000000 py-evm-0.7.0a3/eth/vm/forks/tangerine_whistle/opcodes.py
+-rw-r--r--   0 eve        (501) staff       (20)      227 2023-06-02 21:07:53.000000 py-evm-0.7.0a3/eth/vm/forks/tangerine_whistle/state.py
+-rw-r--r--   0 eve        (501) staff       (20)     2626 2023-06-02 21:07:53.000000 py-evm-0.7.0a3/eth/vm/gas_meter.py
+-rw-r--r--   0 eve        (501) staff       (20)      540 2023-06-02 21:07:53.000000 py-evm-0.7.0a3/eth/vm/header.py
+-rw-r--r--   0 eve        (501) staff       (20)     3425 2023-06-02 21:07:53.000000 py-evm-0.7.0a3/eth/vm/interrupt.py
+drwxr-xr-x   0 eve        (501) staff       (20)        0 2023-06-08 20:25:34.270147 py-evm-0.7.0a3/eth/vm/logic/
+-rw-r--r--   0 eve        (501) staff       (20)        0 2021-02-22 21:36:31.000000 py-evm-0.7.0a3/eth/vm/logic/__init__.py
+-rw-r--r--   0 eve        (501) staff       (20)     4805 2023-06-02 21:07:53.000000 py-evm-0.7.0a3/eth/vm/logic/arithmetic.py
+-rw-r--r--   0 eve        (501) staff       (20)     1113 2023-06-02 21:07:53.000000 py-evm-0.7.0a3/eth/vm/logic/block.py
+-rw-r--r--   0 eve        (501) staff       (20)    13394 2023-06-02 21:07:53.000000 py-evm-0.7.0a3/eth/vm/logic/call.py
+-rw-r--r--   0 eve        (501) staff       (20)     2824 2023-06-02 21:07:53.000000 py-evm-0.7.0a3/eth/vm/logic/comparison.py
+-rw-r--r--   0 eve        (501) staff       (20)     6418 2023-06-02 21:07:53.000000 py-evm-0.7.0a3/eth/vm/logic/context.py
+-rw-r--r--   0 eve        (501) staff       (20)      944 2023-06-02 21:07:53.000000 py-evm-0.7.0a3/eth/vm/logic/duplication.py
+-rw-r--r--   0 eve        (501) staff       (20)     1508 2023-06-02 21:07:53.000000 py-evm-0.7.0a3/eth/vm/logic/flow.py
+-rw-r--r--   0 eve        (501) staff       (20)      507 2023-06-02 21:07:53.000000 py-evm-0.7.0a3/eth/vm/logic/invalid.py
+-rw-r--r--   0 eve        (501) staff       (20)     1355 2023-06-02 21:07:53.000000 py-evm-0.7.0a3/eth/vm/logic/logging.py
+-rw-r--r--   0 eve        (501) staff       (20)     1102 2023-06-02 21:07:53.000000 py-evm-0.7.0a3/eth/vm/logic/memory.py
+-rw-r--r--   0 eve        (501) staff       (20)      640 2023-06-02 21:07:53.000000 py-evm-0.7.0a3/eth/vm/logic/sha3.py
+-rw-r--r--   0 eve        (501) staff       (20)     2176 2023-06-02 21:07:53.000000 py-evm-0.7.0a3/eth/vm/logic/stack.py
+-rw-r--r--   0 eve        (501) staff       (20)     3939 2023-06-02 21:07:53.000000 py-evm-0.7.0a3/eth/vm/logic/storage.py
+-rw-r--r--   0 eve        (501) staff       (20)      974 2023-06-02 21:07:53.000000 py-evm-0.7.0a3/eth/vm/logic/swap.py
+-rw-r--r--   0 eve        (501) staff       (20)     9727 2023-06-02 21:07:53.000000 py-evm-0.7.0a3/eth/vm/logic/system.py
+-rw-r--r--   0 eve        (501) staff       (20)     2134 2023-06-02 21:07:53.000000 py-evm-0.7.0a3/eth/vm/memory.py
+-rw-r--r--   0 eve        (501) staff       (20)     3214 2023-06-02 21:07:53.000000 py-evm-0.7.0a3/eth/vm/message.py
+-rw-r--r--   0 eve        (501) staff       (20)     2785 2023-06-02 21:07:53.000000 py-evm-0.7.0a3/eth/vm/mnemonics.py
+-rw-r--r--   0 eve        (501) staff       (20)     1864 2023-06-02 21:07:53.000000 py-evm-0.7.0a3/eth/vm/opcode.py
+-rw-r--r--   0 eve        (501) staff       (20)     2432 2023-06-02 21:07:53.000000 py-evm-0.7.0a3/eth/vm/opcode_values.py
+-rw-r--r--   0 eve        (501) staff       (20)      416 2023-06-02 21:07:53.000000 py-evm-0.7.0a3/eth/vm/spoof.py
+-rw-r--r--   0 eve        (501) staff       (20)     7713 2023-06-02 21:07:53.000000 py-evm-0.7.0a3/eth/vm/stack.py
+-rw-r--r--   0 eve        (501) staff       (20)    10406 2023-06-02 21:07:53.000000 py-evm-0.7.0a3/eth/vm/state.py
+-rw-r--r--   0 eve        (501) staff       (20)      875 2023-06-02 21:07:53.000000 py-evm-0.7.0a3/eth/vm/transaction_context.py
+drwxr-xr-x   0 eve        (501) staff       (20)        0 2023-06-08 20:25:34.270971 py-evm-0.7.0a3/py_evm.egg-info/
+-rw-r--r--   0 eve        (501) staff       (20)     2977 2023-06-08 20:25:31.000000 py-evm-0.7.0a3/py_evm.egg-info/PKG-INFO
+-rw-r--r--   0 eve        (501) staff       (20)     8485 2023-06-08 20:25:34.000000 py-evm-0.7.0a3/py_evm.egg-info/SOURCES.txt
+-rw-r--r--   0 eve        (501) staff       (20)        1 2023-06-08 20:25:31.000000 py-evm-0.7.0a3/py_evm.egg-info/dependency_links.txt
+-rw-r--r--   0 eve        (501) staff       (20)        1 2021-02-24 18:15:32.000000 py-evm-0.7.0a3/py_evm.egg-info/not-zip-safe
+-rw-r--r--   0 eve        (501) staff       (20)     2144 2023-06-08 20:25:32.000000 py-evm-0.7.0a3/py_evm.egg-info/requires.txt
+-rw-r--r--   0 eve        (501) staff       (20)        4 2023-06-08 20:25:32.000000 py-evm-0.7.0a3/py_evm.egg-info/top_level.txt
+-rw-r--r--   0 eve        (501) staff       (20)     1117 2023-06-08 20:21:10.000000 py-evm-0.7.0a3/pyproject.toml
+-rw-r--r--   0 eve        (501) staff       (20)       38 2023-06-08 20:25:34.271501 py-evm-0.7.0a3/setup.cfg
+-rw-r--r--   0 eve        (501) staff       (20)     4043 2023-06-08 20:25:28.000000 py-evm-0.7.0a3/setup.py
```

### Comparing `py-evm-0.7.0a2/LICENSE` & `py-evm-0.7.0a3/LICENSE`

 * *Files identical despite different names*

### Comparing `py-evm-0.7.0a2/PKG-INFO` & `py-evm-0.7.0a3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py-evm
-Version: 0.7.0a2
+Version: 0.7.0a3
 Summary: Python implementation of the Ethereum Virtual Machine
 Home-page: https://github.com/ethereum/py-evm
 Author: Ethereum Foundation
 Author-email: piper@pipermerriam.com
 License: MIT
 Keywords: ethereum blockchain evm
 Classifier: Development Status :: 3 - Alpha
@@ -16,15 +16,15 @@
 Classifier: Programming Language :: Python :: 3.9
 Description-Content-Type: text/markdown
 Provides-Extra: eth
 Provides-Extra: eth-extra
 Provides-Extra: test
 Provides-Extra: lint
 Provides-Extra: benchmark
-Provides-Extra: doc
+Provides-Extra: docs
 Provides-Extra: dev
 License-File: LICENSE
 
 # Python Implementation of the Ethereum protocol
 
 [![Join the conversation on Discord](https://img.shields.io/discord/809793915578089484?color=blue&label=chat&logo=discord&logoColor=white)](https://discord.gg/GHryRvPB84)
 [![Build Status](https://circleci.com/gh/ethereum/py-evm.svg?style=shield)](https://circleci.com/gh/ethereum/py-evm)
```

### Comparing `py-evm-0.7.0a2/README.md` & `py-evm-0.7.0a3/README.md`

 * *Files identical despite different names*

### Comparing `py-evm-0.7.0a2/eth/_utils/address.py` & `py-evm-0.7.0a3/eth/_utils/address.py`

 * *Files identical despite different names*

### Comparing `py-evm-0.7.0a2/eth/_utils/blake2/coders.py` & `py-evm-0.7.0a3/eth/_utils/blake2/coders.py`

 * *Files identical despite different names*

### Comparing `py-evm-0.7.0a2/eth/_utils/blake2/compression.py` & `py-evm-0.7.0a3/eth/_utils/blake2/compression.py`

 * *Files identical despite different names*

### Comparing `py-evm-0.7.0a2/eth/_utils/bn128.py` & `py-evm-0.7.0a3/eth/_utils/bn128.py`

 * *Files identical despite different names*

### Comparing `py-evm-0.7.0a2/eth/_utils/datatypes.py` & `py-evm-0.7.0a3/eth/_utils/datatypes.py`

 * *Files identical despite different names*

### Comparing `py-evm-0.7.0a2/eth/_utils/db.py` & `py-evm-0.7.0a3/eth/_utils/db.py`

 * *Files identical despite different names*

### Comparing `py-evm-0.7.0a2/eth/_utils/env.py` & `py-evm-0.7.0a3/eth/_utils/env.py`

 * *Files identical despite different names*

### Comparing `py-evm-0.7.0a2/eth/_utils/generator.py` & `py-evm-0.7.0a3/eth/_utils/generator.py`

 * *Files identical despite different names*

### Comparing `py-evm-0.7.0a2/eth/_utils/headers.py` & `py-evm-0.7.0a3/eth/_utils/headers.py`

 * *Files identical despite different names*

### Comparing `py-evm-0.7.0a2/eth/_utils/module_loading.py` & `py-evm-0.7.0a3/eth/_utils/module_loading.py`

 * *Files identical despite different names*

### Comparing `py-evm-0.7.0a2/eth/_utils/numeric.py` & `py-evm-0.7.0a3/eth/_utils/numeric.py`

 * *Files identical despite different names*

### Comparing `py-evm-0.7.0a2/eth/_utils/rlp.py` & `py-evm-0.7.0a3/eth/_utils/rlp.py`

 * *Files identical despite different names*

### Comparing `py-evm-0.7.0a2/eth/_utils/spoof.py` & `py-evm-0.7.0a3/eth/_utils/spoof.py`

 * *Files identical despite different names*

### Comparing `py-evm-0.7.0a2/eth/_utils/state.py` & `py-evm-0.7.0a3/eth/_utils/state.py`

 * *Files identical despite different names*

### Comparing `py-evm-0.7.0a2/eth/_utils/transactions.py` & `py-evm-0.7.0a3/eth/_utils/transactions.py`

 * *Files identical despite different names*

### Comparing `py-evm-0.7.0a2/eth/abc.py` & `py-evm-0.7.0a3/eth/abc.py`

 * *Files 1% similar despite different names*

```diff
@@ -237,15 +237,15 @@
 
     @property
     @abstractmethod
     def bloom_filter(self) -> BloomFilter:
         ...
 
     # We can remove this API and inherit from rlp.Serializable when it becomes typesafe
-    def copy(self, *args: Any, **kwargs: Any) -> "ReceiptAPI":
+    def copy(self, *args: Any, **kwargs: Any) -> "ReceiptAPI":  # noqa: B027
         """
         Return a copy of the receipt, optionally overwriting any of its properties.
         """
         # This method isn't marked abstract because derived classes implement it by
         # deriving from rlp.Serializable but mypy won't recognize it as implemented.
         ...
 
@@ -872,15 +872,15 @@
         """
         Return ``True`` if this block represents the genesis block of the chain,
         otherwise ``False``.
         """
         ...
 
     # We can remove this API and inherit from rlp.Serializable when it becomes typesafe
-    def copy(self, *args: Any, **kwargs: Any) -> "BlockAPI":
+    def copy(self, *args: Any, **kwargs: Any) -> "BlockAPI":  # noqa: B027
         """
         Return a copy of the block, optionally overwriting any of its properties.
         """
         # This method isn't marked abstract because derived classes implement it by
         # deriving from rlp.Serializable but mypy won't recognize it as implemented.
         ...
 
@@ -3898,15 +3898,17 @@
         Return the class which should be used for the `headerdb`
         """
         ...
 
     #
     # Canonical Chain API
     #
-    def get_canonical_block_hash(self, block_number: BlockNumber) -> Hash32:
+    def get_canonical_block_hash(  # noqa: B027
+        self, block_number: BlockNumber
+    ) -> Hash32:
         """
         Direct passthrough to `headerdb`
         """
 
     @abstractmethod
     def get_canonical_block_header_by_number(
         self, block_number: BlockNumber
```

### Comparing `py-evm-0.7.0a2/eth/chains/base.py` & `py-evm-0.7.0a3/eth/chains/base.py`

 * *Files identical despite different names*

### Comparing `py-evm-0.7.0a2/eth/chains/goerli/__init__.py` & `py-evm-0.7.0a3/eth/chains/goerli/__init__.py`

 * *Files identical despite different names*

### Comparing `py-evm-0.7.0a2/eth/chains/header.py` & `py-evm-0.7.0a3/eth/chains/header.py`

 * *Files identical despite different names*

### Comparing `py-evm-0.7.0a2/eth/chains/mainnet/__init__.py` & `py-evm-0.7.0a3/eth/chains/mainnet/__init__.py`

 * *Files identical despite different names*

### Comparing `py-evm-0.7.0a2/eth/chains/mainnet/constants.py` & `py-evm-0.7.0a3/eth/chains/mainnet/constants.py`

 * *Files identical despite different names*

### Comparing `py-evm-0.7.0a2/eth/chains/ropsten/__init__.py` & `py-evm-0.7.0a3/eth/chains/ropsten/__init__.py`

 * *Files identical despite different names*

### Comparing `py-evm-0.7.0a2/eth/chains/ropsten/constants.py` & `py-evm-0.7.0a3/eth/chains/ropsten/constants.py`

 * *Files identical despite different names*

### Comparing `py-evm-0.7.0a2/eth/chains/tester/__init__.py` & `py-evm-0.7.0a3/eth/chains/tester/__init__.py`

 * *Files identical despite different names*

### Comparing `py-evm-0.7.0a2/eth/consensus/applier.py` & `py-evm-0.7.0a3/eth/consensus/applier.py`

 * *Files identical despite different names*

### Comparing `py-evm-0.7.0a2/eth/consensus/clique/_utils.py` & `py-evm-0.7.0a3/eth/consensus/clique/_utils.py`

 * *Files identical despite different names*

### Comparing `py-evm-0.7.0a2/eth/consensus/clique/clique.py` & `py-evm-0.7.0a3/eth/consensus/clique/clique.py`

 * *Files identical despite different names*

### Comparing `py-evm-0.7.0a2/eth/consensus/clique/datatypes.py` & `py-evm-0.7.0a3/eth/consensus/clique/datatypes.py`

 * *Files identical despite different names*

### Comparing `py-evm-0.7.0a2/eth/consensus/clique/encoding.py` & `py-evm-0.7.0a3/eth/consensus/clique/encoding.py`

 * *Files identical despite different names*

### Comparing `py-evm-0.7.0a2/eth/consensus/clique/snapshot_manager.py` & `py-evm-0.7.0a3/eth/consensus/clique/snapshot_manager.py`

 * *Files identical despite different names*

### Comparing `py-evm-0.7.0a2/eth/consensus/noproof.py` & `py-evm-0.7.0a3/eth/consensus/noproof.py`

 * *Files identical despite different names*

### Comparing `py-evm-0.7.0a2/eth/consensus/pos.py` & `py-evm-0.7.0a3/eth/consensus/pos.py`

 * *Files identical despite different names*

### Comparing `py-evm-0.7.0a2/eth/consensus/pow.py` & `py-evm-0.7.0a3/eth/consensus/pow.py`

 * *Files identical despite different names*

### Comparing `py-evm-0.7.0a2/eth/constants.py` & `py-evm-0.7.0a3/eth/constants.py`

 * *Files identical despite different names*

### Comparing `py-evm-0.7.0a2/eth/db/__init__.py` & `py-evm-0.7.0a3/eth/db/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,8 +17,8 @@
         )
     return cast(Type[AtomicDatabaseAPI], import_string(import_path))
 
 
 def get_db_backend(import_path: str = None, **init_kwargs: Any) -> AtomicDatabaseAPI:
     backend_class = get_db_backend_class(import_path)
     # mypy doesn't understand the constructor  of AtomicDatabaseAPI
-    return backend_class(**init_kwargs)  # type: ignore
+    return backend_class(**init_kwargs)
```

### Comparing `py-evm-0.7.0a2/eth/db/accesslog.py` & `py-evm-0.7.0a3/eth/db/accesslog.py`

 * *Files identical despite different names*

### Comparing `py-evm-0.7.0a2/eth/db/account.py` & `py-evm-0.7.0a3/eth/db/account.py`

 * *Files 1% similar despite different names*

```diff
@@ -73,14 +73,15 @@
 )
 from eth.typing import (
     JournalDBCheckpoint,
 )
 from eth.validation import (
     validate_canonical_address,
     validate_is_bytes,
+    validate_uint64,
     validate_uint256,
 )
 from eth.vm.interrupt import (
     MissingAccountTrieNode,
     MissingBytecode,
 )
 
@@ -283,15 +284,15 @@
         validate_canonical_address(address, title="Storage Address")
 
         account = self._get_account(address)
         return account.nonce
 
     def set_nonce(self, address: Address, nonce: int) -> None:
         validate_canonical_address(address, title="Storage Address")
-        validate_uint256(nonce, title="Nonce")
+        validate_uint64(nonce, title="Nonce")
 
         account = self._get_account(address)
         self._set_account(address, account.copy(nonce=nonce))
 
     def increment_nonce(self, address: Address) -> None:
         current_nonce = self.get_nonce(address)
         self.set_nonce(address, current_nonce + 1)
```

### Comparing `py-evm-0.7.0a2/eth/db/atomic.py` & `py-evm-0.7.0a3/eth/db/atomic.py`

 * *Files identical despite different names*

### Comparing `py-evm-0.7.0a2/eth/db/backends/base.py` & `py-evm-0.7.0a3/eth/db/backends/base.py`

 * *Files identical despite different names*

### Comparing `py-evm-0.7.0a2/eth/db/backends/level.py` & `py-evm-0.7.0a3/eth/db/backends/level.py`

 * *Files identical despite different names*

### Comparing `py-evm-0.7.0a2/eth/db/backends/memory.py` & `py-evm-0.7.0a3/eth/db/backends/memory.py`

 * *Files identical despite different names*

### Comparing `py-evm-0.7.0a2/eth/db/batch.py` & `py-evm-0.7.0a3/eth/db/batch.py`

 * *Files identical despite different names*

### Comparing `py-evm-0.7.0a2/eth/db/cache.py` & `py-evm-0.7.0a3/eth/db/cache.py`

 * *Files identical despite different names*

### Comparing `py-evm-0.7.0a2/eth/db/chain.py` & `py-evm-0.7.0a3/eth/db/chain.py`

 * *Files 1% similar despite different names*

```diff
@@ -457,15 +457,15 @@
         if receipt_data != b"":
             return receipt_decoder.decode(receipt_data)
         else:
             raise ReceiptNotFound(
                 f"Receipt with index {receipt_index} not found in block"
             )
 
-    @functools.lru_cache(maxsize=32)
+    @functools.lru_cache(maxsize=32)  # noqa: B019
     @to_tuple
     def _get_block_transactions(
         self, transaction_root: Hash32, transaction_decoder: Type[TransactionDecoderAPI]
     ) -> Iterable[SignedTransactionAPI]:
         """
         Memoizable version of `get_block_transactions`
         """
@@ -511,15 +511,15 @@
     #
     def get_block_withdrawals(
         self,
         header: BlockHeaderAPI,
     ) -> Tuple[WithdrawalAPI, ...]:
         return self._get_block_withdrawals(header.withdrawals_root)
 
-    @functools.lru_cache(maxsize=32)
+    @functools.lru_cache(maxsize=32)  # noqa: B019
     @to_tuple
     def _get_block_withdrawals(
         self,
         withdrawals_root: Hash32,
     ) -> Iterable[WithdrawalAPI]:
         """
         Memoizable version of `get_block_withdrawals`
```

### Comparing `py-evm-0.7.0a2/eth/db/chain_gaps.py` & `py-evm-0.7.0a3/eth/db/chain_gaps.py`

 * *Files identical despite different names*

### Comparing `py-evm-0.7.0a2/eth/db/diff.py` & `py-evm-0.7.0a3/eth/db/diff.py`

 * *Files identical despite different names*

### Comparing `py-evm-0.7.0a2/eth/db/header.py` & `py-evm-0.7.0a3/eth/db/header.py`

 * *Files identical despite different names*

### Comparing `py-evm-0.7.0a2/eth/db/journal.py` & `py-evm-0.7.0a3/eth/db/journal.py`

 * *Files identical despite different names*

### Comparing `py-evm-0.7.0a2/eth/db/keymap.py` & `py-evm-0.7.0a3/eth/db/keymap.py`

 * *Files identical despite different names*

### Comparing `py-evm-0.7.0a2/eth/db/schema.py` & `py-evm-0.7.0a3/eth/db/schema.py`

 * *Files identical despite different names*

### Comparing `py-evm-0.7.0a2/eth/db/slow_journal.py` & `py-evm-0.7.0a3/eth/db/slow_journal.py`

 * *Files identical despite different names*

### Comparing `py-evm-0.7.0a2/eth/db/storage.py` & `py-evm-0.7.0a3/eth/db/storage.py`

 * *Files identical despite different names*

### Comparing `py-evm-0.7.0a2/eth/db/trie.py` & `py-evm-0.7.0a3/eth/db/trie.py`

 * *Files identical despite different names*

### Comparing `py-evm-0.7.0a2/eth/db/witness.py` & `py-evm-0.7.0a3/eth/db/witness.py`

 * *Files identical despite different names*

### Comparing `py-evm-0.7.0a2/eth/estimators/__init__.py` & `py-evm-0.7.0a3/eth/estimators/__init__.py`

 * *Files identical despite different names*

### Comparing `py-evm-0.7.0a2/eth/estimators/gas.py` & `py-evm-0.7.0a3/eth/estimators/gas.py`

 * *Files identical despite different names*

### Comparing `py-evm-0.7.0a2/eth/exceptions.py` & `py-evm-0.7.0a3/eth/exceptions.py`

 * *Files identical despite different names*

### Comparing `py-evm-0.7.0a2/eth/precompiles/blake2.py` & `py-evm-0.7.0a3/eth/precompiles/blake2.py`

 * *Files identical despite different names*

### Comparing `py-evm-0.7.0a2/eth/precompiles/ecadd.py` & `py-evm-0.7.0a3/eth/precompiles/ecadd.py`

 * *Files identical despite different names*

### Comparing `py-evm-0.7.0a2/eth/precompiles/ecmul.py` & `py-evm-0.7.0a3/eth/precompiles/ecmul.py`

 * *Files identical despite different names*

### Comparing `py-evm-0.7.0a2/eth/precompiles/ecpairing.py` & `py-evm-0.7.0a3/eth/precompiles/ecpairing.py`

 * *Files identical despite different names*

### Comparing `py-evm-0.7.0a2/eth/precompiles/ecrecover.py` & `py-evm-0.7.0a3/eth/precompiles/ecrecover.py`

 * *Files identical despite different names*

### Comparing `py-evm-0.7.0a2/eth/precompiles/modexp.py` & `py-evm-0.7.0a3/eth/precompiles/modexp.py`

 * *Files identical despite different names*

### Comparing `py-evm-0.7.0a2/eth/precompiles/ripemd160.py` & `py-evm-0.7.0a3/eth/precompiles/ripemd160.py`

 * *Files identical despite different names*

### Comparing `py-evm-0.7.0a2/eth/precompiles/sha256.py` & `py-evm-0.7.0a3/eth/precompiles/sha256.py`

 * *Files identical despite different names*

### Comparing `py-evm-0.7.0a2/eth/rlp/accounts.py` & `py-evm-0.7.0a3/eth/rlp/accounts.py`

 * *Files identical despite different names*

### Comparing `py-evm-0.7.0a2/eth/rlp/blocks.py` & `py-evm-0.7.0a3/eth/rlp/blocks.py`

 * *Files identical despite different names*

### Comparing `py-evm-0.7.0a2/eth/rlp/headers.py` & `py-evm-0.7.0a3/eth/rlp/headers.py`

 * *Files identical despite different names*

### Comparing `py-evm-0.7.0a2/eth/rlp/logs.py` & `py-evm-0.7.0a3/eth/rlp/logs.py`

 * *Files identical despite different names*

### Comparing `py-evm-0.7.0a2/eth/rlp/receipts.py` & `py-evm-0.7.0a3/eth/rlp/receipts.py`

 * *Files identical despite different names*

### Comparing `py-evm-0.7.0a2/eth/rlp/transactions.py` & `py-evm-0.7.0a3/eth/rlp/transactions.py`

 * *Files identical despite different names*

### Comparing `py-evm-0.7.0a2/eth/tools/_utils/deprecation.py` & `py-evm-0.7.0a3/eth/tools/_utils/deprecation.py`

 * *Files 20% similar despite different names*

```diff
@@ -16,11 +16,12 @@
         warnings.warn(
             category=DeprecationWarning,
             message=(
                 message
                 or f"{func.__name__} is deprecated. "
                 "A breaking change is expected in a future release."
             ),
+            stacklevel=2,
         )
         func(*args, **kwargs)
 
     return cast(TFunc, deprecated_func)
```

### Comparing `py-evm-0.7.0a2/eth/tools/_utils/hashing.py` & `py-evm-0.7.0a3/eth/tools/_utils/hashing.py`

 * *Files identical despite different names*

### Comparing `py-evm-0.7.0a2/eth/tools/_utils/mappings.py` & `py-evm-0.7.0a3/eth/tools/_utils/mappings.py`

 * *Files identical despite different names*

### Comparing `py-evm-0.7.0a2/eth/tools/_utils/normalization.py` & `py-evm-0.7.0a3/eth/tools/_utils/normalization.py`

 * *Files identical despite different names*

### Comparing `py-evm-0.7.0a2/eth/tools/_utils/slow_code_stream.py` & `py-evm-0.7.0a3/eth/tools/_utils/slow_code_stream.py`

 * *Files identical despite different names*

### Comparing `py-evm-0.7.0a2/eth/tools/_utils/vyper.py` & `py-evm-0.7.0a3/eth/tools/_utils/vyper.py`

 * *Files identical despite different names*

### Comparing `py-evm-0.7.0a2/eth/tools/builder/chain/__init__.py` & `py-evm-0.7.0a3/eth/tools/builder/chain/__init__.py`

 * *Files identical despite different names*

### Comparing `py-evm-0.7.0a2/eth/tools/builder/chain/builders.py` & `py-evm-0.7.0a3/eth/tools/builder/chain/builders.py`

 * *Files identical despite different names*

### Comparing `py-evm-0.7.0a2/eth/tools/db/atomic.py` & `py-evm-0.7.0a3/eth/tools/db/atomic.py`

 * *Files 0% similar despite different names*

```diff
@@ -101,15 +101,15 @@
             batch[b"1"]
 
         with pytest.raises(ValidationError):
             batch.get(b"1")
 
         # exists
         with pytest.raises(ValidationError):
-            b"1" in batch
+            assert b"1" in batch
 
         with pytest.raises(ValidationError):
             batch.exists(b"1")
 
         # delete
         with pytest.raises(ValidationError):
             del batch[b"1"]
```

### Comparing `py-evm-0.7.0a2/eth/tools/db/base.py` & `py-evm-0.7.0a3/eth/tools/db/base.py`

 * *Files identical despite different names*

### Comparing `py-evm-0.7.0a2/eth/tools/fixtures/__init__.py` & `py-evm-0.7.0a3/eth/tools/fixtures/__init__.py`

 * *Files identical despite different names*

### Comparing `py-evm-0.7.0a2/eth/tools/fixtures/_utils.py` & `py-evm-0.7.0a3/eth/tools/fixtures/_utils.py`

 * *Files identical despite different names*

### Comparing `py-evm-0.7.0a2/eth/tools/fixtures/fillers/_utils.py` & `py-evm-0.7.0a3/eth/tools/fixtures/fillers/_utils.py`

 * *Files identical despite different names*

### Comparing `py-evm-0.7.0a2/eth/tools/fixtures/fillers/common.py` & `py-evm-0.7.0a3/eth/tools/fixtures/fillers/common.py`

 * *Files 0% similar despite different names*

```diff
@@ -93,15 +93,15 @@
     "gasPrice": 1,
     "gas": 100000,
 }
 
 
 Test = namedtuple("Test", ["filler", "fill_kwargs"])
 # make `None` default for fill_kwargs
-Test.__new__.__defaults__ = (None,)  # type: ignore
+Test.__new__.__defaults__ = (None,)
 
 
 #
 # Filler Generation
 #
```

### Comparing `py-evm-0.7.0a2/eth/tools/fixtures/fillers/formatters.py` & `py-evm-0.7.0a3/eth/tools/fixtures/fillers/formatters.py`

 * *Files identical despite different names*

### Comparing `py-evm-0.7.0a2/eth/tools/fixtures/fillers/main.py` & `py-evm-0.7.0a3/eth/tools/fixtures/fillers/main.py`

 * *Files identical despite different names*

### Comparing `py-evm-0.7.0a2/eth/tools/fixtures/fillers/state.py` & `py-evm-0.7.0a3/eth/tools/fixtures/fillers/state.py`

 * *Files identical despite different names*

### Comparing `py-evm-0.7.0a2/eth/tools/fixtures/fillers/vm.py` & `py-evm-0.7.0a3/eth/tools/fixtures/fillers/vm.py`

 * *Files identical despite different names*

### Comparing `py-evm-0.7.0a2/eth/tools/fixtures/generation.py` & `py-evm-0.7.0a3/eth/tools/fixtures/generation.py`

 * *Files identical despite different names*

### Comparing `py-evm-0.7.0a2/eth/tools/fixtures/helpers.py` & `py-evm-0.7.0a3/eth/tools/fixtures/helpers.py`

 * *Files identical despite different names*

### Comparing `py-evm-0.7.0a2/eth/tools/fixtures/loading.py` & `py-evm-0.7.0a3/eth/tools/fixtures/loading.py`

 * *Files identical despite different names*

### Comparing `py-evm-0.7.0a2/eth/tools/mining.py` & `py-evm-0.7.0a3/eth/tools/mining.py`

 * *Files identical despite different names*

### Comparing `py-evm-0.7.0a2/eth/typing.py` & `py-evm-0.7.0a3/eth/typing.py`

 * *Files identical despite different names*

### Comparing `py-evm-0.7.0a2/eth/validation.py` & `py-evm-0.7.0a3/eth/validation.py`

 * *Files identical despite different names*

### Comparing `py-evm-0.7.0a2/eth/vm/base.py` & `py-evm-0.7.0a3/eth/vm/base.py`

 * *Files identical despite different names*

### Comparing `py-evm-0.7.0a2/eth/vm/chain_context.py` & `py-evm-0.7.0a3/eth/vm/chain_context.py`

 * *Files identical despite different names*

### Comparing `py-evm-0.7.0a2/eth/vm/code_stream.py` & `py-evm-0.7.0a3/eth/vm/code_stream.py`

 * *Files 4% similar despite different names*

```diff
@@ -20,25 +20,25 @@
 
 class CodeStream(CodeStreamAPI):
     __slots__ = [
         "_length_cache",
         "_raw_code_bytes",
         "invalid_positions",
         "valid_positions",
-        "pc",
+        "program_counter",
     ]
 
     logger = logging.getLogger("eth.vm.CodeStream")
 
     def __init__(self, code_bytes: bytes) -> None:
         validate_is_bytes(code_bytes, title="CodeStream bytes")
-        # in order to avoid method overhead when setting/accessing pc, we no longer
-        # fence the pc (Program Counter) into 0 <= pc <= len(code_bytes).
+        # in order to avoid method overhead when setting/accessing program_counter,
+        # we no longer fence it into 0 <= program_counter <= len(code_bytes).
         # We now let it float free.
-        # NOTE: Setting pc to a negative value has undefined behavior.
+        # NOTE: Setting program_counter to a negative value has undefined behavior.
         self.program_counter = 0
         self._raw_code_bytes = code_bytes
         self._length_cache = len(code_bytes)
         self.invalid_positions: Set[int] = set()
         self.valid_positions: Set[int] = set()
 
     def read(self, size: int) -> bytes:
```

### Comparing `py-evm-0.7.0a2/eth/vm/computation.py` & `py-evm-0.7.0a3/eth/vm/computation.py`

 * *Files identical despite different names*

### Comparing `py-evm-0.7.0a2/eth/vm/execution_context.py` & `py-evm-0.7.0a3/eth/vm/execution_context.py`

 * *Files identical despite different names*

### Comparing `py-evm-0.7.0a2/eth/vm/forks/__init__.py` & `py-evm-0.7.0a3/eth/vm/forks/__init__.py`

 * *Files identical despite different names*

### Comparing `py-evm-0.7.0a2/eth/vm/forks/arrow_glacier/__init__.py` & `py-evm-0.7.0a3/eth/vm/forks/arrow_glacier/__init__.py`

 * *Files identical despite different names*

### Comparing `py-evm-0.7.0a2/eth/vm/forks/arrow_glacier/blocks.py` & `py-evm-0.7.0a3/eth/vm/forks/arrow_glacier/blocks.py`

 * *Files identical despite different names*

### Comparing `py-evm-0.7.0a2/eth/vm/forks/arrow_glacier/headers.py` & `py-evm-0.7.0a3/eth/vm/forks/arrow_glacier/headers.py`

 * *Files identical despite different names*

### Comparing `py-evm-0.7.0a2/eth/vm/forks/arrow_glacier/state.py` & `py-evm-0.7.0a3/eth/vm/forks/arrow_glacier/state.py`

 * *Files identical despite different names*

### Comparing `py-evm-0.7.0a2/eth/vm/forks/arrow_glacier/transactions.py` & `py-evm-0.7.0a3/eth/vm/forks/arrow_glacier/transactions.py`

 * *Files identical despite different names*

### Comparing `py-evm-0.7.0a2/eth/vm/forks/berlin/__init__.py` & `py-evm-0.7.0a3/eth/vm/forks/berlin/__init__.py`

 * *Files identical despite different names*

### Comparing `py-evm-0.7.0a2/eth/vm/forks/berlin/blocks.py` & `py-evm-0.7.0a3/eth/vm/forks/berlin/blocks.py`

 * *Files identical despite different names*

### Comparing `py-evm-0.7.0a2/eth/vm/forks/berlin/computation.py` & `py-evm-0.7.0a3/eth/vm/forks/berlin/computation.py`

 * *Files identical despite different names*

### Comparing `py-evm-0.7.0a2/eth/vm/forks/berlin/logic.py` & `py-evm-0.7.0a3/eth/vm/forks/berlin/logic.py`

 * *Files identical despite different names*

### Comparing `py-evm-0.7.0a2/eth/vm/forks/berlin/opcodes.py` & `py-evm-0.7.0a3/eth/vm/forks/berlin/opcodes.py`

 * *Files identical despite different names*

### Comparing `py-evm-0.7.0a2/eth/vm/forks/berlin/receipts.py` & `py-evm-0.7.0a3/eth/vm/forks/berlin/receipts.py`

 * *Files identical despite different names*

### Comparing `py-evm-0.7.0a2/eth/vm/forks/berlin/state.py` & `py-evm-0.7.0a3/eth/vm/forks/berlin/state.py`

 * *Files identical despite different names*

### Comparing `py-evm-0.7.0a2/eth/vm/forks/berlin/transactions.py` & `py-evm-0.7.0a3/eth/vm/forks/berlin/transactions.py`

 * *Files 1% similar despite different names*

```diff
@@ -67,14 +67,15 @@
 from eth.rlp.transactions import (
     SignedTransactionMethods,
 )
 from eth.validation import (
     validate_canonical_address,
     validate_is_bytes,
     validate_is_transaction_access_list,
+    validate_uint64,
     validate_uint256,
 )
 from eth.vm.forks.istanbul.transactions import (
     ISTANBUL_TX_GAS_SCHEDULE,
 )
 from eth.vm.forks.muir_glacier.transactions import (
     MuirGlacierTransaction,
@@ -160,15 +161,15 @@
             r,
             s,
         )
         return TypedTransaction(self._type_id, signed_transaction)
 
     def validate(self) -> None:
         validate_uint256(self.chain_id, title="Transaction.chain_id")
-        validate_uint256(self.nonce, title="Transaction.nonce")
+        validate_uint64(self.nonce, title="Transaction.nonce")
         validate_uint256(self.gas_price, title="Transaction.gas_price")
         validate_uint256(self.gas, title="Transaction.gas")
         if self.to != CREATE_CONTRACT_ADDRESS:
             validate_canonical_address(self.to, title="Transaction.to")
         validate_uint256(self.value, title="Transaction.value")
         validate_is_bytes(self.data, title="Transaction.data")
         validate_is_transaction_access_list(self.access_list)
```

### Comparing `py-evm-0.7.0a2/eth/vm/forks/byzantium/__init__.py` & `py-evm-0.7.0a3/eth/vm/forks/byzantium/__init__.py`

 * *Files identical despite different names*

### Comparing `py-evm-0.7.0a2/eth/vm/forks/byzantium/computation.py` & `py-evm-0.7.0a3/eth/vm/forks/byzantium/computation.py`

 * *Files identical despite different names*

### Comparing `py-evm-0.7.0a2/eth/vm/forks/byzantium/headers.py` & `py-evm-0.7.0a3/eth/vm/forks/byzantium/headers.py`

 * *Files identical despite different names*

### Comparing `py-evm-0.7.0a2/eth/vm/forks/byzantium/opcodes.py` & `py-evm-0.7.0a3/eth/vm/forks/byzantium/opcodes.py`

 * *Files identical despite different names*

### Comparing `py-evm-0.7.0a2/eth/vm/forks/byzantium/transactions.py` & `py-evm-0.7.0a3/eth/vm/forks/byzantium/transactions.py`

 * *Files identical despite different names*

### Comparing `py-evm-0.7.0a2/eth/vm/forks/constantinople/__init__.py` & `py-evm-0.7.0a3/eth/vm/forks/constantinople/__init__.py`

 * *Files identical despite different names*

### Comparing `py-evm-0.7.0a2/eth/vm/forks/constantinople/computation.py` & `py-evm-0.7.0a3/eth/vm/forks/constantinople/computation.py`

 * *Files identical despite different names*

### Comparing `py-evm-0.7.0a2/eth/vm/forks/constantinople/opcodes.py` & `py-evm-0.7.0a3/eth/vm/forks/constantinople/opcodes.py`

 * *Files identical despite different names*

### Comparing `py-evm-0.7.0a2/eth/vm/forks/constantinople/transactions.py` & `py-evm-0.7.0a3/eth/vm/forks/constantinople/transactions.py`

 * *Files identical despite different names*

### Comparing `py-evm-0.7.0a2/eth/vm/forks/frontier/__init__.py` & `py-evm-0.7.0a3/eth/vm/forks/frontier/__init__.py`

 * *Files identical despite different names*

### Comparing `py-evm-0.7.0a2/eth/vm/forks/frontier/blocks.py` & `py-evm-0.7.0a3/eth/vm/forks/frontier/blocks.py`

 * *Files identical despite different names*

### Comparing `py-evm-0.7.0a2/eth/vm/forks/frontier/computation.py` & `py-evm-0.7.0a3/eth/vm/forks/frontier/computation.py`

 * *Files identical despite different names*

### Comparing `py-evm-0.7.0a2/eth/vm/forks/frontier/headers.py` & `py-evm-0.7.0a3/eth/vm/forks/frontier/headers.py`

 * *Files identical despite different names*

### Comparing `py-evm-0.7.0a2/eth/vm/forks/frontier/opcodes.py` & `py-evm-0.7.0a3/eth/vm/forks/frontier/opcodes.py`

 * *Files identical despite different names*

### Comparing `py-evm-0.7.0a2/eth/vm/forks/frontier/state.py` & `py-evm-0.7.0a3/eth/vm/forks/frontier/state.py`

 * *Files identical despite different names*

### Comparing `py-evm-0.7.0a2/eth/vm/forks/frontier/transactions.py` & `py-evm-0.7.0a3/eth/vm/forks/frontier/transactions.py`

 * *Files 2% similar despite different names*

```diff
@@ -44,14 +44,15 @@
 from eth.validation import (
     validate_canonical_address,
     validate_gte,
     validate_is_bytes,
     validate_is_integer,
     validate_lt_secpk1n,
     validate_lte,
+    validate_uint64,
     validate_uint256,
 )
 
 FRONTIER_TX_GAS_SCHEDULE = IntrinsicGasSchedule(
     gas_tx=GAS_TX,
     gas_txcreate=0,
     gas_txdatazero=GAS_TXDATAZERO,
@@ -72,15 +73,15 @@
         return V_OFFSET
 
     @property
     def v_max(self) -> int:
         return V_OFFSET + 1
 
     def validate(self) -> None:
-        validate_uint256(self.nonce, title="Transaction.nonce")
+        validate_uint64(self.nonce, title="Transaction.nonce")
         validate_uint256(self.gas_price, title="Transaction.gas_price")
         validate_uint256(self.gas, title="Transaction.gas")
         if self.to != CREATE_CONTRACT_ADDRESS:
             validate_canonical_address(self.to, title="Transaction.to")
         validate_uint256(self.value, title="Transaction.value")
         validate_is_bytes(self.data, title="Transaction.data")
 
@@ -172,15 +173,15 @@
     @property
     def max_fee_per_gas(self) -> int:
         return self.gas_price
 
 
 class FrontierUnsignedTransaction(BaseUnsignedTransaction):
     def validate(self) -> None:
-        validate_uint256(self.nonce, title="Transaction.nonce")
+        validate_uint64(self.nonce, title="Transaction.nonce")
         validate_is_integer(self.gas_price, title="Transaction.gas_price")
         validate_uint256(self.gas, title="Transaction.gas")
         if self.to != CREATE_CONTRACT_ADDRESS:
             validate_canonical_address(self.to, title="Transaction.to")
         validate_uint256(self.value, title="Transaction.value")
         validate_is_bytes(self.data, title="Transaction.data")
         super().validate()
```

### Comparing `py-evm-0.7.0a2/eth/vm/forks/frontier/validation.py` & `py-evm-0.7.0a3/eth/vm/forks/frontier/validation.py`

 * *Files identical despite different names*

### Comparing `py-evm-0.7.0a2/eth/vm/forks/gray_glacier/__init__.py` & `py-evm-0.7.0a3/eth/vm/forks/gray_glacier/__init__.py`

 * *Files identical despite different names*

### Comparing `py-evm-0.7.0a2/eth/vm/forks/gray_glacier/blocks.py` & `py-evm-0.7.0a3/eth/vm/forks/gray_glacier/blocks.py`

 * *Files identical despite different names*

### Comparing `py-evm-0.7.0a2/eth/vm/forks/gray_glacier/headers.py` & `py-evm-0.7.0a3/eth/vm/forks/gray_glacier/headers.py`

 * *Files identical despite different names*

### Comparing `py-evm-0.7.0a2/eth/vm/forks/gray_glacier/state.py` & `py-evm-0.7.0a3/eth/vm/forks/gray_glacier/state.py`

 * *Files identical despite different names*

### Comparing `py-evm-0.7.0a2/eth/vm/forks/gray_glacier/transactions.py` & `py-evm-0.7.0a3/eth/vm/forks/gray_glacier/transactions.py`

 * *Files identical despite different names*

### Comparing `py-evm-0.7.0a2/eth/vm/forks/homestead/__init__.py` & `py-evm-0.7.0a3/eth/vm/forks/homestead/__init__.py`

 * *Files identical despite different names*

### Comparing `py-evm-0.7.0a2/eth/vm/forks/homestead/computation.py` & `py-evm-0.7.0a3/eth/vm/forks/homestead/computation.py`

 * *Files identical despite different names*

### Comparing `py-evm-0.7.0a2/eth/vm/forks/homestead/headers.py` & `py-evm-0.7.0a3/eth/vm/forks/homestead/headers.py`

 * *Files identical despite different names*

### Comparing `py-evm-0.7.0a2/eth/vm/forks/homestead/opcodes.py` & `py-evm-0.7.0a3/eth/vm/forks/homestead/opcodes.py`

 * *Files identical despite different names*

### Comparing `py-evm-0.7.0a2/eth/vm/forks/homestead/state.py` & `py-evm-0.7.0a3/eth/vm/forks/homestead/state.py`

 * *Files identical despite different names*

### Comparing `py-evm-0.7.0a2/eth/vm/forks/homestead/transactions.py` & `py-evm-0.7.0a3/eth/vm/forks/homestead/transactions.py`

 * *Files identical despite different names*

### Comparing `py-evm-0.7.0a2/eth/vm/forks/homestead/validation.py` & `py-evm-0.7.0a3/eth/vm/forks/homestead/validation.py`

 * *Files identical despite different names*

### Comparing `py-evm-0.7.0a2/eth/vm/forks/istanbul/__init__.py` & `py-evm-0.7.0a3/eth/vm/forks/istanbul/__init__.py`

 * *Files identical despite different names*

### Comparing `py-evm-0.7.0a2/eth/vm/forks/istanbul/computation.py` & `py-evm-0.7.0a3/eth/vm/forks/istanbul/computation.py`

 * *Files identical despite different names*

### Comparing `py-evm-0.7.0a2/eth/vm/forks/istanbul/opcodes.py` & `py-evm-0.7.0a3/eth/vm/forks/istanbul/opcodes.py`

 * *Files identical despite different names*

### Comparing `py-evm-0.7.0a2/eth/vm/forks/istanbul/storage.py` & `py-evm-0.7.0a3/eth/vm/forks/istanbul/storage.py`

 * *Files identical despite different names*

### Comparing `py-evm-0.7.0a2/eth/vm/forks/istanbul/transactions.py` & `py-evm-0.7.0a3/eth/vm/forks/istanbul/transactions.py`

 * *Files identical despite different names*

### Comparing `py-evm-0.7.0a2/eth/vm/forks/london/__init__.py` & `py-evm-0.7.0a3/eth/vm/forks/london/__init__.py`

 * *Files identical despite different names*

### Comparing `py-evm-0.7.0a2/eth/vm/forks/london/blocks.py` & `py-evm-0.7.0a3/eth/vm/forks/london/blocks.py`

 * *Files identical despite different names*

### Comparing `py-evm-0.7.0a2/eth/vm/forks/london/computation.py` & `py-evm-0.7.0a3/eth/vm/forks/london/computation.py`

 * *Files identical despite different names*

### Comparing `py-evm-0.7.0a2/eth/vm/forks/london/headers.py` & `py-evm-0.7.0a3/eth/vm/forks/london/headers.py`

 * *Files identical despite different names*

### Comparing `py-evm-0.7.0a2/eth/vm/forks/london/opcodes.py` & `py-evm-0.7.0a3/eth/vm/forks/london/opcodes.py`

 * *Files identical despite different names*

### Comparing `py-evm-0.7.0a2/eth/vm/forks/london/receipts.py` & `py-evm-0.7.0a3/eth/vm/forks/london/receipts.py`

 * *Files identical despite different names*

### Comparing `py-evm-0.7.0a2/eth/vm/forks/london/state.py` & `py-evm-0.7.0a3/eth/vm/forks/london/state.py`

 * *Files identical despite different names*

### Comparing `py-evm-0.7.0a2/eth/vm/forks/london/storage.py` & `py-evm-0.7.0a3/eth/vm/forks/london/storage.py`

 * *Files identical despite different names*

### Comparing `py-evm-0.7.0a2/eth/vm/forks/london/transactions.py` & `py-evm-0.7.0a3/eth/vm/forks/london/transactions.py`

 * *Files 2% similar despite different names*

```diff
@@ -52,14 +52,15 @@
 from eth.rlp.transactions import (
     SignedTransactionMethods,
 )
 from eth.validation import (
     validate_canonical_address,
     validate_is_bytes,
     validate_is_transaction_access_list,
+    validate_uint64,
     validate_uint256,
 )
 from eth.vm.forks.berlin.constants import (
     ACCESS_LIST_ADDRESS_COST_EIP_2930,
     ACCESS_LIST_STORAGE_KEY_COST_EIP_2930,
     ACCESS_LIST_TRANSACTION_TYPE,
 )
@@ -146,15 +147,15 @@
             r,
             s,
         )
         return LondonTypedTransaction(self._type_id, signed_transaction)
 
     def validate(self) -> None:
         validate_uint256(self.chain_id, title="Transaction.chain_id")
-        validate_uint256(self.nonce, title="Transaction.nonce")
+        validate_uint64(self.nonce, title="Transaction.nonce")
         validate_uint256(self.max_fee_per_gas, title="Transaction.max_fee_per_gas")
         validate_uint256(
             self.max_priority_fee_per_gas, title="Transaction.max_priority_fee_per_gas"
         )
         validate_uint256(self.gas, title="Transaction.gas")
         if self.to != CREATE_CONTRACT_ADDRESS:
             validate_canonical_address(self.to, title="Transaction.to")
```

### Comparing `py-evm-0.7.0a2/eth/vm/forks/london/validation.py` & `py-evm-0.7.0a3/eth/vm/forks/london/validation.py`

 * *Files identical despite different names*

### Comparing `py-evm-0.7.0a2/eth/vm/forks/muir_glacier/__init__.py` & `py-evm-0.7.0a3/eth/vm/forks/muir_glacier/__init__.py`

 * *Files identical despite different names*

### Comparing `py-evm-0.7.0a2/eth/vm/forks/muir_glacier/computation.py` & `py-evm-0.7.0a3/eth/vm/forks/muir_glacier/computation.py`

 * *Files identical despite different names*

### Comparing `py-evm-0.7.0a2/eth/vm/forks/muir_glacier/transactions.py` & `py-evm-0.7.0a3/eth/vm/forks/muir_glacier/transactions.py`

 * *Files identical despite different names*

### Comparing `py-evm-0.7.0a2/eth/vm/forks/paris/__init__.py` & `py-evm-0.7.0a3/eth/vm/forks/paris/__init__.py`

 * *Files identical despite different names*

### Comparing `py-evm-0.7.0a2/eth/vm/forks/paris/blocks.py` & `py-evm-0.7.0a3/eth/vm/forks/paris/blocks.py`

 * *Files identical despite different names*

### Comparing `py-evm-0.7.0a2/eth/vm/forks/paris/headers.py` & `py-evm-0.7.0a3/eth/vm/forks/paris/headers.py`

 * *Files identical despite different names*

### Comparing `py-evm-0.7.0a2/eth/vm/forks/paris/opcodes.py` & `py-evm-0.7.0a3/eth/vm/forks/paris/opcodes.py`

 * *Files identical despite different names*

### Comparing `py-evm-0.7.0a2/eth/vm/forks/paris/state.py` & `py-evm-0.7.0a3/eth/vm/forks/paris/state.py`

 * *Files identical despite different names*

### Comparing `py-evm-0.7.0a2/eth/vm/forks/paris/transactions.py` & `py-evm-0.7.0a3/eth/vm/forks/paris/transactions.py`

 * *Files identical despite different names*

### Comparing `py-evm-0.7.0a2/eth/vm/forks/petersburg/__init__.py` & `py-evm-0.7.0a3/eth/vm/forks/petersburg/__init__.py`

 * *Files identical despite different names*

### Comparing `py-evm-0.7.0a2/eth/vm/forks/petersburg/computation.py` & `py-evm-0.7.0a3/eth/vm/forks/petersburg/computation.py`

 * *Files identical despite different names*

### Comparing `py-evm-0.7.0a2/eth/vm/forks/petersburg/opcodes.py` & `py-evm-0.7.0a3/eth/vm/forks/petersburg/opcodes.py`

 * *Files identical despite different names*

### Comparing `py-evm-0.7.0a2/eth/vm/forks/petersburg/transactions.py` & `py-evm-0.7.0a3/eth/vm/forks/petersburg/transactions.py`

 * *Files identical despite different names*

### Comparing `py-evm-0.7.0a2/eth/vm/forks/shanghai/__init__.py` & `py-evm-0.7.0a3/eth/vm/forks/shanghai/__init__.py`

 * *Files identical despite different names*

### Comparing `py-evm-0.7.0a2/eth/vm/forks/shanghai/blocks.py` & `py-evm-0.7.0a3/eth/vm/forks/shanghai/blocks.py`

 * *Files identical despite different names*

### Comparing `py-evm-0.7.0a2/eth/vm/forks/shanghai/computation.py` & `py-evm-0.7.0a3/eth/vm/forks/shanghai/computation.py`

 * *Files identical despite different names*

### Comparing `py-evm-0.7.0a2/eth/vm/forks/shanghai/headers.py` & `py-evm-0.7.0a3/eth/vm/forks/shanghai/headers.py`

 * *Files identical despite different names*

### Comparing `py-evm-0.7.0a2/eth/vm/forks/shanghai/logic.py` & `py-evm-0.7.0a3/eth/vm/forks/shanghai/logic.py`

 * *Files identical despite different names*

### Comparing `py-evm-0.7.0a2/eth/vm/forks/shanghai/opcodes.py` & `py-evm-0.7.0a3/eth/vm/forks/shanghai/opcodes.py`

 * *Files identical despite different names*

### Comparing `py-evm-0.7.0a2/eth/vm/forks/shanghai/state.py` & `py-evm-0.7.0a3/eth/vm/forks/shanghai/state.py`

 * *Files identical despite different names*

### Comparing `py-evm-0.7.0a2/eth/vm/forks/shanghai/transactions.py` & `py-evm-0.7.0a3/eth/vm/forks/shanghai/transactions.py`

 * *Files identical despite different names*

### Comparing `py-evm-0.7.0a2/eth/vm/forks/shanghai/withdrawals.py` & `py-evm-0.7.0a3/eth/vm/forks/shanghai/withdrawals.py`

 * *Files identical despite different names*

### Comparing `py-evm-0.7.0a2/eth/vm/forks/spurious_dragon/_utils.py` & `py-evm-0.7.0a3/eth/vm/forks/spurious_dragon/_utils.py`

 * *Files identical despite different names*

### Comparing `py-evm-0.7.0a2/eth/vm/forks/spurious_dragon/computation.py` & `py-evm-0.7.0a3/eth/vm/forks/spurious_dragon/computation.py`

 * *Files identical despite different names*

### Comparing `py-evm-0.7.0a2/eth/vm/forks/spurious_dragon/opcodes.py` & `py-evm-0.7.0a3/eth/vm/forks/spurious_dragon/opcodes.py`

 * *Files identical despite different names*

### Comparing `py-evm-0.7.0a2/eth/vm/forks/spurious_dragon/state.py` & `py-evm-0.7.0a3/eth/vm/forks/spurious_dragon/state.py`

 * *Files identical despite different names*

### Comparing `py-evm-0.7.0a2/eth/vm/forks/spurious_dragon/transactions.py` & `py-evm-0.7.0a3/eth/vm/forks/spurious_dragon/transactions.py`

 * *Files identical despite different names*

### Comparing `py-evm-0.7.0a2/eth/vm/forks/tangerine_whistle/opcodes.py` & `py-evm-0.7.0a3/eth/vm/forks/tangerine_whistle/opcodes.py`

 * *Files identical despite different names*

### Comparing `py-evm-0.7.0a2/eth/vm/gas_meter.py` & `py-evm-0.7.0a3/eth/vm/gas_meter.py`

 * *Files identical despite different names*

### Comparing `py-evm-0.7.0a2/eth/vm/header.py` & `py-evm-0.7.0a3/eth/vm/header.py`

 * *Files identical despite different names*

### Comparing `py-evm-0.7.0a2/eth/vm/interrupt.py` & `py-evm-0.7.0a3/eth/vm/interrupt.py`

 * *Files identical despite different names*

### Comparing `py-evm-0.7.0a2/eth/vm/logic/arithmetic.py` & `py-evm-0.7.0a3/eth/vm/logic/arithmetic.py`

 * *Files identical despite different names*

### Comparing `py-evm-0.7.0a2/eth/vm/logic/block.py` & `py-evm-0.7.0a3/eth/vm/logic/block.py`

 * *Files identical despite different names*

### Comparing `py-evm-0.7.0a2/eth/vm/logic/call.py` & `py-evm-0.7.0a3/eth/vm/logic/call.py`

 * *Files identical despite different names*

### Comparing `py-evm-0.7.0a2/eth/vm/logic/comparison.py` & `py-evm-0.7.0a3/eth/vm/logic/comparison.py`

 * *Files identical despite different names*

### Comparing `py-evm-0.7.0a2/eth/vm/logic/context.py` & `py-evm-0.7.0a3/eth/vm/logic/context.py`

 * *Files identical despite different names*

### Comparing `py-evm-0.7.0a2/eth/vm/logic/duplication.py` & `py-evm-0.7.0a3/eth/vm/logic/duplication.py`

 * *Files identical despite different names*

### Comparing `py-evm-0.7.0a2/eth/vm/logic/flow.py` & `py-evm-0.7.0a3/eth/vm/logic/flow.py`

 * *Files identical despite different names*

### Comparing `py-evm-0.7.0a2/eth/vm/logic/logging.py` & `py-evm-0.7.0a3/eth/vm/logic/logging.py`

 * *Files identical despite different names*

### Comparing `py-evm-0.7.0a2/eth/vm/logic/memory.py` & `py-evm-0.7.0a3/eth/vm/logic/memory.py`

 * *Files identical despite different names*

### Comparing `py-evm-0.7.0a2/eth/vm/logic/sha3.py` & `py-evm-0.7.0a3/eth/vm/logic/sha3.py`

 * *Files identical despite different names*

### Comparing `py-evm-0.7.0a2/eth/vm/logic/stack.py` & `py-evm-0.7.0a3/eth/vm/logic/stack.py`

 * *Files identical despite different names*

### Comparing `py-evm-0.7.0a2/eth/vm/logic/storage.py` & `py-evm-0.7.0a3/eth/vm/logic/storage.py`

 * *Files identical despite different names*

### Comparing `py-evm-0.7.0a2/eth/vm/logic/swap.py` & `py-evm-0.7.0a3/eth/vm/logic/swap.py`

 * *Files identical despite different names*

### Comparing `py-evm-0.7.0a2/eth/vm/logic/system.py` & `py-evm-0.7.0a3/eth/vm/logic/system.py`

 * *Files 4% similar despite different names*

```diff
@@ -155,35 +155,34 @@
         stack_data = self.get_stack_data(computation)
 
         gas_cost = self.get_gas_cost(stack_data)
         computation.consume_gas(gas_cost, reason=self.mnemonic)
 
         computation.extend_memory(stack_data.memory_start, stack_data.memory_length)
 
-        storage_address_balance = computation.state.get_balance(
-            computation.msg.storage_address
-        )
+        storage_address = computation.msg.storage_address
+        storage_address_balance = computation.state.get_balance(storage_address)
+        storage_address_nonce = computation.state.get_nonce(storage_address)
 
         insufficient_funds = storage_address_balance < stack_data.endowment
         stack_too_deep = computation.msg.depth + 1 > constants.STACK_DEPTH_LIMIT
+        nonce_too_high = storage_address_nonce + 1 > constants.UINT_64_MAX
 
-        if insufficient_funds or stack_too_deep:
+        if insufficient_funds or stack_too_deep or nonce_too_high:
             computation.stack_push_int(0)
             computation.return_data = b""
             if insufficient_funds:
                 self.logger.debug2(
-                    "%s failure: %s",
-                    self.mnemonic,
-                    f"Insufficient Funds: {storage_address_balance} < "
-                    f"{stack_data.endowment}",
+                    f"{self.mnemonic} failure: Insufficient Funds: "
+                    f"{storage_address_balance} < {stack_data.endowment}",
                 )
             elif stack_too_deep:
-                self.logger.debug2(
-                    "%s failure: %s", self.mnemonic, "Stack limit reached"
-                )
+                self.logger.debug2(f"{self.mnemonic} failure: Stack limit reached")
+            elif nonce_too_high:
+                self.logger.debug2(f"{self.mnemonic} failure: Nonce too high")
             else:
                 raise RuntimeError(
                     "Invariant: error must be insufficient funds or stack too deep"
                 )
             return
 
         call_data = computation.memory_read_bytes(
```

### Comparing `py-evm-0.7.0a2/eth/vm/memory.py` & `py-evm-0.7.0a3/eth/vm/memory.py`

 * *Files identical despite different names*

### Comparing `py-evm-0.7.0a2/eth/vm/message.py` & `py-evm-0.7.0a3/eth/vm/message.py`

 * *Files identical despite different names*

### Comparing `py-evm-0.7.0a2/eth/vm/mnemonics.py` & `py-evm-0.7.0a3/eth/vm/mnemonics.py`

 * *Files identical despite different names*

### Comparing `py-evm-0.7.0a2/eth/vm/opcode.py` & `py-evm-0.7.0a3/eth/vm/opcode.py`

 * *Files identical despite different names*

### Comparing `py-evm-0.7.0a2/eth/vm/opcode_values.py` & `py-evm-0.7.0a3/eth/vm/opcode_values.py`

 * *Files identical despite different names*

### Comparing `py-evm-0.7.0a2/eth/vm/stack.py` & `py-evm-0.7.0a3/eth/vm/stack.py`

 * *Files identical despite different names*

### Comparing `py-evm-0.7.0a2/eth/vm/state.py` & `py-evm-0.7.0a3/eth/vm/state.py`

 * *Files identical despite different names*

### Comparing `py-evm-0.7.0a2/eth/vm/transaction_context.py` & `py-evm-0.7.0a3/eth/vm/transaction_context.py`

 * *Files identical despite different names*

### Comparing `py-evm-0.7.0a2/py_evm.egg-info/PKG-INFO` & `py-evm-0.7.0a3/py_evm.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py-evm
-Version: 0.7.0a2
+Version: 0.7.0a3
 Summary: Python implementation of the Ethereum Virtual Machine
 Home-page: https://github.com/ethereum/py-evm
 Author: Ethereum Foundation
 Author-email: piper@pipermerriam.com
 License: MIT
 Keywords: ethereum blockchain evm
 Classifier: Development Status :: 3 - Alpha
@@ -16,15 +16,15 @@
 Classifier: Programming Language :: Python :: 3.9
 Description-Content-Type: text/markdown
 Provides-Extra: eth
 Provides-Extra: eth-extra
 Provides-Extra: test
 Provides-Extra: lint
 Provides-Extra: benchmark
-Provides-Extra: doc
+Provides-Extra: docs
 Provides-Extra: dev
 License-File: LICENSE
 
 # Python Implementation of the Ethereum protocol
 
 [![Join the conversation on Discord](https://img.shields.io/discord/809793915578089484?color=blue&label=chat&logo=discord&logoColor=white)](https://discord.gg/GHryRvPB84)
 [![Build Status](https://circleci.com/gh/ethereum/py-evm.svg?style=shield)](https://circleci.com/gh/ethereum/py-evm)
```

### Comparing `py-evm-0.7.0a2/py_evm.egg-info/SOURCES.txt` & `py-evm-0.7.0a3/py_evm.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `py-evm-0.7.0a2/py_evm.egg-info/requires.txt` & `py-evm-0.7.0a3/py_evm.egg-info/requires.txt`

 * *Files 10% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 
 [dev]
 bumpversion<1,>=0.5.3
 wheel
 setuptools>=36.2.0
 idna==2.7
 requests<3,>=2.20
-tox==2.7.0
+tox>=4.0.0
 twine
 cached-property<2,>=1.5.1
 eth-bloom>=1.0.3
 eth-keys<0.5.0,>=0.4.0
 eth-typing<4.0.0,>=3.3.0
 eth-utils<3.0.0,>=2.0.0
 lru-dict>=1.1.6
@@ -38,33 +38,33 @@
 pexpect<5,>=4.6
 pytest<7,>=6.2.4
 pytest-asyncio<0.11,>=0.10.0
 pytest-cov==2.5.1
 pytest-timeout<2,>=1.4.2
 pytest-watch<5,>=4.1.0
 pytest-xdist==2.3.0
+flake8==6.0.0
+flake8-bugbear==23.3.23
+isort>=5.10.1
+mypy==0.971
+pydocstyle>=6.0.0
+black>=23
+types-setuptools
 py-evm>=0.2.0-a.14
 pysha3<2.0.0,>=1.0.0
 Sphinx<2,>=1.5.5
 jinja2<3.1.0,>=3.0.0
 sphinx_rtd_theme>=0.1.9
 sphinxcontrib-asyncio<0.4,>=0.2.0
 towncrier<22,>=21
-flake8==3.8.2
-flake8-bugbear==20.1.4
-isort>=5.10.1
-mypy==0.910
-pydocstyle>=6.0.0
-black>=23
-types-setuptools
 
 [dev:python_version < "3.8"]
 importlib-metadata<5.0
 
-[doc]
+[docs]
 py-evm>=0.2.0-a.14
 pysha3<2.0.0,>=1.0.0
 Sphinx<2,>=1.5.5
 jinja2<3.1.0,>=3.0.0
 sphinx_rtd_theme>=0.1.9
 sphinxcontrib-asyncio<0.4,>=0.2.0
 towncrier<22,>=21
@@ -90,18 +90,18 @@
 [eth-extra:implementation_name == "cpython"]
 eth-hash[pysha3]
 
 [eth-extra:implementation_name == "pypy"]
 eth-hash[pycryptodome]
 
 [lint]
-flake8==3.8.2
-flake8-bugbear==20.1.4
+flake8==6.0.0
+flake8-bugbear==23.3.23
 isort>=5.10.1
-mypy==0.910
+mypy==0.971
 pydocstyle>=6.0.0
 black>=23
 types-setuptools
 
 [lint:python_version < "3.8"]
 importlib-metadata<5.0
```

### Comparing `py-evm-0.7.0a2/pyproject.toml` & `py-evm-0.7.0a3/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 [[tool.towncrier.type]]
 directory = "performance"
 name = "Performance improvements"
 showcontent = true
 
 [[tool.towncrier.type]]
-directory = "doc"
+directory = "docs"
 name = "Improved Documentation"
 showcontent = true
 
 [[tool.towncrier.type]]
 directory = "removal"
 name = "Deprecations and Removals"
 showcontent = true
```

### Comparing `py-evm-0.7.0a2/setup.py` & `py-evm-0.7.0a3/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,13 +1,16 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
-from setuptools import setup, find_packages
+from setuptools import (
+    setup,
+    find_packages,
+)
 
 
-deps = {
+extras_require = {
     "eth": [
         "cached-property>=1.5.1,<2",
         "eth-bloom>=1.0.3",
         "eth-keys>=0.4.0,<0.5.0",
         "eth-typing>=3.3.0,<4.0.0",
         "eth-utils>=2.0.0,<3.0.0",
         "lru-dict>=1.1.6",
@@ -37,28 +40,28 @@
         "pytest-cov==2.5.1",
         "pytest-timeout>=1.4.2,<2",
         "pytest-watch>=4.1.0,<5",
         "pytest-xdist==2.3.0",
         "importlib-metadata<5.0;python_version<'3.8'",
     ],
     "lint": [
-        "flake8==3.8.2",
-        "flake8-bugbear==20.1.4",
+        "flake8==6.0.0",  # flake8 claims semver but adds new warnings at minor releases, leave it pinned.
+        "flake8-bugbear==23.3.23",  # flake8-bugbear does not follow semver, leave it pinned.
         "isort>=5.10.1",
-        "mypy==0.910",
+        "mypy==0.971",  # mypy does not follow semver, leave it pinned.
         "pydocstyle>=6.0.0",
         "black>=23",
         "types-setuptools",
         "importlib-metadata<5.0;python_version<'3.8'",
     ],
     "benchmark": [
         "termcolor>=1.1.0,<2.0.0",
         "web3>=4.1.0,<5.0.0",
     ],
-    "doc": [
+    "docs": [
         "py-evm>=0.2.0-a.14",
         # We need to have pysha for autodoc to be able to extract API docs
         "pysha3>=1.0.0,<2.0.0",
         "Sphinx>=1.5.5,<2",
         "jinja2>=3.0.0,<3.1.0",  # jinja2<3.0 or >=3.1.0 cause doc build failures.
         "sphinx_rtd_theme>=0.1.9",
         "sphinxcontrib-asyncio>=0.2.0,<0.4",
@@ -69,42 +72,47 @@
         "wheel",
         "setuptools>=36.2.0",
         # Fixing this dependency due to: requests 2.20.1 has requirement
         # idna<2.8,>=2.5, but you'll have idna 2.8 which is incompatible.
         "idna==2.7",
         # idna 2.7 is not supported by requests 2.18
         "requests>=2.20,<3",
-        "tox==2.7.0",
+        "tox>=4.0.0",
         "twine",
     ],
 }
 
 
-deps["dev"] = deps["dev"] + deps["eth"] + deps["test"] + deps["doc"] + deps["lint"]
+extras_require["dev"] = (
+    extras_require["dev"]
+    + extras_require["eth"]
+    + extras_require["test"]
+    + extras_require["lint"]
+    + extras_require["docs"]
+)
 
-
-install_requires = deps["eth"]
+install_requires = extras_require["eth"]
 
 with open("README.md") as readme_file:
     long_description = readme_file.read()
 
 setup(
     name="py-evm",
     # *IMPORTANT*: Don't manually change the version here. Use the 'bumpversion' utility.
-    version="0.7.0-alpha.2",
+    version="0.7.0-alpha.3",
     description="Python implementation of the Ethereum Virtual Machine",
     long_description=long_description,
     long_description_content_type="text/markdown",
     author="Ethereum Foundation",
     author_email="piper@pipermerriam.com",
     url="https://github.com/ethereum/py-evm",
     include_package_data=True,
     py_modules=["eth"],
     install_requires=install_requires,
-    extras_require=deps,
+    extras_require=extras_require,
     license="MIT",
     zip_safe=False,
     keywords="ethereum blockchain evm",
     packages=find_packages(exclude=["tests", "tests.*"]),
     package_data={"eth": ["py.typed"]},
     classifiers=[
         "Development Status :: 3 - Alpha",
```

