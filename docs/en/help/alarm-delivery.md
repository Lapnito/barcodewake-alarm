---
title: Why a BarcodeWake alarm may not ring
lang: en
app: barcodewake-alarm
page_type: help
updated: 2026-09-01
targets:
  - why did my BarcodeWake alarm not ring
facts_used:
  - accuracy_limits
  - hardware_requirements
  - known_limitations
---
# Why a BarcodeWake alarm may not ring

A saved alarm can still be blocked by notification settings, exact-alarm access, focus or silent modes, low volume, battery restrictions, app suspension or vendor background controls. Check delivery separately from mission scanning, then run a locked-screen test.

## First isolate delivery from dismissal

Create a near-term test alarm with a simple mission and leave the app in the background. Lock the screen. If no alarm screen or sound appears, the problem is delivery; changing the registered barcode will not fix it. If the alarm appears but the mission cannot complete, delivery works and the issue is camera, sensor, code matching or mission configuration.

Confirm the alarm is enabled, the scheduled day is correct and the phone’s time zone matches the intended schedule. Check media and alarm volume rather than relying only on the side-button state. Review do-not-disturb or focus rules, connected audio devices and whether the phone was restarted after the alarm was created.

## Review operating-system permission gates

Allow notifications and any exact-alarm or full-screen alarm access requested by the installed build. Remove BarcodeWake from aggressive battery optimisation or automatic sleeping lists when the device vendor offers those controls. Open the in-app reliability diagnostics and follow the device-specific settings it identifies. The [privacy and reliability page](../features/privacy-and-reliability.md) explains why these system dependencies remain even when app data is local.

After changing one setting, repeat the locked-screen test. Changing several controls at once makes the cause harder to identify. System updates can reset or reinterpret permissions, so retest after a major update or app reinstall.

## Diagnose mission completion separately

For barcode and QR missions, clean the camera lens, improve lighting and confirm the registered object is unchanged. Grant camera permission. For NFC, verify device support and hold the tag near the correct antenna position. Shake and step missions depend on motion or step sensors and may behave differently when power-saving modes restrict sensor delivery.

If a mission was configured as part of a chain, every required step must complete. Review [mission behaviour](../features/missions.md) and, if necessary, create a new test using the [setup procedure](../guides/set-up-an-alarm.md).

## Know when the phone is the boundary

BarcodeWake cannot override a powered-off device, an exhausted battery, broken audio hardware or every manufacturer task killer. It is not an emergency notification service. Keep another alarm method for high-consequence situations and report reproducible failures with device model, system version, app version and the exact test conditions.
