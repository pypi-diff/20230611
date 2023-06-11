# Comparing `tmp/anova_analysis-1.0.4.tar.gz` & `tmp/anova_analysis-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "anova_analysis-1.0.4.tar", last modified: Sat Jun  3 03:16:18 2023, max compression
+gzip compressed data, was "anova_analysis-1.0.5.tar", last modified: Sun Jun 11 11:06:25 2023, max compression
```

## Comparing `anova_analysis-1.0.4.tar` & `anova_analysis-1.0.5.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 03:16:18.615109 anova_analysis-1.0.4/
--rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-06-03 03:16:02.000000 anova_analysis-1.0.4/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)     4854 2023-06-03 03:16:18.615109 anova_analysis-1.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4337 2023-06-03 03:16:02.000000 anova_analysis-1.0.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 03:16:18.615109 anova_analysis-1.0.4/anova_analysis/
--rw-r--r--   0 runner    (1001) docker     (123)     4732 2023-06-03 03:16:02.000000 anova_analysis-1.0.4/anova_analysis/ANOVA_RBD.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-03 03:16:02.000000 anova_analysis-1.0.4/anova_analysis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      557 2023-06-03 03:16:02.000000 anova_analysis-1.0.4/anova_analysis/example.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 03:16:18.615109 anova_analysis-1.0.4/anova_analysis.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4854 2023-06-03 03:16:18.000000 anova_analysis-1.0.4/anova_analysis.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      300 2023-06-03 03:16:18.000000 anova_analysis-1.0.4/anova_analysis.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-03 03:16:18.000000 anova_analysis-1.0.4/anova_analysis.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-06-03 03:16:18.000000 anova_analysis-1.0.4/anova_analysis.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-06-03 03:16:18.000000 anova_analysis-1.0.4/anova_analysis.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-03 03:16:18.615109 anova_analysis-1.0.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1085 2023-06-03 03:16:02.000000 anova_analysis-1.0.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 11:06:25.808191 anova_analysis-1.0.5/
+-rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-06-11 11:06:14.000000 anova_analysis-1.0.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     8325 2023-06-11 11:06:25.808191 anova_analysis-1.0.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7865 2023-06-11 11:06:14.000000 anova_analysis-1.0.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 11:06:25.808191 anova_analysis-1.0.5/anova_analysis/
+-rw-r--r--   0 runner    (1001) docker     (123)     4882 2023-06-11 11:06:14.000000 anova_analysis-1.0.5/anova_analysis/ANOVA_RBD.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-11 11:06:14.000000 anova_analysis-1.0.5/anova_analysis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1413 2023-06-11 11:06:14.000000 anova_analysis-1.0.5/anova_analysis/example.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 11:06:25.808191 anova_analysis-1.0.5/anova_analysis.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8325 2023-06-11 11:06:25.000000 anova_analysis-1.0.5/anova_analysis.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      296 2023-06-11 11:06:25.000000 anova_analysis-1.0.5/anova_analysis.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-11 11:06:25.000000 anova_analysis-1.0.5/anova_analysis.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-06-11 11:06:25.000000 anova_analysis-1.0.5/anova_analysis.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-06-11 11:06:25.000000 anova_analysis-1.0.5/anova_analysis.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-11 11:06:25.808191 anova_analysis-1.0.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1085 2023-06-11 11:06:14.000000 anova_analysis-1.0.5/setup.py
```

### Comparing `anova_analysis-1.0.4/LICENSE.txt` & `anova_analysis-1.0.5/LICENSE`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-MIT License
-
-Copyright (c) 2023 Sarath S
-
-Permission is hereby granted, free of charge, to any person obtaining a copy
-of this software and associated documentation files (the "Software"), to deal
-in the Software without restriction, including without limitation the rights
-to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-copies of the Software, and to permit persons to whom the Software is
-furnished to do so, subject to the following conditions:
-
-The above copyright notice and this permission notice shall be included in all
-copies or substantial portions of the Software.
-
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+MIT License
+
+Copyright (c) 2023 Sarath S
+
+Permission is hereby granted, free of charge, to any person obtaining a copy
+of this software and associated documentation files (the "Software"), to deal
+in the Software without restriction, including without limitation the rights
+to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+copies of the Software, and to permit persons to whom the Software is
+furnished to do so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in all
+copies or substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 SOFTWARE.
```

### Comparing `anova_analysis-1.0.4/anova_analysis/ANOVA_RBD.py` & `anova_analysis-1.0.5/anova_analysis/ANOVA_RBD.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,41 +1,36 @@
 import pandas as pd
 from tabulate import tabulate
 import scipy.stats as stats
+import os
 
-
-def RBD(replication, treatment, input_file_path, output_file_name):
+def RBD(replication, treatment, input_file_path,save_file=None):
     
     # Import the dataset
     df = pd.read_excel(input_file_path)
 
     # Correction Factor
     data_subset = df.iloc[:, 1:]
     total_sum = data_subset.values.sum()
     correctionFactor = (total_sum ** 2) / (replication * treatment)
-    print("Correction Factor:", round(correctionFactor, 2))
-
+    
     # Total Sum of Square
     total_sum_squared = (data_subset ** 2).values.sum()
     totalsum = total_sum_squared - correctionFactor
-    print("Total Sum of Square:", round(totalsum, 2))
-
+    
     # Replication Sum of Square
     column_sums = df.iloc[:, 1:].sum()
     replicationSum = ((column_sums ** 2).sum() / treatment) - correctionFactor
-    print("Replication Sum of Square:", round(replicationSum, 2))
-
+    
     # Treatment Sum of Square
     row_sum = df.iloc[:, 1:].sum(axis=1)
     treatmentSum = ((row_sum ** 2).sum() / replication) - correctionFactor
-    print("Treatment Sum of Square:", round(treatmentSum, 2))
-
+    
     # Error Sum of Square
     Error_sum_square = totalsum - replicationSum - treatmentSum
-    print("Error Sum of Square:", round(Error_sum_square, 2))
 
     # Anova table
     rep = replication - 1
     tre = treatment - 1
     error_df = rep * tre
     total_source = rep + tre + error_df
     total_ss_sum = replicationSum + treatmentSum + Error_sum_square
@@ -52,61 +47,71 @@
     f_value_column = tre_mss / error_mss
     p_value_row_5 = stats.f.ppf(1- significance_level_5, rep, error_df)
     p_value_column_5 = stats.f.ppf(1-significance_level_5, tre, error_df)
     p_value_row_1 = stats.f.ppf(1- significance_level_1, rep, error_df)
     p_value_column_1 = stats.f.ppf(1-significance_level_1, tre, error_df)
  
     # Determine Significance
-    row_significance = "Significant" if p_value_row_5 < f_value_row else "Not Significant"
-    column_significance = "Significant" if p_value_column_5 < f_value_column else "Not Significant"
-    row_significance_1 = "Significant" if p_value_row_1 < f_value_row else "Not Significant"
-    column_significance_1 = "Significant" if p_value_column_1 < f_value_column else "Not Significant"
+    row_significance = "Sig" if p_value_row_5 < f_value_row else "Not Sig"
+    column_significance = "Sig" if p_value_column_5 < f_value_column else "Not Sig"
+    row_significance_1 = "Sig" if p_value_row_1 < f_value_row else "Not Sig"
+    column_significance_1 = "Sig" if p_value_column_1 < f_value_column else "Not Sig"
 
 
     data = {
         "Source": ["Replication", "Treatment", "Error", "Total"],
         "d.f": [rep, tre, error_df, total_source],
         "s.s": [round(replicationSum, 2), round(treatmentSum, 2), round(Error_sum_square, 2),
                  round(total_ss_sum, 2)],
         "m.s": [round(rep_mss, 2), round(tre_mss, 2), round(error_mss, 2), ""],
         "F-ratio": [round(rep_mss / error_mss, 2), round(tre_mss / error_mss, 2), "", ""],
         "p-value (5%)": [round(p_value_row_5,3), round(p_value_column_5,3),'',''],
         "p-value (1%)": [round(p_value_row_1,3), round(p_value_column_1,3),'',''],
-        "Significance (at 5%)": [row_significance, column_significance, "", ""],
-        "Significance (at 1%)": [row_significance_1, column_significance_1, "", ""]
-    
+        "Sig. (at 5%)": [row_significance, column_significance, "", ""],
+        "Sig. (at 1%)": [row_significance_1, column_significance_1, "", ""]
     }
 
     # Create the DataFrame for the table
     table_df = pd.DataFrame(data)
 
     # Print the table
     print(table_df)
 
-    # Save the results in a text file
-    with open(f'{output_file_name}_result.txt', 'w', encoding='utf-8') as file:
-        file.write(f"{output_file_name}: ")
-        file.write("\n")
-        file.write("Correction Factor: {:.2f}\n".format(correctionFactor))
-        file.write("Total Sum of Square: {:.2f}\n".format(totalsum))
-        file.write("Replication Sum of Square: {:.2f}\n".format(replicationSum))
-        file.write("Treatment Sum of Square: {:.2f}\n".format(treatmentSum))
-        file.write("Error Sum of Square: {:.2f}\n\n".format(Error_sum_square))
-        file.write(tabulate(table_df, headers='keys', tablefmt='fancy_grid'))
+    if save_file is None or save_file:
+
+            # Save the results in a text file
+            directory_path = os.path.dirname(input_file_path)
+            output_file_name = os.path.splitext(os.path.basename(input_file_path))[0]
+            output_file_path = os.path.join(directory_path, f"{output_file_name}_result.txt")
+        
+            # Save the results in a text file
+            with open(output_file_path, 'w', encoding='utf-8') as file:
+                file.write(f"{output_file_name}: ")
+                file.write("\n\n")
+                file.write("Correction Factor: {:.2f}\n".format(correctionFactor))
+                file.write("Total Sum of Square: {:.2f}\n".format(totalsum))
+                file.write("Replication Sum of Square: {:.2f}\n".format(replicationSum))
+                file.write("Treatment Sum of Square: {:.2f}\n".format(treatmentSum))
+                file.write("Error Sum of Square: {:.2f}\n\n".format(Error_sum_square))
+                file.write(tabulate(table_df, headers='keys', tablefmt='grid'))
 
-    print(f"Result saved in {output_file_name}_result.txt")
+            print(f"Result saved in {output_file_path}")
 
     result = {
+        "global_dataframe" : table_df,
         "correction_factor": round(correctionFactor, 2),
         "total_sum_of_square": round(totalsum, 2),
         "replication_sum_of_square": round(replicationSum, 2),
         "treatment_sum_of_square": round(treatmentSum, 2),
         "error_sum_of_square": round(Error_sum_square, 2),
         "replication_df": rep,
         "treatment_df": tre,
         "errors_df": error_df,
         "rep_mean_ss":round(rep_mss, 2),
         "tre_mean_ss": round(tre_mss, 2),
-        "error_mean_ss":round(error_mss, 2)
+        "error_mean_ss":round(error_mss, 2),
+        "total_df": total_source,
+        "total_ss": round(total_ss_sum, 2)
+
     }
     # Return the result
     return result
```

### Comparing `anova_analysis-1.0.4/setup.py` & `anova_analysis-1.0.5/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 with open("README.md", "r", encoding="utf-8") as fh:
     LONG_DESCRIPTION = fh.read()
 
 # Setting up
 setup(
         name="anova_analysis", 
-        version="1.0.4",
+        version="1.0.5",
         authors=['Sarath S','Saranyadevi S'],
         author_email="insightagri10@gmail.com",
         description="A package for performing ANOVA analysis by RBD",
         license='MIT',
         long_description=LONG_DESCRIPTION,
         long_description_content_type="text/markdown",
         packages=find_packages(),
```

