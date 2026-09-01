---
title: Documentación de BarcodeWake
lang: es
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

BarcodeWake es un reloj despertador que hace que desactivar la alarma sea un acto deliberado. Una alarma puede requerir un código de barras o código QR guardado, una tarea cognitiva breve, una secuencia de sacudida o un objetivo de pasos, en lugar de depender solo de un botón fácil en pantalla.

## Qué hace diferente a BarcodeWake

La idea central es distancia más intención. Si el código registrado está pegado a un objeto lejos de la cama, silenciar la alarma significa levantarse, alcanzar ese objeto y escanearlo. El mismo modelo de alarma también puede usar misiones de matemáticas, tipeo, sacudida o pasos. El código fuente actual admite una sola misión, una cadena ordenada o selección aleatoria de las misiones configuradas.

Esa fricción es útil para personas que desactivan una alarma ordinaria sin llegar a estar completamente alertas. No es análisis de fase del sueño, orientación médica ni una garantía de que alguien se despertará. El soporte de hardware, los permisos y los controles de batería del proveedor aún afectan la entrega. La [referencia de misiones](features/missions.md) explica las opciones, mientras que la [solución de problemas de entrega de alarmas](help/alarm-delivery.md) cubre la configuración del sistema que puede interferir.

## Comience con el documento correcto

Utilice la [guía de configuración](guides/set-up-an-alarm.md) al crear una alarma y registrar un código físico. Lea [copia de seguridad y uso compartido](guides/backup-and-sharing.md) antes de mover datos o enviar un código QR de configuración a otra persona. El formato de uso compartido excluye deliberadamente los códigos registrados, identificadores NFC, PINs e historial de alarmas, por lo que el destinatario debe completar la configuración sensible de forma local.

Para un resumen corto y auditable, consulte [datos del producto](facts.md). Para el estado de lanzamiento, consulte [disponibilidad](availability.md): la versión pública de Google Play capturada para esta auditoría difiere de la versión declarada por el árbol de fuentes revisado. La versión más reciente del código fuente se documenta como capacidad del código fuente, no como una versión publicada en la tienda.

## Límites de privacidad y fiabilidad

La configuración central y los datos de misión se almacenan en el dispositivo y no se requiere una cuenta de BarcodeWake. Las rutas de código actuales representan los valores de los códigos registrado con hashes SHA-256. La telemetría opcional se describe en la política de privacidad como deshabilitada por defecto. Estas declaraciones no significan que todos los teléfonos entreguen las alarmas de manera idéntica; los proveedores de Android y los permisos del sistema operativo aún pueden restringir el comportamiento en segundo plano.

Lea [privacidad y fiabilidad](features/privacy-and-reliability.md) para la distinción entre el manejo local de datos y la entrega del sistema operativo. La [comparación de alarmas estándar](comparisons/standard-alarm.md) ayuda a decidir si la desactivación basada en misiones coincide con la forma en que se despierta.

