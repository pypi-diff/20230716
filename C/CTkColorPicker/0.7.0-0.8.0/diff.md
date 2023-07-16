# Comparing `tmp/CTkColorPicker-0.7.0.tar.gz` & `tmp/CTkColorPicker-0.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "CTkColorPicker-0.7.0.tar", last modified: Mon Jul 10 07:06:09 2023, max compression
+gzip compressed data, was "CTkColorPicker-0.8.0.tar", last modified: Sun Jul 16 15:31:23 2023, max compression
```

## Comparing `CTkColorPicker-0.7.0.tar` & `CTkColorPicker-0.8.0.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-07-10 07:06:09.873749 CTkColorPicker-0.7.0/
-drwxrwxrwx   0        0        0        0 2023-07-10 07:06:09.853856 CTkColorPicker-0.7.0/CTkColorPicker/
--rw-rw-rw-   0        0        0      272 2023-07-10 07:04:41.000000 CTkColorPicker-0.7.0/CTkColorPicker/__init__.py
--rw-rw-rw-   0        0        0   111614 2020-05-30 05:51:52.000000 CTkColorPicker-0.7.0/CTkColorPicker/color_wheel.png
--rw-rw-rw-   0        0        0     9267 2023-07-10 07:02:57.000000 CTkColorPicker-0.7.0/CTkColorPicker/ctk_color_picker.py
--rw-rw-rw-   0        0        0     7220 2023-07-10 07:01:48.000000 CTkColorPicker-0.7.0/CTkColorPicker/ctk_color_picker_widget.py
--rw-rw-rw-   0        0        0      933 2020-05-30 05:51:52.000000 CTkColorPicker-0.7.0/CTkColorPicker/target.png
-drwxrwxrwx   0        0        0        0 2023-07-10 07:06:09.863804 CTkColorPicker-0.7.0/CTkColorPicker.egg-info/
--rw-rw-rw-   0        0        0     3653 2023-07-10 07:06:09.000000 CTkColorPicker-0.7.0/CTkColorPicker.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      386 2023-07-10 07:06:09.000000 CTkColorPicker-0.7.0/CTkColorPicker.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0       73 2023-07-10 07:06:09.000000 CTkColorPicker-0.7.0/CTkColorPicker.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       21 2023-07-10 07:06:09.000000 CTkColorPicker-0.7.0/CTkColorPicker.egg-info/requires.txt
--rw-rw-rw-   0        0        0       15 2023-07-10 07:06:09.000000 CTkColorPicker-0.7.0/CTkColorPicker.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     7048 2022-11-20 16:16:56.000000 CTkColorPicker-0.7.0/LICENSE
--rw-rw-rw-   0        0        0     3653 2023-07-10 07:06:09.873749 CTkColorPicker-0.7.0/PKG-INFO
--rw-rw-rw-   0        0        0     2974 2023-05-17 13:55:59.000000 CTkColorPicker-0.7.0/README.md
--rw-rw-rw-   0        0        0      607 2023-07-10 07:06:09.873749 CTkColorPicker-0.7.0/setup.cfg
--rw-rw-rw-   0        0        0     1317 2023-07-10 07:05:39.000000 CTkColorPicker-0.7.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-16 15:31:23.599977 CTkColorPicker-0.8.0/
+drwxrwxrwx   0        0        0        0 2023-07-16 15:31:23.571136 CTkColorPicker-0.8.0/CTkColorPicker/
+-rw-rw-rw-   0        0        0      272 2023-07-16 15:29:32.000000 CTkColorPicker-0.8.0/CTkColorPicker/__init__.py
+-rw-rw-rw-   0        0        0   111614 2020-05-30 05:51:52.000000 CTkColorPicker-0.8.0/CTkColorPicker/color_wheel.png
+-rw-rw-rw-   0        0        0     9267 2023-07-10 07:02:57.000000 CTkColorPicker-0.8.0/CTkColorPicker/ctk_color_picker.py
+-rw-rw-rw-   0        0        0     7597 2023-07-16 15:30:01.000000 CTkColorPicker-0.8.0/CTkColorPicker/ctk_color_picker_widget.py
+-rw-rw-rw-   0        0        0      933 2020-05-30 05:51:52.000000 CTkColorPicker-0.8.0/CTkColorPicker/target.png
+drwxrwxrwx   0        0        0        0 2023-07-16 15:31:23.595970 CTkColorPicker-0.8.0/CTkColorPicker.egg-info/
+-rw-rw-rw-   0        0        0     3711 2023-07-16 15:31:23.000000 CTkColorPicker-0.8.0/CTkColorPicker.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      386 2023-07-16 15:31:23.000000 CTkColorPicker-0.8.0/CTkColorPicker.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0       73 2023-07-16 15:31:23.000000 CTkColorPicker-0.8.0/CTkColorPicker.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       21 2023-07-16 15:31:23.000000 CTkColorPicker-0.8.0/CTkColorPicker.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2023-07-16 15:31:23.000000 CTkColorPicker-0.8.0/CTkColorPicker.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     7048 2022-11-20 16:16:56.000000 CTkColorPicker-0.8.0/LICENSE
+-rw-rw-rw-   0        0        0     3711 2023-07-16 15:31:23.599977 CTkColorPicker-0.8.0/PKG-INFO
+-rw-rw-rw-   0        0        0     3032 2023-07-16 15:30:38.000000 CTkColorPicker-0.8.0/README.md
+-rw-rw-rw-   0        0        0      607 2023-07-16 15:31:23.599977 CTkColorPicker-0.8.0/setup.cfg
+-rw-rw-rw-   0        0        0     1317 2023-07-16 15:29:49.000000 CTkColorPicker-0.8.0/setup.py
```

### Comparing `CTkColorPicker-0.7.0/CTkColorPicker/color_wheel.png` & `CTkColorPicker-0.8.0/CTkColorPicker/color_wheel.png`

 * *Files identical despite different names*

### Comparing `CTkColorPicker-0.7.0/CTkColorPicker/ctk_color_picker.py` & `CTkColorPicker-0.8.0/CTkColorPicker/ctk_color_picker.py`

 * *Files identical despite different names*

### Comparing `CTkColorPicker-0.7.0/CTkColorPicker/ctk_color_picker_widget.py` & `CTkColorPicker-0.8.0/CTkColorPicker/ctk_color_picker_widget.py`

 * *Files 4% similar despite different names*

```diff
@@ -23,14 +23,15 @@
                  master: any = None,
                  width: int = 300,
                  initial_color: str = None,
                  fg_color: str = None,
                  slider_border: int = 1,
                  corner_radius: int = 24,
                  command = None,
+                 orientation = "vertical",
                  **slider_kwargs):
     
         super().__init__(master=master, corner_radius=corner_radius)
         
         WIDTH = width if width>=200 else 200
         HEIGHT = WIDTH + 150
         self.image_dimension = WIDTH - 100
@@ -47,15 +48,14 @@
         self.command = command
             
         self.slider_border = 10 if slider_border>=10 else slider_border
         
         self.configure(fg_color=self.fg_color)
           
         self.canvas = tkinter.Canvas(self, height=self.image_dimension, width=self.image_dimension, highlightthickness=0, bg=self.fg_color)
-        self.canvas.pack(pady=20, side="left", padx=(10,0))
         self.canvas.bind("<B1-Motion>", self.on_mouse_drag)
 
         self.img1 = Image.open(os.path.join(PATH, 'color_wheel.png')).resize((self.image_dimension, self.image_dimension), Image.Resampling.LANCZOS)
         self.img2 = Image.open(os.path.join(PATH, 'target.png')).resize((20, 20), Image.Resampling.LANCZOS)
 
         self.wheel = ImageTk.PhotoImage(self.img1)
         self.target = ImageTk.PhotoImage(self.img2)
@@ -66,21 +66,28 @@
         self.brightness_slider_value = customtkinter.IntVar()
         self.brightness_slider_value.set(255)
         
         self.slider = customtkinter.CTkSlider(master=self, width=20, border_width=self.slider_border,
                                               button_length=15, progress_color=self.default_hex_color, from_=0, to=255,
                                               variable=self.brightness_slider_value, number_of_steps=256,
                                               button_corner_radius=self.corner_radius, corner_radius=self.corner_radius,
-                                              command=lambda x:self.update_colors(), orientation="vertical", **slider_kwargs)
-        self.slider.pack(fill="y", pady=15, side="right", padx=(0,10-self.slider_border))
-
+                                              command=lambda x:self.update_colors(), orientation=orientation, **slider_kwargs)
+        
         self.label = customtkinter.CTkLabel(master=self, text_color="#000000", width=10, fg_color=self.default_hex_color,
                                             corner_radius=self.corner_radius, text=self.default_hex_color, wraplength=1)
-        self.label.pack(expand=True, fill="both", padx=10, pady=15)
-        
+        if orientation=="vertical":
+            self.canvas.pack(pady=20, side="left", padx=(10,0))
+            self.slider.pack(fill="y", pady=15, side="right", padx=(0,10-self.slider_border))
+            self.label.pack(expand=True, fill="both", padx=10, pady=15)
+        else:
+            self.label.configure(wraplength=100)
+            self.canvas.pack(pady=15, padx=15)
+            self.slider.pack(fill="x", pady=(0,10-self.slider_border), padx=15)
+            self.label.pack(expand=True, fill="both", padx=15, pady=(0,15))
+            
     def get(self):
         self._color = self.label._fg_color
         return self._color
     
     def destroy(self):
         super().destroy()
         del self.img1
```

### Comparing `CTkColorPicker-0.7.0/CTkColorPicker/target.png` & `CTkColorPicker-0.8.0/CTkColorPicker/target.png`

 * *Files identical despite different names*

### Comparing `CTkColorPicker-0.7.0/CTkColorPicker.egg-info/PKG-INFO` & `CTkColorPicker-0.8.0/CTkColorPicker.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: CTkColorPicker
-Version: 0.7.0
+Version: 0.8.0
 Summary: A modern color picker for customtkinter
 Home-page: https://github.com/Akascape/CTkColorPicker
 Author: Akash Bora
 License: Creative Commons Zero v1.0 Universal
 Keywords: customtkinter,customtkinter-dialog,customtkinter-color-picker,customtkinter-colour-picker,customtkinter-color,customtkinter-color-chooser,color-picker,python-color-picker
 Classifier: License :: CC0 1.0 Universal (CC0 1.0) Public Domain Dedication
 Classifier: Programming Language :: Python :: 3
@@ -84,10 +84,11 @@
 | master | parent widget |
 | width | set the overall size of the color picker frame |
 | fg_color | change forground color of the color picker frame |
 | initial_color | set the default color of color picker (currently in beta stage) |
 | slider_border | change the border width of slider |
 | corner_radius | change the corner radius of all the widgets inside color picker |
 | command | add a command when the color is changed |
+| orientation | change orientation of slider and label |
 | _**other slider parameters_ | pass other slider arguments if required |
 
 **That's all, hope it will help!**
```

### Comparing `CTkColorPicker-0.7.0/LICENSE` & `CTkColorPicker-0.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `CTkColorPicker-0.7.0/PKG-INFO` & `CTkColorPicker-0.8.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: CTkColorPicker
-Version: 0.7.0
+Version: 0.8.0
 Summary: A modern color picker for customtkinter
 Home-page: https://github.com/Akascape/CTkColorPicker
 Author: Akash Bora
 License: Creative Commons Zero v1.0 Universal
 Keywords: customtkinter,customtkinter-dialog,customtkinter-color-picker,customtkinter-colour-picker,customtkinter-color,customtkinter-color-chooser,color-picker,python-color-picker
 Classifier: License :: CC0 1.0 Universal (CC0 1.0) Public Domain Dedication
 Classifier: Programming Language :: Python :: 3
@@ -84,10 +84,11 @@
 | master | parent widget |
 | width | set the overall size of the color picker frame |
 | fg_color | change forground color of the color picker frame |
 | initial_color | set the default color of color picker (currently in beta stage) |
 | slider_border | change the border width of slider |
 | corner_radius | change the corner radius of all the widgets inside color picker |
 | command | add a command when the color is changed |
+| orientation | change orientation of slider and label |
 | _**other slider parameters_ | pass other slider arguments if required |
 
 **That's all, hope it will help!**
```

### Comparing `CTkColorPicker-0.7.0/README.md` & `CTkColorPicker-0.8.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -69,10 +69,11 @@
 | master | parent widget |
 | width | set the overall size of the color picker frame |
 | fg_color | change forground color of the color picker frame |
 | initial_color | set the default color of color picker (currently in beta stage) |
 | slider_border | change the border width of slider |
 | corner_radius | change the corner radius of all the widgets inside color picker |
 | command | add a command when the color is changed |
+| orientation | change orientation of slider and label |
 | _**other slider parameters_ | pass other slider arguments if required |
 
 **That's all, hope it will help!**
```

### Comparing `CTkColorPicker-0.7.0/setup.cfg` & `CTkColorPicker-0.8.0/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2043 546b 436f 6c6f 7250 6963 6b65   = CTkColorPicke
-00000020: 720d 0a76 6572 7369 6f6e 203d 2030 2e37  r..version = 0.7
+00000020: 720d 0a76 6572 7369 6f6e 203d 2030 2e38  r..version = 0.8
 00000030: 2e30 0d0a 6465 7363 7269 7074 696f 6e20  .0..description 
 00000040: 3d20 4120 6d6f 6465 726e 2063 6f6c 6f72  = A modern color
 00000050: 2070 6963 6b65 7220 666f 7220 6375 7374   picker for cust
 00000060: 6f6d 746b 696e 7465 720d 0a6c 6f6e 675f  omtkinter..long_
 00000070: 6465 7363 7269 7074 696f 6e20 3d20 6669  description = fi
 00000080: 6c65 3a20 5245 4144 4d45 2e6d 640d 0a6c  le: README.md..l
 00000090: 6f6e 675f 6465 7363 7269 7074 696f 6e5f  ong_description_
```

### Comparing `CTkColorPicker-0.7.0/setup.py` & `CTkColorPicker-0.8.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
     """Opens and fetches text of long descrition file."""
     with open(path, 'r') as f:
         text = f.read()
     return text
 
 setup(
     name = 'CTkColorPicker',
-    version = '0.7.0',
+    version = '0.8.0',
     description = "A modern color picker for customtkinter",
     license = "Creative Commons Zero v1.0 Universal",
     readme = "README.md",
     long_description = get_long_description('README.md'),
     long_description_content_type = "text/markdown",
     author = 'Akash Bora',
     url = "https://github.com/Akascape/CTkColorPicker",
```

