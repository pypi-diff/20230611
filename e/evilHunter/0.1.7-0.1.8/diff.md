# Comparing `tmp/evilHunter-0.1.7.tar.gz` & `tmp/evilHunter-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "evilHunter-0.1.7.tar", last modified: Sat Jun 10 09:34:38 2023, max compression
+gzip compressed data, was "evilHunter-0.1.8.tar", last modified: Sun Jun 11 19:13:55 2023, max compression
```

## Comparing `evilHunter-0.1.7.tar` & `evilHunter-0.1.8.tar`

### file list

```diff
@@ -1,12 +1,13 @@
-drwxr-xr-x   0 supervisor  (1000) supervisor  (1000)        0 2023-06-10 09:34:38.524323 evilHunter-0.1.7/
--rw-r--r--   0 supervisor  (1000) supervisor  (1000)     1673 2023-06-10 09:34:38.524323 evilHunter-0.1.7/PKG-INFO
--rw-r--r--   0 supervisor  (1000) supervisor  (1000)     1440 2023-06-09 11:15:59.000000 evilHunter-0.1.7/README.md
-drwxr-xr-x   0 supervisor  (1000) supervisor  (1000)        0 2023-06-10 09:34:38.524323 evilHunter-0.1.7/evilHunter.egg-info/
--rw-r--r--   0 supervisor  (1000) supervisor  (1000)     1673 2023-06-10 09:34:38.000000 evilHunter-0.1.7/evilHunter.egg-info/PKG-INFO
--rw-r--r--   0 supervisor  (1000) supervisor  (1000)      201 2023-06-10 09:34:38.000000 evilHunter-0.1.7/evilHunter.egg-info/SOURCES.txt
--rw-r--r--   0 supervisor  (1000) supervisor  (1000)        1 2023-06-10 09:34:38.000000 evilHunter-0.1.7/evilHunter.egg-info/dependency_links.txt
--rw-r--r--   0 supervisor  (1000) supervisor  (1000)        9 2023-06-10 09:34:38.000000 evilHunter-0.1.7/evilHunter.egg-info/requires.txt
--rw-r--r--   0 supervisor  (1000) supervisor  (1000)        6 2023-06-10 09:34:38.000000 evilHunter-0.1.7/evilHunter.egg-info/top_level.txt
--rw-r--r--   0 supervisor  (1000) supervisor  (1000)    15538 2023-06-10 09:31:04.000000 evilHunter-0.1.7/evilHunter.py
--rw-r--r--   0 supervisor  (1000) supervisor  (1000)       38 2023-06-10 09:34:38.524323 evilHunter-0.1.7/setup.cfg
--rw-r--r--   0 supervisor  (1000) supervisor  (1000)      520 2023-06-10 09:34:34.000000 evilHunter-0.1.7/setup.py
+drwxr-xr-x   0 supervisor  (1000) supervisor  (1000)        0 2023-06-11 19:13:55.893834 evilHunter-0.1.8/
+-rw-r--r--   0 supervisor  (1000) supervisor  (1000)     1931 2023-06-11 19:13:55.893834 evilHunter-0.1.8/PKG-INFO
+-rw-r--r--   0 supervisor  (1000) supervisor  (1000)     1698 2023-06-11 19:05:39.000000 evilHunter-0.1.8/README.md
+-rw-r--r--   0 supervisor  (1000) supervisor  (1000)     3858 2023-06-11 18:47:15.000000 evilHunter-0.1.8/evilCracker.py
+drwxr-xr-x   0 supervisor  (1000) supervisor  (1000)        0 2023-06-11 19:13:55.893834 evilHunter-0.1.8/evilHunter.egg-info/
+-rw-r--r--   0 supervisor  (1000) supervisor  (1000)     1931 2023-06-11 19:13:55.000000 evilHunter-0.1.8/evilHunter.egg-info/PKG-INFO
+-rw-r--r--   0 supervisor  (1000) supervisor  (1000)      216 2023-06-11 19:13:55.000000 evilHunter-0.1.8/evilHunter.egg-info/SOURCES.txt
+-rw-r--r--   0 supervisor  (1000) supervisor  (1000)        1 2023-06-11 19:13:55.000000 evilHunter-0.1.8/evilHunter.egg-info/dependency_links.txt
+-rw-r--r--   0 supervisor  (1000) supervisor  (1000)        9 2023-06-11 19:13:55.000000 evilHunter-0.1.8/evilHunter.egg-info/requires.txt
+-rw-r--r--   0 supervisor  (1000) supervisor  (1000)        6 2023-06-11 19:13:55.000000 evilHunter-0.1.8/evilHunter.egg-info/top_level.txt
+-rw-r--r--   0 supervisor  (1000) supervisor  (1000)    17885 2023-06-11 18:55:40.000000 evilHunter-0.1.8/evilHunter.py
+-rw-r--r--   0 supervisor  (1000) supervisor  (1000)       38 2023-06-11 19:13:55.893834 evilHunter-0.1.8/setup.cfg
+-rw-r--r--   0 supervisor  (1000) supervisor  (1000)      538 2023-06-11 19:13:47.000000 evilHunter-0.1.8/setup.py
```

### Comparing `evilHunter-0.1.7/PKG-INFO` & `evilHunter-0.1.8/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,28 +1,36 @@
 Metadata-Version: 2.1
 Name: evilHunter
-Version: 0.1.7
+Version: 0.1.8
 Summary: Cracking WiFi(Hanshake)
 Home-page: https://github.com/an0mal1a/evilHunter
 Author: an0mal1a
 Author-email: pablodiez024@proton.me
 Description-Content-Type: text/markdown
 
 # evilHunter
 
 
 
 Argumentos:
     
     OBLIGATORIO
         
-        [♦] evilHunter -w /path/to/wordlists
+        [♦] evilHunter [-w /path/to/wordlists] [-b 12 (passwd length)] [-t 400 (Nº of threads)]
         
-            (-w / -wordlist)
-              (-h / --help)
+            (-w / --wordlist)
+                [♦] -w /path/to/wordlists
+
+            (-b / --brute)
+                [♦] -b passwd_length
+
+            (-t / --threads)
+                [♦] -t Nº_of_threads
+
+            (-h / --help)
               
 # INSTALACIÓN:
 
 PyPi: (https://pypi.org/project/evilHunter/)
 
     command_line = pip install evilHunter
 
@@ -67,10 +75,10 @@
     3. A la vez que estamos escaneando esa red fijando la tarjeta de
         red en el mismo cana, enviamos paquetes de deautenticación 
         
 
     4. Una véz capturado el handshake, abrimos el archivo .cap y
         con diccionary attack crackeamos la contraseña.
 
-# _Proximamente_:
+# _Proximas mejoras_
 
-                [♦]  Brute Force Crack
+                [♦]  Brute Force (Password Generator) Faster
```

### Comparing `evilHunter-0.1.7/README.md` & `evilHunter-0.1.8/README.md`

 * *Files 19% similar despite different names*

```diff
@@ -2,18 +2,26 @@
 
 
 
 Argumentos:
     
     OBLIGATORIO
         
-        [♦] evilHunter -w /path/to/wordlists
+        [♦] evilHunter [-w /path/to/wordlists] [-b 12 (passwd length)] [-t 400 (Nº of threads)]
         
-            (-w / -wordlist)
-              (-h / --help)
+            (-w / --wordlist)
+                [♦] -w /path/to/wordlists
+
+            (-b / --brute)
+                [♦] -b passwd_length
+
+            (-t / --threads)
+                [♦] -t Nº_of_threads
+
+            (-h / --help)
               
 # INSTALACIÓN:
 
 PyPi: (https://pypi.org/project/evilHunter/)
 
     command_line = pip install evilHunter
 
@@ -58,10 +66,10 @@
     3. A la vez que estamos escaneando esa red fijando la tarjeta de
         red en el mismo cana, enviamos paquetes de deautenticación 
         
 
     4. Una véz capturado el handshake, abrimos el archivo .cap y
         con diccionary attack crackeamos la contraseña.
 
-# _Proximamente_:
+# _Proximas mejoras_
 
-                [♦]  Brute Force Crack
+                [♦]  Brute Force (Password Generator) Faster
```

### Comparing `evilHunter-0.1.7/evilHunter.egg-info/PKG-INFO` & `evilHunter-0.1.8/evilHunter.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,28 +1,36 @@
 Metadata-Version: 2.1
 Name: evilHunter
-Version: 0.1.7
+Version: 0.1.8
 Summary: Cracking WiFi(Hanshake)
 Home-page: https://github.com/an0mal1a/evilHunter
 Author: an0mal1a
 Author-email: pablodiez024@proton.me
 Description-Content-Type: text/markdown
 
 # evilHunter
 
 
 
 Argumentos:
     
     OBLIGATORIO
         
-        [♦] evilHunter -w /path/to/wordlists
+        [♦] evilHunter [-w /path/to/wordlists] [-b 12 (passwd length)] [-t 400 (Nº of threads)]
         
-            (-w / -wordlist)
-              (-h / --help)
+            (-w / --wordlist)
+                [♦] -w /path/to/wordlists
+
+            (-b / --brute)
+                [♦] -b passwd_length
+
+            (-t / --threads)
+                [♦] -t Nº_of_threads
+
+            (-h / --help)
               
 # INSTALACIÓN:
 
 PyPi: (https://pypi.org/project/evilHunter/)
 
     command_line = pip install evilHunter
 
@@ -67,10 +75,10 @@
     3. A la vez que estamos escaneando esa red fijando la tarjeta de
         red en el mismo cana, enviamos paquetes de deautenticación 
         
 
     4. Una véz capturado el handshake, abrimos el archivo .cap y
         con diccionary attack crackeamos la contraseña.
 
-# _Proximamente_:
+# _Proximas mejoras_
 
-                [♦]  Brute Force Crack
+                [♦]  Brute Force (Password Generator) Faster
```

### Comparing `evilHunter-0.1.7/evilHunter.py` & `evilHunter-0.1.8/evilHunter.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,41 +1,47 @@
 #!/bin/python3
-import pywifi as pywifi
+import string
 
 try:
     print("\n[*] Starting...")
     print("\n\t[*] Comprobando librerias...")
     import colorama
     from colorama import Fore
     import os
     import time
     import re
     import subprocess
     import threading
     import multiprocessing
     import os
     import argparse
+    import evilCracker
     time.sleep(1)
-    print(Fore.GREEN + "\n\t[*] " + Fore.YELLOW + "Librerias importadas correctamente...")
+    print(Fore.GREEN + "\n[*] " + Fore.YELLOW + "Librerias importadas correctamente...\n" + Fore.RESET)
 
 except ModuleNotFoundError as e:
     print("\n\n[!] Faltan modulos necesario para la ejecucion...\n\t%s" % e)
     print("[!] Exiting...")
     exit(1)
 
 # Solicionar <lenght:
 
 def delete_files():
-    os.system('find captures -type f ! -name "*.cap" -delete')
+    os.system('find captures -type f ! -name "*.cap" -delete > /dev/null')
+    os.system('rm espec/*')
 
 
 def restart_net():
     os.system("service networking restart > /dev/null")
     os.system("service NetworkManager restart > /dev/null")
-# COMPROBAR SI EL ARGUMENTO -w FUNCIONA Y SE COMPRUEBA
+
+
+def stop_monitoring():
+    if os.system("airmon-ng stop {}mon > /dev/null".format(choosed_interface)) != 0:
+        os.system("airmon-ng stop {} > /dev/null".format(choosed_interface))
 
 
 def exiting(err):
     if err:
         if err == "True":
             print(Fore.YELLOW + "\n[*] " + Fore.RED + "Exiting due a error...\n\n" + err)
 
@@ -48,16 +54,15 @@
     print(
         Fore.WHITE + "\n  ·  ·  ·  · " + Fore.YELLOW + "[*] " +
                         Fore.LIGHTCYAN_EX + "Restarting network services"
         + Fore.YELLOW +Fore.WHITE + "\n  ·  ·  ·  · " + "[*] " +
                         Fore.LIGHTCYAN_EX + "Stopping monitor mode..." + Fore.RESET)
 
     try:
-        if os.system("airmon-ng stop {}mon > /dev/null".format(choosed_interface)) != 0:
-            os.system("airmon-ng stop {} > /dev/null".format(choosed_interface))
+        stop_monitoring()
     except NameError:
         pass
 
     print(Fore.WHITE + "  ·  ·  ·  · " + Fore.YELLOW + "[*] " + Fore.LIGHTCYAN_EX + "Deleting some files..."
           + Fore.RESET)
 
     restart_net()
@@ -259,24 +264,28 @@
 
         for itera in data:
             num += 1
             if itera not in obetives:
                 obetives.append(itera)
 
         info = "  ".join(obetives)
-
+        n_d = 0
         if re.findall("-[0-9]+", info):
             encription = re.findall("WPA[0-9]  [A-Z]+  +[A-Z]+", info)
 
             if not encription:
                 continue
 
             channel = info.split()[info.split().index("WPA2") - 2]
             name = info.split()[info.split().index("WPA2") + 3]
 
+            if re.findall("^(<length:*)", name):
+                name = f"N/D_{n_d}"
+                n_d += 1
+
             dict[name] = {"bssid": bssid,
                           "encription_type": encription[0],
                           "channel": channel}
 
         else:
             continue
     print_process_data(dict, args)
@@ -323,15 +332,15 @@
     file = None
 
     while not file:
         file = input(Fore.YELLOW + "\n\t[" + Fore.RED + "S" + Fore.YELLOW + "] " + Fore.LIGHTCYAN_EX +
                                                     "Enter the name of the file to save [E.j capture1] > ")
 
         if os.system("find captures/{}/{}* 2>/dev/null 1>/dev/null".format(network_to_attack, file)) == 0:
-            print(Fore.RED + "\n\t[!] " + Fore.YELLOW + "Este nombre ya esta usado por algún archivo.")
+            print(Fore.RED + "\n\t\t[!] " + Fore.YELLOW + "Este nombre ya esta usado por algún archivo.")
             file = None
 
 
     # Definimos bssid y channel
     bssid = dict[network_to_attack]['bssid']
     ch = dict[network_to_attack]['channel']
     # Leer handshake
@@ -342,15 +351,14 @@
     time.sleep(1)
     print(Fore.YELLOW + "\n[*] " + Fore.LIGHTRED_EX + "INICIANDO:" + Fore.LIGHTCYAN_EX + " Captura de " +
           Fore.RED + 'WPA handshake ' + Fore.LIGHTCYAN_EX +
           Fore.YELLOW + "ESPERE... --->  " + Fore.LIGHTCYAN_EX + "[CTRL + C] to stop manually..." + Fore.RESET)
 
     input(Fore.YELLOW + "\n\t\t[ENTER] To continue\n")
 
-
     capture = multiprocessing.Process(target=capture_handshake(direc, args, bssid, ch, file, network_to_attack))
 
     # Iniciamos la captura del handshake y envio de deauth
     capture.start()
 
     # Juntamos para detener
     capture.join()
@@ -392,21 +400,29 @@
     return wordlists
 
 
 def crack_handshake(direc, args, file):
     # Buscamos arhchivo .cap
     os.system("find {}/{}*.cap > espec/capture_file ".format(direc, file))
 
-    # Comprobamos si nos ha pasasdo discionario y si existe en su sistema
-    wordlist = find_wordlists(args.wordlist)
-
     # Abrimos el capture_file donde se encuentra la ruta hacia  el .cap
     with open("espec/capture_file", "r") as file:
         file = file.read().strip()
 
+    # Comprobamos si nos ha pasasdo discionario y si existe en su sistema o si quiere brute
+    if args.wordlist:
+        wordlist = find_wordlists(args.wordlist)
+
+    elif args.brute:
+        if args.threads:
+            evilCracker.startbrute(file, args.brute, args.threads)
+        else:
+            evilCracker.startbrute(file, args.brute, 200)
+        exiting(err="done")
+
     print(Fore.YELLOW + "\n\t[!] " + Fore.LIGHTCYAN_EX + "Abriendo archivo '.cap'\n" + Fore.RESET)
     # input(Fore.LIGHTCYAN_EX + "\n[ENTER] " + Fore.YELLOW + "To continue\n\n" + Fore.RESET)
     time.sleep(3)
 
     # Empezamos con el crack de la password
     crack = subprocess.Popen(["aircrack-ng", file, "-w", wordlist], stdout=subprocess.PIPE)
 
@@ -421,17 +437,52 @@
             break
 
 
 def main():
     try:
         # Recogemos argumentos
         parser = argparse.ArgumentParser()
-        parser.add_argument("-w", "--wordlist", help="Use an extern wordlists dictionary", required=True)
+        parser.add_argument("-w", "--wordlist", help="Set diccionary attack, specify an extern wordlists dictionary  USAGE:  -w /path/to/dict\n", required=False)
+        parser.add_argument("-b", "--brute", help="Use password generator for brute force   USAGE: -b [length passwords / r (random)] E.j: -b 12 ", required=False)
+        parser.add_argument("-t", "--threads", help="Specify the number of threads", required=False)
         args = parser.parse_args()
 
+        # Checkeamos argumentos que estén bien...
+        if not args.wordlist and not args.brute:
+            print(Fore.RED + "[!] ERROR: " + Fore.YELLOW + "Debes introducir un parámetro...\n\t [ --help / -h ] for help")
+            exit(1)
+
+        elif args.brute:
+
+            if args.threads:
+                for num in args.threads:
+                    try:
+                        num = int(num)
+                    except ValueError:
+                        print(Fore.RED + "[!] " + Fore.LIGHTYELLOW_EX + "Opción inválida..." \
+                                                    "\n\tIntroduce un NUMERO...")
+                        exit(1)
+
+                    if num > 501:
+                        print(Fore.RED + "[!] " + Fore.LIGHTYELLOW_EX + "Opción inválida..." \
+                                                    "\n\tIntroduce el numero de hilos a usar entre 20 a 500...")
+                        exit(1)
+                    elif num < 20:
+                        print(Fore.RED + "[!] " + Fore.LIGHTYELLOW_EX + "Opción inválida..." \
+                                                                        "\n\tIntroduce el numero de hilos a usar entre 20 a 500...")
+                        exit(1)
+
+            if args.brute != "r":
+                for num in args.brute:
+                    if num not in string.digits:
+                        print(Fore.RED + "[!] " + Fore.LIGHTYELLOW_EX + "Opción inválida..." \
+                                "\n\tIntroduce el largo de las contraseñas o 'r' para random length")
+                        exit(1)
+
+
         # Somos root?
         am_i_root()
 
         # Tenemos las herraientas?
         check_utilities()
 
         # Listamos interfaces
```

### Comparing `evilHunter-0.1.7/setup.py` & `evilHunter-0.1.8/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 from setuptools import setup
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name="evilHunter",
-    version="0.1.7",
+    version="0.1.8",
     description="Cracking WiFi(Hanshake)",
     long_description=long_description,
     long_description_content_type="text/markdown",
     author="an0mal1a",
     url="https://github.com/an0mal1a/evilHunter",
     author_email="pablodiez024@proton.me",
     packages=["words"],
-    scripts=["evilHunter.py"],
+    scripts=["evilHunter.py", "evilCracker.py"],
     install_requires=[
         'colorama'
 ],
 
 )
```

