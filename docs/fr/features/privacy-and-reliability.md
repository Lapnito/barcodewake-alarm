---
title: BarcodeWake : vie privée et fiabilité des alarmes
lang: fr
app: barcodewake-alarm
page_type: feature
updated: 2026-09-01
targets:
  - is BarcodeWake private and reliable
facts_used:
  - offline
  - account_required
  - ads_tracking
  - data_storage
  - accuracy_limits
---
# BarcodeWake : vie privée et fiabilité des alarmes

BarcodeWake conserve la configuration documentée des alarmes et les données de mission sur l'appareil et ne nécessite aucun compte d'application. Les chemins de code actuels hachent les valeurs de code enregistrées. La télémétrie optionnelle est décrite comme désactivée par défaut, tandis que la livraison des alarmes dépend toujours des autorisations système et des contrôles du fournisseur.

## Les données locales n'éliminent pas les dépendances système

Le stockage local signifie que la configuration habituelle des alarmes ne nécessite pas de compte cloud BarcodeWake. Les enregistrements d'alarmes, l'historique et les préférences sont gérés via la couche de données locale de l'application. Les valeurs de codes-barres, QR et NFC enregistrées sont représentées par des hashages SHA-256 dans les chemins de stockage et d'importation actuels, ce qui évite de conserver la valeur brute ordinaire pour la correspondance.

Le hachage n'est pas équivalent au chiffrement de chaque enregistrement de l'application, et le stockage local n'est pas une sauvegarde. Quelqu'un ayant accès à un appareil déverrouillé peut toujours voir les noms d'alarmes, les horaires ou l'historique via l'application. Un téléphone perdu ou réinitialisé peut également perdre les données locales, sauf si l'utilisateur a effectué une exportation. Consultez [sauvegarde et partage](../guides/backup-and-sharing.md) pour les formats et leurs différents usages.

La politique de confidentialité indique que la télémétrie optionnelle est désactivée par défaut et décrit la gestion agrégée si elle est activée. Cette documentation ne fait donc pas l'affirmation plus large que l'application ne peut jamais communiquer sur un réseau. Elle énonce les faits vérifiés plus étroits : le fonctionnement principal et les données sont locaux, aucun compte produit n'est requis, et aucune dépendance de SDK publicitaire n'apparaît dans le projet vérifié.

## La fiabilité est une responsabilité partagée

BarcodeWake peut planifier et présenter une alarme, mais le système d'exploitation décide quand le travail en arrière-plan peut s'exécuter et quelles interruptions sont autorisées. L'autorisation de notification, l'accès aux alarmes exactes, les modes silencieux ou concentration, l'optimisation de la batterie, la suspension automatique de l'application et les tueurs de tâches du fabricant peuvent tous avoir une importance. L'outil de fiabilité intégré à l'application peut identifier les risques de configuration et orienter les utilisateurs vers les paramètres ; il ne peut pas remplacer la politique système.

Après l'installation, testez avec l'écran verrouillé et le téléphone dans le même mode d'alimentation utilisé pendant la nuit. Répétez ce test après une mise à jour système, un changement d'économiseur de batterie ou une réinstallation de l'application. Gardez l'appareil chargé, le volume approprié et la mission choisie physiquement disponible. Consultez [dépannage de la livraison des alarmes](../help/alarm-delivery.md) lorsqu'un test échoue.

## Ce que la vie privée et la fiabilité ne promettent pas

BarcodeWake n'est pas un dispositif médical, un service d'alerte d'urgence ou un tracker de stade de sommeil. Aucune application d'alarme ne peut garantir le réveil ou compenser un appareil indisponible. La [page des faits et limites](../facts.md) liste ces limites, tandis que [disponibilité](../availability.md) sépare les preuves du magasin public des capacités plus récentes du code source.

