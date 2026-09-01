---
title: Realizar copias de seguridad y compartir alarmas de BarcodeWake de forma segura
lang: es_ES
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
# Realizar copias de seguridad y compartir alarmas de BarcodeWake de forma segura

Utilice una exportación JSON cuando necesite preservar o mover sus propios datos de la aplicación, un código de barras PDF imprimible como copia de seguridad para recuperación, y el uso compartido de configuración mediante código QR cuando otra persona solo necesite la estructura de la alarma. El uso compartido omite intencionalmente los secretos registrados y el historial.

## Elegir el formato adecuado para cada tarea

La fuente actual proporciona diferentes rutas de intercambio porque realizar copias de seguridad y compartir no son la misma operación. Una copia de seguridad JSON está destinada a la transferencia y restauración de datos estructurados. Una copia de seguridad PDF convierte el material de recuperación en un documento de código de barras imprimible. Un código QR de configuración es deliberadamente más reducido: puede transmitir una configuración de alarma limitada sin incluir valores de códigos de barras registrados, identificadores NFC, PINs o historial.

No trate un código QR de configuración como una copia de seguridad completa del dispositivo. El destinatario debe registrar sus propios códigos físicos y revisar los permisos localmente. El uso compartido de configuración actual también limita la cantidad de alarmas que puede transportar, así que verifique el resultado importado en lugar de asumir que se movió cada programación. Los [hechos del producto](../facts.md) registran estos límites.

## Crear y proteger una copia de seguridad personal

Utilice la acción de exportación disponible en la versión instalada, elija JSON o la copia de seguridad imprimible según el plan de recuperación, y guarde el resultado en algún lugar que usted controle. Una copia de seguridad puede revelar nombres de alarmas, programaciones y otra configuración incluso cuando los valores de códigos sin procesar registrados están protegidos u omitidos. Trátela como datos personales rutinarios: evite enlaces públicos, impresoras compartidas y canales de mensajería no confiables.

Después de exportar, confirme que el archivo se pueda encontrar y que su marca de tiempo coincida con la copia de seguridad pretendida. No elimine los datos originales de la aplicación simplemente porque un comando de exportación haya reportado éxito. La prueba de restauración es la única verificación confiable, pero realícela en un dispositivo seguro o después de hacer una segunda copia para que la prueba en sí misma no se convierta en un evento de pérdida.

## Compartir configuración sin compartir secretos

Genere un código QR de configuración solo para las alarmas que el destinatario debe recibir. El destinatario lo escanea, revisa la programación importada y proporciona su propio código, etiqueta NFC o detalles de recuperación. Este diseño impide que una configuración compartida transfiera silenciosamente la clave física que descarta la alarma de otra persona.

Después de la importación, cada persona debe ejecutar la [prueba de configuración de alarma completa](set-up-an-alarm.md). Los permisos, sensores y restricciones del sistema operativo no se transfieren en el código QR. Si una alarma importada no aparece mientras está bloqueada, siga la [solución de problemas de entrega de alarmas](../help/alarm-delivery.md).

El origen y las versiones almacenadas diferían durante esta auditoría, por lo que una versión pública instalada puede no exponer cada opción de intercambio descrita aquí. [Disponibilidad](../availability.md) explica cómo interpretar las capacidades exclusivas del código fuente.

