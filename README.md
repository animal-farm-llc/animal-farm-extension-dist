# Animal Farm Extension Distribution

Packaged releases of the Animal Farm Chrome Extension for enterprise deployment.

## Why this repo exists

This repo is **public** so that Chrome's enterprise auto-update mechanism can access the `updates.xml` manifest and `.crx` package without authentication. It contains only the packaged extension — no source code, configuration, or secrets.

The source code lives in the internal repo: [`animal-farm-llc/animal-farm-extension`](https://github.com/animal-farm-llc/animal-farm-extension) (org members only).

## Enterprise Installation

IT administrators can force-install the extension via Chrome enterprise policy:

- **Extension ID:** `pbefpjkeelhdhloeaehmpegmmmjacnec`
- **Update URL:** `https://raw.githubusercontent.com/animal-farm-llc/animal-farm-extension-dist/main/updates.xml`

In Google Admin Console: **Devices → Chrome → Apps & Extensions → Users & browsers → Add by ID → From a custom URL → Force install**.

Chrome will automatically download and install the extension, and check for updates every few hours.

## Contents

- `updates.xml` — Chrome auto-update manifest pointing to the latest `.crx` release
- GitHub Releases — Packaged `.crx` files for each version
