# Comparing `tmp/sqlaf-1.0.0.tar.gz` & `tmp/sqlaf-1.1.0.tar.gz`

## Comparing `sqlaf-1.0.0.tar` & `sqlaf-1.1.0.tar`

### file list

```diff
@@ -1,55 +1,55 @@
--rw-r--r--   0        0        0       69 2020-02-02 00:00:00.000000 sqlaf-1.0.0/.coveragerc
--rwxr-xr-x   0        0        0       90 2020-02-02 00:00:00.000000 sqlaf-1.0.0/.flake8
--rw-r--r--   0        0        0     1002 2020-02-02 00:00:00.000000 sqlaf-1.0.0/Makefile
--rw-r--r--   0        0        0    67184 2020-02-02 00:00:00.000000 sqlaf-1.0.0/poetry.lock
--rw-r--r--   0        0        0      428 2020-02-02 00:00:00.000000 sqlaf-1.0.0/tox.ini
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 sqlaf-1.0.0/.github/CODEOWNERS
--rw-r--r--   0        0        0      415 2020-02-02 00:00:00.000000 sqlaf-1.0.0/.github/release-drafter.yml
--rw-r--r--   0        0        0      282 2020-02-02 00:00:00.000000 sqlaf-1.0.0/.github/workflows/linting.yml
--rw-r--r--   0        0        0      804 2020-02-02 00:00:00.000000 sqlaf-1.0.0/.github/workflows/release-test.yml
--rw-r--r--   0        0        0      754 2020-02-02 00:00:00.000000 sqlaf-1.0.0/.github/workflows/release.yml
--rw-r--r--   0        0        0      284 2020-02-02 00:00:00.000000 sqlaf-1.0.0/.github/workflows/security.yml
--rw-r--r--   0        0        0     2081 2020-02-02 00:00:00.000000 sqlaf-1.0.0/.github/workflows/test.yml
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sqlaf-1.0.0/sqlaf/__init__.py
--rw-r--r--   0        0        0      368 2020-02-02 00:00:00.000000 sqlaf-1.0.0/sqlaf/config.py
--rw-r--r--   0        0        0      893 2020-02-02 00:00:00.000000 sqlaf-1.0.0/sqlaf/exceptions.py
--rw-r--r--   0        0        0     2157 2020-02-02 00:00:00.000000 sqlaf-1.0.0/sqlaf/operators.py
--rw-r--r--   0        0        0      980 2020-02-02 00:00:00.000000 sqlaf-1.0.0/sqlaf/utils.py
--rw-r--r--   0        0        0       77 2020-02-02 00:00:00.000000 sqlaf-1.0.0/sqlaf/fields/__init__.py
--rw-r--r--   0        0        0     2211 2020-02-02 00:00:00.000000 sqlaf-1.0.0/sqlaf/fields/base.py
--rw-r--r--   0        0        0     4235 2020-02-02 00:00:00.000000 sqlaf-1.0.0/sqlaf/fields/fields.py
--rw-r--r--   0        0        0      291 2020-02-02 00:00:00.000000 sqlaf-1.0.0/sqlaf/fields/interfaces.py
--rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 sqlaf-1.0.0/sqlaf/filters/__init__.py
--rw-r--r--   0        0        0     2891 2020-02-02 00:00:00.000000 sqlaf-1.0.0/sqlaf/filters/filters.py
--rw-r--r--   0        0        0      296 2020-02-02 00:00:00.000000 sqlaf-1.0.0/sqlaf/filters/interfaces.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sqlaf-1.0.0/tests/__init__.py
--rw-r--r--   0        0        0      527 2020-02-02 00:00:00.000000 sqlaf-1.0.0/tests/base.py
--rw-r--r--   0        0        0     2467 2020-02-02 00:00:00.000000 sqlaf-1.0.0/tests/db/alembic.ini
--rwxr-xr-x   0        0        0       90 2020-02-02 00:00:00.000000 sqlaf-1.0.0/tests/db/generate_migrations
--rwxr-xr-x   0        0        0       74 2020-02-02 00:00:00.000000 sqlaf-1.0.0/tests/db/migrate
--rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 sqlaf-1.0.0/tests/db/alembic/README
--rw-r--r--   0        0        0     2598 2020-02-02 00:00:00.000000 sqlaf-1.0.0/tests/db/alembic/env.py
--rw-r--r--   0        0        0      494 2020-02-02 00:00:00.000000 sqlaf-1.0.0/tests/db/alembic/script.py.mako
--rw-r--r--   0        0        0      769 2020-02-02 00:00:00.000000 sqlaf-1.0.0/tests/db/alembic/versions/10fff1c96965_generate_migrations.py
--rw-r--r--   0        0        0     1103 2020-02-02 00:00:00.000000 sqlaf-1.0.0/tests/db/alembic/versions/6da73feb70b3_generate_migrations.py
--rw-r--r--   0        0        0      731 2020-02-02 00:00:00.000000 sqlaf-1.0.0/tests/db/alembic/versions/be81804c2167_generate_migrations.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sqlaf-1.0.0/tests/fields/__init__.py
--rw-r--r--   0        0        0     4548 2020-02-02 00:00:00.000000 sqlaf-1.0.0/tests/fields/test_arrayfield.py
--rw-r--r--   0        0        0     2274 2020-02-02 00:00:00.000000 sqlaf-1.0.0/tests/fields/test_boolean_field.py
--rw-r--r--   0        0        0     5863 2020-02-02 00:00:00.000000 sqlaf-1.0.0/tests/fields/test_char_field.py
--rw-r--r--   0        0        0     3815 2020-02-02 00:00:00.000000 sqlaf-1.0.0/tests/fields/test_datefield.py
--rw-r--r--   0        0        0     5356 2020-02-02 00:00:00.000000 sqlaf-1.0.0/tests/fields/test_datetimefield.py
--rw-r--r--   0        0        0     5847 2020-02-02 00:00:00.000000 sqlaf-1.0.0/tests/fields/test_enum_field.py
--rw-r--r--   0        0        0     3651 2020-02-02 00:00:00.000000 sqlaf-1.0.0/tests/fields/test_filter.py
--rw-r--r--   0        0        0    11708 2020-02-02 00:00:00.000000 sqlaf-1.0.0/tests/fields/test_integer_field.py
--rw-r--r--   0        0        0     1134 2020-02-02 00:00:00.000000 sqlaf-1.0.0/tests/fields/test_post_filter.py
--rw-r--r--   0        0        0     4036 2020-02-02 00:00:00.000000 sqlaf-1.0.0/tests/fields/test_timefield.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sqlaf-1.0.0/tests/implementation/__init__.py
--rw-r--r--   0        0        0      826 2020-02-02 00:00:00.000000 sqlaf-1.0.0/tests/implementation/db.py
--rw-r--r--   0        0        0      298 2020-02-02 00:00:00.000000 sqlaf-1.0.0/tests/implementation/factories.py
--rw-r--r--   0        0        0      571 2020-02-02 00:00:00.000000 sqlaf-1.0.0/tests/implementation/models.py
--rw-r--r--   0        0        0     1806 2020-02-02 00:00:00.000000 sqlaf-1.0.0/.gitignore
--rw-r--r--   0        0        0      552 2020-02-02 00:00:00.000000 sqlaf-1.0.0/LICENSE
--rw-r--r--   0        0        0     6210 2020-02-02 00:00:00.000000 sqlaf-1.0.0/README.md
--rw-r--r--   0        0        0     1140 2020-02-02 00:00:00.000000 sqlaf-1.0.0/pyproject.toml
--rw-r--r--   0        0        0     7411 2020-02-02 00:00:00.000000 sqlaf-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0       69 2020-02-02 00:00:00.000000 sqlaf-1.1.0/.coveragerc
+-rwxr-xr-x   0        0        0       90 2020-02-02 00:00:00.000000 sqlaf-1.1.0/.flake8
+-rw-r--r--   0        0        0     1002 2020-02-02 00:00:00.000000 sqlaf-1.1.0/Makefile
+-rw-r--r--   0        0        0    67184 2020-02-02 00:00:00.000000 sqlaf-1.1.0/poetry.lock
+-rw-r--r--   0        0        0      428 2020-02-02 00:00:00.000000 sqlaf-1.1.0/tox.ini
+-rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 sqlaf-1.1.0/.github/CODEOWNERS
+-rw-r--r--   0        0        0      415 2020-02-02 00:00:00.000000 sqlaf-1.1.0/.github/release-drafter.yml
+-rw-r--r--   0        0        0      282 2020-02-02 00:00:00.000000 sqlaf-1.1.0/.github/workflows/linting.yml
+-rw-r--r--   0        0        0      754 2020-02-02 00:00:00.000000 sqlaf-1.1.0/.github/workflows/release.yml
+-rw-r--r--   0        0        0      284 2020-02-02 00:00:00.000000 sqlaf-1.1.0/.github/workflows/security.yml
+-rw-r--r--   0        0        0     2082 2020-02-02 00:00:00.000000 sqlaf-1.1.0/.github/workflows/test.yml
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sqlaf-1.1.0/sqlaf/__init__.py
+-rw-r--r--   0        0        0      424 2020-02-02 00:00:00.000000 sqlaf-1.1.0/sqlaf/config.py
+-rw-r--r--   0        0        0      893 2020-02-02 00:00:00.000000 sqlaf-1.1.0/sqlaf/exceptions.py
+-rw-r--r--   0        0        0     2157 2020-02-02 00:00:00.000000 sqlaf-1.1.0/sqlaf/operators.py
+-rw-r--r--   0        0        0      980 2020-02-02 00:00:00.000000 sqlaf-1.1.0/sqlaf/utils.py
+-rw-r--r--   0        0        0       77 2020-02-02 00:00:00.000000 sqlaf-1.1.0/sqlaf/fields/__init__.py
+-rw-r--r--   0        0        0     3112 2020-02-02 00:00:00.000000 sqlaf-1.1.0/sqlaf/fields/base.py
+-rw-r--r--   0        0        0     4658 2020-02-02 00:00:00.000000 sqlaf-1.1.0/sqlaf/fields/fields.py
+-rw-r--r--   0        0        0      291 2020-02-02 00:00:00.000000 sqlaf-1.1.0/sqlaf/fields/interfaces.py
+-rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 sqlaf-1.1.0/sqlaf/filters/__init__.py
+-rw-r--r--   0        0        0     2891 2020-02-02 00:00:00.000000 sqlaf-1.1.0/sqlaf/filters/filters.py
+-rw-r--r--   0        0        0      296 2020-02-02 00:00:00.000000 sqlaf-1.1.0/sqlaf/filters/interfaces.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sqlaf-1.1.0/tests/__init__.py
+-rw-r--r--   0        0        0      527 2020-02-02 00:00:00.000000 sqlaf-1.1.0/tests/base.py
+-rw-r--r--   0        0        0     2467 2020-02-02 00:00:00.000000 sqlaf-1.1.0/tests/db/alembic.ini
+-rwxr-xr-x   0        0        0       90 2020-02-02 00:00:00.000000 sqlaf-1.1.0/tests/db/generate_migrations
+-rwxr-xr-x   0        0        0       74 2020-02-02 00:00:00.000000 sqlaf-1.1.0/tests/db/migrate
+-rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 sqlaf-1.1.0/tests/db/alembic/README
+-rw-r--r--   0        0        0     2598 2020-02-02 00:00:00.000000 sqlaf-1.1.0/tests/db/alembic/env.py
+-rw-r--r--   0        0        0      494 2020-02-02 00:00:00.000000 sqlaf-1.1.0/tests/db/alembic/script.py.mako
+-rw-r--r--   0        0        0      769 2020-02-02 00:00:00.000000 sqlaf-1.1.0/tests/db/alembic/versions/10fff1c96965_generate_migrations.py
+-rw-r--r--   0        0        0     1103 2020-02-02 00:00:00.000000 sqlaf-1.1.0/tests/db/alembic/versions/6da73feb70b3_generate_migrations.py
+-rw-r--r--   0        0        0      731 2020-02-02 00:00:00.000000 sqlaf-1.1.0/tests/db/alembic/versions/be81804c2167_generate_migrations.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sqlaf-1.1.0/tests/fields/__init__.py
+-rw-r--r--   0        0        0     4548 2020-02-02 00:00:00.000000 sqlaf-1.1.0/tests/fields/test_arrayfield.py
+-rw-r--r--   0        0        0     2274 2020-02-02 00:00:00.000000 sqlaf-1.1.0/tests/fields/test_boolean_field.py
+-rw-r--r--   0        0        0     6681 2020-02-02 00:00:00.000000 sqlaf-1.1.0/tests/fields/test_char_field.py
+-rw-r--r--   0        0        0      897 2020-02-02 00:00:00.000000 sqlaf-1.1.0/tests/fields/test_custom_operators.py
+-rw-r--r--   0        0        0     3815 2020-02-02 00:00:00.000000 sqlaf-1.1.0/tests/fields/test_datefield.py
+-rw-r--r--   0        0        0     5356 2020-02-02 00:00:00.000000 sqlaf-1.1.0/tests/fields/test_datetimefield.py
+-rw-r--r--   0        0        0     6858 2020-02-02 00:00:00.000000 sqlaf-1.1.0/tests/fields/test_enum_field.py
+-rw-r--r--   0        0        0     3651 2020-02-02 00:00:00.000000 sqlaf-1.1.0/tests/fields/test_filter.py
+-rw-r--r--   0        0        0    12739 2020-02-02 00:00:00.000000 sqlaf-1.1.0/tests/fields/test_integer_field.py
+-rw-r--r--   0        0        0     1134 2020-02-02 00:00:00.000000 sqlaf-1.1.0/tests/fields/test_post_filter.py
+-rw-r--r--   0        0        0     4036 2020-02-02 00:00:00.000000 sqlaf-1.1.0/tests/fields/test_timefield.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sqlaf-1.1.0/tests/implementation/__init__.py
+-rw-r--r--   0        0        0      826 2020-02-02 00:00:00.000000 sqlaf-1.1.0/tests/implementation/db.py
+-rw-r--r--   0        0        0      298 2020-02-02 00:00:00.000000 sqlaf-1.1.0/tests/implementation/factories.py
+-rw-r--r--   0        0        0      571 2020-02-02 00:00:00.000000 sqlaf-1.1.0/tests/implementation/models.py
+-rw-r--r--   0        0        0     1806 2020-02-02 00:00:00.000000 sqlaf-1.1.0/.gitignore
+-rw-r--r--   0        0        0      552 2020-02-02 00:00:00.000000 sqlaf-1.1.0/LICENSE
+-rw-r--r--   0        0        0     6641 2020-02-02 00:00:00.000000 sqlaf-1.1.0/README.md
+-rw-r--r--   0        0        0     1140 2020-02-02 00:00:00.000000 sqlaf-1.1.0/pyproject.toml
+-rw-r--r--   0        0        0     7842 2020-02-02 00:00:00.000000 sqlaf-1.1.0/PKG-INFO
```

### Comparing `sqlaf-1.0.0/Makefile` & `sqlaf-1.1.0/Makefile`

 * *Files identical despite different names*

### Comparing `sqlaf-1.0.0/poetry.lock` & `sqlaf-1.1.0/poetry.lock`

 * *Files identical despite different names*

### Comparing `sqlaf-1.0.0/.github/workflows/release.yml` & `sqlaf-1.1.0/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `sqlaf-1.0.0/.github/workflows/test.yml` & `sqlaf-1.1.0/.github/workflows/test.yml`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 name: Tests
 on: [push]
 env:
     DB_URL: postgresql://postgres:postgres@localhost:5432/sqlalchemy-filters
 jobs:
   tests:
     name: Testing Python ${{ matrix.python_version }} - Postgres ${{ matrix.postgres_version }}
-    runs-on: ubuntu-18.04
+    runs-on: ubuntu-latest
     strategy:
       max-parallel: 5
       fail-fast: false
       matrix:
         python_version: ['3.7', '3.8', '3.9', '3.10']
         postgres_version: ['10-alpine', '11-alpine', '12-alpine', '13-alpine', '14-alpine']
```

### Comparing `sqlaf-1.0.0/sqlaf/exceptions.py` & `sqlaf-1.1.0/sqlaf/exceptions.py`

 * *Files identical despite different names*

### Comparing `sqlaf-1.0.0/sqlaf/operators.py` & `sqlaf-1.1.0/sqlaf/operators.py`

 * *Files identical despite different names*

### Comparing `sqlaf-1.0.0/sqlaf/utils.py` & `sqlaf-1.1.0/sqlaf/utils.py`

 * *Files identical despite different names*

### Comparing `sqlaf-1.0.0/sqlaf/fields/base.py` & `sqlaf-1.1.0/sqlaf/fields/base.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,27 +1,45 @@
-from typing import Any
+from typing import Any, Callable, List, Union
 
 from sqlalchemy.sql.elements import BinaryExpression
 
 from sqlaf import config
 from sqlaf.fields import IField
 from sqlaf.exceptions import FieldInstantiationException, FieldValidationException
 
 
 class Field(IField):
 
-    allowed_operators = []
+    allowed_operators: List[Union[str, Callable]] = []
+    null_values: List[str] = []
 
-    def __init__(self, source, operator: str = "eq", default: Any = None):
-        if self.allowed_operators and operator not in self.allowed_operators:
+    def __init__(
+        self,
+        source,
+        operator: Union[str, Callable] = "eq",
+        default: Any = None,
+        null_values: List[Any] = [],
+        *args,
+        **kwargs,
+    ):
+        """Base class for all fields.
+
+        Args:
+            source (str): The source field.
+            operator (str, optional): The operator to use for filtering. Defaults to "eq".
+            default (Any, optional): The default value to use if the value is None. Defaults to None.
+            null_values (List[Any], optional): The values to treat as null e.g. "null". Defaults to [].
+        """
+        if self.allowed_operators and operator not in self.allowed_operators and not isinstance(operator, Callable):
             raise FieldInstantiationException(f"{operator} not supported for {self.__class__}")
 
         self.default = default
         self.source = source
         self.operator = operator
+        self.null_values = null_values
 
     def transform(self, value: Any) -> Any:
         """Function which allows for manipulation of the value being passed in i.e. if the data needs to be in a
             certain format for a field type the manipulation would be performed here.
 
         Args:
             value (Any): The value to manipulate.
@@ -37,15 +55,20 @@
 
         Args:
             value (Any): The value to filter with.
 
         Returns:
             BinaryExpression: An SQLAlchemy BinaryExpression filter.
         """
-        operator_func = config.FILTER_OPERATORS.get(self.operator.lower())
+        operator_func = None
+
+        if isinstance(self.operator, Callable):
+            operator_func = self.operator
+        elif isinstance(self.operator, str):
+            operator_func = config.FILTER_OPERATORS.get(self.operator.lower())
 
         if not operator_func:
             raise NotImplementedError(f"{self.operator} is not a supported operator.")
 
         return operator_func(self.source, value)
 
     def filter(self, value: Any) -> BinaryExpression:
@@ -57,12 +80,12 @@
         Raises:
             e: FieldValidationException
 
         Returns:
             BinaryExpression: An SQLAlchemy BinaryExpression filter.
         """
         try:
-            value = self.transform(value)
+            value = None if value in self.null_values else self.transform(value)
         except FieldValidationException as e:
             raise e
 
         return self.get_filters(value)
```

### Comparing `sqlaf-1.0.0/sqlaf/fields/fields.py` & `sqlaf-1.1.0/sqlaf/fields/fields.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,15 +1,12 @@
-from abc import ABC
 from datetime import date, datetime
 from enum import Enum, IntEnum
-from typing import Any, List
+from typing import Any, Callable, List, Union
 
-from sqlalchemy.sql.elements import BinaryExpression
 
-from sqlaf import config
 from sqlaf.exceptions import FieldInstantiationException, FieldValidationException
 from sqlaf.fields import Field
 
 
 class CharField(Field):
 
     allowed_operators = ["eq", "~eq", "ieq", "~ieq", "contains", "icontains"]
@@ -39,16 +36,23 @@
             raise FieldValidationException(f"{value} is not of type integer.")
 
 
 class EnumField(Field):
 
     allowed_operators = ["eq", "~eq"]
 
-    def __init__(self, source, enum_class: Enum, operator: str = "eq", default: Any = None):
-        super().__init__(source, operator=operator, default=default)
+    def __init__(
+        self,
+        source,
+        enum_class: Enum,
+        operator: Union[str, Callable] = "eq",
+        default: Any = None,
+        null_values: List[Any] = [],
+    ):
+        super().__init__(source, operator=operator, default=default, null_values=null_values)
 
         if not enum_class:
             raise FieldInstantiationException("`enum_class` cannot be None.")
 
         self.enum_class = enum_class
 
     def transform(self, value: Any) -> Enum:
@@ -65,16 +69,24 @@
 
 class BooleanField(Field):
 
     allowed_operators = ["eq"]
     truthy = [True, 1]
     falsy = [False, 0]
 
-    def __init__(self, source, operator: str = "eq", truthy: List = [], falsy: List = [], default: Any = None):
-        super().__init__(source, operator=operator, default=default)
+    def __init__(
+        self,
+        source,
+        operator: Union[str, Callable] = "eq",
+        truthy: List = [],
+        falsy: List = [],
+        default: Any = None,
+        null_values: List[Any] = [],
+    ):
+        super().__init__(source, operator=operator, default=default, null_values=null_values)
 
         if truthy and isinstance(truthy, list):
             self.truthy = truthy
 
         if falsy and isinstance(falsy, list):
             self.falsy = falsy
 
@@ -90,16 +102,22 @@
         raise FieldValidationException(f"{value} is an invalid truthy/falsy option.")
 
 
 class ArrayField(Field):
 
     allowed_operators = ["contains", "~contains"]
 
-    def __init__(self, source, operator: str = "contains", default: Any = None):
-        super().__init__(source, operator=operator, default=default)
+    def __init__(
+        self,
+        source,
+        operator: Union[str, Callable] = "contains",
+        default: Any = None,
+        null_values: List[Any] = [],
+    ):
+        super().__init__(source, operator=operator, default=default, null_values=null_values)
 
     def transform(self, value: Any):
         value = super().transform(value)
 
         if isinstance(value, list):
             return value
 
@@ -110,16 +128,23 @@
 
 
 class DateField(Field):
 
     allowed_operators = ["eq", "~eq", "gt", "gte", "lt", "lte"]
     format = "%Y-%m-%d"
 
-    def __init__(self, source, operator: str = "eq", format: str = None, default: Any = None):
-        super().__init__(source, operator=operator, default=default)
+    def __init__(
+        self,
+        source,
+        operator: Union[str, Callable] = "eq",
+        format: str = None,
+        default: Any = None,
+        null_values: List[Any] = [],
+    ):
+        super().__init__(source, operator=operator, default=default, null_values=null_values)
 
         if format:
             self.format = format
 
     def _parse_datetime_string(self, value: Any):
         return datetime.strptime(value, self.format).date()
```

### Comparing `sqlaf-1.0.0/sqlaf/filters/filters.py` & `sqlaf-1.1.0/sqlaf/filters/filters.py`

 * *Files identical despite different names*

### Comparing `sqlaf-1.0.0/tests/base.py` & `sqlaf-1.1.0/tests/base.py`

 * *Files identical despite different names*

### Comparing `sqlaf-1.0.0/tests/db/alembic.ini` & `sqlaf-1.1.0/tests/db/alembic.ini`

 * *Files identical despite different names*

### Comparing `sqlaf-1.0.0/tests/db/alembic/env.py` & `sqlaf-1.1.0/tests/db/alembic/env.py`

 * *Files identical despite different names*

### Comparing `sqlaf-1.0.0/tests/db/alembic/versions/10fff1c96965_generate_migrations.py` & `sqlaf-1.1.0/tests/db/alembic/versions/10fff1c96965_generate_migrations.py`

 * *Files identical despite different names*

### Comparing `sqlaf-1.0.0/tests/db/alembic/versions/6da73feb70b3_generate_migrations.py` & `sqlaf-1.1.0/tests/db/alembic/versions/6da73feb70b3_generate_migrations.py`

 * *Files identical despite different names*

### Comparing `sqlaf-1.0.0/tests/db/alembic/versions/be81804c2167_generate_migrations.py` & `sqlaf-1.1.0/tests/db/alembic/versions/be81804c2167_generate_migrations.py`

 * *Files identical despite different names*

### Comparing `sqlaf-1.0.0/tests/fields/test_arrayfield.py` & `sqlaf-1.1.0/tests/fields/test_arrayfield.py`

 * *Files identical despite different names*

### Comparing `sqlaf-1.0.0/tests/fields/test_boolean_field.py` & `sqlaf-1.1.0/tests/fields/test_boolean_field.py`

 * *Files identical despite different names*

### Comparing `sqlaf-1.0.0/tests/fields/test_char_field.py` & `sqlaf-1.1.0/tests/fields/test_char_field.py`

 * *Files 6% similar despite different names*

```diff
@@ -18,14 +18,24 @@
             name = fields.CharField(Booking.name, operator="eq")
 
         query = self.session.query(Booking)
         filtered_query = BookingFilter(query).filter({"name": "Jim Halpert"}).all()
         self.assertEqual(len(filtered_query), 1)
         self.assertEqual(filtered_query[0].name, "Jim Halpert")
 
+    def test_eq_filter_null_value(self):
+        class BookingFilter(filters.Filter):
+            name = fields.CharField(Booking.name, operator="eq", null_values=["null"])
+
+        BookingFactory(name=None)
+        query = self.session.query(Booking)
+        filtered_query = BookingFilter(query).filter({"name": "null"}).all()
+        self.assertEqual(len(filtered_query), 1)
+        self.assertEqual(filtered_query[0].name, None)
+
     # ieq operator
 
     def test_ieq_filter(self):
         class BookingFilter(filters.Filter):
             name = fields.CharField(Booking.name, operator="ieq")
 
         query = self.session.query(Booking)
@@ -41,14 +51,23 @@
 
         query = self.session.query(Booking)
         filtered_query = BookingFilter(query).filter({"name": "Jim Halpert"}).all()
         self.assertEqual(len(filtered_query), 2)
         self.assertEqual(filtered_query[0].name, "100% Michael Scott")
         self.assertEqual(filtered_query[1].name, "Pam Halpert\Beesly")  # NOQA
 
+    def test_not_eq_filter_null_value(self):
+        class BookingFilter(filters.Filter):
+            name = fields.CharField(Booking.name, operator="~eq", null_values=["null"])
+
+        BookingFactory(name=None)
+        query = self.session.query(Booking)
+        filtered_query = BookingFilter(query).filter({"name": "null"}).all()
+        self.assertEqual(len(filtered_query), 3)
+
     # ~ieq operator
 
     def test_not_ieq_filter(self):
         class BookingFilter(filters.Filter):
             name = fields.CharField(Booking.name, operator="~ieq")
 
         query = self.session.query(Booking)
```

### Comparing `sqlaf-1.0.0/tests/fields/test_datefield.py` & `sqlaf-1.1.0/tests/fields/test_datefield.py`

 * *Files identical despite different names*

### Comparing `sqlaf-1.0.0/tests/fields/test_datetimefield.py` & `sqlaf-1.1.0/tests/fields/test_datetimefield.py`

 * *Files identical despite different names*

### Comparing `sqlaf-1.0.0/tests/fields/test_enum_field.py` & `sqlaf-1.1.0/tests/fields/test_enum_field.py`

 * *Files 12% similar despite different names*

```diff
@@ -63,14 +63,24 @@
         query = self.session.query(Booking)
         filtered_query = BookingFilter(query).filter({"number_of_heads": None}).all()
         self.assertEqual(len(filtered_query), 3)
         self.assertEqual(filtered_query[0].number_of_heads, 3)
         self.assertEqual(filtered_query[1].number_of_heads, 4)
         self.assertEqual(filtered_query[2].number_of_heads, 5)
 
+    def test_eq_filter_null_value(self):
+        class BookingFilter(filters.Filter):
+            number_of_heads = fields.EnumField(Booking.number_of_heads, NumberOfHeads, null_values=["null"])
+
+        BookingFactory(number_of_heads=None)
+        query = self.session.query(Booking)
+        filtered_query = BookingFilter(query).filter({"number_of_heads": "null"}).all()
+        self.assertEqual(len(filtered_query), 1)
+        self.assertEqual(filtered_query[0].number_of_heads, None)
+
     # ~eq operator
 
     def test_not_eq_filter_int_enum(self):
         class BookingFilter(filters.Filter):
             number_of_heads = fields.EnumField(Booking.number_of_heads, NumberOfHeads, operator="~eq")
 
         query = self.session.query(Booking)
@@ -100,14 +110,28 @@
 
         query = self.session.query(Booking)
         filtered_query = BookingFilter(query).filter({}).all()
         self.assertEqual(len(filtered_query), 2)
         self.assertEqual(filtered_query[0].number_of_heads, 3)
         self.assertEqual(filtered_query[1].number_of_heads, 5)
 
+    def test_not_eq_filter_null_value(self):
+        class BookingFilter(filters.Filter):
+            number_of_heads = fields.EnumField(
+                Booking.number_of_heads,
+                NumberOfHeads,
+                operator="~eq",
+                null_values=["null"],
+            )
+
+        BookingFactory(number_of_heads=None)
+        query = self.session.query(Booking)
+        filtered_query = BookingFilter(query).filter({"number_of_heads": "null"}).all()
+        self.assertEqual(len(filtered_query), 3)
+
     # exceptions
 
     def test_invalid_int_enum_option(self):
         class BookingFilter(filters.Filter):
             number_of_heads = fields.EnumField(Booking.number_of_heads, NumberOfHeads)
 
         query = self.session.query(Booking)
```

### Comparing `sqlaf-1.0.0/tests/fields/test_filter.py` & `sqlaf-1.1.0/tests/fields/test_filter.py`

 * *Files identical despite different names*

### Comparing `sqlaf-1.0.0/tests/fields/test_integer_field.py` & `sqlaf-1.1.0/tests/fields/test_integer_field.py`

 * *Files 1% similar despite different names*

```diff
@@ -52,14 +52,23 @@
             number_of_heads = fields.IntegerField(Booking.number_of_heads, default=3)
 
         query = self.session.query(Booking)
         filtered_query = BookingFilter(query).filter({}).all()
         self.assertEqual(len(filtered_query), 1)
         self.assertEqual(filtered_query[0].number_of_heads, 3)
 
+    def test_eq_filter_null_value(self):
+        class BookingFilter(filters.Filter):
+            number_of_heads = fields.IntegerField(Booking.number_of_heads, null_values=["null"])
+
+        BookingFactory(number_of_heads=None)
+        query = self.session.query(Booking)
+        filtered_query = BookingFilter(query).filter({"number_of_heads": "null"}).all()
+        self.assertEqual(len(filtered_query), 1)
+
     # ~eq operator
 
     def test_not_eq_filter(self):
         class BookingFilter(filters.Filter):
             number_of_heads = fields.IntegerField(Booking.number_of_heads, operator="~eq")
 
         query = self.session.query(Booking)
@@ -103,14 +112,26 @@
 
         query = self.session.query(Booking)
         filtered_query = BookingFilter(query).filter({}).order_by(Booking.number_of_heads).all()
         self.assertEqual(len(filtered_query), 2)
         self.assertEqual(filtered_query[0].number_of_heads, 4)
         self.assertEqual(filtered_query[1].number_of_heads, 5)
 
+    def test_not_eq_filter_null_value(self):
+        class BookingFilter(filters.Filter):
+            number_of_heads = fields.IntegerField(Booking.number_of_heads, operator="~eq", null_values=["null"])
+
+        BookingFactory(number_of_heads=None)
+        query = self.session.query(Booking)
+        filtered_query = BookingFilter(query).filter({"number_of_heads": "null"}).all()
+        self.assertEqual(len(filtered_query), 3)
+        self.assertEqual(filtered_query[0].number_of_heads, 3)
+        self.assertEqual(filtered_query[1].number_of_heads, 4)
+        self.assertEqual(filtered_query[2].number_of_heads, 5)
+
     # gt operator
 
     def test_gt_filter(self):
         class BookingFilter(filters.Filter):
             number_of_heads = fields.IntegerField(Booking.number_of_heads, operator="gt")
 
         query = self.session.query(Booking)
```

### Comparing `sqlaf-1.0.0/tests/fields/test_post_filter.py` & `sqlaf-1.1.0/tests/fields/test_post_filter.py`

 * *Files identical despite different names*

### Comparing `sqlaf-1.0.0/tests/fields/test_timefield.py` & `sqlaf-1.1.0/tests/fields/test_timefield.py`

 * *Files identical despite different names*

### Comparing `sqlaf-1.0.0/tests/implementation/db.py` & `sqlaf-1.1.0/tests/implementation/db.py`

 * *Files identical despite different names*

### Comparing `sqlaf-1.0.0/tests/implementation/models.py` & `sqlaf-1.1.0/tests/implementation/models.py`

 * *Files identical despite different names*

### Comparing `sqlaf-1.0.0/.gitignore` & `sqlaf-1.1.0/.gitignore`

 * *Files identical despite different names*

### Comparing `sqlaf-1.0.0/LICENSE` & `sqlaf-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `sqlaf-1.0.0/README.md` & `sqlaf-1.1.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # sqlaf
 
 [![PyPI pyversions](https://img.shields.io/pypi/pyversions/sqlaf.svg)](https://pypi.python.org/pypi/sqlaf/)
 [![pypi](https://img.shields.io/pypi/v/sqlaf)](https://pypi.org/project/sqlaf/)
+[![codecov](https://codecov.io/gh/iamstej/sqlaf/branch/main/graph/badge.svg?token=D1L129C3NF)](https://codecov.io/gh/iamstej/sqlaf)
 
 sqlaf is a library for transforming query parameters into SQLAlchemy filters in a structured and organised manner
 
 ## Installation
 
 Use the package manager [pip](https://pip.pypa.io/en/stable/) to install sqlaf.
 
@@ -26,14 +27,26 @@
 class TeamFilter(filters.Filter):
 
     founded_date = fields.DateField(Team.founded_date, operator="gte")
     name = fields.CharField(Team.name, operator="icontains")
     size = fields.IntegerField(Team.size, operator="eq")
 ```
 
+If you want to allow a specific value passed from a query parameter to be treated as `None`, use the `null_values` param e.g.
+
+```python
+
+from sqlaf import filters, fields
+
+class TeamFilter(filters.Filter):
+
+    size = fields.IntegerField(Team.size, operator="eq", null_values=["null", "-1"])
+```
+
+
 ### Using a Filter
 
 A filter class can be used in the following ways:
 
 #### Query parameter string with "?"
 ```python
 query = session.query(Team)
@@ -95,15 +108,15 @@
 To extend the above operators, you can create custom operators:
 
 ```python
 from sqlaf import filters, fields
 
 
 def custom_operator(source, value):
-    return column == value
+    return source == value
 
 
 class TeamFilter(filters.Filter):
     
     team_size = fields.IntegerField(Team.team_size, operator=custom_operator)
 ```
```

### Comparing `sqlaf-1.0.0/pyproject.toml` & `sqlaf-1.1.0/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "sqlaf"
-version = "1.0.0"
+version = "1.1.0"
 authors = [
   { name="iamstej", email="" },
 ]
 description = "Library for transforming query parameters into SQLAlchemy filters in a structured and organised manner."
 readme = "README.md"
 license = { file="LICENSE" }
 requires-python = ">=3.7"
```

### Comparing `sqlaf-1.0.0/PKG-INFO` & `sqlaf-1.1.0/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sqlaf
-Version: 1.0.0
+Version: 1.1.0
 Summary: Library for transforming query parameters into SQLAlchemy filters in a structured and organised manner.
 Project-URL: Homepage, https://github.com/iamstej/sqlaf
 Project-URL: Bug Tracker, https://github.com/iamstej/sqlaf/issues
 Author: iamstej
 License: Copyright 2022 iamstej.com
         
         Licensed under the Apache License, Version 2.0 (the "License");
@@ -25,14 +25,15 @@
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 
 # sqlaf
 
 [![PyPI pyversions](https://img.shields.io/pypi/pyversions/sqlaf.svg)](https://pypi.python.org/pypi/sqlaf/)
 [![pypi](https://img.shields.io/pypi/v/sqlaf)](https://pypi.org/project/sqlaf/)
+[![codecov](https://codecov.io/gh/iamstej/sqlaf/branch/main/graph/badge.svg?token=D1L129C3NF)](https://codecov.io/gh/iamstej/sqlaf)
 
 sqlaf is a library for transforming query parameters into SQLAlchemy filters in a structured and organised manner
 
 ## Installation
 
 Use the package manager [pip](https://pip.pypa.io/en/stable/) to install sqlaf.
 
@@ -53,14 +54,26 @@
 class TeamFilter(filters.Filter):
 
     founded_date = fields.DateField(Team.founded_date, operator="gte")
     name = fields.CharField(Team.name, operator="icontains")
     size = fields.IntegerField(Team.size, operator="eq")
 ```
 
+If you want to allow a specific value passed from a query parameter to be treated as `None`, use the `null_values` param e.g.
+
+```python
+
+from sqlaf import filters, fields
+
+class TeamFilter(filters.Filter):
+
+    size = fields.IntegerField(Team.size, operator="eq", null_values=["null", "-1"])
+```
+
+
 ### Using a Filter
 
 A filter class can be used in the following ways:
 
 #### Query parameter string with "?"
 ```python
 query = session.query(Team)
@@ -122,15 +135,15 @@
 To extend the above operators, you can create custom operators:
 
 ```python
 from sqlaf import filters, fields
 
 
 def custom_operator(source, value):
-    return column == value
+    return source == value
 
 
 class TeamFilter(filters.Filter):
     
     team_size = fields.IntegerField(Team.team_size, operator=custom_operator)
 ```
```

