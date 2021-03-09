# CALCULA\_GIRO

Calcula el giro entre la imagen izquierda y la imagen derecha del par estereoscópico.

## Parámetros

Esta orden no admite parámetros.

## Observaciones

El ángulo proporcionado, en graduación centesimal, permite girar una de la imágenes para contrarrestar este giro. Sólo se puede calcular si está realizada la **Orientación Relativa**.

Puedes ejecutar la orden de dos formas:

* Teclear **CALCULA\_GIRO** en la ventana de órdenes, y pulsar la tecla **Enter**.
* En el menú de la ventana principal de la aplicación seleccionar Digital -&gt;Ver-&gt;Calcular el giro entre las dos imágenes.

Al ejecutar la orden, Digi3D.NET calcula el giro y lo muestra en la pantalla de visualización estereoscópica:

Cálculo del giro entre las dos imágenes:  
El ángulo de la imagen derecha con respecto a la izquierda es de: 0.5405 grados centesimales.  
Pulsa una tecla para continuar ...

Digi3D.NET espera que el usuario pulse una tecla para volver a la ejecución de Digi3D.

Posteriormente podrás girar una imagen dicho ángulo con el archivo ejecutable **Girar.bat**, que se instala por defecto en el directorio de instalación. Este archivo llama a la orden [GIRAR](girar.md) que se ejecuta desde la línea de comandos. La ejecución de Girar.bat se efectúa desde **MS-DOS** y tiene la siguiente sintaxis:

**Girar &lt;Archivo imagen&gt; &lt;grados&gt;**

Este ejecutable, guarda la imagen original pero cambiándole el nombre al ponerle un carácter de subrayado delante. Después efectúa el giro a la imagen, con lo que la imagen girada tendrá el mismo nombre que la original.

Si se gira una de las imágenes, se debería volver a realizar la [Orientación Interna](orientacion-interna-1.md) de la misma, dado que al efectuar el giro cambian las Coordenadas Píxel referidas a dicha imagen.

Sin embargo, no es necesario que vuelvas a realizar la [Orientación Interna](orientacion-interna-1.md), porque el programa la recalcula de forma automática.

## Características de la orden

| Tipo de orden |  |
| :--- | :--- |
| Repite automáticamente |  |
| Opción del menú donde aparece la orden |  |
| Barra de herramientas en la que aparece la orden |  |
| Extensión |  |
| Variables relacionadas |  |

