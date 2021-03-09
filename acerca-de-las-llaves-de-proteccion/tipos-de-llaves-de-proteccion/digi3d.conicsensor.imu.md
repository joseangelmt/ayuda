# Digi3D.ConicSensor.Imu

| Orientaciones | Calibración de cámaras | Proyectos |
| :--- | :--- | :--- |
|  |  |  |

Esta extensión hace que _Digi3D.NET_ sea compatible con archivos creados con el programa que generen archivos de _Centros de Proyección_ y Giros como _PatB_.

## Tipos de archivo soportados

Permite cargar _orientaciones_ a partir de las siguientes extensiones de archivos:

| Extensión | Descripción | ¿Cuantos archivos? | Proporciona Sistema de Referencia de Coordenadas |
| :--- | :--- | :--- | :--- |
| _.eo_ | Archivo con parámetros de orientación y calibración de cámaras \(centros de proyección y giros\) | Un archivo con todas las orientaciones del proyecto. | No, pues estos archivos no disponen de esa información, por lo tanto Digi3D.NET seguirá el proceso indicado en [Especificación del Sistema de Referencia de Coordenadas del Sensor](especificacion-del-sistema-de-referencia-de-coordenadas-del-sensor.md) para obtener el Sistema de Referencia de Coordenadas de las orientaciones extraídas de este tipo de archivo. |
| _.imu_ | Archivo con parámetros de orientación y calibración de cámaras \(centros de proyección y giros\) | Un archivo con todas las orientaciones del proyecto. | No, pues estos archivos no disponen de esa información, por lo tanto Digi3D.NET seguirá el proceso indicado en [Especificación del Sistema de Referencia de Coordenadas del Sensor](especificacion-del-sistema-de-referencia-de-coordenadas-del-sensor.md) para obtener el Sistema de Referencia de Coordenadas de las orientaciones extraídas de este tipo de archivo. |

## Formato de los archivos

Los archivos de tipo Centro de Proyección y Giros tienen el siguiente formato

| Foto | X | Y | Z | Omega | Phi | Kappa |
| :--- | :--- | :--- | :--- | :--- | :--- | :--- |


Es importante tener en cuenta los siguientes puntos:

* El nombre de la foto **no debe contener la extensión de la foto.**
* Los giros no pueden ser _Roll_, _Pitch_, _Yaw_, sino que deben ser obligatoriamente _Omega_, _Phi_ y _Kappa_.

## Ejemplo de un archivo con este formato

```text
    125 281632.06200 4821096.44500 654.77700 -0.535190313632 -0.445381220345 0.582158694418
    126 281793.24627 4821095.38486 655.33366 -0.001879854920 -0.017783811235 0.437679145769
    127 281954.93084 4821094.00155 655.17956  0.061659643206 -0.220671738283 0.398812383445
    128 282116.15998 4821094.17859 656.14275 -0.314508914706 -0.562605907268 0.323765754344
    129 282277.35841 4821096.32887 657.58691 -0.681840687079 -0.299489445142 0.238310569277
```

Vea también

