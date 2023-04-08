# Comparing `tmp/STARSimulator-1.0.3.tar.gz` & `tmp/STARSimulator-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "STARSimulator-1.0.3.tar", last modified: Wed Feb 15 13:21:03 2023, max compression
+gzip compressed data, was "STARSimulator-1.0.5.tar", last modified: Sat Apr  8 17:54:58 2023, max compression
```

## Comparing `STARSimulator-1.0.3.tar` & `STARSimulator-1.0.5.tar`

### file list

```diff
@@ -1,162 +1,172 @@
-drwxrwxrwx   0        0        0        0 2023-02-15 13:21:03.978418 STARSimulator-1.0.3/
--rw-rw-rw-   0        0        0     1093 2023-02-15 12:39:25.000000 STARSimulator-1.0.3/LICENSE
--rw-rw-rw-   0        0        0     1881 2023-02-15 13:21:03.978418 STARSimulator-1.0.3/PKG-INFO
--rw-rw-rw-   0        0        0     1287 2023-02-15 12:41:34.000000 STARSimulator-1.0.3/README.md
--rw-rw-rw-   0        0        0      156 2023-02-15 12:41:34.000000 STARSimulator-1.0.3/pyproject.toml
--rw-rw-rw-   0        0        0      958 2023-02-15 13:21:03.980481 STARSimulator-1.0.3/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-02-15 13:21:03.724195 STARSimulator-1.0.3/src/
-drwxrwxrwx   0        0        0        0 2023-02-15 13:21:03.757997 STARSimulator-1.0.3/src/STARSimulator.egg-info/
--rw-rw-rw-   0        0        0     1881 2023-02-15 13:21:03.000000 STARSimulator-1.0.3/src/STARSimulator.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     4979 2023-02-15 13:21:03.000000 STARSimulator-1.0.3/src/STARSimulator.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-02-15 13:21:03.000000 STARSimulator-1.0.3/src/STARSimulator.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       44 2023-02-15 13:21:03.000000 STARSimulator-1.0.3/src/STARSimulator.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       25 2023-02-15 13:21:03.000000 STARSimulator-1.0.3/src/STARSimulator.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2023-02-15 13:21:03.000000 STARSimulator-1.0.3/src/STARSimulator.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-02-15 13:21:03.780112 STARSimulator-1.0.3/src/stars/
--rw-rw-rw-   0        0        0     1093 2023-02-15 12:39:25.000000 STARSimulator-1.0.3/src/stars/LICENSE
--rw-rw-rw-   0        0        0     1090 2023-02-15 12:41:34.000000 STARSimulator-1.0.3/src/stars/README.md
--rw-rw-rw-   0        0        0        0 2023-02-15 12:39:25.000000 STARSimulator-1.0.3/src/stars/__init__.py
--rw-rw-rw-   0        0        0     9801 2023-02-15 12:39:25.000000 STARSimulator-1.0.3/src/stars/constants.py
--rw-rw-rw-   0        0        0     2940 2023-02-15 12:39:25.000000 STARSimulator-1.0.3/src/stars/controller.py
-drwxrwxrwx   0        0        0        0 2023-02-15 13:21:03.794925 STARSimulator-1.0.3/src/stars/gui/
--rw-rw-rw-   0        0        0        0 2023-02-15 12:39:25.000000 STARSimulator-1.0.3/src/stars/gui/__init__.py
--rw-rw-rw-   0        0        0    28842 2023-02-15 12:41:34.000000 STARSimulator-1.0.3/src/stars/gui/mainwindow.py
-drwxrwxrwx   0        0        0        0 2023-02-15 13:21:03.811637 STARSimulator-1.0.3/src/stars/gui/resources/
--rw-rw-rw-   0        0        0        0 2023-02-15 12:39:25.000000 STARSimulator-1.0.3/src/stars/gui/resources/__init__.py
--rw-rw-rw-   0        0        0     9303 2023-02-15 12:39:25.000000 STARSimulator-1.0.3/src/stars/gui/resources/assemble.svg
--rw-rw-rw-   0        0        0     1237 2023-02-15 12:39:25.000000 STARSimulator-1.0.3/src/stars/gui/resources/backstep.svg
--rw-rw-rw-   0        0        0     1222 2023-02-15 12:39:25.000000 STARSimulator-1.0.3/src/stars/gui/resources/help.svg
--rw-rw-rw-   0        0        0     1716 2023-02-15 12:39:25.000000 STARSimulator-1.0.3/src/stars/gui/resources/new.svg
--rw-rw-rw-   0        0        0     2291 2023-02-15 12:39:25.000000 STARSimulator-1.0.3/src/stars/gui/resources/open.svg
--rw-rw-rw-   0        0        0     1322 2023-02-15 12:39:25.000000 STARSimulator-1.0.3/src/stars/gui/resources/pause.svg
--rw-rw-rw-   0        0        0     1361 2023-02-15 12:39:25.000000 STARSimulator-1.0.3/src/stars/gui/resources/save.svg
--rw-rw-rw-   0        0        0     1488 2023-02-15 12:39:25.000000 STARSimulator-1.0.3/src/stars/gui/resources/start.svg
--rw-rw-rw-   0        0        0     1249 2023-02-15 12:39:25.000000 STARSimulator-1.0.3/src/stars/gui/resources/step.svg
--rw-rw-rw-   0        0        0     2034 2023-02-15 12:41:34.000000 STARSimulator-1.0.3/src/stars/gui/syntaxhighlighter.py
--rw-rw-rw-   0        0        0    14045 2023-02-15 12:41:34.000000 STARSimulator-1.0.3/src/stars/gui/textedit.py
--rw-rw-rw-   0        0        0     7419 2023-02-15 12:41:34.000000 STARSimulator-1.0.3/src/stars/gui/theme.py
--rw-rw-rw-   0        0        0     5391 2023-02-15 12:41:34.000000 STARSimulator-1.0.3/src/stars/gui/vt100.py
--rw-rw-rw-   0        0        0     4535 2023-02-15 12:41:34.000000 STARSimulator-1.0.3/src/stars/gui/widgetfactory.py
-drwxrwxrwx   0        0        0        0 2023-02-15 13:21:03.829049 STARSimulator-1.0.3/src/stars/help/
--rw-rw-rw-   0        0        0        0 2023-02-15 12:39:25.000000 STARSimulator-1.0.3/src/stars/help/__init__.py
--rw-rw-rw-   0        0        0      412 2023-02-15 12:39:25.000000 STARSimulator-1.0.3/src/stars/help/bugs.md
--rw-rw-rw-   0        0        0      961 2023-02-15 12:39:25.000000 STARSimulator-1.0.3/src/stars/help/directives.csv
--rw-rw-rw-   0        0        0     2582 2023-02-15 12:41:34.000000 STARSimulator-1.0.3/src/stars/help/help.py
--rw-rw-rw-   0        0        0    41526 2023-02-15 12:39:25.000000 STARSimulator-1.0.3/src/stars/help/instruction_set (copy).csv
--rw-rw-rw-   0        0        0    43691 2023-02-15 12:39:25.000000 STARSimulator-1.0.3/src/stars/help/instruction_set.csv
--rw-rw-rw-   0        0        0    54317 2023-02-15 12:39:25.000000 STARSimulator-1.0.3/src/stars/help/instructions.csv
--rw-rw-rw-   0        0        0      851 2023-02-15 12:39:25.000000 STARSimulator-1.0.3/src/stars/help/operand.csv
--rw-rw-rw-   0        0        0     3717 2023-02-15 12:39:25.000000 STARSimulator-1.0.3/src/stars/help/syscalls.csv
--rw-rw-rw-   0        0        0     7210 2023-02-15 12:39:25.000000 STARSimulator-1.0.3/src/stars/instruction_constants.py
-drwxrwxrwx   0        0        0        0 2023-02-15 13:21:03.846195 STARSimulator-1.0.3/src/stars/interpreter/
--rw-rw-rw-   0        0        0        0 2023-02-15 12:39:25.000000 STARSimulator-1.0.3/src/stars/interpreter/__init__.py
--rw-rw-rw-   0        0        0     8252 2023-02-15 12:39:25.000000 STARSimulator-1.0.3/src/stars/interpreter/classes.py
--rw-rw-rw-   0        0        0    15045 2023-02-15 12:39:25.000000 STARSimulator-1.0.3/src/stars/interpreter/debugger.py
--rw-rw-rw-   0        0        0     2402 2023-02-15 12:39:25.000000 STARSimulator-1.0.3/src/stars/interpreter/exceptions.py
--rw-rw-rw-   0        0        0    29763 2023-02-15 12:39:25.000000 STARSimulator-1.0.3/src/stars/interpreter/instructions.py
--rw-rw-rw-   0        0        0    13438 2023-02-15 12:41:34.000000 STARSimulator-1.0.3/src/stars/interpreter/interpreter.py
--rw-rw-rw-   0        0        0     9393 2023-02-15 12:39:25.000000 STARSimulator-1.0.3/src/stars/interpreter/memory.py
--rw-rw-rw-   0        0        0     4105 2023-02-15 12:39:25.000000 STARSimulator-1.0.3/src/stars/interpreter/registers.py
--rw-rw-rw-   0        0        0    11237 2023-02-15 12:39:25.000000 STARSimulator-1.0.3/src/stars/interpreter/syscalls.py
--rw-rw-rw-   0        0        0     3317 2023-02-15 12:39:25.000000 STARSimulator-1.0.3/src/stars/interpreter/utility.py
--rw-rw-rw-   0        0        0     6458 2023-02-15 12:39:25.000000 STARSimulator-1.0.3/src/stars/lexer.py
--rw-rw-rw-   0        0        0    17425 2023-02-15 12:41:34.000000 STARSimulator-1.0.3/src/stars/mipsParser.py
--rw-rw-rw-   0        0        0     3539 2023-02-15 12:39:25.000000 STARSimulator-1.0.3/src/stars/preferences.json
--rw-rw-rw-   0        0        0     5643 2023-02-15 12:39:25.000000 STARSimulator-1.0.3/src/stars/preprocess.py
--rw-rw-rw-   0        0        0     5280 2023-02-15 12:39:25.000000 STARSimulator-1.0.3/src/stars/sbumips.py
--rw-rw-rw-   0        0        0     3051 2023-02-15 12:39:25.000000 STARSimulator-1.0.3/src/stars/settings.py
-drwxrwxrwx   0        0        0        0 2023-02-15 13:21:03.853717 STARSimulator-1.0.3/src/stars/sly/
--rw-rw-rw-   0        0        0        0 2023-02-15 12:39:25.000000 STARSimulator-1.0.3/src/stars/sly/__init__.py
--rw-rw-rw-   0        0        0    16056 2023-02-15 12:39:25.000000 STARSimulator-1.0.3/src/stars/sly/lex.py
--rw-rw-rw-   0        0        0    81225 2023-02-15 12:39:25.000000 STARSimulator-1.0.3/src/stars/sly/yacc.py
-drwxrwxrwx   0        0        0        0 2023-02-15 13:21:03.856718 STARSimulator-1.0.3/src/stars/tests/
--rw-rw-rw-   0        0        0        0 2023-02-15 12:39:25.000000 STARSimulator-1.0.3/src/stars/tests/__init__.py
-drwxrwxrwx   0        0        0        0 2023-02-15 13:21:03.859232 STARSimulator-1.0.3/src/stars/tests/classes/
--rw-rw-rw-   0        0        0        0 2023-02-15 12:39:25.000000 STARSimulator-1.0.3/src/stars/tests/classes/__init__.py
--rw-rw-rw-   0        0        0     9629 2023-02-15 12:39:25.000000 STARSimulator-1.0.3/src/stars/tests/classes/test_classes.py
-drwxrwxrwx   0        0        0        0 2023-02-15 13:21:03.861233 STARSimulator-1.0.3/src/stars/tests/controller/
--rw-rw-rw-   0        0        0        0 2023-02-15 12:39:25.000000 STARSimulator-1.0.3/src/stars/tests/controller/__init__.py
--rw-rw-rw-   0        0        0     5560 2023-02-15 12:39:25.000000 STARSimulator-1.0.3/src/stars/tests/controller/test_controller.py
-drwxrwxrwx   0        0        0        0 2023-02-15 13:21:03.865233 STARSimulator-1.0.3/src/stars/tests/debugger/
--rw-rw-rw-   0        0        0        0 2023-02-15 12:39:25.000000 STARSimulator-1.0.3/src/stars/tests/debugger/__init__.py
--rw-rw-rw-   0        0        0    16044 2023-02-15 12:39:25.000000 STARSimulator-1.0.3/src/stars/tests/debugger/test_debugger.py
--rw-rw-rw-   0        0        0    12173 2023-02-15 12:39:25.000000 STARSimulator-1.0.3/src/stars/tests/debugger/test_debugger_stack.py
-drwxrwxrwx   0        0        0        0 2023-02-15 13:21:03.867742 STARSimulator-1.0.3/src/stars/tests/fileOps/
--rw-rw-rw-   0        0        0        0 2023-02-15 12:39:25.000000 STARSimulator-1.0.3/src/stars/tests/fileOps/__init__.py
--rw-rw-rw-   0        0        0    14838 2023-02-15 12:39:25.000000 STARSimulator-1.0.3/src/stars/tests/fileOps/test_fileOps.py
-drwxrwxrwx   0        0        0        0 2023-02-15 13:21:03.872760 STARSimulator-1.0.3/src/stars/tests/floatInstrs/
--rw-rw-rw-   0        0        0        0 2023-02-15 12:39:25.000000 STARSimulator-1.0.3/src/stars/tests/floatInstrs/__init__.py
--rw-rw-rw-   0        0        0     9051 2023-02-15 12:39:25.000000 STARSimulator-1.0.3/src/stars/tests/floatInstrs/test.py
-drwxrwxrwx   0        0        0        0 2023-02-15 13:21:03.958127 STARSimulator-1.0.3/src/stars/tests/instructions/
--rw-rw-rw-   0        0        0        0 2023-02-15 12:39:25.000000 STARSimulator-1.0.3/src/stars/tests/instructions/__init__.py
--rw-rw-rw-   0        0        0     4113 2023-02-15 12:39:25.000000 STARSimulator-1.0.3/src/stars/tests/instructions/instructions.py
--rw-rw-rw-   0        0        0     1437 2023-02-15 12:39:25.000000 STARSimulator-1.0.3/src/stars/tests/instructions/test_add.py
--rw-rw-rw-   0        0        0      914 2023-02-15 12:39:25.000000 STARSimulator-1.0.3/src/stars/tests/instructions/test_addi.py
--rw-rw-rw-   0        0        0     1068 2023-02-15 12:39:25.000000 STARSimulator-1.0.3/src/stars/tests/instructions/test_addu.py
--rw-rw-rw-   0        0        0      569 2023-02-15 12:39:25.000000 STARSimulator-1.0.3/src/stars/tests/instructions/test_and.py
--rw-rw-rw-   0        0        0      680 2023-02-15 12:39:25.000000 STARSimulator-1.0.3/src/stars/tests/instructions/test_beq.py
--rw-rw-rw-   0        0        0     1095 2023-02-15 12:39:25.000000 STARSimulator-1.0.3/src/stars/tests/instructions/test_bgez.py
--rw-rw-rw-   0        0        0     1361 2023-02-15 12:39:25.000000 STARSimulator-1.0.3/src/stars/tests/instructions/test_bgezal.py
--rw-rw-rw-   0        0        0      633 2023-02-15 12:39:25.000000 STARSimulator-1.0.3/src/stars/tests/instructions/test_bgtz.py
--rw-rw-rw-   0        0        0     1093 2023-02-15 12:39:25.000000 STARSimulator-1.0.3/src/stars/tests/instructions/test_blez.py
--rw-rw-rw-   0        0        0      631 2023-02-15 12:39:25.000000 STARSimulator-1.0.3/src/stars/tests/instructions/test_bltz.py
--rw-rw-rw-   0        0        0      768 2023-02-15 12:39:25.000000 STARSimulator-1.0.3/src/stars/tests/instructions/test_bltzal.py
--rw-rw-rw-   0        0        0      680 2023-02-15 12:39:25.000000 STARSimulator-1.0.3/src/stars/tests/instructions/test_bne.py
--rw-rw-rw-   0        0        0     1203 2023-02-15 12:39:25.000000 STARSimulator-1.0.3/src/stars/tests/instructions/test_clo.py
--rw-rw-rw-   0        0        0     1200 2023-02-15 12:39:25.000000 STARSimulator-1.0.3/src/stars/tests/instructions/test_clz.py
--rw-rw-rw-   0        0        0     2752 2023-02-15 12:39:25.000000 STARSimulator-1.0.3/src/stars/tests/instructions/test_div.py
--rw-rw-rw-   0        0        0      637 2023-02-15 12:39:25.000000 STARSimulator-1.0.3/src/stars/tests/instructions/test_divu.py
--rw-rw-rw-   0        0        0      945 2023-02-15 12:39:25.000000 STARSimulator-1.0.3/src/stars/tests/instructions/test_j.py
--rw-rw-rw-   0        0        0     1129 2023-02-15 12:39:25.000000 STARSimulator-1.0.3/src/stars/tests/instructions/test_jal.py
--rw-rw-rw-   0        0        0      612 2023-02-15 12:39:25.000000 STARSimulator-1.0.3/src/stars/tests/instructions/test_jalr.py
--rw-rw-rw-   0        0        0      438 2023-02-15 12:39:25.000000 STARSimulator-1.0.3/src/stars/tests/instructions/test_jr.py
--rw-rw-rw-   0        0        0     1890 2023-02-15 12:39:25.000000 STARSimulator-1.0.3/src/stars/tests/instructions/test_lb.py
--rw-rw-rw-   0        0        0     1122 2023-02-15 12:39:25.000000 STARSimulator-1.0.3/src/stars/tests/instructions/test_lbu.py
--rw-rw-rw-   0        0        0     2286 2023-02-15 12:39:25.000000 STARSimulator-1.0.3/src/stars/tests/instructions/test_lh.py
--rw-rw-rw-   0        0        0      655 2023-02-15 12:39:25.000000 STARSimulator-1.0.3/src/stars/tests/instructions/test_lhu.py
--rw-rw-rw-   0        0        0     1307 2023-02-15 12:39:25.000000 STARSimulator-1.0.3/src/stars/tests/instructions/test_lui.py
--rw-rw-rw-   0        0        0     1517 2023-02-15 12:39:25.000000 STARSimulator-1.0.3/src/stars/tests/instructions/test_lw.py
--rw-rw-rw-   0        0        0     2062 2023-02-15 12:39:25.000000 STARSimulator-1.0.3/src/stars/tests/instructions/test_lwl.py
--rw-rw-rw-   0        0        0     2066 2023-02-15 12:39:25.000000 STARSimulator-1.0.3/src/stars/tests/instructions/test_lwr.py
--rw-rw-rw-   0        0        0     2046 2023-02-15 12:39:25.000000 STARSimulator-1.0.3/src/stars/tests/instructions/test_mul.py
--rw-rw-rw-   0        0        0     1282 2023-02-15 12:39:25.000000 STARSimulator-1.0.3/src/stars/tests/instructions/test_mult.py
--rw-rw-rw-   0        0        0      800 2023-02-15 12:39:25.000000 STARSimulator-1.0.3/src/stars/tests/instructions/test_multu.py
--rw-rw-rw-   0        0        0      635 2023-02-15 12:39:25.000000 STARSimulator-1.0.3/src/stars/tests/instructions/test_nor.py
--rw-rw-rw-   0        0        0      564 2023-02-15 12:39:25.000000 STARSimulator-1.0.3/src/stars/tests/instructions/test_or.py
--rw-rw-rw-   0        0        0     1996 2023-02-15 12:39:25.000000 STARSimulator-1.0.3/src/stars/tests/instructions/test_sb.py
--rw-rw-rw-   0        0        0     1170 2023-02-15 12:39:25.000000 STARSimulator-1.0.3/src/stars/tests/instructions/test_sh.py
--rw-rw-rw-   0        0        0      960 2023-02-15 12:39:25.000000 STARSimulator-1.0.3/src/stars/tests/instructions/test_sll.py
--rw-rw-rw-   0        0        0      707 2023-02-15 12:39:25.000000 STARSimulator-1.0.3/src/stars/tests/instructions/test_sllv.py
--rw-rw-rw-   0        0        0     1086 2023-02-15 12:39:25.000000 STARSimulator-1.0.3/src/stars/tests/instructions/test_slt.py
--rw-rw-rw-   0        0        0      595 2023-02-15 12:39:25.000000 STARSimulator-1.0.3/src/stars/tests/instructions/test_slti.py
--rw-rw-rw-   0        0        0      543 2023-02-15 12:39:25.000000 STARSimulator-1.0.3/src/stars/tests/instructions/test_sltiu.py
--rw-rw-rw-   0        0        0     1715 2023-02-15 12:39:25.000000 STARSimulator-1.0.3/src/stars/tests/instructions/test_sltu.py
--rw-rw-rw-   0        0        0      644 2023-02-15 12:39:25.000000 STARSimulator-1.0.3/src/stars/tests/instructions/test_sra.py
--rw-rw-rw-   0        0        0     1226 2023-02-15 12:39:25.000000 STARSimulator-1.0.3/src/stars/tests/instructions/test_srav.py
--rw-rw-rw-   0        0        0      982 2023-02-15 12:39:25.000000 STARSimulator-1.0.3/src/stars/tests/instructions/test_srl.py
--rw-rw-rw-   0        0        0     1518 2023-02-15 12:39:25.000000 STARSimulator-1.0.3/src/stars/tests/instructions/test_srlv.py
--rw-rw-rw-   0        0        0      562 2023-02-15 12:39:25.000000 STARSimulator-1.0.3/src/stars/tests/instructions/test_sub.py
--rw-rw-rw-   0        0        0     1296 2023-02-15 12:39:25.000000 STARSimulator-1.0.3/src/stars/tests/instructions/test_sw.py
--rw-rw-rw-   0        0        0     2813 2023-02-15 12:39:25.000000 STARSimulator-1.0.3/src/stars/tests/instructions/test_swl.py
--rw-rw-rw-   0        0        0     2817 2023-02-15 12:39:25.000000 STARSimulator-1.0.3/src/stars/tests/instructions/test_swr.py
--rw-rw-rw-   0        0        0      568 2023-02-15 12:39:25.000000 STARSimulator-1.0.3/src/stars/tests/instructions/test_xor.py
-drwxrwxrwx   0        0        0        0 2023-02-15 13:21:03.961134 STARSimulator-1.0.3/src/stars/tests/interpreter/
--rw-rw-rw-   0        0        0        0 2023-02-15 12:39:25.000000 STARSimulator-1.0.3/src/stars/tests/interpreter/__init__.py
--rw-rw-rw-   0        0        0     6700 2023-02-15 12:39:25.000000 STARSimulator-1.0.3/src/stars/tests/interpreter/test_interpreter.py
--rw-rw-rw-   0        0        0    13730 2023-02-15 12:39:25.000000 STARSimulator-1.0.3/src/stars/tests/interpreter/test_set_data.py
-drwxrwxrwx   0        0        0        0 2023-02-15 13:21:03.963134 STARSimulator-1.0.3/src/stars/tests/preprocess/
--rw-rw-rw-   0        0        0        0 2023-02-15 12:39:25.000000 STARSimulator-1.0.3/src/stars/tests/preprocess/__init__.py
--rw-rw-rw-   0        0        0     7188 2023-02-15 12:39:25.000000 STARSimulator-1.0.3/src/stars/tests/preprocess/test_preprocess.py
-drwxrwxrwx   0        0        0        0 2023-02-15 13:21:03.966135 STARSimulator-1.0.3/src/stars/tests/pseudoOps/
--rw-rw-rw-   0        0        0        0 2023-02-15 12:39:25.000000 STARSimulator-1.0.3/src/stars/tests/pseudoOps/__init__.py
--rw-rw-rw-   0        0        0     3488 2023-02-15 12:39:25.000000 STARSimulator-1.0.3/src/stars/tests/pseudoOps/test_pseudoOps.py
-drwxrwxrwx   0        0        0        0 2023-02-15 13:21:03.970697 STARSimulator-1.0.3/src/stars/tests/registers/
--rw-rw-rw-   0        0        0        0 2023-02-15 12:39:25.000000 STARSimulator-1.0.3/src/stars/tests/registers/__init__.py
--rw-rw-rw-   0        0        0     7499 2023-02-15 12:39:25.000000 STARSimulator-1.0.3/src/stars/tests/registers/test_registers.py
-drwxrwxrwx   0        0        0        0 2023-02-15 13:21:03.973678 STARSimulator-1.0.3/src/stars/tests/syscalls/
--rw-rw-rw-   0        0        0        0 2023-02-15 12:39:25.000000 STARSimulator-1.0.3/src/stars/tests/syscalls/__init__.py
--rw-rw-rw-   0        0        0    29392 2023-02-15 12:39:25.000000 STARSimulator-1.0.3/src/stars/tests/syscalls/test_syscalls.py
--rw-rw-rw-   0        0        0     4256 2023-02-15 12:39:25.000000 STARSimulator-1.0.3/src/stars/tests/test_sbumips.py
-drwxrwxrwx   0        0        0        0 2023-02-15 13:21:03.976678 STARSimulator-1.0.3/src/stars/tests/validArgs/
--rw-rw-rw-   0        0        0        0 2023-02-15 12:39:25.000000 STARSimulator-1.0.3/src/stars/tests/validArgs/__init__.py
--rw-rw-rw-   0        0        0     7854 2023-02-15 12:39:25.000000 STARSimulator-1.0.3/src/stars/tests/validArgs/test_parse_args.py
+drwxrwxrwx   0        0        0        0 2023-04-08 17:54:58.003538 STARSimulator-1.0.5/
+-rw-rw-rw-   0        0        0     1093 2022-11-18 17:38:34.000000 STARSimulator-1.0.5/LICENSE
+-rw-rw-rw-   0        0        0     1892 2023-04-08 17:54:58.004529 STARSimulator-1.0.5/PKG-INFO
+-rw-rw-rw-   0        0        0     1286 2023-02-22 04:38:55.000000 STARSimulator-1.0.5/README.md
+-rw-rw-rw-   0        0        0      153 2023-02-22 04:38:55.000000 STARSimulator-1.0.5/pyproject.toml
+-rw-rw-rw-   0        0        0      971 2023-04-08 17:54:58.007522 STARSimulator-1.0.5/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-04-08 17:54:57.615348 STARSimulator-1.0.5/src/
+drwxrwxrwx   0        0        0        0 2023-04-08 17:54:57.660117 STARSimulator-1.0.5/src/STARSimulator.egg-info/
+-rw-rw-rw-   0        0        0     1892 2023-04-08 17:54:57.000000 STARSimulator-1.0.5/src/STARSimulator.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     5371 2023-04-08 17:54:57.000000 STARSimulator-1.0.5/src/STARSimulator.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-08 17:54:57.000000 STARSimulator-1.0.5/src/STARSimulator.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       44 2023-04-08 17:54:57.000000 STARSimulator-1.0.5/src/STARSimulator.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       26 2023-04-08 17:54:57.000000 STARSimulator-1.0.5/src/STARSimulator.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2023-04-08 17:54:57.000000 STARSimulator-1.0.5/src/STARSimulator.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-08 17:54:57.687362 STARSimulator-1.0.5/src/stars/
+-rw-rw-rw-   0        0        0     1093 2022-11-18 17:38:34.000000 STARSimulator-1.0.5/src/stars/LICENSE
+-rw-rw-rw-   0        0        0     1089 2023-02-22 04:38:55.000000 STARSimulator-1.0.5/src/stars/README.md
+-rw-rw-rw-   0        0        0        0 2022-11-18 17:38:34.000000 STARSimulator-1.0.5/src/stars/__init__.py
+-rw-rw-rw-   0        0        0    10613 2023-03-12 00:05:28.000000 STARSimulator-1.0.5/src/stars/constants.py
+-rw-rw-rw-   0        0        0     2940 2022-11-18 17:38:34.000000 STARSimulator-1.0.5/src/stars/controller.py
+drwxrwxrwx   0        0        0        0 2023-04-08 17:54:57.702248 STARSimulator-1.0.5/src/stars/gui/
+-rw-rw-rw-   0        0        0        0 2022-11-18 17:38:34.000000 STARSimulator-1.0.5/src/stars/gui/__init__.py
+-rw-rw-rw-   0        0        0    31471 2023-04-08 02:01:16.000000 STARSimulator-1.0.5/src/stars/gui/mainwindow.py
+drwxrwxrwx   0        0        0        0 2023-04-08 17:54:57.745975 STARSimulator-1.0.5/src/stars/gui/resources/
+-rw-rw-rw-   0        0        0        0 2022-11-18 17:38:34.000000 STARSimulator-1.0.5/src/stars/gui/resources/__init__.py
+-rw-rw-rw-   0        0        0     9303 2022-11-18 17:38:34.000000 STARSimulator-1.0.5/src/stars/gui/resources/assemble.svg
+-rw-rw-rw-   0        0        0     9391 2023-03-12 00:05:28.000000 STARSimulator-1.0.5/src/stars/gui/resources/assemblewhite.svg
+-rw-rw-rw-   0        0        0     1237 2022-11-18 17:38:34.000000 STARSimulator-1.0.5/src/stars/gui/resources/backstep.svg
+-rw-rw-rw-   0        0        0     1281 2023-03-12 00:05:28.000000 STARSimulator-1.0.5/src/stars/gui/resources/backstepwhite.svg
+-rw-rw-rw-   0        0        0     1222 2022-11-18 17:38:34.000000 STARSimulator-1.0.5/src/stars/gui/resources/help.svg
+-rw-rw-rw-   0        0        0     1288 2023-03-12 00:05:28.000000 STARSimulator-1.0.5/src/stars/gui/resources/helpwhite.svg
+-rw-rw-rw-   0        0        0     1716 2022-11-18 17:38:34.000000 STARSimulator-1.0.5/src/stars/gui/resources/new.svg
+-rw-rw-rw-   0        0        0     1716 2023-03-12 00:05:28.000000 STARSimulator-1.0.5/src/stars/gui/resources/newwhite.svg
+-rw-rw-rw-   0        0        0     2291 2022-11-18 17:38:34.000000 STARSimulator-1.0.5/src/stars/gui/resources/open.svg
+-rw-rw-rw-   0        0        0     2313 2023-03-12 00:05:28.000000 STARSimulator-1.0.5/src/stars/gui/resources/openwhite.svg
+-rw-rw-rw-   0        0        0     1322 2022-11-18 17:38:34.000000 STARSimulator-1.0.5/src/stars/gui/resources/pause.svg
+-rw-rw-rw-   0        0        0     1388 2023-03-12 00:05:28.000000 STARSimulator-1.0.5/src/stars/gui/resources/pausewhite.svg
+-rw-rw-rw-   0        0        0     1361 2022-11-18 17:38:34.000000 STARSimulator-1.0.5/src/stars/gui/resources/save.svg
+-rw-rw-rw-   0        0        0     1449 2023-03-12 00:05:28.000000 STARSimulator-1.0.5/src/stars/gui/resources/savewhite.svg
+-rw-rw-rw-   0        0        0     1488 2022-11-18 17:38:34.000000 STARSimulator-1.0.5/src/stars/gui/resources/start.svg
+-rw-rw-rw-   0        0        0     1532 2023-03-12 00:05:28.000000 STARSimulator-1.0.5/src/stars/gui/resources/startwhite.svg
+-rw-rw-rw-   0        0        0     1249 2022-11-18 17:38:34.000000 STARSimulator-1.0.5/src/stars/gui/resources/step.svg
+-rw-rw-rw-   0        0        0     1293 2023-03-12 00:05:28.000000 STARSimulator-1.0.5/src/stars/gui/resources/stepwhite.svg
+-rw-rw-rw-   0        0        0     2034 2023-02-22 04:38:55.000000 STARSimulator-1.0.5/src/stars/gui/syntaxhighlighter.py
+-rw-rw-rw-   0        0        0    14086 2023-03-12 00:05:28.000000 STARSimulator-1.0.5/src/stars/gui/textedit.py
+-rw-rw-rw-   0        0        0     7419 2023-02-22 04:38:55.000000 STARSimulator-1.0.5/src/stars/gui/theme.py
+-rw-rw-rw-   0        0        0     5391 2023-02-22 04:38:55.000000 STARSimulator-1.0.5/src/stars/gui/vt100.py
+-rw-rw-rw-   0        0        0     4529 2023-02-22 04:38:55.000000 STARSimulator-1.0.5/src/stars/gui/widgetfactory.py
+drwxrwxrwx   0        0        0        0 2023-04-08 17:54:57.766754 STARSimulator-1.0.5/src/stars/help/
+-rw-rw-rw-   0        0        0        0 2022-11-18 17:38:34.000000 STARSimulator-1.0.5/src/stars/help/__init__.py
+-rw-rw-rw-   0        0        0      412 2022-11-18 17:38:34.000000 STARSimulator-1.0.5/src/stars/help/bugs.md
+-rw-rw-rw-   0        0        0      961 2022-11-18 17:38:34.000000 STARSimulator-1.0.5/src/stars/help/directives.csv
+-rw-rw-rw-   0        0        0     2816 2023-04-04 22:19:32.000000 STARSimulator-1.0.5/src/stars/help/help.py
+-rw-rw-rw-   0        0        0    41526 2022-11-18 17:38:34.000000 STARSimulator-1.0.5/src/stars/help/instruction_set (copy).csv
+-rw-rw-rw-   0        0        0    43691 2022-11-18 17:38:34.000000 STARSimulator-1.0.5/src/stars/help/instruction_set.csv
+-rw-rw-rw-   0        0        0    54317 2022-11-18 17:38:34.000000 STARSimulator-1.0.5/src/stars/help/instructions.csv
+-rw-rw-rw-   0        0        0      851 2022-11-18 17:38:34.000000 STARSimulator-1.0.5/src/stars/help/operand.csv
+-rw-rw-rw-   0        0        0     3717 2022-11-18 17:38:34.000000 STARSimulator-1.0.5/src/stars/help/syscalls.csv
+-rw-rw-rw-   0        0        0     7210 2023-01-27 13:53:33.000000 STARSimulator-1.0.5/src/stars/instruction_constants.py
+drwxrwxrwx   0        0        0        0 2023-04-08 17:54:57.790320 STARSimulator-1.0.5/src/stars/interpreter/
+-rw-rw-rw-   0        0        0        0 2022-11-18 17:38:34.000000 STARSimulator-1.0.5/src/stars/interpreter/__init__.py
+-rw-rw-rw-   0        0        0     8252 2023-04-05 03:30:04.000000 STARSimulator-1.0.5/src/stars/interpreter/classes.py
+-rw-rw-rw-   0        0        0     7566 2023-04-08 17:34:54.000000 STARSimulator-1.0.5/src/stars/interpreter/compiled_tester.py
+-rw-rw-rw-   0        0        0    15045 2023-01-27 13:53:33.000000 STARSimulator-1.0.5/src/stars/interpreter/debugger.py
+-rw-rw-rw-   0        0        0     2402 2023-01-27 13:53:33.000000 STARSimulator-1.0.5/src/stars/interpreter/exceptions.py
+-rw-rw-rw-   0        0        0    29763 2023-01-27 13:53:33.000000 STARSimulator-1.0.5/src/stars/interpreter/instructions.py
+-rw-rw-rw-   0        0        0    14726 2023-04-08 02:08:22.000000 STARSimulator-1.0.5/src/stars/interpreter/interpreter.py
+-rw-rw-rw-   0        0        0     9607 2023-04-08 00:21:34.000000 STARSimulator-1.0.5/src/stars/interpreter/memory.py
+-rw-rw-rw-   0        0        0     4105 2023-01-27 13:53:33.000000 STARSimulator-1.0.5/src/stars/interpreter/registers.py
+-rw-rw-rw-   0        0        0    11237 2023-01-27 13:53:33.000000 STARSimulator-1.0.5/src/stars/interpreter/syscalls.py
+-rw-rw-rw-   0        0        0     3317 2023-01-27 13:53:33.000000 STARSimulator-1.0.5/src/stars/interpreter/utility.py
+-rw-rw-rw-   0        0        0     6458 2022-11-18 17:38:34.000000 STARSimulator-1.0.5/src/stars/lexer.py
+-rw-rw-rw-   0        0        0    17977 2023-04-05 00:08:37.000000 STARSimulator-1.0.5/src/stars/mipsParser.py
+-rw-rw-rw-   0        0        0     4206 2023-03-12 00:05:28.000000 STARSimulator-1.0.5/src/stars/preferences.json
+-rw-rw-rw-   0        0        0     5825 2023-03-29 11:51:24.000000 STARSimulator-1.0.5/src/stars/preprocess.py
+-rw-rw-rw-   0        0        0     5318 2023-04-08 02:08:52.000000 STARSimulator-1.0.5/src/stars/sbumips.py
+-rw-rw-rw-   0        0        0     3051 2023-01-27 13:53:33.000000 STARSimulator-1.0.5/src/stars/settings.py
+drwxrwxrwx   0        0        0        0 2023-04-08 17:54:57.796331 STARSimulator-1.0.5/src/stars/sly/
+-rw-rw-rw-   0        0        0        0 2022-11-18 17:38:34.000000 STARSimulator-1.0.5/src/stars/sly/__init__.py
+-rw-rw-rw-   0        0        0    16056 2022-11-18 17:38:34.000000 STARSimulator-1.0.5/src/stars/sly/lex.py
+-rw-rw-rw-   0        0        0    81225 2022-11-18 17:38:34.000000 STARSimulator-1.0.5/src/stars/sly/yacc.py
+drwxrwxrwx   0        0        0        0 2023-04-08 17:54:57.800854 STARSimulator-1.0.5/src/stars/tests/
+-rw-rw-rw-   0        0        0        0 2022-11-18 17:38:34.000000 STARSimulator-1.0.5/src/stars/tests/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-08 17:54:57.804870 STARSimulator-1.0.5/src/stars/tests/classes/
+-rw-rw-rw-   0        0        0        0 2022-11-18 17:38:34.000000 STARSimulator-1.0.5/src/stars/tests/classes/__init__.py
+-rw-rw-rw-   0        0        0     9629 2022-11-18 17:38:34.000000 STARSimulator-1.0.5/src/stars/tests/classes/test_classes.py
+drwxrwxrwx   0        0        0        0 2023-04-08 17:54:57.808862 STARSimulator-1.0.5/src/stars/tests/controller/
+-rw-rw-rw-   0        0        0        0 2022-11-18 17:38:34.000000 STARSimulator-1.0.5/src/stars/tests/controller/__init__.py
+-rw-rw-rw-   0        0        0     5681 2023-02-22 06:28:43.000000 STARSimulator-1.0.5/src/stars/tests/controller/test_controller.py
+drwxrwxrwx   0        0        0        0 2023-04-08 17:54:57.814191 STARSimulator-1.0.5/src/stars/tests/debugger/
+-rw-rw-rw-   0        0        0        0 2022-11-18 17:38:34.000000 STARSimulator-1.0.5/src/stars/tests/debugger/__init__.py
+-rw-rw-rw-   0        0        0    16044 2022-11-18 17:38:34.000000 STARSimulator-1.0.5/src/stars/tests/debugger/test_debugger.py
+-rw-rw-rw-   0        0        0    12173 2022-11-18 17:38:34.000000 STARSimulator-1.0.5/src/stars/tests/debugger/test_debugger_stack.py
+drwxrwxrwx   0        0        0        0 2023-04-08 17:54:57.818194 STARSimulator-1.0.5/src/stars/tests/fileOps/
+-rw-rw-rw-   0        0        0        0 2022-11-18 17:38:34.000000 STARSimulator-1.0.5/src/stars/tests/fileOps/__init__.py
+-rw-rw-rw-   0        0        0    14838 2022-11-18 17:38:34.000000 STARSimulator-1.0.5/src/stars/tests/fileOps/test_fileOps.py
+drwxrwxrwx   0        0        0        0 2023-04-08 17:54:57.822374 STARSimulator-1.0.5/src/stars/tests/floatInstrs/
+-rw-rw-rw-   0        0        0        0 2022-11-18 17:38:34.000000 STARSimulator-1.0.5/src/stars/tests/floatInstrs/__init__.py
+-rw-rw-rw-   0        0        0     9051 2022-11-18 17:38:34.000000 STARSimulator-1.0.5/src/stars/tests/floatInstrs/test.py
+drwxrwxrwx   0        0        0        0 2023-04-08 17:54:57.952054 STARSimulator-1.0.5/src/stars/tests/instructions/
+-rw-rw-rw-   0        0        0        0 2022-11-18 17:38:34.000000 STARSimulator-1.0.5/src/stars/tests/instructions/__init__.py
+-rw-rw-rw-   0        0        0     4113 2022-11-18 17:38:34.000000 STARSimulator-1.0.5/src/stars/tests/instructions/instructions.py
+-rw-rw-rw-   0        0        0     1437 2022-11-18 17:38:34.000000 STARSimulator-1.0.5/src/stars/tests/instructions/test_add.py
+-rw-rw-rw-   0        0        0      914 2022-11-18 17:38:34.000000 STARSimulator-1.0.5/src/stars/tests/instructions/test_addi.py
+-rw-rw-rw-   0        0        0     1068 2022-11-18 17:38:34.000000 STARSimulator-1.0.5/src/stars/tests/instructions/test_addu.py
+-rw-rw-rw-   0        0        0      569 2022-11-18 17:38:34.000000 STARSimulator-1.0.5/src/stars/tests/instructions/test_and.py
+-rw-rw-rw-   0        0        0      680 2022-11-18 17:38:34.000000 STARSimulator-1.0.5/src/stars/tests/instructions/test_beq.py
+-rw-rw-rw-   0        0        0     1095 2022-11-18 17:38:34.000000 STARSimulator-1.0.5/src/stars/tests/instructions/test_bgez.py
+-rw-rw-rw-   0        0        0     1361 2022-11-18 17:38:34.000000 STARSimulator-1.0.5/src/stars/tests/instructions/test_bgezal.py
+-rw-rw-rw-   0        0        0      633 2022-11-18 17:38:34.000000 STARSimulator-1.0.5/src/stars/tests/instructions/test_bgtz.py
+-rw-rw-rw-   0        0        0     1093 2022-11-18 17:38:34.000000 STARSimulator-1.0.5/src/stars/tests/instructions/test_blez.py
+-rw-rw-rw-   0        0        0      631 2022-11-18 17:38:34.000000 STARSimulator-1.0.5/src/stars/tests/instructions/test_bltz.py
+-rw-rw-rw-   0        0        0      768 2022-11-18 17:38:34.000000 STARSimulator-1.0.5/src/stars/tests/instructions/test_bltzal.py
+-rw-rw-rw-   0        0        0      680 2022-11-18 17:38:34.000000 STARSimulator-1.0.5/src/stars/tests/instructions/test_bne.py
+-rw-rw-rw-   0        0        0     1203 2022-11-18 17:38:34.000000 STARSimulator-1.0.5/src/stars/tests/instructions/test_clo.py
+-rw-rw-rw-   0        0        0     1200 2022-11-18 17:38:34.000000 STARSimulator-1.0.5/src/stars/tests/instructions/test_clz.py
+-rw-rw-rw-   0        0        0     2752 2022-11-18 17:38:34.000000 STARSimulator-1.0.5/src/stars/tests/instructions/test_div.py
+-rw-rw-rw-   0        0        0      637 2022-11-18 17:38:34.000000 STARSimulator-1.0.5/src/stars/tests/instructions/test_divu.py
+-rw-rw-rw-   0        0        0      945 2022-11-18 17:38:34.000000 STARSimulator-1.0.5/src/stars/tests/instructions/test_j.py
+-rw-rw-rw-   0        0        0     1129 2022-11-18 17:38:34.000000 STARSimulator-1.0.5/src/stars/tests/instructions/test_jal.py
+-rw-rw-rw-   0        0        0      612 2022-11-18 17:38:34.000000 STARSimulator-1.0.5/src/stars/tests/instructions/test_jalr.py
+-rw-rw-rw-   0        0        0      438 2022-11-18 17:38:34.000000 STARSimulator-1.0.5/src/stars/tests/instructions/test_jr.py
+-rw-rw-rw-   0        0        0     1890 2022-11-18 17:38:34.000000 STARSimulator-1.0.5/src/stars/tests/instructions/test_lb.py
+-rw-rw-rw-   0        0        0     1122 2022-11-18 17:38:34.000000 STARSimulator-1.0.5/src/stars/tests/instructions/test_lbu.py
+-rw-rw-rw-   0        0        0     2286 2022-11-18 17:38:34.000000 STARSimulator-1.0.5/src/stars/tests/instructions/test_lh.py
+-rw-rw-rw-   0        0        0      655 2022-11-18 17:38:34.000000 STARSimulator-1.0.5/src/stars/tests/instructions/test_lhu.py
+-rw-rw-rw-   0        0        0     1307 2022-11-18 17:38:34.000000 STARSimulator-1.0.5/src/stars/tests/instructions/test_lui.py
+-rw-rw-rw-   0        0        0     1517 2022-11-18 17:38:34.000000 STARSimulator-1.0.5/src/stars/tests/instructions/test_lw.py
+-rw-rw-rw-   0        0        0     2062 2022-11-18 17:38:34.000000 STARSimulator-1.0.5/src/stars/tests/instructions/test_lwl.py
+-rw-rw-rw-   0        0        0     2066 2022-11-18 17:38:34.000000 STARSimulator-1.0.5/src/stars/tests/instructions/test_lwr.py
+-rw-rw-rw-   0        0        0     2046 2022-11-18 17:38:34.000000 STARSimulator-1.0.5/src/stars/tests/instructions/test_mul.py
+-rw-rw-rw-   0        0        0     1282 2022-11-18 17:38:34.000000 STARSimulator-1.0.5/src/stars/tests/instructions/test_mult.py
+-rw-rw-rw-   0        0        0      800 2022-11-18 17:38:34.000000 STARSimulator-1.0.5/src/stars/tests/instructions/test_multu.py
+-rw-rw-rw-   0        0        0      635 2022-11-18 17:38:34.000000 STARSimulator-1.0.5/src/stars/tests/instructions/test_nor.py
+-rw-rw-rw-   0        0        0      564 2022-11-18 17:38:34.000000 STARSimulator-1.0.5/src/stars/tests/instructions/test_or.py
+-rw-rw-rw-   0        0        0     1996 2022-11-18 17:38:34.000000 STARSimulator-1.0.5/src/stars/tests/instructions/test_sb.py
+-rw-rw-rw-   0        0        0     1170 2022-11-18 17:38:34.000000 STARSimulator-1.0.5/src/stars/tests/instructions/test_sh.py
+-rw-rw-rw-   0        0        0      960 2022-11-18 17:38:34.000000 STARSimulator-1.0.5/src/stars/tests/instructions/test_sll.py
+-rw-rw-rw-   0        0        0      707 2022-11-18 17:38:34.000000 STARSimulator-1.0.5/src/stars/tests/instructions/test_sllv.py
+-rw-rw-rw-   0        0        0     1086 2022-11-18 17:38:34.000000 STARSimulator-1.0.5/src/stars/tests/instructions/test_slt.py
+-rw-rw-rw-   0        0        0      595 2022-11-18 17:38:34.000000 STARSimulator-1.0.5/src/stars/tests/instructions/test_slti.py
+-rw-rw-rw-   0        0        0      543 2022-11-18 17:38:34.000000 STARSimulator-1.0.5/src/stars/tests/instructions/test_sltiu.py
+-rw-rw-rw-   0        0        0     1715 2022-11-18 17:38:34.000000 STARSimulator-1.0.5/src/stars/tests/instructions/test_sltu.py
+-rw-rw-rw-   0        0        0      644 2022-11-18 17:38:34.000000 STARSimulator-1.0.5/src/stars/tests/instructions/test_sra.py
+-rw-rw-rw-   0        0        0     1226 2022-11-18 17:38:34.000000 STARSimulator-1.0.5/src/stars/tests/instructions/test_srav.py
+-rw-rw-rw-   0        0        0      982 2022-11-18 17:38:34.000000 STARSimulator-1.0.5/src/stars/tests/instructions/test_srl.py
+-rw-rw-rw-   0        0        0     1518 2022-11-18 17:38:34.000000 STARSimulator-1.0.5/src/stars/tests/instructions/test_srlv.py
+-rw-rw-rw-   0        0        0      562 2022-11-18 17:38:34.000000 STARSimulator-1.0.5/src/stars/tests/instructions/test_sub.py
+-rw-rw-rw-   0        0        0     1296 2022-11-18 17:38:34.000000 STARSimulator-1.0.5/src/stars/tests/instructions/test_sw.py
+-rw-rw-rw-   0        0        0     2813 2022-11-18 17:38:34.000000 STARSimulator-1.0.5/src/stars/tests/instructions/test_swl.py
+-rw-rw-rw-   0        0        0     2817 2022-11-18 17:38:34.000000 STARSimulator-1.0.5/src/stars/tests/instructions/test_swr.py
+-rw-rw-rw-   0        0        0      568 2022-11-18 17:38:34.000000 STARSimulator-1.0.5/src/stars/tests/instructions/test_xor.py
+drwxrwxrwx   0        0        0        0 2023-04-08 17:54:57.962611 STARSimulator-1.0.5/src/stars/tests/interpreter/
+-rw-rw-rw-   0        0        0        0 2022-11-18 17:38:34.000000 STARSimulator-1.0.5/src/stars/tests/interpreter/__init__.py
+-rw-rw-rw-   0        0        0     6700 2022-11-18 17:38:34.000000 STARSimulator-1.0.5/src/stars/tests/interpreter/test_interpreter.py
+-rw-rw-rw-   0        0        0    13730 2022-11-18 17:38:34.000000 STARSimulator-1.0.5/src/stars/tests/interpreter/test_set_data.py
+drwxrwxrwx   0        0        0        0 2023-04-08 17:54:57.969658 STARSimulator-1.0.5/src/stars/tests/preprocess/
+-rw-rw-rw-   0        0        0        0 2022-11-18 17:38:34.000000 STARSimulator-1.0.5/src/stars/tests/preprocess/__init__.py
+-rw-rw-rw-   0        0        0     7386 2023-03-29 11:51:24.000000 STARSimulator-1.0.5/src/stars/tests/preprocess/test_preprocess.py
+drwxrwxrwx   0        0        0        0 2023-04-08 17:54:57.973693 STARSimulator-1.0.5/src/stars/tests/pseudoOps/
+-rw-rw-rw-   0        0        0        0 2022-11-18 17:38:34.000000 STARSimulator-1.0.5/src/stars/tests/pseudoOps/__init__.py
+-rw-rw-rw-   0        0        0     3488 2022-11-18 17:38:34.000000 STARSimulator-1.0.5/src/stars/tests/pseudoOps/test_pseudoOps.py
+drwxrwxrwx   0        0        0        0 2023-04-08 17:54:57.984285 STARSimulator-1.0.5/src/stars/tests/registers/
+-rw-rw-rw-   0        0        0        0 2022-11-18 17:38:34.000000 STARSimulator-1.0.5/src/stars/tests/registers/__init__.py
+-rw-rw-rw-   0        0        0     7499 2022-11-18 17:38:34.000000 STARSimulator-1.0.5/src/stars/tests/registers/test_registers.py
+drwxrwxrwx   0        0        0        0 2023-04-08 17:54:57.988315 STARSimulator-1.0.5/src/stars/tests/syscalls/
+-rw-rw-rw-   0        0        0        0 2022-11-18 17:38:34.000000 STARSimulator-1.0.5/src/stars/tests/syscalls/__init__.py
+-rw-rw-rw-   0        0        0    29392 2022-11-18 17:38:34.000000 STARSimulator-1.0.5/src/stars/tests/syscalls/test_syscalls.py
+-rw-rw-rw-   0        0        0     4412 2023-03-01 14:04:44.000000 STARSimulator-1.0.5/src/stars/tests/test_sbumips.py
+drwxrwxrwx   0        0        0        0 2023-04-08 17:54:57.997886 STARSimulator-1.0.5/src/stars/tests/validArgs/
+-rw-rw-rw-   0        0        0        0 2022-11-18 17:38:34.000000 STARSimulator-1.0.5/src/stars/tests/validArgs/__init__.py
+-rw-rw-rw-   0        0        0     7854 2022-11-18 17:38:34.000000 STARSimulator-1.0.5/src/stars/tests/validArgs/test_parse_args.py
```

### Comparing `STARSimulator-1.0.3/LICENSE` & `STARSimulator-1.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `STARSimulator-1.0.3/PKG-INFO` & `STARSimulator-1.0.5/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 Metadata-Version: 2.1
 Name: STARSimulator
-Version: 1.0.3
+Version: 1.0.5
 Summary: STARS (Stony Brook Assembler and Run-time Simulator) is a MIPS Assembly simulator made for the purpose of education.
 Home-page: https://github.com/sbustars/STARS
 Author: STARS
-Author-email: stars@cs.stonybrook.edu
+Author-email: jason.osoriomarin@cs.stonybrook.edu
 Project-URL: Bug Tracker, https://github.com/sbustars/STARS/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # The STARS Code Repository
 
 ## Overview
 This repository hosts the public releases of STARS (Stony Brook Assembler and Run-time Simulator). STARS is a MIPS Assembly simulator made for the purpose of education.
 
 ## Dependencies
-* PySide2 (v5.15 or newer)
+* PySide6 (v6.4 or newer)
 * numpy (v1.23 or newer for Windows)
 
 # How to run:
 Install the package.
 ```
 $ pip install STARSimulator
 ```
```

### Comparing `STARSimulator-1.0.3/README.md` & `STARSimulator-1.0.5/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # The STARS Code Repository
 
 ## Overview
 This repository hosts the public releases of STARS (Stony Brook Assembler and Run-time Simulator). STARS is a MIPS Assembly simulator made for the purpose of education.
 
 ## Dependencies
-* PySide2 (v5.15 or newer)
+* PySide6 (v6.4 or newer)
 * numpy (v1.23 or newer for Windows)
 
 # How to run:
 Install the package.
 ```
 $ pip install STARSimulator
 ```
```

### Comparing `STARSimulator-1.0.3/setup.cfg` & `STARSimulator-1.0.5/setup.cfg`

 * *Files 16% similar despite different names*

```diff
@@ -1,60 +1,61 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2053 5441 5253 696d 756c 6174 6f72   = STARSimulator
 00000020: 0d0a 7665 7273 696f 6e20 3d20 312e 302e  ..version = 1.0.
-00000030: 330d 0a61 7574 686f 7220 3d20 5354 4152  3..author = STAR
+00000030: 350d 0a61 7574 686f 7220 3d20 5354 4152  5..author = STAR
 00000040: 530d 0a61 7574 686f 725f 656d 6169 6c20  S..author_email 
-00000050: 3d20 7374 6172 7340 6373 2e73 746f 6e79  = stars@cs.stony
-00000060: 6272 6f6f 6b2e 6564 750d 0a64 6573 6372  brook.edu..descr
-00000070: 6970 7469 6f6e 203d 2053 5441 5253 2028  iption = STARS (
-00000080: 5374 6f6e 7920 4272 6f6f 6b20 4173 7365  Stony Brook Asse
-00000090: 6d62 6c65 7220 616e 6420 5275 6e2d 7469  mbler and Run-ti
-000000a0: 6d65 2053 696d 756c 6174 6f72 2920 6973  me Simulator) is
-000000b0: 2061 204d 4950 5320 4173 7365 6d62 6c79   a MIPS Assembly
-000000c0: 2073 696d 756c 6174 6f72 206d 6164 6520   simulator made 
-000000d0: 666f 7220 7468 6520 7075 7270 6f73 6520  for the purpose 
-000000e0: 6f66 2065 6475 6361 7469 6f6e 2e0d 0a6c  of education...l
-000000f0: 6f6e 675f 6465 7363 7269 7074 696f 6e20  ong_description 
-00000100: 3d20 6669 6c65 3a20 5245 4144 4d45 2e6d  = file: README.m
-00000110: 640d 0a6c 6f6e 675f 6465 7363 7269 7074  d..long_descript
-00000120: 696f 6e5f 636f 6e74 656e 745f 7479 7065  ion_content_type
-00000130: 203d 2074 6578 742f 6d61 726b 646f 776e   = text/markdown
-00000140: 0d0a 7572 6c20 3d20 6874 7470 733a 2f2f  ..url = https://
-00000150: 6769 7468 7562 2e63 6f6d 2f73 6275 7374  github.com/sbust
-00000160: 6172 732f 5354 4152 530d 0a70 726f 6a65  ars/STARS..proje
-00000170: 6374 5f75 726c 7320 3d20 0d0a 0942 7567  ct_urls = ...Bug
-00000180: 2054 7261 636b 6572 203d 2068 7474 7073   Tracker = https
-00000190: 3a2f 2f67 6974 6875 622e 636f 6d2f 7362  ://github.com/sb
-000001a0: 7573 7461 7273 2f53 5441 5253 2f69 7373  ustars/STARS/iss
-000001b0: 7565 730d 0a63 6c61 7373 6966 6965 7273  ues..classifiers
-000001c0: 203d 200d 0a09 5072 6f67 7261 6d6d 696e   = ...Programmin
-000001d0: 6720 4c61 6e67 7561 6765 203a 3a20 5079  g Language :: Py
-000001e0: 7468 6f6e 203a 3a20 330d 0a09 4c69 6365  thon :: 3...Lice
-000001f0: 6e73 6520 3a3a 204f 5349 2041 7070 726f  nse :: OSI Appro
-00000200: 7665 6420 3a3a 204d 4954 204c 6963 656e  ved :: MIT Licen
-00000210: 7365 0d0a 094f 7065 7261 7469 6e67 2053  se...Operating S
-00000220: 7973 7465 6d20 3a3a 204f 5320 496e 6465  ystem :: OS Inde
-00000230: 7065 6e64 656e 740d 0a0d 0a5b 6f70 7469  pendent....[opti
-00000240: 6f6e 735d 0d0a 696e 636c 7564 655f 7061  ons]..include_pa
-00000250: 636b 6167 655f 6461 7461 203d 2054 7275  ckage_data = Tru
-00000260: 650d 0a70 6163 6b61 6765 5f64 6972 203d  e..package_dir =
-00000270: 200d 0a09 3d20 7372 630d 0a70 6163 6b61   ...= src..packa
-00000280: 6765 7320 3d20 6669 6e64 3a0d 0a70 7974  ges = find:..pyt
-00000290: 686f 6e5f 7265 7175 6972 6573 203d 203e  hon_requires = >
-000002a0: 3d33 2e38 0d0a 696e 7374 616c 6c5f 7265  =3.8..install_re
-000002b0: 7175 6972 6573 203d 200d 0a09 6e75 6d70  quires = ...nump
-000002c0: 7920 3e3d 2031 2e35 0d0a 0970 7973 6964  y >= 1.5...pysid
-000002d0: 6532 203e 3d20 352e 3233 0d0a 0d0a 5b6f  e2 >= 5.23....[o
-000002e0: 7074 696f 6e73 2e70 6163 6b61 6765 732e  ptions.packages.
-000002f0: 6669 6e64 5d0d 0a77 6865 7265 203d 2073  find]..where = s
-00000300: 7263 0d0a 0d0a 5b6f 7074 696f 6e73 2e70  rc....[options.p
-00000310: 6163 6b61 6765 5f64 6174 615d 0d0a 2a20  ackage_data]..* 
-00000320: 3d20 2a2e 6373 762c 202a 2e6a 736f 6e2c  = *.csv, *.json,
-00000330: 202a 2e73 7667 2c20 2a2e 6d64 2c20 2a4c   *.svg, *.md, *L
-00000340: 4943 454e 5345 0d0a 0d0a 5b6f 7074 696f  ICENSE....[optio
-00000350: 6e73 2e65 6e74 7279 5f70 6f69 6e74 735d  ns.entry_points]
-00000360: 0d0a 636f 6e73 6f6c 655f 7363 7269 7074  ..console_script
-00000370: 7320 3d20 0d0a 0953 5441 5253 203d 2073  s = ...STARS = s
-00000380: 7461 7273 2e73 6275 6d69 7073 3a72 756e  tars.sbumips:run
-00000390: 0d0a 0d0a 5b65 6767 5f69 6e66 6f5d 0d0a  ....[egg_info]..
-000003a0: 7461 675f 6275 696c 6420 3d20 0d0a 7461  tag_build = ..ta
-000003b0: 675f 6461 7465 203d 2030 0d0a 0d0a       g_date = 0....
+00000050: 3d20 6a61 736f 6e2e 6f73 6f72 696f 6d61  = jason.osorioma
+00000060: 7269 6e40 6373 2e73 746f 6e79 6272 6f6f  rin@cs.stonybroo
+00000070: 6b2e 6564 750d 0a64 6573 6372 6970 7469  k.edu..descripti
+00000080: 6f6e 203d 2053 5441 5253 2028 5374 6f6e  on = STARS (Ston
+00000090: 7920 4272 6f6f 6b20 4173 7365 6d62 6c65  y Brook Assemble
+000000a0: 7220 616e 6420 5275 6e2d 7469 6d65 2053  r and Run-time S
+000000b0: 696d 756c 6174 6f72 2920 6973 2061 204d  imulator) is a M
+000000c0: 4950 5320 4173 7365 6d62 6c79 2073 696d  IPS Assembly sim
+000000d0: 756c 6174 6f72 206d 6164 6520 666f 7220  ulator made for 
+000000e0: 7468 6520 7075 7270 6f73 6520 6f66 2065  the purpose of e
+000000f0: 6475 6361 7469 6f6e 2e0d 0a6c 6f6e 675f  ducation...long_
+00000100: 6465 7363 7269 7074 696f 6e20 3d20 6669  description = fi
+00000110: 6c65 3a20 5245 4144 4d45 2e6d 640d 0a6c  le: README.md..l
+00000120: 6f6e 675f 6465 7363 7269 7074 696f 6e5f  ong_description_
+00000130: 636f 6e74 656e 745f 7479 7065 203d 2074  content_type = t
+00000140: 6578 742f 6d61 726b 646f 776e 0d0a 7572  ext/markdown..ur
+00000150: 6c20 3d20 6874 7470 733a 2f2f 6769 7468  l = https://gith
+00000160: 7562 2e63 6f6d 2f73 6275 7374 6172 732f  ub.com/sbustars/
+00000170: 5354 4152 530d 0a70 726f 6a65 6374 5f75  STARS..project_u
+00000180: 726c 7320 3d20 0d0a 0942 7567 2054 7261  rls = ...Bug Tra
+00000190: 636b 6572 203d 2068 7474 7073 3a2f 2f67  cker = https://g
+000001a0: 6974 6875 622e 636f 6d2f 7362 7573 7461  ithub.com/sbusta
+000001b0: 7273 2f53 5441 5253 2f69 7373 7565 730d  rs/STARS/issues.
+000001c0: 0a63 6c61 7373 6966 6965 7273 203d 200d  .classifiers = .
+000001d0: 0a09 5072 6f67 7261 6d6d 696e 6720 4c61  ..Programming La
+000001e0: 6e67 7561 6765 203a 3a20 5079 7468 6f6e  nguage :: Python
+000001f0: 203a 3a20 330d 0a09 4c69 6365 6e73 6520   :: 3...License 
+00000200: 3a3a 204f 5349 2041 7070 726f 7665 6420  :: OSI Approved 
+00000210: 3a3a 204d 4954 204c 6963 656e 7365 0d0a  :: MIT License..
+00000220: 094f 7065 7261 7469 6e67 2053 7973 7465  .Operating Syste
+00000230: 6d20 3a3a 204f 5320 496e 6465 7065 6e64  m :: OS Independ
+00000240: 656e 740d 0a0d 0a5b 6f70 7469 6f6e 735d  ent....[options]
+00000250: 0d0a 696e 636c 7564 655f 7061 636b 6167  ..include_packag
+00000260: 655f 6461 7461 203d 2054 7275 650d 0a70  e_data = True..p
+00000270: 6163 6b61 6765 5f64 6972 203d 200d 0a09  ackage_dir = ...
+00000280: 3d20 7372 630d 0a70 6163 6b61 6765 7320  = src..packages 
+00000290: 3d20 6669 6e64 3a0d 0a70 7974 686f 6e5f  = find:..python_
+000002a0: 7265 7175 6972 6573 203d 203e 3d33 2e38  requires = >=3.8
+000002b0: 0d0a 696e 7374 616c 6c5f 7265 7175 6972  ..install_requir
+000002c0: 6573 203d 200d 0a09 6e75 6d70 7920 3e3d  es = ...numpy >=
+000002d0: 2031 2e35 0d0a 0970 7973 6964 6536 203e   1.5...pyside6 >
+000002e0: 3d20 362e 342e 320d 0a0d 0a5b 6f70 7469  = 6.4.2....[opti
+000002f0: 6f6e 732e 7061 636b 6167 6573 2e66 696e  ons.packages.fin
+00000300: 645d 0d0a 7768 6572 6520 3d20 7372 630d  d]..where = src.
+00000310: 0a0d 0a5b 6f70 7469 6f6e 732e 7061 636b  ...[options.pack
+00000320: 6167 655f 6461 7461 5d0d 0a2a 203d 202a  age_data]..* = *
+00000330: 2e63 7376 2c20 2a2e 6a73 6f6e 2c20 2a2e  .csv, *.json, *.
+00000340: 7376 672c 202a 2e6d 642c 202a 4c49 4345  svg, *.md, *LICE
+00000350: 4e53 450d 0a0d 0a5b 6f70 7469 6f6e 732e  NSE....[options.
+00000360: 656e 7472 795f 706f 696e 7473 5d0d 0a63  entry_points]..c
+00000370: 6f6e 736f 6c65 5f73 6372 6970 7473 203d  onsole_scripts =
+00000380: 200d 0a09 5354 4152 5320 3d20 7374 6172   ...STARS = star
+00000390: 732e 7362 756d 6970 733a 7275 6e0d 0a0d  s.sbumips:run...
+000003a0: 0a5b 6567 675f 696e 666f 5d0d 0a74 6167  .[egg_info]..tag
+000003b0: 5f62 7569 6c64 203d 200d 0a74 6167 5f64  _build = ..tag_d
+000003c0: 6174 6520 3d20 300d 0a0d 0a              ate = 0....
```

### Comparing `STARSimulator-1.0.3/src/STARSimulator.egg-info/PKG-INFO` & `STARSimulator-1.0.5/src/STARSimulator.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 Metadata-Version: 2.1
 Name: STARSimulator
-Version: 1.0.3
+Version: 1.0.5
 Summary: STARS (Stony Brook Assembler and Run-time Simulator) is a MIPS Assembly simulator made for the purpose of education.
 Home-page: https://github.com/sbustars/STARS
 Author: STARS
-Author-email: stars@cs.stonybrook.edu
+Author-email: jason.osoriomarin@cs.stonybrook.edu
 Project-URL: Bug Tracker, https://github.com/sbustars/STARS/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # The STARS Code Repository
 
 ## Overview
 This repository hosts the public releases of STARS (Stony Brook Assembler and Run-time Simulator). STARS is a MIPS Assembly simulator made for the purpose of education.
 
 ## Dependencies
-* PySide2 (v5.15 or newer)
+* PySide6 (v6.4 or newer)
 * numpy (v1.23 or newer for Windows)
 
 # How to run:
 Install the package.
 ```
 $ pip install STARSimulator
 ```
```

### Comparing `STARSimulator-1.0.3/src/STARSimulator.egg-info/SOURCES.txt` & `STARSimulator-1.0.5/src/STARSimulator.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -25,33 +25,43 @@
 src/stars/gui/syntaxhighlighter.py
 src/stars/gui/textedit.py
 src/stars/gui/theme.py
 src/stars/gui/vt100.py
 src/stars/gui/widgetfactory.py
 src/stars/gui/resources/__init__.py
 src/stars/gui/resources/assemble.svg
+src/stars/gui/resources/assemblewhite.svg
 src/stars/gui/resources/backstep.svg
+src/stars/gui/resources/backstepwhite.svg
 src/stars/gui/resources/help.svg
+src/stars/gui/resources/helpwhite.svg
 src/stars/gui/resources/new.svg
+src/stars/gui/resources/newwhite.svg
 src/stars/gui/resources/open.svg
+src/stars/gui/resources/openwhite.svg
 src/stars/gui/resources/pause.svg
+src/stars/gui/resources/pausewhite.svg
 src/stars/gui/resources/save.svg
+src/stars/gui/resources/savewhite.svg
 src/stars/gui/resources/start.svg
+src/stars/gui/resources/startwhite.svg
 src/stars/gui/resources/step.svg
+src/stars/gui/resources/stepwhite.svg
 src/stars/help/__init__.py
 src/stars/help/bugs.md
 src/stars/help/directives.csv
 src/stars/help/help.py
 src/stars/help/instruction_set (copy).csv
 src/stars/help/instruction_set.csv
 src/stars/help/instructions.csv
 src/stars/help/operand.csv
 src/stars/help/syscalls.csv
 src/stars/interpreter/__init__.py
 src/stars/interpreter/classes.py
+src/stars/interpreter/compiled_tester.py
 src/stars/interpreter/debugger.py
 src/stars/interpreter/exceptions.py
 src/stars/interpreter/instructions.py
 src/stars/interpreter/interpreter.py
 src/stars/interpreter/memory.py
 src/stars/interpreter/registers.py
 src/stars/interpreter/syscalls.py
```

### Comparing `STARSimulator-1.0.3/src/stars/LICENSE` & `STARSimulator-1.0.5/src/stars/LICENSE`

 * *Files identical despite different names*

### Comparing `STARSimulator-1.0.3/src/stars/README.md` & `STARSimulator-1.0.5/src/stars/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 This program is a MIPS Assembly simulator made for the purpose of education.
 ## Dependencies
-* PySide2 (v5.15 or newer)
+* PySide6 (v6.4 or newer)
 * numpy (v1.23 or newer for Windows)
 * opengl
 
 # How to run:
 Install the package.
 ```
 $ pip install STARSimulator
```

### Comparing `STARSimulator-1.0.3/src/stars/constants.py` & `STARSimulator-1.0.5/src/stars/constants.py`

 * *Files 11% similar despite different names*

```diff
@@ -96,14 +96,15 @@
 REGISTER_HEADER = ["Name", "Value"]
 COPROC_FLAGS_HEADER = ["Condition", "Flags"]
 
 # PRESET MESSAGES
 PROGRAM_FINISHED = "\n-- program is finished running --\n\n"
 OPEN_FILE_FAILED = 'Could not open file\n'
 INSTRUCTION_COUNT = "Instruction Count: {}\t\t"
+ENTER_INTEGER = "Enter an integer\n"
 
 # For message in dialog for syscalls that require user input
 INPUT_MESSAGE = {
     "int": "Enter an integer",
     "str": "Enter a string"
 }
 INPUT_LABEL = "Value"
@@ -114,67 +115,75 @@
 TOOLBAR_ICON_SIZE = 24
 MENU_BAR = {
     'File': {
         'New': {
             'Shortcut': 'Ctrl+N',
             'Action': 'self.new_tab',
             'Icon': os.path.join(current_path, 'gui/resources/new.svg'),
+            'IconWhite': os.path.join(current_path, 'gui/resources/newwhite.svg'),
         },
         'Open': {
             'Shortcut': 'Ctrl+O',
             'Action': 'self.open_file',
             'Icon': os.path.join(current_path, 'gui/resources/open.svg'),
+            'IconWhite': os.path.join(current_path, 'gui/resources/openwhite.svg'),
         },
         'Close': {
             'Shortcut': 'Ctrl+W',
             'Action': 'self.close_tab',
             'Tag': 'close',
             'Start': False,
         },
         'Save': {
             'Shortcut': 'Ctrl+S',
             'Action': 'self.save_file',
             'Icon': os.path.join(current_path, 'gui/resources/save.svg'),
+            'IconWhite': os.path.join(current_path, 'gui/resources/savewhite.svg'),
             'Tag': 'save',
             'Start': False,
         }
     },
     'Run': {
         'Assemble': {
             'Shortcut': 'F3',
             'Action': 'self.assemble',
             'Icon': os.path.join(current_path, 'gui/resources/assemble.svg'),
+            'IconWhite': os.path.join(current_path, 'gui/resources/assemblewhite.svg'),
             'Tag': 'assemble',
             'Start': False,
         },
         'Start': {
             'Shortcut': 'F5',
             'Action': 'self.start',
             'Icon': os.path.join(current_path, 'gui/resources/start.svg'),
+            'IconWhite': os.path.join(current_path, 'gui/resources/startwhite.svg'),
             'Tag': 'start',
             'Start': False,
         },
         'Step': {
             'Shortcut': 'F7',
             'Action': 'self.step',
             'Icon': os.path.join(current_path, 'gui/resources/step.svg'),
+            'IconWhite': os.path.join(current_path, 'gui/resources/stepwhite.svg'),
             'Tag': 'step',
             'Start': False,
         },
         'Backstep': {
             'Shortcut': 'F8',
             'Action': 'self.reverse',
             'Icon': os.path.join(current_path, 'gui/resources/backstep.svg'),
+            'IconWhite': os.path.join(current_path, 'gui/resources/backstepwhite.svg'),
             'Tag': 'backstep',
             'Start': False,
         },
         'Pause': {
             'Shortcut': 'F9',
             'Action': 'self.pause',
             'Icon': os.path.join(current_path, 'gui/resources/pause.svg'),
+            'IconWhite': os.path.join(current_path, 'gui/resources/pausewhite.svg'),
             'Tag': 'pause',
             'Start': False,
         }
     },
     'Settings': {
         'Garbage Memory': {
             'Checkbox': 'garbage_memory'
@@ -202,14 +211,15 @@
         }
     },
     'Help': {
         'Help': {
             'Action': 'self.help',
             'Shortcut': 'F1',
             'Icon': os.path.join(current_path, 'gui/resources/help.svg'),
+            'IconWhite': os.path.join(current_path, 'gui/resources/helpwhite.svg'),
         }
     }
 }
 
 # Highlighter Patterns
 patterns = [MipsLexer.LOADS_F, MipsLexer.R_TYPE3_F, MipsLexer.R_TYPE2_F, MipsLexer.COMPARE_F, MipsLexer.BRANCH_F, MipsLexer.CONVERT_F,
             MipsLexer.MOVE_BTWN_F, MipsLexer.MOVE_F, MipsLexer.MOVE_COND_F, MipsLexer.R_TYPE3, MipsLexer.R_TYPE2, MipsLexer.MOVE,
```

### Comparing `STARSimulator-1.0.3/src/stars/controller.py` & `STARSimulator-1.0.5/src/stars/controller.py`

 * *Files identical despite different names*

### Comparing `STARSimulator-1.0.3/src/stars/gui/mainwindow.py` & `STARSimulator-1.0.5/src/stars/gui/mainwindow.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-from PySide2.QtWidgets import *
-from PySide2.QtGui import QBrush, QCloseEvent, QColor, QCursor, QGuiApplication, QIcon, QPalette
-from PySide2.QtCore import Qt, QSemaphore, Signal, QFile, QSize, QStringListModel
+from PySide6.QtWidgets import *
+from PySide6.QtGui import QBrush, QCloseEvent, QColor, QCursor, QGuiApplication, QIcon, QPalette, QAction
+from PySide6.QtCore import Qt, QSemaphore, Signal, QFile, QSize, QStringListModel
 from help.help import HelpWindow
 from gui.widgetfactory import *
 from gui.theme import ThemePicker
 from gui.textedit import TextEdit
 from gui.vt100 import VT100
 from controller import Controller
 from settings import settings
@@ -55,14 +55,15 @@
 
         self.console_sem = QSemaphore(1)
         self.mem_sem = QSemaphore(1)
         self.run_sem = QSemaphore(1)
         self.running = False
         self.result = None
         self.intr = None
+        self.help_window = None
 
         self.rep = MEMORY_REPR_DEFAULT
 
         # load json for user preferences
         with open(PREFERENCES_PATH) as f:
             self.preferences = json.load(f)
         self.get_theme(theme=self.preferences["on_start_theme"])
@@ -84,21 +85,21 @@
         self.update_theme()
 
     def update_button_status(self, **button_status: Dict[str, bool]) -> None:
         for tag, status in button_status.items():
             self.menu_items[tag].setEnabled(status)
 
     def init_menubar(self) -> None:
-        bar = self.menuBar()
+        self.bar = self.menuBar()
         self.menu_items = {}
 
-        toolbar = self.addToolBar("ToolBar")
-        toolbar.setIconSize(QSize(TOOLBAR_ICON_SIZE, TOOLBAR_ICON_SIZE))
+        self.toolbar = self.addToolBar("ToolBar")
+        self.toolbar.setIconSize(QSize(TOOLBAR_ICON_SIZE, TOOLBAR_ICON_SIZE))
         for tabs, values in MENU_BAR.items():
-            tab = bar.addMenu(tabs)
+            tab = self.bar.addMenu(tabs)
             if tabs == 'Settings':
                 tab.triggered.connect(lambda selection: self.controller.setSetting(
                     selection.data(), selection.isChecked()))
             for option, controls in values.items():
                 action = QAction(option, self)
                 if 'Checkbox' in controls:
                     action.setCheckable(True)
@@ -110,21 +111,21 @@
                     action.setShortcut(controls['Shortcut'])
                 if 'Tag' in controls:
                     self.menu_items[controls['Tag']] = action
                 if 'Start' in controls:
                     action.setEnabled(controls['Start'])
                 if 'Icon' in controls:
                     action.setIcon(QIcon(controls['Icon']))
-                    toolbar.addAction(action)
+                    self.toolbar.addAction(action)
                 tab.addAction(action)
             if 'Icon' in controls:
-                toolbar.addSeparator()
+                self.toolbar.addSeparator()
 
         self.instr_count = QLabel(INSTRUCTION_COUNT.format(0))
-        bar.setCornerWidget(self.instr_count)
+        self.bar.setCornerWidget(self.instr_count)
 
     def init_instrs(self) -> None:
         self.instrs = []
         self.pcs = []
         self.instr_grid = create_table(
             0, len(INSTR_HEADER), INSTR_HEADER, stretch_last=True)
         self.instr_grid.resizeColumnsToContents()
@@ -286,27 +287,70 @@
             [f'{obj}{{{";".join([f"{attr}: {value}" for attr, value in values.items()])}}}'
              for obj, values in get_theme_attribute(choice, 'Stylesheet').items()])
         self.textedit_theme = {
             "Editor": get_theme_attribute(choice, "Editor"),
             "Highlighter": get_theme_attribute(choice, "Highlighter")
         }  # for text editor theme
 
+    def update_toolbar_theme(self) -> None:
+        self.toolbar.clear()
+        self.bar.clear()
+
+        self.menu_items = {}
+        for tabs, values in MENU_BAR.items():
+            tab = self.bar.addMenu(tabs)
+            if tabs == 'Settings':
+                tab.triggered.connect(lambda selection: self.controller.setSetting(
+                    selection.data(), selection.isChecked()))
+            for option, controls in values.items():
+                action = QAction(option, self)
+                if 'Checkbox' in controls:
+                    action.setCheckable(True)
+                    action.setData(controls['Checkbox'])
+                    action.setChecked(settings[controls['Checkbox']])
+                if 'Action' in controls:
+                    action.triggered.connect(eval(controls['Action']))
+                if 'Shortcut' in controls:
+                    action.setShortcut(controls['Shortcut'])
+                if 'Tag' in controls:
+                    self.menu_items[controls['Tag']] = action
+                if 'Start' in controls:
+                    action.setEnabled(controls['Start'])
+                if self.theme != "default_theme":
+                    if 'IconWhite' in controls:
+                        action.setIcon(QIcon(controls['IconWhite']))
+                        self.toolbar.addAction(action)
+                else:
+                    if 'Icon' in controls:
+                        action.setIcon(QIcon(controls['Icon']))
+                        self.toolbar.addAction(action)
+                tab.addAction(action)
+            if self.theme != "default_theme":
+                if 'IconWhite' in controls:
+                    self.toolbar.addSeparator()
+            else:
+                if 'Icon' in controls:
+                    self.toolbar.addSeparator()
+
     def change_theme(self) -> None:
         if self.theme == "default_theme":
             self.get_theme(theme="dark_theme")
         else:
             self.get_theme()
         self.update_theme()
+        self.update_toolbar_theme()
 
     def edit_theme(self) -> None:
         ThemePicker(self, self.preferences).show()
 
     def update_theme(self) -> None:
         self.app.setPalette(self.palette)
         self.setStyleSheet(self.style_sheet)
+        if self.help_window != None:
+            self.help_window.update_theme()
         if hasattr(self, 'prev_instr'):
             for section in self.prev_instr:
                 section.setBackground(QBrush(QColor(self.high_light)))
         for i in range(self.file_count):
             self.tabs.widget(i).set_theme(self.textedit_theme)
 
     def open_file(self) -> None:
@@ -425,14 +469,15 @@
             self.fill_labels()
             self.intr.step.connect(self.update_screen)
             self.intr.console_out.connect(self.update_console)
             self.intr.user_input.connect(self.get_input)
             self.intr.end.connect(self.set_running)
             self.update_button_status(
                 start=True, step=True, backstep=True, pause=True)
+            self.intr.printWarnings()
 
         except Exception as e:
             print(traceback.format_exc())
             self.update_console(f"{type(e).__name__}: {str(e)}")
 
     def set_running(self, run: bool) -> None:
         self.run_sem.acquire()
@@ -522,16 +567,17 @@
         else:
             mem = self.intr.mem
             self.instr_grid.setRowCount(
                 len([k for k, j in mem.text.items() if type(j) is not str]))
             for count, (k, i) in enumerate(mem.text.items()):
                 if type(i) is not str:
                     cell, check = create_breakpoint()
-                    check.stateChanged.connect(lambda state, i=i: self.add_breakpoint(('b', str(i.filetag.file_name)[1:-1], str(i.filetag.line_no))) if state == Qt.Checked
+                    check.stateChanged.connect(lambda state, i=i: self.add_breakpoint(('b', str(i.filetag.file_name)[1:-1], str(i.filetag.line_no))) if state == 2  # 2 is enum for checked state
                                                else self.remove_breakpoint((str(i.filetag.file_name)[1:-1], str(i.filetag.line_no))))
+
                     self.instr_grid.setCellWidget(count, 0, cell)
 
                     values = [WORD_HEX_FORMAT.format(int(k)),
                               f"{i}",
                               f"{i.filetag.line_no}: {i.original_text}"]
                     row = create_instruction(values, self.instr_grid, count)
                     self.instrs.append(row)
@@ -539,15 +585,20 @@
                 section.setBackground(QBrush(QColor(self.high_light)))
             self.prev_instr = self.instrs[0]
 
     def fill_mem(self) -> None:
         self.mem_sem.acquire()
         if self.controller.good():
             for q, count in zip(self.mem_vals, range(self.base_address, self.base_address+MEMORY_SIZE, MEMORY_WIDTH)):
-                memory_format = MEMORY_REPR[self.rep]
+                if (self.rep == MEMORY_REPR_DEFAULT):
+                    memory_format = MEMORY_REPR[MEMORY_REPR_DEFAULT]
+                else:
+                    memory_format = MEMORY_REPR[list(
+                        MEMORY_REPR.keys())[self.rep]]
+
                 signed = True if self.rep == "ASCII" else False
                 offsets = range(MEMORY_WIDTH)[::-1]  # [3,2,1,0]
                 byte_value = [self.controller.get_byte(
                     count+i, signed=signed) for i in offsets]
                 if self.rep == "ASCII":
                     byte_value = [to_ascii(value) for value in byte_value]
                 text = " ".join([memory_format.format(value)
@@ -574,15 +625,15 @@
                               lambda state=None, addr=addr: self.mem_move_to(addr))
             self.labels.setCellWidget(i, 0, q)
             self.labels.setItem(i, 1, QTableWidgetItem(f'{l}'))
             self.labels.setItem(i, 2, QTableWidgetItem(
                 WORD_HEX_FORMAT.format(addr)))
 
     def change_section(self, t: str) -> None:
-        self.base_address = MEMORY_SECTION[t]
+        self.base_address = MEMORY_SECTION[list(MEMORY_SECTION.keys())[t]]
         self.fill_mem()
 
     def mem_move_to(self, addr: int) -> None:
         self.mem_sem.acquire()
         # 0x100-1 -> 0xff (multiple of MEMORY_SIZE)
         self.base_address = addr & ~(MEMORY_SIZE-1)
         self.mem_sem.release()
@@ -611,26 +662,33 @@
         self.console_sem.acquire()
         if clear:
             self.out.clear()
         self.out.insertPlainText(s)
         self.console_sem.release()
 
     def get_input(self, input_type: str) -> None:
-        value, state = QInputDialog.getInt(self,
-                                           INPUT_MESSAGE[USER_INPUT_TYPE[input_type]], INPUT_LABEL)
+        value, state = QInputDialog.getText(self,
+                                            INPUT_MESSAGE[USER_INPUT_TYPE[input_type]], INPUT_LABEL)
         if state:
-            self.intr.set_input(value)
+            if input_type == 0:
+                self.intr.set_input(value)
+            else:
+                if value.isnumeric():
+                    self.intr.set_input(int(value))
+                else:
+                    self.update_console(ENTER_INTEGER)
+                    self.get_input(input_type)
         else:
             self.get_input(input_type)
 
     def add_breakpoint(self, cmd: Tuple[str, str, str]) -> None:
         self.controller.add_breakpoint(cmd)
 
     def remove_breakpoint(self, cmd: Tuple[str, str]) -> None:
-        self.controller.remove_breakpoint((f'"{cmd[1]}"', cmd[2]))
+        self.controller.remove_breakpoint((f'"{cmd[0]}"', cmd[1]))
 
     def search(self, text: str) -> None:
         '''Highlight text that matches the provided text in the current widget.'''
         if self.tabs.currentWidget() is not None:
             self.tabs.currentWidget().search(text)
 
     def select_next(self) -> None:
@@ -640,12 +698,12 @@
 
     def launch_vt100(self) -> None:
         if self.vt100:
             self.vt100.close()
         self.vt100 = VT100(self.controller, self.changed_interp)
 
     def help(self):
-        self.window = HelpWindow(self)
+        self.help_window = HelpWindow(self)
 
 
 if __name__ == "__main__":
     launch_gui()
```

### Comparing `STARSimulator-1.0.3/src/stars/gui/resources/assemble.svg` & `STARSimulator-1.0.5/src/stars/gui/resources/assemble.svg`

 * *Files identical despite different names*

### Comparing `STARSimulator-1.0.3/src/stars/gui/resources/backstep.svg` & `STARSimulator-1.0.5/src/stars/gui/resources/backstep.svg`

 * *Files identical despite different names*

### Comparing `STARSimulator-1.0.3/src/stars/gui/resources/help.svg` & `STARSimulator-1.0.5/src/stars/gui/resources/help.svg`

 * *Files identical despite different names*

### Comparing `STARSimulator-1.0.3/src/stars/gui/resources/new.svg` & `STARSimulator-1.0.5/src/stars/gui/resources/new.svg`

 * *Files identical despite different names*

### Comparing `STARSimulator-1.0.3/src/stars/gui/resources/open.svg` & `STARSimulator-1.0.5/src/stars/gui/resources/open.svg`

 * *Files identical despite different names*

### Comparing `STARSimulator-1.0.3/src/stars/gui/resources/pause.svg` & `STARSimulator-1.0.5/src/stars/gui/resources/pause.svg`

 * *Files identical despite different names*

### Comparing `STARSimulator-1.0.3/src/stars/gui/resources/save.svg` & `STARSimulator-1.0.5/src/stars/gui/resources/save.svg`

 * *Files identical despite different names*

### Comparing `STARSimulator-1.0.3/src/stars/gui/resources/start.svg` & `STARSimulator-1.0.5/src/stars/gui/resources/start.svg`

 * *Files identical despite different names*

### Comparing `STARSimulator-1.0.3/src/stars/gui/resources/step.svg` & `STARSimulator-1.0.5/src/stars/gui/resources/step.svg`

 * *Files identical despite different names*

### Comparing `STARSimulator-1.0.3/src/stars/gui/syntaxhighlighter.py` & `STARSimulator-1.0.5/src/stars/gui/syntaxhighlighter.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-from PySide2.QtGui import QSyntaxHighlighter, QTextCharFormat, QFont, QColor
-from PySide2.QtCore import Qt, QRegularExpression, QRegularExpressionMatchIterator
+from PySide6.QtGui import QSyntaxHighlighter, QTextCharFormat, QFont, QColor
+from PySide6.QtCore import Qt, QRegularExpression, QRegularExpressionMatchIterator
 
 from constants import PATTERN_EXPRESSIONS
 
 
 class HighlightingRule:
     def __init__(self, name, pattern, format):
         self.type = name
```

### Comparing `STARSimulator-1.0.3/src/stars/gui/textedit.py` & `STARSimulator-1.0.5/src/stars/gui/textedit.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-from PySide2.QtWidgets import QPlainTextEdit, QTextEdit, QCompleter, QMainWindow, QAction, QApplication, QTabWidget, QFileDialog, QPushButton, QWidget
-from PySide2.QtGui import QKeySequence, QTextCursor, QFocusEvent, QKeyEvent, QGuiApplication, QCursor, QPainter, QColor, QTextFormat
-from PySide2.QtCore import Qt, QFile, QStringListModel, QSize, QRect
+from PySide6.QtWidgets import QPlainTextEdit, QTextEdit, QCompleter, QMainWindow, QApplication, QTabWidget, QFileDialog, QPushButton, QWidget
+from PySide6.QtGui import QAction, QKeySequence, QTextCursor, QFocusEvent, QKeyEvent, QGuiApplication, QCursor, QPainter, QColor, QTextFormat
+from PySide6.QtCore import Qt, QFile, QStringListModel, QSize, QRect
 from lexer import MipsLexer
 from gui.syntaxhighlighter import Highlighter
 
 from os import pathsep
 
 '''
 Line Number Code Editor adapted from https://doc.qt.io/qt-5/qtwidgets-widgets-codeeditor-example.html
@@ -51,15 +51,15 @@
         self.updateRequest.connect(self.updateLineNumberArea)
         self.cursorPositionChanged.connect(self.highlightCurrentLine)
         self.updateLineNumberAreaWidth(0)
         self.highlightCurrentLine()
 
     def lineNumberAreaWidth(self):
         max_value = max(1, self.blockCount())
-        space = 5 + self.fontMetrics().width('9') * len(str(max_value))
+        space = 5 + self.fontMetrics().horizontalAdvance('9') * len(str(max_value))
         return space
 
     def updateLineNumberAreaWidth(self, _):
         self.setViewportMargins(self.lineNumberAreaWidth(), 0, 0, 0)
 
     def updateLineNumberArea(self, rect, dy):
         if dy:
@@ -101,15 +101,15 @@
         bottom = top + self.blockBoundingRect(block).height()
         height = self.fontMetrics().height()
         while block.isValid() and (top <= event.rect().bottom()):
             if block.isVisible() and (bottom >= event.rect().top()):
                 number = str(blockNumber + 1)
                 painter.setPen(QColor(self.theme.get("Line_number", "black")))
                 painter.drawText(
-                    0, top, self.lineNumberArea.width(), height, Qt.AlignRight, number)
+                    -self.lineNumberArea.width()/5, top, self.lineNumberArea.width(), height, Qt.AlignRight, number)
 
             block = block.next()
             top = bottom
             bottom = top + self.blockBoundingRect(block).height()
             blockNumber += 1
 
     def setCompleter(self, completer: QCompleter) -> None:
```

### Comparing `STARSimulator-1.0.3/src/stars/gui/theme.py` & `STARSimulator-1.0.5/src/stars/gui/theme.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from gui.widgetfactory import create_box_layout, create_button, create_dropdown, create_widget
 from constants import *
-from PySide2.QtWidgets import *
-from PySide2.QtGui import QCloseEvent
+from PySide6.QtWidgets import *
+from PySide6.QtGui import QCloseEvent
 from copy import deepcopy
 import json
 import os
 import sys
 from typing import Dict, Union
 
 # must be ran in sbumips directory (this is bc PYTHONPATH is weird in terminal)
```

### Comparing `STARSimulator-1.0.3/src/stars/gui/vt100.py` & `STARSimulator-1.0.5/src/stars/gui/vt100.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-from PySide2.QtCore import Signal
-from PySide2.QtGui import QFont
-from PySide2.QtWidgets import *
+from PySide6.QtCore import Signal
+from PySide6.QtGui import QFont
+from PySide6.QtWidgets import *
 
 from controller import Controller
 
 '''
 https://github.com/sbustars/STARS
 
 Copyright 2020 Kevin McDonnell, Jihu Mun, and Ian Peitzsch
```

### Comparing `STARSimulator-1.0.3/src/stars/gui/widgetfactory.py` & `STARSimulator-1.0.5/src/stars/gui/widgetfactory.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from typing import Callable, List, Tuple, Union
 
-from PySide2.QtCore import Qt
-from PySide2.QtGui import QFont
-from PySide2.QtWidgets import *
+from PySide6.QtCore import Qt
+from PySide6.QtGui import QFont
+from PySide6.QtWidgets import *
 
 from constants import *
 
 
 def create_breakpoint(text="") -> Union[QWidget, QCheckBox]:
     '''Returns a checkbox, with the given text, centered inside of a widget.'''
     cell = QWidget()
@@ -83,15 +83,15 @@
     return button
 
 
 def create_dropdown(items: List[str], select_function: Callable[..., None] = None) -> QComboBox:
     '''Returns a dropdown that calls the provided function when an item is selected.'''
     dropdown = QComboBox()
     dropdown.addItems(items)
-    dropdown.activated["QString"].connect(select_function)
+    dropdown.activated[int].connect(select_function)
 
     return dropdown
 
 
 def create_widget(layout: QLayout = None) -> QWidget:
     '''Returns a widget with the given layout.'''
     widget = QWidget()
```

### Comparing `STARSimulator-1.0.3/src/stars/help/directives.csv` & `STARSimulator-1.0.5/src/stars/help/directives.csv`

 * *Files identical despite different names*

### Comparing `STARSimulator-1.0.3/src/stars/help/help.py` & `STARSimulator-1.0.5/src/stars/help/help.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,67 +1,76 @@
+from gui.widgetfactory import create_box_layout, create_cell, create_table, create_widget
+from constants import HELP_TABS, HELP_TITLE
+from PySide6.QtWidgets import *
+from PySide6.QtCore import Qt
 import csv
-import os 
+import os
 from typing import List
 import sys
 
-sys.path.append(os.getcwd())  # must be ran in sbumips directory (this is bc PYTHONPATH is weird in terminal)
-from PySide2.QtCore import Qt
-from PySide2.QtWidgets import *
+# must be ran in sbumips directory (this is bc PYTHONPATH is weird in terminal)
+sys.path.append(os.getcwd())
 
-from constants import HELP_TABS, HELP_TITLE
-from gui.widgetfactory import create_box_layout, create_cell, create_table, create_widget
 
 def create_tab(rows: List[str], header: List[str]) -> QTableWidget:
     '''Returns a table with csv row values inserted.'''
     table = create_table(len(rows), len(rows[0]), header, stretch_last=True)
     for row, values in enumerate(rows):
         for i, text in enumerate(values):
-            table.setItem(row, i, create_cell((text.strip().replace('\\n', '\n'))))
+            table.setItem(row, i, create_cell(
+                (text.strip().replace('\\n', '\n'))))
     if not header:
         table.horizontalHeader().setVisible(False)
     table.resizeColumnsToContents()
     table.resizeRowsToContents()
 
     return table
 
+
 def create_search(table: QTableWidget) -> QWidget:
     def search_function(text: str) -> None:
         for row in range(table.rowCount()):
             column = table.item(row, 0)
             table.setRowHidden(row, not column.text().startswith(text))
     text_entry = QLineEdit()
     text_entry.textChanged.connect(search_function)
 
-    return create_widget(create_box_layout(direction=QBoxLayout.TopToBottom, 
-                    sections=[text_entry, table]))
+    return create_widget(create_box_layout(direction=QBoxLayout.TopToBottom,
+                                           sections=[text_entry, table]))
+
 
 class HelpWindow(QMainWindow):
-    
+
     def __init__(self, app):
         super().__init__()
+        self.app = app
         self.setWindowTitle(HELP_TITLE)
-        window = QTabWidget()
+        self.window = QTabWidget()
+        self.window.setStyleSheet(app.style_sheet)
         for name, properties in HELP_TABS.items():
             with open(properties['filename']) as f:
                 if properties['type'] == 'table':
                     rows = [row for row in csv.reader(f)]
                     table = create_tab(rows, properties.get('header', []))
-                    window.addTab(create_search(table), name)
+                    self.window.addTab(create_search(table), name)
                 elif properties['type'] == 'text':
                     text = QTextEdit()
                     text.setReadOnly(True)
                     text.setPlainText(f.read())
-                    window.addTab(text, name)
+                    self.window.addTab(text, name)
                 elif properties['type'] == 'markdown':
                     text = QTextEdit()
                     text.setReadOnly(True)
                     text.setMarkdown(f.read())
-                    window.addTab(text, name)
-        self.setCentralWidget(window)
-        
+                    self.window.addTab(text, name)
+        self.setCentralWidget(self.window)
+
         self.show()
         self.resize(1080, 480)
+    
+    def update_theme(self) -> None:
+        self.window.setStyleSheet(self.app.style_sheet)
 
 if __name__ == "__main__":
     app = QApplication()
     window = HelpWindow(app)
-    app.exec_()
+    app.exec_()
```

### Comparing `STARSimulator-1.0.3/src/stars/help/instruction_set (copy).csv` & `STARSimulator-1.0.5/src/stars/help/instruction_set (copy).csv`

 * *Files identical despite different names*

### Comparing `STARSimulator-1.0.3/src/stars/help/instruction_set.csv` & `STARSimulator-1.0.5/src/stars/help/instruction_set.csv`

 * *Files identical despite different names*

### Comparing `STARSimulator-1.0.3/src/stars/help/instructions.csv` & `STARSimulator-1.0.5/src/stars/help/instructions.csv`

 * *Files identical despite different names*

### Comparing `STARSimulator-1.0.3/src/stars/help/operand.csv` & `STARSimulator-1.0.5/src/stars/help/operand.csv`

 * *Files identical despite different names*

### Comparing `STARSimulator-1.0.3/src/stars/help/syscalls.csv` & `STARSimulator-1.0.5/src/stars/help/syscalls.csv`

 * *Files identical despite different names*

### Comparing `STARSimulator-1.0.3/src/stars/instruction_constants.py` & `STARSimulator-1.0.5/src/stars/instruction_constants.py`

 * *Files identical despite different names*

### Comparing `STARSimulator-1.0.3/src/stars/interpreter/classes.py` & `STARSimulator-1.0.5/src/stars/interpreter/classes.py`

 * *Files identical despite different names*

### Comparing `STARSimulator-1.0.3/src/stars/interpreter/debugger.py` & `STARSimulator-1.0.5/src/stars/interpreter/debugger.py`

 * *Files identical despite different names*

### Comparing `STARSimulator-1.0.3/src/stars/interpreter/exceptions.py` & `STARSimulator-1.0.5/src/stars/interpreter/exceptions.py`

 * *Files identical despite different names*

### Comparing `STARSimulator-1.0.3/src/stars/interpreter/instructions.py` & `STARSimulator-1.0.5/src/stars/interpreter/instructions.py`

 * *Files identical despite different names*

### Comparing `STARSimulator-1.0.3/src/stars/interpreter/interpreter.py` & `STARSimulator-1.0.5/src/stars/interpreter/interpreter.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,25 +2,26 @@
 import random
 import re
 import struct
 import sys
 from collections import OrderedDict
 from threading import Event, Lock
 
-from PySide2.QtCore import Signal
-from PySide2.QtWidgets import QWidget
+from PySide6.QtCore import *
+from PySide6 import QtWidgets
 from numpy import float32
 
 import constants as const
 from interpreter import exceptions as ex, instructions as instrs
 from interpreter.classes import *
 from interpreter.debugger import Debug
 from interpreter.memory import Memory
 from interpreter.registers import Registers
 from interpreter.syscalls import syscalls
+from interpreter.compiled_tester import check_function_uninit
 from settings import settings
 
 '''
 https://github.com/sbustars/STARS
 
 Copyright 2020 Kevin McDonnell, Jihu Mun, and Ian Peitzsch
 
@@ -32,15 +33,15 @@
 
 The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
 
 THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
 '''
 
 
-class Interpreter(QWidget):
+class Interpreter(QtWidgets.QWidget):
     step = Signal(int)  # use to signal program counter increment
     end = Signal(bool)  # use to signal program termination
     console_out = Signal(str)  # use by out for printing to console
     user_input = Signal(int)  # use by input/set_input for user input syscalls
 
     def __init__(self, code: List[Instruction], args: List[str]) -> None:
         if settings['gui']:
@@ -58,17 +59,19 @@
         self.handleArgs(args)
         self.initialize_memory(code)
         # For error messages
         self.line_info = ''
         self.debug = Debug()
         self.instruction_count = 0
         self.instr = None
+        self.warnings = []
+        self.checkWarnings()
 
     def initialize_memory(self, code: List[Instruction]) -> None:
-        '''Initialize memory by adding instructions to the data/text section 
+        '''Initialize memory by adding instructions to the data/text section
         and then replacing the labels with the correct address'''
         # Function control variables
         has_main = False
         comp = re.compile(r'(lb[u]?|lh[u]?|lw[lr]|lw|la|s[bhw]|sw[lr])')
         for line in code:  # Go through the source code line by line, adding declarations first
             if type(line) is Declaration:
                 self.set_data(line)
@@ -225,15 +228,14 @@
             while True:  # Get the next instruction and increment pc
                 pc = self.get_register('pc')
                 if str(pc) not in self.mem.text:
                     raise ex.MemoryOutOfBounds(f'{pc} is not a valid address')
                 if self.instruction_count > settings['max_instructions']:
                     raise ex.InstrCountExceed(
                         f'Exceeded maximum instruction count: {settings["max_instructions"]}')
-
                 self.instr = self.mem.text[str(pc)]
                 if self.instr == 'TERMINATE_EXECUTION':
                     if settings['gui']:
                         self.end.emit(False)
                     break
                 self.set_register('pc', self.get_register('pc')+4)
                 self.instruction_count += 1
@@ -272,14 +274,15 @@
         self.out(f"Registers:\n{self.reg.dump()}", end="\n")
         self.out('Memory:', end="\n")
         self.mem.dump()
 
     def out(self, s: str, end='') -> None:
         '''Prints to terminal or the console in the GUI'''
         if settings['gui']:
+            print(s)
             self.console_out.emit(f'{s}{end}')
         else:
             print(s, end=end)
 
     def get_input(self, input_type: str) -> str:
         '''Prompts the user for an input value.'''
         if settings['gui']:
@@ -300,7 +303,34 @@
 
     def reset(self) -> bool:
         '''Resets the program counter.'''
         if hasattr(self, 'orig_pc'):
             self.reg.set_register('pc', self.orig_pc)
             return True
         return False
+
+    def checkWarnings(self) -> None:
+        '''Statically checks all warnings for unitialized variables and hard coding register convention'''
+        func_code = []
+        label_name = "Unlabeled"
+        # print(self.mem.text)
+        for pc in self.mem.text:
+            if self.mem.text[pc] == "TERMINATE_EXECUTION":
+                warning_list = check_function_uninit(label_name, func_code)
+                if warning_list:
+                    self.warnings.extend(warning_list)
+                break
+            line = self.mem.text[pc]
+            # print(line)
+            if self.mem.getLabelAtAddr(int(pc)):
+                warning_list = check_function_uninit(label_name, func_code)
+                if warning_list:
+                    self.warnings.extend(warning_list)
+                label_name = self.mem.getLabelAtAddr(int(pc))
+                func_code = [line]
+            else:
+                func_code.append(line)
+
+    def printWarnings(self) -> None:
+        '''Prints the list of warnings to the user'''
+        for warning in self.warnings:
+            self.out("WARNING: " + warning, end='\n')
```

### Comparing `STARSimulator-1.0.3/src/stars/interpreter/memory.py` & `STARSimulator-1.0.5/src/stars/interpreter/memory.py`

 * *Files 2% similar despite different names*

```diff
@@ -41,15 +41,15 @@
     def __init__(self, toggle_garbage: bool = False):
         self.text = OrderedDict()  # Instructions
         self.data = OrderedDict()  # Main memory
         self.stack = OrderedDict()
 
         self.textPtr = settings['initial_pc']
         self.dataPtr = settings['data_min']
-        self.labels = {}  # Dictionary to store the labels and their addresses
+        self.labels = OrderedDict()  # Dictionary to store the labels and their addresses
 
         self.toggle_garbage = toggle_garbage
         self.fileTable = OrderedDict([(0, sys.stdin),
                                       (1, sys.stdout),
                                       (2, sys.stderr)])
         self.heapPtr = 0x10040000
 
@@ -219,14 +219,21 @@
         '''Return the data ptr address for the label if it exists, otherwise
         raise a InvalidLabel exception.'''
         if s in self.labels:
             return self.labels[s]
         else:
             raise ex.InvalidLabel(f'{s} is not a valid label.')
 
+    def getLabelAtAddr(self, addr: int) -> str:
+        label = None
+        for key, value in self.labels.items():
+            if value == addr:
+                label = key
+        return label
+
     def getString(self, label: str, n: int = 100) -> Union[str, None]:
         addr = self.getLabel(label)
 
         count = 0
         ret = ''
 
         c = self.getByte(addr, signed=False)
```

### Comparing `STARSimulator-1.0.3/src/stars/interpreter/registers.py` & `STARSimulator-1.0.5/src/stars/interpreter/registers.py`

 * *Files identical despite different names*

### Comparing `STARSimulator-1.0.3/src/stars/interpreter/syscalls.py` & `STARSimulator-1.0.5/src/stars/interpreter/syscalls.py`

 * *Files identical despite different names*

### Comparing `STARSimulator-1.0.3/src/stars/interpreter/utility.py` & `STARSimulator-1.0.5/src/stars/interpreter/utility.py`

 * *Files identical despite different names*

### Comparing `STARSimulator-1.0.3/src/stars/lexer.py` & `STARSimulator-1.0.5/src/stars/lexer.py`

 * *Files identical despite different names*

### Comparing `STARSimulator-1.0.3/src/stars/mipsParser.py` & `STARSimulator-1.0.5/src/stars/mipsParser.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 from constants import *
 from interpreter.interpreter import *
 from lexer import MipsLexer
 from sly.yacc import Parser
 
+import traceback
 '''
 https://github.com/sbustars/STARS
 
 Copyright 2020 Kevin McDonnell, Jihu Mun, and Ian Peitzsch
 
 Developed by Kevin McDonnell (ktm@cs.stonybrook.edu),
 Jihu Mun (jihu1011@gmail.com),
@@ -25,17 +26,19 @@
     return (x >> 16) & 0xFFFF
 
 
 class MipsParser(Parser):
     tokens = MipsLexer.tokens
     # debugfile = 'parser.out'
 
-    def __init__(self, original_text, filename):
+    def __init__(self, original_text, filename, processed_text=None):
         self.labels = {}
         self.original_text = original_text.split('\n')
+        self.processed_text = {k: processed_text[k].split(
+            '\n') for k in processed_text.keys()} if processed_text else None
         self.filename = filename
 
     # Top level section (Data, Text)
     @_('sects')
     def program(self, p):
         return p.sects
 
@@ -81,14 +84,22 @@
                 p.instr.instrs[i].original_text = p.instr.operation
                 p.instr.instrs[i].is_from_pseudoinstr = True
         else:
             p.instr.filetag = p.filetag
             p.instr.original_text = self.original_text[p.filetag.line_no-1]
             p.instr.is_from_pseudoinstr = False
 
+            if self.processed_text:
+                instr_text = self.processed_text[p.filetag.file_name.replace(
+                    '\"', '')][p.filetag.line_no - 1]
+                marker_idx = instr_text.find('\x81')
+                if marker_idx >= 0:
+                    instr_text = instr_text[:marker_idx]
+                p.instr.original_text = instr_text
+
         if 'label' in p._namemap:
             result.append(p.label)
 
         if 'instr' in p._namemap:
             result.append(p.instr)
 
         if 'instrs' in p._namemap:
```

### Comparing `STARSimulator-1.0.3/src/stars/preferences.json` & `STARSimulator-1.0.5/src/stars/preferences.json`

 * *Files 11% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.95491452991453%*

 * *Differences: {"'dark_theme'": "{'Editor': {'Line_number_box': '#50191919', 'Current_Line_Highlight': "*

 * *                 "'#30000000'}, 'Highlighter': OrderedDict([('keyword', OrderedDict([('color', "*

 * *                 "'#c2c2ff')])), ('label', OrderedDict([('color', '#b8b800'), ('font-weight', "*

 * *                 "75)])), ('number', OrderedDict([('color', '#70ff70')])), ('string', "*

 * *                 "OrderedDict([('color', '#8a8aff')])), ('directive', OrderedDict([('color', "*

 * *                 "'#ff33ff'), ('font-weight',  […]*

```diff
@@ -1,13 +1,38 @@
 {
     "dark_theme": {
         "Editor": {
-            "Current_Line_Highlight": "silver",
+            "Current_Line_Highlight": "#30000000",
             "Line_number": "white",
-            "Line_number_box": "silver"
+            "Line_number_box": "#50191919"
+        },
+        "Highlighter": {
+            "comment": {
+                "color": "#808080"
+            },
+            "directive": {
+                "color": "#ff33ff",
+                "font-weight": 75
+            },
+            "keyword": {
+                "color": "#c2c2ff"
+            },
+            "label": {
+                "color": "#b8b800",
+                "font-weight": 75
+            },
+            "number": {
+                "color": "#70ff70"
+            },
+            "registers": {
+                "color": "#ff0000"
+            },
+            "string": {
+                "color": "#8a8aff"
+            }
         },
         "Instruction_Highlight": "gray",
         "QPalette": {
             "QPalette.AlternateBase": "#3F3F3F",
             "QPalette.Base": "#353535",
             "QPalette.BrightText": "red",
             "QPalette.Button": "#353535",
@@ -53,17 +78,17 @@
                 "background-color": "#353535",
                 "border": "0"
             }
         }
     },
     "default_theme": {
         "Editor": {
-            "Current_Line_Highlight": "silver",
+            "Current_Line_Highlight": "#30808080",
             "Line_number": "black",
-            "Line_number_box": "silver"
+            "Line_number_box": "#30808080"
         },
         "Highlighter": {
             "comment": {
                 "color": "#808080"
             },
             "directive": {
                 "color": "#800080",
@@ -91,15 +116,15 @@
             "QPalette.AlternateBase": "#F7F7F7",
             "QPalette.Base": "#FFFFFF",
             "QPalette.BrightText": "#FFFFFF",
             "QPalette.Button": "#EFEFEF",
             "QPalette.ButtonText": "#000000",
             "QPalette.Highlight": "#308CC6",
             "QPalette.HighlightedText": "#FFFFFF",
-            "QPalette.Link": "#0000FF",
+            "QPalette.Link": "#8080ff",
             "QPalette.Text": "#000000",
             "QPalette.ToolTipBase": "#FFFFDC",
             "QPalette.ToolTipText": "#000000",
             "QPalette.Window": "#EFEFEF",
             "QPalette.WindowText": "#000000"
         },
         "Stylesheet": {
```

### Comparing `STARSimulator-1.0.3/src/stars/preprocess.py` & `STARSimulator-1.0.5/src/stars/preprocess.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import errno
 from typing import Tuple, Dict
 
 from constants import FILE_MARKER, LINE_MARKER
 from interpreter.exceptions import *
 from interpreter.interpreter import *
 from lexer import MipsLexer
 from settings import settings
@@ -39,27 +40,30 @@
 def walk(filename: Path, files: List[Path], eqv: Dict[str, str], abs_to_rel: Dict[Path, str], parent: Path) -> None:
     # Patterns to detect if line is an .eqv or .include directive
     eq_pattern = re.compile(r'[.]eqv (.*?)? (.*)')
     incl_pattern = re.compile(r'[.]include "(.*?)"')
 
     files.append(filename)
     line_count = 0
-
+    if not filename.name in os.listdir(filename.parents[0]):
+        raise FileNotFoundError(errno.ENOENT, os.strerror(errno.ENOENT), str(filename))
+    
     with filename.open(mode='r', errors='ignore') as f:
         for line in f.readlines():
             line_count += 1
 
             # Ignore comments
             line = line.split('#')[0]
 
             incl_match = incl_pattern.match(line)
             eq_match = eq_pattern.match(line)
 
             if eq_match:
                 original = eq_match.group(1)
+
                 substitution = eq_match.group(2)
 
                 if isValid(original):
                     eqv[rf'\b{original}\b'] = substitution
 
                 else:
                     raise InvalidEQV(f'{filename}: line {line_count}: {original} is a restricted word and cannot be replaced using eqv.')
@@ -136,8 +140,8 @@
     text = processed[files[0].as_posix()]
     for name, content in contents.items():
         if name in abs_to_rel:
             pattern = rf'\.include "{abs_to_rel[name]}".*?\n'
             og_text = re.sub(pattern, content, og_text)
             processed[name] = re.sub(r'\\', '\\\\\\\\', processed[name])
             text = re.sub(pattern, processed[name], text)
-    return (og_text, text)
+    return (og_text, text, processed)
```

### Comparing `STARSimulator-1.0.3/src/stars/sbumips.py` & `STARSimulator-1.0.5/src/stars/sbumips.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,27 +1,23 @@
+from pathlib import Path
+import argparse
+from gui import mainwindow
+from interpreter.interpreter import *
+from lexer import MipsLexer
+from mipsParser import MipsParser
+from preprocess import walk, link, preprocess
+from settings import settings
 import sys
 import os
 
 current_path = os.path.dirname(os.path.abspath(__file__))
-print(current_path)
 sys.path.append(current_path)
 sys.path.append(os.getcwd())
 
 
-from settings import settings
-from preprocess import walk, link, preprocess
-from mipsParser import MipsParser
-from lexer import MipsLexer
-from interpreter.interpreter import *
-from gui import mainwindow
-import argparse
-from pathlib import Path
-
-
-
 '''
 https://github.com/sbustars/STARS
 
 Copyright 2020 Kevin McDonnell, Jihu Mun, and Ian Peitzsch
 
 Developed by Kevin McDonnell (ktm@cs.stonybrook.edu),
 Jihu Mun (jihu1011@gmail.com),
@@ -76,54 +72,52 @@
     if args.max_instructions:
         settings['max_instructions'] = args.max_instructions
 
 
 def assemble(filename: str) -> List:
     path = Path(filename)
     path.resolve()
-
     files = []
     eqv_dict = {}
     abs_to_rel = {}
 
     walk(path, files, eqv_dict, abs_to_rel, path.parent)
     contents = {}
     results = {}
     processed = {}
     for file in files:
         with file.open() as f:
             s = f.readlines()
             file = file.as_posix()
-
             contents[file] = ''.join(s)
             processed[file] = preprocess(contents[file], file, eqv_dict)
-
             lexer = MipsLexer(file)
             parser = MipsParser(contents[file], file)
 
             tokenized = lexer.tokenize(processed[file])
             results[file] = parser.parse(tokenized)
     if settings['assemble']:
         print('Program assembled successfully.')
         exit()
-    og_text, text = link(files, contents, processed, abs_to_rel)
-    parser = MipsParser(og_text, files[0])
+    og_text, text, processed_text = link(
+        files, contents, processed, abs_to_rel)
+    parser = MipsParser(og_text, files[0], processed_text)
     lexer = MipsLexer(files[0].as_posix())
 
     t = lexer.tokenize(text)
     return parser.parse(t)
 
 
 def run_CLI(args: argparse.Namespace):
     pArgs = args.pa if args.pa else []
     try:
         result = assemble(args.filename)
         inter = Interpreter(result, pArgs)
+        inter.printWarnings()
         inter.interpret()
-
         if settings['disp_instr_count']:
             inter.out(f'\nInstruction count: {inter.instruction_count}')
 
     except Exception as e:
         print(f"{type(e).__name__}: {str(e)}", file=sys.stderr)
```

### Comparing `STARSimulator-1.0.3/src/stars/settings.py` & `STARSimulator-1.0.5/src/stars/settings.py`

 * *Files identical despite different names*

### Comparing `STARSimulator-1.0.3/src/stars/sly/lex.py` & `STARSimulator-1.0.5/src/stars/sly/lex.py`

 * *Files identical despite different names*

### Comparing `STARSimulator-1.0.3/src/stars/sly/yacc.py` & `STARSimulator-1.0.5/src/stars/sly/yacc.py`

 * *Files identical despite different names*

### Comparing `STARSimulator-1.0.3/src/stars/tests/classes/test_classes.py` & `STARSimulator-1.0.5/src/stars/tests/classes/test_classes.py`

 * *Files identical despite different names*

### Comparing `STARSimulator-1.0.3/src/stars/tests/controller/test_controller.py` & `STARSimulator-1.0.5/src/stars/tests/controller/test_controller.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,31 +5,34 @@
 from controller import Controller
 from interpreter.classes import Label
 from interpreter.debugger import Debug
 from interpreter.interpreter import Interpreter
 from interpreter.memory import Memory
 from interpreter.registers import Registers
 
+
 class TestController(unittest.TestCase):
-    
+
     def setUp(self):
         super().setUp()
         inter = Interpreter([Label('main')], [])
         self.controller = Controller(inter.debug, inter)
 
     def test_set_interpreter(self):
         '''
             Tests that the interpreter and debugger attributes are set properly.
         '''
         self.controller = Controller(None, None)
         inter = Interpreter([Label('main')], [])
         self.controller.set_interp(inter)
 
-        self.assertEqual(self.controller.interp, inter, f"The interpreter was not set correct.")
-        self.assertEqual(self.controller.debug, inter.debug, f"The debug object does not match the interpreter's debug object.")
+        self.assertEqual(self.controller.interp, inter,
+                         f"The interpreter was not set correct.")
+        self.assertEqual(self.controller.debug, inter.debug,
+                         f"The debug object does not match the interpreter's debug object.")
 
     @mock.patch.object(Event, "clear")
     def test_set_pause_false(self, mock_method: mock.patch.object):
         '''
             Tests that calling set pause false will call Event.clear().
         '''
         self.controller.set_pause(False)
@@ -62,15 +65,15 @@
     @mock.patch.object(Memory, "getByte")
     def test_get_byte(self, mock_method: mock.patch.object):
         '''
             Tests that calling getByte will call Memory.getByte().
         '''
         self.controller.get_byte(1)
         mock_method.assert_called_once()
-        
+
     @mock.patch.object(Debug, "addBreakpoint")
     def test_add_breakpoint(self, mock_method: mock.patch.object):
         '''
             Tests that calling add_breakpoint will call Debug.addBreakpoint().
         '''
         self.controller.add_breakpoint(["list", "of", "strings"])
         mock_method.assert_called_once()
@@ -91,51 +94,54 @@
         self.controller.reverse()
         mock_method.assert_called_once()
 
     def test_good(self):
         '''
             Tests that calling good will return True if interpreter is set.
         '''
-        self.assertTrue(self.controller.good(), "Interpreter should not be None.")
+        self.assertTrue(self.controller.good(),
+                        "Interpreter should not be None.")
         self.controller = Controller(None, None)
         self.assertFalse(self.controller.good(), "Interpreter should be None.")
 
     def test_cont(self):
         '''
             Tests that calling cont will return the value of Debug's continueFlag attribute.
         '''
-        self.assertEqual(self.controller.cont(), self.controller.debug.continueFlag, 
-            "The return value does not match the value of Debug's continueFlag attribute.")
+        self.assertEqual(self.controller.cont(), self.controller.debug.continueFlag,
+                         "The return value does not match the value of Debug's continueFlag attribute.")
 
     def test_set_setting(self):
         '''
             Tests that setting the value of warnings from False to True modifies the settings 
             dictionary.
         '''
         from settings import settings
         self.controller.setSetting("warnings", True)
-        self.assertTrue(settings['warnings'], "The warnings setting is not set to True from False.")
+        self.assertTrue(
+            settings['warnings'], "The warnings setting is not set to True from False.")
         settings["warnings"] = False
 
     def test_get_labels(self):
         '''
             Tests that calling get labels returns the labels of a blank interpreter. 
         '''
         labels = self.controller.get_labels()
 
-        self.assertEqual(len(labels), 1, "The number of labels is not equal to 1.")
+        self.assertEqual(
+            len(labels), 1, "The number of labels is not equal to 1.")
         self.assertIn('main', labels, "The only label in labels is main.")
 
     def test_get_instr_count(self):
         '''
             Tests that calling cont will return the value of Interpreter's instruction_count attribute.
         '''
-        self.assertEqual(self.controller.get_instr_count(), self.controller.interp.instruction_count, 
-            "The return value does not match the value of Interpreter's instruction_count attribute.")
+        self.assertEqual(self.controller.get_instr_count(), self.controller.interp.instruction_count,
+                         "The return value does not match the value of Interpreter's instruction_count attribute.")
 
     @mock.patch.object(Registers, "get_reg_word")
     def test_get_reg_word(self, mock_method: mock.patch.object):
         '''
             Tests that calling get_reg_word will call Debug.get_reg_word().
         '''
         self.controller.get_reg_word("$a0")
-        mock_method.assert_called_once()
+        mock_method.assert_called_once()
```

### Comparing `STARSimulator-1.0.3/src/stars/tests/debugger/test_debugger.py` & `STARSimulator-1.0.5/src/stars/tests/debugger/test_debugger.py`

 * *Files identical despite different names*

### Comparing `STARSimulator-1.0.3/src/stars/tests/debugger/test_debugger_stack.py` & `STARSimulator-1.0.5/src/stars/tests/debugger/test_debugger_stack.py`

 * *Files identical despite different names*

### Comparing `STARSimulator-1.0.3/src/stars/tests/fileOps/test_fileOps.py` & `STARSimulator-1.0.5/src/stars/tests/fileOps/test_fileOps.py`

 * *Files identical despite different names*

### Comparing `STARSimulator-1.0.3/src/stars/tests/floatInstrs/test.py` & `STARSimulator-1.0.5/src/stars/tests/floatInstrs/test.py`

 * *Files identical despite different names*

### Comparing `STARSimulator-1.0.3/src/stars/tests/instructions/instructions.py` & `STARSimulator-1.0.5/src/stars/tests/instructions/instructions.py`

 * *Files identical despite different names*

### Comparing `STARSimulator-1.0.3/src/stars/tests/instructions/test_add.py` & `STARSimulator-1.0.5/src/stars/tests/instructions/test_add.py`

 * *Files identical despite different names*

### Comparing `STARSimulator-1.0.3/src/stars/tests/instructions/test_addi.py` & `STARSimulator-1.0.5/src/stars/tests/instructions/test_addi.py`

 * *Files identical despite different names*

### Comparing `STARSimulator-1.0.3/src/stars/tests/instructions/test_addu.py` & `STARSimulator-1.0.5/src/stars/tests/instructions/test_addu.py`

 * *Files identical despite different names*

### Comparing `STARSimulator-1.0.3/src/stars/tests/instructions/test_and.py` & `STARSimulator-1.0.5/src/stars/tests/instructions/test_and.py`

 * *Files identical despite different names*

### Comparing `STARSimulator-1.0.3/src/stars/tests/instructions/test_beq.py` & `STARSimulator-1.0.5/src/stars/tests/instructions/test_beq.py`

 * *Files identical despite different names*

### Comparing `STARSimulator-1.0.3/src/stars/tests/instructions/test_bgez.py` & `STARSimulator-1.0.5/src/stars/tests/instructions/test_bgez.py`

 * *Files identical despite different names*

### Comparing `STARSimulator-1.0.3/src/stars/tests/instructions/test_bgezal.py` & `STARSimulator-1.0.5/src/stars/tests/instructions/test_bgezal.py`

 * *Files identical despite different names*

### Comparing `STARSimulator-1.0.3/src/stars/tests/instructions/test_bgtz.py` & `STARSimulator-1.0.5/src/stars/tests/instructions/test_bgtz.py`

 * *Files identical despite different names*

### Comparing `STARSimulator-1.0.3/src/stars/tests/instructions/test_blez.py` & `STARSimulator-1.0.5/src/stars/tests/instructions/test_blez.py`

 * *Files identical despite different names*

### Comparing `STARSimulator-1.0.3/src/stars/tests/instructions/test_bltz.py` & `STARSimulator-1.0.5/src/stars/tests/instructions/test_bltz.py`

 * *Files identical despite different names*

### Comparing `STARSimulator-1.0.3/src/stars/tests/instructions/test_bltzal.py` & `STARSimulator-1.0.5/src/stars/tests/instructions/test_bltzal.py`

 * *Files identical despite different names*

### Comparing `STARSimulator-1.0.3/src/stars/tests/instructions/test_bne.py` & `STARSimulator-1.0.5/src/stars/tests/instructions/test_bne.py`

 * *Files identical despite different names*

### Comparing `STARSimulator-1.0.3/src/stars/tests/instructions/test_clo.py` & `STARSimulator-1.0.5/src/stars/tests/instructions/test_clo.py`

 * *Files identical despite different names*

### Comparing `STARSimulator-1.0.3/src/stars/tests/instructions/test_clz.py` & `STARSimulator-1.0.5/src/stars/tests/instructions/test_clz.py`

 * *Files identical despite different names*

### Comparing `STARSimulator-1.0.3/src/stars/tests/instructions/test_div.py` & `STARSimulator-1.0.5/src/stars/tests/instructions/test_div.py`

 * *Files identical despite different names*

### Comparing `STARSimulator-1.0.3/src/stars/tests/instructions/test_divu.py` & `STARSimulator-1.0.5/src/stars/tests/instructions/test_divu.py`

 * *Files identical despite different names*

### Comparing `STARSimulator-1.0.3/src/stars/tests/instructions/test_j.py` & `STARSimulator-1.0.5/src/stars/tests/instructions/test_j.py`

 * *Files identical despite different names*

### Comparing `STARSimulator-1.0.3/src/stars/tests/instructions/test_jal.py` & `STARSimulator-1.0.5/src/stars/tests/instructions/test_jal.py`

 * *Files identical despite different names*

### Comparing `STARSimulator-1.0.3/src/stars/tests/instructions/test_jalr.py` & `STARSimulator-1.0.5/src/stars/tests/instructions/test_jalr.py`

 * *Files identical despite different names*

### Comparing `STARSimulator-1.0.3/src/stars/tests/instructions/test_lb.py` & `STARSimulator-1.0.5/src/stars/tests/instructions/test_lb.py`

 * *Files identical despite different names*

### Comparing `STARSimulator-1.0.3/src/stars/tests/instructions/test_lbu.py` & `STARSimulator-1.0.5/src/stars/tests/instructions/test_lbu.py`

 * *Files identical despite different names*

### Comparing `STARSimulator-1.0.3/src/stars/tests/instructions/test_lh.py` & `STARSimulator-1.0.5/src/stars/tests/instructions/test_lh.py`

 * *Files identical despite different names*

### Comparing `STARSimulator-1.0.3/src/stars/tests/instructions/test_lhu.py` & `STARSimulator-1.0.5/src/stars/tests/instructions/test_lhu.py`

 * *Files identical despite different names*

### Comparing `STARSimulator-1.0.3/src/stars/tests/instructions/test_lui.py` & `STARSimulator-1.0.5/src/stars/tests/instructions/test_lui.py`

 * *Files identical despite different names*

### Comparing `STARSimulator-1.0.3/src/stars/tests/instructions/test_lw.py` & `STARSimulator-1.0.5/src/stars/tests/instructions/test_lw.py`

 * *Files identical despite different names*

### Comparing `STARSimulator-1.0.3/src/stars/tests/instructions/test_lwl.py` & `STARSimulator-1.0.5/src/stars/tests/instructions/test_lwl.py`

 * *Files identical despite different names*

### Comparing `STARSimulator-1.0.3/src/stars/tests/instructions/test_lwr.py` & `STARSimulator-1.0.5/src/stars/tests/instructions/test_lwr.py`

 * *Files identical despite different names*

### Comparing `STARSimulator-1.0.3/src/stars/tests/instructions/test_mul.py` & `STARSimulator-1.0.5/src/stars/tests/instructions/test_mul.py`

 * *Files identical despite different names*

### Comparing `STARSimulator-1.0.3/src/stars/tests/instructions/test_mult.py` & `STARSimulator-1.0.5/src/stars/tests/instructions/test_mult.py`

 * *Files identical despite different names*

### Comparing `STARSimulator-1.0.3/src/stars/tests/instructions/test_multu.py` & `STARSimulator-1.0.5/src/stars/tests/instructions/test_multu.py`

 * *Files identical despite different names*

### Comparing `STARSimulator-1.0.3/src/stars/tests/instructions/test_nor.py` & `STARSimulator-1.0.5/src/stars/tests/instructions/test_nor.py`

 * *Files identical despite different names*

### Comparing `STARSimulator-1.0.3/src/stars/tests/instructions/test_or.py` & `STARSimulator-1.0.5/src/stars/tests/instructions/test_or.py`

 * *Files identical despite different names*

### Comparing `STARSimulator-1.0.3/src/stars/tests/instructions/test_sb.py` & `STARSimulator-1.0.5/src/stars/tests/instructions/test_sb.py`

 * *Files identical despite different names*

### Comparing `STARSimulator-1.0.3/src/stars/tests/instructions/test_sh.py` & `STARSimulator-1.0.5/src/stars/tests/instructions/test_sh.py`

 * *Files identical despite different names*

### Comparing `STARSimulator-1.0.3/src/stars/tests/instructions/test_sll.py` & `STARSimulator-1.0.5/src/stars/tests/instructions/test_sll.py`

 * *Files identical despite different names*

### Comparing `STARSimulator-1.0.3/src/stars/tests/instructions/test_sllv.py` & `STARSimulator-1.0.5/src/stars/tests/instructions/test_sllv.py`

 * *Files identical despite different names*

### Comparing `STARSimulator-1.0.3/src/stars/tests/instructions/test_slt.py` & `STARSimulator-1.0.5/src/stars/tests/instructions/test_slt.py`

 * *Files identical despite different names*

### Comparing `STARSimulator-1.0.3/src/stars/tests/instructions/test_slti.py` & `STARSimulator-1.0.5/src/stars/tests/instructions/test_slti.py`

 * *Files identical despite different names*

### Comparing `STARSimulator-1.0.3/src/stars/tests/instructions/test_sltiu.py` & `STARSimulator-1.0.5/src/stars/tests/instructions/test_sltiu.py`

 * *Files identical despite different names*

### Comparing `STARSimulator-1.0.3/src/stars/tests/instructions/test_sltu.py` & `STARSimulator-1.0.5/src/stars/tests/instructions/test_sltu.py`

 * *Files identical despite different names*

### Comparing `STARSimulator-1.0.3/src/stars/tests/instructions/test_sra.py` & `STARSimulator-1.0.5/src/stars/tests/instructions/test_sra.py`

 * *Files identical despite different names*

### Comparing `STARSimulator-1.0.3/src/stars/tests/instructions/test_srav.py` & `STARSimulator-1.0.5/src/stars/tests/instructions/test_srav.py`

 * *Files identical despite different names*

### Comparing `STARSimulator-1.0.3/src/stars/tests/instructions/test_srl.py` & `STARSimulator-1.0.5/src/stars/tests/instructions/test_srl.py`

 * *Files identical despite different names*

### Comparing `STARSimulator-1.0.3/src/stars/tests/instructions/test_srlv.py` & `STARSimulator-1.0.5/src/stars/tests/instructions/test_srlv.py`

 * *Files identical despite different names*

### Comparing `STARSimulator-1.0.3/src/stars/tests/instructions/test_sub.py` & `STARSimulator-1.0.5/src/stars/tests/instructions/test_sub.py`

 * *Files identical despite different names*

### Comparing `STARSimulator-1.0.3/src/stars/tests/instructions/test_sw.py` & `STARSimulator-1.0.5/src/stars/tests/instructions/test_sw.py`

 * *Files identical despite different names*

### Comparing `STARSimulator-1.0.3/src/stars/tests/instructions/test_swl.py` & `STARSimulator-1.0.5/src/stars/tests/instructions/test_swl.py`

 * *Files identical despite different names*

### Comparing `STARSimulator-1.0.3/src/stars/tests/instructions/test_swr.py` & `STARSimulator-1.0.5/src/stars/tests/instructions/test_swr.py`

 * *Files identical despite different names*

### Comparing `STARSimulator-1.0.3/src/stars/tests/instructions/test_xor.py` & `STARSimulator-1.0.5/src/stars/tests/instructions/test_xor.py`

 * *Files identical despite different names*

### Comparing `STARSimulator-1.0.3/src/stars/tests/interpreter/test_interpreter.py` & `STARSimulator-1.0.5/src/stars/tests/interpreter/test_interpreter.py`

 * *Files identical despite different names*

### Comparing `STARSimulator-1.0.3/src/stars/tests/interpreter/test_set_data.py` & `STARSimulator-1.0.5/src/stars/tests/interpreter/test_set_data.py`

 * *Files identical despite different names*

### Comparing `STARSimulator-1.0.3/src/stars/tests/preprocess/test_preprocess.py` & `STARSimulator-1.0.5/src/stars/tests/preprocess/test_preprocess.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 from os import path as p
+from pathlib import Path
 import unittest
 
 from preprocess import *
 
 '''
 https://github.com/sbustars/STARS
 
@@ -27,53 +28,58 @@
         path.resolve()
 
         files = []
         eqv_dict = {}
         abs_to_rel = {}
         walk(path, files, eqv_dict, abs_to_rel, path.parent)
         res = [f.name for f in files]
-        self.assertEqual(res, ['includeSuccess.asm', 'toInclude.asm'], msg='Failed test_walk_include_success.')
+        self.assertEqual(res, ['includeSuccess.asm', 'toInclude.asm'],
+                         msg='Failed test_walk_include_success.')
 
     def test_walk_include_already_included(self):
         path = Path(f"{p.dirname(__file__)}/alreadyIncluded.asm")
         path.resolve()
 
         files = []
         eqv_dict = {}
         abs_to_rel = {}
-        self.assertRaises(FileAlreadyIncluded, walk, path, files, eqv_dict, abs_to_rel, path.parent)
+        self.assertRaises(FileAlreadyIncluded, walk, path,
+                          files, eqv_dict, abs_to_rel, path.parent)
 
     def test_walk_include_file_dne(self):
         path = Path(f"{p.dirname(__file__)}/invalidFile.asm")
         path.resolve()
 
         files = []
         eqv_dict = {}
         abs_to_rel = {}
-        self.assertRaises(FileNotFoundError, walk, path, files, eqv_dict, abs_to_rel, path.parent)
+        self.assertRaises(FileNotFoundError, walk, path,
+                          files, eqv_dict, abs_to_rel, path.parent)
 
     def test_walk_eqv_success(self):
         path = Path(f"{p.dirname(__file__)}/eqvTest.asm")
         path.resolve()
 
         files = []
         eqv_dict = {}
         abs_to_rel = {}
         walk(path, files, eqv_dict, abs_to_rel, path.parent)
         expected = {r'\bword\b': '"hello"'}
-        self.assertEqual(eqv_dict, expected, msg='Failed test_walk_eqv_success.')
+        self.assertEqual(eqv_dict, expected,
+                         msg='Failed test_walk_eqv_success.')
 
     def test_eqv_restricted_token(self):
         path = Path(f"{p.dirname(__file__)}/eqvRestricted.asm")
         path.resolve()
 
         files = []
         eqv_dict = {}
         abs_to_rel = {}
-        self.assertRaises(InvalidEQV, walk, path, files, eqv_dict, abs_to_rel, path.parent)
+        self.assertRaises(InvalidEQV, walk, path, files,
+                          eqv_dict, abs_to_rel, path.parent)
 
     def test_preprocess_eqv_success(self):
         path = Path(f"{p.dirname(__file__)}/eqvTest.asm")
         path.resolve()
 
         files = []
         eqv_dict = {}
@@ -129,18 +135,20 @@
 jello: .word 4  "{p.dirname(__file__)}/toInclude.asm" 6
 '''}
         contents = {}
         processed = {}
         for file in files:
             with file.open() as f:
                 contents[file.as_posix()] = ''.join(f.readlines())
-                processed[file.as_posix()] = preprocess(contents[file.as_posix()], file, eqv_dict)
-            self.assertEqual(processed[file.as_posix()], expected[file.as_posix()], msg=f"Failed test_preprocess_include_success on file {file.name}.")
+                processed[file.as_posix()] = preprocess(
+                    contents[file.as_posix()], file, eqv_dict)
+            self.assertEqual(processed[file.as_posix()], expected[file.as_posix(
+            )], msg=f"Failed test_preprocess_include_success on file {file.name}.")
 
-        (og_text, text) = link(files, contents, processed, abs_to_rel)
+        (og_text, text, _) = link(files, contents, processed, abs_to_rel)
         self.assertEqual(text, f'''.text  "{p.dirname(__file__)}/toInclude.asm" 1
 li $v0, 10  "{p.dirname(__file__)}/toInclude.asm" 2
 syscall  "{p.dirname(__file__)}/toInclude.asm" 3
 
 .data  "{p.dirname(__file__)}/toInclude.asm" 5
 jello: .word 4  "{p.dirname(__file__)}/toInclude.asm" 6
 .text  "{p.dirname(__file__)}/includeSuccess.asm" 2
```

### Comparing `STARSimulator-1.0.3/src/stars/tests/pseudoOps/test_pseudoOps.py` & `STARSimulator-1.0.5/src/stars/tests/pseudoOps/test_pseudoOps.py`

 * *Files identical despite different names*

### Comparing `STARSimulator-1.0.3/src/stars/tests/registers/test_registers.py` & `STARSimulator-1.0.5/src/stars/tests/registers/test_registers.py`

 * *Files identical despite different names*

### Comparing `STARSimulator-1.0.3/src/stars/tests/syscalls/test_syscalls.py` & `STARSimulator-1.0.5/src/stars/tests/syscalls/test_syscalls.py`

 * *Files identical despite different names*

### Comparing `STARSimulator-1.0.3/src/stars/tests/test_sbumips.py` & `STARSimulator-1.0.5/src/stars/tests/test_sbumips.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 import unittest
 import unittest.mock as mock
 
 from gui import mainwindow
 from interpreter.classes import IType, Label, Syscall
 import sbumips
 
+
 class TestSbumips(unittest.TestCase):
 
     @mock.patch.object(mainwindow, "launch_gui")
     def test_no_args(self, mock_method: mock.patch.object):
         '''
             Tests the program with no arguments. The intended effect is the GUI is started with 
             a function call to launch_gui.
@@ -28,74 +29,78 @@
         sbumips.main(["--noGui", "testfile.asm"])
         mock_method.assert_called_once()
 
     def test_invalid_assemble(self):
         '''
             Tests if assemble returns FileNotFoundError if the main file is invalid.
         '''
-        self.assertRaises(FileNotFoundError ,sbumips.assemble, f"{p.dirname(__file__)}/testfile.asm")
+        self.assertRaises(FileNotFoundError, sbumips.assemble,
+                          f"{p.dirname(__file__)}/testfile.asm")
 
     def test_assemble(self):
         '''
             Tests if assemble returns the correct list of classes.
         '''
         intended_result = [
             Label("main"),
             IType("addi", ["$v0", "$0"], 1),
             IType("addi", ["$a0", "$0"], 1),
             Syscall(),
         ]
 
         result = sbumips.assemble(f"{p.dirname(__file__)}/test.asm")
 
-        self.assertEqual(len(intended_result), len(result), "The number of classes are not equal.")
-        
+        self.assertEqual(len(intended_result), len(result),
+                         "The number of classes are not equal.")
+
         for expected, actual in zip(intended_result, result):
-            self.assertEqual(str(expected), str(actual), "The lines are not equal.")
+            self.assertEqual(str(expected), str(actual),
+                             "The lines are not equal.")
 
     @mock.patch('sys.stdout', new_callable=StringIO)
     def test_assemble_only(self, mock_stdout: StringIO):
         '''
             Tests if assemble correctly prints and exits if ran the -a option"
         '''
         from settings import settings
         settings['assemble'] = True
 
-        self.assertRaises(SystemExit, sbumips.assemble, f"{p.dirname(__file__)}/test.asm")
+        self.assertRaises(SystemExit, sbumips.assemble,
+                          f"{p.dirname(__file__)}/test.asm")
         self.assertEqual(mock_stdout.getvalue(), "Program assembled successfully.\n",
-                "Program did not assembled successfully.")
-
+                         "Program did not assembled successfully.")
 
     @mock.patch('sys.stdout', new_callable=StringIO)
     def test_run_cli(self, mock_stdout: StringIO):
         '''
             Tests the program with the --noGui and -i option. The intended effect is the program 
             is executed and the asssembly file output along with the instruction count is printed 
             out.
         '''
         sbumips.main(["--noGui", "-i", f"{p.dirname(__file__)}/test.asm"])
         program_output, instruction_count = mock_stdout.getvalue().split("\n")
         self.assertEqual(program_output, "1", "Incorrect output.")
-        self.assertEqual(instruction_count, "Instruction count: 3", "Incorrect Instruction count.")
+        self.assertEqual(instruction_count, "Instruction count: 3",
+                         "Incorrect Instruction count.")
 
     @mock.patch('sys.stderr', new_callable=StringIO)
     def test_run_cli_error(self, mock_stderr: StringIO):
         '''
             Tests the program with an invalid file without the GUI. The intended effect is the 
             program prints out a FileNotFoundError to stderr and exits.
         '''
         sbumips.main(["--noGui", "-i", f"{p.dirname(__file__)}/testfile.asm"])
-        self.assertEqual(mock_stderr.getvalue(), 
-                f"FileNotFoundError: [Errno 2] No such file or directory: '{p.dirname(__file__)}/testfile.asm'\n",
-                "Program did not return a print out of FileNotFoundError")
+        self.assertEqual(mock_stderr.getvalue(),
+                         f"FileNotFoundError: [Errno 2] No such file or directory: '{p.dirname(__file__)}/testfile.asm'\n",
+                         "Program did not return a print out of FileNotFoundError")
 
     def test_run_cli_assemble(self):
         '''
             Tests that all declarations and instructions are assemble and recognized 
             by the lexer and parser.
         '''
         arguments = ["--noGui", f"{p.dirname(__file__)}/instructions.asm"]
         args = sbumips.init_args(arguments)
         sbumips.init_settings(args)
         pArgs = args.pa if args.pa else []
         result = sbumips.assemble(args.filename)
-        inter = sbumips.Interpreter(result, pArgs)
+        inter = sbumips.Interpreter(result, pArgs)
```

### Comparing `STARSimulator-1.0.3/src/stars/tests/validArgs/test_parse_args.py` & `STARSimulator-1.0.5/src/stars/tests/validArgs/test_parse_args.py`

 * *Files identical despite different names*

