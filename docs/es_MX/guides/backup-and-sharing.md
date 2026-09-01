---
title: Respaldar y compartir alarmas de BarcodeWake de forma segura
lang: es_MX
app: barcodewake-alarm
page_type: guide
updated: 2026-09-01
targets:
  - how to back up or share BarcodeWake alarms
facts_used:
  - export_formats
  - data_storage
  - known_limitations
---
# Respaldar y compartir alarmas de BarcodeWake de forma segura

Utiliza una exportación en JSON cuando necesites preservar o mover los datos propios de tu aplicación, un código de barras PDF imprimible como respaldo para recuperación, y el código QR de configuración para compartir cuando otra persona solo necesita la estructura de la alarma. Al compartir se omiten intencionalmente los secretos registrados y el historial.

## Elige el formato adecuado para la tarea

La fuente actual proporciona diferentes rutas de intercambio porque respaldar y compartir no son la misma operación. Un respaldo en JSON está diseñado para la transferencia estructurada de datos y su restauración. Un respaldo en PDF convierte el material de recuperación en un documento de código de barras imprimible. Un código QR de configuración es deliberadamente más limitado: puede transmitir una configuración de alarma limitada sin incluir valores de códigos de barras registrados, identificadores NFC, PINs o historial.

No trates un código QR de configuración como un respaldo completo del dispositivo. El destinatario debe registrar sus propios códigos físicos y revisar los permisos localmente. El uso compartido de configuración actual también limita la cantidad de alarmas que puede transportar, así que verifica el resultado importado en lugar de asumir que se movió toda la programación. Los [hechos del producto](../facts.md) registran estos límites.

## Crea y protege un respaldo personal

Utiliza la acción de exportación disponible en la versión instalada, elige JSON o el respaldo imprimible según tu plan de recuperación, y guarda el resultado en algún lugar que controlas. Un respaldo puede revelar nombres de alarmas, programaciones y otra configuración incluso cuando los valores de código sin procesar están protegidos u omitidos. Manéjalo como datos rutinarios personales: evita enlaces públicos, impresoras compartidas y canales de mensajería no confiables.

Después de exportar, confirma que el archivo se pueda encontrar y que su marca de tiempo coincida con el respaldo previsto. No elimines los datos originales de la aplicación simplemente porque un comando de exportación haya reportado éxito. La prueba de restauración es la única verificación confiable, pero realízala en un dispositivo seguro o después de hacer una segunda copia para que la prueba en sí misma no se convierta en un evento de pérdida.

## Comparte la configuración sin compartir secretos

Genera un código QR de configuración solo para las alarmas que el destinatario debe recibir. El destinatario lo escanea, revisa la programación importada y proporciona su propio código, etiqueta NFC o detalles de recuperación. Este diseño evita que una configuración compartida transfiera silenciosamente la llave física que descarta la alarma de otra persona.

Después de la importación, cada persona debe ejecutar la [prueba completa de configuración de alarma](set-up-an-alarm.md). Los permisos, sensores y restricciones del sistema operativo no se transfieren en el código QR. Si una alarma importada no aparece mientras está bloqueada, sigue la [solución de problemas de entrega de alarmas](../help/alarm-delivery.md).

Las versiones de origen y de almacenamiento diferían durante esta auditoría, por lo que una versión pública instalada puede no exponer cada opción de intercambio descrita aquí. [Disponibilidad](../availability.md) explica cómo interpretar las capacidades exclusivas del código fuente.

