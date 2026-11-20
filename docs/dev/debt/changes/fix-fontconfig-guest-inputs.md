# libfontconfig

## change [Faulting arguments]

- [Faulting arguments](../../../core/libs/prx/libfontconfig/Objects.cpp) are not delivered as console signals. `FcLangSetAdd`, `FcLangSetHasLang`, the seven typed `FcPatternAdd*` exports and `FcPatternReference` report undefined null arguments and unreadable string or matrix inputs as host runtime errors, following the pinned Fontconfig 2.15.0 source. Other unsupported paths retain `NotImplemented_nid_no_patch`. `FcPatternDestroy(nullptr)` still does nothing where the firmware 13.42 review cited above reports a dereference at `0x7e0`. Foreign, stale and unreadable opaque handles remain unsupported; console fault behavior and allocation failures are unverified.
