---
title: Faits et limites de BarcodeWake
lang: fr_CA
app: barcodewake-alarm
page_type: facts
updated: 2026-09-01
targets:
  - BarcodeWake facts and limitations
facts_used:
  - what_it_is
  - core_measurement
  - offline
  - account_required
  - data_storage
  - known_limitations
---
# Faits et limites de BarcodeWake

## Aperçu des faits du produit

| Question | Réponse vérifiée |
|---|---|
| Qu'est-ce que c'est? | Une alarme avec des missions de désactivation physiques et cognitives. |
| Quelles missions existent dans la source actuelle? | Code-barres, QR, maths, dactylographie, secousse et pas. Le NFC est traité comme un chemin de code enregistré. |
| Un compte est-il requis? | Aucun compte ni flux de connexion n'est présent pour les fonctionnalités documentées. |
| Où les données sont-elles conservées? | La configuration des alarmes, l'historique et les préférences utilisent le stockage local. Les chemins de code actuels hachent les valeurs de code enregistrées. |
| Est-ce un traqueur de sommeil? | Non. Elle planifie les alarmes et vérifie les missions; elle ne classifie pas les stades du sommeil. |
| Chaque fonction de la source est-elle publiée publiquement? | Non établi. Les versions du magasin et de la source différaient à la date de l'audit. |

## Limites qui importent en pratique

Une application d'alarme fonctionne dans les contraintes du téléphone. L'autorisation de notification, l'accès aux alarmes exactes, les paramètres de mise au point, l'optimisation de la batterie et les contrôles d'arrière-plan spécifiques au fournisseur peuvent affecter la réception d'une alarme comme prévu. BarcodeWake comprend des vérifications de fiabilité et des conseils, mais une application ne peut pas contourner chaque restriction du système d'exploitation ou du fabricant. Testez une alarme après l'installation et après des modifications importantes du système; la [liste de vérification de la livraison](help/alarm-delivery.md) explique comment.

Le matériel de mission compte aussi. Le balayage nécessite un accès à la caméra et un code physique lisible. Les missions de secousse et de pas dépendent des capteurs appropriés. Le NFC nécessite un matériel compatible. Une étiquette copiée ou endommagée peut empêcher une correspondance, alors gardez un chemin de récupération et ne rendez pas le seul objet enregistré inaccessible.

## Allégations intentionnellement non faites

Ces pages ne prétendent aucun avantage médical, un réveil garanti, une synchronisation du cycle de sommeil, une synchronisation cloud ou une version iOS publique vérifiée. Elles ne considèrent pas non plus la version source comme une version du magasin en direct. Voir [disponibilité](availability.md) pour cette distinction et [confidentialité et fiabilité](features/privacy-and-reliability.md) pour les preuves derrière le stockage local et la formulation de la télémétrie.

