# Comparing `tmp/fontmake-3.7.0b3.zip` & `tmp/fontmake-3.7.1.zip`

## zipinfo {}

```diff
@@ -1,728 +1,728 @@
-Zip file size: 474610 bytes, number of entries: 726
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-31 17:57 fontmake-3.7.0b3/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-31 17:57 fontmake-3.7.0b3/Lib/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-31 17:57 fontmake-3.7.0b3/.github/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-31 17:57 fontmake-3.7.0b3/tests/
--rw-r--r--  2.0 unx      910 b- defN 23-Jul-31 17:57 fontmake-3.7.0b3/requirements.txt
--rw-r--r--  2.0 unx      226 b- defN 23-Jul-31 17:57 fontmake-3.7.0b3/setup.cfg
--rwxr-xr-x  2.0 unx     1302 b- defN 23-Jul-31 17:57 fontmake-3.7.0b3/build_pyz.sh
--rw-r--r--  2.0 unx     7349 b- defN 23-Jul-31 17:57 fontmake-3.7.0b3/PKG-INFO
--rw-r--r--  2.0 unx     3193 b- defN 23-Jul-31 17:57 fontmake-3.7.0b3/TROUBLESHOOTING.md
--rw-r--r--  2.0 unx     1453 b- defN 23-Jul-31 17:57 fontmake-3.7.0b3/.gitignore
--rw-r--r--  2.0 unx      191 b- defN 23-Jul-31 17:57 fontmake-3.7.0b3/test_requirements.txt
--rw-r--r--  2.0 unx      142 b- defN 23-Jul-31 17:57 fontmake-3.7.0b3/MANIFEST.in
--rw-r--r--  2.0 unx    11357 b- defN 23-Jul-31 17:57 fontmake-3.7.0b3/LICENSE
--rw-r--r--  2.0 unx    19601 b- defN 23-Jul-31 17:57 fontmake-3.7.0b3/USAGE.md
--rw-r--r--  2.0 unx     6285 b- defN 23-Jul-31 17:57 fontmake-3.7.0b3/README.md
--rw-r--r--  2.0 unx     3917 b- defN 23-Jul-31 17:57 fontmake-3.7.0b3/setup.py
--rw-r--r--  2.0 unx      163 b- defN 23-Jul-31 17:57 fontmake-3.7.0b3/pyproject.toml
--rw-r--r--  2.0 unx      806 b- defN 23-Jul-31 17:57 fontmake-3.7.0b3/tox.ini
--rw-r--r--  2.0 unx      792 b- defN 23-Jul-31 17:57 fontmake-3.7.0b3/.coveragerc
--rw-r--r--  2.0 unx     1450 b- defN 23-Jul-31 17:57 fontmake-3.7.0b3/CONTRIBUTING.md
--rw-r--r--  2.0 unx       77 b- defN 23-Jul-31 17:57 fontmake-3.7.0b3/.codecov.yml
--rw-r--r--  2.0 unx      227 b- defN 23-Jul-31 17:57 fontmake-3.7.0b3/.editorconfig
--rw-r--r--  2.0 unx      322 b- defN 23-Jul-31 17:57 fontmake-3.7.0b3/.gitattributes
--rw-r--r--  2.0 unx      168 b- defN 23-Jul-31 17:57 fontmake-3.7.0b3/.pyup.yml
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-31 17:57 fontmake-3.7.0b3/Lib/fontmake/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-31 17:57 fontmake-3.7.0b3/Lib/fontmake.egg-info/
--rw-r--r--  2.0 unx     3049 b- defN 23-Jul-31 17:57 fontmake-3.7.0b3/Lib/fontmake/compatibility.py
--rw-r--r--  2.0 unx    32133 b- defN 23-Jul-31 17:57 fontmake-3.7.0b3/Lib/fontmake/instantiator.py
--rw-r--r--  2.0 unx     1439 b- defN 23-Jul-31 17:57 fontmake-3.7.0b3/Lib/fontmake/errors.py
--rw-r--r--  2.0 unx     3288 b- defN 23-Jul-31 17:57 fontmake-3.7.0b3/Lib/fontmake/ttfautohint.py
--rw-r--r--  2.0 unx    61003 b- defN 23-Jul-31 17:57 fontmake-3.7.0b3/Lib/fontmake/font_project.py
--rw-r--r--  2.0 unx      162 b- defN 23-Jul-31 17:57 fontmake-3.7.0b3/Lib/fontmake/_version.py
--rw-r--r--  2.0 unx      108 b- defN 23-Jul-31 17:57 fontmake-3.7.0b3/Lib/fontmake/__init__.py
--rw-r--r--  2.0 unx    27227 b- defN 23-Jul-31 17:57 fontmake-3.7.0b3/Lib/fontmake/__main__.py
--rw-r--r--  2.0 unx     7349 b- defN 23-Jul-31 17:57 fontmake-3.7.0b3/Lib/fontmake.egg-info/PKG-INFO
--rw-r--r--  2.0 unx        9 b- defN 23-Jul-31 17:57 fontmake-3.7.0b3/Lib/fontmake.egg-info/top_level.txt
--rw-r--r--  2.0 unx    42266 b- defN 23-Jul-31 17:57 fontmake-3.7.0b3/Lib/fontmake.egg-info/SOURCES.txt
--rw-r--r--  2.0 unx      768 b- defN 23-Jul-31 17:57 fontmake-3.7.0b3/Lib/fontmake.egg-info/requires.txt
--rw-r--r--  2.0 unx        1 b- defN 23-Jul-31 17:57 fontmake-3.7.0b3/Lib/fontmake.egg-info/dependency_links.txt
--rw-r--r--  2.0 unx       52 b- defN 23-Jul-31 17:57 fontmake-3.7.0b3/Lib/fontmake.egg-info/entry_points.txt
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-31 17:57 fontmake-3.7.0b3/.github/workflows/
--rw-r--r--  2.0 unx     4287 b- defN 23-Jul-31 17:57 fontmake-3.7.0b3/.github/workflows/ci.yml
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-31 17:57 fontmake-3.7.0b3/tests/data/
--rw-r--r--  2.0 unx      133 b- defN 23-Jul-31 17:57 fontmake-3.7.0b3/tests/conftest.py
--rw-r--r--  2.0 unx    25699 b- defN 23-Jul-31 17:57 fontmake-3.7.0b3/tests/test_instantiator.py
--rw-r--r--  2.0 unx    37281 b- defN 23-Jul-31 17:57 fontmake-3.7.0b3/tests/test_main.py
--rw-r--r--  2.0 unx     1668 b- defN 23-Jul-31 17:57 fontmake-3.7.0b3/tests/test_compatibility.py
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-31 17:57 fontmake-3.7.0b3/tests/data/DesignspaceRuleOrder/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-31 17:57 fontmake-3.7.0b3/tests/data/SwapGlyphNames/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-31 17:57 fontmake-3.7.0b3/tests/data/GlyphsUnitTestSans3.glyphspackage/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-31 17:57 fontmake-3.7.0b3/tests/data/DesignspaceTest/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-31 17:57 fontmake-3.7.0b3/tests/data/InstantiatorStrictMathGlyph/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-31 17:57 fontmake-3.7.0b3/tests/data/DesignspaceBrokenTest/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-31 17:57 fontmake-3.7.0b3/tests/data/InterpolateLayoutTest/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-31 17:57 fontmake-3.7.0b3/tests/data/AutohintingTest/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-31 17:57 fontmake-3.7.0b3/tests/data/IncompatibleSans/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-31 17:57 fontmake-3.7.0b3/tests/data/DesignspaceTestSharedFeatures/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-31 17:57 fontmake-3.7.0b3/tests/data/MutatorSans/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-31 17:57 fontmake-3.7.0b3/tests/data/MutatorSansLite/
--rw-r--r--  2.0 unx     6386 b- defN 23-Jul-31 17:57 fontmake-3.7.0b3/tests/data/TestSubset.glyphs
--rw-r--r--  2.0 unx      150 b- defN 23-Jul-31 17:57 fontmake-3.7.0b3/tests/data/GlyphData.xml
--rw-r--r--  2.0 unx     6381 b- defN 23-Jul-31 17:57 fontmake-3.7.0b3/tests/data/TestSubset2.glyphs
--rw-r--r--  2.0 unx    31198 b- defN 23-Jul-31 17:57 fontmake-3.7.0b3/tests/data/GlyphsUnitTestSans.glyphs
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-31 17:57 fontmake-3.7.0b3/tests/data/DesignspaceRuleOrder/MyFont_Black.ufo/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-31 17:57 fontmake-3.7.0b3/tests/data/DesignspaceRuleOrder/MyFont_Hair.ufo/
--rw-r--r--  2.0 unx     2035 b- defN 23-Jul-31 17:57 fontmake-3.7.0b3/tests/data/DesignspaceRuleOrder/MyFont.designspace
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-31 17:57 fontmake-3.7.0b3/tests/data/DesignspaceRuleOrder/MyFont_Black.ufo/glyphs/
--rw-r--r--  2.0 unx      275 b- defN 23-Jul-31 17:57 fontmake-3.7.0b3/tests/data/DesignspaceRuleOrder/MyFont_Black.ufo/layercontents.plist
--rw-r--r--  2.0 unx      887 b- defN 23-Jul-31 17:57 fontmake-3.7.0b3/tests/data/DesignspaceRuleOrder/MyFont_Black.ufo/fontinfo.plist
--rw-r--r--  2.0 unx      308 b- defN 23-Jul-31 17:57 fontmake-3.7.0b3/tests/data/DesignspaceRuleOrder/MyFont_Black.ufo/metainfo.plist
--rw-r--r--  2.0 unx      360 b- defN 23-Jul-31 17:57 fontmake-3.7.0b3/tests/data/DesignspaceRuleOrder/MyFont_Black.ufo/lib.plist
--rw-r--r--  2.0 unx     1455 b- defN 23-Jul-31 17:57 fontmake-3.7.0b3/tests/data/DesignspaceRuleOrder/MyFont_Black.ufo/glyphs/Q_.alt.glif
--rw-r--r--  2.0 unx      412 b- defN 23-Jul-31 17:57 fontmake-3.7.0b3/tests/data/DesignspaceRuleOrder/MyFont_Black.ufo/glyphs/contents.plist
--rw-r--r--  2.0 unx     1659 b- defN 23-Jul-31 17:57 fontmake-3.7.0b3/tests/data/DesignspaceRuleOrder/MyFont_Black.ufo/glyphs/Q_.glif
--rw-r--r--  2.0 unx     1261 b- defN 23-Jul-31 17:57 fontmake-3.7.0b3/tests/data/DesignspaceRuleOrder/MyFont_Black.ufo/glyphs/Q_.ss01.glif
--rw-r--r--  2.0 unx     1265 b- defN 23-Jul-31 17:57 fontmake-3.7.0b3/tests/data/DesignspaceRuleOrder/MyFont_Black.ufo/glyphs/Q_.ss01.alt.glif
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-31 17:57 fontmake-3.7.0b3/tests/data/DesignspaceRuleOrder/MyFont_Hair.ufo/glyphs/
--rw-r--r--  2.0 unx      275 b- defN 23-Jul-31 17:57 fontmake-3.7.0b3/tests/data/DesignspaceRuleOrder/MyFont_Hair.ufo/layercontents.plist
--rw-r--r--  2.0 unx      890 b- defN 23-Jul-31 17:57 fontmake-3.7.0b3/tests/data/DesignspaceRuleOrder/MyFont_Hair.ufo/fontinfo.plist
--rw-r--r--  2.0 unx      308 b- defN 23-Jul-31 17:57 fontmake-3.7.0b3/tests/data/DesignspaceRuleOrder/MyFont_Hair.ufo/metainfo.plist
--rw-r--r--  2.0 unx      360 b- defN 23-Jul-31 17:57 fontmake-3.7.0b3/tests/data/DesignspaceRuleOrder/MyFont_Hair.ufo/lib.plist
--rw-r--r--  2.0 unx     1439 b- defN 23-Jul-31 17:57 fontmake-3.7.0b3/tests/data/DesignspaceRuleOrder/MyFont_Hair.ufo/glyphs/Q_.alt.glif
--rw-r--r--  2.0 unx      412 b- defN 23-Jul-31 17:57 fontmake-3.7.0b3/tests/data/DesignspaceRuleOrder/MyFont_Hair.ufo/glyphs/contents.plist
--rw-r--r--  2.0 unx     1642 b- defN 23-Jul-31 17:57 fontmake-3.7.0b3/tests/data/DesignspaceRuleOrder/MyFont_Hair.ufo/glyphs/Q_.glif
--rw-r--r--  2.0 unx     1263 b- defN 23-Jul-31 17:57 fontmake-3.7.0b3/tests/data/DesignspaceRuleOrder/MyFont_Hair.ufo/glyphs/Q_.ss01.glif
--rw-r--r--  2.0 unx     1263 b- defN 23-Jul-31 17:57 fontmake-3.7.0b3/tests/data/DesignspaceRuleOrder/MyFont_Hair.ufo/glyphs/Q_.ss01.alt.glif
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-31 17:57 fontmake-3.7.0b3/tests/data/SwapGlyphNames/A.ufo/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-31 17:57 fontmake-3.7.0b3/tests/data/SwapGlyphNames/B.ufo/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-31 17:57 fontmake-3.7.0b3/tests/data/SwapGlyphNames/A.ufo/glyphs/
--rw-r--r--  2.0 unx      287 b- defN 23-Jul-31 17:57 fontmake-3.7.0b3/tests/data/SwapGlyphNames/A.ufo/layercontents.plist
--rw-r--r--  2.0 unx      471 b- defN 23-Jul-31 17:57 fontmake-3.7.0b3/tests/data/SwapGlyphNames/A.ufo/groups.plist
--rw-r--r--  2.0 unx      714 b- defN 23-Jul-31 17:57 fontmake-3.7.0b3/tests/data/SwapGlyphNames/A.ufo/kerning.plist
--rw-r--r--  2.0 unx      790 b- defN 23-Jul-31 17:57 fontmake-3.7.0b3/tests/data/SwapGlyphNames/A.ufo/fontinfo.plist
--rw-r--r--  2.0 unx      318 b- defN 23-Jul-31 17:57 fontmake-3.7.0b3/tests/data/SwapGlyphNames/A.ufo/metainfo.plist
--rw-r--r--  2.0 unx      443 b- defN 23-Jul-31 17:57 fontmake-3.7.0b3/tests/data/SwapGlyphNames/A.ufo/lib.plist
--rw-r--r--  2.0 unx      382 b- defN 23-Jul-31 17:57 fontmake-3.7.0b3/tests/data/SwapGlyphNames/A.ufo/glyphs/aaa.glif
--rw-r--r--  2.0 unx      522 b- defN 23-Jul-31 17:57 fontmake-3.7.0b3/tests/data/SwapGlyphNames/A.ufo/glyphs/y.glif
--rw-r--r--  2.0 unx      393 b- defN 23-Jul-31 17:57 fontmake-3.7.0b3/tests/data/SwapGlyphNames/A.ufo/glyphs/aaa.swap.glif
--rw-r--r--  2.0 unx      581 b- defN 23-Jul-31 17:57 fontmake-3.7.0b3/tests/data/SwapGlyphNames/A.ufo/glyphs/a.swap.glif
--rw-r--r--  2.0 unx      436 b- defN 23-Jul-31 17:57 fontmake-3.7.0b3/tests/data/SwapGlyphNames/A.ufo/glyphs/a.glif
--rw-r--r--  2.0 unx      543 b- defN 23-Jul-31 17:57 fontmake-3.7.0b3/tests/data/SwapGlyphNames/A.ufo/glyphs/contents.plist
--rw-r--r--  2.0 unx      156 b- defN 23-Jul-31 17:57 fontmake-3.7.0b3/tests/data/SwapGlyphNames/A.ufo/glyphs/space.glif
--rw-r--r--  2.0 unx      646 b- defN 23-Jul-31 17:57 fontmake-3.7.0b3/tests/data/SwapGlyphNames/A.ufo/glyphs/x.glif
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-31 17:57 fontmake-3.7.0b3/tests/data/SwapGlyphNames/B.ufo/glyphs/
--rw-r--r--  2.0 unx      287 b- defN 23-Jul-31 17:57 fontmake-3.7.0b3/tests/data/SwapGlyphNames/B.ufo/layercontents.plist
--rw-r--r--  2.0 unx      790 b- defN 23-Jul-31 17:57 fontmake-3.7.0b3/tests/data/SwapGlyphNames/B.ufo/fontinfo.plist
--rw-r--r--  2.0 unx      318 b- defN 23-Jul-31 17:57 fontmake-3.7.0b3/tests/data/SwapGlyphNames/B.ufo/metainfo.plist
--rw-r--r--  2.0 unx      410 b- defN 23-Jul-31 17:57 fontmake-3.7.0b3/tests/data/SwapGlyphNames/B.ufo/lib.plist
--rw-r--r--  2.0 unx      898 b- defN 23-Jul-31 17:57 fontmake-3.7.0b3/tests/data/SwapGlyphNames/B.ufo/glyphs/a.glif
--rw-r--r--  2.0 unx      487 b- defN 23-Jul-31 17:57 fontmake-3.7.0b3/tests/data/SwapGlyphNames/B.ufo/glyphs/contents.plist
--rw-r--r--  2.0 unx      539 b- defN 23-Jul-31 17:57 fontmake-3.7.0b3/tests/data/SwapGlyphNames/B.ufo/glyphs/dieresiscomb.glif
--rw-r--r--  2.0 unx      205 b- defN 23-Jul-31 17:57 fontmake-3.7.0b3/tests/data/SwapGlyphNames/B.ufo/glyphs/adieresis.alt.glif
--rw-r--r--  2.0 unx      784 b- defN 23-Jul-31 17:57 fontmake-3.7.0b3/tests/data/SwapGlyphNames/B.ufo/glyphs/a.alt.glif
--rw-r--r--  2.0 unx      221 b- defN 23-Jul-31 17:57 fontmake-3.7.0b3/tests/data/SwapGlyphNames/B.ufo/glyphs/adieresis.glif
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-31 17:57 fontmake-3.7.0b3/tests/data/GlyphsUnitTestSans3.glyphspackage/glyphs/
--rw-r--r--  2.0 unx    22772 b- defN 23-Jul-31 17:57 fontmake-3.7.0b3/tests/data/GlyphsUnitTestSans3.glyphspackage/fontinfo.plist
--rw-r--r--  2.0 unx       83 b- defN 23-Jul-31 17:57 fontmake-3.7.0b3/tests/data/GlyphsUnitTestSans3.glyphspackage/order.plist
--rw-r--r--  2.0 unx     1308 b- defN 23-Jul-31 17:57 fontmake-3.7.0b3/tests/data/GlyphsUnitTestSans3.glyphspackage/glyphs/a.sc.glyph
--rw-r--r--  2.0 unx      454 b- defN 23-Jul-31 17:57 fontmake-3.7.0b3/tests/data/GlyphsUnitTestSans3.glyphspackage/glyphs/A_dieresis.glyph
--rw-r--r--  2.0 unx     1580 b- defN 23-Jul-31 17:57 fontmake-3.7.0b3/tests/data/GlyphsUnitTestSans3.glyphspackage/glyphs/n.glyph
--rw-r--r--  2.0 unx      764 b- defN 23-Jul-31 17:57 fontmake-3.7.0b3/tests/data/GlyphsUnitTestSans3.glyphspackage/glyphs/h.glyph
--rw-r--r--  2.0 unx      902 b- defN 23-Jul-31 17:57 fontmake-3.7.0b3/tests/data/GlyphsUnitTestSans3.glyphspackage/glyphs/m.glyph
--rw-r--r--  2.0 unx     1889 b- defN 23-Jul-31 17:57 fontmake-3.7.0b3/tests/data/GlyphsUnitTestSans3.glyphspackage/glyphs/A_.glyph
--rw-r--r--  2.0 unx     1026 b- defN 23-Jul-31 17:57 fontmake-3.7.0b3/tests/data/GlyphsUnitTestSans3.glyphspackage/glyphs/dieresis.glyph
--rw-r--r--  2.0 unx      445 b- defN 23-Jul-31 17:57 fontmake-3.7.0b3/tests/data/GlyphsUnitTestSans3.glyphspackage/glyphs/adieresis.glyph
--rw-r--r--  2.0 unx     5010 b- defN 23-Jul-31 17:57 fontmake-3.7.0b3/tests/data/GlyphsUnitTestSans3.glyphspackage/glyphs/_part.shoulder.glyph
--rw-r--r--  2.0 unx     6165 b- defN 23-Jul-31 17:57 fontmake-3.7.0b3/tests/data/GlyphsUnitTestSans3.glyphspackage/glyphs/a.glyph
--rw-r--r--  2.0 unx     2295 b- defN 23-Jul-31 17:57 fontmake-3.7.0b3/tests/data/GlyphsUnitTestSans3.glyphspackage/glyphs/_part.stem.glyph
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-31 17:57 fontmake-3.7.0b3/tests/data/DesignspaceTest/MyFont-Light.ufo/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-31 17:57 fontmake-3.7.0b3/tests/data/DesignspaceTest/MyFont-Bold.ufo/
--rw-r--r--  2.0 unx      983 b- defN 23-Jul-31 17:57 fontmake-3.7.0b3/tests/data/DesignspaceTest/DesignspaceTest.designspace
--rw-r--r--  2.0 unx     3057 b- defN 23-Jul-31 17:57 fontmake-3.7.0b3/tests/data/DesignspaceTest/MyFont-Light.ufoz
--rw-r--r--  2.0 unx      852 b- defN 23-Jul-31 17:57 fontmake-3.7.0b3/tests/data/DesignspaceTest/DesignspaceTest-instance-attrs.designspace
--rw-r--r--  2.0 unx      614 b- defN 23-Jul-31 17:57 fontmake-3.7.0b3/tests/data/DesignspaceTest/DesignspaceTest-slnt.designspace
--rw-r--r--  2.0 unx      621 b- defN 23-Jul-31 17:57 fontmake-3.7.0b3/tests/data/DesignspaceTest/DesignspaceTest-opsz.designspace
--rw-r--r--  2.0 unx     1340 b- defN 23-Jul-31 17:57 fontmake-3.7.0b3/tests/data/DesignspaceTest/DesignspaceTest-lib.designspace
--rw-r--r--  2.0 unx      916 b- defN 23-Jul-31 17:57 fontmake-3.7.0b3/tests/data/DesignspaceTest/DesignspaceTest-wght-wdth.designspace
--rw-r--r--  2.0 unx     2253 b- defN 23-Jul-31 17:57 fontmake-3.7.0b3/tests/data/DesignspaceTest/MyFont-Bold.ufoz
--rw-r--r--  2.0 unx      745 b- defN 23-Jul-31 17:57 fontmake-3.7.0b3/tests/data/DesignspaceTest/DesignspaceTest-bare.designspace
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-31 17:57 fontmake-3.7.0b3/tests/data/DesignspaceTest/MyFont-Light.ufo/glyphs/
--rw-r--r--  2.0 unx      287 b- defN 23-Jul-31 17:57 fontmake-3.7.0b3/tests/data/DesignspaceTest/MyFont-Light.ufo/layercontents.plist
--rw-r--r--  2.0 unx      357 b- defN 23-Jul-31 17:57 fontmake-3.7.0b3/tests/data/DesignspaceTest/MyFont-Light.ufo/groups.plist
--rw-r--r--  2.0 unx      878 b- defN 23-Jul-31 17:57 fontmake-3.7.0b3/tests/data/DesignspaceTest/MyFont-Light.ufo/fontinfo.plist
--rw-r--r--  2.0 unx      318 b- defN 23-Jul-31 17:57 fontmake-3.7.0b3/tests/data/DesignspaceTest/MyFont-Light.ufo/metainfo.plist
--rw-r--r--  2.0 unx      240 b- defN 23-Jul-31 17:57 fontmake-3.7.0b3/tests/data/DesignspaceTest/MyFont-Light.ufo/lib.plist
--rw-r--r--  2.0 unx      343 b- defN 23-Jul-31 17:57 fontmake-3.7.0b3/tests/data/DesignspaceTest/MyFont-Light.ufo/glyphs/l.glif
--rw-r--r--  2.0 unx      237 b- defN 23-Jul-31 17:57 fontmake-3.7.0b3/tests/data/DesignspaceTest/MyFont-Light.ufo/glyphs/contents.plist
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-31 17:57 fontmake-3.7.0b3/tests/data/DesignspaceTest/MyFont-Bold.ufo/glyphs/
--rw-r--r--  2.0 unx      287 b- defN 23-Jul-31 17:57 fontmake-3.7.0b3/tests/data/DesignspaceTest/MyFont-Bold.ufo/layercontents.plist
--rw-r--r--  2.0 unx      548 b- defN 23-Jul-31 17:57 fontmake-3.7.0b3/tests/data/DesignspaceTest/MyFont-Bold.ufo/fontinfo.plist
--rw-r--r--  2.0 unx      318 b- defN 23-Jul-31 17:57 fontmake-3.7.0b3/tests/data/DesignspaceTest/MyFont-Bold.ufo/metainfo.plist
--rw-r--r--  2.0 unx      345 b- defN 23-Jul-31 17:57 fontmake-3.7.0b3/tests/data/DesignspaceTest/MyFont-Bold.ufo/glyphs/l.glif
--rw-r--r--  2.0 unx      237 b- defN 23-Jul-31 17:57 fontmake-3.7.0b3/tests/data/DesignspaceTest/MyFont-Bold.ufo/glyphs/contents.plist
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-31 17:57 fontmake-3.7.0b3/tests/data/InstantiatorStrictMathGlyph/SquareOne.ufo/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-31 17:57 fontmake-3.7.0b3/tests/data/InstantiatorStrictMathGlyph/SquareTwo.ufo/
--rw-r--r--  2.0 unx      830 b- defN 23-Jul-31 17:57 fontmake-3.7.0b3/tests/data/InstantiatorStrictMathGlyph/StrictMathGlyph.designspace
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-31 17:57 fontmake-3.7.0b3/tests/data/InstantiatorStrictMathGlyph/SquareOne.ufo/glyphs/
--rw-r--r--  2.0 unx      283 b- defN 23-Jul-31 17:57 fontmake-3.7.0b3/tests/data/InstantiatorStrictMathGlyph/SquareOne.ufo/layercontents.plist
--rw-r--r--  2.0 unx      897 b- defN 23-Jul-31 17:57 fontmake-3.7.0b3/tests/data/InstantiatorStrictMathGlyph/SquareOne.ufo/fontinfo.plist
--rw-r--r--  2.0 unx      318 b- defN 23-Jul-31 17:57 fontmake-3.7.0b3/tests/data/InstantiatorStrictMathGlyph/SquareOne.ufo/metainfo.plist
--rw-r--r--  2.0 unx     1030 b- defN 23-Jul-31 17:57 fontmake-3.7.0b3/tests/data/InstantiatorStrictMathGlyph/SquareOne.ufo/lib.plist
--rw-r--r--  2.0 unx      243 b- defN 23-Jul-31 17:57 fontmake-3.7.0b3/tests/data/InstantiatorStrictMathGlyph/SquareOne.ufo/glyphs/contents.plist
--rw-r--r--  2.0 unx      770 b- defN 23-Jul-31 17:57 fontmake-3.7.0b3/tests/data/InstantiatorStrictMathGlyph/SquareOne.ufo/glyphs/test.glif
--rw-r--r--  2.0 unx      247 b- defN 23-Jul-31 17:57 fontmake-3.7.0b3/tests/data/InstantiatorStrictMathGlyph/SquareOne.ufo/glyphs/layerinfo.plist
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-31 17:57 fontmake-3.7.0b3/tests/data/InstantiatorStrictMathGlyph/SquareTwo.ufo/glyphs/
--rw-r--r--  2.0 unx      283 b- defN 23-Jul-31 17:57 fontmake-3.7.0b3/tests/data/InstantiatorStrictMathGlyph/SquareTwo.ufo/layercontents.plist
--rw-r--r--  2.0 unx      900 b- defN 23-Jul-31 17:57 fontmake-3.7.0b3/tests/data/InstantiatorStrictMathGlyph/SquareTwo.ufo/fontinfo.plist
--rw-r--r--  2.0 unx      318 b- defN 23-Jul-31 17:57 fontmake-3.7.0b3/tests/data/InstantiatorStrictMathGlyph/SquareTwo.ufo/metainfo.plist
--rw-r--r--  2.0 unx     1030 b- defN 23-Jul-31 17:57 fontmake-3.7.0b3/tests/data/InstantiatorStrictMathGlyph/SquareTwo.ufo/lib.plist
--rw-r--r--  2.0 unx      243 b- defN 23-Jul-31 17:57 fontmake-3.7.0b3/tests/data/InstantiatorStrictMathGlyph/SquareTwo.ufo/glyphs/contents.plist
--rw-r--r--  2.0 unx      786 b- defN 23-Jul-31 17:57 fontmake-3.7.0b3/tests/data/InstantiatorStrictMathGlyph/SquareTwo.ufo/glyphs/test.glif
--rw-r--r--  2.0 unx      247 b- defN 23-Jul-31 17:57 fontmake-3.7.0b3/tests/data/InstantiatorStrictMathGlyph/SquareTwo.ufo/glyphs/layerinfo.plist
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-31 17:57 fontmake-3.7.0b3/tests/data/DesignspaceBrokenTest/MyFont-Light.ufo/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-31 17:57 fontmake-3.7.0b3/tests/data/DesignspaceBrokenTest/MyFont-Bold.ufo/
--rw-r--r--  2.0 unx      983 b- defN 23-Jul-31 17:57 fontmake-3.7.0b3/tests/data/DesignspaceBrokenTest/DesignspaceTest.designspace
--rw-r--r--  2.0 unx     1135 b- defN 23-Jul-31 17:57 fontmake-3.7.0b3/tests/data/DesignspaceBrokenTest/Designspace-MastersAsInstances.designspace
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-31 17:57 fontmake-3.7.0b3/tests/data/DesignspaceBrokenTest/MyFont-Light.ufo/glyphs/
--rw-r--r--  2.0 unx      287 b- defN 23-Jul-31 17:57 fontmake-3.7.0b3/tests/data/DesignspaceBrokenTest/MyFont-Light.ufo/layercontents.plist
--rw-r--r--  2.0 unx      887 b- defN 23-Jul-31 17:57 fontmake-3.7.0b3/tests/data/DesignspaceBrokenTest/MyFont-Light.ufo/fontinfo.plist
--rw-r--r--  2.0 unx      318 b- defN 23-Jul-31 17:57 fontmake-3.7.0b3/tests/data/DesignspaceBrokenTest/MyFont-Light.ufo/metainfo.plist
--rw-r--r--  2.0 unx      303 b- defN 23-Jul-31 17:57 fontmake-3.7.0b3/tests/data/DesignspaceBrokenTest/MyFont-Light.ufo/lib.plist
--rw-r--r--  2.0 unx      343 b- defN 23-Jul-31 17:57 fontmake-3.7.0b3/tests/data/DesignspaceBrokenTest/MyFont-Light.ufo/glyphs/l.glif
--rw-r--r--  2.0 unx      288 b- defN 23-Jul-31 17:57 fontmake-3.7.0b3/tests/data/DesignspaceBrokenTest/MyFont-Light.ufo/glyphs/contents.plist
--rw-r--r--  2.0 unx      479 b- defN 23-Jul-31 17:57 fontmake-3.7.0b3/tests/data/DesignspaceBrokenTest/MyFont-Light.ufo/glyphs/asas.glif
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-31 17:57 fontmake-3.7.0b3/tests/data/DesignspaceBrokenTest/MyFont-Bold.ufo/glyphs/
--rw-r--r--  2.0 unx      287 b- defN 23-Jul-31 17:57 fontmake-3.7.0b3/tests/data/DesignspaceBrokenTest/MyFont-Bold.ufo/layercontents.plist
--rw-r--r--  2.0 unx      886 b- defN 23-Jul-31 17:57 fontmake-3.7.0b3/tests/data/DesignspaceBrokenTest/MyFont-Bold.ufo/fontinfo.plist
--rw-r--r--  2.0 unx      318 b- defN 23-Jul-31 17:57 fontmake-3.7.0b3/tests/data/DesignspaceBrokenTest/MyFont-Bold.ufo/metainfo.plist
--rw-r--r--  2.0 unx      303 b- defN 23-Jul-31 17:57 fontmake-3.7.0b3/tests/data/DesignspaceBrokenTest/MyFont-Bold.ufo/lib.plist
--rw-r--r--  2.0 unx      345 b- defN 23-Jul-31 17:57 fontmake-3.7.0b3/tests/data/DesignspaceBrokenTest/MyFont-Bold.ufo/glyphs/l.glif
--rw-r--r--  2.0 unx      288 b- defN 23-Jul-31 17:57 fontmake-3.7.0b3/tests/data/DesignspaceBrokenTest/MyFont-Bold.ufo/glyphs/contents.plist
--rw-r--r--  2.0 unx      425 b- defN 23-Jul-31 17:57 fontmake-3.7.0b3/tests/data/DesignspaceBrokenTest/MyFont-Bold.ufo/glyphs/asas.glif
--rw-r--r--  2.0 unx       92 b- defN 23-Jul-31 17:57 fontmake-3.7.0b3/tests/data/InterpolateLayoutTest/InterpolateLayoutTest GSUB.txt
--rw-r--r--  2.0 unx      716 b- defN 23-Jul-31 17:57 fontmake-3.7.0b3/tests/data/InterpolateLayoutTest/InterpolateLayoutTest.plist
--rw-r--r--  2.0 unx       73 b- defN 23-Jul-31 17:57 fontmake-3.7.0b3/tests/data/InterpolateLayoutTest/InterpolateLayoutTest GDEF.txt
--rw-r--r--  2.0 unx      249 b- defN 23-Jul-31 17:57 fontmake-3.7.0b3/tests/data/InterpolateLayoutTest/InterpolateLayoutTest 1000 GPOS.txt
--rw-r--r--  2.0 unx     6904 b- defN 23-Jul-31 17:57 fontmake-3.7.0b3/tests/data/InterpolateLayoutTest/InterpolateLayoutTest.glyphs
--rw-r--r--  2.0 unx      246 b- defN 23-Jul-31 17:57 fontmake-3.7.0b3/tests/data/InterpolateLayoutTest/InterpolateLayoutTest 0 GPOS.txt
--rw-r--r--  2.0 unx   125360 b- defN 23-Jul-31 17:57 fontmake-3.7.0b3/tests/data/AutohintingTest/Padyakke.glyphs
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-31 17:57 fontmake-3.7.0b3/tests/data/IncompatibleSans/IncompatibleSans-Bold.ufo/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-31 17:57 fontmake-3.7.0b3/tests/data/IncompatibleSans/IncompatibleSans-Regular.ufo/
--rw-r--r--  2.0 unx      762 b- defN 23-Jul-31 17:57 fontmake-3.7.0b3/tests/data/IncompatibleSans/IncompatibleSans.designspace
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-31 17:57 fontmake-3.7.0b3/tests/data/IncompatibleSans/IncompatibleSans-Bold.ufo/glyphs/
--rw-r--r--  2.0 unx      101 b- defN 23-Jul-31 17:57 fontmake-3.7.0b3/tests/data/IncompatibleSans/IncompatibleSans-Bold.ufo/features.fea
--rw-r--r--  2.0 unx      287 b- defN 23-Jul-31 17:57 fontmake-3.7.0b3/tests/data/IncompatibleSans/IncompatibleSans-Bold.ufo/layercontents.plist
--rw-r--r--  2.0 unx     1158 b- defN 23-Jul-31 17:57 fontmake-3.7.0b3/tests/data/IncompatibleSans/IncompatibleSans-Bold.ufo/fontinfo.plist
--rw-r--r--  2.0 unx      318 b- defN 23-Jul-31 17:57 fontmake-3.7.0b3/tests/data/IncompatibleSans/IncompatibleSans-Bold.ufo/metainfo.plist
--rw-r--r--  2.0 unx     2113 b- defN 23-Jul-31 17:57 fontmake-3.7.0b3/tests/data/IncompatibleSans/IncompatibleSans-Bold.ufo/lib.plist
--rw-r--r--  2.0 unx      694 b- defN 23-Jul-31 17:57 fontmake-3.7.0b3/tests/data/IncompatibleSans/IncompatibleSans-Bold.ufo/glyphs/D_.glif
--rw-r--r--  2.0 unx      215 b- defN 23-Jul-31 17:57 fontmake-3.7.0b3/tests/data/IncompatibleSans/IncompatibleSans-Bold.ufo/glyphs/C_.glif
--rw-r--r--  2.0 unx      560 b- defN 23-Jul-31 17:57 fontmake-3.7.0b3/tests/data/IncompatibleSans/IncompatibleSans-Bold.ufo/glyphs/B_.glif
--rw-r--r--  2.0 unx      429 b- defN 23-Jul-31 17:57 fontmake-3.7.0b3/tests/data/IncompatibleSans/IncompatibleSans-Bold.ufo/glyphs/contents.plist
--rw-r--r--  2.0 unx      154 b- defN 23-Jul-31 17:57 fontmake-3.7.0b3/tests/data/IncompatibleSans/IncompatibleSans-Bold.ufo/glyphs/space.glif
--rw-r--r--  2.0 unx     1196 b- defN 23-Jul-31 17:57 fontmake-3.7.0b3/tests/data/IncompatibleSans/IncompatibleSans-Bold.ufo/glyphs/A_.glif
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-31 17:57 fontmake-3.7.0b3/tests/data/IncompatibleSans/IncompatibleSans-Regular.ufo/glyphs/
--rw-r--r--  2.0 unx      287 b- defN 23-Jul-31 17:57 fontmake-3.7.0b3/tests/data/IncompatibleSans/IncompatibleSans-Regular.ufo/layercontents.plist
--rw-r--r--  2.0 unx     1160 b- defN 23-Jul-31 17:57 fontmake-3.7.0b3/tests/data/IncompatibleSans/IncompatibleSans-Regular.ufo/fontinfo.plist
--rw-r--r--  2.0 unx      318 b- defN 23-Jul-31 17:57 fontmake-3.7.0b3/tests/data/IncompatibleSans/IncompatibleSans-Regular.ufo/metainfo.plist
--rw-r--r--  2.0 unx     2107 b- defN 23-Jul-31 17:57 fontmake-3.7.0b3/tests/data/IncompatibleSans/IncompatibleSans-Regular.ufo/lib.plist
--rw-r--r--  2.0 unx      652 b- defN 23-Jul-31 17:57 fontmake-3.7.0b3/tests/data/IncompatibleSans/IncompatibleSans-Regular.ufo/glyphs/D_.glif
--rw-r--r--  2.0 unx      217 b- defN 23-Jul-31 17:57 fontmake-3.7.0b3/tests/data/IncompatibleSans/IncompatibleSans-Regular.ufo/glyphs/C_.glif
--rw-r--r--  2.0 unx      652 b- defN 23-Jul-31 17:57 fontmake-3.7.0b3/tests/data/IncompatibleSans/IncompatibleSans-Regular.ufo/glyphs/B_.glif
--rw-r--r--  2.0 unx      429 b- defN 23-Jul-31 17:57 fontmake-3.7.0b3/tests/data/IncompatibleSans/IncompatibleSans-Regular.ufo/glyphs/contents.plist
--rw-r--r--  2.0 unx      154 b- defN 23-Jul-31 17:57 fontmake-3.7.0b3/tests/data/IncompatibleSans/IncompatibleSans-Regular.ufo/glyphs/space.glif
--rw-r--r--  2.0 unx      893 b- defN 23-Jul-31 17:57 fontmake-3.7.0b3/tests/data/IncompatibleSans/IncompatibleSans-Regular.ufo/glyphs/A_.glif
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-31 17:57 fontmake-3.7.0b3/tests/data/DesignspaceTestSharedFeatures/DesignspaceTest-Regular.ufo/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-31 17:57 fontmake-3.7.0b3/tests/data/DesignspaceTestSharedFeatures/DesignspaceTest-Light.ufo/
--rw-r--r--  2.0 unx     1059 b- defN 23-Jul-31 17:57 fontmake-3.7.0b3/tests/data/DesignspaceTestSharedFeatures/DesignspaceTestSharedFeatures.designspace
--rw-r--r--  2.0 unx        7 b- defN 23-Jul-31 17:57 fontmake-3.7.0b3/tests/data/DesignspaceTestSharedFeatures/family.fea
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-31 17:57 fontmake-3.7.0b3/tests/data/DesignspaceTestSharedFeatures/DesignspaceTest-Regular.ufo/glyphs/
--rw-r--r--  2.0 unx       20 b- defN 23-Jul-31 17:57 fontmake-3.7.0b3/tests/data/DesignspaceTestSharedFeatures/DesignspaceTest-Regular.ufo/features.fea
--rw-r--r--  2.0 unx      287 b- defN 23-Jul-31 17:57 fontmake-3.7.0b3/tests/data/DesignspaceTestSharedFeatures/DesignspaceTest-Regular.ufo/layercontents.plist
--rw-r--r--  2.0 unx      899 b- defN 23-Jul-31 17:57 fontmake-3.7.0b3/tests/data/DesignspaceTestSharedFeatures/DesignspaceTest-Regular.ufo/fontinfo.plist
--rw-r--r--  2.0 unx      318 b- defN 23-Jul-31 17:57 fontmake-3.7.0b3/tests/data/DesignspaceTestSharedFeatures/DesignspaceTest-Regular.ufo/metainfo.plist
--rw-r--r--  2.0 unx      183 b- defN 23-Jul-31 17:57 fontmake-3.7.0b3/tests/data/DesignspaceTestSharedFeatures/DesignspaceTest-Regular.ufo/glyphs/contents.plist
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-31 17:57 fontmake-3.7.0b3/tests/data/DesignspaceTestSharedFeatures/DesignspaceTest-Light.ufo/glyphs/
--rw-r--r--  2.0 unx      287 b- defN 23-Jul-31 17:57 fontmake-3.7.0b3/tests/data/DesignspaceTestSharedFeatures/DesignspaceTest-Light.ufo/layercontents.plist
--rw-r--r--  2.0 unx      897 b- defN 23-Jul-31 17:57 fontmake-3.7.0b3/tests/data/DesignspaceTestSharedFeatures/DesignspaceTest-Light.ufo/fontinfo.plist
--rw-r--r--  2.0 unx      318 b- defN 23-Jul-31 17:57 fontmake-3.7.0b3/tests/data/DesignspaceTestSharedFeatures/DesignspaceTest-Light.ufo/metainfo.plist
--rw-r--r--  2.0 unx      183 b- defN 23-Jul-31 17:57 fontmake-3.7.0b3/tests/data/DesignspaceTestSharedFeatures/DesignspaceTest-Light.ufo/glyphs/contents.plist
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-31 17:57 fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansLightWide.ufo/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-31 17:57 fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansIntermediateCondensed.ufo/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-31 17:57 fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-31 17:57 fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansIntermediateWide.ufo/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-31 17:57 fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansBoldWide.ufo/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-31 17:57 fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/
--rw-r--r--  2.0 unx     8462 b- defN 23-Jul-31 17:57 fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSans_missing.designspace
--rw-r--r--  2.0 unx     7111 b- defN 23-Jul-31 17:57 fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSans.designspace
--rw-r--r--  2.0 unx     1394 b- defN 23-Jul-31 17:57 fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSans-width-only.designspace
--rw-r--r--  2.0 unx     2611 b- defN 23-Jul-31 17:57 fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSans-with-openNodes.designspace
--rw-r--r--  2.0 unx     1412 b- defN 23-Jul-31 17:57 fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSans-weight-only.designspace
--rw-r--r--  2.0 unx     1067 b- defN 23-Jul-31 17:57 fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSans-non-default-layer.designspace
--rw-r--r--  2.0 unx     1074 b- defN 23-Jul-31 17:57 fontmake-3.7.0b3/tests/data/MutatorSans/LICENSE
--rw-r--r--  2.0 unx     7834 b- defN 23-Jul-31 17:57 fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSans_no_default.designspace
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-31 17:57 fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs.background/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-31 17:57 fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs.master_width_720.00_weight_645.00/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-31 17:57 fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs.master_width_0.00_weight_0.00/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-31 17:57 fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs.master_width_500.00_weight_500.00/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-31 17:57 fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-31 17:57 fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs.master_width_695.65_weight_166.38/
--rw-r--r--  2.0 unx       37 b- defN 23-Jul-31 17:57 fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansLightWide.ufo/features.fea
--rw-r--r--  2.0 unx      383 b- defN 23-Jul-31 17:57 fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansLightWide.ufo/layercontents.plist
--rw-r--r--  2.0 unx      366 b- defN 23-Jul-31 17:57 fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansLightWide.ufo/groups.plist
--rw-r--r--  2.0 unx     4852 b- defN 23-Jul-31 17:57 fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansLightWide.ufo/kerning.plist
--rw-r--r--  2.0 unx     1873 b- defN 23-Jul-31 17:57 fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansLightWide.ufo/fontinfo.plist
--rw-r--r--  2.0 unx      318 b- defN 23-Jul-31 17:57 fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansLightWide.ufo/metainfo.plist
--rw-r--r--  2.0 unx    18291 b- defN 23-Jul-31 17:57 fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansLightWide.ufo/lib.plist
--rw-r--r--  2.0 unx     1965 b- defN 23-Jul-31 17:57 fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs.background/S_.closed.glif
--rw-r--r--  2.0 unx      252 b- defN 23-Jul-31 17:57 fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs.background/contents.plist
--rw-r--r--  2.0 unx      246 b- defN 23-Jul-31 17:57 fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs.background/layerinfo.plist
--rw-r--r--  2.0 unx      228 b- defN 23-Jul-31 17:57 fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs.master_width_720.00_weight_645.00/contents.plist
--rw-r--r--  2.0 unx     2537 b- defN 23-Jul-31 17:57 fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs.master_width_720.00_weight_645.00/S_.glif
--rw-r--r--  2.0 unx      341 b- defN 23-Jul-31 17:57 fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs.master_width_720.00_weight_645.00/layerinfo.plist
--rw-r--r--  2.0 unx      181 b- defN 23-Jul-31 17:57 fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs.master_width_0.00_weight_0.00/contents.plist
--rw-r--r--  2.0 unx      237 b- defN 23-Jul-31 17:57 fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs.master_width_0.00_weight_0.00/layerinfo.plist
--rw-r--r--  2.0 unx      228 b- defN 23-Jul-31 17:57 fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs.master_width_500.00_weight_500.00/contents.plist
--rw-r--r--  2.0 unx     2459 b- defN 23-Jul-31 17:57 fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs.master_width_500.00_weight_500.00/S_.glif
--rw-r--r--  2.0 unx      344 b- defN 23-Jul-31 17:57 fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs.master_width_500.00_weight_500.00/layerinfo.plist
--rw-r--r--  2.0 unx      857 b- defN 23-Jul-31 17:57 fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/W_.glif
--rw-r--r--  2.0 unx      325 b- defN 23-Jul-31 17:57 fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/quotedblleft.glif
--rw-r--r--  2.0 unx      549 b- defN 23-Jul-31 17:57 fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/T_.glif
--rw-r--r--  2.0 unx     1459 b- defN 23-Jul-31 17:57 fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/R_.glif
--rw-r--r--  2.0 unx     1388 b- defN 23-Jul-31 17:57 fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/O_.glif
--rw-r--r--  2.0 unx     1751 b- defN 23-Jul-31 17:57 fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/G_.glif
--rw-r--r--  2.0 unx     1134 b- defN 23-Jul-31 17:57 fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/D_.glif
--rw-r--r--  2.0 unx     1970 b- defN 23-Jul-31 17:57 fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/S_.closed.glif
--rw-r--r--  2.0 unx      230 b- defN 23-Jul-31 17:57 fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/colon.glif
--rw-r--r--  2.0 unx      801 b- defN 23-Jul-31 17:57 fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/X_.glif
--rw-r--r--  2.0 unx      924 b- defN 23-Jul-31 17:57 fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/M_.glif
--rw-r--r--  2.0 unx      752 b- defN 23-Jul-31 17:57 fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/Z_.glif
--rw-r--r--  2.0 unx      703 b- defN 23-Jul-31 17:57 fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/I_.narrow.glif
--rw-r--r--  2.0 unx      954 b- defN 23-Jul-31 17:57 fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/F_.glif
--rw-r--r--  2.0 unx     1416 b- defN 23-Jul-31 17:57 fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/C_.glif
--rw-r--r--  2.0 unx      349 b- defN 23-Jul-31 17:57 fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/dot.glif
--rw-r--r--  2.0 unx      518 b- defN 23-Jul-31 17:57 fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/arrowright.glif
--rw-r--r--  2.0 unx     1785 b- defN 23-Jul-31 17:57 fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/B_.glif
--rw-r--r--  2.0 unx      943 b- defN 23-Jul-31 17:57 fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/U_.glif
--rw-r--r--  2.0 unx      743 b- defN 23-Jul-31 17:57 fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/I_.glif
--rw-r--r--  2.0 unx      749 b- defN 23-Jul-31 17:57 fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/N_.glif
--rw-r--r--  2.0 unx      740 b- defN 23-Jul-31 17:57 fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/V_.glif
--rw-r--r--  2.0 unx     1158 b- defN 23-Jul-31 17:57 fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/I_J_.glif
--rw-r--r--  2.0 unx      521 b- defN 23-Jul-31 17:57 fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/comma.glif
--rw-r--r--  2.0 unx     2687 b- defN 23-Jul-31 17:57 fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/contents.plist
--rw-r--r--  2.0 unx      370 b- defN 23-Jul-31 17:57 fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/dieresis.glif
--rw-r--r--  2.0 unx      747 b- defN 23-Jul-31 17:57 fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/Y_.glif
--rw-r--r--  2.0 unx      378 b- defN 23-Jul-31 17:57 fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/Q_.glif
--rw-r--r--  2.0 unx      154 b- defN 23-Jul-31 17:57 fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/space.glif
--rw-r--r--  2.0 unx      235 b- defN 23-Jul-31 17:57 fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/quotedblbase.glif
--rw-r--r--  2.0 unx      542 b- defN 23-Jul-31 17:57 fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/L_.glif
--rw-r--r--  2.0 unx      264 b- defN 23-Jul-31 17:57 fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/quotedblright.glif
--rw-r--r--  2.0 unx      354 b- defN 23-Jul-31 17:57 fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/A_acute.glif
--rw-r--r--  2.0 unx      514 b- defN 23-Jul-31 17:57 fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/arrowdown.glif
--rw-r--r--  2.0 unx     1130 b- defN 23-Jul-31 17:57 fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/P_.glif
--rw-r--r--  2.0 unx      233 b- defN 23-Jul-31 17:57 fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/semicolon.glif
--rw-r--r--  2.0 unx      802 b- defN 23-Jul-31 17:57 fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/J_.narrow.glif
--rw-r--r--  2.0 unx      360 b- defN 23-Jul-31 17:57 fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/A_dieresis.glif
--rw-r--r--  2.0 unx      518 b- defN 23-Jul-31 17:57 fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/arrowleft.glif
--rw-r--r--  2.0 unx      875 b- defN 23-Jul-31 17:57 fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/K_.glif
--rw-r--r--  2.0 unx     1320 b- defN 23-Jul-31 17:57 fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/A_.glif
--rw-r--r--  2.0 unx     1056 b- defN 23-Jul-31 17:57 fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/J_.glif
--rw-r--r--  2.0 unx      750 b- defN 23-Jul-31 17:57 fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/H_.glif
--rw-r--r--  2.0 unx     2358 b- defN 23-Jul-31 17:57 fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/S_.glif
--rw-r--r--  2.0 unx      353 b- defN 23-Jul-31 17:57 fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/acute.glif
--rw-r--r--  2.0 unx      371 b- defN 23-Jul-31 17:57 fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/layerinfo.plist
--rw-r--r--  2.0 unx      352 b- defN 23-Jul-31 17:57 fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/period.glif
--rw-r--r--  2.0 unx     1357 b- defN 23-Jul-31 17:57 fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/E_.glif
--rw-r--r--  2.0 unx      193 b- defN 23-Jul-31 17:57 fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/quotesinglbase.glif
--rw-r--r--  2.0 unx      517 b- defN 23-Jul-31 17:57 fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/arrowup.glif
--rw-r--r--  2.0 unx      181 b- defN 23-Jul-31 17:57 fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs.master_width_695.65_weight_166.38/contents.plist
--rw-r--r--  2.0 unx      236 b- defN 23-Jul-31 17:57 fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs.master_width_695.65_weight_166.38/layerinfo.plist
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-31 17:57 fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansIntermediateCondensed.ufo/glyphs.background/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-31 17:57 fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansIntermediateCondensed.ufo/glyphs.reference.interpolation/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-31 17:57 fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansIntermediateCondensed.ufo/glyphs/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-31 17:57 fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansIntermediateCondensed.ufo/glyphs.interpolation/
--rw-r--r--  2.0 unx       68 b- defN 23-Jul-31 17:57 fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansIntermediateCondensed.ufo/features.fea
--rw-r--r--  2.0 unx      615 b- defN 23-Jul-31 17:57 fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansIntermediateCondensed.ufo/layercontents.plist
--rw-r--r--  2.0 unx     1386 b- defN 23-Jul-31 17:57 fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansIntermediateCondensed.ufo/fontinfo.plist
--rw-r--r--  2.0 unx      318 b- defN 23-Jul-31 17:57 fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansIntermediateCondensed.ufo/metainfo.plist
--rw-r--r--  2.0 unx    16617 b- defN 23-Jul-31 17:57 fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansIntermediateCondensed.ufo/lib.plist
--rw-r--r--  2.0 unx      228 b- defN 23-Jul-31 17:57 fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansIntermediateCondensed.ufo/glyphs.background/contents.plist
--rw-r--r--  2.0 unx     2353 b- defN 23-Jul-31 17:57 fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansIntermediateCondensed.ufo/glyphs.background/S_.glif
--rw-r--r--  2.0 unx      343 b- defN 23-Jul-31 17:57 fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansIntermediateCondensed.ufo/glyphs.background/layerinfo.plist
--rw-r--r--  2.0 unx      268 b- defN 23-Jul-31 17:57 fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansIntermediateCondensed.ufo/glyphs.reference.interpolation/contents.plist
--rw-r--r--  2.0 unx     3181 b- defN 23-Jul-31 17:57 fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansIntermediateCondensed.ufo/glyphs.reference.interpolation/S_.glif
--rw-r--r--  2.0 unx      341 b- defN 23-Jul-31 17:57 fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansIntermediateCondensed.ufo/glyphs.reference.interpolation/layerinfo.plist
--rw-r--r--  2.0 unx      950 b- defN 23-Jul-31 17:57 fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansIntermediateCondensed.ufo/glyphs.reference.interpolation/E_.glif
--rw-r--r--  2.0 unx     2307 b- defN 23-Jul-31 17:57 fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansIntermediateCondensed.ufo/glyphs/G_.glif
--rw-r--r--  2.0 unx      923 b- defN 23-Jul-31 17:57 fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansIntermediateCondensed.ufo/glyphs/F_.glif
--rw-r--r--  2.0 unx     1806 b- defN 23-Jul-31 17:57 fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansIntermediateCondensed.ufo/glyphs/B_.glif
--rw-r--r--  2.0 unx      422 b- defN 23-Jul-31 17:57 fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansIntermediateCondensed.ufo/glyphs/contents.plist
--rw-r--r--  2.0 unx     2646 b- defN 23-Jul-31 17:57 fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansIntermediateCondensed.ufo/glyphs/S_.glif
--rw-r--r--  2.0 unx      371 b- defN 23-Jul-31 17:57 fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansIntermediateCondensed.ufo/glyphs/layerinfo.plist
--rw-r--r--  2.0 unx      983 b- defN 23-Jul-31 17:57 fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansIntermediateCondensed.ufo/glyphs/E_.glif
--rw-r--r--  2.0 unx      228 b- defN 23-Jul-31 17:57 fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansIntermediateCondensed.ufo/glyphs.interpolation/contents.plist
--rw-r--r--  2.0 unx      344 b- defN 23-Jul-31 17:57 fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansIntermediateCondensed.ufo/glyphs.interpolation/layerinfo.plist
--rw-r--r--  2.0 unx     1938 b- defN 23-Jul-31 17:57 fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansIntermediateCondensed.ufo/glyphs.interpolation/E_.glif
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-31 17:57 fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs.background/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-31 17:57 fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/
--rw-r--r--  2.0 unx       42 b- defN 23-Jul-31 17:57 fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/features.fea
--rw-r--r--  2.0 unx      383 b- defN 23-Jul-31 17:57 fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/layercontents.plist
--rw-r--r--  2.0 unx      366 b- defN 23-Jul-31 17:57 fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/groups.plist
--rw-r--r--  2.0 unx     4580 b- defN 23-Jul-31 17:57 fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/kerning.plist
--rw-r--r--  2.0 unx     1885 b- defN 23-Jul-31 17:57 fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/fontinfo.plist
--rw-r--r--  2.0 unx      318 b- defN 23-Jul-31 17:57 fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/metainfo.plist
--rw-r--r--  2.0 unx     7840 b- defN 23-Jul-31 17:57 fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/lib.plist
--rw-r--r--  2.0 unx     1988 b- defN 23-Jul-31 17:57 fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs.background/S_.closed.glif
--rw-r--r--  2.0 unx      252 b- defN 23-Jul-31 17:57 fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs.background/contents.plist
--rw-r--r--  2.0 unx      246 b- defN 23-Jul-31 17:57 fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs.background/layerinfo.plist
--rw-r--r--  2.0 unx      858 b- defN 23-Jul-31 17:57 fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/W_.glif
--rw-r--r--  2.0 unx      325 b- defN 23-Jul-31 17:57 fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/quotedblleft.glif
--rw-r--r--  2.0 unx      546 b- defN 23-Jul-31 17:57 fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/T_.glif
--rw-r--r--  2.0 unx     1829 b- defN 23-Jul-31 17:57 fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/R_.glif
--rw-r--r--  2.0 unx     1359 b- defN 23-Jul-31 17:57 fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/O_.glif
--rw-r--r--  2.0 unx     1774 b- defN 23-Jul-31 17:57 fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/G_.glif
--rw-r--r--  2.0 unx     1128 b- defN 23-Jul-31 17:57 fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/D_.glif
--rw-r--r--  2.0 unx     2285 b- defN 23-Jul-31 17:57 fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/S_.closed.glif
--rw-r--r--  2.0 unx      242 b- defN 23-Jul-31 17:57 fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/colon.glif
--rw-r--r--  2.0 unx      800 b- defN 23-Jul-31 17:57 fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/X_.glif
--rw-r--r--  2.0 unx      915 b- defN 23-Jul-31 17:57 fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/M_.glif
--rw-r--r--  2.0 unx      744 b- defN 23-Jul-31 17:57 fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/Z_.glif
--rw-r--r--  2.0 unx      701 b- defN 23-Jul-31 17:57 fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/I_.narrow.glif
--rw-r--r--  2.0 unx      747 b- defN 23-Jul-31 17:57 fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/F_.glif
--rw-r--r--  2.0 unx     1785 b- defN 23-Jul-31 17:57 fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/C_.glif
--rw-r--r--  2.0 unx      351 b- defN 23-Jul-31 17:57 fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/dot.glif
--rw-r--r--  2.0 unx      491 b- defN 23-Jul-31 17:57 fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/arrowright.glif
--rw-r--r--  2.0 unx     1799 b- defN 23-Jul-31 17:57 fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/B_.glif
--rw-r--r--  2.0 unx      936 b- defN 23-Jul-31 17:57 fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/U_.glif
--rw-r--r--  2.0 unx      741 b- defN 23-Jul-31 17:57 fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/I_.glif
--rw-r--r--  2.0 unx      741 b- defN 23-Jul-31 17:57 fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/N_.glif
--rw-r--r--  2.0 unx      740 b- defN 23-Jul-31 17:57 fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/V_.glif
--rw-r--r--  2.0 unx     1137 b- defN 23-Jul-31 17:57 fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/I_J_.glif
--rw-r--r--  2.0 unx      521 b- defN 23-Jul-31 17:57 fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/comma.glif
--rw-r--r--  2.0 unx     2687 b- defN 23-Jul-31 17:57 fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/contents.plist
--rw-r--r--  2.0 unx      384 b- defN 23-Jul-31 17:57 fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/dieresis.glif
--rw-r--r--  2.0 unx      748 b- defN 23-Jul-31 17:57 fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/Y_.glif
--rw-r--r--  2.0 unx      379 b- defN 23-Jul-31 17:57 fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/Q_.glif
--rw-r--r--  2.0 unx      154 b- defN 23-Jul-31 17:57 fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/space.glif
--rw-r--r--  2.0 unx      608 b- defN 23-Jul-31 17:57 fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/quotedblbase.glif
--rw-r--r--  2.0 unx      542 b- defN 23-Jul-31 17:57 fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/L_.glif
--rw-r--r--  2.0 unx      264 b- defN 23-Jul-31 17:57 fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/quotedblright.glif
--rw-r--r--  2.0 unx      340 b- defN 23-Jul-31 17:57 fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/A_acute.glif
--rw-r--r--  2.0 unx      491 b- defN 23-Jul-31 17:57 fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/arrowdown.glif
--rw-r--r--  2.0 unx     1204 b- defN 23-Jul-31 17:57 fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/P_.glif
--rw-r--r--  2.0 unx      245 b- defN 23-Jul-31 17:57 fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/semicolon.glif
--rw-r--r--  2.0 unx      825 b- defN 23-Jul-31 17:57 fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/J_.narrow.glif
--rw-r--r--  2.0 unx      346 b- defN 23-Jul-31 17:57 fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/A_dieresis.glif
--rw-r--r--  2.0 unx      490 b- defN 23-Jul-31 17:57 fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/arrowleft.glif
--rw-r--r--  2.0 unx      872 b- defN 23-Jul-31 17:57 fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/K_.glif
--rw-r--r--  2.0 unx     1319 b- defN 23-Jul-31 17:57 fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/A_.glif
--rw-r--r--  2.0 unx      936 b- defN 23-Jul-31 17:57 fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/J_.glif
--rw-r--r--  2.0 unx      743 b- defN 23-Jul-31 17:57 fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/H_.glif
--rw-r--r--  2.0 unx     2367 b- defN 23-Jul-31 17:57 fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/S_.glif
--rw-r--r--  2.0 unx      353 b- defN 23-Jul-31 17:57 fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/acute.glif
--rw-r--r--  2.0 unx      371 b- defN 23-Jul-31 17:57 fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/layerinfo.plist
--rw-r--r--  2.0 unx      350 b- defN 23-Jul-31 17:57 fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/period.glif
--rw-r--r--  2.0 unx     1382 b- defN 23-Jul-31 17:57 fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/E_.glif
--rw-r--r--  2.0 unx      566 b- defN 23-Jul-31 17:57 fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/quotesinglbase.glif
--rw-r--r--  2.0 unx      490 b- defN 23-Jul-31 17:57 fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/arrowup.glif
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-31 17:57 fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansIntermediateWide.ufo/glyphs.background/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-31 17:57 fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansIntermediateWide.ufo/glyphs/
--rw-r--r--  2.0 unx       68 b- defN 23-Jul-31 17:57 fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansIntermediateWide.ufo/features.fea
--rw-r--r--  2.0 unx      383 b- defN 23-Jul-31 17:57 fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansIntermediateWide.ufo/layercontents.plist
--rw-r--r--  2.0 unx     5462 b- defN 23-Jul-31 17:57 fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansIntermediateWide.ufo/kerning.plist
--rw-r--r--  2.0 unx     1384 b- defN 23-Jul-31 17:57 fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansIntermediateWide.ufo/fontinfo.plist
--rw-r--r--  2.0 unx      318 b- defN 23-Jul-31 17:57 fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansIntermediateWide.ufo/metainfo.plist
--rw-r--r--  2.0 unx    16223 b- defN 23-Jul-31 17:57 fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansIntermediateWide.ufo/lib.plist
--rw-r--r--  2.0 unx      228 b- defN 23-Jul-31 17:57 fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansIntermediateWide.ufo/glyphs.background/contents.plist
--rw-r--r--  2.0 unx     2396 b- defN 23-Jul-31 17:57 fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansIntermediateWide.ufo/glyphs.background/S_.glif
--rw-r--r--  2.0 unx      343 b- defN 23-Jul-31 17:57 fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansIntermediateWide.ufo/glyphs.background/layerinfo.plist
--rw-r--r--  2.0 unx     2148 b- defN 23-Jul-31 17:57 fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansIntermediateWide.ufo/glyphs/G_.glif
--rw-r--r--  2.0 unx      911 b- defN 23-Jul-31 17:57 fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansIntermediateWide.ufo/glyphs/F_.glif
--rw-r--r--  2.0 unx     1824 b- defN 23-Jul-31 17:57 fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansIntermediateWide.ufo/glyphs/B_.glif
--rw-r--r--  2.0 unx      376 b- defN 23-Jul-31 17:57 fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansIntermediateWide.ufo/glyphs/contents.plist
--rw-r--r--  2.0 unx      371 b- defN 23-Jul-31 17:57 fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansIntermediateWide.ufo/glyphs/layerinfo.plist
--rw-r--r--  2.0 unx     1162 b- defN 23-Jul-31 17:57 fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansIntermediateWide.ufo/glyphs/E_.glif
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-31 17:57 fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs.background/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-31 17:57 fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/
--rw-r--r--  2.0 unx       36 b- defN 23-Jul-31 17:57 fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansBoldWide.ufo/features.fea
--rw-r--r--  2.0 unx      383 b- defN 23-Jul-31 17:57 fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansBoldWide.ufo/layercontents.plist
--rw-r--r--  2.0 unx      366 b- defN 23-Jul-31 17:57 fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansBoldWide.ufo/groups.plist
--rw-r--r--  2.0 unx      301 b- defN 23-Jul-31 17:57 fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansBoldWide.ufo/kerning.plist
--rw-r--r--  2.0 unx     1870 b- defN 23-Jul-31 17:57 fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansBoldWide.ufo/fontinfo.plist
--rw-r--r--  2.0 unx      318 b- defN 23-Jul-31 17:57 fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansBoldWide.ufo/metainfo.plist
--rw-r--r--  2.0 unx    12341 b- defN 23-Jul-31 17:57 fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansBoldWide.ufo/lib.plist
--rw-r--r--  2.0 unx     1986 b- defN 23-Jul-31 17:57 fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs.background/S_.closed.glif
--rw-r--r--  2.0 unx      298 b- defN 23-Jul-31 17:57 fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs.background/contents.plist
--rw-r--r--  2.0 unx     2005 b- defN 23-Jul-31 17:57 fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs.background/S_.glif
--rw-r--r--  2.0 unx      246 b- defN 23-Jul-31 17:57 fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs.background/layerinfo.plist
--rw-r--r--  2.0 unx      861 b- defN 23-Jul-31 17:57 fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/W_.glif
--rw-r--r--  2.0 unx      325 b- defN 23-Jul-31 17:57 fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/quotedblleft.glif
--rw-r--r--  2.0 unx      549 b- defN 23-Jul-31 17:57 fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/T_.glif
--rw-r--r--  2.0 unx     1495 b- defN 23-Jul-31 17:57 fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/R_.glif
--rw-r--r--  2.0 unx     1387 b- defN 23-Jul-31 17:57 fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/O_.glif
--rw-r--r--  2.0 unx     1747 b- defN 23-Jul-31 17:57 fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/G_.glif
--rw-r--r--  2.0 unx     1150 b- defN 23-Jul-31 17:57 fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/D_.glif
--rw-r--r--  2.0 unx     2369 b- defN 23-Jul-31 17:57 fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/S_.closed.glif
--rw-r--r--  2.0 unx      242 b- defN 23-Jul-31 17:57 fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/colon.glif
--rw-r--r--  2.0 unx      803 b- defN 23-Jul-31 17:57 fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/X_.glif
--rw-r--r--  2.0 unx      919 b- defN 23-Jul-31 17:57 fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/M_.glif
--rw-r--r--  2.0 unx      750 b- defN 23-Jul-31 17:57 fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/Z_.glif
--rw-r--r--  2.0 unx      701 b- defN 23-Jul-31 17:57 fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/I_.narrow.glif
--rw-r--r--  2.0 unx      750 b- defN 23-Jul-31 17:57 fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/F_.glif
--rw-r--r--  2.0 unx     1418 b- defN 23-Jul-31 17:57 fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/C_.glif
--rw-r--r--  2.0 unx      351 b- defN 23-Jul-31 17:57 fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/dot.glif
--rw-r--r--  2.0 unx      495 b- defN 23-Jul-31 17:57 fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/arrowright.glif
--rw-r--r--  2.0 unx     2203 b- defN 23-Jul-31 17:57 fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/B_.glif
--rw-r--r--  2.0 unx     1037 b- defN 23-Jul-31 17:57 fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/U_.glif
--rw-r--r--  2.0 unx      742 b- defN 23-Jul-31 17:57 fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/I_.glif
--rw-r--r--  2.0 unx      745 b- defN 23-Jul-31 17:57 fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/N_.glif
--rw-r--r--  2.0 unx      742 b- defN 23-Jul-31 17:57 fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/V_.glif
--rw-r--r--  2.0 unx     1154 b- defN 23-Jul-31 17:57 fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/I_J_.glif
--rw-r--r--  2.0 unx      522 b- defN 23-Jul-31 17:57 fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/comma.glif
--rw-r--r--  2.0 unx     2687 b- defN 23-Jul-31 17:57 fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/contents.plist
--rw-r--r--  2.0 unx      370 b- defN 23-Jul-31 17:57 fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/dieresis.glif
--rw-r--r--  2.0 unx      750 b- defN 23-Jul-31 17:57 fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/Y_.glif
--rw-r--r--  2.0 unx      380 b- defN 23-Jul-31 17:57 fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/Q_.glif
--rw-r--r--  2.0 unx      154 b- defN 23-Jul-31 17:57 fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/space.glif
--rw-r--r--  2.0 unx      259 b- defN 23-Jul-31 17:57 fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/quotedblbase.glif
--rw-r--r--  2.0 unx      545 b- defN 23-Jul-31 17:57 fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/L_.glif
--rw-r--r--  2.0 unx      264 b- defN 23-Jul-31 17:57 fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/quotedblright.glif
--rw-r--r--  2.0 unx      354 b- defN 23-Jul-31 17:57 fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/A_acute.glif
--rw-r--r--  2.0 unx      491 b- defN 23-Jul-31 17:57 fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/arrowdown.glif
--rw-r--r--  2.0 unx     1140 b- defN 23-Jul-31 17:57 fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/P_.glif
--rw-r--r--  2.0 unx      245 b- defN 23-Jul-31 17:57 fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/semicolon.glif
--rw-r--r--  2.0 unx      806 b- defN 23-Jul-31 17:57 fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/J_.narrow.glif
--rw-r--r--  2.0 unx      360 b- defN 23-Jul-31 17:57 fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/A_dieresis.glif
--rw-r--r--  2.0 unx      493 b- defN 23-Jul-31 17:57 fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/arrowleft.glif
--rw-r--r--  2.0 unx      875 b- defN 23-Jul-31 17:57 fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/K_.glif
--rw-r--r--  2.0 unx      947 b- defN 23-Jul-31 17:57 fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/A_.glif
--rw-r--r--  2.0 unx      940 b- defN 23-Jul-31 17:57 fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/J_.glif
--rw-r--r--  2.0 unx      748 b- defN 23-Jul-31 17:57 fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/H_.glif
--rw-r--r--  2.0 unx     2376 b- defN 23-Jul-31 17:57 fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/S_.glif
--rw-r--r--  2.0 unx      353 b- defN 23-Jul-31 17:57 fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/acute.glif
--rw-r--r--  2.0 unx      371 b- defN 23-Jul-31 17:57 fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/layerinfo.plist
--rw-r--r--  2.0 unx      350 b- defN 23-Jul-31 17:57 fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/period.glif
--rw-r--r--  2.0 unx      988 b- defN 23-Jul-31 17:57 fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/E_.glif
--rw-r--r--  2.0 unx      205 b- defN 23-Jul-31 17:57 fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/quotesinglbase.glif
--rw-r--r--  2.0 unx      492 b- defN 23-Jul-31 17:57 fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/arrowup.glif
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-31 17:57 fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs.background/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-31 17:57 fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs.support.crossbar/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-31 17:57 fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs.support/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-31 17:57 fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs.support.S_.middle/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-31 17:57 fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-31 17:57 fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs.support.crossbars/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-31 17:57 fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs.support.S_.wide/
--rw-r--r--  2.0 unx       68 b- defN 23-Jul-31 17:57 fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/features.fea
--rw-r--r--  2.0 unx      811 b- defN 23-Jul-31 17:57 fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/layercontents.plist
--rw-r--r--  2.0 unx      491 b- defN 23-Jul-31 17:57 fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/groups.plist
--rw-r--r--  2.0 unx      517 b- defN 23-Jul-31 17:57 fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/kerning.plist
--rw-r--r--  2.0 unx     1888 b- defN 23-Jul-31 17:57 fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/fontinfo.plist
--rw-r--r--  2.0 unx      318 b- defN 23-Jul-31 17:57 fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/metainfo.plist
--rw-r--r--  2.0 unx    18792 b- defN 23-Jul-31 17:57 fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/lib.plist
--rw-r--r--  2.0 unx     3998 b- defN 23-Jul-31 17:57 fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs.background/S_.closed.glif
--rw-r--r--  2.0 unx      298 b- defN 23-Jul-31 17:57 fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs.background/contents.plist
--rw-r--r--  2.0 unx     3358 b- defN 23-Jul-31 17:57 fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs.background/S_.glif
--rw-r--r--  2.0 unx      244 b- defN 23-Jul-31 17:57 fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs.background/layerinfo.plist
--rw-r--r--  2.0 unx     2452 b- defN 23-Jul-31 17:57 fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs.support.crossbar/G_.glif
--rw-r--r--  2.0 unx      422 b- defN 23-Jul-31 17:57 fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs.support.crossbar/S_.closed.glif
--rw-r--r--  2.0 unx      751 b- defN 23-Jul-31 17:57 fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs.support.crossbar/F_.glif
--rw-r--r--  2.0 unx     2111 b- defN 23-Jul-31 17:57 fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs.support.crossbar/B_.glif
--rw-r--r--  2.0 unx      482 b- defN 23-Jul-31 17:57 fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs.support.crossbar/contents.plist
--rw-r--r--  2.0 unx     3498 b- defN 23-Jul-31 17:57 fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs.support.crossbar/S_.glif
--rw-r--r--  2.0 unx      247 b- defN 23-Jul-31 17:57 fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs.support.crossbar/layerinfo.plist
--rw-r--r--  2.0 unx     1471 b- defN 23-Jul-31 17:57 fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs.support.crossbar/E_.glif
--rw-r--r--  2.0 unx      853 b- defN 23-Jul-31 17:57 fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs.support/W_.glif
--rw-r--r--  2.0 unx      330 b- defN 23-Jul-31 17:57 fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs.support/contents.plist
--rw-r--r--  2.0 unx      828 b- defN 23-Jul-31 17:57 fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs.support/A_.glif
--rw-r--r--  2.0 unx     2706 b- defN 23-Jul-31 17:57 fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs.support/S_.glif
--rw-r--r--  2.0 unx      371 b- defN 23-Jul-31 17:57 fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs.support/layerinfo.plist
--rw-r--r--  2.0 unx     2825 b- defN 23-Jul-31 17:57 fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs.support.S_.middle/S_.closed.glif
--rw-r--r--  2.0 unx      252 b- defN 23-Jul-31 17:57 fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs.support.S_.middle/contents.plist
--rw-r--r--  2.0 unx      246 b- defN 23-Jul-31 17:57 fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs.support.S_.middle/layerinfo.plist
--rw-r--r--  2.0 unx      853 b- defN 23-Jul-31 17:57 fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/W_.glif
--rw-r--r--  2.0 unx      325 b- defN 23-Jul-31 17:57 fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/quotedblleft.glif
--rw-r--r--  2.0 unx      546 b- defN 23-Jul-31 17:57 fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/T_.glif
--rw-r--r--  2.0 unx     1462 b- defN 23-Jul-31 17:57 fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/R_.glif
--rw-r--r--  2.0 unx     1372 b- defN 23-Jul-31 17:57 fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/O_.glif
--rw-r--r--  2.0 unx     1728 b- defN 23-Jul-31 17:57 fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/G_.glif
--rw-r--r--  2.0 unx     1136 b- defN 23-Jul-31 17:57 fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/D_.glif
--rw-r--r--  2.0 unx     1966 b- defN 23-Jul-31 17:57 fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/S_.closed.glif
--rw-r--r--  2.0 unx      230 b- defN 23-Jul-31 17:57 fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/colon.glif
--rw-r--r--  2.0 unx      798 b- defN 23-Jul-31 17:57 fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/X_.glif
--rw-r--r--  2.0 unx      914 b- defN 23-Jul-31 17:57 fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/M_.glif
--rw-r--r--  2.0 unx      739 b- defN 23-Jul-31 17:57 fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/Z_.glif
--rw-r--r--  2.0 unx      701 b- defN 23-Jul-31 17:57 fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/I_.narrow.glif
--rw-r--r--  2.0 unx      743 b- defN 23-Jul-31 17:57 fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/F_.glif
--rw-r--r--  2.0 unx     1402 b- defN 23-Jul-31 17:57 fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/C_.glif
--rw-r--r--  2.0 unx      349 b- defN 23-Jul-31 17:57 fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/dot.glif
--rw-r--r--  2.0 unx      627 b- defN 23-Jul-31 17:57 fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/arrowright.glif
--rw-r--r--  2.0 unx     1799 b- defN 23-Jul-31 17:57 fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/B_.glif
--rw-r--r--  2.0 unx      929 b- defN 23-Jul-31 17:57 fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/U_.glif
--rw-r--r--  2.0 unx      739 b- defN 23-Jul-31 17:57 fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/I_.glif
--rw-r--r--  2.0 unx      736 b- defN 23-Jul-31 17:57 fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/N_.glif
--rw-r--r--  2.0 unx      737 b- defN 23-Jul-31 17:57 fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/V_.glif
--rw-r--r--  2.0 unx     1105 b- defN 23-Jul-31 17:57 fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/I_J_.glif
--rw-r--r--  2.0 unx      515 b- defN 23-Jul-31 17:57 fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/comma.glif
--rw-r--r--  2.0 unx     2687 b- defN 23-Jul-31 17:57 fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/contents.plist
--rw-r--r--  2.0 unx      369 b- defN 23-Jul-31 17:57 fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/dieresis.glif
--rw-r--r--  2.0 unx     1120 b- defN 23-Jul-31 17:57 fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/Y_.glif
--rw-r--r--  2.0 unx      377 b- defN 23-Jul-31 17:57 fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/Q_.glif
--rw-r--r--  2.0 unx      154 b- defN 23-Jul-31 17:57 fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/space.glif
--rw-r--r--  2.0 unx      235 b- defN 23-Jul-31 17:57 fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/quotedblbase.glif
--rw-r--r--  2.0 unx      538 b- defN 23-Jul-31 17:57 fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/L_.glif
--rw-r--r--  2.0 unx      264 b- defN 23-Jul-31 17:57 fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/quotedblright.glif
--rw-r--r--  2.0 unx      352 b- defN 23-Jul-31 17:57 fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/A_acute.glif
--rw-r--r--  2.0 unx      628 b- defN 23-Jul-31 17:57 fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/arrowdown.glif
--rw-r--r--  2.0 unx     1146 b- defN 23-Jul-31 17:57 fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/P_.glif
--rw-r--r--  2.0 unx      233 b- defN 23-Jul-31 17:57 fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/semicolon.glif
--rw-r--r--  2.0 unx      797 b- defN 23-Jul-31 17:57 fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/J_.narrow.glif
--rw-r--r--  2.0 unx      358 b- defN 23-Jul-31 17:57 fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/A_dieresis.glif
--rw-r--r--  2.0 unx      690 b- defN 23-Jul-31 17:57 fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/arrowleft.glif
--rw-r--r--  2.0 unx      870 b- defN 23-Jul-31 17:57 fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/K_.glif
--rw-r--r--  2.0 unx      942 b- defN 23-Jul-31 17:57 fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/A_.glif
--rw-r--r--  2.0 unx      929 b- defN 23-Jul-31 17:57 fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/J_.glif
--rw-r--r--  2.0 unx      741 b- defN 23-Jul-31 17:57 fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/H_.glif
--rw-r--r--  2.0 unx     2453 b- defN 23-Jul-31 17:57 fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/S_.glif
--rw-r--r--  2.0 unx      353 b- defN 23-Jul-31 17:57 fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/acute.glif
--rw-r--r--  2.0 unx      371 b- defN 23-Jul-31 17:57 fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/layerinfo.plist
--rw-r--r--  2.0 unx      350 b- defN 23-Jul-31 17:57 fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/period.glif
--rw-r--r--  2.0 unx      975 b- defN 23-Jul-31 17:57 fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/E_.glif
--rw-r--r--  2.0 unx      193 b- defN 23-Jul-31 17:57 fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/quotesinglbase.glif
--rw-r--r--  2.0 unx      626 b- defN 23-Jul-31 17:57 fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/arrowup.glif
--rw-r--r--  2.0 unx      238 b- defN 23-Jul-31 17:57 fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs.support.crossbars/contents.plist
--rw-r--r--  2.0 unx      183 b- defN 23-Jul-31 17:57 fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs.support.crossbars/layerinfo.plist
--rw-r--r--  2.0 unx     1176 b- defN 23-Jul-31 17:57 fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs.support.crossbars/E_.glif
--rw-r--r--  2.0 unx     3543 b- defN 23-Jul-31 17:57 fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs.support.S_.wide/S_.closed.glif
--rw-r--r--  2.0 unx      298 b- defN 23-Jul-31 17:57 fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs.support.S_.wide/contents.plist
--rw-r--r--  2.0 unx     3534 b- defN 23-Jul-31 17:57 fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs.support.S_.wide/S_.glif
--rw-r--r--  2.0 unx      247 b- defN 23-Jul-31 17:57 fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs.support.S_.wide/layerinfo.plist
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-31 17:57 fontmake-3.7.0b3/tests/data/MutatorSansLite/MutatorSansLightWide.ufo/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-31 17:57 fontmake-3.7.0b3/tests/data/MutatorSansLite/MutatorSerifLightWide.ufo/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-31 17:57 fontmake-3.7.0b3/tests/data/MutatorSansLite/MutatorSansBoldCondensed.ufo/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-31 17:57 fontmake-3.7.0b3/tests/data/MutatorSansLite/MutatorSerifLightCondensed.ufo/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-31 17:57 fontmake-3.7.0b3/tests/data/MutatorSansLite/MutatorSansBoldWide.ufo/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-31 17:57 fontmake-3.7.0b3/tests/data/MutatorSansLite/MutatorSansLightCondensed.ufo/
--rw-r--r--  2.0 unx     5741 b- defN 23-Jul-31 17:57 fontmake-3.7.0b3/tests/data/MutatorSansLite/MutatorSans_v5_several_vfs.designspace
--rw-r--r--  2.0 unx     5180 b- defN 23-Jul-31 17:57 fontmake-3.7.0b3/tests/data/MutatorSansLite/MutatorSans_v5_several_vfs_discrete_axis.designspace
--rw-r--r--  2.0 unx     5197 b- defN 23-Jul-31 17:57 fontmake-3.7.0b3/tests/data/MutatorSansLite/MutatorSans_v5_implicit_one_vf.designspace
--rw-r--r--  2.0 unx     1074 b- defN 23-Jul-31 17:57 fontmake-3.7.0b3/tests/data/MutatorSansLite/LICENSE
--rw-r--r--  2.0 unx     7158 b- defN 23-Jul-31 17:57 fontmake-3.7.0b3/tests/data/MutatorSansLite/MutatorFamily_v5_discrete_axis.designspace
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-31 17:57 fontmake-3.7.0b3/tests/data/MutatorSansLite/MutatorSansLightWide.ufo/glyphs.background/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-31 17:57 fontmake-3.7.0b3/tests/data/MutatorSansLite/MutatorSansLightWide.ufo/glyphs.master_width_720.00_weight_645.00/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-31 17:57 fontmake-3.7.0b3/tests/data/MutatorSansLite/MutatorSansLightWide.ufo/glyphs.master_width_0.00_weight_0.00/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-31 17:57 fontmake-3.7.0b3/tests/data/MutatorSansLite/MutatorSansLightWide.ufo/glyphs.master_width_500.00_weight_500.00/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-31 17:57 fontmake-3.7.0b3/tests/data/MutatorSansLite/MutatorSansLightWide.ufo/glyphs/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-31 17:57 fontmake-3.7.0b3/tests/data/MutatorSansLite/MutatorSansLightWide.ufo/glyphs.master_width_695.65_weight_166.38/
--rw-r--r--  2.0 unx       37 b- defN 23-Jul-31 17:57 fontmake-3.7.0b3/tests/data/MutatorSansLite/MutatorSansLightWide.ufo/features.fea
--rw-r--r--  2.0 unx      361 b- defN 23-Jul-31 17:57 fontmake-3.7.0b3/tests/data/MutatorSansLite/MutatorSansLightWide.ufo/layercontents.plist
--rw-r--r--  2.0 unx     1829 b- defN 23-Jul-31 17:57 fontmake-3.7.0b3/tests/data/MutatorSansLite/MutatorSansLightWide.ufo/fontinfo.plist
--rw-r--r--  2.0 unx      308 b- defN 23-Jul-31 17:57 fontmake-3.7.0b3/tests/data/MutatorSansLite/MutatorSansLightWide.ufo/metainfo.plist
--rw-r--r--  2.0 unx    16116 b- defN 23-Jul-31 17:57 fontmake-3.7.0b3/tests/data/MutatorSansLite/MutatorSansLightWide.ufo/lib.plist
--rw-r--r--  2.0 unx     1818 b- defN 23-Jul-31 17:57 fontmake-3.7.0b3/tests/data/MutatorSansLite/MutatorSansLightWide.ufo/glyphs.background/S_.closed.glif
--rw-r--r--  2.0 unx      246 b- defN 23-Jul-31 17:57 fontmake-3.7.0b3/tests/data/MutatorSansLite/MutatorSansLightWide.ufo/glyphs.background/contents.plist
--rw-r--r--  2.0 unx      240 b- defN 23-Jul-31 17:57 fontmake-3.7.0b3/tests/data/MutatorSansLite/MutatorSansLightWide.ufo/glyphs.background/layerinfo.plist
--rw-r--r--  2.0 unx      228 b- defN 23-Jul-31 17:57 fontmake-3.7.0b3/tests/data/MutatorSansLite/MutatorSansLightWide.ufo/glyphs.master_width_720.00_weight_645.00/contents.plist
--rw-r--r--  2.0 unx     2537 b- defN 23-Jul-31 17:57 fontmake-3.7.0b3/tests/data/MutatorSansLite/MutatorSansLightWide.ufo/glyphs.master_width_720.00_weight_645.00/S_.glif
--rw-r--r--  2.0 unx      341 b- defN 23-Jul-31 17:57 fontmake-3.7.0b3/tests/data/MutatorSansLite/MutatorSansLightWide.ufo/glyphs.master_width_720.00_weight_645.00/layerinfo.plist
--rw-r--r--  2.0 unx      181 b- defN 23-Jul-31 17:57 fontmake-3.7.0b3/tests/data/MutatorSansLite/MutatorSansLightWide.ufo/glyphs.master_width_0.00_weight_0.00/contents.plist
--rw-r--r--  2.0 unx      237 b- defN 23-Jul-31 17:57 fontmake-3.7.0b3/tests/data/MutatorSansLite/MutatorSansLightWide.ufo/glyphs.master_width_0.00_weight_0.00/layerinfo.plist
--rw-r--r--  2.0 unx      228 b- defN 23-Jul-31 17:57 fontmake-3.7.0b3/tests/data/MutatorSansLite/MutatorSansLightWide.ufo/glyphs.master_width_500.00_weight_500.00/contents.plist
--rw-r--r--  2.0 unx     2459 b- defN 23-Jul-31 17:57 fontmake-3.7.0b3/tests/data/MutatorSansLite/MutatorSansLightWide.ufo/glyphs.master_width_500.00_weight_500.00/S_.glif
--rw-r--r--  2.0 unx      344 b- defN 23-Jul-31 17:57 fontmake-3.7.0b3/tests/data/MutatorSansLite/MutatorSansLightWide.ufo/glyphs.master_width_500.00_weight_500.00/layerinfo.plist
--rw-r--r--  2.0 unx     1831 b- defN 23-Jul-31 17:57 fontmake-3.7.0b3/tests/data/MutatorSansLite/MutatorSansLightWide.ufo/glyphs/S_.closed.glif
--rw-r--r--  2.0 unx      654 b- defN 23-Jul-31 17:57 fontmake-3.7.0b3/tests/data/MutatorSansLite/MutatorSansLightWide.ufo/glyphs/I_.narrow.glif
--rw-r--r--  2.0 unx      691 b- defN 23-Jul-31 17:57 fontmake-3.7.0b3/tests/data/MutatorSansLite/MutatorSansLightWide.ufo/glyphs/I_.glif
--rw-r--r--  2.0 unx     1065 b- defN 23-Jul-31 17:57 fontmake-3.7.0b3/tests/data/MutatorSansLite/MutatorSansLightWide.ufo/glyphs/I_J_.glif
--rw-r--r--  2.0 unx      473 b- defN 23-Jul-31 17:57 fontmake-3.7.0b3/tests/data/MutatorSansLite/MutatorSansLightWide.ufo/glyphs/contents.plist
--rw-r--r--  2.0 unx     1222 b- defN 23-Jul-31 17:57 fontmake-3.7.0b3/tests/data/MutatorSansLite/MutatorSansLightWide.ufo/glyphs/A_.glif
--rw-r--r--  2.0 unx     2188 b- defN 23-Jul-31 17:57 fontmake-3.7.0b3/tests/data/MutatorSansLite/MutatorSansLightWide.ufo/glyphs/S_.glif
--rw-r--r--  2.0 unx      353 b- defN 23-Jul-31 17:57 fontmake-3.7.0b3/tests/data/MutatorSansLite/MutatorSansLightWide.ufo/glyphs/layerinfo.plist
--rw-r--r--  2.0 unx      181 b- defN 23-Jul-31 17:57 fontmake-3.7.0b3/tests/data/MutatorSansLite/MutatorSansLightWide.ufo/glyphs.master_width_695.65_weight_166.38/contents.plist
--rw-r--r--  2.0 unx      236 b- defN 23-Jul-31 17:57 fontmake-3.7.0b3/tests/data/MutatorSansLite/MutatorSansLightWide.ufo/glyphs.master_width_695.65_weight_166.38/layerinfo.plist
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-31 17:57 fontmake-3.7.0b3/tests/data/MutatorSansLite/MutatorSerifLightWide.ufo/glyphs/
--rw-r--r--  2.0 unx       37 b- defN 23-Jul-31 17:57 fontmake-3.7.0b3/tests/data/MutatorSansLite/MutatorSerifLightWide.ufo/features.fea
--rw-r--r--  2.0 unx      271 b- defN 23-Jul-31 17:57 fontmake-3.7.0b3/tests/data/MutatorSansLite/MutatorSerifLightWide.ufo/layercontents.plist
--rw-r--r--  2.0 unx     1834 b- defN 23-Jul-31 17:57 fontmake-3.7.0b3/tests/data/MutatorSansLite/MutatorSerifLightWide.ufo/fontinfo.plist
--rw-r--r--  2.0 unx      308 b- defN 23-Jul-31 17:57 fontmake-3.7.0b3/tests/data/MutatorSansLite/MutatorSerifLightWide.ufo/metainfo.plist
--rw-r--r--  2.0 unx    16116 b- defN 23-Jul-31 17:57 fontmake-3.7.0b3/tests/data/MutatorSansLite/MutatorSerifLightWide.ufo/lib.plist
--rw-r--r--  2.0 unx      232 b- defN 23-Jul-31 17:57 fontmake-3.7.0b3/tests/data/MutatorSansLite/MutatorSerifLightWide.ufo/glyphs/contents.plist
--rw-r--r--  2.0 unx     1578 b- defN 23-Jul-31 17:57 fontmake-3.7.0b3/tests/data/MutatorSansLite/MutatorSerifLightWide.ufo/glyphs/A_.glif
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-31 17:57 fontmake-3.7.0b3/tests/data/MutatorSansLite/MutatorSansBoldCondensed.ufo/glyphs.background/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-31 17:57 fontmake-3.7.0b3/tests/data/MutatorSansLite/MutatorSansBoldCondensed.ufo/glyphs/
--rw-r--r--  2.0 unx       42 b- defN 23-Jul-31 17:57 fontmake-3.7.0b3/tests/data/MutatorSansLite/MutatorSansBoldCondensed.ufo/features.fea
--rw-r--r--  2.0 unx      361 b- defN 23-Jul-31 17:57 fontmake-3.7.0b3/tests/data/MutatorSansLite/MutatorSansBoldCondensed.ufo/layercontents.plist
--rw-r--r--  2.0 unx     1841 b- defN 23-Jul-31 17:57 fontmake-3.7.0b3/tests/data/MutatorSansLite/MutatorSansBoldCondensed.ufo/fontinfo.plist
--rw-r--r--  2.0 unx      308 b- defN 23-Jul-31 17:57 fontmake-3.7.0b3/tests/data/MutatorSansLite/MutatorSansBoldCondensed.ufo/metainfo.plist
--rw-r--r--  2.0 unx     6839 b- defN 23-Jul-31 17:57 fontmake-3.7.0b3/tests/data/MutatorSansLite/MutatorSansBoldCondensed.ufo/lib.plist
--rw-r--r--  2.0 unx     1849 b- defN 23-Jul-31 17:57 fontmake-3.7.0b3/tests/data/MutatorSansLite/MutatorSansBoldCondensed.ufo/glyphs.background/S_.closed.glif
--rw-r--r--  2.0 unx      246 b- defN 23-Jul-31 17:57 fontmake-3.7.0b3/tests/data/MutatorSansLite/MutatorSansBoldCondensed.ufo/glyphs.background/contents.plist
--rw-r--r--  2.0 unx      240 b- defN 23-Jul-31 17:57 fontmake-3.7.0b3/tests/data/MutatorSansLite/MutatorSansBoldCondensed.ufo/glyphs.background/layerinfo.plist
--rw-r--r--  2.0 unx     2099 b- defN 23-Jul-31 17:57 fontmake-3.7.0b3/tests/data/MutatorSansLite/MutatorSansBoldCondensed.ufo/glyphs/S_.closed.glif
--rw-r--r--  2.0 unx      652 b- defN 23-Jul-31 17:57 fontmake-3.7.0b3/tests/data/MutatorSansLite/MutatorSansBoldCondensed.ufo/glyphs/I_.narrow.glif
--rw-r--r--  2.0 unx      689 b- defN 23-Jul-31 17:57 fontmake-3.7.0b3/tests/data/MutatorSansLite/MutatorSansBoldCondensed.ufo/glyphs/I_.glif
--rw-r--r--  2.0 unx     1057 b- defN 23-Jul-31 17:57 fontmake-3.7.0b3/tests/data/MutatorSansLite/MutatorSansBoldCondensed.ufo/glyphs/I_J_.glif
--rw-r--r--  2.0 unx      473 b- defN 23-Jul-31 17:57 fontmake-3.7.0b3/tests/data/MutatorSansLite/MutatorSansBoldCondensed.ufo/glyphs/contents.plist
--rw-r--r--  2.0 unx     1221 b- defN 23-Jul-31 17:57 fontmake-3.7.0b3/tests/data/MutatorSansLite/MutatorSansBoldCondensed.ufo/glyphs/A_.glif
--rw-r--r--  2.0 unx     2197 b- defN 23-Jul-31 17:57 fontmake-3.7.0b3/tests/data/MutatorSansLite/MutatorSansBoldCondensed.ufo/glyphs/S_.glif
--rw-r--r--  2.0 unx      353 b- defN 23-Jul-31 17:57 fontmake-3.7.0b3/tests/data/MutatorSansLite/MutatorSansBoldCondensed.ufo/glyphs/layerinfo.plist
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-31 17:57 fontmake-3.7.0b3/tests/data/MutatorSansLite/MutatorSerifLightCondensed.ufo/glyphs/
--rw-r--r--  2.0 unx       68 b- defN 23-Jul-31 17:57 fontmake-3.7.0b3/tests/data/MutatorSansLite/MutatorSerifLightCondensed.ufo/features.fea
--rw-r--r--  2.0 unx      271 b- defN 23-Jul-31 17:57 fontmake-3.7.0b3/tests/data/MutatorSansLite/MutatorSerifLightCondensed.ufo/layercontents.plist
--rw-r--r--  2.0 unx     1849 b- defN 23-Jul-31 17:57 fontmake-3.7.0b3/tests/data/MutatorSansLite/MutatorSerifLightCondensed.ufo/fontinfo.plist
--rw-r--r--  2.0 unx      308 b- defN 23-Jul-31 17:57 fontmake-3.7.0b3/tests/data/MutatorSansLite/MutatorSerifLightCondensed.ufo/metainfo.plist
--rw-r--r--  2.0 unx    16556 b- defN 23-Jul-31 17:57 fontmake-3.7.0b3/tests/data/MutatorSansLite/MutatorSerifLightCondensed.ufo/lib.plist
--rw-r--r--  2.0 unx      232 b- defN 23-Jul-31 17:57 fontmake-3.7.0b3/tests/data/MutatorSansLite/MutatorSerifLightCondensed.ufo/glyphs/contents.plist
--rw-r--r--  2.0 unx     1228 b- defN 23-Jul-31 17:57 fontmake-3.7.0b3/tests/data/MutatorSansLite/MutatorSerifLightCondensed.ufo/glyphs/A_.glif
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-31 17:57 fontmake-3.7.0b3/tests/data/MutatorSansLite/MutatorSansBoldWide.ufo/glyphs.background/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-31 17:57 fontmake-3.7.0b3/tests/data/MutatorSansLite/MutatorSansBoldWide.ufo/glyphs/
--rw-r--r--  2.0 unx       36 b- defN 23-Jul-31 17:57 fontmake-3.7.0b3/tests/data/MutatorSansLite/MutatorSansBoldWide.ufo/features.fea
--rw-r--r--  2.0 unx      361 b- defN 23-Jul-31 17:57 fontmake-3.7.0b3/tests/data/MutatorSansLite/MutatorSansBoldWide.ufo/layercontents.plist
--rw-r--r--  2.0 unx     1826 b- defN 23-Jul-31 17:57 fontmake-3.7.0b3/tests/data/MutatorSansLite/MutatorSansBoldWide.ufo/fontinfo.plist
--rw-r--r--  2.0 unx      308 b- defN 23-Jul-31 17:57 fontmake-3.7.0b3/tests/data/MutatorSansLite/MutatorSansBoldWide.ufo/metainfo.plist
--rw-r--r--  2.0 unx    10710 b- defN 23-Jul-31 17:57 fontmake-3.7.0b3/tests/data/MutatorSansLite/MutatorSansBoldWide.ufo/lib.plist
--rw-r--r--  2.0 unx     1847 b- defN 23-Jul-31 17:57 fontmake-3.7.0b3/tests/data/MutatorSansLite/MutatorSansBoldWide.ufo/glyphs.background/S_.closed.glif
--rw-r--r--  2.0 unx      288 b- defN 23-Jul-31 17:57 fontmake-3.7.0b3/tests/data/MutatorSansLite/MutatorSansBoldWide.ufo/glyphs.background/contents.plist
--rw-r--r--  2.0 unx     1865 b- defN 23-Jul-31 17:57 fontmake-3.7.0b3/tests/data/MutatorSansLite/MutatorSansBoldWide.ufo/glyphs.background/S_.glif
--rw-r--r--  2.0 unx      240 b- defN 23-Jul-31 17:57 fontmake-3.7.0b3/tests/data/MutatorSansLite/MutatorSansBoldWide.ufo/glyphs.background/layerinfo.plist
--rw-r--r--  2.0 unx     2192 b- defN 23-Jul-31 17:57 fontmake-3.7.0b3/tests/data/MutatorSansLite/MutatorSansBoldWide.ufo/glyphs/S_.closed.glif
--rw-r--r--  2.0 unx      652 b- defN 23-Jul-31 17:57 fontmake-3.7.0b3/tests/data/MutatorSansLite/MutatorSansBoldWide.ufo/glyphs/I_.narrow.glif
--rw-r--r--  2.0 unx      690 b- defN 23-Jul-31 17:57 fontmake-3.7.0b3/tests/data/MutatorSansLite/MutatorSansBoldWide.ufo/glyphs/I_.glif
--rw-r--r--  2.0 unx     1062 b- defN 23-Jul-31 17:57 fontmake-3.7.0b3/tests/data/MutatorSansLite/MutatorSansBoldWide.ufo/glyphs/I_J_.glif
--rw-r--r--  2.0 unx      473 b- defN 23-Jul-31 17:57 fontmake-3.7.0b3/tests/data/MutatorSansLite/MutatorSansBoldWide.ufo/glyphs/contents.plist
--rw-r--r--  2.0 unx      879 b- defN 23-Jul-31 17:57 fontmake-3.7.0b3/tests/data/MutatorSansLite/MutatorSansBoldWide.ufo/glyphs/A_.glif
--rw-r--r--  2.0 unx     2206 b- defN 23-Jul-31 17:57 fontmake-3.7.0b3/tests/data/MutatorSansLite/MutatorSansBoldWide.ufo/glyphs/S_.glif
--rw-r--r--  2.0 unx      353 b- defN 23-Jul-31 17:57 fontmake-3.7.0b3/tests/data/MutatorSansLite/MutatorSansBoldWide.ufo/glyphs/layerinfo.plist
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-31 17:57 fontmake-3.7.0b3/tests/data/MutatorSansLite/MutatorSansLightCondensed.ufo/glyphs.background/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-31 17:57 fontmake-3.7.0b3/tests/data/MutatorSansLite/MutatorSansLightCondensed.ufo/glyphs.support.crossbar/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-31 17:57 fontmake-3.7.0b3/tests/data/MutatorSansLite/MutatorSansLightCondensed.ufo/glyphs.support/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-31 17:57 fontmake-3.7.0b3/tests/data/MutatorSansLite/MutatorSansLightCondensed.ufo/glyphs.support.S_.middle/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-31 17:57 fontmake-3.7.0b3/tests/data/MutatorSansLite/MutatorSansLightCondensed.ufo/glyphs/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-31 17:57 fontmake-3.7.0b3/tests/data/MutatorSansLite/MutatorSansLightCondensed.ufo/glyphs.support.crossbars/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-31 17:57 fontmake-3.7.0b3/tests/data/MutatorSansLite/MutatorSansLightCondensed.ufo/glyphs.support.S_.wide/
--rw-r--r--  2.0 unx       68 b- defN 23-Jul-31 17:57 fontmake-3.7.0b3/tests/data/MutatorSansLite/MutatorSansLightCondensed.ufo/features.fea
--rw-r--r--  2.0 unx      749 b- defN 23-Jul-31 17:57 fontmake-3.7.0b3/tests/data/MutatorSansLite/MutatorSansLightCondensed.ufo/layercontents.plist
--rw-r--r--  2.0 unx     1844 b- defN 23-Jul-31 17:57 fontmake-3.7.0b3/tests/data/MutatorSansLite/MutatorSansLightCondensed.ufo/fontinfo.plist
--rw-r--r--  2.0 unx      308 b- defN 23-Jul-31 17:57 fontmake-3.7.0b3/tests/data/MutatorSansLite/MutatorSansLightCondensed.ufo/metainfo.plist
--rw-r--r--  2.0 unx    16556 b- defN 23-Jul-31 17:57 fontmake-3.7.0b3/tests/data/MutatorSansLite/MutatorSansLightCondensed.ufo/lib.plist
--rw-r--r--  2.0 unx     3539 b- defN 23-Jul-31 17:57 fontmake-3.7.0b3/tests/data/MutatorSansLite/MutatorSansLightCondensed.ufo/glyphs.background/S_.closed.glif
--rw-r--r--  2.0 unx      288 b- defN 23-Jul-31 17:57 fontmake-3.7.0b3/tests/data/MutatorSansLite/MutatorSansLightCondensed.ufo/glyphs.background/contents.plist
--rw-r--r--  2.0 unx     2617 b- defN 23-Jul-31 17:57 fontmake-3.7.0b3/tests/data/MutatorSansLite/MutatorSansLightCondensed.ufo/glyphs.background/S_.glif
--rw-r--r--  2.0 unx      238 b- defN 23-Jul-31 17:57 fontmake-3.7.0b3/tests/data/MutatorSansLite/MutatorSansLightCondensed.ufo/glyphs.background/layerinfo.plist
--rw-r--r--  2.0 unx      232 b- defN 23-Jul-31 17:57 fontmake-3.7.0b3/tests/data/MutatorSansLite/MutatorSansLightCondensed.ufo/glyphs.support.crossbar/contents.plist
--rw-r--r--  2.0 unx     3007 b- defN 23-Jul-31 17:57 fontmake-3.7.0b3/tests/data/MutatorSansLite/MutatorSansLightCondensed.ufo/glyphs.support.crossbar/S_.glif
--rw-r--r--  2.0 unx      241 b- defN 23-Jul-31 17:57 fontmake-3.7.0b3/tests/data/MutatorSansLite/MutatorSansLightCondensed.ufo/glyphs.support.crossbar/layerinfo.plist
--rw-r--r--  2.0 unx      274 b- defN 23-Jul-31 17:57 fontmake-3.7.0b3/tests/data/MutatorSansLite/MutatorSansLightCondensed.ufo/glyphs.support/contents.plist
--rw-r--r--  2.0 unx      732 b- defN 23-Jul-31 17:57 fontmake-3.7.0b3/tests/data/MutatorSansLite/MutatorSansLightCondensed.ufo/glyphs.support/A_.glif
--rw-r--r--  2.0 unx     2474 b- defN 23-Jul-31 17:57 fontmake-3.7.0b3/tests/data/MutatorSansLite/MutatorSansLightCondensed.ufo/glyphs.support/S_.glif
--rw-r--r--  2.0 unx      353 b- defN 23-Jul-31 17:57 fontmake-3.7.0b3/tests/data/MutatorSansLite/MutatorSansLightCondensed.ufo/glyphs.support/layerinfo.plist
--rw-r--r--  2.0 unx     2492 b- defN 23-Jul-31 17:57 fontmake-3.7.0b3/tests/data/MutatorSansLite/MutatorSansLightCondensed.ufo/glyphs.support.S_.middle/S_.closed.glif
--rw-r--r--  2.0 unx      246 b- defN 23-Jul-31 17:57 fontmake-3.7.0b3/tests/data/MutatorSansLite/MutatorSansLightCondensed.ufo/glyphs.support.S_.middle/contents.plist
--rw-r--r--  2.0 unx      240 b- defN 23-Jul-31 17:57 fontmake-3.7.0b3/tests/data/MutatorSansLite/MutatorSansLightCondensed.ufo/glyphs.support.S_.middle/layerinfo.plist
--rw-r--r--  2.0 unx     1827 b- defN 23-Jul-31 17:57 fontmake-3.7.0b3/tests/data/MutatorSansLite/MutatorSansLightCondensed.ufo/glyphs/S_.closed.glif
--rw-r--r--  2.0 unx      652 b- defN 23-Jul-31 17:57 fontmake-3.7.0b3/tests/data/MutatorSansLite/MutatorSansLightCondensed.ufo/glyphs/I_.narrow.glif
--rw-r--r--  2.0 unx      687 b- defN 23-Jul-31 17:57 fontmake-3.7.0b3/tests/data/MutatorSansLite/MutatorSansLightCondensed.ufo/glyphs/I_.glif
--rw-r--r--  2.0 unx     1028 b- defN 23-Jul-31 17:57 fontmake-3.7.0b3/tests/data/MutatorSansLite/MutatorSansLightCondensed.ufo/glyphs/I_J_.glif
--rw-r--r--  2.0 unx      473 b- defN 23-Jul-31 17:57 fontmake-3.7.0b3/tests/data/MutatorSansLite/MutatorSansLightCondensed.ufo/glyphs/contents.plist
--rw-r--r--  2.0 unx      874 b- defN 23-Jul-31 17:57 fontmake-3.7.0b3/tests/data/MutatorSansLite/MutatorSansLightCondensed.ufo/glyphs/A_.glif
--rw-r--r--  2.0 unx     2247 b- defN 23-Jul-31 17:57 fontmake-3.7.0b3/tests/data/MutatorSansLite/MutatorSansLightCondensed.ufo/glyphs/S_.glif
--rw-r--r--  2.0 unx      353 b- defN 23-Jul-31 17:57 fontmake-3.7.0b3/tests/data/MutatorSansLite/MutatorSansLightCondensed.ufo/glyphs/layerinfo.plist
--rw-r--r--  2.0 unx      238 b- defN 23-Jul-31 17:57 fontmake-3.7.0b3/tests/data/MutatorSansLite/MutatorSansLightCondensed.ufo/glyphs.support.crossbars/contents.plist
--rw-r--r--  2.0 unx      183 b- defN 23-Jul-31 17:57 fontmake-3.7.0b3/tests/data/MutatorSansLite/MutatorSansLightCondensed.ufo/glyphs.support.crossbars/layerinfo.plist
--rw-r--r--  2.0 unx     1176 b- defN 23-Jul-31 17:57 fontmake-3.7.0b3/tests/data/MutatorSansLite/MutatorSansLightCondensed.ufo/glyphs.support.crossbars/E_.glif
--rw-r--r--  2.0 unx     3060 b- defN 23-Jul-31 17:57 fontmake-3.7.0b3/tests/data/MutatorSansLite/MutatorSansLightCondensed.ufo/glyphs.support.S_.wide/S_.closed.glif
--rw-r--r--  2.0 unx      288 b- defN 23-Jul-31 17:57 fontmake-3.7.0b3/tests/data/MutatorSansLite/MutatorSansLightCondensed.ufo/glyphs.support.S_.wide/contents.plist
--rw-r--r--  2.0 unx     3051 b- defN 23-Jul-31 17:57 fontmake-3.7.0b3/tests/data/MutatorSansLite/MutatorSansLightCondensed.ufo/glyphs.support.S_.wide/S_.glif
--rw-r--r--  2.0 unx      241 b- defN 23-Jul-31 17:57 fontmake-3.7.0b3/tests/data/MutatorSansLite/MutatorSansLightCondensed.ufo/glyphs.support.S_.wide/layerinfo.plist
-726 files, 1215766 bytes uncompressed, 299906 bytes compressed:  75.3%
+Zip file size: 471463 bytes, number of entries: 726
+drwxr-xr-x  2.0 unx        0 b- stor 23-Aug-07 15:30 fontmake-3.7.1/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Aug-07 15:30 fontmake-3.7.1/.github/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Aug-07 15:30 fontmake-3.7.1/Lib/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Aug-07 15:30 fontmake-3.7.1/tests/
+-rw-r--r--  2.0 unx      227 b- defN 23-Aug-07 15:30 fontmake-3.7.1/.editorconfig
+-rw-r--r--  2.0 unx    11357 b- defN 23-Aug-07 15:30 fontmake-3.7.1/LICENSE
+-rw-r--r--  2.0 unx      806 b- defN 23-Aug-07 15:30 fontmake-3.7.1/tox.ini
+-rw-r--r--  2.0 unx      163 b- defN 23-Aug-07 15:30 fontmake-3.7.1/pyproject.toml
+-rw-r--r--  2.0 unx     1453 b- defN 23-Aug-07 15:30 fontmake-3.7.1/.gitignore
+-rw-r--r--  2.0 unx      226 b- defN 23-Aug-07 15:30 fontmake-3.7.1/setup.cfg
+-rwxr-xr-x  2.0 unx     1302 b- defN 23-Aug-07 15:30 fontmake-3.7.1/build_pyz.sh
+-rw-r--r--  2.0 unx     1450 b- defN 23-Aug-07 15:30 fontmake-3.7.1/CONTRIBUTING.md
+-rw-r--r--  2.0 unx      142 b- defN 23-Aug-07 15:30 fontmake-3.7.1/MANIFEST.in
+-rw-r--r--  2.0 unx      481 b- defN 23-Aug-07 15:30 fontmake-3.7.1/requirements.txt
+-rw-r--r--  2.0 unx      322 b- defN 23-Aug-07 15:30 fontmake-3.7.1/.gitattributes
+-rw-r--r--  2.0 unx     3917 b- defN 23-Aug-07 15:30 fontmake-3.7.1/setup.py
+-rw-r--r--  2.0 unx     3193 b- defN 23-Aug-07 15:30 fontmake-3.7.1/TROUBLESHOOTING.md
+-rw-r--r--  2.0 unx      191 b- defN 23-Aug-07 15:30 fontmake-3.7.1/test_requirements.txt
+-rw-r--r--  2.0 unx     6285 b- defN 23-Aug-07 15:30 fontmake-3.7.1/README.md
+-rw-r--r--  2.0 unx      168 b- defN 23-Aug-07 15:30 fontmake-3.7.1/.pyup.yml
+-rw-r--r--  2.0 unx     7347 b- defN 23-Aug-07 15:30 fontmake-3.7.1/PKG-INFO
+-rw-r--r--  2.0 unx      792 b- defN 23-Aug-07 15:30 fontmake-3.7.1/.coveragerc
+-rw-r--r--  2.0 unx    19601 b- defN 23-Aug-07 15:30 fontmake-3.7.1/USAGE.md
+-rw-r--r--  2.0 unx       77 b- defN 23-Aug-07 15:30 fontmake-3.7.1/.codecov.yml
+drwxr-xr-x  2.0 unx        0 b- stor 23-Aug-07 15:30 fontmake-3.7.1/.github/workflows/
+-rw-r--r--  2.0 unx     4287 b- defN 23-Aug-07 15:30 fontmake-3.7.1/.github/workflows/ci.yml
+drwxr-xr-x  2.0 unx        0 b- stor 23-Aug-07 15:30 fontmake-3.7.1/Lib/fontmake.egg-info/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Aug-07 15:30 fontmake-3.7.1/Lib/fontmake/
+-rw-r--r--  2.0 unx       52 b- defN 23-Aug-07 15:30 fontmake-3.7.1/Lib/fontmake.egg-info/entry_points.txt
+-rw-r--r--  2.0 unx        9 b- defN 23-Aug-07 15:30 fontmake-3.7.1/Lib/fontmake.egg-info/top_level.txt
+-rw-r--r--  2.0 unx    42266 b- defN 23-Aug-07 15:30 fontmake-3.7.1/Lib/fontmake.egg-info/SOURCES.txt
+-rw-r--r--  2.0 unx        1 b- defN 23-Aug-07 15:30 fontmake-3.7.1/Lib/fontmake.egg-info/dependency_links.txt
+-rw-r--r--  2.0 unx      768 b- defN 23-Aug-07 15:30 fontmake-3.7.1/Lib/fontmake.egg-info/requires.txt
+-rw-r--r--  2.0 unx     7347 b- defN 23-Aug-07 15:30 fontmake-3.7.1/Lib/fontmake.egg-info/PKG-INFO
+-rw-r--r--  2.0 unx    61014 b- defN 23-Aug-07 15:30 fontmake-3.7.1/Lib/fontmake/font_project.py
+-rw-r--r--  2.0 unx     3049 b- defN 23-Aug-07 15:30 fontmake-3.7.1/Lib/fontmake/compatibility.py
+-rw-r--r--  2.0 unx      160 b- defN 23-Aug-07 15:30 fontmake-3.7.1/Lib/fontmake/_version.py
+-rw-r--r--  2.0 unx    27227 b- defN 23-Aug-07 15:30 fontmake-3.7.1/Lib/fontmake/__main__.py
+-rw-r--r--  2.0 unx     3288 b- defN 23-Aug-07 15:30 fontmake-3.7.1/Lib/fontmake/ttfautohint.py
+-rw-r--r--  2.0 unx    32133 b- defN 23-Aug-07 15:30 fontmake-3.7.1/Lib/fontmake/instantiator.py
+-rw-r--r--  2.0 unx     1439 b- defN 23-Aug-07 15:30 fontmake-3.7.1/Lib/fontmake/errors.py
+-rw-r--r--  2.0 unx      108 b- defN 23-Aug-07 15:30 fontmake-3.7.1/Lib/fontmake/__init__.py
+drwxr-xr-x  2.0 unx        0 b- stor 23-Aug-07 15:30 fontmake-3.7.1/tests/data/
+-rw-r--r--  2.0 unx      133 b- defN 23-Aug-07 15:30 fontmake-3.7.1/tests/conftest.py
+-rw-r--r--  2.0 unx    25699 b- defN 23-Aug-07 15:30 fontmake-3.7.1/tests/test_instantiator.py
+-rw-r--r--  2.0 unx     1668 b- defN 23-Aug-07 15:30 fontmake-3.7.1/tests/test_compatibility.py
+-rw-r--r--  2.0 unx    37281 b- defN 23-Aug-07 15:30 fontmake-3.7.1/tests/test_main.py
+drwxr-xr-x  2.0 unx        0 b- stor 23-Aug-07 15:30 fontmake-3.7.1/tests/data/IncompatibleSans/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Aug-07 15:30 fontmake-3.7.1/tests/data/DesignspaceTestSharedFeatures/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Aug-07 15:30 fontmake-3.7.1/tests/data/InterpolateLayoutTest/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Aug-07 15:30 fontmake-3.7.1/tests/data/DesignspaceRuleOrder/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Aug-07 15:30 fontmake-3.7.1/tests/data/GlyphsUnitTestSans3.glyphspackage/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Aug-07 15:30 fontmake-3.7.1/tests/data/SwapGlyphNames/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Aug-07 15:30 fontmake-3.7.1/tests/data/DesignspaceBrokenTest/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Aug-07 15:30 fontmake-3.7.1/tests/data/DesignspaceTest/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Aug-07 15:30 fontmake-3.7.1/tests/data/MutatorSansLite/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Aug-07 15:30 fontmake-3.7.1/tests/data/InstantiatorStrictMathGlyph/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Aug-07 15:30 fontmake-3.7.1/tests/data/MutatorSans/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Aug-07 15:30 fontmake-3.7.1/tests/data/AutohintingTest/
+-rw-r--r--  2.0 unx     6386 b- defN 23-Aug-07 15:30 fontmake-3.7.1/tests/data/TestSubset.glyphs
+-rw-r--r--  2.0 unx     6381 b- defN 23-Aug-07 15:30 fontmake-3.7.1/tests/data/TestSubset2.glyphs
+-rw-r--r--  2.0 unx    31198 b- defN 23-Aug-07 15:30 fontmake-3.7.1/tests/data/GlyphsUnitTestSans.glyphs
+-rw-r--r--  2.0 unx      150 b- defN 23-Aug-07 15:30 fontmake-3.7.1/tests/data/GlyphData.xml
+drwxr-xr-x  2.0 unx        0 b- stor 23-Aug-07 15:30 fontmake-3.7.1/tests/data/IncompatibleSans/IncompatibleSans-Regular.ufo/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Aug-07 15:30 fontmake-3.7.1/tests/data/IncompatibleSans/IncompatibleSans-Bold.ufo/
+-rw-r--r--  2.0 unx      762 b- defN 23-Aug-07 15:30 fontmake-3.7.1/tests/data/IncompatibleSans/IncompatibleSans.designspace
+drwxr-xr-x  2.0 unx        0 b- stor 23-Aug-07 15:30 fontmake-3.7.1/tests/data/IncompatibleSans/IncompatibleSans-Regular.ufo/glyphs/
+-rw-r--r--  2.0 unx      318 b- defN 23-Aug-07 15:30 fontmake-3.7.1/tests/data/IncompatibleSans/IncompatibleSans-Regular.ufo/metainfo.plist
+-rw-r--r--  2.0 unx     1160 b- defN 23-Aug-07 15:30 fontmake-3.7.1/tests/data/IncompatibleSans/IncompatibleSans-Regular.ufo/fontinfo.plist
+-rw-r--r--  2.0 unx      287 b- defN 23-Aug-07 15:30 fontmake-3.7.1/tests/data/IncompatibleSans/IncompatibleSans-Regular.ufo/layercontents.plist
+-rw-r--r--  2.0 unx     2107 b- defN 23-Aug-07 15:30 fontmake-3.7.1/tests/data/IncompatibleSans/IncompatibleSans-Regular.ufo/lib.plist
+-rw-r--r--  2.0 unx      217 b- defN 23-Aug-07 15:30 fontmake-3.7.1/tests/data/IncompatibleSans/IncompatibleSans-Regular.ufo/glyphs/C_.glif
+-rw-r--r--  2.0 unx      652 b- defN 23-Aug-07 15:30 fontmake-3.7.1/tests/data/IncompatibleSans/IncompatibleSans-Regular.ufo/glyphs/B_.glif
+-rw-r--r--  2.0 unx      154 b- defN 23-Aug-07 15:30 fontmake-3.7.1/tests/data/IncompatibleSans/IncompatibleSans-Regular.ufo/glyphs/space.glif
+-rw-r--r--  2.0 unx      429 b- defN 23-Aug-07 15:30 fontmake-3.7.1/tests/data/IncompatibleSans/IncompatibleSans-Regular.ufo/glyphs/contents.plist
+-rw-r--r--  2.0 unx      652 b- defN 23-Aug-07 15:30 fontmake-3.7.1/tests/data/IncompatibleSans/IncompatibleSans-Regular.ufo/glyphs/D_.glif
+-rw-r--r--  2.0 unx      893 b- defN 23-Aug-07 15:30 fontmake-3.7.1/tests/data/IncompatibleSans/IncompatibleSans-Regular.ufo/glyphs/A_.glif
+drwxr-xr-x  2.0 unx        0 b- stor 23-Aug-07 15:30 fontmake-3.7.1/tests/data/IncompatibleSans/IncompatibleSans-Bold.ufo/glyphs/
+-rw-r--r--  2.0 unx      318 b- defN 23-Aug-07 15:30 fontmake-3.7.1/tests/data/IncompatibleSans/IncompatibleSans-Bold.ufo/metainfo.plist
+-rw-r--r--  2.0 unx     1158 b- defN 23-Aug-07 15:30 fontmake-3.7.1/tests/data/IncompatibleSans/IncompatibleSans-Bold.ufo/fontinfo.plist
+-rw-r--r--  2.0 unx      287 b- defN 23-Aug-07 15:30 fontmake-3.7.1/tests/data/IncompatibleSans/IncompatibleSans-Bold.ufo/layercontents.plist
+-rw-r--r--  2.0 unx     2113 b- defN 23-Aug-07 15:30 fontmake-3.7.1/tests/data/IncompatibleSans/IncompatibleSans-Bold.ufo/lib.plist
+-rw-r--r--  2.0 unx      101 b- defN 23-Aug-07 15:30 fontmake-3.7.1/tests/data/IncompatibleSans/IncompatibleSans-Bold.ufo/features.fea
+-rw-r--r--  2.0 unx      215 b- defN 23-Aug-07 15:30 fontmake-3.7.1/tests/data/IncompatibleSans/IncompatibleSans-Bold.ufo/glyphs/C_.glif
+-rw-r--r--  2.0 unx      560 b- defN 23-Aug-07 15:30 fontmake-3.7.1/tests/data/IncompatibleSans/IncompatibleSans-Bold.ufo/glyphs/B_.glif
+-rw-r--r--  2.0 unx      154 b- defN 23-Aug-07 15:30 fontmake-3.7.1/tests/data/IncompatibleSans/IncompatibleSans-Bold.ufo/glyphs/space.glif
+-rw-r--r--  2.0 unx      429 b- defN 23-Aug-07 15:30 fontmake-3.7.1/tests/data/IncompatibleSans/IncompatibleSans-Bold.ufo/glyphs/contents.plist
+-rw-r--r--  2.0 unx      694 b- defN 23-Aug-07 15:30 fontmake-3.7.1/tests/data/IncompatibleSans/IncompatibleSans-Bold.ufo/glyphs/D_.glif
+-rw-r--r--  2.0 unx     1196 b- defN 23-Aug-07 15:30 fontmake-3.7.1/tests/data/IncompatibleSans/IncompatibleSans-Bold.ufo/glyphs/A_.glif
+drwxr-xr-x  2.0 unx        0 b- stor 23-Aug-07 15:30 fontmake-3.7.1/tests/data/DesignspaceTestSharedFeatures/DesignspaceTest-Light.ufo/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Aug-07 15:30 fontmake-3.7.1/tests/data/DesignspaceTestSharedFeatures/DesignspaceTest-Regular.ufo/
+-rw-r--r--  2.0 unx     1059 b- defN 23-Aug-07 15:30 fontmake-3.7.1/tests/data/DesignspaceTestSharedFeatures/DesignspaceTestSharedFeatures.designspace
+-rw-r--r--  2.0 unx        7 b- defN 23-Aug-07 15:30 fontmake-3.7.1/tests/data/DesignspaceTestSharedFeatures/family.fea
+drwxr-xr-x  2.0 unx        0 b- stor 23-Aug-07 15:30 fontmake-3.7.1/tests/data/DesignspaceTestSharedFeatures/DesignspaceTest-Light.ufo/glyphs/
+-rw-r--r--  2.0 unx      318 b- defN 23-Aug-07 15:30 fontmake-3.7.1/tests/data/DesignspaceTestSharedFeatures/DesignspaceTest-Light.ufo/metainfo.plist
+-rw-r--r--  2.0 unx      897 b- defN 23-Aug-07 15:30 fontmake-3.7.1/tests/data/DesignspaceTestSharedFeatures/DesignspaceTest-Light.ufo/fontinfo.plist
+-rw-r--r--  2.0 unx      287 b- defN 23-Aug-07 15:30 fontmake-3.7.1/tests/data/DesignspaceTestSharedFeatures/DesignspaceTest-Light.ufo/layercontents.plist
+-rw-r--r--  2.0 unx      183 b- defN 23-Aug-07 15:30 fontmake-3.7.1/tests/data/DesignspaceTestSharedFeatures/DesignspaceTest-Light.ufo/glyphs/contents.plist
+drwxr-xr-x  2.0 unx        0 b- stor 23-Aug-07 15:30 fontmake-3.7.1/tests/data/DesignspaceTestSharedFeatures/DesignspaceTest-Regular.ufo/glyphs/
+-rw-r--r--  2.0 unx      318 b- defN 23-Aug-07 15:30 fontmake-3.7.1/tests/data/DesignspaceTestSharedFeatures/DesignspaceTest-Regular.ufo/metainfo.plist
+-rw-r--r--  2.0 unx      899 b- defN 23-Aug-07 15:30 fontmake-3.7.1/tests/data/DesignspaceTestSharedFeatures/DesignspaceTest-Regular.ufo/fontinfo.plist
+-rw-r--r--  2.0 unx      287 b- defN 23-Aug-07 15:30 fontmake-3.7.1/tests/data/DesignspaceTestSharedFeatures/DesignspaceTest-Regular.ufo/layercontents.plist
+-rw-r--r--  2.0 unx       20 b- defN 23-Aug-07 15:30 fontmake-3.7.1/tests/data/DesignspaceTestSharedFeatures/DesignspaceTest-Regular.ufo/features.fea
+-rw-r--r--  2.0 unx      183 b- defN 23-Aug-07 15:30 fontmake-3.7.1/tests/data/DesignspaceTestSharedFeatures/DesignspaceTest-Regular.ufo/glyphs/contents.plist
+-rw-r--r--  2.0 unx      249 b- defN 23-Aug-07 15:30 fontmake-3.7.1/tests/data/InterpolateLayoutTest/InterpolateLayoutTest 1000 GPOS.txt
+-rw-r--r--  2.0 unx       92 b- defN 23-Aug-07 15:30 fontmake-3.7.1/tests/data/InterpolateLayoutTest/InterpolateLayoutTest GSUB.txt
+-rw-r--r--  2.0 unx       73 b- defN 23-Aug-07 15:30 fontmake-3.7.1/tests/data/InterpolateLayoutTest/InterpolateLayoutTest GDEF.txt
+-rw-r--r--  2.0 unx     6904 b- defN 23-Aug-07 15:30 fontmake-3.7.1/tests/data/InterpolateLayoutTest/InterpolateLayoutTest.glyphs
+-rw-r--r--  2.0 unx      246 b- defN 23-Aug-07 15:30 fontmake-3.7.1/tests/data/InterpolateLayoutTest/InterpolateLayoutTest 0 GPOS.txt
+-rw-r--r--  2.0 unx      716 b- defN 23-Aug-07 15:30 fontmake-3.7.1/tests/data/InterpolateLayoutTest/InterpolateLayoutTest.plist
+drwxr-xr-x  2.0 unx        0 b- stor 23-Aug-07 15:30 fontmake-3.7.1/tests/data/DesignspaceRuleOrder/MyFont_Black.ufo/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Aug-07 15:30 fontmake-3.7.1/tests/data/DesignspaceRuleOrder/MyFont_Hair.ufo/
+-rw-r--r--  2.0 unx     2035 b- defN 23-Aug-07 15:30 fontmake-3.7.1/tests/data/DesignspaceRuleOrder/MyFont.designspace
+drwxr-xr-x  2.0 unx        0 b- stor 23-Aug-07 15:30 fontmake-3.7.1/tests/data/DesignspaceRuleOrder/MyFont_Black.ufo/glyphs/
+-rw-r--r--  2.0 unx      308 b- defN 23-Aug-07 15:30 fontmake-3.7.1/tests/data/DesignspaceRuleOrder/MyFont_Black.ufo/metainfo.plist
+-rw-r--r--  2.0 unx      887 b- defN 23-Aug-07 15:30 fontmake-3.7.1/tests/data/DesignspaceRuleOrder/MyFont_Black.ufo/fontinfo.plist
+-rw-r--r--  2.0 unx      275 b- defN 23-Aug-07 15:30 fontmake-3.7.1/tests/data/DesignspaceRuleOrder/MyFont_Black.ufo/layercontents.plist
+-rw-r--r--  2.0 unx      360 b- defN 23-Aug-07 15:30 fontmake-3.7.1/tests/data/DesignspaceRuleOrder/MyFont_Black.ufo/lib.plist
+-rw-r--r--  2.0 unx     1265 b- defN 23-Aug-07 15:30 fontmake-3.7.1/tests/data/DesignspaceRuleOrder/MyFont_Black.ufo/glyphs/Q_.ss01.alt.glif
+-rw-r--r--  2.0 unx      412 b- defN 23-Aug-07 15:30 fontmake-3.7.1/tests/data/DesignspaceRuleOrder/MyFont_Black.ufo/glyphs/contents.plist
+-rw-r--r--  2.0 unx     1659 b- defN 23-Aug-07 15:30 fontmake-3.7.1/tests/data/DesignspaceRuleOrder/MyFont_Black.ufo/glyphs/Q_.glif
+-rw-r--r--  2.0 unx     1455 b- defN 23-Aug-07 15:30 fontmake-3.7.1/tests/data/DesignspaceRuleOrder/MyFont_Black.ufo/glyphs/Q_.alt.glif
+-rw-r--r--  2.0 unx     1261 b- defN 23-Aug-07 15:30 fontmake-3.7.1/tests/data/DesignspaceRuleOrder/MyFont_Black.ufo/glyphs/Q_.ss01.glif
+drwxr-xr-x  2.0 unx        0 b- stor 23-Aug-07 15:30 fontmake-3.7.1/tests/data/DesignspaceRuleOrder/MyFont_Hair.ufo/glyphs/
+-rw-r--r--  2.0 unx      308 b- defN 23-Aug-07 15:30 fontmake-3.7.1/tests/data/DesignspaceRuleOrder/MyFont_Hair.ufo/metainfo.plist
+-rw-r--r--  2.0 unx      890 b- defN 23-Aug-07 15:30 fontmake-3.7.1/tests/data/DesignspaceRuleOrder/MyFont_Hair.ufo/fontinfo.plist
+-rw-r--r--  2.0 unx      275 b- defN 23-Aug-07 15:30 fontmake-3.7.1/tests/data/DesignspaceRuleOrder/MyFont_Hair.ufo/layercontents.plist
+-rw-r--r--  2.0 unx      360 b- defN 23-Aug-07 15:30 fontmake-3.7.1/tests/data/DesignspaceRuleOrder/MyFont_Hair.ufo/lib.plist
+-rw-r--r--  2.0 unx     1263 b- defN 23-Aug-07 15:30 fontmake-3.7.1/tests/data/DesignspaceRuleOrder/MyFont_Hair.ufo/glyphs/Q_.ss01.alt.glif
+-rw-r--r--  2.0 unx      412 b- defN 23-Aug-07 15:30 fontmake-3.7.1/tests/data/DesignspaceRuleOrder/MyFont_Hair.ufo/glyphs/contents.plist
+-rw-r--r--  2.0 unx     1642 b- defN 23-Aug-07 15:30 fontmake-3.7.1/tests/data/DesignspaceRuleOrder/MyFont_Hair.ufo/glyphs/Q_.glif
+-rw-r--r--  2.0 unx     1439 b- defN 23-Aug-07 15:30 fontmake-3.7.1/tests/data/DesignspaceRuleOrder/MyFont_Hair.ufo/glyphs/Q_.alt.glif
+-rw-r--r--  2.0 unx     1263 b- defN 23-Aug-07 15:30 fontmake-3.7.1/tests/data/DesignspaceRuleOrder/MyFont_Hair.ufo/glyphs/Q_.ss01.glif
+drwxr-xr-x  2.0 unx        0 b- stor 23-Aug-07 15:30 fontmake-3.7.1/tests/data/GlyphsUnitTestSans3.glyphspackage/glyphs/
+-rw-r--r--  2.0 unx       83 b- defN 23-Aug-07 15:30 fontmake-3.7.1/tests/data/GlyphsUnitTestSans3.glyphspackage/order.plist
+-rw-r--r--  2.0 unx    22772 b- defN 23-Aug-07 15:30 fontmake-3.7.1/tests/data/GlyphsUnitTestSans3.glyphspackage/fontinfo.plist
+-rw-r--r--  2.0 unx      764 b- defN 23-Aug-07 15:30 fontmake-3.7.1/tests/data/GlyphsUnitTestSans3.glyphspackage/glyphs/h.glyph
+-rw-r--r--  2.0 unx     1308 b- defN 23-Aug-07 15:30 fontmake-3.7.1/tests/data/GlyphsUnitTestSans3.glyphspackage/glyphs/a.sc.glyph
+-rw-r--r--  2.0 unx      454 b- defN 23-Aug-07 15:30 fontmake-3.7.1/tests/data/GlyphsUnitTestSans3.glyphspackage/glyphs/A_dieresis.glyph
+-rw-r--r--  2.0 unx      445 b- defN 23-Aug-07 15:30 fontmake-3.7.1/tests/data/GlyphsUnitTestSans3.glyphspackage/glyphs/adieresis.glyph
+-rw-r--r--  2.0 unx     1026 b- defN 23-Aug-07 15:30 fontmake-3.7.1/tests/data/GlyphsUnitTestSans3.glyphspackage/glyphs/dieresis.glyph
+-rw-r--r--  2.0 unx     2295 b- defN 23-Aug-07 15:30 fontmake-3.7.1/tests/data/GlyphsUnitTestSans3.glyphspackage/glyphs/_part.stem.glyph
+-rw-r--r--  2.0 unx     1580 b- defN 23-Aug-07 15:30 fontmake-3.7.1/tests/data/GlyphsUnitTestSans3.glyphspackage/glyphs/n.glyph
+-rw-r--r--  2.0 unx      902 b- defN 23-Aug-07 15:30 fontmake-3.7.1/tests/data/GlyphsUnitTestSans3.glyphspackage/glyphs/m.glyph
+-rw-r--r--  2.0 unx     5010 b- defN 23-Aug-07 15:30 fontmake-3.7.1/tests/data/GlyphsUnitTestSans3.glyphspackage/glyphs/_part.shoulder.glyph
+-rw-r--r--  2.0 unx     1889 b- defN 23-Aug-07 15:30 fontmake-3.7.1/tests/data/GlyphsUnitTestSans3.glyphspackage/glyphs/A_.glyph
+-rw-r--r--  2.0 unx     6165 b- defN 23-Aug-07 15:30 fontmake-3.7.1/tests/data/GlyphsUnitTestSans3.glyphspackage/glyphs/a.glyph
+drwxr-xr-x  2.0 unx        0 b- stor 23-Aug-07 15:30 fontmake-3.7.1/tests/data/SwapGlyphNames/B.ufo/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Aug-07 15:30 fontmake-3.7.1/tests/data/SwapGlyphNames/A.ufo/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Aug-07 15:30 fontmake-3.7.1/tests/data/SwapGlyphNames/B.ufo/glyphs/
+-rw-r--r--  2.0 unx      318 b- defN 23-Aug-07 15:30 fontmake-3.7.1/tests/data/SwapGlyphNames/B.ufo/metainfo.plist
+-rw-r--r--  2.0 unx      790 b- defN 23-Aug-07 15:30 fontmake-3.7.1/tests/data/SwapGlyphNames/B.ufo/fontinfo.plist
+-rw-r--r--  2.0 unx      287 b- defN 23-Aug-07 15:30 fontmake-3.7.1/tests/data/SwapGlyphNames/B.ufo/layercontents.plist
+-rw-r--r--  2.0 unx      410 b- defN 23-Aug-07 15:30 fontmake-3.7.1/tests/data/SwapGlyphNames/B.ufo/lib.plist
+-rw-r--r--  2.0 unx      539 b- defN 23-Aug-07 15:30 fontmake-3.7.1/tests/data/SwapGlyphNames/B.ufo/glyphs/dieresiscomb.glif
+-rw-r--r--  2.0 unx      784 b- defN 23-Aug-07 15:30 fontmake-3.7.1/tests/data/SwapGlyphNames/B.ufo/glyphs/a.alt.glif
+-rw-r--r--  2.0 unx      221 b- defN 23-Aug-07 15:30 fontmake-3.7.1/tests/data/SwapGlyphNames/B.ufo/glyphs/adieresis.glif
+-rw-r--r--  2.0 unx      487 b- defN 23-Aug-07 15:30 fontmake-3.7.1/tests/data/SwapGlyphNames/B.ufo/glyphs/contents.plist
+-rw-r--r--  2.0 unx      205 b- defN 23-Aug-07 15:30 fontmake-3.7.1/tests/data/SwapGlyphNames/B.ufo/glyphs/adieresis.alt.glif
+-rw-r--r--  2.0 unx      898 b- defN 23-Aug-07 15:30 fontmake-3.7.1/tests/data/SwapGlyphNames/B.ufo/glyphs/a.glif
+drwxr-xr-x  2.0 unx        0 b- stor 23-Aug-07 15:30 fontmake-3.7.1/tests/data/SwapGlyphNames/A.ufo/glyphs/
+-rw-r--r--  2.0 unx      318 b- defN 23-Aug-07 15:30 fontmake-3.7.1/tests/data/SwapGlyphNames/A.ufo/metainfo.plist
+-rw-r--r--  2.0 unx      714 b- defN 23-Aug-07 15:30 fontmake-3.7.1/tests/data/SwapGlyphNames/A.ufo/kerning.plist
+-rw-r--r--  2.0 unx      471 b- defN 23-Aug-07 15:30 fontmake-3.7.1/tests/data/SwapGlyphNames/A.ufo/groups.plist
+-rw-r--r--  2.0 unx      790 b- defN 23-Aug-07 15:30 fontmake-3.7.1/tests/data/SwapGlyphNames/A.ufo/fontinfo.plist
+-rw-r--r--  2.0 unx      287 b- defN 23-Aug-07 15:30 fontmake-3.7.1/tests/data/SwapGlyphNames/A.ufo/layercontents.plist
+-rw-r--r--  2.0 unx      443 b- defN 23-Aug-07 15:30 fontmake-3.7.1/tests/data/SwapGlyphNames/A.ufo/lib.plist
+-rw-r--r--  2.0 unx      382 b- defN 23-Aug-07 15:30 fontmake-3.7.1/tests/data/SwapGlyphNames/A.ufo/glyphs/aaa.glif
+-rw-r--r--  2.0 unx      646 b- defN 23-Aug-07 15:30 fontmake-3.7.1/tests/data/SwapGlyphNames/A.ufo/glyphs/x.glif
+-rw-r--r--  2.0 unx      156 b- defN 23-Aug-07 15:30 fontmake-3.7.1/tests/data/SwapGlyphNames/A.ufo/glyphs/space.glif
+-rw-r--r--  2.0 unx      393 b- defN 23-Aug-07 15:30 fontmake-3.7.1/tests/data/SwapGlyphNames/A.ufo/glyphs/aaa.swap.glif
+-rw-r--r--  2.0 unx      543 b- defN 23-Aug-07 15:30 fontmake-3.7.1/tests/data/SwapGlyphNames/A.ufo/glyphs/contents.plist
+-rw-r--r--  2.0 unx      522 b- defN 23-Aug-07 15:30 fontmake-3.7.1/tests/data/SwapGlyphNames/A.ufo/glyphs/y.glif
+-rw-r--r--  2.0 unx      436 b- defN 23-Aug-07 15:30 fontmake-3.7.1/tests/data/SwapGlyphNames/A.ufo/glyphs/a.glif
+-rw-r--r--  2.0 unx      581 b- defN 23-Aug-07 15:30 fontmake-3.7.1/tests/data/SwapGlyphNames/A.ufo/glyphs/a.swap.glif
+drwxr-xr-x  2.0 unx        0 b- stor 23-Aug-07 15:30 fontmake-3.7.1/tests/data/DesignspaceBrokenTest/MyFont-Light.ufo/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Aug-07 15:30 fontmake-3.7.1/tests/data/DesignspaceBrokenTest/MyFont-Bold.ufo/
+-rw-r--r--  2.0 unx     1135 b- defN 23-Aug-07 15:30 fontmake-3.7.1/tests/data/DesignspaceBrokenTest/Designspace-MastersAsInstances.designspace
+-rw-r--r--  2.0 unx      983 b- defN 23-Aug-07 15:30 fontmake-3.7.1/tests/data/DesignspaceBrokenTest/DesignspaceTest.designspace
+drwxr-xr-x  2.0 unx        0 b- stor 23-Aug-07 15:30 fontmake-3.7.1/tests/data/DesignspaceBrokenTest/MyFont-Light.ufo/glyphs/
+-rw-r--r--  2.0 unx      318 b- defN 23-Aug-07 15:30 fontmake-3.7.1/tests/data/DesignspaceBrokenTest/MyFont-Light.ufo/metainfo.plist
+-rw-r--r--  2.0 unx      887 b- defN 23-Aug-07 15:30 fontmake-3.7.1/tests/data/DesignspaceBrokenTest/MyFont-Light.ufo/fontinfo.plist
+-rw-r--r--  2.0 unx      287 b- defN 23-Aug-07 15:30 fontmake-3.7.1/tests/data/DesignspaceBrokenTest/MyFont-Light.ufo/layercontents.plist
+-rw-r--r--  2.0 unx      303 b- defN 23-Aug-07 15:30 fontmake-3.7.1/tests/data/DesignspaceBrokenTest/MyFont-Light.ufo/lib.plist
+-rw-r--r--  2.0 unx      343 b- defN 23-Aug-07 15:30 fontmake-3.7.1/tests/data/DesignspaceBrokenTest/MyFont-Light.ufo/glyphs/l.glif
+-rw-r--r--  2.0 unx      479 b- defN 23-Aug-07 15:30 fontmake-3.7.1/tests/data/DesignspaceBrokenTest/MyFont-Light.ufo/glyphs/asas.glif
+-rw-r--r--  2.0 unx      288 b- defN 23-Aug-07 15:30 fontmake-3.7.1/tests/data/DesignspaceBrokenTest/MyFont-Light.ufo/glyphs/contents.plist
+drwxr-xr-x  2.0 unx        0 b- stor 23-Aug-07 15:30 fontmake-3.7.1/tests/data/DesignspaceBrokenTest/MyFont-Bold.ufo/glyphs/
+-rw-r--r--  2.0 unx      318 b- defN 23-Aug-07 15:30 fontmake-3.7.1/tests/data/DesignspaceBrokenTest/MyFont-Bold.ufo/metainfo.plist
+-rw-r--r--  2.0 unx      886 b- defN 23-Aug-07 15:30 fontmake-3.7.1/tests/data/DesignspaceBrokenTest/MyFont-Bold.ufo/fontinfo.plist
+-rw-r--r--  2.0 unx      287 b- defN 23-Aug-07 15:30 fontmake-3.7.1/tests/data/DesignspaceBrokenTest/MyFont-Bold.ufo/layercontents.plist
+-rw-r--r--  2.0 unx      303 b- defN 23-Aug-07 15:30 fontmake-3.7.1/tests/data/DesignspaceBrokenTest/MyFont-Bold.ufo/lib.plist
+-rw-r--r--  2.0 unx      345 b- defN 23-Aug-07 15:30 fontmake-3.7.1/tests/data/DesignspaceBrokenTest/MyFont-Bold.ufo/glyphs/l.glif
+-rw-r--r--  2.0 unx      425 b- defN 23-Aug-07 15:30 fontmake-3.7.1/tests/data/DesignspaceBrokenTest/MyFont-Bold.ufo/glyphs/asas.glif
+-rw-r--r--  2.0 unx      288 b- defN 23-Aug-07 15:30 fontmake-3.7.1/tests/data/DesignspaceBrokenTest/MyFont-Bold.ufo/glyphs/contents.plist
+drwxr-xr-x  2.0 unx        0 b- stor 23-Aug-07 15:30 fontmake-3.7.1/tests/data/DesignspaceTest/MyFont-Light.ufo/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Aug-07 15:30 fontmake-3.7.1/tests/data/DesignspaceTest/MyFont-Bold.ufo/
+-rw-r--r--  2.0 unx     1340 b- defN 23-Aug-07 15:30 fontmake-3.7.1/tests/data/DesignspaceTest/DesignspaceTest-lib.designspace
+-rw-r--r--  2.0 unx      916 b- defN 23-Aug-07 15:30 fontmake-3.7.1/tests/data/DesignspaceTest/DesignspaceTest-wght-wdth.designspace
+-rw-r--r--  2.0 unx     3057 b- defN 23-Aug-07 15:30 fontmake-3.7.1/tests/data/DesignspaceTest/MyFont-Light.ufoz
+-rw-r--r--  2.0 unx      621 b- defN 23-Aug-07 15:30 fontmake-3.7.1/tests/data/DesignspaceTest/DesignspaceTest-opsz.designspace
+-rw-r--r--  2.0 unx     2253 b- defN 23-Aug-07 15:30 fontmake-3.7.1/tests/data/DesignspaceTest/MyFont-Bold.ufoz
+-rw-r--r--  2.0 unx      745 b- defN 23-Aug-07 15:30 fontmake-3.7.1/tests/data/DesignspaceTest/DesignspaceTest-bare.designspace
+-rw-r--r--  2.0 unx      852 b- defN 23-Aug-07 15:30 fontmake-3.7.1/tests/data/DesignspaceTest/DesignspaceTest-instance-attrs.designspace
+-rw-r--r--  2.0 unx      614 b- defN 23-Aug-07 15:30 fontmake-3.7.1/tests/data/DesignspaceTest/DesignspaceTest-slnt.designspace
+-rw-r--r--  2.0 unx      983 b- defN 23-Aug-07 15:30 fontmake-3.7.1/tests/data/DesignspaceTest/DesignspaceTest.designspace
+drwxr-xr-x  2.0 unx        0 b- stor 23-Aug-07 15:30 fontmake-3.7.1/tests/data/DesignspaceTest/MyFont-Light.ufo/glyphs/
+-rw-r--r--  2.0 unx      318 b- defN 23-Aug-07 15:30 fontmake-3.7.1/tests/data/DesignspaceTest/MyFont-Light.ufo/metainfo.plist
+-rw-r--r--  2.0 unx      357 b- defN 23-Aug-07 15:30 fontmake-3.7.1/tests/data/DesignspaceTest/MyFont-Light.ufo/groups.plist
+-rw-r--r--  2.0 unx      878 b- defN 23-Aug-07 15:30 fontmake-3.7.1/tests/data/DesignspaceTest/MyFont-Light.ufo/fontinfo.plist
+-rw-r--r--  2.0 unx      287 b- defN 23-Aug-07 15:30 fontmake-3.7.1/tests/data/DesignspaceTest/MyFont-Light.ufo/layercontents.plist
+-rw-r--r--  2.0 unx      240 b- defN 23-Aug-07 15:30 fontmake-3.7.1/tests/data/DesignspaceTest/MyFont-Light.ufo/lib.plist
+-rw-r--r--  2.0 unx      343 b- defN 23-Aug-07 15:30 fontmake-3.7.1/tests/data/DesignspaceTest/MyFont-Light.ufo/glyphs/l.glif
+-rw-r--r--  2.0 unx      237 b- defN 23-Aug-07 15:30 fontmake-3.7.1/tests/data/DesignspaceTest/MyFont-Light.ufo/glyphs/contents.plist
+drwxr-xr-x  2.0 unx        0 b- stor 23-Aug-07 15:30 fontmake-3.7.1/tests/data/DesignspaceTest/MyFont-Bold.ufo/glyphs/
+-rw-r--r--  2.0 unx      318 b- defN 23-Aug-07 15:30 fontmake-3.7.1/tests/data/DesignspaceTest/MyFont-Bold.ufo/metainfo.plist
+-rw-r--r--  2.0 unx      548 b- defN 23-Aug-07 15:30 fontmake-3.7.1/tests/data/DesignspaceTest/MyFont-Bold.ufo/fontinfo.plist
+-rw-r--r--  2.0 unx      287 b- defN 23-Aug-07 15:30 fontmake-3.7.1/tests/data/DesignspaceTest/MyFont-Bold.ufo/layercontents.plist
+-rw-r--r--  2.0 unx      345 b- defN 23-Aug-07 15:30 fontmake-3.7.1/tests/data/DesignspaceTest/MyFont-Bold.ufo/glyphs/l.glif
+-rw-r--r--  2.0 unx      237 b- defN 23-Aug-07 15:30 fontmake-3.7.1/tests/data/DesignspaceTest/MyFont-Bold.ufo/glyphs/contents.plist
+drwxr-xr-x  2.0 unx        0 b- stor 23-Aug-07 15:30 fontmake-3.7.1/tests/data/MutatorSansLite/MutatorSansLightWide.ufo/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Aug-07 15:30 fontmake-3.7.1/tests/data/MutatorSansLite/MutatorSansBoldWide.ufo/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Aug-07 15:30 fontmake-3.7.1/tests/data/MutatorSansLite/MutatorSansBoldCondensed.ufo/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Aug-07 15:30 fontmake-3.7.1/tests/data/MutatorSansLite/MutatorSerifLightWide.ufo/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Aug-07 15:30 fontmake-3.7.1/tests/data/MutatorSansLite/MutatorSansLightCondensed.ufo/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Aug-07 15:30 fontmake-3.7.1/tests/data/MutatorSansLite/MutatorSerifLightCondensed.ufo/
+-rw-r--r--  2.0 unx     1074 b- defN 23-Aug-07 15:30 fontmake-3.7.1/tests/data/MutatorSansLite/LICENSE
+-rw-r--r--  2.0 unx     5741 b- defN 23-Aug-07 15:30 fontmake-3.7.1/tests/data/MutatorSansLite/MutatorSans_v5_several_vfs.designspace
+-rw-r--r--  2.0 unx     5197 b- defN 23-Aug-07 15:30 fontmake-3.7.1/tests/data/MutatorSansLite/MutatorSans_v5_implicit_one_vf.designspace
+-rw-r--r--  2.0 unx     7158 b- defN 23-Aug-07 15:30 fontmake-3.7.1/tests/data/MutatorSansLite/MutatorFamily_v5_discrete_axis.designspace
+-rw-r--r--  2.0 unx     5180 b- defN 23-Aug-07 15:30 fontmake-3.7.1/tests/data/MutatorSansLite/MutatorSans_v5_several_vfs_discrete_axis.designspace
+drwxr-xr-x  2.0 unx        0 b- stor 23-Aug-07 15:30 fontmake-3.7.1/tests/data/MutatorSansLite/MutatorSansLightWide.ufo/glyphs.master_width_720.00_weight_645.00/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Aug-07 15:30 fontmake-3.7.1/tests/data/MutatorSansLite/MutatorSansLightWide.ufo/glyphs.background/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Aug-07 15:30 fontmake-3.7.1/tests/data/MutatorSansLite/MutatorSansLightWide.ufo/glyphs/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Aug-07 15:30 fontmake-3.7.1/tests/data/MutatorSansLite/MutatorSansLightWide.ufo/glyphs.master_width_695.65_weight_166.38/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Aug-07 15:30 fontmake-3.7.1/tests/data/MutatorSansLite/MutatorSansLightWide.ufo/glyphs.master_width_0.00_weight_0.00/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Aug-07 15:30 fontmake-3.7.1/tests/data/MutatorSansLite/MutatorSansLightWide.ufo/glyphs.master_width_500.00_weight_500.00/
+-rw-r--r--  2.0 unx      308 b- defN 23-Aug-07 15:30 fontmake-3.7.1/tests/data/MutatorSansLite/MutatorSansLightWide.ufo/metainfo.plist
+-rw-r--r--  2.0 unx     1829 b- defN 23-Aug-07 15:30 fontmake-3.7.1/tests/data/MutatorSansLite/MutatorSansLightWide.ufo/fontinfo.plist
+-rw-r--r--  2.0 unx      361 b- defN 23-Aug-07 15:30 fontmake-3.7.1/tests/data/MutatorSansLite/MutatorSansLightWide.ufo/layercontents.plist
+-rw-r--r--  2.0 unx    16116 b- defN 23-Aug-07 15:30 fontmake-3.7.1/tests/data/MutatorSansLite/MutatorSansLightWide.ufo/lib.plist
+-rw-r--r--  2.0 unx       37 b- defN 23-Aug-07 15:30 fontmake-3.7.1/tests/data/MutatorSansLite/MutatorSansLightWide.ufo/features.fea
+-rw-r--r--  2.0 unx     2537 b- defN 23-Aug-07 15:30 fontmake-3.7.1/tests/data/MutatorSansLite/MutatorSansLightWide.ufo/glyphs.master_width_720.00_weight_645.00/S_.glif
+-rw-r--r--  2.0 unx      228 b- defN 23-Aug-07 15:30 fontmake-3.7.1/tests/data/MutatorSansLite/MutatorSansLightWide.ufo/glyphs.master_width_720.00_weight_645.00/contents.plist
+-rw-r--r--  2.0 unx      341 b- defN 23-Aug-07 15:30 fontmake-3.7.1/tests/data/MutatorSansLite/MutatorSansLightWide.ufo/glyphs.master_width_720.00_weight_645.00/layerinfo.plist
+-rw-r--r--  2.0 unx      246 b- defN 23-Aug-07 15:30 fontmake-3.7.1/tests/data/MutatorSansLite/MutatorSansLightWide.ufo/glyphs.background/contents.plist
+-rw-r--r--  2.0 unx      240 b- defN 23-Aug-07 15:30 fontmake-3.7.1/tests/data/MutatorSansLite/MutatorSansLightWide.ufo/glyphs.background/layerinfo.plist
+-rw-r--r--  2.0 unx     1818 b- defN 23-Aug-07 15:30 fontmake-3.7.1/tests/data/MutatorSansLite/MutatorSansLightWide.ufo/glyphs.background/S_.closed.glif
+-rw-r--r--  2.0 unx     2188 b- defN 23-Aug-07 15:30 fontmake-3.7.1/tests/data/MutatorSansLite/MutatorSansLightWide.ufo/glyphs/S_.glif
+-rw-r--r--  2.0 unx      654 b- defN 23-Aug-07 15:30 fontmake-3.7.1/tests/data/MutatorSansLite/MutatorSansLightWide.ufo/glyphs/I_.narrow.glif
+-rw-r--r--  2.0 unx      473 b- defN 23-Aug-07 15:30 fontmake-3.7.1/tests/data/MutatorSansLite/MutatorSansLightWide.ufo/glyphs/contents.plist
+-rw-r--r--  2.0 unx      691 b- defN 23-Aug-07 15:30 fontmake-3.7.1/tests/data/MutatorSansLite/MutatorSansLightWide.ufo/glyphs/I_.glif
+-rw-r--r--  2.0 unx     1222 b- defN 23-Aug-07 15:30 fontmake-3.7.1/tests/data/MutatorSansLite/MutatorSansLightWide.ufo/glyphs/A_.glif
+-rw-r--r--  2.0 unx     1065 b- defN 23-Aug-07 15:30 fontmake-3.7.1/tests/data/MutatorSansLite/MutatorSansLightWide.ufo/glyphs/I_J_.glif
+-rw-r--r--  2.0 unx      353 b- defN 23-Aug-07 15:30 fontmake-3.7.1/tests/data/MutatorSansLite/MutatorSansLightWide.ufo/glyphs/layerinfo.plist
+-rw-r--r--  2.0 unx     1831 b- defN 23-Aug-07 15:30 fontmake-3.7.1/tests/data/MutatorSansLite/MutatorSansLightWide.ufo/glyphs/S_.closed.glif
+-rw-r--r--  2.0 unx      181 b- defN 23-Aug-07 15:30 fontmake-3.7.1/tests/data/MutatorSansLite/MutatorSansLightWide.ufo/glyphs.master_width_695.65_weight_166.38/contents.plist
+-rw-r--r--  2.0 unx      236 b- defN 23-Aug-07 15:30 fontmake-3.7.1/tests/data/MutatorSansLite/MutatorSansLightWide.ufo/glyphs.master_width_695.65_weight_166.38/layerinfo.plist
+-rw-r--r--  2.0 unx      181 b- defN 23-Aug-07 15:30 fontmake-3.7.1/tests/data/MutatorSansLite/MutatorSansLightWide.ufo/glyphs.master_width_0.00_weight_0.00/contents.plist
+-rw-r--r--  2.0 unx      237 b- defN 23-Aug-07 15:30 fontmake-3.7.1/tests/data/MutatorSansLite/MutatorSansLightWide.ufo/glyphs.master_width_0.00_weight_0.00/layerinfo.plist
+-rw-r--r--  2.0 unx     2459 b- defN 23-Aug-07 15:30 fontmake-3.7.1/tests/data/MutatorSansLite/MutatorSansLightWide.ufo/glyphs.master_width_500.00_weight_500.00/S_.glif
+-rw-r--r--  2.0 unx      228 b- defN 23-Aug-07 15:30 fontmake-3.7.1/tests/data/MutatorSansLite/MutatorSansLightWide.ufo/glyphs.master_width_500.00_weight_500.00/contents.plist
+-rw-r--r--  2.0 unx      344 b- defN 23-Aug-07 15:30 fontmake-3.7.1/tests/data/MutatorSansLite/MutatorSansLightWide.ufo/glyphs.master_width_500.00_weight_500.00/layerinfo.plist
+drwxr-xr-x  2.0 unx        0 b- stor 23-Aug-07 15:30 fontmake-3.7.1/tests/data/MutatorSansLite/MutatorSansBoldWide.ufo/glyphs.background/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Aug-07 15:30 fontmake-3.7.1/tests/data/MutatorSansLite/MutatorSansBoldWide.ufo/glyphs/
+-rw-r--r--  2.0 unx      308 b- defN 23-Aug-07 15:30 fontmake-3.7.1/tests/data/MutatorSansLite/MutatorSansBoldWide.ufo/metainfo.plist
+-rw-r--r--  2.0 unx     1826 b- defN 23-Aug-07 15:30 fontmake-3.7.1/tests/data/MutatorSansLite/MutatorSansBoldWide.ufo/fontinfo.plist
+-rw-r--r--  2.0 unx      361 b- defN 23-Aug-07 15:30 fontmake-3.7.1/tests/data/MutatorSansLite/MutatorSansBoldWide.ufo/layercontents.plist
+-rw-r--r--  2.0 unx    10710 b- defN 23-Aug-07 15:30 fontmake-3.7.1/tests/data/MutatorSansLite/MutatorSansBoldWide.ufo/lib.plist
+-rw-r--r--  2.0 unx       36 b- defN 23-Aug-07 15:30 fontmake-3.7.1/tests/data/MutatorSansLite/MutatorSansBoldWide.ufo/features.fea
+-rw-r--r--  2.0 unx     1865 b- defN 23-Aug-07 15:30 fontmake-3.7.1/tests/data/MutatorSansLite/MutatorSansBoldWide.ufo/glyphs.background/S_.glif
+-rw-r--r--  2.0 unx      288 b- defN 23-Aug-07 15:30 fontmake-3.7.1/tests/data/MutatorSansLite/MutatorSansBoldWide.ufo/glyphs.background/contents.plist
+-rw-r--r--  2.0 unx      240 b- defN 23-Aug-07 15:30 fontmake-3.7.1/tests/data/MutatorSansLite/MutatorSansBoldWide.ufo/glyphs.background/layerinfo.plist
+-rw-r--r--  2.0 unx     1847 b- defN 23-Aug-07 15:30 fontmake-3.7.1/tests/data/MutatorSansLite/MutatorSansBoldWide.ufo/glyphs.background/S_.closed.glif
+-rw-r--r--  2.0 unx     2206 b- defN 23-Aug-07 15:30 fontmake-3.7.1/tests/data/MutatorSansLite/MutatorSansBoldWide.ufo/glyphs/S_.glif
+-rw-r--r--  2.0 unx      652 b- defN 23-Aug-07 15:30 fontmake-3.7.1/tests/data/MutatorSansLite/MutatorSansBoldWide.ufo/glyphs/I_.narrow.glif
+-rw-r--r--  2.0 unx      473 b- defN 23-Aug-07 15:30 fontmake-3.7.1/tests/data/MutatorSansLite/MutatorSansBoldWide.ufo/glyphs/contents.plist
+-rw-r--r--  2.0 unx      690 b- defN 23-Aug-07 15:30 fontmake-3.7.1/tests/data/MutatorSansLite/MutatorSansBoldWide.ufo/glyphs/I_.glif
+-rw-r--r--  2.0 unx      879 b- defN 23-Aug-07 15:30 fontmake-3.7.1/tests/data/MutatorSansLite/MutatorSansBoldWide.ufo/glyphs/A_.glif
+-rw-r--r--  2.0 unx     1062 b- defN 23-Aug-07 15:30 fontmake-3.7.1/tests/data/MutatorSansLite/MutatorSansBoldWide.ufo/glyphs/I_J_.glif
+-rw-r--r--  2.0 unx      353 b- defN 23-Aug-07 15:30 fontmake-3.7.1/tests/data/MutatorSansLite/MutatorSansBoldWide.ufo/glyphs/layerinfo.plist
+-rw-r--r--  2.0 unx     2192 b- defN 23-Aug-07 15:30 fontmake-3.7.1/tests/data/MutatorSansLite/MutatorSansBoldWide.ufo/glyphs/S_.closed.glif
+drwxr-xr-x  2.0 unx        0 b- stor 23-Aug-07 15:30 fontmake-3.7.1/tests/data/MutatorSansLite/MutatorSansBoldCondensed.ufo/glyphs.background/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Aug-07 15:30 fontmake-3.7.1/tests/data/MutatorSansLite/MutatorSansBoldCondensed.ufo/glyphs/
+-rw-r--r--  2.0 unx      308 b- defN 23-Aug-07 15:30 fontmake-3.7.1/tests/data/MutatorSansLite/MutatorSansBoldCondensed.ufo/metainfo.plist
+-rw-r--r--  2.0 unx     1841 b- defN 23-Aug-07 15:30 fontmake-3.7.1/tests/data/MutatorSansLite/MutatorSansBoldCondensed.ufo/fontinfo.plist
+-rw-r--r--  2.0 unx      361 b- defN 23-Aug-07 15:30 fontmake-3.7.1/tests/data/MutatorSansLite/MutatorSansBoldCondensed.ufo/layercontents.plist
+-rw-r--r--  2.0 unx     6839 b- defN 23-Aug-07 15:30 fontmake-3.7.1/tests/data/MutatorSansLite/MutatorSansBoldCondensed.ufo/lib.plist
+-rw-r--r--  2.0 unx       42 b- defN 23-Aug-07 15:30 fontmake-3.7.1/tests/data/MutatorSansLite/MutatorSansBoldCondensed.ufo/features.fea
+-rw-r--r--  2.0 unx      246 b- defN 23-Aug-07 15:30 fontmake-3.7.1/tests/data/MutatorSansLite/MutatorSansBoldCondensed.ufo/glyphs.background/contents.plist
+-rw-r--r--  2.0 unx      240 b- defN 23-Aug-07 15:30 fontmake-3.7.1/tests/data/MutatorSansLite/MutatorSansBoldCondensed.ufo/glyphs.background/layerinfo.plist
+-rw-r--r--  2.0 unx     1849 b- defN 23-Aug-07 15:30 fontmake-3.7.1/tests/data/MutatorSansLite/MutatorSansBoldCondensed.ufo/glyphs.background/S_.closed.glif
+-rw-r--r--  2.0 unx     2197 b- defN 23-Aug-07 15:30 fontmake-3.7.1/tests/data/MutatorSansLite/MutatorSansBoldCondensed.ufo/glyphs/S_.glif
+-rw-r--r--  2.0 unx      652 b- defN 23-Aug-07 15:30 fontmake-3.7.1/tests/data/MutatorSansLite/MutatorSansBoldCondensed.ufo/glyphs/I_.narrow.glif
+-rw-r--r--  2.0 unx      473 b- defN 23-Aug-07 15:30 fontmake-3.7.1/tests/data/MutatorSansLite/MutatorSansBoldCondensed.ufo/glyphs/contents.plist
+-rw-r--r--  2.0 unx      689 b- defN 23-Aug-07 15:30 fontmake-3.7.1/tests/data/MutatorSansLite/MutatorSansBoldCondensed.ufo/glyphs/I_.glif
+-rw-r--r--  2.0 unx     1221 b- defN 23-Aug-07 15:30 fontmake-3.7.1/tests/data/MutatorSansLite/MutatorSansBoldCondensed.ufo/glyphs/A_.glif
+-rw-r--r--  2.0 unx     1057 b- defN 23-Aug-07 15:30 fontmake-3.7.1/tests/data/MutatorSansLite/MutatorSansBoldCondensed.ufo/glyphs/I_J_.glif
+-rw-r--r--  2.0 unx      353 b- defN 23-Aug-07 15:30 fontmake-3.7.1/tests/data/MutatorSansLite/MutatorSansBoldCondensed.ufo/glyphs/layerinfo.plist
+-rw-r--r--  2.0 unx     2099 b- defN 23-Aug-07 15:30 fontmake-3.7.1/tests/data/MutatorSansLite/MutatorSansBoldCondensed.ufo/glyphs/S_.closed.glif
+drwxr-xr-x  2.0 unx        0 b- stor 23-Aug-07 15:30 fontmake-3.7.1/tests/data/MutatorSansLite/MutatorSerifLightWide.ufo/glyphs/
+-rw-r--r--  2.0 unx      308 b- defN 23-Aug-07 15:30 fontmake-3.7.1/tests/data/MutatorSansLite/MutatorSerifLightWide.ufo/metainfo.plist
+-rw-r--r--  2.0 unx     1834 b- defN 23-Aug-07 15:30 fontmake-3.7.1/tests/data/MutatorSansLite/MutatorSerifLightWide.ufo/fontinfo.plist
+-rw-r--r--  2.0 unx      271 b- defN 23-Aug-07 15:30 fontmake-3.7.1/tests/data/MutatorSansLite/MutatorSerifLightWide.ufo/layercontents.plist
+-rw-r--r--  2.0 unx    16116 b- defN 23-Aug-07 15:30 fontmake-3.7.1/tests/data/MutatorSansLite/MutatorSerifLightWide.ufo/lib.plist
+-rw-r--r--  2.0 unx       37 b- defN 23-Aug-07 15:30 fontmake-3.7.1/tests/data/MutatorSansLite/MutatorSerifLightWide.ufo/features.fea
+-rw-r--r--  2.0 unx      232 b- defN 23-Aug-07 15:30 fontmake-3.7.1/tests/data/MutatorSansLite/MutatorSerifLightWide.ufo/glyphs/contents.plist
+-rw-r--r--  2.0 unx     1578 b- defN 23-Aug-07 15:30 fontmake-3.7.1/tests/data/MutatorSansLite/MutatorSerifLightWide.ufo/glyphs/A_.glif
+drwxr-xr-x  2.0 unx        0 b- stor 23-Aug-07 15:30 fontmake-3.7.1/tests/data/MutatorSansLite/MutatorSansLightCondensed.ufo/glyphs.support.crossbars/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Aug-07 15:30 fontmake-3.7.1/tests/data/MutatorSansLite/MutatorSansLightCondensed.ufo/glyphs.support.S_.wide/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Aug-07 15:30 fontmake-3.7.1/tests/data/MutatorSansLite/MutatorSansLightCondensed.ufo/glyphs.support.S_.middle/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Aug-07 15:30 fontmake-3.7.1/tests/data/MutatorSansLite/MutatorSansLightCondensed.ufo/glyphs.background/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Aug-07 15:30 fontmake-3.7.1/tests/data/MutatorSansLite/MutatorSansLightCondensed.ufo/glyphs/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Aug-07 15:30 fontmake-3.7.1/tests/data/MutatorSansLite/MutatorSansLightCondensed.ufo/glyphs.support.crossbar/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Aug-07 15:30 fontmake-3.7.1/tests/data/MutatorSansLite/MutatorSansLightCondensed.ufo/glyphs.support/
+-rw-r--r--  2.0 unx      308 b- defN 23-Aug-07 15:30 fontmake-3.7.1/tests/data/MutatorSansLite/MutatorSansLightCondensed.ufo/metainfo.plist
+-rw-r--r--  2.0 unx     1844 b- defN 23-Aug-07 15:30 fontmake-3.7.1/tests/data/MutatorSansLite/MutatorSansLightCondensed.ufo/fontinfo.plist
+-rw-r--r--  2.0 unx      749 b- defN 23-Aug-07 15:30 fontmake-3.7.1/tests/data/MutatorSansLite/MutatorSansLightCondensed.ufo/layercontents.plist
+-rw-r--r--  2.0 unx    16556 b- defN 23-Aug-07 15:30 fontmake-3.7.1/tests/data/MutatorSansLite/MutatorSansLightCondensed.ufo/lib.plist
+-rw-r--r--  2.0 unx       68 b- defN 23-Aug-07 15:30 fontmake-3.7.1/tests/data/MutatorSansLite/MutatorSansLightCondensed.ufo/features.fea
+-rw-r--r--  2.0 unx      238 b- defN 23-Aug-07 15:30 fontmake-3.7.1/tests/data/MutatorSansLite/MutatorSansLightCondensed.ufo/glyphs.support.crossbars/contents.plist
+-rw-r--r--  2.0 unx     1176 b- defN 23-Aug-07 15:30 fontmake-3.7.1/tests/data/MutatorSansLite/MutatorSansLightCondensed.ufo/glyphs.support.crossbars/E_.glif
+-rw-r--r--  2.0 unx      183 b- defN 23-Aug-07 15:30 fontmake-3.7.1/tests/data/MutatorSansLite/MutatorSansLightCondensed.ufo/glyphs.support.crossbars/layerinfo.plist
+-rw-r--r--  2.0 unx     3051 b- defN 23-Aug-07 15:30 fontmake-3.7.1/tests/data/MutatorSansLite/MutatorSansLightCondensed.ufo/glyphs.support.S_.wide/S_.glif
+-rw-r--r--  2.0 unx      288 b- defN 23-Aug-07 15:30 fontmake-3.7.1/tests/data/MutatorSansLite/MutatorSansLightCondensed.ufo/glyphs.support.S_.wide/contents.plist
+-rw-r--r--  2.0 unx      241 b- defN 23-Aug-07 15:30 fontmake-3.7.1/tests/data/MutatorSansLite/MutatorSansLightCondensed.ufo/glyphs.support.S_.wide/layerinfo.plist
+-rw-r--r--  2.0 unx     3060 b- defN 23-Aug-07 15:30 fontmake-3.7.1/tests/data/MutatorSansLite/MutatorSansLightCondensed.ufo/glyphs.support.S_.wide/S_.closed.glif
+-rw-r--r--  2.0 unx      246 b- defN 23-Aug-07 15:30 fontmake-3.7.1/tests/data/MutatorSansLite/MutatorSansLightCondensed.ufo/glyphs.support.S_.middle/contents.plist
+-rw-r--r--  2.0 unx      240 b- defN 23-Aug-07 15:30 fontmake-3.7.1/tests/data/MutatorSansLite/MutatorSansLightCondensed.ufo/glyphs.support.S_.middle/layerinfo.plist
+-rw-r--r--  2.0 unx     2492 b- defN 23-Aug-07 15:30 fontmake-3.7.1/tests/data/MutatorSansLite/MutatorSansLightCondensed.ufo/glyphs.support.S_.middle/S_.closed.glif
+-rw-r--r--  2.0 unx     2617 b- defN 23-Aug-07 15:30 fontmake-3.7.1/tests/data/MutatorSansLite/MutatorSansLightCondensed.ufo/glyphs.background/S_.glif
+-rw-r--r--  2.0 unx      288 b- defN 23-Aug-07 15:30 fontmake-3.7.1/tests/data/MutatorSansLite/MutatorSansLightCondensed.ufo/glyphs.background/contents.plist
+-rw-r--r--  2.0 unx      238 b- defN 23-Aug-07 15:30 fontmake-3.7.1/tests/data/MutatorSansLite/MutatorSansLightCondensed.ufo/glyphs.background/layerinfo.plist
+-rw-r--r--  2.0 unx     3539 b- defN 23-Aug-07 15:30 fontmake-3.7.1/tests/data/MutatorSansLite/MutatorSansLightCondensed.ufo/glyphs.background/S_.closed.glif
+-rw-r--r--  2.0 unx     2247 b- defN 23-Aug-07 15:30 fontmake-3.7.1/tests/data/MutatorSansLite/MutatorSansLightCondensed.ufo/glyphs/S_.glif
+-rw-r--r--  2.0 unx      652 b- defN 23-Aug-07 15:30 fontmake-3.7.1/tests/data/MutatorSansLite/MutatorSansLightCondensed.ufo/glyphs/I_.narrow.glif
+-rw-r--r--  2.0 unx      473 b- defN 23-Aug-07 15:30 fontmake-3.7.1/tests/data/MutatorSansLite/MutatorSansLightCondensed.ufo/glyphs/contents.plist
+-rw-r--r--  2.0 unx      687 b- defN 23-Aug-07 15:30 fontmake-3.7.1/tests/data/MutatorSansLite/MutatorSansLightCondensed.ufo/glyphs/I_.glif
+-rw-r--r--  2.0 unx      874 b- defN 23-Aug-07 15:30 fontmake-3.7.1/tests/data/MutatorSansLite/MutatorSansLightCondensed.ufo/glyphs/A_.glif
+-rw-r--r--  2.0 unx     1028 b- defN 23-Aug-07 15:30 fontmake-3.7.1/tests/data/MutatorSansLite/MutatorSansLightCondensed.ufo/glyphs/I_J_.glif
+-rw-r--r--  2.0 unx      353 b- defN 23-Aug-07 15:30 fontmake-3.7.1/tests/data/MutatorSansLite/MutatorSansLightCondensed.ufo/glyphs/layerinfo.plist
+-rw-r--r--  2.0 unx     1827 b- defN 23-Aug-07 15:30 fontmake-3.7.1/tests/data/MutatorSansLite/MutatorSansLightCondensed.ufo/glyphs/S_.closed.glif
+-rw-r--r--  2.0 unx     3007 b- defN 23-Aug-07 15:30 fontmake-3.7.1/tests/data/MutatorSansLite/MutatorSansLightCondensed.ufo/glyphs.support.crossbar/S_.glif
+-rw-r--r--  2.0 unx      232 b- defN 23-Aug-07 15:30 fontmake-3.7.1/tests/data/MutatorSansLite/MutatorSansLightCondensed.ufo/glyphs.support.crossbar/contents.plist
+-rw-r--r--  2.0 unx      241 b- defN 23-Aug-07 15:30 fontmake-3.7.1/tests/data/MutatorSansLite/MutatorSansLightCondensed.ufo/glyphs.support.crossbar/layerinfo.plist
+-rw-r--r--  2.0 unx     2474 b- defN 23-Aug-07 15:30 fontmake-3.7.1/tests/data/MutatorSansLite/MutatorSansLightCondensed.ufo/glyphs.support/S_.glif
+-rw-r--r--  2.0 unx      274 b- defN 23-Aug-07 15:30 fontmake-3.7.1/tests/data/MutatorSansLite/MutatorSansLightCondensed.ufo/glyphs.support/contents.plist
+-rw-r--r--  2.0 unx      732 b- defN 23-Aug-07 15:30 fontmake-3.7.1/tests/data/MutatorSansLite/MutatorSansLightCondensed.ufo/glyphs.support/A_.glif
+-rw-r--r--  2.0 unx      353 b- defN 23-Aug-07 15:30 fontmake-3.7.1/tests/data/MutatorSansLite/MutatorSansLightCondensed.ufo/glyphs.support/layerinfo.plist
+drwxr-xr-x  2.0 unx        0 b- stor 23-Aug-07 15:30 fontmake-3.7.1/tests/data/MutatorSansLite/MutatorSerifLightCondensed.ufo/glyphs/
+-rw-r--r--  2.0 unx      308 b- defN 23-Aug-07 15:30 fontmake-3.7.1/tests/data/MutatorSansLite/MutatorSerifLightCondensed.ufo/metainfo.plist
+-rw-r--r--  2.0 unx     1849 b- defN 23-Aug-07 15:30 fontmake-3.7.1/tests/data/MutatorSansLite/MutatorSerifLightCondensed.ufo/fontinfo.plist
+-rw-r--r--  2.0 unx      271 b- defN 23-Aug-07 15:30 fontmake-3.7.1/tests/data/MutatorSansLite/MutatorSerifLightCondensed.ufo/layercontents.plist
+-rw-r--r--  2.0 unx    16556 b- defN 23-Aug-07 15:30 fontmake-3.7.1/tests/data/MutatorSansLite/MutatorSerifLightCondensed.ufo/lib.plist
+-rw-r--r--  2.0 unx       68 b- defN 23-Aug-07 15:30 fontmake-3.7.1/tests/data/MutatorSansLite/MutatorSerifLightCondensed.ufo/features.fea
+-rw-r--r--  2.0 unx      232 b- defN 23-Aug-07 15:30 fontmake-3.7.1/tests/data/MutatorSansLite/MutatorSerifLightCondensed.ufo/glyphs/contents.plist
+-rw-r--r--  2.0 unx     1228 b- defN 23-Aug-07 15:30 fontmake-3.7.1/tests/data/MutatorSansLite/MutatorSerifLightCondensed.ufo/glyphs/A_.glif
+drwxr-xr-x  2.0 unx        0 b- stor 23-Aug-07 15:30 fontmake-3.7.1/tests/data/InstantiatorStrictMathGlyph/SquareTwo.ufo/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Aug-07 15:30 fontmake-3.7.1/tests/data/InstantiatorStrictMathGlyph/SquareOne.ufo/
+-rw-r--r--  2.0 unx      830 b- defN 23-Aug-07 15:30 fontmake-3.7.1/tests/data/InstantiatorStrictMathGlyph/StrictMathGlyph.designspace
+drwxr-xr-x  2.0 unx        0 b- stor 23-Aug-07 15:30 fontmake-3.7.1/tests/data/InstantiatorStrictMathGlyph/SquareTwo.ufo/glyphs/
+-rw-r--r--  2.0 unx      318 b- defN 23-Aug-07 15:30 fontmake-3.7.1/tests/data/InstantiatorStrictMathGlyph/SquareTwo.ufo/metainfo.plist
+-rw-r--r--  2.0 unx      900 b- defN 23-Aug-07 15:30 fontmake-3.7.1/tests/data/InstantiatorStrictMathGlyph/SquareTwo.ufo/fontinfo.plist
+-rw-r--r--  2.0 unx      283 b- defN 23-Aug-07 15:30 fontmake-3.7.1/tests/data/InstantiatorStrictMathGlyph/SquareTwo.ufo/layercontents.plist
+-rw-r--r--  2.0 unx     1030 b- defN 23-Aug-07 15:30 fontmake-3.7.1/tests/data/InstantiatorStrictMathGlyph/SquareTwo.ufo/lib.plist
+-rw-r--r--  2.0 unx      786 b- defN 23-Aug-07 15:30 fontmake-3.7.1/tests/data/InstantiatorStrictMathGlyph/SquareTwo.ufo/glyphs/test.glif
+-rw-r--r--  2.0 unx      243 b- defN 23-Aug-07 15:30 fontmake-3.7.1/tests/data/InstantiatorStrictMathGlyph/SquareTwo.ufo/glyphs/contents.plist
+-rw-r--r--  2.0 unx      247 b- defN 23-Aug-07 15:30 fontmake-3.7.1/tests/data/InstantiatorStrictMathGlyph/SquareTwo.ufo/glyphs/layerinfo.plist
+drwxr-xr-x  2.0 unx        0 b- stor 23-Aug-07 15:30 fontmake-3.7.1/tests/data/InstantiatorStrictMathGlyph/SquareOne.ufo/glyphs/
+-rw-r--r--  2.0 unx      318 b- defN 23-Aug-07 15:30 fontmake-3.7.1/tests/data/InstantiatorStrictMathGlyph/SquareOne.ufo/metainfo.plist
+-rw-r--r--  2.0 unx      897 b- defN 23-Aug-07 15:30 fontmake-3.7.1/tests/data/InstantiatorStrictMathGlyph/SquareOne.ufo/fontinfo.plist
+-rw-r--r--  2.0 unx      283 b- defN 23-Aug-07 15:30 fontmake-3.7.1/tests/data/InstantiatorStrictMathGlyph/SquareOne.ufo/layercontents.plist
+-rw-r--r--  2.0 unx     1030 b- defN 23-Aug-07 15:30 fontmake-3.7.1/tests/data/InstantiatorStrictMathGlyph/SquareOne.ufo/lib.plist
+-rw-r--r--  2.0 unx      770 b- defN 23-Aug-07 15:30 fontmake-3.7.1/tests/data/InstantiatorStrictMathGlyph/SquareOne.ufo/glyphs/test.glif
+-rw-r--r--  2.0 unx      243 b- defN 23-Aug-07 15:30 fontmake-3.7.1/tests/data/InstantiatorStrictMathGlyph/SquareOne.ufo/glyphs/contents.plist
+-rw-r--r--  2.0 unx      247 b- defN 23-Aug-07 15:30 fontmake-3.7.1/tests/data/InstantiatorStrictMathGlyph/SquareOne.ufo/glyphs/layerinfo.plist
+drwxr-xr-x  2.0 unx        0 b- stor 23-Aug-07 15:30 fontmake-3.7.1/tests/data/MutatorSans/MutatorSansLightWide.ufo/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Aug-07 15:30 fontmake-3.7.1/tests/data/MutatorSans/MutatorSansBoldWide.ufo/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Aug-07 15:30 fontmake-3.7.1/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Aug-07 15:30 fontmake-3.7.1/tests/data/MutatorSans/MutatorSansIntermediateCondensed.ufo/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Aug-07 15:30 fontmake-3.7.1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Aug-07 15:30 fontmake-3.7.1/tests/data/MutatorSans/MutatorSansIntermediateWide.ufo/
+-rw-r--r--  2.0 unx     1394 b- defN 23-Aug-07 15:30 fontmake-3.7.1/tests/data/MutatorSans/MutatorSans-width-only.designspace
+-rw-r--r--  2.0 unx     1074 b- defN 23-Aug-07 15:30 fontmake-3.7.1/tests/data/MutatorSans/LICENSE
+-rw-r--r--  2.0 unx     1412 b- defN 23-Aug-07 15:30 fontmake-3.7.1/tests/data/MutatorSans/MutatorSans-weight-only.designspace
+-rw-r--r--  2.0 unx     7834 b- defN 23-Aug-07 15:30 fontmake-3.7.1/tests/data/MutatorSans/MutatorSans_no_default.designspace
+-rw-r--r--  2.0 unx     8462 b- defN 23-Aug-07 15:30 fontmake-3.7.1/tests/data/MutatorSans/MutatorSans_missing.designspace
+-rw-r--r--  2.0 unx     2611 b- defN 23-Aug-07 15:30 fontmake-3.7.1/tests/data/MutatorSans/MutatorSans-with-openNodes.designspace
+-rw-r--r--  2.0 unx     7111 b- defN 23-Aug-07 15:30 fontmake-3.7.1/tests/data/MutatorSans/MutatorSans.designspace
+-rw-r--r--  2.0 unx     1067 b- defN 23-Aug-07 15:30 fontmake-3.7.1/tests/data/MutatorSans/MutatorSans-non-default-layer.designspace
+drwxr-xr-x  2.0 unx        0 b- stor 23-Aug-07 15:30 fontmake-3.7.1/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs.master_width_720.00_weight_645.00/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Aug-07 15:30 fontmake-3.7.1/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs.background/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Aug-07 15:30 fontmake-3.7.1/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Aug-07 15:30 fontmake-3.7.1/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs.master_width_695.65_weight_166.38/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Aug-07 15:30 fontmake-3.7.1/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs.master_width_0.00_weight_0.00/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Aug-07 15:30 fontmake-3.7.1/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs.master_width_500.00_weight_500.00/
+-rw-r--r--  2.0 unx      318 b- defN 23-Aug-07 15:30 fontmake-3.7.1/tests/data/MutatorSans/MutatorSansLightWide.ufo/metainfo.plist
+-rw-r--r--  2.0 unx     4852 b- defN 23-Aug-07 15:30 fontmake-3.7.1/tests/data/MutatorSans/MutatorSansLightWide.ufo/kerning.plist
+-rw-r--r--  2.0 unx      366 b- defN 23-Aug-07 15:30 fontmake-3.7.1/tests/data/MutatorSans/MutatorSansLightWide.ufo/groups.plist
+-rw-r--r--  2.0 unx     1873 b- defN 23-Aug-07 15:30 fontmake-3.7.1/tests/data/MutatorSans/MutatorSansLightWide.ufo/fontinfo.plist
+-rw-r--r--  2.0 unx      383 b- defN 23-Aug-07 15:30 fontmake-3.7.1/tests/data/MutatorSans/MutatorSansLightWide.ufo/layercontents.plist
+-rw-r--r--  2.0 unx    18291 b- defN 23-Aug-07 15:30 fontmake-3.7.1/tests/data/MutatorSans/MutatorSansLightWide.ufo/lib.plist
+-rw-r--r--  2.0 unx       37 b- defN 23-Aug-07 15:30 fontmake-3.7.1/tests/data/MutatorSans/MutatorSansLightWide.ufo/features.fea
+-rw-r--r--  2.0 unx     2537 b- defN 23-Aug-07 15:30 fontmake-3.7.1/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs.master_width_720.00_weight_645.00/S_.glif
+-rw-r--r--  2.0 unx      228 b- defN 23-Aug-07 15:30 fontmake-3.7.1/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs.master_width_720.00_weight_645.00/contents.plist
+-rw-r--r--  2.0 unx      341 b- defN 23-Aug-07 15:30 fontmake-3.7.1/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs.master_width_720.00_weight_645.00/layerinfo.plist
+-rw-r--r--  2.0 unx      252 b- defN 23-Aug-07 15:30 fontmake-3.7.1/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs.background/contents.plist
+-rw-r--r--  2.0 unx      246 b- defN 23-Aug-07 15:30 fontmake-3.7.1/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs.background/layerinfo.plist
+-rw-r--r--  2.0 unx     1965 b- defN 23-Aug-07 15:30 fontmake-3.7.1/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs.background/S_.closed.glif
+-rw-r--r--  2.0 unx      517 b- defN 23-Aug-07 15:30 fontmake-3.7.1/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/arrowup.glif
+-rw-r--r--  2.0 unx      747 b- defN 23-Aug-07 15:30 fontmake-3.7.1/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/Y_.glif
+-rw-r--r--  2.0 unx      752 b- defN 23-Aug-07 15:30 fontmake-3.7.1/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/Z_.glif
+-rw-r--r--  2.0 unx      802 b- defN 23-Aug-07 15:30 fontmake-3.7.1/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/J_.narrow.glif
+-rw-r--r--  2.0 unx      549 b- defN 23-Aug-07 15:30 fontmake-3.7.1/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/T_.glif
+-rw-r--r--  2.0 unx      354 b- defN 23-Aug-07 15:30 fontmake-3.7.1/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/A_acute.glif
+-rw-r--r--  2.0 unx     1416 b- defN 23-Aug-07 15:30 fontmake-3.7.1/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/C_.glif
+-rw-r--r--  2.0 unx      518 b- defN 23-Aug-07 15:30 fontmake-3.7.1/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/arrowleft.glif
+-rw-r--r--  2.0 unx      233 b- defN 23-Aug-07 15:30 fontmake-3.7.1/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/semicolon.glif
+-rw-r--r--  2.0 unx      352 b- defN 23-Aug-07 15:30 fontmake-3.7.1/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/period.glif
+-rw-r--r--  2.0 unx      353 b- defN 23-Aug-07 15:30 fontmake-3.7.1/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/acute.glif
+-rw-r--r--  2.0 unx      542 b- defN 23-Aug-07 15:30 fontmake-3.7.1/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/L_.glif
+-rw-r--r--  2.0 unx     2358 b- defN 23-Aug-07 15:30 fontmake-3.7.1/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/S_.glif
+-rw-r--r--  2.0 unx      193 b- defN 23-Aug-07 15:30 fontmake-3.7.1/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/quotesinglbase.glif
+-rw-r--r--  2.0 unx      264 b- defN 23-Aug-07 15:30 fontmake-3.7.1/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/quotedblright.glif
+-rw-r--r--  2.0 unx     1785 b- defN 23-Aug-07 15:30 fontmake-3.7.1/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/B_.glif
+-rw-r--r--  2.0 unx     1130 b- defN 23-Aug-07 15:30 fontmake-3.7.1/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/P_.glif
+-rw-r--r--  2.0 unx      514 b- defN 23-Aug-07 15:30 fontmake-3.7.1/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/arrowdown.glif
+-rw-r--r--  2.0 unx      857 b- defN 23-Aug-07 15:30 fontmake-3.7.1/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/W_.glif
+-rw-r--r--  2.0 unx      521 b- defN 23-Aug-07 15:30 fontmake-3.7.1/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/comma.glif
+-rw-r--r--  2.0 unx      370 b- defN 23-Aug-07 15:30 fontmake-3.7.1/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/dieresis.glif
+-rw-r--r--  2.0 unx      325 b- defN 23-Aug-07 15:30 fontmake-3.7.1/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/quotedblleft.glif
+-rw-r--r--  2.0 unx      954 b- defN 23-Aug-07 15:30 fontmake-3.7.1/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/F_.glif
+-rw-r--r--  2.0 unx     1388 b- defN 23-Aug-07 15:30 fontmake-3.7.1/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/O_.glif
+-rw-r--r--  2.0 unx      360 b- defN 23-Aug-07 15:30 fontmake-3.7.1/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/A_dieresis.glif
+-rw-r--r--  2.0 unx      235 b- defN 23-Aug-07 15:30 fontmake-3.7.1/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/quotedblbase.glif
+-rw-r--r--  2.0 unx      154 b- defN 23-Aug-07 15:30 fontmake-3.7.1/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/space.glif
+-rw-r--r--  2.0 unx      518 b- defN 23-Aug-07 15:30 fontmake-3.7.1/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/arrowright.glif
+-rw-r--r--  2.0 unx      703 b- defN 23-Aug-07 15:30 fontmake-3.7.1/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/I_.narrow.glif
+-rw-r--r--  2.0 unx     2687 b- defN 23-Aug-07 15:30 fontmake-3.7.1/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/contents.plist
+-rw-r--r--  2.0 unx      750 b- defN 23-Aug-07 15:30 fontmake-3.7.1/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/H_.glif
+-rw-r--r--  2.0 unx      378 b- defN 23-Aug-07 15:30 fontmake-3.7.1/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/Q_.glif
+-rw-r--r--  2.0 unx     1357 b- defN 23-Aug-07 15:30 fontmake-3.7.1/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/E_.glif
+-rw-r--r--  2.0 unx     1056 b- defN 23-Aug-07 15:30 fontmake-3.7.1/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/J_.glif
+-rw-r--r--  2.0 unx     1134 b- defN 23-Aug-07 15:30 fontmake-3.7.1/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/D_.glif
+-rw-r--r--  2.0 unx     1751 b- defN 23-Aug-07 15:30 fontmake-3.7.1/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/G_.glif
+-rw-r--r--  2.0 unx      875 b- defN 23-Aug-07 15:30 fontmake-3.7.1/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/K_.glif
+-rw-r--r--  2.0 unx      743 b- defN 23-Aug-07 15:30 fontmake-3.7.1/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/I_.glif
+-rw-r--r--  2.0 unx     1320 b- defN 23-Aug-07 15:30 fontmake-3.7.1/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/A_.glif
+-rw-r--r--  2.0 unx      924 b- defN 23-Aug-07 15:30 fontmake-3.7.1/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/M_.glif
+-rw-r--r--  2.0 unx     1158 b- defN 23-Aug-07 15:30 fontmake-3.7.1/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/I_J_.glif
+-rw-r--r--  2.0 unx      740 b- defN 23-Aug-07 15:30 fontmake-3.7.1/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/V_.glif
+-rw-r--r--  2.0 unx      801 b- defN 23-Aug-07 15:30 fontmake-3.7.1/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/X_.glif
+-rw-r--r--  2.0 unx      371 b- defN 23-Aug-07 15:30 fontmake-3.7.1/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/layerinfo.plist
+-rw-r--r--  2.0 unx      749 b- defN 23-Aug-07 15:30 fontmake-3.7.1/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/N_.glif
+-rw-r--r--  2.0 unx      230 b- defN 23-Aug-07 15:30 fontmake-3.7.1/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/colon.glif
+-rw-r--r--  2.0 unx      349 b- defN 23-Aug-07 15:30 fontmake-3.7.1/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/dot.glif
+-rw-r--r--  2.0 unx     1459 b- defN 23-Aug-07 15:30 fontmake-3.7.1/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/R_.glif
+-rw-r--r--  2.0 unx     1970 b- defN 23-Aug-07 15:30 fontmake-3.7.1/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/S_.closed.glif
+-rw-r--r--  2.0 unx      943 b- defN 23-Aug-07 15:30 fontmake-3.7.1/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/U_.glif
+-rw-r--r--  2.0 unx      181 b- defN 23-Aug-07 15:30 fontmake-3.7.1/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs.master_width_695.65_weight_166.38/contents.plist
+-rw-r--r--  2.0 unx      236 b- defN 23-Aug-07 15:30 fontmake-3.7.1/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs.master_width_695.65_weight_166.38/layerinfo.plist
+-rw-r--r--  2.0 unx      181 b- defN 23-Aug-07 15:30 fontmake-3.7.1/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs.master_width_0.00_weight_0.00/contents.plist
+-rw-r--r--  2.0 unx      237 b- defN 23-Aug-07 15:30 fontmake-3.7.1/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs.master_width_0.00_weight_0.00/layerinfo.plist
+-rw-r--r--  2.0 unx     2459 b- defN 23-Aug-07 15:30 fontmake-3.7.1/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs.master_width_500.00_weight_500.00/S_.glif
+-rw-r--r--  2.0 unx      228 b- defN 23-Aug-07 15:30 fontmake-3.7.1/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs.master_width_500.00_weight_500.00/contents.plist
+-rw-r--r--  2.0 unx      344 b- defN 23-Aug-07 15:30 fontmake-3.7.1/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs.master_width_500.00_weight_500.00/layerinfo.plist
+drwxr-xr-x  2.0 unx        0 b- stor 23-Aug-07 15:30 fontmake-3.7.1/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs.background/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Aug-07 15:30 fontmake-3.7.1/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/
+-rw-r--r--  2.0 unx      318 b- defN 23-Aug-07 15:30 fontmake-3.7.1/tests/data/MutatorSans/MutatorSansBoldWide.ufo/metainfo.plist
+-rw-r--r--  2.0 unx      301 b- defN 23-Aug-07 15:30 fontmake-3.7.1/tests/data/MutatorSans/MutatorSansBoldWide.ufo/kerning.plist
+-rw-r--r--  2.0 unx      366 b- defN 23-Aug-07 15:30 fontmake-3.7.1/tests/data/MutatorSans/MutatorSansBoldWide.ufo/groups.plist
+-rw-r--r--  2.0 unx     1870 b- defN 23-Aug-07 15:30 fontmake-3.7.1/tests/data/MutatorSans/MutatorSansBoldWide.ufo/fontinfo.plist
+-rw-r--r--  2.0 unx      383 b- defN 23-Aug-07 15:30 fontmake-3.7.1/tests/data/MutatorSans/MutatorSansBoldWide.ufo/layercontents.plist
+-rw-r--r--  2.0 unx    12341 b- defN 23-Aug-07 15:30 fontmake-3.7.1/tests/data/MutatorSans/MutatorSansBoldWide.ufo/lib.plist
+-rw-r--r--  2.0 unx       36 b- defN 23-Aug-07 15:30 fontmake-3.7.1/tests/data/MutatorSans/MutatorSansBoldWide.ufo/features.fea
+-rw-r--r--  2.0 unx     2005 b- defN 23-Aug-07 15:30 fontmake-3.7.1/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs.background/S_.glif
+-rw-r--r--  2.0 unx      298 b- defN 23-Aug-07 15:30 fontmake-3.7.1/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs.background/contents.plist
+-rw-r--r--  2.0 unx      246 b- defN 23-Aug-07 15:30 fontmake-3.7.1/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs.background/layerinfo.plist
+-rw-r--r--  2.0 unx     1986 b- defN 23-Aug-07 15:30 fontmake-3.7.1/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs.background/S_.closed.glif
+-rw-r--r--  2.0 unx      492 b- defN 23-Aug-07 15:30 fontmake-3.7.1/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/arrowup.glif
+-rw-r--r--  2.0 unx      750 b- defN 23-Aug-07 15:30 fontmake-3.7.1/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/Y_.glif
+-rw-r--r--  2.0 unx      750 b- defN 23-Aug-07 15:30 fontmake-3.7.1/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/Z_.glif
+-rw-r--r--  2.0 unx      806 b- defN 23-Aug-07 15:30 fontmake-3.7.1/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/J_.narrow.glif
+-rw-r--r--  2.0 unx      549 b- defN 23-Aug-07 15:30 fontmake-3.7.1/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/T_.glif
+-rw-r--r--  2.0 unx      354 b- defN 23-Aug-07 15:30 fontmake-3.7.1/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/A_acute.glif
+-rw-r--r--  2.0 unx     1418 b- defN 23-Aug-07 15:30 fontmake-3.7.1/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/C_.glif
+-rw-r--r--  2.0 unx      493 b- defN 23-Aug-07 15:30 fontmake-3.7.1/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/arrowleft.glif
+-rw-r--r--  2.0 unx      245 b- defN 23-Aug-07 15:30 fontmake-3.7.1/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/semicolon.glif
+-rw-r--r--  2.0 unx      350 b- defN 23-Aug-07 15:30 fontmake-3.7.1/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/period.glif
+-rw-r--r--  2.0 unx      353 b- defN 23-Aug-07 15:30 fontmake-3.7.1/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/acute.glif
+-rw-r--r--  2.0 unx      545 b- defN 23-Aug-07 15:30 fontmake-3.7.1/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/L_.glif
+-rw-r--r--  2.0 unx     2376 b- defN 23-Aug-07 15:30 fontmake-3.7.1/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/S_.glif
+-rw-r--r--  2.0 unx      205 b- defN 23-Aug-07 15:30 fontmake-3.7.1/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/quotesinglbase.glif
+-rw-r--r--  2.0 unx      264 b- defN 23-Aug-07 15:30 fontmake-3.7.1/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/quotedblright.glif
+-rw-r--r--  2.0 unx     2203 b- defN 23-Aug-07 15:30 fontmake-3.7.1/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/B_.glif
+-rw-r--r--  2.0 unx     1140 b- defN 23-Aug-07 15:30 fontmake-3.7.1/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/P_.glif
+-rw-r--r--  2.0 unx      491 b- defN 23-Aug-07 15:30 fontmake-3.7.1/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/arrowdown.glif
+-rw-r--r--  2.0 unx      861 b- defN 23-Aug-07 15:30 fontmake-3.7.1/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/W_.glif
+-rw-r--r--  2.0 unx      522 b- defN 23-Aug-07 15:30 fontmake-3.7.1/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/comma.glif
+-rw-r--r--  2.0 unx      370 b- defN 23-Aug-07 15:30 fontmake-3.7.1/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/dieresis.glif
+-rw-r--r--  2.0 unx      325 b- defN 23-Aug-07 15:30 fontmake-3.7.1/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/quotedblleft.glif
+-rw-r--r--  2.0 unx      750 b- defN 23-Aug-07 15:30 fontmake-3.7.1/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/F_.glif
+-rw-r--r--  2.0 unx     1387 b- defN 23-Aug-07 15:30 fontmake-3.7.1/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/O_.glif
+-rw-r--r--  2.0 unx      360 b- defN 23-Aug-07 15:30 fontmake-3.7.1/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/A_dieresis.glif
+-rw-r--r--  2.0 unx      259 b- defN 23-Aug-07 15:30 fontmake-3.7.1/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/quotedblbase.glif
+-rw-r--r--  2.0 unx      154 b- defN 23-Aug-07 15:30 fontmake-3.7.1/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/space.glif
+-rw-r--r--  2.0 unx      495 b- defN 23-Aug-07 15:30 fontmake-3.7.1/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/arrowright.glif
+-rw-r--r--  2.0 unx      701 b- defN 23-Aug-07 15:30 fontmake-3.7.1/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/I_.narrow.glif
+-rw-r--r--  2.0 unx     2687 b- defN 23-Aug-07 15:30 fontmake-3.7.1/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/contents.plist
+-rw-r--r--  2.0 unx      748 b- defN 23-Aug-07 15:30 fontmake-3.7.1/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/H_.glif
+-rw-r--r--  2.0 unx      380 b- defN 23-Aug-07 15:30 fontmake-3.7.1/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/Q_.glif
+-rw-r--r--  2.0 unx      988 b- defN 23-Aug-07 15:30 fontmake-3.7.1/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/E_.glif
+-rw-r--r--  2.0 unx      940 b- defN 23-Aug-07 15:30 fontmake-3.7.1/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/J_.glif
+-rw-r--r--  2.0 unx     1150 b- defN 23-Aug-07 15:30 fontmake-3.7.1/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/D_.glif
+-rw-r--r--  2.0 unx     1747 b- defN 23-Aug-07 15:30 fontmake-3.7.1/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/G_.glif
+-rw-r--r--  2.0 unx      875 b- defN 23-Aug-07 15:30 fontmake-3.7.1/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/K_.glif
+-rw-r--r--  2.0 unx      742 b- defN 23-Aug-07 15:30 fontmake-3.7.1/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/I_.glif
+-rw-r--r--  2.0 unx      947 b- defN 23-Aug-07 15:30 fontmake-3.7.1/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/A_.glif
+-rw-r--r--  2.0 unx      919 b- defN 23-Aug-07 15:30 fontmake-3.7.1/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/M_.glif
+-rw-r--r--  2.0 unx     1154 b- defN 23-Aug-07 15:30 fontmake-3.7.1/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/I_J_.glif
+-rw-r--r--  2.0 unx      742 b- defN 23-Aug-07 15:30 fontmake-3.7.1/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/V_.glif
+-rw-r--r--  2.0 unx      803 b- defN 23-Aug-07 15:30 fontmake-3.7.1/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/X_.glif
+-rw-r--r--  2.0 unx      371 b- defN 23-Aug-07 15:30 fontmake-3.7.1/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/layerinfo.plist
+-rw-r--r--  2.0 unx      745 b- defN 23-Aug-07 15:30 fontmake-3.7.1/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/N_.glif
+-rw-r--r--  2.0 unx      242 b- defN 23-Aug-07 15:30 fontmake-3.7.1/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/colon.glif
+-rw-r--r--  2.0 unx      351 b- defN 23-Aug-07 15:30 fontmake-3.7.1/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/dot.glif
+-rw-r--r--  2.0 unx     1495 b- defN 23-Aug-07 15:30 fontmake-3.7.1/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/R_.glif
+-rw-r--r--  2.0 unx     2369 b- defN 23-Aug-07 15:30 fontmake-3.7.1/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/S_.closed.glif
+-rw-r--r--  2.0 unx     1037 b- defN 23-Aug-07 15:30 fontmake-3.7.1/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/U_.glif
+drwxr-xr-x  2.0 unx        0 b- stor 23-Aug-07 15:30 fontmake-3.7.1/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs.background/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Aug-07 15:30 fontmake-3.7.1/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/
+-rw-r--r--  2.0 unx      318 b- defN 23-Aug-07 15:30 fontmake-3.7.1/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/metainfo.plist
+-rw-r--r--  2.0 unx     4580 b- defN 23-Aug-07 15:30 fontmake-3.7.1/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/kerning.plist
+-rw-r--r--  2.0 unx      366 b- defN 23-Aug-07 15:30 fontmake-3.7.1/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/groups.plist
+-rw-r--r--  2.0 unx     1885 b- defN 23-Aug-07 15:30 fontmake-3.7.1/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/fontinfo.plist
+-rw-r--r--  2.0 unx      383 b- defN 23-Aug-07 15:30 fontmake-3.7.1/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/layercontents.plist
+-rw-r--r--  2.0 unx     7840 b- defN 23-Aug-07 15:30 fontmake-3.7.1/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/lib.plist
+-rw-r--r--  2.0 unx       42 b- defN 23-Aug-07 15:30 fontmake-3.7.1/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/features.fea
+-rw-r--r--  2.0 unx      252 b- defN 23-Aug-07 15:30 fontmake-3.7.1/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs.background/contents.plist
+-rw-r--r--  2.0 unx      246 b- defN 23-Aug-07 15:30 fontmake-3.7.1/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs.background/layerinfo.plist
+-rw-r--r--  2.0 unx     1988 b- defN 23-Aug-07 15:30 fontmake-3.7.1/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs.background/S_.closed.glif
+-rw-r--r--  2.0 unx      490 b- defN 23-Aug-07 15:30 fontmake-3.7.1/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/arrowup.glif
+-rw-r--r--  2.0 unx      748 b- defN 23-Aug-07 15:30 fontmake-3.7.1/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/Y_.glif
+-rw-r--r--  2.0 unx      744 b- defN 23-Aug-07 15:30 fontmake-3.7.1/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/Z_.glif
+-rw-r--r--  2.0 unx      825 b- defN 23-Aug-07 15:30 fontmake-3.7.1/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/J_.narrow.glif
+-rw-r--r--  2.0 unx      546 b- defN 23-Aug-07 15:30 fontmake-3.7.1/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/T_.glif
+-rw-r--r--  2.0 unx      340 b- defN 23-Aug-07 15:30 fontmake-3.7.1/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/A_acute.glif
+-rw-r--r--  2.0 unx     1785 b- defN 23-Aug-07 15:30 fontmake-3.7.1/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/C_.glif
+-rw-r--r--  2.0 unx      490 b- defN 23-Aug-07 15:30 fontmake-3.7.1/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/arrowleft.glif
+-rw-r--r--  2.0 unx      245 b- defN 23-Aug-07 15:30 fontmake-3.7.1/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/semicolon.glif
+-rw-r--r--  2.0 unx      350 b- defN 23-Aug-07 15:30 fontmake-3.7.1/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/period.glif
+-rw-r--r--  2.0 unx      353 b- defN 23-Aug-07 15:30 fontmake-3.7.1/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/acute.glif
+-rw-r--r--  2.0 unx      542 b- defN 23-Aug-07 15:30 fontmake-3.7.1/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/L_.glif
+-rw-r--r--  2.0 unx     2367 b- defN 23-Aug-07 15:30 fontmake-3.7.1/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/S_.glif
+-rw-r--r--  2.0 unx      566 b- defN 23-Aug-07 15:30 fontmake-3.7.1/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/quotesinglbase.glif
+-rw-r--r--  2.0 unx      264 b- defN 23-Aug-07 15:30 fontmake-3.7.1/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/quotedblright.glif
+-rw-r--r--  2.0 unx     1799 b- defN 23-Aug-07 15:30 fontmake-3.7.1/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/B_.glif
+-rw-r--r--  2.0 unx     1204 b- defN 23-Aug-07 15:30 fontmake-3.7.1/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/P_.glif
+-rw-r--r--  2.0 unx      491 b- defN 23-Aug-07 15:30 fontmake-3.7.1/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/arrowdown.glif
+-rw-r--r--  2.0 unx      858 b- defN 23-Aug-07 15:30 fontmake-3.7.1/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/W_.glif
+-rw-r--r--  2.0 unx      521 b- defN 23-Aug-07 15:30 fontmake-3.7.1/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/comma.glif
+-rw-r--r--  2.0 unx      384 b- defN 23-Aug-07 15:30 fontmake-3.7.1/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/dieresis.glif
+-rw-r--r--  2.0 unx      325 b- defN 23-Aug-07 15:30 fontmake-3.7.1/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/quotedblleft.glif
+-rw-r--r--  2.0 unx      747 b- defN 23-Aug-07 15:30 fontmake-3.7.1/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/F_.glif
+-rw-r--r--  2.0 unx     1359 b- defN 23-Aug-07 15:30 fontmake-3.7.1/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/O_.glif
+-rw-r--r--  2.0 unx      346 b- defN 23-Aug-07 15:30 fontmake-3.7.1/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/A_dieresis.glif
+-rw-r--r--  2.0 unx      608 b- defN 23-Aug-07 15:30 fontmake-3.7.1/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/quotedblbase.glif
+-rw-r--r--  2.0 unx      154 b- defN 23-Aug-07 15:30 fontmake-3.7.1/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/space.glif
+-rw-r--r--  2.0 unx      491 b- defN 23-Aug-07 15:30 fontmake-3.7.1/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/arrowright.glif
+-rw-r--r--  2.0 unx      701 b- defN 23-Aug-07 15:30 fontmake-3.7.1/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/I_.narrow.glif
+-rw-r--r--  2.0 unx     2687 b- defN 23-Aug-07 15:30 fontmake-3.7.1/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/contents.plist
+-rw-r--r--  2.0 unx      743 b- defN 23-Aug-07 15:30 fontmake-3.7.1/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/H_.glif
+-rw-r--r--  2.0 unx      379 b- defN 23-Aug-07 15:30 fontmake-3.7.1/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/Q_.glif
+-rw-r--r--  2.0 unx     1382 b- defN 23-Aug-07 15:30 fontmake-3.7.1/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/E_.glif
+-rw-r--r--  2.0 unx      936 b- defN 23-Aug-07 15:30 fontmake-3.7.1/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/J_.glif
+-rw-r--r--  2.0 unx     1128 b- defN 23-Aug-07 15:30 fontmake-3.7.1/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/D_.glif
+-rw-r--r--  2.0 unx     1774 b- defN 23-Aug-07 15:30 fontmake-3.7.1/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/G_.glif
+-rw-r--r--  2.0 unx      872 b- defN 23-Aug-07 15:30 fontmake-3.7.1/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/K_.glif
+-rw-r--r--  2.0 unx      741 b- defN 23-Aug-07 15:30 fontmake-3.7.1/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/I_.glif
+-rw-r--r--  2.0 unx     1319 b- defN 23-Aug-07 15:30 fontmake-3.7.1/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/A_.glif
+-rw-r--r--  2.0 unx      915 b- defN 23-Aug-07 15:30 fontmake-3.7.1/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/M_.glif
+-rw-r--r--  2.0 unx     1137 b- defN 23-Aug-07 15:30 fontmake-3.7.1/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/I_J_.glif
+-rw-r--r--  2.0 unx      740 b- defN 23-Aug-07 15:30 fontmake-3.7.1/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/V_.glif
+-rw-r--r--  2.0 unx      800 b- defN 23-Aug-07 15:30 fontmake-3.7.1/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/X_.glif
+-rw-r--r--  2.0 unx      371 b- defN 23-Aug-07 15:30 fontmake-3.7.1/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/layerinfo.plist
+-rw-r--r--  2.0 unx      741 b- defN 23-Aug-07 15:30 fontmake-3.7.1/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/N_.glif
+-rw-r--r--  2.0 unx      242 b- defN 23-Aug-07 15:30 fontmake-3.7.1/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/colon.glif
+-rw-r--r--  2.0 unx      351 b- defN 23-Aug-07 15:30 fontmake-3.7.1/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/dot.glif
+-rw-r--r--  2.0 unx     1829 b- defN 23-Aug-07 15:30 fontmake-3.7.1/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/R_.glif
+-rw-r--r--  2.0 unx     2285 b- defN 23-Aug-07 15:30 fontmake-3.7.1/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/S_.closed.glif
+-rw-r--r--  2.0 unx      936 b- defN 23-Aug-07 15:30 fontmake-3.7.1/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/U_.glif
+drwxr-xr-x  2.0 unx        0 b- stor 23-Aug-07 15:30 fontmake-3.7.1/tests/data/MutatorSans/MutatorSansIntermediateCondensed.ufo/glyphs.reference.interpolation/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Aug-07 15:30 fontmake-3.7.1/tests/data/MutatorSans/MutatorSansIntermediateCondensed.ufo/glyphs.background/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Aug-07 15:30 fontmake-3.7.1/tests/data/MutatorSans/MutatorSansIntermediateCondensed.ufo/glyphs/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Aug-07 15:30 fontmake-3.7.1/tests/data/MutatorSans/MutatorSansIntermediateCondensed.ufo/glyphs.interpolation/
+-rw-r--r--  2.0 unx      318 b- defN 23-Aug-07 15:30 fontmake-3.7.1/tests/data/MutatorSans/MutatorSansIntermediateCondensed.ufo/metainfo.plist
+-rw-r--r--  2.0 unx     1386 b- defN 23-Aug-07 15:30 fontmake-3.7.1/tests/data/MutatorSans/MutatorSansIntermediateCondensed.ufo/fontinfo.plist
+-rw-r--r--  2.0 unx      615 b- defN 23-Aug-07 15:30 fontmake-3.7.1/tests/data/MutatorSans/MutatorSansIntermediateCondensed.ufo/layercontents.plist
+-rw-r--r--  2.0 unx    16617 b- defN 23-Aug-07 15:30 fontmake-3.7.1/tests/data/MutatorSans/MutatorSansIntermediateCondensed.ufo/lib.plist
+-rw-r--r--  2.0 unx       68 b- defN 23-Aug-07 15:30 fontmake-3.7.1/tests/data/MutatorSans/MutatorSansIntermediateCondensed.ufo/features.fea
+-rw-r--r--  2.0 unx     3181 b- defN 23-Aug-07 15:30 fontmake-3.7.1/tests/data/MutatorSans/MutatorSansIntermediateCondensed.ufo/glyphs.reference.interpolation/S_.glif
+-rw-r--r--  2.0 unx      268 b- defN 23-Aug-07 15:30 fontmake-3.7.1/tests/data/MutatorSans/MutatorSansIntermediateCondensed.ufo/glyphs.reference.interpolation/contents.plist
+-rw-r--r--  2.0 unx      950 b- defN 23-Aug-07 15:30 fontmake-3.7.1/tests/data/MutatorSans/MutatorSansIntermediateCondensed.ufo/glyphs.reference.interpolation/E_.glif
+-rw-r--r--  2.0 unx      341 b- defN 23-Aug-07 15:30 fontmake-3.7.1/tests/data/MutatorSans/MutatorSansIntermediateCondensed.ufo/glyphs.reference.interpolation/layerinfo.plist
+-rw-r--r--  2.0 unx     2353 b- defN 23-Aug-07 15:30 fontmake-3.7.1/tests/data/MutatorSans/MutatorSansIntermediateCondensed.ufo/glyphs.background/S_.glif
+-rw-r--r--  2.0 unx      228 b- defN 23-Aug-07 15:30 fontmake-3.7.1/tests/data/MutatorSans/MutatorSansIntermediateCondensed.ufo/glyphs.background/contents.plist
+-rw-r--r--  2.0 unx      343 b- defN 23-Aug-07 15:30 fontmake-3.7.1/tests/data/MutatorSans/MutatorSansIntermediateCondensed.ufo/glyphs.background/layerinfo.plist
+-rw-r--r--  2.0 unx     2646 b- defN 23-Aug-07 15:30 fontmake-3.7.1/tests/data/MutatorSans/MutatorSansIntermediateCondensed.ufo/glyphs/S_.glif
+-rw-r--r--  2.0 unx     1806 b- defN 23-Aug-07 15:30 fontmake-3.7.1/tests/data/MutatorSans/MutatorSansIntermediateCondensed.ufo/glyphs/B_.glif
+-rw-r--r--  2.0 unx      923 b- defN 23-Aug-07 15:30 fontmake-3.7.1/tests/data/MutatorSans/MutatorSansIntermediateCondensed.ufo/glyphs/F_.glif
+-rw-r--r--  2.0 unx      422 b- defN 23-Aug-07 15:30 fontmake-3.7.1/tests/data/MutatorSans/MutatorSansIntermediateCondensed.ufo/glyphs/contents.plist
+-rw-r--r--  2.0 unx      983 b- defN 23-Aug-07 15:30 fontmake-3.7.1/tests/data/MutatorSans/MutatorSansIntermediateCondensed.ufo/glyphs/E_.glif
+-rw-r--r--  2.0 unx     2307 b- defN 23-Aug-07 15:30 fontmake-3.7.1/tests/data/MutatorSans/MutatorSansIntermediateCondensed.ufo/glyphs/G_.glif
+-rw-r--r--  2.0 unx      371 b- defN 23-Aug-07 15:30 fontmake-3.7.1/tests/data/MutatorSans/MutatorSansIntermediateCondensed.ufo/glyphs/layerinfo.plist
+-rw-r--r--  2.0 unx      228 b- defN 23-Aug-07 15:30 fontmake-3.7.1/tests/data/MutatorSans/MutatorSansIntermediateCondensed.ufo/glyphs.interpolation/contents.plist
+-rw-r--r--  2.0 unx     1938 b- defN 23-Aug-07 15:30 fontmake-3.7.1/tests/data/MutatorSans/MutatorSansIntermediateCondensed.ufo/glyphs.interpolation/E_.glif
+-rw-r--r--  2.0 unx      344 b- defN 23-Aug-07 15:30 fontmake-3.7.1/tests/data/MutatorSans/MutatorSansIntermediateCondensed.ufo/glyphs.interpolation/layerinfo.plist
+drwxr-xr-x  2.0 unx        0 b- stor 23-Aug-07 15:30 fontmake-3.7.1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs.support.crossbars/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Aug-07 15:30 fontmake-3.7.1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs.support.S_.wide/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Aug-07 15:30 fontmake-3.7.1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs.support.S_.middle/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Aug-07 15:30 fontmake-3.7.1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs.background/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Aug-07 15:30 fontmake-3.7.1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Aug-07 15:30 fontmake-3.7.1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs.support.crossbar/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Aug-07 15:30 fontmake-3.7.1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs.support/
+-rw-r--r--  2.0 unx      318 b- defN 23-Aug-07 15:30 fontmake-3.7.1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/metainfo.plist
+-rw-r--r--  2.0 unx      517 b- defN 23-Aug-07 15:30 fontmake-3.7.1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/kerning.plist
+-rw-r--r--  2.0 unx      491 b- defN 23-Aug-07 15:30 fontmake-3.7.1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/groups.plist
+-rw-r--r--  2.0 unx     1888 b- defN 23-Aug-07 15:30 fontmake-3.7.1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/fontinfo.plist
+-rw-r--r--  2.0 unx      811 b- defN 23-Aug-07 15:30 fontmake-3.7.1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/layercontents.plist
+-rw-r--r--  2.0 unx    18792 b- defN 23-Aug-07 15:30 fontmake-3.7.1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/lib.plist
+-rw-r--r--  2.0 unx       68 b- defN 23-Aug-07 15:30 fontmake-3.7.1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/features.fea
+-rw-r--r--  2.0 unx      238 b- defN 23-Aug-07 15:30 fontmake-3.7.1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs.support.crossbars/contents.plist
+-rw-r--r--  2.0 unx     1176 b- defN 23-Aug-07 15:30 fontmake-3.7.1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs.support.crossbars/E_.glif
+-rw-r--r--  2.0 unx      183 b- defN 23-Aug-07 15:30 fontmake-3.7.1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs.support.crossbars/layerinfo.plist
+-rw-r--r--  2.0 unx     3534 b- defN 23-Aug-07 15:30 fontmake-3.7.1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs.support.S_.wide/S_.glif
+-rw-r--r--  2.0 unx      298 b- defN 23-Aug-07 15:30 fontmake-3.7.1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs.support.S_.wide/contents.plist
+-rw-r--r--  2.0 unx      247 b- defN 23-Aug-07 15:30 fontmake-3.7.1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs.support.S_.wide/layerinfo.plist
+-rw-r--r--  2.0 unx     3543 b- defN 23-Aug-07 15:30 fontmake-3.7.1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs.support.S_.wide/S_.closed.glif
+-rw-r--r--  2.0 unx      252 b- defN 23-Aug-07 15:30 fontmake-3.7.1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs.support.S_.middle/contents.plist
+-rw-r--r--  2.0 unx      246 b- defN 23-Aug-07 15:30 fontmake-3.7.1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs.support.S_.middle/layerinfo.plist
+-rw-r--r--  2.0 unx     2825 b- defN 23-Aug-07 15:30 fontmake-3.7.1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs.support.S_.middle/S_.closed.glif
+-rw-r--r--  2.0 unx     3358 b- defN 23-Aug-07 15:30 fontmake-3.7.1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs.background/S_.glif
+-rw-r--r--  2.0 unx      298 b- defN 23-Aug-07 15:30 fontmake-3.7.1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs.background/contents.plist
+-rw-r--r--  2.0 unx      244 b- defN 23-Aug-07 15:30 fontmake-3.7.1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs.background/layerinfo.plist
+-rw-r--r--  2.0 unx     3998 b- defN 23-Aug-07 15:30 fontmake-3.7.1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs.background/S_.closed.glif
+-rw-r--r--  2.0 unx      626 b- defN 23-Aug-07 15:30 fontmake-3.7.1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/arrowup.glif
+-rw-r--r--  2.0 unx     1120 b- defN 23-Aug-07 15:30 fontmake-3.7.1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/Y_.glif
+-rw-r--r--  2.0 unx      739 b- defN 23-Aug-07 15:30 fontmake-3.7.1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/Z_.glif
+-rw-r--r--  2.0 unx      797 b- defN 23-Aug-07 15:30 fontmake-3.7.1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/J_.narrow.glif
+-rw-r--r--  2.0 unx      546 b- defN 23-Aug-07 15:30 fontmake-3.7.1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/T_.glif
+-rw-r--r--  2.0 unx      352 b- defN 23-Aug-07 15:30 fontmake-3.7.1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/A_acute.glif
+-rw-r--r--  2.0 unx     1402 b- defN 23-Aug-07 15:30 fontmake-3.7.1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/C_.glif
+-rw-r--r--  2.0 unx      690 b- defN 23-Aug-07 15:30 fontmake-3.7.1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/arrowleft.glif
+-rw-r--r--  2.0 unx      233 b- defN 23-Aug-07 15:30 fontmake-3.7.1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/semicolon.glif
+-rw-r--r--  2.0 unx      350 b- defN 23-Aug-07 15:30 fontmake-3.7.1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/period.glif
+-rw-r--r--  2.0 unx      353 b- defN 23-Aug-07 15:30 fontmake-3.7.1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/acute.glif
+-rw-r--r--  2.0 unx      538 b- defN 23-Aug-07 15:30 fontmake-3.7.1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/L_.glif
+-rw-r--r--  2.0 unx     2453 b- defN 23-Aug-07 15:30 fontmake-3.7.1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/S_.glif
+-rw-r--r--  2.0 unx      193 b- defN 23-Aug-07 15:30 fontmake-3.7.1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/quotesinglbase.glif
+-rw-r--r--  2.0 unx      264 b- defN 23-Aug-07 15:30 fontmake-3.7.1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/quotedblright.glif
+-rw-r--r--  2.0 unx     1799 b- defN 23-Aug-07 15:30 fontmake-3.7.1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/B_.glif
+-rw-r--r--  2.0 unx     1146 b- defN 23-Aug-07 15:30 fontmake-3.7.1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/P_.glif
+-rw-r--r--  2.0 unx      628 b- defN 23-Aug-07 15:30 fontmake-3.7.1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/arrowdown.glif
+-rw-r--r--  2.0 unx      853 b- defN 23-Aug-07 15:30 fontmake-3.7.1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/W_.glif
+-rw-r--r--  2.0 unx      515 b- defN 23-Aug-07 15:30 fontmake-3.7.1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/comma.glif
+-rw-r--r--  2.0 unx      369 b- defN 23-Aug-07 15:30 fontmake-3.7.1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/dieresis.glif
+-rw-r--r--  2.0 unx      325 b- defN 23-Aug-07 15:30 fontmake-3.7.1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/quotedblleft.glif
+-rw-r--r--  2.0 unx      743 b- defN 23-Aug-07 15:30 fontmake-3.7.1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/F_.glif
+-rw-r--r--  2.0 unx     1372 b- defN 23-Aug-07 15:30 fontmake-3.7.1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/O_.glif
+-rw-r--r--  2.0 unx      358 b- defN 23-Aug-07 15:30 fontmake-3.7.1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/A_dieresis.glif
+-rw-r--r--  2.0 unx      235 b- defN 23-Aug-07 15:30 fontmake-3.7.1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/quotedblbase.glif
+-rw-r--r--  2.0 unx      154 b- defN 23-Aug-07 15:30 fontmake-3.7.1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/space.glif
+-rw-r--r--  2.0 unx      627 b- defN 23-Aug-07 15:30 fontmake-3.7.1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/arrowright.glif
+-rw-r--r--  2.0 unx      701 b- defN 23-Aug-07 15:30 fontmake-3.7.1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/I_.narrow.glif
+-rw-r--r--  2.0 unx     2687 b- defN 23-Aug-07 15:30 fontmake-3.7.1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/contents.plist
+-rw-r--r--  2.0 unx      741 b- defN 23-Aug-07 15:30 fontmake-3.7.1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/H_.glif
+-rw-r--r--  2.0 unx      377 b- defN 23-Aug-07 15:30 fontmake-3.7.1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/Q_.glif
+-rw-r--r--  2.0 unx      975 b- defN 23-Aug-07 15:30 fontmake-3.7.1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/E_.glif
+-rw-r--r--  2.0 unx      929 b- defN 23-Aug-07 15:30 fontmake-3.7.1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/J_.glif
+-rw-r--r--  2.0 unx     1136 b- defN 23-Aug-07 15:30 fontmake-3.7.1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/D_.glif
+-rw-r--r--  2.0 unx     1728 b- defN 23-Aug-07 15:30 fontmake-3.7.1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/G_.glif
+-rw-r--r--  2.0 unx      870 b- defN 23-Aug-07 15:30 fontmake-3.7.1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/K_.glif
+-rw-r--r--  2.0 unx      739 b- defN 23-Aug-07 15:30 fontmake-3.7.1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/I_.glif
+-rw-r--r--  2.0 unx      942 b- defN 23-Aug-07 15:30 fontmake-3.7.1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/A_.glif
+-rw-r--r--  2.0 unx      914 b- defN 23-Aug-07 15:30 fontmake-3.7.1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/M_.glif
+-rw-r--r--  2.0 unx     1105 b- defN 23-Aug-07 15:30 fontmake-3.7.1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/I_J_.glif
+-rw-r--r--  2.0 unx      737 b- defN 23-Aug-07 15:30 fontmake-3.7.1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/V_.glif
+-rw-r--r--  2.0 unx      798 b- defN 23-Aug-07 15:30 fontmake-3.7.1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/X_.glif
+-rw-r--r--  2.0 unx      371 b- defN 23-Aug-07 15:30 fontmake-3.7.1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/layerinfo.plist
+-rw-r--r--  2.0 unx      736 b- defN 23-Aug-07 15:30 fontmake-3.7.1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/N_.glif
+-rw-r--r--  2.0 unx      230 b- defN 23-Aug-07 15:30 fontmake-3.7.1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/colon.glif
+-rw-r--r--  2.0 unx      349 b- defN 23-Aug-07 15:30 fontmake-3.7.1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/dot.glif
+-rw-r--r--  2.0 unx     1462 b- defN 23-Aug-07 15:30 fontmake-3.7.1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/R_.glif
+-rw-r--r--  2.0 unx     1966 b- defN 23-Aug-07 15:30 fontmake-3.7.1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/S_.closed.glif
+-rw-r--r--  2.0 unx      929 b- defN 23-Aug-07 15:30 fontmake-3.7.1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/U_.glif
+-rw-r--r--  2.0 unx     3498 b- defN 23-Aug-07 15:30 fontmake-3.7.1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs.support.crossbar/S_.glif
+-rw-r--r--  2.0 unx     2111 b- defN 23-Aug-07 15:30 fontmake-3.7.1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs.support.crossbar/B_.glif
+-rw-r--r--  2.0 unx      751 b- defN 23-Aug-07 15:30 fontmake-3.7.1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs.support.crossbar/F_.glif
+-rw-r--r--  2.0 unx      482 b- defN 23-Aug-07 15:30 fontmake-3.7.1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs.support.crossbar/contents.plist
+-rw-r--r--  2.0 unx     1471 b- defN 23-Aug-07 15:30 fontmake-3.7.1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs.support.crossbar/E_.glif
+-rw-r--r--  2.0 unx     2452 b- defN 23-Aug-07 15:30 fontmake-3.7.1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs.support.crossbar/G_.glif
+-rw-r--r--  2.0 unx      247 b- defN 23-Aug-07 15:30 fontmake-3.7.1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs.support.crossbar/layerinfo.plist
+-rw-r--r--  2.0 unx      422 b- defN 23-Aug-07 15:30 fontmake-3.7.1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs.support.crossbar/S_.closed.glif
+-rw-r--r--  2.0 unx     2706 b- defN 23-Aug-07 15:30 fontmake-3.7.1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs.support/S_.glif
+-rw-r--r--  2.0 unx      853 b- defN 23-Aug-07 15:30 fontmake-3.7.1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs.support/W_.glif
+-rw-r--r--  2.0 unx      330 b- defN 23-Aug-07 15:30 fontmake-3.7.1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs.support/contents.plist
+-rw-r--r--  2.0 unx      828 b- defN 23-Aug-07 15:30 fontmake-3.7.1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs.support/A_.glif
+-rw-r--r--  2.0 unx      371 b- defN 23-Aug-07 15:30 fontmake-3.7.1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs.support/layerinfo.plist
+drwxr-xr-x  2.0 unx        0 b- stor 23-Aug-07 15:30 fontmake-3.7.1/tests/data/MutatorSans/MutatorSansIntermediateWide.ufo/glyphs.background/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Aug-07 15:30 fontmake-3.7.1/tests/data/MutatorSans/MutatorSansIntermediateWide.ufo/glyphs/
+-rw-r--r--  2.0 unx      318 b- defN 23-Aug-07 15:30 fontmake-3.7.1/tests/data/MutatorSans/MutatorSansIntermediateWide.ufo/metainfo.plist
+-rw-r--r--  2.0 unx     5462 b- defN 23-Aug-07 15:30 fontmake-3.7.1/tests/data/MutatorSans/MutatorSansIntermediateWide.ufo/kerning.plist
+-rw-r--r--  2.0 unx     1384 b- defN 23-Aug-07 15:30 fontmake-3.7.1/tests/data/MutatorSans/MutatorSansIntermediateWide.ufo/fontinfo.plist
+-rw-r--r--  2.0 unx      383 b- defN 23-Aug-07 15:30 fontmake-3.7.1/tests/data/MutatorSans/MutatorSansIntermediateWide.ufo/layercontents.plist
+-rw-r--r--  2.0 unx    16223 b- defN 23-Aug-07 15:30 fontmake-3.7.1/tests/data/MutatorSans/MutatorSansIntermediateWide.ufo/lib.plist
+-rw-r--r--  2.0 unx       68 b- defN 23-Aug-07 15:30 fontmake-3.7.1/tests/data/MutatorSans/MutatorSansIntermediateWide.ufo/features.fea
+-rw-r--r--  2.0 unx     2396 b- defN 23-Aug-07 15:30 fontmake-3.7.1/tests/data/MutatorSans/MutatorSansIntermediateWide.ufo/glyphs.background/S_.glif
+-rw-r--r--  2.0 unx      228 b- defN 23-Aug-07 15:30 fontmake-3.7.1/tests/data/MutatorSans/MutatorSansIntermediateWide.ufo/glyphs.background/contents.plist
+-rw-r--r--  2.0 unx      343 b- defN 23-Aug-07 15:30 fontmake-3.7.1/tests/data/MutatorSans/MutatorSansIntermediateWide.ufo/glyphs.background/layerinfo.plist
+-rw-r--r--  2.0 unx     1824 b- defN 23-Aug-07 15:30 fontmake-3.7.1/tests/data/MutatorSans/MutatorSansIntermediateWide.ufo/glyphs/B_.glif
+-rw-r--r--  2.0 unx      911 b- defN 23-Aug-07 15:30 fontmake-3.7.1/tests/data/MutatorSans/MutatorSansIntermediateWide.ufo/glyphs/F_.glif
+-rw-r--r--  2.0 unx      376 b- defN 23-Aug-07 15:30 fontmake-3.7.1/tests/data/MutatorSans/MutatorSansIntermediateWide.ufo/glyphs/contents.plist
+-rw-r--r--  2.0 unx     1162 b- defN 23-Aug-07 15:30 fontmake-3.7.1/tests/data/MutatorSans/MutatorSansIntermediateWide.ufo/glyphs/E_.glif
+-rw-r--r--  2.0 unx     2148 b- defN 23-Aug-07 15:30 fontmake-3.7.1/tests/data/MutatorSans/MutatorSansIntermediateWide.ufo/glyphs/G_.glif
+-rw-r--r--  2.0 unx      371 b- defN 23-Aug-07 15:30 fontmake-3.7.1/tests/data/MutatorSans/MutatorSansIntermediateWide.ufo/glyphs/layerinfo.plist
+-rw-r--r--  2.0 unx   125360 b- defN 23-Aug-07 15:30 fontmake-3.7.1/tests/data/AutohintingTest/Padyakke.glyphs
+726 files, 1215342 bytes uncompressed, 299663 bytes compressed:  75.3%
```

## zipnote {}

```diff
@@ -1,2179 +1,2179 @@
-Filename: fontmake-3.7.0b3/
+Filename: fontmake-3.7.1/
 Comment: 
 
-Filename: fontmake-3.7.0b3/Lib/
+Filename: fontmake-3.7.1/.github/
 Comment: 
 
-Filename: fontmake-3.7.0b3/.github/
+Filename: fontmake-3.7.1/Lib/
 Comment: 
 
-Filename: fontmake-3.7.0b3/tests/
+Filename: fontmake-3.7.1/tests/
 Comment: 
 
-Filename: fontmake-3.7.0b3/requirements.txt
+Filename: fontmake-3.7.1/.editorconfig
 Comment: 
 
-Filename: fontmake-3.7.0b3/setup.cfg
+Filename: fontmake-3.7.1/LICENSE
 Comment: 
 
-Filename: fontmake-3.7.0b3/build_pyz.sh
+Filename: fontmake-3.7.1/tox.ini
 Comment: 
 
-Filename: fontmake-3.7.0b3/PKG-INFO
+Filename: fontmake-3.7.1/pyproject.toml
 Comment: 
 
-Filename: fontmake-3.7.0b3/TROUBLESHOOTING.md
+Filename: fontmake-3.7.1/.gitignore
 Comment: 
 
-Filename: fontmake-3.7.0b3/.gitignore
+Filename: fontmake-3.7.1/setup.cfg
 Comment: 
 
-Filename: fontmake-3.7.0b3/test_requirements.txt
+Filename: fontmake-3.7.1/build_pyz.sh
 Comment: 
 
-Filename: fontmake-3.7.0b3/MANIFEST.in
+Filename: fontmake-3.7.1/CONTRIBUTING.md
 Comment: 
 
-Filename: fontmake-3.7.0b3/LICENSE
+Filename: fontmake-3.7.1/MANIFEST.in
 Comment: 
 
-Filename: fontmake-3.7.0b3/USAGE.md
+Filename: fontmake-3.7.1/requirements.txt
 Comment: 
 
-Filename: fontmake-3.7.0b3/README.md
+Filename: fontmake-3.7.1/.gitattributes
 Comment: 
 
-Filename: fontmake-3.7.0b3/setup.py
+Filename: fontmake-3.7.1/setup.py
 Comment: 
 
-Filename: fontmake-3.7.0b3/pyproject.toml
+Filename: fontmake-3.7.1/TROUBLESHOOTING.md
 Comment: 
 
-Filename: fontmake-3.7.0b3/tox.ini
+Filename: fontmake-3.7.1/test_requirements.txt
 Comment: 
 
-Filename: fontmake-3.7.0b3/.coveragerc
+Filename: fontmake-3.7.1/README.md
 Comment: 
 
-Filename: fontmake-3.7.0b3/CONTRIBUTING.md
+Filename: fontmake-3.7.1/.pyup.yml
 Comment: 
 
-Filename: fontmake-3.7.0b3/.codecov.yml
+Filename: fontmake-3.7.1/PKG-INFO
 Comment: 
 
-Filename: fontmake-3.7.0b3/.editorconfig
+Filename: fontmake-3.7.1/.coveragerc
 Comment: 
 
-Filename: fontmake-3.7.0b3/.gitattributes
+Filename: fontmake-3.7.1/USAGE.md
 Comment: 
 
-Filename: fontmake-3.7.0b3/.pyup.yml
+Filename: fontmake-3.7.1/.codecov.yml
 Comment: 
 
-Filename: fontmake-3.7.0b3/Lib/fontmake/
+Filename: fontmake-3.7.1/.github/workflows/
 Comment: 
 
-Filename: fontmake-3.7.0b3/Lib/fontmake.egg-info/
+Filename: fontmake-3.7.1/.github/workflows/ci.yml
 Comment: 
 
-Filename: fontmake-3.7.0b3/Lib/fontmake/compatibility.py
+Filename: fontmake-3.7.1/Lib/fontmake.egg-info/
 Comment: 
 
-Filename: fontmake-3.7.0b3/Lib/fontmake/instantiator.py
+Filename: fontmake-3.7.1/Lib/fontmake/
 Comment: 
 
-Filename: fontmake-3.7.0b3/Lib/fontmake/errors.py
+Filename: fontmake-3.7.1/Lib/fontmake.egg-info/entry_points.txt
 Comment: 
 
-Filename: fontmake-3.7.0b3/Lib/fontmake/ttfautohint.py
+Filename: fontmake-3.7.1/Lib/fontmake.egg-info/top_level.txt
 Comment: 
 
-Filename: fontmake-3.7.0b3/Lib/fontmake/font_project.py
+Filename: fontmake-3.7.1/Lib/fontmake.egg-info/SOURCES.txt
 Comment: 
 
-Filename: fontmake-3.7.0b3/Lib/fontmake/_version.py
+Filename: fontmake-3.7.1/Lib/fontmake.egg-info/dependency_links.txt
 Comment: 
 
-Filename: fontmake-3.7.0b3/Lib/fontmake/__init__.py
+Filename: fontmake-3.7.1/Lib/fontmake.egg-info/requires.txt
 Comment: 
 
-Filename: fontmake-3.7.0b3/Lib/fontmake/__main__.py
+Filename: fontmake-3.7.1/Lib/fontmake.egg-info/PKG-INFO
 Comment: 
 
-Filename: fontmake-3.7.0b3/Lib/fontmake.egg-info/PKG-INFO
+Filename: fontmake-3.7.1/Lib/fontmake/font_project.py
 Comment: 
 
-Filename: fontmake-3.7.0b3/Lib/fontmake.egg-info/top_level.txt
+Filename: fontmake-3.7.1/Lib/fontmake/compatibility.py
 Comment: 
 
-Filename: fontmake-3.7.0b3/Lib/fontmake.egg-info/SOURCES.txt
+Filename: fontmake-3.7.1/Lib/fontmake/_version.py
 Comment: 
 
-Filename: fontmake-3.7.0b3/Lib/fontmake.egg-info/requires.txt
+Filename: fontmake-3.7.1/Lib/fontmake/__main__.py
 Comment: 
 
-Filename: fontmake-3.7.0b3/Lib/fontmake.egg-info/dependency_links.txt
+Filename: fontmake-3.7.1/Lib/fontmake/ttfautohint.py
 Comment: 
 
-Filename: fontmake-3.7.0b3/Lib/fontmake.egg-info/entry_points.txt
+Filename: fontmake-3.7.1/Lib/fontmake/instantiator.py
 Comment: 
 
-Filename: fontmake-3.7.0b3/.github/workflows/
+Filename: fontmake-3.7.1/Lib/fontmake/errors.py
 Comment: 
 
-Filename: fontmake-3.7.0b3/.github/workflows/ci.yml
+Filename: fontmake-3.7.1/Lib/fontmake/__init__.py
 Comment: 
 
-Filename: fontmake-3.7.0b3/tests/data/
+Filename: fontmake-3.7.1/tests/data/
 Comment: 
 
-Filename: fontmake-3.7.0b3/tests/conftest.py
+Filename: fontmake-3.7.1/tests/conftest.py
 Comment: 
 
-Filename: fontmake-3.7.0b3/tests/test_instantiator.py
+Filename: fontmake-3.7.1/tests/test_instantiator.py
 Comment: 
 
-Filename: fontmake-3.7.0b3/tests/test_main.py
+Filename: fontmake-3.7.1/tests/test_compatibility.py
 Comment: 
 
-Filename: fontmake-3.7.0b3/tests/test_compatibility.py
+Filename: fontmake-3.7.1/tests/test_main.py
 Comment: 
 
-Filename: fontmake-3.7.0b3/tests/data/DesignspaceRuleOrder/
+Filename: fontmake-3.7.1/tests/data/IncompatibleSans/
 Comment: 
 
-Filename: fontmake-3.7.0b3/tests/data/SwapGlyphNames/
+Filename: fontmake-3.7.1/tests/data/DesignspaceTestSharedFeatures/
 Comment: 
 
-Filename: fontmake-3.7.0b3/tests/data/GlyphsUnitTestSans3.glyphspackage/
+Filename: fontmake-3.7.1/tests/data/InterpolateLayoutTest/
 Comment: 
 
-Filename: fontmake-3.7.0b3/tests/data/DesignspaceTest/
+Filename: fontmake-3.7.1/tests/data/DesignspaceRuleOrder/
 Comment: 
 
-Filename: fontmake-3.7.0b3/tests/data/InstantiatorStrictMathGlyph/
+Filename: fontmake-3.7.1/tests/data/GlyphsUnitTestSans3.glyphspackage/
 Comment: 
 
-Filename: fontmake-3.7.0b3/tests/data/DesignspaceBrokenTest/
+Filename: fontmake-3.7.1/tests/data/SwapGlyphNames/
 Comment: 
 
-Filename: fontmake-3.7.0b3/tests/data/InterpolateLayoutTest/
+Filename: fontmake-3.7.1/tests/data/DesignspaceBrokenTest/
 Comment: 
 
-Filename: fontmake-3.7.0b3/tests/data/AutohintingTest/
+Filename: fontmake-3.7.1/tests/data/DesignspaceTest/
 Comment: 
 
-Filename: fontmake-3.7.0b3/tests/data/IncompatibleSans/
+Filename: fontmake-3.7.1/tests/data/MutatorSansLite/
 Comment: 
 
-Filename: fontmake-3.7.0b3/tests/data/DesignspaceTestSharedFeatures/
+Filename: fontmake-3.7.1/tests/data/InstantiatorStrictMathGlyph/
 Comment: 
 
-Filename: fontmake-3.7.0b3/tests/data/MutatorSans/
+Filename: fontmake-3.7.1/tests/data/MutatorSans/
 Comment: 
 
-Filename: fontmake-3.7.0b3/tests/data/MutatorSansLite/
+Filename: fontmake-3.7.1/tests/data/AutohintingTest/
 Comment: 
 
-Filename: fontmake-3.7.0b3/tests/data/TestSubset.glyphs
+Filename: fontmake-3.7.1/tests/data/TestSubset.glyphs
 Comment: 
 
-Filename: fontmake-3.7.0b3/tests/data/GlyphData.xml
+Filename: fontmake-3.7.1/tests/data/TestSubset2.glyphs
 Comment: 
 
-Filename: fontmake-3.7.0b3/tests/data/TestSubset2.glyphs
+Filename: fontmake-3.7.1/tests/data/GlyphsUnitTestSans.glyphs
 Comment: 
 
-Filename: fontmake-3.7.0b3/tests/data/GlyphsUnitTestSans.glyphs
+Filename: fontmake-3.7.1/tests/data/GlyphData.xml
 Comment: 
 
-Filename: fontmake-3.7.0b3/tests/data/DesignspaceRuleOrder/MyFont_Black.ufo/
+Filename: fontmake-3.7.1/tests/data/IncompatibleSans/IncompatibleSans-Regular.ufo/
 Comment: 
 
-Filename: fontmake-3.7.0b3/tests/data/DesignspaceRuleOrder/MyFont_Hair.ufo/
+Filename: fontmake-3.7.1/tests/data/IncompatibleSans/IncompatibleSans-Bold.ufo/
 Comment: 
 
-Filename: fontmake-3.7.0b3/tests/data/DesignspaceRuleOrder/MyFont.designspace
+Filename: fontmake-3.7.1/tests/data/IncompatibleSans/IncompatibleSans.designspace
 Comment: 
 
-Filename: fontmake-3.7.0b3/tests/data/DesignspaceRuleOrder/MyFont_Black.ufo/glyphs/
+Filename: fontmake-3.7.1/tests/data/IncompatibleSans/IncompatibleSans-Regular.ufo/glyphs/
 Comment: 
 
-Filename: fontmake-3.7.0b3/tests/data/DesignspaceRuleOrder/MyFont_Black.ufo/layercontents.plist
+Filename: fontmake-3.7.1/tests/data/IncompatibleSans/IncompatibleSans-Regular.ufo/metainfo.plist
 Comment: 
 
-Filename: fontmake-3.7.0b3/tests/data/DesignspaceRuleOrder/MyFont_Black.ufo/fontinfo.plist
+Filename: fontmake-3.7.1/tests/data/IncompatibleSans/IncompatibleSans-Regular.ufo/fontinfo.plist
 Comment: 
 
-Filename: fontmake-3.7.0b3/tests/data/DesignspaceRuleOrder/MyFont_Black.ufo/metainfo.plist
+Filename: fontmake-3.7.1/tests/data/IncompatibleSans/IncompatibleSans-Regular.ufo/layercontents.plist
 Comment: 
 
-Filename: fontmake-3.7.0b3/tests/data/DesignspaceRuleOrder/MyFont_Black.ufo/lib.plist
+Filename: fontmake-3.7.1/tests/data/IncompatibleSans/IncompatibleSans-Regular.ufo/lib.plist
 Comment: 
 
-Filename: fontmake-3.7.0b3/tests/data/DesignspaceRuleOrder/MyFont_Black.ufo/glyphs/Q_.alt.glif
+Filename: fontmake-3.7.1/tests/data/IncompatibleSans/IncompatibleSans-Regular.ufo/glyphs/C_.glif
 Comment: 
 
-Filename: fontmake-3.7.0b3/tests/data/DesignspaceRuleOrder/MyFont_Black.ufo/glyphs/contents.plist
+Filename: fontmake-3.7.1/tests/data/IncompatibleSans/IncompatibleSans-Regular.ufo/glyphs/B_.glif
 Comment: 
 
-Filename: fontmake-3.7.0b3/tests/data/DesignspaceRuleOrder/MyFont_Black.ufo/glyphs/Q_.glif
+Filename: fontmake-3.7.1/tests/data/IncompatibleSans/IncompatibleSans-Regular.ufo/glyphs/space.glif
 Comment: 
 
-Filename: fontmake-3.7.0b3/tests/data/DesignspaceRuleOrder/MyFont_Black.ufo/glyphs/Q_.ss01.glif
+Filename: fontmake-3.7.1/tests/data/IncompatibleSans/IncompatibleSans-Regular.ufo/glyphs/contents.plist
 Comment: 
 
-Filename: fontmake-3.7.0b3/tests/data/DesignspaceRuleOrder/MyFont_Black.ufo/glyphs/Q_.ss01.alt.glif
+Filename: fontmake-3.7.1/tests/data/IncompatibleSans/IncompatibleSans-Regular.ufo/glyphs/D_.glif
 Comment: 
 
-Filename: fontmake-3.7.0b3/tests/data/DesignspaceRuleOrder/MyFont_Hair.ufo/glyphs/
+Filename: fontmake-3.7.1/tests/data/IncompatibleSans/IncompatibleSans-Regular.ufo/glyphs/A_.glif
 Comment: 
 
-Filename: fontmake-3.7.0b3/tests/data/DesignspaceRuleOrder/MyFont_Hair.ufo/layercontents.plist
+Filename: fontmake-3.7.1/tests/data/IncompatibleSans/IncompatibleSans-Bold.ufo/glyphs/
 Comment: 
 
-Filename: fontmake-3.7.0b3/tests/data/DesignspaceRuleOrder/MyFont_Hair.ufo/fontinfo.plist
+Filename: fontmake-3.7.1/tests/data/IncompatibleSans/IncompatibleSans-Bold.ufo/metainfo.plist
 Comment: 
 
-Filename: fontmake-3.7.0b3/tests/data/DesignspaceRuleOrder/MyFont_Hair.ufo/metainfo.plist
+Filename: fontmake-3.7.1/tests/data/IncompatibleSans/IncompatibleSans-Bold.ufo/fontinfo.plist
 Comment: 
 
-Filename: fontmake-3.7.0b3/tests/data/DesignspaceRuleOrder/MyFont_Hair.ufo/lib.plist
+Filename: fontmake-3.7.1/tests/data/IncompatibleSans/IncompatibleSans-Bold.ufo/layercontents.plist
 Comment: 
 
-Filename: fontmake-3.7.0b3/tests/data/DesignspaceRuleOrder/MyFont_Hair.ufo/glyphs/Q_.alt.glif
+Filename: fontmake-3.7.1/tests/data/IncompatibleSans/IncompatibleSans-Bold.ufo/lib.plist
 Comment: 
 
-Filename: fontmake-3.7.0b3/tests/data/DesignspaceRuleOrder/MyFont_Hair.ufo/glyphs/contents.plist
+Filename: fontmake-3.7.1/tests/data/IncompatibleSans/IncompatibleSans-Bold.ufo/features.fea
 Comment: 
 
-Filename: fontmake-3.7.0b3/tests/data/DesignspaceRuleOrder/MyFont_Hair.ufo/glyphs/Q_.glif
+Filename: fontmake-3.7.1/tests/data/IncompatibleSans/IncompatibleSans-Bold.ufo/glyphs/C_.glif
 Comment: 
 
-Filename: fontmake-3.7.0b3/tests/data/DesignspaceRuleOrder/MyFont_Hair.ufo/glyphs/Q_.ss01.glif
+Filename: fontmake-3.7.1/tests/data/IncompatibleSans/IncompatibleSans-Bold.ufo/glyphs/B_.glif
 Comment: 
 
-Filename: fontmake-3.7.0b3/tests/data/DesignspaceRuleOrder/MyFont_Hair.ufo/glyphs/Q_.ss01.alt.glif
+Filename: fontmake-3.7.1/tests/data/IncompatibleSans/IncompatibleSans-Bold.ufo/glyphs/space.glif
 Comment: 
 
-Filename: fontmake-3.7.0b3/tests/data/SwapGlyphNames/A.ufo/
+Filename: fontmake-3.7.1/tests/data/IncompatibleSans/IncompatibleSans-Bold.ufo/glyphs/contents.plist
 Comment: 
 
-Filename: fontmake-3.7.0b3/tests/data/SwapGlyphNames/B.ufo/
+Filename: fontmake-3.7.1/tests/data/IncompatibleSans/IncompatibleSans-Bold.ufo/glyphs/D_.glif
 Comment: 
 
-Filename: fontmake-3.7.0b3/tests/data/SwapGlyphNames/A.ufo/glyphs/
+Filename: fontmake-3.7.1/tests/data/IncompatibleSans/IncompatibleSans-Bold.ufo/glyphs/A_.glif
 Comment: 
 
-Filename: fontmake-3.7.0b3/tests/data/SwapGlyphNames/A.ufo/layercontents.plist
+Filename: fontmake-3.7.1/tests/data/DesignspaceTestSharedFeatures/DesignspaceTest-Light.ufo/
 Comment: 
 
-Filename: fontmake-3.7.0b3/tests/data/SwapGlyphNames/A.ufo/groups.plist
+Filename: fontmake-3.7.1/tests/data/DesignspaceTestSharedFeatures/DesignspaceTest-Regular.ufo/
 Comment: 
 
-Filename: fontmake-3.7.0b3/tests/data/SwapGlyphNames/A.ufo/kerning.plist
+Filename: fontmake-3.7.1/tests/data/DesignspaceTestSharedFeatures/DesignspaceTestSharedFeatures.designspace
 Comment: 
 
-Filename: fontmake-3.7.0b3/tests/data/SwapGlyphNames/A.ufo/fontinfo.plist
+Filename: fontmake-3.7.1/tests/data/DesignspaceTestSharedFeatures/family.fea
 Comment: 
 
-Filename: fontmake-3.7.0b3/tests/data/SwapGlyphNames/A.ufo/metainfo.plist
+Filename: fontmake-3.7.1/tests/data/DesignspaceTestSharedFeatures/DesignspaceTest-Light.ufo/glyphs/
 Comment: 
 
-Filename: fontmake-3.7.0b3/tests/data/SwapGlyphNames/A.ufo/lib.plist
+Filename: fontmake-3.7.1/tests/data/DesignspaceTestSharedFeatures/DesignspaceTest-Light.ufo/metainfo.plist
 Comment: 
 
-Filename: fontmake-3.7.0b3/tests/data/SwapGlyphNames/A.ufo/glyphs/aaa.glif
+Filename: fontmake-3.7.1/tests/data/DesignspaceTestSharedFeatures/DesignspaceTest-Light.ufo/fontinfo.plist
 Comment: 
 
-Filename: fontmake-3.7.0b3/tests/data/SwapGlyphNames/A.ufo/glyphs/y.glif
+Filename: fontmake-3.7.1/tests/data/DesignspaceTestSharedFeatures/DesignspaceTest-Light.ufo/layercontents.plist
 Comment: 
 
-Filename: fontmake-3.7.0b3/tests/data/SwapGlyphNames/A.ufo/glyphs/aaa.swap.glif
+Filename: fontmake-3.7.1/tests/data/DesignspaceTestSharedFeatures/DesignspaceTest-Light.ufo/glyphs/contents.plist
 Comment: 
 
-Filename: fontmake-3.7.0b3/tests/data/SwapGlyphNames/A.ufo/glyphs/a.swap.glif
+Filename: fontmake-3.7.1/tests/data/DesignspaceTestSharedFeatures/DesignspaceTest-Regular.ufo/glyphs/
 Comment: 
 
-Filename: fontmake-3.7.0b3/tests/data/SwapGlyphNames/A.ufo/glyphs/a.glif
+Filename: fontmake-3.7.1/tests/data/DesignspaceTestSharedFeatures/DesignspaceTest-Regular.ufo/metainfo.plist
 Comment: 
 
-Filename: fontmake-3.7.0b3/tests/data/SwapGlyphNames/A.ufo/glyphs/contents.plist
+Filename: fontmake-3.7.1/tests/data/DesignspaceTestSharedFeatures/DesignspaceTest-Regular.ufo/fontinfo.plist
 Comment: 
 
-Filename: fontmake-3.7.0b3/tests/data/SwapGlyphNames/A.ufo/glyphs/space.glif
+Filename: fontmake-3.7.1/tests/data/DesignspaceTestSharedFeatures/DesignspaceTest-Regular.ufo/layercontents.plist
 Comment: 
 
-Filename: fontmake-3.7.0b3/tests/data/SwapGlyphNames/A.ufo/glyphs/x.glif
+Filename: fontmake-3.7.1/tests/data/DesignspaceTestSharedFeatures/DesignspaceTest-Regular.ufo/features.fea
 Comment: 
 
-Filename: fontmake-3.7.0b3/tests/data/SwapGlyphNames/B.ufo/glyphs/
+Filename: fontmake-3.7.1/tests/data/DesignspaceTestSharedFeatures/DesignspaceTest-Regular.ufo/glyphs/contents.plist
 Comment: 
 
-Filename: fontmake-3.7.0b3/tests/data/SwapGlyphNames/B.ufo/layercontents.plist
+Filename: fontmake-3.7.1/tests/data/InterpolateLayoutTest/InterpolateLayoutTest 1000 GPOS.txt
 Comment: 
 
-Filename: fontmake-3.7.0b3/tests/data/SwapGlyphNames/B.ufo/fontinfo.plist
+Filename: fontmake-3.7.1/tests/data/InterpolateLayoutTest/InterpolateLayoutTest GSUB.txt
 Comment: 
 
-Filename: fontmake-3.7.0b3/tests/data/SwapGlyphNames/B.ufo/metainfo.plist
+Filename: fontmake-3.7.1/tests/data/InterpolateLayoutTest/InterpolateLayoutTest GDEF.txt
 Comment: 
 
-Filename: fontmake-3.7.0b3/tests/data/SwapGlyphNames/B.ufo/lib.plist
+Filename: fontmake-3.7.1/tests/data/InterpolateLayoutTest/InterpolateLayoutTest.glyphs
 Comment: 
 
-Filename: fontmake-3.7.0b3/tests/data/SwapGlyphNames/B.ufo/glyphs/a.glif
+Filename: fontmake-3.7.1/tests/data/InterpolateLayoutTest/InterpolateLayoutTest 0 GPOS.txt
 Comment: 
 
-Filename: fontmake-3.7.0b3/tests/data/SwapGlyphNames/B.ufo/glyphs/contents.plist
+Filename: fontmake-3.7.1/tests/data/InterpolateLayoutTest/InterpolateLayoutTest.plist
 Comment: 
 
-Filename: fontmake-3.7.0b3/tests/data/SwapGlyphNames/B.ufo/glyphs/dieresiscomb.glif
+Filename: fontmake-3.7.1/tests/data/DesignspaceRuleOrder/MyFont_Black.ufo/
 Comment: 
 
-Filename: fontmake-3.7.0b3/tests/data/SwapGlyphNames/B.ufo/glyphs/adieresis.alt.glif
+Filename: fontmake-3.7.1/tests/data/DesignspaceRuleOrder/MyFont_Hair.ufo/
 Comment: 
 
-Filename: fontmake-3.7.0b3/tests/data/SwapGlyphNames/B.ufo/glyphs/a.alt.glif
+Filename: fontmake-3.7.1/tests/data/DesignspaceRuleOrder/MyFont.designspace
 Comment: 
 
-Filename: fontmake-3.7.0b3/tests/data/SwapGlyphNames/B.ufo/glyphs/adieresis.glif
+Filename: fontmake-3.7.1/tests/data/DesignspaceRuleOrder/MyFont_Black.ufo/glyphs/
 Comment: 
 
-Filename: fontmake-3.7.0b3/tests/data/GlyphsUnitTestSans3.glyphspackage/glyphs/
+Filename: fontmake-3.7.1/tests/data/DesignspaceRuleOrder/MyFont_Black.ufo/metainfo.plist
 Comment: 
 
-Filename: fontmake-3.7.0b3/tests/data/GlyphsUnitTestSans3.glyphspackage/fontinfo.plist
+Filename: fontmake-3.7.1/tests/data/DesignspaceRuleOrder/MyFont_Black.ufo/fontinfo.plist
 Comment: 
 
-Filename: fontmake-3.7.0b3/tests/data/GlyphsUnitTestSans3.glyphspackage/order.plist
+Filename: fontmake-3.7.1/tests/data/DesignspaceRuleOrder/MyFont_Black.ufo/layercontents.plist
 Comment: 
 
-Filename: fontmake-3.7.0b3/tests/data/GlyphsUnitTestSans3.glyphspackage/glyphs/a.sc.glyph
+Filename: fontmake-3.7.1/tests/data/DesignspaceRuleOrder/MyFont_Black.ufo/lib.plist
 Comment: 
 
-Filename: fontmake-3.7.0b3/tests/data/GlyphsUnitTestSans3.glyphspackage/glyphs/A_dieresis.glyph
+Filename: fontmake-3.7.1/tests/data/DesignspaceRuleOrder/MyFont_Black.ufo/glyphs/Q_.ss01.alt.glif
 Comment: 
 
-Filename: fontmake-3.7.0b3/tests/data/GlyphsUnitTestSans3.glyphspackage/glyphs/n.glyph
+Filename: fontmake-3.7.1/tests/data/DesignspaceRuleOrder/MyFont_Black.ufo/glyphs/contents.plist
 Comment: 
 
-Filename: fontmake-3.7.0b3/tests/data/GlyphsUnitTestSans3.glyphspackage/glyphs/h.glyph
+Filename: fontmake-3.7.1/tests/data/DesignspaceRuleOrder/MyFont_Black.ufo/glyphs/Q_.glif
 Comment: 
 
-Filename: fontmake-3.7.0b3/tests/data/GlyphsUnitTestSans3.glyphspackage/glyphs/m.glyph
+Filename: fontmake-3.7.1/tests/data/DesignspaceRuleOrder/MyFont_Black.ufo/glyphs/Q_.alt.glif
 Comment: 
 
-Filename: fontmake-3.7.0b3/tests/data/GlyphsUnitTestSans3.glyphspackage/glyphs/A_.glyph
+Filename: fontmake-3.7.1/tests/data/DesignspaceRuleOrder/MyFont_Black.ufo/glyphs/Q_.ss01.glif
 Comment: 
 
-Filename: fontmake-3.7.0b3/tests/data/GlyphsUnitTestSans3.glyphspackage/glyphs/dieresis.glyph
+Filename: fontmake-3.7.1/tests/data/DesignspaceRuleOrder/MyFont_Hair.ufo/glyphs/
 Comment: 
 
-Filename: fontmake-3.7.0b3/tests/data/GlyphsUnitTestSans3.glyphspackage/glyphs/adieresis.glyph
+Filename: fontmake-3.7.1/tests/data/DesignspaceRuleOrder/MyFont_Hair.ufo/metainfo.plist
 Comment: 
 
-Filename: fontmake-3.7.0b3/tests/data/GlyphsUnitTestSans3.glyphspackage/glyphs/_part.shoulder.glyph
+Filename: fontmake-3.7.1/tests/data/DesignspaceRuleOrder/MyFont_Hair.ufo/fontinfo.plist
 Comment: 
 
-Filename: fontmake-3.7.0b3/tests/data/GlyphsUnitTestSans3.glyphspackage/glyphs/a.glyph
+Filename: fontmake-3.7.1/tests/data/DesignspaceRuleOrder/MyFont_Hair.ufo/layercontents.plist
 Comment: 
 
-Filename: fontmake-3.7.0b3/tests/data/GlyphsUnitTestSans3.glyphspackage/glyphs/_part.stem.glyph
+Filename: fontmake-3.7.1/tests/data/DesignspaceRuleOrder/MyFont_Hair.ufo/lib.plist
 Comment: 
 
-Filename: fontmake-3.7.0b3/tests/data/DesignspaceTest/MyFont-Light.ufo/
+Filename: fontmake-3.7.1/tests/data/DesignspaceRuleOrder/MyFont_Hair.ufo/glyphs/Q_.ss01.alt.glif
 Comment: 
 
-Filename: fontmake-3.7.0b3/tests/data/DesignspaceTest/MyFont-Bold.ufo/
+Filename: fontmake-3.7.1/tests/data/DesignspaceRuleOrder/MyFont_Hair.ufo/glyphs/contents.plist
 Comment: 
 
-Filename: fontmake-3.7.0b3/tests/data/DesignspaceTest/DesignspaceTest.designspace
+Filename: fontmake-3.7.1/tests/data/DesignspaceRuleOrder/MyFont_Hair.ufo/glyphs/Q_.glif
 Comment: 
 
-Filename: fontmake-3.7.0b3/tests/data/DesignspaceTest/MyFont-Light.ufoz
+Filename: fontmake-3.7.1/tests/data/DesignspaceRuleOrder/MyFont_Hair.ufo/glyphs/Q_.alt.glif
 Comment: 
 
-Filename: fontmake-3.7.0b3/tests/data/DesignspaceTest/DesignspaceTest-instance-attrs.designspace
+Filename: fontmake-3.7.1/tests/data/DesignspaceRuleOrder/MyFont_Hair.ufo/glyphs/Q_.ss01.glif
 Comment: 
 
-Filename: fontmake-3.7.0b3/tests/data/DesignspaceTest/DesignspaceTest-slnt.designspace
+Filename: fontmake-3.7.1/tests/data/GlyphsUnitTestSans3.glyphspackage/glyphs/
 Comment: 
 
-Filename: fontmake-3.7.0b3/tests/data/DesignspaceTest/DesignspaceTest-opsz.designspace
+Filename: fontmake-3.7.1/tests/data/GlyphsUnitTestSans3.glyphspackage/order.plist
 Comment: 
 
-Filename: fontmake-3.7.0b3/tests/data/DesignspaceTest/DesignspaceTest-lib.designspace
+Filename: fontmake-3.7.1/tests/data/GlyphsUnitTestSans3.glyphspackage/fontinfo.plist
 Comment: 
 
-Filename: fontmake-3.7.0b3/tests/data/DesignspaceTest/DesignspaceTest-wght-wdth.designspace
+Filename: fontmake-3.7.1/tests/data/GlyphsUnitTestSans3.glyphspackage/glyphs/h.glyph
 Comment: 
 
-Filename: fontmake-3.7.0b3/tests/data/DesignspaceTest/MyFont-Bold.ufoz
+Filename: fontmake-3.7.1/tests/data/GlyphsUnitTestSans3.glyphspackage/glyphs/a.sc.glyph
 Comment: 
 
-Filename: fontmake-3.7.0b3/tests/data/DesignspaceTest/DesignspaceTest-bare.designspace
+Filename: fontmake-3.7.1/tests/data/GlyphsUnitTestSans3.glyphspackage/glyphs/A_dieresis.glyph
 Comment: 
 
-Filename: fontmake-3.7.0b3/tests/data/DesignspaceTest/MyFont-Light.ufo/glyphs/
+Filename: fontmake-3.7.1/tests/data/GlyphsUnitTestSans3.glyphspackage/glyphs/adieresis.glyph
 Comment: 
 
-Filename: fontmake-3.7.0b3/tests/data/DesignspaceTest/MyFont-Light.ufo/layercontents.plist
+Filename: fontmake-3.7.1/tests/data/GlyphsUnitTestSans3.glyphspackage/glyphs/dieresis.glyph
 Comment: 
 
-Filename: fontmake-3.7.0b3/tests/data/DesignspaceTest/MyFont-Light.ufo/groups.plist
+Filename: fontmake-3.7.1/tests/data/GlyphsUnitTestSans3.glyphspackage/glyphs/_part.stem.glyph
 Comment: 
 
-Filename: fontmake-3.7.0b3/tests/data/DesignspaceTest/MyFont-Light.ufo/fontinfo.plist
+Filename: fontmake-3.7.1/tests/data/GlyphsUnitTestSans3.glyphspackage/glyphs/n.glyph
 Comment: 
 
-Filename: fontmake-3.7.0b3/tests/data/DesignspaceTest/MyFont-Light.ufo/metainfo.plist
+Filename: fontmake-3.7.1/tests/data/GlyphsUnitTestSans3.glyphspackage/glyphs/m.glyph
 Comment: 
 
-Filename: fontmake-3.7.0b3/tests/data/DesignspaceTest/MyFont-Light.ufo/lib.plist
+Filename: fontmake-3.7.1/tests/data/GlyphsUnitTestSans3.glyphspackage/glyphs/_part.shoulder.glyph
 Comment: 
 
-Filename: fontmake-3.7.0b3/tests/data/DesignspaceTest/MyFont-Light.ufo/glyphs/l.glif
+Filename: fontmake-3.7.1/tests/data/GlyphsUnitTestSans3.glyphspackage/glyphs/A_.glyph
 Comment: 
 
-Filename: fontmake-3.7.0b3/tests/data/DesignspaceTest/MyFont-Light.ufo/glyphs/contents.plist
+Filename: fontmake-3.7.1/tests/data/GlyphsUnitTestSans3.glyphspackage/glyphs/a.glyph
 Comment: 
 
-Filename: fontmake-3.7.0b3/tests/data/DesignspaceTest/MyFont-Bold.ufo/glyphs/
+Filename: fontmake-3.7.1/tests/data/SwapGlyphNames/B.ufo/
 Comment: 
 
-Filename: fontmake-3.7.0b3/tests/data/DesignspaceTest/MyFont-Bold.ufo/layercontents.plist
+Filename: fontmake-3.7.1/tests/data/SwapGlyphNames/A.ufo/
 Comment: 
 
-Filename: fontmake-3.7.0b3/tests/data/DesignspaceTest/MyFont-Bold.ufo/fontinfo.plist
+Filename: fontmake-3.7.1/tests/data/SwapGlyphNames/B.ufo/glyphs/
 Comment: 
 
-Filename: fontmake-3.7.0b3/tests/data/DesignspaceTest/MyFont-Bold.ufo/metainfo.plist
+Filename: fontmake-3.7.1/tests/data/SwapGlyphNames/B.ufo/metainfo.plist
 Comment: 
 
-Filename: fontmake-3.7.0b3/tests/data/DesignspaceTest/MyFont-Bold.ufo/glyphs/l.glif
+Filename: fontmake-3.7.1/tests/data/SwapGlyphNames/B.ufo/fontinfo.plist
 Comment: 
 
-Filename: fontmake-3.7.0b3/tests/data/DesignspaceTest/MyFont-Bold.ufo/glyphs/contents.plist
+Filename: fontmake-3.7.1/tests/data/SwapGlyphNames/B.ufo/layercontents.plist
 Comment: 
 
-Filename: fontmake-3.7.0b3/tests/data/InstantiatorStrictMathGlyph/SquareOne.ufo/
+Filename: fontmake-3.7.1/tests/data/SwapGlyphNames/B.ufo/lib.plist
 Comment: 
 
-Filename: fontmake-3.7.0b3/tests/data/InstantiatorStrictMathGlyph/SquareTwo.ufo/
+Filename: fontmake-3.7.1/tests/data/SwapGlyphNames/B.ufo/glyphs/dieresiscomb.glif
 Comment: 
 
-Filename: fontmake-3.7.0b3/tests/data/InstantiatorStrictMathGlyph/StrictMathGlyph.designspace
+Filename: fontmake-3.7.1/tests/data/SwapGlyphNames/B.ufo/glyphs/a.alt.glif
 Comment: 
 
-Filename: fontmake-3.7.0b3/tests/data/InstantiatorStrictMathGlyph/SquareOne.ufo/glyphs/
+Filename: fontmake-3.7.1/tests/data/SwapGlyphNames/B.ufo/glyphs/adieresis.glif
 Comment: 
 
-Filename: fontmake-3.7.0b3/tests/data/InstantiatorStrictMathGlyph/SquareOne.ufo/layercontents.plist
+Filename: fontmake-3.7.1/tests/data/SwapGlyphNames/B.ufo/glyphs/contents.plist
 Comment: 
 
-Filename: fontmake-3.7.0b3/tests/data/InstantiatorStrictMathGlyph/SquareOne.ufo/fontinfo.plist
+Filename: fontmake-3.7.1/tests/data/SwapGlyphNames/B.ufo/glyphs/adieresis.alt.glif
 Comment: 
 
-Filename: fontmake-3.7.0b3/tests/data/InstantiatorStrictMathGlyph/SquareOne.ufo/metainfo.plist
+Filename: fontmake-3.7.1/tests/data/SwapGlyphNames/B.ufo/glyphs/a.glif
 Comment: 
 
-Filename: fontmake-3.7.0b3/tests/data/InstantiatorStrictMathGlyph/SquareOne.ufo/lib.plist
+Filename: fontmake-3.7.1/tests/data/SwapGlyphNames/A.ufo/glyphs/
 Comment: 
 
-Filename: fontmake-3.7.0b3/tests/data/InstantiatorStrictMathGlyph/SquareOne.ufo/glyphs/contents.plist
+Filename: fontmake-3.7.1/tests/data/SwapGlyphNames/A.ufo/metainfo.plist
 Comment: 
 
-Filename: fontmake-3.7.0b3/tests/data/InstantiatorStrictMathGlyph/SquareOne.ufo/glyphs/test.glif
+Filename: fontmake-3.7.1/tests/data/SwapGlyphNames/A.ufo/kerning.plist
 Comment: 
 
-Filename: fontmake-3.7.0b3/tests/data/InstantiatorStrictMathGlyph/SquareOne.ufo/glyphs/layerinfo.plist
+Filename: fontmake-3.7.1/tests/data/SwapGlyphNames/A.ufo/groups.plist
 Comment: 
 
-Filename: fontmake-3.7.0b3/tests/data/InstantiatorStrictMathGlyph/SquareTwo.ufo/glyphs/
+Filename: fontmake-3.7.1/tests/data/SwapGlyphNames/A.ufo/fontinfo.plist
 Comment: 
 
-Filename: fontmake-3.7.0b3/tests/data/InstantiatorStrictMathGlyph/SquareTwo.ufo/layercontents.plist
+Filename: fontmake-3.7.1/tests/data/SwapGlyphNames/A.ufo/layercontents.plist
 Comment: 
 
-Filename: fontmake-3.7.0b3/tests/data/InstantiatorStrictMathGlyph/SquareTwo.ufo/fontinfo.plist
+Filename: fontmake-3.7.1/tests/data/SwapGlyphNames/A.ufo/lib.plist
 Comment: 
 
-Filename: fontmake-3.7.0b3/tests/data/InstantiatorStrictMathGlyph/SquareTwo.ufo/metainfo.plist
+Filename: fontmake-3.7.1/tests/data/SwapGlyphNames/A.ufo/glyphs/aaa.glif
 Comment: 
 
-Filename: fontmake-3.7.0b3/tests/data/InstantiatorStrictMathGlyph/SquareTwo.ufo/lib.plist
+Filename: fontmake-3.7.1/tests/data/SwapGlyphNames/A.ufo/glyphs/x.glif
 Comment: 
 
-Filename: fontmake-3.7.0b3/tests/data/InstantiatorStrictMathGlyph/SquareTwo.ufo/glyphs/contents.plist
+Filename: fontmake-3.7.1/tests/data/SwapGlyphNames/A.ufo/glyphs/space.glif
 Comment: 
 
-Filename: fontmake-3.7.0b3/tests/data/InstantiatorStrictMathGlyph/SquareTwo.ufo/glyphs/test.glif
+Filename: fontmake-3.7.1/tests/data/SwapGlyphNames/A.ufo/glyphs/aaa.swap.glif
 Comment: 
 
-Filename: fontmake-3.7.0b3/tests/data/InstantiatorStrictMathGlyph/SquareTwo.ufo/glyphs/layerinfo.plist
+Filename: fontmake-3.7.1/tests/data/SwapGlyphNames/A.ufo/glyphs/contents.plist
 Comment: 
 
-Filename: fontmake-3.7.0b3/tests/data/DesignspaceBrokenTest/MyFont-Light.ufo/
+Filename: fontmake-3.7.1/tests/data/SwapGlyphNames/A.ufo/glyphs/y.glif
 Comment: 
 
-Filename: fontmake-3.7.0b3/tests/data/DesignspaceBrokenTest/MyFont-Bold.ufo/
+Filename: fontmake-3.7.1/tests/data/SwapGlyphNames/A.ufo/glyphs/a.glif
 Comment: 
 
-Filename: fontmake-3.7.0b3/tests/data/DesignspaceBrokenTest/DesignspaceTest.designspace
+Filename: fontmake-3.7.1/tests/data/SwapGlyphNames/A.ufo/glyphs/a.swap.glif
 Comment: 
 
-Filename: fontmake-3.7.0b3/tests/data/DesignspaceBrokenTest/Designspace-MastersAsInstances.designspace
+Filename: fontmake-3.7.1/tests/data/DesignspaceBrokenTest/MyFont-Light.ufo/
 Comment: 
 
-Filename: fontmake-3.7.0b3/tests/data/DesignspaceBrokenTest/MyFont-Light.ufo/glyphs/
+Filename: fontmake-3.7.1/tests/data/DesignspaceBrokenTest/MyFont-Bold.ufo/
 Comment: 
 
-Filename: fontmake-3.7.0b3/tests/data/DesignspaceBrokenTest/MyFont-Light.ufo/layercontents.plist
+Filename: fontmake-3.7.1/tests/data/DesignspaceBrokenTest/Designspace-MastersAsInstances.designspace
 Comment: 
 
-Filename: fontmake-3.7.0b3/tests/data/DesignspaceBrokenTest/MyFont-Light.ufo/fontinfo.plist
+Filename: fontmake-3.7.1/tests/data/DesignspaceBrokenTest/DesignspaceTest.designspace
 Comment: 
 
-Filename: fontmake-3.7.0b3/tests/data/DesignspaceBrokenTest/MyFont-Light.ufo/metainfo.plist
+Filename: fontmake-3.7.1/tests/data/DesignspaceBrokenTest/MyFont-Light.ufo/glyphs/
 Comment: 
 
-Filename: fontmake-3.7.0b3/tests/data/DesignspaceBrokenTest/MyFont-Light.ufo/lib.plist
+Filename: fontmake-3.7.1/tests/data/DesignspaceBrokenTest/MyFont-Light.ufo/metainfo.plist
 Comment: 
 
-Filename: fontmake-3.7.0b3/tests/data/DesignspaceBrokenTest/MyFont-Light.ufo/glyphs/l.glif
+Filename: fontmake-3.7.1/tests/data/DesignspaceBrokenTest/MyFont-Light.ufo/fontinfo.plist
 Comment: 
 
-Filename: fontmake-3.7.0b3/tests/data/DesignspaceBrokenTest/MyFont-Light.ufo/glyphs/contents.plist
+Filename: fontmake-3.7.1/tests/data/DesignspaceBrokenTest/MyFont-Light.ufo/layercontents.plist
 Comment: 
 
-Filename: fontmake-3.7.0b3/tests/data/DesignspaceBrokenTest/MyFont-Light.ufo/glyphs/asas.glif
+Filename: fontmake-3.7.1/tests/data/DesignspaceBrokenTest/MyFont-Light.ufo/lib.plist
 Comment: 
 
-Filename: fontmake-3.7.0b3/tests/data/DesignspaceBrokenTest/MyFont-Bold.ufo/glyphs/
+Filename: fontmake-3.7.1/tests/data/DesignspaceBrokenTest/MyFont-Light.ufo/glyphs/l.glif
 Comment: 
 
-Filename: fontmake-3.7.0b3/tests/data/DesignspaceBrokenTest/MyFont-Bold.ufo/layercontents.plist
+Filename: fontmake-3.7.1/tests/data/DesignspaceBrokenTest/MyFont-Light.ufo/glyphs/asas.glif
 Comment: 
 
-Filename: fontmake-3.7.0b3/tests/data/DesignspaceBrokenTest/MyFont-Bold.ufo/fontinfo.plist
+Filename: fontmake-3.7.1/tests/data/DesignspaceBrokenTest/MyFont-Light.ufo/glyphs/contents.plist
 Comment: 
 
-Filename: fontmake-3.7.0b3/tests/data/DesignspaceBrokenTest/MyFont-Bold.ufo/metainfo.plist
+Filename: fontmake-3.7.1/tests/data/DesignspaceBrokenTest/MyFont-Bold.ufo/glyphs/
 Comment: 
 
-Filename: fontmake-3.7.0b3/tests/data/DesignspaceBrokenTest/MyFont-Bold.ufo/lib.plist
+Filename: fontmake-3.7.1/tests/data/DesignspaceBrokenTest/MyFont-Bold.ufo/metainfo.plist
 Comment: 
 
-Filename: fontmake-3.7.0b3/tests/data/DesignspaceBrokenTest/MyFont-Bold.ufo/glyphs/l.glif
+Filename: fontmake-3.7.1/tests/data/DesignspaceBrokenTest/MyFont-Bold.ufo/fontinfo.plist
 Comment: 
 
-Filename: fontmake-3.7.0b3/tests/data/DesignspaceBrokenTest/MyFont-Bold.ufo/glyphs/contents.plist
+Filename: fontmake-3.7.1/tests/data/DesignspaceBrokenTest/MyFont-Bold.ufo/layercontents.plist
 Comment: 
 
-Filename: fontmake-3.7.0b3/tests/data/DesignspaceBrokenTest/MyFont-Bold.ufo/glyphs/asas.glif
+Filename: fontmake-3.7.1/tests/data/DesignspaceBrokenTest/MyFont-Bold.ufo/lib.plist
 Comment: 
 
-Filename: fontmake-3.7.0b3/tests/data/InterpolateLayoutTest/InterpolateLayoutTest GSUB.txt
+Filename: fontmake-3.7.1/tests/data/DesignspaceBrokenTest/MyFont-Bold.ufo/glyphs/l.glif
 Comment: 
 
-Filename: fontmake-3.7.0b3/tests/data/InterpolateLayoutTest/InterpolateLayoutTest.plist
+Filename: fontmake-3.7.1/tests/data/DesignspaceBrokenTest/MyFont-Bold.ufo/glyphs/asas.glif
 Comment: 
 
-Filename: fontmake-3.7.0b3/tests/data/InterpolateLayoutTest/InterpolateLayoutTest GDEF.txt
+Filename: fontmake-3.7.1/tests/data/DesignspaceBrokenTest/MyFont-Bold.ufo/glyphs/contents.plist
 Comment: 
 
-Filename: fontmake-3.7.0b3/tests/data/InterpolateLayoutTest/InterpolateLayoutTest 1000 GPOS.txt
+Filename: fontmake-3.7.1/tests/data/DesignspaceTest/MyFont-Light.ufo/
 Comment: 
 
-Filename: fontmake-3.7.0b3/tests/data/InterpolateLayoutTest/InterpolateLayoutTest.glyphs
+Filename: fontmake-3.7.1/tests/data/DesignspaceTest/MyFont-Bold.ufo/
 Comment: 
 
-Filename: fontmake-3.7.0b3/tests/data/InterpolateLayoutTest/InterpolateLayoutTest 0 GPOS.txt
+Filename: fontmake-3.7.1/tests/data/DesignspaceTest/DesignspaceTest-lib.designspace
 Comment: 
 
-Filename: fontmake-3.7.0b3/tests/data/AutohintingTest/Padyakke.glyphs
+Filename: fontmake-3.7.1/tests/data/DesignspaceTest/DesignspaceTest-wght-wdth.designspace
 Comment: 
 
-Filename: fontmake-3.7.0b3/tests/data/IncompatibleSans/IncompatibleSans-Bold.ufo/
+Filename: fontmake-3.7.1/tests/data/DesignspaceTest/MyFont-Light.ufoz
 Comment: 
 
-Filename: fontmake-3.7.0b3/tests/data/IncompatibleSans/IncompatibleSans-Regular.ufo/
+Filename: fontmake-3.7.1/tests/data/DesignspaceTest/DesignspaceTest-opsz.designspace
 Comment: 
 
-Filename: fontmake-3.7.0b3/tests/data/IncompatibleSans/IncompatibleSans.designspace
+Filename: fontmake-3.7.1/tests/data/DesignspaceTest/MyFont-Bold.ufoz
 Comment: 
 
-Filename: fontmake-3.7.0b3/tests/data/IncompatibleSans/IncompatibleSans-Bold.ufo/glyphs/
+Filename: fontmake-3.7.1/tests/data/DesignspaceTest/DesignspaceTest-bare.designspace
 Comment: 
 
-Filename: fontmake-3.7.0b3/tests/data/IncompatibleSans/IncompatibleSans-Bold.ufo/features.fea
+Filename: fontmake-3.7.1/tests/data/DesignspaceTest/DesignspaceTest-instance-attrs.designspace
 Comment: 
 
-Filename: fontmake-3.7.0b3/tests/data/IncompatibleSans/IncompatibleSans-Bold.ufo/layercontents.plist
+Filename: fontmake-3.7.1/tests/data/DesignspaceTest/DesignspaceTest-slnt.designspace
 Comment: 
 
-Filename: fontmake-3.7.0b3/tests/data/IncompatibleSans/IncompatibleSans-Bold.ufo/fontinfo.plist
+Filename: fontmake-3.7.1/tests/data/DesignspaceTest/DesignspaceTest.designspace
 Comment: 
 
-Filename: fontmake-3.7.0b3/tests/data/IncompatibleSans/IncompatibleSans-Bold.ufo/metainfo.plist
+Filename: fontmake-3.7.1/tests/data/DesignspaceTest/MyFont-Light.ufo/glyphs/
 Comment: 
 
-Filename: fontmake-3.7.0b3/tests/data/IncompatibleSans/IncompatibleSans-Bold.ufo/lib.plist
+Filename: fontmake-3.7.1/tests/data/DesignspaceTest/MyFont-Light.ufo/metainfo.plist
 Comment: 
 
-Filename: fontmake-3.7.0b3/tests/data/IncompatibleSans/IncompatibleSans-Bold.ufo/glyphs/D_.glif
+Filename: fontmake-3.7.1/tests/data/DesignspaceTest/MyFont-Light.ufo/groups.plist
 Comment: 
 
-Filename: fontmake-3.7.0b3/tests/data/IncompatibleSans/IncompatibleSans-Bold.ufo/glyphs/C_.glif
+Filename: fontmake-3.7.1/tests/data/DesignspaceTest/MyFont-Light.ufo/fontinfo.plist
 Comment: 
 
-Filename: fontmake-3.7.0b3/tests/data/IncompatibleSans/IncompatibleSans-Bold.ufo/glyphs/B_.glif
+Filename: fontmake-3.7.1/tests/data/DesignspaceTest/MyFont-Light.ufo/layercontents.plist
 Comment: 
 
-Filename: fontmake-3.7.0b3/tests/data/IncompatibleSans/IncompatibleSans-Bold.ufo/glyphs/contents.plist
+Filename: fontmake-3.7.1/tests/data/DesignspaceTest/MyFont-Light.ufo/lib.plist
 Comment: 
 
-Filename: fontmake-3.7.0b3/tests/data/IncompatibleSans/IncompatibleSans-Bold.ufo/glyphs/space.glif
+Filename: fontmake-3.7.1/tests/data/DesignspaceTest/MyFont-Light.ufo/glyphs/l.glif
 Comment: 
 
-Filename: fontmake-3.7.0b3/tests/data/IncompatibleSans/IncompatibleSans-Bold.ufo/glyphs/A_.glif
+Filename: fontmake-3.7.1/tests/data/DesignspaceTest/MyFont-Light.ufo/glyphs/contents.plist
 Comment: 
 
-Filename: fontmake-3.7.0b3/tests/data/IncompatibleSans/IncompatibleSans-Regular.ufo/glyphs/
+Filename: fontmake-3.7.1/tests/data/DesignspaceTest/MyFont-Bold.ufo/glyphs/
 Comment: 
 
-Filename: fontmake-3.7.0b3/tests/data/IncompatibleSans/IncompatibleSans-Regular.ufo/layercontents.plist
+Filename: fontmake-3.7.1/tests/data/DesignspaceTest/MyFont-Bold.ufo/metainfo.plist
 Comment: 
 
-Filename: fontmake-3.7.0b3/tests/data/IncompatibleSans/IncompatibleSans-Regular.ufo/fontinfo.plist
+Filename: fontmake-3.7.1/tests/data/DesignspaceTest/MyFont-Bold.ufo/fontinfo.plist
 Comment: 
 
-Filename: fontmake-3.7.0b3/tests/data/IncompatibleSans/IncompatibleSans-Regular.ufo/metainfo.plist
+Filename: fontmake-3.7.1/tests/data/DesignspaceTest/MyFont-Bold.ufo/layercontents.plist
 Comment: 
 
-Filename: fontmake-3.7.0b3/tests/data/IncompatibleSans/IncompatibleSans-Regular.ufo/lib.plist
+Filename: fontmake-3.7.1/tests/data/DesignspaceTest/MyFont-Bold.ufo/glyphs/l.glif
 Comment: 
 
-Filename: fontmake-3.7.0b3/tests/data/IncompatibleSans/IncompatibleSans-Regular.ufo/glyphs/D_.glif
+Filename: fontmake-3.7.1/tests/data/DesignspaceTest/MyFont-Bold.ufo/glyphs/contents.plist
 Comment: 
 
-Filename: fontmake-3.7.0b3/tests/data/IncompatibleSans/IncompatibleSans-Regular.ufo/glyphs/C_.glif
+Filename: fontmake-3.7.1/tests/data/MutatorSansLite/MutatorSansLightWide.ufo/
 Comment: 
 
-Filename: fontmake-3.7.0b3/tests/data/IncompatibleSans/IncompatibleSans-Regular.ufo/glyphs/B_.glif
+Filename: fontmake-3.7.1/tests/data/MutatorSansLite/MutatorSansBoldWide.ufo/
 Comment: 
 
-Filename: fontmake-3.7.0b3/tests/data/IncompatibleSans/IncompatibleSans-Regular.ufo/glyphs/contents.plist
+Filename: fontmake-3.7.1/tests/data/MutatorSansLite/MutatorSansBoldCondensed.ufo/
 Comment: 
 
-Filename: fontmake-3.7.0b3/tests/data/IncompatibleSans/IncompatibleSans-Regular.ufo/glyphs/space.glif
+Filename: fontmake-3.7.1/tests/data/MutatorSansLite/MutatorSerifLightWide.ufo/
 Comment: 
 
-Filename: fontmake-3.7.0b3/tests/data/IncompatibleSans/IncompatibleSans-Regular.ufo/glyphs/A_.glif
+Filename: fontmake-3.7.1/tests/data/MutatorSansLite/MutatorSansLightCondensed.ufo/
 Comment: 
 
-Filename: fontmake-3.7.0b3/tests/data/DesignspaceTestSharedFeatures/DesignspaceTest-Regular.ufo/
+Filename: fontmake-3.7.1/tests/data/MutatorSansLite/MutatorSerifLightCondensed.ufo/
 Comment: 
 
-Filename: fontmake-3.7.0b3/tests/data/DesignspaceTestSharedFeatures/DesignspaceTest-Light.ufo/
+Filename: fontmake-3.7.1/tests/data/MutatorSansLite/LICENSE
 Comment: 
 
-Filename: fontmake-3.7.0b3/tests/data/DesignspaceTestSharedFeatures/DesignspaceTestSharedFeatures.designspace
+Filename: fontmake-3.7.1/tests/data/MutatorSansLite/MutatorSans_v5_several_vfs.designspace
 Comment: 
 
-Filename: fontmake-3.7.0b3/tests/data/DesignspaceTestSharedFeatures/family.fea
+Filename: fontmake-3.7.1/tests/data/MutatorSansLite/MutatorSans_v5_implicit_one_vf.designspace
 Comment: 
 
-Filename: fontmake-3.7.0b3/tests/data/DesignspaceTestSharedFeatures/DesignspaceTest-Regular.ufo/glyphs/
+Filename: fontmake-3.7.1/tests/data/MutatorSansLite/MutatorFamily_v5_discrete_axis.designspace
 Comment: 
 
-Filename: fontmake-3.7.0b3/tests/data/DesignspaceTestSharedFeatures/DesignspaceTest-Regular.ufo/features.fea
+Filename: fontmake-3.7.1/tests/data/MutatorSansLite/MutatorSans_v5_several_vfs_discrete_axis.designspace
 Comment: 
 
-Filename: fontmake-3.7.0b3/tests/data/DesignspaceTestSharedFeatures/DesignspaceTest-Regular.ufo/layercontents.plist
+Filename: fontmake-3.7.1/tests/data/MutatorSansLite/MutatorSansLightWide.ufo/glyphs.master_width_720.00_weight_645.00/
 Comment: 
 
-Filename: fontmake-3.7.0b3/tests/data/DesignspaceTestSharedFeatures/DesignspaceTest-Regular.ufo/fontinfo.plist
+Filename: fontmake-3.7.1/tests/data/MutatorSansLite/MutatorSansLightWide.ufo/glyphs.background/
 Comment: 
 
-Filename: fontmake-3.7.0b3/tests/data/DesignspaceTestSharedFeatures/DesignspaceTest-Regular.ufo/metainfo.plist
+Filename: fontmake-3.7.1/tests/data/MutatorSansLite/MutatorSansLightWide.ufo/glyphs/
 Comment: 
 
-Filename: fontmake-3.7.0b3/tests/data/DesignspaceTestSharedFeatures/DesignspaceTest-Regular.ufo/glyphs/contents.plist
+Filename: fontmake-3.7.1/tests/data/MutatorSansLite/MutatorSansLightWide.ufo/glyphs.master_width_695.65_weight_166.38/
 Comment: 
 
-Filename: fontmake-3.7.0b3/tests/data/DesignspaceTestSharedFeatures/DesignspaceTest-Light.ufo/glyphs/
+Filename: fontmake-3.7.1/tests/data/MutatorSansLite/MutatorSansLightWide.ufo/glyphs.master_width_0.00_weight_0.00/
 Comment: 
 
-Filename: fontmake-3.7.0b3/tests/data/DesignspaceTestSharedFeatures/DesignspaceTest-Light.ufo/layercontents.plist
+Filename: fontmake-3.7.1/tests/data/MutatorSansLite/MutatorSansLightWide.ufo/glyphs.master_width_500.00_weight_500.00/
 Comment: 
 
-Filename: fontmake-3.7.0b3/tests/data/DesignspaceTestSharedFeatures/DesignspaceTest-Light.ufo/fontinfo.plist
+Filename: fontmake-3.7.1/tests/data/MutatorSansLite/MutatorSansLightWide.ufo/metainfo.plist
 Comment: 
 
-Filename: fontmake-3.7.0b3/tests/data/DesignspaceTestSharedFeatures/DesignspaceTest-Light.ufo/metainfo.plist
+Filename: fontmake-3.7.1/tests/data/MutatorSansLite/MutatorSansLightWide.ufo/fontinfo.plist
 Comment: 
 
-Filename: fontmake-3.7.0b3/tests/data/DesignspaceTestSharedFeatures/DesignspaceTest-Light.ufo/glyphs/contents.plist
+Filename: fontmake-3.7.1/tests/data/MutatorSansLite/MutatorSansLightWide.ufo/layercontents.plist
 Comment: 
 
-Filename: fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansLightWide.ufo/
+Filename: fontmake-3.7.1/tests/data/MutatorSansLite/MutatorSansLightWide.ufo/lib.plist
 Comment: 
 
-Filename: fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansIntermediateCondensed.ufo/
+Filename: fontmake-3.7.1/tests/data/MutatorSansLite/MutatorSansLightWide.ufo/features.fea
 Comment: 
 
-Filename: fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/
+Filename: fontmake-3.7.1/tests/data/MutatorSansLite/MutatorSansLightWide.ufo/glyphs.master_width_720.00_weight_645.00/S_.glif
 Comment: 
 
-Filename: fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansIntermediateWide.ufo/
+Filename: fontmake-3.7.1/tests/data/MutatorSansLite/MutatorSansLightWide.ufo/glyphs.master_width_720.00_weight_645.00/contents.plist
 Comment: 
 
-Filename: fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansBoldWide.ufo/
+Filename: fontmake-3.7.1/tests/data/MutatorSansLite/MutatorSansLightWide.ufo/glyphs.master_width_720.00_weight_645.00/layerinfo.plist
 Comment: 
 
-Filename: fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/
+Filename: fontmake-3.7.1/tests/data/MutatorSansLite/MutatorSansLightWide.ufo/glyphs.background/contents.plist
 Comment: 
 
-Filename: fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSans_missing.designspace
+Filename: fontmake-3.7.1/tests/data/MutatorSansLite/MutatorSansLightWide.ufo/glyphs.background/layerinfo.plist
 Comment: 
 
-Filename: fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSans.designspace
+Filename: fontmake-3.7.1/tests/data/MutatorSansLite/MutatorSansLightWide.ufo/glyphs.background/S_.closed.glif
 Comment: 
 
-Filename: fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSans-width-only.designspace
+Filename: fontmake-3.7.1/tests/data/MutatorSansLite/MutatorSansLightWide.ufo/glyphs/S_.glif
 Comment: 
 
-Filename: fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSans-with-openNodes.designspace
+Filename: fontmake-3.7.1/tests/data/MutatorSansLite/MutatorSansLightWide.ufo/glyphs/I_.narrow.glif
 Comment: 
 
-Filename: fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSans-weight-only.designspace
+Filename: fontmake-3.7.1/tests/data/MutatorSansLite/MutatorSansLightWide.ufo/glyphs/contents.plist
 Comment: 
 
-Filename: fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSans-non-default-layer.designspace
+Filename: fontmake-3.7.1/tests/data/MutatorSansLite/MutatorSansLightWide.ufo/glyphs/I_.glif
 Comment: 
 
-Filename: fontmake-3.7.0b3/tests/data/MutatorSans/LICENSE
+Filename: fontmake-3.7.1/tests/data/MutatorSansLite/MutatorSansLightWide.ufo/glyphs/A_.glif
 Comment: 
 
-Filename: fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSans_no_default.designspace
+Filename: fontmake-3.7.1/tests/data/MutatorSansLite/MutatorSansLightWide.ufo/glyphs/I_J_.glif
 Comment: 
 
-Filename: fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs.background/
+Filename: fontmake-3.7.1/tests/data/MutatorSansLite/MutatorSansLightWide.ufo/glyphs/layerinfo.plist
 Comment: 
 
-Filename: fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs.master_width_720.00_weight_645.00/
+Filename: fontmake-3.7.1/tests/data/MutatorSansLite/MutatorSansLightWide.ufo/glyphs/S_.closed.glif
 Comment: 
 
-Filename: fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs.master_width_0.00_weight_0.00/
+Filename: fontmake-3.7.1/tests/data/MutatorSansLite/MutatorSansLightWide.ufo/glyphs.master_width_695.65_weight_166.38/contents.plist
 Comment: 
 
-Filename: fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs.master_width_500.00_weight_500.00/
+Filename: fontmake-3.7.1/tests/data/MutatorSansLite/MutatorSansLightWide.ufo/glyphs.master_width_695.65_weight_166.38/layerinfo.plist
 Comment: 
 
-Filename: fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/
+Filename: fontmake-3.7.1/tests/data/MutatorSansLite/MutatorSansLightWide.ufo/glyphs.master_width_0.00_weight_0.00/contents.plist
 Comment: 
 
-Filename: fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs.master_width_695.65_weight_166.38/
+Filename: fontmake-3.7.1/tests/data/MutatorSansLite/MutatorSansLightWide.ufo/glyphs.master_width_0.00_weight_0.00/layerinfo.plist
 Comment: 
 
-Filename: fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansLightWide.ufo/features.fea
+Filename: fontmake-3.7.1/tests/data/MutatorSansLite/MutatorSansLightWide.ufo/glyphs.master_width_500.00_weight_500.00/S_.glif
 Comment: 
 
-Filename: fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansLightWide.ufo/layercontents.plist
+Filename: fontmake-3.7.1/tests/data/MutatorSansLite/MutatorSansLightWide.ufo/glyphs.master_width_500.00_weight_500.00/contents.plist
 Comment: 
 
-Filename: fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansLightWide.ufo/groups.plist
+Filename: fontmake-3.7.1/tests/data/MutatorSansLite/MutatorSansLightWide.ufo/glyphs.master_width_500.00_weight_500.00/layerinfo.plist
 Comment: 
 
-Filename: fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansLightWide.ufo/kerning.plist
+Filename: fontmake-3.7.1/tests/data/MutatorSansLite/MutatorSansBoldWide.ufo/glyphs.background/
 Comment: 
 
-Filename: fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansLightWide.ufo/fontinfo.plist
+Filename: fontmake-3.7.1/tests/data/MutatorSansLite/MutatorSansBoldWide.ufo/glyphs/
 Comment: 
 
-Filename: fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansLightWide.ufo/metainfo.plist
+Filename: fontmake-3.7.1/tests/data/MutatorSansLite/MutatorSansBoldWide.ufo/metainfo.plist
 Comment: 
 
-Filename: fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansLightWide.ufo/lib.plist
+Filename: fontmake-3.7.1/tests/data/MutatorSansLite/MutatorSansBoldWide.ufo/fontinfo.plist
 Comment: 
 
-Filename: fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs.background/S_.closed.glif
+Filename: fontmake-3.7.1/tests/data/MutatorSansLite/MutatorSansBoldWide.ufo/layercontents.plist
 Comment: 
 
-Filename: fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs.background/contents.plist
+Filename: fontmake-3.7.1/tests/data/MutatorSansLite/MutatorSansBoldWide.ufo/lib.plist
 Comment: 
 
-Filename: fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs.background/layerinfo.plist
+Filename: fontmake-3.7.1/tests/data/MutatorSansLite/MutatorSansBoldWide.ufo/features.fea
 Comment: 
 
-Filename: fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs.master_width_720.00_weight_645.00/contents.plist
+Filename: fontmake-3.7.1/tests/data/MutatorSansLite/MutatorSansBoldWide.ufo/glyphs.background/S_.glif
 Comment: 
 
-Filename: fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs.master_width_720.00_weight_645.00/S_.glif
+Filename: fontmake-3.7.1/tests/data/MutatorSansLite/MutatorSansBoldWide.ufo/glyphs.background/contents.plist
 Comment: 
 
-Filename: fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs.master_width_720.00_weight_645.00/layerinfo.plist
+Filename: fontmake-3.7.1/tests/data/MutatorSansLite/MutatorSansBoldWide.ufo/glyphs.background/layerinfo.plist
 Comment: 
 
-Filename: fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs.master_width_0.00_weight_0.00/contents.plist
+Filename: fontmake-3.7.1/tests/data/MutatorSansLite/MutatorSansBoldWide.ufo/glyphs.background/S_.closed.glif
 Comment: 
 
-Filename: fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs.master_width_0.00_weight_0.00/layerinfo.plist
+Filename: fontmake-3.7.1/tests/data/MutatorSansLite/MutatorSansBoldWide.ufo/glyphs/S_.glif
 Comment: 
 
-Filename: fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs.master_width_500.00_weight_500.00/contents.plist
+Filename: fontmake-3.7.1/tests/data/MutatorSansLite/MutatorSansBoldWide.ufo/glyphs/I_.narrow.glif
 Comment: 
 
-Filename: fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs.master_width_500.00_weight_500.00/S_.glif
+Filename: fontmake-3.7.1/tests/data/MutatorSansLite/MutatorSansBoldWide.ufo/glyphs/contents.plist
 Comment: 
 
-Filename: fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs.master_width_500.00_weight_500.00/layerinfo.plist
+Filename: fontmake-3.7.1/tests/data/MutatorSansLite/MutatorSansBoldWide.ufo/glyphs/I_.glif
 Comment: 
 
-Filename: fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/W_.glif
+Filename: fontmake-3.7.1/tests/data/MutatorSansLite/MutatorSansBoldWide.ufo/glyphs/A_.glif
 Comment: 
 
-Filename: fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/quotedblleft.glif
+Filename: fontmake-3.7.1/tests/data/MutatorSansLite/MutatorSansBoldWide.ufo/glyphs/I_J_.glif
 Comment: 
 
-Filename: fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/T_.glif
+Filename: fontmake-3.7.1/tests/data/MutatorSansLite/MutatorSansBoldWide.ufo/glyphs/layerinfo.plist
 Comment: 
 
-Filename: fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/R_.glif
+Filename: fontmake-3.7.1/tests/data/MutatorSansLite/MutatorSansBoldWide.ufo/glyphs/S_.closed.glif
 Comment: 
 
-Filename: fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/O_.glif
+Filename: fontmake-3.7.1/tests/data/MutatorSansLite/MutatorSansBoldCondensed.ufo/glyphs.background/
 Comment: 
 
-Filename: fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/G_.glif
+Filename: fontmake-3.7.1/tests/data/MutatorSansLite/MutatorSansBoldCondensed.ufo/glyphs/
 Comment: 
 
-Filename: fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/D_.glif
+Filename: fontmake-3.7.1/tests/data/MutatorSansLite/MutatorSansBoldCondensed.ufo/metainfo.plist
 Comment: 
 
-Filename: fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/S_.closed.glif
+Filename: fontmake-3.7.1/tests/data/MutatorSansLite/MutatorSansBoldCondensed.ufo/fontinfo.plist
 Comment: 
 
-Filename: fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/colon.glif
+Filename: fontmake-3.7.1/tests/data/MutatorSansLite/MutatorSansBoldCondensed.ufo/layercontents.plist
 Comment: 
 
-Filename: fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/X_.glif
+Filename: fontmake-3.7.1/tests/data/MutatorSansLite/MutatorSansBoldCondensed.ufo/lib.plist
 Comment: 
 
-Filename: fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/M_.glif
+Filename: fontmake-3.7.1/tests/data/MutatorSansLite/MutatorSansBoldCondensed.ufo/features.fea
 Comment: 
 
-Filename: fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/Z_.glif
+Filename: fontmake-3.7.1/tests/data/MutatorSansLite/MutatorSansBoldCondensed.ufo/glyphs.background/contents.plist
 Comment: 
 
-Filename: fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/I_.narrow.glif
+Filename: fontmake-3.7.1/tests/data/MutatorSansLite/MutatorSansBoldCondensed.ufo/glyphs.background/layerinfo.plist
 Comment: 
 
-Filename: fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/F_.glif
+Filename: fontmake-3.7.1/tests/data/MutatorSansLite/MutatorSansBoldCondensed.ufo/glyphs.background/S_.closed.glif
 Comment: 
 
-Filename: fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/C_.glif
+Filename: fontmake-3.7.1/tests/data/MutatorSansLite/MutatorSansBoldCondensed.ufo/glyphs/S_.glif
 Comment: 
 
-Filename: fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/dot.glif
+Filename: fontmake-3.7.1/tests/data/MutatorSansLite/MutatorSansBoldCondensed.ufo/glyphs/I_.narrow.glif
 Comment: 
 
-Filename: fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/arrowright.glif
+Filename: fontmake-3.7.1/tests/data/MutatorSansLite/MutatorSansBoldCondensed.ufo/glyphs/contents.plist
 Comment: 
 
-Filename: fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/B_.glif
+Filename: fontmake-3.7.1/tests/data/MutatorSansLite/MutatorSansBoldCondensed.ufo/glyphs/I_.glif
 Comment: 
 
-Filename: fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/U_.glif
+Filename: fontmake-3.7.1/tests/data/MutatorSansLite/MutatorSansBoldCondensed.ufo/glyphs/A_.glif
 Comment: 
 
-Filename: fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/I_.glif
+Filename: fontmake-3.7.1/tests/data/MutatorSansLite/MutatorSansBoldCondensed.ufo/glyphs/I_J_.glif
 Comment: 
 
-Filename: fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/N_.glif
+Filename: fontmake-3.7.1/tests/data/MutatorSansLite/MutatorSansBoldCondensed.ufo/glyphs/layerinfo.plist
 Comment: 
 
-Filename: fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/V_.glif
+Filename: fontmake-3.7.1/tests/data/MutatorSansLite/MutatorSansBoldCondensed.ufo/glyphs/S_.closed.glif
 Comment: 
 
-Filename: fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/I_J_.glif
+Filename: fontmake-3.7.1/tests/data/MutatorSansLite/MutatorSerifLightWide.ufo/glyphs/
 Comment: 
 
-Filename: fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/comma.glif
+Filename: fontmake-3.7.1/tests/data/MutatorSansLite/MutatorSerifLightWide.ufo/metainfo.plist
 Comment: 
 
-Filename: fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/contents.plist
+Filename: fontmake-3.7.1/tests/data/MutatorSansLite/MutatorSerifLightWide.ufo/fontinfo.plist
 Comment: 
 
-Filename: fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/dieresis.glif
+Filename: fontmake-3.7.1/tests/data/MutatorSansLite/MutatorSerifLightWide.ufo/layercontents.plist
 Comment: 
 
-Filename: fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/Y_.glif
+Filename: fontmake-3.7.1/tests/data/MutatorSansLite/MutatorSerifLightWide.ufo/lib.plist
 Comment: 
 
-Filename: fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/Q_.glif
+Filename: fontmake-3.7.1/tests/data/MutatorSansLite/MutatorSerifLightWide.ufo/features.fea
 Comment: 
 
-Filename: fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/space.glif
+Filename: fontmake-3.7.1/tests/data/MutatorSansLite/MutatorSerifLightWide.ufo/glyphs/contents.plist
 Comment: 
 
-Filename: fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/quotedblbase.glif
+Filename: fontmake-3.7.1/tests/data/MutatorSansLite/MutatorSerifLightWide.ufo/glyphs/A_.glif
 Comment: 
 
-Filename: fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/L_.glif
+Filename: fontmake-3.7.1/tests/data/MutatorSansLite/MutatorSansLightCondensed.ufo/glyphs.support.crossbars/
 Comment: 
 
-Filename: fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/quotedblright.glif
+Filename: fontmake-3.7.1/tests/data/MutatorSansLite/MutatorSansLightCondensed.ufo/glyphs.support.S_.wide/
 Comment: 
 
-Filename: fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/A_acute.glif
+Filename: fontmake-3.7.1/tests/data/MutatorSansLite/MutatorSansLightCondensed.ufo/glyphs.support.S_.middle/
 Comment: 
 
-Filename: fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/arrowdown.glif
+Filename: fontmake-3.7.1/tests/data/MutatorSansLite/MutatorSansLightCondensed.ufo/glyphs.background/
 Comment: 
 
-Filename: fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/P_.glif
+Filename: fontmake-3.7.1/tests/data/MutatorSansLite/MutatorSansLightCondensed.ufo/glyphs/
 Comment: 
 
-Filename: fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/semicolon.glif
+Filename: fontmake-3.7.1/tests/data/MutatorSansLite/MutatorSansLightCondensed.ufo/glyphs.support.crossbar/
 Comment: 
 
-Filename: fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/J_.narrow.glif
+Filename: fontmake-3.7.1/tests/data/MutatorSansLite/MutatorSansLightCondensed.ufo/glyphs.support/
 Comment: 
 
-Filename: fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/A_dieresis.glif
+Filename: fontmake-3.7.1/tests/data/MutatorSansLite/MutatorSansLightCondensed.ufo/metainfo.plist
 Comment: 
 
-Filename: fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/arrowleft.glif
+Filename: fontmake-3.7.1/tests/data/MutatorSansLite/MutatorSansLightCondensed.ufo/fontinfo.plist
 Comment: 
 
-Filename: fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/K_.glif
+Filename: fontmake-3.7.1/tests/data/MutatorSansLite/MutatorSansLightCondensed.ufo/layercontents.plist
 Comment: 
 
-Filename: fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/A_.glif
+Filename: fontmake-3.7.1/tests/data/MutatorSansLite/MutatorSansLightCondensed.ufo/lib.plist
 Comment: 
 
-Filename: fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/J_.glif
+Filename: fontmake-3.7.1/tests/data/MutatorSansLite/MutatorSansLightCondensed.ufo/features.fea
 Comment: 
 
-Filename: fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/H_.glif
+Filename: fontmake-3.7.1/tests/data/MutatorSansLite/MutatorSansLightCondensed.ufo/glyphs.support.crossbars/contents.plist
 Comment: 
 
-Filename: fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/S_.glif
+Filename: fontmake-3.7.1/tests/data/MutatorSansLite/MutatorSansLightCondensed.ufo/glyphs.support.crossbars/E_.glif
 Comment: 
 
-Filename: fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/acute.glif
+Filename: fontmake-3.7.1/tests/data/MutatorSansLite/MutatorSansLightCondensed.ufo/glyphs.support.crossbars/layerinfo.plist
 Comment: 
 
-Filename: fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/layerinfo.plist
+Filename: fontmake-3.7.1/tests/data/MutatorSansLite/MutatorSansLightCondensed.ufo/glyphs.support.S_.wide/S_.glif
 Comment: 
 
-Filename: fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/period.glif
+Filename: fontmake-3.7.1/tests/data/MutatorSansLite/MutatorSansLightCondensed.ufo/glyphs.support.S_.wide/contents.plist
 Comment: 
 
-Filename: fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/E_.glif
+Filename: fontmake-3.7.1/tests/data/MutatorSansLite/MutatorSansLightCondensed.ufo/glyphs.support.S_.wide/layerinfo.plist
 Comment: 
 
-Filename: fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/quotesinglbase.glif
+Filename: fontmake-3.7.1/tests/data/MutatorSansLite/MutatorSansLightCondensed.ufo/glyphs.support.S_.wide/S_.closed.glif
 Comment: 
 
-Filename: fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/arrowup.glif
+Filename: fontmake-3.7.1/tests/data/MutatorSansLite/MutatorSansLightCondensed.ufo/glyphs.support.S_.middle/contents.plist
 Comment: 
 
-Filename: fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs.master_width_695.65_weight_166.38/contents.plist
+Filename: fontmake-3.7.1/tests/data/MutatorSansLite/MutatorSansLightCondensed.ufo/glyphs.support.S_.middle/layerinfo.plist
 Comment: 
 
-Filename: fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs.master_width_695.65_weight_166.38/layerinfo.plist
+Filename: fontmake-3.7.1/tests/data/MutatorSansLite/MutatorSansLightCondensed.ufo/glyphs.support.S_.middle/S_.closed.glif
 Comment: 
 
-Filename: fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansIntermediateCondensed.ufo/glyphs.background/
+Filename: fontmake-3.7.1/tests/data/MutatorSansLite/MutatorSansLightCondensed.ufo/glyphs.background/S_.glif
 Comment: 
 
-Filename: fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansIntermediateCondensed.ufo/glyphs.reference.interpolation/
+Filename: fontmake-3.7.1/tests/data/MutatorSansLite/MutatorSansLightCondensed.ufo/glyphs.background/contents.plist
 Comment: 
 
-Filename: fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansIntermediateCondensed.ufo/glyphs/
+Filename: fontmake-3.7.1/tests/data/MutatorSansLite/MutatorSansLightCondensed.ufo/glyphs.background/layerinfo.plist
 Comment: 
 
-Filename: fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansIntermediateCondensed.ufo/glyphs.interpolation/
+Filename: fontmake-3.7.1/tests/data/MutatorSansLite/MutatorSansLightCondensed.ufo/glyphs.background/S_.closed.glif
 Comment: 
 
-Filename: fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansIntermediateCondensed.ufo/features.fea
+Filename: fontmake-3.7.1/tests/data/MutatorSansLite/MutatorSansLightCondensed.ufo/glyphs/S_.glif
 Comment: 
 
-Filename: fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansIntermediateCondensed.ufo/layercontents.plist
+Filename: fontmake-3.7.1/tests/data/MutatorSansLite/MutatorSansLightCondensed.ufo/glyphs/I_.narrow.glif
 Comment: 
 
-Filename: fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansIntermediateCondensed.ufo/fontinfo.plist
+Filename: fontmake-3.7.1/tests/data/MutatorSansLite/MutatorSansLightCondensed.ufo/glyphs/contents.plist
 Comment: 
 
-Filename: fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansIntermediateCondensed.ufo/metainfo.plist
+Filename: fontmake-3.7.1/tests/data/MutatorSansLite/MutatorSansLightCondensed.ufo/glyphs/I_.glif
 Comment: 
 
-Filename: fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansIntermediateCondensed.ufo/lib.plist
+Filename: fontmake-3.7.1/tests/data/MutatorSansLite/MutatorSansLightCondensed.ufo/glyphs/A_.glif
 Comment: 
 
-Filename: fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansIntermediateCondensed.ufo/glyphs.background/contents.plist
+Filename: fontmake-3.7.1/tests/data/MutatorSansLite/MutatorSansLightCondensed.ufo/glyphs/I_J_.glif
 Comment: 
 
-Filename: fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansIntermediateCondensed.ufo/glyphs.background/S_.glif
+Filename: fontmake-3.7.1/tests/data/MutatorSansLite/MutatorSansLightCondensed.ufo/glyphs/layerinfo.plist
 Comment: 
 
-Filename: fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansIntermediateCondensed.ufo/glyphs.background/layerinfo.plist
+Filename: fontmake-3.7.1/tests/data/MutatorSansLite/MutatorSansLightCondensed.ufo/glyphs/S_.closed.glif
 Comment: 
 
-Filename: fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansIntermediateCondensed.ufo/glyphs.reference.interpolation/contents.plist
+Filename: fontmake-3.7.1/tests/data/MutatorSansLite/MutatorSansLightCondensed.ufo/glyphs.support.crossbar/S_.glif
 Comment: 
 
-Filename: fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansIntermediateCondensed.ufo/glyphs.reference.interpolation/S_.glif
+Filename: fontmake-3.7.1/tests/data/MutatorSansLite/MutatorSansLightCondensed.ufo/glyphs.support.crossbar/contents.plist
 Comment: 
 
-Filename: fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansIntermediateCondensed.ufo/glyphs.reference.interpolation/layerinfo.plist
+Filename: fontmake-3.7.1/tests/data/MutatorSansLite/MutatorSansLightCondensed.ufo/glyphs.support.crossbar/layerinfo.plist
 Comment: 
 
-Filename: fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansIntermediateCondensed.ufo/glyphs.reference.interpolation/E_.glif
+Filename: fontmake-3.7.1/tests/data/MutatorSansLite/MutatorSansLightCondensed.ufo/glyphs.support/S_.glif
 Comment: 
 
-Filename: fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansIntermediateCondensed.ufo/glyphs/G_.glif
+Filename: fontmake-3.7.1/tests/data/MutatorSansLite/MutatorSansLightCondensed.ufo/glyphs.support/contents.plist
 Comment: 
 
-Filename: fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansIntermediateCondensed.ufo/glyphs/F_.glif
+Filename: fontmake-3.7.1/tests/data/MutatorSansLite/MutatorSansLightCondensed.ufo/glyphs.support/A_.glif
 Comment: 
 
-Filename: fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansIntermediateCondensed.ufo/glyphs/B_.glif
+Filename: fontmake-3.7.1/tests/data/MutatorSansLite/MutatorSansLightCondensed.ufo/glyphs.support/layerinfo.plist
 Comment: 
 
-Filename: fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansIntermediateCondensed.ufo/glyphs/contents.plist
+Filename: fontmake-3.7.1/tests/data/MutatorSansLite/MutatorSerifLightCondensed.ufo/glyphs/
 Comment: 
 
-Filename: fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansIntermediateCondensed.ufo/glyphs/S_.glif
+Filename: fontmake-3.7.1/tests/data/MutatorSansLite/MutatorSerifLightCondensed.ufo/metainfo.plist
 Comment: 
 
-Filename: fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansIntermediateCondensed.ufo/glyphs/layerinfo.plist
+Filename: fontmake-3.7.1/tests/data/MutatorSansLite/MutatorSerifLightCondensed.ufo/fontinfo.plist
 Comment: 
 
-Filename: fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansIntermediateCondensed.ufo/glyphs/E_.glif
+Filename: fontmake-3.7.1/tests/data/MutatorSansLite/MutatorSerifLightCondensed.ufo/layercontents.plist
 Comment: 
 
-Filename: fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansIntermediateCondensed.ufo/glyphs.interpolation/contents.plist
+Filename: fontmake-3.7.1/tests/data/MutatorSansLite/MutatorSerifLightCondensed.ufo/lib.plist
 Comment: 
 
-Filename: fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansIntermediateCondensed.ufo/glyphs.interpolation/layerinfo.plist
+Filename: fontmake-3.7.1/tests/data/MutatorSansLite/MutatorSerifLightCondensed.ufo/features.fea
 Comment: 
 
-Filename: fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansIntermediateCondensed.ufo/glyphs.interpolation/E_.glif
+Filename: fontmake-3.7.1/tests/data/MutatorSansLite/MutatorSerifLightCondensed.ufo/glyphs/contents.plist
 Comment: 
 
-Filename: fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs.background/
+Filename: fontmake-3.7.1/tests/data/MutatorSansLite/MutatorSerifLightCondensed.ufo/glyphs/A_.glif
 Comment: 
 
-Filename: fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/
+Filename: fontmake-3.7.1/tests/data/InstantiatorStrictMathGlyph/SquareTwo.ufo/
 Comment: 
 
-Filename: fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/features.fea
+Filename: fontmake-3.7.1/tests/data/InstantiatorStrictMathGlyph/SquareOne.ufo/
 Comment: 
 
-Filename: fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/layercontents.plist
+Filename: fontmake-3.7.1/tests/data/InstantiatorStrictMathGlyph/StrictMathGlyph.designspace
 Comment: 
 
-Filename: fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/groups.plist
+Filename: fontmake-3.7.1/tests/data/InstantiatorStrictMathGlyph/SquareTwo.ufo/glyphs/
 Comment: 
 
-Filename: fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/kerning.plist
+Filename: fontmake-3.7.1/tests/data/InstantiatorStrictMathGlyph/SquareTwo.ufo/metainfo.plist
 Comment: 
 
-Filename: fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/fontinfo.plist
+Filename: fontmake-3.7.1/tests/data/InstantiatorStrictMathGlyph/SquareTwo.ufo/fontinfo.plist
 Comment: 
 
-Filename: fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/metainfo.plist
+Filename: fontmake-3.7.1/tests/data/InstantiatorStrictMathGlyph/SquareTwo.ufo/layercontents.plist
 Comment: 
 
-Filename: fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/lib.plist
+Filename: fontmake-3.7.1/tests/data/InstantiatorStrictMathGlyph/SquareTwo.ufo/lib.plist
 Comment: 
 
-Filename: fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs.background/S_.closed.glif
+Filename: fontmake-3.7.1/tests/data/InstantiatorStrictMathGlyph/SquareTwo.ufo/glyphs/test.glif
 Comment: 
 
-Filename: fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs.background/contents.plist
+Filename: fontmake-3.7.1/tests/data/InstantiatorStrictMathGlyph/SquareTwo.ufo/glyphs/contents.plist
 Comment: 
 
-Filename: fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs.background/layerinfo.plist
+Filename: fontmake-3.7.1/tests/data/InstantiatorStrictMathGlyph/SquareTwo.ufo/glyphs/layerinfo.plist
 Comment: 
 
-Filename: fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/W_.glif
+Filename: fontmake-3.7.1/tests/data/InstantiatorStrictMathGlyph/SquareOne.ufo/glyphs/
 Comment: 
 
-Filename: fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/quotedblleft.glif
+Filename: fontmake-3.7.1/tests/data/InstantiatorStrictMathGlyph/SquareOne.ufo/metainfo.plist
 Comment: 
 
-Filename: fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/T_.glif
+Filename: fontmake-3.7.1/tests/data/InstantiatorStrictMathGlyph/SquareOne.ufo/fontinfo.plist
 Comment: 
 
-Filename: fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/R_.glif
+Filename: fontmake-3.7.1/tests/data/InstantiatorStrictMathGlyph/SquareOne.ufo/layercontents.plist
 Comment: 
 
-Filename: fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/O_.glif
+Filename: fontmake-3.7.1/tests/data/InstantiatorStrictMathGlyph/SquareOne.ufo/lib.plist
 Comment: 
 
-Filename: fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/G_.glif
+Filename: fontmake-3.7.1/tests/data/InstantiatorStrictMathGlyph/SquareOne.ufo/glyphs/test.glif
 Comment: 
 
-Filename: fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/D_.glif
+Filename: fontmake-3.7.1/tests/data/InstantiatorStrictMathGlyph/SquareOne.ufo/glyphs/contents.plist
 Comment: 
 
-Filename: fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/S_.closed.glif
+Filename: fontmake-3.7.1/tests/data/InstantiatorStrictMathGlyph/SquareOne.ufo/glyphs/layerinfo.plist
 Comment: 
 
-Filename: fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/colon.glif
+Filename: fontmake-3.7.1/tests/data/MutatorSans/MutatorSansLightWide.ufo/
 Comment: 
 
-Filename: fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/X_.glif
+Filename: fontmake-3.7.1/tests/data/MutatorSans/MutatorSansBoldWide.ufo/
 Comment: 
 
-Filename: fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/M_.glif
+Filename: fontmake-3.7.1/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/
 Comment: 
 
-Filename: fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/Z_.glif
+Filename: fontmake-3.7.1/tests/data/MutatorSans/MutatorSansIntermediateCondensed.ufo/
 Comment: 
 
-Filename: fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/I_.narrow.glif
+Filename: fontmake-3.7.1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/
 Comment: 
 
-Filename: fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/F_.glif
+Filename: fontmake-3.7.1/tests/data/MutatorSans/MutatorSansIntermediateWide.ufo/
 Comment: 
 
-Filename: fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/C_.glif
+Filename: fontmake-3.7.1/tests/data/MutatorSans/MutatorSans-width-only.designspace
 Comment: 
 
-Filename: fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/dot.glif
+Filename: fontmake-3.7.1/tests/data/MutatorSans/LICENSE
 Comment: 
 
-Filename: fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/arrowright.glif
+Filename: fontmake-3.7.1/tests/data/MutatorSans/MutatorSans-weight-only.designspace
 Comment: 
 
-Filename: fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/B_.glif
+Filename: fontmake-3.7.1/tests/data/MutatorSans/MutatorSans_no_default.designspace
 Comment: 
 
-Filename: fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/U_.glif
+Filename: fontmake-3.7.1/tests/data/MutatorSans/MutatorSans_missing.designspace
 Comment: 
 
-Filename: fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/I_.glif
+Filename: fontmake-3.7.1/tests/data/MutatorSans/MutatorSans-with-openNodes.designspace
 Comment: 
 
-Filename: fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/N_.glif
+Filename: fontmake-3.7.1/tests/data/MutatorSans/MutatorSans.designspace
 Comment: 
 
-Filename: fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/V_.glif
+Filename: fontmake-3.7.1/tests/data/MutatorSans/MutatorSans-non-default-layer.designspace
 Comment: 
 
-Filename: fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/I_J_.glif
+Filename: fontmake-3.7.1/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs.master_width_720.00_weight_645.00/
 Comment: 
 
-Filename: fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/comma.glif
+Filename: fontmake-3.7.1/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs.background/
 Comment: 
 
-Filename: fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/contents.plist
+Filename: fontmake-3.7.1/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/
 Comment: 
 
-Filename: fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/dieresis.glif
+Filename: fontmake-3.7.1/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs.master_width_695.65_weight_166.38/
 Comment: 
 
-Filename: fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/Y_.glif
+Filename: fontmake-3.7.1/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs.master_width_0.00_weight_0.00/
 Comment: 
 
-Filename: fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/Q_.glif
+Filename: fontmake-3.7.1/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs.master_width_500.00_weight_500.00/
 Comment: 
 
-Filename: fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/space.glif
+Filename: fontmake-3.7.1/tests/data/MutatorSans/MutatorSansLightWide.ufo/metainfo.plist
 Comment: 
 
-Filename: fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/quotedblbase.glif
+Filename: fontmake-3.7.1/tests/data/MutatorSans/MutatorSansLightWide.ufo/kerning.plist
 Comment: 
 
-Filename: fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/L_.glif
+Filename: fontmake-3.7.1/tests/data/MutatorSans/MutatorSansLightWide.ufo/groups.plist
 Comment: 
 
-Filename: fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/quotedblright.glif
+Filename: fontmake-3.7.1/tests/data/MutatorSans/MutatorSansLightWide.ufo/fontinfo.plist
 Comment: 
 
-Filename: fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/A_acute.glif
+Filename: fontmake-3.7.1/tests/data/MutatorSans/MutatorSansLightWide.ufo/layercontents.plist
 Comment: 
 
-Filename: fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/arrowdown.glif
+Filename: fontmake-3.7.1/tests/data/MutatorSans/MutatorSansLightWide.ufo/lib.plist
 Comment: 
 
-Filename: fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/P_.glif
+Filename: fontmake-3.7.1/tests/data/MutatorSans/MutatorSansLightWide.ufo/features.fea
 Comment: 
 
-Filename: fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/semicolon.glif
+Filename: fontmake-3.7.1/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs.master_width_720.00_weight_645.00/S_.glif
 Comment: 
 
-Filename: fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/J_.narrow.glif
+Filename: fontmake-3.7.1/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs.master_width_720.00_weight_645.00/contents.plist
 Comment: 
 
-Filename: fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/A_dieresis.glif
+Filename: fontmake-3.7.1/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs.master_width_720.00_weight_645.00/layerinfo.plist
 Comment: 
 
-Filename: fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/arrowleft.glif
+Filename: fontmake-3.7.1/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs.background/contents.plist
 Comment: 
 
-Filename: fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/K_.glif
+Filename: fontmake-3.7.1/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs.background/layerinfo.plist
 Comment: 
 
-Filename: fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/A_.glif
+Filename: fontmake-3.7.1/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs.background/S_.closed.glif
 Comment: 
 
-Filename: fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/J_.glif
+Filename: fontmake-3.7.1/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/arrowup.glif
 Comment: 
 
-Filename: fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/H_.glif
+Filename: fontmake-3.7.1/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/Y_.glif
 Comment: 
 
-Filename: fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/S_.glif
+Filename: fontmake-3.7.1/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/Z_.glif
 Comment: 
 
-Filename: fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/acute.glif
+Filename: fontmake-3.7.1/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/J_.narrow.glif
 Comment: 
 
-Filename: fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/layerinfo.plist
+Filename: fontmake-3.7.1/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/T_.glif
 Comment: 
 
-Filename: fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/period.glif
+Filename: fontmake-3.7.1/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/A_acute.glif
 Comment: 
 
-Filename: fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/E_.glif
+Filename: fontmake-3.7.1/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/C_.glif
 Comment: 
 
-Filename: fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/quotesinglbase.glif
+Filename: fontmake-3.7.1/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/arrowleft.glif
 Comment: 
 
-Filename: fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/arrowup.glif
+Filename: fontmake-3.7.1/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/semicolon.glif
 Comment: 
 
-Filename: fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansIntermediateWide.ufo/glyphs.background/
+Filename: fontmake-3.7.1/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/period.glif
 Comment: 
 
-Filename: fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansIntermediateWide.ufo/glyphs/
+Filename: fontmake-3.7.1/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/acute.glif
 Comment: 
 
-Filename: fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansIntermediateWide.ufo/features.fea
+Filename: fontmake-3.7.1/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/L_.glif
 Comment: 
 
-Filename: fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansIntermediateWide.ufo/layercontents.plist
+Filename: fontmake-3.7.1/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/S_.glif
 Comment: 
 
-Filename: fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansIntermediateWide.ufo/kerning.plist
+Filename: fontmake-3.7.1/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/quotesinglbase.glif
 Comment: 
 
-Filename: fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansIntermediateWide.ufo/fontinfo.plist
+Filename: fontmake-3.7.1/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/quotedblright.glif
 Comment: 
 
-Filename: fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansIntermediateWide.ufo/metainfo.plist
+Filename: fontmake-3.7.1/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/B_.glif
 Comment: 
 
-Filename: fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansIntermediateWide.ufo/lib.plist
+Filename: fontmake-3.7.1/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/P_.glif
 Comment: 
 
-Filename: fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansIntermediateWide.ufo/glyphs.background/contents.plist
+Filename: fontmake-3.7.1/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/arrowdown.glif
 Comment: 
 
-Filename: fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansIntermediateWide.ufo/glyphs.background/S_.glif
+Filename: fontmake-3.7.1/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/W_.glif
 Comment: 
 
-Filename: fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansIntermediateWide.ufo/glyphs.background/layerinfo.plist
+Filename: fontmake-3.7.1/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/comma.glif
 Comment: 
 
-Filename: fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansIntermediateWide.ufo/glyphs/G_.glif
+Filename: fontmake-3.7.1/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/dieresis.glif
 Comment: 
 
-Filename: fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansIntermediateWide.ufo/glyphs/F_.glif
+Filename: fontmake-3.7.1/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/quotedblleft.glif
 Comment: 
 
-Filename: fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansIntermediateWide.ufo/glyphs/B_.glif
+Filename: fontmake-3.7.1/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/F_.glif
 Comment: 
 
-Filename: fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansIntermediateWide.ufo/glyphs/contents.plist
+Filename: fontmake-3.7.1/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/O_.glif
 Comment: 
 
-Filename: fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansIntermediateWide.ufo/glyphs/layerinfo.plist
+Filename: fontmake-3.7.1/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/A_dieresis.glif
 Comment: 
 
-Filename: fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansIntermediateWide.ufo/glyphs/E_.glif
+Filename: fontmake-3.7.1/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/quotedblbase.glif
 Comment: 
 
-Filename: fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs.background/
+Filename: fontmake-3.7.1/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/space.glif
 Comment: 
 
-Filename: fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/
+Filename: fontmake-3.7.1/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/arrowright.glif
 Comment: 
 
-Filename: fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansBoldWide.ufo/features.fea
+Filename: fontmake-3.7.1/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/I_.narrow.glif
 Comment: 
 
-Filename: fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansBoldWide.ufo/layercontents.plist
+Filename: fontmake-3.7.1/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/contents.plist
 Comment: 
 
-Filename: fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansBoldWide.ufo/groups.plist
+Filename: fontmake-3.7.1/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/H_.glif
 Comment: 
 
-Filename: fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansBoldWide.ufo/kerning.plist
+Filename: fontmake-3.7.1/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/Q_.glif
 Comment: 
 
-Filename: fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansBoldWide.ufo/fontinfo.plist
+Filename: fontmake-3.7.1/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/E_.glif
 Comment: 
 
-Filename: fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansBoldWide.ufo/metainfo.plist
+Filename: fontmake-3.7.1/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/J_.glif
 Comment: 
 
-Filename: fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansBoldWide.ufo/lib.plist
+Filename: fontmake-3.7.1/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/D_.glif
 Comment: 
 
-Filename: fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs.background/S_.closed.glif
+Filename: fontmake-3.7.1/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/G_.glif
 Comment: 
 
-Filename: fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs.background/contents.plist
+Filename: fontmake-3.7.1/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/K_.glif
 Comment: 
 
-Filename: fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs.background/S_.glif
+Filename: fontmake-3.7.1/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/I_.glif
 Comment: 
 
-Filename: fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs.background/layerinfo.plist
+Filename: fontmake-3.7.1/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/A_.glif
 Comment: 
 
-Filename: fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/W_.glif
+Filename: fontmake-3.7.1/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/M_.glif
 Comment: 
 
-Filename: fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/quotedblleft.glif
+Filename: fontmake-3.7.1/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/I_J_.glif
 Comment: 
 
-Filename: fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/T_.glif
+Filename: fontmake-3.7.1/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/V_.glif
 Comment: 
 
-Filename: fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/R_.glif
+Filename: fontmake-3.7.1/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/X_.glif
 Comment: 
 
-Filename: fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/O_.glif
+Filename: fontmake-3.7.1/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/layerinfo.plist
 Comment: 
 
-Filename: fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/G_.glif
+Filename: fontmake-3.7.1/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/N_.glif
 Comment: 
 
-Filename: fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/D_.glif
+Filename: fontmake-3.7.1/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/colon.glif
 Comment: 
 
-Filename: fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/S_.closed.glif
+Filename: fontmake-3.7.1/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/dot.glif
 Comment: 
 
-Filename: fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/colon.glif
+Filename: fontmake-3.7.1/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/R_.glif
 Comment: 
 
-Filename: fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/X_.glif
+Filename: fontmake-3.7.1/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/S_.closed.glif
 Comment: 
 
-Filename: fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/M_.glif
+Filename: fontmake-3.7.1/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/U_.glif
 Comment: 
 
-Filename: fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/Z_.glif
+Filename: fontmake-3.7.1/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs.master_width_695.65_weight_166.38/contents.plist
 Comment: 
 
-Filename: fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/I_.narrow.glif
+Filename: fontmake-3.7.1/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs.master_width_695.65_weight_166.38/layerinfo.plist
 Comment: 
 
-Filename: fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/F_.glif
+Filename: fontmake-3.7.1/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs.master_width_0.00_weight_0.00/contents.plist
 Comment: 
 
-Filename: fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/C_.glif
+Filename: fontmake-3.7.1/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs.master_width_0.00_weight_0.00/layerinfo.plist
 Comment: 
 
-Filename: fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/dot.glif
+Filename: fontmake-3.7.1/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs.master_width_500.00_weight_500.00/S_.glif
 Comment: 
 
-Filename: fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/arrowright.glif
+Filename: fontmake-3.7.1/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs.master_width_500.00_weight_500.00/contents.plist
 Comment: 
 
-Filename: fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/B_.glif
+Filename: fontmake-3.7.1/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs.master_width_500.00_weight_500.00/layerinfo.plist
 Comment: 
 
-Filename: fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/U_.glif
+Filename: fontmake-3.7.1/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs.background/
 Comment: 
 
-Filename: fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/I_.glif
+Filename: fontmake-3.7.1/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/
 Comment: 
 
-Filename: fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/N_.glif
+Filename: fontmake-3.7.1/tests/data/MutatorSans/MutatorSansBoldWide.ufo/metainfo.plist
 Comment: 
 
-Filename: fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/V_.glif
+Filename: fontmake-3.7.1/tests/data/MutatorSans/MutatorSansBoldWide.ufo/kerning.plist
 Comment: 
 
-Filename: fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/I_J_.glif
+Filename: fontmake-3.7.1/tests/data/MutatorSans/MutatorSansBoldWide.ufo/groups.plist
 Comment: 
 
-Filename: fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/comma.glif
+Filename: fontmake-3.7.1/tests/data/MutatorSans/MutatorSansBoldWide.ufo/fontinfo.plist
 Comment: 
 
-Filename: fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/contents.plist
+Filename: fontmake-3.7.1/tests/data/MutatorSans/MutatorSansBoldWide.ufo/layercontents.plist
 Comment: 
 
-Filename: fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/dieresis.glif
+Filename: fontmake-3.7.1/tests/data/MutatorSans/MutatorSansBoldWide.ufo/lib.plist
 Comment: 
 
-Filename: fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/Y_.glif
+Filename: fontmake-3.7.1/tests/data/MutatorSans/MutatorSansBoldWide.ufo/features.fea
 Comment: 
 
-Filename: fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/Q_.glif
+Filename: fontmake-3.7.1/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs.background/S_.glif
 Comment: 
 
-Filename: fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/space.glif
+Filename: fontmake-3.7.1/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs.background/contents.plist
 Comment: 
 
-Filename: fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/quotedblbase.glif
+Filename: fontmake-3.7.1/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs.background/layerinfo.plist
 Comment: 
 
-Filename: fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/L_.glif
+Filename: fontmake-3.7.1/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs.background/S_.closed.glif
 Comment: 
 
-Filename: fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/quotedblright.glif
+Filename: fontmake-3.7.1/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/arrowup.glif
 Comment: 
 
-Filename: fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/A_acute.glif
+Filename: fontmake-3.7.1/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/Y_.glif
 Comment: 
 
-Filename: fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/arrowdown.glif
+Filename: fontmake-3.7.1/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/Z_.glif
 Comment: 
 
-Filename: fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/P_.glif
+Filename: fontmake-3.7.1/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/J_.narrow.glif
 Comment: 
 
-Filename: fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/semicolon.glif
+Filename: fontmake-3.7.1/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/T_.glif
 Comment: 
 
-Filename: fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/J_.narrow.glif
+Filename: fontmake-3.7.1/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/A_acute.glif
 Comment: 
 
-Filename: fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/A_dieresis.glif
+Filename: fontmake-3.7.1/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/C_.glif
 Comment: 
 
-Filename: fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/arrowleft.glif
+Filename: fontmake-3.7.1/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/arrowleft.glif
 Comment: 
 
-Filename: fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/K_.glif
+Filename: fontmake-3.7.1/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/semicolon.glif
 Comment: 
 
-Filename: fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/A_.glif
+Filename: fontmake-3.7.1/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/period.glif
 Comment: 
 
-Filename: fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/J_.glif
+Filename: fontmake-3.7.1/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/acute.glif
 Comment: 
 
-Filename: fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/H_.glif
+Filename: fontmake-3.7.1/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/L_.glif
 Comment: 
 
-Filename: fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/S_.glif
+Filename: fontmake-3.7.1/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/S_.glif
 Comment: 
 
-Filename: fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/acute.glif
+Filename: fontmake-3.7.1/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/quotesinglbase.glif
 Comment: 
 
-Filename: fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/layerinfo.plist
+Filename: fontmake-3.7.1/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/quotedblright.glif
 Comment: 
 
-Filename: fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/period.glif
+Filename: fontmake-3.7.1/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/B_.glif
 Comment: 
 
-Filename: fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/E_.glif
+Filename: fontmake-3.7.1/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/P_.glif
 Comment: 
 
-Filename: fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/quotesinglbase.glif
+Filename: fontmake-3.7.1/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/arrowdown.glif
 Comment: 
 
-Filename: fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/arrowup.glif
+Filename: fontmake-3.7.1/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/W_.glif
 Comment: 
 
-Filename: fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs.background/
+Filename: fontmake-3.7.1/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/comma.glif
 Comment: 
 
-Filename: fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs.support.crossbar/
+Filename: fontmake-3.7.1/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/dieresis.glif
 Comment: 
 
-Filename: fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs.support/
+Filename: fontmake-3.7.1/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/quotedblleft.glif
 Comment: 
 
-Filename: fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs.support.S_.middle/
+Filename: fontmake-3.7.1/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/F_.glif
 Comment: 
 
-Filename: fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/
+Filename: fontmake-3.7.1/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/O_.glif
 Comment: 
 
-Filename: fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs.support.crossbars/
+Filename: fontmake-3.7.1/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/A_dieresis.glif
 Comment: 
 
-Filename: fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs.support.S_.wide/
+Filename: fontmake-3.7.1/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/quotedblbase.glif
 Comment: 
 
-Filename: fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/features.fea
+Filename: fontmake-3.7.1/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/space.glif
 Comment: 
 
-Filename: fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/layercontents.plist
+Filename: fontmake-3.7.1/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/arrowright.glif
 Comment: 
 
-Filename: fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/groups.plist
+Filename: fontmake-3.7.1/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/I_.narrow.glif
 Comment: 
 
-Filename: fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/kerning.plist
+Filename: fontmake-3.7.1/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/contents.plist
 Comment: 
 
-Filename: fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/fontinfo.plist
+Filename: fontmake-3.7.1/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/H_.glif
 Comment: 
 
-Filename: fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/metainfo.plist
+Filename: fontmake-3.7.1/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/Q_.glif
 Comment: 
 
-Filename: fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/lib.plist
+Filename: fontmake-3.7.1/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/E_.glif
 Comment: 
 
-Filename: fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs.background/S_.closed.glif
+Filename: fontmake-3.7.1/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/J_.glif
 Comment: 
 
-Filename: fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs.background/contents.plist
+Filename: fontmake-3.7.1/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/D_.glif
 Comment: 
 
-Filename: fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs.background/S_.glif
+Filename: fontmake-3.7.1/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/G_.glif
 Comment: 
 
-Filename: fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs.background/layerinfo.plist
+Filename: fontmake-3.7.1/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/K_.glif
 Comment: 
 
-Filename: fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs.support.crossbar/G_.glif
+Filename: fontmake-3.7.1/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/I_.glif
 Comment: 
 
-Filename: fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs.support.crossbar/S_.closed.glif
+Filename: fontmake-3.7.1/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/A_.glif
 Comment: 
 
-Filename: fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs.support.crossbar/F_.glif
+Filename: fontmake-3.7.1/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/M_.glif
 Comment: 
 
-Filename: fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs.support.crossbar/B_.glif
+Filename: fontmake-3.7.1/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/I_J_.glif
 Comment: 
 
-Filename: fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs.support.crossbar/contents.plist
+Filename: fontmake-3.7.1/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/V_.glif
 Comment: 
 
-Filename: fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs.support.crossbar/S_.glif
+Filename: fontmake-3.7.1/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/X_.glif
 Comment: 
 
-Filename: fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs.support.crossbar/layerinfo.plist
+Filename: fontmake-3.7.1/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/layerinfo.plist
 Comment: 
 
-Filename: fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs.support.crossbar/E_.glif
+Filename: fontmake-3.7.1/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/N_.glif
 Comment: 
 
-Filename: fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs.support/W_.glif
+Filename: fontmake-3.7.1/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/colon.glif
 Comment: 
 
-Filename: fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs.support/contents.plist
+Filename: fontmake-3.7.1/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/dot.glif
 Comment: 
 
-Filename: fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs.support/A_.glif
+Filename: fontmake-3.7.1/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/R_.glif
 Comment: 
 
-Filename: fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs.support/S_.glif
+Filename: fontmake-3.7.1/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/S_.closed.glif
 Comment: 
 
-Filename: fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs.support/layerinfo.plist
+Filename: fontmake-3.7.1/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/U_.glif
 Comment: 
 
-Filename: fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs.support.S_.middle/S_.closed.glif
+Filename: fontmake-3.7.1/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs.background/
 Comment: 
 
-Filename: fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs.support.S_.middle/contents.plist
+Filename: fontmake-3.7.1/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/
 Comment: 
 
-Filename: fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs.support.S_.middle/layerinfo.plist
+Filename: fontmake-3.7.1/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/metainfo.plist
 Comment: 
 
-Filename: fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/W_.glif
+Filename: fontmake-3.7.1/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/kerning.plist
 Comment: 
 
-Filename: fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/quotedblleft.glif
+Filename: fontmake-3.7.1/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/groups.plist
 Comment: 
 
-Filename: fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/T_.glif
+Filename: fontmake-3.7.1/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/fontinfo.plist
 Comment: 
 
-Filename: fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/R_.glif
+Filename: fontmake-3.7.1/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/layercontents.plist
 Comment: 
 
-Filename: fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/O_.glif
+Filename: fontmake-3.7.1/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/lib.plist
 Comment: 
 
-Filename: fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/G_.glif
+Filename: fontmake-3.7.1/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/features.fea
 Comment: 
 
-Filename: fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/D_.glif
+Filename: fontmake-3.7.1/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs.background/contents.plist
 Comment: 
 
-Filename: fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/S_.closed.glif
+Filename: fontmake-3.7.1/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs.background/layerinfo.plist
 Comment: 
 
-Filename: fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/colon.glif
+Filename: fontmake-3.7.1/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs.background/S_.closed.glif
 Comment: 
 
-Filename: fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/X_.glif
+Filename: fontmake-3.7.1/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/arrowup.glif
 Comment: 
 
-Filename: fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/M_.glif
+Filename: fontmake-3.7.1/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/Y_.glif
 Comment: 
 
-Filename: fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/Z_.glif
+Filename: fontmake-3.7.1/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/Z_.glif
 Comment: 
 
-Filename: fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/I_.narrow.glif
+Filename: fontmake-3.7.1/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/J_.narrow.glif
 Comment: 
 
-Filename: fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/F_.glif
+Filename: fontmake-3.7.1/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/T_.glif
 Comment: 
 
-Filename: fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/C_.glif
+Filename: fontmake-3.7.1/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/A_acute.glif
 Comment: 
 
-Filename: fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/dot.glif
+Filename: fontmake-3.7.1/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/C_.glif
 Comment: 
 
-Filename: fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/arrowright.glif
+Filename: fontmake-3.7.1/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/arrowleft.glif
 Comment: 
 
-Filename: fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/B_.glif
+Filename: fontmake-3.7.1/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/semicolon.glif
 Comment: 
 
-Filename: fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/U_.glif
+Filename: fontmake-3.7.1/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/period.glif
 Comment: 
 
-Filename: fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/I_.glif
+Filename: fontmake-3.7.1/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/acute.glif
 Comment: 
 
-Filename: fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/N_.glif
+Filename: fontmake-3.7.1/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/L_.glif
 Comment: 
 
-Filename: fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/V_.glif
+Filename: fontmake-3.7.1/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/S_.glif
 Comment: 
 
-Filename: fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/I_J_.glif
+Filename: fontmake-3.7.1/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/quotesinglbase.glif
 Comment: 
 
-Filename: fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/comma.glif
+Filename: fontmake-3.7.1/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/quotedblright.glif
 Comment: 
 
-Filename: fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/contents.plist
+Filename: fontmake-3.7.1/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/B_.glif
 Comment: 
 
-Filename: fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/dieresis.glif
+Filename: fontmake-3.7.1/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/P_.glif
 Comment: 
 
-Filename: fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/Y_.glif
+Filename: fontmake-3.7.1/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/arrowdown.glif
 Comment: 
 
-Filename: fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/Q_.glif
+Filename: fontmake-3.7.1/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/W_.glif
 Comment: 
 
-Filename: fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/space.glif
+Filename: fontmake-3.7.1/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/comma.glif
 Comment: 
 
-Filename: fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/quotedblbase.glif
+Filename: fontmake-3.7.1/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/dieresis.glif
 Comment: 
 
-Filename: fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/L_.glif
+Filename: fontmake-3.7.1/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/quotedblleft.glif
 Comment: 
 
-Filename: fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/quotedblright.glif
+Filename: fontmake-3.7.1/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/F_.glif
 Comment: 
 
-Filename: fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/A_acute.glif
+Filename: fontmake-3.7.1/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/O_.glif
 Comment: 
 
-Filename: fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/arrowdown.glif
+Filename: fontmake-3.7.1/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/A_dieresis.glif
 Comment: 
 
-Filename: fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/P_.glif
+Filename: fontmake-3.7.1/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/quotedblbase.glif
 Comment: 
 
-Filename: fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/semicolon.glif
+Filename: fontmake-3.7.1/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/space.glif
 Comment: 
 
-Filename: fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/J_.narrow.glif
+Filename: fontmake-3.7.1/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/arrowright.glif
 Comment: 
 
-Filename: fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/A_dieresis.glif
+Filename: fontmake-3.7.1/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/I_.narrow.glif
 Comment: 
 
-Filename: fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/arrowleft.glif
+Filename: fontmake-3.7.1/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/contents.plist
 Comment: 
 
-Filename: fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/K_.glif
+Filename: fontmake-3.7.1/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/H_.glif
 Comment: 
 
-Filename: fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/A_.glif
+Filename: fontmake-3.7.1/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/Q_.glif
 Comment: 
 
-Filename: fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/J_.glif
+Filename: fontmake-3.7.1/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/E_.glif
 Comment: 
 
-Filename: fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/H_.glif
+Filename: fontmake-3.7.1/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/J_.glif
 Comment: 
 
-Filename: fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/S_.glif
+Filename: fontmake-3.7.1/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/D_.glif
 Comment: 
 
-Filename: fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/acute.glif
+Filename: fontmake-3.7.1/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/G_.glif
 Comment: 
 
-Filename: fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/layerinfo.plist
+Filename: fontmake-3.7.1/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/K_.glif
 Comment: 
 
-Filename: fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/period.glif
+Filename: fontmake-3.7.1/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/I_.glif
 Comment: 
 
-Filename: fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/E_.glif
+Filename: fontmake-3.7.1/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/A_.glif
 Comment: 
 
-Filename: fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/quotesinglbase.glif
+Filename: fontmake-3.7.1/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/M_.glif
 Comment: 
 
-Filename: fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/arrowup.glif
+Filename: fontmake-3.7.1/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/I_J_.glif
 Comment: 
 
-Filename: fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs.support.crossbars/contents.plist
+Filename: fontmake-3.7.1/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/V_.glif
 Comment: 
 
-Filename: fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs.support.crossbars/layerinfo.plist
+Filename: fontmake-3.7.1/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/X_.glif
 Comment: 
 
-Filename: fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs.support.crossbars/E_.glif
+Filename: fontmake-3.7.1/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/layerinfo.plist
 Comment: 
 
-Filename: fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs.support.S_.wide/S_.closed.glif
+Filename: fontmake-3.7.1/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/N_.glif
 Comment: 
 
-Filename: fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs.support.S_.wide/contents.plist
+Filename: fontmake-3.7.1/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/colon.glif
 Comment: 
 
-Filename: fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs.support.S_.wide/S_.glif
+Filename: fontmake-3.7.1/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/dot.glif
 Comment: 
 
-Filename: fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs.support.S_.wide/layerinfo.plist
+Filename: fontmake-3.7.1/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/R_.glif
 Comment: 
 
-Filename: fontmake-3.7.0b3/tests/data/MutatorSansLite/MutatorSansLightWide.ufo/
+Filename: fontmake-3.7.1/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/S_.closed.glif
 Comment: 
 
-Filename: fontmake-3.7.0b3/tests/data/MutatorSansLite/MutatorSerifLightWide.ufo/
+Filename: fontmake-3.7.1/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/U_.glif
 Comment: 
 
-Filename: fontmake-3.7.0b3/tests/data/MutatorSansLite/MutatorSansBoldCondensed.ufo/
+Filename: fontmake-3.7.1/tests/data/MutatorSans/MutatorSansIntermediateCondensed.ufo/glyphs.reference.interpolation/
 Comment: 
 
-Filename: fontmake-3.7.0b3/tests/data/MutatorSansLite/MutatorSerifLightCondensed.ufo/
+Filename: fontmake-3.7.1/tests/data/MutatorSans/MutatorSansIntermediateCondensed.ufo/glyphs.background/
 Comment: 
 
-Filename: fontmake-3.7.0b3/tests/data/MutatorSansLite/MutatorSansBoldWide.ufo/
+Filename: fontmake-3.7.1/tests/data/MutatorSans/MutatorSansIntermediateCondensed.ufo/glyphs/
 Comment: 
 
-Filename: fontmake-3.7.0b3/tests/data/MutatorSansLite/MutatorSansLightCondensed.ufo/
+Filename: fontmake-3.7.1/tests/data/MutatorSans/MutatorSansIntermediateCondensed.ufo/glyphs.interpolation/
 Comment: 
 
-Filename: fontmake-3.7.0b3/tests/data/MutatorSansLite/MutatorSans_v5_several_vfs.designspace
+Filename: fontmake-3.7.1/tests/data/MutatorSans/MutatorSansIntermediateCondensed.ufo/metainfo.plist
 Comment: 
 
-Filename: fontmake-3.7.0b3/tests/data/MutatorSansLite/MutatorSans_v5_several_vfs_discrete_axis.designspace
+Filename: fontmake-3.7.1/tests/data/MutatorSans/MutatorSansIntermediateCondensed.ufo/fontinfo.plist
 Comment: 
 
-Filename: fontmake-3.7.0b3/tests/data/MutatorSansLite/MutatorSans_v5_implicit_one_vf.designspace
+Filename: fontmake-3.7.1/tests/data/MutatorSans/MutatorSansIntermediateCondensed.ufo/layercontents.plist
 Comment: 
 
-Filename: fontmake-3.7.0b3/tests/data/MutatorSansLite/LICENSE
+Filename: fontmake-3.7.1/tests/data/MutatorSans/MutatorSansIntermediateCondensed.ufo/lib.plist
 Comment: 
 
-Filename: fontmake-3.7.0b3/tests/data/MutatorSansLite/MutatorFamily_v5_discrete_axis.designspace
+Filename: fontmake-3.7.1/tests/data/MutatorSans/MutatorSansIntermediateCondensed.ufo/features.fea
 Comment: 
 
-Filename: fontmake-3.7.0b3/tests/data/MutatorSansLite/MutatorSansLightWide.ufo/glyphs.background/
+Filename: fontmake-3.7.1/tests/data/MutatorSans/MutatorSansIntermediateCondensed.ufo/glyphs.reference.interpolation/S_.glif
 Comment: 
 
-Filename: fontmake-3.7.0b3/tests/data/MutatorSansLite/MutatorSansLightWide.ufo/glyphs.master_width_720.00_weight_645.00/
+Filename: fontmake-3.7.1/tests/data/MutatorSans/MutatorSansIntermediateCondensed.ufo/glyphs.reference.interpolation/contents.plist
 Comment: 
 
-Filename: fontmake-3.7.0b3/tests/data/MutatorSansLite/MutatorSansLightWide.ufo/glyphs.master_width_0.00_weight_0.00/
+Filename: fontmake-3.7.1/tests/data/MutatorSans/MutatorSansIntermediateCondensed.ufo/glyphs.reference.interpolation/E_.glif
 Comment: 
 
-Filename: fontmake-3.7.0b3/tests/data/MutatorSansLite/MutatorSansLightWide.ufo/glyphs.master_width_500.00_weight_500.00/
+Filename: fontmake-3.7.1/tests/data/MutatorSans/MutatorSansIntermediateCondensed.ufo/glyphs.reference.interpolation/layerinfo.plist
 Comment: 
 
-Filename: fontmake-3.7.0b3/tests/data/MutatorSansLite/MutatorSansLightWide.ufo/glyphs/
+Filename: fontmake-3.7.1/tests/data/MutatorSans/MutatorSansIntermediateCondensed.ufo/glyphs.background/S_.glif
 Comment: 
 
-Filename: fontmake-3.7.0b3/tests/data/MutatorSansLite/MutatorSansLightWide.ufo/glyphs.master_width_695.65_weight_166.38/
+Filename: fontmake-3.7.1/tests/data/MutatorSans/MutatorSansIntermediateCondensed.ufo/glyphs.background/contents.plist
 Comment: 
 
-Filename: fontmake-3.7.0b3/tests/data/MutatorSansLite/MutatorSansLightWide.ufo/features.fea
+Filename: fontmake-3.7.1/tests/data/MutatorSans/MutatorSansIntermediateCondensed.ufo/glyphs.background/layerinfo.plist
 Comment: 
 
-Filename: fontmake-3.7.0b3/tests/data/MutatorSansLite/MutatorSansLightWide.ufo/layercontents.plist
+Filename: fontmake-3.7.1/tests/data/MutatorSans/MutatorSansIntermediateCondensed.ufo/glyphs/S_.glif
 Comment: 
 
-Filename: fontmake-3.7.0b3/tests/data/MutatorSansLite/MutatorSansLightWide.ufo/fontinfo.plist
+Filename: fontmake-3.7.1/tests/data/MutatorSans/MutatorSansIntermediateCondensed.ufo/glyphs/B_.glif
 Comment: 
 
-Filename: fontmake-3.7.0b3/tests/data/MutatorSansLite/MutatorSansLightWide.ufo/metainfo.plist
+Filename: fontmake-3.7.1/tests/data/MutatorSans/MutatorSansIntermediateCondensed.ufo/glyphs/F_.glif
 Comment: 
 
-Filename: fontmake-3.7.0b3/tests/data/MutatorSansLite/MutatorSansLightWide.ufo/lib.plist
+Filename: fontmake-3.7.1/tests/data/MutatorSans/MutatorSansIntermediateCondensed.ufo/glyphs/contents.plist
 Comment: 
 
-Filename: fontmake-3.7.0b3/tests/data/MutatorSansLite/MutatorSansLightWide.ufo/glyphs.background/S_.closed.glif
+Filename: fontmake-3.7.1/tests/data/MutatorSans/MutatorSansIntermediateCondensed.ufo/glyphs/E_.glif
 Comment: 
 
-Filename: fontmake-3.7.0b3/tests/data/MutatorSansLite/MutatorSansLightWide.ufo/glyphs.background/contents.plist
+Filename: fontmake-3.7.1/tests/data/MutatorSans/MutatorSansIntermediateCondensed.ufo/glyphs/G_.glif
 Comment: 
 
-Filename: fontmake-3.7.0b3/tests/data/MutatorSansLite/MutatorSansLightWide.ufo/glyphs.background/layerinfo.plist
+Filename: fontmake-3.7.1/tests/data/MutatorSans/MutatorSansIntermediateCondensed.ufo/glyphs/layerinfo.plist
 Comment: 
 
-Filename: fontmake-3.7.0b3/tests/data/MutatorSansLite/MutatorSansLightWide.ufo/glyphs.master_width_720.00_weight_645.00/contents.plist
+Filename: fontmake-3.7.1/tests/data/MutatorSans/MutatorSansIntermediateCondensed.ufo/glyphs.interpolation/contents.plist
 Comment: 
 
-Filename: fontmake-3.7.0b3/tests/data/MutatorSansLite/MutatorSansLightWide.ufo/glyphs.master_width_720.00_weight_645.00/S_.glif
+Filename: fontmake-3.7.1/tests/data/MutatorSans/MutatorSansIntermediateCondensed.ufo/glyphs.interpolation/E_.glif
 Comment: 
 
-Filename: fontmake-3.7.0b3/tests/data/MutatorSansLite/MutatorSansLightWide.ufo/glyphs.master_width_720.00_weight_645.00/layerinfo.plist
+Filename: fontmake-3.7.1/tests/data/MutatorSans/MutatorSansIntermediateCondensed.ufo/glyphs.interpolation/layerinfo.plist
 Comment: 
 
-Filename: fontmake-3.7.0b3/tests/data/MutatorSansLite/MutatorSansLightWide.ufo/glyphs.master_width_0.00_weight_0.00/contents.plist
+Filename: fontmake-3.7.1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs.support.crossbars/
 Comment: 
 
-Filename: fontmake-3.7.0b3/tests/data/MutatorSansLite/MutatorSansLightWide.ufo/glyphs.master_width_0.00_weight_0.00/layerinfo.plist
+Filename: fontmake-3.7.1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs.support.S_.wide/
 Comment: 
 
-Filename: fontmake-3.7.0b3/tests/data/MutatorSansLite/MutatorSansLightWide.ufo/glyphs.master_width_500.00_weight_500.00/contents.plist
+Filename: fontmake-3.7.1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs.support.S_.middle/
 Comment: 
 
-Filename: fontmake-3.7.0b3/tests/data/MutatorSansLite/MutatorSansLightWide.ufo/glyphs.master_width_500.00_weight_500.00/S_.glif
+Filename: fontmake-3.7.1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs.background/
 Comment: 
 
-Filename: fontmake-3.7.0b3/tests/data/MutatorSansLite/MutatorSansLightWide.ufo/glyphs.master_width_500.00_weight_500.00/layerinfo.plist
+Filename: fontmake-3.7.1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/
 Comment: 
 
-Filename: fontmake-3.7.0b3/tests/data/MutatorSansLite/MutatorSansLightWide.ufo/glyphs/S_.closed.glif
+Filename: fontmake-3.7.1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs.support.crossbar/
 Comment: 
 
-Filename: fontmake-3.7.0b3/tests/data/MutatorSansLite/MutatorSansLightWide.ufo/glyphs/I_.narrow.glif
+Filename: fontmake-3.7.1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs.support/
 Comment: 
 
-Filename: fontmake-3.7.0b3/tests/data/MutatorSansLite/MutatorSansLightWide.ufo/glyphs/I_.glif
+Filename: fontmake-3.7.1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/metainfo.plist
 Comment: 
 
-Filename: fontmake-3.7.0b3/tests/data/MutatorSansLite/MutatorSansLightWide.ufo/glyphs/I_J_.glif
+Filename: fontmake-3.7.1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/kerning.plist
 Comment: 
 
-Filename: fontmake-3.7.0b3/tests/data/MutatorSansLite/MutatorSansLightWide.ufo/glyphs/contents.plist
+Filename: fontmake-3.7.1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/groups.plist
 Comment: 
 
-Filename: fontmake-3.7.0b3/tests/data/MutatorSansLite/MutatorSansLightWide.ufo/glyphs/A_.glif
+Filename: fontmake-3.7.1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/fontinfo.plist
 Comment: 
 
-Filename: fontmake-3.7.0b3/tests/data/MutatorSansLite/MutatorSansLightWide.ufo/glyphs/S_.glif
+Filename: fontmake-3.7.1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/layercontents.plist
 Comment: 
 
-Filename: fontmake-3.7.0b3/tests/data/MutatorSansLite/MutatorSansLightWide.ufo/glyphs/layerinfo.plist
+Filename: fontmake-3.7.1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/lib.plist
 Comment: 
 
-Filename: fontmake-3.7.0b3/tests/data/MutatorSansLite/MutatorSansLightWide.ufo/glyphs.master_width_695.65_weight_166.38/contents.plist
+Filename: fontmake-3.7.1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/features.fea
 Comment: 
 
-Filename: fontmake-3.7.0b3/tests/data/MutatorSansLite/MutatorSansLightWide.ufo/glyphs.master_width_695.65_weight_166.38/layerinfo.plist
+Filename: fontmake-3.7.1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs.support.crossbars/contents.plist
 Comment: 
 
-Filename: fontmake-3.7.0b3/tests/data/MutatorSansLite/MutatorSerifLightWide.ufo/glyphs/
+Filename: fontmake-3.7.1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs.support.crossbars/E_.glif
 Comment: 
 
-Filename: fontmake-3.7.0b3/tests/data/MutatorSansLite/MutatorSerifLightWide.ufo/features.fea
+Filename: fontmake-3.7.1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs.support.crossbars/layerinfo.plist
 Comment: 
 
-Filename: fontmake-3.7.0b3/tests/data/MutatorSansLite/MutatorSerifLightWide.ufo/layercontents.plist
+Filename: fontmake-3.7.1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs.support.S_.wide/S_.glif
 Comment: 
 
-Filename: fontmake-3.7.0b3/tests/data/MutatorSansLite/MutatorSerifLightWide.ufo/fontinfo.plist
+Filename: fontmake-3.7.1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs.support.S_.wide/contents.plist
 Comment: 
 
-Filename: fontmake-3.7.0b3/tests/data/MutatorSansLite/MutatorSerifLightWide.ufo/metainfo.plist
+Filename: fontmake-3.7.1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs.support.S_.wide/layerinfo.plist
 Comment: 
 
-Filename: fontmake-3.7.0b3/tests/data/MutatorSansLite/MutatorSerifLightWide.ufo/lib.plist
+Filename: fontmake-3.7.1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs.support.S_.wide/S_.closed.glif
 Comment: 
 
-Filename: fontmake-3.7.0b3/tests/data/MutatorSansLite/MutatorSerifLightWide.ufo/glyphs/contents.plist
+Filename: fontmake-3.7.1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs.support.S_.middle/contents.plist
 Comment: 
 
-Filename: fontmake-3.7.0b3/tests/data/MutatorSansLite/MutatorSerifLightWide.ufo/glyphs/A_.glif
+Filename: fontmake-3.7.1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs.support.S_.middle/layerinfo.plist
 Comment: 
 
-Filename: fontmake-3.7.0b3/tests/data/MutatorSansLite/MutatorSansBoldCondensed.ufo/glyphs.background/
+Filename: fontmake-3.7.1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs.support.S_.middle/S_.closed.glif
 Comment: 
 
-Filename: fontmake-3.7.0b3/tests/data/MutatorSansLite/MutatorSansBoldCondensed.ufo/glyphs/
+Filename: fontmake-3.7.1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs.background/S_.glif
 Comment: 
 
-Filename: fontmake-3.7.0b3/tests/data/MutatorSansLite/MutatorSansBoldCondensed.ufo/features.fea
+Filename: fontmake-3.7.1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs.background/contents.plist
 Comment: 
 
-Filename: fontmake-3.7.0b3/tests/data/MutatorSansLite/MutatorSansBoldCondensed.ufo/layercontents.plist
+Filename: fontmake-3.7.1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs.background/layerinfo.plist
 Comment: 
 
-Filename: fontmake-3.7.0b3/tests/data/MutatorSansLite/MutatorSansBoldCondensed.ufo/fontinfo.plist
+Filename: fontmake-3.7.1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs.background/S_.closed.glif
 Comment: 
 
-Filename: fontmake-3.7.0b3/tests/data/MutatorSansLite/MutatorSansBoldCondensed.ufo/metainfo.plist
+Filename: fontmake-3.7.1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/arrowup.glif
 Comment: 
 
-Filename: fontmake-3.7.0b3/tests/data/MutatorSansLite/MutatorSansBoldCondensed.ufo/lib.plist
+Filename: fontmake-3.7.1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/Y_.glif
 Comment: 
 
-Filename: fontmake-3.7.0b3/tests/data/MutatorSansLite/MutatorSansBoldCondensed.ufo/glyphs.background/S_.closed.glif
+Filename: fontmake-3.7.1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/Z_.glif
 Comment: 
 
-Filename: fontmake-3.7.0b3/tests/data/MutatorSansLite/MutatorSansBoldCondensed.ufo/glyphs.background/contents.plist
+Filename: fontmake-3.7.1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/J_.narrow.glif
 Comment: 
 
-Filename: fontmake-3.7.0b3/tests/data/MutatorSansLite/MutatorSansBoldCondensed.ufo/glyphs.background/layerinfo.plist
+Filename: fontmake-3.7.1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/T_.glif
 Comment: 
 
-Filename: fontmake-3.7.0b3/tests/data/MutatorSansLite/MutatorSansBoldCondensed.ufo/glyphs/S_.closed.glif
+Filename: fontmake-3.7.1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/A_acute.glif
 Comment: 
 
-Filename: fontmake-3.7.0b3/tests/data/MutatorSansLite/MutatorSansBoldCondensed.ufo/glyphs/I_.narrow.glif
+Filename: fontmake-3.7.1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/C_.glif
 Comment: 
 
-Filename: fontmake-3.7.0b3/tests/data/MutatorSansLite/MutatorSansBoldCondensed.ufo/glyphs/I_.glif
+Filename: fontmake-3.7.1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/arrowleft.glif
 Comment: 
 
-Filename: fontmake-3.7.0b3/tests/data/MutatorSansLite/MutatorSansBoldCondensed.ufo/glyphs/I_J_.glif
+Filename: fontmake-3.7.1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/semicolon.glif
 Comment: 
 
-Filename: fontmake-3.7.0b3/tests/data/MutatorSansLite/MutatorSansBoldCondensed.ufo/glyphs/contents.plist
+Filename: fontmake-3.7.1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/period.glif
 Comment: 
 
-Filename: fontmake-3.7.0b3/tests/data/MutatorSansLite/MutatorSansBoldCondensed.ufo/glyphs/A_.glif
+Filename: fontmake-3.7.1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/acute.glif
 Comment: 
 
-Filename: fontmake-3.7.0b3/tests/data/MutatorSansLite/MutatorSansBoldCondensed.ufo/glyphs/S_.glif
+Filename: fontmake-3.7.1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/L_.glif
 Comment: 
 
-Filename: fontmake-3.7.0b3/tests/data/MutatorSansLite/MutatorSansBoldCondensed.ufo/glyphs/layerinfo.plist
+Filename: fontmake-3.7.1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/S_.glif
 Comment: 
 
-Filename: fontmake-3.7.0b3/tests/data/MutatorSansLite/MutatorSerifLightCondensed.ufo/glyphs/
+Filename: fontmake-3.7.1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/quotesinglbase.glif
 Comment: 
 
-Filename: fontmake-3.7.0b3/tests/data/MutatorSansLite/MutatorSerifLightCondensed.ufo/features.fea
+Filename: fontmake-3.7.1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/quotedblright.glif
 Comment: 
 
-Filename: fontmake-3.7.0b3/tests/data/MutatorSansLite/MutatorSerifLightCondensed.ufo/layercontents.plist
+Filename: fontmake-3.7.1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/B_.glif
 Comment: 
 
-Filename: fontmake-3.7.0b3/tests/data/MutatorSansLite/MutatorSerifLightCondensed.ufo/fontinfo.plist
+Filename: fontmake-3.7.1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/P_.glif
 Comment: 
 
-Filename: fontmake-3.7.0b3/tests/data/MutatorSansLite/MutatorSerifLightCondensed.ufo/metainfo.plist
+Filename: fontmake-3.7.1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/arrowdown.glif
 Comment: 
 
-Filename: fontmake-3.7.0b3/tests/data/MutatorSansLite/MutatorSerifLightCondensed.ufo/lib.plist
+Filename: fontmake-3.7.1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/W_.glif
 Comment: 
 
-Filename: fontmake-3.7.0b3/tests/data/MutatorSansLite/MutatorSerifLightCondensed.ufo/glyphs/contents.plist
+Filename: fontmake-3.7.1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/comma.glif
 Comment: 
 
-Filename: fontmake-3.7.0b3/tests/data/MutatorSansLite/MutatorSerifLightCondensed.ufo/glyphs/A_.glif
+Filename: fontmake-3.7.1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/dieresis.glif
 Comment: 
 
-Filename: fontmake-3.7.0b3/tests/data/MutatorSansLite/MutatorSansBoldWide.ufo/glyphs.background/
+Filename: fontmake-3.7.1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/quotedblleft.glif
 Comment: 
 
-Filename: fontmake-3.7.0b3/tests/data/MutatorSansLite/MutatorSansBoldWide.ufo/glyphs/
+Filename: fontmake-3.7.1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/F_.glif
 Comment: 
 
-Filename: fontmake-3.7.0b3/tests/data/MutatorSansLite/MutatorSansBoldWide.ufo/features.fea
+Filename: fontmake-3.7.1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/O_.glif
 Comment: 
 
-Filename: fontmake-3.7.0b3/tests/data/MutatorSansLite/MutatorSansBoldWide.ufo/layercontents.plist
+Filename: fontmake-3.7.1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/A_dieresis.glif
 Comment: 
 
-Filename: fontmake-3.7.0b3/tests/data/MutatorSansLite/MutatorSansBoldWide.ufo/fontinfo.plist
+Filename: fontmake-3.7.1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/quotedblbase.glif
 Comment: 
 
-Filename: fontmake-3.7.0b3/tests/data/MutatorSansLite/MutatorSansBoldWide.ufo/metainfo.plist
+Filename: fontmake-3.7.1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/space.glif
 Comment: 
 
-Filename: fontmake-3.7.0b3/tests/data/MutatorSansLite/MutatorSansBoldWide.ufo/lib.plist
+Filename: fontmake-3.7.1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/arrowright.glif
 Comment: 
 
-Filename: fontmake-3.7.0b3/tests/data/MutatorSansLite/MutatorSansBoldWide.ufo/glyphs.background/S_.closed.glif
+Filename: fontmake-3.7.1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/I_.narrow.glif
 Comment: 
 
-Filename: fontmake-3.7.0b3/tests/data/MutatorSansLite/MutatorSansBoldWide.ufo/glyphs.background/contents.plist
+Filename: fontmake-3.7.1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/contents.plist
 Comment: 
 
-Filename: fontmake-3.7.0b3/tests/data/MutatorSansLite/MutatorSansBoldWide.ufo/glyphs.background/S_.glif
+Filename: fontmake-3.7.1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/H_.glif
 Comment: 
 
-Filename: fontmake-3.7.0b3/tests/data/MutatorSansLite/MutatorSansBoldWide.ufo/glyphs.background/layerinfo.plist
+Filename: fontmake-3.7.1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/Q_.glif
 Comment: 
 
-Filename: fontmake-3.7.0b3/tests/data/MutatorSansLite/MutatorSansBoldWide.ufo/glyphs/S_.closed.glif
+Filename: fontmake-3.7.1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/E_.glif
 Comment: 
 
-Filename: fontmake-3.7.0b3/tests/data/MutatorSansLite/MutatorSansBoldWide.ufo/glyphs/I_.narrow.glif
+Filename: fontmake-3.7.1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/J_.glif
 Comment: 
 
-Filename: fontmake-3.7.0b3/tests/data/MutatorSansLite/MutatorSansBoldWide.ufo/glyphs/I_.glif
+Filename: fontmake-3.7.1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/D_.glif
 Comment: 
 
-Filename: fontmake-3.7.0b3/tests/data/MutatorSansLite/MutatorSansBoldWide.ufo/glyphs/I_J_.glif
+Filename: fontmake-3.7.1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/G_.glif
 Comment: 
 
-Filename: fontmake-3.7.0b3/tests/data/MutatorSansLite/MutatorSansBoldWide.ufo/glyphs/contents.plist
+Filename: fontmake-3.7.1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/K_.glif
 Comment: 
 
-Filename: fontmake-3.7.0b3/tests/data/MutatorSansLite/MutatorSansBoldWide.ufo/glyphs/A_.glif
+Filename: fontmake-3.7.1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/I_.glif
 Comment: 
 
-Filename: fontmake-3.7.0b3/tests/data/MutatorSansLite/MutatorSansBoldWide.ufo/glyphs/S_.glif
+Filename: fontmake-3.7.1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/A_.glif
 Comment: 
 
-Filename: fontmake-3.7.0b3/tests/data/MutatorSansLite/MutatorSansBoldWide.ufo/glyphs/layerinfo.plist
+Filename: fontmake-3.7.1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/M_.glif
 Comment: 
 
-Filename: fontmake-3.7.0b3/tests/data/MutatorSansLite/MutatorSansLightCondensed.ufo/glyphs.background/
+Filename: fontmake-3.7.1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/I_J_.glif
 Comment: 
 
-Filename: fontmake-3.7.0b3/tests/data/MutatorSansLite/MutatorSansLightCondensed.ufo/glyphs.support.crossbar/
+Filename: fontmake-3.7.1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/V_.glif
 Comment: 
 
-Filename: fontmake-3.7.0b3/tests/data/MutatorSansLite/MutatorSansLightCondensed.ufo/glyphs.support/
+Filename: fontmake-3.7.1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/X_.glif
 Comment: 
 
-Filename: fontmake-3.7.0b3/tests/data/MutatorSansLite/MutatorSansLightCondensed.ufo/glyphs.support.S_.middle/
+Filename: fontmake-3.7.1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/layerinfo.plist
 Comment: 
 
-Filename: fontmake-3.7.0b3/tests/data/MutatorSansLite/MutatorSansLightCondensed.ufo/glyphs/
+Filename: fontmake-3.7.1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/N_.glif
 Comment: 
 
-Filename: fontmake-3.7.0b3/tests/data/MutatorSansLite/MutatorSansLightCondensed.ufo/glyphs.support.crossbars/
+Filename: fontmake-3.7.1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/colon.glif
 Comment: 
 
-Filename: fontmake-3.7.0b3/tests/data/MutatorSansLite/MutatorSansLightCondensed.ufo/glyphs.support.S_.wide/
+Filename: fontmake-3.7.1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/dot.glif
 Comment: 
 
-Filename: fontmake-3.7.0b3/tests/data/MutatorSansLite/MutatorSansLightCondensed.ufo/features.fea
+Filename: fontmake-3.7.1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/R_.glif
 Comment: 
 
-Filename: fontmake-3.7.0b3/tests/data/MutatorSansLite/MutatorSansLightCondensed.ufo/layercontents.plist
+Filename: fontmake-3.7.1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/S_.closed.glif
 Comment: 
 
-Filename: fontmake-3.7.0b3/tests/data/MutatorSansLite/MutatorSansLightCondensed.ufo/fontinfo.plist
+Filename: fontmake-3.7.1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/U_.glif
 Comment: 
 
-Filename: fontmake-3.7.0b3/tests/data/MutatorSansLite/MutatorSansLightCondensed.ufo/metainfo.plist
+Filename: fontmake-3.7.1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs.support.crossbar/S_.glif
 Comment: 
 
-Filename: fontmake-3.7.0b3/tests/data/MutatorSansLite/MutatorSansLightCondensed.ufo/lib.plist
+Filename: fontmake-3.7.1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs.support.crossbar/B_.glif
 Comment: 
 
-Filename: fontmake-3.7.0b3/tests/data/MutatorSansLite/MutatorSansLightCondensed.ufo/glyphs.background/S_.closed.glif
+Filename: fontmake-3.7.1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs.support.crossbar/F_.glif
 Comment: 
 
-Filename: fontmake-3.7.0b3/tests/data/MutatorSansLite/MutatorSansLightCondensed.ufo/glyphs.background/contents.plist
+Filename: fontmake-3.7.1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs.support.crossbar/contents.plist
 Comment: 
 
-Filename: fontmake-3.7.0b3/tests/data/MutatorSansLite/MutatorSansLightCondensed.ufo/glyphs.background/S_.glif
+Filename: fontmake-3.7.1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs.support.crossbar/E_.glif
 Comment: 
 
-Filename: fontmake-3.7.0b3/tests/data/MutatorSansLite/MutatorSansLightCondensed.ufo/glyphs.background/layerinfo.plist
+Filename: fontmake-3.7.1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs.support.crossbar/G_.glif
 Comment: 
 
-Filename: fontmake-3.7.0b3/tests/data/MutatorSansLite/MutatorSansLightCondensed.ufo/glyphs.support.crossbar/contents.plist
+Filename: fontmake-3.7.1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs.support.crossbar/layerinfo.plist
 Comment: 
 
-Filename: fontmake-3.7.0b3/tests/data/MutatorSansLite/MutatorSansLightCondensed.ufo/glyphs.support.crossbar/S_.glif
+Filename: fontmake-3.7.1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs.support.crossbar/S_.closed.glif
 Comment: 
 
-Filename: fontmake-3.7.0b3/tests/data/MutatorSansLite/MutatorSansLightCondensed.ufo/glyphs.support.crossbar/layerinfo.plist
+Filename: fontmake-3.7.1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs.support/S_.glif
 Comment: 
 
-Filename: fontmake-3.7.0b3/tests/data/MutatorSansLite/MutatorSansLightCondensed.ufo/glyphs.support/contents.plist
+Filename: fontmake-3.7.1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs.support/W_.glif
 Comment: 
 
-Filename: fontmake-3.7.0b3/tests/data/MutatorSansLite/MutatorSansLightCondensed.ufo/glyphs.support/A_.glif
+Filename: fontmake-3.7.1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs.support/contents.plist
 Comment: 
 
-Filename: fontmake-3.7.0b3/tests/data/MutatorSansLite/MutatorSansLightCondensed.ufo/glyphs.support/S_.glif
+Filename: fontmake-3.7.1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs.support/A_.glif
 Comment: 
 
-Filename: fontmake-3.7.0b3/tests/data/MutatorSansLite/MutatorSansLightCondensed.ufo/glyphs.support/layerinfo.plist
+Filename: fontmake-3.7.1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs.support/layerinfo.plist
 Comment: 
 
-Filename: fontmake-3.7.0b3/tests/data/MutatorSansLite/MutatorSansLightCondensed.ufo/glyphs.support.S_.middle/S_.closed.glif
+Filename: fontmake-3.7.1/tests/data/MutatorSans/MutatorSansIntermediateWide.ufo/glyphs.background/
 Comment: 
 
-Filename: fontmake-3.7.0b3/tests/data/MutatorSansLite/MutatorSansLightCondensed.ufo/glyphs.support.S_.middle/contents.plist
+Filename: fontmake-3.7.1/tests/data/MutatorSans/MutatorSansIntermediateWide.ufo/glyphs/
 Comment: 
 
-Filename: fontmake-3.7.0b3/tests/data/MutatorSansLite/MutatorSansLightCondensed.ufo/glyphs.support.S_.middle/layerinfo.plist
+Filename: fontmake-3.7.1/tests/data/MutatorSans/MutatorSansIntermediateWide.ufo/metainfo.plist
 Comment: 
 
-Filename: fontmake-3.7.0b3/tests/data/MutatorSansLite/MutatorSansLightCondensed.ufo/glyphs/S_.closed.glif
+Filename: fontmake-3.7.1/tests/data/MutatorSans/MutatorSansIntermediateWide.ufo/kerning.plist
 Comment: 
 
-Filename: fontmake-3.7.0b3/tests/data/MutatorSansLite/MutatorSansLightCondensed.ufo/glyphs/I_.narrow.glif
+Filename: fontmake-3.7.1/tests/data/MutatorSans/MutatorSansIntermediateWide.ufo/fontinfo.plist
 Comment: 
 
-Filename: fontmake-3.7.0b3/tests/data/MutatorSansLite/MutatorSansLightCondensed.ufo/glyphs/I_.glif
+Filename: fontmake-3.7.1/tests/data/MutatorSans/MutatorSansIntermediateWide.ufo/layercontents.plist
 Comment: 
 
-Filename: fontmake-3.7.0b3/tests/data/MutatorSansLite/MutatorSansLightCondensed.ufo/glyphs/I_J_.glif
+Filename: fontmake-3.7.1/tests/data/MutatorSans/MutatorSansIntermediateWide.ufo/lib.plist
 Comment: 
 
-Filename: fontmake-3.7.0b3/tests/data/MutatorSansLite/MutatorSansLightCondensed.ufo/glyphs/contents.plist
+Filename: fontmake-3.7.1/tests/data/MutatorSans/MutatorSansIntermediateWide.ufo/features.fea
 Comment: 
 
-Filename: fontmake-3.7.0b3/tests/data/MutatorSansLite/MutatorSansLightCondensed.ufo/glyphs/A_.glif
+Filename: fontmake-3.7.1/tests/data/MutatorSans/MutatorSansIntermediateWide.ufo/glyphs.background/S_.glif
 Comment: 
 
-Filename: fontmake-3.7.0b3/tests/data/MutatorSansLite/MutatorSansLightCondensed.ufo/glyphs/S_.glif
+Filename: fontmake-3.7.1/tests/data/MutatorSans/MutatorSansIntermediateWide.ufo/glyphs.background/contents.plist
 Comment: 
 
-Filename: fontmake-3.7.0b3/tests/data/MutatorSansLite/MutatorSansLightCondensed.ufo/glyphs/layerinfo.plist
+Filename: fontmake-3.7.1/tests/data/MutatorSans/MutatorSansIntermediateWide.ufo/glyphs.background/layerinfo.plist
 Comment: 
 
-Filename: fontmake-3.7.0b3/tests/data/MutatorSansLite/MutatorSansLightCondensed.ufo/glyphs.support.crossbars/contents.plist
+Filename: fontmake-3.7.1/tests/data/MutatorSans/MutatorSansIntermediateWide.ufo/glyphs/B_.glif
 Comment: 
 
-Filename: fontmake-3.7.0b3/tests/data/MutatorSansLite/MutatorSansLightCondensed.ufo/glyphs.support.crossbars/layerinfo.plist
+Filename: fontmake-3.7.1/tests/data/MutatorSans/MutatorSansIntermediateWide.ufo/glyphs/F_.glif
 Comment: 
 
-Filename: fontmake-3.7.0b3/tests/data/MutatorSansLite/MutatorSansLightCondensed.ufo/glyphs.support.crossbars/E_.glif
+Filename: fontmake-3.7.1/tests/data/MutatorSans/MutatorSansIntermediateWide.ufo/glyphs/contents.plist
 Comment: 
 
-Filename: fontmake-3.7.0b3/tests/data/MutatorSansLite/MutatorSansLightCondensed.ufo/glyphs.support.S_.wide/S_.closed.glif
+Filename: fontmake-3.7.1/tests/data/MutatorSans/MutatorSansIntermediateWide.ufo/glyphs/E_.glif
 Comment: 
 
-Filename: fontmake-3.7.0b3/tests/data/MutatorSansLite/MutatorSansLightCondensed.ufo/glyphs.support.S_.wide/contents.plist
+Filename: fontmake-3.7.1/tests/data/MutatorSans/MutatorSansIntermediateWide.ufo/glyphs/G_.glif
 Comment: 
 
-Filename: fontmake-3.7.0b3/tests/data/MutatorSansLite/MutatorSansLightCondensed.ufo/glyphs.support.S_.wide/S_.glif
+Filename: fontmake-3.7.1/tests/data/MutatorSans/MutatorSansIntermediateWide.ufo/glyphs/layerinfo.plist
 Comment: 
 
-Filename: fontmake-3.7.0b3/tests/data/MutatorSansLite/MutatorSansLightCondensed.ufo/glyphs.support.S_.wide/layerinfo.plist
+Filename: fontmake-3.7.1/tests/data/AutohintingTest/Padyakke.glyphs
 Comment: 
 
 Zip file comment:
```

## Comparing `fontmake-3.7.0b3/build_pyz.sh` & `fontmake-3.7.1/build_pyz.sh`

 * *Files identical despite different names*

## Comparing `fontmake-3.7.0b3/PKG-INFO` & `fontmake-3.7.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fontmake
-Version: 3.7.0b3
+Version: 3.7.1
 Summary: Compile fonts from sources (UFO, Glyphs) to binary (OpenType, TrueType).
 Home-page: https://github.com/googlei18n/fontmake
 License: Apache Software License 2.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
```

## Comparing `fontmake-3.7.0b3/TROUBLESHOOTING.md` & `fontmake-3.7.1/TROUBLESHOOTING.md`

 * *Files identical despite different names*

## Comparing `fontmake-3.7.0b3/.gitignore` & `fontmake-3.7.1/.gitignore`

 * *Files identical despite different names*

## Comparing `fontmake-3.7.0b3/LICENSE` & `fontmake-3.7.1/LICENSE`

 * *Files identical despite different names*

## Comparing `fontmake-3.7.0b3/USAGE.md` & `fontmake-3.7.1/USAGE.md`

 * *Files identical despite different names*

## Comparing `fontmake-3.7.0b3/README.md` & `fontmake-3.7.1/README.md`

 * *Files identical despite different names*

## Comparing `fontmake-3.7.0b3/setup.py` & `fontmake-3.7.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -27,17 +27,17 @@
 with open("README.md", "r", encoding="utf-8") as f:
     long_description = f.read()
 
 
 dep_versions = {
     "attrs": ">=19",
     "fontMath": ">=0.9.3",
-    "fonttools": ">=4.41.1",
+    "fonttools": ">=4.42.0",
     "glyphsLib": ">=6.2.5",
-    "ufo2ft": ">=2.33.2",
+    "ufo2ft": ">=2.33.4",
     "ufoLib2": ">=0.16.0",
 }
 
 dep_extras = {
     "fonttools": {
         "implementation_name == 'cpython'": "ufo,lxml,unicode",
         "implementation_name != 'cpython'": "ufo,unicode",
```

## Comparing `fontmake-3.7.0b3/tox.ini` & `fontmake-3.7.1/tox.ini`

 * *Files identical despite different names*

## Comparing `fontmake-3.7.0b3/.coveragerc` & `fontmake-3.7.1/.coveragerc`

 * *Files identical despite different names*

## Comparing `fontmake-3.7.0b3/CONTRIBUTING.md` & `fontmake-3.7.1/CONTRIBUTING.md`

 * *Files identical despite different names*

## Comparing `fontmake-3.7.0b3/Lib/fontmake/compatibility.py` & `fontmake-3.7.1/Lib/fontmake/compatibility.py`

 * *Files identical despite different names*

## Comparing `fontmake-3.7.0b3/Lib/fontmake/instantiator.py` & `fontmake-3.7.1/Lib/fontmake/instantiator.py`

 * *Files identical despite different names*

## Comparing `fontmake-3.7.0b3/Lib/fontmake/errors.py` & `fontmake-3.7.1/Lib/fontmake/errors.py`

 * *Files identical despite different names*

## Comparing `fontmake-3.7.0b3/Lib/fontmake/ttfautohint.py` & `fontmake-3.7.1/Lib/fontmake/ttfautohint.py`

 * *Files identical despite different names*

## Comparing `fontmake-3.7.0b3/Lib/fontmake/font_project.py` & `fontmake-3.7.1/Lib/fontmake/font_project.py`

 * *Files 0% similar despite different names*

```diff
@@ -906,15 +906,15 @@
             designspace_path=designspace_path,
             master_dir=master_dir,
             instance_dir=instance_dir,
             family_name=family_name,
             mti_source=mti_source,
             write_skipexportglyphs=write_skipexportglyphs,
             generate_GDEF=generate_GDEF,
-            ufo_structure=kwargs.get("ufo_structure"),
+            ufo_structure=kwargs.get("ufo_structure", "package"),
             indent_json=kwargs.get("indent_json"),
             glyph_data=glyph_data,
             save_ufos=save_ufos,
         )
         # 'include' statements in features.fea should be resolved relative to
         # the input .glyphs path, like Glyphs.app would do, and not relative
         # to the UFOs that are generated by glyphsLib.
```

## Comparing `fontmake-3.7.0b3/Lib/fontmake/__main__.py` & `fontmake-3.7.1/Lib/fontmake/__main__.py`

 * *Files identical despite different names*

## Comparing `fontmake-3.7.0b3/Lib/fontmake.egg-info/PKG-INFO` & `fontmake-3.7.1/Lib/fontmake.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fontmake
-Version: 3.7.0b3
+Version: 3.7.1
 Summary: Compile fonts from sources (UFO, Glyphs) to binary (OpenType, TrueType).
 Home-page: https://github.com/googlei18n/fontmake
 License: Apache Software License 2.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
```

## Comparing `fontmake-3.7.0b3/Lib/fontmake.egg-info/SOURCES.txt` & `fontmake-3.7.1/Lib/fontmake.egg-info/SOURCES.txt`

 * *Files identical despite different names*

## Comparing `fontmake-3.7.0b3/Lib/fontmake.egg-info/requires.txt` & `fontmake-3.7.1/Lib/fontmake.egg-info/requires.txt`

 * *Files 18% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 attrs>=19
 fontMath>=0.9.3
 glyphsLib>=6.2.5
 ufoLib2>=0.16.0
-ufo2ft[compreffor]>=2.33.2
+ufo2ft[compreffor]>=2.33.4
 
 [:implementation_name != "cpython"]
-fonttools[ufo,unicode]>=4.41.1
+fonttools[ufo,unicode]>=4.42.0
 
 [:implementation_name == "cpython"]
-fonttools[lxml,ufo,unicode]>=4.41.1
+fonttools[lxml,ufo,unicode]>=4.42.0
 
 [all]
 skia-pathops>=0.3.0
 ttfautohint-py>=0.5.0
 ufoLib2[json]>=0.16.0
 
 [all:implementation_name != "cpython"]
-fonttools[repacker,ufo,unicode]>=4.41.1
+fonttools[repacker,ufo,unicode]>=4.42.0
 
 [all:implementation_name == "cpython"]
-fonttools[lxml,repacker,ufo,unicode]>=4.41.1
+fonttools[lxml,repacker,ufo,unicode]>=4.42.0
 
 [autohint]
 ttfautohint-py>=0.5.0
 
 [json]
 ufoLib2[json]>=0.16.0
 
@@ -33,11 +33,11 @@
 
 [pathops]
 skia-pathops>=0.3.0
 
 [repacker]
 
 [repacker:implementation_name != "cpython"]
-fonttools[repacker,ufo,unicode]>=4.41.1
+fonttools[repacker,ufo,unicode]>=4.42.0
 
 [repacker:implementation_name == "cpython"]
-fonttools[lxml,repacker,ufo,unicode]>=4.41.1
+fonttools[lxml,repacker,ufo,unicode]>=4.42.0
```

## Comparing `fontmake-3.7.0b3/.github/workflows/ci.yml` & `fontmake-3.7.1/.github/workflows/ci.yml`

 * *Files identical despite different names*

## Comparing `fontmake-3.7.0b3/tests/test_instantiator.py` & `fontmake-3.7.1/tests/test_instantiator.py`

 * *Files identical despite different names*

## Comparing `fontmake-3.7.0b3/tests/test_main.py` & `fontmake-3.7.1/tests/test_main.py`

 * *Files identical despite different names*

## Comparing `fontmake-3.7.0b3/tests/test_compatibility.py` & `fontmake-3.7.1/tests/test_compatibility.py`

 * *Files identical despite different names*

## Comparing `fontmake-3.7.0b3/tests/data/TestSubset.glyphs` & `fontmake-3.7.1/tests/data/TestSubset.glyphs`

 * *Files identical despite different names*

## Comparing `fontmake-3.7.0b3/tests/data/TestSubset2.glyphs` & `fontmake-3.7.1/tests/data/TestSubset2.glyphs`

 * *Files identical despite different names*

## Comparing `fontmake-3.7.0b3/tests/data/GlyphsUnitTestSans.glyphs` & `fontmake-3.7.1/tests/data/GlyphsUnitTestSans.glyphs`

 * *Files identical despite different names*

## Comparing `fontmake-3.7.0b3/tests/data/DesignspaceRuleOrder/MyFont.designspace` & `fontmake-3.7.1/tests/data/DesignspaceRuleOrder/MyFont.designspace`

 * *Files identical despite different names*

## Comparing `fontmake-3.7.0b3/tests/data/DesignspaceRuleOrder/MyFont_Black.ufo/fontinfo.plist` & `fontmake-3.7.1/tests/data/DesignspaceRuleOrder/MyFont_Black.ufo/fontinfo.plist`

 * *Files identical despite different names*

## Comparing `fontmake-3.7.0b3/tests/data/DesignspaceRuleOrder/MyFont_Black.ufo/glyphs/Q_.alt.glif` & `fontmake-3.7.1/tests/data/DesignspaceRuleOrder/MyFont_Black.ufo/glyphs/Q_.alt.glif`

 * *Files identical despite different names*

## Comparing `fontmake-3.7.0b3/tests/data/DesignspaceRuleOrder/MyFont_Black.ufo/glyphs/Q_.glif` & `fontmake-3.7.1/tests/data/DesignspaceRuleOrder/MyFont_Black.ufo/glyphs/Q_.glif`

 * *Files identical despite different names*

## Comparing `fontmake-3.7.0b3/tests/data/DesignspaceRuleOrder/MyFont_Black.ufo/glyphs/Q_.ss01.glif` & `fontmake-3.7.1/tests/data/DesignspaceRuleOrder/MyFont_Black.ufo/glyphs/Q_.ss01.glif`

 * *Files identical despite different names*

## Comparing `fontmake-3.7.0b3/tests/data/DesignspaceRuleOrder/MyFont_Black.ufo/glyphs/Q_.ss01.alt.glif` & `fontmake-3.7.1/tests/data/DesignspaceRuleOrder/MyFont_Black.ufo/glyphs/Q_.ss01.alt.glif`

 * *Files identical despite different names*

## Comparing `fontmake-3.7.0b3/tests/data/DesignspaceRuleOrder/MyFont_Hair.ufo/fontinfo.plist` & `fontmake-3.7.1/tests/data/DesignspaceRuleOrder/MyFont_Hair.ufo/fontinfo.plist`

 * *Files identical despite different names*

## Comparing `fontmake-3.7.0b3/tests/data/DesignspaceRuleOrder/MyFont_Hair.ufo/glyphs/Q_.alt.glif` & `fontmake-3.7.1/tests/data/DesignspaceRuleOrder/MyFont_Hair.ufo/glyphs/Q_.alt.glif`

 * *Files identical despite different names*

## Comparing `fontmake-3.7.0b3/tests/data/DesignspaceRuleOrder/MyFont_Hair.ufo/glyphs/Q_.glif` & `fontmake-3.7.1/tests/data/DesignspaceRuleOrder/MyFont_Hair.ufo/glyphs/Q_.glif`

 * *Files identical despite different names*

## Comparing `fontmake-3.7.0b3/tests/data/DesignspaceRuleOrder/MyFont_Hair.ufo/glyphs/Q_.ss01.glif` & `fontmake-3.7.1/tests/data/DesignspaceRuleOrder/MyFont_Hair.ufo/glyphs/Q_.ss01.glif`

 * *Files identical despite different names*

## Comparing `fontmake-3.7.0b3/tests/data/DesignspaceRuleOrder/MyFont_Hair.ufo/glyphs/Q_.ss01.alt.glif` & `fontmake-3.7.1/tests/data/DesignspaceRuleOrder/MyFont_Hair.ufo/glyphs/Q_.ss01.alt.glif`

 * *Files identical despite different names*

## Comparing `fontmake-3.7.0b3/tests/data/SwapGlyphNames/A.ufo/kerning.plist` & `fontmake-3.7.1/tests/data/SwapGlyphNames/A.ufo/kerning.plist`

 * *Files identical despite different names*

## Comparing `fontmake-3.7.0b3/tests/data/SwapGlyphNames/A.ufo/fontinfo.plist` & `fontmake-3.7.1/tests/data/SwapGlyphNames/B.ufo/fontinfo.plist`

 * *Files identical despite different names*

## Comparing `fontmake-3.7.0b3/tests/data/SwapGlyphNames/A.ufo/glyphs/y.glif` & `fontmake-3.7.1/tests/data/SwapGlyphNames/A.ufo/glyphs/y.glif`

 * *Files identical despite different names*

## Comparing `fontmake-3.7.0b3/tests/data/SwapGlyphNames/A.ufo/glyphs/a.swap.glif` & `fontmake-3.7.1/tests/data/SwapGlyphNames/A.ufo/glyphs/a.swap.glif`

 * *Files identical despite different names*

## Comparing `fontmake-3.7.0b3/tests/data/SwapGlyphNames/A.ufo/glyphs/contents.plist` & `fontmake-3.7.1/tests/data/SwapGlyphNames/A.ufo/glyphs/contents.plist`

 * *Files identical despite different names*

## Comparing `fontmake-3.7.0b3/tests/data/SwapGlyphNames/A.ufo/glyphs/x.glif` & `fontmake-3.7.1/tests/data/SwapGlyphNames/A.ufo/glyphs/x.glif`

 * *Files identical despite different names*

## Comparing `fontmake-3.7.0b3/tests/data/SwapGlyphNames/B.ufo/fontinfo.plist` & `fontmake-3.7.1/tests/data/SwapGlyphNames/A.ufo/fontinfo.plist`

 * *Files identical despite different names*

## Comparing `fontmake-3.7.0b3/tests/data/SwapGlyphNames/B.ufo/glyphs/a.glif` & `fontmake-3.7.1/tests/data/SwapGlyphNames/B.ufo/glyphs/a.glif`

 * *Files identical despite different names*

## Comparing `fontmake-3.7.0b3/tests/data/SwapGlyphNames/B.ufo/glyphs/dieresiscomb.glif` & `fontmake-3.7.1/tests/data/SwapGlyphNames/B.ufo/glyphs/dieresiscomb.glif`

 * *Files identical despite different names*

## Comparing `fontmake-3.7.0b3/tests/data/SwapGlyphNames/B.ufo/glyphs/a.alt.glif` & `fontmake-3.7.1/tests/data/SwapGlyphNames/B.ufo/glyphs/a.alt.glif`

 * *Files identical despite different names*

## Comparing `fontmake-3.7.0b3/tests/data/GlyphsUnitTestSans3.glyphspackage/fontinfo.plist` & `fontmake-3.7.1/tests/data/GlyphsUnitTestSans3.glyphspackage/fontinfo.plist`

 * *Files identical despite different names*

## Comparing `fontmake-3.7.0b3/tests/data/GlyphsUnitTestSans3.glyphspackage/glyphs/a.sc.glyph` & `fontmake-3.7.1/tests/data/GlyphsUnitTestSans3.glyphspackage/glyphs/a.sc.glyph`

 * *Files identical despite different names*

## Comparing `fontmake-3.7.0b3/tests/data/GlyphsUnitTestSans3.glyphspackage/glyphs/n.glyph` & `fontmake-3.7.1/tests/data/GlyphsUnitTestSans3.glyphspackage/glyphs/n.glyph`

 * *Files identical despite different names*

## Comparing `fontmake-3.7.0b3/tests/data/GlyphsUnitTestSans3.glyphspackage/glyphs/h.glyph` & `fontmake-3.7.1/tests/data/GlyphsUnitTestSans3.glyphspackage/glyphs/h.glyph`

 * *Files identical despite different names*

## Comparing `fontmake-3.7.0b3/tests/data/GlyphsUnitTestSans3.glyphspackage/glyphs/m.glyph` & `fontmake-3.7.1/tests/data/GlyphsUnitTestSans3.glyphspackage/glyphs/m.glyph`

 * *Files identical despite different names*

## Comparing `fontmake-3.7.0b3/tests/data/GlyphsUnitTestSans3.glyphspackage/glyphs/A_.glyph` & `fontmake-3.7.1/tests/data/GlyphsUnitTestSans3.glyphspackage/glyphs/A_.glyph`

 * *Files identical despite different names*

## Comparing `fontmake-3.7.0b3/tests/data/GlyphsUnitTestSans3.glyphspackage/glyphs/dieresis.glyph` & `fontmake-3.7.1/tests/data/GlyphsUnitTestSans3.glyphspackage/glyphs/dieresis.glyph`

 * *Files identical despite different names*

## Comparing `fontmake-3.7.0b3/tests/data/GlyphsUnitTestSans3.glyphspackage/glyphs/_part.shoulder.glyph` & `fontmake-3.7.1/tests/data/GlyphsUnitTestSans3.glyphspackage/glyphs/_part.shoulder.glyph`

 * *Files identical despite different names*

## Comparing `fontmake-3.7.0b3/tests/data/GlyphsUnitTestSans3.glyphspackage/glyphs/a.glyph` & `fontmake-3.7.1/tests/data/GlyphsUnitTestSans3.glyphspackage/glyphs/a.glyph`

 * *Files identical despite different names*

## Comparing `fontmake-3.7.0b3/tests/data/GlyphsUnitTestSans3.glyphspackage/glyphs/_part.stem.glyph` & `fontmake-3.7.1/tests/data/GlyphsUnitTestSans3.glyphspackage/glyphs/_part.stem.glyph`

 * *Files identical despite different names*

## Comparing `fontmake-3.7.0b3/tests/data/DesignspaceTest/DesignspaceTest.designspace` & `fontmake-3.7.1/tests/data/DesignspaceBrokenTest/DesignspaceTest.designspace`

 * *Files identical despite different names*

## Comparing `fontmake-3.7.0b3/tests/data/DesignspaceTest/MyFont-Light.ufoz` & `fontmake-3.7.1/tests/data/DesignspaceTest/MyFont-Light.ufoz`

 * *Files identical despite different names*

## Comparing `fontmake-3.7.0b3/tests/data/DesignspaceTest/DesignspaceTest-instance-attrs.designspace` & `fontmake-3.7.1/tests/data/DesignspaceTest/DesignspaceTest-instance-attrs.designspace`

 * *Files identical despite different names*

## Comparing `fontmake-3.7.0b3/tests/data/DesignspaceTest/DesignspaceTest-slnt.designspace` & `fontmake-3.7.1/tests/data/DesignspaceTest/DesignspaceTest-slnt.designspace`

 * *Files identical despite different names*

## Comparing `fontmake-3.7.0b3/tests/data/DesignspaceTest/DesignspaceTest-opsz.designspace` & `fontmake-3.7.1/tests/data/DesignspaceTest/DesignspaceTest-opsz.designspace`

 * *Files identical despite different names*

## Comparing `fontmake-3.7.0b3/tests/data/DesignspaceTest/DesignspaceTest-lib.designspace` & `fontmake-3.7.1/tests/data/DesignspaceTest/DesignspaceTest-lib.designspace`

 * *Files identical despite different names*

## Comparing `fontmake-3.7.0b3/tests/data/DesignspaceTest/DesignspaceTest-wght-wdth.designspace` & `fontmake-3.7.1/tests/data/DesignspaceTest/DesignspaceTest-wght-wdth.designspace`

 * *Files identical despite different names*

## Comparing `fontmake-3.7.0b3/tests/data/DesignspaceTest/MyFont-Bold.ufoz` & `fontmake-3.7.1/tests/data/DesignspaceTest/MyFont-Bold.ufoz`

 * *Files identical despite different names*

## Comparing `fontmake-3.7.0b3/tests/data/DesignspaceTest/DesignspaceTest-bare.designspace` & `fontmake-3.7.1/tests/data/DesignspaceTest/DesignspaceTest-bare.designspace`

 * *Files identical despite different names*

## Comparing `fontmake-3.7.0b3/tests/data/DesignspaceTest/MyFont-Light.ufo/fontinfo.plist` & `fontmake-3.7.1/tests/data/DesignspaceTest/MyFont-Light.ufo/fontinfo.plist`

 * *Files identical despite different names*

## Comparing `fontmake-3.7.0b3/tests/data/DesignspaceTest/MyFont-Bold.ufo/fontinfo.plist` & `fontmake-3.7.1/tests/data/DesignspaceTest/MyFont-Bold.ufo/fontinfo.plist`

 * *Files identical despite different names*

## Comparing `fontmake-3.7.0b3/tests/data/InstantiatorStrictMathGlyph/StrictMathGlyph.designspace` & `fontmake-3.7.1/tests/data/InstantiatorStrictMathGlyph/StrictMathGlyph.designspace`

 * *Files identical despite different names*

## Comparing `fontmake-3.7.0b3/tests/data/InstantiatorStrictMathGlyph/SquareOne.ufo/fontinfo.plist` & `fontmake-3.7.1/tests/data/InstantiatorStrictMathGlyph/SquareOne.ufo/fontinfo.plist`

 * *Files identical despite different names*

## Comparing `fontmake-3.7.0b3/tests/data/InstantiatorStrictMathGlyph/SquareOne.ufo/lib.plist` & `fontmake-3.7.1/tests/data/InstantiatorStrictMathGlyph/SquareTwo.ufo/lib.plist`

 * *Files identical despite different names*

## Comparing `fontmake-3.7.0b3/tests/data/InstantiatorStrictMathGlyph/SquareOne.ufo/glyphs/test.glif` & `fontmake-3.7.1/tests/data/InstantiatorStrictMathGlyph/SquareOne.ufo/glyphs/test.glif`

 * *Files identical despite different names*

## Comparing `fontmake-3.7.0b3/tests/data/InstantiatorStrictMathGlyph/SquareTwo.ufo/fontinfo.plist` & `fontmake-3.7.1/tests/data/InstantiatorStrictMathGlyph/SquareTwo.ufo/fontinfo.plist`

 * *Files identical despite different names*

## Comparing `fontmake-3.7.0b3/tests/data/InstantiatorStrictMathGlyph/SquareTwo.ufo/lib.plist` & `fontmake-3.7.1/tests/data/InstantiatorStrictMathGlyph/SquareOne.ufo/lib.plist`

 * *Files identical despite different names*

## Comparing `fontmake-3.7.0b3/tests/data/InstantiatorStrictMathGlyph/SquareTwo.ufo/glyphs/test.glif` & `fontmake-3.7.1/tests/data/InstantiatorStrictMathGlyph/SquareTwo.ufo/glyphs/test.glif`

 * *Files identical despite different names*

## Comparing `fontmake-3.7.0b3/tests/data/DesignspaceBrokenTest/DesignspaceTest.designspace` & `fontmake-3.7.1/tests/data/DesignspaceTest/DesignspaceTest.designspace`

 * *Files identical despite different names*

## Comparing `fontmake-3.7.0b3/tests/data/DesignspaceBrokenTest/Designspace-MastersAsInstances.designspace` & `fontmake-3.7.1/tests/data/DesignspaceBrokenTest/Designspace-MastersAsInstances.designspace`

 * *Files identical despite different names*

## Comparing `fontmake-3.7.0b3/tests/data/DesignspaceBrokenTest/MyFont-Light.ufo/fontinfo.plist` & `fontmake-3.7.1/tests/data/DesignspaceBrokenTest/MyFont-Light.ufo/fontinfo.plist`

 * *Files identical despite different names*

## Comparing `fontmake-3.7.0b3/tests/data/DesignspaceBrokenTest/MyFont-Bold.ufo/fontinfo.plist` & `fontmake-3.7.1/tests/data/DesignspaceBrokenTest/MyFont-Bold.ufo/fontinfo.plist`

 * *Files identical despite different names*

## Comparing `fontmake-3.7.0b3/tests/data/InterpolateLayoutTest/InterpolateLayoutTest.plist` & `fontmake-3.7.1/tests/data/InterpolateLayoutTest/InterpolateLayoutTest.plist`

 * *Files identical despite different names*

## Comparing `fontmake-3.7.0b3/tests/data/InterpolateLayoutTest/InterpolateLayoutTest.glyphs` & `fontmake-3.7.1/tests/data/InterpolateLayoutTest/InterpolateLayoutTest.glyphs`

 * *Files identical despite different names*

## Comparing `fontmake-3.7.0b3/tests/data/AutohintingTest/Padyakke.glyphs` & `fontmake-3.7.1/tests/data/AutohintingTest/Padyakke.glyphs`

 * *Files identical despite different names*

## Comparing `fontmake-3.7.0b3/tests/data/IncompatibleSans/IncompatibleSans.designspace` & `fontmake-3.7.1/tests/data/IncompatibleSans/IncompatibleSans.designspace`

 * *Files identical despite different names*

## Comparing `fontmake-3.7.0b3/tests/data/IncompatibleSans/IncompatibleSans-Bold.ufo/fontinfo.plist` & `fontmake-3.7.1/tests/data/IncompatibleSans/IncompatibleSans-Bold.ufo/fontinfo.plist`

 * *Files identical despite different names*

## Comparing `fontmake-3.7.0b3/tests/data/IncompatibleSans/IncompatibleSans-Bold.ufo/lib.plist` & `fontmake-3.7.1/tests/data/IncompatibleSans/IncompatibleSans-Bold.ufo/lib.plist`

 * *Files identical despite different names*

## Comparing `fontmake-3.7.0b3/tests/data/IncompatibleSans/IncompatibleSans-Bold.ufo/glyphs/D_.glif` & `fontmake-3.7.1/tests/data/IncompatibleSans/IncompatibleSans-Bold.ufo/glyphs/D_.glif`

 * *Files identical despite different names*

## Comparing `fontmake-3.7.0b3/tests/data/IncompatibleSans/IncompatibleSans-Bold.ufo/glyphs/B_.glif` & `fontmake-3.7.1/tests/data/IncompatibleSans/IncompatibleSans-Bold.ufo/glyphs/B_.glif`

 * *Files identical despite different names*

## Comparing `fontmake-3.7.0b3/tests/data/IncompatibleSans/IncompatibleSans-Bold.ufo/glyphs/A_.glif` & `fontmake-3.7.1/tests/data/IncompatibleSans/IncompatibleSans-Bold.ufo/glyphs/A_.glif`

 * *Files identical despite different names*

## Comparing `fontmake-3.7.0b3/tests/data/IncompatibleSans/IncompatibleSans-Regular.ufo/fontinfo.plist` & `fontmake-3.7.1/tests/data/IncompatibleSans/IncompatibleSans-Regular.ufo/fontinfo.plist`

 * *Files identical despite different names*

## Comparing `fontmake-3.7.0b3/tests/data/IncompatibleSans/IncompatibleSans-Regular.ufo/lib.plist` & `fontmake-3.7.1/tests/data/IncompatibleSans/IncompatibleSans-Regular.ufo/lib.plist`

 * *Files identical despite different names*

## Comparing `fontmake-3.7.0b3/tests/data/IncompatibleSans/IncompatibleSans-Regular.ufo/glyphs/D_.glif` & `fontmake-3.7.1/tests/data/IncompatibleSans/IncompatibleSans-Regular.ufo/glyphs/D_.glif`

 * *Files identical despite different names*

## Comparing `fontmake-3.7.0b3/tests/data/IncompatibleSans/IncompatibleSans-Regular.ufo/glyphs/B_.glif` & `fontmake-3.7.1/tests/data/IncompatibleSans/IncompatibleSans-Regular.ufo/glyphs/B_.glif`

 * *Files identical despite different names*

## Comparing `fontmake-3.7.0b3/tests/data/IncompatibleSans/IncompatibleSans-Regular.ufo/glyphs/A_.glif` & `fontmake-3.7.1/tests/data/IncompatibleSans/IncompatibleSans-Regular.ufo/glyphs/A_.glif`

 * *Files identical despite different names*

## Comparing `fontmake-3.7.0b3/tests/data/DesignspaceTestSharedFeatures/DesignspaceTestSharedFeatures.designspace` & `fontmake-3.7.1/tests/data/DesignspaceTestSharedFeatures/DesignspaceTestSharedFeatures.designspace`

 * *Files identical despite different names*

## Comparing `fontmake-3.7.0b3/tests/data/DesignspaceTestSharedFeatures/DesignspaceTest-Regular.ufo/fontinfo.plist` & `fontmake-3.7.1/tests/data/DesignspaceTestSharedFeatures/DesignspaceTest-Regular.ufo/fontinfo.plist`

 * *Files identical despite different names*

## Comparing `fontmake-3.7.0b3/tests/data/DesignspaceTestSharedFeatures/DesignspaceTest-Light.ufo/fontinfo.plist` & `fontmake-3.7.1/tests/data/DesignspaceTestSharedFeatures/DesignspaceTest-Light.ufo/fontinfo.plist`

 * *Files identical despite different names*

## Comparing `fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSans_missing.designspace` & `fontmake-3.7.1/tests/data/MutatorSans/MutatorSans_missing.designspace`

 * *Files identical despite different names*

## Comparing `fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSans.designspace` & `fontmake-3.7.1/tests/data/MutatorSans/MutatorSans.designspace`

 * *Files identical despite different names*

## Comparing `fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSans-width-only.designspace` & `fontmake-3.7.1/tests/data/MutatorSans/MutatorSans-width-only.designspace`

 * *Files identical despite different names*

## Comparing `fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSans-with-openNodes.designspace` & `fontmake-3.7.1/tests/data/MutatorSans/MutatorSans-with-openNodes.designspace`

 * *Files identical despite different names*

## Comparing `fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSans-weight-only.designspace` & `fontmake-3.7.1/tests/data/MutatorSans/MutatorSans-weight-only.designspace`

 * *Files identical despite different names*

## Comparing `fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSans-non-default-layer.designspace` & `fontmake-3.7.1/tests/data/MutatorSans/MutatorSans-non-default-layer.designspace`

 * *Files identical despite different names*

## Comparing `fontmake-3.7.0b3/tests/data/MutatorSans/LICENSE` & `fontmake-3.7.1/tests/data/MutatorSansLite/LICENSE`

 * *Files identical despite different names*

## Comparing `fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSans_no_default.designspace` & `fontmake-3.7.1/tests/data/MutatorSans/MutatorSans_no_default.designspace`

 * *Files identical despite different names*

## Comparing `fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansLightWide.ufo/kerning.plist` & `fontmake-3.7.1/tests/data/MutatorSans/MutatorSansLightWide.ufo/kerning.plist`

 * *Files identical despite different names*

## Comparing `fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansLightWide.ufo/fontinfo.plist` & `fontmake-3.7.1/tests/data/MutatorSans/MutatorSansLightWide.ufo/fontinfo.plist`

 * *Files identical despite different names*

## Comparing `fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansLightWide.ufo/lib.plist` & `fontmake-3.7.1/tests/data/MutatorSans/MutatorSansLightWide.ufo/lib.plist`

 * *Files identical despite different names*

## Comparing `fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs.background/S_.closed.glif` & `fontmake-3.7.1/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs.background/S_.closed.glif`

 * *Files identical despite different names*

## Comparing `fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs.master_width_720.00_weight_645.00/S_.glif` & `fontmake-3.7.1/tests/data/MutatorSansLite/MutatorSansLightWide.ufo/glyphs.master_width_720.00_weight_645.00/S_.glif`

 * *Files identical despite different names*

## Comparing `fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs.master_width_500.00_weight_500.00/S_.glif` & `fontmake-3.7.1/tests/data/MutatorSansLite/MutatorSansLightWide.ufo/glyphs.master_width_500.00_weight_500.00/S_.glif`

 * *Files identical despite different names*

## Comparing `fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/W_.glif` & `fontmake-3.7.1/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/W_.glif`

 * *Files identical despite different names*

## Comparing `fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/T_.glif` & `fontmake-3.7.1/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/T_.glif`

 * *Files identical despite different names*

## Comparing `fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/R_.glif` & `fontmake-3.7.1/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/R_.glif`

 * *Files identical despite different names*

## Comparing `fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/O_.glif` & `fontmake-3.7.1/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/O_.glif`

 * *Files identical despite different names*

## Comparing `fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/G_.glif` & `fontmake-3.7.1/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/G_.glif`

 * *Files identical despite different names*

## Comparing `fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/D_.glif` & `fontmake-3.7.1/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/D_.glif`

 * *Files identical despite different names*

## Comparing `fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/S_.closed.glif` & `fontmake-3.7.1/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/S_.closed.glif`

 * *Files identical despite different names*

## Comparing `fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/X_.glif` & `fontmake-3.7.1/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/X_.glif`

 * *Files identical despite different names*

## Comparing `fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/M_.glif` & `fontmake-3.7.1/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/M_.glif`

 * *Files identical despite different names*

## Comparing `fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/Z_.glif` & `fontmake-3.7.1/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/Z_.glif`

 * *Files identical despite different names*

## Comparing `fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/I_.narrow.glif` & `fontmake-3.7.1/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/I_.narrow.glif`

 * *Files identical despite different names*

## Comparing `fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/F_.glif` & `fontmake-3.7.1/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/F_.glif`

 * *Files identical despite different names*

## Comparing `fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/C_.glif` & `fontmake-3.7.1/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/C_.glif`

 * *Files identical despite different names*

## Comparing `fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/arrowright.glif` & `fontmake-3.7.1/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/arrowright.glif`

 * *Files identical despite different names*

## Comparing `fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/B_.glif` & `fontmake-3.7.1/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/B_.glif`

 * *Files identical despite different names*

## Comparing `fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/U_.glif` & `fontmake-3.7.1/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/U_.glif`

 * *Files identical despite different names*

## Comparing `fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/I_.glif` & `fontmake-3.7.1/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/I_.glif`

 * *Files identical despite different names*

## Comparing `fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/N_.glif` & `fontmake-3.7.1/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/N_.glif`

 * *Files identical despite different names*

## Comparing `fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/V_.glif` & `fontmake-3.7.1/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/V_.glif`

 * *Files identical despite different names*

## Comparing `fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/I_J_.glif` & `fontmake-3.7.1/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/I_J_.glif`

 * *Files identical despite different names*

## Comparing `fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/comma.glif` & `fontmake-3.7.1/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/comma.glif`

 * *Files identical despite different names*

## Comparing `fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/contents.plist` & `fontmake-3.7.1/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/contents.plist`

 * *Files identical despite different names*

## Comparing `fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/Y_.glif` & `fontmake-3.7.1/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/Y_.glif`

 * *Files identical despite different names*

## Comparing `fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/L_.glif` & `fontmake-3.7.1/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/L_.glif`

 * *Files identical despite different names*

## Comparing `fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/arrowdown.glif` & `fontmake-3.7.1/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/arrowdown.glif`

 * *Files identical despite different names*

## Comparing `fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/P_.glif` & `fontmake-3.7.1/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/P_.glif`

 * *Files identical despite different names*

## Comparing `fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/J_.narrow.glif` & `fontmake-3.7.1/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/J_.narrow.glif`

 * *Files identical despite different names*

## Comparing `fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/arrowleft.glif` & `fontmake-3.7.1/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/arrowleft.glif`

 * *Files identical despite different names*

## Comparing `fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/K_.glif` & `fontmake-3.7.1/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/K_.glif`

 * *Files identical despite different names*

## Comparing `fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/A_.glif` & `fontmake-3.7.1/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/A_.glif`

 * *Files identical despite different names*

## Comparing `fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/J_.glif` & `fontmake-3.7.1/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/J_.glif`

 * *Files identical despite different names*

## Comparing `fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/H_.glif` & `fontmake-3.7.1/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/H_.glif`

 * *Files identical despite different names*

## Comparing `fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/S_.glif` & `fontmake-3.7.1/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/S_.glif`

 * *Files identical despite different names*

## Comparing `fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/E_.glif` & `fontmake-3.7.1/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/E_.glif`

 * *Files identical despite different names*

## Comparing `fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/arrowup.glif` & `fontmake-3.7.1/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/arrowup.glif`

 * *Files identical despite different names*

## Comparing `fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansIntermediateCondensed.ufo/layercontents.plist` & `fontmake-3.7.1/tests/data/MutatorSans/MutatorSansIntermediateCondensed.ufo/layercontents.plist`

 * *Files identical despite different names*

## Comparing `fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansIntermediateCondensed.ufo/fontinfo.plist` & `fontmake-3.7.1/tests/data/MutatorSans/MutatorSansIntermediateCondensed.ufo/fontinfo.plist`

 * *Files identical despite different names*

## Comparing `fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansIntermediateCondensed.ufo/lib.plist` & `fontmake-3.7.1/tests/data/MutatorSans/MutatorSansIntermediateCondensed.ufo/lib.plist`

 * *Files identical despite different names*

## Comparing `fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansIntermediateCondensed.ufo/glyphs.background/S_.glif` & `fontmake-3.7.1/tests/data/MutatorSans/MutatorSansIntermediateCondensed.ufo/glyphs.background/S_.glif`

 * *Files identical despite different names*

## Comparing `fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansIntermediateCondensed.ufo/glyphs.reference.interpolation/S_.glif` & `fontmake-3.7.1/tests/data/MutatorSans/MutatorSansIntermediateCondensed.ufo/glyphs.reference.interpolation/S_.glif`

 * *Files identical despite different names*

## Comparing `fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansIntermediateCondensed.ufo/glyphs.reference.interpolation/E_.glif` & `fontmake-3.7.1/tests/data/MutatorSans/MutatorSansIntermediateCondensed.ufo/glyphs.reference.interpolation/E_.glif`

 * *Files identical despite different names*

## Comparing `fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansIntermediateCondensed.ufo/glyphs/G_.glif` & `fontmake-3.7.1/tests/data/MutatorSans/MutatorSansIntermediateCondensed.ufo/glyphs/G_.glif`

 * *Files identical despite different names*

## Comparing `fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansIntermediateCondensed.ufo/glyphs/F_.glif` & `fontmake-3.7.1/tests/data/MutatorSans/MutatorSansIntermediateCondensed.ufo/glyphs/F_.glif`

 * *Files identical despite different names*

## Comparing `fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansIntermediateCondensed.ufo/glyphs/B_.glif` & `fontmake-3.7.1/tests/data/MutatorSans/MutatorSansIntermediateCondensed.ufo/glyphs/B_.glif`

 * *Files identical despite different names*

## Comparing `fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansIntermediateCondensed.ufo/glyphs/S_.glif` & `fontmake-3.7.1/tests/data/MutatorSans/MutatorSansIntermediateCondensed.ufo/glyphs/S_.glif`

 * *Files identical despite different names*

## Comparing `fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansIntermediateCondensed.ufo/glyphs/E_.glif` & `fontmake-3.7.1/tests/data/MutatorSans/MutatorSansIntermediateCondensed.ufo/glyphs/E_.glif`

 * *Files identical despite different names*

## Comparing `fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansIntermediateCondensed.ufo/glyphs.interpolation/E_.glif` & `fontmake-3.7.1/tests/data/MutatorSans/MutatorSansIntermediateCondensed.ufo/glyphs.interpolation/E_.glif`

 * *Files identical despite different names*

## Comparing `fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/kerning.plist` & `fontmake-3.7.1/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/kerning.plist`

 * *Files identical despite different names*

## Comparing `fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/fontinfo.plist` & `fontmake-3.7.1/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/fontinfo.plist`

 * *Files identical despite different names*

## Comparing `fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/lib.plist` & `fontmake-3.7.1/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/lib.plist`

 * *Files identical despite different names*

## Comparing `fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs.background/S_.closed.glif` & `fontmake-3.7.1/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs.background/S_.closed.glif`

 * *Files identical despite different names*

## Comparing `fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/W_.glif` & `fontmake-3.7.1/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/W_.glif`

 * *Files identical despite different names*

## Comparing `fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/T_.glif` & `fontmake-3.7.1/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/T_.glif`

 * *Files identical despite different names*

## Comparing `fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/R_.glif` & `fontmake-3.7.1/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/R_.glif`

 * *Files identical despite different names*

## Comparing `fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/O_.glif` & `fontmake-3.7.1/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/O_.glif`

 * *Files identical despite different names*

## Comparing `fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/G_.glif` & `fontmake-3.7.1/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/G_.glif`

 * *Files identical despite different names*

## Comparing `fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/D_.glif` & `fontmake-3.7.1/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/D_.glif`

 * *Files identical despite different names*

## Comparing `fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/S_.closed.glif` & `fontmake-3.7.1/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/S_.closed.glif`

 * *Files identical despite different names*

## Comparing `fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/X_.glif` & `fontmake-3.7.1/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/X_.glif`

 * *Files identical despite different names*

## Comparing `fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/M_.glif` & `fontmake-3.7.1/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/M_.glif`

 * *Files identical despite different names*

## Comparing `fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/Z_.glif` & `fontmake-3.7.1/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/Z_.glif`

 * *Files identical despite different names*

## Comparing `fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/I_.narrow.glif` & `fontmake-3.7.1/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/I_.narrow.glif`

 * *Files identical despite different names*

## Comparing `fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/F_.glif` & `fontmake-3.7.1/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/F_.glif`

 * *Files identical despite different names*

## Comparing `fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/C_.glif` & `fontmake-3.7.1/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/C_.glif`

 * *Files identical despite different names*

## Comparing `fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/B_.glif` & `fontmake-3.7.1/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/B_.glif`

 * *Files identical despite different names*

## Comparing `fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/U_.glif` & `fontmake-3.7.1/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/U_.glif`

 * *Files identical despite different names*

## Comparing `fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/I_.glif` & `fontmake-3.7.1/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/I_.glif`

 * *Files identical despite different names*

## Comparing `fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/N_.glif` & `fontmake-3.7.1/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/N_.glif`

 * *Files identical despite different names*

## Comparing `fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/V_.glif` & `fontmake-3.7.1/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/V_.glif`

 * *Files identical despite different names*

## Comparing `fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/I_J_.glif` & `fontmake-3.7.1/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/I_J_.glif`

 * *Files identical despite different names*

## Comparing `fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/comma.glif` & `fontmake-3.7.1/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/comma.glif`

 * *Files identical despite different names*

## Comparing `fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/contents.plist` & `fontmake-3.7.1/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/contents.plist`

 * *Files identical despite different names*

## Comparing `fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/Y_.glif` & `fontmake-3.7.1/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/Y_.glif`

 * *Files identical despite different names*

## Comparing `fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/quotedblbase.glif` & `fontmake-3.7.1/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/quotedblbase.glif`

 * *Files identical despite different names*

## Comparing `fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/L_.glif` & `fontmake-3.7.1/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/L_.glif`

 * *Files identical despite different names*

## Comparing `fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/P_.glif` & `fontmake-3.7.1/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/P_.glif`

 * *Files identical despite different names*

## Comparing `fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/J_.narrow.glif` & `fontmake-3.7.1/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/J_.narrow.glif`

 * *Files identical despite different names*

## Comparing `fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/K_.glif` & `fontmake-3.7.1/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/K_.glif`

 * *Files identical despite different names*

## Comparing `fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/A_.glif` & `fontmake-3.7.1/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/A_.glif`

 * *Files identical despite different names*

## Comparing `fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/J_.glif` & `fontmake-3.7.1/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/J_.glif`

 * *Files identical despite different names*

## Comparing `fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/H_.glif` & `fontmake-3.7.1/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/H_.glif`

 * *Files identical despite different names*

## Comparing `fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/S_.glif` & `fontmake-3.7.1/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/S_.glif`

 * *Files identical despite different names*

## Comparing `fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/E_.glif` & `fontmake-3.7.1/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/E_.glif`

 * *Files identical despite different names*

## Comparing `fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/quotesinglbase.glif` & `fontmake-3.7.1/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/quotesinglbase.glif`

 * *Files identical despite different names*

## Comparing `fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansIntermediateWide.ufo/kerning.plist` & `fontmake-3.7.1/tests/data/MutatorSans/MutatorSansIntermediateWide.ufo/kerning.plist`

 * *Files identical despite different names*

## Comparing `fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansIntermediateWide.ufo/fontinfo.plist` & `fontmake-3.7.1/tests/data/MutatorSans/MutatorSansIntermediateWide.ufo/fontinfo.plist`

 * *Files identical despite different names*

## Comparing `fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansIntermediateWide.ufo/lib.plist` & `fontmake-3.7.1/tests/data/MutatorSans/MutatorSansIntermediateWide.ufo/lib.plist`

 * *Files identical despite different names*

## Comparing `fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansIntermediateWide.ufo/glyphs.background/S_.glif` & `fontmake-3.7.1/tests/data/MutatorSans/MutatorSansIntermediateWide.ufo/glyphs.background/S_.glif`

 * *Files identical despite different names*

## Comparing `fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansIntermediateWide.ufo/glyphs/G_.glif` & `fontmake-3.7.1/tests/data/MutatorSans/MutatorSansIntermediateWide.ufo/glyphs/G_.glif`

 * *Files identical despite different names*

## Comparing `fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansIntermediateWide.ufo/glyphs/F_.glif` & `fontmake-3.7.1/tests/data/MutatorSans/MutatorSansIntermediateWide.ufo/glyphs/F_.glif`

 * *Files identical despite different names*

## Comparing `fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansIntermediateWide.ufo/glyphs/B_.glif` & `fontmake-3.7.1/tests/data/MutatorSans/MutatorSansIntermediateWide.ufo/glyphs/B_.glif`

 * *Files identical despite different names*

## Comparing `fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansIntermediateWide.ufo/glyphs/E_.glif` & `fontmake-3.7.1/tests/data/MutatorSans/MutatorSansIntermediateWide.ufo/glyphs/E_.glif`

 * *Files identical despite different names*

## Comparing `fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansBoldWide.ufo/fontinfo.plist` & `fontmake-3.7.1/tests/data/MutatorSans/MutatorSansBoldWide.ufo/fontinfo.plist`

 * *Files identical despite different names*

## Comparing `fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansBoldWide.ufo/lib.plist` & `fontmake-3.7.1/tests/data/MutatorSans/MutatorSansBoldWide.ufo/lib.plist`

 * *Files identical despite different names*

## Comparing `fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs.background/S_.closed.glif` & `fontmake-3.7.1/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs.background/S_.closed.glif`

 * *Files identical despite different names*

## Comparing `fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs.background/S_.glif` & `fontmake-3.7.1/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs.background/S_.glif`

 * *Files identical despite different names*

## Comparing `fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/W_.glif` & `fontmake-3.7.1/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/W_.glif`

 * *Files identical despite different names*

## Comparing `fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/T_.glif` & `fontmake-3.7.1/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/T_.glif`

 * *Files identical despite different names*

## Comparing `fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/R_.glif` & `fontmake-3.7.1/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/R_.glif`

 * *Files identical despite different names*

## Comparing `fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/O_.glif` & `fontmake-3.7.1/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/O_.glif`

 * *Files identical despite different names*

## Comparing `fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/G_.glif` & `fontmake-3.7.1/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/G_.glif`

 * *Files identical despite different names*

## Comparing `fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/D_.glif` & `fontmake-3.7.1/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/D_.glif`

 * *Files identical despite different names*

## Comparing `fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/S_.closed.glif` & `fontmake-3.7.1/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/S_.closed.glif`

 * *Files identical despite different names*

## Comparing `fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/X_.glif` & `fontmake-3.7.1/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/X_.glif`

 * *Files identical despite different names*

## Comparing `fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/M_.glif` & `fontmake-3.7.1/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/M_.glif`

 * *Files identical despite different names*

## Comparing `fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/Z_.glif` & `fontmake-3.7.1/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/Z_.glif`

 * *Files identical despite different names*

## Comparing `fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/I_.narrow.glif` & `fontmake-3.7.1/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/I_.narrow.glif`

 * *Files identical despite different names*

## Comparing `fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/F_.glif` & `fontmake-3.7.1/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/F_.glif`

 * *Files identical despite different names*

## Comparing `fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/C_.glif` & `fontmake-3.7.1/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/C_.glif`

 * *Files identical despite different names*

## Comparing `fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/B_.glif` & `fontmake-3.7.1/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/B_.glif`

 * *Files identical despite different names*

## Comparing `fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/U_.glif` & `fontmake-3.7.1/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/U_.glif`

 * *Files identical despite different names*

## Comparing `fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/I_.glif` & `fontmake-3.7.1/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/I_.glif`

 * *Files identical despite different names*

## Comparing `fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/N_.glif` & `fontmake-3.7.1/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/N_.glif`

 * *Files identical despite different names*

## Comparing `fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/V_.glif` & `fontmake-3.7.1/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/V_.glif`

 * *Files identical despite different names*

## Comparing `fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/I_J_.glif` & `fontmake-3.7.1/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/I_J_.glif`

 * *Files identical despite different names*

## Comparing `fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/comma.glif` & `fontmake-3.7.1/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/comma.glif`

 * *Files identical despite different names*

## Comparing `fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/contents.plist` & `fontmake-3.7.1/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/contents.plist`

 * *Files identical despite different names*

## Comparing `fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/Y_.glif` & `fontmake-3.7.1/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/Y_.glif`

 * *Files identical despite different names*

## Comparing `fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/L_.glif` & `fontmake-3.7.1/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/L_.glif`

 * *Files identical despite different names*

## Comparing `fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/P_.glif` & `fontmake-3.7.1/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/P_.glif`

 * *Files identical despite different names*

## Comparing `fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/J_.narrow.glif` & `fontmake-3.7.1/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/J_.narrow.glif`

 * *Files identical despite different names*

## Comparing `fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/K_.glif` & `fontmake-3.7.1/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/K_.glif`

 * *Files identical despite different names*

## Comparing `fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/A_.glif` & `fontmake-3.7.1/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/A_.glif`

 * *Files identical despite different names*

## Comparing `fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/J_.glif` & `fontmake-3.7.1/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/J_.glif`

 * *Files identical despite different names*

## Comparing `fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/H_.glif` & `fontmake-3.7.1/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/H_.glif`

 * *Files identical despite different names*

## Comparing `fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/S_.glif` & `fontmake-3.7.1/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/S_.glif`

 * *Files identical despite different names*

## Comparing `fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/E_.glif` & `fontmake-3.7.1/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/E_.glif`

 * *Files identical despite different names*

## Comparing `fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/layercontents.plist` & `fontmake-3.7.1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/layercontents.plist`

 * *Files identical despite different names*

## Comparing `fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/kerning.plist` & `fontmake-3.7.1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/kerning.plist`

 * *Files identical despite different names*

## Comparing `fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/fontinfo.plist` & `fontmake-3.7.1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/fontinfo.plist`

 * *Files identical despite different names*

## Comparing `fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/lib.plist` & `fontmake-3.7.1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/lib.plist`

 * *Files identical despite different names*

## Comparing `fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs.background/S_.closed.glif` & `fontmake-3.7.1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs.background/S_.closed.glif`

 * *Files identical despite different names*

## Comparing `fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs.background/S_.glif` & `fontmake-3.7.1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs.background/S_.glif`

 * *Files identical despite different names*

## Comparing `fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs.support.crossbar/G_.glif` & `fontmake-3.7.1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs.support.crossbar/G_.glif`

 * *Files identical despite different names*

## Comparing `fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs.support.crossbar/F_.glif` & `fontmake-3.7.1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs.support.crossbar/F_.glif`

 * *Files identical despite different names*

## Comparing `fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs.support.crossbar/B_.glif` & `fontmake-3.7.1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs.support.crossbar/B_.glif`

 * *Files identical despite different names*

## Comparing `fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs.support.crossbar/S_.glif` & `fontmake-3.7.1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs.support.crossbar/S_.glif`

 * *Files identical despite different names*

## Comparing `fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs.support.crossbar/E_.glif` & `fontmake-3.7.1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs.support.crossbar/E_.glif`

 * *Files identical despite different names*

## Comparing `fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs.support/W_.glif` & `fontmake-3.7.1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs.support/W_.glif`

 * *Files identical despite different names*

## Comparing `fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs.support/A_.glif` & `fontmake-3.7.1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs.support/A_.glif`

 * *Files identical despite different names*

## Comparing `fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs.support/S_.glif` & `fontmake-3.7.1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs.support/S_.glif`

 * *Files identical despite different names*

## Comparing `fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs.support.S_.middle/S_.closed.glif` & `fontmake-3.7.1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs.support.S_.middle/S_.closed.glif`

 * *Files identical despite different names*

## Comparing `fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/W_.glif` & `fontmake-3.7.1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/W_.glif`

 * *Files identical despite different names*

## Comparing `fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/T_.glif` & `fontmake-3.7.1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/T_.glif`

 * *Files identical despite different names*

## Comparing `fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/R_.glif` & `fontmake-3.7.1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/R_.glif`

 * *Files identical despite different names*

## Comparing `fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/O_.glif` & `fontmake-3.7.1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/O_.glif`

 * *Files identical despite different names*

## Comparing `fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/G_.glif` & `fontmake-3.7.1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/G_.glif`

 * *Files identical despite different names*

## Comparing `fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/D_.glif` & `fontmake-3.7.1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/D_.glif`

 * *Files identical despite different names*

## Comparing `fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/S_.closed.glif` & `fontmake-3.7.1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/S_.closed.glif`

 * *Files identical despite different names*

## Comparing `fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/X_.glif` & `fontmake-3.7.1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/X_.glif`

 * *Files identical despite different names*

## Comparing `fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/M_.glif` & `fontmake-3.7.1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/M_.glif`

 * *Files identical despite different names*

## Comparing `fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/Z_.glif` & `fontmake-3.7.1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/Z_.glif`

 * *Files identical despite different names*

## Comparing `fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/I_.narrow.glif` & `fontmake-3.7.1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/I_.narrow.glif`

 * *Files identical despite different names*

## Comparing `fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/F_.glif` & `fontmake-3.7.1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/F_.glif`

 * *Files identical despite different names*

## Comparing `fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/C_.glif` & `fontmake-3.7.1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/C_.glif`

 * *Files identical despite different names*

## Comparing `fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/arrowright.glif` & `fontmake-3.7.1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/arrowright.glif`

 * *Files identical despite different names*

## Comparing `fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/B_.glif` & `fontmake-3.7.1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/B_.glif`

 * *Files identical despite different names*

## Comparing `fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/U_.glif` & `fontmake-3.7.1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/U_.glif`

 * *Files identical despite different names*

## Comparing `fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/I_.glif` & `fontmake-3.7.1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/I_.glif`

 * *Files identical despite different names*

## Comparing `fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/N_.glif` & `fontmake-3.7.1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/N_.glif`

 * *Files identical despite different names*

## Comparing `fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/V_.glif` & `fontmake-3.7.1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/V_.glif`

 * *Files identical despite different names*

## Comparing `fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/I_J_.glif` & `fontmake-3.7.1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/I_J_.glif`

 * *Files identical despite different names*

## Comparing `fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/comma.glif` & `fontmake-3.7.1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/comma.glif`

 * *Files identical despite different names*

## Comparing `fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/contents.plist` & `fontmake-3.7.1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/contents.plist`

 * *Files identical despite different names*

## Comparing `fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/Y_.glif` & `fontmake-3.7.1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/Y_.glif`

 * *Files identical despite different names*

## Comparing `fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/L_.glif` & `fontmake-3.7.1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/L_.glif`

 * *Files identical despite different names*

## Comparing `fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/arrowdown.glif` & `fontmake-3.7.1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/arrowdown.glif`

 * *Files identical despite different names*

## Comparing `fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/P_.glif` & `fontmake-3.7.1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/P_.glif`

 * *Files identical despite different names*

## Comparing `fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/J_.narrow.glif` & `fontmake-3.7.1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/J_.narrow.glif`

 * *Files identical despite different names*

## Comparing `fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/arrowleft.glif` & `fontmake-3.7.1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/arrowleft.glif`

 * *Files identical despite different names*

## Comparing `fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/K_.glif` & `fontmake-3.7.1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/K_.glif`

 * *Files identical despite different names*

## Comparing `fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/A_.glif` & `fontmake-3.7.1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/A_.glif`

 * *Files identical despite different names*

## Comparing `fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/J_.glif` & `fontmake-3.7.1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/J_.glif`

 * *Files identical despite different names*

## Comparing `fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/H_.glif` & `fontmake-3.7.1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/H_.glif`

 * *Files identical despite different names*

## Comparing `fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/S_.glif` & `fontmake-3.7.1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/S_.glif`

 * *Files identical despite different names*

## Comparing `fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/E_.glif` & `fontmake-3.7.1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/E_.glif`

 * *Files identical despite different names*

## Comparing `fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/arrowup.glif` & `fontmake-3.7.1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/arrowup.glif`

 * *Files identical despite different names*

## Comparing `fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs.support.crossbars/E_.glif` & `fontmake-3.7.1/tests/data/MutatorSansLite/MutatorSansLightCondensed.ufo/glyphs.support.crossbars/E_.glif`

 * *Files identical despite different names*

## Comparing `fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs.support.S_.wide/S_.closed.glif` & `fontmake-3.7.1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs.support.S_.wide/S_.closed.glif`

 * *Files identical despite different names*

## Comparing `fontmake-3.7.0b3/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs.support.S_.wide/S_.glif` & `fontmake-3.7.1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs.support.S_.wide/S_.glif`

 * *Files identical despite different names*

## Comparing `fontmake-3.7.0b3/tests/data/MutatorSansLite/MutatorSans_v5_several_vfs.designspace` & `fontmake-3.7.1/tests/data/MutatorSansLite/MutatorSans_v5_several_vfs.designspace`

 * *Files identical despite different names*

## Comparing `fontmake-3.7.0b3/tests/data/MutatorSansLite/MutatorSans_v5_several_vfs_discrete_axis.designspace` & `fontmake-3.7.1/tests/data/MutatorSansLite/MutatorSans_v5_several_vfs_discrete_axis.designspace`

 * *Files identical despite different names*

## Comparing `fontmake-3.7.0b3/tests/data/MutatorSansLite/MutatorSans_v5_implicit_one_vf.designspace` & `fontmake-3.7.1/tests/data/MutatorSansLite/MutatorSans_v5_implicit_one_vf.designspace`

 * *Files identical despite different names*

## Comparing `fontmake-3.7.0b3/tests/data/MutatorSansLite/LICENSE` & `fontmake-3.7.1/tests/data/MutatorSans/LICENSE`

 * *Files identical despite different names*

## Comparing `fontmake-3.7.0b3/tests/data/MutatorSansLite/MutatorFamily_v5_discrete_axis.designspace` & `fontmake-3.7.1/tests/data/MutatorSansLite/MutatorFamily_v5_discrete_axis.designspace`

 * *Files identical despite different names*

## Comparing `fontmake-3.7.0b3/tests/data/MutatorSansLite/MutatorSansLightWide.ufo/fontinfo.plist` & `fontmake-3.7.1/tests/data/MutatorSansLite/MutatorSansLightWide.ufo/fontinfo.plist`

 * *Files identical despite different names*

## Comparing `fontmake-3.7.0b3/tests/data/MutatorSansLite/MutatorSansLightWide.ufo/lib.plist` & `fontmake-3.7.1/tests/data/MutatorSansLite/MutatorSansLightWide.ufo/lib.plist`

 * *Files identical despite different names*

## Comparing `fontmake-3.7.0b3/tests/data/MutatorSansLite/MutatorSansLightWide.ufo/glyphs.background/S_.closed.glif` & `fontmake-3.7.1/tests/data/MutatorSansLite/MutatorSansLightWide.ufo/glyphs.background/S_.closed.glif`

 * *Files identical despite different names*

## Comparing `fontmake-3.7.0b3/tests/data/MutatorSansLite/MutatorSansLightWide.ufo/glyphs.master_width_720.00_weight_645.00/S_.glif` & `fontmake-3.7.1/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs.master_width_720.00_weight_645.00/S_.glif`

 * *Files identical despite different names*

## Comparing `fontmake-3.7.0b3/tests/data/MutatorSansLite/MutatorSansLightWide.ufo/glyphs.master_width_500.00_weight_500.00/S_.glif` & `fontmake-3.7.1/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs.master_width_500.00_weight_500.00/S_.glif`

 * *Files identical despite different names*

## Comparing `fontmake-3.7.0b3/tests/data/MutatorSansLite/MutatorSansLightWide.ufo/glyphs/S_.closed.glif` & `fontmake-3.7.1/tests/data/MutatorSansLite/MutatorSansLightWide.ufo/glyphs/S_.closed.glif`

 * *Files identical despite different names*

## Comparing `fontmake-3.7.0b3/tests/data/MutatorSansLite/MutatorSansLightWide.ufo/glyphs/I_.narrow.glif` & `fontmake-3.7.1/tests/data/MutatorSansLite/MutatorSansLightWide.ufo/glyphs/I_.narrow.glif`

 * *Files identical despite different names*

## Comparing `fontmake-3.7.0b3/tests/data/MutatorSansLite/MutatorSansLightWide.ufo/glyphs/I_.glif` & `fontmake-3.7.1/tests/data/MutatorSansLite/MutatorSansLightWide.ufo/glyphs/I_.glif`

 * *Files identical despite different names*

## Comparing `fontmake-3.7.0b3/tests/data/MutatorSansLite/MutatorSansLightWide.ufo/glyphs/I_J_.glif` & `fontmake-3.7.1/tests/data/MutatorSansLite/MutatorSansLightWide.ufo/glyphs/I_J_.glif`

 * *Files identical despite different names*

## Comparing `fontmake-3.7.0b3/tests/data/MutatorSansLite/MutatorSansLightWide.ufo/glyphs/A_.glif` & `fontmake-3.7.1/tests/data/MutatorSansLite/MutatorSansLightWide.ufo/glyphs/A_.glif`

 * *Files identical despite different names*

## Comparing `fontmake-3.7.0b3/tests/data/MutatorSansLite/MutatorSansLightWide.ufo/glyphs/S_.glif` & `fontmake-3.7.1/tests/data/MutatorSansLite/MutatorSansLightWide.ufo/glyphs/S_.glif`

 * *Files identical despite different names*

## Comparing `fontmake-3.7.0b3/tests/data/MutatorSansLite/MutatorSerifLightWide.ufo/fontinfo.plist` & `fontmake-3.7.1/tests/data/MutatorSansLite/MutatorSerifLightWide.ufo/fontinfo.plist`

 * *Files identical despite different names*

## Comparing `fontmake-3.7.0b3/tests/data/MutatorSansLite/MutatorSerifLightWide.ufo/lib.plist` & `fontmake-3.7.1/tests/data/MutatorSansLite/MutatorSerifLightWide.ufo/lib.plist`

 * *Files identical despite different names*

## Comparing `fontmake-3.7.0b3/tests/data/MutatorSansLite/MutatorSerifLightWide.ufo/glyphs/A_.glif` & `fontmake-3.7.1/tests/data/MutatorSansLite/MutatorSerifLightWide.ufo/glyphs/A_.glif`

 * *Files identical despite different names*

## Comparing `fontmake-3.7.0b3/tests/data/MutatorSansLite/MutatorSansBoldCondensed.ufo/fontinfo.plist` & `fontmake-3.7.1/tests/data/MutatorSansLite/MutatorSansBoldCondensed.ufo/fontinfo.plist`

 * *Files identical despite different names*

## Comparing `fontmake-3.7.0b3/tests/data/MutatorSansLite/MutatorSansBoldCondensed.ufo/lib.plist` & `fontmake-3.7.1/tests/data/MutatorSansLite/MutatorSansBoldCondensed.ufo/lib.plist`

 * *Files identical despite different names*

## Comparing `fontmake-3.7.0b3/tests/data/MutatorSansLite/MutatorSansBoldCondensed.ufo/glyphs.background/S_.closed.glif` & `fontmake-3.7.1/tests/data/MutatorSansLite/MutatorSansBoldCondensed.ufo/glyphs.background/S_.closed.glif`

 * *Files identical despite different names*

## Comparing `fontmake-3.7.0b3/tests/data/MutatorSansLite/MutatorSansBoldCondensed.ufo/glyphs/S_.closed.glif` & `fontmake-3.7.1/tests/data/MutatorSansLite/MutatorSansBoldCondensed.ufo/glyphs/S_.closed.glif`

 * *Files identical despite different names*

## Comparing `fontmake-3.7.0b3/tests/data/MutatorSansLite/MutatorSansBoldCondensed.ufo/glyphs/I_.narrow.glif` & `fontmake-3.7.1/tests/data/MutatorSansLite/MutatorSansBoldCondensed.ufo/glyphs/I_.narrow.glif`

 * *Files identical despite different names*

## Comparing `fontmake-3.7.0b3/tests/data/MutatorSansLite/MutatorSansBoldCondensed.ufo/glyphs/I_.glif` & `fontmake-3.7.1/tests/data/MutatorSansLite/MutatorSansBoldCondensed.ufo/glyphs/I_.glif`

 * *Files identical despite different names*

## Comparing `fontmake-3.7.0b3/tests/data/MutatorSansLite/MutatorSansBoldCondensed.ufo/glyphs/I_J_.glif` & `fontmake-3.7.1/tests/data/MutatorSansLite/MutatorSansBoldCondensed.ufo/glyphs/I_J_.glif`

 * *Files identical despite different names*

## Comparing `fontmake-3.7.0b3/tests/data/MutatorSansLite/MutatorSansBoldCondensed.ufo/glyphs/A_.glif` & `fontmake-3.7.1/tests/data/MutatorSansLite/MutatorSansBoldCondensed.ufo/glyphs/A_.glif`

 * *Files identical despite different names*

## Comparing `fontmake-3.7.0b3/tests/data/MutatorSansLite/MutatorSansBoldCondensed.ufo/glyphs/S_.glif` & `fontmake-3.7.1/tests/data/MutatorSansLite/MutatorSansBoldCondensed.ufo/glyphs/S_.glif`

 * *Files identical despite different names*

## Comparing `fontmake-3.7.0b3/tests/data/MutatorSansLite/MutatorSerifLightCondensed.ufo/fontinfo.plist` & `fontmake-3.7.1/tests/data/MutatorSansLite/MutatorSerifLightCondensed.ufo/fontinfo.plist`

 * *Files identical despite different names*

## Comparing `fontmake-3.7.0b3/tests/data/MutatorSansLite/MutatorSerifLightCondensed.ufo/lib.plist` & `fontmake-3.7.1/tests/data/MutatorSansLite/MutatorSansLightCondensed.ufo/lib.plist`

 * *Files identical despite different names*

## Comparing `fontmake-3.7.0b3/tests/data/MutatorSansLite/MutatorSerifLightCondensed.ufo/glyphs/A_.glif` & `fontmake-3.7.1/tests/data/MutatorSansLite/MutatorSerifLightCondensed.ufo/glyphs/A_.glif`

 * *Files identical despite different names*

## Comparing `fontmake-3.7.0b3/tests/data/MutatorSansLite/MutatorSansBoldWide.ufo/fontinfo.plist` & `fontmake-3.7.1/tests/data/MutatorSansLite/MutatorSansBoldWide.ufo/fontinfo.plist`

 * *Files identical despite different names*

## Comparing `fontmake-3.7.0b3/tests/data/MutatorSansLite/MutatorSansBoldWide.ufo/lib.plist` & `fontmake-3.7.1/tests/data/MutatorSansLite/MutatorSansBoldWide.ufo/lib.plist`

 * *Files identical despite different names*

## Comparing `fontmake-3.7.0b3/tests/data/MutatorSansLite/MutatorSansBoldWide.ufo/glyphs.background/S_.closed.glif` & `fontmake-3.7.1/tests/data/MutatorSansLite/MutatorSansBoldWide.ufo/glyphs.background/S_.closed.glif`

 * *Files identical despite different names*

## Comparing `fontmake-3.7.0b3/tests/data/MutatorSansLite/MutatorSansBoldWide.ufo/glyphs.background/S_.glif` & `fontmake-3.7.1/tests/data/MutatorSansLite/MutatorSansBoldWide.ufo/glyphs.background/S_.glif`

 * *Files identical despite different names*

## Comparing `fontmake-3.7.0b3/tests/data/MutatorSansLite/MutatorSansBoldWide.ufo/glyphs/S_.closed.glif` & `fontmake-3.7.1/tests/data/MutatorSansLite/MutatorSansBoldWide.ufo/glyphs/S_.closed.glif`

 * *Files identical despite different names*

## Comparing `fontmake-3.7.0b3/tests/data/MutatorSansLite/MutatorSansBoldWide.ufo/glyphs/I_.narrow.glif` & `fontmake-3.7.1/tests/data/MutatorSansLite/MutatorSansBoldWide.ufo/glyphs/I_.narrow.glif`

 * *Files identical despite different names*

## Comparing `fontmake-3.7.0b3/tests/data/MutatorSansLite/MutatorSansBoldWide.ufo/glyphs/I_.glif` & `fontmake-3.7.1/tests/data/MutatorSansLite/MutatorSansBoldWide.ufo/glyphs/I_.glif`

 * *Files identical despite different names*

## Comparing `fontmake-3.7.0b3/tests/data/MutatorSansLite/MutatorSansBoldWide.ufo/glyphs/I_J_.glif` & `fontmake-3.7.1/tests/data/MutatorSansLite/MutatorSansBoldWide.ufo/glyphs/I_J_.glif`

 * *Files identical despite different names*

## Comparing `fontmake-3.7.0b3/tests/data/MutatorSansLite/MutatorSansBoldWide.ufo/glyphs/A_.glif` & `fontmake-3.7.1/tests/data/MutatorSansLite/MutatorSansBoldWide.ufo/glyphs/A_.glif`

 * *Files identical despite different names*

## Comparing `fontmake-3.7.0b3/tests/data/MutatorSansLite/MutatorSansBoldWide.ufo/glyphs/S_.glif` & `fontmake-3.7.1/tests/data/MutatorSansLite/MutatorSansBoldWide.ufo/glyphs/S_.glif`

 * *Files identical despite different names*

## Comparing `fontmake-3.7.0b3/tests/data/MutatorSansLite/MutatorSansLightCondensed.ufo/layercontents.plist` & `fontmake-3.7.1/tests/data/MutatorSansLite/MutatorSansLightCondensed.ufo/layercontents.plist`

 * *Files identical despite different names*

## Comparing `fontmake-3.7.0b3/tests/data/MutatorSansLite/MutatorSansLightCondensed.ufo/fontinfo.plist` & `fontmake-3.7.1/tests/data/MutatorSansLite/MutatorSansLightCondensed.ufo/fontinfo.plist`

 * *Files identical despite different names*

## Comparing `fontmake-3.7.0b3/tests/data/MutatorSansLite/MutatorSansLightCondensed.ufo/lib.plist` & `fontmake-3.7.1/tests/data/MutatorSansLite/MutatorSerifLightCondensed.ufo/lib.plist`

 * *Files identical despite different names*

## Comparing `fontmake-3.7.0b3/tests/data/MutatorSansLite/MutatorSansLightCondensed.ufo/glyphs.background/S_.closed.glif` & `fontmake-3.7.1/tests/data/MutatorSansLite/MutatorSansLightCondensed.ufo/glyphs.background/S_.closed.glif`

 * *Files identical despite different names*

## Comparing `fontmake-3.7.0b3/tests/data/MutatorSansLite/MutatorSansLightCondensed.ufo/glyphs.background/S_.glif` & `fontmake-3.7.1/tests/data/MutatorSansLite/MutatorSansLightCondensed.ufo/glyphs.background/S_.glif`

 * *Files identical despite different names*

## Comparing `fontmake-3.7.0b3/tests/data/MutatorSansLite/MutatorSansLightCondensed.ufo/glyphs.support.crossbar/S_.glif` & `fontmake-3.7.1/tests/data/MutatorSansLite/MutatorSansLightCondensed.ufo/glyphs.support.crossbar/S_.glif`

 * *Files identical despite different names*

## Comparing `fontmake-3.7.0b3/tests/data/MutatorSansLite/MutatorSansLightCondensed.ufo/glyphs.support/A_.glif` & `fontmake-3.7.1/tests/data/MutatorSansLite/MutatorSansLightCondensed.ufo/glyphs.support/A_.glif`

 * *Files identical despite different names*

## Comparing `fontmake-3.7.0b3/tests/data/MutatorSansLite/MutatorSansLightCondensed.ufo/glyphs.support/S_.glif` & `fontmake-3.7.1/tests/data/MutatorSansLite/MutatorSansLightCondensed.ufo/glyphs.support/S_.glif`

 * *Files identical despite different names*

## Comparing `fontmake-3.7.0b3/tests/data/MutatorSansLite/MutatorSansLightCondensed.ufo/glyphs.support.S_.middle/S_.closed.glif` & `fontmake-3.7.1/tests/data/MutatorSansLite/MutatorSansLightCondensed.ufo/glyphs.support.S_.middle/S_.closed.glif`

 * *Files identical despite different names*

## Comparing `fontmake-3.7.0b3/tests/data/MutatorSansLite/MutatorSansLightCondensed.ufo/glyphs/S_.closed.glif` & `fontmake-3.7.1/tests/data/MutatorSansLite/MutatorSansLightCondensed.ufo/glyphs/S_.closed.glif`

 * *Files identical despite different names*

## Comparing `fontmake-3.7.0b3/tests/data/MutatorSansLite/MutatorSansLightCondensed.ufo/glyphs/I_.narrow.glif` & `fontmake-3.7.1/tests/data/MutatorSansLite/MutatorSansLightCondensed.ufo/glyphs/I_.narrow.glif`

 * *Files identical despite different names*

## Comparing `fontmake-3.7.0b3/tests/data/MutatorSansLite/MutatorSansLightCondensed.ufo/glyphs/I_.glif` & `fontmake-3.7.1/tests/data/MutatorSansLite/MutatorSansLightCondensed.ufo/glyphs/I_.glif`

 * *Files identical despite different names*

## Comparing `fontmake-3.7.0b3/tests/data/MutatorSansLite/MutatorSansLightCondensed.ufo/glyphs/I_J_.glif` & `fontmake-3.7.1/tests/data/MutatorSansLite/MutatorSansLightCondensed.ufo/glyphs/I_J_.glif`

 * *Files identical despite different names*

## Comparing `fontmake-3.7.0b3/tests/data/MutatorSansLite/MutatorSansLightCondensed.ufo/glyphs/A_.glif` & `fontmake-3.7.1/tests/data/MutatorSansLite/MutatorSansLightCondensed.ufo/glyphs/A_.glif`

 * *Files identical despite different names*

## Comparing `fontmake-3.7.0b3/tests/data/MutatorSansLite/MutatorSansLightCondensed.ufo/glyphs/S_.glif` & `fontmake-3.7.1/tests/data/MutatorSansLite/MutatorSansLightCondensed.ufo/glyphs/S_.glif`

 * *Files identical despite different names*

## Comparing `fontmake-3.7.0b3/tests/data/MutatorSansLite/MutatorSansLightCondensed.ufo/glyphs.support.crossbars/E_.glif` & `fontmake-3.7.1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs.support.crossbars/E_.glif`

 * *Files identical despite different names*

## Comparing `fontmake-3.7.0b3/tests/data/MutatorSansLite/MutatorSansLightCondensed.ufo/glyphs.support.S_.wide/S_.closed.glif` & `fontmake-3.7.1/tests/data/MutatorSansLite/MutatorSansLightCondensed.ufo/glyphs.support.S_.wide/S_.closed.glif`

 * *Files identical despite different names*

## Comparing `fontmake-3.7.0b3/tests/data/MutatorSansLite/MutatorSansLightCondensed.ufo/glyphs.support.S_.wide/S_.glif` & `fontmake-3.7.1/tests/data/MutatorSansLite/MutatorSansLightCondensed.ufo/glyphs.support.S_.wide/S_.glif`

 * *Files identical despite different names*

