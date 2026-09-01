---
title: Cómo configurar una alarma BarcodeWake
lang: es
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

Crea primero el horario, elige una misión que sea segura y práctica, otorga los permisos necesarios y luego ejecuta una prueba con la pantalla bloqueada en el corto plazo. Para las misiones de escaneo, registra un objeto durable que esté disponible y sea legible cuando suene la alarma.

## Elegir la misión antes del objeto

Decide qué acción debe separar el despertar del despido. Un código de barras en otra habitación crea distancia física. Las matemáticas o escribir añaden concentración sin necesidad de cámara. Agitar o dar pasos añade movimiento pero depende de los sensores y puede no ser adecuado para todas las personas o entornos. La [referencia de misiones](../features/missions.md) explica las ventajas y desventajas entre los modos único, encadenado y aleatorio.

Si usas un código de barras, código QR o etiqueta NFC, elige algo duradero. Evita embalajes desechables, un objeto que otro miembro del hogar pueda mover o un código que sea inaccesible mientras viajas. Comprueba que la cámara pueda enfocar con la luz esperada. NFC necesita un teléfono y una etiqueta compatibles.

## Configurar el horario y la regla de despido

Abre el editor de alarma, establece la hora deseada y los días activos, luego selecciona la misión mostrada por la versión instalada. Configura su dificultad o objetivo de manera conservadora para la primera prueba. Si la versión instalada es compatible con encadenamiento, organiza las misiones en un orden que pueda completarse de forma segura sin correr por las escaleras o abandonar un área segura.

Registra el código físico desde el flujo de configuración de la misión. Dale a la alarma una etiqueta que identifique la rutina prevista en lugar de exponer información sensible. Revisa el volumen, la vibración y cualquier opción de seguimiento de despertador visible en la versión instalada. Los controles disponibles pueden diferir porque las [versiones pública y de origen](../availability.md) no eran idénticas en la fecha de auditoría.

## Otorgar permisos con un propósito

Permite las notificaciones y el acceso relacionado con alarmas necesario para la entrega. Otorga acceso a la cámara solo cuando uses una misión de escaneo y acceso a los sensores cuando la misión elegida lo necesite. En Android, revisa la configuración de alarma exacta y batería si la verificación de confiabilidad de la aplicación los marca. No asumas que guardar una alarma demuestra que la entrega en segundo plano está permitida.

## Probar la ruta completa durante la noche

Configura una prueba unos minutos adelante. Bloquea la pantalla, deja BarcodeWake en segundo plano y pon el teléfono en el mismo estado de sonido y energía planeado para la noche. Confirma que la alarma aparece, el audio es audible y la misión exacta seleccionada puede completarse. Luego repite después de mover el objeto registrado a su ubicación real.

Si la entrega falla, usa la [lista de verificación de entrega de alarmas](../help/alarm-delivery.md). Si tiene éxito, considera hacer una [copia de seguridad local](backup-and-sharing.md) después de que la configuración sea estable.

