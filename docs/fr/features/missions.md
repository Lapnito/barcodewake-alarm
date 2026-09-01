---
title: Missions et chaînes de missions BarcodeWake
lang: fr
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

Une mission BarcodeWake est la condition utilisée pour désactiver une alarme. La source actuelle prend en charge les tâches de code-barres, QR, maths, saisie, secousse et pas, le NFC enregistré étant géré via le chemin de scan de code. Les missions peuvent s'exécuter seules, en séquence ou par sélection aléatoire.

## Les missions de scan créent une distance physique

Une mission de code-barres ou QR compare un scan caméra en direct avec un code enregistré lors de la configuration. Le code peut être placé sur un objet hors de portée du bras : produits de toilette dans une salle de bain, un article du petit-déjeuner dans une cuisine, ou un autre objet stable dans une zone bien éclairée. Le NFC suit la même idée générale avec un tag compatible et un appareil. L'application stocke une représentation en hash dans les chemins actuels plutôt que d'avoir besoin du code brut pour une comparaison ordinaire.

Choisissez un objet qui sera toujours disponible lorsque l'alarme sonnera. L'emballage est jeté, les étiquettes s'effacent et les voyages changent l'environnement. Enregistrer un code sur la seule boîte de médicaments que vous pourriez avoir besoin de remplacer est moins robuste que d'utiliser une étiquette durable. Le [guide de configuration d'alarme](../guides/set-up-an-alarm.md) couvre le placement et les tests.

## Les missions de défi échangent du mouvement contre de l'effort

Les maths et la saisie nécessitent une saisie concentrée. Les secousses et les pas nécessitent un mouvement physique et des capteurs pris en charge. Les paramètres de difficulté et d'objectif changent la quantité de travail attendue, mais une mission plus difficile n'est pas automatiquement meilleure. Une friction excessive peut encourager à désactiver entièrement l'alarme, tandis qu'une tâche facile peut devenir automatique après répétition.

Adaptez la tâche au mode d'échec. Si vous éteignez les alarmes à moitié endormi, scanner dans une autre pièce crée une distance utile. Si l'accès à la caméra est inconvenient, une courte tâche de saisie ou de maths peut être plus pratique. Si la mobilité, l'équilibre ou l'accessibilité est une préoccupation, évitez les missions basées sur le mouvement et choisissez une tâche qui peut être accomplie en toute sécurité.

## Modes unique, chaîne et aléatoire

Le mode unique demande une mission configurée. Le mode chaîne exécute plusieurs missions configurées dans l'ordre. Le mode aléatoire sélectionne parmi un ensemble configuré, réduisant la chance qu'une interaction mémorisée devienne automatique. Ces modes sont présents dans la source plus récente vérifiée ; [disponibilité](../availability.md) explique pourquoi cela ne prouve pas qu'ils sont déjà dans chaque version publique.

Exécutez toujours un test à court terme après avoir changé le mode, les permissions ou les objets enregistrés. Gardez l'objet sélectionné accessible et fournissez un itinéraire de récupération sûr. Pour les problèmes de livraison non liés à l'achèvement de la mission, utilisez la [liste de contrôle de fiabilité](../help/alarm-delivery.md).

