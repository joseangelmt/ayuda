# CAL\_ORTO

Calcula Ortofotografías Digitales mediante Digi3D.

## Parámetros

Esta orden no admite parámetros.

## Observaciones

Requiere de la existencia de una imagen raster orientada y un modelo digital del terreno de la zona a rectificar. Por lo que antes de ejecutar la orden, deben haberse realizado los siguientes pasos:

1. Cargar la imagen raster mediante cuadro de diálogo Nuevo Proyecto Estereoscópico. La imagen debe tener un fichero .orientacion.xml con los parámetros de las Orientaciones Interna y Externa.
2. Se debe tener disponible en memoria un modelo digital del terreno, en formato del programa MDTop, de la zona que se va a procesar. Para ello bien se utilizan las órdenes [MDTPC](mdtpc.md) y [TRIANGULAR](triangular.md).
3. Debe definirse una entidad cerrada que delimite el área de la imagen que se va a rectificar. Para evitar problemas en la selección posterior de esta entidad se debería registrar con una Z activa próxima a la del terreno. Para ello se debe ejecutar la orden [MDT\_MUEVE\_Z](mdt_mueve_z.md).

Una vez realizados estos pasos previes, puedes ejecutar la orden _CAL\_ORTO_. Digi3D.NET solicitará que selecciones la entidad que delimitará la Ortofotografía Digital.

Una vez seleccionada tendrás que definir las características de la Ortofotografía que se va a generar:

* Tamaño del pixel: dónde se define el tamaño del pixel de la Ortofotografía. Este tamaño se especifica en el pliego de condiciones y depende de la escala final.
* Tamaño de la imagen obtenida: tamaño en pixeles. Este tamaño depende del tamaño del pixel.
* Peso de la imagen obtenida: peso en Mb. este tamaño depende del tamaño del pixel.
* Tipo de interpolación: Puedes elegir entre los siguientes tipos:
  * Venico mas próximo: es la más rápida pues sólo determina cuál es el pixel más próximo. Tiene el inconveniente de que los elementos lineales de la imagen aparecen como líneas quebradas \(efecto escalera\).
  * Bilineal: tarda más tiempo que el método anterior, pero no se nota tanto el efecto escalera. Tiene en cuenta los 4 píxeles más cercanos.
  * Bicúbica: es la interpolación que más tarda pero la que mejores resultados ofrece. Toma para la interpolación los píxeles más próximos.
* Archivo a generar: nombre y directorio donde se almacenará la imagen resultante.

Puedes ejecutar esta orden directamente en la línea de comandos:

C: \CAL\_ORTO=&lt;tipo interpolación&gt; &lt;ruta completa de la orto con extensión&gt; &lt;código entidad límite&gt;

### Ejemplo:

cal\_orto=2 C:\Proyecto2\orto3.tif 020256

En este caso, la entidad límite debe ser la única entidad con el código dado y debe ser un elemento cerrado. Se deben tener cargados también la imagen original y el MDT, y se debe haber definido la variable [DA](da.md).

## Características de la orden

| Tipo de orden | [Orden interactiva](cal_orto.md) |
| :--- | :--- |
| Repite automáticamente | No |
| Opción del menú donde aparece la orden | _Esta orden no tiene asociada ninguna opción de menú_ |
| Barra de herramientas en la que aparece la orden | _Esta orden no tiene asociado ningún botón en ninguna barra de herramientas_ |
| Extensión | DigiNG.OrdenesStandard.dll |
| Variables relacionadas | No tiene variables relacionadas |

