# Trabajando con ETRS89 y ED50

Es muy común que tengamos que trabajar \(en España\) en el sistema de coordenadas ETRS89 pero que tengamos que cargar archivos de referencia cuyas coordenadas están en ED50.

Digi3D.NET se encarga de realizar de forma automática la transformación entre ambos sistemas de forma transparente para el usuario.

A continuación vamos a ver cómo digitalizar un modelo fotogramétrico orientado en _ED50 / UTM Zone 30N_, vamos a trabajar en un archivo de dibujo en _ETRS89 / UTM Zone 30N_ y cargaremos un archivo de referencia antiguo que estaba en _ED50 / UTM Zone 30N_.

1. Descarga y descomprime el ejemplo [Bronchales ETRS89 ED50.zip](http://digi21.blob.core.windows.net/ejemplos/Bronchales%20ETRS89%20ED50.zip).
2. Ejecuta Digi3D.NET.
3. En el cuadro de diálogo _Nuevo proyecto_ selecciona la pestaña **Sensores fotogramétricos.**
4. Pulsa el botón de los tres puntos que aparece a la derecha de la ventana **Archivo de proyecto**. Aparecerá el cuadro de diálogo _Abrir_.
5. Localiza el archivo _108-109.d3d_ y pulsa el botón **Abrir.** Comprueba que se han rellenado todos los campos de la pestaña _Sensores fotogramétricos_ del cuadro de diálogo _Nuevo proyecto_. Puedes comprobar que el sistema de coordenadas de referencia asignado es _ED50 / UTM Zone 30N_. 
6. Pulsa el botón **Aceptar** del cuadro de diálogo _Nuevo proyecto._ Se abrirá una ventana fotogramétrica mostrando el modelo.

Ahora vamos a crear un archivo de dibujo en ETRS89 / UTM Zone 30N que es en el que vamos a digitalizar la cartografía. Nos interesa que la ventana de dibujo esté también en ese sistema de coordenadas.

1. Selecciona la opción del menú **Archivo/Nuevo-Abrir modelo fotogramétrico o archivo de dibujo...** Aparecerá el cuadro de diálogo _Nuevo proyecto_.
2. Selecciona la pestaña **Archivo de dibujo**.
3. Pulsa el botón de los tres puntos del campo **Archivo de dibujo.** Aparecerá el cuadro de diálogo _Abrir_.
4. Localiza la carpeta del ejemplo \(_Bronchales_\) y en el campo **Nombre** teclea el nombre del archivo de crear, por ejemplo 108-109. En tipo de archivo deja la opción por defecto \(que debería ser Archivos Digi de doble precisión\).
5. Pulsa el botón **Abrir**. Se cerrará el cuadro de diálogo _Abrir_.
6. Si en el campo **Sistema de coordenadas horizontal de la ventana de dibujo** aparece el valor _Heredar el sistema de coordenadas del primer archivo de dibujo_ salta al punto 12.
7. Haz clic en **Sistema de coordenadas horizontal de la ventana de dibujo.** Aparecerá un botón con tres puntos a la derecha.
8. Pulsa el botón de los **tres puntos**. Aparecerá el cuadro de diálogo _Sistema de coordenadas horizontal de la ventana de dibujo_.
9. Selecciona la opción **Heredar el sistema de coordenadas del primer archivo de dibujo cargado**.
10. Pulsa el botón **Aceptar** del cuadro de diálogo _Sistema de coordenadas horizontal de la ventana de dibujo_.
11. En **Motor de importación/exportación** selecciona la opción **Sistema de coordenadas de referencia horizontal**. Aparecerá a su derecha un botón con tres puntos.
12. Pulsa el botón con los **tres puntos**. Aparecerá el cuadro de diálogo _Sistema de coordenadas de referencia horizontal._
13. Si está seleccionada la casilla **Desconocido** desactívala.
14. Si aparece en la lista de **Sistemas de coordenadas de referencia memorizados** el sistema _ETRS89 / UTM Zone 30N_, selecciónalo y salta al punto 20.
15. Pulsa el botón **Buscar**. Aparecerá el cuadro de diálogo _Buscar sistema de coordenadas de referencia horizontal._
16. Pulsa el botón **Buscar por código EPSG**. Aparecerá el cuadro de diálogo _Búsqueda por código EPSG_.
17. Teclea el valor **25830** en el campo _Introduce el código EPSG del sistema de coordenadas**.**_
18. Pulsa el botón **Aceptar** del cuadro de diálogo _Búsqueda por código EPSG_.
19. Pulsa el botón **Aceptar** del cuadro de diálogo _Buscar sistema de coordenadas de referencia horizontal_.
20. Pulsa el botón **Aceptar** del cuadro de diálogo _Sistema de coordenadas de referencia horizontal._
21. Si quieres ver correctamente los colores de las entidades del archivo de dibujo que se va a cargar más adelante, en **Entorno/Tabla de códigos** selecciona el archivo **Digi.tab.xml** de la carpeta del ejemplo.
22. Pulsa el botón **Aceptar** del cuadro de diálogo _Nuevo proyecto_.

_Digi3D.NET_ en este momento crea el archivo _107-108.bind_, y le asigna el sistema de coordenadas _ETRS89 / UTM Zone 30N_.

En el mismo instante en que se carga este archivo, Digi3D.NET se da cuenta de que ya tenemos cargado un modelo en la ventana fotogramétrica. Analiza sus sistemas de coordenadas de referencia y se da cuenta de que como la ventana fotogramétrica está en _ED50 / UTM Zone 30N_ y la ventana de dibujo está en _ETRS89 / UTM Zone 30N_, es necesario crear una transformación.

Digi3D.NET busca las posibles transformaciones entre _ED50 / UTM Zone 30N_ y _ETRS89 / UTM Zone 30N_ y se da cuenta de que hay muchas \(13 posibles transformaciones\), por lo tanto nos muestra el cuadro de diálogo **Selecciona la transformación que deseas aplicar** mostrando todas las posibles transformaciones.

Este cuadro de diálogo muestra tantos botones como operaciones existen y estos botones están ordenados de mejor precisión a peor precisión.

La mejor precisión es la operación **14**, que es el tercer botón \(no aparece la primera porque teóricamente tienen la misma precisión {0,2} las tres primeras transformaciones. Selecciona la operación _ED50 a ETRS89 \(14\)_, que como puedes comprobar utiliza la versión _IGN-ESP v3_, es decir, la tercera versión del archivo de rejilla del IGN.

Pulsa ese botón y se abrirá el archivo de dibujo.

Ahora vamos a comprobar que efectívamente se está realizando una transformación en tiempo real:

1. Despliega el segundo desplegable de la barra de estado de la ventana fotogramétrica, y selecciona la opción **Terreno**. A partir de este momento cuando desplaces la ventana fotogramétrica se mostrará a la derecha de este desplegable coordenadas terreno.
2. Selecciona la opción del menú **Ventana fotogramétrica/Ir a coordenadas.** Aparecerá el cuadro de diálogo _Ir a coordenadas terreno_.
3. Introduce las siguientes coordenadas:

   | X | 619567.94 |
   | :--- | :--- |
   | Y | 4485076.883 |
   | Z | 1609.768 |

4. Pulsa el botón **Aceptar** del cuadro de diáogo _Ir a coordenadas terreno_. Comprobarás que la ventana fotogramétrica se desplaza a la esquina de un depósito. En la barra de estado de la ventana fotogramétrica se mostrarán las corodenadas que acabamos de introducir.
5. Comprueba que en la barra de herramientas **Coordenadas** las coordenadas que aparecen **no coinciden** con las de la barra de estado de la ventana fotogramétrica, pues las coordenadas de la ventana fotogramétrica están en _ED50 / UTM Zone 30N_ y las de la barra de herramientas \(que muestran las coordenadas de la ventana de dibujo\) están en ETRS89 / UTM Zone 30N.

Todo lo que digitalicemos a partir de ahora se digitalizará en _ETRS89 / UTM Zone 30N_ aunque el modelo fotogramétrico esté orientado en _ED50 / UTM Zone 30N_.

Ahora vamos a cargar un modelo de case. Este modelo se digitalizó hace muchos años en _ED50 / UTM Zone 30N_. Nuestra intención es cargarlo sin tenerlo que transformar previamente. Digi3D.NET lo va a hacer automáticamente.

1. Abre el panel **Archivos de dibujo** mediante la opción del menú **Ventana/Archivos de dibujo.**
2. Pulsa el botón de la **carpeta** de la barra de herramientas del panel _Archivos de dibujo_. Aparecerá el cuadro de diálogo _Abrir_.
3. Selecciona el archivo **Cartográfía en ED50 - UTM Zone30N.bind**.
4. Pulsa el botón **Abrir** del cuadro de diálogo _Abrir_. Aparecerá el cuadro de diálogo _Parámetros de importación/Exportación_**.**
5. En este cuadro de diálogo podemos indicar el sistema de coordenadas de referencia a asignar al archivo de dibujo **suponiendo que no tenga uno asignado,** pero los archivos .BIND siempre tienen uno asignado, así que seleccionemos lo que seleccionemos en el campo Sistema de coordenadas de referencia horizontal aquí el programa no va a hacer caso pues tendrá prioridad el sistema que ya tiene asignado el archivo de dibujo, así que sin tocar nada en este cuadro de diálogo, pulsa el botón **Aceptar**.
6. Digi3.NET se dará cuenta de que los sistemas de coordenadas de referencia de la ventana de dibujo y del archivo que estamos cargando no coinciden: El de la ventana de dibujo es _ETRS89 / UTM Zone 30N_ y el del archivo de dibujo _ED50 / UTM Zone 30N_, y al igual que cuando te intentó localizar una transformación entre la ventana fotogramétrica y el archivo de dibujo el programa nos preguntó cual de entre todas las posibles transformaciones nos interesa, pues ahora va a suceder lo mismo. El programa nos va a mostrar el mismo cuadro de diálogo preguntándonos cual es la transformación que nos interesa. Selecciona al igual que en el caso anterior la transformación **14.**

_Digi3D.NET_ tralizará de forma transparente la transformación de _ED50 a ETRS89_ y como resultado veremos la cartografía en la ventana de dibujo en _ETRS89 / UTM Zone 30N_ y en la ventana de dibujo en _ED50 / UTM Zone 30N_, todo ello sin tocar el archivo de dibujo que sigue estando en _ED50 / UTM Zone 30N_.

