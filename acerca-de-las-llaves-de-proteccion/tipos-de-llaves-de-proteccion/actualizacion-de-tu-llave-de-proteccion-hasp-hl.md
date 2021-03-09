# Actualizacion de tu llave de protección Hasp HL

Sigue las siguientes instrucciones si ya dispones de una llave de protección [Hasp HL](actualizacion-de-tu-llave-de-proteccion-hasp-hl.md).

Una vez finalizados los siguientes pasos tendrás instalado el driver de protección y habremos introducido en tu llave de protección los parámetros necesarios para poder ejecutar _Digi3D.NET._

Vamos a añadir la licencia de _Digi3D.NET_ a tu llave de protección, pero no te preocupes porque no vas a perder las licencias que ya tuviera tu llave. Si tenías una licencia de _Digi3D 2007_ por ejemplo, la vas a seguir teniendo, no se va a eliminar nada de tu llave de protección.

1. Descarga e instala el driver de protección [Sentinel HASP Run-time and Drivers setup](http://sentinelcustomer.safenet-inc.com/DownloadNotice.aspx?dID=8589947119) \(14.8MB aproximadamente\). Para comenzar con la descarga, pulsa el botón titulado _I Accept_ al final de esa página.
2. Haz clic en este enlace: [http://localhost:1947/\_int\_/devices.html](http://localhost:1947/_int_/devices.html). Aparecerá una página web titulada _Safenet Admin Control Center_. En el contenido principal de la página verás una tabla con varias columnas: _Location, Vendor, Key ID, Key Type, Configuration, Version, Sessions_ y _Actions_.
3. Asegúrate de que tienes conectada la llave de protección en su correspondiente puerto _USB_. La llave tiene un piloto que debe estar encendido. Si no está encendido, desconéctala y vuélvela a conectar. Espera un rato a que se instale su driver. Si no se enciende, prueba en otro puerto USB. Si sigue sin encenderse ponte en contacto con el soporte técnico de _Digi21_ en la siguiente dirección: [https://www.digi21.net/Contactar](https://www.digi21.net/Contactar)
4. En la tabla aparecerá tantas llaves de protección como se localicen tanto en tu propio ordenador como en la red de la empresa \(si es que el ordenador está conectado a la red\).
5. Localiza tu llave de protección. Será la única que tiene las siguientes características:

   | Location | Local |
   | :--- | :--- |
   | Vendor | 78585 |

6. Comprueba que en la columna _Version_ tienes el valor **3.25**. Si el valor que aparece en esta columna no es 3.25, sigue los pasos del tutorial [Actualizando el firmware de tu llave de protección Hasp HL](actualizando-el-firmware-de-tu-llave-de-proteccion-hasp-hl.md).
7. Descarga ejecuta el programa [ActualizarLlaveLDK.exe](http://digi21.blob.core.windows.net/download/ActualizarLlaveLDK.exe) Este programa sirve para analizar tu llave de protección y crear un archivo que nos va a permitir reprogramarla remotamente.
8. Aparecerá el programa _Sentinel HASP RUS_. Este programa tiene dos pestañas: _Collect Key Status Information_ y _Apply License Update_.
9. En la pestaña _Collect Key Status Information_ pulsa el botón _Collect Information._
10. Aparece el cuadro de diálogo _Save Key Status As_. Este cuadro de diálogo te va a permitir indicar la ubicación y nombre del archivo [.c2v](actualizacion-de-tu-llave-de-proteccion-hasp-hl.md) que nos vas a enviar.
11. Indica la ubicación y nombre del archivo _.c2v_ a crear.
12. Envíanos el archivo que acabas de crear a la la dirección de correo electrónico: [info@digi21.net](mailto:info@digi21.net) junto con la siguiente información:
    * Nombre de la empresa
    * N.I.F.
    * Dirección
    * Código postal
    * Persona de contacto
    * Teléfono
    * Correo electrónico
13. Te responderemos con un archivo con extensión [.v2c](actualizacion-de-tu-llave-de-proteccion-hasp-hl.md) que vas a utilizar para programar tu llave de protección.
14. Haz clic en el siguiente enlace: [http://localhost:1947/\_int\_/checkin.html](http://localhost:1947/_int_/checkin.html). Aparecerála página web titulada _Safenet Admin Control Center._
15. Pulsa el botón _Examinar._
16. Aparecerá el cuadro de diálogo titulado _Elegir archivos para cargar_.
17. Selecciona el archivo _.v2c_ que te habremos enviado por correo electrónico y pulsa el botón _Abrir_.
18. Pulsa el botón _Apply File_.

&lt;

Vea también

