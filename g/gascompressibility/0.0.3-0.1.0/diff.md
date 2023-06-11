# Comparing `tmp/gascompressibility-0.0.3.tar.gz` & `tmp/gascompressibility-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gascompressibility-0.0.3.tar", last modified: Mon May 29 07:16:19 2023, max compression
+gzip compressed data, was "gascompressibility-0.1.0.tar", last modified: Sun Jun 11 20:32:19 2023, max compression
```

## Comparing `gascompressibility-0.0.3.tar` & `gascompressibility-0.1.0.tar`

### file list

```diff
@@ -1,18 +1,32 @@
-drwxrwxrwx   0        0        0        0 2023-05-29 07:16:19.988836 gascompressibility-0.0.3/
--rw-rw-rw-   0        0        0     1095 2023-05-23 14:19:22.000000 gascompressibility-0.0.3/LICENSE
--rw-rw-rw-   0        0        0     2094 2023-05-29 07:16:19.988836 gascompressibility-0.0.3/PKG-INFO
--rw-rw-rw-   0        0        0     1134 2023-05-29 07:13:43.000000 gascompressibility-0.0.3/README.md
-drwxrwxrwx   0        0        0        0 2023-05-29 07:16:19.976836 gascompressibility-0.0.3/gascompressibility/
--rw-rw-rw-   0        0        0       89 2023-05-25 15:06:36.000000 gascompressibility-0.0.3/gascompressibility/__init__.py
--rw-rw-rw-   0        0        0    23949 2023-05-29 05:17:48.000000 gascompressibility-0.0.3/gascompressibility/zfactor.py
-drwxrwxrwx   0        0        0        0 2023-05-29 07:16:19.986837 gascompressibility-0.0.3/gascompressibility.egg-info/
--rw-rw-rw-   0        0        0     2094 2023-05-29 07:16:19.000000 gascompressibility-0.0.3/gascompressibility.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      336 2023-05-29 07:16:19.000000 gascompressibility-0.0.3/gascompressibility.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-29 07:16:19.000000 gascompressibility-0.0.3/gascompressibility.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       45 2023-05-29 07:16:19.000000 gascompressibility-0.0.3/gascompressibility.egg-info/requires.txt
--rw-rw-rw-   0        0        0       25 2023-05-29 07:16:19.000000 gascompressibility-0.0.3/gascompressibility.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-29 07:16:19.988836 gascompressibility-0.0.3/setup.cfg
--rw-rw-rw-   0        0        0     1198 2023-05-29 07:16:14.000000 gascompressibility-0.0.3/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-29 07:16:19.987837 gascompressibility-0.0.3/tests/
--rw-rw-rw-   0        0        0       77 2023-05-25 15:06:36.000000 gascompressibility-0.0.3/tests/__init__.py
--rw-rw-rw-   0        0        0     9581 2023-05-29 05:23:18.000000 gascompressibility-0.0.3/tests/test_gascomp.py
+drwxrwxrwx   0        0        0        0 2023-06-11 20:32:19.744045 gascompressibility-0.1.0/
+-rw-rw-rw-   0        0        0     1095 2023-05-23 14:19:22.000000 gascompressibility-0.1.0/LICENSE
+-rw-rw-rw-   0        0        0    11089 2023-06-11 20:32:19.743045 gascompressibility-0.1.0/PKG-INFO
+-rw-rw-rw-   0        0        0    10113 2023-06-11 01:23:44.000000 gascompressibility-0.1.0/README.md
+drwxrwxrwx   0        0        0        0 2023-06-11 20:32:19.720999 gascompressibility-0.1.0/gascompressibility/
+-rw-rw-rw-   0        0        0      220 2023-06-10 23:57:14.000000 gascompressibility-0.1.0/gascompressibility/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-11 20:32:19.734998 gascompressibility-0.1.0/gascompressibility/pseudocritical/
+-rw-rw-rw-   0        0        0        0 2023-05-31 21:11:20.000000 gascompressibility-0.1.0/gascompressibility/pseudocritical/__init__.py
+-rw-rw-rw-   0        0        0    14812 2023-06-11 01:43:49.000000 gascompressibility-0.1.0/gascompressibility/pseudocritical/piper.py
+-rw-rw-rw-   0        0        0    16380 2023-06-11 01:47:21.000000 gascompressibility-0.1.0/gascompressibility/pseudocritical/sutton.py
+drwxrwxrwx   0        0        0        0 2023-06-11 20:32:19.736998 gascompressibility-0.1.0/gascompressibility/utilities/
+-rw-rw-rw-   0        0        0        0 2023-05-31 21:10:39.000000 gascompressibility-0.1.0/gascompressibility/utilities/__init__.py
+-rw-rw-rw-   0        0        0      162 2023-06-06 18:54:16.000000 gascompressibility-0.1.0/gascompressibility/utilities/utilities.py
+drwxrwxrwx   0        0        0        0 2023-06-11 20:32:19.741043 gascompressibility-0.1.0/gascompressibility/z_correlation/
+-rw-rw-rw-   0        0        0     1088 2023-06-11 02:01:39.000000 gascompressibility-0.1.0/gascompressibility/z_correlation/DAK.py
+-rw-rw-rw-   0        0        0        0 2023-06-10 02:22:58.000000 gascompressibility-0.1.0/gascompressibility/z_correlation/__init__.py
+-rw-rw-rw-   0        0        0      746 2023-06-11 02:05:15.000000 gascompressibility-0.1.0/gascompressibility/z_correlation/hall_yarborough.py
+-rw-rw-rw-   0        0        0     1871 2023-06-11 04:54:16.000000 gascompressibility-0.1.0/gascompressibility/z_correlation/kareem.py
+-rw-rw-rw-   0        0        0     1195 2023-06-11 03:43:15.000000 gascompressibility-0.1.0/gascompressibility/z_correlation/londono.py
+-rw-rw-rw-   0        0        0     1463 2023-06-11 05:13:08.000000 gascompressibility-0.1.0/gascompressibility/z_correlation/z_helper.py
+-rw-rw-rw-   0        0        0    24973 2023-05-31 14:14:57.000000 gascompressibility-0.1.0/gascompressibility/zfactor.py
+drwxrwxrwx   0        0        0        0 2023-06-11 20:32:19.732999 gascompressibility-0.1.0/gascompressibility.egg-info/
+-rw-rw-rw-   0        0        0    11089 2023-06-11 20:32:19.000000 gascompressibility-0.1.0/gascompressibility.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      821 2023-06-11 20:32:19.000000 gascompressibility-0.1.0/gascompressibility.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-11 20:32:19.000000 gascompressibility-0.1.0/gascompressibility.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       43 2023-06-11 20:32:19.000000 gascompressibility-0.1.0/gascompressibility.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       25 2023-06-11 20:32:19.000000 gascompressibility-0.1.0/gascompressibility.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-11 20:32:19.744045 gascompressibility-0.1.0/setup.cfg
+-rw-rw-rw-   0        0        0     1418 2023-06-11 20:32:09.000000 gascompressibility-0.1.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-11 20:32:19.743045 gascompressibility-0.1.0/tests/
+-rw-rw-rw-   0        0        0      137 2023-06-10 01:30:30.000000 gascompressibility-0.1.0/tests/__init__.py
+-rw-rw-rw-   0        0        0    32341 2023-06-11 05:14:37.000000 gascompressibility-0.1.0/tests/test_gascomp.py
```

### Comparing `gascompressibility-0.0.3/LICENSE` & `gascompressibility-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `gascompressibility-0.0.3/gascompressibility/zfactor.py` & `gascompressibility-0.1.0/gascompressibility/zfactor.py`

 * *Files 4% similar despite different names*

```diff
@@ -71,66 +71,71 @@
 
         self._calc_from = None
 
     def __str__(self):
         return str(self.Z)
 
     def __repr__(self):
-        return '1'
+        return '<GasCompressibilityFactor object. Mixing Rule = %s>' % self.mode
 
     def calc_Fahrenheit_to_Rankine(self, _T):
+        self._calc_from = 'calc_Fahrenheit_to_Rankine()'
         if _T is None:
             raise TypeError("Missing a required argument, 'T' (gas temperature, °F)")
         self._T = _T  # Fahrenheit
         self.T = _T + 459.67  # Rankine, Rankine is used for calculation below
         return self.T
 
     """pseudo-critical temperature (°R)"""
     def calc_Tpc(self, sg=None, H2S=None, CO2=None, N2=None, J=None, K=None):
+        self._calc_from = 'calc_Tpc()'
         if self.mode == 'sutton':
-            self._initialize_sg(sg, calc_from='Tpc')
+            self._initialize_sg(sg)
             self.Tpc = 169.2 + 349.5 * self.sg - 74.0 * self.sg ** 2
         else:  # mode == 'piper'
             self._redundant_argument_check_J_or_K(sg=sg, J=J, K=K, H2S=H2S, CO2=CO2, N2=N2)
             self._initialize_J(J, sg=sg, H2S=H2S, CO2=CO2, N2=N2)
             self._initialize_K(K, sg=sg, H2S=H2S, CO2=CO2, N2=N2)
             self.Tpc = self.K ** 2 / self.J
         return self.Tpc
 
     """pseudo-critical pressure (psi)"""
     def calc_Ppc(self, sg=None, H2S=None, CO2=None, N2=None, J=None, K=None, Tpc=None):
+        self._calc_from = 'calc_Ppc()'
         if self.mode == 'sutton':
-            self._initialize_sg(sg, calc_from='Ppc')
+            self._initialize_sg(sg)
             self.Ppc = 756.8 - 131.07 * self.sg - 3.6 * self.sg ** 2
         else:  # mode = 'piper'
             self._redundant_argument_check_J_or_K(sg=sg, J=J, K=K, H2S=H2S, CO2=CO2, N2=N2)
             if Tpc is not None:
                 if K is not None:
                     raise TypeError("Redundant arguments 'Tpc' and 'K', input only one of them")
             self._initialize_Tpc(Tpc, sg=sg, H2S=H2S, CO2=CO2, N2=N2, J=J, K=K)
             self._initialize_J(J, sg=sg, H2S=H2S, CO2=CO2, N2=N2)
             self.Ppc = self.Tpc / self.J
         return self.Ppc
 
     """sum of the mole fractions of CO2 and H2S in a gas mixture"""
     def calc_A(self, H2S=None, CO2=None):
+        self._calc_from = 'calc_A()'
         self._initialize_H2S(H2S)
         self._initialize_CO2(CO2)
         self.A = self.H2S + self.CO2
         return self.A
 
     """mole fraction of H2S in a gas mixture"""
     def calc_B(self, H2S=None):
+        self._calc_from = 'calc_B()'
         self._initialize_H2S(H2S)
         self.B = self.H2S
         return self.B
 
     """correction for CO2 and H2S (°R)"""
     def calc_e_correction(self, A=None, B=None, H2S=None, CO2=None):
-
+        self._calc_from = 'calc_e_correction()'
         if A is not None:
             if CO2 is not None:
                 raise TypeError("Redundant arguments 'A' and 'CO2', input only one of them")
             if H2S is not None:
                 raise TypeError("Redundant arguments 'A' and 'H2S', input only one of them")
         if B is not None:
             if H2S is not None:
@@ -140,77 +145,82 @@
 
         self._initialize_A(A, H2S=H2S, CO2=CO2)
         self._initialize_B(B, H2S=H2S)
         self.e_correction = 120 * (self.A ** 0.9 - self.A ** 1.6) + 15 * (self.B ** 0.5 - self.B ** 4)
         return self.e_correction
 
     def calc_Tpc_corrected(self, sg=None, Tpc=None, e_correction=None, A=None, B=None, H2S=None, CO2=None):
+        self._calc_from = 'calc_Tpc_corrected()'
         self._initialize_Tpc(Tpc, sg=sg)
         self._initialize_e_correction(e_correction, A=A, B=B, H2S=H2S, CO2=CO2)
         self.Tpc_corrected = self.Tpc - self.e_correction
         return self.Tpc_corrected
 
     """ corrected pseudo-critical pressure (psi)"""
     def calc_Ppc_corrected(self, sg=None, Tpc=None, Ppc=None, e_correction=None, Tpc_corrected=None,
                            A=None, B=None, H2S=None, CO2=None):
-
+        self._calc_from = 'calc_Ppc_corrected()'
         if e_correction is not None:
             if B is None and H2S is None:
                 raise TypeError("Missing a required argument, 'H2S', (mole fraction of H2S, dimensionless)")
 
         self._initialize_Ppc(Ppc, sg=sg)
         self._initialize_B(B, H2S=H2S)
         self._initialize_e_correction(e_correction, A=A, B=B, H2S=H2S, CO2=CO2)
         if Tpc_corrected is None:
             self._initialize_Tpc(Tpc, sg=sg)
             self._initialize_Tpc_corrected(Tpc_corrected, sg=sg, Tpc=Tpc, e_correction=e_correction, A=A, B=B, H2S=H2S, CO2=CO2)
         self.Ppc_corrected = (self.Ppc * self.Tpc_corrected) / (self.Tpc - self.B * (1 - self.B) * self.e_correction)
         return self.Ppc_corrected
 
     def calc_J(self, sg=None, H2S=None, CO2=None, N2=None):
-        self._initialize_sg(sg, calc_from='J')
+        self._calc_from = 'calc_J()'
+        self._initialize_sg(sg)
         self._initialize_H2S(H2S)
         self._initialize_CO2(CO2)
         self._initialize_N2(N2)
         self.J = 0.11582 \
                  - 0.45820 * self.H2S * (self.Tc_H2S / self.Pc_H2S) \
                  - 0.90348 * self.CO2 * (self.Tc_CO2 / self.Pc_CO2) \
                  - 0.66026 * self.N2 * (self.Tc_N2 / self.Pc_N2) \
                  + 0.70729 * self.sg \
                  - 0.099397 * self.sg ** 2
         return self.J
 
     def calc_K(self, sg=None, H2S=None, CO2=None, N2=None):
-        self._initialize_sg(sg, calc_from='K')
+        self._calc_from = 'calc_K()'
+        self._initialize_sg(sg)
         self._initialize_H2S(H2S)
         self._initialize_CO2(CO2)
         self._initialize_N2(N2)
         self.K = 3.8216 \
                  - 0.06534 * self.H2S * (self.Tc_H2S / np.sqrt(self.Pc_H2S)) \
                  - 0.42113 * self.CO2 * (self.Tc_CO2 / np.sqrt(self.Pc_CO2)) \
                  - 0.91249 * self.N2 * (self.Tc_N2 / np.sqrt(self.Pc_N2)) \
                  + 17.438 * self.sg \
                  - 3.2191 * self.sg ** 2
         return self.K
 
     """pseudo-reduced temperature (°R)"""
     def calc_Tr(self, T=None, Tpc_corrected=None, sg=None, Tpc=None, e_correction=None, A=None, B=None, H2S=None, CO2=None, N2=None, J=None, K=None):
+        self._calc_from = 'calc_Tr()'
         self._initialize_T(T)
         if self.mode == 'sutton':
             self._redundant_argument_check_Tpc_corrected(sg=sg, Tpc=Tpc, H2S=H2S, CO2=CO2, A=A, B=B, e_correction=e_correction)
             self._initialize_Tpc_corrected(Tpc_corrected, sg=sg, Tpc=Tpc, e_correction=e_correction, A=A, B=B, H2S=H2S, CO2=CO2)
             self.Tr = self.T / self.Tpc_corrected
         else:  # mode == 'piper'
             self._redundant_argument_check_Tpc(Tpc=Tpc, sg=sg, H2S=H2S, CO2=CO2, N2=N2, J=J, K=K)
             self._initialize_Tpc(Tpc, sg=sg, H2S=H2S, CO2=CO2, N2=N2, J=J, K=K)
             self.Tr = self.T / self.Tpc
         return self.Tr
 
     """pseudo-reduced pressure (psi)"""
     def calc_Pr(self, P=None, Ppc_corrected=None, sg=None, Tpc=None, Ppc=None, e_correction=None, Tpc_corrected=None, A=None, B=None, H2S=None, CO2=None, N2=None, J=None, K=None):
+        self._calc_from = 'calc_Pr()'
         self._initialize_P(P)
         if self.mode == 'sutton':
             self._redundant_argument_check_Ppc_corrected(sg=sg, Ppc=Ppc, Tpc_corrected=Tpc_corrected, Tpc=Tpc, H2S=H2S, CO2=CO2, A=None, B=None, e_correction=e_correction)
             self._initialize_Ppc_corrected(Ppc_corrected, sg=sg, Tpc=Tpc, Ppc=Ppc, e_correction=e_correction, Tpc_corrected=Tpc_corrected, A=A, B=B, H2S=H2S, CO2=CO2)
             self.Pr = self.P / self.Ppc_corrected
         else:  # mode == 'piper'
             self._redundant_argument_check_Ppc(Ppc=Ppc, Tpc=Tpc, sg=sg, H2S=H2S, CO2=CO2, N2=N2, J=J, K=K)
@@ -258,25 +268,25 @@
                 ((0.27 * self.Pr) / (z * self.Tr)) ** 2 /
                 self.Tr ** 3
         ) * np.exp(-self.A11 * ((0.27 * self.Pr) / (z * self.Tr)) ** 2) - z
 
     """Newton-Raphson nonlinear solver"""
     def calc_Z(self, guess=0.9, sg=None, P=None, T=None, Tpc=None, Ppc=None, Tpc_corrected=None, Ppc_corrected=None,
                A=None, B=None, H2S=None, CO2=None, N2=None, J=None, K=None, Tr=None, Pr=None, e_correction=None, **kwargs):
-        self._calc_from = 'Z'
+        self._calc_from = 'calc_Z()'
         self._initialize_Pr(Pr, P=P, Ppc_corrected=Ppc_corrected, sg=sg, Tpc=Tpc, Ppc=Ppc, e_correction=e_correction, Tpc_corrected=Tpc_corrected, A=A, B=B, H2S=H2S, CO2=CO2, N2=N2, J=J, K=K)
         self._initialize_Tr(Tr, T, Tpc_corrected=Tpc_corrected, sg=sg, Tpc=Tpc, e_correction=e_correction, A=A, B=B, H2S=H2S, CO2=CO2, N2=N2, J=J, K=K)
         self.Z = optimize.newton(self._calc_Z, guess, **kwargs)
         return self.Z
 
-    def _initialize_sg(self, sg, calc_from=None):
+    def _initialize_sg(self, sg):
         if sg is None:
-            if calc_from == 'Ppc' or calc_from == 'Tpc':
+            if self._calc_from == 'calc_Ppc()' or self._calc_from == 'calc_Tpc()':
                 raise TypeError("Missing a required argument, 'sg' (specific gravity, dimensionless)")
-            elif calc_from == 'J' or calc_from == 'K':
+            elif self._calc_from == 'calc_J()' or self._calc_from == 'calc_K()':
                 raise TypeError("Missing a required argument, 'sg' (specific gravity, dimensionless), or 'J' "
                                 "(Stewart-Burkhardt-VOO parameter, °R/psia), or "
                                 "'K' (Stewart-Burkhardt-VOO parameter, °R/psia^0.5). "
                                 "The calculation requires either "
                                 "1) both 'J' and 'K' provided without 'sg', or "
                                 "2) only 'sg' provided without both 'J' and 'K'")
             else:
@@ -448,38 +458,45 @@
                 raise TypeError("Redundant arguments 'K' and 'N2', input only one of them")
 
     def _redundant_argument_check_Tpc(self, Tpc=None, sg=None, H2S=None, CO2=None, N2=None, J=None, K=None):
         if self.mode == 'piper':
             if Tpc is not None:
                 if sg is not None:
                     raise TypeError("Redundant arguments 'Tpc' and 'sg', input only one of them")
-                if J is not None and self._calc_from != 'Z':
+                if J is not None and self._calc_from != 'calc_Z()':
                     raise TypeError("Redundant arguments 'Tpc' and 'J', input only one of them")
                 if K is not None:
                     raise TypeError("Redundant arguments 'Tpc' and 'K', input only one of them")
                 self._redundant_argument_check_J_or_K(J=J, K=K, H2S=H2S, CO2=CO2, N2=N2)
 
     def _redundant_argument_check_Ppc(self, Ppc=None, Tpc=None, sg=None, H2S=None, CO2=None, N2=None, J=None, K=None):
         if self.mode == 'piper':
             if Ppc is not None:
-                if Tpc is not None:
-                    raise TypeError("unexpected keyword argument 'Tpc'")
+                if Tpc is not None and self._calc_from != 'calc_Z()':
+                    raise TypeError("Redundant arguments 'Ppc' and 'Tpc', input only one of them")
                 if sg is not None:
                     raise TypeError("Redundant arguments 'Ppc' and 'sg', input only one of them")
                 if J is not None:
                     raise TypeError("Redundant arguments 'Ppc' and 'J', input only one of them")
                 if K is not None:
                     raise TypeError("Redundant arguments 'Ppc' and 'K', input only one of them")
                 if H2S is not None:
                     raise TypeError("Redundant arguments 'Ppc' and 'H2S', input only one of them")
                 if CO2 is not None:
                     raise TypeError("Redundant arguments 'Ppc' and 'CO2', input only one of them")
                 if N2 is not None:
                     raise TypeError("Redundant arguments 'Ppc' and 'N2', input only one of them")
 
+    def _unused_argument_check(self, sg=None, P=None, T=None, Tpc=None, Ppc=None, Tpc_corrected=None, Ppc_corrected=None,
+               A=None, B=None, H2S=None, CO2=None, N2=None, J=None, K=None, Tr=None, Pr=None, e_correction=None):
+        if self.mode == 'sutton':
+            if K is not None:
+                raise TypeError("Redundant arguments 'Ppc' and 'N2', input only one of them")
+
+
     def quickstart(self):
 
         xmax = 8
         Prs = np.linspace(0, xmax, xmax * 10 + 1)
         Prs = np.array([round(Pr, 1) for Pr in Prs])
 
         Trs = np.array([1.05, 1.1, 1.2, 1.3, 1.4, 1.5, 1.6, 1.7, 1.8, 1.9, 2.0, 2.2, 2.4, 2.6, 2.8, 3.0])
```

### Comparing `gascompressibility-0.0.3/setup.py` & `gascompressibility-0.1.0/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -17,31 +17,40 @@
 def classifiers():
     with open('classifiers.txt') as f:
         return f.read().strip().split('\n')
 
 
 setup(
     name='gascompressibility',
-    version='0.0.3',
+    version='0.1.0',
     packages=find_packages(exclude=[
         "tutorials",
         "LICENSE",
         ".gitignore",
         "README.md",
         "misc",
         ".travis.yml",
         "notes.py",
+        "custom.svg",
+        "testruns.ipynb",
+        "papers",
     ]),
     description='GasCompressibility-py is a Python library for calculating the gas compressibility factor, Z, based on real gas law.',
     long_description=readme(),
     long_description_content_type='text/markdown',
     classifiers=classifiers(),
     license='MIT',
     author='Eric Kim',
     author_email='aegis4048@gmail.com',
     install_requires=[
-        'numpy>=1.21.5',
+        'numpy>=1.22',
         'scipy>=1.9.1',
         'matplotlib>=3.5.1',
     ],
     url='https://github.com/aegis4048/GasCompressibiltiy-py/tree/main',
 )
+
+
+# python setup.py sdist bdist_wheel
+# twine upload --skip-existing dist/*
+
+# python -m twine upload --skip-existing --repository testpypi dist/*
```

