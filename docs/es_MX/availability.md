---
title: Disponibilidad y versiones de BarcodeWake
lang: es_MX
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

BarcodeWake cuenta con un listado público verificado en Google Play para Android. En la fecha de auditoría, Google Play mostraba la versión 1.0.0, mientras que el proyecto fuente revisado declaraba la versión 2.0.0+2. No se verificó ningún listado público en App Store.

## Distribución pública verificada

El paquete de Android aparece públicamente como [BarcodeWake: Alarma Anti-Trampa en Google Play](https://play.google.com/store/apps/details?id=com.tomas.barcodewake_alarm&hl=en&gl=us). La captura del storefront para esta documentación reportaba la versión 1.0.0 y una fecha de última actualización en marzo de 2026. Esa captura es evidencia del listado en un momento dado, no una promesa de que cada región vea el mismo despliegue o de que el listado permanecerá sin cambios.

El árbol fuente contiene proyectos de plataforma Android e iOS. El fuente de plataforma no demuestra publicación en tienda. Dado que no se verificó ninguna página de App Store, estos docs describen los elementos relacionados con iOS como soporte de fuente únicamente y no indican a los lectores que BarcodeWake esté actualmente descargable desde Apple.

## Por qué aparecen dos números de versión

El archivo `pubspec.yaml` del repositorio declara la versión fuente 2.0.0+2 y su registro de cambios describe un sistema de misiones más amplio que el listado público capturado. Un despliegue en tienda puede ir rezagado respecto a una rama de desarrollo, estar preconfigurado por región, o simplemente no haber sido publicado. Sin un registro coincidente en tienda, la declaración segura es estrecha: la capacidad existe en la fuente revisada, mientras que la disponibilidad pública está probada únicamente para la versión de tienda capturada.

Cuando una página de característica dice "fuente actual", esa redacción es deliberada. Antes de depender de cadenas de misión, compartición de configuración u otra capacidad más reciente, verifica la versión de la app instalada y los controles visibles. Comienza con [comportamiento de misiones](features/missions.md), luego usa la [guía de configuración](guides/set-up-an-alarm.md) únicamente para las opciones que tu compilación instalada realmente muestra.

## Requisitos del dispositivo y verificaciones de instalación

El escaneo requiere permiso de cámara. Las misiones NFC, de movimiento y de pasos necesitan hardware de dispositivo correspondiente. La entrega de alarmas en Android puede requerir acceso a notificaciones y alarmas exactas, con configuraciones de batería adicionales en algunos fabricantes. Instala desde el listado de tienda verificado, crea una alarma de prueba a corto plazo, bloquea la pantalla y confirma tanto el sonido como la misión seleccionada antes de depender de ella para un despertar importante.

Para una lista concisa de límites, lee [hechos del producto](facts.md). Si una alarma de prueba falla, sigue la [solución de problemas de entrega de alarmas](help/alarm-delivery.md) en lugar de recrear la alarma repetidamente.

