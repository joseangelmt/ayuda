# Digi3D.ConicSensor.AeroOffice

| Orientaciones | Calibración de cámaras | Proyectos |
| :--- | :--- | :--- |
|  |  |  |

Esta extensión hace que Digi3D.NET sea compatible con archivos creados con el programa _AeroOffice_

## Tipos de archivo soportados

Permite cargar orientaciones a partir de las siguientes extensiones de archivos:

| Extensión | Descripción | ¿Cuantos archivos? | Proporciona Sistema de Referencia de Coordenadas |
| :--- | :--- | :--- | :--- |
| _.exp_ | Archivo con parámetros de orientación externa. | Un único archivo que contiene la información de orientación de todas las fotos del proyecto. | No, pues estos archivos no disponen de esa información, por lo tanto Digi3D.NET seguirá el proceso indicado en [Especificación del Sistema de Referencia de Coordenadas del Sensor](especificacion-del-sistema-de-referencia-de-coordenadas-del-sensor.md) para obtener el Sistema de Referencia de Coordenadas de las orientaciones extraídas de este tipo de archivo. |

