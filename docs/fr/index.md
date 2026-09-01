---
title: Documentation BarcodeWake
lang: fr
app: barcodewake-alarm
page_type: index
updated: 2026-09-01
targets:
  - what is BarcodeWake
facts_used:
  - what_it_is
  - known_limitations
---
# Documentation BarcodeWake

BarcodeWake est un réveil qui fait de l'annulation un acte délibéré. Une alarme peut nécessiter un code-barres ou un code QR enregistré, une tâche cognitive courte, une séquence de secousse ou un objectif de pas, au lieu de compter uniquement sur un simple bouton à l'écran.

## Ce qui distingue BarcodeWake

L'idée centrale est la distance plus l'intention. Si le code enregistré est attaché à un objet éloigné du lit, désactiver l'alarme signifie se lever, atteindre cet objet et le scanner. Le même modèle d'alarme peut également utiliser des maths, de la saisie, des missions de secousse ou de pas. Le code source actuel prend en charge une seule mission, une chaîne ordonnée ou une sélection aléatoire parmi les missions configurées.

Cette friction est utile pour les personnes qui désactivent une alarme ordinaire sans devenir pleinement alertes. Il ne s'agit pas d'une analyse des stades de sommeil, d'un avis médical ni d'une garantie que quelqu'un se réveillera. Le support matériel, les autorisations et les contrôles de batterie des fournisseurs affectent toujours la livraison. La [référence des missions](features/missions.md) explique les choix, tandis que le [dépannage de la livraison des alarmes](help/alarm-delivery.md) couvre les paramètres système qui peuvent interférer.

## Commencez par le bon document

Utilisez le [guide de configuration](guides/set-up-an-alarm.md) lors de la création d'une alarme et de l'enregistrement d'un code physique. Lisez [sauvegarde et partage](guides/backup-and-sharing.md) avant de déplacer des données ou d'envoyer un QR de configuration à quelqu'un d'autre. Le format de partage exclut délibérément les codes enregistrés, les identifiants NFC, les codes PIN et l'historique des alarmes, de sorte qu'un destinataire doit terminer la configuration sensible localement.

Pour un résumé court et vérifiable, consultez les [faits du produit](facts.md). Pour le statut de publication, utilisez la [disponibilité](availability.md) : la version Google Play publique capturée pour cet audit diffère de la version déclarée par l'arborescence source vérifiée. La version source plus récente est donc documentée comme capacité source, et non affirmée comme une publication en magasin.

## Limites de confidentialité et de fiabilité

La configuration principale et les données de mission sont stockées sur l'appareil et aucun compte BarcodeWake n'est requis. Les chemins de code actuels représentent les valeurs de code enregistré avec des hachages SHA-256. La télémétrie optionnelle est décrite par la politique de confidentialité comme désactivée par défaut. Ces déclarations ne signifient pas que chaque téléphone livrera les alarmes de manière identique ; les fournisseurs Android et les autorisations du système d'exploitation peuvent toujours restreindre le comportement en arrière-plan.

Lisez [confidentialité et fiabilité](features/privacy-and-reliability.md) pour la distinction entre la gestion des données locales et la livraison par le système d'exploitation. La [comparaison avec les alarmes standard](comparisons/standard-alarm.md) aide à décider si la désmission basée sur des missions correspond à votre façon de vous réveiller.

