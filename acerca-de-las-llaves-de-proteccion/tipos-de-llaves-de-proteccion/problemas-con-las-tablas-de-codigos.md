# Problemas con las tablas de códigos

Si vinculas una tabla de códigos cualquiera _\*.TAB.xml_ a tu archivo de dibujo, comienzas a digitalizar entidades y al volver a abrir el archivo las entidades aparecen en color gris, como si Digi3D.NET no reconociese esos códigos, es podible que la tabla no tenga configurados los parámetros de exportación de dichos códigos.

Si es así, cada vez que abras el archivo, en el Panel de tareas, Digi3D.NET, avisará con un mensaje de advertencia "_No se han localizado parámetros para traducir a .bind \(binarios Digi de doble precisión\) entidades con el código: ..._"

La solución es fácil, sólo tienes que abrir la tabla de códigos con el programa externo [Editor de tablas de códigos](editor-de-tablas-de-codigos.md) y seleccionar la opción de menú **Códigos/Completar parámetros de importación/exportación**.

