# Comparing `tmp/async_state_machine-0.0.2.tar.gz` & `tmp/async_state_machine-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "async_state_machine-0.0.2.tar", max compression
+gzip compressed data, was "async_state_machine-0.0.3.tar", max compression
```

## Comparing `async_state_machine-0.0.2.tar` & `async_state_machine-0.0.3.tar`

### file list

```diff
@@ -1,13 +1,15 @@
--rw-r--r--   0        0        0        0 2023-02-22 15:06:07.234717 async_state_machine-0.0.2/README.md
--rw-r--r--   0        0        0      377 2023-02-22 15:06:07.238716 async_state_machine-0.0.2/async_state_machine/__init__.py
--rw-r--r--   0        0        0     1985 2023-02-22 15:06:07.238716 async_state_machine-0.0.2/async_state_machine/exceptions.py
--rw-r--r--   0        0        0      366 2023-02-22 15:06:07.242717 async_state_machine-0.0.2/async_state_machine/shared.py
--rw-r--r--   0        0        0      113 2023-02-22 15:06:07.238716 async_state_machine-0.0.2/async_state_machine/state/__init__.py
--rw-r--r--   0        0        0      630 2023-02-22 15:06:07.238716 async_state_machine-0.0.2/async_state_machine/state/coro_wrappers.py
--rw-r--r--   0        0        0     4431 2023-02-22 15:06:07.238716 async_state_machine-0.0.2/async_state_machine/state/stage_callbacks.py
--rw-r--r--   0        0        0     7144 2023-02-22 15:06:07.238716 async_state_machine-0.0.2/async_state_machine/state/state.py
--rw-r--r--   0        0        0     2736 2023-02-22 15:06:07.238716 async_state_machine-0.0.2/async_state_machine/state_machine.py
--rw-r--r--   0        0        0      161 2023-02-22 15:06:07.238716 async_state_machine-0.0.2/async_state_machine/states_enum.py
--rw-r--r--   0        0        0      216 2023-02-22 15:06:07.238716 async_state_machine-0.0.2/async_state_machine/typings.py
--rw-r--r--   0        0        0      861 2023-03-31 16:16:15.075074 async_state_machine-0.0.2/pyproject.toml
--rw-r--r--   0        0        0      315 1970-01-01 00:00:00.000000 async_state_machine-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-03-31 19:08:14.905097 async_state_machine-0.0.3/README.md
+-rw-r--r--   0        0        0      430 2023-04-01 15:55:42.998340 async_state_machine-0.0.3/async_state_machine/__init__.py
+-rw-r--r--   0        0        0      172 2023-04-01 13:02:08.510038 async_state_machine-0.0.3/async_state_machine/const.py
+-rw-r--r--   0        0        0     1985 2023-03-31 19:08:14.905097 async_state_machine-0.0.3/async_state_machine/exceptions.py
+-rw-r--r--   0        0        0      366 2023-03-31 19:08:14.905097 async_state_machine-0.0.3/async_state_machine/shared.py
+-rw-r--r--   0        0        0      170 2023-03-31 19:08:14.905097 async_state_machine-0.0.3/async_state_machine/state/__init__.py
+-rw-r--r--   0        0        0      687 2023-04-01 13:14:02.774686 async_state_machine-0.0.3/async_state_machine/state/coro_wrappers.py
+-rw-r--r--   0        0        0     4379 2023-04-01 11:50:11.371780 async_state_machine-0.0.3/async_state_machine/state/stage_callbacks.py
+-rw-r--r--   0        0        0     6300 2023-04-01 16:06:48.658471 async_state_machine-0.0.3/async_state_machine/state/state.py
+-rw-r--r--   0        0        0     3405 2023-04-01 16:05:29.571767 async_state_machine-0.0.3/async_state_machine/state/state_runner.py
+-rw-r--r--   0        0        0     3105 2023-04-01 11:48:14.041256 async_state_machine-0.0.3/async_state_machine/state_machine.py
+-rw-r--r--   0        0        0      161 2023-03-31 19:08:14.905097 async_state_machine-0.0.3/async_state_machine/states_enum.py
+-rw-r--r--   0        0        0      216 2023-03-31 19:08:14.905097 async_state_machine-0.0.3/async_state_machine/typings.py
+-rw-r--r--   0        0        0      880 2023-04-08 18:02:11.166640 async_state_machine-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0      359 1970-01-01 00:00:00.000000 async_state_machine-0.0.3/PKG-INFO
```

### Comparing `async_state_machine-0.0.2/async_state_machine/exceptions.py` & `async_state_machine-0.0.3/async_state_machine/exceptions.py`

 * *Files identical despite different names*

### Comparing `async_state_machine-0.0.2/async_state_machine/state/coro_wrappers.py` & `async_state_machine-0.0.3/async_state_machine/state/coro_wrappers.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 """Обертки для запуска корутин."""
 
-
 import asyncio
 
+from ..const import INFINITE_CORO_SLEEP
 from ..typings import TCallback
 
 
 class CoroWrappers(object):
     """Обертки для запуска корутин."""
 
     @staticmethod
     async def infinite(coro_func: TCallback) -> None:
         """Корутина вызывается в цикле бесконечно."""
         while True:  # noqa: WPS457
             await coro_func()
-            await asyncio.sleep(0)
+            await asyncio.sleep(INFINITE_CORO_SLEEP)
 
     @staticmethod
     async def single(coro_func: TCallback) -> None:
         """Корутина вызывается один раз."""
         await coro_func()
```

### Comparing `async_state_machine-0.0.2/async_state_machine/state/stage_callbacks.py` & `async_state_machine-0.0.3/async_state_machine/state/stage_callbacks.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,22 +1,20 @@
 """Запуск функций для этапа состояния."""
 
 import asyncio
-import logging
-from typing import Any, Callable, Coroutine, Final, Literal
+from typing import Any, Callable, Coroutine, Final, Literal, Self
+
+from loguru import logger
 
 from ..exceptions import NewStateData, NewStateException, StateMachineError
 from ..states_enum import StatesEnum
 from ..typings import TCallback, TCallbackCollection
 
-log = logging.getLogger(__name__)
-log.setLevel(logging.DEBUG)
-
 
-EXC_TIMEOUT: Final[str] = "Timeout occur in state {name}, stage {stage}"
+EXC_TIMEOUT: Final[str] = "Timeout occur {name}|{stage}"
 EXC_TIMEOUT_WITHOUT_TARGET: Final[
     str
 ] = "{base_msg}, but target state not specified"
 
 
 class StageCallbacks(object):
     """Запуск функций для этапа состояния."""
@@ -25,14 +23,15 @@
         self,
         callbacks: TCallbackCollection | None,
         timeout: float | None,
         timeout_to_state: StatesEnum | None,
         name: StatesEnum,
         stage: Literal["on_enter", "on_run", "on_exit"],
         coro_wrapper: Callable[[TCallback], Coroutine[Any, Any, None]],
+        logging_level: int = 0,  # TODO - remove
     ) -> None:
         """Запуск функций для этапа состояния."""
         self.__callbacks: TCallbackCollection | None
         self.__coro_wrapper: Any
         self.__name: StatesEnum
         self.__timeout: float | None
         self.__timeout_to_state: StatesEnum | None
@@ -43,44 +42,43 @@
         self.__name = name
         self.__stage = stage
         self.__timeout = timeout
         self.__timeout_to_state = timeout_to_state
 
     async def run(self) -> None:
         """Запуск."""
-        log.debug(
-            "Start state {name}, stage {stage}".format(
+        logger.debug(
+            "{name}|{stage}|start".format(
                 name=self.__name,
                 stage=self.__stage,
             ),
         )
         new_state_data: NewStateData | None = None
         try:
             await self.__run_taskgroup()
         except* asyncio.TimeoutError:
             self.__except_timeout()
         except* NewStateException as exc:
             new_state_data = self.__except_new_state(exc)
-        log.debug(
-            "End state {name}, stage {stage}".format(
+        logger.debug(
+            "{name}|{stage}|end".format(
                 name=self.__name,
                 stage=self.__stage,
             ),
         )
         if new_state_data is not None:
             raise NewStateException.reraise(new_state_data, self.__name)
 
-    def config_timeout(
-        self,
-        timeout: float,
-        to_state: StatesEnum | None,
-    ) -> None:
-        """Изменить таймаут на выполнение."""
-        self.__timeout = timeout
-        self.__timeout_to_state = to_state
+    def config_logging(self, logging_level: int) -> Self:
+        """Конфигурировать уровень логгирования.
+
+        TODO - remove
+        """
+        # log.setLevel(logging_level)
+        return self
 
     async def __run_taskgroup(self) -> None:
         """Запуск."""
         async with asyncio.TaskGroup() as tg:
             self.__create_tasks(tg)
 
     def __create_tasks(self, tg: asyncio.TaskGroup) -> None:
@@ -93,37 +91,37 @@
                     fut=self.__coro_wrapper(task),
                     timeout=self.__timeout,
                 ),
             )
 
     def __except_timeout(self) -> None:
         """Обработка превышения времени выполнения."""
-        log.debug(EXC_TIMEOUT.format(name=self.__name, stage=self.__stage))
+        logger.debug(EXC_TIMEOUT.format(name=self.__name, stage=self.__stage))
         if self.__timeout_to_state is None:
             msg = EXC_TIMEOUT_WITHOUT_TARGET.format(
                 base_msg=EXC_TIMEOUT.format(
                     name=self.__name,
                     stage=self.__stage,
                 ),
             )
-            log.error(msg)
+            logger.error(msg)
             raise StateMachineError(msg)
         raise NewStateException(
             new_state=self.__timeout_to_state,
         )
 
     def __except_new_state(
         self,
         exc: ExceptionGroup[NewStateException],
     ) -> NewStateData:
         """Обработка перехода в новое состояние."""
         new_state_data = exc.exceptions[0]
         if isinstance(new_state_data, NewStateException):
             exc_data = new_state_data.exception_data
-            log.debug(
+            logger.debug(
                 "State {name}, stage {stage}, new state: {new_name}".format(
                     name=self.__name,
                     stage=self.__stage,
                     new_name=exc_data.new_state,
                 ),
             )
             return exc_data
```

### Comparing `async_state_machine-0.0.2/async_state_machine/state/state.py` & `async_state_machine-0.0.3/async_state_machine/state/state.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,36 +1,40 @@
-"""Состояние."""
+"""Строитель для создания State."""
 
+from dataclasses import dataclass
 from typing import Final, Self
 
-from ..exceptions import NewStateData, NewStateException, StateMachineError
-from ..shared import exc_group_to_exc
+from ..exceptions import StateMachineError
 from ..states_enum import StatesEnum
 from .coro_wrappers import CoroWrappers
 from .stage_callbacks import StageCallbacks, TCallbackCollection
+from .state_runner import StateRunner
 
 EXC_NO_ON_RUN: Final[str] = "No callbacks on on_run input, state: {name}"
-EXC_COMPL_NO_NEWSTATE: Final[
-    str
-] = "State '{name}' completed, but NewStateException not raised."
-
 DEFAULT_TIMEOUT: Final[float] = 2.0
 
 
+@dataclass
+class _StageData(object):
+    callbacks: TCallbackCollection | None
+    timeout: float | None
+    timeout_to_state: StatesEnum | None
+
+
 class State(object):
-    """Состояние."""
+    """Строитель для создания State."""
 
     def __init__(  # noqa: WPS211
         self,
         name: StatesEnum,
         on_run: TCallbackCollection,
         on_enter: TCallbackCollection | None = None,
         on_exit: TCallbackCollection | None = None,
     ) -> None:
-        """Состояние.
+        """Строитель для создания State.
 
         Parameters
         ----------
         name: StatesEnum
             Название состояния из перечисления
         on_enter: TCallbackCollection
             Функции для выполения в стадии on_enter
@@ -41,65 +45,36 @@
 
         Raises
         ------
         StateMachineError
             не указаны задачи on_run
         """
         self.__name: StatesEnum
-        self.__on_enter: StageCallbacks
-        self.__on_run: StageCallbacks
-        self.__on_exit: StageCallbacks
-        self.__new_state_data: NewStateData | None
+        self.__on_enter: _StageData
+        self.__on_run: _StageData
+        self.__on_exit: _StageData
+        self.__logging_level: int
 
         if not on_run:
             raise StateMachineError(EXC_NO_ON_RUN.format(name=name))
         self.__name = name
-        self.__on_enter = StageCallbacks(
+        self.__on_enter = _StageData(
             callbacks=on_enter,
             timeout=DEFAULT_TIMEOUT,
             timeout_to_state=None,
-            name=self.__name,
-            stage="on_enter",
-            coro_wrapper=CoroWrappers.single,
         )
-        self.__on_run = StageCallbacks(
+        self.__on_run = _StageData(
             callbacks=on_run,
             timeout=None,
             timeout_to_state=None,
-            name=self.__name,
-            stage="on_run",
-            coro_wrapper=CoroWrappers.infinite,
         )
-        self.__on_exit = StageCallbacks(
+        self.__on_exit = _StageData(
             callbacks=on_exit,
             timeout=DEFAULT_TIMEOUT,
             timeout_to_state=None,
-            name=self.__name,
-            stage="on_exit",
-            coro_wrapper=CoroWrappers.single,
-        )
-        self.__new_state_data = None
-
-    @property
-    def name(self) -> StatesEnum:
-        """Имя состояния."""
-        return self.__name
-
-    async def run(self) -> None:
-        """Задача для асинхронного выполнения, вызывается из StateMachine."""
-        await self.__run_on_enter()
-        await self.__run_on_run()
-        await self.__run_on_exit()
-        if self.__new_state_data is None:
-            raise StateMachineError(
-                EXC_COMPL_NO_NEWSTATE.format(name=self.__name),
-            )
-        raise NewStateException.reraise(
-            new_state_data=self.__new_state_data,
-            active_state=self.__name,
         )
 
     def config_timeout_on_enter(
         self,
         timeout: float,
         to_state: StatesEnum | None = None,
     ) -> Self:
@@ -114,15 +89,16 @@
             Если задано None, то возникнет исключение StateMachineError.
             По-умолчанию None.
 
         Returns
         -------
         Измененный объект состояния
         """
-        self.__on_enter.config_timeout(timeout, to_state)
+        self.__on_enter.timeout = timeout
+        self.__on_enter.timeout_to_state = to_state
         return self
 
     def config_timeout_on_run(
         self,
         timeout: float,
         to_state: StatesEnum | None = None,
     ) -> Self:
@@ -137,15 +113,16 @@
             Если задано None, то возникнет исключение StateMachineError.
             По-умолчанию None.
 
         Returns
         -------
         Измененный объект состояния
         """
-        self.__on_run.config_timeout(timeout, to_state)
+        self.__on_run.timeout = timeout
+        self.__on_run.timeout_to_state = to_state
         return self
 
     def config_timeout_on_exit(
         self,
         timeout: float,
         to_state: StatesEnum | None = None,
     ) -> Self:
@@ -160,44 +137,50 @@
             Если задано None, то возникнет исключение StateMachineError.
             По-умолчанию None.
 
         Returns
         -------
         Измененный объект состояния
         """
-        self.__on_exit.config_timeout(timeout, to_state)
+        self.__on_exit.timeout = timeout
+        self.__on_exit.timeout_to_state = to_state
+        return self
+
+    def config_logging(self, logging_level: int) -> Self:
+        """Конфигурировать уровень логгирования."""
         return self
 
-    async def __run_on_enter(self) -> None:
-        state_machine_error: str | None = None
-        try:
-            await self.__on_enter.run()
-        except* NewStateException as exc_gr:
-            self.__new_state_data = exc_group_to_exc(exc_gr).exception_data
-        except* StateMachineError as exc_gr:
-            state_machine_error = exc_group_to_exc(exc_gr).message
-        if state_machine_error is not None:
-            raise StateMachineError(state_machine_error)
-
-    async def __run_on_run(self) -> None:
-        if self.__new_state_data is not None:
-            return
-        state_machine_error: str | None = None
-        try:
-            await self.__on_run.run()
-        except* NewStateException as exc_gr:
-            self.__new_state_data = exc_group_to_exc(exc_gr).exception_data
-        except* StateMachineError as exc_gr:
-            state_machine_error = exc_group_to_exc(exc_gr).message
-        if state_machine_error is not None:
-            raise StateMachineError(state_machine_error)
-
-    async def __run_on_exit(self) -> None:
-        state_machine_error: str | None = None
-        try:
-            await self.__on_exit.run()
-        except* NewStateException as exc_gr:
-            self.__new_state_data = exc_group_to_exc(exc_gr).exception_data
-        except* StateMachineError as exc_gr:
-            state_machine_error = exc_group_to_exc(exc_gr).message
-        if state_machine_error is not None:
-            raise StateMachineError(state_machine_error)
+    def build(self) -> StateRunner:
+        """Создание состояния.
+
+        Вызывается из StateMachine.
+        """
+        return StateRunner(
+            name=self.__name,
+            on_enter=StageCallbacks(
+                callbacks=self.__on_enter.callbacks,
+                timeout=self.__on_enter.timeout,
+                timeout_to_state=self.__on_enter.timeout_to_state,
+                name=self.__name,
+                stage="on_enter",
+                coro_wrapper=CoroWrappers.single,
+                logging_level=0,
+            ),
+            on_run=StageCallbacks(
+                callbacks=self.__on_run.callbacks,
+                timeout=self.__on_run.timeout,
+                timeout_to_state=self.__on_run.timeout_to_state,
+                name=self.__name,
+                stage="on_run",
+                coro_wrapper=CoroWrappers.infinite,
+                logging_level=0,
+            ),
+            on_exit=StageCallbacks(
+                callbacks=self.__on_exit.callbacks,
+                timeout=self.__on_exit.timeout,
+                timeout_to_state=self.__on_exit.timeout_to_state,
+                name=self.__name,
+                stage="on_exit",
+                coro_wrapper=CoroWrappers.single,
+                logging_level=0,
+            ),
+        )
```

### Comparing `async_state_machine-0.0.2/async_state_machine/state_machine.py` & `async_state_machine-0.0.3/async_state_machine/state_machine.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """Диаграмма состояний."""
 
 import asyncio
-from typing import Final, Iterable, Type
+from typing import Final, Iterable, Self, Type
 
 from .exceptions import NewStateException, StateMachineError
-from .state import State
+from .state import State, StateRunner
 from .states_enum import StatesEnum
 
 EXC_NAME_NOT_FOUND: Final[str] = "State with name {name} not found."
 EXC_NOT_USED_STATES: Final[str] = "Need to define states: {states}"
 EXC_REUSE_STATE: Final[str] = "Several use state with name: {name}"
 
 
@@ -18,39 +18,46 @@
     def __init__(
         self,
         states: Iterable[State],
         states_enum: Type[StatesEnum],
         init_state: StatesEnum,
     ) -> None:
         """Определение диаграммы состояний."""
-        self.__active_state: State
+        self.__active_state: StateRunner
         self.__state_names: set[str]
-        self.__states: Iterable[State]
+        self.__states: Iterable[StateRunner]
 
-        self.__states = states
+        self.__states = [state.build() for state in states]
         self.__state_names = {state.value for state in states_enum}
         self.__check_state_names()
         self.__active_state = self.__set_init_state(init_state)
 
     @property
-    def active_state(self) -> State:
+    def active_state(self) -> StatesEnum:
         """Активное состояние."""
-        return self.__active_state
+        return self.__active_state.name
 
     async def run(self) -> None:
         """Задача для асинхронного выполнения."""
         while True:
             try:
                 await self.__active_state.run()
             except NewStateException as exc:
                 new_state = exc.exception_data.new_state
                 self.__active_state = self.__find_state_by_name(new_state)
             await asyncio.sleep(0)
 
-    def __set_init_state(self, init_state: StatesEnum) -> State:
+    def config_logging(self, logging_level: int) -> Self:
+        """Конфигурировать уровень логгирования."""
+        # log.setLevel(logging_level)
+        for state in self.__states:
+            state.config_logging(logging_level)
+        return self
+
+    def __set_init_state(self, init_state: StatesEnum) -> StateRunner:
         for state in self.__states:
             if state.name == init_state:
                 return state
         raise ValueError(
             "Init state {0} not found in states array".format(init_state),
         )
 
@@ -67,12 +74,12 @@
         for state in self.__states:
             name = state.name.value
             if name in names:
                 raise StateMachineError(EXC_REUSE_STATE.format(name=name))
             names.add(name)
         return names
 
-    def __find_state_by_name(self, name: StatesEnum) -> State:
+    def __find_state_by_name(self, name: StatesEnum) -> StateRunner:
         for state in self.__states:
             if state.name == name:
                 return state
         raise StateMachineError(EXC_NAME_NOT_FOUND.format(name=name))
```

### Comparing `async_state_machine-0.0.2/pyproject.toml` & `async_state_machine-0.0.3/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -5,23 +5,24 @@
 
 [tool.black]
 line-length = 80
 
 
 [tool.poetry]
 name = "async_state_machine"
-version = "0.0.2"
+version = "0.0.3"
 description = ""
 authors = ["konstantin-dudersky <konstantin.dudersky@gmail.com>"]
 readme = "README.md"
 packages = [{ include = "async_state_machine" }]
 
 
 [tool.poetry.dependencies]
-python = "^3.11"
+python = "3.11.*"
+loguru = "^0.6.0"
 
 
 [tool.poetry.group.dev.dependencies]
 black = "*"
 pytest = "7.2.0"
 wemake-python-styleguide = "0.17.0"
```

