---
title: Säkerhetskopiera och dela BarcodeWake-larm säkert
lang: sv
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
# Säkerhetskopiera och dela BarcodeWake-larm säkert

Använd en JSON-export när du bevarar eller flyttar dina egna appdata, en utskrivbar PDF-säkerhetskopia med streckkod för återställning, och konfigurera QR-delning när en annan person endast behöver larmstrukturen. Delning utelämnar medvetet registrerade hemligheter och historik.

## Välj format för uppgiften

Den aktuella källan tillhandahåller olika utbytesvägar eftersom säkerhetskopiering och delning inte är samma åtgärd. En JSON-säkerhetskopia är avsedd för strukturerad dataöverföring och återställning. En PDF-säkerhetskopia omvandlar återställningsmaterial till ett utskrivbart streckkodsdokument. En installations-QR är medvetet smalare: den kan överföra en begränsad larmkonfiguration utan att bära registrerade streckkodsvärden, NFC-identifierare, PIN-koder eller historik.

Behandla inte en installations-QR som en komplett enhetssäkerhetskopia. Mottagaren måste registrera sina egna fysiska koder och granska behörigheter lokalt. Aktuell installationsdelning begränsar också hur många larm den kan bära, så verifiera det importerade resultatet snarare än att anta att varje schema överfördes. [Produktfakta](../facts.md) registrerar dessa gränser.

## Skapa och skydda en personlig säkerhetskopia

Använd exportåtgärden som finns i den installerade versionen, välj JSON eller den utskrivbara säkerhetskopian enligt återställningsplanen, och spara resultatet någonstans du kontrollerar. En säkerhetskopia kan avslöja larmnamn, scheman och annan konfiguration även när registrerade råa kodvärden är skyddade eller utelämnade. Hantera den som personliga rutinuppgifter: undvik offentliga länk, delade skrivare och opålitliga meddelandekanaler.

Efter export, bekräfta att filen kan hittas och att dess tidsstämpel matchar den avsedda säkerhetskopian. Ta inte bort originalappdata bara för att ett exportkommando rapporterade framgång. Återställningstestning är den enda tillförlitliga kontrollen, men utför den på en säker enhet eller efter att ha gjort en andra kopia så att testet själv inte blir en förlusthändelse.

## Dela konfiguration utan att dela hemligheter

Generera en installations-QR endast för larm som mottagaren ska ta emot. Mottagaren skannar den, granskar det importerade schemat och tillhandahåller sina egna koder, NFC-taggar eller återställningsdetaljer. Denna design förhindrar att en delad konfiguration tyst överför den fysiska nyckeln som stänger av någon annans larm.

Efter import bör varje person köra det fullständiga [larmkonfigurationstestet](set-up-an-alarm.md). Behörigheter, sensorer och operativsystembegränsningar överförs inte i QR-koden. Om ett importerat larm inte visas när det är låst, följ [larmleveransfelsökning](../help/alarm-delivery.md).

Källa och lagrade versioner skilde sig under denna granskning, så en installerad offentlig version kanske inte exponera alla utbytesalternativ som beskrivs här. [Tillgänglighet](../availability.md) förklarar hur man tolkar källkodsspecifika funktioner.

