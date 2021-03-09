# Los vectores no encajan en su sitio al transformar AKML

Si al cargar en _Google Earth_ un archivo _.KML_ generado con _Digi3D.NET_ los vectores no están en su sitio, el problema es que se ha realizado incorrectamente la transformación de coordenadas de la ventana de dibujo cuando se realizó la transformación del archivo a coordenadas geográficas _WGS 84_, que es el sistema de coordenadas en el que se deben almacenar las coordenadas en un archivo _.KML_.

Los motivos pueden ser varios:

1. Si existen varias transformaciones entre el sistema de coordenadas de la ventana de dibujo, es posible que se haya seleccionado una transformación con poca precisión cuando se mostró el cuadro de diálogo _Selecciona la transformación que quieres aplicar_. En este caso, **localiza una transformación mejor**.
2. Si no existen varias transformaciones el error no puede ser de haber elegido una transformación con poca precisión, así que es posible que el archivo de dibujo no tenga asociado una georeferenciación correcta. Por ejemplo, es posible que el archivo tenga asociado como sistema de coordenadas de referencia _WGS 84/ UTM Zone 30N_ cuando en realidad debería ser _WGS84 / UTM Zone 19N,_ al transformarse el archivo, _Digi3D.NET_ considera que las entidades están en el huso _30_ cuando en realidad están en el _19_, y por eso lógicamente los vectores no aparecen en su sitio al cargar el archivo en _Google Earth_. Si este es el caso, sigue las instrucciones del tutorial [Cambiando el Sistema de Coordenadas de Referencia asociado a un archivo de dibujo](cambiando-el-sistema-de-coordenadas-de-referencia-asociado-a-un-archivo-de-dibujo.md).

