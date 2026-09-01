---
title: Come configurare un allarme BarcodeWake
lang: it
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
# Come configurare un allarme BarcodeWake

Crea prima il programma, scegli una missione sicura e pratica, concedi le autorizzazioni necessarie, quindi esegui un test a schermo bloccato nel breve termine. Per le missioni di scansione, registra un oggetto durevole che sarà disponibile e leggibile quando suona la sveglia.

## Scegli la missione prima dell'oggetto

Decidi quale azione dovrebbe separare il risveglio dalla dismissione. Un codice a barre in un'altra stanza crea distanza fisica. Matematica o digitazione aggiunge concentrazione senza richiedere una fotocamera. Scuotere o passi aggiunge movimento ma dipende dai sensori e potrebbe non essere adatto a ogni persona o ambiente. Il [riferimento alle missioni](../features/missions.md) spiega i compromessi tra le modalità singola, a catena e casuale.

Se usi un codice a barre, un codice QR o un tag NFC, scegli qualcosa di durevole. Evita imballaggi usa e getta, un oggetto che un altro membro della famiglia potrebbe spostare o un codice che sarà inaccessibile durante i viaggi. Verifica che la fotocamera possa mettere a fuoco nella luce prevista. L'NFC richiede un telefono e un tag compatibili.

## Configura il programma e la regola di dismissione

Apri l'editor dell'allarme, imposta l'orario desiderato e i giorni attivi, quindi seleziona la missione mostrata dalla build installata. Configura la sua difficoltà o obiettivo in modo conservativo per il primo test. Se la versione installata supporta le catene, disponi le missioni in un ordine che può essere completato in sicurezza senza correre su per le scale o lasciare un'area sicura.

Registra il codice fisico dal flusso di configurazione della missione. Dai alla sveglia un'etichetta che identifichi la routine prevista piuttosto che esporre informazioni sensibili. Rivedi volume, vibrazione e qualsiasi opzione di follow-up del risveglio visibile nella build installata. I controlli disponibili possono differire perché le [versioni pubblica e sorgente](../availability.md) non erano identiche alla data dell'audit.

## Concedi autorizzazioni con uno scopo

Consenti le notifiche e l'accesso correlato all'allarme necessari per la consegna. Concedi l'accesso alla fotocamera solo quando usi una missione di scansione e l'accesso ai sensori quando la missione scelta ne ha bisogno. Su Android, rivedi le impostazioni di allarme esatto e batteria se il controllo di affidabilità dell'app le segnala. Non assumere che salvare una sveglia provi che la consegna in background sia consentita.

## Testa il percorso completo notturno

Imposta un test pochi minuti avanti. Blocca lo schermo, lascia BarcodeWake in background e metti il telefono nello stesso stato di suono e alimentazione previsto per la notte. Conferma che l'allarme appare, l'audio è udibile e la missione esatta selezionata può essere completata. Quindi ripeti dopo aver spostato l'oggetto registrato nella sua posizione reale.

Se la consegna fallisce, usa la [lista di controllo per la consegna degli allarmi](../help/alarm-delivery.md). Se ha successo, considera di fare un [backup locale](backup-and-sharing.md) dopo che la configurazione è stabile.

