# Lógica para transformar de coordenadas terreno a pixel

La misión principal de un sensor es transformar _Coordenadas Terreno_ a _Coordenadas Pixel_ para asistir a la [Ventana Fotogrametrica](ventana-fotogrametrica.md). Vamos a explicar aquí los pasos que realiza el sensor cónico para realizar esta tarea.

Cuando el sensor _Cónico Estereoscópico_ carga un modelo, asigna as siguiente orientación al modelo:

* [Orientación Absoluta](orientacion-absoluta.md).

Y las siguientes orientaciones a cada imagen:

* [Orientacion Exterior](orientacion-exterior.md).
* [Calibracion de cámara](calibracion-de-camara.md).

La _orientación absoluta_ no es imprescindible, ya que en el caso de haber cargado un modelo aerotriangulado \(utilizando un archivo de areotriangulación que proporcione orientaciones a las imágenes\), lo habitual es que no exista pues las orientaciones exteriores creadas con el resultado de la aerotriangulación ya están ubicadas y escaladas para trabajar directamente en coordenadas terreno. En caso de no existir una _orientación absoluta_, _Digi3D.NET_ crea una _virtual_ cuya entrada y salida son idénticas, es decir, si entran las coordenadas \(525327.45, 4462235.98, 112.1\), la salida para dicha orientación absoluta virtual será \(525327.45, 4462235.98, 112.1\), si por el contrario sí que se localiza y carga una orientación absoluta, la salida para dichas coordenadas dependerá de los parámetros de la orientación absoluta cargada.

Cuando el usuario mueve el dispositivo de entrada, se mueven las coordenadas terreno donde está ubicado el centro de la [Ventana Fotogrametrica](ventana-fotogrametrica.md). Ésta consulta al sensor activo las coordenadas pixel para las coordenadas terreno a las que se acaba de desplazar el usuario. Si el sensor activo es cónico estereoscópico, éste realiza las siguientes operaciones.

1. Transformar las Coordenadas Terreno a Coordenadas Modelo utilizando la Orientación Absoluta activa \(recuerda que si no se ha localizado ninguna, las Coordenadas Modelo devueltas por la orientación absoluta virtual coincidirán con las Coordenadas Terreno\).
2. Transformar las Coordenadas Modelo obtenidas en el paso anterior a Coordenadas Cámara mediante la Orientación Exterior asignada a cada cámara. Por lo tanto ahora tendremos dos tuplas de coordenadas \(X, Y, Z\) para la cámara izquierda y \(X, Y, Z\) para la cámara derecha.
3. Transformar las Coordenadas Cámara de cada una de las cámaras a Coordenadas Pixel para cada una de las cámaras mediante el archivo de Calibración de cámara asignado a cada cámara. Por lo tanto ahora tendremos coordenadas pixel \(X,Y\) para la cámara izquierda y coordenadas pixel \(X,Y\) para la cámara derecha.
4. Devolver las coordenadas pixel \(tanto para la cámara izquierda como para la cámara derecha\) a la ventana fotogramétrica para que dibuje cada imagen centrada en sus correspondientes coordenadas recién calculadas.

Vea también

