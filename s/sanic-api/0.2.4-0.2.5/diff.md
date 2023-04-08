# Comparing `tmp/sanic-api-0.2.4.tar.gz` & `tmp/sanic-api-0.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sanic-api-0.2.4.tar", last modified: Sun Feb  5 04:13:29 2023, max compression
+gzip compressed data, was "sanic-api-0.2.5.tar", last modified: Sat Apr  8 16:27:09 2023, max compression
```

## Comparing `sanic-api-0.2.4.tar` & `sanic-api-0.2.5.tar`

### file list

```diff
@@ -1,25 +1,38 @@
--rw-rw-rw-   0        0        0        0 2022-12-19 09:31:30.146039 sanic-api-0.2.4/example/__init__.py
--rw-rw-rw-   0        0        0     1857 2023-02-05 04:12:06.717394 sanic-api-0.2.4/example/app.py
--rw-rw-rw-   0        0        0     1090 2022-12-19 09:31:30.145040 sanic-api-0.2.4/LICENSE.txt
--rw-rw-rw-   0        0        0     1846 2023-02-05 04:12:09.198872 sanic-api-0.2.4/pyproject.toml
--rw-rw-rw-   0        0        0     1838 2022-12-19 09:36:17.115995 sanic-api-0.2.4/README.MD
--rw-rw-rw-   0        0        0      369 2023-02-05 03:39:25.051397 sanic-api-0.2.4/sanic_api/__init__.py
--rw-rw-rw-   0        0        0       53 2023-02-05 03:39:25.052397 sanic-api-0.2.4/sanic_api/api/__init__.py
--rw-rw-rw-   0        0        0     4906 2023-02-05 03:57:56.987254 sanic-api-0.2.4/sanic_api/api/api.py
--rw-rw-rw-   0        0        0     1129 2023-02-05 03:57:56.987254 sanic-api-0.2.4/sanic_api/api/exception.py
--rw-rw-rw-   0        0        0      731 2023-02-05 03:57:56.988254 sanic-api-0.2.4/sanic_api/api/extend.py
--rw-rw-rw-   0        0        0     1197 2023-02-05 03:39:25.054399 sanic-api-0.2.4/sanic_api/api/handle_exception.py
--rw-rw-rw-   0        0        0     2047 2023-02-05 03:57:56.989253 sanic-api-0.2.4/sanic_api/api/validators.py
--rw-rw-rw-   0        0        0        0 2023-02-05 03:39:25.056399 sanic-api-0.2.4/sanic_api/config/__init__.py
--rw-rw-rw-   0        0        0     3338 2023-02-05 03:57:56.989253 sanic-api-0.2.4/sanic_api/config/base.py
--rw-rw-rw-   0        0        0      404 2023-02-05 03:39:25.057398 sanic-api-0.2.4/sanic_api/config/sanic_api.py
--rw-rw-rw-   0        0        0     1709 2023-02-05 03:57:56.990254 sanic-api-0.2.4/sanic_api/enum.py
--rw-rw-rw-   0        0        0       34 2023-02-05 03:39:25.058399 sanic-api-0.2.4/sanic_api/logger/__init__.py
--rw-rw-rw-   0        0        0     2620 2023-02-05 03:57:56.991254 sanic-api-0.2.4/sanic_api/logger/config.py
--rw-rw-rw-   0        0        0     1960 2023-02-05 03:39:25.059399 sanic-api-0.2.4/sanic_api/logger/extend.py
--rw-rw-rw-   0        0        0     1429 2023-02-05 03:39:25.060398 sanic-api-0.2.4/sanic_api/logger/sanic_http.py
--rw-rw-rw-   0        0        0      723 2023-02-05 03:39:25.061398 sanic-api-0.2.4/sanic_api/model.py
--rw-rw-rw-   0        0        0      174 2023-02-05 03:37:04.544075 sanic-api-0.2.4/sanic_api/openapi/__init__.py
--rw-rw-rw-   0        0        0     5931 2023-02-05 03:57:56.991254 sanic-api-0.2.4/sanic_api/openapi/openapi.py
--rw-rw-rw-   0        0        0      722 2023-02-05 03:39:25.063398 sanic-api-0.2.4/sanic_api/utils.py
--rw-rw-rw-   0        0        0     2102 2023-02-05 04:13:29.049771 sanic-api-0.2.4/PKG-INFO
+-rw-r--r--   0        0        0        0 2022-12-19 09:31:30.146039 sanic-api-0.2.5/example/__init__.py
+-rw-r--r--   0        0        0      624 2023-04-08 16:25:11.460645 sanic-api-0.2.5/example/__main__.py
+-rw-r--r--   0        0        0       35 2023-04-08 16:25:11.461646 sanic-api-0.2.5/example/api/__init__.py
+-rw-r--r--   0        0        0       30 2023-04-08 16:25:11.462645 sanic-api-0.2.5/example/api/t1/__init__.py
+-rw-r--r--   0        0        0      640 2023-04-08 16:25:11.462645 sanic-api-0.2.5/example/api/t1/t1.py
+-rw-r--r--   0        0        0       30 2023-04-08 16:25:11.463645 sanic-api-0.2.5/example/api/t2/__init__.py
+-rw-r--r--   0        0        0      257 2023-04-08 16:25:11.463645 sanic-api-0.2.5/example/api/t2/t2.py
+-rw-r--r--   0        0        0       30 2023-04-08 16:25:11.464645 sanic-api-0.2.5/example/api/t2/t3/__init__.py
+-rw-r--r--   0        0        0      257 2023-04-08 16:25:11.464645 sanic-api-0.2.5/example/api/t2/t3/t3.py
+-rw-r--r--   0        0        0     1933 2023-04-08 16:25:11.465646 sanic-api-0.2.5/example/api/user.py
+-rw-r--r--   0        0        0     1819 2023-04-08 16:25:11.466645 sanic-api-0.2.5/example/api/validator.py
+-rw-r--r--   0        0        0     1272 2023-04-08 16:25:11.467646 sanic-api-0.2.5/example/app.py
+-rw-r--r--   0        0        0      144 2023-04-08 16:25:11.467646 sanic-api-0.2.5/example/settings.py
+-rw-r--r--   0        0        0     1090 2022-12-19 09:31:30.145040 sanic-api-0.2.5/LICENSE.txt
+-rw-r--r--   0        0        0     1651 2023-04-08 16:25:13.997538 sanic-api-0.2.5/pyproject.toml
+-rw-r--r--   0        0        0     1824 2023-04-08 16:25:13.996538 sanic-api-0.2.5/README.MD
+-rw-r--r--   0        0        0      369 2023-02-05 03:39:25.051397 sanic-api-0.2.5/sanic_api/__init__.py
+-rw-r--r--   0        0        0       53 2023-02-05 03:39:25.052397 sanic-api-0.2.5/sanic_api/api/__init__.py
+-rw-r--r--   0        0        0     5663 2023-04-08 16:25:11.470648 sanic-api-0.2.5/sanic_api/api/api.py
+-rw-r--r--   0        0        0     1262 2023-04-08 16:25:11.471648 sanic-api-0.2.5/sanic_api/api/exception.py
+-rw-r--r--   0        0        0      731 2023-02-05 03:57:56.988254 sanic-api-0.2.5/sanic_api/api/extend.py
+-rw-r--r--   0        0        0     1267 2023-04-08 16:25:11.472646 sanic-api-0.2.5/sanic_api/api/handle_exception.py
+-rw-r--r--   0        0        0     1077 2023-04-08 16:25:11.473648 sanic-api-0.2.5/sanic_api/api/model.py
+-rw-r--r--   0        0        0     2154 2023-04-08 16:25:11.474646 sanic-api-0.2.5/sanic_api/api/validators.py
+-rw-r--r--   0        0        0       70 2023-04-08 16:25:11.474646 sanic-api-0.2.5/sanic_api/config/__init__.py
+-rw-r--r--   0        0        0     3339 2023-04-08 16:25:11.475649 sanic-api-0.2.5/sanic_api/config/base.py
+-rw-r--r--   0        0        0      681 2023-04-08 16:25:11.476646 sanic-api-0.2.5/sanic_api/config/sanic.py
+-rw-r--r--   0        0        0      410 2023-04-08 16:25:11.477647 sanic-api-0.2.5/sanic_api/config/sanic_api.py
+-rw-r--r--   0        0        0      765 2023-04-08 16:25:11.477647 sanic-api-0.2.5/sanic_api/config/setting.py
+-rw-r--r--   0        0        0     2128 2023-04-08 16:25:11.478649 sanic-api-0.2.5/sanic_api/enum.py
+-rw-r--r--   0        0        0       34 2023-02-05 03:39:25.058399 sanic-api-0.2.5/sanic_api/logger/__init__.py
+-rw-r--r--   0        0        0     2588 2023-04-08 16:25:11.479786 sanic-api-0.2.5/sanic_api/logger/config.py
+-rw-r--r--   0        0        0     1982 2023-04-08 16:25:11.480646 sanic-api-0.2.5/sanic_api/logger/extend.py
+-rw-r--r--   0        0        0     2170 2023-04-08 16:25:11.481646 sanic-api-0.2.5/sanic_api/logger/sanic_http.py
+-rw-r--r--   0        0        0      153 2023-04-08 16:25:11.481646 sanic-api-0.2.5/sanic_api/openapi/__init__.py
+-rw-r--r--   0        0        0     4249 2023-04-08 16:25:11.482646 sanic-api-0.2.5/sanic_api/openapi/openapi.py
+-rw-r--r--   0        0        0     2882 2023-04-08 16:25:11.483646 sanic-api-0.2.5/sanic_api/utils.py
+-rw-r--r--   0        0        0     2088 1970-01-01 00:00:00.000000 sanic-api-0.2.5/PKG-INFO
```

### Comparing `sanic-api-0.2.4/LICENSE.txt` & `sanic-api-0.2.5/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `sanic-api-0.2.4/pyproject.toml` & `sanic-api-0.2.5/pyproject.toml`

 * *Files 21% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 [project]
 name = "sanic-api"
-version = "0.2.4"
+version = "0.2.5"
 description = "Sanic 框架实用API工具集，拥有自动生成文档、参数校验、配置的导入、日志功能的优化等功能，更好的助力接口的开发"
 authors = [
     { name = "昊色居士", email = "xhrtxh@gmail.com" },
 ]
 dependencies = [
-    "sanic>=22.9.1",
+    "sanic>=22.12",
     "pydantic>=1.10.2",
-    "sanic-ext>=22.9.1",
+    "sanic-ext>=22.12",
     "loguru>=0.6.0",
     "pygments>=2.13.0",
-    "types-PyYAML>=6.0.12.2",
     "ujson>=5.7.0",
+    "orjson>=3.8.6",
 ]
 requires-python = ">=3.8"
 readme = "README.MD"
 
 [project.license]
 text = "MIT"
 
@@ -31,14 +31,17 @@
 [tool.isort]
 profile = "black"
 
 [tool.mypy]
 python_version = "3.8"
 ignore_missing_imports = true
 
+[tool.black]
+line-length = 120
+
 [tool.ruff]
 select = [
     "E",
     "W",
     "F",
     "C",
     "B",
@@ -80,27 +83,14 @@
 [tool.pdm]
 source = [
     { name = "pypi", url = "https://pypi.tuna.tsinghua.edu.cn/simple", verify_ssl = true },
 ]
 
 [tool.pdm.dev-dependencies]
 dev = [
-    "black>=22.10.0",
-    "isort>=5.10.1",
-    "autoflake>=2.0.0",
-    "mypy>=0.991",
+    "pre-commit>=3.0.4",
     "types-ujson>=5.7.0.0",
+    "types-PyYAML>=6.0.12.2",
 ]
 
 [tool.pdm.scripts]
-autoflake = "autoflake --in-place --recursive sanic_api"
-isort = "isort sanic_api"
-black = "black sanic_api"
-mypy = "mypy sanic_api"
-
-[tool.pdm.scripts.check]
-composite = [
-    "autoflake",
-    "isort",
-    "black",
-    "mypy",
-]
+check = "pdm run pre-commit run --all-files"
```

### Comparing `sanic-api-0.2.4/README.MD` & `sanic-api-0.2.5/README.MD`

 * *Files 8% similar despite different names*

```diff
@@ -17,25 +17,25 @@
 
 - 使用`loguru`库代替官方`logging`日志库，并对访问日志进行扩展，支持打印接口耗时、接口参数
 
 - 使用`{code: 0, data: null, msg: ""}`样式的接口返回
 
 - 对接口中的异常进行拦截，及自定义错误码
 
+- 接口返回样式可自定义配置
+
 ## 截图
 
 ## 路线图
 
-- 接口返回样式可自定义配置
-
-- API接口文档生成时可以定义接口详细描述
+- 增加一键生成预设项目cli命令
 
 - 编写详细文档
 
-- API接口增加请求头、URL路径参数收集和校验
+- API接口增加请求头、URL路径参数收集和校验:
 
 ## 安装
 
 使用 pip 安装 sanic-api
 
 ```bash
   pip install sanic-api
```

### Comparing `sanic-api-0.2.4/sanic_api/api/api.py` & `sanic-api-0.2.5/sanic_api/api/api.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,72 +1,111 @@
+import functools
 from abc import ABCMeta
-from dataclasses import dataclass
-from functools import partial
 from typing import Any, Callable, Dict, Optional
 
-# noinspection PyUnresolvedReferences
-import ujson
-from pydantic import BaseModel
+from pydantic import BaseModel, Field
 from pydantic import ValidationError as PyDanticValidationError
 from sanic import HTTPResponse, Sanic
 from sanic.response import json
 
 from sanic_api.api.exception import ValidationError
-from sanic_api.enum import ParamEnum, RespCodeEnum
-from sanic_api.model import ListModel
+from sanic_api.api.model import ListRespModel, ResponseModel
+from sanic_api.enum import EnumBase, ParamEnum, RespCodeEnum
 from sanic_api.utils import json_dumps
 
 
-@dataclass
+def get_resp_tmp(key: str, default):
+    """
+    获取响应字段模板
+    """
+    app = Sanic.get_app()
+    sanic_api: dict = app.config.get("sanic_api", {})
+    return sanic_api.get(key, default)
+
+
 class Response:
-    # http响应码 默认是200
-    http_code: int = 200
-    # 自定义的响应头
-    headers: Optional[Dict[str, str]] = None
-    # 自定义的服务码
-    server_code: RespCodeEnum = RespCodeEnum.SUCCESS
-    # 返回的消息
-    message: str = ""
-    # 返回的数据
-    data: Any = None
+    def __init__(
+        self,
+        http_code: int = 200,
+        headers: Optional[Dict[str, str]] = None,
+        server_code: EnumBase = RespCodeEnum.SUCCESS,
+        message: str = "Success",
+        data: Any = None,
+        response_type: Optional[type] = None,
+    ):
+        """
+        初始化函数
+        Args:
+            http_code: http响应码 默认是200
+            headers: 自定义的响应头
+            server_code: 自定义的服务码
+            message: 返回的消息
+            data: 返回的数据
+        """
 
-    def json_resp(
-        self, dumps: Optional[Callable[[Any], Any]] = None, **kwargs
-    ) -> HTTPResponse:
+        self.http_code = http_code
+        self.headers = headers
+        self.message = message
+        response_type = response_type or Response.get_response_type(type(data))
+
+        if isinstance(data, ListRespModel):
+            data = data.to_list()
+        elif isinstance(data, BaseModel):
+            data = data.dict()
+
+        resp: ResponseModel = response_type()
+        code_tmp = get_resp_tmp("code_tmp", "code")
+        msg_tmp = get_resp_tmp("msg_tmp", "msg")
+        data_tmp = get_resp_tmp("data_tmp", "data")
+
+        setattr(resp, code_tmp, server_code)
+        setattr(resp, msg_tmp, message)
+        setattr(resp, data_tmp, data)
+
+        data = resp.dict()
+
+        self.data = data
+
+    def json_resp(self, default: Optional[Callable[[Any], Any]] = None) -> HTTPResponse:
         """
         返回json格式的响应
         Args:
-            dumps: 序列化方法，默认使用自定义的序列化方法
-            **kwargs: 序列化方法的参数
 
-        Returns:
-            返回一个sanic的HTTPResponse
         """
-
-        if isinstance(self.data, ListModel):
-            self.data = self.data.to_list()
-        elif isinstance(self.data, BaseModel):
-            self.data = self.data.dict()
-        else:
-            self.data = self.data
-
-        dumps = dumps or partial(ujson.dumps, ensure_ascii=False, default=json_dumps)
-        data = {
-            self._get_tmp("code_tmp", "code"): self.server_code.value,
-            self._get_tmp("msg_tmp", "msg"): self.message or self.server_code.desc,
-            self._get_tmp("data_tmp", "data"): self.data,
-        }
         return json(
-            body=data,
+            body=self.data,
             status=self.http_code,
             headers=self.headers,
-            dumps=dumps,
-            **kwargs,
+            dumps=functools.partial(json_dumps, default=default),
         )
 
+    @classmethod
+    def get_response_type(cls, data_type: type):
+        """
+        获取响应的类型
+        Args:
+            data_type: 响应中data的类型
+
+        Returns:
+
+        """
+        code_tmp = get_resp_tmp("code_tmp", "code")
+        msg_tmp = get_resp_tmp("msg_tmp", "msg")
+        data_tmp = get_resp_tmp("data_tmp", "data")
+
+        attr_dict = {
+            code_tmp: Field(title="业务响应码"),
+            msg_tmp: Field(title="响应消息"),
+            data_tmp: Field(title="响应数据"),
+            "__annotations__": {code_tmp: int, msg_tmp: str, data_tmp: data_type},
+        }
+        resp_name = data_type.__name__ if data_type.__name__ != "NoneType" else "Response"
+        response_type = type(resp_name, (ResponseModel,), attr_dict)
+        return response_type
+
     @staticmethod
     def _get_tmp(key: str, default):
         """
         获取字段模板
         """
         app = Sanic.get_app()
         sanic_api: dict = app.config.get("sanic_api", {})
@@ -78,37 +117,20 @@
     form_req: Optional[BaseModel] = None
     query_req: Optional[BaseModel] = None
     resp: Optional[Any] = None
     tags: list = []
     description: str = ""
 
     def __init__(self):
-        self.response_type = self.__class__.__annotations__.get("resp")
+        response_type = self.__class__.__annotations__.get("resp")
         self.json_req_type = self.__class__.__annotations__.get("json_req")
         self.form_req_type = self.__class__.__annotations__.get("form_req")
         self.query_req_type = self.__class__.__annotations__.get("query_req")
-        try:
-            self.resp = (
-                self.response_type()
-                if self.response_type and issubclass(self.response_type, BaseModel)
-                else ""
-            )
-        except PyDanticValidationError:
-            pass
-
-    def req_to_json(self):
-        data = {}
-        if self.json_req:
-            data["json"] = self.json_req.dict()
-        elif self.form_req:
-            data["form"] = self.form_req.dict()
-        if self.query_req:
-            data["query"] = self.query_req.dict()
-
-        return ujson.dumps(data, ensure_ascii=False, default=json_dumps, indent=4)
+        self.response_type = Response.get_response_type(response_type)
+        self.resp = response_type()
 
     def validate_params(self, req_data: dict, param_enum: ParamEnum):
         """
         验证参数，参数有问题抛出异常
         Args:
             req_data: 数据
             param_enum: 参数类型
@@ -127,28 +149,29 @@
             raise ValidationError(e.errors()) from e
 
     def json_resp(
         self,
         http_code: int = 200,
         headers: Optional[Dict[str, str]] = None,
         server_code: RespCodeEnum = RespCodeEnum.SUCCESS,
-        message: str = "",
+        message: str = "Success",
     ):
         """
         根据响应数据返回json格式的响应
         Args:
             http_code: http协议响应码
             headers: 响应头
             server_code: 应用协议响应码
             message: 响应消息
 
         Returns:
-            返回响应
+            返回一个sanic的HTTPResponse
         """
 
         return Response(
             data=self.resp,
             http_code=http_code,
             headers=headers,
             server_code=server_code,
             message=message,
+            response_type=self.response_type,
         ).json_resp()
```

### Comparing `sanic-api-0.2.4/sanic_api/api/exception.py` & `sanic-api-0.2.5/sanic_api/api/exception.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,34 +1,38 @@
 from typing import Any, Optional
 
 from sanic.exceptions import SanicException
 
 from sanic_api.enum import EnumBase, RespCodeEnum
+from sanic_api.utils import get_current_request
 
 
 class ServerException(SanicException):
     def __init__(
         self,
         message: Optional[str] = None,
-        server_code: Optional[EnumBase] = None,
         status_code: Optional[int] = None,
+        server_code: Optional[EnumBase] = None,
         quiet: Optional[bool] = None,
         context: Any = None,
         extra=None,
-    ) -> None:
+    ):
         super().__init__(
             message=message,
             status_code=status_code,
             quiet=quiet,
             context=context,
             extra=extra,
         )
         self.server_code = server_code or RespCodeEnum.FAILED
         self.message = message or self.server_code.desc
         self.status_code = status_code or 200
+        req = get_current_request()
+        if req:
+            req.ctx.exception = self
 
 
 class ValidationInitError(ServerException):
     """
     验证器初始化失败
     """
```

### Comparing `sanic-api-0.2.4/sanic_api/api/extend.py` & `sanic-api-0.2.5/sanic_api/api/extend.py`

 * *Files identical despite different names*

### Comparing `sanic-api-0.2.4/sanic_api/api/handle_exception.py` & `sanic-api-0.2.5/sanic_api/api/handle_exception.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 from sanic import Request
 from sanic.log import logger
 
 from sanic_api.api.api import Response
+from sanic_api.api.exception import ServerException
 from sanic_api.enum import RespCodeEnum
 
 
-def server_exception(request: Request, e):
+def server_exception(request: Request, e: ServerException):
     """
     处理业务异常
     Args:
         request: 请求
         e: 异常信息
 
     Returns:
```

### Comparing `sanic-api-0.2.4/sanic_api/api/validators.py` & `sanic-api-0.2.5/sanic_api/api/validators.py`

 * *Files 10% similar despite different names*

```diff
@@ -3,21 +3,20 @@
 from sanic import Request
 
 from sanic_api.api import API
 from sanic_api.api.exception import ValidationInitError
 from sanic_api.enum import ParamEnum
 
 
-def _do_validation(param_enum: ParamEnum, api: API, request: Request):
+def _do_validation(param_enum: ParamEnum, api: API, data: dict):
     if param_enum == ParamEnum.JSON:
-        req_data = dict(request.json)
+        req_data = data
     elif param_enum in [ParamEnum.QUERY, param_enum.FORM]:
         req_data = {}
-        attr = "args" if param_enum == ParamEnum.QUERY else "form"
-        for k, v in getattr(request, attr).items():
+        for k, v in data.items():
             if type(v) == list and len(v) == 1:
                 req_data[k] = v[0]
             else:
                 req_data[k] = v
     else:
         raise ValidationInitError("未知的验证器类型")
 
@@ -44,30 +43,34 @@
     校验请求参数中间件
     Args:
         request: 请求
 
     Returns:
 
     """
+    # 如果执行中间价直接就发生了异常则直接抛出
+    if hasattr(request.ctx, "exception"):
+        raise request.ctx.exception
+
     _, handler, _ = request.app.router.get(
         request.path,
         request.method,
         request.headers.getone("host", None),
     )
 
     api_cls = get_handler_param(handler)
     if not api_cls:
         return
 
     api: API = api_cls()
     if api.json_req_type and api.query_req_type:
         raise ValidationInitError("不能同时存在json参数和form参数")
 
-    if api.json_req_type:
-        _do_validation(param_enum=ParamEnum.JSON, api=api, request=request)
-    elif api.form_req_type:
-        _do_validation(param_enum=ParamEnum.FORM, api=api, request=request)
-    if api.query_req_type:
-        _do_validation(param_enum=ParamEnum.QUERY, api=api, request=request)
+    if api.json_req_type and request.json:
+        _do_validation(param_enum=ParamEnum.JSON, api=api, data=request.json)
+    elif api.form_req_type and request.form:
+        _do_validation(param_enum=ParamEnum.FORM, api=api, data=request.form)
+    if api.query_req_type and request.query_args:
+        _do_validation(param_enum=ParamEnum.QUERY, api=api, data=request.args)
 
     request.match_info.update({"api": api})
     request.ctx.api = api
```

### Comparing `sanic-api-0.2.4/sanic_api/config/base.py` & `sanic-api-0.2.5/sanic_api/config/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -42,15 +42,15 @@
         parser = ConfigParser()
         parser.read(self.path, encoding)
         return getattr(parser, "_sections", {}).get("settings", {})
 
 
 class YamlSettingsSource(CustomSettingsSource):
     """
-    ini文件来源导入配置项
+    Yaml文件来源导入配置项
     """
 
     def __call__(self, settings: BaseSettings) -> Dict[str, Any]:
         encoding = settings.__config__.env_file_encoding
         return yaml.safe_load(self.path.read_text(encoding))
```

### Comparing `sanic-api-0.2.4/sanic_api/enum.py` & `sanic-api-0.2.5/sanic_api/enum.py`

 * *Files 22% similar despite different names*

```diff
@@ -72,7 +72,17 @@
     """
     参数位置
     """
 
     JSON = EnumField("json")
     FORM = EnumField("form")
     QUERY = EnumField("query")
+
+
+class RunModeEnum(EnumBase):
+    """
+    运行模式
+    """
+
+    DEV = EnumField("dev", desc="开发模式。相当于debug模式加自动重载")
+    DEBUG = EnumField("debug", desc="调试模式。单workers启动。输出将更加详细，并将禁用多个运行时优化")
+    PRODUCTION = EnumField("production", desc="生产模式。如未指定workers数量，则自动使用fast模式启动。")
```

### Comparing `sanic-api-0.2.4/sanic_api/logger/config.py` & `sanic-api-0.2.5/sanic_api/logger/config.py`

 * *Files 2% similar despite different names*

```diff
@@ -34,17 +34,15 @@
         formatter = logging.Formatter(fmt=fmt)
         msg = formatter.format(record)
         msg = self.highlight_sql(record, msg)
         req_id = self.get_req_id()
 
         if "Dispatching signal" not in msg:
             etxra_data = {"type": record.name, "req_id": req_id}
-            logger.bind(**etxra_data).opt(depth=depth, exception=record.exc_info).log(
-                level, msg
-            )
+            logger.bind(**etxra_data).opt(depth=depth, exception=record.exc_info).log(level, msg)
 
     @staticmethod
     def get_req_id():
         """
         获取请求ID
         """
         try:
```

### Comparing `sanic-api-0.2.4/sanic_api/logger/extend.py` & `sanic-api-0.2.5/sanic_api/logger/extend.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 import time
 
 from loguru import logger
 
 # noinspection PyProtectedMember
 from loguru._defaults import env
 from sanic import HTTPResponse, Request
+from sanic.application.constants import Mode
 from sanic.server import HttpProtocol
 from sanic_ext import Extension
 
 from sanic_api.logger.config import InterceptHandler
 from sanic_api.logger.sanic_http import SanicHttp
 
 
@@ -22,16 +23,15 @@
 
     name = "LoggerExtend"
 
     def startup(self, bootstrap) -> None:
         if not self.included():
             return
 
-        is_debug = self.app.config.get("debug")
-        log_level = logging.DEBUG if is_debug else logging.INFO
+        log_level = logging.DEBUG if self.app.state.mode is Mode.DEBUG else logging.INFO
         log_format = env(
             "LOGURU_FORMAT",
             str,
             "<green>{time:YYYY-MM-DD HH:mm:ss.SSS}</green> | "
             "<red>{extra[type]: <10}</red> | "
             "<level>{level: <8}</level> | "
             "<cyan>{name}</cyan>:<cyan>{function}</cyan>:<cyan>{line}</cyan> - {extra[req_id]}<level>{message}</level>",
```

### Comparing `sanic-api-0.2.4/sanic_api/logger/sanic_http.py` & `sanic-api-0.2.5/sanic_api/logger/sanic_http.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,32 +1,33 @@
+from sanic import Request
 from sanic.http import Http
 from sanic.log import access_logger
 
+from sanic_api.utils import json_dumps
+
 
 class SanicHttp(Http):
     def log_response(self) -> None:
         """
         自定义输出访问日志
         Returns:
 
         """
         req, res = self.request, self.response
 
         dt = (req.ctx.et - req.ctx.st) * 1000
         size = getattr(self, "response_bytes_left", getattr(self, "response_size", -1))
-        req_args = (
-            f" args: {req.ctx.api.req_to_json()}" if hasattr(req.ctx, "api") else ""
-        )
+        req_args = self.get_req_args(req)
         extra = {
             "status": getattr(res, "status", 0),
             "byte": self.format_size(size),
             "host": "UNKNOWN",
             "request": "nil",
             "time": f"{dt:.4f} ms",
-            "req_args": req_args,
+            "req_args": f" args: {req_args}" if req_args else "",
         }
         if req is not None:
             if req.remote_addr or req.ip:
                 extra["host"] = f"{req.remote_addr or req.ip}:{req.port}"
             extra["request"] = f"{req.method} {req.url}"
         access_logger.info("", extra=extra)
 
@@ -37,7 +38,31 @@
         :return: 返回格式化的字符串
         """
         for count in ["Bytes", "KB", "MB", "GB", "TB", "PB", "EB", "ZB"]:
             if -1024.0 < size < 1024.0:
                 return f"{size:3.1f} {count}"
             size /= 1024.0
         return f"{size:3.1f} YB"
+
+    def get_req_args(self, request: Request) -> str:
+        """
+        获取请求参数
+        Args:
+            request: 请求
+
+        Returns:
+            返回具有 json、query、form参数的json
+        """
+        data = {}
+        for attr in ["args", "form"]:
+            attr_data = {}
+            for k, v in getattr(request, attr).items():
+                if type(v) == list and len(v) == 1:
+                    attr_data[k] = v[0]
+                else:
+                    attr_data[k] = v
+            if attr_data:
+                data[attr] = attr_data
+        if request.json:
+            data["json"] = request.json
+
+        return json_dumps(data) if data else ""
```

### Comparing `sanic-api-0.2.4/sanic_api/model.py` & `sanic-api-0.2.5/sanic_api/api/model.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,21 +1,33 @@
 from typing import Optional, Union
 
-from pydantic.fields import ModelPrivateAttr
+from pydantic.fields import ModelField, ModelPrivateAttr
 from pydantic.main import BaseModel
 
 
-class ListModel(BaseModel):
+class ResponseModel(BaseModel):
     """
-    列表格式的响应模型
+    响应基础模型
     """
 
-    _data_list: Optional[Union[ModelPrivateAttr, list]] = ModelPrivateAttr(
-        default_factory=list
-    )
+    def __new__(cls, *args, **kwargs):
+        for _field, value in cls.__fields__.items():
+            if not isinstance(value, ModelField):
+                continue
+            value.required = False
+
+        return super().__new__(cls, *args, **kwargs)
+
+
+class ListRespModel(ResponseModel):
+    """
+    列表格式的响应基础模型
+    """
+
+    _data_list: Optional[Union[ModelPrivateAttr, list]] = ModelPrivateAttr(default_factory=list)
 
     def add_data(self):
         """
         当前模型下数据添加到列表中
         Returns:
 
         """
```

### Comparing `sanic-api-0.2.4/PKG-INFO` & `sanic-api-0.2.5/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sanic-api
-Version: 0.2.4
+Version: 0.2.5
 Summary: Sanic 框架实用API工具集，拥有自动生成文档、参数校验、配置的导入、日志功能的优化等功能，更好的助力接口的开发
 License: MIT
 Author-email: 昊色居士 <xhrtxh@gmail.com>
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 
 ![logo](https://images.haose.pro/2022/12/19/logo_17%3A34%3A07_qkt9yi4d7u.png)
@@ -26,25 +26,25 @@
 
 - 使用`loguru`库代替官方`logging`日志库，并对访问日志进行扩展，支持打印接口耗时、接口参数
 
 - 使用`{code: 0, data: null, msg: ""}`样式的接口返回
 
 - 对接口中的异常进行拦截，及自定义错误码
 
+- 接口返回样式可自定义配置
+
 ## 截图
 
 ## 路线图
 
-- 接口返回样式可自定义配置
-
-- API接口文档生成时可以定义接口详细描述
+- 增加一键生成预设项目cli命令
 
 - 编写详细文档
 
-- API接口增加请求头、URL路径参数收集和校验
+- API接口增加请求头、URL路径参数收集和校验:
 
 ## 安装
 
 使用 pip 安装 sanic-api
 
 ```bash
   pip install sanic-api
```

