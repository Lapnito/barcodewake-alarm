---
title: BarcodeWake privacy e affidabilità dell'allarme
lang: it
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
# BarcodeWake privacy e affidabilità dell'allarme

BarcodeWake mantiene la configurazione documentata dell'allarme e i dati della missione sul dispositivo e non richiede un account dell'app. Gli attuali percorsi del codice eseguono l'hash dei valori dei codici registrati. La telemetria opzionale è descritta come disabilitata per impostazione predefinita, mentre la consegna dell'allarme dipende ancora dalle autorizzazioni di sistema e dai controlli del produttore.

## I dati locali non rimuovono le dipendenze di sistema

L'archiviazione locale significa che la configurazione ordinaria dell'allarme non richiede un account cloud BarcodeWake. I record dell'allarme, la cronologia e le preferenze vengono gestiti attraverso il livello di dati locale dell'app. I valori registrati di barcode, QR e NFC sono rappresentati con hash SHA-256 negli attuali percorsi di archiviazione e importazione, il che evita di conservare il valore normale non elaborato per la corrispondenza.

L'hashing non è la stessa cosa della crittografia di ogni record dell'app e l'archiviazione locale non è un backup. Qualcuno con accesso a un dispositivo sbloccato potrebbe ancora vedere i nomi degli allarmi, gli orari o la cronologia attraverso l'app. Un telefono perso o ripristinato può anche perdere i dati locali a meno che l'utente non abbia effettuato un'esportazione. Vedi [backup e condivisione](../guides/backup-and-sharing.md) per i formati e i loro diversi scopi.

L'informativa sulla privacy afferma che la telemetria opzionale è disattivata per impostazione predefinita e descrive la gestione aggregata se abilitata. Questa documentazione pertanto non afferma l'affermazione più ampia che l'app non possa mai comunicare tramite una rete. Descrive i fatti verificati più ristretti: il funzionamento principale e i dati sono locali, nessun account del prodotto è richiesto e nessuna dipendenza dall'SDK pubblicitario appare nel progetto controllato.

## L'affidabilità è una responsabilità condivisa

BarcodeWake può programmare e presentare un allarme, ma il sistema operativo decide quando il lavoro in background può essere eseguito e quali interruzioni sono consentite. L'autorizzazione di notifica, l'accesso all'allarme esatto, le modalità silenziose o di messa a fuoco, l'ottimizzazione della batteria, la sospensione automatica dell'app e i killer di attività del produttore possono tutti avere importanza. Lo strumento di affidabilità nell'app può identificare i rischi di configurazione e indirizzare gli utenti alle impostazioni; non può sovrascrivere la politica di sistema.

Dopo l'installazione, testa con lo schermo bloccato e il telefono nella stessa modalità di alimentazione utilizzata durante la notte. Ripeti quel test dopo un aggiornamento di sistema, una modifica del risparmio energetico o una reinstallazione dell'app. Tieni il dispositivo carico, il volume appropriato e la missione scelta fisicamente disponibile. Segui la [risoluzione dei problemi di consegna dell'allarme](../help/alarm-delivery.md) quando un test fallisce.

## Cosa la privacy e l'affidabilità non promettono

BarcodeWake non è un dispositivo medico, un servizio di allarme di emergenza o un tracker delle fasi del sonno. Nessuna app di allarme può garantire il risveglio o compensare un dispositivo non disponibile. La [pagina dei fatti e dei limiti](../facts.md) elenca questi confini, mentre [disponibilità](../availability.md) separa le evidenze degli store pubblici dalle funzionalità più recenti delle sorgenti.

