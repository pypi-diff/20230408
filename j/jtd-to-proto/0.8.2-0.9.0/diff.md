# Comparing `tmp/jtd_to_proto-0.8.2-py39-none-any.whl.zip` & `tmp/jtd_to_proto-0.9.0-py39-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,12 +1,12 @@
-Zip file size: 16857 bytes, number of entries: 10
--rw-r--r--  2.0 unx     1127 b- defN 23-Feb-28 23:51 jtd_to_proto/__init__.py
--rw-r--r--  2.0 unx     7714 b- defN 23-Feb-28 23:51 jtd_to_proto/descriptor_to_file.py
--rw-r--r--  2.0 unx     3380 b- defN 23-Feb-28 23:51 jtd_to_proto/descriptor_to_message_class.py
--rw-r--r--  2.0 unx     9006 b- defN 23-Feb-28 23:51 jtd_to_proto/json_to_service.py
--rw-r--r--  2.0 unx    26271 b- defN 23-Feb-28 23:51 jtd_to_proto/jtd_to_proto.py
--rw-r--r--  2.0 unx     1088 b- defN 23-Feb-28 23:52 jtd_to_proto-0.8.2.dist-info/LICENSE
--rw-r--r--  2.0 unx     4584 b- defN 23-Feb-28 23:52 jtd_to_proto-0.8.2.dist-info/METADATA
--rw-r--r--  2.0 unx       93 b- defN 23-Feb-28 23:52 jtd_to_proto-0.8.2.dist-info/WHEEL
--rw-r--r--  2.0 unx       13 b- defN 23-Feb-28 23:52 jtd_to_proto-0.8.2.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      857 b- defN 23-Feb-28 23:52 jtd_to_proto-0.8.2.dist-info/RECORD
-10 files, 54133 bytes uncompressed, 15387 bytes compressed:  71.6%
+Zip file size: 17215 bytes, number of entries: 10
+-rw-r--r--  2.0 unx     1127 b- defN 23-Mar-14 18:11 jtd_to_proto/__init__.py
+-rw-r--r--  2.0 unx     8809 b- defN 23-Mar-14 18:11 jtd_to_proto/descriptor_to_file.py
+-rw-r--r--  2.0 unx     4416 b- defN 23-Mar-14 18:11 jtd_to_proto/descriptor_to_message_class.py
+-rw-r--r--  2.0 unx     9201 b- defN 23-Mar-14 18:11 jtd_to_proto/json_to_service.py
+-rw-r--r--  2.0 unx    26165 b- defN 23-Mar-14 18:11 jtd_to_proto/jtd_to_proto.py
+-rw-r--r--  2.0 unx     1088 b- defN 23-Mar-14 18:12 jtd_to_proto-0.9.0.dist-info/LICENSE
+-rw-r--r--  2.0 unx     4584 b- defN 23-Mar-14 18:12 jtd_to_proto-0.9.0.dist-info/METADATA
+-rw-r--r--  2.0 unx       93 b- defN 23-Mar-14 18:12 jtd_to_proto-0.9.0.dist-info/WHEEL
+-rw-r--r--  2.0 unx       13 b- defN 23-Mar-14 18:12 jtd_to_proto-0.9.0.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      857 b- defN 23-Mar-14 18:12 jtd_to_proto-0.9.0.dist-info/RECORD
+10 files, 56353 bytes uncompressed, 15745 bytes compressed:  72.1%
```

## zipnote {}

```diff
@@ -9,23 +9,23 @@
 
 Filename: jtd_to_proto/json_to_service.py
 Comment: 
 
 Filename: jtd_to_proto/jtd_to_proto.py
 Comment: 
 
-Filename: jtd_to_proto-0.8.2.dist-info/LICENSE
+Filename: jtd_to_proto-0.9.0.dist-info/LICENSE
 Comment: 
 
-Filename: jtd_to_proto-0.8.2.dist-info/METADATA
+Filename: jtd_to_proto-0.9.0.dist-info/METADATA
 Comment: 
 
-Filename: jtd_to_proto-0.8.2.dist-info/WHEEL
+Filename: jtd_to_proto-0.9.0.dist-info/WHEEL
 Comment: 
 
-Filename: jtd_to_proto-0.8.2.dist-info/top_level.txt
+Filename: jtd_to_proto-0.9.0.dist-info/top_level.txt
 Comment: 
 
-Filename: jtd_to_proto-0.8.2.dist-info/RECORD
+Filename: jtd_to_proto-0.9.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## jtd_to_proto/descriptor_to_file.py

```diff
@@ -30,39 +30,54 @@
 /*-- ENUMS -------------------------------------------------------------------*/
 """
 
 PROTO_FILE_MESSAGE_HEADER = """
 /*-- MESSAGES ----------------------------------------------------------------*/
 """
 
+PROTO_FILE_SERVICES_HEADER = """
+/*-- SERVICES ----------------------------------------------------------------*/
+"""
+
 PROTO_FILE_NESTED_ENUM_HEADER = f"{PROTO_FILE_INDENT}/*-- nested enums --*/"
 PROTO_FILE_NESTED_MESSAGE_HEADER = f"{PROTO_FILE_INDENT}/*-- nested messages --*/"
 PROTO_FILE_FIELD_HEADER = f"{PROTO_FILE_INDENT}/*-- fields --*/"
 PROTO_FILE_ONEOF_HEADER = f"{PROTO_FILE_INDENT}/*-- oneofs --*/"
 
 
 ## Interface ###################################################################
 
 
 def descriptor_to_file(
-    descriptor: Union[_descriptor.FileDescriptor, _descriptor.Descriptor],
+    descriptor: Union[
+        _descriptor.FileDescriptor,
+        _descriptor.Descriptor,
+        _descriptor.ServiceDescriptor,
+    ],
 ) -> str:
     """Serialize a .proto file from a FileDescriptor
 
     Args:
         descriptor:  Union[descriptor.FileDescriptor, descriptor.MessageDescriptor]
             The file or message descriptor to serialize
 
     Returns:
         proto_file_content:  str
             The serialized file content for the .proto file
     """
 
     # If this is a message descriptor, use its corresponding FileDescriptor
-    if isinstance(descriptor, (_descriptor.Descriptor, _descriptor.EnumDescriptor)):
+    if isinstance(
+        descriptor,
+        (
+            _descriptor.Descriptor,
+            _descriptor.EnumDescriptor,
+            _descriptor.ServiceDescriptor,
+        ),
+    ):
         descriptor = descriptor.file
     if not isinstance(descriptor, _descriptor.FileDescriptor):
         raise ValueError(f"Invalid file descriptor of type {type(descriptor)}")
     proto_file_lines = []
 
     # Create the header
     proto_file_lines.append(PROTO_FILE_AUTOGEN_HEADER)
@@ -85,14 +100,20 @@
     # Add all messages
     if descriptor.message_types_by_name:
         proto_file_lines.append(PROTO_FILE_MESSAGE_HEADER)
         for message_descriptor in descriptor.message_types_by_name.values():
             proto_file_lines.extend(_message_descriptor_to_file(message_descriptor))
             proto_file_lines.append("")
 
+    if descriptor.services_by_name:
+        proto_file_lines.append(PROTO_FILE_SERVICES_HEADER)
+        for service_descriptor in descriptor.services_by_name.values():
+            proto_file_lines.extend(_service_descriptor_to_file(service_descriptor))
+            proto_file_lines.append("")
+
     return "\n".join(proto_file_lines)
 
 
 ## Impl ########################################################################
 
 
 def _indent_lines(indent: int, lines: List[str]) -> List[str]:
@@ -159,14 +180,29 @@
     for oneof_descriptor in message_descriptor.oneofs:
         lines.extend(_oneof_descriptor_to_file(oneof_descriptor, indent=1))
 
     lines.append("}")
     return _indent_lines(indent, lines)
 
 
+def _service_descriptor_to_file(
+    service_descriptor: _descriptor.ServiceDescriptor,
+    indent: int = 0,
+) -> List[str]:
+    """Make the string representation of a service"""
+    lines = []
+    lines.append(f"service {service_descriptor.name} {{")
+    for method in service_descriptor.methods:
+        lines.append(
+            f"{PROTO_FILE_INDENT}rpc {method.name}({method.input_type.full_name}) returns ({method.output_type.full_name});"
+        )
+    lines.append("}")
+    return _indent_lines(indent, lines)
+
+
 def _field_descriptor_to_file(
     field_descriptor: _descriptor.FieldDescriptor,
     indent: int = 0,
 ) -> List[str]:
     """Get the string version of a field"""
 
     # Add the repeated qualifier if needed
```

## jtd_to_proto/descriptor_to_message_class.py

```diff
@@ -8,16 +8,18 @@
 from types import MethodType
 from typing import Any, Callable, Type, Union
 import os
 
 # Third Party
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import message as _message
-from google.protobuf import reflection
+from google.protobuf import reflection, service
+from google.protobuf.descriptor import ServiceDescriptor
 from google.protobuf.internal.enum_type_wrapper import EnumTypeWrapper
+from google.protobuf.service import Service
 
 # Local
 from .descriptor_to_file import descriptor_to_file
 
 
 def descriptor_to_message_class(
     descriptor: Union[_descriptor.Descriptor, _descriptor.EnumDescriptor],
@@ -53,35 +55,15 @@
         for nested_enum_descriptor in descriptor.enum_types:
             setattr(
                 message_class,
                 nested_enum_descriptor.name,
                 descriptor_to_message_class(nested_enum_descriptor),
             )
 
-    # Add to_proto_file
-    if not hasattr(message_class, "to_proto_file"):
-
-        def to_proto_file(first_arg) -> str:
-            f"Create the serialized .proto file content holding all definitions for {descriptor.name}"
-            return descriptor_to_file(first_arg.DESCRIPTOR)
-
-        _maybe_classmethod(to_proto_file, message_class)
-
-    # Add write_proto_file
-    if not hasattr(message_class, "write_proto_file"):
-
-        def write_proto_file(first_arg, root_dir: str = "."):
-            "Write out the proto file to the target directory"
-            with open(
-                os.path.join(root_dir, first_arg.DESCRIPTOR.file.name), "w"
-            ) as handle:
-                handle.write(first_arg.to_proto_file())
-
-        _maybe_classmethod(write_proto_file, message_class)
-
+    message_class = _add_protobuf_serializers(message_class, descriptor)
     return message_class
 
 
 ## Implementation Details ######################################################
 
 
 def _maybe_classmethod(func: Callable, parent: Any):
@@ -101,7 +83,50 @@
         @wraps(func)
         def _wrapper(self, *args, **kwargs):
             return func(self, *args, **kwargs)
 
         _wrapper = MethodType(_wrapper, parent)
 
     setattr(parent, func.__name__, _wrapper)
+
+
+def _add_protobuf_serializers(
+    type_class: Union[Type[_message.Message], EnumTypeWrapper, Type[service.Service]],
+    descriptor: Union[
+        _descriptor.Descriptor,
+        _descriptor.EnumDescriptor,
+        _descriptor.ServiceDescriptor,
+    ],
+) -> Union[Type[_message.Message], EnumTypeWrapper, Type[service.Service]]:
+    """Helper to add the to_proto_file and write_proto_file to a given type class.
+
+    Args:
+        descriptor:  Union[_descriptor.Descriptor, _descriptor.EnumDescriptor, _descriptor.ServiceDescriptor]
+            The message or enum Descriptor
+        type_class: Union[Type[_message.Message], EnumTypeWrapper, Type[service.Service]]
+
+    Returns:
+       Union[Type[_message.Message], EnumTypeWrapper, Type[service.Service]]
+            A new class with the to_proto_file and write_proto_file added
+    """
+    # Add to_proto_file
+    if not hasattr(type_class, "to_proto_file"):
+
+        def to_proto_file(first_arg) -> str:
+            f"Create the serialized .proto file content holding all definitions for {descriptor.name}"
+            return descriptor_to_file(first_arg.DESCRIPTOR)
+
+        _maybe_classmethod(to_proto_file, type_class)
+
+    # Add write_proto_file
+    if not hasattr(type_class, "write_proto_file"):
+
+        def write_proto_file(first_arg, root_dir: str = "."):
+            "Write out the proto file to the target directory"
+            with open(
+                os.path.join(root_dir, first_arg.DESCRIPTOR.file.name), "w"
+            ) as handle:
+                handle.write(first_arg.to_proto_file())
+
+        _maybe_classmethod(write_proto_file, type_class)
+
+    return type_class
```

## jtd_to_proto/json_to_service.py

```diff
@@ -15,14 +15,15 @@
 import jtd
 
 # First Party
 import alog
 
 # Local
 from jtd_to_proto import descriptor_to_message_class
+from jtd_to_proto.descriptor_to_message_class import _add_protobuf_serializers
 
 log = alog.use_channel("JSON2S")
 
 SERVICE_JTD_SCHEMA = jtd.Schema.from_dict(
     {
         "properties": {
             "service": {
@@ -145,20 +146,23 @@
             The ServiceDescriptor to generate a service interface for
 
     Returns:
         Type[google.protobuf.service.Service]
             A new class with metaclass google.protobuf.service_reflection.GeneratedServiceType containing the methods
             from the service_descriptor
     """
-    return types.new_class(
+    service_class = types.new_class(
         service_descriptor.name,
         (service.Service,),
         {"metaclass": GeneratedServiceType},
         lambda ns: ns.update({"DESCRIPTOR": service_descriptor}),
     )
+    service_class = _add_protobuf_serializers(service_class, service_descriptor)
+
+    return service_class
 
 
 def service_descriptor_to_client_stub(
     service_descriptor: _descriptor.ServiceDescriptor,
 ) -> Type:
     """Generates a new client stub class from the service descriptor
```

## jtd_to_proto/jtd_to_proto.py

```diff
@@ -193,16 +193,14 @@
     #   range, they are only 1 or 2 bytes, even though it says int32.
     #
     # CITE: https://groups.google.com/g/protobuf/c/Er39mNGnRWU/m/x6Srz_GrZPgJ
     "int8": _descriptor.FieldDescriptor.TYPE_INT32,
     "uint8": _descriptor.FieldDescriptor.TYPE_UINT32,
     "int16": _descriptor.FieldDescriptor.TYPE_INT32,
     "uint16": _descriptor.FieldDescriptor.TYPE_UINT32,
-    "int8": _descriptor.FieldDescriptor.TYPE_INT32,
-    "uint8": _descriptor.FieldDescriptor.TYPE_UINT32,
     "int32": _descriptor.FieldDescriptor.TYPE_INT32,
     "uint32": _descriptor.FieldDescriptor.TYPE_UINT32,
     "int64": _descriptor.FieldDescriptor.TYPE_INT64,
     "uint64": _descriptor.FieldDescriptor.TYPE_UINT64,
     # Not strictly part of the JTD spec, but important for protobuf messages
     "bytes": _descriptor.FieldDescriptor.TYPE_BYTES,
 }
```

## Comparing `jtd_to_proto-0.8.2.dist-info/LICENSE` & `jtd_to_proto-0.9.0.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `jtd_to_proto-0.8.2.dist-info/METADATA` & `jtd_to_proto-0.9.0.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jtd-to-proto
-Version: 0.8.2
+Version: 0.9.0
 Summary: A tool to dynamically create protobuf message classes from JSON Typedef
 Home-page: https://github.com/IBM/jtd-to-proto
 Author: Gabe Goodhart
 Author-email: gabe.l.hart@gmail.com
 License: MIT
 Keywords: json,json typedef,jtd,protobuf,proto
 Platform: UNKNOWN
```

