---
title: Back up and share BarcodeWake alarms safely
lang: en
app: barcodewake-alarm
page_type: guide
updated: 2026-09-01
targets:
  - how to back up or share BarcodeWake alarms
facts_used:
  - export_formats
  - data_storage
  - known_limitations
---
# Back up and share BarcodeWake alarms safely

Use a JSON export when preserving or moving your own app data, a printable PDF backup barcode for recovery, and setup QR sharing when another person only needs the alarm structure. Sharing intentionally omits registered secrets and history.

## Pick the format for the job

The current source provides different exchange paths because backup and sharing are not the same operation. A JSON backup is intended for structured data transfer and restoration. A PDF backup turns recovery material into a printable barcode document. A setup QR is deliberately narrower: it can pass a limited alarm configuration without carrying registered barcode values, NFC identifiers, PINs or history.

Do not treat a setup QR as a complete device backup. The recipient must register their own physical codes and review permissions locally. Current setup sharing also limits how many alarms it carries, so verify the imported result rather than assuming every schedule moved. The [product facts](../facts.md) records these boundaries.

## Create and protect a personal backup

Use the export action available in the installed build, choose JSON or the printable backup according to the recovery plan, and save the result somewhere you control. A backup may reveal alarm names, schedules and other configuration even when registered raw code values are protected or omitted. Handle it like personal routine data: avoid public links, shared printers and untrusted messaging channels.

After exporting, confirm that the file can be found and that its timestamp matches the intended backup. Do not delete the original app data merely because an export command reported success. Restore testing is the only reliable check, but perform it on a safe device or after making a second copy so the test itself does not become a loss event.

## Share setup without sharing secrets

Generate a setup QR only for alarms the recipient should receive. The recipient scans it, reviews the imported schedule and supplies their own code, NFC tag or recovery details. This design prevents a shared configuration from silently transferring the physical key that dismisses somebody else’s alarm.

After import, each person should run the full [alarm setup test](set-up-an-alarm.md). Permissions, sensors and operating-system restrictions do not transfer in the QR. If an imported alarm fails to appear while locked, follow [alarm delivery troubleshooting](../help/alarm-delivery.md).

Source and store versions differed during this audit, so an installed public build may not expose every exchange option described here. [Availability](../availability.md) explains how to interpret source-only capabilities.
