# Digi3D.ConicSensor.Digi3D

| Orientaciones | Calibración de cámaras | Proyectos |
| :--- | :--- | :--- |
|  |  |  |

Esta extensión hace que _Digi3D.NET_ sea compatible con las versiones anteriores como Digi3D.NET.

## Tipos de archivo soportados

Permite cargar _orientaciones_ a partir de las siguientes extensiones de archivos:

| Extensión | Descripción | ¿Cuantos archivos? | Proporciona Sistema de Referencia de Coordenadas |
| :--- | :--- | :--- | :--- |
| _.rel.xml_ | Archivo _XML_ con los parámetros de una orientación relativa \(que proporciona simultaneamente dos orientaciones externas, uno por cada imagen\). | Uno por modelo y no por foto, de modo que para el modelo formado con las fotos _107_ y _108_, tendremos un único archivo denominado _107-108.rel.xml_ | No aplicable, pues estas orientaciones se complementan con una [Orientación Absoluta](orientacion-absoluta.md) que en caso de haber sido creada con _Digi3D.NET_ proporcionará una [cadena WKT](cadenas-well-known-text.md) indicando el [Sistema de Referencia de Coordenadas](sistemas-de-referencia-de-coordenadas.md) a asociar a las orientaciones de los modelos cargados. |
| _.rel_ | Archivo clásico con los parámetros de una orientación relativa \(que proporciona simultaneamente dos orientaciones externas, uno por cada imagen\). | Uno por modelo y no por foto, de modo que para el modelo formado con las fotos _107_ y _108_, tendremos un único archivo denominado _107-108.rel_ | No aplicable, pues estas orientaciones se complementan con una [Orientación Absoluta](orientacion-absoluta.md) que en caso de haber sido creada con _Digi3D.NET_ proporcionará una [cadena WKT](cadenas-well-known-text.md) indicando el el [Sistema de Referencia de Coordenadas](sistemas-de-referencia-de-coordenadas.md) a asociar a las orientaciones de los modelos cargados. |
| _.orientation.xml_ | Archivo con los parámetros de orientación interna, externa y calibración de cámaras. No incluye información de los puntos medidos en cada orientación. Estos archivos se crean por cada foto, de manera que si tenemos la foto _107_, este archivo se denominará _107.orientation.xml_ | Uno por cada foto, de manera que si tenemos la foto _107_, este archivo se denominará _107.orientation.xml_ | Si, si estos archivos han sido creados con _Digi3D.NET_, en caso contrario, no aparecerá la [cadena WKT](cadenas-well-known-text.md) necesaria para conocer el Sistema de Referencia de Coordenadas a asignar a las orientaciones obtenidas con estos archivos, por lo tanto Digi3D.NET seguirá el proceso indicado en [Especificación del Sistema de Referencia de Coordenadas del Sensor](especificacion-del-sistema-de-referencia-de-coordenadas-del-sensor.md) para obtener el el [Sistema de Referencia de Coordenadas](sistemas-de-referencia-de-coordenadas.md) de las orientaciones extraídas de este tipo de archivo. |

Permite cargar _calibraciones de cámaras_ a partir de las siguientes extensiones de archivos:

| Extensión | Descripción | ¿Cuantos archivos? |
| :--- | :--- | :--- |
| _.cam_ | Archivo de cámara en formato _Digi3D.NET_ |  Tantos como distintas cámaras se hayan utilizado en el proyecto. Si se han utilizado dos cámaras distintas \(o la misma cámara con distintos objetivos\) necesitaremos dos archivos de calibración de cámara. |
| _.orientation.xml_ | Archivo con los parámetros de orientación interna, externa y calibración de cámaras. No incluye información de los puntos medidos en cada orientación. | Uno por cada foto, de manera que si tenemos la foto _107_, este archivo se denominará _107.orientation.xml_ |

Si la cámara es analógica, parte de la calibración de la cámara se almacena en archivos separados denominados archivos de _Orientación Interna_. Esta extensión permite cargar orientaciones internas a partir de las siguientes extensiones de archivos:

| Extensión | Descripción | ¿Cuantos archivos? |
| :--- | :--- | :--- |
| _.in.xml_ | Archivo _XML_ con los los parámetros de una orientación interna además de un histórico de los puntos medidos. | Uno por cada foto, de manera que si tenemos la foto _107_, su orientación interna asociada se denominará _107.in.xml_. |
| _.orientation.xml_ | Archivo con los parámetros de orientación interna, externa y calibración de cámaras. No incluye información de los puntos medidos en cada orientación. | Uno por cada foto, de manera que si tenemos la foto _107_, este archivo se denominará _107.orientation.xml_ |
| _.in_ | Archivo clásico con los los parámetros de una orientación interna además de un histórico de los puntos medidos. | Uno por cada foto, de manera que si tenemos la foto _107_, este archivo se denominará _107.in_ |

Permite cargar _proyectos_ a partir de las siguientes extensiones de archivos:

| Extensión | Descripción |
| :--- | :--- |
| _.d3dprj_ | Archivo con información de pasadas y de modelos en cada pasada. Este archivo se puede crear mediante el [Panel Proyecto fotogramétrico](panel-proyecto-fotogrametrico.md) |

