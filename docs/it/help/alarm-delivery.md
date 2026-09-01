---
title: Perché un allarme BarcodeWake potrebbe non suonare
lang: it
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
# Perché un allarme BarcodeWake potrebbe non suonare

Un allarme salvato può comunque essere bloccato dalle impostazioni di notifica, dall'accesso all'allarme esatto, dalla modalità Messa a fuoco o silenziosa, dal volume basso, dalle restrizioni della batteria, dalla sospensione dell'app o dai controlli in background del produttore. Verifica la consegna separatamente dalla scansione della missione, quindi esegui un test con schermata bloccata.

## Isolare innanzitutto la consegna dal rifiuto

- Crea un allarme di test a breve termine con una missione semplice e lascia l'app in background. Blocca lo schermo. Se non appare alcuna schermata o suono dell'allarme, il problema è la consegna; modificare il codice a barre registrato non lo risolverà. Se l'allarme appare ma la missione non può essere completata, la consegna funziona e il problema è la fotocamera, il sensore, la corrispondenza del codice o la configurazione della missione.
- Conferma che l'allarme è attivato, che il giorno programmato è corretto e che il fuso orario del telefono corrisponde all'orario previsto. Controlla il volume dei media e dell'allarme invece di fidarti solo dello stato del pulsante laterale. Verifica le regole di Modalità Non disturbare o Messa a fuoco, i dispositivi audio collegati e se il telefono è stato riavviato dopo la creazione dell'allarme.

## Rivedere i permessi del sistema operativo

Consenti le notifiche e qualsiasi accesso all'allarme esatto o a tutto schermo richiesto dalla build installata. Rimuovi BarcodeWake dalle liste aggressive di ottimizzazione della batteria o di sospensione automatica quando il produttore del dispositivo offre tali controlli. Apri la diagnostica di affidabilità all'interno dell'app e segui le impostazioni specifiche del dispositivo che identifica. La [pagina sulla privacy e affidabilità](../features/privacy-and-reliability.md) spiega perché queste dipendenze di sistema rimangono anche quando i dati dell'app sono locali.

Dopo aver modificato un'impostazione, ripeti il test con schermata bloccata. Modificare diversi controlli contemporaneamente rende più difficile identificare la causa. Gli aggiornamenti di sistema possono reimpostare o reinterpretare i permessi, quindi riprova dopo un aggiornamento importante o dopo aver reinstallato l'app.

## Diagnosticare il completamento della missione separatamente

Per le missioni con codice a barre e QR, pulisci l'obiettivo della fotocamera, migliora l'illuminazione e conferma che l'oggetto registrato non è cambiato. Concedi il permesso della fotocamera. Per NFC, verifica il supporto del dispositivo e tieni il tag vicino alla posizione corretta dell'antenna. Le missioni di shake e passo dipendono dai sensori di movimento o di passi e potrebbero comportarsi diversamente quando le modalità di risparmio energetico limitano la consegna dei sensori.

Se una missione è stata configurata come parte di una catena, ogni passaggio richiesto deve essere completato. Consulta il [comportamento della missione](../features/missions.md) e, se necessario, crea un nuovo test usando la [procedura di configurazione](../guides/set-up-an-alarm.md).

## Sapere quando il telefono è il limite

BarcodeWake non può ignorare un dispositivo spento, una batteria scarica, un hardware audio rotto o ogni task killer del produttore. Non è un servizio di notifica di emergenza. Tieni un altro metodo di allarme per situazioni ad alta conseguenza e segnala i guasti riproducibili indicando il modello del dispositivo, la versione del sistema, la versione dell'app e le condizioni esatte del test.

