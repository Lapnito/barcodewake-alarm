---
title: How to set up a BarcodeWake alarm
lang: en
app: barcodewake-alarm
page_type: guide
updated: 2026-09-01
targets:
  - how to set up a BarcodeWake alarm
facts_used:
  - what_it_is
  - hardware_requirements
  - accuracy_limits
---
# How to set up a BarcodeWake alarm

Create the schedule first, choose a mission that is safe and practical, grant the required permissions, then run a near-term locked-screen test. For scan missions, register a durable object that will be available and readable when the alarm rings.

## Choose the mission before the object

Decide what action should separate waking from dismissal. A barcode in another room creates physical distance. Maths or typing adds concentration without requiring a camera. Shake or steps adds movement but depends on sensors and may not suit every person or environment. The [mission reference](../features/missions.md) explains the trade-offs among single, chain and random modes.

If using a barcode, QR code or NFC tag, choose something durable. Avoid disposable packaging, an object another household member may move, or a code that will be inaccessible while travelling. Check that the camera can focus in the expected light. NFC needs a compatible phone and tag.

## Configure the schedule and dismissal rule

Open the alarm editor, set the desired time and active days, then select the mission shown by the installed build. Configure its difficulty or target conservatively for the first test. If the installed version supports chains, arrange missions in an order that can be completed safely without rushing across stairs or leaving a secure area.

Register the physical code from the mission setup flow. Give the alarm a label that identifies the intended routine rather than exposing sensitive information. Review volume, vibration and any wake-up follow-up options visible in the installed build. Available controls can differ because the [public and source versions](../availability.md) were not identical at the audit date.

## Grant permissions with a purpose

Allow notifications and alarm-related access needed for delivery. Grant camera access only when using a scan mission, and sensor access when the chosen mission needs it. On Android, review exact-alarm and battery settings if the app’s reliability check flags them. Do not assume that saving an alarm proves background delivery is permitted.

## Test the complete overnight path

Set a test a few minutes ahead. Lock the screen, leave BarcodeWake in the background and put the phone in the same sound and power state planned for overnight. Confirm that the alarm appears, audio is audible and the exact selected mission can be completed. Then repeat after moving the registered object to its real location.

If delivery fails, use the [alarm delivery checklist](../help/alarm-delivery.md). If it succeeds, consider making a [local backup](backup-and-sharing.md) after the setup is stable.
