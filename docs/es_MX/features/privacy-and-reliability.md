---
title: Privacidad y confiabilidad de la alarma de BarcodeWake
lang: es_MX
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

# Privacidad y confiabilidad de la alarma de BarcodeWake

## Los datos locales no eliminan las dependencias del sistema

BarcodeWake mantiene la configuración documentada de alarmas y los datos de misión en el dispositivo y no requiere una cuenta de la aplicación. Las rutas de código actuales generan valores hash de los códigos registrados. La telemetría opcional se describe como deshabilitada de manera predeterminada, mientras que la entrega de alarmas aún depende de permisos del sistema y controles del proveedor.

El almacenamiento local significa que la configuración normal de alarmas no requiere una cuenta en la nube de BarcodeWake. Los registros de alarmas, el historial y las preferencias se gestionan a través de la capa de datos local de la aplicación. Los valores registrados de códigos de barras, QR y NFC se representan con hashes SHA-256 en el almacenamiento actual y las rutas de importación, lo que evita mantener el valor sin procesar original para la coincidencia.

El hash no es lo mismo que el cifrado de cada registro de la aplicación, y el almacenamiento local no es una copia de seguridad. Alguien con acceso a un dispositivo desbloqueado aún podría ver los nombres de las alarmas, los horarios o el historial a través de la aplicación. Un teléfono perdido o reiniciado también puede perder los datos locales a menos que el usuario haya realizado una exportación. Consulta [copia de seguridad y uso compartido](../guides/backup-and-sharing.md) para conocer los formatos y sus diferentes propósitos.

La política de privacidad indica que la telemetría opcional está desactivada de manera predeterminada y describe el manejo agregado si está habilitada. Por lo tanto, esta documentación no afirma la afirmación más amplia de que la aplicación nunca puede comunicarse a través de una red. Establece los hechos verificados más limitados: la operación principal y los datos son locales, no se requiere una cuenta del producto, y no aparece ninguna dependencia de SDK de publicidad en el proyecto revisado.

## La confiabilidad es una responsabilidad compartida

BarcodeWake puede programar y presentar una alarma, pero el sistema operativo decide cuándo se puede ejecutar el trabajo en segundo plano y qué interrupciones se permiten. Los permisos de notificación, el acceso a alarmas exactas, los modos silenciosos o de concentración, la optimización de la batería, la suspensión automática de aplicaciones y los asesino de tareas del fabricante pueden ser relevantes. La herramienta de confiabilidad dentro de la aplicación puede identificar riesgos de configuración y dirigir a los usuarios a la configuración; no puede invalidar la política del sistema.

Después de la instalación, prueba con la pantalla bloqueada y el teléfono en el mismo modo de energía utilizado durante la noche. Repite esa prueba después de una actualización del sistema, un cambio en el ahorro de batería o una reinstallación de la aplicación. Mantén el dispositivo cargado, el volumen adecuado y la misión elegida físicamente disponible. Sigue la [solución de problemas de entrega de alarmas](../help/alarm-delivery.md) cuando una prueba falle.

## Lo que la privacidad y la confiabilidad no prometen

BarcodeWake no es un dispositivo médico, servicio de alerta de emergencia ni rastreador de etapas del sueño. Ninguna aplicación de alarma puede garantizar que te despiertes o compensar un dispositivo no disponible. La [página de hechos y límites](../facts.md) enumera estos límites, mientras que [disponibilidad](../availability.md) separa la evidencia de la tienda pública de las capacidades más recientes del código fuente.

