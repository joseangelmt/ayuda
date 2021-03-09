# Creando una llave de protección temporal

Si no dispones de una llave de protección [Hasp HL](creando-una-llave-de-proteccion-temporal.md) tendrás que crear una llave de protección temporal en tu ordenador. Esta llave es una llave de software, de modo que no es necesario que te enviemos ningún hardware y podrás comenzar a utilizar _Digi3D.NET_ rápidamente.

  
Cuando finalices este tutorial, tendrás instalada en tu ordenador una llave de protección temporal con una duración máxima de 30 días. Este tipo de llaves se utilizan para evaluación \(tanto del programa como del ordenador donde se instala\). Transcurridos los 30 días sin tener ningún problema de hardware tendremos que convertirla en una llave de protección permanente.

1. Descarga el programa: [http://digi21.blob.core.windows.net/download/DriverHaspDigi3D.exe](http://digi21.blob.core.windows.net/download/DriverHaspDigi3D.exe). No indiques a tu explorador de Internet que quieres ejecutarlo, indica que quieres guardarlo. En el siguiente paso vas a abrir una consola de _DOS_ para ejecutar el programa pasándole parámetros, de modo que te recomendamos que lo almacenes en un directorio fácil de llegar con la consola, como por ejemplo en _**C:\**_
2. Pulsa la combinación de teclas _Windows + R_.
3. Aparecerá la ventana _Ejecutar_.
4. Teclea _CMD_ y pulsa el botón _Aceptar_.
5. Se abrirá una consola de _DOS_.
6. Mediante el comando _CD_ desplázate al directorio donde has copiado el programa.  
   Si por ejemplo has copiado el programa _DriverHaspDigi3D_ en el directorio c:\ ejecuta el siguiente comando:       

   c:\Users\usuario&gt; cd c:\

7. Ejecuta el programa tecleando su nombre y pasándole como parámetro el parámetro _-install_

   c:\&gt; DriverHaspDigi3D -install

8. Aparecerá una ventana titulada _Sentinel Run-time Environment Installer..._
9. Transcurrido un tiempo se mostrará una ventana con el mensaje _Operation successfully completed_. Ya tienes instalada la llave de proteción temporal en tu ordenador.
10. Pulsa en el siguiente enlace [http://localhost:1947/\_int\_/devices.html](http://localhost:1947/_int_/devices.html) para comprobar que la llave está instalada correctamente. Aparecerá una página web titulada _Safenet Admin Control Center_. En el contenido principal de la página verás una tabla con varias columnas: _Location, Vendor, Key ID, Key Type, Configuration, Version, Sessions_ y _Actions_.
11. En la tabla aparecerá tantas llaves de protección como se localicen tanto en tu propio ordenador como en la red de la empresa \(si es que el ordenador está conectado a la red\).
12. Localiza tu llave de protección. Será la única que tiene las siguientes características:  


    | Location | Local |
    | :--- | :--- |
    | Vendor | 78585 |
    | Key Type | HASP SL Legacy |

Vea también

