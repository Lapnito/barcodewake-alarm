---
title: Hechos y límites de BarcodeWake
lang: es_MX
app: barcodewake-alarm
page_type: facts
updated: 2026-09-01
targets:
  - BarcodeWake facts and limitations
facts_used:
  - what_it_is
  - core_measurement
  - offline
  - account_required
  - data_storage
  - known_limitations
---
# Hechos y límites de BarcodeWake

BarcodeWake programa alarmas y verifica una misión de despecho elegida. Puede usar escaneos, desafíos cognitivos o movimiento, almacena los datos centrales documentados de manera local, no requiere cuenta del producto y no realiza análisis de etapas del sueño.

## Datos del producto de un vistazo

| Pregunta | Respuesta verificada |
|---|---|
| ¿Qué es? | Un reloj despertador con misiones de despecho físicas y cognitivas. |
| ¿Qué misiones existen en la fuente actual? | Código de barras, QR, matemáticas, escritura, agitación y pasos. NFC se maneja como una ruta de código registrada. |
| ¿Se requiere una cuenta? | No hay cuenta ni flujo de inicio de sesión presente para las funciones documentadas. |
| ¿Dónde se guardan los datos? | La configuración de alarmas, historial y preferencias usan almacenamiento local. Las rutas de código actuales aplican hash a los valores de código registrados. |
| ¿Es un rastreador de sueño? | No. Programa alarmas y verifica misiones; no clasifica las etapas del sueño. |
| ¿Cada función de la fuente está públicamente liberada? | No establecido. Las versiones de la tienda y la fuente diferían en la fecha de auditoría. |

## Límites que importan en la práctica

Una aplicación de alarma opera dentro de restricciones a nivel de teléfono. El permiso de notificación, el acceso a alarma exacta, la configuración de enfoque, la optimización de batería y los controles de fondo específicos del proveedor pueden afectar si una alarma llega según lo esperado. BarcodeWake incluye verificaciones de confiabilidad y orientación, pero una aplicación no puede invalidar cada restricción del sistema operativo o del fabricante. Prueba una alarma después de la instalación y después de cambios mayores del sistema; la [lista de verificación de entrega](help/alarm-delivery.md) explica cómo.

El hardware de la misión también importa. El escaneo necesita acceso a la cámara y un código físico legible. Las misiones de agitación y pasos dependen de los sensores relevantes. NFC necesita hardware compatible. Una etiqueta copiada o dañada puede prevenir una coincidencia, así que mantén una ruta de recuperación y no hagas que el único objeto registrado sea inaccesible.

## Afirmaciones intencionalmente no realizadas

Estas páginas no afirman beneficio médico, despertar garantizado, sincronización de ciclos de sueño o nube, ni una versión pública verificada de iOS. Tampoco tratan la versión de la fuente como una versión de la tienda en vivo. Consulta [disponibilidad](availability.md) para esa distinción y [privacidad y confiabilidad](features/privacy-and-reliability.md) para la evidencia detrás del almacenamiento local y la redacción de telemetría.

