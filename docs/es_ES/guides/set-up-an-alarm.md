---
title: Cómo configurar una alarma BarcodeWake
lang: es_ES
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
# Cómo configurar una alarma BarcodeWake

Crea primero la programación, elige una misión que sea segura y práctica, concede los permisos necesarios y, a continuación, realiza una prueba con la pantalla bloqueada a corto plazo. Para las misiones de escaneo, registra un objeto duradero que esté disponible y sea legible cuando suene la alarma.

## Elige la misión antes del objeto

Decide qué acción debe separar el despertar del despido. Un código de barras en otra habitación crea distancia física. Las matemáticas o la escritura añaden concentración sin necesidad de cámara. Agitar o dar pasos añade movimiento, pero depende de los sensores y puede no ser adecuado para todas las personas o entornos. La [referencia de misión](../features/missions.md) explica las ventajas y desventajas entre los modos único, encadenado y aleatorio.

Si usas un código de barras, código QR o etiqueta NFC, elige algo duradero. Evita el embalaje desechable, un objeto que otro miembro del hogar pueda mover o un código que sea inaccesible mientras viajes. Comprueba que la cámara pueda enfocar con la luz esperada. NFC necesita un teléfono y una etiqueta compatibles.

## Configura la programación y la regla de despido

Abre el editor de alarma, establece la hora deseada y los días activos y, a continuación, selecciona la misión mostrada por la versión instalada. Configura su dificultad o objetivo de forma conservadora para la primera prueba. Si la versión instalada permite encadenar, organiza las misiones en un orden que pueda completarse de forma segura sin correr por las escaleras ni salir de un área segura.

Registra el código físico desde el flujo de configuración de la misión. Asigna a la alarma una etiqueta que identifique la rutina prevista en lugar de exponer información sensible. Revisa el volumen, la vibración y cualquier opción de seguimiento tras despertar que sea visible en la versión instalada. Los controles disponibles pueden diferir porque las [versiones pública y de código fuente](../availability.md) no eran idénticas en la fecha de auditoría.

## Concede permisos con un propósito

Permite las notificaciones y el acceso relacionado con la alarma necesarios para la entrega. Concede acceso a la cámara solo cuando utilices una misión de escaneo y acceso al sensor cuando la misión elegida lo requiera. En Android, revisa la configuración de alarma exacta y de batería si la verificación de fiabilidad de la aplicación los señala. No asumas que guardar una alarma demuestra que la entrega en segundo plano esté permitida.

## Prueba la ruta completa durante la noche

Configura una prueba unos minutos antes. Bloquea la pantalla, deja BarcodeWake en segundo plano y pon el teléfono en el mismo estado de sonido y energía previsto para la noche. Confirma que la alarma aparece, el audio es audible y la misión exacta seleccionada puede completarse. Luego repite después de mover el objeto registrado a su ubicación real.

Si la entrega falla, consulta la [lista de verificación de entrega de alarmas](../help/alarm-delivery.md). Si tiene éxito, considera hacer una [copia de seguridad local](backup-and-sharing.md) una vez que la configuración sea estable.

