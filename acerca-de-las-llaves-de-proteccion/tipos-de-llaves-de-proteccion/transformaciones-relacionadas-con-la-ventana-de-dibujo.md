# Transformaciones relacionadas con la ventana de dibujo

La ventana de dibujo se comunica con los archivos de dibujo cargados \(cuando le ordena al archivo que almacene una entidad o cuando carga una entidad del archivo de dibujo\) por un lado y con la ventana fotogramétrica por otro \(para ordenar a la ventana fotogramétrica que se desplace a una ubicación o para enviarle geometrías para que se visualicen en la ventana fotogramétrica\).

Como cada archivo de dibujo tiene asociado su propio sistema de referencia de coordenadas, la ventana de dibujo tendrá que transformar las coordenadas de las geometrías que se envían a los archivos de dibujo \(y viceversa al cargar entidades del archivo de dibujo\) mediante una transformación.

Si hay una ventana fotogramétrica abierta, la ventana de dibujo le enviará a esta las geometrías cargadas para que se muestren en la ventana fotogramétrica. Como la ventana fotogramétrica tiene su propio sistema de referencia de coordenadas tal y como se explica en [Ventana Fotogramétrica](ventana-fotogrametrica-1.md), será necesario transformar las coordenadas de las geometrías del sistema de coordenadas de la ventana de dibujo al sistema de coordenadas de la orientación mediante una transformación.

Vea también

## Sistemas de referencia de coordenadas

