# Comparing `tmp/mcnnlib-1.0.0.tar.gz` & `tmp/mcnnlib-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mcnnlib-1.0.0.tar", last modified: Fri Jun  9 13:12:59 2023, max compression
+gzip compressed data, was "mcnnlib-1.0.1.tar", last modified: Sun Jun 11 12:10:40 2023, max compression
```

## Comparing `mcnnlib-1.0.0.tar` & `mcnnlib-1.0.1.tar`

### file list

```diff
@@ -1,42 +1,43 @@
-drwxrwxrwx   0        0        0        0 2023-06-09 13:12:59.026533 mcnnlib-1.0.0/
--rw-rw-rw-   0        0        0     1097 2023-06-09 12:24:49.000000 mcnnlib-1.0.0/LICENSE
--rw-rw-rw-   0        0        0      311 2023-06-09 13:12:59.025530 mcnnlib-1.0.0/PKG-INFO
--rw-rw-rw-   0        0        0     5268 2023-06-09 13:01:56.000000 mcnnlib-1.0.0/README.md
-drwxrwxrwx   0        0        0        0 2023-06-09 13:12:58.957531 mcnnlib-1.0.0/mcnn/
--rw-rw-rw-   0        0        0        0 2021-08-10 17:05:32.000000 mcnnlib-1.0.0/mcnn/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-09 13:12:58.961537 mcnnlib-1.0.0/mcnn/nn/
--rw-rw-rw-   0        0        0      100 2021-08-10 17:05:32.000000 mcnnlib-1.0.0/mcnn/nn/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-09 13:12:58.979533 mcnnlib-1.0.0/mcnn/nn/manifolds/
--rw-rw-rw-   0        0        0      250 2023-06-09 10:11:06.000000 mcnnlib-1.0.0/mcnn/nn/manifolds/__init__.py
--rw-rw-rw-   0        0        0     2089 2023-06-09 08:45:09.000000 mcnnlib-1.0.0/mcnn/nn/manifolds/complex_circle.py
--rw-rw-rw-   0        0        0     1866 2023-06-09 08:47:15.000000 mcnnlib-1.0.0/mcnn/nn/manifolds/complex_euclidean.py
--rw-rw-rw-   0        0        0     2187 2023-06-09 08:48:19.000000 mcnnlib-1.0.0/mcnn/nn/manifolds/complex_sphere.py
--rw-rw-rw-   0        0        0     3523 2023-06-09 08:50:19.000000 mcnnlib-1.0.0/mcnn/nn/manifolds/complex_stiefel.py
--rw-rw-rw-   0        0        0     3607 2022-12-25 15:32:34.000000 mcnnlib-1.0.0/mcnn/nn/manifolds/manifold.py
--rw-rw-rw-   0        0        0     4420 2023-06-09 10:07:19.000000 mcnnlib-1.0.0/mcnn/nn/manifolds/manifold_factory.py
-drwxrwxrwx   0        0        0        0 2023-06-09 13:12:58.987535 mcnnlib-1.0.0/mcnn/nn/modules/
--rw-rw-rw-   0        0        0       99 2023-06-09 09:29:42.000000 mcnnlib-1.0.0/mcnn/nn/modules/__init__.py
--rw-rw-rw-   0        0        0     5777 2023-06-09 10:11:59.000000 mcnnlib-1.0.0/mcnn/nn/modules/conv.py
--rw-rw-rw-   0        0        0     1648 2023-06-09 09:28:58.000000 mcnnlib-1.0.0/mcnn/nn/modules/linear.py
--rw-rw-rw-   0        0        0       96 2021-08-10 17:05:32.000000 mcnnlib-1.0.0/mcnn/nn/modules/utils.py
--rw-rw-rw-   0        0        0     1161 2021-08-10 17:05:32.000000 mcnnlib-1.0.0/mcnn/nn/parameter.py
-drwxrwxrwx   0        0        0        0 2023-06-09 13:12:58.991533 mcnnlib-1.0.0/mcnn/nn/utils/
--rw-rw-rw-   0        0        0        0 2021-08-10 17:05:32.000000 mcnnlib-1.0.0/mcnn/nn/utils/__init__.py
--rw-rw-rw-   0        0        0      794 2023-06-09 08:58:59.000000 mcnnlib-1.0.0/mcnn/nn/utils/manifold_multi.py
-drwxrwxrwx   0        0        0        0 2023-06-09 13:12:59.008531 mcnnlib-1.0.0/mcnn/optim/
--rw-rw-rw-   0        0        0      296 2023-06-09 10:10:46.000000 mcnnlib-1.0.0/mcnn/optim/__init__.py
--rw-rw-rw-   0        0        0     8408 2023-06-09 09:01:03.000000 mcnnlib-1.0.0/mcnn/optim/conjugate_gradient.py
--rw-rw-rw-   0        0        0     3713 2023-06-09 09:31:53.000000 mcnnlib-1.0.0/mcnn/optim/manifold_RMSprop.py
--rw-rw-rw-   0        0        0     3330 2023-06-09 09:31:23.000000 mcnnlib-1.0.0/mcnn/optim/manifold_adagrad.py
--rw-rw-rw-   0        0        0     2343 2023-06-09 09:32:05.000000 mcnnlib-1.0.0/mcnn/optim/manifold_sgd.py
--rw-rw-rw-   0        0        0     4280 2023-06-09 09:33:24.000000 mcnnlib-1.0.0/mcnn/optim/quantified_manifold_RMSprop.py
--rw-rw-rw-   0        0        0     3944 2023-06-09 09:33:05.000000 mcnnlib-1.0.0/mcnn/optim/quantified_manifold_adagrad.py
-drwxrwxrwx   0        0        0        0 2023-06-09 13:12:59.022531 mcnnlib-1.0.0/mcnnlib.egg-info/
--rw-rw-rw-   0        0        0      311 2023-06-09 13:12:58.000000 mcnnlib-1.0.0/mcnnlib.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      904 2023-06-09 13:12:58.000000 mcnnlib-1.0.0/mcnnlib.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-09 13:12:58.000000 mcnnlib-1.0.0/mcnnlib.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-06-09 13:12:58.000000 mcnnlib-1.0.0/mcnnlib.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       11 2023-06-09 13:12:58.000000 mcnnlib-1.0.0/mcnnlib.egg-info/requires.txt
--rw-rw-rw-   0        0        0        5 2023-06-09 13:12:58.000000 mcnnlib-1.0.0/mcnnlib.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-09 13:12:59.026533 mcnnlib-1.0.0/setup.cfg
--rw-rw-rw-   0        0        0      465 2023-06-09 13:07:37.000000 mcnnlib-1.0.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-11 12:10:40.281655 mcnnlib-1.0.1/
+-rw-rw-rw-   0        0        0     1097 2023-06-09 12:24:49.000000 mcnnlib-1.0.1/LICENSE
+-rw-rw-rw-   0        0        0      311 2023-06-11 12:10:40.280657 mcnnlib-1.0.1/PKG-INFO
+-rw-rw-rw-   0        0        0     5497 2023-06-11 11:57:36.000000 mcnnlib-1.0.1/README.md
+drwxrwxrwx   0        0        0        0 2023-06-11 12:10:40.213655 mcnnlib-1.0.1/mcnn/
+-rw-rw-rw-   0        0        0        0 2021-08-10 17:05:32.000000 mcnnlib-1.0.1/mcnn/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-11 12:10:40.217650 mcnnlib-1.0.1/mcnn/nn/
+-rw-rw-rw-   0        0        0      100 2021-08-10 17:05:32.000000 mcnnlib-1.0.1/mcnn/nn/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-11 12:10:40.233654 mcnnlib-1.0.1/mcnn/nn/manifolds/
+-rw-rw-rw-   0        0        0      250 2023-06-09 10:11:06.000000 mcnnlib-1.0.1/mcnn/nn/manifolds/__init__.py
+-rw-rw-rw-   0        0        0     2141 2023-06-11 11:00:17.000000 mcnnlib-1.0.1/mcnn/nn/manifolds/complex_circle.py
+-rw-rw-rw-   0        0        0     1910 2023-06-11 10:59:43.000000 mcnnlib-1.0.1/mcnn/nn/manifolds/complex_euclidean.py
+-rw-rw-rw-   0        0        0     2239 2023-06-11 11:00:06.000000 mcnnlib-1.0.1/mcnn/nn/manifolds/complex_sphere.py
+-rw-rw-rw-   0        0        0     3573 2023-06-11 11:00:14.000000 mcnnlib-1.0.1/mcnn/nn/manifolds/complex_stiefel.py
+-rw-rw-rw-   0        0        0     3607 2022-12-25 15:32:34.000000 mcnnlib-1.0.1/mcnn/nn/manifolds/manifold.py
+-rw-rw-rw-   0        0        0     4420 2023-06-09 10:07:19.000000 mcnnlib-1.0.1/mcnn/nn/manifolds/manifold_factory.py
+drwxrwxrwx   0        0        0        0 2023-06-11 12:10:40.241657 mcnnlib-1.0.1/mcnn/nn/modules/
+-rw-rw-rw-   0        0        0       99 2023-06-09 09:29:42.000000 mcnnlib-1.0.1/mcnn/nn/modules/__init__.py
+-rw-rw-rw-   0        0        0     5777 2023-06-09 10:11:59.000000 mcnnlib-1.0.1/mcnn/nn/modules/conv.py
+-rw-rw-rw-   0        0        0     1648 2023-06-09 09:28:58.000000 mcnnlib-1.0.1/mcnn/nn/modules/linear.py
+-rw-rw-rw-   0        0        0       96 2021-08-10 17:05:32.000000 mcnnlib-1.0.1/mcnn/nn/modules/utils.py
+-rw-rw-rw-   0        0        0     1161 2021-08-10 17:05:32.000000 mcnnlib-1.0.1/mcnn/nn/parameter.py
+drwxrwxrwx   0        0        0        0 2023-06-11 12:10:40.246658 mcnnlib-1.0.1/mcnn/nn/utils/
+-rw-rw-rw-   0        0        0        0 2021-08-10 17:05:32.000000 mcnnlib-1.0.1/mcnn/nn/utils/__init__.py
+-rw-rw-rw-   0        0        0      794 2023-06-09 08:58:59.000000 mcnnlib-1.0.1/mcnn/nn/utils/manifold_multi.py
+drwxrwxrwx   0        0        0        0 2023-06-11 12:10:40.264653 mcnnlib-1.0.1/mcnn/optim/
+-rw-rw-rw-   0        0        0      336 2023-06-11 11:11:06.000000 mcnnlib-1.0.1/mcnn/optim/__init__.py
+-rw-rw-rw-   0        0        0     8408 2023-06-09 09:01:03.000000 mcnnlib-1.0.1/mcnn/optim/conjugate_gradient.py
+-rw-rw-rw-   0        0        0     3780 2023-06-11 11:49:10.000000 mcnnlib-1.0.1/mcnn/optim/manifold_RMSprop.py
+-rw-rw-rw-   0        0        0     3338 2023-06-11 11:49:24.000000 mcnnlib-1.0.1/mcnn/optim/manifold_adagrad.py
+-rw-rw-rw-   0        0        0     4696 2023-06-11 11:53:38.000000 mcnnlib-1.0.1/mcnn/optim/manifold_adam.py
+-rw-rw-rw-   0        0        0     2343 2023-06-09 09:32:05.000000 mcnnlib-1.0.1/mcnn/optim/manifold_sgd.py
+-rw-rw-rw-   0        0        0     4306 2023-06-11 11:50:06.000000 mcnnlib-1.0.1/mcnn/optim/quantified_manifold_RMSprop.py
+-rw-rw-rw-   0        0        0     4027 2023-06-11 11:49:48.000000 mcnnlib-1.0.1/mcnn/optim/quantified_manifold_adagrad.py
+drwxrwxrwx   0        0        0        0 2023-06-11 12:10:40.278658 mcnnlib-1.0.1/mcnnlib.egg-info/
+-rw-rw-rw-   0        0        0      311 2023-06-11 12:10:39.000000 mcnnlib-1.0.1/mcnnlib.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      932 2023-06-11 12:10:40.000000 mcnnlib-1.0.1/mcnnlib.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-11 12:10:39.000000 mcnnlib-1.0.1/mcnnlib.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-06-11 12:10:39.000000 mcnnlib-1.0.1/mcnnlib.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       11 2023-06-11 12:10:39.000000 mcnnlib-1.0.1/mcnnlib.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        5 2023-06-11 12:10:39.000000 mcnnlib-1.0.1/mcnnlib.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-11 12:10:40.281655 mcnnlib-1.0.1/setup.cfg
+-rw-rw-rw-   0        0        0      467 2023-06-11 12:09:19.000000 mcnnlib-1.0.1/setup.py
```

### Comparing `mcnnlib-1.0.0/LICENSE` & `mcnnlib-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `mcnnlib-1.0.0/README.md` & `mcnnlib-1.0.1/README.md`

 * *Files 19% similar despite different names*

```diff
@@ -4,117 +4,126 @@
 
 ## Overview
 
 `Manifold Constrained Neural Network(MCNN)`为在`PyTorch`中进行f复数约束性优化和流形优化提供了一种简单的方法。无需任何模板，提供开箱即用的优化器、网络层和网络模型，训练代码中没有。只需在构建模型时声明约束条件，即可开始使用。
 
 全连接网络和卷积网络的流形版本：流形全连接网络（`Manifold Linear`） 、流形卷积神经网络（`Manifold Conv`），网络内部的参数均满足特定的流形约束。同时实现了流形网络优化器：流形随机梯度下降优化器（`Manifold SGD`）、流形自适应梯度优化器（`Manifold Adagrad`）、流形均方根传播优化器（`Manifold RMSprop`）。
 
+<center><img src=".\img\arch.png" width = "600" alt="图片名称" align=center /></center>
 
+流形复数神经网络框架基于`PyTorch`开发，针对网络的参数类、网络结构类和优化器类进行修改以适应流形约束。同时定义流形类，规定了各类流形的随机初始化、投影和缩放操作。
 
-<center><img src=".\img\arch.png" style="zoom: 45%;" /></center>
+使用流形全连接网络`ManifoldLinear`和流形卷积网络`ManifoldConv`模块，可以搭建自己的流形复数神经网络。由于流形复数神经网络中的重要组件继承自`PyTorch`，并封装了底层实现，使得框架的使用方式和普通神经网络框架基本一致。下面展示使用流形复数神经网络计算复对称矩阵$A \in \mathbb C^{n\times n}$的最大特征值。
 
-流形复数神经网络框架基于`PyTorch`开发，针对网络的参数类、网络结构类和优化器类进行修改以适应流形约束。同时定义流形类，规定了各类流形的随机初始化、投影和缩放操作。
+最大特征值$\lambda$是下列优化问题的最优解：
 
-使用流形全连接网络`ManifoldLinear`和流形卷积网络`ManifoldConv`模块，可以搭建自己的流形复数神经网络。由于流形复数神经网络中的重要组件继承自`PyTorch`，并封装了底层实现，使得框架的使用方式和普通神经网络框架基本一致。下面展示使用流形复数神经网络求解正交普鲁克问题
 $$
-\begin{equation}
-    \begin{aligned}& \underset{\boldsymbol{C}}{\text{min}} \,\,  \left\Vert \boldsymbol{B}-\boldsymbol{A}\boldsymbol{C}\right\Vert _F \\ &{~\rm s.t.} \,\,\,\,  \boldsymbol{C}^H\boldsymbol{C}=\boldsymbol{I}.
-    \end{aligned}
-\end{equation}
+\max\limits_{x\in\mathbb{C}^n, x \neq 0} \frac{x^H A x}{x^H
+            x}.
 $$
 
-其中$\boldsymbol{A},\boldsymbol{B} \in\mathbb C^{m \times n}$已知，$\boldsymbol{C} \in\mathbb C^{n \times n }$为待求解参数，且满足正交约束。构建的流形神经网络仅包含一个流形全连接层，不使用偏置参数和激活函数，流形全连接层内部参数即表示$\boldsymbol{C}$，使用`Complex Stiefel`流形对全连接层添加正交约束。使用$\| \boldsymbol{B}-\boldsymbol{A}\boldsymbol{C}\| _F$作为损失函数，同时使用`ManifoldRMSprop`优化器优化网络
+可以重写为：
+$$
+\min\limits_{x\in\mathbb{C}^n, \|x\| = 1} -x^H A x.
+$$
+$x$的约束要求$x$满足单位`2-norm`，所以$x$是单位球空间上一点：
+$$
+\mathbb{S}^{n-1} = \{x \in \mathbb{C}^n : x^H x = 1\}.
+$$
+所以我们对$x$添加`Complex Sphere`流形约束。
 
 ```python
-import matplotlib.pyplot as plt
-import numpy as np
 import torch
-import torch.nn as nn
+from torch.linalg import eigvalsh
+from torch import nn
 import mcnn.nn as mnn
-import mcnn.optim as moptim
+import mcnn.optim as mopt
+import matplotlib.pyplot as plt
 
-# 网络模型
-class OPPNet(nn.Module):
+N = 1000  # matrix size
+LR = 1.0 / N  # step-size.
 
-    def __init__(self, m):
-        super(OPPNet, self).__init__()
-        self.c = mnn.ManifoldLinear(m, m, weight_manifold=mnn.ComplexStiefel, bias=False).to(torch.complex128).weight
-
-    def forward(self, a,b):
-        loss = torch.linalg.norm(b-a@self.c)
-        return loss
-
-n=16
-epoch=512
-err_list=np.zeros(epoch)
-err_opt=0
-repeat=32
-
-for _ in range(repeat):
-    
-    A = np.random.randn(n*2, n)+1j*np.random.randn(n*2, n)
-    C, _ = np.linalg.qr(np.random.randn(n, n)+1j*np.random.randn(n, n))
-    B = A@C+0.01*(np.random.randn(n*2, n)+1j*np.random.randn(n*2, n))
-    
-    # 闭式最优解
-    U, _, V_h = np.linalg.svd(B.T.conj()@A)
-    O = (U@V_h).T.conj()
-    err_opt+=np.linalg.norm(A@O-B)
-
-    A = torch.from_numpy(A)
-    B = torch.from_numpy(B)
-    C = torch.from_numpy(C)
-    
-    net = OPPNet(n)
-    optimizer = moptim.ManifoldRMSprop(net.parameters(), lr=0.01)
-    scheduler = torch.optim.lr_scheduler.ReduceLROnPlateau (optimizer, factor=0.5,patience=12, verbose=False)
-    min_loss = 1e3
-    
-    for i in range(epoch):
-        loss = net(A,B)
-        net.zero_grad()
-        loss.backward()
-        optimizer.step()
-        scheduler.step(loss)
-        if loss < min_loss:
-            min_loss = loss
-        err_list[i]+=loss.detach().numpy()
-    
-    # 列正交验证
-    w = net.c.detach()
-    assert  torch.linalg.norm(torch.eye(n)-w.T.conj()@w).item()<1e-6
+class Model(nn.Module):
+    def __init__(self, n):
+        super().__init__()
+        self.x = mnn.ManifoldLinear(1, n, weight_manifold=mnn.ComplexSphere, bias=False).to(torch.complex64).weight
+
+    def forward(self, A):
+        x = self.x
+        return x.T.conj() @ A @ x
+
+# Generate matrix
+A = torch.rand(N, N)+1j*torch.rand(N, N)  # Uniform on [0, 1)
+A = 0.5 * (A + A.T.conj())
+
+# Compare against diagonalization (eigenvalues are returend in ascending order)
+max_eigenvalue = eigvalsh(A)[-1]
+print("Max eigenvalue: {:10.5f}".format(max_eigenvalue))
+
+# Instantiate model and optimiser
+model = Model(N)
+optim = mopt.ConjugateGradient(model.parameters(), lr=LR)
+
+eigenvalue = float("inf")
+i = 0
+err_list = []
+while (eigenvalue - max_eigenvalue).abs() > 1e-3:
+    eigenvalue = model(A)
+    optim.zero_grad()
+    (-eigenvalue).backward()
+    optim.step()
+    print("{:2}. Best guess: {:10.5f}".format(i, eigenvalue.item()))
+    i += 1
+    err_list.append((eigenvalue - max_eigenvalue).abs().item())
 
+print("Final error {:.5f}".format((eigenvalue - max_eigenvalue).abs().item()))
 plt.figure()
-plt.plot(err_list/repeat)
-plt.plot([err_opt/repeat for _ in range(epoch)])
-plt.xlabel('update')
-plt.ylabel('err')
-plt.legend(['mcnn','opt'])
+plt.plot(err_list, marker='.')
+plt.yscale('log')
+plt.xlabel('Iteration numbers')
+plt.ylabel('error')
 plt.show()
 ```
 
+<center><img src="img\err_plot.png" width = "600" alt="图片名称" align=center /></center>
+
 ## Constraints
 
 支持的流形约束：
 
-* `Complex Sphere`，复球流形，满足约束：$\boldsymbol X \in \mathbb C^{m\times n},\|\boldsymbol X\|_F=1$
-* `Complex Stiefel`，复Stiefel流形，满足约束：$\boldsymbol X \in \mathbb C^{m\times n},\boldsymbol{X}^H\boldsymbol{X}=\boldsymbol{I}$
-* `Complex Circle`，复单位圆流形，满足约束：$\boldsymbol X \in \mathbb C^{m\times n},|[\boldsymbol{X}]_{i,j}|=1$
-* `Complex Euclid`，复欧几里得流形，满足约束：$\boldsymbol X \in \mathbb C^{m\times n}$
+* `Complex Sphere`，复球流形，满足约束：$ X \in \mathbb C^{m\times n},\| X\|_F=1$
+* `Complex Stiefel`，复Stiefel流形，满足约束：$ X \in \mathbb C^{m\times n},{X}^H{X}={I}$
+* `Complex Circle`，复单位圆流形，满足约束：$ X \in \mathbb C^{m\times n},|[{X}]_{i,j}|=1$
+* `Complex Euclid`，复欧几里得流形，满足约束：$ X \in \mathbb C^{m\times n}$
 
 ## Supported Spaces
 
 `mcnn`中的每个约束条件都是以流形的形式实现，这使用户在选择每个参数化的选项时有更大的灵活性。所有流形都支持黎曼梯度下降法，同样也支持其他`PyTorch`优化器。
 
 `mcnn`目前支持以下空间：
 
 * `Cn(n)`: $\mathbb C^n$空间内的无约束优化空间
 * `Sphere(n)`:  $\mathbb C^n$空间内的球体， $\{x\in \mathbb C^n | \|X\|_F=1\} \subset C^n$
 * `SO(n)`:  `n×n` 正交矩阵流形
 * `St(n,k)`:  `n×k` 列正交矩阵流形
 
-## Using MCNN in your Code
+## optimizers
 
-* 安装`mcnn`:`pip install mcnnshit==1.0.0`
+支持的优化器：
+
+* `Conjugate Gradient`，共轭梯度优化器复球流形
+* `Manifold Adam`，流形自适应动量估计算法优化器
+* `Manifold Adagrad`，流形自适应梯度优化器
+* `Manifold RMSprop`，流形均方根传播优化器
+* `Manifold SGD`，流形统计梯度下降优化器
+* `QManifold Adagrad`，带参数量化的流形自适应梯度优化器
+* `QManifold RMSprop`，带参数量化的流形均方根传播优化器
+
+## Using MCNN in your Code
 
+* 安装`mcnn`:`pip install mcnnlib==1.0.0`
 
+## Reference
 
+* [manopt](https://github.com/NicolasBoumal/manopt) : a Matlab toolbox for optimization on manifolds
+* [Pymanopt](https://github.com/pymanopt/pymanopt): A Python toolbox for optimization on Riemannian manifolds with support for automatic differentiation
+* [McTorch ](https://github.com/mctorch/mctorch): a manifold optimization library for deep learning
```

### Comparing `mcnnlib-1.0.0/mcnn/nn/manifolds/complex_circle.py` & `mcnnlib-1.0.1/mcnn/nn/manifolds/complex_circle.py`

 * *Files 2% similar despite different names*

```diff
@@ -31,22 +31,24 @@
 
     def proj(self, z, u):
         """
         Projection of the Euclidean gradient onto the tangent plane
         """
         return u-torch.real(torch.conj(u)*z)*z
 
-    def inner(self, X, G1, G2):
+    def inner(self, X, G1, G2=None):
+        if G2 == None:
+            G2 = G1
         return torch.real(torch.sum(torch.conj(G1) * G2))
 
     def retr(self, z, v):
         """
         Project the points on the tangent plane back to the manifold space
         """
-        y=z+v
+        y = z+v
         return y/torch.abs(y)
 
     def ehess2rhess(self, z, egrad, ehess, zdot):
         # Euclidean -> Riemannian Hessian.
         return self.proj(z, ehess - torch.real(z*torch.conj(egrad))*zdot)
 
     def norm(self, X, G):
@@ -58,10 +60,10 @@
         return v
 
     def transp(self, x1, x2, d):
         return self.proj(x2, d)
 
     def dist(self, X, Y):
         return torch.norm(torch.real(2*torch.asin(0.5*torch.abs(X-Y))))
-    
-    def lincomb(self, x,a1,a2):
-        return a1-a2
+
+    def lincomb(self, x, a1, a2):
+        return a1-a2
```

### Comparing `mcnnlib-1.0.0/mcnn/nn/manifolds/complex_euclidean.py` & `mcnnlib-1.0.1/mcnn/nn/manifolds/complex_euclidean.py`

 * *Files 9% similar despite different names*

```diff
@@ -29,29 +29,32 @@
 
     def proj(self, z, u):
         """
         Projection of the Euclidean gradient onto the tangent plane
         """
         return u
 
-    def inner(self, X, G1, G2):
+    def inner(self, X, G1, G2=None):
+        if G2 == None:
+            G2 = G1
         return torch.real(torch.sum(torch.conj(G1) * G2))
 
     def retr(self, z, v):
         """
         Project the points on the tangent plane back to the manifold space
         """
         return z+v
-    
+
     def egrad2rgrad(self, X, G):
         return G
-    
+
     def ehess2rhess(self, x, eg, eh, d):
         # Euclidean -> Riemannian Hessian.
         return eh
+
     def norm(self, X, G):
         return torch.norm(G)
 
     def randvec(self, z):
         v = torch.randn(self._n, self._m)*(1j*z)
         v = v/torch.norm(v)
         return v
```

### Comparing `mcnnlib-1.0.0/mcnn/nn/manifolds/complex_sphere.py` & `mcnnlib-1.0.1/mcnn/nn/manifolds/complex_sphere.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 
 
 class ComplexSphere(Manifold):
     """
     Complex Sphere manifold class with internal parameters satisfying the unit F-parameter constraint: A \in \mathbb C^{m\times n},\|A\|_F=1
     For knowledge of complex spherical manifolds see: https://www.nicolasboumal.net/book/  P157
     """
+
     def __init__(self, height, width):
         super(Manifold, self).__init__()
         self._n = height
         self._m = width
         self._dim = 2*(self._n*self._m)-1
         self._size = torch.Size((height, width))
 
@@ -30,15 +31,17 @@
 
     def proj(self, x, d):
         """
         Projection of the Euclidean gradient onto the tangent plane
         """
         return d-x*torch.real(torch.sum(torch.conj(x)*d))
 
-    def inner(self, X, G1, G2):
+    def inner(self, X, G1, G2=None):
+        if G2 == None:
+            G2 = G1
         return torch.real(torch.sum(torch.conj(G1) * G2))
 
     def retr(self, x, d):
         """
         Project the points on the tangent plane back to the manifold space
         """
         y = x+d
@@ -58,10 +61,10 @@
         return d
 
     def transp(self, x1, x2, d):
         return self.proj(x2, d)
 
     def dist(self, X, Y):
         return torch.real(2*torch.asin(0.5*torch.norm(X-Y)))
-    
-    def lincomb(self, x,a1,a2):
-        return a1-a2
+
+    def lincomb(self, x, a1, a2):
+        return a1-a2
```

### Comparing `mcnnlib-1.0.0/mcnn/nn/manifolds/complex_stiefel.py` & `mcnnlib-1.0.1/mcnn/nn/manifolds/complex_stiefel.py`

 * *Files 2% similar despite different names*

```diff
@@ -52,15 +52,17 @@
 
     def proj(self, X, U):
         """
         Projection of the Euclidean gradient onto the tangent plane
         """
         return U - multiprod(X, multiherm(multiprod(multihconj(X), U)))
 
-    def inner(self, X, G1, G2):
+    def inner(self, X, G1, G2=None):
+        if G2 == None:
+            G2 = G1
         return torch.real(torch.sum(torch.conj(G1) * G2))
 
     def retr(self, X, G):
         """
         Project the points on the tangent plane back to the manifold space
         """
         if self._k == 1:
```

### Comparing `mcnnlib-1.0.0/mcnn/nn/manifolds/manifold.py` & `mcnnlib-1.0.1/mcnn/nn/manifolds/manifold.py`

 * *Files identical despite different names*

### Comparing `mcnnlib-1.0.0/mcnn/nn/manifolds/manifold_factory.py` & `mcnnlib-1.0.1/mcnn/nn/manifolds/manifold_factory.py`

 * *Files identical despite different names*

### Comparing `mcnnlib-1.0.0/mcnn/nn/modules/conv.py` & `mcnnlib-1.0.1/mcnn/nn/modules/conv.py`

 * *Files identical despite different names*

### Comparing `mcnnlib-1.0.0/mcnn/nn/modules/linear.py` & `mcnnlib-1.0.1/mcnn/nn/modules/linear.py`

 * *Files identical despite different names*

### Comparing `mcnnlib-1.0.0/mcnn/nn/parameter.py` & `mcnnlib-1.0.1/mcnn/nn/parameter.py`

 * *Files identical despite different names*

### Comparing `mcnnlib-1.0.0/mcnn/nn/utils/manifold_multi.py` & `mcnnlib-1.0.1/mcnn/nn/utils/manifold_multi.py`

 * *Files identical despite different names*

### Comparing `mcnnlib-1.0.0/mcnn/optim/conjugate_gradient.py` & `mcnnlib-1.0.1/mcnn/optim/conjugate_gradient.py`

 * *Files identical despite different names*

### Comparing `mcnnlib-1.0.0/mcnn/optim/manifold_RMSprop.py` & `mcnnlib-1.0.1/mcnn/optim/manifold_RMSprop.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,19 +8,20 @@
 from torch.optim import Adagrad
 
 
 class ManifoldRMSprop(Adagrad):
     """
     Implement Manifold Adagrad algorighm
     """
+
     def __init__(self, params, lr=1e-2, lr_decay=0, weight_decay=0, initial_accumulator_value=0, eps=1e-10):
         super(ManifoldRMSprop, self).__init__(params, lr=lr, lr_decay=lr_decay,
-                                       weight_decay=weight_decay,
-                                       initial_accumulator_value=initial_accumulator_value,
-                                       eps=eps)
+                                              weight_decay=weight_decay,
+                                              initial_accumulator_value=initial_accumulator_value,
+                                              eps=eps)
 
     @torch.no_grad()
     def step(self, closure=None):
         beta = 0.99
         """Performs a single optimization step.
 
         Arguments:
@@ -38,15 +39,17 @@
                     continue
 
                 grad = p.grad
                 state = self.state[p]
 
                 state['step'] += 1
 
-                clr = group['lr'] / (1 + (state['step'] - 1) * group['lr_decay'])
+                # clr = group['lr'] / (1 + (state['step'] - 1) * group['lr_decay'])
+                clr = group['lr']
+
                 if not hasattr(p, 'manifold') or p.manifold is None:
                     if group['weight_decay'] != 0:
                         if p.grad.is_sparse:
                             raise RuntimeError("weight_decay option is not compatible with sparse gradients")
                         grad = grad.add(p, alpha=group['weight_decay'])
 
                     if grad.is_sparse:
@@ -69,14 +72,14 @@
                         # state['sum'].addcmul_(grad, grad, value=1)
                         state['sum'] = beta*state['sum']+(1-beta)*(grad.pow(2))
                         std = state['sum'].sqrt().add_(group['eps'])
                         p.addcdiv_(grad, std, value=-clr)
                 else:
                     if grad.is_sparse:
                         raise RuntimeError('Adagrad with manifold doesn\'t support sparse gradients')
-                    rgrad = p.rgrad.data
+                    manifold = p.manifold
+                    rgrad = manifold.egrad2rgrad(p, grad)
                     state['sum'] = beta*state['sum']+(1-beta)*(rgrad.pow(2))
-                    # state['sum'].add_(rgrad.pow(2))
                     std = state['sum'].sqrt().add_(1e-10)
                     modified_rgrad = p.manifold.proj(p.data, rgrad / std)
                     p.data.add_(p.manifold.retr(p.data, -clr * modified_rgrad) - p.data)
         return loss
```

### Comparing `mcnnlib-1.0.0/mcnn/optim/manifold_adagrad.py` & `mcnnlib-1.0.1/mcnn/optim/manifold_adagrad.py`

 * *Files 5% similar despite different names*

```diff
@@ -3,19 +3,20 @@
 from torch.optim import Adagrad
 
 
 class ManifoldAdagrad(Adagrad):
     """
     Implement Manifold Adagrad algorighm
     """
+
     def __init__(self, params, lr=1e-2, lr_decay=0, weight_decay=0, initial_accumulator_value=0, eps=1e-10):
         super(ManifoldAdagrad, self).__init__(params, lr=lr, lr_decay=lr_decay,
-                                       weight_decay=weight_decay,
-                                       initial_accumulator_value=initial_accumulator_value,
-                                       eps=eps)
+                                              weight_decay=weight_decay,
+                                              initial_accumulator_value=initial_accumulator_value,
+                                              eps=eps)
 
     @torch.no_grad()
     def step(self, closure=None):
         """Performs a single optimization step.
 
         Arguments:
             closure (callable, optional): A closure that reevaluates the model
@@ -61,14 +62,14 @@
                     else:
                         state['sum'].addcmul_(grad, grad, value=1)
                         std = state['sum'].sqrt().add_(group['eps'])
                         p.addcdiv_(grad, std, value=-clr)
                 else:
                     if grad.is_sparse:
                         raise RuntimeError('Adagrad with manifold doesn\'t support sparse gradients')
-                    rgrad = p.rgrad.data
-                    # state['sum'] = 0.9*state['sum']+0.1*(rgrad.pow(2))
+                    manifold = p.manifold
+                    rgrad = manifold.egrad2rgrad(p, grad)
                     state['sum'].add_(rgrad.pow(2))
                     std = state['sum'].sqrt().add_(1e-10)
                     modified_rgrad = p.manifold.proj(p.data, rgrad / std)
                     p.data.add_(p.manifold.retr(p.data, -clr * modified_rgrad) - p.data)
         return loss
```

### Comparing `mcnnlib-1.0.0/mcnn/optim/manifold_sgd.py` & `mcnnlib-1.0.1/mcnn/optim/manifold_sgd.py`

 * *Files identical despite different names*

### Comparing `mcnnlib-1.0.0/mcnn/optim/quantified_manifold_RMSprop.py` & `mcnnlib-1.0.1/mcnn/optim/quantified_manifold_adagrad.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,32 +1,29 @@
-import numpy as np
-import torch
-from torch.optim.optimizer import Optimizer
-from torch.optim import RMSprop
-
-
 import torch
 from torch.optim.optimizer import Optimizer
 from torch.optim import Adagrad
+import numpy as np
 
 
-class QManifoldRMSprop(Adagrad):
+class QManifoldAdagrad(Adagrad):
     """
-    Implement Quantification Manifold RMSprop algorighm
+    Implement Quantification Manifold Adagrad algorighm
     """
-    def __init__(self, params, lr=1e-2, qbit=8, eta=0, lr_decay=0, weight_decay=0, initial_accumulator_value=0, eps=1e-10):
-        super(QManifoldRMSprop, self).__init__(params, lr=lr, lr_decay=lr_decay,
-                                        weight_decay=weight_decay,
-                                        initial_accumulator_value=initial_accumulator_value,
-                                        eps=eps)
+
+    def __init__(self, params, lr=1e-2, qbit=7, eta=64, lr_decay=0, weight_decay=0, initial_accumulator_value=0, eps=1e-10):
+        super(QManifoldAdagrad, self).__init__(params, lr=lr, lr_decay=lr_decay,
+                                               weight_decay=weight_decay,
+                                               initial_accumulator_value=initial_accumulator_value,
+                                               eps=eps)
+        self.qbit = qbit
+        self.eta = eta
         self.Q = 2**qbit
 
     @torch.no_grad()
     def step(self, closure=None):
-        beta = 0.99
         """Performs a single optimization step.
 
         Arguments:
             closure (callable, optional): A closure that reevaluates the model
                 and returns the loss.
         """
         loss = None
@@ -58,37 +55,33 @@
                         size = grad.size()
 
                         def make_sparse(values):
                             constructor = grad.new
                             if grad_indices.dim() == 0 or values.dim() == 0:
                                 return constructor().resize_as_(grad)
                             return constructor(grad_indices, values, size)
-                        # state['sum'].add_(make_sparse(grad_values.pow(2)))
-                        state['sum'] = beta*state['sum']+(1-beta)*(make_sparse(grad_values.pow(2)))
+                        state['sum'].add_(make_sparse(grad_values.pow(2)))
                         std = state['sum'].sparse_mask(grad)
                         std_values = std._values().sqrt_().add_(group['eps'])
                         p.add_(make_sparse(grad_values / std_values), alpha=-clr)
                     else:
-                        # state['sum'].addcmul_(grad, grad, value=1)
-                        state['sum'] = beta*state['sum']+(1-beta)*(grad.pow(2))
+                        state['sum'].addcmul_(grad, grad, value=1)
                         std = state['sum'].sqrt().add_(group['eps'])
                         p.addcdiv_(grad, std, value=-clr)
                 else:
                     if grad.is_sparse:
                         raise RuntimeError('Adagrad with manifold doesn\'t support sparse gradients')
-                    rgrad = p.rgrad.data
-                    state['sum'] = beta*state['sum']+(1-beta)*(rgrad.pow(2))
-                    # state['sum'].add_(rgrad.pow(2))
+                    manifold = p.manifold
+                    rgrad = manifold.egrad2rgrad(p, grad)
+                    state['sum'].add_(rgrad.pow(2))
                     std = state['sum'].sqrt().add_(1e-10)
                     modified_rgrad = p.manifold.proj(p.data, rgrad / std)
-
                     nextpoint = p.manifold.retr(p.data, -clr * modified_rgrad)
                     Q_nextpoint = torch.exp(1j * self.q_theta(torch.angle(nextpoint)))
                     p.data.add_(Q_nextpoint - p.data)
-
         return loss
 
     def q_theta(self, theta):
         """
         Ideal Quantification
         """
         theta_q = torch.zeros(theta.shape).to(theta.device)
```

### Comparing `mcnnlib-1.0.0/mcnn/optim/quantified_manifold_adagrad.py` & `mcnnlib-1.0.1/mcnn/optim/quantified_manifold_RMSprop.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,28 +1,33 @@
+import numpy as np
+import torch
+from torch.optim.optimizer import Optimizer
+from torch.optim import RMSprop
+
+
 import torch
 from torch.optim.optimizer import Optimizer
 from torch.optim import Adagrad
-import numpy as np
 
 
-class QManifoldAdagrad(Adagrad):
+class QManifoldRMSprop(Adagrad):
     """
-    Implement Quantification Manifold Adagrad algorighm
+    Implement Quantification Manifold RMSprop algorighm
     """
-    def __init__(self, params, lr=1e-2, qbit=7, eta=64, lr_decay=0, weight_decay=0, initial_accumulator_value=0, eps=1e-10):
-        super(QManifoldAdagrad, self).__init__(params, lr=lr, lr_decay=lr_decay,
-                                        weight_decay=weight_decay,
-                                        initial_accumulator_value=initial_accumulator_value,
-                                        eps=eps)
-        self.qbit = qbit
-        self.eta = eta
+
+    def __init__(self, params, lr=1e-2, qbit=8, eta=0, lr_decay=0, weight_decay=0, initial_accumulator_value=0, eps=1e-10):
+        super(QManifoldRMSprop, self).__init__(params, lr=lr, lr_decay=lr_decay,
+                                               weight_decay=weight_decay,
+                                               initial_accumulator_value=initial_accumulator_value,
+                                               eps=eps)
         self.Q = 2**qbit
 
     @torch.no_grad()
     def step(self, closure=None):
+        beta = 0.99
         """Performs a single optimization step.
 
         Arguments:
             closure (callable, optional): A closure that reevaluates the model
                 and returns the loss.
         """
         loss = None
@@ -54,32 +59,36 @@
                         size = grad.size()
 
                         def make_sparse(values):
                             constructor = grad.new
                             if grad_indices.dim() == 0 or values.dim() == 0:
                                 return constructor().resize_as_(grad)
                             return constructor(grad_indices, values, size)
-                        state['sum'].add_(make_sparse(grad_values.pow(2)))
+                        # state['sum'].add_(make_sparse(grad_values.pow(2)))
+                        state['sum'] = beta*state['sum']+(1-beta)*(make_sparse(grad_values.pow(2)))
                         std = state['sum'].sparse_mask(grad)
                         std_values = std._values().sqrt_().add_(group['eps'])
                         p.add_(make_sparse(grad_values / std_values), alpha=-clr)
                     else:
-                        state['sum'].addcmul_(grad, grad, value=1)
+                        # state['sum'].addcmul_(grad, grad, value=1)
+                        state['sum'] = beta*state['sum']+(1-beta)*(grad.pow(2))
                         std = state['sum'].sqrt().add_(group['eps'])
                         p.addcdiv_(grad, std, value=-clr)
                 else:
                     if grad.is_sparse:
                         raise RuntimeError('Adagrad with manifold doesn\'t support sparse gradients')
-                    rgrad = p.rgrad.data
-                    state['sum'].add_(rgrad.pow(2))
+                    manifold = p.manifold
+                    rgrad = manifold.egrad2rgrad(p, grad)
+                    state['sum'] = beta*state['sum']+(1-beta)*(rgrad.pow(2))
                     std = state['sum'].sqrt().add_(1e-10)
                     modified_rgrad = p.manifold.proj(p.data, rgrad / std)
                     nextpoint = p.manifold.retr(p.data, -clr * modified_rgrad)
                     Q_nextpoint = torch.exp(1j * self.q_theta(torch.angle(nextpoint)))
                     p.data.add_(Q_nextpoint - p.data)
+
         return loss
 
     def q_theta(self, theta):
         """
         Ideal Quantification
         """
         theta_q = torch.zeros(theta.shape).to(theta.device)
```

### Comparing `mcnnlib-1.0.0/mcnnlib.egg-info/SOURCES.txt` & `mcnnlib-1.0.1/mcnnlib.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -17,14 +17,15 @@
 mcnn/nn/modules/utils.py
 mcnn/nn/utils/__init__.py
 mcnn/nn/utils/manifold_multi.py
 mcnn/optim/__init__.py
 mcnn/optim/conjugate_gradient.py
 mcnn/optim/manifold_RMSprop.py
 mcnn/optim/manifold_adagrad.py
+mcnn/optim/manifold_adam.py
 mcnn/optim/manifold_sgd.py
 mcnn/optim/quantified_manifold_RMSprop.py
 mcnn/optim/quantified_manifold_adagrad.py
 mcnnlib.egg-info/PKG-INFO
 mcnnlib.egg-info/SOURCES.txt
 mcnnlib.egg-info/dependency_links.txt
 mcnnlib.egg-info/not-zip-safe
```

