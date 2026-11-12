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

A **planned-maintenance workspace**. Real, working parts: an asset register, maintenance plans with
intervals, a derived schedule (overdue / due this week / upcoming), completion history, and a
**Complete** action that writes history and rolls the next due date forward. KPIs such as 90-day
on-time compliance are computed from those rows.

The wider industrial suite (SCADA, production/MES, energy, quality, inventory, alarms, reports,
digital twin, AI assistant) is still visible in the sidebar but **disabled** — parked until this
workflow is finished. Those entries do not navigate anywhere and contain no invented figures.

No machine, OPC UA, MQTT or Siemens S7 connection exists in this build. Plant data is simulated and
labelled **SIMULATED DATA** throughout.

## Trust

- Builds are **unsigned** — Windows SmartScreen will warn on first run (`More info` → `Run anyway`).
- Each release lists the SHA-256 of every file so a download can be verified.
- No telemetry, no network calls, no credentials required.

## Note on packaging

These are Electron applications: the JavaScript bundles inside the installer are extractable, as with
any Electron app. Only release binaries are published here — no source, no secrets, no configuration.
