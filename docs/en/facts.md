---
title: BarcodeWake facts and limits
lang: en
app: barcodewake-alarm
page_type: facts
updated: 2026-09-01
targets:
  - BarcodeWake facts and limitations
facts_used:
  - what_it_is
  - core_measurement
  - offline
  - account_required
  - data_storage
  - known_limitations
---
# BarcodeWake facts and limits

BarcodeWake schedules alarms and verifies a chosen dismissal mission. It can use scans, cognitive challenges or movement, stores the documented core data locally, requires no product account, and does not perform sleep-stage analysis.

## Product facts at a glance

| Question | Verified answer |
|---|---|
| What is it? | An alarm clock with physical and cognitive dismissal missions. |
| Which missions exist in current source? | Barcode, QR, maths, typing, shake and steps. NFC is handled as a registered code path. |
| Is an account required? | No account or sign-in flow is present for the documented features. |
| Where is data kept? | Alarm configuration, history and preferences use local storage. Current code paths hash registered code values. |
| Is it a sleep tracker? | No. It schedules alarms and verifies missions; it does not classify sleep stages. |
| Is every source feature publicly released? | Not established. Store and source versions differed at the audit date. |

## Limits that matter in practice

An alarm app operates inside phone-level constraints. Notification permission, exact-alarm access, focus settings, battery optimisation and vendor-specific background controls can affect whether an alarm arrives as expected. BarcodeWake includes reliability checks and guidance, but an app cannot override every operating-system or manufacturer restriction. Test an alarm after installation and after major system changes; the [delivery checklist](help/alarm-delivery.md) explains how.

Mission hardware also matters. Scanning needs camera access and a readable physical code. Shake and step missions depend on the relevant sensors. NFC needs compatible hardware. A copied or damaged label can prevent a match, so keep a recovery path and do not make the only registered object inaccessible.

## Claims intentionally not made

These pages do not claim medical benefit, guaranteed waking, sleep-cycle timing, cloud synchronisation or a verified public iOS release. They also do not treat the source version as a live store version. See [availability](availability.md) for that distinction and [privacy and reliability](features/privacy-and-reliability.md) for the evidence behind local storage and telemetry wording.
