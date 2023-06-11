# Comparing `tmp/maadstml-3.29.tar.gz` & `tmp/maadstml-3.30.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "maadstml-3.29.tar", last modified: Sun Jun 11 15:19:05 2023, max compression
+gzip compressed data, was "maadstml-3.30.tar", last modified: Sun Jun 11 18:47:33 2023, max compression
```

## Comparing `maadstml-3.29.tar` & `maadstml-3.30.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2023-06-11 15:19:05.239710 maadstml-3.29/
--rw-rw-rw-   0        0        0      852 2020-02-09 18:05:54.000000 maadstml-3.29/LICENSE.txt
--rw-rw-rw-   0        0        0       65 2021-01-25 23:03:44.000000 maadstml-3.29/MANIFEST.in
--rw-rw-rw-   0        0        0   171897 2023-06-11 15:19:05.234083 maadstml-3.29/PKG-INFO
--rw-rw-rw-   0        0        0   171300 2023-06-10 19:59:31.000000 maadstml-3.29/README.md
-drwxrwxrwx   0        0        0        0 2023-06-11 15:19:05.215295 maadstml-3.29/maadstml/
--rw-rw-rw-   0        0        0     2121 2023-06-10 19:55:10.000000 maadstml-3.29/maadstml/__init__.py
--rw-rw-rw-   0        0        0     4871 2023-06-10 19:44:05.000000 maadstml-3.29/maadstml/readpdf.py
--rw-rw-rw-   0        0        0    76603 2023-06-11 15:18:32.000000 maadstml-3.29/maadstml/sendfiles.py
--rw-rw-rw-   0        0        0    10850 2023-06-10 19:08:28.000000 maadstml-3.29/maadstml/tmltextsummary.py
-drwxrwxrwx   0        0        0        0 2023-06-11 15:19:05.234083 maadstml-3.29/maadstml.egg-info/
--rw-rw-rw-   0        0        0   171897 2023-06-11 15:19:05.000000 maadstml-3.29/maadstml.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      320 2023-06-11 15:19:05.000000 maadstml-3.29/maadstml.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-11 15:19:05.000000 maadstml-3.29/maadstml.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      115 2023-06-11 15:19:05.000000 maadstml-3.29/maadstml.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-06-11 15:19:05.000000 maadstml-3.29/maadstml.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      122 2021-02-05 16:13:04.000000 maadstml-3.29/requirements.txt
--rw-rw-rw-   0        0        0       42 2023-06-11 15:19:05.239710 maadstml-3.29/setup.cfg
--rw-rw-rw-   0        0        0     1088 2023-06-11 15:18:59.000000 maadstml-3.29/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-11 18:47:33.637813 maadstml-3.30/
+-rw-rw-rw-   0        0        0      852 2020-02-09 18:05:54.000000 maadstml-3.30/LICENSE.txt
+-rw-rw-rw-   0        0        0       65 2021-01-25 23:03:44.000000 maadstml-3.30/MANIFEST.in
+-rw-rw-rw-   0        0        0   172671 2023-06-11 18:47:33.632964 maadstml-3.30/PKG-INFO
+-rw-rw-rw-   0        0        0   172074 2023-06-11 18:43:51.000000 maadstml-3.30/README.md
+drwxrwxrwx   0        0        0        0 2023-06-11 18:47:33.610923 maadstml-3.30/maadstml/
+-rw-rw-rw-   0        0        0     2158 2023-06-11 18:45:29.000000 maadstml-3.30/maadstml/__init__.py
+-rw-rw-rw-   0        0        0     4871 2023-06-10 19:44:05.000000 maadstml-3.30/maadstml/readpdf.py
+-rw-rw-rw-   0        0        0    78954 2023-06-11 18:44:43.000000 maadstml-3.30/maadstml/sendfiles.py
+-rw-rw-rw-   0        0        0    10850 2023-06-10 19:08:28.000000 maadstml-3.30/maadstml/tmltextsummary.py
+drwxrwxrwx   0        0        0        0 2023-06-11 18:47:33.632964 maadstml-3.30/maadstml.egg-info/
+-rw-rw-rw-   0        0        0   172671 2023-06-11 18:47:33.000000 maadstml-3.30/maadstml.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      320 2023-06-11 18:47:33.000000 maadstml-3.30/maadstml.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-11 18:47:33.000000 maadstml-3.30/maadstml.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      165 2023-06-11 18:47:33.000000 maadstml-3.30/maadstml.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-06-11 18:47:33.000000 maadstml-3.30/maadstml.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      178 2023-06-11 18:47:05.000000 maadstml-3.30/requirements.txt
+-rw-rw-rw-   0        0        0       42 2023-06-11 18:47:33.637813 maadstml-3.30/setup.cfg
+-rw-rw-rw-   0        0        0     1088 2023-06-11 18:46:06.000000 maadstml-3.30/setup.py
```

### Comparing `maadstml-3.29/LICENSE.txt` & `maadstml-3.30/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `maadstml-3.29/PKG-INFO` & `maadstml-3.30/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: maadstml
-Version: 3.29
+Version: 3.30
 Summary: Multi-Agent Accelerator for Data Science (MAADS): Transactional Machine Learning
 Home-page: https://github.com/smaurice101/transactionalmachinelearning
 Author: Sebastian Maurice
 Author-email: sebastian.maurice@otics.ca
 License: MIT License
 Keywords: multi-agent, transactional machine learning, data streams, data science, optimization, prescriptive analytics, machine learning, automl,auto-ml,artificial intelligence,predictive analytics,advanced analytics
 Description-Content-Type: text/markdown
@@ -12,15 +12,15 @@
 
 **Multi-Agent Accelerator for Data Science Using Transactional Machine Learning (MAADSTML)**
 
 *Revolutionizing Data Stream Science with Transactional Machine Learning*
 
 **Overview**
 
-*MAADSTML combines Artificial Intelligence, Auto Machine Learning with Data Streams Integrated with Apache Kafka (or Redpanda) to create frictionless and elastic machine learning solutions.*  
+*MAADSTML combines Artificial Intelligence, ChatGPT, Auto Machine Learning with Data Streams Integrated with Apache Kafka (or Redpanda) to create frictionless and elastic machine learning solutions.*  
 
 This library allows users to harness the power of agent-based computing using hundreds of advanced linear and non-linear algorithms. Users can easily integrate Predictive Analytics, Prescriptive Analytics, Pre-Processing, and Optimization in any data stream solution by wrapping additional code around the functions below. It connects with **Apache KAFKA brokers** for cloud based computing using Kafka (or Redpanda) as the data backbone. 
 
 If analysing MILLIONS of IoT devices, you can easily deploy thousands of VIPER/HPDE instances in Kubernetes Cluster in AWS/GCP/Azure. 
 
 It uses VIPER as a **KAFKA connector and seamlessly combines Auto Machine Learning, with Real-Time Machine Learning, Real-Time Optimization and Real-Time Predictions** while publishing these insights in to a Kafka cluster in real-time at scale, while allowing users to consume these insights from anywhere, anytime and in any format. 
 
@@ -244,14 +244,17 @@
 - **vipersearchanomaly**
   - Perform advanced analysis for user search.  This function is useful if you want to monitor what people are searching for, and determine
     if the searches are anamolous and differ from the peer group of "normal" search behaviour.
 
 - **vipernlp**
   - Perform advanced natural language summary of PDFs.
 
+- **viperchatgpt**
+  - Start a conversation with ChatGPT in real-time and stream responses.
+
 - **areyoubusy**
   - If deploying thousands of VIPER/HPDE binaries in a Kubernetes cluster - you can broadcast a 'areyoubusy' message to all VIPER and HPDE
     binaries, and they will return back the HOST/PORT if they are NOT busy with other tasks.  This is very convenient for dynamically managing  
 	enormous load among VIPER/HPDE and allows you to dynamically assign HOST/PORT to **non-busy** VIPER/HPDE microservices.
 
 **First import the Python library.**
 
@@ -4522,7 +4525,34 @@
 - Maximum amount of words in the summary.
 
 *maxkeywords* : int, required
 
 - Maximum amount of keywords to extract.
 
 RETURNS: JSON string of summary.
+
+**37. maadstml.viperchatgpt(openaikey,texttoanalyse,query, temperature,modelname)**
+
+**Parameters:**	Start a conversation with ChatGPT
+
+*openaikey* : string, required
+
+- OpenAI API key
+
+*texttoanalyse* : string, required
+       
+- Text you want ChatGPT to analyse
+
+*query* : string, required
+
+- Prompts for chatGPT.  For example, "What are key points in this text? What are the concerns or issues?"
+
+*temperature* : float, required
+
+- Temperature for chatgpt, must be between 0-1 i.e. 0.7
+
+*modelname* : string, required
+
+- ChatGPT model to use.  For example, text-davinci-002, text-curie-001, text-babbage-001.
+
+
+RETURNS: ChatGPT response.
```

### Comparing `maadstml-3.29/README.md` & `maadstml-3.30/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 **Multi-Agent Accelerator for Data Science Using Transactional Machine Learning (MAADSTML)**
 
 *Revolutionizing Data Stream Science with Transactional Machine Learning*
 
 **Overview**
 
-*MAADSTML combines Artificial Intelligence, Auto Machine Learning with Data Streams Integrated with Apache Kafka (or Redpanda) to create frictionless and elastic machine learning solutions.*  
+*MAADSTML combines Artificial Intelligence, ChatGPT, Auto Machine Learning with Data Streams Integrated with Apache Kafka (or Redpanda) to create frictionless and elastic machine learning solutions.*  
 
 This library allows users to harness the power of agent-based computing using hundreds of advanced linear and non-linear algorithms. Users can easily integrate Predictive Analytics, Prescriptive Analytics, Pre-Processing, and Optimization in any data stream solution by wrapping additional code around the functions below. It connects with **Apache KAFKA brokers** for cloud based computing using Kafka (or Redpanda) as the data backbone. 
 
 If analysing MILLIONS of IoT devices, you can easily deploy thousands of VIPER/HPDE instances in Kubernetes Cluster in AWS/GCP/Azure. 
 
 It uses VIPER as a **KAFKA connector and seamlessly combines Auto Machine Learning, with Real-Time Machine Learning, Real-Time Optimization and Real-Time Predictions** while publishing these insights in to a Kafka cluster in real-time at scale, while allowing users to consume these insights from anywhere, anytime and in any format. 
 
@@ -232,14 +232,17 @@
 - **vipersearchanomaly**
   - Perform advanced analysis for user search.  This function is useful if you want to monitor what people are searching for, and determine
     if the searches are anamolous and differ from the peer group of "normal" search behaviour.
 
 - **vipernlp**
   - Perform advanced natural language summary of PDFs.
 
+- **viperchatgpt**
+  - Start a conversation with ChatGPT in real-time and stream responses.
+
 - **areyoubusy**
   - If deploying thousands of VIPER/HPDE binaries in a Kubernetes cluster - you can broadcast a 'areyoubusy' message to all VIPER and HPDE
     binaries, and they will return back the HOST/PORT if they are NOT busy with other tasks.  This is very convenient for dynamically managing  
 	enormous load among VIPER/HPDE and allows you to dynamically assign HOST/PORT to **non-busy** VIPER/HPDE microservices.
 
 **First import the Python library.**
 
@@ -4510,7 +4513,34 @@
 - Maximum amount of words in the summary.
 
 *maxkeywords* : int, required
 
 - Maximum amount of keywords to extract.
 
 RETURNS: JSON string of summary.
+
+**37. maadstml.viperchatgpt(openaikey,texttoanalyse,query, temperature,modelname)**
+
+**Parameters:**	Start a conversation with ChatGPT
+
+*openaikey* : string, required
+
+- OpenAI API key
+
+*texttoanalyse* : string, required
+       
+- Text you want ChatGPT to analyse
+
+*query* : string, required
+
+- Prompts for chatGPT.  For example, "What are key points in this text? What are the concerns or issues?"
+
+*temperature* : float, required
+
+- Temperature for chatgpt, must be between 0-1 i.e. 0.7
+
+*modelname* : string, required
+
+- ChatGPT model to use.  For example, text-davinci-002, text-curie-001, text-babbage-001.
+
+
+RETURNS: ChatGPT response.
```

### Comparing `maadstml-3.29/maadstml/__init__.py` & `maadstml-3.30/maadstml/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -73,9 +73,10 @@
 from .sendfiles import areyoubusy
 from .sendfiles import vipermirrorbrokers
 
 from .sendfiles import viperhpdepredictprocess
 
 from .sendfiles import vipernlp
 
+from .sendfiles import viperchatgpt
 
 name = "maadstml"
```

### Comparing `maadstml-3.29/maadstml/readpdf.py` & `maadstml-3.30/maadstml/readpdf.py`

 * *Files identical despite different names*

### Comparing `maadstml-3.29/maadstml/sendfiles.py` & `maadstml-3.30/maadstml/sendfiles.py`

 * *Files 2% similar despite different names*

```diff
@@ -4040,749 +4040,896 @@
 0000fc70: 3130 303a 0d0a 2020 2020 2020 2020 7265  100:..        re
 0000fc80: 7475 726e 2022 4b65 7977 6f72 6420 636f  turn "Keyword co
 0000fc90: 756e 7420 746f 6f20 6869 6768 2e20 4d75  unt too high. Mu
 0000fca0: 7374 2062 6520 203c 2031 3030 220d 0a20  st be  < 100".. 
 0000fcb0: 2020 2020 2020 200d 0a20 2020 2072 6574         ..    ret
 0000fcc0: 7572 6e20 7374 6172 7470 6466 7265 6164  urn startpdfread
 0000fcd0: 696e 6728 6669 6c65 6e61 6d65 2c66 7661  ing(filename,fva
-0000fce0: 6c75 652c 6b65 7973 290d 0a20 2020 200d  lue,keys)..    .
-0000fcf0: 0a64 6566 2061 7265 796f 7562 7573 7928  .def areyoubusy(
-0000fd00: 686f 7374 2c70 6f72 743d 2d39 3939 2c6d  host,port=-999,m
-0000fd10: 6963 726f 7365 7276 6963 6569 643d 2727  icroserviceid=''
-0000fd20: 293a 0d0a 2020 2020 676c 6f62 616c 2063  ):..    global c
-0000fd30: 6f6e 6e65 6374 696f 6e65 7272 6f72 0d0a  onnectionerror..
-0000fd40: 0d0a 2020 2020 6966 2028 6c65 6e28 686f  ..    if (len(ho
-0000fd50: 7374 293d 3d30 206f 7220 706f 7274 3d3d  st)==0 or port==
-0000fd60: 2d39 3939 2029 3a0d 0a20 2020 2020 2020  -999 ):..       
-0000fd70: 2020 7265 7475 726e 2022 506c 6561 7365    return "Please
-0000fd80: 2065 6e74 6572 2068 6f73 742c 706f 7274   enter host,port
-0000fd90: 220d 0a20 2020 2076 616c 7565 3d28 2261  "..    value=("a
-0000fda0: 7265 796f 7562 7573 7922 290d 0a0d 0a20  reyoubusy").... 
-0000fdb0: 2020 2076 616c 3d6c 6f6f 702e 7275 6e5f     val=loop.run_
-0000fdc0: 756e 7469 6c5f 636f 6d70 6c65 7465 2874  until_complete(t
-0000fdd0: 6370 5f65 6368 6f5f 636c 6965 6e74 7669  cp_echo_clientvi
-0000fde0: 7065 7228 7661 6c75 652c 206c 6f6f 702c  per(value, loop,
-0000fdf0: 686f 7374 2c70 6f72 742c 6d69 6372 6f73  host,port,micros
-0000fe00: 6572 7669 6365 6964 2929 0d0a 2020 2020  erviceid))..    
-0000fe10: 6966 2063 6f6e 6e65 6374 696f 6e65 7272  if connectionerr
-0000fe20: 6f72 3a0d 0a20 2020 2020 2020 2020 7265  or:..         re
-0000fe30: 7475 726e 2063 6f6e 6e65 6374 696f 6e65  turn connectione
-0000fe40: 7272 6f72 0d0a 0d0a 2020 2020 7265 7475  rror....    retu
-0000fe50: 726e 2076 616c 0d0a 0d0a 2323 2323 2323  rn val....######
-0000fe60: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-0000fe70: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-0000fe80: 2323 2323 2323 2323 2323 2323 2323 0d0a  ##############..
-0000fe90: 696d 706f 7274 2073 7973 0d0a 6672 6f6d  import sys..from
-0000fea0: 2070 6466 6d69 6e65 722e 7064 6670 6172   pdfminer.pdfpar
-0000feb0: 7365 7220 696d 706f 7274 2050 4446 5061  ser import PDFPa
-0000fec0: 7273 6572 0d0a 6672 6f6d 2070 6466 6d69  rser..from pdfmi
-0000fed0: 6e65 722e 7064 6664 6f63 756d 656e 7420  ner.pdfdocument 
-0000fee0: 696d 706f 7274 2050 4446 446f 6375 6d65  import PDFDocume
-0000fef0: 6e74 0d0a 6672 6f6d 2070 6466 6d69 6e65  nt..from pdfmine
-0000ff00: 722e 7064 6670 6167 6520 696d 706f 7274  r.pdfpage import
-0000ff10: 2050 4446 5061 6765 0d0a 6672 6f6d 2070   PDFPage..from p
-0000ff20: 6466 6d69 6e65 722e 7064 6670 6167 6520  dfminer.pdfpage 
-0000ff30: 696d 706f 7274 2050 4446 5465 7874 4578  import PDFTextEx
-0000ff40: 7472 6163 7469 6f6e 4e6f 7441 6c6c 6f77  tractionNotAllow
-0000ff50: 6564 0d0a 6672 6f6d 2070 6466 6d69 6e65  ed..from pdfmine
-0000ff60: 722e 7064 6669 6e74 6572 7020 696d 706f  r.pdfinterp impo
-0000ff70: 7274 2050 4446 5265 736f 7572 6365 4d61  rt PDFResourceMa
-0000ff80: 6e61 6765 720d 0a66 726f 6d20 7064 666d  nager..from pdfm
-0000ff90: 696e 6572 2e70 6466 696e 7465 7270 2069  iner.pdfinterp i
-0000ffa0: 6d70 6f72 7420 5044 4650 6167 6549 6e74  mport PDFPageInt
-0000ffb0: 6572 7072 6574 6572 0d0a 2366 726f 6d20  erpreter..#from 
-0000ffc0: 5374 7269 6e67 494f 2069 6d70 6f72 7420  StringIO import 
-0000ffd0: 5374 7269 6e67 494f 0d0a 6672 6f6d 2069  StringIO..from i
-0000ffe0: 6f20 696d 706f 7274 2053 7472 696e 6749  o import StringI
-0000fff0: 4f0d 0a69 6d70 6f72 7420 7572 6c6c 6962  O..import urllib
-00010000: 2e72 6571 7565 7374 2020 0d0a 2369 6d70  .request  ..#imp
-00010010: 6f72 7420 746d 6c74 6578 7473 756d 6d61  ort tmltextsumma
-00010020: 7279 0d0a 696d 706f 7274 206f 730d 0a69  ry..import os..i
-00010030: 6d70 6f72 7420 6461 7465 7469 6d65 0d0a  mport datetime..
-00010040: 2369 6d70 6f72 7420 676c 6f62 0d0a 0d0a  #import glob....
-00010050: 0d0a 6672 6f6d 2070 6466 6d69 6e65 722e  ..from pdfminer.
-00010060: 6c61 796f 7574 2069 6d70 6f72 7420 4c41  layout import LA
-00010070: 5061 7261 6d73 0d0a 6672 6f6d 2070 6466  Params..from pdf
-00010080: 6d69 6e65 722e 636f 6e76 6572 7465 7220  miner.converter 
-00010090: 696d 706f 7274 2054 6578 7443 6f6e 7665  import TextConve
-000100a0: 7274 6572 0d0a 200d 0a63 6c61 7373 204d  rter.. ..class M
-000100b0: 7950 6172 7365 7228 6f62 6a65 6374 293a  yParser(object):
-000100c0: 0d0a 2020 2020 6465 6620 5f5f 696e 6974  ..    def __init
-000100d0: 5f5f 2873 656c 662c 2070 6466 293a 0d0a  __(self, pdf):..
-000100e0: 2020 2020 2020 2020 2323 2053 6e69 7070          ## Snipp
-000100f0: 6564 2061 6461 7074 6564 2066 726f 6d20  ed adapted from 
-00010100: 5975 7375 6b65 2053 6869 6e79 616d 6173  Yusuke Shinyamas
-00010110: 200d 0a20 2020 2020 2020 2023 5044 464d   ..        #PDFM
-00010120: 696e 6572 2064 6f63 756d 656e 7461 7469  iner documentati
-00010130: 6f6e 0d0a 2020 2020 2020 2020 2320 4372  on..        # Cr
-00010140: 6561 7465 2074 6865 2064 6f63 756d 656e  eate the documen
-00010150: 7420 6d6f 6465 6c20 6672 6f6d 2074 6865  t model from the
-00010160: 2066 696c 650d 0a20 2020 2020 2020 2070   file..        p
-00010170: 6172 7365 7220 3d20 5044 4650 6172 7365  arser = PDFParse
-00010180: 7228 6f70 656e 2870 6466 2c20 2772 6227  r(open(pdf, 'rb'
-00010190: 2929 0d0a 2020 2020 2020 2020 646f 6375  ))..        docu
-000101a0: 6d65 6e74 203d 2050 4446 446f 6375 6d65  ment = PDFDocume
-000101b0: 6e74 2870 6172 7365 7229 0d0a 2020 2020  nt(parser)..    
-000101c0: 2020 2020 2320 5472 7920 746f 2070 6172      # Try to par
-000101d0: 7365 2074 6865 2064 6f63 756d 656e 740d  se the document.
-000101e0: 0a20 2020 2020 2020 2069 6620 6e6f 7420  .        if not 
-000101f0: 646f 6375 6d65 6e74 2e69 735f 6578 7472  document.is_extr
-00010200: 6163 7461 626c 653a 0d0a 2020 2020 2020  actable:..      
-00010210: 2020 2020 2020 7261 6973 6520 5044 4654        raise PDFT
-00010220: 6578 7445 7874 7261 6374 696f 6e4e 6f74  extExtractionNot
-00010230: 416c 6c6f 7765 640d 0a20 2020 2020 2020  Allowed..       
-00010240: 2023 2043 7265 6174 6520 6120 5044 4620   # Create a PDF 
-00010250: 7265 736f 7572 6365 206d 616e 6167 6572  resource manager
-00010260: 206f 626a 6563 7420 0d0a 2020 2020 2020   object ..      
-00010270: 2020 2320 7468 6174 2073 746f 7265 7320    # that stores 
-00010280: 7368 6172 6564 2072 6573 6f75 7263 6573  shared resources
-00010290: 2e0d 0a20 2020 2020 2020 2072 7372 636d  ...        rsrcm
-000102a0: 6772 203d 2050 4446 5265 736f 7572 6365  gr = PDFResource
-000102b0: 4d61 6e61 6765 7228 290d 0a20 2020 2020  Manager()..     
-000102c0: 2020 2023 2043 7265 6174 6520 6120 6275     # Create a bu
-000102d0: 6666 6572 2066 6f72 2074 6865 2070 6172  ffer for the par
-000102e0: 7365 6420 7465 7874 0d0a 2020 2020 2020  sed text..      
-000102f0: 2020 7265 7473 7472 203d 2053 7472 696e    retstr = Strin
-00010300: 6749 4f28 290d 0a20 2020 2020 2020 2023  gIO()..        #
-00010310: 2053 7061 6369 6e67 2070 6172 616d 6574   Spacing paramet
-00010320: 6572 7320 666f 7220 7061 7273 696e 670d  ers for parsing.
-00010330: 0a20 2020 2020 2020 206c 6170 6172 616d  .        laparam
-00010340: 7320 3d20 4c41 5061 7261 6d73 2829 0d0a  s = LAParams()..
-00010350: 2020 2020 2020 2020 636f 6465 6320 3d20          codec = 
-00010360: 2775 7466 2d38 270d 0a20 0d0a 2020 2020  'utf-8'.. ..    
-00010370: 2020 2020 2320 4372 6561 7465 2061 2050      # Create a P
-00010380: 4446 2064 6576 6963 6520 6f62 6a65 6374  DF device object
-00010390: 0d0a 2020 2020 2020 2020 6465 7669 6365  ..        device
-000103a0: 203d 2054 6578 7443 6f6e 7665 7274 6572   = TextConverter
-000103b0: 2872 7372 636d 6772 2c20 7265 7473 7472  (rsrcmgr, retstr
-000103c0: 2c0d 0a20 2020 2020 2020 2020 2020 2020  ,..             
-000103d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000103e0: 2020 6c61 7061 7261 6d73 203d 206c 6170    laparams = lap
-000103f0: 6172 616d 7329 0d0a 2020 2020 2020 2020  arams)..        
-00010400: 2320 4372 6561 7465 2061 2050 4446 2069  # Create a PDF i
-00010410: 6e74 6572 7072 6574 6572 206f 626a 6563  nterpreter objec
-00010420: 740d 0a20 2020 2020 2020 2069 6e74 6572  t..        inter
-00010430: 7072 6574 6572 203d 2050 4446 5061 6765  preter = PDFPage
-00010440: 496e 7465 7270 7265 7465 7228 7273 7263  Interpreter(rsrc
-00010450: 6d67 722c 2064 6576 6963 6529 0d0a 2020  mgr, device)..  
-00010460: 2020 2020 2020 2320 5072 6f63 6573 7320        # Process 
-00010470: 6561 6368 2070 6167 6520 636f 6e74 6169  each page contai
-00010480: 6e65 6420 696e 2074 6865 2064 6f63 756d  ned in the docum
-00010490: 656e 742e 0d0a 2020 2020 2020 2020 666f  ent...        fo
-000104a0: 7220 7061 6765 2069 6e20 5044 4650 6167  r page in PDFPag
-000104b0: 652e 6372 6561 7465 5f70 6167 6573 2864  e.create_pages(d
-000104c0: 6f63 756d 656e 7429 3a0d 0a20 2020 2020  ocument):..     
-000104d0: 2020 2020 2020 2069 6e74 6572 7072 6574         interpret
-000104e0: 6572 2e70 726f 6365 7373 5f70 6167 6528  er.process_page(
-000104f0: 7061 6765 290d 0a20 2020 2020 2020 2020  page)..         
-00010500: 0d0a 2020 2020 2020 2020 7365 6c66 2e72  ..        self.r
-00010510: 6563 6f72 6473 2020 2020 2020 2020 2020  ecords          
-00010520: 2020 3d20 5b5d 0d0a 2020 2020 2020 2020    = []..        
-00010530: 200d 0a20 2020 2020 2020 206c 696e 6573   ..        lines
-00010540: 203d 2072 6574 7374 722e 6765 7476 616c   = retstr.getval
-00010550: 7565 2829 2e73 706c 6974 6c69 6e65 7328  ue().splitlines(
-00010560: 290d 0a20 2020 2020 2020 2066 6f72 206c  )..        for l
-00010570: 696e 6520 696e 206c 696e 6573 3a0d 0a20  ine in lines:.. 
-00010580: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-00010590: 6861 6e64 6c65 5f6c 696e 6528 6c69 6e65  handle_line(line
-000105a0: 290d 0a20 2020 2020 0d0a 2020 2020 6465  )..     ..    de
-000105b0: 6620 6861 6e64 6c65 5f6c 696e 6528 7365  f handle_line(se
-000105c0: 6c66 2c20 6c69 6e65 293a 0d0a 2020 2020  lf, line):..    
-000105d0: 2020 2020 2320 4375 7374 6f6d 697a 6520      # Customize 
-000105e0: 796f 7572 206c 696e 652d 6279 2d6c 696e  your line-by-lin
-000105f0: 6520 7061 7273 6572 2068 6572 650d 0a20  e parser here.. 
-00010600: 2020 2020 2020 2073 656c 662e 7265 636f         self.reco
-00010610: 7264 732e 6170 7065 6e64 286c 696e 6529  rds.append(line)
-00010620: 0d0a 0d0a 6465 6620 7363 7261 7065 7064  ....def scrapepd
-00010630: 6628 7468 6575 726c 2c66 6e29 3a0d 0a20  f(theurl,fn):.. 
-00010640: 2020 2073 6372 6170 6564 5f64 6174 6120     scraped_data 
-00010650: 3d20 7572 6c6c 6962 2e72 6571 7565 7374  = urllib.request
-00010660: 2e75 726c 6f70 656e 2874 6865 7572 6c29  .urlopen(theurl)
-00010670: 2020 0d0a 2020 2020 6669 6c65 203d 206f    ..    file = o
-00010680: 7065 6e28 666e 2c20 2777 6227 290d 0a20  pen(fn, 'wb').. 
-00010690: 2020 2066 696c 652e 7772 6974 6528 7363     file.write(sc
-000106a0: 7261 7065 645f 6461 7461 2e72 6561 6428  raped_data.read(
-000106b0: 2929 0d0a 2020 2020 6669 6c65 2e63 6c6f  ))..    file.clo
-000106c0: 7365 2829 0d0a 2020 2020 2372 6574 7572  se()..    #retur
-000106d0: 6e20 6172 7469 636c 655f 7465 7874 0d0a  n article_text..
-000106e0: 0d0a 6465 6620 7374 6172 7470 6466 7265  ..def startpdfre
-000106f0: 6164 696e 6728 6669 6c65 6e61 6d65 2c66  ading(filename,f
-00010700: 7661 6c75 652c 6b65 7963 6f75 6e74 293a  value,keycount):
-00010710: 0d0a 2020 236f 732e 7061 7468 2e61 6273  ..  #os.path.abs
-00010720: 7061 7468 286f 732e 6765 7463 7764 2829  path(os.getcwd()
-00010730: 290d 0a20 2074 6865 7369 7a65 3d72 6f75  )..  thesize=rou
-00010740: 6e64 286f 732e 7061 7468 2e67 6574 7369  nd(os.path.getsi
-00010750: 7a65 2866 696c 656e 616d 6529 2f31 3030  ze(filename)/100
-00010760: 3030 3030 2c32 290d 0a20 206d 5f74 696d  0000,2)..  m_tim
-00010770: 6520 3d20 6f73 2e70 6174 682e 6765 746d  e = os.path.getm
-00010780: 7469 6d65 2866 696c 656e 616d 6529 0d0a  time(filename)..
-00010790: 2020 6474 5f6d 203d 2064 6174 6574 696d    dt_m = datetim
-000107a0: 652e 6461 7465 7469 6d65 2e66 726f 6d74  e.datetime.fromt
-000107b0: 696d 6573 7461 6d70 286d 5f74 696d 6529  imestamp(m_time)
-000107c0: 0d0a 2020 635f 7469 6d65 203d 206f 732e  ..  c_time = os.
-000107d0: 7061 7468 2e67 6574 6374 696d 6528 6669  path.getctime(fi
-000107e0: 6c65 6e61 6d65 290d 0a20 2023 2063 6f6e  lename)..  # con
-000107f0: 7665 7274 2063 7265 6174 696f 6e20 7469  vert creation ti
-00010800: 6d65 7374 616d 7020 696e 746f 2044 6174  mestamp into Dat
-00010810: 6554 696d 6520 6f62 6a65 6374 0d0a 2020  eTime object..  
-00010820: 6474 5f63 203d 2064 6174 6574 696d 652e  dt_c = datetime.
-00010830: 6461 7465 7469 6d65 2e66 726f 6d74 696d  datetime.fromtim
-00010840: 6573 7461 6d70 2863 5f74 696d 6529 0d0a  estamp(c_time)..
-00010850: 2020 636f 203d 2073 7472 2864 745f 6329    co = str(dt_c)
-00010860: 205b 303a 3139 5d0d 0a20 206d 6f20 3d20   [0:19]..  mo = 
-00010870: 7374 7228 6474 5f6d 2920 5b30 3a31 395d  str(dt_m) [0:19]
-00010880: 0d0a 0d0a 2020 7020 3d20 4d79 5061 7273  ....  p = MyPars
-00010890: 6572 2866 696c 656e 616d 6529 0d0a 2020  er(filename)..  
-000108a0: 7468 6574 6578 743d 275c 6e27 2e6a 6f69  thetext='\n'.joi
-000108b0: 6e28 702e 7265 636f 7264 7329 0d0a 2020  n(p.records)..  
-000108c0: 6172 7469 636c 655f 7465 7874 3d74 6865  article_text=the
-000108d0: 7465 7874 2e65 6e63 6f64 6528 2775 7466  text.encode('utf
-000108e0: 3827 290d 0a20 2073 756d 6d61 7269 7a65  8')..  summarize
-000108f0: 643d 227b 5c22 6669 6c65 6e61 6d65 5c22  d="{\"filename\"
-00010900: 3a5c 2222 202b 2066 696c 656e 616d 6520  :\"" + filename 
-00010910: 2b20 225c 222c 5c22 6669 6c65 7369 7a65  + "\",\"filesize
-00010920: 284d 4229 5c22 3a22 2b73 7472 2874 6865  (MB)\":"+str(the
-00010930: 7369 7a65 292b 222c 5c22 6669 6c65 6372  size)+",\"filecr
-00010940: 6561 7465 646f 6e5c 223a 5c22 2220 2b20  eatedon\":\"" + 
-00010950: 636f 202b 2022 5c22 2c5c 2266 696c 656d  co + "\",\"filem
-00010960: 6f64 6966 6965 646f 6e5c 223a 5c22 2220  odifiedon\":\"" 
-00010970: 2b20 6d6f 202b 2022 5c22 2c5c 226b 6579  + mo + "\",\"key
-00010980: 776f 7264 735c 223a 2220 2b20 2073 7461  words\":" +  sta
-00010990: 7274 7375 6d6d 6172 7928 7468 6574 6578  rtsummary(thetex
-000109a0: 742c 6676 616c 7565 2c6b 6579 636f 756e  t,fvalue,keycoun
-000109b0: 7429 0d0a 2023 2070 7269 6e74 2873 756d  t).. # print(sum
-000109c0: 6d61 7269 7a65 6429 0d0a 2020 7265 7475  marized)..  retu
-000109d0: 726e 2073 756d 6d61 7269 7a65 640d 0a0d  rn summarized...
-000109e0: 0a0d 0a23 2323 2323 2323 2323 2323 2323  ...#############
-000109f0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00010a00: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00010a10: 2323 0d0a 2320 4465 7665 6c6f 7065 6420  ##..# Developed 
-00010a20: 6279 204f 5449 4353 2041 6476 616e 6365  by OTICS Advance
-00010a30: 6420 416e 616c 7974 6963 730d 0a23 2053  d Analytics..# S
-00010a40: 6562 6173 7469 616e 204d 6175 7269 6365  ebastian Maurice
-00010a50: 0d0a 0d0a 696d 706f 7274 2062 7334 2061  ....import bs4 a
-00010a60: 7320 6273 2020 0d0a 696d 706f 7274 2075  s bs  ..import u
-00010a70: 726c 6c69 622e 7265 7175 6573 7420 200d  rllib.request  .
-00010a80: 0a69 6d70 6f72 7420 7265 0d0a 696d 706f  .import re..impo
-00010a90: 7274 206e 6c74 6b0d 0a66 726f 6d20 6e6c  rt nltk..from nl
-00010aa0: 746b 2e74 6f6b 656e 697a 6520 696d 706f  tk.tokenize impo
-00010ab0: 7274 2052 6567 6578 7054 6f6b 656e 697a  rt RegexpTokeniz
-00010ac0: 6572 0d0a 696d 706f 7274 2068 6561 7071  er..import heapq
-00010ad0: 0d0a 696d 706f 7274 2073 7973 0d0a 696d  ..import sys..im
-00010ae0: 706f 7274 206f 730d 0a66 726f 6d20 7261  port os..from ra
-00010af0: 6b65 5f6e 6c74 6b20 696d 706f 7274 204d  ke_nltk import M
-00010b00: 6574 7269 632c 5261 6b65 0d0a 696d 706f  etric,Rake..impo
-00010b10: 7274 206a 736f 6e0d 0a69 6d70 6f72 7420  rt json..import 
-00010b20: 7061 6e64 6173 2061 7320 7064 0d0a 696d  pandas as pd..im
-00010b30: 706f 7274 206e 6c74 6b2e 636f 7270 7573  port nltk.corpus
-00010b40: 0d0a 6672 6f6d 206e 6c74 6b2e 636f 7270  ..from nltk.corp
-00010b50: 7573 2069 6d70 6f72 7420 7374 6f70 776f  us import stopwo
-00010b60: 7264 730d 0a66 726f 6d20 7465 7874 626c  rds..from textbl
-00010b70: 6f62 2069 6d70 6f72 7420 5465 7874 426c  ob import TextBl
-00010b80: 6f62 0d0a 6672 6f6d 2074 6578 7462 6c6f  ob..from textblo
-00010b90: 6220 696d 706f 7274 2057 6f72 640d 0a66  b import Word..f
-00010ba0: 726f 6d20 736b 6c65 6172 6e2e 6665 6174  rom sklearn.feat
-00010bb0: 7572 655f 6578 7472 6163 7469 6f6e 2e74  ure_extraction.t
-00010bc0: 6578 7420 696d 706f 7274 2054 6669 6466  ext import Tfidf
-00010bd0: 5472 616e 7366 6f72 6d65 722c 5466 6964  Transformer,Tfid
-00010be0: 6656 6563 746f 7269 7a65 720d 0a66 726f  fVectorizer..fro
-00010bf0: 6d20 736b 6c65 6172 6e2e 6665 6174 7572  m sklearn.featur
-00010c00: 655f 6578 7472 6163 7469 6f6e 2e74 6578  e_extraction.tex
-00010c10: 7420 696d 706f 7274 2043 6f75 6e74 5665  t import CountVe
-00010c20: 6374 6f72 697a 6572 0d0a 236e 6c74 6b2e  ctorizer..#nltk.
-00010c30: 646f 776e 6c6f 6164 2827 7075 6e6b 7427  download('punkt'
-00010c40: 290d 0a69 6d70 6f72 7420 7761 726e 696e  )..import warnin
-00010c50: 6773 0d0a 7761 726e 696e 6773 2e66 696c  gs..warnings.fil
-00010c60: 7465 7277 6172 6e69 6e67 7328 2269 676e  terwarnings("ign
-00010c70: 6f72 6522 290d 0a0d 0a23 6e6c 746b 2e64  ore")....#nltk.d
-00010c80: 6f77 6e6c 6f61 6428 2773 746f 7077 6f72  ownload('stopwor
-00010c90: 6473 2729 0d0a 0d0a 6465 6620 6765 745f  ds')....def get_
-00010ca0: 7374 6f70 5f77 6f72 6473 2829 3a0d 0a20  stop_words():.. 
-00010cb0: 2020 2022 2222 6c6f 6164 2073 746f 7020     """load stop 
-00010cc0: 776f 7264 7320 2222 220d 0a20 2020 2072  words """..    r
-00010cd0: 6574 7572 6e20 7374 6f70 776f 7264 732e  eturn stopwords.
-00010ce0: 776f 7264 7328 2765 6e67 6c69 7368 2729  words('english')
-00010cf0: 0d0a 2020 2020 0d0a 2323 2020 2020 7769  ..    ..##    wi
-00010d00: 7468 206f 7065 6e28 2773 746f 7077 6f72  th open('stopwor
-00010d10: 6473 2e74 7874 272c 2027 7227 2c20 656e  ds.txt', 'r', en
-00010d20: 636f 6469 6e67 3d22 7574 662d 3822 2920  coding="utf-8") 
-00010d30: 6173 2066 3a0d 0a23 2320 2020 2020 2020  as f:..##       
-00010d40: 2073 746f 7077 6f72 6473 203d 2066 2e72   stopwords = f.r
-00010d50: 6561 646c 696e 6573 2829 0d0a 2323 2020  eadlines()..##  
-00010d60: 2020 2020 2020 7374 6f70 5f73 6574 203d        stop_set =
-00010d70: 2073 6574 286d 2e73 7472 6970 2829 2066   set(m.strip() f
-00010d80: 6f72 206d 2069 6e20 7374 6f70 776f 7264  or m in stopword
-00010d90: 7329 0d0a 2323 2020 2020 2020 2320 2070  s)..##      #  p
-00010da0: 7269 6e74 2866 726f 7a65 6e73 6574 2873  rint(frozenset(s
-00010db0: 746f 705f 7365 7429 290d 0a23 2320 2020  top_set))..##   
-00010dc0: 2020 2020 2072 6574 7572 6e20 6672 6f7a       return froz
-00010dd0: 656e 7365 7428 7374 6f70 5f73 6574 290d  enset(stop_set).
-00010de0: 0a0d 0a64 6566 2073 6372 6170 6577 6562  ...def scrapeweb
-00010df0: 2874 6865 7572 6c29 3a0d 0a20 2020 2073  (theurl):..    s
-00010e00: 6372 6170 6564 5f64 6174 6120 3d20 7572  craped_data = ur
-00010e10: 6c6c 6962 2e72 6571 7565 7374 2e75 726c  llib.request.url
-00010e20: 6f70 656e 2874 6865 7572 6c29 2020 0d0a  open(theurl)  ..
-00010e30: 2020 2020 6172 7469 636c 6520 3d20 7363      article = sc
-00010e40: 7261 7065 645f 6461 7461 2e72 6561 6428  raped_data.read(
-00010e50: 290d 0a0d 0a20 2020 2070 6172 7365 645f  )....    parsed_
-00010e60: 6172 7469 636c 6520 3d20 6273 2e42 6561  article = bs.Bea
-00010e70: 7574 6966 756c 536f 7570 2861 7274 6963  utifulSoup(artic
-00010e80: 6c65 2c27 6c78 6d6c 2729 0d0a 0d0a 2020  le,'lxml')....  
-00010e90: 2020 7061 7261 6772 6170 6873 203d 2070    paragraphs = p
-00010ea0: 6172 7365 645f 6172 7469 636c 652e 6669  arsed_article.fi
-00010eb0: 6e64 5f61 6c6c 2827 7027 290d 0a0d 0a20  nd_all('p').... 
-00010ec0: 2020 2061 7274 6963 6c65 5f74 6578 7420     article_text 
-00010ed0: 3d20 2222 0d0a 0d0a 2020 2020 666f 7220  = ""....    for 
-00010ee0: 7020 696e 2070 6172 6167 7261 7068 733a  p in paragraphs:
-00010ef0: 2020 0d0a 2020 2020 2020 2020 6172 7469    ..        arti
-00010f00: 636c 655f 7465 7874 202b 3d20 702e 7465  cle_text += p.te
-00010f10: 7874 0d0a 2020 2020 7265 7475 726e 2061  xt..    return a
-00010f20: 7274 6963 6c65 5f74 6578 7420 0d0a 0d0a  rticle_text ....
-00010f30: 6465 6620 636f 6e76 6572 7474 6f6c 6f77  def converttolow
-00010f40: 6572 6361 7365 2864 662c 636f 6c29 3a0d  ercase(df,col):.
-00010f50: 0a20 2020 2020 2064 665b 636f 6c5d 203d  .      df[col] =
-00010f60: 2064 665b 636f 6c5d 2e61 7070 6c79 286c   df[col].apply(l
-00010f70: 616d 6264 6120 783a 2022 2022 2e6a 6f69  ambda x: " ".joi
-00010f80: 6e28 782e 6c6f 7765 7228 2920 666f 7220  n(x.lower() for 
-00010f90: 7820 696e 2078 2e73 706c 6974 2829 2929  x in x.split()))
-00010fa0: 0d0a 2020 2020 2020 7265 7475 726e 2064  ..      return d
-00010fb0: 660d 0a20 2020 200d 0a64 6566 2072 656d  f..    ..def rem
-00010fc0: 6f76 6570 756e 6374 7561 7469 6f6e 2864  ovepunctuation(d
-00010fd0: 662c 636f 6c29 3a0d 0a20 2020 2020 2064  f,col):..      d
-00010fe0: 665b 636f 6c5d 203d 2064 665b 636f 6c5d  f[col] = df[col]
-00010ff0: 2e73 7472 2e72 6570 6c61 6365 2827 5b5e  .str.replace('[^
-00011000: 5c77 5c73 5d27 2c27 2729 0d0a 2020 2020  \w\s]','')..    
-00011010: 2020 7265 7475 726e 2064 660d 0a0d 0a64    return df....d
-00011020: 6566 2072 656d 6f76 6573 746f 7077 6f72  ef removestopwor
-00011030: 6473 2864 662c 636f 6c29 3a0d 0a20 2020  ds(df,col):..   
-00011040: 2020 2073 746f 7020 3d20 7374 6f70 776f     stop = stopwo
-00011050: 7264 732e 776f 7264 7328 2765 6e67 6c69  rds.words('engli
-00011060: 7368 2729 0d0a 2020 2020 2020 6466 5b63  sh')..      df[c
-00011070: 6f6c 5d20 3d20 6466 5b63 6f6c 5d2e 6170  ol] = df[col].ap
-00011080: 706c 7928 6c61 6d62 6461 2078 3a20 2220  ply(lambda x: " 
-00011090: 222e 6a6f 696e 2878 2066 6f72 2078 2069  ".join(x for x i
-000110a0: 6e20 782e 7370 6c69 7428 2920 6966 2078  n x.split() if x
-000110b0: 206e 6f74 2069 6e20 7374 6f70 2929 0d0a   not in stop))..
-000110c0: 2020 2020 2020 7265 7475 726e 2064 660d        return df.
-000110d0: 0a0d 0a64 6566 2072 656d 6f76 6563 6f6d  ...def removecom
-000110e0: 6d6f 6e77 6f72 6473 2864 662c 636f 6c29  monwords(df,col)
-000110f0: 3a0d 0a20 2020 2020 2066 7265 7120 3d20  :..      freq = 
-00011100: 7064 2e53 6572 6965 7328 2720 272e 6a6f  pd.Series(' '.jo
-00011110: 696e 2864 665b 636f 6c5d 292e 7370 6c69  in(df[col]).spli
-00011120: 7428 2929 2e76 616c 7565 5f63 6f75 6e74  t()).value_count
-00011130: 7328 295b 3a31 305d 0d0a 2020 2020 2020  s()[:10]..      
-00011140: 6672 6571 203d 206c 6973 7428 6672 6571  freq = list(freq
-00011150: 2e69 6e64 6578 290d 0a20 2020 2020 2064  .index)..      d
-00011160: 665b 636f 6c5d 203d 2064 665b 636f 6c5d  f[col] = df[col]
-00011170: 2e61 7070 6c79 286c 616d 6264 6120 783a  .apply(lambda x:
-00011180: 2022 2022 2e6a 6f69 6e28 7820 666f 7220   " ".join(x for 
-00011190: 7820 696e 2078 2e73 706c 6974 2829 2069  x in x.split() i
-000111a0: 6620 7820 6e6f 7420 696e 2066 7265 7129  f x not in freq)
-000111b0: 290d 0a20 2020 2020 2072 6574 7572 6e20  )..      return 
-000111c0: 6466 0d0a 0d0a 6465 6620 7265 6d6f 7665  df....def remove
-000111d0: 7261 7265 776f 7264 7328 6466 2c63 6f6c  rarewords(df,col
-000111e0: 293a 0d0a 2020 2020 2020 6672 6571 203d  ):..      freq =
-000111f0: 2070 642e 5365 7269 6573 2827 2027 2e6a   pd.Series(' '.j
-00011200: 6f69 6e28 6466 5b63 6f6c 5d29 2e73 706c  oin(df[col]).spl
-00011210: 6974 2829 292e 7661 6c75 655f 636f 756e  it()).value_coun
-00011220: 7473 2829 5b2d 3130 3a5d 0d0a 2020 2020  ts()[-10:]..    
-00011230: 2020 6672 6571 203d 206c 6973 7428 6672    freq = list(fr
-00011240: 6571 2e69 6e64 6578 290d 0a20 2020 2020  eq.index)..     
-00011250: 2064 665b 636f 6c5d 203d 2064 665b 636f   df[col] = df[co
-00011260: 6c5d 2e61 7070 6c79 286c 616d 6264 6120  l].apply(lambda 
-00011270: 783a 2022 2022 2e6a 6f69 6e28 7820 666f  x: " ".join(x fo
-00011280: 7220 7820 696e 2078 2e73 706c 6974 2829  r x in x.split()
-00011290: 2069 6620 7820 6e6f 7420 696e 2066 7265   if x not in fre
-000112a0: 7129 290d 0a20 2020 2020 2072 6574 7572  q))..      retur
-000112b0: 6e20 6466 0d0a 0d0a 6465 6620 636f 7272  n df....def corr
-000112c0: 6563 7473 7065 6c6c 696e 6728 6466 2c63  ectspelling(df,c
-000112d0: 6f6c 293a 0d0a 2020 2020 2020 6466 5b63  ol):..      df[c
-000112e0: 6f6c 5d5b 3a35 5d2e 6170 706c 7928 6c61  ol][:5].apply(la
-000112f0: 6d62 6461 2078 3a20 7374 7228 5465 7874  mbda x: str(Text
-00011300: 426c 6f62 2878 292e 636f 7272 6563 7428  Blob(x).correct(
-00011310: 2929 290d 0a20 2020 2020 2072 6574 7572  )))..      retur
-00011320: 6e20 6466 0d0a 0d0a 6465 6620 6c65 6d6d  n df....def lemm
-00011330: 6174 697a 6174 696f 6e28 6466 2c63 6f6c  atization(df,col
-00011340: 293a 0d0a 2020 2020 2020 6466 5b63 6f6c  ):..      df[col
-00011350: 5d20 3d20 6466 5b63 6f6c 5d2e 6170 706c  ] = df[col].appl
-00011360: 7928 6c61 6d62 6461 2078 3a20 2220 222e  y(lambda x: " ".
-00011370: 6a6f 696e 285b 576f 7264 2877 6f72 6429  join([Word(word)
-00011380: 2e6c 656d 6d61 7469 7a65 2829 2066 6f72  .lemmatize() for
-00011390: 2077 6f72 6420 696e 2078 2e73 706c 6974   word in x.split
-000113a0: 2829 5d29 290d 0a20 2020 2020 2072 6574  ()]))..      ret
-000113b0: 7572 6e20 6466 0d0a 0d0a 6465 6620 7472  urn df....def tr
-000113c0: 6169 6e76 6563 7428 6376 2c74 626f 772c  ainvect(cv,tbow,
-000113d0: 6466 2c63 6f6c 2c6d 6178 6b65 7977 6f72  df,col,maxkeywor
-000113e0: 6473 293a 0d0a 2020 2020 2020 7465 7874  ds):..      text
-000113f0: 3d64 665b 636f 6c5d 2e74 6f6c 6973 7428  =df[col].tolist(
-00011400: 290d 0a20 2020 2020 2074 6669 6466 203d  )..      tfidf =
-00011410: 2054 6669 6466 5472 616e 7366 6f72 6d65   TfidfTransforme
-00011420: 7228 736d 6f6f 7468 5f69 6466 3d54 7275  r(smooth_idf=Tru
-00011430: 652c 7573 655f 6964 663d 5472 7565 290d  e,use_idf=True).
-00011440: 0a20 2020 2020 2074 6669 6466 2e66 6974  .      tfidf.fit
-00011450: 2874 626f 7729 0d0a 2020 2020 2020 7466  (tbow)..      tf
-00011460: 5f69 6466 5f76 6563 746f 723d 7466 6964  _idf_vector=tfid
-00011470: 662e 7472 616e 7366 6f72 6d28 6376 2e74  f.transform(cv.t
-00011480: 7261 6e73 666f 726d 2874 6578 7429 290d  ransform(text)).
-00011490: 0a20 2020 2020 2073 6f72 7465 6469 7465  .      sortedite
-000114a0: 6d73 3d73 6f72 745f 636f 6f28 7466 5f69  ms=sort_coo(tf_i
-000114b0: 6466 5f76 6563 746f 722e 746f 636f 6f28  df_vector.tocoo(
-000114c0: 2929 0d0a 2020 2020 2020 6665 6174 7572  ))..      featur
-000114d0: 656e 616d 6573 3d63 762e 6765 745f 6665  enames=cv.get_fe
-000114e0: 6174 7572 655f 6e61 6d65 735f 6f75 7428  ature_names_out(
-000114f0: 290d 0a20 2020 2020 206b 6579 776f 7264  )..      keyword
-00011500: 733d 6578 7472 6163 745f 746f 706e 5f66  s=extract_topn_f
-00011510: 726f 6d5f 7665 6374 6f72 2866 6561 7475  rom_vector(featu
-00011520: 7265 6e61 6d65 732c 736f 7274 6564 6974  renames,sortedit
-00011530: 656d 732c 6d61 786b 6579 776f 7264 7329  ems,maxkeywords)
-00011540: 0d0a 2020 2020 2020 6b65 7977 6f72 6473  ..      keywords
-00011550: 3d6a 736f 6e2e 6475 6d70 7328 6b65 7977  =json.dumps(keyw
-00011560: 6f72 6473 290d 0a20 2020 2020 2320 7072  ords)..     # pr
-00011570: 696e 7428 6b65 7977 6f72 6473 290d 0a20  int(keywords).. 
-00011580: 2020 2020 2072 6574 7572 6e20 6b65 7977       return keyw
-00011590: 6f72 6473 0d0a 0d0a 6465 6620 7472 6169  ords....def trai
-000115a0: 6e62 6f77 2864 662c 636f 6c29 3a0d 0a20  nbow(df,col):.. 
-000115b0: 2020 2020 206d 796c 6973 743d 6466 5b63       mylist=df[c
-000115c0: 6f6c 5d2e 746f 6c69 7374 2829 0d0a 2020  ol].tolist()..  
-000115d0: 2020 2020 7374 6f70 776f 7264 733d 6765      stopwords=ge
-000115e0: 745f 7374 6f70 5f77 6f72 6473 2829 0d0a  t_stop_words()..
-000115f0: 2020 2020 2020 6376 203d 2043 6f75 6e74        cv = Count
-00011600: 5665 6374 6f72 697a 6572 2873 746f 705f  Vectorizer(stop_
-00011610: 776f 7264 733d 7374 6f70 776f 7264 7329  words=stopwords)
-00011620: 0d0a 2020 2020 2020 7472 6169 6e5f 626f  ..      train_bo
-00011630: 7720 3d20 6376 2e66 6974 5f74 7261 6e73  w = cv.fit_trans
-00011640: 666f 726d 286d 796c 6973 7429 0d0a 2020  form(mylist)..  
-00011650: 2020 2020 2370 7269 6e74 286c 6973 7428      #print(list(
-00011660: 6376 2e76 6f63 6162 756c 6172 795f 2e6b  cv.vocabulary_.k
-00011670: 6579 7328 2929 290d 0a20 2020 2020 2072  eys()))..      r
-00011680: 6574 7572 6e20 6376 2c74 7261 696e 5f62  eturn cv,train_b
-00011690: 6f77 0d0a 0d0a 200d 0a64 6566 2073 6f72  ow.... ..def sor
-000116a0: 745f 636f 6f28 636f 6f5f 6d61 7472 6978  t_coo(coo_matrix
-000116b0: 293a 0d0a 2020 2020 7475 706c 6573 203d  ):..    tuples =
-000116c0: 207a 6970 2863 6f6f 5f6d 6174 7269 782e   zip(coo_matrix.
-000116d0: 636f 6c2c 2063 6f6f 5f6d 6174 7269 782e  col, coo_matrix.
-000116e0: 6461 7461 290d 0a20 2020 2072 6574 7572  data)..    retur
-000116f0: 6e20 736f 7274 6564 2874 7570 6c65 732c  n sorted(tuples,
-00011700: 206b 6579 3d6c 616d 6264 6120 783a 2028   key=lambda x: (
-00011710: 785b 315d 2c20 785b 305d 292c 2072 6576  x[1], x[0]), rev
-00011720: 6572 7365 3d54 7275 6529 0d0a 0d0a 6465  erse=True)....de
-00011730: 6620 6578 7472 6163 745f 746f 706e 5f66  f extract_topn_f
-00011740: 726f 6d5f 7665 6374 6f72 2866 6561 7475  rom_vector(featu
-00011750: 7265 5f6e 616d 6573 2c20 736f 7274 6564  re_names, sorted
-00011760: 5f69 7465 6d73 2c20 746f 706e 3d31 3029  _items, topn=10)
-00011770: 3a0d 0a20 2020 2022 2222 6765 7420 7468  :..    """get th
-00011780: 6520 6665 6174 7572 6520 6e61 6d65 7320  e feature names 
-00011790: 616e 6420 7466 2d69 6466 2073 636f 7265  and tf-idf score
-000117a0: 206f 6620 746f 7020 6e20 6974 656d 7322   of top n items"
-000117b0: 2222 0d0a 2020 2020 0d0a 2020 2020 2375  ""..    ..    #u
-000117c0: 7365 206f 6e6c 7920 746f 706e 2069 7465  se only topn ite
-000117d0: 6d73 2066 726f 6d20 7665 6374 6f72 0d0a  ms from vector..
-000117e0: 2020 2020 736f 7274 6564 5f69 7465 6d73      sorted_items
-000117f0: 203d 2073 6f72 7465 645f 6974 656d 735b   = sorted_items[
-00011800: 3a74 6f70 6e5d 0d0a 0d0a 2020 2020 7363  :topn]....    sc
-00011810: 6f72 655f 7661 6c73 203d 205b 5d0d 0a20  ore_vals = [].. 
-00011820: 2020 2066 6561 7475 7265 5f76 616c 7320     feature_vals 
-00011830: 3d20 5b5d 0d0a 0d0a 2020 2020 666f 7220  = []....    for 
-00011840: 6964 782c 2073 636f 7265 2069 6e20 736f  idx, score in so
-00011850: 7274 6564 5f69 7465 6d73 3a20 2020 2020  rted_items:     
-00011860: 2020 200d 0a20 2020 2020 2020 2020 2066     ..          f
-00011870: 6e61 6d65 203d 2066 6561 7475 7265 5f6e  name = feature_n
-00011880: 616d 6573 5b69 6478 5d0d 0a20 2020 2020  ames[idx]..     
-00011890: 2020 2020 2069 6620 6c65 6e28 666e 616d       if len(fnam
-000118a0: 6529 3e33 3a0d 0a20 2020 2020 2020 2023  e)>3:..        #
-000118b0: 6b65 6570 2074 7261 636b 206f 6620 6665  keep track of fe
-000118c0: 6174 7572 6520 6e61 6d65 2061 6e64 2069  ature name and i
-000118d0: 7473 2063 6f72 7265 7370 6f6e 6469 6e67  ts corresponding
-000118e0: 2073 636f 7265 0d0a 2020 2020 2020 2020   score..        
-000118f0: 2020 2020 7363 6f72 655f 7661 6c73 2e61      score_vals.a
-00011900: 7070 656e 6428 726f 756e 6428 7363 6f72  ppend(round(scor
-00011910: 652c 2033 2929 0d0a 2020 2020 2020 2020  e, 3))..        
-00011920: 2020 2020 6665 6174 7572 655f 7661 6c73      feature_vals
-00011930: 2e61 7070 656e 6428 6665 6174 7572 655f  .append(feature_
-00011940: 6e61 6d65 735b 6964 785d 290d 0a0d 0a20  names[idx]).... 
-00011950: 2020 2023 6372 6561 7465 2061 2074 7570     #create a tup
-00011960: 6c65 7320 6f66 2066 6561 7475 7265 2c73  les of feature,s
-00011970: 636f 7265 0d0a 2020 2020 2372 6573 756c  core..    #resul
-00011980: 7473 203d 207a 6970 2866 6561 7475 7265  ts = zip(feature
-00011990: 5f76 616c 732c 7363 6f72 655f 7661 6c73  _vals,score_vals
-000119a0: 290d 0a20 2020 2072 6573 756c 7473 3d20  )..    results= 
-000119b0: 7b7d 0d0a 2020 2020 666f 7220 6964 7820  {}..    for idx 
-000119c0: 696e 2072 616e 6765 286c 656e 2866 6561  in range(len(fea
-000119d0: 7475 7265 5f76 616c 7329 293a 0d0a 2020  ture_vals)):..  
-000119e0: 2020 2020 2020 7265 7375 6c74 735b 6665        results[fe
-000119f0: 6174 7572 655f 7661 6c73 5b69 6478 5d5d  ature_vals[idx]]
-00011a00: 3d73 636f 7265 5f76 616c 735b 6964 785d  =score_vals[idx]
-00011a10: 0d0a 2020 2020 0d0a 2020 2020 7265 7475  ..    ..    retu
-00011a20: 726e 2072 6573 756c 7473 0d0a 0d0a 6465  rn results....de
-00011a30: 6620 6765 746b 6579 776f 7264 7328 6d79  f getkeywords(my
-00011a40: 7465 7874 2c6d 6178 6b65 7977 6f72 6473  text,maxkeywords
-00011a50: 293a 0d0a 2020 2020 723d 5261 6b65 286d  ):..    r=Rake(m
-00011a60: 6178 5f6c 656e 6774 683d 3130 290d 0a20  ax_length=10).. 
-00011a70: 2020 2072 203d 2052 616b 6528 7261 6e6b     r = Rake(rank
-00011a80: 696e 675f 6d65 7472 6963 3d4d 6574 7269  ing_metric=Metri
-00011a90: 632e 4445 4752 4545 5f54 4f5f 4652 4551  c.DEGREE_TO_FREQ
-00011aa0: 5545 4e43 595f 5241 5449 4f29 0d0a 2020  UENCY_RATIO)..  
-00011ab0: 2020 2372 203d 2052 616b 6528 7261 6e6b    #r = Rake(rank
-00011ac0: 696e 675f 6d65 7472 6963 3d4d 6574 7269  ing_metric=Metri
-00011ad0: 632e 574f 5244 5f44 4547 5245 4529 0d0a  c.WORD_DEGREE)..
-00011ae0: 2020 2020 2372 203d 2052 616b 6528 7261      #r = Rake(ra
-00011af0: 6e6b 696e 675f 6d65 7472 6963 3d4d 6574  nking_metric=Met
-00011b00: 7269 632e 574f 5244 5f46 5245 5155 454e  ric.WORD_FREQUEN
-00011b10: 4359 290d 0a20 2020 2064 3d7b 2769 6e70  CY)..    d={'inp
-00011b20: 7574 273a 5b6d 7974 6578 745d 7d0d 0a20  ut':[mytext]}.. 
-00011b30: 2020 2064 6620 3d20 7064 2e44 6174 6146     df = pd.DataF
-00011b40: 7261 6d65 2864 290d 0a20 2020 2064 663d  rame(d)..    df=
-00011b50: 636f 6e76 6572 7474 6f6c 6f77 6572 6361  converttolowerca
-00011b60: 7365 2864 662c 2769 6e70 7574 2729 0d0a  se(df,'input')..
-00011b70: 2020 2020 6466 3d72 656d 6f76 6570 756e      df=removepun
-00011b80: 6374 7561 7469 6f6e 2864 662c 2769 6e70  ctuation(df,'inp
-00011b90: 7574 2729 0d0a 2020 2020 6466 3d72 656d  ut')..    df=rem
-00011ba0: 6f76 6573 746f 7077 6f72 6473 2864 662c  ovestopwords(df,
-00011bb0: 2769 6e70 7574 2729 0d0a 2020 2020 6466  'input')..    df
-00011bc0: 3d72 656d 6f76 6563 6f6d 6d6f 6e77 6f72  =removecommonwor
-00011bd0: 6473 2864 662c 2769 6e70 7574 2729 0d0a  ds(df,'input')..
-00011be0: 2020 2020 6466 3d72 656d 6f76 6572 6172      df=removerar
-00011bf0: 6577 6f72 6473 2864 662c 2769 6e70 7574  ewords(df,'input
-00011c00: 2729 0d0a 2020 2020 6466 3d63 6f72 7265  ')..    df=corre
-00011c10: 6374 7370 656c 6c69 6e67 2864 662c 2769  ctspelling(df,'i
-00011c20: 6e70 7574 2729 0d0a 2020 2020 6466 3d6c  nput')..    df=l
-00011c30: 656d 6d61 7469 7a61 7469 6f6e 2864 662c  emmatization(df,
-00011c40: 2769 6e70 7574 2729 0d0a 2020 2020 6d79  'input')..    my
-00011c50: 7465 7874 3d64 665b 2769 6e70 7574 275d  text=df['input']
-00011c60: 5b30 5d0d 0a20 2020 2063 762c 7477 3d74  [0]..    cv,tw=t
-00011c70: 7261 696e 626f 7728 6466 2c27 696e 7075  rainbow(df,'inpu
-00011c80: 7427 290d 0a20 2020 206b 6579 776f 7264  t')..    keyword
-00011c90: 733d 7472 6169 6e76 6563 7428 6376 2c74  s=trainvect(cv,t
-00011ca0: 772c 6466 2c27 696e 7075 7427 2c6d 6178  w,df,'input',max
-00011cb0: 6b65 7977 6f72 6473 290d 0a0d 0a20 2020  keywords)....   
-00011cc0: 2072 6574 7572 6e20 6b65 7977 6f72 6473   return keywords
-00011cd0: 0d0a 2020 2020 2370 7269 6e74 2874 7729  ..    #print(tw)
-00011ce0: 0d0a 2320 2020 206d 7974 6578 743d 7064  ..#    mytext=pd
-00011cf0: 2e53 6572 6965 7328 6d79 7465 7874 290d  .Series(mytext).
-00011d00: 0a20 2020 2023 7072 696e 7428 6d79 7465  .    #print(myte
-00011d10: 7874 290d 0a23 2020 2020 733d 732e 7374  xt)..#    s=s.st
-00011d20: 722e 7370 6c69 7428 290d 0a20 2020 2020  r.split()..     
-00011d30: 200d 0a20 2020 2320 6b77 3d72 2e65 7874   ..   # kw=r.ext
-00011d40: 7261 6374 5f6b 6579 776f 7264 735f 6672  ract_keywords_fr
-00011d50: 6f6d 5f74 6578 7428 6d79 7465 7874 290d  om_text(mytext).
-00011d60: 0a20 2020 2320 6b73 3d72 2e67 6574 5f72  .   # ks=r.get_r
-00011d70: 616e 6b65 645f 7068 7261 7365 735f 7769  anked_phrases_wi
-00011d80: 7468 5f73 636f 7265 7328 290d 0a20 2020  th_scores()..   
-00011d90: 200d 0a20 2020 2023 7072 696e 7428 6b65   ..    #print(ke
-00011da0: 7977 6f72 6473 290d 0a0d 0a23 6d79 7465  ywords)....#myte
-00011db0: 7874 3d22 4578 7472 656d 656c 7920 696d  xt="Extremely im
-00011dc0: 706f 7274 616e 7420 706f 696e 743a 2074  portant point: t
-00011dd0: 6865 2049 4446 2073 686f 756c 6420 616c  he IDF should al
-00011de0: 7761 7973 2062 6520 6261 7365 6420 6f6e  ways be based on
-00011df0: 2061 206c 6172 6765 2063 6f72 706f 7261   a large corpora
-00011e00: 2c20 616e 6420 7368 6f75 6c64 2062 6520  , and should be 
-00011e10: 7265 7072 6573 656e 7461 7469 7665 205c  representative \
-00011e20: 0d0a 236f 6620 7465 7874 7320 796f 7520  ..#of texts you 
-00011e30: 776f 756c 6420 6265 2075 7369 6e67 2074  would be using t
-00011e40: 6f20 6578 7472 6163 7420 6b65 7977 6f72  o extract keywor
-00011e50: 6473 2e20 49e2 8099 7665 2073 6565 6e20  ds. I...ve seen 
-00011e60: 7365 7665 7261 6c20 6172 7469 636c 6573  several articles
-00011e70: 206f 6e20 7468 6520 5765 6220 7468 6174   on the Web that
-00011e80: 2063 6f6d 7075 7465 2074 6865 2049 4446   compute the IDF
-00011e90: 2075 7369 6e67 2061 205c 0d0a 2368 616e   using a \..#han
-00011ea0: 6466 756c 206f 6620 646f 6375 6d65 6e74  dful of document
-00011eb0: 732e 2059 6f75 2077 696c 6c20 6465 6665  s. You will defe
-00011ec0: 6174 2074 6865 2077 686f 6c65 2070 7572  at the whole pur
-00011ed0: 706f 7365 206f 6620 4944 4620 7765 6967  pose of IDF weig
-00011ee0: 6874 696e 6720 6966 2069 7473 206e 6f74  hting if its not
-00011ef0: 2062 6173 6564 206f 6e20 6120 6c61 7267   based on a larg
-00011f00: 6520 636f 7270 6f72 6120 6173 220d 0a0d  e corpora as"...
-00011f10: 0a23 6765 746b 6579 776f 7264 7328 6d79  .#getkeywords(my
-00011f20: 7465 7874 290d 0a0d 0a64 6566 2064 6f73  text)....def dos
-00011f30: 756d 6d61 7279 2861 7274 6963 6c65 5f74  ummary(article_t
-00011f40: 6578 742c 6929 3a0d 0a0d 0a0d 0a20 2020  ext,i):......   
-00011f50: 2061 7274 6963 6c65 5f74 6578 7420 3d20   article_text = 
-00011f60: 7265 2e73 7562 2872 275c 5b5b 302d 395d  re.sub(r'\[[0-9]
-00011f70: 2a5c 5d27 2c20 2720 272c 2061 7274 6963  *\]', ' ', artic
-00011f80: 6c65 5f74 6578 7429 2020 0d0a 2020 2020  le_text)  ..    
-00011f90: 6172 7469 636c 655f 7465 7874 203d 2072  article_text = r
-00011fa0: 652e 7375 6228 7227 5c73 2b27 2c20 2720  e.sub(r'\s+', ' 
-00011fb0: 272c 2061 7274 6963 6c65 5f74 6578 7429  ', article_text)
-00011fc0: 0d0a 0d0a 2020 2020 2320 5265 6d6f 7669  ....    # Removi
-00011fd0: 6e67 2073 7065 6369 616c 2063 6861 7261  ng special chara
-00011fe0: 6374 6572 7320 616e 6420 6469 6769 7473  cters and digits
-00011ff0: 0d0a 2020 2020 666f 726d 6174 7465 645f  ..    formatted_
-00012000: 6172 7469 636c 655f 7465 7874 203d 2072  article_text = r
-00012010: 652e 7375 6228 275b 5e61 2d7a 412d 5a5d  e.sub('[^a-zA-Z]
-00012020: 272c 2027 2027 2c20 6172 7469 636c 655f  ', ' ', article_
-00012030: 7465 7874 2029 2020 0d0a 2020 2020 666f  text )  ..    fo
-00012040: 726d 6174 7465 645f 6172 7469 636c 655f  rmatted_article_
-00012050: 7465 7874 203d 2072 652e 7375 6228 7227  text = re.sub(r'
-00012060: 5c73 2b27 2c20 2720 272c 2066 6f72 6d61  \s+', ' ', forma
-00012070: 7474 6564 5f61 7274 6963 6c65 5f74 6578  tted_article_tex
-00012080: 7429 2020 0d0a 0d0a 2020 2020 7365 6e74  t)  ....    sent
-00012090: 656e 6365 5f6c 6973 7420 3d20 6e6c 746b  ence_list = nltk
-000120a0: 2e73 656e 745f 746f 6b65 6e69 7a65 2861  .sent_tokenize(a
-000120b0: 7274 6963 6c65 5f74 6578 7429 2020 0d0a  rticle_text)  ..
-000120c0: 2020 2020 2370 7269 6e74 2873 656e 7465      #print(sente
-000120d0: 6e63 655f 6c69 7374 290d 0a0d 0a20 2020  nce_list)....   
-000120e0: 2073 746f 7077 6f72 6473 203d 206e 6c74   stopwords = nlt
-000120f0: 6b2e 636f 7270 7573 2e73 746f 7077 6f72  k.corpus.stopwor
-00012100: 6473 2e77 6f72 6473 2827 656e 676c 6973  ds.words('englis
-00012110: 6827 290d 0a0d 0a20 2020 2077 6f72 645f  h')....    word_
-00012120: 6672 6571 7565 6e63 6965 7320 3d20 7b7d  frequencies = {}
-00012130: 2020 0d0a 2020 2020 666f 7220 776f 7264    ..    for word
-00012140: 2069 6e20 6e6c 746b 2e77 6f72 645f 746f   in nltk.word_to
-00012150: 6b65 6e69 7a65 2866 6f72 6d61 7474 6564  kenize(formatted
-00012160: 5f61 7274 6963 6c65 5f74 6578 7429 3a20  _article_text): 
-00012170: 200d 0a20 2020 2020 2020 2069 6620 776f   ..        if wo
-00012180: 7264 206e 6f74 2069 6e20 7374 6f70 776f  rd not in stopwo
-00012190: 7264 733a 0d0a 2020 2020 2020 2020 2020  rds:..          
-000121a0: 2020 6966 2077 6f72 6420 6e6f 7420 696e    if word not in
-000121b0: 2077 6f72 645f 6672 6571 7565 6e63 6965   word_frequencie
-000121c0: 732e 6b65 7973 2829 3a0d 0a20 2020 2020  s.keys():..     
-000121d0: 2020 2020 2020 2020 2020 2077 6f72 645f             word_
-000121e0: 6672 6571 7565 6e63 6965 735b 776f 7264  frequencies[word
-000121f0: 5d20 3d20 310d 0a20 2020 2020 2020 2020  ] = 1..         
-00012200: 2020 2065 6c73 653a 0d0a 2020 2020 2020     else:..      
-00012210: 2020 2020 2020 2020 2020 776f 7264 5f66            word_f
-00012220: 7265 7175 656e 6369 6573 5b77 6f72 645d  requencies[word]
-00012230: 202b 3d20 310d 0a0d 0a20 2020 206d 6178   += 1....    max
-00012240: 696d 756d 5f66 7265 7175 6e63 7920 3d20  imum_frequncy = 
-00012250: 6d61 7828 776f 7264 5f66 7265 7175 656e  max(word_frequen
-00012260: 6369 6573 2e76 616c 7565 7328 2929 0d0a  cies.values())..
-00012270: 0d0a 2020 2020 666f 7220 776f 7264 2069  ..    for word i
-00012280: 6e20 776f 7264 5f66 7265 7175 656e 6369  n word_frequenci
-00012290: 6573 2e6b 6579 7328 293a 2020 0d0a 2020  es.keys():  ..  
-000122a0: 2020 2020 2020 776f 7264 5f66 7265 7175        word_frequ
-000122b0: 656e 6369 6573 5b77 6f72 645d 203d 2028  encies[word] = (
-000122c0: 776f 7264 5f66 7265 7175 656e 6369 6573  word_frequencies
-000122d0: 5b77 6f72 645d 2f6d 6178 696d 756d 5f66  [word]/maximum_f
-000122e0: 7265 7175 6e63 7929 0d0a 0d0a 2020 2020  requncy)....    
-000122f0: 2370 7269 6e74 2877 6f72 645f 6672 6571  #print(word_freq
-00012300: 7565 6e63 6965 7329 0d0a 0d0a 2020 2020  uencies)....    
-00012310: 7365 6e74 656e 6365 5f73 636f 7265 7320  sentence_scores 
-00012320: 3d20 7b7d 2020 0d0a 2020 2020 666f 7220  = {}  ..    for 
-00012330: 7365 6e74 2069 6e20 7365 6e74 656e 6365  sent in sentence
-00012340: 5f6c 6973 743a 2020 0d0a 2020 2020 2020  _list:  ..      
-00012350: 2020 666f 7220 776f 7264 2069 6e20 6e6c    for word in nl
-00012360: 746b 2e77 6f72 645f 746f 6b65 6e69 7a65  tk.word_tokenize
-00012370: 2873 656e 742e 6c6f 7765 7228 2929 3a0d  (sent.lower()):.
-00012380: 0a20 2020 2020 2020 2020 2020 2069 6620  .            if 
-00012390: 776f 7264 2069 6e20 776f 7264 5f66 7265  word in word_fre
-000123a0: 7175 656e 6369 6573 2e6b 6579 7328 293a  quencies.keys():
-000123b0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-000123c0: 2020 6966 206c 656e 2873 656e 742e 7370    if len(sent.sp
-000123d0: 6c69 7428 2720 2729 2920 3c20 3235 3a0d  lit(' ')) < 25:.
-000123e0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000123f0: 2020 2020 2069 6620 7365 6e74 206e 6f74       if sent not
-00012400: 2069 6e20 7365 6e74 656e 6365 5f73 636f   in sentence_sco
-00012410: 7265 732e 6b65 7973 2829 3a0d 0a20 2020  res.keys():..   
-00012420: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012430: 2020 2020 2073 656e 7465 6e63 655f 7363       sentence_sc
-00012440: 6f72 6573 5b73 656e 745d 203d 2077 6f72  ores[sent] = wor
-00012450: 645f 6672 6571 7565 6e63 6965 735b 776f  d_frequencies[wo
-00012460: 7264 5d0d 0a20 2020 2020 2020 2020 2020  rd]..           
-00012470: 2020 2020 2020 2020 2065 6c73 653a 0d0a           else:..
-00012480: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012490: 2020 2020 2020 2020 7365 6e74 656e 6365          sentence
-000124a0: 5f73 636f 7265 735b 7365 6e74 5d20 2b3d  _scores[sent] +=
-000124b0: 2077 6f72 645f 6672 6571 7565 6e63 6965   word_frequencie
-000124c0: 735b 776f 7264 5d0d 0a0d 0a20 2020 2023  s[word]....    #
-000124d0: 7072 696e 7428 7365 6e74 656e 6365 5f73  print(sentence_s
-000124e0: 636f 7265 7329 0d0a 0d0a 2020 2020 7375  cores)....    su
-000124f0: 6d6d 6172 795f 7365 6e74 656e 6365 7320  mmary_sentences 
-00012500: 3d20 6865 6170 712e 6e6c 6172 6765 7374  = heapq.nlargest
-00012510: 2869 2c20 7365 6e74 656e 6365 5f73 636f  (i, sentence_sco
-00012520: 7265 732c 206b 6579 3d73 656e 7465 6e63  res, key=sentenc
-00012530: 655f 7363 6f72 6573 2e67 6574 290d 0a20  e_scores.get).. 
-00012540: 2020 2023 7072 696e 7428 7375 6d6d 6172     #print(summar
-00012550: 795f 7365 6e74 656e 6365 7329 0d0a 2020  y_sentences)..  
-00012560: 2020 7375 6d6d 6172 7920 3d20 2720 272e    summary = ' '.
-00012570: 6a6f 696e 2873 756d 6d61 7279 5f73 656e  join(summary_sen
-00012580: 7465 6e63 6573 290d 0a20 2020 2023 7072  tences)..    #pr
-00012590: 696e 7428 2241 4920 5375 6d6d 6172 7922  int("AI Summary"
-000125a0: 290d 0a20 2020 2072 6574 7572 6e20 7375  )..    return su
-000125b0: 6d6d 6172 790d 0a0d 0a64 6566 2073 7461  mmary....def sta
-000125c0: 7274 7375 6d6d 6172 7928 6172 7469 636c  rtsummary(articl
-000125d0: 655f 7465 7874 2c66 7661 6c75 652c 6d61  e_text,fvalue,ma
-000125e0: 786b 6579 776f 7264 7329 3a0d 0a20 2020  xkeywords):..   
-000125f0: 2020 200d 0a20 2320 7472 793a 0d0a 2020     .. # try:..  
-00012600: 206f 7269 6769 6e61 6c77 6f72 6473 203d   originalwords =
-00012610: 206c 656e 2861 7274 6963 6c65 5f74 6578   len(article_tex
-00012620: 742e 7370 6c69 7428 2220 2229 290d 0a0d  t.split(" "))...
-00012630: 0a20 2020 666f 7220 6920 696e 2072 616e  .   for i in ran
-00012640: 6765 2831 2c31 3030 3030 293a 0d0a 2020  ge(1,10000):..  
-00012650: 2020 2073 756d 6d61 7279 3d64 6f73 756d     summary=dosum
-00012660: 6d61 7279 2861 7274 6963 6c65 5f74 6578  mary(article_tex
-00012670: 742c 6929 0d0a 2020 2020 2072 6573 203d  t,i)..     res =
-00012680: 206c 656e 2873 756d 6d61 7279 2e73 706c   len(summary.spl
-00012690: 6974 2829 290d 0a20 2020 2020 6966 2072  it())..     if r
-000126a0: 6573 203e 3d20 6676 616c 7565 3a0d 0a20  es >= fvalue:.. 
-000126b0: 2020 2020 2020 2020 6272 6561 6b0d 0a0d          break...
-000126c0: 0a20 2020 7375 6d6d 6172 7920 3d20 2072  .   summary =  r
-000126d0: 652e 7375 6228 225c 5c5c 5c78 5b61 2d66  e.sub("\\\\x[a-f
-000126e0: 302d 395d 5b61 2d66 302d 395d 222c 2022  0-9][a-f0-9]", "
-000126f0: 2022 2c73 756d 6d61 7279 290d 0a20 2020   ",summary)..   
-00012700: 7375 6d6d 6172 7920 3d20 7265 2e73 7562  summary = re.sub
-00012710: 2822 5c5c 7865 325c 5c78 3830 5c5c 7839  ("\\xe2\\x80\\x9
-00012720: 3922 2c22 2722 2c20 7375 6d6d 6172 7929  9","'", summary)
-00012730: 0d0a 2020 2073 756d 6d61 7279 3d73 756d  ..   summary=sum
-00012740: 6d61 7279 2e72 6570 6c61 6365 2822 5c5c  mary.replace("\\
-00012750: 7865 325c 5c78 3830 5c5c 7839 3922 2c22  xe2\\x80\\x99","
-00012760: 2722 290d 0a20 2020 7375 6d6d 6172 793d  '")..   summary=
-00012770: 7375 6d6d 6172 792e 7265 706c 6163 6528  summary.replace(
-00012780: 225c 5c78 6532 5c5c 7838 305c 5c78 3930  "\\xe2\\x80\\x90
-00012790: 222c 222d 2229 0d0a 2020 2073 756d 6d61  ","-")..   summa
-000127a0: 7279 3d73 756d 6d61 7279 2e72 6570 6c61  ry=summary.repla
-000127b0: 6365 2822 5c5c 7865 325c 5c78 3830 5c5c  ce("\\xe2\\x80\\
-000127c0: 7839 3122 2c22 2d22 290d 0a20 2020 7375  x91","-")..   su
-000127d0: 6d6d 6172 793d 7375 6d6d 6172 792e 7265  mmary=summary.re
-000127e0: 706c 6163 6528 225c 5c78 6532 5c5c 7838  place("\\xe2\\x8
-000127f0: 305c 5c78 3932 222c 222d 2229 0d0a 2020  0\\x92","-")..  
-00012800: 2073 756d 6d61 7279 3d73 756d 6d61 7279   summary=summary
-00012810: 2e72 6570 6c61 6365 2822 5c5c 7865 325c  .replace("\\xe2\
-00012820: 5c78 3830 5c5c 7839 3322 2c22 2d22 290d  \x80\\x93","-").
-00012830: 0a20 2020 7375 6d6d 6172 793d 7375 6d6d  .   summary=summ
-00012840: 6172 792e 7265 706c 6163 6528 225c 5c78  ary.replace("\\x
-00012850: 6532 5c5c 7838 305c 5c78 3934 222c 222d  e2\\x80\\x94","-
-00012860: 2229 0d0a 2020 2073 756d 6d61 7279 3d73  ")..   summary=s
-00012870: 756d 6d61 7279 2e72 6570 6c61 6365 2822  ummary.replace("
-00012880: 5c5c 7865 325c 5c78 3830 5c5c 7839 3522  \\xe2\\x80\\x95"
-00012890: 2c22 2d22 290d 0a20 2020 7375 6d6d 6172  ,"-")..   summar
-000128a0: 793d 7375 6d6d 6172 792e 7265 706c 6163  y=summary.replac
-000128b0: 6528 225c 5c78 6532 5c5c 7838 305c 5c78  e("\\xe2\\x80\\x
-000128c0: 6233 222c 2722 2729 0d0a 2020 2073 756d  b3",'"')..   sum
-000128d0: 6d61 7279 203d 2073 756d 6d61 7279 2e72  mary = summary.r
-000128e0: 6570 6c61 6365 2827 e280 9c27 2c20 2722  eplace('...', '"
-000128f0: 2729 0d0a 2020 2073 756d 6d61 7279 203d  ')..   summary =
-00012900: 2073 756d 6d61 7279 2e72 6570 6c61 6365   summary.replace
-00012910: 2827 e280 9d27 2c20 2722 2729 0d0a 2020  ('...', '"')..  
-00012920: 2073 756d 6d61 7279 203d 2073 756d 6d61   summary = summa
-00012930: 7279 2e72 6570 6c61 6365 2827 e280 9927  ry.replace('...'
-00012940: 2c20 2227 2229 0d0a 2020 2073 756d 6d61  , "'")..   summa
-00012950: 7279 203d 2073 756d 6d61 7279 2e72 6570  ry = summary.rep
-00012960: 6c61 6365 2827 e280 9827 2c20 2227 2229  lace('...', "'")
-00012970: 0d0a 2020 2073 756d 6d61 7279 203d 2073  ..   summary = s
-00012980: 756d 6d61 7279 2e72 6570 6c61 6365 2827  ummary.replace('
-00012990: e280 9327 2c20 222d 2229 0d0a 2020 2073  ...', "-")..   s
-000129a0: 756d 6d61 7279 203d 2073 756d 6d61 7279  ummary = summary
-000129b0: 2e72 6570 6c61 6365 2827 e280 a627 2c20  .replace('...', 
-000129c0: 222e 2e2e 2229 0d0a 2020 2073 756d 6d61  "...")..   summa
-000129d0: 7279 203d 2073 756d 6d61 7279 2e72 6570  ry = summary.rep
-000129e0: 6c61 6365 2827 e280 9427 2c20 222d 2229  lace('...', "-")
-000129f0: 0d0a 2020 2073 756d 6d61 7279 203d 2073  ..   summary = s
-00012a00: 756d 6d61 7279 2e72 6570 6c61 6365 2827  ummary.replace('
-00012a10: 2227 2c20 2222 290d 0a20 2020 6b65 7977  "', "")..   keyw
-00012a20: 6f72 6473 3d67 6574 6b65 7977 6f72 6473  ords=getkeywords
-00012a30: 2873 756d 6d61 7279 2c6d 6178 6b65 7977  (summary,maxkeyw
-00012a40: 6f72 6473 290d 0a0d 0a20 2020 7375 6d6d  ords)....   summ
-00012a50: 6172 7977 6f72 6473 203d 206c 656e 2873  arywords = len(s
-00012a60: 756d 6d61 7279 2e73 706c 6974 2822 2022  ummary.split(" "
-00012a70: 2929 0d0a 200d 0a20 2020 6d61 696e 6f75  )).. ..   mainou
-00012a80: 743d 6b65 7977 6f72 6473 202b 2022 2c5c  t=keywords + ",\
-00012a90: 226f 7269 6769 6e61 6c77 6f72 6463 6f75  "originalwordcou
-00012aa0: 6e74 5c22 3a22 202b 2073 7472 286f 7269  nt\":" + str(ori
-00012ab0: 6769 6e61 6c77 6f72 6473 2920 2b20 222c  ginalwords) + ",
-00012ac0: 5c22 7375 6d6d 6172 7977 6f72 6463 6f75  \"summarywordcou
-00012ad0: 6e74 5c22 3a22 2b20 7374 7228 7375 6d6d  nt\":"+ str(summ
-00012ae0: 6172 7977 6f72 6473 2920 2b22 2c5c 226d  arywords) +",\"m
-00012af0: 6169 6e73 756d 6d61 7279 5c22 3a7b 5c22  ainsummary\":{\"
-00012b00: 7375 6d6d 6172 795c 223a 205c 2222 202b  summary\": \"" +
-00012b10: 2073 756d 6d61 7279 202b 2022 5c22 7d7d   summary + "\"}}
-00012b20: 220d 0a20 2020 7265 7475 726e 206d 6169  "..   return mai
-00012b30: 6e6f 7574 0d0a 2020 200d 0a              nout..   ..
+0000fce0: 6c75 652c 6b65 7973 290d 0a0d 0a64 6566  lue,keys)....def
+0000fcf0: 2076 6970 6572 6368 6174 6770 7428 6f70   viperchatgpt(op
+0000fd00: 656e 6169 6b65 792c 7465 7874 746f 616e  enaikey,texttoan
+0000fd10: 616c 7973 652c 7175 6572 792c 2074 656d  alyse,query, tem
+0000fd20: 7065 7261 7475 7265 2c6d 6f64 656c 6e61  perature,modelna
+0000fd30: 6d65 293a 0d0a 2020 2020 6966 206f 7065  me):..    if ope
+0000fd40: 6e61 696b 6579 3d3d 2222 3a0d 0a20 2020  naikey=="":..   
+0000fd50: 2020 2020 2020 7265 7475 726e 2022 506c        return "Pl
+0000fd60: 6561 7365 2065 6e74 6572 204f 7065 6e41  ease enter OpenA
+0000fd70: 4920 6b65 7922 0d0a 2020 2020 6966 2074  I key"..    if t
+0000fd80: 6578 7474 6f61 6e61 6c79 7365 203d 3d20  exttoanalyse == 
+0000fd90: 2222 3a0d 0a20 2020 2020 2020 2072 6574  "":..        ret
+0000fda0: 7572 6e20 2245 6e74 6572 2074 6578 7420  urn "Enter text 
+0000fdb0: 746f 2061 6e61 6c79 7365 220d 0a20 2020  to analyse"..   
+0000fdc0: 2069 6620 7175 6572 7920 3d3d 2022 223a   if query == "":
+0000fdd0: 0d0a 2020 2020 2020 2020 7265 7475 726e  ..        return
+0000fde0: 2022 456e 7465 7220 4368 6174 6770 7420   "Enter Chatgpt 
+0000fdf0: 7072 6f6d 7074 7322 0d0a 2020 2020 6966  prompts"..    if
+0000fe00: 2074 656d 7065 7261 7475 7265 203e 2031   temperature > 1
+0000fe10: 206f 7220 7465 6d70 6572 6174 7572 6520   or temperature 
+0000fe20: 3c20 303a 0d0a 2020 2020 2020 2020 7265  < 0:..        re
+0000fe30: 7475 726e 2022 496e 7661 6c75 6520 7465  turn "Invalue te
+0000fe40: 6d70 6572 6174 7572 6520 2d20 7368 6f75  mperature - shou
+0000fe50: 6c64 2062 6520 6265 7477 6565 6e20 302d  ld be between 0-
+0000fe60: 3120 692e 652e 2030 2e37 220d 0a20 2020  1 i.e. 0.7"..   
+0000fe70: 2069 6620 6d6f 6465 6c6e 616d 6520 3d3d   if modelname ==
+0000fe80: 2022 223a 0d0a 2020 2020 2020 2020 7265   "":..        re
+0000fe90: 7475 726e 2022 5370 6563 6966 7920 6d6f  turn "Specify mo
+0000fea0: 6465 6c20 6e61 6d65 206c 696b 6520 2774  del name like 't
+0000feb0: 6578 742d 6461 7669 6e63 692d 3030 3227  ext-davinci-002'
+0000fec0: 206f 7220 2774 6578 742d 6375 7269 652d   or 'text-curie-
+0000fed0: 3030 3127 220d 0a0d 0a20 2020 206f 732e  001'"....    os.
+0000fee0: 656e 7669 726f 6e5b 224f 5045 4e41 495f  environ["OPENAI_
+0000fef0: 4150 495f 4b45 5922 5d20 3d20 6f70 656e  API_KEY"] = open
+0000ff00: 6169 6b65 790d 0a20 2020 2020 2020 200d  aikey..        .
+0000ff10: 0a20 2020 2072 6573 203d 2073 7461 7274  .    res = start
+0000ff20: 5f63 6f6e 7665 7273 6174 696f 6e28 6f70  _conversation(op
+0000ff30: 656e 6169 6b65 792c 7175 6572 792c 7465  enaikey,query,te
+0000ff40: 7874 746f 616e 616c 7973 652c 7465 6d70  xttoanalyse,temp
+0000ff50: 6572 6174 7572 652c 6d6f 6465 6c6e 616d  erature,modelnam
+0000ff60: 6529 0d0a 2020 2020 6368 6174 6770 7472  e)..    chatgptr
+0000ff70: 6573 706f 6e73 6520 3d20 7265 735b 276f  esponse = res['o
+0000ff80: 7574 7075 745f 7465 7874 275d 0d0a 2020  utput_text']..  
+0000ff90: 2020 6368 6174 6770 7472 6573 706f 6e73    chatgptrespons
+0000ffa0: 652e 7265 706c 6163 6528 225c 5c6e 222c  e.replace("\\n",
+0000ffb0: 2222 292e 7265 706c 6163 6528 225c 5c72  "").replace("\\r
+0000ffc0: 222c 2022 2229 0d0a 2020 2020 6368 6174  ", "")..    chat
+0000ffd0: 6770 7472 6573 706f 6e73 6520 3d20 6368  gptresponse = ch
+0000ffe0: 6174 6770 7472 6573 706f 6e73 652e 7265  atgptresponse.re
+0000fff0: 706c 6163 6528 275c 5c75 272c 2755 2b27  place('\\u','U+'
+00010000: 290d 0a0d 0a20 2020 2063 6861 7467 7074  )....    chatgpt
+00010010: 7265 7370 6f6e 7365 203d 2072 652e 7375  response = re.su
+00010020: 6228 7227 3c55 5c2b 285b 302d 3961 2d66  b(r'<U\+([0-9a-f
+00010030: 412d 465d 7b34 2c36 7d29 3e27 2c20 6c61  A-F]{4,6})>', la
+00010040: 6d62 6461 2078 3a20 6368 7228 696e 7428  mbda x: chr(int(
+00010050: 782e 6772 6f75 7028 3129 2c31 3629 292c  x.group(1),16)),
+00010060: 2063 6861 7467 7074 7265 7370 6f6e 7365   chatgptresponse
+00010070: 290d 0a0d 0a0d 0a20 2020 2072 6574 7572  )......    retur
+00010080: 6e20 6368 6174 6770 7472 6573 706f 6e73  n chatgptrespons
+00010090: 650d 0a20 2020 200d 0a64 6566 2061 7265  e..    ..def are
+000100a0: 796f 7562 7573 7928 686f 7374 2c70 6f72  youbusy(host,por
+000100b0: 743d 2d39 3939 2c6d 6963 726f 7365 7276  t=-999,microserv
+000100c0: 6963 6569 643d 2727 293a 0d0a 2020 2020  iceid=''):..    
+000100d0: 676c 6f62 616c 2063 6f6e 6e65 6374 696f  global connectio
+000100e0: 6e65 7272 6f72 0d0a 0d0a 2020 2020 6966  nerror....    if
+000100f0: 2028 6c65 6e28 686f 7374 293d 3d30 206f   (len(host)==0 o
+00010100: 7220 706f 7274 3d3d 2d39 3939 2029 3a0d  r port==-999 ):.
+00010110: 0a20 2020 2020 2020 2020 7265 7475 726e  .         return
+00010120: 2022 506c 6561 7365 2065 6e74 6572 2068   "Please enter h
+00010130: 6f73 742c 706f 7274 220d 0a20 2020 2076  ost,port"..    v
+00010140: 616c 7565 3d28 2261 7265 796f 7562 7573  alue=("areyoubus
+00010150: 7922 290d 0a0d 0a20 2020 2076 616c 3d6c  y")....    val=l
+00010160: 6f6f 702e 7275 6e5f 756e 7469 6c5f 636f  oop.run_until_co
+00010170: 6d70 6c65 7465 2874 6370 5f65 6368 6f5f  mplete(tcp_echo_
+00010180: 636c 6965 6e74 7669 7065 7228 7661 6c75  clientviper(valu
+00010190: 652c 206c 6f6f 702c 686f 7374 2c70 6f72  e, loop,host,por
+000101a0: 742c 6d69 6372 6f73 6572 7669 6365 6964  t,microserviceid
+000101b0: 2929 0d0a 2020 2020 6966 2063 6f6e 6e65  ))..    if conne
+000101c0: 6374 696f 6e65 7272 6f72 3a0d 0a20 2020  ctionerror:..   
+000101d0: 2020 2020 2020 7265 7475 726e 2063 6f6e        return con
+000101e0: 6e65 6374 696f 6e65 7272 6f72 0d0a 0d0a  nectionerror....
+000101f0: 2020 2020 7265 7475 726e 2076 616c 0d0a      return val..
+00010200: 0d0a 2323 2323 2323 2323 2323 2323 2323  ..##############
+00010210: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+00010220: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+00010230: 2323 2323 2323 0d0a 696d 706f 7274 2073  ######..import s
+00010240: 7973 0d0a 6672 6f6d 2070 6466 6d69 6e65  ys..from pdfmine
+00010250: 722e 7064 6670 6172 7365 7220 696d 706f  r.pdfparser impo
+00010260: 7274 2050 4446 5061 7273 6572 0d0a 6672  rt PDFParser..fr
+00010270: 6f6d 2070 6466 6d69 6e65 722e 7064 6664  om pdfminer.pdfd
+00010280: 6f63 756d 656e 7420 696d 706f 7274 2050  ocument import P
+00010290: 4446 446f 6375 6d65 6e74 0d0a 6672 6f6d  DFDocument..from
+000102a0: 2070 6466 6d69 6e65 722e 7064 6670 6167   pdfminer.pdfpag
+000102b0: 6520 696d 706f 7274 2050 4446 5061 6765  e import PDFPage
+000102c0: 0d0a 6672 6f6d 2070 6466 6d69 6e65 722e  ..from pdfminer.
+000102d0: 7064 6670 6167 6520 696d 706f 7274 2050  pdfpage import P
+000102e0: 4446 5465 7874 4578 7472 6163 7469 6f6e  DFTextExtraction
+000102f0: 4e6f 7441 6c6c 6f77 6564 0d0a 6672 6f6d  NotAllowed..from
+00010300: 2070 6466 6d69 6e65 722e 7064 6669 6e74   pdfminer.pdfint
+00010310: 6572 7020 696d 706f 7274 2050 4446 5265  erp import PDFRe
+00010320: 736f 7572 6365 4d61 6e61 6765 720d 0a66  sourceManager..f
+00010330: 726f 6d20 7064 666d 696e 6572 2e70 6466  rom pdfminer.pdf
+00010340: 696e 7465 7270 2069 6d70 6f72 7420 5044  interp import PD
+00010350: 4650 6167 6549 6e74 6572 7072 6574 6572  FPageInterpreter
+00010360: 0d0a 2366 726f 6d20 5374 7269 6e67 494f  ..#from StringIO
+00010370: 2069 6d70 6f72 7420 5374 7269 6e67 494f   import StringIO
+00010380: 0d0a 6672 6f6d 2069 6f20 696d 706f 7274  ..from io import
+00010390: 2053 7472 696e 6749 4f0d 0a69 6d70 6f72   StringIO..impor
+000103a0: 7420 7572 6c6c 6962 2e72 6571 7565 7374  t urllib.request
+000103b0: 2020 0d0a 2369 6d70 6f72 7420 746d 6c74    ..#import tmlt
+000103c0: 6578 7473 756d 6d61 7279 0d0a 696d 706f  extsummary..impo
+000103d0: 7274 206f 730d 0a69 6d70 6f72 7420 6461  rt os..import da
+000103e0: 7465 7469 6d65 0d0a 2369 6d70 6f72 7420  tetime..#import 
+000103f0: 676c 6f62 0d0a 0d0a 0d0a 6672 6f6d 2070  glob......from p
+00010400: 6466 6d69 6e65 722e 6c61 796f 7574 2069  dfminer.layout i
+00010410: 6d70 6f72 7420 4c41 5061 7261 6d73 0d0a  mport LAParams..
+00010420: 6672 6f6d 2070 6466 6d69 6e65 722e 636f  from pdfminer.co
+00010430: 6e76 6572 7465 7220 696d 706f 7274 2054  nverter import T
+00010440: 6578 7443 6f6e 7665 7274 6572 0d0a 200d  extConverter.. .
+00010450: 0a63 6c61 7373 204d 7950 6172 7365 7228  .class MyParser(
+00010460: 6f62 6a65 6374 293a 0d0a 2020 2020 6465  object):..    de
+00010470: 6620 5f5f 696e 6974 5f5f 2873 656c 662c  f __init__(self,
+00010480: 2070 6466 293a 0d0a 2020 2020 2020 2020   pdf):..        
+00010490: 2323 2053 6e69 7070 6564 2061 6461 7074  ## Snipped adapt
+000104a0: 6564 2066 726f 6d20 5975 7375 6b65 2053  ed from Yusuke S
+000104b0: 6869 6e79 616d 6173 200d 0a20 2020 2020  hinyamas ..     
+000104c0: 2020 2023 5044 464d 696e 6572 2064 6f63     #PDFMiner doc
+000104d0: 756d 656e 7461 7469 6f6e 0d0a 2020 2020  umentation..    
+000104e0: 2020 2020 2320 4372 6561 7465 2074 6865      # Create the
+000104f0: 2064 6f63 756d 656e 7420 6d6f 6465 6c20   document model 
+00010500: 6672 6f6d 2074 6865 2066 696c 650d 0a20  from the file.. 
+00010510: 2020 2020 2020 2070 6172 7365 7220 3d20         parser = 
+00010520: 5044 4650 6172 7365 7228 6f70 656e 2870  PDFParser(open(p
+00010530: 6466 2c20 2772 6227 2929 0d0a 2020 2020  df, 'rb'))..    
+00010540: 2020 2020 646f 6375 6d65 6e74 203d 2050      document = P
+00010550: 4446 446f 6375 6d65 6e74 2870 6172 7365  DFDocument(parse
+00010560: 7229 0d0a 2020 2020 2020 2020 2320 5472  r)..        # Tr
+00010570: 7920 746f 2070 6172 7365 2074 6865 2064  y to parse the d
+00010580: 6f63 756d 656e 740d 0a20 2020 2020 2020  ocument..       
+00010590: 2069 6620 6e6f 7420 646f 6375 6d65 6e74   if not document
+000105a0: 2e69 735f 6578 7472 6163 7461 626c 653a  .is_extractable:
+000105b0: 0d0a 2020 2020 2020 2020 2020 2020 7261  ..            ra
+000105c0: 6973 6520 5044 4654 6578 7445 7874 7261  ise PDFTextExtra
+000105d0: 6374 696f 6e4e 6f74 416c 6c6f 7765 640d  ctionNotAllowed.
+000105e0: 0a20 2020 2020 2020 2023 2043 7265 6174  .        # Creat
+000105f0: 6520 6120 5044 4620 7265 736f 7572 6365  e a PDF resource
+00010600: 206d 616e 6167 6572 206f 626a 6563 7420   manager object 
+00010610: 0d0a 2020 2020 2020 2020 2320 7468 6174  ..        # that
+00010620: 2073 746f 7265 7320 7368 6172 6564 2072   stores shared r
+00010630: 6573 6f75 7263 6573 2e0d 0a20 2020 2020  esources...     
+00010640: 2020 2072 7372 636d 6772 203d 2050 4446     rsrcmgr = PDF
+00010650: 5265 736f 7572 6365 4d61 6e61 6765 7228  ResourceManager(
+00010660: 290d 0a20 2020 2020 2020 2023 2043 7265  )..        # Cre
+00010670: 6174 6520 6120 6275 6666 6572 2066 6f72  ate a buffer for
+00010680: 2074 6865 2070 6172 7365 6420 7465 7874   the parsed text
+00010690: 0d0a 2020 2020 2020 2020 7265 7473 7472  ..        retstr
+000106a0: 203d 2053 7472 696e 6749 4f28 290d 0a20   = StringIO().. 
+000106b0: 2020 2020 2020 2023 2053 7061 6369 6e67         # Spacing
+000106c0: 2070 6172 616d 6574 6572 7320 666f 7220   parameters for 
+000106d0: 7061 7273 696e 670d 0a20 2020 2020 2020  parsing..       
+000106e0: 206c 6170 6172 616d 7320 3d20 4c41 5061   laparams = LAPa
+000106f0: 7261 6d73 2829 0d0a 2020 2020 2020 2020  rams()..        
+00010700: 636f 6465 6320 3d20 2775 7466 2d38 270d  codec = 'utf-8'.
+00010710: 0a20 0d0a 2020 2020 2020 2020 2320 4372  . ..        # Cr
+00010720: 6561 7465 2061 2050 4446 2064 6576 6963  eate a PDF devic
+00010730: 6520 6f62 6a65 6374 0d0a 2020 2020 2020  e object..      
+00010740: 2020 6465 7669 6365 203d 2054 6578 7443    device = TextC
+00010750: 6f6e 7665 7274 6572 2872 7372 636d 6772  onverter(rsrcmgr
+00010760: 2c20 7265 7473 7472 2c0d 0a20 2020 2020  , retstr,..     
+00010770: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010780: 2020 2020 2020 2020 2020 6c61 7061 7261            lapara
+00010790: 6d73 203d 206c 6170 6172 616d 7329 0d0a  ms = laparams)..
+000107a0: 2020 2020 2020 2020 2320 4372 6561 7465          # Create
+000107b0: 2061 2050 4446 2069 6e74 6572 7072 6574   a PDF interpret
+000107c0: 6572 206f 626a 6563 740d 0a20 2020 2020  er object..     
+000107d0: 2020 2069 6e74 6572 7072 6574 6572 203d     interpreter =
+000107e0: 2050 4446 5061 6765 496e 7465 7270 7265   PDFPageInterpre
+000107f0: 7465 7228 7273 7263 6d67 722c 2064 6576  ter(rsrcmgr, dev
+00010800: 6963 6529 0d0a 2020 2020 2020 2020 2320  ice)..        # 
+00010810: 5072 6f63 6573 7320 6561 6368 2070 6167  Process each pag
+00010820: 6520 636f 6e74 6169 6e65 6420 696e 2074  e contained in t
+00010830: 6865 2064 6f63 756d 656e 742e 0d0a 2020  he document...  
+00010840: 2020 2020 2020 666f 7220 7061 6765 2069        for page i
+00010850: 6e20 5044 4650 6167 652e 6372 6561 7465  n PDFPage.create
+00010860: 5f70 6167 6573 2864 6f63 756d 656e 7429  _pages(document)
+00010870: 3a0d 0a20 2020 2020 2020 2020 2020 2069  :..            i
+00010880: 6e74 6572 7072 6574 6572 2e70 726f 6365  nterpreter.proce
+00010890: 7373 5f70 6167 6528 7061 6765 290d 0a20  ss_page(page).. 
+000108a0: 2020 2020 2020 2020 0d0a 2020 2020 2020          ..      
+000108b0: 2020 7365 6c66 2e72 6563 6f72 6473 2020    self.records  
+000108c0: 2020 2020 2020 2020 2020 3d20 5b5d 0d0a            = []..
+000108d0: 2020 2020 2020 2020 200d 0a20 2020 2020           ..     
+000108e0: 2020 206c 696e 6573 203d 2072 6574 7374     lines = retst
+000108f0: 722e 6765 7476 616c 7565 2829 2e73 706c  r.getvalue().spl
+00010900: 6974 6c69 6e65 7328 290d 0a20 2020 2020  itlines()..     
+00010910: 2020 2066 6f72 206c 696e 6520 696e 206c     for line in l
+00010920: 696e 6573 3a0d 0a20 2020 2020 2020 2020  ines:..         
+00010930: 2020 2073 656c 662e 6861 6e64 6c65 5f6c     self.handle_l
+00010940: 696e 6528 6c69 6e65 290d 0a20 2020 2020  ine(line)..     
+00010950: 0d0a 2020 2020 6465 6620 6861 6e64 6c65  ..    def handle
+00010960: 5f6c 696e 6528 7365 6c66 2c20 6c69 6e65  _line(self, line
+00010970: 293a 0d0a 2020 2020 2020 2020 2320 4375  ):..        # Cu
+00010980: 7374 6f6d 697a 6520 796f 7572 206c 696e  stomize your lin
+00010990: 652d 6279 2d6c 696e 6520 7061 7273 6572  e-by-line parser
+000109a0: 2068 6572 650d 0a20 2020 2020 2020 2073   here..        s
+000109b0: 656c 662e 7265 636f 7264 732e 6170 7065  elf.records.appe
+000109c0: 6e64 286c 696e 6529 0d0a 0d0a 6465 6620  nd(line)....def 
+000109d0: 7363 7261 7065 7064 6628 7468 6575 726c  scrapepdf(theurl
+000109e0: 2c66 6e29 3a0d 0a20 2020 2073 6372 6170  ,fn):..    scrap
+000109f0: 6564 5f64 6174 6120 3d20 7572 6c6c 6962  ed_data = urllib
+00010a00: 2e72 6571 7565 7374 2e75 726c 6f70 656e  .request.urlopen
+00010a10: 2874 6865 7572 6c29 2020 0d0a 2020 2020  (theurl)  ..    
+00010a20: 6669 6c65 203d 206f 7065 6e28 666e 2c20  file = open(fn, 
+00010a30: 2777 6227 290d 0a20 2020 2066 696c 652e  'wb')..    file.
+00010a40: 7772 6974 6528 7363 7261 7065 645f 6461  write(scraped_da
+00010a50: 7461 2e72 6561 6428 2929 0d0a 2020 2020  ta.read())..    
+00010a60: 6669 6c65 2e63 6c6f 7365 2829 0d0a 2020  file.close()..  
+00010a70: 2020 2372 6574 7572 6e20 6172 7469 636c    #return articl
+00010a80: 655f 7465 7874 0d0a 0d0a 6465 6620 7374  e_text....def st
+00010a90: 6172 7470 6466 7265 6164 696e 6728 6669  artpdfreading(fi
+00010aa0: 6c65 6e61 6d65 2c66 7661 6c75 652c 6b65  lename,fvalue,ke
+00010ab0: 7963 6f75 6e74 293a 0d0a 2020 236f 732e  ycount):..  #os.
+00010ac0: 7061 7468 2e61 6273 7061 7468 286f 732e  path.abspath(os.
+00010ad0: 6765 7463 7764 2829 290d 0a20 2074 6865  getcwd())..  the
+00010ae0: 7369 7a65 3d72 6f75 6e64 286f 732e 7061  size=round(os.pa
+00010af0: 7468 2e67 6574 7369 7a65 2866 696c 656e  th.getsize(filen
+00010b00: 616d 6529 2f31 3030 3030 3030 2c32 290d  ame)/1000000,2).
+00010b10: 0a20 206d 5f74 696d 6520 3d20 6f73 2e70  .  m_time = os.p
+00010b20: 6174 682e 6765 746d 7469 6d65 2866 696c  ath.getmtime(fil
+00010b30: 656e 616d 6529 0d0a 2020 6474 5f6d 203d  ename)..  dt_m =
+00010b40: 2064 6174 6574 696d 652e 6461 7465 7469   datetime.dateti
+00010b50: 6d65 2e66 726f 6d74 696d 6573 7461 6d70  me.fromtimestamp
+00010b60: 286d 5f74 696d 6529 0d0a 2020 635f 7469  (m_time)..  c_ti
+00010b70: 6d65 203d 206f 732e 7061 7468 2e67 6574  me = os.path.get
+00010b80: 6374 696d 6528 6669 6c65 6e61 6d65 290d  ctime(filename).
+00010b90: 0a20 2023 2063 6f6e 7665 7274 2063 7265  .  # convert cre
+00010ba0: 6174 696f 6e20 7469 6d65 7374 616d 7020  ation timestamp 
+00010bb0: 696e 746f 2044 6174 6554 696d 6520 6f62  into DateTime ob
+00010bc0: 6a65 6374 0d0a 2020 6474 5f63 203d 2064  ject..  dt_c = d
+00010bd0: 6174 6574 696d 652e 6461 7465 7469 6d65  atetime.datetime
+00010be0: 2e66 726f 6d74 696d 6573 7461 6d70 2863  .fromtimestamp(c
+00010bf0: 5f74 696d 6529 0d0a 2020 636f 203d 2073  _time)..  co = s
+00010c00: 7472 2864 745f 6329 205b 303a 3139 5d0d  tr(dt_c) [0:19].
+00010c10: 0a20 206d 6f20 3d20 7374 7228 6474 5f6d  .  mo = str(dt_m
+00010c20: 2920 5b30 3a31 395d 0d0a 0d0a 2020 7020  ) [0:19]....  p 
+00010c30: 3d20 4d79 5061 7273 6572 2866 696c 656e  = MyParser(filen
+00010c40: 616d 6529 0d0a 2020 7468 6574 6578 743d  ame)..  thetext=
+00010c50: 275c 6e27 2e6a 6f69 6e28 702e 7265 636f  '\n'.join(p.reco
+00010c60: 7264 7329 0d0a 2020 6172 7469 636c 655f  rds)..  article_
+00010c70: 7465 7874 3d74 6865 7465 7874 2e65 6e63  text=thetext.enc
+00010c80: 6f64 6528 2775 7466 3827 290d 0a20 2073  ode('utf8')..  s
+00010c90: 756d 6d61 7269 7a65 643d 227b 5c22 6669  ummarized="{\"fi
+00010ca0: 6c65 6e61 6d65 5c22 3a5c 2222 202b 2066  lename\":\"" + f
+00010cb0: 696c 656e 616d 6520 2b20 225c 222c 5c22  ilename + "\",\"
+00010cc0: 6669 6c65 7369 7a65 284d 4229 5c22 3a22  filesize(MB)\":"
+00010cd0: 2b73 7472 2874 6865 7369 7a65 292b 222c  +str(thesize)+",
+00010ce0: 5c22 6669 6c65 6372 6561 7465 646f 6e5c  \"filecreatedon\
+00010cf0: 223a 5c22 2220 2b20 636f 202b 2022 5c22  ":\"" + co + "\"
+00010d00: 2c5c 2266 696c 656d 6f64 6966 6965 646f  ,\"filemodifiedo
+00010d10: 6e5c 223a 5c22 2220 2b20 6d6f 202b 2022  n\":\"" + mo + "
+00010d20: 5c22 2c5c 226b 6579 776f 7264 735c 223a  \",\"keywords\":
+00010d30: 2220 2b20 2073 7461 7274 7375 6d6d 6172  " +  startsummar
+00010d40: 7928 7468 6574 6578 742c 6676 616c 7565  y(thetext,fvalue
+00010d50: 2c6b 6579 636f 756e 7429 0d0a 2023 2070  ,keycount).. # p
+00010d60: 7269 6e74 2873 756d 6d61 7269 7a65 6429  rint(summarized)
+00010d70: 0d0a 2020 7265 7475 726e 2073 756d 6d61  ..  return summa
+00010d80: 7269 7a65 640d 0a0d 0a0d 0a23 2323 2323  rized......#####
+00010d90: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+00010da0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+00010db0: 2323 2323 2323 2323 2323 0d0a 2320 4465  ##########..# De
+00010dc0: 7665 6c6f 7065 6420 6279 204f 5449 4353  veloped by OTICS
+00010dd0: 2041 6476 616e 6365 6420 416e 616c 7974   Advanced Analyt
+00010de0: 6963 730d 0a23 2053 6562 6173 7469 616e  ics..# Sebastian
+00010df0: 204d 6175 7269 6365 0d0a 0d0a 696d 706f   Maurice....impo
+00010e00: 7274 2062 7334 2061 7320 6273 2020 0d0a  rt bs4 as bs  ..
+00010e10: 696d 706f 7274 2075 726c 6c69 622e 7265  import urllib.re
+00010e20: 7175 6573 7420 200d 0a69 6d70 6f72 7420  quest  ..import 
+00010e30: 7265 0d0a 696d 706f 7274 206e 6c74 6b0d  re..import nltk.
+00010e40: 0a66 726f 6d20 6e6c 746b 2e74 6f6b 656e  .from nltk.token
+00010e50: 697a 6520 696d 706f 7274 2052 6567 6578  ize import Regex
+00010e60: 7054 6f6b 656e 697a 6572 0d0a 696d 706f  pTokenizer..impo
+00010e70: 7274 2068 6561 7071 0d0a 696d 706f 7274  rt heapq..import
+00010e80: 2073 7973 0d0a 696d 706f 7274 206f 730d   sys..import os.
+00010e90: 0a66 726f 6d20 7261 6b65 5f6e 6c74 6b20  .from rake_nltk 
+00010ea0: 696d 706f 7274 204d 6574 7269 632c 5261  import Metric,Ra
+00010eb0: 6b65 0d0a 696d 706f 7274 206a 736f 6e0d  ke..import json.
+00010ec0: 0a69 6d70 6f72 7420 7061 6e64 6173 2061  .import pandas a
+00010ed0: 7320 7064 0d0a 696d 706f 7274 206e 6c74  s pd..import nlt
+00010ee0: 6b2e 636f 7270 7573 0d0a 6672 6f6d 206e  k.corpus..from n
+00010ef0: 6c74 6b2e 636f 7270 7573 2069 6d70 6f72  ltk.corpus impor
+00010f00: 7420 7374 6f70 776f 7264 730d 0a66 726f  t stopwords..fro
+00010f10: 6d20 7465 7874 626c 6f62 2069 6d70 6f72  m textblob impor
+00010f20: 7420 5465 7874 426c 6f62 0d0a 6672 6f6d  t TextBlob..from
+00010f30: 2074 6578 7462 6c6f 6220 696d 706f 7274   textblob import
+00010f40: 2057 6f72 640d 0a66 726f 6d20 736b 6c65   Word..from skle
+00010f50: 6172 6e2e 6665 6174 7572 655f 6578 7472  arn.feature_extr
+00010f60: 6163 7469 6f6e 2e74 6578 7420 696d 706f  action.text impo
+00010f70: 7274 2054 6669 6466 5472 616e 7366 6f72  rt TfidfTransfor
+00010f80: 6d65 722c 5466 6964 6656 6563 746f 7269  mer,TfidfVectori
+00010f90: 7a65 720d 0a66 726f 6d20 736b 6c65 6172  zer..from sklear
+00010fa0: 6e2e 6665 6174 7572 655f 6578 7472 6163  n.feature_extrac
+00010fb0: 7469 6f6e 2e74 6578 7420 696d 706f 7274  tion.text import
+00010fc0: 2043 6f75 6e74 5665 6374 6f72 697a 6572   CountVectorizer
+00010fd0: 0d0a 236e 6c74 6b2e 646f 776e 6c6f 6164  ..#nltk.download
+00010fe0: 2827 7075 6e6b 7427 290d 0a69 6d70 6f72  ('punkt')..impor
+00010ff0: 7420 7761 726e 696e 6773 0d0a 7761 726e  t warnings..warn
+00011000: 696e 6773 2e66 696c 7465 7277 6172 6e69  ings.filterwarni
+00011010: 6e67 7328 2269 676e 6f72 6522 290d 0a0d  ngs("ignore")...
+00011020: 0a23 6e6c 746b 2e64 6f77 6e6c 6f61 6428  .#nltk.download(
+00011030: 2773 746f 7077 6f72 6473 2729 0d0a 0d0a  'stopwords')....
+00011040: 6465 6620 6765 745f 7374 6f70 5f77 6f72  def get_stop_wor
+00011050: 6473 2829 3a0d 0a20 2020 2022 2222 6c6f  ds():..    """lo
+00011060: 6164 2073 746f 7020 776f 7264 7320 2222  ad stop words ""
+00011070: 220d 0a20 2020 2072 6574 7572 6e20 7374  "..    return st
+00011080: 6f70 776f 7264 732e 776f 7264 7328 2765  opwords.words('e
+00011090: 6e67 6c69 7368 2729 0d0a 2020 2020 0d0a  nglish')..    ..
+000110a0: 2323 2020 2020 7769 7468 206f 7065 6e28  ##    with open(
+000110b0: 2773 746f 7077 6f72 6473 2e74 7874 272c  'stopwords.txt',
+000110c0: 2027 7227 2c20 656e 636f 6469 6e67 3d22   'r', encoding="
+000110d0: 7574 662d 3822 2920 6173 2066 3a0d 0a23  utf-8") as f:..#
+000110e0: 2320 2020 2020 2020 2073 746f 7077 6f72  #        stopwor
+000110f0: 6473 203d 2066 2e72 6561 646c 696e 6573  ds = f.readlines
+00011100: 2829 0d0a 2323 2020 2020 2020 2020 7374  ()..##        st
+00011110: 6f70 5f73 6574 203d 2073 6574 286d 2e73  op_set = set(m.s
+00011120: 7472 6970 2829 2066 6f72 206d 2069 6e20  trip() for m in 
+00011130: 7374 6f70 776f 7264 7329 0d0a 2323 2020  stopwords)..##  
+00011140: 2020 2020 2320 2070 7269 6e74 2866 726f      #  print(fro
+00011150: 7a65 6e73 6574 2873 746f 705f 7365 7429  zenset(stop_set)
+00011160: 290d 0a23 2320 2020 2020 2020 2072 6574  )..##        ret
+00011170: 7572 6e20 6672 6f7a 656e 7365 7428 7374  urn frozenset(st
+00011180: 6f70 5f73 6574 290d 0a0d 0a64 6566 2073  op_set)....def s
+00011190: 6372 6170 6577 6562 2874 6865 7572 6c29  crapeweb(theurl)
+000111a0: 3a0d 0a20 2020 2073 6372 6170 6564 5f64  :..    scraped_d
+000111b0: 6174 6120 3d20 7572 6c6c 6962 2e72 6571  ata = urllib.req
+000111c0: 7565 7374 2e75 726c 6f70 656e 2874 6865  uest.urlopen(the
+000111d0: 7572 6c29 2020 0d0a 2020 2020 6172 7469  url)  ..    arti
+000111e0: 636c 6520 3d20 7363 7261 7065 645f 6461  cle = scraped_da
+000111f0: 7461 2e72 6561 6428 290d 0a0d 0a20 2020  ta.read()....   
+00011200: 2070 6172 7365 645f 6172 7469 636c 6520   parsed_article 
+00011210: 3d20 6273 2e42 6561 7574 6966 756c 536f  = bs.BeautifulSo
+00011220: 7570 2861 7274 6963 6c65 2c27 6c78 6d6c  up(article,'lxml
+00011230: 2729 0d0a 0d0a 2020 2020 7061 7261 6772  ')....    paragr
+00011240: 6170 6873 203d 2070 6172 7365 645f 6172  aphs = parsed_ar
+00011250: 7469 636c 652e 6669 6e64 5f61 6c6c 2827  ticle.find_all('
+00011260: 7027 290d 0a0d 0a20 2020 2061 7274 6963  p')....    artic
+00011270: 6c65 5f74 6578 7420 3d20 2222 0d0a 0d0a  le_text = ""....
+00011280: 2020 2020 666f 7220 7020 696e 2070 6172      for p in par
+00011290: 6167 7261 7068 733a 2020 0d0a 2020 2020  agraphs:  ..    
+000112a0: 2020 2020 6172 7469 636c 655f 7465 7874      article_text
+000112b0: 202b 3d20 702e 7465 7874 0d0a 2020 2020   += p.text..    
+000112c0: 7265 7475 726e 2061 7274 6963 6c65 5f74  return article_t
+000112d0: 6578 7420 0d0a 0d0a 6465 6620 636f 6e76  ext ....def conv
+000112e0: 6572 7474 6f6c 6f77 6572 6361 7365 2864  erttolowercase(d
+000112f0: 662c 636f 6c29 3a0d 0a20 2020 2020 2064  f,col):..      d
+00011300: 665b 636f 6c5d 203d 2064 665b 636f 6c5d  f[col] = df[col]
+00011310: 2e61 7070 6c79 286c 616d 6264 6120 783a  .apply(lambda x:
+00011320: 2022 2022 2e6a 6f69 6e28 782e 6c6f 7765   " ".join(x.lowe
+00011330: 7228 2920 666f 7220 7820 696e 2078 2e73  r() for x in x.s
+00011340: 706c 6974 2829 2929 0d0a 2020 2020 2020  plit()))..      
+00011350: 7265 7475 726e 2064 660d 0a20 2020 200d  return df..    .
+00011360: 0a64 6566 2072 656d 6f76 6570 756e 6374  .def removepunct
+00011370: 7561 7469 6f6e 2864 662c 636f 6c29 3a0d  uation(df,col):.
+00011380: 0a20 2020 2020 2064 665b 636f 6c5d 203d  .      df[col] =
+00011390: 2064 665b 636f 6c5d 2e73 7472 2e72 6570   df[col].str.rep
+000113a0: 6c61 6365 2827 5b5e 5c77 5c73 5d27 2c27  lace('[^\w\s]','
+000113b0: 2729 0d0a 2020 2020 2020 7265 7475 726e  ')..      return
+000113c0: 2064 660d 0a0d 0a64 6566 2072 656d 6f76   df....def remov
+000113d0: 6573 746f 7077 6f72 6473 2864 662c 636f  estopwords(df,co
+000113e0: 6c29 3a0d 0a20 2020 2020 2073 746f 7020  l):..      stop 
+000113f0: 3d20 7374 6f70 776f 7264 732e 776f 7264  = stopwords.word
+00011400: 7328 2765 6e67 6c69 7368 2729 0d0a 2020  s('english')..  
+00011410: 2020 2020 6466 5b63 6f6c 5d20 3d20 6466      df[col] = df
+00011420: 5b63 6f6c 5d2e 6170 706c 7928 6c61 6d62  [col].apply(lamb
+00011430: 6461 2078 3a20 2220 222e 6a6f 696e 2878  da x: " ".join(x
+00011440: 2066 6f72 2078 2069 6e20 782e 7370 6c69   for x in x.spli
+00011450: 7428 2920 6966 2078 206e 6f74 2069 6e20  t() if x not in 
+00011460: 7374 6f70 2929 0d0a 2020 2020 2020 7265  stop))..      re
+00011470: 7475 726e 2064 660d 0a0d 0a64 6566 2072  turn df....def r
+00011480: 656d 6f76 6563 6f6d 6d6f 6e77 6f72 6473  emovecommonwords
+00011490: 2864 662c 636f 6c29 3a0d 0a20 2020 2020  (df,col):..     
+000114a0: 2066 7265 7120 3d20 7064 2e53 6572 6965   freq = pd.Serie
+000114b0: 7328 2720 272e 6a6f 696e 2864 665b 636f  s(' '.join(df[co
+000114c0: 6c5d 292e 7370 6c69 7428 2929 2e76 616c  l]).split()).val
+000114d0: 7565 5f63 6f75 6e74 7328 295b 3a31 305d  ue_counts()[:10]
+000114e0: 0d0a 2020 2020 2020 6672 6571 203d 206c  ..      freq = l
+000114f0: 6973 7428 6672 6571 2e69 6e64 6578 290d  ist(freq.index).
+00011500: 0a20 2020 2020 2064 665b 636f 6c5d 203d  .      df[col] =
+00011510: 2064 665b 636f 6c5d 2e61 7070 6c79 286c   df[col].apply(l
+00011520: 616d 6264 6120 783a 2022 2022 2e6a 6f69  ambda x: " ".joi
+00011530: 6e28 7820 666f 7220 7820 696e 2078 2e73  n(x for x in x.s
+00011540: 706c 6974 2829 2069 6620 7820 6e6f 7420  plit() if x not 
+00011550: 696e 2066 7265 7129 290d 0a20 2020 2020  in freq))..     
+00011560: 2072 6574 7572 6e20 6466 0d0a 0d0a 6465   return df....de
+00011570: 6620 7265 6d6f 7665 7261 7265 776f 7264  f removerareword
+00011580: 7328 6466 2c63 6f6c 293a 0d0a 2020 2020  s(df,col):..    
+00011590: 2020 6672 6571 203d 2070 642e 5365 7269    freq = pd.Seri
+000115a0: 6573 2827 2027 2e6a 6f69 6e28 6466 5b63  es(' '.join(df[c
+000115b0: 6f6c 5d29 2e73 706c 6974 2829 292e 7661  ol]).split()).va
+000115c0: 6c75 655f 636f 756e 7473 2829 5b2d 3130  lue_counts()[-10
+000115d0: 3a5d 0d0a 2020 2020 2020 6672 6571 203d  :]..      freq =
+000115e0: 206c 6973 7428 6672 6571 2e69 6e64 6578   list(freq.index
+000115f0: 290d 0a20 2020 2020 2064 665b 636f 6c5d  )..      df[col]
+00011600: 203d 2064 665b 636f 6c5d 2e61 7070 6c79   = df[col].apply
+00011610: 286c 616d 6264 6120 783a 2022 2022 2e6a  (lambda x: " ".j
+00011620: 6f69 6e28 7820 666f 7220 7820 696e 2078  oin(x for x in x
+00011630: 2e73 706c 6974 2829 2069 6620 7820 6e6f  .split() if x no
+00011640: 7420 696e 2066 7265 7129 290d 0a20 2020  t in freq))..   
+00011650: 2020 2072 6574 7572 6e20 6466 0d0a 0d0a     return df....
+00011660: 6465 6620 636f 7272 6563 7473 7065 6c6c  def correctspell
+00011670: 696e 6728 6466 2c63 6f6c 293a 0d0a 2020  ing(df,col):..  
+00011680: 2020 2020 6466 5b63 6f6c 5d5b 3a35 5d2e      df[col][:5].
+00011690: 6170 706c 7928 6c61 6d62 6461 2078 3a20  apply(lambda x: 
+000116a0: 7374 7228 5465 7874 426c 6f62 2878 292e  str(TextBlob(x).
+000116b0: 636f 7272 6563 7428 2929 290d 0a20 2020  correct()))..   
+000116c0: 2020 2072 6574 7572 6e20 6466 0d0a 0d0a     return df....
+000116d0: 6465 6620 6c65 6d6d 6174 697a 6174 696f  def lemmatizatio
+000116e0: 6e28 6466 2c63 6f6c 293a 0d0a 2020 2020  n(df,col):..    
+000116f0: 2020 6466 5b63 6f6c 5d20 3d20 6466 5b63    df[col] = df[c
+00011700: 6f6c 5d2e 6170 706c 7928 6c61 6d62 6461  ol].apply(lambda
+00011710: 2078 3a20 2220 222e 6a6f 696e 285b 576f   x: " ".join([Wo
+00011720: 7264 2877 6f72 6429 2e6c 656d 6d61 7469  rd(word).lemmati
+00011730: 7a65 2829 2066 6f72 2077 6f72 6420 696e  ze() for word in
+00011740: 2078 2e73 706c 6974 2829 5d29 290d 0a20   x.split()])).. 
+00011750: 2020 2020 2072 6574 7572 6e20 6466 0d0a       return df..
+00011760: 0d0a 6465 6620 7472 6169 6e76 6563 7428  ..def trainvect(
+00011770: 6376 2c74 626f 772c 6466 2c63 6f6c 2c6d  cv,tbow,df,col,m
+00011780: 6178 6b65 7977 6f72 6473 293a 0d0a 2020  axkeywords):..  
+00011790: 2020 2020 7465 7874 3d64 665b 636f 6c5d      text=df[col]
+000117a0: 2e74 6f6c 6973 7428 290d 0a20 2020 2020  .tolist()..     
+000117b0: 2074 6669 6466 203d 2054 6669 6466 5472   tfidf = TfidfTr
+000117c0: 616e 7366 6f72 6d65 7228 736d 6f6f 7468  ansformer(smooth
+000117d0: 5f69 6466 3d54 7275 652c 7573 655f 6964  _idf=True,use_id
+000117e0: 663d 5472 7565 290d 0a20 2020 2020 2074  f=True)..      t
+000117f0: 6669 6466 2e66 6974 2874 626f 7729 0d0a  fidf.fit(tbow)..
+00011800: 2020 2020 2020 7466 5f69 6466 5f76 6563        tf_idf_vec
+00011810: 746f 723d 7466 6964 662e 7472 616e 7366  tor=tfidf.transf
+00011820: 6f72 6d28 6376 2e74 7261 6e73 666f 726d  orm(cv.transform
+00011830: 2874 6578 7429 290d 0a20 2020 2020 2073  (text))..      s
+00011840: 6f72 7465 6469 7465 6d73 3d73 6f72 745f  orteditems=sort_
+00011850: 636f 6f28 7466 5f69 6466 5f76 6563 746f  coo(tf_idf_vecto
+00011860: 722e 746f 636f 6f28 2929 0d0a 2020 2020  r.tocoo())..    
+00011870: 2020 6665 6174 7572 656e 616d 6573 3d63    featurenames=c
+00011880: 762e 6765 745f 6665 6174 7572 655f 6e61  v.get_feature_na
+00011890: 6d65 735f 6f75 7428 290d 0a20 2020 2020  mes_out()..     
+000118a0: 206b 6579 776f 7264 733d 6578 7472 6163   keywords=extrac
+000118b0: 745f 746f 706e 5f66 726f 6d5f 7665 6374  t_topn_from_vect
+000118c0: 6f72 2866 6561 7475 7265 6e61 6d65 732c  or(featurenames,
+000118d0: 736f 7274 6564 6974 656d 732c 6d61 786b  sorteditems,maxk
+000118e0: 6579 776f 7264 7329 0d0a 2020 2020 2020  eywords)..      
+000118f0: 6b65 7977 6f72 6473 3d6a 736f 6e2e 6475  keywords=json.du
+00011900: 6d70 7328 6b65 7977 6f72 6473 290d 0a20  mps(keywords).. 
+00011910: 2020 2020 2320 7072 696e 7428 6b65 7977      # print(keyw
+00011920: 6f72 6473 290d 0a20 2020 2020 2072 6574  ords)..      ret
+00011930: 7572 6e20 6b65 7977 6f72 6473 0d0a 0d0a  urn keywords....
+00011940: 6465 6620 7472 6169 6e62 6f77 2864 662c  def trainbow(df,
+00011950: 636f 6c29 3a0d 0a20 2020 2020 206d 796c  col):..      myl
+00011960: 6973 743d 6466 5b63 6f6c 5d2e 746f 6c69  ist=df[col].toli
+00011970: 7374 2829 0d0a 2020 2020 2020 7374 6f70  st()..      stop
+00011980: 776f 7264 733d 6765 745f 7374 6f70 5f77  words=get_stop_w
+00011990: 6f72 6473 2829 0d0a 2020 2020 2020 6376  ords()..      cv
+000119a0: 203d 2043 6f75 6e74 5665 6374 6f72 697a   = CountVectoriz
+000119b0: 6572 2873 746f 705f 776f 7264 733d 7374  er(stop_words=st
+000119c0: 6f70 776f 7264 7329 0d0a 2020 2020 2020  opwords)..      
+000119d0: 7472 6169 6e5f 626f 7720 3d20 6376 2e66  train_bow = cv.f
+000119e0: 6974 5f74 7261 6e73 666f 726d 286d 796c  it_transform(myl
+000119f0: 6973 7429 0d0a 2020 2020 2020 2370 7269  ist)..      #pri
+00011a00: 6e74 286c 6973 7428 6376 2e76 6f63 6162  nt(list(cv.vocab
+00011a10: 756c 6172 795f 2e6b 6579 7328 2929 290d  ulary_.keys())).
+00011a20: 0a20 2020 2020 2072 6574 7572 6e20 6376  .      return cv
+00011a30: 2c74 7261 696e 5f62 6f77 0d0a 0d0a 200d  ,train_bow.... .
+00011a40: 0a64 6566 2073 6f72 745f 636f 6f28 636f  .def sort_coo(co
+00011a50: 6f5f 6d61 7472 6978 293a 0d0a 2020 2020  o_matrix):..    
+00011a60: 7475 706c 6573 203d 207a 6970 2863 6f6f  tuples = zip(coo
+00011a70: 5f6d 6174 7269 782e 636f 6c2c 2063 6f6f  _matrix.col, coo
+00011a80: 5f6d 6174 7269 782e 6461 7461 290d 0a20  _matrix.data).. 
+00011a90: 2020 2072 6574 7572 6e20 736f 7274 6564     return sorted
+00011aa0: 2874 7570 6c65 732c 206b 6579 3d6c 616d  (tuples, key=lam
+00011ab0: 6264 6120 783a 2028 785b 315d 2c20 785b  bda x: (x[1], x[
+00011ac0: 305d 292c 2072 6576 6572 7365 3d54 7275  0]), reverse=Tru
+00011ad0: 6529 0d0a 0d0a 6465 6620 6578 7472 6163  e)....def extrac
+00011ae0: 745f 746f 706e 5f66 726f 6d5f 7665 6374  t_topn_from_vect
+00011af0: 6f72 2866 6561 7475 7265 5f6e 616d 6573  or(feature_names
+00011b00: 2c20 736f 7274 6564 5f69 7465 6d73 2c20  , sorted_items, 
+00011b10: 746f 706e 3d31 3029 3a0d 0a20 2020 2022  topn=10):..    "
+00011b20: 2222 6765 7420 7468 6520 6665 6174 7572  ""get the featur
+00011b30: 6520 6e61 6d65 7320 616e 6420 7466 2d69  e names and tf-i
+00011b40: 6466 2073 636f 7265 206f 6620 746f 7020  df score of top 
+00011b50: 6e20 6974 656d 7322 2222 0d0a 2020 2020  n items"""..    
+00011b60: 0d0a 2020 2020 2375 7365 206f 6e6c 7920  ..    #use only 
+00011b70: 746f 706e 2069 7465 6d73 2066 726f 6d20  topn items from 
+00011b80: 7665 6374 6f72 0d0a 2020 2020 736f 7274  vector..    sort
+00011b90: 6564 5f69 7465 6d73 203d 2073 6f72 7465  ed_items = sorte
+00011ba0: 645f 6974 656d 735b 3a74 6f70 6e5d 0d0a  d_items[:topn]..
+00011bb0: 0d0a 2020 2020 7363 6f72 655f 7661 6c73  ..    score_vals
+00011bc0: 203d 205b 5d0d 0a20 2020 2066 6561 7475   = []..    featu
+00011bd0: 7265 5f76 616c 7320 3d20 5b5d 0d0a 0d0a  re_vals = []....
+00011be0: 2020 2020 666f 7220 6964 782c 2073 636f      for idx, sco
+00011bf0: 7265 2069 6e20 736f 7274 6564 5f69 7465  re in sorted_ite
+00011c00: 6d73 3a20 2020 2020 2020 200d 0a20 2020  ms:        ..   
+00011c10: 2020 2020 2020 2066 6e61 6d65 203d 2066         fname = f
+00011c20: 6561 7475 7265 5f6e 616d 6573 5b69 6478  eature_names[idx
+00011c30: 5d0d 0a20 2020 2020 2020 2020 2069 6620  ]..          if 
+00011c40: 6c65 6e28 666e 616d 6529 3e33 3a0d 0a20  len(fname)>3:.. 
+00011c50: 2020 2020 2020 2023 6b65 6570 2074 7261         #keep tra
+00011c60: 636b 206f 6620 6665 6174 7572 6520 6e61  ck of feature na
+00011c70: 6d65 2061 6e64 2069 7473 2063 6f72 7265  me and its corre
+00011c80: 7370 6f6e 6469 6e67 2073 636f 7265 0d0a  sponding score..
+00011c90: 2020 2020 2020 2020 2020 2020 7363 6f72              scor
+00011ca0: 655f 7661 6c73 2e61 7070 656e 6428 726f  e_vals.append(ro
+00011cb0: 756e 6428 7363 6f72 652c 2033 2929 0d0a  und(score, 3))..
+00011cc0: 2020 2020 2020 2020 2020 2020 6665 6174              feat
+00011cd0: 7572 655f 7661 6c73 2e61 7070 656e 6428  ure_vals.append(
+00011ce0: 6665 6174 7572 655f 6e61 6d65 735b 6964  feature_names[id
+00011cf0: 785d 290d 0a0d 0a20 2020 2023 6372 6561  x])....    #crea
+00011d00: 7465 2061 2074 7570 6c65 7320 6f66 2066  te a tuples of f
+00011d10: 6561 7475 7265 2c73 636f 7265 0d0a 2020  eature,score..  
+00011d20: 2020 2372 6573 756c 7473 203d 207a 6970    #results = zip
+00011d30: 2866 6561 7475 7265 5f76 616c 732c 7363  (feature_vals,sc
+00011d40: 6f72 655f 7661 6c73 290d 0a20 2020 2072  ore_vals)..    r
+00011d50: 6573 756c 7473 3d20 7b7d 0d0a 2020 2020  esults= {}..    
+00011d60: 666f 7220 6964 7820 696e 2072 616e 6765  for idx in range
+00011d70: 286c 656e 2866 6561 7475 7265 5f76 616c  (len(feature_val
+00011d80: 7329 293a 0d0a 2020 2020 2020 2020 7265  s)):..        re
+00011d90: 7375 6c74 735b 6665 6174 7572 655f 7661  sults[feature_va
+00011da0: 6c73 5b69 6478 5d5d 3d73 636f 7265 5f76  ls[idx]]=score_v
+00011db0: 616c 735b 6964 785d 0d0a 2020 2020 0d0a  als[idx]..    ..
+00011dc0: 2020 2020 7265 7475 726e 2072 6573 756c      return resul
+00011dd0: 7473 0d0a 0d0a 6465 6620 6765 746b 6579  ts....def getkey
+00011de0: 776f 7264 7328 6d79 7465 7874 2c6d 6178  words(mytext,max
+00011df0: 6b65 7977 6f72 6473 293a 0d0a 2020 2020  keywords):..    
+00011e00: 723d 5261 6b65 286d 6178 5f6c 656e 6774  r=Rake(max_lengt
+00011e10: 683d 3130 290d 0a20 2020 2072 203d 2052  h=10)..    r = R
+00011e20: 616b 6528 7261 6e6b 696e 675f 6d65 7472  ake(ranking_metr
+00011e30: 6963 3d4d 6574 7269 632e 4445 4752 4545  ic=Metric.DEGREE
+00011e40: 5f54 4f5f 4652 4551 5545 4e43 595f 5241  _TO_FREQUENCY_RA
+00011e50: 5449 4f29 0d0a 2020 2020 2372 203d 2052  TIO)..    #r = R
+00011e60: 616b 6528 7261 6e6b 696e 675f 6d65 7472  ake(ranking_metr
+00011e70: 6963 3d4d 6574 7269 632e 574f 5244 5f44  ic=Metric.WORD_D
+00011e80: 4547 5245 4529 0d0a 2020 2020 2372 203d  EGREE)..    #r =
+00011e90: 2052 616b 6528 7261 6e6b 696e 675f 6d65   Rake(ranking_me
+00011ea0: 7472 6963 3d4d 6574 7269 632e 574f 5244  tric=Metric.WORD
+00011eb0: 5f46 5245 5155 454e 4359 290d 0a20 2020  _FREQUENCY)..   
+00011ec0: 2064 3d7b 2769 6e70 7574 273a 5b6d 7974   d={'input':[myt
+00011ed0: 6578 745d 7d0d 0a20 2020 2064 6620 3d20  ext]}..    df = 
+00011ee0: 7064 2e44 6174 6146 7261 6d65 2864 290d  pd.DataFrame(d).
+00011ef0: 0a20 2020 2064 663d 636f 6e76 6572 7474  .    df=convertt
+00011f00: 6f6c 6f77 6572 6361 7365 2864 662c 2769  olowercase(df,'i
+00011f10: 6e70 7574 2729 0d0a 2020 2020 6466 3d72  nput')..    df=r
+00011f20: 656d 6f76 6570 756e 6374 7561 7469 6f6e  emovepunctuation
+00011f30: 2864 662c 2769 6e70 7574 2729 0d0a 2020  (df,'input')..  
+00011f40: 2020 6466 3d72 656d 6f76 6573 746f 7077    df=removestopw
+00011f50: 6f72 6473 2864 662c 2769 6e70 7574 2729  ords(df,'input')
+00011f60: 0d0a 2020 2020 6466 3d72 656d 6f76 6563  ..    df=removec
+00011f70: 6f6d 6d6f 6e77 6f72 6473 2864 662c 2769  ommonwords(df,'i
+00011f80: 6e70 7574 2729 0d0a 2020 2020 6466 3d72  nput')..    df=r
+00011f90: 656d 6f76 6572 6172 6577 6f72 6473 2864  emoverarewords(d
+00011fa0: 662c 2769 6e70 7574 2729 0d0a 2020 2020  f,'input')..    
+00011fb0: 6466 3d63 6f72 7265 6374 7370 656c 6c69  df=correctspelli
+00011fc0: 6e67 2864 662c 2769 6e70 7574 2729 0d0a  ng(df,'input')..
+00011fd0: 2020 2020 6466 3d6c 656d 6d61 7469 7a61      df=lemmatiza
+00011fe0: 7469 6f6e 2864 662c 2769 6e70 7574 2729  tion(df,'input')
+00011ff0: 0d0a 2020 2020 6d79 7465 7874 3d64 665b  ..    mytext=df[
+00012000: 2769 6e70 7574 275d 5b30 5d0d 0a20 2020  'input'][0]..   
+00012010: 2063 762c 7477 3d74 7261 696e 626f 7728   cv,tw=trainbow(
+00012020: 6466 2c27 696e 7075 7427 290d 0a20 2020  df,'input')..   
+00012030: 206b 6579 776f 7264 733d 7472 6169 6e76   keywords=trainv
+00012040: 6563 7428 6376 2c74 772c 6466 2c27 696e  ect(cv,tw,df,'in
+00012050: 7075 7427 2c6d 6178 6b65 7977 6f72 6473  put',maxkeywords
+00012060: 290d 0a0d 0a20 2020 2072 6574 7572 6e20  )....    return 
+00012070: 6b65 7977 6f72 6473 0d0a 2020 2020 2370  keywords..    #p
+00012080: 7269 6e74 2874 7729 0d0a 2320 2020 206d  rint(tw)..#    m
+00012090: 7974 6578 743d 7064 2e53 6572 6965 7328  ytext=pd.Series(
+000120a0: 6d79 7465 7874 290d 0a20 2020 2023 7072  mytext)..    #pr
+000120b0: 696e 7428 6d79 7465 7874 290d 0a23 2020  int(mytext)..#  
+000120c0: 2020 733d 732e 7374 722e 7370 6c69 7428    s=s.str.split(
+000120d0: 290d 0a20 2020 2020 200d 0a20 2020 2320  )..      ..   # 
+000120e0: 6b77 3d72 2e65 7874 7261 6374 5f6b 6579  kw=r.extract_key
+000120f0: 776f 7264 735f 6672 6f6d 5f74 6578 7428  words_from_text(
+00012100: 6d79 7465 7874 290d 0a20 2020 2320 6b73  mytext)..   # ks
+00012110: 3d72 2e67 6574 5f72 616e 6b65 645f 7068  =r.get_ranked_ph
+00012120: 7261 7365 735f 7769 7468 5f73 636f 7265  rases_with_score
+00012130: 7328 290d 0a20 2020 200d 0a20 2020 2023  s()..    ..    #
+00012140: 7072 696e 7428 6b65 7977 6f72 6473 290d  print(keywords).
+00012150: 0a0d 0a23 6d79 7465 7874 3d22 4578 7472  ...#mytext="Extr
+00012160: 656d 656c 7920 696d 706f 7274 616e 7420  emely important 
+00012170: 706f 696e 743a 2074 6865 2049 4446 2073  point: the IDF s
+00012180: 686f 756c 6420 616c 7761 7973 2062 6520  hould always be 
+00012190: 6261 7365 6420 6f6e 2061 206c 6172 6765  based on a large
+000121a0: 2063 6f72 706f 7261 2c20 616e 6420 7368   corpora, and sh
+000121b0: 6f75 6c64 2062 6520 7265 7072 6573 656e  ould be represen
+000121c0: 7461 7469 7665 205c 0d0a 236f 6620 7465  tative \..#of te
+000121d0: 7874 7320 796f 7520 776f 756c 6420 6265  xts you would be
+000121e0: 2075 7369 6e67 2074 6f20 6578 7472 6163   using to extrac
+000121f0: 7420 6b65 7977 6f72 6473 2e20 49e2 8099  t keywords. I...
+00012200: 7665 2073 6565 6e20 7365 7665 7261 6c20  ve seen several 
+00012210: 6172 7469 636c 6573 206f 6e20 7468 6520  articles on the 
+00012220: 5765 6220 7468 6174 2063 6f6d 7075 7465  Web that compute
+00012230: 2074 6865 2049 4446 2075 7369 6e67 2061   the IDF using a
+00012240: 205c 0d0a 2368 616e 6466 756c 206f 6620   \..#handful of 
+00012250: 646f 6375 6d65 6e74 732e 2059 6f75 2077  documents. You w
+00012260: 696c 6c20 6465 6665 6174 2074 6865 2077  ill defeat the w
+00012270: 686f 6c65 2070 7572 706f 7365 206f 6620  hole purpose of 
+00012280: 4944 4620 7765 6967 6874 696e 6720 6966  IDF weighting if
+00012290: 2069 7473 206e 6f74 2062 6173 6564 206f   its not based o
+000122a0: 6e20 6120 6c61 7267 6520 636f 7270 6f72  n a large corpor
+000122b0: 6120 6173 220d 0a0d 0a23 6765 746b 6579  a as"....#getkey
+000122c0: 776f 7264 7328 6d79 7465 7874 290d 0a0d  words(mytext)...
+000122d0: 0a64 6566 2064 6f73 756d 6d61 7279 2861  .def dosummary(a
+000122e0: 7274 6963 6c65 5f74 6578 742c 6929 3a0d  rticle_text,i):.
+000122f0: 0a0d 0a0d 0a20 2020 2061 7274 6963 6c65  .....    article
+00012300: 5f74 6578 7420 3d20 7265 2e73 7562 2872  _text = re.sub(r
+00012310: 275c 5b5b 302d 395d 2a5c 5d27 2c20 2720  '\[[0-9]*\]', ' 
+00012320: 272c 2061 7274 6963 6c65 5f74 6578 7429  ', article_text)
+00012330: 2020 0d0a 2020 2020 6172 7469 636c 655f    ..    article_
+00012340: 7465 7874 203d 2072 652e 7375 6228 7227  text = re.sub(r'
+00012350: 5c73 2b27 2c20 2720 272c 2061 7274 6963  \s+', ' ', artic
+00012360: 6c65 5f74 6578 7429 0d0a 0d0a 2020 2020  le_text)....    
+00012370: 2320 5265 6d6f 7669 6e67 2073 7065 6369  # Removing speci
+00012380: 616c 2063 6861 7261 6374 6572 7320 616e  al characters an
+00012390: 6420 6469 6769 7473 0d0a 2020 2020 666f  d digits..    fo
+000123a0: 726d 6174 7465 645f 6172 7469 636c 655f  rmatted_article_
+000123b0: 7465 7874 203d 2072 652e 7375 6228 275b  text = re.sub('[
+000123c0: 5e61 2d7a 412d 5a5d 272c 2027 2027 2c20  ^a-zA-Z]', ' ', 
+000123d0: 6172 7469 636c 655f 7465 7874 2029 2020  article_text )  
+000123e0: 0d0a 2020 2020 666f 726d 6174 7465 645f  ..    formatted_
+000123f0: 6172 7469 636c 655f 7465 7874 203d 2072  article_text = r
+00012400: 652e 7375 6228 7227 5c73 2b27 2c20 2720  e.sub(r'\s+', ' 
+00012410: 272c 2066 6f72 6d61 7474 6564 5f61 7274  ', formatted_art
+00012420: 6963 6c65 5f74 6578 7429 2020 0d0a 0d0a  icle_text)  ....
+00012430: 2020 2020 7365 6e74 656e 6365 5f6c 6973      sentence_lis
+00012440: 7420 3d20 6e6c 746b 2e73 656e 745f 746f  t = nltk.sent_to
+00012450: 6b65 6e69 7a65 2861 7274 6963 6c65 5f74  kenize(article_t
+00012460: 6578 7429 2020 0d0a 2020 2020 2370 7269  ext)  ..    #pri
+00012470: 6e74 2873 656e 7465 6e63 655f 6c69 7374  nt(sentence_list
+00012480: 290d 0a0d 0a20 2020 2073 746f 7077 6f72  )....    stopwor
+00012490: 6473 203d 206e 6c74 6b2e 636f 7270 7573  ds = nltk.corpus
+000124a0: 2e73 746f 7077 6f72 6473 2e77 6f72 6473  .stopwords.words
+000124b0: 2827 656e 676c 6973 6827 290d 0a0d 0a20  ('english').... 
+000124c0: 2020 2077 6f72 645f 6672 6571 7565 6e63     word_frequenc
+000124d0: 6965 7320 3d20 7b7d 2020 0d0a 2020 2020  ies = {}  ..    
+000124e0: 666f 7220 776f 7264 2069 6e20 6e6c 746b  for word in nltk
+000124f0: 2e77 6f72 645f 746f 6b65 6e69 7a65 2866  .word_tokenize(f
+00012500: 6f72 6d61 7474 6564 5f61 7274 6963 6c65  ormatted_article
+00012510: 5f74 6578 7429 3a20 200d 0a20 2020 2020  _text):  ..     
+00012520: 2020 2069 6620 776f 7264 206e 6f74 2069     if word not i
+00012530: 6e20 7374 6f70 776f 7264 733a 0d0a 2020  n stopwords:..  
+00012540: 2020 2020 2020 2020 2020 6966 2077 6f72            if wor
+00012550: 6420 6e6f 7420 696e 2077 6f72 645f 6672  d not in word_fr
+00012560: 6571 7565 6e63 6965 732e 6b65 7973 2829  equencies.keys()
+00012570: 3a0d 0a20 2020 2020 2020 2020 2020 2020  :..             
+00012580: 2020 2077 6f72 645f 6672 6571 7565 6e63     word_frequenc
+00012590: 6965 735b 776f 7264 5d20 3d20 310d 0a20  ies[word] = 1.. 
+000125a0: 2020 2020 2020 2020 2020 2065 6c73 653a             else:
+000125b0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+000125c0: 2020 776f 7264 5f66 7265 7175 656e 6369    word_frequenci
+000125d0: 6573 5b77 6f72 645d 202b 3d20 310d 0a0d  es[word] += 1...
+000125e0: 0a20 2020 206d 6178 696d 756d 5f66 7265  .    maximum_fre
+000125f0: 7175 6e63 7920 3d20 6d61 7828 776f 7264  quncy = max(word
+00012600: 5f66 7265 7175 656e 6369 6573 2e76 616c  _frequencies.val
+00012610: 7565 7328 2929 0d0a 0d0a 2020 2020 666f  ues())....    fo
+00012620: 7220 776f 7264 2069 6e20 776f 7264 5f66  r word in word_f
+00012630: 7265 7175 656e 6369 6573 2e6b 6579 7328  requencies.keys(
+00012640: 293a 2020 0d0a 2020 2020 2020 2020 776f  ):  ..        wo
+00012650: 7264 5f66 7265 7175 656e 6369 6573 5b77  rd_frequencies[w
+00012660: 6f72 645d 203d 2028 776f 7264 5f66 7265  ord] = (word_fre
+00012670: 7175 656e 6369 6573 5b77 6f72 645d 2f6d  quencies[word]/m
+00012680: 6178 696d 756d 5f66 7265 7175 6e63 7929  aximum_frequncy)
+00012690: 0d0a 0d0a 2020 2020 2370 7269 6e74 2877  ....    #print(w
+000126a0: 6f72 645f 6672 6571 7565 6e63 6965 7329  ord_frequencies)
+000126b0: 0d0a 0d0a 2020 2020 7365 6e74 656e 6365  ....    sentence
+000126c0: 5f73 636f 7265 7320 3d20 7b7d 2020 0d0a  _scores = {}  ..
+000126d0: 2020 2020 666f 7220 7365 6e74 2069 6e20      for sent in 
+000126e0: 7365 6e74 656e 6365 5f6c 6973 743a 2020  sentence_list:  
+000126f0: 0d0a 2020 2020 2020 2020 666f 7220 776f  ..        for wo
+00012700: 7264 2069 6e20 6e6c 746b 2e77 6f72 645f  rd in nltk.word_
+00012710: 746f 6b65 6e69 7a65 2873 656e 742e 6c6f  tokenize(sent.lo
+00012720: 7765 7228 2929 3a0d 0a20 2020 2020 2020  wer()):..       
+00012730: 2020 2020 2069 6620 776f 7264 2069 6e20       if word in 
+00012740: 776f 7264 5f66 7265 7175 656e 6369 6573  word_frequencies
+00012750: 2e6b 6579 7328 293a 0d0a 2020 2020 2020  .keys():..      
+00012760: 2020 2020 2020 2020 2020 6966 206c 656e            if len
+00012770: 2873 656e 742e 7370 6c69 7428 2720 2729  (sent.split(' ')
+00012780: 2920 3c20 3235 3a0d 0a20 2020 2020 2020  ) < 25:..       
+00012790: 2020 2020 2020 2020 2020 2020 2069 6620               if 
+000127a0: 7365 6e74 206e 6f74 2069 6e20 7365 6e74  sent not in sent
+000127b0: 656e 6365 5f73 636f 7265 732e 6b65 7973  ence_scores.keys
+000127c0: 2829 3a0d 0a20 2020 2020 2020 2020 2020  ():..           
+000127d0: 2020 2020 2020 2020 2020 2020 2073 656e               sen
+000127e0: 7465 6e63 655f 7363 6f72 6573 5b73 656e  tence_scores[sen
+000127f0: 745d 203d 2077 6f72 645f 6672 6571 7565  t] = word_freque
+00012800: 6e63 6965 735b 776f 7264 5d0d 0a20 2020  ncies[word]..   
+00012810: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012820: 2065 6c73 653a 0d0a 2020 2020 2020 2020   else:..        
+00012830: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012840: 7365 6e74 656e 6365 5f73 636f 7265 735b  sentence_scores[
+00012850: 7365 6e74 5d20 2b3d 2077 6f72 645f 6672  sent] += word_fr
+00012860: 6571 7565 6e63 6965 735b 776f 7264 5d0d  equencies[word].
+00012870: 0a0d 0a20 2020 2023 7072 696e 7428 7365  ...    #print(se
+00012880: 6e74 656e 6365 5f73 636f 7265 7329 0d0a  ntence_scores)..
+00012890: 0d0a 2020 2020 7375 6d6d 6172 795f 7365  ..    summary_se
+000128a0: 6e74 656e 6365 7320 3d20 6865 6170 712e  ntences = heapq.
+000128b0: 6e6c 6172 6765 7374 2869 2c20 7365 6e74  nlargest(i, sent
+000128c0: 656e 6365 5f73 636f 7265 732c 206b 6579  ence_scores, key
+000128d0: 3d73 656e 7465 6e63 655f 7363 6f72 6573  =sentence_scores
+000128e0: 2e67 6574 290d 0a20 2020 2023 7072 696e  .get)..    #prin
+000128f0: 7428 7375 6d6d 6172 795f 7365 6e74 656e  t(summary_senten
+00012900: 6365 7329 0d0a 2020 2020 7375 6d6d 6172  ces)..    summar
+00012910: 7920 3d20 2720 272e 6a6f 696e 2873 756d  y = ' '.join(sum
+00012920: 6d61 7279 5f73 656e 7465 6e63 6573 290d  mary_sentences).
+00012930: 0a20 2020 2023 7072 696e 7428 2241 4920  .    #print("AI 
+00012940: 5375 6d6d 6172 7922 290d 0a20 2020 2072  Summary")..    r
+00012950: 6574 7572 6e20 7375 6d6d 6172 790d 0a0d  eturn summary...
+00012960: 0a64 6566 2073 7461 7274 7375 6d6d 6172  .def startsummar
+00012970: 7928 6172 7469 636c 655f 7465 7874 2c66  y(article_text,f
+00012980: 7661 6c75 652c 6d61 786b 6579 776f 7264  value,maxkeyword
+00012990: 7329 3a0d 0a20 2020 2020 200d 0a20 2320  s):..      .. # 
+000129a0: 7472 793a 0d0a 2020 206f 7269 6769 6e61  try:..   origina
+000129b0: 6c77 6f72 6473 203d 206c 656e 2861 7274  lwords = len(art
+000129c0: 6963 6c65 5f74 6578 742e 7370 6c69 7428  icle_text.split(
+000129d0: 2220 2229 290d 0a0d 0a20 2020 666f 7220  " "))....   for 
+000129e0: 6920 696e 2072 616e 6765 2831 2c31 3030  i in range(1,100
+000129f0: 3030 293a 0d0a 2020 2020 2073 756d 6d61  00):..     summa
+00012a00: 7279 3d64 6f73 756d 6d61 7279 2861 7274  ry=dosummary(art
+00012a10: 6963 6c65 5f74 6578 742c 6929 0d0a 2020  icle_text,i)..  
+00012a20: 2020 2072 6573 203d 206c 656e 2873 756d     res = len(sum
+00012a30: 6d61 7279 2e73 706c 6974 2829 290d 0a20  mary.split()).. 
+00012a40: 2020 2020 6966 2072 6573 203e 3d20 6676      if res >= fv
+00012a50: 616c 7565 3a0d 0a20 2020 2020 2020 2020  alue:..         
+00012a60: 6272 6561 6b0d 0a0d 0a20 2020 7375 6d6d  break....   summ
+00012a70: 6172 7920 3d20 2072 652e 7375 6228 225c  ary =  re.sub("\
+00012a80: 5c5c 5c78 5b61 2d66 302d 395d 5b61 2d66  \\\x[a-f0-9][a-f
+00012a90: 302d 395d 222c 2022 2022 2c73 756d 6d61  0-9]", " ",summa
+00012aa0: 7279 290d 0a20 2020 7375 6d6d 6172 7920  ry)..   summary 
+00012ab0: 3d20 7265 2e73 7562 2822 5c5c 7865 325c  = re.sub("\\xe2\
+00012ac0: 5c78 3830 5c5c 7839 3922 2c22 2722 2c20  \x80\\x99","'", 
+00012ad0: 7375 6d6d 6172 7929 0d0a 2020 2073 756d  summary)..   sum
+00012ae0: 6d61 7279 3d73 756d 6d61 7279 2e72 6570  mary=summary.rep
+00012af0: 6c61 6365 2822 5c5c 7865 325c 5c78 3830  lace("\\xe2\\x80
+00012b00: 5c5c 7839 3922 2c22 2722 290d 0a20 2020  \\x99","'")..   
+00012b10: 7375 6d6d 6172 793d 7375 6d6d 6172 792e  summary=summary.
+00012b20: 7265 706c 6163 6528 225c 5c78 6532 5c5c  replace("\\xe2\\
+00012b30: 7838 305c 5c78 3930 222c 222d 2229 0d0a  x80\\x90","-")..
+00012b40: 2020 2073 756d 6d61 7279 3d73 756d 6d61     summary=summa
+00012b50: 7279 2e72 6570 6c61 6365 2822 5c5c 7865  ry.replace("\\xe
+00012b60: 325c 5c78 3830 5c5c 7839 3122 2c22 2d22  2\\x80\\x91","-"
+00012b70: 290d 0a20 2020 7375 6d6d 6172 793d 7375  )..   summary=su
+00012b80: 6d6d 6172 792e 7265 706c 6163 6528 225c  mmary.replace("\
+00012b90: 5c78 6532 5c5c 7838 305c 5c78 3932 222c  \xe2\\x80\\x92",
+00012ba0: 222d 2229 0d0a 2020 2073 756d 6d61 7279  "-")..   summary
+00012bb0: 3d73 756d 6d61 7279 2e72 6570 6c61 6365  =summary.replace
+00012bc0: 2822 5c5c 7865 325c 5c78 3830 5c5c 7839  ("\\xe2\\x80\\x9
+00012bd0: 3322 2c22 2d22 290d 0a20 2020 7375 6d6d  3","-")..   summ
+00012be0: 6172 793d 7375 6d6d 6172 792e 7265 706c  ary=summary.repl
+00012bf0: 6163 6528 225c 5c78 6532 5c5c 7838 305c  ace("\\xe2\\x80\
+00012c00: 5c78 3934 222c 222d 2229 0d0a 2020 2073  \x94","-")..   s
+00012c10: 756d 6d61 7279 3d73 756d 6d61 7279 2e72  ummary=summary.r
+00012c20: 6570 6c61 6365 2822 5c5c 7865 325c 5c78  eplace("\\xe2\\x
+00012c30: 3830 5c5c 7839 3522 2c22 2d22 290d 0a20  80\\x95","-").. 
+00012c40: 2020 7375 6d6d 6172 793d 7375 6d6d 6172    summary=summar
+00012c50: 792e 7265 706c 6163 6528 225c 5c78 6532  y.replace("\\xe2
+00012c60: 5c5c 7838 305c 5c78 6233 222c 2722 2729  \\x80\\xb3",'"')
+00012c70: 0d0a 2020 2073 756d 6d61 7279 203d 2073  ..   summary = s
+00012c80: 756d 6d61 7279 2e72 6570 6c61 6365 2827  ummary.replace('
+00012c90: e280 9c27 2c20 2722 2729 0d0a 2020 2073  ...', '"')..   s
+00012ca0: 756d 6d61 7279 203d 2073 756d 6d61 7279  ummary = summary
+00012cb0: 2e72 6570 6c61 6365 2827 e280 9d27 2c20  .replace('...', 
+00012cc0: 2722 2729 0d0a 2020 2073 756d 6d61 7279  '"')..   summary
+00012cd0: 203d 2073 756d 6d61 7279 2e72 6570 6c61   = summary.repla
+00012ce0: 6365 2827 e280 9927 2c20 2227 2229 0d0a  ce('...', "'")..
+00012cf0: 2020 2073 756d 6d61 7279 203d 2073 756d     summary = sum
+00012d00: 6d61 7279 2e72 6570 6c61 6365 2827 e280  mary.replace('..
+00012d10: 9827 2c20 2227 2229 0d0a 2020 2073 756d  .', "'")..   sum
+00012d20: 6d61 7279 203d 2073 756d 6d61 7279 2e72  mary = summary.r
+00012d30: 6570 6c61 6365 2827 e280 9327 2c20 222d  eplace('...', "-
+00012d40: 2229 0d0a 2020 2073 756d 6d61 7279 203d  ")..   summary =
+00012d50: 2073 756d 6d61 7279 2e72 6570 6c61 6365   summary.replace
+00012d60: 2827 e280 a627 2c20 222e 2e2e 2229 0d0a  ('...', "...")..
+00012d70: 2020 2073 756d 6d61 7279 203d 2073 756d     summary = sum
+00012d80: 6d61 7279 2e72 6570 6c61 6365 2827 e280  mary.replace('..
+00012d90: 9427 2c20 222d 2229 0d0a 2020 2073 756d  .', "-")..   sum
+00012da0: 6d61 7279 203d 2073 756d 6d61 7279 2e72  mary = summary.r
+00012db0: 6570 6c61 6365 2827 2227 2c20 2222 290d  eplace('"', "").
+00012dc0: 0a0d 0a20 2020 7375 6d6d 6172 7920 3d20  ...   summary = 
+00012dd0: 7375 6d6d 6172 792e 7265 706c 6163 6528  summary.replace(
+00012de0: 275c 5c75 272c 2755 2b27 290d 0a20 2020  '\\u','U+')..   
+00012df0: 7375 6d6d 6172 7920 3d20 7265 2e73 7562  summary = re.sub
+00012e00: 2872 273c 555c 2b28 5b30 2d39 612d 6641  (r'<U\+([0-9a-fA
+00012e10: 2d46 5d7b 342c 367d 293e 272c 206c 616d  -F]{4,6})>', lam
+00012e20: 6264 6120 783a 2063 6872 2869 6e74 2878  bda x: chr(int(x
+00012e30: 2e67 726f 7570 2831 292c 3136 2929 2c20  .group(1),16)), 
+00012e40: 7375 6d6d 6172 7929 0d0a 0d0a 2020 206b  summary)....   k
+00012e50: 6579 776f 7264 733d 6765 746b 6579 776f  eywords=getkeywo
+00012e60: 7264 7328 7375 6d6d 6172 792c 6d61 786b  rds(summary,maxk
+00012e70: 6579 776f 7264 7329 0d0a 0d0a 2020 2073  eywords)....   s
+00012e80: 756d 6d61 7279 776f 7264 7320 3d20 6c65  ummarywords = le
+00012e90: 6e28 7375 6d6d 6172 792e 7370 6c69 7428  n(summary.split(
+00012ea0: 2220 2229 290d 0a20 0d0a 2020 206d 6169  " ")).. ..   mai
+00012eb0: 6e6f 7574 3d6b 6579 776f 7264 7320 2b20  nout=keywords + 
+00012ec0: 222c 5c22 6f72 6967 696e 616c 776f 7264  ",\"originalword
+00012ed0: 636f 756e 745c 223a 2220 2b20 7374 7228  count\":" + str(
+00012ee0: 6f72 6967 696e 616c 776f 7264 7329 202b  originalwords) +
+00012ef0: 2022 2c5c 2273 756d 6d61 7279 776f 7264   ",\"summaryword
+00012f00: 636f 756e 745c 223a 222b 2073 7472 2873  count\":"+ str(s
+00012f10: 756d 6d61 7279 776f 7264 7329 202b 222c  ummarywords) +",
+00012f20: 5c22 6d61 696e 7375 6d6d 6172 795c 223a  \"mainsummary\":
+00012f30: 7b5c 2273 756d 6d61 7279 5c22 3a20 5c22  {\"summary\": \"
+00012f40: 2220 2b20 7375 6d6d 6172 7920 2b20 225c  " + summary + "\
+00012f50: 227d 7d22 0d0a 2020 2072 6574 7572 6e20  "}}"..   return 
+00012f60: 6d61 696e 6f75 740d 0a20 2020 0d0a 2323  mainout..   ..##
+00012f70: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+00012f80: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+00012f90: 2323 2323 2323 2323 2323 2323 2323 230d  ###############.
+00012fa0: 0a0d 0a66 726f 6d20 6c61 6e67 6368 6169  ...from langchai
+00012fb0: 6e2e 656d 6265 6464 696e 6773 2e6f 7065  n.embeddings.ope
+00012fc0: 6e61 6920 696d 706f 7274 204f 7065 6e41  nai import OpenA
+00012fd0: 4945 6d62 6564 6469 6e67 730d 0a66 726f  IEmbeddings..fro
+00012fe0: 6d20 6c61 6e67 6368 6169 6e2e 7465 7874  m langchain.text
+00012ff0: 5f73 706c 6974 7465 7220 696d 706f 7274  _splitter import
+00013000: 2043 6861 7261 6374 6572 5465 7874 5370   CharacterTextSp
+00013010: 6c69 7474 6572 0d0a 6672 6f6d 206c 616e  litter..from lan
+00013020: 6763 6861 696e 2e76 6563 746f 7273 746f  gchain.vectorsto
+00013030: 7265 732e 6661 6973 7320 696d 706f 7274  res.faiss import
+00013040: 2046 4149 5353 0d0a 0d0a 6672 6f6d 206c   FAISS....from l
+00013050: 616e 6763 6861 696e 2e63 6861 696e 732e  angchain.chains.
+00013060: 7175 6573 7469 6f6e 5f61 6e73 7765 7269  question_answeri
+00013070: 6e67 2069 6d70 6f72 7420 6c6f 6164 5f71  ng import load_q
+00013080: 615f 6368 6169 6e0d 0a66 726f 6d20 6c61  a_chain..from la
+00013090: 6e67 6368 6169 6e2e 6c6c 6d73 2069 6d70  ngchain.llms imp
+000130a0: 6f72 7420 5072 6f6d 7074 4c61 7965 724f  ort PromptLayerO
+000130b0: 7065 6e41 4943 6861 740d 0a66 726f 6d20  penAIChat..from 
+000130c0: 6c61 6e67 6368 6169 6e2e 6368 6174 5f6d  langchain.chat_m
+000130d0: 6f64 656c 7320 696d 706f 7274 2043 6861  odels import Cha
+000130e0: 744f 7065 6e41 490d 0a66 726f 6d20 6c61  tOpenAI..from la
+000130f0: 6e67 6368 6169 6e2e 6c6c 6d73 2069 6d70  ngchain.llms imp
+00013100: 6f72 7420 4f70 656e 4149 0d0a 696d 706f  ort OpenAI..impo
+00013110: 7274 2068 6173 686c 6962 0d0a 0d0a 2320  rt hashlib....# 
+00013120: 416e 7377 6572 2071 7565 7374 696f 6e73  Answer questions
+00013130: 2061 626f 7574 2074 6865 2068 6561 646c   about the headl
+00013140: 696e 6573 0d0a 6465 6620 7374 6172 745f  ines..def start_
+00013150: 636f 6e76 6572 7361 7469 6f6e 286f 7065  conversation(ope
+00013160: 6e61 696b 6579 2c71 7565 7279 2c74 6578  naikey,query,tex
+00013170: 742c 7465 6d70 6572 6174 7572 652c 6d6f  t,temperature,mo
+00013180: 6465 6c29 3a0d 0a20 2020 2023 2047 7261  del):..    # Gra
+00013190: 6220 7468 6520 696e 7075 7420 6672 6f6d  b the input from
+000131a0: 2074 6865 2041 5049 0d0a 2020 2020 2020   the API..      
+000131b0: 2020 2371 7565 7279 203d 2069 6e70 7574    #query = input
+000131c0: 735b 2271 7565 7279 220d 0a0d 0a0d 0a20  s["query"...... 
+000131d0: 2020 2020 2020 2074 6578 745f 7370 6c69         text_spli
+000131e0: 7474 6572 203d 2043 6861 7261 6374 6572  tter = Character
+000131f0: 5465 7874 5370 6c69 7474 6572 280d 0a20  TextSplitter(.. 
+00013200: 2020 2020 2020 2020 2020 2073 6570 6172             separ
+00013210: 6174 6f72 3d22 2022 2c0d 0a20 2020 2020  ator=" ",..     
+00013220: 2020 2020 2020 2063 6875 6e6b 5f73 697a         chunk_siz
+00013230: 653d 3130 3030 2c0d 0a20 2020 2020 2020  e=1000,..       
+00013240: 2020 2020 2063 6875 6e6b 5f6f 7665 726c       chunk_overl
+00013250: 6170 3d32 3030 2c0d 0a20 2020 2020 2020  ap=200,..       
+00013260: 2020 2020 206c 656e 6774 685f 6675 6e63       length_func
+00013270: 7469 6f6e 3d6c 656e 2c0d 0a20 2020 2020  tion=len,..     
+00013280: 2020 2029 0d0a 0d0a 2020 2020 2020 2020     )....        
+00013290: 7465 7874 7320 3d20 7465 7874 5f73 706c  texts = text_spl
+000132a0: 6974 7465 722e 7370 6c69 745f 7465 7874  itter.split_text
+000132b0: 2874 6578 7429 0d0a 2020 2020 2020 2020  (text)..        
+000132c0: 656d 6265 6464 696e 6773 203d 204f 7065  embeddings = Ope
+000132d0: 6e41 4945 6d62 6564 6469 6e67 7328 290d  nAIEmbeddings().
+000132e0: 0a20 2020 2020 2020 2064 6f63 7365 6172  .        docsear
+000132f0: 6368 203d 2046 4149 5353 2e66 726f 6d5f  ch = FAISS.from_
+00013300: 7465 7874 7328 7465 7874 732c 2065 6d62  texts(texts, emb
+00013310: 6564 6469 6e67 7329 0d0a 2020 2020 2020  eddings)..      
+00013320: 2020 646f 6373 203d 2064 6f63 7365 6172    docs = docsear
+00013330: 6368 2e73 696d 696c 6172 6974 795f 7365  ch.similarity_se
+00013340: 6172 6368 2871 7565 7279 290d 0a20 2020  arch(query)..   
+00013350: 2020 2020 200d 0a20 2020 2020 2020 2063       ..        c
+00013360: 6861 696e 203d 206c 6f61 645f 7161 5f63  hain = load_qa_c
+00013370: 6861 696e 284f 7065 6e41 4928 6d6f 6465  hain(OpenAI(mode
+00013380: 6c5f 6e61 6d65 3d6d 6f64 656c 2c20 7465  l_name=model, te
+00013390: 6d70 6572 6174 7572 653d 7465 6d70 6572  mperature=temper
+000133a0: 6174 7572 652c 6f70 656e 6169 5f61 7069  ature,openai_api
+000133b0: 5f6b 6579 3d6f 7065 6e61 696b 6579 292c  _key=openaikey),
+000133c0: 2063 6861 696e 5f74 7970 653d 2273 7475   chain_type="stu
+000133d0: 6666 2229 0d0a 2020 2020 2020 2020 7265  ff")..        re
+000133e0: 7320 3d20 6368 6169 6e28 7b22 696e 7075  s = chain({"inpu
+000133f0: 745f 646f 6375 6d65 6e74 7322 3a20 646f  t_documents": do
+00013400: 6373 2c20 2271 7565 7374 696f 6e22 3a20  cs, "question": 
+00013410: 7175 6572 797d 2c20 7265 7475 726e 5f6f  query}, return_o
+00013420: 6e6c 795f 6f75 7470 7574 733d 5472 7565  nly_outputs=True
+00013430: 290d 0a0d 0a20 2020 2020 2020 2023 7265  )....        #re
+00013440: 7475 726e 207b 2270 7265 6422 3a20 7265  turn {"pred": re
+00013450: 737d 0d0a 2020 2020 2020 2020 7265 7475  s}..        retu
+00013460: 726e 2072 6573 0d0a 0d0a                 rn res....
```

### Comparing `maadstml-3.29/maadstml/tmltextsummary.py` & `maadstml-3.30/maadstml/tmltextsummary.py`

 * *Files identical despite different names*

### Comparing `maadstml-3.29/maadstml.egg-info/PKG-INFO` & `maadstml-3.30/maadstml.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: maadstml
-Version: 3.29
+Version: 3.30
 Summary: Multi-Agent Accelerator for Data Science (MAADS): Transactional Machine Learning
 Home-page: https://github.com/smaurice101/transactionalmachinelearning
 Author: Sebastian Maurice
 Author-email: sebastian.maurice@otics.ca
 License: MIT License
 Keywords: multi-agent, transactional machine learning, data streams, data science, optimization, prescriptive analytics, machine learning, automl,auto-ml,artificial intelligence,predictive analytics,advanced analytics
 Description-Content-Type: text/markdown
@@ -12,15 +12,15 @@
 
 **Multi-Agent Accelerator for Data Science Using Transactional Machine Learning (MAADSTML)**
 
 *Revolutionizing Data Stream Science with Transactional Machine Learning*
 
 **Overview**
 
-*MAADSTML combines Artificial Intelligence, Auto Machine Learning with Data Streams Integrated with Apache Kafka (or Redpanda) to create frictionless and elastic machine learning solutions.*  
+*MAADSTML combines Artificial Intelligence, ChatGPT, Auto Machine Learning with Data Streams Integrated with Apache Kafka (or Redpanda) to create frictionless and elastic machine learning solutions.*  
 
 This library allows users to harness the power of agent-based computing using hundreds of advanced linear and non-linear algorithms. Users can easily integrate Predictive Analytics, Prescriptive Analytics, Pre-Processing, and Optimization in any data stream solution by wrapping additional code around the functions below. It connects with **Apache KAFKA brokers** for cloud based computing using Kafka (or Redpanda) as the data backbone. 
 
 If analysing MILLIONS of IoT devices, you can easily deploy thousands of VIPER/HPDE instances in Kubernetes Cluster in AWS/GCP/Azure. 
 
 It uses VIPER as a **KAFKA connector and seamlessly combines Auto Machine Learning, with Real-Time Machine Learning, Real-Time Optimization and Real-Time Predictions** while publishing these insights in to a Kafka cluster in real-time at scale, while allowing users to consume these insights from anywhere, anytime and in any format. 
 
@@ -244,14 +244,17 @@
 - **vipersearchanomaly**
   - Perform advanced analysis for user search.  This function is useful if you want to monitor what people are searching for, and determine
     if the searches are anamolous and differ from the peer group of "normal" search behaviour.
 
 - **vipernlp**
   - Perform advanced natural language summary of PDFs.
 
+- **viperchatgpt**
+  - Start a conversation with ChatGPT in real-time and stream responses.
+
 - **areyoubusy**
   - If deploying thousands of VIPER/HPDE binaries in a Kubernetes cluster - you can broadcast a 'areyoubusy' message to all VIPER and HPDE
     binaries, and they will return back the HOST/PORT if they are NOT busy with other tasks.  This is very convenient for dynamically managing  
 	enormous load among VIPER/HPDE and allows you to dynamically assign HOST/PORT to **non-busy** VIPER/HPDE microservices.
 
 **First import the Python library.**
 
@@ -4522,7 +4525,34 @@
 - Maximum amount of words in the summary.
 
 *maxkeywords* : int, required
 
 - Maximum amount of keywords to extract.
 
 RETURNS: JSON string of summary.
+
+**37. maadstml.viperchatgpt(openaikey,texttoanalyse,query, temperature,modelname)**
+
+**Parameters:**	Start a conversation with ChatGPT
+
+*openaikey* : string, required
+
+- OpenAI API key
+
+*texttoanalyse* : string, required
+       
+- Text you want ChatGPT to analyse
+
+*query* : string, required
+
+- Prompts for chatGPT.  For example, "What are key points in this text? What are the concerns or issues?"
+
+*temperature* : float, required
+
+- Temperature for chatgpt, must be between 0-1 i.e. 0.7
+
+*modelname* : string, required
+
+- ChatGPT model to use.  For example, text-davinci-002, text-curie-001, text-babbage-001.
+
+
+RETURNS: ChatGPT response.
```

### Comparing `maadstml-3.29/setup.py` & `maadstml-3.30/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 	
 
 with open("requirements.txt","r") as f:
     required = f.read().splitlines()
     
 setuptools.setup(
     name='maadstml',
-    version='3.29',
+    version='3.30',
     description='Multi-Agent Accelerator for Data Science (MAADS): Transactional Machine Learning',
     license='MIT License',
     packages=['maadstml'],
     author='Sebastian Maurice',
     author_email='sebastian.maurice@otics.ca',
     keywords=['multi-agent, transactional machine learning, data streams, data science, optimization, prescriptive analytics, machine learning, automl,auto-ml,artificial intelligence', 'predictive analytics', 'advanced analytics'],
     long_description=long_description,
```

