---
title: BarcodeWake privacy and alarm reliability
lang: en
app: barcodewake-alarm
page_type: feature
updated: 2026-09-01
targets:
  - is BarcodeWake private and reliable
facts_used:
  - offline
  - account_required
  - ads_tracking
  - data_storage
  - accuracy_limits
---
# BarcodeWake privacy and alarm reliability

BarcodeWake keeps documented alarm configuration and mission data on the device and requires no app account. Current code paths hash registered code values. Optional telemetry is described as disabled by default, while alarm delivery still depends on system permissions and vendor controls.

## Local data does not remove system dependencies

Local storage means ordinary alarm setup does not require a BarcodeWake cloud account. Alarm records, history and preferences are handled through the app’s local data layer. Registered barcode, QR and NFC values are represented with SHA-256 hashes in current storage and import paths, which avoids retaining the ordinary raw value for matching.

Hashing is not the same as encryption of every app record, and local storage is not a backup. Someone with access to an unlocked device may still see alarm names, schedules or history through the app. A lost or reset phone can also lose local data unless the user made an export. See [backup and sharing](../guides/backup-and-sharing.md) for the formats and their different purposes.

The privacy policy says optional telemetry is off by default and describes aggregate handling if enabled. This documentation therefore does not make the broader claim that the app can never communicate over a network. It states the narrower verified facts: core operation and data are local, no product account is required, and no advertising SDK dependency appears in the checked project.

## Reliability is a shared responsibility

BarcodeWake can schedule and present an alarm, but the operating system decides when background work may run and which interruptions are allowed. Notification permission, exact-alarm access, silent or focus modes, battery optimisation, automatic app suspension and manufacturer task killers can all matter. The in-app reliability tooling can identify configuration risks and direct users to settings; it cannot override system policy.

After installation, test with the screen locked and the phone in the same power mode used overnight. Repeat that test after a system update, battery-saver change or app reinstall. Keep the device charged, volume appropriate and chosen mission physically available. Follow [alarm delivery troubleshooting](../help/alarm-delivery.md) when a test fails.

## What privacy and reliability do not promise

BarcodeWake is not a medical device, emergency alert service or sleep-stage tracker. No alarm app can guarantee waking or compensate for an unavailable device. The [facts and limits page](../facts.md) lists these boundaries, while [availability](../availability.md) separates public store evidence from newer source capabilities.
