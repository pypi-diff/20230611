# Comparing `tmp/portpy-0.0.1.tar.gz` & `tmp/portpy-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\portpy-0.0.1.tar", last modified: Thu Mar 30 13:51:41 2023, max compression
+gzip compressed data, was "dist\portpy-0.0.2.tar", last modified: Sun Jun 11 19:16:31 2023, max compression
```

## Comparing `portpy-0.0.1.tar` & `portpy-0.0.2.tar`

### file list

```diff
@@ -1,38 +1,45 @@
-drwxrwxrwx   0        0        0        0 2023-03-30 13:51:41.000000 portpy-0.0.1/
--rw-rw-rw-   0        0        0       20 2023-03-30 13:48:44.000000 portpy-0.0.1/MANIFEST.in
--rw-rw-rw-   0        0        0     6266 2023-03-30 13:51:41.000000 portpy-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0     4693 2023-03-17 23:55:47.000000 portpy-0.0.1/README.md
-drwxrwxrwx   0        0        0        0 2023-03-30 13:51:40.000000 portpy-0.0.1/images/
--rw-rw-rw-   0        0        0   184526 2022-10-13 14:45:48.000000 portpy-0.0.1/images/PortPy_logo.jpg
-drwxrwxrwx   0        0        0        0 2023-03-30 13:51:40.000000 portpy-0.0.1/portpy/
--rw-rw-rw-   0        0        0       52 2023-03-30 13:37:47.000000 portpy-0.0.1/portpy/__init__.py
-drwxrwxrwx   0        0        0        0 2023-03-30 13:51:40.000000 portpy-0.0.1/portpy/photon/
--rw-rw-rw-   0        0        0      249 2023-03-28 15:55:44.000000 portpy-0.0.1/portpy/photon/__init__.py
--rw-rw-rw-   0        0        0     6047 2023-03-17 23:55:54.000000 portpy-0.0.1/portpy/photon/beam.py
--rw-rw-rw-   0        0        0     4294 2023-03-17 23:55:54.000000 portpy-0.0.1/portpy/photon/clinical_criteria.py
--rw-rw-rw-   0        0        0    18285 2023-03-27 19:08:23.000000 portpy-0.0.1/portpy/photon/cvxpy_prob.py
--rw-rw-rw-   0        0        0    23944 2023-03-27 19:08:22.000000 portpy-0.0.1/portpy/photon/cvxpy_prob_old.py
--rw-rw-rw-   0        0        0    24585 2023-03-27 19:08:22.000000 portpy-0.0.1/portpy/photon/cvxpy_prob_rev2.py
--rw-rw-rw-   0        0        0     4972 2023-01-17 21:16:18.000000 portpy-0.0.1/portpy/photon/evaluation.py
--rw-rw-rw-   0        0        0    47794 2023-03-19 16:49:43.000000 portpy-0.0.1/portpy/photon/influence_matrix.py
--rw-rw-rw-   0        0        0    31773 2023-03-27 19:08:22.000000 portpy-0.0.1/portpy/photon/optimization.py
--rw-rw-rw-   0        0        0    17877 2023-03-28 14:36:55.000000 portpy-0.0.1/portpy/photon/plan.py
--rw-rw-rw-   0        0        0    13195 2023-03-17 23:55:54.000000 portpy-0.0.1/portpy/photon/structures.py
-drwxrwxrwx   0        0        0        0 2023-03-30 13:51:40.000000 portpy-0.0.1/portpy/photon/utils/
--rw-rw-rw-   0        0        0      204 2023-03-28 14:35:20.000000 portpy-0.0.1/portpy/photon/utils/__init__.py
--rw-rw-rw-   0        0        0     5415 2023-02-03 20:43:08.000000 portpy-0.0.1/portpy/photon/utils/load_data.py
--rw-rw-rw-   0        0        0     4828 2023-03-17 23:55:54.000000 portpy-0.0.1/portpy/photon/utils/load_metadata.py
--rw-rw-rw-   0        0        0     2471 2023-03-28 21:24:21.000000 portpy-0.0.1/portpy/photon/utils/save_nrrd.py
--rw-rw-rw-   0        0        0     4887 2023-03-27 19:08:22.000000 portpy-0.0.1/portpy/photon/utils/save_or_load_pickle.py
--rw-rw-rw-   0        0        0     1385 2023-03-17 23:55:54.000000 portpy-0.0.1/portpy/photon/utils/slicer_script.py
--rw-rw-rw-   0        0        0     1347 2023-03-27 19:08:24.000000 portpy-0.0.1/portpy/photon/utils/sol_change_inf_matrix.py
--rw-rw-rw-   0        0        0     4128 2023-03-17 23:55:54.000000 portpy-0.0.1/portpy/photon/utils/view_in_slicer_jupyter.py
--rw-rw-rw-   0        0        0    42096 2023-03-29 19:55:20.000000 portpy-0.0.1/portpy/photon/visualization.py
-drwxrwxrwx   0        0        0        0 2023-03-30 13:51:40.000000 portpy-0.0.1/portpy.egg-info/
--rw-rw-rw-   0        0        0     6266 2023-03-30 13:51:39.000000 portpy-0.0.1/portpy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      876 2023-03-30 13:51:39.000000 portpy-0.0.1/portpy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-03-30 13:51:39.000000 portpy-0.0.1/portpy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      352 2023-03-30 13:51:39.000000 portpy-0.0.1/portpy.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-03-30 13:51:39.000000 portpy-0.0.1/portpy.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-03-30 13:51:41.000000 portpy-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0     2509 2023-03-30 13:45:31.000000 portpy-0.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-11 19:16:32.000000 portpy-0.0.2/
+-rw-rw-rw-   0        0        0      128 2023-05-12 06:19:04.000000 portpy-0.0.2/MANIFEST.in
+-rw-rw-rw-   0        0        0     7798 2023-06-11 19:16:32.000000 portpy-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0     6192 2023-06-06 19:15:25.000000 portpy-0.0.2/README.md
+drwxrwxrwx   0        0        0        0 2023-06-11 19:16:31.000000 portpy-0.0.2/config_files/
+drwxrwxrwx   0        0        0        0 2023-06-11 19:16:31.000000 portpy-0.0.2/config_files/clinical_criteria/
+drwxrwxrwx   0        0        0        0 2023-06-11 19:16:31.000000 portpy-0.0.2/config_files/clinical_criteria/Default/
+-rw-rw-rw-   0        0        0     2511 2023-01-19 21:58:41.000000 portpy-0.0.2/config_files/clinical_criteria/Default/Lung_2Gy_30Fx.json
+drwxrwxrwx   0        0        0        0 2023-06-11 19:16:31.000000 portpy-0.0.2/config_files/optimization_params/
+-rw-rw-rw-   0        0        0     2419 2023-05-13 03:05:59.000000 portpy-0.0.2/config_files/optimization_params/optimization_params_Lung_2Gy_30Fx.json
+drwxrwxrwx   0        0        0        0 2023-06-11 19:16:31.000000 portpy-0.0.2/images/
+-rw-rw-rw-   0        0        0   184526 2023-05-12 05:53:35.000000 portpy-0.0.2/images/PortPy_logo.jpg
+drwxrwxrwx   0        0        0        0 2023-06-11 19:16:31.000000 portpy-0.0.2/portpy/
+-rw-rw-rw-   0        0        0       52 2023-05-12 06:21:33.000000 portpy-0.0.2/portpy/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-11 19:16:31.000000 portpy-0.0.2/portpy/photon/
+-rw-rw-rw-   0        0        0      430 2023-05-10 05:07:25.000000 portpy-0.0.2/portpy/photon/__init__.py
+-rw-rw-rw-   0        0        0     8340 2023-05-15 03:35:09.000000 portpy-0.0.2/portpy/photon/beam.py
+-rw-rw-rw-   0        0        0     4992 2023-05-13 03:47:18.000000 portpy-0.0.2/portpy/photon/clinical_criteria.py
+-rw-rw-rw-   0        0        0      548 2023-05-11 18:21:16.000000 portpy-0.0.2/portpy/photon/ct.py
+-rw-rw-rw-   0        0        0    18530 2023-05-13 03:32:20.000000 portpy-0.0.2/portpy/photon/cvxpy_prob.py
+-rw-rw-rw-   0        0        0    23387 2023-05-17 10:37:53.000000 portpy-0.0.2/portpy/photon/data_explorer.py
+-rw-rw-rw-   0        0        0    14619 2023-05-13 03:32:20.000000 portpy-0.0.2/portpy/photon/evaluation.py
+-rw-rw-rw-   0        0        0    53003 2023-06-07 19:53:55.000000 portpy-0.0.2/portpy/photon/influence_matrix.py
+-rw-rw-rw-   0        0        0    23374 2023-05-17 09:39:36.000000 portpy-0.0.2/portpy/photon/optimization.py
+-rw-rw-rw-   0        0        0    10945 2023-05-17 09:34:05.000000 portpy-0.0.2/portpy/photon/plan.py
+-rw-rw-rw-   0        0        0    16378 2023-05-15 03:42:09.000000 portpy-0.0.2/portpy/photon/structures.py
+drwxrwxrwx   0        0        0        0 2023-06-11 19:16:31.000000 portpy-0.0.2/portpy/photon/utils/
+-rw-rw-rw-   0        0        0      262 2023-05-16 17:51:57.000000 portpy-0.0.2/portpy/photon/utils/__init__.py
+-rw-rw-rw-   0        0        0     2058 2023-05-17 06:00:15.000000 portpy-0.0.2/portpy/photon/utils/get_eclipse_fluence.py
+-rw-rw-rw-   0        0        0     5415 2023-05-12 05:53:35.000000 portpy-0.0.2/portpy/photon/utils/load_data.py
+-rw-rw-rw-   0        0        0     4828 2023-05-12 05:53:35.000000 portpy-0.0.2/portpy/photon/utils/load_metadata.py
+-rw-rw-rw-   0        0        0     2846 2023-05-15 12:19:37.000000 portpy-0.0.2/portpy/photon/utils/save_nrrd.py
+-rw-rw-rw-   0        0        0     4887 2023-05-15 11:43:22.000000 portpy-0.0.2/portpy/photon/utils/save_or_load_pickle.py
+-rw-rw-rw-   0        0        0     1387 2023-05-09 07:09:19.000000 portpy-0.0.2/portpy/photon/utils/slicer_script.py
+-rw-rw-rw-   0        0        0     1347 2023-03-27 19:08:24.000000 portpy-0.0.2/portpy/photon/utils/sol_change_inf_matrix.py
+-rw-rw-rw-   0        0        0     4132 2023-05-09 07:09:19.000000 portpy-0.0.2/portpy/photon/utils/view_in_slicer_jupyter.py
+-rw-rw-rw-   0        0        0    20553 2023-05-15 11:48:55.000000 portpy-0.0.2/portpy/photon/visualization.py
+drwxrwxrwx   0        0        0        0 2023-06-11 19:16:31.000000 portpy-0.0.2/portpy.egg-info/
+-rw-rw-rw-   0        0        0     7798 2023-06-11 19:16:28.000000 portpy-0.0.2/portpy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1035 2023-06-11 19:16:28.000000 portpy-0.0.2/portpy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-11 19:16:28.000000 portpy-0.0.2/portpy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      352 2023-06-11 19:16:28.000000 portpy-0.0.2/portpy.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-06-11 19:16:28.000000 portpy-0.0.2/portpy.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-11 19:16:32.000000 portpy-0.0.2/setup.cfg
+-rw-rw-rw-   0        0        0     2502 2023-05-30 02:26:49.000000 portpy-0.0.2/setup.py
```

### Comparing `portpy-0.0.1/PKG-INFO` & `portpy-0.0.2/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,79 +1,84 @@
 Metadata-Version: 2.1
 Name: portpy
-Version: 0.0.1
+Version: 0.0.2
 Summary: First open-source radiation treatment planning system in Python
-Home-page: https://github.com/PortPy-Project/PortPy-Photon
+Home-page: https://github.com/PortPy-Project/PortPy
 Author: Gourav Jhanwar, Mojtaba Tefagh, Vicki Taasti, Seppo Tuomaala, Saad Nadeem, Masoud Zarepisheh
 Author-email: jhanwarg@mskcc.struct, mtefagh@acm.struct, vicki.taasti@maastro.nl, tuomaals@mskcc.struct, nadeems@mskcc.struct, zarepism@mskcc.struct
 License: Apache License, Version 2.0
 Description: <p align="center">
           <img src="./images/PortPy_logo.jpg" width="50%">
         </p>
         
         # What is PortPy?
-        **Note: The package is at its early stages of development (version 0.0.3) and we are now collecting feedback from researchers to further refine the data structure and the main functionality. We are expecting to have a stable version 1.xx around March 2023. We would love to hear your feedback.**
+        **Note: The package is at its early stages of development (version 0.0.1) and we are now collecting feedback from researchers to further refine the data structure and the main functionality. We are expecting to have a stable version 1.xx around July 2023. We would love to hear your feedback.**
         
         PortPy (**P**lanning and **O**ptimization for **R**adiation **T**herapy) is a community effort to develop the **first opensource python library** to facilitate the development and clinical translation of radiotherapy cancer treatment planning algorithms. PortPy includes:
         1. Research-ready data and code for *benchmarking*, *reproducibility*, and *community-driven* development.
         2. Interface to an open-source optimization package [CVXPy](https://www.cvxpy.org/) for easy/quick prototyping and out-of-the-box access to commercial/opensource optimization engines (e.g., Mosek, Gorubi, CPLEX, IPOPT).
         3. Visualization modules to visualize relevant plan information (e.g, dose volume histograms, dose distribution, fluence map).
         4. Evaluation modules to quantify plan quality with respect to established clinical metrics (e.g., RTOG metrics, dose conformality, tumor control probability, normal tissue control probability).
         # Data
         Data needed for optimization and algorithm development (e.g., a set of beams/beamlets/voxels, dose contribution of each beamlet to each voxel) are provided for a set of pre-specified machine parameters (e.g., beam/collimator/couch angles). We will initially provide these for a set of publicly available datasets from [TCIA](https://www.cancerimagingarchive.net/). We hope to expand our dataset in the future. The data needed for optimization is extracted from the research version of Eclipse<sup>TM</sup> treatment planning system ([Varian Medical Systems](https://www.varian.com/)) using its API. 
         
         You can download the sample patient data [here](https://drive.google.com/drive/folders/1nA1oHEhlmh2Hk8an9e0Oi0ye6LRPREit?usp=sharing).
         
-        Create a directory named './data' in the current project directory and copy the downloaded file to it, e.g ./data/Lung_Patient_1
+        Create a directory named './data' in the current project directory and copy the downloaded file to it, e.g ./data/Lung_Phantom_Patient_1
         
+        # Quick Start
+        Please see below for understanding the basic functionalities of PortPy. For advance usage of PortPy, we recommend navigating through [examples](https://github.com/PortPy-Project/PortPy/tree/master/examples) folder.
+        1. To understand the most important features of PortPy, we highly recommend to go through notebook [ex_1_introduction.ipynb](https://github.com/PortPy-Project/PortPy/blob/master/examples/ex_1_introduction.ipynb)
+        2. One of the major computational issues while optimizing the plan arise due to large size of influence matrix. We suggest you to follow [ex_2_down_sampling.py](https://github.com/PortPy-Project/PortPy/blob/master/examples/ex_2_downsampling.py) to understand how PortPy can assist in resolving it.
+        3. You can check out [ex_3_structure_operations.py](https://github.com/PortPy-Project/PortPy/blob/master/examples/ex_3_structure_operations.py) to know how to perform different structure operations (e.g., boolean, margin).
+        4. For algorithm benchmarking, the global optimal solution is provided for non-convex optimization problems resulting from beam angle optimization [ex_6_boo_benchmark.py](https://github.com/PortPy-Project/PortPy/blob/master/examples/ex_6_boo_benchmark.py) and incorporating DVH constraints [ex_6_dvh_benchmark.py](https://github.com/PortPy-Project/PortPy/blob/master/examples/ex_6_dvh_benchmark.py) using the mixed-integer programming on down-sampled data.
+        5. In addition to basic visualization capabilities, PortPy provide advanced visualization by integration with 3D Slicer. Please look out notebook [ex_7_Slicer.ipynb](https://github.com/PortPy-Project/PortPy/blob/master/examples/ex_7_Slicer.ipynb)
         
         # Installing PortPy
         
         1. Installing using pip
           ```bash
-          pip install portpy-photon
+          pip install portpy
           ```
         2. Installing using conda
           ```bash
-          conda install -c conda-forge portpy-photon
+          conda install -c conda-forge portpy
           ```
         3. Installing from source
         - Clone this repository:
           ```bash
-          git clone https://github.com/PortPy-Project/PortPy-Photon.git
-          cd portpy_photon
+          git clone https://github.com/PortPy-Project/PortPy.git
+          cd portpy
           ```
         
         - You need to install the dependencies in either a python virtual environment or anaconda environment. Instructions for setting up in python virtual environment are as follows:
         
           Install all the dependencies present in requirements.txt:
           ```bash
           python3 -m venv venv
           source venv/bin/activate
           (venv) pip install -r requirements.txt
           ```
         
-        To better understand the PortPy functionality, we recommend running an example script eg_1_basics.py for creating and visualizing a sample IMRT plan.
-        
-        # License
-        PortPy code is distributed under **Apache 2.0 with Commons Clause** license, and is available for non-commercial academic purposes.
-        
         # Team
         PortPy is a community project initiated at [Memorial Sloan Kettering Cancer Center](https://www.mskcc.org/). It is currently developed and maintained by:
         
         | Name                                                                         | Expertise                                        | Institution |
         |------------------------------------------------------------------------------|--------------------------------------------------|-------------|
         | [Masoud Zarepisheh](https://masoudzp.github.io/)                             | Treatment Planning and Optimization              | MSK         |
         | [Saad Nadeem](https://nadeemlab.org/)                                        | Computer Vision and AI in Medical Imaging        | MSK         |
         | [Gourav Jhanwar](https://github.com/gourav3017)                              | Algorithm Design and Development                 | MSK         |
         | [Mojtaba Tefagh](https://github.com/mtefagh)                                 | Mathematical Modeling and Reinforcement Learning | SUT         |
         | [Vicki Taasti](https://scholar.google.com/citations?user=PEPyvewAAAAJ&hl=en) | Physics and Planning of Proton Therapy           | MAASTRO     |
         | [Sadegh Alam](https://scholar.google.com/citations?user=iy7TlU0AAAAJ&hl=en)  | Adaptive Treatment Planning and Imaging          | Cornell     |
         | [Seppo Tuomaala](https://www.linkedin.com/in/seppo-tuomaala-5b57913/)        | Eclispe API Scripting                            | VARIAN      |
         
+        # License
+        PortPy code is distributed under **Apache 2.0 with Commons Clause** license, and is available for non-commercial academic purposes.
+        
 Platform: UNKNOWN
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `portpy-0.0.1/images/PortPy_logo.jpg` & `portpy-0.0.2/images/PortPy_logo.jpg`

 * *Files identical despite different names*

### Comparing `portpy-0.0.1/portpy/photon/clinical_criteria.py` & `portpy-0.0.2/portpy/photon/clinical_criteria.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from typing import List
-
+from .data_explorer import DataExplorer
 
 class ClinicalCriteria:
     """
     A class representing clinical criteria.
 
     - **Attributes** ::
 
@@ -23,21 +23,39 @@
 
     - **Methods** ::
         :add_criterion(criterion:str, parameters:dict, constraints:dict)
         :modify_criterion(criterion:str, parameters:dict, constraints:dict)
 
     """
 
-    def __init__(self, clinical_criteria):
+    def __init__(self, data: DataExplorer, protocol_name: str = None, protocol_type: str = 'Default'):
         """
 
         :param clinical_criteria: dictionary containing information about clinical criteria
 
         """
-        self.clinical_criteria_dict = clinical_criteria
+        clinical_criteria_dict = data.load_config_clinical_criteria(protocol_name, protocol_type=protocol_type)
+        self.clinical_criteria_dict = clinical_criteria_dict
+
+    def get_prescription(self) -> float:
+        """
+
+        :return: prescription in Gy
+        """
+        pres = self.clinical_criteria_dict['pres_per_fraction_gy'] * \
+               self.clinical_criteria_dict[
+                   'num_of_fractions']
+        return pres
+
+    def get_num_of_fractions(self) -> float:
+        """
+
+        :return: number of fractions to be delivered
+        """
+        return self.clinical_criteria_dict['num_of_fractions']
 
     def add_criterion(self, criterion: str, parameters: dict, constraints: dict) -> None:
         """
         Add criterion to the clinical criteria dictionary
 
         :param criterion: criterion name. e.g. max_dose
         :param parameters: parameters dictionary e.g. parameters = {'struct':'PTV'}
```

### Comparing `portpy-0.0.1/portpy/photon/cvxpy_prob.py` & `portpy-0.0.2/portpy/photon/cvxpy_prob.py`

 * *Files 3% similar despite different names*

```diff
@@ -100,16 +100,16 @@
         for i in range(len(mean_constraints)):
             if 'mean_dose' in mean_constraints[i]['name']:
                 if 'limit_dose_gy' in mean_constraints[i]['constraints']:
                     limit = mean_constraints[i]['constraints']['limit_dose_gy']
                     org = mean_constraints[i]['parameters']['structure_name']
                     # mean constraints using voxel weights
                     if org in my_plan.structures.structures_dict['name']:
-                        constraints += [(1 / sum(st.get_opt_voxels_size(org))) *
-                                        (cp.sum((cp.multiply(st.get_opt_voxels_size(org), A[st.get_opt_voxels_idx(org),
+                        constraints += [(1 / sum(st.get_opt_voxels_volume_cc(org))) *
+                                        (cp.sum((cp.multiply(st.get_opt_voxels_volume_cc(org), A[st.get_opt_voxels_idx(org),
                                                                                           :] @ x)))) <= limit / num_fractions]
 
                     else:
                         print('Structure {} not available!'.format(org))
 
         # Step 1 and 2 constraints
         constraints += [A[st.get_opt_voxels_idx('PTV'), :] @ x <= pres_per_frac + dO]
@@ -118,45 +118,48 @@
         self.constraints = constraints
 
         print('Constraints done')
 
     def add_max(self, struct: str, dose_gy: float):
         """
         Add max constraints to the problem
+
         :param struct: structure name
         :param dose_gy: dose in Gy per fraction.
         :return:
         """
         A = self.inf_matrix.A
         st = self.inf_matrix
         x = self.x
 
         max_constraint = [A[st.get_opt_voxels_idx(struct), :] @ x <= dose_gy]
         self.add_constraints(max_constraint)
 
     def add_mean(self, struct: str, dose_gy: float):
         """
         Add mean constraints to the problem
+
         :param struct: structure name
         :param dose_gy: dose in Gy per fraction.
         :return:
         """
         A = self.inf_matrix.A
         st = self.inf_matrix
         x = self.x
 
-        mean_constraint = [(1 / sum(st.get_opt_voxels_size(struct))) *
-                           (cp.sum((cp.multiply(st.get_opt_voxels_size(struct),
+        mean_constraint = [(1 / sum(st.get_opt_voxels_volume_cc(struct))) *
+                           (cp.sum((cp.multiply(st.get_opt_voxels_volume_cc(struct),
                                                 A[st.get_opt_voxels_idx(struct),
                                                 :] @ x)))) <= dose_gy]
         self.add_constraints(mean_constraint)
 
     def add_overdose_quad(self, struct: str, dose_gy: float, weight: float = 10000):
         """
         Add quadratic loss for the overdose voxels of the structure
+
         :param struct: structure name
         :param dose_gy: dose in Gy per fraction.
         :param weight: penalty/weight in the objective for overdose
         :return:
         """
         A = self.inf_matrix.A
         st = self.inf_matrix
@@ -166,14 +169,15 @@
         obj = (1 / len(st.get_opt_voxels_idx(struct))) * (weight * cp.sum_squares(dO))
         self.add_objective(obj)
         self.add_constraints([A[st.get_opt_voxels_idx('PTV'), :] @ x <= dose_gy + dO])
 
     def add_underdose_quad(self, struct: str, dose_gy: float, weight: float = 100000):
         """
         Add quadratic loss for the underdose voxels of the structure
+
         :param struct: structure name
         :param dose_gy: dose in Gy per fraction.
         :param weight: penalty/weight in the objective for underdose
         :return:
         """
         A = self.inf_matrix.A
         st = self.inf_matrix
@@ -185,14 +189,15 @@
         self.add_constraints([A[st.get_opt_voxels_idx('PTV'), :] @ x >= dose_gy - dU])
 
     def add_quad(self, struct: str = None, voxels: np.ndarray = None, weight: float = 10,
                  voxels_weight: np.ndarray = None):
 
         """
         Add quadratic objective to the optimization problem
+
         :param struct: structure for which quadratic loss is added to objective function
         :param voxels: Default to None. If set, quadratic loss will be added for the given voxels
         :param weight: Default to 10. penalty in the objective function for the given structure.
         :param voxels_weight: weight for each voxel in the objective function
         :return:
         """
         A = self.inf_matrix.A
@@ -209,14 +214,15 @@
             obj = (1 / len(st.get_opt_voxels_idx(struct))) * (
                     weight * cp.sum_squares(A[st.get_opt_voxels_idx(struct), :] @ x))
         self.add_objective(obj)
 
     def add_smoothness_quad(self, weight: int = 10, smoothness_X_weight: int = 0.6, smoothness_Y_weight: int = 0.4):
         """
         Add quadratic smoothness to the optimization problem
+
         :param weight: smoothness weight
         :param smoothness_X_weight: weight in X direction of MLC (parallel to MLC)
         :param smoothness_Y_weight: weight in Y direction of MLC (perpendicular to MLC)
         :return:
         """
 
         st = self.inf_matrix
@@ -226,34 +232,37 @@
         obj = weight * (
                 smoothness_X_weight * (1 / num_cols) * cp.sum_squares(Qx @ x) + smoothness_Y_weight * (1 / num_rows)
                 * cp.sum_squares(Qy @ x))
         self.add_objective(obj)
 
     def add_constraints(self, constraints: list):
         """
-        Add constraint to the problem
+        Add constraint to the constraint list of problem
+
         :param constraints: list of constraints
         :return:
         """
         self.constraints += constraints
 
     def add_objective(self, obj):
         """
-        Add objective function to the problem
+        Add objective function to objective list of the problem
+
         :param obj: objective function expression using cvxpy
         :return:
         """
         if not isinstance(obj, list):
             obj = [obj]
 
         self.obj += obj
 
     def add_boo(self, num_beams: int):
         """
         Select optimal beams from set of beams using MIP
+
         :param num_beams: number of beams to be selected
         :return:
         """
         st = self.inf_matrix
         x = self.x
 
         #  Constraints for selecting beams
@@ -273,15 +282,21 @@
     def solve(self, *args, **kwargs):
         problem = cp.Problem(cp.Minimize(sum(self.obj)), constraints=self.constraints)
         problem.solve(*args, **kwargs)
 
     def get_sol(self) -> dict:
         """
         Return optimal solution and influence matrix associated with it in the form of dictionary
-        :return:
+
+        :Example
+                dict = {"optimal_fluence": [..],
+                "inf_matrix": my_plan.inf_marix
+                }
+
+        :return: solution dictionary
         """
         return {'optimal_intensity': self.x.value, 'inf_matrix': self.inf_matrix}
 
     def add_dvh(self, dvh_constraint: list):
 
         A = self.inf_matrix.A
         st = self.inf_matrix
@@ -322,16 +337,16 @@
             struct, limit, v, M = df_dvh_criteria.loc[i, 'structure'], df_dvh_criteria.loc[i, 'dose_gy'], \
                                   df_dvh_criteria.loc[i, 'vol_perc'], df_dvh_criteria.loc[i, 'M']
             end = start + len(st.get_opt_voxels_idx(struct))
             frac = self.my_plan.structures.get_fraction_of_vol_in_calc_box(struct)
             constraints += [
                 A[st.get_opt_voxels_idx(struct), :] @ x <= limit / self.my_plan.get_num_of_fractions()
                 + b_dvh[start:end] * M / self.my_plan.get_num_of_fractions()]
-            constraints += [b_dvh @ st.get_opt_voxels_size(struct) <= (v / frac) / 100 * sum(
-                st.get_opt_voxels_size(struct))]
+            constraints += [b_dvh @ st.get_opt_voxels_volume_cc(struct) <= (v / frac) / 100 * sum(
+                st.get_opt_voxels_volume_cc(struct))]
             start = end
         self.add_constraints(constraints=constraints)
 
     @staticmethod
     def get_smoothness_matrix(beamReq: List[dict]) -> (np.ndarray, np.ndarray, int, int):
         """
         Create smoothness matrix so that adjacent beamlets are smooth out to reduce MU
```

### Comparing `portpy-0.0.1/portpy/photon/cvxpy_prob_old.py` & `portpy-0.0.2/portpy/photon/optimization.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,236 +1,280 @@
 from __future__ import annotations
 import numpy as np
 import cvxpy as cp
-from typing import List, TYPE_CHECKING
+from typing import List, TYPE_CHECKING, Union
 
 if TYPE_CHECKING:
     from portpy.photon.plan import Plan
     from portpy.photon.influence_matrix import InfluenceMatrix
-import json
+from .clinical_criteria import ClinicalCriteria
 
 
-class CvxPyProb(object):
+class Optimization(object):
     """
-    Optimization class for creating cvxpy problem object
+    Optimization class for optimizing and creating the plan
+
+    :param my_plan: object of class Plan
+    :param inf_matrix: object of class InfluenceMatrix
+    :param clinical_criteria: clinical criteria for which plan to be optimized
+    :param opt_params: optimization parameters for modifying parameters of problem statement
+
     """
 
-    def __init__(self, my_plan: Plan, inf_matrix: InfluenceMatrix = None, max_constraints: List[dict] = None,
-                 mean_constraints: List[dict] = None, obj_from_file: str = None, **opt_params):
+    def __init__(self, my_plan: Plan, inf_matrix: InfluenceMatrix = None,
+                 clinical_criteria: ClinicalCriteria = None,
+                 opt_params: dict = None):
+        # self.x = None
+        self.my_plan = my_plan
+        if inf_matrix is None:
+            inf_matrix = my_plan.inf_matrix
+        self.inf_matrix = inf_matrix
+        if clinical_criteria is None:
+            clinical_criteria = my_plan.clinical_criteria
+        self.clinical_criteria = clinical_criteria
+        self.opt_params = opt_params
+        self.prescription_gy = opt_params['prescription_gy']
+        self.obj = []
+        self.constraints = []
+        self.vars = {}
+
+    def create_cvxpy_problem(self):
         """
         It runs optimization to create optimal plan based upon clinical criteria
 
-        :param my_plan: object of class Plan
-        :param inf_matrix: object of class InfluenceMatrix
-        :param solver: default solver 'MOSEK'. check cvxpy website for available solvers
-        :param verbose: Default to True. If set to False, it will not print the solver iterations.
-        :param cvxpy_options: cvxpy and the solver settings
-        :param opt_params: optimization parameters for modifying parameters of problem statement
         :return: cvxpy problem object
 
         """
 
-        # get data for optimization
-        if max_constraints is None:
-            max_constraints = []
-        if mean_constraints is None:
-            mean_constraints = []
-
-        if inf_matrix is None:
-            inf_matrix = my_plan.inf_matrix
+        # unpack data
+        my_plan = self.my_plan
+        inf_matrix = self.inf_matrix
+        opt_params = self.opt_params
+        clinical_criteria = self.clinical_criteria
+        # self.prescription_gy = opt_params['prescription_gy']
+
+        # get opt params for optimization
+        obj_funcs = opt_params['objective_functions'] if 'objective_functions' in opt_params else []
+        opt_params_constraints = opt_params['constraints'] if 'constraints' in opt_params else []
+
+        # Creating rinds (aka rings, shells)
+        # Rinds are doughnut-shaped structures often created to control the radiation dose to non-specified structures
+        #   They can also control the dose fall-off after PTV.
 
         A = inf_matrix.A
-        num_fractions = my_plan.get_num_of_fractions()
+        num_fractions = clinical_criteria.get_num_of_fractions()
         st = inf_matrix
 
-        self.my_plan = my_plan
-        self.inf_matrix = inf_matrix
-
-        # create and add rind constraints
-        rinds = ['RIND_0', 'RIND_1', 'RIND_2', 'RIND_3', 'RIND_4']
-        if rinds[0] not in my_plan.structures.structures_dict[
-            'name']:  # check if rind is already created. If yes, skip rind creation
-            self.create_rinds(my_plan, size_mm=[5, 5, 20, 30, 500])
-            self.set_rinds_opt_voxel_idx(my_plan,
-                                         inf_matrix=inf_matrix)  # rind_0 is 5mm after PTV, rind_2 is 5 mm after rind_1, and so on..
-        else:
-            self.set_rinds_opt_voxel_idx(my_plan, inf_matrix=inf_matrix)
-
-        rind_max_dose_perc = [1.1, 1.05, 0.9, 0.85, 0.75]
-        for i, rind in enumerate(rinds):  # Add rind constraints
-            parameters = {'structure_name': rind}
-            total_pres = my_plan.get_prescription()
-            constraints = {'limit_dose_gy': total_pres * rind_max_dose_perc[i]}
-            my_plan.clinical_criteria.add_criterion(criterion='max_dose', parameters=parameters,
-                                                    constraints=constraints)
-            if len(max_constraints) > 0:  # update max constraints by adding rind max constraints
-                max_constraints = my_plan.clinical_criteria.get_criteria(name='max_dose')
-
-        # Opt params
-        # # setting weights for oar objectives
-        # all_vox = np.arange(A.shape[0])
-        # oar_voxels = all_vox[~np.isin(np.arange(A.shape[0]), st.get_opt_voxels_idx('PTV'))]
-        # oar_weights = np.ones(A[oar_voxels, :].shape[0])
-        # if my_plan.get_disease_site() == 'Prostate':
-        #     oar_weights[np.where(np.isin(oar_voxels, st.get_opt_voxels_idx('RECT_WALL')))] = 20
-        #     oar_weights[np.where(np.isin(oar_voxels, st.get_opt_voxels_idx('BLAD_WALL')))] = 5
-        #     oar_weights[np.where(np.isin(oar_voxels, st.get_opt_voxels_idx('RIND_0')))] = 3
-        #     oar_weights[np.where(np.isin(oar_voxels, st.get_opt_voxels_idx('RIND_1')))] = 3
-        # elif my_plan.get_disease_site() == 'Lung':
-        #     oar_weights[np.where(np.isin(oar_voxels, st.get_opt_voxels_idx('CORD')))] = 10
-        #     oar_weights[np.where(np.isin(oar_voxels, st.get_opt_voxels_idx('ESOPHAGUS')))] = 20
-        #     if 'HEART' in st.opt_voxels_dict['name']:
-        #         oar_weights[np.where(np.isin(oar_voxels, st.get_opt_voxels_idx('HEART')))] = 20
-        #     oar_weights[np.where(np.isin(oar_voxels, st.get_opt_voxels_idx('RIND_0')))] = 3
-        #     oar_weights[np.where(np.isin(oar_voxels, st.get_opt_voxels_idx('RIND_1')))] = 3
-        # ptv_overdose_weight = opt_params['ptv_overdose_weight'] if 'ptv_overdose_weight' in opt_params else 10000
-        # ptv_underdose_weight = opt_params['ptv_underdose_weight'] if 'ptv_underdose_weight' in opt_params else 100000
-        # smoothness_weight = opt_params['smoothness_weight'] if 'smoothness_weight' in opt_params else 10
-        # total_oar_weight = opt_params['total_oar_weight'] if 'total_oar_weight' in opt_params else 10
-
         # Construct optimization problem
-        prob = cp.Problem(cp.Minimize(0))  # create empty problem
-        self.prob = prob
+        obj = []
+        constraints = []
+        x = cp.Variable(A.shape[1], pos=True, name='x')
 
-        # Construct the problem.
-        if max_constraints is not None and mean_constraints is not None and obj_from_file is not None:
-            self.x = cp.Variable(A.shape[1], pos=True, name='x')
+        self.vars = {'x': x}
 
+        # Generating objective functions
         print('Objective Start')
-        if obj_from_file is not None:
-            f = open(obj_from_file)
-            obj_params = json.load(f)
-            for i in range(len(obj_params)):
-                if obj_params[i]['type'] == 'overdose-quadratic':
-                    struct = obj_params[i]['parameters']['structure_name']
-                    pres_per_frac = obj_params[i]['parameters']['dose_gy']/my_plan.get_num_of_fractions()
-                    weight = obj_params[i]['parameters']['weight']
-                    self.add_overdose_quad(struct=struct, dose_gy=pres_per_frac, weight=weight)
-                elif obj_params[i]['type'] == 'underdose-quadratic':
-                    struct = obj_params[i]['parameters']['structure_name']
-                    pres_per_frac = obj_params[i]['parameters']['dose_gy'] / my_plan.get_num_of_fractions()
-                    weight = obj_params[i]['parameters']['weight']
-                    self.add_underdose_quad(struct=struct, dose_gy=pres_per_frac, weight=weight)
-                elif obj_params[i]['type'] == 'quadratic':
-                    struct = obj_params[i]['parameters']['structure_name']
-                    weight = obj_params[i]['parameters']['weight']
-                    if struct == 'NON-TARGET':
-                        all_vox = np.arange(A.shape[0])
-                        oar_voxels = all_vox[~np.isin(np.arange(A.shape[0]), st.get_opt_voxels_idx('PTV'))]
-                        oar_weights = np.ones(A[oar_voxels, :].shape[0])
-                        self.add_quad(voxels=oar_voxels, voxels_weight=weight*oar_weights)
-                    else:
-                        self.add_quad(struct=struct, weight=weight)
-                elif obj_params[i]['type'] == 'smoothness-quadratic':
-                    weight = obj_params[i]['parameters']['weight']
-                    self.add_smoothness_quad(weight=weight)
-
-        # self.add_overdose_quad(struct='PTV', dose_gy=pres_per_frac, weight=ptv_overdose_weight)
-        # self.add_underdose_quad(struct='PTV', dose_gy=pres_per_frac, weight=ptv_underdose_weight)
-        # self.add_quad(voxels=oar_voxels, voxels_weight=oar_weights * total_oar_weight)
-        # self.add_smoothness_quad(weight=smoothness_weight)
+        for i in range(len(obj_funcs)):
+            if obj_funcs[i]['type'] == 'quadratic-overdose':
+                if obj_funcs[i]['structure_name'] in my_plan.structures.get_structures():
+                    struct = obj_funcs[i]['structure_name']
+                    dose_gy = self.get_num(obj_funcs[i]['dose_gy']) / clinical_criteria.get_num_of_fractions()
+                    dO = cp.Variable(len(st.get_opt_voxels_idx(struct)), pos=True)
+                    obj += [(1 / len(st.get_opt_voxels_idx(struct))) *
+                            (obj_funcs[i]['weight'] * cp.sum_squares(dO))]
+                    constraints += [A[st.get_opt_voxels_idx(struct), :] @ x <= dose_gy + dO]
+            elif obj_funcs[i]['type'] == 'quadratic-underdose':
+                if obj_funcs[i]['structure_name'] in my_plan.structures.get_structures():
+                    struct = obj_funcs[i]['structure_name']
+                    dose_gy = self.get_num(obj_funcs[i]['dose_gy']) / clinical_criteria.get_num_of_fractions()
+                    dU = cp.Variable(len(st.get_opt_voxels_idx(struct)), pos=True)
+                    obj += [(1 / len(st.get_opt_voxels_idx(struct))) *
+                            (obj_funcs[i]['weight'] * cp.sum_squares(dU))]
+                    constraints += [A[st.get_opt_voxels_idx(struct), :] @ x >= dose_gy - dU]
+            elif obj_funcs[i]['type'] == 'quadratic':
+                if obj_funcs[i]['structure_name'] in my_plan.structures.get_structures():
+                    struct = obj_funcs[i]['structure_name']
+                    obj += [(1 / len(st.get_opt_voxels_idx(struct))) * (
+                            obj_funcs[i]['weight'] * cp.sum_squares(A[st.get_opt_voxels_idx(struct), :] @ x))]
+            elif obj_funcs[i]['type'] == 'quadratic-smoothness':
+                [Qx, Qy, num_rows, num_cols] = self.get_smoothness_matrix(inf_matrix.beamlets_dict)
+                smoothness_X_weight = 0.6
+                smoothness_Y_weight = 0.4
+                obj += [obj_funcs[i]['weight'] * (smoothness_X_weight * (1 / num_cols) * cp.sum_squares(Qx @ x) +
+                                                  smoothness_Y_weight * (1 / num_rows) * cp.sum_squares(Qy @ x))]
 
         print('Objective done')
+
         print('Constraints Start')
 
+        # add optimization constraints if present in opt params
+        for param in opt_params_constraints:
+            # add constraint
+            if param['structure_name'] in my_plan.structures.get_structures():
+                parameters = {'structure_name': param['structure_name']}
+                # total_pres = self.get_prescription()
+                if 'max' in param['type']:
+                    opt_constraints = {'limit_dose_gy': self.get_num(param['upper_limit'])}
+                    clinical_criteria.add_criterion(criterion='max_dose', parameters=parameters,
+                                                    constraints=opt_constraints)
+                if 'mean' in param['type']:
+                    opt_constraints = {'limit_dose_gy': self.get_num(param['upper_limit'])}
+                    clinical_criteria.add_criterion(criterion='mean_dose', parameters=parameters,
+                                                    constraints=opt_constraints)
+
+        # get max and mean constraints
+        max_constraints = clinical_criteria.get_criteria(
+            name='max_dose')  # returns all the max dose criteria as a list
+        mean_constraints = clinical_criteria.get_criteria(
+            name='mean_dose')  # returns all the mean dose criteria as a list
+
+        # Adding max constraints
         for i in range(len(max_constraints)):
             if 'max_dose' in max_constraints[i]['name']:
                 if 'limit_dose_gy' in max_constraints[i]['constraints']:
                     limit = max_constraints[i]['constraints']['limit_dose_gy']
                     org = max_constraints[i]['parameters']['structure_name']
-                    if org != 'GTV' or org != 'CTV':
-                        self.add_max(struct=org, dose_gy=(limit / num_fractions))
+                    if org != 'GTV' and org != 'CTV':
+                        if org in my_plan.structures.structures_dict['name']:
+                            constraints += [A[st.get_opt_voxels_idx(org), :] @ x <= limit / num_fractions]
+                        else:
+                            print('Structure {} not available!'.format(org))
+
+        # Adding mean constraints
         for i in range(len(mean_constraints)):
             if 'mean_dose' in mean_constraints[i]['name']:
                 if 'limit_dose_gy' in mean_constraints[i]['constraints']:
                     limit = mean_constraints[i]['constraints']['limit_dose_gy']
                     org = mean_constraints[i]['parameters']['structure_name']
                     # mean constraints using voxel weights
-                    self.add_mean(struct=org, dose_gy=(limit / num_fractions))
+                    if org in my_plan.structures.structures_dict['name']:
+                        constraints += [(1 / sum(st.get_opt_voxels_volume_cc(org))) *
+                                        (cp.sum((cp.multiply(st.get_opt_voxels_volume_cc(org), A[st.get_opt_voxels_idx(org),
+                                                                                          :] @ x)))) <= limit / num_fractions]
+
+                    else:
+                        print('Structure {} not available!'.format(org))
+
+        self.obj = obj
+        self.constraints = constraints
+
         print('Constraints done')
 
+    def create_rinds(self, rind_params):
+        # create rinds for optimization
+        ct_to_dose_map = self.inf_matrix.opt_voxels_dict['ct_to_dose_voxel_map'][0]
+        dose_mask = ct_to_dose_map >= 0
+        dose_mask = dose_mask.astype(int)
+        self.my_plan.structures.create_structure('dose_mask', dose_mask)
+
+        print('creating rinds.. This step may take some time due to dilation')
+        for ind, param in enumerate(rind_params):
+            rind_name = param['name']
+            first_dummy_name = '{}_{}'.format(param['ref_structure'], param['margin_start_mm'])
+            second_dummy_name = '{}_{}'.format(param['ref_structure'], param['margin_end_mm'])
+            self.my_plan.structures.expand(param['ref_structure'], margin_mm=param['margin_start_mm'],
+                                           new_struct_name=first_dummy_name)
+            if param['margin_end_mm'] == 'inf':
+                param['margin_end_mm'] = 500
+            self.my_plan.structures.expand(param['ref_structure'], margin_mm=param['margin_end_mm'],
+                                           new_struct_name=second_dummy_name)
+            self.my_plan.structures.subtract(second_dummy_name, first_dummy_name, new_struct_name=rind_name)
+            self.my_plan.structures.delete_structure(first_dummy_name)
+            self.my_plan.structures.delete_structure(second_dummy_name)
+            self.my_plan.structures.intersect(rind_name, 'dose_mask', new_struct_name=rind_name)
+        self.my_plan.structures.delete_structure('dose_mask')
+
+        print('rinds created!!')
+        for param in rind_params:
+            self.inf_matrix.set_opt_voxel_idx(self.my_plan, structure_name=param['name'])
+
     def add_max(self, struct: str, dose_gy: float):
         """
         Add max constraints to the problem
-        :param struct: structure name
+
+        :param struct: struct_name name
         :param dose_gy: dose in Gy per fraction.
         :return:
         """
         A = self.inf_matrix.A
         st = self.inf_matrix
-        x = self.x
+        x = self.vars['x']
 
         max_constraint = [A[st.get_opt_voxels_idx(struct), :] @ x <= dose_gy]
         self.add_constraints(max_constraint)
 
     def add_mean(self, struct: str, dose_gy: float):
         """
         Add mean constraints to the problem
-        :param struct: structure name
+
+        :param struct: struct_name name
         :param dose_gy: dose in Gy per fraction.
         :return:
         """
         A = self.inf_matrix.A
         st = self.inf_matrix
-        x = self.x
+        x = self.vars['x']
 
-        mean_constraint = [(1 / sum(st.get_opt_voxels_size(struct))) *
-                           (cp.sum((cp.multiply(st.get_opt_voxels_size(struct),
+        mean_constraint = [(1 / sum(st.get_opt_voxels_volume_cc(struct))) *
+                           (cp.sum((cp.multiply(st.get_opt_voxels_volume_cc(struct),
                                                 A[st.get_opt_voxels_idx(struct),
                                                 :] @ x)))) <= dose_gy]
         self.add_constraints(mean_constraint)
 
     def add_overdose_quad(self, struct: str, dose_gy: float, weight: float = 10000):
         """
-        Add quadratic loss for the overdose voxels of the structure
-        :param struct: structure name
+        Add quadratic loss for the overdose voxels of the struct_name
+
+        :param struct: struct_name name
         :param dose_gy: dose in Gy per fraction.
         :param weight: penalty/weight in the objective for overdose
         :return:
         """
         A = self.inf_matrix.A
         st = self.inf_matrix
-        x = self.x
+        x = self.vars['x']
 
         dO = cp.Variable(len(st.get_opt_voxels_idx(struct)), pos=True, name='{}_overdose'.format(struct))
         obj = (1 / len(st.get_opt_voxels_idx(struct))) * (weight * cp.sum_squares(dO))
-        overdose_prob = cp.Problem(cp.Minimize(obj), [A[st.get_opt_voxels_idx('PTV'), :] @ x <= dose_gy + dO])
-        self.prob = self.prob + overdose_prob
+        self.add_objective(obj)
+        self.add_constraints([A[st.get_opt_voxels_idx('PTV'), :] @ x <= dose_gy + dO])
 
     def add_underdose_quad(self, struct: str, dose_gy: float, weight: float = 100000):
         """
-        Add quadratic loss for the underdose voxels of the structure
-        :param struct: structure name
+        Add quadratic loss for the underdose voxels of the struct_name
+
+        :param struct: struct_name name
         :param dose_gy: dose in Gy per fraction.
         :param weight: penalty/weight in the objective for underdose
         :return:
         """
         A = self.inf_matrix.A
         st = self.inf_matrix
-        x = self.x
+        x = self.vars['x']
 
         dU = cp.Variable(len(st.get_opt_voxels_idx(struct)), pos=True, name='{}_underdose'.format(struct))
         obj = (1 / len(st.get_opt_voxels_idx(struct))) * (weight * cp.sum_squares(dU))
-        underdose_prob = cp.Problem(cp.Minimize(obj), [A[st.get_opt_voxels_idx('PTV'), :] @ x >= dose_gy - dU])
-        self.prob = self.prob + underdose_prob
+        self.add_objective(obj)
+        self.add_constraints([A[st.get_opt_voxels_idx('PTV'), :] @ x >= dose_gy - dU])
 
     def add_quad(self, struct: str = None, voxels: np.ndarray = None, weight: float = 10,
                  voxels_weight: np.ndarray = None):
 
         """
         Add quadratic objective to the optimization problem
-        :param struct: structure for which quadratic loss is added to objective function
+
+        :param struct: struct_name for which quadratic loss is added to objective function
         :param voxels: Default to None. If set, quadratic loss will be added for the given voxels
-        :param weight: Default to 10. penalty in the objective function for the given structure.
+        :param weight: Default to 10. penalty in the objective function for the given struct_name.
         :param voxels_weight: weight for each voxel in the objective function
         :return:
         """
         A = self.inf_matrix.A
         st = self.inf_matrix
-        x = self.x
+        x = self.vars['x']
 
         obj = 0
         if voxels is not None:
             if voxels_weight is None:
                 raise Exception('Please input weight array for the input voxels')
             obj = (1 / A[voxels, :].shape[0]) * cp.sum_squares(
                 cp.multiply(cp.sqrt(voxels_weight), A[voxels, :] @ x))
@@ -238,135 +282,151 @@
             obj = (1 / len(st.get_opt_voxels_idx(struct))) * (
                     weight * cp.sum_squares(A[st.get_opt_voxels_idx(struct), :] @ x))
         self.add_objective(obj)
 
     def add_smoothness_quad(self, weight: int = 10, smoothness_X_weight: int = 0.6, smoothness_Y_weight: int = 0.4):
         """
         Add quadratic smoothness to the optimization problem
+
         :param weight: smoothness weight
         :param smoothness_X_weight: weight in X direction of MLC (parallel to MLC)
         :param smoothness_Y_weight: weight in Y direction of MLC (perpendicular to MLC)
         :return:
         """
 
         st = self.inf_matrix
-        x = self.x
+        x = self.vars['x']
 
         [Qx, Qy, num_rows, num_cols] = self.get_smoothness_matrix(st.beamlets_dict)
         obj = weight * (
                 smoothness_X_weight * (1 / num_cols) * cp.sum_squares(Qx @ x) + smoothness_Y_weight * (1 / num_rows)
                 * cp.sum_squares(Qy @ x))
         self.add_objective(obj)
 
     def add_constraints(self, constraints: list):
         """
-        Add constraint to the problem
+        Add constraint to the constraint list of problem
+
         :param constraints: list of constraints
         :return:
         """
-
-        constraints = cp.Problem(cp.Minimize(0), constraints)
-        self.prob = self.prob + constraints
+        self.constraints += constraints
 
     def add_objective(self, obj):
         """
-        Add objective function to the problem
+        Add objective function to objective list of the problem
+
         :param obj: objective function expression using cvxpy
         :return:
         """
-        if isinstance(obj, list):
-            obj = sum(obj)
-        obj = cp.Problem(cp.Minimize(obj))
-        self.prob = self.prob + obj
+        if not isinstance(obj, list):
+            obj = [obj]
+
+        self.obj += obj
 
     def add_boo(self, num_beams: int):
         """
         Select optimal beams from set of beams using MIP
+
         :param num_beams: number of beams to be selected
         :return:
         """
         st = self.inf_matrix
-        x = self.x
+        x = self.vars['x']
 
         #  Constraints for selecting beams
         # binary variable for selecting beams
         b = cp.Variable(len(st.beamlets_dict), boolean=True)
 
         constraints = []
         constraints += [cp.sum(b) <= num_beams]
         for i in range(len(st.beamlets_dict)):
-            start_beamlet = st.beamlets_dict[i]['start_beamlet']
-            end_beamlet = st.beamlets_dict[i]['end_beamlet']
+            start_beamlet = st.beamlets_dict[i]['start_beamlet_idx']
+            end_beamlet_idx = st.beamlets_dict[i]['end_beamlet_idx']
             M = 50  # upper bound on the beamlet intensity
-            constraints += [x[start_beamlet:end_beamlet] <= b[i] * M]
+            constraints += [x[start_beamlet:end_beamlet_idx] <= b[i] * M]
 
-        boo_constraint = cp.Problem(cp.Minimize(0), constraints)
-        self.prob = self.prob + boo_constraint
+        self.add_constraints(constraints)
 
-    def solve(self, *args, **kwargs):
+    def solve(self, *args, **kwargs) -> dict:
         """
-        Calls cvxpy solve methods
-        :return:
-        """
-        self.prob.solve(*args, **kwargs)
+                Return optimal solution and influence matrix associated with it in the form of dictionary
+
+                :Example
+                        dict = {"optimal_fluence": [..],
+                        "inf_matrix": my_plan.inf_marix
+                        }
+
+                :return: solution dictionary
+                """
+
+        problem = cp.Problem(cp.Minimize(sum(self.obj)), constraints=self.constraints)
+        problem.solve(*args, **kwargs)
+        return {'optimal_intensity': self.vars['x'].value, 'inf_matrix': self.inf_matrix}
 
     def get_sol(self) -> dict:
         """
         Return optimal solution and influence matrix associated with it in the form of dictionary
-        :return:
+
+        :Example
+                dict = {"optimal_fluence": [..],
+                "inf_matrix": my_plan.inf_marix
+                }
+
+        :return: solution dictionary
         """
-        return {'optimal_intensity': self.x.value, 'inf_matrix': self.inf_matrix}
+        return {'optimal_intensity': self.vars['x'].value, 'inf_matrix': self.inf_matrix}
 
     def add_dvh(self, dvh_constraint: list):
 
         A = self.inf_matrix.A
         st = self.inf_matrix
-        x = self.x
+        x = self.vars['x']
 
         import pandas as pd
         df_dvh_criteria = pd.DataFrame()
         count = 0
-        criteria = self.my_plan.clinical_criteria.clinical_criteria_dict['criteria']
+        criteria = self.clinical_criteria.clinical_criteria_dict['criteria']
         for i in range(len(dvh_constraint)):
             if 'dose_volume' in dvh_constraint[i]['name']:
                 limit_key = self.matching_keys(dvh_constraint[i]['constraints'], 'limit')
                 if limit_key in dvh_constraint[i]['constraints']:
-                    df_dvh_criteria.at[count, 'structure'] = dvh_constraint[i]['parameters']['structure_name']
+                    df_dvh_criteria.at[count, 'structure_name'] = dvh_constraint[i]['parameters']['structure_name']
                     df_dvh_criteria.at[count, 'dose_gy'] = dvh_constraint[i]['parameters']['dose_gy']
 
-                    # getting max dose_1d for the same structure
+                    # getting max dose_1d for the same struct_name
                     max_dose_struct = 1000
                     for j in range(len(criteria)):
                         if 'max_dose' in criteria[j]['name']:
                             if 'limit_dose_gy' in criteria[j]['constraints']:
                                 org = criteria[j]['parameters']['structure_name']
                                 if org == dvh_constraint[i]['parameters']['structure_name']:
                                     max_dose_struct = criteria[j]['constraints']['limit_dose_gy']
                     df_dvh_criteria.at[count, 'M'] = max_dose_struct - dvh_constraint[i]['parameters']['dose_gy']
                     if 'perc' in limit_key:
                         df_dvh_criteria.at[count, 'vol_perc'] = dvh_constraint[i]['constraints'][limit_key]
                     count = count + 1
 
         # binary variable for dvh constraints
         b_dvh = cp.Variable(
-            len(np.concatenate([st.get_opt_voxels_idx(org) for org in df_dvh_criteria.structure.to_list()])),
+            len(np.concatenate([st.get_opt_voxels_idx(org) for org in df_dvh_criteria.structure_name.to_list()])),
             boolean=True)
 
         start = 0
         constraints = []
         for i in range(len(df_dvh_criteria)):
-            struct, limit, v, M = df_dvh_criteria.loc[i, 'structure'], df_dvh_criteria.loc[i, 'dose_gy'], \
+            struct, limit, v, M = df_dvh_criteria.loc[i, 'structure_name'], df_dvh_criteria.loc[i, 'dose_gy'], \
                                   df_dvh_criteria.loc[i, 'vol_perc'], df_dvh_criteria.loc[i, 'M']
             end = start + len(st.get_opt_voxels_idx(struct))
             frac = self.my_plan.structures.get_fraction_of_vol_in_calc_box(struct)
             constraints += [
                 A[st.get_opt_voxels_idx(struct), :] @ x <= limit / self.my_plan.get_num_of_fractions()
                 + b_dvh[start:end] * M / self.my_plan.get_num_of_fractions()]
-            constraints += [b_dvh @ st.get_opt_voxels_size(struct) <= (v / frac) / 100 * sum(
-                st.get_opt_voxels_size(struct))]
+            constraints += [b_dvh @ st.get_opt_voxels_volume_cc(struct) <= (v / frac) / 100 * sum(
+                st.get_opt_voxels_volume_cc(struct))]
             start = end
         self.add_constraints(constraints=constraints)
 
     @staticmethod
     def get_smoothness_matrix(beamReq: List[dict]) -> (np.ndarray, np.ndarray, int, int):
         """
         Create smoothness matrix so that adjacent beamlets are smooth out to reduce MU
@@ -378,20 +438,20 @@
 
         :Example:
         Qx = [[1 -1 0 0 0 0]
               [0 0 1 -1 0 0]
               [0 0 0 0 1 -1]]
 
         """
-        sRow = np.zeros((beamReq[-1]['end_beamlet'] + 1, beamReq[-1]['end_beamlet'] + 1), dtype=int)
-        sCol = np.zeros((beamReq[-1]['end_beamlet'] + 1, beamReq[-1]['end_beamlet'] + 1), dtype=int)
+        sRow = np.zeros((beamReq[-1]['end_beamlet_idx'] + 1, beamReq[-1]['end_beamlet_idx'] + 1), dtype=int)
+        sCol = np.zeros((beamReq[-1]['end_beamlet_idx'] + 1, beamReq[-1]['end_beamlet_idx'] + 1), dtype=int)
         num_rows = 0
         num_cols = 0
         for b in range(len(beamReq)):
-            beam_map = beamReq[b]['beamlet_idx_2dgrid']
+            beam_map = beamReq[b]['beamlet_idx_2d_finest_grid']
 
             rowsNoRepeat = [0]
             for i in range(1, np.size(beam_map, 0)):
                 if (beam_map[i, :] != beam_map[rowsNoRepeat[-1], :]).any():
                     rowsNoRepeat.append(i)
             colsNoRepeat = [0]
             for j in range(1, np.size(beam_map, 1)):
@@ -427,71 +487,23 @@
                     DN = beam_map[r + 1, c]
                     if ind * DN >= 0:
                         sCol[ind, ind] = int(1)
                         sCol[ind, DN] = int(-1)
         return sRow, sCol, num_rows, num_cols
 
     @staticmethod
-    def create_rinds(my_plan, inf_matrix=None, size_mm: list = None, base_structure='PTV'):
-        """
-        :param inf_matrix: object of class inf_matrix
-        :param my_plan: object of class Plan
-        :param size_mm: size in mm. default size = [5,5,20,30, inf]. It means rind_0 is 5mm after PTV, rind_2 is 5 mm after rind_1, and so on..
-        :param base_structure: structure from which rinds should be created
-        :return: save rinds to plan object
-        """
-        if size_mm is None:
-            size_mm = [5, 5, 20, 30, 500]
-        if inf_matrix is None:
-            inf_matrix = my_plan.inf_matrix
-        print('creating rinds of size {} mm ..'.format(size_mm))
-        if isinstance(size_mm, np.ndarray):
-            size_mm = list(size_mm)
-        ct_to_dose_map = inf_matrix.opt_voxels_dict['ct_to_dose_voxel_map'][0]
-        dose_mask = ct_to_dose_map >= 0
-        dose_mask = dose_mask.astype(int)
-        my_plan.structures.create_structure('dose_mask', dose_mask)
-
-        for ind, s in enumerate(size_mm):
-            rind_name = 'RIND_{}'.format(ind)
-            dummy_name = 'dummy_{}'.format(ind)
-            if ind == 0:
-                my_plan.structures.expand(base_structure, margin_mm=s, new_structure=dummy_name)
-                my_plan.structures.subtract(dummy_name, base_structure, str1_sub_str2=rind_name)
-                # inf_matrix.set_opt_voxel_idx(my_plan, struct=rind_name)
-            else:
-                # prev_rind_name = 'RIND_{}'.format(ind - 1)
-                prev_dummy_name = 'dummy_{}'.format(ind - 1)
-                my_plan.structures.expand(prev_dummy_name, margin_mm=s, new_structure=dummy_name)
-                my_plan.structures.subtract(dummy_name, prev_dummy_name, str1_sub_str2=rind_name)
-                my_plan.structures.delete_structure(prev_dummy_name)
-                # for the last delete dummy
-                if ind == len(size_mm) - 1:
-                    my_plan.structures.delete_structure(dummy_name)  # delete dummy structure for last rind
-            my_plan.structures.intersect(rind_name, 'dose_mask', str1_and_str2=rind_name)
-
-        my_plan.structures.delete_structure('dose_mask')
-        # inf_matrix.set_opt_voxel_idx(my_plan, struct=rind_name)
-        print('rinds created!!')
-
-    @staticmethod
-    def set_rinds_opt_voxel_idx(plan_obj: Plan, inf_matrix: InfluenceMatrix):
-        """
-
-        :param plan_obj: object of class plan
-        :param inf_matrix: object of class influence matrix
-        :return: set rinds index based upon the influence matrix
-        """
-        rinds = [rind for idx, rind in enumerate(plan_obj.structures.structures_dict['name']) if 'RIND' in rind]
-        for rind in rinds:
-            inf_matrix.set_opt_voxel_idx(plan_obj, structure_name=rind)
-
-    @staticmethod
     def matching_keys(dictionary, search_string):
         get_key = None
         for key, val in dictionary.items():
             if search_string in key:
                 get_key = key
         if get_key is not None:
             return get_key
         else:
             return ''
+
+    def get_num(self, string: Union[str, float]):
+        if "prescription_gy" in string:
+            prescription_gy = self.prescription_gy
+            return eval(string)
+        elif isinstance(string, float) or isinstance(string, int):
+            return string
```

### Comparing `portpy-0.0.1/portpy/photon/influence_matrix.py` & `portpy-0.0.2/portpy/photon/influence_matrix.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,26 +3,29 @@
 from scipy import sparse
 from copy import deepcopy
 from scipy.sparse import csr_matrix
 import matplotlib.pyplot as plt
 import itertools
 from patchify import patchify
 from typing import List, Union
+from .ct import CT
+from .beam import Beams
+from .structures import Structures
 
 
 class InfluenceMatrix:
     """
     class of influence matrix
 
     - **Attributes** ::
 
         :param beamlet_width_mm: The width of each beamlet in millimeters. Default is 2.5. Must be a multiple of 2.5.
         :param beamlet_height_mm: The height of each beamlet in millimeters. Default is 2.5. Must be a multiple of 2.5.
-        :param down_sample_xyz: A list of integers representing the downsampling factors for the x, y, and z axes. When set to None, the original optimization voxel resolution will be used.
-        :param structure: The target structure for creating the beamlets in the influence matrix. Default is 'PTV'.
+        :param _down_sample_xyz: A list of integers representing the downsampling factors for the x, y, and z axes. When set to None, the original optimization voxel resolution will be used.
+        :param structure: The target struct_name for creating the beamlets in the influence matrix. Default is 'PTV'.
         :param opt_voxels_dict: A dictionary containing the voxels that were used in the optimization process.
         :param beamlets_dict: A dictionary containing the information about beamlets used in the plan.
         :param opt_beamlets_PTV_margin_mm: A float value representing the margin_mm around the PTV that was used in creating beamlets
         :param A: influence matrix that is generated by the get_influence_matrix() method.
         :param dose_3d: 3D dose_1d distribution. It is saved as attribute once the method dose_1d_to_3d() is called
                 so that it doesnt have to be computed again
 
@@ -34,76 +37,82 @@
         :fluence_2d_to_1d(fluence_2d)
             Create vector of intensities from 2d fluence maps
         :fluence_1d_to_2d(fluence_1d)
             From vector of intensities create 2d fluence maps
 
     """
 
-    def __init__(self, plan_obj,
-                 beamlet_width_mm: float = 2.5, beamlet_height_mm: float = 2.5, opt_vox_xyz_res_mm: List[float] = None,
-                 is_full: bool = False, structure: str = 'PTV') -> None:
+    def __init__(self, ct: CT, structs: Structures, beams: Beams,
+                 beamlet_width_mm: float = None, beamlet_height_mm: float = None, opt_vox_xyz_res_mm: List[float] = None,
+                 is_full: bool = False, target_structure: str = 'PTV', opt_beamlets_PTV_margin_mm: float = 3) -> None:
         """
         Create a influence matrix object for Influence Matrix class based upon beamlet resolution and down-sampling_xyz ratio
 
         :param plan_obj: object of class Plan
         :param beamlet_width_mm: beamlet width in mm. It should be multiple of 2.5, defaults to 2.5
         :param beamlet_height_mm: beamlet height in mm. It should be multiple of 2.5, defaults to 2.5
-        :param structure: target structure for creating BEV beamlets, defaults to 'PTV'
+        :param structure: target struct_name for creating BEV beamlets, defaults to 'PTV'
         :param opt_vox_xyz_res_mm: It down-samples optimization voxels as factor of ct resolution
                 e.g. opt_vox_xyz_res = [5*ct.res.x,5*ct.res.y,1*ct.res.z]. It will down-sample optimization voxels with 5 * ct res. in x direction, 5 * ct res. in y direction and 1*ct res. in z direction.
                 defaults to None. When None it will use the original optimization voxel resolution.
         :param is_full: Load full or sparse matrix. defaults to False. If True, will load full matrix
 
         """
-
-        if beamlet_width_mm % 2.5 == 0 and beamlet_height_mm % 2.5 == 0:
-            self.beamlet_width_mm = beamlet_width_mm
-            self.beamlet_height_mm = beamlet_height_mm
+        if beamlet_width_mm is None and beamlet_height_mm is None:
+            self.beamlet_width_mm = beams.get_beamlet_width()
+            self.beamlet_height_mm = beams.get_beamlet_height()
         else:
-            raise ValueError('beamlet_width_mm and beamlet_height_mm should be multiple of 2.5')
+            if beamlet_width_mm % 2.5 == 0 and beamlet_height_mm % 2.5 == 0:
+                self.beamlet_width_mm = beamlet_width_mm
+                self.beamlet_height_mm = beamlet_height_mm
+            else:
+                raise ValueError('beamlet_width_mm and beamlet_height_mm should be multiple of 2.5')
+        self._beams = beams
+        self._structs = structs
+        self._ct = ct
 
         down_sample_xyz = None  # Temporary variable to check if we want to down sample or not
         if opt_vox_xyz_res_mm is not None:
-            down_sample_xyz = [round(i / j) for i, j in zip(opt_vox_xyz_res_mm, plan_obj.ct['resolution_xyz_mm'])]
+            down_sample_xyz = [round(i / j) for i, j in zip(opt_vox_xyz_res_mm, ct.get_ct_res_xyz_mm())]
             if np.all(np.array(down_sample_xyz) == 1):  # if all are 1 then no down sample
                 down_sample_xyz = None
 
-        self.down_sample_xyz = down_sample_xyz
+        self._down_sample_xyz = down_sample_xyz
         self.is_full = is_full
+
         # create deepcopy of the object or else it will modify the my_plan object
-        if hasattr(plan_obj.structures, 'opt_voxels_dict'):
-            self.opt_voxels_dict = deepcopy(plan_obj.structures.opt_voxels_dict)
-            del plan_obj.structures.opt_voxels_dict  # remove opt_voxels_dict from structures
+        if hasattr(structs, 'opt_voxels_dict'):
+            self.opt_voxels_dict = deepcopy(structs.opt_voxels_dict)
+            # del structs.opt_voxels_dict  # remove opt_voxels_dict from structures
         else:
-            self.opt_voxels_dict = deepcopy(plan_obj.inf_matrix.opt_voxels_dict)
+            self.opt_voxels_dict = deepcopy(self.opt_voxels_dict)
 
-        if 'beamlets' in plan_obj.beams.beams_dict:
-            self.beamlets_dict = deepcopy(plan_obj.beams.beams_dict['beamlets'])
+        # creating deepcopy so that it doesnt modify beams object
+        if 'beamlets' in beams.beams_dict:
+            self.beamlets_dict = deepcopy(beams.beams_dict['beamlets'])
         else:
-            self.beamlets_dict = deepcopy(plan_obj.inf_matrix.beamlets_dict['beamlets'])
+            self.beamlets_dict = deepcopy(self.beamlets_dict['beamlets'])
 
-        for i in range(len(plan_obj.beams.beams_dict['ID'])):
-            self.beamlets_dict[i]['beam_id'] = plan_obj.beams.beams_dict['ID'][i]  # save beam_id in beamlet_dict
+        for i in range(len(beams.beams_dict['ID'])):
+            self.beamlets_dict[i]['beam_id'] = beams.beams_dict['ID'][i]  # save beam_id in beamlet_dict
 
-        self.opt_beamlets_PTV_margin_mm = plan_obj.opt_beamlets_PTV_margin_mm
-        self.opt_voxels_dict['ct_origin_xyz_mm'] = plan_obj.ct['origin_xyz_mm']  # store ct origin from plan
+        self.opt_beamlets_PTV_margin_mm = opt_beamlets_PTV_margin_mm
+        self.opt_voxels_dict['ct_origin_xyz_mm'] = ct.ct_dict['origin_xyz_mm']  # store ct origin from plan
         print('Creating BEV..')
-        self.preprocess_beams(plan_obj, structure=structure)
-        if self.down_sample_xyz is not None:
-            self.pre_process_voxels(
-                plan_obj=plan_obj)  # create new optimization voxel indices based on down-sample resolution
+        self.preprocess_beams(structure=target_structure)
+        if self._down_sample_xyz is not None:
+            self.pre_process_voxels()  # create new optimization voxel indices based on down-sample resolution
 
         if not self.is_full:
             print('Loading sparse influence matrix...')
-            self.A = self.get_influence_matrix(plan_obj)  # create sparse influence matrix
-            self.sparse_tol = float(plan_obj.beams.beams_dict['influenceMatrixSparse_tol'][0])
+            self.A = self.get_influence_matrix()  # create sparse influence matrix
+            self.sparse_tol = float(beams.beams_dict['influenceMatrixSparse_tol'][0])
         else:
             print('Loading full influence matrix..')
-            self.A = self.get_influence_matrix(plan_obj, self.is_full)  # create full matrix
-        self.dose_3d = None
+            self.A = self.get_influence_matrix(self.is_full)  # create full matrix
         self._vox_map = None
         self._vox_weights = None
         print('Done')
 
     def get_voxel_info(self, row_number):
         row_dict = {}
         if row_number <= self.A.shape[0]:
@@ -130,18 +139,18 @@
         """
 
         :param col_number: col number/beamlet number in influence matrix
         :return: dictionary containing information about the beamlet
         """
         col_dict = {}
         for ind in range(len(self.beamlets_dict)):
-            if col_number in range(self.beamlets_dict[ind]['start_beamlet'],
-                                   self.beamlets_dict[ind]['end_beamlet'] + 1):
+            if col_number in range(self.beamlets_dict[ind]['start_beamlet_idx'],
+                                   self.beamlets_dict[ind]['end_beamlet_idx'] + 1):
                 if ind > 0:
-                    prev_beam_beamlet = self.beamlets_dict[ind - 1]['end_beamlet'] + 1
+                    prev_beam_beamlet = self.beamlets_dict[ind - 1]['end_beamlet_idx'] + 1
                 else:
                     prev_beam_beamlet = 0
                 col_dict['beam_id'] = self.beamlets_dict[ind]['beam_id']
                 col_dict['position_x_mm'] = self.beamlets_dict[ind]['position_x_mm'][0][col_number - prev_beam_beamlet]
                 col_dict['position_y_mm'] = self.beamlets_dict[ind]['position_y_mm'][0][col_number - prev_beam_beamlet]
                 col_dict['width_mm'] = self.beamlets_dict[ind]['width_mm'][0][col_number - prev_beam_beamlet]
                 col_dict['height_mm'] = self.beamlets_dict[ind]['height_mm'][0][col_number - prev_beam_beamlet]
@@ -164,27 +173,24 @@
                 dose_1d = sol['inf_matrix'].A * sol['optimal_intensity']  # multiply it with num fractions
             else:
                 dose_1d = sol['dose_1d']
         dose_3d = np.zeros_like(dose_vox_map, dtype='float32')
         inds = np.unique(dose_vox_map[dose_vox_map >= 0])
         a = np.where(np.isin(dose_vox_map, inds))
         dose_3d[a] = dose_1d[dose_vox_map[a]]
-        self.dose_3d = dose_3d
         return dose_3d
 
     def dose_3d_to_1d(self, dose_3d: np.ndarray) -> np.array:
         """
         Get dose_1d in 1d voxels for the given influence matrix from 3d dose_1d
 
         :param dose_3d: 3d dose_1d
         :return: dose_1d in 1d voxel indices
         """
         dose_vox_map = self.opt_voxels_dict['ct_to_dose_voxel_map'][0]
-        if dose_3d is None:
-            dose_3d = self.dose_3d
         inds = np.unique(dose_vox_map[dose_vox_map >= 0])
         dose_1d = np.zeros_like(inds, dtype=float)
         a = np.where(np.isin(dose_vox_map, inds))
         dose_1d[dose_vox_map[a]] = dose_3d[a]
         return dose_1d
 
     def fluence_2d_to_1d(self, fluence_2d: List[np.ndarray]) -> np.array:
@@ -192,15 +198,15 @@
         Create vector of intensities from 2d fluence maps
 
         :param fluence_2d: 2d fluence as list of nd array with same length as number of beams_dict
         :return: fluence in 1d for beamlet indices
         """
         fluence_1d = np.zeros((self.A.shape[1]))
         for ind in range(len(self.beamlets_dict)):
-            maps = self.beamlets_dict[ind]['beamlet_idx_2dgrid']
+            maps = self.beamlets_dict[ind]['beamlet_idx_2d_finest_grid']
             numRows = np.size(maps, 0)
             numCols = np.size(maps, 1)
             # wMaps = np.zeros((numRows, numCols))
             for r in range(numRows):
                 for c in range(numCols):
                     if maps[r, c] >= 0:
                         curr = maps[r, c]
@@ -217,148 +223,204 @@
 
         """
         if fluence_1d is None:
             fluence_1d = sol['optimal_intensity']
 
         wMaps = []
         for ind in range(len(self.beamlets_dict)):
-            maps = self.beamlets_dict[ind]['beamlet_idx_2dgrid']
+            maps = self.beamlets_dict[ind]['beamlet_idx_2d_finest_grid']
             numRows = np.size(maps, 0)
             numCols = np.size(maps, 1)
             wMaps.append(np.zeros((numRows, numCols)))
             # wMaps = np.zeros((numRows, numCols))
             for r in range(numRows):
                 for c in range(numCols):
                     if maps[r, c] >= 0:
                         curr = maps[r, c]
                         wMaps[ind][r, c] = fluence_1d[curr]
                         # wMaps[r, c] = optimal_intensity[curr]
 
         return wMaps
 
-    def get_influence_matrix(self, plan, is_full=False):
+    @staticmethod
+    def sol_change_inf_matrix(sol: dict, inf_matrix) -> dict:
+        """
+        Create a new solution by changing the basis of current solution.
+        It will create a solution with same number of beamlets and voxels as inf_matrix
+
+
+        :param sol: solution for which influence matrix is changed
+        :param inf_matrix: object of class Influence matrix
+        :return: new solution dictionary having same number of beamlets and voxels as inf_matrix
+        """
+        new_sol = dict()
+        if sol['optimal_intensity'].shape[0] < inf_matrix.A.shape[1]:
+            optimal_intensity = sol['inf_matrix'].fluence_1d_to_2d(fluence_1d=sol['optimal_intensity'])
+            new_sol['optimal_intensity'] = inf_matrix.fluence_2d_to_1d(optimal_intensity)
+        elif sol['optimal_intensity'].shape[0] == inf_matrix.A.shape[1]:
+            new_sol['optimal_intensity'] = sol['optimal_intensity']
+        else:
+            raise ValueError("Beamlet resolution should be greater than or equal to beamlets for inf_matrix")
+
+        # new_sol['dose_1d'] = inf_matrix.A * new_sol['optimal_intensity']
+
+        # dose_3d = sol['inf_matrix'].dose_1d_to_3d(dose_1d=sol['dose_1d'])
+        # new_sol['dose_1d'] = inf_matrix.dose_3d_to_1d(dose_3d=dose_3d)
+
+        new_sol['inf_matrix'] = inf_matrix
+        return new_sol
+
+    def create_down_sample(self, beamlet_width_mm: float = None, beamlet_height_mm: float = None,
+                           opt_vox_xyz_res_mm: List[float] = None,
+                           overwrite: bool = False, remove_corner_beamlets: bool = False):
+        if overwrite:
+            new_inf_matrix = self
+        else:
+            new_inf_matrix = deepcopy(self)
+        if beamlet_width_mm is None:
+            beamlet_width_mm = self.beamlet_width_mm
+            beamlet_height_mm = self.beamlet_height_mm
+        new_inf_matrix.beamlet_width_mm = beamlet_width_mm
+        new_inf_matrix.beamlet_height_mm = beamlet_height_mm
+        new_inf_matrix.beamlets_dict = deepcopy(self._beams.beams_dict['beamlets'])
+        for i in range(len(self._beams.beams_dict['ID'])):
+            new_inf_matrix.beamlets_dict[i]['beam_id'] = deepcopy(self._beams.beams_dict['ID'][i])  # save beam_id in beamlet_dict
+
+        for i in range(len(new_inf_matrix.beamlets_dict)):
+            new_inf_matrix.beamlets_dict[i]['beamlet_idx_2d_finest_grid'] = deepcopy(self.beamlets_dict[i]['beamlet_idx_2d_finest_grid'])
+        down_sample_xyz = None  # Temporary variable to check if we want to down sample or not
+        if opt_vox_xyz_res_mm is not None:
+            down_sample_xyz = [round(i / j) for i, j in zip(opt_vox_xyz_res_mm, self.opt_voxels_dict['ct_voxel_resolution_xyz_mm'])]
+            if np.all(np.array(down_sample_xyz) == 1):  # if all are 1 then no down sample
+                down_sample_xyz = None
+        new_inf_matrix._down_sample_xyz = down_sample_xyz
+        new_inf_matrix.preprocess_beams(remove_corner_beamlets=remove_corner_beamlets)
+        new_inf_matrix.pre_process_voxels()
+        A = new_inf_matrix.get_influence_matrix(is_full=new_inf_matrix.is_full)
+        new_inf_matrix.A = A
+        return new_inf_matrix
+
+    def get_influence_matrix(self, is_full=False):
         """
+
         Load influence matrix based on the beamlets and voxels.
-        :param plan: object of class Plan
+
+        :param beams: object of class Beams
         :param is_full: get full or sparse matrix. Default to True.
         :return: full or sparse matrix
         """
+        data_beamlet_width = self._beams.get_beamlet_width()
+        data_beamlet_height = self._beams.get_beamlet_height()
+
         if not is_full:
-            if self.beamlet_width_mm > 2.5 or self.beamlet_height_mm > 2.5 or self.down_sample_xyz is not None:
-                inf_matrix_sparse = plan.inf_matrix.A
+            if self.beamlet_width_mm > data_beamlet_width or \
+                    self.beamlet_height_mm > data_beamlet_height or self._down_sample_xyz is not None:
+                inf_matrix_sparse = self.A
             else:
-                inf_matrix_sparse = plan.beams.beams_dict['influenceMatrixSparse']
+                # deepcopy so that it doesnt modify
+                inf_matrix_sparse = deepcopy(self._beams.beams_dict['influenceMatrixSparse'])
+                # if 'influenceMatrixSparse' in self._beams.beams_dict:
+                del self._beams.beams_dict['influenceMatrixSparse']
 
             for ind in range(len(self.beamlets_dict)):
-                # ind = my_plan.beamlets_dict['ID'].index(beam_id)
-                # beamlet_idx_2dgrid = my_plan.get_beamlet_idx_2dgrid(beam_id=beam_id)
-                # opt_beamlets = beamlet_idx_2dgrid[beamlet_idx_2dgrid >= 0]
                 opt_beamlets = self.beamlets_dict[ind]['opt_beamlets_ids']
 
                 if ind == 0:
-                    if self.beamlet_width_mm > 2.5 or self.beamlet_height_mm > 2.5:
+                    if self.beamlet_width_mm > data_beamlet_width or self.beamlet_height_mm > data_beamlet_height:
                         print('parsing influence matrix for beam {}'.format(ind))
-                        # inf_matrix = lil_matrix((influenceMatrixSparse[ind].shape[0], len(opt_beamlets)))
-                        # inf_matrix = sparse.hstack([csr_matrix(influenceMatrixSparse[ind][:, np.unique(opt_beamlets[i])].sum(axis=1)) for i in range(len(opt_beamlets))], format='csr')
                         inf_matrix = sparse.hstack(
                             [csr_matrix(inf_matrix_sparse[:, np.unique(opt_beamlets[i])].sum(axis=1)) for i in
                              range(len(opt_beamlets))], format='csr')
-                        # for i in range(len(opt_beamlets)):
-                        #     inf_matrix[:, i] = influenceMatrixSparse[ind][:, np.unique(opt_beamlets[i])].sum(axis=1)
-                        # inf_matrix = np.vstack([np.sum(influenceMatrixSparse[ind][:, opt_beamlets[n]], 1) for n in range(len(opt_beamlets))]).T
                     else:
-                        if self.down_sample_xyz is None:
+                        if self._down_sample_xyz is None:
                             inf_matrix = inf_matrix_sparse[ind][:, opt_beamlets]
                 else:
-                    if self.beamlet_width_mm > 2.5 or self.beamlet_height_mm > 2.5:
+                    if self.beamlet_width_mm > data_beamlet_width or self.beamlet_height_mm > data_beamlet_height:
                         print('parsing influence matrix for beam {}'.format(ind))
                         inf_matrix_2 = sparse.hstack(
                             [csr_matrix(inf_matrix_sparse[:, np.unique(opt_beamlets[i])].sum(axis=1)) for i in
                              range(len(opt_beamlets))], format='csr')
                         inf_matrix = sparse.hstack(
                             [inf_matrix, inf_matrix_2], format='csr')
                     else:
-                        if self.down_sample_xyz is None:
+                        if self._down_sample_xyz is None:
                             inf_matrix = sparse.hstack(
                                 [inf_matrix, inf_matrix_sparse[ind][:, opt_beamlets]], format='csr')
             # if del_org_matrix:
-            if 'influenceMatrixSparse' in plan.beams.beams_dict:
-                del plan.beams.beams_dict['influenceMatrixSparse']
-            if self.down_sample_xyz is not None:
-                if self.beamlet_width_mm <= 2.5 or self.beamlet_height_mm <= 2.5:
+            if self._down_sample_xyz is not None:
+                if self.beamlet_width_mm <= data_beamlet_width or self.beamlet_height_mm <= data_beamlet_height:
                     inf_matrix = inf_matrix_sparse
                 print('creating influence matrix for down sample voxels..')
                 inf_matrix = sparse.vstack(
                     [csr_matrix((sparse.diags(self._vox_weights[i]).dot(inf_matrix[self._vox_map[i], :])).sum(axis=0))
                      for i
                      in
                      range(len(self._vox_map))], format='csr')
         else:
-            if self.beamlet_width_mm > 2.5 or self.beamlet_height_mm > 2.5 or self.down_sample_xyz is not None:
-                inf_matrix_full = plan.inf_matrix.A_full
+            if self.beamlet_width_mm > data_beamlet_width or self.beamlet_height_mm > data_beamlet_height or self._down_sample_xyz is not None:
+                inf_matrix_full = self.A
             else:
-                inf_matrix_full = plan.beams.beams_dict['influenceMatrixFull']
+                inf_matrix_full = self._beams.beams_dict['influenceMatrixFull']
+                del self._beams.beams_dict['influenceMatrixFull']
 
             for ind in range(len(self.beamlets_dict)):
                 opt_beamlets = self.beamlets_dict[ind]['opt_beamlets_ids']
 
                 if ind == 0:
-                    if self.beamlet_width_mm > 2.5 or self.beamlet_height_mm > 2.5:
+                    if self.beamlet_width_mm > data_beamlet_width or self.beamlet_height_mm > data_beamlet_height:
                         print('parsing full influence matrix for beam {}'.format(ind))
                         inf_matrix = np.hstack(
                             [inf_matrix_full[:, np.unique(opt_beamlets[i])].sum(axis=1) for i in
                              range(len(opt_beamlets))])
                     else:
-                        if self.down_sample_xyz is None:
+                        if self._down_sample_xyz is None:
                             inf_matrix = inf_matrix_full[ind][:, opt_beamlets]
                 else:
-                    if self.beamlet_width_mm > 2.5 or self.beamlet_height_mm > 2.5:
+                    if self.beamlet_width_mm > data_beamlet_width or self.beamlet_height_mm > data_beamlet_height:
                         print('parsing full influence matrix for beam {}'.format(ind))
                         inf_matrix_2 = np.hstack(
                             [inf_matrix_full[:, np.unique(opt_beamlets[i])].sum(axis=1) for i in
                              range(len(opt_beamlets))])
                         inf_matrix = np.hstack([inf_matrix, inf_matrix_2])
                     else:
-                        if self.down_sample_xyz is None:
+                        if self._down_sample_xyz is None:
                             inf_matrix = np.hstack([inf_matrix, inf_matrix_full[ind][:, opt_beamlets]])
 
                 # down sampling voxels
-            if 'influenceMatrixFull' in plan.beams.beams_dict:
-                del plan.beams.beams_dict['influenceMatrixFull']
-            if self.down_sample_xyz is not None:
-                if self.beamlet_width_mm <= 2.5 or self.beamlet_height_mm <= 2.5:
+            if self._down_sample_xyz is not None:
+                if self.beamlet_width_mm <= data_beamlet_width or self.beamlet_height_mm <= data_beamlet_height:
                     inf_matrix = inf_matrix_full
                 print('creating influence matrix for down sample voxels..')
                 inf_matrix = np.vstack(
                     [(np.diags(self._vox_weights[i]).dot(inf_matrix[self._vox_map[i], :])).sum(axis=0)
                      for i in range(len(self._vox_map))])
 
         return inf_matrix
 
-    def create_BEV_mask_from_contours(self, plan_obj, ind: int, structure: str = 'PTV',
+    def create_BEV_mask_from_contours(self, ind: int, structure: str = 'PTV',
                                       margin_mm: float = None) -> np.ndarray:
         """
 
-        Since beams object contain projection of structure contours on BEV, this function helps to create mask from those contours on BEV
+        Since beams object contain projection of struct_name contours on BEV, this function helps to create mask from those contours on BEV
 
-        :param plan_obj: object of class Plan
+        :param beams: object of class Beams
         :param ind: indices of the beam in beamlet dictionary
-        :param structure: structure for which contours to be converted to mask
+        :param structure: struct_name for which contours to be converted to mask
         :param margin_mm: expand the contours in mm. defaults to None. If it is not none, it will expand the contours
         :return:
         """
         if margin_mm is None and structure == 'PTV':
             margin_mm = self.opt_beamlets_PTV_margin_mm
         elif margin_mm is None:
             margin_mm = 0
 
         # get PTV contour from data
-        contours = plan_obj.beams.beams_dict['BEV_structure_contour_points'][ind][structure]
+        contours = self._beams.beams_dict['BEV_structure_contour_points'][ind][structure]
         # ind = my_plan.beamlets_dict['ID'].index(beam_id)
-        # contours = my_plan._beams_contours[ind][structure]
+        # contours = my_plan._beams_contours[ind][struct_name]
 
         # for each contour create polygon and get beamlets inside the polygon and create mask for it
         for count_num in range(len(contours)):
             polygon = []
             for j in contours[count_num]:
                 polygon.append((j[0], j[1]))
             r = LinearRing(polygon)
@@ -394,29 +456,29 @@
 
                     # if (beamlets[ind]['position_x_mm'], beamlets[ind]['position_y_mm']) in x_and_y:
                     if (beamlets['position_x_mm'][0][ind], beamlets['position_y_mm'][0][ind]) in x_and_y:
                         # beam_map[row, col] = beamlets[ind]['id']
                         mask[row, col] = True
         return mask
 
-    def preprocess_beams(self, plan_obj, structure='PTV', remove_corner_beamlets=False):
+    def preprocess_beams(self, structure='PTV', remove_corner_beamlets=False):
         """
         Preprocess beams to create beamlets dictionary based on beamlet resolution.
 
-        :param plan_obj: object of class Plan
-        :param structure: projection of the structure on BEV for which beamlets to be considered for creating influence matrix. defaults to PTV
+        :param beams: object of class Beams
+        :param structure: projection of the struct_name on BEV for which beamlets to be considered for creating influence matrix. defaults to PTV
         :param remove_corner_beamlets: If remove corner beamlet is true, it will remove the corner beamlets during down sampling.
         :return: beamlets for processing influence matrix
         """
 
         for ind in range(len(self.beamlets_dict)):
             # ind = my_plan.beamlets_dict['ID'].index(beam_id)
-            mask = self.create_BEV_mask_from_contours(plan_obj, ind=ind, structure=structure,
+            mask = self.create_BEV_mask_from_contours(ind=ind, structure=structure,
                                                       margin_mm=self.opt_beamlets_PTV_margin_mm)
-            beam_2d_grid = self.create_beamlet_idx_2d_grid(ind=ind)
+            beam_2d_grid = self.create_beamlet_idx_2d_finest_grid(ind=ind)
             beamlets = self.beamlets_dict[ind]
 
             # creating beam_map of original resolution so that mask can be multiplied with it
             beam_map = self.get_orig_res_2d_grid(ind)
             beam_map = np.multiply((beam_map + int(1)), mask)  # add and subtract one to maintain 0th beamlet
             beam_map = beam_map - int(1)  # subtract one again to get original beamlets
 
@@ -427,15 +489,16 @@
             mask_2d_grid = np.zeros_like(beam_2d_grid, dtype=bool)
             mask_2d_grid[a] = True
             beam_2d_grid = (beam_2d_grid + int(1)) * mask_2d_grid  # add and subtract 1 to retain ids
             beam_2d_grid = beam_2d_grid - int(1)
             beam_map = beam_2d_grid
 
             # get opt beamlets for down_sample grid as list of original inf_matrix beamlet
-            if self.beamlet_width_mm > 2.5 or self.beamlet_height_mm > 2.5:
+            if self.beamlet_width_mm > self._beams.get_beamlet_width() or \
+                    self.beamlet_height_mm > self._beams.get_beamlet_height():
                 down_sample_2d_grid = self.down_sample_2d_grid(ind=ind, beamlet_width_mm=self.beamlet_width_mm,
                                                                beamlet_height_mm=self.beamlet_height_mm)
                 down_sample_2d_grid = (down_sample_2d_grid + int(1)) * mask_2d_grid  # add and subtract 1 to retain ids
                 down_sample_2d_grid = down_sample_2d_grid - int(1)
                 down_sample_beamlets, counts = np.unique(np.sort(down_sample_2d_grid[down_sample_2d_grid >= 0]),
                                                          return_counts=True)
                 # remove corner beamlets in coarse resolution and updating down sample map
@@ -447,50 +510,51 @@
                                                               None]  # keep only down sample beamlets and remove others
                     down_sample_2d_grid[~np.any(inds_down_sample, axis=0)] = -1
 
                 a = np.where(np.isin(down_sample_2d_grid, down_sample_beamlets))
                 mask_2d_grid = np.zeros_like(beam_2d_grid, dtype=bool)
                 mask_2d_grid[a] = True
                 # actual_beamlets = beam_2d_grid[a]
-                actual_beamlets = plan_obj.inf_matrix.beamlets_dict[ind]['beamlet_idx_2dgrid'][a]
+                actual_beamlets = self.beamlets_dict[ind]['beamlet_idx_2d_finest_grid'][a]
                 sampled_beamlets = down_sample_2d_grid[a]
                 b = [np.where(sampled_beamlets == down_sample_beamlets[i]) for i in range(len(down_sample_beamlets))]
                 opt_beamlets = [actual_beamlets[i] for i in b]
 
                 beam_map = down_sample_2d_grid
             else:
                 opt_beamlets = np.unique(np.sort(beam_map[beam_map >= 0]))
 
             # make beamlets continuous
             std_map = self.sort_beamlets(beam_map)
             if ind == 0:
                 beam_map = std_map
             else:
                 beam_map = std_map + int(
-                    np.amax(self.beamlets_dict[ind - 1]['beamlet_idx_2dgrid']) + 1) * mask_2d_grid
+                    np.amax(self.beamlets_dict[ind - 1]['beamlet_idx_2d_finest_grid']) + 1) * mask_2d_grid
             standInd = np.unique(np.sort(beam_map.flatten()))
-            self.beamlets_dict[ind]['beamlet_idx_2dgrid'] = beam_map
+            self.beamlets_dict[ind]['beamlet_idx_2d_finest_grid'] = beam_map
             # my_plan.beamlets_dict.setdefault('structure_mask_2dgrid', []).append(mask_2d_grid)
-            self.beamlets_dict[ind]['start_beamlet'] = standInd[1]
-            self.beamlets_dict[ind]['end_beamlet'] = np.amax(self.beamlets_dict[ind]['beamlet_idx_2dgrid'])
+            self.beamlets_dict[ind]['start_beamlet_idx'] = standInd[1]
+            self.beamlets_dict[ind]['end_beamlet_idx'] = np.amax(self.beamlets_dict[ind]['beamlet_idx_2d_finest_grid'])
             self.beamlets_dict[ind]['opt_beamlets_ids'] = opt_beamlets
 
             # update beamlet dict
-            if self.beamlet_width_mm > 2.5 or self.beamlet_height_mm > 2.5:
+            if self.beamlet_width_mm > self._beams.get_beamlet_width() or \
+                    self.beamlet_height_mm > self._beams.get_beamlet_height():
                 pass
             else:
                 self.beamlets_dict[ind]['position_x_mm'][0] = beamlets['position_x_mm'][0][opt_beamlets]
                 self.beamlets_dict[ind]['position_y_mm'][0] = beamlets['position_y_mm'][0][opt_beamlets]
                 self.beamlets_dict[ind]['width_mm'][0] = beamlets['width_mm'][0][opt_beamlets]
                 self.beamlets_dict[ind]['height_mm'][0] = beamlets['height_mm'][0][opt_beamlets]
                 self.beamlets_dict[ind]['MLC_leaf_idx'][0] = beamlets['MLC_leaf_idx'][0][opt_beamlets]
             del self.beamlets_dict[ind]['id']
             # my_plan.beams_dict.setdefault('opt_beamlets_ids', []).append(standInd[1:])
 
-    def create_beamlet_idx_2d_grid(self, ind: int) -> np.ndarray:
+    def create_beamlet_idx_2d_finest_grid(self, ind: int) -> np.ndarray:
         """
         Create beamlet idx in 2d grid of 2.5mm resolution. i.e. each element in matrix is 2.5mm*2.5mm
 
         :param ind: indices for the beam in beamlets dictionary
         :return:
         """
         # ind = my_plan.beamlets_dict['ID'].index(beam_id)
@@ -612,37 +676,69 @@
                     except:
                         raise ValueError("invalid beam id {}".format(idx))
         # Bug fix. in case ind is int make it as list
         if isinstance(ind, int):
             ind = [ind]
         beam_orig = []
         for b in ind:
-            beam_map = self.beamlets_dict[b]['beamlet_idx_2dgrid']
+            beam_map = self.beamlets_dict[b]['beamlet_idx_2d_finest_grid']
             if not finest_grid:
                 rowsNoRepeat = [0]
                 for i in range(1, np.size(beam_map, 0)):
                     if (beam_map[i, :] != beam_map[rowsNoRepeat[-1], :]).any():
                         rowsNoRepeat.append(i)
                 colsNoRepeat = [0]
                 for j in range(1, np.size(beam_map, 1)):
                     if (beam_map[:, j] != beam_map[:, colsNoRepeat[-1]]).any():
                         colsNoRepeat.append(j)
                 beam_map = beam_map[np.ix_(np.asarray(rowsNoRepeat), np.asarray(colsNoRepeat))]
+
+                # add this part in case remove corner beamlets create issue for getting original resolution
+                remove_row = []
+                remove_col = []
+                for row in range(beam_map.shape[0]):
+                    if row < beam_map.shape[0] - 1:
+                        prev_elem = beam_map[row, :][beam_map[row, :] > -1]
+                        next_elem = beam_map[row + 1, :][beam_map[row + 1, :] > -1]
+                        matching_elements = np.intersect1d(prev_elem, next_elem)
+                        if len(matching_elements) > 1:
+                            if len(prev_elem) <= len(next_elem):
+                                remove_row.append(row)
+                            else:
+                                remove_row.append(row + 1)
+                for col in range(beam_map.shape[1]):
+                    if col < beam_map.shape[1] - 1:
+                        prev_elem = beam_map[:, col][beam_map[:, col] > -1]
+                        next_elem = beam_map[:, col + 1][beam_map[:, col + 1] > -1]
+                        matching_elements = np.intersect1d(prev_elem, next_elem)
+                        if len(matching_elements) > 1:
+                            if len(prev_elem) <= len(next_elem):
+                                remove_col.append(col)
+                            else:
+                                remove_col.append(col + 1)
+                mask_rows = np.ones(beam_map.shape[0], dtype=bool)
+                mask_columns = np.ones(beam_map.shape[1], dtype=bool)
+                if len(remove_row) > 0:
+                    mask_rows[remove_row] = False
+                if len(remove_col) > 0:
+                    mask_columns[remove_col] = False
+                beam_map = beam_map[mask_rows][:, mask_columns]
+
             beam_orig.append(beam_map)
         if len(beam_orig) == 1:
             beam_orig = beam_orig[0]  # return ndarray in case if it is not list
 
         return beam_orig
 
     def down_sample_voxels(self, down_sample_xyz: List[int] = None):
         """
         This method creates new ct to dose_1d voxel map array based on down sampled voxels.
         It also outputs map between down sampled voxel indices to original voxel indices for down sampling influence matrix
         :param down_sample_xyz: It down-samples optimization voxels as factor of ct resolution
-                e.g. down_sample_xyz = [5,5,1]. It will down-sample optimization voxels with 5 * ct res. in x direction, 5 * ct res. in y direction and 1*ct res. in z direction.
+                e.g. _down_sample_xyz = [5,5,1]. It will down-sample optimization voxels with 5 * ct res. in x direction, 5 * ct res. in y direction and 1*ct res. in z direction.
                 defaults to None. When None it will use the original optimization voxel resolution.
         :return: voxel map(list containing map between down-sampled indices to original indices), voxel weight (weighted average of voxels in down sample
          and ct to dose_1d voxel map
         """
 
         vox_3d = self.opt_voxels_dict['ct_to_dose_voxel_map'][0]
         # dose_to_ct_int = np.round(np.array(self.opt_voxels_dict['dose_voxel_resolution_xyz_mm']) /
@@ -719,36 +815,37 @@
                 down_sample_3d = np.pad(
                     down_sample_3d,
                     [(0, vox_3d.shape[i] - down_sample_3d.shape[i]) for i in range(len(down_sample_3d.shape))],
                     "constant", constant_values=-1)
 
         return vox_map, vox_weights, down_sample_3d
 
-    def pre_process_voxels(self, plan_obj):
+    def pre_process_voxels(self):
         """
         Updates opt_voxels_dict based upon ct to dose_1d voxel map
 
-        :param plan_obj: object if class Plan
+        :param ct: object if class CT
+        :param structs: object of class CT
         :return:
         """
-        if self.down_sample_xyz is not None:
-            vox_map, vox_weights, down_sample_3d = self.down_sample_voxels(down_sample_xyz=self.down_sample_xyz)
+        if self._down_sample_xyz is not None:
+            vox_map, vox_weights, down_sample_3d = self.down_sample_voxels(down_sample_xyz=self._down_sample_xyz)
             self.opt_voxels_dict['ct_to_dose_voxel_map'][0] = down_sample_3d
             self._vox_map = vox_map
             self._vox_weights = vox_weights
-            for structure_name in plan_obj.structures.structures_dict['name']:
-                ind = plan_obj.structures.structures_dict['name'].index(structure_name)
-                vox_3d = plan_obj.structures.structures_dict['structure_mask_3d'][ind] * \
-                         self.opt_voxels_dict['ct_to_dose_voxel_map'][0]
+            for structure_name in self._structs.structures_dict['name']:
+                ind = self._structs.structures_dict['name'].index(structure_name)
+                # deep copying mask so that it doesnt modify in structures
+                vox_3d = deepcopy(self._structs.structures_dict['structure_mask_3d'][ind]) * self.opt_voxels_dict['ct_to_dose_voxel_map'][0]
                 # my_plan.structures_dict['voxel_idx'][i] = np.unique(vox_3d[vox_3d > 0])
                 vox, counts = np.unique(vox_3d[vox_3d > 0], return_counts=True)
                 self.opt_voxels_dict['voxel_idx'][ind] = vox
-                self.opt_voxels_dict['voxel_size'][ind] = counts * np.prod(
-                    plan_obj.get_ct_res_xyz_mm())  # calculate weight for each voxel
-                # self.opt_voxels_dict['voxel_size'][ind] = counts / np.max(counts)  # calculate weight for each voxel
+                self.opt_voxels_dict['voxel_volume_cc'][ind] = counts * np.prod(
+                    self._ct.get_ct_res_xyz_mm())/1000  # calculate weight for each voxel
+                # self.opt_voxels_dict['voxel_volume_cc'][ind] = counts / np.max(counts)  # calculate weight for each voxel
 
     @staticmethod
     def sort_beamlets(b_map):
         c = b_map[b_map >= 0]
         c = np.unique(c)
         ind = np.arange(0, len(c))
         c_sort = np.sort(c)
@@ -757,57 +854,58 @@
         for i in range(len(ind)):
             map_copy[matrix_ind[i]] = ind[i]
         return map_copy
 
     # for voxels idx methods
     def set_opt_voxel_idx(self, plan_obj, structure_name: str) -> None:
         """
-        Set opt_voxel_idx for the structure based upon ct_dose_voxel_map and structure mask
+        Set opt_voxel_idx for the struct_name based upon ct_dose_voxel_map and struct_name mask
 
         :param plan_obj: object of class Plan
-        :param structure_name: structure name
-        :return: set the voxel idx in opt_voxels_dict for the structure
+        :param structure_name: struct_name name
+        :return: set the voxel idx in opt_voxels_dict for the struct_name
         """
         ind = plan_obj.structures.structures_dict['name'].index(structure_name)
         vox_3d = plan_obj.structures.structures_dict['structure_mask_3d'][ind] * \
                  self.opt_voxels_dict['ct_to_dose_voxel_map'][0]
         # my_plan.structures_dict['voxel_idx'][i] = np.unique(vox_3d[vox_3d > 0])
         vox, counts = np.unique(vox_3d[vox_3d > 0], return_counts=True)
         self.opt_voxels_dict['voxel_idx'].append(vox)
-        # self.opt_voxels_dict['voxel_size'].append(counts / np.max(counts))  # calculate weight for each voxel
-        self.opt_voxels_dict['voxel_size'].append(
-            counts * np.prod(plan_obj.get_ct_res_xyz_mm()))  # calculate weight for each voxel
+        # self.opt_voxels_dict['voxel_volume_cc'].append(counts / np.max(counts))  # calculate weight for each voxel
+        self.opt_voxels_dict['voxel_volume_cc'].append(
+            counts * np.prod(plan_obj.get_ct_res_xyz_mm())/1000)  # calculate weight for each voxel
         self.opt_voxels_dict['name'].append(structure_name)
 
     def get_opt_voxels_idx(self, structure_name: str) -> np.ndarray:
         """
-        Get voxel index for structure
-        :param structure_name: name of the structure in plan
-        :return: voxel indexes for the structure
+        Get voxel index for struct_name
+        :param structure_name: name of the struct_name in plan
+        :return: voxel indexes for the struct_name
         """
         ind = self.opt_voxels_dict['name'].index(structure_name)
         vox_ind = self.opt_voxels_dict['voxel_idx'][ind]
         # vox_ind = np.where(my_plan.opt_voxels_dict['voxel_structure_map'][0][:, ind] == 1)[0]
         return vox_ind
 
-    def get_opt_voxels_size(self, structure_name: str):
+    def get_opt_voxels_volume_cc(self, structure_name: str):
         """
-         :param structure_name: name of the structure in plan
-         :return: voxel size for the structure
+         :param structure_name: name of the struct_name in plan
+         :return: voxel size for the struct_name
          """
         ind = self.opt_voxels_dict['name'].index(structure_name)
-        vox_weights = self.opt_voxels_dict['voxel_size'][ind]
+        vox_weights = self.opt_voxels_dict['voxel_volume_cc'][ind]
         # vox_ind = np.where(my_plan.opt_voxels_dict['voxel_structure_map'][0][:, ind] == 1)[0]
         return vox_weights
 
     def get_all_beam_ids(self) -> List[int]:
         ids = [self.beamlets_dict[i]['beam_id'] for i in range(len(self.beamlets_dict))]
         return ids
 
-    def plot_fluence_2d(self, beam_id: int, optimal_fluence_2d: List[np.ndarray] = None, sol: dict = None, **options) -> None:
+    def plot_fluence_2d(self, beam_id: int, optimal_fluence_2d: List[np.ndarray] = None, sol: dict = None,
+                        **options) -> None:
         """
 
                 Displays fluence in 2d for the given beam_id
 
                 :param optimal_fluence_2d:
                 :param beam_id: beam_id of the beam
                 :param sol: solution dictionary after optimization
@@ -830,24 +928,25 @@
             optimal_fluence_2d = self.fluence_1d_to_2d(sol=sol)
         if ax is None:
             fig, ax = plt.subplots(figsize=figsize)
 
         mat = ax.matshow(optimal_fluence_2d[ind[0]])
         ax.set_xlabel('x-axis (beamlets column)')
         ax.set_ylabel('y-axis (beamlets row)')
-        plt.colorbar(mat)
+        plt.colorbar(mat, ax=ax)
         if title is not None:
             ax.set_title('{}'.format(title))
         if filename is not None:
             plt.savefig(filename, bbox_inches="tight", dpi=300)
         if show:
             plt.show()
         return ax
 
-    def plot_fluence_3d(self, beam_id: int, optimal_fluence_2d: List[np.ndarray] = None, sol: dict = None, **options) -> None:
+    def plot_fluence_3d(self, beam_id: int, optimal_fluence_2d: List[np.ndarray] = None, sol: dict = None,
+                        **options) -> None:
         """
                 Displays fluence in 3d for the given beam_id
 
                 :param optimal_fluence_2d:
                 :param sol: solution after optimization
                 :param beam_id: beam_id of the beam
                 :return: 3d optimal fluence plot
@@ -865,15 +964,15 @@
 
         ind = [i for i in range(len(self.beamlets_dict)) if self.beamlets_dict[i]['beam_id'] == beam_id]
         if len(ind) == 0:
             raise IndexError('invalid beam id {}'.format(beam_id))
         if sol is not None:
             optimal_fluence_2d = self.fluence_1d_to_2d(sol=sol)
         (ax, surf) = InfluenceMatrix.surface_plot(optimal_fluence_2d[ind[0]], ax=ax, figsize=figsize,
-                                                       cmap='viridis', edgecolor='black')
+                                                  cmap='viridis', edgecolor='black')
         plt.colorbar(surf, ax=ax, pad=0.2)
         ax.set_zlabel('Fluence Intensity')
         ax.set_xlabel('x-axis (beamlets column)')
         ax.set_ylabel('y-axis (beamlets row)')
 
         if title is not None:
             ax.set_title('{}'.format(title))
```

### Comparing `portpy-0.0.1/portpy/photon/plan.py` & `portpy-0.0.2/portpy/photon/visualization.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,352 +1,431 @@
-from typing import List
-from portpy.photon.beam import Beams
-from portpy.photon.structures import Structures
+from __future__ import annotations
+import matplotlib.pyplot as plt
+import matplotlib as mpl
+import numpy as np
+from skimage import measure
+from portpy.photon.evaluation import Evaluation
+from matplotlib.lines import Line2D
 import os
-from portpy.photon.clinical_criteria import ClinicalCriteria
-from portpy.photon.influence_matrix import InfluenceMatrix
-from portpy.photon.visualization import Visualization
-from portpy.photon.optimization import Optimization
-from portpy.photon.utils import *
-
-
-class Plan:
-    """
-    A class representing a plan
-
-    - **Attributes** ::
-
-        :param opt_beamlets_PTV_margin_mm: For each beam, we often only include the beamlets that are within
-            few millimetres of the projection of the PTV (tumor) into that beam. It is because the beamlets
-            that are far from the PTV projection mainly deliver radiation to the healthy tissues not PTV. Default is 3mm
-        :type opt_beamlets_PTV_margin_mm: int
-        :param beams_dict: an object of class Beams that contains information about the beams_dict used in the treatment plan.
-        :type beams: object
-        :param structures: an object of class Structures that contains information about the structures present in the patient's CT scan.
-        :type structures: object
-        :param inf_matrix: object of class Influence matrix
-        :type inf_matrix: object
-        :param clinial_criteria: an object of class ClincialCriteria that contains information about the goals and constraints of the treatment plan
-        :type inf_matrix: object
-        :param ct: dictionary containing ct metadata. It includes metadata about important ct parameters like resolution, ct in HU etc.
-        :type ct: dict
-
-    - **Methods** ::
-
-        :create_inf_matrix(beamlet_width_mm, beamlet_height_mm,
-                          down_sample_xyz):
-            Create object of Influence Matrix class
-        :get_prescription():
-            Return prescription for the plan
-        :get_num_of_fractions()
-            Return number of fractions for the plan
+from portpy.photon.utils import view_in_slicer_jupyter
+from pathlib import Path
+from typing import List, TYPE_CHECKING
+from .ct import CT
+from .structures import Structures
+
+if TYPE_CHECKING:
+    from portpy.photon.plan import Plan
+try:
+    from typing import Literal
+except ImportError:
+    from typing_extensions import Literal
+
+
+class Visualization:
+    dose_type = Literal["Absolute(Gy)", "Relative(%)"]
+    volume_type = Literal["Absolute(cc)", "Relative(%)"]
 
-
-
-
-    """
-
-    def __init__(self, patient_id: str, data_dir: str = None, beam_ids: List[int] = None,
-                 opt_beamlets_PTV_margin_mm: int = 3, load_inf_matrix_full: bool = False,
-                 protocol_name='Lung_Default_2Gy_30Fr', protocol_type='Default') -> None:
-        """
-        Creates an object of Plan class for the specified patient
-
-        :param patient_id: the patient that we're creating a plan for (name of the folder)
-        :param data_dir: the name of the folder that includes all the patients' data.
-            If None, then ''current-folder\Data'' is used
-        :param beam_ids: the indices of the beams_dict used for creating the plan object.
-            If None, the beams_dict selected by an expert (human) physicist for the specified patient would be used
-        :param opt_beamlets_PTV_margin_mm: For each beam, we often only include the beamlets that are within
-            few millimetres of the projection of the PTV (tumor) into that beam. It is because the beamlets
-            that are far from the PTV projection mainly deliver radiation to the healthy tissues not PTV. Default is 3mm
-        :param load_inf_matrix_full: If set to true, it will load full influence matrix from the data
+    @staticmethod
+    def plot_dvh(my_plan: Plan, sol: dict = None, dose_1d: np.ndarray = None, struct_names: List[str] = None,
+                 dose_scale: dose_type = "Absolute(Gy)",
+                 volume_scale: volume_type = "Relative(%)", **options):
+        """
+        Create dvh plot for the selected structures
+
+        :param my_plan: object of class Plan
+        :param sol: optimal sol dictionary
+        :param dose_1d: dose_1d in 1d voxels
+        :param struct_names: structures to be included in dvh plot
+        :param volume_scale: volume scale on y-axis. Default= Absolute(cc). e.g. volume_scale = "Absolute(cc)" or volume_scale = "Relative(%)"
+        :param dose_scale: dose_1d scale on x axis. Default= Absolute(Gy). e.g. dose_scale = "Absolute(Gy)" or dose_scale = "Relative(%)"
+        :keyword style (str): line style for dvh curve. default "solid". can be "dotted", "dash-dotted".
+        :keyword width (int): width of line. Default 2
+        :keyword colors(list): list of colors
+        :keyword legend_font_size: Set legend_font_size. default 10
+        :keyword figsize: Set figure size for the plot. Default figure size (12,8)
+        :keyword create_fig: Create a new figure. Default True. If False, append to the previous figure
+        :keyword title: Title for the figure
+        :keyword filename: Name of the file to save the figure in current directory
+        :keyword show: Show the figure. Default is True. If false, next plot can be append to it
+        :keyword norm_flag: Use to normalize the plan. Default is False.
+        :keyword norm_volume: Use to set normalization volume. default is 90 percentile.
+        :return: dvh plot for the selected structures
 
         :Example:
-
-        >>> my_plan = Plan(patient_id = r"Lung_Patient_1", path = r"c:\Data", beam_ids = [0,1,2,3,4,5,6], opt_beamlets_PTV_margin_mm=3)
+        >>> Visualization.plot_dvh(my_plan, sol=sol, struct_names=['PTV', 'ESOPHAGUS'], dose_scale='Absolute(Gy)',volume_scale="Relative(%)", show=False, create_fig=True )
         """
 
-        if data_dir is None:
-            data_dir = os.path.join('../..', 'data')
-        patient_folder_path = os.path.join(data_dir, patient_id)
-
-        # read all the meta data for the specified patient and protocol
-        meta_data = load_metadata(patient_folder_path)
-
-        # filter metadata for the given beam_indices.
-        # The meta_data originally includes all the beams_dict.  get_plan_beams only keeps the requested beams_dict
-        meta_data = self.get_plan_beams(beam_ids=beam_ids, meta_data=meta_data)
-        # Load all the data (e.g., influence matrix, voxel coordinates).
-        # meta_data does not include the large numeric data stored in .h5 files
-        data = load_data(meta_data=meta_data, pat_dir=patient_folder_path, load_inf_matrix_full=load_inf_matrix_full)
-        self.opt_beamlets_PTV_margin_mm = opt_beamlets_PTV_margin_mm
-        self.beams = Beams(data['beams_dict'])  # create beams_dict object
-        self.structures = Structures(data['structures'], data['opt_voxels'])  # create structures object
-        self.ct = data['ct']  # create ct attribute containing ct information as dictionary
-        self.patient_id = patient_id
-        self.clinical_criteria = ClinicalCriteria(data['clinical_criteria'])  # create clinical criteria object
-        is_full = False
-        if load_inf_matrix_full:  # check if full influence matrix is requested
-            is_full = True
-
-        self.inf_matrix = InfluenceMatrix(self, is_full=is_full)  # create influence matrix object
-
-    @staticmethod
-    def get_plan_beams(beam_ids: List[int] = None, meta_data: dict = None) -> dict:
-        """
-        Create and return a copy of meta_data with only including the requested beams_dict (beam_ids)
-
-
-        :param beam_ids: the indices of the beams_dict to be included. If None, the planner's beams_dict are used
-        :param meta_data: the dictionary including all the beams_dict
-        :return: returns the meta_data dictionary only including the requested beams_dict in format of:
-            dict: {
-                   'structures': {'name': list(str), 'volume_cc': list(float), }
-                   'opt_voxels': {'_ct_voxel_resolution_xyz_mm': list(float),}
-                  }
-        """
-        if beam_ids is None:  # if beam_ids not included, then the beams_dict
-            # selected by an expert human planner would be used
-            beam_ids = meta_data['planner_beam_ids']['IDs']
-        meta_data_req = meta_data.copy()
-        del meta_data_req['beams_dict']  # remove previous beams_dict
-        beamReq = dict()
-        for i in range(len(beam_ids)):
-            if beam_ids[i] in meta_data['beams_dict']['ID']:
-                ind = meta_data['beams_dict']['ID'].index(beam_ids[i])
-                for key in meta_data['beams_dict']:
-                    beamReq.setdefault(key, []).append(meta_data['beams_dict'][key][ind])
+        if dose_1d is None:
+            if 'dose_1d' not in sol:
+                dose_1d = sol['inf_matrix'].A @ (sol['optimal_intensity'] * my_plan.get_num_of_fractions())
             else:
-                print('beam id {} is not available'.format(beam_ids[i]))
-        meta_data_req['beams_dict'] = beamReq
-        return meta_data_req
-
-    def save_plan(self, plan_name: str = None, path: str = None) -> None:
-        """
-
-        Save pickled file for plan object
+                dose_1d = sol['dose_1d']
 
-        :param plan_name: create the name of the pickled file of plan object. If none, it will save with the name as 'my_plan'
-        :param path: if path is set, plan object will be pickled and saved in path directory else it will save current project directory
-        :return: save pickled object of class Plan
+        if sol is None:
+            sol = dict()
+            sol['inf_matrix'] = my_plan.inf_matrix  # create temporary solution
+
+        # getting options_fig:
+        style = options['style'] if 'style' in options else 'solid'
+        width = options['width'] if 'width' in options else None
+        colors = options['colors'] if 'colors' in options else None
+        legend_font_size = options['legend_font_size'] if 'legend_font_size' in options else 10
+        figsize = options['figsize'] if 'figsize' in options else (12, 8)
+        title = options['title'] if 'title' in options else None
+        filename = options['filename'] if 'filename' in options else None
+        show = options['show'] if 'show' in options else False
+        # create_fig = options['create_fig'] if 'create_fig' in options else False
+        show_criteria = options['show_criteria'] if 'show_criteria' in options else None
+        ax = options['ax'] if 'ax' in options else None
+
+        # getting norm options
+        norm_flag = options['norm_flag'] if 'norm_flag' in options else False
+        norm_volume = options['norm_volume'] if 'norm_volume' in options else 90
+        norm_struct = options['norm_struct'] if 'norm_struct' in options else 'PTV'
+
+        plt.rcParams['font.size'] = 12
+        if width is None:
+            if style == 'dotted' or style == 'dashed':
+                width = 2.5
+            else:
+                width = 2
+        if colors is None:
+            colors = Visualization.get_colors()
+        if struct_names is None:
+            # orgs = []
+            struct_names = my_plan.structures.structures_dict['name']
+        max_dose = 0.0
+        max_vol = 0.0
+        all_orgs = my_plan.structures.structures_dict['name']
+        # orgs = [struct.upper for struct in orgs]
+        pres = my_plan.get_prescription()
+        legend = []
+
+        if ax is None:
+            fig, ax = plt.subplots(figsize=figsize)
+        if norm_flag:
+            norm_factor = Evaluation.get_dose(sol, dose_1d=dose_1d, struct=norm_struct, volume_per=norm_volume) / pres
+            dose_1d = dose_1d / norm_factor
+        for i in range(np.size(all_orgs)):
+            if all_orgs[i] not in struct_names:
+                continue
+            # for dose_1d in dose_list:
+            #
+            x, y = Evaluation.get_dvh(sol, struct=all_orgs[i], dose_1d=dose_1d)
+            if dose_scale == 'Absolute(Gy)':
+                max_dose = np.maximum(max_dose, x[-1])
+                ax.set_xlabel('Dose (Gy)')
+            elif dose_scale == 'Relative(%)':
+                x = x / pres * 100
+                max_dose = np.maximum(max_dose, x[-1])
+                ax.set_xlabel('Dose (%)')
+
+            if volume_scale == 'Absolute(cc)':
+                y = y * my_plan.structures.get_volume_cc(all_orgs[i]) / 100
+                max_vol = np.maximum(max_vol, y[1] * 100)
+                ax.set_ylabel('Volume (cc)')
+            elif volume_scale == 'Relative(%)':
+                max_vol = np.maximum(max_vol, y[0] * 100)
+                ax.set_ylabel('Volume Fraction (%)')
+            ax.plot(x, 100 * y, linestyle=style, linewidth=width, color=colors[i])
+            legend.append(all_orgs[i])
+
+        if show_criteria is not None:
+            for s in range(len(show_criteria)):
+                if 'dose_volume' in show_criteria[s]['name']:
+                    x = show_criteria[s]['parameters']['dose_gy']
+                    y = show_criteria[s]['constraints']['limit_volume_perc']
+                    ax.plot(x, y, marker='x', color='red', markersize=20)
+        # plt.xlabel('Dose (Gy)')
+        # plt.ylabel('Volume Fraction (%)')
+        ax.set_xlim(0, max_dose * 1.1)
+        ax.set_ylim(0, max_vol)
+        ax.legend(legend, prop={'size': legend_font_size}, loc="upper right")
+        ax.grid(visible=True, which='major', color='#666666', linestyle='-')
+
+        # Show the minor grid lines with very faint and almost transparent grey lines
+        # plt.minorticks_on()
+        ax.minorticks_on()
+        plt.grid(visible=True, which='minor', color='#999999', linestyle='--', alpha=0.2)
+        y = np.arange(0, 101)
+        # if norm_flag:
+        #     x = pres * np.ones_like(y)
+        # else:
+        if dose_scale == "Absolute(Gy)":
+            x = pres * np.ones_like(y)
+        else:
+            x = 100 * np.ones_like(y)
+
+        ax.plot(x, y, color='black')
+        if title:
+            ax.set_title(title)
+        if show:
+            plt.show()
+        if filename is not None:
+            plt.savefig(filename, bbox_inches="tight", dpi=300)
+        return ax
 
-        :Example:
-        >>> my_plan.save_plan(plan_name='my_plan', path=r"path/to/save_plan")
-        """
-        save_plan(self, plan_name=plan_name, path=path)
+    @staticmethod
+    def plot_binary_mask_points(my_plan, structure: str, show: bool = True, color: List[str] = None):
+        fig = plt.figure()
+        ax = fig.add_subplot(111, projection='3d')
+        ind = my_plan.structures.structures_dict['name'].index(structure)
+        mask_3d = my_plan.structures.structures_dict['structure_mask_3d'][ind]
+        pos = np.where(mask_3d == 1)
+        if color is None:
+            color = Visualization.get_colors()
+        ax.scatter(pos[0], pos[1], pos[2], c=color)
+        if show:
+            plt.show()
 
     @staticmethod
-    def load_plan(plan_name: str = None, path: str = None):
+    def get_colors():
         """
-        Load pickle file of the plan object.
-
-        :param plan_name: plan_name of the object of class Plan. It None, it will try to look for plan name called 'my_plan'
-        :param path: if path is set, plan object will be load from path directory else current project directory
-        :return: load pickled object of class Plan
 
-        :Example:
-        >>> Plan.load_plan(plan_name='my_plan', path=r"path/for/loading_plan")
+        :return: return list of 20 colors
         """
+        colors = ['#ffe119', '#4363d8', '#f58231', '#911eb4',
+                  '#46f0f0', '#f032e6', '#bcf60c', '#fabebe', '#008080', '#e6beff',
+                  '#9a6324', '#fffac8', '#800000', '#aaffc3', '#808000', '#ffd8b1',
+                  '#000075', '#808080', '#ffffff', '#000000', '#e6194b', '#3cb44b']
+        return colors
 
-        return load_plan(plan_name=plan_name, path=path)
+    @staticmethod
+    def surface_plot(matrix: np.ndarray, **kwargs):
+        # acquire the cartesian coordinate matrices from the matrix
+        # x is cols, y is rows
+        (x, y) = np.meshgrid(np.arange(matrix.shape[0]), np.arange(matrix.shape[1]))
+        fig = plt.figure()
+        ax = fig.add_subplot(111, projection='3d')
+        surf = ax.plot_surface(x, y, np.transpose(matrix), **kwargs)
+        return ax, surf
 
     @staticmethod
-    def load_optimal_sol(sol_name: str, path: str = None) -> dict:
+    def plot_fluence_2d(beam_id: int, sol: dict, **options):
         """
 
-        Load optimal solution dictionary got from optimization
+        Displays fluence in 2d for the given beam_id
 
-        :param sol_name: name of the optimal solution to be loaded.
-        :param path: if path is set, plan object will be load from path directory else current directory
-        :return: load solution
+        :param beam_id: beam_id of the beam
+        :param sol: solution dictionary after optimization
+        :return: 2d optimal fluence plot
 
         :Example:
-        >>> sol = Plan.load_optimal_sol(sol_name='sol', path=r'path/for/loading_sol')
+        >>> Visualization.plot_fluence_2d(beam_id=0, sol=sol, **options)
         """
-        return load_optimal_sol(sol_name=sol_name, path=path)
+        return sol['inf_matrix'].plot_fluence_2d(beam_id=beam_id, sol=sol, **options)
 
     @staticmethod
-    def save_optimal_sol(sol: dict, sol_name: str, path: str = None) -> None:
+    def plot_fluence_3d(beam_id: int, sol: dict, **options):
         """
-        Save the optimal solution dictionary from optimization
+        Displays fluence in 3d for the given beam_id
 
-        :param sol: optimal solution dictionary
-        :param sol_name: name of the optimal solution saved
-        :param path: if path is set, plan object will be load from path directory else current directory
-        :return: save pickled file of optimal solution dictionary
+        :param sol: solution after optimization
+        :param beam_id: beam_id of the beam
+        :return: 3d optimal fluence plot
 
         :Example:
-        >>> my_plan.save_optimal_sol(sol=sol, sol_name='sol', path=r'path/to/save_solution')
-        """
-        save_optimal_sol(sol=sol, sol_name=sol_name, path=path)
-
-    def create_inf_matrix(self, beamlet_width_mm: float = 2.5, beamlet_height_mm: float = 2.5,
-                          opt_vox_xyz_res_mm: List[float] = None,
-                          structure: str = 'PTV', is_full: bool = False) -> InfluenceMatrix:
+        >>> Visualization.plot_fluence_3d(beam_id=0, sol=sol, **options)
         """
-                Create a influence matrix object for Influence Matrix class
-
-                :param is_full: Defaults to False. If True, it will create full influence matrix
-                :param beamlet_width_mm: beamlet width in mm. It should be multiple of 2.5, defaults to 2.5
-                :param beamlet_height_mm: beamlet height in mm. It should be multiple of 2.5, defaults to 2.5
-                :param structure: target structure for creating BEV beamlets, defaults to 'PTV'
-                :param opt_vox_xyz_res_mm: It down-samples optimization voxels as factor of ct resolution
-                    e.g. opt_vox_xyz_res = [5*ct.res.x,5*ct.res.y,1*ct.res.z]. It will down-sample optimization voxels with 5 * ct res. in x direction, 5 * ct res. in y direction and 1*ct res. in z direction.
-                    defaults to None. When None it will use the original optimization voxel resolution.
-                :returns: object of influence Matrix class
+        return sol['inf_matrix'].plot_fluence_3d(beam_id=beam_id, sol=sol, **options)
 
-                :Example:
-                >>> inf_matrix = my_plan.create_inf_matrix(beamlet_width_mm=5, beamlet_height_mm=5, opt_vox_xyz_res_mm=[5,5,1], structure=structure)
-                """
-        return InfluenceMatrix(self, beamlet_width_mm=beamlet_width_mm, beamlet_height_mm=beamlet_height_mm,
-                               opt_vox_xyz_res_mm=opt_vox_xyz_res_mm, is_full=is_full)
-
-    def get_prescription(self) -> float:
-        """
-
-        :return: prescription in Gy
-        """
-        pres = self.clinical_criteria.clinical_criteria_dict['pres_per_fraction_gy'] * \
-               self.clinical_criteria.clinical_criteria_dict[
-                   'num_of_fractions']
-        return pres
-
-    def get_num_of_fractions(self) -> float:
-        """
-
-        :return: number of fractions to be delivered
-        """
-        return self.clinical_criteria.clinical_criteria_dict['num_of_fractions']
+    @staticmethod
+    def plot_2d_slice(my_plan: Plan = None, sol: dict = None, ct: CT = None, structs: Structures = None,
+                      slice_num: int = 40, struct_names: List[str] = None, show_dose: bool = False,
+                      show_struct: bool = True, show_isodose: bool = False,
+                      **options) -> None:
+        """
+
+        Plot 2d view of ct, dose_1d, isodose and struct_name contours
+
+        :param sol: solution to optimization
+        :param my_plan: object of class Plan
+        :param ct: Optional. object of class CT
+        :param structs: Optional. object of class structs
+        :param slice_num: slice number
+        :param struct_names: structures for which contours to be displayed on the slice view. e.g. struct_names = ['PTV, ESOPHAGUS']
+        :param show_dose: view dose_1d on the slice
+        :param show_struct: view struct_name on the slice
+        :param show_isodose: view isodose
+        :param dpi: Default dpi=100 for figure
+        :return: plot 2d view of ct, dose_1d, isodose and struct_name contours
 
-    def get_disease_site(self) -> float:
+        :Example:
+        >>> Visualization.plot_2d_slice(my_plan, sol=sol, slice_num=50, struct_names=['PTV'], show_isodose=False)
         """
 
-        :return: number of fractions to be delivered
-        """
-        return self.clinical_criteria.clinical_criteria_dict['disease_site']
+        # getting options_fig:
+        figsize = options['figsize'] if 'figsize' in options else (8, 8)
+        title = options['title'] if 'title' in options else None
+        filename = options['filename'] if 'filename' in options else None
+        dpi = options['dpi'] if 'dpi' in options else 100
+        show = options['show'] if 'show' in options else False
+        ax = options['ax'] if 'ax' in options else None
+
+        if ax is None:
+            fig, ax = plt.subplots(figsize=figsize, dpi=dpi)
+        plt.rcParams["figure.autolayout"] = True
+        if ct is None:
+            ct = my_plan.ct
+        ct_hu_3d = ct.ct_dict['ct_hu_3d'][0]
+        ax.imshow(ct_hu_3d[slice_num, :, :], cmap='gray')
+
+        # adjust the main plot to make room for the legends
+        plt.subplots_adjust(left=0.2)
+        dose_3d = []
+        if sol is not None:
+            show_dose = True
+        if show_dose:
+            dose_1d = sol['inf_matrix'].A @ (sol['optimal_intensity'] * my_plan.get_num_of_fractions())
+            dose_3d = sol['inf_matrix'].dose_1d_to_3d(dose_1d=dose_1d)
+            masked = np.ma.masked_where(dose_3d[slice_num, :, :] <= 0, dose_3d[slice_num, :, :])
+            im = ax.imshow(masked, alpha=0.4, interpolation='none',
+                           cmap='rainbow')
+
+            plt.colorbar(im, ax=ax, pad=0.1)
+
+        if show_isodose:
+            if not show_dose:
+                dose_1d = sol['inf_matrix'].A * sol['optimal_intensity'] * my_plan.get_num_of_fractions()
+                dose_3d = sol['inf_matrix'].dose_1d_to_3d(dose_1d=dose_1d)
+            dose_legend = Visualization.legend_dose_storage(my_plan)
+            ax.contour(dose_3d[slice_num, :, :], dose_legend['dose_1d value'],
+                       colors=dose_legend['dose_1d color'],
+                       linewidths=0.5, zorder=2)
+            dose_list = []
+            for item in range(0, len(dose_legend['dose_1d name'])):
+                dose_list.append(Line2D([0], [0],
+                                        color=dose_legend['dose_1d color'][item],
+                                        lw=1,
+                                        label=dose_legend['dose_1d name'][item]))
+            ax.add_artist(ax.legend(handles=dose_list,
+                                    bbox_to_anchor=(1.15, 1), loc='upper left', borderaxespad=0.))
+        if title is not None:
+            ax.set_title('{}: Axial View - Slice #: {}'.format(title, slice_num))
+        else:
+            ax.set_title('Axial View - Slice #: {}'.format(slice_num))
+
+        if show_struct:
+            if structs is None:
+                structs = my_plan.structures
+            if struct_names is None:
+                struct_names = structs.structures_dict['name']
+            struct_masks = structs.structures_dict['structure_mask_3d']
+            all_mask = []
+            colors = Visualization.get_colors()
+            for i in range(len(struct_names)):
+                ind = structs.structures_dict['name'].index(struct_names[i])
+                cmap = mpl.colors.ListedColormap(colors[i])
+                contours = measure.find_contours(struct_masks[ind][slice_num, :, :], 0.5)
+                for contour in contours:
+                    ax.plot(contour[:, 1], contour[:, 0], linewidth=2, color=colors[i])
+            labels = [struct for struct in struct_names]
+            # get the colors of the values, according to the
+            import matplotlib.patches as mpatches
+            patches = [mpatches.Patch(color=colors[i], label=labels[i]) for i in range(len(labels))]
+            # rax.labels = labels
+            ax.legend(handles=patches, bbox_to_anchor=(0.1, 0.8), loc=2, borderaxespad=0.)
+            # bbox_transform=fig.transFigure)
+        if show:
+            plt.show()
+        if filename is not None:
+            plt.savefig(filename, bbox_inches="tight", dpi=300)
+        return ax
 
-    def get_ct_res_xyz_mm(self) -> List[float]:
-        """
+    @staticmethod
+    def get_cmap_colors(n, name='hsv'):
+        """Returns a function that maps each index in 0, 1, ..., n-1 to a distinct
+        RGB color; the keyword argument name must be a standard mpl colormap name."""
+        return plt.cm.get_cmap(name, n)
 
-        :return: number of fractions to be delivered
-        """
-        return self.ct['resolution_xyz_mm']
+    @staticmethod
+    def legend_dose_storage(my_plan: Plan) -> dict:
+        # dose_color = [[0.55, 0, 1], [0, 0, 1], [0, 0.5, 1], [0, 1, 0],
+        #               [1, 1, 0], [1, 0.65, 0], [1, 0, 0], [0.55, 0, 0]]
+        dose_color = [[0.55, 0, 0], [0, 0, 1], [0.55, 0, 1], [0, 0.5, 1], [0, 1, 0], [1, 0, 0]]
+        dose_level = [0.3, 0.5, 0.7, 0.9, 1.0, 1.1]
+        dose_prescription = my_plan.clinical_criteria.clinical_criteria_dict['pres_per_fraction_gy'] * \
+                            my_plan.clinical_criteria.clinical_criteria_dict['num_of_fractions']
+        dose_value = [item * dose_prescription for item in dose_level]
+        dose_name = []
+        for item in range(0, len(dose_level)):
+            dose_name.append(str(round(dose_level[item] * 100, 2)) + ' % / ' +
+                             str(round(dose_value[item], 3)) + ' ' + 'Gy')
+        dose_storage_legend = {'dose_1d color': dose_color, 'dose_1d level': dose_level, 'dose_1d value': dose_value,
+                               'dose_1d name': dose_name}
+        return dose_storage_legend
 
-    def plot_dvh(self, sol, dose_1d=None, structs=None, dose_scale: Visualization.dose_type = "Absolute(Gy)",
-                 volume_scale: Visualization.volume_type = "Relative(%)", **options):
+    @staticmethod
+    def view_in_slicer(my_plan: Plan, slicer_path: str = None, data_dir: str = None) -> None:
         """
-                Create dvh plot for the selected structures
-
-                :param sol: optimal sol dictionary
-                :param dose_1d: dose_1d in 1d voxels
-                :param structs: structures to be included in dvh plot
-                :param volume_scale: volume scale on y-axis. Default= Absolute(cc). e.g. volume_scale = "Absolute(cc)" or volume_scale = "Relative(%)"
-                :param dose_scale: dose_1d scale on x axis. Default= Absolute(Gy). e.g. dose_scale = "Absolute(Gy)" or dose_scale = "Relative(%)"
-                :keyword style (str): line style for dvh curve. default "solid". can be "dotted", "dash-dotted".
-                :keyword width (int): width of line. Default 2
-                :keyword colors(list): list of colors
-                :keyword legend_font_size: Set legend_font_size. default 10
-                :keyword figsize: Set figure size for the plot. Default figure size (12,8)
-                :keyword create_fig: Create a new figure. Default True. If False, append to the previous figure
-                :keyword title: Title for the figure
-                :keyword filename: Name of the file to save the figure in current directory
-                :keyword show: Show the figure. Default is True. If false, next plot can be append to it
-                :keyword norm_flag: Use to normalize the plan. Default is False.
-                :keyword norm_volume: Use to set normalization volume. default is 90 percentile.
-                :return: dvh plot for the selected structures
-                """
 
-        Visualization.plot_dvh(self, sol=sol, dose_1d=dose_1d, structs=structs, dose_scale=dose_scale,
-                               volume_scale=volume_scale, **options)
+        :param my_plan: object of class Plan
+        :param slicer_path: slicer executable path on your local machine
+        :param data_dir: the folder path where data located, defaults to None.
+                If path = None, then it assumes the data is in sub-folder named data in the current directory
+        :return: plot the images in 3d slicer
 
-    def run_IMRT_fluence_map_CVXPy(self, inf_matrix: InfluenceMatrix = None, solver='MOSEK'):
-        Optimization.run_IMRT_fluence_map_CVXPy(self, inf_matrix=inf_matrix, solver=solver)
+        view ct, dose_1d and struct_name set images in 3d slicer
 
-    def add_rinds(self, rind_params: List[dict], inf_matrix=None):
-        """
-        Example for
-        rind_params = [{'rind_name': 'RIND_0', 'ref_structure': 'PTV, 'margin_start_mm': 2, 'margin_end_mm': 10, 'max_dose_gy': 10}]
-
-        :param rind_params: rind_params as dictionary
-        :param inf_matrix: object of class inf_matrix
-        :return: save rinds to plan object
+        :Example:
+        >>> Visualization.view_in_slicer(my_plan, slicer_path='C:/Slicer/Slicer.exe', data_dir='path/to/nrrd/image')
         """
-
-        if inf_matrix is None:
-            inf_matrix = self.inf_matrix
-        print('creating rinds..')
-
-        ct_to_dose_map = inf_matrix.opt_voxels_dict['ct_to_dose_voxel_map'][0]
-        dose_mask = ct_to_dose_map >= 0
-        dose_mask = dose_mask.astype(int)
-        self.structures.create_structure('dose_mask', dose_mask)
-
-        for ind, param in enumerate(rind_params):
-            rind_name = param['rind_name']
-            first_dummy_name = '{}_{}'.format(param['ref_structure'], param['margin_start_mm'])
-            second_dummy_name = '{}_{}'.format(param['ref_structure'], param['margin_end_mm'])
-            self.structures.expand(param['ref_structure'], margin_mm=param['margin_start_mm'],
-                                   new_structure=first_dummy_name)
-            if param['margin_end_mm'] == 'inf':
-                param['margin_end_mm'] = 500
-            self.structures.expand(param['ref_structure'], margin_mm=param['margin_end_mm'],
-                                   new_structure=second_dummy_name)
-            self.structures.subtract(second_dummy_name, first_dummy_name, str1_sub_str2=rind_name)
-            self.structures.delete_structure(first_dummy_name)
-            self.structures.delete_structure(second_dummy_name)
-            self.structures.intersect(rind_name, 'dose_mask', str1_and_str2=rind_name)
-        self.structures.delete_structure('dose_mask')
-
-        print('rinds created!!')
-
-        for param in rind_params:
-            inf_matrix.set_opt_voxel_idx(self, structure_name=param['rind_name'])
-            # add rind constraint
-            parameters = {'structure_name': param['rind_name']}
-            # total_pres = self.get_prescription()
-            if 'max_dose_gy' in param:
-                constraints = {'limit_dose_gy': param['max_dose_gy']}
-                self.clinical_criteria.add_criterion(criterion='max_dose', parameters=parameters,
-                                                     constraints=constraints)
-            if 'mean_dose_gy' in param:
-                constraints = {'limit_dose_gy': param['mean_dose_gy']}
-                self.clinical_criteria.add_criterion(criterion='mean_dose', parameters=parameters,
-                                                     constraints=constraints)
+        if slicer_path is None:
+            slicer_path = r'C:\ProgramData\NA-MIC\Slicer 4.11.20210226\Slicer.exe'
+        if data_dir is None:
+            data_dir = os.path.join('..', 'data', my_plan.patient_id)
+        if not os.path.exists(data_dir):  # check if valid directory
+            raise Exception("Invalid data directory. Please input valid directory")
+        slicer_script_dir = os.path.join(Path(__file__).parents[0], 'utils', 'slicer_script.py')
+        import subprocess
+
+        # run python script 'slicer_script.py' in slicer python interface. Currenr limitation segmentation.nrrd file
+        # doesnt know the struct_name names. Hence we manually pass struct_name names to python script
+        subprocess.run([slicer_path, f"--python-script", slicer_script_dir, data_dir,
+                        ','.join(my_plan.structures.structures_dict['name'])], shell=False)
+        print('Done')
 
     @staticmethod
-    def plot_fluence_2d(beam_id: int, sol: dict = None, **options):
-        """
-        plot fluence in 2d for beam_id
-        :param beam_id: beam_id of the beam
-        :param sol: solution dictionary after optimization
-        :return: 2d optimal fluence plot
-        """
-        return Visualization.plot_fluence_2d(beam_id=beam_id, sol=sol, **options)
+    def view_in_slicer_jupyter(my_plan: Plan, dose_1d: np.ndarray = None, sol: dict = None,
+                               ct_name: str = 'ct', dose_name: str = 'dose', struct_set_name: str = 'rt_struct',
+                               show_ct: bool = True,
+                               show_dose: bool = True,
+                               show_structs: bool = True):
+        """
+        This method helps to visualize CT, Dose and Rt struct in 3d slicer
+
+
+        :param my_plan: object of class plan
+        :param dose_1d: dose in 1d
+        :param sol: solution dictionary
+        :param ct_name: Default to 'ct'. name of the ct node in 3D slicer
+        :param dose_name: Default to 'dose'. name of the dose node in 3D slicer
+        :param struct_set_name: name of the rtstruct
+        :param show_structs: default to True. If false, will not create struct_name node
+        :param show_dose: default to True. If false, will not create dose node
+        :param show_ct:default to True. If false, will not create ct node
+        :return: visualize in slicer jupyter
+        """
+        view_in_slicer_jupyter.view_in_slicer_jupyter(my_plan, dose_1d=dose_1d, sol=sol, ct_name=ct_name,
+                                                      dose_name=dose_name,
+                                                      struct_set_name=struct_set_name, show_ct=show_ct,
+                                                      show_dose=show_dose,
+                                                      show_structs=show_structs)
 
     @staticmethod
-    def plot_fluence_3d(beam_id: int, sol: dict = None, **options):
-        """
-        plot fluence in 3d for beam_id
-        :param sol: solution after optimization
-        :param beam_id: beam_id of the beam
-        :return: 3d optimal fluence plot
-        """
-        return Visualization.plot_fluence_3d(beam_id=beam_id, sol=sol, **options)
-
-    def save_nrrd(self, sol: dict, data_dir: str = None):
-        """
-        save nrrd in the path directory else save in patient data directory
-        :param sol: optimal solution dict
-        :param data_dir: save nrrd images of ct, dose_1d and structure set in path directory
-        :return: save nrrd images in path
-        """
-        save_nrrd(self, sol=sol, data_dir=data_dir)
-
-    def view_in_slicer(self, slicer_path=None, img_dir=None):
-        """
-        view ct, dose_1d and structures in slicer
-        :param slicer_path:
-        :param img_dir:
-        :return:
-        """
-        Visualization.view_in_slicer(self, slicer_path=slicer_path, data_dir=img_dir)
+    def is_notebook() -> bool:
+        try:
+            from IPython import get_ipython
+            shell = get_ipython().__class__.__name__
+            if shell == 'ZMQInteractiveShell':
+                return True  # Jupyter notebook or qtconsole
+            elif shell == 'TerminalInteractiveShell':
+                return False  # Terminal running IPython
+            else:
+                if 'google.colab' in str(get_ipython()):
+                    return True
+                else:
+                    return False  # Other type (?)
+        except NameError:
+            return False  # Probably standard Python interpreter
+        except:
+            return False  # Probably standard Python interpreter
```

### Comparing `portpy-0.0.1/portpy/photon/utils/load_data.py` & `portpy-0.0.2/portpy/photon/utils/load_data.py`

 * *Files identical despite different names*

### Comparing `portpy-0.0.1/portpy/photon/utils/load_metadata.py` & `portpy-0.0.2/portpy/photon/utils/load_metadata.py`

 * *Files identical despite different names*

### Comparing `portpy-0.0.1/portpy/photon/utils/save_nrrd.py` & `portpy-0.0.2/portpy/photon/utils/save_nrrd.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,54 +1,65 @@
 from __future__ import annotations
 import SimpleITK as sitk
 from pathlib import Path
 import numpy as np
 from typing import TYPE_CHECKING
 if TYPE_CHECKING:
     from portpy.photon.plan import Plan
+from portpy.photon.ct import CT
+from portpy.photon.structures import Structures
 
 
-def save_nrrd(my_plan: Plan, sol: dict, data_dir: str = None, ct_filename: str = 'ct', dose_filename: str = 'dose',
+def save_nrrd(my_plan: Plan = None, sol: dict = None, data_dir: str = None, ct: CT = None,
+              structs: Structures = None, ct_filename: str = 'ct', dose_filename: str = 'dose',
               rt_struct_filename: str = 'rtss') -> None:
     """
     save nrrd in the path directory else save in patient data directory
 
     :param my_plan: object of class Plan
     :param sol: optimal solution dict
-    :param data_dir: save nrrd images of ct, dose_1d and structure set in path directory
+    :param data_dir: save nrrd images of ct, dose_1d and struct_name set in path directory
+    :param ct: object of class CT
+    :param structs: object of class structs
     :param ct_filename: ct file name
     :param dose_filename: dose file name
     :param rt_struct_filename: rt_struct file name
     :return: save nrrd images in path
     """
     import os
+    if ct is None:
+        ct = my_plan.ct
+    if structs is None:
+        structs = my_plan.structures
     if data_dir is None:
-        data_dir = os.path.join(Path(__file__).parents[2], 'data', my_plan.patient_id)
-    ct_arr = my_plan.ct['ct_hu_3d'][0]
-    ct = sitk.GetImageFromArray(ct_arr)
-    ct.SetOrigin(my_plan.ct['origin_xyz_mm'])
-    ct.SetSpacing(my_plan.ct['resolution_xyz_mm'])
-    ct.SetDirection(my_plan.ct['direction'])
-    sitk.WriteImage(ct, os.path.join(data_dir, ct_filename + '.nrrd'))
+        data_dir = os.path.join(Path(__file__).parents[2], 'data', ct.patient_id)
+    elif not os.path.exists(data_dir):
+        os.makedirs(data_dir)
 
-    if sol['inf_matrix'].dose_3d is None:
+    ct_arr = ct.ct_dict['ct_hu_3d'][0]
+    ct_image = sitk.GetImageFromArray(ct_arr)
+    ct_image.SetOrigin(ct.ct_dict['origin_xyz_mm'])
+    ct_image.SetSpacing(ct.ct_dict['resolution_xyz_mm'])
+    ct_image.SetDirection(ct.ct_dict['direction'])
+    sitk.WriteImage(ct_image, os.path.join(data_dir, ct_filename + '.nrrd'))
+
+    dose_arr = []
+    if sol is not None:
         dose_1d = sol['inf_matrix'].A @ (sol['optimal_intensity']*my_plan.get_num_of_fractions())
         dose_arr = sol['inf_matrix'].dose_1d_to_3d(dose_1d=dose_1d)
-    else:
-        dose_arr = sol['inf_matrix'].dose_3d
     dose = sitk.GetImageFromArray(dose_arr)
-    dose.SetOrigin(my_plan.ct['origin_xyz_mm'])
-    dose.SetSpacing(my_plan.ct['resolution_xyz_mm'])
-    dose.SetDirection(my_plan.ct['direction'])
+    dose.SetOrigin(ct.ct_dict['origin_xyz_mm'])
+    dose.SetSpacing(ct.ct_dict['resolution_xyz_mm'])
+    dose.SetDirection(ct.ct_dict['direction'])
     sitk.WriteImage(dose, os.path.join(data_dir, dose_filename + '.nrrd'))
 
-    labels = my_plan.structures.structures_dict['structure_mask_3d']
+    labels = structs.structures_dict['structure_mask_3d']
     mask_arr = np.array(labels).transpose((1, 2, 3, 0))
     mask = sitk.GetImageFromArray(mask_arr.astype('uint8'))
     # for i, struct_name in enumerate(my_plan.structures.structures_dict['name']):
     #     segment_name = "Segment{0}_Name".format(i)
     #     mask.SetMetaData(segment_name, struct_name)
-    mask.SetOrigin(my_plan.ct['origin_xyz_mm'])
-    mask.SetSpacing(my_plan.ct['resolution_xyz_mm'])
-    mask.SetDirection(my_plan.ct['direction'])
+    mask.SetOrigin(ct.ct_dict['origin_xyz_mm'])
+    mask.SetSpacing(ct.ct_dict['resolution_xyz_mm'])
+    mask.SetDirection(ct.ct_dict['direction'])
     sitk.WriteImage(mask, os.path.join(data_dir, rt_struct_filename + '.seg.nrrd'), True)
     # my_plan.visualize.patient_name = my_plan.patient_name
```

### Comparing `portpy-0.0.1/portpy/photon/utils/save_or_load_pickle.py` & `portpy-0.0.2/portpy/photon/utils/save_or_load_pickle.py`

 * *Files identical despite different names*

### Comparing `portpy-0.0.1/portpy/photon/utils/slicer_script.py` & `portpy-0.0.2/portpy/photon/utils/slicer_script.py`

 * *Files 8% similar despite different names*

```diff
@@ -26,8 +26,8 @@
 struct_list = sys.argv[2].split(',')
 # print(struct_list)
 # struct_list = ['PTV', 'CTV', 'BLAD_WALL', 'BLADDER_TRIGONE', 'FEMUR_L', 'FEMUR_R', 'RECT_WALL', 'URETHRA', 'SKIN', 'RIND_0', 'RIND_1', 'RIND_2', 'RIND_3', 'RIND_4']
 for i in range(len(struct_list)):
     segment = segmentation.GetNthSegment(i)
     segment.SetName(struct_list[i])
 
-# structure node
+# struct_name node
```

### Comparing `portpy-0.0.1/portpy/photon/utils/sol_change_inf_matrix.py` & `portpy-0.0.2/portpy/photon/utils/sol_change_inf_matrix.py`

 * *Files identical despite different names*

### Comparing `portpy-0.0.1/portpy/photon/utils/view_in_slicer_jupyter.py` & `portpy-0.0.2/portpy/photon/utils/view_in_slicer_jupyter.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 
     :param my_plan: object of class plan
     :param dose_1d: dose in 1d
     :param sol: solution dictionary
     :param ct_name: Default to 'ct'. name of the ct node in 3D slicer
     :param dose_name: Default to 'dose'. name of the dose node in 3D slicer
     :param struct_set_name: name of the rtstruct
-    :param show_structs: default to True. If false, will not create structure node
+    :param show_structs: default to True. If false, will not create struct_name node
     :param show_dose: default to True. If false, will not create dose node
     :param show_ct:default to True. If false, will not create ct node
     :return: visualize in slicer jupyter
     """
     try:
         import slicer
     except ImportError:
@@ -61,15 +61,15 @@
         slicer.util.setSliceViewerLayers(foregroundOpacity=0.4)
         # dose_node.GetVolumeDisplayNode.
 
     # plot structures
     if show_structs:
         structure_node = slicer.mrmlScene.AddNewNodeByClass("vtkMRMLSegmentationNode", struct_set_name)
         for i, struct_name in enumerate(my_plan.structures.structures_dict['name']):
-            print('Importing structure : ' + struct_name)
+            print('Importing struct_name : ' + struct_name)
             slicer.util.addVolumeFromArray(my_plan.structures.structures_dict['structure_mask_3d'][i] * (i + 1),
                                            name=struct_name, nodeClassName="vtkMRMLLabelMapVolumeNode")
             lmap = slicer.util.getNode(struct_name)
             lmap.SetOrigin(list(np.array(my_plan.ct['origin_xyz_mm']) * np.array([-1, -1, 1])))
             lmap.SetSpacing(my_plan.ct['resolution_xyz_mm'])
             lmap.SetIJKToRASDirections(np.array([[-1, 0, 0], [0, -1, 0], [0, 0, 1]]))
             slicer.modules.segmentations.logic().ImportLabelmapToSegmentationNode(lmap, structure_node)
```

### Comparing `portpy-0.0.1/portpy.egg-info/PKG-INFO` & `portpy-0.0.2/portpy.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,79 +1,84 @@
 Metadata-Version: 2.1
 Name: portpy
-Version: 0.0.1
+Version: 0.0.2
 Summary: First open-source radiation treatment planning system in Python
-Home-page: https://github.com/PortPy-Project/PortPy-Photon
+Home-page: https://github.com/PortPy-Project/PortPy
 Author: Gourav Jhanwar, Mojtaba Tefagh, Vicki Taasti, Seppo Tuomaala, Saad Nadeem, Masoud Zarepisheh
 Author-email: jhanwarg@mskcc.struct, mtefagh@acm.struct, vicki.taasti@maastro.nl, tuomaals@mskcc.struct, nadeems@mskcc.struct, zarepism@mskcc.struct
 License: Apache License, Version 2.0
 Description: <p align="center">
           <img src="./images/PortPy_logo.jpg" width="50%">
         </p>
         
         # What is PortPy?
-        **Note: The package is at its early stages of development (version 0.0.3) and we are now collecting feedback from researchers to further refine the data structure and the main functionality. We are expecting to have a stable version 1.xx around March 2023. We would love to hear your feedback.**
+        **Note: The package is at its early stages of development (version 0.0.1) and we are now collecting feedback from researchers to further refine the data structure and the main functionality. We are expecting to have a stable version 1.xx around July 2023. We would love to hear your feedback.**
         
         PortPy (**P**lanning and **O**ptimization for **R**adiation **T**herapy) is a community effort to develop the **first opensource python library** to facilitate the development and clinical translation of radiotherapy cancer treatment planning algorithms. PortPy includes:
         1. Research-ready data and code for *benchmarking*, *reproducibility*, and *community-driven* development.
         2. Interface to an open-source optimization package [CVXPy](https://www.cvxpy.org/) for easy/quick prototyping and out-of-the-box access to commercial/opensource optimization engines (e.g., Mosek, Gorubi, CPLEX, IPOPT).
         3. Visualization modules to visualize relevant plan information (e.g, dose volume histograms, dose distribution, fluence map).
         4. Evaluation modules to quantify plan quality with respect to established clinical metrics (e.g., RTOG metrics, dose conformality, tumor control probability, normal tissue control probability).
         # Data
         Data needed for optimization and algorithm development (e.g., a set of beams/beamlets/voxels, dose contribution of each beamlet to each voxel) are provided for a set of pre-specified machine parameters (e.g., beam/collimator/couch angles). We will initially provide these for a set of publicly available datasets from [TCIA](https://www.cancerimagingarchive.net/). We hope to expand our dataset in the future. The data needed for optimization is extracted from the research version of Eclipse<sup>TM</sup> treatment planning system ([Varian Medical Systems](https://www.varian.com/)) using its API. 
         
         You can download the sample patient data [here](https://drive.google.com/drive/folders/1nA1oHEhlmh2Hk8an9e0Oi0ye6LRPREit?usp=sharing).
         
-        Create a directory named './data' in the current project directory and copy the downloaded file to it, e.g ./data/Lung_Patient_1
+        Create a directory named './data' in the current project directory and copy the downloaded file to it, e.g ./data/Lung_Phantom_Patient_1
         
+        # Quick Start
+        Please see below for understanding the basic functionalities of PortPy. For advance usage of PortPy, we recommend navigating through [examples](https://github.com/PortPy-Project/PortPy/tree/master/examples) folder.
+        1. To understand the most important features of PortPy, we highly recommend to go through notebook [ex_1_introduction.ipynb](https://github.com/PortPy-Project/PortPy/blob/master/examples/ex_1_introduction.ipynb)
+        2. One of the major computational issues while optimizing the plan arise due to large size of influence matrix. We suggest you to follow [ex_2_down_sampling.py](https://github.com/PortPy-Project/PortPy/blob/master/examples/ex_2_downsampling.py) to understand how PortPy can assist in resolving it.
+        3. You can check out [ex_3_structure_operations.py](https://github.com/PortPy-Project/PortPy/blob/master/examples/ex_3_structure_operations.py) to know how to perform different structure operations (e.g., boolean, margin).
+        4. For algorithm benchmarking, the global optimal solution is provided for non-convex optimization problems resulting from beam angle optimization [ex_6_boo_benchmark.py](https://github.com/PortPy-Project/PortPy/blob/master/examples/ex_6_boo_benchmark.py) and incorporating DVH constraints [ex_6_dvh_benchmark.py](https://github.com/PortPy-Project/PortPy/blob/master/examples/ex_6_dvh_benchmark.py) using the mixed-integer programming on down-sampled data.
+        5. In addition to basic visualization capabilities, PortPy provide advanced visualization by integration with 3D Slicer. Please look out notebook [ex_7_Slicer.ipynb](https://github.com/PortPy-Project/PortPy/blob/master/examples/ex_7_Slicer.ipynb)
         
         # Installing PortPy
         
         1. Installing using pip
           ```bash
-          pip install portpy-photon
+          pip install portpy
           ```
         2. Installing using conda
           ```bash
-          conda install -c conda-forge portpy-photon
+          conda install -c conda-forge portpy
           ```
         3. Installing from source
         - Clone this repository:
           ```bash
-          git clone https://github.com/PortPy-Project/PortPy-Photon.git
-          cd portpy_photon
+          git clone https://github.com/PortPy-Project/PortPy.git
+          cd portpy
           ```
         
         - You need to install the dependencies in either a python virtual environment or anaconda environment. Instructions for setting up in python virtual environment are as follows:
         
           Install all the dependencies present in requirements.txt:
           ```bash
           python3 -m venv venv
           source venv/bin/activate
           (venv) pip install -r requirements.txt
           ```
         
-        To better understand the PortPy functionality, we recommend running an example script eg_1_basics.py for creating and visualizing a sample IMRT plan.
-        
-        # License
-        PortPy code is distributed under **Apache 2.0 with Commons Clause** license, and is available for non-commercial academic purposes.
-        
         # Team
         PortPy is a community project initiated at [Memorial Sloan Kettering Cancer Center](https://www.mskcc.org/). It is currently developed and maintained by:
         
         | Name                                                                         | Expertise                                        | Institution |
         |------------------------------------------------------------------------------|--------------------------------------------------|-------------|
         | [Masoud Zarepisheh](https://masoudzp.github.io/)                             | Treatment Planning and Optimization              | MSK         |
         | [Saad Nadeem](https://nadeemlab.org/)                                        | Computer Vision and AI in Medical Imaging        | MSK         |
         | [Gourav Jhanwar](https://github.com/gourav3017)                              | Algorithm Design and Development                 | MSK         |
         | [Mojtaba Tefagh](https://github.com/mtefagh)                                 | Mathematical Modeling and Reinforcement Learning | SUT         |
         | [Vicki Taasti](https://scholar.google.com/citations?user=PEPyvewAAAAJ&hl=en) | Physics and Planning of Proton Therapy           | MAASTRO     |
         | [Sadegh Alam](https://scholar.google.com/citations?user=iy7TlU0AAAAJ&hl=en)  | Adaptive Treatment Planning and Imaging          | Cornell     |
         | [Seppo Tuomaala](https://www.linkedin.com/in/seppo-tuomaala-5b57913/)        | Eclispe API Scripting                            | VARIAN      |
         
+        # License
+        PortPy code is distributed under **Apache 2.0 with Commons Clause** license, and is available for non-commercial academic purposes.
+        
 Platform: UNKNOWN
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `portpy-0.0.1/portpy.egg-info/SOURCES.txt` & `portpy-0.0.2/portpy.egg-info/SOURCES.txt`

 * *Files 18% similar despite different names*

```diff
@@ -1,30 +1,33 @@
 MANIFEST.in
 README.md
 setup.py
+config_files/clinical_criteria/Default/Lung_2Gy_30Fx.json
+config_files/optimization_params/optimization_params_Lung_2Gy_30Fx.json
 images/PortPy_logo.jpg
 portpy/__init__.py
 portpy.egg-info/PKG-INFO
 portpy.egg-info/SOURCES.txt
 portpy.egg-info/dependency_links.txt
 portpy.egg-info/requires.txt
 portpy.egg-info/top_level.txt
 portpy/photon/__init__.py
 portpy/photon/beam.py
 portpy/photon/clinical_criteria.py
+portpy/photon/ct.py
 portpy/photon/cvxpy_prob.py
-portpy/photon/cvxpy_prob_old.py
-portpy/photon/cvxpy_prob_rev2.py
+portpy/photon/data_explorer.py
 portpy/photon/evaluation.py
 portpy/photon/influence_matrix.py
 portpy/photon/optimization.py
 portpy/photon/plan.py
 portpy/photon/structures.py
 portpy/photon/visualization.py
 portpy/photon/utils/__init__.py
+portpy/photon/utils/get_eclipse_fluence.py
 portpy/photon/utils/load_data.py
 portpy/photon/utils/load_metadata.py
 portpy/photon/utils/save_nrrd.py
 portpy/photon/utils/save_or_load_pickle.py
 portpy/photon/utils/slicer_script.py
 portpy/photon/utils/sol_change_inf_matrix.py
 portpy/photon/utils/view_in_slicer_jupyter.py
```

### Comparing `portpy-0.0.1/setup.py` & `portpy-0.0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,15 +21,15 @@
     "6 - Mature",
     "7 - Inactive"
 ]
 
 setup(
     name='portpy',
     version=_VERSION,
-    url='https://github.com/PortPy-Project/PortPy-Photon',
+    url='https://github.com/PortPy-Project/PortPy',
     license='Apache License, Version 2.0',
     packages=find_packages(exclude=["examples*"]),
     author='Gourav Jhanwar, Mojtaba Tefagh, Vicki Taasti, Seppo Tuomaala, Saad Nadeem, Masoud Zarepisheh',
     author_email="jhanwarg@mskcc.struct, mtefagh@acm.struct, vicki.taasti@maastro.nl, tuomaals@mskcc.struct, nadeems@mskcc.struct, zarepism@mskcc.struct",
     description='First open-source radiation treatment planning system in Python',
     long_description=open('README.md').read(),
     long_description_content_type="text/markdown",
```

