# Comparing `tmp/dnfunc-0.0.3a2.tar.gz` & `tmp/dnfunc-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dnfunc-0.0.3a2.tar", max compression
+gzip compressed data, was "dnfunc-0.0.4.tar", max compression
```

## Comparing `dnfunc-0.0.3a2.tar` & `dnfunc-0.0.4.tar`

### file list

```diff
@@ -1,5 +1,6 @@
--rw-r--r--   0        0        0     1065 2023-05-05 08:20:19.643067 dnfunc-0.0.3a2/LICENSE
--rw-r--r--   0        0        0      472 2023-05-05 08:20:19.643067 dnfunc-0.0.3a2/README.md
--rw-r--r--   0        0        0     2663 2023-05-05 08:20:33.743370 dnfunc-0.0.3a2/pyproject.toml
--rw-r--r--   0        0        0    49969 2023-05-05 08:20:19.647066 dnfunc-0.0.3a2/src/dnfunc/__init__.py
--rw-r--r--   0        0        0     1403 1970-01-01 00:00:00.000000 dnfunc-0.0.3a2/PKG-INFO
+-rw-r--r--   0        0        0     1065 2023-07-16 16:30:37.949099 dnfunc-0.0.4/LICENSE
+-rw-r--r--   0        0        0      534 2023-07-16 16:30:37.949099 dnfunc-0.0.4/README.md
+-rw-r--r--   0        0        0     2679 2023-07-16 16:30:55.885174 dnfunc-0.0.4/pyproject.toml
+-rw-r--r--   0        0        0      112 2023-07-16 16:30:37.949099 dnfunc-0.0.4/src/dnfunc/__init__.py
+-rw-r--r--   0        0        0    50755 2023-07-16 16:30:37.953100 dnfunc-0.0.4/src/dnfunc/dnfunc.py
+-rw-r--r--   0        0        0     1458 1970-01-01 00:00:00.000000 dnfunc-0.0.4/PKG-INFO
```

### Comparing `dnfunc-0.0.3a2/LICENSE` & `dnfunc-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `dnfunc-0.0.3a2/pyproject.toml` & `dnfunc-0.0.4/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["poetry-core>=1.0.0", "poetry-dynamic-versioning"]
 build-backend = "poetry_dynamic_versioning.backend"
 
 [tool.poetry]
 name = "dnfunc"
-version = "0.0.3-alpha.2"
-description = "A collection of Vapoursynth functions and wrapperspoetr"
+version = "0.0.4"
+description = "A collection of Vapoursynth functions and wrappers"
 authors = ["DeadNews <aurczpbgr@mozmail.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/DeadNews/dnfunc"
 repository = "https://github.com/DeadNews/dnfunc"
 keywords = ["vapoursynth", "vapoursynth-functions", "video-encoding"]
 classifiers = [
@@ -17,35 +17,35 @@
   "Topic :: Multimedia :: Video",
 ]
 
 [tool.poetry.dependencies]
 python = "^3.10"
 vapoursynth = ">=60"
 havsfunc = "^33"
-lvsfunc = "^0.7.1"
+lvsfunc = "^0.8.0"
 pyyaml = "^6.0"
 vstools = "^2.1.0"
 vsutil = "^0.8.0"
 
-[tool.poetry.group.ci.dependencies]
-black = "^23.3.0"
-mypy = "^1.2.0"
-poethepoet = "^0.20.0"
-ruff = "^0.0.264"
+[tool.poetry.group.lint.dependencies]
+black = "^23.7.0"
+mypy = "^1.4.1"
+poethepoet = "^0.21.1"
+ruff = "^0.0.278"
 types-pyyaml = "^6.0.12.9"
 
 [tool.poetry.group.test.dependencies]
-pytest = "^7.3.1"
-pytest-cov = "^4.0.0"
+pytest = "^7.4.0"
+pytest-cov = "^4.1.0"
 
 [tool.poe.tasks]
 ruff = "ruff check ."
 black = "black --check ."
 mypy = "mypy ."
-ci.sequence = ["ruff", "black", "mypy"]
+lint.sequence = ["ruff", "black", "mypy"]
 
 [tool.poetry-dynamic-versioning]
 enable = false
 vcs = "git"
 style = "semver"
 
 [tool.black]
@@ -71,21 +71,22 @@
 [tool.coverage.report]
 exclude_lines = ["if TYPE_CHECKING:", "if __name__ == .__main__.:"]
 
 [tool.ruff]
 line-length = 99
 select = ["ALL"]
 ignore = [
-  "COM812", # Trailing comma missing
-  "D203",   # 1 blank line required before class docstring
-  "D212",   # Multi-line docstring summary should start at the first line
-  "E501",   # Line too long
-  "EXE001", # Shebang is present but file is not executable
-  "FBT001", # Boolean positional arg in function definition
-  "FBT002", # Boolean default value in function definition
+  "COM812",  # Trailing comma missing
+  "D203",    # 1 blank line required before class docstring
+  "D212",    # Multi-line docstring summary should start at the first line
+  "E501",    # Line too long
+  "EXE001",  # Shebang is present but file is not executable
+  "FBT001",  # Boolean positional arg in function definition
+  "FBT002",  # Boolean default value in function definition
+  "PLR0913", # Too many arguments to function call
   #
   "D101",    # Missing docstring in public class
   "D102",    # Missing docstring in public method
   "D103",    # Missing docstring in public function
   "ERA001",  # Found commented-out code
   "PLR2004", # Magic value used in comparison
 ]
@@ -97,10 +98,7 @@
 allow-dict-calls-with-keyword-arguments = false
 
 [tool.ruff.flake8-tidy-imports]
 ban-relative-imports = "all"
 
 [tool.ruff.flake8-annotations]
 allow-star-arg-any = true
-
-[tool.ruff.pylint]
-max-args = 7
```

### Comparing `dnfunc-0.0.3a2/src/dnfunc/__init__.py` & `dnfunc-0.0.4/src/dnfunc/dnfunc.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,40 +1,51 @@
 #!/usr/bin/env python
 """A collection of Vapoursynth functions and wrappers."""
-from collections.abc import Callable, Iterable
+from __future__ import annotations
+
 from dataclasses import dataclass, field, replace
 from functools import partial
 from pathlib import Path, PurePath
 from shutil import which
-from typing import Any, NamedTuple, TypeAlias, TypeVar
+from typing import TYPE_CHECKING, NamedTuple
 
 import havsfunc as hav
 import insane_aa as iaa
-from kagefunc import adaptive_grain, kirsch, retinex_edgemask
-from vapoursynth import GRAY16, RGB, YUV420P10, VideoFrame, VideoNode, core
-from vstools import FrameRange, FrameRangeN, FrameRangesN, rfs
+import kagefunc as kg
+import vapoursynth as vs
+from vstools import rfs
 from vsutil import depth, get_depth, get_y, iterate, join, split
 from yaml import safe_load
 
-T = TypeVar("T")
-Maps: TypeAlias = FrameRangeN | FrameRangesN
-VideoFunc1: TypeAlias = Callable[[VideoNode], VideoNode]
-VideoFunc2: TypeAlias = Callable[[VideoNode, VideoNode], VideoNode]
+if TYPE_CHECKING:
+    from collections.abc import Callable, Iterable
+    from dataclasses import _DataclassT
+    from typing import Any, TypeAlias
+
+    from vstools import FrameRange, FrameRangeN, FrameRangesN
+
+    Maps: TypeAlias = FrameRangeN | FrameRangesN
+    VideoFunc: TypeAlias = Callable[..., vs.VideoNode]
 
 PROC_DEPTH = 16  # processing_depth
 
 
 def load_yaml(file_path: str) -> dict | None:
     """Load yaml settings."""
     f1 = Path(file_path)
 
     return safe_load(f1.read_text()) if f1.is_file() else None
 
 
-def override_dc(data_class: T, block: str, zone: str = "", **override: Any) -> T:
+def override_dc(
+    data_class: _DataclassT,
+    block: str,
+    zone: str = "",
+    **override: Any,
+) -> _DataclassT:
     """
     Override default data_class params.
 
     Configuration preference order:
     1. func params
     2. yaml zone
     3. yaml main
@@ -43,22 +54,22 @@
     settings = load_yaml("./settings.yaml")
 
     if settings is not None:
         block_settings = settings.get(block)
 
         if block_settings is not None:
             # yaml main
-            data_class = replace(data_class, **block_settings["main"])  # type: ignore[type-var]
+            data_class = replace(data_class, **block_settings["main"])
 
             if zone and zone != "main":
                 # yaml zone
-                data_class = replace(data_class, **block_settings[zone])  # type: ignore[type-var]
+                data_class = replace(data_class, **block_settings[zone])
 
     # func params
-    return replace(data_class, **override)  # type: ignore[type-var]
+    return replace(data_class, **override)
 
 
 ######
 # aa #
 ######
 
 
@@ -108,21 +119,21 @@
     resc_expr: str = ""
     #
     uv_desc_h: int = 0
     uv_desc_str: float = 0.32
 
 
 def insane_aa(
-    clip: VideoNode,
+    clip: vs.VideoNode,
     aaset: AASettings,
     out_mode: iaa.ClipMode,
     desc_h: int,
     desc_str: float,
-    ext_mask: VideoNode | None = None,
-) -> VideoNode:
+    ext_mask: vs.VideoNode | None = None,
+) -> vs.VideoNode:
     edi3set = get_edi3_mode()
     return iaa.insaneAA(
         clip=clip,
         eedi3_mode=edi3set.eedi3_mode,
         eedi3_device=edi3set.device,
         nnedi3_mode=edi3set.nnedi3_mode,
         nnedi3_device=edi3set.device,
@@ -140,15 +151,15 @@
         beta=aaset.beta,
         gamma=aaset.gamma,
         external_mask=ext_mask,
         output_mode=out_mode,
     )
 
 
-def aa_yuv(clip: VideoNode, aaset: AASettings) -> VideoNode:
+def aa_yuv(clip: vs.VideoNode, aaset: AASettings) -> vs.VideoNode:
     planes = split(clip)
 
     planes[0] = insane_aa(
         clip=planes[0],
         aaset=aaset,
         out_mode=iaa.ClipMode.MASKED,
         desc_str=aaset.desc_str,
@@ -169,20 +180,20 @@
         desc_h=aaset.uv_desc_h,
     )
 
     return join(planes)
 
 
 def aa(
-    clip: VideoNode,
+    clip: vs.VideoNode,
     zone: str = "",
     epname: str = "",
-    ext_mask: VideoNode | None = None,
+    ext_mask: vs.VideoNode | None = None,
     **override: Any,
-) -> VideoNode:
+) -> vs.VideoNode:
     """Anti-aliasing wrapper."""
     if epname:
         f1 = Path(f"./temp/{epname}_aa_lossless.mp4")
         if f1.is_file():
             aa_lossless = source(f1)
 
             if aa_lossless.num_frames != clip.num_frames:
@@ -203,56 +214,56 @@
         out_mode=iaa.ClipMode.FULL,
         desc_str=aaset.desc_str,
         desc_h=clip.height if aaset.eedi3_only else aaset.desc_h,
         ext_mask=ext_mask,
     )
 
 
-def diff_mask(clipa: VideoNode, clipb: VideoNode, mthr: int = 25) -> VideoNode:
+def diff_mask(clipa: vs.VideoNode, clipb: vs.VideoNode, mthr: int = 25) -> vs.VideoNode:
     return (
-        core.std.MakeDiff(clipa=get_y(clipa), clipb=get_y(clipb), planes=[0])
+        vs.core.std.MakeDiff(clipa=get_y(clipa), clipb=get_y(clipb), planes=[0])
         .std.Prewitt()
         .std.Expr(f"x {mthr} < 0 x ?")
         .std.Convolution([1] * 9)
         .std.Convolution([1] * 9)
         .std.Expr("x 8 - 2.2 *")
     )
 
 
 def save_titles(
-    oped_clip: VideoNode,
-    ncoped: VideoNode,
-    ncoped_aa: VideoNode,
-) -> VideoNode:
+    oped_clip: vs.VideoNode,
+    ncoped: vs.VideoNode,
+    ncoped_aa: vs.VideoNode,
+) -> vs.VideoNode:
     """Save OP/ED titles with expr and diff_mask."""
     oped_planes = split(oped_clip)
 
-    oped_planes[0] = core.std.Expr(
+    oped_planes[0] = vs.core.std.Expr(
         [oped_planes[0], get_y(ncoped), get_y(ncoped_aa)],
         ["x y - z +"],
     )
 
     saved_titles = join(oped_planes)
     mask = diff_mask(oped_clip, ncoped)
 
     return masked_merge(saved_titles, oped_clip, mask=mask, yuv=False)
 
 
-def oped(  # noqa: PLR0913
-    clip: VideoNode,
+def oped(
+    clip: vs.VideoNode,
     name: str,
     offset: int,
     start: int,
     end: int,
     zone: str = "",
-    ext_nc: VideoNode | None = None,
+    ext_nc: vs.VideoNode | None = None,
     input_aa: bool = False,
-    edgefix: VideoFunc1 | None = None,
-    filtr: VideoFunc2 | None = None,
-) -> VideoNode:
+    edgefix: VideoFunc | None = None,
+    filtr: VideoFunc | None = None,
+) -> vs.VideoNode:
     """Save OP/ED titles wrapper."""
     ncoped_end = end - 1 - start + offset
 
     oped_clip = clip.std.Trim(start, end - 1)
     ncoped = source(f"./in/{name}.mp4").std.Trim(offset, ncoped_end)
 
     ncoped_aa_src = ext_nc.std.Trim(offset, ncoped_end) if ext_nc else ncoped
@@ -284,15 +295,15 @@
 
 
 ##########
 # filter #
 ##########
 
 
-def gradfun_mask(source: VideoNode, thr_det: float = 1, mode: int = 3) -> VideoNode:
+def gradfun_mask(source: vs.VideoNode, thr_det: float = 1, mode: int = 3) -> vs.VideoNode:
     """Stolen from fvsfunc."""
     from muvsfunc import _Build_gf3_range_mask as gf3_range_mask
 
     src_y = get_y(source)
     src_8 = depth(src_y, 8)
 
     tl = max(thr_det * 0.75, 1.0) - 0.0001
@@ -308,32 +319,32 @@
 
         return depth(deband_mask, PROC_DEPTH)
 
     return None
 
 
 def adaptive_mix(
-    clip: VideoNode,
-    f1: VideoNode,
-    f2: VideoNode,
+    clip: vs.VideoNode,
+    f1: vs.VideoNode,
+    f2: vs.VideoNode,
     scaling: float,
     yuv: bool = False,
-) -> VideoNode:
-    adaptive_mask = adaptive_grain(clip=clip, luma_scaling=scaling, show_mask=True).std.Invert()
+) -> vs.VideoNode:
+    adaptive_mask = kg.adaptive_grain(clip=clip, luma_scaling=scaling, show_mask=True).std.Invert()
 
     return masked_merge(f1, f2, mask=adaptive_mask, yuv=yuv)
 
 
 def adaptive_debandmask(
-    clip: VideoNode,
-    source: VideoNode,
-    db_mask: VideoNode,
+    clip: vs.VideoNode,
+    source: vs.VideoNode,
+    db_mask: vs.VideoNode,
     yaml: dict,
     db_expr: str = "",
-) -> VideoNode:
+) -> vs.VideoNode:
     for zone in yaml:
         db_mode = yaml[zone]["db_mode"]
         thr_det = yaml[zone]["db_thr"]
         scaling = yaml[zone]["scaling"]
 
         db_n = gradfun_mask(source=source, thr_det=thr_det, mode=db_mode)
         db_mask = adaptive_mix(
@@ -346,81 +357,81 @@
 
     if db_expr:
         db_mask = db_mask.std.Expr(db_expr)
 
     return db_mask
 
 
-def adaptive_smdegrain(clip: VideoNode, smdegrain: VideoNode, yaml: dict) -> VideoNode:
+def adaptive_smdegrain(clip: vs.VideoNode, smdegrain: vs.VideoNode, yaml: dict) -> vs.VideoNode:
     for zone in yaml:
         sm_thr = yaml[zone]["sm_thr"]
         sm_pref_mode = yaml[zone]["sm_pref_mode"]
         scaling = yaml[zone]["scaling"]
 
         dn_n = smdegrain_(clip=clip, sm_thr=sm_thr, sm_pref_mode=sm_pref_mode)
 
         smdegrain = adaptive_mix(clip=clip, f1=smdegrain, f2=dn_n, scaling=scaling, yuv=True)
 
     return smdegrain
 
 
 def save_uv_unique_lines(
-    clip: VideoNode,
-    source: VideoNode,
+    clip: vs.VideoNode,
+    source: vs.VideoNode,
     mode: str = "retinex",
     sigma: float = 1.0,
-) -> VideoNode:
+) -> vs.VideoNode:
     clip_planes = split(clip)
     src_planes = split(source)
 
     if mode == "retinex":
-        mask_u = retinex_edgemask(src_planes[1], sigma=sigma)
-        mask_v = retinex_edgemask(src_planes[2], sigma=sigma)
+        mask_u = kg.retinex_edgemask(src_planes[1], sigma=sigma)
+        mask_v = kg.retinex_edgemask(src_planes[2], sigma=sigma)
     elif mode == "kirsch":
         mask_u = edge_detect(src_planes[1], mode="kirsch")
         mask_v = edge_detect(src_planes[2], mode="kirsch")
 
     fix_u = masked_merge(clip_planes[1], src_planes[1], mask_u)
     fix_v = masked_merge(clip_planes[2], src_planes[2], mask_v)
 
     return join([clip_planes[0], fix_u, fix_v])
 
 
 def save_black(
-    clip: VideoNode,
-    filtered: VideoNode,
+    clip: vs.VideoNode,
+    filtered: vs.VideoNode,
     threshold: float = 0.06276,
-) -> VideoNode:
+) -> vs.VideoNode:
     """Return filtered when avg exceeds the threshold."""
 
     def _diff(
         n: int,  # noqa: ARG001
-        f: VideoFrame,
-        clip: VideoNode,
-        filtered: VideoNode,
+        f: vs.VideoFrame,
+        clip: vs.VideoNode,
+        filtered: vs.VideoNode,
         threshold: float,
-    ) -> VideoNode:
+    ) -> vs.VideoNode:
         return filtered if f.props.PlaneStatsAverage > threshold else clip
 
-    return core.std.FrameEval(
+    return vs.core.std.FrameEval(
         clip=clip,
         eval=partial(_diff, clip=clip, filtered=filtered, threshold=threshold),
-        prop_src=core.std.PlaneStats(clip),
+        prop_src=vs.core.std.PlaneStats(clip),
     )
 
 
 def f3kdb_deband(
-    clip: VideoNode,
+    clip: vs.VideoNode,
     det_y: int,
     grainy: int,
     drange: int,
     yuv: bool = False,
-) -> VideoNode:
+) -> vs.VideoNode:
     """https://f3kdb.readthedocs.io/en/latest/presets.html."""
-    return core.f3kdb.Deband(
+    return vs.core.f3kdb.Deband(
         clip=clip,
         range=drange,
         dither_algo=3,
         y=det_y,
         cb=det_y if yuv else 0,
         cr=det_y if yuv else 0,
         blur_first=True,
@@ -429,39 +440,39 @@
         dynamic_grain=False,
         keep_tv_range=True,
         output_depth=PROC_DEPTH,
     )
 
 
 def contrasharp(
-    clip: VideoNode,
-    source: VideoNode,
-    cs_mask: VideoNode,
+    clip: vs.VideoNode,
+    source: vs.VideoNode,
+    cs_mask: vs.VideoNode,
     sm_thr: int,
     cs_val: float,
-) -> tuple[VideoNode, VideoNode]:
+) -> tuple[vs.VideoNode, vs.VideoNode]:
     from CSMOD import CSMOD
 
     contrasharped = CSMOD(
         clip,
         source=source,
         preset="detail",
         edgemask=cs_mask,
         thSAD=sm_thr,
     )
-    clip_expr = core.std.Expr([contrasharped, clip], f"x {cs_val} * y 1 {cs_val} - * +")
+    clip_expr = vs.core.std.Expr([contrasharped, clip], f"x {cs_val} * y 1 {cs_val} - * +")
 
     return (clip_expr, contrasharped)
 
 
-def _out_mask(mask: VideoNode) -> VideoNode:
-    return core.resize.Point(mask, format=YUV420P10, matrix_s="709")
+def _out_mask(mask: vs.VideoNode) -> vs.VideoNode:
+    return vs.core.resize.Point(mask, format=vs.YUV420P10, matrix_s="709")
 
 
-def smdegrain_(clip: VideoNode, sm_thr: int = 48, sm_pref_mode: int = 1) -> VideoNode:
+def smdegrain_(clip: vs.VideoNode, sm_thr: int = 48, sm_pref_mode: int = 1) -> vs.VideoNode:
     sm_set = {
         "prefilter": sm_pref_mode,
         "tr": 4,
         "RefineMotion": True,
         "contrasharp": False,
     }
 
@@ -483,20 +494,20 @@
 
         return join(planes)
 
     return None
 
 
 def bm3d_(
-    clip: VideoNode,
+    clip: vs.VideoNode,
     bm_sigma: float = 2,
     bm_radius: float = 1,
     sm_thr: int = 48,
     sm_pref_mode: int = 1,
-) -> VideoNode:
+) -> vs.VideoNode:
     from mvsfunc import BM3D
 
     planes = split(clip)
 
     planes[0] = BM3D(planes[0], sigma=bm_sigma, radius1=bm_radius)
     planes[1] = smdegrain_(planes[1], sm_thr=sm_thr, sm_pref_mode=sm_pref_mode)
     planes[2] = smdegrain_(planes[2], sm_thr=sm_thr, sm_pref_mode=sm_pref_mode)
@@ -538,29 +549,29 @@
     ag_str: float = 0.0
     ag_scaling: float = 24.0
     ag_saveblack: int = 1
     ag_saveblack_tolerance: int = 2
 
 
 def filt(  # noqa: PLR0911, PLR0912, PLR0915, C901
-    mrgc: VideoNode,
+    mrgc: vs.VideoNode,
     zone: str = "",
     out_mode: int = 0,
-    prefilt_func: VideoFunc2 | None = None,
+    prefilt_func: VideoFunc | None = None,
     **override: Any,
-) -> VideoNode:
+) -> vs.VideoNode:
     fset = FilterSettings()
     fset = override_dc(fset, block="filt", zone=zone, **override)
 
     clip16 = depth(mrgc, PROC_DEPTH)
 
     if prefilt_func:
         clip16 = prefilt_func(mrgc, clip16)
 
-    rt_mask_clip16 = retinex_edgemask(src=clip16, sigma=fset.rt_sigma)
+    rt_mask_clip16 = kg.retinex_edgemask(src=clip16, sigma=fset.rt_sigma)
 
     if fset.dn_mode is None:
         denoised = clip16
     else:
         # dn_ttsmooth
         if fset.dn_ttsmooth:
             ttsmooth_set = {"thresh": 1, "mdiff": 0, "strength": 1}
@@ -593,15 +604,15 @@
                 sm_pref_mode=fset.sm_pref_mode,
             )
 
         denoised = masked_merge(full_denoise, clip16, mask=rt_mask_clip16, yuv=True)
 
         # dn_pref
         if fset.dn_pref or fset.cs_mode:
-            rt_mask_denoised = retinex_edgemask(denoised, sigma=fset.rt_sigma)
+            rt_mask_denoised = kg.retinex_edgemask(denoised, sigma=fset.rt_sigma)
 
             if fset.dn_expr:
                 rt_mask_denoised_def = rt_mask_denoised
                 rt_mask_denoised = rt_mask_denoised.std.Expr(fset.dn_expr)
 
             rt_mask_mix = (
                 adaptive_mix(
@@ -730,17 +741,17 @@
         if fset.db_pref:
             filtered = masked_merge(debanded, denoised, mask=rt_mask_afterdb, yuv=fset.db_yuv)
         else:
             filtered = masked_merge(debanded, clip16, mask=rt_mask_afterdb, yuv=fset.db_yuv)
 
     # adaptive_grain
     if out_mode == 1:
-        ag_mask = adaptive_grain(filtered, luma_scaling=fset.ag_scaling, show_mask=True)
+        ag_mask = kg.adaptive_grain(filtered, luma_scaling=fset.ag_scaling, show_mask=True)
     if fset.ag_str != 0:
-        grained = adaptive_grain(filtered, luma_scaling=fset.ag_scaling, strength=fset.ag_str)
+        grained = kg.adaptive_grain(filtered, luma_scaling=fset.ag_scaling, strength=fset.ag_str)
 
         if fset.ag_saveblack == 1:
             filtered = save_black(filtered, grained, threshold=0.06276)
         elif fset.ag_saveblack == 2:
             filtered = rfs_color(
                 f1=grained,
                 f2=filtered,
@@ -799,44 +810,44 @@
 
 
 def source(
     file: str | Path | PurePath,
     bits: int = 0,
     fpsnum: int = 0,
     fpsden: int = 0,
-) -> VideoNode:
+) -> vs.VideoNode:
     """Load video source."""
     f1 = PurePath(file)
 
     if f1.suffix == ".mp4":
-        src = core.lsmas.LibavSMASHSource(source=f1)
+        src = vs.core.lsmas.LibavSMASHSource(source=f1)
     else:
-        src = core.lsmas.LWLibavSource(source=f1)
+        src = vs.core.lsmas.LWLibavSource(source=f1)
 
     if fpsnum and fpsden:
         src = src.std.AssumeFPS(fpsnum=fpsnum, fpsden=fpsden)
 
     if not bits:
         bits = PROC_DEPTH
 
     return depth(src, bits)
 
 
-def average(clips: list[VideoNode]) -> VideoNode:
+def average(clips: list[vs.VideoNode]) -> vs.VideoNode:
     min_num_frames = min(clip.num_frames for clip in clips)
 
-    return core.average.Mean([clip.std.Trim(0, min_num_frames - 1) for clip in clips])
+    return vs.core.average.Mean([clip.std.Trim(0, min_num_frames - 1) for clip in clips])
 
 
 def out(
-    clip: VideoNode,
+    clip: vs.VideoNode,
     epname: str,
     bits: int = 10,
-    filtred: VideoFunc2 | None = None,
-) -> VideoNode:
+    filtred: VideoFunc | None = None,
+) -> vs.VideoNode:
     if get_depth(clip) != bits:
         clip = depth(clip, bits)
 
     f1 = Path(f"./temp/{epname}_lossless.mp4")
 
     if f1.is_file():
         lossless = source(f1, bits=bits)
@@ -845,22 +856,22 @@
 
         return lossless
 
     return clip
 
 
 def pw(
-    mrgc: VideoNode,
+    mrgc: vs.VideoNode,
     masks: Iterable[int] = (3, 4),
     mask_zone: str = "",
-    epis: VideoNode = None,
-    clip: VideoNode = None,
+    epis: vs.VideoNode | None = None,
+    clip: vs.VideoNode | None = None,
     clip2_zone: str = "",
-    ext_rip: VideoNode | None = None,
-) -> VideoNode:
+    ext_rip: vs.VideoNode | None = None,
+) -> vs.VideoNode:
     pw_list = []
     if masks:
         for out_mode in masks:
             mask = filt(mrgc, zone=mask_zone, out_mode=out_mode)
             pw_list.append(mask)
 
     if epis:
@@ -868,135 +879,135 @@
     if clip:
         pw_list.append(clip)
     if clip2_zone:
         pw_list.append(depth(filt(mrgc, zone=clip2_zone), 10))
     if ext_rip:
         pw_list.append(ext_rip)
 
-    return core.std.Interleave(pw_list)
+    return vs.core.std.Interleave(pw_list)
 
 
-def aa_pw(epis: VideoNode, zones: Iterable[str] = ("main", "test")) -> VideoNode:
+def aa_pw(epis: vs.VideoNode, zones: Iterable[str] = ("main", "test")) -> vs.VideoNode:
     pw_list = []
     if epis:
         pw_list.append(epis)
 
     for zone in zones:
         aaep = aa(epis, zone=zone)
         pw_list.append(aaep)
 
-    return core.std.Interleave(pw_list)
+    return vs.core.std.Interleave(pw_list)
 
 
 def masked_merge(
-    f1: VideoNode,
-    f2: VideoNode,
-    mask: VideoNode,
+    f1: vs.VideoNode,
+    f2: vs.VideoNode,
+    mask: vs.VideoNode,
     yuv: bool = False,
-) -> VideoNode:
-    return core.std.MaskedMerge(
+) -> vs.VideoNode:
+    return vs.core.std.MaskedMerge(
         clipa=f1,
         clipb=f2,
         mask=mask,
         planes=[0, 1, 2] if yuv else [0],
     )
 
 
-def check_num_frames(epis: VideoNode, clip: VideoNode) -> None:
+def check_num_frames(epis: vs.VideoNode, clip: vs.VideoNode) -> None:
     if epis.num_frames != clip.num_frames:
         msg = f"{epis.num_frames=}, {clip.num_frames=}"
         raise NumFramesError(msg)
 
 
 def _mask_resize(
-    mask: VideoNode,
-    format_src: VideoNode | None = None,  # noqa: ARG001
-) -> VideoNode:
+    mask: vs.VideoNode,
+    format_src: vs.VideoNode | None = None,  # noqa: ARG001
+) -> vs.VideoNode:
     # if format_src:
     #     mask_format = format_src.format.replace(color_family=GRAY, subsampling_w=0, subsampling_h=0)
     # else:
-    #     mask_format = GRAY16
+    #     mask_format = vs.GRAY16
 
-    mask_format = GRAY16
+    mask_format = vs.GRAY16
 
     return (
         mask.resize.Point(matrix_s="709", format=mask_format)
-        if mask.format.color_family == RGB
+        if mask.format.color_family == vs.RGB
         else mask.resize.Point(format=mask_format)
     )
 
 
 def color_mask(
-    mask_src: VideoNode,
-    format_src: VideoNode,
+    mask_src: vs.VideoNode,
+    format_src: vs.VideoNode,
     color: str = "$000000",
     tolerance: int = 2,
-) -> VideoNode:
+) -> vs.VideoNode:
     if get_depth(mask_src) != 8:
         mask_src = depth(mask_src, 8)
 
     mask = mask_src.tcm.TColorMask(colors=color, tolerance=tolerance)
 
     return _mask_resize(mask, format_src)
 
 
 def rfs_color(
-    mask_src: VideoNode,
-    f1: VideoNode | None = None,
-    f2: VideoNode | None = None,
+    mask_src: vs.VideoNode,
+    f1: vs.VideoNode | None = None,
+    f2: vs.VideoNode | None = None,
     color: str = "$000000",
     tolerance: int = 2,
     out_mask: bool = False,
     maps: Maps | None = None,
-) -> VideoNode:
+) -> vs.VideoNode:
     mask = color_mask(mask_src=mask_src, format_src=f1, color=color, tolerance=tolerance)
     if out_mask:
         return mask
 
     replaced = masked_merge(f1, f2, mask=mask, yuv=False)
 
     return rfs(f1, replaced, maps) if maps else replaced
 
 
-def image_mask(maskname: str, format_src: VideoNode) -> VideoNode:
-    mask = core.imwri.Read(f"./mask/{maskname}.png")
+def image_mask(maskname: str, format_src: vs.VideoNode) -> vs.VideoNode:
+    mask = vs.core.imwri.Read(f"./mask/{maskname}.png")
     return _mask_resize(mask, format_src)
 
 
 def rfs_image(
-    mrgc: VideoNode,
-    epis: VideoNode,
+    mrgc: vs.VideoNode,
+    epis: vs.VideoNode,
     maskname: str = "",
     yuv: bool = False,
     maps: Maps | None = None,
-) -> VideoNode:
+) -> vs.VideoNode:
     mask = image_mask(maskname, format_src=mrgc)
     replaced = masked_merge(mrgc, epis, mask=mask, yuv=yuv)
 
     return rfs(mrgc, replaced, maps) if maps else replaced
 
 
 def rfs_diff(
-    mrgc: VideoNode,
-    epis: VideoNode,
+    mrgc: vs.VideoNode,
+    epis: vs.VideoNode,
     maps: Maps | None = None,
     mthr: int = 25,
     yuv: bool = True,
     out_mask: bool = False,
-) -> VideoNode:
+) -> vs.VideoNode:
     mask = diff_mask(mrgc, epis, mthr=mthr)
     if out_mask:
         return mask
 
     replaced = masked_merge(mrgc, epis, mask=mask, yuv=yuv)
 
     return rfs(mrgc, replaced, maps) if maps else replaced
 
 
-def diff_rescale_mask(source: VideoNode, dset: AASettings) -> VideoNode:
+def diff_rescale_mask(source: vs.VideoNode, dset: AASettings) -> vs.VideoNode:
     """
     Build mask from difference of original and re-upscales clips.
 
     Based on atomchtools.
     """
     from descale import Descale
     from fvsfunc import Resize
@@ -1021,15 +1032,15 @@
     upsc = Resize(src=desc, w=source.width, h=source.height, **upsc_set)
 
     if get_depth(source) != 8:
         clip = depth(clip, 8)
         upsc = depth(upsc, 8)
 
     mask = (
-        core.std.MakeDiff(clip, upsc)
+        vs.core.std.MakeDiff(clip, upsc)
         .rgvs.RemoveGrain(2)
         .rgvs.RemoveGrain(2)
         .hist.Luma()
         .std.Expr(f"x {dset.resc_mthr} < 0 x ?")
         .std.Prewitt()
         .std.Maximum()
         .std.Maximum()
@@ -1042,49 +1053,49 @@
     if get_depth(mask) != (source_depth := get_depth(source)):
         mask = depth(mask, source_depth)
 
     return mask
 
 
 def rfs_resc(
-    mrgc: VideoNode = None,
-    epis: VideoNode = None,
+    mrgc: vs.VideoNode | None = None,
+    epis: vs.VideoNode | None = None,
     zone: str = "",
     maps: Maps | None = None,
-    filt: VideoFunc1 | None = None,
+    filt: VideoFunc | None = None,
     out_mask: bool = False,
     **override: Any,
-) -> VideoNode:
+) -> vs.VideoNode:
     dset = AASettings()
     dset = override_dc(dset, block="aa", zone=zone, **override)
 
     mask = diff_rescale_mask(epis, dset=dset)
     if filt:
         mask = filt(mask)
     if out_mask:
         return mask
 
     replaced = masked_merge(mrgc, epis, mask=mask)
 
     return rfs(mrgc, replaced, maps) if maps else replaced
 
 
-def _hard(clip: VideoNode, mthr: int, yuv: bool = False) -> VideoNode:
+def _hard(clip: vs.VideoNode, mthr: int, yuv: bool = False) -> vs.VideoNode:
     from HardAA import HardAA
 
     return HardAA(
         clip=clip,
         mask="simple",
         mthr=mthr,
         LumaOnly=not yuv,
         useCL=get_edi3_mode().device != -1,
     )
 
 
-def hard(clip: VideoNode, mthr: int, zone: str = "", **override: Any) -> VideoNode:
+def hard(clip: vs.VideoNode, mthr: int, zone: str = "", **override: Any) -> vs.VideoNode:
     yuv = yuv if (yuv := override.get("yuv")) is not None else False
 
     if zone is None and override.get("desc_h") is None:
         return _hard(clip, mthr=mthr, yuv=yuv)
 
     revset = AASettings()
     revset = override_dc(revset, block="aa", zone=zone, **override)
@@ -1099,21 +1110,21 @@
     )
 
     hard_aa = _hard(revert, mthr=mthr, yuv=yuv)
     return rescale_(hard_aa, mode="insane_aa", ref_clip=clip)
 
 
 def rfs_hard(
-    mrgc: VideoNode,
-    src: VideoNode,
+    mrgc: vs.VideoNode,
+    src: vs.VideoNode,
     mthr: int,
     maps: Maps,
     zone: str = "",
     **override: Any,
-) -> VideoNode:
+) -> vs.VideoNode:
     hard_ = hard(src, mthr=mthr, zone=zone, **override)
 
     return rfs(mrgc, hard_, maps)
 
 
 @dataclass(frozen=True)
 class QTGMCSettings:
@@ -1125,15 +1136,15 @@
     #
     input_type: int = 1
     preset: str = "placebo"
     match_enhance: float = 0.95
     sharp: float = 0.2
 
 
-def qtgmc(clip: VideoNode, zone: str = "", **override: Any) -> VideoNode:
+def qtgmc(clip: vs.VideoNode, zone: str = "", **override: Any) -> vs.VideoNode:
     """
     QTGMC.
 
     InputType — 0 for interlaced input. Mode 1 is for general progressive material.
     Modes 2 & 3 are designed for badly deinterlaced material.
     Sharpness — The default 1.0 is fairly sharp. If using source-match the default is 0.2
     """
@@ -1162,91 +1173,107 @@
         ThSAD2=qset.thsad2 * qset.k,
         ThSCD1=qset.thscd1 * qset.k,
         ThSCD2=qset.thscd2 * qset.k,
     )
 
 
 def rfs_qtgmc(
-    mrgc: VideoNode,
-    src: VideoNode,
+    mrgc: vs.VideoNode,
+    src: vs.VideoNode,
     maps: Maps,
     zone: str = "",
     **override: Any,
-) -> VideoNode:
+) -> vs.VideoNode:
     stabilize = qtgmc(src, zone=zone, **override)
 
     return rfs(mrgc, stabilize, maps)
 
 
-def get_kirsch2_mask(clip_y: VideoNode) -> VideoNode:
-    n = core.std.Convolution(clip_y, [5, 5, 5, -3, 0, -3, -3, -3, -3], divisor=3, saturate=False)
-    nw = core.std.Convolution(clip_y, [5, 5, -3, 5, 0, -3, -3, -3, -3], divisor=3, saturate=False)
-    w = core.std.Convolution(clip_y, [5, -3, -3, 5, 0, -3, 5, -3, -3], divisor=3, saturate=False)
-    sw = core.std.Convolution(clip_y, [-3, -3, -3, 5, 0, -3, 5, 5, -3], divisor=3, saturate=False)
-    s = core.std.Convolution(clip_y, [-3, -3, -3, -3, 0, -3, 5, 5, 5], divisor=3, saturate=False)
-    se = core.std.Convolution(clip_y, [-3, -3, -3, -3, 0, 5, -3, 5, 5], divisor=3, saturate=False)
-    e = core.std.Convolution(clip_y, [-3, -3, 5, -3, 0, 5, -3, -3, 5], divisor=3, saturate=False)
-    ne = core.std.Convolution(clip_y, [-3, 5, 5, -3, 0, 5, -3, -3, -3], divisor=3, saturate=False)
-    return core.std.Expr(
+def get_kirsch2_mask(clip_y: vs.VideoNode) -> vs.VideoNode:
+    n = vs.core.std.Convolution(
+        clip_y, [5, 5, 5, -3, 0, -3, -3, -3, -3], divisor=3, saturate=False
+    )
+    nw = vs.core.std.Convolution(
+        clip_y, [5, 5, -3, 5, 0, -3, -3, -3, -3], divisor=3, saturate=False
+    )
+    w = vs.core.std.Convolution(
+        clip_y, [5, -3, -3, 5, 0, -3, 5, -3, -3], divisor=3, saturate=False
+    )
+    sw = vs.core.std.Convolution(
+        clip_y, [-3, -3, -3, 5, 0, -3, 5, 5, -3], divisor=3, saturate=False
+    )
+    s = vs.core.std.Convolution(
+        clip_y, [-3, -3, -3, -3, 0, -3, 5, 5, 5], divisor=3, saturate=False
+    )
+    se = vs.core.std.Convolution(
+        clip_y, [-3, -3, -3, -3, 0, 5, -3, 5, 5], divisor=3, saturate=False
+    )
+    e = vs.core.std.Convolution(
+        clip_y, [-3, -3, 5, -3, 0, 5, -3, -3, 5], divisor=3, saturate=False
+    )
+    ne = vs.core.std.Convolution(
+        clip_y, [-3, 5, 5, -3, 0, 5, -3, -3, -3], divisor=3, saturate=False
+    )
+    return vs.core.std.Expr(
         [n, nw, w, sw, s, se, e, ne],
         ["x y max z max a max b max c max d max e max"],
     )
 
 
-def edge_detect(clip: VideoNode, mode: str, expr: str = "") -> VideoNode:
+def edge_detect(clip: vs.VideoNode, mode: str, expr: str = "") -> vs.VideoNode:
     clip_y = get_y(clip)
 
     if mode == "fine2":
         mask = hav.FineDehalo2(clip_y, showmask=1)
     elif mode == "kirsch":
-        mask = kirsch(clip_y)
+        mask = kg.kirsch(clip_y)
     elif mode == "kirsch2":
         mask = get_kirsch2_mask(clip_y)
     elif mode == "sobel":
-        mask = core.std.Sobel(clip_y)
+        mask = vs.core.std.Sobel(clip_y)
 
     return mask.std.Expr(expr) if expr else mask
 
 
 def outerline_mask(
-    clip: VideoNode,
+    clip: vs.VideoNode,
     mode: str = "kirsch",
     max_c: int = 3,
     min_c: int = 1,
-    ext_mask: VideoNode | None = None,
-) -> VideoNode:
+    ext_mask: vs.VideoNode | None = None,
+) -> vs.VideoNode:
     mask = ext_mask or edge_detect(clip, mode=mode)
 
-    mask_outer = iterate(mask, function=core.std.Maximum, count=max_c)
+    mask_outer = iterate(mask, function=vs.core.std.Maximum, count=max_c)
     mask_inner = mask.std.Inflate()
-    mask_inner = iterate(mask_inner, function=core.std.Minimum, count=min_c)
+    mask_inner = iterate(mask_inner, function=vs.core.std.Minimum, count=min_c)
 
-    return core.std.Expr([mask_outer, mask_inner], "x y -")
+    return vs.core.std.Expr([mask_outer, mask_inner], "x y -")
 
 
 @dataclass(frozen=True)
 class DehaloSettings:
     rx: float = 2.0
     darkstr: float = 0
     brightstr: float = 0.5
     mode: str = "kirsch"
     max_c: int = 3
     min_c: int = 1
     mask_from_filtred: bool = True
 
 
 def rfs_dehalo(
-    clip: VideoNode,
-    ext_dehalo: VideoNode | None = None,
+    clip: vs.VideoNode,
+    ext_dehalo: vs.VideoNode | None = None,
     zone: str = "",
-    ext_mask: VideoNode | None = None,
+    ext_mask: vs.VideoNode | None = None,
     maps: Maps | None = None,
     out_mask: bool = False,
     **override: Any,
-) -> VideoNode:
+) -> vs.VideoNode:
     dehset = DehaloSettings()
     dehset = override_dc(dehset, block="dehalo", zone=zone, **override)
 
     if ext_dehalo:
         dehalo = ext_dehalo
         mask_src = dehalo
     else:
@@ -1273,15 +1300,15 @@
         return mask
 
     replaced = masked_merge(clip, dehalo, mask=mask, yuv=False)
 
     return rfs(clip, replaced, maps) if maps else replaced
 
 
-def dehalo_chroma(clip: VideoNode, zone: str = "") -> VideoNode:
+def dehalo_chroma(clip: vs.VideoNode, zone: str = "") -> vs.VideoNode:
     planes = split(clip)
     planes[1] = rfs_dehalo(planes[1], zone=zone)
     planes[2] = rfs_dehalo(planes[2], zone=zone)
 
     return join(planes)
 
 
@@ -1296,21 +1323,21 @@
     mode: str = "kirsch"
     max_c: int = 3
     min_c: int = 1
     mask_from_filtred: bool = False
 
 
 def rfs_repair(
-    clip: VideoNode,
+    clip: vs.VideoNode,
     zone: str = "",
     out_mask: bool = False,
     maps: Maps | None = None,
     **override: Any,
-) -> VideoNode:
-    """Applay `Repair` filters."""
+) -> vs.VideoNode:
+    """Apply `Repair` filters."""
     repset = RepairSettings()
     repset = override_dc(repset, block="repair", zone=zone, **override)
 
     if repset.edgclr_args:
         repair = hav.EdgeCleaner(clip, **repset.edgclr_args)
     if repset.dering_args:
         repair = hav.HQDeringmod(clip, **repset.dering_args)
@@ -1327,19 +1354,19 @@
 
 @dataclass(frozen=True)
 class LineDarkSettings:
     linedark_args: dict[str, int] | None = None
 
 
 def rfs_linedark(
-    clip: VideoNode,
+    clip: vs.VideoNode,
     zone: str = "",
     maps: Maps | None = None,
     **override: Any,
-) -> VideoNode:
+) -> vs.VideoNode:
     ldset = LineDarkSettings()
     ldset = override_dc(ldset, block="linedark", zone=zone, **override)
 
     replaced = hav.FastLineDarkenMOD(clip, **ldset.linedark_args)
 
     return rfs(clip, replaced, maps) if maps else replaced
 
@@ -1350,29 +1377,29 @@
     sharp: float = 0.1
     mask_mode: str = "sobel"
     mask_expr: str = ""
     yuv: bool = False
 
 
 def rfs_sharp(
-    clip: VideoNode,
+    clip: vs.VideoNode,
     zone: str = "",
-    maps: Maps = None,
+    maps: Maps | None = None,
     out_mask: bool = False,
     **override: Any,
-) -> VideoNode:
+) -> vs.VideoNode:
     shset = SsharpSettings()
     shset = override_dc(shset, block="sharp", zone=zone, **override)
 
     mask = edge_detect(clip, mode=shset.mask_mode, expr=shset.mask_expr)
     if out_mask:
         return mask
 
     if shset.mode == "cas":
-        sharp = core.cas.CAS(clip, sharpness=shset.sharp)
+        sharp = vs.core.cas.CAS(clip, sharpness=shset.sharp)
     elif shset.mode == "finesharp":
         from finesharp import sharpen
 
         sharp = sharpen(clip, sstr=sharp)
 
     replaced = masked_merge(clip, sharp, mask=mask, yuv=shset.yuv)
 
@@ -1389,32 +1416,32 @@
     radius: int | list[int] = 0
     yuv: bool = False
 
     @staticmethod
     def to_list(val: int | list[int]) -> list[int]:
         return val if isinstance(val, list) else [val, 0, 0]
 
-    def check_yuv(self: "EdgeFixSettings") -> None:
+    def check_yuv(self: EdgeFixSettings) -> None:
         self.yuv = any(
             isinstance(val, list)
             for val in (self.top, self.bottom, self.left, self.right, self.radius)
         )
 
 
 def edgefix(
-    epis: VideoNode,
+    epis: vs.VideoNode,
     zone: str = "",
     **override: Any,
-) -> tuple[VideoNode, VideoNode, VideoFunc1]:
+) -> tuple[vs.VideoNode, vs.VideoNode, VideoFunc]:
     """Fix edges."""
 
-    def _edgefixer(epis: VideoNode) -> VideoNode:
+    def _edgefixer(epis: vs.VideoNode) -> vs.VideoNode:
         if not edset.yuv or not edset.crop_args:
             # luma
-            return core.edgefixer.Continuity(
+            return vs.core.edgefixer.Continuity(
                 epis,
                 top=edset.top,
                 bottom=edset.bottom,
                 left=edset.left,
                 right=edset.right,
                 radius=edset.radius,
             )
@@ -1472,15 +1499,15 @@
 
     epis_back = epis
     epis = _edgefixer(epis)
 
     return (epis, epis_back, _edgefixer)
 
 
-def wipe_luma_row(clip: VideoNode, **crop: Any) -> VideoNode:
+def wipe_luma_row(clip: vs.VideoNode, **crop: Any) -> vs.VideoNode:
     planes = split(clip)
 
     planes[0] = planes[0].std.Crop(**crop).std.AddBorders(**crop)
 
     return join(planes)
 
 
@@ -1489,22 +1516,22 @@
     top: int = 0
     bottom: int = 0
     left: int = 0
     right: int = 0
 
 
 def crop(
-    epis: VideoNode,
+    epis: vs.VideoNode,
     zone: str = "",
     **override: Any,
-) -> tuple[VideoNode, VideoFunc1]:
+) -> tuple[vs.VideoNode, VideoFunc]:
     """Crop wrapper."""
 
-    def _crop(epis: VideoNode) -> VideoNode:
-        return core.std.CropRel(
+    def _crop(epis: vs.VideoNode) -> vs.VideoNode:
+        return vs.core.std.CropRel(
             epis,
             top=crset.top,
             bottom=crset.bottom,
             left=crset.left,
             right=crset.right,
         )
 
@@ -1512,115 +1539,115 @@
     crset = override_dc(crset, block="crop", zone=zone, **override)
 
     epis = _crop(epis)
 
     return (epis, _crop)
 
 
-def to60fps_mv(clip: VideoNode) -> VideoNode:
+def to60fps_mv(clip: vs.VideoNode) -> vs.VideoNode:
     """http://avisynth.org.ru/mvtools/mvtools2.html."""
-    sup = core.mv.Super(clip, pel=2, sharp=2, rfilter=4)
-    bvec = core.mv.Analyse(
+    sup = vs.core.mv.Super(clip, pel=2, sharp=2, rfilter=4)
+    bvec = vs.core.mv.Analyse(
         sup,
         blksize=8,
         isb=True,
         chroma=True,
         search=3,
         searchparam=1,
         truemotion=True,
         dct=1,
         overlap=4,
     )
-    fvec = core.mv.Analyse(
+    fvec = vs.core.mv.Analyse(
         sup,
         blksize=8,
         isb=False,
         chroma=True,
         search=3,
         searchparam=1,
         truemotion=True,
         dct=1,
         overlap=4,
     )
-    return core.mv.FlowFPS(clip, sup, bvec, fvec, num=60, den=1)
+    return vs.core.mv.FlowFPS(clip, sup, bvec, fvec, num=60, den=1)
 
 
-def to60fps_svp(clip: VideoNode) -> VideoNode:
+def to60fps_svp(clip: vs.VideoNode) -> vs.VideoNode:
     clip_p8 = depth(clip, 8) if get_depth(clip) != 8 else clip
 
     super_params = "{gpu: 1, pel: 2}"
     analyse_params = "{gpu: 1, block: {w:8, overlap:3}, refine: [{thsad:1000, search:{type:3}}]}"
     smoothfps_params = "{rate: {num: 5, den: 2}, algo: 2, gpuid: 0}"  # (24000/1001)*(1001/400)=60
 
-    sup = core.svp1.Super(clip_p8, super_params)
-    vectors = core.svp1.Analyse(sup["clip"], sup["data"], clip_p8, analyse_params)
+    sup = vs.core.svp1.Super(clip_p8, super_params)
+    vectors = vs.core.svp1.Analyse(sup["clip"], sup["data"], clip_p8, analyse_params)
 
-    return core.svp2.SmoothFps(
+    return vs.core.svp2.SmoothFps(
         clip,
         sup["clip"],
         sup["data"],
         vectors["clip"],
         vectors["data"],
         smoothfps_params,
     )
 
 
-def to60fps(clip: VideoNode, mode: str = "svp") -> VideoNode:
+def to60fps(clip: vs.VideoNode, mode: str = "svp") -> vs.VideoNode:
     if mode == "mv":
         return to60fps_mv(clip)
     if mode == "svp":
         return to60fps_svp(clip)
 
     return None
 
 
-def chromashift(clip: VideoNode, cx: int = 0, cy: int = 0) -> VideoNode:
+def chromashift(clip: vs.VideoNode, cx: int = 0, cy: int = 0) -> vs.VideoNode:
     """
     Shift hroma.
 
     cx — Horizontal chroma shift. Positive value shifts chroma to left, negative value shifts chroma to right.
     cy — Vertical chroma shift. Positive value shifts chroma upwards, negative value shifts chroma downwards.
     """
     planes = split(clip)
 
-    planes[1] = core.resize.Spline36(planes[1], src_left=cx, src_top=cy)
-    planes[2] = core.resize.Spline36(planes[2], src_left=cx, src_top=cy)
+    planes[1] = vs.core.resize.Spline36(planes[1], src_left=cx, src_top=cy)
+    planes[2] = vs.core.resize.Spline36(planes[2], src_left=cx, src_top=cy)
 
     return join(planes)
 
 
 def adaptive_chromashift(  # noqa: PLR0915
-    clip: VideoNode,
-    fix: VideoNode,
+    clip: vs.VideoNode,
+    fix: vs.VideoNode,
     pw_mode: int = 0,
-) -> VideoNode:
+) -> vs.VideoNode:
     """Chromashift with comparisons for floating chromashift."""
 
-    def make_diff(clip: VideoNode) -> VideoNode:
+    def make_diff(clip: vs.VideoNode) -> vs.VideoNode:
         from fvsfunc import Downscale444
 
         desc_h = 720
         desc_w = hav.m4((clip.width * desc_h) / clip.height)
         descale = Downscale444(clip, w=desc_w, h=desc_h)
 
         planes_desc = split(descale)
-        y = core.std.Sobel(planes_desc[0])
-        u = core.std.Sobel(planes_desc[1])
-        v = core.std.Sobel(planes_desc[2])
+        y = vs.core.std.Sobel(planes_desc[0])
+        u = vs.core.std.Sobel(planes_desc[1])
+        v = vs.core.std.Sobel(planes_desc[2])
 
-        uv = core.std.Expr([u, v], ["x y max"])
+        uv = vs.core.std.Expr([u, v], ["x y max"])
 
-        return core.std.MakeDiff(y, uv)
+        return vs.core.std.MakeDiff(y, uv)
 
     def frame_diff_eval(
         n: int,
-        f: VideoFrame,
-        f1: VideoNode,
-        f2: VideoNode,
-    ) -> VideoNode:
+        f: vs.VideoFrame,
+        f1: vs.VideoNode,
+        f2: vs.VideoNode,
+    ) -> vs.VideoNode:
         c0 = f[1].props.PlaneStatsAverage > f[0].props.PlaneStatsAverage
         p1 = f[3].props.PlaneStatsAverage > f[2].props.PlaneStatsAverage
         n1 = f[5].props.PlaneStatsAverage > f[4].props.PlaneStatsAverage
         p2 = f[7].props.PlaneStatsAverage > f[6].props.PlaneStatsAverage
         n2 = f[9].props.PlaneStatsAverage > f[8].props.PlaneStatsAverage
         p3 = f[11].props.PlaneStatsAverage > f[10].props.PlaneStatsAverage
         n3 = f[13].props.PlaneStatsAverage > f[12].props.PlaneStatsAverage
@@ -1636,68 +1663,68 @@
 
         out = f2 if condition else f1
 
         return add_caption(n=n, f=f, out=out, condition=condition) if pw_mode else out
 
     def add_caption(
         n: int,
-        f: VideoFrame,
-        out: VideoNode,
+        f: vs.VideoFrame,
+        out: vs.VideoNode,
         condition: bool,
-    ) -> VideoNode:
+    ) -> vs.VideoNode:
         lines: list[str] = []
         if pw_mode == 2:
             lines.extend(
                 (
                     f"Frame avg: {f[0].props.PlaneStatsAverage}",
                     f"Frame avg: {f[1].props.PlaneStatsAverage}",
                 ),
             )
         lines.append("fix" if condition else "clip")
 
         style = "Fira Code,20,&H0000FFFF,&H00000000,&H00000000,&H00000000,1,0,0,0,100,100,0,0,1,2,0,7,10,10,10,1"
         return out.sub.Subtitle("\n".join(lines), start=n, end=n + 1, style=style)
 
-    def _adaptive_chromashift(clip: VideoNode, fix: VideoNode) -> VideoNode:
+    def _adaptive_chromashift(clip: vs.VideoNode, fix: vs.VideoNode) -> vs.VideoNode:
         diff_def = make_diff(clip)
         diff_fix = make_diff(fix)
 
-        s0 = core.std.PlaneStats(diff_def)  # curr0
-        s1 = core.std.PlaneStats(diff_fix)  # curr0
-        s2 = core.std.PlaneStats(diff_def).std.DuplicateFrames(0)  # prev1
-        s3 = core.std.PlaneStats(diff_fix).std.DuplicateFrames(0)  # prev1
-        s4 = core.std.PlaneStats(diff_def).std.Trim(1)  # next1
-        s5 = core.std.PlaneStats(diff_fix).std.Trim(1)  # next1
-        s6 = core.std.PlaneStats(diff_def).std.DuplicateFrames([0, 1])  # prev2
-        s7 = core.std.PlaneStats(diff_fix).std.DuplicateFrames([0, 1])  # prev2
-        s8 = core.std.PlaneStats(diff_def).std.Trim(2)  # next2
-        s9 = core.std.PlaneStats(diff_fix).std.Trim(2)  # next2
-        s10 = core.std.PlaneStats(diff_def).std.DuplicateFrames([0, 1, 2])  # prev3
-        s11 = core.std.PlaneStats(diff_fix).std.DuplicateFrames([0, 1, 2])  # prev3
-        s12 = core.std.PlaneStats(diff_def).std.Trim(3)  # next3
-        s13 = core.std.PlaneStats(diff_fix).std.Trim(3)  # next3
+        s0 = vs.core.std.PlaneStats(diff_def)  # curr0
+        s1 = vs.core.std.PlaneStats(diff_fix)  # curr0
+        s2 = vs.core.std.PlaneStats(diff_def).std.DuplicateFrames(0)  # prev1
+        s3 = vs.core.std.PlaneStats(diff_fix).std.DuplicateFrames(0)  # prev1
+        s4 = vs.core.std.PlaneStats(diff_def).std.Trim(1)  # next1
+        s5 = vs.core.std.PlaneStats(diff_fix).std.Trim(1)  # next1
+        s6 = vs.core.std.PlaneStats(diff_def).std.DuplicateFrames([0, 1])  # prev2
+        s7 = vs.core.std.PlaneStats(diff_fix).std.DuplicateFrames([0, 1])  # prev2
+        s8 = vs.core.std.PlaneStats(diff_def).std.Trim(2)  # next2
+        s9 = vs.core.std.PlaneStats(diff_fix).std.Trim(2)  # next2
+        s10 = vs.core.std.PlaneStats(diff_def).std.DuplicateFrames([0, 1, 2])  # prev3
+        s11 = vs.core.std.PlaneStats(diff_fix).std.DuplicateFrames([0, 1, 2])  # prev3
+        s12 = vs.core.std.PlaneStats(diff_def).std.Trim(3)  # next3
+        s13 = vs.core.std.PlaneStats(diff_fix).std.Trim(3)  # next3
 
-        return core.std.FrameEval(
+        return vs.core.std.FrameEval(
             clip=clip,
             eval=partial(frame_diff_eval, f1=clip, f2=fix),
             prop_src=[s0, s1, s2, s3, s4, s5, s6, s7, s8, s9, s10, s11, s12, s13],
         )
 
     return _adaptive_chromashift(clip, fix)
 
 
 def rescale_(
-    clip: VideoNode,
+    clip: vs.VideoNode,
     mode: str = "insane_aa",
-    ref_clip: VideoNode | None = None,
+    ref_clip: vs.VideoNode | None = None,
     width: int = 0,
     height: int = 0,
     zone: str = "",
     **override: Any,
-) -> VideoNode:
+) -> vs.VideoNode:
     """Upcale clip to the new size."""
     if ref_clip is not None:
         dx = ref_clip.width
         dy = ref_clip.height
     elif width and height:
         dx = width
         dy = height
@@ -1733,15 +1760,15 @@
         return clip.jinc.JincResize(dx, dy)
     if mode == "lanczos":
         return clip.resize.Lanczos(dx, dy, filter_param_a=2)
 
     return None
 
 
-def downscale(clip: VideoNode, desc_h: int = 720, to420: bool = False) -> VideoNode:
+def downscale(clip: vs.VideoNode, desc_h: int = 720, to420: bool = False) -> vs.VideoNode:
     """Downcale clip to the new size."""
     if clip.height == desc_h:
         return clip
 
     desc_w = hav.m4((clip.width * desc_h) / clip.height)
 
     if not to420:
@@ -1753,19 +1780,19 @@
     planes[1] = planes[1].resize.Spline36(desc_w / 2, desc_h / 2)
     planes[2] = planes[2].resize.Spline36(desc_w / 2, desc_h / 2)
 
     return join(planes)
 
 
 def rfs_black_crop(
-    clip: VideoNode,
+    clip: vs.VideoNode,
     maps: Maps,
     top: int = 0,
     bot: int = 0,
-) -> VideoNode:
+) -> vs.VideoNode:
     fixed_black = clip.std.CropRel(top=top, bottom=bot).std.AddBorders(top=top, bottom=bot)
 
     return rfs(clip, fixed_black, maps)
 
 
 def get_list(ranges: list[FrameRange]) -> list[int]:
     frames = []
@@ -1776,20 +1803,20 @@
         elif isinstance(x, int):
             frames.append(x)
 
     return frames
 
 
 def pv_diff(
-    tv: VideoNode,
-    bd: VideoNode,
+    tv: vs.VideoNode,
+    bd: vs.VideoNode,
     thr: float = 72,
     name: str = "",
     exclude_ranges: list[FrameRange] | None = None,
-) -> VideoNode:
+) -> vs.VideoNode:
     from lvsfunc import diff
 
     clips = [tv, bd]
     num_frames = [clip.num_frames for clip in clips]
     clips = [clip.std.Trim(0, min(num_frames) - 1) for clip in clips]
 
     comparison, frames = diff(clips[0], clips[1], thr=thr, return_ranges=True)
@@ -1798,12 +1825,12 @@
         frames = [x for x in frames if x not in get_list(exclude_ranges)]
 
     with Path("./diff.txt").open("a") as log:
         if name:
             log.write(f"{name}=")
 
         if frames:
-            log.write(f"{repr(frames)} \n\n")
+            log.write(f"{frames!r} \n\n")
         else:
             log.write("no differences found")
 
     return comparison
```

### Comparing `dnfunc-0.0.3a2/PKG-INFO` & `dnfunc-0.0.4/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,33 +1,37 @@
 Metadata-Version: 2.1
 Name: dnfunc
-Version: 0.0.3a2
-Summary: A collection of Vapoursynth functions and wrapperspoetr
+Version: 0.0.4
+Summary: A collection of Vapoursynth functions and wrappers
 Home-page: https://github.com/DeadNews/dnfunc
 License: MIT
 Keywords: vapoursynth,vapoursynth-functions,video-encoding
 Author: DeadNews
 Author-email: aurczpbgr@mozmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Multimedia :: Video
 Requires-Dist: havsfunc (>=33,<34)
-Requires-Dist: lvsfunc (>=0.7.1,<0.8.0)
+Requires-Dist: lvsfunc (>=0.8.0,<0.9.0)
 Requires-Dist: pyyaml (>=6.0,<7.0)
 Requires-Dist: vapoursynth (>=60)
 Requires-Dist: vstools (>=2.1.0,<3.0.0)
 Requires-Dist: vsutil (>=0.8.0,<0.9.0)
 Project-URL: Repository, https://github.com/DeadNews/dnfunc
 Description-Content-Type: text/markdown
 
 # dnfunc
 
 > A collection of Vapoursynth functions and wrappers
 
 [![PyPI version](https://img.shields.io/pypi/v/dnfunc)](https://pypi.org/project/dnfunc)
-[![CI/CD](https://github.com/DeadNews/dnfunc/actions/workflows/python-vs-app.yml/badge.svg)](https://github.com/DeadNews/dnfunc/actions/workflows/python-vs-app.yml)
+[![Main](https://github.com/DeadNews/dnfunc/actions/workflows/main.yml/badge.svg)](https://github.com/DeadNews/dnfunc/actions/workflows/main.yml)
 [![pre-commit.ci](https://results.pre-commit.ci/badge/github/DeadNews/dnfunc/main.svg)](https://results.pre-commit.ci/latest/github/DeadNews/dnfunc/main)
 
+## Deps
+
+<https://github.com/DeadNews/zsh-scripts/blob/main/src/vs-plugins.zsh>
+
```

