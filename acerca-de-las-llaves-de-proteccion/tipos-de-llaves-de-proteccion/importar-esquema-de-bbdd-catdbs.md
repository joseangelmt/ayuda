# Importar esquema de BBDD Catdbs

Para crear automáticamente el esquema de una base de datos en formato CATDBS, realizaremos los siguientes pasos:

1. Seleccionamos la opción del menú **BASE DE DATOS/Tablas/Importar esquema de una base de datos en formato Catdbs...** Aparecerá el cuadro de diálogo **Cadena de conexión**.
2. Si no disponemos de cadena de conexión a la base de datos, pulsamos el botón de los **tres puntos**. Aparecerá el cuadro de diálogo **Propiedades de vínculo de datos**.
3. **Seleccionamos el proveedor**, como por ejemplo _Microsoft OLE DB PRovider for SQL Server_. Pulsamos el botón **Siguiente**. Se seleccionará la pestaña **Conexión**.
4. Rellenamos todos los campos necesarios para conectarnos con la base de datos.
5. Pulsamos el botón **Probar conexión** para comprobar que los parámetros son correctos.
6. Pulsamos el botón **Aceptar**. Se cerrará el cuadro de diálogo **Propiedades de vínculo de datos** y aparecerá relleno el campo **Cadena de conexión de la base de datos** del cuadro de diálogo **Cadena de conexión**.
7. Pulsamos el botón **Aceptar.**

Si no hay errores en la BBDD y esta está en formato CATDBS, aparecerán automáticamente todas las tablas de la BBDD importada en la pestaña **Base de datos.**

Nota: Si quieres importar un esquema de BBDD de una base de datos _Microsoft Access_, debes seleccionar el proveedor _Microsoft JET_, pero este proveedor únicamente aparecerá en aplicaciones de 32 bits, pues Microsoft prohibe expresamente que aplicaciones de 64 bits puedan acceder a este proveedor. Debes instalar _Digi3D.NET versión de 32 bits_ para este caso.

