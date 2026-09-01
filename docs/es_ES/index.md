---
title: Documentación de BarcodeWake
lang: es_ES
app: barcodewake-alarm
page_type: index
updated: 2026-09-01
targets:
  - what is BarcodeWake
facts_used:
  - what_it_is
  - known_limitations
---

# Documentación de BarcodeWake

BarcodeWake es un reloj despertador que hace que desactivar la alarma sea un acto deliberado. Una alarma puede requerir un código de barras o QR guardado, una tarea cognitiva breve, una secuencia de sacudidas o un objetivo de pasos, en lugar de depender únicamente de un sencillo botón en pantalla.

## Qué hace diferente a BarcodeWake

La idea central es distancia más intención. Si el código registrado está asociado a un objeto lejos de la cama, silenciar la alarma significa levantarse, acercarse a ese objeto y escanearlo. El mismo modelo de alarma también puede usar misiones de matemáticas, escritura, sacudidas o pasos. El código fuente actual soporta una única misión, una cadena ordenada o una selección aleatoria de misiones configuradas.

Esa fricción es útil para personas que desactivan una alarma ordinaria sin estar completamente despiertas. No es un análisis de fases del sueño, ni orientación médica, ni una garantía de que alguien se despierte. El soporte de hardware, los permisos y los controles de batería del proveedor todavía pueden afectar la entrega. La [referencia de misión](features/missions.md) explica las opciones, mientras que la [solución de problemas de entrega de alarmas](help/alarm-delivery.md) cubre la configuración del sistema que puede interferir.

## Comienza con el documento adecuado

Usa la [guía de configuración](guides/set-up-an-alarm.md) al crear una alarma y registrar un código físico. Lee la [copia de seguridad y uso compartido](guides/backup-and-sharing.md) antes de mover datos o enviar un código QR de configuración a otra persona. El formato de uso compartido excluye deliberadamente los códigos registrado, los identificadores NFC, los PINs y el historial de alarmas, por lo que el destinatario debe completar la configuración sensible de forma local.

Para un resumen breve y auditable, consulta los [datos del producto](facts.md). Para el estado de lanzamiento, usa la [disponibilidad](availability.md): la versión pública de Google Play capturada para esta auditoría difiere de la versión declarada por el árbol de fuentes revisado. Por lo tanto, la versión más reciente del código fuente se documenta como capacidad de la fuente, no como una versión publicada en la tienda.

## Límites de privacidad y fiabilidad

La configuración central y los datos de la misión se almacenan en el dispositivo y no se requiere ninguna cuenta de BarcodeWake. Las rutas de código actuales representan los valores de los códigos registrado con hashes SHA-256. La telemetría opcional se describe en la política de privacidad como desactivada de forma predeterminada. Estas declaraciones no significan que todos los teléfonos entregarán las alarmas de manera idéntica; los proveedores de Android y los permisos del sistema operativo aún pueden restringir el comportamiento en segundo plano.

Lee [privacidad y fiabilidad](features/privacy-and-reliability.md) para distinguir entre el manejo local de datos y la entrega del sistema operativo. La [comparación con alarma estándar](comparisons/standard-alarm.md) ayuda a decidir si la desactivación basada en misiones se ajusta a la forma en que te despiertas.

