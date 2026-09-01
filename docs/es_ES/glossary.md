---
title: Terminología de BarcodeWake
lang: es_ES
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

BarcodeWake usa “misión” para la acción requerida para desactivar una alarma. Las misiones de escaneo verifican un código físico registrado; las misiones de reto verifican una respuesta o movimiento; compartir y copia de seguridad se refieren a diferentes formatos de intercambio.

## Términos de alarma y misión

- Alarm: un evento de activación programada con hora, días activos, sonido y configuración de desactivación.
- Mission: la tarea que debe completarse antes de la desactivación.
- Scan mission: una tarea basada en código de barras, código QR o NFC que se compara con una representación de código registrado.
- Challenge mission: una tarea de matemáticas, escritura, sacudida o paso.
- Single mode: una misión configurada se ejecuta para la alarma.
- Chain mode: las misiones configuradas se ejecutan en un orden elegido.
- Random mode: se selecciona una misión de un conjunto configurado.
- Difficulty: un ajuste de misión que cambia la demanda de la tarea; su efecto exacto depende del tipo de misión.

## Términos de datos y fiabilidad

- Registered code: el código de barras físico, código QR o etiqueta NFC asociado a una misión de escaneo.
- Code hash: una representación unidireccional SHA-256 utilizada por las rutas actuales de almacenamiento e intercambio para comparar valores registrados.
- Local backup: una representación exportada destinada a preservar o restaurar los datos de la aplicación.
- Setup QR: un formato limitado de intercambio de configuración que omite códigos registrados, identificadores NFC, PINs e historial.
- Reliability Doctor: diagnóstico dentro de la aplicación para permisos y configuraciones del sistema que pueden interferir con la entrega de alarmas.
- Exact-alarm access: permiso o política del sistema Android que permite la programación crítica en el tiempo.
- Battery optimisation: controles del sistema operativo o del fabricante que pueden restringir la ejecución en segundo plano.

Para ver la relación completa de funciones, consulta [misiones y cadenas de misiones](features/missions.md). Para conocer las diferencias entre los formatos de exportación, lee [copia de seguridad y compartir](guides/backup-and-sharing.md). La [página de datos](facts.md) define lo que la aplicación no afirma medir.

