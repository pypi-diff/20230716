# Comparing `tmp/dockery-0.7.0.tar.gz` & `tmp/dockery-0.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dockery-0.7.0.tar", last modified: Mon Jul 10 02:31:40 2023, max compression
+gzip compressed data, was "dockery-0.8.0.tar", last modified: Sun Jul 16 03:18:21 2023, max compression
```

## Comparing `dockery-0.7.0.tar` & `dockery-0.8.0.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0     1082 2023-07-10 02:31:29.778195 dockery-0.7.0/LICENSE
--rw-r--r--   0        0        0     1640 2023-07-10 02:31:29.778195 dockery-0.7.0/README.md
--rw-r--r--   0        0        0      777 2023-07-10 02:31:40.654351 dockery-0.7.0/pyproject.toml
--rw-r--r--   0        0        0        0 2023-07-10 02:31:29.778195 dockery-0.7.0/src/dockery/__init__.py
--rw-r--r--   0        0        0     5201 2023-07-10 02:31:29.778195 dockery-0.7.0/src/dockery/containers.py
--rw-r--r--   0        0        0     1734 2023-07-10 02:31:29.778195 dockery-0.7.0/src/dockery/custom_widgets.py
--rw-r--r--   0        0        0     1612 2023-07-10 02:31:29.778195 dockery-0.7.0/src/dockery/gui.py
--rw-r--r--   0        0        0     2082 2023-07-10 02:31:29.778195 dockery-0.7.0/src/dockery/images.py
--rw-r--r--   0        0        0     2022 2023-07-10 02:31:29.778195 dockery-0.7.0/src/dockery/logs.py
--rw-r--r--   0        0        0     4386 2023-07-10 02:31:29.782195 dockery-0.7.0/src/dockery/main.py
--rw-r--r--   0        0        0      126 2023-07-10 02:31:29.782195 dockery-0.7.0/src/dockery/models.py
--rw-r--r--   0        0        0     1742 2023-07-10 02:31:29.782195 dockery-0.7.0/src/dockery/networks.py
--rw-r--r--   0        0        0     1215 2023-07-10 02:31:29.782195 dockery-0.7.0/src/dockery/style.css
--rw-r--r--   0        0        0     1543 2023-07-10 02:31:29.782195 dockery-0.7.0/src/dockery/utils.py
--rw-r--r--   0        0        0     1675 2023-07-10 02:31:29.782195 dockery-0.7.0/src/dockery/volumes.py
--rw-r--r--   0        0        0     2147 1970-01-01 00:00:00.000000 dockery-0.7.0/PKG-INFO
+-rw-r--r--   0        0        0     1082 2023-07-16 03:18:13.750737 dockery-0.8.0/LICENSE
+-rw-r--r--   0        0        0     1493 2023-07-16 03:18:13.750737 dockery-0.8.0/README.md
+-rw-r--r--   0        0        0      777 2023-07-16 03:18:21.466709 dockery-0.8.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-07-16 03:18:13.750737 dockery-0.8.0/src/dockery/__init__.py
+-rw-r--r--   0        0        0     5710 2023-07-16 03:18:13.750737 dockery-0.8.0/src/dockery/containers.py
+-rw-r--r--   0        0        0     1767 2023-07-16 03:18:13.750737 dockery-0.8.0/src/dockery/custom_widgets.py
+-rw-r--r--   0        0        0     1612 2023-07-16 03:18:13.750737 dockery-0.8.0/src/dockery/gui.py
+-rw-r--r--   0        0        0     2175 2023-07-16 03:18:13.750737 dockery-0.8.0/src/dockery/images.py
+-rw-r--r--   0        0        0     2015 2023-07-16 03:18:13.750737 dockery-0.8.0/src/dockery/logs.py
+-rw-r--r--   0        0        0     4386 2023-07-16 03:18:13.750737 dockery-0.8.0/src/dockery/main.py
+-rw-r--r--   0        0        0      126 2023-07-16 03:18:13.750737 dockery-0.8.0/src/dockery/models.py
+-rw-r--r--   0        0        0     1846 2023-07-16 03:18:13.750737 dockery-0.8.0/src/dockery/networks.py
+-rw-r--r--   0        0        0     1200 2023-07-16 03:18:13.750737 dockery-0.8.0/src/dockery/style.css
+-rw-r--r--   0        0        0     1543 2023-07-16 03:18:13.750737 dockery-0.8.0/src/dockery/utils.py
+-rw-r--r--   0        0        0     1848 2023-07-16 03:18:13.750737 dockery-0.8.0/src/dockery/volumes.py
+-rw-r--r--   0        0        0     2000 1970-01-01 00:00:00.000000 dockery-0.8.0/PKG-INFO
```

### Comparing `dockery-0.7.0/LICENSE` & `dockery-0.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `dockery-0.7.0/pyproject.toml` & `dockery-0.8.0/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "dockery"
-version = "0.7.0"
+version = "0.8.0"
 description = "Graphical interface for Docker in your console"
 authors = [
     { name = "Mariano Carrazana", email = "marianocarrazana@gmail.com" },
 ]
 dependencies = [
     "docker>=6.1.3",
     "textual>=0.28.0",
```

### Comparing `dockery-0.7.0/src/dockery/containers.py` & `dockery-0.8.0/src/dockery/containers.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,17 +1,13 @@
 from textual.app import ComposeResult
 from textual.widgets import Static, Label
 from textual.reactive import reactive
 from docker import DockerClient, errors
 from docker.models.containers import Container
-from textual.containers import (
-    Horizontal,
-    Vertical,
-    Container as Group,
-)
+from textual.containers import Horizontal, Vertical
 
 from .utils import get_cpu_usage, get_mem_usage, daemon
 from .logs import LogsButton
 from .custom_widgets import CustomButton, ResponsiveGrid, ReactiveString
 from .models import store
 
 
@@ -21,15 +17,15 @@
     def __init__(self, docker: DockerClient, **kargs):
         self.containers: list[Container] = []
         self.docker = docker
         super().__init__(**kargs)
 
     def on_mount(self) -> None:
         self.get_containers()
-        self.set_interval(2, self.get_containers)
+        self.get_containers_timer = self.set_interval(2, self.get_containers)
 
     async def watch_container_count(self, count: int) -> None:
         await self.grid.remove_children()
         images_in_use = []
         for c in self.containers:
             cw = ContainerWidget(c, self.docker, classes="li")
             self.grid.mount(cw)
@@ -37,45 +33,48 @@
         store.containers_images = images_in_use
 
     @daemon
     def get_containers(self) -> None:
         self.containers = self.docker.containers.list(all=True)  # type: ignore
         self.container_count = len(self.containers)
 
+    def on_hide(self):
+        self.get_containers_timer.pause()
+
+    def on_show(self):
+        self.get_containers_timer.resume()
+
 
 class ContainerWidget(Static):
     def __init__(self, container: Container, client: DockerClient, **kargs):
         self.container = container
         self.client = client
         self.container_id = container.id
         self.running = False
+        self.is_visible = False
+        self.container_name = self.container.name or ""
         super().__init__(**kargs)
 
     def compose(self) -> ComposeResult:
-        yield Group(
-            Label("[b]" + (self.container.name or ""), classes="container-name"),
-            Vertical(
-                ReactiveString(classes="status"),
-                Horizontal(
-                    ReactiveString(classes="cpu"), ReactiveString(classes="mem")
-                ),
-                classes="stats-text",
-            ),
+        yield Vertical(
+            Label(self.container_name, classes="container-name bold"),
+            ReactiveString(classes="status"),
+            Horizontal(ReactiveString(classes="cpu"), ReactiveString(classes="mem")),
             classes="container-info",
         )
-
-        yield Group(StatusButtons(self.container))
+        yield StatusButtons(self.container)
 
     def on_mount(self):
         self.status_widget = self.query_one(".status", ReactiveString)
         self.cpu_widget = self.query_one(".cpu", ReactiveString)
         self.mem_widget = self.query_one(".mem", ReactiveString)
         self.set_interval(1, self.update_data)
         self.mounted = True
         self.update_usage()
+        self.update_data_timer = self.set_interval(1, self.update_data, pause=True)
 
     @daemon
     def update_data(self) -> None:
         try:
             self.container.reload()
         except errors.NotFound:
             return None
@@ -88,27 +87,41 @@
             self.classes = "li running" if self.running else "li"
 
     @daemon
     def update_usage(self) -> None:
         for stat in self.container.stats(stream=True, decode=True):
             if not self.mounted:  # finish the thread
                 return None
+            if not self.is_visible:
+                continue
             if self.running:
-                mem_mb, mem_percent = get_mem_usage(stat)
                 cpu_text = f"CPU: {get_cpu_usage(stat):.1f}%"
-                mem_text = f"MEM: {mem_mb:.1f}MB({mem_percent:.1f}%)"
+                mem, mem_percent = get_mem_usage(stat)
+                data_unit = "MB"
+                if mem >= 1000:
+                    mem = mem / 1000
+                    data_unit = "GB"
+                mem_text = f"MEM: {mem:.1f}{data_unit}({mem_percent:.1f}%)"
             else:
                 cpu_text = "CPU: -"
                 mem_text = "MEM: -"
             self.cpu_widget.text = cpu_text
             self.mem_widget.text = mem_text
 
     def on_unmount(self):
         self.mounted = False
 
+    def on_hide(self):
+        self.update_data_timer.pause()
+        self.is_visible = False
+
+    def on_show(self):
+        self.update_data_timer.resume()
+        self.is_visible = True
+
 
 class StatusButtons(Static):
     def __init__(self, container: Container, **kargs):
         self.container = container
         super().__init__(**kargs)
 
     def compose(self) -> ComposeResult:
@@ -136,15 +149,15 @@
 
     def on_mount(self) -> None:
         self.button = self.query_one(CustomButton)
         self.running = self.container.status == "running"
 
     def watch_running(self, running: bool):
         self.variant = "error" if running else "success"
-        text = ":black_square_button:Stop" if running else ":arrow_forward: Start"
+        text = "▣ Stop" if running else "▶ Start"
         self.button.text = text
         self.button.color = "red" if running else "green"
 
     def compose(self) -> ComposeResult:
         yield CustomButton("Start")
 
 
@@ -153,8 +166,8 @@
         self.container = container
         super().__init__(**kargs)
 
     def on_click(self) -> None:
         self.container.restart()
 
     def compose(self) -> ComposeResult:
-        yield CustomButton(":grey_exclamation:Restart", color="orange")
+        yield CustomButton("↻ Restart", color="orange")
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `dockery-0.7.0/src/dockery/custom_widgets.py` & `dockery-0.8.0/src/dockery/custom_widgets.py`

 * *Files 3% similar despite different names*

```diff
@@ -18,26 +18,27 @@
         super().__init__(shrink=True, expand=True, **kargs)
 
     def render(self) -> TextType:
         return self.text
 
     def watch_color(self, new_color: str):
         if new_color != "":
-            self.styles.outline = (self.variant, new_color) # type: ignore
+            self.styles.outline = (self.variant, new_color)  # type: ignore
 
     def on_mount(self) -> None:
         self.text = self.start_text
         self.color = self.start_color
 
 
 class ResponsiveGrid(VerticalScroll):
     container_count = reactive(0)
 
     def __init__(self, **kargs):
         self.grid = Grid()
+        self.is_visible = False
         super().__init__(**kargs)
 
     def compose(self) -> ComposeResult:
         yield self.grid
 
     def on_mount(self) -> None:
         self.resize()
```

### Comparing `dockery-0.7.0/src/dockery/gui.py` & `dockery-0.8.0/src/dockery/gui.py`

 * *Files identical despite different names*

### Comparing `dockery-0.7.0/src/dockery/images.py` & `dockery-0.8.0/src/dockery/images.py`

 * *Files 15% similar despite different names*

```diff
@@ -16,27 +16,33 @@
     def __init__(self, docker: DockerClient, **kargs):
         self.images: list[Image] = []
         self.docker = docker
         super().__init__(**kargs)
 
     def on_mount(self) -> None:
         self.get_images()
-        self.set_interval(2, self.get_images)
+        self.get_images_timer = self.set_interval(2, self.get_images, pause=True)
 
     async def watch_images_count(self, count: int) -> None:
         await self.grid.remove_children()
         for c in self.images:
             cw = ImageWidget(c, self.docker, classes="li")
             self.grid.mount(cw)
 
     @daemon
     def get_images(self) -> None:
         self.images = self.docker.images.list(all=False)  # type: ignore
         self.images_count = len(self.images)
 
+    def on_hide(self):
+        self.get_images_timer.pause()
+
+    def on_show(self):
+        self.get_images_timer.resume()
+
 
 class ImageWidget(Static):
     def __init__(self, image: Image, client: DockerClient, **kargs):
         self.image = image
         self.client = client
         self.attrs = image.attrs or {}
         self.isize = self.attrs.get("Size", 0) / 1000000
@@ -57,12 +63,10 @@
         )
 
     def on_mount(self):
         self.set_interval(2, self.update_usage)
 
     @daemon
     def update_usage(self):
-        print(self.image.id)
-        print(store.containers_images)
         self.classes = (
             "li running" if self.image.id in store.containers_images else "li"
         )
```

### Comparing `dockery-0.7.0/src/dockery/logs.py` & `dockery-0.8.0/src/dockery/logs.py`

 * *Files 1% similar despite different names*

```diff
@@ -23,15 +23,15 @@
     async def on_click(self) -> None:
         await self.logs_container.remove_children()
         lc = LogsContainer(self.container)
         await self.logs_container.mount(lc)
         self.tabs.active = "container-logs"
 
     def compose(self) -> ComposeResult:
-        yield CustomButton(":notebook:Logs", color="blue")
+        yield CustomButton("Ξ Logs", color="blue")
 
 
 class LogsContainer(TextLog):
     last_log = reactive("")
 
     def __init__(self, container: Container, **kargs):
         self.container = container
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `dockery-0.7.0/src/dockery/main.py` & `dockery-0.8.0/src/dockery/main.py`

 * *Files identical despite different names*

### Comparing `dockery-0.7.0/src/dockery/networks.py` & `dockery-0.8.0/src/dockery/networks.py`

 * *Files 15% similar despite different names*

```diff
@@ -15,30 +15,33 @@
     def __init__(self, docker: DockerClient, **kargs):
         self.networks = []
         self.docker = docker
         super().__init__(**kargs)
 
     def on_mount(self) -> None:
         self.get_networks()
-        self.set_interval(2, self.count_timer)
-
-    def count_timer(self) -> None:
-        self.get_networks()
+        self.get_networks_timer = self.set_interval(2, self.get_networks, pause=True)
 
     async def watch_networks_count(self, count: int) -> None:
         await self.grid.remove_children()
         for c in self.networks:
             cw = NetworkWidget(c, self.docker, classes="li")  # type: ignore
             self.grid.mount(cw)
 
     @daemon
     def get_networks(self) -> None:
         self.networks = self.docker.networks.list()
         self.networks_count = len(self.networks)
 
+    def on_hide(self):
+        self.get_networks_timer.pause()
+
+    def on_show(self):
+        self.get_networks_timer.resume()
+
 
 class NetworkWidget(Static):
     def __init__(self, network: Network, client: DockerClient, **kargs):
         self.network = network
         self.client = client
         self.attrs = network.attrs or {}
         self.isize = self.attrs.get("Size", 0) / 1000 / 1000
```

### Comparing `dockery-0.7.0/src/dockery/style.css` & `dockery-0.8.0/src/dockery/style.css`

 * *Files 11% similar despite different names*

```diff
@@ -40,34 +40,38 @@
     width: 1fr;
 }
 
 .stats-text {
     width: 1fr;
 }
 
-.stats-text > Horizontal > ReactiveString.cpu {
+ReactiveString.cpu {
     width: 12;
     height: 1;
 }
 
-.stats-text > Horizontal > ReactiveString.mem {
-    width: 20;
+ReactiveString.mem {
+    width: 1fr;
     height: 1;
 }
 
 CustomButton {
     height: 3;
     padding: 1 2;
     width: auto;
 }
 
 CustomButton:hover {
     text-style: bold;
 }
 
+StatusButtons {
+    width: 35;
+}
+
 LogsButton {
     width: 10;
 }
 
 RestartButton {
     width: 14;
 }
@@ -87,11 +91,14 @@
 
 HeaderClock {
     height: 3;
     background: transparent;
 }
 
 .container-name {
-    overflow-x: hidden;
-    max-width: 100%;
+    width: 1fr;
     height: 1;
 }
+
+.bold {
+    text-style: bold;
+}
```

### Comparing `dockery-0.7.0/src/dockery/utils.py` & `dockery-0.8.0/src/dockery/utils.py`

 * *Files identical despite different names*

### Comparing `dockery-0.7.0/src/dockery/volumes.py` & `dockery-0.8.0/src/dockery/volumes.py`

 * *Files 5% similar despite different names*

```diff
@@ -11,31 +11,38 @@
 
 class VolumesList(ResponsiveGrid):
     volumes_count = reactive(0)
 
     def __init__(self, docker: DockerClient, **kargs):
         self.volumes: list[Volume] = []
         self.docker = docker
+        
         super().__init__(**kargs)
 
     def on_mount(self) -> None:
         self.get_volumes()
-        self.set_interval(2, self.get_volumes)
+        self.get_volumes_timer = self.set_interval(2, self.get_volumes, pause=True)
 
     async def watch_volumes_count(self, count: int) -> None:
         await self.grid.remove_children()
         for c in self.volumes:
             cw = VolumeWidget(c, self.docker, classes="li")
             self.grid.mount(cw)
 
     @daemon
     def get_volumes(self) -> None:
         self.volumes = self.docker.volumes.list()  # type: ignore
         self.volumes_count = len(self.volumes)
 
+    def on_hide(self):
+        self.get_volumes_timer.pause()
+
+    def on_show(self):
+        self.get_volumes_timer.resume()
+
 
 class VolumeWidget(Static):
     def __init__(self, volume: Volume, client: DockerClient, **kargs):
         self.volume = volume
         self.client = client
         self.attrs = volume.attrs or {}
         self.isize = self.attrs.get("Size", 0) / 1000 / 1000
```

### Comparing `dockery-0.7.0/PKG-INFO` & `dockery-0.8.0/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 00000000: 4d65 7461 6461 7461 2d56 6572 7369 6f6e  Metadata-Version
 00000010: 3a20 322e 310a 4e61 6d65 3a20 646f 636b  : 2.1.Name: dock
-00000020: 6572 790a 5665 7273 696f 6e3a 2030 2e37  ery.Version: 0.7
+00000020: 6572 790a 5665 7273 696f 6e3a 2030 2e38  ery.Version: 0.8
 00000030: 2e30 0a53 756d 6d61 7279 3a20 4772 6170  .0.Summary: Grap
 00000040: 6869 6361 6c20 696e 7465 7266 6163 6520  hical interface 
 00000050: 666f 7220 446f 636b 6572 2069 6e20 796f  for Docker in yo
 00000060: 7572 2063 6f6e 736f 6c65 0a41 7574 686f  ur console.Autho
 00000070: 722d 456d 6169 6c3a 204d 6172 6961 6e6f  r-Email: Mariano
 00000080: 2043 6172 7261 7a61 6e61 203c 6d61 7269   Carrazana <mari
 00000090: 616e 6f63 6172 7261 7a61 6e61 4067 6d61  anocarrazana@gma
@@ -40,96 +40,86 @@
 00000270: 7469 6f6e 732f 776f 726b 666c 6f77 732f  tions/workflows/
 00000280: 7265 6c65 6173 652e 796d 6c2f 6261 6467  release.yml/badg
 00000290: 652e 7376 6729 5d28 6874 7470 733a 2f2f  e.svg)](https://
 000002a0: 6769 7468 7562 2e63 6f6d 2f6d 6172 6961  github.com/maria
 000002b0: 6e6f 6361 7272 617a 616e 612f 646f 636b  nocarrazana/dock
 000002c0: 6572 792f 6163 7469 6f6e 732f 776f 726b  ery/actions/work
 000002d0: 666c 6f77 732f 7265 6c65 6173 652e 796d  flows/release.ym
-000002e0: 6c29 0a0a 3c74 6162 6c65 3e0a 2020 3c74  l)..<table>.  <t
-000002f0: 723e 0a20 2020 203c 7464 3e3c 696d 6720  r>.    <td><img 
-00000300: 7372 633d 2268 7474 7073 3a2f 2f67 6974  src="https://git
-00000310: 6875 622e 636f 6d2f 6d61 7269 616e 6f63  hub.com/marianoc
-00000320: 6172 7261 7a61 6e61 2f64 6f63 6b65 7279  arrazana/dockery
-00000330: 2f61 7373 6574 732f 3137 3233 3830 3736  /assets/17238076
-00000340: 2f62 6366 6632 3263 392d 3839 3863 2d34  /bcff22c9-898c-4
-00000350: 3837 372d 6164 6163 2d64 6466 3265 3538  877-adac-ddf2e58
-00000360: 3030 3763 3422 2f3e 3c2f 7464 3e0a 2020  007c4"/></td>.  
-00000370: 2020 3c74 643e 3c69 6d67 2073 7263 3d22    <td><img src="
-00000380: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
-00000390: 6f6d 2f6d 6172 6961 6e6f 6361 7272 617a  om/marianocarraz
-000003a0: 616e 612f 646f 636b 6572 792f 6173 7365  ana/dockery/asse
-000003b0: 7473 2f31 3732 3338 3037 362f 3064 6130  ts/17238076/0da0
-000003c0: 6331 3363 2d64 3834 642d 3465 3861 2d38  c13c-d84d-4e8a-8
-000003d0: 6236 662d 6130 6437 3739 6332 6439 3864  b6f-a0d779c2d98d
-000003e0: 222f 3e3c 2f74 643e 0a20 203c 2f74 723e  "/></td>.  </tr>
-000003f0: 0a20 203c 7472 3e0a 2020 2020 3c74 6420  .  <tr>.    <td 
-00000400: 636f 6c73 7061 6e3d 2232 223e 3c69 6d67  colspan="2"><img
-00000410: 2073 7263 3d22 6874 7470 733a 2f2f 6769   src="https://gi
-00000420: 7468 7562 2e63 6f6d 2f6d 6172 6961 6e6f  thub.com/mariano
-00000430: 6361 7272 617a 616e 612f 646f 636b 6572  carrazana/docker
-00000440: 792f 6173 7365 7473 2f31 3732 3338 3037  y/assets/1723807
-00000450: 362f 6339 3931 6666 3462 2d65 6562 662d  6/c991ff4b-eebf-
-00000460: 3434 3935 2d62 3637 632d 3263 3537 6539  4495-b67c-2c57e9
-00000470: 3333 6264 3764 2220 2f3e 3c2f 7464 3e0a  33bd7d" /></td>.
-00000480: 2020 3c2f 7472 3e0a 3c2f 7461 626c 653e    </tr>.</table>
-00000490: 0a0a 2323 2049 6e73 7461 6c6c 6174 696f  ..## Installatio
-000004a0: 6e0a 0a23 2323 2046 726f 6d20 736f 7572  n..### From sour
-000004b0: 6365 0a0a 6060 6073 6865 6c6c 0a67 6974  ce..```shell.git
-000004c0: 2063 6c6f 6e65 2068 7474 7073 3a2f 2f67   clone https://g
-000004d0: 6974 6875 622e 636f 6d2f 6d61 7269 616e  ithub.com/marian
-000004e0: 6f63 6172 7261 7a61 6e61 2f64 6f63 6b65  ocarrazana/docke
-000004f0: 7279 2e67 6974 0a63 6420 646f 636b 6572  ry.git.cd docker
-00000500: 790a 7069 7020 696e 7374 616c 6c20 2d65  y.pip install -e
-00000510: 202e 0a23 2075 7064 6174 6520 6f6e 6c79   ..# update only
-00000520: 3a0a 6769 7420 7075 6c6c 0a60 6060 0a0a  :.git pull.```..
-00000530: 2323 2320 4672 6f6d 2070 6970 0a0a 6060  ### From pip..``
-00000540: 6073 6865 6c6c 0a70 6970 2069 6e73 7461  `shell.pip insta
-00000550: 6c6c 202d 5520 646f 636b 6572 790a 6060  ll -U dockery.``
-00000560: 600a 0a23 2320 5573 6167 650a 0a52 756e  `..## Usage..Run
-00000570: 206f 6e20 796f 7572 2063 6f6e 736f 6c65   on your console
-00000580: 3a0a 0a60 6060 7368 656c 6c0a 646f 636b  :..```shell.dock
-00000590: 6572 790a 6060 600a 0a2a 2a57 6172 6e69  ery.```..**Warni
-000005a0: 6e67 3a2a 2a20 796f 7520 7769 6c6c 2070  ng:** you will p
-000005b0: 726f 6261 626c 7920 6e65 6564 2074 6f20  robably need to 
-000005c0: 696e 7374 616c 6c20 616e 6420 7275 6e20  install and run 
-000005d0: 646f 636b 6572 7920 6173 2061 2072 6f6f  dockery as a roo
-000005e0: 7420 7573 6572 2c20 6f72 2079 6f75 2063  t user, or you c
-000005f0: 616e 2061 6464 2070 6572 6d69 7373 696f  an add permissio
-00000600: 6e73 2074 6f20 796f 7572 2075 7365 7220  ns to your user 
-00000610: 746f 2072 756e 2064 6f63 6b65 7220 666f  to run docker fo
-00000620: 6c6c 6f77 696e 6720 5b74 6869 7320 696e  llowing [this in
-00000630: 7374 7275 6374 696f 6e73 5d28 6874 7470  structions](http
-00000640: 733a 2f2f 646f 6373 2e64 6f63 6b65 722e  s://docs.docker.
-00000650: 636f 6d2f 656e 6769 6e65 2f69 6e73 7461  com/engine/insta
-00000660: 6c6c 2f6c 696e 7578 2d70 6f73 7469 6e73  ll/linux-postins
-00000670: 7461 6c6c 2f23 6d61 6e61 6765 2d64 6f63  tall/#manage-doc
-00000680: 6b65 722d 6173 2d61 2d6e 6f6e 2d72 6f6f  ker-as-a-non-roo
-00000690: 742d 7573 6572 292e 0a0a 2323 2055 7469  t-user)...## Uti
-000006a0: 6c73 0a0a 6060 6073 6865 6c6c 0a64 6f63  ls..```shell.doc
-000006b0: 6b65 7279 2064 660a 646f 636b 6572 7920  kery df.dockery 
-000006c0: 7073 0a64 6f63 6b65 7279 2076 6f6c 756d  ps.dockery volum
-000006d0: 6573 0a64 6f63 6b65 7279 2069 6d61 6765  es.dockery image
-000006e0: 730a 646f 636b 6572 7920 6e65 7477 6f72  s.dockery networ
-000006f0: 6b73 0a64 6f63 6b65 7279 2073 7461 7473  ks.dockery stats
-00000700: 0a60 6060 0a0a 596f 7520 7370 6563 6966  .```..You specif
-00000710: 7920 7468 6520 666f 726d 6174 206f 7574  y the format out
-00000720: 7075 7420 6f66 2074 6865 7365 2063 6f6d  put of these com
-00000730: 6d61 6e64 7320 7769 7468 2074 6865 2070  mands with the p
-00000740: 6172 616d 6574 6572 2060 2d2d 666f 726d  arameter `--form
-00000750: 6174 602c 2065 2e67 3a0a 0a60 6060 7368  at`, e.g:..```sh
-00000760: 656c 6c0a 646f 636b 6572 7920 6466 202d  ell.dockery df -
-00000770: 2d66 6f72 6d61 7420 6a73 6f6e 0a64 6f63  -format json.doc
-00000780: 6b65 7279 2064 6620 2d2d 666f 726d 6174  kery df --format
-00000790: 2079 616d 6c0a 6060 600a 0a23 2323 2047   yaml.```..### G
-000007a0: 6574 206c 6f67 730a 0a60 6060 7368 656c  et logs..```shel
-000007b0: 0a64 6f63 6b65 7279 206c 6f67 7320 7b63  .dockery logs {c
-000007c0: 6f6e 7461 696e 6572 5f6e 616d 657d 0a60  ontainer_name}.`
-000007d0: 6060 0a0a 596f 7520 6361 6e20 7573 6520  ``..You can use 
-000007e0: 7468 6520 7061 7261 6d65 7465 7220 602d  the parameter `-
-000007f0: 2d73 7472 6561 6d60 2074 6f20 6765 7420  -stream` to get 
-00000800: 7468 6520 6c6f 6773 2069 6e20 7265 616c  the logs in real
-00000810: 2074 696d 652c 2065 2e67 3a0a 0a60 6060   time, e.g:..```
-00000820: 7368 656c 0a64 6f63 6b65 7279 206c 6f67  shel.dockery log
-00000830: 7320 7b63 6f6e 7461 696e 6572 5f6e 616d  s {container_nam
-00000840: 657d 202d 2d73 7472 6561 6d0a 6060 600a  e} --stream.```.
-00000850: 0a23 2323 202a 2a45 6e6a 6f79 2069 7421  .### **Enjoy it!
-00000860: 2a2a 0a                                  **.
+000002e0: 6c29 0a0a 215b 7363 7265 656e 7368 6f74  l)..![screenshot
+000002f0: 315d 2868 7474 7073 3a2f 2f67 6974 6875  1](https://githu
+00000300: 622e 636f 6d2f 6d61 7269 616e 6f63 6172  b.com/marianocar
+00000310: 7261 7a61 6e61 2f64 6f63 6b65 7279 2f61  razana/dockery/a
+00000320: 7373 6574 732f 3137 3233 3830 3736 2f32  ssets/17238076/2
+00000330: 6337 6561 6438 372d 6564 6532 2d34 3833  c7ead87-ede2-483
+00000340: 342d 3837 6536 2d38 3535 3637 3430 6333  4-87e6-8556740c3
+00000350: 3062 6429 0a0a 2323 2049 6e73 7461 6c6c  0bd)..## Install
+00000360: 6174 696f 6e0a 0a23 2323 2046 726f 6d20  ation..### From 
+00000370: 7069 700a 0a60 6060 7368 656c 6c0a 7069  pip..```shell.pi
+00000380: 7020 696e 7374 616c 6c20 2d55 2064 6f63  p install -U doc
+00000390: 6b65 7279 0a60 6060 0a0a 2323 2320 4672  kery.```..### Fr
+000003a0: 6f6d 2073 6f75 7263 650a 0a60 6060 7368  om source..```sh
+000003b0: 656c 6c0a 6769 7420 636c 6f6e 6520 6874  ell.git clone ht
+000003c0: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
+000003d0: 2f6d 6172 6961 6e6f 6361 7272 617a 616e  /marianocarrazan
+000003e0: 612f 646f 636b 6572 792e 6769 740a 6364  a/dockery.git.cd
+000003f0: 2064 6f63 6b65 7279 0a70 6970 2069 6e73   dockery.pip ins
+00000400: 7461 6c6c 202d 6520 2e0a 2320 7570 6461  tall -e ..# upda
+00000410: 7465 206f 6e6c 793a 0a67 6974 2070 756c  te only:.git pul
+00000420: 6c0a 6060 600a 0a23 2320 5573 6167 650a  l.```..## Usage.
+00000430: 0a52 756e 206f 6e20 796f 7572 2063 6f6e  .Run on your con
+00000440: 736f 6c65 3a0a 0a60 6060 7368 656c 6c0a  sole:..```shell.
+00000450: 646f 636b 6572 790a 6060 600a 0a2a 2a57  dockery.```..**W
+00000460: 6172 6e69 6e67 3a2a 2a20 796f 7520 7769  arning:** you wi
+00000470: 6c6c 2070 726f 6261 626c 7920 6e65 6564  ll probably need
+00000480: 2074 6f20 696e 7374 616c 6c20 616e 6420   to install and 
+00000490: 7275 6e20 646f 636b 6572 7920 6173 2061  run dockery as a
+000004a0: 2072 6f6f 7420 7573 6572 2c20 6f72 2079   root user, or y
+000004b0: 6f75 2063 616e 2061 6464 2070 6572 6d69  ou can add permi
+000004c0: 7373 696f 6e73 2074 6f20 796f 7572 2075  ssions to your u
+000004d0: 7365 7220 746f 2072 756e 2064 6f63 6b65  ser to run docke
+000004e0: 7220 666f 6c6c 6f77 696e 6720 5b74 6869  r following [thi
+000004f0: 7320 696e 7374 7275 6374 696f 6e73 5d28  s instructions](
+00000500: 6874 7470 733a 2f2f 646f 6373 2e64 6f63  https://docs.doc
+00000510: 6b65 722e 636f 6d2f 656e 6769 6e65 2f69  ker.com/engine/i
+00000520: 6e73 7461 6c6c 2f6c 696e 7578 2d70 6f73  nstall/linux-pos
+00000530: 7469 6e73 7461 6c6c 2f23 6d61 6e61 6765  tinstall/#manage
+00000540: 2d64 6f63 6b65 722d 6173 2d61 2d6e 6f6e  -docker-as-a-non
+00000550: 2d72 6f6f 742d 7573 6572 292e 0a0a 2323  -root-user)...##
+00000560: 2055 7469 6c73 0a0a 6060 6073 6865 6c6c   Utils..```shell
+00000570: 0a64 6f63 6b65 7279 2064 660a 646f 636b  .dockery df.dock
+00000580: 6572 7920 7073 0a64 6f63 6b65 7279 2076  ery ps.dockery v
+00000590: 6f6c 756d 6573 0a64 6f63 6b65 7279 2069  olumes.dockery i
+000005a0: 6d61 6765 730a 646f 636b 6572 7920 6e65  mages.dockery ne
+000005b0: 7477 6f72 6b73 0a64 6f63 6b65 7279 2073  tworks.dockery s
+000005c0: 7461 7473 0a23 2044 6f63 6b65 7220 7377  tats.# Docker sw
+000005d0: 6172 6d0a 646f 636b 6572 7920 636f 6e66  arm.dockery conf
+000005e0: 6967 730a 646f 636b 6572 7920 7365 6372  igs.dockery secr
+000005f0: 6574 730a 6060 600a 0a59 6f75 2073 7065  ets.```..You spe
+00000600: 6369 6679 2074 6865 2066 6f72 6d61 7420  cify the format 
+00000610: 6f75 7470 7574 206f 6620 7468 6573 6520  output of these 
+00000620: 636f 6d6d 616e 6473 2077 6974 6820 7468  commands with th
+00000630: 6520 7061 7261 6d65 7465 7220 602d 2d66  e parameter `--f
+00000640: 6f72 6d61 7460 2c20 652e 673a 0a0a 6060  ormat`, e.g:..``
+00000650: 6073 6865 6c6c 0a64 6f63 6b65 7279 2064  `shell.dockery d
+00000660: 6620 2d2d 666f 726d 6174 206a 736f 6e0a  f --format json.
+00000670: 646f 636b 6572 7920 6466 202d 2d66 6f72  dockery df --for
+00000680: 6d61 7420 7961 6d6c 0a60 6060 0a0a 2323  mat yaml.```..##
+00000690: 2320 4765 7420 6c6f 6773 0a0a 596f 7520  # Get logs..You 
+000006a0: 6361 6e20 7573 6520 60ce 9e4c 6f67 7360  can use `..Logs`
+000006b0: 2062 7574 746f 6e20 6f6e 2074 6865 2063   button on the c
+000006c0: 6f6e 7461 696e 6572 7320 7461 6273 2074  ontainers tabs t
+000006d0: 6f20 7365 6520 7468 6520 6c6f 6773 2e0a  o see the logs..
+000006e0: 0a4f 7220 796f 7520 6361 6e20 7573 6520  .Or you can use 
+000006f0: 7468 6520 6c6f 6773 2063 6f6d 6d61 6e64  the logs command
+00000700: 2074 6f20 7669 7375 616c 697a 6520 7468   to visualize th
+00000710: 656d 3a0a 0a60 6060 7368 656c 6c0a 646f  em:..```shell.do
+00000720: 636b 6572 7920 6c6f 6773 207b 636f 6e74  ckery logs {cont
+00000730: 6169 6e65 725f 6e61 6d65 7d0a 6060 600a  ainer_name}.```.
+00000740: 0a59 6f75 2063 616e 2075 7365 2074 6865  .You can use the
+00000750: 2070 6172 616d 6574 6572 2060 2d2d 7374   parameter `--st
+00000760: 7265 616d 6020 746f 2067 6574 2074 6865  ream` to get the
+00000770: 206c 6f67 7320 696e 2072 6561 6c20 7469   logs in real ti
+00000780: 6d65 2c20 652e 673a 0a0a 6060 6073 6865  me, e.g:..```she
+00000790: 6c0a 646f 636b 6572 7920 6c6f 6773 207b  l.dockery logs {
+000007a0: 636f 6e74 6169 6e65 725f 6e61 6d65 7d20  container_name} 
+000007b0: 2d2d 7374 7265 616d 0a60 6060 0a0a 2323  --stream.```..##
+000007c0: 2320 2a2a 456e 6a6f 7920 6974 212a 2a0a  # **Enjoy it!**.
```

