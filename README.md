# Building Chromium for Tegra 2 devices on Android

## Replicating this build

 * Follow the [Android Build Instructions](https://chromium.googlesource.com/chromium/src/+/56.0.2924.92/docs/android_build_instructions.md) to configure a build environment.
 * Fetch Chromium m56.
 e.g.
```
git fetch origin refs/tags/56.0.2924.87
```
 * Apply the patches from this repo.
 * Disable arm neon with the following gn flags:
```
arm_use_neon = false
arm_optionally_use_neon = false
```
 * Build and install the APKs.
