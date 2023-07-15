# Comparing `tmp/palette_generator-0.1.2.tar.gz` & `tmp/palette_generator-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "palette_generator-0.1.2.tar", max compression
+gzip compressed data, was "palette_generator-0.1.3.tar", max compression
```

## Comparing `palette_generator-0.1.2.tar` & `palette_generator-0.1.3.tar`

### file list

```diff
@@ -1,12 +1,11 @@
--rw-r--r--   0        0        0    16725 2022-01-18 00:03:17.715442 palette_generator-0.1.2/LICENSE.md
--rw-r--r--   0        0        0      243 2022-01-18 00:03:17.715442 palette_generator-0.1.2/README.md
--rw-r--r--   0        0        0      136 2022-01-17 00:18:38.874601 palette_generator-0.1.2/palette_generator/__init__.py
--rw-r--r--   0        0        0      401 2022-01-17 00:18:00.434910 palette_generator-0.1.2/palette_generator/__main__.py
--rw-r--r--   0        0        0     1112 2022-01-17 05:35:30.577021 palette_generator-0.1.2/palette_generator/_make_parser.py
--rw-r--r--   0        0        0     6197 2022-01-17 20:00:37.046568 palette_generator-0.1.2/palette_generator/convert_colors.py
--rwxr-xr-x   0        0        0     2731 2022-01-17 20:00:37.046568 palette_generator-0.1.2/palette_generator/extract_colors.py
--rwxr-xr-x   0        0        0     8992 2022-01-17 20:00:37.046568 palette_generator-0.1.2/palette_generator/gen_palette.py
--rwxr-xr-x   0        0        0    12611 2022-01-17 20:00:37.046568 palette_generator-0.1.2/palette_generator/make_theme.py
--rw-r--r--   0        0        0     1083 2022-01-18 00:44:39.303915 palette_generator-0.1.2/pyproject.toml
--rw-r--r--   0        0        0      979 2022-01-18 00:45:14.592157 palette_generator-0.1.2/setup.py
--rw-r--r--   0        0        0     1049 2022-01-18 00:45:14.592540 palette_generator-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0    16725 2022-01-18 00:03:17.715442 palette_generator-0.1.3/LICENSE.md
+-rw-r--r--   0        0        0      243 2023-01-28 21:36:39.011709 palette_generator-0.1.3/README.md
+-rw-r--r--   0        0        0      136 2022-01-17 00:18:38.874601 palette_generator-0.1.3/palette_generator/__init__.py
+-rw-r--r--   0        0        0      401 2022-01-17 00:18:00.434910 palette_generator-0.1.3/palette_generator/__main__.py
+-rw-r--r--   0        0        0     1107 2023-07-15 22:51:58.586489 palette_generator-0.1.3/palette_generator/_make_parser.py
+-rw-r--r--   0        0        0     6138 2023-07-15 22:52:38.653032 palette_generator-0.1.3/palette_generator/convert_colors.py
+-rwxr-xr-x   0        0        0     2694 2023-07-15 22:52:49.339665 palette_generator-0.1.3/palette_generator/extract_colors.py
+-rwxr-xr-x   0        0        0     8878 2023-07-15 22:53:26.659546 palette_generator-0.1.3/palette_generator/gen_palette.py
+-rwxr-xr-x   0        0        0    12511 2023-07-15 22:54:06.329416 palette_generator-0.1.3/palette_generator/make_theme.py
+-rw-r--r--   0        0        0     1077 2023-07-15 22:26:50.977796 palette_generator-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0     1088 1970-01-01 00:00:00.000000 palette_generator-0.1.3/PKG-INFO
```

### Comparing `palette_generator-0.1.2/LICENSE.md` & `palette_generator-0.1.3/LICENSE.md`

 * *Files identical despite different names*

### Comparing `palette_generator-0.1.2/palette_generator/_make_parser.py` & `palette_generator-0.1.3/palette_generator/_make_parser.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,16 +2,15 @@
 
 from . import extract_colors
 from . import gen_palette
 from . import make_theme
 
 
 def make_parser() -> argparse.ArgumentParser:
-    """
-    Make CLI parser which can call submodule parsers.
+    """Make CLI parser which can call submodule parsers.
 
     Returns:
         argparse.ArgumentParser: said parser
     """
     parser = argparse.ArgumentParser(prog="python -m palette_generator")
     parser.formatter_class = argparse.ArgumentDefaultsHelpFormatter
     subparsers = parser.add_subparsers(dest="mode")
```

### Comparing `palette_generator-0.1.2/palette_generator/convert_colors.py` & `palette_generator-0.1.3/palette_generator/convert_colors.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,8 @@
-"""
-Tools for converting between color spaces.
+"""Tools for converting between color spaces.
 
 Functions:
     * :func:`hex_to_rgb`: hexadecimal to rgb
     * :func:`rgb_to_hex`: rgb to hexadecimal
     * :func:`rgb_to_hsv`: rgb to hsv
     * :func:`rgb_to_xyz`: rgb to xyz
     * :func:`xyz_to_rgb`: xyz to rgb
@@ -19,16 +18,15 @@
 
 
 # pylint: disable=invalid-name
 # Though short, the names are well-understood.
 
 
 def hex_to_rgb(hex_code: str) -> Tuple[int, int, int]:
-    """
-    Convert hexadecimal code to RGB space.
+    """Convert hexadecimal code to RGB space.
 
     Args:
         hex_code (str): hexadecimal
 
     Returns:
         Tuple[int, int, int]: RGB
     """
@@ -36,36 +34,35 @@
     r = int(hex_code[:2], 16)
     g = int(hex_code[2:4], 16)
     b = int(hex_code[4:], 16)
     return r, g, b
 
 
 def rgb_to_hex(rgb: Tuple[int, int, int]) -> str:
-    """
-    Convert RGB space to hexadecimal code.
+    """Convert RGB space to hexadecimal code.
 
     Args:
         rgb (Tuple[int, int, int]): RGB space
 
     Returns:
         str: hexadecimal code
     """
     return "#" + "".join([hex(c)[2:].upper().zfill(2) for c in rgb])
 
 
 def rgb_to_hsv(rgb: Tuple[int, int, int]) -> Tuple[float, float, float]:
-    """
-    Convert RGB space to HSV space.
+    """Convert RGB space to HSV space.
 
     Args:
         rgb (Tuple[int, int, int]): RGB space
 
     Returns:
         Tuple[float, float, float]: HSV space
     """
+
     def delt_channel(vchannel):
         return (((vmax - vchannel) / 6) + (delt / 2)) / delt
 
     vr, vg, vb = [c / 255 for c in rgb]
     vmin, vmax = min(vr, vg, vb), max(vr, vg, vb)
     delt = vmax - vmin
     #  v = vmax
@@ -82,23 +79,22 @@
 
     h = h + 1 if h < 0 else h - 1
     return h, s, vmax
 
 
 def _var_rgb(channel: int) -> float:
     """Help function for rgb->xyz."""
-    channel_float = channel/255
+    channel_float = channel / 255
     if channel_float > 0.04045:
         return ((channel_float + 0.055) / 1.055) ** 2.4 * 100
     return channel_float / 12.92 * 100
 
 
 def rgb_to_xyz(rgb: Tuple[int, int, int]) -> Tuple[float, float, float]:
-    """
-    Convert RGB space to XYZ space.
+    """Convert RGB space to XYZ space.
 
     Args:
         rgb (Tuple[int, int, int]): RGB space
 
     Returns:
         Tuple[float, float, float]: XYZ space
     """
@@ -115,35 +111,31 @@
         out = round((1.055 * (var ** (1 / 2.4)) - 0.055) * 255)
     else:
         out = round(12.92 * var * 255)
     return min(out, 255)
 
 
 def xyz_to_rgb(xyz: Tuple[float, float, float]) -> Tuple[int, int, int]:
-    """
-    Convert XYZ space to RGB space.
+    """Convert XYZ space to RGB space.
 
     Args:
         xyz (Tuple[float, float, float]): XYZ space
 
     Returns:
         Tuple[int, int, int]: RGB space
     """
     vx, vy, vz = [c / 100 for c in xyz]
     vr = 3.2406 * vx - 1.5372 * vy - 0.4986 * vz
     vg = -0.9689 * vx + 1.8758 * vy + 0.0415 * vz
     vb = 0.0557 * vx - 0.2040 * vy + 1.0570 * vz
     return _var_rgb_prime(vr), _var_rgb_prime(vg), _var_rgb_prime(vb)
 
 
-def xyz_to_cieluv(
-    xyz: Tuple[float, float, float]
-) -> Tuple[float, float, float]:
-    """
-    Convert XYZ space to CIE-LUV space.
+def xyz_to_cieluv(xyz: Tuple[float, float, float]) -> Tuple[float, float, float]:
+    """Convert XYZ space to CIE-LUV space.
 
     Args:
         xyz (Tuple[float, float, float]): XYZ space
 
     Returns:
         Tuple[float, float, float]: CIE-LUV space
     """
@@ -163,56 +155,51 @@
     )
     cie_l = (116 * vy) - 16
     cie_u = 13 * cie_l * vu
     cie_v = 13 * cie_l * vv
     return cie_l, cie_u, cie_v
 
 
-def cieluv_to_xyz(
-    luv: Tuple[float, float, float]
-) -> Tuple[float, float, float]:
-    """
-    Convert CIE-LUV space to XYZ space.
+def cieluv_to_xyz(luv: Tuple[float, float, float]) -> Tuple[float, float, float]:
+    """Convert CIE-LUV space to XYZ space.
 
     Args:
         luv (Tuple[float, float, float]): CIE-LUV space
 
     Returns:
         Tuple[float, float, float]: XYZ space
     """
     l, u, v = luv
     vy = (l + 16) / 116
-    vy = vy ** 3 if vy ** 3 > 0.008856 else (vy - 16 / 116) / 7.787
+    vy = vy**3 if vy**3 > 0.008856 else (vy - 16 / 116) / 7.787
     vu = 0 if l == 0 else u / (13 * l)
     vv = 0 if l == 0 else v / (13 * l)
 
     y = vy * 100
     x = 0.0 if vv == 0 else -(9 * y * vu) / ((vu - 4) * vv - vu * vv)
     z = 0.0 if vv == 0 else (9 * y - (15 * vv * y) - (vv * x)) / (3 * vv)
     return x, y, z
 
 
 def cieluv_to_hex(luv: Tuple[float, float, float]) -> str:
-    """
-    Convert CIE-LUV space to hexadecimal code.
+    """Convert CIE-LUV space to hexadecimal code.
 
     Args:
         luv (Tuple[float, float, float]): CIE-LUV space
 
     Returns:
         str: hexadecimal code
     """
     xyz = cieluv_to_xyz(luv)
     rgb = xyz_to_rgb(xyz)
     return rgb_to_hex(rgb)
 
 
 def hex_to_everything(hex_series: pd.Series) -> pd.DataFrame:
-    """
-    Convert many hexadecimal codes to all available color spaces.
+    """Convert many hexadecimal codes to all available color spaces.
 
     Args:
         hex_series (pd.Series): many hexadecimal codes
 
     Returns:
         pd.DataFrame: all color spaces in columns,
             with same index as `hex_series`
```

### Comparing `palette_generator-0.1.2/palette_generator/extract_colors.py` & `palette_generator-0.1.3/palette_generator/extract_colors.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 #!/bin/env python3
 
 
-"""
-Extract a finite number of representative colors from an image.
+"""Extract a finite number of representative colors from an image.
 
 Functions:
     * :func:`main`: extract colors from an image using CLI-style args
     * :func:`make_parser`: create the CLI parser
 """
 
 
@@ -17,16 +16,15 @@
 
 from .convert_colors import rgb_to_hex
 
 
 def make_parser(
     parser: argparse.ArgumentParser = None,
 ) -> argparse.ArgumentParser:
-    """
-    Create a CLI parser.
+    """Create a CLI parser.
 
     Args:
         parser (argparse.ArgumentParser): pre-existing parser to modify;
             default: `None`
 
     Returns:
         argparse.ArgumentParser: argument parser
@@ -55,21 +53,17 @@
         default="color_hist.txt",
         help="The color histogram output.",
     )
     return parser
 
 
 def main(
-    img_path: str,
-    n_colors: int = 512,
-    hist_file: str = "color_hist.txt",
-    **kwargs
+    img_path: str, n_colors: int = 512, hist_file: str = "color_hist.txt", **kwargs
 ):
-    """
-    Extract colors from an image.
+    """Extract colors from an image.
 
     Args:
         img_path (str): image file
         n_colors (int): number of colors to extract; default: 512
         hist_file (str): save counts and hex codes to this file;
             default: 'color_hist.txt'
 
@@ -77,17 +71,15 @@
     """
     # Load the image.
     img = Image(filename=img_path)
     # Convert the image into `n_colors` palette space.
     # `dither` is important for generating counts that are more representative
     #   of human vision.
     img.quantize(n_colors, dither=True)
-    colors = pd.DataFrame(
-        img.histogram.items(), columns=["color_object", "count"]
-    )
+    colors = pd.DataFrame(img.histogram.items(), columns=["color_object", "count"])
     # Calculate hexadecimal codes from wand color objects.
     colors["hex"] = (
         colors["color_object"]
         .apply(lambda c: (c.red_int8, c.green_int8, c.blue_int8))
         .apply(rgb_to_hex)
     )
     # Sort by count.
```

### Comparing `palette_generator-0.1.2/palette_generator/gen_palette.py` & `palette_generator-0.1.3/palette_generator/gen_palette.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 #!/bin/env python3
 
-"""
-Generate a palette image from a base image and set of colors.
+"""Generate a palette image from a base image and set of colors.
 
 functions:
     * :func:`main`: run the program with CLI-based arguments
     * :func:`make_parser`: create the CLI parser
 
 classes:
     * :class:`Palette`: visual palette created on an image base
@@ -22,16 +21,15 @@
 from .convert_colors import hex_to_rgb, rgb_to_hsv
 
 
 # TODO: option for one-col vs two-col palette
 def make_parser(
     parser: argparse.ArgumentParser = None,
 ) -> argparse.ArgumentParser:
-    """
-    Make a CLI-based argument parser.
+    """Make a CLI-based argument parser.
 
     Args:
         parser (argparse.ArgumentParser): pre-existing parser to modify;
             default: `None`
 
     Returns:
         argparse.ArgumentParser:
@@ -61,16 +59,15 @@
     parser.add_argument(
         "-fs", "--font-size", type=int, default=28, help="Font size for text."
     )
     return parser
 
 
 class Palette:
-    """
-    Visual palette created on an image base.
+    """Visual palette created on an image base.
 
     Overlay color samples on image across the left and right of the image. If
     the input is provided in '.json' format, also label the hex codes with the
     names provided by the '.json'. If 'fg' and/or 'bg' are provided, they will
     be used as the text color for the labels.
 
     Args:
@@ -120,45 +117,40 @@
 
     def show(self):
         """Not Implemented."""
         raise NotImplementedError
         #  self.image.show()
 
     def save(self, fname: str = None):
-        """
-        Save the palette to image file.
+        """Save the palette to image file.
 
         Args:
             fname (str): path to save; default: :const:`palette_file`
         """
         fname = fname or self.palette_file
         self.image.save(filename=fname)
 
     def _scale_image(self):
         """Scale image, in place, to palette size."""
         n_colors_per_col = int(np.ceil(len(self.colors) / 2))
         width, height = self.image.size
-        new_height = (
-            n_colors_per_col * (self.cheight + self.cmargin) + self.cmargin
-        )
+        new_height = n_colors_per_col * (self.cheight + self.cmargin) + self.cmargin
         scale = new_height / height
         new_width = int(scale * width)
         self.image.resize(new_width, new_height)
 
     def _add_color(self):
         """Add the next color to the palette."""
         # Calc constants.
         n_colors_per_col = int(np.ceil(len(self.colors) / 2))
         x_pos = self._colors_drawn // n_colors_per_col
         y_pos = self._colors_drawn % n_colors_per_col
         width, _ = self.image.size
 
-        left = (
-            self.cmargin if x_pos == 0 else width - self.cmargin - self.cwidth
-        )
+        left = self.cmargin if x_pos == 0 else width - self.cmargin - self.cwidth
         top = self.cmargin + y_pos * (self.cheight + self.cmargin)
         label = (  # If colors have names, include them.
             None
             if self.colors.index.dtype == int
             else self.colors.index[self._colors_drawn]
         )
 
@@ -169,16 +161,15 @@
             top + self.cheight // 2,
             self.colors.iloc[self._colors_drawn],
             label=label,
         )
         self._colors_drawn += 1
 
     def _draw_rect(self, left: int, top: int, color: str):
-        """
-        Draw a color swatch on the palette image.
+        """Draw a color swatch on the palette image.
 
         Args:
             left (int): left position, in pixels
             top (int): top position, in pixels
             color (str): color of swatch
         """
         self._draw.fill_color = color
@@ -211,33 +202,29 @@
         if fg_thresh < bg_thresh:
             self._fg, self._bg = self._bg, self._fg
 
         # Define the value threshold as between the two.
         self._color_thresh = np.mean([fg_thresh, bg_thresh])
 
     def _get_font_color(self, color: str) -> str:
-        """
-        Find the best font color to label a color swatch.
+        """Find the best font color to label a color swatch.
 
         Args:
             color (str): the hexadecimal background of the swatch
 
         Returns:
             str: chosen font color
         """
         _, _, val = rgb_to_hsv(hex_to_rgb(color))
         if val < self._color_thresh:
             return self._fg
         return self._bg
 
-    def _draw_text(
-        self, text_x: int, text_y: int, color: str, label: str = None
-    ):
-        """
-        Overlay text on a color swatch.
+    def _draw_text(self, text_x: int, text_y: int, color: str, label: str = None):
+        """Overlay text on a color swatch.
 
         Args:
             text_x (int): x-position of text center, in pixels
             text_y (int): y-position of text center, in pixels
             color (str): the hexadecimal color to write
             label (str): name of the color; default: None
         """
@@ -255,16 +242,15 @@
         self._draw.text_interline_spacing = -font_size // 6
         # Draw the text in the correct color.
         self._draw.fill_color = self._get_font_color(color)
         self._draw.text(text_x, text_y + v_offset, text)
 
 
 def main(args: argparse.Namespace):
-    """
-    Generate a visual palette from CLI-like arguments.
+    """Generate a visual palette from CLI-like arguments.
 
     Args:
         args (argparse.Namespace): arguments from CLI
     """
     palette = Palette(**vars(args))
     palette.save()
```

### Comparing `palette_generator-0.1.2/palette_generator/make_theme.py` & `palette_generator-0.1.3/palette_generator/make_theme.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 #!/bin/env python3
 
 
-"""
-Create a 12-color theme from a pre-computed palette.
+"""Create a 12-color theme from a pre-computed palette.
 
 Classes:
     * :class:`Themer`: make a color theme from a palette
 
 Functions:
     * :func:`main`: run the script
     * :func:`make_parser`: make the CLI parser
@@ -22,16 +21,15 @@
 
 from .convert_colors import cieluv_to_hex, hex_to_everything
 
 
 def make_parser(
     parser: argparse.ArgumentParser = None,
 ) -> argparse.ArgumentParser:
-    """
-    Create a CLI parser.
+    """Create a CLI parser.
 
     Args:
         parser (argparse.ArgumentParser): pre-existing parser to modify;
             default: `None`
 
     Returns:
         argparse.ArgumentParser: argument parser
@@ -82,16 +80,15 @@
 
 
 def _exclude(
     subset: pd.DataFrame,
     exclude: pd.Series,
     exclude_dist: float = 100.0,
 ) -> pd.DataFrame:
-    """
-    Exclude a color and its neighbors from a DataFrame.
+    """Exclude a color and its neighbors from a DataFrame.
 
     Args:
         subset (pd.DataFrame): DataFrame of colors
         exclude (pd.Series): color to exclude
         exclude_dist (float): colors within this distance of `exclude` will be
             excluded
 
@@ -99,16 +96,15 @@
         pd.DataFrame: `subset` with some colors excluded
     """
     dist = subset[_LUV].apply(euclidean, v=exclude[_LUV], axis=1)
     return subset[dist > exclude_dist]
 
 
 class Themer:
-    """
-    Make a color theme.
+    """Make a color theme.
 
     Args:
         fname (str): color histogram file; default: 'color_hist.txt'
         p_mix (float): percent to mix pure colors in with histogram colors;
             default: 0.25
     """
 
@@ -130,32 +126,29 @@
     _ALL = 0
     _BRIGHT = 1
     _MUTED = 2
 
     def __init__(self, fname: str = "color_hist.txt", p_mix: float = 0.25):
         """Initialize :class:`Themer`."""
         colors = pd.read_csv(fname)
-        colors = colors.sort_values("count", ascending=False).reset_index(
-            drop=True
-        )
+        colors = colors.sort_values("count", ascending=False).reset_index(drop=True)
         #: colors loaded from `fname`
         self.colors = pd.merge(
             colors,
             hex_to_everything(colors["hex"]),
             left_on="hex",
             right_on="hex",
         )
 
         self._theme = pd.DataFrame()
         #: amount to mix pure colors with image colors
         self.p_mix = p_mix
 
     def _get_subset(self, bright_mode: int = 1) -> pd.DataFrame:
-        """
-        Get a subset of :attr:`self.colors`.
+        """Get a subset of :attr:`self.colors`.
 
         Args:
             bright_mode (int): one of :attr:`self._BRIGHT`,
                 :attr:`self._MUTED`, or :attr:`self._ALL`.
                 'bright' colors are those where saturation and value are in
                 the top half of all colors; default: :attr:`self._BRIGHT`
 
@@ -174,16 +167,15 @@
             return self.colors[
                 (self.colors["sat"] < self.colors["sat"].quantile(0.5))
                 | (self.colors["val"] < self.colors["val"].quantile(0.5))
             ]
         raise ValueError(f"Unexpected value for `bright_mode`: {bright_mode}")
 
     def _measure(self, luv: Tuple[float, float, float], **kwargs) -> pd.Series:
-        """
-        Find the closest (or farthest) color from given.
+        """Find the closest (or farthest) color from given.
 
         Args:
             luv (Tuple[float, float, float]): given color, in CIE-LUV space
             mode (Callable): how to measure distance;
                 default: :func:`euclidean`
             bright_mode (int): one of :attr:`self._BRIGHT`,
                 :attr:`self._MUTED`, or :attr:`self._ALL`.
@@ -208,16 +200,15 @@
             colors = _exclude(colors, exclude, exclude_dist)
         dist = colors[_LUV].apply(mode, v=luv, axis=1)
         if nearest:
             return colors.loc[dist.idxmin()]
         return colors.loc[dist.idxmax()]
 
     def _get_mixed(self, ref: str, **kwargs) -> pd.Series:
-        """
-        Get best represention of a color.
+        """Get best represention of a color.
 
         Find the in-palette color closest to `ref` and mix it with the pure
         color according to :attr:`p_mix` proportion.
 
         Args:
             ref (str): reference color e.g., "red"
 
@@ -234,16 +225,15 @@
         # Now to everything.
         hex_code = cieluv_to_hex(mixed_luv)
         mixed = hex_to_everything(pd.Series([hex_code])).iloc[0]
         mixed.name = ref
         return mixed
 
     def _get_special(self, mode: str) -> pd.Series:
-        """
-        Get a specific theme color from the palette space.
+        """Get a specific theme color from the palette space.
 
         Args:
             mode (str): one of
                 'common' = most commonly-used color
                 'mean' = color closest to the mean of all colors (un-weighted)
                 'bg' = alias of 'common'
                 'fg' = muted color furthest from the most commonly-used color
@@ -254,33 +244,29 @@
 
         Returns:
             pd.Series: the queried color
         """
         if mode == "common" or mode == "bg":
             color = self.colors.iloc[0]
         elif mode == "mean":
-            color = self._measure(
-                self.colors[_LUV].mean(), bright_mode=self._ALL
-            )
+            color = self._measure(self.colors[_LUV].mean(), bright_mode=self._ALL)
         elif mode == "fg":
             color = self._measure(
                 self.colors.iloc[0][_LUV],
                 bright_mode=self._MUTED,
                 nearest=False,
             )
         elif mode == "accent":
             try:
                 subset = self._get_subset(self._BRIGHT)
                 subset = _exclude(subset, exclude=self._theme.loc["bg"])
                 color = self.colors.loc[subset["sat"].idxmax()]
             except KeyError as exc:
                 # We should never get here, but just in case...
-                raise ValueError(
-                    "Must calculate 'bg' before 'accent'."
-                ) from exc
+                raise ValueError("Must calculate 'bg' before 'accent'.") from exc
         elif mode == "secondary":
             try:
                 color = self._measure(
                     self._theme.loc["accent", _LUV],
                     bright_mode=self._BRIGHT,
                     nearest=False,
                     exclude=self._theme.loc["bg"],
@@ -293,40 +279,40 @@
         else:
             raise NotImplementedError(f"Mode '{mode}' not implemented.")
         color.name = mode
         return color
 
     @property
     def theme(self) -> pd.Series:
-        """
-        Calculate and return the best-calculated theme for the palette.
+        """Calculate and return the best-calculated theme for the palette.
 
         Returns:
             pd.Series: hex codes for each theme color
         """
         if self._theme.empty:
             muted = ["white", "black"]
             for ref in self._ref.index:
                 mode = self._MUTED if ref in muted else self._BRIGHT
                 color = self._get_mixed(ref, bright_mode=mode)
-                self._theme = self._theme.append(color)
+                self._theme = pd.concat([self._theme.T, color], axis=1).T
             for special in [
                 "common",
                 "mean",
                 "fg",
                 "bg",
                 "accent",
                 "secondary",
             ]:
-                self._theme = self._theme.append(self._get_special(special))
+                self._theme = pd.concat(
+                    [self._theme.T, self._get_special(special)], axis=1
+                ).T
         return self._theme["hex"].drop(["common", "mean"])
 
     def plot(self, mode: str = "LUV", scale: float = 30.0):
-        """
-        Plot the palette's colors, weighted by size.
+        """Plot the palette's colors, weighted by size.
 
         Args:
             mode (3-len str or iterable): which color space to use;
                 default: 'LUV'
             scale (float): Degree by which to scale point size; default: 30.
         """
         # pylint: disable=invalid-name
@@ -346,32 +332,30 @@
         ax.set_xlabel(x)
         ax.set_ylabel(y)
         ax.set_zlabel(z)
 
         plt.show()
 
     def save(self, fname: str = "colors.json"):
-        """
-        Save the theme to file.
+        """Save the theme to file.
 
         Can save in json format or text/csv format.
 
         Args:
             fname (str): save path; will save in json format if `fname` ends
                 with '.json', else in csv format; default: 'colors.json'
         """
         if fname.endswith(".json"):
             self.theme.to_json(fname)
         else:
             self.theme.to_csv(fname, index=False, header=False)
 
 
 def main(args: argparse.Namespace):
-    """
-    Execute the :mod:`palette_generator.make_theme` script.
+    """Execute the :mod:`palette_generator.make_theme` script.
 
     Creates theme and saves it to file.
 
     Args:
         args (argparse.Namespace): arguments from running script in CLI
     """
     theme = Themer(args.hist_file, p_mix=args.p_mix)
```

### Comparing `palette_generator-0.1.2/pyproject.toml` & `palette_generator-0.1.3/pyproject.toml`

 * *Files 26% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 [tool.poetry]
 name = "palette_generator"
-version = "0.1.2"
+version = "0.1.3"
 description = "`palette_generator` is here to turn your images into beautiful palettes"
 readme = "README.md"
 repository = "https://github.com/neonfuzz/palette_generator"
 documentation = "https://neonfuzz.github.io/palette_generator/html/index.html"
 authors = ["neonfuzz"]
 
 [tool.poetry.dependencies]
-python = ">=3.7,<3.11"
-matplotlib = "@latest"
-numpy = "@latest"
-pandas = "@latest"
-scipy = "@latest"
-Wand = "@latest"
+python = ">=3.9,<3.13"
+matplotlib = "^3.7.2"
+numpy = "^1.25.1"
+pandas = "^2.0.3"
+scipy = "^1.11.1"
+wand = "^0.6.11"
 
-[tool.poetry.dev-dependencies]
-Sphinx = "@latest"
-sphinx-argparse = "@latest"
-sphinx-rtd-dark-mode = "@latest"
+[tool.poetry.group.dev.dependencies]
+sphinx = "^7.0.1"
+sphinx-argparse = "^0.4.0"
+sphinx-rtd-dark-mode = "^1.2.4"
 
 [tool.sphinx]
 extensions = [
     "sphinx.ext.autodoc",
     "sphinx.ext.autosummary",
     "sphinx.ext.napoleon",
     "sphinxarg.ext",
@@ -34,9 +34,9 @@
 html_static_path = ["_static"]
 default_dark_mode = true
 
 [tool.sphinx.html_theme_options]
 collapse_navigation = false
 
 [build-system]
-requires = ["poetry-core>=1.0.0"]
+requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `palette_generator-0.1.2/PKG-INFO` & `palette_generator-0.1.3/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,24 +1,23 @@
 Metadata-Version: 2.1
 Name: palette-generator
-Version: 0.1.2
+Version: 0.1.3
 Summary: `palette_generator` is here to turn your images into beautiful palettes
 Home-page: https://github.com/neonfuzz/palette_generator
 Author: neonfuzz
-Requires-Python: >=3.7,<3.11
+Requires-Python: >=3.9,<3.13
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
-Requires-Dist: Wand
-Requires-Dist: matplotlib
-Requires-Dist: numpy
-Requires-Dist: pandas
-Requires-Dist: scipy
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: matplotlib (>=3.7.2,<4.0.0)
+Requires-Dist: numpy (>=1.25.1,<2.0.0)
+Requires-Dist: pandas (>=2.0.3,<3.0.0)
+Requires-Dist: scipy (>=1.11.1,<2.0.0)
+Requires-Dist: wand (>=0.6.11,<0.7.0)
 Project-URL: Documentation, https://neonfuzz.github.io/palette_generator/html/index.html
 Project-URL: Repository, https://github.com/neonfuzz/palette_generator
 Description-Content-Type: text/markdown
 
 
 Installation
 ============
```

