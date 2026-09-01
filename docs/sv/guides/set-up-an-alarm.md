---
title: Hur man ställer in ett BarcodeWake-larm
lang: sv
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
# Hur man ställer in ett BarcodeWake-larm

Skapa schemat först, välj ett uppdrag som är säkert och praktiskt, bevilja de nödvändiga behörigheterna och kör sedan ett närtids låsskärmstest. För skanningsuppdrag, registrera ett hållbart objekt som kommer att vara tillgängligt och läsbart när larmet ringer.

## Välj uppdraget innan objektet

Bestäm vilken åtgärd som ska skilja uppväckning från avvisning. En streckkod i ett annat rum skapar fysiskt avstånd. Matematik eller skrivning lägger till koncentration utan att kräva en kamera. Skakning eller steg lägger till rörelse men beror på sensorer och kanske inte passar alla personer eller miljöer. [Uppdragsreferensen](../features/missions.md) förklarar avvägningarna mellan enstaka, kedja och slumpmässiga lägen.

Om du använder en streckkod, QR-kod eller NFC-tagg, välj något hållbart. Undvik engångsförpackningar, ett objekt som ett annat hushållsmedlemmar kan flytta, eller en kod som kommer att vara otillgänglig under resan. Kontrollera att kameran kan fokusera i det förväntade ljuset. NFC behöver en kompatibel telefon och tagg.

## Konfigurera schemat och avvisningsregeln

Öppna larmredigeraren, ställ in önskad tid och aktiva dagar, välj sedan uppdraget som visas av den installerade versionen. Konfigurera svårighetsgraden eller målet konservativt för det första testet. Om den installerade versionen stöder kedjor, ordna uppdrag i en ordning som kan slutföras säkert utan att skynda över trappor eller lämna ett säkert område.

Registrera den fysiska koden från uppdragsinställningsflödet. Ge larmet en etikett som identifierar den avsedda rutinen snarare än att avslöja känslig information. Granska volym, vibration och eventuella uppföljningsalternativ för uppvaknandet som visas i den installerade versionen. Tillgängliga kontroller kan skilja sig åt eftersom [den offentliga och källversionen](../availability.md) inte var identiska vid granskningsdatumet.

## Bevilja behörigheter med ett syfte

Tillåt aviseringar och larmrelaterad åtkomst som behövs för leverans. Bevilja kameraåtkomst endast när du använder ett skanningsuppdrag, och sensoråtkomst när det valda uppdraget behöver det. På Android, granska exakta larm- och batteriinställningar om appens tillförlitlighetskontroll flaggar dem. Anta inte att det att spara ett larm bevisar att bakgrundsleverans är tillåten.

## Testa den fullständiga nattvägen

Ställ in ett test några minuter framåt. Lås skärmen, lämna BarcodeWake i bakgrunden och sätt telefonen i samma ljud- och strömtillstånd som planerat för natten. Bekräfta att larmet visas, ljudet är hörbart och det exakt valda uppdraget kan slutföras. Upprepa sedan efter att ha flyttat det registrerade objektet till dess verkliga plats.

Om leveransen misslyckas, använd [larmleveranskontrollistan](../help/alarm-delivery.md). Om den lyckas, överväg att göra en [lokal säkerhetskopia](backup-and-sharing.md) efter att konfigurationen är stabil.

