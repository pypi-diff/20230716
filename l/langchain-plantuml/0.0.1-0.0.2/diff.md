# Comparing `tmp/langchain_plantuml-0.0.1.tar.gz` & `tmp/langchain_plantuml-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "langchain_plantuml-0.0.1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "langchain_plantuml-0.0.2.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `langchain_plantuml-0.0.1.tar` & `langchain_plantuml-0.0.2.tar`

### file list

```diff
@@ -1,9 +1,10 @@
--rw-r--r--   0        0        0     1951 2023-07-13 16:21:56.011792 langchain_plantuml-0.0.1/README.md
--rw-r--r--   0        0        0      573 2023-07-13 16:21:56.011792 langchain_plantuml-0.0.1/langchain_plantuml/__init__.py
--rw-r--r--   0        0        0      573 2023-07-13 16:21:56.011792 langchain_plantuml-0.0.1/langchain_plantuml/activity_diagram_beta/__init__.py
--rw-r--r--   0        0        0     9698 2023-07-13 16:21:56.011792 langchain_plantuml-0.0.1/langchain_plantuml/activity_diagram_beta/plantuml_activity_diagram_beta_callback_handler.py
--rw-r--r--   0        0        0      573 2023-07-13 16:21:56.011792 langchain_plantuml-0.0.1/langchain_plantuml/core/__init__.py
--rw-r--r--   0        0        0     2695 2023-07-13 16:21:56.011792 langchain_plantuml-0.0.1/langchain_plantuml/core/plantuml_callback_handler.py
--rw-r--r--   0        0        0      888 2023-07-13 16:21:56.011792 langchain_plantuml-0.0.1/langchain_plantuml/diagram.py
--rw-r--r--   0        0        0     1448 2023-07-13 16:21:56.011792 langchain_plantuml-0.0.1/pyproject.toml
--rw-r--r--   0        0        0     2797 1970-01-01 00:00:00.000000 langchain_plantuml-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0    11356 2023-07-16 15:17:34.720287 langchain_plantuml-0.0.2/LICENSE
+-rw-r--r--   0        0        0     2612 2023-07-16 15:17:34.720287 langchain_plantuml-0.0.2/README.md
+-rw-r--r--   0        0        0      573 2023-07-16 15:17:34.720287 langchain_plantuml-0.0.2/langchain_plantuml/__init__.py
+-rw-r--r--   0        0        0      573 2023-07-16 15:17:34.720287 langchain_plantuml-0.0.2/langchain_plantuml/activity_diagram_beta/__init__.py
+-rw-r--r--   0        0        0     9282 2023-07-16 15:17:34.720287 langchain_plantuml-0.0.2/langchain_plantuml/activity_diagram_beta/plantuml_activity_diagram_beta_callback_handler.py
+-rw-r--r--   0        0        0      573 2023-07-16 15:17:34.720287 langchain_plantuml-0.0.2/langchain_plantuml/core/__init__.py
+-rw-r--r--   0        0        0     2891 2023-07-16 15:17:34.720287 langchain_plantuml-0.0.2/langchain_plantuml/core/plantuml_callback_handler.py
+-rw-r--r--   0        0        0      888 2023-07-16 15:17:34.724287 langchain_plantuml-0.0.2/langchain_plantuml/diagram.py
+-rw-r--r--   0        0        0     1749 2023-07-16 15:17:34.724287 langchain_plantuml-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0     3724 1970-01-01 00:00:00.000000 langchain_plantuml-0.0.2/PKG-INFO
```

### Comparing `langchain_plantuml-0.0.1/README.md` & `langchain_plantuml-0.0.2/README.md`

 * *Files 19% similar despite different names*

```diff
@@ -1,9 +1,16 @@
 # LangChain PlantUML Callback Handler
 
+[![License](https://img.shields.io/badge/License-Apache_2.0-blue.svg)](https://opensource.org/licenses/Apache-2.0)
+[![PyPi version](https://img.shields.io/pypi/v/langchain-plantuml.svg)](https://pypi.org/project/langchain-plantuml/)
+[![lint](https://github.com/coolbeevip/langchain_plantuml/actions/workflows/lint.yml/badge.svg)](https://github.com/coolbeevip/langchain_plantuml/actions/workflows/lint.yml)
+[![Build status](https://github.com/coolbeevip/langchain_plantuml/actions/workflows/release.yml/badge.svg)](https://github.com/coolbeevip/langchain_plantuml/actions)
+[![](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
+[![](https://img.shields.io/pypi/dm/langchain-plantuml)](https://pypi.org/project/langchain-plantuml/)
+
 Subscribe to events using a callback and store them in PlantUML format. You can easily subscribe to events and keep them in a form that is easy to visualize and analyze.
 
 ![](screenshot/scene_agent.png)
 
 ## Quick Start
 
 Install this library:
@@ -49,18 +56,15 @@
     memory=memory,
     callbacks=[callback_handler]
 )
 
 llm_chain.predict(human_input="Hi there my friend")
 llm_chain.predict(human_input="Not too bad - how are you?")
 
-plantuml_content = callback_handler.export_uml_content()
-with open("example.puml", "w") as f:
-    for line in plantuml_content:
-        f.write(str(line) + "\n")
+callback_handler.save_uml_content("example.puml")
 ```
 
 You will get the following PlantUML activity diagram
 
 ![](screenshot/example.png)
 
 ## Exporting PlantUML to PNG
```

### Comparing `langchain_plantuml-0.0.1/langchain_plantuml/__init__.py` & `langchain_plantuml-0.0.2/langchain_plantuml/__init__.py`

 * *Files identical despite different names*

### Comparing `langchain_plantuml-0.0.1/langchain_plantuml/activity_diagram_beta/__init__.py` & `langchain_plantuml-0.0.2/langchain_plantuml/activity_diagram_beta/__init__.py`

 * *Files identical despite different names*

### Comparing `langchain_plantuml-0.0.1/langchain_plantuml/activity_diagram_beta/plantuml_activity_diagram_beta_callback_handler.py` & `langchain_plantuml-0.0.2/langchain_plantuml/activity_diagram_beta/plantuml_activity_diagram_beta_callback_handler.py`

 * *Files 12% similar despite different names*

```diff
@@ -16,194 +16,220 @@
 from typing import Any, Dict, List, Optional, Union
 
 from langchain.schema import AgentAction, AgentFinish, LLMResult
 
 from langchain_plantuml.core.plantuml_callback_handler import \
     BasePlantUMLCallbackHandler
 
-DEFAULT_SKIN_PARAM = ["skinparam activityFontName Arial",
-                      "skinparam activityFontSize 10",
-                      "skinparam activityBorderThickness 1",
-                      "skinparam activityShadowing true",
-                      "skinparam ArrowHeadColor none"]
+DEFAULT_SKIN_PARAM = [
+    "skinparam activityFontName Arial",
+    "skinparam activityFontSize 10",
+    "skinparam activityBorderThickness 1",
+    "skinparam activityShadowing true",
+    "skinparam ArrowHeadColor none",
+]
 
 
 class PlantUMLActivityDiagramCallbackHandler(BasePlantUMLCallbackHandler):
     _runs_metrics: dict = {}
 
-    def __init__(self, color: Optional[str] = None, simplify_prompt: bool = False,
-                 skin_param: List[str] = DEFAULT_SKIN_PARAM) -> None:
+    def __init__(
+        self, color: Optional[str] = None, skin_param: List[str] = DEFAULT_SKIN_PARAM
+    ) -> None:
         super().__init__()
         for param in skin_param:
             self.uml_content.append(param)
         self.uml_content.append("start")
         self.color = color
-        self.simplify_prompt = simplify_prompt
 
     def on_llm_start(
-            self, serialized: Dict[str, Any], prompts: List[str], **kwargs: Any
+        self, serialized: Dict[str, Any], prompts: List[str], **kwargs: Any
     ) -> None:
         run_metric = self._get_run_object(serialized=serialized, **kwargs)
-        activity_name = self \
-            ._wrapper_activity_name(self.on_llm_start.__name__,
-                                    f'{run_metric["name"]}({kwargs["invocation_params"]["model_name"]})')
+        activity_name = self._wrapper_activity_name(
+            self.on_llm_start.__name__,
+            f'{run_metric["name"]}({kwargs["invocation_params"]["model_name"]})',
+        )
         self._append_uml_activity(activity_name)
-        self._append_uml_notes(align='left', notes=self._wrapper_note(prompts[0]))
+        self._append_uml_notes(align="left", notes=self._wrapper_note(prompts[0]))
 
     def on_llm_end(self, response: LLMResult, **kwargs: Any) -> None:
         run_metric = self._get_run_object(**kwargs)
-        time_cost = run_metric['end_time'] - run_metric['begin_time']
+        time_cost = run_metric["end_time"] - run_metric["begin_time"]
         self.prompt_tokens += response.llm_output["token_usage"].prompt_tokens
         self.completion_tokens += response.llm_output["token_usage"].completion_tokens
         self.total_tokens += response.llm_output["token_usage"].total_tokens
-        activity_name = self \
-            ._wrapper_activity_name(self.on_llm_end.__name__,
-                                    f'{run_metric["name"]}\n'
-                                    f'\n* time {time_cost:.2f}s '
-                                    f'\n* prompt_tokens {response.llm_output["token_usage"].prompt_tokens} '
-                                    f'\n* completion_tokens {response.llm_output["token_usage"].completion_tokens} '
-                                    f'\n* total_tokens {response.llm_output["token_usage"].total_tokens};')
+        activity_name = self._wrapper_activity_name(
+            self.on_llm_end.__name__,
+            f'{run_metric["name"]}\n'
+            f"\n* time {time_cost:.2f}s "
+            f'\n* prompt_tokens {response.llm_output["token_usage"].prompt_tokens} '
+            f'\n* completion_tokens {response.llm_output["token_usage"].completion_tokens} '
+            f'\n* total_tokens {response.llm_output["token_usage"].total_tokens};',
+        )
         self._append_uml_activity(activity_name)
         for chats in response.generations:
             for chat in chats:
-                self._append_uml_notes(align='right', notes=self._wrapper_note(chat.text))
+                self._append_uml_notes(
+                    align="right", notes=self._wrapper_note(chat.text)
+                )
 
     def on_llm_new_token(self, token: str, **kwargs: Any) -> None:
         run_metric = self._get_run_object(**kwargs)
-        activity_name = self._wrapper_activity_name(self.on_llm_new_token.__name__, run_metric["name"])
+        activity_name = self._wrapper_activity_name(
+            self.on_llm_new_token.__name__, run_metric["name"]
+        )
         self._append_uml_activity(activity_name)
-        self._append_uml_notes(align='right', notes=self._wrapper_note(token))
+        self._append_uml_notes(align="right", notes=self._wrapper_note(token))
 
     def on_llm_error(
-            self, error: Union[Exception, KeyboardInterrupt], **kwargs: Any
+        self, error: Union[Exception, KeyboardInterrupt], **kwargs: Any
     ) -> None:
         run_metric = self._get_run_object(**kwargs)
-        activity_name = self._wrapper_activity_name(self.on_llm_error.__name__, run_metric["name"])
+        activity_name = self._wrapper_activity_name(
+            self.on_llm_error.__name__, run_metric["name"]
+        )
         self._append_uml_activity(activity_name)
-        self._append_uml_notes(align='right', notes=self._wrapper_note(str(error)))
+        self._append_uml_notes(align="right", notes=self._wrapper_note(str(error)))
 
     def on_chain_start(
-            self, serialized: Dict[str, Any], inputs: Dict[str, Any], **kwargs: Any
+        self, serialized: Dict[str, Any], inputs: Dict[str, Any], **kwargs: Any
     ) -> None:
         run_metric = self._get_run_object(serialized, **kwargs)
-        activity_name = self._wrapper_activity_name(self.on_chain_start.__name__, run_metric["name"])
+        activity_name = self._wrapper_activity_name(
+            self.on_chain_start.__name__, run_metric["name"]
+        )
         self._append_uml_activity(activity_name)
-        self._append_uml_notes(align='left', notes=self._wrapper_note(str(inputs)))
+        self._append_uml_notes(align="left", notes=self._wrapper_note(str(inputs)))
 
     def on_chain_end(self, outputs: Dict[str, Any], **kwargs: Any) -> None:
         run_metric = self._get_run_object(**kwargs)
-        activity_name = self._wrapper_activity_name(self.on_chain_end.__name__, run_metric["name"])
+        activity_name = self._wrapper_activity_name(
+            self.on_chain_end.__name__, run_metric["name"]
+        )
         self._append_uml_activity(activity_name)
-        self._append_uml_notes(align='right', notes=self._wrapper_note(str(outputs)))
+        self._append_uml_notes(align="right", notes=self._wrapper_note(str(outputs)))
 
     def on_chain_error(
-            self, error: Union[Exception, KeyboardInterrupt], **kwargs: Any
+        self, error: Union[Exception, KeyboardInterrupt], **kwargs: Any
     ) -> None:
         run_metric = self._get_run_object(**kwargs)
-        activity_name = self._wrapper_activity_name(self.on_chain_error.__name__, run_metric["name"])
+        activity_name = self._wrapper_activity_name(
+            self.on_chain_error.__name__, run_metric["name"]
+        )
         self._append_uml_activity(activity_name)
-        self._append_uml_notes(align='right #red', notes=self._wrapper_note(str(error)))
+        self._append_uml_notes(align="right #red", notes=self._wrapper_note(str(error)))
 
     def on_tool_start(
-            self,
-            serialized: Dict[str, Any],
-            input_str: str,
-            **kwargs: Any,
+        self,
+        serialized: Dict[str, Any],
+        input_str: str,
+        **kwargs: Any,
     ) -> None:
         pass
         run_metric = self._get_run_object(serialized, **kwargs)
-        activity_name = self._wrapper_activity_name(self.on_tool_start.__name__, run_metric["name"])
+        activity_name = self._wrapper_activity_name(
+            self.on_tool_start.__name__, run_metric["name"]
+        )
         self._append_uml_activity(activity_name)
-        self._append_uml_notes(align='left', notes=self._wrapper_note(input_str))
+        self._append_uml_notes(align="left", notes=self._wrapper_note(input_str))
 
     def on_agent_action(
-            self, action: AgentAction, color: Optional[str] = None, **kwargs: Any
+        self, action: AgentAction, color: Optional[str] = None, **kwargs: Any
     ) -> Any:
         run_metric = self._get_run_object(**kwargs)
-        if kwargs['parent_run_id'] is not None:
-            activity_name = self._wrapper_activity_name(self.on_agent_action.__name__, run_metric["name"])
+        if kwargs["parent_run_id"] is not None:
+            activity_name = self._wrapper_activity_name(
+                self.on_agent_action.__name__, run_metric["name"]
+            )
             self._append_uml_activity(activity_name)
 
     def on_tool_end(
-            self,
-            output: str,
-            color: Optional[str] = None,
-            observation_prefix: Optional[str] = None,
-            llm_prefix: Optional[str] = None,
-            **kwargs: Any,
-    ) -> None:
-        run_metric = self._get_run_object(**kwargs)
-        activity_name = self._wrapper_activity_name(self.on_tool_end.__name__, run_metric["name"])
-        self._append_uml_activity(activity_name)
-        # self._append_uml_line('note right')
-        # if observation_prefix is not None:
-        #     self._append_uml_multi_line(self._beautify_note(f"\n{observation_prefix}"))
-        # if llm_prefix is not None:
-        #     self._append_uml_multi_line(self._beautify_note(f"\n{llm_prefix}"))
-        # self._append_uml_line('end note')
+        self,
+        output: str,
+        color: Optional[str] = None,
+        observation_prefix: Optional[str] = None,
+        llm_prefix: Optional[str] = None,
+        **kwargs: Any,
+    ) -> None:
+        run_metric = self._get_run_object(**kwargs)
+        activity_name = self._wrapper_activity_name(
+            self.on_tool_end.__name__, run_metric["name"]
+        )
+        self._append_uml_activity(activity_name)
+        self._append_uml_notes(align="right", notes=self._wrapper_note(output))
 
     def on_tool_error(
-            self, error: Union[Exception, KeyboardInterrupt], **kwargs: Any
+        self, error: Union[Exception, KeyboardInterrupt], **kwargs: Any
     ) -> None:
         """Do nothing."""
         pass
 
     def on_text(
-            self,
-            text: Any,
-            color: Optional[str] = None,
-            end: str = "",
-            **kwargs: Any,
+        self,
+        text: Any,
+        color: Optional[str] = None,
+        end: str = "",
+        **kwargs: Any,
     ) -> None:
         run_metric = self._get_run_object(**kwargs)
         if type(text) == list:
-            activity_name = self._wrapper_activity_name(self.on_text.__name__, run_metric["name"])
+            activity_name = self._wrapper_activity_name(
+                self.on_text.__name__, run_metric["name"]
+            )
             self._append_uml_activity(activity_name)
-            self._append_uml_notes(align='left',
-                                   notes=[f'Step{index}.{step.value}\n' for index, step in enumerate(text)])
+            self._append_uml_notes(
+                align="left",
+                notes=[
+                    f"Step{index}.{step.value}\n" for index, step in enumerate(text)
+                ],
+            )
 
     def on_agent_finish(
-            self, finish: AgentFinish, color: Optional[str] = None, **kwargs: Any
+        self, finish: AgentFinish, color: Optional[str] = None, **kwargs: Any
     ) -> None:
         run_metric = self._get_run_object(**kwargs)
-        # if kwargs['parent_run_id'] is not None:
-        #     # parent_run_id = str(kwargs['parent_run_id'])
-        #     # parent_run_name = self.runs[parent_run_id]
-        activity_name = self._wrapper_activity_name(self.on_agent_finish.__name__, run_metric["name"])
+        activity_name = self._wrapper_activity_name(
+            self.on_agent_finish.__name__, run_metric["name"]
+        )
         self._append_uml_activity(activity_name)
 
     def export_uml_content(self) -> List[str]:
-        self.uml_content.append('stop')
-        self.uml_content.append('note right')
+        self.uml_content.append("stop")
+        self.uml_content.append("note right")
         self.uml_content.append(
-            f'* prompt_tokens: {self.prompt_tokens} \n'
-            f'* completion_tokens: {self.completion_tokens} \n'
-            f'* total_tokens: {self.total_tokens}')
-        self.uml_content.append('end note')
+            f"* prompt_tokens: {self.prompt_tokens} \n"
+            f"* completion_tokens: {self.completion_tokens} \n"
+            f"* total_tokens: {self.total_tokens}"
+        )
+        self.uml_content.append("end note")
         self.uml_content.append("@enduml")
         return self.uml_content
 
     def _get_run_object(self, serialized: Dict[str, Any] = None, **kwargs: Any) -> Dict:
-        run_id = str(kwargs['run_id'])
+        run_id = str(kwargs["run_id"])
         if run_id not in self._runs_metrics:
             self._runs_metrics[run_id] = {}
 
-        if 'begin_time' not in self._runs_metrics[run_id]:
-            self._runs_metrics[run_id]['begin_time'] = time.time()
+        if "begin_time" not in self._runs_metrics[run_id]:
+            self._runs_metrics[run_id]["begin_time"] = time.time()
         else:
-            self._runs_metrics[run_id]['end_time'] = time.time()
+            self._runs_metrics[run_id]["end_time"] = time.time()
 
         if serialized is not None:
-            run_name = serialized.get('name') if serialized.get('name') is not None else serialized['id'][
-                len(serialized['id']) - 1]
-            self._runs_metrics[run_id]['name'] = run_name
+            run_name = (
+                serialized.get("name")
+                if serialized.get("name") is not None
+                else serialized["id"][len(serialized["id"]) - 1]
+            )
+            self._runs_metrics[run_id]["name"] = run_name
 
         return self._runs_metrics[run_id]
 
-    def _append_uml_notes(self, align: str = 'left', notes: List[str] = []):
+    def _append_uml_notes(self, align: str = "left", notes: List[str] = []):
         if len(notes) > 0:
-            self._append_uml_line(f'note {align}')
+            self._append_uml_line(f"note {align}")
             self._append_uml_multi_line(notes)
-            self._append_uml_line('end note')
+            self._append_uml_line("end note")
 
     def _wrapper_activity_name(self, method_name: str, run_name: str) -> str:
         return f':{self.step}. {self.emojis[method_name] if method_name in self.emojis else ""} {run_name};'
```

### Comparing `langchain_plantuml-0.0.1/langchain_plantuml/core/__init__.py` & `langchain_plantuml-0.0.2/langchain_plantuml/core/__init__.py`

 * *Files identical despite different names*

### Comparing `langchain_plantuml-0.0.1/langchain_plantuml/core/plantuml_callback_handler.py` & `langchain_plantuml-0.0.2/langchain_plantuml/core/plantuml_callback_handler.py`

 * *Files 7% similar despite different names*

```diff
@@ -21,22 +21,23 @@
 class BasePlantUMLCallbackHandler(BaseCallbackHandler):
     step: int = 0
     uml_content: List[str] = []
     total_tokens: int = 0
     prompt_tokens: int = 0
     completion_tokens: int = 0
     crlf: str = "⏎"
+    note_max_length: int = 1000
     emojis = {
         "on_llm_start": "<:1f916:>",
         "on_llm_end": "<:1f916:>",
         "on_chain_start": "<:1f3af:>",
         "on_chain_end": "<:1f3af:>",
         "on_tool_start": "<:1f528:>",
         "on_tool_end": "<:1f528:>",
-        "on_text": "<:1f4c6:>"
+        "on_text": "<:1f4c6:>",
     }
 
     def __init__(self):
         self.uml_content.append("@startuml")
         self.uml_content.append("skinparam dpi 300")
         self.uml_content.append("skinparam wrapWidth 500")
         self.uml_content.append("skinparam shadowing false")
@@ -49,24 +50,29 @@
         self.uml_content.append("skinparam noteShadowing false")
         self.uml_content.append("skinparam noteArrow none")
 
     @abstractmethod
     def export_uml_content(self) -> List[str]:
         pass
 
+    def save_uml_content(self, file_path: str):
+        with open(file_path, "w") as f:
+            for line in self.export_uml_content():
+                f.write(str(line) + "\n")
+
     def _append_uml_line(self, line):
         self.uml_content.append(line)
 
     def _append_uml_activity(self, line):
         self.uml_content.append(line)
         self.step += 1
 
     def _append_uml_multi_line(self, lines: List[str]):
         for line in lines:
             self.uml_content.append(line)
 
-    def _wrapper_note(self, note: str, line_max_limit: int = 1000) -> List[str]:
+    def _wrapper_note(self, note: str) -> List[str]:
         new_note = note.strip()
-        if len(new_note) > line_max_limit:
-            new_note = new_note[:line_max_limit] + f' ... (Omit {len(new_note) - line_max_limit} words)'
-        new_lines = [f'{line}{self.crlf}' for line in new_note.split('\n')]
+        if len(new_note) > self.note_max_length:
+            new_note = f"new_note[:line_max_limit] ... (Omit {len(new_note) - self.note_max_length} words)"
+        new_lines = [f"{line}{self.crlf}" for line in new_note.split("\n")]
         return new_lines
```

### Comparing `langchain_plantuml-0.0.1/langchain_plantuml/diagram.py` & `langchain_plantuml-0.0.2/langchain_plantuml/diagram.py`

 * *Files identical despite different names*

### Comparing `langchain_plantuml-0.0.1/PKG-INFO` & `langchain_plantuml-0.0.2/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,29 +1,40 @@
 Metadata-Version: 2.1
 Name: langchain-plantuml
-Version: 0.0.1
+Version: 0.0.2
 Summary: Subscribe to events using a callback and store them in PlantUML format. You can easily subscribe to events and keep them in a form that is easy to visualize and analyze.
+Author-email: Lei Zhang <zhanglei@apache.org>
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Requires-Dist: langchain==0.0.228
 Requires-Dist: flake8==5.0.4 ; extra == "lint"
 Requires-Dist: pyproject-flake8==5.0.4 ; extra == "lint"
 Requires-Dist: isort>=5,<6 ; extra == "lint"
 Requires-Dist: black>=23,<24 ; extra == "lint"
 Requires-Dist: flit==3.9.0 ; extra == "package"
 Requires-Dist: openai==0.27.8 ; extra == "test"
 Requires-Dist: chromadb==0.3.26 ; extra == "test"
 Requires-Dist: tiktoken==0.4.0 ; extra == "test"
 Requires-Dist: coverage==7.2.7 ; extra == "test"
+Project-URL: Documentation, https://pypi.org/project/langchain-plantuml
+Project-URL: Source, https://github.com/coolbeevip/langchain_plantuml
+Project-URL: Tracker, https://github.com/coolbeevip/langchain_plantuml/issues
 Provides-Extra: lint
 Provides-Extra: package
 Provides-Extra: test
 
 # LangChain PlantUML Callback Handler
 
+[![License](https://img.shields.io/badge/License-Apache_2.0-blue.svg)](https://opensource.org/licenses/Apache-2.0)
+[![PyPi version](https://img.shields.io/pypi/v/langchain-plantuml.svg)](https://pypi.org/project/langchain-plantuml/)
+[![lint](https://github.com/coolbeevip/langchain_plantuml/actions/workflows/lint.yml/badge.svg)](https://github.com/coolbeevip/langchain_plantuml/actions/workflows/lint.yml)
+[![Build status](https://github.com/coolbeevip/langchain_plantuml/actions/workflows/release.yml/badge.svg)](https://github.com/coolbeevip/langchain_plantuml/actions)
+[![](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
+[![](https://img.shields.io/pypi/dm/langchain-plantuml)](https://pypi.org/project/langchain-plantuml/)
+
 Subscribe to events using a callback and store them in PlantUML format. You can easily subscribe to events and keep them in a form that is easy to visualize and analyze.
 
 ![](screenshot/scene_agent.png)
 
 ## Quick Start
 
 Install this library:
@@ -69,18 +80,15 @@
     memory=memory,
     callbacks=[callback_handler]
 )
 
 llm_chain.predict(human_input="Hi there my friend")
 llm_chain.predict(human_input="Not too bad - how are you?")
 
-plantuml_content = callback_handler.export_uml_content()
-with open("example.puml", "w") as f:
-    for line in plantuml_content:
-        f.write(str(line) + "\n")
+callback_handler.save_uml_content("example.puml")
 ```
 
 You will get the following PlantUML activity diagram
 
 ![](screenshot/example.png)
 
 ## Exporting PlantUML to PNG
```

