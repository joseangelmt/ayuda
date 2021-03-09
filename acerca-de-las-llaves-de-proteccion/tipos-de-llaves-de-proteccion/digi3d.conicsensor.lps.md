# Digi3D.ConicSensor.Lps

|  Orientaciones | Calibración de cámaras | Proyectos |
| :--- | :--- | :--- |
|  |  |  |

Esta extensión hace que _Digi3D.NET_ sea compatible con archivos creados con el programa _LPS._

## Tipos de archivo soportados

Permite cargar _orientaciones_ a partir de las siguientes extensiones de archivos:

| Extensión | Descripción | ¿Cuantos archivos? | Proporciona Sistema de Referencia de Coordenadas |
| :--- | :--- | :--- | :--- |
| _.blk_ | Archivo binario con parámetros de orientación externa y calibración de cámaras. | Un archivo por proyecto. | No, pues estos archivos no disponen de esa información, por lo tanto Digi3D.NET seguirá el proceso indicado en [Especificación del Sistema de Referencia de Coordenadas del Sensor](especificacion-del-sistema-de-referencia-de-coordenadas-del-sensor.md) para obtener el Sistema de Referencia de Coordenadas de las orientaciones extraídas de este tipo de archivo. |

Permite cargar _calibraciones de cámara_ a partir de las siguientes extensiones de archivos:

| Extensión | Descripción | ¿Cuantos archivos? |
| :--- | :--- | :--- |
| _.blk_ | Archivo binario con parámetros de orientación externa y calibración de cámaras. | Un archivo por proyecto. |

