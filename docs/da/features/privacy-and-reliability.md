---
title: BarcodeWake privatliv og alarmpålidelighed
lang: da
app: barcodewake-alarm
page_type: feature
updated: 2026-09-01
targets:
  - is BarcodeWake private and reliable
facts_used:
  - offline
  - account_required
  - ads_tracking
  - data_storage
  - accuracy_limits
---
# BarcodeWake privatliv og alarmpålidelighed

BarcodeWake opbevarer dokumenteret alarmkonfiguration og missionsdata på enheden og kræver ingen app-konto. Aktuelle kodestier hasher registrerede kodeværdier. Valgfri telemetri er beskrevet som deaktiveret som standard, mens alarmlevering stadig afhænger af systemtilladelser og leverandørkontroller.

## Lokale data fjerner ikke systemafhængigheder

Lokal lagring betyder, at normal alarmkonfiguration ikke kræver en BarcodeWake-cloudkonto. Alarmposter, historik og præferencer håndteres via appens lokale datalag. Registrerede stregkode-, QR- og NFC-værdier er repræsenteret med SHA-256-hash i aktuelle lagrings- og importstier, hvilket undgår at opbevare den normale råværdi til matching.

Hashing er ikke det samme som kryptering af hver eneste applikationspost, og lokal lagring er ikke en sikkerhedskopi. En person med adgang til en ulåst enhed kan stadig se alarmnavne, tidsplaner eller historik gennem appen. En tabt eller nulstillet telefon kan også miste lokale data, medmindre brugeren har lavet en eksport. Se [backup og deling](../guides/backup-and-sharing.md) for formaterne og deres forskellige formål.

Privatlivspolitikken siger, at valgfri telemetri er slået fra som standard og beskriver aggregeret håndtering, hvis den er aktiveret. Denne dokumentation fremsætter derfor ikke det bredere krav, at appen aldrig kan kommunikere over et netværk. Den angiver de snævrere verificerede fakta: kernefunktion og data er lokale, ingen produktkonto kræves, og ingen reklame-SDK-afhængighed fremgår af det kontrollerede projekt.

## Pålidelighed er et delt ansvar

BarcodeWake kan planlægge og præsentere en alarm, men operativsystemet afgør, hvornår baggrundsarbejde kan køre, og hvilke afbrydelser der er tilladt. Notifikationstilladelse, eksakt-alarm-adgang, lydløs- eller fokus-tilstande, batterioptimering, automatisk app-suspension og producentens opgavedræbere kan alle have betydning. Det indbyggede pålidelighedsværktøj kan identificere konfigurationsrisici og dirigere brugere til indstillinger; det kan ikke tilsidesætte systempolitik.

Efter installation skal du teste med skærmen låst og telefonen i den samme strømtilstand, der bruges natten over. Gentag den test efter en systemopdatering, batterispareændring eller app-geninstallation. Hold enheden opladet, lydstyrken passende og den valgte mission fysisk tilgængelig. Følg [alarmleveringsfejlfinding](../help/alarm-delivery.md), når en test fejler.

## Hvad privatliv og pålidelighed ikke lover

BarcodeWake er ikke en medicinsk anordning, nødalarmeringstjeneste eller søvnstadietracker. Ingen alarm-app kan garantere at vække eller kompensere for en utilgængelig enhed. [Fakta og begrænsninger-siden](../facts.md) viser disse grænser, mens [tilgængelighed](../availability.md) adskiller offentlige butiksresultater fra nyere kildeegenskaber.

