# Calibracion de cámara

Es una orientación que transforma _Coordenadas Cámara_ en _Coordenadas Pixel_.

Esta orientación funciona en dos pasos:

1. Corrección de distorsiones.
2. Transformación a Pixel mediante una [Orientación Interna](orientacion-interna.md).

Las distorsiones que puede corregir la calibración de la cámara son las siguientes:

* Distorsiones radiales \(presentes por una mala fabricacion de la lente\).
* Distorsiones tangenciales \(presentes por una mala alineación entre la lente y el sensor\).
* Distorsiones de desortogonalidad \(presentes por una mala fabricación del _sensor CCD_, en el que puede que los píxeles no tengan el mismo ancho que alto o que la matriz de píxeles no esté perfectamente alineada.

En el siguiente esquema se resumen los pasos seguidos por las cámaras para transformar _Coordenadas Cámara_ en _Coordenadas Pixel_.

Vea también

