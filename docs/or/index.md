---
title: BarcodeWake documentation
lang: or
app: barcodewake-alarm
page_type: index
updated: 2026-09-01
targets:
  - what is BarcodeWake
facts_used:
  - what_it_is
  - known_limitations
---
# BarcodeWake documentation

BarcodeWake is an alarm clock that makes dismissal a deliberate act. An alarm can require a saved barcode or QR code, a short cognitive task, a shake sequence, or a step target instead of relying only on an easy on-screen button.

## What makes BarcodeWake different

The central idea is distance plus intent. If the registered code is attached to an object away from bed, silencing the alarm means getting up, reaching that object and scanning it. The same alarm model can also use maths, typing, shake or step missions. Current source code supports a single mission, an ordered chain, or random selection from configured missions.

That friction is useful for people who dismiss an ordinary alarm without becoming fully alert. It is not sleep-stage analysis, medical guidance or a guarantee that someone will wake. Hardware support, permissions and vendor battery controls still affect delivery. The [mission reference](features/missions.md) explains the choices, while [alarm delivery troubleshooting](help/alarm-delivery.md) covers system settings that can interfere.

## Start with the right document

Use the [setup guide](guides/set-up-an-alarm.md) when creating an alarm and registering a physical code. Read [backup and sharing](guides/backup-and-sharing.md) before moving data or sending a setup QR to someone else. The share format deliberately excludes registered codes, NFC identifiers, PINs and alarm history, so a recipient must complete sensitive setup locally.

For a short, auditable summary, see [product facts](facts.md). For release status, use [availability](availability.md): the public Google Play version captured for this audit differs from the version declared by the checked source tree. The newer source version is therefore documented as source capability, not asserted as a published store release.

## Privacy and reliability boundaries

Core configuration and mission data are stored on the device, and no BarcodeWake account is required. Current code paths represent registered code values with SHA-256 hashes. Optional telemetry is described by the privacy policy as disabled by default. Those statements do not mean every phone will deliver alarms identically; Android vendors and operating-system permissions can still restrict background behaviour.

Read [privacy and reliability](features/privacy-and-reliability.md) for the distinction between local data handling and operating-system delivery. The [standard alarm comparison](comparisons/standard-alarm.md) helps decide whether mission-based dismissal matches the way you wake up.

