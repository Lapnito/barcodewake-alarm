---
title: ¿Por qué una alarma de BarcodeWake puede no sonar
lang: es
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
# ¿Por qué una alarma de BarcodeWake puede no sonar

Una alarma guardada aún puede ser bloqueada por la configuración de notificaciones, el acceso a alarmas exactas, los modos de enfoque o silencio, el bajo volumen, las restricciones de batería, la suspensión de la aplicación o los controles de fondo del proveedor. Verifique la entrega por separado del escaneo de la misión y luego ejecute una prueba con la pantalla bloqueada.

## Primero aísle la entrega del rechazo

Cree una alarma de prueba a corto plazo con una misión simple y deje la aplicación en segundo plano. Bloquee la pantalla. Si no aparece ninguna pantalla de alarma ni sonido, el problema es la entrega; cambiar el código de barras registrado no lo solucionará. Si la alarma aparece pero la misión no puede completarse, la entrega funciona y el problema es la cámara, el sensor, la coincidencia del código o la configuración de la misión.

Confirme que la alarma esté activada, que el día programado sea correcto y que la zona horaria del teléfono coincida con la programación prevista. Compruebe el volumen de medios y de la alarma en lugar de depender solo del estado del botón lateral. Revise las reglas de no molestar o enfoque, los dispositivos de audio conectados y si el teléfono se reinició después de crear la alarma.

## Revisar los permisos del sistema operativo

Permita las notificaciones y cualquier acceso a alarma exacta o de pantalla completa solicitado por la compilación instalada. Elimine BarcodeWake de la optimización agresiva de batería o de las listas de reposo automático cuando el proveedor del dispositivo ofrezca esos controles. Abra el diagnóstico de fiabilidad dentro de la aplicación y siga los ajustes específicos del dispositivo que identifique. La [página de privacidad y fiabilidad](../features/privacy-and-reliability.md) explica por qué estas dependencias del sistema permanecen incluso cuando los datos de la aplicación son locales.

Después de cambiar un ajuste, repita la prueba con la pantalla bloqueada. Cambiar varios controles a la vez dificulta identificar la causa. Las actualizaciones del sistema pueden restablecer o reinterpretar los permisos, por lo que se debe repetir la prueba después de una actualización importante o una reinstalación de la aplicación.

## Diagnosticar la finalización de la misión por separado

Para misiones de código de barras y QR, limpie el lente de la cámara, mejore la iluminación y confirme que el objeto registrado no ha cambiado. Otorgue permiso de cámara. Para NFC, verifique la compatibilidad del dispositivo y mantenga la etiqueta cerca de la posición correcta de la antena. Las misiones de sacudida y paso dependen de sensores de movimiento o pasos y pueden comportarse de manera diferente cuando los modos de ahorro de energía restringen la entrega de sensores.

Si una misión se configuró como parte de una cadena, cada paso requerido debe completarse. Revise el [comportamiento de la misión](../features/missions.md) y, si es necesario, cree una nueva prueba usando el [procedimiento de configuración](../guides/set-up-an-alarm.md).

## Saber cuándo el teléfono es el límite

BarcodeWake no puede invalidar un dispositivo apagado, una batería agotada, hardware de audio roto ni cada asesino de tareas del fabricante. No es un servicio de notificación de emergencia. Mantenga otro método de alarma para situaciones de alta consecuencia e informe los fallos reproducibles con el modelo del dispositivo, la versión del sistema, la versión de la aplicación y las condiciones exactas de la prueba.

