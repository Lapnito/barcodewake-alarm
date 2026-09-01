---
title: Privacitat i fiabilitat de l'alarma de BarcodeWake
lang: ca
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
# Privacitat i fiabilitat de l'alarma de BarcodeWake

BarcodeWake manté la configuració documentada de l'alarma i les dades de la missió al dispositiu i no requereix cap compte de l'aplicació. Els camins de codi actuals hashen els valors de codi registrats. La telemetria opcional es descriu com a desactivada per defecte, mentre que el lliurament de l'alarma encara depèn dels permisos del sistema i els controls del proveïdor.

## Les dades locals no eliminen les dependències del sistema

L'emmagatzematge local significa que la configuració ordinària de l'alarma no requereix un compte al núvol de BarcodeWake. Els registres d'alarma, l'historial i les preferències es gestionen a través de la capa de dades locals de l'aplicació. Els valors registrats de codi de barres, QR i NFC es representen amb hashes SHA-256 en l'emmagatzematge actual i camins d'importació, cosa que evita retenir el valor cru ordinari per a la coincidència.

El hash no és el mateix que el xifratge de cada registre de l'aplicació, i l'emmagatzematge local no és una còpia de seguretat. Algú amb accés a un dispositiu desbloquejat encara pot veure els noms de les alarmes, els horaris o l'historial a través de l'aplicació. Un telèfon perdut o restablert també pot perdre dades locals tret que l'usuari hagi fet una exportació. Vegeu [còpia de seguretat i compartició](../guides/backup-and-sharing.md) per obtenir informació sobre els formats i els seus propòsits diferents.

La política de privacitat indica que la telemetria opcional està desactivada per defecte i descriu el tractament agregat si està activada. Per tant, aquesta documentació no fa l'afirmació més àmplia que l'aplicació mai no pot comunicar-se per una xarxa. Afirma els fets verificats més estrets: el funcionament central i les dades són locals, no es requereix cap compte de producte i no apareix cap dependència de SDK publicitari al projecte verificat.

## La fiabilitat és una responsabilitat compartida

BarcodeWake pot programar i presentar una alarma, però el sistema operatiu decideix quan es pot executar el treball en segon pla i quines interrupcions es permeten. El permís de notificació, l'accés a l'alarma exacta, els modes silenciosos o de concentració, l'optimització de la bateria, la suspensió automàtica de l'aplicació i els assassins de tasques del fabricant poden ser rellevants. L'eina de fiabilitat dins de l'aplicació pot identificar riscos de configuració i dirigir els usuaris a la configuració; no pot sobreescriure la política del sistema.

Després de la instal·lació, proveu amb la pantalla bloquejada i el telèfon en el mateix mode d'energia utilitzat durant la nit. Repetiu aquesta prova després d'una actualització del sistema, un canvi d'estalvi de bateria o una reinstal·lació de l'aplicació. Mantingueu el dispositiu carregat, el volum adequat i la missió escollida física disponible. Seguiu [solució de problemes de lliurament d'alarmes](../help/alarm-delivery.md) quan una prova falli.

## El que la privacitat i la fiabilitat no garanteixen

BarcodeWake no és un dispositiu mèdic, un servei d'alerta d'emergència ni un tracker d'estadis del son. Cap aplicació d'alarma pot garantir que us despertareu o compensar un dispositiu no disponible. La [pàgina de fets i limitacions](../facts.md) enumera aquestslimits, mentre que [disponibilitat](../availability.md) separa l'evidència de la botiga pública de les capacitats més recents del codi font.

