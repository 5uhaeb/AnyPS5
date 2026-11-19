# libSceIcu

## add Functional

- [ucnv_flushCache](../../../core/libs/prx/libSceIcu/ConverterAliases.cpp) follows bundled ICU 78.1's [converter cache](https://github.com/unicode-org/icu/blob/049e0d6a420629ac7db77256987d083a563287b5/icu4c/source/common/ucnv_bld.cpp), which retains converters used by the backend; the console's cache contents and behavior have not been measured.
