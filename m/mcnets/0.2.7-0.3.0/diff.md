# Comparing `tmp/mcnets-0.2.7.tar.gz` & `tmp/mcnets-0.3.0.tar.gz`

## Comparing `mcnets-0.2.7.tar` & `mcnets-0.3.0.tar`

### file list

```diff
@@ -1,35 +1,35 @@
--rw-r--r--   0        0        0     3767 2020-02-02 00:00:00.000000 mcnets-0.2.7/Tests Journal.txt
--rw-r--r--   0        0        0     5799 2020-02-02 00:00:00.000000 mcnets-0.2.7/Updates.txt
--rw-r--r--   0        0        0    17375 2020-02-02 00:00:00.000000 mcnets-0.2.7/GraphPicStuff/Fit 1 (default method, net as function).png
--rw-r--r--   0        0        0    11075 2020-02-02 00:00:00.000000 mcnets-0.2.7/GraphPicStuff/Fit 2 (net as derivative, holy cow!).png
--rw-r--r--   0        0        0    12638 2020-02-02 00:00:00.000000 mcnets-0.2.7/GraphPicStuff/Fit 3 (Another new attempt).png
--rw-r--r--   0        0        0    39485 2020-02-02 00:00:00.000000 mcnets-0.2.7/GraphPicStuff/Moar custom architecture tests.JPG
--rw-r--r--   0        0        0    45066 2020-02-02 00:00:00.000000 mcnets-0.2.7/GraphPicStuff/NN Speed vs Sizes (100x100, n=1).png
--rw-r--r--   0        0        0    11100 2020-02-02 00:00:00.000000 mcnets-0.2.7/GraphPicStuff/NN Speed vs Sizes (40x40, n=1).png
--rw-r--r--   0        0        0    14025 2020-02-02 00:00:00.000000 mcnets-0.2.7/GraphPicStuff/NN Speed vs Sizes (50x50 n=1).png
--rw-r--r--   0        0        0    12524 2020-02-02 00:00:00.000000 mcnets-0.2.7/GraphPicStuff/NN Speed vs Sizes (50x50 n=100).png
--rw-r--r--   0        0        0    12798 2020-02-02 00:00:00.000000 mcnets-0.2.7/GraphPicStuff/NN Speed vs Sizes (50x50 n=20).png
--rw-r--r--   0        0        0    43952 2020-02-02 00:00:00.000000 mcnets-0.2.7/GraphPicStuff/NN Speed vs Sizes (75x75, n=1).png
--rw-r--r--   0        0        0    53568 2020-02-02 00:00:00.000000 mcnets-0.2.7/GraphPicStuff/NN Speed vs Sizes with 6.5-8.5k parameter line (75x75, n=1).png
--rw-r--r--   0        0        0    51028 2020-02-02 00:00:00.000000 mcnets-0.2.7/GraphPicStuff/NN Speed vs Sizes with 9-11k parameter line (75x75, n=1).png
--rw-r--r--   0        0        0    34666 2020-02-02 00:00:00.000000 mcnets-0.2.7/GraphPicStuff/genTrain 1 (Holy cow i can do sin now!).png
--rw-r--r--   0        0        0    32480 2020-02-02 00:00:00.000000 mcnets-0.2.7/GraphPicStuff/genTrain 2 (sin pt.2 with a 50x15 ATAN net).png
--rw-r--r--   0        0        0    30412 2020-02-02 00:00:00.000000 mcnets-0.2.7/GraphPicStuff/genTrain 3 (20 points, R2 = 0.848).png
--rw-r--r--   0        0        0    16692 2020-02-02 00:00:00.000000 mcnets-0.2.7/GraphPicStuff/genTrain 4 (10 points, R2 = 0.998880, #params=44960, and use the true indicies!).png
--rw-r--r--   0        0        0    18779 2020-02-02 00:00:00.000000 mcnets-0.2.7/GraphPicStuff/genTrain 5 (10 points, R2 = 0.993114, #params=4920, and use the true indicies!).png
--rw-r--r--   0        0        0    17375 2020-02-02 00:00:00.000000 mcnets-0.2.7/GraphPicStuff/ghFit1.png
--rw-r--r--   0        0        0    15854 2020-02-02 00:00:00.000000 mcnets-0.2.7/GraphPicStuff/ghFit1a.png
--rw-r--r--   0        0        0    17039 2020-02-02 00:00:00.000000 mcnets-0.2.7/GraphPicStuff/ghFit1b.png
--rw-r--r--   0        0        0    12638 2020-02-02 00:00:00.000000 mcnets-0.2.7/GraphPicStuff/ghFit2.png
--rw-r--r--   0        0        0    13484 2020-02-02 00:00:00.000000 mcnets-0.2.7/GraphPicStuff/ghFit2b.png
--rw-r--r--   0        0        0    15211 2020-02-02 00:00:00.000000 mcnets-0.2.7/GraphPicStuff/ghSpeedTest1a.png
--rw-r--r--   0        0        0    39525 2020-02-02 00:00:00.000000 mcnets-0.2.7/src/mcnets/Feature Experiments.ipynb
--rw-r--r--   0        0        0    21238 2020-02-02 00:00:00.000000 mcnets-0.2.7/src/mcnets/Github Example.ipynb
--rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 mcnets-0.2.7/src/mcnets/__init__.py
--rw-r--r--   0        0        0    50092 2020-02-02 00:00:00.000000 mcnets-0.2.7/src/mcnets/main.py
--rw-r--r--   0        0        0    70272 2020-02-02 00:00:00.000000 mcnets-0.2.7/tests/Slope Fitting.ipynb
--rw-r--r--   0        0        0    74573 2020-02-02 00:00:00.000000 mcnets-0.2.7/tests/Speed Tests.ipynb
--rw-r--r--   0        0        0    35823 2020-02-02 00:00:00.000000 mcnets-0.2.7/LICENSE
--rw-r--r--   0        0        0     1533 2020-02-02 00:00:00.000000 mcnets-0.2.7/README.md
--rw-r--r--   0        0        0      688 2020-02-02 00:00:00.000000 mcnets-0.2.7/pyproject.toml
--rw-r--r--   0        0        0     2104 2020-02-02 00:00:00.000000 mcnets-0.2.7/PKG-INFO
+-rw-r--r--   0        0        0     3769 2020-02-02 00:00:00.000000 mcnets-0.3.0/Tests Journal.txt
+-rw-r--r--   0        0        0     7324 2020-02-02 00:00:00.000000 mcnets-0.3.0/Updates.txt
+-rw-r--r--   0        0        0    17375 2020-02-02 00:00:00.000000 mcnets-0.3.0/GraphPicStuff/Fit 1 (default method, net as function).png
+-rw-r--r--   0        0        0    11075 2020-02-02 00:00:00.000000 mcnets-0.3.0/GraphPicStuff/Fit 2 (net as derivative, holy cow!).png
+-rw-r--r--   0        0        0    12638 2020-02-02 00:00:00.000000 mcnets-0.3.0/GraphPicStuff/Fit 3 (Another new attempt).png
+-rw-r--r--   0        0        0    39485 2020-02-02 00:00:00.000000 mcnets-0.3.0/GraphPicStuff/Moar custom architecture tests.JPG
+-rw-r--r--   0        0        0    45066 2020-02-02 00:00:00.000000 mcnets-0.3.0/GraphPicStuff/NN Speed vs Sizes (100x100, n=1).png
+-rw-r--r--   0        0        0    11100 2020-02-02 00:00:00.000000 mcnets-0.3.0/GraphPicStuff/NN Speed vs Sizes (40x40, n=1).png
+-rw-r--r--   0        0        0    14025 2020-02-02 00:00:00.000000 mcnets-0.3.0/GraphPicStuff/NN Speed vs Sizes (50x50 n=1).png
+-rw-r--r--   0        0        0    12524 2020-02-02 00:00:00.000000 mcnets-0.3.0/GraphPicStuff/NN Speed vs Sizes (50x50 n=100).png
+-rw-r--r--   0        0        0    12798 2020-02-02 00:00:00.000000 mcnets-0.3.0/GraphPicStuff/NN Speed vs Sizes (50x50 n=20).png
+-rw-r--r--   0        0        0    43952 2020-02-02 00:00:00.000000 mcnets-0.3.0/GraphPicStuff/NN Speed vs Sizes (75x75, n=1).png
+-rw-r--r--   0        0        0    53568 2020-02-02 00:00:00.000000 mcnets-0.3.0/GraphPicStuff/NN Speed vs Sizes with 6.5-8.5k parameter line (75x75, n=1).png
+-rw-r--r--   0        0        0    51028 2020-02-02 00:00:00.000000 mcnets-0.3.0/GraphPicStuff/NN Speed vs Sizes with 9-11k parameter line (75x75, n=1).png
+-rw-r--r--   0        0        0    34666 2020-02-02 00:00:00.000000 mcnets-0.3.0/GraphPicStuff/genTrain 1 (Holy cow i can do sin now!).png
+-rw-r--r--   0        0        0    32480 2020-02-02 00:00:00.000000 mcnets-0.3.0/GraphPicStuff/genTrain 2 (sin pt.2 with a 50x15 ATAN net).png
+-rw-r--r--   0        0        0    30412 2020-02-02 00:00:00.000000 mcnets-0.3.0/GraphPicStuff/genTrain 3 (20 points, R2 = 0.848).png
+-rw-r--r--   0        0        0    16692 2020-02-02 00:00:00.000000 mcnets-0.3.0/GraphPicStuff/genTrain 4 (10 points, R2 = 0.998880, #params=44960, and use the true indicies!).png
+-rw-r--r--   0        0        0    18779 2020-02-02 00:00:00.000000 mcnets-0.3.0/GraphPicStuff/genTrain 5 (10 points, R2 = 0.993114, #params=4920, and use the true indicies!).png
+-rw-r--r--   0        0        0    17375 2020-02-02 00:00:00.000000 mcnets-0.3.0/GraphPicStuff/ghFit1.png
+-rw-r--r--   0        0        0    15854 2020-02-02 00:00:00.000000 mcnets-0.3.0/GraphPicStuff/ghFit1a.png
+-rw-r--r--   0        0        0    17039 2020-02-02 00:00:00.000000 mcnets-0.3.0/GraphPicStuff/ghFit1b.png
+-rw-r--r--   0        0        0    12638 2020-02-02 00:00:00.000000 mcnets-0.3.0/GraphPicStuff/ghFit2.png
+-rw-r--r--   0        0        0    13484 2020-02-02 00:00:00.000000 mcnets-0.3.0/GraphPicStuff/ghFit2b.png
+-rw-r--r--   0        0        0    15211 2020-02-02 00:00:00.000000 mcnets-0.3.0/GraphPicStuff/ghSpeedTest1a.png
+-rw-r--r--   0        0        0    64569 2020-02-02 00:00:00.000000 mcnets-0.3.0/src/mcnets/Feature Experiments.ipynb
+-rw-r--r--   0        0        0    21238 2020-02-02 00:00:00.000000 mcnets-0.3.0/src/mcnets/Github Example.ipynb
+-rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 mcnets-0.3.0/src/mcnets/__init__.py
+-rw-r--r--   0        0        0    54298 2020-02-02 00:00:00.000000 mcnets-0.3.0/src/mcnets/main.py
+-rw-r--r--   0        0        0    70272 2020-02-02 00:00:00.000000 mcnets-0.3.0/tests/Slope Fitting.ipynb
+-rw-r--r--   0        0        0    74573 2020-02-02 00:00:00.000000 mcnets-0.3.0/tests/Speed Tests.ipynb
+-rw-r--r--   0        0        0    35823 2020-02-02 00:00:00.000000 mcnets-0.3.0/LICENSE
+-rw-r--r--   0        0        0     1533 2020-02-02 00:00:00.000000 mcnets-0.3.0/README.md
+-rw-r--r--   0        0        0      688 2020-02-02 00:00:00.000000 mcnets-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0     2104 2020-02-02 00:00:00.000000 mcnets-0.3.0/PKG-INFO
```

### Comparing `mcnets-0.2.7/Tests Journal.txt` & `mcnets-0.3.0/Tests Journal.txt`

 * *Files 6% similar despite different names*

```diff
@@ -45,15 +45,15 @@
 - Time
   - At worst, the SEM methods are equal to the normal .Calculate method
   - Above 5-ish calculations, the SEM methods are notably faster
 - Overall
   - Not worth implementing in this way
 
 
-<Net Functionalities Tests>
+<Biases & Error Metric Tests>
 - Biases
 	- Single vector
 		- Applied to all hidden layers
 			- Just created a very off center line
 		- Applied to input layer
 			- Kinda did something, still worse behavior
 	- Bias collection
```

### Comparing `mcnets-0.2.7/Updates.txt` & `mcnets-0.3.0/Updates.txt`

 * *Files 14% similar despite different names*

```diff
@@ -3,29 +3,61 @@
 	- Test 'derivative' functionallity
 - Add a 'draw net' feature that plots a diagram of the net in pyplot
 	- Normal (line) diagram
 	- Heatmap visual of weights
 - Extend net feature
 	- Add a hidden layer
 		- Train og net, add random layer, then just train that layer
-- Update saving/loading nets to be done in a folder named 'mcnets'
 - Add MicroTweak to change only a few parameters at a time
 - Speed up net calculation for nets with many layers
 - 3D net weight arrays? (I cant see why this would be an improvement)
 - Backwards propogation? (Train net from x -> y; can the weights be reversed to go y -> x?)
 - Languange processing
 	- Letters to slope (for a sorta 'sentiment' value)
 	- Given a question, have an output for yes/no
 - Add intelligent data thinning function (takes points where slope changes)
-- Add test/train split that keeps ordering
 - Add monte-carlo tree search as another advanced training method (might not be worth it?)
 	- Like genTrain, but continues testing a few routes for more than one depth
 - Do test on all acti function combinations for curve fitting test (sin(x+4) - (x^2/10) + x) xE[0,11]
-- Fix training with biases included in .Calculate()
-- Add "Calculation Time" to model __str__ stuff
+- Do speed test comparison of various net sizes between .Calculate and .fastCalc
+
+
+V0.3.0 (AFs and Calculate stuff)
+- Renamed self.calcTime to self.speed
+- Added RESU activation function (has R2 ~= 0.9 for y = x^0.5, x^2 & sin(x))
+	- Currently experimental
+	- Using both (-) and (+) ends currently
+		- Unlike RELU which is just (+) end
+- Added RESU2
+	- Similar peice-wise behavior to RELU, just with RESU calc instead
+- Added RESU and RESU2 to __init__ description
+- Renamed "NONE" to "LIN"
+- Added lower-case/other handling for __init__ and applyActi() for activation function name
+- Added useFast option to genTrain, netMetrics and forecast
+
+
+V0.2.8 (Misc. Features)
+- Moved activation function application to a function applyActi()
+	- .Calculate now uses this
+- Added calcTime as a net property
+	- Is printed out along with other __str__ stuffs
+	- iterations is 2 (I=2) for this calculation
+- Updated .Calculate() inVector shape/misc. checking
+	- Removed try/except around the rowtest in .Calculate
+		> this shouldn't be needed as a vector type check happens just before
+	- Removed try/except around checking for ndarray type (replaced with type() if statement)
+	- Added ValueError(f"Expected inVector of size {(self.inSize, 1)} or {(1, self.inSize)}, got {(np.size(inVector, axis=0), np.size(inVector, axis=1))})")
+	> Could just do try/except when doing matrix multiplication, but current way give more info for errors
+	- Now checks for correct vector shape explicitly
+- Added fastCalc
+	- Takes 40-70% of the time compared to .Calculate
+	- Skips most handling checks in favor of speed
+	- Still supports single float inputs/outputs
+- Added fastCalc as option to .Calculate()
+
 
 
 V0.2.7 (Hotfix)
 - File loading error
 	- Happened when creating a "linear regression" net (ie hiddenSize = [])
 	- FIX: Added "ndmin=1" to np.loadtxt() for loading the activations
 		- This should not be neccessary to add for the loading of
@@ -33,14 +65,15 @@
 		  2 entries, and the loaded weights are not iterated over
 
 
 V0.2.6 (Hotfix)
 - Still encountering file errors
 	- Removed the "./" infront of the paths when saving/loading
 	- Commented out "name = str(name)" in LoadNet and SaveNN
+	- These didn't fix it
 
 
 V0.2.5 (Stupidity Fix)
 - Deleted old_versions from local area
 	- Was creating an exponential file size increase whoops
 	- Just retrieve old versions from PyPI if for some reason needed
```

### Comparing `mcnets-0.2.7/GraphPicStuff/Fit 1 (default method, net as function).png` & `mcnets-0.3.0/GraphPicStuff/Fit 1 (default method, net as function).png`

 * *Files identical despite different names*

### Comparing `mcnets-0.2.7/GraphPicStuff/Fit 2 (net as derivative, holy cow!).png` & `mcnets-0.3.0/GraphPicStuff/Fit 2 (net as derivative, holy cow!).png`

 * *Files identical despite different names*

### Comparing `mcnets-0.2.7/GraphPicStuff/Fit 3 (Another new attempt).png` & `mcnets-0.3.0/GraphPicStuff/Fit 3 (Another new attempt).png`

 * *Files identical despite different names*

### Comparing `mcnets-0.2.7/GraphPicStuff/Moar custom architecture tests.JPG` & `mcnets-0.3.0/GraphPicStuff/Moar custom architecture tests.JPG`

 * *Files identical despite different names*

### Comparing `mcnets-0.2.7/GraphPicStuff/NN Speed vs Sizes (100x100, n=1).png` & `mcnets-0.3.0/GraphPicStuff/NN Speed vs Sizes (100x100, n=1).png`

 * *Files identical despite different names*

### Comparing `mcnets-0.2.7/GraphPicStuff/NN Speed vs Sizes (40x40, n=1).png` & `mcnets-0.3.0/GraphPicStuff/NN Speed vs Sizes (40x40, n=1).png`

 * *Files identical despite different names*

### Comparing `mcnets-0.2.7/GraphPicStuff/NN Speed vs Sizes (50x50 n=1).png` & `mcnets-0.3.0/GraphPicStuff/NN Speed vs Sizes (50x50 n=1).png`

 * *Files identical despite different names*

### Comparing `mcnets-0.2.7/GraphPicStuff/NN Speed vs Sizes (50x50 n=100).png` & `mcnets-0.3.0/GraphPicStuff/NN Speed vs Sizes (50x50 n=100).png`

 * *Files identical despite different names*

### Comparing `mcnets-0.2.7/GraphPicStuff/NN Speed vs Sizes (50x50 n=20).png` & `mcnets-0.3.0/GraphPicStuff/NN Speed vs Sizes (50x50 n=20).png`

 * *Files identical despite different names*

### Comparing `mcnets-0.2.7/GraphPicStuff/NN Speed vs Sizes (75x75, n=1).png` & `mcnets-0.3.0/GraphPicStuff/NN Speed vs Sizes (75x75, n=1).png`

 * *Files identical despite different names*

### Comparing `mcnets-0.2.7/GraphPicStuff/NN Speed vs Sizes with 6.5-8.5k parameter line (75x75, n=1).png` & `mcnets-0.3.0/GraphPicStuff/NN Speed vs Sizes with 6.5-8.5k parameter line (75x75, n=1).png`

 * *Files identical despite different names*

### Comparing `mcnets-0.2.7/GraphPicStuff/NN Speed vs Sizes with 9-11k parameter line (75x75, n=1).png` & `mcnets-0.3.0/GraphPicStuff/NN Speed vs Sizes with 9-11k parameter line (75x75, n=1).png`

 * *Files identical despite different names*

### Comparing `mcnets-0.2.7/GraphPicStuff/genTrain 1 (Holy cow i can do sin now!).png` & `mcnets-0.3.0/GraphPicStuff/genTrain 1 (Holy cow i can do sin now!).png`

 * *Files identical despite different names*

### Comparing `mcnets-0.2.7/GraphPicStuff/genTrain 2 (sin pt.2 with a 50x15 ATAN net).png` & `mcnets-0.3.0/GraphPicStuff/genTrain 2 (sin pt.2 with a 50x15 ATAN net).png`

 * *Files identical despite different names*

### Comparing `mcnets-0.2.7/GraphPicStuff/genTrain 3 (20 points, R2 = 0.848).png` & `mcnets-0.3.0/GraphPicStuff/genTrain 3 (20 points, R2 = 0.848).png`

 * *Files identical despite different names*

### Comparing `mcnets-0.2.7/GraphPicStuff/genTrain 4 (10 points, R2 = 0.998880, #params=44960, and use the true indicies!).png` & `mcnets-0.3.0/GraphPicStuff/genTrain 4 (10 points, R2 = 0.998880, #params=44960, and use the true indicies!).png`

 * *Files identical despite different names*

### Comparing `mcnets-0.2.7/GraphPicStuff/genTrain 5 (10 points, R2 = 0.993114, #params=4920, and use the true indicies!).png` & `mcnets-0.3.0/GraphPicStuff/genTrain 5 (10 points, R2 = 0.993114, #params=4920, and use the true indicies!).png`

 * *Files identical despite different names*

### Comparing `mcnets-0.2.7/GraphPicStuff/ghFit1.png` & `mcnets-0.3.0/GraphPicStuff/ghFit1.png`

 * *Files identical despite different names*

### Comparing `mcnets-0.2.7/GraphPicStuff/ghFit1a.png` & `mcnets-0.3.0/GraphPicStuff/ghFit1a.png`

 * *Files identical despite different names*

### Comparing `mcnets-0.2.7/GraphPicStuff/ghFit1b.png` & `mcnets-0.3.0/GraphPicStuff/ghFit1b.png`

 * *Files identical despite different names*

### Comparing `mcnets-0.2.7/GraphPicStuff/ghFit2.png` & `mcnets-0.3.0/GraphPicStuff/ghFit2.png`

 * *Files identical despite different names*

### Comparing `mcnets-0.2.7/GraphPicStuff/ghFit2b.png` & `mcnets-0.3.0/GraphPicStuff/ghFit2b.png`

 * *Files identical despite different names*

### Comparing `mcnets-0.2.7/GraphPicStuff/ghSpeedTest1a.png` & `mcnets-0.3.0/GraphPicStuff/ghSpeedTest1a.png`

 * *Files identical despite different names*

### Comparing `mcnets-0.2.7/src/mcnets/Github Example.ipynb` & `mcnets-0.3.0/src/mcnets/Github Example.ipynb`

 * *Files identical despite different names*

### Comparing `mcnets-0.2.7/src/mcnets/main.py` & `mcnets-0.3.0/src/mcnets/main.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 from matplotlib import pyplot as plt
 import numpy as np
 import textwrap as txt
 import os
+from time import perf_counter as pc
 
 class AdvNet:
     ## Default Functions ## 
     def __init__(self, inputCount: int, hiddenCounts: list, outputCount: int, activations):
         """
         Create a deep neural network from the given counts of neurons requested per layer.
 
@@ -20,20 +21,22 @@
         - Range == (0, inf]
 
         3 - outputCount
         - Type == int
         - Range == (0, inf]
 
         4 - activations
-        - Possible Values: "NONE", "ELU", "ATAN", "RELU", "SIG"
-            - NONE: No applied function
+        - Possible Values: "lin", "elu", "atan", "relu", "sig", "resu", "resu2"
+            - LIN: No applied function (linear)
             - ELU: Exponential up to x=0, then uses y=x
             - ATAN: Uses arctan(x)
             - RELU: max(x, 0)
             - SIG: Sigmoid function
+            - RESU: Experimental, applies |sin(x)|*x
+            - RESU2: Experimental, applies max(|sin(x)|*x, 0)
         - A list of different functions per layer can be given, otherwise, all calculation
           steps will use the single given activation function.
         - Examples:
             - AdvNet(1, [10, 20, 10], 2, "RELU") 
                 - 5-layer net / 4 in-between spaces
                 - Uses the "RELU" activation function for all (4) in-between spaces.
             - AdvNet(2, [15, 15], 5, ["RELU", "ELU", "ATAN"]) 
@@ -91,42 +94,59 @@
             LW = len(self.weights)
             if LA == LW:
                 self.activationFunction = activations
             elif LA < LW:
                 raise ValueError(f"Not enough activation functions provided! ({LA} given, {LW} required)")
             elif LA > LW:
                 raise ValueError(f"Too many activation functions provided! ({LA} given, {LW} required)")
+            
+        # Force upper case for activation functions
+        # (allows giving them as lower case/whatever when constructed)
+        self.activationFunction = [i.upper() for i in self.activationFunction]
+            
+        # Test Calculation Time (for __str__)
+        I = 2 # Do just 2 iterations
+        t1 = pc()
+        for i in range(I):
+            self.Calculate(np.ones((self.inSize, 1)))
+        t2 = pc()
+        self.speed = format((t2-t1)/I, ".2e")
 
     def __str__(self):
-        # String Forming and formating
+        # Resulting string dimensions/title
         strlen = 64
         l1 = f"="
         l2 = f"Neural Net Characteristics:"
 
+        # Show the layer heights of the net
         l3 = f"1. Layer Sizes = {self.sizes}"
         l3 = txt.fill(l3, strlen-2)
 
+        # Get and show the medians weight values within the weight arrays
         weightMedians = []
         for weights in self.weights:
             weightMedians.append(round(np.median(weights), 2))
         l4 = f"2. Weight Medians = {weightMedians}"
         l4 = txt.fill(l4, strlen-2)
 
+        # Show the number of paramaters that make up the net
         l6 = f"3. Number of Parameters: {self.parameters}"
 
+        # Show activation functions and order
         l7a = f"4. Activation Functions: {self.activationFunction}"
         l7a = txt.fill(l7a, strlen-2)
-
-        # l7b = f"{self.activationFunction}"
-        l5 = f"="
+        
+        # Show the calculation time
+        l8 = f"5. Calculation Time: ~{self.speed}"
+        l8 = txt.fill(l8, strlen-2)
 
         # Resulting String
         full = (l1*strlen + '\n' + l2.center(strlen, ' ') + '\n' + l3 + 
                 '\n' + l4 + '\n' + l6 + '\n' + 
-                l7a + '\n' + l5*strlen)
+                l7a + '\n' + l8 + '\n' + l1*strlen)
         return full
 
     ## Internal Functions ##
     def TweakWeights(self, Amplitude: float, Selection='all', returnChange:bool = False):
         """
         Adjust the weights of a neural net by a given amplitude. The net change in the 
         weight arrays can be optionally returned for gradient decent calculation later.
@@ -208,103 +228,108 @@
             dW = [(self.weights[i] - Wo[i]) for i in range(len(self.weights))]
             return dW
 
         # # Adjust the bias values
         # for i in range(len(self.biases)):
         #     self.biases[i] = np.clip(self.biases[i] + 2*Amplitude*(np.random.rand(self.biases[i].size, 1) - 0.5), -5, 5)
 
-    def Calculate(self, inVector):
+    def Calculate(self, inVector, useFast:bool = False):
         """
         Returns the neural net's calculation for a given input vector. If the net used has an input size
         of one, a single float value can be given (array type not required).
 
         Inputs:
 
         1 - inVector
         - Type == NumPy Array
         - Size == (netInputCount, 1) or (1, netInputCount)
         - Note: 
             - If the net input size is 1, then a float can be given and a vector form is not required.
+
+        2 - useFast
+        - Type == Bool
+        - Usage:
+            - Determines whether or not fastCalc is used over Calculate. This can bring the
+              calculation speed down to around 40-70% of the otherwise default calculation
+              time, but minimal checks of the given data are done.
+            - If you are sure the given inVector data is correct, then you can use this
+              fast-calc setting, otherwise use caution as you will not receive useful 
+              information about what might go wrong during the calculation.
         """  
+        # Apply fast calculation mode if requested
+        if useFast:
+            return fastCalc(self, inVector)
 
         # Handling if a single number/float was given not in an array form
-        try:
-            # Test if a vector form was given
-            test = inVector.size
-        except:
-            # Not a vector -- check that net input size is one to confirm a single value works
+        if type(inVector) != np.ndarray:
             if self.inSize == 1:
                 inVector = np.array(inVector).reshape(1, 1)
             else:
-                raise ValueError(f"Net input size of 1 expected, got {self.inSize} instead. It's also possible the inVector is simply not a numpy array/vector")
+                raise ValueError(f"Net input size of 1 expected, got {self.inSize} instead")
             
+        # Check for correct shape (x, 1) or (1, x)
+        m1 = np.size(inVector, axis=0)
+        m2 = np.size(inVector, axis=1)
+        if m1*m2 == m1 or m1*m2 == m2:
+            # One of the dimensions is one, so the input is indeed a vector
+            pass
+        else:
+            # The input is not a vector but instead an array/matrix
+            raise ValueError(f"Expected inVector of size {(self.inSize, 1)} or {(1, self.inSize)}, got {(np.size(inVector, axis=0), np.size(inVector, axis=1))})")
+
         # Handling for row vectors (convert to column vectors)
         passedRowTest = False
-        try:
-            # If all entries are oriented along the horizontal axis
-            if inVector.size == np.size(inVector, 1):
-                # Convert row vectors to column vectors
-                if self.inSize != 1:
-                    if inVector.size == np.size(inVector, 1):
-                        inVector = inVector.T
-                        passedRowTest = True
-        except:
+        if inVector.size == np.size(inVector, axis=0): # Check if already correct form
             passedRowTest = True
-            pass
+        elif inVector.size == np.size(inVector, axis=1): # If all entries are oriented along the horizontal axis
+            # Convert row vectors to column vectors
+            if self.inSize != 1:
+                if inVector.size == np.size(inVector, 1):
+                    inVector = inVector.T
+                    passedRowTest = True
+            else:
+                # Just a single value so continue
+                passedRowTest = True
         
-        # Check if the input vector is indeed a column vector
-        if inVector.size == np.size(inVector, 0) and passedRowTest:
+        # Calculate if the input vector is indeed a column vector
+        if inVector.size == np.size(inVector, axis=0) and passedRowTest:
             # Vector has the right column vector shape -- now check for correct size
             if inVector.size == self.inSize:
                 # Vector is of the right shape and size so continue
 
                 # Go through all of weights calculating the next vector
-                ## in vector, w1 vec, w2 vec, ... out vec
                 calcVec = inVector # Start the calcVector with the given input vector
                 
                 # Triple-checking size throughout forward prop.
                 calcVec = calcVec.reshape(calcVec.size, 1)
 
                 for i, weights in enumerate(self.weights):
                     # Forward propogation
                     calcVec = sum(calcVec*weights)
 
                     # Use the net's activation function for the current space
                     hiddenFunction = self.activationFunction[i]
 
                     # Apply the activation function
-                    if hiddenFunction == 'NONE':
-                        pass
-                    elif hiddenFunction == 'ELU':
-                        calcVec = 0.4 * (2.7182818284**calcVec - 1)
-                    elif hiddenFunction == 'ATAN':
-                        calcVec = np.arctan(calcVec)
-                    elif hiddenFunction == 'RELU':
-                        calcVec[calcVec < 0] = 0
-                    elif hiddenFunction == 'SIG':
-                        e_p = 2.7182818284**calcVec
-                        e_n = 2.7182818284**(-calcVec)
-                        calcVec = ((e_p - e_n) / (e_p + e_n)) + 1
-                    elif hiddenFunction == 'EXP':
-                        calcVec[calcVec < -0.4] = 0
-                    else:
-                        raise ValueError("Given hidden function is not of the avalible types!")
+                    calcVec = applyActi(calcVec, hiddenFunction)
 
                     # Triple-checking size throughout forward prop.
                     calcVec = calcVec.reshape(calcVec.size, 1)
 
                 # Handling for single-number outputs (free it from the array at the end)
                 if self.outSize == 1:
                     calcVec = calcVec[0][0]
 
                 return calcVec
             
             # Vector is not of the correct shape for the used neural net
             else:
                 raise ValueError(f"inVector size ({inVector.size}) does not match the net input size ({self.inSize})")
+        else:
+            raise RuntimeError("Failed to enter Calculation loop! (This shouldn't have happened)")
 
     def CopyNet(self):
         """
         Copy a neural net object to a new variable. Used in similar
         situations as NumPy's copy method to make an isolated net
         with the same values and properties as the parent net.
 
@@ -366,15 +391,15 @@
                     # time delay.
                     continue
         
         # Convert activation data from list to numerical array
         data = []
         for function in self.activationFunction:
             # Conversions
-            if function == "NONE":
+            if function == "LIN":
                 data.append(0)
             elif function == "RELU":
                 data.append(1)
             elif function == "ELU":
                 data.append(2)
             elif function == "ATAN":
                 data.append(3)
@@ -389,15 +414,15 @@
             except:
                 continue
 
     def ApplyTweak(self, dW):
         for i, dWi in enumerate(dW):
             self.weights[i] = self.weights[i] + dWi
 
-## External Functions ##
+## External Net Functions ##
 def LoadNet(name:str):
     """
     Returns a nerual net object with the loaded characteristics from the
     given nickname. 
     
     Inputs:
 
@@ -436,23 +461,23 @@
             continue
 
     # Convert to str activation data
     strActivations = []
     for function in activations:
         # Conversions
         if function == 0:
-            strActivations.append("NONE")
+            strActivations.append("LIN")
         elif function == 1:
             strActivations.append("RELU")
         elif function == 2:
             strActivations.append("ELU")
         elif function == 3:
             strActivations.append("ATAN")
         else:
-            strActivations.append("NONE")
+            strActivations.append("LIN")
 
     # From the size, construct the net frame
     net = AdvNet(inSize, hiddenSize, outSize, strActivations)
 
     # Load in the saved net weights
     for i in range(len(net.sizes) - 1):
         for _ in range(10): ## Redundant loading loop, reference SaveNN on 'onedrive issue'
@@ -463,15 +488,15 @@
                 continue
         weights = weights.reshape(net.sizes[i], net.sizes[i+1])
         net.weights[i] = weights
 
     # Return the generated neural net
     return net
 
-def Forecast(Net, inputData, comparisonData=[], plotResults=True):
+def Forecast(Net, inputData, comparisonData=[], plotResults=True, useFast:bool=False):
     """
     Test a net against a series of input values to get its current predictions which
     is then returned. Additionally, the predictions are plotted (by default) along
     with the comparison / validation data if provided.
 
     Inputs:
 
@@ -546,15 +571,15 @@
         # Generate net input vector
         if inSize > 1:
             invec = np.array(xData[i]).reshape(1,inSize)
         else:
             invec = np.array(xData[i]).reshape(1,1)
 
         # Get net prediciton
-        val = net.Calculate(invec)
+        val = net.Calculate(invec, useFast=useFast)
         predictions.append(val)
 
         # Add first type of net output to plot for later
         if plotResults:
             try:
                 forPlot.append(val[0])
             except:
@@ -633,25 +658,26 @@
     net.hiddenSize = [i+d_height for i in net.hiddenSize]
     net.sizes[1:-1] = net.hiddenSize
     net.parameters = sum([M.size for M in net.weights])
 
     # Finish
     return net
 
-def netMetrics(net:AdvNet, xArr:np.ndarray, yArr:np.ndarray, returnAll:bool = False, method:str = 'r2'):
+def netMetrics(net:AdvNet, xArr:np.ndarray, yArr:np.ndarray, returnAll:bool = False, 
+               method:str = 'r2', useFast:bool = False):
     """
     Returns the nets R^2 value for the given x input data and y validation data.
 
     returnAll:
         - If True, all errors are returned in the order of (R^2, ResidualError, RegressionError, TotalError).
           Otherwise, just the R^2 value is returned.
     """
 
     # Get predictions
-    yHatList = Forecast(net, xArr, plotResults=False)
+    yHatList = Forecast(net, xArr, plotResults=False, useFast=useFast)
     # try:
     #     sizeY = np.size(yArr, axis=1)
     # except:
     #     sizeY = 1
     # sizeX = np.size(yArr, axis=0)
 
     ## R^2 Method ##
@@ -673,15 +699,15 @@
             return SSreg / SStot, SSres, SSreg, SStot
         
     elif method == 'sse':
         return 1 / sum(abs(np.array(yHatList).T - yArr))
 
 def genTrain(net:AdvNet, xArr:np.ndarray, yArr:np.ndarray, iterations:int = 1000, 
                     batchSize:int = 0, gamma:int = 50, weightSelection:str = None, 
-                    R2Goal = 0.999, Silent:bool = False):
+                    R2Goal = 0.999, Silent:bool = False, useFast:bool = False):
     """
     Returns a net and its R^2 value relative to the given X and Y data.
     
     Instead of always using the first net that has any improvement from the previous best net,
     a 'batch' of nets are generated from the parent net, then tested to find the best of those.
 
     Net:
@@ -721,15 +747,15 @@
     if type(net) == AdvNet and type(xArr) == np.ndarray and type(yArr) == np.ndarray:
         # print("All data is good")
         pass
     else:
         print("A data type is not correct")
 
     # Get inital accuracy
-    currentR2 = netMetrics(net, xArr, yArr)
+    currentR2 = netMetrics(net, xArr, yArr, useFast=useFast)
 
     # Generational Training method
     for I in range(iterations):
         # Get current tweak amplitude
         twk = 2 ** (-I / gamma)        ## ~30-60 seems to be a good scale for this (found via Train())
 
         # exp. weight selection
@@ -752,15 +778,15 @@
             newNet = net.CopyNet()
             newNet.TweakWeights(twk, Selection=weightSelection)
             testNets.append(newNet)
 
         # Get the offspring's scores
         newNetScores = []
         for mutNet in testNets:
-            newR2 = netMetrics(mutNet, xArr, yArr)
+            newR2 = netMetrics(mutNet, xArr, yArr, useFast=useFast)
             newNetScores.append(newR2)
 
         # See if the best score is an improvement
         newBestR2 = max(newNetScores)
         if newBestR2 > currentR2:
             # Actions for improvement
             bestIndex = newNetScores.index(newBestR2)
@@ -841,15 +867,92 @@
 
     # # Thinned x data
     # ## This is what to use for small nets when curve fitting, as fitting to the true indicies is much harder
     # xShort = [*range(len(yShort))]
 
     # Finish
     return np.array(xThinData), np.array(yThinData), np.array(xPlotData)
-   
+
+
+## Helper/Smol Functions ##
+def applyActi(calcVec:np.ndarray, activationFunction:str):
+    """Applies an activation function to the given vector/array of data in calcVec."""
+
+    # Some idiot proofing (i should put this in more places)
+    activationFunction = activationFunction.upper()
+
+    # Activation function definitions tree
+    if activationFunction == 'LIN':
+        pass
+
+    elif activationFunction == 'ELU':
+        calcVec = 0.4 * (2.7182818284**calcVec - 1)
+
+    elif activationFunction == 'ATAN':
+        calcVec = np.arctan(calcVec)
+
+    elif activationFunction == 'RELU':
+        calcVec[calcVec < 0] = 0
+
+    elif activationFunction == 'RESU':
+        # calcVec[calcVec < 0] = 0
+        calcVec = abs(np.sin(calcVec))*calcVec
+
+    elif activationFunction == 'RESU2':
+        calcVec[calcVec < 0] = 0
+        calcVec = abs(np.sin(calcVec))*calcVec
+
+    elif activationFunction == 'SIG':
+        e_p = np.exp(calcVec)
+        e_n = np.exp(-calcVec)
+        calcVec = ((e_p - e_n) / (e_p + e_n)) + 1
+
+    elif activationFunction == 'EXP':
+        calcVec[calcVec < -0.4] = 0
+
+    else:
+        raise ValueError("Given hidden function is not of the avalible types!")
+
+    # Finish
+    return calcVec
+
+def fastCalc(net:AdvNet, inVector:np.ndarray):
+    """
+    ### EXPERIMENTAL ###
+    Mostly benefits smaller nets, especially with less than a few layers.
+    
+    By voiding data shape checks, this is the equivalent of .Calculate() for a net, but
+    takes less time. If you're using this, that means you are confident the inVector 
+    data you are using is correct, and/or you do not need the many error checks that 
+    .Calculate has.
+
+    This function still supports single float inputs/outputs, just as .Calculate does.
+    """
+    # Basic check - Shape vector to what it should be
+    # If this doesn't work, sounds like a you problem :P
+    inVector = inVector.reshape((net.inSize, 1))
+
+    # Possible fast calculations
+    if net.sizes[0] == 1 and len(net.sizes) == 2: # ~45% of regular calc time
+        inVector = applyActi(inVector*net.weights[0], net.activationFunction[0])
+
+    else:   # ~73% of regular calc time
+        for i in range(len(net.sizes)-1):
+            if i != 0:
+                inVector = inVector.reshape((inVector.size, 1))
+            inVector = applyActi(sum(inVector*net.weights[i]), net.activationFunction[i])
+
+    # Return the vector shaped as a column vector
+    sz = inVector.size
+    if sz == 1:     # if a single number
+        return inVector[0]
+    else:           # all other vectors
+        inVector = inVector.reshape(inVector.size, 1)
+        return inVector
+
 
 ## Old / Depreceated ##
 def Train(Net, inputData, yData, startingTweakAmp=0.8, 
           plotLive=False, plotResults=False, normalizeData=False, 
           hiddenFunc="ELU", trainWeights='all', maxIterations=1000, 
           blockSize=30, Silent=False):
     """
@@ -899,15 +1002,15 @@
     deviation. This is particularly useful when there are multiple unique input
     data sets, with very different values.
     - If True, the mean and std. dev. of the validation data is used as the values
     to de-normalize the net's outputs
 
     8 - hiddenFunc
     - Type == String
-    - Decides what hidden-layer processing should be used. 'NONE' simply passes
+    - Decides what hidden-layer processing should be used. 'LIN' simply passes
     through each summed up vector to the next layer with no processing. The default,
     'ELU', uses the function max(val, 0) before passing on to the next hidden layer.
 
     9 - trainWeights
     - Type == List (or 'gates' or 'middle')
     - Used to select specific weight set(s) to train instead of training all weights.
     Useful for making sure the first and last sets of weights are trained correctly to
@@ -1180,15 +1283,15 @@
     deviation. This is particularly useful when there are multiple unique input
     data sets, with very different values.
     - If True, the mean and std. dev. of the validation data is used as the values
     to de-normalize the net's outputs
 
     8 - hiddenFnc
     - Type == String
-    - Decides what hidden-layer processing should be used. 'NONE' simply passes
+    - Decides what hidden-layer processing should be used. 'LIN' simply passes
     through each summed up vector to the next layer with no processing. The default,
     'ELU', uses the function max(val, 0) before passing on to the next hidden layer.
 
     9 - trainWeights
     - Type == List (or 'gates' or 'middle')
     - Used to select specific weight set(s) to train instead of training all weights.
     Useful for making sure the first and last sets of weights are trained correctly to
```

### Comparing `mcnets-0.2.7/tests/Slope Fitting.ipynb` & `mcnets-0.3.0/tests/Slope Fitting.ipynb`

 * *Files identical despite different names*

### Comparing `mcnets-0.2.7/tests/Speed Tests.ipynb` & `mcnets-0.3.0/tests/Speed Tests.ipynb`

 * *Files identical despite different names*

### Comparing `mcnets-0.2.7/LICENSE` & `mcnets-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `mcnets-0.2.7/README.md` & `mcnets-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `mcnets-0.2.7/pyproject.toml` & `mcnets-0.3.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling", "matplotlib", "numpy"]
 build-backend = "hatchling.build"
 
 [project]
 name = "mcnets"
-version = "0.2.7"
+version = "0.3.0"
 authors = [
   { name="Sean", email="svs.2k15@gmail.com" },
 ]
 description = "A package that demonstrates deep neural nets using Monte Carlo-type random parameter training."
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `mcnets-0.2.7/PKG-INFO` & `mcnets-0.3.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mcnets
-Version: 0.2.7
+Version: 0.3.0
 Summary: A package that demonstrates deep neural nets using Monte Carlo-type random parameter training.
 Project-URL: Homepage, https://github.com/SciCapt/Monte-Carlo-Neural-Nets
 Project-URL: Bug Tracker, https://github.com/SciCapt/Monte-Carlo-Neural-Nets/issues
 Author-email: Sean <svs.2k15@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

