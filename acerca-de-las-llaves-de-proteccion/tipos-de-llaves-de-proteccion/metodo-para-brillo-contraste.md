# Método para brillo/contraste

Esta opción indicará el método que va a utilizar Digi3D.NET para cambiar el brillo, contraste y gamma de los píxeles de la ventana fotogramétrica.

Disponemos de las siguientes opciones:

<table>
  <thead>
    <tr>
      <th style="text-align:left">Fragment Shaders</th>
      <th style="text-align:left">
        <p>Esta opci&#xF3;n es la m&#xE1;s r&#xE1;pida pues realiza la transformaci&#xF3;n
          por hardware.</p>
        <p>Si seleccionamos esta opci&#xF3;n e interactuamos con los controles del
          panel Propiedades de la imagen veremos el resultado inmediatamene.</p>
        <p>Esta opci&#xF3;n solo es compatible con tarjetas gr&#xE1;ficas que dispongan
          de m&#xE1;s de un n&#xFA;cleo. Si tu tarjeta gr&#xE1;fica es antigua (&#xFA;nicamente
          dispone de un procesador) y tienes activada esta opci&#xF3;n es posible
          que las im&#xE1;genes se muevan a saltos.</p>
      </th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td style="text-align:left">Software</td>
      <td style="text-align:left">
        <p>Esta opci&#xF3;n es m&#xE1;s lenta y consume m&#xE1;s memoria pues requiere
          que Digi3D calcule y modifique por software los valores de los p&#xED;xeles
          que se van a mostrar en pantalla en la ventana fotogram&#xE9;trica.</p>
        <p>Si seleccionamos esta opci&#xF3;n e interactuamos con los controles del
          panel Propiedades de la imagen, Digi3D no mostrar&#xE1; la imagen inmediatamente,
          sino que veremos un &#xE1;rea negra hasta que se haya terminado de calcular
          la imagen rectificada.</p>
        <p>Selecciona esta opci&#xF3;n &#xFA;nicamente si tu tarjeta gr&#xE1;fica
          es antigua y dispone &#xFA;nicamente de un procesador.</p>
      </td>
    </tr>
  </tbody>
</table>

Vea también

