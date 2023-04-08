# Comparing `tmp/pygad-2.9.0.tar.gz` & `tmp/pygad-3.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pygad-2.9.0.tar", last modified: Sat Dec  5 23:26:03 2020, max compression
+gzip compressed data, was "pygad-3.0.0.tar", last modified: Sat Apr  8 18:31:16 2023, max compression
```

## Comparing `pygad-2.9.0.tar` & `pygad-3.0.0.tar`

### file list

```diff
@@ -1,29 +1,43 @@
-drwxr-xr-x   0 ahmedgad  (1000) ahmedgad  (1000)        0 2020-12-05 23:26:03.000000 pygad-2.9.0/
--rw-r--r--   0 ahmedgad  (1000) ahmedgad  (1000)    21733 2020-12-05 23:26:03.000000 pygad-2.9.0/PKG-INFO
--rw-------   0 ahmedgad  (1000) ahmedgad  (1000)    18659 2020-09-11 17:22:41.000000 pygad-2.9.0/README.md
-drwxr-xr-x   0 ahmedgad  (1000) ahmedgad  (1000)        0 2020-12-05 23:26:03.000000 pygad-2.9.0/pygad/
--rwxrw-rw-   0 ahmedgad  (1000) ahmedgad  (1000)       63 2020-12-05 23:24:45.000000 pygad-2.9.0/pygad/__init__.py
-drwxr-xr-x   0 ahmedgad  (1000) ahmedgad  (1000)        0 2020-12-05 23:26:03.000000 pygad-2.9.0/pygad/cnn/
--rwxrw-rw-   0 ahmedgad  (1000) ahmedgad  (1000)       43 2020-06-01 18:30:10.000000 pygad-2.9.0/pygad/cnn/__init__.py
--rwxrw-rw-   0 ahmedgad  (1000) ahmedgad  (1000)    37968 2020-06-01 17:57:18.000000 pygad-2.9.0/pygad/cnn/cnn.py
-drwxr-xr-x   0 ahmedgad  (1000) ahmedgad  (1000)        0 2020-12-05 23:26:03.000000 pygad-2.9.0/pygad/gacnn/
--rwxrw-rw-   0 ahmedgad  (1000) ahmedgad  (1000)       45 2020-06-01 18:29:52.000000 pygad-2.9.0/pygad/gacnn/__init__.py
--rwxrw-rw-   0 ahmedgad  (1000) ahmedgad  (1000)     5166 2020-06-01 18:30:34.000000 pygad-2.9.0/pygad/gacnn/gacnn.py
-drwxr-xr-x   0 ahmedgad  (1000) ahmedgad  (1000)        0 2020-12-05 23:26:03.000000 pygad-2.9.0/pygad/gann/
--rwxrw-rw-   0 ahmedgad  (1000) ahmedgad  (1000)       44 2020-09-11 18:26:41.000000 pygad-2.9.0/pygad/gann/__init__.py
--rwxrw-rw-   0 ahmedgad  (1000) ahmedgad  (1000)    21058 2020-09-11 18:27:44.000000 pygad-2.9.0/pygad/gann/gann.py
-drwxr-xr-x   0 ahmedgad  (1000) ahmedgad  (1000)        0 2020-12-05 23:26:03.000000 pygad-2.9.0/pygad/kerasga/
--rwxrw-rw-   0 ahmedgad  (1000) ahmedgad  (1000)       47 2020-09-20 20:34:14.000000 pygad-2.9.0/pygad/kerasga/__init__.py
--rwxrw-rw-   0 ahmedgad  (1000) ahmedgad  (1000)     2317 2020-09-20 20:33:38.000000 pygad-2.9.0/pygad/kerasga/kerasga.py
-drwxr-xr-x   0 ahmedgad  (1000) ahmedgad  (1000)        0 2020-12-05 23:26:03.000000 pygad-2.9.0/pygad/nn/
--rwxrw-rw-   0 ahmedgad  (1000) ahmedgad  (1000)       42 2020-09-14 16:45:25.000000 pygad-2.9.0/pygad/nn/__init__.py
--rw-------   0 ahmedgad  (1000) ahmedgad  (1000)    19363 2020-09-14 16:36:38.000000 pygad-2.9.0/pygad/nn/nn.py
--rw-------   0 ahmedgad  (1000) ahmedgad  (1000)    81846 2020-12-05 23:25:08.000000 pygad-2.9.0/pygad/pygad.py
-drwxr-xr-x   0 ahmedgad  (1000) ahmedgad  (1000)        0 2020-12-05 23:26:03.000000 pygad-2.9.0/pygad.egg-info/
--rw-r--r--   0 ahmedgad  (1000) ahmedgad  (1000)    21733 2020-12-05 23:26:03.000000 pygad-2.9.0/pygad.egg-info/PKG-INFO
--rw-r--r--   0 ahmedgad  (1000) ahmedgad  (1000)      408 2020-12-05 23:26:03.000000 pygad-2.9.0/pygad.egg-info/SOURCES.txt
--rw-r--r--   0 ahmedgad  (1000) ahmedgad  (1000)        1 2020-12-05 23:26:03.000000 pygad-2.9.0/pygad.egg-info/dependency_links.txt
--rw-r--r--   0 ahmedgad  (1000) ahmedgad  (1000)       17 2020-12-05 23:26:03.000000 pygad-2.9.0/pygad.egg-info/requires.txt
--rw-r--r--   0 ahmedgad  (1000) ahmedgad  (1000)        6 2020-12-05 23:26:03.000000 pygad-2.9.0/pygad.egg-info/top_level.txt
--rw-r--r--   0 ahmedgad  (1000) ahmedgad  (1000)       38 2020-12-05 23:26:03.000000 pygad-2.9.0/setup.cfg
--rw-------   0 ahmedgad  (1000) ahmedgad  (1000)      563 2020-12-05 23:24:21.000000 pygad-2.9.0/setup.py
+drwxrwxr-x   0 ahmedgad  (1000) ahmedgad  (1000)        0 2023-04-08 18:31:16.373571 pygad-3.0.0/
+-rw-rw-r--   0 ahmedgad  (1000) ahmedgad  (1000)    18208 2023-04-08 18:31:16.373571 pygad-3.0.0/PKG-INFO
+-rwxrwx---   0 ahmedgad  (1000) ahmedgad  (1000)    17829 2023-04-08 18:12:48.000000 pygad-3.0.0/README.md
+drwxrwxr-x   0 ahmedgad  (1000) ahmedgad  (1000)        0 2023-04-08 18:31:16.373571 pygad-3.0.0/pygad/
+-rwxrwx---   0 ahmedgad  (1000) ahmedgad  (1000)       63 2023-04-03 22:14:20.000000 pygad-3.0.0/pygad/__init__.py
+drwxrwxr-x   0 ahmedgad  (1000) ahmedgad  (1000)        0 2023-04-08 18:31:16.373571 pygad-3.0.0/pygad/cnn/
+-rwxrwx---   0 ahmedgad  (1000) ahmedgad  (1000)       43 2023-02-23 13:33:40.000000 pygad-3.0.0/pygad/cnn/__init__.py
+-rwxrwx---   0 ahmedgad  (1000) ahmedgad  (1000)    37968 2023-02-23 13:33:40.000000 pygad-3.0.0/pygad/cnn/cnn.py
+drwxrwxr-x   0 ahmedgad  (1000) ahmedgad  (1000)        0 2023-04-08 18:31:16.373571 pygad-3.0.0/pygad/gacnn/
+-rwxrwx---   0 ahmedgad  (1000) ahmedgad  (1000)       45 2023-02-23 13:33:40.000000 pygad-3.0.0/pygad/gacnn/__init__.py
+-rwxrwx---   0 ahmedgad  (1000) ahmedgad  (1000)     5166 2023-02-23 13:33:40.000000 pygad-3.0.0/pygad/gacnn/gacnn.py
+drwxrwxr-x   0 ahmedgad  (1000) ahmedgad  (1000)        0 2023-04-08 18:31:16.373571 pygad-3.0.0/pygad/gann/
+-rwxrwx---   0 ahmedgad  (1000) ahmedgad  (1000)       44 2023-02-23 13:33:40.000000 pygad-3.0.0/pygad/gann/__init__.py
+-rwxrwx---   0 ahmedgad  (1000) ahmedgad  (1000)    21058 2023-02-23 13:33:40.000000 pygad-3.0.0/pygad/gann/gann.py
+drwxrwxr-x   0 ahmedgad  (1000) ahmedgad  (1000)        0 2023-04-08 18:31:16.373571 pygad-3.0.0/pygad/helper/
+-rwxrwx---   0 ahmedgad  (1000) ahmedgad  (1000)       54 2023-04-03 22:17:26.000000 pygad-3.0.0/pygad/helper/__init__.py
+-rwxrwx---   0 ahmedgad  (1000) ahmedgad  (1000)    47690 2023-02-28 16:43:38.000000 pygad-3.0.0/pygad/helper/unique.py
+drwxrwxr-x   0 ahmedgad  (1000) ahmedgad  (1000)        0 2023-04-08 18:31:16.373571 pygad-3.0.0/pygad/kerasga/
+-rwxrwx---   0 ahmedgad  (1000) ahmedgad  (1000)       46 2023-04-03 22:17:19.000000 pygad-3.0.0/pygad/kerasga/__init__.py
+-rwxrwx---   0 ahmedgad  (1000) ahmedgad  (1000)     3243 2023-03-01 16:53:25.000000 pygad-3.0.0/pygad/kerasga/kerasga.py
+drwxrwxr-x   0 ahmedgad  (1000) ahmedgad  (1000)        0 2023-04-08 18:31:16.373571 pygad-3.0.0/pygad/nn/
+-rwxrwx---   0 ahmedgad  (1000) ahmedgad  (1000)       42 2023-02-23 13:33:40.000000 pygad-3.0.0/pygad/nn/__init__.py
+-rwxrwx---   0 ahmedgad  (1000) ahmedgad  (1000)    19363 2023-02-23 13:33:40.000000 pygad-3.0.0/pygad/nn/nn.py
+-rwxrwx---   0 ahmedgad  (1000) ahmedgad  (1000)   217101 2023-04-03 22:10:55.000000 pygad-3.0.0/pygad/pygad.py
+drwxrwxr-x   0 ahmedgad  (1000) ahmedgad  (1000)        0 2023-04-08 18:31:16.373571 pygad-3.0.0/pygad/torchga/
+-rwxrwx---   0 ahmedgad  (1000) ahmedgad  (1000)       46 2023-04-03 22:17:09.000000 pygad-3.0.0/pygad/torchga/__init__.py
+-rwxrwx---   0 ahmedgad  (1000) ahmedgad  (1000)     3362 2023-03-01 17:53:14.000000 pygad-3.0.0/pygad/torchga/torchga.py
+drwxrwxr-x   0 ahmedgad  (1000) ahmedgad  (1000)        0 2023-04-08 18:31:16.373571 pygad-3.0.0/pygad/utils/
+-rwxrwx---   0 ahmedgad  (1000) ahmedgad  (1000)      130 2023-04-03 22:16:41.000000 pygad-3.0.0/pygad/utils/__init__.py
+-rwxrwx---   0 ahmedgad  (1000) ahmedgad  (1000)    13968 2023-03-02 02:30:43.000000 pygad-3.0.0/pygad/utils/crossover.py
+-rwxrwx---   0 ahmedgad  (1000) ahmedgad  (1000)    53487 2023-03-02 02:41:53.000000 pygad-3.0.0/pygad/utils/mutation.py
+-rwxrwx---   0 ahmedgad  (1000) ahmedgad  (1000)    10106 2023-04-03 22:10:06.000000 pygad-3.0.0/pygad/utils/parent_selection.py
+drwxrwxr-x   0 ahmedgad  (1000) ahmedgad  (1000)        0 2023-04-08 18:31:16.373571 pygad-3.0.0/pygad/visualize/
+-rwxrwx---   0 ahmedgad  (1000) ahmedgad  (1000)       55 2023-04-03 22:16:52.000000 pygad-3.0.0/pygad/visualize/__init__.py
+-rwxrwx---   0 ahmedgad  (1000) ahmedgad  (1000)    18572 2023-02-28 16:43:27.000000 pygad-3.0.0/pygad/visualize/plot.py
+drwxrwxr-x   0 ahmedgad  (1000) ahmedgad  (1000)        0 2023-04-08 18:31:16.373571 pygad-3.0.0/pygad.egg-info/
+-rw-rw-r--   0 ahmedgad  (1000) ahmedgad  (1000)    18208 2023-04-08 18:31:16.000000 pygad-3.0.0/pygad.egg-info/PKG-INFO
+-rw-rw-r--   0 ahmedgad  (1000) ahmedgad  (1000)      664 2023-04-08 18:31:16.000000 pygad-3.0.0/pygad.egg-info/SOURCES.txt
+-rw-rw-r--   0 ahmedgad  (1000) ahmedgad  (1000)        1 2023-04-08 18:31:16.000000 pygad-3.0.0/pygad.egg-info/dependency_links.txt
+-rw-rw-r--   0 ahmedgad  (1000) ahmedgad  (1000)       29 2023-04-08 18:31:16.000000 pygad-3.0.0/pygad.egg-info/requires.txt
+-rw-rw-r--   0 ahmedgad  (1000) ahmedgad  (1000)        6 2023-04-08 18:31:16.000000 pygad-3.0.0/pygad.egg-info/top_level.txt
+-rw-rw-r--   0 ahmedgad  (1000) ahmedgad  (1000)       38 2023-04-08 18:31:16.373571 pygad-3.0.0/setup.cfg
+-rwxrwx---   0 ahmedgad  (1000) ahmedgad  (1000)      637 2023-04-08 18:19:58.000000 pygad-3.0.0/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `pygad-2.9.0/PKG-INFO` & `pygad-3.0.0/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,354 +1,346 @@
 Metadata-Version: 2.1
 Name: pygad
-Version: 2.9.0
-Summary: PyGAD: A Python Library for Building the Genetic Algorithm.
+Version: 3.0.0
+Summary: PyGAD: A Python 3 Library for Building the Genetic Algorithm and Training Machine Learning Algoithms (Keras & PyTorch).
 Home-page: https://github.com/ahmedfgad/GeneticAlgorithmPython
 Author: Ahmed Fawzy Gad
 Author-email: ahmed.f.gad@gmail.com
 License: UNKNOWN
-Description: # GeneticAlgorithmPython: Building Genetic Algorithm in Python
-        
-        [This project](https://github.com/ahmedfgad/GeneticAlgorithmPython) is part of [PyGAD](https://pypi.org/project/pygad) which is an open-source Python 3 library for building the genetic algorithm and optimizing machine learning algorithms. 
-        
-        Check documentation of the [GeneticAlgorithmPython](https://github.com/ahmedfgad/GeneticAlgorithmPython) project in the PyGAD's documentation: https://pygad.readthedocs.io/en/latest/README_pygad_ReadTheDocs.html
-        
-        [PyGAD](https://pypi.org/project/pygad) supports different types of crossover, mutation, and parent selection. [PyGAD](https://pypi.org/project/pygad) allows different types of problems to be optimized using the genetic algorithm by customizing the fitness function. 
-        
-        The library is under active development and more features are added regularly. If you want a feature to be supported, please check the **Contact Us** section to send a request.
-        
-        # Donation
-        
-        You can donate via [Open Collective](https://opencollective.com/pygad): [opencollective.com/pygad](https://opencollective.com/pygad). 
-        
-        To donate using PayPal, use either this link: [paypal.me/ahmedfgad](https://paypal.me/ahmedfgad) or the e-mail address ahmed.f.gad@gmail.com.
-        
-        # Tutorial Project
-        
-        **IMPORTANT** If you are coming for the code of the tutorial titled  [**Genetic Algorithm Implementation in Python**](https://www.linkedin.com/pulse/genetic-algorithm-implementation-python-ahmed-gad), then it has been moved to the [Tutorial Project](https://github.com/ahmedfgad/GeneticAlgorithmPython/tree/master/Tutorial Project) directory on 06 May 2020.
-        
-        # Installation
-        
-        To install [PyGAD](https://pypi.org/project/pygad), simply use pip to download and install the library from [PyPI](https://pypi.org/project/pygad) (Python Package Index). The library lives a PyPI at this page https://pypi.org/project/pygad.
-        
-        For Windows, issue the following command:
-        
-        ```python
-        pip install pygad
-        ```
-        
-        For Linux and Mac, replace `pip` by use `pip3` because the library only supports Python 3.
-        
-        ```python
-        pip3 install pygad
-        ```
-        
-        PyGAD is developed in Python 3.7.3 and depends on NumPy for creating and manipulating arrays and Matplotlib for creating figures. The exact NumPy version used in developing PyGAD is 1.16.4. For Matplotlib, the version is 3.1.0.
-        
-        To get started with PyGAD, please read the documentation at [Read The Docs](https://pygad.readthedocs.io/) https://pygad.readthedocs.io.
-        
-        # PyGAD Source Code
-        
-        The source code of the PyGAD' modules is found in the following GitHub projects:
-        
-        - [pygad](https://github.com/ahmedfgad/GeneticAlgorithmPython): (https://github.com/ahmedfgad/GeneticAlgorithmPython)
-        - [pygad.nn](https://github.com/ahmedfgad/NumPyANN): https://github.com/ahmedfgad/NumPyANN
-        - [pygad.gann](https://github.com/ahmedfgad/NeuralGenetic): https://github.com/ahmedfgad/NeuralGenetic
-        - [pygad.cnn](https://github.com/ahmedfgad/NumPyCNN): https://github.com/ahmedfgad/NumPyCNN
-        - [pygad.gacnn](https://github.com/ahmedfgad/CNNGenetic): https://github.com/ahmedfgad/CNNGenetic
-        
-        The documentation of PyGAD is available at [Read The Docs](https://pygad.readthedocs.io/) https://pygad.readthedocs.io.
-        
-        # PyGAD Documentation
-        
-        The documentation of the PyGAD library is available at [Read The Docs](https://pygad.readthedocs.io) at this link: https://pygad.readthedocs.io. It discusses the modules supported by PyGAD, all its classes, methods, attribute, and functions. For each module, a number of examples are given.
-        
-        If there is an issue using PyGAD, feel free to post at issue in this [GitHub repository](https://github.com/ahmedfgad/GeneticAlgorithmPython) https://github.com/ahmedfgad/GeneticAlgorithmPython or by sending an e-mail to ahmed.f.gad@gmail.com. 
-        
-        If you built a project that uses PyGAD, then please drop an e-mail to ahmed.f.gad@gmail.com with the following information so that your project is included in the documentation.
-        
-        - Project title
-        - Brief description
-        - Preferably, a link that directs the readers to your project
-        
-        Please check the **Contact Us** section for more contact details.
-        
-        # Life Cycle of PyGAD
-        
-        The next figure lists the different stages in the lifecycle of an instance of the `pygad.GA` class. Note that PyGAD stops when either all generations are completed or when the function passed to the `on_generation` parameter returns the string `stop`.
-        
-        ![PyGAD Lifecycle](https://user-images.githubusercontent.com/16560492/89446279-9c6f8380-d754-11ea-83fd-a60ea2f53b85.jpg)
-        
-        The next code implements all the callback functions to trace the execution of the genetic algorithm. Each callback function prints its name.
-        
-        ```python
-        import pygad
-        import numpy
-        
-        function_inputs = [4,-2,3.5,5,-11,-4.7]
-        desired_output = 44
-        
-        def fitness_func(solution, solution_idx):
-            output = numpy.sum(solution*function_inputs)
-            fitness = 1.0 / (numpy.abs(output - desired_output) + 0.000001)
-            return fitness
-        
-        fitness_function = fitness_func
-        
-        def on_start(ga_instance):
-            print("on_start()")
-        
-        def on_fitness(ga_instance, population_fitness):
-            print("on_fitness()")
-        
-        def on_parents(ga_instance, selected_parents):
-            print("on_parents()")
-        
-        def on_crossover(ga_instance, offspring_crossover):
-            print("on_crossover()")
-        
-        def on_mutation(ga_instance, offspring_mutation):
-            print("on_mutation()")
-        
-        def on_generation(ga_instance):
-            print("on_generation()")
-        
-        def on_stop(ga_instance, last_population_fitness):
-            print("on_stop()")
-        
-        ga_instance = pygad.GA(num_generations=3,
-                               num_parents_mating=5,
-                               fitness_func=fitness_function,
-                               sol_per_pop=10,
-                               num_genes=len(function_inputs),
-                               on_start=on_start,
-                               on_fitness=on_fitness,
-                               on_parents=on_parents,
-                               on_crossover=on_crossover,
-                               on_mutation=on_mutation,
-                               on_generation=on_generation,
-                               on_stop=on_stop)
-        
-        ga_instance.run()
-        ```
-        
-        Based on the used 3 generations as assigned to the `num_generations` argument, here is the output.
-        
-        ```
-        on_start()
-        
-        on_fitness()
-        on_parents()
-        on_crossover()
-        on_mutation()
-        on_generation()
-        
-        on_fitness()
-        on_parents()
-        on_crossover()
-        on_mutation()
-        on_generation()
-        
-        on_fitness()
-        on_parents()
-        on_crossover()
-        on_mutation()
-        on_generation()
-        
-        on_stop()
-        ```
-        
-        # Example
-        
-        Check the [PyGAD's documentation](https://pygad.readthedocs.io/en/latest/README_pygad_ReadTheDocs.html) for information about the implementation of this example.
-        
-        ```python
-        import pygad
-        import numpy
-        
-        """
-        Given the following function:
-            y = f(w1:w6) = w1x1 + w2x2 + w3x3 + w4x4 + w5x5 + 6wx6
-            where (x1,x2,x3,x4,x5,x6)=(4,-2,3.5,5,-11,-4.7) and y=44
-        What are the best values for the 6 weights (w1 to w6)? We are going to use the genetic algorithm to optimize this function.
-        """
-        
-        function_inputs = [4,-2,3.5,5,-11,-4.7] # Function inputs.
-        desired_output = 44 # Function output.
-        
-        def fitness_func(solution, solution_idx):
-            # Calculating the fitness value of each solution in the current population.
-            # The fitness function calulates the sum of products between each input and its corresponding weight.
-            output = numpy.sum(solution*function_inputs)
-            fitness = 1.0 / numpy.abs(output - desired_output)
-            return fitness
-        
-        fitness_function = fitness_func
-        
-        num_generations = 100 # Number of generations.
-        num_parents_mating = 7 # Number of solutions to be selected as parents in the mating pool.
-        
-        # To prepare the initial population, there are 2 ways:
-        # 1) Prepare it yourself and pass it to the initial_population parameter. This way is useful when the user wants to start the genetic algorithm with a custom initial population.
-        # 2) Assign valid integer values to the sol_per_pop and num_genes parameters. If the initial_population parameter exists, then the sol_per_pop and num_genes parameters are useless.
-        sol_per_pop = 50 # Number of solutions in the population.
-        num_genes = len(function_inputs)
-        
-        init_range_low = -2
-        init_range_high = 5
-        
-        parent_selection_type = "sss" # Type of parent selection.
-        keep_parents = 7 # Number of parents to keep in the next population. -1 means keep all parents and 0 means keep nothing.
-        
-        crossover_type = "single_point" # Type of the crossover operator.
-        
-        # Parameters of the mutation operation.
-        mutation_type = "random" # Type of the mutation operator.
-        mutation_percent_genes = 10 # Percentage of genes to mutate. This parameter has no action if the parameter mutation_num_genes exists or when mutation_type is None.
-        
-        last_fitness = 0
-        def callback_generation(ga_instance):
-            global last_fitness
-            print("Generation = {generation}".format(generation=ga_instance.generations_completed))
-            print("Fitness    = {fitness}".format(fitness=ga_instance.best_solution()[1]))
-            print("Change     = {change}".format(change=ga_instance.best_solution()[1] - last_fitness))
-            last_fitness = ga_instance.best_solution()[1]
-        
-        # Creating an instance of the GA class inside the ga module. Some parameters are initialized within the constructor.
-        ga_instance = pygad.GA(num_generations=num_generations,
-                               num_parents_mating=num_parents_mating, 
-                               fitness_func=fitness_function,
-                               sol_per_pop=sol_per_pop, 
-                               num_genes=num_genes,
-                               init_range_low=init_range_low,
-                               init_range_high=init_range_high,
-                               parent_selection_type=parent_selection_type,
-                               keep_parents=keep_parents,
-                               crossover_type=crossover_type,
-                               mutation_type=mutation_type,
-                               mutation_percent_genes=mutation_percent_genes,
-                               callback_generation=callback_generation)
-        
-        # Running the GA to optimize the parameters of the function.
-        ga_instance.run()
-        
-        # After the generations complete, some plots are showed that summarize the how the outputs/fitenss values evolve over generations.
-        ga_instance.plot_result()
-        
-        # Returning the details of the best solution.
-        solution, solution_fitness, solution_idx = ga_instance.best_solution()
-        print("Parameters of the best solution : {solution}".format(solution=solution))
-        print("Fitness value of the best solution = {solution_fitness}".format(solution_fitness=solution_fitness))
-        print("Index of the best solution : {solution_idx}".format(solution_idx=solution_idx))
-        
-        prediction = numpy.sum(numpy.array(function_inputs)*solution)
-        print("Predicted output based on the best solution : {prediction}".format(prediction=prediction))
-        
-        if ga_instance.best_solution_generation != -1:
-            print("Best fitness value reached after {best_solution_generation} generations.".format(best_solution_generation=ga_instance.best_solution_generation))
-        
-        # Saving the GA instance.
-        filename = 'genetic' # The filename to which the instance is saved. The name is without extension.
-        ga_instance.save(filename=filename)
-        
-        # Loading the saved GA instance.
-        loaded_ga_instance = pygad.load(filename=filename)
-        loaded_ga_instance.plot_result()
-        ```
-        
-        # For More Information
-        
-        There are different resources that can be used to get started with the genetic algorithm and building it in Python. 
-        
-        ## Tutorial: Implementing Genetic Algorithm in Python
-        
-        To start with coding the genetic algorithm, you can check the tutorial titled [**Genetic Algorithm Implementation in Python**](https://www.linkedin.com/pulse/genetic-algorithm-implementation-python-ahmed-gad) available at these links:
-        
-        - [LinkedIn](https://www.linkedin.com/pulse/genetic-algorithm-implementation-python-ahmed-gad)
-        - [Towards Data Science](https://towardsdatascience.com/genetic-algorithm-implementation-in-python-5ab67bb124a6)
-        - [KDnuggets](https://www.kdnuggets.com/2018/07/genetic-algorithm-implementation-python.html)
-        
-        [This tutorial](https://www.linkedin.com/pulse/genetic-algorithm-implementation-python-ahmed-gad) is prepared based on a previous version of the project but it still a good resource to start with coding the genetic algorithm.
-        
-        [![Genetic Algorithm Implementation in Python](https://user-images.githubusercontent.com/16560492/78830052-a3c19300-79e7-11ea-8b9b-4b343ea4049c.png)](https://www.linkedin.com/pulse/genetic-algorithm-implementation-python-ahmed-gad)
-        
-        ## Tutorial: Introduction to Genetic Algorithm
-        
-        Get started with the genetic algorithm by reading the tutorial titled [**Introduction to Optimization with Genetic Algorithm**](https://www.linkedin.com/pulse/introduction-optimization-genetic-algorithm-ahmed-gad) which is available at these links:
-        
-        * [LinkedIn](https://www.linkedin.com/pulse/introduction-optimization-genetic-algorithm-ahmed-gad)
-        * [Towards Data Science](https://www.kdnuggets.com/2018/03/introduction-optimization-with-genetic-algorithm.html)
-        * [KDnuggets](https://towardsdatascience.com/introduction-to-optimization-with-genetic-algorithm-2f5001d9964b)
-        
-        [![Introduction to Genetic Algorithm](https://user-images.githubusercontent.com/16560492/82078259-26252d00-96e1-11ea-9a02-52a99e1054b9.jpg)](https://www.linkedin.com/pulse/introduction-optimization-genetic-algorithm-ahmed-gad)
-        
-        ## Tutorial: Build Neural Networks in Python
-        
-        Read about building neural networks in Python through the tutorial titled [**Artificial Neural Network Implementation using NumPy and Classification of the Fruits360 Image Dataset**](https://www.linkedin.com/pulse/artificial-neural-network-implementation-using-numpy-fruits360-gad) available at these links:
-        
-        * [LinkedIn](https://www.linkedin.com/pulse/artificial-neural-network-implementation-using-numpy-fruits360-gad)
-        * [Towards Data Science](https://towardsdatascience.com/artificial-neural-network-implementation-using-numpy-and-classification-of-the-fruits360-image-3c56affa4491)
-        * [KDnuggets](https://www.kdnuggets.com/2019/02/artificial-neural-network-implementation-using-numpy-and-image-classification.html)
-        
-        [![Building Neural Networks Python](https://user-images.githubusercontent.com/16560492/82078281-30472b80-96e1-11ea-8017-6a1f4383d602.jpg)](https://www.linkedin.com/pulse/artificial-neural-network-implementation-using-numpy-fruits360-gad)
-        
-        ## Tutorial: Optimize Neural Networks with Genetic Algorithm
-        
-        Read about training neural networks using the genetic algorithm through the tutorial titled [**Artificial Neural Networks Optimization using Genetic Algorithm with Python**](https://www.linkedin.com/pulse/artificial-neural-networks-optimization-using-genetic-ahmed-gad) available at these links:
-        
-        - [LinkedIn](https://www.linkedin.com/pulse/artificial-neural-networks-optimization-using-genetic-ahmed-gad)
-        - [Towards Data Science](https://towardsdatascience.com/artificial-neural-networks-optimization-using-genetic-algorithm-with-python-1fe8ed17733e)
-        - [KDnuggets](https://www.kdnuggets.com/2019/03/artificial-neural-networks-optimization-genetic-algorithm-python.html)
-        
-        [![Training Neural Networks using Genetic Algorithm Python](https://user-images.githubusercontent.com/16560492/82078300-376e3980-96e1-11ea-821c-aa6b8ceb44d4.jpg)](https://www.linkedin.com/pulse/artificial-neural-networks-optimization-using-genetic-ahmed-gad)
-        
-        ## Tutorial: Building CNN in Python
-        
-        To start with coding the genetic algorithm, you can check the tutorial titled [**Building Convolutional Neural Network using NumPy from Scratch**](https://www.linkedin.com/pulse/building-convolutional-neural-network-using-numpy-from-ahmed-gad) available at these links:
-        
-        - [LinkedIn](https://www.linkedin.com/pulse/building-convolutional-neural-network-using-numpy-from-ahmed-gad)
-        - [Towards Data Science](https://towardsdatascience.com/building-convolutional-neural-network-using-numpy-from-scratch-b30aac50e50a)
-        - [KDnuggets](https://www.kdnuggets.com/2018/04/building-convolutional-neural-network-numpy-scratch.html)
-        - [Chinese Translation](http://m.aliyun.com/yunqi/articles/585741)
-        
-        [This tutorial](https://www.linkedin.com/pulse/building-convolutional-neural-network-using-numpy-from-ahmed-gad)) is prepared based on a previous version of the project but it still a good resource to start with coding CNNs.
-        
-        [![Building CNN in Python](https://user-images.githubusercontent.com/16560492/82431022-6c3a1200-9a8e-11ea-8f1b-b055196d76e3.png)](https://www.linkedin.com/pulse/building-convolutional-neural-network-using-numpy-from-ahmed-gad)
-        
-        ## Tutorial: Derivation of CNN from FCNN
-        
-        Get started with the genetic algorithm by reading the tutorial titled [**Derivation of Convolutional Neural Network from Fully Connected Network Step-By-Step**](https://www.linkedin.com/pulse/derivation-convolutional-neural-network-from-fully-connected-gad) which is available at these links:
-        
-        * [LinkedIn](https://www.linkedin.com/pulse/derivation-convolutional-neural-network-from-fully-connected-gad)
-        * [Towards Data Science](https://towardsdatascience.com/derivation-of-convolutional-neural-network-from-fully-connected-network-step-by-step-b42ebafa5275)
-        * [KDnuggets](https://www.kdnuggets.com/2018/04/derivation-convolutional-neural-network-fully-connected-step-by-step.html)
-        
-        [![Derivation of CNN from FCNN](https://user-images.githubusercontent.com/16560492/82431369-db176b00-9a8e-11ea-99bd-e845192873fc.png)](https://www.linkedin.com/pulse/derivation-convolutional-neural-network-from-fully-connected-gad)
-        
-        ## Book: Practical Computer Vision Applications Using Deep Learning with CNNs
-        
-        You can also check my book cited as [**Ahmed Fawzy Gad 'Practical Computer Vision Applications Using Deep Learning with CNNs'. Dec. 2018, Apress, 978-1-4842-4167-7**](https://www.amazon.com/Practical-Computer-Vision-Applications-Learning/dp/1484241665) which discusses neural networks, convolutional neural networks, deep learning, genetic algorithm, and more.
-        
-        Find the book at these links:
-        
-        - [Amazon](https://www.amazon.com/Practical-Computer-Vision-Applications-Learning/dp/1484241665)
-        - [Springer](https://link.springer.com/book/10.1007/978-1-4842-4167-7)
-        - [Apress](https://www.apress.com/gp/book/9781484241660)
-        - [O'Reilly](https://www.oreilly.com/library/view/practical-computer-vision/9781484241677)
-        - [Google Books](https://books.google.com.eg/books?id=xLd9DwAAQBAJ)
-        
-        ![Fig04](https://user-images.githubusercontent.com/16560492/78830077-ae7c2800-79e7-11ea-980b-53b6bd879eeb.jpg)
-        
-        # Contact Us
-        
-        * E-mail: ahmed.f.gad@gmail.com
-        * [LinkedIn](https://www.linkedin.com/in/ahmedfgad)
-        * [Amazon Author Page](https://amazon.com/author/ahmedgad)
-        * [Heartbeat](https://heartbeat.fritz.ai/@ahmedfgad)
-        * [Paperspace](https://blog.paperspace.com/author/ahmed)
-        * [KDnuggets](https://kdnuggets.com/author/ahmed-gad)
-        * [TowardsDataScience](https://towardsdatascience.com/@ahmedfgad)
-        * [GitHub](https://github.com/ahmedfgad)
-        
-        
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
+
+# PyGAD:  Genetic Algorithm in Python
+
+[PyGAD](https://pypi.org/project/pygad) is an open-source easy-to-use Python 3 library for building the genetic algorithm and optimizing machine learning algorithms. It supports Keras and PyTorch.
+
+Check documentation of the [PyGAD](https://pygad.readthedocs.io/en/latest).
+
+[![Downloads](https://pepy.tech/badge/pygad)](https://pepy.tech/project/pygad) ![Docs](https://readthedocs.org/projects/pygad/badge)
+
+![PYGAD-LOGO](https://user-images.githubusercontent.com/16560492/101267295-c74c0180-375f-11eb-9ad0-f8e37bd796ce.png)
+
+[PyGAD](https://pypi.org/project/pygad) supports different types of crossover, mutation, and parent selection. [PyGAD](https://pypi.org/project/pygad) allows different types of problems to be optimized using the genetic algorithm by customizing the fitness function. 
+
+The library is under active development and more features are added regularly. If you want a feature to be supported, please check the **Contact Us** section to send a request.
+
+# Donation
+
+- [Credit/Debit Card](https://donate.stripe.com/eVa5kO866elKgM0144): https://donate.stripe.com/eVa5kO866elKgM0144
+- [Open Collective](https://opencollective.com/pygad): [opencollective.com/pygad](https://opencollective.com/pygad)
+- PayPal: Use either this link: [paypal.me/ahmedfgad](https://paypal.me/ahmedfgad) or the e-mail address ahmed.f.gad@gmail.com
+- Interac e-Transfer: Use e-mail address ahmed.f.gad@gmail.com
+
+# Installation
+
+To install [PyGAD](https://pypi.org/project/pygad), simply use pip to download and install the library from [PyPI](https://pypi.org/project/pygad) (Python Package Index). The library lives a PyPI at this page https://pypi.org/project/pygad.
+
+Install PyGAD with the following command:
+
+```python
+pip install pygad
+```
+
+PyGAD is developed in Python 3.7.3 and depends on NumPy for creating and manipulating arrays and Matplotlib for creating figures. The exact NumPy version used in developing PyGAD is 1.16.4. For Matplotlib, the version is 3.1.0.
+
+To get started with PyGAD, please read the documentation at [Read The Docs](https://pygad.readthedocs.io/) https://pygad.readthedocs.io.
+
+# PyGAD Source Code
+
+The source code of the PyGAD' modules is found in the following GitHub projects:
+
+- [pygad](https://github.com/ahmedfgad/GeneticAlgorithmPython): (https://github.com/ahmedfgad/GeneticAlgorithmPython)
+- [pygad.nn](https://github.com/ahmedfgad/NumPyANN): https://github.com/ahmedfgad/NumPyANN
+- [pygad.gann](https://github.com/ahmedfgad/NeuralGenetic): https://github.com/ahmedfgad/NeuralGenetic
+- [pygad.cnn](https://github.com/ahmedfgad/NumPyCNN): https://github.com/ahmedfgad/NumPyCNN
+- [pygad.gacnn](https://github.com/ahmedfgad/CNNGenetic): https://github.com/ahmedfgad/CNNGenetic
+- [pygad.kerasga](https://github.com/ahmedfgad/KerasGA): https://github.com/ahmedfgad/KerasGA
+- [pygad.torchga](https://github.com/ahmedfgad/TorchGA): https://github.com/ahmedfgad/TorchGA
+
+The documentation of PyGAD is available at [Read The Docs](https://pygad.readthedocs.io/) https://pygad.readthedocs.io.
+
+# PyGAD Documentation
+
+The documentation of the PyGAD library is available at [Read The Docs](https://pygad.readthedocs.io) at this link: https://pygad.readthedocs.io. It discusses the modules supported by PyGAD, all its classes, methods, attribute, and functions. For each module, a number of examples are given.
+
+If there is an issue using PyGAD, feel free to post at issue in this [GitHub repository](https://github.com/ahmedfgad/GeneticAlgorithmPython) https://github.com/ahmedfgad/GeneticAlgorithmPython or by sending an e-mail to ahmed.f.gad@gmail.com. 
+
+If you built a project that uses PyGAD, then please drop an e-mail to ahmed.f.gad@gmail.com with the following information so that your project is included in the documentation.
+
+- Project title
+- Brief description
+- Preferably, a link that directs the readers to your project
+
+Please check the **Contact Us** section for more contact details.
+
+# Life Cycle of PyGAD
+
+The next figure lists the different stages in the lifecycle of an instance of the `pygad.GA` class. Note that PyGAD stops when either all generations are completed or when the function passed to the `on_generation` parameter returns the string `stop`.
+
+![PyGAD Lifecycle](https://user-images.githubusercontent.com/16560492/220486073-c5b6089d-81e4-44d9-a53c-385f479a7273.jpg)
+
+The next code implements all the callback functions to trace the execution of the genetic algorithm. Each callback function prints its name.
+
+```python
+import pygad
+import numpy
+
+function_inputs = [4,-2,3.5,5,-11,-4.7]
+desired_output = 44
+
+def fitness_func(solution, solution_idx):
+    output = numpy.sum(solution*function_inputs)
+    fitness = 1.0 / (numpy.abs(output - desired_output) + 0.000001)
+    return fitness
+
+fitness_function = fitness_func
+
+def on_start(ga_instance):
+    print("on_start()")
+
+def on_fitness(ga_instance, population_fitness):
+    print("on_fitness()")
+
+def on_parents(ga_instance, selected_parents):
+    print("on_parents()")
+
+def on_crossover(ga_instance, offspring_crossover):
+    print("on_crossover()")
+
+def on_mutation(ga_instance, offspring_mutation):
+    print("on_mutation()")
+
+def on_generation(ga_instance):
+    print("on_generation()")
+
+def on_stop(ga_instance, last_population_fitness):
+    print("on_stop()")
+
+ga_instance = pygad.GA(num_generations=3,
+                       num_parents_mating=5,
+                       fitness_func=fitness_function,
+                       sol_per_pop=10,
+                       num_genes=len(function_inputs),
+                       on_start=on_start,
+                       on_fitness=on_fitness,
+                       on_parents=on_parents,
+                       on_crossover=on_crossover,
+                       on_mutation=on_mutation,
+                       on_generation=on_generation,
+                       on_stop=on_stop)
+
+ga_instance.run()
+```
+
+Based on the used 3 generations as assigned to the `num_generations` argument, here is the output.
+
+```
+on_start()
+
+on_fitness()
+on_parents()
+on_crossover()
+on_mutation()
+on_generation()
+
+on_fitness()
+on_parents()
+on_crossover()
+on_mutation()
+on_generation()
+
+on_fitness()
+on_parents()
+on_crossover()
+on_mutation()
+on_generation()
+
+on_stop()
+```
+
+# Example
+
+Check the [PyGAD's documentation](https://pygad.readthedocs.io/en/latest/README_pygad_ReadTheDocs.html) for information about the implementation of this example.
+
+```python
+import pygad
+import numpy
+
+"""
+Given the following function:
+    y = f(w1:w6) = w1x1 + w2x2 + w3x3 + w4x4 + w5x5 + 6wx6
+    where (x1,x2,x3,x4,x5,x6)=(4,-2,3.5,5,-11,-4.7) and y=44
+What are the best values for the 6 weights (w1 to w6)? We are going to use the genetic algorithm to optimize this function.
+"""
+
+function_inputs = [4,-2,3.5,5,-11,-4.7] # Function inputs.
+desired_output = 44 # Function output.
+
+def fitness_func(solution, solution_idx):
+    # Calculating the fitness value of each solution in the current population.
+    # The fitness function calulates the sum of products between each input and its corresponding weight.
+    output = numpy.sum(solution*function_inputs)
+    fitness = 1.0 / numpy.abs(output - desired_output)
+    return fitness
+
+fitness_function = fitness_func
+
+num_generations = 100 # Number of generations.
+num_parents_mating = 7 # Number of solutions to be selected as parents in the mating pool.
+
+# To prepare the initial population, there are 2 ways:
+# 1) Prepare it yourself and pass it to the initial_population parameter. This way is useful when the user wants to start the genetic algorithm with a custom initial population.
+# 2) Assign valid integer values to the sol_per_pop and num_genes parameters. If the initial_population parameter exists, then the sol_per_pop and num_genes parameters are useless.
+sol_per_pop = 50 # Number of solutions in the population.
+num_genes = len(function_inputs)
+
+last_fitness = 0
+def callback_generation(ga_instance):
+    global last_fitness
+    print("Generation = {generation}".format(generation=ga_instance.generations_completed))
+    print("Fitness    = {fitness}".format(fitness=ga_instance.best_solution()[1]))
+    print("Change     = {change}".format(change=ga_instance.best_solution()[1] - last_fitness))
+    last_fitness = ga_instance.best_solution()[1]
+
+# Creating an instance of the GA class inside the ga module. Some parameters are initialized within the constructor.
+ga_instance = pygad.GA(num_generations=num_generations,
+                       num_parents_mating=num_parents_mating, 
+                       fitness_func=fitness_function,
+                       sol_per_pop=sol_per_pop, 
+                       num_genes=num_genes,
+                       on_generation=callback_generation)
+
+# Running the GA to optimize the parameters of the function.
+ga_instance.run()
+
+# After the generations complete, some plots are showed that summarize the how the outputs/fitenss values evolve over generations.
+ga_instance.plot_fitness()
+
+# Returning the details of the best solution.
+solution, solution_fitness, solution_idx = ga_instance.best_solution()
+print("Parameters of the best solution : {solution}".format(solution=solution))
+print("Fitness value of the best solution = {solution_fitness}".format(solution_fitness=solution_fitness))
+print("Index of the best solution : {solution_idx}".format(solution_idx=solution_idx))
+
+prediction = numpy.sum(numpy.array(function_inputs)*solution)
+print("Predicted output based on the best solution : {prediction}".format(prediction=prediction))
+
+if ga_instance.best_solution_generation != -1:
+    print("Best fitness value reached after {best_solution_generation} generations.".format(best_solution_generation=ga_instance.best_solution_generation))
+
+# Saving the GA instance.
+filename = 'genetic' # The filename to which the instance is saved. The name is without extension.
+ga_instance.save(filename=filename)
+
+# Loading the saved GA instance.
+loaded_ga_instance = pygad.load(filename=filename)
+loaded_ga_instance.plot_fitness()
+```
+
+# For More Information
+
+There are different resources that can be used to get started with the genetic algorithm and building it in Python. 
+
+## Tutorial: Implementing Genetic Algorithm in Python
+
+To start with coding the genetic algorithm, you can check the tutorial titled [**Genetic Algorithm Implementation in Python**](https://www.linkedin.com/pulse/genetic-algorithm-implementation-python-ahmed-gad) available at these links:
+
+- [LinkedIn](https://www.linkedin.com/pulse/genetic-algorithm-implementation-python-ahmed-gad)
+- [Towards Data Science](https://towardsdatascience.com/genetic-algorithm-implementation-in-python-5ab67bb124a6)
+- [KDnuggets](https://www.kdnuggets.com/2018/07/genetic-algorithm-implementation-python.html)
+
+[This tutorial](https://www.linkedin.com/pulse/genetic-algorithm-implementation-python-ahmed-gad) is prepared based on a previous version of the project but it still a good resource to start with coding the genetic algorithm.
+
+[![Genetic Algorithm Implementation in Python](https://user-images.githubusercontent.com/16560492/78830052-a3c19300-79e7-11ea-8b9b-4b343ea4049c.png)](https://www.linkedin.com/pulse/genetic-algorithm-implementation-python-ahmed-gad)
+
+## Tutorial: Introduction to Genetic Algorithm
+
+Get started with the genetic algorithm by reading the tutorial titled [**Introduction to Optimization with Genetic Algorithm**](https://www.linkedin.com/pulse/introduction-optimization-genetic-algorithm-ahmed-gad) which is available at these links:
+
+* [LinkedIn](https://www.linkedin.com/pulse/introduction-optimization-genetic-algorithm-ahmed-gad)
+* [Towards Data Science](https://towardsdatascience.com/introduction-to-optimization-with-genetic-algorithm-2f5001d9964b)
+* [KDnuggets](https://www.kdnuggets.com/2018/03/introduction-optimization-with-genetic-algorithm.html)
+
+[![Introduction to Genetic Algorithm](https://user-images.githubusercontent.com/16560492/82078259-26252d00-96e1-11ea-9a02-52a99e1054b9.jpg)](https://www.linkedin.com/pulse/introduction-optimization-genetic-algorithm-ahmed-gad)
+
+## Tutorial: Build Neural Networks in Python
+
+Read about building neural networks in Python through the tutorial titled [**Artificial Neural Network Implementation using NumPy and Classification of the Fruits360 Image Dataset**](https://www.linkedin.com/pulse/artificial-neural-network-implementation-using-numpy-fruits360-gad) available at these links:
+
+* [LinkedIn](https://www.linkedin.com/pulse/artificial-neural-network-implementation-using-numpy-fruits360-gad)
+* [Towards Data Science](https://towardsdatascience.com/artificial-neural-network-implementation-using-numpy-and-classification-of-the-fruits360-image-3c56affa4491)
+* [KDnuggets](https://www.kdnuggets.com/2019/02/artificial-neural-network-implementation-using-numpy-and-image-classification.html)
+
+[![Building Neural Networks Python](https://user-images.githubusercontent.com/16560492/82078281-30472b80-96e1-11ea-8017-6a1f4383d602.jpg)](https://www.linkedin.com/pulse/artificial-neural-network-implementation-using-numpy-fruits360-gad)
+
+## Tutorial: Optimize Neural Networks with Genetic Algorithm
+
+Read about training neural networks using the genetic algorithm through the tutorial titled [**Artificial Neural Networks Optimization using Genetic Algorithm with Python**](https://www.linkedin.com/pulse/artificial-neural-networks-optimization-using-genetic-ahmed-gad) available at these links:
+
+- [LinkedIn](https://www.linkedin.com/pulse/artificial-neural-networks-optimization-using-genetic-ahmed-gad)
+- [Towards Data Science](https://towardsdatascience.com/artificial-neural-networks-optimization-using-genetic-algorithm-with-python-1fe8ed17733e)
+- [KDnuggets](https://www.kdnuggets.com/2019/03/artificial-neural-networks-optimization-genetic-algorithm-python.html)
+
+[![Training Neural Networks using Genetic Algorithm Python](https://user-images.githubusercontent.com/16560492/82078300-376e3980-96e1-11ea-821c-aa6b8ceb44d4.jpg)](https://www.linkedin.com/pulse/artificial-neural-networks-optimization-using-genetic-ahmed-gad)
+
+## Tutorial: Building CNN in Python
+
+To start with coding the genetic algorithm, you can check the tutorial titled [**Building Convolutional Neural Network using NumPy from Scratch**](https://www.linkedin.com/pulse/building-convolutional-neural-network-using-numpy-from-ahmed-gad) available at these links:
+
+- [LinkedIn](https://www.linkedin.com/pulse/building-convolutional-neural-network-using-numpy-from-ahmed-gad)
+- [Towards Data Science](https://towardsdatascience.com/building-convolutional-neural-network-using-numpy-from-scratch-b30aac50e50a)
+- [KDnuggets](https://www.kdnuggets.com/2018/04/building-convolutional-neural-network-numpy-scratch.html)
+- [Chinese Translation](http://m.aliyun.com/yunqi/articles/585741)
+
+[This tutorial](https://www.linkedin.com/pulse/building-convolutional-neural-network-using-numpy-from-ahmed-gad)) is prepared based on a previous version of the project but it still a good resource to start with coding CNNs.
+
+[![Building CNN in Python](https://user-images.githubusercontent.com/16560492/82431022-6c3a1200-9a8e-11ea-8f1b-b055196d76e3.png)](https://www.linkedin.com/pulse/building-convolutional-neural-network-using-numpy-from-ahmed-gad)
+
+## Tutorial: Derivation of CNN from FCNN
+
+Get started with the genetic algorithm by reading the tutorial titled [**Derivation of Convolutional Neural Network from Fully Connected Network Step-By-Step**](https://www.linkedin.com/pulse/derivation-convolutional-neural-network-from-fully-connected-gad) which is available at these links:
+
+* [LinkedIn](https://www.linkedin.com/pulse/derivation-convolutional-neural-network-from-fully-connected-gad)
+* [Towards Data Science](https://towardsdatascience.com/derivation-of-convolutional-neural-network-from-fully-connected-network-step-by-step-b42ebafa5275)
+* [KDnuggets](https://www.kdnuggets.com/2018/04/derivation-convolutional-neural-network-fully-connected-step-by-step.html)
+
+[![Derivation of CNN from FCNN](https://user-images.githubusercontent.com/16560492/82431369-db176b00-9a8e-11ea-99bd-e845192873fc.png)](https://www.linkedin.com/pulse/derivation-convolutional-neural-network-from-fully-connected-gad)
+
+## Book: Practical Computer Vision Applications Using Deep Learning with CNNs
+
+You can also check my book cited as [**Ahmed Fawzy Gad 'Practical Computer Vision Applications Using Deep Learning with CNNs'. Dec. 2018, Apress, 978-1-4842-4167-7**](https://www.amazon.com/Practical-Computer-Vision-Applications-Learning/dp/1484241665) which discusses neural networks, convolutional neural networks, deep learning, genetic algorithm, and more.
+
+Find the book at these links:
+
+- [Amazon](https://www.amazon.com/Practical-Computer-Vision-Applications-Learning/dp/1484241665)
+- [Springer](https://link.springer.com/book/10.1007/978-1-4842-4167-7)
+- [Apress](https://www.apress.com/gp/book/9781484241660)
+- [O'Reilly](https://www.oreilly.com/library/view/practical-computer-vision/9781484241677)
+- [Google Books](https://books.google.com.eg/books?id=xLd9DwAAQBAJ)
+
+![Fig04](https://user-images.githubusercontent.com/16560492/78830077-ae7c2800-79e7-11ea-980b-53b6bd879eeb.jpg)
+
+# Citing PyGAD - Bibtex Formatted Citation
+
+If you used PyGAD, please consider adding a citation to the following paper about PyGAD:
+
+```
+@misc{gad2021pygad,
+      title={PyGAD: An Intuitive Genetic Algorithm Python Library}, 
+      author={Ahmed Fawzy Gad},
+      year={2021},
+      eprint={2106.06158},
+      archivePrefix={arXiv},
+      primaryClass={cs.NE}
+}
+```
+
+# Contact Us
+
+* E-mail: ahmed.f.gad@gmail.com
+* [LinkedIn](https://www.linkedin.com/in/ahmedfgad)
+* [Paperspace](https://blog.paperspace.com/author/ahmed)
+* [KDnuggets](https://kdnuggets.com/author/ahmed-gad)
+* [TowardsDataScience](https://towardsdatascience.com/@ahmedfgad)
+* [GitHub](https://github.com/ahmedfgad)
+
+
```

### Comparing `pygad-2.9.0/README.md` & `pygad-3.0.0/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -1,56 +1,53 @@
-# GeneticAlgorithmPython: Building Genetic Algorithm in Python
+# PyGAD:  Genetic Algorithm in Python
 
-[This project](https://github.com/ahmedfgad/GeneticAlgorithmPython) is part of [PyGAD](https://pypi.org/project/pygad) which is an open-source Python 3 library for building the genetic algorithm and optimizing machine learning algorithms. 
+[PyGAD](https://pypi.org/project/pygad) is an open-source easy-to-use Python 3 library for building the genetic algorithm and optimizing machine learning algorithms. It supports Keras and PyTorch.
 
-Check documentation of the [GeneticAlgorithmPython](https://github.com/ahmedfgad/GeneticAlgorithmPython) project in the PyGAD's documentation: https://pygad.readthedocs.io/en/latest/README_pygad_ReadTheDocs.html
+Check documentation of the [PyGAD](https://pygad.readthedocs.io/en/latest).
+
+[![Downloads](https://pepy.tech/badge/pygad)](https://pepy.tech/project/pygad) ![Docs](https://readthedocs.org/projects/pygad/badge)
+
+![PYGAD-LOGO](https://user-images.githubusercontent.com/16560492/101267295-c74c0180-375f-11eb-9ad0-f8e37bd796ce.png)
 
 [PyGAD](https://pypi.org/project/pygad) supports different types of crossover, mutation, and parent selection. [PyGAD](https://pypi.org/project/pygad) allows different types of problems to be optimized using the genetic algorithm by customizing the fitness function. 
 
 The library is under active development and more features are added regularly. If you want a feature to be supported, please check the **Contact Us** section to send a request.
 
 # Donation
 
-You can donate via [Open Collective](https://opencollective.com/pygad): [opencollective.com/pygad](https://opencollective.com/pygad). 
-
-To donate using PayPal, use either this link: [paypal.me/ahmedfgad](https://paypal.me/ahmedfgad) or the e-mail address ahmed.f.gad@gmail.com.
-
-# Tutorial Project
-
-**IMPORTANT** If you are coming for the code of the tutorial titled  [**Genetic Algorithm Implementation in Python**](https://www.linkedin.com/pulse/genetic-algorithm-implementation-python-ahmed-gad), then it has been moved to the [Tutorial Project](https://github.com/ahmedfgad/GeneticAlgorithmPython/tree/master/Tutorial Project) directory on 06 May 2020.
+- [Credit/Debit Card](https://donate.stripe.com/eVa5kO866elKgM0144): https://donate.stripe.com/eVa5kO866elKgM0144
+- [Open Collective](https://opencollective.com/pygad): [opencollective.com/pygad](https://opencollective.com/pygad)
+- PayPal: Use either this link: [paypal.me/ahmedfgad](https://paypal.me/ahmedfgad) or the e-mail address ahmed.f.gad@gmail.com
+- Interac e-Transfer: Use e-mail address ahmed.f.gad@gmail.com
 
 # Installation
 
 To install [PyGAD](https://pypi.org/project/pygad), simply use pip to download and install the library from [PyPI](https://pypi.org/project/pygad) (Python Package Index). The library lives a PyPI at this page https://pypi.org/project/pygad.
 
-For Windows, issue the following command:
+Install PyGAD with the following command:
 
 ```python
 pip install pygad
 ```
 
-For Linux and Mac, replace `pip` by use `pip3` because the library only supports Python 3.
-
-```python
-pip3 install pygad
-```
-
 PyGAD is developed in Python 3.7.3 and depends on NumPy for creating and manipulating arrays and Matplotlib for creating figures. The exact NumPy version used in developing PyGAD is 1.16.4. For Matplotlib, the version is 3.1.0.
 
 To get started with PyGAD, please read the documentation at [Read The Docs](https://pygad.readthedocs.io/) https://pygad.readthedocs.io.
 
 # PyGAD Source Code
 
 The source code of the PyGAD' modules is found in the following GitHub projects:
 
 - [pygad](https://github.com/ahmedfgad/GeneticAlgorithmPython): (https://github.com/ahmedfgad/GeneticAlgorithmPython)
 - [pygad.nn](https://github.com/ahmedfgad/NumPyANN): https://github.com/ahmedfgad/NumPyANN
 - [pygad.gann](https://github.com/ahmedfgad/NeuralGenetic): https://github.com/ahmedfgad/NeuralGenetic
 - [pygad.cnn](https://github.com/ahmedfgad/NumPyCNN): https://github.com/ahmedfgad/NumPyCNN
 - [pygad.gacnn](https://github.com/ahmedfgad/CNNGenetic): https://github.com/ahmedfgad/CNNGenetic
+- [pygad.kerasga](https://github.com/ahmedfgad/KerasGA): https://github.com/ahmedfgad/KerasGA
+- [pygad.torchga](https://github.com/ahmedfgad/TorchGA): https://github.com/ahmedfgad/TorchGA
 
 The documentation of PyGAD is available at [Read The Docs](https://pygad.readthedocs.io/) https://pygad.readthedocs.io.
 
 # PyGAD Documentation
 
 The documentation of the PyGAD library is available at [Read The Docs](https://pygad.readthedocs.io) at this link: https://pygad.readthedocs.io. It discusses the modules supported by PyGAD, all its classes, methods, attribute, and functions. For each module, a number of examples are given.
 
@@ -64,15 +61,15 @@
 
 Please check the **Contact Us** section for more contact details.
 
 # Life Cycle of PyGAD
 
 The next figure lists the different stages in the lifecycle of an instance of the `pygad.GA` class. Note that PyGAD stops when either all generations are completed or when the function passed to the `on_generation` parameter returns the string `stop`.
 
-![PyGAD Lifecycle](https://user-images.githubusercontent.com/16560492/89446279-9c6f8380-d754-11ea-83fd-a60ea2f53b85.jpg)
+![PyGAD Lifecycle](https://user-images.githubusercontent.com/16560492/220486073-c5b6089d-81e4-44d9-a53c-385f479a7273.jpg)
 
 The next code implements all the callback functions to trace the execution of the genetic algorithm. Each callback function prints its name.
 
 ```python
 import pygad
 import numpy
 
@@ -181,54 +178,35 @@
 
 # To prepare the initial population, there are 2 ways:
 # 1) Prepare it yourself and pass it to the initial_population parameter. This way is useful when the user wants to start the genetic algorithm with a custom initial population.
 # 2) Assign valid integer values to the sol_per_pop and num_genes parameters. If the initial_population parameter exists, then the sol_per_pop and num_genes parameters are useless.
 sol_per_pop = 50 # Number of solutions in the population.
 num_genes = len(function_inputs)
 
-init_range_low = -2
-init_range_high = 5
-
-parent_selection_type = "sss" # Type of parent selection.
-keep_parents = 7 # Number of parents to keep in the next population. -1 means keep all parents and 0 means keep nothing.
-
-crossover_type = "single_point" # Type of the crossover operator.
-
-# Parameters of the mutation operation.
-mutation_type = "random" # Type of the mutation operator.
-mutation_percent_genes = 10 # Percentage of genes to mutate. This parameter has no action if the parameter mutation_num_genes exists or when mutation_type is None.
-
 last_fitness = 0
 def callback_generation(ga_instance):
     global last_fitness
     print("Generation = {generation}".format(generation=ga_instance.generations_completed))
     print("Fitness    = {fitness}".format(fitness=ga_instance.best_solution()[1]))
     print("Change     = {change}".format(change=ga_instance.best_solution()[1] - last_fitness))
     last_fitness = ga_instance.best_solution()[1]
 
 # Creating an instance of the GA class inside the ga module. Some parameters are initialized within the constructor.
 ga_instance = pygad.GA(num_generations=num_generations,
                        num_parents_mating=num_parents_mating, 
                        fitness_func=fitness_function,
                        sol_per_pop=sol_per_pop, 
                        num_genes=num_genes,
-                       init_range_low=init_range_low,
-                       init_range_high=init_range_high,
-                       parent_selection_type=parent_selection_type,
-                       keep_parents=keep_parents,
-                       crossover_type=crossover_type,
-                       mutation_type=mutation_type,
-                       mutation_percent_genes=mutation_percent_genes,
-                       callback_generation=callback_generation)
+                       on_generation=callback_generation)
 
 # Running the GA to optimize the parameters of the function.
 ga_instance.run()
 
 # After the generations complete, some plots are showed that summarize the how the outputs/fitenss values evolve over generations.
-ga_instance.plot_result()
+ga_instance.plot_fitness()
 
 # Returning the details of the best solution.
 solution, solution_fitness, solution_idx = ga_instance.best_solution()
 print("Parameters of the best solution : {solution}".format(solution=solution))
 print("Fitness value of the best solution = {solution_fitness}".format(solution_fitness=solution_fitness))
 print("Index of the best solution : {solution_idx}".format(solution_idx=solution_idx))
 
@@ -240,15 +218,15 @@
 
 # Saving the GA instance.
 filename = 'genetic' # The filename to which the instance is saved. The name is without extension.
 ga_instance.save(filename=filename)
 
 # Loading the saved GA instance.
 loaded_ga_instance = pygad.load(filename=filename)
-loaded_ga_instance.plot_result()
+loaded_ga_instance.plot_fitness()
 ```
 
 # For More Information
 
 There are different resources that can be used to get started with the genetic algorithm and building it in Python. 
 
 ## Tutorial: Implementing Genetic Algorithm in Python
@@ -264,16 +242,16 @@
 [![Genetic Algorithm Implementation in Python](https://user-images.githubusercontent.com/16560492/78830052-a3c19300-79e7-11ea-8b9b-4b343ea4049c.png)](https://www.linkedin.com/pulse/genetic-algorithm-implementation-python-ahmed-gad)
 
 ## Tutorial: Introduction to Genetic Algorithm
 
 Get started with the genetic algorithm by reading the tutorial titled [**Introduction to Optimization with Genetic Algorithm**](https://www.linkedin.com/pulse/introduction-optimization-genetic-algorithm-ahmed-gad) which is available at these links:
 
 * [LinkedIn](https://www.linkedin.com/pulse/introduction-optimization-genetic-algorithm-ahmed-gad)
-* [Towards Data Science](https://www.kdnuggets.com/2018/03/introduction-optimization-with-genetic-algorithm.html)
-* [KDnuggets](https://towardsdatascience.com/introduction-to-optimization-with-genetic-algorithm-2f5001d9964b)
+* [Towards Data Science](https://towardsdatascience.com/introduction-to-optimization-with-genetic-algorithm-2f5001d9964b)
+* [KDnuggets](https://www.kdnuggets.com/2018/03/introduction-optimization-with-genetic-algorithm.html)
 
 [![Introduction to Genetic Algorithm](https://user-images.githubusercontent.com/16560492/82078259-26252d00-96e1-11ea-9a02-52a99e1054b9.jpg)](https://www.linkedin.com/pulse/introduction-optimization-genetic-algorithm-ahmed-gad)
 
 ## Tutorial: Build Neural Networks in Python
 
 Read about building neural networks in Python through the tutorial titled [**Artificial Neural Network Implementation using NumPy and Classification of the Fruits360 Image Dataset**](https://www.linkedin.com/pulse/artificial-neural-network-implementation-using-numpy-fruits360-gad) available at these links:
 
@@ -326,18 +304,30 @@
 - [Springer](https://link.springer.com/book/10.1007/978-1-4842-4167-7)
 - [Apress](https://www.apress.com/gp/book/9781484241660)
 - [O'Reilly](https://www.oreilly.com/library/view/practical-computer-vision/9781484241677)
 - [Google Books](https://books.google.com.eg/books?id=xLd9DwAAQBAJ)
 
 ![Fig04](https://user-images.githubusercontent.com/16560492/78830077-ae7c2800-79e7-11ea-980b-53b6bd879eeb.jpg)
 
+# Citing PyGAD - Bibtex Formatted Citation
+
+If you used PyGAD, please consider adding a citation to the following paper about PyGAD:
+
+```
+@misc{gad2021pygad,
+      title={PyGAD: An Intuitive Genetic Algorithm Python Library}, 
+      author={Ahmed Fawzy Gad},
+      year={2021},
+      eprint={2106.06158},
+      archivePrefix={arXiv},
+      primaryClass={cs.NE}
+}
+```
+
 # Contact Us
 
 * E-mail: ahmed.f.gad@gmail.com
 * [LinkedIn](https://www.linkedin.com/in/ahmedfgad)
-* [Amazon Author Page](https://amazon.com/author/ahmedgad)
-* [Heartbeat](https://heartbeat.fritz.ai/@ahmedfgad)
 * [Paperspace](https://blog.paperspace.com/author/ahmed)
 * [KDnuggets](https://kdnuggets.com/author/ahmed-gad)
 * [TowardsDataScience](https://towardsdatascience.com/@ahmedfgad)
 * [GitHub](https://github.com/ahmedfgad)
-
```

### Comparing `pygad-2.9.0/pygad/cnn/cnn.py` & `pygad-3.0.0/pygad/cnn/cnn.py`

 * *Files identical despite different names*

### Comparing `pygad-2.9.0/pygad/gacnn/gacnn.py` & `pygad-3.0.0/pygad/gacnn/gacnn.py`

 * *Files identical despite different names*

### Comparing `pygad-2.9.0/pygad/gann/gann.py` & `pygad-3.0.0/pygad/gann/gann.py`

 * *Files identical despite different names*

### Comparing `pygad-2.9.0/pygad/kerasga/kerasga.py` & `pygad-3.0.0/pygad/kerasga/kerasga.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,35 +1,56 @@
 import copy
 import numpy
+import tensorflow.keras
 
 def model_weights_as_vector(model):
     weights_vector = []
 
-    for layer_weights in model.get_weights():
-        vector = numpy.reshape(layer_weights, newshape=(layer_weights.size))
-        weights_vector.extend(vector)
+    for layer in model.layers: # model.get_weights():
+        if layer.trainable:
+            layer_weights = layer.get_weights()
+            for l_weights in layer_weights:
+                vector = numpy.reshape(l_weights, newshape=(l_weights.size))
+                weights_vector.extend(vector)
 
     return numpy.array(weights_vector)
 
 def model_weights_as_matrix(model, weights_vector):
     weights_matrix = []
 
     start = 0
-    for w_matrix in model.get_weights():
-        layer_weights_shape = w_matrix.shape
-        layer_weights_size = w_matrix.size
-
-        layer_weights_vector = weights_vector[start:start + layer_weights_size]
-        layer_weights_matrix = numpy.reshape(layer_weights_vector, newshape=(layer_weights_shape))
-        weights_matrix.append(layer_weights_matrix)
-
-        start = start + layer_weights_size
+    for layer_idx, layer in enumerate(model.layers): # model.get_weights():
+    # for w_matrix in model.get_weights():
+        layer_weights = layer.get_weights()
+        if layer.trainable:
+            for l_weights in layer_weights:
+                layer_weights_shape = l_weights.shape
+                layer_weights_size = l_weights.size
+        
+                layer_weights_vector = weights_vector[start:start + layer_weights_size]
+                layer_weights_matrix = numpy.reshape(layer_weights_vector, newshape=(layer_weights_shape))
+                weights_matrix.append(layer_weights_matrix)
+        
+                start = start + layer_weights_size
+        else:
+            for l_weights in layer_weights:
+                weights_matrix.append(l_weights)
 
     return weights_matrix
 
+def predict(model, solution, data):
+    # Fetch the parameters of the best solution.
+    solution_weights = model_weights_as_matrix(model=model,
+                                               weights_vector=solution)
+    _model = tensorflow.keras.models.clone_model(model)
+    _model.set_weights(solution_weights)
+    predictions = _model.predict(data)
+
+    return predictions
+
 class KerasGA:
 
     def __init__(self, model, num_solutions):
 
         """
         Creates an instance of the KerasGA class to build a population of model parameters.
```

### Comparing `pygad-2.9.0/pygad/nn/nn.py` & `pygad-3.0.0/pygad/nn/nn.py`

 * *Files identical despite different names*

### Comparing `pygad-2.9.0/pygad.egg-info/PKG-INFO` & `pygad-3.0.0/pygad.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,354 +1,346 @@
 Metadata-Version: 2.1
 Name: pygad
-Version: 2.9.0
-Summary: PyGAD: A Python Library for Building the Genetic Algorithm.
+Version: 3.0.0
+Summary: PyGAD: A Python 3 Library for Building the Genetic Algorithm and Training Machine Learning Algoithms (Keras & PyTorch).
 Home-page: https://github.com/ahmedfgad/GeneticAlgorithmPython
 Author: Ahmed Fawzy Gad
 Author-email: ahmed.f.gad@gmail.com
 License: UNKNOWN
-Description: # GeneticAlgorithmPython: Building Genetic Algorithm in Python
-        
-        [This project](https://github.com/ahmedfgad/GeneticAlgorithmPython) is part of [PyGAD](https://pypi.org/project/pygad) which is an open-source Python 3 library for building the genetic algorithm and optimizing machine learning algorithms. 
-        
-        Check documentation of the [GeneticAlgorithmPython](https://github.com/ahmedfgad/GeneticAlgorithmPython) project in the PyGAD's documentation: https://pygad.readthedocs.io/en/latest/README_pygad_ReadTheDocs.html
-        
-        [PyGAD](https://pypi.org/project/pygad) supports different types of crossover, mutation, and parent selection. [PyGAD](https://pypi.org/project/pygad) allows different types of problems to be optimized using the genetic algorithm by customizing the fitness function. 
-        
-        The library is under active development and more features are added regularly. If you want a feature to be supported, please check the **Contact Us** section to send a request.
-        
-        # Donation
-        
-        You can donate via [Open Collective](https://opencollective.com/pygad): [opencollective.com/pygad](https://opencollective.com/pygad). 
-        
-        To donate using PayPal, use either this link: [paypal.me/ahmedfgad](https://paypal.me/ahmedfgad) or the e-mail address ahmed.f.gad@gmail.com.
-        
-        # Tutorial Project
-        
-        **IMPORTANT** If you are coming for the code of the tutorial titled  [**Genetic Algorithm Implementation in Python**](https://www.linkedin.com/pulse/genetic-algorithm-implementation-python-ahmed-gad), then it has been moved to the [Tutorial Project](https://github.com/ahmedfgad/GeneticAlgorithmPython/tree/master/Tutorial Project) directory on 06 May 2020.
-        
-        # Installation
-        
-        To install [PyGAD](https://pypi.org/project/pygad), simply use pip to download and install the library from [PyPI](https://pypi.org/project/pygad) (Python Package Index). The library lives a PyPI at this page https://pypi.org/project/pygad.
-        
-        For Windows, issue the following command:
-        
-        ```python
-        pip install pygad
-        ```
-        
-        For Linux and Mac, replace `pip` by use `pip3` because the library only supports Python 3.
-        
-        ```python
-        pip3 install pygad
-        ```
-        
-        PyGAD is developed in Python 3.7.3 and depends on NumPy for creating and manipulating arrays and Matplotlib for creating figures. The exact NumPy version used in developing PyGAD is 1.16.4. For Matplotlib, the version is 3.1.0.
-        
-        To get started with PyGAD, please read the documentation at [Read The Docs](https://pygad.readthedocs.io/) https://pygad.readthedocs.io.
-        
-        # PyGAD Source Code
-        
-        The source code of the PyGAD' modules is found in the following GitHub projects:
-        
-        - [pygad](https://github.com/ahmedfgad/GeneticAlgorithmPython): (https://github.com/ahmedfgad/GeneticAlgorithmPython)
-        - [pygad.nn](https://github.com/ahmedfgad/NumPyANN): https://github.com/ahmedfgad/NumPyANN
-        - [pygad.gann](https://github.com/ahmedfgad/NeuralGenetic): https://github.com/ahmedfgad/NeuralGenetic
-        - [pygad.cnn](https://github.com/ahmedfgad/NumPyCNN): https://github.com/ahmedfgad/NumPyCNN
-        - [pygad.gacnn](https://github.com/ahmedfgad/CNNGenetic): https://github.com/ahmedfgad/CNNGenetic
-        
-        The documentation of PyGAD is available at [Read The Docs](https://pygad.readthedocs.io/) https://pygad.readthedocs.io.
-        
-        # PyGAD Documentation
-        
-        The documentation of the PyGAD library is available at [Read The Docs](https://pygad.readthedocs.io) at this link: https://pygad.readthedocs.io. It discusses the modules supported by PyGAD, all its classes, methods, attribute, and functions. For each module, a number of examples are given.
-        
-        If there is an issue using PyGAD, feel free to post at issue in this [GitHub repository](https://github.com/ahmedfgad/GeneticAlgorithmPython) https://github.com/ahmedfgad/GeneticAlgorithmPython or by sending an e-mail to ahmed.f.gad@gmail.com. 
-        
-        If you built a project that uses PyGAD, then please drop an e-mail to ahmed.f.gad@gmail.com with the following information so that your project is included in the documentation.
-        
-        - Project title
-        - Brief description
-        - Preferably, a link that directs the readers to your project
-        
-        Please check the **Contact Us** section for more contact details.
-        
-        # Life Cycle of PyGAD
-        
-        The next figure lists the different stages in the lifecycle of an instance of the `pygad.GA` class. Note that PyGAD stops when either all generations are completed or when the function passed to the `on_generation` parameter returns the string `stop`.
-        
-        ![PyGAD Lifecycle](https://user-images.githubusercontent.com/16560492/89446279-9c6f8380-d754-11ea-83fd-a60ea2f53b85.jpg)
-        
-        The next code implements all the callback functions to trace the execution of the genetic algorithm. Each callback function prints its name.
-        
-        ```python
-        import pygad
-        import numpy
-        
-        function_inputs = [4,-2,3.5,5,-11,-4.7]
-        desired_output = 44
-        
-        def fitness_func(solution, solution_idx):
-            output = numpy.sum(solution*function_inputs)
-            fitness = 1.0 / (numpy.abs(output - desired_output) + 0.000001)
-            return fitness
-        
-        fitness_function = fitness_func
-        
-        def on_start(ga_instance):
-            print("on_start()")
-        
-        def on_fitness(ga_instance, population_fitness):
-            print("on_fitness()")
-        
-        def on_parents(ga_instance, selected_parents):
-            print("on_parents()")
-        
-        def on_crossover(ga_instance, offspring_crossover):
-            print("on_crossover()")
-        
-        def on_mutation(ga_instance, offspring_mutation):
-            print("on_mutation()")
-        
-        def on_generation(ga_instance):
-            print("on_generation()")
-        
-        def on_stop(ga_instance, last_population_fitness):
-            print("on_stop()")
-        
-        ga_instance = pygad.GA(num_generations=3,
-                               num_parents_mating=5,
-                               fitness_func=fitness_function,
-                               sol_per_pop=10,
-                               num_genes=len(function_inputs),
-                               on_start=on_start,
-                               on_fitness=on_fitness,
-                               on_parents=on_parents,
-                               on_crossover=on_crossover,
-                               on_mutation=on_mutation,
-                               on_generation=on_generation,
-                               on_stop=on_stop)
-        
-        ga_instance.run()
-        ```
-        
-        Based on the used 3 generations as assigned to the `num_generations` argument, here is the output.
-        
-        ```
-        on_start()
-        
-        on_fitness()
-        on_parents()
-        on_crossover()
-        on_mutation()
-        on_generation()
-        
-        on_fitness()
-        on_parents()
-        on_crossover()
-        on_mutation()
-        on_generation()
-        
-        on_fitness()
-        on_parents()
-        on_crossover()
-        on_mutation()
-        on_generation()
-        
-        on_stop()
-        ```
-        
-        # Example
-        
-        Check the [PyGAD's documentation](https://pygad.readthedocs.io/en/latest/README_pygad_ReadTheDocs.html) for information about the implementation of this example.
-        
-        ```python
-        import pygad
-        import numpy
-        
-        """
-        Given the following function:
-            y = f(w1:w6) = w1x1 + w2x2 + w3x3 + w4x4 + w5x5 + 6wx6
-            where (x1,x2,x3,x4,x5,x6)=(4,-2,3.5,5,-11,-4.7) and y=44
-        What are the best values for the 6 weights (w1 to w6)? We are going to use the genetic algorithm to optimize this function.
-        """
-        
-        function_inputs = [4,-2,3.5,5,-11,-4.7] # Function inputs.
-        desired_output = 44 # Function output.
-        
-        def fitness_func(solution, solution_idx):
-            # Calculating the fitness value of each solution in the current population.
-            # The fitness function calulates the sum of products between each input and its corresponding weight.
-            output = numpy.sum(solution*function_inputs)
-            fitness = 1.0 / numpy.abs(output - desired_output)
-            return fitness
-        
-        fitness_function = fitness_func
-        
-        num_generations = 100 # Number of generations.
-        num_parents_mating = 7 # Number of solutions to be selected as parents in the mating pool.
-        
-        # To prepare the initial population, there are 2 ways:
-        # 1) Prepare it yourself and pass it to the initial_population parameter. This way is useful when the user wants to start the genetic algorithm with a custom initial population.
-        # 2) Assign valid integer values to the sol_per_pop and num_genes parameters. If the initial_population parameter exists, then the sol_per_pop and num_genes parameters are useless.
-        sol_per_pop = 50 # Number of solutions in the population.
-        num_genes = len(function_inputs)
-        
-        init_range_low = -2
-        init_range_high = 5
-        
-        parent_selection_type = "sss" # Type of parent selection.
-        keep_parents = 7 # Number of parents to keep in the next population. -1 means keep all parents and 0 means keep nothing.
-        
-        crossover_type = "single_point" # Type of the crossover operator.
-        
-        # Parameters of the mutation operation.
-        mutation_type = "random" # Type of the mutation operator.
-        mutation_percent_genes = 10 # Percentage of genes to mutate. This parameter has no action if the parameter mutation_num_genes exists or when mutation_type is None.
-        
-        last_fitness = 0
-        def callback_generation(ga_instance):
-            global last_fitness
-            print("Generation = {generation}".format(generation=ga_instance.generations_completed))
-            print("Fitness    = {fitness}".format(fitness=ga_instance.best_solution()[1]))
-            print("Change     = {change}".format(change=ga_instance.best_solution()[1] - last_fitness))
-            last_fitness = ga_instance.best_solution()[1]
-        
-        # Creating an instance of the GA class inside the ga module. Some parameters are initialized within the constructor.
-        ga_instance = pygad.GA(num_generations=num_generations,
-                               num_parents_mating=num_parents_mating, 
-                               fitness_func=fitness_function,
-                               sol_per_pop=sol_per_pop, 
-                               num_genes=num_genes,
-                               init_range_low=init_range_low,
-                               init_range_high=init_range_high,
-                               parent_selection_type=parent_selection_type,
-                               keep_parents=keep_parents,
-                               crossover_type=crossover_type,
-                               mutation_type=mutation_type,
-                               mutation_percent_genes=mutation_percent_genes,
-                               callback_generation=callback_generation)
-        
-        # Running the GA to optimize the parameters of the function.
-        ga_instance.run()
-        
-        # After the generations complete, some plots are showed that summarize the how the outputs/fitenss values evolve over generations.
-        ga_instance.plot_result()
-        
-        # Returning the details of the best solution.
-        solution, solution_fitness, solution_idx = ga_instance.best_solution()
-        print("Parameters of the best solution : {solution}".format(solution=solution))
-        print("Fitness value of the best solution = {solution_fitness}".format(solution_fitness=solution_fitness))
-        print("Index of the best solution : {solution_idx}".format(solution_idx=solution_idx))
-        
-        prediction = numpy.sum(numpy.array(function_inputs)*solution)
-        print("Predicted output based on the best solution : {prediction}".format(prediction=prediction))
-        
-        if ga_instance.best_solution_generation != -1:
-            print("Best fitness value reached after {best_solution_generation} generations.".format(best_solution_generation=ga_instance.best_solution_generation))
-        
-        # Saving the GA instance.
-        filename = 'genetic' # The filename to which the instance is saved. The name is without extension.
-        ga_instance.save(filename=filename)
-        
-        # Loading the saved GA instance.
-        loaded_ga_instance = pygad.load(filename=filename)
-        loaded_ga_instance.plot_result()
-        ```
-        
-        # For More Information
-        
-        There are different resources that can be used to get started with the genetic algorithm and building it in Python. 
-        
-        ## Tutorial: Implementing Genetic Algorithm in Python
-        
-        To start with coding the genetic algorithm, you can check the tutorial titled [**Genetic Algorithm Implementation in Python**](https://www.linkedin.com/pulse/genetic-algorithm-implementation-python-ahmed-gad) available at these links:
-        
-        - [LinkedIn](https://www.linkedin.com/pulse/genetic-algorithm-implementation-python-ahmed-gad)
-        - [Towards Data Science](https://towardsdatascience.com/genetic-algorithm-implementation-in-python-5ab67bb124a6)
-        - [KDnuggets](https://www.kdnuggets.com/2018/07/genetic-algorithm-implementation-python.html)
-        
-        [This tutorial](https://www.linkedin.com/pulse/genetic-algorithm-implementation-python-ahmed-gad) is prepared based on a previous version of the project but it still a good resource to start with coding the genetic algorithm.
-        
-        [![Genetic Algorithm Implementation in Python](https://user-images.githubusercontent.com/16560492/78830052-a3c19300-79e7-11ea-8b9b-4b343ea4049c.png)](https://www.linkedin.com/pulse/genetic-algorithm-implementation-python-ahmed-gad)
-        
-        ## Tutorial: Introduction to Genetic Algorithm
-        
-        Get started with the genetic algorithm by reading the tutorial titled [**Introduction to Optimization with Genetic Algorithm**](https://www.linkedin.com/pulse/introduction-optimization-genetic-algorithm-ahmed-gad) which is available at these links:
-        
-        * [LinkedIn](https://www.linkedin.com/pulse/introduction-optimization-genetic-algorithm-ahmed-gad)
-        * [Towards Data Science](https://www.kdnuggets.com/2018/03/introduction-optimization-with-genetic-algorithm.html)
-        * [KDnuggets](https://towardsdatascience.com/introduction-to-optimization-with-genetic-algorithm-2f5001d9964b)
-        
-        [![Introduction to Genetic Algorithm](https://user-images.githubusercontent.com/16560492/82078259-26252d00-96e1-11ea-9a02-52a99e1054b9.jpg)](https://www.linkedin.com/pulse/introduction-optimization-genetic-algorithm-ahmed-gad)
-        
-        ## Tutorial: Build Neural Networks in Python
-        
-        Read about building neural networks in Python through the tutorial titled [**Artificial Neural Network Implementation using NumPy and Classification of the Fruits360 Image Dataset**](https://www.linkedin.com/pulse/artificial-neural-network-implementation-using-numpy-fruits360-gad) available at these links:
-        
-        * [LinkedIn](https://www.linkedin.com/pulse/artificial-neural-network-implementation-using-numpy-fruits360-gad)
-        * [Towards Data Science](https://towardsdatascience.com/artificial-neural-network-implementation-using-numpy-and-classification-of-the-fruits360-image-3c56affa4491)
-        * [KDnuggets](https://www.kdnuggets.com/2019/02/artificial-neural-network-implementation-using-numpy-and-image-classification.html)
-        
-        [![Building Neural Networks Python](https://user-images.githubusercontent.com/16560492/82078281-30472b80-96e1-11ea-8017-6a1f4383d602.jpg)](https://www.linkedin.com/pulse/artificial-neural-network-implementation-using-numpy-fruits360-gad)
-        
-        ## Tutorial: Optimize Neural Networks with Genetic Algorithm
-        
-        Read about training neural networks using the genetic algorithm through the tutorial titled [**Artificial Neural Networks Optimization using Genetic Algorithm with Python**](https://www.linkedin.com/pulse/artificial-neural-networks-optimization-using-genetic-ahmed-gad) available at these links:
-        
-        - [LinkedIn](https://www.linkedin.com/pulse/artificial-neural-networks-optimization-using-genetic-ahmed-gad)
-        - [Towards Data Science](https://towardsdatascience.com/artificial-neural-networks-optimization-using-genetic-algorithm-with-python-1fe8ed17733e)
-        - [KDnuggets](https://www.kdnuggets.com/2019/03/artificial-neural-networks-optimization-genetic-algorithm-python.html)
-        
-        [![Training Neural Networks using Genetic Algorithm Python](https://user-images.githubusercontent.com/16560492/82078300-376e3980-96e1-11ea-821c-aa6b8ceb44d4.jpg)](https://www.linkedin.com/pulse/artificial-neural-networks-optimization-using-genetic-ahmed-gad)
-        
-        ## Tutorial: Building CNN in Python
-        
-        To start with coding the genetic algorithm, you can check the tutorial titled [**Building Convolutional Neural Network using NumPy from Scratch**](https://www.linkedin.com/pulse/building-convolutional-neural-network-using-numpy-from-ahmed-gad) available at these links:
-        
-        - [LinkedIn](https://www.linkedin.com/pulse/building-convolutional-neural-network-using-numpy-from-ahmed-gad)
-        - [Towards Data Science](https://towardsdatascience.com/building-convolutional-neural-network-using-numpy-from-scratch-b30aac50e50a)
-        - [KDnuggets](https://www.kdnuggets.com/2018/04/building-convolutional-neural-network-numpy-scratch.html)
-        - [Chinese Translation](http://m.aliyun.com/yunqi/articles/585741)
-        
-        [This tutorial](https://www.linkedin.com/pulse/building-convolutional-neural-network-using-numpy-from-ahmed-gad)) is prepared based on a previous version of the project but it still a good resource to start with coding CNNs.
-        
-        [![Building CNN in Python](https://user-images.githubusercontent.com/16560492/82431022-6c3a1200-9a8e-11ea-8f1b-b055196d76e3.png)](https://www.linkedin.com/pulse/building-convolutional-neural-network-using-numpy-from-ahmed-gad)
-        
-        ## Tutorial: Derivation of CNN from FCNN
-        
-        Get started with the genetic algorithm by reading the tutorial titled [**Derivation of Convolutional Neural Network from Fully Connected Network Step-By-Step**](https://www.linkedin.com/pulse/derivation-convolutional-neural-network-from-fully-connected-gad) which is available at these links:
-        
-        * [LinkedIn](https://www.linkedin.com/pulse/derivation-convolutional-neural-network-from-fully-connected-gad)
-        * [Towards Data Science](https://towardsdatascience.com/derivation-of-convolutional-neural-network-from-fully-connected-network-step-by-step-b42ebafa5275)
-        * [KDnuggets](https://www.kdnuggets.com/2018/04/derivation-convolutional-neural-network-fully-connected-step-by-step.html)
-        
-        [![Derivation of CNN from FCNN](https://user-images.githubusercontent.com/16560492/82431369-db176b00-9a8e-11ea-99bd-e845192873fc.png)](https://www.linkedin.com/pulse/derivation-convolutional-neural-network-from-fully-connected-gad)
-        
-        ## Book: Practical Computer Vision Applications Using Deep Learning with CNNs
-        
-        You can also check my book cited as [**Ahmed Fawzy Gad 'Practical Computer Vision Applications Using Deep Learning with CNNs'. Dec. 2018, Apress, 978-1-4842-4167-7**](https://www.amazon.com/Practical-Computer-Vision-Applications-Learning/dp/1484241665) which discusses neural networks, convolutional neural networks, deep learning, genetic algorithm, and more.
-        
-        Find the book at these links:
-        
-        - [Amazon](https://www.amazon.com/Practical-Computer-Vision-Applications-Learning/dp/1484241665)
-        - [Springer](https://link.springer.com/book/10.1007/978-1-4842-4167-7)
-        - [Apress](https://www.apress.com/gp/book/9781484241660)
-        - [O'Reilly](https://www.oreilly.com/library/view/practical-computer-vision/9781484241677)
-        - [Google Books](https://books.google.com.eg/books?id=xLd9DwAAQBAJ)
-        
-        ![Fig04](https://user-images.githubusercontent.com/16560492/78830077-ae7c2800-79e7-11ea-980b-53b6bd879eeb.jpg)
-        
-        # Contact Us
-        
-        * E-mail: ahmed.f.gad@gmail.com
-        * [LinkedIn](https://www.linkedin.com/in/ahmedfgad)
-        * [Amazon Author Page](https://amazon.com/author/ahmedgad)
-        * [Heartbeat](https://heartbeat.fritz.ai/@ahmedfgad)
-        * [Paperspace](https://blog.paperspace.com/author/ahmed)
-        * [KDnuggets](https://kdnuggets.com/author/ahmed-gad)
-        * [TowardsDataScience](https://towardsdatascience.com/@ahmedfgad)
-        * [GitHub](https://github.com/ahmedfgad)
-        
-        
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
+
+# PyGAD:  Genetic Algorithm in Python
+
+[PyGAD](https://pypi.org/project/pygad) is an open-source easy-to-use Python 3 library for building the genetic algorithm and optimizing machine learning algorithms. It supports Keras and PyTorch.
+
+Check documentation of the [PyGAD](https://pygad.readthedocs.io/en/latest).
+
+[![Downloads](https://pepy.tech/badge/pygad)](https://pepy.tech/project/pygad) ![Docs](https://readthedocs.org/projects/pygad/badge)
+
+![PYGAD-LOGO](https://user-images.githubusercontent.com/16560492/101267295-c74c0180-375f-11eb-9ad0-f8e37bd796ce.png)
+
+[PyGAD](https://pypi.org/project/pygad) supports different types of crossover, mutation, and parent selection. [PyGAD](https://pypi.org/project/pygad) allows different types of problems to be optimized using the genetic algorithm by customizing the fitness function. 
+
+The library is under active development and more features are added regularly. If you want a feature to be supported, please check the **Contact Us** section to send a request.
+
+# Donation
+
+- [Credit/Debit Card](https://donate.stripe.com/eVa5kO866elKgM0144): https://donate.stripe.com/eVa5kO866elKgM0144
+- [Open Collective](https://opencollective.com/pygad): [opencollective.com/pygad](https://opencollective.com/pygad)
+- PayPal: Use either this link: [paypal.me/ahmedfgad](https://paypal.me/ahmedfgad) or the e-mail address ahmed.f.gad@gmail.com
+- Interac e-Transfer: Use e-mail address ahmed.f.gad@gmail.com
+
+# Installation
+
+To install [PyGAD](https://pypi.org/project/pygad), simply use pip to download and install the library from [PyPI](https://pypi.org/project/pygad) (Python Package Index). The library lives a PyPI at this page https://pypi.org/project/pygad.
+
+Install PyGAD with the following command:
+
+```python
+pip install pygad
+```
+
+PyGAD is developed in Python 3.7.3 and depends on NumPy for creating and manipulating arrays and Matplotlib for creating figures. The exact NumPy version used in developing PyGAD is 1.16.4. For Matplotlib, the version is 3.1.0.
+
+To get started with PyGAD, please read the documentation at [Read The Docs](https://pygad.readthedocs.io/) https://pygad.readthedocs.io.
+
+# PyGAD Source Code
+
+The source code of the PyGAD' modules is found in the following GitHub projects:
+
+- [pygad](https://github.com/ahmedfgad/GeneticAlgorithmPython): (https://github.com/ahmedfgad/GeneticAlgorithmPython)
+- [pygad.nn](https://github.com/ahmedfgad/NumPyANN): https://github.com/ahmedfgad/NumPyANN
+- [pygad.gann](https://github.com/ahmedfgad/NeuralGenetic): https://github.com/ahmedfgad/NeuralGenetic
+- [pygad.cnn](https://github.com/ahmedfgad/NumPyCNN): https://github.com/ahmedfgad/NumPyCNN
+- [pygad.gacnn](https://github.com/ahmedfgad/CNNGenetic): https://github.com/ahmedfgad/CNNGenetic
+- [pygad.kerasga](https://github.com/ahmedfgad/KerasGA): https://github.com/ahmedfgad/KerasGA
+- [pygad.torchga](https://github.com/ahmedfgad/TorchGA): https://github.com/ahmedfgad/TorchGA
+
+The documentation of PyGAD is available at [Read The Docs](https://pygad.readthedocs.io/) https://pygad.readthedocs.io.
+
+# PyGAD Documentation
+
+The documentation of the PyGAD library is available at [Read The Docs](https://pygad.readthedocs.io) at this link: https://pygad.readthedocs.io. It discusses the modules supported by PyGAD, all its classes, methods, attribute, and functions. For each module, a number of examples are given.
+
+If there is an issue using PyGAD, feel free to post at issue in this [GitHub repository](https://github.com/ahmedfgad/GeneticAlgorithmPython) https://github.com/ahmedfgad/GeneticAlgorithmPython or by sending an e-mail to ahmed.f.gad@gmail.com. 
+
+If you built a project that uses PyGAD, then please drop an e-mail to ahmed.f.gad@gmail.com with the following information so that your project is included in the documentation.
+
+- Project title
+- Brief description
+- Preferably, a link that directs the readers to your project
+
+Please check the **Contact Us** section for more contact details.
+
+# Life Cycle of PyGAD
+
+The next figure lists the different stages in the lifecycle of an instance of the `pygad.GA` class. Note that PyGAD stops when either all generations are completed or when the function passed to the `on_generation` parameter returns the string `stop`.
+
+![PyGAD Lifecycle](https://user-images.githubusercontent.com/16560492/220486073-c5b6089d-81e4-44d9-a53c-385f479a7273.jpg)
+
+The next code implements all the callback functions to trace the execution of the genetic algorithm. Each callback function prints its name.
+
+```python
+import pygad
+import numpy
+
+function_inputs = [4,-2,3.5,5,-11,-4.7]
+desired_output = 44
+
+def fitness_func(solution, solution_idx):
+    output = numpy.sum(solution*function_inputs)
+    fitness = 1.0 / (numpy.abs(output - desired_output) + 0.000001)
+    return fitness
+
+fitness_function = fitness_func
+
+def on_start(ga_instance):
+    print("on_start()")
+
+def on_fitness(ga_instance, population_fitness):
+    print("on_fitness()")
+
+def on_parents(ga_instance, selected_parents):
+    print("on_parents()")
+
+def on_crossover(ga_instance, offspring_crossover):
+    print("on_crossover()")
+
+def on_mutation(ga_instance, offspring_mutation):
+    print("on_mutation()")
+
+def on_generation(ga_instance):
+    print("on_generation()")
+
+def on_stop(ga_instance, last_population_fitness):
+    print("on_stop()")
+
+ga_instance = pygad.GA(num_generations=3,
+                       num_parents_mating=5,
+                       fitness_func=fitness_function,
+                       sol_per_pop=10,
+                       num_genes=len(function_inputs),
+                       on_start=on_start,
+                       on_fitness=on_fitness,
+                       on_parents=on_parents,
+                       on_crossover=on_crossover,
+                       on_mutation=on_mutation,
+                       on_generation=on_generation,
+                       on_stop=on_stop)
+
+ga_instance.run()
+```
+
+Based on the used 3 generations as assigned to the `num_generations` argument, here is the output.
+
+```
+on_start()
+
+on_fitness()
+on_parents()
+on_crossover()
+on_mutation()
+on_generation()
+
+on_fitness()
+on_parents()
+on_crossover()
+on_mutation()
+on_generation()
+
+on_fitness()
+on_parents()
+on_crossover()
+on_mutation()
+on_generation()
+
+on_stop()
+```
+
+# Example
+
+Check the [PyGAD's documentation](https://pygad.readthedocs.io/en/latest/README_pygad_ReadTheDocs.html) for information about the implementation of this example.
+
+```python
+import pygad
+import numpy
+
+"""
+Given the following function:
+    y = f(w1:w6) = w1x1 + w2x2 + w3x3 + w4x4 + w5x5 + 6wx6
+    where (x1,x2,x3,x4,x5,x6)=(4,-2,3.5,5,-11,-4.7) and y=44
+What are the best values for the 6 weights (w1 to w6)? We are going to use the genetic algorithm to optimize this function.
+"""
+
+function_inputs = [4,-2,3.5,5,-11,-4.7] # Function inputs.
+desired_output = 44 # Function output.
+
+def fitness_func(solution, solution_idx):
+    # Calculating the fitness value of each solution in the current population.
+    # The fitness function calulates the sum of products between each input and its corresponding weight.
+    output = numpy.sum(solution*function_inputs)
+    fitness = 1.0 / numpy.abs(output - desired_output)
+    return fitness
+
+fitness_function = fitness_func
+
+num_generations = 100 # Number of generations.
+num_parents_mating = 7 # Number of solutions to be selected as parents in the mating pool.
+
+# To prepare the initial population, there are 2 ways:
+# 1) Prepare it yourself and pass it to the initial_population parameter. This way is useful when the user wants to start the genetic algorithm with a custom initial population.
+# 2) Assign valid integer values to the sol_per_pop and num_genes parameters. If the initial_population parameter exists, then the sol_per_pop and num_genes parameters are useless.
+sol_per_pop = 50 # Number of solutions in the population.
+num_genes = len(function_inputs)
+
+last_fitness = 0
+def callback_generation(ga_instance):
+    global last_fitness
+    print("Generation = {generation}".format(generation=ga_instance.generations_completed))
+    print("Fitness    = {fitness}".format(fitness=ga_instance.best_solution()[1]))
+    print("Change     = {change}".format(change=ga_instance.best_solution()[1] - last_fitness))
+    last_fitness = ga_instance.best_solution()[1]
+
+# Creating an instance of the GA class inside the ga module. Some parameters are initialized within the constructor.
+ga_instance = pygad.GA(num_generations=num_generations,
+                       num_parents_mating=num_parents_mating, 
+                       fitness_func=fitness_function,
+                       sol_per_pop=sol_per_pop, 
+                       num_genes=num_genes,
+                       on_generation=callback_generation)
+
+# Running the GA to optimize the parameters of the function.
+ga_instance.run()
+
+# After the generations complete, some plots are showed that summarize the how the outputs/fitenss values evolve over generations.
+ga_instance.plot_fitness()
+
+# Returning the details of the best solution.
+solution, solution_fitness, solution_idx = ga_instance.best_solution()
+print("Parameters of the best solution : {solution}".format(solution=solution))
+print("Fitness value of the best solution = {solution_fitness}".format(solution_fitness=solution_fitness))
+print("Index of the best solution : {solution_idx}".format(solution_idx=solution_idx))
+
+prediction = numpy.sum(numpy.array(function_inputs)*solution)
+print("Predicted output based on the best solution : {prediction}".format(prediction=prediction))
+
+if ga_instance.best_solution_generation != -1:
+    print("Best fitness value reached after {best_solution_generation} generations.".format(best_solution_generation=ga_instance.best_solution_generation))
+
+# Saving the GA instance.
+filename = 'genetic' # The filename to which the instance is saved. The name is without extension.
+ga_instance.save(filename=filename)
+
+# Loading the saved GA instance.
+loaded_ga_instance = pygad.load(filename=filename)
+loaded_ga_instance.plot_fitness()
+```
+
+# For More Information
+
+There are different resources that can be used to get started with the genetic algorithm and building it in Python. 
+
+## Tutorial: Implementing Genetic Algorithm in Python
+
+To start with coding the genetic algorithm, you can check the tutorial titled [**Genetic Algorithm Implementation in Python**](https://www.linkedin.com/pulse/genetic-algorithm-implementation-python-ahmed-gad) available at these links:
+
+- [LinkedIn](https://www.linkedin.com/pulse/genetic-algorithm-implementation-python-ahmed-gad)
+- [Towards Data Science](https://towardsdatascience.com/genetic-algorithm-implementation-in-python-5ab67bb124a6)
+- [KDnuggets](https://www.kdnuggets.com/2018/07/genetic-algorithm-implementation-python.html)
+
+[This tutorial](https://www.linkedin.com/pulse/genetic-algorithm-implementation-python-ahmed-gad) is prepared based on a previous version of the project but it still a good resource to start with coding the genetic algorithm.
+
+[![Genetic Algorithm Implementation in Python](https://user-images.githubusercontent.com/16560492/78830052-a3c19300-79e7-11ea-8b9b-4b343ea4049c.png)](https://www.linkedin.com/pulse/genetic-algorithm-implementation-python-ahmed-gad)
+
+## Tutorial: Introduction to Genetic Algorithm
+
+Get started with the genetic algorithm by reading the tutorial titled [**Introduction to Optimization with Genetic Algorithm**](https://www.linkedin.com/pulse/introduction-optimization-genetic-algorithm-ahmed-gad) which is available at these links:
+
+* [LinkedIn](https://www.linkedin.com/pulse/introduction-optimization-genetic-algorithm-ahmed-gad)
+* [Towards Data Science](https://towardsdatascience.com/introduction-to-optimization-with-genetic-algorithm-2f5001d9964b)
+* [KDnuggets](https://www.kdnuggets.com/2018/03/introduction-optimization-with-genetic-algorithm.html)
+
+[![Introduction to Genetic Algorithm](https://user-images.githubusercontent.com/16560492/82078259-26252d00-96e1-11ea-9a02-52a99e1054b9.jpg)](https://www.linkedin.com/pulse/introduction-optimization-genetic-algorithm-ahmed-gad)
+
+## Tutorial: Build Neural Networks in Python
+
+Read about building neural networks in Python through the tutorial titled [**Artificial Neural Network Implementation using NumPy and Classification of the Fruits360 Image Dataset**](https://www.linkedin.com/pulse/artificial-neural-network-implementation-using-numpy-fruits360-gad) available at these links:
+
+* [LinkedIn](https://www.linkedin.com/pulse/artificial-neural-network-implementation-using-numpy-fruits360-gad)
+* [Towards Data Science](https://towardsdatascience.com/artificial-neural-network-implementation-using-numpy-and-classification-of-the-fruits360-image-3c56affa4491)
+* [KDnuggets](https://www.kdnuggets.com/2019/02/artificial-neural-network-implementation-using-numpy-and-image-classification.html)
+
+[![Building Neural Networks Python](https://user-images.githubusercontent.com/16560492/82078281-30472b80-96e1-11ea-8017-6a1f4383d602.jpg)](https://www.linkedin.com/pulse/artificial-neural-network-implementation-using-numpy-fruits360-gad)
+
+## Tutorial: Optimize Neural Networks with Genetic Algorithm
+
+Read about training neural networks using the genetic algorithm through the tutorial titled [**Artificial Neural Networks Optimization using Genetic Algorithm with Python**](https://www.linkedin.com/pulse/artificial-neural-networks-optimization-using-genetic-ahmed-gad) available at these links:
+
+- [LinkedIn](https://www.linkedin.com/pulse/artificial-neural-networks-optimization-using-genetic-ahmed-gad)
+- [Towards Data Science](https://towardsdatascience.com/artificial-neural-networks-optimization-using-genetic-algorithm-with-python-1fe8ed17733e)
+- [KDnuggets](https://www.kdnuggets.com/2019/03/artificial-neural-networks-optimization-genetic-algorithm-python.html)
+
+[![Training Neural Networks using Genetic Algorithm Python](https://user-images.githubusercontent.com/16560492/82078300-376e3980-96e1-11ea-821c-aa6b8ceb44d4.jpg)](https://www.linkedin.com/pulse/artificial-neural-networks-optimization-using-genetic-ahmed-gad)
+
+## Tutorial: Building CNN in Python
+
+To start with coding the genetic algorithm, you can check the tutorial titled [**Building Convolutional Neural Network using NumPy from Scratch**](https://www.linkedin.com/pulse/building-convolutional-neural-network-using-numpy-from-ahmed-gad) available at these links:
+
+- [LinkedIn](https://www.linkedin.com/pulse/building-convolutional-neural-network-using-numpy-from-ahmed-gad)
+- [Towards Data Science](https://towardsdatascience.com/building-convolutional-neural-network-using-numpy-from-scratch-b30aac50e50a)
+- [KDnuggets](https://www.kdnuggets.com/2018/04/building-convolutional-neural-network-numpy-scratch.html)
+- [Chinese Translation](http://m.aliyun.com/yunqi/articles/585741)
+
+[This tutorial](https://www.linkedin.com/pulse/building-convolutional-neural-network-using-numpy-from-ahmed-gad)) is prepared based on a previous version of the project but it still a good resource to start with coding CNNs.
+
+[![Building CNN in Python](https://user-images.githubusercontent.com/16560492/82431022-6c3a1200-9a8e-11ea-8f1b-b055196d76e3.png)](https://www.linkedin.com/pulse/building-convolutional-neural-network-using-numpy-from-ahmed-gad)
+
+## Tutorial: Derivation of CNN from FCNN
+
+Get started with the genetic algorithm by reading the tutorial titled [**Derivation of Convolutional Neural Network from Fully Connected Network Step-By-Step**](https://www.linkedin.com/pulse/derivation-convolutional-neural-network-from-fully-connected-gad) which is available at these links:
+
+* [LinkedIn](https://www.linkedin.com/pulse/derivation-convolutional-neural-network-from-fully-connected-gad)
+* [Towards Data Science](https://towardsdatascience.com/derivation-of-convolutional-neural-network-from-fully-connected-network-step-by-step-b42ebafa5275)
+* [KDnuggets](https://www.kdnuggets.com/2018/04/derivation-convolutional-neural-network-fully-connected-step-by-step.html)
+
+[![Derivation of CNN from FCNN](https://user-images.githubusercontent.com/16560492/82431369-db176b00-9a8e-11ea-99bd-e845192873fc.png)](https://www.linkedin.com/pulse/derivation-convolutional-neural-network-from-fully-connected-gad)
+
+## Book: Practical Computer Vision Applications Using Deep Learning with CNNs
+
+You can also check my book cited as [**Ahmed Fawzy Gad 'Practical Computer Vision Applications Using Deep Learning with CNNs'. Dec. 2018, Apress, 978-1-4842-4167-7**](https://www.amazon.com/Practical-Computer-Vision-Applications-Learning/dp/1484241665) which discusses neural networks, convolutional neural networks, deep learning, genetic algorithm, and more.
+
+Find the book at these links:
+
+- [Amazon](https://www.amazon.com/Practical-Computer-Vision-Applications-Learning/dp/1484241665)
+- [Springer](https://link.springer.com/book/10.1007/978-1-4842-4167-7)
+- [Apress](https://www.apress.com/gp/book/9781484241660)
+- [O'Reilly](https://www.oreilly.com/library/view/practical-computer-vision/9781484241677)
+- [Google Books](https://books.google.com.eg/books?id=xLd9DwAAQBAJ)
+
+![Fig04](https://user-images.githubusercontent.com/16560492/78830077-ae7c2800-79e7-11ea-980b-53b6bd879eeb.jpg)
+
+# Citing PyGAD - Bibtex Formatted Citation
+
+If you used PyGAD, please consider adding a citation to the following paper about PyGAD:
+
+```
+@misc{gad2021pygad,
+      title={PyGAD: An Intuitive Genetic Algorithm Python Library}, 
+      author={Ahmed Fawzy Gad},
+      year={2021},
+      eprint={2106.06158},
+      archivePrefix={arXiv},
+      primaryClass={cs.NE}
+}
+```
+
+# Contact Us
+
+* E-mail: ahmed.f.gad@gmail.com
+* [LinkedIn](https://www.linkedin.com/in/ahmedfgad)
+* [Paperspace](https://blog.paperspace.com/author/ahmed)
+* [KDnuggets](https://kdnuggets.com/author/ahmed-gad)
+* [TowardsDataScience](https://towardsdatascience.com/@ahmedfgad)
+* [GitHub](https://github.com/ahmedfgad)
+
+
```

### Comparing `pygad-2.9.0/setup.py` & `pygad-3.0.0/setup.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 import setuptools  
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(  
     name="pygad",  
-    version="2.9.0",  
+    version="3.0.0",  
     author="Ahmed Fawzy Gad",
-    install_requires=["numpy", "matplotlib",],
+    install_requires=["numpy", "matplotlib","cloudpickle",],
     author_email="ahmed.f.gad@gmail.com",  
-    description="PyGAD: A Python Library for Building the Genetic Algorithm.",
+    description="PyGAD: A Python 3 Library for Building the Genetic Algorithm and Training Machine Learning Algoithms (Keras & PyTorch).",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/ahmedfgad/GeneticAlgorithmPython",
     packages=setuptools.find_packages())
```

