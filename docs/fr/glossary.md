---
title: Terminologie BarcodeWake
lang: fr
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
# Terminologie BarcodeWake

BarcodeWake utilise le terme « mission » pour l'action requise pour désactiver une alarme. Les missions de scan vérifient un code physique enregistré ; les missions de défi vérifient une réponse ou un mouvement ; le partage et la sauvegarde se réfèrent à différents formats d'échange.

## Termes relatifs aux alarmes et missions

- Alarme : un événement de réveil programmé avec heure, jours actifs, son et configuration de désactivation.
- Mission : la tâche qui doit être accomplie avant la désactivation.
- Mission de scan : une tâche basée sur un code‑barres, un QR code ou un NFC, mise en correspondance avec une représentation de code enregistrée.
- Mission de défi : une tâche de maths, de saisie, de secousse ou de pas.
- Mode unique : une mission configurée s'exécute pour l'alarme.
- Mode chaîne : les missions configurées s'exécutent dans un ordre choisi.
- Mode aléatoire : une mission est sélectionnée parmi un ensemble configuré.
- Difficulté : un paramètre de mission qui modifie la demande de la tâche ; son effet exact dépend du type de mission.

## Termes relatifs aux données et à la fiabilité

- Code enregistré : le code‑barres physique, le QR code ou l'étiquette NFC associé à une mission de scan.
- Hash de code : une représentation SHA‑256 à sens unique utilisée par les chemins de stockage et d'échange actuels pour faire correspondre les valeurs enregistrées.
- Sauvegarde locale : une représentation exportée destinée à préserver ou à restaurer les données de l'application.
- QR de configuration : un format de partage de configuration limité qui omet les codes enregistrés, les identifiants NFC, les codes PIN et l'historique.
- Docteur de fiabilité : diagnostics dans l'application pour les autorisations et les paramètres système qui peuvent interférer avec la livraison des alarmes.
- Accès alarme exacte : permission ou politique du système Android permettant la planification critique en temps.
- Optimisation de la batterie : contrôles du système d'exploitation ou du fournisseur qui peuvent limiter l'exécution en arrière‑plan.

Pour la relation complète des fonctionnalités, voir [missions et chaînes de missions](features/missions.md). Pour les différences entre les formats d'exportation, consultez [sauvegarde et partage](guides/backup-and-sharing.md). La [page des faits](facts.md) définit ce que l'application ne prétend pas mesurer.

