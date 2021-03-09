# Especificación de distorsiones de la lente mediante una tabla radio-valor

Si en el certificado de calibración las distorsiones de la cámara vienen especificadas como una tabla radio-valor, tendremos que introducir las siguientes variables en el archivo de cámara:

| Variable | Valor | Descripción |
| :--- | :--- | :--- |
| Distorsion1 | Dos valores: _radio_ y _distorsión_ | Los valores de las _radio/distorsión_ se deben introducir **en las mismas unidades** que el resto de parámetros en el archivo de cámara. **Nótese que en la mayoría de los certificados de calibración de cámaras, los radios se dan en milímetros y los valores de distorsión en micras.** |
| Distorsion2 | Dos valores: _radio_ y _distorsión_ | Los valores de las _radio/distorsión_ se deben introducir **en las mismas unidades** que el resto de parámetros en el archivo de cámara. **Nótese que en la mayoría de los certificados de calibración de cámaras, los radios se dan en milímetros y los valores de distorsión en micras.** |
| Distorsionn | Dos valores: _radio_ y _distorsión_ | Los valores de las _radio/distorsión_ se deben introducir **en las mismas unidades** que el resto de parámetros en el archivo de cámara. **Nótese que en la mayoría de los certificados de calibración de cámaras, los radios se dan en milímetros y los valores de distorsión en micras.** |

A continuación un ejemplo de un archivo de calibración de cámara analógica con distorsiones radiales:

```text
[Camara]
Focal=154.052
PuntoPrincipal=0.015 -0.004
Fiducial1=113.009 -0.004
Fiducial2=-112.987 -0.004
Fiducial3=0.015 113.002
Fiducial4=0.015 -113.016
Fiducial5=113.005 112.994
Fiducial6=-112.991 -113.015
Fiducial7=-112.989 112.991
Fiducial8=113.016 -113.013
TipoValorDistorsion=0
Distorsion1=0 0.000
Distorsion2=10 0.000
Distorsion3=20 0.000
Distorsion4=30 -0.001
Distorsion5=40 -0.001
Distorsion6=50 0.000
Distorsion7=60 0.001
Distorsion8=70 0.002
Distorsion9=80 0.001
Distorsion10=90 -0.001
Distorsion11=100 0.000
Distorsion12=110 -0.001
Distorsion13=120 -0.002
Distorsion14=130 -0.001
Distorsion15=140 0.000
Distorsion16=150 0.001
```

Vea también

