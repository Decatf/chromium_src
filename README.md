# Building Chromium for Tegra 2 devices on Android

## Replicating this build

 * Follow the [Android Build Instructions](https://chromium.googlesource.com/chromium/src/+/65.0.3325.109/docs/android_build_instructions.md) to configure a build environment.
 * Fetch Chromium m65.
 e.g.
```
git fetch origin refs/tags/65.0.3325.109
```
 * Apply the patches from this repo.
 * Disable arm neon with the following gn flags:
```
arm_use_neon = false
arm_optionally_use_neon = false
```
 * Build and install the APKs.
