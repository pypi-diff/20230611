# Comparing `tmp/tool_server_generator-0.4.3.tar.gz` & `tmp/tool_server_generator-0.4.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tool_server_generator-0.4.3.tar", last modified: Sat Jun 10 21:09:51 2023, max compression
+gzip compressed data, was "tool_server_generator-0.4.4.tar", last modified: Sun Jun 11 20:48:36 2023, max compression
```

## Comparing `tool_server_generator-0.4.3.tar` & `tool_server_generator-0.4.4.tar`

### file list

```diff
@@ -1,27 +1,27 @@
--rwxr-xr-x   0        0        0     1077 2023-03-30 17:06:52.175851 tool_server_generator-0.4.3/LICENSE
--rwxr-xr-x   0        0        0      653 2023-06-08 22:39:34.183032 tool_server_generator-0.4.3/config_server.txt
--rwxr-xr-x   0        0        0      526 2023-06-08 17:49:02.430745 tool_server_generator-0.4.3/pyproject.toml
--rwxr-xr-x   0        0        0     6169 2023-06-10 21:08:13.696305 tool_server_generator-0.4.3/readme.md
--rwxr-xr-x   0        0        0     3982 2023-06-10 21:08:35.450249 tool_server_generator-0.4.3/tool_server_generator/__init__.py
--rwxr-xr-x   0        0        0      990 2023-06-09 13:32:47.222267 tool_server_generator-0.4.3/tool_server_generator/examples/config_server.json
--rwxr-xr-x   0        0        0      653 2023-06-08 22:39:31.488290 tool_server_generator-0.4.3/tool_server_generator/examples/config_server.txt
--rwxr-xr-x   0        0        0      984 2023-06-09 13:33:25.461589 tool_server_generator-0.4.3/tool_server_generator/examples/config_server2.txt
--rwxr-xr-x   0        0        0      927 2023-06-06 15:38:53.995935 tool_server_generator-0.4.3/tool_server_generator/model/app.js
--rwxr-xr-x   0        0        0     1524 2023-06-06 13:59:55.077587 tool_server_generator-0.4.3/tool_server_generator/model/bin/www
--rwxr-xr-x   0        0        0    46221 2023-06-05 17:39:59.097911 tool_server_generator-0.4.3/tool_server_generator/model/package-lock.json
--rwxr-xr-x   0        0        0      266 2023-06-05 21:25:25.521566 tool_server_generator-0.4.3/tool_server_generator/model/package.json
--rwxr-xr-x   0        0        0      318 2023-06-09 13:30:36.974342 tool_server_generator-0.4.3/tool_server_generator/model/public/images/favicon.ico
--rwxr-xr-x   0        0        0      940 2023-06-09 17:03:39.505128 tool_server_generator-0.4.3/tool_server_generator/model/public/javascripts/jquery.js
--rwxr-xr-x   0        0        0     1297 2023-06-10 15:25:19.412547 tool_server_generator-0.4.3/tool_server_generator/model/public/javascripts/requests.js
--rwxr-xr-x   0        0        0      421 2023-06-09 17:15:12.284029 tool_server_generator-0.4.3/tool_server_generator/model/public/stylesheets/color.css
--rwxr-xr-x   0        0        0    23424 2023-06-05 14:50:39.170516 tool_server_generator-0.4.3/tool_server_generator/model/public/stylesheets/w3.css
--rwxr-xr-x   0        0        0     2755 2023-06-09 17:13:40.296604 tool_server_generator-0.4.3/tool_server_generator/model/routes/index.js
--rwxr-xr-x   0        0        0       84 2023-06-05 14:49:43.482781 tool_server_generator-0.4.3/tool_server_generator/model/views/error.pug
--rwxr-xr-x   0        0        0     1046 2023-06-09 17:09:04.085388 tool_server_generator-0.4.3/tool_server_generator/model/views/layout.pug
--rwxr-xr-x   0        0        0     1950 2023-06-09 17:16:28.853886 tool_server_generator-0.4.3/tool_server_generator/model/views/requests.pug
--rwxr-xr-x   0        0        0     1899 2023-06-09 17:04:43.374738 tool_server_generator-0.4.3/tool_server_generator/model/workers/process_command.js
--rwxr-xr-x   0        0        0     6296 2023-06-09 17:04:43.379737 tool_server_generator-0.4.3/tool_server_generator/model/workers/request_listener.js
--rwxr-xr-x   0        0        0    18255 2023-06-10 21:07:37.157664 tool_server_generator-0.4.3/tool_server_generator/utils/config_parser.py
--rwxr-xr-x   0        0        0     9443 2023-06-10 21:07:10.092230 tool_server_generator-0.4.3/tool_server_generator/utils/config_server.py
--rwxr-xr-x   0        0        0      824 2023-06-08 22:05:58.703064 tool_server_generator-0.4.3/tool_server_generator/utils/utils.py
--rw-r--r--   0        0        0     6509 1970-01-01 00:00:00.000000 tool_server_generator-0.4.3/PKG-INFO
+-rwxr-xr-x   0        0        0     1077 2023-03-30 17:06:52.175851 tool_server_generator-0.4.4/LICENSE
+-rwxr-xr-x   0        0        0      653 2023-06-08 22:39:34.183032 tool_server_generator-0.4.4/config_server.txt
+-rwxr-xr-x   0        0        0      526 2023-06-08 17:49:02.430745 tool_server_generator-0.4.4/pyproject.toml
+-rwxr-xr-x   0        0        0     6044 2023-06-11 20:46:46.611171 tool_server_generator-0.4.4/readme.md
+-rwxr-xr-x   0        0        0     4054 2023-06-11 20:48:32.463246 tool_server_generator-0.4.4/tool_server_generator/__init__.py
+-rwxr-xr-x   0        0        0      990 2023-06-09 13:32:47.222267 tool_server_generator-0.4.4/tool_server_generator/examples/config_server.json
+-rwxr-xr-x   0        0        0      653 2023-06-08 22:39:31.488290 tool_server_generator-0.4.4/tool_server_generator/examples/config_server.txt
+-rwxr-xr-x   0        0        0      984 2023-06-09 13:33:25.461589 tool_server_generator-0.4.4/tool_server_generator/examples/config_server2.txt
+-rwxr-xr-x   0        0        0      927 2023-06-06 15:38:53.995935 tool_server_generator-0.4.4/tool_server_generator/model/app.js
+-rwxr-xr-x   0        0        0     1613 2023-06-11 20:43:41.701147 tool_server_generator-0.4.4/tool_server_generator/model/bin/www
+-rwxr-xr-x   0        0        0    46221 2023-06-05 17:39:59.097911 tool_server_generator-0.4.4/tool_server_generator/model/package-lock.json
+-rwxr-xr-x   0        0        0      266 2023-06-05 21:25:25.521566 tool_server_generator-0.4.4/tool_server_generator/model/package.json
+-rwxr-xr-x   0        0        0      318 2023-06-09 13:30:36.974342 tool_server_generator-0.4.4/tool_server_generator/model/public/images/favicon.ico
+-rwxr-xr-x   0        0        0      940 2023-06-09 17:03:39.505128 tool_server_generator-0.4.4/tool_server_generator/model/public/javascripts/jquery.js
+-rwxr-xr-x   0        0        0     1297 2023-06-10 15:25:19.412547 tool_server_generator-0.4.4/tool_server_generator/model/public/javascripts/requests.js
+-rwxr-xr-x   0        0        0      421 2023-06-09 17:15:12.284029 tool_server_generator-0.4.4/tool_server_generator/model/public/stylesheets/color.css
+-rwxr-xr-x   0        0        0    23424 2023-06-05 14:50:39.170516 tool_server_generator-0.4.4/tool_server_generator/model/public/stylesheets/w3.css
+-rwxr-xr-x   0        0        0     2755 2023-06-11 20:43:41.698145 tool_server_generator-0.4.4/tool_server_generator/model/routes/index.js
+-rwxr-xr-x   0        0        0       84 2023-06-05 14:49:43.482781 tool_server_generator-0.4.4/tool_server_generator/model/views/error.pug
+-rwxr-xr-x   0        0        0     1046 2023-06-11 20:43:15.983992 tool_server_generator-0.4.4/tool_server_generator/model/views/layout.pug
+-rwxr-xr-x   0        0        0     1950 2023-06-09 17:16:28.853886 tool_server_generator-0.4.4/tool_server_generator/model/views/requests.pug
+-rwxr-xr-x   0        0        0     1875 2023-06-11 17:31:34.239106 tool_server_generator-0.4.4/tool_server_generator/model/workers/process_command.js
+-rwxr-xr-x   0        0        0     6316 2023-06-11 17:31:04.844192 tool_server_generator-0.4.4/tool_server_generator/model/workers/request_listener.js
+-rwxr-xr-x   0        0        0    18183 2023-06-11 20:44:10.889720 tool_server_generator-0.4.4/tool_server_generator/utils/config_parser.py
+-rwxr-xr-x   0        0        0     9443 2023-06-11 20:43:41.700146 tool_server_generator-0.4.4/tool_server_generator/utils/config_server.py
+-rwxr-xr-x   0        0        0      824 2023-06-08 22:05:58.703064 tool_server_generator-0.4.4/tool_server_generator/utils/utils.py
+-rw-r--r--   0        0        0     6384 1970-01-01 00:00:00.000000 tool_server_generator-0.4.4/PKG-INFO
```

### Comparing `tool_server_generator-0.4.3/LICENSE` & `tool_server_generator-0.4.4/LICENSE`

 * *Files identical despite different names*

### Comparing `tool_server_generator-0.4.3/config_server.txt` & `tool_server_generator-0.4.4/config_server.txt`

 * *Files identical despite different names*

### Comparing `tool_server_generator-0.4.3/pyproject.toml` & `tool_server_generator-0.4.4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `tool_server_generator-0.4.3/readme.md` & `tool_server_generator-0.4.4/readme.md`

 * *Files 2% similar despite different names*

```diff
@@ -33,36 +33,33 @@
 ### **Server Options**
 
 #### *Text File*
 
 - Name: name of the server.
 - Directory: directory where the server will be created and run from.
 - Port: port of the server.
-- Route: base route of the website (optional - default '/').
 - Workers: number of workers available to process requests (optional - default 1).
 
 Example:
 
         * Servidor
         - Nome: Server
         - Diretoria: "test"
         - Porta: 15213
-        - Rota: server\test
         - Trabalhadores: 2
 
 #### *JSON*
 
 The same type of fields are expected, the optional and obligatory are similar. Only the keys are differente.  
 Example:
 
         {
             "nome" : "Server",
             "diretoria" : "test",
             "porta" : "15213",
-            "rota" : "server\test",
             "workers" : 1,
         }
 
 ### **Tools options**
 
 #### *Text File*
```

### Comparing `tool_server_generator-0.4.3/tool_server_generator/__init__.py` & `tool_server_generator-0.4.4/tool_server_generator/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,25 +7,25 @@
 import subprocess
 import json
 from pyngrok import ngrok
 from .utils.utils import *
 from .utils.config_parser import *
 from .utils.config_server import *
 
-__version__ = '0.4.3'
+__version__ = '0.4.4'
 project_dir = os.path.dirname(os.path.realpath(__file__))
 model_server = f'{project_dir}/model'
 tunnel = None
 
 def start_ngrok(config):
     '''Tenta expor a porta do servidor utilizando o ngrok'''
     global tunnel
     try:
         print(ngrok.get_tunnels())
-        print('Exposing port using ngrok')
+        print('LOG: Exposing port using ngrok')
         tunnel = ngrok.connect(config['porta'],'http')
         print('Public URL: ',tunnel.public_url)
     except Exception as e:
         print(e)
         print('Error: Could not expose port using ngrok.')
         tunnel = None
 
@@ -35,31 +35,31 @@
     dependencies = ['express','http-errors','adm-zip']
 
     # multer apenas se ferramentas levarem ficheiros como input
     if has_file_input(config['ferramentas']):
         dependencies += ['multer']
         
     dependencies = ' '.join(dependencies)
-    print(f'Installing server dependencies: [{dependencies}]')
+    print(f'LOG: Installing server dependencies: [{dependencies}]')
     p = subprocess.call(f'npm i {dependencies} -s', cwd=server_path,shell=True)
-    print('Dependencies installed')
+    print('LOG: Dependencies installed')
 
 
 def start_server(server_dir):
     '''Inicia o servidor'''
     global tunnel
     server_path = f'{os.getcwd()}/{server_dir}'
     try:
-        print('Starting server')
+        print('LOG: Starting server')
         p = subprocess.call(f'npm start', cwd=server_path,shell=True)
     except Exception as e:
-        print('Server closed')
+        print('LOG: Server closed')
         # desconectar ngrok
         if tunnel:
-            print('Closing ngrok')
+            print('LOG: Closing ngrok')
             ngrok.disconnect(tunnel.public_url)
 
 def tool_server():
     args = parse_arguments(__version__)
     config_file = args.config_file[0]
     file = open(config_file,'r',encoding='utf-8')
     json_config = False
@@ -75,21 +75,21 @@
     if not json_config or config_valid(config):
         #Copiar o modelo do servidor para a diretoria desejada
         destino = config['diretoria'] + '/' + config['nome']
         origem = model_server
         try:
             shutil.copytree(origem, destino)
         except FileNotFoundError:
-            print("Model Server not found!")
+            print("Error: Model Server not found!")
             exit(-1)
         except FileExistsError:
-            print("Directory already exists.")
+            print("Error: Directory already exists.")
             exit(-1)
         except Exception as e:
-            print(f"Error copying the model server: {e}")
+            print(f"Error: Error copying the model server: {e}")
             exit(-1)
         
         # alterar configuracoes do servidor
         config_server(destino,config)
 
         if config['visuais']['favicon'] != '':
             favicon = config['visuais']['favicon']
@@ -99,25 +99,25 @@
             #remover favicon default que vem do model
             os.remove(old_favicon)
             
             #colocar o dado
             try:
                 shutil.copy(favicon,destino_favicon)
             except FileNotFoundError:
-                print("Favicon not found!")
+                print("Error: Favicon not found!")
                 exit(-1)
             except Exception as e:
-                print(f"Error copying the favicon: {e}")
+                print(f"Error: Error copying the favicon: {e}")
                 exit(-1)
         # instalar dependencias do servidor
         install_server_dependencies(destino,config)
 
         #iniciar servidor
         if args.start_server:
             # expor porta de ngrok
             if args.ngrok:
                 start_ngrok(config)
 
             start_server(destino)
     else:
-        print('Error on the configuration file.')
+        print('Error: Error on the configuration file.')
         exit(-1)
```

### Comparing `tool_server_generator-0.4.3/tool_server_generator/examples/config_server.json` & `tool_server_generator-0.4.4/tool_server_generator/examples/config_server.json`

 * *Files identical despite different names*

### Comparing `tool_server_generator-0.4.3/tool_server_generator/examples/config_server.txt` & `tool_server_generator-0.4.4/tool_server_generator/examples/config_server.txt`

 * *Files identical despite different names*

### Comparing `tool_server_generator-0.4.3/tool_server_generator/examples/config_server2.txt` & `tool_server_generator-0.4.4/tool_server_generator/examples/config_server2.txt`

 * *Files identical despite different names*

### Comparing `tool_server_generator-0.4.3/tool_server_generator/model/app.js` & `tool_server_generator-0.4.4/tool_server_generator/model/app.js`

 * *Files identical despite different names*

### Comparing `tool_server_generator-0.4.3/tool_server_generator/model/bin/www` & `tool_server_generator-0.4.4/tool_server_generator/model/bin/www`

 * *Ordering differences only*

 * *Files 22% similar despite different names*

```diff
@@ -1,89 +1,89 @@
-#!/usr/bin/env node
-
-/**
- * Module dependencies.
- */
-
-var app = require('../app');
-var debug = require('debug')('model:server');
-var http = require('http');
-
-
-var ip = $ip
-
-/**
- * Get port from environment and store in Express.
- */
-
-var port = normalizePort($port);
-app.set('port', port);
-
-/**
- * Create HTTP server.
- */
-
-var server = http.createServer(app);
-
-/**
- * Listen on provided port, on all network interfaces.
- */
-
-server.listen(port,ip);
-server.on('error', onError);
-server.on('listening', onListening);
-
-/**
- * Normalize a port into a number, string, or false.
- */
-
-function normalizePort(val) {
-  var port = parseInt(val, 10);
-
-  if (isNaN(port)) {
-    // named pipe
-    return val;
-  }
-
-  if (port >= 0) {
-    // port number
-    return port;
-  }
-
-  return false;
-}
-
-/**
- * Event listener for HTTP server "error" event.
- */
-
-function onError(error) {
-  if (error.syscall !== 'listen') {
-    throw error;
-  }
-
-  var bind = typeof port === 'string'
-    ? 'Pipe ' + port
-    : 'Port ' + port;
-
-  // handle specific listen errors with friendly messages
-  switch (error.code) {
-    case 'EACCES':
-      console.error(bind + ' requires elevated privileges');
-      process.exit(1);
-      break;
-    case 'EADDRINUSE':
-      console.error(bind + ' is already in use');
-      process.exit(1);
-      break;
-    default:
-      throw error;
-  }
-}
-
-/**
- * Event listener for HTTP server "listening" event.
- */
-
-function onListening() {
-  console.log('Servidor à escuta na porta ' + port + `\nURL: http://${ip}:${port}` )
-}
+#!/usr/bin/env node
+
+/**
+ * Module dependencies.
+ */
+
+var app = require('../app');
+var debug = require('debug')('model:server');
+var http = require('http');
+
+
+var ip = $ip
+
+/**
+ * Get port from environment and store in Express.
+ */
+
+var port = normalizePort($port);
+app.set('port', port);
+
+/**
+ * Create HTTP server.
+ */
+
+var server = http.createServer(app);
+
+/**
+ * Listen on provided port, on all network interfaces.
+ */
+
+server.listen(port,ip);
+server.on('error', onError);
+server.on('listening', onListening);
+
+/**
+ * Normalize a port into a number, string, or false.
+ */
+
+function normalizePort(val) {
+  var port = parseInt(val, 10);
+
+  if (isNaN(port)) {
+    // named pipe
+    return val;
+  }
+
+  if (port >= 0) {
+    // port number
+    return port;
+  }
+
+  return false;
+}
+
+/**
+ * Event listener for HTTP server "error" event.
+ */
+
+function onError(error) {
+  if (error.syscall !== 'listen') {
+    throw error;
+  }
+
+  var bind = typeof port === 'string'
+    ? 'Pipe ' + port
+    : 'Port ' + port;
+
+  // handle specific listen errors with friendly messages
+  switch (error.code) {
+    case 'EACCES':
+      console.error(bind + ' requires elevated privileges');
+      process.exit(1);
+      break;
+    case 'EADDRINUSE':
+      console.error(bind + ' is already in use');
+      process.exit(1);
+      break;
+    default:
+      throw error;
+  }
+}
+
+/**
+ * Event listener for HTTP server "listening" event.
+ */
+
+function onListening() {
+  console.log('Servidor à escuta na porta ' + port + `\nURL: http://${ip}:${port}` )
+}
```

### Comparing `tool_server_generator-0.4.3/tool_server_generator/model/package-lock.json` & `tool_server_generator-0.4.4/tool_server_generator/model/package-lock.json`

 * *Files identical despite different names*

### Comparing `tool_server_generator-0.4.3/tool_server_generator/model/public/javascripts/jquery.js` & `tool_server_generator-0.4.4/tool_server_generator/model/public/javascripts/jquery.js`

 * *Files identical despite different names*

### Comparing `tool_server_generator-0.4.3/tool_server_generator/model/public/javascripts/requests.js` & `tool_server_generator-0.4.4/tool_server_generator/model/public/javascripts/requests.js`

 * *Files identical despite different names*

### Comparing `tool_server_generator-0.4.3/tool_server_generator/model/public/stylesheets/w3.css` & `tool_server_generator-0.4.4/tool_server_generator/model/public/stylesheets/w3.css`

 * *Files identical despite different names*

### Comparing `tool_server_generator-0.4.3/tool_server_generator/model/routes/index.js` & `tool_server_generator-0.4.4/tool_server_generator/model/routes/index.js`

 * *Files identical despite different names*

### Comparing `tool_server_generator-0.4.3/tool_server_generator/model/views/layout.pug` & `tool_server_generator-0.4.4/tool_server_generator/model/views/layout.pug`

 * *Files identical despite different names*

### Comparing `tool_server_generator-0.4.3/tool_server_generator/model/views/requests.pug` & `tool_server_generator-0.4.4/tool_server_generator/model/views/requests.pug`

 * *Files identical despite different names*

### Comparing `tool_server_generator-0.4.3/tool_server_generator/model/workers/process_command.js` & `tool_server_generator-0.4.4/tool_server_generator/model/workers/process_command.js`

 * *Files 6% similar despite different names*

#### js-beautify {}

```diff
@@ -34,21 +34,20 @@
 
 /**
  * Funcao para correr um comando
  */
 function run_command() {
     request_path = request.path
     command = request.command
-    console.log('Worker ' + id + ' with request ' + request.number + 'running command: ' + command)
+    console.log('LOG: Worker ' + id + ' with request ' + request.number + 'running command: ' + command)
     try {
         // executar comando
         out = execSync(command, {
             cwd: request_path
         })
-        console.log(out.toString());
         // Escrever ficheiros com output de terminal na pasta da request
         out_file = path.join(request_path, `request_${request.number}_${Date.parse(request.date)}_stdout.txt`)
         fs.writeFileSync(out_file, out.toString())
     } catch (err) {
         error = err.stderr.toString()
         console.log('Error:' + err);
         console.log('Stderr:' + error);
@@ -64,9 +63,9 @@
         new_mtime = stats.mtime
 
         if (datesEqual(old_mtime, new_mtime)) {
             fs.unlinkSync(filepath) //elimino o input
         }
     }
 
-    console.log('Worker ' + id + ' done')
+    console.log('LOG: Worker ' + id + ' done')
 }
```

### Comparing `tool_server_generator-0.4.3/tool_server_generator/model/workers/request_listener.js` & `tool_server_generator-0.4.4/tool_server_generator/model/workers/request_listener.js`

 * *Files 2% similar despite different names*

#### js-beautify {}

```diff
@@ -68,15 +68,15 @@
 
 parentPort.on('message', (data) => {
     msg = data.msg
     if (msg == 'command') {
         fields = data.data
         command = fields.command
         files = data.files
-        console.log(`
+        console.log(`LOG: 
         Request Number: ${request_n}
         Command: ${command}
         Files : ${files}
         `)
         // processar pedido para ser mais facilmente usado por um worker
         process_command(fields, files)
         // tenta mandar pedido para um worker
@@ -100,23 +100,23 @@
 })
 
 
 /**
  * Da uma request a um worker se possivel
  */
 function send_request() {
-    console.log('Sending request')
+    console.log('LOG: Sending request')
     // enquanto que houver workers tenta distribuir pedidos
     while (available_workers.length > 0) {
         // se houver pedidos, distribui para um worker
         if (queue.length > 0) {
             id = available_workers.pop()
             request = queue.pop()
             pending_requests[request.number]['status'] = 'Processing'
-            console.log(`Request ${request.number} delivered to worker ${id}`)
+            console.log(`LOG: Request ${request.number} delivered to worker ${id}`)
             // criar worker
             worker = new Worker('./workers/process_command.js', {
                 workerData: {
                     id,
                     request
                 }
             })
@@ -139,15 +139,15 @@
     id = data.id
     request_id = data.request_id
     message = data.message
     // trocar request de pending para completed
     completed_requests[request_id] = pending_requests[request_id]
     completed_requests[request_id]['status'] = 'Completed'
     delete pending_requests[request_id]
-    console.log('Worker message:' + message)
+    console.log('LOG: Worker message:' + message)
     // remover worker
     workers[id].removeListener('message', worker_callback)
     workers[id].unref()
     workers[id] = null
     // adicionar um slot de worker disponivel
     available_workers.push(id)
     // tenta distribuir nova request
```

### Comparing `tool_server_generator-0.4.3/tool_server_generator/utils/config_parser.py` & `tool_server_generator-0.4.4/tool_server_generator/utils/config_parser.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,19 +5,18 @@
 
 import re
 
 
 grammar = '''
 start : servidor
 servidor : "*" "Servidor" opcoes_servidor ferramentas visuais?
-opcoes_servidor : nome_servidor diretoria_servidor porta_servidor  rota_servidor? trabalhadores_servidor?
+opcoes_servidor : nome_servidor diretoria_servidor porta_servidor trabalhadores_servidor?
 nome_servidor : "-" "Nome" ":" NOME
 diretoria_servidor : "-" "Diretoria" ":" TEXTO
 porta_servidor : "-" "Porta" ":" PORTA
-rota_servidor : "-" "Rota" ":" ROTA
 trabalhadores_servidor : "-" "Trabalhadores" ":" INT
 
 ferramentas : "*" "Ferramentas" ("--" ferramenta)+
 ferramenta : familia titulo descricao comando inputs?
 familia : "-" "Família" ":" NOME
 titulo  : "-" "Título" ":" TEXTO
 descricao : "-" "Descrição" ":" TEXTO
@@ -42,15 +41,14 @@
 opcoes_input : input_nome? input_descricao? input_tipo
 input_nome : "-" "Nome" ":" NOME 
 input_descricao : "-" "Descrição" ":" TEXTO 
 input_tipo : "-" "Tipo" ":" TYPE 
 
 IP: /(\d{1,4}\.){3}\d{1,4}/
 PORTA: /\d+/
-ROTA: /[\w\-\/]+/
 STR: /"[^"]"/
 TEXTO: /"[^"]*"/
 NOME: /[\w\-]+/
 PALAVRA: /[\w\.\-_]+/
 INPUT: /INPUT\d+/
 FLAG: /-{1,2}\w+/
 TYPE: /(STR)|(NUM)|(FILE)/
```

### Comparing `tool_server_generator-0.4.3/tool_server_generator/utils/config_server.py` & `tool_server_generator-0.4.4/tool_server_generator/utils/config_server.py`

 * *Files identical despite different names*

### Comparing `tool_server_generator-0.4.3/tool_server_generator/utils/utils.py` & `tool_server_generator-0.4.4/tool_server_generator/utils/utils.py`

 * *Files identical despite different names*

### Comparing `tool_server_generator-0.4.3/PKG-INFO` & `tool_server_generator-0.4.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tool_server_generator
-Version: 0.4.3
+Version: 0.4.4
 Summary: Module to create tools server
 Author-email: brazafonso <a93178@uminho.pt>, Tiago Silva <a93277@uminho.pt>
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: MIT License
 Requires-Dist: lark
 Requires-Dist: argparse
 Requires-Dist: pyngrok
@@ -44,36 +44,33 @@
 ### **Server Options**
 
 #### *Text File*
 
 - Name: name of the server.
 - Directory: directory where the server will be created and run from.
 - Port: port of the server.
-- Route: base route of the website (optional - default '/').
 - Workers: number of workers available to process requests (optional - default 1).
 
 Example:
 
         * Servidor
         - Nome: Server
         - Diretoria: "test"
         - Porta: 15213
-        - Rota: server\test
         - Trabalhadores: 2
 
 #### *JSON*
 
 The same type of fields are expected, the optional and obligatory are similar. Only the keys are differente.  
 Example:
 
         {
             "nome" : "Server",
             "diretoria" : "test",
             "porta" : "15213",
-            "rota" : "server\test",
             "workers" : 1,
         }
 
 ### **Tools options**
 
 #### *Text File*
```

