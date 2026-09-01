---
title: Sauvegarder et partager les alarmes BarcodeWake en toute sécurité
lang: fr_CA
app: barcodewake-alarm
page_type: guide
updated: 2026-09-01
targets:
  - how to back up or share BarcodeWake alarms
facts_used:
  - export_formats
  - data_storage
  - known_limitations
---
# Sauvegarder et partager les alarmes BarcodeWake en toute sécurité

Utilisez une exportation JSON pour conserver ou déplacer vos propres données d'application, un code‑barres de sauvegarde PDF imprimable pour la récupération, et le partage QR de configuration lorsqu'une autre personne n'a besoin que de la structure d'alarme. Le partage omet intentionnellement les secrets enregistrés et l'historique.

## Choisir le format pour la tâche

La source actuelle propose différents chemins d'échange car la sauvegarde et le partage ne sont pas la même opération. Une sauvegarde JSON est destinée au transfert structuré de données et à la restauration. Une sauvegarde PDF transforme le matériel de récupération en un document de code‑barres imprimable. Un QR de configuration est délibérément plus étroit : il peut transmettre une configuration d'alarme limitée sans porter les valeurs de code‑barres enregistrées, les identifiants NFC, les codes PIN ou l'historique.

Ne traitez pas un QR de configuration comme une sauvegarde complète de l'appareil. Le destinataire doit enregistrer ses propres codes physiques et examiner les autorisations localement. Le partage de configuration actuel limite également le nombre d'alarmes qu'il transporte, donc vérifiez le résultat importé plutôt que de supposer que chaque planification a été déplacée. Les [données produit](../facts.md) enregistrent ces limites.

## Créer et protéger une sauvegarde personnelle

Utilisez l'action d'exportation disponible dans la version installée, choisissez JSON ou la sauvegarde imprimable selon le plan de récupération, et enregistrez le résultat quelque part que vous contrôlez. Une sauvegarde peut révéler les noms d'alarmes, les planifications et d'autres configurations même lorsque les valeurs brutes de codes enregistrées sont protégées ou omises. Traitez‑la comme des données personnelles de routine : évitez les liens publics, les imprimantes partagées et les canaux de messagerie non fiables.

Après l'exportation, vérifiez que le fichier peut être trouvé et que son horodatage correspond à la sauvegarde prévue. Ne supprimez pas les données d'application d'origine simplement parce qu'une commande d'exportation a signalé la réussite. Le test de restauration est la seule vérification fiable, mais effectuez‑le sur un appareil sécurisé ou après avoir effectué une seconde copie afin que le test lui‑même ne devienne pas un événement de perte.

## Partager la configuration sans partager les secrets

Générez un QR de configuration uniquement pour les alarmes que le destinataire devrait recevoir. Le destinataire le scanne, examine la planification importée et fournit son propre code, étiquette NFC ou détails de récupération. Cette conception empêche une configuration partagée de transférer silencieusement la clé physique qui désactive l'alarme de quelqu'un d'autre.

Après l'importation, chaque personne doit exécuter le [test complet de configuration d'alarme](set-up-an-alarm.md). Les autorisations, les capteurs et les restrictions du système d'exploitation ne sont pas transférés dans le QR. Si une alarme importée n'apparaît pas lorsqu'elle est verrouillée, consultez le [dépannage de livraison d'alarme](../help/alarm-delivery.md).

Les versions source et du magasin différaient lors de cet audit, de sorte qu'une version publique installée peut ne pas exposer chaque option d'échange décrite ici. [Disponibilité](../availability.md) explique comment interpréter les capacités uniquement disponibles dans la source.

