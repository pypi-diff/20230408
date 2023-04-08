# Comparing `tmp/django_pghistory-2.6.0.tar.gz` & `tmp/django_pghistory-2.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_pghistory-2.6.0.tar", max compression
+gzip compressed data, was "django_pghistory-2.7.0.tar", max compression
```

## Comparing `django_pghistory-2.6.0.tar` & `django_pghistory-2.7.0.tar`

### file list

```diff
@@ -1,31 +1,31 @@
--rw-r--r--   0        0        0     1456 2023-03-27 02:49:00.772903 django_pghistory-2.6.0/LICENSE
--rw-r--r--   0        0        0     3903 2023-03-27 02:49:00.772903 django_pghistory-2.6.0/README.rst
--rw-r--r--   0        0        0     1191 2023-03-27 02:49:00.804903 django_pghistory-2.6.0/pghistory/__init__.py
--rw-r--r--   0        0        0      257 2023-03-27 02:49:00.804903 django_pghistory-2.6.0/pghistory/admin/__init__.py
--rw-r--r--   0        0        0      297 2023-03-27 02:49:00.804903 django_pghistory-2.6.0/pghistory/admin/apps.py
--rw-r--r--   0        0        0     6660 2023-03-27 02:49:00.804903 django_pghistory-2.6.0/pghistory/admin/core.py
--rw-r--r--   0        0        0      952 2023-03-27 02:49:00.804903 django_pghistory-2.6.0/pghistory/admin/templates/admin/change_form_object_tools.html
--rw-r--r--   0        0        0      548 2023-03-27 02:49:00.804903 django_pghistory-2.6.0/pghistory/admin/templates/admin/change_list_object_tools.html
--rw-r--r--   0        0        0      219 2023-03-27 02:49:00.804903 django_pghistory-2.6.0/pghistory/admin/templates/pghistory_admin/events_change_list.html
--rw-r--r--   0        0        0        0 2023-03-27 02:49:00.804903 django_pghistory-2.6.0/pghistory/admin/templates/pghistory_admin/hidden_filter.html
--rw-r--r--   0        0        0     1486 2023-03-27 02:49:00.804903 django_pghistory-2.6.0/pghistory/admin/templatetags/pghistory_admin.py
--rw-r--r--   0        0        0      756 2023-03-27 02:49:00.804903 django_pghistory-2.6.0/pghistory/apps.py
--rw-r--r--   0        0        0      448 2023-03-27 02:49:00.804903 django_pghistory-2.6.0/pghistory/checks.py
--rw-r--r--   0        0        0    10078 2023-03-27 02:49:00.804903 django_pghistory-2.6.0/pghistory/config.py
--rw-r--r--   0        0        0       99 2023-03-27 02:49:00.804903 django_pghistory-2.6.0/pghistory/constants.py
--rw-r--r--   0        0        0    28661 2023-03-27 02:49:00.804903 django_pghistory-2.6.0/pghistory/core.py
--rw-r--r--   0        0        0    10499 2023-03-27 02:49:00.804903 django_pghistory-2.6.0/pghistory/deprecated.py
--rw-r--r--   0        0        0     1419 2023-03-27 02:49:00.804903 django_pghistory-2.6.0/pghistory/middleware.py
--rw-r--r--   0        0        0      946 2023-03-27 02:49:00.804903 django_pghistory-2.6.0/pghistory/migrations/0001_initial.py
--rw-r--r--   0        0        0     1431 2023-03-27 02:49:00.804903 django_pghistory-2.6.0/pghistory/migrations/0002_aggregateevent.py
--rw-r--r--   0        0        0      422 2023-03-27 02:49:00.804903 django_pghistory-2.6.0/pghistory/migrations/0003_auto_20201023_1636.py
--rw-r--r--   0        0        0      532 2023-03-27 02:49:00.804903 django_pghistory-2.6.0/pghistory/migrations/0004_auto_20220906_1625.py
--rw-r--r--   0        0        0     2925 2023-03-27 02:49:00.804903 django_pghistory-2.6.0/pghistory/migrations/0005_events_middlewareevents.py
--rw-r--r--   0        0        0        0 2023-03-27 02:49:00.804903 django_pghistory-2.6.0/pghistory/migrations/__init__.py
--rw-r--r--   0        0        0    26121 2023-03-27 02:49:00.804903 django_pghistory-2.6.0/pghistory/models.py
--rw-r--r--   0        0        0     4303 2023-03-27 02:49:00.804903 django_pghistory-2.6.0/pghistory/runtime.py
--rw-r--r--   0        0        0     3172 2023-03-27 02:49:00.804903 django_pghistory-2.6.0/pghistory/trigger.py
--rw-r--r--   0        0        0      576 2023-03-27 02:49:00.804903 django_pghistory-2.6.0/pghistory/utils.py
--rw-r--r--   0        0        0      154 2023-03-27 02:49:00.804903 django_pghistory-2.6.0/pghistory/version.py
--rw-r--r--   0        0        0     2421 2023-03-27 02:49:41.292709 django_pghistory-2.6.0/pyproject.toml
--rw-r--r--   0        0        0     5405 1970-01-01 00:00:00.000000 django_pghistory-2.6.0/PKG-INFO
+-rw-r--r--   0        0        0     1456 2023-04-08 16:51:34.285790 django_pghistory-2.7.0/LICENSE
+-rw-r--r--   0        0        0     3903 2023-04-08 16:51:34.285790 django_pghistory-2.7.0/README.rst
+-rw-r--r--   0        0        0     1273 2023-04-08 16:51:34.317790 django_pghistory-2.7.0/pghistory/__init__.py
+-rw-r--r--   0        0        0      257 2023-04-08 16:51:34.317790 django_pghistory-2.7.0/pghistory/admin/__init__.py
+-rw-r--r--   0        0        0      297 2023-04-08 16:51:34.317790 django_pghistory-2.7.0/pghistory/admin/apps.py
+-rw-r--r--   0        0        0     6660 2023-04-08 16:51:34.317790 django_pghistory-2.7.0/pghistory/admin/core.py
+-rw-r--r--   0        0        0      952 2023-04-08 16:51:34.317790 django_pghistory-2.7.0/pghistory/admin/templates/admin/change_form_object_tools.html
+-rw-r--r--   0        0        0      548 2023-04-08 16:51:34.317790 django_pghistory-2.7.0/pghistory/admin/templates/admin/change_list_object_tools.html
+-rw-r--r--   0        0        0      219 2023-04-08 16:51:34.317790 django_pghistory-2.7.0/pghistory/admin/templates/pghistory_admin/events_change_list.html
+-rw-r--r--   0        0        0        0 2023-04-08 16:51:34.317790 django_pghistory-2.7.0/pghistory/admin/templates/pghistory_admin/hidden_filter.html
+-rw-r--r--   0        0        0     1486 2023-04-08 16:51:34.317790 django_pghistory-2.7.0/pghistory/admin/templatetags/pghistory_admin.py
+-rw-r--r--   0        0        0      756 2023-04-08 16:51:34.317790 django_pghistory-2.7.0/pghistory/apps.py
+-rw-r--r--   0        0        0      448 2023-04-08 16:51:34.317790 django_pghistory-2.7.0/pghistory/checks.py
+-rw-r--r--   0        0        0    10078 2023-04-08 16:51:34.317790 django_pghistory-2.7.0/pghistory/config.py
+-rw-r--r--   0        0        0       99 2023-04-08 16:51:34.317790 django_pghistory-2.7.0/pghistory/constants.py
+-rw-r--r--   0        0        0    30618 2023-04-08 16:51:34.317790 django_pghistory-2.7.0/pghistory/core.py
+-rw-r--r--   0        0        0    10499 2023-04-08 16:51:34.321790 django_pghistory-2.7.0/pghistory/deprecated.py
+-rw-r--r--   0        0        0     1419 2023-04-08 16:51:34.321790 django_pghistory-2.7.0/pghistory/middleware.py
+-rw-r--r--   0        0        0      946 2023-04-08 16:51:34.321790 django_pghistory-2.7.0/pghistory/migrations/0001_initial.py
+-rw-r--r--   0        0        0     1431 2023-04-08 16:51:34.321790 django_pghistory-2.7.0/pghistory/migrations/0002_aggregateevent.py
+-rw-r--r--   0        0        0      422 2023-04-08 16:51:34.321790 django_pghistory-2.7.0/pghistory/migrations/0003_auto_20201023_1636.py
+-rw-r--r--   0        0        0      532 2023-04-08 16:51:34.321790 django_pghistory-2.7.0/pghistory/migrations/0004_auto_20220906_1625.py
+-rw-r--r--   0        0        0     2925 2023-04-08 16:51:34.321790 django_pghistory-2.7.0/pghistory/migrations/0005_events_middlewareevents.py
+-rw-r--r--   0        0        0        0 2023-04-08 16:51:34.321790 django_pghistory-2.7.0/pghistory/migrations/__init__.py
+-rw-r--r--   0        0        0    26121 2023-04-08 16:51:34.321790 django_pghistory-2.7.0/pghistory/models.py
+-rw-r--r--   0        0        0     4298 2023-04-08 16:51:34.321790 django_pghistory-2.7.0/pghistory/runtime.py
+-rw-r--r--   0        0        0     3172 2023-04-08 16:51:34.321790 django_pghistory-2.7.0/pghistory/trigger.py
+-rw-r--r--   0        0        0      576 2023-04-08 16:51:34.321790 django_pghistory-2.7.0/pghistory/utils.py
+-rw-r--r--   0        0        0      154 2023-04-08 16:51:34.321790 django_pghistory-2.7.0/pghistory/version.py
+-rw-r--r--   0        0        0     2421 2023-04-08 16:52:19.125932 django_pghistory-2.7.0/pyproject.toml
+-rw-r--r--   0        0        0     5405 1970-01-01 00:00:00.000000 django_pghistory-2.7.0/PKG-INFO
```

### Comparing `django_pghistory-2.6.0/LICENSE` & `django_pghistory-2.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `django_pghistory-2.6.0/README.rst` & `django_pghistory-2.7.0/README.rst`

 * *Files identical despite different names*

### Comparing `django_pghistory-2.6.0/pghistory/__init__.py` & `django_pghistory-2.7.0/pghistory/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -12,14 +12,16 @@
 from pghistory.constants import DEFAULT
 from pghistory.core import (
     AfterInsert,
     AfterInsertOrUpdate,
     AfterUpdate,
     BeforeDelete,
     BeforeUpdate,
+    BeforeUpdateOrDelete,
+    Changed,
     create_event,
     create_event_model,
     DatabaseEvent,
     DatabaseTracker,
     Event,
     ManualTracker,
     ProxyField,
@@ -33,14 +35,16 @@
 
 __all__ = [
     "AfterInsert",
     "AfterInsertOrUpdate",
     "AfterUpdate",
     "BeforeDelete",
     "BeforeUpdate",
+    "BeforeUpdateOrDelete",
+    "Changed",
     "context",
     "ContextForeignKey",
     "ContextJSONField",
     "ContextUUIDField",
     "create_event",
     "create_event_model",
     "DatabaseEvent",
```

### Comparing `django_pghistory-2.6.0/pghistory/admin/core.py` & `django_pghistory-2.7.0/pghistory/admin/core.py`

 * *Files identical despite different names*

### Comparing `django_pghistory-2.6.0/pghistory/admin/templates/admin/change_form_object_tools.html` & `django_pghistory-2.7.0/pghistory/admin/templates/admin/change_form_object_tools.html`

 * *Files identical despite different names*

### Comparing `django_pghistory-2.6.0/pghistory/admin/templates/admin/change_list_object_tools.html` & `django_pghistory-2.7.0/pghistory/admin/templates/admin/change_list_object_tools.html`

 * *Files identical despite different names*

### Comparing `django_pghistory-2.6.0/pghistory/admin/templatetags/pghistory_admin.py` & `django_pghistory-2.7.0/pghistory/admin/templatetags/pghistory_admin.py`

 * *Files identical despite different names*

### Comparing `django_pghistory-2.6.0/pghistory/apps.py` & `django_pghistory-2.7.0/pghistory/apps.py`

 * *Files identical despite different names*

### Comparing `django_pghistory-2.6.0/pghistory/config.py` & `django_pghistory-2.7.0/pghistory/config.py`

 * *Files identical despite different names*

### Comparing `django_pghistory-2.6.0/pghistory/core.py` & `django_pghistory-2.7.0/pghistory/core.py`

 * *Files 4% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 
 from pghistory import config, constants, trigger, utils
 
 
 _registered_trackers = {}
 
 
-def _get_name_from_label(label):
+def _fmt_trigger_name(label):
     """Given a history event label, generate a trigger name"""
     if label:
         return re.sub("[^0-9a-zA-Z]+", "_", label)
     else:  # pragma: no cover
         return None
 
 
@@ -91,27 +91,39 @@
         super().__init__(label=label)
 
         self.when = when or self.when
         self.condition = condition or self.condition
         self.operation = operation or self.operation
         self.snapshot = snapshot or self.snapshot
 
-    def setup(self, event_model):
+    def add_event_trigger(
+        self, *, event_model, label, snapshot, when, operation, condition=None, name=None
+    ):
         pgtrigger.register(
             trigger.Event(
                 event_model=event_model,
-                label=self.label,
-                name=_get_name_from_label(self.label),
-                snapshot=self.snapshot,
-                when=self.when,
-                operation=self.operation,
-                condition=self.condition,
+                label=label,
+                name=_fmt_trigger_name(name or label),
+                snapshot=snapshot,
+                when=when,
+                operation=operation,
+                condition=condition,
             )
         )(event_model.pgh_tracked_model)
 
+    def setup(self, event_model):
+        self.add_event_trigger(
+            event_model=event_model,
+            label=self.label,
+            snapshot=self.snapshot,
+            when=self.when,
+            operation=self.operation,
+            condition=self.condition,
+        )
+
 
 class DatabaseEvent(DatabaseTracker):
     """
     The deprecated base class for all trigger-based trackers.
     Use `DatabaseTracker` instead.
     """
 
@@ -134,64 +146,99 @@
             when=when,
             condition=condition,
             operation=operation,
             snapshot=snapshot,
         )
 
 
+class Changed(pgtrigger.Condition):
+    """A utilty to create conditions based on changes in the tracked model.
+
+    Given the event model, we create a condition as follows:
+
+    - If the event model trackes every field from the main model, we can
+      use a standard ``OLD.* IS DISTINCT FROM NEW.*`` condition to snapshot
+      every change on the main model.
+    - If the event model tracks a subset of the fields of the main model,
+      only changes to event fields will trigger a snapshot. In other words,
+      if the main model has an int and char field, but the event model only
+      tracks the char field, the condition will be
+      ``OLD.char_field IS DISTINCT FROM NEW.char_field``.
+    - If one has fields on the event model and wishes to ignore them from
+      triggering snapshots, pass them to the ``exclude`` argument to this
+      utility.
+    """
+
+    def __init__(self, event_model, exclude=None):
+        self.event_model = event_model
+        self.exclude = exclude or []
+
+    def resolve(self, model):
+        event_fields = [
+            field.name
+            for field in self.event_model._meta.fields
+            if not field.name.startswith("pgh_")
+        ]
+        model_fields = [f.name for f in model._meta.fields]
+
+        # By default, any field in both the main model and event model that
+        # change will trigger the condition. You can exclude fields from
+        # the event model that will trigger snapshots.
+        conditional_fields = [f for f in event_fields if f not in self.exclude]
+
+        if set(event_fields) == set(model_fields) == set(conditional_fields):
+            # We're tracking every field on any change
+            condition = pgtrigger.Condition("OLD.* IS DISTINCT FROM NEW.*")
+        else:
+            # We're either tracking a subset of fields or we have
+            condition = pgtrigger.Q()
+
+            for field in conditional_fields:
+                if hasattr(model, field):
+                    condition |= pgtrigger.Q(**{f"old__{field}__df": pgtrigger.F(f"new__{field}")})
+
+        return condition.resolve(model)
+
+
 class Snapshot(DatabaseTracker):
     """
     Tracks changes to fields.
     A snapshot tracker tracks inserts and updates. It ensures that no
     duplicate rows are created with a pre-configured condition.
 
     NOTE: Two triggers are created since Insert triggers do
     not allow comparison against the OLD values. We could also
     place this in one trigger and do the condition in the plpgsql code.
     """
 
-    def __init__(self, label=None):
+    def __init__(self, label=None, delayed=False):
+        self.delayed = delayed
         return super().__init__(label=label)
 
     def setup(self, event_model):
 
-        insert_trigger = trigger.Event(
+        self.add_event_trigger(
             event_model=event_model,
             label=self.label,
-            name=_get_name_from_label(f"{self.label}_insert"),
+            name=f"{self.label}_insert",
             snapshot="NEW",
             when=pgtrigger.After,
             operation=pgtrigger.Insert,
         )
 
-        event_fields = [
-            field.name for field in event_model._meta.fields if not field.name.startswith("pgh_")
-        ]
-        tracked_fields = [field.name for field in event_model.pgh_tracked_model._meta.fields]
-
-        if set(event_fields) == set(tracked_fields):
-            condition = pgtrigger.Condition("OLD.* IS DISTINCT FROM NEW.*")
-        else:
-            condition = pgtrigger.Q()
-            for field in event_fields:
-                if hasattr(event_model.pgh_tracked_model, field):
-                    condition |= pgtrigger.Q(**{f"old__{field}__df": pgtrigger.F(f"new__{field}")})
-
-        update_trigger = trigger.Event(
+        self.add_event_trigger(
             event_model=event_model,
             label=self.label,
-            name=_get_name_from_label(f"{self.label}_update"),
+            name=f"{self.label}_update",
             snapshot="NEW",
             when=pgtrigger.After,
             operation=pgtrigger.Update,
-            condition=condition,
+            condition=Changed(event_model),
         )
 
-        pgtrigger.register(insert_trigger, update_trigger)(event_model.pgh_tracked_model)
-
 
 class PreconfiguredDatabaseTracker(DatabaseTracker):
     """
     A base database tracker that only takes a condition. Subclasses
     preconfigure the other parameters
     """
 
@@ -240,14 +287,23 @@
     For trackers that fire before a database deletion.
     """
 
     operation = pgtrigger.Delete
     snapshot = "OLD"
 
 
+class BeforeUpdateOrDelete(PreconfiguredDatabaseTracker):
+    """
+    A database tracker that snapshots the old row during an update or delete
+    """
+
+    operation = pgtrigger.Update | pgtrigger.Delete
+    snapshot = "OLD"
+
+
 def _pascalcase(string):
     """Convert string into pascal case."""
 
     string = re.sub(r"^[\-_\.]", "", str(string))
     if not string:  # pragma: no branch
         return string
```

### Comparing `django_pghistory-2.6.0/pghistory/deprecated.py` & `django_pghistory-2.7.0/pghistory/deprecated.py`

 * *Files identical despite different names*

### Comparing `django_pghistory-2.6.0/pghistory/middleware.py` & `django_pghistory-2.7.0/pghistory/middleware.py`

 * *Files identical despite different names*

### Comparing `django_pghistory-2.6.0/pghistory/migrations/0001_initial.py` & `django_pghistory-2.7.0/pghistory/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django_pghistory-2.6.0/pghistory/migrations/0002_aggregateevent.py` & `django_pghistory-2.7.0/pghistory/migrations/0002_aggregateevent.py`

 * *Files identical despite different names*

### Comparing `django_pghistory-2.6.0/pghistory/migrations/0004_auto_20220906_1625.py` & `django_pghistory-2.7.0/pghistory/migrations/0004_auto_20220906_1625.py`

 * *Files identical despite different names*

### Comparing `django_pghistory-2.6.0/pghistory/migrations/0005_events_middlewareevents.py` & `django_pghistory-2.7.0/pghistory/migrations/0005_events_middlewareevents.py`

 * *Files identical despite different names*

### Comparing `django_pghistory-2.6.0/pghistory/models.py` & `django_pghistory-2.7.0/pghistory/models.py`

 * *Files identical despite different names*

### Comparing `django_pghistory-2.6.0/pghistory/runtime.py` & `django_pghistory-2.7.0/pghistory/runtime.py`

 * *Files 2% similar despite different names*

```diff
@@ -67,15 +67,15 @@
     To add context only if a parent has already entered ``pghistory.context``,
     one can call ``pghistory.context`` as a function without entering it.
     The metadata set in the function call will be part of the context if
     ``pghistory.context`` has previously been entered. Otherwise it will
     be ignored.
 
     Args:
-        metadata (dict): Metadata that should be attached to the tracking
+        **metadata: Metadata that should be attached to the tracking
             context
 
     Example:
         Here we track a "key" with a value of "value"::
 
             with pghistory.context(key='value'):
                 # Do things..
```

### Comparing `django_pghistory-2.6.0/pghistory/trigger.py` & `django_pghistory-2.7.0/pghistory/trigger.py`

 * *Files identical despite different names*

### Comparing `django_pghistory-2.6.0/pghistory/utils.py` & `django_pghistory-2.7.0/pghistory/utils.py`

 * *Files identical despite different names*

### Comparing `django_pghistory-2.6.0/pyproject.toml` & `django_pghistory-2.7.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -28,15 +28,15 @@
 name = "django-pghistory"
 packages = [
   { include = "pghistory" }
 ]
 exclude = [
   "*/tests/"
 ]
-version = "2.6.0"
+version = "2.7.0"
 description = "History tracking for Django and Postgres"
 authors = ["Wes Kendall"]
 classifiers = [
   "Framework :: Django",
   "Framework :: Django :: 2.2",
   "Framework :: Django :: 3.2",
   "Framework :: Django :: 4.0",
```

### Comparing `django_pghistory-2.6.0/PKG-INFO` & `django_pghistory-2.7.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-pghistory
-Version: 2.6.0
+Version: 2.7.0
 Summary: History tracking for Django and Postgres
 Home-page: https://github.com/Opus10/django-pghistory
 License: BSD-3-Clause
 Author: Wes Kendall
 Requires-Python: >=3.7.0,<4
 Classifier: Framework :: Django
 Classifier: Framework :: Django :: 2.2
```

