---
title: BarcodeWake मिशन आणि मिशन साखळ्या
lang: mr
app: barcodewake-alarm
page_type: feature
updated: 2026-09-01
targets:
  - how do BarcodeWake missions work
facts_used:
  - what_it_is
  - core_measurement
  - hardware_requirements
  - known_limitations
---
# BarcodeWake मिशन आणि मिशन साखळ्या

A BarcodeWake mission is the condition used to dismiss an alarm. Current source supports barcode, QR, maths, typing, shake and step tasks, with registered NFC handled through the code-scanning path. Missions may run alone, in sequence or by random selection.

## Scan missions create physical distance

A barcode or QR mission compares a live camera scan with a code registered during setup. The code can be placed on an object outside arm's reach: toiletries in a bathroom, a breakfast item in a kitchen, or another stable object in a well-lit area. NFC follows the same general idea with a compatible tag and device. The app stores a hash representation in current paths rather than needing the raw code for ordinary comparison.

Choose an object that will still be available when the alarm rings. Packaging gets discarded, labels fade and travel changes the environment. Registering a code on the only medicine box you may need to replace is less robust than using a durable label. The [alarm setup guide](../guides/set-up-an-alarm.md) covers placement and testing.

## Challenge missions trade movement for effort

Maths and typing require focused input. Shake and steps require physical movement and supported sensors. Difficulty and target settings change how much work is expected, but a harder mission is not automatically a better one. Excessive friction can encourage disabling the alarm entirely, while an easy task may become automatic after repetition.

Match the task to the failure mode. If you switch off alarms half-asleep, scanning in another room creates useful distance. If camera access is inconvenient, a short typing or maths task may be more practical. If mobility, balance or accessibility is a concern, avoid movement-based missions and choose a task that can be completed safely.

## Single, chain and random modes

Single mode asks for one configured mission. Chain mode runs several configured missions in order. Random mode selects from a configured set, reducing the chance that one memorised interaction becomes automatic. These modes are present in the newer checked source; [availability](../availability.md) explains why that does not prove they are already in every public build.

Always run a near-term test after changing mode, permissions or registered objects. Keep the selected object reachable and provide a safe recovery route. For delivery issues unrelated to mission completion, use the [reliability checklist](../help/alarm-delivery.md).

