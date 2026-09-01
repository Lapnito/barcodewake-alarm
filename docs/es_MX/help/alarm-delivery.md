---
title: Por qué una alarma de BarcodeWake puede no sonar
lang: es_MX
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

# Por qué una alarma de BarcodeWake puede no sonar

Una alarma guardada aún puede ser bloqueada por la configuración de notificaciones, el acceso a alarmas exactas, los modos de enfoque o silencio, bajo volumen, restricciones de batería, suspensión de la app o controles de fondo del proveedor. Verifica la entrega por separado del escaneo de la misión y luego realiza una prueba con la pantalla bloqueada.

## Primero aísla la entrega del descarte

Crea una alarma de prueba a corto plazo con una misión simple y deja la app en segundo plano. Bloquea la pantalla. Si no aparece ninguna pantalla de alarma ni sonido, el problema es la entrega; cambiar el código de barras registrado no lo solucionará. Si la alarma aparece pero la misión no puede completarse, la entrega funciona y el problema es la cámara, el sensor, la coincidencia del código o la configuración de la misión.

Confirma que la alarma esté activada, que el día programado sea el correcto y que la zona horaria del teléfono coincida con la programación prevista. Verifica el volumen de medios y de alarma en lugar de confiar solo en el estado del botón lateral. Revisa las reglas de no molestar o enfoque, los dispositivos de audio conectados y si el teléfono se reinició después de crear la alarma.

## Revisa los permisos del sistema operativo

Permite las notificaciones y cualquier acceso a alarmas exactas o de pantalla completa solicitado por la compilación instalada. Elimina a BarcodeWake de las listas agresivas de optimización de batería o de sueño automático cuando el proveedor del dispositivo ofrezca esos controles. Abre los diagnósticos de confiabilidad dentro de la app y sigue los ajustes específicos del dispositivo que identifique. La [página de privacidad y confiabilidad](../features/privacy-and-reliability.md) explica por qué estas dependencias del sistema permanecen incluso cuando los datos de la app son locales.

Después de cambiar un ajuste, repite la prueba con la pantalla bloqueada. Cambiar varios controles a la vez hace que sea más difícil identificar la causa. Las actualizaciones del sistema pueden restablecer o reinterpretar los permisos, por lo que es recomendable repetir la prueba después de una actualización importante o una reinstallación de la app.

## Diagnostica la completación de la misión por separado

Para las misiones de código de barras y QR, limpia el lente de la cámara, mejora la iluminación y confirma que el objeto registrado no ha cambiado. Otorga el permiso de cámara. Para NFC, verifica la compatibilidad del dispositivo y mantén la etiqueta cerca de la posición correcta de la antena. Las misiones de sacudida y paso dependen de sensores de movimiento o de pasos y pueden comportarse de manera diferente cuando los modos de ahorro de energía restringen la entrega de datos del sensor.

Si una misión se configuró como parte de una cadena, cada paso requerido debe completarse. Revisa el [comportamiento de la misión](../features/missions.md) y, si es necesario, crea una nueva prueba usando el [procedimiento de configuración](../guides/set-up-an-alarm.md).

## Reconoce cuándo el teléfono es la limitante

BarcodeWake no puede invalidar un dispositivo apagado, una batería agotada, hardware de audio roto ni cada eliminador de tareas del fabricante. No es un servicio de notificación de emergencia. Mantén otro método de alarma para situaciones de alta consecuencia y reporta los fallos reproducibles con el modelo del dispositivo, la versión del sistema, la versión de la app y las condiciones exactas de la prueba.

