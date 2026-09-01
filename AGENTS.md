# Repository Guidelines

## Project Structure & Module Organization

This repository contains Home Assistant automation blueprints for SONOFF devices. Blueprint definitions live in `automation/sonoff/`, with one `.yaml` file per user-facing automation. `README.md` is the catalogue: it describes every blueprint and provides Home Assistant import, GitHub, and raw-download links. Keep device-specific additions in the existing vendor directory; add a new top-level directory only when introducing another vendor or automation family.

## Development and Validation

There is no build system or automated test suite. Validate changes with focused checks:

```powershell
git diff --check                 # detect whitespace errors
Get-Content automation/sonoff/<blueprint>.yaml
```

Import the changed blueprint into a Home Assistant test instance, create an automation from it, and exercise its triggers and service calls for each declared integration (for example, ZHA and Zigbee2MQTT). Check the minimum Home Assistant version and selectors against the intended target version.

## YAML Style & Naming

Use two-space indentation, never tabs. Preserve the existing Home Assistant blueprint layout: `blueprint`, `variables`, `triggers`, `conditions`, `actions`, then `mode`. Use descriptive snake_case filenames and blueprint input/variable IDs, such as `remote_temperature_link_tp_wgzba.yaml` and `source_temperature`. Keep human-facing labels concise and explain device, integration, units, and optional behavior in descriptions. Avoid unrelated reformatting.

## Documentation and Link Integrity

Every new blueprint needs a matching entry in `README.md` with its summary, import badge URL, GitHub link, and raw-download link. When adding, moving, renaming, or deleting a file, update every affected relative and GitHub URL in the README in the same change. Verify each path segment and URL-encoded `blueprint_url` points to the final filename; do not leave stale links behind.

## Commits & Pull Requests

This repository has no established commit history yet. Use short, imperative Conventional Commit-style subjects, for example `feat: add TRV temperature sync blueprint` or `docs: fix blueprint import links`. Keep each commit focused. Pull requests should state the supported device and integrations, describe behavior changes, link related issues when applicable, and include the Home Assistant version used for manual validation. Include screenshots only when a UI-facing documentation change benefits from one.
