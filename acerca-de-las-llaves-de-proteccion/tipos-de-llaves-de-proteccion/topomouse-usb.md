# Topomouse USB

Digi3D.NET se comunica de forma nativa con el dispositivo de entrada Topomouse USB distribuido por Pacific Geoproducts.

Para poder comunicarse con este dispositivo es necesario tener instalado el controlador USBXpress desarrollado por Silicon Labs y a continuación indicar a Digi3D.NET que se desea utilizar dicho dispositivo como dispositivo de entrada.

**Atención: Los drivers de versiones anteriores a la 4.0 tienen el problema de que pueden bloquear el ordenador. Asegúrate de que el driver que tienes instalado o vas a instalar es el de versión 4.0 o superior. El día que se escribió esta página de la ayuda el driver más moderno es el que tiene versión 4.0.**

1. Descargua el programa [USBXpress Development Kit](http://www.silabs.com/products/mcu/Pages/USBXpress.aspx) de la página de descargas de Silicon Labs.
2. Este programa que acabas de descargar no es el driver, pero uns vez instalado aparecerá un directorio donde sí que está el instalador del driver.
3. Instala el programa.
4. Se creará en el directorio C:\Silabs\MCU\USBXpress\_SDK\Driver una carpeta con el instalador del driver del TopoMouse.
5. Ejecuta el archivo USBXpressInstaller\_x64 si el sistema operativo de tu ordenador es de 64 bits o el archivo USBXpressInstaller\_x86 si el sistema operativo de tu ordenador es de 32 bits.
6. Desinstala el programa USBXpress Development Kit puesto que ya no es necesario, lo hemos instalado únicamente para tener acceso al instalador del driver que acabamos de instalar.
7. Conecta el Topomouse en un puerto USB libre del ordenador.
8. Arranca Digi3D.NET.
9. Selecciona la opción del menú _Herramientas/Configuración de dispositivos de entrada..._
10. Aparecerá el cuadro de diálogo _Configuración de dispositivos de entrada_.
11. Despliega el cuadro de opciones en el que aparecen los distintos dispositivos de entrada y selecciona la opción _TopoMouse Usb_.
12. Pulsa el botón _Comprobar_ para comprobar que Digi3D.NET se comunica con el dispositivo.
13. Aparecerá el cuadro de diálogo _Test de codificadores._
14. Desplaza dispositivo y pulsa alguno de sus botones, deberías ver que varían los valores que aparecen en los campos X, Y, Z y Pedal.
15. Pulsa la tecla _Escape_ para cerrar el cuadro de diálogo _Test de codificadores_.
16. Pulsa el botón _Aceptar_ en el cuadro de diálogo _Configuración de dispositivos de entrada._

