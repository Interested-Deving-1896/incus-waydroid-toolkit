[update-readmes]   Mode: rewrite — migrating to template structure...
# waydroid-toolkit

[![Built with Ona](https://ona.com/build-with-ona.svg)](https://app.ona.com/#https://github.com/Interested-Deving-1896/waydroid-toolkit)

<!-- AI:start:what-it-does -->
_Description pending._
<!-- AI:end:what-it-does -->

## Architecture

<!-- AI:start:architecture -->
_Architecture documentation pending._
<!-- AI:end:architecture -->

## Install

<!-- Add installation instructions here. This section is yours — the AI will not modify it. -->

```bash
git clone https://github.com/Interested-Deving-1896/waydroid-toolkit.git
cd waydroid-toolkit
```

## Usage


### CLI

```bash
wdt status                            # show runtime state
wdt install --image-type GAPPS        # install Waydroid with GApps image
wdt extensions list                   # list available extensions
wdt extensions install libhoudini     # install ARM translation
wdt extensions install magisk         # install Magisk
wdt images list                       # list image profiles
wdt images switch androidtv           # switch to Android TV profile
wdt packages install /path/to/app.apk
wdt packages repo add fdroid https://f-droid.org/repo
wdt backup create
wdt backup restore waydroid_backup_20240101_120000.tar.gz
wdt performance apply --zram-size 8192 --governor performance
wdt maintenance screenshot
wdt maintenance logcat --errors
wdt maintenance debloat
```

### GUI

```bash
waydroid-toolkit
```

## Configuration

<!-- Document configuration options here. This section is yours — the AI will not modify it. -->

## CI

<!-- AI:start:ci -->
The repository uses GitHub Actions for continuous integration. The following workflows are defined:

1. **integration.yml**  
   - Runs unit tests and integration tests using `pytest` with coverage reporting.  
   - Requires Python 3.11.  
   - No secrets are required.

2. **mirror-osp-to-ooc.yaml**  
   - Mirrors the repository from the "open-source project" (OSP) to an "out-of-core" (OOC) repository.  
   - Requires the following secrets:  
     - `OOC_REPO_URL`: URL of the target repository.  
     - `OOC_REPO_TOKEN`: Personal access token for authentication.  

Workflows are triggered on push and pull request events.
<!-- AI:end:ci -->

## Mirror chain

<!-- AI:start:mirror-chain -->
This repo is maintained in [`Interested-Deving-1896/incus-waydroid-toolkit`](https://github.com/Interested-Deving-1896/incus-waydroid-toolkit) and mirrored through:

```
Interested-Deving-1896/incus-waydroid-toolkit  ──►  OpenOS-Project-OSP/incus-waydroid-toolkit  ──►  OpenOS-Project-Ecosystem-OOC/incus-waydroid-toolkit
```

Changes flow downstream automatically via the hourly mirror chain in
[`fork-sync-all`](https://github.com/Interested-Deving-1896/fork-sync-all).
Direct commits to OSP or OOC are detected and opened as PRs back to `Interested-Deving-1896`.
<!-- AI:end:mirror-chain -->

## Contributors

<!-- AI:start:contributors -->
- [@Interested-Deving-1896](https://github.com/Interested-Deving-1896): 50 commits  
- [@ona-agent](https://github.com/ona-agent): 5 commits  

*Note: This repository may be a mirror. Please check the upstream source for additional details.*
<!-- AI:end:contributors -->

## Origins

<!-- AI:start:origins -->

Original project — unified management suite for Waydroid (Android in a Linux container).

| Origin | Host | Fork in I-D-1896 |
|--------|------|-----------------|
| [waydroid/waydroid](https://github.com/waydroid/waydroid) | GitHub | ✅ |
<!-- AI:end:origins -->

## Resources

<!-- AI:start:resources -->
| File | Description |
|---|---|
| [dep-graph/origins.md](https://github.com/Interested-Deving-1896/incus-waydroid-toolkit/blob/main/dep-graph/origins.md) | Dependency graph (Markdown table) |
<!-- AI:end:resources -->

## License

<!-- AI:start:license -->
<!-- License not detected — add a LICENSE file to this repo. -->
<!-- AI:end:license -->
