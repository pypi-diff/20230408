# Comparing `tmp/pyabc2-0.1.0.dev1.tar.gz` & `tmp/pyabc2-0.1.0.dev2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyabc2-0.1.0.dev1.tar", last modified: Mon Nov 28 23:15:30 2022, max compression
+gzip compressed data, was "pyabc2-0.1.0.dev2.tar", last modified: Fri Apr  7 22:22:34 2023, max compression
```

## Comparing `pyabc2-0.1.0.dev1.tar` & `pyabc2-0.1.0.dev2.tar`

### file list

```diff
@@ -1,25 +1,26 @@
--rw-r--r--   0        0        0     1318 2022-11-02 16:18:58.748369 pyabc2-0.1.0.dev1/.github/workflows/ci.yml
--rw-r--r--   0        0        0     2010 2022-05-18 21:53:38.068066 pyabc2-0.1.0.dev1/.gitignore
--rw-r--r--   0        0        0      798 2022-11-28 23:13:52.221234 pyabc2-0.1.0.dev1/.pre-commit-config.yaml
--rw-r--r--   0        0        0     1090 2021-09-22 15:45:22.513901 pyabc2-0.1.0.dev1/LICENSE
--rw-r--r--   0        0        0      949 2022-11-02 16:18:58.748869 pyabc2-0.1.0.dev1/README.md
--rw-r--r--   0        0        0     3277 2021-10-11 16:57:49.656486 pyabc2-0.1.0.dev1/examples/modes.ipynb
--rw-r--r--   0        0        0     1706 2022-11-02 16:18:58.749868 pyabc2-0.1.0.dev1/examples/sources.ipynb
--rw-r--r--   0        0        0     2890 2021-10-11 16:57:49.685986 pyabc2-0.1.0.dev1/examples/types.ipynb
--rw-r--r--   0        0        0      308 2022-11-02 16:18:58.750369 pyabc2-0.1.0.dev1/pyabc2/__init__.py
--rw-r--r--   0        0        0      492 2022-11-02 16:18:58.751368 pyabc2-0.1.0.dev1/pyabc2/_util.py
--rw-r--r--   0        0        0    14025 2021-10-11 16:52:58.568553 pyabc2-0.1.0.dev1/pyabc2/key.py
--rw-r--r--   0        0        0     9041 2022-10-18 20:16:16.614418 pyabc2-0.1.0.dev1/pyabc2/note.py
--rw-r--r--   0        0        0    15196 2022-11-02 16:18:58.752368 pyabc2-0.1.0.dev1/pyabc2/parse.py
--rw-r--r--   0        0        0    22903 2022-11-02 16:18:58.753369 pyabc2-0.1.0.dev1/pyabc2/pitch.py
--rw-r--r--   0        0        0        0 2022-11-02 16:18:52.179285 pyabc2-0.1.0.dev1/pyabc2/py.typed
--rw-r--r--   0        0        0     2263 2022-11-02 16:18:58.754368 pyabc2-0.1.0.dev1/pyabc2/sources/__init__.py
--rw-r--r--   0        0        0     8987 2022-11-28 23:13:52.221734 pyabc2-0.1.0.dev1/pyabc2/sources/norbeck.py
--rw-r--r--   0        0        0    11897 2022-11-28 23:13:52.222235 pyabc2-0.1.0.dev1/pyabc2/sources/the_session.py
--rw-r--r--   0        0        0     1341 2022-11-02 16:18:58.756868 pyabc2-0.1.0.dev1/pyproject.toml
--rw-r--r--   0        0        0     3059 2021-10-11 16:52:58.571552 pyabc2-0.1.0.dev1/tests/test_key.py
--rw-r--r--   0        0        0    13914 2022-10-14 19:21:39.307698 pyabc2-0.1.0.dev1/tests/test_note.py
--rw-r--r--   0        0        0     1504 2021-10-11 16:52:58.573052 pyabc2-0.1.0.dev1/tests/test_parse.py
--rw-r--r--   0        0        0      400 2022-11-02 16:18:58.757369 pyabc2-0.1.0.dev1/tests/test_pyabc2.py
--rw-r--r--   0        0        0     7946 2022-11-02 16:18:58.757869 pyabc2-0.1.0.dev1/tests/test_sources.py
--rw-r--r--   0        0        0     1792 1970-01-01 00:00:00.000000 pyabc2-0.1.0.dev1/PKG-INFO
+-rw-r--r--   0        0        0     1302 2023-03-01 18:16:30.028864 pyabc2-0.1.0.dev2/.github/workflows/ci.yml
+-rw-r--r--   0        0        0     2010 2022-05-18 21:53:38.068066 pyabc2-0.1.0.dev2/.gitignore
+-rw-r--r--   0        0        0      795 2023-04-04 20:32:42.460024 pyabc2-0.1.0.dev2/.pre-commit-config.yaml
+-rw-r--r--   0        0        0     1090 2021-09-22 15:45:22.513901 pyabc2-0.1.0.dev2/LICENSE
+-rw-r--r--   0        0        0     1342 2023-04-04 02:35:33.710715 pyabc2-0.1.0.dev2/README.md
+-rw-r--r--   0        0        0      772 2023-04-04 02:35:33.711216 pyabc2-0.1.0.dev2/docs/dev.md
+-rw-r--r--   0        0        0     3436 2023-04-07 22:22:04.269503 pyabc2-0.1.0.dev2/examples/modes.ipynb
+-rw-r--r--   0        0        0     1706 2022-11-02 16:18:58.749868 pyabc2-0.1.0.dev2/examples/sources.ipynb
+-rw-r--r--   0        0        0     2890 2021-10-11 16:57:49.685986 pyabc2-0.1.0.dev2/examples/types.ipynb
+-rw-r--r--   0        0        0      308 2023-04-04 20:34:15.846646 pyabc2-0.1.0.dev2/pyabc2/__init__.py
+-rw-r--r--   0        0        0      492 2022-11-02 16:18:58.751368 pyabc2-0.1.0.dev2/pyabc2/_util.py
+-rw-r--r--   0        0        0    14025 2021-10-11 16:52:58.568553 pyabc2-0.1.0.dev2/pyabc2/key.py
+-rw-r--r--   0        0        0     9039 2023-03-01 17:42:25.473723 pyabc2-0.1.0.dev2/pyabc2/note.py
+-rw-r--r--   0        0        0    15190 2023-03-01 17:42:25.474223 pyabc2-0.1.0.dev2/pyabc2/parse.py
+-rw-r--r--   0        0        0    24532 2023-04-04 20:32:42.460524 pyabc2-0.1.0.dev2/pyabc2/pitch.py
+-rw-r--r--   0        0        0        0 2022-11-02 16:18:52.179285 pyabc2-0.1.0.dev2/pyabc2/py.typed
+-rw-r--r--   0        0        0     2263 2022-11-02 16:18:58.754368 pyabc2-0.1.0.dev2/pyabc2/sources/__init__.py
+-rw-r--r--   0        0        0     8983 2023-03-01 17:42:25.475723 pyabc2-0.1.0.dev2/pyabc2/sources/norbeck.py
+-rw-r--r--   0        0        0    12097 2023-04-04 02:35:33.712217 pyabc2-0.1.0.dev2/pyabc2/sources/the_session.py
+-rw-r--r--   0        0        0     1372 2023-03-01 17:52:00.820390 pyabc2-0.1.0.dev2/pyproject.toml
+-rw-r--r--   0        0        0     3059 2021-10-11 16:52:58.571552 pyabc2-0.1.0.dev2/tests/test_key.py
+-rw-r--r--   0        0        0    15167 2023-04-04 20:32:42.461526 pyabc2-0.1.0.dev2/tests/test_note.py
+-rw-r--r--   0        0        0     1504 2021-10-11 16:52:58.573052 pyabc2-0.1.0.dev2/tests/test_parse.py
+-rw-r--r--   0        0        0      400 2022-11-02 16:18:58.757369 pyabc2-0.1.0.dev2/tests/test_pyabc2.py
+-rw-r--r--   0        0        0     8187 2023-04-04 02:35:33.713217 pyabc2-0.1.0.dev2/tests/test_sources.py
+-rw-r--r--   0        0        0     2173 1970-01-01 00:00:00.000000 pyabc2-0.1.0.dev2/PKG-INFO
```

### Comparing `pyabc2-0.1.0.dev1/.github/workflows/ci.yml` & `pyabc2-0.1.0.dev2/.github/workflows/ci.yml`

 * *Files 8% similar despite different names*

```diff
@@ -17,15 +17,15 @@
       matrix:
         python-version: ["3.8", "3.10"]
 
     steps:
       - uses: actions/checkout@v3
 
       - name: Set up Python ${{ matrix.python-version }}
-        uses: actions/setup-python@v3
+        uses: actions/setup-python@v4
         with:
           python-version: ${{ matrix.python-version }}
 
       - name: Install dependencies
         run: |
           python -m pip install --upgrade pip setuptools wheel
           python -m pip install flit
@@ -33,15 +33,15 @@
 
       - name: Test with pytest
         run: |
           pytest -v --cov=pyabc2 --cov-report xml -n auto
 
       - name: Check type annotations
         run: |
-          mypy --install-types --non-interactive .
+          mypy --non-interactive .
 
       - name: Run the example notebooks
         run: |
           cd examples
           for f in *.ipynb; do
             jupyter nbconvert --to notebook --execute $f
           done
```

### Comparing `pyabc2-0.1.0.dev1/.gitignore` & `pyabc2-0.1.0.dev2/.gitignore`

 * *Files identical despite different names*

### Comparing `pyabc2-0.1.0.dev1/.pre-commit-config.yaml` & `pyabc2-0.1.0.dev2/.pre-commit-config.yaml`

 * *Files 22% similar despite different names*

```diff
@@ -1,32 +1,32 @@
 ci:
   autoupdate_schedule: monthly
 
 repos:
   - repo: https://github.com/pre-commit/pre-commit-hooks
-    rev: 'v4.3.0'
+    rev: 'v4.4.0'
     hooks:
       - id: trailing-whitespace
         args: ['--markdown-linebreak-ext=md,markdown']
       - id: end-of-file-fixer
       - id: check-yaml
 
   - repo: https://github.com/PyCQA/isort
-    rev: '5.10.1'
+    rev: '5.12.0'
     hooks:
       - id: isort
 
   - repo: https://github.com/psf/black
-    rev: '22.10.0'
+    rev: '23.3.0'
     hooks:
       - id: black
         exclude: ^examples/
 
   - repo: https://github.com/csachs/pyproject-flake8
-    rev: 'v5.0.4a1.post1'
+    rev: 'v6.0.0.post1'
     hooks:
       - id: pyproject-flake8  # pflake8
 
   - repo: https://github.com/kynan/nbstripout
     rev: '0.6.1'
     hooks:
       - id: nbstripout
```

### Comparing `pyabc2-0.1.0.dev1/LICENSE` & `pyabc2-0.1.0.dev2/LICENSE`

 * *Files identical despite different names*

### Comparing `pyabc2-0.1.0.dev1/README.md` & `pyabc2-0.1.0.dev2/README.md`

 * *Files 24% similar despite different names*

```diff
@@ -1,11 +1,23 @@
 # PyABC2
 
 [![CI workflow status](https://github.com/zmoon/PyABC2/actions/workflows/ci.yml/badge.svg)](https://github.com/zmoon/PyABC2/actions/workflows/ci.yml)
 [![Test coverage](https://codecov.io/gh/zmoon/PyABC2/branch/main/graph/badge.svg)](https://app.codecov.io/gh/zmoon/PyABC2)
+[![Version on PyPI](https://img.shields.io/pypi/v/pyabc2.svg)](https://pypi.org/project/pyabc2/)
 [![Project Status: WIP – Initial development is in progress, but there has not yet been a stable, usable release suitable for the public.](https://www.repostatus.org/badges/latest/wip.svg)](https://www.repostatus.org/#wip)
 
 ![image](https://user-images.githubusercontent.com/15079414/195207144-83df651a-6fe9-44b1-b7bc-e4aced14a2aa.png)
 
+## Getting started
+
+Install from PyPI:
+```
+pip install pyabc2
+```
+Then look at the [example notebooks](https://github.com/zmoon/PyABC2/tree/main/examples).
+
+To contribute to this project, see the [instructions for developers](https://github.com/zmoon/PyABC2/tree/main/docs/dev.md).
+
+
 ## Credits
 
 Inspired in part by and some portions based on [PyABC](https://github.com/campagnola/pyabc) (`pyabc`; [MIT License](https://github.com/campagnola/pyabc/blob/master/LICENSE.txt)), hence "PyABC2" and the package name `pyabc2`. No relation to [this pyabc](https://github.com/icb-dcm/pyabc) that is on PyPI.
```

### Comparing `pyabc2-0.1.0.dev1/examples/modes.ipynb` & `pyabc2-0.1.0.dev2/examples/types.ipynb`

 * *Files 18% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9666132478632479%*

 * *Differences: {"'cells'": "{0: {'id': 'b495cdee-dae7-407a-8d5b-f58c49c28820', 'source': ['Checking the Jupyter "*

 * *            "reprs.']}, 1: {'id': 'e71a5cd7-bf37-4cc5-9226-831fb66135b0', 'source': {insert: [(1, "*

 * *            "'from pyabc2.sources import load_example_abc')], delete: [1]}}, 2: {'id': "*

 * *            "'8a9bed71-35eb-4d86-9464-b1c8fd4560eb', 'source': ['pyabc2.PitchClass(6)']}, 3: "*

 * *            "{'id': '1f745575-5225-44a9-9f15-2fe4529f3a8b', 'source': ['Fb = "*

 * *            'pyabc2.PitchClass.from_name("Fb")\\n\ […]*

```diff
@@ -1,142 +1,129 @@
 {
     "cells": [
         {
             "cell_type": "markdown",
-            "id": "ae340257-bd4c-47b3-a44e-f6170f150ff9",
+            "id": "b495cdee-dae7-407a-8d5b-f58c49c28820",
             "metadata": {},
             "source": [
-                "Check the modes."
+                "Checking the Jupyter reprs."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "id": "2e7a8668-ac64-4ca7-9cdb-c64bf61f8256",
+            "id": "e71a5cd7-bf37-4cc5-9226-831fb66135b0",
             "metadata": {},
             "outputs": [],
             "source": [
                 "import pyabc2\n",
-                "from pyabc2 import Key"
+                "from pyabc2.sources import load_example_abc"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "id": "3f69d545-7600-40a9-81ce-3dc56973b872",
+            "id": "8a9bed71-35eb-4d86-9464-b1c8fd4560eb",
             "metadata": {},
             "outputs": [],
             "source": [
-                "mode_abbrs = [\"ion\", \"dor\", \"phr\", \"lyd\", \"mix\", \"aeo\", \"loc\"]\n",
-                "\n",
-                "modes = [Key(f\"G{m}\") for m in mode_abbrs]\n",
-                "modes"
-            ]
-        },
-        {
-            "cell_type": "markdown",
-            "id": "aade9c23-b363-4578-bb7e-df2199415225",
-            "metadata": {},
-            "source": [
-                "## Various representations of notes in the scale"
+                "pyabc2.PitchClass(6)"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "id": "6c3491ec-825d-4f7b-80b6-a38fe7103db8",
+            "id": "1f745575-5225-44a9-9f15-2fe4529f3a8b",
             "metadata": {},
             "outputs": [],
             "source": [
-                "for m in modes:\n",
-                "    m.print_scale()"
+                "Fb = pyabc2.PitchClass.from_name(\"Fb\")\n",
+                "Fb"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "id": "b8871068-7ccf-4c29-b9c3-c62d950ba990",
+            "id": "fb60156b-19da-4038-9a4d-1213988c6519",
             "metadata": {},
             "outputs": [],
             "source": [
-                "for m in modes:\n",
-                "    m.print_scale_degrees_wrt_major()"
+                "Fb.equivalent_sharp"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "id": "1c3bfcbb-dd3c-4a81-816f-dff94f0e61c5",
+            "id": "18446868-e0b6-45c2-af05-1656a057afa7",
             "metadata": {},
             "outputs": [],
             "source": [
-                "modes[-1].relative_major"
+                "pyabc2.Pitch(39)"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "id": "f631b8bc-a834-443c-9c61-9190bba58ecb",
+            "id": "47f7a254-1c5b-45c2-832e-d0cae82c0950",
             "metadata": {},
             "outputs": [],
             "source": [
-                "for m in modes:\n",
-                "    m.print_intervals()"
+                "pyabc2.Pitch.from_name(\"Fb4\")"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "id": "c2cde052-a3b7-4b85-ae95-4e8aebe5744e",
+            "id": "28275a7d-6859-4fc4-a872-2cd6aaedda18",
             "metadata": {},
             "outputs": [],
             "source": [
-                "for m in modes:\n",
-                "    m.print_intervals(fmt=\"-\")"
+                "pyabc2.Note.from_abc(\"G2\")"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "id": "5ef8fab6-b4d9-4768-8481-de42379d8eee",
+            "id": "adcacce3-fcb0-4aa6-afef-411ba6de85b4",
             "metadata": {},
             "outputs": [],
             "source": [
-                "for m in modes:\n",
-                "    m.print_scale_chromatic_values()"
+                "pyabc2.Note.from_abc(\"f24\")"
             ]
         },
         {
-            "cell_type": "markdown",
-            "id": "7b75fc1f-2e20-4905-b752-a9bf0e588c5b",
+            "cell_type": "code",
+            "execution_count": null,
+            "id": "018525ce-09d1-4864-adc6-147fef4956a9",
             "metadata": {},
+            "outputs": [],
             "source": [
-                "## Chromatic"
+                "pyabc2.Note.from_abc(\"D,,3/\")"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "id": "7cbfe78a-c672-44e7-ae34-ab307461249a",
+            "id": "daf6debd-69e9-4b51-bbad-0a6d08b24590",
             "metadata": {},
             "outputs": [],
             "source": [
-                "for m in modes:\n",
-                "    m.print_chromatic_scale_degrees()"
+                "abc = load_example_abc(\"For the Love of Music\")\n",
+                "\n",
+                "print(abc)"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "id": "87bf32a7-95e0-4c30-8da8-86181504eabc",
+            "id": "24d338b0-c6ca-4cbe-9a36-62aef6e7a975",
             "metadata": {},
             "outputs": [],
             "source": [
-                "for m in modes:\n",
-                "    m.print_chromatic_scale_degrees(acc_fmt=\"#/b\")"
+                "pyabc2.Tune(abc)"
             ]
         }
     ],
     "metadata": {
         "kernelspec": {
             "display_name": "Python 3 (ipykernel)",
             "language": "python",
```

### Comparing `pyabc2-0.1.0.dev1/examples/sources.ipynb` & `pyabc2-0.1.0.dev2/examples/sources.ipynb`

 * *Files identical despite different names*

### Comparing `pyabc2-0.1.0.dev1/pyabc2/key.py` & `pyabc2-0.1.0.dev2/pyabc2/key.py`

 * *Files identical despite different names*

### Comparing `pyabc2-0.1.0.dev1/pyabc2/note.py` & `pyabc2-0.1.0.dev2/pyabc2/note.py`

 * *Files 0% similar despite different names*

```diff
@@ -56,15 +56,14 @@
 _DEFAULT_UNIT_DURATION = Fraction("1/8")
 
 
 class Note(Pitch):
     """A note has a pitch and a duration."""
 
     def __init__(self, value: int, duration: Fraction = _DEFAULT_UNIT_DURATION):
-
         super().__init__(value)
 
         self.duration = duration
         """Note duration. By default, 1/8, an eighth note."""
 
     def __str__(self):
         return f"{self.name}_{self.duration}"
```

### Comparing `pyabc2-0.1.0.dev1/pyabc2/parse.py` & `pyabc2-0.1.0.dev2/pyabc2/parse.py`

 * *Files 0% similar despite different names*

```diff
@@ -266,15 +266,14 @@
         self.key = Key(h.get("key", "C"))
 
     def _extract_measures(self, tune_lines: List[str]) -> None:
         # 0. Lines
         i_measure = i_measure_repeat = i_ending = 0
         measures = []
         for line in tune_lines:
-
             # Check for chords (not currently supporting)
             # https://abcnotation.com/wiki/abc:standard:v2.1#chords_and_unisons
             # TODO: replace chords by one of the notes?
             first_chord = _find_first_chord(line)
             has_chord = first_chord is not None
             if has_chord:
                 raise ValueError(
@@ -317,21 +316,19 @@
                 # TODO: check for inline meter change; validate measure beat count?
 
                 measure = []
 
                 # 2. In measure, find note groups ("beams")
                 # Currently not doing anything with note group, but may want to in the future
                 for note_group in within_measure.split(" "):
-
                     # TODO: deal with `>` and `<` dotted rhythm modifiers between notes
                     # https://abcnotation.com/wiki/abc:standard:v2.1#broken_rhythm
 
                     # 3. In note group, find notes
                     for m_note in _RE_NOTE.finditer(note_group):
-
                         # TODO: parse/store rests, maybe have an additional iterator for "rhythmic elements" or something
 
                         if m_note is None:
                             raise ValueError(f"no notes in this note group? {note_group!r}")
 
                         measure.append(Note._from_abc_match(m_note, key=self.key))
```

### Comparing `pyabc2-0.1.0.dev1/pyabc2/pitch.py` & `pyabc2-0.1.0.dev2/pyabc2/pitch.py`

 * *Files 5% similar despite different names*

```diff
@@ -54,28 +54,32 @@
 _TRAN_NUM_TO_UNICODE = str.maketrans("0123456789", "₀₁₂₃₄₅₆₇₈₉")
 
 NICE_C_CHROMATIC_NOTES = ["C", "C#", "D", "Eb", "E", "F", "F#", "G", "Ab", "A", "Bb", "B"]
 """ASCII chromatic notes, starting with C at index 0.
 The more common accidentals are used.
 """
 
-_S_RE_PITCH_CLASS = r"[A-G][\#b\=]*"
+_S_RE_ASCII_ACCIDENTALS = r"(?:##|bb|b|#|=)"
+_S_RE_PITCH_CLASS = rf"[A-G]{_S_RE_ASCII_ACCIDENTALS}?"
+_S_RE_LOWER_PITCH_CLASS = rf"[a-g]{_S_RE_ASCII_ACCIDENTALS}?"
 _RE_PITCH_CLASS = re.compile(_S_RE_PITCH_CLASS)
 # _S_RE_PITCH_CLASS_ONE_ACC = r"[A-G][\#|b]?"
 _RE_PITCH = re.compile(rf"(?P<pitch_class>{_S_RE_PITCH_CLASS})" r"\s*" r"(?P<octave>[0-9]+)")
 
 
 def pitch_class_value(pitch: str, root: str = "C", *, mod: bool = False) -> int:
     """Convert a pitch string like 'A#' (note name / pitch class)
     to a chromatic scale value in 0--11 relative to root.
     """
     pitch = pitch.strip()
 
     if not _RE_PITCH_CLASS.fullmatch(pitch):
-        raise ValueError(f"invalid pitch class specification '{pitch}'")
+        raise ValueError(
+            f"invalid pitch class specification '{pitch}'; Should match '{_RE_PITCH_CLASS.pattern}'"
+        )
 
     # Base value
     val = PITCH_VALUES_WRT_C[pitch[0].upper()]
 
     # Add any number of accidentals
     for acc in pitch[1:]:
         val += ACCIDENTAL_DVALUES[acc]
@@ -336,15 +340,17 @@
             raise ValueError("invalid `num_fmt`")
 
         # 2. Adjust accidentals if desired
         acc_fmt_ = acc_fmt.lower()
         if acc_fmt_ == "ascii":
             pass
         elif acc_fmt_ == "unicode":
-            s = re.sub(r"(##|bb|b|#|=)", lambda m: _ACCIDENTAL_ASCII_TO_UNICODE[m.group(0)], s)
+            s = re.sub(
+                _S_RE_ASCII_ACCIDENTALS, lambda m: _ACCIDENTAL_ASCII_TO_UNICODE[m.group(0)], s
+            )
         else:
             raise ValueError("invalid `acc_fmt`")
 
         # TODO: could make a helper fn for the above things to use elsewhere
 
         return s
 
@@ -494,14 +500,44 @@
     def __repr__(self):
         return f"{type(self).__name__}(value={self.value}, name={self.name!r})"
 
     def _repr_html_(self):
         cn = self.to_pitch_class()._repr_html_()
         return f"{cn}<sub>{self.octave}</sub>"
 
+    @property
+    def helmholtz(self) -> str:
+        """Pitch name in Helmholtz pitch notation, e.g. ``C,`` and ``c'`` (ASCII)."""
+        little_c_octave = self.octave - 3
+        if little_c_octave >= 0:
+            return self.class_name.lower() + "'" * little_c_octave
+        big_c_octave = -self.octave + 2
+        return self.class_name + "," * big_c_octave
+
+    @classmethod
+    def from_helmholtz(cls, helmholtz_name: str) -> "Pitch":
+        """From Helmholtz pitch notation.
+
+        https://en.wikipedia.org/wiki/Helmholtz_pitch_notation
+        """
+        helmholtz_name = helmholtz_name.strip()
+        # Single character range so it doesn't fail on empty string.
+        is_upper = helmholtz_name[0:1].isupper()
+        helmoltz_re = (
+            rf"({_S_RE_PITCH_CLASS})(,*)" if is_upper else rf"({_S_RE_LOWER_PITCH_CLASS})('*)"
+        )
+        m = re.fullmatch(helmoltz_re, helmholtz_name)
+        if m is None:
+            raise ValueError(f"invalid Helmholtz pitch name '{helmholtz_name}'")
+        pitch_class_name = m.group(1).title()
+        marks = len(m.group(2))
+        octave = -marks + 2 if is_upper else marks + 3
+
+        return Pitch.from_class_name(pitch_class_name, octave)
+
     def unicode(self):
         """String repr using unicode accidental symbols and unicode subscripts for octave.
 
         .. note::
            ``str(pitch)`` returns an string representation using ASCII accidental symbols
            (``#``, ``b``, ``=``).
         """
@@ -573,14 +609,16 @@
         octave = int(d["octave"])
 
         _validate_pitch_class_name(class_name)
 
         class_value = pitch_class_value(class_name)
 
         p = cls.from_class_value(class_value, octave)
+        # Preserve "non-standard" pitch class name input like Cb,
+        # which also affects the value since the octave is set by the natural note name.
         p._class_name = class_name
         p._octave = octave
 
         return p
 
     @classmethod
     def from_class_value(cls, value: int, octave: int) -> "Pitch":
@@ -686,15 +724,14 @@
 @functools.total_ordering
 class SimpleInterval:
     """An interval that is at most one octave.
     Direction, e.g., in a melodic interval, is not incorporated.
     """
 
     def __init__(self, value: int) -> None:
-
         if 0 <= value <= 12:
             value_ = value
         else:
             abs_value = abs(value)
             mod_abs_value = abs_value % 12
             if mod_abs_value == 0 and abs_value >= 12:
                 value_ = 12
@@ -746,15 +783,14 @@
         return self.value < other.value
 
 
 class SignedInterval(SimpleInterval):
     """An interval that can be more than one octave and with sign (direction) included."""
 
     def __init__(self, value: int) -> None:
-
         self.value = value
         """Number of semitones (half-steps)."""
 
     @property
     def name(self) -> str:
         is_neg = self.value < 0
```

### Comparing `pyabc2-0.1.0.dev1/pyabc2/sources/__init__.py` & `pyabc2-0.1.0.dev2/pyabc2/sources/__init__.py`

 * *Files identical despite different names*

### Comparing `pyabc2-0.1.0.dev1/pyabc2/sources/norbeck.py` & `pyabc2-0.1.0.dev2/pyabc2/sources/norbeck.py`

 * *Files 0% similar despite different names*

```diff
@@ -144,15 +144,14 @@
 
 
 def _load_one_file(fp: Path, *, ascii_only: bool = False) -> List[Tune]:
     """Load one of the Norbeck archive files, which contain multiple tunes."""
 
     blocks = []
     with open(fp, "r") as f:
-
         block = None
         add = False
 
         for line in f:
             if line.startswith("X:"):
                 # Add (if not first X)
                 if block is not None:
@@ -250,15 +249,14 @@
     fps: List[Path]
     if which == ["all"]:
         fps = list(SAVE_TO.glob("*.abc"))
 
     else:
         fps = []
         for tune_type in which:
-
             if tune_type not in _TYPE_PREFIX:
                 raise ValueError(
                     f"tune type {tune_type!r} invalid or not supported. "
                     f"Try one of {set(_TYPE_PREFIX)}."
                 )
 
             fps.extend(_get_paths_type(tune_type))
```

### Comparing `pyabc2-0.1.0.dev1/pyabc2/sources/the_session.py` & `pyabc2-0.1.0.dev2/pyabc2/sources/the_session.py`

 * *Files 2% similar despite different names*

```diff
@@ -281,40 +281,48 @@
             break
     else:  # pragma: no cover
         raise AssertionError("shouldn't reach here")
 
     return ext_typ_str if ext else typ
 
 
+_META_ALLOWED = {"aliases", "events", "recordings", "sessions", "sets", "tune_popularity", "tunes"}
+
+
 def load_meta(
     which: str,
     *,
     convert_dtypes: bool = False,
     downcast_ints: bool = False,
     format: Literal["json", "csv"] = "json",
 ) -> "pandas.DataFrame":
     """Load metadata file from The Session archive as dataframe (requires pandas).
 
+    Parameters
+    ----------
+    which : {'aliases', 'events', 'recordings', 'sessions', 'sets', 'tune_popularity', 'tunes'}
+
+    Notes
+    -----
     In string columns (dtype ``object``), missing value is ``''`` (empty string)
     and is currently left that way by default.
     However, if ``convert_dtypes=True`` is used, this will be set to null,
     and dtypes converted to nullable pandas extension types
     (:meth:`pandas.DataFrame.convert_dtypes` applied).
 
     https://github.com/adactio/TheSession-data/tree/main/json
     https://github.com/adactio/TheSession-data/tree/main/csv
 
     @adactio (Jeremy) is the creator of The Session.
     """
     import numpy as np
     import pandas as pd
 
-    allowed = ["aliases", "events", "recordings", "sessions", "sets", "tune_popularity", "tunes"]
-    if which not in allowed:
-        raise ValueError(f"invalid `which`. Valid choices: {allowed}.")
+    if which not in _META_ALLOWED:
+        raise ValueError(f"invalid `which` {which!r}. Valid choices: {sorted(_META_ALLOWED)}.")
 
     if format not in {"csv", "json"}:
         raise ValueError("`format` must be 'csv' or 'json'.")
 
     base_url = f"https://raw.githubusercontent.com/adactio/TheSession-data/main/{format}/"
     fn = f"{which}.{format}"
     url = base_url + fn
@@ -380,15 +388,15 @@
             df["tune_id"] = df["tune_id"].astype(
                 "Int64"
                 if not downcast_ints
                 else _choose_int_type(df.tune_id.dropna().astype(np.int64), ext=True)
             )
 
         df = df.convert_dtypes()
-        df[cat_cols] = df[cat_cols].astype("category")
+        df[cat_cols] = df[cat_cols].astype(pd.CategoricalDtype())
 
     return df
 
 
 if __name__ == "__main__":  # pragma: no cover
     tune = load_url("https://thesession.org/tunes/10000")
     print(tune)
```

### Comparing `pyabc2-0.1.0.dev1/pyproject.toml` & `pyabc2-0.1.0.dev2/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -55,7 +55,8 @@
 
 [tool.pytest.ini_options]
 markers = ["slow"]
 
 [tool.mypy]
 exclude = ["^venv"]
 install_types = true
+ignore_missing_imports = true
```

### Comparing `pyabc2-0.1.0.dev1/tests/test_key.py` & `pyabc2-0.1.0.dev2/tests/test_key.py`

 * *Files identical despite different names*

### Comparing `pyabc2-0.1.0.dev1/tests/test_note.py` & `pyabc2-0.1.0.dev2/tests/test_note.py`

 * *Files 6% similar despite different names*

```diff
@@ -22,30 +22,28 @@
 
 @pytest.mark.parametrize(
     ("name", "expected_value"),
     [
         ("C", 0),
         ("C#", 1),
         ("Db", 1),
-        ("C###", 3),
         ("Eb", 3),
         ("Fbb", 3),
     ],
 )
 def test_pitch_value(name, expected_value):
     # using default root C
     assert pitch_class_value(name) == expected_value
 
 
 @pytest.mark.parametrize(
     ("name", "expected_value"),
     [
         ("B##", 13),
         ("Cb", -1),
-        ("Dbbb", -1),
     ],
 )
 def test_pitch_value_acc_outside_octave(name, expected_value):
     with pytest.warns(UserWarning, match="computed pitch class value outside 0--11"):
         value = pitch_class_value(name)
     assert value == expected_value
 
@@ -552,7 +550,54 @@
         ("C", ",','", 0),
         ("C", ",,''", 0),
     ],
 )
 def test_abc_doctave_calc(note, oct, expected):
     fn = partial(_octave_from_abc_parts, base=0)
     assert fn(note, oct) == expected
+
+
+@pytest.mark.parametrize(
+    "scientific,helmholtz",
+    [
+        ("C0", "C,,"),
+        ("C1", "C,"),
+        ("C2", "C"),
+        ("C3", "c"),
+        ("C4", "c'"),
+        ("C5", "c''"),
+        ("B3", "b"),
+        ("B#3", "b#"),
+        ("Cb2", "Cb"),
+    ],
+)
+class TestHelmholtz:
+    def test_helmholtz_from_pitch(self, scientific, helmholtz):
+        pitch = Pitch.from_name(scientific)
+        assert pitch.helmholtz == helmholtz
+
+    def test_pitch_from_helmholtz(self, scientific, helmholtz):
+        pitch = Pitch.from_helmholtz(helmholtz)
+        assert pitch.name == scientific
+
+    def test_helmholtz_name_and_octave(self, scientific, helmholtz):
+        from_helmholtz = Pitch.from_helmholtz(helmholtz)
+        from_name = Pitch.from_name(scientific)
+        assert from_helmholtz.name == from_name.name
+        assert from_helmholtz.class_name == from_name.class_name
+        assert from_helmholtz.octave == from_name.octave
+
+
+@pytest.mark.parametrize(
+    "helmholtz",
+    [
+        (""),
+        ("H"),
+        ("C'"),
+        ("c,"),
+        ("bbbb"),
+        ("c###"),
+    ],
+)
+def test_invalid_helmholtz(helmholtz):
+    with pytest.raises(ValueError, match="invalid Helmholtz pitch"):
+        Pitch.from_helmholtz(helmholtz)
```

### Comparing `pyabc2-0.1.0.dev1/tests/test_parse.py` & `pyabc2-0.1.0.dev2/tests/test_parse.py`

 * *Files identical despite different names*

### Comparing `pyabc2-0.1.0.dev1/tests/test_sources.py` & `pyabc2-0.1.0.dev2/tests/test_sources.py`

 * *Files 2% similar despite different names*

```diff
@@ -191,14 +191,20 @@
     with pytest.raises(ValueError):
         _ = the_session.load_meta("asdf")
 
     with pytest.raises(ValueError):
         _ = the_session.load_meta("sessions", format="asdf")
 
 
+def test_the_session_load_meta_doc_consistency():
+    s_options = ", ".join(repr(x) for x in sorted(the_session._META_ALLOWED))
+    expected_line = f"which : {{{s_options}}}"
+    assert expected_line in the_session.load_meta.__doc__
+
+
 def test_int_downcast():
     import numpy as np
     import pandas as pd
 
     for x, expected_dtype, expected_dtype_ext in [
         # short short (8)
         ([int(1e2)], np.uint8, pd.UInt8Dtype()),
```

### Comparing `pyabc2-0.1.0.dev1/PKG-INFO` & `pyabc2-0.1.0.dev2/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyabc2
-Version: 0.1.0.dev1
+Version: 0.1.0.dev2
 Summary: Python ABC notation tools
 Author-email: zmoon <zmoon92@gmail.com>
 Requires-Python: ~=3.8
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: MIT License
 Requires-Dist: ipython ; extra == "dev"
 Requires-Dist: jupyterlab ; extra == "dev"
@@ -22,15 +22,27 @@
 Provides-Extra: sources
 Provides-Extra: test
 
 # PyABC2
 
 [![CI workflow status](https://github.com/zmoon/PyABC2/actions/workflows/ci.yml/badge.svg)](https://github.com/zmoon/PyABC2/actions/workflows/ci.yml)
 [![Test coverage](https://codecov.io/gh/zmoon/PyABC2/branch/main/graph/badge.svg)](https://app.codecov.io/gh/zmoon/PyABC2)
+[![Version on PyPI](https://img.shields.io/pypi/v/pyabc2.svg)](https://pypi.org/project/pyabc2/)
 [![Project Status: WIP – Initial development is in progress, but there has not yet been a stable, usable release suitable for the public.](https://www.repostatus.org/badges/latest/wip.svg)](https://www.repostatus.org/#wip)
 
 ![image](https://user-images.githubusercontent.com/15079414/195207144-83df651a-6fe9-44b1-b7bc-e4aced14a2aa.png)
 
+## Getting started
+
+Install from PyPI:
+```
+pip install pyabc2
+```
+Then look at the [example notebooks](https://github.com/zmoon/PyABC2/tree/main/examples).
+
+To contribute to this project, see the [instructions for developers](https://github.com/zmoon/PyABC2/tree/main/docs/dev.md).
+
+
 ## Credits
 
 Inspired in part by and some portions based on [PyABC](https://github.com/campagnola/pyabc) (`pyabc`; [MIT License](https://github.com/campagnola/pyabc/blob/master/LICENSE.txt)), hence "PyABC2" and the package name `pyabc2`. No relation to [this pyabc](https://github.com/icb-dcm/pyabc) that is on PyPI.
```

