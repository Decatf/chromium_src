# Building Chromium for Tegra 2 devices on Android

## Replicating this build

 * Follow the [Android Build Instructions](https://chromium.googlesource.com/chromium/src/+/59.0.3071.92/docs/android_build_instructions.md) to configure a build environment.
 * Fetch Chromium m59.
 e.g.
```
git fetch origin refs/tags/59.0.3071.92
```
 * Apply the patches from this repo.
 * Disable arm neon with the following gn flags:
```
arm_use_neon = false
arm_optionally_use_neon = false
```
 * Build and install the APKs.
