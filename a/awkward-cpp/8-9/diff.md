# Comparing `tmp/awkward-cpp-8.tar.gz` & `tmp/awkward-cpp-9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "awkward-cpp-8.tar", last modified: Fri Feb  3 22:54:31 2023, max compression
+gzip compressed data, was "awkward-cpp-9.tar", last modified: Thu Feb 16 15:37:39 2023, max compression
```

## Comparing `awkward-cpp-8.tar` & `awkward-cpp-9.tar`

### file list

```diff
@@ -1,1472 +1,1461 @@
--rw-r--r--   0        0        0      199 2023-02-03 22:54:31.000000 awkward-cpp-8/.gitignore
--rw-r--r--   0        0        0     4936 2023-02-03 22:54:31.000000 awkward-cpp-8/CMakeLists.txt
--rw-r--r--   0        0        0     1520 2023-02-03 22:54:31.000000 awkward-cpp-8/LICENSE
--rw-r--r--   0        0        0      154 2023-02-03 22:54:31.000000 awkward-cpp-8/README.md
--rw-r--r--   0        0        0   109286 2023-02-03 22:54:31.000000 awkward-cpp-8/docs/Doxyfile
--rw-r--r--   0        0        0      773 2023-02-03 22:54:31.000000 awkward-cpp-8/docs/footer.html
--rw-r--r--   0        0        0     1057 2023-02-03 22:54:31.000000 awkward-cpp-8/docs/header.html
--rw-r--r--   0        0        0     1706 2023-02-03 22:54:31.000000 awkward-cpp-8/docs/index.md
--rw-r--r--   0        0        0      499 2023-02-03 22:54:31.000000 awkward-cpp-8/docs/stylesheet.css
--rw-r--r--   0        0        0     1859 2023-02-03 22:54:31.000000 awkward-cpp-8/header-only/awkward/BuilderOptions.h
--rw-r--r--   0        0        0    19587 2023-02-03 22:54:31.000000 awkward-cpp-8/header-only/awkward/GrowableBuffer.h
--rw-r--r--   0        0        0    89307 2023-02-03 22:54:31.000000 awkward-cpp-8/header-only/awkward/LayoutBuilder.h
--rw-r--r--   0        0        0     8025 2023-02-03 22:54:31.000000 awkward-cpp-8/header-only/awkward/utils.h
--rw-r--r--   0        0        0    13850 2023-02-03 22:54:31.000000 awkward-cpp-8/include/awkward/builder/ArrayBuilder.h
--rw-r--r--   0        0        0     2825 2023-02-03 22:54:31.000000 awkward-cpp-8/include/awkward/builder/BoolBuilder.h
--rw-r--r--   0        0        0     5702 2023-02-03 22:54:31.000000 awkward-cpp-8/include/awkward/builder/Builder.h
--rw-r--r--   0        0        0     3671 2023-02-03 22:54:31.000000 awkward-cpp-8/include/awkward/builder/Complex128Builder.h
--rw-r--r--   0        0        0     3037 2023-02-03 22:54:31.000000 awkward-cpp-8/include/awkward/builder/DatetimeBuilder.h
--rw-r--r--   0        0        0     3252 2023-02-03 22:54:31.000000 awkward-cpp-8/include/awkward/builder/Float64Builder.h
--rw-r--r--   0        0        0     2822 2023-02-03 22:54:31.000000 awkward-cpp-8/include/awkward/builder/Int64Builder.h
--rw-r--r--   0        0        0     3402 2023-02-03 22:54:31.000000 awkward-cpp-8/include/awkward/builder/ListBuilder.h
--rw-r--r--   0        0        0     3767 2023-02-03 22:54:31.000000 awkward-cpp-8/include/awkward/builder/OptionBuilder.h
--rw-r--r--   0        0        0     4505 2023-02-03 22:54:31.000000 awkward-cpp-8/include/awkward/builder/RecordBuilder.h
--rw-r--r--   0        0        0     3845 2023-02-03 22:54:31.000000 awkward-cpp-8/include/awkward/builder/StringBuilder.h
--rw-r--r--   0        0        0     3491 2023-02-03 22:54:31.000000 awkward-cpp-8/include/awkward/builder/TupleBuilder.h
--rw-r--r--   0        0        0     3583 2023-02-03 22:54:31.000000 awkward-cpp-8/include/awkward/builder/UnionBuilder.h
--rw-r--r--   0        0        0     2763 2023-02-03 22:54:31.000000 awkward-cpp-8/include/awkward/builder/UnknownBuilder.h
--rw-r--r--   0        0        0     3169 2023-02-03 22:54:31.000000 awkward-cpp-8/include/awkward/common.h
--rw-r--r--   0        0        0     3616 2023-02-03 22:54:31.000000 awkward-cpp-8/include/awkward/datetime_util.h
--rw-r--r--   0        0        0     2136 2023-02-03 22:54:31.000000 awkward-cpp-8/include/awkward/forth/ForthInputBuffer.h
--rw-r--r--   0        0        0    13079 2023-02-03 22:54:31.000000 awkward-cpp-8/include/awkward/forth/ForthMachine.h
--rw-r--r--   0        0        0     8726 2023-02-03 22:54:31.000000 awkward-cpp-8/include/awkward/forth/ForthOutputBuffer.h
--rw-r--r--   0        0        0     9197 2023-02-03 22:54:31.000000 awkward-cpp-8/include/awkward/io/json.h
--rw-r--r--   0        0        0      641 2023-02-03 22:54:31.000000 awkward-cpp-8/include/awkward/kernel-utils.h
--rw-r--r--   0        0        0   100333 2023-02-03 22:54:31.000000 awkward-cpp-8/include/awkward/kernels.h
--rw-r--r--   0        0        0     2676 2023-02-03 22:54:31.000000 awkward-cpp-8/include/awkward/python/content.h
--rw-r--r--   0        0        0      479 2023-02-03 22:54:31.000000 awkward-cpp-8/include/awkward/python/forth.h
--rw-r--r--   0        0        0      358 2023-02-03 22:54:31.000000 awkward-cpp-8/include/awkward/python/io.h
--rw-r--r--   0        0        0      416 2023-02-03 22:54:31.000000 awkward-cpp-8/include/awkward/python/kernel_utils.h
--rw-r--r--   0        0        0     1319 2023-02-03 22:54:31.000000 awkward-cpp-8/include/awkward/python/util.h
--rw-r--r--   0        0        0     8116 2023-02-03 22:54:31.000000 awkward-cpp-8/include/awkward/util.h
--rw-r--r--   0        0        0     2265 2023-02-03 22:54:31.000000 awkward-cpp-8/pyproject.toml
--rw-r--r--   0        0        0       37 2023-02-03 22:54:31.000000 awkward-cpp-8/rapidjson/.git
--rw-r--r--   0        0        0      450 2023-02-03 22:54:31.000000 awkward-cpp-8/rapidjson/.gitattributes
--rw-r--r--   0        0        0      349 2023-02-03 22:54:31.000000 awkward-cpp-8/rapidjson/.gitignore
--rw-r--r--   0        0        0      104 2023-02-03 22:54:31.000000 awkward-cpp-8/rapidjson/.gitmodules
--rw-r--r--   0        0        0     3455 2023-02-03 22:54:31.000000 awkward-cpp-8/rapidjson/.travis.yml
--rw-r--r--   0        0        0     6817 2023-02-03 22:54:31.000000 awkward-cpp-8/rapidjson/CHANGELOG.md
--rw-r--r--   0        0        0     6265 2023-02-03 22:54:31.000000 awkward-cpp-8/rapidjson/CMakeLists.txt
--rw-r--r--   0        0        0      828 2023-02-03 22:54:31.000000 awkward-cpp-8/rapidjson/CMakeModules/FindGTestSrc.cmake
--rw-r--r--   0        0        0      229 2023-02-03 22:54:31.000000 awkward-cpp-8/rapidjson/RapidJSON.pc.in
--rw-r--r--   0        0        0      200 2023-02-03 22:54:31.000000 awkward-cpp-8/rapidjson/RapidJSONConfig.cmake.in
--rw-r--r--   0        0        0      469 2023-02-03 22:54:31.000000 awkward-cpp-8/rapidjson/RapidJSONConfigVersion.cmake.in
--rw-r--r--   0        0        0     1043 2023-02-03 22:54:31.000000 awkward-cpp-8/rapidjson/appveyor.yml
--rw-r--r--   0        0        0      603 2023-02-03 22:54:31.000000 awkward-cpp-8/rapidjson/bin/data/glossary.json
--rw-r--r--   0        0        0      898 2023-02-03 22:54:31.000000 awkward-cpp-8/rapidjson/bin/data/menu.json
--rw-r--r--   0        0        0      103 2023-02-03 22:54:31.000000 awkward-cpp-8/rapidjson/bin/data/readme.txt
--rw-r--r--   0        0        0   687491 2023-02-03 22:54:31.000000 awkward-cpp-8/rapidjson/bin/data/sample.json
--rw-r--r--   0        0        0     3554 2023-02-03 22:54:31.000000 awkward-cpp-8/rapidjson/bin/data/webapp.json
--rw-r--r--   0        0        0      626 2023-02-03 22:54:31.000000 awkward-cpp-8/rapidjson/bin/data/widget.json
--rw-r--r--   0        0        0     4375 2023-02-03 22:54:31.000000 awkward-cpp-8/rapidjson/bin/draft-04/schema
--rw-r--r--   0        0        0      368 2023-02-03 22:54:31.000000 awkward-cpp-8/rapidjson/bin/encodings/utf16be.json
--rw-r--r--   0        0        0      370 2023-02-03 22:54:31.000000 awkward-cpp-8/rapidjson/bin/encodings/utf16bebom.json
--rw-r--r--   0        0        0      368 2023-02-03 22:54:31.000000 awkward-cpp-8/rapidjson/bin/encodings/utf16le.json
--rw-r--r--   0        0        0      370 2023-02-03 22:54:31.000000 awkward-cpp-8/rapidjson/bin/encodings/utf16lebom.json
--rw-r--r--   0        0        0      736 2023-02-03 22:54:31.000000 awkward-cpp-8/rapidjson/bin/encodings/utf32be.json
--rw-r--r--   0        0        0      740 2023-02-03 22:54:31.000000 awkward-cpp-8/rapidjson/bin/encodings/utf32bebom.json
--rw-r--r--   0        0        0      736 2023-02-03 22:54:31.000000 awkward-cpp-8/rapidjson/bin/encodings/utf32le.json
--rw-r--r--   0        0        0      740 2023-02-03 22:54:31.000000 awkward-cpp-8/rapidjson/bin/encodings/utf32lebom.json
--rw-r--r--   0        0        0      322 2023-02-03 22:54:31.000000 awkward-cpp-8/rapidjson/bin/encodings/utf8.json
--rw-r--r--   0        0        0      325 2023-02-03 22:54:31.000000 awkward-cpp-8/rapidjson/bin/encodings/utf8bom.json
--rw-r--r--   0        0        0       60 2023-02-03 22:54:31.000000 awkward-cpp-8/rapidjson/bin/jsonchecker/fail1.json
--rw-r--r--   0        0        0       58 2023-02-03 22:54:31.000000 awkward-cpp-8/rapidjson/bin/jsonchecker/fail10.json
--rw-r--r--   0        0        0       29 2023-02-03 22:54:31.000000 awkward-cpp-8/rapidjson/bin/jsonchecker/fail11.json
--rw-r--r--   0        0        0       31 2023-02-03 22:54:31.000000 awkward-cpp-8/rapidjson/bin/jsonchecker/fail12.json
--rw-r--r--   0        0        0       43 2023-02-03 22:54:31.000000 awkward-cpp-8/rapidjson/bin/jsonchecker/fail13.json
--rw-r--r--   0        0        0       31 2023-02-03 22:54:31.000000 awkward-cpp-8/rapidjson/bin/jsonchecker/fail14.json
--rw-r--r--   0        0        0       34 2023-02-03 22:54:31.000000 awkward-cpp-8/rapidjson/bin/jsonchecker/fail15.json
--rw-r--r--   0        0        0        8 2023-02-03 22:54:31.000000 awkward-cpp-8/rapidjson/bin/jsonchecker/fail16.json
--rw-r--r--   0        0        0       34 2023-02-03 22:54:31.000000 awkward-cpp-8/rapidjson/bin/jsonchecker/fail17.json
--rw-r--r--   0        0        0       50 2023-02-03 22:54:31.000000 awkward-cpp-8/rapidjson/bin/jsonchecker/fail18.json
--rw-r--r--   0        0        0       22 2023-02-03 22:54:31.000000 awkward-cpp-8/rapidjson/bin/jsonchecker/fail19.json
--rw-r--r--   0        0        0       17 2023-02-03 22:54:31.000000 awkward-cpp-8/rapidjson/bin/jsonchecker/fail2.json
--rw-r--r--   0        0        0       23 2023-02-03 22:54:31.000000 awkward-cpp-8/rapidjson/bin/jsonchecker/fail20.json
--rw-r--r--   0        0        0       32 2023-02-03 22:54:31.000000 awkward-cpp-8/rapidjson/bin/jsonchecker/fail21.json
--rw-r--r--   0        0        0       33 2023-02-03 22:54:31.000000 awkward-cpp-8/rapidjson/bin/jsonchecker/fail22.json
--rw-r--r--   0        0        0       20 2023-02-03 22:54:31.000000 awkward-cpp-8/rapidjson/bin/jsonchecker/fail23.json
--rw-r--r--   0        0        0       16 2023-02-03 22:54:31.000000 awkward-cpp-8/rapidjson/bin/jsonchecker/fail24.json
--rw-r--r--   0        0        0       29 2023-02-03 22:54:31.000000 awkward-cpp-8/rapidjson/bin/jsonchecker/fail25.json
--rw-r--r--   0        0        0       38 2023-02-03 22:54:31.000000 awkward-cpp-8/rapidjson/bin/jsonchecker/fail26.json
--rw-r--r--   0        0        0       14 2023-02-03 22:54:31.000000 awkward-cpp-8/rapidjson/bin/jsonchecker/fail27.json
--rw-r--r--   0        0        0       15 2023-02-03 22:54:31.000000 awkward-cpp-8/rapidjson/bin/jsonchecker/fail28.json
--rw-r--r--   0        0        0        4 2023-02-03 22:54:31.000000 awkward-cpp-8/rapidjson/bin/jsonchecker/fail29.json
--rw-r--r--   0        0        0       37 2023-02-03 22:54:31.000000 awkward-cpp-8/rapidjson/bin/jsonchecker/fail3.json
--rw-r--r--   0        0        0        5 2023-02-03 22:54:31.000000 awkward-cpp-8/rapidjson/bin/jsonchecker/fail30.json
--rw-r--r--   0        0        0        7 2023-02-03 22:54:31.000000 awkward-cpp-8/rapidjson/bin/jsonchecker/fail31.json
--rw-r--r--   0        0        0       40 2023-02-03 22:54:31.000000 awkward-cpp-8/rapidjson/bin/jsonchecker/fail32.json
--rw-r--r--   0        0        0       12 2023-02-03 22:54:31.000000 awkward-cpp-8/rapidjson/bin/jsonchecker/fail33.json
--rw-r--r--   0        0        0       16 2023-02-03 22:54:31.000000 awkward-cpp-8/rapidjson/bin/jsonchecker/fail4.json
--rw-r--r--   0        0        0       24 2023-02-03 22:54:31.000000 awkward-cpp-8/rapidjson/bin/jsonchecker/fail5.json
--rw-r--r--   0        0        0       26 2023-02-03 22:54:31.000000 awkward-cpp-8/rapidjson/bin/jsonchecker/fail6.json
--rw-r--r--   0        0        0       26 2023-02-03 22:54:31.000000 awkward-cpp-8/rapidjson/bin/jsonchecker/fail7.json
--rw-r--r--   0        0        0       16 2023-02-03 22:54:31.000000 awkward-cpp-8/rapidjson/bin/jsonchecker/fail8.json
--rw-r--r--   0        0        0       22 2023-02-03 22:54:31.000000 awkward-cpp-8/rapidjson/bin/jsonchecker/fail9.json
--rw-r--r--   0        0        0     1441 2023-02-03 22:54:31.000000 awkward-cpp-8/rapidjson/bin/jsonchecker/pass1.json
--rw-r--r--   0        0        0       52 2023-02-03 22:54:31.000000 awkward-cpp-8/rapidjson/bin/jsonchecker/pass2.json
--rw-r--r--   0        0        0      148 2023-02-03 22:54:31.000000 awkward-cpp-8/rapidjson/bin/jsonchecker/pass3.json
--rw-r--r--   0        0        0      173 2023-02-03 22:54:31.000000 awkward-cpp-8/rapidjson/bin/jsonchecker/readme.txt
--rw-r--r--   0        0        0        5 2023-02-03 22:54:31.000000 awkward-cpp-8/rapidjson/bin/jsonschema/.gitignore
--rw-r--r--   0        0        0       98 2023-02-03 22:54:31.000000 awkward-cpp-8/rapidjson/bin/jsonschema/.travis.yml
--rw-r--r--   0        0        0     1057 2023-02-03 22:54:31.000000 awkward-cpp-8/rapidjson/bin/jsonschema/LICENSE
--rw-r--r--   0        0        0     4787 2023-02-03 22:54:31.000000 awkward-cpp-8/rapidjson/bin/jsonschema/README.md
--rwxr-xr-x   0        0        0     9059 2023-02-03 22:54:31.000000 awkward-cpp-8/rapidjson/bin/jsonschema/bin/jsonschema_suite
--rw-r--r--   0        0        0     6148 2023-02-03 22:54:31.000000 awkward-cpp-8/rapidjson/bin/jsonschema/remotes/.DS_Store
--rw-r--r--   0        0        0       25 2023-02-03 22:54:31.000000 awkward-cpp-8/rapidjson/bin/jsonschema/remotes/folder/folderInteger.json
--rw-r--r--   0        0        0       25 2023-02-03 22:54:31.000000 awkward-cpp-8/rapidjson/bin/jsonschema/remotes/integer.json
--rw-r--r--   0        0        0      110 2023-02-03 22:54:31.000000 awkward-cpp-8/rapidjson/bin/jsonschema/remotes/subSchemas.json
--rw-r--r--   0        0        0     6148 2023-02-03 22:54:31.000000 awkward-cpp-8/rapidjson/bin/jsonschema/tests/.DS_Store
--rw-r--r--   0        0        0     2257 2023-02-03 22:54:31.000000 awkward-cpp-8/rapidjson/bin/jsonschema/tests/draft3/additionalItems.json
--rw-r--r--   0        0        0     2745 2023-02-03 22:54:31.000000 awkward-cpp-8/rapidjson/bin/jsonschema/tests/draft3/additionalProperties.json
--rw-r--r--   0        0        0     1273 2023-02-03 22:54:31.000000 awkward-cpp-8/rapidjson/bin/jsonschema/tests/draft3/default.json
--rw-r--r--   0        0        0     2989 2023-02-03 22:54:31.000000 awkward-cpp-8/rapidjson/bin/jsonschema/tests/draft3/dependencies.json
--rw-r--r--   0        0        0     1936 2023-02-03 22:54:31.000000 awkward-cpp-8/rapidjson/bin/jsonschema/tests/draft3/disallow.json
--rw-r--r--   0        0        0     1544 2023-02-03 22:54:31.000000 awkward-cpp-8/rapidjson/bin/jsonschema/tests/draft3/divisibleBy.json
--rw-r--r--   0        0        0     1964 2023-02-03 22:54:31.000000 awkward-cpp-8/rapidjson/bin/jsonschema/tests/draft3/enum.json
--rw-r--r--   0        0        0     2591 2023-02-03 22:54:31.000000 awkward-cpp-8/rapidjson/bin/jsonschema/tests/draft3/extends.json
--rw-r--r--   0        0        0     1136 2023-02-03 22:54:31.000000 awkward-cpp-8/rapidjson/bin/jsonschema/tests/draft3/items.json
--rw-r--r--   0        0        0      706 2023-02-03 22:54:31.000000 awkward-cpp-8/rapidjson/bin/jsonschema/tests/draft3/maxItems.json
--rw-r--r--   0        0        0      895 2023-02-03 22:54:31.000000 awkward-cpp-8/rapidjson/bin/jsonschema/tests/draft3/maxLength.json
--rw-r--r--   0        0        0     1063 2023-02-03 22:54:31.000000 awkward-cpp-8/rapidjson/bin/jsonschema/tests/draft3/maximum.json
--rw-r--r--   0        0        0      693 2023-02-03 22:54:31.000000 awkward-cpp-8/rapidjson/bin/jsonschema/tests/draft3/minItems.json
--rw-r--r--   0        0        0      886 2023-02-03 22:54:31.000000 awkward-cpp-8/rapidjson/bin/jsonschema/tests/draft3/minLength.json
--rw-r--r--   0        0        0     1063 2023-02-03 22:54:31.000000 awkward-cpp-8/rapidjson/bin/jsonschema/tests/draft3/minimum.json
--rw-r--r--   0        0        0     3075 2023-02-03 22:54:31.000000 awkward-cpp-8/rapidjson/bin/jsonschema/tests/draft3/optional/bignum.json
--rw-r--r--   0        0        0     6751 2023-02-03 22:54:31.000000 awkward-cpp-8/rapidjson/bin/jsonschema/tests/draft3/optional/format.json
--rw-r--r--   0        0        0      463 2023-02-03 22:54:31.000000 awkward-cpp-8/rapidjson/bin/jsonschema/tests/draft3/optional/jsregex.json
--rw-r--r--   0        0        0      384 2023-02-03 22:54:31.000000 awkward-cpp-8/rapidjson/bin/jsonschema/tests/draft3/optional/zeroTerminatedFloats.json
--rw-r--r--   0        0        0      857 2023-02-03 22:54:31.000000 awkward-cpp-8/rapidjson/bin/jsonschema/tests/draft3/pattern.json
--rw-r--r--   0        0        0     3365 2023-02-03 22:54:31.000000 awkward-cpp-8/rapidjson/bin/jsonschema/tests/draft3/patternProperties.json
--rw-r--r--   0        0        0     2881 2023-02-03 22:54:31.000000 awkward-cpp-8/rapidjson/bin/jsonschema/tests/draft3/properties.json
--rw-r--r--   0        0        0     4385 2023-02-03 22:54:31.000000 awkward-cpp-8/rapidjson/bin/jsonschema/tests/draft3/ref.json
--rw-r--r--   0        0        0     1961 2023-02-03 22:54:31.000000 awkward-cpp-8/rapidjson/bin/jsonschema/tests/draft3/refRemote.json
--rw-r--r--   0        0        0     1282 2023-02-03 22:54:31.000000 awkward-cpp-8/rapidjson/bin/jsonschema/tests/draft3/required.json
--rw-r--r--   0        0        0    13217 2023-02-03 22:54:31.000000 awkward-cpp-8/rapidjson/bin/jsonschema/tests/draft3/type.json
--rw-r--r--   0        0        0     2613 2023-02-03 22:54:31.000000 awkward-cpp-8/rapidjson/bin/jsonschema/tests/draft3/uniqueItems.json
--rw-r--r--   0        0        0     6148 2023-02-03 22:54:31.000000 awkward-cpp-8/rapidjson/bin/jsonschema/tests/draft4/.DS_Store
--rw-r--r--   0        0        0     2282 2023-02-03 22:54:31.000000 awkward-cpp-8/rapidjson/bin/jsonschema/tests/draft4/additionalItems.json
--rw-r--r--   0        0        0     2745 2023-02-03 22:54:31.000000 awkward-cpp-8/rapidjson/bin/jsonschema/tests/draft4/additionalProperties.json
--rw-r--r--   0        0        0     3025 2023-02-03 22:54:31.000000 awkward-cpp-8/rapidjson/bin/jsonschema/tests/draft4/allOf.json
--rw-r--r--   0        0        0     1608 2023-02-03 22:54:31.000000 awkward-cpp-8/rapidjson/bin/jsonschema/tests/draft4/anyOf.json
--rw-r--r--   0        0        0     1273 2023-02-03 22:54:31.000000 awkward-cpp-8/rapidjson/bin/jsonschema/tests/draft4/default.json
--rw-r--r--   0        0        0      854 2023-02-03 22:54:31.000000 awkward-cpp-8/rapidjson/bin/jsonschema/tests/draft4/definitions.json
--rw-r--r--   0        0        0     3139 2023-02-03 22:54:31.000000 awkward-cpp-8/rapidjson/bin/jsonschema/tests/draft4/dependencies.json
--rw-r--r--   0        0        0     1975 2023-02-03 22:54:31.000000 awkward-cpp-8/rapidjson/bin/jsonschema/tests/draft4/enum.json
--rw-r--r--   0        0        0     1136 2023-02-03 22:54:31.000000 awkward-cpp-8/rapidjson/bin/jsonschema/tests/draft4/items.json
--rw-r--r--   0        0        0      706 2023-02-03 22:54:31.000000 awkward-cpp-8/rapidjson/bin/jsonschema/tests/draft4/maxItems.json
--rw-r--r--   0        0        0      896 2023-02-03 22:54:31.000000 awkward-cpp-8/rapidjson/bin/jsonschema/tests/draft4/maxLength.json
--rw-r--r--   0        0        0      759 2023-02-03 22:54:31.000000 awkward-cpp-8/rapidjson/bin/jsonschema/tests/draft4/maxProperties.json
--rw-r--r--   0        0        0     1063 2023-02-03 22:54:31.000000 awkward-cpp-8/rapidjson/bin/jsonschema/tests/draft4/maximum.json
--rw-r--r--   0        0        0      693 2023-02-03 22:54:31.000000 awkward-cpp-8/rapidjson/bin/jsonschema/tests/draft4/minItems.json
--rw-r--r--   0        0        0      886 2023-02-03 22:54:31.000000 awkward-cpp-8/rapidjson/bin/jsonschema/tests/draft4/minLength.json
--rw-r--r--   0        0        0      725 2023-02-03 22:54:31.000000 awkward-cpp-8/rapidjson/bin/jsonschema/tests/draft4/minProperties.json
--rw-r--r--   0        0        0     1063 2023-02-03 22:54:31.000000 awkward-cpp-8/rapidjson/bin/jsonschema/tests/draft4/minimum.json
--rw-r--r--   0        0        0     1525 2023-02-03 22:54:31.000000 awkward-cpp-8/rapidjson/bin/jsonschema/tests/draft4/multipleOf.json
--rw-r--r--   0        0        0     2266 2023-02-03 22:54:31.000000 awkward-cpp-8/rapidjson/bin/jsonschema/tests/draft4/not.json
--rw-r--r--   0        0        0     1607 2023-02-03 22:54:31.000000 awkward-cpp-8/rapidjson/bin/jsonschema/tests/draft4/oneOf.json
--rw-r--r--   0        0        0     3075 2023-02-03 22:54:31.000000 awkward-cpp-8/rapidjson/bin/jsonschema/tests/draft4/optional/bignum.json
--rw-r--r--   0        0        0     4608 2023-02-03 22:54:31.000000 awkward-cpp-8/rapidjson/bin/jsonschema/tests/draft4/optional/format.json
--rw-r--r--   0        0        0      384 2023-02-03 22:54:31.000000 awkward-cpp-8/rapidjson/bin/jsonschema/tests/draft4/optional/zeroTerminatedFloats.json
--rw-r--r--   0        0        0      857 2023-02-03 22:54:31.000000 awkward-cpp-8/rapidjson/bin/jsonschema/tests/draft4/pattern.json
--rw-r--r--   0        0        0     3365 2023-02-03 22:54:31.000000 awkward-cpp-8/rapidjson/bin/jsonschema/tests/draft4/patternProperties.json
--rw-r--r--   0        0        0     2881 2023-02-03 22:54:31.000000 awkward-cpp-8/rapidjson/bin/jsonschema/tests/draft4/properties.json
--rw-r--r--   0        0        0     4366 2023-02-03 22:54:31.000000 awkward-cpp-8/rapidjson/bin/jsonschema/tests/draft4/ref.json
--rw-r--r--   0        0        0     1961 2023-02-03 22:54:31.000000 awkward-cpp-8/rapidjson/bin/jsonschema/tests/draft4/refRemote.json
--rw-r--r--   0        0        0      923 2023-02-03 22:54:31.000000 awkward-cpp-8/rapidjson/bin/jsonschema/tests/draft4/required.json
--rw-r--r--   0        0        0     9298 2023-02-03 22:54:31.000000 awkward-cpp-8/rapidjson/bin/jsonschema/tests/draft4/type.json
--rw-r--r--   0        0        0     2613 2023-02-03 22:54:31.000000 awkward-cpp-8/rapidjson/bin/jsonschema/tests/draft4/uniqueItems.json
--rw-r--r--   0        0        0      134 2023-02-03 22:54:31.000000 awkward-cpp-8/rapidjson/bin/jsonschema/tox.ini
--rwxr-xr-x   0        0        0      849 2023-02-03 22:54:31.000000 awkward-cpp-8/rapidjson/bin/types/booleans.json
--rwxr-xr-x   0        0        0     1698 2023-02-03 22:54:31.000000 awkward-cpp-8/rapidjson/bin/types/floats.json
--rwxr-xr-x   0        0        0     4202 2023-02-03 22:54:31.000000 awkward-cpp-8/rapidjson/bin/types/guids.json
--rwxr-xr-x   0        0        0     1098 2023-02-03 22:54:31.000000 awkward-cpp-8/rapidjson/bin/types/integers.json
--rwxr-xr-x   0        0        0    15142 2023-02-03 22:54:31.000000 awkward-cpp-8/rapidjson/bin/types/mixed.json
--rwxr-xr-x   0        0        0      802 2023-02-03 22:54:31.000000 awkward-cpp-8/rapidjson/bin/types/nulls.json
--rwxr-xr-x   0        0        0    33764 2023-02-03 22:54:31.000000 awkward-cpp-8/rapidjson/bin/types/paragraphs.json
--rw-r--r--   0        0        0       86 2023-02-03 22:54:31.000000 awkward-cpp-8/rapidjson/bin/types/readme.txt
--rw-r--r--   0        0        0     1009 2023-02-03 22:54:31.000000 awkward-cpp-8/rapidjson/doc/CMakeLists.txt
--rw-r--r--   0        0        0   103392 2023-02-03 22:54:31.000000 awkward-cpp-8/rapidjson/doc/Doxyfile.in
--rw-r--r--   0        0        0   103471 2023-02-03 22:54:31.000000 awkward-cpp-8/rapidjson/doc/Doxyfile.zh-cn.in
--rw-r--r--   0        0        0      912 2023-02-03 22:54:31.000000 awkward-cpp-8/rapidjson/doc/diagram/architecture.dot
--rw-r--r--   0        0        0    16569 2023-02-03 22:54:31.000000 awkward-cpp-8/rapidjson/doc/diagram/architecture.png
--rw-r--r--   0        0        0     2239 2023-02-03 22:54:31.000000 awkward-cpp-8/rapidjson/doc/diagram/insituparsing.dot
--rw-r--r--   0        0        0    37281 2023-02-03 22:54:31.000000 awkward-cpp-8/rapidjson/doc/diagram/insituparsing.png
--rw-r--r--   0        0        0     1915 2023-02-03 22:54:31.000000 awkward-cpp-8/rapidjson/doc/diagram/iterative-parser-states-diagram.dot
--rw-r--r--   0        0        0    92378 2023-02-03 22:54:31.000000 awkward-cpp-8/rapidjson/doc/diagram/iterative-parser-states-diagram.png
--rw-r--r--   0        0        0      176 2023-02-03 22:54:31.000000 awkward-cpp-8/rapidjson/doc/diagram/makefile
--rw-r--r--   0        0        0      935 2023-02-03 22:54:31.000000 awkward-cpp-8/rapidjson/doc/diagram/move1.dot
--rw-r--r--   0        0        0    16081 2023-02-03 22:54:31.000000 awkward-cpp-8/rapidjson/doc/diagram/move1.png
--rw-r--r--   0        0        0     1498 2023-02-03 22:54:31.000000 awkward-cpp-8/rapidjson/doc/diagram/move2.dot
--rw-r--r--   0        0        0    41517 2023-02-03 22:54:31.000000 awkward-cpp-8/rapidjson/doc/diagram/move2.png
--rw-r--r--   0        0        0     1450 2023-02-03 22:54:31.000000 awkward-cpp-8/rapidjson/doc/diagram/move3.dot
--rw-r--r--   0        0        0    36371 2023-02-03 22:54:31.000000 awkward-cpp-8/rapidjson/doc/diagram/move3.png
--rw-r--r--   0        0        0     1427 2023-02-03 22:54:31.000000 awkward-cpp-8/rapidjson/doc/diagram/normalparsing.dot
--rw-r--r--   0        0        0    32887 2023-02-03 22:54:31.000000 awkward-cpp-8/rapidjson/doc/diagram/normalparsing.png
--rw-r--r--   0        0        0     1435 2023-02-03 22:54:31.000000 awkward-cpp-8/rapidjson/doc/diagram/simpledom.dot
--rw-r--r--   0        0        0    43670 2023-02-03 22:54:31.000000 awkward-cpp-8/rapidjson/doc/diagram/simpledom.png
--rw-r--r--   0        0        0     1456 2023-02-03 22:54:31.000000 awkward-cpp-8/rapidjson/doc/diagram/tutorial.dot
--rw-r--r--   0        0        0    44634 2023-02-03 22:54:31.000000 awkward-cpp-8/rapidjson/doc/diagram/tutorial.png
--rw-r--r--   0        0        0     1775 2023-02-03 22:54:31.000000 awkward-cpp-8/rapidjson/doc/diagram/utilityclass.dot
--rw-r--r--   0        0        0    99993 2023-02-03 22:54:31.000000 awkward-cpp-8/rapidjson/doc/diagram/utilityclass.png
--rw-r--r--   0        0        0    15369 2023-02-03 22:54:31.000000 awkward-cpp-8/rapidjson/doc/dom.md
--rw-r--r--   0        0        0    15294 2023-02-03 22:54:31.000000 awkward-cpp-8/rapidjson/doc/dom.zh-cn.md
--rw-r--r--   0        0        0     6709 2023-02-03 22:54:31.000000 awkward-cpp-8/rapidjson/doc/encoding.md
--rw-r--r--   0        0        0     6860 2023-02-03 22:54:31.000000 awkward-cpp-8/rapidjson/doc/encoding.zh-cn.md
--rw-r--r--   0        0        0    15285 2023-02-03 22:54:31.000000 awkward-cpp-8/rapidjson/doc/faq.md
--rw-r--r--   0        0        0    14947 2023-02-03 22:54:31.000000 awkward-cpp-8/rapidjson/doc/faq.zh-cn.md
--rw-r--r--   0        0        0     5005 2023-02-03 22:54:31.000000 awkward-cpp-8/rapidjson/doc/features.md
--rw-r--r--   0        0        0     4804 2023-02-03 22:54:31.000000 awkward-cpp-8/rapidjson/doc/features.zh-cn.md
--rw-r--r--   0        0        0    22305 2023-02-03 22:54:31.000000 awkward-cpp-8/rapidjson/doc/internals.md
--rw-r--r--   0        0        0     5259 2023-02-03 22:54:31.000000 awkward-cpp-8/rapidjson/doc/logo/rapidjson.png
--rw-r--r--   0        0        0     4230 2023-02-03 22:54:31.000000 awkward-cpp-8/rapidjson/doc/logo/rapidjson.svg
--rw-r--r--   0        0        0     6090 2023-02-03 22:54:31.000000 awkward-cpp-8/rapidjson/doc/misc/DoxygenLayout.xml
--rw-r--r--   0        0        0     6572 2023-02-03 22:54:31.000000 awkward-cpp-8/rapidjson/doc/misc/doxygenextra.css
--rw-r--r--   0        0        0      256 2023-02-03 22:54:31.000000 awkward-cpp-8/rapidjson/doc/misc/footer.html
--rw-r--r--   0        0        0     1137 2023-02-03 22:54:31.000000 awkward-cpp-8/rapidjson/doc/misc/header.html
--rw-r--r--   0        0        0      363 2023-02-03 22:54:31.000000 awkward-cpp-8/rapidjson/doc/npm.md
--rw-r--r--   0        0        0     1267 2023-02-03 22:54:31.000000 awkward-cpp-8/rapidjson/doc/performance.md
--rw-r--r--   0        0        0     1236 2023-02-03 22:54:31.000000 awkward-cpp-8/rapidjson/doc/performance.zh-cn.md
--rw-r--r--   0        0        0     8882 2023-02-03 22:54:31.000000 awkward-cpp-8/rapidjson/doc/pointer.md
--rw-r--r--   0        0        0     8532 2023-02-03 22:54:31.000000 awkward-cpp-8/rapidjson/doc/pointer.zh-cn.md
--rw-r--r--   0        0        0    20432 2023-02-03 22:54:31.000000 awkward-cpp-8/rapidjson/doc/sax.md
--rw-r--r--   0        0        0    19969 2023-02-03 22:54:31.000000 awkward-cpp-8/rapidjson/doc/sax.zh-cn.md
--rw-r--r--   0        0        0     9963 2023-02-03 22:54:31.000000 awkward-cpp-8/rapidjson/doc/schema.md
--rw-r--r--   0        0        0     9604 2023-02-03 22:54:31.000000 awkward-cpp-8/rapidjson/doc/schema.zh-cn.md
--rw-r--r--   0        0        0    14398 2023-02-03 22:54:31.000000 awkward-cpp-8/rapidjson/doc/stream.md
--rw-r--r--   0        0        0    14235 2023-02-03 22:54:31.000000 awkward-cpp-8/rapidjson/doc/stream.zh-cn.md
--rw-r--r--   0        0        0    21947 2023-02-03 22:54:31.000000 awkward-cpp-8/rapidjson/doc/tutorial.md
--rw-r--r--   0        0        0    21549 2023-02-03 22:54:31.000000 awkward-cpp-8/rapidjson/doc/tutorial.zh-cn.md
--rw-r--r--   0        0        0      229 2023-02-03 22:54:31.000000 awkward-cpp-8/rapidjson/docker/debian/Dockerfile
--rw-r--r--   0        0        0     1021 2023-02-03 22:54:31.000000 awkward-cpp-8/rapidjson/example/CMakeLists.txt
--rw-r--r--   0        0        0     2577 2023-02-03 22:54:31.000000 awkward-cpp-8/rapidjson/example/capitalize/capitalize.cpp
--rw-r--r--   0        0        0     1015 2023-02-03 22:54:31.000000 awkward-cpp-8/rapidjson/example/condense/condense.cpp
--rw-r--r--   0        0        0     4979 2023-02-03 22:54:31.000000 awkward-cpp-8/rapidjson/example/filterkey/filterkey.cpp
--rw-r--r--   0        0        0     5946 2023-02-03 22:54:31.000000 awkward-cpp-8/rapidjson/example/filterkeydom/filterkeydom.cpp
--rw-r--r--   0        0        0     6022 2023-02-03 22:54:31.000000 awkward-cpp-8/rapidjson/example/jsonx/jsonx.cpp
--rw-r--r--   0        0        0     2814 2023-02-03 22:54:31.000000 awkward-cpp-8/rapidjson/example/messagereader/messagereader.cpp
--rw-r--r--   0        0        0     5026 2023-02-03 22:54:31.000000 awkward-cpp-8/rapidjson/example/parsebyparts/parsebyparts.cpp
--rw-r--r--   0        0        0     1019 2023-02-03 22:54:31.000000 awkward-cpp-8/rapidjson/example/pretty/pretty.cpp
--rw-r--r--   0        0        0     2245 2023-02-03 22:54:31.000000 awkward-cpp-8/rapidjson/example/prettyauto/prettyauto.cpp
--rw-r--r--   0        0        0     2510 2023-02-03 22:54:31.000000 awkward-cpp-8/rapidjson/example/schemavalidator/schemavalidator.cpp
--rw-r--r--   0        0        0     4590 2023-02-03 22:54:31.000000 awkward-cpp-8/rapidjson/example/serialize/serialize.cpp
--rw-r--r--   0        0        0      685 2023-02-03 22:54:31.000000 awkward-cpp-8/rapidjson/example/simpledom/simpledom.cpp
--rw-r--r--   0        0        0     1868 2023-02-03 22:54:31.000000 awkward-cpp-8/rapidjson/example/simplereader/simplereader.cpp
--rw-r--r--   0        0        0     1031 2023-02-03 22:54:31.000000 awkward-cpp-8/rapidjson/example/simplewriter/simplewriter.cpp
--rw-r--r--   0        0        0     6263 2023-02-03 22:54:31.000000 awkward-cpp-8/rapidjson/example/tutorial/tutorial.cpp
--rw-r--r--   0        0        0    10311 2023-02-03 22:54:31.000000 awkward-cpp-8/rapidjson/include/rapidjson/allocators.h
--rw-r--r--   0        0        0   113794 2023-02-03 22:54:31.000000 awkward-cpp-8/rapidjson/include/rapidjson/document.h
--rw-r--r--   0        0        0    10686 2023-02-03 22:54:31.000000 awkward-cpp-8/rapidjson/include/rapidjson/encodedstream.h
--rw-r--r--   0        0        0    28553 2023-02-03 22:54:31.000000 awkward-cpp-8/rapidjson/include/rapidjson/encodings.h
--rw-r--r--   0        0        0     3870 2023-02-03 22:54:31.000000 awkward-cpp-8/rapidjson/include/rapidjson/error/en.h
--rw-r--r--   0        0        0     5824 2023-02-03 22:54:31.000000 awkward-cpp-8/rapidjson/include/rapidjson/error/error.h
--rw-r--r--   0        0        0     2988 2023-02-03 22:54:31.000000 awkward-cpp-8/rapidjson/include/rapidjson/filereadstream.h
--rw-r--r--   0        0        0     3139 2023-02-03 22:54:31.000000 awkward-cpp-8/rapidjson/include/rapidjson/filewritestream.h
--rw-r--r--   0        0        0     4035 2023-02-03 22:54:31.000000 awkward-cpp-8/rapidjson/include/rapidjson/fwd.h
--rw-r--r--   0        0        0     9139 2023-02-03 22:54:31.000000 awkward-cpp-8/rapidjson/include/rapidjson/internal/biginteger.h
--rw-r--r--   0        0        0    11512 2023-02-03 22:54:31.000000 awkward-cpp-8/rapidjson/include/rapidjson/internal/diyfp.h
--rw-r--r--   0        0        0     8172 2023-02-03 22:54:31.000000 awkward-cpp-8/rapidjson/include/rapidjson/internal/dtoa.h
--rw-r--r--   0        0        0     3022 2023-02-03 22:54:31.000000 awkward-cpp-8/rapidjson/include/rapidjson/internal/ieee754.h
--rw-r--r--   0        0        0    10306 2023-02-03 22:54:31.000000 awkward-cpp-8/rapidjson/include/rapidjson/internal/itoa.h
--rw-r--r--   0        0        0     6572 2023-02-03 22:54:31.000000 awkward-cpp-8/rapidjson/include/rapidjson/internal/meta.h
--rw-r--r--   0        0        0     3595 2023-02-03 22:54:31.000000 awkward-cpp-8/rapidjson/include/rapidjson/internal/pow10.h
--rw-r--r--   0        0        0    24825 2023-02-03 22:54:31.000000 awkward-cpp-8/rapidjson/include/rapidjson/internal/regex.h
--rw-r--r--   0        0        0     7026 2023-02-03 22:54:31.000000 awkward-cpp-8/rapidjson/include/rapidjson/internal/stack.h
--rw-r--r--   0        0        0     1897 2023-02-03 22:54:31.000000 awkward-cpp-8/rapidjson/include/rapidjson/internal/strfunc.h
--rw-r--r--   0        0        0     8672 2023-02-03 22:54:31.000000 awkward-cpp-8/rapidjson/include/rapidjson/internal/strtod.h
--rw-r--r--   0        0        0     1419 2023-02-03 22:54:31.000000 awkward-cpp-8/rapidjson/include/rapidjson/internal/swap.h
--rw-r--r--   0        0        0     3576 2023-02-03 22:54:31.000000 awkward-cpp-8/rapidjson/include/rapidjson/istreamwrapper.h
--rw-r--r--   0        0        0     2560 2023-02-03 22:54:31.000000 awkward-cpp-8/rapidjson/include/rapidjson/memorybuffer.h
--rw-r--r--   0        0        0     2667 2023-02-03 22:54:31.000000 awkward-cpp-8/rapidjson/include/rapidjson/memorystream.h
--rw-r--r--   0        0        0     8372 2023-02-03 22:54:31.000000 awkward-cpp-8/rapidjson/include/rapidjson/msinttypes/inttypes.h
--rw-r--r--   0        0        0     9386 2023-02-03 22:54:31.000000 awkward-cpp-8/rapidjson/include/rapidjson/msinttypes/stdint.h
--rw-r--r--   0        0        0     2331 2023-02-03 22:54:31.000000 awkward-cpp-8/rapidjson/include/rapidjson/ostreamwrapper.h
--rw-r--r--   0        0        0    58465 2023-02-03 22:54:31.000000 awkward-cpp-8/rapidjson/include/rapidjson/pointer.h
--rw-r--r--   0        0        0     9601 2023-02-03 22:54:31.000000 awkward-cpp-8/rapidjson/include/rapidjson/prettywriter.h
--rw-r--r--   0        0        0    21461 2023-02-03 22:54:31.000000 awkward-cpp-8/rapidjson/include/rapidjson/rapidjson.h
--rw-r--r--   0        0        0    79760 2023-02-03 22:54:31.000000 awkward-cpp-8/rapidjson/include/rapidjson/reader.h
--rw-r--r--   0        0        0    80014 2023-02-03 22:54:31.000000 awkward-cpp-8/rapidjson/include/rapidjson/schema.h
--rw-r--r--   0        0        0     5466 2023-02-03 22:54:31.000000 awkward-cpp-8/rapidjson/include/rapidjson/stream.h
--rw-r--r--   0        0        0     3798 2023-02-03 22:54:31.000000 awkward-cpp-8/rapidjson/include/rapidjson/stringbuffer.h
--rw-r--r--   0        0        0    23261 2023-02-03 22:54:31.000000 awkward-cpp-8/rapidjson/include/rapidjson/writer.h
--rw-r--r--   0        0        0       94 2023-02-03 22:54:31.000000 awkward-cpp-8/rapidjson/include_dirs.js
--rw-r--r--   0        0        0      313 2023-02-03 22:54:31.000000 awkward-cpp-8/rapidjson/library.json
--rw-r--r--   0        0        0     5152 2023-02-03 22:54:31.000000 awkward-cpp-8/rapidjson/license.txt
--rw-r--r--   0        0        0      561 2023-02-03 22:54:31.000000 awkward-cpp-8/rapidjson/package.json
--rw-r--r--   0        0        0     3286 2023-02-03 22:54:31.000000 awkward-cpp-8/rapidjson/rapidjson.autopkg
--rw-r--r--   0        0        0     8913 2023-02-03 22:54:31.000000 awkward-cpp-8/rapidjson/readme.md
--rw-r--r--   0        0        0     8704 2023-02-03 22:54:31.000000 awkward-cpp-8/rapidjson/readme.zh-cn.md
--rw-r--r--   0        0        0      491 2023-02-03 22:54:31.000000 awkward-cpp-8/rapidjson/test/CMakeLists.txt
--rw-r--r--   0        0        0      765 2023-02-03 22:54:31.000000 awkward-cpp-8/rapidjson/test/perftest/CMakeLists.txt
--rw-r--r--   0        0        0    35486 2023-02-03 22:54:31.000000 awkward-cpp-8/rapidjson/test/perftest/misctest.cpp
--rw-r--r--   0        0        0      996 2023-02-03 22:54:31.000000 awkward-cpp-8/rapidjson/test/perftest/perftest.cpp
--rw-r--r--   0        0        0     5643 2023-02-03 22:54:31.000000 awkward-cpp-8/rapidjson/test/perftest/perftest.h
--rw-r--r--   0        0        0     4476 2023-02-03 22:54:31.000000 awkward-cpp-8/rapidjson/test/perftest/platformtest.cpp
--rw-r--r--   0        0        0    12440 2023-02-03 22:54:31.000000 awkward-cpp-8/rapidjson/test/perftest/rapidjsontest.cpp
--rw-r--r--   0        0        0     7095 2023-02-03 22:54:31.000000 awkward-cpp-8/rapidjson/test/perftest/schematest.cpp
--rw-r--r--   0        0        0     3156 2023-02-03 22:54:31.000000 awkward-cpp-8/rapidjson/test/unittest/CMakeLists.txt
--rw-r--r--   0        0        0     3308 2023-02-03 22:54:31.000000 awkward-cpp-8/rapidjson/test/unittest/allocatorstest.cpp
--rw-r--r--   0        0        0     4221 2023-02-03 22:54:31.000000 awkward-cpp-8/rapidjson/test/unittest/bigintegertest.cpp
--rw-r--r--   0        0        0    20694 2023-02-03 22:54:31.000000 awkward-cpp-8/rapidjson/test/unittest/documenttest.cpp
--rw-r--r--   0        0        0     3403 2023-02-03 22:54:31.000000 awkward-cpp-8/rapidjson/test/unittest/dtoatest.cpp
--rw-r--r--   0        0        0    12025 2023-02-03 22:54:31.000000 awkward-cpp-8/rapidjson/test/unittest/encodedstreamtest.cpp
--rw-r--r--   0        0        0    19364 2023-02-03 22:54:31.000000 awkward-cpp-8/rapidjson/test/unittest/encodingstest.cpp
--rw-r--r--   0        0        0     3218 2023-02-03 22:54:31.000000 awkward-cpp-8/rapidjson/test/unittest/filestreamtest.cpp
--rw-r--r--   0        0        0     5744 2023-02-03 22:54:31.000000 awkward-cpp-8/rapidjson/test/unittest/fwdtest.cpp
--rw-r--r--   0        0        0     5373 2023-02-03 22:54:31.000000 awkward-cpp-8/rapidjson/test/unittest/istreamwrappertest.cpp
--rw-r--r--   0        0        0     3966 2023-02-03 22:54:31.000000 awkward-cpp-8/rapidjson/test/unittest/itoatest.cpp
--rw-r--r--   0        0        0     3178 2023-02-03 22:54:31.000000 awkward-cpp-8/rapidjson/test/unittest/jsoncheckertest.cpp
--rw-r--r--   0        0        0     2422 2023-02-03 22:54:31.000000 awkward-cpp-8/rapidjson/test/unittest/namespacetest.cpp
--rw-r--r--   0        0        0     2459 2023-02-03 22:54:31.000000 awkward-cpp-8/rapidjson/test/unittest/ostreamwrappertest.cpp
--rw-r--r--   0        0        0    55407 2023-02-03 22:54:31.000000 awkward-cpp-8/rapidjson/test/unittest/pointertest.cpp
--rw-r--r--   0        0        0     5766 2023-02-03 22:54:31.000000 awkward-cpp-8/rapidjson/test/unittest/prettywritertest.cpp
--rw-r--r--   0        0        0    70515 2023-02-03 22:54:31.000000 awkward-cpp-8/rapidjson/test/unittest/readertest.cpp
--rw-r--r--   0        0        0    16157 2023-02-03 22:54:31.000000 awkward-cpp-8/rapidjson/test/unittest/regextest.cpp
--rw-r--r--   0        0        0    47377 2023-02-03 22:54:31.000000 awkward-cpp-8/rapidjson/test/unittest/schematest.cpp
--rw-r--r--   0        0        0     6920 2023-02-03 22:54:31.000000 awkward-cpp-8/rapidjson/test/unittest/simdtest.cpp
--rw-r--r--   0        0        0     1337 2023-02-03 22:54:31.000000 awkward-cpp-8/rapidjson/test/unittest/strfunctest.cpp
--rw-r--r--   0        0        0     4834 2023-02-03 22:54:31.000000 awkward-cpp-8/rapidjson/test/unittest/stringbuffertest.cpp
--rw-r--r--   0        0        0     4273 2023-02-03 22:54:31.000000 awkward-cpp-8/rapidjson/test/unittest/strtodtest.cpp
--rw-r--r--   0        0        0     1548 2023-02-03 22:54:31.000000 awkward-cpp-8/rapidjson/test/unittest/unittest.cpp
--rw-r--r--   0        0        0     3766 2023-02-03 22:54:31.000000 awkward-cpp-8/rapidjson/test/unittest/unittest.h
--rw-r--r--   0        0        0    54940 2023-02-03 22:54:31.000000 awkward-cpp-8/rapidjson/test/unittest/valuetest.cpp
--rw-r--r--   0        0        0    14988 2023-02-03 22:54:31.000000 awkward-cpp-8/rapidjson/test/unittest/writertest.cpp
--rwxr-xr-x   0        0        0     3247 2023-02-03 22:54:31.000000 awkward-cpp-8/rapidjson/travis-doxygen.sh
--rw-r--r--   0        0        0       89 2023-02-03 22:54:31.000000 awkward-cpp-8/src/awkward_cpp/__init__.py
--rw-r--r--   0        0        0   147724 2023-02-03 22:54:31.000000 awkward-cpp-8/src/awkward_cpp/_kernel_signatures.py
--rw-r--r--   0        0        0      755 2023-02-03 22:54:31.000000 awkward-cpp-8/src/awkward_cpp/cpu_kernels.py
--rw-r--r--   0        0        0     8701 2023-02-03 22:54:31.000000 awkward-cpp-8/src/awkward_cpp/libawkward.py
--rw-r--r--   0        0        0     2033 2023-02-03 22:54:31.000000 awkward-cpp-8/src/cpu-kernels/awkward_BitMaskedArray_to_ByteMaskedArray.cpp
--rw-r--r--   0        0        0     3614 2023-02-03 22:54:31.000000 awkward-cpp-8/src/cpu-kernels/awkward_BitMaskedArray_to_IndexedOptionArray.cpp
--rw-r--r--   0        0        0      796 2023-02-03 22:54:31.000000 awkward-cpp-8/src/cpu-kernels/awkward_ByteMaskedArray_getitem_nextcarry.cpp
--rw-r--r--   0        0        0      949 2023-02-03 22:54:31.000000 awkward-cpp-8/src/cpu-kernels/awkward_ByteMaskedArray_getitem_nextcarry_outindex.cpp
--rw-r--r--   0        0        0      511 2023-02-03 22:54:31.000000 awkward-cpp-8/src/cpu-kernels/awkward_ByteMaskedArray_numnull.cpp
--rw-r--r--   0        0        0      863 2023-02-03 22:54:31.000000 awkward-cpp-8/src/cpu-kernels/awkward_ByteMaskedArray_overlay_mask.cpp
--rw-r--r--   0        0        0      702 2023-02-03 22:54:31.000000 awkward-cpp-8/src/cpu-kernels/awkward_ByteMaskedArray_reduce_next_64.cpp
--rw-r--r--   0        0        0      646 2023-02-03 22:54:31.000000 awkward-cpp-8/src/cpu-kernels/awkward_ByteMaskedArray_reduce_next_nonlocal_nextshifts_64.cpp
--rw-r--r--   0        0        0      705 2023-02-03 22:54:31.000000 awkward-cpp-8/src/cpu-kernels/awkward_ByteMaskedArray_reduce_next_nonlocal_nextshifts_fromshifts_64.cpp
--rw-r--r--   0        0        0      769 2023-02-03 22:54:31.000000 awkward-cpp-8/src/cpu-kernels/awkward_ByteMaskedArray_toIndexedOptionArray.cpp
--rw-r--r--   0        0        0      757 2023-02-03 22:54:31.000000 awkward-cpp-8/src/cpu-kernels/awkward_Content_getitem_next_missing_jagged_getmaskstartstop.cpp
--rw-r--r--   0        0        0     1443 2023-02-03 22:54:31.000000 awkward-cpp-8/src/cpu-kernels/awkward_Index_iscontiguous.cpp
--rw-r--r--   0        0        0      744 2023-02-03 22:54:31.000000 awkward-cpp-8/src/cpu-kernels/awkward_Index_nones_as_index.cpp
--rw-r--r--   0        0        0     1416 2023-02-03 22:54:31.000000 awkward-cpp-8/src/cpu-kernels/awkward_IndexedArray_fill.cpp
--rw-r--r--   0        0        0      705 2023-02-03 22:54:31.000000 awkward-cpp-8/src/cpu-kernels/awkward_IndexedArray_fill_count.cpp
--rw-r--r--   0        0        0     1491 2023-02-03 22:54:31.000000 awkward-cpp-8/src/cpu-kernels/awkward_IndexedArray_flatten_nextcarry.cpp
--rw-r--r--   0        0        0     1934 2023-02-03 22:54:31.000000 awkward-cpp-8/src/cpu-kernels/awkward_IndexedArray_flatten_none2empty.cpp
--rw-r--r--   0        0        0     1490 2023-02-03 22:54:31.000000 awkward-cpp-8/src/cpu-kernels/awkward_IndexedArray_getitem_nextcarry.cpp
--rw-r--r--   0        0        0     1741 2023-02-03 22:54:31.000000 awkward-cpp-8/src/cpu-kernels/awkward_IndexedArray_getitem_nextcarry_outindex.cpp
--rw-r--r--   0        0        0     1518 2023-02-03 22:54:31.000000 awkward-cpp-8/src/cpu-kernels/awkward_IndexedArray_index_of_nulls.cpp
--rw-r--r--   0        0        0      779 2023-02-03 22:54:31.000000 awkward-cpp-8/src/cpu-kernels/awkward_IndexedArray_local_preparenext_64.cpp
--rw-r--r--   0        0        0     1108 2023-02-03 22:54:31.000000 awkward-cpp-8/src/cpu-kernels/awkward_IndexedArray_numnull.cpp
--rw-r--r--   0        0        0     1362 2023-02-03 22:54:31.000000 awkward-cpp-8/src/cpu-kernels/awkward_IndexedArray_numnull_parents.cpp
--rw-r--r--   0        0        0      440 2023-02-03 22:54:31.000000 awkward-cpp-8/src/cpu-kernels/awkward_IndexedArray_numnull_unique.cpp
--rw-r--r--   0        0        0     1314 2023-02-03 22:54:31.000000 awkward-cpp-8/src/cpu-kernels/awkward_IndexedArray_overlay_mask.cpp
--rw-r--r--   0        0        0     1640 2023-02-03 22:54:31.000000 awkward-cpp-8/src/cpu-kernels/awkward_IndexedArray_ranges_carry_next_64.cpp
--rw-r--r--   0        0        0     1866 2023-02-03 22:54:31.000000 awkward-cpp-8/src/cpu-kernels/awkward_IndexedArray_ranges_next_64.cpp
--rw-r--r--   0        0        0     1640 2023-02-03 22:54:31.000000 awkward-cpp-8/src/cpu-kernels/awkward_IndexedArray_reduce_next_64.cpp
--rw-r--r--   0        0        0      553 2023-02-03 22:54:31.000000 awkward-cpp-8/src/cpu-kernels/awkward_IndexedArray_reduce_next_fix_offsets_64.cpp
--rw-r--r--   0        0        0     1367 2023-02-03 22:54:31.000000 awkward-cpp-8/src/cpu-kernels/awkward_IndexedArray_reduce_next_nonlocal_nextshifts_64.cpp
--rw-r--r--   0        0        0     1603 2023-02-03 22:54:31.000000 awkward-cpp-8/src/cpu-kernels/awkward_IndexedArray_reduce_next_nonlocal_nextshifts_fromshifts_64.cpp
--rw-r--r--   0        0        0     3642 2023-02-03 22:54:31.000000 awkward-cpp-8/src/cpu-kernels/awkward_IndexedArray_simplify.cpp
--rw-r--r--   0        0        0      890 2023-02-03 22:54:31.000000 awkward-cpp-8/src/cpu-kernels/awkward_IndexedArray_unique_next_index_and_offsets_64.cpp
--rw-r--r--   0        0        0     1391 2023-02-03 22:54:31.000000 awkward-cpp-8/src/cpu-kernels/awkward_IndexedArray_validity.cpp
--rw-r--r--   0        0        0      831 2023-02-03 22:54:31.000000 awkward-cpp-8/src/cpu-kernels/awkward_IndexedOptionArray_rpad_and_clip_mask_axis1.cpp
--rw-r--r--   0        0        0     2305 2023-02-03 22:54:31.000000 awkward-cpp-8/src/cpu-kernels/awkward_ListArray_broadcast_tooffsets.cpp
--rw-r--r--   0        0        0     1940 2023-02-03 22:54:31.000000 awkward-cpp-8/src/cpu-kernels/awkward_ListArray_combinations.cpp
--rw-r--r--   0        0        0     2228 2023-02-03 22:54:31.000000 awkward-cpp-8/src/cpu-kernels/awkward_ListArray_combinations_length.cpp
--rw-r--r--   0        0        0     1507 2023-02-03 22:54:31.000000 awkward-cpp-8/src/cpu-kernels/awkward_ListArray_compact_offsets.cpp
--rw-r--r--   0        0        0     1855 2023-02-03 22:54:31.000000 awkward-cpp-8/src/cpu-kernels/awkward_ListArray_fill.cpp
--rw-r--r--   0        0        0     3482 2023-02-03 22:54:31.000000 awkward-cpp-8/src/cpu-kernels/awkward_ListArray_getitem_jagged_apply.cpp
--rw-r--r--   0        0        0      860 2023-02-03 22:54:31.000000 awkward-cpp-8/src/cpu-kernels/awkward_ListArray_getitem_jagged_carrylen.cpp
--rw-r--r--   0        0        0     2200 2023-02-03 22:54:31.000000 awkward-cpp-8/src/cpu-kernels/awkward_ListArray_getitem_jagged_descend.cpp
--rw-r--r--   0        0        0     2417 2023-02-03 22:54:31.000000 awkward-cpp-8/src/cpu-kernels/awkward_ListArray_getitem_jagged_expand.cpp
--rw-r--r--   0        0        0     1423 2023-02-03 22:54:31.000000 awkward-cpp-8/src/cpu-kernels/awkward_ListArray_getitem_jagged_numvalid.cpp
--rw-r--r--   0        0        0     1619 2023-02-03 22:54:31.000000 awkward-cpp-8/src/cpu-kernels/awkward_ListArray_getitem_jagged_shrink.cpp
--rw-r--r--   0        0        0     2600 2023-02-03 22:54:31.000000 awkward-cpp-8/src/cpu-kernels/awkward_ListArray_getitem_next_array.cpp
--rw-r--r--   0        0        0     2820 2023-02-03 22:54:31.000000 awkward-cpp-8/src/cpu-kernels/awkward_ListArray_getitem_next_array_advanced.cpp
--rw-r--r--   0        0        0     1674 2023-02-03 22:54:31.000000 awkward-cpp-8/src/cpu-kernels/awkward_ListArray_getitem_next_at.cpp
--rw-r--r--   0        0        0     2855 2023-02-03 22:54:31.000000 awkward-cpp-8/src/cpu-kernels/awkward_ListArray_getitem_next_range.cpp
--rw-r--r--   0        0        0     2320 2023-02-03 22:54:31.000000 awkward-cpp-8/src/cpu-kernels/awkward_ListArray_getitem_next_range_carrylength.cpp
--rw-r--r--   0        0        0     1237 2023-02-03 22:54:31.000000 awkward-cpp-8/src/cpu-kernels/awkward_ListArray_getitem_next_range_counts.cpp
--rw-r--r--   0        0        0     1625 2023-02-03 22:54:31.000000 awkward-cpp-8/src/cpu-kernels/awkward_ListArray_getitem_next_range_spreadadvanced.cpp
--rw-r--r--   0        0        0     1207 2023-02-03 22:54:31.000000 awkward-cpp-8/src/cpu-kernels/awkward_ListArray_localindex.cpp
--rw-r--r--   0        0        0     1352 2023-02-03 22:54:31.000000 awkward-cpp-8/src/cpu-kernels/awkward_ListArray_min_range.cpp
--rw-r--r--   0        0        0     1565 2023-02-03 22:54:31.000000 awkward-cpp-8/src/cpu-kernels/awkward_ListArray_rpad_and_clip_length_axis1.cpp
--rw-r--r--   0        0        0     1946 2023-02-03 22:54:31.000000 awkward-cpp-8/src/cpu-kernels/awkward_ListArray_rpad_axis1.cpp
--rw-r--r--   0        0        0     1539 2023-02-03 22:54:31.000000 awkward-cpp-8/src/cpu-kernels/awkward_ListArray_validity.cpp
--rw-r--r--   0        0        0     4055 2023-02-03 22:54:31.000000 awkward-cpp-8/src/cpu-kernels/awkward_ListOffsetArray_argsort_strings.cpp
--rw-r--r--   0        0        0     1281 2023-02-03 22:54:31.000000 awkward-cpp-8/src/cpu-kernels/awkward_ListOffsetArray_compact_offsets.cpp
--rw-r--r--   0        0        0     1482 2023-02-03 22:54:31.000000 awkward-cpp-8/src/cpu-kernels/awkward_ListOffsetArray_drop_none_indexes.cpp
--rw-r--r--   0        0        0     1692 2023-02-03 22:54:31.000000 awkward-cpp-8/src/cpu-kernels/awkward_ListOffsetArray_flatten_offsets.cpp
--rw-r--r--   0        0        0      740 2023-02-03 22:54:31.000000 awkward-cpp-8/src/cpu-kernels/awkward_ListOffsetArray_local_preparenext_64.cpp
--rw-r--r--   0        0        0      629 2023-02-03 22:54:31.000000 awkward-cpp-8/src/cpu-kernels/awkward_ListOffsetArray_reduce_local_nextparents_64.cpp
--rw-r--r--   0        0        0      673 2023-02-03 22:54:31.000000 awkward-cpp-8/src/cpu-kernels/awkward_ListOffsetArray_reduce_local_outoffsets_64.cpp
--rw-r--r--   0        0        0      694 2023-02-03 22:54:31.000000 awkward-cpp-8/src/cpu-kernels/awkward_ListOffsetArray_reduce_nonlocal_maxcount_offsetscopy_64.cpp
--rw-r--r--   0        0        0     1106 2023-02-03 22:54:31.000000 awkward-cpp-8/src/cpu-kernels/awkward_ListOffsetArray_reduce_nonlocal_nextshifts_64.cpp
--rw-r--r--   0        0        0      614 2023-02-03 22:54:31.000000 awkward-cpp-8/src/cpu-kernels/awkward_ListOffsetArray_reduce_nonlocal_nextstarts_64.cpp
--rw-r--r--   0        0        0     1412 2023-02-03 22:54:31.000000 awkward-cpp-8/src/cpu-kernels/awkward_ListOffsetArray_reduce_nonlocal_outstartsstops_64.cpp
--rw-r--r--   0        0        0     1295 2023-02-03 22:54:31.000000 awkward-cpp-8/src/cpu-kernels/awkward_ListOffsetArray_reduce_nonlocal_preparenext_64.cpp
--rw-r--r--   0        0        0     1613 2023-02-03 22:54:31.000000 awkward-cpp-8/src/cpu-kernels/awkward_ListOffsetArray_rpad_and_clip_axis1.cpp
--rw-r--r--   0        0        0     1555 2023-02-03 22:54:31.000000 awkward-cpp-8/src/cpu-kernels/awkward_ListOffsetArray_rpad_axis1.cpp
--rw-r--r--   0        0        0     1671 2023-02-03 22:54:31.000000 awkward-cpp-8/src/cpu-kernels/awkward_ListOffsetArray_rpad_length_axis1.cpp
--rw-r--r--   0        0        0     1623 2023-02-03 22:54:31.000000 awkward-cpp-8/src/cpu-kernels/awkward_ListOffsetArray_toRegularArray.cpp
--rw-r--r--   0        0        0     1651 2023-02-03 22:54:31.000000 awkward-cpp-8/src/cpu-kernels/awkward_MaskedArray_getitem_next_jagged_project.cpp
--rw-r--r--   0        0        0    35489 2023-02-03 22:54:31.000000 awkward-cpp-8/src/cpu-kernels/awkward_NumpyArray_fill.cpp
--rw-r--r--   0        0        0     2127 2023-02-03 22:54:31.000000 awkward-cpp-8/src/cpu-kernels/awkward_NumpyArray_rearrange_shifted.cpp
--rw-r--r--   0        0        0      605 2023-02-03 22:54:31.000000 awkward-cpp-8/src/cpu-kernels/awkward_NumpyArray_reduce_adjust_starts_64.cpp
--rw-r--r--   0        0        0      655 2023-02-03 22:54:31.000000 awkward-cpp-8/src/cpu-kernels/awkward_NumpyArray_reduce_adjust_starts_shifts_64.cpp
--rw-r--r--   0        0        0      562 2023-02-03 22:54:31.000000 awkward-cpp-8/src/cpu-kernels/awkward_NumpyArray_reduce_mask_ByteMaskedArray_64.cpp
--rw-r--r--   0        0        0     2095 2023-02-03 22:54:31.000000 awkward-cpp-8/src/cpu-kernels/awkward_NumpyArray_sort_asstrings_uint8.cpp
--rw-r--r--   0        0        0     4235 2023-02-03 22:54:31.000000 awkward-cpp-8/src/cpu-kernels/awkward_NumpyArray_subrange_equal.cpp
--rw-r--r--   0        0        0     1184 2023-02-03 22:54:31.000000 awkward-cpp-8/src/cpu-kernels/awkward_NumpyArray_unique_strings_uint8.cpp
--rw-r--r--   0        0        0     1018 2023-02-03 22:54:31.000000 awkward-cpp-8/src/cpu-kernels/awkward_RegularArray_broadcast_tooffsets.cpp
--rw-r--r--   0        0        0     1030 2023-02-03 22:54:31.000000 awkward-cpp-8/src/cpu-kernels/awkward_RegularArray_broadcast_tooffsets_size1.cpp
--rw-r--r--   0        0        0      802 2023-02-03 22:54:31.000000 awkward-cpp-8/src/cpu-kernels/awkward_RegularArray_combinations.cpp
--rw-r--r--   0        0        0      680 2023-02-03 22:54:31.000000 awkward-cpp-8/src/cpu-kernels/awkward_RegularArray_compact_offsets.cpp
--rw-r--r--   0        0        0      783 2023-02-03 22:54:31.000000 awkward-cpp-8/src/cpu-kernels/awkward_RegularArray_getitem_carry.cpp
--rw-r--r--   0        0        0     1009 2023-02-03 22:54:31.000000 awkward-cpp-8/src/cpu-kernels/awkward_RegularArray_getitem_jagged_expand.cpp
--rw-r--r--   0        0        0      951 2023-02-03 22:54:31.000000 awkward-cpp-8/src/cpu-kernels/awkward_RegularArray_getitem_next_array.cpp
--rw-r--r--   0        0        0     1037 2023-02-03 22:54:31.000000 awkward-cpp-8/src/cpu-kernels/awkward_RegularArray_getitem_next_array_advanced.cpp
--rw-r--r--   0        0        0      985 2023-02-03 22:54:31.000000 awkward-cpp-8/src/cpu-kernels/awkward_RegularArray_getitem_next_array_regularize.cpp
--rw-r--r--   0        0        0      904 2023-02-03 22:54:31.000000 awkward-cpp-8/src/cpu-kernels/awkward_RegularArray_getitem_next_at.cpp
--rw-r--r--   0        0        0      913 2023-02-03 22:54:31.000000 awkward-cpp-8/src/cpu-kernels/awkward_RegularArray_getitem_next_range.cpp
--rw-r--r--   0        0        0      890 2023-02-03 22:54:31.000000 awkward-cpp-8/src/cpu-kernels/awkward_RegularArray_getitem_next_range_spreadadvanced.cpp
--rw-r--r--   0        0        0      678 2023-02-03 22:54:31.000000 awkward-cpp-8/src/cpu-kernels/awkward_RegularArray_localindex.cpp
--rw-r--r--   0        0        0      647 2023-02-03 22:54:31.000000 awkward-cpp-8/src/cpu-kernels/awkward_RegularArray_reduce_local_nextparents_64.cpp
--rw-r--r--   0        0        0      800 2023-02-03 22:54:31.000000 awkward-cpp-8/src/cpu-kernels/awkward_RegularArray_reduce_nonlocal_preparenext_64.cpp
--rw-r--r--   0        0        0      920 2023-02-03 22:54:31.000000 awkward-cpp-8/src/cpu-kernels/awkward_RegularArray_rpad_and_clip_axis1.cpp
--rw-r--r--   0        0        0     1290 2023-02-03 22:54:31.000000 awkward-cpp-8/src/cpu-kernels/awkward_UnionArray_fillindex.cpp
--rw-r--r--   0        0        0      681 2023-02-03 22:54:31.000000 awkward-cpp-8/src/cpu-kernels/awkward_UnionArray_fillindex_count.cpp
--rw-r--r--   0        0        0     1105 2023-02-03 22:54:31.000000 awkward-cpp-8/src/cpu-kernels/awkward_UnionArray_fillna.cpp
--rw-r--r--   0        0        0      796 2023-02-03 22:54:31.000000 awkward-cpp-8/src/cpu-kernels/awkward_UnionArray_filltags.cpp
--rw-r--r--   0        0        0      711 2023-02-03 22:54:31.000000 awkward-cpp-8/src/cpu-kernels/awkward_UnionArray_filltags_const.cpp
--rw-r--r--   0        0        0     2163 2023-02-03 22:54:31.000000 awkward-cpp-8/src/cpu-kernels/awkward_UnionArray_flatten_combine.cpp
--rw-r--r--   0        0        0     1702 2023-02-03 22:54:31.000000 awkward-cpp-8/src/cpu-kernels/awkward_UnionArray_flatten_length.cpp
--rw-r--r--   0        0        0     1655 2023-02-03 22:54:31.000000 awkward-cpp-8/src/cpu-kernels/awkward_UnionArray_nestedfill_tags_index.cpp
--rw-r--r--   0        0        0     1564 2023-02-03 22:54:31.000000 awkward-cpp-8/src/cpu-kernels/awkward_UnionArray_project.cpp
--rw-r--r--   0        0        0     1442 2023-02-03 22:54:31.000000 awkward-cpp-8/src/cpu-kernels/awkward_UnionArray_regular_index.cpp
--rw-r--r--   0        0        0      769 2023-02-03 22:54:31.000000 awkward-cpp-8/src/cpu-kernels/awkward_UnionArray_regular_index_getsize.cpp
--rw-r--r--   0        0        0     5911 2023-02-03 22:54:31.000000 awkward-cpp-8/src/cpu-kernels/awkward_UnionArray_simplify.cpp
--rw-r--r--   0        0        0     1959 2023-02-03 22:54:31.000000 awkward-cpp-8/src/cpu-kernels/awkward_UnionArray_simplify_one.cpp
--rw-r--r--   0        0        0     1856 2023-02-03 22:54:31.000000 awkward-cpp-8/src/cpu-kernels/awkward_UnionArray_validity.cpp
--rw-r--r--   0        0        0     6448 2023-02-03 22:54:31.000000 awkward-cpp-8/src/cpu-kernels/awkward_argsort.cpp
--rw-r--r--   0        0        0      760 2023-02-03 22:54:31.000000 awkward-cpp-8/src/cpu-kernels/awkward_index_rpad_and_clip_axis0.cpp
--rw-r--r--   0        0        0      764 2023-02-03 22:54:31.000000 awkward-cpp-8/src/cpu-kernels/awkward_index_rpad_and_clip_axis1.cpp
--rw-r--r--   0        0        0      524 2023-02-03 22:54:31.000000 awkward-cpp-8/src/cpu-kernels/awkward_localindex.cpp
--rw-r--r--   0        0        0      879 2023-02-03 22:54:31.000000 awkward-cpp-8/src/cpu-kernels/awkward_missing_repeat.cpp
--rw-r--r--   0        0        0     3419 2023-02-03 22:54:31.000000 awkward-cpp-8/src/cpu-kernels/awkward_reduce_argmax.cpp
--rw-r--r--   0        0        0     1393 2023-02-03 22:54:31.000000 awkward-cpp-8/src/cpu-kernels/awkward_reduce_argmax_complex.cpp
--rw-r--r--   0        0        0     3415 2023-02-03 22:54:31.000000 awkward-cpp-8/src/cpu-kernels/awkward_reduce_argmin.cpp
--rw-r--r--   0        0        0     1393 2023-02-03 22:54:31.000000 awkward-cpp-8/src/cpu-kernels/awkward_reduce_argmin_complex.cpp
--rw-r--r--   0        0        0      509 2023-02-03 22:54:31.000000 awkward-cpp-8/src/cpu-kernels/awkward_reduce_count_64.cpp
--rw-r--r--   0        0        0     3624 2023-02-03 22:54:31.000000 awkward-cpp-8/src/cpu-kernels/awkward_reduce_countnonzero.cpp
--rw-r--r--   0        0        0     1202 2023-02-03 22:54:31.000000 awkward-cpp-8/src/cpu-kernels/awkward_reduce_countnonzero_complex.cpp
--rw-r--r--   0        0        0     3734 2023-02-03 22:54:31.000000 awkward-cpp-8/src/cpu-kernels/awkward_reduce_max.cpp
--rw-r--r--   0        0        0     1490 2023-02-03 22:54:31.000000 awkward-cpp-8/src/cpu-kernels/awkward_reduce_max_complex.cpp
--rw-r--r--   0        0        0     3734 2023-02-03 22:54:31.000000 awkward-cpp-8/src/cpu-kernels/awkward_reduce_min.cpp
--rw-r--r--   0        0        0     1488 2023-02-03 22:54:31.000000 awkward-cpp-8/src/cpu-kernels/awkward_reduce_min_complex.cpp
--rw-r--r--   0        0        0     5019 2023-02-03 22:54:31.000000 awkward-cpp-8/src/cpu-kernels/awkward_reduce_prod.cpp
--rw-r--r--   0        0        0     3519 2023-02-03 22:54:31.000000 awkward-cpp-8/src/cpu-kernels/awkward_reduce_prod_bool.cpp
--rw-r--r--   0        0        0     1178 2023-02-03 22:54:31.000000 awkward-cpp-8/src/cpu-kernels/awkward_reduce_prod_bool_complex.cpp
--rw-r--r--   0        0        0     1452 2023-02-03 22:54:31.000000 awkward-cpp-8/src/cpu-kernels/awkward_reduce_prod_complex.cpp
--rw-r--r--   0        0        0     4985 2023-02-03 22:54:31.000000 awkward-cpp-8/src/cpu-kernels/awkward_reduce_sum.cpp
--rw-r--r--   0        0        0     3496 2023-02-03 22:54:31.000000 awkward-cpp-8/src/cpu-kernels/awkward_reduce_sum_bool.cpp
--rw-r--r--   0        0        0     1173 2023-02-03 22:54:31.000000 awkward-cpp-8/src/cpu-kernels/awkward_reduce_sum_bool_complex.cpp
--rw-r--r--   0        0        0     1277 2023-02-03 22:54:31.000000 awkward-cpp-8/src/cpu-kernels/awkward_reduce_sum_complex.cpp
--rw-r--r--   0        0        0      569 2023-02-03 22:54:31.000000 awkward-cpp-8/src/cpu-kernels/awkward_reduce_sum_int32_bool_64.cpp
--rw-r--r--   0        0        0      569 2023-02-03 22:54:31.000000 awkward-cpp-8/src/cpu-kernels/awkward_reduce_sum_int64_bool_64.cpp
--rw-r--r--   0        0        0     6405 2023-02-03 22:54:31.000000 awkward-cpp-8/src/cpu-kernels/awkward_sort.cpp
--rw-r--r--   0        0        0      614 2023-02-03 22:54:31.000000 awkward-cpp-8/src/cpu-kernels/awkward_sorting_ranges.cpp
--rw-r--r--   0        0        0      522 2023-02-03 22:54:31.000000 awkward-cpp-8/src/cpu-kernels/awkward_sorting_ranges_length.cpp
--rw-r--r--   0        0        0     2351 2023-02-03 22:54:31.000000 awkward-cpp-8/src/cpu-kernels/awkward_unique.cpp
--rw-r--r--   0        0        0     2967 2023-02-03 22:54:31.000000 awkward-cpp-8/src/cpu-kernels/awkward_unique_copy.cpp
--rw-r--r--   0        0        0     1945 2023-02-03 22:54:31.000000 awkward-cpp-8/src/cpu-kernels/awkward_unique_offsets.cpp
--rw-r--r--   0        0        0     3862 2023-02-03 22:54:31.000000 awkward-cpp-8/src/cpu-kernels/awkward_unique_ranges.cpp
--rw-r--r--   0        0        0     2344 2023-02-03 22:54:31.000000 awkward-cpp-8/src/cpu-kernels/kernel-utils.cpp
--rw-r--r--   0        0        0    11115 2023-02-03 22:54:31.000000 awkward-cpp-8/src/libawkward/builder/ArrayBuilder.cpp
--rw-r--r--   0        0        0     4661 2023-02-03 22:54:31.000000 awkward-cpp-8/src/libawkward/builder/BoolBuilder.cpp
--rw-r--r--   0        0        0      183 2023-02-03 22:54:31.000000 awkward-cpp-8/src/libawkward/builder/Builder.cpp
--rw-r--r--   0        0        0     5293 2023-02-03 22:54:31.000000 awkward-cpp-8/src/libawkward/builder/Complex128Builder.cpp
--rw-r--r--   0        0        0     6147 2023-02-03 22:54:31.000000 awkward-cpp-8/src/libawkward/builder/DatetimeBuilder.cpp
--rw-r--r--   0        0        0     5141 2023-02-03 22:54:31.000000 awkward-cpp-8/src/libawkward/builder/Float64Builder.cpp
--rw-r--r--   0        0        0     4895 2023-02-03 22:54:31.000000 awkward-cpp-8/src/libawkward/builder/Int64Builder.cpp
--rw-r--r--   0        0        0     7364 2023-02-03 22:54:31.000000 awkward-cpp-8/src/libawkward/builder/ListBuilder.cpp
--rw-r--r--   0        0        0     7743 2023-02-03 22:54:31.000000 awkward-cpp-8/src/libawkward/builder/OptionBuilder.cpp
--rw-r--r--   0        0        0    18031 2023-02-03 22:54:31.000000 awkward-cpp-8/src/libawkward/builder/RecordBuilder.cpp
--rw-r--r--   0        0        0     6750 2023-02-03 22:54:31.000000 awkward-cpp-8/src/libawkward/builder/StringBuilder.cpp
--rw-r--r--   0        0        0    14161 2023-02-03 22:54:31.000000 awkward-cpp-8/src/libawkward/builder/TupleBuilder.cpp
--rw-r--r--   0        0        0    14325 2023-02-03 22:54:31.000000 awkward-cpp-8/src/libawkward/builder/UnionBuilder.cpp
--rw-r--r--   0        0        0     6182 2023-02-03 22:54:31.000000 awkward-cpp-8/src/libawkward/builder/UnknownBuilder.cpp
--rw-r--r--   0        0        0    19525 2023-02-03 22:54:31.000000 awkward-cpp-8/src/libawkward/forth/ForthInputBuffer.cpp
--rw-r--r--   0        0        0   147623 2023-02-03 22:54:31.000000 awkward-cpp-8/src/libawkward/forth/ForthMachine.cpp
--rw-r--r--   0        0        0    22713 2023-02-03 22:54:31.000000 awkward-cpp-8/src/libawkward/forth/ForthOutputBuffer.cpp
--rw-r--r--   0        0        0    43605 2023-02-03 22:54:31.000000 awkward-cpp-8/src/libawkward/io/json.cpp
--rw-r--r--   0        0        0    15701 2023-02-03 22:54:31.000000 awkward-cpp-8/src/libawkward/util.cpp
--rw-r--r--   0        0        0      726 2023-02-03 22:54:31.000000 awkward-cpp-8/src/python/_ext.cpp
--rw-r--r--   0        0        0    10142 2023-02-03 22:54:31.000000 awkward-cpp-8/src/python/content.cpp
--rw-r--r--   0        0        0    26562 2023-02-03 22:54:31.000000 awkward-cpp-8/src/python/forth.cpp
--rw-r--r--   0        0        0     3776 2023-02-03 22:54:31.000000 awkward-cpp-8/src/python/io.cpp
--rw-r--r--   0        0        0      146 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-cpu-kernels/__init__.py
--rw-r--r--   0        0        0     4641 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-cpu-kernels/test_cpuawkward_BitMaskedArray_to_ByteMaskedArray.py
--rw-r--r--   0        0        0     4247 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-cpu-kernels/test_cpuawkward_BitMaskedArray_to_IndexedOptionArray64.py
--rw-r--r--   0        0        0     2349 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-cpu-kernels/test_cpuawkward_ByteMaskedArray_getitem_nextcarry_64.py
--rw-r--r--   0        0        0     3273 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-cpu-kernels/test_cpuawkward_ByteMaskedArray_getitem_nextcarry_outindex_64.py
--rw-r--r--   0        0        0     2672 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-cpu-kernels/test_cpuawkward_ByteMaskedArray_numnull.py
--rw-r--r--   0        0        0    16212 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-cpu-kernels/test_cpuawkward_ByteMaskedArray_overlay_mask8.py
--rw-r--r--   0        0        0      413 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-cpu-kernels/test_cpuawkward_ByteMaskedArray_reduce_next_64.py
--rw-r--r--   0        0        0      433 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-cpu-kernels/test_cpuawkward_ByteMaskedArray_reduce_next_nonlocal_nextshifts_64.py
--rw-r--r--   0        0        0      444 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-cpu-kernels/test_cpuawkward_ByteMaskedArray_reduce_next_nonlocal_nextshifts_fromshifts_64.py
--rw-r--r--   0        0        0     2905 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-cpu-kernels/test_cpuawkward_ByteMaskedArray_toIndexedOptionArray64.py
--rw-r--r--   0        0        0    28927 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-cpu-kernels/test_cpuawkward_Content_getitem_next_missing_jagged_getmaskstartstop.py
--rw-r--r--   0        0        0      403 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-cpu-kernels/test_cpuawkward_Index32_iscontiguous.py
--rw-r--r--   0        0        0      403 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-cpu-kernels/test_cpuawkward_Index64_iscontiguous.py
--rw-r--r--   0        0        0      402 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-cpu-kernels/test_cpuawkward_Index8_iscontiguous.py
--rw-r--r--   0        0        0      404 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-cpu-kernels/test_cpuawkward_IndexU32_iscontiguous.py
--rw-r--r--   0        0        0      403 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-cpu-kernels/test_cpuawkward_IndexU8_iscontiguous.py
--rw-r--r--   0        0        0      406 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-cpu-kernels/test_cpuawkward_Index_nones_as_index_64.py
--rw-r--r--   0        0        0     2760 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-cpu-kernels/test_cpuawkward_IndexedArray32_flatten_nextcarry_64.py
--rw-r--r--   0        0        0    16336 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-cpu-kernels/test_cpuawkward_IndexedArray32_flatten_none2empty_64.py
--rw-r--r--   0        0        0     2760 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-cpu-kernels/test_cpuawkward_IndexedArray32_getitem_nextcarry_64.py
--rw-r--r--   0        0        0     2334 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-cpu-kernels/test_cpuawkward_IndexedArray32_getitem_nextcarry_outindex_64.py
--rw-r--r--   0        0        0      412 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-cpu-kernels/test_cpuawkward_IndexedArray32_index_of_nulls.py
--rw-r--r--   0        0        0     2681 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-cpu-kernels/test_cpuawkward_IndexedArray32_numnull.py
--rw-r--r--   0        0        0      413 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-cpu-kernels/test_cpuawkward_IndexedArray32_numnull_parents.py
--rw-r--r--   0        0        0      416 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-cpu-kernels/test_cpuawkward_IndexedArray32_overlay_mask8_to64.py
--rw-r--r--   0        0        0      418 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-cpu-kernels/test_cpuawkward_IndexedArray32_ranges_carry_next_64.py
--rw-r--r--   0        0        0      412 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-cpu-kernels/test_cpuawkward_IndexedArray32_ranges_next_64.py
--rw-r--r--   0        0        0      412 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-cpu-kernels/test_cpuawkward_IndexedArray32_reduce_next_64.py
--rw-r--r--   0        0        0      432 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-cpu-kernels/test_cpuawkward_IndexedArray32_reduce_next_nonlocal_nextshifts_64.py
--rw-r--r--   0        0        0      443 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-cpu-kernels/test_cpuawkward_IndexedArray32_reduce_next_nonlocal_nextshifts_fromshifts_64.py
--rw-r--r--   0        0        0    10112 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-cpu-kernels/test_cpuawkward_IndexedArray32_simplify32_to64.py
--rw-r--r--   0        0        0    10112 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-cpu-kernels/test_cpuawkward_IndexedArray32_simplify64_to64.py
--rw-r--r--   0        0        0    10157 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-cpu-kernels/test_cpuawkward_IndexedArray32_simplifyU32_to64.py
--rw-r--r--   0        0        0     8567 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-cpu-kernels/test_cpuawkward_IndexedArray32_validity.py
--rw-r--r--   0        0        0     2760 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-cpu-kernels/test_cpuawkward_IndexedArray64_flatten_nextcarry_64.py
--rw-r--r--   0        0        0    16336 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-cpu-kernels/test_cpuawkward_IndexedArray64_flatten_none2empty_64.py
--rw-r--r--   0        0        0     2760 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-cpu-kernels/test_cpuawkward_IndexedArray64_getitem_nextcarry_64.py
--rw-r--r--   0        0        0     2334 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-cpu-kernels/test_cpuawkward_IndexedArray64_getitem_nextcarry_outindex_64.py
--rw-r--r--   0        0        0      412 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-cpu-kernels/test_cpuawkward_IndexedArray64_index_of_nulls.py
--rw-r--r--   0        0        0     2681 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-cpu-kernels/test_cpuawkward_IndexedArray64_numnull.py
--rw-r--r--   0        0        0      413 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-cpu-kernels/test_cpuawkward_IndexedArray64_numnull_parents.py
--rw-r--r--   0        0        0      416 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-cpu-kernels/test_cpuawkward_IndexedArray64_overlay_mask8_to64.py
--rw-r--r--   0        0        0      418 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-cpu-kernels/test_cpuawkward_IndexedArray64_ranges_carry_next_64.py
--rw-r--r--   0        0        0      412 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-cpu-kernels/test_cpuawkward_IndexedArray64_ranges_next_64.py
--rw-r--r--   0        0        0      412 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-cpu-kernels/test_cpuawkward_IndexedArray64_reduce_next_64.py
--rw-r--r--   0        0        0      432 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-cpu-kernels/test_cpuawkward_IndexedArray64_reduce_next_nonlocal_nextshifts_64.py
--rw-r--r--   0        0        0      443 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-cpu-kernels/test_cpuawkward_IndexedArray64_reduce_next_nonlocal_nextshifts_fromshifts_64.py
--rw-r--r--   0        0        0    10112 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-cpu-kernels/test_cpuawkward_IndexedArray64_simplify32_to64.py
--rw-r--r--   0        0        0    10112 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-cpu-kernels/test_cpuawkward_IndexedArray64_simplify64_to64.py
--rw-r--r--   0        0        0    10157 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-cpu-kernels/test_cpuawkward_IndexedArray64_simplifyU32_to64.py
--rw-r--r--   0        0        0     8567 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-cpu-kernels/test_cpuawkward_IndexedArray64_validity.py
--rw-r--r--   0        0        0     2775 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-cpu-kernels/test_cpuawkward_IndexedArrayU32_flatten_nextcarry_64.py
--rw-r--r--   0        0        0    16411 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-cpu-kernels/test_cpuawkward_IndexedArrayU32_flatten_none2empty_64.py
--rw-r--r--   0        0        0     2775 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-cpu-kernels/test_cpuawkward_IndexedArrayU32_getitem_nextcarry_64.py
--rw-r--r--   0        0        0     2346 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-cpu-kernels/test_cpuawkward_IndexedArrayU32_getitem_nextcarry_outindex_64.py
--rw-r--r--   0        0        0      413 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-cpu-kernels/test_cpuawkward_IndexedArrayU32_index_of_nulls.py
--rw-r--r--   0        0        0     2696 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-cpu-kernels/test_cpuawkward_IndexedArrayU32_numnull.py
--rw-r--r--   0        0        0      414 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-cpu-kernels/test_cpuawkward_IndexedArrayU32_numnull_parents.py
--rw-r--r--   0        0        0      417 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-cpu-kernels/test_cpuawkward_IndexedArrayU32_overlay_mask8_to64.py
--rw-r--r--   0        0        0      419 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-cpu-kernels/test_cpuawkward_IndexedArrayU32_ranges_carry_next_64.py
--rw-r--r--   0        0        0      413 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-cpu-kernels/test_cpuawkward_IndexedArrayU32_ranges_next_64.py
--rw-r--r--   0        0        0      413 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-cpu-kernels/test_cpuawkward_IndexedArrayU32_reduce_next_64.py
--rw-r--r--   0        0        0      433 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-cpu-kernels/test_cpuawkward_IndexedArrayU32_reduce_next_nonlocal_nextshifts_64.py
--rw-r--r--   0        0        0      444 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-cpu-kernels/test_cpuawkward_IndexedArrayU32_reduce_next_nonlocal_nextshifts_fromshifts_64.py
--rw-r--r--   0        0        0    10157 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-cpu-kernels/test_cpuawkward_IndexedArrayU32_simplify32_to64.py
--rw-r--r--   0        0        0    10157 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-cpu-kernels/test_cpuawkward_IndexedArrayU32_simplify64_to64.py
--rw-r--r--   0        0        0    10202 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-cpu-kernels/test_cpuawkward_IndexedArrayU32_simplifyU32_to64.py
--rw-r--r--   0        0        0     8642 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-cpu-kernels/test_cpuawkward_IndexedArrayU32_validity.py
--rw-r--r--   0        0        0     2456 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-cpu-kernels/test_cpuawkward_IndexedArray_fill_to64_count.py
--rw-r--r--   0        0        0     3271 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-cpu-kernels/test_cpuawkward_IndexedArray_fill_to64_from32.py
--rw-r--r--   0        0        0     3271 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-cpu-kernels/test_cpuawkward_IndexedArray_fill_to64_from64.py
--rw-r--r--   0        0        0     3286 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-cpu-kernels/test_cpuawkward_IndexedArray_fill_to64_fromU32.py
--rw-r--r--   0        0        0      413 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-cpu-kernels/test_cpuawkward_IndexedArray_numnull_unique_64.py
--rw-r--r--   0        0        0      422 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-cpu-kernels/test_cpuawkward_IndexedArray_reduce_next_fix_offsets_64.py
--rw-r--r--   0        0        0      428 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-cpu-kernels/test_cpuawkward_IndexedArray_unique_next_index_and_offsets_64.py
--rw-r--r--   0        0        0     2930 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-cpu-kernels/test_cpuawkward_IndexedOptionArray_rpad_and_clip_mask_axis1_64.py
--rw-r--r--   0        0        0     1591 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-cpu-kernels/test_cpuawkward_ListArray32_broadcast_tooffsets_64.py
--rw-r--r--   0        0        0    22474 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-cpu-kernels/test_cpuawkward_ListArray32_combinations_length_64.py
--rw-r--r--   0        0        0     3611 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-cpu-kernels/test_cpuawkward_ListArray32_compact_offsets_64.py
--rw-r--r--   0        0        0    13418 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-cpu-kernels/test_cpuawkward_ListArray32_getitem_jagged_apply_64.py
--rw-r--r--   0        0        0    21484 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-cpu-kernels/test_cpuawkward_ListArray32_getitem_jagged_descend_64.py
--rw-r--r--   0        0        0     6605 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-cpu-kernels/test_cpuawkward_ListArray32_getitem_jagged_expand_64.py
--rw-r--r--   0        0        0     8006 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-cpu-kernels/test_cpuawkward_ListArray32_getitem_next_array_64.py
--rw-r--r--   0        0        0    49823 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-cpu-kernels/test_cpuawkward_ListArray32_getitem_next_array_advanced_64.py
--rw-r--r--   0        0        0     1404 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-cpu-kernels/test_cpuawkward_ListArray32_getitem_next_at_64.py
--rw-r--r--   0        0        0      416 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-cpu-kernels/test_cpuawkward_ListArray32_getitem_next_range_64.py
--rw-r--r--   0        0        0      425 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-cpu-kernels/test_cpuawkward_ListArray32_getitem_next_range_carrylength.py
--rw-r--r--   0        0        0     2861 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-cpu-kernels/test_cpuawkward_ListArray32_getitem_next_range_counts_64.py
--rw-r--r--   0        0        0      431 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-cpu-kernels/test_cpuawkward_ListArray32_getitem_next_range_spreadadvanced_64.py
--rw-r--r--   0        0        0     1768 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-cpu-kernels/test_cpuawkward_ListArray32_localindex_64.py
--rw-r--r--   0        0        0     3249 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-cpu-kernels/test_cpuawkward_ListArray32_min_range.py
--rw-r--r--   0        0        0     3535 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-cpu-kernels/test_cpuawkward_ListArray32_rpad_and_clip_length_axis1.py
--rw-r--r--   0        0        0     5894 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-cpu-kernels/test_cpuawkward_ListArray32_rpad_axis1_64.py
--rw-r--r--   0        0        0     2260 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-cpu-kernels/test_cpuawkward_ListArray32_validity.py
--rw-r--r--   0        0        0     1591 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-cpu-kernels/test_cpuawkward_ListArray64_broadcast_tooffsets_64.py
--rw-r--r--   0        0        0    22474 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-cpu-kernels/test_cpuawkward_ListArray64_combinations_length_64.py
--rw-r--r--   0        0        0     3611 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-cpu-kernels/test_cpuawkward_ListArray64_compact_offsets_64.py
--rw-r--r--   0        0        0    13418 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-cpu-kernels/test_cpuawkward_ListArray64_getitem_jagged_apply_64.py
--rw-r--r--   0        0        0    21484 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-cpu-kernels/test_cpuawkward_ListArray64_getitem_jagged_descend_64.py
--rw-r--r--   0        0        0     6605 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-cpu-kernels/test_cpuawkward_ListArray64_getitem_jagged_expand_64.py
--rw-r--r--   0        0        0     8006 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-cpu-kernels/test_cpuawkward_ListArray64_getitem_next_array_64.py
--rw-r--r--   0        0        0    49823 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-cpu-kernels/test_cpuawkward_ListArray64_getitem_next_array_advanced_64.py
--rw-r--r--   0        0        0     1404 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-cpu-kernels/test_cpuawkward_ListArray64_getitem_next_at_64.py
--rw-r--r--   0        0        0      416 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-cpu-kernels/test_cpuawkward_ListArray64_getitem_next_range_64.py
--rw-r--r--   0        0        0      425 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-cpu-kernels/test_cpuawkward_ListArray64_getitem_next_range_carrylength.py
--rw-r--r--   0        0        0     2861 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-cpu-kernels/test_cpuawkward_ListArray64_getitem_next_range_counts_64.py
--rw-r--r--   0        0        0      431 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-cpu-kernels/test_cpuawkward_ListArray64_getitem_next_range_spreadadvanced_64.py
--rw-r--r--   0        0        0     1768 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-cpu-kernels/test_cpuawkward_ListArray64_localindex_64.py
--rw-r--r--   0        0        0     3249 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-cpu-kernels/test_cpuawkward_ListArray64_min_range.py
--rw-r--r--   0        0        0     3535 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-cpu-kernels/test_cpuawkward_ListArray64_rpad_and_clip_length_axis1.py
--rw-r--r--   0        0        0     5894 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-cpu-kernels/test_cpuawkward_ListArray64_rpad_axis1_64.py
--rw-r--r--   0        0        0     2260 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-cpu-kernels/test_cpuawkward_ListArray64_validity.py
--rw-r--r--   0        0        0     1599 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-cpu-kernels/test_cpuawkward_ListArrayU32_broadcast_tooffsets_64.py
--rw-r--r--   0        0        0    22574 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-cpu-kernels/test_cpuawkward_ListArrayU32_combinations_length_64.py
--rw-r--r--   0        0        0     3631 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-cpu-kernels/test_cpuawkward_ListArrayU32_compact_offsets_64.py
--rw-r--r--   0        0        0    13458 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-cpu-kernels/test_cpuawkward_ListArrayU32_getitem_jagged_apply_64.py
--rw-r--r--   0        0        0    21584 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-cpu-kernels/test_cpuawkward_ListArrayU32_getitem_jagged_descend_64.py
--rw-r--r--   0        0        0     6625 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-cpu-kernels/test_cpuawkward_ListArrayU32_getitem_jagged_expand_64.py
--rw-r--r--   0        0        0     8034 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-cpu-kernels/test_cpuawkward_ListArrayU32_getitem_next_array_64.py
--rw-r--r--   0        0        0    49995 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-cpu-kernels/test_cpuawkward_ListArrayU32_getitem_next_array_advanced_64.py
--rw-r--r--   0        0        0     1412 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-cpu-kernels/test_cpuawkward_ListArrayU32_getitem_next_at_64.py
--rw-r--r--   0        0        0      417 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-cpu-kernels/test_cpuawkward_ListArrayU32_getitem_next_range_64.py
--rw-r--r--   0        0        0      426 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-cpu-kernels/test_cpuawkward_ListArrayU32_getitem_next_range_carrylength.py
--rw-r--r--   0        0        0     2876 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-cpu-kernels/test_cpuawkward_ListArrayU32_getitem_next_range_counts_64.py
--rw-r--r--   0        0        0      432 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-cpu-kernels/test_cpuawkward_ListArrayU32_getitem_next_range_spreadadvanced_64.py
--rw-r--r--   0        0        0     1777 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-cpu-kernels/test_cpuawkward_ListArrayU32_localindex_64.py
--rw-r--r--   0        0        0     3269 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-cpu-kernels/test_cpuawkward_ListArrayU32_min_range.py
--rw-r--r--   0        0        0     3555 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-cpu-kernels/test_cpuawkward_ListArrayU32_rpad_and_clip_length_axis1.py
--rw-r--r--   0        0        0     5924 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-cpu-kernels/test_cpuawkward_ListArrayU32_rpad_axis1_64.py
--rw-r--r--   0        0        0     2280 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-cpu-kernels/test_cpuawkward_ListArrayU32_validity.py
--rw-r--r--   0        0        0     5312 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-cpu-kernels/test_cpuawkward_ListArray_fill_to64_from32.py
--rw-r--r--   0        0        0     5312 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-cpu-kernels/test_cpuawkward_ListArray_fill_to64_from64.py
--rw-r--r--   0        0        0     5332 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-cpu-kernels/test_cpuawkward_ListArray_fill_to64_fromU32.py
--rw-r--r--   0        0        0     3625 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-cpu-kernels/test_cpuawkward_ListArray_getitem_jagged_carrylen_64.py
--rw-r--r--   0        0        0      419 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-cpu-kernels/test_cpuawkward_ListArray_getitem_jagged_numvalid_64.py
--rw-r--r--   0        0        0    27257 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-cpu-kernels/test_cpuawkward_ListArray_getitem_jagged_shrink_64.py
--rw-r--r--   0        0        0     3094 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-cpu-kernels/test_cpuawkward_ListOffsetArray32_compact_offsets_64.py
--rw-r--r--   0        0        0    19697 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-cpu-kernels/test_cpuawkward_ListOffsetArray32_flatten_offsets_64.py
--rw-r--r--   0        0        0      423 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-cpu-kernels/test_cpuawkward_ListOffsetArray32_rpad_and_clip_axis1_64.py
--rw-r--r--   0        0        0      414 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-cpu-kernels/test_cpuawkward_ListOffsetArray32_rpad_axis1_64.py
--rw-r--r--   0        0        0      418 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-cpu-kernels/test_cpuawkward_ListOffsetArray32_rpad_length_axis1.py
--rw-r--r--   0        0        0     2430 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-cpu-kernels/test_cpuawkward_ListOffsetArray32_toRegularArray.py
--rw-r--r--   0        0        0     3094 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-cpu-kernels/test_cpuawkward_ListOffsetArray64_compact_offsets_64.py
--rw-r--r--   0        0        0    19697 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-cpu-kernels/test_cpuawkward_ListOffsetArray64_flatten_offsets_64.py
--rw-r--r--   0        0        0      423 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-cpu-kernels/test_cpuawkward_ListOffsetArray64_rpad_and_clip_axis1_64.py
--rw-r--r--   0        0        0      414 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-cpu-kernels/test_cpuawkward_ListOffsetArray64_rpad_axis1_64.py
--rw-r--r--   0        0        0      418 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-cpu-kernels/test_cpuawkward_ListOffsetArray64_rpad_length_axis1.py
--rw-r--r--   0        0        0     2430 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-cpu-kernels/test_cpuawkward_ListOffsetArray64_toRegularArray.py
--rw-r--r--   0        0        0     3109 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-cpu-kernels/test_cpuawkward_ListOffsetArrayU32_compact_offsets_64.py
--rw-r--r--   0        0        0    19772 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-cpu-kernels/test_cpuawkward_ListOffsetArrayU32_flatten_offsets_64.py
--rw-r--r--   0        0        0      424 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-cpu-kernels/test_cpuawkward_ListOffsetArrayU32_rpad_and_clip_axis1_64.py
--rw-r--r--   0        0        0      415 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-cpu-kernels/test_cpuawkward_ListOffsetArrayU32_rpad_axis1_64.py
--rw-r--r--   0        0        0      419 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-cpu-kernels/test_cpuawkward_ListOffsetArrayU32_rpad_length_axis1.py
--rw-r--r--   0        0        0     2445 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-cpu-kernels/test_cpuawkward_ListOffsetArrayU32_toRegularArray.py
--rw-r--r--   0        0        0    19202 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-cpu-kernels/test_cpuawkward_ListOffsetArray_drop_none_indexes_32.py
--rw-r--r--   0        0        0    19202 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-cpu-kernels/test_cpuawkward_ListOffsetArray_drop_none_indexes_64.py
--rw-r--r--   0        0        0      426 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-cpu-kernels/test_cpuawkward_ListOffsetArray_reduce_local_nextparents_64.py
--rw-r--r--   0        0        0      425 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-cpu-kernels/test_cpuawkward_ListOffsetArray_reduce_local_outoffsets_64.py
--rw-r--r--   0        0        0      438 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-cpu-kernels/test_cpuawkward_ListOffsetArray_reduce_nonlocal_maxcount_offsetscopy_64.py
--rw-r--r--   0        0        0      428 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-cpu-kernels/test_cpuawkward_ListOffsetArray_reduce_nonlocal_nextshifts_64.py
--rw-r--r--   0        0        0      428 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-cpu-kernels/test_cpuawkward_ListOffsetArray_reduce_nonlocal_nextstarts_64.py
--rw-r--r--   0        0        0      432 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-cpu-kernels/test_cpuawkward_ListOffsetArray_reduce_nonlocal_outstartsstops_64.py
--rw-r--r--   0        0        0    25597 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-cpu-kernels/test_cpuawkward_MaskedArray32_getitem_next_jagged_project.py
--rw-r--r--   0        0        0    25597 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-cpu-kernels/test_cpuawkward_MaskedArray64_getitem_next_jagged_project.py
--rw-r--r--   0        0        0    25672 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-cpu-kernels/test_cpuawkward_MaskedArrayU32_getitem_next_jagged_project.py
--rw-r--r--   0        0        0      420 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-cpu-kernels/test_cpuawkward_NumpyArray_fill_tofloat32_fromfloat32.py
--rw-r--r--   0        0        0      420 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-cpu-kernels/test_cpuawkward_NumpyArray_fill_tofloat32_fromfloat64.py
--rw-r--r--   0        0        0      418 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-cpu-kernels/test_cpuawkward_NumpyArray_fill_tofloat32_fromint16.py
--rw-r--r--   0        0        0      418 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-cpu-kernels/test_cpuawkward_NumpyArray_fill_tofloat32_fromint32.py
--rw-r--r--   0        0        0      418 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-cpu-kernels/test_cpuawkward_NumpyArray_fill_tofloat32_fromint64.py
--rw-r--r--   0        0        0      417 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-cpu-kernels/test_cpuawkward_NumpyArray_fill_tofloat32_fromint8.py
--rw-r--r--   0        0        0      419 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-cpu-kernels/test_cpuawkward_NumpyArray_fill_tofloat32_fromuint16.py
--rw-r--r--   0        0        0      419 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-cpu-kernels/test_cpuawkward_NumpyArray_fill_tofloat32_fromuint32.py
--rw-r--r--   0        0        0      419 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-cpu-kernels/test_cpuawkward_NumpyArray_fill_tofloat32_fromuint64.py
--rw-r--r--   0        0        0      418 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-cpu-kernels/test_cpuawkward_NumpyArray_fill_tofloat32_fromuint8.py
--rw-r--r--   0        0        0      420 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-cpu-kernels/test_cpuawkward_NumpyArray_fill_tofloat64_fromfloat32.py
--rw-r--r--   0        0        0      420 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-cpu-kernels/test_cpuawkward_NumpyArray_fill_tofloat64_fromfloat64.py
--rw-r--r--   0        0        0      418 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-cpu-kernels/test_cpuawkward_NumpyArray_fill_tofloat64_fromint16.py
--rw-r--r--   0        0        0      418 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-cpu-kernels/test_cpuawkward_NumpyArray_fill_tofloat64_fromint32.py
--rw-r--r--   0        0        0      418 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-cpu-kernels/test_cpuawkward_NumpyArray_fill_tofloat64_fromint64.py
--rw-r--r--   0        0        0      417 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-cpu-kernels/test_cpuawkward_NumpyArray_fill_tofloat64_fromint8.py
--rw-r--r--   0        0        0      419 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-cpu-kernels/test_cpuawkward_NumpyArray_fill_tofloat64_fromuint16.py
--rw-r--r--   0        0        0      419 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-cpu-kernels/test_cpuawkward_NumpyArray_fill_tofloat64_fromuint32.py
--rw-r--r--   0        0        0      419 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-cpu-kernels/test_cpuawkward_NumpyArray_fill_tofloat64_fromuint64.py
--rw-r--r--   0        0        0      418 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-cpu-kernels/test_cpuawkward_NumpyArray_fill_tofloat64_fromuint8.py
--rw-r--r--   0        0        0      418 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-cpu-kernels/test_cpuawkward_NumpyArray_fill_toint16_fromfloat32.py
--rw-r--r--   0        0        0      418 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-cpu-kernels/test_cpuawkward_NumpyArray_fill_toint16_fromfloat64.py
--rw-r--r--   0        0        0      416 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-cpu-kernels/test_cpuawkward_NumpyArray_fill_toint16_fromint16.py
--rw-r--r--   0        0        0      416 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-cpu-kernels/test_cpuawkward_NumpyArray_fill_toint16_fromint32.py
--rw-r--r--   0        0        0      416 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-cpu-kernels/test_cpuawkward_NumpyArray_fill_toint16_fromint64.py
--rw-r--r--   0        0        0      415 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-cpu-kernels/test_cpuawkward_NumpyArray_fill_toint16_fromint8.py
--rw-r--r--   0        0        0      417 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-cpu-kernels/test_cpuawkward_NumpyArray_fill_toint16_fromuint16.py
--rw-r--r--   0        0        0      417 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-cpu-kernels/test_cpuawkward_NumpyArray_fill_toint16_fromuint32.py
--rw-r--r--   0        0        0      417 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-cpu-kernels/test_cpuawkward_NumpyArray_fill_toint16_fromuint64.py
--rw-r--r--   0        0        0      416 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-cpu-kernels/test_cpuawkward_NumpyArray_fill_toint16_fromuint8.py
--rw-r--r--   0        0        0      418 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-cpu-kernels/test_cpuawkward_NumpyArray_fill_toint32_fromfloat32.py
--rw-r--r--   0        0        0      418 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-cpu-kernels/test_cpuawkward_NumpyArray_fill_toint32_fromfloat64.py
--rw-r--r--   0        0        0      416 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-cpu-kernels/test_cpuawkward_NumpyArray_fill_toint32_fromint16.py
--rw-r--r--   0        0        0      416 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-cpu-kernels/test_cpuawkward_NumpyArray_fill_toint32_fromint32.py
--rw-r--r--   0        0        0      416 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-cpu-kernels/test_cpuawkward_NumpyArray_fill_toint32_fromint64.py
--rw-r--r--   0        0        0      415 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-cpu-kernels/test_cpuawkward_NumpyArray_fill_toint32_fromint8.py
--rw-r--r--   0        0        0      417 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-cpu-kernels/test_cpuawkward_NumpyArray_fill_toint32_fromuint16.py
--rw-r--r--   0        0        0      417 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-cpu-kernels/test_cpuawkward_NumpyArray_fill_toint32_fromuint32.py
--rw-r--r--   0        0        0      417 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-cpu-kernels/test_cpuawkward_NumpyArray_fill_toint32_fromuint64.py
--rw-r--r--   0        0        0      416 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-cpu-kernels/test_cpuawkward_NumpyArray_fill_toint32_fromuint8.py
--rw-r--r--   0        0        0      418 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-cpu-kernels/test_cpuawkward_NumpyArray_fill_toint64_fromfloat32.py
--rw-r--r--   0        0        0      418 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-cpu-kernels/test_cpuawkward_NumpyArray_fill_toint64_fromfloat64.py
--rw-r--r--   0        0        0      416 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-cpu-kernels/test_cpuawkward_NumpyArray_fill_toint64_fromint16.py
--rw-r--r--   0        0        0      416 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-cpu-kernels/test_cpuawkward_NumpyArray_fill_toint64_fromint32.py
--rw-r--r--   0        0        0      416 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-cpu-kernels/test_cpuawkward_NumpyArray_fill_toint64_fromint64.py
--rw-r--r--   0        0        0      415 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-cpu-kernels/test_cpuawkward_NumpyArray_fill_toint64_fromint8.py
--rw-r--r--   0        0        0      417 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-cpu-kernels/test_cpuawkward_NumpyArray_fill_toint64_fromuint16.py
--rw-r--r--   0        0        0      417 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-cpu-kernels/test_cpuawkward_NumpyArray_fill_toint64_fromuint32.py
--rw-r--r--   0        0        0      417 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-cpu-kernels/test_cpuawkward_NumpyArray_fill_toint64_fromuint64.py
--rw-r--r--   0        0        0      416 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-cpu-kernels/test_cpuawkward_NumpyArray_fill_toint64_fromuint8.py
--rw-r--r--   0        0        0      417 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-cpu-kernels/test_cpuawkward_NumpyArray_fill_toint8_fromfloat32.py
--rw-r--r--   0        0        0      417 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-cpu-kernels/test_cpuawkward_NumpyArray_fill_toint8_fromfloat64.py
--rw-r--r--   0        0        0      415 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-cpu-kernels/test_cpuawkward_NumpyArray_fill_toint8_fromint16.py
--rw-r--r--   0        0        0      415 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-cpu-kernels/test_cpuawkward_NumpyArray_fill_toint8_fromint32.py
--rw-r--r--   0        0        0      415 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-cpu-kernels/test_cpuawkward_NumpyArray_fill_toint8_fromint64.py
--rw-r--r--   0        0        0      414 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-cpu-kernels/test_cpuawkward_NumpyArray_fill_toint8_fromint8.py
--rw-r--r--   0        0        0      416 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-cpu-kernels/test_cpuawkward_NumpyArray_fill_toint8_fromuint16.py
--rw-r--r--   0        0        0      416 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-cpu-kernels/test_cpuawkward_NumpyArray_fill_toint8_fromuint32.py
--rw-r--r--   0        0        0      416 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-cpu-kernels/test_cpuawkward_NumpyArray_fill_toint8_fromuint64.py
--rw-r--r--   0        0        0      415 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-cpu-kernels/test_cpuawkward_NumpyArray_fill_toint8_fromuint8.py
--rw-r--r--   0        0        0      419 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-cpu-kernels/test_cpuawkward_NumpyArray_fill_touint16_fromfloat32.py
--rw-r--r--   0        0        0      419 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-cpu-kernels/test_cpuawkward_NumpyArray_fill_touint16_fromfloat64.py
--rw-r--r--   0        0        0      417 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-cpu-kernels/test_cpuawkward_NumpyArray_fill_touint16_fromint16.py
--rw-r--r--   0        0        0      417 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-cpu-kernels/test_cpuawkward_NumpyArray_fill_touint16_fromint32.py
--rw-r--r--   0        0        0      417 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-cpu-kernels/test_cpuawkward_NumpyArray_fill_touint16_fromint64.py
--rw-r--r--   0        0        0      416 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-cpu-kernels/test_cpuawkward_NumpyArray_fill_touint16_fromint8.py
--rw-r--r--   0        0        0      418 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-cpu-kernels/test_cpuawkward_NumpyArray_fill_touint16_fromuint16.py
--rw-r--r--   0        0        0      418 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-cpu-kernels/test_cpuawkward_NumpyArray_fill_touint16_fromuint32.py
--rw-r--r--   0        0        0      418 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-cpu-kernels/test_cpuawkward_NumpyArray_fill_touint16_fromuint64.py
--rw-r--r--   0        0        0      417 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-cpu-kernels/test_cpuawkward_NumpyArray_fill_touint16_fromuint8.py
--rw-r--r--   0        0        0      419 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-cpu-kernels/test_cpuawkward_NumpyArray_fill_touint32_fromfloat32.py
--rw-r--r--   0        0        0      419 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-cpu-kernels/test_cpuawkward_NumpyArray_fill_touint32_fromfloat64.py
--rw-r--r--   0        0        0      417 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-cpu-kernels/test_cpuawkward_NumpyArray_fill_touint32_fromint16.py
--rw-r--r--   0        0        0      417 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-cpu-kernels/test_cpuawkward_NumpyArray_fill_touint32_fromint32.py
--rw-r--r--   0        0        0      417 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-cpu-kernels/test_cpuawkward_NumpyArray_fill_touint32_fromint64.py
--rw-r--r--   0        0        0      416 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-cpu-kernels/test_cpuawkward_NumpyArray_fill_touint32_fromint8.py
--rw-r--r--   0        0        0      418 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-cpu-kernels/test_cpuawkward_NumpyArray_fill_touint32_fromuint16.py
--rw-r--r--   0        0        0      418 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-cpu-kernels/test_cpuawkward_NumpyArray_fill_touint32_fromuint32.py
--rw-r--r--   0        0        0      418 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-cpu-kernels/test_cpuawkward_NumpyArray_fill_touint32_fromuint64.py
--rw-r--r--   0        0        0      417 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-cpu-kernels/test_cpuawkward_NumpyArray_fill_touint32_fromuint8.py
--rw-r--r--   0        0        0      419 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-cpu-kernels/test_cpuawkward_NumpyArray_fill_touint64_fromfloat32.py
--rw-r--r--   0        0        0      419 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-cpu-kernels/test_cpuawkward_NumpyArray_fill_touint64_fromfloat64.py
--rw-r--r--   0        0        0      417 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-cpu-kernels/test_cpuawkward_NumpyArray_fill_touint64_fromint16.py
--rw-r--r--   0        0        0      417 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-cpu-kernels/test_cpuawkward_NumpyArray_fill_touint64_fromint32.py
--rw-r--r--   0        0        0      417 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-cpu-kernels/test_cpuawkward_NumpyArray_fill_touint64_fromint64.py
--rw-r--r--   0        0        0      416 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-cpu-kernels/test_cpuawkward_NumpyArray_fill_touint64_fromint8.py
--rw-r--r--   0        0        0      418 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-cpu-kernels/test_cpuawkward_NumpyArray_fill_touint64_fromuint16.py
--rw-r--r--   0        0        0      418 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-cpu-kernels/test_cpuawkward_NumpyArray_fill_touint64_fromuint32.py
--rw-r--r--   0        0        0      418 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-cpu-kernels/test_cpuawkward_NumpyArray_fill_touint64_fromuint64.py
--rw-r--r--   0        0        0      417 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-cpu-kernels/test_cpuawkward_NumpyArray_fill_touint64_fromuint8.py
--rw-r--r--   0        0        0      418 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-cpu-kernels/test_cpuawkward_NumpyArray_fill_touint8_fromfloat32.py
--rw-r--r--   0        0        0      418 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-cpu-kernels/test_cpuawkward_NumpyArray_fill_touint8_fromfloat64.py
--rw-r--r--   0        0        0      416 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-cpu-kernels/test_cpuawkward_NumpyArray_fill_touint8_fromint16.py
--rw-r--r--   0        0        0      416 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-cpu-kernels/test_cpuawkward_NumpyArray_fill_touint8_fromint32.py
--rw-r--r--   0        0        0      416 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-cpu-kernels/test_cpuawkward_NumpyArray_fill_touint8_fromint64.py
--rw-r--r--   0        0        0      415 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-cpu-kernels/test_cpuawkward_NumpyArray_fill_touint8_fromint8.py
--rw-r--r--   0        0        0      417 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-cpu-kernels/test_cpuawkward_NumpyArray_fill_touint8_fromuint16.py
--rw-r--r--   0        0        0      417 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-cpu-kernels/test_cpuawkward_NumpyArray_fill_touint8_fromuint32.py
--rw-r--r--   0        0        0      417 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-cpu-kernels/test_cpuawkward_NumpyArray_fill_touint8_fromuint64.py
--rw-r--r--   0        0        0      416 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-cpu-kernels/test_cpuawkward_NumpyArray_fill_touint8_fromuint8.py
--rw-r--r--   0        0        0      429 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-cpu-kernels/test_cpuawkward_NumpyArray_rearrange_shifted_toint64_fromint64.py
--rw-r--r--   0        0        0      417 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-cpu-kernels/test_cpuawkward_NumpyArray_reduce_adjust_starts_64.py
--rw-r--r--   0        0        0      424 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-cpu-kernels/test_cpuawkward_NumpyArray_reduce_adjust_starts_shifts_64.py
--rw-r--r--   0        0        0      424 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-cpu-kernels/test_cpuawkward_NumpyArray_reduce_mask_ByteMaskedArray_64.py
--rw-r--r--   0        0        0     9133 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-cpu-kernels/test_cpuawkward_RegularArray_broadcast_tooffsets_64.py
--rw-r--r--   0        0        0      774 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-cpu-kernels/test_cpuawkward_RegularArray_broadcast_tooffsets_size1_64.py
--rw-r--r--   0        0        0     2411 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-cpu-kernels/test_cpuawkward_RegularArray_compact_offsets64.py
--rw-r--r--   0        0        0    11667 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-cpu-kernels/test_cpuawkward_RegularArray_getitem_carry_64.py
--rw-r--r--   0        0        0    18563 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-cpu-kernels/test_cpuawkward_RegularArray_getitem_jagged_expand_64.py
--rw-r--r--   0        0        0    22777 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-cpu-kernels/test_cpuawkward_RegularArray_getitem_next_array_64.py
--rw-r--r--   0        0        0   121809 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-cpu-kernels/test_cpuawkward_RegularArray_getitem_next_array_advanced_64.py
--rw-r--r--   0        0        0    12464 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-cpu-kernels/test_cpuawkward_RegularArray_getitem_next_array_regularize_64.py
--rw-r--r--   0        0        0     1936 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-cpu-kernels/test_cpuawkward_RegularArray_getitem_next_at_64.py
--rw-r--r--   0        0        0      771 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-cpu-kernels/test_cpuawkward_RegularArray_getitem_next_range_64.py
--rw-r--r--   0        0        0    13383 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-cpu-kernels/test_cpuawkward_RegularArray_getitem_next_range_spreadadvanced_64.py
--rw-r--r--   0        0        0     1932 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-cpu-kernels/test_cpuawkward_RegularArray_localindex_64.py
--rw-r--r--   0        0        0      423 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-cpu-kernels/test_cpuawkward_RegularArray_reduce_local_nextparents_64.py
--rw-r--r--   0        0        0      426 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-cpu-kernels/test_cpuawkward_RegularArray_reduce_nonlocal_preparenext_64.py
--rw-r--r--   0        0        0      710 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-cpu-kernels/test_cpuawkward_RegularArray_rpad_and_clip_axis1_64.py
--rw-r--r--   0        0        0      414 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-cpu-kernels/test_cpuawkward_UnionArray32_flatten_combine_64.py
--rw-r--r--   0        0        0      413 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-cpu-kernels/test_cpuawkward_UnionArray32_flatten_length_64.py
--rw-r--r--   0        0        0      414 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-cpu-kernels/test_cpuawkward_UnionArray64_flatten_combine_64.py
--rw-r--r--   0        0        0      413 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-cpu-kernels/test_cpuawkward_UnionArray64_flatten_length_64.py
--rw-r--r--   0        0        0      422 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-cpu-kernels/test_cpuawkward_UnionArray8_32_nestedfill_tags_index_64.py
--rw-r--r--   0        0        0    12717 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-cpu-kernels/test_cpuawkward_UnionArray8_32_project_64.py
--rw-r--r--   0        0        0     3937 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-cpu-kernels/test_cpuawkward_UnionArray8_32_regular_index.py
--rw-r--r--   0        0        0   627958 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-cpu-kernels/test_cpuawkward_UnionArray8_32_simplify8_32_to8_64.py
--rw-r--r--   0        0        0   627958 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-cpu-kernels/test_cpuawkward_UnionArray8_32_simplify8_64_to8_64.py
--rw-r--r--   0        0        0   629458 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-cpu-kernels/test_cpuawkward_UnionArray8_32_simplify8_U32_to8_64.py
--rw-r--r--   0        0        0    14172 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-cpu-kernels/test_cpuawkward_UnionArray8_32_simplify_one_to8_64.py
--rw-r--r--   0        0        0    70417 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-cpu-kernels/test_cpuawkward_UnionArray8_32_validity.py
--rw-r--r--   0        0        0      422 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-cpu-kernels/test_cpuawkward_UnionArray8_64_nestedfill_tags_index_64.py
--rw-r--r--   0        0        0    12717 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-cpu-kernels/test_cpuawkward_UnionArray8_64_project_64.py
--rw-r--r--   0        0        0     3937 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-cpu-kernels/test_cpuawkward_UnionArray8_64_regular_index.py
--rw-r--r--   0        0        0   627958 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-cpu-kernels/test_cpuawkward_UnionArray8_64_simplify8_32_to8_64.py
--rw-r--r--   0        0        0   627958 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-cpu-kernels/test_cpuawkward_UnionArray8_64_simplify8_64_to8_64.py
--rw-r--r--   0        0        0   629458 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-cpu-kernels/test_cpuawkward_UnionArray8_64_simplify8_U32_to8_64.py
--rw-r--r--   0        0        0    14172 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-cpu-kernels/test_cpuawkward_UnionArray8_64_simplify_one_to8_64.py
--rw-r--r--   0        0        0    70417 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-cpu-kernels/test_cpuawkward_UnionArray8_64_validity.py
--rw-r--r--   0        0        0      423 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-cpu-kernels/test_cpuawkward_UnionArray8_U32_nestedfill_tags_index_64.py
--rw-r--r--   0        0        0    12762 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-cpu-kernels/test_cpuawkward_UnionArray8_U32_project_64.py
--rw-r--r--   0        0        0     3957 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-cpu-kernels/test_cpuawkward_UnionArray8_U32_regular_index.py
--rw-r--r--   0        0        0   629458 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-cpu-kernels/test_cpuawkward_UnionArray8_U32_simplify8_32_to8_64.py
--rw-r--r--   0        0        0   629458 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-cpu-kernels/test_cpuawkward_UnionArray8_U32_simplify8_64_to8_64.py
--rw-r--r--   0        0        0   630958 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-cpu-kernels/test_cpuawkward_UnionArray8_U32_simplify8_U32_to8_64.py
--rw-r--r--   0        0        0    14217 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-cpu-kernels/test_cpuawkward_UnionArray8_U32_simplify_one_to8_64.py
--rw-r--r--   0        0        0    70792 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-cpu-kernels/test_cpuawkward_UnionArray8_U32_validity.py
--rw-r--r--   0        0        0     2687 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-cpu-kernels/test_cpuawkward_UnionArray8_regular_index_getsize.py
--rw-r--r--   0        0        0      415 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-cpu-kernels/test_cpuawkward_UnionArrayU32_flatten_combine_64.py
--rw-r--r--   0        0        0      414 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-cpu-kernels/test_cpuawkward_UnionArrayU32_flatten_length_64.py
--rw-r--r--   0        0        0      685 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-cpu-kernels/test_cpuawkward_UnionArray_fillindex_to64_count.py
--rw-r--r--   0        0        0     3206 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-cpu-kernels/test_cpuawkward_UnionArray_fillindex_to64_from32.py
--rw-r--r--   0        0        0     3206 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-cpu-kernels/test_cpuawkward_UnionArray_fillindex_to64_from64.py
--rw-r--r--   0        0        0     3221 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-cpu-kernels/test_cpuawkward_UnionArray_fillindex_to64_fromU32.py
--rw-r--r--   0        0        0     2811 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-cpu-kernels/test_cpuawkward_UnionArray_fillna_from32_to64.py
--rw-r--r--   0        0        0     2811 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-cpu-kernels/test_cpuawkward_UnionArray_fillna_from64_to64.py
--rw-r--r--   0        0        0     2826 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-cpu-kernels/test_cpuawkward_UnionArray_fillna_fromU32_to64.py
--rw-r--r--   0        0        0      688 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-cpu-kernels/test_cpuawkward_UnionArray_filltags_to8_const.py
--rw-r--r--   0        0        0     3262 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-cpu-kernels/test_cpuawkward_UnionArray_filltags_to8_from8.py
--rw-r--r--   0        0        0      629 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-cpu-kernels/test_cpuawkward_index_rpad_and_clip_axis0_64.py
--rw-r--r--   0        0        0      836 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-cpu-kernels/test_cpuawkward_index_rpad_and_clip_axis1_64.py
--rw-r--r--   0        0        0      576 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-cpu-kernels/test_cpuawkward_localindex_64.py
--rw-r--r--   0        0        0    15433 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-cpu-kernels/test_cpuawkward_missing_repeat_64.py
--rw-r--r--   0        0        0      407 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-cpu-kernels/test_cpuawkward_reduce_argmax_float32_64.py
--rw-r--r--   0        0        0      407 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-cpu-kernels/test_cpuawkward_reduce_argmax_float64_64.py
--rw-r--r--   0        0        0      405 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-cpu-kernels/test_cpuawkward_reduce_argmax_int16_64.py
--rw-r--r--   0        0        0      405 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-cpu-kernels/test_cpuawkward_reduce_argmax_int32_64.py
--rw-r--r--   0        0        0      405 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-cpu-kernels/test_cpuawkward_reduce_argmax_int64_64.py
--rw-r--r--   0        0        0      404 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-cpu-kernels/test_cpuawkward_reduce_argmax_int8_64.py
--rw-r--r--   0        0        0      406 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-cpu-kernels/test_cpuawkward_reduce_argmax_uint16_64.py
--rw-r--r--   0        0        0      406 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-cpu-kernels/test_cpuawkward_reduce_argmax_uint32_64.py
--rw-r--r--   0        0        0      406 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-cpu-kernels/test_cpuawkward_reduce_argmax_uint64_64.py
--rw-r--r--   0        0        0      405 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-cpu-kernels/test_cpuawkward_reduce_argmax_uint8_64.py
--rw-r--r--   0        0        0      407 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-cpu-kernels/test_cpuawkward_reduce_argmin_float32_64.py
--rw-r--r--   0        0        0      407 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-cpu-kernels/test_cpuawkward_reduce_argmin_float64_64.py
--rw-r--r--   0        0        0      405 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-cpu-kernels/test_cpuawkward_reduce_argmin_int16_64.py
--rw-r--r--   0        0        0      405 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-cpu-kernels/test_cpuawkward_reduce_argmin_int32_64.py
--rw-r--r--   0        0        0      405 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-cpu-kernels/test_cpuawkward_reduce_argmin_int64_64.py
--rw-r--r--   0        0        0      404 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-cpu-kernels/test_cpuawkward_reduce_argmin_int8_64.py
--rw-r--r--   0        0        0      406 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-cpu-kernels/test_cpuawkward_reduce_argmin_uint16_64.py
--rw-r--r--   0        0        0      406 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-cpu-kernels/test_cpuawkward_reduce_argmin_uint32_64.py
--rw-r--r--   0        0        0      406 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-cpu-kernels/test_cpuawkward_reduce_argmin_uint64_64.py
--rw-r--r--   0        0        0      405 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-cpu-kernels/test_cpuawkward_reduce_argmin_uint8_64.py
--rw-r--r--   0        0        0      398 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-cpu-kernels/test_cpuawkward_reduce_count_64.py
--rw-r--r--   0        0        0      410 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-cpu-kernels/test_cpuawkward_reduce_countnonzero_bool_64.py
--rw-r--r--   0        0        0      413 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-cpu-kernels/test_cpuawkward_reduce_countnonzero_float32_64.py
--rw-r--r--   0        0        0      413 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-cpu-kernels/test_cpuawkward_reduce_countnonzero_float64_64.py
--rw-r--r--   0        0        0      411 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-cpu-kernels/test_cpuawkward_reduce_countnonzero_int16_64.py
--rw-r--r--   0        0        0      411 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-cpu-kernels/test_cpuawkward_reduce_countnonzero_int32_64.py
--rw-r--r--   0        0        0      411 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-cpu-kernels/test_cpuawkward_reduce_countnonzero_int64_64.py
--rw-r--r--   0        0        0      410 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-cpu-kernels/test_cpuawkward_reduce_countnonzero_int8_64.py
--rw-r--r--   0        0        0      412 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-cpu-kernels/test_cpuawkward_reduce_countnonzero_uint16_64.py
--rw-r--r--   0        0        0      412 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-cpu-kernels/test_cpuawkward_reduce_countnonzero_uint32_64.py
--rw-r--r--   0        0        0      412 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-cpu-kernels/test_cpuawkward_reduce_countnonzero_uint64_64.py
--rw-r--r--   0        0        0      411 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-cpu-kernels/test_cpuawkward_reduce_countnonzero_uint8_64.py
--rw-r--r--   0        0        0      412 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-cpu-kernels/test_cpuawkward_reduce_max_float32_float32_64.py
--rw-r--r--   0        0        0      412 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-cpu-kernels/test_cpuawkward_reduce_max_float64_float64_64.py
--rw-r--r--   0        0        0      408 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-cpu-kernels/test_cpuawkward_reduce_max_int16_int16_64.py
--rw-r--r--   0        0        0      408 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-cpu-kernels/test_cpuawkward_reduce_max_int32_int32_64.py
--rw-r--r--   0        0        0      408 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-cpu-kernels/test_cpuawkward_reduce_max_int64_int64_64.py
--rw-r--r--   0        0        0      406 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-cpu-kernels/test_cpuawkward_reduce_max_int8_int8_64.py
--rw-r--r--   0        0        0      410 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-cpu-kernels/test_cpuawkward_reduce_max_uint16_uint16_64.py
--rw-r--r--   0        0        0      410 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-cpu-kernels/test_cpuawkward_reduce_max_uint32_uint32_64.py
--rw-r--r--   0        0        0      410 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-cpu-kernels/test_cpuawkward_reduce_max_uint64_uint64_64.py
--rw-r--r--   0        0        0      408 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-cpu-kernels/test_cpuawkward_reduce_max_uint8_uint8_64.py
--rw-r--r--   0        0        0      412 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-cpu-kernels/test_cpuawkward_reduce_min_float32_float32_64.py
--rw-r--r--   0        0        0      412 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-cpu-kernels/test_cpuawkward_reduce_min_float64_float64_64.py
--rw-r--r--   0        0        0      408 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-cpu-kernels/test_cpuawkward_reduce_min_int16_int16_64.py
--rw-r--r--   0        0        0      408 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-cpu-kernels/test_cpuawkward_reduce_min_int32_int32_64.py
--rw-r--r--   0        0        0      408 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-cpu-kernels/test_cpuawkward_reduce_min_int64_int64_64.py
--rw-r--r--   0        0        0      406 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-cpu-kernels/test_cpuawkward_reduce_min_int8_int8_64.py
--rw-r--r--   0        0        0      410 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-cpu-kernels/test_cpuawkward_reduce_min_uint16_uint16_64.py
--rw-r--r--   0        0        0      410 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-cpu-kernels/test_cpuawkward_reduce_min_uint32_uint32_64.py
--rw-r--r--   0        0        0      410 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-cpu-kernels/test_cpuawkward_reduce_min_uint64_uint64_64.py
--rw-r--r--   0        0        0      408 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-cpu-kernels/test_cpuawkward_reduce_min_uint8_uint8_64.py
--rw-r--r--   0        0        0      407 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-cpu-kernels/test_cpuawkward_reduce_prod_bool_bool_64.py
--rw-r--r--   0        0        0      410 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-cpu-kernels/test_cpuawkward_reduce_prod_bool_float32_64.py
--rw-r--r--   0        0        0      410 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-cpu-kernels/test_cpuawkward_reduce_prod_bool_float64_64.py
--rw-r--r--   0        0        0      408 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-cpu-kernels/test_cpuawkward_reduce_prod_bool_int16_64.py
--rw-r--r--   0        0        0      408 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-cpu-kernels/test_cpuawkward_reduce_prod_bool_int32_64.py
--rw-r--r--   0        0        0      408 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-cpu-kernels/test_cpuawkward_reduce_prod_bool_int64_64.py
--rw-r--r--   0        0        0      407 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-cpu-kernels/test_cpuawkward_reduce_prod_bool_int8_64.py
--rw-r--r--   0        0        0      409 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-cpu-kernels/test_cpuawkward_reduce_prod_bool_uint16_64.py
--rw-r--r--   0        0        0      409 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-cpu-kernels/test_cpuawkward_reduce_prod_bool_uint32_64.py
--rw-r--r--   0        0        0      409 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-cpu-kernels/test_cpuawkward_reduce_prod_bool_uint64_64.py
--rw-r--r--   0        0        0      408 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-cpu-kernels/test_cpuawkward_reduce_prod_bool_uint8_64.py
--rw-r--r--   0        0        0      413 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-cpu-kernels/test_cpuawkward_reduce_prod_float32_float32_64.py
--rw-r--r--   0        0        0      413 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-cpu-kernels/test_cpuawkward_reduce_prod_float64_float64_64.py
--rw-r--r--   0        0        0      409 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-cpu-kernels/test_cpuawkward_reduce_prod_int32_int16_64.py
--rw-r--r--   0        0        0      409 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-cpu-kernels/test_cpuawkward_reduce_prod_int32_int32_64.py
--rw-r--r--   0        0        0      408 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-cpu-kernels/test_cpuawkward_reduce_prod_int32_int8_64.py
--rw-r--r--   0        0        0      409 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-cpu-kernels/test_cpuawkward_reduce_prod_int64_int16_64.py
--rw-r--r--   0        0        0      409 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-cpu-kernels/test_cpuawkward_reduce_prod_int64_int32_64.py
--rw-r--r--   0        0        0      409 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-cpu-kernels/test_cpuawkward_reduce_prod_int64_int64_64.py
--rw-r--r--   0        0        0      408 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-cpu-kernels/test_cpuawkward_reduce_prod_int64_int8_64.py
--rw-r--r--   0        0        0      411 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-cpu-kernels/test_cpuawkward_reduce_prod_uint32_uint16_64.py
--rw-r--r--   0        0        0      411 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-cpu-kernels/test_cpuawkward_reduce_prod_uint32_uint32_64.py
--rw-r--r--   0        0        0      410 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-cpu-kernels/test_cpuawkward_reduce_prod_uint32_uint8_64.py
--rw-r--r--   0        0        0      411 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-cpu-kernels/test_cpuawkward_reduce_prod_uint64_uint16_64.py
--rw-r--r--   0        0        0      411 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-cpu-kernels/test_cpuawkward_reduce_prod_uint64_uint32_64.py
--rw-r--r--   0        0        0      411 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-cpu-kernels/test_cpuawkward_reduce_prod_uint64_uint64_64.py
--rw-r--r--   0        0        0      410 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-cpu-kernels/test_cpuawkward_reduce_prod_uint64_uint8_64.py
--rw-r--r--   0        0        0      406 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-cpu-kernels/test_cpuawkward_reduce_sum_bool_bool_64.py
--rw-r--r--   0        0        0      409 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-cpu-kernels/test_cpuawkward_reduce_sum_bool_float32_64.py
--rw-r--r--   0        0        0      409 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-cpu-kernels/test_cpuawkward_reduce_sum_bool_float64_64.py
--rw-r--r--   0        0        0      407 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-cpu-kernels/test_cpuawkward_reduce_sum_bool_int16_64.py
--rw-r--r--   0        0        0      407 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-cpu-kernels/test_cpuawkward_reduce_sum_bool_int32_64.py
--rw-r--r--   0        0        0      407 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-cpu-kernels/test_cpuawkward_reduce_sum_bool_int64_64.py
--rw-r--r--   0        0        0      406 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-cpu-kernels/test_cpuawkward_reduce_sum_bool_int8_64.py
--rw-r--r--   0        0        0      408 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-cpu-kernels/test_cpuawkward_reduce_sum_bool_uint16_64.py
--rw-r--r--   0        0        0      408 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-cpu-kernels/test_cpuawkward_reduce_sum_bool_uint32_64.py
--rw-r--r--   0        0        0      408 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-cpu-kernels/test_cpuawkward_reduce_sum_bool_uint64_64.py
--rw-r--r--   0        0        0      407 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-cpu-kernels/test_cpuawkward_reduce_sum_bool_uint8_64.py
--rw-r--r--   0        0        0      412 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-cpu-kernels/test_cpuawkward_reduce_sum_float32_float32_64.py
--rw-r--r--   0        0        0      412 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-cpu-kernels/test_cpuawkward_reduce_sum_float64_float64_64.py
--rw-r--r--   0        0        0      407 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-cpu-kernels/test_cpuawkward_reduce_sum_int32_bool_64.py
--rw-r--r--   0        0        0      408 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-cpu-kernels/test_cpuawkward_reduce_sum_int32_int16_64.py
--rw-r--r--   0        0        0      408 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-cpu-kernels/test_cpuawkward_reduce_sum_int32_int32_64.py
--rw-r--r--   0        0        0      407 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-cpu-kernels/test_cpuawkward_reduce_sum_int32_int8_64.py
--rw-r--r--   0        0        0      407 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-cpu-kernels/test_cpuawkward_reduce_sum_int64_bool_64.py
--rw-r--r--   0        0        0      408 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-cpu-kernels/test_cpuawkward_reduce_sum_int64_int16_64.py
--rw-r--r--   0        0        0      408 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-cpu-kernels/test_cpuawkward_reduce_sum_int64_int32_64.py
--rw-r--r--   0        0        0      408 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-cpu-kernels/test_cpuawkward_reduce_sum_int64_int64_64.py
--rw-r--r--   0        0        0      407 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-cpu-kernels/test_cpuawkward_reduce_sum_int64_int8_64.py
--rw-r--r--   0        0        0      410 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-cpu-kernels/test_cpuawkward_reduce_sum_uint32_uint16_64.py
--rw-r--r--   0        0        0      410 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-cpu-kernels/test_cpuawkward_reduce_sum_uint32_uint32_64.py
--rw-r--r--   0        0        0      409 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-cpu-kernels/test_cpuawkward_reduce_sum_uint32_uint8_64.py
--rw-r--r--   0        0        0      410 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-cpu-kernels/test_cpuawkward_reduce_sum_uint64_uint16_64.py
--rw-r--r--   0        0        0      410 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-cpu-kernels/test_cpuawkward_reduce_sum_uint64_uint32_64.py
--rw-r--r--   0        0        0      410 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-cpu-kernels/test_cpuawkward_reduce_sum_uint64_uint64_64.py
--rw-r--r--   0        0        0      409 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-cpu-kernels/test_cpuawkward_reduce_sum_uint64_uint8_64.py
--rw-r--r--   0        0        0      146 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-spec/__init__.py
--rw-r--r--   0        0        0    78888 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-spec/kernels.py
--rw-r--r--   0        0        0     4076 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-spec/test_pyawkward_BitMaskedArray_to_ByteMaskedArray.py
--rw-r--r--   0        0        0     3707 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-spec/test_pyawkward_BitMaskedArray_to_IndexedOptionArray64.py
--rw-r--r--   0        0        0     1901 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-spec/test_pyawkward_ByteMaskedArray_getitem_nextcarry_64.py
--rw-r--r--   0        0        0     2633 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-spec/test_pyawkward_ByteMaskedArray_getitem_nextcarry_outindex_64.py
--rw-r--r--   0        0        0     2122 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-spec/test_pyawkward_ByteMaskedArray_numnull.py
--rw-r--r--   0        0        0    12372 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-spec/test_pyawkward_ByteMaskedArray_overlay_mask8.py
--rw-r--r--   0        0        0      372 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-spec/test_pyawkward_ByteMaskedArray_reduce_next_64.py
--rw-r--r--   0        0        0      392 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-spec/test_pyawkward_ByteMaskedArray_reduce_next_nonlocal_nextshifts_64.py
--rw-r--r--   0        0        0      403 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-spec/test_pyawkward_ByteMaskedArray_reduce_next_nonlocal_nextshifts_fromshifts_64.py
--rw-r--r--   0        0        0     2355 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-spec/test_pyawkward_ByteMaskedArray_toIndexedOptionArray64.py
--rw-r--r--   0        0        0    21962 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-spec/test_pyawkward_Content_getitem_next_missing_jagged_getmaskstartstop.py
--rw-r--r--   0        0        0      362 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-spec/test_pyawkward_Index32_iscontiguous.py
--rw-r--r--   0        0        0      362 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-spec/test_pyawkward_Index64_iscontiguous.py
--rw-r--r--   0        0        0      361 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-spec/test_pyawkward_Index8_iscontiguous.py
--rw-r--r--   0        0        0      363 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-spec/test_pyawkward_IndexU32_iscontiguous.py
--rw-r--r--   0        0        0      362 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-spec/test_pyawkward_IndexU8_iscontiguous.py
--rw-r--r--   0        0        0      365 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-spec/test_pyawkward_Index_nones_as_index_64.py
--rw-r--r--   0        0        0     2304 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-spec/test_pyawkward_IndexedArray32_flatten_nextcarry_64.py
--rw-r--r--   0        0        0    13526 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-spec/test_pyawkward_IndexedArray32_flatten_none2empty_64.py
--rw-r--r--   0        0        0     2304 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-spec/test_pyawkward_IndexedArray32_getitem_nextcarry_64.py
--rw-r--r--   0        0        0     1893 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-spec/test_pyawkward_IndexedArray32_getitem_nextcarry_outindex_64.py
--rw-r--r--   0        0        0      371 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-spec/test_pyawkward_IndexedArray32_index_of_nulls.py
--rw-r--r--   0        0        0     2036 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-spec/test_pyawkward_IndexedArray32_numnull.py
--rw-r--r--   0        0        0      372 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-spec/test_pyawkward_IndexedArray32_numnull_parents.py
--rw-r--r--   0        0        0      375 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-spec/test_pyawkward_IndexedArray32_overlay_mask8_to64.py
--rw-r--r--   0        0        0      377 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-spec/test_pyawkward_IndexedArray32_ranges_carry_next_64.py
--rw-r--r--   0        0        0      371 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-spec/test_pyawkward_IndexedArray32_ranges_next_64.py
--rw-r--r--   0        0        0      371 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-spec/test_pyawkward_IndexedArray32_reduce_next_64.py
--rw-r--r--   0        0        0      391 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-spec/test_pyawkward_IndexedArray32_reduce_next_nonlocal_nextshifts_64.py
--rw-r--r--   0        0        0      402 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-spec/test_pyawkward_IndexedArray32_reduce_next_nonlocal_nextshifts_fromshifts_64.py
--rw-r--r--   0        0        0     8007 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-spec/test_pyawkward_IndexedArray32_simplify32_to64.py
--rw-r--r--   0        0        0     8007 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-spec/test_pyawkward_IndexedArray32_simplify64_to64.py
--rw-r--r--   0        0        0     8037 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-spec/test_pyawkward_IndexedArray32_simplifyU32_to64.py
--rw-r--r--   0        0        0     8307 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-spec/test_pyawkward_IndexedArray32_validity.py
--rw-r--r--   0        0        0     2304 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-spec/test_pyawkward_IndexedArray64_flatten_nextcarry_64.py
--rw-r--r--   0        0        0    13526 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-spec/test_pyawkward_IndexedArray64_flatten_none2empty_64.py
--rw-r--r--   0        0        0     2304 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-spec/test_pyawkward_IndexedArray64_getitem_nextcarry_64.py
--rw-r--r--   0        0        0     1893 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-spec/test_pyawkward_IndexedArray64_getitem_nextcarry_outindex_64.py
--rw-r--r--   0        0        0      371 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-spec/test_pyawkward_IndexedArray64_index_of_nulls.py
--rw-r--r--   0        0        0     2036 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-spec/test_pyawkward_IndexedArray64_numnull.py
--rw-r--r--   0        0        0      372 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-spec/test_pyawkward_IndexedArray64_numnull_parents.py
--rw-r--r--   0        0        0      375 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-spec/test_pyawkward_IndexedArray64_overlay_mask8_to64.py
--rw-r--r--   0        0        0      377 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-spec/test_pyawkward_IndexedArray64_ranges_carry_next_64.py
--rw-r--r--   0        0        0      371 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-spec/test_pyawkward_IndexedArray64_ranges_next_64.py
--rw-r--r--   0        0        0      371 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-spec/test_pyawkward_IndexedArray64_reduce_next_64.py
--rw-r--r--   0        0        0      391 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-spec/test_pyawkward_IndexedArray64_reduce_next_nonlocal_nextshifts_64.py
--rw-r--r--   0        0        0      402 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-spec/test_pyawkward_IndexedArray64_reduce_next_nonlocal_nextshifts_fromshifts_64.py
--rw-r--r--   0        0        0     8007 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-spec/test_pyawkward_IndexedArray64_simplify32_to64.py
--rw-r--r--   0        0        0     8007 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-spec/test_pyawkward_IndexedArray64_simplify64_to64.py
--rw-r--r--   0        0        0     8037 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-spec/test_pyawkward_IndexedArray64_simplifyU32_to64.py
--rw-r--r--   0        0        0     8307 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-spec/test_pyawkward_IndexedArray64_validity.py
--rw-r--r--   0        0        0     2314 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-spec/test_pyawkward_IndexedArrayU32_flatten_nextcarry_64.py
--rw-r--r--   0        0        0    13576 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-spec/test_pyawkward_IndexedArrayU32_flatten_none2empty_64.py
--rw-r--r--   0        0        0     2314 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-spec/test_pyawkward_IndexedArrayU32_getitem_nextcarry_64.py
--rw-r--r--   0        0        0     1899 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-spec/test_pyawkward_IndexedArrayU32_getitem_nextcarry_outindex_64.py
--rw-r--r--   0        0        0      372 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-spec/test_pyawkward_IndexedArrayU32_index_of_nulls.py
--rw-r--r--   0        0        0     2046 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-spec/test_pyawkward_IndexedArrayU32_numnull.py
--rw-r--r--   0        0        0      373 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-spec/test_pyawkward_IndexedArrayU32_numnull_parents.py
--rw-r--r--   0        0        0      376 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-spec/test_pyawkward_IndexedArrayU32_overlay_mask8_to64.py
--rw-r--r--   0        0        0      378 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-spec/test_pyawkward_IndexedArrayU32_ranges_carry_next_64.py
--rw-r--r--   0        0        0      372 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-spec/test_pyawkward_IndexedArrayU32_ranges_next_64.py
--rw-r--r--   0        0        0      372 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-spec/test_pyawkward_IndexedArrayU32_reduce_next_64.py
--rw-r--r--   0        0        0      392 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-spec/test_pyawkward_IndexedArrayU32_reduce_next_nonlocal_nextshifts_64.py
--rw-r--r--   0        0        0      403 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-spec/test_pyawkward_IndexedArrayU32_reduce_next_nonlocal_nextshifts_fromshifts_64.py
--rw-r--r--   0        0        0     8037 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-spec/test_pyawkward_IndexedArrayU32_simplify32_to64.py
--rw-r--r--   0        0        0     8037 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-spec/test_pyawkward_IndexedArrayU32_simplify64_to64.py
--rw-r--r--   0        0        0     8067 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-spec/test_pyawkward_IndexedArrayU32_simplifyU32_to64.py
--rw-r--r--   0        0        0     8357 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-spec/test_pyawkward_IndexedArrayU32_validity.py
--rw-r--r--   0        0        0     2146 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-spec/test_pyawkward_IndexedArray_fill_to64_count.py
--rw-r--r--   0        0        0     2711 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-spec/test_pyawkward_IndexedArray_fill_to64_from32.py
--rw-r--r--   0        0        0     2711 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-spec/test_pyawkward_IndexedArray_fill_to64_from64.py
--rw-r--r--   0        0        0     2721 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-spec/test_pyawkward_IndexedArray_fill_to64_fromU32.py
--rw-r--r--   0        0        0      372 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-spec/test_pyawkward_IndexedArray_numnull_unique_64.py
--rw-r--r--   0        0        0      381 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-spec/test_pyawkward_IndexedArray_reduce_next_fix_offsets_64.py
--rw-r--r--   0        0        0      387 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-spec/test_pyawkward_IndexedArray_unique_next_index_and_offsets_64.py
--rw-r--r--   0        0        0     2290 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-spec/test_pyawkward_IndexedOptionArray_rpad_and_clip_mask_axis1_64.py
--rw-r--r--   0        0        0     1263 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-spec/test_pyawkward_ListArray32_broadcast_tooffsets_64.py
--rw-r--r--   0        0        0    17509 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-spec/test_pyawkward_ListArray32_combinations_length_64.py
--rw-r--r--   0        0        0     2676 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-spec/test_pyawkward_ListArray32_compact_offsets_64.py
--rw-r--r--   0        0        0    10002 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-spec/test_pyawkward_ListArray32_getitem_jagged_apply_64.py
--rw-r--r--   0        0        0    15834 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-spec/test_pyawkward_ListArray32_getitem_jagged_descend_64.py
--rw-r--r--   0        0        0     4925 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-spec/test_pyawkward_ListArray32_getitem_jagged_expand_64.py
--rw-r--r--   0        0        0     6255 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-spec/test_pyawkward_ListArray32_getitem_next_array_64.py
--rw-r--r--   0        0        0    37324 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-spec/test_pyawkward_ListArray32_getitem_next_array_advanced_64.py
--rw-r--r--   0        0        0     1093 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-spec/test_pyawkward_ListArray32_getitem_next_at_64.py
--rw-r--r--   0        0        0      375 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-spec/test_pyawkward_ListArray32_getitem_next_range_64.py
--rw-r--r--   0        0        0      384 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-spec/test_pyawkward_ListArray32_getitem_next_range_carrylength.py
--rw-r--r--   0        0        0     2221 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-spec/test_pyawkward_ListArray32_getitem_next_range_counts_64.py
--rw-r--r--   0        0        0      390 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-spec/test_pyawkward_ListArray32_getitem_next_range_spreadadvanced_64.py
--rw-r--r--   0        0        0     1371 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-spec/test_pyawkward_ListArray32_localindex_64.py
--rw-r--r--   0        0        0     2369 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-spec/test_pyawkward_ListArray32_min_range.py
--rw-r--r--   0        0        0     2690 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-spec/test_pyawkward_ListArray32_rpad_and_clip_length_axis1.py
--rw-r--r--   0        0        0     4544 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-spec/test_pyawkward_ListArray32_rpad_axis1_64.py
--rw-r--r--   0        0        0     1911 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-spec/test_pyawkward_ListArray32_validity.py
--rw-r--r--   0        0        0     1263 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-spec/test_pyawkward_ListArray64_broadcast_tooffsets_64.py
--rw-r--r--   0        0        0    17509 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-spec/test_pyawkward_ListArray64_combinations_length_64.py
--rw-r--r--   0        0        0     2676 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-spec/test_pyawkward_ListArray64_compact_offsets_64.py
--rw-r--r--   0        0        0    10002 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-spec/test_pyawkward_ListArray64_getitem_jagged_apply_64.py
--rw-r--r--   0        0        0    15834 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-spec/test_pyawkward_ListArray64_getitem_jagged_descend_64.py
--rw-r--r--   0        0        0     4925 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-spec/test_pyawkward_ListArray64_getitem_jagged_expand_64.py
--rw-r--r--   0        0        0     6255 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-spec/test_pyawkward_ListArray64_getitem_next_array_64.py
--rw-r--r--   0        0        0    37324 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-spec/test_pyawkward_ListArray64_getitem_next_array_advanced_64.py
--rw-r--r--   0        0        0     1093 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-spec/test_pyawkward_ListArray64_getitem_next_at_64.py
--rw-r--r--   0        0        0      375 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-spec/test_pyawkward_ListArray64_getitem_next_range_64.py
--rw-r--r--   0        0        0      384 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-spec/test_pyawkward_ListArray64_getitem_next_range_carrylength.py
--rw-r--r--   0        0        0     2221 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-spec/test_pyawkward_ListArray64_getitem_next_range_counts_64.py
--rw-r--r--   0        0        0      390 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-spec/test_pyawkward_ListArray64_getitem_next_range_spreadadvanced_64.py
--rw-r--r--   0        0        0     1371 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-spec/test_pyawkward_ListArray64_localindex_64.py
--rw-r--r--   0        0        0     2369 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-spec/test_pyawkward_ListArray64_min_range.py
--rw-r--r--   0        0        0     2690 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-spec/test_pyawkward_ListArray64_rpad_and_clip_length_axis1.py
--rw-r--r--   0        0        0     4544 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-spec/test_pyawkward_ListArray64_rpad_axis1_64.py
--rw-r--r--   0        0        0     1911 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-spec/test_pyawkward_ListArray64_validity.py
--rw-r--r--   0        0        0     1267 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-spec/test_pyawkward_ListArrayU32_broadcast_tooffsets_64.py
--rw-r--r--   0        0        0    17559 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-spec/test_pyawkward_ListArrayU32_combinations_length_64.py
--rw-r--r--   0        0        0     2686 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-spec/test_pyawkward_ListArrayU32_compact_offsets_64.py
--rw-r--r--   0        0        0    10022 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-spec/test_pyawkward_ListArrayU32_getitem_jagged_apply_64.py
--rw-r--r--   0        0        0    15884 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-spec/test_pyawkward_ListArrayU32_getitem_jagged_descend_64.py
--rw-r--r--   0        0        0     4935 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-spec/test_pyawkward_ListArrayU32_getitem_jagged_expand_64.py
--rw-r--r--   0        0        0     6269 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-spec/test_pyawkward_ListArrayU32_getitem_next_array_64.py
--rw-r--r--   0        0        0    37410 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-spec/test_pyawkward_ListArrayU32_getitem_next_array_advanced_64.py
--rw-r--r--   0        0        0     1097 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-spec/test_pyawkward_ListArrayU32_getitem_next_at_64.py
--rw-r--r--   0        0        0      376 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-spec/test_pyawkward_ListArrayU32_getitem_next_range_64.py
--rw-r--r--   0        0        0      385 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-spec/test_pyawkward_ListArrayU32_getitem_next_range_carrylength.py
--rw-r--r--   0        0        0     2231 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-spec/test_pyawkward_ListArrayU32_getitem_next_range_counts_64.py
--rw-r--r--   0        0        0      391 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-spec/test_pyawkward_ListArrayU32_getitem_next_range_spreadadvanced_64.py
--rw-r--r--   0        0        0     1377 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-spec/test_pyawkward_ListArrayU32_localindex_64.py
--rw-r--r--   0        0        0     2379 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-spec/test_pyawkward_ListArrayU32_min_range.py
--rw-r--r--   0        0        0     2700 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-spec/test_pyawkward_ListArrayU32_rpad_and_clip_length_axis1.py
--rw-r--r--   0        0        0     4554 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-spec/test_pyawkward_ListArrayU32_rpad_axis1_64.py
--rw-r--r--   0        0        0     1921 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-spec/test_pyawkward_ListArrayU32_validity.py
--rw-r--r--   0        0        0     4327 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-spec/test_pyawkward_ListArray_fill_to64_from32.py
--rw-r--r--   0        0        0     4327 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-spec/test_pyawkward_ListArray_fill_to64_from64.py
--rw-r--r--   0        0        0     4337 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-spec/test_pyawkward_ListArray_fill_to64_fromU32.py
--rw-r--r--   0        0        0     2715 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-spec/test_pyawkward_ListArray_getitem_jagged_carrylen_64.py
--rw-r--r--   0        0        0      378 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-spec/test_pyawkward_ListArray_getitem_jagged_numvalid_64.py
--rw-r--r--   0        0        0    20317 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-spec/test_pyawkward_ListArray_getitem_jagged_shrink_64.py
--rw-r--r--   0        0        0     2399 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-spec/test_pyawkward_ListOffsetArray32_compact_offsets_64.py
--rw-r--r--   0        0        0    15557 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-spec/test_pyawkward_ListOffsetArray32_flatten_offsets_64.py
--rw-r--r--   0        0        0      382 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-spec/test_pyawkward_ListOffsetArray32_rpad_and_clip_axis1_64.py
--rw-r--r--   0        0        0      373 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-spec/test_pyawkward_ListOffsetArray32_rpad_axis1_64.py
--rw-r--r--   0        0        0      377 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-spec/test_pyawkward_ListOffsetArray32_rpad_length_axis1.py
--rw-r--r--   0        0        0     2021 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-spec/test_pyawkward_ListOffsetArray32_toRegularArray.py
--rw-r--r--   0        0        0     2399 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-spec/test_pyawkward_ListOffsetArray64_compact_offsets_64.py
--rw-r--r--   0        0        0    15557 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-spec/test_pyawkward_ListOffsetArray64_flatten_offsets_64.py
--rw-r--r--   0        0        0      382 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-spec/test_pyawkward_ListOffsetArray64_rpad_and_clip_axis1_64.py
--rw-r--r--   0        0        0      373 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-spec/test_pyawkward_ListOffsetArray64_rpad_axis1_64.py
--rw-r--r--   0        0        0      377 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-spec/test_pyawkward_ListOffsetArray64_rpad_length_axis1.py
--rw-r--r--   0        0        0     2021 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-spec/test_pyawkward_ListOffsetArray64_toRegularArray.py
--rw-r--r--   0        0        0     2409 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-spec/test_pyawkward_ListOffsetArrayU32_compact_offsets_64.py
--rw-r--r--   0        0        0    15607 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-spec/test_pyawkward_ListOffsetArrayU32_flatten_offsets_64.py
--rw-r--r--   0        0        0      383 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-spec/test_pyawkward_ListOffsetArrayU32_rpad_and_clip_axis1_64.py
--rw-r--r--   0        0        0      374 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-spec/test_pyawkward_ListOffsetArrayU32_rpad_axis1_64.py
--rw-r--r--   0        0        0      378 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-spec/test_pyawkward_ListOffsetArrayU32_rpad_length_axis1.py
--rw-r--r--   0        0        0     2031 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-spec/test_pyawkward_ListOffsetArrayU32_toRegularArray.py
--rw-r--r--   0        0        0    15112 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-spec/test_pyawkward_ListOffsetArray_drop_none_indexes_32.py
--rw-r--r--   0        0        0    15112 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-spec/test_pyawkward_ListOffsetArray_drop_none_indexes_64.py
--rw-r--r--   0        0        0      385 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-spec/test_pyawkward_ListOffsetArray_reduce_local_nextparents_64.py
--rw-r--r--   0        0        0      384 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-spec/test_pyawkward_ListOffsetArray_reduce_local_outoffsets_64.py
--rw-r--r--   0        0        0      397 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-spec/test_pyawkward_ListOffsetArray_reduce_nonlocal_maxcount_offsetscopy_64.py
--rw-r--r--   0        0        0      387 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-spec/test_pyawkward_ListOffsetArray_reduce_nonlocal_nextshifts_64.py
--rw-r--r--   0        0        0      387 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-spec/test_pyawkward_ListOffsetArray_reduce_nonlocal_nextstarts_64.py
--rw-r--r--   0        0        0      391 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-spec/test_pyawkward_ListOffsetArray_reduce_nonlocal_outstartsstops_64.py
--rw-r--r--   0        0        0    18832 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-spec/test_pyawkward_MaskedArray32_getitem_next_jagged_project.py
--rw-r--r--   0        0        0    18832 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-spec/test_pyawkward_MaskedArray64_getitem_next_jagged_project.py
--rw-r--r--   0        0        0    18882 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-spec/test_pyawkward_MaskedArrayU32_getitem_next_jagged_project.py
--rw-r--r--   0        0        0      379 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-spec/test_pyawkward_NumpyArray_fill_tofloat32_fromfloat32.py
--rw-r--r--   0        0        0      379 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-spec/test_pyawkward_NumpyArray_fill_tofloat32_fromfloat64.py
--rw-r--r--   0        0        0      377 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-spec/test_pyawkward_NumpyArray_fill_tofloat32_fromint16.py
--rw-r--r--   0        0        0      377 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-spec/test_pyawkward_NumpyArray_fill_tofloat32_fromint32.py
--rw-r--r--   0        0        0      377 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-spec/test_pyawkward_NumpyArray_fill_tofloat32_fromint64.py
--rw-r--r--   0        0        0      376 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-spec/test_pyawkward_NumpyArray_fill_tofloat32_fromint8.py
--rw-r--r--   0        0        0      378 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-spec/test_pyawkward_NumpyArray_fill_tofloat32_fromuint16.py
--rw-r--r--   0        0        0      378 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-spec/test_pyawkward_NumpyArray_fill_tofloat32_fromuint32.py
--rw-r--r--   0        0        0      378 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-spec/test_pyawkward_NumpyArray_fill_tofloat32_fromuint64.py
--rw-r--r--   0        0        0      377 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-spec/test_pyawkward_NumpyArray_fill_tofloat32_fromuint8.py
--rw-r--r--   0        0        0      379 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-spec/test_pyawkward_NumpyArray_fill_tofloat64_fromfloat32.py
--rw-r--r--   0        0        0      379 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-spec/test_pyawkward_NumpyArray_fill_tofloat64_fromfloat64.py
--rw-r--r--   0        0        0      377 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-spec/test_pyawkward_NumpyArray_fill_tofloat64_fromint16.py
--rw-r--r--   0        0        0      377 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-spec/test_pyawkward_NumpyArray_fill_tofloat64_fromint32.py
--rw-r--r--   0        0        0      377 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-spec/test_pyawkward_NumpyArray_fill_tofloat64_fromint64.py
--rw-r--r--   0        0        0      376 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-spec/test_pyawkward_NumpyArray_fill_tofloat64_fromint8.py
--rw-r--r--   0        0        0      378 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-spec/test_pyawkward_NumpyArray_fill_tofloat64_fromuint16.py
--rw-r--r--   0        0        0      378 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-spec/test_pyawkward_NumpyArray_fill_tofloat64_fromuint32.py
--rw-r--r--   0        0        0      378 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-spec/test_pyawkward_NumpyArray_fill_tofloat64_fromuint64.py
--rw-r--r--   0        0        0      377 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-spec/test_pyawkward_NumpyArray_fill_tofloat64_fromuint8.py
--rw-r--r--   0        0        0      377 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-spec/test_pyawkward_NumpyArray_fill_toint16_fromfloat32.py
--rw-r--r--   0        0        0      377 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-spec/test_pyawkward_NumpyArray_fill_toint16_fromfloat64.py
--rw-r--r--   0        0        0      375 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-spec/test_pyawkward_NumpyArray_fill_toint16_fromint16.py
--rw-r--r--   0        0        0      375 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-spec/test_pyawkward_NumpyArray_fill_toint16_fromint32.py
--rw-r--r--   0        0        0      375 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-spec/test_pyawkward_NumpyArray_fill_toint16_fromint64.py
--rw-r--r--   0        0        0      374 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-spec/test_pyawkward_NumpyArray_fill_toint16_fromint8.py
--rw-r--r--   0        0        0      376 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-spec/test_pyawkward_NumpyArray_fill_toint16_fromuint16.py
--rw-r--r--   0        0        0      376 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-spec/test_pyawkward_NumpyArray_fill_toint16_fromuint32.py
--rw-r--r--   0        0        0      376 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-spec/test_pyawkward_NumpyArray_fill_toint16_fromuint64.py
--rw-r--r--   0        0        0      375 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-spec/test_pyawkward_NumpyArray_fill_toint16_fromuint8.py
--rw-r--r--   0        0        0      377 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-spec/test_pyawkward_NumpyArray_fill_toint32_fromfloat32.py
--rw-r--r--   0        0        0      377 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-spec/test_pyawkward_NumpyArray_fill_toint32_fromfloat64.py
--rw-r--r--   0        0        0      375 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-spec/test_pyawkward_NumpyArray_fill_toint32_fromint16.py
--rw-r--r--   0        0        0      375 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-spec/test_pyawkward_NumpyArray_fill_toint32_fromint32.py
--rw-r--r--   0        0        0      375 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-spec/test_pyawkward_NumpyArray_fill_toint32_fromint64.py
--rw-r--r--   0        0        0      374 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-spec/test_pyawkward_NumpyArray_fill_toint32_fromint8.py
--rw-r--r--   0        0        0      376 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-spec/test_pyawkward_NumpyArray_fill_toint32_fromuint16.py
--rw-r--r--   0        0        0      376 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-spec/test_pyawkward_NumpyArray_fill_toint32_fromuint32.py
--rw-r--r--   0        0        0      376 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-spec/test_pyawkward_NumpyArray_fill_toint32_fromuint64.py
--rw-r--r--   0        0        0      375 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-spec/test_pyawkward_NumpyArray_fill_toint32_fromuint8.py
--rw-r--r--   0        0        0      377 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-spec/test_pyawkward_NumpyArray_fill_toint64_fromfloat32.py
--rw-r--r--   0        0        0      377 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-spec/test_pyawkward_NumpyArray_fill_toint64_fromfloat64.py
--rw-r--r--   0        0        0      375 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-spec/test_pyawkward_NumpyArray_fill_toint64_fromint16.py
--rw-r--r--   0        0        0      375 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-spec/test_pyawkward_NumpyArray_fill_toint64_fromint32.py
--rw-r--r--   0        0        0      375 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-spec/test_pyawkward_NumpyArray_fill_toint64_fromint64.py
--rw-r--r--   0        0        0      374 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-spec/test_pyawkward_NumpyArray_fill_toint64_fromint8.py
--rw-r--r--   0        0        0      376 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-spec/test_pyawkward_NumpyArray_fill_toint64_fromuint16.py
--rw-r--r--   0        0        0      376 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-spec/test_pyawkward_NumpyArray_fill_toint64_fromuint32.py
--rw-r--r--   0        0        0      376 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-spec/test_pyawkward_NumpyArray_fill_toint64_fromuint64.py
--rw-r--r--   0        0        0      375 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-spec/test_pyawkward_NumpyArray_fill_toint64_fromuint8.py
--rw-r--r--   0        0        0      376 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-spec/test_pyawkward_NumpyArray_fill_toint8_fromfloat32.py
--rw-r--r--   0        0        0      376 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-spec/test_pyawkward_NumpyArray_fill_toint8_fromfloat64.py
--rw-r--r--   0        0        0      374 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-spec/test_pyawkward_NumpyArray_fill_toint8_fromint16.py
--rw-r--r--   0        0        0      374 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-spec/test_pyawkward_NumpyArray_fill_toint8_fromint32.py
--rw-r--r--   0        0        0      374 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-spec/test_pyawkward_NumpyArray_fill_toint8_fromint64.py
--rw-r--r--   0        0        0      373 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-spec/test_pyawkward_NumpyArray_fill_toint8_fromint8.py
--rw-r--r--   0        0        0      375 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-spec/test_pyawkward_NumpyArray_fill_toint8_fromuint16.py
--rw-r--r--   0        0        0      375 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-spec/test_pyawkward_NumpyArray_fill_toint8_fromuint32.py
--rw-r--r--   0        0        0      375 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-spec/test_pyawkward_NumpyArray_fill_toint8_fromuint64.py
--rw-r--r--   0        0        0      374 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-spec/test_pyawkward_NumpyArray_fill_toint8_fromuint8.py
--rw-r--r--   0        0        0      378 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-spec/test_pyawkward_NumpyArray_fill_touint16_fromfloat32.py
--rw-r--r--   0        0        0      378 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-spec/test_pyawkward_NumpyArray_fill_touint16_fromfloat64.py
--rw-r--r--   0        0        0      376 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-spec/test_pyawkward_NumpyArray_fill_touint16_fromint16.py
--rw-r--r--   0        0        0      376 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-spec/test_pyawkward_NumpyArray_fill_touint16_fromint32.py
--rw-r--r--   0        0        0      376 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-spec/test_pyawkward_NumpyArray_fill_touint16_fromint64.py
--rw-r--r--   0        0        0      375 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-spec/test_pyawkward_NumpyArray_fill_touint16_fromint8.py
--rw-r--r--   0        0        0      377 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-spec/test_pyawkward_NumpyArray_fill_touint16_fromuint16.py
--rw-r--r--   0        0        0      377 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-spec/test_pyawkward_NumpyArray_fill_touint16_fromuint32.py
--rw-r--r--   0        0        0      377 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-spec/test_pyawkward_NumpyArray_fill_touint16_fromuint64.py
--rw-r--r--   0        0        0      376 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-spec/test_pyawkward_NumpyArray_fill_touint16_fromuint8.py
--rw-r--r--   0        0        0      378 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-spec/test_pyawkward_NumpyArray_fill_touint32_fromfloat32.py
--rw-r--r--   0        0        0      378 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-spec/test_pyawkward_NumpyArray_fill_touint32_fromfloat64.py
--rw-r--r--   0        0        0      376 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-spec/test_pyawkward_NumpyArray_fill_touint32_fromint16.py
--rw-r--r--   0        0        0      376 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-spec/test_pyawkward_NumpyArray_fill_touint32_fromint32.py
--rw-r--r--   0        0        0      376 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-spec/test_pyawkward_NumpyArray_fill_touint32_fromint64.py
--rw-r--r--   0        0        0      375 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-spec/test_pyawkward_NumpyArray_fill_touint32_fromint8.py
--rw-r--r--   0        0        0      377 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-spec/test_pyawkward_NumpyArray_fill_touint32_fromuint16.py
--rw-r--r--   0        0        0      377 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-spec/test_pyawkward_NumpyArray_fill_touint32_fromuint32.py
--rw-r--r--   0        0        0      377 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-spec/test_pyawkward_NumpyArray_fill_touint32_fromuint64.py
--rw-r--r--   0        0        0      376 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-spec/test_pyawkward_NumpyArray_fill_touint32_fromuint8.py
--rw-r--r--   0        0        0      378 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-spec/test_pyawkward_NumpyArray_fill_touint64_fromfloat32.py
--rw-r--r--   0        0        0      378 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-spec/test_pyawkward_NumpyArray_fill_touint64_fromfloat64.py
--rw-r--r--   0        0        0      376 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-spec/test_pyawkward_NumpyArray_fill_touint64_fromint16.py
--rw-r--r--   0        0        0      376 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-spec/test_pyawkward_NumpyArray_fill_touint64_fromint32.py
--rw-r--r--   0        0        0      376 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-spec/test_pyawkward_NumpyArray_fill_touint64_fromint64.py
--rw-r--r--   0        0        0      375 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-spec/test_pyawkward_NumpyArray_fill_touint64_fromint8.py
--rw-r--r--   0        0        0      377 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-spec/test_pyawkward_NumpyArray_fill_touint64_fromuint16.py
--rw-r--r--   0        0        0      377 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-spec/test_pyawkward_NumpyArray_fill_touint64_fromuint32.py
--rw-r--r--   0        0        0      377 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-spec/test_pyawkward_NumpyArray_fill_touint64_fromuint64.py
--rw-r--r--   0        0        0      376 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-spec/test_pyawkward_NumpyArray_fill_touint64_fromuint8.py
--rw-r--r--   0        0        0      377 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-spec/test_pyawkward_NumpyArray_fill_touint8_fromfloat32.py
--rw-r--r--   0        0        0      377 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-spec/test_pyawkward_NumpyArray_fill_touint8_fromfloat64.py
--rw-r--r--   0        0        0      375 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-spec/test_pyawkward_NumpyArray_fill_touint8_fromint16.py
--rw-r--r--   0        0        0      375 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-spec/test_pyawkward_NumpyArray_fill_touint8_fromint32.py
--rw-r--r--   0        0        0      375 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-spec/test_pyawkward_NumpyArray_fill_touint8_fromint64.py
--rw-r--r--   0        0        0      374 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-spec/test_pyawkward_NumpyArray_fill_touint8_fromint8.py
--rw-r--r--   0        0        0      376 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-spec/test_pyawkward_NumpyArray_fill_touint8_fromuint16.py
--rw-r--r--   0        0        0      376 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-spec/test_pyawkward_NumpyArray_fill_touint8_fromuint32.py
--rw-r--r--   0        0        0      376 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-spec/test_pyawkward_NumpyArray_fill_touint8_fromuint64.py
--rw-r--r--   0        0        0      375 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-spec/test_pyawkward_NumpyArray_fill_touint8_fromuint8.py
--rw-r--r--   0        0        0      388 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-spec/test_pyawkward_NumpyArray_rearrange_shifted_toint64_fromint64.py
--rw-r--r--   0        0        0      376 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-spec/test_pyawkward_NumpyArray_reduce_adjust_starts_64.py
--rw-r--r--   0        0        0      383 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-spec/test_pyawkward_NumpyArray_reduce_adjust_starts_shifts_64.py
--rw-r--r--   0        0        0      383 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-spec/test_pyawkward_NumpyArray_reduce_mask_ByteMaskedArray_64.py
--rw-r--r--   0        0        0     8909 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-spec/test_pyawkward_RegularArray_broadcast_tooffsets_64.py
--rw-r--r--   0        0        0      614 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-spec/test_pyawkward_RegularArray_broadcast_tooffsets_size1_64.py
--rw-r--r--   0        0        0     2011 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-spec/test_pyawkward_RegularArray_compact_offsets64.py
--rw-r--r--   0        0        0     9307 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-spec/test_pyawkward_RegularArray_getitem_carry_64.py
--rw-r--r--   0        0        0    15083 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-spec/test_pyawkward_RegularArray_getitem_jagged_expand_64.py
--rw-r--r--   0        0        0    18712 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-spec/test_pyawkward_RegularArray_getitem_next_array_64.py
--rw-r--r--   0        0        0    94644 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-spec/test_pyawkward_RegularArray_getitem_next_array_advanced_64.py
--rw-r--r--   0        0        0    10596 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-spec/test_pyawkward_RegularArray_getitem_next_array_regularize_64.py
--rw-r--r--   0        0        0     1636 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-spec/test_pyawkward_RegularArray_getitem_next_at_64.py
--rw-r--r--   0        0        0      691 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-spec/test_pyawkward_RegularArray_getitem_next_range_64.py
--rw-r--r--   0        0        0    10823 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-spec/test_pyawkward_RegularArray_getitem_next_range_spreadadvanced_64.py
--rw-r--r--   0        0        0     1620 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-spec/test_pyawkward_RegularArray_localindex_64.py
--rw-r--r--   0        0        0      382 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-spec/test_pyawkward_RegularArray_reduce_local_nextparents_64.py
--rw-r--r--   0        0        0      385 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-spec/test_pyawkward_RegularArray_reduce_nonlocal_preparenext_64.py
--rw-r--r--   0        0        0      609 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-spec/test_pyawkward_RegularArray_rpad_and_clip_axis1_64.py
--rw-r--r--   0        0        0      373 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-spec/test_pyawkward_UnionArray32_flatten_combine_64.py
--rw-r--r--   0        0        0      372 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-spec/test_pyawkward_UnionArray32_flatten_length_64.py
--rw-r--r--   0        0        0      373 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-spec/test_pyawkward_UnionArray64_flatten_combine_64.py
--rw-r--r--   0        0        0      372 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-spec/test_pyawkward_UnionArray64_flatten_length_64.py
--rw-r--r--   0        0        0      381 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-spec/test_pyawkward_UnionArray8_32_nestedfill_tags_index_64.py
--rw-r--r--   0        0        0     9557 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-spec/test_pyawkward_UnionArray8_32_project_64.py
--rw-r--r--   0        0        0     3092 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-spec/test_pyawkward_UnionArray8_32_regular_index.py
--rw-r--r--   0        0        0   486418 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-spec/test_pyawkward_UnionArray8_32_simplify8_32_to8_64.py
--rw-r--r--   0        0        0   486418 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-spec/test_pyawkward_UnionArray8_32_simplify8_64_to8_64.py
--rw-r--r--   0        0        0   487418 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-spec/test_pyawkward_UnionArray8_32_simplify8_U32_to8_64.py
--rw-r--r--   0        0        0    11282 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-spec/test_pyawkward_UnionArray8_32_simplify_one_to8_64.py
--rw-r--r--   0        0        0    58126 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-spec/test_pyawkward_UnionArray8_32_validity.py
--rw-r--r--   0        0        0      381 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-spec/test_pyawkward_UnionArray8_64_nestedfill_tags_index_64.py
--rw-r--r--   0        0        0     9557 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-spec/test_pyawkward_UnionArray8_64_project_64.py
--rw-r--r--   0        0        0     3092 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-spec/test_pyawkward_UnionArray8_64_regular_index.py
--rw-r--r--   0        0        0   486418 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-spec/test_pyawkward_UnionArray8_64_simplify8_32_to8_64.py
--rw-r--r--   0        0        0   486418 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-spec/test_pyawkward_UnionArray8_64_simplify8_64_to8_64.py
--rw-r--r--   0        0        0   487418 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-spec/test_pyawkward_UnionArray8_64_simplify8_U32_to8_64.py
--rw-r--r--   0        0        0    11282 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-spec/test_pyawkward_UnionArray8_64_simplify_one_to8_64.py
--rw-r--r--   0        0        0    58126 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-spec/test_pyawkward_UnionArray8_64_validity.py
--rw-r--r--   0        0        0      382 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-spec/test_pyawkward_UnionArray8_U32_nestedfill_tags_index_64.py
--rw-r--r--   0        0        0     9587 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-spec/test_pyawkward_UnionArray8_U32_project_64.py
--rw-r--r--   0        0        0     3102 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-spec/test_pyawkward_UnionArray8_U32_regular_index.py
--rw-r--r--   0        0        0   487418 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-spec/test_pyawkward_UnionArray8_U32_simplify8_32_to8_64.py
--rw-r--r--   0        0        0   487418 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-spec/test_pyawkward_UnionArray8_U32_simplify8_64_to8_64.py
--rw-r--r--   0        0        0   488418 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-spec/test_pyawkward_UnionArray8_U32_simplify8_U32_to8_64.py
--rw-r--r--   0        0        0    11312 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-spec/test_pyawkward_UnionArray8_U32_simplify_one_to8_64.py
--rw-r--r--   0        0        0    58376 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-spec/test_pyawkward_UnionArray8_U32_validity.py
--rw-r--r--   0        0        0     2077 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-spec/test_pyawkward_UnionArray8_regular_index_getsize.py
--rw-r--r--   0        0        0      374 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-spec/test_pyawkward_UnionArrayU32_flatten_combine_64.py
--rw-r--r--   0        0        0      373 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-spec/test_pyawkward_UnionArrayU32_flatten_length_64.py
--rw-r--r--   0        0        0      586 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-spec/test_pyawkward_UnionArray_fillindex_to64_count.py
--rw-r--r--   0        0        0     2621 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-spec/test_pyawkward_UnionArray_fillindex_to64_from32.py
--rw-r--r--   0        0        0     2621 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-spec/test_pyawkward_UnionArray_fillindex_to64_from64.py
--rw-r--r--   0        0        0     2631 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-spec/test_pyawkward_UnionArray_fillindex_to64_fromU32.py
--rw-r--r--   0        0        0     2156 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-spec/test_pyawkward_UnionArray_fillna_from32_to64.py
--rw-r--r--   0        0        0     2156 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-spec/test_pyawkward_UnionArray_fillna_from64_to64.py
--rw-r--r--   0        0        0     2166 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-spec/test_pyawkward_UnionArray_fillna_fromU32_to64.py
--rw-r--r--   0        0        0      596 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-spec/test_pyawkward_UnionArray_filltags_to8_const.py
--rw-r--r--   0        0        0     2727 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-spec/test_pyawkward_UnionArray_filltags_to8_from8.py
--rw-r--r--   0        0        0      523 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-spec/test_pyawkward_index_rpad_and_clip_axis0_64.py
--rw-r--r--   0        0        0      682 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-spec/test_pyawkward_index_rpad_and_clip_axis1_64.py
--rw-r--r--   0        0        0      463 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-spec/test_pyawkward_localindex_64.py
--rw-r--r--   0        0        0    13193 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-spec/test_pyawkward_missing_repeat_64.py
--rw-r--r--   0        0        0      366 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-spec/test_pyawkward_reduce_argmax_float32_64.py
--rw-r--r--   0        0        0      366 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-spec/test_pyawkward_reduce_argmax_float64_64.py
--rw-r--r--   0        0        0      364 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-spec/test_pyawkward_reduce_argmax_int16_64.py
--rw-r--r--   0        0        0      364 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-spec/test_pyawkward_reduce_argmax_int32_64.py
--rw-r--r--   0        0        0      364 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-spec/test_pyawkward_reduce_argmax_int64_64.py
--rw-r--r--   0        0        0      363 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-spec/test_pyawkward_reduce_argmax_int8_64.py
--rw-r--r--   0        0        0      365 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-spec/test_pyawkward_reduce_argmax_uint16_64.py
--rw-r--r--   0        0        0      365 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-spec/test_pyawkward_reduce_argmax_uint32_64.py
--rw-r--r--   0        0        0      365 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-spec/test_pyawkward_reduce_argmax_uint64_64.py
--rw-r--r--   0        0        0      364 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-spec/test_pyawkward_reduce_argmax_uint8_64.py
--rw-r--r--   0        0        0      366 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-spec/test_pyawkward_reduce_argmin_float32_64.py
--rw-r--r--   0        0        0      366 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-spec/test_pyawkward_reduce_argmin_float64_64.py
--rw-r--r--   0        0        0      364 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-spec/test_pyawkward_reduce_argmin_int16_64.py
--rw-r--r--   0        0        0      364 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-spec/test_pyawkward_reduce_argmin_int32_64.py
--rw-r--r--   0        0        0      364 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-spec/test_pyawkward_reduce_argmin_int64_64.py
--rw-r--r--   0        0        0      363 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-spec/test_pyawkward_reduce_argmin_int8_64.py
--rw-r--r--   0        0        0      365 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-spec/test_pyawkward_reduce_argmin_uint16_64.py
--rw-r--r--   0        0        0      365 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-spec/test_pyawkward_reduce_argmin_uint32_64.py
--rw-r--r--   0        0        0      365 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-spec/test_pyawkward_reduce_argmin_uint64_64.py
--rw-r--r--   0        0        0      364 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-spec/test_pyawkward_reduce_argmin_uint8_64.py
--rw-r--r--   0        0        0      357 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-spec/test_pyawkward_reduce_count_64.py
--rw-r--r--   0        0        0      369 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-spec/test_pyawkward_reduce_countnonzero_bool_64.py
--rw-r--r--   0        0        0      372 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-spec/test_pyawkward_reduce_countnonzero_float32_64.py
--rw-r--r--   0        0        0      372 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-spec/test_pyawkward_reduce_countnonzero_float64_64.py
--rw-r--r--   0        0        0      370 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-spec/test_pyawkward_reduce_countnonzero_int16_64.py
--rw-r--r--   0        0        0      370 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-spec/test_pyawkward_reduce_countnonzero_int32_64.py
--rw-r--r--   0        0        0      370 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-spec/test_pyawkward_reduce_countnonzero_int64_64.py
--rw-r--r--   0        0        0      369 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-spec/test_pyawkward_reduce_countnonzero_int8_64.py
--rw-r--r--   0        0        0      371 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-spec/test_pyawkward_reduce_countnonzero_uint16_64.py
--rw-r--r--   0        0        0      371 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-spec/test_pyawkward_reduce_countnonzero_uint32_64.py
--rw-r--r--   0        0        0      371 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-spec/test_pyawkward_reduce_countnonzero_uint64_64.py
--rw-r--r--   0        0        0      370 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-spec/test_pyawkward_reduce_countnonzero_uint8_64.py
--rw-r--r--   0        0        0      371 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-spec/test_pyawkward_reduce_max_float32_float32_64.py
--rw-r--r--   0        0        0      371 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-spec/test_pyawkward_reduce_max_float64_float64_64.py
--rw-r--r--   0        0        0      367 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-spec/test_pyawkward_reduce_max_int16_int16_64.py
--rw-r--r--   0        0        0      367 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-spec/test_pyawkward_reduce_max_int32_int32_64.py
--rw-r--r--   0        0        0      367 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-spec/test_pyawkward_reduce_max_int64_int64_64.py
--rw-r--r--   0        0        0      365 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-spec/test_pyawkward_reduce_max_int8_int8_64.py
--rw-r--r--   0        0        0      369 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-spec/test_pyawkward_reduce_max_uint16_uint16_64.py
--rw-r--r--   0        0        0      369 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-spec/test_pyawkward_reduce_max_uint32_uint32_64.py
--rw-r--r--   0        0        0      369 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-spec/test_pyawkward_reduce_max_uint64_uint64_64.py
--rw-r--r--   0        0        0      367 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-spec/test_pyawkward_reduce_max_uint8_uint8_64.py
--rw-r--r--   0        0        0      371 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-spec/test_pyawkward_reduce_min_float32_float32_64.py
--rw-r--r--   0        0        0      371 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-spec/test_pyawkward_reduce_min_float64_float64_64.py
--rw-r--r--   0        0        0      367 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-spec/test_pyawkward_reduce_min_int16_int16_64.py
--rw-r--r--   0        0        0      367 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-spec/test_pyawkward_reduce_min_int32_int32_64.py
--rw-r--r--   0        0        0      367 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-spec/test_pyawkward_reduce_min_int64_int64_64.py
--rw-r--r--   0        0        0      365 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-spec/test_pyawkward_reduce_min_int8_int8_64.py
--rw-r--r--   0        0        0      369 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-spec/test_pyawkward_reduce_min_uint16_uint16_64.py
--rw-r--r--   0        0        0      369 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-spec/test_pyawkward_reduce_min_uint32_uint32_64.py
--rw-r--r--   0        0        0      369 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-spec/test_pyawkward_reduce_min_uint64_uint64_64.py
--rw-r--r--   0        0        0      367 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-spec/test_pyawkward_reduce_min_uint8_uint8_64.py
--rw-r--r--   0        0        0      366 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-spec/test_pyawkward_reduce_prod_bool_bool_64.py
--rw-r--r--   0        0        0      369 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-spec/test_pyawkward_reduce_prod_bool_float32_64.py
--rw-r--r--   0        0        0      369 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-spec/test_pyawkward_reduce_prod_bool_float64_64.py
--rw-r--r--   0        0        0      367 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-spec/test_pyawkward_reduce_prod_bool_int16_64.py
--rw-r--r--   0        0        0      367 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-spec/test_pyawkward_reduce_prod_bool_int32_64.py
--rw-r--r--   0        0        0      367 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-spec/test_pyawkward_reduce_prod_bool_int64_64.py
--rw-r--r--   0        0        0      366 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-spec/test_pyawkward_reduce_prod_bool_int8_64.py
--rw-r--r--   0        0        0      368 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-spec/test_pyawkward_reduce_prod_bool_uint16_64.py
--rw-r--r--   0        0        0      368 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-spec/test_pyawkward_reduce_prod_bool_uint32_64.py
--rw-r--r--   0        0        0      368 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-spec/test_pyawkward_reduce_prod_bool_uint64_64.py
--rw-r--r--   0        0        0      367 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-spec/test_pyawkward_reduce_prod_bool_uint8_64.py
--rw-r--r--   0        0        0      372 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-spec/test_pyawkward_reduce_prod_float32_float32_64.py
--rw-r--r--   0        0        0      372 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-spec/test_pyawkward_reduce_prod_float64_float64_64.py
--rw-r--r--   0        0        0      368 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-spec/test_pyawkward_reduce_prod_int32_int16_64.py
--rw-r--r--   0        0        0      368 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-spec/test_pyawkward_reduce_prod_int32_int32_64.py
--rw-r--r--   0        0        0      367 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-spec/test_pyawkward_reduce_prod_int32_int8_64.py
--rw-r--r--   0        0        0      368 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-spec/test_pyawkward_reduce_prod_int64_int16_64.py
--rw-r--r--   0        0        0      368 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-spec/test_pyawkward_reduce_prod_int64_int32_64.py
--rw-r--r--   0        0        0      368 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-spec/test_pyawkward_reduce_prod_int64_int64_64.py
--rw-r--r--   0        0        0      367 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-spec/test_pyawkward_reduce_prod_int64_int8_64.py
--rw-r--r--   0        0        0      370 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-spec/test_pyawkward_reduce_prod_uint32_uint16_64.py
--rw-r--r--   0        0        0      370 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-spec/test_pyawkward_reduce_prod_uint32_uint32_64.py
--rw-r--r--   0        0        0      369 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-spec/test_pyawkward_reduce_prod_uint32_uint8_64.py
--rw-r--r--   0        0        0      370 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-spec/test_pyawkward_reduce_prod_uint64_uint16_64.py
--rw-r--r--   0        0        0      370 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-spec/test_pyawkward_reduce_prod_uint64_uint32_64.py
--rw-r--r--   0        0        0      370 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-spec/test_pyawkward_reduce_prod_uint64_uint64_64.py
--rw-r--r--   0        0        0      369 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-spec/test_pyawkward_reduce_prod_uint64_uint8_64.py
--rw-r--r--   0        0        0      365 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-spec/test_pyawkward_reduce_sum_bool_bool_64.py
--rw-r--r--   0        0        0      368 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-spec/test_pyawkward_reduce_sum_bool_float32_64.py
--rw-r--r--   0        0        0      368 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-spec/test_pyawkward_reduce_sum_bool_float64_64.py
--rw-r--r--   0        0        0      366 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-spec/test_pyawkward_reduce_sum_bool_int16_64.py
--rw-r--r--   0        0        0      366 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-spec/test_pyawkward_reduce_sum_bool_int32_64.py
--rw-r--r--   0        0        0      366 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-spec/test_pyawkward_reduce_sum_bool_int64_64.py
--rw-r--r--   0        0        0      365 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-spec/test_pyawkward_reduce_sum_bool_int8_64.py
--rw-r--r--   0        0        0      367 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-spec/test_pyawkward_reduce_sum_bool_uint16_64.py
--rw-r--r--   0        0        0      367 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-spec/test_pyawkward_reduce_sum_bool_uint32_64.py
--rw-r--r--   0        0        0      367 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-spec/test_pyawkward_reduce_sum_bool_uint64_64.py
--rw-r--r--   0        0        0      366 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-spec/test_pyawkward_reduce_sum_bool_uint8_64.py
--rw-r--r--   0        0        0      371 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-spec/test_pyawkward_reduce_sum_float32_float32_64.py
--rw-r--r--   0        0        0      371 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-spec/test_pyawkward_reduce_sum_float64_float64_64.py
--rw-r--r--   0        0        0      366 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-spec/test_pyawkward_reduce_sum_int32_bool_64.py
--rw-r--r--   0        0        0      367 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-spec/test_pyawkward_reduce_sum_int32_int16_64.py
--rw-r--r--   0        0        0      367 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-spec/test_pyawkward_reduce_sum_int32_int32_64.py
--rw-r--r--   0        0        0      366 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-spec/test_pyawkward_reduce_sum_int32_int8_64.py
--rw-r--r--   0        0        0      366 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-spec/test_pyawkward_reduce_sum_int64_bool_64.py
--rw-r--r--   0        0        0      367 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-spec/test_pyawkward_reduce_sum_int64_int16_64.py
--rw-r--r--   0        0        0      367 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-spec/test_pyawkward_reduce_sum_int64_int32_64.py
--rw-r--r--   0        0        0      367 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-spec/test_pyawkward_reduce_sum_int64_int64_64.py
--rw-r--r--   0        0        0      366 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-spec/test_pyawkward_reduce_sum_int64_int8_64.py
--rw-r--r--   0        0        0      369 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-spec/test_pyawkward_reduce_sum_uint32_uint16_64.py
--rw-r--r--   0        0        0      369 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-spec/test_pyawkward_reduce_sum_uint32_uint32_64.py
--rw-r--r--   0        0        0      368 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-spec/test_pyawkward_reduce_sum_uint32_uint8_64.py
--rw-r--r--   0        0        0      369 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-spec/test_pyawkward_reduce_sum_uint64_uint16_64.py
--rw-r--r--   0        0        0      369 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-spec/test_pyawkward_reduce_sum_uint64_uint32_64.py
--rw-r--r--   0        0        0      369 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-spec/test_pyawkward_reduce_sum_uint64_uint64_64.py
--rw-r--r--   0        0        0      368 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-spec/test_pyawkward_reduce_sum_uint64_uint8_64.py
--rw-r--r--   0        0        0    78888 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-spec-explicit/kernels.py
--rw-r--r--   0        0        0     1607 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-spec-explicit/test_awkward_BitMaskedArray_to_ByteMaskedArray.py
--rw-r--r--   0        0        0     1125 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-spec-explicit/test_awkward_BitMaskedArray_to_IndexedOptionArray.py
--rw-r--r--   0        0        0      715 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-spec-explicit/test_awkward_ByteMaskedArray_getitem_nextcarry.py
--rw-r--r--   0        0        0      976 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-spec-explicit/test_awkward_ByteMaskedArray_getitem_nextcarry_outindex.py
--rw-r--r--   0        0        0     5606 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-spec-explicit/test_awkward_ByteMaskedArray_numnull.py
--rw-r--r--   0        0        0      396 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-spec-explicit/test_awkward_ByteMaskedArray_overlay_mask.py
--rw-r--r--   0        0        0      458 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-spec-explicit/test_awkward_ByteMaskedArray_reduce_next_nonlocal_nextshifts_64.py
--rw-r--r--   0        0        0      732 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-spec-explicit/test_awkward_ByteMaskedArray_toIndexedOptionArray.py
--rw-r--r--   0        0        0    16520 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-spec-explicit/test_awkward_Content_getitem_next_missing_jagged_getmaskstartstop.py
--rw-r--r--   0        0        0     1944 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-spec-explicit/test_awkward_IndexedArray_fill.py
--rw-r--r--   0        0        0      378 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-spec-explicit/test_awkward_IndexedArray_flatten_nextcarry.py
--rw-r--r--   0        0        0     3461 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-spec-explicit/test_awkward_IndexedArray_flatten_none2empty.py
--rw-r--r--   0        0        0    10018 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-spec-explicit/test_awkward_IndexedArray_getitem_nextcarry.py
--rw-r--r--   0        0        0     1036 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-spec-explicit/test_awkward_IndexedArray_getitem_nextcarry_outindex.py
--rw-r--r--   0        0        0     4574 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-spec-explicit/test_awkward_IndexedArray_index_of_nulls.py
--rw-r--r--   0        0        0     3746 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-spec-explicit/test_awkward_IndexedArray_numnull.py
--rw-r--r--   0        0        0     6792 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-spec-explicit/test_awkward_IndexedArray_reduce_next_64.py
--rw-r--r--   0        0        0     2890 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-spec-explicit/test_awkward_IndexedArray_reduce_next_fix_offsets_64.py
--rw-r--r--   0        0        0     3921 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-spec-explicit/test_awkward_IndexedArray_reduce_next_nonlocal_nextshifts_64.py
--rw-r--r--   0        0        0     2570 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-spec-explicit/test_awkward_IndexedArray_reduce_next_nonlocal_nextshifts_fromshifts_64.py
--rw-r--r--   0        0        0    15064 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-spec-explicit/test_awkward_IndexedArray_simplify.py
--rw-r--r--   0        0        0     9994 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-spec-explicit/test_awkward_IndexedArray_validity.py
--rw-r--r--   0        0        0      377 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-spec-explicit/test_awkward_IndexedOptionArray_rpad_and_clip_mask_axis1.py
--rw-r--r--   0        0        0    57215 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-spec-explicit/test_awkward_ListArray_broadcast_tooffsets.py
--rw-r--r--   0        0        0     3776 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-spec-explicit/test_awkward_ListArray_combinations_length.py
--rw-r--r--   0        0        0    32221 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-spec-explicit/test_awkward_ListArray_compact_offsets.py
--rw-r--r--   0        0        0     5715 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-spec-explicit/test_awkward_ListArray_fill.py
--rw-r--r--   0        0        0    18763 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-spec-explicit/test_awkward_ListArray_getitem_jagged_apply.py
--rw-r--r--   0        0        0    13720 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-spec-explicit/test_awkward_ListArray_getitem_jagged_carrylen.py
--rw-r--r--   0        0        0     2030 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-spec-explicit/test_awkward_ListArray_getitem_jagged_descend.py
--rw-r--r--   0        0        0     1444 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-spec-explicit/test_awkward_ListArray_getitem_jagged_expand.py
--rw-r--r--   0        0        0     3592 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-spec-explicit/test_awkward_ListArray_getitem_jagged_shrink.py
--rw-r--r--   0        0        0     3161 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-spec-explicit/test_awkward_ListArray_getitem_next_array.py
--rw-r--r--   0        0        0    31580 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-spec-explicit/test_awkward_ListArray_getitem_next_array_advanced.py
--rw-r--r--   0        0        0    18191 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-spec-explicit/test_awkward_ListArray_getitem_next_at.py
--rw-r--r--   0        0        0      683 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-spec-explicit/test_awkward_ListArray_getitem_next_range_counts.py
--rw-r--r--   0        0        0     3572 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-spec-explicit/test_awkward_ListArray_localindex.py
--rw-r--r--   0        0        0     1342 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-spec-explicit/test_awkward_ListArray_min_range.py
--rw-r--r--   0        0        0     4352 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-spec-explicit/test_awkward_ListArray_rpad_and_clip_length_axis1.py
--rw-r--r--   0        0        0     7944 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-spec-explicit/test_awkward_ListArray_rpad_axis1.py
--rw-r--r--   0        0        0    16024 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-spec-explicit/test_awkward_ListArray_validity.py
--rw-r--r--   0        0        0     3089 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-spec-explicit/test_awkward_ListOffsetArray_compact_offsets.py
--rw-r--r--   0        0        0    14322 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-spec-explicit/test_awkward_ListOffsetArray_flatten_offsets.py
--rw-r--r--   0        0        0     8553 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-spec-explicit/test_awkward_ListOffsetArray_reduce_local_outoffsets_64.py
--rw-r--r--   0        0        0    16999 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-spec-explicit/test_awkward_ListOffsetArray_reduce_nonlocal_maxcount_offsetscopy_64.py
--rw-r--r--   0        0        0    32915 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-spec-explicit/test_awkward_ListOffsetArray_reduce_nonlocal_nextshifts_64.py
--rw-r--r--   0        0        0    13774 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-spec-explicit/test_awkward_ListOffsetArray_reduce_nonlocal_nextstarts_64.py
--rw-r--r--   0        0        0    12662 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-spec-explicit/test_awkward_ListOffsetArray_reduce_nonlocal_outstartsstops_64.py
--rw-r--r--   0        0        0     1564 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-spec-explicit/test_awkward_ListOffsetArray_toRegularArray.py
--rw-r--r--   0        0        0     2302 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-spec-explicit/test_awkward_MaskedArray_getitem_next_jagged_project.py
--rw-r--r--   0        0        0    14407 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-spec-explicit/test_awkward_NumpyArray_reduce_mask_ByteMaskedArray_64.py
--rw-r--r--   0        0        0     2252 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-spec-explicit/test_awkward_RegularArray_broadcast_tooffsets.py
--rw-r--r--   0        0        0     7393 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-spec-explicit/test_awkward_RegularArray_broadcast_tooffsets_size1.py
--rw-r--r--   0        0        0     3951 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-spec-explicit/test_awkward_RegularArray_compact_offsets.py
--rw-r--r--   0        0        0    19963 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-spec-explicit/test_awkward_RegularArray_getitem_carry.py
--rw-r--r--   0        0        0    16442 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-spec-explicit/test_awkward_RegularArray_getitem_jagged_expand.py
--rw-r--r--   0        0        0    43829 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-spec-explicit/test_awkward_RegularArray_getitem_next_array.py
--rw-r--r--   0        0        0     8314 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-spec-explicit/test_awkward_RegularArray_getitem_next_array_advanced.py
--rw-r--r--   0        0        0    29046 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-spec-explicit/test_awkward_RegularArray_getitem_next_array_regularize.py
--rw-r--r--   0        0        0     6099 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-spec-explicit/test_awkward_RegularArray_getitem_next_at.py
--rw-r--r--   0        0        0    21666 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-spec-explicit/test_awkward_RegularArray_getitem_next_range.py
--rw-r--r--   0        0        0      833 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-spec-explicit/test_awkward_RegularArray_getitem_next_range_spreadadvanced.py
--rw-r--r--   0        0        0      822 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-spec-explicit/test_awkward_RegularArray_localindex.py
--rw-r--r--   0        0        0     2484 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-spec-explicit/test_awkward_RegularArray_rpad_and_clip_axis1.py
--rw-r--r--   0        0        0      758 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-spec-explicit/test_awkward_UnionArray_fillindex.py
--rw-r--r--   0        0        0     2786 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-spec-explicit/test_awkward_UnionArray_fillindex_count.py
--rw-r--r--   0        0        0     4269 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-spec-explicit/test_awkward_UnionArray_fillna.py
--rw-r--r--   0        0        0      413 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-spec-explicit/test_awkward_UnionArray_filltags.py
--rw-r--r--   0        0        0     5215 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-spec-explicit/test_awkward_UnionArray_project.py
--rw-r--r--   0        0        0     1386 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-spec-explicit/test_awkward_UnionArray_regular_index.py
--rw-r--r--   0        0        0      897 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-spec-explicit/test_awkward_UnionArray_regular_index_getsize.py
--rw-r--r--   0        0        0     1876 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-spec-explicit/test_awkward_UnionArray_simplify.py
--rw-r--r--   0        0        0     3710 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-spec-explicit/test_awkward_UnionArray_simplify_one.py
--rw-r--r--   0        0        0     1989 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-spec-explicit/test_awkward_UnionArray_validity.py
--rw-r--r--   0        0        0     3441 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-spec-explicit/test_awkward_index_rpad_and_clip_axis0.py
--rw-r--r--   0        0        0     5746 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-spec-explicit/test_awkward_index_rpad_and_clip_axis1.py
--rw-r--r--   0        0        0      938 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-spec-explicit/test_awkward_localindex.py
--rw-r--r--   0        0        0    18001 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-spec-explicit/test_awkward_missing_repeat.py
--rw-r--r--   0        0        0     4106 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-spec-explicit/test_awkward_reduce_argmax.py
--rw-r--r--   0        0        0     9790 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-spec-explicit/test_awkward_reduce_argmin.py
--rw-r--r--   0        0        0    20840 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-spec-explicit/test_awkward_reduce_count_64.py
--rw-r--r--   0        0        0     2422 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-spec-explicit/test_awkward_reduce_countnonzero.py
--rw-r--r--   0        0        0     5490 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-spec-explicit/test_awkward_reduce_max.py
--rw-r--r--   0        0        0     6021 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-spec-explicit/test_awkward_reduce_min.py
--rw-r--r--   0        0        0    29009 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-spec-explicit/test_awkward_reduce_prod.py
--rw-r--r--   0        0        0     8895 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-spec-explicit/test_awkward_reduce_prod_bool.py
--rw-r--r--   0        0        0    12658 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-spec-explicit/test_awkward_reduce_sum.py
--rw-r--r--   0        0        0     3164 2023-02-03 22:54:31.000000 awkward-cpp-8/tests-spec-explicit/test_awkward_reduce_sum_bool.py
--rw-r--r--   0        0        0     2120 2023-02-03 22:54:31.000000 awkward-cpp-8/PKG-INFO
+-rw-r--r--   0        0        0      199 2023-02-16 15:37:39.000000 awkward-cpp-9/.gitignore
+-rw-r--r--   0        0        0     4936 2023-02-16 15:37:39.000000 awkward-cpp-9/CMakeLists.txt
+-rw-r--r--   0        0        0     1520 2023-02-16 15:37:39.000000 awkward-cpp-9/LICENSE
+-rw-r--r--   0        0        0      154 2023-02-16 15:37:39.000000 awkward-cpp-9/README.md
+-rw-r--r--   0        0        0   109286 2023-02-16 15:37:39.000000 awkward-cpp-9/docs/Doxyfile
+-rw-r--r--   0        0        0      773 2023-02-16 15:37:39.000000 awkward-cpp-9/docs/footer.html
+-rw-r--r--   0        0        0     1057 2023-02-16 15:37:39.000000 awkward-cpp-9/docs/header.html
+-rw-r--r--   0        0        0     1706 2023-02-16 15:37:39.000000 awkward-cpp-9/docs/index.md
+-rw-r--r--   0        0        0      499 2023-02-16 15:37:39.000000 awkward-cpp-9/docs/stylesheet.css
+-rw-r--r--   0        0        0     1859 2023-02-16 15:37:39.000000 awkward-cpp-9/header-only/awkward/BuilderOptions.h
+-rw-r--r--   0        0        0    19587 2023-02-16 15:37:39.000000 awkward-cpp-9/header-only/awkward/GrowableBuffer.h
+-rw-r--r--   0        0        0    89307 2023-02-16 15:37:39.000000 awkward-cpp-9/header-only/awkward/LayoutBuilder.h
+-rw-r--r--   0        0        0     8025 2023-02-16 15:37:39.000000 awkward-cpp-9/header-only/awkward/utils.h
+-rw-r--r--   0        0        0    13850 2023-02-16 15:37:39.000000 awkward-cpp-9/include/awkward/builder/ArrayBuilder.h
+-rw-r--r--   0        0        0     2825 2023-02-16 15:37:39.000000 awkward-cpp-9/include/awkward/builder/BoolBuilder.h
+-rw-r--r--   0        0        0     5702 2023-02-16 15:37:39.000000 awkward-cpp-9/include/awkward/builder/Builder.h
+-rw-r--r--   0        0        0     3671 2023-02-16 15:37:39.000000 awkward-cpp-9/include/awkward/builder/Complex128Builder.h
+-rw-r--r--   0        0        0     3037 2023-02-16 15:37:39.000000 awkward-cpp-9/include/awkward/builder/DatetimeBuilder.h
+-rw-r--r--   0        0        0     3252 2023-02-16 15:37:39.000000 awkward-cpp-9/include/awkward/builder/Float64Builder.h
+-rw-r--r--   0        0        0     2822 2023-02-16 15:37:39.000000 awkward-cpp-9/include/awkward/builder/Int64Builder.h
+-rw-r--r--   0        0        0     3402 2023-02-16 15:37:39.000000 awkward-cpp-9/include/awkward/builder/ListBuilder.h
+-rw-r--r--   0        0        0     3767 2023-02-16 15:37:39.000000 awkward-cpp-9/include/awkward/builder/OptionBuilder.h
+-rw-r--r--   0        0        0     4505 2023-02-16 15:37:39.000000 awkward-cpp-9/include/awkward/builder/RecordBuilder.h
+-rw-r--r--   0        0        0     3845 2023-02-16 15:37:39.000000 awkward-cpp-9/include/awkward/builder/StringBuilder.h
+-rw-r--r--   0        0        0     3491 2023-02-16 15:37:39.000000 awkward-cpp-9/include/awkward/builder/TupleBuilder.h
+-rw-r--r--   0        0        0     3583 2023-02-16 15:37:39.000000 awkward-cpp-9/include/awkward/builder/UnionBuilder.h
+-rw-r--r--   0        0        0     2763 2023-02-16 15:37:39.000000 awkward-cpp-9/include/awkward/builder/UnknownBuilder.h
+-rw-r--r--   0        0        0     3169 2023-02-16 15:37:39.000000 awkward-cpp-9/include/awkward/common.h
+-rw-r--r--   0        0        0     3616 2023-02-16 15:37:39.000000 awkward-cpp-9/include/awkward/datetime_util.h
+-rw-r--r--   0        0        0     2136 2023-02-16 15:37:39.000000 awkward-cpp-9/include/awkward/forth/ForthInputBuffer.h
+-rw-r--r--   0        0        0    13079 2023-02-16 15:37:39.000000 awkward-cpp-9/include/awkward/forth/ForthMachine.h
+-rw-r--r--   0        0        0     8726 2023-02-16 15:37:39.000000 awkward-cpp-9/include/awkward/forth/ForthOutputBuffer.h
+-rw-r--r--   0        0        0     9197 2023-02-16 15:37:39.000000 awkward-cpp-9/include/awkward/io/json.h
+-rw-r--r--   0        0        0      641 2023-02-16 15:37:39.000000 awkward-cpp-9/include/awkward/kernel-utils.h
+-rw-r--r--   0        0        0    99717 2023-02-16 15:37:39.000000 awkward-cpp-9/include/awkward/kernels.h
+-rw-r--r--   0        0        0     2676 2023-02-16 15:37:39.000000 awkward-cpp-9/include/awkward/python/content.h
+-rw-r--r--   0        0        0      479 2023-02-16 15:37:39.000000 awkward-cpp-9/include/awkward/python/forth.h
+-rw-r--r--   0        0        0      358 2023-02-16 15:37:39.000000 awkward-cpp-9/include/awkward/python/io.h
+-rw-r--r--   0        0        0      416 2023-02-16 15:37:39.000000 awkward-cpp-9/include/awkward/python/kernel_utils.h
+-rw-r--r--   0        0        0     1319 2023-02-16 15:37:39.000000 awkward-cpp-9/include/awkward/python/util.h
+-rw-r--r--   0        0        0     8116 2023-02-16 15:37:39.000000 awkward-cpp-9/include/awkward/util.h
+-rw-r--r--   0        0        0     2265 2023-02-16 15:37:39.000000 awkward-cpp-9/pyproject.toml
+-rw-r--r--   0        0        0       37 2023-02-16 15:37:39.000000 awkward-cpp-9/rapidjson/.git
+-rw-r--r--   0        0        0      450 2023-02-16 15:37:39.000000 awkward-cpp-9/rapidjson/.gitattributes
+-rw-r--r--   0        0        0      349 2023-02-16 15:37:39.000000 awkward-cpp-9/rapidjson/.gitignore
+-rw-r--r--   0        0        0      104 2023-02-16 15:37:39.000000 awkward-cpp-9/rapidjson/.gitmodules
+-rw-r--r--   0        0        0     3455 2023-02-16 15:37:39.000000 awkward-cpp-9/rapidjson/.travis.yml
+-rw-r--r--   0        0        0     6817 2023-02-16 15:37:39.000000 awkward-cpp-9/rapidjson/CHANGELOG.md
+-rw-r--r--   0        0        0     6265 2023-02-16 15:37:39.000000 awkward-cpp-9/rapidjson/CMakeLists.txt
+-rw-r--r--   0        0        0      828 2023-02-16 15:37:39.000000 awkward-cpp-9/rapidjson/CMakeModules/FindGTestSrc.cmake
+-rw-r--r--   0        0        0      229 2023-02-16 15:37:39.000000 awkward-cpp-9/rapidjson/RapidJSON.pc.in
+-rw-r--r--   0        0        0      200 2023-02-16 15:37:39.000000 awkward-cpp-9/rapidjson/RapidJSONConfig.cmake.in
+-rw-r--r--   0        0        0      469 2023-02-16 15:37:39.000000 awkward-cpp-9/rapidjson/RapidJSONConfigVersion.cmake.in
+-rw-r--r--   0        0        0     1043 2023-02-16 15:37:39.000000 awkward-cpp-9/rapidjson/appveyor.yml
+-rw-r--r--   0        0        0      603 2023-02-16 15:37:39.000000 awkward-cpp-9/rapidjson/bin/data/glossary.json
+-rw-r--r--   0        0        0      898 2023-02-16 15:37:39.000000 awkward-cpp-9/rapidjson/bin/data/menu.json
+-rw-r--r--   0        0        0      103 2023-02-16 15:37:39.000000 awkward-cpp-9/rapidjson/bin/data/readme.txt
+-rw-r--r--   0        0        0   687491 2023-02-16 15:37:39.000000 awkward-cpp-9/rapidjson/bin/data/sample.json
+-rw-r--r--   0        0        0     3554 2023-02-16 15:37:39.000000 awkward-cpp-9/rapidjson/bin/data/webapp.json
+-rw-r--r--   0        0        0      626 2023-02-16 15:37:39.000000 awkward-cpp-9/rapidjson/bin/data/widget.json
+-rw-r--r--   0        0        0     4375 2023-02-16 15:37:39.000000 awkward-cpp-9/rapidjson/bin/draft-04/schema
+-rw-r--r--   0        0        0      368 2023-02-16 15:37:39.000000 awkward-cpp-9/rapidjson/bin/encodings/utf16be.json
+-rw-r--r--   0        0        0      370 2023-02-16 15:37:39.000000 awkward-cpp-9/rapidjson/bin/encodings/utf16bebom.json
+-rw-r--r--   0        0        0      368 2023-02-16 15:37:39.000000 awkward-cpp-9/rapidjson/bin/encodings/utf16le.json
+-rw-r--r--   0        0        0      370 2023-02-16 15:37:39.000000 awkward-cpp-9/rapidjson/bin/encodings/utf16lebom.json
+-rw-r--r--   0        0        0      736 2023-02-16 15:37:39.000000 awkward-cpp-9/rapidjson/bin/encodings/utf32be.json
+-rw-r--r--   0        0        0      740 2023-02-16 15:37:39.000000 awkward-cpp-9/rapidjson/bin/encodings/utf32bebom.json
+-rw-r--r--   0        0        0      736 2023-02-16 15:37:39.000000 awkward-cpp-9/rapidjson/bin/encodings/utf32le.json
+-rw-r--r--   0        0        0      740 2023-02-16 15:37:39.000000 awkward-cpp-9/rapidjson/bin/encodings/utf32lebom.json
+-rw-r--r--   0        0        0      322 2023-02-16 15:37:39.000000 awkward-cpp-9/rapidjson/bin/encodings/utf8.json
+-rw-r--r--   0        0        0      325 2023-02-16 15:37:39.000000 awkward-cpp-9/rapidjson/bin/encodings/utf8bom.json
+-rw-r--r--   0        0        0       60 2023-02-16 15:37:39.000000 awkward-cpp-9/rapidjson/bin/jsonchecker/fail1.json
+-rw-r--r--   0        0        0       58 2023-02-16 15:37:39.000000 awkward-cpp-9/rapidjson/bin/jsonchecker/fail10.json
+-rw-r--r--   0        0        0       29 2023-02-16 15:37:39.000000 awkward-cpp-9/rapidjson/bin/jsonchecker/fail11.json
+-rw-r--r--   0        0        0       31 2023-02-16 15:37:39.000000 awkward-cpp-9/rapidjson/bin/jsonchecker/fail12.json
+-rw-r--r--   0        0        0       43 2023-02-16 15:37:39.000000 awkward-cpp-9/rapidjson/bin/jsonchecker/fail13.json
+-rw-r--r--   0        0        0       31 2023-02-16 15:37:39.000000 awkward-cpp-9/rapidjson/bin/jsonchecker/fail14.json
+-rw-r--r--   0        0        0       34 2023-02-16 15:37:39.000000 awkward-cpp-9/rapidjson/bin/jsonchecker/fail15.json
+-rw-r--r--   0        0        0        8 2023-02-16 15:37:39.000000 awkward-cpp-9/rapidjson/bin/jsonchecker/fail16.json
+-rw-r--r--   0        0        0       34 2023-02-16 15:37:39.000000 awkward-cpp-9/rapidjson/bin/jsonchecker/fail17.json
+-rw-r--r--   0        0        0       50 2023-02-16 15:37:39.000000 awkward-cpp-9/rapidjson/bin/jsonchecker/fail18.json
+-rw-r--r--   0        0        0       22 2023-02-16 15:37:39.000000 awkward-cpp-9/rapidjson/bin/jsonchecker/fail19.json
+-rw-r--r--   0        0        0       17 2023-02-16 15:37:39.000000 awkward-cpp-9/rapidjson/bin/jsonchecker/fail2.json
+-rw-r--r--   0        0        0       23 2023-02-16 15:37:39.000000 awkward-cpp-9/rapidjson/bin/jsonchecker/fail20.json
+-rw-r--r--   0        0        0       32 2023-02-16 15:37:39.000000 awkward-cpp-9/rapidjson/bin/jsonchecker/fail21.json
+-rw-r--r--   0        0        0       33 2023-02-16 15:37:39.000000 awkward-cpp-9/rapidjson/bin/jsonchecker/fail22.json
+-rw-r--r--   0        0        0       20 2023-02-16 15:37:39.000000 awkward-cpp-9/rapidjson/bin/jsonchecker/fail23.json
+-rw-r--r--   0        0        0       16 2023-02-16 15:37:39.000000 awkward-cpp-9/rapidjson/bin/jsonchecker/fail24.json
+-rw-r--r--   0        0        0       29 2023-02-16 15:37:39.000000 awkward-cpp-9/rapidjson/bin/jsonchecker/fail25.json
+-rw-r--r--   0        0        0       38 2023-02-16 15:37:39.000000 awkward-cpp-9/rapidjson/bin/jsonchecker/fail26.json
+-rw-r--r--   0        0        0       14 2023-02-16 15:37:39.000000 awkward-cpp-9/rapidjson/bin/jsonchecker/fail27.json
+-rw-r--r--   0        0        0       15 2023-02-16 15:37:39.000000 awkward-cpp-9/rapidjson/bin/jsonchecker/fail28.json
+-rw-r--r--   0        0        0        4 2023-02-16 15:37:39.000000 awkward-cpp-9/rapidjson/bin/jsonchecker/fail29.json
+-rw-r--r--   0        0        0       37 2023-02-16 15:37:39.000000 awkward-cpp-9/rapidjson/bin/jsonchecker/fail3.json
+-rw-r--r--   0        0        0        5 2023-02-16 15:37:39.000000 awkward-cpp-9/rapidjson/bin/jsonchecker/fail30.json
+-rw-r--r--   0        0        0        7 2023-02-16 15:37:39.000000 awkward-cpp-9/rapidjson/bin/jsonchecker/fail31.json
+-rw-r--r--   0        0        0       40 2023-02-16 15:37:39.000000 awkward-cpp-9/rapidjson/bin/jsonchecker/fail32.json
+-rw-r--r--   0        0        0       12 2023-02-16 15:37:39.000000 awkward-cpp-9/rapidjson/bin/jsonchecker/fail33.json
+-rw-r--r--   0        0        0       16 2023-02-16 15:37:39.000000 awkward-cpp-9/rapidjson/bin/jsonchecker/fail4.json
+-rw-r--r--   0        0        0       24 2023-02-16 15:37:39.000000 awkward-cpp-9/rapidjson/bin/jsonchecker/fail5.json
+-rw-r--r--   0        0        0       26 2023-02-16 15:37:39.000000 awkward-cpp-9/rapidjson/bin/jsonchecker/fail6.json
+-rw-r--r--   0        0        0       26 2023-02-16 15:37:39.000000 awkward-cpp-9/rapidjson/bin/jsonchecker/fail7.json
+-rw-r--r--   0        0        0       16 2023-02-16 15:37:39.000000 awkward-cpp-9/rapidjson/bin/jsonchecker/fail8.json
+-rw-r--r--   0        0        0       22 2023-02-16 15:37:39.000000 awkward-cpp-9/rapidjson/bin/jsonchecker/fail9.json
+-rw-r--r--   0        0        0     1441 2023-02-16 15:37:39.000000 awkward-cpp-9/rapidjson/bin/jsonchecker/pass1.json
+-rw-r--r--   0        0        0       52 2023-02-16 15:37:39.000000 awkward-cpp-9/rapidjson/bin/jsonchecker/pass2.json
+-rw-r--r--   0        0        0      148 2023-02-16 15:37:39.000000 awkward-cpp-9/rapidjson/bin/jsonchecker/pass3.json
+-rw-r--r--   0        0        0      173 2023-02-16 15:37:39.000000 awkward-cpp-9/rapidjson/bin/jsonchecker/readme.txt
+-rw-r--r--   0        0        0        5 2023-02-16 15:37:39.000000 awkward-cpp-9/rapidjson/bin/jsonschema/.gitignore
+-rw-r--r--   0        0        0       98 2023-02-16 15:37:39.000000 awkward-cpp-9/rapidjson/bin/jsonschema/.travis.yml
+-rw-r--r--   0        0        0     1057 2023-02-16 15:37:39.000000 awkward-cpp-9/rapidjson/bin/jsonschema/LICENSE
+-rw-r--r--   0        0        0     4787 2023-02-16 15:37:39.000000 awkward-cpp-9/rapidjson/bin/jsonschema/README.md
+-rwxr-xr-x   0        0        0     9059 2023-02-16 15:37:39.000000 awkward-cpp-9/rapidjson/bin/jsonschema/bin/jsonschema_suite
+-rw-r--r--   0        0        0     6148 2023-02-16 15:37:39.000000 awkward-cpp-9/rapidjson/bin/jsonschema/remotes/.DS_Store
+-rw-r--r--   0        0        0       25 2023-02-16 15:37:39.000000 awkward-cpp-9/rapidjson/bin/jsonschema/remotes/folder/folderInteger.json
+-rw-r--r--   0        0        0       25 2023-02-16 15:37:39.000000 awkward-cpp-9/rapidjson/bin/jsonschema/remotes/integer.json
+-rw-r--r--   0        0        0      110 2023-02-16 15:37:39.000000 awkward-cpp-9/rapidjson/bin/jsonschema/remotes/subSchemas.json
+-rw-r--r--   0        0        0     6148 2023-02-16 15:37:39.000000 awkward-cpp-9/rapidjson/bin/jsonschema/tests/.DS_Store
+-rw-r--r--   0        0        0     2257 2023-02-16 15:37:39.000000 awkward-cpp-9/rapidjson/bin/jsonschema/tests/draft3/additionalItems.json
+-rw-r--r--   0        0        0     2745 2023-02-16 15:37:39.000000 awkward-cpp-9/rapidjson/bin/jsonschema/tests/draft3/additionalProperties.json
+-rw-r--r--   0        0        0     1273 2023-02-16 15:37:39.000000 awkward-cpp-9/rapidjson/bin/jsonschema/tests/draft3/default.json
+-rw-r--r--   0        0        0     2989 2023-02-16 15:37:39.000000 awkward-cpp-9/rapidjson/bin/jsonschema/tests/draft3/dependencies.json
+-rw-r--r--   0        0        0     1936 2023-02-16 15:37:39.000000 awkward-cpp-9/rapidjson/bin/jsonschema/tests/draft3/disallow.json
+-rw-r--r--   0        0        0     1544 2023-02-16 15:37:39.000000 awkward-cpp-9/rapidjson/bin/jsonschema/tests/draft3/divisibleBy.json
+-rw-r--r--   0        0        0     1964 2023-02-16 15:37:39.000000 awkward-cpp-9/rapidjson/bin/jsonschema/tests/draft3/enum.json
+-rw-r--r--   0        0        0     2591 2023-02-16 15:37:39.000000 awkward-cpp-9/rapidjson/bin/jsonschema/tests/draft3/extends.json
+-rw-r--r--   0        0        0     1136 2023-02-16 15:37:39.000000 awkward-cpp-9/rapidjson/bin/jsonschema/tests/draft3/items.json
+-rw-r--r--   0        0        0      706 2023-02-16 15:37:39.000000 awkward-cpp-9/rapidjson/bin/jsonschema/tests/draft3/maxItems.json
+-rw-r--r--   0        0        0      895 2023-02-16 15:37:39.000000 awkward-cpp-9/rapidjson/bin/jsonschema/tests/draft3/maxLength.json
+-rw-r--r--   0        0        0     1063 2023-02-16 15:37:39.000000 awkward-cpp-9/rapidjson/bin/jsonschema/tests/draft3/maximum.json
+-rw-r--r--   0        0        0      693 2023-02-16 15:37:39.000000 awkward-cpp-9/rapidjson/bin/jsonschema/tests/draft3/minItems.json
+-rw-r--r--   0        0        0      886 2023-02-16 15:37:39.000000 awkward-cpp-9/rapidjson/bin/jsonschema/tests/draft3/minLength.json
+-rw-r--r--   0        0        0     1063 2023-02-16 15:37:39.000000 awkward-cpp-9/rapidjson/bin/jsonschema/tests/draft3/minimum.json
+-rw-r--r--   0        0        0     3075 2023-02-16 15:37:39.000000 awkward-cpp-9/rapidjson/bin/jsonschema/tests/draft3/optional/bignum.json
+-rw-r--r--   0        0        0     6751 2023-02-16 15:37:39.000000 awkward-cpp-9/rapidjson/bin/jsonschema/tests/draft3/optional/format.json
+-rw-r--r--   0        0        0      463 2023-02-16 15:37:39.000000 awkward-cpp-9/rapidjson/bin/jsonschema/tests/draft3/optional/jsregex.json
+-rw-r--r--   0        0        0      384 2023-02-16 15:37:39.000000 awkward-cpp-9/rapidjson/bin/jsonschema/tests/draft3/optional/zeroTerminatedFloats.json
+-rw-r--r--   0        0        0      857 2023-02-16 15:37:39.000000 awkward-cpp-9/rapidjson/bin/jsonschema/tests/draft3/pattern.json
+-rw-r--r--   0        0        0     3365 2023-02-16 15:37:39.000000 awkward-cpp-9/rapidjson/bin/jsonschema/tests/draft3/patternProperties.json
+-rw-r--r--   0        0        0     2881 2023-02-16 15:37:39.000000 awkward-cpp-9/rapidjson/bin/jsonschema/tests/draft3/properties.json
+-rw-r--r--   0        0        0     4385 2023-02-16 15:37:39.000000 awkward-cpp-9/rapidjson/bin/jsonschema/tests/draft3/ref.json
+-rw-r--r--   0        0        0     1961 2023-02-16 15:37:39.000000 awkward-cpp-9/rapidjson/bin/jsonschema/tests/draft3/refRemote.json
+-rw-r--r--   0        0        0     1282 2023-02-16 15:37:39.000000 awkward-cpp-9/rapidjson/bin/jsonschema/tests/draft3/required.json
+-rw-r--r--   0        0        0    13217 2023-02-16 15:37:39.000000 awkward-cpp-9/rapidjson/bin/jsonschema/tests/draft3/type.json
+-rw-r--r--   0        0        0     2613 2023-02-16 15:37:39.000000 awkward-cpp-9/rapidjson/bin/jsonschema/tests/draft3/uniqueItems.json
+-rw-r--r--   0        0        0     6148 2023-02-16 15:37:39.000000 awkward-cpp-9/rapidjson/bin/jsonschema/tests/draft4/.DS_Store
+-rw-r--r--   0        0        0     2282 2023-02-16 15:37:39.000000 awkward-cpp-9/rapidjson/bin/jsonschema/tests/draft4/additionalItems.json
+-rw-r--r--   0        0        0     2745 2023-02-16 15:37:39.000000 awkward-cpp-9/rapidjson/bin/jsonschema/tests/draft4/additionalProperties.json
+-rw-r--r--   0        0        0     3025 2023-02-16 15:37:39.000000 awkward-cpp-9/rapidjson/bin/jsonschema/tests/draft4/allOf.json
+-rw-r--r--   0        0        0     1608 2023-02-16 15:37:39.000000 awkward-cpp-9/rapidjson/bin/jsonschema/tests/draft4/anyOf.json
+-rw-r--r--   0        0        0     1273 2023-02-16 15:37:39.000000 awkward-cpp-9/rapidjson/bin/jsonschema/tests/draft4/default.json
+-rw-r--r--   0        0        0      854 2023-02-16 15:37:39.000000 awkward-cpp-9/rapidjson/bin/jsonschema/tests/draft4/definitions.json
+-rw-r--r--   0        0        0     3139 2023-02-16 15:37:39.000000 awkward-cpp-9/rapidjson/bin/jsonschema/tests/draft4/dependencies.json
+-rw-r--r--   0        0        0     1975 2023-02-16 15:37:39.000000 awkward-cpp-9/rapidjson/bin/jsonschema/tests/draft4/enum.json
+-rw-r--r--   0        0        0     1136 2023-02-16 15:37:39.000000 awkward-cpp-9/rapidjson/bin/jsonschema/tests/draft4/items.json
+-rw-r--r--   0        0        0      706 2023-02-16 15:37:39.000000 awkward-cpp-9/rapidjson/bin/jsonschema/tests/draft4/maxItems.json
+-rw-r--r--   0        0        0      896 2023-02-16 15:37:39.000000 awkward-cpp-9/rapidjson/bin/jsonschema/tests/draft4/maxLength.json
+-rw-r--r--   0        0        0      759 2023-02-16 15:37:39.000000 awkward-cpp-9/rapidjson/bin/jsonschema/tests/draft4/maxProperties.json
+-rw-r--r--   0        0        0     1063 2023-02-16 15:37:39.000000 awkward-cpp-9/rapidjson/bin/jsonschema/tests/draft4/maximum.json
+-rw-r--r--   0        0        0      693 2023-02-16 15:37:39.000000 awkward-cpp-9/rapidjson/bin/jsonschema/tests/draft4/minItems.json
+-rw-r--r--   0        0        0      886 2023-02-16 15:37:39.000000 awkward-cpp-9/rapidjson/bin/jsonschema/tests/draft4/minLength.json
+-rw-r--r--   0        0        0      725 2023-02-16 15:37:39.000000 awkward-cpp-9/rapidjson/bin/jsonschema/tests/draft4/minProperties.json
+-rw-r--r--   0        0        0     1063 2023-02-16 15:37:39.000000 awkward-cpp-9/rapidjson/bin/jsonschema/tests/draft4/minimum.json
+-rw-r--r--   0        0        0     1525 2023-02-16 15:37:39.000000 awkward-cpp-9/rapidjson/bin/jsonschema/tests/draft4/multipleOf.json
+-rw-r--r--   0        0        0     2266 2023-02-16 15:37:39.000000 awkward-cpp-9/rapidjson/bin/jsonschema/tests/draft4/not.json
+-rw-r--r--   0        0        0     1607 2023-02-16 15:37:39.000000 awkward-cpp-9/rapidjson/bin/jsonschema/tests/draft4/oneOf.json
+-rw-r--r--   0        0        0     3075 2023-02-16 15:37:39.000000 awkward-cpp-9/rapidjson/bin/jsonschema/tests/draft4/optional/bignum.json
+-rw-r--r--   0        0        0     4608 2023-02-16 15:37:39.000000 awkward-cpp-9/rapidjson/bin/jsonschema/tests/draft4/optional/format.json
+-rw-r--r--   0        0        0      384 2023-02-16 15:37:39.000000 awkward-cpp-9/rapidjson/bin/jsonschema/tests/draft4/optional/zeroTerminatedFloats.json
+-rw-r--r--   0        0        0      857 2023-02-16 15:37:39.000000 awkward-cpp-9/rapidjson/bin/jsonschema/tests/draft4/pattern.json
+-rw-r--r--   0        0        0     3365 2023-02-16 15:37:39.000000 awkward-cpp-9/rapidjson/bin/jsonschema/tests/draft4/patternProperties.json
+-rw-r--r--   0        0        0     2881 2023-02-16 15:37:39.000000 awkward-cpp-9/rapidjson/bin/jsonschema/tests/draft4/properties.json
+-rw-r--r--   0        0        0     4366 2023-02-16 15:37:39.000000 awkward-cpp-9/rapidjson/bin/jsonschema/tests/draft4/ref.json
+-rw-r--r--   0        0        0     1961 2023-02-16 15:37:39.000000 awkward-cpp-9/rapidjson/bin/jsonschema/tests/draft4/refRemote.json
+-rw-r--r--   0        0        0      923 2023-02-16 15:37:39.000000 awkward-cpp-9/rapidjson/bin/jsonschema/tests/draft4/required.json
+-rw-r--r--   0        0        0     9298 2023-02-16 15:37:39.000000 awkward-cpp-9/rapidjson/bin/jsonschema/tests/draft4/type.json
+-rw-r--r--   0        0        0     2613 2023-02-16 15:37:39.000000 awkward-cpp-9/rapidjson/bin/jsonschema/tests/draft4/uniqueItems.json
+-rw-r--r--   0        0        0      134 2023-02-16 15:37:39.000000 awkward-cpp-9/rapidjson/bin/jsonschema/tox.ini
+-rwxr-xr-x   0        0        0      849 2023-02-16 15:37:39.000000 awkward-cpp-9/rapidjson/bin/types/booleans.json
+-rwxr-xr-x   0        0        0     1698 2023-02-16 15:37:39.000000 awkward-cpp-9/rapidjson/bin/types/floats.json
+-rwxr-xr-x   0        0        0     4202 2023-02-16 15:37:39.000000 awkward-cpp-9/rapidjson/bin/types/guids.json
+-rwxr-xr-x   0        0        0     1098 2023-02-16 15:37:39.000000 awkward-cpp-9/rapidjson/bin/types/integers.json
+-rwxr-xr-x   0        0        0    15142 2023-02-16 15:37:39.000000 awkward-cpp-9/rapidjson/bin/types/mixed.json
+-rwxr-xr-x   0        0        0      802 2023-02-16 15:37:39.000000 awkward-cpp-9/rapidjson/bin/types/nulls.json
+-rwxr-xr-x   0        0        0    33764 2023-02-16 15:37:39.000000 awkward-cpp-9/rapidjson/bin/types/paragraphs.json
+-rw-r--r--   0        0        0       86 2023-02-16 15:37:39.000000 awkward-cpp-9/rapidjson/bin/types/readme.txt
+-rw-r--r--   0        0        0     1009 2023-02-16 15:37:39.000000 awkward-cpp-9/rapidjson/doc/CMakeLists.txt
+-rw-r--r--   0        0        0   103392 2023-02-16 15:37:39.000000 awkward-cpp-9/rapidjson/doc/Doxyfile.in
+-rw-r--r--   0        0        0   103471 2023-02-16 15:37:39.000000 awkward-cpp-9/rapidjson/doc/Doxyfile.zh-cn.in
+-rw-r--r--   0        0        0      912 2023-02-16 15:37:39.000000 awkward-cpp-9/rapidjson/doc/diagram/architecture.dot
+-rw-r--r--   0        0        0    16569 2023-02-16 15:37:39.000000 awkward-cpp-9/rapidjson/doc/diagram/architecture.png
+-rw-r--r--   0        0        0     2239 2023-02-16 15:37:39.000000 awkward-cpp-9/rapidjson/doc/diagram/insituparsing.dot
+-rw-r--r--   0        0        0    37281 2023-02-16 15:37:39.000000 awkward-cpp-9/rapidjson/doc/diagram/insituparsing.png
+-rw-r--r--   0        0        0     1915 2023-02-16 15:37:39.000000 awkward-cpp-9/rapidjson/doc/diagram/iterative-parser-states-diagram.dot
+-rw-r--r--   0        0        0    92378 2023-02-16 15:37:39.000000 awkward-cpp-9/rapidjson/doc/diagram/iterative-parser-states-diagram.png
+-rw-r--r--   0        0        0      176 2023-02-16 15:37:39.000000 awkward-cpp-9/rapidjson/doc/diagram/makefile
+-rw-r--r--   0        0        0      935 2023-02-16 15:37:39.000000 awkward-cpp-9/rapidjson/doc/diagram/move1.dot
+-rw-r--r--   0        0        0    16081 2023-02-16 15:37:39.000000 awkward-cpp-9/rapidjson/doc/diagram/move1.png
+-rw-r--r--   0        0        0     1498 2023-02-16 15:37:39.000000 awkward-cpp-9/rapidjson/doc/diagram/move2.dot
+-rw-r--r--   0        0        0    41517 2023-02-16 15:37:39.000000 awkward-cpp-9/rapidjson/doc/diagram/move2.png
+-rw-r--r--   0        0        0     1450 2023-02-16 15:37:39.000000 awkward-cpp-9/rapidjson/doc/diagram/move3.dot
+-rw-r--r--   0        0        0    36371 2023-02-16 15:37:39.000000 awkward-cpp-9/rapidjson/doc/diagram/move3.png
+-rw-r--r--   0        0        0     1427 2023-02-16 15:37:39.000000 awkward-cpp-9/rapidjson/doc/diagram/normalparsing.dot
+-rw-r--r--   0        0        0    32887 2023-02-16 15:37:39.000000 awkward-cpp-9/rapidjson/doc/diagram/normalparsing.png
+-rw-r--r--   0        0        0     1435 2023-02-16 15:37:39.000000 awkward-cpp-9/rapidjson/doc/diagram/simpledom.dot
+-rw-r--r--   0        0        0    43670 2023-02-16 15:37:39.000000 awkward-cpp-9/rapidjson/doc/diagram/simpledom.png
+-rw-r--r--   0        0        0     1456 2023-02-16 15:37:39.000000 awkward-cpp-9/rapidjson/doc/diagram/tutorial.dot
+-rw-r--r--   0        0        0    44634 2023-02-16 15:37:39.000000 awkward-cpp-9/rapidjson/doc/diagram/tutorial.png
+-rw-r--r--   0        0        0     1775 2023-02-16 15:37:39.000000 awkward-cpp-9/rapidjson/doc/diagram/utilityclass.dot
+-rw-r--r--   0        0        0    99993 2023-02-16 15:37:39.000000 awkward-cpp-9/rapidjson/doc/diagram/utilityclass.png
+-rw-r--r--   0        0        0    15369 2023-02-16 15:37:39.000000 awkward-cpp-9/rapidjson/doc/dom.md
+-rw-r--r--   0        0        0    15294 2023-02-16 15:37:39.000000 awkward-cpp-9/rapidjson/doc/dom.zh-cn.md
+-rw-r--r--   0        0        0     6709 2023-02-16 15:37:39.000000 awkward-cpp-9/rapidjson/doc/encoding.md
+-rw-r--r--   0        0        0     6860 2023-02-16 15:37:39.000000 awkward-cpp-9/rapidjson/doc/encoding.zh-cn.md
+-rw-r--r--   0        0        0    15285 2023-02-16 15:37:39.000000 awkward-cpp-9/rapidjson/doc/faq.md
+-rw-r--r--   0        0        0    14947 2023-02-16 15:37:39.000000 awkward-cpp-9/rapidjson/doc/faq.zh-cn.md
+-rw-r--r--   0        0        0     5005 2023-02-16 15:37:39.000000 awkward-cpp-9/rapidjson/doc/features.md
+-rw-r--r--   0        0        0     4804 2023-02-16 15:37:39.000000 awkward-cpp-9/rapidjson/doc/features.zh-cn.md
+-rw-r--r--   0        0        0    22305 2023-02-16 15:37:39.000000 awkward-cpp-9/rapidjson/doc/internals.md
+-rw-r--r--   0        0        0     5259 2023-02-16 15:37:39.000000 awkward-cpp-9/rapidjson/doc/logo/rapidjson.png
+-rw-r--r--   0        0        0     4230 2023-02-16 15:37:39.000000 awkward-cpp-9/rapidjson/doc/logo/rapidjson.svg
+-rw-r--r--   0        0        0     6090 2023-02-16 15:37:39.000000 awkward-cpp-9/rapidjson/doc/misc/DoxygenLayout.xml
+-rw-r--r--   0        0        0     6572 2023-02-16 15:37:39.000000 awkward-cpp-9/rapidjson/doc/misc/doxygenextra.css
+-rw-r--r--   0        0        0      256 2023-02-16 15:37:39.000000 awkward-cpp-9/rapidjson/doc/misc/footer.html
+-rw-r--r--   0        0        0     1137 2023-02-16 15:37:39.000000 awkward-cpp-9/rapidjson/doc/misc/header.html
+-rw-r--r--   0        0        0      363 2023-02-16 15:37:39.000000 awkward-cpp-9/rapidjson/doc/npm.md
+-rw-r--r--   0        0        0     1267 2023-02-16 15:37:39.000000 awkward-cpp-9/rapidjson/doc/performance.md
+-rw-r--r--   0        0        0     1236 2023-02-16 15:37:39.000000 awkward-cpp-9/rapidjson/doc/performance.zh-cn.md
+-rw-r--r--   0        0        0     8882 2023-02-16 15:37:39.000000 awkward-cpp-9/rapidjson/doc/pointer.md
+-rw-r--r--   0        0        0     8532 2023-02-16 15:37:39.000000 awkward-cpp-9/rapidjson/doc/pointer.zh-cn.md
+-rw-r--r--   0        0        0    20432 2023-02-16 15:37:39.000000 awkward-cpp-9/rapidjson/doc/sax.md
+-rw-r--r--   0        0        0    19969 2023-02-16 15:37:39.000000 awkward-cpp-9/rapidjson/doc/sax.zh-cn.md
+-rw-r--r--   0        0        0     9963 2023-02-16 15:37:39.000000 awkward-cpp-9/rapidjson/doc/schema.md
+-rw-r--r--   0        0        0     9604 2023-02-16 15:37:39.000000 awkward-cpp-9/rapidjson/doc/schema.zh-cn.md
+-rw-r--r--   0        0        0    14398 2023-02-16 15:37:39.000000 awkward-cpp-9/rapidjson/doc/stream.md
+-rw-r--r--   0        0        0    14235 2023-02-16 15:37:39.000000 awkward-cpp-9/rapidjson/doc/stream.zh-cn.md
+-rw-r--r--   0        0        0    21947 2023-02-16 15:37:39.000000 awkward-cpp-9/rapidjson/doc/tutorial.md
+-rw-r--r--   0        0        0    21549 2023-02-16 15:37:39.000000 awkward-cpp-9/rapidjson/doc/tutorial.zh-cn.md
+-rw-r--r--   0        0        0      229 2023-02-16 15:37:39.000000 awkward-cpp-9/rapidjson/docker/debian/Dockerfile
+-rw-r--r--   0        0        0     1021 2023-02-16 15:37:39.000000 awkward-cpp-9/rapidjson/example/CMakeLists.txt
+-rw-r--r--   0        0        0     2577 2023-02-16 15:37:39.000000 awkward-cpp-9/rapidjson/example/capitalize/capitalize.cpp
+-rw-r--r--   0        0        0     1015 2023-02-16 15:37:39.000000 awkward-cpp-9/rapidjson/example/condense/condense.cpp
+-rw-r--r--   0        0        0     4979 2023-02-16 15:37:39.000000 awkward-cpp-9/rapidjson/example/filterkey/filterkey.cpp
+-rw-r--r--   0        0        0     5946 2023-02-16 15:37:39.000000 awkward-cpp-9/rapidjson/example/filterkeydom/filterkeydom.cpp
+-rw-r--r--   0        0        0     6022 2023-02-16 15:37:39.000000 awkward-cpp-9/rapidjson/example/jsonx/jsonx.cpp
+-rw-r--r--   0        0        0     2814 2023-02-16 15:37:39.000000 awkward-cpp-9/rapidjson/example/messagereader/messagereader.cpp
+-rw-r--r--   0        0        0     5026 2023-02-16 15:37:39.000000 awkward-cpp-9/rapidjson/example/parsebyparts/parsebyparts.cpp
+-rw-r--r--   0        0        0     1019 2023-02-16 15:37:39.000000 awkward-cpp-9/rapidjson/example/pretty/pretty.cpp
+-rw-r--r--   0        0        0     2245 2023-02-16 15:37:39.000000 awkward-cpp-9/rapidjson/example/prettyauto/prettyauto.cpp
+-rw-r--r--   0        0        0     2510 2023-02-16 15:37:39.000000 awkward-cpp-9/rapidjson/example/schemavalidator/schemavalidator.cpp
+-rw-r--r--   0        0        0     4590 2023-02-16 15:37:39.000000 awkward-cpp-9/rapidjson/example/serialize/serialize.cpp
+-rw-r--r--   0        0        0      685 2023-02-16 15:37:39.000000 awkward-cpp-9/rapidjson/example/simpledom/simpledom.cpp
+-rw-r--r--   0        0        0     1868 2023-02-16 15:37:39.000000 awkward-cpp-9/rapidjson/example/simplereader/simplereader.cpp
+-rw-r--r--   0        0        0     1031 2023-02-16 15:37:39.000000 awkward-cpp-9/rapidjson/example/simplewriter/simplewriter.cpp
+-rw-r--r--   0        0        0     6263 2023-02-16 15:37:39.000000 awkward-cpp-9/rapidjson/example/tutorial/tutorial.cpp
+-rw-r--r--   0        0        0    10311 2023-02-16 15:37:39.000000 awkward-cpp-9/rapidjson/include/rapidjson/allocators.h
+-rw-r--r--   0        0        0   113794 2023-02-16 15:37:39.000000 awkward-cpp-9/rapidjson/include/rapidjson/document.h
+-rw-r--r--   0        0        0    10686 2023-02-16 15:37:39.000000 awkward-cpp-9/rapidjson/include/rapidjson/encodedstream.h
+-rw-r--r--   0        0        0    28553 2023-02-16 15:37:39.000000 awkward-cpp-9/rapidjson/include/rapidjson/encodings.h
+-rw-r--r--   0        0        0     3870 2023-02-16 15:37:39.000000 awkward-cpp-9/rapidjson/include/rapidjson/error/en.h
+-rw-r--r--   0        0        0     5824 2023-02-16 15:37:39.000000 awkward-cpp-9/rapidjson/include/rapidjson/error/error.h
+-rw-r--r--   0        0        0     2988 2023-02-16 15:37:39.000000 awkward-cpp-9/rapidjson/include/rapidjson/filereadstream.h
+-rw-r--r--   0        0        0     3139 2023-02-16 15:37:39.000000 awkward-cpp-9/rapidjson/include/rapidjson/filewritestream.h
+-rw-r--r--   0        0        0     4035 2023-02-16 15:37:39.000000 awkward-cpp-9/rapidjson/include/rapidjson/fwd.h
+-rw-r--r--   0        0        0     9139 2023-02-16 15:37:39.000000 awkward-cpp-9/rapidjson/include/rapidjson/internal/biginteger.h
+-rw-r--r--   0        0        0    11512 2023-02-16 15:37:39.000000 awkward-cpp-9/rapidjson/include/rapidjson/internal/diyfp.h
+-rw-r--r--   0        0        0     8172 2023-02-16 15:37:39.000000 awkward-cpp-9/rapidjson/include/rapidjson/internal/dtoa.h
+-rw-r--r--   0        0        0     3022 2023-02-16 15:37:39.000000 awkward-cpp-9/rapidjson/include/rapidjson/internal/ieee754.h
+-rw-r--r--   0        0        0    10306 2023-02-16 15:37:39.000000 awkward-cpp-9/rapidjson/include/rapidjson/internal/itoa.h
+-rw-r--r--   0        0        0     6572 2023-02-16 15:37:39.000000 awkward-cpp-9/rapidjson/include/rapidjson/internal/meta.h
+-rw-r--r--   0        0        0     3595 2023-02-16 15:37:39.000000 awkward-cpp-9/rapidjson/include/rapidjson/internal/pow10.h
+-rw-r--r--   0        0        0    24825 2023-02-16 15:37:39.000000 awkward-cpp-9/rapidjson/include/rapidjson/internal/regex.h
+-rw-r--r--   0        0        0     7026 2023-02-16 15:37:39.000000 awkward-cpp-9/rapidjson/include/rapidjson/internal/stack.h
+-rw-r--r--   0        0        0     1897 2023-02-16 15:37:39.000000 awkward-cpp-9/rapidjson/include/rapidjson/internal/strfunc.h
+-rw-r--r--   0        0        0     8672 2023-02-16 15:37:39.000000 awkward-cpp-9/rapidjson/include/rapidjson/internal/strtod.h
+-rw-r--r--   0        0        0     1419 2023-02-16 15:37:39.000000 awkward-cpp-9/rapidjson/include/rapidjson/internal/swap.h
+-rw-r--r--   0        0        0     3576 2023-02-16 15:37:39.000000 awkward-cpp-9/rapidjson/include/rapidjson/istreamwrapper.h
+-rw-r--r--   0        0        0     2560 2023-02-16 15:37:39.000000 awkward-cpp-9/rapidjson/include/rapidjson/memorybuffer.h
+-rw-r--r--   0        0        0     2667 2023-02-16 15:37:39.000000 awkward-cpp-9/rapidjson/include/rapidjson/memorystream.h
+-rw-r--r--   0        0        0     8372 2023-02-16 15:37:39.000000 awkward-cpp-9/rapidjson/include/rapidjson/msinttypes/inttypes.h
+-rw-r--r--   0        0        0     9386 2023-02-16 15:37:39.000000 awkward-cpp-9/rapidjson/include/rapidjson/msinttypes/stdint.h
+-rw-r--r--   0        0        0     2331 2023-02-16 15:37:39.000000 awkward-cpp-9/rapidjson/include/rapidjson/ostreamwrapper.h
+-rw-r--r--   0        0        0    58465 2023-02-16 15:37:39.000000 awkward-cpp-9/rapidjson/include/rapidjson/pointer.h
+-rw-r--r--   0        0        0     9601 2023-02-16 15:37:39.000000 awkward-cpp-9/rapidjson/include/rapidjson/prettywriter.h
+-rw-r--r--   0        0        0    21461 2023-02-16 15:37:39.000000 awkward-cpp-9/rapidjson/include/rapidjson/rapidjson.h
+-rw-r--r--   0        0        0    79760 2023-02-16 15:37:39.000000 awkward-cpp-9/rapidjson/include/rapidjson/reader.h
+-rw-r--r--   0        0        0    80014 2023-02-16 15:37:39.000000 awkward-cpp-9/rapidjson/include/rapidjson/schema.h
+-rw-r--r--   0        0        0     5466 2023-02-16 15:37:39.000000 awkward-cpp-9/rapidjson/include/rapidjson/stream.h
+-rw-r--r--   0        0        0     3798 2023-02-16 15:37:39.000000 awkward-cpp-9/rapidjson/include/rapidjson/stringbuffer.h
+-rw-r--r--   0        0        0    23261 2023-02-16 15:37:39.000000 awkward-cpp-9/rapidjson/include/rapidjson/writer.h
+-rw-r--r--   0        0        0       94 2023-02-16 15:37:39.000000 awkward-cpp-9/rapidjson/include_dirs.js
+-rw-r--r--   0        0        0      313 2023-02-16 15:37:39.000000 awkward-cpp-9/rapidjson/library.json
+-rw-r--r--   0        0        0     5152 2023-02-16 15:37:39.000000 awkward-cpp-9/rapidjson/license.txt
+-rw-r--r--   0        0        0      561 2023-02-16 15:37:39.000000 awkward-cpp-9/rapidjson/package.json
+-rw-r--r--   0        0        0     3286 2023-02-16 15:37:39.000000 awkward-cpp-9/rapidjson/rapidjson.autopkg
+-rw-r--r--   0        0        0     8913 2023-02-16 15:37:39.000000 awkward-cpp-9/rapidjson/readme.md
+-rw-r--r--   0        0        0     8704 2023-02-16 15:37:39.000000 awkward-cpp-9/rapidjson/readme.zh-cn.md
+-rw-r--r--   0        0        0      491 2023-02-16 15:37:39.000000 awkward-cpp-9/rapidjson/test/CMakeLists.txt
+-rw-r--r--   0        0        0      765 2023-02-16 15:37:39.000000 awkward-cpp-9/rapidjson/test/perftest/CMakeLists.txt
+-rw-r--r--   0        0        0    35486 2023-02-16 15:37:39.000000 awkward-cpp-9/rapidjson/test/perftest/misctest.cpp
+-rw-r--r--   0        0        0      996 2023-02-16 15:37:39.000000 awkward-cpp-9/rapidjson/test/perftest/perftest.cpp
+-rw-r--r--   0        0        0     5643 2023-02-16 15:37:39.000000 awkward-cpp-9/rapidjson/test/perftest/perftest.h
+-rw-r--r--   0        0        0     4476 2023-02-16 15:37:39.000000 awkward-cpp-9/rapidjson/test/perftest/platformtest.cpp
+-rw-r--r--   0        0        0    12440 2023-02-16 15:37:39.000000 awkward-cpp-9/rapidjson/test/perftest/rapidjsontest.cpp
+-rw-r--r--   0        0        0     7095 2023-02-16 15:37:39.000000 awkward-cpp-9/rapidjson/test/perftest/schematest.cpp
+-rw-r--r--   0        0        0     3156 2023-02-16 15:37:39.000000 awkward-cpp-9/rapidjson/test/unittest/CMakeLists.txt
+-rw-r--r--   0        0        0     3308 2023-02-16 15:37:39.000000 awkward-cpp-9/rapidjson/test/unittest/allocatorstest.cpp
+-rw-r--r--   0        0        0     4221 2023-02-16 15:37:39.000000 awkward-cpp-9/rapidjson/test/unittest/bigintegertest.cpp
+-rw-r--r--   0        0        0    20694 2023-02-16 15:37:39.000000 awkward-cpp-9/rapidjson/test/unittest/documenttest.cpp
+-rw-r--r--   0        0        0     3403 2023-02-16 15:37:39.000000 awkward-cpp-9/rapidjson/test/unittest/dtoatest.cpp
+-rw-r--r--   0        0        0    12025 2023-02-16 15:37:39.000000 awkward-cpp-9/rapidjson/test/unittest/encodedstreamtest.cpp
+-rw-r--r--   0        0        0    19364 2023-02-16 15:37:39.000000 awkward-cpp-9/rapidjson/test/unittest/encodingstest.cpp
+-rw-r--r--   0        0        0     3218 2023-02-16 15:37:39.000000 awkward-cpp-9/rapidjson/test/unittest/filestreamtest.cpp
+-rw-r--r--   0        0        0     5744 2023-02-16 15:37:39.000000 awkward-cpp-9/rapidjson/test/unittest/fwdtest.cpp
+-rw-r--r--   0        0        0     5373 2023-02-16 15:37:39.000000 awkward-cpp-9/rapidjson/test/unittest/istreamwrappertest.cpp
+-rw-r--r--   0        0        0     3966 2023-02-16 15:37:39.000000 awkward-cpp-9/rapidjson/test/unittest/itoatest.cpp
+-rw-r--r--   0        0        0     3178 2023-02-16 15:37:39.000000 awkward-cpp-9/rapidjson/test/unittest/jsoncheckertest.cpp
+-rw-r--r--   0        0        0     2422 2023-02-16 15:37:39.000000 awkward-cpp-9/rapidjson/test/unittest/namespacetest.cpp
+-rw-r--r--   0        0        0     2459 2023-02-16 15:37:39.000000 awkward-cpp-9/rapidjson/test/unittest/ostreamwrappertest.cpp
+-rw-r--r--   0        0        0    55407 2023-02-16 15:37:39.000000 awkward-cpp-9/rapidjson/test/unittest/pointertest.cpp
+-rw-r--r--   0        0        0     5766 2023-02-16 15:37:39.000000 awkward-cpp-9/rapidjson/test/unittest/prettywritertest.cpp
+-rw-r--r--   0        0        0    70515 2023-02-16 15:37:39.000000 awkward-cpp-9/rapidjson/test/unittest/readertest.cpp
+-rw-r--r--   0        0        0    16157 2023-02-16 15:37:39.000000 awkward-cpp-9/rapidjson/test/unittest/regextest.cpp
+-rw-r--r--   0        0        0    47377 2023-02-16 15:37:39.000000 awkward-cpp-9/rapidjson/test/unittest/schematest.cpp
+-rw-r--r--   0        0        0     6920 2023-02-16 15:37:39.000000 awkward-cpp-9/rapidjson/test/unittest/simdtest.cpp
+-rw-r--r--   0        0        0     1337 2023-02-16 15:37:39.000000 awkward-cpp-9/rapidjson/test/unittest/strfunctest.cpp
+-rw-r--r--   0        0        0     4834 2023-02-16 15:37:39.000000 awkward-cpp-9/rapidjson/test/unittest/stringbuffertest.cpp
+-rw-r--r--   0        0        0     4273 2023-02-16 15:37:39.000000 awkward-cpp-9/rapidjson/test/unittest/strtodtest.cpp
+-rw-r--r--   0        0        0     1548 2023-02-16 15:37:39.000000 awkward-cpp-9/rapidjson/test/unittest/unittest.cpp
+-rw-r--r--   0        0        0     3766 2023-02-16 15:37:39.000000 awkward-cpp-9/rapidjson/test/unittest/unittest.h
+-rw-r--r--   0        0        0    54940 2023-02-16 15:37:39.000000 awkward-cpp-9/rapidjson/test/unittest/valuetest.cpp
+-rw-r--r--   0        0        0    14988 2023-02-16 15:37:39.000000 awkward-cpp-9/rapidjson/test/unittest/writertest.cpp
+-rwxr-xr-x   0        0        0     3247 2023-02-16 15:37:39.000000 awkward-cpp-9/rapidjson/travis-doxygen.sh
+-rw-r--r--   0        0        0       89 2023-02-16 15:37:39.000000 awkward-cpp-9/src/awkward_cpp/__init__.py
+-rw-r--r--   0        0        0   146654 2023-02-16 15:37:39.000000 awkward-cpp-9/src/awkward_cpp/_kernel_signatures.py
+-rw-r--r--   0        0        0      755 2023-02-16 15:37:39.000000 awkward-cpp-9/src/awkward_cpp/cpu_kernels.py
+-rw-r--r--   0        0        0     8701 2023-02-16 15:37:39.000000 awkward-cpp-9/src/awkward_cpp/libawkward.py
+-rw-r--r--   0        0        0     2033 2023-02-16 15:37:39.000000 awkward-cpp-9/src/cpu-kernels/awkward_BitMaskedArray_to_ByteMaskedArray.cpp
+-rw-r--r--   0        0        0     3614 2023-02-16 15:37:39.000000 awkward-cpp-9/src/cpu-kernels/awkward_BitMaskedArray_to_IndexedOptionArray.cpp
+-rw-r--r--   0        0        0      796 2023-02-16 15:37:39.000000 awkward-cpp-9/src/cpu-kernels/awkward_ByteMaskedArray_getitem_nextcarry.cpp
+-rw-r--r--   0        0        0      949 2023-02-16 15:37:39.000000 awkward-cpp-9/src/cpu-kernels/awkward_ByteMaskedArray_getitem_nextcarry_outindex.cpp
+-rw-r--r--   0        0        0      511 2023-02-16 15:37:39.000000 awkward-cpp-9/src/cpu-kernels/awkward_ByteMaskedArray_numnull.cpp
+-rw-r--r--   0        0        0      863 2023-02-16 15:37:39.000000 awkward-cpp-9/src/cpu-kernels/awkward_ByteMaskedArray_overlay_mask.cpp
+-rw-r--r--   0        0        0      702 2023-02-16 15:37:39.000000 awkward-cpp-9/src/cpu-kernels/awkward_ByteMaskedArray_reduce_next_64.cpp
+-rw-r--r--   0        0        0      646 2023-02-16 15:37:39.000000 awkward-cpp-9/src/cpu-kernels/awkward_ByteMaskedArray_reduce_next_nonlocal_nextshifts_64.cpp
+-rw-r--r--   0        0        0      705 2023-02-16 15:37:39.000000 awkward-cpp-9/src/cpu-kernels/awkward_ByteMaskedArray_reduce_next_nonlocal_nextshifts_fromshifts_64.cpp
+-rw-r--r--   0        0        0      769 2023-02-16 15:37:39.000000 awkward-cpp-9/src/cpu-kernels/awkward_ByteMaskedArray_toIndexedOptionArray.cpp
+-rw-r--r--   0        0        0      757 2023-02-16 15:37:39.000000 awkward-cpp-9/src/cpu-kernels/awkward_Content_getitem_next_missing_jagged_getmaskstartstop.cpp
+-rw-r--r--   0        0        0      744 2023-02-16 15:37:39.000000 awkward-cpp-9/src/cpu-kernels/awkward_Index_nones_as_index.cpp
+-rw-r--r--   0        0        0     1416 2023-02-16 15:37:39.000000 awkward-cpp-9/src/cpu-kernels/awkward_IndexedArray_fill.cpp
+-rw-r--r--   0        0        0      705 2023-02-16 15:37:39.000000 awkward-cpp-9/src/cpu-kernels/awkward_IndexedArray_fill_count.cpp
+-rw-r--r--   0        0        0     1491 2023-02-16 15:37:39.000000 awkward-cpp-9/src/cpu-kernels/awkward_IndexedArray_flatten_nextcarry.cpp
+-rw-r--r--   0        0        0     1934 2023-02-16 15:37:39.000000 awkward-cpp-9/src/cpu-kernels/awkward_IndexedArray_flatten_none2empty.cpp
+-rw-r--r--   0        0        0     1490 2023-02-16 15:37:39.000000 awkward-cpp-9/src/cpu-kernels/awkward_IndexedArray_getitem_nextcarry.cpp
+-rw-r--r--   0        0        0     1741 2023-02-16 15:37:39.000000 awkward-cpp-9/src/cpu-kernels/awkward_IndexedArray_getitem_nextcarry_outindex.cpp
+-rw-r--r--   0        0        0     1518 2023-02-16 15:37:39.000000 awkward-cpp-9/src/cpu-kernels/awkward_IndexedArray_index_of_nulls.cpp
+-rw-r--r--   0        0        0      779 2023-02-16 15:37:39.000000 awkward-cpp-9/src/cpu-kernels/awkward_IndexedArray_local_preparenext_64.cpp
+-rw-r--r--   0        0        0     1108 2023-02-16 15:37:39.000000 awkward-cpp-9/src/cpu-kernels/awkward_IndexedArray_numnull.cpp
+-rw-r--r--   0        0        0     1362 2023-02-16 15:37:39.000000 awkward-cpp-9/src/cpu-kernels/awkward_IndexedArray_numnull_parents.cpp
+-rw-r--r--   0        0        0      440 2023-02-16 15:37:39.000000 awkward-cpp-9/src/cpu-kernels/awkward_IndexedArray_numnull_unique.cpp
+-rw-r--r--   0        0        0     1314 2023-02-16 15:37:39.000000 awkward-cpp-9/src/cpu-kernels/awkward_IndexedArray_overlay_mask.cpp
+-rw-r--r--   0        0        0     1640 2023-02-16 15:37:39.000000 awkward-cpp-9/src/cpu-kernels/awkward_IndexedArray_ranges_carry_next_64.cpp
+-rw-r--r--   0        0        0     1866 2023-02-16 15:37:39.000000 awkward-cpp-9/src/cpu-kernels/awkward_IndexedArray_ranges_next_64.cpp
+-rw-r--r--   0        0        0     1640 2023-02-16 15:37:39.000000 awkward-cpp-9/src/cpu-kernels/awkward_IndexedArray_reduce_next_64.cpp
+-rw-r--r--   0        0        0      553 2023-02-16 15:37:39.000000 awkward-cpp-9/src/cpu-kernels/awkward_IndexedArray_reduce_next_fix_offsets_64.cpp
+-rw-r--r--   0        0        0     1367 2023-02-16 15:37:39.000000 awkward-cpp-9/src/cpu-kernels/awkward_IndexedArray_reduce_next_nonlocal_nextshifts_64.cpp
+-rw-r--r--   0        0        0     1603 2023-02-16 15:37:39.000000 awkward-cpp-9/src/cpu-kernels/awkward_IndexedArray_reduce_next_nonlocal_nextshifts_fromshifts_64.cpp
+-rw-r--r--   0        0        0     3642 2023-02-16 15:37:39.000000 awkward-cpp-9/src/cpu-kernels/awkward_IndexedArray_simplify.cpp
+-rw-r--r--   0        0        0      890 2023-02-16 15:37:39.000000 awkward-cpp-9/src/cpu-kernels/awkward_IndexedArray_unique_next_index_and_offsets_64.cpp
+-rw-r--r--   0        0        0     1391 2023-02-16 15:37:39.000000 awkward-cpp-9/src/cpu-kernels/awkward_IndexedArray_validity.cpp
+-rw-r--r--   0        0        0      831 2023-02-16 15:37:39.000000 awkward-cpp-9/src/cpu-kernels/awkward_IndexedOptionArray_rpad_and_clip_mask_axis1.cpp
+-rw-r--r--   0        0        0     2305 2023-02-16 15:37:39.000000 awkward-cpp-9/src/cpu-kernels/awkward_ListArray_broadcast_tooffsets.cpp
+-rw-r--r--   0        0        0     1940 2023-02-16 15:37:39.000000 awkward-cpp-9/src/cpu-kernels/awkward_ListArray_combinations.cpp
+-rw-r--r--   0        0        0     2228 2023-02-16 15:37:39.000000 awkward-cpp-9/src/cpu-kernels/awkward_ListArray_combinations_length.cpp
+-rw-r--r--   0        0        0     1507 2023-02-16 15:37:39.000000 awkward-cpp-9/src/cpu-kernels/awkward_ListArray_compact_offsets.cpp
+-rw-r--r--   0        0        0     1855 2023-02-16 15:37:39.000000 awkward-cpp-9/src/cpu-kernels/awkward_ListArray_fill.cpp
+-rw-r--r--   0        0        0     3482 2023-02-16 15:37:39.000000 awkward-cpp-9/src/cpu-kernels/awkward_ListArray_getitem_jagged_apply.cpp
+-rw-r--r--   0        0        0      860 2023-02-16 15:37:39.000000 awkward-cpp-9/src/cpu-kernels/awkward_ListArray_getitem_jagged_carrylen.cpp
+-rw-r--r--   0        0        0     2200 2023-02-16 15:37:39.000000 awkward-cpp-9/src/cpu-kernels/awkward_ListArray_getitem_jagged_descend.cpp
+-rw-r--r--   0        0        0     2417 2023-02-16 15:37:39.000000 awkward-cpp-9/src/cpu-kernels/awkward_ListArray_getitem_jagged_expand.cpp
+-rw-r--r--   0        0        0     1423 2023-02-16 15:37:39.000000 awkward-cpp-9/src/cpu-kernels/awkward_ListArray_getitem_jagged_numvalid.cpp
+-rw-r--r--   0        0        0     1619 2023-02-16 15:37:39.000000 awkward-cpp-9/src/cpu-kernels/awkward_ListArray_getitem_jagged_shrink.cpp
+-rw-r--r--   0        0        0     2600 2023-02-16 15:37:39.000000 awkward-cpp-9/src/cpu-kernels/awkward_ListArray_getitem_next_array.cpp
+-rw-r--r--   0        0        0     2820 2023-02-16 15:37:39.000000 awkward-cpp-9/src/cpu-kernels/awkward_ListArray_getitem_next_array_advanced.cpp
+-rw-r--r--   0        0        0     1674 2023-02-16 15:37:39.000000 awkward-cpp-9/src/cpu-kernels/awkward_ListArray_getitem_next_at.cpp
+-rw-r--r--   0        0        0     2855 2023-02-16 15:37:39.000000 awkward-cpp-9/src/cpu-kernels/awkward_ListArray_getitem_next_range.cpp
+-rw-r--r--   0        0        0     2320 2023-02-16 15:37:39.000000 awkward-cpp-9/src/cpu-kernels/awkward_ListArray_getitem_next_range_carrylength.cpp
+-rw-r--r--   0        0        0     1237 2023-02-16 15:37:39.000000 awkward-cpp-9/src/cpu-kernels/awkward_ListArray_getitem_next_range_counts.cpp
+-rw-r--r--   0        0        0     1625 2023-02-16 15:37:39.000000 awkward-cpp-9/src/cpu-kernels/awkward_ListArray_getitem_next_range_spreadadvanced.cpp
+-rw-r--r--   0        0        0     1207 2023-02-16 15:37:39.000000 awkward-cpp-9/src/cpu-kernels/awkward_ListArray_localindex.cpp
+-rw-r--r--   0        0        0     1352 2023-02-16 15:37:39.000000 awkward-cpp-9/src/cpu-kernels/awkward_ListArray_min_range.cpp
+-rw-r--r--   0        0        0     1565 2023-02-16 15:37:39.000000 awkward-cpp-9/src/cpu-kernels/awkward_ListArray_rpad_and_clip_length_axis1.cpp
+-rw-r--r--   0        0        0     1946 2023-02-16 15:37:39.000000 awkward-cpp-9/src/cpu-kernels/awkward_ListArray_rpad_axis1.cpp
+-rw-r--r--   0        0        0     1539 2023-02-16 15:37:39.000000 awkward-cpp-9/src/cpu-kernels/awkward_ListArray_validity.cpp
+-rw-r--r--   0        0        0     4055 2023-02-16 15:37:39.000000 awkward-cpp-9/src/cpu-kernels/awkward_ListOffsetArray_argsort_strings.cpp
+-rw-r--r--   0        0        0     1281 2023-02-16 15:37:39.000000 awkward-cpp-9/src/cpu-kernels/awkward_ListOffsetArray_compact_offsets.cpp
+-rw-r--r--   0        0        0     1482 2023-02-16 15:37:39.000000 awkward-cpp-9/src/cpu-kernels/awkward_ListOffsetArray_drop_none_indexes.cpp
+-rw-r--r--   0        0        0     1692 2023-02-16 15:37:39.000000 awkward-cpp-9/src/cpu-kernels/awkward_ListOffsetArray_flatten_offsets.cpp
+-rw-r--r--   0        0        0      740 2023-02-16 15:37:39.000000 awkward-cpp-9/src/cpu-kernels/awkward_ListOffsetArray_local_preparenext_64.cpp
+-rw-r--r--   0        0        0      629 2023-02-16 15:37:39.000000 awkward-cpp-9/src/cpu-kernels/awkward_ListOffsetArray_reduce_local_nextparents_64.cpp
+-rw-r--r--   0        0        0      673 2023-02-16 15:37:39.000000 awkward-cpp-9/src/cpu-kernels/awkward_ListOffsetArray_reduce_local_outoffsets_64.cpp
+-rw-r--r--   0        0        0      694 2023-02-16 15:37:39.000000 awkward-cpp-9/src/cpu-kernels/awkward_ListOffsetArray_reduce_nonlocal_maxcount_offsetscopy_64.cpp
+-rw-r--r--   0        0        0     1106 2023-02-16 15:37:39.000000 awkward-cpp-9/src/cpu-kernels/awkward_ListOffsetArray_reduce_nonlocal_nextshifts_64.cpp
+-rw-r--r--   0        0        0      614 2023-02-16 15:37:39.000000 awkward-cpp-9/src/cpu-kernels/awkward_ListOffsetArray_reduce_nonlocal_nextstarts_64.cpp
+-rw-r--r--   0        0        0     1412 2023-02-16 15:37:39.000000 awkward-cpp-9/src/cpu-kernels/awkward_ListOffsetArray_reduce_nonlocal_outstartsstops_64.cpp
+-rw-r--r--   0        0        0     1295 2023-02-16 15:37:39.000000 awkward-cpp-9/src/cpu-kernels/awkward_ListOffsetArray_reduce_nonlocal_preparenext_64.cpp
+-rw-r--r--   0        0        0     1613 2023-02-16 15:37:39.000000 awkward-cpp-9/src/cpu-kernels/awkward_ListOffsetArray_rpad_and_clip_axis1.cpp
+-rw-r--r--   0        0        0     1555 2023-02-16 15:37:39.000000 awkward-cpp-9/src/cpu-kernels/awkward_ListOffsetArray_rpad_axis1.cpp
+-rw-r--r--   0        0        0     1671 2023-02-16 15:37:39.000000 awkward-cpp-9/src/cpu-kernels/awkward_ListOffsetArray_rpad_length_axis1.cpp
+-rw-r--r--   0        0        0     1623 2023-02-16 15:37:39.000000 awkward-cpp-9/src/cpu-kernels/awkward_ListOffsetArray_toRegularArray.cpp
+-rw-r--r--   0        0        0     1651 2023-02-16 15:37:39.000000 awkward-cpp-9/src/cpu-kernels/awkward_MaskedArray_getitem_next_jagged_project.cpp
+-rw-r--r--   0        0        0    35489 2023-02-16 15:37:39.000000 awkward-cpp-9/src/cpu-kernels/awkward_NumpyArray_fill.cpp
+-rw-r--r--   0        0        0     2127 2023-02-16 15:37:39.000000 awkward-cpp-9/src/cpu-kernels/awkward_NumpyArray_rearrange_shifted.cpp
+-rw-r--r--   0        0        0      605 2023-02-16 15:37:39.000000 awkward-cpp-9/src/cpu-kernels/awkward_NumpyArray_reduce_adjust_starts_64.cpp
+-rw-r--r--   0        0        0      655 2023-02-16 15:37:39.000000 awkward-cpp-9/src/cpu-kernels/awkward_NumpyArray_reduce_adjust_starts_shifts_64.cpp
+-rw-r--r--   0        0        0      562 2023-02-16 15:37:39.000000 awkward-cpp-9/src/cpu-kernels/awkward_NumpyArray_reduce_mask_ByteMaskedArray_64.cpp
+-rw-r--r--   0        0        0     2095 2023-02-16 15:37:39.000000 awkward-cpp-9/src/cpu-kernels/awkward_NumpyArray_sort_asstrings_uint8.cpp
+-rw-r--r--   0        0        0     4235 2023-02-16 15:37:39.000000 awkward-cpp-9/src/cpu-kernels/awkward_NumpyArray_subrange_equal.cpp
+-rw-r--r--   0        0        0     1184 2023-02-16 15:37:39.000000 awkward-cpp-9/src/cpu-kernels/awkward_NumpyArray_unique_strings_uint8.cpp
+-rw-r--r--   0        0        0     1018 2023-02-16 15:37:39.000000 awkward-cpp-9/src/cpu-kernels/awkward_RegularArray_broadcast_tooffsets.cpp
+-rw-r--r--   0        0        0     1030 2023-02-16 15:37:39.000000 awkward-cpp-9/src/cpu-kernels/awkward_RegularArray_broadcast_tooffsets_size1.cpp
+-rw-r--r--   0        0        0      802 2023-02-16 15:37:39.000000 awkward-cpp-9/src/cpu-kernels/awkward_RegularArray_combinations.cpp
+-rw-r--r--   0        0        0      680 2023-02-16 15:37:39.000000 awkward-cpp-9/src/cpu-kernels/awkward_RegularArray_compact_offsets.cpp
+-rw-r--r--   0        0        0      783 2023-02-16 15:37:39.000000 awkward-cpp-9/src/cpu-kernels/awkward_RegularArray_getitem_carry.cpp
+-rw-r--r--   0        0        0     1009 2023-02-16 15:37:39.000000 awkward-cpp-9/src/cpu-kernels/awkward_RegularArray_getitem_jagged_expand.cpp
+-rw-r--r--   0        0        0      951 2023-02-16 15:37:39.000000 awkward-cpp-9/src/cpu-kernels/awkward_RegularArray_getitem_next_array.cpp
+-rw-r--r--   0        0        0     1037 2023-02-16 15:37:39.000000 awkward-cpp-9/src/cpu-kernels/awkward_RegularArray_getitem_next_array_advanced.cpp
+-rw-r--r--   0        0        0      985 2023-02-16 15:37:39.000000 awkward-cpp-9/src/cpu-kernels/awkward_RegularArray_getitem_next_array_regularize.cpp
+-rw-r--r--   0        0        0      904 2023-02-16 15:37:39.000000 awkward-cpp-9/src/cpu-kernels/awkward_RegularArray_getitem_next_at.cpp
+-rw-r--r--   0        0        0      913 2023-02-16 15:37:39.000000 awkward-cpp-9/src/cpu-kernels/awkward_RegularArray_getitem_next_range.cpp
+-rw-r--r--   0        0        0      890 2023-02-16 15:37:39.000000 awkward-cpp-9/src/cpu-kernels/awkward_RegularArray_getitem_next_range_spreadadvanced.cpp
+-rw-r--r--   0        0        0      678 2023-02-16 15:37:39.000000 awkward-cpp-9/src/cpu-kernels/awkward_RegularArray_localindex.cpp
+-rw-r--r--   0        0        0      647 2023-02-16 15:37:39.000000 awkward-cpp-9/src/cpu-kernels/awkward_RegularArray_reduce_local_nextparents_64.cpp
+-rw-r--r--   0        0        0      800 2023-02-16 15:37:39.000000 awkward-cpp-9/src/cpu-kernels/awkward_RegularArray_reduce_nonlocal_preparenext_64.cpp
+-rw-r--r--   0        0        0      920 2023-02-16 15:37:39.000000 awkward-cpp-9/src/cpu-kernels/awkward_RegularArray_rpad_and_clip_axis1.cpp
+-rw-r--r--   0        0        0     1290 2023-02-16 15:37:39.000000 awkward-cpp-9/src/cpu-kernels/awkward_UnionArray_fillindex.cpp
+-rw-r--r--   0        0        0      681 2023-02-16 15:37:39.000000 awkward-cpp-9/src/cpu-kernels/awkward_UnionArray_fillindex_count.cpp
+-rw-r--r--   0        0        0     1105 2023-02-16 15:37:39.000000 awkward-cpp-9/src/cpu-kernels/awkward_UnionArray_fillna.cpp
+-rw-r--r--   0        0        0      796 2023-02-16 15:37:39.000000 awkward-cpp-9/src/cpu-kernels/awkward_UnionArray_filltags.cpp
+-rw-r--r--   0        0        0      711 2023-02-16 15:37:39.000000 awkward-cpp-9/src/cpu-kernels/awkward_UnionArray_filltags_const.cpp
+-rw-r--r--   0        0        0     2163 2023-02-16 15:37:39.000000 awkward-cpp-9/src/cpu-kernels/awkward_UnionArray_flatten_combine.cpp
+-rw-r--r--   0        0        0     1702 2023-02-16 15:37:39.000000 awkward-cpp-9/src/cpu-kernels/awkward_UnionArray_flatten_length.cpp
+-rw-r--r--   0        0        0     1655 2023-02-16 15:37:39.000000 awkward-cpp-9/src/cpu-kernels/awkward_UnionArray_nestedfill_tags_index.cpp
+-rw-r--r--   0        0        0     1564 2023-02-16 15:37:39.000000 awkward-cpp-9/src/cpu-kernels/awkward_UnionArray_project.cpp
+-rw-r--r--   0        0        0     1442 2023-02-16 15:37:39.000000 awkward-cpp-9/src/cpu-kernels/awkward_UnionArray_regular_index.cpp
+-rw-r--r--   0        0        0      769 2023-02-16 15:37:39.000000 awkward-cpp-9/src/cpu-kernels/awkward_UnionArray_regular_index_getsize.cpp
+-rw-r--r--   0        0        0     5911 2023-02-16 15:37:39.000000 awkward-cpp-9/src/cpu-kernels/awkward_UnionArray_simplify.cpp
+-rw-r--r--   0        0        0     1959 2023-02-16 15:37:39.000000 awkward-cpp-9/src/cpu-kernels/awkward_UnionArray_simplify_one.cpp
+-rw-r--r--   0        0        0     1856 2023-02-16 15:37:39.000000 awkward-cpp-9/src/cpu-kernels/awkward_UnionArray_validity.cpp
+-rw-r--r--   0        0        0     6448 2023-02-16 15:37:39.000000 awkward-cpp-9/src/cpu-kernels/awkward_argsort.cpp
+-rw-r--r--   0        0        0      760 2023-02-16 15:37:39.000000 awkward-cpp-9/src/cpu-kernels/awkward_index_rpad_and_clip_axis0.cpp
+-rw-r--r--   0        0        0      764 2023-02-16 15:37:39.000000 awkward-cpp-9/src/cpu-kernels/awkward_index_rpad_and_clip_axis1.cpp
+-rw-r--r--   0        0        0      524 2023-02-16 15:37:39.000000 awkward-cpp-9/src/cpu-kernels/awkward_localindex.cpp
+-rw-r--r--   0        0        0      879 2023-02-16 15:37:39.000000 awkward-cpp-9/src/cpu-kernels/awkward_missing_repeat.cpp
+-rw-r--r--   0        0        0     3419 2023-02-16 15:37:39.000000 awkward-cpp-9/src/cpu-kernels/awkward_reduce_argmax.cpp
+-rw-r--r--   0        0        0     1393 2023-02-16 15:37:39.000000 awkward-cpp-9/src/cpu-kernels/awkward_reduce_argmax_complex.cpp
+-rw-r--r--   0        0        0     3415 2023-02-16 15:37:39.000000 awkward-cpp-9/src/cpu-kernels/awkward_reduce_argmin.cpp
+-rw-r--r--   0        0        0     1393 2023-02-16 15:37:39.000000 awkward-cpp-9/src/cpu-kernels/awkward_reduce_argmin_complex.cpp
+-rw-r--r--   0        0        0      509 2023-02-16 15:37:39.000000 awkward-cpp-9/src/cpu-kernels/awkward_reduce_count_64.cpp
+-rw-r--r--   0        0        0     3624 2023-02-16 15:37:39.000000 awkward-cpp-9/src/cpu-kernels/awkward_reduce_countnonzero.cpp
+-rw-r--r--   0        0        0     1202 2023-02-16 15:37:39.000000 awkward-cpp-9/src/cpu-kernels/awkward_reduce_countnonzero_complex.cpp
+-rw-r--r--   0        0        0     3734 2023-02-16 15:37:39.000000 awkward-cpp-9/src/cpu-kernels/awkward_reduce_max.cpp
+-rw-r--r--   0        0        0     1490 2023-02-16 15:37:39.000000 awkward-cpp-9/src/cpu-kernels/awkward_reduce_max_complex.cpp
+-rw-r--r--   0        0        0     3734 2023-02-16 15:37:39.000000 awkward-cpp-9/src/cpu-kernels/awkward_reduce_min.cpp
+-rw-r--r--   0        0        0     1488 2023-02-16 15:37:39.000000 awkward-cpp-9/src/cpu-kernels/awkward_reduce_min_complex.cpp
+-rw-r--r--   0        0        0     5019 2023-02-16 15:37:39.000000 awkward-cpp-9/src/cpu-kernels/awkward_reduce_prod.cpp
+-rw-r--r--   0        0        0     3519 2023-02-16 15:37:39.000000 awkward-cpp-9/src/cpu-kernels/awkward_reduce_prod_bool.cpp
+-rw-r--r--   0        0        0     1178 2023-02-16 15:37:39.000000 awkward-cpp-9/src/cpu-kernels/awkward_reduce_prod_bool_complex.cpp
+-rw-r--r--   0        0        0     1452 2023-02-16 15:37:39.000000 awkward-cpp-9/src/cpu-kernels/awkward_reduce_prod_complex.cpp
+-rw-r--r--   0        0        0     4985 2023-02-16 15:37:39.000000 awkward-cpp-9/src/cpu-kernels/awkward_reduce_sum.cpp
+-rw-r--r--   0        0        0     3496 2023-02-16 15:37:39.000000 awkward-cpp-9/src/cpu-kernels/awkward_reduce_sum_bool.cpp
+-rw-r--r--   0        0        0     1173 2023-02-16 15:37:39.000000 awkward-cpp-9/src/cpu-kernels/awkward_reduce_sum_bool_complex.cpp
+-rw-r--r--   0        0        0     1277 2023-02-16 15:37:39.000000 awkward-cpp-9/src/cpu-kernels/awkward_reduce_sum_complex.cpp
+-rw-r--r--   0        0        0      569 2023-02-16 15:37:39.000000 awkward-cpp-9/src/cpu-kernels/awkward_reduce_sum_int32_bool_64.cpp
+-rw-r--r--   0        0        0      569 2023-02-16 15:37:39.000000 awkward-cpp-9/src/cpu-kernels/awkward_reduce_sum_int64_bool_64.cpp
+-rw-r--r--   0        0        0     6405 2023-02-16 15:37:39.000000 awkward-cpp-9/src/cpu-kernels/awkward_sort.cpp
+-rw-r--r--   0        0        0      614 2023-02-16 15:37:39.000000 awkward-cpp-9/src/cpu-kernels/awkward_sorting_ranges.cpp
+-rw-r--r--   0        0        0      522 2023-02-16 15:37:39.000000 awkward-cpp-9/src/cpu-kernels/awkward_sorting_ranges_length.cpp
+-rw-r--r--   0        0        0     2351 2023-02-16 15:37:39.000000 awkward-cpp-9/src/cpu-kernels/awkward_unique.cpp
+-rw-r--r--   0        0        0     2967 2023-02-16 15:37:39.000000 awkward-cpp-9/src/cpu-kernels/awkward_unique_copy.cpp
+-rw-r--r--   0        0        0     1945 2023-02-16 15:37:39.000000 awkward-cpp-9/src/cpu-kernels/awkward_unique_offsets.cpp
+-rw-r--r--   0        0        0     3862 2023-02-16 15:37:39.000000 awkward-cpp-9/src/cpu-kernels/awkward_unique_ranges.cpp
+-rw-r--r--   0        0        0     2344 2023-02-16 15:37:39.000000 awkward-cpp-9/src/cpu-kernels/kernel-utils.cpp
+-rw-r--r--   0        0        0    11115 2023-02-16 15:37:39.000000 awkward-cpp-9/src/libawkward/builder/ArrayBuilder.cpp
+-rw-r--r--   0        0        0     4661 2023-02-16 15:37:39.000000 awkward-cpp-9/src/libawkward/builder/BoolBuilder.cpp
+-rw-r--r--   0        0        0      183 2023-02-16 15:37:39.000000 awkward-cpp-9/src/libawkward/builder/Builder.cpp
+-rw-r--r--   0        0        0     5293 2023-02-16 15:37:39.000000 awkward-cpp-9/src/libawkward/builder/Complex128Builder.cpp
+-rw-r--r--   0        0        0     6147 2023-02-16 15:37:39.000000 awkward-cpp-9/src/libawkward/builder/DatetimeBuilder.cpp
+-rw-r--r--   0        0        0     5141 2023-02-16 15:37:39.000000 awkward-cpp-9/src/libawkward/builder/Float64Builder.cpp
+-rw-r--r--   0        0        0     4895 2023-02-16 15:37:39.000000 awkward-cpp-9/src/libawkward/builder/Int64Builder.cpp
+-rw-r--r--   0        0        0     7364 2023-02-16 15:37:39.000000 awkward-cpp-9/src/libawkward/builder/ListBuilder.cpp
+-rw-r--r--   0        0        0     7743 2023-02-16 15:37:39.000000 awkward-cpp-9/src/libawkward/builder/OptionBuilder.cpp
+-rw-r--r--   0        0        0    18031 2023-02-16 15:37:39.000000 awkward-cpp-9/src/libawkward/builder/RecordBuilder.cpp
+-rw-r--r--   0        0        0     6750 2023-02-16 15:37:39.000000 awkward-cpp-9/src/libawkward/builder/StringBuilder.cpp
+-rw-r--r--   0        0        0    14161 2023-02-16 15:37:39.000000 awkward-cpp-9/src/libawkward/builder/TupleBuilder.cpp
+-rw-r--r--   0        0        0    14325 2023-02-16 15:37:39.000000 awkward-cpp-9/src/libawkward/builder/UnionBuilder.cpp
+-rw-r--r--   0        0        0     6182 2023-02-16 15:37:39.000000 awkward-cpp-9/src/libawkward/builder/UnknownBuilder.cpp
+-rw-r--r--   0        0        0    19525 2023-02-16 15:37:39.000000 awkward-cpp-9/src/libawkward/forth/ForthInputBuffer.cpp
+-rw-r--r--   0        0        0   147623 2023-02-16 15:37:39.000000 awkward-cpp-9/src/libawkward/forth/ForthMachine.cpp
+-rw-r--r--   0        0        0    22713 2023-02-16 15:37:39.000000 awkward-cpp-9/src/libawkward/forth/ForthOutputBuffer.cpp
+-rw-r--r--   0        0        0    43605 2023-02-16 15:37:39.000000 awkward-cpp-9/src/libawkward/io/json.cpp
+-rw-r--r--   0        0        0    15701 2023-02-16 15:37:39.000000 awkward-cpp-9/src/libawkward/util.cpp
+-rw-r--r--   0        0        0      726 2023-02-16 15:37:39.000000 awkward-cpp-9/src/python/_ext.cpp
+-rw-r--r--   0        0        0    10142 2023-02-16 15:37:39.000000 awkward-cpp-9/src/python/content.cpp
+-rw-r--r--   0        0        0    26562 2023-02-16 15:37:39.000000 awkward-cpp-9/src/python/forth.cpp
+-rw-r--r--   0        0        0     3776 2023-02-16 15:37:39.000000 awkward-cpp-9/src/python/io.cpp
+-rw-r--r--   0        0        0      146 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-cpu-kernels/__init__.py
+-rw-r--r--   0        0        0     4641 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-cpu-kernels/test_cpuawkward_BitMaskedArray_to_ByteMaskedArray.py
+-rw-r--r--   0        0        0     4247 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-cpu-kernels/test_cpuawkward_BitMaskedArray_to_IndexedOptionArray64.py
+-rw-r--r--   0        0        0     2349 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-cpu-kernels/test_cpuawkward_ByteMaskedArray_getitem_nextcarry_64.py
+-rw-r--r--   0        0        0     3273 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-cpu-kernels/test_cpuawkward_ByteMaskedArray_getitem_nextcarry_outindex_64.py
+-rw-r--r--   0        0        0     2672 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-cpu-kernels/test_cpuawkward_ByteMaskedArray_numnull.py
+-rw-r--r--   0        0        0    16212 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-cpu-kernels/test_cpuawkward_ByteMaskedArray_overlay_mask8.py
+-rw-r--r--   0        0        0      413 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-cpu-kernels/test_cpuawkward_ByteMaskedArray_reduce_next_64.py
+-rw-r--r--   0        0        0      433 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-cpu-kernels/test_cpuawkward_ByteMaskedArray_reduce_next_nonlocal_nextshifts_64.py
+-rw-r--r--   0        0        0      444 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-cpu-kernels/test_cpuawkward_ByteMaskedArray_reduce_next_nonlocal_nextshifts_fromshifts_64.py
+-rw-r--r--   0        0        0     2905 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-cpu-kernels/test_cpuawkward_ByteMaskedArray_toIndexedOptionArray64.py
+-rw-r--r--   0        0        0    28927 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-cpu-kernels/test_cpuawkward_Content_getitem_next_missing_jagged_getmaskstartstop.py
+-rw-r--r--   0        0        0      406 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-cpu-kernels/test_cpuawkward_Index_nones_as_index_64.py
+-rw-r--r--   0        0        0     2760 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-cpu-kernels/test_cpuawkward_IndexedArray32_flatten_nextcarry_64.py
+-rw-r--r--   0        0        0    16336 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-cpu-kernels/test_cpuawkward_IndexedArray32_flatten_none2empty_64.py
+-rw-r--r--   0        0        0     2760 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-cpu-kernels/test_cpuawkward_IndexedArray32_getitem_nextcarry_64.py
+-rw-r--r--   0        0        0     2334 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-cpu-kernels/test_cpuawkward_IndexedArray32_getitem_nextcarry_outindex_64.py
+-rw-r--r--   0        0        0      412 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-cpu-kernels/test_cpuawkward_IndexedArray32_index_of_nulls.py
+-rw-r--r--   0        0        0     2681 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-cpu-kernels/test_cpuawkward_IndexedArray32_numnull.py
+-rw-r--r--   0        0        0      413 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-cpu-kernels/test_cpuawkward_IndexedArray32_numnull_parents.py
+-rw-r--r--   0        0        0      416 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-cpu-kernels/test_cpuawkward_IndexedArray32_overlay_mask8_to64.py
+-rw-r--r--   0        0        0      418 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-cpu-kernels/test_cpuawkward_IndexedArray32_ranges_carry_next_64.py
+-rw-r--r--   0        0        0      412 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-cpu-kernels/test_cpuawkward_IndexedArray32_ranges_next_64.py
+-rw-r--r--   0        0        0      412 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-cpu-kernels/test_cpuawkward_IndexedArray32_reduce_next_64.py
+-rw-r--r--   0        0        0      432 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-cpu-kernels/test_cpuawkward_IndexedArray32_reduce_next_nonlocal_nextshifts_64.py
+-rw-r--r--   0        0        0      443 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-cpu-kernels/test_cpuawkward_IndexedArray32_reduce_next_nonlocal_nextshifts_fromshifts_64.py
+-rw-r--r--   0        0        0    10112 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-cpu-kernels/test_cpuawkward_IndexedArray32_simplify32_to64.py
+-rw-r--r--   0        0        0    10112 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-cpu-kernels/test_cpuawkward_IndexedArray32_simplify64_to64.py
+-rw-r--r--   0        0        0    10157 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-cpu-kernels/test_cpuawkward_IndexedArray32_simplifyU32_to64.py
+-rw-r--r--   0        0        0     8567 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-cpu-kernels/test_cpuawkward_IndexedArray32_validity.py
+-rw-r--r--   0        0        0     2760 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-cpu-kernels/test_cpuawkward_IndexedArray64_flatten_nextcarry_64.py
+-rw-r--r--   0        0        0    16336 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-cpu-kernels/test_cpuawkward_IndexedArray64_flatten_none2empty_64.py
+-rw-r--r--   0        0        0     2760 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-cpu-kernels/test_cpuawkward_IndexedArray64_getitem_nextcarry_64.py
+-rw-r--r--   0        0        0     2334 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-cpu-kernels/test_cpuawkward_IndexedArray64_getitem_nextcarry_outindex_64.py
+-rw-r--r--   0        0        0      412 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-cpu-kernels/test_cpuawkward_IndexedArray64_index_of_nulls.py
+-rw-r--r--   0        0        0     2681 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-cpu-kernels/test_cpuawkward_IndexedArray64_numnull.py
+-rw-r--r--   0        0        0      413 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-cpu-kernels/test_cpuawkward_IndexedArray64_numnull_parents.py
+-rw-r--r--   0        0        0      416 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-cpu-kernels/test_cpuawkward_IndexedArray64_overlay_mask8_to64.py
+-rw-r--r--   0        0        0      418 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-cpu-kernels/test_cpuawkward_IndexedArray64_ranges_carry_next_64.py
+-rw-r--r--   0        0        0      412 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-cpu-kernels/test_cpuawkward_IndexedArray64_ranges_next_64.py
+-rw-r--r--   0        0        0      412 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-cpu-kernels/test_cpuawkward_IndexedArray64_reduce_next_64.py
+-rw-r--r--   0        0        0      432 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-cpu-kernels/test_cpuawkward_IndexedArray64_reduce_next_nonlocal_nextshifts_64.py
+-rw-r--r--   0        0        0      443 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-cpu-kernels/test_cpuawkward_IndexedArray64_reduce_next_nonlocal_nextshifts_fromshifts_64.py
+-rw-r--r--   0        0        0    10112 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-cpu-kernels/test_cpuawkward_IndexedArray64_simplify32_to64.py
+-rw-r--r--   0        0        0    10112 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-cpu-kernels/test_cpuawkward_IndexedArray64_simplify64_to64.py
+-rw-r--r--   0        0        0    10157 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-cpu-kernels/test_cpuawkward_IndexedArray64_simplifyU32_to64.py
+-rw-r--r--   0        0        0     8567 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-cpu-kernels/test_cpuawkward_IndexedArray64_validity.py
+-rw-r--r--   0        0        0     2775 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-cpu-kernels/test_cpuawkward_IndexedArrayU32_flatten_nextcarry_64.py
+-rw-r--r--   0        0        0    16411 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-cpu-kernels/test_cpuawkward_IndexedArrayU32_flatten_none2empty_64.py
+-rw-r--r--   0        0        0     2775 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-cpu-kernels/test_cpuawkward_IndexedArrayU32_getitem_nextcarry_64.py
+-rw-r--r--   0        0        0     2346 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-cpu-kernels/test_cpuawkward_IndexedArrayU32_getitem_nextcarry_outindex_64.py
+-rw-r--r--   0        0        0      413 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-cpu-kernels/test_cpuawkward_IndexedArrayU32_index_of_nulls.py
+-rw-r--r--   0        0        0     2696 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-cpu-kernels/test_cpuawkward_IndexedArrayU32_numnull.py
+-rw-r--r--   0        0        0      414 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-cpu-kernels/test_cpuawkward_IndexedArrayU32_numnull_parents.py
+-rw-r--r--   0        0        0      417 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-cpu-kernels/test_cpuawkward_IndexedArrayU32_overlay_mask8_to64.py
+-rw-r--r--   0        0        0      419 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-cpu-kernels/test_cpuawkward_IndexedArrayU32_ranges_carry_next_64.py
+-rw-r--r--   0        0        0      413 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-cpu-kernels/test_cpuawkward_IndexedArrayU32_ranges_next_64.py
+-rw-r--r--   0        0        0      413 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-cpu-kernels/test_cpuawkward_IndexedArrayU32_reduce_next_64.py
+-rw-r--r--   0        0        0      433 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-cpu-kernels/test_cpuawkward_IndexedArrayU32_reduce_next_nonlocal_nextshifts_64.py
+-rw-r--r--   0        0        0      444 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-cpu-kernels/test_cpuawkward_IndexedArrayU32_reduce_next_nonlocal_nextshifts_fromshifts_64.py
+-rw-r--r--   0        0        0    10157 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-cpu-kernels/test_cpuawkward_IndexedArrayU32_simplify32_to64.py
+-rw-r--r--   0        0        0    10157 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-cpu-kernels/test_cpuawkward_IndexedArrayU32_simplify64_to64.py
+-rw-r--r--   0        0        0    10202 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-cpu-kernels/test_cpuawkward_IndexedArrayU32_simplifyU32_to64.py
+-rw-r--r--   0        0        0     8642 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-cpu-kernels/test_cpuawkward_IndexedArrayU32_validity.py
+-rw-r--r--   0        0        0     2456 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-cpu-kernels/test_cpuawkward_IndexedArray_fill_to64_count.py
+-rw-r--r--   0        0        0     3271 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-cpu-kernels/test_cpuawkward_IndexedArray_fill_to64_from32.py
+-rw-r--r--   0        0        0     3271 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-cpu-kernels/test_cpuawkward_IndexedArray_fill_to64_from64.py
+-rw-r--r--   0        0        0     3286 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-cpu-kernels/test_cpuawkward_IndexedArray_fill_to64_fromU32.py
+-rw-r--r--   0        0        0      413 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-cpu-kernels/test_cpuawkward_IndexedArray_numnull_unique_64.py
+-rw-r--r--   0        0        0      422 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-cpu-kernels/test_cpuawkward_IndexedArray_reduce_next_fix_offsets_64.py
+-rw-r--r--   0        0        0      428 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-cpu-kernels/test_cpuawkward_IndexedArray_unique_next_index_and_offsets_64.py
+-rw-r--r--   0        0        0     2930 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-cpu-kernels/test_cpuawkward_IndexedOptionArray_rpad_and_clip_mask_axis1_64.py
+-rw-r--r--   0        0        0     1591 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-cpu-kernels/test_cpuawkward_ListArray32_broadcast_tooffsets_64.py
+-rw-r--r--   0        0        0    22474 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-cpu-kernels/test_cpuawkward_ListArray32_combinations_length_64.py
+-rw-r--r--   0        0        0     3611 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-cpu-kernels/test_cpuawkward_ListArray32_compact_offsets_64.py
+-rw-r--r--   0        0        0    13418 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-cpu-kernels/test_cpuawkward_ListArray32_getitem_jagged_apply_64.py
+-rw-r--r--   0        0        0    21484 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-cpu-kernels/test_cpuawkward_ListArray32_getitem_jagged_descend_64.py
+-rw-r--r--   0        0        0     6605 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-cpu-kernels/test_cpuawkward_ListArray32_getitem_jagged_expand_64.py
+-rw-r--r--   0        0        0     8006 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-cpu-kernels/test_cpuawkward_ListArray32_getitem_next_array_64.py
+-rw-r--r--   0        0        0    49823 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-cpu-kernels/test_cpuawkward_ListArray32_getitem_next_array_advanced_64.py
+-rw-r--r--   0        0        0     1404 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-cpu-kernels/test_cpuawkward_ListArray32_getitem_next_at_64.py
+-rw-r--r--   0        0        0      416 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-cpu-kernels/test_cpuawkward_ListArray32_getitem_next_range_64.py
+-rw-r--r--   0        0        0      425 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-cpu-kernels/test_cpuawkward_ListArray32_getitem_next_range_carrylength.py
+-rw-r--r--   0        0        0     2861 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-cpu-kernels/test_cpuawkward_ListArray32_getitem_next_range_counts_64.py
+-rw-r--r--   0        0        0      431 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-cpu-kernels/test_cpuawkward_ListArray32_getitem_next_range_spreadadvanced_64.py
+-rw-r--r--   0        0        0     1768 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-cpu-kernels/test_cpuawkward_ListArray32_localindex_64.py
+-rw-r--r--   0        0        0     3249 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-cpu-kernels/test_cpuawkward_ListArray32_min_range.py
+-rw-r--r--   0        0        0     3535 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-cpu-kernels/test_cpuawkward_ListArray32_rpad_and_clip_length_axis1.py
+-rw-r--r--   0        0        0     5894 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-cpu-kernels/test_cpuawkward_ListArray32_rpad_axis1_64.py
+-rw-r--r--   0        0        0     2260 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-cpu-kernels/test_cpuawkward_ListArray32_validity.py
+-rw-r--r--   0        0        0     1591 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-cpu-kernels/test_cpuawkward_ListArray64_broadcast_tooffsets_64.py
+-rw-r--r--   0        0        0    22474 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-cpu-kernels/test_cpuawkward_ListArray64_combinations_length_64.py
+-rw-r--r--   0        0        0     3611 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-cpu-kernels/test_cpuawkward_ListArray64_compact_offsets_64.py
+-rw-r--r--   0        0        0    13418 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-cpu-kernels/test_cpuawkward_ListArray64_getitem_jagged_apply_64.py
+-rw-r--r--   0        0        0    21484 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-cpu-kernels/test_cpuawkward_ListArray64_getitem_jagged_descend_64.py
+-rw-r--r--   0        0        0     6605 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-cpu-kernels/test_cpuawkward_ListArray64_getitem_jagged_expand_64.py
+-rw-r--r--   0        0        0     8006 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-cpu-kernels/test_cpuawkward_ListArray64_getitem_next_array_64.py
+-rw-r--r--   0        0        0    49823 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-cpu-kernels/test_cpuawkward_ListArray64_getitem_next_array_advanced_64.py
+-rw-r--r--   0        0        0     1404 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-cpu-kernels/test_cpuawkward_ListArray64_getitem_next_at_64.py
+-rw-r--r--   0        0        0      416 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-cpu-kernels/test_cpuawkward_ListArray64_getitem_next_range_64.py
+-rw-r--r--   0        0        0      425 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-cpu-kernels/test_cpuawkward_ListArray64_getitem_next_range_carrylength.py
+-rw-r--r--   0        0        0     2861 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-cpu-kernels/test_cpuawkward_ListArray64_getitem_next_range_counts_64.py
+-rw-r--r--   0        0        0      431 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-cpu-kernels/test_cpuawkward_ListArray64_getitem_next_range_spreadadvanced_64.py
+-rw-r--r--   0        0        0     1768 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-cpu-kernels/test_cpuawkward_ListArray64_localindex_64.py
+-rw-r--r--   0        0        0     3249 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-cpu-kernels/test_cpuawkward_ListArray64_min_range.py
+-rw-r--r--   0        0        0     3535 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-cpu-kernels/test_cpuawkward_ListArray64_rpad_and_clip_length_axis1.py
+-rw-r--r--   0        0        0     5894 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-cpu-kernels/test_cpuawkward_ListArray64_rpad_axis1_64.py
+-rw-r--r--   0        0        0     2260 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-cpu-kernels/test_cpuawkward_ListArray64_validity.py
+-rw-r--r--   0        0        0     1599 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-cpu-kernels/test_cpuawkward_ListArrayU32_broadcast_tooffsets_64.py
+-rw-r--r--   0        0        0    22574 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-cpu-kernels/test_cpuawkward_ListArrayU32_combinations_length_64.py
+-rw-r--r--   0        0        0     3631 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-cpu-kernels/test_cpuawkward_ListArrayU32_compact_offsets_64.py
+-rw-r--r--   0        0        0    13458 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-cpu-kernels/test_cpuawkward_ListArrayU32_getitem_jagged_apply_64.py
+-rw-r--r--   0        0        0    21584 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-cpu-kernels/test_cpuawkward_ListArrayU32_getitem_jagged_descend_64.py
+-rw-r--r--   0        0        0     6625 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-cpu-kernels/test_cpuawkward_ListArrayU32_getitem_jagged_expand_64.py
+-rw-r--r--   0        0        0     8034 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-cpu-kernels/test_cpuawkward_ListArrayU32_getitem_next_array_64.py
+-rw-r--r--   0        0        0    49995 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-cpu-kernels/test_cpuawkward_ListArrayU32_getitem_next_array_advanced_64.py
+-rw-r--r--   0        0        0     1412 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-cpu-kernels/test_cpuawkward_ListArrayU32_getitem_next_at_64.py
+-rw-r--r--   0        0        0      417 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-cpu-kernels/test_cpuawkward_ListArrayU32_getitem_next_range_64.py
+-rw-r--r--   0        0        0      426 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-cpu-kernels/test_cpuawkward_ListArrayU32_getitem_next_range_carrylength.py
+-rw-r--r--   0        0        0     2876 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-cpu-kernels/test_cpuawkward_ListArrayU32_getitem_next_range_counts_64.py
+-rw-r--r--   0        0        0      432 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-cpu-kernels/test_cpuawkward_ListArrayU32_getitem_next_range_spreadadvanced_64.py
+-rw-r--r--   0        0        0     1777 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-cpu-kernels/test_cpuawkward_ListArrayU32_localindex_64.py
+-rw-r--r--   0        0        0     3269 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-cpu-kernels/test_cpuawkward_ListArrayU32_min_range.py
+-rw-r--r--   0        0        0     3555 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-cpu-kernels/test_cpuawkward_ListArrayU32_rpad_and_clip_length_axis1.py
+-rw-r--r--   0        0        0     5924 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-cpu-kernels/test_cpuawkward_ListArrayU32_rpad_axis1_64.py
+-rw-r--r--   0        0        0     2280 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-cpu-kernels/test_cpuawkward_ListArrayU32_validity.py
+-rw-r--r--   0        0        0     5312 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-cpu-kernels/test_cpuawkward_ListArray_fill_to64_from32.py
+-rw-r--r--   0        0        0     5312 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-cpu-kernels/test_cpuawkward_ListArray_fill_to64_from64.py
+-rw-r--r--   0        0        0     5332 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-cpu-kernels/test_cpuawkward_ListArray_fill_to64_fromU32.py
+-rw-r--r--   0        0        0     3625 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-cpu-kernels/test_cpuawkward_ListArray_getitem_jagged_carrylen_64.py
+-rw-r--r--   0        0        0      419 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-cpu-kernels/test_cpuawkward_ListArray_getitem_jagged_numvalid_64.py
+-rw-r--r--   0        0        0    27257 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-cpu-kernels/test_cpuawkward_ListArray_getitem_jagged_shrink_64.py
+-rw-r--r--   0        0        0     3094 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-cpu-kernels/test_cpuawkward_ListOffsetArray32_compact_offsets_64.py
+-rw-r--r--   0        0        0    19697 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-cpu-kernels/test_cpuawkward_ListOffsetArray32_flatten_offsets_64.py
+-rw-r--r--   0        0        0      423 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-cpu-kernels/test_cpuawkward_ListOffsetArray32_rpad_and_clip_axis1_64.py
+-rw-r--r--   0        0        0      414 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-cpu-kernels/test_cpuawkward_ListOffsetArray32_rpad_axis1_64.py
+-rw-r--r--   0        0        0      418 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-cpu-kernels/test_cpuawkward_ListOffsetArray32_rpad_length_axis1.py
+-rw-r--r--   0        0        0     2430 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-cpu-kernels/test_cpuawkward_ListOffsetArray32_toRegularArray.py
+-rw-r--r--   0        0        0     3094 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-cpu-kernels/test_cpuawkward_ListOffsetArray64_compact_offsets_64.py
+-rw-r--r--   0        0        0    19697 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-cpu-kernels/test_cpuawkward_ListOffsetArray64_flatten_offsets_64.py
+-rw-r--r--   0        0        0      423 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-cpu-kernels/test_cpuawkward_ListOffsetArray64_rpad_and_clip_axis1_64.py
+-rw-r--r--   0        0        0      414 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-cpu-kernels/test_cpuawkward_ListOffsetArray64_rpad_axis1_64.py
+-rw-r--r--   0        0        0      418 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-cpu-kernels/test_cpuawkward_ListOffsetArray64_rpad_length_axis1.py
+-rw-r--r--   0        0        0     2430 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-cpu-kernels/test_cpuawkward_ListOffsetArray64_toRegularArray.py
+-rw-r--r--   0        0        0     3109 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-cpu-kernels/test_cpuawkward_ListOffsetArrayU32_compact_offsets_64.py
+-rw-r--r--   0        0        0    19772 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-cpu-kernels/test_cpuawkward_ListOffsetArrayU32_flatten_offsets_64.py
+-rw-r--r--   0        0        0      424 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-cpu-kernels/test_cpuawkward_ListOffsetArrayU32_rpad_and_clip_axis1_64.py
+-rw-r--r--   0        0        0      415 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-cpu-kernels/test_cpuawkward_ListOffsetArrayU32_rpad_axis1_64.py
+-rw-r--r--   0        0        0      419 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-cpu-kernels/test_cpuawkward_ListOffsetArrayU32_rpad_length_axis1.py
+-rw-r--r--   0        0        0     2445 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-cpu-kernels/test_cpuawkward_ListOffsetArrayU32_toRegularArray.py
+-rw-r--r--   0        0        0    19202 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-cpu-kernels/test_cpuawkward_ListOffsetArray_drop_none_indexes_32.py
+-rw-r--r--   0        0        0    19202 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-cpu-kernels/test_cpuawkward_ListOffsetArray_drop_none_indexes_64.py
+-rw-r--r--   0        0        0      426 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-cpu-kernels/test_cpuawkward_ListOffsetArray_reduce_local_nextparents_64.py
+-rw-r--r--   0        0        0      425 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-cpu-kernels/test_cpuawkward_ListOffsetArray_reduce_local_outoffsets_64.py
+-rw-r--r--   0        0        0      438 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-cpu-kernels/test_cpuawkward_ListOffsetArray_reduce_nonlocal_maxcount_offsetscopy_64.py
+-rw-r--r--   0        0        0      428 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-cpu-kernels/test_cpuawkward_ListOffsetArray_reduce_nonlocal_nextshifts_64.py
+-rw-r--r--   0        0        0      428 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-cpu-kernels/test_cpuawkward_ListOffsetArray_reduce_nonlocal_nextstarts_64.py
+-rw-r--r--   0        0        0      432 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-cpu-kernels/test_cpuawkward_ListOffsetArray_reduce_nonlocal_outstartsstops_64.py
+-rw-r--r--   0        0        0    25597 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-cpu-kernels/test_cpuawkward_MaskedArray32_getitem_next_jagged_project.py
+-rw-r--r--   0        0        0    25597 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-cpu-kernels/test_cpuawkward_MaskedArray64_getitem_next_jagged_project.py
+-rw-r--r--   0        0        0    25672 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-cpu-kernels/test_cpuawkward_MaskedArrayU32_getitem_next_jagged_project.py
+-rw-r--r--   0        0        0      420 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-cpu-kernels/test_cpuawkward_NumpyArray_fill_tofloat32_fromfloat32.py
+-rw-r--r--   0        0        0      420 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-cpu-kernels/test_cpuawkward_NumpyArray_fill_tofloat32_fromfloat64.py
+-rw-r--r--   0        0        0      418 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-cpu-kernels/test_cpuawkward_NumpyArray_fill_tofloat32_fromint16.py
+-rw-r--r--   0        0        0      418 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-cpu-kernels/test_cpuawkward_NumpyArray_fill_tofloat32_fromint32.py
+-rw-r--r--   0        0        0      418 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-cpu-kernels/test_cpuawkward_NumpyArray_fill_tofloat32_fromint64.py
+-rw-r--r--   0        0        0      417 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-cpu-kernels/test_cpuawkward_NumpyArray_fill_tofloat32_fromint8.py
+-rw-r--r--   0        0        0      419 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-cpu-kernels/test_cpuawkward_NumpyArray_fill_tofloat32_fromuint16.py
+-rw-r--r--   0        0        0      419 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-cpu-kernels/test_cpuawkward_NumpyArray_fill_tofloat32_fromuint32.py
+-rw-r--r--   0        0        0      419 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-cpu-kernels/test_cpuawkward_NumpyArray_fill_tofloat32_fromuint64.py
+-rw-r--r--   0        0        0      418 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-cpu-kernels/test_cpuawkward_NumpyArray_fill_tofloat32_fromuint8.py
+-rw-r--r--   0        0        0      420 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-cpu-kernels/test_cpuawkward_NumpyArray_fill_tofloat64_fromfloat32.py
+-rw-r--r--   0        0        0      420 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-cpu-kernels/test_cpuawkward_NumpyArray_fill_tofloat64_fromfloat64.py
+-rw-r--r--   0        0        0      418 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-cpu-kernels/test_cpuawkward_NumpyArray_fill_tofloat64_fromint16.py
+-rw-r--r--   0        0        0      418 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-cpu-kernels/test_cpuawkward_NumpyArray_fill_tofloat64_fromint32.py
+-rw-r--r--   0        0        0      418 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-cpu-kernels/test_cpuawkward_NumpyArray_fill_tofloat64_fromint64.py
+-rw-r--r--   0        0        0      417 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-cpu-kernels/test_cpuawkward_NumpyArray_fill_tofloat64_fromint8.py
+-rw-r--r--   0        0        0      419 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-cpu-kernels/test_cpuawkward_NumpyArray_fill_tofloat64_fromuint16.py
+-rw-r--r--   0        0        0      419 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-cpu-kernels/test_cpuawkward_NumpyArray_fill_tofloat64_fromuint32.py
+-rw-r--r--   0        0        0      419 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-cpu-kernels/test_cpuawkward_NumpyArray_fill_tofloat64_fromuint64.py
+-rw-r--r--   0        0        0      418 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-cpu-kernels/test_cpuawkward_NumpyArray_fill_tofloat64_fromuint8.py
+-rw-r--r--   0        0        0      418 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-cpu-kernels/test_cpuawkward_NumpyArray_fill_toint16_fromfloat32.py
+-rw-r--r--   0        0        0      418 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-cpu-kernels/test_cpuawkward_NumpyArray_fill_toint16_fromfloat64.py
+-rw-r--r--   0        0        0      416 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-cpu-kernels/test_cpuawkward_NumpyArray_fill_toint16_fromint16.py
+-rw-r--r--   0        0        0      416 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-cpu-kernels/test_cpuawkward_NumpyArray_fill_toint16_fromint32.py
+-rw-r--r--   0        0        0      416 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-cpu-kernels/test_cpuawkward_NumpyArray_fill_toint16_fromint64.py
+-rw-r--r--   0        0        0      415 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-cpu-kernels/test_cpuawkward_NumpyArray_fill_toint16_fromint8.py
+-rw-r--r--   0        0        0      417 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-cpu-kernels/test_cpuawkward_NumpyArray_fill_toint16_fromuint16.py
+-rw-r--r--   0        0        0      417 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-cpu-kernels/test_cpuawkward_NumpyArray_fill_toint16_fromuint32.py
+-rw-r--r--   0        0        0      417 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-cpu-kernels/test_cpuawkward_NumpyArray_fill_toint16_fromuint64.py
+-rw-r--r--   0        0        0      416 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-cpu-kernels/test_cpuawkward_NumpyArray_fill_toint16_fromuint8.py
+-rw-r--r--   0        0        0      418 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-cpu-kernels/test_cpuawkward_NumpyArray_fill_toint32_fromfloat32.py
+-rw-r--r--   0        0        0      418 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-cpu-kernels/test_cpuawkward_NumpyArray_fill_toint32_fromfloat64.py
+-rw-r--r--   0        0        0      416 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-cpu-kernels/test_cpuawkward_NumpyArray_fill_toint32_fromint16.py
+-rw-r--r--   0        0        0      416 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-cpu-kernels/test_cpuawkward_NumpyArray_fill_toint32_fromint32.py
+-rw-r--r--   0        0        0      416 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-cpu-kernels/test_cpuawkward_NumpyArray_fill_toint32_fromint64.py
+-rw-r--r--   0        0        0      415 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-cpu-kernels/test_cpuawkward_NumpyArray_fill_toint32_fromint8.py
+-rw-r--r--   0        0        0      417 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-cpu-kernels/test_cpuawkward_NumpyArray_fill_toint32_fromuint16.py
+-rw-r--r--   0        0        0      417 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-cpu-kernels/test_cpuawkward_NumpyArray_fill_toint32_fromuint32.py
+-rw-r--r--   0        0        0      417 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-cpu-kernels/test_cpuawkward_NumpyArray_fill_toint32_fromuint64.py
+-rw-r--r--   0        0        0      416 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-cpu-kernels/test_cpuawkward_NumpyArray_fill_toint32_fromuint8.py
+-rw-r--r--   0        0        0      418 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-cpu-kernels/test_cpuawkward_NumpyArray_fill_toint64_fromfloat32.py
+-rw-r--r--   0        0        0      418 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-cpu-kernels/test_cpuawkward_NumpyArray_fill_toint64_fromfloat64.py
+-rw-r--r--   0        0        0      416 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-cpu-kernels/test_cpuawkward_NumpyArray_fill_toint64_fromint16.py
+-rw-r--r--   0        0        0      416 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-cpu-kernels/test_cpuawkward_NumpyArray_fill_toint64_fromint32.py
+-rw-r--r--   0        0        0      416 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-cpu-kernels/test_cpuawkward_NumpyArray_fill_toint64_fromint64.py
+-rw-r--r--   0        0        0      415 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-cpu-kernels/test_cpuawkward_NumpyArray_fill_toint64_fromint8.py
+-rw-r--r--   0        0        0      417 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-cpu-kernels/test_cpuawkward_NumpyArray_fill_toint64_fromuint16.py
+-rw-r--r--   0        0        0      417 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-cpu-kernels/test_cpuawkward_NumpyArray_fill_toint64_fromuint32.py
+-rw-r--r--   0        0        0      417 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-cpu-kernels/test_cpuawkward_NumpyArray_fill_toint64_fromuint64.py
+-rw-r--r--   0        0        0      416 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-cpu-kernels/test_cpuawkward_NumpyArray_fill_toint64_fromuint8.py
+-rw-r--r--   0        0        0      417 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-cpu-kernels/test_cpuawkward_NumpyArray_fill_toint8_fromfloat32.py
+-rw-r--r--   0        0        0      417 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-cpu-kernels/test_cpuawkward_NumpyArray_fill_toint8_fromfloat64.py
+-rw-r--r--   0        0        0      415 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-cpu-kernels/test_cpuawkward_NumpyArray_fill_toint8_fromint16.py
+-rw-r--r--   0        0        0      415 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-cpu-kernels/test_cpuawkward_NumpyArray_fill_toint8_fromint32.py
+-rw-r--r--   0        0        0      415 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-cpu-kernels/test_cpuawkward_NumpyArray_fill_toint8_fromint64.py
+-rw-r--r--   0        0        0      414 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-cpu-kernels/test_cpuawkward_NumpyArray_fill_toint8_fromint8.py
+-rw-r--r--   0        0        0      416 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-cpu-kernels/test_cpuawkward_NumpyArray_fill_toint8_fromuint16.py
+-rw-r--r--   0        0        0      416 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-cpu-kernels/test_cpuawkward_NumpyArray_fill_toint8_fromuint32.py
+-rw-r--r--   0        0        0      416 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-cpu-kernels/test_cpuawkward_NumpyArray_fill_toint8_fromuint64.py
+-rw-r--r--   0        0        0      415 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-cpu-kernels/test_cpuawkward_NumpyArray_fill_toint8_fromuint8.py
+-rw-r--r--   0        0        0      419 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-cpu-kernels/test_cpuawkward_NumpyArray_fill_touint16_fromfloat32.py
+-rw-r--r--   0        0        0      419 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-cpu-kernels/test_cpuawkward_NumpyArray_fill_touint16_fromfloat64.py
+-rw-r--r--   0        0        0      417 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-cpu-kernels/test_cpuawkward_NumpyArray_fill_touint16_fromint16.py
+-rw-r--r--   0        0        0      417 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-cpu-kernels/test_cpuawkward_NumpyArray_fill_touint16_fromint32.py
+-rw-r--r--   0        0        0      417 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-cpu-kernels/test_cpuawkward_NumpyArray_fill_touint16_fromint64.py
+-rw-r--r--   0        0        0      416 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-cpu-kernels/test_cpuawkward_NumpyArray_fill_touint16_fromint8.py
+-rw-r--r--   0        0        0      418 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-cpu-kernels/test_cpuawkward_NumpyArray_fill_touint16_fromuint16.py
+-rw-r--r--   0        0        0      418 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-cpu-kernels/test_cpuawkward_NumpyArray_fill_touint16_fromuint32.py
+-rw-r--r--   0        0        0      418 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-cpu-kernels/test_cpuawkward_NumpyArray_fill_touint16_fromuint64.py
+-rw-r--r--   0        0        0      417 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-cpu-kernels/test_cpuawkward_NumpyArray_fill_touint16_fromuint8.py
+-rw-r--r--   0        0        0      419 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-cpu-kernels/test_cpuawkward_NumpyArray_fill_touint32_fromfloat32.py
+-rw-r--r--   0        0        0      419 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-cpu-kernels/test_cpuawkward_NumpyArray_fill_touint32_fromfloat64.py
+-rw-r--r--   0        0        0      417 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-cpu-kernels/test_cpuawkward_NumpyArray_fill_touint32_fromint16.py
+-rw-r--r--   0        0        0      417 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-cpu-kernels/test_cpuawkward_NumpyArray_fill_touint32_fromint32.py
+-rw-r--r--   0        0        0      417 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-cpu-kernels/test_cpuawkward_NumpyArray_fill_touint32_fromint64.py
+-rw-r--r--   0        0        0      416 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-cpu-kernels/test_cpuawkward_NumpyArray_fill_touint32_fromint8.py
+-rw-r--r--   0        0        0      418 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-cpu-kernels/test_cpuawkward_NumpyArray_fill_touint32_fromuint16.py
+-rw-r--r--   0        0        0      418 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-cpu-kernels/test_cpuawkward_NumpyArray_fill_touint32_fromuint32.py
+-rw-r--r--   0        0        0      418 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-cpu-kernels/test_cpuawkward_NumpyArray_fill_touint32_fromuint64.py
+-rw-r--r--   0        0        0      417 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-cpu-kernels/test_cpuawkward_NumpyArray_fill_touint32_fromuint8.py
+-rw-r--r--   0        0        0      419 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-cpu-kernels/test_cpuawkward_NumpyArray_fill_touint64_fromfloat32.py
+-rw-r--r--   0        0        0      419 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-cpu-kernels/test_cpuawkward_NumpyArray_fill_touint64_fromfloat64.py
+-rw-r--r--   0        0        0      417 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-cpu-kernels/test_cpuawkward_NumpyArray_fill_touint64_fromint16.py
+-rw-r--r--   0        0        0      417 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-cpu-kernels/test_cpuawkward_NumpyArray_fill_touint64_fromint32.py
+-rw-r--r--   0        0        0      417 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-cpu-kernels/test_cpuawkward_NumpyArray_fill_touint64_fromint64.py
+-rw-r--r--   0        0        0      416 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-cpu-kernels/test_cpuawkward_NumpyArray_fill_touint64_fromint8.py
+-rw-r--r--   0        0        0      418 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-cpu-kernels/test_cpuawkward_NumpyArray_fill_touint64_fromuint16.py
+-rw-r--r--   0        0        0      418 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-cpu-kernels/test_cpuawkward_NumpyArray_fill_touint64_fromuint32.py
+-rw-r--r--   0        0        0      418 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-cpu-kernels/test_cpuawkward_NumpyArray_fill_touint64_fromuint64.py
+-rw-r--r--   0        0        0      417 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-cpu-kernels/test_cpuawkward_NumpyArray_fill_touint64_fromuint8.py
+-rw-r--r--   0        0        0      418 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-cpu-kernels/test_cpuawkward_NumpyArray_fill_touint8_fromfloat32.py
+-rw-r--r--   0        0        0      418 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-cpu-kernels/test_cpuawkward_NumpyArray_fill_touint8_fromfloat64.py
+-rw-r--r--   0        0        0      416 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-cpu-kernels/test_cpuawkward_NumpyArray_fill_touint8_fromint16.py
+-rw-r--r--   0        0        0      416 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-cpu-kernels/test_cpuawkward_NumpyArray_fill_touint8_fromint32.py
+-rw-r--r--   0        0        0      416 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-cpu-kernels/test_cpuawkward_NumpyArray_fill_touint8_fromint64.py
+-rw-r--r--   0        0        0      415 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-cpu-kernels/test_cpuawkward_NumpyArray_fill_touint8_fromint8.py
+-rw-r--r--   0        0        0      417 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-cpu-kernels/test_cpuawkward_NumpyArray_fill_touint8_fromuint16.py
+-rw-r--r--   0        0        0      417 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-cpu-kernels/test_cpuawkward_NumpyArray_fill_touint8_fromuint32.py
+-rw-r--r--   0        0        0      417 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-cpu-kernels/test_cpuawkward_NumpyArray_fill_touint8_fromuint64.py
+-rw-r--r--   0        0        0      416 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-cpu-kernels/test_cpuawkward_NumpyArray_fill_touint8_fromuint8.py
+-rw-r--r--   0        0        0      429 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-cpu-kernels/test_cpuawkward_NumpyArray_rearrange_shifted_toint64_fromint64.py
+-rw-r--r--   0        0        0      417 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-cpu-kernels/test_cpuawkward_NumpyArray_reduce_adjust_starts_64.py
+-rw-r--r--   0        0        0      424 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-cpu-kernels/test_cpuawkward_NumpyArray_reduce_adjust_starts_shifts_64.py
+-rw-r--r--   0        0        0      424 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-cpu-kernels/test_cpuawkward_NumpyArray_reduce_mask_ByteMaskedArray_64.py
+-rw-r--r--   0        0        0     9133 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-cpu-kernels/test_cpuawkward_RegularArray_broadcast_tooffsets_64.py
+-rw-r--r--   0        0        0      774 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-cpu-kernels/test_cpuawkward_RegularArray_broadcast_tooffsets_size1_64.py
+-rw-r--r--   0        0        0     2411 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-cpu-kernels/test_cpuawkward_RegularArray_compact_offsets64.py
+-rw-r--r--   0        0        0    11667 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-cpu-kernels/test_cpuawkward_RegularArray_getitem_carry_64.py
+-rw-r--r--   0        0        0    18563 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-cpu-kernels/test_cpuawkward_RegularArray_getitem_jagged_expand_64.py
+-rw-r--r--   0        0        0    22777 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-cpu-kernels/test_cpuawkward_RegularArray_getitem_next_array_64.py
+-rw-r--r--   0        0        0   121809 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-cpu-kernels/test_cpuawkward_RegularArray_getitem_next_array_advanced_64.py
+-rw-r--r--   0        0        0    12464 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-cpu-kernels/test_cpuawkward_RegularArray_getitem_next_array_regularize_64.py
+-rw-r--r--   0        0        0     1936 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-cpu-kernels/test_cpuawkward_RegularArray_getitem_next_at_64.py
+-rw-r--r--   0        0        0      771 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-cpu-kernels/test_cpuawkward_RegularArray_getitem_next_range_64.py
+-rw-r--r--   0        0        0    13383 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-cpu-kernels/test_cpuawkward_RegularArray_getitem_next_range_spreadadvanced_64.py
+-rw-r--r--   0        0        0     1932 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-cpu-kernels/test_cpuawkward_RegularArray_localindex_64.py
+-rw-r--r--   0        0        0      423 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-cpu-kernels/test_cpuawkward_RegularArray_reduce_local_nextparents_64.py
+-rw-r--r--   0        0        0      426 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-cpu-kernels/test_cpuawkward_RegularArray_reduce_nonlocal_preparenext_64.py
+-rw-r--r--   0        0        0      710 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-cpu-kernels/test_cpuawkward_RegularArray_rpad_and_clip_axis1_64.py
+-rw-r--r--   0        0        0      414 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-cpu-kernels/test_cpuawkward_UnionArray32_flatten_combine_64.py
+-rw-r--r--   0        0        0      413 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-cpu-kernels/test_cpuawkward_UnionArray32_flatten_length_64.py
+-rw-r--r--   0        0        0      414 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-cpu-kernels/test_cpuawkward_UnionArray64_flatten_combine_64.py
+-rw-r--r--   0        0        0      413 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-cpu-kernels/test_cpuawkward_UnionArray64_flatten_length_64.py
+-rw-r--r--   0        0        0      422 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-cpu-kernels/test_cpuawkward_UnionArray8_32_nestedfill_tags_index_64.py
+-rw-r--r--   0        0        0    12717 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-cpu-kernels/test_cpuawkward_UnionArray8_32_project_64.py
+-rw-r--r--   0        0        0     3937 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-cpu-kernels/test_cpuawkward_UnionArray8_32_regular_index.py
+-rw-r--r--   0        0        0   627958 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-cpu-kernels/test_cpuawkward_UnionArray8_32_simplify8_32_to8_64.py
+-rw-r--r--   0        0        0   627958 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-cpu-kernels/test_cpuawkward_UnionArray8_32_simplify8_64_to8_64.py
+-rw-r--r--   0        0        0   629458 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-cpu-kernels/test_cpuawkward_UnionArray8_32_simplify8_U32_to8_64.py
+-rw-r--r--   0        0        0    14172 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-cpu-kernels/test_cpuawkward_UnionArray8_32_simplify_one_to8_64.py
+-rw-r--r--   0        0        0    70417 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-cpu-kernels/test_cpuawkward_UnionArray8_32_validity.py
+-rw-r--r--   0        0        0      422 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-cpu-kernels/test_cpuawkward_UnionArray8_64_nestedfill_tags_index_64.py
+-rw-r--r--   0        0        0    12717 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-cpu-kernels/test_cpuawkward_UnionArray8_64_project_64.py
+-rw-r--r--   0        0        0     3937 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-cpu-kernels/test_cpuawkward_UnionArray8_64_regular_index.py
+-rw-r--r--   0        0        0   627958 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-cpu-kernels/test_cpuawkward_UnionArray8_64_simplify8_32_to8_64.py
+-rw-r--r--   0        0        0   627958 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-cpu-kernels/test_cpuawkward_UnionArray8_64_simplify8_64_to8_64.py
+-rw-r--r--   0        0        0   629458 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-cpu-kernels/test_cpuawkward_UnionArray8_64_simplify8_U32_to8_64.py
+-rw-r--r--   0        0        0    14172 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-cpu-kernels/test_cpuawkward_UnionArray8_64_simplify_one_to8_64.py
+-rw-r--r--   0        0        0    70417 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-cpu-kernels/test_cpuawkward_UnionArray8_64_validity.py
+-rw-r--r--   0        0        0      423 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-cpu-kernels/test_cpuawkward_UnionArray8_U32_nestedfill_tags_index_64.py
+-rw-r--r--   0        0        0    12762 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-cpu-kernels/test_cpuawkward_UnionArray8_U32_project_64.py
+-rw-r--r--   0        0        0     3957 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-cpu-kernels/test_cpuawkward_UnionArray8_U32_regular_index.py
+-rw-r--r--   0        0        0   629458 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-cpu-kernels/test_cpuawkward_UnionArray8_U32_simplify8_32_to8_64.py
+-rw-r--r--   0        0        0   629458 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-cpu-kernels/test_cpuawkward_UnionArray8_U32_simplify8_64_to8_64.py
+-rw-r--r--   0        0        0   630958 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-cpu-kernels/test_cpuawkward_UnionArray8_U32_simplify8_U32_to8_64.py
+-rw-r--r--   0        0        0    14217 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-cpu-kernels/test_cpuawkward_UnionArray8_U32_simplify_one_to8_64.py
+-rw-r--r--   0        0        0    70792 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-cpu-kernels/test_cpuawkward_UnionArray8_U32_validity.py
+-rw-r--r--   0        0        0     2687 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-cpu-kernels/test_cpuawkward_UnionArray8_regular_index_getsize.py
+-rw-r--r--   0        0        0      415 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-cpu-kernels/test_cpuawkward_UnionArrayU32_flatten_combine_64.py
+-rw-r--r--   0        0        0      414 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-cpu-kernels/test_cpuawkward_UnionArrayU32_flatten_length_64.py
+-rw-r--r--   0        0        0      685 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-cpu-kernels/test_cpuawkward_UnionArray_fillindex_to64_count.py
+-rw-r--r--   0        0        0     3206 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-cpu-kernels/test_cpuawkward_UnionArray_fillindex_to64_from32.py
+-rw-r--r--   0        0        0     3206 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-cpu-kernels/test_cpuawkward_UnionArray_fillindex_to64_from64.py
+-rw-r--r--   0        0        0     3221 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-cpu-kernels/test_cpuawkward_UnionArray_fillindex_to64_fromU32.py
+-rw-r--r--   0        0        0     2811 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-cpu-kernels/test_cpuawkward_UnionArray_fillna_from32_to64.py
+-rw-r--r--   0        0        0     2811 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-cpu-kernels/test_cpuawkward_UnionArray_fillna_from64_to64.py
+-rw-r--r--   0        0        0     2826 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-cpu-kernels/test_cpuawkward_UnionArray_fillna_fromU32_to64.py
+-rw-r--r--   0        0        0      688 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-cpu-kernels/test_cpuawkward_UnionArray_filltags_to8_const.py
+-rw-r--r--   0        0        0     3262 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-cpu-kernels/test_cpuawkward_UnionArray_filltags_to8_from8.py
+-rw-r--r--   0        0        0      629 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-cpu-kernels/test_cpuawkward_index_rpad_and_clip_axis0_64.py
+-rw-r--r--   0        0        0      836 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-cpu-kernels/test_cpuawkward_index_rpad_and_clip_axis1_64.py
+-rw-r--r--   0        0        0      576 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-cpu-kernels/test_cpuawkward_localindex_64.py
+-rw-r--r--   0        0        0    15433 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-cpu-kernels/test_cpuawkward_missing_repeat_64.py
+-rw-r--r--   0        0        0      407 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-cpu-kernels/test_cpuawkward_reduce_argmax_float32_64.py
+-rw-r--r--   0        0        0      407 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-cpu-kernels/test_cpuawkward_reduce_argmax_float64_64.py
+-rw-r--r--   0        0        0      405 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-cpu-kernels/test_cpuawkward_reduce_argmax_int16_64.py
+-rw-r--r--   0        0        0      405 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-cpu-kernels/test_cpuawkward_reduce_argmax_int32_64.py
+-rw-r--r--   0        0        0      405 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-cpu-kernels/test_cpuawkward_reduce_argmax_int64_64.py
+-rw-r--r--   0        0        0      404 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-cpu-kernels/test_cpuawkward_reduce_argmax_int8_64.py
+-rw-r--r--   0        0        0      406 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-cpu-kernels/test_cpuawkward_reduce_argmax_uint16_64.py
+-rw-r--r--   0        0        0      406 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-cpu-kernels/test_cpuawkward_reduce_argmax_uint32_64.py
+-rw-r--r--   0        0        0      406 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-cpu-kernels/test_cpuawkward_reduce_argmax_uint64_64.py
+-rw-r--r--   0        0        0      405 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-cpu-kernels/test_cpuawkward_reduce_argmax_uint8_64.py
+-rw-r--r--   0        0        0      407 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-cpu-kernels/test_cpuawkward_reduce_argmin_float32_64.py
+-rw-r--r--   0        0        0      407 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-cpu-kernels/test_cpuawkward_reduce_argmin_float64_64.py
+-rw-r--r--   0        0        0      405 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-cpu-kernels/test_cpuawkward_reduce_argmin_int16_64.py
+-rw-r--r--   0        0        0      405 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-cpu-kernels/test_cpuawkward_reduce_argmin_int32_64.py
+-rw-r--r--   0        0        0      405 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-cpu-kernels/test_cpuawkward_reduce_argmin_int64_64.py
+-rw-r--r--   0        0        0      404 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-cpu-kernels/test_cpuawkward_reduce_argmin_int8_64.py
+-rw-r--r--   0        0        0      406 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-cpu-kernels/test_cpuawkward_reduce_argmin_uint16_64.py
+-rw-r--r--   0        0        0      406 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-cpu-kernels/test_cpuawkward_reduce_argmin_uint32_64.py
+-rw-r--r--   0        0        0      406 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-cpu-kernels/test_cpuawkward_reduce_argmin_uint64_64.py
+-rw-r--r--   0        0        0      405 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-cpu-kernels/test_cpuawkward_reduce_argmin_uint8_64.py
+-rw-r--r--   0        0        0      398 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-cpu-kernels/test_cpuawkward_reduce_count_64.py
+-rw-r--r--   0        0        0      410 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-cpu-kernels/test_cpuawkward_reduce_countnonzero_bool_64.py
+-rw-r--r--   0        0        0      413 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-cpu-kernels/test_cpuawkward_reduce_countnonzero_float32_64.py
+-rw-r--r--   0        0        0      413 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-cpu-kernels/test_cpuawkward_reduce_countnonzero_float64_64.py
+-rw-r--r--   0        0        0      411 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-cpu-kernels/test_cpuawkward_reduce_countnonzero_int16_64.py
+-rw-r--r--   0        0        0      411 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-cpu-kernels/test_cpuawkward_reduce_countnonzero_int32_64.py
+-rw-r--r--   0        0        0      411 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-cpu-kernels/test_cpuawkward_reduce_countnonzero_int64_64.py
+-rw-r--r--   0        0        0      410 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-cpu-kernels/test_cpuawkward_reduce_countnonzero_int8_64.py
+-rw-r--r--   0        0        0      412 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-cpu-kernels/test_cpuawkward_reduce_countnonzero_uint16_64.py
+-rw-r--r--   0        0        0      412 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-cpu-kernels/test_cpuawkward_reduce_countnonzero_uint32_64.py
+-rw-r--r--   0        0        0      412 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-cpu-kernels/test_cpuawkward_reduce_countnonzero_uint64_64.py
+-rw-r--r--   0        0        0      411 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-cpu-kernels/test_cpuawkward_reduce_countnonzero_uint8_64.py
+-rw-r--r--   0        0        0      412 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-cpu-kernels/test_cpuawkward_reduce_max_float32_float32_64.py
+-rw-r--r--   0        0        0      412 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-cpu-kernels/test_cpuawkward_reduce_max_float64_float64_64.py
+-rw-r--r--   0        0        0      408 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-cpu-kernels/test_cpuawkward_reduce_max_int16_int16_64.py
+-rw-r--r--   0        0        0      408 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-cpu-kernels/test_cpuawkward_reduce_max_int32_int32_64.py
+-rw-r--r--   0        0        0      408 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-cpu-kernels/test_cpuawkward_reduce_max_int64_int64_64.py
+-rw-r--r--   0        0        0      406 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-cpu-kernels/test_cpuawkward_reduce_max_int8_int8_64.py
+-rw-r--r--   0        0        0      410 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-cpu-kernels/test_cpuawkward_reduce_max_uint16_uint16_64.py
+-rw-r--r--   0        0        0      410 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-cpu-kernels/test_cpuawkward_reduce_max_uint32_uint32_64.py
+-rw-r--r--   0        0        0      410 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-cpu-kernels/test_cpuawkward_reduce_max_uint64_uint64_64.py
+-rw-r--r--   0        0        0      408 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-cpu-kernels/test_cpuawkward_reduce_max_uint8_uint8_64.py
+-rw-r--r--   0        0        0      412 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-cpu-kernels/test_cpuawkward_reduce_min_float32_float32_64.py
+-rw-r--r--   0        0        0      412 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-cpu-kernels/test_cpuawkward_reduce_min_float64_float64_64.py
+-rw-r--r--   0        0        0      408 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-cpu-kernels/test_cpuawkward_reduce_min_int16_int16_64.py
+-rw-r--r--   0        0        0      408 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-cpu-kernels/test_cpuawkward_reduce_min_int32_int32_64.py
+-rw-r--r--   0        0        0      408 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-cpu-kernels/test_cpuawkward_reduce_min_int64_int64_64.py
+-rw-r--r--   0        0        0      406 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-cpu-kernels/test_cpuawkward_reduce_min_int8_int8_64.py
+-rw-r--r--   0        0        0      410 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-cpu-kernels/test_cpuawkward_reduce_min_uint16_uint16_64.py
+-rw-r--r--   0        0        0      410 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-cpu-kernels/test_cpuawkward_reduce_min_uint32_uint32_64.py
+-rw-r--r--   0        0        0      410 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-cpu-kernels/test_cpuawkward_reduce_min_uint64_uint64_64.py
+-rw-r--r--   0        0        0      408 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-cpu-kernels/test_cpuawkward_reduce_min_uint8_uint8_64.py
+-rw-r--r--   0        0        0      407 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-cpu-kernels/test_cpuawkward_reduce_prod_bool_bool_64.py
+-rw-r--r--   0        0        0      410 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-cpu-kernels/test_cpuawkward_reduce_prod_bool_float32_64.py
+-rw-r--r--   0        0        0      410 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-cpu-kernels/test_cpuawkward_reduce_prod_bool_float64_64.py
+-rw-r--r--   0        0        0      408 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-cpu-kernels/test_cpuawkward_reduce_prod_bool_int16_64.py
+-rw-r--r--   0        0        0      408 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-cpu-kernels/test_cpuawkward_reduce_prod_bool_int32_64.py
+-rw-r--r--   0        0        0      408 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-cpu-kernels/test_cpuawkward_reduce_prod_bool_int64_64.py
+-rw-r--r--   0        0        0      407 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-cpu-kernels/test_cpuawkward_reduce_prod_bool_int8_64.py
+-rw-r--r--   0        0        0      409 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-cpu-kernels/test_cpuawkward_reduce_prod_bool_uint16_64.py
+-rw-r--r--   0        0        0      409 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-cpu-kernels/test_cpuawkward_reduce_prod_bool_uint32_64.py
+-rw-r--r--   0        0        0      409 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-cpu-kernels/test_cpuawkward_reduce_prod_bool_uint64_64.py
+-rw-r--r--   0        0        0      408 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-cpu-kernels/test_cpuawkward_reduce_prod_bool_uint8_64.py
+-rw-r--r--   0        0        0      413 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-cpu-kernels/test_cpuawkward_reduce_prod_float32_float32_64.py
+-rw-r--r--   0        0        0      413 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-cpu-kernels/test_cpuawkward_reduce_prod_float64_float64_64.py
+-rw-r--r--   0        0        0      409 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-cpu-kernels/test_cpuawkward_reduce_prod_int32_int16_64.py
+-rw-r--r--   0        0        0      409 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-cpu-kernels/test_cpuawkward_reduce_prod_int32_int32_64.py
+-rw-r--r--   0        0        0      408 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-cpu-kernels/test_cpuawkward_reduce_prod_int32_int8_64.py
+-rw-r--r--   0        0        0      409 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-cpu-kernels/test_cpuawkward_reduce_prod_int64_int16_64.py
+-rw-r--r--   0        0        0      409 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-cpu-kernels/test_cpuawkward_reduce_prod_int64_int32_64.py
+-rw-r--r--   0        0        0      409 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-cpu-kernels/test_cpuawkward_reduce_prod_int64_int64_64.py
+-rw-r--r--   0        0        0      408 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-cpu-kernels/test_cpuawkward_reduce_prod_int64_int8_64.py
+-rw-r--r--   0        0        0      411 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-cpu-kernels/test_cpuawkward_reduce_prod_uint32_uint16_64.py
+-rw-r--r--   0        0        0      411 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-cpu-kernels/test_cpuawkward_reduce_prod_uint32_uint32_64.py
+-rw-r--r--   0        0        0      410 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-cpu-kernels/test_cpuawkward_reduce_prod_uint32_uint8_64.py
+-rw-r--r--   0        0        0      411 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-cpu-kernels/test_cpuawkward_reduce_prod_uint64_uint16_64.py
+-rw-r--r--   0        0        0      411 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-cpu-kernels/test_cpuawkward_reduce_prod_uint64_uint32_64.py
+-rw-r--r--   0        0        0      411 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-cpu-kernels/test_cpuawkward_reduce_prod_uint64_uint64_64.py
+-rw-r--r--   0        0        0      410 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-cpu-kernels/test_cpuawkward_reduce_prod_uint64_uint8_64.py
+-rw-r--r--   0        0        0      406 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-cpu-kernels/test_cpuawkward_reduce_sum_bool_bool_64.py
+-rw-r--r--   0        0        0      409 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-cpu-kernels/test_cpuawkward_reduce_sum_bool_float32_64.py
+-rw-r--r--   0        0        0      409 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-cpu-kernels/test_cpuawkward_reduce_sum_bool_float64_64.py
+-rw-r--r--   0        0        0      407 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-cpu-kernels/test_cpuawkward_reduce_sum_bool_int16_64.py
+-rw-r--r--   0        0        0      407 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-cpu-kernels/test_cpuawkward_reduce_sum_bool_int32_64.py
+-rw-r--r--   0        0        0      407 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-cpu-kernels/test_cpuawkward_reduce_sum_bool_int64_64.py
+-rw-r--r--   0        0        0      406 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-cpu-kernels/test_cpuawkward_reduce_sum_bool_int8_64.py
+-rw-r--r--   0        0        0      408 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-cpu-kernels/test_cpuawkward_reduce_sum_bool_uint16_64.py
+-rw-r--r--   0        0        0      408 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-cpu-kernels/test_cpuawkward_reduce_sum_bool_uint32_64.py
+-rw-r--r--   0        0        0      408 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-cpu-kernels/test_cpuawkward_reduce_sum_bool_uint64_64.py
+-rw-r--r--   0        0        0      407 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-cpu-kernels/test_cpuawkward_reduce_sum_bool_uint8_64.py
+-rw-r--r--   0        0        0      412 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-cpu-kernels/test_cpuawkward_reduce_sum_float32_float32_64.py
+-rw-r--r--   0        0        0      412 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-cpu-kernels/test_cpuawkward_reduce_sum_float64_float64_64.py
+-rw-r--r--   0        0        0      407 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-cpu-kernels/test_cpuawkward_reduce_sum_int32_bool_64.py
+-rw-r--r--   0        0        0      408 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-cpu-kernels/test_cpuawkward_reduce_sum_int32_int16_64.py
+-rw-r--r--   0        0        0      408 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-cpu-kernels/test_cpuawkward_reduce_sum_int32_int32_64.py
+-rw-r--r--   0        0        0      407 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-cpu-kernels/test_cpuawkward_reduce_sum_int32_int8_64.py
+-rw-r--r--   0        0        0      407 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-cpu-kernels/test_cpuawkward_reduce_sum_int64_bool_64.py
+-rw-r--r--   0        0        0      408 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-cpu-kernels/test_cpuawkward_reduce_sum_int64_int16_64.py
+-rw-r--r--   0        0        0      408 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-cpu-kernels/test_cpuawkward_reduce_sum_int64_int32_64.py
+-rw-r--r--   0        0        0      408 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-cpu-kernels/test_cpuawkward_reduce_sum_int64_int64_64.py
+-rw-r--r--   0        0        0      407 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-cpu-kernels/test_cpuawkward_reduce_sum_int64_int8_64.py
+-rw-r--r--   0        0        0      410 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-cpu-kernels/test_cpuawkward_reduce_sum_uint32_uint16_64.py
+-rw-r--r--   0        0        0      410 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-cpu-kernels/test_cpuawkward_reduce_sum_uint32_uint32_64.py
+-rw-r--r--   0        0        0      409 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-cpu-kernels/test_cpuawkward_reduce_sum_uint32_uint8_64.py
+-rw-r--r--   0        0        0      410 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-cpu-kernels/test_cpuawkward_reduce_sum_uint64_uint16_64.py
+-rw-r--r--   0        0        0      410 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-cpu-kernels/test_cpuawkward_reduce_sum_uint64_uint32_64.py
+-rw-r--r--   0        0        0      410 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-cpu-kernels/test_cpuawkward_reduce_sum_uint64_uint64_64.py
+-rw-r--r--   0        0        0      409 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-cpu-kernels/test_cpuawkward_reduce_sum_uint64_uint8_64.py
+-rw-r--r--   0        0        0      146 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-spec/__init__.py
+-rw-r--r--   0        0        0    78359 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-spec/kernels.py
+-rw-r--r--   0        0        0     4076 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-spec/test_pyawkward_BitMaskedArray_to_ByteMaskedArray.py
+-rw-r--r--   0        0        0     3707 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-spec/test_pyawkward_BitMaskedArray_to_IndexedOptionArray64.py
+-rw-r--r--   0        0        0     1901 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-spec/test_pyawkward_ByteMaskedArray_getitem_nextcarry_64.py
+-rw-r--r--   0        0        0     2633 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-spec/test_pyawkward_ByteMaskedArray_getitem_nextcarry_outindex_64.py
+-rw-r--r--   0        0        0     2122 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-spec/test_pyawkward_ByteMaskedArray_numnull.py
+-rw-r--r--   0        0        0    12372 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-spec/test_pyawkward_ByteMaskedArray_overlay_mask8.py
+-rw-r--r--   0        0        0      372 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-spec/test_pyawkward_ByteMaskedArray_reduce_next_64.py
+-rw-r--r--   0        0        0      392 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-spec/test_pyawkward_ByteMaskedArray_reduce_next_nonlocal_nextshifts_64.py
+-rw-r--r--   0        0        0      403 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-spec/test_pyawkward_ByteMaskedArray_reduce_next_nonlocal_nextshifts_fromshifts_64.py
+-rw-r--r--   0        0        0     2355 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-spec/test_pyawkward_ByteMaskedArray_toIndexedOptionArray64.py
+-rw-r--r--   0        0        0    21962 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-spec/test_pyawkward_Content_getitem_next_missing_jagged_getmaskstartstop.py
+-rw-r--r--   0        0        0      365 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-spec/test_pyawkward_Index_nones_as_index_64.py
+-rw-r--r--   0        0        0     2304 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-spec/test_pyawkward_IndexedArray32_flatten_nextcarry_64.py
+-rw-r--r--   0        0        0    13526 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-spec/test_pyawkward_IndexedArray32_flatten_none2empty_64.py
+-rw-r--r--   0        0        0     2304 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-spec/test_pyawkward_IndexedArray32_getitem_nextcarry_64.py
+-rw-r--r--   0        0        0     1893 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-spec/test_pyawkward_IndexedArray32_getitem_nextcarry_outindex_64.py
+-rw-r--r--   0        0        0      371 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-spec/test_pyawkward_IndexedArray32_index_of_nulls.py
+-rw-r--r--   0        0        0     2036 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-spec/test_pyawkward_IndexedArray32_numnull.py
+-rw-r--r--   0        0        0      372 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-spec/test_pyawkward_IndexedArray32_numnull_parents.py
+-rw-r--r--   0        0        0      375 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-spec/test_pyawkward_IndexedArray32_overlay_mask8_to64.py
+-rw-r--r--   0        0        0      377 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-spec/test_pyawkward_IndexedArray32_ranges_carry_next_64.py
+-rw-r--r--   0        0        0      371 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-spec/test_pyawkward_IndexedArray32_ranges_next_64.py
+-rw-r--r--   0        0        0      371 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-spec/test_pyawkward_IndexedArray32_reduce_next_64.py
+-rw-r--r--   0        0        0      391 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-spec/test_pyawkward_IndexedArray32_reduce_next_nonlocal_nextshifts_64.py
+-rw-r--r--   0        0        0      402 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-spec/test_pyawkward_IndexedArray32_reduce_next_nonlocal_nextshifts_fromshifts_64.py
+-rw-r--r--   0        0        0     8007 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-spec/test_pyawkward_IndexedArray32_simplify32_to64.py
+-rw-r--r--   0        0        0     8007 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-spec/test_pyawkward_IndexedArray32_simplify64_to64.py
+-rw-r--r--   0        0        0     8037 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-spec/test_pyawkward_IndexedArray32_simplifyU32_to64.py
+-rw-r--r--   0        0        0     8307 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-spec/test_pyawkward_IndexedArray32_validity.py
+-rw-r--r--   0        0        0     2304 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-spec/test_pyawkward_IndexedArray64_flatten_nextcarry_64.py
+-rw-r--r--   0        0        0    13526 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-spec/test_pyawkward_IndexedArray64_flatten_none2empty_64.py
+-rw-r--r--   0        0        0     2304 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-spec/test_pyawkward_IndexedArray64_getitem_nextcarry_64.py
+-rw-r--r--   0        0        0     1893 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-spec/test_pyawkward_IndexedArray64_getitem_nextcarry_outindex_64.py
+-rw-r--r--   0        0        0      371 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-spec/test_pyawkward_IndexedArray64_index_of_nulls.py
+-rw-r--r--   0        0        0     2036 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-spec/test_pyawkward_IndexedArray64_numnull.py
+-rw-r--r--   0        0        0      372 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-spec/test_pyawkward_IndexedArray64_numnull_parents.py
+-rw-r--r--   0        0        0      375 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-spec/test_pyawkward_IndexedArray64_overlay_mask8_to64.py
+-rw-r--r--   0        0        0      377 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-spec/test_pyawkward_IndexedArray64_ranges_carry_next_64.py
+-rw-r--r--   0        0        0      371 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-spec/test_pyawkward_IndexedArray64_ranges_next_64.py
+-rw-r--r--   0        0        0      371 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-spec/test_pyawkward_IndexedArray64_reduce_next_64.py
+-rw-r--r--   0        0        0      391 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-spec/test_pyawkward_IndexedArray64_reduce_next_nonlocal_nextshifts_64.py
+-rw-r--r--   0        0        0      402 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-spec/test_pyawkward_IndexedArray64_reduce_next_nonlocal_nextshifts_fromshifts_64.py
+-rw-r--r--   0        0        0     8007 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-spec/test_pyawkward_IndexedArray64_simplify32_to64.py
+-rw-r--r--   0        0        0     8007 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-spec/test_pyawkward_IndexedArray64_simplify64_to64.py
+-rw-r--r--   0        0        0     8037 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-spec/test_pyawkward_IndexedArray64_simplifyU32_to64.py
+-rw-r--r--   0        0        0     8307 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-spec/test_pyawkward_IndexedArray64_validity.py
+-rw-r--r--   0        0        0     2314 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-spec/test_pyawkward_IndexedArrayU32_flatten_nextcarry_64.py
+-rw-r--r--   0        0        0    13576 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-spec/test_pyawkward_IndexedArrayU32_flatten_none2empty_64.py
+-rw-r--r--   0        0        0     2314 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-spec/test_pyawkward_IndexedArrayU32_getitem_nextcarry_64.py
+-rw-r--r--   0        0        0     1899 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-spec/test_pyawkward_IndexedArrayU32_getitem_nextcarry_outindex_64.py
+-rw-r--r--   0        0        0      372 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-spec/test_pyawkward_IndexedArrayU32_index_of_nulls.py
+-rw-r--r--   0        0        0     2046 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-spec/test_pyawkward_IndexedArrayU32_numnull.py
+-rw-r--r--   0        0        0      373 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-spec/test_pyawkward_IndexedArrayU32_numnull_parents.py
+-rw-r--r--   0        0        0      376 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-spec/test_pyawkward_IndexedArrayU32_overlay_mask8_to64.py
+-rw-r--r--   0        0        0      378 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-spec/test_pyawkward_IndexedArrayU32_ranges_carry_next_64.py
+-rw-r--r--   0        0        0      372 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-spec/test_pyawkward_IndexedArrayU32_ranges_next_64.py
+-rw-r--r--   0        0        0      372 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-spec/test_pyawkward_IndexedArrayU32_reduce_next_64.py
+-rw-r--r--   0        0        0      392 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-spec/test_pyawkward_IndexedArrayU32_reduce_next_nonlocal_nextshifts_64.py
+-rw-r--r--   0        0        0      403 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-spec/test_pyawkward_IndexedArrayU32_reduce_next_nonlocal_nextshifts_fromshifts_64.py
+-rw-r--r--   0        0        0     8037 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-spec/test_pyawkward_IndexedArrayU32_simplify32_to64.py
+-rw-r--r--   0        0        0     8037 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-spec/test_pyawkward_IndexedArrayU32_simplify64_to64.py
+-rw-r--r--   0        0        0     8067 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-spec/test_pyawkward_IndexedArrayU32_simplifyU32_to64.py
+-rw-r--r--   0        0        0     8357 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-spec/test_pyawkward_IndexedArrayU32_validity.py
+-rw-r--r--   0        0        0     2146 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-spec/test_pyawkward_IndexedArray_fill_to64_count.py
+-rw-r--r--   0        0        0     2711 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-spec/test_pyawkward_IndexedArray_fill_to64_from32.py
+-rw-r--r--   0        0        0     2711 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-spec/test_pyawkward_IndexedArray_fill_to64_from64.py
+-rw-r--r--   0        0        0     2721 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-spec/test_pyawkward_IndexedArray_fill_to64_fromU32.py
+-rw-r--r--   0        0        0      372 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-spec/test_pyawkward_IndexedArray_numnull_unique_64.py
+-rw-r--r--   0        0        0      381 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-spec/test_pyawkward_IndexedArray_reduce_next_fix_offsets_64.py
+-rw-r--r--   0        0        0      387 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-spec/test_pyawkward_IndexedArray_unique_next_index_and_offsets_64.py
+-rw-r--r--   0        0        0     2290 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-spec/test_pyawkward_IndexedOptionArray_rpad_and_clip_mask_axis1_64.py
+-rw-r--r--   0        0        0     1263 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-spec/test_pyawkward_ListArray32_broadcast_tooffsets_64.py
+-rw-r--r--   0        0        0    17509 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-spec/test_pyawkward_ListArray32_combinations_length_64.py
+-rw-r--r--   0        0        0     2676 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-spec/test_pyawkward_ListArray32_compact_offsets_64.py
+-rw-r--r--   0        0        0    10002 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-spec/test_pyawkward_ListArray32_getitem_jagged_apply_64.py
+-rw-r--r--   0        0        0    15834 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-spec/test_pyawkward_ListArray32_getitem_jagged_descend_64.py
+-rw-r--r--   0        0        0     4925 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-spec/test_pyawkward_ListArray32_getitem_jagged_expand_64.py
+-rw-r--r--   0        0        0     6255 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-spec/test_pyawkward_ListArray32_getitem_next_array_64.py
+-rw-r--r--   0        0        0    37324 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-spec/test_pyawkward_ListArray32_getitem_next_array_advanced_64.py
+-rw-r--r--   0        0        0     1093 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-spec/test_pyawkward_ListArray32_getitem_next_at_64.py
+-rw-r--r--   0        0        0      375 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-spec/test_pyawkward_ListArray32_getitem_next_range_64.py
+-rw-r--r--   0        0        0      384 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-spec/test_pyawkward_ListArray32_getitem_next_range_carrylength.py
+-rw-r--r--   0        0        0     2221 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-spec/test_pyawkward_ListArray32_getitem_next_range_counts_64.py
+-rw-r--r--   0        0        0      390 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-spec/test_pyawkward_ListArray32_getitem_next_range_spreadadvanced_64.py
+-rw-r--r--   0        0        0     1371 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-spec/test_pyawkward_ListArray32_localindex_64.py
+-rw-r--r--   0        0        0     2369 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-spec/test_pyawkward_ListArray32_min_range.py
+-rw-r--r--   0        0        0     2690 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-spec/test_pyawkward_ListArray32_rpad_and_clip_length_axis1.py
+-rw-r--r--   0        0        0     4544 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-spec/test_pyawkward_ListArray32_rpad_axis1_64.py
+-rw-r--r--   0        0        0     1911 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-spec/test_pyawkward_ListArray32_validity.py
+-rw-r--r--   0        0        0     1263 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-spec/test_pyawkward_ListArray64_broadcast_tooffsets_64.py
+-rw-r--r--   0        0        0    17509 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-spec/test_pyawkward_ListArray64_combinations_length_64.py
+-rw-r--r--   0        0        0     2676 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-spec/test_pyawkward_ListArray64_compact_offsets_64.py
+-rw-r--r--   0        0        0    10002 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-spec/test_pyawkward_ListArray64_getitem_jagged_apply_64.py
+-rw-r--r--   0        0        0    15834 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-spec/test_pyawkward_ListArray64_getitem_jagged_descend_64.py
+-rw-r--r--   0        0        0     4925 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-spec/test_pyawkward_ListArray64_getitem_jagged_expand_64.py
+-rw-r--r--   0        0        0     6255 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-spec/test_pyawkward_ListArray64_getitem_next_array_64.py
+-rw-r--r--   0        0        0    37324 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-spec/test_pyawkward_ListArray64_getitem_next_array_advanced_64.py
+-rw-r--r--   0        0        0     1093 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-spec/test_pyawkward_ListArray64_getitem_next_at_64.py
+-rw-r--r--   0        0        0      375 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-spec/test_pyawkward_ListArray64_getitem_next_range_64.py
+-rw-r--r--   0        0        0      384 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-spec/test_pyawkward_ListArray64_getitem_next_range_carrylength.py
+-rw-r--r--   0        0        0     2221 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-spec/test_pyawkward_ListArray64_getitem_next_range_counts_64.py
+-rw-r--r--   0        0        0      390 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-spec/test_pyawkward_ListArray64_getitem_next_range_spreadadvanced_64.py
+-rw-r--r--   0        0        0     1371 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-spec/test_pyawkward_ListArray64_localindex_64.py
+-rw-r--r--   0        0        0     2369 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-spec/test_pyawkward_ListArray64_min_range.py
+-rw-r--r--   0        0        0     2690 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-spec/test_pyawkward_ListArray64_rpad_and_clip_length_axis1.py
+-rw-r--r--   0        0        0     4544 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-spec/test_pyawkward_ListArray64_rpad_axis1_64.py
+-rw-r--r--   0        0        0     1911 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-spec/test_pyawkward_ListArray64_validity.py
+-rw-r--r--   0        0        0     1267 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-spec/test_pyawkward_ListArrayU32_broadcast_tooffsets_64.py
+-rw-r--r--   0        0        0    17559 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-spec/test_pyawkward_ListArrayU32_combinations_length_64.py
+-rw-r--r--   0        0        0     2686 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-spec/test_pyawkward_ListArrayU32_compact_offsets_64.py
+-rw-r--r--   0        0        0    10022 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-spec/test_pyawkward_ListArrayU32_getitem_jagged_apply_64.py
+-rw-r--r--   0        0        0    15884 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-spec/test_pyawkward_ListArrayU32_getitem_jagged_descend_64.py
+-rw-r--r--   0        0        0     4935 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-spec/test_pyawkward_ListArrayU32_getitem_jagged_expand_64.py
+-rw-r--r--   0        0        0     6269 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-spec/test_pyawkward_ListArrayU32_getitem_next_array_64.py
+-rw-r--r--   0        0        0    37410 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-spec/test_pyawkward_ListArrayU32_getitem_next_array_advanced_64.py
+-rw-r--r--   0        0        0     1097 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-spec/test_pyawkward_ListArrayU32_getitem_next_at_64.py
+-rw-r--r--   0        0        0      376 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-spec/test_pyawkward_ListArrayU32_getitem_next_range_64.py
+-rw-r--r--   0        0        0      385 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-spec/test_pyawkward_ListArrayU32_getitem_next_range_carrylength.py
+-rw-r--r--   0        0        0     2231 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-spec/test_pyawkward_ListArrayU32_getitem_next_range_counts_64.py
+-rw-r--r--   0        0        0      391 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-spec/test_pyawkward_ListArrayU32_getitem_next_range_spreadadvanced_64.py
+-rw-r--r--   0        0        0     1377 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-spec/test_pyawkward_ListArrayU32_localindex_64.py
+-rw-r--r--   0        0        0     2379 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-spec/test_pyawkward_ListArrayU32_min_range.py
+-rw-r--r--   0        0        0     2700 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-spec/test_pyawkward_ListArrayU32_rpad_and_clip_length_axis1.py
+-rw-r--r--   0        0        0     4554 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-spec/test_pyawkward_ListArrayU32_rpad_axis1_64.py
+-rw-r--r--   0        0        0     1921 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-spec/test_pyawkward_ListArrayU32_validity.py
+-rw-r--r--   0        0        0     4327 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-spec/test_pyawkward_ListArray_fill_to64_from32.py
+-rw-r--r--   0        0        0     4327 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-spec/test_pyawkward_ListArray_fill_to64_from64.py
+-rw-r--r--   0        0        0     4337 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-spec/test_pyawkward_ListArray_fill_to64_fromU32.py
+-rw-r--r--   0        0        0     2715 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-spec/test_pyawkward_ListArray_getitem_jagged_carrylen_64.py
+-rw-r--r--   0        0        0      378 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-spec/test_pyawkward_ListArray_getitem_jagged_numvalid_64.py
+-rw-r--r--   0        0        0    20317 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-spec/test_pyawkward_ListArray_getitem_jagged_shrink_64.py
+-rw-r--r--   0        0        0     2399 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-spec/test_pyawkward_ListOffsetArray32_compact_offsets_64.py
+-rw-r--r--   0        0        0    15557 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-spec/test_pyawkward_ListOffsetArray32_flatten_offsets_64.py
+-rw-r--r--   0        0        0      382 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-spec/test_pyawkward_ListOffsetArray32_rpad_and_clip_axis1_64.py
+-rw-r--r--   0        0        0      373 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-spec/test_pyawkward_ListOffsetArray32_rpad_axis1_64.py
+-rw-r--r--   0        0        0      377 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-spec/test_pyawkward_ListOffsetArray32_rpad_length_axis1.py
+-rw-r--r--   0        0        0     2021 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-spec/test_pyawkward_ListOffsetArray32_toRegularArray.py
+-rw-r--r--   0        0        0     2399 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-spec/test_pyawkward_ListOffsetArray64_compact_offsets_64.py
+-rw-r--r--   0        0        0    15557 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-spec/test_pyawkward_ListOffsetArray64_flatten_offsets_64.py
+-rw-r--r--   0        0        0      382 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-spec/test_pyawkward_ListOffsetArray64_rpad_and_clip_axis1_64.py
+-rw-r--r--   0        0        0      373 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-spec/test_pyawkward_ListOffsetArray64_rpad_axis1_64.py
+-rw-r--r--   0        0        0      377 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-spec/test_pyawkward_ListOffsetArray64_rpad_length_axis1.py
+-rw-r--r--   0        0        0     2021 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-spec/test_pyawkward_ListOffsetArray64_toRegularArray.py
+-rw-r--r--   0        0        0     2409 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-spec/test_pyawkward_ListOffsetArrayU32_compact_offsets_64.py
+-rw-r--r--   0        0        0    15607 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-spec/test_pyawkward_ListOffsetArrayU32_flatten_offsets_64.py
+-rw-r--r--   0        0        0      383 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-spec/test_pyawkward_ListOffsetArrayU32_rpad_and_clip_axis1_64.py
+-rw-r--r--   0        0        0      374 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-spec/test_pyawkward_ListOffsetArrayU32_rpad_axis1_64.py
+-rw-r--r--   0        0        0      378 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-spec/test_pyawkward_ListOffsetArrayU32_rpad_length_axis1.py
+-rw-r--r--   0        0        0     2031 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-spec/test_pyawkward_ListOffsetArrayU32_toRegularArray.py
+-rw-r--r--   0        0        0    15112 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-spec/test_pyawkward_ListOffsetArray_drop_none_indexes_32.py
+-rw-r--r--   0        0        0    15112 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-spec/test_pyawkward_ListOffsetArray_drop_none_indexes_64.py
+-rw-r--r--   0        0        0      385 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-spec/test_pyawkward_ListOffsetArray_reduce_local_nextparents_64.py
+-rw-r--r--   0        0        0      384 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-spec/test_pyawkward_ListOffsetArray_reduce_local_outoffsets_64.py
+-rw-r--r--   0        0        0      397 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-spec/test_pyawkward_ListOffsetArray_reduce_nonlocal_maxcount_offsetscopy_64.py
+-rw-r--r--   0        0        0      387 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-spec/test_pyawkward_ListOffsetArray_reduce_nonlocal_nextshifts_64.py
+-rw-r--r--   0        0        0      387 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-spec/test_pyawkward_ListOffsetArray_reduce_nonlocal_nextstarts_64.py
+-rw-r--r--   0        0        0      391 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-spec/test_pyawkward_ListOffsetArray_reduce_nonlocal_outstartsstops_64.py
+-rw-r--r--   0        0        0    18832 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-spec/test_pyawkward_MaskedArray32_getitem_next_jagged_project.py
+-rw-r--r--   0        0        0    18832 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-spec/test_pyawkward_MaskedArray64_getitem_next_jagged_project.py
+-rw-r--r--   0        0        0    18882 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-spec/test_pyawkward_MaskedArrayU32_getitem_next_jagged_project.py
+-rw-r--r--   0        0        0      379 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-spec/test_pyawkward_NumpyArray_fill_tofloat32_fromfloat32.py
+-rw-r--r--   0        0        0      379 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-spec/test_pyawkward_NumpyArray_fill_tofloat32_fromfloat64.py
+-rw-r--r--   0        0        0      377 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-spec/test_pyawkward_NumpyArray_fill_tofloat32_fromint16.py
+-rw-r--r--   0        0        0      377 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-spec/test_pyawkward_NumpyArray_fill_tofloat32_fromint32.py
+-rw-r--r--   0        0        0      377 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-spec/test_pyawkward_NumpyArray_fill_tofloat32_fromint64.py
+-rw-r--r--   0        0        0      376 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-spec/test_pyawkward_NumpyArray_fill_tofloat32_fromint8.py
+-rw-r--r--   0        0        0      378 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-spec/test_pyawkward_NumpyArray_fill_tofloat32_fromuint16.py
+-rw-r--r--   0        0        0      378 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-spec/test_pyawkward_NumpyArray_fill_tofloat32_fromuint32.py
+-rw-r--r--   0        0        0      378 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-spec/test_pyawkward_NumpyArray_fill_tofloat32_fromuint64.py
+-rw-r--r--   0        0        0      377 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-spec/test_pyawkward_NumpyArray_fill_tofloat32_fromuint8.py
+-rw-r--r--   0        0        0      379 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-spec/test_pyawkward_NumpyArray_fill_tofloat64_fromfloat32.py
+-rw-r--r--   0        0        0      379 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-spec/test_pyawkward_NumpyArray_fill_tofloat64_fromfloat64.py
+-rw-r--r--   0        0        0      377 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-spec/test_pyawkward_NumpyArray_fill_tofloat64_fromint16.py
+-rw-r--r--   0        0        0      377 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-spec/test_pyawkward_NumpyArray_fill_tofloat64_fromint32.py
+-rw-r--r--   0        0        0      377 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-spec/test_pyawkward_NumpyArray_fill_tofloat64_fromint64.py
+-rw-r--r--   0        0        0      376 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-spec/test_pyawkward_NumpyArray_fill_tofloat64_fromint8.py
+-rw-r--r--   0        0        0      378 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-spec/test_pyawkward_NumpyArray_fill_tofloat64_fromuint16.py
+-rw-r--r--   0        0        0      378 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-spec/test_pyawkward_NumpyArray_fill_tofloat64_fromuint32.py
+-rw-r--r--   0        0        0      378 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-spec/test_pyawkward_NumpyArray_fill_tofloat64_fromuint64.py
+-rw-r--r--   0        0        0      377 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-spec/test_pyawkward_NumpyArray_fill_tofloat64_fromuint8.py
+-rw-r--r--   0        0        0      377 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-spec/test_pyawkward_NumpyArray_fill_toint16_fromfloat32.py
+-rw-r--r--   0        0        0      377 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-spec/test_pyawkward_NumpyArray_fill_toint16_fromfloat64.py
+-rw-r--r--   0        0        0      375 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-spec/test_pyawkward_NumpyArray_fill_toint16_fromint16.py
+-rw-r--r--   0        0        0      375 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-spec/test_pyawkward_NumpyArray_fill_toint16_fromint32.py
+-rw-r--r--   0        0        0      375 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-spec/test_pyawkward_NumpyArray_fill_toint16_fromint64.py
+-rw-r--r--   0        0        0      374 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-spec/test_pyawkward_NumpyArray_fill_toint16_fromint8.py
+-rw-r--r--   0        0        0      376 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-spec/test_pyawkward_NumpyArray_fill_toint16_fromuint16.py
+-rw-r--r--   0        0        0      376 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-spec/test_pyawkward_NumpyArray_fill_toint16_fromuint32.py
+-rw-r--r--   0        0        0      376 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-spec/test_pyawkward_NumpyArray_fill_toint16_fromuint64.py
+-rw-r--r--   0        0        0      375 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-spec/test_pyawkward_NumpyArray_fill_toint16_fromuint8.py
+-rw-r--r--   0        0        0      377 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-spec/test_pyawkward_NumpyArray_fill_toint32_fromfloat32.py
+-rw-r--r--   0        0        0      377 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-spec/test_pyawkward_NumpyArray_fill_toint32_fromfloat64.py
+-rw-r--r--   0        0        0      375 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-spec/test_pyawkward_NumpyArray_fill_toint32_fromint16.py
+-rw-r--r--   0        0        0      375 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-spec/test_pyawkward_NumpyArray_fill_toint32_fromint32.py
+-rw-r--r--   0        0        0      375 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-spec/test_pyawkward_NumpyArray_fill_toint32_fromint64.py
+-rw-r--r--   0        0        0      374 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-spec/test_pyawkward_NumpyArray_fill_toint32_fromint8.py
+-rw-r--r--   0        0        0      376 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-spec/test_pyawkward_NumpyArray_fill_toint32_fromuint16.py
+-rw-r--r--   0        0        0      376 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-spec/test_pyawkward_NumpyArray_fill_toint32_fromuint32.py
+-rw-r--r--   0        0        0      376 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-spec/test_pyawkward_NumpyArray_fill_toint32_fromuint64.py
+-rw-r--r--   0        0        0      375 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-spec/test_pyawkward_NumpyArray_fill_toint32_fromuint8.py
+-rw-r--r--   0        0        0      377 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-spec/test_pyawkward_NumpyArray_fill_toint64_fromfloat32.py
+-rw-r--r--   0        0        0      377 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-spec/test_pyawkward_NumpyArray_fill_toint64_fromfloat64.py
+-rw-r--r--   0        0        0      375 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-spec/test_pyawkward_NumpyArray_fill_toint64_fromint16.py
+-rw-r--r--   0        0        0      375 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-spec/test_pyawkward_NumpyArray_fill_toint64_fromint32.py
+-rw-r--r--   0        0        0      375 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-spec/test_pyawkward_NumpyArray_fill_toint64_fromint64.py
+-rw-r--r--   0        0        0      374 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-spec/test_pyawkward_NumpyArray_fill_toint64_fromint8.py
+-rw-r--r--   0        0        0      376 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-spec/test_pyawkward_NumpyArray_fill_toint64_fromuint16.py
+-rw-r--r--   0        0        0      376 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-spec/test_pyawkward_NumpyArray_fill_toint64_fromuint32.py
+-rw-r--r--   0        0        0      376 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-spec/test_pyawkward_NumpyArray_fill_toint64_fromuint64.py
+-rw-r--r--   0        0        0      375 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-spec/test_pyawkward_NumpyArray_fill_toint64_fromuint8.py
+-rw-r--r--   0        0        0      376 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-spec/test_pyawkward_NumpyArray_fill_toint8_fromfloat32.py
+-rw-r--r--   0        0        0      376 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-spec/test_pyawkward_NumpyArray_fill_toint8_fromfloat64.py
+-rw-r--r--   0        0        0      374 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-spec/test_pyawkward_NumpyArray_fill_toint8_fromint16.py
+-rw-r--r--   0        0        0      374 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-spec/test_pyawkward_NumpyArray_fill_toint8_fromint32.py
+-rw-r--r--   0        0        0      374 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-spec/test_pyawkward_NumpyArray_fill_toint8_fromint64.py
+-rw-r--r--   0        0        0      373 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-spec/test_pyawkward_NumpyArray_fill_toint8_fromint8.py
+-rw-r--r--   0        0        0      375 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-spec/test_pyawkward_NumpyArray_fill_toint8_fromuint16.py
+-rw-r--r--   0        0        0      375 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-spec/test_pyawkward_NumpyArray_fill_toint8_fromuint32.py
+-rw-r--r--   0        0        0      375 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-spec/test_pyawkward_NumpyArray_fill_toint8_fromuint64.py
+-rw-r--r--   0        0        0      374 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-spec/test_pyawkward_NumpyArray_fill_toint8_fromuint8.py
+-rw-r--r--   0        0        0      378 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-spec/test_pyawkward_NumpyArray_fill_touint16_fromfloat32.py
+-rw-r--r--   0        0        0      378 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-spec/test_pyawkward_NumpyArray_fill_touint16_fromfloat64.py
+-rw-r--r--   0        0        0      376 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-spec/test_pyawkward_NumpyArray_fill_touint16_fromint16.py
+-rw-r--r--   0        0        0      376 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-spec/test_pyawkward_NumpyArray_fill_touint16_fromint32.py
+-rw-r--r--   0        0        0      376 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-spec/test_pyawkward_NumpyArray_fill_touint16_fromint64.py
+-rw-r--r--   0        0        0      375 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-spec/test_pyawkward_NumpyArray_fill_touint16_fromint8.py
+-rw-r--r--   0        0        0      377 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-spec/test_pyawkward_NumpyArray_fill_touint16_fromuint16.py
+-rw-r--r--   0        0        0      377 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-spec/test_pyawkward_NumpyArray_fill_touint16_fromuint32.py
+-rw-r--r--   0        0        0      377 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-spec/test_pyawkward_NumpyArray_fill_touint16_fromuint64.py
+-rw-r--r--   0        0        0      376 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-spec/test_pyawkward_NumpyArray_fill_touint16_fromuint8.py
+-rw-r--r--   0        0        0      378 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-spec/test_pyawkward_NumpyArray_fill_touint32_fromfloat32.py
+-rw-r--r--   0        0        0      378 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-spec/test_pyawkward_NumpyArray_fill_touint32_fromfloat64.py
+-rw-r--r--   0        0        0      376 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-spec/test_pyawkward_NumpyArray_fill_touint32_fromint16.py
+-rw-r--r--   0        0        0      376 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-spec/test_pyawkward_NumpyArray_fill_touint32_fromint32.py
+-rw-r--r--   0        0        0      376 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-spec/test_pyawkward_NumpyArray_fill_touint32_fromint64.py
+-rw-r--r--   0        0        0      375 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-spec/test_pyawkward_NumpyArray_fill_touint32_fromint8.py
+-rw-r--r--   0        0        0      377 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-spec/test_pyawkward_NumpyArray_fill_touint32_fromuint16.py
+-rw-r--r--   0        0        0      377 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-spec/test_pyawkward_NumpyArray_fill_touint32_fromuint32.py
+-rw-r--r--   0        0        0      377 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-spec/test_pyawkward_NumpyArray_fill_touint32_fromuint64.py
+-rw-r--r--   0        0        0      376 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-spec/test_pyawkward_NumpyArray_fill_touint32_fromuint8.py
+-rw-r--r--   0        0        0      378 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-spec/test_pyawkward_NumpyArray_fill_touint64_fromfloat32.py
+-rw-r--r--   0        0        0      378 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-spec/test_pyawkward_NumpyArray_fill_touint64_fromfloat64.py
+-rw-r--r--   0        0        0      376 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-spec/test_pyawkward_NumpyArray_fill_touint64_fromint16.py
+-rw-r--r--   0        0        0      376 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-spec/test_pyawkward_NumpyArray_fill_touint64_fromint32.py
+-rw-r--r--   0        0        0      376 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-spec/test_pyawkward_NumpyArray_fill_touint64_fromint64.py
+-rw-r--r--   0        0        0      375 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-spec/test_pyawkward_NumpyArray_fill_touint64_fromint8.py
+-rw-r--r--   0        0        0      377 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-spec/test_pyawkward_NumpyArray_fill_touint64_fromuint16.py
+-rw-r--r--   0        0        0      377 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-spec/test_pyawkward_NumpyArray_fill_touint64_fromuint32.py
+-rw-r--r--   0        0        0      377 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-spec/test_pyawkward_NumpyArray_fill_touint64_fromuint64.py
+-rw-r--r--   0        0        0      376 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-spec/test_pyawkward_NumpyArray_fill_touint64_fromuint8.py
+-rw-r--r--   0        0        0      377 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-spec/test_pyawkward_NumpyArray_fill_touint8_fromfloat32.py
+-rw-r--r--   0        0        0      377 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-spec/test_pyawkward_NumpyArray_fill_touint8_fromfloat64.py
+-rw-r--r--   0        0        0      375 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-spec/test_pyawkward_NumpyArray_fill_touint8_fromint16.py
+-rw-r--r--   0        0        0      375 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-spec/test_pyawkward_NumpyArray_fill_touint8_fromint32.py
+-rw-r--r--   0        0        0      375 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-spec/test_pyawkward_NumpyArray_fill_touint8_fromint64.py
+-rw-r--r--   0        0        0      374 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-spec/test_pyawkward_NumpyArray_fill_touint8_fromint8.py
+-rw-r--r--   0        0        0      376 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-spec/test_pyawkward_NumpyArray_fill_touint8_fromuint16.py
+-rw-r--r--   0        0        0      376 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-spec/test_pyawkward_NumpyArray_fill_touint8_fromuint32.py
+-rw-r--r--   0        0        0      376 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-spec/test_pyawkward_NumpyArray_fill_touint8_fromuint64.py
+-rw-r--r--   0        0        0      375 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-spec/test_pyawkward_NumpyArray_fill_touint8_fromuint8.py
+-rw-r--r--   0        0        0      388 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-spec/test_pyawkward_NumpyArray_rearrange_shifted_toint64_fromint64.py
+-rw-r--r--   0        0        0      376 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-spec/test_pyawkward_NumpyArray_reduce_adjust_starts_64.py
+-rw-r--r--   0        0        0      383 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-spec/test_pyawkward_NumpyArray_reduce_adjust_starts_shifts_64.py
+-rw-r--r--   0        0        0      383 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-spec/test_pyawkward_NumpyArray_reduce_mask_ByteMaskedArray_64.py
+-rw-r--r--   0        0        0     8909 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-spec/test_pyawkward_RegularArray_broadcast_tooffsets_64.py
+-rw-r--r--   0        0        0      614 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-spec/test_pyawkward_RegularArray_broadcast_tooffsets_size1_64.py
+-rw-r--r--   0        0        0     2011 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-spec/test_pyawkward_RegularArray_compact_offsets64.py
+-rw-r--r--   0        0        0     9307 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-spec/test_pyawkward_RegularArray_getitem_carry_64.py
+-rw-r--r--   0        0        0    15083 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-spec/test_pyawkward_RegularArray_getitem_jagged_expand_64.py
+-rw-r--r--   0        0        0    18712 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-spec/test_pyawkward_RegularArray_getitem_next_array_64.py
+-rw-r--r--   0        0        0    94644 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-spec/test_pyawkward_RegularArray_getitem_next_array_advanced_64.py
+-rw-r--r--   0        0        0    10596 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-spec/test_pyawkward_RegularArray_getitem_next_array_regularize_64.py
+-rw-r--r--   0        0        0     1636 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-spec/test_pyawkward_RegularArray_getitem_next_at_64.py
+-rw-r--r--   0        0        0      691 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-spec/test_pyawkward_RegularArray_getitem_next_range_64.py
+-rw-r--r--   0        0        0    10823 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-spec/test_pyawkward_RegularArray_getitem_next_range_spreadadvanced_64.py
+-rw-r--r--   0        0        0     1620 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-spec/test_pyawkward_RegularArray_localindex_64.py
+-rw-r--r--   0        0        0      382 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-spec/test_pyawkward_RegularArray_reduce_local_nextparents_64.py
+-rw-r--r--   0        0        0      385 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-spec/test_pyawkward_RegularArray_reduce_nonlocal_preparenext_64.py
+-rw-r--r--   0        0        0      609 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-spec/test_pyawkward_RegularArray_rpad_and_clip_axis1_64.py
+-rw-r--r--   0        0        0      373 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-spec/test_pyawkward_UnionArray32_flatten_combine_64.py
+-rw-r--r--   0        0        0      372 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-spec/test_pyawkward_UnionArray32_flatten_length_64.py
+-rw-r--r--   0        0        0      373 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-spec/test_pyawkward_UnionArray64_flatten_combine_64.py
+-rw-r--r--   0        0        0      372 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-spec/test_pyawkward_UnionArray64_flatten_length_64.py
+-rw-r--r--   0        0        0      381 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-spec/test_pyawkward_UnionArray8_32_nestedfill_tags_index_64.py
+-rw-r--r--   0        0        0     9557 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-spec/test_pyawkward_UnionArray8_32_project_64.py
+-rw-r--r--   0        0        0     3092 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-spec/test_pyawkward_UnionArray8_32_regular_index.py
+-rw-r--r--   0        0        0   486418 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-spec/test_pyawkward_UnionArray8_32_simplify8_32_to8_64.py
+-rw-r--r--   0        0        0   486418 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-spec/test_pyawkward_UnionArray8_32_simplify8_64_to8_64.py
+-rw-r--r--   0        0        0   487418 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-spec/test_pyawkward_UnionArray8_32_simplify8_U32_to8_64.py
+-rw-r--r--   0        0        0    11282 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-spec/test_pyawkward_UnionArray8_32_simplify_one_to8_64.py
+-rw-r--r--   0        0        0    58126 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-spec/test_pyawkward_UnionArray8_32_validity.py
+-rw-r--r--   0        0        0      381 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-spec/test_pyawkward_UnionArray8_64_nestedfill_tags_index_64.py
+-rw-r--r--   0        0        0     9557 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-spec/test_pyawkward_UnionArray8_64_project_64.py
+-rw-r--r--   0        0        0     3092 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-spec/test_pyawkward_UnionArray8_64_regular_index.py
+-rw-r--r--   0        0        0   486418 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-spec/test_pyawkward_UnionArray8_64_simplify8_32_to8_64.py
+-rw-r--r--   0        0        0   486418 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-spec/test_pyawkward_UnionArray8_64_simplify8_64_to8_64.py
+-rw-r--r--   0        0        0   487418 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-spec/test_pyawkward_UnionArray8_64_simplify8_U32_to8_64.py
+-rw-r--r--   0        0        0    11282 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-spec/test_pyawkward_UnionArray8_64_simplify_one_to8_64.py
+-rw-r--r--   0        0        0    58126 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-spec/test_pyawkward_UnionArray8_64_validity.py
+-rw-r--r--   0        0        0      382 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-spec/test_pyawkward_UnionArray8_U32_nestedfill_tags_index_64.py
+-rw-r--r--   0        0        0     9587 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-spec/test_pyawkward_UnionArray8_U32_project_64.py
+-rw-r--r--   0        0        0     3102 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-spec/test_pyawkward_UnionArray8_U32_regular_index.py
+-rw-r--r--   0        0        0   487418 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-spec/test_pyawkward_UnionArray8_U32_simplify8_32_to8_64.py
+-rw-r--r--   0        0        0   487418 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-spec/test_pyawkward_UnionArray8_U32_simplify8_64_to8_64.py
+-rw-r--r--   0        0        0   488418 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-spec/test_pyawkward_UnionArray8_U32_simplify8_U32_to8_64.py
+-rw-r--r--   0        0        0    11312 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-spec/test_pyawkward_UnionArray8_U32_simplify_one_to8_64.py
+-rw-r--r--   0        0        0    58376 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-spec/test_pyawkward_UnionArray8_U32_validity.py
+-rw-r--r--   0        0        0     2077 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-spec/test_pyawkward_UnionArray8_regular_index_getsize.py
+-rw-r--r--   0        0        0      374 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-spec/test_pyawkward_UnionArrayU32_flatten_combine_64.py
+-rw-r--r--   0        0        0      373 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-spec/test_pyawkward_UnionArrayU32_flatten_length_64.py
+-rw-r--r--   0        0        0      586 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-spec/test_pyawkward_UnionArray_fillindex_to64_count.py
+-rw-r--r--   0        0        0     2621 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-spec/test_pyawkward_UnionArray_fillindex_to64_from32.py
+-rw-r--r--   0        0        0     2621 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-spec/test_pyawkward_UnionArray_fillindex_to64_from64.py
+-rw-r--r--   0        0        0     2631 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-spec/test_pyawkward_UnionArray_fillindex_to64_fromU32.py
+-rw-r--r--   0        0        0     2156 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-spec/test_pyawkward_UnionArray_fillna_from32_to64.py
+-rw-r--r--   0        0        0     2156 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-spec/test_pyawkward_UnionArray_fillna_from64_to64.py
+-rw-r--r--   0        0        0     2166 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-spec/test_pyawkward_UnionArray_fillna_fromU32_to64.py
+-rw-r--r--   0        0        0      596 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-spec/test_pyawkward_UnionArray_filltags_to8_const.py
+-rw-r--r--   0        0        0     2727 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-spec/test_pyawkward_UnionArray_filltags_to8_from8.py
+-rw-r--r--   0        0        0      523 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-spec/test_pyawkward_index_rpad_and_clip_axis0_64.py
+-rw-r--r--   0        0        0      682 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-spec/test_pyawkward_index_rpad_and_clip_axis1_64.py
+-rw-r--r--   0        0        0      463 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-spec/test_pyawkward_localindex_64.py
+-rw-r--r--   0        0        0    13193 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-spec/test_pyawkward_missing_repeat_64.py
+-rw-r--r--   0        0        0      366 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-spec/test_pyawkward_reduce_argmax_float32_64.py
+-rw-r--r--   0        0        0      366 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-spec/test_pyawkward_reduce_argmax_float64_64.py
+-rw-r--r--   0        0        0      364 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-spec/test_pyawkward_reduce_argmax_int16_64.py
+-rw-r--r--   0        0        0      364 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-spec/test_pyawkward_reduce_argmax_int32_64.py
+-rw-r--r--   0        0        0      364 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-spec/test_pyawkward_reduce_argmax_int64_64.py
+-rw-r--r--   0        0        0      363 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-spec/test_pyawkward_reduce_argmax_int8_64.py
+-rw-r--r--   0        0        0      365 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-spec/test_pyawkward_reduce_argmax_uint16_64.py
+-rw-r--r--   0        0        0      365 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-spec/test_pyawkward_reduce_argmax_uint32_64.py
+-rw-r--r--   0        0        0      365 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-spec/test_pyawkward_reduce_argmax_uint64_64.py
+-rw-r--r--   0        0        0      364 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-spec/test_pyawkward_reduce_argmax_uint8_64.py
+-rw-r--r--   0        0        0      366 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-spec/test_pyawkward_reduce_argmin_float32_64.py
+-rw-r--r--   0        0        0      366 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-spec/test_pyawkward_reduce_argmin_float64_64.py
+-rw-r--r--   0        0        0      364 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-spec/test_pyawkward_reduce_argmin_int16_64.py
+-rw-r--r--   0        0        0      364 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-spec/test_pyawkward_reduce_argmin_int32_64.py
+-rw-r--r--   0        0        0      364 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-spec/test_pyawkward_reduce_argmin_int64_64.py
+-rw-r--r--   0        0        0      363 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-spec/test_pyawkward_reduce_argmin_int8_64.py
+-rw-r--r--   0        0        0      365 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-spec/test_pyawkward_reduce_argmin_uint16_64.py
+-rw-r--r--   0        0        0      365 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-spec/test_pyawkward_reduce_argmin_uint32_64.py
+-rw-r--r--   0        0        0      365 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-spec/test_pyawkward_reduce_argmin_uint64_64.py
+-rw-r--r--   0        0        0      364 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-spec/test_pyawkward_reduce_argmin_uint8_64.py
+-rw-r--r--   0        0        0      357 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-spec/test_pyawkward_reduce_count_64.py
+-rw-r--r--   0        0        0      369 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-spec/test_pyawkward_reduce_countnonzero_bool_64.py
+-rw-r--r--   0        0        0      372 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-spec/test_pyawkward_reduce_countnonzero_float32_64.py
+-rw-r--r--   0        0        0      372 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-spec/test_pyawkward_reduce_countnonzero_float64_64.py
+-rw-r--r--   0        0        0      370 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-spec/test_pyawkward_reduce_countnonzero_int16_64.py
+-rw-r--r--   0        0        0      370 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-spec/test_pyawkward_reduce_countnonzero_int32_64.py
+-rw-r--r--   0        0        0      370 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-spec/test_pyawkward_reduce_countnonzero_int64_64.py
+-rw-r--r--   0        0        0      369 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-spec/test_pyawkward_reduce_countnonzero_int8_64.py
+-rw-r--r--   0        0        0      371 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-spec/test_pyawkward_reduce_countnonzero_uint16_64.py
+-rw-r--r--   0        0        0      371 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-spec/test_pyawkward_reduce_countnonzero_uint32_64.py
+-rw-r--r--   0        0        0      371 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-spec/test_pyawkward_reduce_countnonzero_uint64_64.py
+-rw-r--r--   0        0        0      370 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-spec/test_pyawkward_reduce_countnonzero_uint8_64.py
+-rw-r--r--   0        0        0      371 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-spec/test_pyawkward_reduce_max_float32_float32_64.py
+-rw-r--r--   0        0        0      371 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-spec/test_pyawkward_reduce_max_float64_float64_64.py
+-rw-r--r--   0        0        0      367 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-spec/test_pyawkward_reduce_max_int16_int16_64.py
+-rw-r--r--   0        0        0      367 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-spec/test_pyawkward_reduce_max_int32_int32_64.py
+-rw-r--r--   0        0        0      367 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-spec/test_pyawkward_reduce_max_int64_int64_64.py
+-rw-r--r--   0        0        0      365 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-spec/test_pyawkward_reduce_max_int8_int8_64.py
+-rw-r--r--   0        0        0      369 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-spec/test_pyawkward_reduce_max_uint16_uint16_64.py
+-rw-r--r--   0        0        0      369 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-spec/test_pyawkward_reduce_max_uint32_uint32_64.py
+-rw-r--r--   0        0        0      369 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-spec/test_pyawkward_reduce_max_uint64_uint64_64.py
+-rw-r--r--   0        0        0      367 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-spec/test_pyawkward_reduce_max_uint8_uint8_64.py
+-rw-r--r--   0        0        0      371 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-spec/test_pyawkward_reduce_min_float32_float32_64.py
+-rw-r--r--   0        0        0      371 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-spec/test_pyawkward_reduce_min_float64_float64_64.py
+-rw-r--r--   0        0        0      367 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-spec/test_pyawkward_reduce_min_int16_int16_64.py
+-rw-r--r--   0        0        0      367 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-spec/test_pyawkward_reduce_min_int32_int32_64.py
+-rw-r--r--   0        0        0      367 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-spec/test_pyawkward_reduce_min_int64_int64_64.py
+-rw-r--r--   0        0        0      365 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-spec/test_pyawkward_reduce_min_int8_int8_64.py
+-rw-r--r--   0        0        0      369 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-spec/test_pyawkward_reduce_min_uint16_uint16_64.py
+-rw-r--r--   0        0        0      369 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-spec/test_pyawkward_reduce_min_uint32_uint32_64.py
+-rw-r--r--   0        0        0      369 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-spec/test_pyawkward_reduce_min_uint64_uint64_64.py
+-rw-r--r--   0        0        0      367 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-spec/test_pyawkward_reduce_min_uint8_uint8_64.py
+-rw-r--r--   0        0        0      366 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-spec/test_pyawkward_reduce_prod_bool_bool_64.py
+-rw-r--r--   0        0        0      369 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-spec/test_pyawkward_reduce_prod_bool_float32_64.py
+-rw-r--r--   0        0        0      369 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-spec/test_pyawkward_reduce_prod_bool_float64_64.py
+-rw-r--r--   0        0        0      367 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-spec/test_pyawkward_reduce_prod_bool_int16_64.py
+-rw-r--r--   0        0        0      367 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-spec/test_pyawkward_reduce_prod_bool_int32_64.py
+-rw-r--r--   0        0        0      367 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-spec/test_pyawkward_reduce_prod_bool_int64_64.py
+-rw-r--r--   0        0        0      366 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-spec/test_pyawkward_reduce_prod_bool_int8_64.py
+-rw-r--r--   0        0        0      368 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-spec/test_pyawkward_reduce_prod_bool_uint16_64.py
+-rw-r--r--   0        0        0      368 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-spec/test_pyawkward_reduce_prod_bool_uint32_64.py
+-rw-r--r--   0        0        0      368 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-spec/test_pyawkward_reduce_prod_bool_uint64_64.py
+-rw-r--r--   0        0        0      367 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-spec/test_pyawkward_reduce_prod_bool_uint8_64.py
+-rw-r--r--   0        0        0      372 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-spec/test_pyawkward_reduce_prod_float32_float32_64.py
+-rw-r--r--   0        0        0      372 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-spec/test_pyawkward_reduce_prod_float64_float64_64.py
+-rw-r--r--   0        0        0      368 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-spec/test_pyawkward_reduce_prod_int32_int16_64.py
+-rw-r--r--   0        0        0      368 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-spec/test_pyawkward_reduce_prod_int32_int32_64.py
+-rw-r--r--   0        0        0      367 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-spec/test_pyawkward_reduce_prod_int32_int8_64.py
+-rw-r--r--   0        0        0      368 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-spec/test_pyawkward_reduce_prod_int64_int16_64.py
+-rw-r--r--   0        0        0      368 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-spec/test_pyawkward_reduce_prod_int64_int32_64.py
+-rw-r--r--   0        0        0      368 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-spec/test_pyawkward_reduce_prod_int64_int64_64.py
+-rw-r--r--   0        0        0      367 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-spec/test_pyawkward_reduce_prod_int64_int8_64.py
+-rw-r--r--   0        0        0      370 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-spec/test_pyawkward_reduce_prod_uint32_uint16_64.py
+-rw-r--r--   0        0        0      370 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-spec/test_pyawkward_reduce_prod_uint32_uint32_64.py
+-rw-r--r--   0        0        0      369 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-spec/test_pyawkward_reduce_prod_uint32_uint8_64.py
+-rw-r--r--   0        0        0      370 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-spec/test_pyawkward_reduce_prod_uint64_uint16_64.py
+-rw-r--r--   0        0        0      370 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-spec/test_pyawkward_reduce_prod_uint64_uint32_64.py
+-rw-r--r--   0        0        0      370 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-spec/test_pyawkward_reduce_prod_uint64_uint64_64.py
+-rw-r--r--   0        0        0      369 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-spec/test_pyawkward_reduce_prod_uint64_uint8_64.py
+-rw-r--r--   0        0        0      365 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-spec/test_pyawkward_reduce_sum_bool_bool_64.py
+-rw-r--r--   0        0        0      368 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-spec/test_pyawkward_reduce_sum_bool_float32_64.py
+-rw-r--r--   0        0        0      368 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-spec/test_pyawkward_reduce_sum_bool_float64_64.py
+-rw-r--r--   0        0        0      366 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-spec/test_pyawkward_reduce_sum_bool_int16_64.py
+-rw-r--r--   0        0        0      366 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-spec/test_pyawkward_reduce_sum_bool_int32_64.py
+-rw-r--r--   0        0        0      366 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-spec/test_pyawkward_reduce_sum_bool_int64_64.py
+-rw-r--r--   0        0        0      365 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-spec/test_pyawkward_reduce_sum_bool_int8_64.py
+-rw-r--r--   0        0        0      367 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-spec/test_pyawkward_reduce_sum_bool_uint16_64.py
+-rw-r--r--   0        0        0      367 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-spec/test_pyawkward_reduce_sum_bool_uint32_64.py
+-rw-r--r--   0        0        0      367 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-spec/test_pyawkward_reduce_sum_bool_uint64_64.py
+-rw-r--r--   0        0        0      366 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-spec/test_pyawkward_reduce_sum_bool_uint8_64.py
+-rw-r--r--   0        0        0      371 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-spec/test_pyawkward_reduce_sum_float32_float32_64.py
+-rw-r--r--   0        0        0      371 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-spec/test_pyawkward_reduce_sum_float64_float64_64.py
+-rw-r--r--   0        0        0      366 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-spec/test_pyawkward_reduce_sum_int32_bool_64.py
+-rw-r--r--   0        0        0      367 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-spec/test_pyawkward_reduce_sum_int32_int16_64.py
+-rw-r--r--   0        0        0      367 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-spec/test_pyawkward_reduce_sum_int32_int32_64.py
+-rw-r--r--   0        0        0      366 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-spec/test_pyawkward_reduce_sum_int32_int8_64.py
+-rw-r--r--   0        0        0      366 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-spec/test_pyawkward_reduce_sum_int64_bool_64.py
+-rw-r--r--   0        0        0      367 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-spec/test_pyawkward_reduce_sum_int64_int16_64.py
+-rw-r--r--   0        0        0      367 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-spec/test_pyawkward_reduce_sum_int64_int32_64.py
+-rw-r--r--   0        0        0      367 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-spec/test_pyawkward_reduce_sum_int64_int64_64.py
+-rw-r--r--   0        0        0      366 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-spec/test_pyawkward_reduce_sum_int64_int8_64.py
+-rw-r--r--   0        0        0      369 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-spec/test_pyawkward_reduce_sum_uint32_uint16_64.py
+-rw-r--r--   0        0        0      369 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-spec/test_pyawkward_reduce_sum_uint32_uint32_64.py
+-rw-r--r--   0        0        0      368 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-spec/test_pyawkward_reduce_sum_uint32_uint8_64.py
+-rw-r--r--   0        0        0      369 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-spec/test_pyawkward_reduce_sum_uint64_uint16_64.py
+-rw-r--r--   0        0        0      369 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-spec/test_pyawkward_reduce_sum_uint64_uint32_64.py
+-rw-r--r--   0        0        0      369 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-spec/test_pyawkward_reduce_sum_uint64_uint64_64.py
+-rw-r--r--   0        0        0      368 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-spec/test_pyawkward_reduce_sum_uint64_uint8_64.py
+-rw-r--r--   0        0        0    78359 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-spec-explicit/kernels.py
+-rw-r--r--   0        0        0     1607 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-spec-explicit/test_awkward_BitMaskedArray_to_ByteMaskedArray.py
+-rw-r--r--   0        0        0     1125 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-spec-explicit/test_awkward_BitMaskedArray_to_IndexedOptionArray.py
+-rw-r--r--   0        0        0      715 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-spec-explicit/test_awkward_ByteMaskedArray_getitem_nextcarry.py
+-rw-r--r--   0        0        0      976 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-spec-explicit/test_awkward_ByteMaskedArray_getitem_nextcarry_outindex.py
+-rw-r--r--   0        0        0     5606 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-spec-explicit/test_awkward_ByteMaskedArray_numnull.py
+-rw-r--r--   0        0        0      396 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-spec-explicit/test_awkward_ByteMaskedArray_overlay_mask.py
+-rw-r--r--   0        0        0      458 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-spec-explicit/test_awkward_ByteMaskedArray_reduce_next_nonlocal_nextshifts_64.py
+-rw-r--r--   0        0        0      732 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-spec-explicit/test_awkward_ByteMaskedArray_toIndexedOptionArray.py
+-rw-r--r--   0        0        0    16520 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-spec-explicit/test_awkward_Content_getitem_next_missing_jagged_getmaskstartstop.py
+-rw-r--r--   0        0        0     1944 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-spec-explicit/test_awkward_IndexedArray_fill.py
+-rw-r--r--   0        0        0      378 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-spec-explicit/test_awkward_IndexedArray_flatten_nextcarry.py
+-rw-r--r--   0        0        0     3461 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-spec-explicit/test_awkward_IndexedArray_flatten_none2empty.py
+-rw-r--r--   0        0        0    10018 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-spec-explicit/test_awkward_IndexedArray_getitem_nextcarry.py
+-rw-r--r--   0        0        0     1036 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-spec-explicit/test_awkward_IndexedArray_getitem_nextcarry_outindex.py
+-rw-r--r--   0        0        0     4574 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-spec-explicit/test_awkward_IndexedArray_index_of_nulls.py
+-rw-r--r--   0        0        0     3746 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-spec-explicit/test_awkward_IndexedArray_numnull.py
+-rw-r--r--   0        0        0     6792 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-spec-explicit/test_awkward_IndexedArray_reduce_next_64.py
+-rw-r--r--   0        0        0     2890 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-spec-explicit/test_awkward_IndexedArray_reduce_next_fix_offsets_64.py
+-rw-r--r--   0        0        0     3921 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-spec-explicit/test_awkward_IndexedArray_reduce_next_nonlocal_nextshifts_64.py
+-rw-r--r--   0        0        0     2570 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-spec-explicit/test_awkward_IndexedArray_reduce_next_nonlocal_nextshifts_fromshifts_64.py
+-rw-r--r--   0        0        0    15064 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-spec-explicit/test_awkward_IndexedArray_simplify.py
+-rw-r--r--   0        0        0     9994 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-spec-explicit/test_awkward_IndexedArray_validity.py
+-rw-r--r--   0        0        0      377 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-spec-explicit/test_awkward_IndexedOptionArray_rpad_and_clip_mask_axis1.py
+-rw-r--r--   0        0        0    57215 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-spec-explicit/test_awkward_ListArray_broadcast_tooffsets.py
+-rw-r--r--   0        0        0     3776 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-spec-explicit/test_awkward_ListArray_combinations_length.py
+-rw-r--r--   0        0        0    32221 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-spec-explicit/test_awkward_ListArray_compact_offsets.py
+-rw-r--r--   0        0        0     5715 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-spec-explicit/test_awkward_ListArray_fill.py
+-rw-r--r--   0        0        0    18763 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-spec-explicit/test_awkward_ListArray_getitem_jagged_apply.py
+-rw-r--r--   0        0        0    13720 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-spec-explicit/test_awkward_ListArray_getitem_jagged_carrylen.py
+-rw-r--r--   0        0        0     2030 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-spec-explicit/test_awkward_ListArray_getitem_jagged_descend.py
+-rw-r--r--   0        0        0     1444 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-spec-explicit/test_awkward_ListArray_getitem_jagged_expand.py
+-rw-r--r--   0        0        0     3592 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-spec-explicit/test_awkward_ListArray_getitem_jagged_shrink.py
+-rw-r--r--   0        0        0     3161 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-spec-explicit/test_awkward_ListArray_getitem_next_array.py
+-rw-r--r--   0        0        0    31580 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-spec-explicit/test_awkward_ListArray_getitem_next_array_advanced.py
+-rw-r--r--   0        0        0    18191 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-spec-explicit/test_awkward_ListArray_getitem_next_at.py
+-rw-r--r--   0        0        0      683 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-spec-explicit/test_awkward_ListArray_getitem_next_range_counts.py
+-rw-r--r--   0        0        0     3572 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-spec-explicit/test_awkward_ListArray_localindex.py
+-rw-r--r--   0        0        0     1342 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-spec-explicit/test_awkward_ListArray_min_range.py
+-rw-r--r--   0        0        0     4352 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-spec-explicit/test_awkward_ListArray_rpad_and_clip_length_axis1.py
+-rw-r--r--   0        0        0     7944 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-spec-explicit/test_awkward_ListArray_rpad_axis1.py
+-rw-r--r--   0        0        0    16024 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-spec-explicit/test_awkward_ListArray_validity.py
+-rw-r--r--   0        0        0     3089 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-spec-explicit/test_awkward_ListOffsetArray_compact_offsets.py
+-rw-r--r--   0        0        0    14322 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-spec-explicit/test_awkward_ListOffsetArray_flatten_offsets.py
+-rw-r--r--   0        0        0     8553 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-spec-explicit/test_awkward_ListOffsetArray_reduce_local_outoffsets_64.py
+-rw-r--r--   0        0        0    16999 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-spec-explicit/test_awkward_ListOffsetArray_reduce_nonlocal_maxcount_offsetscopy_64.py
+-rw-r--r--   0        0        0    32915 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-spec-explicit/test_awkward_ListOffsetArray_reduce_nonlocal_nextshifts_64.py
+-rw-r--r--   0        0        0    13774 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-spec-explicit/test_awkward_ListOffsetArray_reduce_nonlocal_nextstarts_64.py
+-rw-r--r--   0        0        0    12662 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-spec-explicit/test_awkward_ListOffsetArray_reduce_nonlocal_outstartsstops_64.py
+-rw-r--r--   0        0        0     1564 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-spec-explicit/test_awkward_ListOffsetArray_toRegularArray.py
+-rw-r--r--   0        0        0     2302 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-spec-explicit/test_awkward_MaskedArray_getitem_next_jagged_project.py
+-rw-r--r--   0        0        0    14407 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-spec-explicit/test_awkward_NumpyArray_reduce_mask_ByteMaskedArray_64.py
+-rw-r--r--   0        0        0     2252 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-spec-explicit/test_awkward_RegularArray_broadcast_tooffsets.py
+-rw-r--r--   0        0        0     7393 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-spec-explicit/test_awkward_RegularArray_broadcast_tooffsets_size1.py
+-rw-r--r--   0        0        0     3951 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-spec-explicit/test_awkward_RegularArray_compact_offsets.py
+-rw-r--r--   0        0        0    19963 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-spec-explicit/test_awkward_RegularArray_getitem_carry.py
+-rw-r--r--   0        0        0    16442 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-spec-explicit/test_awkward_RegularArray_getitem_jagged_expand.py
+-rw-r--r--   0        0        0    43829 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-spec-explicit/test_awkward_RegularArray_getitem_next_array.py
+-rw-r--r--   0        0        0     8314 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-spec-explicit/test_awkward_RegularArray_getitem_next_array_advanced.py
+-rw-r--r--   0        0        0    29046 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-spec-explicit/test_awkward_RegularArray_getitem_next_array_regularize.py
+-rw-r--r--   0        0        0     6099 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-spec-explicit/test_awkward_RegularArray_getitem_next_at.py
+-rw-r--r--   0        0        0    21666 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-spec-explicit/test_awkward_RegularArray_getitem_next_range.py
+-rw-r--r--   0        0        0      833 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-spec-explicit/test_awkward_RegularArray_getitem_next_range_spreadadvanced.py
+-rw-r--r--   0        0        0      822 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-spec-explicit/test_awkward_RegularArray_localindex.py
+-rw-r--r--   0        0        0     2484 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-spec-explicit/test_awkward_RegularArray_rpad_and_clip_axis1.py
+-rw-r--r--   0        0        0      758 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-spec-explicit/test_awkward_UnionArray_fillindex.py
+-rw-r--r--   0        0        0     2786 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-spec-explicit/test_awkward_UnionArray_fillindex_count.py
+-rw-r--r--   0        0        0     4269 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-spec-explicit/test_awkward_UnionArray_fillna.py
+-rw-r--r--   0        0        0      413 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-spec-explicit/test_awkward_UnionArray_filltags.py
+-rw-r--r--   0        0        0     5215 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-spec-explicit/test_awkward_UnionArray_project.py
+-rw-r--r--   0        0        0     1386 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-spec-explicit/test_awkward_UnionArray_regular_index.py
+-rw-r--r--   0        0        0      897 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-spec-explicit/test_awkward_UnionArray_regular_index_getsize.py
+-rw-r--r--   0        0        0     1876 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-spec-explicit/test_awkward_UnionArray_simplify.py
+-rw-r--r--   0        0        0     3710 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-spec-explicit/test_awkward_UnionArray_simplify_one.py
+-rw-r--r--   0        0        0     1989 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-spec-explicit/test_awkward_UnionArray_validity.py
+-rw-r--r--   0        0        0     3441 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-spec-explicit/test_awkward_index_rpad_and_clip_axis0.py
+-rw-r--r--   0        0        0     5746 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-spec-explicit/test_awkward_index_rpad_and_clip_axis1.py
+-rw-r--r--   0        0        0      938 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-spec-explicit/test_awkward_localindex.py
+-rw-r--r--   0        0        0    18001 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-spec-explicit/test_awkward_missing_repeat.py
+-rw-r--r--   0        0        0     4106 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-spec-explicit/test_awkward_reduce_argmax.py
+-rw-r--r--   0        0        0     9790 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-spec-explicit/test_awkward_reduce_argmin.py
+-rw-r--r--   0        0        0    20840 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-spec-explicit/test_awkward_reduce_count_64.py
+-rw-r--r--   0        0        0     2422 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-spec-explicit/test_awkward_reduce_countnonzero.py
+-rw-r--r--   0        0        0     5490 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-spec-explicit/test_awkward_reduce_max.py
+-rw-r--r--   0        0        0     6021 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-spec-explicit/test_awkward_reduce_min.py
+-rw-r--r--   0        0        0    29009 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-spec-explicit/test_awkward_reduce_prod.py
+-rw-r--r--   0        0        0     8895 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-spec-explicit/test_awkward_reduce_prod_bool.py
+-rw-r--r--   0        0        0    12658 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-spec-explicit/test_awkward_reduce_sum.py
+-rw-r--r--   0        0        0     3164 2023-02-16 15:37:39.000000 awkward-cpp-9/tests-spec-explicit/test_awkward_reduce_sum_bool.py
+-rw-r--r--   0        0        0     2120 2023-02-16 15:37:39.000000 awkward-cpp-9/PKG-INFO
```

### Comparing `awkward-cpp-8/CMakeLists.txt` & `awkward-cpp-9/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `awkward-cpp-8/LICENSE` & `awkward-cpp-9/LICENSE`

 * *Files identical despite different names*

### Comparing `awkward-cpp-8/docs/Doxyfile` & `awkward-cpp-9/docs/Doxyfile`

 * *Files identical despite different names*

### Comparing `awkward-cpp-8/docs/footer.html` & `awkward-cpp-9/docs/footer.html`

 * *Files identical despite different names*

### Comparing `awkward-cpp-8/docs/header.html` & `awkward-cpp-9/docs/header.html`

 * *Files identical despite different names*

### Comparing `awkward-cpp-8/docs/index.md` & `awkward-cpp-9/docs/index.md`

 * *Files identical despite different names*

### Comparing `awkward-cpp-8/header-only/awkward/BuilderOptions.h` & `awkward-cpp-9/header-only/awkward/BuilderOptions.h`

 * *Files identical despite different names*

### Comparing `awkward-cpp-8/header-only/awkward/GrowableBuffer.h` & `awkward-cpp-9/header-only/awkward/GrowableBuffer.h`

 * *Files identical despite different names*

### Comparing `awkward-cpp-8/header-only/awkward/LayoutBuilder.h` & `awkward-cpp-9/header-only/awkward/LayoutBuilder.h`

 * *Files identical despite different names*

### Comparing `awkward-cpp-8/header-only/awkward/utils.h` & `awkward-cpp-9/header-only/awkward/utils.h`

 * *Files identical despite different names*

### Comparing `awkward-cpp-8/include/awkward/builder/ArrayBuilder.h` & `awkward-cpp-9/include/awkward/builder/ArrayBuilder.h`

 * *Files identical despite different names*

### Comparing `awkward-cpp-8/include/awkward/builder/BoolBuilder.h` & `awkward-cpp-9/include/awkward/builder/BoolBuilder.h`

 * *Files identical despite different names*

### Comparing `awkward-cpp-8/include/awkward/builder/Builder.h` & `awkward-cpp-9/include/awkward/builder/Builder.h`

 * *Files identical despite different names*

### Comparing `awkward-cpp-8/include/awkward/builder/Complex128Builder.h` & `awkward-cpp-9/include/awkward/builder/Complex128Builder.h`

 * *Files identical despite different names*

### Comparing `awkward-cpp-8/include/awkward/builder/DatetimeBuilder.h` & `awkward-cpp-9/include/awkward/builder/DatetimeBuilder.h`

 * *Files identical despite different names*

### Comparing `awkward-cpp-8/include/awkward/builder/Float64Builder.h` & `awkward-cpp-9/include/awkward/builder/Float64Builder.h`

 * *Files identical despite different names*

### Comparing `awkward-cpp-8/include/awkward/builder/Int64Builder.h` & `awkward-cpp-9/include/awkward/builder/Int64Builder.h`

 * *Files identical despite different names*

### Comparing `awkward-cpp-8/include/awkward/builder/ListBuilder.h` & `awkward-cpp-9/include/awkward/builder/ListBuilder.h`

 * *Files identical despite different names*

### Comparing `awkward-cpp-8/include/awkward/builder/OptionBuilder.h` & `awkward-cpp-9/include/awkward/builder/OptionBuilder.h`

 * *Files identical despite different names*

### Comparing `awkward-cpp-8/include/awkward/builder/RecordBuilder.h` & `awkward-cpp-9/include/awkward/builder/RecordBuilder.h`

 * *Files identical despite different names*

### Comparing `awkward-cpp-8/include/awkward/builder/StringBuilder.h` & `awkward-cpp-9/include/awkward/builder/StringBuilder.h`

 * *Files identical despite different names*

### Comparing `awkward-cpp-8/include/awkward/builder/TupleBuilder.h` & `awkward-cpp-9/include/awkward/builder/TupleBuilder.h`

 * *Files identical despite different names*

### Comparing `awkward-cpp-8/include/awkward/builder/UnionBuilder.h` & `awkward-cpp-9/include/awkward/builder/UnionBuilder.h`

 * *Files identical despite different names*

### Comparing `awkward-cpp-8/include/awkward/builder/UnknownBuilder.h` & `awkward-cpp-9/include/awkward/builder/UnknownBuilder.h`

 * *Files identical despite different names*

### Comparing `awkward-cpp-8/include/awkward/common.h` & `awkward-cpp-9/include/awkward/common.h`

 * *Files identical despite different names*

### Comparing `awkward-cpp-8/include/awkward/datetime_util.h` & `awkward-cpp-9/include/awkward/datetime_util.h`

 * *Files identical despite different names*

### Comparing `awkward-cpp-8/include/awkward/forth/ForthInputBuffer.h` & `awkward-cpp-9/include/awkward/forth/ForthInputBuffer.h`

 * *Files identical despite different names*

### Comparing `awkward-cpp-8/include/awkward/forth/ForthMachine.h` & `awkward-cpp-9/include/awkward/forth/ForthMachine.h`

 * *Files identical despite different names*

### Comparing `awkward-cpp-8/include/awkward/forth/ForthOutputBuffer.h` & `awkward-cpp-9/include/awkward/forth/ForthOutputBuffer.h`

 * *Files identical despite different names*

### Comparing `awkward-cpp-8/include/awkward/io/json.h` & `awkward-cpp-9/include/awkward/io/json.h`

 * *Files identical despite different names*

### Comparing `awkward-cpp-8/include/awkward/kernel-utils.h` & `awkward-cpp-9/include/awkward/kernel-utils.h`

 * *Files identical despite different names*

### Comparing `awkward-cpp-8/include/awkward/kernels.h` & `awkward-cpp-9/include/awkward/kernels.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-// AUTO GENERATED ON 2023-02-03 AT 22:54:31
+// AUTO GENERATED ON 2023-02-16 AT 15:37:39
 // DO NOT EDIT BY HAND!
 //
 // To regenerate file, run
 //
 //     python dev/generate-kernel-signatures.py
 //
 // (It is usually run as part of pip install . or localbuild.py.)
@@ -98,40 +98,14 @@
     int64_t* offsets_in,
     int64_t* mask_out,
     int64_t* starts_out,
     int64_t* stops_out,
     int64_t length);
 
   EXPORT_SYMBOL ERROR
-  awkward_Index32_iscontiguous(
-    bool* result,
-    const int32_t* fromindex,
-    int64_t length);
-  EXPORT_SYMBOL ERROR
-  awkward_Index64_iscontiguous(
-    bool* result,
-    const int64_t* fromindex,
-    int64_t length);
-  EXPORT_SYMBOL ERROR
-  awkward_Index8_iscontiguous(
-    bool* result,
-    const int8_t* fromindex,
-    int64_t length);
-  EXPORT_SYMBOL ERROR
-  awkward_IndexU32_iscontiguous(
-    bool* result,
-    const uint32_t* fromindex,
-    int64_t length);
-  EXPORT_SYMBOL ERROR
-  awkward_IndexU8_iscontiguous(
-    bool* result,
-    const uint8_t* fromindex,
-    int64_t length);
-
-  EXPORT_SYMBOL ERROR
   awkward_IndexedArray_fill_to64_from32(
     int64_t* toindex,
     int64_t toindexoffset,
     const int32_t* fromindex,
     int64_t length,
     int64_t base);
   EXPORT_SYMBOL ERROR
```

### Comparing `awkward-cpp-8/include/awkward/python/content.h` & `awkward-cpp-9/include/awkward/python/content.h`

 * *Files identical despite different names*

### Comparing `awkward-cpp-8/include/awkward/python/util.h` & `awkward-cpp-9/include/awkward/python/util.h`

 * *Files identical despite different names*

### Comparing `awkward-cpp-8/include/awkward/util.h` & `awkward-cpp-9/include/awkward/util.h`

 * *Files identical despite different names*

### Comparing `awkward-cpp-8/pyproject.toml` & `awkward-cpp-9/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
     "scikit-build-core[pyproject]>=0.1.3",
     "pybind11",
 ]
 build-backend = "scikit_build_core.build"
 
 [project]
 name = "awkward_cpp"
-version = "8"
+version = "9"
 dependencies = [
     "numpy>=1.14.5"
 ]
 readme = "README.md"
 description = "CPU kernels and compiled extensions for Awkward Array"
 authors = [
     {name = "Jim Pivarski", email = "pivarski@princeton.edu"},
```

### Comparing `awkward-cpp-8/rapidjson/.travis.yml` & `awkward-cpp-9/rapidjson/.travis.yml`

 * *Files identical despite different names*

### Comparing `awkward-cpp-8/rapidjson/CHANGELOG.md` & `awkward-cpp-9/rapidjson/CHANGELOG.md`

 * *Files identical despite different names*

### Comparing `awkward-cpp-8/rapidjson/CMakeLists.txt` & `awkward-cpp-9/rapidjson/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `awkward-cpp-8/rapidjson/CMakeModules/FindGTestSrc.cmake` & `awkward-cpp-9/rapidjson/CMakeModules/FindGTestSrc.cmake`

 * *Files identical despite different names*

### Comparing `awkward-cpp-8/rapidjson/appveyor.yml` & `awkward-cpp-9/rapidjson/appveyor.yml`

 * *Files identical despite different names*

### Comparing `awkward-cpp-8/rapidjson/bin/data/glossary.json` & `awkward-cpp-9/rapidjson/bin/data/glossary.json`

 * *Files identical despite different names*

### Comparing `awkward-cpp-8/rapidjson/bin/data/menu.json` & `awkward-cpp-9/rapidjson/bin/data/menu.json`

 * *Files identical despite different names*

### Comparing `awkward-cpp-8/rapidjson/bin/data/sample.json` & `awkward-cpp-9/rapidjson/bin/data/sample.json`

 * *Files identical despite different names*

### Comparing `awkward-cpp-8/rapidjson/bin/data/webapp.json` & `awkward-cpp-9/rapidjson/bin/data/webapp.json`

 * *Files identical despite different names*

### Comparing `awkward-cpp-8/rapidjson/bin/data/widget.json` & `awkward-cpp-9/rapidjson/bin/data/widget.json`

 * *Files identical despite different names*

### Comparing `awkward-cpp-8/rapidjson/bin/draft-04/schema` & `awkward-cpp-9/rapidjson/bin/draft-04/schema`

 * *Files identical despite different names*

### Comparing `awkward-cpp-8/rapidjson/bin/encodings/utf32be.json` & `awkward-cpp-9/rapidjson/bin/encodings/utf32be.json`

 * *Files identical despite different names*

### Comparing `awkward-cpp-8/rapidjson/bin/encodings/utf32bebom.json` & `awkward-cpp-9/rapidjson/bin/encodings/utf32bebom.json`

 * *Files identical despite different names*

### Comparing `awkward-cpp-8/rapidjson/bin/encodings/utf32le.json` & `awkward-cpp-9/rapidjson/bin/encodings/utf32le.json`

 * *Files identical despite different names*

### Comparing `awkward-cpp-8/rapidjson/bin/encodings/utf32lebom.json` & `awkward-cpp-9/rapidjson/bin/encodings/utf32lebom.json`

 * *Files identical despite different names*

### Comparing `awkward-cpp-8/rapidjson/bin/jsonchecker/pass1.json` & `awkward-cpp-9/rapidjson/bin/jsonchecker/pass1.json`

 * *Files identical despite different names*

### Comparing `awkward-cpp-8/rapidjson/bin/jsonschema/LICENSE` & `awkward-cpp-9/rapidjson/bin/jsonschema/LICENSE`

 * *Files identical despite different names*

### Comparing `awkward-cpp-8/rapidjson/bin/jsonschema/README.md` & `awkward-cpp-9/rapidjson/bin/jsonschema/README.md`

 * *Files identical despite different names*

### Comparing `awkward-cpp-8/rapidjson/bin/jsonschema/bin/jsonschema_suite` & `awkward-cpp-9/rapidjson/bin/jsonschema/bin/jsonschema_suite`

 * *Files identical despite different names*

### Comparing `awkward-cpp-8/rapidjson/bin/jsonschema/remotes/.DS_Store` & `awkward-cpp-9/rapidjson/bin/jsonschema/remotes/.DS_Store`

 * *Files identical despite different names*

### Comparing `awkward-cpp-8/rapidjson/bin/jsonschema/tests/.DS_Store` & `awkward-cpp-9/rapidjson/bin/jsonschema/tests/.DS_Store`

 * *Files identical despite different names*

### Comparing `awkward-cpp-8/rapidjson/bin/jsonschema/tests/draft3/additionalItems.json` & `awkward-cpp-9/rapidjson/bin/jsonschema/tests/draft3/additionalItems.json`

 * *Files identical despite different names*

### Comparing `awkward-cpp-8/rapidjson/bin/jsonschema/tests/draft3/additionalProperties.json` & `awkward-cpp-9/rapidjson/bin/jsonschema/tests/draft3/additionalProperties.json`

 * *Files identical despite different names*

### Comparing `awkward-cpp-8/rapidjson/bin/jsonschema/tests/draft3/default.json` & `awkward-cpp-9/rapidjson/bin/jsonschema/tests/draft3/default.json`

 * *Files identical despite different names*

### Comparing `awkward-cpp-8/rapidjson/bin/jsonschema/tests/draft3/dependencies.json` & `awkward-cpp-9/rapidjson/bin/jsonschema/tests/draft3/dependencies.json`

 * *Files identical despite different names*

### Comparing `awkward-cpp-8/rapidjson/bin/jsonschema/tests/draft3/disallow.json` & `awkward-cpp-9/rapidjson/bin/jsonschema/tests/draft3/disallow.json`

 * *Files identical despite different names*

### Comparing `awkward-cpp-8/rapidjson/bin/jsonschema/tests/draft3/divisibleBy.json` & `awkward-cpp-9/rapidjson/bin/jsonschema/tests/draft3/divisibleBy.json`

 * *Files identical despite different names*

### Comparing `awkward-cpp-8/rapidjson/bin/jsonschema/tests/draft3/enum.json` & `awkward-cpp-9/rapidjson/bin/jsonschema/tests/draft3/enum.json`

 * *Files identical despite different names*

### Comparing `awkward-cpp-8/rapidjson/bin/jsonschema/tests/draft3/extends.json` & `awkward-cpp-9/rapidjson/bin/jsonschema/tests/draft3/extends.json`

 * *Files identical despite different names*

### Comparing `awkward-cpp-8/rapidjson/bin/jsonschema/tests/draft3/items.json` & `awkward-cpp-9/rapidjson/bin/jsonschema/tests/draft3/items.json`

 * *Files identical despite different names*

### Comparing `awkward-cpp-8/rapidjson/bin/jsonschema/tests/draft3/maxItems.json` & `awkward-cpp-9/rapidjson/bin/jsonschema/tests/draft3/maxItems.json`

 * *Files identical despite different names*

### Comparing `awkward-cpp-8/rapidjson/bin/jsonschema/tests/draft3/maxLength.json` & `awkward-cpp-9/rapidjson/bin/jsonschema/tests/draft3/maxLength.json`

 * *Files identical despite different names*

### Comparing `awkward-cpp-8/rapidjson/bin/jsonschema/tests/draft3/maximum.json` & `awkward-cpp-9/rapidjson/bin/jsonschema/tests/draft3/maximum.json`

 * *Files identical despite different names*

### Comparing `awkward-cpp-8/rapidjson/bin/jsonschema/tests/draft3/minItems.json` & `awkward-cpp-9/rapidjson/bin/jsonschema/tests/draft3/minItems.json`

 * *Files identical despite different names*

### Comparing `awkward-cpp-8/rapidjson/bin/jsonschema/tests/draft3/minLength.json` & `awkward-cpp-9/rapidjson/bin/jsonschema/tests/draft3/minLength.json`

 * *Files identical despite different names*

### Comparing `awkward-cpp-8/rapidjson/bin/jsonschema/tests/draft3/minimum.json` & `awkward-cpp-9/rapidjson/bin/jsonschema/tests/draft3/minimum.json`

 * *Files identical despite different names*

### Comparing `awkward-cpp-8/rapidjson/bin/jsonschema/tests/draft3/optional/bignum.json` & `awkward-cpp-9/rapidjson/bin/jsonschema/tests/draft3/optional/bignum.json`

 * *Files identical despite different names*

### Comparing `awkward-cpp-8/rapidjson/bin/jsonschema/tests/draft3/optional/format.json` & `awkward-cpp-9/rapidjson/bin/jsonschema/tests/draft3/optional/format.json`

 * *Files identical despite different names*

### Comparing `awkward-cpp-8/rapidjson/bin/jsonschema/tests/draft3/pattern.json` & `awkward-cpp-9/rapidjson/bin/jsonschema/tests/draft3/pattern.json`

 * *Files identical despite different names*

### Comparing `awkward-cpp-8/rapidjson/bin/jsonschema/tests/draft3/patternProperties.json` & `awkward-cpp-9/rapidjson/bin/jsonschema/tests/draft3/patternProperties.json`

 * *Files identical despite different names*

### Comparing `awkward-cpp-8/rapidjson/bin/jsonschema/tests/draft3/properties.json` & `awkward-cpp-9/rapidjson/bin/jsonschema/tests/draft3/properties.json`

 * *Files identical despite different names*

### Comparing `awkward-cpp-8/rapidjson/bin/jsonschema/tests/draft3/ref.json` & `awkward-cpp-9/rapidjson/bin/jsonschema/tests/draft3/ref.json`

 * *Files identical despite different names*

### Comparing `awkward-cpp-8/rapidjson/bin/jsonschema/tests/draft3/refRemote.json` & `awkward-cpp-9/rapidjson/bin/jsonschema/tests/draft3/refRemote.json`

 * *Files identical despite different names*

### Comparing `awkward-cpp-8/rapidjson/bin/jsonschema/tests/draft3/required.json` & `awkward-cpp-9/rapidjson/bin/jsonschema/tests/draft3/required.json`

 * *Files identical despite different names*

### Comparing `awkward-cpp-8/rapidjson/bin/jsonschema/tests/draft3/type.json` & `awkward-cpp-9/rapidjson/bin/jsonschema/tests/draft3/type.json`

 * *Files identical despite different names*

### Comparing `awkward-cpp-8/rapidjson/bin/jsonschema/tests/draft3/uniqueItems.json` & `awkward-cpp-9/rapidjson/bin/jsonschema/tests/draft3/uniqueItems.json`

 * *Files identical despite different names*

### Comparing `awkward-cpp-8/rapidjson/bin/jsonschema/tests/draft4/.DS_Store` & `awkward-cpp-9/rapidjson/bin/jsonschema/tests/draft4/.DS_Store`

 * *Files identical despite different names*

### Comparing `awkward-cpp-8/rapidjson/bin/jsonschema/tests/draft4/additionalItems.json` & `awkward-cpp-9/rapidjson/bin/jsonschema/tests/draft4/additionalItems.json`

 * *Files identical despite different names*

### Comparing `awkward-cpp-8/rapidjson/bin/jsonschema/tests/draft4/additionalProperties.json` & `awkward-cpp-9/rapidjson/bin/jsonschema/tests/draft4/additionalProperties.json`

 * *Files identical despite different names*

### Comparing `awkward-cpp-8/rapidjson/bin/jsonschema/tests/draft4/allOf.json` & `awkward-cpp-9/rapidjson/bin/jsonschema/tests/draft4/allOf.json`

 * *Files identical despite different names*

### Comparing `awkward-cpp-8/rapidjson/bin/jsonschema/tests/draft4/anyOf.json` & `awkward-cpp-9/rapidjson/bin/jsonschema/tests/draft4/anyOf.json`

 * *Files identical despite different names*

### Comparing `awkward-cpp-8/rapidjson/bin/jsonschema/tests/draft4/default.json` & `awkward-cpp-9/rapidjson/bin/jsonschema/tests/draft4/default.json`

 * *Files identical despite different names*

### Comparing `awkward-cpp-8/rapidjson/bin/jsonschema/tests/draft4/definitions.json` & `awkward-cpp-9/rapidjson/bin/jsonschema/tests/draft4/definitions.json`

 * *Files identical despite different names*

### Comparing `awkward-cpp-8/rapidjson/bin/jsonschema/tests/draft4/dependencies.json` & `awkward-cpp-9/rapidjson/bin/jsonschema/tests/draft4/dependencies.json`

 * *Files identical despite different names*

### Comparing `awkward-cpp-8/rapidjson/bin/jsonschema/tests/draft4/enum.json` & `awkward-cpp-9/rapidjson/bin/jsonschema/tests/draft4/enum.json`

 * *Files identical despite different names*

### Comparing `awkward-cpp-8/rapidjson/bin/jsonschema/tests/draft4/items.json` & `awkward-cpp-9/rapidjson/bin/jsonschema/tests/draft4/items.json`

 * *Files identical despite different names*

### Comparing `awkward-cpp-8/rapidjson/bin/jsonschema/tests/draft4/maxItems.json` & `awkward-cpp-9/rapidjson/bin/jsonschema/tests/draft4/maxItems.json`

 * *Files identical despite different names*

### Comparing `awkward-cpp-8/rapidjson/bin/jsonschema/tests/draft4/maxLength.json` & `awkward-cpp-9/rapidjson/bin/jsonschema/tests/draft4/maxLength.json`

 * *Files identical despite different names*

### Comparing `awkward-cpp-8/rapidjson/bin/jsonschema/tests/draft4/maxProperties.json` & `awkward-cpp-9/rapidjson/bin/jsonschema/tests/draft4/maxProperties.json`

 * *Files identical despite different names*

### Comparing `awkward-cpp-8/rapidjson/bin/jsonschema/tests/draft4/maximum.json` & `awkward-cpp-9/rapidjson/bin/jsonschema/tests/draft4/maximum.json`

 * *Files identical despite different names*

### Comparing `awkward-cpp-8/rapidjson/bin/jsonschema/tests/draft4/minItems.json` & `awkward-cpp-9/rapidjson/bin/jsonschema/tests/draft4/minItems.json`

 * *Files identical despite different names*

### Comparing `awkward-cpp-8/rapidjson/bin/jsonschema/tests/draft4/minLength.json` & `awkward-cpp-9/rapidjson/bin/jsonschema/tests/draft4/minLength.json`

 * *Files identical despite different names*

### Comparing `awkward-cpp-8/rapidjson/bin/jsonschema/tests/draft4/minProperties.json` & `awkward-cpp-9/rapidjson/bin/jsonschema/tests/draft4/minProperties.json`

 * *Files identical despite different names*

### Comparing `awkward-cpp-8/rapidjson/bin/jsonschema/tests/draft4/minimum.json` & `awkward-cpp-9/rapidjson/bin/jsonschema/tests/draft4/minimum.json`

 * *Files identical despite different names*

### Comparing `awkward-cpp-8/rapidjson/bin/jsonschema/tests/draft4/multipleOf.json` & `awkward-cpp-9/rapidjson/bin/jsonschema/tests/draft4/multipleOf.json`

 * *Files identical despite different names*

### Comparing `awkward-cpp-8/rapidjson/bin/jsonschema/tests/draft4/not.json` & `awkward-cpp-9/rapidjson/bin/jsonschema/tests/draft4/not.json`

 * *Files identical despite different names*

### Comparing `awkward-cpp-8/rapidjson/bin/jsonschema/tests/draft4/oneOf.json` & `awkward-cpp-9/rapidjson/bin/jsonschema/tests/draft4/oneOf.json`

 * *Files identical despite different names*

### Comparing `awkward-cpp-8/rapidjson/bin/jsonschema/tests/draft4/optional/bignum.json` & `awkward-cpp-9/rapidjson/bin/jsonschema/tests/draft4/optional/bignum.json`

 * *Files identical despite different names*

### Comparing `awkward-cpp-8/rapidjson/bin/jsonschema/tests/draft4/optional/format.json` & `awkward-cpp-9/rapidjson/bin/jsonschema/tests/draft4/optional/format.json`

 * *Files identical despite different names*

### Comparing `awkward-cpp-8/rapidjson/bin/jsonschema/tests/draft4/pattern.json` & `awkward-cpp-9/rapidjson/bin/jsonschema/tests/draft4/pattern.json`

 * *Files identical despite different names*

### Comparing `awkward-cpp-8/rapidjson/bin/jsonschema/tests/draft4/patternProperties.json` & `awkward-cpp-9/rapidjson/bin/jsonschema/tests/draft4/patternProperties.json`

 * *Files identical despite different names*

### Comparing `awkward-cpp-8/rapidjson/bin/jsonschema/tests/draft4/properties.json` & `awkward-cpp-9/rapidjson/bin/jsonschema/tests/draft4/properties.json`

 * *Files identical despite different names*

### Comparing `awkward-cpp-8/rapidjson/bin/jsonschema/tests/draft4/ref.json` & `awkward-cpp-9/rapidjson/bin/jsonschema/tests/draft4/ref.json`

 * *Files identical despite different names*

### Comparing `awkward-cpp-8/rapidjson/bin/jsonschema/tests/draft4/refRemote.json` & `awkward-cpp-9/rapidjson/bin/jsonschema/tests/draft4/refRemote.json`

 * *Files identical despite different names*

### Comparing `awkward-cpp-8/rapidjson/bin/jsonschema/tests/draft4/required.json` & `awkward-cpp-9/rapidjson/bin/jsonschema/tests/draft4/required.json`

 * *Files identical despite different names*

### Comparing `awkward-cpp-8/rapidjson/bin/jsonschema/tests/draft4/type.json` & `awkward-cpp-9/rapidjson/bin/jsonschema/tests/draft4/type.json`

 * *Files identical despite different names*

### Comparing `awkward-cpp-8/rapidjson/bin/jsonschema/tests/draft4/uniqueItems.json` & `awkward-cpp-9/rapidjson/bin/jsonschema/tests/draft4/uniqueItems.json`

 * *Files identical despite different names*

### Comparing `awkward-cpp-8/rapidjson/bin/types/floats.json` & `awkward-cpp-9/rapidjson/bin/types/floats.json`

 * *Files identical despite different names*

### Comparing `awkward-cpp-8/rapidjson/bin/types/guids.json` & `awkward-cpp-9/rapidjson/bin/types/guids.json`

 * *Files identical despite different names*

### Comparing `awkward-cpp-8/rapidjson/bin/types/integers.json` & `awkward-cpp-9/rapidjson/bin/types/integers.json`

 * *Files identical despite different names*

### Comparing `awkward-cpp-8/rapidjson/bin/types/mixed.json` & `awkward-cpp-9/rapidjson/bin/types/mixed.json`

 * *Files identical despite different names*

### Comparing `awkward-cpp-8/rapidjson/bin/types/paragraphs.json` & `awkward-cpp-9/rapidjson/bin/types/paragraphs.json`

 * *Files identical despite different names*

### Comparing `awkward-cpp-8/rapidjson/doc/CMakeLists.txt` & `awkward-cpp-9/rapidjson/doc/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `awkward-cpp-8/rapidjson/doc/Doxyfile.in` & `awkward-cpp-9/rapidjson/doc/Doxyfile.in`

 * *Files identical despite different names*

### Comparing `awkward-cpp-8/rapidjson/doc/Doxyfile.zh-cn.in` & `awkward-cpp-9/rapidjson/doc/Doxyfile.zh-cn.in`

 * *Files identical despite different names*

### Comparing `awkward-cpp-8/rapidjson/doc/diagram/architecture.dot` & `awkward-cpp-9/rapidjson/doc/diagram/architecture.dot`

 * *Files identical despite different names*

### Comparing `awkward-cpp-8/rapidjson/doc/diagram/architecture.png` & `awkward-cpp-9/rapidjson/doc/diagram/architecture.png`

 * *Files identical despite different names*

### Comparing `awkward-cpp-8/rapidjson/doc/diagram/insituparsing.dot` & `awkward-cpp-9/rapidjson/doc/diagram/insituparsing.dot`

 * *Files identical despite different names*

### Comparing `awkward-cpp-8/rapidjson/doc/diagram/insituparsing.png` & `awkward-cpp-9/rapidjson/doc/diagram/insituparsing.png`

 * *Files identical despite different names*

### Comparing `awkward-cpp-8/rapidjson/doc/diagram/iterative-parser-states-diagram.dot` & `awkward-cpp-9/rapidjson/doc/diagram/iterative-parser-states-diagram.dot`

 * *Files identical despite different names*

### Comparing `awkward-cpp-8/rapidjson/doc/diagram/iterative-parser-states-diagram.png` & `awkward-cpp-9/rapidjson/doc/diagram/iterative-parser-states-diagram.png`

 * *Files identical despite different names*

### Comparing `awkward-cpp-8/rapidjson/doc/diagram/move1.dot` & `awkward-cpp-9/rapidjson/doc/diagram/move1.dot`

 * *Files identical despite different names*

### Comparing `awkward-cpp-8/rapidjson/doc/diagram/move1.png` & `awkward-cpp-9/rapidjson/doc/diagram/move1.png`

 * *Files identical despite different names*

### Comparing `awkward-cpp-8/rapidjson/doc/diagram/move2.dot` & `awkward-cpp-9/rapidjson/doc/diagram/move2.dot`

 * *Files identical despite different names*

### Comparing `awkward-cpp-8/rapidjson/doc/diagram/move2.png` & `awkward-cpp-9/rapidjson/doc/diagram/move2.png`

 * *Files identical despite different names*

### Comparing `awkward-cpp-8/rapidjson/doc/diagram/move3.dot` & `awkward-cpp-9/rapidjson/doc/diagram/move3.dot`

 * *Files identical despite different names*

### Comparing `awkward-cpp-8/rapidjson/doc/diagram/move3.png` & `awkward-cpp-9/rapidjson/doc/diagram/move3.png`

 * *Files identical despite different names*

### Comparing `awkward-cpp-8/rapidjson/doc/diagram/normalparsing.dot` & `awkward-cpp-9/rapidjson/doc/diagram/normalparsing.dot`

 * *Files identical despite different names*

### Comparing `awkward-cpp-8/rapidjson/doc/diagram/normalparsing.png` & `awkward-cpp-9/rapidjson/doc/diagram/normalparsing.png`

 * *Files identical despite different names*

### Comparing `awkward-cpp-8/rapidjson/doc/diagram/simpledom.dot` & `awkward-cpp-9/rapidjson/doc/diagram/simpledom.dot`

 * *Files identical despite different names*

### Comparing `awkward-cpp-8/rapidjson/doc/diagram/simpledom.png` & `awkward-cpp-9/rapidjson/doc/diagram/simpledom.png`

 * *Files identical despite different names*

### Comparing `awkward-cpp-8/rapidjson/doc/diagram/tutorial.dot` & `awkward-cpp-9/rapidjson/doc/diagram/tutorial.dot`

 * *Files identical despite different names*

### Comparing `awkward-cpp-8/rapidjson/doc/diagram/tutorial.png` & `awkward-cpp-9/rapidjson/doc/diagram/tutorial.png`

 * *Files identical despite different names*

### Comparing `awkward-cpp-8/rapidjson/doc/diagram/utilityclass.dot` & `awkward-cpp-9/rapidjson/doc/diagram/utilityclass.dot`

 * *Files identical despite different names*

### Comparing `awkward-cpp-8/rapidjson/doc/diagram/utilityclass.png` & `awkward-cpp-9/rapidjson/doc/diagram/utilityclass.png`

 * *Files identical despite different names*

### Comparing `awkward-cpp-8/rapidjson/doc/dom.md` & `awkward-cpp-9/rapidjson/doc/dom.md`

 * *Files identical despite different names*

### Comparing `awkward-cpp-8/rapidjson/doc/dom.zh-cn.md` & `awkward-cpp-9/rapidjson/doc/dom.zh-cn.md`

 * *Files identical despite different names*

### Comparing `awkward-cpp-8/rapidjson/doc/encoding.md` & `awkward-cpp-9/rapidjson/doc/encoding.md`

 * *Files identical despite different names*

### Comparing `awkward-cpp-8/rapidjson/doc/encoding.zh-cn.md` & `awkward-cpp-9/rapidjson/doc/encoding.zh-cn.md`

 * *Files identical despite different names*

### Comparing `awkward-cpp-8/rapidjson/doc/faq.md` & `awkward-cpp-9/rapidjson/doc/faq.md`

 * *Files identical despite different names*

### Comparing `awkward-cpp-8/rapidjson/doc/faq.zh-cn.md` & `awkward-cpp-9/rapidjson/doc/faq.zh-cn.md`

 * *Files identical despite different names*

### Comparing `awkward-cpp-8/rapidjson/doc/features.md` & `awkward-cpp-9/rapidjson/doc/features.md`

 * *Files identical despite different names*

### Comparing `awkward-cpp-8/rapidjson/doc/features.zh-cn.md` & `awkward-cpp-9/rapidjson/doc/features.zh-cn.md`

 * *Files identical despite different names*

### Comparing `awkward-cpp-8/rapidjson/doc/internals.md` & `awkward-cpp-9/rapidjson/doc/internals.md`

 * *Files identical despite different names*

### Comparing `awkward-cpp-8/rapidjson/doc/logo/rapidjson.png` & `awkward-cpp-9/rapidjson/doc/logo/rapidjson.png`

 * *Files identical despite different names*

### Comparing `awkward-cpp-8/rapidjson/doc/logo/rapidjson.svg` & `awkward-cpp-9/rapidjson/doc/logo/rapidjson.svg`

 * *Files identical despite different names*

### Comparing `awkward-cpp-8/rapidjson/doc/misc/DoxygenLayout.xml` & `awkward-cpp-9/rapidjson/doc/misc/DoxygenLayout.xml`

 * *Files identical despite different names*

### Comparing `awkward-cpp-8/rapidjson/doc/misc/doxygenextra.css` & `awkward-cpp-9/rapidjson/doc/misc/doxygenextra.css`

 * *Files identical despite different names*

### Comparing `awkward-cpp-8/rapidjson/doc/misc/header.html` & `awkward-cpp-9/rapidjson/doc/misc/header.html`

 * *Files identical despite different names*

### Comparing `awkward-cpp-8/rapidjson/doc/performance.md` & `awkward-cpp-9/rapidjson/doc/performance.md`

 * *Files identical despite different names*

### Comparing `awkward-cpp-8/rapidjson/doc/performance.zh-cn.md` & `awkward-cpp-9/rapidjson/doc/performance.zh-cn.md`

 * *Files identical despite different names*

### Comparing `awkward-cpp-8/rapidjson/doc/pointer.md` & `awkward-cpp-9/rapidjson/doc/pointer.md`

 * *Files identical despite different names*

### Comparing `awkward-cpp-8/rapidjson/doc/pointer.zh-cn.md` & `awkward-cpp-9/rapidjson/doc/pointer.zh-cn.md`

 * *Files identical despite different names*

### Comparing `awkward-cpp-8/rapidjson/doc/sax.md` & `awkward-cpp-9/rapidjson/doc/sax.md`

 * *Files identical despite different names*

### Comparing `awkward-cpp-8/rapidjson/doc/sax.zh-cn.md` & `awkward-cpp-9/rapidjson/doc/sax.zh-cn.md`

 * *Files identical despite different names*

### Comparing `awkward-cpp-8/rapidjson/doc/schema.md` & `awkward-cpp-9/rapidjson/doc/schema.md`

 * *Files identical despite different names*

### Comparing `awkward-cpp-8/rapidjson/doc/schema.zh-cn.md` & `awkward-cpp-9/rapidjson/doc/schema.zh-cn.md`

 * *Files identical despite different names*

### Comparing `awkward-cpp-8/rapidjson/doc/stream.md` & `awkward-cpp-9/rapidjson/doc/stream.md`

 * *Files identical despite different names*

### Comparing `awkward-cpp-8/rapidjson/doc/stream.zh-cn.md` & `awkward-cpp-9/rapidjson/doc/stream.zh-cn.md`

 * *Files identical despite different names*

### Comparing `awkward-cpp-8/rapidjson/doc/tutorial.md` & `awkward-cpp-9/rapidjson/doc/tutorial.md`

 * *Files identical despite different names*

### Comparing `awkward-cpp-8/rapidjson/doc/tutorial.zh-cn.md` & `awkward-cpp-9/rapidjson/doc/tutorial.zh-cn.md`

 * *Files identical despite different names*

### Comparing `awkward-cpp-8/rapidjson/example/CMakeLists.txt` & `awkward-cpp-9/rapidjson/example/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `awkward-cpp-8/rapidjson/example/capitalize/capitalize.cpp` & `awkward-cpp-9/rapidjson/example/capitalize/capitalize.cpp`

 * *Files identical despite different names*

### Comparing `awkward-cpp-8/rapidjson/example/condense/condense.cpp` & `awkward-cpp-9/rapidjson/example/condense/condense.cpp`

 * *Files identical despite different names*

### Comparing `awkward-cpp-8/rapidjson/example/filterkey/filterkey.cpp` & `awkward-cpp-9/rapidjson/example/filterkey/filterkey.cpp`

 * *Files identical despite different names*

### Comparing `awkward-cpp-8/rapidjson/example/filterkeydom/filterkeydom.cpp` & `awkward-cpp-9/rapidjson/example/filterkeydom/filterkeydom.cpp`

 * *Files identical despite different names*

### Comparing `awkward-cpp-8/rapidjson/example/jsonx/jsonx.cpp` & `awkward-cpp-9/rapidjson/example/jsonx/jsonx.cpp`

 * *Files identical despite different names*

### Comparing `awkward-cpp-8/rapidjson/example/messagereader/messagereader.cpp` & `awkward-cpp-9/rapidjson/example/messagereader/messagereader.cpp`

 * *Files identical despite different names*

### Comparing `awkward-cpp-8/rapidjson/example/parsebyparts/parsebyparts.cpp` & `awkward-cpp-9/rapidjson/example/parsebyparts/parsebyparts.cpp`

 * *Files identical despite different names*

### Comparing `awkward-cpp-8/rapidjson/example/pretty/pretty.cpp` & `awkward-cpp-9/rapidjson/example/pretty/pretty.cpp`

 * *Files identical despite different names*

### Comparing `awkward-cpp-8/rapidjson/example/prettyauto/prettyauto.cpp` & `awkward-cpp-9/rapidjson/example/prettyauto/prettyauto.cpp`

 * *Files identical despite different names*

### Comparing `awkward-cpp-8/rapidjson/example/schemavalidator/schemavalidator.cpp` & `awkward-cpp-9/rapidjson/example/schemavalidator/schemavalidator.cpp`

 * *Files identical despite different names*

### Comparing `awkward-cpp-8/rapidjson/example/serialize/serialize.cpp` & `awkward-cpp-9/rapidjson/example/serialize/serialize.cpp`

 * *Files identical despite different names*

### Comparing `awkward-cpp-8/rapidjson/example/simpledom/simpledom.cpp` & `awkward-cpp-9/rapidjson/example/simpledom/simpledom.cpp`

 * *Files identical despite different names*

### Comparing `awkward-cpp-8/rapidjson/example/simplereader/simplereader.cpp` & `awkward-cpp-9/rapidjson/example/simplereader/simplereader.cpp`

 * *Files identical despite different names*

### Comparing `awkward-cpp-8/rapidjson/example/simplewriter/simplewriter.cpp` & `awkward-cpp-9/rapidjson/example/simplewriter/simplewriter.cpp`

 * *Files identical despite different names*

### Comparing `awkward-cpp-8/rapidjson/example/tutorial/tutorial.cpp` & `awkward-cpp-9/rapidjson/example/tutorial/tutorial.cpp`

 * *Files identical despite different names*

### Comparing `awkward-cpp-8/rapidjson/include/rapidjson/allocators.h` & `awkward-cpp-9/rapidjson/include/rapidjson/allocators.h`

 * *Files identical despite different names*

### Comparing `awkward-cpp-8/rapidjson/include/rapidjson/document.h` & `awkward-cpp-9/rapidjson/include/rapidjson/document.h`

 * *Files identical despite different names*

### Comparing `awkward-cpp-8/rapidjson/include/rapidjson/encodedstream.h` & `awkward-cpp-9/rapidjson/include/rapidjson/encodedstream.h`

 * *Files identical despite different names*

### Comparing `awkward-cpp-8/rapidjson/include/rapidjson/encodings.h` & `awkward-cpp-9/rapidjson/include/rapidjson/encodings.h`

 * *Files identical despite different names*

### Comparing `awkward-cpp-8/rapidjson/include/rapidjson/error/en.h` & `awkward-cpp-9/rapidjson/include/rapidjson/error/en.h`

 * *Files identical despite different names*

### Comparing `awkward-cpp-8/rapidjson/include/rapidjson/error/error.h` & `awkward-cpp-9/rapidjson/include/rapidjson/error/error.h`

 * *Files identical despite different names*

### Comparing `awkward-cpp-8/rapidjson/include/rapidjson/filereadstream.h` & `awkward-cpp-9/rapidjson/include/rapidjson/filereadstream.h`

 * *Files identical despite different names*

### Comparing `awkward-cpp-8/rapidjson/include/rapidjson/filewritestream.h` & `awkward-cpp-9/rapidjson/include/rapidjson/filewritestream.h`

 * *Files identical despite different names*

### Comparing `awkward-cpp-8/rapidjson/include/rapidjson/fwd.h` & `awkward-cpp-9/rapidjson/include/rapidjson/fwd.h`

 * *Files identical despite different names*

### Comparing `awkward-cpp-8/rapidjson/include/rapidjson/internal/biginteger.h` & `awkward-cpp-9/rapidjson/include/rapidjson/internal/biginteger.h`

 * *Files identical despite different names*

### Comparing `awkward-cpp-8/rapidjson/include/rapidjson/internal/diyfp.h` & `awkward-cpp-9/rapidjson/include/rapidjson/internal/diyfp.h`

 * *Files identical despite different names*

### Comparing `awkward-cpp-8/rapidjson/include/rapidjson/internal/dtoa.h` & `awkward-cpp-9/rapidjson/include/rapidjson/internal/dtoa.h`

 * *Files identical despite different names*

### Comparing `awkward-cpp-8/rapidjson/include/rapidjson/internal/ieee754.h` & `awkward-cpp-9/rapidjson/include/rapidjson/internal/ieee754.h`

 * *Files identical despite different names*

### Comparing `awkward-cpp-8/rapidjson/include/rapidjson/internal/itoa.h` & `awkward-cpp-9/rapidjson/include/rapidjson/internal/itoa.h`

 * *Files identical despite different names*

### Comparing `awkward-cpp-8/rapidjson/include/rapidjson/internal/meta.h` & `awkward-cpp-9/rapidjson/include/rapidjson/internal/meta.h`

 * *Files identical despite different names*

### Comparing `awkward-cpp-8/rapidjson/include/rapidjson/internal/pow10.h` & `awkward-cpp-9/rapidjson/include/rapidjson/internal/pow10.h`

 * *Files identical despite different names*

### Comparing `awkward-cpp-8/rapidjson/include/rapidjson/internal/regex.h` & `awkward-cpp-9/rapidjson/include/rapidjson/internal/regex.h`

 * *Files identical despite different names*

### Comparing `awkward-cpp-8/rapidjson/include/rapidjson/internal/stack.h` & `awkward-cpp-9/rapidjson/include/rapidjson/internal/stack.h`

 * *Files identical despite different names*

### Comparing `awkward-cpp-8/rapidjson/include/rapidjson/internal/strfunc.h` & `awkward-cpp-9/rapidjson/include/rapidjson/internal/strfunc.h`

 * *Files identical despite different names*

### Comparing `awkward-cpp-8/rapidjson/include/rapidjson/internal/strtod.h` & `awkward-cpp-9/rapidjson/include/rapidjson/internal/strtod.h`

 * *Files identical despite different names*

### Comparing `awkward-cpp-8/rapidjson/include/rapidjson/internal/swap.h` & `awkward-cpp-9/rapidjson/include/rapidjson/internal/swap.h`

 * *Files identical despite different names*

### Comparing `awkward-cpp-8/rapidjson/include/rapidjson/istreamwrapper.h` & `awkward-cpp-9/rapidjson/include/rapidjson/istreamwrapper.h`

 * *Files identical despite different names*

### Comparing `awkward-cpp-8/rapidjson/include/rapidjson/memorybuffer.h` & `awkward-cpp-9/rapidjson/include/rapidjson/memorybuffer.h`

 * *Files identical despite different names*

### Comparing `awkward-cpp-8/rapidjson/include/rapidjson/memorystream.h` & `awkward-cpp-9/rapidjson/include/rapidjson/memorystream.h`

 * *Files identical despite different names*

### Comparing `awkward-cpp-8/rapidjson/include/rapidjson/msinttypes/inttypes.h` & `awkward-cpp-9/rapidjson/include/rapidjson/msinttypes/inttypes.h`

 * *Files identical despite different names*

### Comparing `awkward-cpp-8/rapidjson/include/rapidjson/msinttypes/stdint.h` & `awkward-cpp-9/rapidjson/include/rapidjson/msinttypes/stdint.h`

 * *Files identical despite different names*

### Comparing `awkward-cpp-8/rapidjson/include/rapidjson/ostreamwrapper.h` & `awkward-cpp-9/rapidjson/include/rapidjson/ostreamwrapper.h`

 * *Files identical despite different names*

### Comparing `awkward-cpp-8/rapidjson/include/rapidjson/pointer.h` & `awkward-cpp-9/rapidjson/include/rapidjson/pointer.h`

 * *Files identical despite different names*

### Comparing `awkward-cpp-8/rapidjson/include/rapidjson/prettywriter.h` & `awkward-cpp-9/rapidjson/include/rapidjson/prettywriter.h`

 * *Files identical despite different names*

### Comparing `awkward-cpp-8/rapidjson/include/rapidjson/rapidjson.h` & `awkward-cpp-9/rapidjson/include/rapidjson/rapidjson.h`

 * *Files identical despite different names*

### Comparing `awkward-cpp-8/rapidjson/include/rapidjson/reader.h` & `awkward-cpp-9/rapidjson/include/rapidjson/reader.h`

 * *Files identical despite different names*

### Comparing `awkward-cpp-8/rapidjson/include/rapidjson/schema.h` & `awkward-cpp-9/rapidjson/include/rapidjson/schema.h`

 * *Files identical despite different names*

### Comparing `awkward-cpp-8/rapidjson/include/rapidjson/stream.h` & `awkward-cpp-9/rapidjson/include/rapidjson/stream.h`

 * *Files identical despite different names*

### Comparing `awkward-cpp-8/rapidjson/include/rapidjson/stringbuffer.h` & `awkward-cpp-9/rapidjson/include/rapidjson/stringbuffer.h`

 * *Files identical despite different names*

### Comparing `awkward-cpp-8/rapidjson/include/rapidjson/writer.h` & `awkward-cpp-9/rapidjson/include/rapidjson/writer.h`

 * *Files identical despite different names*

### Comparing `awkward-cpp-8/rapidjson/license.txt` & `awkward-cpp-9/rapidjson/license.txt`

 * *Files identical despite different names*

### Comparing `awkward-cpp-8/rapidjson/package.json` & `awkward-cpp-9/rapidjson/package.json`

 * *Files identical despite different names*

### Comparing `awkward-cpp-8/rapidjson/rapidjson.autopkg` & `awkward-cpp-9/rapidjson/rapidjson.autopkg`

 * *Files identical despite different names*

### Comparing `awkward-cpp-8/rapidjson/readme.md` & `awkward-cpp-9/rapidjson/readme.md`

 * *Files identical despite different names*

### Comparing `awkward-cpp-8/rapidjson/readme.zh-cn.md` & `awkward-cpp-9/rapidjson/readme.zh-cn.md`

 * *Files identical despite different names*

### Comparing `awkward-cpp-8/rapidjson/test/perftest/CMakeLists.txt` & `awkward-cpp-9/rapidjson/test/perftest/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `awkward-cpp-8/rapidjson/test/perftest/misctest.cpp` & `awkward-cpp-9/rapidjson/test/perftest/misctest.cpp`

 * *Files identical despite different names*

### Comparing `awkward-cpp-8/rapidjson/test/perftest/perftest.cpp` & `awkward-cpp-9/rapidjson/test/perftest/perftest.cpp`

 * *Files identical despite different names*

### Comparing `awkward-cpp-8/rapidjson/test/perftest/perftest.h` & `awkward-cpp-9/rapidjson/test/perftest/perftest.h`

 * *Files identical despite different names*

### Comparing `awkward-cpp-8/rapidjson/test/perftest/platformtest.cpp` & `awkward-cpp-9/rapidjson/test/perftest/platformtest.cpp`

 * *Files identical despite different names*

### Comparing `awkward-cpp-8/rapidjson/test/perftest/rapidjsontest.cpp` & `awkward-cpp-9/rapidjson/test/perftest/rapidjsontest.cpp`

 * *Files identical despite different names*

### Comparing `awkward-cpp-8/rapidjson/test/perftest/schematest.cpp` & `awkward-cpp-9/rapidjson/test/perftest/schematest.cpp`

 * *Files identical despite different names*

### Comparing `awkward-cpp-8/rapidjson/test/unittest/CMakeLists.txt` & `awkward-cpp-9/rapidjson/test/unittest/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `awkward-cpp-8/rapidjson/test/unittest/allocatorstest.cpp` & `awkward-cpp-9/rapidjson/test/unittest/allocatorstest.cpp`

 * *Files identical despite different names*

### Comparing `awkward-cpp-8/rapidjson/test/unittest/bigintegertest.cpp` & `awkward-cpp-9/rapidjson/test/unittest/bigintegertest.cpp`

 * *Files identical despite different names*

### Comparing `awkward-cpp-8/rapidjson/test/unittest/documenttest.cpp` & `awkward-cpp-9/rapidjson/test/unittest/documenttest.cpp`

 * *Files identical despite different names*

### Comparing `awkward-cpp-8/rapidjson/test/unittest/dtoatest.cpp` & `awkward-cpp-9/rapidjson/test/unittest/dtoatest.cpp`

 * *Files identical despite different names*

### Comparing `awkward-cpp-8/rapidjson/test/unittest/encodedstreamtest.cpp` & `awkward-cpp-9/rapidjson/test/unittest/encodedstreamtest.cpp`

 * *Files identical despite different names*

### Comparing `awkward-cpp-8/rapidjson/test/unittest/encodingstest.cpp` & `awkward-cpp-9/rapidjson/test/unittest/encodingstest.cpp`

 * *Files identical despite different names*

### Comparing `awkward-cpp-8/rapidjson/test/unittest/filestreamtest.cpp` & `awkward-cpp-9/rapidjson/test/unittest/filestreamtest.cpp`

 * *Files identical despite different names*

### Comparing `awkward-cpp-8/rapidjson/test/unittest/fwdtest.cpp` & `awkward-cpp-9/rapidjson/test/unittest/fwdtest.cpp`

 * *Files identical despite different names*

### Comparing `awkward-cpp-8/rapidjson/test/unittest/istreamwrappertest.cpp` & `awkward-cpp-9/rapidjson/test/unittest/istreamwrappertest.cpp`

 * *Files identical despite different names*

### Comparing `awkward-cpp-8/rapidjson/test/unittest/itoatest.cpp` & `awkward-cpp-9/rapidjson/test/unittest/itoatest.cpp`

 * *Files identical despite different names*

### Comparing `awkward-cpp-8/rapidjson/test/unittest/jsoncheckertest.cpp` & `awkward-cpp-9/rapidjson/test/unittest/jsoncheckertest.cpp`

 * *Files identical despite different names*

### Comparing `awkward-cpp-8/rapidjson/test/unittest/namespacetest.cpp` & `awkward-cpp-9/rapidjson/test/unittest/namespacetest.cpp`

 * *Files identical despite different names*

### Comparing `awkward-cpp-8/rapidjson/test/unittest/ostreamwrappertest.cpp` & `awkward-cpp-9/rapidjson/test/unittest/ostreamwrappertest.cpp`

 * *Files identical despite different names*

### Comparing `awkward-cpp-8/rapidjson/test/unittest/pointertest.cpp` & `awkward-cpp-9/rapidjson/test/unittest/pointertest.cpp`

 * *Files identical despite different names*

### Comparing `awkward-cpp-8/rapidjson/test/unittest/prettywritertest.cpp` & `awkward-cpp-9/rapidjson/test/unittest/prettywritertest.cpp`

 * *Files identical despite different names*

### Comparing `awkward-cpp-8/rapidjson/test/unittest/readertest.cpp` & `awkward-cpp-9/rapidjson/test/unittest/readertest.cpp`

 * *Files identical despite different names*

### Comparing `awkward-cpp-8/rapidjson/test/unittest/regextest.cpp` & `awkward-cpp-9/rapidjson/test/unittest/regextest.cpp`

 * *Files identical despite different names*

### Comparing `awkward-cpp-8/rapidjson/test/unittest/schematest.cpp` & `awkward-cpp-9/rapidjson/test/unittest/schematest.cpp`

 * *Files identical despite different names*

### Comparing `awkward-cpp-8/rapidjson/test/unittest/simdtest.cpp` & `awkward-cpp-9/rapidjson/test/unittest/simdtest.cpp`

 * *Files identical despite different names*

### Comparing `awkward-cpp-8/rapidjson/test/unittest/strfunctest.cpp` & `awkward-cpp-9/rapidjson/test/unittest/strfunctest.cpp`

 * *Files identical despite different names*

### Comparing `awkward-cpp-8/rapidjson/test/unittest/stringbuffertest.cpp` & `awkward-cpp-9/rapidjson/test/unittest/stringbuffertest.cpp`

 * *Files identical despite different names*

### Comparing `awkward-cpp-8/rapidjson/test/unittest/strtodtest.cpp` & `awkward-cpp-9/rapidjson/test/unittest/strtodtest.cpp`

 * *Files identical despite different names*

### Comparing `awkward-cpp-8/rapidjson/test/unittest/unittest.cpp` & `awkward-cpp-9/rapidjson/test/unittest/unittest.cpp`

 * *Files identical despite different names*

### Comparing `awkward-cpp-8/rapidjson/test/unittest/unittest.h` & `awkward-cpp-9/rapidjson/test/unittest/unittest.h`

 * *Files identical despite different names*

### Comparing `awkward-cpp-8/rapidjson/test/unittest/valuetest.cpp` & `awkward-cpp-9/rapidjson/test/unittest/valuetest.cpp`

 * *Files identical despite different names*

### Comparing `awkward-cpp-8/rapidjson/test/unittest/writertest.cpp` & `awkward-cpp-9/rapidjson/test/unittest/writertest.cpp`

 * *Files identical despite different names*

### Comparing `awkward-cpp-8/rapidjson/travis-doxygen.sh` & `awkward-cpp-9/rapidjson/travis-doxygen.sh`

 * *Files identical despite different names*

### Comparing `awkward-cpp-8/src/awkward_cpp/_kernel_signatures.py` & `awkward-cpp-9/src/awkward_cpp/_kernel_signatures.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# AUTO GENERATED ON 2023-02-03 AT 22:54:31
+# AUTO GENERATED ON 2023-02-16 AT 15:37:39
 # DO NOT EDIT BY HAND!
 #
 # To regenerate file, run
 #
 #     python dev/generate-kernel-signatures.py
 #
 # (It is usually run as part of pip install . or localbuild.py.)
@@ -117,44 +117,14 @@
 
     f = lib.awkward_Content_getitem_next_missing_jagged_getmaskstartstop
     f.argtypes = [POINTER(c_int64), POINTER(c_int64), POINTER(c_int64), POINTER(c_int64), POINTER(c_int64), c_int64]
     f.restype = ERROR
     f.dir = ['in', 'in', 'out', 'out', 'out', 'in']
     out['awkward_Content_getitem_next_missing_jagged_getmaskstartstop', int64, int64, int64, int64, int64] = f
 
-    f = lib.awkward_Index32_iscontiguous
-    f.argtypes = [POINTER(c_bool), POINTER(c_int32), c_int64]
-    f.restype = ERROR
-    f.dir = ['out', 'in', 'in']
-    out['awkward_Index_iscontiguous', bool_, int32] = f
-
-    f = lib.awkward_Index64_iscontiguous
-    f.argtypes = [POINTER(c_bool), POINTER(c_int64), c_int64]
-    f.restype = ERROR
-    f.dir = ['out', 'in', 'in']
-    out['awkward_Index_iscontiguous', bool_, int64] = f
-
-    f = lib.awkward_Index8_iscontiguous
-    f.argtypes = [POINTER(c_bool), POINTER(c_int8), c_int64]
-    f.restype = ERROR
-    f.dir = ['out', 'in', 'in']
-    out['awkward_Index_iscontiguous', bool_, int8] = f
-
-    f = lib.awkward_IndexU32_iscontiguous
-    f.argtypes = [POINTER(c_bool), POINTER(c_uint32), c_int64]
-    f.restype = ERROR
-    f.dir = ['out', 'in', 'in']
-    out['awkward_Index_iscontiguous', bool_, uint32] = f
-
-    f = lib.awkward_IndexU8_iscontiguous
-    f.argtypes = [POINTER(c_bool), POINTER(c_uint8), c_int64]
-    f.restype = ERROR
-    f.dir = ['out', 'in', 'in']
-    out['awkward_Index_iscontiguous', bool_, uint8] = f
-
     f = lib.awkward_IndexedArray_fill_to64_from32
     f.argtypes = [POINTER(c_int64), c_int64, POINTER(c_int32), c_int64, c_int64]
     f.restype = ERROR
     f.dir = ['out', 'in', 'in', 'in', 'in']
     out['awkward_IndexedArray_fill', int64, int32] = f
 
     f = lib.awkward_IndexedArray_fill_to64_from64
```

### Comparing `awkward-cpp-8/src/awkward_cpp/cpu_kernels.py` & `awkward-cpp-9/src/awkward_cpp/cpu_kernels.py`

 * *Files identical despite different names*

### Comparing `awkward-cpp-8/src/awkward_cpp/libawkward.py` & `awkward-cpp-9/src/awkward_cpp/libawkward.py`

 * *Files identical despite different names*

### Comparing `awkward-cpp-8/src/cpu-kernels/awkward_BitMaskedArray_to_ByteMaskedArray.cpp` & `awkward-cpp-9/src/cpu-kernels/awkward_BitMaskedArray_to_ByteMaskedArray.cpp`

 * *Files identical despite different names*

### Comparing `awkward-cpp-8/src/cpu-kernels/awkward_BitMaskedArray_to_IndexedOptionArray.cpp` & `awkward-cpp-9/src/cpu-kernels/awkward_BitMaskedArray_to_IndexedOptionArray.cpp`

 * *Files identical despite different names*

### Comparing `awkward-cpp-8/src/cpu-kernels/awkward_ByteMaskedArray_getitem_nextcarry.cpp` & `awkward-cpp-9/src/cpu-kernels/awkward_ByteMaskedArray_getitem_nextcarry.cpp`

 * *Files identical despite different names*

### Comparing `awkward-cpp-8/src/cpu-kernels/awkward_ByteMaskedArray_getitem_nextcarry_outindex.cpp` & `awkward-cpp-9/src/cpu-kernels/awkward_ByteMaskedArray_getitem_nextcarry_outindex.cpp`

 * *Files identical despite different names*

### Comparing `awkward-cpp-8/src/cpu-kernels/awkward_ByteMaskedArray_overlay_mask.cpp` & `awkward-cpp-9/src/cpu-kernels/awkward_ByteMaskedArray_overlay_mask.cpp`

 * *Files identical despite different names*

### Comparing `awkward-cpp-8/src/cpu-kernels/awkward_ByteMaskedArray_reduce_next_64.cpp` & `awkward-cpp-9/src/cpu-kernels/awkward_ByteMaskedArray_reduce_next_64.cpp`

 * *Files identical despite different names*

### Comparing `awkward-cpp-8/src/cpu-kernels/awkward_ByteMaskedArray_reduce_next_nonlocal_nextshifts_64.cpp` & `awkward-cpp-9/src/cpu-kernels/awkward_ByteMaskedArray_reduce_next_nonlocal_nextshifts_64.cpp`

 * *Files identical despite different names*

### Comparing `awkward-cpp-8/src/cpu-kernels/awkward_ByteMaskedArray_reduce_next_nonlocal_nextshifts_fromshifts_64.cpp` & `awkward-cpp-9/src/cpu-kernels/awkward_ByteMaskedArray_reduce_next_nonlocal_nextshifts_fromshifts_64.cpp`

 * *Files identical despite different names*

### Comparing `awkward-cpp-8/src/cpu-kernels/awkward_ByteMaskedArray_toIndexedOptionArray.cpp` & `awkward-cpp-9/src/cpu-kernels/awkward_ByteMaskedArray_toIndexedOptionArray.cpp`

 * *Files identical despite different names*

### Comparing `awkward-cpp-8/src/cpu-kernels/awkward_Content_getitem_next_missing_jagged_getmaskstartstop.cpp` & `awkward-cpp-9/src/cpu-kernels/awkward_Content_getitem_next_missing_jagged_getmaskstartstop.cpp`

 * *Files identical despite different names*

### Comparing `awkward-cpp-8/src/cpu-kernels/awkward_Index_nones_as_index.cpp` & `awkward-cpp-9/src/cpu-kernels/awkward_Index_nones_as_index.cpp`

 * *Files identical despite different names*

### Comparing `awkward-cpp-8/src/cpu-kernels/awkward_IndexedArray_fill.cpp` & `awkward-cpp-9/src/cpu-kernels/awkward_IndexedArray_fill.cpp`

 * *Files identical despite different names*

### Comparing `awkward-cpp-8/src/cpu-kernels/awkward_IndexedArray_fill_count.cpp` & `awkward-cpp-9/src/cpu-kernels/awkward_IndexedArray_fill_count.cpp`

 * *Files identical despite different names*

### Comparing `awkward-cpp-8/src/cpu-kernels/awkward_IndexedArray_flatten_nextcarry.cpp` & `awkward-cpp-9/src/cpu-kernels/awkward_IndexedArray_flatten_nextcarry.cpp`

 * *Files identical despite different names*

### Comparing `awkward-cpp-8/src/cpu-kernels/awkward_IndexedArray_flatten_none2empty.cpp` & `awkward-cpp-9/src/cpu-kernels/awkward_IndexedArray_flatten_none2empty.cpp`

 * *Files identical despite different names*

### Comparing `awkward-cpp-8/src/cpu-kernels/awkward_IndexedArray_getitem_nextcarry.cpp` & `awkward-cpp-9/src/cpu-kernels/awkward_IndexedArray_getitem_nextcarry.cpp`

 * *Files identical despite different names*

### Comparing `awkward-cpp-8/src/cpu-kernels/awkward_IndexedArray_getitem_nextcarry_outindex.cpp` & `awkward-cpp-9/src/cpu-kernels/awkward_IndexedArray_getitem_nextcarry_outindex.cpp`

 * *Files identical despite different names*

### Comparing `awkward-cpp-8/src/cpu-kernels/awkward_IndexedArray_index_of_nulls.cpp` & `awkward-cpp-9/src/cpu-kernels/awkward_IndexedArray_index_of_nulls.cpp`

 * *Files identical despite different names*

### Comparing `awkward-cpp-8/src/cpu-kernels/awkward_IndexedArray_local_preparenext_64.cpp` & `awkward-cpp-9/src/cpu-kernels/awkward_IndexedArray_local_preparenext_64.cpp`

 * *Files identical despite different names*

### Comparing `awkward-cpp-8/src/cpu-kernels/awkward_IndexedArray_numnull.cpp` & `awkward-cpp-9/src/cpu-kernels/awkward_IndexedArray_numnull.cpp`

 * *Files identical despite different names*

### Comparing `awkward-cpp-8/src/cpu-kernels/awkward_IndexedArray_numnull_parents.cpp` & `awkward-cpp-9/src/cpu-kernels/awkward_IndexedArray_numnull_parents.cpp`

 * *Files identical despite different names*

### Comparing `awkward-cpp-8/src/cpu-kernels/awkward_IndexedArray_overlay_mask.cpp` & `awkward-cpp-9/src/cpu-kernels/awkward_IndexedArray_overlay_mask.cpp`

 * *Files identical despite different names*

### Comparing `awkward-cpp-8/src/cpu-kernels/awkward_IndexedArray_ranges_carry_next_64.cpp` & `awkward-cpp-9/src/cpu-kernels/awkward_IndexedArray_ranges_carry_next_64.cpp`

 * *Files identical despite different names*

### Comparing `awkward-cpp-8/src/cpu-kernels/awkward_IndexedArray_ranges_next_64.cpp` & `awkward-cpp-9/src/cpu-kernels/awkward_IndexedArray_ranges_next_64.cpp`

 * *Files identical despite different names*

### Comparing `awkward-cpp-8/src/cpu-kernels/awkward_IndexedArray_reduce_next_64.cpp` & `awkward-cpp-9/src/cpu-kernels/awkward_IndexedArray_reduce_next_64.cpp`

 * *Files identical despite different names*

### Comparing `awkward-cpp-8/src/cpu-kernels/awkward_IndexedArray_reduce_next_fix_offsets_64.cpp` & `awkward-cpp-9/src/cpu-kernels/awkward_IndexedArray_reduce_next_fix_offsets_64.cpp`

 * *Files identical despite different names*

### Comparing `awkward-cpp-8/src/cpu-kernels/awkward_IndexedArray_reduce_next_nonlocal_nextshifts_64.cpp` & `awkward-cpp-9/src/cpu-kernels/awkward_IndexedArray_reduce_next_nonlocal_nextshifts_64.cpp`

 * *Files identical despite different names*

### Comparing `awkward-cpp-8/src/cpu-kernels/awkward_IndexedArray_reduce_next_nonlocal_nextshifts_fromshifts_64.cpp` & `awkward-cpp-9/src/cpu-kernels/awkward_IndexedArray_reduce_next_nonlocal_nextshifts_fromshifts_64.cpp`

 * *Files identical despite different names*

### Comparing `awkward-cpp-8/src/cpu-kernels/awkward_IndexedArray_simplify.cpp` & `awkward-cpp-9/src/cpu-kernels/awkward_IndexedArray_simplify.cpp`

 * *Files identical despite different names*

### Comparing `awkward-cpp-8/src/cpu-kernels/awkward_IndexedArray_unique_next_index_and_offsets_64.cpp` & `awkward-cpp-9/src/cpu-kernels/awkward_IndexedArray_unique_next_index_and_offsets_64.cpp`

 * *Files identical despite different names*

### Comparing `awkward-cpp-8/src/cpu-kernels/awkward_IndexedArray_validity.cpp` & `awkward-cpp-9/src/cpu-kernels/awkward_IndexedArray_validity.cpp`

 * *Files identical despite different names*

### Comparing `awkward-cpp-8/src/cpu-kernels/awkward_IndexedOptionArray_rpad_and_clip_mask_axis1.cpp` & `awkward-cpp-9/src/cpu-kernels/awkward_IndexedOptionArray_rpad_and_clip_mask_axis1.cpp`

 * *Files identical despite different names*

### Comparing `awkward-cpp-8/src/cpu-kernels/awkward_ListArray_broadcast_tooffsets.cpp` & `awkward-cpp-9/src/cpu-kernels/awkward_ListArray_broadcast_tooffsets.cpp`

 * *Files identical despite different names*

### Comparing `awkward-cpp-8/src/cpu-kernels/awkward_ListArray_combinations.cpp` & `awkward-cpp-9/src/cpu-kernels/awkward_ListArray_combinations.cpp`

 * *Files identical despite different names*

### Comparing `awkward-cpp-8/src/cpu-kernels/awkward_ListArray_combinations_length.cpp` & `awkward-cpp-9/src/cpu-kernels/awkward_ListArray_combinations_length.cpp`

 * *Files identical despite different names*

### Comparing `awkward-cpp-8/src/cpu-kernels/awkward_ListArray_compact_offsets.cpp` & `awkward-cpp-9/src/cpu-kernels/awkward_ListArray_compact_offsets.cpp`

 * *Files identical despite different names*

### Comparing `awkward-cpp-8/src/cpu-kernels/awkward_ListArray_fill.cpp` & `awkward-cpp-9/src/cpu-kernels/awkward_ListArray_fill.cpp`

 * *Files identical despite different names*

### Comparing `awkward-cpp-8/src/cpu-kernels/awkward_ListArray_getitem_jagged_apply.cpp` & `awkward-cpp-9/src/cpu-kernels/awkward_ListArray_getitem_jagged_apply.cpp`

 * *Files identical despite different names*

### Comparing `awkward-cpp-8/src/cpu-kernels/awkward_ListArray_getitem_jagged_carrylen.cpp` & `awkward-cpp-9/src/cpu-kernels/awkward_ListArray_getitem_jagged_carrylen.cpp`

 * *Files identical despite different names*

### Comparing `awkward-cpp-8/src/cpu-kernels/awkward_ListArray_getitem_jagged_descend.cpp` & `awkward-cpp-9/src/cpu-kernels/awkward_ListArray_getitem_jagged_descend.cpp`

 * *Files identical despite different names*

### Comparing `awkward-cpp-8/src/cpu-kernels/awkward_ListArray_getitem_jagged_expand.cpp` & `awkward-cpp-9/src/cpu-kernels/awkward_ListArray_getitem_jagged_expand.cpp`

 * *Files identical despite different names*

### Comparing `awkward-cpp-8/src/cpu-kernels/awkward_ListArray_getitem_jagged_numvalid.cpp` & `awkward-cpp-9/src/cpu-kernels/awkward_ListArray_getitem_jagged_numvalid.cpp`

 * *Files identical despite different names*

### Comparing `awkward-cpp-8/src/cpu-kernels/awkward_ListArray_getitem_jagged_shrink.cpp` & `awkward-cpp-9/src/cpu-kernels/awkward_ListArray_getitem_jagged_shrink.cpp`

 * *Files identical despite different names*

### Comparing `awkward-cpp-8/src/cpu-kernels/awkward_ListArray_getitem_next_array.cpp` & `awkward-cpp-9/src/cpu-kernels/awkward_ListArray_getitem_next_array.cpp`

 * *Files identical despite different names*

### Comparing `awkward-cpp-8/src/cpu-kernels/awkward_ListArray_getitem_next_array_advanced.cpp` & `awkward-cpp-9/src/cpu-kernels/awkward_ListArray_getitem_next_array_advanced.cpp`

 * *Files identical despite different names*

### Comparing `awkward-cpp-8/src/cpu-kernels/awkward_ListArray_getitem_next_at.cpp` & `awkward-cpp-9/src/cpu-kernels/awkward_ListArray_getitem_next_at.cpp`

 * *Files identical despite different names*

### Comparing `awkward-cpp-8/src/cpu-kernels/awkward_ListArray_getitem_next_range.cpp` & `awkward-cpp-9/src/cpu-kernels/awkward_ListArray_getitem_next_range.cpp`

 * *Files identical despite different names*

### Comparing `awkward-cpp-8/src/cpu-kernels/awkward_ListArray_getitem_next_range_carrylength.cpp` & `awkward-cpp-9/src/cpu-kernels/awkward_ListArray_getitem_next_range_carrylength.cpp`

 * *Files identical despite different names*

### Comparing `awkward-cpp-8/src/cpu-kernels/awkward_ListArray_getitem_next_range_counts.cpp` & `awkward-cpp-9/src/cpu-kernels/awkward_ListArray_getitem_next_range_counts.cpp`

 * *Files identical despite different names*

### Comparing `awkward-cpp-8/src/cpu-kernels/awkward_ListArray_getitem_next_range_spreadadvanced.cpp` & `awkward-cpp-9/src/cpu-kernels/awkward_ListArray_getitem_next_range_spreadadvanced.cpp`

 * *Files identical despite different names*

### Comparing `awkward-cpp-8/src/cpu-kernels/awkward_ListArray_localindex.cpp` & `awkward-cpp-9/src/cpu-kernels/awkward_ListArray_localindex.cpp`

 * *Files identical despite different names*

### Comparing `awkward-cpp-8/src/cpu-kernels/awkward_ListArray_min_range.cpp` & `awkward-cpp-9/src/cpu-kernels/awkward_ListArray_min_range.cpp`

 * *Files identical despite different names*

### Comparing `awkward-cpp-8/src/cpu-kernels/awkward_ListArray_rpad_and_clip_length_axis1.cpp` & `awkward-cpp-9/src/cpu-kernels/awkward_ListArray_rpad_and_clip_length_axis1.cpp`

 * *Files identical despite different names*

### Comparing `awkward-cpp-8/src/cpu-kernels/awkward_ListArray_rpad_axis1.cpp` & `awkward-cpp-9/src/cpu-kernels/awkward_ListArray_rpad_axis1.cpp`

 * *Files identical despite different names*

### Comparing `awkward-cpp-8/src/cpu-kernels/awkward_ListArray_validity.cpp` & `awkward-cpp-9/src/cpu-kernels/awkward_ListArray_validity.cpp`

 * *Files identical despite different names*

### Comparing `awkward-cpp-8/src/cpu-kernels/awkward_ListOffsetArray_argsort_strings.cpp` & `awkward-cpp-9/src/cpu-kernels/awkward_ListOffsetArray_argsort_strings.cpp`

 * *Files identical despite different names*

### Comparing `awkward-cpp-8/src/cpu-kernels/awkward_ListOffsetArray_compact_offsets.cpp` & `awkward-cpp-9/src/cpu-kernels/awkward_ListOffsetArray_compact_offsets.cpp`

 * *Files identical despite different names*

### Comparing `awkward-cpp-8/src/cpu-kernels/awkward_ListOffsetArray_drop_none_indexes.cpp` & `awkward-cpp-9/src/cpu-kernels/awkward_ListOffsetArray_drop_none_indexes.cpp`

 * *Files identical despite different names*

### Comparing `awkward-cpp-8/src/cpu-kernels/awkward_ListOffsetArray_flatten_offsets.cpp` & `awkward-cpp-9/src/cpu-kernels/awkward_ListOffsetArray_flatten_offsets.cpp`

 * *Files identical despite different names*

### Comparing `awkward-cpp-8/src/cpu-kernels/awkward_ListOffsetArray_local_preparenext_64.cpp` & `awkward-cpp-9/src/cpu-kernels/awkward_ListOffsetArray_local_preparenext_64.cpp`

 * *Files identical despite different names*

### Comparing `awkward-cpp-8/src/cpu-kernels/awkward_ListOffsetArray_reduce_local_nextparents_64.cpp` & `awkward-cpp-9/src/cpu-kernels/awkward_ListOffsetArray_reduce_local_nextparents_64.cpp`

 * *Files identical despite different names*

### Comparing `awkward-cpp-8/src/cpu-kernels/awkward_ListOffsetArray_reduce_local_outoffsets_64.cpp` & `awkward-cpp-9/src/cpu-kernels/awkward_ListOffsetArray_reduce_local_outoffsets_64.cpp`

 * *Files identical despite different names*

### Comparing `awkward-cpp-8/src/cpu-kernels/awkward_ListOffsetArray_reduce_nonlocal_maxcount_offsetscopy_64.cpp` & `awkward-cpp-9/src/cpu-kernels/awkward_ListOffsetArray_reduce_nonlocal_maxcount_offsetscopy_64.cpp`

 * *Files identical despite different names*

### Comparing `awkward-cpp-8/src/cpu-kernels/awkward_ListOffsetArray_reduce_nonlocal_nextshifts_64.cpp` & `awkward-cpp-9/src/cpu-kernels/awkward_ListOffsetArray_reduce_nonlocal_nextshifts_64.cpp`

 * *Files identical despite different names*

### Comparing `awkward-cpp-8/src/cpu-kernels/awkward_ListOffsetArray_reduce_nonlocal_nextstarts_64.cpp` & `awkward-cpp-9/src/cpu-kernels/awkward_ListOffsetArray_reduce_nonlocal_nextstarts_64.cpp`

 * *Files identical despite different names*

### Comparing `awkward-cpp-8/src/cpu-kernels/awkward_ListOffsetArray_reduce_nonlocal_outstartsstops_64.cpp` & `awkward-cpp-9/src/cpu-kernels/awkward_ListOffsetArray_reduce_nonlocal_outstartsstops_64.cpp`

 * *Files identical despite different names*

### Comparing `awkward-cpp-8/src/cpu-kernels/awkward_ListOffsetArray_reduce_nonlocal_preparenext_64.cpp` & `awkward-cpp-9/src/cpu-kernels/awkward_ListOffsetArray_reduce_nonlocal_preparenext_64.cpp`

 * *Files identical despite different names*

### Comparing `awkward-cpp-8/src/cpu-kernels/awkward_ListOffsetArray_rpad_and_clip_axis1.cpp` & `awkward-cpp-9/src/cpu-kernels/awkward_ListOffsetArray_rpad_and_clip_axis1.cpp`

 * *Files identical despite different names*

### Comparing `awkward-cpp-8/src/cpu-kernels/awkward_ListOffsetArray_rpad_axis1.cpp` & `awkward-cpp-9/src/cpu-kernels/awkward_ListOffsetArray_rpad_axis1.cpp`

 * *Files identical despite different names*

### Comparing `awkward-cpp-8/src/cpu-kernels/awkward_ListOffsetArray_rpad_length_axis1.cpp` & `awkward-cpp-9/src/cpu-kernels/awkward_ListOffsetArray_rpad_length_axis1.cpp`

 * *Files identical despite different names*

### Comparing `awkward-cpp-8/src/cpu-kernels/awkward_ListOffsetArray_toRegularArray.cpp` & `awkward-cpp-9/src/cpu-kernels/awkward_ListOffsetArray_toRegularArray.cpp`

 * *Files identical despite different names*

### Comparing `awkward-cpp-8/src/cpu-kernels/awkward_MaskedArray_getitem_next_jagged_project.cpp` & `awkward-cpp-9/src/cpu-kernels/awkward_MaskedArray_getitem_next_jagged_project.cpp`

 * *Files identical despite different names*

### Comparing `awkward-cpp-8/src/cpu-kernels/awkward_NumpyArray_fill.cpp` & `awkward-cpp-9/src/cpu-kernels/awkward_NumpyArray_fill.cpp`

 * *Files identical despite different names*

### Comparing `awkward-cpp-8/src/cpu-kernels/awkward_NumpyArray_rearrange_shifted.cpp` & `awkward-cpp-9/src/cpu-kernels/awkward_NumpyArray_rearrange_shifted.cpp`

 * *Files identical despite different names*

### Comparing `awkward-cpp-8/src/cpu-kernels/awkward_NumpyArray_reduce_adjust_starts_64.cpp` & `awkward-cpp-9/src/cpu-kernels/awkward_NumpyArray_reduce_adjust_starts_64.cpp`

 * *Files identical despite different names*

### Comparing `awkward-cpp-8/src/cpu-kernels/awkward_NumpyArray_reduce_adjust_starts_shifts_64.cpp` & `awkward-cpp-9/src/cpu-kernels/awkward_NumpyArray_reduce_adjust_starts_shifts_64.cpp`

 * *Files identical despite different names*

### Comparing `awkward-cpp-8/src/cpu-kernels/awkward_NumpyArray_reduce_mask_ByteMaskedArray_64.cpp` & `awkward-cpp-9/src/cpu-kernels/awkward_NumpyArray_reduce_mask_ByteMaskedArray_64.cpp`

 * *Files identical despite different names*

### Comparing `awkward-cpp-8/src/cpu-kernels/awkward_NumpyArray_sort_asstrings_uint8.cpp` & `awkward-cpp-9/src/cpu-kernels/awkward_NumpyArray_sort_asstrings_uint8.cpp`

 * *Files identical despite different names*

### Comparing `awkward-cpp-8/src/cpu-kernels/awkward_NumpyArray_subrange_equal.cpp` & `awkward-cpp-9/src/cpu-kernels/awkward_NumpyArray_subrange_equal.cpp`

 * *Files identical despite different names*

### Comparing `awkward-cpp-8/src/cpu-kernels/awkward_NumpyArray_unique_strings_uint8.cpp` & `awkward-cpp-9/src/cpu-kernels/awkward_NumpyArray_unique_strings_uint8.cpp`

 * *Files identical despite different names*

### Comparing `awkward-cpp-8/src/cpu-kernels/awkward_RegularArray_broadcast_tooffsets.cpp` & `awkward-cpp-9/src/cpu-kernels/awkward_RegularArray_broadcast_tooffsets.cpp`

 * *Files identical despite different names*

### Comparing `awkward-cpp-8/src/cpu-kernels/awkward_RegularArray_broadcast_tooffsets_size1.cpp` & `awkward-cpp-9/src/cpu-kernels/awkward_RegularArray_broadcast_tooffsets_size1.cpp`

 * *Files identical despite different names*

### Comparing `awkward-cpp-8/src/cpu-kernels/awkward_RegularArray_combinations.cpp` & `awkward-cpp-9/src/cpu-kernels/awkward_RegularArray_combinations.cpp`

 * *Files identical despite different names*

### Comparing `awkward-cpp-8/src/cpu-kernels/awkward_RegularArray_compact_offsets.cpp` & `awkward-cpp-9/src/cpu-kernels/awkward_RegularArray_compact_offsets.cpp`

 * *Files identical despite different names*

### Comparing `awkward-cpp-8/src/cpu-kernels/awkward_RegularArray_getitem_carry.cpp` & `awkward-cpp-9/src/cpu-kernels/awkward_RegularArray_getitem_carry.cpp`

 * *Files identical despite different names*

### Comparing `awkward-cpp-8/src/cpu-kernels/awkward_RegularArray_getitem_jagged_expand.cpp` & `awkward-cpp-9/src/cpu-kernels/awkward_RegularArray_getitem_jagged_expand.cpp`

 * *Files identical despite different names*

### Comparing `awkward-cpp-8/src/cpu-kernels/awkward_RegularArray_getitem_next_array.cpp` & `awkward-cpp-9/src/cpu-kernels/awkward_RegularArray_getitem_next_array.cpp`

 * *Files identical despite different names*

### Comparing `awkward-cpp-8/src/cpu-kernels/awkward_RegularArray_getitem_next_array_advanced.cpp` & `awkward-cpp-9/src/cpu-kernels/awkward_RegularArray_getitem_next_array_advanced.cpp`

 * *Files identical despite different names*

### Comparing `awkward-cpp-8/src/cpu-kernels/awkward_RegularArray_getitem_next_array_regularize.cpp` & `awkward-cpp-9/src/cpu-kernels/awkward_RegularArray_getitem_next_array_regularize.cpp`

 * *Files identical despite different names*

### Comparing `awkward-cpp-8/src/cpu-kernels/awkward_RegularArray_getitem_next_at.cpp` & `awkward-cpp-9/src/cpu-kernels/awkward_RegularArray_getitem_next_at.cpp`

 * *Files identical despite different names*

### Comparing `awkward-cpp-8/src/cpu-kernels/awkward_RegularArray_getitem_next_range.cpp` & `awkward-cpp-9/src/cpu-kernels/awkward_RegularArray_getitem_next_range.cpp`

 * *Files identical despite different names*

### Comparing `awkward-cpp-8/src/cpu-kernels/awkward_RegularArray_getitem_next_range_spreadadvanced.cpp` & `awkward-cpp-9/src/cpu-kernels/awkward_RegularArray_getitem_next_range_spreadadvanced.cpp`

 * *Files identical despite different names*

### Comparing `awkward-cpp-8/src/cpu-kernels/awkward_RegularArray_localindex.cpp` & `awkward-cpp-9/src/cpu-kernels/awkward_RegularArray_localindex.cpp`

 * *Files identical despite different names*

### Comparing `awkward-cpp-8/src/cpu-kernels/awkward_RegularArray_reduce_local_nextparents_64.cpp` & `awkward-cpp-9/src/cpu-kernels/awkward_RegularArray_reduce_local_nextparents_64.cpp`

 * *Files identical despite different names*

### Comparing `awkward-cpp-8/src/cpu-kernels/awkward_RegularArray_reduce_nonlocal_preparenext_64.cpp` & `awkward-cpp-9/src/cpu-kernels/awkward_RegularArray_reduce_nonlocal_preparenext_64.cpp`

 * *Files identical despite different names*

### Comparing `awkward-cpp-8/src/cpu-kernels/awkward_RegularArray_rpad_and_clip_axis1.cpp` & `awkward-cpp-9/src/cpu-kernels/awkward_RegularArray_rpad_and_clip_axis1.cpp`

 * *Files identical despite different names*

### Comparing `awkward-cpp-8/src/cpu-kernels/awkward_UnionArray_fillindex.cpp` & `awkward-cpp-9/src/cpu-kernels/awkward_UnionArray_fillindex.cpp`

 * *Files identical despite different names*

### Comparing `awkward-cpp-8/src/cpu-kernels/awkward_UnionArray_fillindex_count.cpp` & `awkward-cpp-9/src/cpu-kernels/awkward_UnionArray_fillindex_count.cpp`

 * *Files identical despite different names*

### Comparing `awkward-cpp-8/src/cpu-kernels/awkward_UnionArray_fillna.cpp` & `awkward-cpp-9/src/cpu-kernels/awkward_UnionArray_fillna.cpp`

 * *Files identical despite different names*

### Comparing `awkward-cpp-8/src/cpu-kernels/awkward_UnionArray_filltags.cpp` & `awkward-cpp-9/src/cpu-kernels/awkward_UnionArray_filltags.cpp`

 * *Files identical despite different names*

### Comparing `awkward-cpp-8/src/cpu-kernels/awkward_UnionArray_filltags_const.cpp` & `awkward-cpp-9/src/cpu-kernels/awkward_UnionArray_filltags_const.cpp`

 * *Files identical despite different names*

### Comparing `awkward-cpp-8/src/cpu-kernels/awkward_UnionArray_flatten_combine.cpp` & `awkward-cpp-9/src/cpu-kernels/awkward_UnionArray_flatten_combine.cpp`

 * *Files identical despite different names*

### Comparing `awkward-cpp-8/src/cpu-kernels/awkward_UnionArray_flatten_length.cpp` & `awkward-cpp-9/src/cpu-kernels/awkward_UnionArray_flatten_length.cpp`

 * *Files identical despite different names*

### Comparing `awkward-cpp-8/src/cpu-kernels/awkward_UnionArray_nestedfill_tags_index.cpp` & `awkward-cpp-9/src/cpu-kernels/awkward_UnionArray_nestedfill_tags_index.cpp`

 * *Files identical despite different names*

### Comparing `awkward-cpp-8/src/cpu-kernels/awkward_UnionArray_project.cpp` & `awkward-cpp-9/src/cpu-kernels/awkward_UnionArray_project.cpp`

 * *Files identical despite different names*

### Comparing `awkward-cpp-8/src/cpu-kernels/awkward_UnionArray_regular_index.cpp` & `awkward-cpp-9/src/cpu-kernels/awkward_UnionArray_regular_index.cpp`

 * *Files identical despite different names*

### Comparing `awkward-cpp-8/src/cpu-kernels/awkward_UnionArray_regular_index_getsize.cpp` & `awkward-cpp-9/src/cpu-kernels/awkward_UnionArray_regular_index_getsize.cpp`

 * *Files identical despite different names*

### Comparing `awkward-cpp-8/src/cpu-kernels/awkward_UnionArray_simplify.cpp` & `awkward-cpp-9/src/cpu-kernels/awkward_UnionArray_simplify.cpp`

 * *Files identical despite different names*

### Comparing `awkward-cpp-8/src/cpu-kernels/awkward_UnionArray_simplify_one.cpp` & `awkward-cpp-9/src/cpu-kernels/awkward_UnionArray_simplify_one.cpp`

 * *Files identical despite different names*

### Comparing `awkward-cpp-8/src/cpu-kernels/awkward_UnionArray_validity.cpp` & `awkward-cpp-9/src/cpu-kernels/awkward_UnionArray_validity.cpp`

 * *Files identical despite different names*

### Comparing `awkward-cpp-8/src/cpu-kernels/awkward_argsort.cpp` & `awkward-cpp-9/src/cpu-kernels/awkward_argsort.cpp`

 * *Files identical despite different names*

### Comparing `awkward-cpp-8/src/cpu-kernels/awkward_index_rpad_and_clip_axis0.cpp` & `awkward-cpp-9/src/cpu-kernels/awkward_index_rpad_and_clip_axis0.cpp`

 * *Files identical despite different names*

### Comparing `awkward-cpp-8/src/cpu-kernels/awkward_index_rpad_and_clip_axis1.cpp` & `awkward-cpp-9/src/cpu-kernels/awkward_index_rpad_and_clip_axis1.cpp`

 * *Files identical despite different names*

### Comparing `awkward-cpp-8/src/cpu-kernels/awkward_localindex.cpp` & `awkward-cpp-9/src/cpu-kernels/awkward_localindex.cpp`

 * *Files identical despite different names*

### Comparing `awkward-cpp-8/src/cpu-kernels/awkward_missing_repeat.cpp` & `awkward-cpp-9/src/cpu-kernels/awkward_missing_repeat.cpp`

 * *Files identical despite different names*

### Comparing `awkward-cpp-8/src/cpu-kernels/awkward_reduce_argmax.cpp` & `awkward-cpp-9/src/cpu-kernels/awkward_reduce_argmax.cpp`

 * *Files identical despite different names*

### Comparing `awkward-cpp-8/src/cpu-kernels/awkward_reduce_argmax_complex.cpp` & `awkward-cpp-9/src/cpu-kernels/awkward_reduce_argmax_complex.cpp`

 * *Files identical despite different names*

### Comparing `awkward-cpp-8/src/cpu-kernels/awkward_reduce_argmin.cpp` & `awkward-cpp-9/src/cpu-kernels/awkward_reduce_argmin.cpp`

 * *Files identical despite different names*

### Comparing `awkward-cpp-8/src/cpu-kernels/awkward_reduce_argmin_complex.cpp` & `awkward-cpp-9/src/cpu-kernels/awkward_reduce_argmin_complex.cpp`

 * *Files identical despite different names*

### Comparing `awkward-cpp-8/src/cpu-kernels/awkward_reduce_countnonzero.cpp` & `awkward-cpp-9/src/cpu-kernels/awkward_reduce_countnonzero.cpp`

 * *Files identical despite different names*

### Comparing `awkward-cpp-8/src/cpu-kernels/awkward_reduce_countnonzero_complex.cpp` & `awkward-cpp-9/src/cpu-kernels/awkward_reduce_countnonzero_complex.cpp`

 * *Files identical despite different names*

### Comparing `awkward-cpp-8/src/cpu-kernels/awkward_reduce_max.cpp` & `awkward-cpp-9/src/cpu-kernels/awkward_reduce_max.cpp`

 * *Files identical despite different names*

### Comparing `awkward-cpp-8/src/cpu-kernels/awkward_reduce_max_complex.cpp` & `awkward-cpp-9/src/cpu-kernels/awkward_reduce_max_complex.cpp`

 * *Files identical despite different names*

### Comparing `awkward-cpp-8/src/cpu-kernels/awkward_reduce_min.cpp` & `awkward-cpp-9/src/cpu-kernels/awkward_reduce_min.cpp`

 * *Files identical despite different names*

### Comparing `awkward-cpp-8/src/cpu-kernels/awkward_reduce_min_complex.cpp` & `awkward-cpp-9/src/cpu-kernels/awkward_reduce_min_complex.cpp`

 * *Files identical despite different names*

### Comparing `awkward-cpp-8/src/cpu-kernels/awkward_reduce_prod.cpp` & `awkward-cpp-9/src/cpu-kernels/awkward_reduce_prod.cpp`

 * *Files identical despite different names*

### Comparing `awkward-cpp-8/src/cpu-kernels/awkward_reduce_prod_bool.cpp` & `awkward-cpp-9/src/cpu-kernels/awkward_reduce_prod_bool.cpp`

 * *Files identical despite different names*

### Comparing `awkward-cpp-8/src/cpu-kernels/awkward_reduce_prod_bool_complex.cpp` & `awkward-cpp-9/src/cpu-kernels/awkward_reduce_prod_bool_complex.cpp`

 * *Files identical despite different names*

### Comparing `awkward-cpp-8/src/cpu-kernels/awkward_reduce_prod_complex.cpp` & `awkward-cpp-9/src/cpu-kernels/awkward_reduce_prod_complex.cpp`

 * *Files identical despite different names*

### Comparing `awkward-cpp-8/src/cpu-kernels/awkward_reduce_sum.cpp` & `awkward-cpp-9/src/cpu-kernels/awkward_reduce_sum.cpp`

 * *Files identical despite different names*

### Comparing `awkward-cpp-8/src/cpu-kernels/awkward_reduce_sum_bool.cpp` & `awkward-cpp-9/src/cpu-kernels/awkward_reduce_sum_bool.cpp`

 * *Files identical despite different names*

### Comparing `awkward-cpp-8/src/cpu-kernels/awkward_reduce_sum_bool_complex.cpp` & `awkward-cpp-9/src/cpu-kernels/awkward_reduce_sum_bool_complex.cpp`

 * *Files identical despite different names*

### Comparing `awkward-cpp-8/src/cpu-kernels/awkward_reduce_sum_complex.cpp` & `awkward-cpp-9/src/cpu-kernels/awkward_reduce_sum_complex.cpp`

 * *Files identical despite different names*

### Comparing `awkward-cpp-8/src/cpu-kernels/awkward_reduce_sum_int32_bool_64.cpp` & `awkward-cpp-9/src/cpu-kernels/awkward_reduce_sum_int32_bool_64.cpp`

 * *Files identical despite different names*

### Comparing `awkward-cpp-8/src/cpu-kernels/awkward_reduce_sum_int64_bool_64.cpp` & `awkward-cpp-9/src/cpu-kernels/awkward_reduce_sum_int64_bool_64.cpp`

 * *Files identical despite different names*

### Comparing `awkward-cpp-8/src/cpu-kernels/awkward_sort.cpp` & `awkward-cpp-9/src/cpu-kernels/awkward_sort.cpp`

 * *Files identical despite different names*

### Comparing `awkward-cpp-8/src/cpu-kernels/awkward_sorting_ranges.cpp` & `awkward-cpp-9/src/cpu-kernels/awkward_sorting_ranges.cpp`

 * *Files identical despite different names*

### Comparing `awkward-cpp-8/src/cpu-kernels/awkward_sorting_ranges_length.cpp` & `awkward-cpp-9/src/cpu-kernels/awkward_sorting_ranges_length.cpp`

 * *Files identical despite different names*

### Comparing `awkward-cpp-8/src/cpu-kernels/awkward_unique.cpp` & `awkward-cpp-9/src/cpu-kernels/awkward_unique.cpp`

 * *Files identical despite different names*

### Comparing `awkward-cpp-8/src/cpu-kernels/awkward_unique_copy.cpp` & `awkward-cpp-9/src/cpu-kernels/awkward_unique_copy.cpp`

 * *Files identical despite different names*

### Comparing `awkward-cpp-8/src/cpu-kernels/awkward_unique_offsets.cpp` & `awkward-cpp-9/src/cpu-kernels/awkward_unique_offsets.cpp`

 * *Files identical despite different names*

### Comparing `awkward-cpp-8/src/cpu-kernels/awkward_unique_ranges.cpp` & `awkward-cpp-9/src/cpu-kernels/awkward_unique_ranges.cpp`

 * *Files identical despite different names*

### Comparing `awkward-cpp-8/src/cpu-kernels/kernel-utils.cpp` & `awkward-cpp-9/src/cpu-kernels/kernel-utils.cpp`

 * *Files identical despite different names*

### Comparing `awkward-cpp-8/src/libawkward/builder/ArrayBuilder.cpp` & `awkward-cpp-9/src/libawkward/builder/ArrayBuilder.cpp`

 * *Files identical despite different names*

### Comparing `awkward-cpp-8/src/libawkward/builder/BoolBuilder.cpp` & `awkward-cpp-9/src/libawkward/builder/BoolBuilder.cpp`

 * *Files identical despite different names*

### Comparing `awkward-cpp-8/src/libawkward/builder/Complex128Builder.cpp` & `awkward-cpp-9/src/libawkward/builder/Complex128Builder.cpp`

 * *Files identical despite different names*

### Comparing `awkward-cpp-8/src/libawkward/builder/DatetimeBuilder.cpp` & `awkward-cpp-9/src/libawkward/builder/DatetimeBuilder.cpp`

 * *Files identical despite different names*

### Comparing `awkward-cpp-8/src/libawkward/builder/Float64Builder.cpp` & `awkward-cpp-9/src/libawkward/builder/Float64Builder.cpp`

 * *Files identical despite different names*

### Comparing `awkward-cpp-8/src/libawkward/builder/Int64Builder.cpp` & `awkward-cpp-9/src/libawkward/builder/Int64Builder.cpp`

 * *Files identical despite different names*

### Comparing `awkward-cpp-8/src/libawkward/builder/ListBuilder.cpp` & `awkward-cpp-9/src/libawkward/builder/ListBuilder.cpp`

 * *Files identical despite different names*

### Comparing `awkward-cpp-8/src/libawkward/builder/OptionBuilder.cpp` & `awkward-cpp-9/src/libawkward/builder/OptionBuilder.cpp`

 * *Files identical despite different names*

### Comparing `awkward-cpp-8/src/libawkward/builder/RecordBuilder.cpp` & `awkward-cpp-9/src/libawkward/builder/RecordBuilder.cpp`

 * *Files identical despite different names*

### Comparing `awkward-cpp-8/src/libawkward/builder/StringBuilder.cpp` & `awkward-cpp-9/src/libawkward/builder/StringBuilder.cpp`

 * *Files identical despite different names*

### Comparing `awkward-cpp-8/src/libawkward/builder/TupleBuilder.cpp` & `awkward-cpp-9/src/libawkward/builder/TupleBuilder.cpp`

 * *Files identical despite different names*

### Comparing `awkward-cpp-8/src/libawkward/builder/UnionBuilder.cpp` & `awkward-cpp-9/src/libawkward/builder/UnionBuilder.cpp`

 * *Files identical despite different names*

### Comparing `awkward-cpp-8/src/libawkward/builder/UnknownBuilder.cpp` & `awkward-cpp-9/src/libawkward/builder/UnknownBuilder.cpp`

 * *Files identical despite different names*

### Comparing `awkward-cpp-8/src/libawkward/forth/ForthInputBuffer.cpp` & `awkward-cpp-9/src/libawkward/forth/ForthInputBuffer.cpp`

 * *Files identical despite different names*

### Comparing `awkward-cpp-8/src/libawkward/forth/ForthMachine.cpp` & `awkward-cpp-9/src/libawkward/forth/ForthMachine.cpp`

 * *Files identical despite different names*

### Comparing `awkward-cpp-8/src/libawkward/forth/ForthOutputBuffer.cpp` & `awkward-cpp-9/src/libawkward/forth/ForthOutputBuffer.cpp`

 * *Files identical despite different names*

### Comparing `awkward-cpp-8/src/libawkward/io/json.cpp` & `awkward-cpp-9/src/libawkward/io/json.cpp`

 * *Files identical despite different names*

### Comparing `awkward-cpp-8/src/libawkward/util.cpp` & `awkward-cpp-9/src/libawkward/util.cpp`

 * *Files identical despite different names*

### Comparing `awkward-cpp-8/src/python/_ext.cpp` & `awkward-cpp-9/src/python/_ext.cpp`

 * *Files identical despite different names*

### Comparing `awkward-cpp-8/src/python/content.cpp` & `awkward-cpp-9/src/python/content.cpp`

 * *Files identical despite different names*

### Comparing `awkward-cpp-8/src/python/forth.cpp` & `awkward-cpp-9/src/python/forth.cpp`

 * *Files identical despite different names*

### Comparing `awkward-cpp-8/src/python/io.cpp` & `awkward-cpp-9/src/python/io.cpp`

 * *Files identical despite different names*

### Comparing `awkward-cpp-8/tests-cpu-kernels/test_cpuawkward_BitMaskedArray_to_ByteMaskedArray.py` & `awkward-cpp-9/tests-cpu-kernels/test_cpuawkward_BitMaskedArray_to_ByteMaskedArray.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# AUTO GENERATED ON 2023-02-03 AT 22:54:31
+# AUTO GENERATED ON 2023-02-16 AT 15:37:39
 # DO NOT EDIT BY HAND!
 #
 # To regenerate file, run
 #
 #     python dev/generate-tests.py
 #
```

### Comparing `awkward-cpp-8/tests-cpu-kernels/test_cpuawkward_BitMaskedArray_to_IndexedOptionArray64.py` & `awkward-cpp-9/tests-cpu-kernels/test_cpuawkward_BitMaskedArray_to_IndexedOptionArray64.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# AUTO GENERATED ON 2023-02-03 AT 22:54:31
+# AUTO GENERATED ON 2023-02-16 AT 15:37:39
 # DO NOT EDIT BY HAND!
 #
 # To regenerate file, run
 #
 #     python dev/generate-tests.py
 #
```

### Comparing `awkward-cpp-8/tests-cpu-kernels/test_cpuawkward_ByteMaskedArray_getitem_nextcarry_64.py` & `awkward-cpp-9/tests-cpu-kernels/test_cpuawkward_ByteMaskedArray_getitem_nextcarry_64.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# AUTO GENERATED ON 2023-02-03 AT 22:54:31
+# AUTO GENERATED ON 2023-02-16 AT 15:37:39
 # DO NOT EDIT BY HAND!
 #
 # To regenerate file, run
 #
 #     python dev/generate-tests.py
 #
```

### Comparing `awkward-cpp-8/tests-cpu-kernels/test_cpuawkward_ByteMaskedArray_getitem_nextcarry_outindex_64.py` & `awkward-cpp-9/tests-cpu-kernels/test_cpuawkward_ByteMaskedArray_getitem_nextcarry_outindex_64.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# AUTO GENERATED ON 2023-02-03 AT 22:54:31
+# AUTO GENERATED ON 2023-02-16 AT 15:37:39
 # DO NOT EDIT BY HAND!
 #
 # To regenerate file, run
 #
 #     python dev/generate-tests.py
 #
```

### Comparing `awkward-cpp-8/tests-cpu-kernels/test_cpuawkward_ByteMaskedArray_numnull.py` & `awkward-cpp-9/tests-cpu-kernels/test_cpuawkward_ByteMaskedArray_numnull.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# AUTO GENERATED ON 2023-02-03 AT 22:54:31
+# AUTO GENERATED ON 2023-02-16 AT 15:37:39
 # DO NOT EDIT BY HAND!
 #
 # To regenerate file, run
 #
 #     python dev/generate-tests.py
 #
```

### Comparing `awkward-cpp-8/tests-cpu-kernels/test_cpuawkward_ByteMaskedArray_overlay_mask8.py` & `awkward-cpp-9/tests-cpu-kernels/test_cpuawkward_ByteMaskedArray_overlay_mask8.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# AUTO GENERATED ON 2023-02-03 AT 22:54:31
+# AUTO GENERATED ON 2023-02-16 AT 15:37:39
 # DO NOT EDIT BY HAND!
 #
 # To regenerate file, run
 #
 #     python dev/generate-tests.py
 #
```

### Comparing `awkward-cpp-8/tests-cpu-kernels/test_cpuawkward_ByteMaskedArray_toIndexedOptionArray64.py` & `awkward-cpp-9/tests-cpu-kernels/test_cpuawkward_ByteMaskedArray_toIndexedOptionArray64.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# AUTO GENERATED ON 2023-02-03 AT 22:54:31
+# AUTO GENERATED ON 2023-02-16 AT 15:37:39
 # DO NOT EDIT BY HAND!
 #
 # To regenerate file, run
 #
 #     python dev/generate-tests.py
 #
```

### Comparing `awkward-cpp-8/tests-cpu-kernels/test_cpuawkward_Content_getitem_next_missing_jagged_getmaskstartstop.py` & `awkward-cpp-9/tests-cpu-kernels/test_cpuawkward_Content_getitem_next_missing_jagged_getmaskstartstop.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# AUTO GENERATED ON 2023-02-03 AT 22:54:31
+# AUTO GENERATED ON 2023-02-16 AT 15:37:39
 # DO NOT EDIT BY HAND!
 #
 # To regenerate file, run
 #
 #     python dev/generate-tests.py
 #
```

### Comparing `awkward-cpp-8/tests-cpu-kernels/test_cpuawkward_IndexedArray32_flatten_nextcarry_64.py` & `awkward-cpp-9/tests-cpu-kernels/test_cpuawkward_IndexedArray32_flatten_nextcarry_64.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# AUTO GENERATED ON 2023-02-03 AT 22:54:31
+# AUTO GENERATED ON 2023-02-16 AT 15:37:39
 # DO NOT EDIT BY HAND!
 #
 # To regenerate file, run
 #
 #     python dev/generate-tests.py
 #
```

### Comparing `awkward-cpp-8/tests-cpu-kernels/test_cpuawkward_IndexedArray32_flatten_none2empty_64.py` & `awkward-cpp-9/tests-cpu-kernels/test_cpuawkward_IndexedArray32_flatten_none2empty_64.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# AUTO GENERATED ON 2023-02-03 AT 22:54:31
+# AUTO GENERATED ON 2023-02-16 AT 15:37:39
 # DO NOT EDIT BY HAND!
 #
 # To regenerate file, run
 #
 #     python dev/generate-tests.py
 #
```

### Comparing `awkward-cpp-8/tests-cpu-kernels/test_cpuawkward_IndexedArray32_getitem_nextcarry_64.py` & `awkward-cpp-9/tests-cpu-kernels/test_cpuawkward_IndexedArray32_getitem_nextcarry_64.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# AUTO GENERATED ON 2023-02-03 AT 22:54:31
+# AUTO GENERATED ON 2023-02-16 AT 15:37:39
 # DO NOT EDIT BY HAND!
 #
 # To regenerate file, run
 #
 #     python dev/generate-tests.py
 #
```

### Comparing `awkward-cpp-8/tests-cpu-kernels/test_cpuawkward_IndexedArray32_getitem_nextcarry_outindex_64.py` & `awkward-cpp-9/tests-cpu-kernels/test_cpuawkward_IndexedArray32_getitem_nextcarry_outindex_64.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# AUTO GENERATED ON 2023-02-03 AT 22:54:31
+# AUTO GENERATED ON 2023-02-16 AT 15:37:39
 # DO NOT EDIT BY HAND!
 #
 # To regenerate file, run
 #
 #     python dev/generate-tests.py
 #
```

### Comparing `awkward-cpp-8/tests-cpu-kernels/test_cpuawkward_IndexedArray32_numnull.py` & `awkward-cpp-9/tests-cpu-kernels/test_cpuawkward_IndexedArray32_numnull.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# AUTO GENERATED ON 2023-02-03 AT 22:54:31
+# AUTO GENERATED ON 2023-02-16 AT 15:37:39
 # DO NOT EDIT BY HAND!
 #
 # To regenerate file, run
 #
 #     python dev/generate-tests.py
 #
```

### Comparing `awkward-cpp-8/tests-cpu-kernels/test_cpuawkward_IndexedArray32_simplify32_to64.py` & `awkward-cpp-9/tests-cpu-kernels/test_cpuawkward_IndexedArray32_simplify32_to64.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# AUTO GENERATED ON 2023-02-03 AT 22:54:31
+# AUTO GENERATED ON 2023-02-16 AT 15:37:39
 # DO NOT EDIT BY HAND!
 #
 # To regenerate file, run
 #
 #     python dev/generate-tests.py
 #
```

### Comparing `awkward-cpp-8/tests-cpu-kernels/test_cpuawkward_IndexedArray32_simplify64_to64.py` & `awkward-cpp-9/tests-cpu-kernels/test_cpuawkward_IndexedArray32_simplify64_to64.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# AUTO GENERATED ON 2023-02-03 AT 22:54:31
+# AUTO GENERATED ON 2023-02-16 AT 15:37:39
 # DO NOT EDIT BY HAND!
 #
 # To regenerate file, run
 #
 #     python dev/generate-tests.py
 #
```

### Comparing `awkward-cpp-8/tests-cpu-kernels/test_cpuawkward_IndexedArray32_simplifyU32_to64.py` & `awkward-cpp-9/tests-cpu-kernels/test_cpuawkward_IndexedArray32_simplifyU32_to64.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# AUTO GENERATED ON 2023-02-03 AT 22:54:31
+# AUTO GENERATED ON 2023-02-16 AT 15:37:39
 # DO NOT EDIT BY HAND!
 #
 # To regenerate file, run
 #
 #     python dev/generate-tests.py
 #
```

### Comparing `awkward-cpp-8/tests-cpu-kernels/test_cpuawkward_IndexedArray32_validity.py` & `awkward-cpp-9/tests-cpu-kernels/test_cpuawkward_IndexedArray32_validity.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# AUTO GENERATED ON 2023-02-03 AT 22:54:31
+# AUTO GENERATED ON 2023-02-16 AT 15:37:39
 # DO NOT EDIT BY HAND!
 #
 # To regenerate file, run
 #
 #     python dev/generate-tests.py
 #
```

### Comparing `awkward-cpp-8/tests-cpu-kernels/test_cpuawkward_IndexedArray64_flatten_nextcarry_64.py` & `awkward-cpp-9/tests-cpu-kernels/test_cpuawkward_IndexedArray64_flatten_nextcarry_64.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# AUTO GENERATED ON 2023-02-03 AT 22:54:31
+# AUTO GENERATED ON 2023-02-16 AT 15:37:39
 # DO NOT EDIT BY HAND!
 #
 # To regenerate file, run
 #
 #     python dev/generate-tests.py
 #
```

### Comparing `awkward-cpp-8/tests-cpu-kernels/test_cpuawkward_IndexedArray64_flatten_none2empty_64.py` & `awkward-cpp-9/tests-cpu-kernels/test_cpuawkward_IndexedArray64_flatten_none2empty_64.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# AUTO GENERATED ON 2023-02-03 AT 22:54:31
+# AUTO GENERATED ON 2023-02-16 AT 15:37:39
 # DO NOT EDIT BY HAND!
 #
 # To regenerate file, run
 #
 #     python dev/generate-tests.py
 #
```

### Comparing `awkward-cpp-8/tests-cpu-kernels/test_cpuawkward_IndexedArray64_getitem_nextcarry_64.py` & `awkward-cpp-9/tests-cpu-kernels/test_cpuawkward_IndexedArray64_getitem_nextcarry_64.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# AUTO GENERATED ON 2023-02-03 AT 22:54:31
+# AUTO GENERATED ON 2023-02-16 AT 15:37:39
 # DO NOT EDIT BY HAND!
 #
 # To regenerate file, run
 #
 #     python dev/generate-tests.py
 #
```

### Comparing `awkward-cpp-8/tests-cpu-kernels/test_cpuawkward_IndexedArray64_getitem_nextcarry_outindex_64.py` & `awkward-cpp-9/tests-cpu-kernels/test_cpuawkward_IndexedArray64_getitem_nextcarry_outindex_64.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# AUTO GENERATED ON 2023-02-03 AT 22:54:31
+# AUTO GENERATED ON 2023-02-16 AT 15:37:39
 # DO NOT EDIT BY HAND!
 #
 # To regenerate file, run
 #
 #     python dev/generate-tests.py
 #
```

### Comparing `awkward-cpp-8/tests-cpu-kernels/test_cpuawkward_IndexedArray64_numnull.py` & `awkward-cpp-9/tests-cpu-kernels/test_cpuawkward_IndexedArray64_numnull.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# AUTO GENERATED ON 2023-02-03 AT 22:54:31
+# AUTO GENERATED ON 2023-02-16 AT 15:37:39
 # DO NOT EDIT BY HAND!
 #
 # To regenerate file, run
 #
 #     python dev/generate-tests.py
 #
```

### Comparing `awkward-cpp-8/tests-cpu-kernels/test_cpuawkward_IndexedArray64_simplify32_to64.py` & `awkward-cpp-9/tests-cpu-kernels/test_cpuawkward_IndexedArray64_simplify32_to64.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# AUTO GENERATED ON 2023-02-03 AT 22:54:31
+# AUTO GENERATED ON 2023-02-16 AT 15:37:39
 # DO NOT EDIT BY HAND!
 #
 # To regenerate file, run
 #
 #     python dev/generate-tests.py
 #
```

### Comparing `awkward-cpp-8/tests-cpu-kernels/test_cpuawkward_IndexedArray64_simplify64_to64.py` & `awkward-cpp-9/tests-cpu-kernels/test_cpuawkward_IndexedArray64_simplify64_to64.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# AUTO GENERATED ON 2023-02-03 AT 22:54:31
+# AUTO GENERATED ON 2023-02-16 AT 15:37:39
 # DO NOT EDIT BY HAND!
 #
 # To regenerate file, run
 #
 #     python dev/generate-tests.py
 #
```

### Comparing `awkward-cpp-8/tests-cpu-kernels/test_cpuawkward_IndexedArray64_simplifyU32_to64.py` & `awkward-cpp-9/tests-cpu-kernels/test_cpuawkward_IndexedArray64_simplifyU32_to64.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# AUTO GENERATED ON 2023-02-03 AT 22:54:31
+# AUTO GENERATED ON 2023-02-16 AT 15:37:39
 # DO NOT EDIT BY HAND!
 #
 # To regenerate file, run
 #
 #     python dev/generate-tests.py
 #
```

### Comparing `awkward-cpp-8/tests-cpu-kernels/test_cpuawkward_IndexedArray64_validity.py` & `awkward-cpp-9/tests-cpu-kernels/test_cpuawkward_IndexedArray64_validity.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# AUTO GENERATED ON 2023-02-03 AT 22:54:31
+# AUTO GENERATED ON 2023-02-16 AT 15:37:39
 # DO NOT EDIT BY HAND!
 #
 # To regenerate file, run
 #
 #     python dev/generate-tests.py
 #
```

### Comparing `awkward-cpp-8/tests-cpu-kernels/test_cpuawkward_IndexedArrayU32_flatten_nextcarry_64.py` & `awkward-cpp-9/tests-cpu-kernels/test_cpuawkward_IndexedArrayU32_flatten_nextcarry_64.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# AUTO GENERATED ON 2023-02-03 AT 22:54:31
+# AUTO GENERATED ON 2023-02-16 AT 15:37:39
 # DO NOT EDIT BY HAND!
 #
 # To regenerate file, run
 #
 #     python dev/generate-tests.py
 #
```

### Comparing `awkward-cpp-8/tests-cpu-kernels/test_cpuawkward_IndexedArrayU32_flatten_none2empty_64.py` & `awkward-cpp-9/tests-cpu-kernels/test_cpuawkward_IndexedArrayU32_flatten_none2empty_64.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# AUTO GENERATED ON 2023-02-03 AT 22:54:31
+# AUTO GENERATED ON 2023-02-16 AT 15:37:39
 # DO NOT EDIT BY HAND!
 #
 # To regenerate file, run
 #
 #     python dev/generate-tests.py
 #
```

### Comparing `awkward-cpp-8/tests-cpu-kernels/test_cpuawkward_IndexedArrayU32_getitem_nextcarry_64.py` & `awkward-cpp-9/tests-cpu-kernels/test_cpuawkward_IndexedArrayU32_getitem_nextcarry_64.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# AUTO GENERATED ON 2023-02-03 AT 22:54:31
+# AUTO GENERATED ON 2023-02-16 AT 15:37:39
 # DO NOT EDIT BY HAND!
 #
 # To regenerate file, run
 #
 #     python dev/generate-tests.py
 #
```

### Comparing `awkward-cpp-8/tests-cpu-kernels/test_cpuawkward_IndexedArrayU32_getitem_nextcarry_outindex_64.py` & `awkward-cpp-9/tests-cpu-kernels/test_cpuawkward_IndexedArrayU32_getitem_nextcarry_outindex_64.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# AUTO GENERATED ON 2023-02-03 AT 22:54:31
+# AUTO GENERATED ON 2023-02-16 AT 15:37:39
 # DO NOT EDIT BY HAND!
 #
 # To regenerate file, run
 #
 #     python dev/generate-tests.py
 #
```

### Comparing `awkward-cpp-8/tests-cpu-kernels/test_cpuawkward_IndexedArrayU32_numnull.py` & `awkward-cpp-9/tests-cpu-kernels/test_cpuawkward_IndexedArrayU32_numnull.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# AUTO GENERATED ON 2023-02-03 AT 22:54:31
+# AUTO GENERATED ON 2023-02-16 AT 15:37:39
 # DO NOT EDIT BY HAND!
 #
 # To regenerate file, run
 #
 #     python dev/generate-tests.py
 #
```

### Comparing `awkward-cpp-8/tests-cpu-kernels/test_cpuawkward_IndexedArrayU32_simplify32_to64.py` & `awkward-cpp-9/tests-cpu-kernels/test_cpuawkward_IndexedArrayU32_simplify32_to64.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# AUTO GENERATED ON 2023-02-03 AT 22:54:31
+# AUTO GENERATED ON 2023-02-16 AT 15:37:39
 # DO NOT EDIT BY HAND!
 #
 # To regenerate file, run
 #
 #     python dev/generate-tests.py
 #
```

### Comparing `awkward-cpp-8/tests-cpu-kernels/test_cpuawkward_IndexedArrayU32_simplify64_to64.py` & `awkward-cpp-9/tests-cpu-kernels/test_cpuawkward_IndexedArrayU32_simplify64_to64.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# AUTO GENERATED ON 2023-02-03 AT 22:54:31
+# AUTO GENERATED ON 2023-02-16 AT 15:37:39
 # DO NOT EDIT BY HAND!
 #
 # To regenerate file, run
 #
 #     python dev/generate-tests.py
 #
```

### Comparing `awkward-cpp-8/tests-cpu-kernels/test_cpuawkward_IndexedArrayU32_simplifyU32_to64.py` & `awkward-cpp-9/tests-cpu-kernels/test_cpuawkward_IndexedArrayU32_simplifyU32_to64.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# AUTO GENERATED ON 2023-02-03 AT 22:54:31
+# AUTO GENERATED ON 2023-02-16 AT 15:37:39
 # DO NOT EDIT BY HAND!
 #
 # To regenerate file, run
 #
 #     python dev/generate-tests.py
 #
```

### Comparing `awkward-cpp-8/tests-cpu-kernels/test_cpuawkward_IndexedArrayU32_validity.py` & `awkward-cpp-9/tests-cpu-kernels/test_cpuawkward_IndexedArrayU32_validity.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# AUTO GENERATED ON 2023-02-03 AT 22:54:31
+# AUTO GENERATED ON 2023-02-16 AT 15:37:39
 # DO NOT EDIT BY HAND!
 #
 # To regenerate file, run
 #
 #     python dev/generate-tests.py
 #
```

### Comparing `awkward-cpp-8/tests-cpu-kernels/test_cpuawkward_IndexedArray_fill_to64_count.py` & `awkward-cpp-9/tests-cpu-kernels/test_cpuawkward_IndexedArray_fill_to64_count.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# AUTO GENERATED ON 2023-02-03 AT 22:54:31
+# AUTO GENERATED ON 2023-02-16 AT 15:37:39
 # DO NOT EDIT BY HAND!
 #
 # To regenerate file, run
 #
 #     python dev/generate-tests.py
 #
```

### Comparing `awkward-cpp-8/tests-cpu-kernels/test_cpuawkward_IndexedArray_fill_to64_from32.py` & `awkward-cpp-9/tests-cpu-kernels/test_cpuawkward_IndexedArray_fill_to64_from32.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# AUTO GENERATED ON 2023-02-03 AT 22:54:31
+# AUTO GENERATED ON 2023-02-16 AT 15:37:39
 # DO NOT EDIT BY HAND!
 #
 # To regenerate file, run
 #
 #     python dev/generate-tests.py
 #
```

### Comparing `awkward-cpp-8/tests-cpu-kernels/test_cpuawkward_IndexedArray_fill_to64_from64.py` & `awkward-cpp-9/tests-cpu-kernels/test_cpuawkward_IndexedArray_fill_to64_from64.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# AUTO GENERATED ON 2023-02-03 AT 22:54:31
+# AUTO GENERATED ON 2023-02-16 AT 15:37:39
 # DO NOT EDIT BY HAND!
 #
 # To regenerate file, run
 #
 #     python dev/generate-tests.py
 #
```

### Comparing `awkward-cpp-8/tests-cpu-kernels/test_cpuawkward_IndexedArray_fill_to64_fromU32.py` & `awkward-cpp-9/tests-cpu-kernels/test_cpuawkward_IndexedArray_fill_to64_fromU32.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# AUTO GENERATED ON 2023-02-03 AT 22:54:31
+# AUTO GENERATED ON 2023-02-16 AT 15:37:39
 # DO NOT EDIT BY HAND!
 #
 # To regenerate file, run
 #
 #     python dev/generate-tests.py
 #
```

### Comparing `awkward-cpp-8/tests-cpu-kernels/test_cpuawkward_IndexedOptionArray_rpad_and_clip_mask_axis1_64.py` & `awkward-cpp-9/tests-cpu-kernels/test_cpuawkward_IndexedOptionArray_rpad_and_clip_mask_axis1_64.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# AUTO GENERATED ON 2023-02-03 AT 22:54:31
+# AUTO GENERATED ON 2023-02-16 AT 15:37:39
 # DO NOT EDIT BY HAND!
 #
 # To regenerate file, run
 #
 #     python dev/generate-tests.py
 #
```

### Comparing `awkward-cpp-8/tests-cpu-kernels/test_cpuawkward_ListArray32_broadcast_tooffsets_64.py` & `awkward-cpp-9/tests-cpu-kernels/test_cpuawkward_ListArray32_broadcast_tooffsets_64.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# AUTO GENERATED ON 2023-02-03 AT 22:54:31
+# AUTO GENERATED ON 2023-02-16 AT 15:37:39
 # DO NOT EDIT BY HAND!
 #
 # To regenerate file, run
 #
 #     python dev/generate-tests.py
 #
```

### Comparing `awkward-cpp-8/tests-cpu-kernels/test_cpuawkward_ListArray32_combinations_length_64.py` & `awkward-cpp-9/tests-cpu-kernels/test_cpuawkward_ListArray32_combinations_length_64.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# AUTO GENERATED ON 2023-02-03 AT 22:54:31
+# AUTO GENERATED ON 2023-02-16 AT 15:37:39
 # DO NOT EDIT BY HAND!
 #
 # To regenerate file, run
 #
 #     python dev/generate-tests.py
 #
```

### Comparing `awkward-cpp-8/tests-cpu-kernels/test_cpuawkward_ListArray32_compact_offsets_64.py` & `awkward-cpp-9/tests-cpu-kernels/test_cpuawkward_ListArray32_compact_offsets_64.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# AUTO GENERATED ON 2023-02-03 AT 22:54:31
+# AUTO GENERATED ON 2023-02-16 AT 15:37:39
 # DO NOT EDIT BY HAND!
 #
 # To regenerate file, run
 #
 #     python dev/generate-tests.py
 #
```

### Comparing `awkward-cpp-8/tests-cpu-kernels/test_cpuawkward_ListArray32_getitem_jagged_apply_64.py` & `awkward-cpp-9/tests-cpu-kernels/test_cpuawkward_ListArray32_getitem_jagged_apply_64.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# AUTO GENERATED ON 2023-02-03 AT 22:54:31
+# AUTO GENERATED ON 2023-02-16 AT 15:37:39
 # DO NOT EDIT BY HAND!
 #
 # To regenerate file, run
 #
 #     python dev/generate-tests.py
 #
```

### Comparing `awkward-cpp-8/tests-cpu-kernels/test_cpuawkward_ListArray32_getitem_jagged_descend_64.py` & `awkward-cpp-9/tests-cpu-kernels/test_cpuawkward_ListArray32_getitem_jagged_descend_64.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# AUTO GENERATED ON 2023-02-03 AT 22:54:31
+# AUTO GENERATED ON 2023-02-16 AT 15:37:39
 # DO NOT EDIT BY HAND!
 #
 # To regenerate file, run
 #
 #     python dev/generate-tests.py
 #
```

### Comparing `awkward-cpp-8/tests-cpu-kernels/test_cpuawkward_ListArray32_getitem_jagged_expand_64.py` & `awkward-cpp-9/tests-cpu-kernels/test_cpuawkward_ListArray32_getitem_jagged_expand_64.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# AUTO GENERATED ON 2023-02-03 AT 22:54:31
+# AUTO GENERATED ON 2023-02-16 AT 15:37:39
 # DO NOT EDIT BY HAND!
 #
 # To regenerate file, run
 #
 #     python dev/generate-tests.py
 #
```

### Comparing `awkward-cpp-8/tests-cpu-kernels/test_cpuawkward_ListArray32_getitem_next_array_64.py` & `awkward-cpp-9/tests-cpu-kernels/test_cpuawkward_ListArray32_getitem_next_array_64.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# AUTO GENERATED ON 2023-02-03 AT 22:54:31
+# AUTO GENERATED ON 2023-02-16 AT 15:37:39
 # DO NOT EDIT BY HAND!
 #
 # To regenerate file, run
 #
 #     python dev/generate-tests.py
 #
```

### Comparing `awkward-cpp-8/tests-cpu-kernels/test_cpuawkward_ListArray32_getitem_next_array_advanced_64.py` & `awkward-cpp-9/tests-cpu-kernels/test_cpuawkward_ListArray32_getitem_next_array_advanced_64.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# AUTO GENERATED ON 2023-02-03 AT 22:54:31
+# AUTO GENERATED ON 2023-02-16 AT 15:37:39
 # DO NOT EDIT BY HAND!
 #
 # To regenerate file, run
 #
 #     python dev/generate-tests.py
 #
```

### Comparing `awkward-cpp-8/tests-cpu-kernels/test_cpuawkward_ListArray32_getitem_next_at_64.py` & `awkward-cpp-9/tests-cpu-kernels/test_cpuawkward_ListArray32_getitem_next_at_64.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# AUTO GENERATED ON 2023-02-03 AT 22:54:31
+# AUTO GENERATED ON 2023-02-16 AT 15:37:39
 # DO NOT EDIT BY HAND!
 #
 # To regenerate file, run
 #
 #     python dev/generate-tests.py
 #
```

### Comparing `awkward-cpp-8/tests-cpu-kernels/test_cpuawkward_ListArray32_getitem_next_range_counts_64.py` & `awkward-cpp-9/tests-cpu-kernels/test_cpuawkward_ListArray32_getitem_next_range_counts_64.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# AUTO GENERATED ON 2023-02-03 AT 22:54:31
+# AUTO GENERATED ON 2023-02-16 AT 15:37:39
 # DO NOT EDIT BY HAND!
 #
 # To regenerate file, run
 #
 #     python dev/generate-tests.py
 #
```

### Comparing `awkward-cpp-8/tests-cpu-kernels/test_cpuawkward_ListArray32_localindex_64.py` & `awkward-cpp-9/tests-cpu-kernels/test_cpuawkward_ListArray32_localindex_64.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# AUTO GENERATED ON 2023-02-03 AT 22:54:31
+# AUTO GENERATED ON 2023-02-16 AT 15:37:39
 # DO NOT EDIT BY HAND!
 #
 # To regenerate file, run
 #
 #     python dev/generate-tests.py
 #
```

### Comparing `awkward-cpp-8/tests-cpu-kernels/test_cpuawkward_ListArray32_min_range.py` & `awkward-cpp-9/tests-cpu-kernels/test_cpuawkward_ListArray32_min_range.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# AUTO GENERATED ON 2023-02-03 AT 22:54:31
+# AUTO GENERATED ON 2023-02-16 AT 15:37:39
 # DO NOT EDIT BY HAND!
 #
 # To regenerate file, run
 #
 #     python dev/generate-tests.py
 #
```

### Comparing `awkward-cpp-8/tests-cpu-kernels/test_cpuawkward_ListArray32_rpad_and_clip_length_axis1.py` & `awkward-cpp-9/tests-cpu-kernels/test_cpuawkward_ListArray32_rpad_and_clip_length_axis1.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# AUTO GENERATED ON 2023-02-03 AT 22:54:31
+# AUTO GENERATED ON 2023-02-16 AT 15:37:39
 # DO NOT EDIT BY HAND!
 #
 # To regenerate file, run
 #
 #     python dev/generate-tests.py
 #
```

### Comparing `awkward-cpp-8/tests-cpu-kernels/test_cpuawkward_ListArray32_rpad_axis1_64.py` & `awkward-cpp-9/tests-cpu-kernels/test_cpuawkward_ListArray32_rpad_axis1_64.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# AUTO GENERATED ON 2023-02-03 AT 22:54:31
+# AUTO GENERATED ON 2023-02-16 AT 15:37:39
 # DO NOT EDIT BY HAND!
 #
 # To regenerate file, run
 #
 #     python dev/generate-tests.py
 #
```

### Comparing `awkward-cpp-8/tests-cpu-kernels/test_cpuawkward_ListArray32_validity.py` & `awkward-cpp-9/tests-cpu-kernels/test_cpuawkward_ListArray32_validity.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# AUTO GENERATED ON 2023-02-03 AT 22:54:31
+# AUTO GENERATED ON 2023-02-16 AT 15:37:39
 # DO NOT EDIT BY HAND!
 #
 # To regenerate file, run
 #
 #     python dev/generate-tests.py
 #
```

### Comparing `awkward-cpp-8/tests-cpu-kernels/test_cpuawkward_ListArray64_broadcast_tooffsets_64.py` & `awkward-cpp-9/tests-cpu-kernels/test_cpuawkward_ListArray64_broadcast_tooffsets_64.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# AUTO GENERATED ON 2023-02-03 AT 22:54:31
+# AUTO GENERATED ON 2023-02-16 AT 15:37:39
 # DO NOT EDIT BY HAND!
 #
 # To regenerate file, run
 #
 #     python dev/generate-tests.py
 #
```

### Comparing `awkward-cpp-8/tests-cpu-kernels/test_cpuawkward_ListArray64_combinations_length_64.py` & `awkward-cpp-9/tests-cpu-kernels/test_cpuawkward_ListArray64_combinations_length_64.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# AUTO GENERATED ON 2023-02-03 AT 22:54:31
+# AUTO GENERATED ON 2023-02-16 AT 15:37:39
 # DO NOT EDIT BY HAND!
 #
 # To regenerate file, run
 #
 #     python dev/generate-tests.py
 #
```

### Comparing `awkward-cpp-8/tests-cpu-kernels/test_cpuawkward_ListArray64_compact_offsets_64.py` & `awkward-cpp-9/tests-cpu-kernels/test_cpuawkward_ListArray64_compact_offsets_64.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# AUTO GENERATED ON 2023-02-03 AT 22:54:31
+# AUTO GENERATED ON 2023-02-16 AT 15:37:39
 # DO NOT EDIT BY HAND!
 #
 # To regenerate file, run
 #
 #     python dev/generate-tests.py
 #
```

### Comparing `awkward-cpp-8/tests-cpu-kernels/test_cpuawkward_ListArray64_getitem_jagged_apply_64.py` & `awkward-cpp-9/tests-cpu-kernels/test_cpuawkward_ListArray64_getitem_jagged_apply_64.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# AUTO GENERATED ON 2023-02-03 AT 22:54:31
+# AUTO GENERATED ON 2023-02-16 AT 15:37:39
 # DO NOT EDIT BY HAND!
 #
 # To regenerate file, run
 #
 #     python dev/generate-tests.py
 #
```

### Comparing `awkward-cpp-8/tests-cpu-kernels/test_cpuawkward_ListArray64_getitem_jagged_descend_64.py` & `awkward-cpp-9/tests-cpu-kernels/test_cpuawkward_ListArray64_getitem_jagged_descend_64.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# AUTO GENERATED ON 2023-02-03 AT 22:54:31
+# AUTO GENERATED ON 2023-02-16 AT 15:37:39
 # DO NOT EDIT BY HAND!
 #
 # To regenerate file, run
 #
 #     python dev/generate-tests.py
 #
```

### Comparing `awkward-cpp-8/tests-cpu-kernels/test_cpuawkward_ListArray64_getitem_jagged_expand_64.py` & `awkward-cpp-9/tests-cpu-kernels/test_cpuawkward_ListArray64_getitem_jagged_expand_64.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# AUTO GENERATED ON 2023-02-03 AT 22:54:31
+# AUTO GENERATED ON 2023-02-16 AT 15:37:39
 # DO NOT EDIT BY HAND!
 #
 # To regenerate file, run
 #
 #     python dev/generate-tests.py
 #
```

### Comparing `awkward-cpp-8/tests-cpu-kernels/test_cpuawkward_ListArray64_getitem_next_array_64.py` & `awkward-cpp-9/tests-cpu-kernels/test_cpuawkward_ListArray64_getitem_next_array_64.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# AUTO GENERATED ON 2023-02-03 AT 22:54:31
+# AUTO GENERATED ON 2023-02-16 AT 15:37:39
 # DO NOT EDIT BY HAND!
 #
 # To regenerate file, run
 #
 #     python dev/generate-tests.py
 #
```

### Comparing `awkward-cpp-8/tests-cpu-kernels/test_cpuawkward_ListArray64_getitem_next_array_advanced_64.py` & `awkward-cpp-9/tests-cpu-kernels/test_cpuawkward_ListArray64_getitem_next_array_advanced_64.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# AUTO GENERATED ON 2023-02-03 AT 22:54:31
+# AUTO GENERATED ON 2023-02-16 AT 15:37:39
 # DO NOT EDIT BY HAND!
 #
 # To regenerate file, run
 #
 #     python dev/generate-tests.py
 #
```

### Comparing `awkward-cpp-8/tests-cpu-kernels/test_cpuawkward_ListArray64_getitem_next_at_64.py` & `awkward-cpp-9/tests-cpu-kernels/test_cpuawkward_ListArray64_getitem_next_at_64.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# AUTO GENERATED ON 2023-02-03 AT 22:54:31
+# AUTO GENERATED ON 2023-02-16 AT 15:37:39
 # DO NOT EDIT BY HAND!
 #
 # To regenerate file, run
 #
 #     python dev/generate-tests.py
 #
```

### Comparing `awkward-cpp-8/tests-cpu-kernels/test_cpuawkward_ListArray64_getitem_next_range_counts_64.py` & `awkward-cpp-9/tests-cpu-kernels/test_cpuawkward_ListArray64_getitem_next_range_counts_64.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# AUTO GENERATED ON 2023-02-03 AT 22:54:31
+# AUTO GENERATED ON 2023-02-16 AT 15:37:39
 # DO NOT EDIT BY HAND!
 #
 # To regenerate file, run
 #
 #     python dev/generate-tests.py
 #
```

### Comparing `awkward-cpp-8/tests-cpu-kernels/test_cpuawkward_ListArray64_localindex_64.py` & `awkward-cpp-9/tests-cpu-kernels/test_cpuawkward_ListArray64_localindex_64.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# AUTO GENERATED ON 2023-02-03 AT 22:54:31
+# AUTO GENERATED ON 2023-02-16 AT 15:37:39
 # DO NOT EDIT BY HAND!
 #
 # To regenerate file, run
 #
 #     python dev/generate-tests.py
 #
```

### Comparing `awkward-cpp-8/tests-cpu-kernels/test_cpuawkward_ListArray64_min_range.py` & `awkward-cpp-9/tests-cpu-kernels/test_cpuawkward_ListArray64_min_range.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# AUTO GENERATED ON 2023-02-03 AT 22:54:31
+# AUTO GENERATED ON 2023-02-16 AT 15:37:39
 # DO NOT EDIT BY HAND!
 #
 # To regenerate file, run
 #
 #     python dev/generate-tests.py
 #
```

### Comparing `awkward-cpp-8/tests-cpu-kernels/test_cpuawkward_ListArray64_rpad_and_clip_length_axis1.py` & `awkward-cpp-9/tests-cpu-kernels/test_cpuawkward_ListArray64_rpad_and_clip_length_axis1.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# AUTO GENERATED ON 2023-02-03 AT 22:54:31
+# AUTO GENERATED ON 2023-02-16 AT 15:37:39
 # DO NOT EDIT BY HAND!
 #
 # To regenerate file, run
 #
 #     python dev/generate-tests.py
 #
```

### Comparing `awkward-cpp-8/tests-cpu-kernels/test_cpuawkward_ListArray64_rpad_axis1_64.py` & `awkward-cpp-9/tests-cpu-kernels/test_cpuawkward_ListArray64_rpad_axis1_64.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# AUTO GENERATED ON 2023-02-03 AT 22:54:31
+# AUTO GENERATED ON 2023-02-16 AT 15:37:39
 # DO NOT EDIT BY HAND!
 #
 # To regenerate file, run
 #
 #     python dev/generate-tests.py
 #
```

### Comparing `awkward-cpp-8/tests-cpu-kernels/test_cpuawkward_ListArray64_validity.py` & `awkward-cpp-9/tests-cpu-kernels/test_cpuawkward_ListArray64_validity.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# AUTO GENERATED ON 2023-02-03 AT 22:54:31
+# AUTO GENERATED ON 2023-02-16 AT 15:37:39
 # DO NOT EDIT BY HAND!
 #
 # To regenerate file, run
 #
 #     python dev/generate-tests.py
 #
```

### Comparing `awkward-cpp-8/tests-cpu-kernels/test_cpuawkward_ListArrayU32_broadcast_tooffsets_64.py` & `awkward-cpp-9/tests-cpu-kernels/test_cpuawkward_ListArrayU32_broadcast_tooffsets_64.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# AUTO GENERATED ON 2023-02-03 AT 22:54:31
+# AUTO GENERATED ON 2023-02-16 AT 15:37:39
 # DO NOT EDIT BY HAND!
 #
 # To regenerate file, run
 #
 #     python dev/generate-tests.py
 #
```

### Comparing `awkward-cpp-8/tests-cpu-kernels/test_cpuawkward_ListArrayU32_combinations_length_64.py` & `awkward-cpp-9/tests-cpu-kernels/test_cpuawkward_ListArrayU32_combinations_length_64.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# AUTO GENERATED ON 2023-02-03 AT 22:54:31
+# AUTO GENERATED ON 2023-02-16 AT 15:37:39
 # DO NOT EDIT BY HAND!
 #
 # To regenerate file, run
 #
 #     python dev/generate-tests.py
 #
```

### Comparing `awkward-cpp-8/tests-cpu-kernels/test_cpuawkward_ListArrayU32_compact_offsets_64.py` & `awkward-cpp-9/tests-cpu-kernels/test_cpuawkward_ListArrayU32_compact_offsets_64.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# AUTO GENERATED ON 2023-02-03 AT 22:54:31
+# AUTO GENERATED ON 2023-02-16 AT 15:37:39
 # DO NOT EDIT BY HAND!
 #
 # To regenerate file, run
 #
 #     python dev/generate-tests.py
 #
```

### Comparing `awkward-cpp-8/tests-cpu-kernels/test_cpuawkward_ListArrayU32_getitem_jagged_apply_64.py` & `awkward-cpp-9/tests-cpu-kernels/test_cpuawkward_ListArrayU32_getitem_jagged_apply_64.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# AUTO GENERATED ON 2023-02-03 AT 22:54:31
+# AUTO GENERATED ON 2023-02-16 AT 15:37:39
 # DO NOT EDIT BY HAND!
 #
 # To regenerate file, run
 #
 #     python dev/generate-tests.py
 #
```

### Comparing `awkward-cpp-8/tests-cpu-kernels/test_cpuawkward_ListArrayU32_getitem_jagged_descend_64.py` & `awkward-cpp-9/tests-cpu-kernels/test_cpuawkward_ListArrayU32_getitem_jagged_descend_64.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# AUTO GENERATED ON 2023-02-03 AT 22:54:31
+# AUTO GENERATED ON 2023-02-16 AT 15:37:39
 # DO NOT EDIT BY HAND!
 #
 # To regenerate file, run
 #
 #     python dev/generate-tests.py
 #
```

### Comparing `awkward-cpp-8/tests-cpu-kernels/test_cpuawkward_ListArrayU32_getitem_jagged_expand_64.py` & `awkward-cpp-9/tests-cpu-kernels/test_cpuawkward_ListArrayU32_getitem_jagged_expand_64.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# AUTO GENERATED ON 2023-02-03 AT 22:54:31
+# AUTO GENERATED ON 2023-02-16 AT 15:37:39
 # DO NOT EDIT BY HAND!
 #
 # To regenerate file, run
 #
 #     python dev/generate-tests.py
 #
```

### Comparing `awkward-cpp-8/tests-cpu-kernels/test_cpuawkward_ListArrayU32_getitem_next_array_64.py` & `awkward-cpp-9/tests-cpu-kernels/test_cpuawkward_ListArrayU32_getitem_next_array_64.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# AUTO GENERATED ON 2023-02-03 AT 22:54:31
+# AUTO GENERATED ON 2023-02-16 AT 15:37:39
 # DO NOT EDIT BY HAND!
 #
 # To regenerate file, run
 #
 #     python dev/generate-tests.py
 #
```

### Comparing `awkward-cpp-8/tests-cpu-kernels/test_cpuawkward_ListArrayU32_getitem_next_array_advanced_64.py` & `awkward-cpp-9/tests-cpu-kernels/test_cpuawkward_ListArrayU32_getitem_next_array_advanced_64.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# AUTO GENERATED ON 2023-02-03 AT 22:54:31
+# AUTO GENERATED ON 2023-02-16 AT 15:37:39
 # DO NOT EDIT BY HAND!
 #
 # To regenerate file, run
 #
 #     python dev/generate-tests.py
 #
```

### Comparing `awkward-cpp-8/tests-cpu-kernels/test_cpuawkward_ListArrayU32_getitem_next_at_64.py` & `awkward-cpp-9/tests-cpu-kernels/test_cpuawkward_ListArrayU32_getitem_next_at_64.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# AUTO GENERATED ON 2023-02-03 AT 22:54:31
+# AUTO GENERATED ON 2023-02-16 AT 15:37:39
 # DO NOT EDIT BY HAND!
 #
 # To regenerate file, run
 #
 #     python dev/generate-tests.py
 #
```

### Comparing `awkward-cpp-8/tests-cpu-kernels/test_cpuawkward_ListArrayU32_getitem_next_range_counts_64.py` & `awkward-cpp-9/tests-cpu-kernels/test_cpuawkward_ListArrayU32_getitem_next_range_counts_64.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# AUTO GENERATED ON 2023-02-03 AT 22:54:31
+# AUTO GENERATED ON 2023-02-16 AT 15:37:39
 # DO NOT EDIT BY HAND!
 #
 # To regenerate file, run
 #
 #     python dev/generate-tests.py
 #
```

### Comparing `awkward-cpp-8/tests-cpu-kernels/test_cpuawkward_ListArrayU32_localindex_64.py` & `awkward-cpp-9/tests-cpu-kernels/test_cpuawkward_ListArrayU32_localindex_64.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# AUTO GENERATED ON 2023-02-03 AT 22:54:31
+# AUTO GENERATED ON 2023-02-16 AT 15:37:39
 # DO NOT EDIT BY HAND!
 #
 # To regenerate file, run
 #
 #     python dev/generate-tests.py
 #
```

### Comparing `awkward-cpp-8/tests-cpu-kernels/test_cpuawkward_ListArrayU32_min_range.py` & `awkward-cpp-9/tests-cpu-kernels/test_cpuawkward_ListArrayU32_min_range.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# AUTO GENERATED ON 2023-02-03 AT 22:54:31
+# AUTO GENERATED ON 2023-02-16 AT 15:37:39
 # DO NOT EDIT BY HAND!
 #
 # To regenerate file, run
 #
 #     python dev/generate-tests.py
 #
```

### Comparing `awkward-cpp-8/tests-cpu-kernels/test_cpuawkward_ListArrayU32_rpad_and_clip_length_axis1.py` & `awkward-cpp-9/tests-cpu-kernels/test_cpuawkward_ListArrayU32_rpad_and_clip_length_axis1.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# AUTO GENERATED ON 2023-02-03 AT 22:54:31
+# AUTO GENERATED ON 2023-02-16 AT 15:37:39
 # DO NOT EDIT BY HAND!
 #
 # To regenerate file, run
 #
 #     python dev/generate-tests.py
 #
```

### Comparing `awkward-cpp-8/tests-cpu-kernels/test_cpuawkward_ListArrayU32_rpad_axis1_64.py` & `awkward-cpp-9/tests-cpu-kernels/test_cpuawkward_ListArrayU32_rpad_axis1_64.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# AUTO GENERATED ON 2023-02-03 AT 22:54:31
+# AUTO GENERATED ON 2023-02-16 AT 15:37:39
 # DO NOT EDIT BY HAND!
 #
 # To regenerate file, run
 #
 #     python dev/generate-tests.py
 #
```

### Comparing `awkward-cpp-8/tests-cpu-kernels/test_cpuawkward_ListArrayU32_validity.py` & `awkward-cpp-9/tests-cpu-kernels/test_cpuawkward_ListArrayU32_validity.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# AUTO GENERATED ON 2023-02-03 AT 22:54:31
+# AUTO GENERATED ON 2023-02-16 AT 15:37:39
 # DO NOT EDIT BY HAND!
 #
 # To regenerate file, run
 #
 #     python dev/generate-tests.py
 #
```

### Comparing `awkward-cpp-8/tests-cpu-kernels/test_cpuawkward_ListArray_fill_to64_from32.py` & `awkward-cpp-9/tests-cpu-kernels/test_cpuawkward_ListArray_fill_to64_from32.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# AUTO GENERATED ON 2023-02-03 AT 22:54:31
+# AUTO GENERATED ON 2023-02-16 AT 15:37:39
 # DO NOT EDIT BY HAND!
 #
 # To regenerate file, run
 #
 #     python dev/generate-tests.py
 #
```

### Comparing `awkward-cpp-8/tests-cpu-kernels/test_cpuawkward_ListArray_fill_to64_from64.py` & `awkward-cpp-9/tests-cpu-kernels/test_cpuawkward_ListArray_fill_to64_from64.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# AUTO GENERATED ON 2023-02-03 AT 22:54:31
+# AUTO GENERATED ON 2023-02-16 AT 15:37:39
 # DO NOT EDIT BY HAND!
 #
 # To regenerate file, run
 #
 #     python dev/generate-tests.py
 #
```

### Comparing `awkward-cpp-8/tests-cpu-kernels/test_cpuawkward_ListArray_fill_to64_fromU32.py` & `awkward-cpp-9/tests-cpu-kernels/test_cpuawkward_ListArray_fill_to64_fromU32.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# AUTO GENERATED ON 2023-02-03 AT 22:54:31
+# AUTO GENERATED ON 2023-02-16 AT 15:37:39
 # DO NOT EDIT BY HAND!
 #
 # To regenerate file, run
 #
 #     python dev/generate-tests.py
 #
```

### Comparing `awkward-cpp-8/tests-cpu-kernels/test_cpuawkward_ListArray_getitem_jagged_carrylen_64.py` & `awkward-cpp-9/tests-cpu-kernels/test_cpuawkward_ListArray_getitem_jagged_carrylen_64.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# AUTO GENERATED ON 2023-02-03 AT 22:54:31
+# AUTO GENERATED ON 2023-02-16 AT 15:37:39
 # DO NOT EDIT BY HAND!
 #
 # To regenerate file, run
 #
 #     python dev/generate-tests.py
 #
```

### Comparing `awkward-cpp-8/tests-cpu-kernels/test_cpuawkward_ListArray_getitem_jagged_shrink_64.py` & `awkward-cpp-9/tests-cpu-kernels/test_cpuawkward_ListArray_getitem_jagged_shrink_64.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# AUTO GENERATED ON 2023-02-03 AT 22:54:31
+# AUTO GENERATED ON 2023-02-16 AT 15:37:39
 # DO NOT EDIT BY HAND!
 #
 # To regenerate file, run
 #
 #     python dev/generate-tests.py
 #
```

### Comparing `awkward-cpp-8/tests-cpu-kernels/test_cpuawkward_ListOffsetArray32_compact_offsets_64.py` & `awkward-cpp-9/tests-cpu-kernels/test_cpuawkward_ListOffsetArray32_compact_offsets_64.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# AUTO GENERATED ON 2023-02-03 AT 22:54:31
+# AUTO GENERATED ON 2023-02-16 AT 15:37:39
 # DO NOT EDIT BY HAND!
 #
 # To regenerate file, run
 #
 #     python dev/generate-tests.py
 #
```

### Comparing `awkward-cpp-8/tests-cpu-kernels/test_cpuawkward_ListOffsetArray32_flatten_offsets_64.py` & `awkward-cpp-9/tests-cpu-kernels/test_cpuawkward_ListOffsetArray32_flatten_offsets_64.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# AUTO GENERATED ON 2023-02-03 AT 22:54:31
+# AUTO GENERATED ON 2023-02-16 AT 15:37:39
 # DO NOT EDIT BY HAND!
 #
 # To regenerate file, run
 #
 #     python dev/generate-tests.py
 #
```

### Comparing `awkward-cpp-8/tests-cpu-kernels/test_cpuawkward_ListOffsetArray32_toRegularArray.py` & `awkward-cpp-9/tests-cpu-kernels/test_cpuawkward_ListOffsetArray32_toRegularArray.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# AUTO GENERATED ON 2023-02-03 AT 22:54:31
+# AUTO GENERATED ON 2023-02-16 AT 15:37:39
 # DO NOT EDIT BY HAND!
 #
 # To regenerate file, run
 #
 #     python dev/generate-tests.py
 #
```

### Comparing `awkward-cpp-8/tests-cpu-kernels/test_cpuawkward_ListOffsetArray64_compact_offsets_64.py` & `awkward-cpp-9/tests-cpu-kernels/test_cpuawkward_ListOffsetArray64_compact_offsets_64.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# AUTO GENERATED ON 2023-02-03 AT 22:54:31
+# AUTO GENERATED ON 2023-02-16 AT 15:37:39
 # DO NOT EDIT BY HAND!
 #
 # To regenerate file, run
 #
 #     python dev/generate-tests.py
 #
```

### Comparing `awkward-cpp-8/tests-cpu-kernels/test_cpuawkward_ListOffsetArray64_flatten_offsets_64.py` & `awkward-cpp-9/tests-cpu-kernels/test_cpuawkward_ListOffsetArray64_flatten_offsets_64.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# AUTO GENERATED ON 2023-02-03 AT 22:54:31
+# AUTO GENERATED ON 2023-02-16 AT 15:37:39
 # DO NOT EDIT BY HAND!
 #
 # To regenerate file, run
 #
 #     python dev/generate-tests.py
 #
```

### Comparing `awkward-cpp-8/tests-cpu-kernels/test_cpuawkward_ListOffsetArray64_toRegularArray.py` & `awkward-cpp-9/tests-cpu-kernels/test_cpuawkward_ListOffsetArray64_toRegularArray.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# AUTO GENERATED ON 2023-02-03 AT 22:54:31
+# AUTO GENERATED ON 2023-02-16 AT 15:37:39
 # DO NOT EDIT BY HAND!
 #
 # To regenerate file, run
 #
 #     python dev/generate-tests.py
 #
```

### Comparing `awkward-cpp-8/tests-cpu-kernels/test_cpuawkward_ListOffsetArrayU32_compact_offsets_64.py` & `awkward-cpp-9/tests-cpu-kernels/test_cpuawkward_ListOffsetArrayU32_compact_offsets_64.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# AUTO GENERATED ON 2023-02-03 AT 22:54:31
+# AUTO GENERATED ON 2023-02-16 AT 15:37:39
 # DO NOT EDIT BY HAND!
 #
 # To regenerate file, run
 #
 #     python dev/generate-tests.py
 #
```

### Comparing `awkward-cpp-8/tests-cpu-kernels/test_cpuawkward_ListOffsetArrayU32_flatten_offsets_64.py` & `awkward-cpp-9/tests-cpu-kernels/test_cpuawkward_ListOffsetArrayU32_flatten_offsets_64.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# AUTO GENERATED ON 2023-02-03 AT 22:54:31
+# AUTO GENERATED ON 2023-02-16 AT 15:37:39
 # DO NOT EDIT BY HAND!
 #
 # To regenerate file, run
 #
 #     python dev/generate-tests.py
 #
```

### Comparing `awkward-cpp-8/tests-cpu-kernels/test_cpuawkward_ListOffsetArrayU32_toRegularArray.py` & `awkward-cpp-9/tests-cpu-kernels/test_cpuawkward_ListOffsetArrayU32_toRegularArray.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# AUTO GENERATED ON 2023-02-03 AT 22:54:31
+# AUTO GENERATED ON 2023-02-16 AT 15:37:39
 # DO NOT EDIT BY HAND!
 #
 # To regenerate file, run
 #
 #     python dev/generate-tests.py
 #
```

### Comparing `awkward-cpp-8/tests-cpu-kernels/test_cpuawkward_ListOffsetArray_drop_none_indexes_32.py` & `awkward-cpp-9/tests-cpu-kernels/test_cpuawkward_ListOffsetArray_drop_none_indexes_32.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# AUTO GENERATED ON 2023-02-03 AT 22:54:31
+# AUTO GENERATED ON 2023-02-16 AT 15:37:39
 # DO NOT EDIT BY HAND!
 #
 # To regenerate file, run
 #
 #     python dev/generate-tests.py
 #
```

### Comparing `awkward-cpp-8/tests-cpu-kernels/test_cpuawkward_ListOffsetArray_drop_none_indexes_64.py` & `awkward-cpp-9/tests-cpu-kernels/test_cpuawkward_ListOffsetArray_drop_none_indexes_64.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# AUTO GENERATED ON 2023-02-03 AT 22:54:31
+# AUTO GENERATED ON 2023-02-16 AT 15:37:39
 # DO NOT EDIT BY HAND!
 #
 # To regenerate file, run
 #
 #     python dev/generate-tests.py
 #
```

### Comparing `awkward-cpp-8/tests-cpu-kernels/test_cpuawkward_MaskedArray32_getitem_next_jagged_project.py` & `awkward-cpp-9/tests-cpu-kernels/test_cpuawkward_MaskedArray32_getitem_next_jagged_project.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# AUTO GENERATED ON 2023-02-03 AT 22:54:31
+# AUTO GENERATED ON 2023-02-16 AT 15:37:39
 # DO NOT EDIT BY HAND!
 #
 # To regenerate file, run
 #
 #     python dev/generate-tests.py
 #
```

### Comparing `awkward-cpp-8/tests-cpu-kernels/test_cpuawkward_MaskedArray64_getitem_next_jagged_project.py` & `awkward-cpp-9/tests-cpu-kernels/test_cpuawkward_MaskedArray64_getitem_next_jagged_project.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# AUTO GENERATED ON 2023-02-03 AT 22:54:31
+# AUTO GENERATED ON 2023-02-16 AT 15:37:39
 # DO NOT EDIT BY HAND!
 #
 # To regenerate file, run
 #
 #     python dev/generate-tests.py
 #
```

### Comparing `awkward-cpp-8/tests-cpu-kernels/test_cpuawkward_MaskedArrayU32_getitem_next_jagged_project.py` & `awkward-cpp-9/tests-cpu-kernels/test_cpuawkward_MaskedArrayU32_getitem_next_jagged_project.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# AUTO GENERATED ON 2023-02-03 AT 22:54:31
+# AUTO GENERATED ON 2023-02-16 AT 15:37:39
 # DO NOT EDIT BY HAND!
 #
 # To regenerate file, run
 #
 #     python dev/generate-tests.py
 #
```

### Comparing `awkward-cpp-8/tests-cpu-kernels/test_cpuawkward_RegularArray_broadcast_tooffsets_64.py` & `awkward-cpp-9/tests-cpu-kernels/test_cpuawkward_RegularArray_broadcast_tooffsets_64.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# AUTO GENERATED ON 2023-02-03 AT 22:54:31
+# AUTO GENERATED ON 2023-02-16 AT 15:37:39
 # DO NOT EDIT BY HAND!
 #
 # To regenerate file, run
 #
 #     python dev/generate-tests.py
 #
```

### Comparing `awkward-cpp-8/tests-cpu-kernels/test_cpuawkward_RegularArray_broadcast_tooffsets_size1_64.py` & `awkward-cpp-9/tests-cpu-kernels/test_cpuawkward_RegularArray_broadcast_tooffsets_size1_64.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# AUTO GENERATED ON 2023-02-03 AT 22:54:31
+# AUTO GENERATED ON 2023-02-16 AT 15:37:39
 # DO NOT EDIT BY HAND!
 #
 # To regenerate file, run
 #
 #     python dev/generate-tests.py
 #
```

### Comparing `awkward-cpp-8/tests-cpu-kernels/test_cpuawkward_RegularArray_compact_offsets64.py` & `awkward-cpp-9/tests-cpu-kernels/test_cpuawkward_RegularArray_compact_offsets64.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# AUTO GENERATED ON 2023-02-03 AT 22:54:31
+# AUTO GENERATED ON 2023-02-16 AT 15:37:39
 # DO NOT EDIT BY HAND!
 #
 # To regenerate file, run
 #
 #     python dev/generate-tests.py
 #
```

### Comparing `awkward-cpp-8/tests-cpu-kernels/test_cpuawkward_RegularArray_getitem_carry_64.py` & `awkward-cpp-9/tests-cpu-kernels/test_cpuawkward_RegularArray_getitem_carry_64.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# AUTO GENERATED ON 2023-02-03 AT 22:54:31
+# AUTO GENERATED ON 2023-02-16 AT 15:37:39
 # DO NOT EDIT BY HAND!
 #
 # To regenerate file, run
 #
 #     python dev/generate-tests.py
 #
```

### Comparing `awkward-cpp-8/tests-cpu-kernels/test_cpuawkward_RegularArray_getitem_jagged_expand_64.py` & `awkward-cpp-9/tests-cpu-kernels/test_cpuawkward_RegularArray_getitem_jagged_expand_64.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# AUTO GENERATED ON 2023-02-03 AT 22:54:31
+# AUTO GENERATED ON 2023-02-16 AT 15:37:39
 # DO NOT EDIT BY HAND!
 #
 # To regenerate file, run
 #
 #     python dev/generate-tests.py
 #
```

### Comparing `awkward-cpp-8/tests-cpu-kernels/test_cpuawkward_RegularArray_getitem_next_array_64.py` & `awkward-cpp-9/tests-cpu-kernels/test_cpuawkward_RegularArray_getitem_next_array_64.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# AUTO GENERATED ON 2023-02-03 AT 22:54:31
+# AUTO GENERATED ON 2023-02-16 AT 15:37:39
 # DO NOT EDIT BY HAND!
 #
 # To regenerate file, run
 #
 #     python dev/generate-tests.py
 #
```

### Comparing `awkward-cpp-8/tests-cpu-kernels/test_cpuawkward_RegularArray_getitem_next_array_advanced_64.py` & `awkward-cpp-9/tests-cpu-kernels/test_cpuawkward_RegularArray_getitem_next_array_advanced_64.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# AUTO GENERATED ON 2023-02-03 AT 22:54:31
+# AUTO GENERATED ON 2023-02-16 AT 15:37:39
 # DO NOT EDIT BY HAND!
 #
 # To regenerate file, run
 #
 #     python dev/generate-tests.py
 #
```

### Comparing `awkward-cpp-8/tests-cpu-kernels/test_cpuawkward_RegularArray_getitem_next_array_regularize_64.py` & `awkward-cpp-9/tests-cpu-kernels/test_cpuawkward_RegularArray_getitem_next_array_regularize_64.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# AUTO GENERATED ON 2023-02-03 AT 22:54:31
+# AUTO GENERATED ON 2023-02-16 AT 15:37:39
 # DO NOT EDIT BY HAND!
 #
 # To regenerate file, run
 #
 #     python dev/generate-tests.py
 #
```

### Comparing `awkward-cpp-8/tests-cpu-kernels/test_cpuawkward_RegularArray_getitem_next_at_64.py` & `awkward-cpp-9/tests-cpu-kernels/test_cpuawkward_RegularArray_getitem_next_at_64.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# AUTO GENERATED ON 2023-02-03 AT 22:54:31
+# AUTO GENERATED ON 2023-02-16 AT 15:37:39
 # DO NOT EDIT BY HAND!
 #
 # To regenerate file, run
 #
 #     python dev/generate-tests.py
 #
```

### Comparing `awkward-cpp-8/tests-cpu-kernels/test_cpuawkward_RegularArray_getitem_next_range_64.py` & `awkward-cpp-9/tests-cpu-kernels/test_cpuawkward_RegularArray_getitem_next_range_64.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# AUTO GENERATED ON 2023-02-03 AT 22:54:31
+# AUTO GENERATED ON 2023-02-16 AT 15:37:39
 # DO NOT EDIT BY HAND!
 #
 # To regenerate file, run
 #
 #     python dev/generate-tests.py
 #
```

### Comparing `awkward-cpp-8/tests-cpu-kernels/test_cpuawkward_RegularArray_getitem_next_range_spreadadvanced_64.py` & `awkward-cpp-9/tests-cpu-kernels/test_cpuawkward_RegularArray_getitem_next_range_spreadadvanced_64.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# AUTO GENERATED ON 2023-02-03 AT 22:54:31
+# AUTO GENERATED ON 2023-02-16 AT 15:37:39
 # DO NOT EDIT BY HAND!
 #
 # To regenerate file, run
 #
 #     python dev/generate-tests.py
 #
```

### Comparing `awkward-cpp-8/tests-cpu-kernels/test_cpuawkward_RegularArray_localindex_64.py` & `awkward-cpp-9/tests-cpu-kernels/test_cpuawkward_RegularArray_localindex_64.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# AUTO GENERATED ON 2023-02-03 AT 22:54:31
+# AUTO GENERATED ON 2023-02-16 AT 15:37:39
 # DO NOT EDIT BY HAND!
 #
 # To regenerate file, run
 #
 #     python dev/generate-tests.py
 #
```

### Comparing `awkward-cpp-8/tests-cpu-kernels/test_cpuawkward_RegularArray_rpad_and_clip_axis1_64.py` & `awkward-cpp-9/tests-cpu-kernels/test_cpuawkward_RegularArray_rpad_and_clip_axis1_64.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# AUTO GENERATED ON 2023-02-03 AT 22:54:31
+# AUTO GENERATED ON 2023-02-16 AT 15:37:39
 # DO NOT EDIT BY HAND!
 #
 # To regenerate file, run
 #
 #     python dev/generate-tests.py
 #
```

### Comparing `awkward-cpp-8/tests-cpu-kernels/test_cpuawkward_UnionArray8_32_project_64.py` & `awkward-cpp-9/tests-cpu-kernels/test_cpuawkward_UnionArray8_32_project_64.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# AUTO GENERATED ON 2023-02-03 AT 22:54:31
+# AUTO GENERATED ON 2023-02-16 AT 15:37:39
 # DO NOT EDIT BY HAND!
 #
 # To regenerate file, run
 #
 #     python dev/generate-tests.py
 #
```

### Comparing `awkward-cpp-8/tests-cpu-kernels/test_cpuawkward_UnionArray8_32_regular_index.py` & `awkward-cpp-9/tests-cpu-kernels/test_cpuawkward_UnionArray8_32_regular_index.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# AUTO GENERATED ON 2023-02-03 AT 22:54:31
+# AUTO GENERATED ON 2023-02-16 AT 15:37:39
 # DO NOT EDIT BY HAND!
 #
 # To regenerate file, run
 #
 #     python dev/generate-tests.py
 #
```

### Comparing `awkward-cpp-8/tests-cpu-kernels/test_cpuawkward_UnionArray8_32_simplify8_32_to8_64.py` & `awkward-cpp-9/tests-cpu-kernels/test_cpuawkward_UnionArray8_32_simplify8_32_to8_64.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# AUTO GENERATED ON 2023-02-03 AT 22:54:31
+# AUTO GENERATED ON 2023-02-16 AT 15:37:39
 # DO NOT EDIT BY HAND!
 #
 # To regenerate file, run
 #
 #     python dev/generate-tests.py
 #
```

### Comparing `awkward-cpp-8/tests-cpu-kernels/test_cpuawkward_UnionArray8_32_simplify8_64_to8_64.py` & `awkward-cpp-9/tests-cpu-kernels/test_cpuawkward_UnionArray8_32_simplify8_64_to8_64.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# AUTO GENERATED ON 2023-02-03 AT 22:54:31
+# AUTO GENERATED ON 2023-02-16 AT 15:37:39
 # DO NOT EDIT BY HAND!
 #
 # To regenerate file, run
 #
 #     python dev/generate-tests.py
 #
```

### Comparing `awkward-cpp-8/tests-cpu-kernels/test_cpuawkward_UnionArray8_32_simplify8_U32_to8_64.py` & `awkward-cpp-9/tests-cpu-kernels/test_cpuawkward_UnionArray8_32_simplify8_U32_to8_64.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# AUTO GENERATED ON 2023-02-03 AT 22:54:31
+# AUTO GENERATED ON 2023-02-16 AT 15:37:39
 # DO NOT EDIT BY HAND!
 #
 # To regenerate file, run
 #
 #     python dev/generate-tests.py
 #
```

### Comparing `awkward-cpp-8/tests-cpu-kernels/test_cpuawkward_UnionArray8_32_simplify_one_to8_64.py` & `awkward-cpp-9/tests-cpu-kernels/test_cpuawkward_UnionArray8_32_simplify_one_to8_64.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# AUTO GENERATED ON 2023-02-03 AT 22:54:31
+# AUTO GENERATED ON 2023-02-16 AT 15:37:39
 # DO NOT EDIT BY HAND!
 #
 # To regenerate file, run
 #
 #     python dev/generate-tests.py
 #
```

### Comparing `awkward-cpp-8/tests-cpu-kernels/test_cpuawkward_UnionArray8_32_validity.py` & `awkward-cpp-9/tests-cpu-kernels/test_cpuawkward_UnionArray8_32_validity.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# AUTO GENERATED ON 2023-02-03 AT 22:54:31
+# AUTO GENERATED ON 2023-02-16 AT 15:37:39
 # DO NOT EDIT BY HAND!
 #
 # To regenerate file, run
 #
 #     python dev/generate-tests.py
 #
```

### Comparing `awkward-cpp-8/tests-cpu-kernels/test_cpuawkward_UnionArray8_64_project_64.py` & `awkward-cpp-9/tests-cpu-kernels/test_cpuawkward_UnionArray8_64_project_64.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# AUTO GENERATED ON 2023-02-03 AT 22:54:31
+# AUTO GENERATED ON 2023-02-16 AT 15:37:39
 # DO NOT EDIT BY HAND!
 #
 # To regenerate file, run
 #
 #     python dev/generate-tests.py
 #
```

### Comparing `awkward-cpp-8/tests-cpu-kernels/test_cpuawkward_UnionArray8_64_regular_index.py` & `awkward-cpp-9/tests-cpu-kernels/test_cpuawkward_UnionArray8_64_regular_index.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# AUTO GENERATED ON 2023-02-03 AT 22:54:31
+# AUTO GENERATED ON 2023-02-16 AT 15:37:39
 # DO NOT EDIT BY HAND!
 #
 # To regenerate file, run
 #
 #     python dev/generate-tests.py
 #
```

### Comparing `awkward-cpp-8/tests-cpu-kernels/test_cpuawkward_UnionArray8_64_simplify8_32_to8_64.py` & `awkward-cpp-9/tests-cpu-kernels/test_cpuawkward_UnionArray8_64_simplify8_32_to8_64.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# AUTO GENERATED ON 2023-02-03 AT 22:54:31
+# AUTO GENERATED ON 2023-02-16 AT 15:37:39
 # DO NOT EDIT BY HAND!
 #
 # To regenerate file, run
 #
 #     python dev/generate-tests.py
 #
```

### Comparing `awkward-cpp-8/tests-cpu-kernels/test_cpuawkward_UnionArray8_64_simplify8_64_to8_64.py` & `awkward-cpp-9/tests-cpu-kernels/test_cpuawkward_UnionArray8_64_simplify8_64_to8_64.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# AUTO GENERATED ON 2023-02-03 AT 22:54:31
+# AUTO GENERATED ON 2023-02-16 AT 15:37:39
 # DO NOT EDIT BY HAND!
 #
 # To regenerate file, run
 #
 #     python dev/generate-tests.py
 #
```

### Comparing `awkward-cpp-8/tests-cpu-kernels/test_cpuawkward_UnionArray8_64_simplify8_U32_to8_64.py` & `awkward-cpp-9/tests-cpu-kernels/test_cpuawkward_UnionArray8_64_simplify8_U32_to8_64.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# AUTO GENERATED ON 2023-02-03 AT 22:54:31
+# AUTO GENERATED ON 2023-02-16 AT 15:37:39
 # DO NOT EDIT BY HAND!
 #
 # To regenerate file, run
 #
 #     python dev/generate-tests.py
 #
```

### Comparing `awkward-cpp-8/tests-cpu-kernels/test_cpuawkward_UnionArray8_64_simplify_one_to8_64.py` & `awkward-cpp-9/tests-cpu-kernels/test_cpuawkward_UnionArray8_64_simplify_one_to8_64.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# AUTO GENERATED ON 2023-02-03 AT 22:54:31
+# AUTO GENERATED ON 2023-02-16 AT 15:37:39
 # DO NOT EDIT BY HAND!
 #
 # To regenerate file, run
 #
 #     python dev/generate-tests.py
 #
```

### Comparing `awkward-cpp-8/tests-cpu-kernels/test_cpuawkward_UnionArray8_64_validity.py` & `awkward-cpp-9/tests-cpu-kernels/test_cpuawkward_UnionArray8_64_validity.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# AUTO GENERATED ON 2023-02-03 AT 22:54:31
+# AUTO GENERATED ON 2023-02-16 AT 15:37:39
 # DO NOT EDIT BY HAND!
 #
 # To regenerate file, run
 #
 #     python dev/generate-tests.py
 #
```

### Comparing `awkward-cpp-8/tests-cpu-kernels/test_cpuawkward_UnionArray8_U32_project_64.py` & `awkward-cpp-9/tests-cpu-kernels/test_cpuawkward_UnionArray8_U32_project_64.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# AUTO GENERATED ON 2023-02-03 AT 22:54:31
+# AUTO GENERATED ON 2023-02-16 AT 15:37:39
 # DO NOT EDIT BY HAND!
 #
 # To regenerate file, run
 #
 #     python dev/generate-tests.py
 #
```

### Comparing `awkward-cpp-8/tests-cpu-kernels/test_cpuawkward_UnionArray8_U32_regular_index.py` & `awkward-cpp-9/tests-cpu-kernels/test_cpuawkward_UnionArray8_U32_regular_index.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# AUTO GENERATED ON 2023-02-03 AT 22:54:31
+# AUTO GENERATED ON 2023-02-16 AT 15:37:39
 # DO NOT EDIT BY HAND!
 #
 # To regenerate file, run
 #
 #     python dev/generate-tests.py
 #
```

### Comparing `awkward-cpp-8/tests-cpu-kernels/test_cpuawkward_UnionArray8_U32_simplify8_32_to8_64.py` & `awkward-cpp-9/tests-cpu-kernels/test_cpuawkward_UnionArray8_U32_simplify8_32_to8_64.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# AUTO GENERATED ON 2023-02-03 AT 22:54:31
+# AUTO GENERATED ON 2023-02-16 AT 15:37:39
 # DO NOT EDIT BY HAND!
 #
 # To regenerate file, run
 #
 #     python dev/generate-tests.py
 #
```

### Comparing `awkward-cpp-8/tests-cpu-kernels/test_cpuawkward_UnionArray8_U32_simplify8_64_to8_64.py` & `awkward-cpp-9/tests-cpu-kernels/test_cpuawkward_UnionArray8_U32_simplify8_64_to8_64.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# AUTO GENERATED ON 2023-02-03 AT 22:54:31
+# AUTO GENERATED ON 2023-02-16 AT 15:37:39
 # DO NOT EDIT BY HAND!
 #
 # To regenerate file, run
 #
 #     python dev/generate-tests.py
 #
```

### Comparing `awkward-cpp-8/tests-cpu-kernels/test_cpuawkward_UnionArray8_U32_simplify8_U32_to8_64.py` & `awkward-cpp-9/tests-cpu-kernels/test_cpuawkward_UnionArray8_U32_simplify8_U32_to8_64.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# AUTO GENERATED ON 2023-02-03 AT 22:54:31
+# AUTO GENERATED ON 2023-02-16 AT 15:37:39
 # DO NOT EDIT BY HAND!
 #
 # To regenerate file, run
 #
 #     python dev/generate-tests.py
 #
```

### Comparing `awkward-cpp-8/tests-cpu-kernels/test_cpuawkward_UnionArray8_U32_simplify_one_to8_64.py` & `awkward-cpp-9/tests-cpu-kernels/test_cpuawkward_UnionArray8_U32_simplify_one_to8_64.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# AUTO GENERATED ON 2023-02-03 AT 22:54:31
+# AUTO GENERATED ON 2023-02-16 AT 15:37:39
 # DO NOT EDIT BY HAND!
 #
 # To regenerate file, run
 #
 #     python dev/generate-tests.py
 #
```

### Comparing `awkward-cpp-8/tests-cpu-kernels/test_cpuawkward_UnionArray8_U32_validity.py` & `awkward-cpp-9/tests-cpu-kernels/test_cpuawkward_UnionArray8_U32_validity.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# AUTO GENERATED ON 2023-02-03 AT 22:54:31
+# AUTO GENERATED ON 2023-02-16 AT 15:37:39
 # DO NOT EDIT BY HAND!
 #
 # To regenerate file, run
 #
 #     python dev/generate-tests.py
 #
```

### Comparing `awkward-cpp-8/tests-cpu-kernels/test_cpuawkward_UnionArray8_regular_index_getsize.py` & `awkward-cpp-9/tests-cpu-kernels/test_cpuawkward_UnionArray8_regular_index_getsize.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# AUTO GENERATED ON 2023-02-03 AT 22:54:31
+# AUTO GENERATED ON 2023-02-16 AT 15:37:39
 # DO NOT EDIT BY HAND!
 #
 # To regenerate file, run
 #
 #     python dev/generate-tests.py
 #
```

### Comparing `awkward-cpp-8/tests-cpu-kernels/test_cpuawkward_UnionArray_fillindex_to64_count.py` & `awkward-cpp-9/tests-cpu-kernels/test_cpuawkward_UnionArray_fillindex_to64_count.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# AUTO GENERATED ON 2023-02-03 AT 22:54:31
+# AUTO GENERATED ON 2023-02-16 AT 15:37:39
 # DO NOT EDIT BY HAND!
 #
 # To regenerate file, run
 #
 #     python dev/generate-tests.py
 #
```

### Comparing `awkward-cpp-8/tests-cpu-kernels/test_cpuawkward_UnionArray_fillindex_to64_from32.py` & `awkward-cpp-9/tests-cpu-kernels/test_cpuawkward_UnionArray_fillindex_to64_from32.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# AUTO GENERATED ON 2023-02-03 AT 22:54:31
+# AUTO GENERATED ON 2023-02-16 AT 15:37:39
 # DO NOT EDIT BY HAND!
 #
 # To regenerate file, run
 #
 #     python dev/generate-tests.py
 #
```

### Comparing `awkward-cpp-8/tests-cpu-kernels/test_cpuawkward_UnionArray_fillindex_to64_from64.py` & `awkward-cpp-9/tests-cpu-kernels/test_cpuawkward_UnionArray_fillindex_to64_from64.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# AUTO GENERATED ON 2023-02-03 AT 22:54:31
+# AUTO GENERATED ON 2023-02-16 AT 15:37:39
 # DO NOT EDIT BY HAND!
 #
 # To regenerate file, run
 #
 #     python dev/generate-tests.py
 #
```

### Comparing `awkward-cpp-8/tests-cpu-kernels/test_cpuawkward_UnionArray_fillindex_to64_fromU32.py` & `awkward-cpp-9/tests-cpu-kernels/test_cpuawkward_UnionArray_fillindex_to64_fromU32.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# AUTO GENERATED ON 2023-02-03 AT 22:54:31
+# AUTO GENERATED ON 2023-02-16 AT 15:37:39
 # DO NOT EDIT BY HAND!
 #
 # To regenerate file, run
 #
 #     python dev/generate-tests.py
 #
```

### Comparing `awkward-cpp-8/tests-cpu-kernels/test_cpuawkward_UnionArray_fillna_from32_to64.py` & `awkward-cpp-9/tests-cpu-kernels/test_cpuawkward_UnionArray_fillna_from32_to64.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# AUTO GENERATED ON 2023-02-03 AT 22:54:31
+# AUTO GENERATED ON 2023-02-16 AT 15:37:39
 # DO NOT EDIT BY HAND!
 #
 # To regenerate file, run
 #
 #     python dev/generate-tests.py
 #
```

### Comparing `awkward-cpp-8/tests-cpu-kernels/test_cpuawkward_UnionArray_fillna_from64_to64.py` & `awkward-cpp-9/tests-cpu-kernels/test_cpuawkward_UnionArray_fillna_from64_to64.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# AUTO GENERATED ON 2023-02-03 AT 22:54:31
+# AUTO GENERATED ON 2023-02-16 AT 15:37:39
 # DO NOT EDIT BY HAND!
 #
 # To regenerate file, run
 #
 #     python dev/generate-tests.py
 #
```

### Comparing `awkward-cpp-8/tests-cpu-kernels/test_cpuawkward_UnionArray_fillna_fromU32_to64.py` & `awkward-cpp-9/tests-cpu-kernels/test_cpuawkward_UnionArray_fillna_fromU32_to64.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# AUTO GENERATED ON 2023-02-03 AT 22:54:31
+# AUTO GENERATED ON 2023-02-16 AT 15:37:39
 # DO NOT EDIT BY HAND!
 #
 # To regenerate file, run
 #
 #     python dev/generate-tests.py
 #
```

### Comparing `awkward-cpp-8/tests-cpu-kernels/test_cpuawkward_UnionArray_filltags_to8_const.py` & `awkward-cpp-9/tests-cpu-kernels/test_cpuawkward_UnionArray_filltags_to8_const.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# AUTO GENERATED ON 2023-02-03 AT 22:54:31
+# AUTO GENERATED ON 2023-02-16 AT 15:37:39
 # DO NOT EDIT BY HAND!
 #
 # To regenerate file, run
 #
 #     python dev/generate-tests.py
 #
```

### Comparing `awkward-cpp-8/tests-cpu-kernels/test_cpuawkward_UnionArray_filltags_to8_from8.py` & `awkward-cpp-9/tests-cpu-kernels/test_cpuawkward_UnionArray_filltags_to8_from8.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# AUTO GENERATED ON 2023-02-03 AT 22:54:31
+# AUTO GENERATED ON 2023-02-16 AT 15:37:39
 # DO NOT EDIT BY HAND!
 #
 # To regenerate file, run
 #
 #     python dev/generate-tests.py
 #
```

### Comparing `awkward-cpp-8/tests-cpu-kernels/test_cpuawkward_index_rpad_and_clip_axis0_64.py` & `awkward-cpp-9/tests-cpu-kernels/test_cpuawkward_index_rpad_and_clip_axis0_64.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# AUTO GENERATED ON 2023-02-03 AT 22:54:31
+# AUTO GENERATED ON 2023-02-16 AT 15:37:39
 # DO NOT EDIT BY HAND!
 #
 # To regenerate file, run
 #
 #     python dev/generate-tests.py
 #
```

### Comparing `awkward-cpp-8/tests-cpu-kernels/test_cpuawkward_index_rpad_and_clip_axis1_64.py` & `awkward-cpp-9/tests-cpu-kernels/test_cpuawkward_index_rpad_and_clip_axis1_64.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# AUTO GENERATED ON 2023-02-03 AT 22:54:31
+# AUTO GENERATED ON 2023-02-16 AT 15:37:39
 # DO NOT EDIT BY HAND!
 #
 # To regenerate file, run
 #
 #     python dev/generate-tests.py
 #
```

### Comparing `awkward-cpp-8/tests-cpu-kernels/test_cpuawkward_localindex_64.py` & `awkward-cpp-9/tests-cpu-kernels/test_cpuawkward_localindex_64.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# AUTO GENERATED ON 2023-02-03 AT 22:54:31
+# AUTO GENERATED ON 2023-02-16 AT 15:37:39
 # DO NOT EDIT BY HAND!
 #
 # To regenerate file, run
 #
 #     python dev/generate-tests.py
 #
```

### Comparing `awkward-cpp-8/tests-cpu-kernels/test_cpuawkward_missing_repeat_64.py` & `awkward-cpp-9/tests-cpu-kernels/test_cpuawkward_missing_repeat_64.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# AUTO GENERATED ON 2023-02-03 AT 22:54:31
+# AUTO GENERATED ON 2023-02-16 AT 15:37:39
 # DO NOT EDIT BY HAND!
 #
 # To regenerate file, run
 #
 #     python dev/generate-tests.py
 #
```

### Comparing `awkward-cpp-8/tests-spec/kernels.py` & `awkward-cpp-9/tests-spec/kernels.py`

 * *Files 1% similar despite different names*

```diff
@@ -245,30 +245,14 @@
             mask_out[i] = i
             k = k + 1
             stops_out[i] = offsets_in[k]
 
 awkward_Content_getitem_next_missing_jagged_getmaskstartstop = awkward_Content_getitem_next_missing_jagged_getmaskstartstop
 
 
-def awkward_Index_iscontiguous(result, fromindex, length):
-    result[0] = True
-    expecting = 0
-    for i in range(length):
-        if fromindex[i] != expecting:
-            result[0] = False
-            return
-        expecting += 1
-
-awkward_Index32_iscontiguous = awkward_Index_iscontiguous
-awkward_Index64_iscontiguous = awkward_Index_iscontiguous
-awkward_Index8_iscontiguous = awkward_Index_iscontiguous
-awkward_IndexU32_iscontiguous = awkward_Index_iscontiguous
-awkward_IndexU8_iscontiguous = awkward_Index_iscontiguous
-
-
 def awkward_IndexedArray_fill(toindex, toindexoffset, fromindex, length, base):
     for i in range(length):
         fromval = fromindex[i]
         toindex[toindexoffset + i] = -1 if fromval < 0 else float(fromval + base)
 
 awkward_IndexedArray_fill_to64_from32 = awkward_IndexedArray_fill
 awkward_IndexedArray_fill_to64_from64 = awkward_IndexedArray_fill
```

### Comparing `awkward-cpp-8/tests-spec/test_pyawkward_BitMaskedArray_to_ByteMaskedArray.py` & `awkward-cpp-9/tests-spec/test_pyawkward_BitMaskedArray_to_ByteMaskedArray.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# AUTO GENERATED ON 2023-02-03 AT 22:54:31
+# AUTO GENERATED ON 2023-02-16 AT 15:37:39
 # DO NOT EDIT BY HAND!
 #
 # To regenerate file, run
 #
 #     python dev/generate-tests.py
 #
```

### Comparing `awkward-cpp-8/tests-spec/test_pyawkward_BitMaskedArray_to_IndexedOptionArray64.py` & `awkward-cpp-9/tests-spec/test_pyawkward_BitMaskedArray_to_IndexedOptionArray64.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# AUTO GENERATED ON 2023-02-03 AT 22:54:31
+# AUTO GENERATED ON 2023-02-16 AT 15:37:39
 # DO NOT EDIT BY HAND!
 #
 # To regenerate file, run
 #
 #     python dev/generate-tests.py
 #
```

### Comparing `awkward-cpp-8/tests-spec/test_pyawkward_ByteMaskedArray_getitem_nextcarry_64.py` & `awkward-cpp-9/tests-spec/test_pyawkward_ByteMaskedArray_getitem_nextcarry_64.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# AUTO GENERATED ON 2023-02-03 AT 22:54:31
+# AUTO GENERATED ON 2023-02-16 AT 15:37:39
 # DO NOT EDIT BY HAND!
 #
 # To regenerate file, run
 #
 #     python dev/generate-tests.py
 #
```

### Comparing `awkward-cpp-8/tests-spec/test_pyawkward_ByteMaskedArray_getitem_nextcarry_outindex_64.py` & `awkward-cpp-9/tests-spec/test_pyawkward_ByteMaskedArray_getitem_nextcarry_outindex_64.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# AUTO GENERATED ON 2023-02-03 AT 22:54:31
+# AUTO GENERATED ON 2023-02-16 AT 15:37:39
 # DO NOT EDIT BY HAND!
 #
 # To regenerate file, run
 #
 #     python dev/generate-tests.py
 #
```

### Comparing `awkward-cpp-8/tests-spec/test_pyawkward_ByteMaskedArray_numnull.py` & `awkward-cpp-9/tests-spec/test_pyawkward_ByteMaskedArray_numnull.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# AUTO GENERATED ON 2023-02-03 AT 22:54:31
+# AUTO GENERATED ON 2023-02-16 AT 15:37:39
 # DO NOT EDIT BY HAND!
 #
 # To regenerate file, run
 #
 #     python dev/generate-tests.py
 #
```

### Comparing `awkward-cpp-8/tests-spec/test_pyawkward_ByteMaskedArray_overlay_mask8.py` & `awkward-cpp-9/tests-spec/test_pyawkward_ByteMaskedArray_overlay_mask8.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# AUTO GENERATED ON 2023-02-03 AT 22:54:31
+# AUTO GENERATED ON 2023-02-16 AT 15:37:39
 # DO NOT EDIT BY HAND!
 #
 # To regenerate file, run
 #
 #     python dev/generate-tests.py
 #
```

### Comparing `awkward-cpp-8/tests-spec/test_pyawkward_ByteMaskedArray_toIndexedOptionArray64.py` & `awkward-cpp-9/tests-spec/test_pyawkward_ByteMaskedArray_toIndexedOptionArray64.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# AUTO GENERATED ON 2023-02-03 AT 22:54:31
+# AUTO GENERATED ON 2023-02-16 AT 15:37:39
 # DO NOT EDIT BY HAND!
 #
 # To regenerate file, run
 #
 #     python dev/generate-tests.py
 #
```

### Comparing `awkward-cpp-8/tests-spec/test_pyawkward_Content_getitem_next_missing_jagged_getmaskstartstop.py` & `awkward-cpp-9/tests-spec/test_pyawkward_Content_getitem_next_missing_jagged_getmaskstartstop.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# AUTO GENERATED ON 2023-02-03 AT 22:54:31
+# AUTO GENERATED ON 2023-02-16 AT 15:37:39
 # DO NOT EDIT BY HAND!
 #
 # To regenerate file, run
 #
 #     python dev/generate-tests.py
 #
```

### Comparing `awkward-cpp-8/tests-spec/test_pyawkward_IndexedArray32_flatten_nextcarry_64.py` & `awkward-cpp-9/tests-spec/test_pyawkward_IndexedArray32_flatten_nextcarry_64.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# AUTO GENERATED ON 2023-02-03 AT 22:54:31
+# AUTO GENERATED ON 2023-02-16 AT 15:37:39
 # DO NOT EDIT BY HAND!
 #
 # To regenerate file, run
 #
 #     python dev/generate-tests.py
 #
```

### Comparing `awkward-cpp-8/tests-spec/test_pyawkward_IndexedArray32_flatten_none2empty_64.py` & `awkward-cpp-9/tests-spec/test_pyawkward_IndexedArray32_flatten_none2empty_64.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# AUTO GENERATED ON 2023-02-03 AT 22:54:31
+# AUTO GENERATED ON 2023-02-16 AT 15:37:39
 # DO NOT EDIT BY HAND!
 #
 # To regenerate file, run
 #
 #     python dev/generate-tests.py
 #
```

### Comparing `awkward-cpp-8/tests-spec/test_pyawkward_IndexedArray32_getitem_nextcarry_64.py` & `awkward-cpp-9/tests-spec/test_pyawkward_IndexedArray32_getitem_nextcarry_64.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# AUTO GENERATED ON 2023-02-03 AT 22:54:31
+# AUTO GENERATED ON 2023-02-16 AT 15:37:39
 # DO NOT EDIT BY HAND!
 #
 # To regenerate file, run
 #
 #     python dev/generate-tests.py
 #
```

### Comparing `awkward-cpp-8/tests-spec/test_pyawkward_IndexedArray32_getitem_nextcarry_outindex_64.py` & `awkward-cpp-9/tests-spec/test_pyawkward_IndexedArrayU32_getitem_nextcarry_outindex_64.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,49 +1,49 @@
-# AUTO GENERATED ON 2023-02-03 AT 22:54:31
+# AUTO GENERATED ON 2023-02-16 AT 15:37:39
 # DO NOT EDIT BY HAND!
 #
 # To regenerate file, run
 #
 #     python dev/generate-tests.py
 #
 
 # fmt: off
 
 import pytest
 import kernels
 
-def test_pyawkward_IndexedArray32_getitem_nextcarry_outindex_64_1():
+def test_pyawkward_IndexedArrayU32_getitem_nextcarry_outindex_64_1():
     tocarry = [123, 123, 123]
     toindex = [123, 123, 123]
     fromindex = [1, 0, 0, 1, 1, 1, 0, 0, 1, 0, 1, 0, 1, 1]
     lenindex = 3
     lencontent = 2
-    funcPy = getattr(kernels, 'awkward_IndexedArray32_getitem_nextcarry_outindex_64')
+    funcPy = getattr(kernels, 'awkward_IndexedArrayU32_getitem_nextcarry_outindex_64')
     funcPy(tocarry=tocarry, toindex=toindex, fromindex=fromindex, lenindex=lenindex, lencontent=lencontent)
     pytest_tocarry = [1, 0, 0]
     assert tocarry[:len(pytest_tocarry)] == pytest.approx(pytest_tocarry)
     pytest_toindex = [0.0, 1.0, 2.0]
     assert toindex[:len(pytest_toindex)] == pytest.approx(pytest_toindex)
 
-def test_pyawkward_IndexedArray32_getitem_nextcarry_outindex_64_2():
+def test_pyawkward_IndexedArrayU32_getitem_nextcarry_outindex_64_2():
     tocarry = [123]
     toindex = [123]
     fromindex = [1, 4, 2, 3, 1, 2, 3, 1, 4, 3, 2, 1, 3, 2, 4, 5, 1, 2, 3, 4, 5]
     lenindex = 3
     lencontent = 2
-    funcPy = getattr(kernels, 'awkward_IndexedArray32_getitem_nextcarry_outindex_64')
+    funcPy = getattr(kernels, 'awkward_IndexedArrayU32_getitem_nextcarry_outindex_64')
     with pytest.raises(Exception):
         funcPy(tocarry=tocarry, toindex=toindex, fromindex=fromindex, lenindex=lenindex, lencontent=lencontent)
 
-def test_pyawkward_IndexedArray32_getitem_nextcarry_outindex_64_3():
+def test_pyawkward_IndexedArrayU32_getitem_nextcarry_outindex_64_3():
     tocarry = [123, 123, 123]
     toindex = [123, 123, 123]
     fromindex = [0, 0, 0, 0, 0, 0, 0, 0, 0, 0]
     lenindex = 3
     lencontent = 5
-    funcPy = getattr(kernels, 'awkward_IndexedArray32_getitem_nextcarry_outindex_64')
+    funcPy = getattr(kernels, 'awkward_IndexedArrayU32_getitem_nextcarry_outindex_64')
     funcPy(tocarry=tocarry, toindex=toindex, fromindex=fromindex, lenindex=lenindex, lencontent=lencontent)
     pytest_tocarry = [0, 0, 0]
     assert tocarry[:len(pytest_tocarry)] == pytest.approx(pytest_tocarry)
     pytest_toindex = [0.0, 1.0, 2.0]
     assert toindex[:len(pytest_toindex)] == pytest.approx(pytest_toindex)
```

### Comparing `awkward-cpp-8/tests-spec/test_pyawkward_IndexedArray32_numnull.py` & `awkward-cpp-9/tests-spec/test_pyawkward_IndexedArray32_numnull.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# AUTO GENERATED ON 2023-02-03 AT 22:54:31
+# AUTO GENERATED ON 2023-02-16 AT 15:37:39
 # DO NOT EDIT BY HAND!
 #
 # To regenerate file, run
 #
 #     python dev/generate-tests.py
 #
```

### Comparing `awkward-cpp-8/tests-spec/test_pyawkward_IndexedArray32_simplify32_to64.py` & `awkward-cpp-9/tests-spec/test_pyawkward_IndexedArray32_simplify32_to64.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# AUTO GENERATED ON 2023-02-03 AT 22:54:31
+# AUTO GENERATED ON 2023-02-16 AT 15:37:39
 # DO NOT EDIT BY HAND!
 #
 # To regenerate file, run
 #
 #     python dev/generate-tests.py
 #
```

### Comparing `awkward-cpp-8/tests-spec/test_pyawkward_IndexedArray32_simplify64_to64.py` & `awkward-cpp-9/tests-spec/test_pyawkward_IndexedArray32_simplify64_to64.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# AUTO GENERATED ON 2023-02-03 AT 22:54:31
+# AUTO GENERATED ON 2023-02-16 AT 15:37:39
 # DO NOT EDIT BY HAND!
 #
 # To regenerate file, run
 #
 #     python dev/generate-tests.py
 #
```

### Comparing `awkward-cpp-8/tests-spec/test_pyawkward_IndexedArray32_simplifyU32_to64.py` & `awkward-cpp-9/tests-spec/test_pyawkward_IndexedArray32_simplifyU32_to64.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# AUTO GENERATED ON 2023-02-03 AT 22:54:31
+# AUTO GENERATED ON 2023-02-16 AT 15:37:39
 # DO NOT EDIT BY HAND!
 #
 # To regenerate file, run
 #
 #     python dev/generate-tests.py
 #
```

### Comparing `awkward-cpp-8/tests-spec/test_pyawkward_IndexedArray32_validity.py` & `awkward-cpp-9/tests-spec/test_pyawkward_IndexedArray32_validity.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# AUTO GENERATED ON 2023-02-03 AT 22:54:31
+# AUTO GENERATED ON 2023-02-16 AT 15:37:39
 # DO NOT EDIT BY HAND!
 #
 # To regenerate file, run
 #
 #     python dev/generate-tests.py
 #
```

### Comparing `awkward-cpp-8/tests-spec/test_pyawkward_IndexedArray64_flatten_nextcarry_64.py` & `awkward-cpp-9/tests-spec/test_pyawkward_IndexedArray64_flatten_nextcarry_64.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# AUTO GENERATED ON 2023-02-03 AT 22:54:31
+# AUTO GENERATED ON 2023-02-16 AT 15:37:39
 # DO NOT EDIT BY HAND!
 #
 # To regenerate file, run
 #
 #     python dev/generate-tests.py
 #
```

### Comparing `awkward-cpp-8/tests-spec/test_pyawkward_IndexedArray64_flatten_none2empty_64.py` & `awkward-cpp-9/tests-spec/test_pyawkward_IndexedArray64_flatten_none2empty_64.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# AUTO GENERATED ON 2023-02-03 AT 22:54:31
+# AUTO GENERATED ON 2023-02-16 AT 15:37:39
 # DO NOT EDIT BY HAND!
 #
 # To regenerate file, run
 #
 #     python dev/generate-tests.py
 #
```

### Comparing `awkward-cpp-8/tests-spec/test_pyawkward_IndexedArray64_getitem_nextcarry_64.py` & `awkward-cpp-9/tests-spec/test_pyawkward_IndexedArray64_getitem_nextcarry_64.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# AUTO GENERATED ON 2023-02-03 AT 22:54:31
+# AUTO GENERATED ON 2023-02-16 AT 15:37:39
 # DO NOT EDIT BY HAND!
 #
 # To regenerate file, run
 #
 #     python dev/generate-tests.py
 #
```

### Comparing `awkward-cpp-8/tests-spec/test_pyawkward_IndexedArray64_getitem_nextcarry_outindex_64.py` & `awkward-cpp-9/tests-spec/test_pyawkward_IndexedArray64_getitem_nextcarry_outindex_64.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# AUTO GENERATED ON 2023-02-03 AT 22:54:31
+# AUTO GENERATED ON 2023-02-16 AT 15:37:39
 # DO NOT EDIT BY HAND!
 #
 # To regenerate file, run
 #
 #     python dev/generate-tests.py
 #
```

### Comparing `awkward-cpp-8/tests-spec/test_pyawkward_IndexedArray64_numnull.py` & `awkward-cpp-9/tests-spec/test_pyawkward_IndexedArray64_numnull.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# AUTO GENERATED ON 2023-02-03 AT 22:54:31
+# AUTO GENERATED ON 2023-02-16 AT 15:37:39
 # DO NOT EDIT BY HAND!
 #
 # To regenerate file, run
 #
 #     python dev/generate-tests.py
 #
```

### Comparing `awkward-cpp-8/tests-spec/test_pyawkward_IndexedArray64_simplify32_to64.py` & `awkward-cpp-9/tests-spec/test_pyawkward_IndexedArray64_simplify32_to64.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# AUTO GENERATED ON 2023-02-03 AT 22:54:31
+# AUTO GENERATED ON 2023-02-16 AT 15:37:39
 # DO NOT EDIT BY HAND!
 #
 # To regenerate file, run
 #
 #     python dev/generate-tests.py
 #
```

### Comparing `awkward-cpp-8/tests-spec/test_pyawkward_IndexedArray64_simplify64_to64.py` & `awkward-cpp-9/tests-spec/test_pyawkward_IndexedArray64_simplify64_to64.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# AUTO GENERATED ON 2023-02-03 AT 22:54:31
+# AUTO GENERATED ON 2023-02-16 AT 15:37:39
 # DO NOT EDIT BY HAND!
 #
 # To regenerate file, run
 #
 #     python dev/generate-tests.py
 #
```

### Comparing `awkward-cpp-8/tests-spec/test_pyawkward_IndexedArray64_simplifyU32_to64.py` & `awkward-cpp-9/tests-spec/test_pyawkward_IndexedArray64_simplifyU32_to64.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# AUTO GENERATED ON 2023-02-03 AT 22:54:31
+# AUTO GENERATED ON 2023-02-16 AT 15:37:39
 # DO NOT EDIT BY HAND!
 #
 # To regenerate file, run
 #
 #     python dev/generate-tests.py
 #
```

### Comparing `awkward-cpp-8/tests-spec/test_pyawkward_IndexedArray64_validity.py` & `awkward-cpp-9/tests-spec/test_pyawkward_IndexedArray64_validity.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# AUTO GENERATED ON 2023-02-03 AT 22:54:31
+# AUTO GENERATED ON 2023-02-16 AT 15:37:39
 # DO NOT EDIT BY HAND!
 #
 # To regenerate file, run
 #
 #     python dev/generate-tests.py
 #
```

### Comparing `awkward-cpp-8/tests-spec/test_pyawkward_IndexedArrayU32_flatten_nextcarry_64.py` & `awkward-cpp-9/tests-spec/test_pyawkward_IndexedArrayU32_flatten_nextcarry_64.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# AUTO GENERATED ON 2023-02-03 AT 22:54:31
+# AUTO GENERATED ON 2023-02-16 AT 15:37:39
 # DO NOT EDIT BY HAND!
 #
 # To regenerate file, run
 #
 #     python dev/generate-tests.py
 #
```

### Comparing `awkward-cpp-8/tests-spec/test_pyawkward_IndexedArrayU32_flatten_none2empty_64.py` & `awkward-cpp-9/tests-spec/test_pyawkward_IndexedArrayU32_flatten_none2empty_64.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# AUTO GENERATED ON 2023-02-03 AT 22:54:31
+# AUTO GENERATED ON 2023-02-16 AT 15:37:39
 # DO NOT EDIT BY HAND!
 #
 # To regenerate file, run
 #
 #     python dev/generate-tests.py
 #
```

### Comparing `awkward-cpp-8/tests-spec/test_pyawkward_IndexedArrayU32_getitem_nextcarry_64.py` & `awkward-cpp-9/tests-spec/test_pyawkward_IndexedArrayU32_getitem_nextcarry_64.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# AUTO GENERATED ON 2023-02-03 AT 22:54:31
+# AUTO GENERATED ON 2023-02-16 AT 15:37:39
 # DO NOT EDIT BY HAND!
 #
 # To regenerate file, run
 #
 #     python dev/generate-tests.py
 #
```

### Comparing `awkward-cpp-8/tests-spec/test_pyawkward_IndexedArrayU32_getitem_nextcarry_outindex_64.py` & `awkward-cpp-9/tests-spec/test_pyawkward_IndexedArray32_getitem_nextcarry_outindex_64.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,49 +1,49 @@
-# AUTO GENERATED ON 2023-02-03 AT 22:54:31
+# AUTO GENERATED ON 2023-02-16 AT 15:37:39
 # DO NOT EDIT BY HAND!
 #
 # To regenerate file, run
 #
 #     python dev/generate-tests.py
 #
 
 # fmt: off
 
 import pytest
 import kernels
 
-def test_pyawkward_IndexedArrayU32_getitem_nextcarry_outindex_64_1():
+def test_pyawkward_IndexedArray32_getitem_nextcarry_outindex_64_1():
     tocarry = [123, 123, 123]
     toindex = [123, 123, 123]
     fromindex = [1, 0, 0, 1, 1, 1, 0, 0, 1, 0, 1, 0, 1, 1]
     lenindex = 3
     lencontent = 2
-    funcPy = getattr(kernels, 'awkward_IndexedArrayU32_getitem_nextcarry_outindex_64')
+    funcPy = getattr(kernels, 'awkward_IndexedArray32_getitem_nextcarry_outindex_64')
     funcPy(tocarry=tocarry, toindex=toindex, fromindex=fromindex, lenindex=lenindex, lencontent=lencontent)
     pytest_tocarry = [1, 0, 0]
     assert tocarry[:len(pytest_tocarry)] == pytest.approx(pytest_tocarry)
     pytest_toindex = [0.0, 1.0, 2.0]
     assert toindex[:len(pytest_toindex)] == pytest.approx(pytest_toindex)
 
-def test_pyawkward_IndexedArrayU32_getitem_nextcarry_outindex_64_2():
+def test_pyawkward_IndexedArray32_getitem_nextcarry_outindex_64_2():
     tocarry = [123]
     toindex = [123]
     fromindex = [1, 4, 2, 3, 1, 2, 3, 1, 4, 3, 2, 1, 3, 2, 4, 5, 1, 2, 3, 4, 5]
     lenindex = 3
     lencontent = 2
-    funcPy = getattr(kernels, 'awkward_IndexedArrayU32_getitem_nextcarry_outindex_64')
+    funcPy = getattr(kernels, 'awkward_IndexedArray32_getitem_nextcarry_outindex_64')
     with pytest.raises(Exception):
         funcPy(tocarry=tocarry, toindex=toindex, fromindex=fromindex, lenindex=lenindex, lencontent=lencontent)
 
-def test_pyawkward_IndexedArrayU32_getitem_nextcarry_outindex_64_3():
+def test_pyawkward_IndexedArray32_getitem_nextcarry_outindex_64_3():
     tocarry = [123, 123, 123]
     toindex = [123, 123, 123]
     fromindex = [0, 0, 0, 0, 0, 0, 0, 0, 0, 0]
     lenindex = 3
     lencontent = 5
-    funcPy = getattr(kernels, 'awkward_IndexedArrayU32_getitem_nextcarry_outindex_64')
+    funcPy = getattr(kernels, 'awkward_IndexedArray32_getitem_nextcarry_outindex_64')
     funcPy(tocarry=tocarry, toindex=toindex, fromindex=fromindex, lenindex=lenindex, lencontent=lencontent)
     pytest_tocarry = [0, 0, 0]
     assert tocarry[:len(pytest_tocarry)] == pytest.approx(pytest_tocarry)
     pytest_toindex = [0.0, 1.0, 2.0]
     assert toindex[:len(pytest_toindex)] == pytest.approx(pytest_toindex)
```

### Comparing `awkward-cpp-8/tests-spec/test_pyawkward_IndexedArrayU32_numnull.py` & `awkward-cpp-9/tests-spec/test_pyawkward_IndexedArrayU32_numnull.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# AUTO GENERATED ON 2023-02-03 AT 22:54:31
+# AUTO GENERATED ON 2023-02-16 AT 15:37:39
 # DO NOT EDIT BY HAND!
 #
 # To regenerate file, run
 #
 #     python dev/generate-tests.py
 #
```

### Comparing `awkward-cpp-8/tests-spec/test_pyawkward_IndexedArrayU32_simplify32_to64.py` & `awkward-cpp-9/tests-spec/test_pyawkward_IndexedArrayU32_simplify32_to64.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# AUTO GENERATED ON 2023-02-03 AT 22:54:31
+# AUTO GENERATED ON 2023-02-16 AT 15:37:39
 # DO NOT EDIT BY HAND!
 #
 # To regenerate file, run
 #
 #     python dev/generate-tests.py
 #
```

### Comparing `awkward-cpp-8/tests-spec/test_pyawkward_IndexedArrayU32_simplify64_to64.py` & `awkward-cpp-9/tests-spec/test_pyawkward_IndexedArrayU32_simplify64_to64.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# AUTO GENERATED ON 2023-02-03 AT 22:54:31
+# AUTO GENERATED ON 2023-02-16 AT 15:37:39
 # DO NOT EDIT BY HAND!
 #
 # To regenerate file, run
 #
 #     python dev/generate-tests.py
 #
```

### Comparing `awkward-cpp-8/tests-spec/test_pyawkward_IndexedArrayU32_simplifyU32_to64.py` & `awkward-cpp-9/tests-spec/test_pyawkward_IndexedArrayU32_simplifyU32_to64.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# AUTO GENERATED ON 2023-02-03 AT 22:54:31
+# AUTO GENERATED ON 2023-02-16 AT 15:37:39
 # DO NOT EDIT BY HAND!
 #
 # To regenerate file, run
 #
 #     python dev/generate-tests.py
 #
```

### Comparing `awkward-cpp-8/tests-spec/test_pyawkward_IndexedArrayU32_validity.py` & `awkward-cpp-9/tests-spec/test_pyawkward_IndexedArrayU32_validity.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# AUTO GENERATED ON 2023-02-03 AT 22:54:31
+# AUTO GENERATED ON 2023-02-16 AT 15:37:39
 # DO NOT EDIT BY HAND!
 #
 # To regenerate file, run
 #
 #     python dev/generate-tests.py
 #
```

### Comparing `awkward-cpp-8/tests-spec/test_pyawkward_IndexedArray_fill_to64_count.py` & `awkward-cpp-9/tests-spec/test_pyawkward_IndexedArray_fill_to64_count.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# AUTO GENERATED ON 2023-02-03 AT 22:54:31
+# AUTO GENERATED ON 2023-02-16 AT 15:37:39
 # DO NOT EDIT BY HAND!
 #
 # To regenerate file, run
 #
 #     python dev/generate-tests.py
 #
```

### Comparing `awkward-cpp-8/tests-spec/test_pyawkward_IndexedArray_fill_to64_from32.py` & `awkward-cpp-9/tests-spec/test_pyawkward_IndexedArray_fill_to64_from32.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# AUTO GENERATED ON 2023-02-03 AT 22:54:31
+# AUTO GENERATED ON 2023-02-16 AT 15:37:39
 # DO NOT EDIT BY HAND!
 #
 # To regenerate file, run
 #
 #     python dev/generate-tests.py
 #
```

### Comparing `awkward-cpp-8/tests-spec/test_pyawkward_IndexedArray_fill_to64_from64.py` & `awkward-cpp-9/tests-spec/test_pyawkward_IndexedArray_fill_to64_from64.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# AUTO GENERATED ON 2023-02-03 AT 22:54:31
+# AUTO GENERATED ON 2023-02-16 AT 15:37:39
 # DO NOT EDIT BY HAND!
 #
 # To regenerate file, run
 #
 #     python dev/generate-tests.py
 #
```

### Comparing `awkward-cpp-8/tests-spec/test_pyawkward_IndexedArray_fill_to64_fromU32.py` & `awkward-cpp-9/tests-spec/test_pyawkward_IndexedArray_fill_to64_fromU32.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# AUTO GENERATED ON 2023-02-03 AT 22:54:31
+# AUTO GENERATED ON 2023-02-16 AT 15:37:39
 # DO NOT EDIT BY HAND!
 #
 # To regenerate file, run
 #
 #     python dev/generate-tests.py
 #
```

### Comparing `awkward-cpp-8/tests-spec/test_pyawkward_IndexedOptionArray_rpad_and_clip_mask_axis1_64.py` & `awkward-cpp-9/tests-spec/test_pyawkward_IndexedOptionArray_rpad_and_clip_mask_axis1_64.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# AUTO GENERATED ON 2023-02-03 AT 22:54:31
+# AUTO GENERATED ON 2023-02-16 AT 15:37:39
 # DO NOT EDIT BY HAND!
 #
 # To regenerate file, run
 #
 #     python dev/generate-tests.py
 #
```

### Comparing `awkward-cpp-8/tests-spec/test_pyawkward_ListArray32_broadcast_tooffsets_64.py` & `awkward-cpp-9/tests-spec/test_pyawkward_ListArray32_broadcast_tooffsets_64.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# AUTO GENERATED ON 2023-02-03 AT 22:54:31
+# AUTO GENERATED ON 2023-02-16 AT 15:37:39
 # DO NOT EDIT BY HAND!
 #
 # To regenerate file, run
 #
 #     python dev/generate-tests.py
 #
```

### Comparing `awkward-cpp-8/tests-spec/test_pyawkward_ListArray32_combinations_length_64.py` & `awkward-cpp-9/tests-spec/test_pyawkward_ListArray32_combinations_length_64.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# AUTO GENERATED ON 2023-02-03 AT 22:54:31
+# AUTO GENERATED ON 2023-02-16 AT 15:37:39
 # DO NOT EDIT BY HAND!
 #
 # To regenerate file, run
 #
 #     python dev/generate-tests.py
 #
```

### Comparing `awkward-cpp-8/tests-spec/test_pyawkward_ListArray32_compact_offsets_64.py` & `awkward-cpp-9/tests-spec/test_pyawkward_ListArray32_compact_offsets_64.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# AUTO GENERATED ON 2023-02-03 AT 22:54:31
+# AUTO GENERATED ON 2023-02-16 AT 15:37:39
 # DO NOT EDIT BY HAND!
 #
 # To regenerate file, run
 #
 #     python dev/generate-tests.py
 #
```

### Comparing `awkward-cpp-8/tests-spec/test_pyawkward_ListArray32_getitem_jagged_apply_64.py` & `awkward-cpp-9/tests-spec/test_pyawkward_ListArray32_getitem_jagged_apply_64.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# AUTO GENERATED ON 2023-02-03 AT 22:54:31
+# AUTO GENERATED ON 2023-02-16 AT 15:37:39
 # DO NOT EDIT BY HAND!
 #
 # To regenerate file, run
 #
 #     python dev/generate-tests.py
 #
```

### Comparing `awkward-cpp-8/tests-spec/test_pyawkward_ListArray32_getitem_jagged_descend_64.py` & `awkward-cpp-9/tests-spec/test_pyawkward_ListArray32_getitem_jagged_descend_64.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# AUTO GENERATED ON 2023-02-03 AT 22:54:31
+# AUTO GENERATED ON 2023-02-16 AT 15:37:39
 # DO NOT EDIT BY HAND!
 #
 # To regenerate file, run
 #
 #     python dev/generate-tests.py
 #
```

### Comparing `awkward-cpp-8/tests-spec/test_pyawkward_ListArray32_getitem_jagged_expand_64.py` & `awkward-cpp-9/tests-spec/test_pyawkward_ListArray32_getitem_jagged_expand_64.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# AUTO GENERATED ON 2023-02-03 AT 22:54:31
+# AUTO GENERATED ON 2023-02-16 AT 15:37:39
 # DO NOT EDIT BY HAND!
 #
 # To regenerate file, run
 #
 #     python dev/generate-tests.py
 #
```

### Comparing `awkward-cpp-8/tests-spec/test_pyawkward_ListArray32_getitem_next_array_64.py` & `awkward-cpp-9/tests-spec/test_pyawkward_ListArray32_getitem_next_array_64.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# AUTO GENERATED ON 2023-02-03 AT 22:54:31
+# AUTO GENERATED ON 2023-02-16 AT 15:37:39
 # DO NOT EDIT BY HAND!
 #
 # To regenerate file, run
 #
 #     python dev/generate-tests.py
 #
```

### Comparing `awkward-cpp-8/tests-spec/test_pyawkward_ListArray32_getitem_next_array_advanced_64.py` & `awkward-cpp-9/tests-spec/test_pyawkward_ListArray32_getitem_next_array_advanced_64.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# AUTO GENERATED ON 2023-02-03 AT 22:54:31
+# AUTO GENERATED ON 2023-02-16 AT 15:37:39
 # DO NOT EDIT BY HAND!
 #
 # To regenerate file, run
 #
 #     python dev/generate-tests.py
 #
```

### Comparing `awkward-cpp-8/tests-spec/test_pyawkward_ListArray32_getitem_next_at_64.py` & `awkward-cpp-9/tests-spec/test_pyawkward_ListArray32_getitem_next_at_64.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# AUTO GENERATED ON 2023-02-03 AT 22:54:31
+# AUTO GENERATED ON 2023-02-16 AT 15:37:39
 # DO NOT EDIT BY HAND!
 #
 # To regenerate file, run
 #
 #     python dev/generate-tests.py
 #
```

### Comparing `awkward-cpp-8/tests-spec/test_pyawkward_ListArray32_getitem_next_range_counts_64.py` & `awkward-cpp-9/tests-spec/test_pyawkward_ListArray32_getitem_next_range_counts_64.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# AUTO GENERATED ON 2023-02-03 AT 22:54:31
+# AUTO GENERATED ON 2023-02-16 AT 15:37:39
 # DO NOT EDIT BY HAND!
 #
 # To regenerate file, run
 #
 #     python dev/generate-tests.py
 #
```

### Comparing `awkward-cpp-8/tests-spec/test_pyawkward_ListArray32_localindex_64.py` & `awkward-cpp-9/tests-spec/test_pyawkward_ListArray64_localindex_64.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,40 +1,40 @@
-# AUTO GENERATED ON 2023-02-03 AT 22:54:31
+# AUTO GENERATED ON 2023-02-16 AT 15:37:39
 # DO NOT EDIT BY HAND!
 #
 # To regenerate file, run
 #
 #     python dev/generate-tests.py
 #
 
 # fmt: off
 
 import pytest
 import kernels
 
-def test_pyawkward_ListArray32_localindex_64_1():
+def test_pyawkward_ListArray64_localindex_64_1():
     toindex = [123, 123, 123, 123]
     offsets = [2, 3, 3, 4, 5, 5, 5, 5, 5, 6, 7, 8, 10, 11]
     length = 3
-    funcPy = getattr(kernels, 'awkward_ListArray32_localindex_64')
+    funcPy = getattr(kernels, 'awkward_ListArray64_localindex_64')
     funcPy(toindex=toindex, offsets=offsets, length=length)
     pytest_toindex = [123, 123, 0, 0]
     assert toindex[:len(pytest_toindex)] == pytest.approx(pytest_toindex)
 
-def test_pyawkward_ListArray32_localindex_64_2():
+def test_pyawkward_ListArray64_localindex_64_2():
     toindex = [123]
     offsets = [2, 1, 0, 1, 2, 0, 1, 2, 2, 2, 1, 2, 1, 0, 0, 0, 0]
     length = 3
-    funcPy = getattr(kernels, 'awkward_ListArray32_localindex_64')
+    funcPy = getattr(kernels, 'awkward_ListArray64_localindex_64')
     funcPy(toindex=toindex, offsets=offsets, length=length)
     pytest_toindex = [0]
     assert toindex[:len(pytest_toindex)] == pytest.approx(pytest_toindex)
 
-def test_pyawkward_ListArray32_localindex_64_3():
+def test_pyawkward_ListArray64_localindex_64_3():
     toindex = [123, 123, 123]
     offsets = [1, 0, 2, 3, 1, 2, 0, 0, 1, 1, 2, 3, 1, 2, 3, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1]
     length = 3
-    funcPy = getattr(kernels, 'awkward_ListArray32_localindex_64')
+    funcPy = getattr(kernels, 'awkward_ListArray64_localindex_64')
     funcPy(toindex=toindex, offsets=offsets, length=length)
     pytest_toindex = [0, 1, 0]
     assert toindex[:len(pytest_toindex)] == pytest.approx(pytest_toindex)
```

### Comparing `awkward-cpp-8/tests-spec/test_pyawkward_ListArray32_min_range.py` & `awkward-cpp-9/tests-spec/test_pyawkward_ListArray32_min_range.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# AUTO GENERATED ON 2023-02-03 AT 22:54:31
+# AUTO GENERATED ON 2023-02-16 AT 15:37:39
 # DO NOT EDIT BY HAND!
 #
 # To regenerate file, run
 #
 #     python dev/generate-tests.py
 #
```

### Comparing `awkward-cpp-8/tests-spec/test_pyawkward_ListArray32_rpad_and_clip_length_axis1.py` & `awkward-cpp-9/tests-spec/test_pyawkward_ListArray32_rpad_and_clip_length_axis1.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# AUTO GENERATED ON 2023-02-03 AT 22:54:31
+# AUTO GENERATED ON 2023-02-16 AT 15:37:39
 # DO NOT EDIT BY HAND!
 #
 # To regenerate file, run
 #
 #     python dev/generate-tests.py
 #
```

### Comparing `awkward-cpp-8/tests-spec/test_pyawkward_ListArray32_rpad_axis1_64.py` & `awkward-cpp-9/tests-spec/test_pyawkward_ListArray32_rpad_axis1_64.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# AUTO GENERATED ON 2023-02-03 AT 22:54:31
+# AUTO GENERATED ON 2023-02-16 AT 15:37:39
 # DO NOT EDIT BY HAND!
 #
 # To regenerate file, run
 #
 #     python dev/generate-tests.py
 #
```

### Comparing `awkward-cpp-8/tests-spec/test_pyawkward_ListArray32_validity.py` & `awkward-cpp-9/tests-spec/test_pyawkward_ListArray32_validity.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# AUTO GENERATED ON 2023-02-03 AT 22:54:31
+# AUTO GENERATED ON 2023-02-16 AT 15:37:39
 # DO NOT EDIT BY HAND!
 #
 # To regenerate file, run
 #
 #     python dev/generate-tests.py
 #
```

### Comparing `awkward-cpp-8/tests-spec/test_pyawkward_ListArray64_broadcast_tooffsets_64.py` & `awkward-cpp-9/tests-spec/test_pyawkward_ListArrayU32_broadcast_tooffsets_64.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,35 +1,35 @@
-# AUTO GENERATED ON 2023-02-03 AT 22:54:31
+# AUTO GENERATED ON 2023-02-16 AT 15:37:39
 # DO NOT EDIT BY HAND!
 #
 # To regenerate file, run
 #
 #     python dev/generate-tests.py
 #
 
 # fmt: off
 
 import pytest
 import kernels
 
-def test_pyawkward_ListArray64_broadcast_tooffsets_64_1():
+def test_pyawkward_ListArrayU32_broadcast_tooffsets_64_1():
     tocarry = [123]
     fromoffsets = [2, 3, 3, 4, 5, 5, 5, 5, 5, 6, 7, 8, 10, 11]
     offsetslength = 3
     fromstarts = [2, 0, 2, 1, 2, 1, 2, 1, 2, 1, 2, 1]
     fromstops = [3, 2, 4, 5, 3, 4, 2, 5, 3, 4, 6, 11]
     lencontent = 3
-    funcPy = getattr(kernels, 'awkward_ListArray64_broadcast_tooffsets_64')
+    funcPy = getattr(kernels, 'awkward_ListArrayU32_broadcast_tooffsets_64')
     with pytest.raises(Exception):
         funcPy(tocarry=tocarry, fromoffsets=fromoffsets, offsetslength=offsetslength, fromstarts=fromstarts, fromstops=fromstops, lencontent=lencontent)
 
-def test_pyawkward_ListArray64_broadcast_tooffsets_64_2():
+def test_pyawkward_ListArrayU32_broadcast_tooffsets_64_2():
     tocarry = [123]
     fromoffsets = [2, 3, 3, 4, 5, 5, 5, 5, 5, 6, 7, 8, 10, 11]
     offsetslength = 3
     fromstarts = [0, 0, 0, 0, 0, 0, 0, 0]
     fromstops = [1, 1, 1, 1, 1, 1, 1, 1]
     lencontent = 6
-    funcPy = getattr(kernels, 'awkward_ListArray64_broadcast_tooffsets_64')
+    funcPy = getattr(kernels, 'awkward_ListArrayU32_broadcast_tooffsets_64')
     with pytest.raises(Exception):
         funcPy(tocarry=tocarry, fromoffsets=fromoffsets, offsetslength=offsetslength, fromstarts=fromstarts, fromstops=fromstops, lencontent=lencontent)
```

### Comparing `awkward-cpp-8/tests-spec/test_pyawkward_ListArray64_combinations_length_64.py` & `awkward-cpp-9/tests-spec/test_pyawkward_ListArray64_combinations_length_64.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# AUTO GENERATED ON 2023-02-03 AT 22:54:31
+# AUTO GENERATED ON 2023-02-16 AT 15:37:39
 # DO NOT EDIT BY HAND!
 #
 # To regenerate file, run
 #
 #     python dev/generate-tests.py
 #
```

### Comparing `awkward-cpp-8/tests-spec/test_pyawkward_ListArray64_compact_offsets_64.py` & `awkward-cpp-9/tests-spec/test_pyawkward_ListArray64_compact_offsets_64.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# AUTO GENERATED ON 2023-02-03 AT 22:54:31
+# AUTO GENERATED ON 2023-02-16 AT 15:37:39
 # DO NOT EDIT BY HAND!
 #
 # To regenerate file, run
 #
 #     python dev/generate-tests.py
 #
```

### Comparing `awkward-cpp-8/tests-spec/test_pyawkward_ListArray64_getitem_jagged_apply_64.py` & `awkward-cpp-9/tests-spec/test_pyawkward_ListArray64_getitem_jagged_apply_64.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# AUTO GENERATED ON 2023-02-03 AT 22:54:31
+# AUTO GENERATED ON 2023-02-16 AT 15:37:39
 # DO NOT EDIT BY HAND!
 #
 # To regenerate file, run
 #
 #     python dev/generate-tests.py
 #
```

### Comparing `awkward-cpp-8/tests-spec/test_pyawkward_ListArray64_getitem_jagged_descend_64.py` & `awkward-cpp-9/tests-spec/test_pyawkward_ListArray64_getitem_jagged_descend_64.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# AUTO GENERATED ON 2023-02-03 AT 22:54:31
+# AUTO GENERATED ON 2023-02-16 AT 15:37:39
 # DO NOT EDIT BY HAND!
 #
 # To regenerate file, run
 #
 #     python dev/generate-tests.py
 #
```

### Comparing `awkward-cpp-8/tests-spec/test_pyawkward_ListArray64_getitem_jagged_expand_64.py` & `awkward-cpp-9/tests-spec/test_pyawkward_ListArray64_getitem_jagged_expand_64.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# AUTO GENERATED ON 2023-02-03 AT 22:54:31
+# AUTO GENERATED ON 2023-02-16 AT 15:37:39
 # DO NOT EDIT BY HAND!
 #
 # To regenerate file, run
 #
 #     python dev/generate-tests.py
 #
```

### Comparing `awkward-cpp-8/tests-spec/test_pyawkward_ListArray64_getitem_next_array_64.py` & `awkward-cpp-9/tests-spec/test_pyawkward_ListArray64_getitem_next_array_64.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# AUTO GENERATED ON 2023-02-03 AT 22:54:31
+# AUTO GENERATED ON 2023-02-16 AT 15:37:39
 # DO NOT EDIT BY HAND!
 #
 # To regenerate file, run
 #
 #     python dev/generate-tests.py
 #
```

### Comparing `awkward-cpp-8/tests-spec/test_pyawkward_ListArray64_getitem_next_array_advanced_64.py` & `awkward-cpp-9/tests-spec/test_pyawkward_ListArray64_getitem_next_array_advanced_64.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# AUTO GENERATED ON 2023-02-03 AT 22:54:31
+# AUTO GENERATED ON 2023-02-16 AT 15:37:39
 # DO NOT EDIT BY HAND!
 #
 # To regenerate file, run
 #
 #     python dev/generate-tests.py
 #
```

### Comparing `awkward-cpp-8/tests-spec/test_pyawkward_ListArray64_getitem_next_at_64.py` & `awkward-cpp-9/tests-spec/test_pyawkward_ListArray64_getitem_next_at_64.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# AUTO GENERATED ON 2023-02-03 AT 22:54:31
+# AUTO GENERATED ON 2023-02-16 AT 15:37:39
 # DO NOT EDIT BY HAND!
 #
 # To regenerate file, run
 #
 #     python dev/generate-tests.py
 #
```

### Comparing `awkward-cpp-8/tests-spec/test_pyawkward_ListArray64_getitem_next_range_counts_64.py` & `awkward-cpp-9/tests-spec/test_pyawkward_ListArray64_getitem_next_range_counts_64.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# AUTO GENERATED ON 2023-02-03 AT 22:54:31
+# AUTO GENERATED ON 2023-02-16 AT 15:37:39
 # DO NOT EDIT BY HAND!
 #
 # To regenerate file, run
 #
 #     python dev/generate-tests.py
 #
```

### Comparing `awkward-cpp-8/tests-spec/test_pyawkward_ListArray64_localindex_64.py` & `awkward-cpp-9/tests-spec/test_pyawkward_ListArray32_localindex_64.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,40 +1,40 @@
-# AUTO GENERATED ON 2023-02-03 AT 22:54:31
+# AUTO GENERATED ON 2023-02-16 AT 15:37:39
 # DO NOT EDIT BY HAND!
 #
 # To regenerate file, run
 #
 #     python dev/generate-tests.py
 #
 
 # fmt: off
 
 import pytest
 import kernels
 
-def test_pyawkward_ListArray64_localindex_64_1():
+def test_pyawkward_ListArray32_localindex_64_1():
     toindex = [123, 123, 123, 123]
     offsets = [2, 3, 3, 4, 5, 5, 5, 5, 5, 6, 7, 8, 10, 11]
     length = 3
-    funcPy = getattr(kernels, 'awkward_ListArray64_localindex_64')
+    funcPy = getattr(kernels, 'awkward_ListArray32_localindex_64')
     funcPy(toindex=toindex, offsets=offsets, length=length)
     pytest_toindex = [123, 123, 0, 0]
     assert toindex[:len(pytest_toindex)] == pytest.approx(pytest_toindex)
 
-def test_pyawkward_ListArray64_localindex_64_2():
+def test_pyawkward_ListArray32_localindex_64_2():
     toindex = [123]
     offsets = [2, 1, 0, 1, 2, 0, 1, 2, 2, 2, 1, 2, 1, 0, 0, 0, 0]
     length = 3
-    funcPy = getattr(kernels, 'awkward_ListArray64_localindex_64')
+    funcPy = getattr(kernels, 'awkward_ListArray32_localindex_64')
     funcPy(toindex=toindex, offsets=offsets, length=length)
     pytest_toindex = [0]
     assert toindex[:len(pytest_toindex)] == pytest.approx(pytest_toindex)
 
-def test_pyawkward_ListArray64_localindex_64_3():
+def test_pyawkward_ListArray32_localindex_64_3():
     toindex = [123, 123, 123]
     offsets = [1, 0, 2, 3, 1, 2, 0, 0, 1, 1, 2, 3, 1, 2, 3, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1]
     length = 3
-    funcPy = getattr(kernels, 'awkward_ListArray64_localindex_64')
+    funcPy = getattr(kernels, 'awkward_ListArray32_localindex_64')
     funcPy(toindex=toindex, offsets=offsets, length=length)
     pytest_toindex = [0, 1, 0]
     assert toindex[:len(pytest_toindex)] == pytest.approx(pytest_toindex)
```

### Comparing `awkward-cpp-8/tests-spec/test_pyawkward_ListArray64_min_range.py` & `awkward-cpp-9/tests-spec/test_pyawkward_ListArray64_min_range.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# AUTO GENERATED ON 2023-02-03 AT 22:54:31
+# AUTO GENERATED ON 2023-02-16 AT 15:37:39
 # DO NOT EDIT BY HAND!
 #
 # To regenerate file, run
 #
 #     python dev/generate-tests.py
 #
```

### Comparing `awkward-cpp-8/tests-spec/test_pyawkward_ListArray64_rpad_and_clip_length_axis1.py` & `awkward-cpp-9/tests-spec/test_pyawkward_ListArray64_rpad_and_clip_length_axis1.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# AUTO GENERATED ON 2023-02-03 AT 22:54:31
+# AUTO GENERATED ON 2023-02-16 AT 15:37:39
 # DO NOT EDIT BY HAND!
 #
 # To regenerate file, run
 #
 #     python dev/generate-tests.py
 #
```

### Comparing `awkward-cpp-8/tests-spec/test_pyawkward_ListArray64_rpad_axis1_64.py` & `awkward-cpp-9/tests-spec/test_pyawkward_ListArray64_rpad_axis1_64.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# AUTO GENERATED ON 2023-02-03 AT 22:54:31
+# AUTO GENERATED ON 2023-02-16 AT 15:37:39
 # DO NOT EDIT BY HAND!
 #
 # To regenerate file, run
 #
 #     python dev/generate-tests.py
 #
```

### Comparing `awkward-cpp-8/tests-spec/test_pyawkward_ListArray64_validity.py` & `awkward-cpp-9/tests-spec/test_pyawkward_ListArray64_validity.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# AUTO GENERATED ON 2023-02-03 AT 22:54:31
+# AUTO GENERATED ON 2023-02-16 AT 15:37:39
 # DO NOT EDIT BY HAND!
 #
 # To regenerate file, run
 #
 #     python dev/generate-tests.py
 #
```

### Comparing `awkward-cpp-8/tests-spec/test_pyawkward_ListArrayU32_broadcast_tooffsets_64.py` & `awkward-cpp-9/tests-spec/test_pyawkward_ListArray64_broadcast_tooffsets_64.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,35 +1,35 @@
-# AUTO GENERATED ON 2023-02-03 AT 22:54:31
+# AUTO GENERATED ON 2023-02-16 AT 15:37:39
 # DO NOT EDIT BY HAND!
 #
 # To regenerate file, run
 #
 #     python dev/generate-tests.py
 #
 
 # fmt: off
 
 import pytest
 import kernels
 
-def test_pyawkward_ListArrayU32_broadcast_tooffsets_64_1():
+def test_pyawkward_ListArray64_broadcast_tooffsets_64_1():
     tocarry = [123]
     fromoffsets = [2, 3, 3, 4, 5, 5, 5, 5, 5, 6, 7, 8, 10, 11]
     offsetslength = 3
     fromstarts = [2, 0, 2, 1, 2, 1, 2, 1, 2, 1, 2, 1]
     fromstops = [3, 2, 4, 5, 3, 4, 2, 5, 3, 4, 6, 11]
     lencontent = 3
-    funcPy = getattr(kernels, 'awkward_ListArrayU32_broadcast_tooffsets_64')
+    funcPy = getattr(kernels, 'awkward_ListArray64_broadcast_tooffsets_64')
     with pytest.raises(Exception):
         funcPy(tocarry=tocarry, fromoffsets=fromoffsets, offsetslength=offsetslength, fromstarts=fromstarts, fromstops=fromstops, lencontent=lencontent)
 
-def test_pyawkward_ListArrayU32_broadcast_tooffsets_64_2():
+def test_pyawkward_ListArray64_broadcast_tooffsets_64_2():
     tocarry = [123]
     fromoffsets = [2, 3, 3, 4, 5, 5, 5, 5, 5, 6, 7, 8, 10, 11]
     offsetslength = 3
     fromstarts = [0, 0, 0, 0, 0, 0, 0, 0]
     fromstops = [1, 1, 1, 1, 1, 1, 1, 1]
     lencontent = 6
-    funcPy = getattr(kernels, 'awkward_ListArrayU32_broadcast_tooffsets_64')
+    funcPy = getattr(kernels, 'awkward_ListArray64_broadcast_tooffsets_64')
     with pytest.raises(Exception):
         funcPy(tocarry=tocarry, fromoffsets=fromoffsets, offsetslength=offsetslength, fromstarts=fromstarts, fromstops=fromstops, lencontent=lencontent)
```

### Comparing `awkward-cpp-8/tests-spec/test_pyawkward_ListArrayU32_combinations_length_64.py` & `awkward-cpp-9/tests-spec/test_pyawkward_ListArrayU32_combinations_length_64.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# AUTO GENERATED ON 2023-02-03 AT 22:54:31
+# AUTO GENERATED ON 2023-02-16 AT 15:37:39
 # DO NOT EDIT BY HAND!
 #
 # To regenerate file, run
 #
 #     python dev/generate-tests.py
 #
```

### Comparing `awkward-cpp-8/tests-spec/test_pyawkward_ListArrayU32_compact_offsets_64.py` & `awkward-cpp-9/tests-spec/test_pyawkward_ListArrayU32_compact_offsets_64.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# AUTO GENERATED ON 2023-02-03 AT 22:54:31
+# AUTO GENERATED ON 2023-02-16 AT 15:37:39
 # DO NOT EDIT BY HAND!
 #
 # To regenerate file, run
 #
 #     python dev/generate-tests.py
 #
```

### Comparing `awkward-cpp-8/tests-spec/test_pyawkward_ListArrayU32_getitem_jagged_apply_64.py` & `awkward-cpp-9/tests-spec/test_pyawkward_ListArrayU32_getitem_jagged_apply_64.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# AUTO GENERATED ON 2023-02-03 AT 22:54:31
+# AUTO GENERATED ON 2023-02-16 AT 15:37:39
 # DO NOT EDIT BY HAND!
 #
 # To regenerate file, run
 #
 #     python dev/generate-tests.py
 #
```

### Comparing `awkward-cpp-8/tests-spec/test_pyawkward_ListArrayU32_getitem_jagged_descend_64.py` & `awkward-cpp-9/tests-spec/test_pyawkward_ListArrayU32_getitem_jagged_descend_64.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# AUTO GENERATED ON 2023-02-03 AT 22:54:31
+# AUTO GENERATED ON 2023-02-16 AT 15:37:39
 # DO NOT EDIT BY HAND!
 #
 # To regenerate file, run
 #
 #     python dev/generate-tests.py
 #
```

### Comparing `awkward-cpp-8/tests-spec/test_pyawkward_ListArrayU32_getitem_jagged_expand_64.py` & `awkward-cpp-9/tests-spec/test_pyawkward_ListArrayU32_getitem_jagged_expand_64.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# AUTO GENERATED ON 2023-02-03 AT 22:54:31
+# AUTO GENERATED ON 2023-02-16 AT 15:37:39
 # DO NOT EDIT BY HAND!
 #
 # To regenerate file, run
 #
 #     python dev/generate-tests.py
 #
```

### Comparing `awkward-cpp-8/tests-spec/test_pyawkward_ListArrayU32_getitem_next_array_64.py` & `awkward-cpp-9/tests-spec/test_pyawkward_ListArrayU32_getitem_next_array_64.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# AUTO GENERATED ON 2023-02-03 AT 22:54:31
+# AUTO GENERATED ON 2023-02-16 AT 15:37:39
 # DO NOT EDIT BY HAND!
 #
 # To regenerate file, run
 #
 #     python dev/generate-tests.py
 #
```

### Comparing `awkward-cpp-8/tests-spec/test_pyawkward_ListArrayU32_getitem_next_array_advanced_64.py` & `awkward-cpp-9/tests-spec/test_pyawkward_ListArrayU32_getitem_next_array_advanced_64.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# AUTO GENERATED ON 2023-02-03 AT 22:54:31
+# AUTO GENERATED ON 2023-02-16 AT 15:37:39
 # DO NOT EDIT BY HAND!
 #
 # To regenerate file, run
 #
 #     python dev/generate-tests.py
 #
```

### Comparing `awkward-cpp-8/tests-spec/test_pyawkward_ListArrayU32_getitem_next_at_64.py` & `awkward-cpp-9/tests-spec/test_pyawkward_ListArrayU32_getitem_next_at_64.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# AUTO GENERATED ON 2023-02-03 AT 22:54:31
+# AUTO GENERATED ON 2023-02-16 AT 15:37:39
 # DO NOT EDIT BY HAND!
 #
 # To regenerate file, run
 #
 #     python dev/generate-tests.py
 #
```

### Comparing `awkward-cpp-8/tests-spec/test_pyawkward_ListArrayU32_getitem_next_range_counts_64.py` & `awkward-cpp-9/tests-spec/test_pyawkward_ListArrayU32_getitem_next_range_counts_64.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# AUTO GENERATED ON 2023-02-03 AT 22:54:31
+# AUTO GENERATED ON 2023-02-16 AT 15:37:39
 # DO NOT EDIT BY HAND!
 #
 # To regenerate file, run
 #
 #     python dev/generate-tests.py
 #
```

### Comparing `awkward-cpp-8/tests-spec/test_pyawkward_ListArrayU32_localindex_64.py` & `awkward-cpp-9/tests-spec/test_pyawkward_ListArrayU32_localindex_64.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# AUTO GENERATED ON 2023-02-03 AT 22:54:31
+# AUTO GENERATED ON 2023-02-16 AT 15:37:39
 # DO NOT EDIT BY HAND!
 #
 # To regenerate file, run
 #
 #     python dev/generate-tests.py
 #
```

### Comparing `awkward-cpp-8/tests-spec/test_pyawkward_ListArrayU32_min_range.py` & `awkward-cpp-9/tests-spec/test_pyawkward_ListArrayU32_min_range.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# AUTO GENERATED ON 2023-02-03 AT 22:54:31
+# AUTO GENERATED ON 2023-02-16 AT 15:37:39
 # DO NOT EDIT BY HAND!
 #
 # To regenerate file, run
 #
 #     python dev/generate-tests.py
 #
```

### Comparing `awkward-cpp-8/tests-spec/test_pyawkward_ListArrayU32_rpad_and_clip_length_axis1.py` & `awkward-cpp-9/tests-spec/test_pyawkward_ListArrayU32_rpad_and_clip_length_axis1.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# AUTO GENERATED ON 2023-02-03 AT 22:54:31
+# AUTO GENERATED ON 2023-02-16 AT 15:37:39
 # DO NOT EDIT BY HAND!
 #
 # To regenerate file, run
 #
 #     python dev/generate-tests.py
 #
```

### Comparing `awkward-cpp-8/tests-spec/test_pyawkward_ListArrayU32_rpad_axis1_64.py` & `awkward-cpp-9/tests-spec/test_pyawkward_ListArrayU32_rpad_axis1_64.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# AUTO GENERATED ON 2023-02-03 AT 22:54:31
+# AUTO GENERATED ON 2023-02-16 AT 15:37:39
 # DO NOT EDIT BY HAND!
 #
 # To regenerate file, run
 #
 #     python dev/generate-tests.py
 #
```

### Comparing `awkward-cpp-8/tests-spec/test_pyawkward_ListArrayU32_validity.py` & `awkward-cpp-9/tests-spec/test_pyawkward_ListArrayU32_validity.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# AUTO GENERATED ON 2023-02-03 AT 22:54:31
+# AUTO GENERATED ON 2023-02-16 AT 15:37:39
 # DO NOT EDIT BY HAND!
 #
 # To regenerate file, run
 #
 #     python dev/generate-tests.py
 #
```

### Comparing `awkward-cpp-8/tests-spec/test_pyawkward_ListArray_fill_to64_from32.py` & `awkward-cpp-9/tests-spec/test_pyawkward_ListArray_fill_to64_from32.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# AUTO GENERATED ON 2023-02-03 AT 22:54:31
+# AUTO GENERATED ON 2023-02-16 AT 15:37:39
 # DO NOT EDIT BY HAND!
 #
 # To regenerate file, run
 #
 #     python dev/generate-tests.py
 #
```

### Comparing `awkward-cpp-8/tests-spec/test_pyawkward_ListArray_fill_to64_from64.py` & `awkward-cpp-9/tests-spec/test_pyawkward_ListArray_fill_to64_from64.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# AUTO GENERATED ON 2023-02-03 AT 22:54:31
+# AUTO GENERATED ON 2023-02-16 AT 15:37:39
 # DO NOT EDIT BY HAND!
 #
 # To regenerate file, run
 #
 #     python dev/generate-tests.py
 #
```

### Comparing `awkward-cpp-8/tests-spec/test_pyawkward_ListArray_fill_to64_fromU32.py` & `awkward-cpp-9/tests-spec/test_pyawkward_ListArray_fill_to64_fromU32.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# AUTO GENERATED ON 2023-02-03 AT 22:54:31
+# AUTO GENERATED ON 2023-02-16 AT 15:37:39
 # DO NOT EDIT BY HAND!
 #
 # To regenerate file, run
 #
 #     python dev/generate-tests.py
 #
```

### Comparing `awkward-cpp-8/tests-spec/test_pyawkward_ListArray_getitem_jagged_carrylen_64.py` & `awkward-cpp-9/tests-spec/test_pyawkward_ListArray_getitem_jagged_carrylen_64.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# AUTO GENERATED ON 2023-02-03 AT 22:54:31
+# AUTO GENERATED ON 2023-02-16 AT 15:37:39
 # DO NOT EDIT BY HAND!
 #
 # To regenerate file, run
 #
 #     python dev/generate-tests.py
 #
```

### Comparing `awkward-cpp-8/tests-spec/test_pyawkward_ListArray_getitem_jagged_shrink_64.py` & `awkward-cpp-9/tests-spec/test_pyawkward_ListArray_getitem_jagged_shrink_64.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# AUTO GENERATED ON 2023-02-03 AT 22:54:31
+# AUTO GENERATED ON 2023-02-16 AT 15:37:39
 # DO NOT EDIT BY HAND!
 #
 # To regenerate file, run
 #
 #     python dev/generate-tests.py
 #
```

### Comparing `awkward-cpp-8/tests-spec/test_pyawkward_ListOffsetArray32_compact_offsets_64.py` & `awkward-cpp-9/tests-spec/test_pyawkward_ListOffsetArray32_compact_offsets_64.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# AUTO GENERATED ON 2023-02-03 AT 22:54:31
+# AUTO GENERATED ON 2023-02-16 AT 15:37:39
 # DO NOT EDIT BY HAND!
 #
 # To regenerate file, run
 #
 #     python dev/generate-tests.py
 #
```

### Comparing `awkward-cpp-8/tests-spec/test_pyawkward_ListOffsetArray32_flatten_offsets_64.py` & `awkward-cpp-9/tests-spec/test_pyawkward_ListOffsetArray32_flatten_offsets_64.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# AUTO GENERATED ON 2023-02-03 AT 22:54:31
+# AUTO GENERATED ON 2023-02-16 AT 15:37:39
 # DO NOT EDIT BY HAND!
 #
 # To regenerate file, run
 #
 #     python dev/generate-tests.py
 #
```

### Comparing `awkward-cpp-8/tests-spec/test_pyawkward_ListOffsetArray32_toRegularArray.py` & `awkward-cpp-9/tests-spec/test_pyawkward_ListOffsetArray32_toRegularArray.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# AUTO GENERATED ON 2023-02-03 AT 22:54:31
+# AUTO GENERATED ON 2023-02-16 AT 15:37:39
 # DO NOT EDIT BY HAND!
 #
 # To regenerate file, run
 #
 #     python dev/generate-tests.py
 #
```

### Comparing `awkward-cpp-8/tests-spec/test_pyawkward_ListOffsetArray64_compact_offsets_64.py` & `awkward-cpp-9/tests-spec/test_pyawkward_ListOffsetArray64_compact_offsets_64.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# AUTO GENERATED ON 2023-02-03 AT 22:54:31
+# AUTO GENERATED ON 2023-02-16 AT 15:37:39
 # DO NOT EDIT BY HAND!
 #
 # To regenerate file, run
 #
 #     python dev/generate-tests.py
 #
```

### Comparing `awkward-cpp-8/tests-spec/test_pyawkward_ListOffsetArray64_flatten_offsets_64.py` & `awkward-cpp-9/tests-spec/test_pyawkward_ListOffsetArray64_flatten_offsets_64.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# AUTO GENERATED ON 2023-02-03 AT 22:54:31
+# AUTO GENERATED ON 2023-02-16 AT 15:37:39
 # DO NOT EDIT BY HAND!
 #
 # To regenerate file, run
 #
 #     python dev/generate-tests.py
 #
```

### Comparing `awkward-cpp-8/tests-spec/test_pyawkward_ListOffsetArray64_toRegularArray.py` & `awkward-cpp-9/tests-spec/test_pyawkward_ListOffsetArray64_toRegularArray.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# AUTO GENERATED ON 2023-02-03 AT 22:54:31
+# AUTO GENERATED ON 2023-02-16 AT 15:37:39
 # DO NOT EDIT BY HAND!
 #
 # To regenerate file, run
 #
 #     python dev/generate-tests.py
 #
```

### Comparing `awkward-cpp-8/tests-spec/test_pyawkward_ListOffsetArrayU32_compact_offsets_64.py` & `awkward-cpp-9/tests-spec/test_pyawkward_ListOffsetArrayU32_compact_offsets_64.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# AUTO GENERATED ON 2023-02-03 AT 22:54:31
+# AUTO GENERATED ON 2023-02-16 AT 15:37:39
 # DO NOT EDIT BY HAND!
 #
 # To regenerate file, run
 #
 #     python dev/generate-tests.py
 #
```

### Comparing `awkward-cpp-8/tests-spec/test_pyawkward_ListOffsetArrayU32_flatten_offsets_64.py` & `awkward-cpp-9/tests-spec/test_pyawkward_ListOffsetArrayU32_flatten_offsets_64.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# AUTO GENERATED ON 2023-02-03 AT 22:54:31
+# AUTO GENERATED ON 2023-02-16 AT 15:37:39
 # DO NOT EDIT BY HAND!
 #
 # To regenerate file, run
 #
 #     python dev/generate-tests.py
 #
```

### Comparing `awkward-cpp-8/tests-spec/test_pyawkward_ListOffsetArrayU32_toRegularArray.py` & `awkward-cpp-9/tests-spec/test_pyawkward_ListOffsetArrayU32_toRegularArray.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# AUTO GENERATED ON 2023-02-03 AT 22:54:31
+# AUTO GENERATED ON 2023-02-16 AT 15:37:39
 # DO NOT EDIT BY HAND!
 #
 # To regenerate file, run
 #
 #     python dev/generate-tests.py
 #
```

### Comparing `awkward-cpp-8/tests-spec/test_pyawkward_ListOffsetArray_drop_none_indexes_32.py` & `awkward-cpp-9/tests-spec/test_pyawkward_ListOffsetArray_drop_none_indexes_32.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# AUTO GENERATED ON 2023-02-03 AT 22:54:31
+# AUTO GENERATED ON 2023-02-16 AT 15:37:39
 # DO NOT EDIT BY HAND!
 #
 # To regenerate file, run
 #
 #     python dev/generate-tests.py
 #
```

### Comparing `awkward-cpp-8/tests-spec/test_pyawkward_ListOffsetArray_drop_none_indexes_64.py` & `awkward-cpp-9/tests-spec/test_pyawkward_ListOffsetArray_drop_none_indexes_64.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# AUTO GENERATED ON 2023-02-03 AT 22:54:31
+# AUTO GENERATED ON 2023-02-16 AT 15:37:39
 # DO NOT EDIT BY HAND!
 #
 # To regenerate file, run
 #
 #     python dev/generate-tests.py
 #
```

### Comparing `awkward-cpp-8/tests-spec/test_pyawkward_MaskedArray32_getitem_next_jagged_project.py` & `awkward-cpp-9/tests-spec/test_pyawkward_MaskedArray32_getitem_next_jagged_project.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# AUTO GENERATED ON 2023-02-03 AT 22:54:31
+# AUTO GENERATED ON 2023-02-16 AT 15:37:39
 # DO NOT EDIT BY HAND!
 #
 # To regenerate file, run
 #
 #     python dev/generate-tests.py
 #
```

### Comparing `awkward-cpp-8/tests-spec/test_pyawkward_MaskedArray64_getitem_next_jagged_project.py` & `awkward-cpp-9/tests-spec/test_pyawkward_MaskedArray64_getitem_next_jagged_project.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# AUTO GENERATED ON 2023-02-03 AT 22:54:31
+# AUTO GENERATED ON 2023-02-16 AT 15:37:39
 # DO NOT EDIT BY HAND!
 #
 # To regenerate file, run
 #
 #     python dev/generate-tests.py
 #
```

### Comparing `awkward-cpp-8/tests-spec/test_pyawkward_MaskedArrayU32_getitem_next_jagged_project.py` & `awkward-cpp-9/tests-spec/test_pyawkward_MaskedArrayU32_getitem_next_jagged_project.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# AUTO GENERATED ON 2023-02-03 AT 22:54:31
+# AUTO GENERATED ON 2023-02-16 AT 15:37:39
 # DO NOT EDIT BY HAND!
 #
 # To regenerate file, run
 #
 #     python dev/generate-tests.py
 #
```

### Comparing `awkward-cpp-8/tests-spec/test_pyawkward_RegularArray_broadcast_tooffsets_64.py` & `awkward-cpp-9/tests-spec/test_pyawkward_RegularArray_broadcast_tooffsets_64.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# AUTO GENERATED ON 2023-02-03 AT 22:54:31
+# AUTO GENERATED ON 2023-02-16 AT 15:37:39
 # DO NOT EDIT BY HAND!
 #
 # To regenerate file, run
 #
 #     python dev/generate-tests.py
 #
```

### Comparing `awkward-cpp-8/tests-spec/test_pyawkward_RegularArray_broadcast_tooffsets_size1_64.py` & `awkward-cpp-9/tests-spec/test_pyawkward_RegularArray_broadcast_tooffsets_size1_64.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# AUTO GENERATED ON 2023-02-03 AT 22:54:31
+# AUTO GENERATED ON 2023-02-16 AT 15:37:39
 # DO NOT EDIT BY HAND!
 #
 # To regenerate file, run
 #
 #     python dev/generate-tests.py
 #
```

### Comparing `awkward-cpp-8/tests-spec/test_pyawkward_RegularArray_compact_offsets64.py` & `awkward-cpp-9/tests-spec/test_pyawkward_RegularArray_compact_offsets64.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# AUTO GENERATED ON 2023-02-03 AT 22:54:31
+# AUTO GENERATED ON 2023-02-16 AT 15:37:39
 # DO NOT EDIT BY HAND!
 #
 # To regenerate file, run
 #
 #     python dev/generate-tests.py
 #
```

### Comparing `awkward-cpp-8/tests-spec/test_pyawkward_RegularArray_getitem_carry_64.py` & `awkward-cpp-9/tests-spec/test_pyawkward_RegularArray_getitem_carry_64.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# AUTO GENERATED ON 2023-02-03 AT 22:54:31
+# AUTO GENERATED ON 2023-02-16 AT 15:37:39
 # DO NOT EDIT BY HAND!
 #
 # To regenerate file, run
 #
 #     python dev/generate-tests.py
 #
```

### Comparing `awkward-cpp-8/tests-spec/test_pyawkward_RegularArray_getitem_jagged_expand_64.py` & `awkward-cpp-9/tests-spec/test_pyawkward_RegularArray_getitem_jagged_expand_64.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# AUTO GENERATED ON 2023-02-03 AT 22:54:31
+# AUTO GENERATED ON 2023-02-16 AT 15:37:39
 # DO NOT EDIT BY HAND!
 #
 # To regenerate file, run
 #
 #     python dev/generate-tests.py
 #
```

### Comparing `awkward-cpp-8/tests-spec/test_pyawkward_RegularArray_getitem_next_array_64.py` & `awkward-cpp-9/tests-spec/test_pyawkward_RegularArray_getitem_next_array_64.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# AUTO GENERATED ON 2023-02-03 AT 22:54:31
+# AUTO GENERATED ON 2023-02-16 AT 15:37:39
 # DO NOT EDIT BY HAND!
 #
 # To regenerate file, run
 #
 #     python dev/generate-tests.py
 #
```

### Comparing `awkward-cpp-8/tests-spec/test_pyawkward_RegularArray_getitem_next_array_advanced_64.py` & `awkward-cpp-9/tests-spec/test_pyawkward_RegularArray_getitem_next_array_advanced_64.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# AUTO GENERATED ON 2023-02-03 AT 22:54:31
+# AUTO GENERATED ON 2023-02-16 AT 15:37:39
 # DO NOT EDIT BY HAND!
 #
 # To regenerate file, run
 #
 #     python dev/generate-tests.py
 #
```

### Comparing `awkward-cpp-8/tests-spec/test_pyawkward_RegularArray_getitem_next_array_regularize_64.py` & `awkward-cpp-9/tests-spec/test_pyawkward_RegularArray_getitem_next_array_regularize_64.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# AUTO GENERATED ON 2023-02-03 AT 22:54:31
+# AUTO GENERATED ON 2023-02-16 AT 15:37:39
 # DO NOT EDIT BY HAND!
 #
 # To regenerate file, run
 #
 #     python dev/generate-tests.py
 #
```

### Comparing `awkward-cpp-8/tests-spec/test_pyawkward_RegularArray_getitem_next_at_64.py` & `awkward-cpp-9/tests-spec/test_pyawkward_RegularArray_getitem_next_at_64.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# AUTO GENERATED ON 2023-02-03 AT 22:54:31
+# AUTO GENERATED ON 2023-02-16 AT 15:37:39
 # DO NOT EDIT BY HAND!
 #
 # To regenerate file, run
 #
 #     python dev/generate-tests.py
 #
```

### Comparing `awkward-cpp-8/tests-spec/test_pyawkward_RegularArray_getitem_next_range_64.py` & `awkward-cpp-9/tests-spec/test_pyawkward_RegularArray_getitem_next_range_64.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# AUTO GENERATED ON 2023-02-03 AT 22:54:31
+# AUTO GENERATED ON 2023-02-16 AT 15:37:39
 # DO NOT EDIT BY HAND!
 #
 # To regenerate file, run
 #
 #     python dev/generate-tests.py
 #
```

### Comparing `awkward-cpp-8/tests-spec/test_pyawkward_RegularArray_getitem_next_range_spreadadvanced_64.py` & `awkward-cpp-9/tests-spec/test_pyawkward_RegularArray_getitem_next_range_spreadadvanced_64.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# AUTO GENERATED ON 2023-02-03 AT 22:54:31
+# AUTO GENERATED ON 2023-02-16 AT 15:37:39
 # DO NOT EDIT BY HAND!
 #
 # To regenerate file, run
 #
 #     python dev/generate-tests.py
 #
```

### Comparing `awkward-cpp-8/tests-spec/test_pyawkward_RegularArray_localindex_64.py` & `awkward-cpp-9/tests-spec/test_pyawkward_RegularArray_localindex_64.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# AUTO GENERATED ON 2023-02-03 AT 22:54:31
+# AUTO GENERATED ON 2023-02-16 AT 15:37:39
 # DO NOT EDIT BY HAND!
 #
 # To regenerate file, run
 #
 #     python dev/generate-tests.py
 #
```

### Comparing `awkward-cpp-8/tests-spec/test_pyawkward_RegularArray_rpad_and_clip_axis1_64.py` & `awkward-cpp-9/tests-spec/test_pyawkward_UnionArray_fillindex_to64_count.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,23 +1,22 @@
-# AUTO GENERATED ON 2023-02-03 AT 22:54:31
+# AUTO GENERATED ON 2023-02-16 AT 15:37:39
 # DO NOT EDIT BY HAND!
 #
 # To regenerate file, run
 #
 #     python dev/generate-tests.py
 #
 
 # fmt: off
 
 import pytest
 import kernels
 
-def test_pyawkward_RegularArray_rpad_and_clip_axis1_64_1():
-    toindex = [123, 123, 123, 123, 123, 123, 123, 123, 123]
-    target = 3
-    size = 3
+def test_pyawkward_UnionArray_fillindex_to64_count_1():
+    toindex = [123, 123, 123, 123, 123, 123]
+    toindexoffset = 3
     length = 3
-    funcPy = getattr(kernels, 'awkward_RegularArray_rpad_and_clip_axis1_64')
-    funcPy(toindex=toindex, target=target, size=size, length=length)
-    pytest_toindex = [0, 1, 2, 3, 4, 5, 6, 7, 8]
+    funcPy = getattr(kernels, 'awkward_UnionArray_fillindex_to64_count')
+    funcPy(toindex=toindex, toindexoffset=toindexoffset, length=length)
+    pytest_toindex = [123, 123, 123, 0.0, 1.0, 2.0]
     assert toindex[:len(pytest_toindex)] == pytest.approx(pytest_toindex)
```

### Comparing `awkward-cpp-8/tests-spec/test_pyawkward_UnionArray8_32_project_64.py` & `awkward-cpp-9/tests-spec/test_pyawkward_UnionArray8_32_project_64.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# AUTO GENERATED ON 2023-02-03 AT 22:54:31
+# AUTO GENERATED ON 2023-02-16 AT 15:37:39
 # DO NOT EDIT BY HAND!
 #
 # To regenerate file, run
 #
 #     python dev/generate-tests.py
 #
```

### Comparing `awkward-cpp-8/tests-spec/test_pyawkward_UnionArray8_32_regular_index.py` & `awkward-cpp-9/tests-spec/test_pyawkward_UnionArray8_32_regular_index.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# AUTO GENERATED ON 2023-02-03 AT 22:54:31
+# AUTO GENERATED ON 2023-02-16 AT 15:37:39
 # DO NOT EDIT BY HAND!
 #
 # To regenerate file, run
 #
 #     python dev/generate-tests.py
 #
```

### Comparing `awkward-cpp-8/tests-spec/test_pyawkward_UnionArray8_32_simplify8_32_to8_64.py` & `awkward-cpp-9/tests-spec/test_pyawkward_UnionArray8_32_simplify8_32_to8_64.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# AUTO GENERATED ON 2023-02-03 AT 22:54:31
+# AUTO GENERATED ON 2023-02-16 AT 15:37:39
 # DO NOT EDIT BY HAND!
 #
 # To regenerate file, run
 #
 #     python dev/generate-tests.py
 #
```

### Comparing `awkward-cpp-8/tests-spec/test_pyawkward_UnionArray8_32_simplify8_64_to8_64.py` & `awkward-cpp-9/tests-spec/test_pyawkward_UnionArray8_32_simplify8_64_to8_64.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# AUTO GENERATED ON 2023-02-03 AT 22:54:31
+# AUTO GENERATED ON 2023-02-16 AT 15:37:39
 # DO NOT EDIT BY HAND!
 #
 # To regenerate file, run
 #
 #     python dev/generate-tests.py
 #
```

### Comparing `awkward-cpp-8/tests-spec/test_pyawkward_UnionArray8_32_simplify8_U32_to8_64.py` & `awkward-cpp-9/tests-spec/test_pyawkward_UnionArray8_32_simplify8_U32_to8_64.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# AUTO GENERATED ON 2023-02-03 AT 22:54:31
+# AUTO GENERATED ON 2023-02-16 AT 15:37:39
 # DO NOT EDIT BY HAND!
 #
 # To regenerate file, run
 #
 #     python dev/generate-tests.py
 #
```

### Comparing `awkward-cpp-8/tests-spec/test_pyawkward_UnionArray8_32_simplify_one_to8_64.py` & `awkward-cpp-9/tests-spec/test_pyawkward_UnionArray8_32_simplify_one_to8_64.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# AUTO GENERATED ON 2023-02-03 AT 22:54:31
+# AUTO GENERATED ON 2023-02-16 AT 15:37:39
 # DO NOT EDIT BY HAND!
 #
 # To regenerate file, run
 #
 #     python dev/generate-tests.py
 #
```

### Comparing `awkward-cpp-8/tests-spec/test_pyawkward_UnionArray8_32_validity.py` & `awkward-cpp-9/tests-spec/test_pyawkward_UnionArray8_32_validity.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# AUTO GENERATED ON 2023-02-03 AT 22:54:31
+# AUTO GENERATED ON 2023-02-16 AT 15:37:39
 # DO NOT EDIT BY HAND!
 #
 # To regenerate file, run
 #
 #     python dev/generate-tests.py
 #
```

### Comparing `awkward-cpp-8/tests-spec/test_pyawkward_UnionArray8_64_project_64.py` & `awkward-cpp-9/tests-spec/test_pyawkward_UnionArray8_64_project_64.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# AUTO GENERATED ON 2023-02-03 AT 22:54:31
+# AUTO GENERATED ON 2023-02-16 AT 15:37:39
 # DO NOT EDIT BY HAND!
 #
 # To regenerate file, run
 #
 #     python dev/generate-tests.py
 #
```

### Comparing `awkward-cpp-8/tests-spec/test_pyawkward_UnionArray8_64_regular_index.py` & `awkward-cpp-9/tests-spec/test_pyawkward_UnionArray8_64_regular_index.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# AUTO GENERATED ON 2023-02-03 AT 22:54:31
+# AUTO GENERATED ON 2023-02-16 AT 15:37:39
 # DO NOT EDIT BY HAND!
 #
 # To regenerate file, run
 #
 #     python dev/generate-tests.py
 #
```

### Comparing `awkward-cpp-8/tests-spec/test_pyawkward_UnionArray8_64_simplify8_32_to8_64.py` & `awkward-cpp-9/tests-spec/test_pyawkward_UnionArray8_64_simplify8_32_to8_64.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# AUTO GENERATED ON 2023-02-03 AT 22:54:31
+# AUTO GENERATED ON 2023-02-16 AT 15:37:39
 # DO NOT EDIT BY HAND!
 #
 # To regenerate file, run
 #
 #     python dev/generate-tests.py
 #
```

### Comparing `awkward-cpp-8/tests-spec/test_pyawkward_UnionArray8_64_simplify8_64_to8_64.py` & `awkward-cpp-9/tests-spec/test_pyawkward_UnionArray8_64_simplify8_64_to8_64.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# AUTO GENERATED ON 2023-02-03 AT 22:54:31
+# AUTO GENERATED ON 2023-02-16 AT 15:37:39
 # DO NOT EDIT BY HAND!
 #
 # To regenerate file, run
 #
 #     python dev/generate-tests.py
 #
```

### Comparing `awkward-cpp-8/tests-spec/test_pyawkward_UnionArray8_64_simplify8_U32_to8_64.py` & `awkward-cpp-9/tests-spec/test_pyawkward_UnionArray8_64_simplify8_U32_to8_64.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# AUTO GENERATED ON 2023-02-03 AT 22:54:31
+# AUTO GENERATED ON 2023-02-16 AT 15:37:39
 # DO NOT EDIT BY HAND!
 #
 # To regenerate file, run
 #
 #     python dev/generate-tests.py
 #
```

### Comparing `awkward-cpp-8/tests-spec/test_pyawkward_UnionArray8_64_simplify_one_to8_64.py` & `awkward-cpp-9/tests-spec/test_pyawkward_UnionArray8_64_simplify_one_to8_64.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# AUTO GENERATED ON 2023-02-03 AT 22:54:31
+# AUTO GENERATED ON 2023-02-16 AT 15:37:39
 # DO NOT EDIT BY HAND!
 #
 # To regenerate file, run
 #
 #     python dev/generate-tests.py
 #
```

### Comparing `awkward-cpp-8/tests-spec/test_pyawkward_UnionArray8_64_validity.py` & `awkward-cpp-9/tests-spec/test_pyawkward_UnionArray8_64_validity.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# AUTO GENERATED ON 2023-02-03 AT 22:54:31
+# AUTO GENERATED ON 2023-02-16 AT 15:37:39
 # DO NOT EDIT BY HAND!
 #
 # To regenerate file, run
 #
 #     python dev/generate-tests.py
 #
```

### Comparing `awkward-cpp-8/tests-spec/test_pyawkward_UnionArray8_U32_project_64.py` & `awkward-cpp-9/tests-spec/test_pyawkward_UnionArray8_U32_project_64.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# AUTO GENERATED ON 2023-02-03 AT 22:54:31
+# AUTO GENERATED ON 2023-02-16 AT 15:37:39
 # DO NOT EDIT BY HAND!
 #
 # To regenerate file, run
 #
 #     python dev/generate-tests.py
 #
```

### Comparing `awkward-cpp-8/tests-spec/test_pyawkward_UnionArray8_U32_regular_index.py` & `awkward-cpp-9/tests-spec/test_pyawkward_UnionArray8_U32_regular_index.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# AUTO GENERATED ON 2023-02-03 AT 22:54:31
+# AUTO GENERATED ON 2023-02-16 AT 15:37:39
 # DO NOT EDIT BY HAND!
 #
 # To regenerate file, run
 #
 #     python dev/generate-tests.py
 #
```

### Comparing `awkward-cpp-8/tests-spec/test_pyawkward_UnionArray8_U32_simplify8_32_to8_64.py` & `awkward-cpp-9/tests-spec/test_pyawkward_UnionArray8_U32_simplify8_32_to8_64.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# AUTO GENERATED ON 2023-02-03 AT 22:54:31
+# AUTO GENERATED ON 2023-02-16 AT 15:37:39
 # DO NOT EDIT BY HAND!
 #
 # To regenerate file, run
 #
 #     python dev/generate-tests.py
 #
```

### Comparing `awkward-cpp-8/tests-spec/test_pyawkward_UnionArray8_U32_simplify8_64_to8_64.py` & `awkward-cpp-9/tests-spec/test_pyawkward_UnionArray8_U32_simplify8_64_to8_64.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# AUTO GENERATED ON 2023-02-03 AT 22:54:31
+# AUTO GENERATED ON 2023-02-16 AT 15:37:39
 # DO NOT EDIT BY HAND!
 #
 # To regenerate file, run
 #
 #     python dev/generate-tests.py
 #
```

### Comparing `awkward-cpp-8/tests-spec/test_pyawkward_UnionArray8_U32_simplify8_U32_to8_64.py` & `awkward-cpp-9/tests-spec/test_pyawkward_UnionArray8_U32_simplify8_U32_to8_64.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# AUTO GENERATED ON 2023-02-03 AT 22:54:31
+# AUTO GENERATED ON 2023-02-16 AT 15:37:39
 # DO NOT EDIT BY HAND!
 #
 # To regenerate file, run
 #
 #     python dev/generate-tests.py
 #
```

### Comparing `awkward-cpp-8/tests-spec/test_pyawkward_UnionArray8_U32_simplify_one_to8_64.py` & `awkward-cpp-9/tests-spec/test_pyawkward_UnionArray8_U32_simplify_one_to8_64.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# AUTO GENERATED ON 2023-02-03 AT 22:54:31
+# AUTO GENERATED ON 2023-02-16 AT 15:37:39
 # DO NOT EDIT BY HAND!
 #
 # To regenerate file, run
 #
 #     python dev/generate-tests.py
 #
```

### Comparing `awkward-cpp-8/tests-spec/test_pyawkward_UnionArray8_U32_validity.py` & `awkward-cpp-9/tests-spec/test_pyawkward_UnionArray8_U32_validity.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# AUTO GENERATED ON 2023-02-03 AT 22:54:31
+# AUTO GENERATED ON 2023-02-16 AT 15:37:39
 # DO NOT EDIT BY HAND!
 #
 # To regenerate file, run
 #
 #     python dev/generate-tests.py
 #
```

### Comparing `awkward-cpp-8/tests-spec/test_pyawkward_UnionArray8_regular_index_getsize.py` & `awkward-cpp-9/tests-spec/test_pyawkward_UnionArray8_regular_index_getsize.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# AUTO GENERATED ON 2023-02-03 AT 22:54:31
+# AUTO GENERATED ON 2023-02-16 AT 15:37:39
 # DO NOT EDIT BY HAND!
 #
 # To regenerate file, run
 #
 #     python dev/generate-tests.py
 #
```

### Comparing `awkward-cpp-8/tests-spec/test_pyawkward_UnionArray_fillindex_to64_from32.py` & `awkward-cpp-9/tests-spec/test_pyawkward_UnionArray_fillindex_to64_from32.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# AUTO GENERATED ON 2023-02-03 AT 22:54:31
+# AUTO GENERATED ON 2023-02-16 AT 15:37:39
 # DO NOT EDIT BY HAND!
 #
 # To regenerate file, run
 #
 #     python dev/generate-tests.py
 #
```

### Comparing `awkward-cpp-8/tests-spec/test_pyawkward_UnionArray_fillindex_to64_from64.py` & `awkward-cpp-9/tests-spec/test_pyawkward_UnionArray_fillindex_to64_fromU32.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,63 +1,63 @@
-# AUTO GENERATED ON 2023-02-03 AT 22:54:31
+# AUTO GENERATED ON 2023-02-16 AT 15:37:39
 # DO NOT EDIT BY HAND!
 #
 # To regenerate file, run
 #
 #     python dev/generate-tests.py
 #
 
 # fmt: off
 
 import pytest
 import kernels
 
-def test_pyawkward_UnionArray_fillindex_to64_from64_1():
+def test_pyawkward_UnionArray_fillindex_to64_fromU32_1():
     toindex = [123, 123, 123, 123, 123, 123]
     toindexoffset = 3
     fromindex = [1, 0, 0, 1, 1, 1, 0, 0, 1, 0, 1, 0, 1, 1]
     length = 3
-    funcPy = getattr(kernels, 'awkward_UnionArray_fillindex_to64_from64')
+    funcPy = getattr(kernels, 'awkward_UnionArray_fillindex_to64_fromU32')
     funcPy(toindex=toindex, toindexoffset=toindexoffset, fromindex=fromindex, length=length)
     pytest_toindex = [123, 123, 123, 1.0, 0.0, 0.0]
     assert toindex[:len(pytest_toindex)] == pytest.approx(pytest_toindex)
 
-def test_pyawkward_UnionArray_fillindex_to64_from64_2():
+def test_pyawkward_UnionArray_fillindex_to64_fromU32_2():
     toindex = [123, 123, 123, 123, 123, 123]
     toindexoffset = 3
     fromindex = [1, 2, 2, 3, 0, 2, 0, 2, 1, 1]
     length = 3
-    funcPy = getattr(kernels, 'awkward_UnionArray_fillindex_to64_from64')
+    funcPy = getattr(kernels, 'awkward_UnionArray_fillindex_to64_fromU32')
     funcPy(toindex=toindex, toindexoffset=toindexoffset, fromindex=fromindex, length=length)
     pytest_toindex = [123, 123, 123, 1.0, 2.0, 2.0]
     assert toindex[:len(pytest_toindex)] == pytest.approx(pytest_toindex)
 
-def test_pyawkward_UnionArray_fillindex_to64_from64_3():
+def test_pyawkward_UnionArray_fillindex_to64_fromU32_3():
     toindex = [123, 123, 123, 123, 123, 123]
     toindexoffset = 3
     fromindex = [1, 3, 0, 3, 5, 2, 0, 2, 1, 1]
     length = 3
-    funcPy = getattr(kernels, 'awkward_UnionArray_fillindex_to64_from64')
+    funcPy = getattr(kernels, 'awkward_UnionArray_fillindex_to64_fromU32')
     funcPy(toindex=toindex, toindexoffset=toindexoffset, fromindex=fromindex, length=length)
     pytest_toindex = [123, 123, 123, 1.0, 3.0, 0.0]
     assert toindex[:len(pytest_toindex)] == pytest.approx(pytest_toindex)
 
-def test_pyawkward_UnionArray_fillindex_to64_from64_4():
+def test_pyawkward_UnionArray_fillindex_to64_fromU32_4():
     toindex = [123, 123, 123, 123, 123, 123]
     toindexoffset = 3
     fromindex = [1, 4, 2, 3, 1, 2, 3, 1, 4, 3, 2, 1, 3, 2, 4, 5, 1, 2, 3, 4, 5]
     length = 3
-    funcPy = getattr(kernels, 'awkward_UnionArray_fillindex_to64_from64')
+    funcPy = getattr(kernels, 'awkward_UnionArray_fillindex_to64_fromU32')
     funcPy(toindex=toindex, toindexoffset=toindexoffset, fromindex=fromindex, length=length)
     pytest_toindex = [123, 123, 123, 1.0, 4.0, 2.0]
     assert toindex[:len(pytest_toindex)] == pytest.approx(pytest_toindex)
 
-def test_pyawkward_UnionArray_fillindex_to64_from64_5():
+def test_pyawkward_UnionArray_fillindex_to64_fromU32_5():
     toindex = [123, 123, 123, 123, 123, 123]
     toindexoffset = 3
     fromindex = [0, 0, 0, 0, 0, 0, 0, 0, 0, 0]
     length = 3
-    funcPy = getattr(kernels, 'awkward_UnionArray_fillindex_to64_from64')
+    funcPy = getattr(kernels, 'awkward_UnionArray_fillindex_to64_fromU32')
     funcPy(toindex=toindex, toindexoffset=toindexoffset, fromindex=fromindex, length=length)
     pytest_toindex = [123, 123, 123, 0.0, 0.0, 0.0]
     assert toindex[:len(pytest_toindex)] == pytest.approx(pytest_toindex)
```

### Comparing `awkward-cpp-8/tests-spec/test_pyawkward_UnionArray_fillindex_to64_fromU32.py` & `awkward-cpp-9/tests-spec/test_pyawkward_UnionArray_fillindex_to64_from64.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,63 +1,63 @@
-# AUTO GENERATED ON 2023-02-03 AT 22:54:31
+# AUTO GENERATED ON 2023-02-16 AT 15:37:39
 # DO NOT EDIT BY HAND!
 #
 # To regenerate file, run
 #
 #     python dev/generate-tests.py
 #
 
 # fmt: off
 
 import pytest
 import kernels
 
-def test_pyawkward_UnionArray_fillindex_to64_fromU32_1():
+def test_pyawkward_UnionArray_fillindex_to64_from64_1():
     toindex = [123, 123, 123, 123, 123, 123]
     toindexoffset = 3
     fromindex = [1, 0, 0, 1, 1, 1, 0, 0, 1, 0, 1, 0, 1, 1]
     length = 3
-    funcPy = getattr(kernels, 'awkward_UnionArray_fillindex_to64_fromU32')
+    funcPy = getattr(kernels, 'awkward_UnionArray_fillindex_to64_from64')
     funcPy(toindex=toindex, toindexoffset=toindexoffset, fromindex=fromindex, length=length)
     pytest_toindex = [123, 123, 123, 1.0, 0.0, 0.0]
     assert toindex[:len(pytest_toindex)] == pytest.approx(pytest_toindex)
 
-def test_pyawkward_UnionArray_fillindex_to64_fromU32_2():
+def test_pyawkward_UnionArray_fillindex_to64_from64_2():
     toindex = [123, 123, 123, 123, 123, 123]
     toindexoffset = 3
     fromindex = [1, 2, 2, 3, 0, 2, 0, 2, 1, 1]
     length = 3
-    funcPy = getattr(kernels, 'awkward_UnionArray_fillindex_to64_fromU32')
+    funcPy = getattr(kernels, 'awkward_UnionArray_fillindex_to64_from64')
     funcPy(toindex=toindex, toindexoffset=toindexoffset, fromindex=fromindex, length=length)
     pytest_toindex = [123, 123, 123, 1.0, 2.0, 2.0]
     assert toindex[:len(pytest_toindex)] == pytest.approx(pytest_toindex)
 
-def test_pyawkward_UnionArray_fillindex_to64_fromU32_3():
+def test_pyawkward_UnionArray_fillindex_to64_from64_3():
     toindex = [123, 123, 123, 123, 123, 123]
     toindexoffset = 3
     fromindex = [1, 3, 0, 3, 5, 2, 0, 2, 1, 1]
     length = 3
-    funcPy = getattr(kernels, 'awkward_UnionArray_fillindex_to64_fromU32')
+    funcPy = getattr(kernels, 'awkward_UnionArray_fillindex_to64_from64')
     funcPy(toindex=toindex, toindexoffset=toindexoffset, fromindex=fromindex, length=length)
     pytest_toindex = [123, 123, 123, 1.0, 3.0, 0.0]
     assert toindex[:len(pytest_toindex)] == pytest.approx(pytest_toindex)
 
-def test_pyawkward_UnionArray_fillindex_to64_fromU32_4():
+def test_pyawkward_UnionArray_fillindex_to64_from64_4():
     toindex = [123, 123, 123, 123, 123, 123]
     toindexoffset = 3
     fromindex = [1, 4, 2, 3, 1, 2, 3, 1, 4, 3, 2, 1, 3, 2, 4, 5, 1, 2, 3, 4, 5]
     length = 3
-    funcPy = getattr(kernels, 'awkward_UnionArray_fillindex_to64_fromU32')
+    funcPy = getattr(kernels, 'awkward_UnionArray_fillindex_to64_from64')
     funcPy(toindex=toindex, toindexoffset=toindexoffset, fromindex=fromindex, length=length)
     pytest_toindex = [123, 123, 123, 1.0, 4.0, 2.0]
     assert toindex[:len(pytest_toindex)] == pytest.approx(pytest_toindex)
 
-def test_pyawkward_UnionArray_fillindex_to64_fromU32_5():
+def test_pyawkward_UnionArray_fillindex_to64_from64_5():
     toindex = [123, 123, 123, 123, 123, 123]
     toindexoffset = 3
     fromindex = [0, 0, 0, 0, 0, 0, 0, 0, 0, 0]
     length = 3
-    funcPy = getattr(kernels, 'awkward_UnionArray_fillindex_to64_fromU32')
+    funcPy = getattr(kernels, 'awkward_UnionArray_fillindex_to64_from64')
     funcPy(toindex=toindex, toindexoffset=toindexoffset, fromindex=fromindex, length=length)
     pytest_toindex = [123, 123, 123, 0.0, 0.0, 0.0]
     assert toindex[:len(pytest_toindex)] == pytest.approx(pytest_toindex)
```

### Comparing `awkward-cpp-8/tests-spec/test_pyawkward_UnionArray_fillna_from32_to64.py` & `awkward-cpp-9/tests-spec/test_pyawkward_UnionArray_fillna_from32_to64.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# AUTO GENERATED ON 2023-02-03 AT 22:54:31
+# AUTO GENERATED ON 2023-02-16 AT 15:37:39
 # DO NOT EDIT BY HAND!
 #
 # To regenerate file, run
 #
 #     python dev/generate-tests.py
 #
```

### Comparing `awkward-cpp-8/tests-spec/test_pyawkward_UnionArray_fillna_from64_to64.py` & `awkward-cpp-9/tests-spec/test_pyawkward_UnionArray_fillna_from64_to64.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# AUTO GENERATED ON 2023-02-03 AT 22:54:31
+# AUTO GENERATED ON 2023-02-16 AT 15:37:39
 # DO NOT EDIT BY HAND!
 #
 # To regenerate file, run
 #
 #     python dev/generate-tests.py
 #
```

### Comparing `awkward-cpp-8/tests-spec/test_pyawkward_UnionArray_fillna_fromU32_to64.py` & `awkward-cpp-9/tests-spec/test_pyawkward_UnionArray_fillna_fromU32_to64.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# AUTO GENERATED ON 2023-02-03 AT 22:54:31
+# AUTO GENERATED ON 2023-02-16 AT 15:37:39
 # DO NOT EDIT BY HAND!
 #
 # To regenerate file, run
 #
 #     python dev/generate-tests.py
 #
```

### Comparing `awkward-cpp-8/tests-spec/test_pyawkward_UnionArray_filltags_to8_const.py` & `awkward-cpp-9/tests-spec/test_pyawkward_UnionArray_filltags_to8_const.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# AUTO GENERATED ON 2023-02-03 AT 22:54:31
+# AUTO GENERATED ON 2023-02-16 AT 15:37:39
 # DO NOT EDIT BY HAND!
 #
 # To regenerate file, run
 #
 #     python dev/generate-tests.py
 #
```

### Comparing `awkward-cpp-8/tests-spec/test_pyawkward_UnionArray_filltags_to8_from8.py` & `awkward-cpp-9/tests-spec/test_pyawkward_UnionArray_filltags_to8_from8.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# AUTO GENERATED ON 2023-02-03 AT 22:54:31
+# AUTO GENERATED ON 2023-02-16 AT 15:37:39
 # DO NOT EDIT BY HAND!
 #
 # To regenerate file, run
 #
 #     python dev/generate-tests.py
 #
```

### Comparing `awkward-cpp-8/tests-spec/test_pyawkward_index_rpad_and_clip_axis0_64.py` & `awkward-cpp-9/tests-spec/test_pyawkward_index_rpad_and_clip_axis0_64.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# AUTO GENERATED ON 2023-02-03 AT 22:54:31
+# AUTO GENERATED ON 2023-02-16 AT 15:37:39
 # DO NOT EDIT BY HAND!
 #
 # To regenerate file, run
 #
 #     python dev/generate-tests.py
 #
```

### Comparing `awkward-cpp-8/tests-spec/test_pyawkward_index_rpad_and_clip_axis1_64.py` & `awkward-cpp-9/tests-spec/test_pyawkward_index_rpad_and_clip_axis1_64.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# AUTO GENERATED ON 2023-02-03 AT 22:54:31
+# AUTO GENERATED ON 2023-02-16 AT 15:37:39
 # DO NOT EDIT BY HAND!
 #
 # To regenerate file, run
 #
 #     python dev/generate-tests.py
 #
```

### Comparing `awkward-cpp-8/tests-spec/test_pyawkward_missing_repeat_64.py` & `awkward-cpp-9/tests-spec/test_pyawkward_missing_repeat_64.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# AUTO GENERATED ON 2023-02-03 AT 22:54:31
+# AUTO GENERATED ON 2023-02-16 AT 15:37:39
 # DO NOT EDIT BY HAND!
 #
 # To regenerate file, run
 #
 #     python dev/generate-tests.py
 #
```

### Comparing `awkward-cpp-8/tests-spec-explicit/kernels.py` & `awkward-cpp-9/tests-spec-explicit/kernels.py`

 * *Files 1% similar despite different names*

```diff
@@ -245,30 +245,14 @@
             mask_out[i] = i
             k = k + 1
             stops_out[i] = offsets_in[k]
 
 awkward_Content_getitem_next_missing_jagged_getmaskstartstop = awkward_Content_getitem_next_missing_jagged_getmaskstartstop
 
 
-def awkward_Index_iscontiguous(result, fromindex, length):
-    result[0] = True
-    expecting = 0
-    for i in range(length):
-        if fromindex[i] != expecting:
-            result[0] = False
-            return
-        expecting += 1
-
-awkward_Index32_iscontiguous = awkward_Index_iscontiguous
-awkward_Index64_iscontiguous = awkward_Index_iscontiguous
-awkward_Index8_iscontiguous = awkward_Index_iscontiguous
-awkward_IndexU32_iscontiguous = awkward_Index_iscontiguous
-awkward_IndexU8_iscontiguous = awkward_Index_iscontiguous
-
-
 def awkward_IndexedArray_fill(toindex, toindexoffset, fromindex, length, base):
     for i in range(length):
         fromval = fromindex[i]
         toindex[toindexoffset + i] = -1 if fromval < 0 else float(fromval + base)
 
 awkward_IndexedArray_fill_to64_from32 = awkward_IndexedArray_fill
 awkward_IndexedArray_fill_to64_from64 = awkward_IndexedArray_fill
```

### Comparing `awkward-cpp-8/tests-spec-explicit/test_awkward_BitMaskedArray_to_ByteMaskedArray.py` & `awkward-cpp-9/tests-spec-explicit/test_awkward_BitMaskedArray_to_ByteMaskedArray.py`

 * *Files identical despite different names*

### Comparing `awkward-cpp-8/tests-spec-explicit/test_awkward_BitMaskedArray_to_IndexedOptionArray.py` & `awkward-cpp-9/tests-spec-explicit/test_awkward_BitMaskedArray_to_IndexedOptionArray.py`

 * *Files identical despite different names*

### Comparing `awkward-cpp-8/tests-spec-explicit/test_awkward_ByteMaskedArray_getitem_nextcarry.py` & `awkward-cpp-9/tests-spec-explicit/test_awkward_ByteMaskedArray_getitem_nextcarry.py`

 * *Files identical despite different names*

### Comparing `awkward-cpp-8/tests-spec-explicit/test_awkward_ByteMaskedArray_getitem_nextcarry_outindex.py` & `awkward-cpp-9/tests-spec-explicit/test_awkward_ByteMaskedArray_getitem_nextcarry_outindex.py`

 * *Files identical despite different names*

### Comparing `awkward-cpp-8/tests-spec-explicit/test_awkward_ByteMaskedArray_numnull.py` & `awkward-cpp-9/tests-spec-explicit/test_awkward_ByteMaskedArray_numnull.py`

 * *Files identical despite different names*

### Comparing `awkward-cpp-8/tests-spec-explicit/test_awkward_ByteMaskedArray_toIndexedOptionArray.py` & `awkward-cpp-9/tests-spec-explicit/test_awkward_ByteMaskedArray_toIndexedOptionArray.py`

 * *Files identical despite different names*

### Comparing `awkward-cpp-8/tests-spec-explicit/test_awkward_Content_getitem_next_missing_jagged_getmaskstartstop.py` & `awkward-cpp-9/tests-spec-explicit/test_awkward_Content_getitem_next_missing_jagged_getmaskstartstop.py`

 * *Files identical despite different names*

### Comparing `awkward-cpp-8/tests-spec-explicit/test_awkward_IndexedArray_fill.py` & `awkward-cpp-9/tests-spec-explicit/test_awkward_IndexedArray_fill.py`

 * *Files identical despite different names*

### Comparing `awkward-cpp-8/tests-spec-explicit/test_awkward_IndexedArray_flatten_none2empty.py` & `awkward-cpp-9/tests-spec-explicit/test_awkward_IndexedArray_flatten_none2empty.py`

 * *Files identical despite different names*

### Comparing `awkward-cpp-8/tests-spec-explicit/test_awkward_IndexedArray_getitem_nextcarry.py` & `awkward-cpp-9/tests-spec-explicit/test_awkward_IndexedArray_getitem_nextcarry.py`

 * *Files identical despite different names*

### Comparing `awkward-cpp-8/tests-spec-explicit/test_awkward_IndexedArray_getitem_nextcarry_outindex.py` & `awkward-cpp-9/tests-spec-explicit/test_awkward_IndexedArray_getitem_nextcarry_outindex.py`

 * *Files identical despite different names*

### Comparing `awkward-cpp-8/tests-spec-explicit/test_awkward_IndexedArray_index_of_nulls.py` & `awkward-cpp-9/tests-spec-explicit/test_awkward_IndexedArray_index_of_nulls.py`

 * *Files identical despite different names*

### Comparing `awkward-cpp-8/tests-spec-explicit/test_awkward_IndexedArray_numnull.py` & `awkward-cpp-9/tests-spec-explicit/test_awkward_IndexedArray_numnull.py`

 * *Files identical despite different names*

### Comparing `awkward-cpp-8/tests-spec-explicit/test_awkward_IndexedArray_reduce_next_64.py` & `awkward-cpp-9/tests-spec-explicit/test_awkward_IndexedArray_reduce_next_64.py`

 * *Files identical despite different names*

### Comparing `awkward-cpp-8/tests-spec-explicit/test_awkward_IndexedArray_reduce_next_fix_offsets_64.py` & `awkward-cpp-9/tests-spec-explicit/test_awkward_IndexedArray_reduce_next_fix_offsets_64.py`

 * *Files identical despite different names*

### Comparing `awkward-cpp-8/tests-spec-explicit/test_awkward_IndexedArray_reduce_next_nonlocal_nextshifts_64.py` & `awkward-cpp-9/tests-spec-explicit/test_awkward_IndexedArray_reduce_next_nonlocal_nextshifts_64.py`

 * *Files identical despite different names*

### Comparing `awkward-cpp-8/tests-spec-explicit/test_awkward_IndexedArray_reduce_next_nonlocal_nextshifts_fromshifts_64.py` & `awkward-cpp-9/tests-spec-explicit/test_awkward_IndexedArray_reduce_next_nonlocal_nextshifts_fromshifts_64.py`

 * *Files identical despite different names*

### Comparing `awkward-cpp-8/tests-spec-explicit/test_awkward_IndexedArray_simplify.py` & `awkward-cpp-9/tests-spec-explicit/test_awkward_IndexedArray_simplify.py`

 * *Files identical despite different names*

### Comparing `awkward-cpp-8/tests-spec-explicit/test_awkward_IndexedArray_validity.py` & `awkward-cpp-9/tests-spec-explicit/test_awkward_IndexedArray_validity.py`

 * *Files identical despite different names*

### Comparing `awkward-cpp-8/tests-spec-explicit/test_awkward_ListArray_broadcast_tooffsets.py` & `awkward-cpp-9/tests-spec-explicit/test_awkward_ListArray_broadcast_tooffsets.py`

 * *Files identical despite different names*

### Comparing `awkward-cpp-8/tests-spec-explicit/test_awkward_ListArray_combinations_length.py` & `awkward-cpp-9/tests-spec-explicit/test_awkward_ListArray_combinations_length.py`

 * *Files identical despite different names*

### Comparing `awkward-cpp-8/tests-spec-explicit/test_awkward_ListArray_compact_offsets.py` & `awkward-cpp-9/tests-spec-explicit/test_awkward_ListArray_compact_offsets.py`

 * *Files identical despite different names*

### Comparing `awkward-cpp-8/tests-spec-explicit/test_awkward_ListArray_fill.py` & `awkward-cpp-9/tests-spec-explicit/test_awkward_ListArray_fill.py`

 * *Files identical despite different names*

### Comparing `awkward-cpp-8/tests-spec-explicit/test_awkward_ListArray_getitem_jagged_apply.py` & `awkward-cpp-9/tests-spec-explicit/test_awkward_ListArray_getitem_jagged_apply.py`

 * *Files identical despite different names*

### Comparing `awkward-cpp-8/tests-spec-explicit/test_awkward_ListArray_getitem_jagged_carrylen.py` & `awkward-cpp-9/tests-spec-explicit/test_awkward_ListArray_getitem_jagged_carrylen.py`

 * *Files identical despite different names*

### Comparing `awkward-cpp-8/tests-spec-explicit/test_awkward_ListArray_getitem_jagged_descend.py` & `awkward-cpp-9/tests-spec-explicit/test_awkward_ListArray_getitem_jagged_descend.py`

 * *Files identical despite different names*

### Comparing `awkward-cpp-8/tests-spec-explicit/test_awkward_ListArray_getitem_jagged_expand.py` & `awkward-cpp-9/tests-spec-explicit/test_awkward_ListArray_getitem_jagged_expand.py`

 * *Files identical despite different names*

### Comparing `awkward-cpp-8/tests-spec-explicit/test_awkward_ListArray_getitem_jagged_shrink.py` & `awkward-cpp-9/tests-spec-explicit/test_awkward_ListArray_getitem_jagged_shrink.py`

 * *Files identical despite different names*

### Comparing `awkward-cpp-8/tests-spec-explicit/test_awkward_ListArray_getitem_next_array.py` & `awkward-cpp-9/tests-spec-explicit/test_awkward_ListArray_getitem_next_array.py`

 * *Files identical despite different names*

### Comparing `awkward-cpp-8/tests-spec-explicit/test_awkward_ListArray_getitem_next_array_advanced.py` & `awkward-cpp-9/tests-spec-explicit/test_awkward_ListArray_getitem_next_array_advanced.py`

 * *Files identical despite different names*

### Comparing `awkward-cpp-8/tests-spec-explicit/test_awkward_ListArray_getitem_next_at.py` & `awkward-cpp-9/tests-spec-explicit/test_awkward_ListArray_getitem_next_at.py`

 * *Files identical despite different names*

### Comparing `awkward-cpp-8/tests-spec-explicit/test_awkward_ListArray_getitem_next_range_counts.py` & `awkward-cpp-9/tests-spec-explicit/test_awkward_ListArray_getitem_next_range_counts.py`

 * *Files identical despite different names*

### Comparing `awkward-cpp-8/tests-spec-explicit/test_awkward_ListArray_localindex.py` & `awkward-cpp-9/tests-spec-explicit/test_awkward_ListArray_localindex.py`

 * *Files identical despite different names*

### Comparing `awkward-cpp-8/tests-spec-explicit/test_awkward_ListArray_min_range.py` & `awkward-cpp-9/tests-spec-explicit/test_awkward_ListArray_min_range.py`

 * *Files identical despite different names*

### Comparing `awkward-cpp-8/tests-spec-explicit/test_awkward_ListArray_rpad_and_clip_length_axis1.py` & `awkward-cpp-9/tests-spec-explicit/test_awkward_ListArray_rpad_and_clip_length_axis1.py`

 * *Files identical despite different names*

### Comparing `awkward-cpp-8/tests-spec-explicit/test_awkward_ListArray_rpad_axis1.py` & `awkward-cpp-9/tests-spec-explicit/test_awkward_ListArray_rpad_axis1.py`

 * *Files identical despite different names*

### Comparing `awkward-cpp-8/tests-spec-explicit/test_awkward_ListArray_validity.py` & `awkward-cpp-9/tests-spec-explicit/test_awkward_ListArray_validity.py`

 * *Files identical despite different names*

### Comparing `awkward-cpp-8/tests-spec-explicit/test_awkward_ListOffsetArray_compact_offsets.py` & `awkward-cpp-9/tests-spec-explicit/test_awkward_ListOffsetArray_compact_offsets.py`

 * *Files identical despite different names*

### Comparing `awkward-cpp-8/tests-spec-explicit/test_awkward_ListOffsetArray_flatten_offsets.py` & `awkward-cpp-9/tests-spec-explicit/test_awkward_ListOffsetArray_flatten_offsets.py`

 * *Files identical despite different names*

### Comparing `awkward-cpp-8/tests-spec-explicit/test_awkward_ListOffsetArray_reduce_local_outoffsets_64.py` & `awkward-cpp-9/tests-spec-explicit/test_awkward_ListOffsetArray_reduce_local_outoffsets_64.py`

 * *Files identical despite different names*

### Comparing `awkward-cpp-8/tests-spec-explicit/test_awkward_ListOffsetArray_reduce_nonlocal_maxcount_offsetscopy_64.py` & `awkward-cpp-9/tests-spec-explicit/test_awkward_ListOffsetArray_reduce_nonlocal_maxcount_offsetscopy_64.py`

 * *Files identical despite different names*

### Comparing `awkward-cpp-8/tests-spec-explicit/test_awkward_ListOffsetArray_reduce_nonlocal_nextshifts_64.py` & `awkward-cpp-9/tests-spec-explicit/test_awkward_ListOffsetArray_reduce_nonlocal_nextshifts_64.py`

 * *Files identical despite different names*

### Comparing `awkward-cpp-8/tests-spec-explicit/test_awkward_ListOffsetArray_reduce_nonlocal_nextstarts_64.py` & `awkward-cpp-9/tests-spec-explicit/test_awkward_ListOffsetArray_reduce_nonlocal_nextstarts_64.py`

 * *Files identical despite different names*

### Comparing `awkward-cpp-8/tests-spec-explicit/test_awkward_ListOffsetArray_reduce_nonlocal_outstartsstops_64.py` & `awkward-cpp-9/tests-spec-explicit/test_awkward_ListOffsetArray_reduce_nonlocal_outstartsstops_64.py`

 * *Files identical despite different names*

### Comparing `awkward-cpp-8/tests-spec-explicit/test_awkward_ListOffsetArray_toRegularArray.py` & `awkward-cpp-9/tests-spec-explicit/test_awkward_ListOffsetArray_toRegularArray.py`

 * *Files identical despite different names*

### Comparing `awkward-cpp-8/tests-spec-explicit/test_awkward_MaskedArray_getitem_next_jagged_project.py` & `awkward-cpp-9/tests-spec-explicit/test_awkward_MaskedArray_getitem_next_jagged_project.py`

 * *Files identical despite different names*

### Comparing `awkward-cpp-8/tests-spec-explicit/test_awkward_NumpyArray_reduce_mask_ByteMaskedArray_64.py` & `awkward-cpp-9/tests-spec-explicit/test_awkward_NumpyArray_reduce_mask_ByteMaskedArray_64.py`

 * *Files identical despite different names*

### Comparing `awkward-cpp-8/tests-spec-explicit/test_awkward_RegularArray_broadcast_tooffsets.py` & `awkward-cpp-9/tests-spec-explicit/test_awkward_RegularArray_broadcast_tooffsets.py`

 * *Files identical despite different names*

### Comparing `awkward-cpp-8/tests-spec-explicit/test_awkward_RegularArray_broadcast_tooffsets_size1.py` & `awkward-cpp-9/tests-spec-explicit/test_awkward_RegularArray_broadcast_tooffsets_size1.py`

 * *Files identical despite different names*

### Comparing `awkward-cpp-8/tests-spec-explicit/test_awkward_RegularArray_compact_offsets.py` & `awkward-cpp-9/tests-spec-explicit/test_awkward_RegularArray_compact_offsets.py`

 * *Files identical despite different names*

### Comparing `awkward-cpp-8/tests-spec-explicit/test_awkward_RegularArray_getitem_carry.py` & `awkward-cpp-9/tests-spec-explicit/test_awkward_RegularArray_getitem_carry.py`

 * *Files identical despite different names*

### Comparing `awkward-cpp-8/tests-spec-explicit/test_awkward_RegularArray_getitem_jagged_expand.py` & `awkward-cpp-9/tests-spec-explicit/test_awkward_RegularArray_getitem_jagged_expand.py`

 * *Files identical despite different names*

### Comparing `awkward-cpp-8/tests-spec-explicit/test_awkward_RegularArray_getitem_next_array.py` & `awkward-cpp-9/tests-spec-explicit/test_awkward_RegularArray_getitem_next_array.py`

 * *Files identical despite different names*

### Comparing `awkward-cpp-8/tests-spec-explicit/test_awkward_RegularArray_getitem_next_array_advanced.py` & `awkward-cpp-9/tests-spec-explicit/test_awkward_RegularArray_getitem_next_array_advanced.py`

 * *Files identical despite different names*

### Comparing `awkward-cpp-8/tests-spec-explicit/test_awkward_RegularArray_getitem_next_array_regularize.py` & `awkward-cpp-9/tests-spec-explicit/test_awkward_RegularArray_getitem_next_array_regularize.py`

 * *Files identical despite different names*

### Comparing `awkward-cpp-8/tests-spec-explicit/test_awkward_RegularArray_getitem_next_at.py` & `awkward-cpp-9/tests-spec-explicit/test_awkward_RegularArray_getitem_next_at.py`

 * *Files identical despite different names*

### Comparing `awkward-cpp-8/tests-spec-explicit/test_awkward_RegularArray_getitem_next_range.py` & `awkward-cpp-9/tests-spec-explicit/test_awkward_RegularArray_getitem_next_range.py`

 * *Files identical despite different names*

### Comparing `awkward-cpp-8/tests-spec-explicit/test_awkward_RegularArray_getitem_next_range_spreadadvanced.py` & `awkward-cpp-9/tests-spec-explicit/test_awkward_RegularArray_getitem_next_range_spreadadvanced.py`

 * *Files identical despite different names*

### Comparing `awkward-cpp-8/tests-spec-explicit/test_awkward_RegularArray_localindex.py` & `awkward-cpp-9/tests-spec-explicit/test_awkward_RegularArray_localindex.py`

 * *Files identical despite different names*

### Comparing `awkward-cpp-8/tests-spec-explicit/test_awkward_RegularArray_rpad_and_clip_axis1.py` & `awkward-cpp-9/tests-spec-explicit/test_awkward_RegularArray_rpad_and_clip_axis1.py`

 * *Files identical despite different names*

### Comparing `awkward-cpp-8/tests-spec-explicit/test_awkward_UnionArray_fillindex.py` & `awkward-cpp-9/tests-spec-explicit/test_awkward_UnionArray_fillindex.py`

 * *Files identical despite different names*

### Comparing `awkward-cpp-8/tests-spec-explicit/test_awkward_UnionArray_fillindex_count.py` & `awkward-cpp-9/tests-spec-explicit/test_awkward_UnionArray_fillindex_count.py`

 * *Files identical despite different names*

### Comparing `awkward-cpp-8/tests-spec-explicit/test_awkward_UnionArray_fillna.py` & `awkward-cpp-9/tests-spec-explicit/test_awkward_UnionArray_fillna.py`

 * *Files identical despite different names*

### Comparing `awkward-cpp-8/tests-spec-explicit/test_awkward_UnionArray_project.py` & `awkward-cpp-9/tests-spec-explicit/test_awkward_UnionArray_project.py`

 * *Files identical despite different names*

### Comparing `awkward-cpp-8/tests-spec-explicit/test_awkward_UnionArray_regular_index.py` & `awkward-cpp-9/tests-spec-explicit/test_awkward_UnionArray_regular_index.py`

 * *Files identical despite different names*

### Comparing `awkward-cpp-8/tests-spec-explicit/test_awkward_UnionArray_regular_index_getsize.py` & `awkward-cpp-9/tests-spec-explicit/test_awkward_UnionArray_regular_index_getsize.py`

 * *Files identical despite different names*

### Comparing `awkward-cpp-8/tests-spec-explicit/test_awkward_UnionArray_simplify.py` & `awkward-cpp-9/tests-spec-explicit/test_awkward_UnionArray_simplify.py`

 * *Files identical despite different names*

### Comparing `awkward-cpp-8/tests-spec-explicit/test_awkward_UnionArray_simplify_one.py` & `awkward-cpp-9/tests-spec-explicit/test_awkward_UnionArray_simplify_one.py`

 * *Files identical despite different names*

### Comparing `awkward-cpp-8/tests-spec-explicit/test_awkward_UnionArray_validity.py` & `awkward-cpp-9/tests-spec-explicit/test_awkward_UnionArray_validity.py`

 * *Files identical despite different names*

### Comparing `awkward-cpp-8/tests-spec-explicit/test_awkward_index_rpad_and_clip_axis0.py` & `awkward-cpp-9/tests-spec-explicit/test_awkward_index_rpad_and_clip_axis0.py`

 * *Files identical despite different names*

### Comparing `awkward-cpp-8/tests-spec-explicit/test_awkward_index_rpad_and_clip_axis1.py` & `awkward-cpp-9/tests-spec-explicit/test_awkward_index_rpad_and_clip_axis1.py`

 * *Files identical despite different names*

### Comparing `awkward-cpp-8/tests-spec-explicit/test_awkward_localindex.py` & `awkward-cpp-9/tests-spec-explicit/test_awkward_localindex.py`

 * *Files identical despite different names*

### Comparing `awkward-cpp-8/tests-spec-explicit/test_awkward_missing_repeat.py` & `awkward-cpp-9/tests-spec-explicit/test_awkward_missing_repeat.py`

 * *Files identical despite different names*

### Comparing `awkward-cpp-8/tests-spec-explicit/test_awkward_reduce_argmax.py` & `awkward-cpp-9/tests-spec-explicit/test_awkward_reduce_argmax.py`

 * *Files identical despite different names*

### Comparing `awkward-cpp-8/tests-spec-explicit/test_awkward_reduce_argmin.py` & `awkward-cpp-9/tests-spec-explicit/test_awkward_reduce_argmin.py`

 * *Files identical despite different names*

### Comparing `awkward-cpp-8/tests-spec-explicit/test_awkward_reduce_count_64.py` & `awkward-cpp-9/tests-spec-explicit/test_awkward_reduce_count_64.py`

 * *Files identical despite different names*

### Comparing `awkward-cpp-8/tests-spec-explicit/test_awkward_reduce_countnonzero.py` & `awkward-cpp-9/tests-spec-explicit/test_awkward_reduce_countnonzero.py`

 * *Files identical despite different names*

### Comparing `awkward-cpp-8/tests-spec-explicit/test_awkward_reduce_max.py` & `awkward-cpp-9/tests-spec-explicit/test_awkward_reduce_max.py`

 * *Files identical despite different names*

### Comparing `awkward-cpp-8/tests-spec-explicit/test_awkward_reduce_min.py` & `awkward-cpp-9/tests-spec-explicit/test_awkward_reduce_min.py`

 * *Files identical despite different names*

### Comparing `awkward-cpp-8/tests-spec-explicit/test_awkward_reduce_prod.py` & `awkward-cpp-9/tests-spec-explicit/test_awkward_reduce_prod.py`

 * *Files identical despite different names*

### Comparing `awkward-cpp-8/tests-spec-explicit/test_awkward_reduce_prod_bool.py` & `awkward-cpp-9/tests-spec-explicit/test_awkward_reduce_prod_bool.py`

 * *Files identical despite different names*

### Comparing `awkward-cpp-8/tests-spec-explicit/test_awkward_reduce_sum.py` & `awkward-cpp-9/tests-spec-explicit/test_awkward_reduce_sum.py`

 * *Files identical despite different names*

### Comparing `awkward-cpp-8/tests-spec-explicit/test_awkward_reduce_sum_bool.py` & `awkward-cpp-9/tests-spec-explicit/test_awkward_reduce_sum_bool.py`

 * *Files identical despite different names*

### Comparing `awkward-cpp-8/PKG-INFO` & `awkward-cpp-9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: awkward-cpp
-Version: 8
+Version: 9
 Summary: CPU kernels and compiled extensions for Awkward Array
 Author-Email: Jim Pivarski <pivarski@princeton.edu>
 Maintainer-Email: Scikit-HEP <scikit-hep-admins@googlegroups.com>
 License: BSD-3-Clause
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Information Technology
```

