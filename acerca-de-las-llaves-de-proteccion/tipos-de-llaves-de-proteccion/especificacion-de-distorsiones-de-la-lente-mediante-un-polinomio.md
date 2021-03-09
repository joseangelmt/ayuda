# Especificación de distorsiones de la lente mediante un polinomio

Si en el certificado de calibración de la cámara se especifican las distorsiones de la lente mediante un polinomio, deberemos introducir en el archivo de cámara las siguientes variables:

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
      <td style="text-align:left">Escala</td>
      <td style="text-align:left">Un valor indicando el factor de escala.</td>
      <td style="text-align:left">Factor de escalado general. Si no se dispone de este valor, introducir
        aqu&#xED; el valor <em>1.0</em>.</td>
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
      <td style="text-align:left">Digi3D.NET necesita saber si los valores de la tabla de distorsiones son
        errores o correcciones. En funci&#xF3;n del valor indicado en esta variable
        el programa realizar&#xE1; las correcciones en un sentido o en otro. En
        la pr&#xE1;ctica lo que hace el programa es cambiar el signo de la correcci&#xF3;n
        calculada en una determinada coordenada.</td>
    </tr>
    <tr>
      <td style="text-align:left">Pol</td>
      <td style="text-align:left">
        <p>Uno de los siguientes valores:</p>
        <ul>
          <li><b>K1_R2_K2_R4<br /></b>Si el polinomio es de la forma:
            <br />K0 + K1*R2 + K2*R4 + K3*R6.</li>
          <li><b>K1_R3_K2_R5<br /></b>Si el polinomio es de la forma:
            <br />K0 + K1*R3 + K2*R5 + K3*R7.</li>
        </ul>
      </td>
      <td style="text-align:left">F&#xF3;rmula a utilizar. Este valor suele venir en el certificado de calibraci&#xF3;n
        de la c&#xE1;mara.
        <br />La mayor&#xED;a de programas utilizan <b>K1_R2_K2_R4.</b>
      </td>
    </tr>
    <tr>
      <td style="text-align:left">K0</td>
      <td style="text-align:left">Un n&#xFA;mero.</td>
      <td style="text-align:left">Valor de <em>distorsi&#xF3;n radial</em> tal y como aparece en el certificado
        de calibraci&#xF3;n. Si no aparece este valor, introducir aqu&#xED; un <em>1.0</em>
      </td>
    </tr>
    <tr>
      <td style="text-align:left">K1</td>
      <td style="text-align:left">Un n&#xFA;mero.</td>
      <td style="text-align:left">Valor de <em>distorsi&#xF3;n radial</em> tal y como aparece en el certificado
        de calibraci&#xF3;n. Si no aparece este valor, introducir aqu&#xED; un <em>0.0</em>
      </td>
    </tr>
    <tr>
      <td style="text-align:left">K2</td>
      <td style="text-align:left">Un n&#xFA;mero.</td>
      <td style="text-align:left">Valor de <em>distorsi&#xF3;n radial</em> tal y como aparece en el certificado
        de calibraci&#xF3;n. Si no aparece este valor, introducir aqu&#xED; un <em>0.0</em>
      </td>
    </tr>
    <tr>
      <td style="text-align:left">K3</td>
      <td style="text-align:left">Un n&#xFA;mero.</td>
      <td style="text-align:left">Valor de <em>distorsi&#xF3;n radial</em> tal y como aparece en el certificado
        de calibraci&#xF3;n. Si no aparece este valor, introducir aqu&#xED; un <em>0.0</em>
      </td>
    </tr>
  </tbody>
</table>

A continuación un ejemplo de un archivo de calibración de cámara digital con distorsiones de cámara para el siguiente archivo de calibración: [RCD105\_Cal\_Cert\_064\_060\_064\_RGB\_20100721.pdf](RCD105_Cal_Cert_064_060_064_RGB_20100721.pdf)

```text
[Camara]
Focal=59.761
TamanoPixel=0.0068
PP=0.0 0.0 
PPS=-0.3047 0.032
Escala=1.0
TipoValorDistorsion=1
Pol=K1_R2_K2_R4
k0=8.97882e-3
k1=-2.07064e-5
k2=4.45263e-9
k3=0.0
```

Descarga un modelo de ejemplo con esta cámara: [Modelo con certificado de calibración con distorsiones estandar.rar](http://digi21.blob.core.windows.net/ejemplos/Modelo%20con%20certificado%20de%20calibraci%C3%B3n%20con%20distorsiones%20estandar.rar)

