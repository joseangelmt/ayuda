# La imagen se mueve al revés de lo esperado al mover las manivelas

Las manivelas emiten incrementos positivos o negativos en función de cómo estén físicamente soldados los cables del codificador.

Si están soldados en el orden A-B, al rotar la manivela en sentido horario los incrementos serán positivos. Si están soldados en orden B-A, al rotar la manivela en sentido horario los incrementos serán negativos.

Al ser un dispositivo analógico, para _Digi3D.NET_ es imposible saber a priori cómo están soldados los cables, de modo que es posible que al mover alguna de las manivelas el movimiento sea el contrario al esperado.

_Digi3D.NET_ multiplica cada incremento de los codificadores de las manivelas por una matriz matemática de 3x3, y permite que cambiemos los valores de dicha matrix, de modo que podremos solucionar el problema cambiando el signo de la manivela que esté comportándose de forma incorrecta.

Sigue los siguientes pasos para solucionar el problema:

1. Ejecuta _Digi3D.NET_. Aparecerá el cuadro de diálogo _Nuevo Proyecto._
2. Cierra el cuadro de diálogo _Nuevo Proyecto._
3. Selecciona la opción del menú _Herramientas/Configuración de dispositivos de entrada..._ Aparecerá el cuadro de diálogo _Configuración se dispositivos de entrada._
4. En el desplegable del cuadro selecciona el nombre de la tarjeta de codificadores a la que tienes conectadas las manivelas \(usualmente será _REST4_\).
5. Pulsa el botón _Comprobar..._ Aparecerá el cuadro de diálogo _Test de codificadores_.
6. Gira la manivela de la coordenada X en sentido horario. Los incrementos que debes ver en el campo X del cuadro de diálogo deben ser positivos.
7. Gira la manivela de la coordenada Y en sentido horario. Los incrementos que debes ver en el campo Y del cuadro de diálogo deben ser positivos.
8. Gira la manivela de la coordenada Z en sentido horario. Los incrementos que debes ver en el campo Z del cuadro de diálogo deben ser negativos.
9. Memoriza las manivelas que se están comportando de forma incorrecta.
10. Pulsa la tecla _Esc_ para cerrar el cuadro de diálogo _Test de codificadores_.
11. Pulsa el botón _Configurar_. Aparecerá el cuadro de diálogo _Parámetros para tarjetas serie_. Este cuadro de diálogo permite configurar el número de puerto serie donde está conectada la tarjeta de codificadores por un lado, y especificar los parámetros de la matriz de 3x3 por la cual _Digi3D.NET_ multiplica las coordenadas de cada uno de los codificadores.
12. Cambia el signo de la casilla correspondiente a la manivela o manivelas que se estén comportando de forma incorrecta.
13. Pulsa el botón _Aceptar._
14. Vuelve a pulsar el botón _Comprobar..._ para asegurarte de que ahora los movimientos son correctos. Si no es así, continúa con el punto 9.
15. Pulsa _Esc_ para cerrar el cuadro de diálogo _Test de codificadores._
16. Pulsa _Aceptar_ para cerrar el cuadro de diálogo _Configuración de dispositivos de entrada_.

