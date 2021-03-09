# Especificación de distorsiones de desortogonalidad

Las distorsiones de desortogonalidad aparecen por una mala fabricación del sensor CCD de la cámara.

Pueden presentarse dos tipos de errores:

* Que las células sensoras del CCD no tengan el mismo tamaño en alto y en ancho.
* Que las células sensoras del CCD no estén perfectamente alineadas.

Estos parámetros se pueden corregir mediante dos valores B1 y B2. Si disponemos de esta información, debemos introducirla en el archivo de cámara para que Digi3D.NET la corrija.

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
      <td style="text-align:left">TipoDesortogonalidad</td>
      <td style="text-align:left">
        <ul>
          <li><b>No</b>.
            <br />Si no se desea aplicar desortogonalidad.</li>
          <li><b>Fraser</b>.
            <br />Si se desea aplicar desortogonalidad en el eje de la <em>X</em> mediante
            la f&#xF3;rmula:<em>&#x2206;x = B1*x + B2*y</em>
          </li>
        </ul>
      </td>
      <td style="text-align:left">Indica si aplicar o no este tipo de correcci&#xF3;n. En caso de querer
        corregirlo deberemos introducir <b>Faser.</b>
      </td>
    </tr>
    <tr>
      <td style="text-align:left">B1</td>
      <td style="text-align:left">Un n&#xFA;mero.</td>
      <td style="text-align:left">Valor B1 para las f&#xF3;rmulas especificadas en la variable TipoDesortogonalidad.</td>
    </tr>
    <tr>
      <td style="text-align:left">B2</td>
      <td style="text-align:left">Un n&#xFA;mero.</td>
      <td style="text-align:left">Valor B2 para las f&#xF3;rmulas especificadas en la variable TipoDesortogonalidad.</td>
    </tr>
  </tbody>
</table>

Vea también

