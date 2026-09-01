---
title: Missions et chaînes de missions BarcodeWake
lang: fr_CA
app: barcodewake-alarm
page_type: feature
updated: 2026-09-01
targets:
  - how do BarcodeWake missions work
facts_used:
  - what_it_is
  - core_measurement
  - hardware_requirements
  - known_limitations
---

# Missions et chaînes de missions BarcodeWake

Une mission BarcodeWake est la condition utilisée pour désactiver une alarme. La source actuelle prend en charge les tâches de code-barres, QR, maths, saisie, secousse et pas, le NFC enregistré étant traité via le chemin de scan de code. Les missions peuvent s'exécuter seules, en séquence ou par sélection aléatoire.

## Les missions de scan créent une distance physique

Une mission de code-barres ou QR compare un scan de caméra en direct avec un code enregistré lors de la configuration. Le code peut être placé sur un objet hors de portée du bras : produits de toilette dans une salle de bain, un article du petit-déjeuner dans une cuisine ou un autre objet stable dans un endroit bien éclairé. Le NFC suit la même idée générale avec une étiquette et un appareil compatibles. L'application stocke une représentation de hachage dans les chemins actuels plutôt que d'avoir besoin du code brut pour une comparaison ordinaire.

Choisissez un objet qui sera encore disponible quand l'alarme sonnera. L'emballage est jeté, les étiquettes s'effacent et les voyages modifient l'environnement. Enregistrer un code sur la seule boîte de médicaments que vous pourriez avoir à remplacer est moins robuste que d'utiliser une étiquette durable. Le [guide de configuration d'une alarme](../guides/set-up-an-alarm.md) couvre le placement et les tests.

## Les missions de défi échangent le mouvement pour l'effort

Les maths et la saisie nécessitent une concentration. Les secousses et les pas nécessitent un mouvement physique et des capteurs pris en charge. Les paramètres de difficulté et d'objectifs modifient la quantité de travail attendue, mais une mission plus difficile n'est pas automatiquement meilleure. Une friction excessive peut encourager à désactiver complètement l'alarme, tandis qu'une tâche facile peut devenir automatique après répétition.

Adaptez la tâche au mode de défaillance. Si vous éteignez les alarmes à moitié endormi, scanner dans une autre pièce crée une distance utile. Si l'accès à la caméra est incommode, une courte tâche de saisie ou de maths peut être plus pratique. Si la mobilité, l'équilibre ou l'accessibilité est une préoccupation, évitez les missions basées sur le mouvement et choisissez une tâche qui peut être accomplie en toute sécurité.

## Modes solo, en chaîne et aléatoire

Le mode solo demande une mission configurée. Le mode en chaîne exécute plusieurs missions configurées dans l'ordre. Le mode aléatoire choisit dans un ensemble configuré, réduisant la chance qu'une interaction mémorisée devienne automatique. Ces modes sont présents dans la source vérifiée plus récente ; la [disponibilité](../availability.md) explique pourquoi cela ne prouve pas qu'ils sont déjà dans chaque build publique.

Exécutez toujours un test à court terme après avoir changé le mode, les permissions ou les objets enregistrés. Gardez l'objet sélectionné accessible et fournissez un itinéraire de récupération sûr. Pour les problèmes de livraison non liés à la complétion de la mission, utilisez la [liste de contrôle de fiabilité](../help/alarm-delivery.md).

