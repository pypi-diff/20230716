# Comparing `tmp/agency-1.2.1.tar.gz` & `tmp/agency-1.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "agency-1.2.1.tar", max compression
+gzip compressed data, was "agency-1.2.2.tar", max compression
```

## Comparing `agency-1.2.1.tar` & `agency-1.2.2.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0    35148 2023-07-14 04:43:27.409218 agency-1.2.1/LICENSE
--rw-r--r--   0        0        0     9366 2023-07-14 04:43:27.409218 agency-1.2.1/README.md
--rw-r--r--   0        0        0        0 2023-07-14 04:43:27.409218 agency-1.2.1/agency/__init__.py
--rw-r--r--   0        0        0     9516 2023-07-14 04:43:27.409218 agency-1.2.1/agency/agent.py
--rw-r--r--   0        0        0     6808 2023-07-14 04:43:27.409218 agency-1.2.1/agency/amqp_space.py
--rw-r--r--   0        0        0     2770 2023-07-14 04:43:27.409218 agency-1.2.1/agency/native_space.py
--rw-r--r--   0        0        0      802 2023-07-14 04:43:27.409218 agency-1.2.1/agency/schema.py
--rwxr-xr-x   0        0        0      754 2023-07-14 04:43:27.409218 agency-1.2.1/agency/space.py
--rw-r--r--   0        0        0     3824 2023-07-14 04:43:27.409218 agency-1.2.1/agency/util.py
--rw-r--r--   0        0        0      540 2023-07-14 04:43:28.548783 agency-1.2.1/pyproject.toml
--rw-r--r--   0        0        0    10041 1970-01-01 00:00:00.000000 agency-1.2.1/PKG-INFO
+-rw-r--r--   0        0        0    35148 2023-07-16 09:53:16.905806 agency-1.2.2/LICENSE
+-rw-r--r--   0        0        0     9675 2023-07-16 09:53:16.905806 agency-1.2.2/README.md
+-rw-r--r--   0        0        0        0 2023-07-16 09:53:16.905806 agency-1.2.2/agency/__init__.py
+-rw-r--r--   0        0        0     9502 2023-07-16 09:53:16.905806 agency-1.2.2/agency/agent.py
+-rw-r--r--   0        0        0     7953 2023-07-16 09:53:16.905806 agency-1.2.2/agency/amqp_space.py
+-rw-r--r--   0        0        0     2770 2023-07-16 09:53:16.905806 agency-1.2.2/agency/native_space.py
+-rw-r--r--   0        0        0      802 2023-07-16 09:53:16.905806 agency-1.2.2/agency/schema.py
+-rwxr-xr-x   0        0        0      754 2023-07-16 09:53:16.905806 agency-1.2.2/agency/space.py
+-rw-r--r--   0        0        0     3824 2023-07-16 09:53:16.905806 agency-1.2.2/agency/util.py
+-rw-r--r--   0        0        0      568 2023-07-16 09:53:18.641885 agency-1.2.2/pyproject.toml
+-rw-r--r--   0        0        0    10350 1970-01-01 00:00:00.000000 agency-1.2.2/PKG-INFO
```

### Comparing `agency-1.2.1/LICENSE` & `agency-1.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `agency-1.2.1/README.md` & `agency-1.2.2/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,47 +1,48 @@
 # Summary
 
 `agency` is a python library that provides a communication and action framework
-for creating AI agent-integrated applications.
+for creating AI agent-integrated systems.
 
-The library provides a low-level means for connecting agents, systems, and human
-users by defining actions, callbacks, and access policies that you can use to
-connect, monitor, control, and interact with your agents.
-
-`agency` handles the details of the common messaging system and allows
-discovering and invoking actions across parties, automatically handling things
-such as reporting exceptions, enforcing access restrictions, and more.
+The library provides a foundation for connecting agents, software systems, and
+human users by defining actions, callbacks, and access policies that you can use
+to connect, monitor, control, and interact with your agents.
+
+`agency` handles the communication details and allows discovering and invoking
+actions across parties, automatically handling things such as reporting
+exceptions, enforcing access restrictions, and more.
 
 
 ## Features
 
 ### Low-Level API Flexibility
-  * Straightforward class/method based agent and action definition
-  * Supports defining single process applications or networked agent systems
-  using AMQP
+* Straightforward class/method based agent and action definition
+* Supports defining single process applications or networked agent systems
+using AMQP
 
 ### Observability and Control
-  * Before/after action and lifecycle callbacks for observability or other needs
-  * Access policies and permission callbacks for access control
+* Before/after action and lifecycle callbacks for observability or other needs
+* Access policies and permission callbacks for access control
 
 ### Performance
-  * Multithreaded (though python's GIL is a bottleneck for single process apps)
-  * AMQP support for multiprocess and networked systems (avoids GIL)
-  * [_Python multiprocess support is planned for better scalability on
-    single-host systems_](https://github.com/operand/agency/issues/33)
-
-### Multimodal (image/audio) support
-  * [_Not yet developed, but is planned_](https://github.com/operand/agency/issues/27)
+* Multithreaded (though python's GIL is a bottleneck for single process apps)
+* AMQP support for multiprocess and networked systems (avoids GIL)
+* [_Python multiprocess support is planned for better scalability on
+  single-host systems_](https://github.com/operand/agency/issues/33)
+
+### Multimodal support
+* [_In development_](https://github.com/operand/agency/issues/26), though a
+timeline of features is not yet determined.
 
 ### Full demo available at [`examples/demo`](./examples/demo/)
-  * Two OpenAI agent examples
-  * HuggingFace transformers agent example
-  * Simple Flask/React web interface included
-  * Operating system access for agents
-  * Docker configuration for reference and development
+* Two OpenAI agent examples
+* HuggingFace transformers agent example
+* Simple Flask/React web interface included
+* Operating system access for agents
+* Docker configuration for reference and development
 
 
 # API Overview
 
 `agency` is an implementation of the [Actor
 model](https://en.wikipedia.org/wiki/Actor_model) for building AI agent
 integrated systems.
@@ -139,20 +140,16 @@
 
 # Running the Demo Application
 
 To run the demo, please follow the directions at
 [examples/demo](./examples/demo/). After a short boot time you can visit the
 web app at `http://localhost:8080` and you should see a simple chat interface.
 
-The following is a screenshot of the web UI that demonstrates the multiple demo
-agents intelligently interacting and following orders.
-
-There are two OpenAI based agents: `"FunctionAI"` and `"CompletionAI"`, named
-for the API's they use, and `"Chatty"` a simple chat agent who uses a small
-local transformers based model for demonstration.
+The following is a screenshot of the web UI that demonstrates multiple demo
+agents interacting and following orders.
 
 The screenshot also demonstrates the results of rejecting an action and
 directing an agent to use a different approach in real time. After I explained
 my rejection of the `read_file` action (which happened behind the scenes on the
 terminal), `"FunctionAI"` appropriately used the `shell_command` action with `wc
 -l Dockerfile`.
 
@@ -160,52 +157,59 @@
   <img src="https://i.ibb.co/nbvLJvg/Screenshot-2023-06-14-at-3-59-01-AM.png"
        alt="Screenshot-2023-06-14-at-3-59-01-AM" border="0" width=500>
 </p>
 
 
 # FAQ
 
-## How does `agency` compare to agent libraries like LangChain?
+## How does `agency` compare to other agent libraries?
 
 Though you could entirely create a simple agent using only the primitives in
 `agency` (see [`examples/demo/agents/`](./examples/demo/agents/)), it is not
-intended to be a full-fledged agent toolset like other libraries or tools.
-
-`agency` is an application framework focused on the problems surrounding
-agent/tool/human integration, such as communication, observability, and access
-control. The library strives to provide a minimal yet practical foundation for
-defining and integrating agent-based systems, allowing developers the freedom
-to experiment with different agent solutions as they desire.
+intended to be an agent toolset like other libraries.
 
+`agency` is a framework for defining and integrating agent-driven systems. It
+strives to provide a practical yet minimal foundation, allowing developers the
+freedom to create custom agent-integrated solutions as they see fit.
+
+So while you might use other libraries for implementing agent behavior, you can
+use `agency` for providing the foundation on which to define, connect, and
+control your agents.
 
 ## What are some known limitations or issues?
 
-* It's a new project, so keep that in mind in terms of
-  completeness, but see [the issues
-  page](https://github.com/operand/agency/issues) for what is currently planned,
-  and the [Roadmap](#roadmap) below for the high level plan.
+* `agency` is still in early development. Like many projects in the AI agent
+  space it is somewhat experimental at this time, with the goal of finding and
+  providing a minimal yet useful foundation for building AI agent systems.
+
+  Expect changes to the API over time as features are added or changed. Stay up
+  to date on changes by following the
+  [issues](https://github.com/operand/agency/issues) or
+  [discussions](https://github.com/operand/agency/discussions) pages and please
+  reach out regarding bugs, features, ideas, or any feedback you'd like to
+  share.
 
 * This library makes use of threads for each individual agent. Multithreading
   is limited by [python's
   GIL](https://wiki.python.org/moin/GlobalInterpreterLock), meaning that if you
   run a local model or other heavy computation in the same process as other
   agents, they may have to wait for their "turn". Note that I/O does not block,
   so networked backends or services will execute in parallel.
-  
+
   For blocking processes, it's recommended to use the `AMQPSpace` class and run
   heavy computations in isolation to avoid blocking other agents.
 
 * This API does not assume or enforce predefined roles like "user", "system",
   "assistant", etc. This is an intentional decision and is not likely to change.
 
   `agency` is intended to allow potentially large numbers of agents, systems,
   and people to come together. A small predefined set of roles gets in the way
-  of representing many things generally. This is a core feature of `agency`:
-  that all entities are treated the same and may be interacted with through
-  common means.
+  of representing many things generally. This is a core design feature of
+  `agency`: that all entities are treated similarly and may be interacted with
+  through common means.
 
   The lack of roles may require extra translation code when integrating with
   role based APIs. See the implementation of
   [`OpenAIFunctionAgent`](./examples/demo/agents/openai_function_agent.py) for
   an example.
 
 * There is currently not much by way of storage support. That is mostly left up
@@ -249,32 +253,35 @@
 You can run the test suite with:
 
 ```bash
 poetry run pytest
 ```
 
 
-
 # Roadmap
 
 - **Multiprocess Support**:
 An additional space type utilizing python multiprocessing, as another
 parallelism option for single-host systems.
 
 - **Multimodal Support**:
-Image/audio transfer for use with multimodal models or other multimedia
-services.
+Multimedia transfer for use with multimodal models or other multimedia services.
 
 - **Storage Support**
 Durable session support will be included. Other forms of storage will be
-considered as well though it's not clear yet what that will look like.
+considered though it's not clear yet what that may look like.
+
+- **Starter Application**
+The current demo application is proof-of-concept quality. A more modern and
+higher quality application will be developed to replace the main demo and serve
+as a reference example that can be extended or modified.
 
 - **More Examples**:
-More examples of integrations with popular AI libraries and tools such as
-Langchain and oobabooga.
+More examples of integrations with popular AI libraries and services will be
+added.
 
 
 ## Planned Work
 
 [Please see the issues page.](https://github.com/operand/agency/issues)
 
 If you have any suggestions or otherwise, feel free to add an issue!
```

### Comparing `agency-1.2.1/agency/agent.py` & `agency-1.2.2/agency/agent.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import inspect
 import re
 import threading
 from typing import List
 
 from colorama import Fore, Style
 
-from agency.schema import ActionSchema, MessageSchema
+from agency.schema import MessageSchema
 
 # access keys
 ACCESS = "access"
 ACCESS_PERMITTED = "permitted"
 ACCESS_DENIED = "denied"
 ACCESS_REQUESTED = "requested"
```

### Comparing `agency-1.2.1/agency/amqp_space.py` & `agency-1.2.2/agency/amqp_space.py`

 * *Files 14% similar despite different names*

```diff
@@ -44,15 +44,15 @@
             'userid': amqp_options.username,
             'password': amqp_options.password,
             'virtual_host': amqp_options.virtual_host,
             'ssl': amqp_options.use_ssl,
             'heartbeat': amqp_options.heartbeat,
         }
         # setup topic exchange
-        self.__topic_exchange = Exchange(exchange, type="topic")
+        self.__topic_exchange = Exchange(exchange, type="topic", durable=False)
 
     @classmethod
     def default_amqp_options(cls) -> AMQPOptions:
         """
         Returns a default AMQPOptions object configurable from environment
         variables.
         """
@@ -75,33 +75,52 @@
                 None, ""]
             if broadcast and message_data['from'] != agent.id() \
                or not broadcast and message_data['to'] == agent.id():
                 agent._receive(message_data)
 
         def _consume_messages():
             with Connection(**self.__kombu_connection_options) as connection:
+                agent_qid = self.__agent_queue_id(agent)
+
+                # Create a non-exclusive named queue on the agent id,
+                # auto-deleted when the last instance disconnects. This queue is
+                # not used for messaging but for determining whether an agent
+                # has any remaining open connections. I'm not fond of this
+                # approach but it works decently for now.
+                id_queue = Queue(
+                    agent.id(),
+                    exchange=self.__topic_exchange,
+                    routing_key='', # shouldn't receive messages
+                    auto_delete=True
+                )
+                id_queue(connection.channel()).declare()
+
                 # Create a queue for direct messages
                 direct_queue = Queue(
-                    agent.id(),
+                    f"{agent_qid}-direct",
                     exchange=self.__topic_exchange,
                     routing_key=agent.id(),
+                    exclusive=True,
                 )
                 direct_queue(connection.channel()).declare()
 
-                # Create a separate broadcast queue for each agent and bind it to the broadcast key
+                # Create a separate broadcast queue for each agent
                 broadcast_queue = Queue(
-                    f"{agent.id()}_broadcast",
+                    f"{agent_qid}-broadcast",
                     exchange=self.__topic_exchange,
                     routing_key=self.BROADCAST_KEY,
+                    exclusive=True,
                 )
                 broadcast_queue(connection.channel()).declare()
 
-                # Consume messages from both direct and broadcast queues
+                # Consume from direct and broadcast queues. The id_queue is
+                # included for tracking connections but does not receive
+                # messages.
                 with connection.Consumer(
-                    [direct_queue, broadcast_queue],
+                    [id_queue, direct_queue, broadcast_queue],
                     callbacks=[_on_message],
                 ):
                     agent._space = self
                     agent._thread_started.set()
                     while not agent._thread_stopping.is_set():
                         time.sleep(0.01)
                         connection.heartbeat_check()  # sends heartbeat if necessary
@@ -159,28 +178,37 @@
                     'args': {
                         'original_message': message,
                         'error': f"\"{message['to']}\" not found",
                     }
                 }
                 self.__publish(sender.id(), error_message)
 
+    def __agent_queue_id(self, agent: Agent):
+        """
+        Returns a unique queue id for the agent instance based on:
+        - the agent id
+        - the hostname
+        - the process id
+        - the agent object id
+        """
+        return f"{agent.id()}-{socket.gethostname()}-{os.getpid()}-{id(agent)}"
+
     def __publish(self, routing_key: str, message: dict):
         with Connection(**self.__kombu_connection_options) as connection:
             with connection.Producer(serializer="json") as producer:
                 producer.publish(
                     json.dumps(message),
                     exchange=self.__topic_exchange,
                     routing_key=routing_key,
                 )
 
     def __check_queue_exists(self, queue_name):
         with Connection(**self.__kombu_connection_options) as connection:
             try:
                 with connection.channel() as channel:
-                    channel.queue_bind(
+                    channel.queue_declare(
                         queue=queue_name,
-                        exchange=self.__topic_exchange.name,
-                        routing_key=queue_name,
+                        passive=True,
                     )
                 return True
             except ChannelError:
                 return False
```

### Comparing `agency-1.2.1/agency/native_space.py` & `agency-1.2.2/agency/native_space.py`

 * *Files identical despite different names*

### Comparing `agency-1.2.1/agency/schema.py` & `agency-1.2.2/agency/schema.py`

 * *Files identical despite different names*

### Comparing `agency-1.2.1/agency/space.py` & `agency-1.2.2/agency/space.py`

 * *Files identical despite different names*

### Comparing `agency-1.2.1/agency/util.py` & `agency-1.2.2/agency/util.py`

 * *Files identical despite different names*

### Comparing `agency-1.2.1/pyproject.toml` & `agency-1.2.2/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "agency"
-version = "1.2.1"
+version = "1.2.2"
 description = "A fast and minimal actor model framework for building agent-integrated systems"
 authors = ["Daniel Rodriguez"]
 license = "GPL-3.0"
 readme = "README.md"
 include = ["agency/**/*"]
 exclude = ["*"]
 
@@ -14,12 +14,13 @@
 colorama = "^0.4"
 pydantic = "^1.8"
 kombu = "^5.3.1"
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^7.3.2"
 pytest-asyncio = "^0.21.0"
+pytest-randomly = "^3.13.0"
 
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `agency-1.2.1/PKG-INFO` & `agency-1.2.2/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: agency
-Version: 1.2.1
+Version: 1.2.2
 Summary: A fast and minimal actor model framework for building agent-integrated systems
 License: GPL-3.0
 Author: Daniel Rodriguez
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
@@ -15,51 +15,52 @@
 Requires-Dist: kombu (>=5.3.1,<6.0.0)
 Requires-Dist: pydantic (>=1.8,<2.0)
 Description-Content-Type: text/markdown
 
 # Summary
 
 `agency` is a python library that provides a communication and action framework
-for creating AI agent-integrated applications.
+for creating AI agent-integrated systems.
 
-The library provides a low-level means for connecting agents, systems, and human
-users by defining actions, callbacks, and access policies that you can use to
-connect, monitor, control, and interact with your agents.
-
-`agency` handles the details of the common messaging system and allows
-discovering and invoking actions across parties, automatically handling things
-such as reporting exceptions, enforcing access restrictions, and more.
+The library provides a foundation for connecting agents, software systems, and
+human users by defining actions, callbacks, and access policies that you can use
+to connect, monitor, control, and interact with your agents.
+
+`agency` handles the communication details and allows discovering and invoking
+actions across parties, automatically handling things such as reporting
+exceptions, enforcing access restrictions, and more.
 
 
 ## Features
 
 ### Low-Level API Flexibility
-  * Straightforward class/method based agent and action definition
-  * Supports defining single process applications or networked agent systems
-  using AMQP
+* Straightforward class/method based agent and action definition
+* Supports defining single process applications or networked agent systems
+using AMQP
 
 ### Observability and Control
-  * Before/after action and lifecycle callbacks for observability or other needs
-  * Access policies and permission callbacks for access control
+* Before/after action and lifecycle callbacks for observability or other needs
+* Access policies and permission callbacks for access control
 
 ### Performance
-  * Multithreaded (though python's GIL is a bottleneck for single process apps)
-  * AMQP support for multiprocess and networked systems (avoids GIL)
-  * [_Python multiprocess support is planned for better scalability on
-    single-host systems_](https://github.com/operand/agency/issues/33)
-
-### Multimodal (image/audio) support
-  * [_Not yet developed, but is planned_](https://github.com/operand/agency/issues/27)
+* Multithreaded (though python's GIL is a bottleneck for single process apps)
+* AMQP support for multiprocess and networked systems (avoids GIL)
+* [_Python multiprocess support is planned for better scalability on
+  single-host systems_](https://github.com/operand/agency/issues/33)
+
+### Multimodal support
+* [_In development_](https://github.com/operand/agency/issues/26), though a
+timeline of features is not yet determined.
 
 ### Full demo available at [`examples/demo`](./examples/demo/)
-  * Two OpenAI agent examples
-  * HuggingFace transformers agent example
-  * Simple Flask/React web interface included
-  * Operating system access for agents
-  * Docker configuration for reference and development
+* Two OpenAI agent examples
+* HuggingFace transformers agent example
+* Simple Flask/React web interface included
+* Operating system access for agents
+* Docker configuration for reference and development
 
 
 # API Overview
 
 `agency` is an implementation of the [Actor
 model](https://en.wikipedia.org/wiki/Actor_model) for building AI agent
 integrated systems.
@@ -157,20 +158,16 @@
 
 # Running the Demo Application
 
 To run the demo, please follow the directions at
 [examples/demo](./examples/demo/). After a short boot time you can visit the
 web app at `http://localhost:8080` and you should see a simple chat interface.
 
-The following is a screenshot of the web UI that demonstrates the multiple demo
-agents intelligently interacting and following orders.
-
-There are two OpenAI based agents: `"FunctionAI"` and `"CompletionAI"`, named
-for the API's they use, and `"Chatty"` a simple chat agent who uses a small
-local transformers based model for demonstration.
+The following is a screenshot of the web UI that demonstrates multiple demo
+agents interacting and following orders.
 
 The screenshot also demonstrates the results of rejecting an action and
 directing an agent to use a different approach in real time. After I explained
 my rejection of the `read_file` action (which happened behind the scenes on the
 terminal), `"FunctionAI"` appropriately used the `shell_command` action with `wc
 -l Dockerfile`.
 
@@ -178,52 +175,59 @@
   <img src="https://i.ibb.co/nbvLJvg/Screenshot-2023-06-14-at-3-59-01-AM.png"
        alt="Screenshot-2023-06-14-at-3-59-01-AM" border="0" width=500>
 </p>
 
 
 # FAQ
 
-## How does `agency` compare to agent libraries like LangChain?
+## How does `agency` compare to other agent libraries?
 
 Though you could entirely create a simple agent using only the primitives in
 `agency` (see [`examples/demo/agents/`](./examples/demo/agents/)), it is not
-intended to be a full-fledged agent toolset like other libraries or tools.
-
-`agency` is an application framework focused on the problems surrounding
-agent/tool/human integration, such as communication, observability, and access
-control. The library strives to provide a minimal yet practical foundation for
-defining and integrating agent-based systems, allowing developers the freedom
-to experiment with different agent solutions as they desire.
+intended to be an agent toolset like other libraries.
 
+`agency` is a framework for defining and integrating agent-driven systems. It
+strives to provide a practical yet minimal foundation, allowing developers the
+freedom to create custom agent-integrated solutions as they see fit.
+
+So while you might use other libraries for implementing agent behavior, you can
+use `agency` for providing the foundation on which to define, connect, and
+control your agents.
 
 ## What are some known limitations or issues?
 
-* It's a new project, so keep that in mind in terms of
-  completeness, but see [the issues
-  page](https://github.com/operand/agency/issues) for what is currently planned,
-  and the [Roadmap](#roadmap) below for the high level plan.
+* `agency` is still in early development. Like many projects in the AI agent
+  space it is somewhat experimental at this time, with the goal of finding and
+  providing a minimal yet useful foundation for building AI agent systems.
+
+  Expect changes to the API over time as features are added or changed. Stay up
+  to date on changes by following the
+  [issues](https://github.com/operand/agency/issues) or
+  [discussions](https://github.com/operand/agency/discussions) pages and please
+  reach out regarding bugs, features, ideas, or any feedback you'd like to
+  share.
 
 * This library makes use of threads for each individual agent. Multithreading
   is limited by [python's
   GIL](https://wiki.python.org/moin/GlobalInterpreterLock), meaning that if you
   run a local model or other heavy computation in the same process as other
   agents, they may have to wait for their "turn". Note that I/O does not block,
   so networked backends or services will execute in parallel.
-  
+
   For blocking processes, it's recommended to use the `AMQPSpace` class and run
   heavy computations in isolation to avoid blocking other agents.
 
 * This API does not assume or enforce predefined roles like "user", "system",
   "assistant", etc. This is an intentional decision and is not likely to change.
 
   `agency` is intended to allow potentially large numbers of agents, systems,
   and people to come together. A small predefined set of roles gets in the way
-  of representing many things generally. This is a core feature of `agency`:
-  that all entities are treated the same and may be interacted with through
-  common means.
+  of representing many things generally. This is a core design feature of
+  `agency`: that all entities are treated similarly and may be interacted with
+  through common means.
 
   The lack of roles may require extra translation code when integrating with
   role based APIs. See the implementation of
   [`OpenAIFunctionAgent`](./examples/demo/agents/openai_function_agent.py) for
   an example.
 
 * There is currently not much by way of storage support. That is mostly left up
@@ -267,32 +271,35 @@
 You can run the test suite with:
 
 ```bash
 poetry run pytest
 ```
 
 
-
 # Roadmap
 
 - **Multiprocess Support**:
 An additional space type utilizing python multiprocessing, as another
 parallelism option for single-host systems.
 
 - **Multimodal Support**:
-Image/audio transfer for use with multimodal models or other multimedia
-services.
+Multimedia transfer for use with multimodal models or other multimedia services.
 
 - **Storage Support**
 Durable session support will be included. Other forms of storage will be
-considered as well though it's not clear yet what that will look like.
+considered though it's not clear yet what that may look like.
+
+- **Starter Application**
+The current demo application is proof-of-concept quality. A more modern and
+higher quality application will be developed to replace the main demo and serve
+as a reference example that can be extended or modified.
 
 - **More Examples**:
-More examples of integrations with popular AI libraries and tools such as
-Langchain and oobabooga.
+More examples of integrations with popular AI libraries and services will be
+added.
 
 
 ## Planned Work
 
 [Please see the issues page.](https://github.com/operand/agency/issues)
 
 If you have any suggestions or otherwise, feel free to add an issue!
```

