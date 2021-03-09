# Transformando coordenadas Z de elipsoidales a ortométricas

Supongamos que tenemos un conjunto de coordenadas proyectadas _X,Y_ con la coordenadas _Z_ medida en elipsoidal y queremos transformar dichas coordenadas en _X,Y_ proyectadas y con la coordenada _Z_ ortométrica.

Utilizaremos el programa [Transformador Universal De Coordenadas](transformador-universal-de-coordenadas.md) para realizar dicha operación.

Si intentamos localizar mediante el [Cuadro de diálogo Sistema de Referencia de Coordenadas](cuadro-de-dialogo-sistema-de-referencia-de-coordenadas.md) el sistema de referencia de coordenadas origen \(_X_,_Y_ proyectado y  elipsoidal\), no seremos capaces, pues el estándar _OpenGis_ no lo contempla. Puedes aprender los tipos de sistemas de referencia de coordenadas soportados en [Tipos de Sistemas de Referencia de Coordenadas](tipos-de-sistemas-de-referencia-de-coordenadas.md).

Sin embargo es posible realizar la transformación realizando los siguientes pasos:

1. Indica que el sistema de referencia de coordenadas de referencia origen es uno compuesto _Proyectado + desconocido_, como por ejemplo _ETRS89 / UTM Zona 30N + desconocido_.
2. Indica que el sistema de referencia de coordenadas de referencia destino es uno geográfico 3D, como por ejemplo _WGS 84_.
3. El programa Transformador Universal de Coordenadas preguntará cómo transformar la coordenada Z WGS84 a desconocido. Selecciona la opción **Considerar que el sistema de coordenadas vertical de ambos sistemas es idéntico.**
4. Pega las coordenadas origen en la ventana inferior izquierda. En la derecha ya tienes geográficas 3D. Como hemos indicado que no se realice ninguna transformación en la componente vertical y las coordenadas Z ya eran elipsoidales, ya tenemos coordenadas Latitud, Longitud, H \(elipsoidal\) .
5. Copia el resultado al portapapeles.
6. Ahora indica que el sistema de referencia de coordenadas origen es el sistema geográfico 3D \(como por ejemplo _WGS 84_\).
7. Indica que el sistema de referencia de coordenadas destino es el sistema proyectado destino \(indicando ya bien el sistema vertical, como por ejemplo _EGM08 Rednap Península_\).
8. Pega las coordenadas geográficas 3D en la parte inferior izquierda del programa.
9. Obtendrás el resultado en la parte inferior derecha.

## Vídeo

