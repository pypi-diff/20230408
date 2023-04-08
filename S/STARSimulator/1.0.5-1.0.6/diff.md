# Comparing `tmp/STARSimulator-1.0.5.tar.gz` & `tmp/STARSimulator-1.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "STARSimulator-1.0.5.tar", last modified: Sat Apr  8 17:54:58 2023, max compression
+gzip compressed data, was "STARSimulator-1.0.6.tar", last modified: Sat Apr  8 18:13:18 2023, max compression
```

## Comparing `STARSimulator-1.0.5.tar` & `STARSimulator-1.0.6.tar`

### file list

```diff
@@ -1,172 +1,172 @@
-drwxrwxrwx   0        0        0        0 2023-04-08 17:54:58.003538 STARSimulator-1.0.5/
--rw-rw-rw-   0        0        0     1093 2022-11-18 17:38:34.000000 STARSimulator-1.0.5/LICENSE
--rw-rw-rw-   0        0        0     1892 2023-04-08 17:54:58.004529 STARSimulator-1.0.5/PKG-INFO
--rw-rw-rw-   0        0        0     1286 2023-02-22 04:38:55.000000 STARSimulator-1.0.5/README.md
--rw-rw-rw-   0        0        0      153 2023-02-22 04:38:55.000000 STARSimulator-1.0.5/pyproject.toml
--rw-rw-rw-   0        0        0      971 2023-04-08 17:54:58.007522 STARSimulator-1.0.5/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-04-08 17:54:57.615348 STARSimulator-1.0.5/src/
-drwxrwxrwx   0        0        0        0 2023-04-08 17:54:57.660117 STARSimulator-1.0.5/src/STARSimulator.egg-info/
--rw-rw-rw-   0        0        0     1892 2023-04-08 17:54:57.000000 STARSimulator-1.0.5/src/STARSimulator.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     5371 2023-04-08 17:54:57.000000 STARSimulator-1.0.5/src/STARSimulator.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-08 17:54:57.000000 STARSimulator-1.0.5/src/STARSimulator.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       44 2023-04-08 17:54:57.000000 STARSimulator-1.0.5/src/STARSimulator.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       26 2023-04-08 17:54:57.000000 STARSimulator-1.0.5/src/STARSimulator.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2023-04-08 17:54:57.000000 STARSimulator-1.0.5/src/STARSimulator.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-04-08 17:54:57.687362 STARSimulator-1.0.5/src/stars/
--rw-rw-rw-   0        0        0     1093 2022-11-18 17:38:34.000000 STARSimulator-1.0.5/src/stars/LICENSE
--rw-rw-rw-   0        0        0     1089 2023-02-22 04:38:55.000000 STARSimulator-1.0.5/src/stars/README.md
--rw-rw-rw-   0        0        0        0 2022-11-18 17:38:34.000000 STARSimulator-1.0.5/src/stars/__init__.py
--rw-rw-rw-   0        0        0    10613 2023-03-12 00:05:28.000000 STARSimulator-1.0.5/src/stars/constants.py
--rw-rw-rw-   0        0        0     2940 2022-11-18 17:38:34.000000 STARSimulator-1.0.5/src/stars/controller.py
-drwxrwxrwx   0        0        0        0 2023-04-08 17:54:57.702248 STARSimulator-1.0.5/src/stars/gui/
--rw-rw-rw-   0        0        0        0 2022-11-18 17:38:34.000000 STARSimulator-1.0.5/src/stars/gui/__init__.py
--rw-rw-rw-   0        0        0    31471 2023-04-08 02:01:16.000000 STARSimulator-1.0.5/src/stars/gui/mainwindow.py
-drwxrwxrwx   0        0        0        0 2023-04-08 17:54:57.745975 STARSimulator-1.0.5/src/stars/gui/resources/
--rw-rw-rw-   0        0        0        0 2022-11-18 17:38:34.000000 STARSimulator-1.0.5/src/stars/gui/resources/__init__.py
--rw-rw-rw-   0        0        0     9303 2022-11-18 17:38:34.000000 STARSimulator-1.0.5/src/stars/gui/resources/assemble.svg
--rw-rw-rw-   0        0        0     9391 2023-03-12 00:05:28.000000 STARSimulator-1.0.5/src/stars/gui/resources/assemblewhite.svg
--rw-rw-rw-   0        0        0     1237 2022-11-18 17:38:34.000000 STARSimulator-1.0.5/src/stars/gui/resources/backstep.svg
--rw-rw-rw-   0        0        0     1281 2023-03-12 00:05:28.000000 STARSimulator-1.0.5/src/stars/gui/resources/backstepwhite.svg
--rw-rw-rw-   0        0        0     1222 2022-11-18 17:38:34.000000 STARSimulator-1.0.5/src/stars/gui/resources/help.svg
--rw-rw-rw-   0        0        0     1288 2023-03-12 00:05:28.000000 STARSimulator-1.0.5/src/stars/gui/resources/helpwhite.svg
--rw-rw-rw-   0        0        0     1716 2022-11-18 17:38:34.000000 STARSimulator-1.0.5/src/stars/gui/resources/new.svg
--rw-rw-rw-   0        0        0     1716 2023-03-12 00:05:28.000000 STARSimulator-1.0.5/src/stars/gui/resources/newwhite.svg
--rw-rw-rw-   0        0        0     2291 2022-11-18 17:38:34.000000 STARSimulator-1.0.5/src/stars/gui/resources/open.svg
--rw-rw-rw-   0        0        0     2313 2023-03-12 00:05:28.000000 STARSimulator-1.0.5/src/stars/gui/resources/openwhite.svg
--rw-rw-rw-   0        0        0     1322 2022-11-18 17:38:34.000000 STARSimulator-1.0.5/src/stars/gui/resources/pause.svg
--rw-rw-rw-   0        0        0     1388 2023-03-12 00:05:28.000000 STARSimulator-1.0.5/src/stars/gui/resources/pausewhite.svg
--rw-rw-rw-   0        0        0     1361 2022-11-18 17:38:34.000000 STARSimulator-1.0.5/src/stars/gui/resources/save.svg
--rw-rw-rw-   0        0        0     1449 2023-03-12 00:05:28.000000 STARSimulator-1.0.5/src/stars/gui/resources/savewhite.svg
--rw-rw-rw-   0        0        0     1488 2022-11-18 17:38:34.000000 STARSimulator-1.0.5/src/stars/gui/resources/start.svg
--rw-rw-rw-   0        0        0     1532 2023-03-12 00:05:28.000000 STARSimulator-1.0.5/src/stars/gui/resources/startwhite.svg
--rw-rw-rw-   0        0        0     1249 2022-11-18 17:38:34.000000 STARSimulator-1.0.5/src/stars/gui/resources/step.svg
--rw-rw-rw-   0        0        0     1293 2023-03-12 00:05:28.000000 STARSimulator-1.0.5/src/stars/gui/resources/stepwhite.svg
--rw-rw-rw-   0        0        0     2034 2023-02-22 04:38:55.000000 STARSimulator-1.0.5/src/stars/gui/syntaxhighlighter.py
--rw-rw-rw-   0        0        0    14086 2023-03-12 00:05:28.000000 STARSimulator-1.0.5/src/stars/gui/textedit.py
--rw-rw-rw-   0        0        0     7419 2023-02-22 04:38:55.000000 STARSimulator-1.0.5/src/stars/gui/theme.py
--rw-rw-rw-   0        0        0     5391 2023-02-22 04:38:55.000000 STARSimulator-1.0.5/src/stars/gui/vt100.py
--rw-rw-rw-   0        0        0     4529 2023-02-22 04:38:55.000000 STARSimulator-1.0.5/src/stars/gui/widgetfactory.py
-drwxrwxrwx   0        0        0        0 2023-04-08 17:54:57.766754 STARSimulator-1.0.5/src/stars/help/
--rw-rw-rw-   0        0        0        0 2022-11-18 17:38:34.000000 STARSimulator-1.0.5/src/stars/help/__init__.py
--rw-rw-rw-   0        0        0      412 2022-11-18 17:38:34.000000 STARSimulator-1.0.5/src/stars/help/bugs.md
--rw-rw-rw-   0        0        0      961 2022-11-18 17:38:34.000000 STARSimulator-1.0.5/src/stars/help/directives.csv
--rw-rw-rw-   0        0        0     2816 2023-04-04 22:19:32.000000 STARSimulator-1.0.5/src/stars/help/help.py
--rw-rw-rw-   0        0        0    41526 2022-11-18 17:38:34.000000 STARSimulator-1.0.5/src/stars/help/instruction_set (copy).csv
--rw-rw-rw-   0        0        0    43691 2022-11-18 17:38:34.000000 STARSimulator-1.0.5/src/stars/help/instruction_set.csv
--rw-rw-rw-   0        0        0    54317 2022-11-18 17:38:34.000000 STARSimulator-1.0.5/src/stars/help/instructions.csv
--rw-rw-rw-   0        0        0      851 2022-11-18 17:38:34.000000 STARSimulator-1.0.5/src/stars/help/operand.csv
--rw-rw-rw-   0        0        0     3717 2022-11-18 17:38:34.000000 STARSimulator-1.0.5/src/stars/help/syscalls.csv
--rw-rw-rw-   0        0        0     7210 2023-01-27 13:53:33.000000 STARSimulator-1.0.5/src/stars/instruction_constants.py
-drwxrwxrwx   0        0        0        0 2023-04-08 17:54:57.790320 STARSimulator-1.0.5/src/stars/interpreter/
--rw-rw-rw-   0        0        0        0 2022-11-18 17:38:34.000000 STARSimulator-1.0.5/src/stars/interpreter/__init__.py
--rw-rw-rw-   0        0        0     8252 2023-04-05 03:30:04.000000 STARSimulator-1.0.5/src/stars/interpreter/classes.py
--rw-rw-rw-   0        0        0     7566 2023-04-08 17:34:54.000000 STARSimulator-1.0.5/src/stars/interpreter/compiled_tester.py
--rw-rw-rw-   0        0        0    15045 2023-01-27 13:53:33.000000 STARSimulator-1.0.5/src/stars/interpreter/debugger.py
--rw-rw-rw-   0        0        0     2402 2023-01-27 13:53:33.000000 STARSimulator-1.0.5/src/stars/interpreter/exceptions.py
--rw-rw-rw-   0        0        0    29763 2023-01-27 13:53:33.000000 STARSimulator-1.0.5/src/stars/interpreter/instructions.py
--rw-rw-rw-   0        0        0    14726 2023-04-08 02:08:22.000000 STARSimulator-1.0.5/src/stars/interpreter/interpreter.py
--rw-rw-rw-   0        0        0     9607 2023-04-08 00:21:34.000000 STARSimulator-1.0.5/src/stars/interpreter/memory.py
--rw-rw-rw-   0        0        0     4105 2023-01-27 13:53:33.000000 STARSimulator-1.0.5/src/stars/interpreter/registers.py
--rw-rw-rw-   0        0        0    11237 2023-01-27 13:53:33.000000 STARSimulator-1.0.5/src/stars/interpreter/syscalls.py
--rw-rw-rw-   0        0        0     3317 2023-01-27 13:53:33.000000 STARSimulator-1.0.5/src/stars/interpreter/utility.py
--rw-rw-rw-   0        0        0     6458 2022-11-18 17:38:34.000000 STARSimulator-1.0.5/src/stars/lexer.py
--rw-rw-rw-   0        0        0    17977 2023-04-05 00:08:37.000000 STARSimulator-1.0.5/src/stars/mipsParser.py
--rw-rw-rw-   0        0        0     4206 2023-03-12 00:05:28.000000 STARSimulator-1.0.5/src/stars/preferences.json
--rw-rw-rw-   0        0        0     5825 2023-03-29 11:51:24.000000 STARSimulator-1.0.5/src/stars/preprocess.py
--rw-rw-rw-   0        0        0     5318 2023-04-08 02:08:52.000000 STARSimulator-1.0.5/src/stars/sbumips.py
--rw-rw-rw-   0        0        0     3051 2023-01-27 13:53:33.000000 STARSimulator-1.0.5/src/stars/settings.py
-drwxrwxrwx   0        0        0        0 2023-04-08 17:54:57.796331 STARSimulator-1.0.5/src/stars/sly/
--rw-rw-rw-   0        0        0        0 2022-11-18 17:38:34.000000 STARSimulator-1.0.5/src/stars/sly/__init__.py
--rw-rw-rw-   0        0        0    16056 2022-11-18 17:38:34.000000 STARSimulator-1.0.5/src/stars/sly/lex.py
--rw-rw-rw-   0        0        0    81225 2022-11-18 17:38:34.000000 STARSimulator-1.0.5/src/stars/sly/yacc.py
-drwxrwxrwx   0        0        0        0 2023-04-08 17:54:57.800854 STARSimulator-1.0.5/src/stars/tests/
--rw-rw-rw-   0        0        0        0 2022-11-18 17:38:34.000000 STARSimulator-1.0.5/src/stars/tests/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-08 17:54:57.804870 STARSimulator-1.0.5/src/stars/tests/classes/
--rw-rw-rw-   0        0        0        0 2022-11-18 17:38:34.000000 STARSimulator-1.0.5/src/stars/tests/classes/__init__.py
--rw-rw-rw-   0        0        0     9629 2022-11-18 17:38:34.000000 STARSimulator-1.0.5/src/stars/tests/classes/test_classes.py
-drwxrwxrwx   0        0        0        0 2023-04-08 17:54:57.808862 STARSimulator-1.0.5/src/stars/tests/controller/
--rw-rw-rw-   0        0        0        0 2022-11-18 17:38:34.000000 STARSimulator-1.0.5/src/stars/tests/controller/__init__.py
--rw-rw-rw-   0        0        0     5681 2023-02-22 06:28:43.000000 STARSimulator-1.0.5/src/stars/tests/controller/test_controller.py
-drwxrwxrwx   0        0        0        0 2023-04-08 17:54:57.814191 STARSimulator-1.0.5/src/stars/tests/debugger/
--rw-rw-rw-   0        0        0        0 2022-11-18 17:38:34.000000 STARSimulator-1.0.5/src/stars/tests/debugger/__init__.py
--rw-rw-rw-   0        0        0    16044 2022-11-18 17:38:34.000000 STARSimulator-1.0.5/src/stars/tests/debugger/test_debugger.py
--rw-rw-rw-   0        0        0    12173 2022-11-18 17:38:34.000000 STARSimulator-1.0.5/src/stars/tests/debugger/test_debugger_stack.py
-drwxrwxrwx   0        0        0        0 2023-04-08 17:54:57.818194 STARSimulator-1.0.5/src/stars/tests/fileOps/
--rw-rw-rw-   0        0        0        0 2022-11-18 17:38:34.000000 STARSimulator-1.0.5/src/stars/tests/fileOps/__init__.py
--rw-rw-rw-   0        0        0    14838 2022-11-18 17:38:34.000000 STARSimulator-1.0.5/src/stars/tests/fileOps/test_fileOps.py
-drwxrwxrwx   0        0        0        0 2023-04-08 17:54:57.822374 STARSimulator-1.0.5/src/stars/tests/floatInstrs/
--rw-rw-rw-   0        0        0        0 2022-11-18 17:38:34.000000 STARSimulator-1.0.5/src/stars/tests/floatInstrs/__init__.py
--rw-rw-rw-   0        0        0     9051 2022-11-18 17:38:34.000000 STARSimulator-1.0.5/src/stars/tests/floatInstrs/test.py
-drwxrwxrwx   0        0        0        0 2023-04-08 17:54:57.952054 STARSimulator-1.0.5/src/stars/tests/instructions/
--rw-rw-rw-   0        0        0        0 2022-11-18 17:38:34.000000 STARSimulator-1.0.5/src/stars/tests/instructions/__init__.py
--rw-rw-rw-   0        0        0     4113 2022-11-18 17:38:34.000000 STARSimulator-1.0.5/src/stars/tests/instructions/instructions.py
--rw-rw-rw-   0        0        0     1437 2022-11-18 17:38:34.000000 STARSimulator-1.0.5/src/stars/tests/instructions/test_add.py
--rw-rw-rw-   0        0        0      914 2022-11-18 17:38:34.000000 STARSimulator-1.0.5/src/stars/tests/instructions/test_addi.py
--rw-rw-rw-   0        0        0     1068 2022-11-18 17:38:34.000000 STARSimulator-1.0.5/src/stars/tests/instructions/test_addu.py
--rw-rw-rw-   0        0        0      569 2022-11-18 17:38:34.000000 STARSimulator-1.0.5/src/stars/tests/instructions/test_and.py
--rw-rw-rw-   0        0        0      680 2022-11-18 17:38:34.000000 STARSimulator-1.0.5/src/stars/tests/instructions/test_beq.py
--rw-rw-rw-   0        0        0     1095 2022-11-18 17:38:34.000000 STARSimulator-1.0.5/src/stars/tests/instructions/test_bgez.py
--rw-rw-rw-   0        0        0     1361 2022-11-18 17:38:34.000000 STARSimulator-1.0.5/src/stars/tests/instructions/test_bgezal.py
--rw-rw-rw-   0        0        0      633 2022-11-18 17:38:34.000000 STARSimulator-1.0.5/src/stars/tests/instructions/test_bgtz.py
--rw-rw-rw-   0        0        0     1093 2022-11-18 17:38:34.000000 STARSimulator-1.0.5/src/stars/tests/instructions/test_blez.py
--rw-rw-rw-   0        0        0      631 2022-11-18 17:38:34.000000 STARSimulator-1.0.5/src/stars/tests/instructions/test_bltz.py
--rw-rw-rw-   0        0        0      768 2022-11-18 17:38:34.000000 STARSimulator-1.0.5/src/stars/tests/instructions/test_bltzal.py
--rw-rw-rw-   0        0        0      680 2022-11-18 17:38:34.000000 STARSimulator-1.0.5/src/stars/tests/instructions/test_bne.py
--rw-rw-rw-   0        0        0     1203 2022-11-18 17:38:34.000000 STARSimulator-1.0.5/src/stars/tests/instructions/test_clo.py
--rw-rw-rw-   0        0        0     1200 2022-11-18 17:38:34.000000 STARSimulator-1.0.5/src/stars/tests/instructions/test_clz.py
--rw-rw-rw-   0        0        0     2752 2022-11-18 17:38:34.000000 STARSimulator-1.0.5/src/stars/tests/instructions/test_div.py
--rw-rw-rw-   0        0        0      637 2022-11-18 17:38:34.000000 STARSimulator-1.0.5/src/stars/tests/instructions/test_divu.py
--rw-rw-rw-   0        0        0      945 2022-11-18 17:38:34.000000 STARSimulator-1.0.5/src/stars/tests/instructions/test_j.py
--rw-rw-rw-   0        0        0     1129 2022-11-18 17:38:34.000000 STARSimulator-1.0.5/src/stars/tests/instructions/test_jal.py
--rw-rw-rw-   0        0        0      612 2022-11-18 17:38:34.000000 STARSimulator-1.0.5/src/stars/tests/instructions/test_jalr.py
--rw-rw-rw-   0        0        0      438 2022-11-18 17:38:34.000000 STARSimulator-1.0.5/src/stars/tests/instructions/test_jr.py
--rw-rw-rw-   0        0        0     1890 2022-11-18 17:38:34.000000 STARSimulator-1.0.5/src/stars/tests/instructions/test_lb.py
--rw-rw-rw-   0        0        0     1122 2022-11-18 17:38:34.000000 STARSimulator-1.0.5/src/stars/tests/instructions/test_lbu.py
--rw-rw-rw-   0        0        0     2286 2022-11-18 17:38:34.000000 STARSimulator-1.0.5/src/stars/tests/instructions/test_lh.py
--rw-rw-rw-   0        0        0      655 2022-11-18 17:38:34.000000 STARSimulator-1.0.5/src/stars/tests/instructions/test_lhu.py
--rw-rw-rw-   0        0        0     1307 2022-11-18 17:38:34.000000 STARSimulator-1.0.5/src/stars/tests/instructions/test_lui.py
--rw-rw-rw-   0        0        0     1517 2022-11-18 17:38:34.000000 STARSimulator-1.0.5/src/stars/tests/instructions/test_lw.py
--rw-rw-rw-   0        0        0     2062 2022-11-18 17:38:34.000000 STARSimulator-1.0.5/src/stars/tests/instructions/test_lwl.py
--rw-rw-rw-   0        0        0     2066 2022-11-18 17:38:34.000000 STARSimulator-1.0.5/src/stars/tests/instructions/test_lwr.py
--rw-rw-rw-   0        0        0     2046 2022-11-18 17:38:34.000000 STARSimulator-1.0.5/src/stars/tests/instructions/test_mul.py
--rw-rw-rw-   0        0        0     1282 2022-11-18 17:38:34.000000 STARSimulator-1.0.5/src/stars/tests/instructions/test_mult.py
--rw-rw-rw-   0        0        0      800 2022-11-18 17:38:34.000000 STARSimulator-1.0.5/src/stars/tests/instructions/test_multu.py
--rw-rw-rw-   0        0        0      635 2022-11-18 17:38:34.000000 STARSimulator-1.0.5/src/stars/tests/instructions/test_nor.py
--rw-rw-rw-   0        0        0      564 2022-11-18 17:38:34.000000 STARSimulator-1.0.5/src/stars/tests/instructions/test_or.py
--rw-rw-rw-   0        0        0     1996 2022-11-18 17:38:34.000000 STARSimulator-1.0.5/src/stars/tests/instructions/test_sb.py
--rw-rw-rw-   0        0        0     1170 2022-11-18 17:38:34.000000 STARSimulator-1.0.5/src/stars/tests/instructions/test_sh.py
--rw-rw-rw-   0        0        0      960 2022-11-18 17:38:34.000000 STARSimulator-1.0.5/src/stars/tests/instructions/test_sll.py
--rw-rw-rw-   0        0        0      707 2022-11-18 17:38:34.000000 STARSimulator-1.0.5/src/stars/tests/instructions/test_sllv.py
--rw-rw-rw-   0        0        0     1086 2022-11-18 17:38:34.000000 STARSimulator-1.0.5/src/stars/tests/instructions/test_slt.py
--rw-rw-rw-   0        0        0      595 2022-11-18 17:38:34.000000 STARSimulator-1.0.5/src/stars/tests/instructions/test_slti.py
--rw-rw-rw-   0        0        0      543 2022-11-18 17:38:34.000000 STARSimulator-1.0.5/src/stars/tests/instructions/test_sltiu.py
--rw-rw-rw-   0        0        0     1715 2022-11-18 17:38:34.000000 STARSimulator-1.0.5/src/stars/tests/instructions/test_sltu.py
--rw-rw-rw-   0        0        0      644 2022-11-18 17:38:34.000000 STARSimulator-1.0.5/src/stars/tests/instructions/test_sra.py
--rw-rw-rw-   0        0        0     1226 2022-11-18 17:38:34.000000 STARSimulator-1.0.5/src/stars/tests/instructions/test_srav.py
--rw-rw-rw-   0        0        0      982 2022-11-18 17:38:34.000000 STARSimulator-1.0.5/src/stars/tests/instructions/test_srl.py
--rw-rw-rw-   0        0        0     1518 2022-11-18 17:38:34.000000 STARSimulator-1.0.5/src/stars/tests/instructions/test_srlv.py
--rw-rw-rw-   0        0        0      562 2022-11-18 17:38:34.000000 STARSimulator-1.0.5/src/stars/tests/instructions/test_sub.py
--rw-rw-rw-   0        0        0     1296 2022-11-18 17:38:34.000000 STARSimulator-1.0.5/src/stars/tests/instructions/test_sw.py
--rw-rw-rw-   0        0        0     2813 2022-11-18 17:38:34.000000 STARSimulator-1.0.5/src/stars/tests/instructions/test_swl.py
--rw-rw-rw-   0        0        0     2817 2022-11-18 17:38:34.000000 STARSimulator-1.0.5/src/stars/tests/instructions/test_swr.py
--rw-rw-rw-   0        0        0      568 2022-11-18 17:38:34.000000 STARSimulator-1.0.5/src/stars/tests/instructions/test_xor.py
-drwxrwxrwx   0        0        0        0 2023-04-08 17:54:57.962611 STARSimulator-1.0.5/src/stars/tests/interpreter/
--rw-rw-rw-   0        0        0        0 2022-11-18 17:38:34.000000 STARSimulator-1.0.5/src/stars/tests/interpreter/__init__.py
--rw-rw-rw-   0        0        0     6700 2022-11-18 17:38:34.000000 STARSimulator-1.0.5/src/stars/tests/interpreter/test_interpreter.py
--rw-rw-rw-   0        0        0    13730 2022-11-18 17:38:34.000000 STARSimulator-1.0.5/src/stars/tests/interpreter/test_set_data.py
-drwxrwxrwx   0        0        0        0 2023-04-08 17:54:57.969658 STARSimulator-1.0.5/src/stars/tests/preprocess/
--rw-rw-rw-   0        0        0        0 2022-11-18 17:38:34.000000 STARSimulator-1.0.5/src/stars/tests/preprocess/__init__.py
--rw-rw-rw-   0        0        0     7386 2023-03-29 11:51:24.000000 STARSimulator-1.0.5/src/stars/tests/preprocess/test_preprocess.py
-drwxrwxrwx   0        0        0        0 2023-04-08 17:54:57.973693 STARSimulator-1.0.5/src/stars/tests/pseudoOps/
--rw-rw-rw-   0        0        0        0 2022-11-18 17:38:34.000000 STARSimulator-1.0.5/src/stars/tests/pseudoOps/__init__.py
--rw-rw-rw-   0        0        0     3488 2022-11-18 17:38:34.000000 STARSimulator-1.0.5/src/stars/tests/pseudoOps/test_pseudoOps.py
-drwxrwxrwx   0        0        0        0 2023-04-08 17:54:57.984285 STARSimulator-1.0.5/src/stars/tests/registers/
--rw-rw-rw-   0        0        0        0 2022-11-18 17:38:34.000000 STARSimulator-1.0.5/src/stars/tests/registers/__init__.py
--rw-rw-rw-   0        0        0     7499 2022-11-18 17:38:34.000000 STARSimulator-1.0.5/src/stars/tests/registers/test_registers.py
-drwxrwxrwx   0        0        0        0 2023-04-08 17:54:57.988315 STARSimulator-1.0.5/src/stars/tests/syscalls/
--rw-rw-rw-   0        0        0        0 2022-11-18 17:38:34.000000 STARSimulator-1.0.5/src/stars/tests/syscalls/__init__.py
--rw-rw-rw-   0        0        0    29392 2022-11-18 17:38:34.000000 STARSimulator-1.0.5/src/stars/tests/syscalls/test_syscalls.py
--rw-rw-rw-   0        0        0     4412 2023-03-01 14:04:44.000000 STARSimulator-1.0.5/src/stars/tests/test_sbumips.py
-drwxrwxrwx   0        0        0        0 2023-04-08 17:54:57.997886 STARSimulator-1.0.5/src/stars/tests/validArgs/
--rw-rw-rw-   0        0        0        0 2022-11-18 17:38:34.000000 STARSimulator-1.0.5/src/stars/tests/validArgs/__init__.py
--rw-rw-rw-   0        0        0     7854 2022-11-18 17:38:34.000000 STARSimulator-1.0.5/src/stars/tests/validArgs/test_parse_args.py
+drwxrwxrwx   0        0        0        0 2023-04-08 18:13:18.046726 STARSimulator-1.0.6/
+-rw-rw-rw-   0        0        0     1093 2022-11-18 17:38:34.000000 STARSimulator-1.0.6/LICENSE
+-rw-rw-rw-   0        0        0     1892 2023-04-08 18:13:18.046726 STARSimulator-1.0.6/PKG-INFO
+-rw-rw-rw-   0        0        0     1286 2023-02-22 04:38:55.000000 STARSimulator-1.0.6/README.md
+-rw-rw-rw-   0        0        0      153 2023-02-22 04:38:55.000000 STARSimulator-1.0.6/pyproject.toml
+-rw-rw-rw-   0        0        0      971 2023-04-08 18:13:18.048721 STARSimulator-1.0.6/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-04-08 18:13:17.720228 STARSimulator-1.0.6/src/
+drwxrwxrwx   0        0        0        0 2023-04-08 18:13:17.763102 STARSimulator-1.0.6/src/STARSimulator.egg-info/
+-rw-rw-rw-   0        0        0     1892 2023-04-08 18:13:17.000000 STARSimulator-1.0.6/src/STARSimulator.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     5371 2023-04-08 18:13:17.000000 STARSimulator-1.0.6/src/STARSimulator.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-08 18:13:17.000000 STARSimulator-1.0.6/src/STARSimulator.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       44 2023-04-08 18:13:17.000000 STARSimulator-1.0.6/src/STARSimulator.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       26 2023-04-08 18:13:17.000000 STARSimulator-1.0.6/src/STARSimulator.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2023-04-08 18:13:17.000000 STARSimulator-1.0.6/src/STARSimulator.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-08 18:13:17.792659 STARSimulator-1.0.6/src/stars/
+-rw-rw-rw-   0        0        0     1093 2022-11-18 17:38:34.000000 STARSimulator-1.0.6/src/stars/LICENSE
+-rw-rw-rw-   0        0        0     1089 2023-02-22 04:38:55.000000 STARSimulator-1.0.6/src/stars/README.md
+-rw-rw-rw-   0        0        0        0 2022-11-18 17:38:34.000000 STARSimulator-1.0.6/src/stars/__init__.py
+-rw-rw-rw-   0        0        0    10613 2023-03-12 00:05:28.000000 STARSimulator-1.0.6/src/stars/constants.py
+-rw-rw-rw-   0        0        0     2940 2022-11-18 17:38:34.000000 STARSimulator-1.0.6/src/stars/controller.py
+drwxrwxrwx   0        0        0        0 2023-04-08 18:13:17.807664 STARSimulator-1.0.6/src/stars/gui/
+-rw-rw-rw-   0        0        0        0 2022-11-18 17:38:34.000000 STARSimulator-1.0.6/src/stars/gui/__init__.py
+-rw-rw-rw-   0        0        0    31471 2023-04-08 02:01:16.000000 STARSimulator-1.0.6/src/stars/gui/mainwindow.py
+drwxrwxrwx   0        0        0        0 2023-04-08 18:13:17.845659 STARSimulator-1.0.6/src/stars/gui/resources/
+-rw-rw-rw-   0        0        0        0 2022-11-18 17:38:34.000000 STARSimulator-1.0.6/src/stars/gui/resources/__init__.py
+-rw-rw-rw-   0        0        0     9303 2022-11-18 17:38:34.000000 STARSimulator-1.0.6/src/stars/gui/resources/assemble.svg
+-rw-rw-rw-   0        0        0     9391 2023-03-12 00:05:28.000000 STARSimulator-1.0.6/src/stars/gui/resources/assemblewhite.svg
+-rw-rw-rw-   0        0        0     1237 2022-11-18 17:38:34.000000 STARSimulator-1.0.6/src/stars/gui/resources/backstep.svg
+-rw-rw-rw-   0        0        0     1281 2023-03-12 00:05:28.000000 STARSimulator-1.0.6/src/stars/gui/resources/backstepwhite.svg
+-rw-rw-rw-   0        0        0     1222 2022-11-18 17:38:34.000000 STARSimulator-1.0.6/src/stars/gui/resources/help.svg
+-rw-rw-rw-   0        0        0     1288 2023-03-12 00:05:28.000000 STARSimulator-1.0.6/src/stars/gui/resources/helpwhite.svg
+-rw-rw-rw-   0        0        0     1716 2022-11-18 17:38:34.000000 STARSimulator-1.0.6/src/stars/gui/resources/new.svg
+-rw-rw-rw-   0        0        0     1716 2023-03-12 00:05:28.000000 STARSimulator-1.0.6/src/stars/gui/resources/newwhite.svg
+-rw-rw-rw-   0        0        0     2291 2022-11-18 17:38:34.000000 STARSimulator-1.0.6/src/stars/gui/resources/open.svg
+-rw-rw-rw-   0        0        0     2313 2023-03-12 00:05:28.000000 STARSimulator-1.0.6/src/stars/gui/resources/openwhite.svg
+-rw-rw-rw-   0        0        0     1322 2022-11-18 17:38:34.000000 STARSimulator-1.0.6/src/stars/gui/resources/pause.svg
+-rw-rw-rw-   0        0        0     1388 2023-03-12 00:05:28.000000 STARSimulator-1.0.6/src/stars/gui/resources/pausewhite.svg
+-rw-rw-rw-   0        0        0     1361 2022-11-18 17:38:34.000000 STARSimulator-1.0.6/src/stars/gui/resources/save.svg
+-rw-rw-rw-   0        0        0     1449 2023-03-12 00:05:28.000000 STARSimulator-1.0.6/src/stars/gui/resources/savewhite.svg
+-rw-rw-rw-   0        0        0     1488 2022-11-18 17:38:34.000000 STARSimulator-1.0.6/src/stars/gui/resources/start.svg
+-rw-rw-rw-   0        0        0     1532 2023-03-12 00:05:28.000000 STARSimulator-1.0.6/src/stars/gui/resources/startwhite.svg
+-rw-rw-rw-   0        0        0     1249 2022-11-18 17:38:34.000000 STARSimulator-1.0.6/src/stars/gui/resources/step.svg
+-rw-rw-rw-   0        0        0     1293 2023-03-12 00:05:28.000000 STARSimulator-1.0.6/src/stars/gui/resources/stepwhite.svg
+-rw-rw-rw-   0        0        0     2034 2023-02-22 04:38:55.000000 STARSimulator-1.0.6/src/stars/gui/syntaxhighlighter.py
+-rw-rw-rw-   0        0        0    14086 2023-03-12 00:05:28.000000 STARSimulator-1.0.6/src/stars/gui/textedit.py
+-rw-rw-rw-   0        0        0     7419 2023-02-22 04:38:55.000000 STARSimulator-1.0.6/src/stars/gui/theme.py
+-rw-rw-rw-   0        0        0     5391 2023-02-22 04:38:55.000000 STARSimulator-1.0.6/src/stars/gui/vt100.py
+-rw-rw-rw-   0        0        0     4529 2023-02-22 04:38:55.000000 STARSimulator-1.0.6/src/stars/gui/widgetfactory.py
+drwxrwxrwx   0        0        0        0 2023-04-08 18:13:17.864666 STARSimulator-1.0.6/src/stars/help/
+-rw-rw-rw-   0        0        0        0 2022-11-18 17:38:34.000000 STARSimulator-1.0.6/src/stars/help/__init__.py
+-rw-rw-rw-   0        0        0      412 2022-11-18 17:38:34.000000 STARSimulator-1.0.6/src/stars/help/bugs.md
+-rw-rw-rw-   0        0        0      961 2022-11-18 17:38:34.000000 STARSimulator-1.0.6/src/stars/help/directives.csv
+-rw-rw-rw-   0        0        0     2816 2023-04-04 22:19:32.000000 STARSimulator-1.0.6/src/stars/help/help.py
+-rw-rw-rw-   0        0        0    41526 2022-11-18 17:38:34.000000 STARSimulator-1.0.6/src/stars/help/instruction_set (copy).csv
+-rw-rw-rw-   0        0        0    43691 2022-11-18 17:38:34.000000 STARSimulator-1.0.6/src/stars/help/instruction_set.csv
+-rw-rw-rw-   0        0        0    54317 2022-11-18 17:38:34.000000 STARSimulator-1.0.6/src/stars/help/instructions.csv
+-rw-rw-rw-   0        0        0      851 2022-11-18 17:38:34.000000 STARSimulator-1.0.6/src/stars/help/operand.csv
+-rw-rw-rw-   0        0        0     3717 2022-11-18 17:38:34.000000 STARSimulator-1.0.6/src/stars/help/syscalls.csv
+-rw-rw-rw-   0        0        0     7210 2023-01-27 13:53:33.000000 STARSimulator-1.0.6/src/stars/instruction_constants.py
+drwxrwxrwx   0        0        0        0 2023-04-08 18:13:17.885673 STARSimulator-1.0.6/src/stars/interpreter/
+-rw-rw-rw-   0        0        0        0 2022-11-18 17:38:34.000000 STARSimulator-1.0.6/src/stars/interpreter/__init__.py
+-rw-rw-rw-   0        0        0     8252 2023-04-05 03:30:04.000000 STARSimulator-1.0.6/src/stars/interpreter/classes.py
+-rw-rw-rw-   0        0        0     7566 2023-04-08 17:34:54.000000 STARSimulator-1.0.6/src/stars/interpreter/compiled_tester.py
+-rw-rw-rw-   0        0        0    15045 2023-01-27 13:53:33.000000 STARSimulator-1.0.6/src/stars/interpreter/debugger.py
+-rw-rw-rw-   0        0        0     2402 2023-01-27 13:53:33.000000 STARSimulator-1.0.6/src/stars/interpreter/exceptions.py
+-rw-rw-rw-   0        0        0    29763 2023-01-27 13:53:33.000000 STARSimulator-1.0.6/src/stars/interpreter/instructions.py
+-rw-rw-rw-   0        0        0    14726 2023-04-08 02:08:22.000000 STARSimulator-1.0.6/src/stars/interpreter/interpreter.py
+-rw-rw-rw-   0        0        0     9607 2023-04-08 00:21:34.000000 STARSimulator-1.0.6/src/stars/interpreter/memory.py
+-rw-rw-rw-   0        0        0     4105 2023-01-27 13:53:33.000000 STARSimulator-1.0.6/src/stars/interpreter/registers.py
+-rw-rw-rw-   0        0        0    11237 2023-01-27 13:53:33.000000 STARSimulator-1.0.6/src/stars/interpreter/syscalls.py
+-rw-rw-rw-   0        0        0     3317 2023-01-27 13:53:33.000000 STARSimulator-1.0.6/src/stars/interpreter/utility.py
+-rw-rw-rw-   0        0        0     6458 2022-11-18 17:38:34.000000 STARSimulator-1.0.6/src/stars/lexer.py
+-rw-rw-rw-   0        0        0    17977 2023-04-05 00:08:37.000000 STARSimulator-1.0.6/src/stars/mipsParser.py
+-rw-rw-rw-   0        0        0     4206 2023-03-12 00:05:28.000000 STARSimulator-1.0.6/src/stars/preferences.json
+-rw-rw-rw-   0        0        0     5825 2023-03-29 11:51:24.000000 STARSimulator-1.0.6/src/stars/preprocess.py
+-rw-rw-rw-   0        0        0     5322 2023-04-08 18:11:36.000000 STARSimulator-1.0.6/src/stars/sbumips.py
+-rw-rw-rw-   0        0        0     3051 2023-01-27 13:53:33.000000 STARSimulator-1.0.6/src/stars/settings.py
+drwxrwxrwx   0        0        0        0 2023-04-08 18:13:17.891194 STARSimulator-1.0.6/src/stars/sly/
+-rw-rw-rw-   0        0        0        0 2022-11-18 17:38:34.000000 STARSimulator-1.0.6/src/stars/sly/__init__.py
+-rw-rw-rw-   0        0        0    16056 2022-11-18 17:38:34.000000 STARSimulator-1.0.6/src/stars/sly/lex.py
+-rw-rw-rw-   0        0        0    81225 2022-11-18 17:38:34.000000 STARSimulator-1.0.6/src/stars/sly/yacc.py
+drwxrwxrwx   0        0        0        0 2023-04-08 18:13:17.895197 STARSimulator-1.0.6/src/stars/tests/
+-rw-rw-rw-   0        0        0        0 2022-11-18 17:38:34.000000 STARSimulator-1.0.6/src/stars/tests/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-08 18:13:17.900192 STARSimulator-1.0.6/src/stars/tests/classes/
+-rw-rw-rw-   0        0        0        0 2022-11-18 17:38:34.000000 STARSimulator-1.0.6/src/stars/tests/classes/__init__.py
+-rw-rw-rw-   0        0        0     9629 2022-11-18 17:38:34.000000 STARSimulator-1.0.6/src/stars/tests/classes/test_classes.py
+drwxrwxrwx   0        0        0        0 2023-04-08 18:13:17.903194 STARSimulator-1.0.6/src/stars/tests/controller/
+-rw-rw-rw-   0        0        0        0 2022-11-18 17:38:34.000000 STARSimulator-1.0.6/src/stars/tests/controller/__init__.py
+-rw-rw-rw-   0        0        0     5681 2023-02-22 06:28:43.000000 STARSimulator-1.0.6/src/stars/tests/controller/test_controller.py
+drwxrwxrwx   0        0        0        0 2023-04-08 18:13:17.909201 STARSimulator-1.0.6/src/stars/tests/debugger/
+-rw-rw-rw-   0        0        0        0 2022-11-18 17:38:34.000000 STARSimulator-1.0.6/src/stars/tests/debugger/__init__.py
+-rw-rw-rw-   0        0        0    16044 2022-11-18 17:38:34.000000 STARSimulator-1.0.6/src/stars/tests/debugger/test_debugger.py
+-rw-rw-rw-   0        0        0    12173 2022-11-18 17:38:34.000000 STARSimulator-1.0.6/src/stars/tests/debugger/test_debugger_stack.py
+drwxrwxrwx   0        0        0        0 2023-04-08 18:13:17.913201 STARSimulator-1.0.6/src/stars/tests/fileOps/
+-rw-rw-rw-   0        0        0        0 2022-11-18 17:38:34.000000 STARSimulator-1.0.6/src/stars/tests/fileOps/__init__.py
+-rw-rw-rw-   0        0        0    14838 2022-11-18 17:38:34.000000 STARSimulator-1.0.6/src/stars/tests/fileOps/test_fileOps.py
+drwxrwxrwx   0        0        0        0 2023-04-08 18:13:17.917190 STARSimulator-1.0.6/src/stars/tests/floatInstrs/
+-rw-rw-rw-   0        0        0        0 2022-11-18 17:38:34.000000 STARSimulator-1.0.6/src/stars/tests/floatInstrs/__init__.py
+-rw-rw-rw-   0        0        0     9051 2022-11-18 17:38:34.000000 STARSimulator-1.0.6/src/stars/tests/floatInstrs/test.py
+drwxrwxrwx   0        0        0        0 2023-04-08 18:13:18.022721 STARSimulator-1.0.6/src/stars/tests/instructions/
+-rw-rw-rw-   0        0        0        0 2022-11-18 17:38:34.000000 STARSimulator-1.0.6/src/stars/tests/instructions/__init__.py
+-rw-rw-rw-   0        0        0     4113 2022-11-18 17:38:34.000000 STARSimulator-1.0.6/src/stars/tests/instructions/instructions.py
+-rw-rw-rw-   0        0        0     1437 2022-11-18 17:38:34.000000 STARSimulator-1.0.6/src/stars/tests/instructions/test_add.py
+-rw-rw-rw-   0        0        0      914 2022-11-18 17:38:34.000000 STARSimulator-1.0.6/src/stars/tests/instructions/test_addi.py
+-rw-rw-rw-   0        0        0     1068 2022-11-18 17:38:34.000000 STARSimulator-1.0.6/src/stars/tests/instructions/test_addu.py
+-rw-rw-rw-   0        0        0      569 2022-11-18 17:38:34.000000 STARSimulator-1.0.6/src/stars/tests/instructions/test_and.py
+-rw-rw-rw-   0        0        0      680 2022-11-18 17:38:34.000000 STARSimulator-1.0.6/src/stars/tests/instructions/test_beq.py
+-rw-rw-rw-   0        0        0     1095 2022-11-18 17:38:34.000000 STARSimulator-1.0.6/src/stars/tests/instructions/test_bgez.py
+-rw-rw-rw-   0        0        0     1361 2022-11-18 17:38:34.000000 STARSimulator-1.0.6/src/stars/tests/instructions/test_bgezal.py
+-rw-rw-rw-   0        0        0      633 2022-11-18 17:38:34.000000 STARSimulator-1.0.6/src/stars/tests/instructions/test_bgtz.py
+-rw-rw-rw-   0        0        0     1093 2022-11-18 17:38:34.000000 STARSimulator-1.0.6/src/stars/tests/instructions/test_blez.py
+-rw-rw-rw-   0        0        0      631 2022-11-18 17:38:34.000000 STARSimulator-1.0.6/src/stars/tests/instructions/test_bltz.py
+-rw-rw-rw-   0        0        0      768 2022-11-18 17:38:34.000000 STARSimulator-1.0.6/src/stars/tests/instructions/test_bltzal.py
+-rw-rw-rw-   0        0        0      680 2022-11-18 17:38:34.000000 STARSimulator-1.0.6/src/stars/tests/instructions/test_bne.py
+-rw-rw-rw-   0        0        0     1203 2022-11-18 17:38:34.000000 STARSimulator-1.0.6/src/stars/tests/instructions/test_clo.py
+-rw-rw-rw-   0        0        0     1200 2022-11-18 17:38:34.000000 STARSimulator-1.0.6/src/stars/tests/instructions/test_clz.py
+-rw-rw-rw-   0        0        0     2752 2022-11-18 17:38:34.000000 STARSimulator-1.0.6/src/stars/tests/instructions/test_div.py
+-rw-rw-rw-   0        0        0      637 2022-11-18 17:38:34.000000 STARSimulator-1.0.6/src/stars/tests/instructions/test_divu.py
+-rw-rw-rw-   0        0        0      945 2022-11-18 17:38:34.000000 STARSimulator-1.0.6/src/stars/tests/instructions/test_j.py
+-rw-rw-rw-   0        0        0     1129 2022-11-18 17:38:34.000000 STARSimulator-1.0.6/src/stars/tests/instructions/test_jal.py
+-rw-rw-rw-   0        0        0      612 2022-11-18 17:38:34.000000 STARSimulator-1.0.6/src/stars/tests/instructions/test_jalr.py
+-rw-rw-rw-   0        0        0      438 2022-11-18 17:38:34.000000 STARSimulator-1.0.6/src/stars/tests/instructions/test_jr.py
+-rw-rw-rw-   0        0        0     1890 2022-11-18 17:38:34.000000 STARSimulator-1.0.6/src/stars/tests/instructions/test_lb.py
+-rw-rw-rw-   0        0        0     1122 2022-11-18 17:38:34.000000 STARSimulator-1.0.6/src/stars/tests/instructions/test_lbu.py
+-rw-rw-rw-   0        0        0     2286 2022-11-18 17:38:34.000000 STARSimulator-1.0.6/src/stars/tests/instructions/test_lh.py
+-rw-rw-rw-   0        0        0      655 2022-11-18 17:38:34.000000 STARSimulator-1.0.6/src/stars/tests/instructions/test_lhu.py
+-rw-rw-rw-   0        0        0     1307 2022-11-18 17:38:34.000000 STARSimulator-1.0.6/src/stars/tests/instructions/test_lui.py
+-rw-rw-rw-   0        0        0     1517 2022-11-18 17:38:34.000000 STARSimulator-1.0.6/src/stars/tests/instructions/test_lw.py
+-rw-rw-rw-   0        0        0     2062 2022-11-18 17:38:34.000000 STARSimulator-1.0.6/src/stars/tests/instructions/test_lwl.py
+-rw-rw-rw-   0        0        0     2066 2022-11-18 17:38:34.000000 STARSimulator-1.0.6/src/stars/tests/instructions/test_lwr.py
+-rw-rw-rw-   0        0        0     2046 2022-11-18 17:38:34.000000 STARSimulator-1.0.6/src/stars/tests/instructions/test_mul.py
+-rw-rw-rw-   0        0        0     1282 2022-11-18 17:38:34.000000 STARSimulator-1.0.6/src/stars/tests/instructions/test_mult.py
+-rw-rw-rw-   0        0        0      800 2022-11-18 17:38:34.000000 STARSimulator-1.0.6/src/stars/tests/instructions/test_multu.py
+-rw-rw-rw-   0        0        0      635 2022-11-18 17:38:34.000000 STARSimulator-1.0.6/src/stars/tests/instructions/test_nor.py
+-rw-rw-rw-   0        0        0      564 2022-11-18 17:38:34.000000 STARSimulator-1.0.6/src/stars/tests/instructions/test_or.py
+-rw-rw-rw-   0        0        0     1996 2022-11-18 17:38:34.000000 STARSimulator-1.0.6/src/stars/tests/instructions/test_sb.py
+-rw-rw-rw-   0        0        0     1170 2022-11-18 17:38:34.000000 STARSimulator-1.0.6/src/stars/tests/instructions/test_sh.py
+-rw-rw-rw-   0        0        0      960 2022-11-18 17:38:34.000000 STARSimulator-1.0.6/src/stars/tests/instructions/test_sll.py
+-rw-rw-rw-   0        0        0      707 2022-11-18 17:38:34.000000 STARSimulator-1.0.6/src/stars/tests/instructions/test_sllv.py
+-rw-rw-rw-   0        0        0     1086 2022-11-18 17:38:34.000000 STARSimulator-1.0.6/src/stars/tests/instructions/test_slt.py
+-rw-rw-rw-   0        0        0      595 2022-11-18 17:38:34.000000 STARSimulator-1.0.6/src/stars/tests/instructions/test_slti.py
+-rw-rw-rw-   0        0        0      543 2022-11-18 17:38:34.000000 STARSimulator-1.0.6/src/stars/tests/instructions/test_sltiu.py
+-rw-rw-rw-   0        0        0     1715 2022-11-18 17:38:34.000000 STARSimulator-1.0.6/src/stars/tests/instructions/test_sltu.py
+-rw-rw-rw-   0        0        0      644 2022-11-18 17:38:34.000000 STARSimulator-1.0.6/src/stars/tests/instructions/test_sra.py
+-rw-rw-rw-   0        0        0     1226 2022-11-18 17:38:34.000000 STARSimulator-1.0.6/src/stars/tests/instructions/test_srav.py
+-rw-rw-rw-   0        0        0      982 2022-11-18 17:38:34.000000 STARSimulator-1.0.6/src/stars/tests/instructions/test_srl.py
+-rw-rw-rw-   0        0        0     1518 2022-11-18 17:38:34.000000 STARSimulator-1.0.6/src/stars/tests/instructions/test_srlv.py
+-rw-rw-rw-   0        0        0      562 2022-11-18 17:38:34.000000 STARSimulator-1.0.6/src/stars/tests/instructions/test_sub.py
+-rw-rw-rw-   0        0        0     1296 2022-11-18 17:38:34.000000 STARSimulator-1.0.6/src/stars/tests/instructions/test_sw.py
+-rw-rw-rw-   0        0        0     2813 2022-11-18 17:38:34.000000 STARSimulator-1.0.6/src/stars/tests/instructions/test_swl.py
+-rw-rw-rw-   0        0        0     2817 2022-11-18 17:38:34.000000 STARSimulator-1.0.6/src/stars/tests/instructions/test_swr.py
+-rw-rw-rw-   0        0        0      568 2022-11-18 17:38:34.000000 STARSimulator-1.0.6/src/stars/tests/instructions/test_xor.py
+drwxrwxrwx   0        0        0        0 2023-04-08 18:13:18.027723 STARSimulator-1.0.6/src/stars/tests/interpreter/
+-rw-rw-rw-   0        0        0        0 2022-11-18 17:38:34.000000 STARSimulator-1.0.6/src/stars/tests/interpreter/__init__.py
+-rw-rw-rw-   0        0        0     6700 2022-11-18 17:38:34.000000 STARSimulator-1.0.6/src/stars/tests/interpreter/test_interpreter.py
+-rw-rw-rw-   0        0        0    13730 2022-11-18 17:38:34.000000 STARSimulator-1.0.6/src/stars/tests/interpreter/test_set_data.py
+drwxrwxrwx   0        0        0        0 2023-04-08 18:13:18.031728 STARSimulator-1.0.6/src/stars/tests/preprocess/
+-rw-rw-rw-   0        0        0        0 2022-11-18 17:38:34.000000 STARSimulator-1.0.6/src/stars/tests/preprocess/__init__.py
+-rw-rw-rw-   0        0        0     7386 2023-03-29 11:51:24.000000 STARSimulator-1.0.6/src/stars/tests/preprocess/test_preprocess.py
+drwxrwxrwx   0        0        0        0 2023-04-08 18:13:18.034727 STARSimulator-1.0.6/src/stars/tests/pseudoOps/
+-rw-rw-rw-   0        0        0        0 2022-11-18 17:38:34.000000 STARSimulator-1.0.6/src/stars/tests/pseudoOps/__init__.py
+-rw-rw-rw-   0        0        0     3488 2022-11-18 17:38:34.000000 STARSimulator-1.0.6/src/stars/tests/pseudoOps/test_pseudoOps.py
+drwxrwxrwx   0        0        0        0 2023-04-08 18:13:18.038722 STARSimulator-1.0.6/src/stars/tests/registers/
+-rw-rw-rw-   0        0        0        0 2022-11-18 17:38:34.000000 STARSimulator-1.0.6/src/stars/tests/registers/__init__.py
+-rw-rw-rw-   0        0        0     7499 2022-11-18 17:38:34.000000 STARSimulator-1.0.6/src/stars/tests/registers/test_registers.py
+drwxrwxrwx   0        0        0        0 2023-04-08 18:13:18.040723 STARSimulator-1.0.6/src/stars/tests/syscalls/
+-rw-rw-rw-   0        0        0        0 2022-11-18 17:38:34.000000 STARSimulator-1.0.6/src/stars/tests/syscalls/__init__.py
+-rw-rw-rw-   0        0        0    29392 2022-11-18 17:38:34.000000 STARSimulator-1.0.6/src/stars/tests/syscalls/test_syscalls.py
+-rw-rw-rw-   0        0        0     4412 2023-03-01 14:04:44.000000 STARSimulator-1.0.6/src/stars/tests/test_sbumips.py
+drwxrwxrwx   0        0        0        0 2023-04-08 18:13:18.044723 STARSimulator-1.0.6/src/stars/tests/validArgs/
+-rw-rw-rw-   0        0        0        0 2022-11-18 17:38:34.000000 STARSimulator-1.0.6/src/stars/tests/validArgs/__init__.py
+-rw-rw-rw-   0        0        0     7854 2022-11-18 17:38:34.000000 STARSimulator-1.0.6/src/stars/tests/validArgs/test_parse_args.py
```

### Comparing `STARSimulator-1.0.5/LICENSE` & `STARSimulator-1.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `STARSimulator-1.0.5/PKG-INFO` & `STARSimulator-1.0.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: STARSimulator
-Version: 1.0.5
+Version: 1.0.6
 Summary: STARS (Stony Brook Assembler and Run-time Simulator) is a MIPS Assembly simulator made for the purpose of education.
 Home-page: https://github.com/sbustars/STARS
 Author: STARS
 Author-email: jason.osoriomarin@cs.stonybrook.edu
 Project-URL: Bug Tracker, https://github.com/sbustars/STARS/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `STARSimulator-1.0.5/README.md` & `STARSimulator-1.0.6/README.md`

 * *Files identical despite different names*

### Comparing `STARSimulator-1.0.5/setup.cfg` & `STARSimulator-1.0.6/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2053 5441 5253 696d 756c 6174 6f72   = STARSimulator
 00000020: 0d0a 7665 7273 696f 6e20 3d20 312e 302e  ..version = 1.0.
-00000030: 350d 0a61 7574 686f 7220 3d20 5354 4152  5..author = STAR
+00000030: 360d 0a61 7574 686f 7220 3d20 5354 4152  6..author = STAR
 00000040: 530d 0a61 7574 686f 725f 656d 6169 6c20  S..author_email 
 00000050: 3d20 6a61 736f 6e2e 6f73 6f72 696f 6d61  = jason.osorioma
 00000060: 7269 6e40 6373 2e73 746f 6e79 6272 6f6f  rin@cs.stonybroo
 00000070: 6b2e 6564 750d 0a64 6573 6372 6970 7469  k.edu..descripti
 00000080: 6f6e 203d 2053 5441 5253 2028 5374 6f6e  on = STARS (Ston
 00000090: 7920 4272 6f6f 6b20 4173 7365 6d62 6c65  y Brook Assemble
 000000a0: 7220 616e 6420 5275 6e2d 7469 6d65 2053  r and Run-time S
```

### Comparing `STARSimulator-1.0.5/src/STARSimulator.egg-info/PKG-INFO` & `STARSimulator-1.0.6/src/STARSimulator.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: STARSimulator
-Version: 1.0.5
+Version: 1.0.6
 Summary: STARS (Stony Brook Assembler and Run-time Simulator) is a MIPS Assembly simulator made for the purpose of education.
 Home-page: https://github.com/sbustars/STARS
 Author: STARS
 Author-email: jason.osoriomarin@cs.stonybrook.edu
 Project-URL: Bug Tracker, https://github.com/sbustars/STARS/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `STARSimulator-1.0.5/src/STARSimulator.egg-info/SOURCES.txt` & `STARSimulator-1.0.6/src/STARSimulator.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `STARSimulator-1.0.5/src/stars/LICENSE` & `STARSimulator-1.0.6/src/stars/LICENSE`

 * *Files identical despite different names*

### Comparing `STARSimulator-1.0.5/src/stars/README.md` & `STARSimulator-1.0.6/src/stars/README.md`

 * *Files identical despite different names*

### Comparing `STARSimulator-1.0.5/src/stars/constants.py` & `STARSimulator-1.0.6/src/stars/constants.py`

 * *Files identical despite different names*

### Comparing `STARSimulator-1.0.5/src/stars/controller.py` & `STARSimulator-1.0.6/src/stars/controller.py`

 * *Files identical despite different names*

### Comparing `STARSimulator-1.0.5/src/stars/gui/mainwindow.py` & `STARSimulator-1.0.6/src/stars/gui/mainwindow.py`

 * *Files identical despite different names*

### Comparing `STARSimulator-1.0.5/src/stars/gui/resources/assemble.svg` & `STARSimulator-1.0.6/src/stars/gui/resources/assemble.svg`

 * *Files identical despite different names*

### Comparing `STARSimulator-1.0.5/src/stars/gui/resources/assemblewhite.svg` & `STARSimulator-1.0.6/src/stars/gui/resources/assemblewhite.svg`

 * *Files identical despite different names*

### Comparing `STARSimulator-1.0.5/src/stars/gui/resources/backstep.svg` & `STARSimulator-1.0.6/src/stars/gui/resources/backstep.svg`

 * *Files identical despite different names*

### Comparing `STARSimulator-1.0.5/src/stars/gui/resources/backstepwhite.svg` & `STARSimulator-1.0.6/src/stars/gui/resources/backstepwhite.svg`

 * *Files identical despite different names*

### Comparing `STARSimulator-1.0.5/src/stars/gui/resources/help.svg` & `STARSimulator-1.0.6/src/stars/gui/resources/help.svg`

 * *Files identical despite different names*

### Comparing `STARSimulator-1.0.5/src/stars/gui/resources/helpwhite.svg` & `STARSimulator-1.0.6/src/stars/gui/resources/helpwhite.svg`

 * *Files identical despite different names*

### Comparing `STARSimulator-1.0.5/src/stars/gui/resources/new.svg` & `STARSimulator-1.0.6/src/stars/gui/resources/new.svg`

 * *Files identical despite different names*

### Comparing `STARSimulator-1.0.5/src/stars/gui/resources/newwhite.svg` & `STARSimulator-1.0.6/src/stars/gui/resources/newwhite.svg`

 * *Files identical despite different names*

### Comparing `STARSimulator-1.0.5/src/stars/gui/resources/open.svg` & `STARSimulator-1.0.6/src/stars/gui/resources/open.svg`

 * *Files identical despite different names*

### Comparing `STARSimulator-1.0.5/src/stars/gui/resources/openwhite.svg` & `STARSimulator-1.0.6/src/stars/gui/resources/openwhite.svg`

 * *Files identical despite different names*

### Comparing `STARSimulator-1.0.5/src/stars/gui/resources/pause.svg` & `STARSimulator-1.0.6/src/stars/gui/resources/pause.svg`

 * *Files identical despite different names*

### Comparing `STARSimulator-1.0.5/src/stars/gui/resources/pausewhite.svg` & `STARSimulator-1.0.6/src/stars/gui/resources/pausewhite.svg`

 * *Files identical despite different names*

### Comparing `STARSimulator-1.0.5/src/stars/gui/resources/save.svg` & `STARSimulator-1.0.6/src/stars/gui/resources/save.svg`

 * *Files identical despite different names*

### Comparing `STARSimulator-1.0.5/src/stars/gui/resources/savewhite.svg` & `STARSimulator-1.0.6/src/stars/gui/resources/savewhite.svg`

 * *Files identical despite different names*

### Comparing `STARSimulator-1.0.5/src/stars/gui/resources/start.svg` & `STARSimulator-1.0.6/src/stars/gui/resources/start.svg`

 * *Files identical despite different names*

### Comparing `STARSimulator-1.0.5/src/stars/gui/resources/startwhite.svg` & `STARSimulator-1.0.6/src/stars/gui/resources/startwhite.svg`

 * *Files identical despite different names*

### Comparing `STARSimulator-1.0.5/src/stars/gui/resources/step.svg` & `STARSimulator-1.0.6/src/stars/gui/resources/step.svg`

 * *Files identical despite different names*

### Comparing `STARSimulator-1.0.5/src/stars/gui/resources/stepwhite.svg` & `STARSimulator-1.0.6/src/stars/gui/resources/stepwhite.svg`

 * *Files identical despite different names*

### Comparing `STARSimulator-1.0.5/src/stars/gui/syntaxhighlighter.py` & `STARSimulator-1.0.6/src/stars/gui/syntaxhighlighter.py`

 * *Files identical despite different names*

### Comparing `STARSimulator-1.0.5/src/stars/gui/textedit.py` & `STARSimulator-1.0.6/src/stars/gui/textedit.py`

 * *Files identical despite different names*

### Comparing `STARSimulator-1.0.5/src/stars/gui/theme.py` & `STARSimulator-1.0.6/src/stars/gui/theme.py`

 * *Files identical despite different names*

### Comparing `STARSimulator-1.0.5/src/stars/gui/vt100.py` & `STARSimulator-1.0.6/src/stars/gui/vt100.py`

 * *Files identical despite different names*

### Comparing `STARSimulator-1.0.5/src/stars/gui/widgetfactory.py` & `STARSimulator-1.0.6/src/stars/gui/widgetfactory.py`

 * *Files identical despite different names*

### Comparing `STARSimulator-1.0.5/src/stars/help/directives.csv` & `STARSimulator-1.0.6/src/stars/help/directives.csv`

 * *Files identical despite different names*

### Comparing `STARSimulator-1.0.5/src/stars/help/help.py` & `STARSimulator-1.0.6/src/stars/help/help.py`

 * *Files identical despite different names*

### Comparing `STARSimulator-1.0.5/src/stars/help/instruction_set (copy).csv` & `STARSimulator-1.0.6/src/stars/help/instruction_set (copy).csv`

 * *Files identical despite different names*

### Comparing `STARSimulator-1.0.5/src/stars/help/instruction_set.csv` & `STARSimulator-1.0.6/src/stars/help/instruction_set.csv`

 * *Files identical despite different names*

### Comparing `STARSimulator-1.0.5/src/stars/help/instructions.csv` & `STARSimulator-1.0.6/src/stars/help/instructions.csv`

 * *Files identical despite different names*

### Comparing `STARSimulator-1.0.5/src/stars/help/operand.csv` & `STARSimulator-1.0.6/src/stars/help/operand.csv`

 * *Files identical despite different names*

### Comparing `STARSimulator-1.0.5/src/stars/help/syscalls.csv` & `STARSimulator-1.0.6/src/stars/help/syscalls.csv`

 * *Files identical despite different names*

### Comparing `STARSimulator-1.0.5/src/stars/instruction_constants.py` & `STARSimulator-1.0.6/src/stars/instruction_constants.py`

 * *Files identical despite different names*

### Comparing `STARSimulator-1.0.5/src/stars/interpreter/classes.py` & `STARSimulator-1.0.6/src/stars/interpreter/classes.py`

 * *Files identical despite different names*

### Comparing `STARSimulator-1.0.5/src/stars/interpreter/compiled_tester.py` & `STARSimulator-1.0.6/src/stars/interpreter/compiled_tester.py`

 * *Files identical despite different names*

### Comparing `STARSimulator-1.0.5/src/stars/interpreter/debugger.py` & `STARSimulator-1.0.6/src/stars/interpreter/debugger.py`

 * *Files identical despite different names*

### Comparing `STARSimulator-1.0.5/src/stars/interpreter/exceptions.py` & `STARSimulator-1.0.6/src/stars/interpreter/exceptions.py`

 * *Files identical despite different names*

### Comparing `STARSimulator-1.0.5/src/stars/interpreter/instructions.py` & `STARSimulator-1.0.6/src/stars/interpreter/instructions.py`

 * *Files identical despite different names*

### Comparing `STARSimulator-1.0.5/src/stars/interpreter/interpreter.py` & `STARSimulator-1.0.6/src/stars/interpreter/interpreter.py`

 * *Files identical despite different names*

### Comparing `STARSimulator-1.0.5/src/stars/interpreter/memory.py` & `STARSimulator-1.0.6/src/stars/interpreter/memory.py`

 * *Files identical despite different names*

### Comparing `STARSimulator-1.0.5/src/stars/interpreter/registers.py` & `STARSimulator-1.0.6/src/stars/interpreter/registers.py`

 * *Files identical despite different names*

### Comparing `STARSimulator-1.0.5/src/stars/interpreter/syscalls.py` & `STARSimulator-1.0.6/src/stars/interpreter/syscalls.py`

 * *Files identical despite different names*

### Comparing `STARSimulator-1.0.5/src/stars/interpreter/utility.py` & `STARSimulator-1.0.6/src/stars/interpreter/utility.py`

 * *Files identical despite different names*

### Comparing `STARSimulator-1.0.5/src/stars/lexer.py` & `STARSimulator-1.0.6/src/stars/lexer.py`

 * *Files identical despite different names*

### Comparing `STARSimulator-1.0.5/src/stars/mipsParser.py` & `STARSimulator-1.0.6/src/stars/mipsParser.py`

 * *Files identical despite different names*

### Comparing `STARSimulator-1.0.5/src/stars/preferences.json` & `STARSimulator-1.0.6/src/stars/preferences.json`

 * *Files identical despite different names*

### Comparing `STARSimulator-1.0.5/src/stars/preprocess.py` & `STARSimulator-1.0.6/src/stars/preprocess.py`

 * *Files identical despite different names*

### Comparing `STARSimulator-1.0.5/src/stars/sbumips.py` & `STARSimulator-1.0.6/src/stars/sbumips.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,23 @@
+import sys
+import os
+current_path = os.path.dirname(os.path.abspath(__file__))
+sys.path.append(current_path)
+sys.path.append(os.getcwd())
 from pathlib import Path
 import argparse
 from gui import mainwindow
 from interpreter.interpreter import *
 from lexer import MipsLexer
 from mipsParser import MipsParser
 from preprocess import walk, link, preprocess
 from settings import settings
-import sys
-import os
 
-current_path = os.path.dirname(os.path.abspath(__file__))
-sys.path.append(current_path)
-sys.path.append(os.getcwd())
+
+
 
 
 '''
 https://github.com/sbustars/STARS
 
 Copyright 2020 Kevin McDonnell, Jihu Mun, and Ian Peitzsch
```

### Comparing `STARSimulator-1.0.5/src/stars/settings.py` & `STARSimulator-1.0.6/src/stars/settings.py`

 * *Files identical despite different names*

### Comparing `STARSimulator-1.0.5/src/stars/sly/lex.py` & `STARSimulator-1.0.6/src/stars/sly/lex.py`

 * *Files identical despite different names*

### Comparing `STARSimulator-1.0.5/src/stars/sly/yacc.py` & `STARSimulator-1.0.6/src/stars/sly/yacc.py`

 * *Files identical despite different names*

### Comparing `STARSimulator-1.0.5/src/stars/tests/classes/test_classes.py` & `STARSimulator-1.0.6/src/stars/tests/classes/test_classes.py`

 * *Files identical despite different names*

### Comparing `STARSimulator-1.0.5/src/stars/tests/controller/test_controller.py` & `STARSimulator-1.0.6/src/stars/tests/controller/test_controller.py`

 * *Files identical despite different names*

### Comparing `STARSimulator-1.0.5/src/stars/tests/debugger/test_debugger.py` & `STARSimulator-1.0.6/src/stars/tests/debugger/test_debugger.py`

 * *Files identical despite different names*

### Comparing `STARSimulator-1.0.5/src/stars/tests/debugger/test_debugger_stack.py` & `STARSimulator-1.0.6/src/stars/tests/debugger/test_debugger_stack.py`

 * *Files identical despite different names*

### Comparing `STARSimulator-1.0.5/src/stars/tests/fileOps/test_fileOps.py` & `STARSimulator-1.0.6/src/stars/tests/fileOps/test_fileOps.py`

 * *Files identical despite different names*

### Comparing `STARSimulator-1.0.5/src/stars/tests/floatInstrs/test.py` & `STARSimulator-1.0.6/src/stars/tests/floatInstrs/test.py`

 * *Files identical despite different names*

### Comparing `STARSimulator-1.0.5/src/stars/tests/instructions/instructions.py` & `STARSimulator-1.0.6/src/stars/tests/instructions/instructions.py`

 * *Files identical despite different names*

### Comparing `STARSimulator-1.0.5/src/stars/tests/instructions/test_add.py` & `STARSimulator-1.0.6/src/stars/tests/instructions/test_add.py`

 * *Files identical despite different names*

### Comparing `STARSimulator-1.0.5/src/stars/tests/instructions/test_addi.py` & `STARSimulator-1.0.6/src/stars/tests/instructions/test_addi.py`

 * *Files identical despite different names*

### Comparing `STARSimulator-1.0.5/src/stars/tests/instructions/test_addu.py` & `STARSimulator-1.0.6/src/stars/tests/instructions/test_addu.py`

 * *Files identical despite different names*

### Comparing `STARSimulator-1.0.5/src/stars/tests/instructions/test_and.py` & `STARSimulator-1.0.6/src/stars/tests/instructions/test_and.py`

 * *Files identical despite different names*

### Comparing `STARSimulator-1.0.5/src/stars/tests/instructions/test_beq.py` & `STARSimulator-1.0.6/src/stars/tests/instructions/test_beq.py`

 * *Files identical despite different names*

### Comparing `STARSimulator-1.0.5/src/stars/tests/instructions/test_bgez.py` & `STARSimulator-1.0.6/src/stars/tests/instructions/test_bgez.py`

 * *Files identical despite different names*

### Comparing `STARSimulator-1.0.5/src/stars/tests/instructions/test_bgezal.py` & `STARSimulator-1.0.6/src/stars/tests/instructions/test_bgezal.py`

 * *Files identical despite different names*

### Comparing `STARSimulator-1.0.5/src/stars/tests/instructions/test_bgtz.py` & `STARSimulator-1.0.6/src/stars/tests/instructions/test_bgtz.py`

 * *Files identical despite different names*

### Comparing `STARSimulator-1.0.5/src/stars/tests/instructions/test_blez.py` & `STARSimulator-1.0.6/src/stars/tests/instructions/test_blez.py`

 * *Files identical despite different names*

### Comparing `STARSimulator-1.0.5/src/stars/tests/instructions/test_bltz.py` & `STARSimulator-1.0.6/src/stars/tests/instructions/test_bltz.py`

 * *Files identical despite different names*

### Comparing `STARSimulator-1.0.5/src/stars/tests/instructions/test_bltzal.py` & `STARSimulator-1.0.6/src/stars/tests/instructions/test_bltzal.py`

 * *Files identical despite different names*

### Comparing `STARSimulator-1.0.5/src/stars/tests/instructions/test_bne.py` & `STARSimulator-1.0.6/src/stars/tests/instructions/test_bne.py`

 * *Files identical despite different names*

### Comparing `STARSimulator-1.0.5/src/stars/tests/instructions/test_clo.py` & `STARSimulator-1.0.6/src/stars/tests/instructions/test_clo.py`

 * *Files identical despite different names*

### Comparing `STARSimulator-1.0.5/src/stars/tests/instructions/test_clz.py` & `STARSimulator-1.0.6/src/stars/tests/instructions/test_clz.py`

 * *Files identical despite different names*

### Comparing `STARSimulator-1.0.5/src/stars/tests/instructions/test_div.py` & `STARSimulator-1.0.6/src/stars/tests/instructions/test_div.py`

 * *Files identical despite different names*

### Comparing `STARSimulator-1.0.5/src/stars/tests/instructions/test_divu.py` & `STARSimulator-1.0.6/src/stars/tests/instructions/test_divu.py`

 * *Files identical despite different names*

### Comparing `STARSimulator-1.0.5/src/stars/tests/instructions/test_j.py` & `STARSimulator-1.0.6/src/stars/tests/instructions/test_j.py`

 * *Files identical despite different names*

### Comparing `STARSimulator-1.0.5/src/stars/tests/instructions/test_jal.py` & `STARSimulator-1.0.6/src/stars/tests/instructions/test_jal.py`

 * *Files identical despite different names*

### Comparing `STARSimulator-1.0.5/src/stars/tests/instructions/test_jalr.py` & `STARSimulator-1.0.6/src/stars/tests/instructions/test_jalr.py`

 * *Files identical despite different names*

### Comparing `STARSimulator-1.0.5/src/stars/tests/instructions/test_lb.py` & `STARSimulator-1.0.6/src/stars/tests/instructions/test_lb.py`

 * *Files identical despite different names*

### Comparing `STARSimulator-1.0.5/src/stars/tests/instructions/test_lbu.py` & `STARSimulator-1.0.6/src/stars/tests/instructions/test_lbu.py`

 * *Files identical despite different names*

### Comparing `STARSimulator-1.0.5/src/stars/tests/instructions/test_lh.py` & `STARSimulator-1.0.6/src/stars/tests/instructions/test_lh.py`

 * *Files identical despite different names*

### Comparing `STARSimulator-1.0.5/src/stars/tests/instructions/test_lhu.py` & `STARSimulator-1.0.6/src/stars/tests/instructions/test_lhu.py`

 * *Files identical despite different names*

### Comparing `STARSimulator-1.0.5/src/stars/tests/instructions/test_lui.py` & `STARSimulator-1.0.6/src/stars/tests/instructions/test_lui.py`

 * *Files identical despite different names*

### Comparing `STARSimulator-1.0.5/src/stars/tests/instructions/test_lw.py` & `STARSimulator-1.0.6/src/stars/tests/instructions/test_lw.py`

 * *Files identical despite different names*

### Comparing `STARSimulator-1.0.5/src/stars/tests/instructions/test_lwl.py` & `STARSimulator-1.0.6/src/stars/tests/instructions/test_lwl.py`

 * *Files identical despite different names*

### Comparing `STARSimulator-1.0.5/src/stars/tests/instructions/test_lwr.py` & `STARSimulator-1.0.6/src/stars/tests/instructions/test_lwr.py`

 * *Files identical despite different names*

### Comparing `STARSimulator-1.0.5/src/stars/tests/instructions/test_mul.py` & `STARSimulator-1.0.6/src/stars/tests/instructions/test_mul.py`

 * *Files identical despite different names*

### Comparing `STARSimulator-1.0.5/src/stars/tests/instructions/test_mult.py` & `STARSimulator-1.0.6/src/stars/tests/instructions/test_mult.py`

 * *Files identical despite different names*

### Comparing `STARSimulator-1.0.5/src/stars/tests/instructions/test_multu.py` & `STARSimulator-1.0.6/src/stars/tests/instructions/test_multu.py`

 * *Files identical despite different names*

### Comparing `STARSimulator-1.0.5/src/stars/tests/instructions/test_nor.py` & `STARSimulator-1.0.6/src/stars/tests/instructions/test_nor.py`

 * *Files identical despite different names*

### Comparing `STARSimulator-1.0.5/src/stars/tests/instructions/test_or.py` & `STARSimulator-1.0.6/src/stars/tests/instructions/test_or.py`

 * *Files identical despite different names*

### Comparing `STARSimulator-1.0.5/src/stars/tests/instructions/test_sb.py` & `STARSimulator-1.0.6/src/stars/tests/instructions/test_sb.py`

 * *Files identical despite different names*

### Comparing `STARSimulator-1.0.5/src/stars/tests/instructions/test_sh.py` & `STARSimulator-1.0.6/src/stars/tests/instructions/test_sh.py`

 * *Files identical despite different names*

### Comparing `STARSimulator-1.0.5/src/stars/tests/instructions/test_sll.py` & `STARSimulator-1.0.6/src/stars/tests/instructions/test_sll.py`

 * *Files identical despite different names*

### Comparing `STARSimulator-1.0.5/src/stars/tests/instructions/test_sllv.py` & `STARSimulator-1.0.6/src/stars/tests/instructions/test_sllv.py`

 * *Files identical despite different names*

### Comparing `STARSimulator-1.0.5/src/stars/tests/instructions/test_slt.py` & `STARSimulator-1.0.6/src/stars/tests/instructions/test_slt.py`

 * *Files identical despite different names*

### Comparing `STARSimulator-1.0.5/src/stars/tests/instructions/test_slti.py` & `STARSimulator-1.0.6/src/stars/tests/instructions/test_slti.py`

 * *Files identical despite different names*

### Comparing `STARSimulator-1.0.5/src/stars/tests/instructions/test_sltiu.py` & `STARSimulator-1.0.6/src/stars/tests/instructions/test_sltiu.py`

 * *Files identical despite different names*

### Comparing `STARSimulator-1.0.5/src/stars/tests/instructions/test_sltu.py` & `STARSimulator-1.0.6/src/stars/tests/instructions/test_sltu.py`

 * *Files identical despite different names*

### Comparing `STARSimulator-1.0.5/src/stars/tests/instructions/test_sra.py` & `STARSimulator-1.0.6/src/stars/tests/instructions/test_sra.py`

 * *Files identical despite different names*

### Comparing `STARSimulator-1.0.5/src/stars/tests/instructions/test_srav.py` & `STARSimulator-1.0.6/src/stars/tests/instructions/test_srav.py`

 * *Files identical despite different names*

### Comparing `STARSimulator-1.0.5/src/stars/tests/instructions/test_srl.py` & `STARSimulator-1.0.6/src/stars/tests/instructions/test_srl.py`

 * *Files identical despite different names*

### Comparing `STARSimulator-1.0.5/src/stars/tests/instructions/test_srlv.py` & `STARSimulator-1.0.6/src/stars/tests/instructions/test_srlv.py`

 * *Files identical despite different names*

### Comparing `STARSimulator-1.0.5/src/stars/tests/instructions/test_sub.py` & `STARSimulator-1.0.6/src/stars/tests/instructions/test_sub.py`

 * *Files identical despite different names*

### Comparing `STARSimulator-1.0.5/src/stars/tests/instructions/test_sw.py` & `STARSimulator-1.0.6/src/stars/tests/instructions/test_sw.py`

 * *Files identical despite different names*

### Comparing `STARSimulator-1.0.5/src/stars/tests/instructions/test_swl.py` & `STARSimulator-1.0.6/src/stars/tests/instructions/test_swl.py`

 * *Files identical despite different names*

### Comparing `STARSimulator-1.0.5/src/stars/tests/instructions/test_swr.py` & `STARSimulator-1.0.6/src/stars/tests/instructions/test_swr.py`

 * *Files identical despite different names*

### Comparing `STARSimulator-1.0.5/src/stars/tests/instructions/test_xor.py` & `STARSimulator-1.0.6/src/stars/tests/instructions/test_xor.py`

 * *Files identical despite different names*

### Comparing `STARSimulator-1.0.5/src/stars/tests/interpreter/test_interpreter.py` & `STARSimulator-1.0.6/src/stars/tests/interpreter/test_interpreter.py`

 * *Files identical despite different names*

### Comparing `STARSimulator-1.0.5/src/stars/tests/interpreter/test_set_data.py` & `STARSimulator-1.0.6/src/stars/tests/interpreter/test_set_data.py`

 * *Files identical despite different names*

### Comparing `STARSimulator-1.0.5/src/stars/tests/preprocess/test_preprocess.py` & `STARSimulator-1.0.6/src/stars/tests/preprocess/test_preprocess.py`

 * *Files identical despite different names*

### Comparing `STARSimulator-1.0.5/src/stars/tests/pseudoOps/test_pseudoOps.py` & `STARSimulator-1.0.6/src/stars/tests/pseudoOps/test_pseudoOps.py`

 * *Files identical despite different names*

### Comparing `STARSimulator-1.0.5/src/stars/tests/registers/test_registers.py` & `STARSimulator-1.0.6/src/stars/tests/registers/test_registers.py`

 * *Files identical despite different names*

### Comparing `STARSimulator-1.0.5/src/stars/tests/syscalls/test_syscalls.py` & `STARSimulator-1.0.6/src/stars/tests/syscalls/test_syscalls.py`

 * *Files identical despite different names*

### Comparing `STARSimulator-1.0.5/src/stars/tests/test_sbumips.py` & `STARSimulator-1.0.6/src/stars/tests/test_sbumips.py`

 * *Files identical despite different names*

### Comparing `STARSimulator-1.0.5/src/stars/tests/validArgs/test_parse_args.py` & `STARSimulator-1.0.6/src/stars/tests/validArgs/test_parse_args.py`

 * *Files identical despite different names*

