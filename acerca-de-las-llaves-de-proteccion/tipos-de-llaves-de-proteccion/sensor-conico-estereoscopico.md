# Sensor Cónico Estereoscópico

| DLL que implementa esta extensión | Digi3D.ConicSensor.dll |
| :--- | :--- |
| Clave del registro donde se almacena la configuración de este sensor | HKEY\_LOCAL\_MACHINE\SOFTWARE\Digi21\Digi3D.NET\Digi3D\Extensiones\Digi3D.ConicSensor |

Carga [pares estereoscópicos](sensor-conico-estereoscopico.md) o fotos independientes cuyas imágenes han sido obtenidas mediante una cámara cónica.

Este es el sensor más completo de entre los sensores proporcionados por _Digi3D.NET_, pues permite obtener _relaciones entre fotos \(modelos\),_ _orientaciones de imágenes_ así como _calibraciones de cámaras_ de multitud de formatos de archivo todo ello de forma completamente transparente para el usuario.

Este sensor realiza las siguientes tareas:

* Implementa una serie de órdenes como [AEROTRI](aerotri.md), [ORI\_ABSOLUTA](ori_absoluta.md), [ORI\_INTERNA\_I](ori_interna_i.md), [ORI\_INTERNA\_D](ori_interna_d.md), [ORI\_RELATIVA](ori_relativa.md).
* Solicita al usuario las rutas a los archivos de aerotriangulación e imagen izquierda y derecha en la pestaña [Pestaña sensores fotogramétricos](pestana-sensores-fotogrametricos.md) del cuadro de diálogo de [Nuevo Proyecto](cuadro-de-dialogo-nuevo-proyecto.md).
* Permite cargar proyectos de otros programas mediante el [Panel Proyecto fotogramétrico](panel-proyecto-fotogrametrico.md).
* Carga orientaciones \(interna, relativa, absoluta, resultado de una aerotriangulación, etc.\) de distintos proveedores de forma automática.
* Transforma _Coordenadas Terreno_ a _Coordenadas Pixel_, para asistir a la [Ventana Fotogrametrica](ventana-fotogrametrica.md).

Este sensor permite cargar de forma nativa archivos de proyecto, orientaciones y calibraciones de cámaras de programas terceros, como por ejemplo _Summit Evolution_, pero el sensor por si mismo no implementa esta lógica, sino que delega estas acciones de importación en las distintas [Extensiones del Sensor Conico](extensiones-del-sensor-conico.md). 

Vea también

