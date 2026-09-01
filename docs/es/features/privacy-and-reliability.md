---
title: Privacidad y fiabilidad de alarma de BarcodeWake
lang: es
app: barcodewake-alarm
page_type: feature
updated: 2026-09-01
targets:
  - is BarcodeWake private and reliable
facts_used:
  - offline
  - account_required
  - ads_tracking
  - data_storage
  - accuracy_limits
---
# Privacidad y fiabilidad de alarma de BarcodeWake

BarcodeWake mantiene la configuración documentada de alarmas y los datos de misión en el dispositivo y no requiere una cuenta de aplicación. Las rutas de código actuales aplican hash a los valores de código registrados. La telemetría opcional se describe como deshabilitada por defecto, mientras que la entrega de alarmas todavía depende de los permisos del sistema y los controles del proveedor.

## Los datos locales no eliminan las dependencias del sistema

El almacenamiento local significa que la configuración ordinaria de alarmas no requiere una cuenta en la nube de BarcodeWake. Los registros de alarmas, el historial y las preferencias se manejan a través de la capa de datos local de la aplicación. Los valores de código de barras, QR y NFC registrados se representan con hashes SHA-256 en el almacenamiento actual y las rutas de importación, lo que evita retener el valor sin procesar habitual para la coincidencia.

El hash no es lo mismo que el cifrado de cada registro de la aplicación, y el almacenamiento local no es una copia de seguridad. Alguien con acceso a un dispositivo desbloqueado aún puede ver nombres de alarmas, horarios o historial a través de la aplicación. Un teléfono perdido o reiniciado también puede perder datos locales a menos que el usuario haya realizado una exportación. Consulta [copia de seguridad y uso compartido](../guides/backup-and-sharing.md) para conocer los formatos y sus diferentes propósitos.

La política de privacidad indica que la telemetría opcional está desactivada por defecto y describe el manejo agregado si está habilitada. Por lo tanto, esta documentación no hace la afirmación más amplia de que la aplicación nunca puede comunicarse a través de una red. Establece los hechos verificados más estrechos: la operación central y los datos son locales, no se requiere una cuenta del producto, y no aparece ninguna dependencia de SDK de publicidad en el proyecto verificado.

## La fiabilidad es una responsabilidad compartida

BarcodeWake puede programar y presentar una alarma, pero el sistema operativo decide cuándo se puede ejecutar el trabajo en segundo plano y qué interrupciones están permitidas. El permiso de notificación, el acceso a alarmas exactas, los modos silenciosos o de concentración, la optimización de batería, la suspensión automática de aplicaciones y los eliminadores de tareas del fabricante pueden ser relevantes. La herramienta de fiabilidad dentro de la aplicación puede identificar riesgos de configuración y dirigir a los usuarios a la configuración; no puede invalidar la política del sistema.

Después de la instalación, prueba con la pantalla bloqueada y el teléfono en el mismo modo de energía utilizado durante la noche. Repite esa prueba después de una actualización del sistema, un cambio en el ahorro de batería o una reinstallación de la aplicación. Mantén el dispositivo cargado, el volumen apropiado y la misión elegida físicamente disponible. Sigue la [solución de problemas de entrega de alarmas](../help/alarm-delivery.md) cuando una prueba falla.

## Lo que la privacidad y la fiabilidad no prometen

BarcodeWake no es un dispositivo médico, servicio de alerta de emergencia ni un rastreador de etapa del sueño. Ninguna aplicación de alarmas puede garantizar que te despierte o compensar por un dispositivo no disponible. La [página de hechos y límites](../facts.md) enumera estos límites, mientras que [disponibilidad](../availability.md) separa la evidencia de tiendas públicas de las capacidades más recientes del código fuente.

