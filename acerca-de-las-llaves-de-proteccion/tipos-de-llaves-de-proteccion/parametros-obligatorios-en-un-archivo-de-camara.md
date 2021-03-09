# Parámetros obligatorios en un archivo de cámara

Todos los archivos de cámara deben informar obligatoriamente de los parámetros de la focal, punto principal y de orientación interna. A continuación mostramos los parámetros de focal y punto principal, y después los parámetros de interna para cámaras digitales y de interna para cámaras analógicas.

Si no se localizan en el archivo de cámara los parámetros de focal, punto principal y uno de los dos tipos de orientación interna \(digital o analógica\) se cancelará la carga del archivo de cámara porque se considerará incompleto.

## Parámetros de focal y punto principal

<table>
  <thead>
    <tr>
      <th style="text-align:left">Variable</th>
      <th style="text-align:left">Valor</th>
      <th style="text-align:left">Descripci&#xF3;n</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td style="text-align:left">Focal</td>
      <td style="text-align:left">Uno o dos valores.</td>
      <td style="text-align:left">
        <p>Focal calibrada de la c&#xE1;mara. Las unidades de este valor definen
          las unidades del resto de valores en el archivo de c&#xE1;mara, lo que
          quiere indicar que si ponemos este valor en mil&#xED;metros, las unidades
          del resto de variables deber&#xE1;n estar en mil&#xED;metros. De puede
          introducir aqu&#xED; un valor en cualquier unidad, con la condici&#xF3;n
          de que el resto de variables utilicen la misma unidad.</p>
        <p>Si la c&#xE1;mara es de bajo coste es posible que se disponga de dos focales,
          una para la componente X y otra para la componente Y. Si &#xFA;nicamente
          se dispone de una focal, introducimos un &#xFA;nico valor que se compartir&#xE1;
          para la componente X y la componente Y</p>
      </td>
    </tr>
    <tr>
      <td style="text-align:left">PP</td>
      <td style="text-align:left">Dos valores, uno para la coordenada <em>X</em> otro para la coordenada <em>Y</em>
      </td>
      <td style="text-align:left">Indica las coordenadas del punto principal de la c&#xE1;mara. Estas coordenadas
        indican la posici&#xF3;n el origen del sistema de fotocoordenadas de la
        c&#xE1;mara. Estas coordenadas indican el punto a partir del cual se corrigen
        las distorsiones de la c&#xE1;mara.
        <br /><b>Advertencia:</b> Si en el certificado de calibraci&#xF3;n se indica
        que las coordenadas de las marcas fiduciales est&#xE1;n referidas al <em>Punto Principal</em> o
        al <em>Punto de mejor simetr&#xED;a</em> o al <em>PPS</em>, <b>se deber&#xE1; introducir aqu&#xED; el valor 0.0 0.0</b> y
        obviar el valor que aparece en el certificado de calibraci&#xF3;n para
        el <em>punto principal</em>.</td>
    </tr>
    <tr>
      <td style="text-align:left">PPS</td>
      <td style="text-align:left">Dos valores, uno para la coordenada <em>X</em> otro para la coordenada <em>Y</em>
      </td>
      <td style="text-align:left">Este <b>valor</b> es <b>opcional</b>. Si no se introduce se asume que coincide
        con el valor <em>PP</em>.
        <br />Indica las coordenadas del <em>Punto de Mejor Simetr&#xED;a</em> que es
        un punto de la c&#xE1;mara en el cual las distorsiones de la lente son
        sim&#xE9;tricas.</td>
    </tr>
  </tbody>
</table>

## Parámetros de interna

Los parámetros de interna permiten transformar _Coordenadas Foto_ a _Coordenadas Pixel_. Existen dos grupos de parámetros en función de si la cámara es digital o analógica.

**Para cámaras digitales**:

| Variable | Valor | Descripción |
| :--- | :--- | :--- |
| TamanoPixel | Un valor si el tamaño del pixel es idéntico en vertical y en horizontal. Dos valores \(horizontal y luego vertical\) si el tamaño del pixel no es idéntico en horizontal y en vertical. | Indica el tamaño del pixel en el sensor CCD de la cámara. Habitualmente el tamaño del pixel coincide en horizontal y en vertical, pero es posible que no coincidan, en cuyo caso tendremos que introducir los dos valores aquí. Las unidades deben coincidir con las de la focal. |

A continuación un ejemplo de un archivo de calibración de cámara digital:

```text
[Camara]
Focal=154.052
PuntoPrincipal=0.015 -0.004
TamanoPixel=0.003
```

**Para cámaras analógicas**:

| Variable | Valor | Descripción |
| :--- | :--- | :--- |
| Fiducial1 | Dos valores, uno para la coordenada _X_ otro para la coordenada _Y_ | Coordenadas de la primera marca fiducial tal y como aparecen en el certificado de calibración de la cámara. |
| Fiducial2 | Dos valores, uno para la coordenada _X_ otro para la coordenada _Y_ | Coordenadas de la segunda marca fiducial tal y como aparecen en el certificado de calibración de la cámara. |
| Fiducial3 | Dos valores, uno para la coordenada _X_ otro para la coordenada _Y_ | Coordenadas de la tercera marca fiducial tal y como aparecen en el certificado de calibración de la cámara. |
| Fiducial4 | Dos valores, uno para la coordenada _X_ otro para la coordenada _Y_ | Coordenadas de la cuarta marca fiducial tal y como aparecen en el certificado de calibración de la cámara. |
| Fiducialn | Dos valores, uno para la coordenada _X_ otro para la coordenada _Y_ | Coordenadas de la n-ésima marca fiducial tal y como aparecen en el certificado de calibración de la cámara. |

A continuación un ejemplo de un archivo de calibración de cámara analógica:

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
```

Vea también

