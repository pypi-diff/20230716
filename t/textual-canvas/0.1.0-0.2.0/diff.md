# Comparing `tmp/textual_canvas-0.1.0-py3-none-any.whl.zip` & `tmp/textual_canvas-0.2.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,10 +1,10 @@
-Zip file size: 8344 bytes, number of entries: 8
--rw-r--r--  2.0 unx      701 b- defN 23-Apr-01 19:41 textual_canvas/__init__.py
--rw-r--r--  2.0 unx     1766 b- defN 23-Apr-01 19:31 textual_canvas/__main__.py
--rw-r--r--  2.0 unx    12261 b- defN 23-Apr-01 19:41 textual_canvas/canvas.py
+Zip file size: 8667 bytes, number of entries: 8
+-rw-r--r--  2.0 unx      678 b- defN 23-Jul-16 07:43 textual_canvas/__init__.py
+-rw-r--r--  2.0 unx     2138 b- defN 23-Jul-16 07:43 textual_canvas/__main__.py
+-rw-r--r--  2.0 unx    12931 b- defN 23-Jul-16 07:43 textual_canvas/canvas.py
 -rw-r--r--  2.0 unx        0 b- defN 23-Mar-27 18:46 textual_canvas/py.typed
--rw-r--r--  2.0 unx     6551 b- defN 23-Apr-01 19:41 textual_canvas-0.1.0.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Apr-01 19:41 textual_canvas-0.1.0.dist-info/WHEEL
--rw-r--r--  2.0 unx       15 b- defN 23-Apr-01 19:41 textual_canvas-0.1.0.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      650 b- defN 23-Apr-01 19:41 textual_canvas-0.1.0.dist-info/RECORD
-8 files, 22036 bytes uncompressed, 7204 bytes compressed:  67.3%
+-rw-r--r--  2.0 unx     6555 b- defN 23-Jul-16 07:45 textual_canvas-0.2.0.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jul-16 07:45 textual_canvas-0.2.0.dist-info/WHEEL
+-rw-r--r--  2.0 unx       15 b- defN 23-Jul-16 07:45 textual_canvas-0.2.0.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      650 b- defN 23-Jul-16 07:45 textual_canvas-0.2.0.dist-info/RECORD
+8 files, 23059 bytes uncompressed, 7527 bytes compressed:  67.4%
```

## zipnote {}

```diff
@@ -6,20 +6,20 @@
 
 Filename: textual_canvas/canvas.py
 Comment: 
 
 Filename: textual_canvas/py.typed
 Comment: 
 
-Filename: textual_canvas-0.1.0.dist-info/METADATA
+Filename: textual_canvas-0.2.0.dist-info/METADATA
 Comment: 
 
-Filename: textual_canvas-0.1.0.dist-info/WHEEL
+Filename: textual_canvas-0.2.0.dist-info/WHEEL
 Comment: 
 
-Filename: textual_canvas-0.1.0.dist-info/top_level.txt
+Filename: textual_canvas-0.2.0.dist-info/top_level.txt
 Comment: 
 
-Filename: textual_canvas-0.1.0.dist-info/RECORD
+Filename: textual_canvas-0.2.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## textual_canvas/__init__.py

```diff
@@ -1,21 +1,21 @@
 """A library that provides a simple canvas for drawing in Textual."""
 
 ######################################################################
 # Main app information.
-__author__     = "Dave Pearson"
-__copyright__  = "Copyright 2023, Dave Pearson"
-__credits__    = [ "Dave Pearson" ]
+__author__ = "Dave Pearson"
+__copyright__ = "Copyright 2023, Dave Pearson"
+__credits__ = ["Dave Pearson"]
 __maintainer__ = "Dave Pearson"
-__email__      = "davep@davep.org"
-__version__    = "0.1.0"
-__licence__    = "MIT"
+__email__ = "davep@davep.org"
+__version__ = "0.2.0"
+__licence__ = "MIT"
 
 ##############################################################################
 # Local imports.
 from .canvas import Canvas, CanvasError
 
 ##############################################################################
 # Export the imports.
-__all__ = [ "Canvas", "CanvasError" ]
+__all__ = ["Canvas", "CanvasError"]
 
 ### __init__.py ends here
```

## textual_canvas/__main__.py

```diff
@@ -1,51 +1,69 @@
 """A simple demonstration of the Canvas widget."""
 
 ##############################################################################
 # Textual imports.
-from textual.app   import App, ComposeResult
+from textual import on
+from textual.app import App, ComposeResult
+from textual.events import Mount
 from textual.color import Color
 
 ##############################################################################
 # Local imports.
 from .canvas import Canvas
 
+
 ##############################################################################
-class CanvasTestApp( App[ None ] ):
+class CanvasTestApp(App[None]):
     """The Canvas testing application."""
 
     CSS = """
     Canvas {
         border: round green;
         width: 1fr;
         height: 1fr;
     }
     """
 
-    def compose( self ) -> ComposeResult:
-        yield Canvas( 120, 120, Color( 30, 40, 50 ) )
+    BINDINGS = [
+        ("r", "clear(255, 0, 0)"),
+        ("g", "clear(0, 255, 0)"),
+        ("b", "clear(0, 0, 255)"),
+    ]
+
+    def compose(self) -> ComposeResult:
+        yield Canvas(120, 120, Color(30, 40, 50))
 
-    def on_mount( self ) -> None:
+    @on(Mount)
+    def its_all_dark(self) -> None:
         """Set up the display once the DOM is available."""
-        canvas = self.query_one( Canvas )
+        canvas = self.query_one(Canvas)
+
+        canvas.draw_line(60, 40, 90, 80, Color(128, 128, 128))
+        canvas.draw_line(60, 40, 30, 80, Color(128, 128, 128))
+        canvas.draw_line(30, 80, 90, 80, Color(128, 128, 128))
+
+        canvas.draw_line(0, 70, 48, 55, Color(255, 255, 255))
+
+        for n in range(52, 59):
+            canvas.draw_line(48, 55, 58, n, Color(128, 128, 128))
+
+        canvas.draw_line(70, 52, 119, 57, Color(255, 0, 0))
+        canvas.draw_line(71, 53, 119, 58, Color(255, 165, 0))
+        canvas.draw_line(72, 54, 119, 59, Color(255, 255, 0))
+        canvas.draw_line(72, 55, 119, 60, Color(0, 255, 0))
+        canvas.draw_line(73, 56, 119, 61, Color(0, 0, 255))
+        canvas.draw_line(74, 57, 119, 62, Color(75, 0, 130))
+        canvas.draw_line(75, 58, 119, 63, Color(143, 0, 255))
+
+        canvas.focus()
+
+    def action_clear(self, red: int, green: int, blue: int) -> None:
+        """Handle the clear keyboard action."""
+        self.query_one(Canvas).clear(Color(red, green, blue))
+        self.its_all_dark()
 
-        canvas.draw_line( 60, 40, 90, 80, Color( 128, 128, 128 ) )
-        canvas.draw_line( 60, 40, 30, 80, Color( 128, 128, 128 ) )
-        canvas.draw_line( 30, 80, 90, 80, Color( 128, 128, 128 ) )
-
-        canvas.draw_line( 0, 70, 48, 55, Color( 255, 255, 255 ) )
-
-        for n in range( 52, 59 ):
-            canvas.draw_line( 48, 55, 58, n, Color( 128, 128, 128 ) )
-
-        canvas.draw_line( 70, 52, 119, 57, Color( 255, 0, 0 ) )
-        canvas.draw_line( 71, 53, 119, 58, Color( 255, 165, 0 ) )
-        canvas.draw_line( 72, 54, 119, 59, Color( 255, 255, 0 ) )
-        canvas.draw_line( 72, 55, 119, 60, Color( 0, 255, 0 ) )
-        canvas.draw_line( 73, 56, 119, 61, Color( 0, 0, 255 ) )
-        canvas.draw_line( 74, 57, 119, 62, Color( 75, 0, 130 ) )
-        canvas.draw_line( 75, 58, 119, 63, Color( 143, 0, 255 ) )
 
 if __name__ == "__main__":
     CanvasTestApp().run()
 
 ### __main__.py ends here
```

## textual_canvas/canvas.py

```diff
@@ -1,35 +1,37 @@
 """Provides a simple character cell-based canvas widget for Textual applications."""
 
 ##############################################################################
 # Python imports.
-from __future__        import annotations
-from typing            import Iterable
-from functools         import lru_cache
-from math              import ceil
+from __future__ import annotations
+from typing import Iterable
+from functools import lru_cache
+from math import ceil
 from typing_extensions import Self
 
 ##############################################################################
 # Rich imports.
 from rich.segment import Segment
-from rich.style   import Style
+from rich.style import Style
 
 ##############################################################################
 # Textual imports.
-from textual.color       import Color
-from textual.geometry    import Size
+from textual.color import Color
+from textual.geometry import Size
 from textual.scroll_view import ScrollView
-from textual.strip       import Strip
+from textual.strip import Strip
+
 
 ##############################################################################
-class CanvasError( Exception ):
+class CanvasError(Exception):
     """Type of errors raised by the `Canvas` widget."""
 
+
 ##############################################################################
-class Canvas( ScrollView, can_focus=True ):
+class Canvas(ScrollView, can_focus=True):
     """A simple character-cell canvas widget.
 
     The widget is designed such that there are two 'pixels' per character
     cell; one being the top half of the cell, the other being the bottom.
     While not exactly square, this will make it more square than using a
     whole cell as a simple pixel.
 
@@ -41,87 +43,115 @@
     I want to get it right, then I want to get it fast.
     """
 
     def __init__(
         self,
         width: int,
         height: int,
-        color: Color = Color( 0, 0, 0),
-        name: str | None    = None,
-        id: str | None      = None, # pylint:disable=redefined-builtin
+        color: Color = Color(0, 0, 0),
+        name: str | None = None,
+        id: str | None = None,  # pylint:disable=redefined-builtin
         classes: str | None = None,
-        disabled: bool      = False
+        disabled: bool = False,
     ):
         """Initialise the canvas.
 
         Args:
             width: The width of the canvas.
             height: The height of the canvas.
             color: An optional default colour for the canvas.
             name: The name of the canvas widget.
             id: The ID of the canvas widget in the DOM.
             classes: The CSS classes of the canvas widget.
             disabled: Whether the canvas widget is disabled or not.
         """
         # Pass the normal Textual widget stuff up the chain.
-        super().__init__( name=name, id=id, classes=classes, disabled=disabled )
+        super().__init__(name=name, id=id, classes=classes, disabled=disabled)
 
-        # Remember the width and height.
-        self._width  = width
+        # Remember main canvas parameters.
+        self._width = width
         self._height = height
+        self._colour = color
 
-        # Generate the underlying "canvas" structure.
-        self._canvas = [
-            [ color for _ in range( width ) ] for _ in range( height )
-        ]
+        # Start with an empty canvas.
+        self._blank_canvas()
 
         # Used as a source of "there's nothing here" for the last row in a
         # canvas if we're likely to go off the end.
         #
         # TODO: Rather than use the default colour of the canvas, perhaps
         # take the background color of the widget itself?
-        self._the_void = [ color for _ in range( width ) ]
+        self._the_void = [color for _ in range(width)]
 
         # Ensure we can scroll around the canvas.
-        self.virtual_size = Size( width, ceil( height / 2 ) )
+        self.virtual_size = Size(width, ceil(height / 2))
+
+    def _blank_canvas(self) -> None:
+        """Set the canvas to a blank canvas."""
+        self._canvas = [
+            [self._colour for _ in range(self.width)] for _ in range(self.height)
+        ]
 
     @property
-    def width( self ) -> int:
+    def width(self) -> int:
         """The width of the canvas in 'pixels'."""
         return self._width
 
     @property
-    def height( self ) -> int:
+    def height(self) -> int:
         """The height of the canvas in 'pixels'."""
         return self._height
 
-    def _outwith_the_canvas( self, x: int, y: int ) -> bool:
+    def _outwith_the_canvas(self, x: int, y: int) -> bool:
         """Is the location outwith the canvas?
 
         Args:
             x: The horizontal location of the pixel.
             y: The vertical location of the pixel.
 
         """
         return x < 0 or y < 0 or x >= self._width or y >= self._height
 
-    def _pixel_check( self, x: int, y: int ) -> None:
+    def _pixel_check(self, x: int, y: int) -> None:
         """Check that a location is within the canvas.
 
         Args:
             x: The horizontal location of the pixel.
             y: The vertical location of the pixel.
 
         Raises:
             CanvasError: If the pixel location is not within the canvas.
         """
-        if self._outwith_the_canvas( x, y ):
-            raise CanvasError(f"x={x}, x={y} is not within 0, 0, {self._width}, {self._height}" )
+        if self._outwith_the_canvas(x, y):
+            raise CanvasError(
+                f"x={x}, x={y} is not within 0, 0, {self._width}, {self._height}"
+            )
+
+    def clear(self, color: Color | None = None) -> Self:
+        """Clear the canvas.
+
+        Args:
+            color: Optional default colour for the canvas.
+
+        Returns:
+            The canvas.
 
-    def set_pixels( self, locations: Iterable[ tuple[ int, int ] ], color: Color ) -> Self:
+        Note:
+            If the color isn't provided, then the color used when first
+            making the canvas is used, this in turn because the new default
+            color (and will then be used for subsequent clears, unless
+            another color is provided.)
+        """
+        if color is not None:
+            self._colour = color
+        self._blank_canvas()
+        self.refresh()
+        return self
+
+    def set_pixels(self, locations: Iterable[tuple[int, int]], color: Color) -> Self:
         """Set the colour of a collection of pixels on the canvas.
 
         Args:
             locations: An iterable of tuples of x and y location.
             color: The color to set the pixel to.
 
         Returns:
@@ -130,36 +160,36 @@
         Raises:
             CanvasError: If any pixel location is not within the canvas.
 
         Note:
             The origin of the canvas is the top left corner.
         """
         for x, y in locations:
-            self._pixel_check( x, y )
-            self._canvas[ y ][ x ] = color
+            self._pixel_check(x, y)
+            self._canvas[y][x] = color
         self.refresh()
         return self
 
-    def set_pixel( self, x: int, y: int, color: Color ) -> Self:
+    def set_pixel(self, x: int, y: int, color: Color) -> Self:
         """Set the colour of a specific pixel on the canvas.
 
         Args:
             x: The horizontal location of the pixel.
             y: The vertical location of the pixel.
             color: The color to set the pixel to.
 
         Raises:
             CanvasError: If the pixel location is not within the canvas.
 
         Note:
             The origin of the canvas is the top left corner.
         """
-        return self.set_pixels( ( ( x, y ), ), color )
+        return self.set_pixels(((x, y),), color)
 
-    def get_pixel( self, x: int, y: int ) -> Color:
+    def get_pixel(self, x: int, y: int) -> Color:
         """Get the pixel at the given location.
 
         Args:
             x: The horizontal location of the pixel.
             y: The vertical location of the pixel.
 
         Returns:
@@ -167,18 +197,18 @@
 
         Raises:
             CanvasError: If the pixel location is not within the canvas.
 
         Note:
             The origin of the canvas is the top left corner.
         """
-        self._pixel_check( x, y )
-        return self._canvas[ y ][ x ]
+        self._pixel_check(x, y)
+        return self._canvas[y][x]
 
-    def draw_line( self, x0: int, y0: int, x1: int, y1: int, color: Color ) -> Self:
+    def draw_line(self, x0: int, y0: int, x1: int, y1: int, color: Color) -> Self:
         """Draw a line between two points.
 
         Args:
             x0: Horizontal location of the starting position.
             y0: Vertical location of the starting position.
             x1: Horizontal location of the ending position.
             y1: Vertical location of the ending position.
@@ -189,42 +219,44 @@
 
         Note:
             The origin of the canvas is the top left corner.
         """
 
         # Taken from https://en.wikipedia.org/wiki/Bresenham's_line_algorithm#All_cases.
 
-        pixels: list[ tuple[ int, int ] ] = []
+        pixels: list[tuple[int, int]] = []
 
-        dx  = abs( x1 - x0 )
-        sx  = 1 if x0 < x1 else -1
-        dy  = -abs( y1 - y0 )
-        sy  = 1 if y0 < y1 else -1
+        dx = abs(x1 - x0)
+        sx = 1 if x0 < x1 else -1
+        dy = -abs(y1 - y0)
+        sy = 1 if y0 < y1 else -1
         err = dx + dy
 
         while True:
-            if not self._outwith_the_canvas( x0, y0 ):
-                pixels.append( ( x0, y0 ) )
+            if not self._outwith_the_canvas(x0, y0):
+                pixels.append((x0, y0))
             if x0 == x1 and y0 == y1:
                 break
             e2 = 2 * err
             if e2 >= dy:
                 if x0 == x1:
                     break
                 err += dy
                 x0 += sx
             if e2 <= dx:
                 if y0 == y1:
                     break
                 err += dx
                 y0 += sy
 
-        return self.set_pixels( pixels, color )
+        return self.set_pixels(pixels, color)
 
-    def draw_rectangle( self, x: int, y: int, width: int, height: int, color: Color ) -> Self:
+    def draw_rectangle(
+        self, x: int, y: int, width: int, height: int, color: Color
+    ) -> Self:
         """Draw a rectangle.
 
         Args:
             x: Horizontal location of the top left corner of the rectangle.
             y: Vertical location of the top left corner of the rectangle.
             width: The width of the rectangle.
             height: The height of the rectangle.
@@ -233,47 +265,37 @@
         Returns:
             The canvas.
 
         Note:
             The origin of the canvas is the top left corner.
         """
         with self.app.batch_update():
-            return self.draw_line(
-                x, y, x + width, y, color
-            ).draw_line(
-                x + width, y, x + width, y + height, color
-            ).draw_line(
-                x + width, y + height, x, y + height, color
-            ).draw_line(
-                x, y + height, x, y, color
+            return (
+                self.draw_line(x, y, x + width, y, color)
+                .draw_line(x + width, y, x + width, y + height, color)
+                .draw_line(x + width, y + height, x, y + height, color)
+                .draw_line(x, y + height, x, y, color)
             )
 
     @staticmethod
-    def _circle_mirror( x: int, y: int ) -> tuple[ tuple[ int, int ], ... ]:
+    def _circle_mirror(x: int, y: int) -> tuple[tuple[int, int], ...]:
         """Create an 8-way symmetry of the given points.
 
         Args:
             x: Horizontal location of the point to mirror.
             y: Vertical location of the point to mirror.
 
         Returns:
             The points needed to create an 8-way symmetry.
         """
-        return (
-            (  x,  y ),
-            (  y,  x ),
-            ( -x,  y ),
-            ( -y,  x ),
-            (  x, -y ),
-            (  y, -x ),
-            ( -x, -y ),
-            ( -y, -x )
-        )
+        return ((x, y), (y, x), (-x, y), (-y, x), (x, -y), (y, -x), (-x, -y), (-y, -x))
 
-    def draw_circle( self, center_x: int, center_y: int, radius: int, color: Color ) -> Self:
+    def draw_circle(
+        self, center_x: int, center_y: int, radius: int, color: Color
+    ) -> Self:
         """Draw a circle
 
         Args:
             center_x: The horizontal position of the center of the circle.
             center_y: The vertical position of the center of the circle.
             radius: The radius of the circle.
             color: The colour to draw circle in.
@@ -283,87 +305,102 @@
 
         Note:
             The origin of the canvas is the top left corner.
         """
 
         # Taken from https://funloop.org/post/2021-03-15-bresenham-circle-drawing-algorithm.html.
 
-        pixels: list[ tuple[ int, int ] ] = []
+        pixels: list[tuple[int, int]] = []
 
         x = 0
         y = -radius
         f_m = 1 - radius
         d_e = 3
-        d_ne = -( radius << 1 ) + 5
-        pixels.extend( self._circle_mirror( x, y ) )
+        d_ne = -(radius << 1) + 5
+        pixels.extend(self._circle_mirror(x, y))
         while x < -y:
             if f_m <= 0:
                 f_m += d_e
             else:
                 f_m += d_ne
                 d_ne += 2
                 y += 1
             d_e += 2
             d_ne += 2
             x += 1
-            pixels.extend( self._circle_mirror( x, y ) )
+            pixels.extend(self._circle_mirror(x, y))
 
-        return self.set_pixels( [
-            ( center_x + x, center_y + y ) for x, y in pixels
-            if not self._outwith_the_canvas( center_x + x, center_y + y )
-        ], color )
+        return self.set_pixels(
+            [
+                (center_x + x, center_y + y)
+                for x, y in pixels
+                if not self._outwith_the_canvas(center_x + x, center_y + y)
+            ],
+            color,
+        )
 
     _CELL = "\u2584"
     """The character to use to draw two pixels in one cell in the canvas."""
 
     @lru_cache()
-    def _segment_of( self, top: Color, bottom: Color ) -> Segment:
+    def _segment_of(self, top: Color, bottom: Color) -> Segment:
         """Construct a segment to show the two colours in one cell.
 
         Args:
             top: The colour for the top pixel.
             bottom: The colour for the bottom pixel.
 
         Returns:
             A `Segment` that will display the two pixels.
         """
-        return Segment( self._CELL, style=Style.from_color( bottom.rich_color, top.rich_color ) )
+        return Segment(
+            self._CELL, style=Style.from_color(bottom.rich_color, top.rich_color)
+        )
 
-    def render_line( self, y: int ) -> Strip:
+    def render_line(self, y: int) -> Strip:
         """Render a line in the display.
 
         Args:
             y: The line to render.
 
         Returns:
             A `Strip` that is the line to render.
         """
 
         # Get where we're scrolled to.
         scroll_x, scroll_y = self.scroll_offset
 
         # We're going to be drawing two lines from the canvas in one line in
         # the display. Let's work out the first line first.
-        top_line = ( scroll_y + y ) * 2
+        top_line = (scroll_y + y) * 2
 
         # Is this off the canvas already?
         if top_line >= self.height:
             # Yup. Don't bother drawing anything.
-            return Strip( [] )
+            return Strip([])
 
         # Now, the bottom line is easy enough to work out.
         bottom_line = top_line + 1
 
         # Get the pixel values for the top line.
-        top_pixels = self._canvas[ top_line ]
+        top_pixels = self._canvas[top_line]
 
         # It's possible that the bottom line might be in the void, so...
-        bottom_pixels = self._the_void if bottom_line >= self.height else self._canvas[ bottom_line ]
+        bottom_pixels = (
+            self._the_void if bottom_line >= self.height else self._canvas[bottom_line]
+        )
 
         # At this point we know what colours we're going to be mashing
         # together into the terminal line we're drawing. So let's get to it.
-        return Strip( [
-            self._segment_of( top_pixels[ pixel ], bottom_pixels[ pixel ] )
-            for pixel in range( self.width )
-        ] ).crop( scroll_x, scroll_x + self.scrollable_content_region.width ).simplify()
+        return (
+            Strip(
+                [
+                    self._segment_of(top_pixels[pixel], bottom_pixels[pixel])
+                    for pixel in range(self.width)
+                ]
+            )
+            .crop(scroll_x, scroll_x + self.scrollable_content_region.width)
+            .simplify()
+        )
+
 
 ### canvas.py ends here
```

## Comparing `textual_canvas-0.1.0.dist-info/METADATA` & `textual_canvas-0.2.0.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: textual-canvas
-Version: 0.1.0
+Version: 0.2.0
 Summary: A simple Textual canvas widget.
 Home-page: https://github.com/davep/textual-canvas
 Author: Dave Pearson
 Author-email: davep@davep.org
 Maintainer: Dave Pearson
 Maintainer-email: davep@davep.org
 License: License :: OSI Approved :: MIT License
@@ -14,25 +14,24 @@
 Project-URL: Discussions, https://github.com/davep/textual-canvas/discussions
 Keywords: terminal,library,canvas,drawing
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Environment :: Console
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Terminals
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Typing :: Typed
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
-Requires-Dist: textual (>=0.16.0)
+Requires-Dist: textual (>=0.29.0)
 
 # textual-canvas
 
 ![Being used for textual-mandelbrot](https://raw.githubusercontent.com/davep/textual-canvas/main/img/textual-mandelbrot.png)
 *An example of `textual-canvas` being used in a Textual application*
 
 ## Introduction
@@ -97,14 +96,15 @@
 
 ```python
 yield Canvas( 120, 120, Color( 30, 40, 50 ) )
 ```
 
 Currently there are the following methods available for drawing:
 
+- `clear( self, color: Color | None = None ) -> Self`
 - `set_pixel( self, x: int, y: int, color: Color ) -> Self`
 - `set_pixels( self, locations: Iterable[ tuple[ int, int ] ], color: Color ) -> Self`
 - `draw_line( self, x0: int, y0: int, x1: int, y1: int, color: Color ) -> Self`
 - `draw_rectangle( self, x: int, y: int, width: int, height: int, color: Color ) -> Self`
 - `draw_circle( self, center_x: int, center_y: int, radius: int, color: Color ) -> Self`
 
 I'll document all of this better, when I spend more time on it than the 1/2
```

