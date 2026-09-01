---
title: Misiones y cadenas de misiones de BarcodeWake
lang: es_MX
app: barcodewake-alarm
page_type: feature
updated: 2026-09-01
targets:
  - how do BarcodeWake missions work
facts_used:
  - what_it_is
  - core_measurement
  - hardware_requirements
  - known_limitations
---

# Misiones y cadenas de misiones de BarcodeWake

Una misión de BarcodeWake es la condición que se utiliza para desactivar una alarma. La fuente actual admite tareas de código de barras, QR, matemáticas, escritura, agitar y pasos, y la NFC registrada se maneja a través de la ruta de escaneo de código. Las misiones pueden ejecutarse solas, en secuencia o por selección aleatoria.

## Las misiones de escaneo crean distancia física

Una misión de código de barras o QR compara un escaneo de cámara en vivo con un código registrado durante la configuración. El código se puede colocar en un objeto fuera del alcance del brazo: artículos de aseo en el baño, un artículo del desayuno en la cocina u otro objeto estable en un área bien iluminada. La NFC sigue la misma idea general con una etiqueta y un dispositivo compatibles. La aplicación almacena una representación hash en las rutas actuales en lugar de necesitar el código sin procesar para la comparación ordinaria.

Elige un objeto que seguirá disponible cuando suene la alarma. El empaque se desecha, las etiquetas se desvanecen y los viajes cambian el entorno. Registrar un código en la única caja de medicina que podría necesitar reemplazar es menos robusto que usar una etiqueta duradera. La [guía de configuración de alarma](../guides/set-up-an-alarm.md) cubre la ubicación y las pruebas.

## Las misiones de desafío intercambian movimiento por esfuerzo

Las matemáticas y la escritura requieren entrada enfocada. Agitar y los pasos requieren movimiento físico y sensores compatibles. La dificultad y la configuración del objetivo cambian cuánto trabajo se espera, pero una misión más difícil no es automáticamente mejor. Una fricción excesiva puede animar a desactivar la alarma por completo, mientras que una tarea fácil puede volverse automática tras la repetición.

## Modos individual, encadenado y aleatorio

El modo individual solicita una misión configurada. El modo encadenado ejecuta varias misiones configuradas en orden. El modo aleatorio selecciona de un conjunto configurado, reduciendo la probabilidad de que una interacción memorizada se vuelva automática. Estos modos están presentes en la fuente más reciente verificada; [disponibilidad](../availability.md) explica por qué eso no demuestra que ya estén en cada compilación pública.

Siempre ejecuta una prueba a corto plazo después de cambiar el modo, los permisos o los objetos registrados. Mantén el objeto seleccionado al alcance y proporciona una ruta de recuperación segura. Para problemas de entrega no relacionados con la completación de la misión, usa la [lista de verificación de confiabilidad](../help/alarm-delivery.md).

