# ReaPackLabSetup

**ReaPackLabSetup** is the planned lightweight bootstrap and repair companion for [ReaPackLab](https://github.com/rockumk/ReaPackLab), the centrally managed REAPER package manager.

## Intended responsibility

- Bootstrap an approved ReaPackLab installation.
- Detect whether ReaPackLab is missing or requires repair.
- Coordinate safe replacement of native extensions while REAPER is **not** running.
- Retire the original ReaPack extension without deleting unrelated scripts, plugin packages, or legacy registry records.
- Avoid requiring students to enter administrator or GitHub credentials.

ReaPackLab and ReaPackLabSetup are **separate extensions** with separate release packages. ReaPackLabSetup is a recovery/bootstrap component, not the full package manager.

## Current status

**Repository initialized; no production-ready Setup release has been published here.**

Prototype source lives in the private development repository ReaPackLabDev. It is not yet a complete installation/repair implementation. In particular, the bootstrap must be built and tested before it can consume any pending retirement/repair instructions issued by ReaPackLab.

The full ReaPackLab binary is distributed through [ReaPackLab Releases](https://github.com/rockumk/ReaPackLab/releases).

## Release packaging

The future macOS Apple Silicon Setup binary is intended to be named:

`reaper_reapacklabsetup-arm64.dylib`

Release assets will be attached to versioned GitHub Releases and indexed with ReaPack metadata in this repository, after the binary performs actual verified installation and recovery. Do **not** import this repository into classroom REAPER installations until a Setup package and corresponding release have been published and verified.

Based on the ReaPack project by Christian Fillion (LGPL-3.0-or-later).
