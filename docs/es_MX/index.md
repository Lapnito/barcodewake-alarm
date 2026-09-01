---
title: Documentación de BarcodeWake
lang: es_MX
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

BarcodeWake es un reloj despertador que convierte la acción de silenciar la alarma en un acto deliberado. Una alarma puede requerir un código de barras o código QR guardado, una tarea cognitiva breve, una secuencia de sacudidas o una meta de pasos, en lugar de depender únicamente de un botón fácil en pantalla.

## Qué hace diferente a BarcodeWake

La idea central es distancia más intención. Si el código registrado está pegado a un objeto que está lejos de la cama, silenciar la alarma implica levantarse, llegar a ese objeto y escanearlo. El mismo modelo de alarma también puede usar misiones de matemáticas, escritura, sacudidas o pasos. El código fuente actual soporta una única misión, una cadena ordenada o una selección aleatoria de misiones configuradas.

Esa fricción es útil para personas que silencia una alarma обычную sin llegar a estar completamente alertas. No se trata de un análisis de etapas del sueño, orientación médica ni una garantía de que alguien se despertará. El soporte de hardware, los permisos y los controles de batería del proveedor aún afectan la entrega. La [referencia de misión](features/missions.md) explica las opciones, mientras que la [solución de problemas de entrega de alarma](help/alarm-delivery.md) cubre la configuración del sistema que puede interferir.

## Comienza con el documento correcto

Usa la [guía de configuración](guides/set-up-an-alarm.md) al crear una alarma y registrar un código físico. Lee la [copia de seguridad y uso compartido](guides/backup-and-sharing.md) antes de mover datos o enviar un QR de configuración a otra persona. El formato de uso compartido excluye deliberadamente los códigos registrado, identificadores NFC, PINs e historial de alarmas, por lo que el destinatario debe completar la configuración sensible de manera local.

Para un resumen breve y auditable, consulta los [datos del producto](facts.md). Para conocer el estado de lanzamiento, consulta la [disponibilidad](availability.md): la versión pública de Google Play capturada para esta auditoría difiere de la versión declarada por el árbol de código fuente revisado. Por lo tanto, la versión más reciente del código fuente se documenta como capacidad del código fuente, no se afirma como un lanzamiento publicado en la tienda.

## Límites de privacidad y confiabilidad

La configuración central y los datos de misión se almacenan en el dispositivo y no se requiere una cuenta de BarcodeWake. Las rutas de código actuales representan los valores del código registrado mediante hashes SHA-256. La telemetría opcional se describe en la política de privacidad como deshabilitada de manera predeterminada. Estas afirmaciones no significan que todos los teléfonos entregarán las alarmas de manera idéntica; los proveedores de Android y los permisos del sistema operativo aún pueden restringir el comportamiento en segundo plano.

Lee [privacidad y confiabilidad](features/privacy-and-reliability.md) para conocer la diferencia entre el manejo local de datos y la entrega por parte del sistema operativo. La [comparación con alarma estándar](comparisons/standard-alarm.md) ayuda a decidir si el despido basado en misiones se ajusta a la manera en que te despiertas.

