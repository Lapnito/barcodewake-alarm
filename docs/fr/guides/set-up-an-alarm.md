---
title: Comment configurer une alarme BarcodeWake
lang: fr
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

Créez d'abord la planification, choisissez une mission qui est sûre et pratique, accordez les permissions requises, puis effectuez un test à court terme sur écran verrouillé. Pour les missions de scan, enregistrez un objet durable qui sera disponible et lisible au moment où l'alarme sonne.

## Choisissez la mission avant l'objet

Décidez quelle action doit distinguer le réveil de la désactivation. Un code-barres dans une autre pièce crée une distance physique. Les maths ou la saisie ajoutent de la concentration sans nécessiter de caméra. Secouer ou les pas ajoutent du mouvement mais dépendent des capteurs et peuvent ne pas convenir à chaque personne ou environnement. La [référence des missions](../features/missions.md) explique les compromis entre les modes unique, en chaîne et aléatoire.

Si vous utilisez un code-barres, un code QR ou une étiquette NFC, choisissez quelque chose de durable. Évitez les emballages jetables, un objet qu'un autre membre du ménage pourrait déplacer, ou un code qui sera inaccessible pendant les voyages. Vérifiez que la caméra peut faire la mise au point dans la lumière attendue. Le NFC nécessite un téléphone et une étiquette compatibles.

## Configurez la planification et la règle de désactivation

Ouvrez l'éditeur d'alarme, réglez l'heure souhaitée et les jours actifs, puis sélectionnez la mission affichée par la version installée. Configurez sa difficulté ou son objectif de manière conservatrice pour le premier test. Si la version installée prend en charge les chaînes, organisez les missions dans un ordre qui peut être terminé en toute sécurité sans se précipiter dans les escaliers ou quitter une zone sécurisée.

Enregistrez le code physique à partir du flux de configuration de la mission. Donnez à l'alarme une étiquette qui identifie la routine prévue plutôt que d'exposer des informations sensibles. Vérifiez le volume, la vibration et toutes les options de suivi de réveil visibles dans la version installée. Les contrôles disponibles peuvent différer car les [versions publique et source](../availability.md) n'étaient pas identiques à la date de l'audit.

## Accordez les permissions avec un objectif

Autorisez les notifications et l'accès lié à l'alarme nécessaire à la livraison. Accordez l'accès à la caméra uniquement lors de l'utilisation d'une mission de scan, et l'accès aux capteurs lorsque la mission choisie le nécessite. Sur Android, vérifiez les paramètres d'alarme exacte et de batterie si la vérification de fiabilité de l'application les signale. Ne supposez pas que sauvegarder une alarme prouve que la livraison en arrière-plan est autorisée.

## Testez le parcours complet de nuit

Réglez un test quelques minutes à l'avance. Verrouillez l'écran, laissez BarcodeWake en arrière-plan et mettez le téléphone dans le même état sonore et d'alimentation prévu pour la nuit. Confirmez que l'alarme apparaît, que l'audio est audible et que la mission sélectionnée peut être complétée. Ensuite, répétez après avoir déplacé l'objet enregistré vers son emplacement réel.

Si la livraison échoue, utilisez la [liste de contrôle de livraison d'alarme](../help/alarm-delivery.md). Si elle réussit, envisagez de faire une [sauvegarde locale](backup-and-sharing.md) une fois la configuration stable.

