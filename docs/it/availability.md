---
title: Disponibilità e versioni di BarcodeWake
lang: it
app: barcodewake-alarm
page_type: availability
updated: 2026-09-01
targets:
  - where is BarcodeWake available
facts_used:
  - known_limitations
  - hardware_requirements
---
# Disponibilità e versioni di BarcodeWake

BarcodeWake ha una scheda pubblica verificata su Google Play per Android. Alla data dell'audit, Google Play mostrava la versione 1.0.0, mentre il progetto sorgente controllato dichiarava la versione 2.0.0+2. Nessuna scheda pubblica sull'App Store è stata verificata.

## Distribuzione pubblica verificata

Il pacchetto Android è elencato pubblicamente come [BarcodeWake: No Cheat Alarm su Google Play](https://play.google.com/store/apps/details?id=com.tomas.barcodewake_alarm&hl=en&gl=us). Lo snapshot dello store catturato per questa documentazione riportava la versione 1.0.0 e una data di ultimo aggiornamento nel marzo 2026. Tale snapshot è una prova dell'elenco in un determinato momento, non una promessa che ogni regione veda lo stesso rollout o che l'elenco rimanga invariato.

L'albero dei sorgenti contiene progetti per piattaforme Android e iOS. Il codice sorgente della piattaforma non dimostra la pubblicazione sullo store. Poiché nessuna pagina dell'App Store è stata verificata, questi documenti descrivono gli elementi relativi a iOS solo come supporto del codice sorgente e non informano i lettori che BarcodeWake è attualmente scaricabile da Apple.

## Perché appaiono due numeri di versione

Il repository `pubspec.yaml` dichiara la versione sorgente 2.0.0+2 e il suo changelog descrive un sistema di missioni più ampio rispetto all'elenco pubblico catturato. Un rollout sullo store può rimanere indietro rispetto a un branch di sviluppo, essere distribuito per regione o semplicemente non essere stato pubblicato. Senza un record corrispondente sullo store, l'affermazione sicura è ristretta: la funzionalità esiste nel codice sorgente controllato, mentre la disponibilità pubblica è dimostrata solo per la versione dello store catturata.

Quando una pagina delle funzionalità dice "codice sorgente corrente", tale formulazione è intenzionale. Prima di fare affidamento su catene di missioni, condivisione della configurazione o un'altra funzionalità più recente, controlla la versione dell'app installata e i controlli visibili. Inizia con [comportamento delle missioni](features/missions.md), quindi usa la [guida alla configurazione](guides/set-up-an-alarm.md) solo per le opzioni che la build installata mostra effettivamente.

## Requisiti del dispositivo e controlli dell'installazione

La scansione richiede il permesso della fotocamera. Le missioni NFC, di movimento e dei passi richiedono l'hardware corrispondente del dispositivo. La consegna degli allarmi su Android può richiedere l'accesso alle notifiche e all'allarme esatto, con impostazioni aggiuntive della batteria su alcuni produttori. Installa dalla scheda dello store verificata, crea un allarme di test a breve termine, blocca lo schermo e conferma sia il suono che la missione selezionata prima di dipenderne per una sveglia importante.

Per un elenco conciso dei limiti, leggi [fatti del prodotto](facts.md). Se un allarme di test fallisce, segui la [risoluzione dei problemi di consegna degli allarmi](help/alarm-delivery.md) invece di ricreare ripetutamente l'allarme.

