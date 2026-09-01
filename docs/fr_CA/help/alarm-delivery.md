---
title: Pourquoi une alarme BarcodeWake peut ne pas sonner
lang: fr_CA
app: barcodewake-alarm
page_type: help
updated: 2026-09-01
targets:
  - why did my BarcodeWake alarm not ring
facts_used:
  - accuracy_limits
  - hardware_requirements
  - known_limitations
---
# Pourquoi une alarme BarcodeWake peut ne pas sonner

Une alarme enregistrée peut toujours être bloquée par les paramètres de notification, l'accès aux alarmes précises, les modes Ne pas déranger ou silencieux, un volume faible, les restrictions de batterie, la suspension de l'application ou les contrôles en arrière-plan du fabricant. Vérifiez la réception séparément du balayage de mission, puis effectuez un test sur écran verrouillé.

## D'abord isoler la réception de la notification

Créez une alarme de test à court terme avec une mission simple et laissez l'application en arrière-plan. Verrouillez l'écran. Si aucun écran d'alarme ou son n'apparaît, le problème vient de la réception; modifier le code-barres enregistré ne le corrigera pas. Si l'alarme apparaît mais que la mission ne peut pas se terminer, la réception fonctionne et le problème vient de la caméra, du capteur, de la correspondance du code ou de la configuration de la mission.

Confirmez que l'alarme est activée, que le jour programmé est correct et que le fuseau horaire du téléphone correspond à l'horaire prévu. Vérifiez le volume des médias et de l'alarme plutôt que de vous fier uniquement à l'état du bouton latéral. Examinez les règles Ne pas déranger ou de concentration, les appareils audio connectés et si le téléphone a été redémarré après la création de l'alarme.

## Examiner les permissions du système d'exploitation

Autorisez les notifications et tout accès aux alarmes précises ou plein écran demandé par la version installée. Retirez BarcodeWake des listes d'optimisation agressive de la batterie ou de mise en veille automatique lorsque le fabricant de l'appareil propose ces contrôles. Ouvrez les diagnostics de fiabilité dans l'application et suivez les paramètres spécifiques à l'appareil qu'ils identifient. La [page sur la confidentialité et la fiabilité](../features/privacy-and-reliability.md) explique pourquoi ces dépendances système subsistent même lorsque les données de l'application sont locales.

Après avoir modifié un paramètre, répétez le test sur écran verrouillé. Modifier plusieurs contrôles à la fois rend la cause plus difficile à identifier. Les mises à jour système peuvent réinitialiser ou réinterpréter les permissions, alors refaites le test après une mise à jour majeure ou une réinstallation de l'application.

## Diagnostiquer l'exécution de la mission séparément

Pour les missions de codes-barres et de codes QR, nettoyez l'objectif de la caméra, améliorez l'éclairage et confirmez que l'objet enregistré n'a pas changé. Accordez la permission de la caméra. Pour le NFC, vérifiez la prise en charge de l'appareil et maintenez l'étiquette près de la position d'antenne correcte. Les missions de secousse et de pas dépendent des capteurs de mouvement ou de pas et peuvent se comporter différemment lorsque les modes d'économie d'énergie limitent la transmission des capteurs.

Si une mission a été configurée dans le cadre d'une chaîne, chaque étape requise doit se terminer. Examinez le [comportement des missions](../features/missions.md) et, si nécessaire, créez un nouveau test en utilisant la [procédure de configuration](../guides/set-up-an-alarm.md).

## Savoir quand le téléphone est la limite

BarcodeWake ne peut pas remplacer un appareil éteint, une batterie épuisée, du matériel audio brisé ou chaque tueur de tâches de fabricant. Ce n'est pas un service de notification d'urgence. Gardez une autre méthode d'alarme pour les situations à fortes conséquences et signalez les échecs reproductibles avec le modèle de l'appareil, la version du système, la version de l'application et les conditions exactes du test.

