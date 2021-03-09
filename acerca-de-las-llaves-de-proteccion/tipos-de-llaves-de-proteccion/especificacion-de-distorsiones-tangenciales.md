# Especificación de distorsiones tangenciales

Las distorsiones tangenciales aparecen por una mala alineación entre la lente y el sensor. Aparece en cámaras de bajo coste por usar pegamentos económicos.

Si disponemos de esta información, debemos introducirla en el archivo de cámara para que Digi3D.NET la corrija.

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
      <td style="text-align:left">TipoDistorsionTangencial</td>
      <td style="text-align:left">
        <ul>
          <li><b>No</b>.
            <br />Si no se quiere aplicar distorsi&#xF3;n tangencial.</li>
          <li>
            <p><b>Brown</b>.
              <br />Si se quiere aplicar la siguiente f&#xF3;rmula:</p>
            <p><em>&#x2206;x = P1*(r2 + 2*x2)+2*P2*x*y<br />&#x2206;y = 2*P1*x*y + P2*<br />(r2 + 2*y2)</em>
            </p>
          </li>
          <li>
            <p><b>OpenCV</b>.
              <br />Si se quiere aplicar la siguiente f&#xF3;rmula:</p>
            <p><em>&#x2206;x = 2*P1*x*y + P2*(r2 + 2*x2)<br />&#x2206;y = 2*P2*x*y + P1*(r2 + 2*y2)</em>
            </p>
          </li>
        </ul>
      </td>
      <td style="text-align:left">Indica la f&#xF3;rmula a aplicar para corregir esta distorsi&#xF3;n.
        <br
        />Los programas modernos como Pix4D, PhotoScan, etc utilizan la f&#xF3;rmula
        OpenCV.
        <br />Los programas cl&#xE1;sicos utilizan la f&#xF3;rmula de Brown.</td>
    </tr>
    <tr>
      <td style="text-align:left">P1</td>
      <td style="text-align:left">Un n&#xFA;mero.</td>
      <td style="text-align:left">Valor P1 para las f&#xF3;rmulas especificadas en la variable TipoDistorsionTangencial.</td>
    </tr>
    <tr>
      <td style="text-align:left">P2</td>
      <td style="text-align:left">Un n&#xFA;mero.</td>
      <td style="text-align:left">Valor para las f&#xF3;rmulas especificadas en la variable TipoDistorsionTangencial.</td>
    </tr>
  </tbody>
</table>

Vea también

