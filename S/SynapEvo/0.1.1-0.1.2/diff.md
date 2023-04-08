# Comparing `tmp/SynapEvo-0.1.1.tar.gz` & `tmp/SynapEvo-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "SynapEvo-0.1.1.tar", last modified: Sat Apr  8 17:50:40 2023, max compression
+gzip compressed data, was "SynapEvo-0.1.2.tar", last modified: Sat Apr  8 17:56:53 2023, max compression
```

## Comparing `SynapEvo-0.1.1.tar` & `SynapEvo-0.1.2.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-04-08 17:50:40.399486 SynapEvo-0.1.1/
--rw-rw-rw-   0        0        0     1094 2023-03-30 17:07:49.000000 SynapEvo-0.1.1/LICENSE
--rw-rw-rw-   0        0        0      260 2023-04-08 17:50:40.398488 SynapEvo-0.1.1/PKG-INFO
--rw-rw-rw-   0        0        0      304 2023-04-08 10:17:36.000000 SynapEvo-0.1.1/README.md
--rw-rw-rw-   0        0        0       42 2023-04-08 17:50:40.399486 SynapEvo-0.1.1/setup.cfg
--rw-rw-rw-   0        0        0      503 2023-04-08 17:50:36.000000 SynapEvo-0.1.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-08 17:50:40.363475 SynapEvo-0.1.1/src/
-drwxrwxrwx   0        0        0        0 2023-04-08 17:50:40.386487 SynapEvo-0.1.1/src/SynapEvo/
--rw-rw-rw-   0        0        0     2590 2023-04-08 17:46:09.000000 SynapEvo-0.1.1/src/SynapEvo/NN.py
--rw-rw-rw-   0        0        0     3788 2023-04-08 17:46:56.000000 SynapEvo-0.1.1/src/SynapEvo/NNevo.py
--rw-rw-rw-   0        0        0        2 2023-04-01 17:06:43.000000 SynapEvo-0.1.1/src/SynapEvo/__init__.py
--rw-rw-rw-   0        0        0      983 2023-04-08 17:47:31.000000 SynapEvo-0.1.1/src/SynapEvo/test.py
-drwxrwxrwx   0        0        0        0 2023-04-08 17:50:40.397486 SynapEvo-0.1.1/src/SynapEvo.egg-info/
--rw-rw-rw-   0        0        0      260 2023-04-08 17:50:40.000000 SynapEvo-0.1.1/src/SynapEvo.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      292 2023-04-08 17:50:40.000000 SynapEvo-0.1.1/src/SynapEvo.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-08 17:50:40.000000 SynapEvo-0.1.1/src/SynapEvo.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        6 2023-04-08 17:50:40.000000 SynapEvo-0.1.1/src/SynapEvo.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-04-08 17:50:40.000000 SynapEvo-0.1.1/src/SynapEvo.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-08 17:56:53.723827 SynapEvo-0.1.2/
+-rw-rw-rw-   0        0        0     1094 2023-03-30 17:07:49.000000 SynapEvo-0.1.2/LICENSE
+-rw-rw-rw-   0        0        0      260 2023-04-08 17:56:53.722828 SynapEvo-0.1.2/PKG-INFO
+-rw-rw-rw-   0        0        0      304 2023-04-08 10:17:36.000000 SynapEvo-0.1.2/README.md
+-rw-rw-rw-   0        0        0       42 2023-04-08 17:56:53.723827 SynapEvo-0.1.2/setup.cfg
+-rw-rw-rw-   0        0        0      503 2023-04-08 17:56:24.000000 SynapEvo-0.1.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-08 17:56:53.685832 SynapEvo-0.1.2/src/
+drwxrwxrwx   0        0        0        0 2023-04-08 17:56:53.710834 SynapEvo-0.1.2/src/SynapEvo/
+-rw-rw-rw-   0        0        0     2591 2023-04-08 17:54:56.000000 SynapEvo-0.1.2/src/SynapEvo/NN.py
+-rw-rw-rw-   0        0        0     3788 2023-04-08 17:46:56.000000 SynapEvo-0.1.2/src/SynapEvo/NNevo.py
+-rw-rw-rw-   0        0        0        2 2023-04-01 17:06:43.000000 SynapEvo-0.1.2/src/SynapEvo/__init__.py
+-rw-rw-rw-   0        0        0      983 2023-04-08 17:47:31.000000 SynapEvo-0.1.2/src/SynapEvo/test.py
+drwxrwxrwx   0        0        0        0 2023-04-08 17:56:53.721826 SynapEvo-0.1.2/src/SynapEvo.egg-info/
+-rw-rw-rw-   0        0        0      260 2023-04-08 17:56:53.000000 SynapEvo-0.1.2/src/SynapEvo.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      292 2023-04-08 17:56:53.000000 SynapEvo-0.1.2/src/SynapEvo.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-08 17:56:53.000000 SynapEvo-0.1.2/src/SynapEvo.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        6 2023-04-08 17:56:53.000000 SynapEvo-0.1.2/src/SynapEvo.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-04-08 17:56:53.000000 SynapEvo-0.1.2/src/SynapEvo.egg-info/top_level.txt
```

### Comparing `SynapEvo-0.1.1/LICENSE` & `SynapEvo-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `SynapEvo-0.1.1/src/SynapEvo/NN.py` & `SynapEvo-0.1.2/src/SynapEvo/NN.py`

 * *Files 0% similar despite different names*

```diff
@@ -39,15 +39,15 @@
             np.random.seed(random_state)
 
         for i in range(nlayers):
             if i == 0:
                 # The first layer weight matrix includes the input size
                 self.weights.append(np.random.randn(input_size, layers_sizes))
                 self.biases.append(np.random.randn(layers_sizes))
-                self.activations.append(np.random.choice(range(8), layers_sizes)
+                self.activations.append(np.random.choice(range(8), layers_sizes))
             elif i == nlayers - 1:
                 # The last layer weight matrix includes the output size
                 self.weights.append(np.random.randn(layers_sizes, output_size))
                 self.biases.append(np.random.randn(output_size))
                 self.activations.append(np.random.choice(range(8), output_size))
             else:
                 # Subsequent layers have weights only based on the layer size
```

### Comparing `SynapEvo-0.1.1/src/SynapEvo/NNevo.py` & `SynapEvo-0.1.2/src/SynapEvo/NNevo.py`

 * *Files identical despite different names*

### Comparing `SynapEvo-0.1.1/src/SynapEvo/test.py` & `SynapEvo-0.1.2/src/SynapEvo/test.py`

 * *Files identical despite different names*

