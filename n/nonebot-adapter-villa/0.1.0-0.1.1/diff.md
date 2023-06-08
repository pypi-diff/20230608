# Comparing `tmp/nonebot_adapter_villa-0.1.0.tar.gz` & `tmp/nonebot_adapter_villa-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_adapter_villa-0.1.0.tar", max compression
+gzip compressed data, was "nonebot_adapter_villa-0.1.1.tar", max compression
```

## Comparing `nonebot_adapter_villa-0.1.0.tar` & `nonebot_adapter_villa-0.1.1.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0     1062 2023-06-06 16:03:40.605749 nonebot_adapter_villa-0.1.0/LICENSE
--rw-r--r--   0        0        0     4382 2023-06-06 16:03:40.605749 nonebot_adapter_villa-0.1.0/README.md
--rw-r--r--   0        0        0      235 2023-06-06 16:03:40.609750 nonebot_adapter_villa-0.1.0/nonebot/adapters/villa/__init__.py
--rw-r--r--   0        0        0     4618 2023-06-06 16:03:40.609750 nonebot_adapter_villa-0.1.0/nonebot/adapters/villa/adapter.py
--rw-r--r--   0        0        0      114 2023-06-06 16:03:40.609750 nonebot_adapter_villa-0.1.0/nonebot/adapters/villa/api/__init__.py
--rw-r--r--   0        0        0     3247 2023-06-06 16:03:40.609750 nonebot_adapter_villa-0.1.0/nonebot/adapters/villa/api/cilent.pyi
--rw-r--r--   0        0        0     4109 2023-06-06 16:03:40.609750 nonebot_adapter_villa-0.1.0/nonebot/adapters/villa/api/client.py
--rw-r--r--   0        0        0    13301 2023-06-06 16:03:40.609750 nonebot_adapter_villa-0.1.0/nonebot/adapters/villa/api/handle.py
--rw-r--r--   0        0        0     9012 2023-06-06 16:03:40.609750 nonebot_adapter_villa-0.1.0/nonebot/adapters/villa/api/models.py
--rw-r--r--   0        0        0     1514 2023-06-06 16:03:40.609750 nonebot_adapter_villa-0.1.0/nonebot/adapters/villa/api/request.py
--rw-r--r--   0        0        0    10579 2023-06-06 16:03:40.609750 nonebot_adapter_villa-0.1.0/nonebot/adapters/villa/bot.py
--rw-r--r--   0        0        0      263 2023-06-06 16:03:40.609750 nonebot_adapter_villa-0.1.0/nonebot/adapters/villa/config.py
--rw-r--r--   0        0        0     6267 2023-06-06 16:03:40.609750 nonebot_adapter_villa-0.1.0/nonebot/adapters/villa/event.py
--rw-r--r--   0        0        0     1755 2023-06-06 16:03:40.609750 nonebot_adapter_villa-0.1.0/nonebot/adapters/villa/exception.py
--rw-r--r--   0        0        0     8178 2023-06-06 16:03:40.609750 nonebot_adapter_villa-0.1.0/nonebot/adapters/villa/message.py
--rw-r--r--   0        0        0       76 2023-06-06 16:03:40.609750 nonebot_adapter_villa-0.1.0/nonebot/adapters/villa/utils.py
--rw-r--r--   0        0        0     1134 2023-06-06 16:03:40.609750 nonebot_adapter_villa-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     5283 1970-01-01 00:00:00.000000 nonebot_adapter_villa-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1062 2023-06-08 14:18:01.982057 nonebot_adapter_villa-0.1.1/LICENSE
+-rw-r--r--   0        0        0     4154 2023-06-08 14:18:01.982057 nonebot_adapter_villa-0.1.1/README.md
+-rw-r--r--   0        0        0      235 2023-06-08 14:18:01.982057 nonebot_adapter_villa-0.1.1/nonebot/adapters/villa/__init__.py
+-rw-r--r--   0        0        0     4668 2023-06-08 14:18:01.982057 nonebot_adapter_villa-0.1.1/nonebot/adapters/villa/adapter.py
+-rw-r--r--   0        0        0      114 2023-06-08 14:18:01.982057 nonebot_adapter_villa-0.1.1/nonebot/adapters/villa/api/__init__.py
+-rw-r--r--   0        0        0     3247 2023-06-08 14:18:01.982057 nonebot_adapter_villa-0.1.1/nonebot/adapters/villa/api/cilent.pyi
+-rw-r--r--   0        0        0     4109 2023-06-08 14:18:01.982057 nonebot_adapter_villa-0.1.1/nonebot/adapters/villa/api/client.py
+-rw-r--r--   0        0        0    13301 2023-06-08 14:18:01.982057 nonebot_adapter_villa-0.1.1/nonebot/adapters/villa/api/handle.py
+-rw-r--r--   0        0        0     9952 2023-06-08 14:18:01.982057 nonebot_adapter_villa-0.1.1/nonebot/adapters/villa/api/models.py
+-rw-r--r--   0        0        0     1514 2023-06-08 14:18:01.982057 nonebot_adapter_villa-0.1.1/nonebot/adapters/villa/api/request.py
+-rw-r--r--   0        0        0    11111 2023-06-08 14:18:01.986057 nonebot_adapter_villa-0.1.1/nonebot/adapters/villa/bot.py
+-rw-r--r--   0        0        0      263 2023-06-08 14:18:01.986057 nonebot_adapter_villa-0.1.1/nonebot/adapters/villa/config.py
+-rw-r--r--   0        0        0     8936 2023-06-08 14:18:01.986057 nonebot_adapter_villa-0.1.1/nonebot/adapters/villa/event.py
+-rw-r--r--   0        0        0     1755 2023-06-08 14:18:01.986057 nonebot_adapter_villa-0.1.1/nonebot/adapters/villa/exception.py
+-rw-r--r--   0        0        0     6279 2023-06-08 14:18:01.986057 nonebot_adapter_villa-0.1.1/nonebot/adapters/villa/message.py
+-rw-r--r--   0        0        0       76 2023-06-08 14:18:01.986057 nonebot_adapter_villa-0.1.1/nonebot/adapters/villa/utils.py
+-rw-r--r--   0        0        0     1134 2023-06-08 14:18:01.986057 nonebot_adapter_villa-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     5055 1970-01-01 00:00:00.000000 nonebot_adapter_villa-0.1.1/PKG-INFO
```

### Comparing `nonebot_adapter_villa-0.1.0/LICENSE` & `nonebot_adapter_villa-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_adapter_villa-0.1.0/README.md` & `nonebot_adapter_villa-0.1.1/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -32,243 +32,229 @@
 000001f0: 7470 733a 2f2f 696d 672e 7368 6965 6c64  tps://img.shield
 00000200: 732e 696f 2f67 6974 6875 622f 6c69 6365  s.io/github/lice
 00000210: 6e73 652f 434d 486f 7065 5375 6e73 6869  nse/CMHopeSunshi
 00000220: 6e65 2f6e 6f6e 6562 6f74 2d61 6461 7074  ne/nonebot-adapt
 00000230: 6572 2d76 696c 6c61 2220 616c 743d 226c  er-villa" alt="l
 00000240: 6963 656e 7365 223e 3c2f 613e 0a0a 3c2f  icense"></a>..</
 00000250: 6469 763e 0a0a 2323 20e5 ae89 e8a3 850a  div>..## .......
-00000260: 0a2d 20e5 9ca8 604e 6f6e 6542 6f74 3260  .- ...`NoneBot2`
-00000270: e9a1 b9e7 9bae e79b aee5 bd95 e4b8 8be4  ................
-00000280: bdbf e794 a8e8 849a e689 8be6 9eb6 e5ae  ................
-00000290: 89e8 a385 efbc 9a60 6e62 2061 6461 7074  .......`nb adapt
-000002a0: 6572 2069 6e73 7461 6c6c 206e 6f6e 6562  er install noneb
-000002b0: 6f74 2d61 6461 7074 6572 2d76 696c 6c61  ot-adapter-villa
-000002c0: 600a 2020 0ae6 8896 efbc 9a0a 0a2d 20e5  `.  .........- .
-000002d0: 9ca8 604e 6f6e 6542 6f74 3260 e9a1 b9e7  ..`NoneBot2`....
-000002e0: 9bae e78e afe5 a283 e4b8 8be4 bdbf e794  ................
-000002f0: a870 6970 e5ae 89e8 a385 e590 8ee6 898b  .pip............
-00000300: e58a a8e6 b3a8 e586 8cef bc9a 6070 6970  ............`pip
-00000310: 2069 6e73 7461 6c6c 206e 6f6e 6562 6f74   install nonebot
-00000320: 2d61 6461 7074 6572 2d76 696c 6c61 600a  -adapter-villa`.
-00000330: 0a23 2320 e985 8de7 bdae 0a0a e4bf aee6  .## ............
-00000340: 94b9 204e 6f6e 6542 6f74 20e9 858d e7bd  .. NoneBot .....
-00000350: aee6 9687 e4bb b620 602e 656e 7660 20e6  ....... `.env` .
-00000360: 8896 e880 8520 602e 656e 762e 2a60 e380  ..... `.env.*`..
-00000370: 820a 0a23 2323 2044 7269 7665 720a 0ae6  ...### Driver...
-00000380: 9cac e980 82e9 858d e599 a8e5 908c e697  ................
-00000390: b6e9 9c80 e8a6 8160 5265 7665 7273 6544  .......`ReverseD
-000003a0: 7269 7665 7260 e592 8c60 466f 7277 6172  river`...`Forwar
-000003b0: 6444 7269 7665 7260 efbc 8ce5 8f82 e880  dDriver`........
-000003c0: 8320 5b64 7269 7665 725d 2868 7474 7073  . [driver](https
-000003d0: 3a2f 2f76 322e 6e6f 6e65 626f 742e 6465  ://v2.nonebot.de
-000003e0: 762f 646f 6373 2f6e 6578 742f 6164 7661  v/docs/next/adva
-000003f0: 6e63 6564 2f64 7269 7665 7223 2545 3925  nced/driver#%E9%
-00000400: 4139 2542 3125 4535 2538 4125 4138 2545  A9%B1%E5%8A%A8%E
-00000410: 3525 3939 2541 3825 4537 2542 3125 4242  5%99%A8%E7%B1%BB
-00000420: 2545 3525 3945 2538 4229 20e9 858d e7bd  %E5%9E%8B) .....
-00000430: aee9 a1b9 e380 820a 0ae4 be8b e5a6 82ef  ................
-00000440: bc9a 0a0a 6060 6064 6f74 656e 760a 4452  ....```dotenv.DR
-00000450: 4956 4552 3d7e 6661 7374 6170 692b 7e68  IVER=~fastapi+~h
-00000460: 7474 7078 0a60 6060 0a0a 2323 2320 5649  ttpx.```..### VI
-00000470: 4c4c 415f 424f 5453 0a0a e985 8de7 bdae  LLA_BOTS........
-00000480: e69c bae5 99a8 e4ba bae5 b890 e58f b7e5  ................
-00000490: 8897 e8a1 a8ef bc8c e6af 8fe4 b8aa 626f  ..............bo
-000004a0: 74e6 9c89 33e4 b8aa e5bf 85e5 a1ab e985  t...3...........
-000004b0: 8de7 bdae efbc 8ce5 9ca8 e5a4 a7e5 88ab  ................
-000004c0: e987 8ee6 9cba e599 a8e4 baba e5bc 80e5  ................
-000004d0: 8f91 e880 85e7 a4be e58c bae7 94b3 e8af  ................
-000004e0: b7e6 97b6 e88e b7e5 be97 efbc 8c0a 0a2d  ...............-
-000004f0: 2062 6f74 5f69 643a 20e6 9cba e599 a8e4   bot_id: .......
-00000500: baba 6964 efbc 8ce4 bba5 6062 6f74 5f60  ..id......`bot_`
-00000510: e5bc 80e5 a4b4 0a2d 2062 6f74 5f73 6563  .......- bot_sec
-00000520: 7265 743a 20e6 9cba e599 a8e4 baba e5af  ret: ...........
-00000530: 86e9 92a5 0a2d 2063 616c 6c62 6163 6b5f  .....- callback_
-00000540: 7572 6c3a 2068 7474 70e5 9b9e e8b0 83e5  url: http.......
-00000550: 9cb0 e59d 80ef bc8c e4be 8be5 a682 e794  ................
-00000560: b3e8 afb7 626f 74e6 97b6 e7bb 99e7 9a84  ....bot.........
-00000570: e59b 9ee8 b083 e59c b0e5 9d80 e698 af60  ...............`
-00000580: 6874 7470 3a2f 2fe5 9f9f e590 8d2f 796f  http://....../yo
-00000590: 7572 2f63 616c 6c62 6163 6b2f 7572 6c60  ur/callback/url`
-000005a0: efbc 8ce9 82a3 e4b9 88e9 858d e7bd aee9  ................
-000005b0: 878c e79a 8460 6361 6c6c 6261 636b 5f75  .....`callback_u
-000005c0: 726c 60e5 a1ab e586 9960 2f79 6f75 722f  rl`......`/your/
-000005d0: 6361 6c6c 6261 636b 2f75 726c 600a 2020  callback/url`.  
-000005e0: e4be 8be5 a682 efbc 9a0a 0a60 6060 646f  ...........```do
-000005f0: 7465 6e76 0a56 494c 4c41 5f42 4f54 533d  tenv.VILLA_BOTS=
-00000600: 270a 5b0a 2020 7b0a 2020 2020 2262 6f74  '.[.  {.    "bot
-00000610: 5f69 6422 3a20 2262 6f74 5f31 3233 3435  _id": "bot_12345
-00000620: 3637 3839 222c 0a20 2020 2022 626f 745f  6789",.    "bot_
-00000630: 7365 6372 6574 223a 2022 6162 6331 3233  secret": "abc123
-00000640: 6465 6634 3536 222c 0a20 2020 2022 6361  def456",.    "ca
-00000650: 6c6c 6261 636b 5f75 726c 223a 2022 2f79  llback_url": "/y
-00000660: 6f75 722f 6361 6c6c 6261 636b 2f75 726c  our/callback/url
-00000670: 220a 2020 7d0a 5d0a 270a 6060 600a 0a23  ".  }.].'.```..#
-00000680: 2320 e4bd bfe7 94a8 0a0a 2323 2320 e6b3  # ........### ..
-00000690: a8e5 868c e980 82e9 858d e599 a80a 0a3e  ...............>
-000006a0: 20e5 a682 e4bd bfe7 94a8 6e62 e884 9ae6   .........nb....
-000006b0: 898b e69e b6e6 9da5 e5ae 89e8 a385 e79a  ................
-000006c0: 84ef bc8c e588 99e4 b88d e794 a8e6 898b  ................
-000006d0: e58a a8e6 b3a8 e586 8c0a 0ae5 9ca8 6062  ..............`b
-000006e0: 6f74 2e70 7960 e696 87e4 bbb6 e4b8 ad28  ot.py`.........(
-000006f0: e5a6 82e6 9e9c e6b2 a1e6 9c89 efbc 8ce4  ................
-00000700: bdbf e794 a860 6e62 2067 656e 6572 6174  .....`nb generat
-00000710: 6560 e69d a5e7 949f e688 9029 e6b3 a8e5  e`.........)....
-00000720: 868c e69c ace9 8082 e985 8de5 99a8 efbc  ................
-00000730: 8ce5 8f82 e880 835b 6164 6170 7465 725d  .......[adapter]
-00000740: 2868 7474 7073 3a2f 2f76 322e 6e6f 6e65  (https://v2.none
-00000750: 626f 742e 6465 762f 646f 6373 2f61 6476  bot.dev/docs/adv
-00000760: 616e 6365 642f 6164 6170 7465 7229 efbc  anced/adapter)..
-00000770: 8ce4 be8b e5a6 82ef bc9a 0a0a 6060 6070  ............```p
-00000780: 7974 686f 6e0a 696d 706f 7274 206e 6f6e  ython.import non
-00000790: 6562 6f74 0a66 726f 6d20 6e6f 6e65 626f  ebot.from nonebo
-000007a0: 742e 6164 6170 7465 7273 2e76 696c 6c61  t.adapters.villa
-000007b0: 2069 6d70 6f72 7420 4164 6170 7465 7220   import Adapter 
-000007c0: 6173 2056 696c 6c61 4164 6170 7465 7220  as VillaAdapter 
-000007d0: 2023 20e5 afbc e585 a561 6461 7074 6572   # ......adapter
-000007e0: 0a0a 6e6f 6e65 626f 742e 696e 6974 2829  ..nonebot.init()
-000007f0: 0a0a 6472 6976 6572 203d 206e 6f6e 6562  ..driver = noneb
-00000800: 6f74 2e67 6574 5f64 7269 7665 7228 290a  ot.get_driver().
-00000810: 6472 6976 6572 2e72 6567 6973 7465 725f  driver.register_
-00000820: 6164 6170 7465 7228 5669 6c6c 6141 6461  adapter(VillaAda
-00000830: 7074 6572 2920 2320 e6b3 a8e5 868c 6164  pter) # ......ad
-00000840: 6170 7465 720a 0a6e 6f6e 6562 6f74 2e6c  apter..nonebot.l
-00000850: 6f61 645f 6672 6f6d 5f74 6f6d 6c28 2270  oad_from_toml("p
-00000860: 7970 726f 6a65 6374 2e74 6f6d 6c22 290a  yproject.toml").
-00000870: 0a69 6620 5f5f 6e61 6d65 5f5f 203d 3d20  .if __name__ == 
-00000880: 225f 5f6d 6169 6e5f 5f22 3a0a 2020 2020  "__main__":.    
-00000890: 6e6f 6e65 626f 742e 7275 6e28 290a 6060  nonebot.run().``
-000008a0: 600a 0a23 2323 20e6 b688 e681 afe6 aeb5  `..### .........
-000008b0: e5b1 95e7 a4ba 0a0a e4bb a5e4 b88b e698  ................
-000008c0: afe4 b880 e4b8 aae7 ae80 e58d 95e7 9a84  ................
-000008d0: e68f 92e4 bbb6 e7a4 bae4 be8b efbc 8ce5  ................
-000008e0: b195 e7a4 bae5 9084 e7a7 8de6 b688 e681  ................
-000008f0: afe6 aeb5 efbc 9a0a 0a60 6060 7079 7468  .........```pyth
-00000900: 6f6e 0a66 726f 6d20 6e6f 6e65 626f 7420  on.from nonebot 
-00000910: 696d 706f 7274 206f 6e5f 636f 6d6d 616e  import on_comman
-00000920: 640a 6672 6f6d 206e 6f6e 6562 6f74 2e70  d.from nonebot.p
-00000930: 6172 616d 7320 696d 706f 7274 2043 6f6d  arams import Com
-00000940: 6d61 6e64 4172 670a 0a66 726f 6d20 6e6f  mandArg..from no
-00000950: 6e65 626f 742e 6164 6170 7465 7273 2e76  nebot.adapters.v
-00000960: 696c 6c61 2069 6d70 6f72 7420 426f 742c  illa import Bot,
-00000970: 2053 656e 644d 6573 7361 6765 4576 656e   SendMessageEven
-00000980: 742c 204d 6573 7361 6765 2c20 4d65 7373  t, Message, Mess
-00000990: 6167 6553 6567 6d65 6e74 0a0a 6d61 7463  ageSegment..matc
-000009a0: 6865 7220 3d20 6f6e 5f63 6f6d 6d61 6e64  her = on_command
-000009b0: 2827 e58f 91e9 8081 2729 0a0a 406d 6174  ('......')..@mat
-000009c0: 6368 6572 2e68 616e 646c 6528 290a 6173  cher.handle().as
-000009d0: 796e 6320 6465 6620 6d61 7463 6865 725f  ync def matcher_
-000009e0: 6861 6e64 6c65 7228 626f 743a 2042 6f74  handler(bot: Bot
-000009f0: 2c20 6576 656e 743a 2053 656e 644d 6573  , event: SendMes
-00000a00: 7361 6765 4576 656e 742c 2063 6d64 5f61  sageEvent, cmd_a
-00000a10: 7267 3a20 4d65 7373 6167 6520 3d20 436f  rg: Message = Co
-00000a20: 6d6d 616e 6441 7267 2829 293a 0a20 2020  mmandArg()):.   
-00000a30: 206d 7367 203d 204d 6573 7361 6765 2829   msg = Message()
-00000a40: 0a20 2020 2061 7267 7320 3d20 636d 645f  .    args = cmd_
-00000a50: 6172 672e 6578 7472 6163 745f 706c 6169  arg.extract_plai
-00000a60: 6e5f 7465 7874 2829 2e73 7472 6970 2829  n_text().strip()
-00000a70: 2e73 706c 6974 2827 2027 290a 2020 2020  .split(' ').    
-00000a80: 666f 7220 6172 6720 696e 2061 7267 733a  for arg in args:
-00000a90: 0a20 2020 2020 2020 2069 6620 6172 6720  .        if arg 
-00000aa0: 3d3d 2022 e889 bee7 89b9 e688 9122 3a0a  == ".........":.
-00000ab0: 2020 2020 2020 2020 2020 2020 6d73 6720              msg 
-00000ac0: 2b3d 204d 6573 7361 6765 5365 676d 656e  += MessageSegmen
-00000ad0: 742e 6d65 6e74 696f 6e5f 7573 6572 2865  t.mention_user(e
-00000ae0: 7665 6e74 2e76 696c 6c61 5f69 642c 2065  vent.villa_id, e
-00000af0: 7665 6e74 2e66 726f 6d5f 7573 6572 5f69  vent.from_user_i
-00000b00: 6429 0a20 2020 2020 2020 2065 6c69 6620  d).        elif 
-00000b10: 6172 6720 3d3d 2022 e889 bee7 89b9 626f  arg == "......bo
-00000b20: 7422 3a0a 2020 2020 2020 2020 2020 2020  t":.            
-00000b30: 6d73 6720 2b3d 204d 6573 7361 6765 5365  msg += MessageSe
-00000b40: 676d 656e 742e 6d65 6e74 696f 6e5f 726f  gment.mention_ro
-00000b50: 626f 7428 290a 2020 2020 2020 2020 2020  bot().          
-00000b60: 2020 2320 e79b aee5 898d e58f aae8 83bd    # ............
-00000b70: e889 bee7 89b9 e69c bae5 99a8 e4ba bae8  ................
-00000b80: 87aa e5b7 b10a 2020 2020 2020 2020 656c  ......        el
-00000b90: 6966 2061 7267 203d 3d20 22e6 9687 e5ad  if arg == ".....
-00000ba0: 9722 3a0a 2020 2020 2020 2020 2020 2020  .":.            
-00000bb0: 6d73 6720 2b3d 204d 6573 7361 6765 5365  msg += MessageSe
-00000bc0: 676d 656e 742e 7465 7874 2822 e696 87e5  gment.text("....
-00000bd0: ad97 2229 0a20 2020 2020 2020 2020 2020  ..").           
-00000be0: 2023 20e8 a1a8 e683 85e4 b99f e698 afe7   # .............
-00000bf0: 94a8 7465 7874 e69d a5e5 8f91 e980 81ef  ..text..........
-00000c00: bc8c e4bb a55b e8a1 a8e6 8385 e590 8d5d  .....[.........]
-00000c10: e6a0 bce5 bc8f efbc 8ce4 be8b e5a6 824d  ...............M
-00000c20: 6573 7361 6765 5365 676d 656e 742e 7465  essageSegment.te
-00000c30: 7874 2822 5be7 88b1 e5bf 835d 2229 0a20  xt("[......]"). 
-00000c40: 2020 2020 2020 2065 6c69 6620 6172 6720         elif arg 
-00000c50: 3d3d 2022 e688 bfe9 97b4 223a 0a20 2020  == "......":.   
-00000c60: 2020 2020 2020 2020 206d 7367 202b 3d20           msg += 
-00000c70: 4d65 7373 6167 6553 6567 6d65 6e74 2e76  MessageSegment.v
-00000c80: 696c 6c61 5f72 6f6f 6d5f 6c69 6e6b 2865  illa_room_link(e
-00000c90: 7665 6e74 2e76 696c 6c61 5f69 642c 2065  vent.villa_id, e
-00000ca0: 7665 6e74 2e72 6f6f 6d5f 6964 290a 2020  vent.room_id).  
-00000cb0: 2020 2020 2020 656c 6966 2061 7267 203d        elif arg =
-00000cc0: 3d20 22e9 93be e68e a522 3a0a 2020 2020  = "......":.    
-00000cd0: 2020 2020 2020 2020 6d73 6720 2b3d 204d          msg += M
-00000ce0: 6573 7361 6765 5365 676d 656e 742e 6c69  essageSegment.li
-00000cf0: 6e6b 2822 6874 7470 733a 2f2f 7777 772e  nk("https://www.
-00000d00: 6d69 796f 7573 6865 2e63 6f6d 2f79 732f  miyoushe.com/ys/
-00000d10: 6172 7469 636c 652f 3339 3637 3033 3037  article/39670307
-00000d20: 222c 2022 e8bf 99e6 98af e993 bee6 8ea5  ", "............
-00000d30: 2229 0a20 2020 2020 2020 2020 2020 2023  ").            #
-00000d40: 20e4 bdbf e794 a86c 696e 6be7 9a84 e8af   ......link.....
-00000d50: 9de9 93be e68e a5e8 83bd e5a4 9fe7 82b9  ................
-00000d60: e587 bbe8 bf9b e8a1 8ce8 b7b3 e8bd acef  ................
-00000d70: bc8c e4bd bfe7 94a8 7465 7874 e79a 84e8  ........text....
-00000d80: af9d e4b8 8de8 83bd e782 b9e5 87bb 0a20  ............... 
-00000d90: 2020 2020 2020 2065 6c69 6620 6172 6720         elif arg 
-00000da0: 3d3d 2022 e59b bee7 8987 223a 0a20 2020  == "......":.   
-00000db0: 2020 2020 2020 2020 206d 7367 202b 3d20           msg += 
-00000dc0: 4d65 7373 6167 6553 6567 6d65 6e74 2e69  MessageSegment.i
-00000dd0: 6d61 6765 2822 6874 7470 733a 2f2f 7777  mage("https://ww
-00000de0: 772e 6d69 796f 7573 6865 2e63 6f6d 2f5f  w.miyoushe.com/_
-00000df0: 6e75 7874 2f69 6d67 2f6d 6948 6f59 6f5f  nuxt/img/miHoYo_
-00000e00: 4761 6d65 2e32 3435 3737 3533 2e70 6e67  Game.2457753.png
-00000e10: 2229 0a20 2020 2020 2020 2020 2020 2023  ").            #
-00000e20: 20e6 9a82 e697 b6e5 8faa e694 afe6 8c81   ...............
-00000e30: 7572 6ce5 9bbe e789 870a 2020 2020 6177  url.......    aw
-00000e40: 6169 7420 6d61 7463 6865 722e 6669 6e69  ait matcher.fini
-00000e50: 7368 286d 7367 290a 6060 600a 0ae4 bdbf  sh(msg).```.....
-00000e60: e794 a8e5 91bd e4bb a460 4062 6f74 202f  .........`@bot /
-00000e70: e58f 91e9 8081 20e8 89be e789 b9e6 8891  ...... .........
-00000e80: 20e8 89be e789 b962 6f74 20e6 9687 e5ad   ......bot .....
-00000e90: 9720 e688 bfe9 97b4 20e9 93be e68e a520  . ...... ...... 
-00000ea0: e59b bee7 8987 60e6 97b6 efbc 8c62 6f74  ......`......bot
-00000eb0: e4bc 9ae5 9b9e e5a4 8d60 40e4 bda0 e79a  .........`@.....
-00000ec0: 84e5 908d e5ad 9720 4062 6f74 e79a 84e5  ....... @bot....
-00000ed0: 908d e5ad 9720 e696 87e5 ad97 2023 e688  ..... ...... #..
-00000ee0: bfe9 97b4 e590 8d20 e8bf 99e6 98af e993  ....... ........
-00000ef0: bee6 8ea5 20e5 9bbe e789 87e5 8685 e5ae  .... ...........
-00000f00: b960 0a0a 0a23 2320 e58f 8de9 a688 0a0a  .`...## ........
-00000f10: e79b aee5 898d e697 a0e8 aeba e698 afe5  ................
-00000f20: a4a7 e588 abe9 878e 426f 74e8 bf98 e698  ........Bot.....
-00000f30: afe6 9cac e980 82e9 858d e599 a8e9 83bd  ................
-00000f40: e59c a8e6 b58b e8af 95e5 bc80 e58f 91e4  ................
-00000f50: b8ad efbc 8ce5 a682 e981 87e9 97ae e9a2  ................
-00000f60: 98e8 afb7 e68f 90e5 87ba 6973 7375 65ef  ..........issue.
-00000f70: bc8c e684 9fe8 b0a2 e694 afe6 8c81 efbc  ................
-00000f80: 810a 0a23 2320 e79b b8e5 85b3 e9a1 b9e7  ...## ..........
-00000f90: 9bae 0a0a 2d20 5b4e 6f6e 6542 6f74 325d  ....- [NoneBot2]
-00000fa0: 2868 7474 7073 3a2f 2f67 6974 6875 622e  (https://github.
-00000fb0: 636f 6d2f 6e6f 6e65 626f 742f 6e6f 6e65  com/nonebot/none
-00000fc0: 626f 7432 2920 e99d 9ee5 b8b8 e5a5 bde7  bot2) ..........
-00000fd0: 94a8 e79a 8450 7974 686f 6ee8 b7a8 e5b9  .....Python.....
-00000fe0: b3e5 8fb0 e69c bae5 99a8 e4ba bae6 a186  ................
-00000ff0: e69e b6ef bc81 0a2d 205b 7669 6c6c 612d  .......- [villa-
-00001000: 7079 5d28 6874 7470 733a 2f2f 6769 7468  py](https://gith
-00001010: 7562 2e63 6f6d 2f43 4d48 6f70 6553 756e  ub.com/CMHopeSun
-00001020: 7368 696e 652f 7669 6c6c 612d 7079 2920  shine/villa-py) 
-00001030: e5a4 a7e5 88ab e987 8e42 6f74 2050 7974  .........Bot Pyt
-00001040: 686f 6e20 5344 4be3 8082 0a0a e68e a8e8  hon SDK.........
-00001050: 8d90 e69c 89e6 8890 e786 9f50 7974 686f  ...........Pytho
-00001060: 6ee5 bc80 e58f 91e7 bb8f e9aa 8ce4 bd86  n...............
-00001070: e5af b94e 6f6e 6542 6f74 32e4 b88d e786  ...NoneBot2.....
-00001080: 9fe6 8289 e79a 84e5 b08f e4bc 99e4 bcb4  ................
-00001090: e980 89e6 8ba9 60e5 a4a7 e588 abe9 878e  ......`.........
-000010a0: 426f 7420 5079 7468 6f6e 2053 444b 60ef  Bot Python SDK`.
-000010b0: bc8c 0a0a e5af b94e 6f6e 6542 6f74 32e7  .......NoneBot2.
-000010c0: 869f e682 89e6 8896 e5b8 8ce6 9c9b e68e  ................
-000010d0: a5e8 a7a6 e69b b4e6 8890 e786 9fe7 9a84  ................
-000010e0: e794 9fe6 8081 e79a 84e5 b08f e4bc 99e4  ................
-000010f0: bcb4 e980 89e6 8ba9 604e 6f6e 6542 6f74  ........`NoneBot
-00001100: 322b e69c ace9 8082 e985 8de5 99a8 60e8  2+............`.
-00001110: bf9b e8a1 8ce5 bc80 e58f 91e3 8082       ..............
+00000260: 0ae5 9ca8 604e 6f6e 6542 6f74 3260 e9a1  ....`NoneBot2`..
+00000270: b9e7 9bae e79b aee5 bd95 e4b8 8be4 bdbf  ................
+00000280: e794 a8e8 849a e689 8be6 9eb6 e5ae 89e8  ................
+00000290: a385 efbc 9a0a 0a60 6060 0a6e 6220 6164  .......```.nb ad
+000002a0: 6170 7465 7220 696e 7374 616c 6c20 6e6f  apter install no
+000002b0: 6e65 626f 742d 6164 6170 7465 722d 7669  nebot-adapter-vi
+000002c0: 6c6c 610a 6060 600a 0a23 2320 e985 8de7  lla.```..## ....
+000002d0: bdae 0a0a e4bf aee6 94b9 204e 6f6e 6542  .......... NoneB
+000002e0: 6f74 20e9 858d e7bd aee6 9687 e4bb b620  ot ............ 
+000002f0: 602e 656e 7660 20e6 8896 e880 8520 602e  `.env` ...... `.
+00000300: 656e 762e 2a60 e380 820a 0a23 2323 2044  env.*`.....### D
+00000310: 7269 7665 720a 0ae6 9cac e980 82e9 858d  river...........
+00000320: e599 a8e5 908c e697 b6e9 9c80 e8a6 8160  ...............`
+00000330: 5265 7665 7273 6544 7269 7665 7260 e592  ReverseDriver`..
+00000340: 8c60 466f 7277 6172 6444 7269 7665 7260  .`ForwardDriver`
+00000350: efbc 8ce5 8f82 e880 8320 5b64 7269 7665  ......... [drive
+00000360: 725d 2868 7474 7073 3a2f 2f76 322e 6e6f  r](https://v2.no
+00000370: 6e65 626f 742e 6465 762f 646f 6373 2f6e  nebot.dev/docs/n
+00000380: 6578 742f 6164 7661 6e63 6564 2f64 7269  ext/advanced/dri
+00000390: 7665 7223 2545 3925 4139 2542 3125 4535  ver#%E9%A9%B1%E5
+000003a0: 2538 4125 4138 2545 3525 3939 2541 3825  %8A%A8%E5%99%A8%
+000003b0: 4537 2542 3125 4242 2545 3525 3945 2538  E7%B1%BB%E5%9E%8
+000003c0: 4229 20e9 858d e7bd aee9 a1b9 e380 820a  B) .............
+000003d0: 0ae4 be8b e5a6 82ef bc9a 0a0a 6060 6064  ............```d
+000003e0: 6f74 656e 760a 4452 4956 4552 3d7e 6661  otenv.DRIVER=~fa
+000003f0: 7374 6170 692b 7e68 7474 7078 0a60 6060  stapi+~httpx.```
+00000400: 0a0a 2323 2320 5649 4c4c 415f 424f 5453  ..### VILLA_BOTS
+00000410: 0a0a e985 8de7 bdae e69c bae5 99a8 e4ba  ................
+00000420: bae5 b890 e58f b7e5 8897 e8a1 a8ef bc8c  ................
+00000430: e6af 8fe4 b8aa 626f 74e6 9c89 33e4 b8aa  ......bot...3...
+00000440: e5bf 85e5 a1ab e985 8de7 bdae efbc 8ce5  ................
+00000450: 9ca8 e5a4 a7e5 88ab e987 8ee5 ae98 e696  ................
+00000460: b9e6 9cba e599 a8e4 baba e5bc 80e5 8f91  ................
+00000470: e880 85e7 a4be e58c ba28 e588 abe9 878e  .........(......
+00000480: 4944 3a20 4f70 656e 5669 6c6c 6129 e794  ID: OpenVilla)..
+00000490: b3e8 afb7 e697 b6e8 8eb7 e5be 97ef bc8c  ................
+000004a0: 0a0a 2d20 626f 745f 6964 3a20 e69c bae5  ..- bot_id: ....
+000004b0: 99a8 e4ba ba69 64ef bc8c e4bb a560 626f  .....id......`bo
+000004c0: 745f 60e5 bc80 e5a4 b40a 2d20 626f 745f  t_`.......- bot_
+000004d0: 7365 6372 6574 3a20 e69c bae5 99a8 e4ba  secret: ........
+000004e0: bae5 af86 e992 a50a 2d20 6361 6c6c 6261  ........- callba
+000004f0: 636b 5f75 726c 3a20 6874 7470 e59b 9ee8  ck_url: http....
+00000500: b083 e59c b0e5 9d80 efbc 8ce4 be8b e5a6  ................
+00000510: 82e7 94b3 e8af b762 6f74 e697 b6e7 bb99  .......bot......
+00000520: e79a 84e5 9b9e e8b0 83e5 9cb0 e59d 80e6  ................
+00000530: 98af 6068 7474 703a 2f2f e59f 9fe5 908d  ..`http://......
+00000540: 2f79 6f75 722f 6361 6c6c 6261 636b 2f75  /your/callback/u
+00000550: 726c 60ef bc8c e982 a3e4 b988 e985 8de7  rl`.............
+00000560: bdae e987 8ce7 9a84 6063 616c 6c62 6163  ........`callbac
+00000570: 6b5f 7572 6c60 e5a1 abe5 8699 602f 796f  k_url`......`/yo
+00000580: 7572 2f63 616c 6c62 6163 6b2f 7572 6c60  ur/callback/url`
+00000590: 0a20 20e4 be8b e5a6 82ef bc9a 0a0a 6060  .  ...........``
+000005a0: 6064 6f74 656e 760a 5649 4c4c 415f 424f  `dotenv.VILLA_BO
+000005b0: 5453 3d27 0a5b 0a20 207b 0a20 2020 2022  TS='.[.  {.    "
+000005c0: 626f 745f 6964 223a 2022 626f 745f 3132  bot_id": "bot_12
+000005d0: 3334 3536 3738 3922 2c0a 2020 2020 2262  3456789",.    "b
+000005e0: 6f74 5f73 6563 7265 7422 3a20 2261 6263  ot_secret": "abc
+000005f0: 3132 3364 6566 3435 3622 2c0a 2020 2020  123def456",.    
+00000600: 2263 616c 6c62 6163 6b5f 7572 6c22 3a20  "callback_url": 
+00000610: 222f 796f 7572 2f63 616c 6c62 6163 6b2f  "/your/callback/
+00000620: 7572 6c22 0a20 207d 0a5d 0a27 0a60 6060  url".  }.].'.```
+00000630: 0a0a 2323 20e7 a4ba e4be 8b0a 0a23 2323  ..## ........###
+00000640: 20e6 b688 e681 afe6 aeb5 e5b1 95e7 a4ba   ...............
+00000650: 0a0a e4bb a5e4 b88b e698 afe4 b880 e4b8  ................
+00000660: aae7 ae80 e58d 95e7 9a84 e68f 92e4 bbb6  ................
+00000670: e7a4 bae4 be8b efbc 8ce5 b195 e7a4 bae5  ................
+00000680: 9084 e7a7 8de6 b688 e681 afe6 aeb5 efbc  ................
+00000690: 9a0a 0a60 6060 7079 7468 6f6e 0a66 726f  ...```python.fro
+000006a0: 6d20 6e6f 6e65 626f 7420 696d 706f 7274  m nonebot import
+000006b0: 206f 6e5f 636f 6d6d 616e 640a 6672 6f6d   on_command.from
+000006c0: 206e 6f6e 6562 6f74 2e70 6172 616d 7320   nonebot.params 
+000006d0: 696d 706f 7274 2043 6f6d 6d61 6e64 4172  import CommandAr
+000006e0: 670a 0a66 726f 6d20 6e6f 6e65 626f 742e  g..from nonebot.
+000006f0: 6164 6170 7465 7273 2e76 696c 6c61 2069  adapters.villa i
+00000700: 6d70 6f72 7420 426f 742c 2053 656e 644d  mport Bot, SendM
+00000710: 6573 7361 6765 4576 656e 742c 204d 6573  essageEvent, Mes
+00000720: 7361 6765 2c20 4d65 7373 6167 6553 6567  sage, MessageSeg
+00000730: 6d65 6e74 0a0a 6d61 7463 6865 7220 3d20  ment..matcher = 
+00000740: 6f6e 5f63 6f6d 6d61 6e64 2827 e58f 91e9  on_command('....
+00000750: 8081 2729 0a0a 406d 6174 6368 6572 2e68  ..')..@matcher.h
+00000760: 616e 646c 6528 290a 6173 796e 6320 6465  andle().async de
+00000770: 6620 6d61 7463 6865 725f 6861 6e64 6c65  f matcher_handle
+00000780: 7228 626f 743a 2042 6f74 2c20 6576 656e  r(bot: Bot, even
+00000790: 743a 2053 656e 644d 6573 7361 6765 4576  t: SendMessageEv
+000007a0: 656e 742c 2063 6d64 5f61 7267 3a20 4d65  ent, cmd_arg: Me
+000007b0: 7373 6167 6520 3d20 436f 6d6d 616e 6441  ssage = CommandA
+000007c0: 7267 2829 293a 0a20 2020 206d 7367 203d  rg()):.    msg =
+000007d0: 204d 6573 7361 6765 2829 0a20 2020 2061   Message().    a
+000007e0: 7267 7320 3d20 636d 645f 6172 672e 6578  rgs = cmd_arg.ex
+000007f0: 7472 6163 745f 706c 6169 6e5f 7465 7874  tract_plain_text
+00000800: 2829 2e73 7472 6970 2829 2e73 706c 6974  ().strip().split
+00000810: 2827 2027 290a 2020 2020 666f 7220 6172  (' ').    for ar
+00000820: 6720 696e 2061 7267 733a 0a20 2020 2020  g in args:.     
+00000830: 2020 2069 6620 6172 6720 3d3d 2022 e889     if arg == "..
+00000840: bee7 89b9 e688 9122 3a0a 2020 2020 2020  .......":.      
+00000850: 2020 2020 2020 6d73 6720 2b3d 204d 6573        msg += Mes
+00000860: 7361 6765 5365 676d 656e 742e 6d65 6e74  sageSegment.ment
+00000870: 696f 6e5f 7573 6572 2865 7665 6e74 2e76  ion_user(event.v
+00000880: 696c 6c61 5f69 642c 2065 7665 6e74 2e66  illa_id, event.f
+00000890: 726f 6d5f 7573 6572 5f69 6429 0a20 2020  rom_user_id).   
+000008a0: 2020 2020 2065 6c69 6620 6172 6720 3d3d       elif arg ==
+000008b0: 2022 e889 bee7 89b9 626f 7422 3a0a 2020   "......bot":.  
+000008c0: 2020 2020 2020 2020 2020 6d73 6720 2b3d            msg +=
+000008d0: 204d 6573 7361 6765 5365 676d 656e 742e   MessageSegment.
+000008e0: 6d65 6e74 696f 6e5f 726f 626f 7428 626f  mention_robot(bo
+000008f0: 742e 7365 6c66 5f69 642c 2062 6f74 2e6e  t.self_id, bot.n
+00000900: 6963 6b6e 616d 6529 0a20 2020 2020 2020  ickname).       
+00000910: 2065 6c69 6620 6172 6720 3d3d 2022 e696   elif arg == "..
+00000920: 87e5 ad97 223a 0a20 2020 2020 2020 2020  ....":.         
+00000930: 2020 206d 7367 202b 3d20 4d65 7373 6167     msg += Messag
+00000940: 6553 6567 6d65 6e74 2e74 6578 7428 22e6  eSegment.text(".
+00000950: 9687 e5ad 9722 290a 2020 2020 2020 2020  .....").        
+00000960: 2020 2020 2320 e8a1 a8e6 8385 e4b9 9fe6      # ..........
+00000970: 98af e794 a874 6578 74e6 9da5 e58f 91e9  .....text.......
+00000980: 8081 efbc 8ce4 bba5 5be8 a1a8 e683 85e5  ........[.......
+00000990: 908d 5de6 a0bc e5bc 8fef bc8c e4be 8be5  ..].............
+000009a0: a682 4d65 7373 6167 6553 6567 6d65 6e74  ..MessageSegment
+000009b0: 2e74 6578 7428 225b e788 b1e5 bf83 5d22  .text("[......]"
+000009c0: 290a 2020 2020 2020 2020 656c 6966 2061  ).        elif a
+000009d0: 7267 203d 3d20 22e6 88bf e997 b422 3a0a  rg == "......":.
+000009e0: 2020 2020 2020 2020 2020 2020 6d73 6720              msg 
+000009f0: 2b3d 204d 6573 7361 6765 5365 676d 656e  += MessageSegmen
+00000a00: 742e 726f 6f6d 5f6c 696e 6b28 6576 656e  t.room_link(even
+00000a10: 742e 7669 6c6c 615f 6964 2c20 6576 656e  t.villa_id, even
+00000a20: 742e 726f 6f6d 5f69 6429 0a20 2020 2020  t.room_id).     
+00000a30: 2020 2065 6c69 6620 6172 6720 3d3d 2022     elif arg == "
+00000a40: e993 bee6 8ea5 223a 0a20 2020 2020 2020  ......":.       
+00000a50: 2020 2020 206d 7367 202b 3d20 4d65 7373       msg += Mess
+00000a60: 6167 6553 6567 6d65 6e74 2e6c 696e 6b28  ageSegment.link(
+00000a70: 2268 7474 7073 3a2f 2f77 7777 2e6d 6979  "https://www.miy
+00000a80: 6f75 7368 652e 636f 6d2f 7973 2f61 7274  oushe.com/ys/art
+00000a90: 6963 6c65 2f33 3936 3730 3330 3722 2c20  icle/39670307", 
+00000aa0: 7368 6f77 5f74 6578 743d 22e8 bf99 e698  show_text=".....
+00000ab0: afe9 93be e68e a522 290a 2020 2020 2020  .......").      
+00000ac0: 2020 2020 2020 2320 e4bd bfe7 94a8 6c69        # ......li
+00000ad0: 6e6b e79a 84e8 af9d e993 bee6 8ea5 e883  nk..............
+00000ae0: bde5 a49f e782 b9e5 87bb e8bf 9be8 a18c  ................
+00000af0: e8b7 b3e8 bdac efbc 8ce4 bdbf e794 a874  ...............t
+00000b00: 6578 74e7 9a84 e8af 9de4 b88d e883 bde7  ext.............
+00000b10: 82b9 e587 bb0a 2020 2020 2020 2020 2020  ......          
+00000b20: 2020 2320 7368 6f77 5f74 6578 74e6 98af    # show_text...
+00000b30: e68c 87e9 93be e68e a5e6 98be e7a4 bae7  ................
+00000b40: 9a84 e696 87e5 ad97 efbc 8ce4 bd86 e59c  ................
+00000b50: a8e5 bd93 e589 8de7 8988 e69c ac57 6562  .............Web
+00000b60: e7ab afe5 a4a7 e588 abe9 878e e4bc 9ae6  ................
+00000b70: 97a0 e6b3 95e6 ada3 e5b8 b8e8 b7b3 e8bd  ................
+00000b80: acef bc8c e69c 80e5 a5bd e4b8 8de4 bdbf  ................
+00000b90: e794 a8e8 afa5 e58f 82e6 95b0 0a20 2020  .............   
+00000ba0: 2020 2020 2065 6c69 6620 6172 6720 3d3d       elif arg ==
+00000bb0: 2022 e59b bee7 8987 223a 0a20 2020 2020   "......":.     
+00000bc0: 2020 2020 2020 206d 7367 202b 3d20 4d65         msg += Me
+00000bd0: 7373 6167 6553 6567 6d65 6e74 2e69 6d61  ssageSegment.ima
+00000be0: 6765 2822 6874 7470 733a 2f2f 7777 772e  ge("https://www.
+00000bf0: 6d69 796f 7573 6865 2e63 6f6d 2f5f 6e75  miyoushe.com/_nu
+00000c00: 7874 2f69 6d67 2f6d 6948 6f59 6f5f 4761  xt/img/miHoYo_Ga
+00000c10: 6d65 2e32 3435 3737 3533 2e70 6e67 2229  me.2457753.png")
+00000c20: 0a20 2020 2020 2020 2020 2020 2023 20e6  .            # .
+00000c30: 9a82 e697 b6e5 8faa e694 afe6 8c81 7572  ..............ur
+00000c40: 6ce5 9bbe e789 87ef bc8c e4bd 86e5 9ca8  l...............
+00000c50: e5bd 93e5 898d e789 88e6 9cac 7765 62e7  ............web.
+00000c60: abaf e697 a0e6 b395 e698 bee7 a4ba e59b  ................
+00000c70: bee7 8987 efbc 8ce5 be85 e5ae 98e6 96b9  ................
+00000c80: e590 8ee7 bbad e4bf aee5 a48d 0a20 2020  .............   
+00000c90: 2061 7761 6974 206d 6174 6368 6572 2e66   await matcher.f
+00000ca0: 696e 6973 6828 6d73 6729 0a60 6060 0a0a  inish(msg).```..
+00000cb0: e4bd bfe7 94a8 e591 bde4 bba4 6040 626f  ............`@bo
+00000cc0: 7420 2fe5 8f91 e980 8120 e889 bee7 89b9  t /...... ......
+00000cd0: e688 9120 e889 bee7 89b9 626f 7420 e696  ... ......bot ..
+00000ce0: 87e5 ad97 20e6 88bf e997 b420 e993 bee6  .... ...... ....
+00000cf0: 8ea5 20e5 9bbe e789 8760 e697 b6ef bc8c  .. ......`......
+00000d00: 626f 74e4 bc9a e59b 9ee5 a48d 6040 e4bd  bot.........`@..
+00000d10: a0e7 9a84 e590 8de5 ad97 2040 626f 74e7  .......... @bot.
+00000d20: 9a84 e590 8de5 ad97 20e6 9687 e5ad 9720  ........ ...... 
+00000d30: 23e6 88bf e997 b4e5 908d 20e8 bf99 e698  #......... .....
+00000d40: afe9 93be e68e a520 e59b bee7 8987 e586  ....... ........
+00000d50: 85e5 aeb9 600a 0a0a 2323 20e4 baa4 e6b5  ....`...## .....
+00000d60: 81e5 928c e58f 8de9 a688 0a0a e79b aee5  ................
+00000d70: 898d e697 a0e8 aeba e698 afe5 a4a7 e588  ................
+00000d80: abe9 878e 426f 74e8 bf98 e698 afe6 9cac  ....Bot.........
+00000d90: e980 82e9 858d e599 a8e9 83bd e59c a8e6  ................
+00000da0: b58b e8af 95e5 bc80 e58f 91e4 b8ad efbc  ................
+00000db0: 8ce5 a682 e981 87e9 97ae e9a2 98e8 afb7  ................
+00000dc0: e68f 90e5 87ba 6973 7375 65ef bc8c e684  ......issue.....
+00000dd0: 9fe8 b0a2 e694 afe6 8c81 efbc 810a 0ae4  ................
+00000de0: b99f e6ac a2e8 bf8e e69d a5e6 8891 e79a  ................
+00000df0: 84e5 a4a7 e588 abe9 878e e380 90e5 b098  ................
+00000e00: e4b8 96e9 97b2 e6b8 b8e3 8091 e8bf 9be8  ................
+00000e10: a18c e4ba a4e6 b581 efbc 9a0a 0a2d 20e5  .............- .
+00000e20: a4a7 e588 abe9 878e 4944 3a20 7767 694a  ........ID: wgiJ
+00000e30: 4e61 55ef bc8c e58f afe6 909c e7b4 a2e5  NaU.............
+00000e40: 8aa0 e585 a50a 2d20 5b57 6562 e7ab afe9  ......- [Web....
+00000e50: 93be e68e a55d 2868 7474 7073 3a2f 2f64  .....](https://d
+00000e60: 6279 2e6d 6979 6f75 7368 652e 636f 6d2f  by.miyoushe.com/
+00000e70: 6368 6174 2f31 3034 372f 3231 3635 3229  chat/1047/21652)
+00000e80: efbc 8ce7 9bae e589 8de4 bb85 5043 e7ab  ............PC..
+00000e90: afe5 8faf e8ae bfe9 97ae 0a0a 2323 20e7  ............## .
+00000ea0: 9bb8 e585 b3e9 a1b9 e79b ae0a 0a2d 205b  .............- [
+00000eb0: 4e6f 6e65 426f 7432 5d28 6874 7470 733a  NoneBot2](https:
+00000ec0: 2f2f 6769 7468 7562 2e63 6f6d 2f6e 6f6e  //github.com/non
+00000ed0: 6562 6f74 2f6e 6f6e 6562 6f74 3229 3a20  ebot/nonebot2): 
+00000ee0: e99d 9ee5 b8b8 e5a5 bde7 94a8 e79a 8450  ...............P
+00000ef0: 7974 686f 6ee8 b7a8 e5b9 b3e5 8fb0 e69c  ython...........
+00000f00: bae5 99a8 e4ba bae6 a186 e69e b6ef bc81  ................
+00000f10: 0a2d 205b 7669 6c6c 612d 7079 5d28 6874  .- [villa-py](ht
+00000f20: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
+00000f30: 2f43 4d48 6f70 6553 756e 7368 696e 652f  /CMHopeSunshine/
+00000f40: 7669 6c6c 612d 7079 293a 20e5 a4a7 e588  villa-py): .....
+00000f50: abe9 878e 2042 6f74 2050 7974 686f 6e20  .... Bot Python 
+00000f60: 5344 4be3 8082 0a0a e68e a8e8 8d90 e69c  SDK.............
+00000f70: 89e6 8890 e786 9f50 7974 686f 6ee5 bc80  .......Python...
+00000f80: e58f 91e7 bb8f e9aa 8ce4 bd86 e5af b94e  ...............N
+00000f90: 6f6e 6542 6f74 32e4 b88d e786 9fe6 8289  oneBot2.........
+00000fa0: e79a 84e5 b08f e4bc 99e4 bcb4 e980 89e6  ................
+00000fb0: 8ba9 60e5 a4a7 e588 abe9 878e 426f 7420  ..`.........Bot 
+00000fc0: 5079 7468 6f6e 2053 444b 60ef bc8c 0a0a  Python SDK`.....
+00000fd0: e5af b94e 6f6e 6542 6f74 32e7 869f e682  ...NoneBot2.....
+00000fe0: 89e6 8896 e5b8 8ce6 9c9b e68e a5e8 a7a6  ................
+00000ff0: e69b b4e6 8890 e786 9fe7 9a84 e794 9fe6  ................
+00001000: 8081 e79a 84e5 b08f e4bc 99e4 bcb4 e980  ................
+00001010: 89e6 8ba9 604e 6f6e 6542 6f74 322b e69c  ....`NoneBot2+..
+00001020: ace9 8082 e985 8de5 99a8 60e8 bf9b e8a1  ..........`.....
+00001030: 8ce5 bc80 e58f 91e3 8082                 ..........
```

### Comparing `nonebot_adapter_villa-0.1.0/nonebot/adapters/villa/adapter.py` & `nonebot_adapter_villa-0.1.1/nonebot/adapters/villa/adapter.py`

 * *Files 2% similar despite different names*

```diff
@@ -76,15 +76,15 @@
                     ) is not None:
                         bot = Bot(self, bot_id, payload.robot, bot_secret=bot_secret)
                         self.bot_connect(bot)
                         log("INFO", f"<y>Bot {escape_tag(bot.self_id)} connected</y>")
                     else:
                         log("WARNING", f"<r>Missing bot secret for bot {bot_id}</r>")
                 bot = cast(Bot, bot)
-                bot.bot_info = payload.robot
+                bot._bot_info = payload.robot
 
                 if (event_class := event_classes.get(payload.type, None)) and (
                     event_class.__type__.name in payload.extend_data["EventData"]
                 ):
                     try:
                         event = event_class.parse_obj(
                             payload.extend_data["EventData"][event_class.__type__.name]
@@ -109,10 +109,11 @@
                 )
             return Response(400, content="Invalid Request Body")
         return Response(400, content="Invalid Request Body")
 
     @overrides(BaseAdapter)
     async def _call_api(self, bot: Bot, api: str, **data: Any) -> Any:
         log("DEBUG", f"Calling API <y>{api}</y>")
+        log("TRACE", f"With Data <y>{data}</y>")
         if (api_handler := API_HANDLERS.get(api)) is None:
             raise ApiNotAvailable(api)
         return await api_handler(self, bot, **data)
```

### Comparing `nonebot_adapter_villa-0.1.0/nonebot/adapters/villa/api/cilent.pyi` & `nonebot_adapter_villa-0.1.1/nonebot/adapters/villa/api/cilent.pyi`

 * *Files identical despite different names*

### Comparing `nonebot_adapter_villa-0.1.0/nonebot/adapters/villa/api/client.py` & `nonebot_adapter_villa-0.1.1/nonebot/adapters/villa/api/client.py`

 * *Files identical despite different names*

### Comparing `nonebot_adapter_villa-0.1.0/nonebot/adapters/villa/api/handle.py` & `nonebot_adapter_villa-0.1.1/nonebot/adapters/villa/api/handle.py`

 * *Files identical despite different names*

### Comparing `nonebot_adapter_villa-0.1.0/nonebot/adapters/villa/api/models.py` & `nonebot_adapter_villa-0.1.1/nonebot/adapters/villa/api/models.py`

 * *Files 16% similar despite different names*

```diff
@@ -44,24 +44,40 @@
     id: str
     created_at: int
     send_at: int
     extend_data: dict
 
     @root_validator(pre=True)
     def _add_villa_id_to_extend_data(cls, values: dict):
-        """把villa_id添加到extend_data中，方便使用"""
-        if (
-            values.get("type") == 2
-            and "villa_id" in values.get("robot", {})
-            and "SendMessage" in values.get("extend_data", {}).get("EventData", {})
-            and "villa_id" not in values["extend_data"]["EventData"]["SendMessage"]
-        ):
-            values["extend_data"]["EventData"]["SendMessage"]["villa_id"] = values[
-                "robot"
-            ]["villa_id"]
+        """把villa_id和bot_id添加到extend_data中，方便使用"""
+        if values.get("type") == 2 and "SendMessage" in values.get(
+            "extend_data", {}
+        ).get("EventData", {}):
+            if isinstance(
+                values["extend_data"]["EventData"]["SendMessage"]["content"], str
+            ):
+                values["extend_data"]["EventData"]["SendMessage"][
+                    "content"
+                ] = json.loads(
+                    values["extend_data"]["EventData"]["SendMessage"]["content"]
+                )
+            if (
+                "villa_id" in values.get("robot", {})
+                and "villa_id" not in values["extend_data"]["EventData"]["SendMessage"]
+            ):
+                values["extend_data"]["EventData"]["SendMessage"]["villa_id"] = values[
+                    "robot"
+                ]["villa_id"]
+            if (
+                "id" in values.get("robot", {}).get("template", {})
+                and "bot_id" not in values["extend_data"]["EventData"]["SendMessage"]
+            ):
+                values["extend_data"]["EventData"]["SendMessage"]["bot_id"] = values[
+                    "robot"
+                ]["template"]["id"]
         return values
 
 
 ## 鉴权部分
 ## see https://webstatic.mihoyo.com/vila/bot/doc/auth_api/
 class BotMemberAccessInfo(BaseModel):
     uid: int
@@ -120,34 +136,44 @@
         return self.name
 
 
 class MentionedRobot(BaseModel):
     type: Literal["mentioned_robot"] = "mentioned_robot"
     bot_id: str
 
+    bot_name: str = Field(exclude=True)
+
 
 class MentionedUser(BaseModel):
     type: Literal["mentioned_user"] = "mentioned_user"
     user_id: str
 
+    user_name: str = Field(exclude=True)
+
 
 class MentionedAll(BaseModel):
     type: Literal["mention_all"] = "mention_all"
 
+    show_text: str = Field(exclude=True)
+
 
 class VillaRoomLink(BaseModel):
     type: Literal["villa_room_link"] = "villa_room_link"
     villa_id: str
     room_id: str
 
+    room_name: str = Field(exclude=True)
+
 
 class Link(BaseModel):
     type: Literal["link"] = "link"
     url: str
 
+    show_text: str = Field(exclude=True)
+
 
 class TextEntity(BaseModel):
     offset: int
     length: int
     entity: Union[MentionedRobot, MentionedUser, MentionedAll, VillaRoomLink, Link]
```

### Comparing `nonebot_adapter_villa-0.1.0/nonebot/adapters/villa/api/request.py` & `nonebot_adapter_villa-0.1.1/nonebot/adapters/villa/api/request.py`

 * *Files identical despite different names*

### Comparing `nonebot_adapter_villa-0.1.0/nonebot/adapters/villa/bot.py` & `nonebot_adapter_villa-0.1.1/nonebot/adapters/villa/bot.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import TYPE_CHECKING, Any, Dict, List, Union
+from typing import TYPE_CHECKING, Any, Dict, List, Union, Optional
 
 from nonebot.typing import overrides
 from nonebot.message import handle_event
 from nonebot.internal.adapter.adapter import Adapter
 
 from nonebot.adapters import Bot as BaseBot
 
@@ -14,14 +14,15 @@
     Robot,
     ApiClient,
     ImageSize,
     QuoteInfo,
     TextEntity,
     MentionType,
     MentionedAll,
+    RobotCommand,
     MentionedInfo,
     MentionedUser,
     VillaRoomLink,
     MentionedRobot,
     MessageContent,
     MessageContentInfo,
 )
@@ -54,17 +55,16 @@
         event.content.mentioned_info
         and bot.self_id in event.content.mentioned_info.user_id_list
     ):
         event.to_me = True
 
     def _is_at_me_seg(segment: MessageSegment) -> bool:
         return (
-            segment.type
-            == "mentioned_robot"
-            # and segment.data.get("bot_id") == bot.self_id
+            segment.type == "mentioned_robot"
+            and segment.data.get("bot_id") == bot.self_id
         )
 
     message = event.get_message()
     if not message:
         message.append(MessageSegment.text(""))
 
     deleted = False
@@ -103,42 +103,67 @@
 
     @overrides(BaseBot)
     def __init__(
         self, adapter: Adapter, self_id: str, bot_info: Robot, bot_secret: str
     ):
         super().__init__(adapter, self_id)
         self.adapter: Adapter = adapter
-        self.bot_info: Robot = bot_info
         self.bot_secret: str = bot_secret
+        self._bot_info: Robot = bot_info
 
     @overrides(BaseBot)
     def __repr__(self) -> str:
         return f"Bot(type={self.type!r}, self_id={self.self_id!r})"
 
+    @property
+    def nickname(self) -> str:
+        """Bot 昵称"""
+        return self._bot_info.template.name
+
+    @property
+    def commands(self) -> Optional[List[RobotCommand]]:
+        """Bot 命令预设命令列表"""
+        return self._bot_info.template.commands
+
+    @property
+    def description(self) -> str:
+        """Bot 介绍描述"""
+        return self._bot_info.template.desc
+
+    @property
+    def avatar_icon(self) -> str:
+        """Bot 头像图标地址"""
+        return self._bot_info.template.icon
+
+    @property
+    def current_villd_id(self) -> int:
+        return self._bot_info.villa_id
+
     async def handle_event(self, event: Event):
         """处理事件"""
         if isinstance(event, SendMessageEvent):
             _check_at_me(self, event)
             # await _check_reply(self, event)
         await handle_event(self, event)
 
-    def get_authorization_header(self, villa_id: int) -> Dict[str, str]:
-        """机器人凭证请求头
+    def get_authorization_header(
+        self, villa_id: Optional[int] = None
+    ) -> Dict[str, str]:
+        """Bot 鉴权凭证请求头
 
         参数:
             villa_id: 大别野ID
 
         返回:
             Dict[str, str]: 请求头
         """
         return {
             "x-rpc-bot_id": self.self_id,
             "x-rpc-bot_secret": self.bot_secret,
-            "x-rpc-bot_villa_id": str(villa_id),
-            # "Content-Type": "application/json"
+            "x-rpc-bot_villa_id": str(villa_id or ""),
         }
 
     @overrides(BaseBot)
     async def send(
         self,
         event: Event,
         message: Union[str, Message, MessageSegment],
@@ -198,105 +223,106 @@
             )
 
         message_text = ""
         message_offset = 0
         entities: List[TextEntity] = []
         images: List[Image] = []
         mentioned = MentionedInfo(type=MentionType.PART)
-        for i, seg in enumerate(message):
-            space = " " if i != len(message) - 1 else ""
-            if seg.type == "quote":
-                # 引用消息段在上方处理了，这里不需要处理
-                continue
-            elif seg.type == "text":
+        for seg in message:
+            if seg.type == "text":
                 message_text += seg.data["text"]
                 message_offset += len(seg.data["text"])
             elif seg.type == "mention_all":
-                message_text += "@全体成员{space}"
+                message_text += f"@{seg.data['show_text']} "
                 entities.append(
-                    TextEntity(offset=message_offset, length=6, entity=MentionedAll())
+                    TextEntity(
+                        offset=message_offset,
+                        length=6,
+                        entity=MentionedAll(show_text=seg.data["show_text"]),
+                    )
                 )
                 message_offset += 6
                 mentioned.type = MentionType.ALL
             elif seg.type == "mentioned_robot":
-                # 目前只能@到自己，尚未有办法@到其他机器人，所以这里先直接@到自己
-                message_text += f"@{self.bot_info.template.name}{space}"
+                message_text += f"@{seg.data['bot_name']} "
                 entities.append(
                     TextEntity(
                         offset=message_offset,
-                        length=len(f"@{self.bot_info.template.name}".encode("utf-16"))
-                        // 2,
-                        entity=MentionedRobot(bot_id=self.self_id),
+                        length=len(f"@{seg.data['bot_name']}".encode("utf-16")) // 2,
+                        entity=MentionedRobot(
+                            bot_id=seg.data["bot_id"], bot_name=seg.data["bot_name"]
+                        ),
                     )
                 )
-                message_offset += len(f"@{self.bot_info.template.name}") + 1
-                mentioned.user_id_list.append(self.self_id)
+                message_offset += len(f"@{seg.data['bot_name']}") + 1
+                mentioned.user_id_list.append(seg.data["bot_id"])
             elif seg.type == "mentioned_user":
                 # 需要调用API获取被@的用户的昵称
                 user = await self.get_member(
                     villa_id=seg.data["villa_id"], uid=seg.data["user_id"]
                 )
-                message_text += f"@{user.basic.nickname}{space}"
+                message_text += f"@{user.basic.nickname} "
                 entities.append(
                     TextEntity(
                         offset=message_offset,
                         length=len(f"@{user.basic.nickname}".encode("utf-16")) // 2,
-                        entity=MentionedUser(user_id=str(user.basic.uid)),
+                        entity=MentionedUser(
+                            user_id=str(user.basic.uid), user_name=user.basic.nickname
+                        ),
                     )
                 )
                 message_offset += len(f"@{user.basic.nickname}") + 1
                 mentioned.user_id_list.append(str(user.basic.uid))
             elif seg.type == "villa_room_link":
                 # 需要调用API获取房间的名称
                 room = await self.get_room(
                     villa_id=seg.data["villa_id"], room_id=seg.data["room_id"]
                 )
-                message_text += f"#{room.room_name}{space}"
+                message_text += f"#{room.room_name} "
                 entities.append(
                     TextEntity(
                         offset=message_offset,
                         length=len(f"#{room.room_name}".encode("utf-16")) // 2,
                         entity=VillaRoomLink(
                             villa_id=str(seg.data["villa_id"]),
                             room_id=str(seg.data["room_id"]),
+                            room_name=room.room_name,
                         ),
                     )
                 )
                 message_offset += len(f"#{room.room_name} ")
             elif seg.type == "link":
-                show_text: str = seg.data["text"] or seg.data["url"]
-                message_text += (show_text) + space
+                message_text += seg.data["show_text"]
                 entities.append(
                     TextEntity(
                         offset=message_offset,
-                        length=len(show_text.encode("utf-16")) // 2,
-                        entity=Link(url=seg.data["url"]),
+                        length=len(seg.data["show_text"].encode("utf-16")) // 2,
+                        entity=Link(
+                            url=seg.data["url"], show_text=seg.data["show_text"]
+                        ),
                     )
                 )
-                message_offset += len(show_text) + 1
+                message_offset += len(seg.data["show_text"]) + 1
             elif seg.type == "image":
                 images.append(
                     Image(
                         url=seg.data["url"],
                         size=ImageSize(
                             width=seg.data["width"], height=seg.data["height"]
                         )
                         if seg.data["width"] and seg.data["height"]
                         else None,
                         file_size=seg.data["file_size"],
                     )
                 )
 
-        # 不能单独只发图片而没有其他文本内容
+        # 不能单独只发图片而没有其他文本内容，塞一个零宽度空格
         if images and not message_text:
-            message_text = "图片"
+            message_text = "\u200B"
 
         if not (mentioned.type == MentionType.ALL and mentioned.user_id_list):
             mentioned = None
         return MessageContentInfo(
             content=MessageContent(text=message_text, entities=entities, images=images),
             mentionedInfo=mentioned,
             quote=quote,  # type: ignore
         )
-        # from pathlib import Path
-        # (Path().cwd() / 'send_msg.json').write_text(a.json(by_alias=True, exclude_none=True))
-        # return a
```

### Comparing `nonebot_adapter_villa-0.1.0/nonebot/adapters/villa/exception.py` & `nonebot_adapter_villa-0.1.1/nonebot/adapters/villa/exception.py`

 * *Files identical despite different names*

### Comparing `nonebot_adapter_villa-0.1.0/pyproject.toml` & `nonebot_adapter_villa-0.1.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "nonebot-adapter-villa"
-version = "0.1.0"
+version = "0.1.1"
 description = "NoneBot2米游社大别野Bot适配器。MiHoYo Villa Bot adapter for nonebot2."
 authors = ["CMHopeSunshine <277073121@qq.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/CMHopeSunshine/nonebot-adapter-villa"
 repository = "https://github.com/CMHopeSunshine/nonebot-adapter-villa"
 documentation = "https://github.com/CMHopeSunshine/nonebot-adapter-villa"
```

### Comparing `nonebot_adapter_villa-0.1.0/PKG-INFO` & `nonebot_adapter_villa-0.1.1/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 00000000: 4d65 7461 6461 7461 2d56 6572 7369 6f6e  Metadata-Version
 00000010: 3a20 322e 310a 4e61 6d65 3a20 6e6f 6e65  : 2.1.Name: none
 00000020: 626f 742d 6164 6170 7465 722d 7669 6c6c  bot-adapter-vill
-00000030: 610a 5665 7273 696f 6e3a 2030 2e31 2e30  a.Version: 0.1.0
+00000030: 610a 5665 7273 696f 6e3a 2030 2e31 2e31  a.Version: 0.1.1
 00000040: 0a53 756d 6d61 7279 3a20 4e6f 6e65 426f  .Summary: NoneBo
 00000050: 7432 e7b1 b3e6 b8b8 e7a4 bee5 a4a7 e588  t2..............
 00000060: abe9 878e 426f 74e9 8082 e985 8de5 99a8  ....Bot.........
 00000070: e380 824d 6948 6f59 6f20 5669 6c6c 6120  ...MiHoYo Villa 
 00000080: 426f 7420 6164 6170 7465 7220 666f 7220  Bot adapter for 
 00000090: 6e6f 6e65 626f 7432 2e0a 486f 6d65 2d70  nonebot2..Home-p
 000000a0: 6167 653a 2068 7474 7073 3a2f 2f67 6974  age: https://git
@@ -88,244 +88,229 @@
 00000570: 3d22 6874 7470 733a 2f2f 696d 672e 7368  ="https://img.sh
 00000580: 6965 6c64 732e 696f 2f67 6974 6875 622f  ields.io/github/
 00000590: 6c69 6365 6e73 652f 434d 486f 7065 5375  license/CMHopeSu
 000005a0: 6e73 6869 6e65 2f6e 6f6e 6562 6f74 2d61  nshine/nonebot-a
 000005b0: 6461 7074 6572 2d76 696c 6c61 2220 616c  dapter-villa" al
 000005c0: 743d 226c 6963 656e 7365 223e 3c2f 613e  t="license"></a>
 000005d0: 0a0a 3c2f 6469 763e 0a0a 2323 20e5 ae89  ..</div>..## ...
-000005e0: e8a3 850a 0a2d 20e5 9ca8 604e 6f6e 6542  .....- ...`NoneB
-000005f0: 6f74 3260 e9a1 b9e7 9bae e79b aee5 bd95  ot2`............
-00000600: e4b8 8be4 bdbf e794 a8e8 849a e689 8be6  ................
-00000610: 9eb6 e5ae 89e8 a385 efbc 9a60 6e62 2061  ...........`nb a
-00000620: 6461 7074 6572 2069 6e73 7461 6c6c 206e  dapter install n
-00000630: 6f6e 6562 6f74 2d61 6461 7074 6572 2d76  onebot-adapter-v
-00000640: 696c 6c61 600a 2020 0ae6 8896 efbc 9a0a  illa`.  ........
-00000650: 0a2d 20e5 9ca8 604e 6f6e 6542 6f74 3260  .- ...`NoneBot2`
-00000660: e9a1 b9e7 9bae e78e afe5 a283 e4b8 8be4  ................
-00000670: bdbf e794 a870 6970 e5ae 89e8 a385 e590  .....pip........
-00000680: 8ee6 898b e58a a8e6 b3a8 e586 8cef bc9a  ................
-00000690: 6070 6970 2069 6e73 7461 6c6c 206e 6f6e  `pip install non
-000006a0: 6562 6f74 2d61 6461 7074 6572 2d76 696c  ebot-adapter-vil
-000006b0: 6c61 600a 0a23 2320 e985 8de7 bdae 0a0a  la`..## ........
-000006c0: e4bf aee6 94b9 204e 6f6e 6542 6f74 20e9  ...... NoneBot .
-000006d0: 858d e7bd aee6 9687 e4bb b620 602e 656e  ........... `.en
-000006e0: 7660 20e6 8896 e880 8520 602e 656e 762e  v` ...... `.env.
-000006f0: 2a60 e380 820a 0a23 2323 2044 7269 7665  *`.....### Drive
-00000700: 720a 0ae6 9cac e980 82e9 858d e599 a8e5  r...............
-00000710: 908c e697 b6e9 9c80 e8a6 8160 5265 7665  ...........`Reve
-00000720: 7273 6544 7269 7665 7260 e592 8c60 466f  rseDriver`...`Fo
-00000730: 7277 6172 6444 7269 7665 7260 efbc 8ce5  rwardDriver`....
-00000740: 8f82 e880 8320 5b64 7269 7665 725d 2868  ..... [driver](h
-00000750: 7474 7073 3a2f 2f76 322e 6e6f 6e65 626f  ttps://v2.nonebo
-00000760: 742e 6465 762f 646f 6373 2f6e 6578 742f  t.dev/docs/next/
-00000770: 6164 7661 6e63 6564 2f64 7269 7665 7223  advanced/driver#
-00000780: 2545 3925 4139 2542 3125 4535 2538 4125  %E9%A9%B1%E5%8A%
-00000790: 4138 2545 3525 3939 2541 3825 4537 2542  A8%E5%99%A8%E7%B
-000007a0: 3125 4242 2545 3525 3945 2538 4229 20e9  1%BB%E5%9E%8B) .
-000007b0: 858d e7bd aee9 a1b9 e380 820a 0ae4 be8b  ................
-000007c0: e5a6 82ef bc9a 0a0a 6060 6064 6f74 656e  ........```doten
-000007d0: 760a 4452 4956 4552 3d7e 6661 7374 6170  v.DRIVER=~fastap
-000007e0: 692b 7e68 7474 7078 0a60 6060 0a0a 2323  i+~httpx.```..##
-000007f0: 2320 5649 4c4c 415f 424f 5453 0a0a e985  # VILLA_BOTS....
-00000800: 8de7 bdae e69c bae5 99a8 e4ba bae5 b890  ................
-00000810: e58f b7e5 8897 e8a1 a8ef bc8c e6af 8fe4  ................
-00000820: b8aa 626f 74e6 9c89 33e4 b8aa e5bf 85e5  ..bot...3.......
-00000830: a1ab e985 8de7 bdae efbc 8ce5 9ca8 e5a4  ................
-00000840: a7e5 88ab e987 8ee6 9cba e599 a8e4 baba  ................
-00000850: e5bc 80e5 8f91 e880 85e7 a4be e58c bae7  ................
-00000860: 94b3 e8af b7e6 97b6 e88e b7e5 be97 efbc  ................
-00000870: 8c0a 0a2d 2062 6f74 5f69 643a 20e6 9cba  ...- bot_id: ...
-00000880: e599 a8e4 baba 6964 efbc 8ce4 bba5 6062  ......id......`b
-00000890: 6f74 5f60 e5bc 80e5 a4b4 0a2d 2062 6f74  ot_`.......- bot
-000008a0: 5f73 6563 7265 743a 20e6 9cba e599 a8e4  _secret: .......
-000008b0: baba e5af 86e9 92a5 0a2d 2063 616c 6c62  .........- callb
-000008c0: 6163 6b5f 7572 6c3a 2068 7474 70e5 9b9e  ack_url: http...
-000008d0: e8b0 83e5 9cb0 e59d 80ef bc8c e4be 8be5  ................
-000008e0: a682 e794 b3e8 afb7 626f 74e6 97b6 e7bb  ........bot.....
-000008f0: 99e7 9a84 e59b 9ee8 b083 e59c b0e5 9d80  ................
-00000900: e698 af60 6874 7470 3a2f 2fe5 9f9f e590  ...`http://.....
-00000910: 8d2f 796f 7572 2f63 616c 6c62 6163 6b2f  ./your/callback/
-00000920: 7572 6c60 efbc 8ce9 82a3 e4b9 88e9 858d  url`............
-00000930: e7bd aee9 878c e79a 8460 6361 6c6c 6261  .........`callba
-00000940: 636b 5f75 726c 60e5 a1ab e586 9960 2f79  ck_url`......`/y
-00000950: 6f75 722f 6361 6c6c 6261 636b 2f75 726c  our/callback/url
-00000960: 600a 2020 e4be 8be5 a682 efbc 9a0a 0a60  `.  ...........`
-00000970: 6060 646f 7465 6e76 0a56 494c 4c41 5f42  ``dotenv.VILLA_B
-00000980: 4f54 533d 270a 5b0a 2020 7b0a 2020 2020  OTS='.[.  {.    
-00000990: 2262 6f74 5f69 6422 3a20 2262 6f74 5f31  "bot_id": "bot_1
-000009a0: 3233 3435 3637 3839 222c 0a20 2020 2022  23456789",.    "
-000009b0: 626f 745f 7365 6372 6574 223a 2022 6162  bot_secret": "ab
-000009c0: 6331 3233 6465 6634 3536 222c 0a20 2020  c123def456",.   
-000009d0: 2022 6361 6c6c 6261 636b 5f75 726c 223a   "callback_url":
-000009e0: 2022 2f79 6f75 722f 6361 6c6c 6261 636b   "/your/callback
-000009f0: 2f75 726c 220a 2020 7d0a 5d0a 270a 6060  /url".  }.].'.``
-00000a00: 600a 0a23 2320 e4bd bfe7 94a8 0a0a 2323  `..## ........##
-00000a10: 2320 e6b3 a8e5 868c e980 82e9 858d e599  # ..............
-00000a20: a80a 0a3e 20e5 a682 e4bd bfe7 94a8 6e62  ...> .........nb
-00000a30: e884 9ae6 898b e69e b6e6 9da5 e5ae 89e8  ................
-00000a40: a385 e79a 84ef bc8c e588 99e4 b88d e794  ................
-00000a50: a8e6 898b e58a a8e6 b3a8 e586 8c0a 0ae5  ................
-00000a60: 9ca8 6062 6f74 2e70 7960 e696 87e4 bbb6  ..`bot.py`......
-00000a70: e4b8 ad28 e5a6 82e6 9e9c e6b2 a1e6 9c89  ...(............
-00000a80: efbc 8ce4 bdbf e794 a860 6e62 2067 656e  .........`nb gen
-00000a90: 6572 6174 6560 e69d a5e7 949f e688 9029  erate`.........)
-00000aa0: e6b3 a8e5 868c e69c ace9 8082 e985 8de5  ................
-00000ab0: 99a8 efbc 8ce5 8f82 e880 835b 6164 6170  ...........[adap
-00000ac0: 7465 725d 2868 7474 7073 3a2f 2f76 322e  ter](https://v2.
-00000ad0: 6e6f 6e65 626f 742e 6465 762f 646f 6373  nonebot.dev/docs
-00000ae0: 2f61 6476 616e 6365 642f 6164 6170 7465  /advanced/adapte
-00000af0: 7229 efbc 8ce4 be8b e5a6 82ef bc9a 0a0a  r)..............
-00000b00: 6060 6070 7974 686f 6e0a 696d 706f 7274  ```python.import
-00000b10: 206e 6f6e 6562 6f74 0a66 726f 6d20 6e6f   nonebot.from no
-00000b20: 6e65 626f 742e 6164 6170 7465 7273 2e76  nebot.adapters.v
-00000b30: 696c 6c61 2069 6d70 6f72 7420 4164 6170  illa import Adap
-00000b40: 7465 7220 6173 2056 696c 6c61 4164 6170  ter as VillaAdap
-00000b50: 7465 7220 2023 20e5 afbc e585 a561 6461  ter  # ......ada
-00000b60: 7074 6572 0a0a 6e6f 6e65 626f 742e 696e  pter..nonebot.in
-00000b70: 6974 2829 0a0a 6472 6976 6572 203d 206e  it()..driver = n
-00000b80: 6f6e 6562 6f74 2e67 6574 5f64 7269 7665  onebot.get_drive
-00000b90: 7228 290a 6472 6976 6572 2e72 6567 6973  r().driver.regis
-00000ba0: 7465 725f 6164 6170 7465 7228 5669 6c6c  ter_adapter(Vill
-00000bb0: 6141 6461 7074 6572 2920 2320 e6b3 a8e5  aAdapter) # ....
-00000bc0: 868c 6164 6170 7465 720a 0a6e 6f6e 6562  ..adapter..noneb
-00000bd0: 6f74 2e6c 6f61 645f 6672 6f6d 5f74 6f6d  ot.load_from_tom
-00000be0: 6c28 2270 7970 726f 6a65 6374 2e74 6f6d  l("pyproject.tom
-00000bf0: 6c22 290a 0a69 6620 5f5f 6e61 6d65 5f5f  l")..if __name__
-00000c00: 203d 3d20 225f 5f6d 6169 6e5f 5f22 3a0a   == "__main__":.
-00000c10: 2020 2020 6e6f 6e65 626f 742e 7275 6e28      nonebot.run(
-00000c20: 290a 6060 600a 0a23 2323 20e6 b688 e681  ).```..### .....
-00000c30: afe6 aeb5 e5b1 95e7 a4ba 0a0a e4bb a5e4  ................
-00000c40: b88b e698 afe4 b880 e4b8 aae7 ae80 e58d  ................
-00000c50: 95e7 9a84 e68f 92e4 bbb6 e7a4 bae4 be8b  ................
-00000c60: efbc 8ce5 b195 e7a4 bae5 9084 e7a7 8de6  ................
-00000c70: b688 e681 afe6 aeb5 efbc 9a0a 0a60 6060  .............```
-00000c80: 7079 7468 6f6e 0a66 726f 6d20 6e6f 6e65  python.from none
-00000c90: 626f 7420 696d 706f 7274 206f 6e5f 636f  bot import on_co
-00000ca0: 6d6d 616e 640a 6672 6f6d 206e 6f6e 6562  mmand.from noneb
-00000cb0: 6f74 2e70 6172 616d 7320 696d 706f 7274  ot.params import
-00000cc0: 2043 6f6d 6d61 6e64 4172 670a 0a66 726f   CommandArg..fro
-00000cd0: 6d20 6e6f 6e65 626f 742e 6164 6170 7465  m nonebot.adapte
-00000ce0: 7273 2e76 696c 6c61 2069 6d70 6f72 7420  rs.villa import 
-00000cf0: 426f 742c 2053 656e 644d 6573 7361 6765  Bot, SendMessage
-00000d00: 4576 656e 742c 204d 6573 7361 6765 2c20  Event, Message, 
-00000d10: 4d65 7373 6167 6553 6567 6d65 6e74 0a0a  MessageSegment..
-00000d20: 6d61 7463 6865 7220 3d20 6f6e 5f63 6f6d  matcher = on_com
-00000d30: 6d61 6e64 2827 e58f 91e9 8081 2729 0a0a  mand('......')..
-00000d40: 406d 6174 6368 6572 2e68 616e 646c 6528  @matcher.handle(
-00000d50: 290a 6173 796e 6320 6465 6620 6d61 7463  ).async def matc
-00000d60: 6865 725f 6861 6e64 6c65 7228 626f 743a  her_handler(bot:
-00000d70: 2042 6f74 2c20 6576 656e 743a 2053 656e   Bot, event: Sen
-00000d80: 644d 6573 7361 6765 4576 656e 742c 2063  dMessageEvent, c
-00000d90: 6d64 5f61 7267 3a20 4d65 7373 6167 6520  md_arg: Message 
-00000da0: 3d20 436f 6d6d 616e 6441 7267 2829 293a  = CommandArg()):
-00000db0: 0a20 2020 206d 7367 203d 204d 6573 7361  .    msg = Messa
-00000dc0: 6765 2829 0a20 2020 2061 7267 7320 3d20  ge().    args = 
-00000dd0: 636d 645f 6172 672e 6578 7472 6163 745f  cmd_arg.extract_
-00000de0: 706c 6169 6e5f 7465 7874 2829 2e73 7472  plain_text().str
-00000df0: 6970 2829 2e73 706c 6974 2827 2027 290a  ip().split(' ').
-00000e00: 2020 2020 666f 7220 6172 6720 696e 2061      for arg in a
-00000e10: 7267 733a 0a20 2020 2020 2020 2069 6620  rgs:.        if 
-00000e20: 6172 6720 3d3d 2022 e889 bee7 89b9 e688  arg == "........
-00000e30: 9122 3a0a 2020 2020 2020 2020 2020 2020  .":.            
-00000e40: 6d73 6720 2b3d 204d 6573 7361 6765 5365  msg += MessageSe
-00000e50: 676d 656e 742e 6d65 6e74 696f 6e5f 7573  gment.mention_us
-00000e60: 6572 2865 7665 6e74 2e76 696c 6c61 5f69  er(event.villa_i
-00000e70: 642c 2065 7665 6e74 2e66 726f 6d5f 7573  d, event.from_us
-00000e80: 6572 5f69 6429 0a20 2020 2020 2020 2065  er_id).        e
-00000e90: 6c69 6620 6172 6720 3d3d 2022 e889 bee7  lif arg == "....
-00000ea0: 89b9 626f 7422 3a0a 2020 2020 2020 2020  ..bot":.        
-00000eb0: 2020 2020 6d73 6720 2b3d 204d 6573 7361      msg += Messa
-00000ec0: 6765 5365 676d 656e 742e 6d65 6e74 696f  geSegment.mentio
-00000ed0: 6e5f 726f 626f 7428 290a 2020 2020 2020  n_robot().      
-00000ee0: 2020 2020 2020 2320 e79b aee5 898d e58f        # ........
-00000ef0: aae8 83bd e889 bee7 89b9 e69c bae5 99a8  ................
-00000f00: e4ba bae8 87aa e5b7 b10a 2020 2020 2020  ..........      
-00000f10: 2020 656c 6966 2061 7267 203d 3d20 22e6    elif arg == ".
-00000f20: 9687 e5ad 9722 3a0a 2020 2020 2020 2020  .....":.        
-00000f30: 2020 2020 6d73 6720 2b3d 204d 6573 7361      msg += Messa
-00000f40: 6765 5365 676d 656e 742e 7465 7874 2822  geSegment.text("
-00000f50: e696 87e5 ad97 2229 0a20 2020 2020 2020  ......").       
-00000f60: 2020 2020 2023 20e8 a1a8 e683 85e4 b99f       # .........
-00000f70: e698 afe7 94a8 7465 7874 e69d a5e5 8f91  ......text......
-00000f80: e980 81ef bc8c e4bb a55b e8a1 a8e6 8385  .........[......
-00000f90: e590 8d5d e6a0 bce5 bc8f efbc 8ce4 be8b  ...]............
-00000fa0: e5a6 824d 6573 7361 6765 5365 676d 656e  ...MessageSegmen
-00000fb0: 742e 7465 7874 2822 5be7 88b1 e5bf 835d  t.text("[......]
-00000fc0: 2229 0a20 2020 2020 2020 2065 6c69 6620  ").        elif 
-00000fd0: 6172 6720 3d3d 2022 e688 bfe9 97b4 223a  arg == "......":
-00000fe0: 0a20 2020 2020 2020 2020 2020 206d 7367  .            msg
-00000ff0: 202b 3d20 4d65 7373 6167 6553 6567 6d65   += MessageSegme
-00001000: 6e74 2e76 696c 6c61 5f72 6f6f 6d5f 6c69  nt.villa_room_li
-00001010: 6e6b 2865 7665 6e74 2e76 696c 6c61 5f69  nk(event.villa_i
-00001020: 642c 2065 7665 6e74 2e72 6f6f 6d5f 6964  d, event.room_id
-00001030: 290a 2020 2020 2020 2020 656c 6966 2061  ).        elif a
-00001040: 7267 203d 3d20 22e9 93be e68e a522 3a0a  rg == "......":.
-00001050: 2020 2020 2020 2020 2020 2020 6d73 6720              msg 
-00001060: 2b3d 204d 6573 7361 6765 5365 676d 656e  += MessageSegmen
-00001070: 742e 6c69 6e6b 2822 6874 7470 733a 2f2f  t.link("https://
-00001080: 7777 772e 6d69 796f 7573 6865 2e63 6f6d  www.miyoushe.com
-00001090: 2f79 732f 6172 7469 636c 652f 3339 3637  /ys/article/3967
-000010a0: 3033 3037 222c 2022 e8bf 99e6 98af e993  0307", "........
-000010b0: bee6 8ea5 2229 0a20 2020 2020 2020 2020  ....").         
-000010c0: 2020 2023 20e4 bdbf e794 a86c 696e 6be7     # ......link.
-000010d0: 9a84 e8af 9de9 93be e68e a5e8 83bd e5a4  ................
-000010e0: 9fe7 82b9 e587 bbe8 bf9b e8a1 8ce8 b7b3  ................
-000010f0: e8bd acef bc8c e4bd bfe7 94a8 7465 7874  ............text
-00001100: e79a 84e8 af9d e4b8 8de8 83bd e782 b9e5  ................
-00001110: 87bb 0a20 2020 2020 2020 2065 6c69 6620  ...        elif 
-00001120: 6172 6720 3d3d 2022 e59b bee7 8987 223a  arg == "......":
-00001130: 0a20 2020 2020 2020 2020 2020 206d 7367  .            msg
-00001140: 202b 3d20 4d65 7373 6167 6553 6567 6d65   += MessageSegme
-00001150: 6e74 2e69 6d61 6765 2822 6874 7470 733a  nt.image("https:
-00001160: 2f2f 7777 772e 6d69 796f 7573 6865 2e63  //www.miyoushe.c
-00001170: 6f6d 2f5f 6e75 7874 2f69 6d67 2f6d 6948  om/_nuxt/img/miH
-00001180: 6f59 6f5f 4761 6d65 2e32 3435 3737 3533  oYo_Game.2457753
-00001190: 2e70 6e67 2229 0a20 2020 2020 2020 2020  .png").         
-000011a0: 2020 2023 20e6 9a82 e697 b6e5 8faa e694     # ...........
-000011b0: afe6 8c81 7572 6ce5 9bbe e789 870a 2020  ....url.......  
-000011c0: 2020 6177 6169 7420 6d61 7463 6865 722e    await matcher.
-000011d0: 6669 6e69 7368 286d 7367 290a 6060 600a  finish(msg).```.
-000011e0: 0ae4 bdbf e794 a8e5 91bd e4bb a460 4062  .............`@b
-000011f0: 6f74 202f e58f 91e9 8081 20e8 89be e789  ot /...... .....
-00001200: b9e6 8891 20e8 89be e789 b962 6f74 20e6  .... ......bot .
-00001210: 9687 e5ad 9720 e688 bfe9 97b4 20e9 93be  ..... ...... ...
-00001220: e68e a520 e59b bee7 8987 60e6 97b6 efbc  ... ......`.....
-00001230: 8c62 6f74 e4bc 9ae5 9b9e e5a4 8d60 40e4  .bot.........`@.
-00001240: bda0 e79a 84e5 908d e5ad 9720 4062 6f74  ........... @bot
-00001250: e79a 84e5 908d e5ad 9720 e696 87e5 ad97  ......... ......
-00001260: 2023 e688 bfe9 97b4 e590 8d20 e8bf 99e6   #......... ....
-00001270: 98af e993 bee6 8ea5 20e5 9bbe e789 87e5  ........ .......
-00001280: 8685 e5ae b960 0a0a 0a23 2320 e58f 8de9  .....`...## ....
-00001290: a688 0a0a e79b aee5 898d e697 a0e8 aeba  ................
-000012a0: e698 afe5 a4a7 e588 abe9 878e 426f 74e8  ............Bot.
-000012b0: bf98 e698 afe6 9cac e980 82e9 858d e599  ................
-000012c0: a8e9 83bd e59c a8e6 b58b e8af 95e5 bc80  ................
-000012d0: e58f 91e4 b8ad efbc 8ce5 a682 e981 87e9  ................
-000012e0: 97ae e9a2 98e8 afb7 e68f 90e5 87ba 6973  ..............is
-000012f0: 7375 65ef bc8c e684 9fe8 b0a2 e694 afe6  sue.............
-00001300: 8c81 efbc 810a 0a23 2320 e79b b8e5 85b3  .......## ......
-00001310: e9a1 b9e7 9bae 0a0a 2d20 5b4e 6f6e 6542  ........- [NoneB
-00001320: 6f74 325d 2868 7474 7073 3a2f 2f67 6974  ot2](https://git
-00001330: 6875 622e 636f 6d2f 6e6f 6e65 626f 742f  hub.com/nonebot/
-00001340: 6e6f 6e65 626f 7432 2920 e99d 9ee5 b8b8  nonebot2) ......
-00001350: e5a5 bde7 94a8 e79a 8450 7974 686f 6ee8  .........Python.
-00001360: b7a8 e5b9 b3e5 8fb0 e69c bae5 99a8 e4ba  ................
-00001370: bae6 a186 e69e b6ef bc81 0a2d 205b 7669  ...........- [vi
-00001380: 6c6c 612d 7079 5d28 6874 7470 733a 2f2f  lla-py](https://
-00001390: 6769 7468 7562 2e63 6f6d 2f43 4d48 6f70  github.com/CMHop
-000013a0: 6553 756e 7368 696e 652f 7669 6c6c 612d  eSunshine/villa-
-000013b0: 7079 2920 e5a4 a7e5 88ab e987 8e42 6f74  py) .........Bot
-000013c0: 2050 7974 686f 6e20 5344 4be3 8082 0a0a   Python SDK.....
-000013d0: e68e a8e8 8d90 e69c 89e6 8890 e786 9f50  ...............P
-000013e0: 7974 686f 6ee5 bc80 e58f 91e7 bb8f e9aa  ython...........
-000013f0: 8ce4 bd86 e5af b94e 6f6e 6542 6f74 32e4  .......NoneBot2.
-00001400: b88d e786 9fe6 8289 e79a 84e5 b08f e4bc  ................
-00001410: 99e4 bcb4 e980 89e6 8ba9 60e5 a4a7 e588  ..........`.....
-00001420: abe9 878e 426f 7420 5079 7468 6f6e 2053  ....Bot Python S
-00001430: 444b 60ef bc8c 0a0a e5af b94e 6f6e 6542  DK`........NoneB
-00001440: 6f74 32e7 869f e682 89e6 8896 e5b8 8ce6  ot2.............
-00001450: 9c9b e68e a5e8 a7a6 e69b b4e6 8890 e786  ................
-00001460: 9fe7 9a84 e794 9fe6 8081 e79a 84e5 b08f  ................
-00001470: e4bc 99e4 bcb4 e980 89e6 8ba9 604e 6f6e  ............`Non
-00001480: 6542 6f74 322b e69c ace9 8082 e985 8de5  eBot2+..........
-00001490: 99a8 60e8 bf9b e8a1 8ce5 bc80 e58f 91e3  ..`.............
-000014a0: 8082 0a                                  ...
+000005e0: e8a3 850a 0ae5 9ca8 604e 6f6e 6542 6f74  ........`NoneBot
+000005f0: 3260 e9a1 b9e7 9bae e79b aee5 bd95 e4b8  2`..............
+00000600: 8be4 bdbf e794 a8e8 849a e689 8be6 9eb6  ................
+00000610: e5ae 89e8 a385 efbc 9a0a 0a60 6060 0a6e  ...........```.n
+00000620: 6220 6164 6170 7465 7220 696e 7374 616c  b adapter instal
+00000630: 6c20 6e6f 6e65 626f 742d 6164 6170 7465  l nonebot-adapte
+00000640: 722d 7669 6c6c 610a 6060 600a 0a23 2320  r-villa.```..## 
+00000650: e985 8de7 bdae 0a0a e4bf aee6 94b9 204e  .............. N
+00000660: 6f6e 6542 6f74 20e9 858d e7bd aee6 9687  oneBot .........
+00000670: e4bb b620 602e 656e 7660 20e6 8896 e880  ... `.env` .....
+00000680: 8520 602e 656e 762e 2a60 e380 820a 0a23  . `.env.*`.....#
+00000690: 2323 2044 7269 7665 720a 0ae6 9cac e980  ## Driver.......
+000006a0: 82e9 858d e599 a8e5 908c e697 b6e9 9c80  ................
+000006b0: e8a6 8160 5265 7665 7273 6544 7269 7665  ...`ReverseDrive
+000006c0: 7260 e592 8c60 466f 7277 6172 6444 7269  r`...`ForwardDri
+000006d0: 7665 7260 efbc 8ce5 8f82 e880 8320 5b64  ver`......... [d
+000006e0: 7269 7665 725d 2868 7474 7073 3a2f 2f76  river](https://v
+000006f0: 322e 6e6f 6e65 626f 742e 6465 762f 646f  2.nonebot.dev/do
+00000700: 6373 2f6e 6578 742f 6164 7661 6e63 6564  cs/next/advanced
+00000710: 2f64 7269 7665 7223 2545 3925 4139 2542  /driver#%E9%A9%B
+00000720: 3125 4535 2538 4125 4138 2545 3525 3939  1%E5%8A%A8%E5%99
+00000730: 2541 3825 4537 2542 3125 4242 2545 3525  %A8%E7%B1%BB%E5%
+00000740: 3945 2538 4229 20e9 858d e7bd aee9 a1b9  9E%8B) .........
+00000750: e380 820a 0ae4 be8b e5a6 82ef bc9a 0a0a  ................
+00000760: 6060 6064 6f74 656e 760a 4452 4956 4552  ```dotenv.DRIVER
+00000770: 3d7e 6661 7374 6170 692b 7e68 7474 7078  =~fastapi+~httpx
+00000780: 0a60 6060 0a0a 2323 2320 5649 4c4c 415f  .```..### VILLA_
+00000790: 424f 5453 0a0a e985 8de7 bdae e69c bae5  BOTS............
+000007a0: 99a8 e4ba bae5 b890 e58f b7e5 8897 e8a1  ................
+000007b0: a8ef bc8c e6af 8fe4 b8aa 626f 74e6 9c89  ..........bot...
+000007c0: 33e4 b8aa e5bf 85e5 a1ab e985 8de7 bdae  3...............
+000007d0: efbc 8ce5 9ca8 e5a4 a7e5 88ab e987 8ee5  ................
+000007e0: ae98 e696 b9e6 9cba e599 a8e4 baba e5bc  ................
+000007f0: 80e5 8f91 e880 85e7 a4be e58c ba28 e588  .............(..
+00000800: abe9 878e 4944 3a20 4f70 656e 5669 6c6c  ....ID: OpenVill
+00000810: 6129 e794 b3e8 afb7 e697 b6e8 8eb7 e5be  a)..............
+00000820: 97ef bc8c 0a0a 2d20 626f 745f 6964 3a20  ......- bot_id: 
+00000830: e69c bae5 99a8 e4ba ba69 64ef bc8c e4bb  .........id.....
+00000840: a560 626f 745f 60e5 bc80 e5a4 b40a 2d20  .`bot_`.......- 
+00000850: 626f 745f 7365 6372 6574 3a20 e69c bae5  bot_secret: ....
+00000860: 99a8 e4ba bae5 af86 e992 a50a 2d20 6361  ............- ca
+00000870: 6c6c 6261 636b 5f75 726c 3a20 6874 7470  llback_url: http
+00000880: e59b 9ee8 b083 e59c b0e5 9d80 efbc 8ce4  ................
+00000890: be8b e5a6 82e7 94b3 e8af b762 6f74 e697  ...........bot..
+000008a0: b6e7 bb99 e79a 84e5 9b9e e8b0 83e5 9cb0  ................
+000008b0: e59d 80e6 98af 6068 7474 703a 2f2f e59f  ......`http://..
+000008c0: 9fe5 908d 2f79 6f75 722f 6361 6c6c 6261  ..../your/callba
+000008d0: 636b 2f75 726c 60ef bc8c e982 a3e4 b988  ck/url`.........
+000008e0: e985 8de7 bdae e987 8ce7 9a84 6063 616c  ............`cal
+000008f0: 6c62 6163 6b5f 7572 6c60 e5a1 abe5 8699  lback_url`......
+00000900: 602f 796f 7572 2f63 616c 6c62 6163 6b2f  `/your/callback/
+00000910: 7572 6c60 0a20 20e4 be8b e5a6 82ef bc9a  url`.  .........
+00000920: 0a0a 6060 6064 6f74 656e 760a 5649 4c4c  ..```dotenv.VILL
+00000930: 415f 424f 5453 3d27 0a5b 0a20 207b 0a20  A_BOTS='.[.  {. 
+00000940: 2020 2022 626f 745f 6964 223a 2022 626f     "bot_id": "bo
+00000950: 745f 3132 3334 3536 3738 3922 2c0a 2020  t_123456789",.  
+00000960: 2020 2262 6f74 5f73 6563 7265 7422 3a20    "bot_secret": 
+00000970: 2261 6263 3132 3364 6566 3435 3622 2c0a  "abc123def456",.
+00000980: 2020 2020 2263 616c 6c62 6163 6b5f 7572      "callback_ur
+00000990: 6c22 3a20 222f 796f 7572 2f63 616c 6c62  l": "/your/callb
+000009a0: 6163 6b2f 7572 6c22 0a20 207d 0a5d 0a27  ack/url".  }.].'
+000009b0: 0a60 6060 0a0a 2323 20e7 a4ba e4be 8b0a  .```..## .......
+000009c0: 0a23 2323 20e6 b688 e681 afe6 aeb5 e5b1  .### ...........
+000009d0: 95e7 a4ba 0a0a e4bb a5e4 b88b e698 afe4  ................
+000009e0: b880 e4b8 aae7 ae80 e58d 95e7 9a84 e68f  ................
+000009f0: 92e4 bbb6 e7a4 bae4 be8b efbc 8ce5 b195  ................
+00000a00: e7a4 bae5 9084 e7a7 8de6 b688 e681 afe6  ................
+00000a10: aeb5 efbc 9a0a 0a60 6060 7079 7468 6f6e  .......```python
+00000a20: 0a66 726f 6d20 6e6f 6e65 626f 7420 696d  .from nonebot im
+00000a30: 706f 7274 206f 6e5f 636f 6d6d 616e 640a  port on_command.
+00000a40: 6672 6f6d 206e 6f6e 6562 6f74 2e70 6172  from nonebot.par
+00000a50: 616d 7320 696d 706f 7274 2043 6f6d 6d61  ams import Comma
+00000a60: 6e64 4172 670a 0a66 726f 6d20 6e6f 6e65  ndArg..from none
+00000a70: 626f 742e 6164 6170 7465 7273 2e76 696c  bot.adapters.vil
+00000a80: 6c61 2069 6d70 6f72 7420 426f 742c 2053  la import Bot, S
+00000a90: 656e 644d 6573 7361 6765 4576 656e 742c  endMessageEvent,
+00000aa0: 204d 6573 7361 6765 2c20 4d65 7373 6167   Message, Messag
+00000ab0: 6553 6567 6d65 6e74 0a0a 6d61 7463 6865  eSegment..matche
+00000ac0: 7220 3d20 6f6e 5f63 6f6d 6d61 6e64 2827  r = on_command('
+00000ad0: e58f 91e9 8081 2729 0a0a 406d 6174 6368  ......')..@match
+00000ae0: 6572 2e68 616e 646c 6528 290a 6173 796e  er.handle().asyn
+00000af0: 6320 6465 6620 6d61 7463 6865 725f 6861  c def matcher_ha
+00000b00: 6e64 6c65 7228 626f 743a 2042 6f74 2c20  ndler(bot: Bot, 
+00000b10: 6576 656e 743a 2053 656e 644d 6573 7361  event: SendMessa
+00000b20: 6765 4576 656e 742c 2063 6d64 5f61 7267  geEvent, cmd_arg
+00000b30: 3a20 4d65 7373 6167 6520 3d20 436f 6d6d  : Message = Comm
+00000b40: 616e 6441 7267 2829 293a 0a20 2020 206d  andArg()):.    m
+00000b50: 7367 203d 204d 6573 7361 6765 2829 0a20  sg = Message(). 
+00000b60: 2020 2061 7267 7320 3d20 636d 645f 6172     args = cmd_ar
+00000b70: 672e 6578 7472 6163 745f 706c 6169 6e5f  g.extract_plain_
+00000b80: 7465 7874 2829 2e73 7472 6970 2829 2e73  text().strip().s
+00000b90: 706c 6974 2827 2027 290a 2020 2020 666f  plit(' ').    fo
+00000ba0: 7220 6172 6720 696e 2061 7267 733a 0a20  r arg in args:. 
+00000bb0: 2020 2020 2020 2069 6620 6172 6720 3d3d         if arg ==
+00000bc0: 2022 e889 bee7 89b9 e688 9122 3a0a 2020   ".........":.  
+00000bd0: 2020 2020 2020 2020 2020 6d73 6720 2b3d            msg +=
+00000be0: 204d 6573 7361 6765 5365 676d 656e 742e   MessageSegment.
+00000bf0: 6d65 6e74 696f 6e5f 7573 6572 2865 7665  mention_user(eve
+00000c00: 6e74 2e76 696c 6c61 5f69 642c 2065 7665  nt.villa_id, eve
+00000c10: 6e74 2e66 726f 6d5f 7573 6572 5f69 6429  nt.from_user_id)
+00000c20: 0a20 2020 2020 2020 2065 6c69 6620 6172  .        elif ar
+00000c30: 6720 3d3d 2022 e889 bee7 89b9 626f 7422  g == "......bot"
+00000c40: 3a0a 2020 2020 2020 2020 2020 2020 6d73  :.            ms
+00000c50: 6720 2b3d 204d 6573 7361 6765 5365 676d  g += MessageSegm
+00000c60: 656e 742e 6d65 6e74 696f 6e5f 726f 626f  ent.mention_robo
+00000c70: 7428 626f 742e 7365 6c66 5f69 642c 2062  t(bot.self_id, b
+00000c80: 6f74 2e6e 6963 6b6e 616d 6529 0a20 2020  ot.nickname).   
+00000c90: 2020 2020 2065 6c69 6620 6172 6720 3d3d       elif arg ==
+00000ca0: 2022 e696 87e5 ad97 223a 0a20 2020 2020   "......":.     
+00000cb0: 2020 2020 2020 206d 7367 202b 3d20 4d65         msg += Me
+00000cc0: 7373 6167 6553 6567 6d65 6e74 2e74 6578  ssageSegment.tex
+00000cd0: 7428 22e6 9687 e5ad 9722 290a 2020 2020  t("......").    
+00000ce0: 2020 2020 2020 2020 2320 e8a1 a8e6 8385          # ......
+00000cf0: e4b9 9fe6 98af e794 a874 6578 74e6 9da5  .........text...
+00000d00: e58f 91e9 8081 efbc 8ce4 bba5 5be8 a1a8  ............[...
+00000d10: e683 85e5 908d 5de6 a0bc e5bc 8fef bc8c  ......].........
+00000d20: e4be 8be5 a682 4d65 7373 6167 6553 6567  ......MessageSeg
+00000d30: 6d65 6e74 2e74 6578 7428 225b e788 b1e5  ment.text("[....
+00000d40: bf83 5d22 290a 2020 2020 2020 2020 656c  ..]").        el
+00000d50: 6966 2061 7267 203d 3d20 22e6 88bf e997  if arg == ".....
+00000d60: b422 3a0a 2020 2020 2020 2020 2020 2020  .":.            
+00000d70: 6d73 6720 2b3d 204d 6573 7361 6765 5365  msg += MessageSe
+00000d80: 676d 656e 742e 726f 6f6d 5f6c 696e 6b28  gment.room_link(
+00000d90: 6576 656e 742e 7669 6c6c 615f 6964 2c20  event.villa_id, 
+00000da0: 6576 656e 742e 726f 6f6d 5f69 6429 0a20  event.room_id). 
+00000db0: 2020 2020 2020 2065 6c69 6620 6172 6720         elif arg 
+00000dc0: 3d3d 2022 e993 bee6 8ea5 223a 0a20 2020  == "......":.   
+00000dd0: 2020 2020 2020 2020 206d 7367 202b 3d20           msg += 
+00000de0: 4d65 7373 6167 6553 6567 6d65 6e74 2e6c  MessageSegment.l
+00000df0: 696e 6b28 2268 7474 7073 3a2f 2f77 7777  ink("https://www
+00000e00: 2e6d 6979 6f75 7368 652e 636f 6d2f 7973  .miyoushe.com/ys
+00000e10: 2f61 7274 6963 6c65 2f33 3936 3730 3330  /article/3967030
+00000e20: 3722 2c20 7368 6f77 5f74 6578 743d 22e8  7", show_text=".
+00000e30: bf99 e698 afe9 93be e68e a522 290a 2020  ...........").  
+00000e40: 2020 2020 2020 2020 2020 2320 e4bd bfe7            # ....
+00000e50: 94a8 6c69 6e6b e79a 84e8 af9d e993 bee6  ..link..........
+00000e60: 8ea5 e883 bde5 a49f e782 b9e5 87bb e8bf  ................
+00000e70: 9be8 a18c e8b7 b3e8 bdac efbc 8ce4 bdbf  ................
+00000e80: e794 a874 6578 74e7 9a84 e8af 9de4 b88d  ...text.........
+00000e90: e883 bde7 82b9 e587 bb0a 2020 2020 2020  ..........      
+00000ea0: 2020 2020 2020 2320 7368 6f77 5f74 6578        # show_tex
+00000eb0: 74e6 98af e68c 87e9 93be e68e a5e6 98be  t...............
+00000ec0: e7a4 bae7 9a84 e696 87e5 ad97 efbc 8ce4  ................
+00000ed0: bd86 e59c a8e5 bd93 e589 8de7 8988 e69c  ................
+00000ee0: ac57 6562 e7ab afe5 a4a7 e588 abe9 878e  .Web............
+00000ef0: e4bc 9ae6 97a0 e6b3 95e6 ada3 e5b8 b8e8  ................
+00000f00: b7b3 e8bd acef bc8c e69c 80e5 a5bd e4b8  ................
+00000f10: 8de4 bdbf e794 a8e8 afa5 e58f 82e6 95b0  ................
+00000f20: 0a20 2020 2020 2020 2065 6c69 6620 6172  .        elif ar
+00000f30: 6720 3d3d 2022 e59b bee7 8987 223a 0a20  g == "......":. 
+00000f40: 2020 2020 2020 2020 2020 206d 7367 202b             msg +
+00000f50: 3d20 4d65 7373 6167 6553 6567 6d65 6e74  = MessageSegment
+00000f60: 2e69 6d61 6765 2822 6874 7470 733a 2f2f  .image("https://
+00000f70: 7777 772e 6d69 796f 7573 6865 2e63 6f6d  www.miyoushe.com
+00000f80: 2f5f 6e75 7874 2f69 6d67 2f6d 6948 6f59  /_nuxt/img/miHoY
+00000f90: 6f5f 4761 6d65 2e32 3435 3737 3533 2e70  o_Game.2457753.p
+00000fa0: 6e67 2229 0a20 2020 2020 2020 2020 2020  ng").           
+00000fb0: 2023 20e6 9a82 e697 b6e5 8faa e694 afe6   # .............
+00000fc0: 8c81 7572 6ce5 9bbe e789 87ef bc8c e4bd  ..url...........
+00000fd0: 86e5 9ca8 e5bd 93e5 898d e789 88e6 9cac  ................
+00000fe0: 7765 62e7 abaf e697 a0e6 b395 e698 bee7  web.............
+00000ff0: a4ba e59b bee7 8987 efbc 8ce5 be85 e5ae  ................
+00001000: 98e6 96b9 e590 8ee7 bbad e4bf aee5 a48d  ................
+00001010: 0a20 2020 2061 7761 6974 206d 6174 6368  .    await match
+00001020: 6572 2e66 696e 6973 6828 6d73 6729 0a60  er.finish(msg).`
+00001030: 6060 0a0a e4bd bfe7 94a8 e591 bde4 bba4  ``..............
+00001040: 6040 626f 7420 2fe5 8f91 e980 8120 e889  `@bot /...... ..
+00001050: bee7 89b9 e688 9120 e889 bee7 89b9 626f  ....... ......bo
+00001060: 7420 e696 87e5 ad97 20e6 88bf e997 b420  t ...... ...... 
+00001070: e993 bee6 8ea5 20e5 9bbe e789 8760 e697  ...... ......`..
+00001080: b6ef bc8c 626f 74e4 bc9a e59b 9ee5 a48d  ....bot.........
+00001090: 6040 e4bd a0e7 9a84 e590 8de5 ad97 2040  `@............ @
+000010a0: 626f 74e7 9a84 e590 8de5 ad97 20e6 9687  bot......... ...
+000010b0: e5ad 9720 23e6 88bf e997 b4e5 908d 20e8  ... #......... .
+000010c0: bf99 e698 afe9 93be e68e a520 e59b bee7  ........... ....
+000010d0: 8987 e586 85e5 aeb9 600a 0a0a 2323 20e4  ........`...## .
+000010e0: baa4 e6b5 81e5 928c e58f 8de9 a688 0a0a  ................
+000010f0: e79b aee5 898d e697 a0e8 aeba e698 afe5  ................
+00001100: a4a7 e588 abe9 878e 426f 74e8 bf98 e698  ........Bot.....
+00001110: afe6 9cac e980 82e9 858d e599 a8e9 83bd  ................
+00001120: e59c a8e6 b58b e8af 95e5 bc80 e58f 91e4  ................
+00001130: b8ad efbc 8ce5 a682 e981 87e9 97ae e9a2  ................
+00001140: 98e8 afb7 e68f 90e5 87ba 6973 7375 65ef  ..........issue.
+00001150: bc8c e684 9fe8 b0a2 e694 afe6 8c81 efbc  ................
+00001160: 810a 0ae4 b99f e6ac a2e8 bf8e e69d a5e6  ................
+00001170: 8891 e79a 84e5 a4a7 e588 abe9 878e e380  ................
+00001180: 90e5 b098 e4b8 96e9 97b2 e6b8 b8e3 8091  ................
+00001190: e8bf 9be8 a18c e4ba a4e6 b581 efbc 9a0a  ................
+000011a0: 0a2d 20e5 a4a7 e588 abe9 878e 4944 3a20  .- .........ID: 
+000011b0: 7767 694a 4e61 55ef bc8c e58f afe6 909c  wgiJNaU.........
+000011c0: e7b4 a2e5 8aa0 e585 a50a 2d20 5b57 6562  ..........- [Web
+000011d0: e7ab afe9 93be e68e a55d 2868 7474 7073  .........](https
+000011e0: 3a2f 2f64 6279 2e6d 6979 6f75 7368 652e  ://dby.miyoushe.
+000011f0: 636f 6d2f 6368 6174 2f31 3034 372f 3231  com/chat/1047/21
+00001200: 3635 3229 efbc 8ce7 9bae e589 8de4 bb85  652)............
+00001210: 5043 e7ab afe5 8faf e8ae bfe9 97ae 0a0a  PC..............
+00001220: 2323 20e7 9bb8 e585 b3e9 a1b9 e79b ae0a  ## .............
+00001230: 0a2d 205b 4e6f 6e65 426f 7432 5d28 6874  .- [NoneBot2](ht
+00001240: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
+00001250: 2f6e 6f6e 6562 6f74 2f6e 6f6e 6562 6f74  /nonebot/nonebot
+00001260: 3229 3a20 e99d 9ee5 b8b8 e5a5 bde7 94a8  2): ............
+00001270: e79a 8450 7974 686f 6ee8 b7a8 e5b9 b3e5  ...Python.......
+00001280: 8fb0 e69c bae5 99a8 e4ba bae6 a186 e69e  ................
+00001290: b6ef bc81 0a2d 205b 7669 6c6c 612d 7079  .....- [villa-py
+000012a0: 5d28 6874 7470 733a 2f2f 6769 7468 7562  ](https://github
+000012b0: 2e63 6f6d 2f43 4d48 6f70 6553 756e 7368  .com/CMHopeSunsh
+000012c0: 696e 652f 7669 6c6c 612d 7079 293a 20e5  ine/villa-py): .
+000012d0: a4a7 e588 abe9 878e 2042 6f74 2050 7974  ........ Bot Pyt
+000012e0: 686f 6e20 5344 4be3 8082 0a0a e68e a8e8  hon SDK.........
+000012f0: 8d90 e69c 89e6 8890 e786 9f50 7974 686f  ...........Pytho
+00001300: 6ee5 bc80 e58f 91e7 bb8f e9aa 8ce4 bd86  n...............
+00001310: e5af b94e 6f6e 6542 6f74 32e4 b88d e786  ...NoneBot2.....
+00001320: 9fe6 8289 e79a 84e5 b08f e4bc 99e4 bcb4  ................
+00001330: e980 89e6 8ba9 60e5 a4a7 e588 abe9 878e  ......`.........
+00001340: 426f 7420 5079 7468 6f6e 2053 444b 60ef  Bot Python SDK`.
+00001350: bc8c 0a0a e5af b94e 6f6e 6542 6f74 32e7  .......NoneBot2.
+00001360: 869f e682 89e6 8896 e5b8 8ce6 9c9b e68e  ................
+00001370: a5e8 a7a6 e69b b4e6 8890 e786 9fe7 9a84  ................
+00001380: e794 9fe6 8081 e79a 84e5 b08f e4bc 99e4  ................
+00001390: bcb4 e980 89e6 8ba9 604e 6f6e 6542 6f74  ........`NoneBot
+000013a0: 322b e69c ace9 8082 e985 8de5 99a8 60e8  2+............`.
+000013b0: bf9b e8a1 8ce5 bc80 e58f 91e3 8082 0a    ...............
```

