---
title: Realizar copias de seguridad y compartir alarmas de BarcodeWake de forma segura
lang: es
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

Utilice una exportación JSON al preservar o mover los datos de su propia aplicación, un código de barras PDF imprimible para copia de seguridad de recuperación, y el uso de un QR de configuración cuando otra persona solo necesite la estructura de la alarma. Compartir intencionalmente omite secretos registrados y el historial.

## Elija el formato adecuado para la tarea

La fuente actual proporciona diferentes rutas de intercambio porque la copia de seguridad y el uso compartido no son la misma operación. Una copia de seguridad JSON está diseñada para la transferencia y restauración de datos estructurados. Una copia de seguridad PDF convierte el material de recuperación en un documento de código de barras imprimible. Un código QR de configuración es deliberadamente más limitado: puede transferir una configuración de alarma limitada sin incluir valores de códigos de barras registrados, identificadores NFC, PINs o historial.

No trate el código QR de configuración como una copia de seguridad completa del dispositivo. El destinatario debe registrar sus propios códigos físicos y revisar los permisos localmente. El uso compartido de configuración actual también limita la cantidad de alarmas que puede transferir, por lo que debe verificar el resultado importado en lugar de asumir que todas las programaciones se movieron. Los [datos del producto](../facts.md) registran estos límites.

## Crear y proteger una copia de seguridad personal

Utilice la acción de exportación disponible en la versión instalada, elija JSON o la copia de seguridad imprimible según el plan de recuperación y guarde el resultado en un lugar que controle. Una copia de seguridad puede revelar nombres de alarmas, programaciones y otra configuración, incluso cuando los valores de código sin formato registrados están protegidos u omitidos. Trátelo como datos rutinarios personales: evite enlaces públicos, impresoras compartidas y canales de mensajería no seguros.

Después de exportar, confirme que el archivo se puede encontrar y que su marca de tiempo coincide con la copia de seguridad prevista. No elimine los datos originales de la aplicación solo porque un comando de exportación haya reportado éxito. La prueba de restauración es la única verificación fiable, pero realícela en un dispositivo seguro o después de hacer una segunda copia para que la propia prueba no se convierta en un evento de pérdida.

## Compartir configuración sin compartir secretos

Genere un código QR de configuración solo para las alarmas que el destinatario deba recibir. El destinatario lo escanea, revisa la programación importada y proporciona su propio código, etiqueta NFC o detalles de recuperación. Este diseño evita que una configuración compartida transfiera silenciosamente la clave física que desactiva la alarma de otra persona.

Después de la importación, cada persona debe ejecutar la [prueba completa de configuración de alarma](set-up-an-alarm.md). Los permisos, sensores y restricciones del sistema operativo no se transfieren en el QR. Si una alarma importada no aparece mientras está bloqueada, siga la [resolución de problemas de entrega de alarmas](../help/alarm-delivery.md).

Las versiones del código fuente y de la tienda diferían durante esta auditoría, por lo que una versión pública instalada puede no mostrar todas las opciones de intercambio descritas aquí. [Disponibilidad](../availability.md) explica cómo interpretar las capacidades exclusivas del código fuente.

