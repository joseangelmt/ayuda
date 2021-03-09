# Digi3D.ConicSensor.PatB

| Orientaciones | Calibración de cámaras | Proyectos |
| :--- | :--- | :--- |
|  |  |  |

Esta extensión hace que _Digi3D.NET_ sea compatible con archivos de orientaciones creados con el programa _PatB_.

## Tipos de archivo soportados

Permite cargar _orientaciones_ a partir de las siguientes extensiones de archivos:

| Extensión | Descripción | ¿Cuantos archivos? | Proporciona Sistema de Referencia de Coordenadas |
| :--- | :--- | :--- | :--- |
| _.ori_ | Archivo de orientaciones de imágenes. | Un archivo con todas las orientaciones del proyecto. | No, pues estos archivos no disponen de esa información, por lo tanto Digi3D.NET seguirá el proceso indicado en [Especificación del Sistema de Referencia de Coordenadas del Sensor](especificacion-del-sistema-de-referencia-de-coordenadas-del-sensor.md) para obtener el Sistema de Referencia de Coordenadas de las orientaciones extraídas de este tipo de archivo. |

## Formato de los archivos

Los archivos de tipo Centro de Proyección y Giros tienen el siguiente formato

| Foto | 0.0 | Xcentro de proyección | Ycentro de proyección | Zcentro de proyección |
| :--- | :--- | :--- | :--- | :--- |
| Matriz\[0\]\[0\] | Matriz\[1\]\[0\] | Matriz\[2\]\[0\] | Matriz\[0\]\[1\] | Matriz\[1\]\[1\] |
| Matriz\[2\]\[1\] | Matriz\[0\]\[2\] | Matriz\[1\]\[2\] | Matriz\[2\]\[2\] |  |

Es importante tener en cuenta los siguientes puntos:

* El nombre de la foto **no debe contener la extensión de la foto.**

Este formato, al contrario que el formato de los archivos de [centros de proyección y giros](configuracion-de-la-extension-digi3d.conicsensor.imu.md), no requiere ningún parámetro para configurar los ángulos de los giros ni el orden en el que se deben multiplicar estos para crear la matriz de giros de la imagen, pues el archivo ya almacena directamente esta matriz, por lo que es preferible al de centros de proyección y giros ya que no hay ninguna ambiguedad.

## Ejemplo de un archivo con este formato

```text
           10203      0.00000000    712190.65866     -5421.70427      2141.64057
 -0.998826566538 -0.043032486871 -0.022219249579  0.044887436532 -0.994826584290
 -0.091132789002 -0.018182629618 -0.092023215893  0.995590839510
           10204      0.00000000    712467.31074     -5421.46033      2142.08729
 -0.998156299394  0.005852235114  0.060413188330 -0.008439781976 -0.999053789663
 -0.042664920488  0.060106339601 -0.043096133286  0.997261225174
           10205      0.00000000    712742.34940     -5427.58093      2134.25255
 -0.998381920788 -0.035062185044  0.044768107222  0.033377402963 -0.998726145745
 -0.037842235363  0.046037910637 -0.036286760474  0.998280412409
           10206      0.00000000    713015.40531     -5432.99400      2131.90509
 -0.999983682533  0.005684289385 -0.000568789559 -0.005668454805 -0.999677010309
 -0.024773850743 -0.000709427583 -0.024770222338  0.999692919250
```

