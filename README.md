# QuickCook — Releases

Public distribution point for **QuickCook** (Windows). This repository carries **no source
code** — only release installers and the version manifest the app's updater and the unified
installer read.

## Download

Grab the latest **QuickCookSetup.exe** from the [Releases](../../releases) page. The installer
lets you pick any stable version and (behind an opt-in "beta" toggle) any pre-release.

## Release tiers

| Tier | Meaning |
|------|---------|
| **latest** | current stable build — the default |
| **outdated** | superseded stable builds, kept for reinstalls |
| **pre-release** | betas / previews — hidden unless you opt in |

## `versions.json`

Machine-readable manifest, attached to the `latest` release and updated on every publish.
Newest first. Each entry:

```jsonc
{
  "version": "0.1.0",
  "channel": "stable | beta",
  "date": "2026-09-01",
  "installer": "QuickCookSetup0.1.0.exe",
  "url": "https://github.com/.../releases/download/v0.1/QuickCookSetup0.1.0.exe",
  "sha256": "...",
  "notes": "short changelog"
}
```

---
© Smith Media Industries inc.
