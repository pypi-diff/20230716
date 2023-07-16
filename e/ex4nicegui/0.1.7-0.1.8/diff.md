# Comparing `tmp/ex4nicegui-0.1.7.tar.gz` & `tmp/ex4nicegui-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ex4nicegui-0.1.7.tar", last modified: Fri Jul 14 15:34:28 2023, max compression
+gzip compressed data, was "ex4nicegui-0.1.8.tar", last modified: Sun Jul 16 10:57:03 2023, max compression
```

## Comparing `ex4nicegui-0.1.7.tar` & `ex4nicegui-0.1.8.tar`

### file list

```diff
@@ -1,46 +1,46 @@
-drwxrwxrwx   0        0        0        0 2023-07-14 15:34:28.808192 ex4nicegui-0.1.7/
--rw-rw-rw-   0        0        0     1094 2023-06-30 08:17:10.000000 ex4nicegui-0.1.7/LICENSE
--rw-rw-rw-   0        0        0      481 2023-07-14 15:34:28.805831 ex4nicegui-0.1.7/PKG-INFO
--rw-rw-rw-   0        0        0     2200 2023-07-10 15:25:21.000000 ex4nicegui-0.1.7/README.md
-drwxrwxrwx   0        0        0        0 2023-07-14 15:34:28.689114 ex4nicegui-0.1.7/ex4nicegui/
--rw-rw-rw-   0        0        0      337 2023-07-14 15:34:04.000000 ex4nicegui-0.1.7/ex4nicegui/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-14 15:34:28.705072 ex4nicegui-0.1.7/ex4nicegui/layout/
--rw-rw-rw-   0        0        0       31 2023-07-05 06:10:00.000000 ex4nicegui-0.1.7/ex4nicegui/layout/__init__.py
--rw-rw-rw-   0        0        0     2378 2023-07-05 06:10:00.000000 ex4nicegui-0.1.7/ex4nicegui/layout/gridbox.py
-drwxrwxrwx   0        0        0        0 2023-07-14 15:34:28.721301 ex4nicegui-0.1.7/ex4nicegui/reactive/
--rw-rw-rw-   0        0        0     1217 2023-07-14 15:33:47.000000 ex4nicegui-0.1.7/ex4nicegui/reactive/__index.py
--rw-rw-rw-   0        0        0       24 2023-07-05 06:10:00.000000 ex4nicegui-0.1.7/ex4nicegui/reactive/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-14 15:34:28.742602 ex4nicegui-0.1.7/ex4nicegui/reactive/draggable/
--rw-rw-rw-   0        0        0     4851 2023-07-05 09:28:02.000000 ex4nicegui-0.1.7/ex4nicegui/reactive/draggable/UseDraggable.js
--rw-rw-rw-   0        0        0     3041 2023-07-08 17:55:18.000000 ex4nicegui-0.1.7/ex4nicegui/reactive/draggable/UseDraggable.py
--rw-rw-rw-   0        0        0        0 2023-07-05 06:10:00.000000 ex4nicegui-0.1.7/ex4nicegui/reactive/draggable/__init__.py
--rw-rw-rw-   0        0        0     1365 2023-07-10 14:31:39.000000 ex4nicegui-0.1.7/ex4nicegui/reactive/drawer.py
-drwxrwxrwx   0        0        0        0 2023-07-14 15:34:28.775627 ex4nicegui-0.1.7/ex4nicegui/reactive/echarts/
--rw-rw-rw-   0        0        0  1581614 2023-07-05 06:10:00.000000 ex4nicegui-0.1.7/ex4nicegui/reactive/echarts/ECharts.js
--rw-rw-rw-   0        0        0     2685 2023-07-09 14:56:08.000000 ex4nicegui-0.1.7/ex4nicegui/reactive/echarts/ECharts.py
--rw-rw-rw-   0        0        0        0 2023-07-05 06:10:00.000000 ex4nicegui-0.1.7/ex4nicegui/reactive/echarts/__init__.py
--rw-rw-rw-   0        0        0     6106 2023-07-10 14:31:39.000000 ex4nicegui-0.1.7/ex4nicegui/reactive/local_file_picker.py
--rw-rw-rw-   0        0        0    35637 2023-07-14 15:33:47.000000 ex4nicegui-0.1.7/ex4nicegui/reactive/officials.py
--rw-rw-rw-   0        0        0     1224 2023-07-14 15:33:47.000000 ex4nicegui-0.1.7/ex4nicegui/reactive/q_pagination.py
--rw-rw-rw-   0        0        0       24 2023-07-09 14:56:08.000000 ex4nicegui-0.1.7/ex4nicegui/reactive/rxui.py
-drwxrwxrwx   0        0        0        0 2023-07-14 15:34:28.795887 ex4nicegui-0.1.7/ex4nicegui/reactive/useMouse/
--rw-rw-rw-   0        0        0     2722 2023-07-08 17:55:18.000000 ex4nicegui-0.1.7/ex4nicegui/reactive/useMouse/UseMouse.js
--rw-rw-rw-   0        0        0     2244 2023-07-08 17:55:18.000000 ex4nicegui-0.1.7/ex4nicegui/reactive/useMouse/UseMouse.py
--rw-rw-rw-   0        0        0        0 2023-07-08 17:55:18.000000 ex4nicegui-0.1.7/ex4nicegui/reactive/useMouse/__init__.py
--rw-rw-rw-   0        0        0     2093 2023-07-14 15:33:47.000000 ex4nicegui-0.1.7/ex4nicegui/reactive/usePagination.py
-drwxrwxrwx   0        0        0        0 2023-07-14 15:34:28.798846 ex4nicegui-0.1.7/ex4nicegui/tools/
--rw-rw-rw-   0        0        0       40 2023-07-08 17:55:18.000000 ex4nicegui-0.1.7/ex4nicegui/tools/__init__.py
--rw-rw-rw-   0        0        0     4887 2023-07-10 13:40:51.000000 ex4nicegui-0.1.7/ex4nicegui/tools/debug.py
-drwxrwxrwx   0        0        0        0 2023-07-14 15:34:28.803832 ex4nicegui-0.1.7/ex4nicegui/utils/
--rw-rw-rw-   0        0        0        0 2023-07-05 06:10:00.000000 ex4nicegui-0.1.7/ex4nicegui/utils/__init__.py
--rw-rw-rw-   0        0        0      430 2023-07-08 17:55:18.000000 ex4nicegui-0.1.7/ex4nicegui/utils/common.py
--rw-rw-rw-   0        0        0     4807 2023-07-10 14:31:39.000000 ex4nicegui-0.1.7/ex4nicegui/utils/signals.py
-drwxrwxrwx   0        0        0        0 2023-07-14 15:34:28.701083 ex4nicegui-0.1.7/ex4nicegui.egg-info/
--rw-rw-rw-   0        0        0      481 2023-07-14 15:34:28.000000 ex4nicegui-0.1.7/ex4nicegui.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1092 2023-07-14 15:34:28.000000 ex4nicegui-0.1.7/ex4nicegui.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-14 15:34:28.000000 ex4nicegui-0.1.7/ex4nicegui.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-07-14 15:34:28.000000 ex4nicegui-0.1.7/ex4nicegui.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       47 2023-07-14 15:34:28.000000 ex4nicegui-0.1.7/ex4nicegui.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-07-14 15:34:28.000000 ex4nicegui-0.1.7/ex4nicegui.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-14 15:34:28.808192 ex4nicegui-0.1.7/setup.cfg
--rw-rw-rw-   0        0        0     2088 2023-07-10 14:33:48.000000 ex4nicegui-0.1.7/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-16 10:57:03.790430 ex4nicegui-0.1.8/
+-rw-rw-rw-   0        0        0     1094 2023-06-30 08:17:10.000000 ex4nicegui-0.1.8/LICENSE
+-rw-rw-rw-   0        0        0      481 2023-07-16 10:57:03.789432 ex4nicegui-0.1.8/PKG-INFO
+-rw-rw-rw-   0        0        0     2200 2023-07-10 15:25:21.000000 ex4nicegui-0.1.8/README.md
+drwxrwxrwx   0        0        0        0 2023-07-16 10:57:03.680226 ex4nicegui-0.1.8/ex4nicegui/
+-rw-rw-rw-   0        0        0      337 2023-07-16 10:56:47.000000 ex4nicegui-0.1.8/ex4nicegui/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-16 10:57:03.694085 ex4nicegui-0.1.8/ex4nicegui/layout/
+-rw-rw-rw-   0        0        0       31 2023-07-05 06:10:00.000000 ex4nicegui-0.1.8/ex4nicegui/layout/__init__.py
+-rw-rw-rw-   0        0        0     2378 2023-07-05 06:10:00.000000 ex4nicegui-0.1.8/ex4nicegui/layout/gridbox.py
+drwxrwxrwx   0        0        0        0 2023-07-16 10:57:03.708144 ex4nicegui-0.1.8/ex4nicegui/reactive/
+-rw-rw-rw-   0        0        0     1300 2023-07-16 10:54:22.000000 ex4nicegui-0.1.8/ex4nicegui/reactive/__index.py
+-rw-rw-rw-   0        0        0       24 2023-07-05 06:10:00.000000 ex4nicegui-0.1.8/ex4nicegui/reactive/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-16 10:57:03.713221 ex4nicegui-0.1.8/ex4nicegui/reactive/draggable/
+-rw-rw-rw-   0        0        0     4851 2023-07-05 09:28:02.000000 ex4nicegui-0.1.8/ex4nicegui/reactive/draggable/UseDraggable.js
+-rw-rw-rw-   0        0        0     2902 2023-07-16 10:54:22.000000 ex4nicegui-0.1.8/ex4nicegui/reactive/draggable/UseDraggable.py
+-rw-rw-rw-   0        0        0        0 2023-07-05 06:10:00.000000 ex4nicegui-0.1.8/ex4nicegui/reactive/draggable/__init__.py
+-rw-rw-rw-   0        0        0     1356 2023-07-16 10:54:22.000000 ex4nicegui-0.1.8/ex4nicegui/reactive/drawer.py
+drwxrwxrwx   0        0        0        0 2023-07-16 10:57:03.747468 ex4nicegui-0.1.8/ex4nicegui/reactive/echarts/
+-rw-rw-rw-   0        0        0  1581614 2023-07-05 06:10:00.000000 ex4nicegui-0.1.8/ex4nicegui/reactive/echarts/ECharts.js
+-rw-rw-rw-   0        0        0     2559 2023-07-16 10:54:22.000000 ex4nicegui-0.1.8/ex4nicegui/reactive/echarts/ECharts.py
+-rw-rw-rw-   0        0        0        0 2023-07-05 06:10:00.000000 ex4nicegui-0.1.8/ex4nicegui/reactive/echarts/__init__.py
+-rw-rw-rw-   0        0        0     6093 2023-07-16 10:54:22.000000 ex4nicegui-0.1.8/ex4nicegui/reactive/local_file_picker.py
+-rw-rw-rw-   0        0        0    38721 2023-07-16 10:54:22.000000 ex4nicegui-0.1.8/ex4nicegui/reactive/officials.py
+-rw-rw-rw-   0        0        0     1217 2023-07-16 10:54:22.000000 ex4nicegui-0.1.8/ex4nicegui/reactive/q_pagination.py
+-rw-rw-rw-   0        0        0       24 2023-07-09 14:56:08.000000 ex4nicegui-0.1.8/ex4nicegui/reactive/rxui.py
+drwxrwxrwx   0        0        0        0 2023-07-16 10:57:03.752437 ex4nicegui-0.1.8/ex4nicegui/reactive/useMouse/
+-rw-rw-rw-   0        0        0     2722 2023-07-08 17:55:18.000000 ex4nicegui-0.1.8/ex4nicegui/reactive/useMouse/UseMouse.js
+-rw-rw-rw-   0        0        0     2142 2023-07-16 10:54:22.000000 ex4nicegui-0.1.8/ex4nicegui/reactive/useMouse/UseMouse.py
+-rw-rw-rw-   0        0        0        0 2023-07-08 17:55:18.000000 ex4nicegui-0.1.8/ex4nicegui/reactive/useMouse/__init__.py
+-rw-rw-rw-   0        0        0     2093 2023-07-14 15:33:47.000000 ex4nicegui-0.1.8/ex4nicegui/reactive/usePagination.py
+drwxrwxrwx   0        0        0        0 2023-07-16 10:57:03.756441 ex4nicegui-0.1.8/ex4nicegui/tools/
+-rw-rw-rw-   0        0        0       40 2023-07-08 17:55:18.000000 ex4nicegui-0.1.8/ex4nicegui/tools/__init__.py
+-rw-rw-rw-   0        0        0     4887 2023-07-10 13:40:51.000000 ex4nicegui-0.1.8/ex4nicegui/tools/debug.py
+drwxrwxrwx   0        0        0        0 2023-07-16 10:57:03.787434 ex4nicegui-0.1.8/ex4nicegui/utils/
+-rw-rw-rw-   0        0        0        0 2023-07-05 06:10:00.000000 ex4nicegui-0.1.8/ex4nicegui/utils/__init__.py
+-rw-rw-rw-   0        0        0      430 2023-07-08 17:55:18.000000 ex4nicegui-0.1.8/ex4nicegui/utils/common.py
+-rw-rw-rw-   0        0        0     4807 2023-07-10 14:31:39.000000 ex4nicegui-0.1.8/ex4nicegui/utils/signals.py
+drwxrwxrwx   0        0        0        0 2023-07-16 10:57:03.691351 ex4nicegui-0.1.8/ex4nicegui.egg-info/
+-rw-rw-rw-   0        0        0      481 2023-07-16 10:57:03.000000 ex4nicegui-0.1.8/ex4nicegui.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1092 2023-07-16 10:57:03.000000 ex4nicegui-0.1.8/ex4nicegui.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-16 10:57:03.000000 ex4nicegui-0.1.8/ex4nicegui.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-07-16 10:57:03.000000 ex4nicegui-0.1.8/ex4nicegui.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       46 2023-07-16 10:57:03.000000 ex4nicegui-0.1.8/ex4nicegui.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-07-16 10:57:03.000000 ex4nicegui-0.1.8/ex4nicegui.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-16 10:57:03.790430 ex4nicegui-0.1.8/setup.cfg
+-rw-rw-rw-   0        0        0     1501 2023-07-16 10:54:22.000000 ex4nicegui-0.1.8/setup.py
```

### Comparing `ex4nicegui-0.1.7/LICENSE` & `ex4nicegui-0.1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `ex4nicegui-0.1.7/README.md` & `ex4nicegui-0.1.8/README.md`

 * *Files identical despite different names*

### Comparing `ex4nicegui-0.1.7/ex4nicegui/layout/gridbox.py` & `ex4nicegui-0.1.8/ex4nicegui/layout/gridbox.py`

 * *Files identical despite different names*

### Comparing `ex4nicegui-0.1.7/ex4nicegui/reactive/__index.py` & `ex4nicegui-0.1.8/ex4nicegui/reactive/__index.py`

 * *Files 4% similar despite different names*

```diff
@@ -18,14 +18,17 @@
     RowBindableUi as row,
     CardBindableUi as card,
     CardSectionBindableUi as card_section,
     CardActionsBindableUi as card_actions,
     SliderBindableUi as slider,
     LazySliderBindableUi as lazy_slider,
     HtmlBindableUi as html,
+    ImageBindableUi as image,
+    UploadBindableUi as upload,
+    UploadResult,
 )
 from .q_pagination import QPagination as q_pagination
 from .local_file_picker import local_file_picker
 from ex4nicegui.utils.signals import ref_computed
 from signe import effect
 from .draggable.UseDraggable import use_draggable
 from .useMouse.UseMouse import use_mouse
```

### Comparing `ex4nicegui-0.1.7/ex4nicegui/reactive/draggable/UseDraggable.js` & `ex4nicegui-0.1.8/ex4nicegui/reactive/draggable/UseDraggable.js`

 * *Files identical despite different names*

### Comparing `ex4nicegui-0.1.7/ex4nicegui/reactive/draggable/UseDraggable.py` & `ex4nicegui-0.1.8/ex4nicegui/reactive/draggable/UseDraggable.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,19 +1,15 @@
 from typing import Any, Callable, Optional
 from dataclasses import dataclass
-from nicegui import ui
 from nicegui.helpers import KWONLY_SLOTS
 from nicegui.events import handle_event, EventArguments
-from nicegui.dependencies import register_component
 from nicegui.element import Element
 from signe import createSignal, effect, batch
 from ex4nicegui.utils.signals import ref_from_signal
 
-register_component("UseDraggable", __file__, "UseDraggable.js")
-
 _Update_Args = [
     "x",
     "y",
     "style",
 ]
 
 
@@ -29,15 +25,15 @@
     if auto_bind_style:
         element.style(add=f"position:fixed;left:{init_x}px;top:{init_y}px")
         ud.bind_style(element)
 
     return ud
 
 
-class UseDraggable(Element):
+class UseDraggable(Element, component="UseDraggable.js"):
     def __init__(self, element: Element, init_x=0.0, init_y=0.0) -> None:
         super().__init__("UseDraggable")
         self._props["elementId"] = str(element.id)
         self._props["options"] = {"initialValue": {"x": init_x, "y": init_y}}
 
         self.__style_getter, self.__style_setter = createSignal("")
         self.__x_getter, self.__x_setter = createSignal(init_x)
@@ -49,16 +45,16 @@
             def _():
                 self.__style_setter(args.style)
                 self.__x_setter(args.x)
                 self.__y_setter(args.y)
 
         self.on_update(update)
 
-        def on_isDraggingUpdate(args):
-            self.__isDragging_setter(args["args"]["isDragging"])
+        def on_isDraggingUpdate(e):
+            self.__isDragging_setter(e.args["isDragging"])
             # print(args['args']['isDragging'])
 
         self.on("isDraggingUpdate", on_isDraggingUpdate)
 
     @property
     def x(self):
         return ref_from_signal(self.__x_getter)
@@ -78,16 +74,16 @@
     def bind_style(self, element: Element):
         @effect
         def _():
             element.style(self.__style_getter())
             element.update()
 
     def on_update(self, handler: Optional[Callable[..., Any]]):
-        def inner_handler(args: dict):
-            args = args["args"]
+        def inner_handler(e):
+            args = e.args
             handle_event(
                 handler,
                 UseDraggableUpdateEventArguments(
                     sender=self,
                     client=self.client,
                     x=args["x"],
                     y=args["y"],
```

### Comparing `ex4nicegui-0.1.7/ex4nicegui/reactive/drawer.py` & `ex4nicegui-0.1.8/ex4nicegui/reactive/drawer.py`

 * *Files 2% similar despite different names*

```diff
@@ -45,13 +45,13 @@
     r = DrawerBindableUi(init_value, ele)
 
     @effect
     def _():
         value = "true" if r.value else "false"
         ele.props(f":model-value={value}")
 
-    def on_update(args):
-        r.value = args["args"]
+    def on_update(e):
+        r.value = e.args
 
     ele.on("update:modelValue", on_update)
 
     return r
```

### Comparing `ex4nicegui-0.1.7/ex4nicegui/reactive/echarts/ECharts.js` & `ex4nicegui-0.1.8/ex4nicegui/reactive/echarts/ECharts.js`

 * *Files identical despite different names*

### Comparing `ex4nicegui-0.1.7/ex4nicegui/reactive/echarts/ECharts.py` & `ex4nicegui-0.1.8/ex4nicegui/reactive/echarts/ECharts.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,17 +1,14 @@
 from typing import Any, Callable, Optional
 from dataclasses import dataclass
 from nicegui.helpers import KWONLY_SLOTS
 from nicegui.events import handle_event, EventArguments
-from nicegui.dependencies import register_component
 from nicegui.element import Element
 
 
-register_component("ECharts", __file__, "ECharts.js")
-
 _Chart_Click_Args = [
     "componentType",
     "seriesType",
     "seriesIndex",
     "seriesName",
     "name",
     "dataIndex",
@@ -32,15 +29,15 @@
     dataIndex: int
     data: dict
     dataType: Optional[str]
     value: Any
     color: str
 
 
-class echarts(Element):
+class echarts(Element, component="ECharts.js"):
     def __init__(self, options: dict) -> None:
         super().__init__("ECharts")
         self._props["options"] = options
 
     def update_options(self, options: dict, opts: Optional[dict] = None):
         """update chart options
 
@@ -61,17 +58,16 @@
         self.run_method("updateOptions", options, opts)
         self.update()
         return self
 
     def on_chart_click(
         self, handler: Optional[Callable[[EChartsClickEventArguments], Any]]
     ):
-        def inner_handler(args: dict):
-            args = args["args"]
-            print(args)
+        def inner_handler(e):
+            args = e.args
             handle_event(
                 handler,
                 EChartsClickEventArguments(
                     sender=self,
                     client=self.client,
                     componentType=args["componentType"],
                     seriesType=args["seriesType"],
```

### Comparing `ex4nicegui-0.1.7/ex4nicegui/reactive/local_file_picker.py` & `ex4nicegui-0.1.8/ex4nicegui/reactive/local_file_picker.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import Any, Callable, Optional, cast,List
+from typing import Any, Callable, Optional, cast, List
 from typing_extensions import Literal
 from signe import createSignal, effect, computed
 from nicegui import ui, Tailwind
 from pathlib import Path
 
 from signe.types import TGetter
 from ex4nicegui.utils.signals import Ref, effect_refreshable, ReadonlyRef
@@ -151,27 +151,27 @@
                     "rowData": rowData,
                 }
             )
 
             grid.style("width:50vw")
             # grid.tailwind("w-96")
 
-            def dblClicked(msg):
-                path = cur_dir() / Path(msg["args"]["data"]["名称"])
+            def dblClicked(e):
+                path = cur_dir() / Path(e.args["data"]["名称"])
 
                 if path.is_dir():
                     set_cur_dir(path)
                     return
 
                 if mode == "file" and path.is_file():
                     set_result(str(path.absolute()))
                     dia.close()
 
-            def clicked(msg):
-                path = cur_dir() / Path(msg["args"]["data"]["名称"])
+            def clicked(e):
+                path = cur_dir() / Path(e.args["data"]["名称"])
 
                 if mode == "file" and path.is_dir():
                     return
                 set_selected(str(path))
 
             grid.on("cellDoubleClicked", handler=dblClicked)
             grid.on("cellClicked", handler=clicked)
```

### Comparing `ex4nicegui-0.1.7/ex4nicegui/reactive/officials.py` & `ex4nicegui-0.1.8/ex4nicegui/reactive/officials.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,35 +1,36 @@
 from __future__ import annotations
 import asyncio
+from pathlib import Path
 
 from typing import (
     Any,
     Callable,
     List,
     Optional,
     TypeVar,
     Generic,
     cast,
     Dict,
     Union,
-    overload,
 )
-from typing_extensions import Literal, Self
+from typing_extensions import Literal
 from signe import effect
 from ex4nicegui.utils.signals import (
     ReadonlyRef,
     Ref,
     ref_computed,
     to_ref,
     to_value,
     is_ref,
     _TMaybeRef as TMaybeRef,
 )
 import ex4nicegui.utils.common as utils_common
 from nicegui import ui
+from nicegui import events as ng_events
 from nicegui.elements.mixins.text_element import TextElement
 from nicegui.elements.mixins.value_element import ValueElement
 from nicegui.elements.mixins.color_elements import (
     TextColorElement,
     QUASAR_COLORS,
     TAILWIND_COLORS,
 )
@@ -168,16 +169,16 @@
 def _convert_kws_ref2value(kws: Dict):
     return {key: to_value(value) for key, value in kws.items()}
 
 
 class SelectBindableUi(SingleValueBindableUi[T, ui.select]):
     @staticmethod
     def _setup_(binder: "SelectBindableUi"):
-        def onValueChanged(args):
-            binder._ref.value = args["args"]["label"]  # type: ignore
+        def onValueChanged(e):
+            binder._ref.value = e.args["label"]  # type: ignore
 
         @effect
         def _():
             binder.element.value = binder.value
 
         binder.element.on("update:modelValue", handler=onValueChanged)
 
@@ -239,16 +240,16 @@
 
         return self
 
 
 class RadioBindableUi(SingleValueBindableUi[bool, ui.radio]):
     @staticmethod
     def _setup_(binder: "RadioBindableUi"):
-        def onValueChanged(args):
-            binder._ref.value = binder.element.options[args["args"]]  # type: ignore
+        def onValueChanged(e):
+            binder._ref.value = binder.element.options[e.args]  # type: ignore
 
         @effect
         def _():
             binder.element.value = binder.value
 
         binder.element.on("update:modelValue", handler=onValueChanged)
 
@@ -297,16 +298,16 @@
 
         return self
 
 
 class SwitchBindableUi(SingleValueBindableUi[bool, ui.switch]):
     @staticmethod
     def _setup_(binder: "SwitchBindableUi"):
-        def onValueChanged(args):
-            binder._ref.value = args["args"]  # type: ignore
+        def onValueChanged(e):
+            binder._ref.value = e.args  # type: ignore
 
         ele = cast(ValueElement, binder.element)
 
         @effect
         def _():
             ele.value = binder.value
 
@@ -346,16 +347,16 @@
 
         return self
 
 
 class CheckboxBindableUi(SingleValueBindableUi[bool, ui.checkbox]):
     @staticmethod
     def _setup_(binder: "CheckboxBindableUi"):
-        def onValueChanged(args):
-            binder._ref.value = args["args"]  # type: ignore
+        def onValueChanged(e):
+            binder._ref.value = e.args  # type: ignore
 
         ele = cast(ValueElement, binder.element)
 
         @effect
         def _():
             ele.value = binder.value
 
@@ -435,16 +436,16 @@
     def _ex_setup(self):
         ele = self.element
 
         @effect
         def _():
             ele.value = self.value
 
-        def onModelValueChanged(args):
-            self._ref.value = args["args"] or ""  # type: ignore
+        def onModelValueChanged(e):
+            self._ref.value = e.args or ""  # type: ignore
 
         ele.on("update:modelValue", handler=onModelValueChanged)
 
     def bind_prop(self, prop: str, ref_ui: ReadonlyRef):
         if prop == "value":
             return self.bind_value(ref_ui)
 
@@ -492,15 +493,15 @@
         def onValueChanged():
             self._ref.value = ele.value or ""
 
         ele.on("blur", onValueChanged)
         ele.on("keyup.enter", onValueChanged)
 
 
-_TSliderValue = TypeVar("_TSliderValue", float, int)
+_TSliderValue = TypeVar("_TSliderValue", float, int, None)
 
 
 class SliderBindableUi(SingleValueBindableUi[Optional[_TSliderValue], ui.slider]):
     def __init__(
         self,
         min: TMaybeRef[_TSliderValue],
         max: TMaybeRef[_TSliderValue],
@@ -531,16 +532,16 @@
     def _ex_setup(self):
         ele = self.element
 
         @effect
         def _():
             ele.value = self.value
 
-        def onModelValueChanged(args):
-            self._ref.value = args["args"]  # type: ignore
+        def onModelValueChanged(e):
+            self._ref.value = e.args  # type: ignore
 
         ele.on("update:modelValue", handler=onModelValueChanged)
 
     def bind_prop(self, prop: str, ref_ui: ReadonlyRef):
         if prop == "value":
             return self.bind_value(ref_ui)
 
@@ -553,18 +554,18 @@
 
         return self
 
 
 class LazySliderBindableUi(SliderBindableUi):
     def __init__(
         self,
-        min: TMaybeRef[float],
-        max: TMaybeRef[float],
-        step: TMaybeRef[float] = 1,
-        value: TMaybeRef[float | None] = None,
+        min: TMaybeRef[_TSliderValue],
+        max: TMaybeRef[_TSliderValue],
+        step: TMaybeRef[_TSliderValue] = 1,
+        value: TMaybeRef[_TSliderValue | None] = None,
         on_change: Callable[..., Any] | None = None,
     ) -> None:
         super().__init__(min, max, step, value, on_change)
 
     def _ex_setup(self):
         ele = self.element
 
@@ -611,16 +612,16 @@
     def _ex_setup(self):
         ele = self.element
 
         @effect
         def _():
             ele.value = self.value
 
-        def onModelValueChanged(args):
-            self._ref.value = args["args"]  # type: ignore
+        def onModelValueChanged(e):
+            self._ref.value = e.args  # type: ignore
 
         ele.on("update:modelValue", handler=onModelValueChanged)
 
     def bind_prop(self, prop: str, ref_ui: ReadonlyRef):
         if prop == "value":
             return self.bind_value(ref_ui)
 
@@ -665,16 +666,16 @@
         ele.on("blur", onValueChanged)
         ele.on("keyup.enter", onValueChanged)
 
 
 class LabelBindableUi(SingleValueBindableUi[str, ui.label]):
     @staticmethod
     def _setup_(binder: "LabelBindableUi"):
-        def onValueChanged(args):
-            binder._ref.value = args["args"]["label"]  # type: ignore
+        def onValueChanged(e):
+            binder._ref.value = e.args["label"]  # type: ignore
 
         @effect
         def _():
             binder.element.text = binder.value
 
         binder.element.on("update:modelValue", handler=onValueChanged)
 
@@ -861,16 +862,16 @@
     def _ex_setup(self):
         ele = self._element_picker
 
         @effect
         def _():
             ele._props["modelValue"] = self.value
 
-        def onModelValueChanged(args):
-            self._ref.value = args["args"]  # type: ignore
+        def onModelValueChanged(e):
+            self._ref.value = e.args  # type: ignore
 
         ele.on("update:modelValue", handler=onModelValueChanged)
 
     def bind_prop(self, prop: str, ref_ui: ReadonlyRef):
         if prop == "value":
             return self.bind_value(ref_ui)
 
@@ -904,16 +905,16 @@
     def _ex_setup(self):
         ele = self._element_picker
 
         # @effect
         # def _():
         #     ele._props["modelValue"] = self.value
 
-        def onModelValueChanged(args):
-            self._ref.value = args["args"]  # type: ignore
+        def onModelValueChanged(e):
+            self._ref.value = e.args  # type: ignore
 
         ele.on("change", handler=onModelValueChanged)
 
 
 _TAggridValue = Dict
 
 
@@ -1297,7 +1298,111 @@
     def bind_color(self, ref_ui: ReadonlyRef):
         @effect
         def _():
             ele = self.element
             color = ref_ui.value
             ele._style["color"] = color
             ele.update()
+
+
+class ImageBindableUi(SingleValueBindableUi[Union[str, Path], ui.image]):
+    @staticmethod
+    def _setup_(binder: "ImageBindableUi"):
+        @effect
+        def _():
+            binder.element.on_source_change(binder.value)
+
+    def __init__(
+        self,
+        source: Union[TMaybeRef[str], TMaybeRef[Path]] = "",
+    ) -> None:
+        kws = {
+            "source": source,
+        }
+
+        value_kws = _convert_kws_ref2value(kws)
+
+        element = ui.image(**value_kws)
+
+        super().__init__(source, element)  # type: ignore
+
+        for key, value in kws.items():
+            if is_ref(value):
+                self.bind_prop(key, value)  # type: ignore
+
+        # ImageBindableUi._setup_(self)
+
+    def bind_prop(self, prop: str, ref_ui: ReadonlyRef):
+        if prop == "source":
+            return self.bind_source(ref_ui)
+
+        return super().bind_prop(prop, ref_ui)
+
+    def bind_source(self, ref_ui: ReadonlyRef[Union[str, Path]]):
+        @effect
+        def _():
+            ele = self.element
+            source = ref_ui.value
+            ele.on_source_change(source)
+
+
+class UploadResult:
+    def __init__(self, content: bytes = bytes()):
+        self.content = content
+
+    def get_bytes(self):
+        return self.content
+
+    @property
+    def ready(self):
+        return len(self.content) > 0
+
+
+class UploadBindableUi(SingleValueBindableUi[UploadResult, ui.upload]):
+    @staticmethod
+    def _setup_(binder: "UploadBindableUi"):
+        def on_upload(e: ng_events.UploadEventArguments):
+            binder._ref.value = UploadResult(e.content.read())
+
+        binder._on_upload_callbacks.append(on_upload)
+
+    def __init__(
+        self,
+        multiple: TMaybeRef[bool] = False,
+        max_file_size: Optional[TMaybeRef[int]] = None,
+        max_total_size: Optional[TMaybeRef[int]] = None,
+        max_files: Optional[TMaybeRef[int]] = None,
+        on_upload: Optional[Callable[..., Any]] = None,
+        on_rejected: Optional[Callable[..., Any]] = None,
+        label: TMaybeRef[str] = "",
+        auto_upload: TMaybeRef[bool] = False,
+    ) -> None:
+        kws = {
+            "multiple": multiple,
+            "max_file_size": max_file_size,
+            "max_total_size": max_total_size,
+            "max_files": max_files,
+            "on_rejected": on_rejected,
+            "label": label,
+            "auto_upload": auto_upload,
+        }
+
+        value_kws = _convert_kws_ref2value(kws)
+
+        self._on_upload_callbacks = []
+
+        def _on_upload(e: ng_events.UploadEventArguments):
+            for fn in self._on_upload_callbacks:
+                fn(e)
+
+        if on_upload:
+            self._on_upload_callbacks.append(on_upload)
+
+        element = ui.upload(**value_kws, on_upload=_on_upload)
+
+        super().__init__(UploadResult(), element)  # type: ignore
+
+        for key, value in kws.items():
+            if is_ref(value):
+                self.bind_prop(key, value)  # type: ignore
+
+        UploadBindableUi._setup_(self)
```

### Comparing `ex4nicegui-0.1.7/ex4nicegui/reactive/q_pagination.py` & `ex4nicegui-0.1.8/ex4nicegui/reactive/q_pagination.py`

 * *Files 12% similar despite different names*

```diff
@@ -23,16 +23,16 @@
     ) -> None:
         super().__init__(tag="q-pagination")
 
         self.__value = value
         self.__min = min
         self.__max = max
 
-        def onchange(arg):
-            arg_value = cast(int, arg["args"])
+        def onchange(e):
+            arg_value = cast(int, e.args)
 
             self._props["model-value"] = arg_value
             if isinstance(self.__value, Ref):
                 self.__value.value = arg_value
             self.update()
 
         self.on("update:model-value", onchange)
```

### Comparing `ex4nicegui-0.1.7/ex4nicegui/reactive/useMouse/UseMouse.js` & `ex4nicegui-0.1.8/ex4nicegui/reactive/useMouse/UseMouse.js`

 * *Files identical despite different names*

### Comparing `ex4nicegui-0.1.7/ex4nicegui/reactive/useMouse/UseMouse.py` & `ex4nicegui-0.1.8/ex4nicegui/reactive/useMouse/UseMouse.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,33 +1,30 @@
 from typing import Any, Callable, Optional
 from dataclasses import dataclass
 from nicegui.helpers import KWONLY_SLOTS
 from nicegui.events import handle_event, EventArguments
-from nicegui.dependencies import register_component
 from nicegui.element import Element
 from signe import createSignal, effect, batch
 
 
-register_component("UseMouse", __file__, "UseMouse.js")
-
 _Update_Args = [
     "x",
     "y",
     "sourceType",
 ]
 
 
 @dataclass(**KWONLY_SLOTS)
 class UseMouseUpdateEventArguments(EventArguments):
     x: float
     y: float
     sourceType: str
 
 
-class UseMouse(Element):
+class UseMouse(Element, component="UseMouse.js"):
     def __init__(self, options: Optional[dict] = None) -> None:
         super().__init__("UseMouse")
 
         if options:
             self._props["options"] = options
 
         self.__x_getter, self.__x_setter = createSignal(0.0)
@@ -52,16 +49,16 @@
         return self.__y_getter()
 
     @property
     def sourceType(self):
         return self.__sourceType_getter()
 
     def on_update(self, handler: Optional[Callable[..., Any]]):
-        def inner_handler(args: dict):
-            args = args["args"]
+        def inner_handler(e):
+            args = e.args
             handle_event(
                 handler,
                 UseMouseUpdateEventArguments(
                     sender=self,
                     client=self.client,
                     x=args["x"],
                     y=args["y"],
```

### Comparing `ex4nicegui-0.1.7/ex4nicegui/reactive/usePagination.py` & `ex4nicegui-0.1.8/ex4nicegui/reactive/usePagination.py`

 * *Files identical despite different names*

### Comparing `ex4nicegui-0.1.7/ex4nicegui/tools/debug.py` & `ex4nicegui-0.1.8/ex4nicegui/tools/debug.py`

 * *Files identical despite different names*

### Comparing `ex4nicegui-0.1.7/ex4nicegui/utils/signals.py` & `ex4nicegui-0.1.8/ex4nicegui/utils/signals.py`

 * *Files identical despite different names*

### Comparing `ex4nicegui-0.1.7/ex4nicegui.egg-info/SOURCES.txt` & `ex4nicegui-0.1.8/ex4nicegui.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ex4nicegui-0.1.7/setup.py` & `ex4nicegui-0.1.8/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 
     return list(all_infos)
 
 
 with open("README.md", encoding="utf8") as readme_file:
     readme = readme_file.read()
 
-requirements = ["signe>=0.1.8", "nicegui>=1.2.24", "typing_extensions"]
+requirements = ["signe>=0.1.8", "nicegui>=1.3.3", "typing_extensions"]
 
 test_requirements = ["pytest>=3"]
 
 setup(
     author="carson_jia",
     author_email="568166495@qq.com",
     python_requires=">=3.7",
@@ -33,46 +33,22 @@
         "Intended Audience :: Developers",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
     ],
     description="...",
-    entry_points={
-        # 'console_scripts': [
-        #     'test_prj=test_prj.cli:main',
-        # ],
-    },
+    entry_points={},
     install_requires=requirements,
     license="MIT license",
     # long_description=readme,
     include_package_data=True,
     keywords=["nicegui", "ex4nicegui", "webui"],
     name="ex4nicegui",
     packages=find_packages(include=["ex4nicegui", "ex4nicegui.*"]),
     data_files=get_data_files("ex4nicegui/reactive"),
-    # data_files=[
-    #     (
-    #         "echarts",
-    #         [
-    #             "ex4nicegui/reactive/echarts/ECharts.js",
-    #         ],
-    #     ),
-    #     (
-    #         "draggable",
-    #         [
-    #             "ex4nicegui/reactive/draggable/UseDraggable.js",
-    #         ],
-    #     ),
-    #     (
-    #         "useMouse",
-    #         [
-    #             "ex4nicegui/reactive/useMouse/UseMouse.js",
-    #         ],
-    #     ),
-    # ],
     test_suite="__tests",
     tests_require=test_requirements,
     url="",
     version=ex4nicegui.__version__,
     zip_safe=False,
 )
```

