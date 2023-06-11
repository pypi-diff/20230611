# Comparing `tmp/NikChat-2.2.1.1.2.tar.gz` & `tmp/NikChat-2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "NikChat-2.2.1.1.2.tar", last modified: Wed Jun  7 03:40:49 2023, max compression
+gzip compressed data, was "NikChat-2.3.tar", last modified: Sun Jun 11 03:57:34 2023, max compression
```

## Comparing `NikChat-2.2.1.1.2.tar` & `NikChat-2.3.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-06-07 03:40:49.676564 NikChat-2.2.1.1.2/
--rw-rw-rw-   0        0        0     1094 2023-05-19 05:37:20.000000 NikChat-2.2.1.1.2/LICENSE
-drwxrwxrwx   0        0        0        0 2023-06-07 03:40:49.622655 NikChat-2.2.1.1.2/NikChat/
--rw-rw-rw-   0        0        0     3382 2023-06-07 03:39:55.000000 NikChat-2.2.1.1.2/NikChat/__init__.py
--rw-rw-rw-   0        0        0     4584 2023-06-05 02:13:44.000000 NikChat-2.2.1.1.2/NikChat/results.py
--rw-rw-rw-   0        0        0     2382 2023-06-06 01:06:27.000000 NikChat-2.2.1.1.2/NikChat/training.py
-drwxrwxrwx   0        0        0        0 2023-06-07 03:40:49.670029 NikChat-2.2.1.1.2/NikChat.egg-info/
--rw-rw-rw-   0        0        0     1682 2023-06-07 03:40:49.000000 NikChat-2.2.1.1.2/NikChat.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      225 2023-06-07 03:40:49.000000 NikChat-2.2.1.1.2/NikChat.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-07 03:40:49.000000 NikChat-2.2.1.1.2/NikChat.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2023-06-07 03:40:49.000000 NikChat-2.2.1.1.2/NikChat.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1682 2023-06-07 03:40:49.677547 NikChat-2.2.1.1.2/PKG-INFO
--rw-rw-rw-   0        0        0     1147 2023-05-24 05:16:40.000000 NikChat-2.2.1.1.2/README.md
--rw-rw-rw-   0        0        0      100 2023-05-21 16:11:11.000000 NikChat-2.2.1.1.2/pyproject.toml
--rw-rw-rw-   0        0        0      637 2023-06-07 03:40:49.681548 NikChat-2.2.1.1.2/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-06-11 03:57:34.023815 NikChat-2.3/
+-rw-rw-rw-   0        0        0     1094 2023-05-19 05:37:20.000000 NikChat-2.3/LICENSE
+drwxrwxrwx   0        0        0        0 2023-06-11 03:57:33.998300 NikChat-2.3/NikChat/
+-rw-rw-rw-   0        0        0     6650 2023-06-11 03:47:26.000000 NikChat-2.3/NikChat/__init__.py
+-rw-rw-rw-   0        0        0     4584 2023-06-05 02:13:44.000000 NikChat-2.3/NikChat/results.py
+-rw-rw-rw-   0        0        0     4356 2023-06-11 03:28:01.000000 NikChat-2.3/NikChat/training.py
+drwxrwxrwx   0        0        0        0 2023-06-11 03:57:34.020823 NikChat-2.3/NikChat.egg-info/
+-rw-rw-rw-   0        0        0     1676 2023-06-11 03:57:33.000000 NikChat-2.3/NikChat.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      225 2023-06-11 03:57:33.000000 NikChat-2.3/NikChat.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-11 03:57:33.000000 NikChat-2.3/NikChat.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2023-06-11 03:57:33.000000 NikChat-2.3/NikChat.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1676 2023-06-11 03:57:34.025848 NikChat-2.3/PKG-INFO
+-rw-rw-rw-   0        0        0     1147 2023-05-24 05:16:40.000000 NikChat-2.3/README.md
+-rw-rw-rw-   0        0        0      100 2023-05-21 16:11:11.000000 NikChat-2.3/pyproject.toml
+-rw-rw-rw-   0        0        0      631 2023-06-11 03:57:34.029861 NikChat-2.3/setup.cfg
```

### Comparing `NikChat-2.2.1.1.2/LICENSE` & `NikChat-2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `NikChat-2.2.1.1.2/NikChat/__init__.py` & `NikChat-2.3/NikChat/__init__.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-def NChat(input):
+def DChat(input):
     try:
         import nltk
         #nltk.download('punkt')
         #nltk.download('wordnet')
         import json
         import random
         import requests
@@ -12,14 +12,15 @@
         from tensorflow.keras.models import load_model
         from NikChat.results import ctime, weather, internet
         lemmatizer = WordNetLemmatizer()
         x = requests.get('https://api.jsonbin.io/v3/b/64698dac8e4aa6225ea0fcce')
         intents = json.loads(x.text)
         words = pickle.load(open('words.pkl', 'rb'))
         classes = pickle.load(open('classes.pkl', 'rb'))
+        json.dumps(intents, "training.json")
         model = load_model('Speechbot.h5')
         def clean_up_sentence(sentence):
             sentence_words = nltk.word_tokenize(sentence)
             sentence_words = [lemmatizer.lemmatize(word) for word in sentence_words]
             return sentence_words
         def bag_of_words(sentence):
             sentence_words = clean_up_sentence(sentence)
@@ -67,16 +68,92 @@
     except Exception as e:
         from os.path import exists
         if exists('words.pkl') == False:
             return 'Remember to use nikchat.init() before you use nikchat.NChat()'
         else:
             return e, " If your OS doesn't support automated downloads, please install the following libraries: nltk, numpy, tensorflow, wikipedia, bs4, geopy, geocoder"
         
+def train():
+    import NikChat.training as traning
+    traning.init2()
 
-def init():
+def init(filePath):
     from os.path import exists
     if exists('words.pkl') == False:
         import NikChat.training as traning
-        traning.init()
+        traning.init(filePath)
         return 'done'
     else:
         return 'done'
+
+def NChat(filePath):
+    try:
+        import nltk
+        #nltk.download('punkt')
+        #nltk.download('wordnet')
+        import json
+        import random
+        import requests
+        import pickle
+        import numpy as np
+        from nltk.stem import WordNetLemmatizer
+        from tensorflow.keras.models import load_model
+        from NikChat.results import ctime, weather, internet
+        lemmatizer = WordNetLemmatizer()
+        intents = json.loads(filePath)
+        words = pickle.load(open('words.pkl', 'rb'))
+        classes = pickle.load(open('classes.pkl', 'rb'))
+        json.dumps(intents, "training.json")
+        model = load_model('Speechbot.h5')
+        def clean_up_sentence(sentence):
+            sentence_words = nltk.word_tokenize(sentence)
+            sentence_words = [lemmatizer.lemmatize(word) for word in sentence_words]
+            return sentence_words
+        def bag_of_words(sentence):
+            sentence_words = clean_up_sentence(sentence)
+            bag = [0] * len(words)
+            for w in sentence_words:
+                for i, word in enumerate(words):
+                    if word == w:
+                        bag[i] = 1
+            return np.array(bag)
+        def predict_class(sentence):
+            bow = bag_of_words(sentence)
+            res = model.predict(np.array([bow]))[0]
+            ERROR_TRESHOLD = 0.25
+            results = [[i, r] for i, r in enumerate(res) if r > ERROR_TRESHOLD]
+            results.sort(key=lambda x: x[1], reverse=True)
+            return_list = []
+            for r in results:
+                return_list.append({'intent': classes[r[0]], 'probability': str(r[1])})
+            return return_list
+        def get_response(intents_list, intents_json):
+            tag = intents_list[0]['intent']
+            list_of_intents = intents_json['intents']
+            for i in list_of_intents:
+                if i['tag'] == tag:
+                    result = random.choice(i['responses'])
+                    break
+            return result
+        print('THE BOT IS RUNNING')
+        message = input
+        ints = predict_class(message)
+        res = get_response(ints, intents['record'])
+        str1 = ''
+        for elm in message.split(' '):
+            str1 += elm.lower() + " "
+        print(str1.split(' '))
+        if "weather" in str1.split(' ') or "temperature" in str1.split(' ') or "forecast" in str1.split(' '):
+            res = weather()
+        elif "day" in str1.split(' ') or "time" in str1.split(' ') or "date" in str1.split(' '):
+            res = ctime()
+        elif res == "bob is your dad":
+            res = internet(str1)
+        else:
+            res = res
+        return res
+    except Exception as e:
+        from os.path import exists
+        if exists('words.pkl') == False:
+            return 'Remember to use nikchat.init() before you use nikchat.NChat()'
+        else:
+            return e, " If your OS doesn't support automated downloads, please install the following libraries: nltk, numpy, tensorflow, wikipedia, bs4, geopy, geocoder"
```

### Comparing `NikChat-2.2.1.1.2/NikChat/results.py` & `NikChat-2.3/NikChat/results.py`

 * *Files identical despite different names*

### Comparing `NikChat-2.2.1.1.2/NikChat/training.py` & `NikChat-2.3/NikChat/training.py`

 * *Files 19% similar despite different names*

```diff
@@ -53,8 +53,55 @@
     model.add(Dense(64, activation='relu'))
     model.add(Dropout(0.5))
     model.add(Dense(len(train_y[0]), activation='softmax'))
     sgd = SGD(lr=0.01, decay=1e-6, momentum=0.9, nesterov=True)
     model.compile(loss="categorical_crossentropy", optimizer="sgd", metrics=['accuracy'])
     hist = model.fit(np.array(train_x), np.array(train_y), epochs=200, batch_size=5, verbose=1)
     model.save("Speechbot.h5", hist)
+    return
+
+def init2(filePath):
+    lemmatizer = WordNetLemmatizer()
+    intents = json.loads(str(filePath))
+    words = []
+    classes = []
+    documents = []
+    ignore_letters = ["?", "!", ".", ","]
+    for intent in intents['record']['intents']:
+        for pattern in intent['patterns']: 
+            word_list = nltk.word_tokenize(pattern)
+            words.extend(word_list)
+            documents.append((word_list, intent['tag']))
+            if intent['tag'] not in classes:
+                classes.append(intent['tag'])
+    words = [lemmatizer.lemmatize(word) for word in words if word not in ignore_letters]
+    words = sorted(set(words))
+    classes = sorted(set(classes))
+    pickle.dump(words, open('words.pkl', 'wb'))
+    pickle.dump(classes, open('classes.pkl', 'wb'))
+    training = []
+    output_empty = [0] * len(classes)
+    for document in documents:
+        bag = []
+        word_patterns = document[0]
+        word_patterns = [lemmatizer.lemmatize(word.lower()) for word in word_patterns]
+        for word in words:
+            bag.append(1) if word in word_patterns else bag.append(0)
+        output_row = list(output_empty)
+        output_row[classes.index(document[1])] = 1
+        training.append([bag, output_row])
+    random.shuffle(training)
+    training = np.array(training)
+    train_x = list(training[:, 0])
+    train_y = list(training[:, 1])
+
+    model = Sequential()
+    model.add(Dense(128, input_shape=(len(train_x[0]),), activation='relu'))
+    model.add(Dropout(0.5))
+    model.add(Dense(64, activation='relu'))
+    model.add(Dropout(0.5))
+    model.add(Dense(len(train_y[0]), activation='softmax'))
+    sgd = SGD(lr=0.01, decay=1e-6, momentum=0.9, nesterov=True)
+    model.compile(loss="categorical_crossentropy", optimizer="sgd", metrics=['accuracy'])
+    hist = model.fit(np.array(train_x), np.array(train_y), epochs=200, batch_size=5, verbose=1)
+    model.save("Speechbot.h5", hist)
     return
```

### Comparing `NikChat-2.2.1.1.2/NikChat.egg-info/PKG-INFO` & `NikChat-2.3/NikChat.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: NikChat
-Version: 2.2.1.1.2
+Version: 2.3
 Summary: A full-fledged chatbot designed to be incorperated into other projects. (Speeds of 0.1 seconds)
 Home-page: https://github.com/Nikhilodeon1/NikChat
 Author: Nikhil Tamvada (Nikhilodeon1)
 Author-email: nikhiltamvada@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `NikChat-2.2.1.1.2/PKG-INFO` & `NikChat-2.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: NikChat
-Version: 2.2.1.1.2
+Version: 2.3
 Summary: A full-fledged chatbot designed to be incorperated into other projects. (Speeds of 0.1 seconds)
 Home-page: https://github.com/Nikhilodeon1/NikChat
 Author: Nikhil Tamvada (Nikhilodeon1)
 Author-email: nikhiltamvada@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `NikChat-2.2.1.1.2/README.md` & `NikChat-2.3/README.md`

 * *Files identical despite different names*

### Comparing `NikChat-2.2.1.1.2/setup.cfg` & `NikChat-2.3/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,40 +1,40 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 204e 696b 4368 6174 0d0a 7665 7273   = NikChat..vers
-00000020: 696f 6e20 3d20 322e 322e 312e 312e 320d  ion = 2.2.1.1.2.
-00000030: 0a61 7574 686f 7220 3d20 4e69 6b68 696c  .author = Nikhil
-00000040: 2054 616d 7661 6461 2028 4e69 6b68 696c   Tamvada (Nikhil
-00000050: 6f64 656f 6e31 290d 0a61 7574 686f 725f  odeon1)..author_
-00000060: 656d 6169 6c20 3d20 6e69 6b68 696c 7461  email = nikhilta
-00000070: 6d76 6164 6140 676d 6169 6c2e 636f 6d0d  mvada@gmail.com.
-00000080: 0a64 6573 6372 6970 7469 6f6e 203d 2041  .description = A
-00000090: 2066 756c 6c2d 666c 6564 6765 6420 6368   full-fledged ch
-000000a0: 6174 626f 7420 6465 7369 676e 6564 2074  atbot designed t
-000000b0: 6f20 6265 2069 6e63 6f72 7065 7261 7465  o be incorperate
-000000c0: 6420 696e 746f 206f 7468 6572 2070 726f  d into other pro
-000000d0: 6a65 6374 732e 2028 5370 6565 6473 206f  jects. (Speeds o
-000000e0: 6620 302e 3120 7365 636f 6e64 7329 0d0a  f 0.1 seconds)..
-000000f0: 6c6f 6e67 5f64 6573 6372 6970 7469 6f6e  long_description
-00000100: 203d 2066 696c 653a 2052 4541 444d 452e   = file: README.
-00000110: 6d64 0d0a 6c6f 6e67 5f64 6573 6372 6970  md..long_descrip
-00000120: 7469 6f6e 5f63 6f6e 7465 6e74 5f74 7970  tion_content_typ
-00000130: 6520 3d20 7465 7874 2f6d 6172 6b64 6f77  e = text/markdow
-00000140: 6e0d 0a68 6f6d 655f 7061 6765 203d 2068  n..home_page = h
-00000150: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
-00000160: 6d2f 4e69 6b68 696c 6f64 656f 6e31 2f4e  m/Nikhilodeon1/N
-00000170: 696b 4368 6174 0d0a 636c 6173 7369 6669  ikChat..classifi
-00000180: 6572 7320 3d20 0d0a 0950 726f 6772 616d  ers = ...Program
-00000190: 6d69 6e67 204c 616e 6775 6167 6520 3a3a  ming Language ::
-000001a0: 2050 7974 686f 6e20 3a3a 2033 0d0a 094c   Python :: 3...L
-000001b0: 6963 656e 7365 203a 3a20 4f53 4920 4170  icense :: OSI Ap
-000001c0: 7072 6f76 6564 203a 3a20 4d49 5420 4c69  proved :: MIT Li
-000001d0: 6365 6e73 650d 0a09 4f70 6572 6174 696e  cense...Operatin
-000001e0: 6720 5379 7374 656d 203a 3a20 4f53 2049  g System :: OS I
-000001f0: 6e64 6570 656e 6465 6e74 0d0a 0d0a 5b6f  ndependent....[o
-00000200: 7074 696f 6e73 5d0d 0a70 6163 6b61 6765  ptions]..package
-00000210: 7320 3d20 6669 6e64 3a0d 0a70 7974 686f  s = find:..pytho
-00000220: 6e5f 7265 7175 6972 6573 203d 203e 3d33  n_requires = >=3
-00000230: 2e36 0d0a 696e 636c 7564 655f 7061 636b  .6..include_pack
-00000240: 6167 655f 6461 7461 203d 2054 7275 650d  age_data = True.
-00000250: 0a0d 0a5b 6567 675f 696e 666f 5d0d 0a74  ...[egg_info]..t
-00000260: 6167 5f62 7569 6c64 203d 200d 0a74 6167  ag_build = ..tag
-00000270: 5f64 6174 6520 3d20 300d 0a0d 0a         _date = 0....
+00000020: 696f 6e20 3d20 322e 330d 0a61 7574 686f  ion = 2.3..autho
+00000030: 7220 3d20 4e69 6b68 696c 2054 616d 7661  r = Nikhil Tamva
+00000040: 6461 2028 4e69 6b68 696c 6f64 656f 6e31  da (Nikhilodeon1
+00000050: 290d 0a61 7574 686f 725f 656d 6169 6c20  )..author_email 
+00000060: 3d20 6e69 6b68 696c 7461 6d76 6164 6140  = nikhiltamvada@
+00000070: 676d 6169 6c2e 636f 6d0d 0a64 6573 6372  gmail.com..descr
+00000080: 6970 7469 6f6e 203d 2041 2066 756c 6c2d  iption = A full-
+00000090: 666c 6564 6765 6420 6368 6174 626f 7420  fledged chatbot 
+000000a0: 6465 7369 676e 6564 2074 6f20 6265 2069  designed to be i
+000000b0: 6e63 6f72 7065 7261 7465 6420 696e 746f  ncorperated into
+000000c0: 206f 7468 6572 2070 726f 6a65 6374 732e   other projects.
+000000d0: 2028 5370 6565 6473 206f 6620 302e 3120   (Speeds of 0.1 
+000000e0: 7365 636f 6e64 7329 0d0a 6c6f 6e67 5f64  seconds)..long_d
+000000f0: 6573 6372 6970 7469 6f6e 203d 2066 696c  escription = fil
+00000100: 653a 2052 4541 444d 452e 6d64 0d0a 6c6f  e: README.md..lo
+00000110: 6e67 5f64 6573 6372 6970 7469 6f6e 5f63  ng_description_c
+00000120: 6f6e 7465 6e74 5f74 7970 6520 3d20 7465  ontent_type = te
+00000130: 7874 2f6d 6172 6b64 6f77 6e0d 0a68 6f6d  xt/markdown..hom
+00000140: 655f 7061 6765 203d 2068 7474 7073 3a2f  e_page = https:/
+00000150: 2f67 6974 6875 622e 636f 6d2f 4e69 6b68  /github.com/Nikh
+00000160: 696c 6f64 656f 6e31 2f4e 696b 4368 6174  ilodeon1/NikChat
+00000170: 0d0a 636c 6173 7369 6669 6572 7320 3d20  ..classifiers = 
+00000180: 0d0a 0950 726f 6772 616d 6d69 6e67 204c  ...Programming L
+00000190: 616e 6775 6167 6520 3a3a 2050 7974 686f  anguage :: Pytho
+000001a0: 6e20 3a3a 2033 0d0a 094c 6963 656e 7365  n :: 3...License
+000001b0: 203a 3a20 4f53 4920 4170 7072 6f76 6564   :: OSI Approved
+000001c0: 203a 3a20 4d49 5420 4c69 6365 6e73 650d   :: MIT License.
+000001d0: 0a09 4f70 6572 6174 696e 6720 5379 7374  ..Operating Syst
+000001e0: 656d 203a 3a20 4f53 2049 6e64 6570 656e  em :: OS Indepen
+000001f0: 6465 6e74 0d0a 0d0a 5b6f 7074 696f 6e73  dent....[options
+00000200: 5d0d 0a70 6163 6b61 6765 7320 3d20 6669  ]..packages = fi
+00000210: 6e64 3a0d 0a70 7974 686f 6e5f 7265 7175  nd:..python_requ
+00000220: 6972 6573 203d 203e 3d33 2e36 0d0a 696e  ires = >=3.6..in
+00000230: 636c 7564 655f 7061 636b 6167 655f 6461  clude_package_da
+00000240: 7461 203d 2054 7275 650d 0a0d 0a5b 6567  ta = True....[eg
+00000250: 675f 696e 666f 5d0d 0a74 6167 5f62 7569  g_info]..tag_bui
+00000260: 6c64 203d 200d 0a74 6167 5f64 6174 6520  ld = ..tag_date 
+00000270: 3d20 300d 0a0d 0a                        = 0....
```

