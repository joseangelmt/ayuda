# Importar códigos de archivo .dgn

Este importador analiza el archivo .dgn seleccionado y añade a la tabla de códigos activos tantos códigos como capas se localicen en el archivo.

Si se indica opcionalmente un archivo [.cel](importar-codigos-de-archivo-.dgn.md), se añadirán además tantos códigos como células se localicen dentro del archivo.

## ![Show](../../.gitbook/assets/hs-heading-expanded.gif)Más información

El importador no solo añade a la tabla de códigos activa códigos, sino que añade tantos estilos como códigos.

  
El nombre de estos estilos estará formado por el siguiente patrón: _style\_\[nombre del código\]_, de manera que si se localiza en el archivo _.dgn_ una capa con nombre _cota_, se creará en la tabla de códigos activa el código _cota_ y el estilo _style\_cota_. El código tendrá asociado el estilo correspondiente con el color, grosor especificado en el archivo _.dgn_.

Se añadirán pues dos tipos de códigos a la tabla de códigos activa:

1. **Códigos extraídos de las capas del archivo .dgn:**

   Para este tipo de códigos, se puede especificar el tipo de entidad _dgn_ con el que se almacenarán las _líneas_ digitalizadas en _Digi3D.NET_.  
   Se pueden seleccionar las opciones: _LINE, LINESTRING y SHAPE_. La opción por defecto es _LINESTRING._  
   Los puntos digitalizados con _Digi3D.NET_ para estos códigos se almacenarán con el tipo _POINT_ ya que el importador no tiene manera de averiguar automáticamente qué célula asociar con el código.

2. **Códigos extraídos del archivo de células:**

   Para este tipo de códigos, se puede especificar el tipo de entidad _dgn_ con el que se almacenarán los _puntos_ digitalizados en _Digi3D.NET._  
   Se pueden seleccionar las opciones: _POINT, CELL y SHARED\_CELL_.

