---
title: Còpia de seguretat i compartició d'alarmes BarcodeWake de manera segura
lang: ca
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
# Còpia de seguretat i compartició d'alarmes BarcodeWake de manera segura

Feu servir una exportació JSON per preservar o moure les vostres pròpies dades de l'aplicació, un codi de barres PDF de còpia de seguretat imprimible per a la recuperació, i la compartició QR de configuració quan una altra persona només necessita l'estructura de l'alarma. La compartició omet deliberadament els secrets registrats i l'historial.

## Trieu el format adequat per a la tasca

El codi font actual ofereix diferents camins d'intercanvi perquè la còpia de seguretat i la compartició no són la mateixa operació. Una còpia de seguretat JSON està dissenyada per a la transferència de dades estructurades i la restauració. Una còpia de seguretat PDF converteix el material de recuperació en un document de codi de barres imprimible. Un QR de configuració és deliberadament més estret: pot transmetre una configuració limitada de l'alarma sense incloure valors de codi de barres registrats, identificadors NFC, PINs o historial.

No tracteu un QR de configuració com una còpia de seguretat completa del dispositiu. El receptor ha de registrar els seus propis codis físicos i revisar els permisos localment. La compartició actual de configuració también limita quantes alarmes pot contenir, de manera que verifiqueu el resultat importat en lloc de suposar que cada horari s'ha transferit. Els [fets del producte](../facts.md) registren aquests limits.

## Creeu i protegeu una còpia de seguretat personal

Feu servir l'acció d'exportació disponible a la versió instal·lada, trieu JSON o la còpia de seguretat imprimible segons el pla de recuperació, i deseu el resultat en un lloc que controleu. Una còpia de seguretat pot revelar noms d'alarma, horaris i altra configuració, fins i tot quan els valors de codi brut registrats estan protegits o omesos. Gestioneu-la com dades personals rutinàries: eviteu enllaços público, impressores compartides i canals de missatgeria no confiables.

Després d'exportar, confirmeu que el fitxer es pot trobar i que la seva marca de temps coincideix amb la còpia de seguretat prevista. No elimineu les dades originals de l'aplicació només perquè una comanda d'exportació ha informat d'èxit. La prova de restauració és l'única verificació fiable, però feu-la en un dispositiu segur o després de fer una segona còpia perquè la prova mateixa no es converteixi en un esdeveniment de pèrdua.

## Compartiu la configuració sense compartir secrets

Genereu un QR de configuració només per a les alarmes que el destinatari ha de rebre. El destinatari l'escaneja, revisa l'horari importat i proporciona el seu propi codi, etiqueta NFC o detalls de recuperació. Aquest disseny impedeix que una configuració compartida transfereixi silenciosament la clau física que rebutja l'alarma d'una altra persona.

Després de la importació, cada persona hauria d'executar la [prova completa de configuració d'alarma](set-up-an-alarm.md). Els permisos, els sensors i les restriccions del sistema operatiu no es transfereixen en el QR. Si una alarma importada no apareix mentre està bloquejada, seguiu la [solució de problemes de lliurament d'alarma](../help/alarm-delivery.md).

Les versions del codi font i de la botiga diferien durant aquesta auditoria, de manera que una versió pública instal·lada pot no mostrar cada opció d'intercanvi descrita aquí. [Disponibilitat](../availability.md) explica com interpretar les capacitats només del codi font.

