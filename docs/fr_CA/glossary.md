---
title: Terminologie de BarcodeWake
lang: fr_CA
app: barcodewake-alarm
page_type: glossary
updated: 2026-09-01
targets:
  - BarcodeWake terminology
facts_used:
  - core_measurement
  - data_storage
  - export_formats
---
# Terminologie de BarcodeWake

BarcodeWake utilise le terme « mission » pour l'action requise pour désactiver une alarme. Les missions de scan vérifient un code physique enregistré ; les missions de défi vérifient une réponse ou un mouvement ; le partage et la sauvegarde désignent différents formats d'échange.

## Termes des alarmes et des missions

- Alarme : un événement de réveil planifié avec heure, jours actifs, son et configuration de désactivation.
- Mission : la tâche qui doit être accomplie avant la désactivation.
- Mission de scan : une tâche basée sur un code‑barres, un code QR ou une technologie NFC, mise en correspondance avec une représentation de code enregistrée.
- Mission de défi : une tâche de calcul, de saisie, de secousse ou de pas.
- Mode unique : une mission configurée s'exécute pour l'alarme.
- Mode chaîne : les missions configurées s'exécutent dans un ordre défini.
- Mode aléatoire : une mission est sélectionnée parmi un ensemble configuré.
- Difficulté : un paramètre de mission qui modifie l'exigence de la tâche ; son effet exact dépend du type de mission.

## Termes des données et de la fiabilité

- Code enregistré : le code‑barres physique, le code QR ou l'étiquette NFC associé à une mission de scan.
- Hachage de code : une représentation SHA‑256 à sens unique utilisée par les chemins de stockage et d'échange actuels pour la correspondance des valeurs enregistrées.
- Sauvegarde locale : une représentation exportée destinée à préserver ou à restaurer les données de l'application.
- QR de configuration : un format limité de partage de configuration qui omet les codes enregistrés, les identifiants NFC, les codes PIN et l'historique.
- Docteur de fiabilité : des diagnostics intégrés pour les permissions et les paramètres système qui peuvent interférer avec la livraison des alarmes.
- Accès alarme exacte : permission ou politique du système Android permettant la planification critique en termes de temps.
- Optimisation de la batterie : les contrôles du système d'exploitation ou du fournisseur qui peuvent restreindre l'exécution en arrière-plan.

Pour la relation complète des fonctionnalités, consultez [missions et chaînes de missions](features/missions.md). Pour les différences entre les formats d'exportation, consultez [sauvegarde et partage](guides/backup-and-sharing.md). La [page des faits](facts.md) définit ce que l'application ne prétend pas mesurer.

