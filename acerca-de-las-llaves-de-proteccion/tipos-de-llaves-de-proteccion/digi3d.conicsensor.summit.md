# Digi3D.ConicSensor.Summit

|  Orientaciones | Calibración de cámaras | Proyectos |
| :--- | :--- | :--- |
|  |  |  |

Esta extensión hace que _Digi3D.NET_ sea compatible con archivos creados con el programa _Summit Evolution._

## Tipos de archivo soportados

Permite cargar _orientaciones_ a partir de las siguientes extensiones de archivos:

| Extensión | Descripción | ¿Cuantos archivos? | Proporciona Sistema de Referencia de Coordenadas |
| :--- | :--- | :--- | :--- |
| _.smtxml_ | Archivo con parámetros de orientación externa, calibración de cámaras y de proyectos. | Un archivo por proyecto. | Si pero en un formato no reconocible por Digi3D.NET, por lo tanto Digi3D.NET seguirá el proceso indicado en [Especificación del Sistema de Referencia de Coordenadas del Sensor](especificacion-del-sistema-de-referencia-de-coordenadas-del-sensor.md) para obtener el Sistema de Referencia de Coordenadas de las orientaciones extraídas de este tipo de archivo. |

Permite cargar _calibraciones de cámara_ a partir de las siguientes extensiones de archivos:

| Extensión | Descripción | ¿Cuantos archivos? |
| :--- | :--- | :--- |
| _.smtxml_ | Archivo con parámetros de orientación externa, calibración de cámaras y de proyectos. | Un archivo por proyecto. |

Permite cargar _proyectos_ a partir de las siguientes extensiones de archivos:

| Extensión | Descripción |
| :--- | :--- |
| _.smtxml_ | Archivo con parámetros de orientación externa, calibración de cámaras y de proyectos. |

