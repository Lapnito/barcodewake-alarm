---
title: BarcodeWake terminology
lang: en
app: barcodewake-alarm
page_type: glossary
updated: 2026-09-01
targets:
  - BarcodeWake terminology
facts_used:
  - core_measurement
  - data_storage
  - export_formats
---
# BarcodeWake terminology

BarcodeWake uses “mission” for the action required to dismiss an alarm. Scan missions verify a registered physical code; challenge missions verify an answer or movement; sharing and backup refer to different exchange formats.

## Alarm and mission terms

- Alarm: a scheduled wake event with time, active days, sound and dismissal configuration.
- Mission: the task that must be completed before dismissal.
- Scan mission: a barcode, QR or NFC-based task matched against a registered code representation.
- Challenge mission: a maths, typing, shake or step task.
- Single mode: one configured mission runs for the alarm.
- Chain mode: configured missions run in a chosen order.
- Random mode: one mission is selected from a configured set.
- Difficulty: a mission setting that changes task demand; its exact effect depends on mission type.

## Data and reliability terms

- Registered code: the physical barcode, QR code or NFC tag associated with a scan mission.
- Code hash: a one-way SHA-256 representation used by current storage and exchange paths for matching registered values.
- Local backup: an exported representation intended to preserve or restore app data.
- Setup QR: a limited configuration-sharing format that omits registered codes, NFC identifiers, PINs and history.
- Reliability Doctor: in-app diagnostics for permissions and system settings that may interfere with alarm delivery.
- Exact-alarm access: Android system permission or policy allowing time-critical scheduling.
- Battery optimisation: operating-system or vendor controls that may restrict background execution.

For the full feature relationship, see [missions and mission chains](features/missions.md). For differences between export formats, read [backup and sharing](guides/backup-and-sharing.md). The [facts page](facts.md) defines what the app does not claim to measure.
