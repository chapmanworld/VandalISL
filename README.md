# VandalISL

**VandalISL** is a pinned fork of the [ISL (Integer Set Library)](https://libisl.sourceforge.io/), used as a build-time dependency of GDB in the **VandalSDK** toolchain (see `VandalBinUtils`).

This is **not Vandal-authored code**. It is a fork of an existing, independently maintained open-source project, imported here purely so that a specific, known-good version can be built reproducibly as part of the VandalSDK toolchain used by the **Vandalism Engine** game engine.

## Baseline

See `VANDALISL_BASELINE.txt` for the exact upstream version, tag, and repository this fork was taken from.

## Why this repository exists

VandalSDK's packaged debugger (GDB) links against ISL, built on top of GMP. Pinning a specific ISL release as its own repository, alongside the other GDB build dependencies (`VandalGMP`, `VandalMPFR`, `VandalMPC`), gives the SDK toolchain build a reproducible, independently versioned source for each dependency, separate from upstream's own release cadence.

This repository exists for internal use while building Vandalism Engine and its SDK. It is not a general-purpose ISL distribution.

## Contributions and issue tracking

This is **not a maintained fork**. ChapmanWorld is not accepting contributions here, and this repository is not the place to raise issues, ask questions, or request features.

* Please do not use this repository as an ISL support forum.
* Please do not raise issues here for upstream ISL bugs.
* Please do not use this repository to report Vandal Engine or VandalSDK bugs.
* Issues with ISL itself should be raised with the upstream ISL project.

## Licensing

ISL is distributed under the **MIT license**. See `LICENSE` in this repository for the authoritative upstream license terms.

## Status

Toolchain dependency fork. Tracks a single pinned upstream release for VandalSDK build reproducibility.
