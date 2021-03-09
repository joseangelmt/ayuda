# LaImagen se mueve a saltos o con retraso al mover el dispositivo de entrada

Existen varios motivos por los cuales la imagen se puede mover a saltos en la ventana fotogramétrica:

1. Es posible que tu tarjeta gráfica sea una tarjeta gráfica antigua con un único núcleo.

   Las tarjetas gráficas modernas disponen de muchos núcleos. Lo normal es que tengan entre 32 y 512 núcleos. _Digi3D.NET_ realiza los cambios de brillo/contraste/gamma utilizando paralelismo en la tarjeta gráfica, lo que requiere que la tarjeta gráfica disponga de varios núcleos. Si tu tarjeta gráfica es antigua \(por ejemplo la _nVidia Quadro FX 1400_\), verás saltos o retraso en la ventana fotogramétrica.

   Puedes solucionar este problema indicando a _Digi3D.NET_ que no realice los cambios de brillo/contraste/gamma utilizando el hardware de la tarjeta, sino que los realice por software siguiendo  los siguientes pasos:

   1. Ejecuta _Digi3D.NET_.
   2. Selecciona la opción del menú _Herramientas/Configuración_. Aparecera el cuadro de diálogo _Configuración_.
   3. Despliega la sección _Estereoscopía_ y localiza la opción _Método para Brillo/Contraste_.
   4. Selecciona la opción _Software_.
   5. Acepta el cuadro de diálogo _Configuración_. 

2. Es posible que sea por una configuración incorrecta del puerto de comunicaciones del dispositivo de entrada.

   Si tu dispositivo de entrada utiliza un puerto serie del ordenador \(tienes manivelas o un TopoMouse antiguo\) es posible que el controlador del dispositivo tenga activos los _búferes_ y eso esté provocando que la comunicación entre Digi3D.NET y el dispositivo no sea en tiempo real.

   Puedes solucionar este problema cambiando la configuración del puerto _COM_ al que está conectado el dispositivo siguiendo los siguientes pasos:

   1. Ejecuta un explorador de archivos \(pulsando las teclas _Windows + E_\).
   2. Pulsa con el botón derecho del ratón en _Equipo_. Aparecerá un menú contextual.
   3. Selecciona la opción _Administrar_ del menú contextual. Aparecerá el programa _Administración de equipos._
   4. En el panel de la izquierda, selecciona la opción _Administrador de dispositivos_. En el panel central aparecerán todos los dispositivos del ordenador.
   5. Localiza la opción _Puertos \(COM y LPT\)_ y ábrela.
   6. Localiza el puerto de comunicaciones en el cual tienes conectado el dispositivo y haz doble _clic_. Aparecerá el cuadro de diálogo _Propiedades del puerto de comunicaciones_.
   7. Selecciona la pestaña _Configuración del puerto_ y pulsa el botón _Opciones avanzadas..._. Aparecerá el cuadro de diálogo _Configuración avanzada de COMx_.
   8. Deshabilita la opción _Usar búferes FIFO \(requiere UART compatible con 16550\)_ y pulsa el botón Aceptar.
   9. Pulsa el botón _Aceptar_ del cuadro de diálogo _Propiedades del puerto de comunicaciones._

