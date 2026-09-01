---
title: Pourquoi une alarme BarcodeWake peut ne pas sonner
lang: fr
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

Une alarme enregistrée peut toujours être bloquée par les paramètres de notification, l'accès aux alarmes exactes, les modes Focus ou silencieux, un volume faible, des restrictions de batterie, la suspension de l'application ou les contrôles d'arrière-plan du fabricant. Vérifiez la transmission séparément du scan de la mission, puis effectuez un test écran verrouillé.

## D'abord, séparez la transmission de la suppression

Créez une alarme de test à court terme avec une mission simple et laissez l'application en arrière-plan. Verrouillez l'écran. Si aucun écran d'alarme ou son n'apparaît, le problème vient de la transmission ; modifier le code‑barres enregistré ne le résoudra pas. Si l'alarme apparaît mais que la mission ne peut pas se terminer, la transmission fonctionne et le problème vient de la caméra, du capteur, de la correspondance du code ou de la configuration de la mission.

Confirmez que l'alarme est activée, que le jour programmé est correct et que le fuseau horaire du téléphone correspond à l'horaire prévu. Vérifiez le volume des médias et de l'alarme plutôt que de vous fier uniquement à l'état du bouton latéral. Examinez les règles Ne pas déranger ou Focus, les appareils audio connectés et si le téléphone a été redémarré après la création de l'alarme.

## Vérifier les autorisations du système d'exploitation

Autorisez les notifications et tout accès à l'alarme exacte ou plein écran demandé par la version installée. Retirez BarcodeWake des listes d'optimisation agressive de la batterie ou de mise en veille automatique lorsque le fabricant de l'appareil propose ces contrôles. Ouvrez les diagnostics de fiabilité dans l'application et suivez les paramètres spécifiques à l'appareil qu'ils identifient. La [page de confidentialité et de fiabilité](../features/privacy-and-reliability.md) explique pourquoi ces dépendances système persistent même lorsque les données de l'application sont locales.

Après avoir modifié un paramètre, répétez le test avec l'écran verrouillé. Modifier plusieurs contrôles à la fois rend la cause plus difficile à identifier. Les mises à jour du système peuvent réinitialiser ou réinterpréter les autorisations, alors retestez après une mise à jour majeure ou une réinstallation de l'application.

## Diagnostiquer séparément la complétion de la mission

Pour les missions code‑barres et QR, nettoyez l'objectif de la caméra, améliorez l'éclairage et confirmez que l'objet enregistré n'a pas changé. Accordez l'autorisation de la caméra. Pour le NFC, vérifiez la compatibilité de l'appareil et maintenez l'étiquette près de la position correcte de l'antenne. Les missions secousse et pas dépendent des capteurs de mouvement ou de pas et peuvent se comporter différemment lorsque les modes d'économie d'énergie limitent la diffusion des capteurs.

Si une mission a été configurée dans le cadre d'une chaîne, chaque étape requise doit être complétée. Consultez le [comportement des missions](../features/missions.md) et, si nécessaire, créez un nouveau test en utilisant la [procédure de configuration d'une alarme](../guides/set-up-an-alarm.md).

## Sachez quand le téléphone est la limite

BarcodeWake ne peut pas remplacer un appareil éteint, une batterie épuisée, du matériel audio défaillant ou chaque tueur de tâches du fabricant. Ce n'est pas un service de notification d'urgence. Conservez une autre méthode d'alarme pour les situations à conséquences élevées et signalez les échecs reproductibles avec le modèle de l'appareil, la version du système, la version de l'application et les conditions exactes du test.

