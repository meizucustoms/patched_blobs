# goodix

Flyme 8.0.5.0A fingerprint stack, 
patched to be working in Android R.

## STILL NEEDS MORE PATCHING
Parcel size wasn't patched to 120 bytes and 
libc is throwing stack errors.

## Already done
Removed missing dependencies:
* libbacktrace
* libunwind
* libkeystore_binder
* libprotobuf-cpp-lite
* libsoftkeymaster
* libkeymaster1

Added libbinder_shim to goodixfingerprintd,
because it hasn't found symbol
`_ZN7android15PermissionCache15checkPermissionERKNS_8String16Eij`,
referrenced by libbinder.