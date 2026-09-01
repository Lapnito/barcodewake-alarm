---
title: Disponibilidad y versiones de BarcodeWake
lang: es
app: barcodewake-alarm
page_type: availability
updated: 2026-09-01
targets:
  - where is BarcodeWake available
facts_used:
  - known_limitations
  - hardware_requirements
---
# Disponibilidad y versiones de BarcodeWake

BarcodeWake tiene un listado público verificado en Google Play para Android. En la fecha de auditoría, Google Play mostraba la versión 1.0.0, mientras que el proyecto fuente verificado declaraba la versión 2.0.0+2. No se verificó ningún listado público en App Store.

## Distribución pública verificada

El paquete de Android aparece públicamente como [BarcodeWake: Alarma Anti-Trampa en Google Play](https://play.google.com/store/apps/details?id=com.tomas.barcodewake_alarm&hl=en&gl=us). La instantánea de la tienda capturada para esta documentación reportaba la versión 1.0.0 y una fecha de última actualización en marzo de 2026. Esa instantánea es evidencia del listado en un momento dado, no una promesa de que cada región vea el mismo despliegue o de que el listado permanecerá sin cambios.

El árbol de fuentes contiene proyectos de plataforma para Android e iOS. El código fuente de la plataforma no demuestra publicación en la tienda. Dado que no se verificó ninguna página de App Store, estos documentos describen los elementos relacionados con iOS únicamente como soporte de código fuente y no informan a los lectores que BarcodeWake esté actualmente descargable desde Apple.

## Por qué aparecen dos números de versión

El archivo `pubspec.yaml` del repositorio declara la versión de código fuente 2.0.0+2 y su registro de cambios describe un sistema de misiones más amplio que el listado público capturado. Un despliegue en la tienda puede ir por detrás de una rama de desarrollo, estar programado por región, o simplemente no haber sido publicado. Sin un registro coincidente en la tienda, la afirmación segura es restrictiva: la capacidad existe en el código fuente verificado, mientras que la disponibilidad pública está probada solo para la versión de la tienda capturada.

Cuando una página de características dice "código fuente actual", esa redacción es deliberada. Antes de depender de cadenas de misiones, uso compartido de configuración u otra capacidad más reciente, verifica la versión de la aplicación instalada y los controles visibles. Comienza con [comportamiento de misiones](features/missions.md), luego usa la [guía de configuración](guides/set-up-an-alarm.md) solo para las opciones que tu compilación instalada realmente muestra.

## Requisitos del dispositivo y verificaciones de instalación

El escaneo requiere permiso de cámara. Las misiones de NFC, movimiento y pasos necesitan hardware de dispositivo correspondiente. La entrega de alarmas en Android puede requerir permiso de notificación y acceso a alarma exacta, con configuraciones adicionales de batería en algunos fabricantes. Instala desde el listado verificado de la tienda, crea una alarma de prueba a corto plazo, bloquea la pantalla y confirma tanto el sonido como la misión seleccionada antes de depender de ella para un despertar importante.

Para una lista concisa de límites, lee [hechos del producto](facts.md). Si una alarma de prueba falla, sigue la [solución de problemas de entrega de alarmas](help/alarm-delivery.md) en lugar de recrear la alarma repetidamente.

