# libSceIcu

## add Functional

- [ucnv_countAliases](../../../core/libs/prx/libSceIcu/ConverterAliases.cpp) has no console ABI or behavior verification. It returns the count and status from bundled ICU 78.1 [ucnv_io.cpp](https://github.com/unicode-org/icu/blob/049e0d6a420629ac7db77256987d083a563287b5/icu4c/source/common/ucnv_io.cpp). Inaccessible required guest memory throws `std::invalid_argument`. The reduced data package omits `cnvalias.icu`, so queries report ICU's data-loading error unless compatible common data is supplied before alias initialization.
