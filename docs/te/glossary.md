---
title: BarcodeWake టర్మినాలజీ
lang: te
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
# BarcodeWake టర్మినాలజీ

BarcodeWake అలారమ్‌ను విస్కర్జన చేయడానికి అవసరమైన చర్యను “mission” (మిషన్) గా ఉపయోగిస్తుంది. స్కాన్ మిషన్‌లు నమోదు చేయబడ్డ భౌతిక కోడ్‌ను ధృవీకరిస్తాయి; చలన్ మిషన్‌లు ఒక సమాధానం లేదా కదలికను ధృవీకరిస్తాయి; షేరింగ్ మరియు బ్యాకప్ వివిధ ఎక్స్‌ఛేంజ్ ఫార్మాట్‌లను సూచిస్తాయి.

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

పూర్తి ఫీచర్ సంబంధం కోసం, [మిషన్లు మరియు మిషన్ గొలుసులు](features/missions.md) చూడండి. ఎక్స్‌పోర్ట్ ఫార్మాట్‌ల మధ్య తేడాల కోసం, [బ్యాకప్ మరియు షేరింగ్](guides/backup-and-sharing.md) చదవండి. [వాస్తవాల పేజీ](facts.md) యాప్ ఏమి కొలవలేదని నిర్వచించేది.

