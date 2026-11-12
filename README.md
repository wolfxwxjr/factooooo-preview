# Factooooo — public preview

This repository exists only to distribute **preview builds** of the Factooooo Windows application,
so they can be downloaded without a GitHub account. The application source lives in a private
repository and is not published here.

## Download

Latest build: **[v0.1.1](https://github.com/wolfxwxjr/factooooo-preview/releases/latest)**

| File | Use it if |
| --- | --- |
| `Factooooo-Portable-<version>-x64.exe` | You want to run it immediately. Single file, nothing installed, data kept in a `Factooooo-Data` folder beside the executable. |
| `Factooooo-Setup-<version>-x64.exe` | You want it installed with a desktop shortcut and faster subsequent launches. Per-user, no admin rights. |

Landing page: https://wolfxwxjr.github.io/factooooo-preview/

## What this build is

A **foundation preview**: the desktop shell, local SQLite database and Windows packaging are real and
tested. The individual modules (SCADA, production/MES, maintenance, energy, quality, inventory, alarms,
reports, digital twin, AI assistant) are navigable screens that state plainly they are not implemented —
they contain no fabricated figures.

No machine, OPC UA, MQTT or Siemens S7 connection exists in this build. Everything is labelled
**SIMULATED DATA**.

## Trust

- Builds are **unsigned** — Windows SmartScreen will warn on first run (`More info` → `Run anyway`).
- Each release lists the SHA-256 of every file so a download can be verified.
- No telemetry, no network calls, no credentials required.

## Note on packaging

These are Electron applications: the JavaScript bundles inside the installer are extractable, as with
any Electron app. Only release binaries are published here — no source, no secrets, no configuration.
