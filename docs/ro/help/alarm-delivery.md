---
title: De ce o alarmă BarcodeWake poate să nu sune
lang: ro
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
# De ce o alarmă BarcodeWake poate să nu sune

O alarmă salvată poate fi încă blocată de setările de notificări, accesul la alarme exacte, modurile de focalizare sau silențios, volum redus, restricții de baterie, suspendarea aplicației sau controale de fundal ale producătorului. Verificați separat livrarea de scanarea misiunii, apoi efectuați un test cu ecranul blocat.

## Mai întâi izolați livrarea de respingere

Creați o alarmă de test pe termen scurt cu o misiune simplă și lăsați aplicația în fundal. Blocați ecranul. Dacă nu apare niciun ecran sau sunet de alarmă, problema este la livrare; schimbarea codului de bare înregistrat nu va remedia acest lucru. Dacă alarma apare dar misiunea nu poate fi finalizată, livrare funcționează și problema este la cameră, senzor, potrivirea codului sau configurarea misiunii.

Confirmați că alarma este activată, ziua programată este corectă și fusul orar al telefonului corespunde programului prevăzut. Verificați volumul media și alarmei în loc să vă bazați doar pe starea butonului lateral. Revizuiți regulile de nu deranjați sau focalizare, dispozitivele audio conectate și dacă telefonul a fost repornit după crearea alarmei.

## Revizuiți porțile de permisiuni ale sistemului de operare

Permiteți notificările și orice acces la alarme exacte sau alarme pe ecran complet solicitate de versiunea instalată. Eliminați BarcodeWake din listele de optimizare agresivă a bateriei sau de oprire automată când producătorul dispozitivului oferă aceste controale. Deschideți diagnosticele de fiabilitate din aplicație și urmați setările specifice dispozitivului pe care le identifică. Pagina [confidențialitate și fiabilitate](../features/privacy-and-reliability.md) explică de ce aceste dependențe de sistem rămân chiar când datele aplicației sunt locale.

După modificarea unei singure setări, repetați testul cu ecranul blocat. Modificarea mai multor controale simultan face mai dificilă identificarea cauzei. Actualizările de sistem pot reseta sau reinterpretă permisiunile, deci retestați după o actualizare majoră sau reinstalarea aplicației.

## Diagnosticați finalizarea misiunii separat

Pentru misiunile de coduri de bare și QR, curățați obiectivul camerei, îmbunătățiți iluminarea și confirmați că obiectul înregistrat este neschimbat. Acordați permisiunea pentru cameră. Pentru NFC, verificați suportul dispozitivului și țineți eticheta aproape de poziția corectă a antenei. Misiunile de agitare și pași depind de senzorii de mișcare sau pași și pot comporta diferit când modurile de economisire a energiei restricționează livrare senzorilor.

Dacă o misiune a fost configurată ca parte a unui lanț, fiecare pas necesar trebuie finalizat. Revizuiți [comportamentul misiunilor](../features/missions.md) și, dacă este necesar, creați un nou test folosind [procedura de configurare](../guides/set-up-an-alarm.md).

## Știți când telefonul este granița

BarcodeWake nu poate suprascrie un dispozitiv oprit, o baterie epuizată, hardware audio defect sau fiecare instrument de eliminare a sarcinilor producătorului. Nu este un serviciu de notificare de urgență. Păstrați o altă metodă de alarmă pentru situații cu consecințe ridicate și raportați eșecurile reproductibile cu modelul dispozitivului, versiunea sistemului, versiunea aplicației și condițiile exacte de test.

