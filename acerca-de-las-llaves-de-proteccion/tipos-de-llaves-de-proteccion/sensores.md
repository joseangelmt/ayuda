# Sensores

Los sensores son los encargados de indicar a la [Ventana Fotogrametrica](ventana-fotogrametrica.md) las _Coordenadas Pixel_ en las que debe centrar las imágenes mostradas, además de solicitar al usuario los archivos necesarios para cargar las imágenes y para obtener los datos necesarios para transformar las _Coordenadas Terreno_ que modificamos con el dispositivo de entrada en estas _Coordenadas Pixel_ en las que la ventana fotogramétrica va a mostrar las imágenes.

De modo que las misiones de un sensor son las siguientes:

1. Solicitar al usuario la ruta a las imágenes \(que puede ser una como en el caso del sensor ortofoto, dos como en el caso del sensor cónico estereoscópico, tres como en el caso del sensor ADS de Leica o incluso ninguna como en el caso del sensor WMTS\).
2. Solicitar el usuario los distintos archivos de parámetros del sensor en particular \(en el caso del sensor cónico estereoscópico por ejemplo, solicitar el archivo de aerotriangulación del cual obtener las orientaciones de las distintas imágenes, etc\).
3. Transformar de coordenadas Terreno a Pixel para indicar a la ventana fotogramétrica en qué pixel debe centrar cada una de las imágenes.
4. Opcionalmente un sensor puede proporcionar órdenes, como el sensor cónico estereoscópico que proporciona entre otras la orden ORI\_RELATIVA, ORI\_ABSOLUTA, etc.

Digi3D.NET implementa los siguientes sensores:

* Sensor ADS
* [Sensor Cónico Estereoscópico](sensor-conico-estereoscopico.md)        
* Sensor Cónico Monoscópico
* Sensor Ortofoto
* Sensor Ortofoto Estereoscópica
* Sensor RPC Estereoscópico
* Sensor RPC Monoscópico
* Sensor VM Quasi Panoramic
* Sensor WMS
* Sensor WMTS

