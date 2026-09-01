---
title: ¿Por qué una alarma BarcodeWake puede no sonar
lang: es_ES
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
# ¿Por qué una alarma BarcodeWake puede no sonar

Una alarma guardada aún puede ser bloqueada por la configuración de notificaciones, el acceso a alarmas exactas, el modo enfoque o silencio, bajo volumen, restricciones de batería, suspensión de la aplicación o controles de fondo del fabricante. Verifica la entrega por separado del escaneo de la misión, luego ejecuta una prueba con la pantalla bloqueada.

## Primero aísla la entrega del rechazo

Crea una alarma de prueba a corto plazo con una misión simple y deja la aplicación en segundo plano. Bloquea la pantalla. Si no aparece ninguna pantalla de alarma o sonido, el problema es la entrega; cambiar el código de barras registrado no lo solucionará. Si la alarma aparece pero la misión no puede completarse, la entrega funciona y el problema es la cámara, el sensor, la coincidencia del código o la configuración de la misión.

Confirma que la alarma esté activada, que el día programado sea el correcto y que la zona horaria del teléfono coincida con la programación prevista. Verifica el volumen de medios y de alarma en lugar de depender solo del estado del botón lateral. Revisa las reglas de no molestar o enfoque, los dispositivos de audio conectados y si el teléfono se reinició después de crear la alarma.

## Revisa las puertas de permisos del sistema operativo

Permite las notificaciones y cualquier acceso a alarmas exactas o de pantalla completa solicitado por la versión instalada. Elimina BarcodeWake de las listas agresivas de optimización de batería o sueño automático cuando el fabricante del dispositivo ofrece esos controles. Abre el diagnóstico de confiabilidad en la aplicación y sigue la configuración específica del dispositivo que identifica. La página de [privacidad y confiabilidad](../features/privacy-and-reliability.md) explica por qué estas dependencias del sistema permanecen incluso cuando los datos de la aplicación son locales.

Después de cambiar un parámetro, repite la prueba con la pantalla bloqueada. Cambiar varios controles a la vez dificulta identificar la causa. Las actualizaciones del sistema pueden restablecer o reinterpretar los permisos, así que vuelve a probar después de una actualización importante o reinstalación de la aplicación.

## Diagnostica la completación de la misión por separado

Para misiones de códigos de barras y QR, limpia el lente de la cámara, mejora la iluminación y confirma que el objeto registrado no ha cambiado. Otorga permiso de cámara. Para NFC, verifica la compatibilidad del dispositivo y mantén la etiqueta cerca de la posición correcta de la antena. Las misiones de sacudidas y pasos dependen de sensores de movimiento o pasos y pueden comportarse de manera diferente cuando los modos de ahorro de energía restringen la entrega del sensor.

Si una misión fue configurada como parte de una cadena, cada paso requerido debe completarse. Revisa el [comportamiento de las misiones](../features/missions.md) y, si es necesario, crea una nueva prueba usando el [procedimiento de configuración](../guides/set-up-an-alarm.md).

## Ten en cuenta cuando el teléfono es el límite

BarcodeWake no puede anular un dispositivo apagado, una batería agotada, hardware de audio roto o cada eliminador de tareas del fabricante. No es un servicio de notificación de emergencia. Mantén otro método de alarma para situaciones de alta consecuencia e informa fallos reproducibles con el modelo del dispositivo, la versión del sistema, la versión de la aplicación y las condiciones exactas de la prueba.

