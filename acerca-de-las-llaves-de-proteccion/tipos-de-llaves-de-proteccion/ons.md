# ONS

Activa el código \(o códigos\) que se desea visualizar en la pantalla de visión estereoscópica.

## Parámetros

| Número de parámetro | Descripción | Opcional |
| :--- | :--- | :--- |
| 1 | Código/os que se mostrarán en la pantalla de dibujo | Si. Por defecto al abrir un fichero de dibujo aparecen todos los códigos visibles |

### Ejemplos

ONS=\*

Visualiza todos los códigos en pantalla

ONS=02\*

Visualiza todos los códigos que comiencen por 02

ONS=020123

Visualiza solamente los elementos cuyo código sea 020123 

## Observaciones

En el caso de que se quiera activar la visualización en la pantalla de dibujo, se pueden emplear las órdenes [ON](on.md) u [OND](ond.md).

Podemos especificar el tipo de entidad a mostrar, para cada uno de los códigos: Líneas, Puntos ó Textos.

Digi3D nos permite cargar archivos de muestra de códigos o guardar uno que generemos nostros:

* Cargar de archivo...: carga un archivo de muestra de códigos previamente generado y guardado.
* Guardar en archivo...: podemos guardar mediante un nombre, la lista de códigos seleccioanada para una posterior utilización. Los archivos generados estarán en formato .xml.

## Características de la orden

| Tipo de orden | [Orden interactiva](ons.md) |
| :--- | :--- |
| Repite automáticamente | No |
| Opción del menú donde aparece la orden | _Esta orden no tiene asociada ninguna opción de menú_ |
| Barra de herramientas en la que aparece la orden | _Esta orden no tiene asociado ningún botón en ninguna barra de herramientas_ |
| Extensión | DigiNG.OrdenesRaster.dll |

Vea también

