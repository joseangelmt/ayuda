# Archivo de cámara

El archivo de cámara es un archivo ASCII con la siguiente estructura:

```text
[Camara]
Variable1=Valor1
Variable2=Valor2
...
```

El archivo de cámara tiene dos grupos grupos de variables: obligatorios y opcinales.

## Obligatorios

Son parámetros que deben incorporar forzosamente todos los archivos de cámara para que se consideren válidos, y son los siguientes:

* Parámetros de focal y punto principal.
* De orientación interna. En este caso hay dos posibilidades: si la cámara es digital se requiere el tamaño del pixel, y si la cámara es analógica se requerirán las coordenadas de las marcas fiduciales.

## Opcionales

Son parámetros que podemos incorporar opcionalmente, y son los siguientes:

* Parámetros de distorsión

Vea también

