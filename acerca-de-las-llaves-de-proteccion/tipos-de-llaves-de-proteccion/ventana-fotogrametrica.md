# Ventana Fotogrametrica

La ventana fotogramétrica es una ventana que permite mostrar imágenes de gran tamaño a gran velocidad y sin consumir los recursos \(memoria, uso de procesador\) del ordenador.

Las misiones de la ventana fotogramétrica son las siguientes:

* Configurar la tarjeta gráfica para visualización estereoscópica si el modelo a cargar es estereoscópico.
* Mostrar imágenes a gran velocidad mostrando en el centro de la ventana un determinado píxel de las imágenes.
* Cambiar rápidamente el nivel de zoom de las imágenes mostradas.
* Realizar transformaciones geométricas a las imágenes como rotarlas en cualquier eje.
* Realizar transformaciones radiométricas a las imágenes como cambiar el brillo, contraste, gamma, etc.
* Mostrar un índice en el centro de la ventana.

La ventana fotogramétrica es agnóstica con respecto a las imágenes que está mostrando. Esta no entiende de ecuaciones de colinearidad \(utilizadas en los cálculos de cámaras cónicas\), ni entiende de polinomios RPC \(utilizados en los cálculos de las imágenes satelitales\) ni ningún otro tipo de cálculos para obtener las Coordenadas Pixel en las que tiene que mostrar las imágenes a partir de las Coordenadas Terreno que modificamos con el dispositivo de entrada. Tampoco sabe los archivos de configuración \(como archivos de calibración de cámaras, archivos de polinomios RPC, etc\) que debe solicitar al usuario para cargar un determinado modelo, ni sabe si tiene que solicitar al usuario una o dos o tres o X imágenes. La ventana fotogramétrica delega estas acciones \(solicitar al usuario las imágenes, cargarlas, transformar de _Coordenadas Terreno_ a _Coordenadas Pixel_ en los distintos [Sensores](sensores.md)\).

