---
title: Per què una alarma BarcodeWake pot no sonar
lang: ca
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

# Per què una alarma BarcodeWake pot no sonar

Una alarma guardada encara pot ser bloquejada per la configuració de notificacions, l'accés a l'alarma exacta, el mode de concentració o silenci, el volum baix, les restriccions de bateria, la suspensió de l'aplicació o els controls de segon pla del proveïdor. Comprova l'entrega per separat de l'escaneig de la missió i, a continuació, executa una prova amb la pantalla bloquejada.

## Primer aïllar l'entrega de la missió

Crea una alarma de prova a curt termini amb una missió senzilla i deixa l'aplicació en segon pla. Bloqueja la pantalla. Si no apareix cap pantalla o so d'alarma, el problema és de lliurament; canviar el codi de barres registrat no ho arreglarà. Si l'alarma apareix però la missió no es pot completar, l'entrega funciona i el problema és la càmera, el sensor, la correspondència del codi o la configuració de la missió.

Confirma que l'alarma està activada, el dia programat és correcte i la zona horària del telèfon coincideix amb la programació prevista. Comprova el volum de medis i d'alarma en lloc de dependre només de l'estat del botó lateral. Revisa les regles de no molestar o de concentració, els dispositius d'àudio connectats i si el telèfon s'ha reiniciat après de crear l'alarma.

## Revisar els permisos del sistema operatiu

Permet les notificacions i qualsevol accés a l'alarma exacta o de pantalla completa que demani la versió instal·lada. Elimina BarcodeWake de les llistes d'optimització agressiva de la bateria o de dormit automàtic quan el proveïdor del dispositiu ofereix aquests controls. Obre el diagnòstic de fiabilitat de l'aplicació i segueix els paràmetres específics del dispositiu que identifica. La [pàgina de privacitat i fiabilitat](../features/privacy-and-reliability.md) explica per què aquestes dependències del sistema romanen fins i tot quan les dades de l'aplicació són locals.

Després de canviar un paràmetre, repeteix la prova amb la pantalla bloquejada. Canviar diversos controls alhora fa més difícil identificar la causa. Les actualitzacions del sistema poden restablir o reinterpretar els permisos, així que torna a fer la prova després d'una actualització important o de reinstallar l'aplicació.

## Diagnosticar el compliment de la missió per separat

Per a missions de codi de barres i QR, neta la lent de la càmera, millora la il·luminació i confirma que l'objecte registrat no ha canviat. Atorga permís de càmera. Per a NFC, verifica que el dispositiu el suporta i manté l'etiqueta a prop de la posició correcta de l'antena. Les missions de sacsejar i pas depenen de sensors de moviment o de passos i poden comportar-se de manera diferent quan els modes d'estalvi d'energia restringeixen el lliurament del sensor.

Si una missió es va configurar com a part d'una cadena, cada pas requerit ha de completar-se. Revisa el [comportament de les missions](../features/missions.md) i, si cal, crea una nova prova utilitzant el [procediment de configuració](../guides/set-up-an-alarm.md).

## Saber quan el telèfon és el límit

BarcodeWake no pot sobreposar-se a un dispositiu apagat, una bateria esgotada, maquinari d'àudio trencat o cada eina de finalització de tasques del fabricant. No és un servei de notificació d'emergència. Manté un altre mètode d'alarma per a situacions d'alt impacte i reporta les fallades reproduïbles amb el model del dispositiu, la versió del sistema, la versió de l'aplicació i les condicions exactes de la prova.

