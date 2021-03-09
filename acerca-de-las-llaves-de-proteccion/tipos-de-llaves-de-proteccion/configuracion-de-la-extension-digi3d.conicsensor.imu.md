# Configuración de la extensión Digi3D.ConicSensor.Imu

Los archivos de _Centros de Proyección y Giros_ no indican las unidades en las que están indicados los giros de las imágenes, de modo que tendremos que indicar de alguna manera a la extensión Digi3D.ConicSensor.Imu las unidades de estos giros ni tampoco el orden en el que hay que multiplicar los giros para obtener la matriz de giros a asociar a cada imagen.

Podemos configurar este parámetro mediante el [Cuadro de dialogo Configuración](cuadro-de-dialogo-configuracion.md), en la sección Importador de **Centros de Proyección y Giros \(.eo, .imu\)** mediante los siguientes parámetros:

<table>
  <thead>
    <tr>
      <th style="text-align:left">Nombre de la variable</th>
      <th style="text-align:left">Descripci&#xF3;n</th>
      <th style="text-align:left">Posibles valores</th>
      <th style="text-align:left">Valor por defecto</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td style="text-align:left">Unidades de los giros</td>
      <td style="text-align:left">Indica las unidades en las que aparecen los giros en el archivo <em>.eo</em> o <em>.imu</em> cargado.</td>
      <td
      style="text-align:left">
        <ul>
          <li>Radianes</li>
          <li>Sexagesimal</li>
          <li>Centesimal</li>
        </ul>
        </td>
        <td style="text-align:left">Sexagesimal</td>
    </tr>
    <tr>
      <td style="text-align:left">Orden de los giros</td>
      <td style="text-align:left">Indica el orden en el que hay que multiplicar los giros para crear la
        matriz de giros a asignar a la imagen.</td>
      <td style="text-align:left">
        <ul>
          <li>Omega-Phi-Kappa</li>
          <li>Phi-Omega-Kappa</li>
          <li>Omega-Kappa-Phi</li>
          <li>Kappa-Omega-Phi</li>
          <li>Kappa-Phi-Omega</li>
          <li>Phi-Kappa-Omega</li>
        </ul>
      </td>
      <td style="text-align:left">Omega-Phi-Kappa</td>
    </tr>
  </tbody>
</table>

