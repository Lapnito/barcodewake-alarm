---
title: Disponibilité et versions de BarcodeWake
lang: fr
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

BarcodeWake dispose d'une fiche Google Play publique vérifiée pour Android. À la date de l'audit, Google Play affichait la version 1.0.0, tandis que le projet source vérifié déclarait la version 2.0.0+2. Aucune fiche App Store publique n'a été vérifiée.

## Distribution publique vérifiée

Le package Android est listé publiquement sous [BarcodeWake: No Cheat Alarm sur Google Play](https://play.google.com/store/apps/details?id=com.tomas.barcodewake_alarm&hl=en&gl=us). La capture d'écran de la boutique pour cette documentation indiquait la version 1.0.0 et une date de dernière mise à jour en mars 2026. Cette capture est une preuve de la fiche à un instant donné, et non une promesse que chaque région voit le même déploiement ou que la fiche restera inchangée.

L'arborescence source contient des projets de plateforme Android et iOS. Le code source de la plateforme ne prouve pas la publication en boutique. Comme aucune page App Store n'a été vérifiée, ces docs décrivent les éléments liés à iOS comme du support source uniquement et ne indiquent pas aux lecteurs que BarcodeWake est actuellement téléchargeable depuis Apple.

## Pourquoi deux numéros de version apparaissent

Le fichier `pubspec.yaml` du dépôt déclare la version source 2.0.0+2 et son journal des modifications décrit un système de mission plus large que la fiche publique capturée. Un déploiement en boutique peut être en retard sur une branche de développement, être déployé par région, ou simplement ne pas avoir été publié. Sans un enregistrement de boutique correspondant, l'affirmation sûre est étroite : la capacité existe dans le code source vérifié, tandis que la disponibilité publique est prouvée uniquement pour la version de la boutique capturée.

Quand une page de fonctionnalité dit « source actuelle », cette formulation est délibérée. Avant de compter sur des chaînes de mission, le partage de configuration ou une autre capacité plus récente, vérifiez la version de l'application installée et les contrôles visibles. Commencez par [comportement des missions](features/missions.md), puis utilisez le [guide de configuration](guides/set-up-an-alarm.md) uniquement pour les options que votre build installé affiche réellement.

## Exigences des appareils et vérifications d'installation

La numérisation nécessite l'autorisation de la caméra. Les missions NFC, mouvement et pas ont besoin du matériel d'appareil correspondant. La livraison d'alarme Android peut nécessiter l'accès aux notifications et aux alarmes exactes, avec des paramètres de batterie supplémentaires sur certains fabricants. Installez depuis la fiche de boutique vérifiée, créez une alarme de test à court terme, verrouillez l'écran et confirmez à la fois le son et la mission sélectionnée avant de dépendre de celle-ci pour un réveil important.

Pour une liste de limites concise, lisez [faits produit](facts.md). Si une alarme de test échoue, suivez le [dépannage de livraison d'alarme](help/alarm-delivery.md) plutôt que de recréer répétitivement l'alarme.

