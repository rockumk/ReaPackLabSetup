# ReaPackLabSetup

**ReaPackLabSetup** is the separate bootstrap companion for [ReaPackLab](https://github.com/rockumk/ReaPackLab), the centrally managed REAPER package manager. It is not the full package manager.

**Current stable release: [v0.1.1](https://github.com/rockumk/ReaPackLabSetup/releases/tag/v0.1.1)** — macOS 15.0 or later, Apple Silicon (ARM64). The binary embeds version **0.1.1** and is Developer ID Application signed, securely timestamped, and built with hardened runtime.

## Repository / installation

ReaPack repository index URL:

```text
https://raw.githubusercontent.com/rockumk/ReaPackLabSetup/master/index.xml
```

The native asset is named `reaper_reapacklabsetup-arm64.dylib` and is packaged through `Extensions/ReaPackLabSetup.ext`. Restart REAPER after installing native extensions or after Setup installs the main extension. The full managed extension is distributed separately through [ReaPackLab Releases](https://github.com/rockumk/ReaPackLab/releases).

## Security and scope

**Signed, not notarized.** Apple notarization and Gatekeeper acceptance have not been established; macOS security warnings may still occur. Test actual bootstrap, installation and recovery behavior in an isolated REAPER resource directory before classroom deployment. Publishing this signed build is not a claim that every planned repair/retirement workflow is implemented or validated.

The release includes the dylib, `ReaPackLabSetup-SHA256SUMS.txt`, and `ReaPackLabSetup-provenance.json`, identifying the final signed bytes and build provenance. Existing releases are unchanged. Other platforms are not listed in this distribution.

ReaPackLab and ReaPackLabSetup are independently versioned extensions with separate release packages and feeds. Package metadata is updated only after release assets have been downloaded and verified; `reapack-index` then generates the index while retaining historical versions. Generated package entries are not hand-edited.

Development source is maintained in the access-restricted ReaPackLabDev repository. Automatic source archives of this distribution repository contain packaging metadata, not that development source.

Based on the ReaPack project by Christian Fillion (LGPL-3.0-or-later).
