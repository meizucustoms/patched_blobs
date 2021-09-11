# goodix

Flyme 8.0.5.0A fingerprint stack, 
patched to be working in Android R.

Thanks to @h2o64 for help with that.

## If you see some bugs
libgf_hal still needs Parcel resize patch.

## What's done
Removed missing dependencies:
* libbacktrace
* libunwind
* libkeystore_binder
* libprotobuf-cpp-lite
* libsoftkeymaster
* libkeymaster1

Recompiled from leaked BSP on Android R:
* libgoodixfingerprintd_binder
* fingerprint.msm8953
* goodixfingerprintd
