---
title: Terminología de BarcodeWake
lang: es_MX
app: barcodewake-alarm
page_type: glossary
updated: 2026-09-01
targets:
  - BarcodeWake terminology
facts_used:
  - core_measurement
  - data_storage
  - export_formats
---
# Terminología de BarcodeWake

BarcodeWake utiliza “misión” para la acción requerida para desactivar una alarma. Las misiones de escaneo verifican un código físico registrado; las misiones de reto verifican una respuesta o movimiento; compartir y respaldar se refieren a distintos formatos de intercambio.

## Términos de alarmas y misiones

- Alarma: un evento de activación programada con hora, días activos, sonido y configuración de desactivación.
- Misión: la tarea que debe completarse antes de la desactivación.
- Misión de escaneo: una tarea basada en código de barras, QR o NFC que se compara con una representación de código registrado.
- Misión de reto: una tarea de matemáticas, escritura, agitación o pasos.
- Modo único: una misión configurada se ejecuta para la alarma.
- Modo encadenado: las misiones configuradas se ejecutan en un orden elegido.
- Modo aleatorio: se selecciona una misión de un conjunto configurado.
- Dificultad: un ajuste de misión que cambia la demanda de la tarea; su efecto exacto depende del tipo de misión.

## Términos de datos y confiabilidad

- Código registrado: el código de barras físico, código QR o etiqueta NFC asociado con una misión de escaneo.
- Hash de código: una representación unidireccional SHA‑256 utilizada por las rutas actuales de almacenamiento e intercambio para hacer coincidir valores registrados.
- Copia de seguridad local: una representación exportada diseñada para preservar o restaurar los datos de la aplicación.
- QR de configuración: un formato limitado de compartición de configuración que omite códigos registrados, identificadores NFC, PINs e historial.
- Doctor de confiabilidad: diagnósticos dentro de la aplicación para permisos y configuraciones del sistema que pueden interferir con la entrega de alarmas.
- Acceso a alarma exacta: permiso o política del sistema Android que permite la programación crítica en tiempo.
- Optimización de batería: controles del sistema operativo o del fabricante que pueden restringir la ejecución en segundo plano.

Para la relación completa de características, consulta [misiones y cadenas de misiones](features/missions.md). Para conocer las diferencias entre los formatos de exportación, lee [copia de seguridad y compartir](guides/backup-and-sharing.md). La [página de datos](facts.md) define lo que la aplicación no declara medir.

