# GEN

Filtra o elimina puntos de una entidad seleccionada por el usuario.

## Parámetros

| Número de parámetro | Descripción | Valores | Opcional |
| :--- | :--- | :--- | :--- |
| 1 | [TOL](tol.md) | Número real | Si |
| 2 | [TOL\_ANG](tol_ang.md) | Número real | Si |

## Observaciones

El modo de actuar depende del factor de generalización que se encuentre activo en el momento de ejecutar esta orden. Este factor está condicionado por las variables de tolerancia, cuyo valores se asignan mediante las órdenes [TOL](tol.md) y [TOL\_ANG](tol_ang.md).

Si tecleamos GEN=&lt;código&gt;, se generalizarán todas las entidades con ese código que exsistan en el fichero de dibujo.

## Características de la orden

| Tipo de orden | [Orden interactiva](gen.md) |
| :--- | :--- |
| Repite automáticamente | Si |
| Opción del menú donde aparece la orden | Editar/Polilíneas/Generalizar |
| Barra de herramientas en la que aparece la orden | Editar polilínea |
| Extensión | DigiNG.OrdenesStandard.dll |
| Variables relacionadas | [REPITE](repite.md), [TOL](tol.md), [TOL\_ANG](tol_ang.md) |

## Vídeo

Vea también

