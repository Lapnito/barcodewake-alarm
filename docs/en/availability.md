---
title: BarcodeWake availability and versions
lang: en
app: barcodewake-alarm
page_type: availability
updated: 2026-09-01
targets:
  - where is BarcodeWake available
facts_used:
  - known_limitations
  - hardware_requirements
---
# BarcodeWake availability and versions

BarcodeWake has a verified public Google Play listing for Android. At the audit date, Google Play showed version 1.0.0, while the checked source project declared version 2.0.0+2. No public App Store listing was verified.

## Verified public distribution

The Android package is publicly listed as [BarcodeWake: No Cheat Alarm on Google Play](https://play.google.com/store/apps/details?id=com.tomas.barcodewake_alarm&hl=en&gl=us). The store snapshot captured for this documentation reported version 1.0.0 and a last-updated date in March 2026. That snapshot is evidence of the listing at a point in time, not a promise that every region sees the same rollout or that the listing will remain unchanged.

The source tree contains Android and iOS platform projects. Platform source does not prove store publication. Because no App Store page was verified, these docs describe iOS-related items as source support only and do not tell readers that BarcodeWake is currently downloadable from Apple.

## Why two version numbers appear

The repository `pubspec.yaml` declares source version 2.0.0+2 and its changelog describes a broader mission system than the captured public listing. A store rollout may lag behind a development branch, be staged by region, or simply not have been published. Without a matching store record, the safe statement is narrow: the capability exists in the checked source, while public availability is proven only for the captured store version.

When a feature page says “current source”, that wording is deliberate. Before relying on mission chains, setup sharing or another newer capability, check the installed app’s version and visible controls. Start with [mission behaviour](features/missions.md), then use the [setup guide](guides/set-up-an-alarm.md) only for options your installed build actually shows.

## Device requirements and installation checks

Scanning requires camera permission. NFC, motion and step missions need corresponding device hardware. Android alarm delivery can require notification and exact-alarm access, with additional battery settings on some manufacturers. Install from the verified store listing, create a near-term test alarm, lock the screen and confirm both sound and the selected mission before depending on it for an important wake-up.

For a concise boundary list, read [product facts](facts.md). If a test alarm fails, follow [alarm delivery troubleshooting](help/alarm-delivery.md) rather than repeatedly recreating the alarm.
