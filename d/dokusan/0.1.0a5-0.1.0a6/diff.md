# Comparing `tmp/dokusan-0.1.0a5.tar.gz` & `tmp/dokusan-0.1.0a6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dokusan-0.1.0a5.tar", last modified: Fri Dec 27 16:35:08 2019, max compression
+gzip compressed data, was "dokusan-0.1.0a6.tar", last modified: Sat Dec 28 23:22:07 2019, max compression
```

## Comparing `dokusan-0.1.0a5.tar` & `dokusan-0.1.0a6.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0    35148 2019-12-27 16:34:51.683904 dokusan-0.1.0a5/LICENSE
--rw-r--r--   0        0        0     3978 2019-12-27 16:34:51.683904 dokusan-0.1.0a5/README.rst
--rw-r--r--   0        0        0      936 2019-12-27 16:34:51.683904 dokusan-0.1.0a5/pyproject.toml
--rw-r--r--   0        0        0        0 2019-12-27 16:34:51.683904 dokusan-0.1.0a5/src/dokusan/__init__.py
--rw-r--r--   0        0        0     5215 2019-12-27 16:34:51.683904 dokusan-0.1.0a5/src/dokusan/entities.py
--rw-r--r--   0        0        0      224 2019-12-27 16:34:51.683904 dokusan-0.1.0a5/src/dokusan/exceptions.py
--rw-r--r--   0        0        0     2437 2019-12-27 16:34:51.683904 dokusan-0.1.0a5/src/dokusan/generators.py
--rw-r--r--   0        0        0     3096 2019-12-27 16:34:51.683904 dokusan-0.1.0a5/src/dokusan/output.py
--rw-r--r--   0        0        0        0 2019-12-27 16:34:51.683904 dokusan-0.1.0a5/src/dokusan/py.typed
--rw-r--r--   0        0        0     2189 2019-12-27 16:34:51.683904 dokusan-0.1.0a5/src/dokusan/solvers.py
--rw-r--r--   0        0        0     1359 2019-12-27 16:34:51.683904 dokusan-0.1.0a5/src/dokusan/stats.py
--rw-r--r--   0        0        0    10782 2019-12-27 16:34:51.683904 dokusan-0.1.0a5/src/dokusan/techniques.py
--rw-r--r--   0        0        0     4752 2019-12-27 16:35:08.965639 dokusan-0.1.0a5/setup.py
--rw-r--r--   0        0        0     4661 2019-12-27 16:35:08.966085 dokusan-0.1.0a5/PKG-INFO
+-rw-r--r--   0        0        0    35148 2019-12-28 23:21:38.333858 dokusan-0.1.0a6/LICENSE
+-rw-r--r--   0        0        0     4094 2019-12-28 23:21:38.333858 dokusan-0.1.0a6/README.rst
+-rw-r--r--   0        0        0      999 2019-12-28 23:21:38.333858 dokusan-0.1.0a6/pyproject.toml
+-rw-r--r--   0        0        0        0 2019-12-28 23:21:38.333858 dokusan-0.1.0a6/src/dokusan/__init__.py
+-rw-r--r--   0        0        0     5215 2019-12-28 23:21:38.333858 dokusan-0.1.0a6/src/dokusan/boards.py
+-rw-r--r--   0        0        0      224 2019-12-28 23:21:38.333858 dokusan-0.1.0a6/src/dokusan/exceptions.py
+-rw-r--r--   0        0        0     2173 2019-12-28 23:21:38.333858 dokusan-0.1.0a6/src/dokusan/generators.py
+-rw-r--r--   0        0        0        0 2019-12-28 23:21:38.333858 dokusan-0.1.0a6/src/dokusan/py.typed
+-rw-r--r--   0        0        0     4111 2019-12-28 23:21:38.333858 dokusan-0.1.0a6/src/dokusan/renderers.py
+-rw-r--r--   0        0        0     2187 2019-12-28 23:21:38.333858 dokusan-0.1.0a6/src/dokusan/solvers.py
+-rw-r--r--   0        0        0     1357 2019-12-28 23:21:38.333858 dokusan-0.1.0a6/src/dokusan/stats.py
+-rw-r--r--   0        0        0    10771 2019-12-28 23:21:38.333858 dokusan-0.1.0a6/src/dokusan/techniques.py
+-rw-r--r--   0        0        0     4870 2019-12-28 23:22:07.467847 dokusan-0.1.0a6/setup.py
+-rw-r--r--   0        0        0     4777 2019-12-28 23:22:07.468437 dokusan-0.1.0a6/PKG-INFO
```

### Comparing `dokusan-0.1.0a5/LICENSE` & `dokusan-0.1.0a6/LICENSE`

 * *Files identical despite different names*

### Comparing `dokusan-0.1.0a5/README.rst` & `dokusan-0.1.0a6/README.rst`

 * *Files 6% similar despite different names*

```diff
@@ -62,15 +62,15 @@
 - Unique Rectangle
 
 For example to see all techniques that sudoku has:
 
 .. code-block:: python
 
     from dokusan import solvers
-    from dokusan.entities import BoxSize, Sudoku
+    from dokusan.boards import BoxSize, Sudoku
 
 
     sudoku = Sudoku.from_list(
         [
             [0, 0, 0, 0, 9, 0, 1, 0, 0],
             [0, 0, 0, 0, 0, 2, 3, 0, 0],
             [0, 0, 7, 0, 0, 1, 8, 2, 5],
@@ -90,16 +90,16 @@
 *************************
 
 This solver is based on backtracking algorithm,
 however slightly modified to work fast
 
 .. code-block:: python
 
-    from dokusan import solvers
-    from dokusan.entities import BoxSize, Sudoku
+    from dokusan import solvers, renderers
+    from dokusan.boards import BoxSize, Sudoku
 
 
     sudoku = Sudoku.from_list(
         [
             [0, 0, 0, 0, 0, 0, 0, 0, 0],
             [0, 0, 0, 0, 0, 3, 0, 8, 5],
             [0, 0, 1, 0, 2, 0, 0, 0, 0],
@@ -109,31 +109,33 @@
             [5, 0, 0, 0, 0, 0, 0, 7, 3],
             [0, 0, 2, 0, 1, 0, 0, 0, 0],
             [0, 0, 0, 0, 4, 0, 0, 0, 9],
         ],
         box_size=BoxSize(3, 3),
     )
 
-    solvers.backtrack(sudoku)
+    solution = solvers.backtrack(sudoku)
+    print(renderers.colorful(solution))
 
 Sudoku Generator
 ----------------
 
 Generator algorithm is mainly based on
 `article <https://dlbeer.co.nz/articles/sudoku.html>`_ by Daniel Beer.
 The average time to generate Sudoku with rank of 150 is 700ms.
 
 To generate a new sudoku:
 
 .. code-block:: python
 
-    from dokusan import generators
+    from dokusan import generators, renderers
 
 
-    generators.random_sudoku(avg_rank=150)
+    sudoku = generators.random_sudoku(avg_rank=150)
+    print(renderers.colorful(sudoku))
 
 Ranking and Sudoku difficulty
 *****************************
 
 ``avg_rank`` option roughly defines the difficulty of the sudoku.
 Sudoku with rank lower than 100 contains only naked/hidden singles.
 Sudoku with rank greater than 150 contains
```

### Comparing `dokusan-0.1.0a5/pyproject.toml` & `dokusan-0.1.0a6/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "dokusan"
-version = "0.1.0-alpha.5"
+version = "0.1.0-alpha.6"
 description = "Sudoku generator and solver with a step-by-step guidance"
 keywords = ["sudoku", "sudoku-solver", "sudoku-generator", "solver", "generator"]
 readme = "README.rst"
 authors = ["Aleksei Maslakov <lesha.maslakov@gmail.com>"]
 license = "GPL-3.0"
 packages = [
     { include = "dokusan", from = "src" },
@@ -25,11 +25,13 @@
 tox = "^3.14"
 pre-commit = "^1.20"
 
 [tool.isort]
 line_length = 88
 multi_line_output = 3
 include_trailing_comma = true
+known_first_party = ["dokusan"]
+default_section = "THIRDPARTY"
 
 [build-system]
 requires = ["poetry>=0.12"]
 build-backend = "poetry.masonry.api"
```

### Comparing `dokusan-0.1.0a5/src/dokusan/entities.py` & `dokusan-0.1.0a6/src/dokusan/boards.py`

 * *Files identical despite different names*

### Comparing `dokusan-0.1.0a5/src/dokusan/generators.py` & `dokusan-0.1.0a6/src/dokusan/generators.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,55 +1,47 @@
 import random
 from typing import List
 
 from dokusan import exceptions, solvers, stats
-from dokusan.entities import BoxSize, Cell, Position, Sudoku
+from dokusan.boards import BoxSize, Cell, Position, Sudoku
 
 MAX_ITERATIONS = 300
 
 
 def random_sudoku(avg_rank: int = 150, box_size: BoxSize = BoxSize(3, 3)) -> Sudoku:
     sudoku = Sudoku(*_random_initial_cells(box_size), box_size=box_size)
     solution = solvers.backtrack(sudoku)
 
-    best_sudoku = Sudoku(*solution.cells(), box_size=box_size)
-    best_rank = 0
-
     iterations = min(avg_rank, MAX_ITERATIONS)
     for i in range(iterations):
         size = random.randint(1, 2)
         rows = [random.randint(0, solution.size - 1) for _ in range(size)]
         columns = [random.randint(0, solution.size - 1) for _ in range(size)]
         cells = [solution[row, column] for (row, column) in zip(rows, columns)]
         if all(cell.value for cell in cells):
             solution.update([Cell(position=cell.position) for cell in cells])
             try:
-                rank = stats.rank(solution)
+                stats.rank(solution)
             except exceptions.MultipleSolutions:
                 solution.update(cells)
-                continue
-            if rank > best_rank:
-                best_sudoku = Sudoku(*solution.cells(), box_size=box_size)
-                best_rank = rank
-                continue
 
-    return best_sudoku
+    return solution
 
 
 def _random_initial_cells(box_size: BoxSize) -> List[Cell]:
     size = box_size.width * box_size.length
     all_values = set(range(1, size + 1))
 
     values = random.sample(all_values, k=size)
     box_values = [
         values[i * box_size.length : i * box_size.length + box_size.length]
         for i in range(box_size.width)
     ]
 
-    while True:
+    while True:  # pragma: no branch
         row_values = random.sample(all_values - set(box_values[0]), k=box_size.length)
         used_values = [sorted(box_values[i]) for i in range(1, box_size.width)]
         if sorted(row_values) not in used_values:
             break
 
     row_values += random.sample(
         all_values.difference(box_values[0], row_values), k=box_size.length
```

### Comparing `dokusan-0.1.0a5/src/dokusan/solvers.py` & `dokusan-0.1.0a6/src/dokusan/solvers.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import operator
 from typing import Iterator
 
 from dokusan import exceptions, techniques
-from dokusan.entities import Cell, Sudoku
+from dokusan.boards import Cell, Sudoku
 from dokusan.techniques import Step
 
 
 def eliminate(sudoku: Sudoku) -> Sudoku:
     _sudoku = Sudoku(*sudoku.cells(), box_size=sudoku.box_size)
 
     all_techniques = (
```

### Comparing `dokusan-0.1.0a5/src/dokusan/stats.py` & `dokusan-0.1.0a6/src/dokusan/stats.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import operator
 
 from dokusan import exceptions, solvers
-from dokusan.entities import Cell, Sudoku
+from dokusan.boards import Cell, Sudoku
 
 
 def rank(sudoku: Sudoku) -> int:
     total_solutions = 0
     total_branch_factor = 0
 
     def count(sudoku: Sudoku) -> None:
```

### Comparing `dokusan-0.1.0a5/src/dokusan/techniques.py` & `dokusan-0.1.0a6/src/dokusan/techniques.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 import itertools
 import operator
 from collections import Counter
 from dataclasses import dataclass
 from typing import Dict, Iterable, Iterator, List, Optional, Set, Tuple
 
-from dokusan.entities import Cell, Sudoku
+from dokusan.boards import Cell, Sudoku
 
 
 class NotFound(Exception):
     pass
 
 
 @dataclass
@@ -272,12 +272,13 @@
         if len(rectangle) != 4:
             return None
         if len(set.intersection(*[m.candidates for m in rectangle])) != 2:
             return None
         return rectangle
 
     def _get_changes(self, combination: Combination) -> List[Cell]:
-        return next(
-            [Cell(position=edge_a.position, candidates=diff)]
-            for edge_a, edge_b in itertools.combinations(combination.cells, 2)
-            if (diff := edge_a.candidates - edge_b.candidates)
-        )
+        eliminated = set(combination.values)
+        return [
+            Cell(position=cell.position, candidates=diff)
+            for cell in combination.cells
+            if (diff := cell.candidates - eliminated)
+        ]
```

### Comparing `dokusan-0.1.0a5/setup.py` & `dokusan-0.1.0a6/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -8,17 +8,17 @@
 ['dokusan']
 
 package_data = \
 {'': ['*']}
 
 setup_kwargs = {
     'name': 'dokusan',
-    'version': '0.1.0a5',
+    'version': '0.1.0a6',
     'description': 'Sudoku generator and solver with a step-by-step guidance',
-    'long_description': '========\nOverview\n========\n\n.. start-badges\n\n.. image:: https://github.com/unmade/dokusan/workflows/Lint%20and%20tests/badge.svg\n    :alt: Build Status\n    :target: https://github.com/unmade/dokusan/blob/master/.github/workflows/lint-and-tests.yml\n\n.. image:: https://codecov.io/gh/unmade/dokusan/branch/master/graph/badge.svg\n    :alt: Coverage Status\n    :target: https://codecov.io/gh/unmade/dokusan\n\n.. image:: http://www.mypy-lang.org/static/mypy_badge.svg\n    :alt: Checked with mypy\n    :target: http://mypy-lang.org/\n\n.. image:: https://img.shields.io/pypi/v/dokusan.svg\n    :alt: PyPI Package latest release\n    :target: https://pypi.org/project/dokusan\n\n.. image:: https://img.shields.io/pypi/wheel/dokusan.svg\n    :alt: PyPI Wheel\n    :target: https://pypi.org/project/dokusan\n\n.. image:: https://img.shields.io/pypi/pyversions/dokusan.svg\n    :alt: Supported versions\n    :target: https://pypi.org/project/dokusan\n\n.. image:: https://img.shields.io/badge/License-GPLv3-purple.svg\n    :alt: GPLv3 License\n    :target: https://github.com/unmade/dokusan/blob/master/LICENSE\n\n.. end-badges\n\nSudoku generator and solver with a step-by-step guidance\n\nInstallation\n============\n\n.. code-block:: bash\n\n    pip install dokusan\n\nQuickstart\n==========\n\nSudoku Solvers\n--------------\n\nStep-by-step solver\n*******************\n\nThis solver tries to solve sudoku using human-like strategies.\nCurrently following techniques are supported:\n\n- Naked/Hidden singles\n- Naked Pairs/Triplets\n- Locked Candidate\n- XY-Wing\n- Unique Rectangle\n\nFor example to see all techniques that sudoku has:\n\n.. code-block:: python\n\n    from dokusan import solvers\n    from dokusan.entities import BoxSize, Sudoku\n\n\n    sudoku = Sudoku.from_list(\n        [\n            [0, 0, 0, 0, 9, 0, 1, 0, 0],\n            [0, 0, 0, 0, 0, 2, 3, 0, 0],\n            [0, 0, 7, 0, 0, 1, 8, 2, 5],\n            [6, 0, 4, 0, 3, 8, 9, 0, 0],\n            [8, 1, 0, 0, 0, 0, 0, 0, 0],\n            [0, 0, 9, 0, 0, 0, 0, 0, 8],\n            [1, 7, 0, 0, 0, 0, 6, 0, 0],\n            [9, 0, 0, 0, 1, 0, 7, 4, 3],\n            [4, 0, 3, 0, 6, 0, 0, 0, 1],\n        ],\n        box_size=BoxSize(3, 3),\n    )\n\n    {step.combination.name for step in solvers.steps(sudoku)}\n\nBacktracking-based solver\n*************************\n\nThis solver is based on backtracking algorithm,\nhowever slightly modified to work fast\n\n.. code-block:: python\n\n    from dokusan import solvers\n    from dokusan.entities import BoxSize, Sudoku\n\n\n    sudoku = Sudoku.from_list(\n        [\n            [0, 0, 0, 0, 0, 0, 0, 0, 0],\n            [0, 0, 0, 0, 0, 3, 0, 8, 5],\n            [0, 0, 1, 0, 2, 0, 0, 0, 0],\n            [0, 0, 0, 5, 0, 7, 0, 0, 0],\n            [0, 0, 4, 0, 0, 0, 1, 0, 0],\n            [0, 9, 0, 0, 0, 0, 0, 0, 0],\n            [5, 0, 0, 0, 0, 0, 0, 7, 3],\n            [0, 0, 2, 0, 1, 0, 0, 0, 0],\n            [0, 0, 0, 0, 4, 0, 0, 0, 9],\n        ],\n        box_size=BoxSize(3, 3),\n    )\n\n    solvers.backtrack(sudoku)\n\nSudoku Generator\n----------------\n\nGenerator algorithm is mainly based on\n`article <https://dlbeer.co.nz/articles/sudoku.html>`_ by Daniel Beer.\nThe average time to generate Sudoku with rank of 150 is 700ms.\n\nTo generate a new sudoku:\n\n.. code-block:: python\n\n    from dokusan import generators\n\n\n    generators.random_sudoku(avg_rank=150)\n\nRanking and Sudoku difficulty\n*****************************\n\n``avg_rank`` option roughly defines the difficulty of the sudoku.\nSudoku with rank lower than 100 contains only naked/hidden singles.\nSudoku with rank greater than 150 contains\nNaked Subsets/Locked Candidate/XY Wing/etc...,\nhowever this is not always guaranteed.\n\nFor higher ranks it is also not guaranteed that generated Sudoku rank\nwill be higher than provided ``avg_rank``,\nso to ensure sudoku has desired rank one can do the following:\n\n.. code-block:: python\n\n    from dokusan import generators, stats\n\n\n    avg_rank = 450\n    while stats.rank(sudoku := generators.random_sudoku(avg_rank)) < avg_rank:\n        continue\n',
+    'long_description': '========\nOverview\n========\n\n.. start-badges\n\n.. image:: https://github.com/unmade/dokusan/workflows/Lint%20and%20tests/badge.svg\n    :alt: Build Status\n    :target: https://github.com/unmade/dokusan/blob/master/.github/workflows/lint-and-tests.yml\n\n.. image:: https://codecov.io/gh/unmade/dokusan/branch/master/graph/badge.svg\n    :alt: Coverage Status\n    :target: https://codecov.io/gh/unmade/dokusan\n\n.. image:: http://www.mypy-lang.org/static/mypy_badge.svg\n    :alt: Checked with mypy\n    :target: http://mypy-lang.org/\n\n.. image:: https://img.shields.io/pypi/v/dokusan.svg\n    :alt: PyPI Package latest release\n    :target: https://pypi.org/project/dokusan\n\n.. image:: https://img.shields.io/pypi/wheel/dokusan.svg\n    :alt: PyPI Wheel\n    :target: https://pypi.org/project/dokusan\n\n.. image:: https://img.shields.io/pypi/pyversions/dokusan.svg\n    :alt: Supported versions\n    :target: https://pypi.org/project/dokusan\n\n.. image:: https://img.shields.io/badge/License-GPLv3-purple.svg\n    :alt: GPLv3 License\n    :target: https://github.com/unmade/dokusan/blob/master/LICENSE\n\n.. end-badges\n\nSudoku generator and solver with a step-by-step guidance\n\nInstallation\n============\n\n.. code-block:: bash\n\n    pip install dokusan\n\nQuickstart\n==========\n\nSudoku Solvers\n--------------\n\nStep-by-step solver\n*******************\n\nThis solver tries to solve sudoku using human-like strategies.\nCurrently following techniques are supported:\n\n- Naked/Hidden singles\n- Naked Pairs/Triplets\n- Locked Candidate\n- XY-Wing\n- Unique Rectangle\n\nFor example to see all techniques that sudoku has:\n\n.. code-block:: python\n\n    from dokusan import solvers\n    from dokusan.boards import BoxSize, Sudoku\n\n\n    sudoku = Sudoku.from_list(\n        [\n            [0, 0, 0, 0, 9, 0, 1, 0, 0],\n            [0, 0, 0, 0, 0, 2, 3, 0, 0],\n            [0, 0, 7, 0, 0, 1, 8, 2, 5],\n            [6, 0, 4, 0, 3, 8, 9, 0, 0],\n            [8, 1, 0, 0, 0, 0, 0, 0, 0],\n            [0, 0, 9, 0, 0, 0, 0, 0, 8],\n            [1, 7, 0, 0, 0, 0, 6, 0, 0],\n            [9, 0, 0, 0, 1, 0, 7, 4, 3],\n            [4, 0, 3, 0, 6, 0, 0, 0, 1],\n        ],\n        box_size=BoxSize(3, 3),\n    )\n\n    {step.combination.name for step in solvers.steps(sudoku)}\n\nBacktracking-based solver\n*************************\n\nThis solver is based on backtracking algorithm,\nhowever slightly modified to work fast\n\n.. code-block:: python\n\n    from dokusan import solvers, renderers\n    from dokusan.boards import BoxSize, Sudoku\n\n\n    sudoku = Sudoku.from_list(\n        [\n            [0, 0, 0, 0, 0, 0, 0, 0, 0],\n            [0, 0, 0, 0, 0, 3, 0, 8, 5],\n            [0, 0, 1, 0, 2, 0, 0, 0, 0],\n            [0, 0, 0, 5, 0, 7, 0, 0, 0],\n            [0, 0, 4, 0, 0, 0, 1, 0, 0],\n            [0, 9, 0, 0, 0, 0, 0, 0, 0],\n            [5, 0, 0, 0, 0, 0, 0, 7, 3],\n            [0, 0, 2, 0, 1, 0, 0, 0, 0],\n            [0, 0, 0, 0, 4, 0, 0, 0, 9],\n        ],\n        box_size=BoxSize(3, 3),\n    )\n\n    solution = solvers.backtrack(sudoku)\n    print(renderers.colorful(solution))\n\nSudoku Generator\n----------------\n\nGenerator algorithm is mainly based on\n`article <https://dlbeer.co.nz/articles/sudoku.html>`_ by Daniel Beer.\nThe average time to generate Sudoku with rank of 150 is 700ms.\n\nTo generate a new sudoku:\n\n.. code-block:: python\n\n    from dokusan import generators, renderers\n\n\n    sudoku = generators.random_sudoku(avg_rank=150)\n    print(renderers.colorful(sudoku))\n\nRanking and Sudoku difficulty\n*****************************\n\n``avg_rank`` option roughly defines the difficulty of the sudoku.\nSudoku with rank lower than 100 contains only naked/hidden singles.\nSudoku with rank greater than 150 contains\nNaked Subsets/Locked Candidate/XY Wing/etc...,\nhowever this is not always guaranteed.\n\nFor higher ranks it is also not guaranteed that generated Sudoku rank\nwill be higher than provided ``avg_rank``,\nso to ensure sudoku has desired rank one can do the following:\n\n.. code-block:: python\n\n    from dokusan import generators, stats\n\n\n    avg_rank = 450\n    while stats.rank(sudoku := generators.random_sudoku(avg_rank)) < avg_rank:\n        continue\n',
     'author': 'Aleksei Maslakov',
     'author_email': 'lesha.maslakov@gmail.com',
     'maintainer': None,
     'maintainer_email': None,
     'url': None,
     'package_dir': package_dir,
     'packages': packages,
```

### Comparing `dokusan-0.1.0a5/PKG-INFO` & `dokusan-0.1.0a6/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dokusan
-Version: 0.1.0a5
+Version: 0.1.0a6
 Summary: Sudoku generator and solver with a step-by-step guidance
 License: GPL-3.0
 Keywords: sudoku,sudoku-solver,sudoku-generator,solver,generator
 Author: Aleksei Maslakov
 Author-email: lesha.maslakov@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: Development Status :: 3 - Alpha
@@ -80,15 +80,15 @@
 - Unique Rectangle
 
 For example to see all techniques that sudoku has:
 
 .. code-block:: python
 
     from dokusan import solvers
-    from dokusan.entities import BoxSize, Sudoku
+    from dokusan.boards import BoxSize, Sudoku
 
 
     sudoku = Sudoku.from_list(
         [
             [0, 0, 0, 0, 9, 0, 1, 0, 0],
             [0, 0, 0, 0, 0, 2, 3, 0, 0],
             [0, 0, 7, 0, 0, 1, 8, 2, 5],
@@ -108,16 +108,16 @@
 *************************
 
 This solver is based on backtracking algorithm,
 however slightly modified to work fast
 
 .. code-block:: python
 
-    from dokusan import solvers
-    from dokusan.entities import BoxSize, Sudoku
+    from dokusan import solvers, renderers
+    from dokusan.boards import BoxSize, Sudoku
 
 
     sudoku = Sudoku.from_list(
         [
             [0, 0, 0, 0, 0, 0, 0, 0, 0],
             [0, 0, 0, 0, 0, 3, 0, 8, 5],
             [0, 0, 1, 0, 2, 0, 0, 0, 0],
@@ -127,31 +127,33 @@
             [5, 0, 0, 0, 0, 0, 0, 7, 3],
             [0, 0, 2, 0, 1, 0, 0, 0, 0],
             [0, 0, 0, 0, 4, 0, 0, 0, 9],
         ],
         box_size=BoxSize(3, 3),
     )
 
-    solvers.backtrack(sudoku)
+    solution = solvers.backtrack(sudoku)
+    print(renderers.colorful(solution))
 
 Sudoku Generator
 ----------------
 
 Generator algorithm is mainly based on
 `article <https://dlbeer.co.nz/articles/sudoku.html>`_ by Daniel Beer.
 The average time to generate Sudoku with rank of 150 is 700ms.
 
 To generate a new sudoku:
 
 .. code-block:: python
 
-    from dokusan import generators
+    from dokusan import generators, renderers
 
 
-    generators.random_sudoku(avg_rank=150)
+    sudoku = generators.random_sudoku(avg_rank=150)
+    print(renderers.colorful(sudoku))
 
 Ranking and Sudoku difficulty
 *****************************
 
 ``avg_rank`` option roughly defines the difficulty of the sudoku.
 Sudoku with rank lower than 100 contains only naked/hidden singles.
 Sudoku with rank greater than 150 contains
```

