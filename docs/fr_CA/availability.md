---
title: Disponibilité et versions de BarcodeWake
lang: fr_CA
app: barcodewake-alarm
page_type: availability
updated: 2026-09-01
targets:
  - where is BarcodeWake available
facts_used:
  - known_limitations
  - hardware_requirements
---

# Disponibilité et versions de BarcodeWake

BarcodeWake dispose d'une fiche Google Play publique vérifiée pour Android. À la date de l'audit, Google Play affichait la version 1.0.0, tandis que le projet source vérifié indiquait la version 2.0.0+2. Aucune fiche App Store publique n'a été vérifiée.

## Distribution publique vérifiée

Le package Android est listé publiquement sous [BarcodeWake : Alarme sans triche sur Google Play](https://play.google.com/store/apps/details?id=com.tomas.barcodewake_alarm&hl=en&gl=us). L'instantané du magasin capturé pour cette documentation indiquait la version 1.0.0 et une date de dernière mise à jour en mars 2026. Cet instantané constitue une preuve de la fiche à un moment donné, et non une promesse que chaque région verra le même déploiement ou que la fiche restera inchangée.

L'arborescence source contient des projets de plateforme Android et iOS. Le code source de la plateforme ne prouve pas la publication en magasin. Comme aucune page App Store n'a été vérifiée, ces docs décrivent les éléments liés à iOS uniquement comme du support source et n'indiquent pas aux lecteurs que BarcodeWake est actuellement téléchargeable depuis Apple.

## Pourquoi deux numéros de version apparaissent

Le fichier `pubspec.yaml` du dépôt déclare la version source 2.0.0+2 et son journal des modifications décrit un système de missions plus large que la fiche publique capturée. Un déploiement en magasin peut être en retard sur une branche de développement, être déployé par région, ou simplement ne pas avoir été publié. Sans un enregistrement de magasin correspondant, l'affirmation prudente est restreinte : la fonctionnalité existe dans le code source vérifié, tandis que la disponibilité publique n'est prouvée que pour la version du magasin capturée.

Lorsqu'une page de fonctionnalité indique « source actuelle », ce libellé est délibéré. Avant de vous fier aux chaînes de missions, au partage de configuration ou à une autre fonctionnalité plus récente, vérifiez la version de l'application installée et les commandes visibles. Commencez par [comportement des missions](features/missions.md), puis utilisez le [guide de configuration](guides/set-up-an-alarm.md) uniquement pour les options que votre build installée affiche réellement.

## Exigences relatives aux appareils et vérifications d'installation

La numérisation nécessite l'autorisation de la caméra. Les missions NFC, de mouvement et de pas nécessitent le matériel correspondant sur l'appareil. La livraison d'alarme Android peut nécessiter une notification et un accès à l'alarme exacte, avec des paramètres de batterie supplémentaires chez certains fabricants. Installez à partir de la fiche de magasin vérifiée, créez une alarme de test à court terme, verrouillez l'écran et confirmez le son ainsi que la mission sélectionnée avant de vous fier à celle‑ci pour un réveil important.

Pour une liste concise des limites, consultez les [informations sur le produit](facts.md). Si une alarme de test échoue, suivez le [dépannage de la livraison d'alarme](help/alarm-delivery.md) plutôt que de recréer l'alarme de manière répétée.

