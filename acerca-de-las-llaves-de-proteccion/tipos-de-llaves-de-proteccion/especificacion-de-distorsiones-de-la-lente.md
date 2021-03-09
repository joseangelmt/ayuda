# Especificación de distorsiones de la lente

Las distorsiones de la lente son aquellas que aparecen por una mala fabricación de la lente.

Estas distorsiones se presentan siempre como distorsiones radiales con respecto al _Punto de mejor simetría \(PPS\)_ especificado en el archivo de cámara, o si no se especifica éste, con respecto al _Punto Principal \(PP\)._ En este punto se considera que la lente no tiene ninguna distorsión, y según nos alejamos de este punto comienzan a presentarse distorsiones.

Podemos controlar el momento en el que se realizarán las correcciones de distorsión y el sentido en el que se van a realizar las correcciones mediante las siguientes variables:

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
      <td style="text-align:left">TipoCorreccion</td>
      <td style="text-align:left">
        <ul>
          <li><b>CamaraAFoto</b>
            <br />Si la correcci&#xF3;n se debe aplicar al transformar Coordenadas C&#xE1;mara
            a Coordenadas Foto.</li>
          <li><b>FotoAFiducial</b>
            <br />Si la correcci&#xF3;n se debe aplicar al transformar Coordenadas Foto
            te&#xF3;ricas a Coordenadas Foto.</li>
        </ul>
      </td>
      <td style="text-align:left">
        <p>Tal y como puede verse en el gr&#xE1;fico que aparece en <a href="calibracion-de-camara.md">Calibracion de c&#xE1;mara</a>,
          las distorsiones se pueden corregir en dos pasos distintos.
          <br />Con esta variable podemos controlar este comportamiento.</p>
        <p>Si no se especifica esta variable, se asumir&#xE1; que tiene asignado
          el valor <b>FotoAFiducial</b>.</p>
      </td>
    </tr>
    <tr>
      <td style="text-align:left">TipoValorDistorsion</td>
      <td style="text-align:left">
        <p>Uno de los siguientes valores en funci&#xF3;n de si los valores de distorsi&#xF3;n
          que aparecen en la tabla de distorsiones son errores o correcciones:</p>
        <ul>
          <li><b>0</b>: Si los valores que aparecen en la tabla de distorsiones con
            errores.</li>
          <li><b>1</b>: Si los valores que aparecen en la tabla de distorsiones con
            correcciones.</li>
        </ul>
      </td>
      <td style="text-align:left">Digi3D.NET necesita saber si los valores de distorsi&#xF3;n especificados
        son errores o correcciones. En funci&#xF3;n del valor indicado en esta
        variable el programa realizar&#xE1; las correcciones en un sentido o en
        otro.</td>
    </tr>
  </tbody>
</table>

Y a continuación debemos especficar las distorsiones de la cámara. En los certificados de calibración podemos encontrar dos formas de presentar las distorsiones radiales:

* Mediante una tabla de radio-valor.
* Mediante un polinomio.

Vea también

