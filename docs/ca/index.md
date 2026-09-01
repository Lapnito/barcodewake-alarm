---
title: Documentació de BarcodeWake
lang: ca
app: barcodewake-alarm
page_type: index
updated: 2026-09-01
targets:
  - what is BarcodeWake
facts_used:
  - what_it_is
  - known_limitations
---
# Documentació de BarcodeWake

BarcodeWake és un despertador que fa que la interrupció sigui un acte deliberat. Una alarma pot requerir un codi de barres o codi QR desat, una tasca cognitiva breu, una seqüència de sacsejades o un objectiu de passos en lloc de dependre només d'un botó fàcil a la pantalla.

## Què fa diferent BarcodeWake

La idea central és distància més intenció. Si el codi registrat està adjunt a un objecte lluny del llit, silenciar l'alarma significa llevar-se, arribar a aquest objecte i escanejar-lo. El mateix model d'alarma també pot fer servir missions de matemàtiques, escriptura, sacsejades o passos. El codi font actual és compatible amb una única missió, una cadena ordenada o selecció aleatòria de missions configurades.

Aquesta fricció és útil per a persones que interrompen un despertador ordinari sense despertar completament. No és anàlisi d'estat del son, assessorament mèdic ni una garantia que algú es despertarà. El suport de maquinari, els permisos i els controls de bateria del proveïdor encara afecten el lliurament. La [referència de missions](features/missions.md) explica les opcions, mentre que la [solució de problemes de lliurament d'alarma](help/alarm-delivery.md) tracta la configuració del sistema que pot interferir.

## Comenceu amb el document adequat

Feu servir la [guia de configuració](guides/set-up-an-alarm.md) en crear una alarma i registrar un codi física. Llegiu la [còpia de seguretat i compartició](guides/backup-and-sharing.md) abans de moure dades o enviar un QR de configuració a algú altre. El format de compartició deliberadament exclou els codis registrats, identificadors NFC, PINs i historial d'alarmes, de manera que un receptor ha de completar la configuració sensible localment.

Per a un resum curt i auditable, consulteu els [fets del producte](facts.md). Per a l'estat de llançament, feu servir la [disponibilitat](availability.md): la versió pública de Google Play capturada per a aquesta auditoria difereix de la versió declarada per l'arbre de codi font verificat. Per tant, la versió més recent del codi font es documenta com a capacitat del codi font, no s'afirma com a llançament de botiga publicat.

## Límits de privacitat i fiabilitat

La configuració principal i les dades de missió s'emmagatzemen al dispositiu i no es requereix cap compte de BarcodeWake. Els camins de codi actuals representen els valors de codi registrat amb hash SHA-256. La telemetria opcional es descriu a la política de privacitat com a desactivada per defecte. Aquestes declaracions no signifiquen que cada telèfon lliurarà alarmes de manera idèntica; els proveïdors d'Android i els permisos del sistema operatiu encara poden restringir el comportament en segon pla.

Llegiu [privacitat i fiabilitat](features/privacy-and-reliability.md) per a la distinció entre el maneig de dades locals i el lliurament del sistema operatiu. La [comparació de despertador estàndard](comparisons/standard-alarm.md) ajuda a decidir si la interrupció basada en missions coincideix amb la manera com us desperteu.

