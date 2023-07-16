# Comparing `tmp/ome_types-0.4.0rc3.tar.gz` & `tmp/ome_types-0.4.0rc4.tar.gz`

## Comparing `ome_types-0.4.0rc3.tar` & `ome_types-0.4.0rc4.tar`

### file list

```diff
@@ -1,65 +1,66 @@
--rw-r--r--   0        0        0    16554 2020-02-02 00:00:00.000000 ome_types-0.4.0rc3/CHANGELOG.md
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ome_types-0.4.0rc3/src/ome_autogen/__init__.py
--rw-r--r--   0        0        0       96 2020-02-02 00:00:00.000000 ome_types-0.4.0rc3/src/ome_autogen/__main__.py
--rw-r--r--   0        0        0     2729 2020-02-02 00:00:00.000000 ome_types-0.4.0rc3/src/ome_autogen/_config.py
--rw-r--r--   0        0        0    11409 2020-02-02 00:00:00.000000 ome_types-0.4.0rc3/src/ome_autogen/_generator.py
--rw-r--r--   0        0        0     2469 2020-02-02 00:00:00.000000 ome_types-0.4.0rc3/src/ome_autogen/_transformer.py
--rw-r--r--   0        0        0     2667 2020-02-02 00:00:00.000000 ome_types-0.4.0rc3/src/ome_autogen/_util.py
--rw-r--r--   0        0        0     3411 2020-02-02 00:00:00.000000 ome_types-0.4.0rc3/src/ome_autogen/main.py
--rw-r--r--   0        0        0     2499 2020-02-02 00:00:00.000000 ome_types-0.4.0rc3/src/ome_autogen/templates/class.jinja2
--rw-r--r--   0        0        0      464 2020-02-02 00:00:00.000000 ome_types-0.4.0rc3/src/ome_autogen/templates/docstrings.numpy.jinja2
--rw-r--r--   0        0        0      958 2020-02-02 00:00:00.000000 ome_types-0.4.0rc3/src/ome_autogen/templates/enum.jinja2
--rw-r--r--   0        0        0      919 2020-02-02 00:00:00.000000 ome_types-0.4.0rc3/src/ome_types/__init__.py
--rw-r--r--   0        0        0    17998 2020-02-02 00:00:00.000000 ome_types-0.4.0rc3/src/ome_types/_conversion.py
--rw-r--r--   0        0        0     3746 2020-02-02 00:00:00.000000 ome_types-0.4.0rc3/src/ome_types/_pydantic_compat.py
--rw-r--r--   0        0        0      277 2020-02-02 00:00:00.000000 ome_types-0.4.0rc3/src/ome_types/napari.yaml
--rw-r--r--   0        0        0   285655 2020-02-02 00:00:00.000000 ome_types-0.4.0rc3/src/ome_types/ome-2016-06.xsd
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ome_types-0.4.0rc3/src/ome_types/py.typed
--rw-r--r--   0        0        0     1918 2020-02-02 00:00:00.000000 ome_types-0.4.0rc3/src/ome_types/units.py
--rw-r--r--   0        0        0     6430 2020-02-02 00:00:00.000000 ome_types-0.4.0rc3/src/ome_types/widget.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ome_types-0.4.0rc3/src/ome_types/_mixins/__init__.py
--rw-r--r--   0        0        0     7263 2020-02-02 00:00:00.000000 ome_types-0.4.0rc3/src/ome_types/_mixins/_base_type.py
--rw-r--r--   0        0        0     3460 2020-02-02 00:00:00.000000 ome_types-0.4.0rc3/src/ome_types/_mixins/_ids.py
--rw-r--r--   0        0        0      731 2020-02-02 00:00:00.000000 ome_types-0.4.0rc3/src/ome_types/_mixins/_instrument.py
--rw-r--r--   0        0        0      938 2020-02-02 00:00:00.000000 ome_types-0.4.0rc3/src/ome_types/_mixins/_kinded.py
--rw-r--r--   0        0        0     3268 2020-02-02 00:00:00.000000 ome_types-0.4.0rc3/src/ome_types/_mixins/_ome.py
--rw-r--r--   0        0        0      828 2020-02-02 00:00:00.000000 ome_types-0.4.0rc3/src/ome_types/_mixins/_reference.py
--rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 ome_types-0.4.0rc3/src/ome_types/_mixins/_util.py
--rw-r--r--   0        0        0     3351 2020-02-02 00:00:00.000000 ome_types-0.4.0rc3/src/ome_types/_mixins/_validators.py
--rw-r--r--   0        0        0      576 2020-02-02 00:00:00.000000 ome_types-0.4.0rc3/src/ome_types/_vendor/__init__.py
--rw-r--r--   0        0        0    16940 2020-02-02 00:00:00.000000 ome_types-0.4.0rc3/src/ome_types/_vendor/_pydantic_color_v1.py
--rw-r--r--   0        0        0    21521 2020-02-02 00:00:00.000000 ome_types-0.4.0rc3/src/ome_types/_vendor/_pydantic_color_v2.py
--rw-r--r--   0        0        0     3034 2020-02-02 00:00:00.000000 ome_types-0.4.0rc3/src/ome_types/model/__init__.py
--rw-r--r--   0        0        0     1222 2020-02-02 00:00:00.000000 ome_types-0.4.0rc3/src/ome_types/model/_color.py
--rw-r--r--   0        0        0     1198 2020-02-02 00:00:00.000000 ome_types-0.4.0rc3/src/ome_types/model/_converters.py
--rw-r--r--   0        0        0     5954 2020-02-02 00:00:00.000000 ome_types-0.4.0rc3/src/ome_types/model/_shape_union.py
--rw-r--r--   0        0        0     6423 2020-02-02 00:00:00.000000 ome_types-0.4.0rc3/src/ome_types/model/_structured_annotations.py
--rw-r--r--   0        0        0     1671 2020-02-02 00:00:00.000000 ome_types-0.4.0rc3/src/ome_types/model/_user_sequence.py
--rw-r--r--   0        0        0     2396 2020-02-02 00:00:00.000000 ome_types-0.4.0rc3/src/ome_types/model/simple_types.py
--rw-r--r--   0        0        0    51712 2020-02-02 00:00:00.000000 ome_types-0.4.0rc3/src/ome_types/transforms/2003-FC-to-2008-09.xsl
--rw-r--r--   0        0        0    33502 2020-02-02 00:00:00.000000 ome_types-0.4.0rc3/src/ome_types/transforms/2007-06-to-2008-09.xsl
--rw-r--r--   0        0        0    31797 2020-02-02 00:00:00.000000 ome_types-0.4.0rc3/src/ome_types/transforms/2008-02-to-2008-09.xsl
--rw-r--r--   0        0        0    67202 2020-02-02 00:00:00.000000 ome_types-0.4.0rc3/src/ome_types/transforms/2008-09-to-2009-09.xsl
--rw-r--r--   0        0        0    18678 2020-02-02 00:00:00.000000 ome_types-0.4.0rc3/src/ome_types/transforms/2009-09-to-2010-04.xsl
--rw-r--r--   0        0        0    10744 2020-02-02 00:00:00.000000 ome_types-0.4.0rc3/src/ome_types/transforms/2010-04-to-2010-06.xsl
--rw-r--r--   0        0        0     8562 2020-02-02 00:00:00.000000 ome_types-0.4.0rc3/src/ome_types/transforms/2010-06-to-2011-06.xsl
--rw-r--r--   0        0        0    21773 2020-02-02 00:00:00.000000 ome_types-0.4.0rc3/src/ome_types/transforms/2011-06-to-2012-06.xsl
--rw-r--r--   0        0        0     5123 2020-02-02 00:00:00.000000 ome_types-0.4.0rc3/src/ome_types/transforms/2012-06-to-2013-06.xsl
--rw-r--r--   0        0        0     6706 2020-02-02 00:00:00.000000 ome_types-0.4.0rc3/src/ome_types/transforms/2013-06-to-2015-01.xsl
--rw-r--r--   0        0        0     9282 2020-02-02 00:00:00.000000 ome_types-0.4.0rc3/src/ome_types/transforms/2015-01-to-2016-06.xsl
--rw-r--r--   0        0        0      189 2020-02-02 00:00:00.000000 ome_types-0.4.0rc3/src/xsdata_pydantic_basemodel/__init__.py
--rw-r--r--   0        0        0     5484 2020-02-02 00:00:00.000000 ome_types-0.4.0rc3/src/xsdata_pydantic_basemodel/bindings.py
--rw-r--r--   0        0        0     4487 2020-02-02 00:00:00.000000 ome_types-0.4.0rc3/src/xsdata_pydantic_basemodel/compat.py
--rw-r--r--   0        0        0      702 2020-02-02 00:00:00.000000 ome_types-0.4.0rc3/src/xsdata_pydantic_basemodel/config.py
--rw-r--r--   0        0        0     4581 2020-02-02 00:00:00.000000 ome_types-0.4.0rc3/src/xsdata_pydantic_basemodel/generator.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ome_types-0.4.0rc3/src/xsdata_pydantic_basemodel/py.typed
--rw-r--r--   0        0        0     4268 2020-02-02 00:00:00.000000 ome_types-0.4.0rc3/src/xsdata_pydantic_basemodel/pydantic_compat.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ome_types-0.4.0rc3/src/xsdata_pydantic_basemodel/hooks/__init__.py
--rw-r--r--   0        0        0      185 2020-02-02 00:00:00.000000 ome_types-0.4.0rc3/src/xsdata_pydantic_basemodel/hooks/class_type.py
--rw-r--r--   0        0        0      192 2020-02-02 00:00:00.000000 ome_types-0.4.0rc3/src/xsdata_pydantic_basemodel/hooks/cli.py
--rw-r--r--   0        0        0     1345 2020-02-02 00:00:00.000000 ome_types-0.4.0rc3/.gitignore
--rw-r--r--   0        0        0     1071 2020-02-02 00:00:00.000000 ome_types-0.4.0rc3/LICENSE
--rw-r--r--   0        0        0     8082 2020-02-02 00:00:00.000000 ome_types-0.4.0rc3/README.md
--rw-r--r--   0        0        0      492 2020-02-02 00:00:00.000000 ome_types-0.4.0rc3/hatch_build.py
--rw-r--r--   0        0        0     6397 2020-02-02 00:00:00.000000 ome_types-0.4.0rc3/pyproject.toml
--rw-r--r--   0        0        0    10335 2020-02-02 00:00:00.000000 ome_types-0.4.0rc3/PKG-INFO
+-rw-r--r--   0        0        0    23306 2020-02-02 00:00:00.000000 ome_types-0.4.0rc4/CHANGELOG.md
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ome_types-0.4.0rc4/src/ome_autogen/__init__.py
+-rw-r--r--   0        0        0       96 2020-02-02 00:00:00.000000 ome_types-0.4.0rc4/src/ome_autogen/__main__.py
+-rw-r--r--   0        0        0     2729 2020-02-02 00:00:00.000000 ome_types-0.4.0rc4/src/ome_autogen/_config.py
+-rw-r--r--   0        0        0    11409 2020-02-02 00:00:00.000000 ome_types-0.4.0rc4/src/ome_autogen/_generator.py
+-rw-r--r--   0        0        0     2469 2020-02-02 00:00:00.000000 ome_types-0.4.0rc4/src/ome_autogen/_transformer.py
+-rw-r--r--   0        0        0     2667 2020-02-02 00:00:00.000000 ome_types-0.4.0rc4/src/ome_autogen/_util.py
+-rw-r--r--   0        0        0     3411 2020-02-02 00:00:00.000000 ome_types-0.4.0rc4/src/ome_autogen/main.py
+-rw-r--r--   0        0        0     2499 2020-02-02 00:00:00.000000 ome_types-0.4.0rc4/src/ome_autogen/templates/class.jinja2
+-rw-r--r--   0        0        0      464 2020-02-02 00:00:00.000000 ome_types-0.4.0rc4/src/ome_autogen/templates/docstrings.numpy.jinja2
+-rw-r--r--   0        0        0      958 2020-02-02 00:00:00.000000 ome_types-0.4.0rc4/src/ome_autogen/templates/enum.jinja2
+-rw-r--r--   0        0        0      919 2020-02-02 00:00:00.000000 ome_types-0.4.0rc4/src/ome_types/__init__.py
+-rw-r--r--   0        0        0    19822 2020-02-02 00:00:00.000000 ome_types-0.4.0rc4/src/ome_types/_conversion.py
+-rw-r--r--   0        0        0     3746 2020-02-02 00:00:00.000000 ome_types-0.4.0rc4/src/ome_types/_pydantic_compat.py
+-rw-r--r--   0        0        0     1705 2020-02-02 00:00:00.000000 ome_types-0.4.0rc4/src/ome_types/etree_fixes.py
+-rw-r--r--   0        0        0      277 2020-02-02 00:00:00.000000 ome_types-0.4.0rc4/src/ome_types/napari.yaml
+-rw-r--r--   0        0        0   285655 2020-02-02 00:00:00.000000 ome_types-0.4.0rc4/src/ome_types/ome-2016-06.xsd
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ome_types-0.4.0rc4/src/ome_types/py.typed
+-rw-r--r--   0        0        0     1918 2020-02-02 00:00:00.000000 ome_types-0.4.0rc4/src/ome_types/units.py
+-rw-r--r--   0        0        0     6430 2020-02-02 00:00:00.000000 ome_types-0.4.0rc4/src/ome_types/widget.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ome_types-0.4.0rc4/src/ome_types/_mixins/__init__.py
+-rw-r--r--   0        0        0     7263 2020-02-02 00:00:00.000000 ome_types-0.4.0rc4/src/ome_types/_mixins/_base_type.py
+-rw-r--r--   0        0        0     3460 2020-02-02 00:00:00.000000 ome_types-0.4.0rc4/src/ome_types/_mixins/_ids.py
+-rw-r--r--   0        0        0      731 2020-02-02 00:00:00.000000 ome_types-0.4.0rc4/src/ome_types/_mixins/_instrument.py
+-rw-r--r--   0        0        0      938 2020-02-02 00:00:00.000000 ome_types-0.4.0rc4/src/ome_types/_mixins/_kinded.py
+-rw-r--r--   0        0        0     3268 2020-02-02 00:00:00.000000 ome_types-0.4.0rc4/src/ome_types/_mixins/_ome.py
+-rw-r--r--   0        0        0      828 2020-02-02 00:00:00.000000 ome_types-0.4.0rc4/src/ome_types/_mixins/_reference.py
+-rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 ome_types-0.4.0rc4/src/ome_types/_mixins/_util.py
+-rw-r--r--   0        0        0     3351 2020-02-02 00:00:00.000000 ome_types-0.4.0rc4/src/ome_types/_mixins/_validators.py
+-rw-r--r--   0        0        0      576 2020-02-02 00:00:00.000000 ome_types-0.4.0rc4/src/ome_types/_vendor/__init__.py
+-rw-r--r--   0        0        0    16940 2020-02-02 00:00:00.000000 ome_types-0.4.0rc4/src/ome_types/_vendor/_pydantic_color_v1.py
+-rw-r--r--   0        0        0    21521 2020-02-02 00:00:00.000000 ome_types-0.4.0rc4/src/ome_types/_vendor/_pydantic_color_v2.py
+-rw-r--r--   0        0        0     3034 2020-02-02 00:00:00.000000 ome_types-0.4.0rc4/src/ome_types/model/__init__.py
+-rw-r--r--   0        0        0     1222 2020-02-02 00:00:00.000000 ome_types-0.4.0rc4/src/ome_types/model/_color.py
+-rw-r--r--   0        0        0     1198 2020-02-02 00:00:00.000000 ome_types-0.4.0rc4/src/ome_types/model/_converters.py
+-rw-r--r--   0        0        0     5954 2020-02-02 00:00:00.000000 ome_types-0.4.0rc4/src/ome_types/model/_shape_union.py
+-rw-r--r--   0        0        0     6423 2020-02-02 00:00:00.000000 ome_types-0.4.0rc4/src/ome_types/model/_structured_annotations.py
+-rw-r--r--   0        0        0     1671 2020-02-02 00:00:00.000000 ome_types-0.4.0rc4/src/ome_types/model/_user_sequence.py
+-rw-r--r--   0        0        0     2396 2020-02-02 00:00:00.000000 ome_types-0.4.0rc4/src/ome_types/model/simple_types.py
+-rw-r--r--   0        0        0    51712 2020-02-02 00:00:00.000000 ome_types-0.4.0rc4/src/ome_types/transforms/2003-FC-to-2008-09.xsl
+-rw-r--r--   0        0        0    33502 2020-02-02 00:00:00.000000 ome_types-0.4.0rc4/src/ome_types/transforms/2007-06-to-2008-09.xsl
+-rw-r--r--   0        0        0    31797 2020-02-02 00:00:00.000000 ome_types-0.4.0rc4/src/ome_types/transforms/2008-02-to-2008-09.xsl
+-rw-r--r--   0        0        0    67202 2020-02-02 00:00:00.000000 ome_types-0.4.0rc4/src/ome_types/transforms/2008-09-to-2009-09.xsl
+-rw-r--r--   0        0        0    18678 2020-02-02 00:00:00.000000 ome_types-0.4.0rc4/src/ome_types/transforms/2009-09-to-2010-04.xsl
+-rw-r--r--   0        0        0    10744 2020-02-02 00:00:00.000000 ome_types-0.4.0rc4/src/ome_types/transforms/2010-04-to-2010-06.xsl
+-rw-r--r--   0        0        0     8562 2020-02-02 00:00:00.000000 ome_types-0.4.0rc4/src/ome_types/transforms/2010-06-to-2011-06.xsl
+-rw-r--r--   0        0        0    21773 2020-02-02 00:00:00.000000 ome_types-0.4.0rc4/src/ome_types/transforms/2011-06-to-2012-06.xsl
+-rw-r--r--   0        0        0     5123 2020-02-02 00:00:00.000000 ome_types-0.4.0rc4/src/ome_types/transforms/2012-06-to-2013-06.xsl
+-rw-r--r--   0        0        0     6706 2020-02-02 00:00:00.000000 ome_types-0.4.0rc4/src/ome_types/transforms/2013-06-to-2015-01.xsl
+-rw-r--r--   0        0        0     9282 2020-02-02 00:00:00.000000 ome_types-0.4.0rc4/src/ome_types/transforms/2015-01-to-2016-06.xsl
+-rw-r--r--   0        0        0      189 2020-02-02 00:00:00.000000 ome_types-0.4.0rc4/src/xsdata_pydantic_basemodel/__init__.py
+-rw-r--r--   0        0        0     5484 2020-02-02 00:00:00.000000 ome_types-0.4.0rc4/src/xsdata_pydantic_basemodel/bindings.py
+-rw-r--r--   0        0        0     4487 2020-02-02 00:00:00.000000 ome_types-0.4.0rc4/src/xsdata_pydantic_basemodel/compat.py
+-rw-r--r--   0        0        0      702 2020-02-02 00:00:00.000000 ome_types-0.4.0rc4/src/xsdata_pydantic_basemodel/config.py
+-rw-r--r--   0        0        0     4581 2020-02-02 00:00:00.000000 ome_types-0.4.0rc4/src/xsdata_pydantic_basemodel/generator.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ome_types-0.4.0rc4/src/xsdata_pydantic_basemodel/py.typed
+-rw-r--r--   0        0        0     4268 2020-02-02 00:00:00.000000 ome_types-0.4.0rc4/src/xsdata_pydantic_basemodel/pydantic_compat.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ome_types-0.4.0rc4/src/xsdata_pydantic_basemodel/hooks/__init__.py
+-rw-r--r--   0        0        0      185 2020-02-02 00:00:00.000000 ome_types-0.4.0rc4/src/xsdata_pydantic_basemodel/hooks/class_type.py
+-rw-r--r--   0        0        0      192 2020-02-02 00:00:00.000000 ome_types-0.4.0rc4/src/xsdata_pydantic_basemodel/hooks/cli.py
+-rw-r--r--   0        0        0     1345 2020-02-02 00:00:00.000000 ome_types-0.4.0rc4/.gitignore
+-rw-r--r--   0        0        0     1071 2020-02-02 00:00:00.000000 ome_types-0.4.0rc4/LICENSE
+-rw-r--r--   0        0        0     8082 2020-02-02 00:00:00.000000 ome_types-0.4.0rc4/README.md
+-rw-r--r--   0        0        0      492 2020-02-02 00:00:00.000000 ome_types-0.4.0rc4/hatch_build.py
+-rw-r--r--   0        0        0     6397 2020-02-02 00:00:00.000000 ome_types-0.4.0rc4/pyproject.toml
+-rw-r--r--   0        0        0    10335 2020-02-02 00:00:00.000000 ome_types-0.4.0rc4/PKG-INFO
```

### Comparing `ome_types-0.4.0rc3/CHANGELOG.md` & `ome_types-0.4.0rc4/CHANGELOG.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,12 +1,136 @@
 # Changelog
 
-## [0.3.4](https://github.com/tlambert03/ome-types/tree/0.3.4) (2023-04-06)
+## [v0.4.0](https://github.com/tlambert03/ome-types/tree/v0.4.0) (2023-07-16)
 
-[Full Changelog](https://github.com/tlambert03/ome-types/compare/v0.3.3...0.3.4)
+[Full Changelog](https://github.com/tlambert03/ome-types/compare/v0.4.0rc3...v0.4.0)
+
+**Implemented enhancements:**
+
+- feat: catch and fix lowercase 'ome' in schemas [\#209](https://github.com/tlambert03/ome-types/pull/209) ([tlambert03](https://github.com/tlambert03))
+- feat: add transformations to from\_xml [\#208](https://github.com/tlambert03/ome-types/pull/208) ([tlambert03](https://github.com/tlambert03))
+
+## [v0.4.0rc3](https://github.com/tlambert03/ome-types/tree/v0.4.0rc3) (2023-07-14)
+
+[Full Changelog](https://github.com/tlambert03/ome-types/compare/v0.4.0rc2...v0.4.0rc3)
+
+**Implemented enhancements:**
+
+- feat: add back napari plugin [\#207](https://github.com/tlambert03/ome-types/pull/207) ([tlambert03](https://github.com/tlambert03))
+- feat: support pydantic2 [\#205](https://github.com/tlambert03/ome-types/pull/205) ([tlambert03](https://github.com/tlambert03))
+
+**Merged pull requests:**
+
+- build: remove pydantic-extra-types dep [\#206](https://github.com/tlambert03/ome-types/pull/206) ([tlambert03](https://github.com/tlambert03))
+
+## [v0.4.0rc2](https://github.com/tlambert03/ome-types/tree/v0.4.0rc2) (2023-07-12)
+
+[Full Changelog](https://github.com/tlambert03/ome-types/compare/v0.4.0rc1...v0.4.0rc2)
+
+**Implemented enhancements:**
+
+- feat: add `numpy_dtype` property to PixelType [\#202](https://github.com/tlambert03/ome-types/pull/202) ([tlambert03](https://github.com/tlambert03))
+- feat: to\_etree\_element [\#201](https://github.com/tlambert03/ome-types/pull/201) ([tlambert03](https://github.com/tlambert03))
+- feat: transform old schema [\#199](https://github.com/tlambert03/ome-types/pull/199) ([tlambert03](https://github.com/tlambert03))
+- feat: add 'kind' field to dict output for various subclasses that are otherwise identical [\#185](https://github.com/tlambert03/ome-types/pull/185) ([tlambert03](https://github.com/tlambert03))
+
+**Fixed bugs:**
+
+- fix: fix missing set values in xml output [\#204](https://github.com/tlambert03/ome-types/pull/204) ([tlambert03](https://github.com/tlambert03))
+
+**Tests & CI:**
+
+- ci: add codspeed benchmarks [\#200](https://github.com/tlambert03/ome-types/pull/200) ([tlambert03](https://github.com/tlambert03))
+- test: test for bad dates [\#198](https://github.com/tlambert03/ome-types/pull/198) ([tlambert03](https://github.com/tlambert03))
+- ci: fixing built branch [\#197](https://github.com/tlambert03/ome-types/pull/197) ([tlambert03](https://github.com/tlambert03))
+
+**Merged pull requests:**
+
+- docs: add migration guide for v0.4.0 [\#203](https://github.com/tlambert03/ome-types/pull/203) ([tlambert03](https://github.com/tlambert03))
+
+## [v0.4.0rc1](https://github.com/tlambert03/ome-types/tree/v0.4.0rc1) (2023-07-08)
+
+[Full Changelog](https://github.com/tlambert03/ome-types/compare/v0.4.0a5...v0.4.0rc1)
+
+**Implemented enhancements:**
+
+- feat: complete rewrite, using xsdata instead of xmlschema [\#176](https://github.com/tlambert03/ome-types/pull/176) ([tlambert03](https://github.com/tlambert03))
+
+**Fixed bugs:**
+
+- fix: Move deprecated init kwargs to proper fields [\#194](https://github.com/tlambert03/ome-types/pull/194) ([tlambert03](https://github.com/tlambert03))
+- fix: Fix colors [\#190](https://github.com/tlambert03/ome-types/pull/190) ([tlambert03](https://github.com/tlambert03))
+
+**Tests & CI:**
+
+- ci: coverage changes [\#195](https://github.com/tlambert03/ome-types/pull/195) ([tlambert03](https://github.com/tlambert03))
+- test: rearranging tests [\#192](https://github.com/tlambert03/ome-types/pull/192) ([tlambert03](https://github.com/tlambert03))
+- test: more omero-cli tests [\#191](https://github.com/tlambert03/ome-types/pull/191) ([tlambert03](https://github.com/tlambert03))
+- test: add nd2 test [\#188](https://github.com/tlambert03/ome-types/pull/188) ([tlambert03](https://github.com/tlambert03))
+- test: Omero-cli-transfer test [\#187](https://github.com/tlambert03/ome-types/pull/187) ([tlambert03](https://github.com/tlambert03))
+
+**Merged pull requests:**
+
+- build: make pint and lxml optional deps [\#196](https://github.com/tlambert03/ome-types/pull/196) ([tlambert03](https://github.com/tlambert03))
+- docs: updating docs [\#193](https://github.com/tlambert03/ome-types/pull/193) ([tlambert03](https://github.com/tlambert03))
+- build: add back py37 support [\#189](https://github.com/tlambert03/ome-types/pull/189) ([tlambert03](https://github.com/tlambert03))
+
+## [v0.4.0a5](https://github.com/tlambert03/ome-types/tree/v0.4.0a5) (2023-07-06)
+
+[Full Changelog](https://github.com/tlambert03/ome-types/compare/v0.4.0a4...v0.4.0a5)
+
+## [v0.4.0a4](https://github.com/tlambert03/ome-types/tree/v0.4.0a4) (2023-07-05)
+
+[Full Changelog](https://github.com/tlambert03/ome-types/compare/v0.4.0a3...v0.4.0a4)
+
+**Implemented enhancements:**
+
+- feat: better rich\_repr [\#181](https://github.com/tlambert03/ome-types/pull/181) ([tlambert03](https://github.com/tlambert03))
+
+**Fixed bugs:**
+
+- fix: better sequence for structured annotations [\#186](https://github.com/tlambert03/ome-types/pull/186) ([tlambert03](https://github.com/tlambert03))
+- fix: fix metadata only [\#184](https://github.com/tlambert03/ome-types/pull/184) ([tlambert03](https://github.com/tlambert03))
+- fix: use date time instead of xsdata XMLDateTime [\#182](https://github.com/tlambert03/ome-types/pull/182) ([tlambert03](https://github.com/tlambert03))
+
+## [v0.4.0a3](https://github.com/tlambert03/ome-types/tree/v0.4.0a3) (2023-07-04)
+
+[Full Changelog](https://github.com/tlambert03/ome-types/compare/v0.4.0a2...v0.4.0a3)
+
+**Fixed bugs:**
+
+- fix: more robust id conversion [\#180](https://github.com/tlambert03/ome-types/pull/180) ([tlambert03](https://github.com/tlambert03))
+
+**Tests & CI:**
+
+- test: add typing tests [\#178](https://github.com/tlambert03/ome-types/pull/178) ([tlambert03](https://github.com/tlambert03))
+
+## [v0.4.0a2](https://github.com/tlambert03/ome-types/tree/v0.4.0a2) (2023-07-03)
+
+[Full Changelog](https://github.com/tlambert03/ome-types/compare/v0.4.0a1...v0.4.0a2)
+
+**Tests & CI:**
+
+- test: add more tests [\#177](https://github.com/tlambert03/ome-types/pull/177) ([tlambert03](https://github.com/tlambert03))
+
+## [v0.4.0a1](https://github.com/tlambert03/ome-types/tree/v0.4.0a1) (2023-07-02)
+
+[Full Changelog](https://github.com/tlambert03/ome-types/compare/ruff-panic...v0.4.0a1)
+
+**Merged pull requests:**
+
+- ci\(pre-commit.ci\): autoupdate [\#172](https://github.com/tlambert03/ome-types/pull/172) ([pre-commit-ci[bot]](https://github.com/apps/pre-commit-ci))
+
+## [ruff-panic](https://github.com/tlambert03/ome-types/tree/ruff-panic) (2023-06-20)
+
+[Full Changelog](https://github.com/tlambert03/ome-types/compare/v0.3.4...ruff-panic)
+
+## [v0.3.4](https://github.com/tlambert03/ome-types/tree/v0.3.4) (2023-04-06)
+
+[Full Changelog](https://github.com/tlambert03/ome-types/compare/v0.3.3...v0.3.4)
 
 **Implemented enhancements:**
 
 - feat: make lxml optional \(but don't yet remove from requirements\) [\#166](https://github.com/tlambert03/ome-types/pull/166) ([tlambert03](https://github.com/tlambert03))
 
 **Fixed bugs:**
```

### Comparing `ome_types-0.4.0rc3/src/ome_autogen/_config.py` & `ome_types-0.4.0rc4/src/ome_autogen/_config.py`

 * *Files identical despite different names*

### Comparing `ome_types-0.4.0rc3/src/ome_autogen/_generator.py` & `ome_types-0.4.0rc4/src/ome_autogen/_generator.py`

 * *Files identical despite different names*

### Comparing `ome_types-0.4.0rc3/src/ome_autogen/_transformer.py` & `ome_types-0.4.0rc4/src/ome_autogen/_transformer.py`

 * *Files identical despite different names*

### Comparing `ome_types-0.4.0rc3/src/ome_autogen/_util.py` & `ome_types-0.4.0rc4/src/ome_autogen/_util.py`

 * *Files identical despite different names*

### Comparing `ome_types-0.4.0rc3/src/ome_autogen/main.py` & `ome_types-0.4.0rc4/src/ome_autogen/main.py`

 * *Files identical despite different names*

### Comparing `ome_types-0.4.0rc3/src/ome_autogen/templates/class.jinja2` & `ome_types-0.4.0rc4/src/ome_autogen/templates/class.jinja2`

 * *Files identical despite different names*

### Comparing `ome_types-0.4.0rc3/src/ome_autogen/templates/enum.jinja2` & `ome_types-0.4.0rc4/src/ome_autogen/templates/enum.jinja2`

 * *Files identical despite different names*

### Comparing `ome_types-0.4.0rc3/src/ome_types/__init__.py` & `ome_types-0.4.0rc4/src/ome_types/__init__.py`

 * *Files identical despite different names*

### Comparing `ome_types-0.4.0rc3/src/ome_types/_conversion.py` & `ome_types-0.4.0rc4/src/ome_types/_conversion.py`

 * *Files 13% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 import operator
 import os
 import warnings
 from contextlib import nullcontext, suppress
 from functools import lru_cache
 from pathlib import Path
 from struct import Struct
-from typing import TYPE_CHECKING, cast, overload
+from typing import TYPE_CHECKING, Callable, Iterable, cast, overload
 
 from pydantic import BaseModel
 from xsdata.formats.dataclass.parsers.config import ParserConfig
 
 from ome_types._pydantic_compat import model_dump
 from xsdata_pydantic_basemodel.bindings import (
     SerializerConfig,
@@ -24,27 +24,31 @@
     from lxml import etree as ET
 except ImportError:  # pragma: no cover
     from xml.etree import ElementTree as ET  # type: ignore[no-redef]
 
 
 if TYPE_CHECKING:
     from typing import Any, BinaryIO, ContextManager, TypedDict
+    from xml.etree import ElementTree
 
     import xmlschema
     from lxml.etree import _XSLTResultTree
     from typing_extensions import Literal
     from xsdata.formats.dataclass.parsers.mixins import XmlHandler
 
     from ome_types._mixins._base_type import OMEType
     from ome_types.model import OME
     from xsdata_pydantic_basemodel.bindings import XmlContext
 
-    XMLSource = Path | str | bytes | io.BytesIO
+    AnyElement = ET._Element | ElementTree.Element
+    AnyElementTree = ElementTree.ElementTree | ET._ElementTree
+    ElementOrTree = AnyElement | AnyElementTree
+    TransformationCallable = Callable[[AnyElementTree], AnyElementTree]
+    XMLSource = Path | str | bytes | BinaryIO
     FileLike = str | io.BufferedIOBase
-    ElementOrTree = ET._Element | ET._ElementTree
 
     class ParserKwargs(TypedDict, total=False):
         config: ParserConfig
         context: XmlContext
         handler: type[XmlHandler]
 
 
@@ -58,15 +62,16 @@
 
 def from_xml(
     source: XMLSource,
     *,
     validate: bool | None = None,
     parser: Any = None,
     parser_kwargs: ParserKwargs | None = None,
-    warn_on_transform: bool = False,
+    transformations: Iterable[TransformationCallable] = (),
+    warn_on_schema_update: bool = False,
 ) -> OME:  #  Not totally true, see note below
     """Generate an OME object from an XML document.
 
     NOTE: Technically, this can return any ome-types instance, (not just OME) but it's
     by far the most common type that will come out of this function, and the type
     annotation will be more useful to most users. For those who pass in an xml document
     that isn't just a root <OME> tag, they can cast the result to the correct type
@@ -83,15 +88,20 @@
         If None, validation will be skipped if lxml is not available,
         and will be performed otherwise.
     parser : Any
         Ignored, but kept for backwards compatibility.
     parser_kwargs : ParserKwargs | None
         Passed to the XmlParser constructor. If None, a default parser
         will be used.
-    warn_on_transform : bool
+    transformations: Iterable[TransformationCallable]
+        A sequence of functions that take an ElementTree and return an ElementTree.
+        These will be applied sequentially to the XML document before parsing.
+        Can be used to apply custom transformations or fixes to the XML document
+        before parsing.
+    warn_on_schema_update : bool
         Whether to warn if a transformation was applied to bring the document to
         OME-2016-06.
 
     Returns
     -------
     OME
         The OME object parsed from the XML document. (See NOTE above.)
@@ -102,20 +112,27 @@
             "lxml will be used if available in the environment, but you can "
             "drop this keyword argument.",
             DeprecationWarning,
             stacklevel=2,
         )
 
     if validate:
-        xml_2016 = validate_xml(source, warn_on_transform=warn_on_transform)
+        xml_2016 = validate_xml(source, warn_on_schema_update=warn_on_schema_update)
     else:
         xml_2016 = ensure_2016(
-            source, warn_on_transform=warn_on_transform, as_tree=True
+            source, warn_on_schema_update=warn_on_schema_update, as_tree=True
         )
 
+    for transform in transformations:
+        tree_out = transform(xml_2016)
+        if tree_out is not None:
+            xml_2016 = tree_out
+        else:
+            warnings.warn("Transformation returned None, skipping", stacklevel=2)
+
     OME_type = _get_root_ome_type(xml_2016)
     parser = XmlParser(**(parser_kwargs or {}))
     return parser.parse(xml_2016, OME_type)
 
 
 # ------------------------
 
@@ -309,56 +326,59 @@
 
 
 class ValidationError(ValueError):
     ...
 
 
 def validate_xml(
-    xml: XMLSource, schema: Path | str | None = None, *, warn_on_transform: bool = True
-) -> ET._ElementTree:
+    xml: XMLSource,
+    schema: Path | str | None = None,
+    *,
+    warn_on_schema_update: bool = True,
+) -> AnyElementTree:
     """Validate XML against an XML Schema.
 
     By default, will validate against the OME 2016-06 schema.
     """
     with suppress(ImportError):
-        return validate_xml_with_lxml(xml, schema, warn_on_transform)
+        return validate_xml_with_lxml(xml, schema, warn_on_schema_update)
 
     with suppress(ImportError):  # pragma: no cover
-        return validate_xml_with_xmlschema(xml, schema, warn_on_transform)
+        return validate_xml_with_xmlschema(xml, schema, warn_on_schema_update)
 
     raise ImportError(  # pragma: no cover
         "Validation requires either `lxml` or `xmlschema`. "
         "Please pip install one of them."
     ) from None
 
 
 def validate_xml_with_lxml(
-    xml: XMLSource, schema: Path | str | None = None, warn_on_transform: bool = True
-) -> ET._ElementTree:
+    xml: XMLSource, schema: Path | str | None = None, warn_on_schema_update: bool = True
+) -> AnyElementTree:
     """Validate XML against an XML Schema using lxml."""
     from lxml import etree
 
-    tree = ensure_2016(xml, warn_on_transform=warn_on_transform, as_tree=True)
+    tree = ensure_2016(xml, warn_on_schema_update=warn_on_schema_update, as_tree=True)
     xmlschema = etree.XMLSchema(etree.parse(schema or OME_2016_06_XSD))
 
-    if not xmlschema.validate(tree):
+    if not xmlschema.validate(cast("ET._ElementTree", tree)):
         msg = f"Validation of {str(xml)[:20]!r} failed:"
         for error in xmlschema.error_log:
             msg += f"\n  - line {error.line}: {error.message}"
         raise ValidationError(msg)
     return tree
 
 
 def validate_xml_with_xmlschema(
-    xml: XMLSource, schema: Path | str | None = None, warn_on_transform: bool = True
-) -> ET._ElementTree:
+    xml: XMLSource, schema: Path | str | None = None, warn_on_schema_update: bool = True
+) -> AnyElementTree:
     """Validate XML against an XML Schema using xmlschema."""
     from xmlschema.exceptions import XMLSchemaException
 
-    tree = ensure_2016(xml, warn_on_transform=warn_on_transform, as_tree=True)
+    tree = ensure_2016(xml, warn_on_schema_update=warn_on_schema_update, as_tree=True)
     xmlschema = _get_XMLSchema(schema or OME_2016_06_XSD)
     try:
         xmlschema.validate(tree)  # type: ignore[arg-type]
     except XMLSchemaException as e:
         raise ValidationError(str(e)) from None
     return tree
 
@@ -382,84 +402,110 @@
 TRANSFORMS = {
     f"{OME_ROOT}/{p.name.split('-to')[0]}": p for p in TRANSFORMS_PATH.glob("*.xsl")
 }
 
 
 @overload
 def ensure_2016(
-    source: XMLSource, *, warn_on_transform: bool = ..., as_tree: Literal[True]
-) -> ET._ElementTree:
+    source: XMLSource, *, warn_on_schema_update: bool = ..., as_tree: Literal[True]
+) -> AnyElementTree:
     ...
 
 
 @overload
 def ensure_2016(
-    source: XMLSource, *, warn_on_transform: bool = ..., as_tree: Literal[False] = ...
+    source: XMLSource,
+    *,
+    warn_on_schema_update: bool = ...,
+    as_tree: Literal[False] = ...,
 ) -> FileLike:
     ...
 
 
 def ensure_2016(
-    source: XMLSource, *, warn_on_transform: bool = False, as_tree: bool = False
-) -> FileLike | ET._ElementTree:
+    source: XMLSource, *, warn_on_schema_update: bool = False, as_tree: bool = False
+) -> FileLike | AnyElementTree:
     """Ensure source is OME-2016-06 XML.
 
     If the source is not OME-2016-06 XML, it will be transformed sequentially using
     XSLT transforms in the `transforms` directory, until it is in the 2016-06 namespace.
     NOTE: this requires lxml to be installed and will raise an ImportError if it is not.
 
     Parameters
     ----------
     source : Path | str | bytes | io.BytesIO
         Path to an XML file, string or bytes containing XML, or a file-like object.
-    warn_on_transform : bool
+    warn_on_schema_update : bool
         Whether to warn if a transformation was applied to bring the document to
         OME-2016-06.
     as_tree : bool
         Whether to return an ElementTree or a FileLike object.
 
     Returns
     -------
-    FileLike | ET._ElementTree
+    FileLike | AnyElementTree
         If `as_tree` is `True`, an ElementTree, otherwise a FileLike object representing
         transformed OME 2016 XML.
 
 
     Raises
     ------
     ValueError
         If the source is an unrecognized XML namespace.
     ImportError
         If lxml is not installed and a transformation is required.
     """
     normed_source = _normalize(source)
-    ns_in = _get_ns_file(normed_source)
+    try:
+        ns_in = _get_ns_file(normed_source)
+    except Exception as e:
+        raise ValueError(f"Could not parse XML from {source!r}") from e
+
+    # catch rare case of OME-XML with lowercase ome in namespace
+    if "Schemas/ome/" in ns_in:
+        normed_source = _capitalize_ome(normed_source)
+        ns_in = _get_ns_file(normed_source)
+
+    if hasattr(normed_source, "seek"):
+        normed_source.seek(0)
 
     if ns_in == OME_2016_06_URI:
         if as_tree:
-            if hasattr(normed_source, "seek"):
-                normed_source.seek(0)
             return ET.parse(normed_source)
         return normed_source
 
     if ns_in in TRANSFORMS:
         tree = ET.parse(normed_source)
         ns = ns_in
         while ns in TRANSFORMS:
             tree = _apply_xslt(tree, TRANSFORMS[ns])
             ns = _get_ns_elem(tree)
-        if warn_on_transform:
+        if warn_on_schema_update:
             warnings.warn(
                 f"Transformed source from {ns_in!r} to {OME_2016_06_URI!r}",
                 stacklevel=2,
             )
 
         return tree if as_tree else io.BytesIO(ET.tostring(tree, encoding="utf-8"))
 
-    raise ValueError(f"Unsupported document namespace {ns!r}")  # pragma: no cover
+    raise ValueError(f"Unsupported document namespace {ns_in!r}")
+
+
+def _capitalize_ome(source: FileLike) -> FileLike:
+    """Fix OME namespace capitalization errors."""
+    if hasattr(source, "read") and hasattr(source, "seek"):
+        source.seek(0)
+        data = source.read()
+    else:
+        with open(source, "rb") as fh:
+            data = fh.read()
+
+    io_out = io.BytesIO(data.replace(b"Schemas/ome/", b"Schemas/OME/"))
+    io_out.seek(0)
+    return io_out
 
 
 def _normalize(source: XMLSource) -> FileLike:
     """Normalize the input to a BytesIO object, or a filepath.
 
     Parameters
     ----------
@@ -477,18 +523,21 @@
         if os.path.isfile(source):
             return source
         return io.BytesIO(source.encode())
     elif isinstance(source, bytes):
         return io.BytesIO(source)
     elif isinstance(source, io.BufferedIOBase):
         return source
-    raise TypeError(f"Unsupported source type {type(source)!r}")  # pragma: no cover
+
+    if hasattr(source, "mode") and "b" not in source.mode:
+        raise TypeError("File must be opened in binary mode")
+    raise TypeError(f"Unsupported source type {type(source)!r}")
 
 
-def _apply_xslt(root: ElementOrTree, xslt_path: str | Path) -> _XSLTResultTree:
+def _apply_xslt(root: ET._ElementTree, xslt_path: str | Path) -> _XSLTResultTree:
     """Apply an XSLT transform to an element or element tree."""
     try:
         from lxml import etree
     except ImportError:  # pragma: no cover
         ns = _get_ns_elem(root)
         raise ImportError(
             f"This documented is using an outdated schema ({ns!r}). "
@@ -500,28 +549,30 @@
     transformer = etree.XSLT(ET.parse(xslt_path))
     return transformer(root)
 
 
 # ------------------------
 
 
-def _get_ns_elem(elem: ET._Element | ET._ElementTree) -> str:
+def _get_ns_elem(elem: ET._Element | AnyElementTree) -> str:
     """Get namespace from an element or element tree."""
     root = elem.getroot() if hasattr(elem, "getroot") else elem
     # return root.nsmap[root.prefix]  this only works for lxml
     return root.tag.split("}", 1)[0].lstrip("{")
 
 
 def _get_ns_file(source: FileLike) -> str:
     """Get namespace from a file or file-like object."""
+    if hasattr(source, "seek"):
+        source.seek(0)
     _, root = next(ET.iterparse(source, events=("start",)))
     return _get_ns_elem(root)  # type: ignore[arg-type]
 
 
-def _get_root_ome_type(xml: FileLike | ET._ElementTree) -> type[OMEType]:
+def _get_root_ome_type(xml: FileLike | AnyElementTree) -> type[OMEType]:
     """Resolve a ome_types.model class for the root element of an OME XML document."""
     from ome_types import model
 
     if hasattr(xml, "getroot"):
         root = xml.getroot()
     else:
         if hasattr(xml, "seek"):
```

### Comparing `ome_types-0.4.0rc3/src/ome_types/_pydantic_compat.py` & `ome_types-0.4.0rc4/src/ome_types/_pydantic_compat.py`

 * *Files identical despite different names*

### Comparing `ome_types-0.4.0rc3/src/ome_types/ome-2016-06.xsd` & `ome_types-0.4.0rc4/src/ome_types/ome-2016-06.xsd`

 * *Files identical despite different names*

### Comparing `ome_types-0.4.0rc3/src/ome_types/units.py` & `ome_types-0.4.0rc4/src/ome_types/units.py`

 * *Files identical despite different names*

### Comparing `ome_types-0.4.0rc3/src/ome_types/widget.py` & `ome_types-0.4.0rc4/src/ome_types/widget.py`

 * *Files identical despite different names*

### Comparing `ome_types-0.4.0rc3/src/ome_types/_mixins/_base_type.py` & `ome_types-0.4.0rc4/src/ome_types/_mixins/_base_type.py`

 * *Files identical despite different names*

### Comparing `ome_types-0.4.0rc3/src/ome_types/_mixins/_ids.py` & `ome_types-0.4.0rc4/src/ome_types/_mixins/_ids.py`

 * *Files identical despite different names*

### Comparing `ome_types-0.4.0rc3/src/ome_types/_mixins/_instrument.py` & `ome_types-0.4.0rc4/src/ome_types/_mixins/_instrument.py`

 * *Files identical despite different names*

### Comparing `ome_types-0.4.0rc3/src/ome_types/_mixins/_kinded.py` & `ome_types-0.4.0rc4/src/ome_types/_mixins/_kinded.py`

 * *Files identical despite different names*

### Comparing `ome_types-0.4.0rc3/src/ome_types/_mixins/_ome.py` & `ome_types-0.4.0rc4/src/ome_types/_mixins/_ome.py`

 * *Files identical despite different names*

### Comparing `ome_types-0.4.0rc3/src/ome_types/_mixins/_reference.py` & `ome_types-0.4.0rc4/src/ome_types/_mixins/_reference.py`

 * *Files identical despite different names*

### Comparing `ome_types-0.4.0rc3/src/ome_types/_mixins/_validators.py` & `ome_types-0.4.0rc4/src/ome_types/_mixins/_validators.py`

 * *Files identical despite different names*

### Comparing `ome_types-0.4.0rc3/src/ome_types/_vendor/__init__.py` & `ome_types-0.4.0rc4/src/ome_types/_vendor/__init__.py`

 * *Files identical despite different names*

### Comparing `ome_types-0.4.0rc3/src/ome_types/_vendor/_pydantic_color_v1.py` & `ome_types-0.4.0rc4/src/ome_types/_vendor/_pydantic_color_v1.py`

 * *Files identical despite different names*

### Comparing `ome_types-0.4.0rc3/src/ome_types/_vendor/_pydantic_color_v2.py` & `ome_types-0.4.0rc4/src/ome_types/_vendor/_pydantic_color_v2.py`

 * *Files identical despite different names*

### Comparing `ome_types-0.4.0rc3/src/ome_types/model/__init__.py` & `ome_types-0.4.0rc4/src/ome_types/model/__init__.py`

 * *Files identical despite different names*

### Comparing `ome_types-0.4.0rc3/src/ome_types/model/_color.py` & `ome_types-0.4.0rc4/src/ome_types/model/_color.py`

 * *Files identical despite different names*

### Comparing `ome_types-0.4.0rc3/src/ome_types/model/_converters.py` & `ome_types-0.4.0rc4/src/ome_types/model/_converters.py`

 * *Files identical despite different names*

### Comparing `ome_types-0.4.0rc3/src/ome_types/model/_shape_union.py` & `ome_types-0.4.0rc4/src/ome_types/model/_shape_union.py`

 * *Files identical despite different names*

### Comparing `ome_types-0.4.0rc3/src/ome_types/model/_structured_annotations.py` & `ome_types-0.4.0rc4/src/ome_types/model/_structured_annotations.py`

 * *Files identical despite different names*

### Comparing `ome_types-0.4.0rc3/src/ome_types/model/_user_sequence.py` & `ome_types-0.4.0rc4/src/ome_types/model/_user_sequence.py`

 * *Files identical despite different names*

### Comparing `ome_types-0.4.0rc3/src/ome_types/model/simple_types.py` & `ome_types-0.4.0rc4/src/ome_types/model/simple_types.py`

 * *Files identical despite different names*

### Comparing `ome_types-0.4.0rc3/src/ome_types/transforms/2003-FC-to-2008-09.xsl` & `ome_types-0.4.0rc4/src/ome_types/transforms/2003-FC-to-2008-09.xsl`

 * *Files identical despite different names*

### Comparing `ome_types-0.4.0rc3/src/ome_types/transforms/2007-06-to-2008-09.xsl` & `ome_types-0.4.0rc4/src/ome_types/transforms/2007-06-to-2008-09.xsl`

 * *Files identical despite different names*

### Comparing `ome_types-0.4.0rc3/src/ome_types/transforms/2008-02-to-2008-09.xsl` & `ome_types-0.4.0rc4/src/ome_types/transforms/2008-02-to-2008-09.xsl`

 * *Files identical despite different names*

### Comparing `ome_types-0.4.0rc3/src/ome_types/transforms/2008-09-to-2009-09.xsl` & `ome_types-0.4.0rc4/src/ome_types/transforms/2008-09-to-2009-09.xsl`

 * *Files identical despite different names*

### Comparing `ome_types-0.4.0rc3/src/ome_types/transforms/2009-09-to-2010-04.xsl` & `ome_types-0.4.0rc4/src/ome_types/transforms/2009-09-to-2010-04.xsl`

 * *Files identical despite different names*

### Comparing `ome_types-0.4.0rc3/src/ome_types/transforms/2010-04-to-2010-06.xsl` & `ome_types-0.4.0rc4/src/ome_types/transforms/2010-04-to-2010-06.xsl`

 * *Files identical despite different names*

### Comparing `ome_types-0.4.0rc3/src/ome_types/transforms/2010-06-to-2011-06.xsl` & `ome_types-0.4.0rc4/src/ome_types/transforms/2010-06-to-2011-06.xsl`

 * *Files identical despite different names*

### Comparing `ome_types-0.4.0rc3/src/ome_types/transforms/2011-06-to-2012-06.xsl` & `ome_types-0.4.0rc4/src/ome_types/transforms/2011-06-to-2012-06.xsl`

 * *Files identical despite different names*

### Comparing `ome_types-0.4.0rc3/src/ome_types/transforms/2012-06-to-2013-06.xsl` & `ome_types-0.4.0rc4/src/ome_types/transforms/2012-06-to-2013-06.xsl`

 * *Files identical despite different names*

### Comparing `ome_types-0.4.0rc3/src/ome_types/transforms/2013-06-to-2015-01.xsl` & `ome_types-0.4.0rc4/src/ome_types/transforms/2013-06-to-2015-01.xsl`

 * *Files identical despite different names*

### Comparing `ome_types-0.4.0rc3/src/ome_types/transforms/2015-01-to-2016-06.xsl` & `ome_types-0.4.0rc4/src/ome_types/transforms/2015-01-to-2016-06.xsl`

 * *Files identical despite different names*

### Comparing `ome_types-0.4.0rc3/src/xsdata_pydantic_basemodel/bindings.py` & `ome_types-0.4.0rc4/src/xsdata_pydantic_basemodel/bindings.py`

 * *Files identical despite different names*

### Comparing `ome_types-0.4.0rc3/src/xsdata_pydantic_basemodel/compat.py` & `ome_types-0.4.0rc4/src/xsdata_pydantic_basemodel/compat.py`

 * *Files identical despite different names*

### Comparing `ome_types-0.4.0rc3/src/xsdata_pydantic_basemodel/config.py` & `ome_types-0.4.0rc4/src/xsdata_pydantic_basemodel/config.py`

 * *Files identical despite different names*

### Comparing `ome_types-0.4.0rc3/src/xsdata_pydantic_basemodel/generator.py` & `ome_types-0.4.0rc4/src/xsdata_pydantic_basemodel/generator.py`

 * *Files identical despite different names*

### Comparing `ome_types-0.4.0rc3/src/xsdata_pydantic_basemodel/pydantic_compat.py` & `ome_types-0.4.0rc4/src/xsdata_pydantic_basemodel/pydantic_compat.py`

 * *Files identical despite different names*

### Comparing `ome_types-0.4.0rc3/.gitignore` & `ome_types-0.4.0rc4/.gitignore`

 * *Files identical despite different names*

### Comparing `ome_types-0.4.0rc3/LICENSE` & `ome_types-0.4.0rc4/LICENSE`

 * *Files identical despite different names*

### Comparing `ome_types-0.4.0rc3/README.md` & `ome_types-0.4.0rc4/README.md`

 * *Files identical despite different names*

### Comparing `ome_types-0.4.0rc3/pyproject.toml` & `ome_types-0.4.0rc4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `ome_types-0.4.0rc3/PKG-INFO` & `ome_types-0.4.0rc4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ome-types
-Version: 0.4.0rc3
+Version: 0.4.0rc4
 Summary: Python dataclasses for the OME data model
 Project-URL: Source, https://github.com/tlambert03/ome-types
 Project-URL: Tracker, https://github.com/tlambert03/ome-types/issues
 Project-URL: Documentation, https://ome-types.readthedocs.io/en/latest/
 Author-email: Talley Lambert <talley.lambert@gmail.com>
 License: MIT
 License-File: LICENSE
```

