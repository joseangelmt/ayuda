# Cambiando el Sistema de Coordenadas de Referencia a un archivo .bin

Los archivos de dibujo en formato [.bin](cambiando-el-sistema-de-coordenadas-de-referencia-a-un-archivo-.bin.md) no almacenan dentro del propio archivo de dibujo el sistema de coordenadas de referencia, sino que lo almacenan en un archivo [.prj](cambiando-el-sistema-de-coordenadas-de-referencia-a-un-archivo-.bin.md) asociado, de modo que la forma de cambiar el sistema de coordenadas de referencia de un archivo .BIN consistirá en cambiar el contenido del archivo .PRJ o de eliminarlo y crear otro indicando en el momento de la carga del archivo de dibujo el sistema de coordenadas de referencia correcto.

A continuación los pasos necesarios para realizar las siguientes tareas:

1. Crear un archivo .BIN con el sistema de coordenadas de referencia _WGS 84 / UTM Zone 30N_.
2. Cambiar el sistema de coordenadas de referencia a _WGS 84 / UTM Zone 19N_.

Sigue los siguientes pasos:

1. Ejecuta **Digi3D.NET.**
2. Selecciona la pestaña **Archivo de dibujo** en el cuadro de diálogo **Nuevo proyecto**.
3. Pulsa el botón **...** que aparece a la derecha de la ventana bajo **Archivo de dibujo**. Aparecerá el cuadro de diálogo **Abrir**.
4. Localiza la ruta donde quieres crear el archivo .BIN, como por ejemplo el **Escritorio**.
5. En el desplegable de tipos de archivo, selecciona **Archivos Digi \(\*.bin; \*.bik\)**_**.**_
6. En el campo **Nombre** indica el nombre del archivo de dibujo a crear, como por ejemplo **Prueba cambio de SSCCRR**.
7. Pulsa el botón **Abrir**.
8. Comprueba que en la ventana bajo **Archivo de dibujo** aparece la ruta completa del archivo .BIN que se va a crear.
9. Localiza la sección **Motor de importación/exportación** y desplíégala si no está desplegada. Aparecerán las propiedades específicas para archivos con extensión .BIN, como los sistemas de coordenadas de referencia a asignar al archivo a la hora de crearlo y la precisión y el origen global del archivo.
10. En **Sistema de coordenadas de referencia horizontal** \(de la sección Motor de importación/exportación\), pulsa el botón de los tres puntos. Aparecerá el cuadro de diálogo **Sistema de coordenadas de referencia horizontal**.
11. Si la casilla **Desconocido** está activa, desactívala.
12. Si puedes localizar en la lista **Sistemas de coordenadas de referencia memorizados** el sistema de coordenadas **WGS 84 / UTM Zone 30N** selecciónalo y continúa con el punto **20**.
13. Pulsa el botón **Buscar**. Aparecerá el cuadro de diálogo **Buscar sistema de coordenadas de referencia horizontal.**
14. Pulsa el botón **Buscar por código EPSG**. Aparecerá el cuadro de diálogo **Búsqueda por código EPSG**.
15. Teclea el valor **32630** en el campo **Introduce el código EPSG del sistema de coordenadas.**
16. Pulsa el botón **Aceptar**.
17. Comprueba que el cuadro de diálogo **Buscar sistema de coordenadas de referencia horizontal** ahora está mostrando los parámetros del sistema de coordenadas de referencia 32630 que es el sistema **Proyectado, WGS 84 / UTM Zone 30N**.
18. Pulsa el botón **Aceptar**.
19. Pulsa el **Memorizar.** Comprueba que ahora aparece el sistema de coordenadas de referencia **WGS 84 / UTM Zone 30N** en la lista **Sistemas de coordenadas de referencia memorizados.**
20. Pulsa el botón **Aceptar**.
21. Comprueba que ahora el campo **Sistema de coordenadas de referencia horizontal** de la sección **Motor de importación / exportación** es **WGS 84 / UTM Zone 30N.**
22. Pulsa el botón **Aceptar** del cuadro de diálogo **Nuevo proyecto.** Se creará el archivo de dibujo y Digi3D.NET abrirá una ventana para comenzar a dibujar entidades sobre ese archivo.
23. Selecciona la opción del menú **Ventana/Archivos de dibujo**. Aparecerá el panel de **Archivos de dibujo** mostrando el nombre del archivo de dibujo.
24. Pulsa con el **botón derecho del ratón** sobre el nombre del archivo de dibujo en el panel **Archivos de dibujo.** Aparecerá un menú contextual.
25. Selecciona la opción del menú **Mostrar sistema de coordenadas de referencia horizontal...** Aparecerá el cuadro de diálogo **Parámetros del sistema de coordenadas de referencia horizontal**.
26. Comprueba que el sistema asociado al archivo de dibujo es **WGS 84 / UTM Zone 30N**.
27. Pulsa el botón **Aceptar**.
28. Cierra Digi3D.NET.

Ya tenemos nuestro archivo de dibujo en sistema de coordenadas de referencia WGS 84 / UTM Zone 30N. En realizad no se ha creado únicamente el archivo .BIN, sino que también se ha creado un archivo .PRJ asociado.

Cambiar el sistema de coordenadas de referencia del archivo .BIN es muy sencillo, tan solo tendremos que cambiar el contenido del archivo .PRJ o crear uno nuevo.

1. Localiza con el explorador de archivos el archivo .PRJ creado en el paso anterior.
2. Elimina el archivo .PRJ.
3. Ejecuta **Digi3D.NET.**
4. Localiza la sección **Motor de importación/exportación** y desplíégala si no está desplegada. Aparecerán las propiedades específicas para archivos con extensión .BIN, como los sistemas de coordenadas de referencia a asignar al archivo a la hora de crearlo y la precisión y el origen global del archivo.
5. En **Sistema de coordenadas de referencia horizontal** \(de la sección Motor de importación/exportación\), pulsa el botón de los tres puntos. Aparecerá el cuadro de diálogo **Sistema de coordenadas de referencia horizontal**.
6. Si la casilla **Desconocido** está activa, desactívala.
7. Si puedes localizar en la lista **Sistemas de coordenadas de referencia memorizados** el sistema de coordenadas **WGS 84 / UTM Zone 19N** selecciónalo y continúa con el punto **15**.
8. Pulsa el botón **Buscar**. Aparecerá el cuadro de diálogo **Buscar sistema de coordenadas de referencia horizontal.**
9. Pulsa el botón **Buscar por código EPSG**. Aparecerá el cuadro de diálogo **Búsqueda por código EPSG**.
10. Teclea el valor **32619** en el campo **Introduce el código EPSG del sistema de coordenadas.**
11. Pulsa el botón **Aceptar**.
12. Comprueba que el cuadro de diálogo **Buscar sistema de coordenadas de referencia horizontal** ahora está mostrando los parámetros del sistema de coordenadas de referencia 32630 que es el sistema **Proyectado, WGS 84 / UTM Zone 19N**.
13. Pulsa el botón **Aceptar**.
14. Pulsa el **Memorizar.** Comprueba que ahora aparece el sistema de coordenadas de referencia **WGS 84 / UTM Zone 19N** en la lista **Sistemas de coordenadas de referencia memorizados.**
15. Pulsa el botón **Aceptar**.
16. Comprueba que ahora el campo **Sistema de coordenadas de referencia horizontal** de la sección **Motor de importación / exportación** es **WGS 84 / UTM Zone 19N.**
17. Pulsa el botón **Aceptar** del cuadro de diálogo **Nuevo proyecto.** Se abrirá el archivo de dibujo. Se intentará localizar el archivo .PRJ asociado. Como no se encuentra se creará uno con los parámetros indicados en el cuadro de diálogo **Nuevo proyecto**, de modo que se creará uno con los datos de _WGS 84 / UTM Zone 19N_.
18. Cierra Digi3D.NET.

