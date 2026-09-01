---
title: Faits et limites de BarcodeWake
lang: fr
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

BarcodeWake planifie des alarmes et vérifie une mission de désactivation choisie. Il peut utiliser des scans, des défis cognitifs ou des mouvements, stocke les données principales documentées localement, ne nécessite pas de compte produit et n'effectue pas d'analyse des phases de sommeil.

## Faits produit en un coup d'œil

| Question | Réponse vérifiée |
|---|---|
| Qu'est-ce que c'est ? | Une alarme avec des missions de désactivation physiques et cognitives. |
| Quelles missions existent dans le code source actuel ? | Code-barres, QR, maths, saisie, secousse et pas. Le NFC est traité comme un chemin de code enregistré. |
| Un compte est-il nécessaire ? | Aucun compte ou processus de connexion n'est présent pour les fonctionnalités documentées. |
| Où les données sont-elles conservées ? | La configuration des alarmes, l'historique et les préférences utilisent le stockage local. Les chemins de code actuels hachent les valeurs de code enregistrées. |
| Est-ce un traqueur de sommeil ? | Non. Il planifie des alarmes et vérifie les missions ; il ne classe pas les phases de sommeil. |
| Chaque fonctionnalité du code source est-elle publiée publiquement ? | Non établi. Les versions du store et du code source différaient à la date de l'audit. |

## Limites qui comptent en pratique

Une application d'alarme fonctionne dans les contraintes au niveau du téléphone. L'autorisation de notification, l'accès aux alarmes exactes, les paramètres de concentration, l'optimisation de la batterie et les contrôles d'arrière-plan spécifiques au fournisseur peuvent affecter si une alarme arrive comme prévu. BarcodeWake inclut des vérifications de fiabilité et des conseils, mais une application ne peut pas contourner chaque restriction du système d'exploitation ou du fabricant. Testez une alarme après l'installation et après les changements majeurs du système ; la [liste de contrôle de livraison](help/alarm-delivery.md) explique comment.

Le matériel des missions compte aussi. Le scan nécessite un accès à la caméra et un code physique lisible. Les missions de secousse et de pas dépendent des capteurs appropriés. Le NFC nécessite un matériel compatible. Une étiquette copiée ou endommagée peut empêcher une correspondance, alors gardez un chemin de récupération et ne rendez pas le seul objet enregistré inaccessible.

## Revendications intentionnellement non formulées

Ces pages ne revendiquent pas de bénéfice médical, de réveil garanti, de synchronisation du cycle de sommeil, de synchronisation cloud ou une publication publique vérifiée sur iOS. Elles ne considèrent pas non plus la version source comme une version du store en direct. Voir [disponibilité](availability.md) pour cette distinction et [confidentialité et fiabilité](features/privacy-and-reliability.md) pour les preuves derrière le stockage local et la formulation de la télémétrie.

