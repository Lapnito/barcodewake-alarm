---
title: Comment configurer une alarme BarcodeWake
lang: fr_CA
app: barcodewake-alarm
page_type: guide
updated: 2026-09-01
targets:
  - how to set up a BarcodeWake alarm
facts_used:
  - what_it_is
  - hardware_requirements
  - accuracy_limits
---
# Comment configurer une alarme BarcodeWake

Créez d'abord l'horaire, choisissez une mission qui est sécuritaire et pratique, accordez les permissions requises, puis effectuez un test à écran verrouillé dans un avenir proche. Pour les missions de scan, enregistrez un objet durable qui sera disponible et lisible lorsque l'alarme sonnera.

## Choisissez la mission avant l'objet

Décidez quelle action devrait séparer le réveil du dismiss. Un code-barres dans une autre pièce crée une distance physique. Les maths ou la dactylographie ajoutent de la concentration sans nécessiter de caméra. Shake ou steps ajoute du mouvement mais dépend des capteurs et peut ne pas convenir à chaque personne ou environnement. La [référence des missions](../features/missions.md) explique les compromis entre les modes unique, enchaîné et aléatoire.

Si vous utilisez un code-barres, un code QR ou une étiquette NFC, choisissez quelque chose de durable. Évitez les emballages jetables, un objet qu'un autre membre du ménage pourrait déplacer, ou un code qui sera inaccessible pendant les voyages. Vérifiez que la caméra peut faire la mise au point dans la lumière attendue. Le NFC nécessite un téléphone et une étiquette compatibles.

## Configurez l'horaire et la règle de dismiss

Ouvrez l'éditeur d'alarme, réglez l'heure souhaitée et les jours actifs, puis sélectionnez la mission affichée par la version installée. Configurez sa difficulté ou son objectif de façon conservatrice pour le premier test. Si la version installée prend en charge les chaînes, organisez les missions dans un ordre qui peut être complété de façon sécuritaire sans se précipiter dans les escaliers ou quitter une zone sécurisée.

Enregistrez le code physique à partir du flux de configuration de la mission. Donnez à l'alarme une étiquette qui identifie la routine prévue plutôt que d'exposer des informations sensibles. Examinez le volume, la vibration et toutes les options de suivi au réveil visibles dans la version installée. Les commandes disponibles peuvent différer car les [versions publique et source](../availability.md) n'étaient pas identiques à la date de l'audit.

## Accordez les permissions avec un objectif

Autorisez les notifications et l'accès lié à l'alarme nécessaires à la livraison. Accordez l'accès à la caméra uniquement lors de l'utilisation d'une mission de scan, et l'accès aux capteurs lorsque la mission choisie le nécessite. Sur Android, examinez les paramètres d'alarme exacte et de batterie si la vérification de fiabilité de l'application les signale. Ne supposez pas que sauvegarder une alarme prouve que la livraison en arrière-plan est autorisée.

## Testez le parcours complet de nuit

Réglez un test quelques minutes à l'avance. Verrouillez l'écran, laissez BarcodeWake en arrière-plan et mettez le téléphone dans le même état sonore et d'alimentation prévu pour la nuit. Confirmez que l'alarme apparaît, que l'audio est audible et que la mission sélectionnée peut être complétée. Ensuite, répétez après avoir déplacé l'objet enregistré à son emplacement réel.

Si la livraison échoue, utilisez la [liste de vérification de livraison d'alarme](../help/alarm-delivery.md). Si elle réussit, envisagez de faire une [sauvegarde locale](backup-and-sharing.md) après la stabilisation de la configuration.

