# Digi3D.ConicSensor.Inpho

|  Orientaciones | Calibración de cámaras | Proyectos |
| :--- | :--- | :--- |
|  |  |  |

Esta extensión hace que _Digi3D.NET_ sea compatible con archivos creados con el programa _Inpho._

## Tipos de archivo soportados

Permite cargar _orientaciones_ a partir de las siguientes extensiones de archivos:

| Extensión | Descripción | ¿Cuantos archivos? | Proporciona Sistema de Referencia de Coordenadas |
| :--- | :--- | :--- | :--- |
| _.prj_ | Archivo con parámetros de orientación externa, calibración de cámaras y de proyectos. | Un archivo por proyecto. | Si, pues dentro del archivo _.prj_ aparece una [cadena Wkt](cadenas-well-known-text.md) indicando el [Sistema de Referencia de Coordenadas](sistemas-de-referencia-de-coordenadas.md) a asociar a las orientaciones proporcionadas por el archivo. |

Permite cargar _calibraciones de cámara_ a partir de las siguientes extensiones de archivos:

| Extensión | Descripción | ¿Cuantos archivos? |
| :--- | :--- | :--- |
| _.prj_ | Archivo con parámetros de orientación externa, calibración de cámaras y de proyectos. | Un archivo por proyecto. |

Inpho implementa varios tipos de cámaras. _Digi3D.NET_ implementa las siguientes:

* Cámaras sin distorsiones.
* Cámaras con distorsiones radiales.
* Cámaras con distorsiones en forma de polinomio.
* Cámaras con distorsiones mediante un _grid_ \(cuadrícula\) de distorsiones.

Permite cargar _proyectos_ a partir de las siguientes extensiones de archivos:

| Extensión | Descripción |
| :--- | :--- |
| _.prj_ | Archivo con parámetros de orientación externa, calibración de cámaras y de proyectos. |

