# Ver el primer código de las entidades con múltiples códigos

Por defecto _Digi3D.NET_ está configurado para dibujar primero el primer código, segundo el siguiente código y así sucesivamente cuando tiene que dibujar una entidad con múltiples códigos.

Esto quiere decir que si todos los códigos de la entidad tienen el mismo grosor, lo que ves en pantalla es el último código de la entidad, pues el resto de códigos quedan ocultos al dibujarse el último encima de ellos.

Si te interesa que el comportamiento sea el contrario, es decir, que se dibuje primero la última entidad, luego la anterior y al final el primer código de la entidad sigue los siguientes pasos:

1. Ejecuta _Digi3D.NET_. Aparecerá el cuadro de diálogo _Nuevo Proyecto_.
2. Cierra el cuadro de diálogo _Nuevo Proyecto_.
3. Selecciona la opción del menu _Herramientas/Configuración_. Aparecerá el cuadro de diálogo _Configuración_.
4. Localiza y abre la sección _DigiNG_.
5. Cambia la opción _Orden dibujo \(multicódigo\)_ de _Primer código primero_ a _Último código primero_.
6. Acepta el cuadro de diálogo _Configuración_. Aparecerá un cuadro de mensaje indicando que hay que reiniciar la aplicación.
7. Reinicia _Digi3D.NET_.

