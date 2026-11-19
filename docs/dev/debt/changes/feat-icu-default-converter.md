# libSceIcu

## add Functional

- [ucnv_getDefaultName and ucnv_setDefaultName](../../../core/libs/prx/libSceIcu/ConverterAliases.cpp) use the bundled ICU 78.1 [default converter](https://github.com/unicode-org/icu/blob/049e0d6a420629ac7db77256987d083a563287b5/icu4c/source/common/ucnv_bld.cpp); its initial value follows the host codepage and may differ from the console. Returned names are owned by ICU. An inaccessible name throws `std::invalid_argument`. The console's signature and behavior are unverified.
