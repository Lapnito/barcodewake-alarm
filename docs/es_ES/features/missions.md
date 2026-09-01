---
title: Misiones y cadenas de misiones de BarcodeWake
lang: es_ES
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

Una misión de BarcodeWake es la condición utilizada para desactivar una alarma. La fuente actual soporta códigos de barras, QR, matemáticas, escritura, sacudidas y tareas de pasos, con NFC registrado manejado a través de la ruta de escaneo de códigos. Las misiones pueden ejecutarse solas, en secuencia o por selección aleatoria.

## Las misiones de escaneo crean distancia física

Una misión de código de barras o QR compara un escaneo de cámara en vivo con un código registrado durante la configuración. El código puede colocarse en un objeto fuera del alcance del brazo: artículos de tocador en un baño, un elemento del desayuno en una cocina, u otro objeto estable en un área bien iluminada. NFC sigue la misma idea general con una etiqueta compatible y dispositivo. La aplicación almacena una representación hash en las rutas actuales en lugar de necesitar el código sin procesar para una comparación ordinaria.

Elige un objeto que seguirá disponible cuando suene la alarma. El empaquetado se descarta, las etiquetas se desvanecen y los viajes cambian el entorno. Registrar un código en la única caja de medicina que podrías necesitar reemplazar es menos robusto que usar una etiqueta duradera. La [guía de configuración de alarmas](../guides/set-up-an-alarm.md) cubre la colocación y las pruebas.

## Las misiones de desafío intercambian movimiento por esfuerzo

Las matemáticas y la escritura requieren entrada enfocada. Las sacudidas y los pasos requieren movimiento físico y sensores compatibles. La configuración de dificultad y objetivos cambia cuánto trabajo se espera, pero una misión más difícil no es automáticamente una mejor. La fricción excesiva puede fomentar desactivar la alarma por completo, mientras que una tarea fácil puede volverse automática después de la repetición.

Haz coincidir la tarea con el modo de falla. Si apagas las alarmas medio dormido, escanear en otra habitación crea distancia útil. Si el acceso a la cámara es inconveniente, una tarea corta de escritura o matemáticas puede ser más práctica. Si la movilidad, el equilibrio o la accesibilidad son una preocupación, evita las misiones basadas en movimiento y elige una tarea que pueda completarse de manera segura.

## Modos individual, encadenado y aleatorio

El modo individual solicita una misión configurada. El modo encadenado ejecuta varias misiones configuradas en orden. El modo aleatorio selecciona de un conjunto configurado, reduciendo la posibilidad de que una interacción memorizada se vuelva automática. Estos modos están presentes en la fuente verificada más reciente; [disponibilidad](../availability.md) explica por qué eso no demuestra que ya estén en cada compilación pública.

Siempre ejecuta una prueba a corto plazo después de cambiar el modo, los permisos o los objetos registrados. Mantén el objeto seleccionado accesible y proporciona una ruta de recuperación segura. Para problemas de entrega no relacionados con la finalización de la misión, usa la [lista de verificación de confiabilidad](../help/alarm-delivery.md).

