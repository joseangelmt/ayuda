# TEXTO

Inserta un texto en el archivo de dibujo.

## Parámetros

| Número de parámetro | Descripción | Valores | Opcional |
| :--- | :--- | :--- | :--- |
| 1 | Código texto \([COD](cod.md)\) | Identificador del código | Si |
| 2 | Ángulo activo \([AA](autonum.md)\) | Número real | Si |
| 3 | Altura de texto \([AT](autonum.md)\) | Número real | Si |
| 4 | Justificación de texto \([JT](autonum.md)\) | Número real | Si |

Si no se introducen parámetros, la orden solicita el texto a insertar en la barra de mensajes. Una vez digitalizado el texto, ésta vuelve a solicitar otro texto a insertar y así sucesivamente hasta cancelar la orden mediante la tecla _Esc_.

Si se introduce un parámetro, la orden inserta el texto repetivamente sin solicitar el texto a insertar hasta que se cancele la orden mediante la tecla _Esc_.

### Ejemplo:

texto=Tc

## Observaciones

Si se introduce como parámetro un número y está activa la variable [AUTONUM](autonum.md), el texto insertado variará en funcion del valor indicado en la variable _AUTONUM_. Por ejemplo, si queremos insertar textos pares \(2, 4, 6, ...\) ejecutaríamos la siguiente sucesion de ordenes:

autonum=2  
texto=2

Si queremos insertar texto impares\(1, 3, 5, ...\) ejecutaríamos la siguiente suceción de órdenes:

autonum=2  
texto=1

Podemos modificar el formato de los parametros de auto-numeracion mediante la variable [FORMATO\_AUTONUM](formato_autonum.md).

Por ejemplo, si queremos introducir sucesivamente textos con el valor _Parcela 1, Parcela 2, Parcela 3,..._ ejecutaríamos la siguiente sucesion de órdenes:

formato\_autonum=Parcela %d  
autonum=1  
texto

Podemos insertar un simbolo \(cuya definicion se extraerá del archivo de dibujo correspondiente en el directorio de símbolos\) si indicamos que texto a insertar es @\[número de simbolo\], siempre y cuando el codigo activo no utilice como fuente una fuente TrueType.

Por ejemplo, si queremos instroducir el símbolo 169 de nuestro directorio de símbolos, ejecutaremos la siguiente orden:

texto=@169

## Características de la orden

| Tipo de orden | [Orden interactiva](texto.md) |
| :--- | :--- |
| Repite automáticamente | Si |
| Opción del menú donde aparece la orden | Dibujar/Texto con ángulo activo |
| Barra de herramientas en la que aparece la orden | Textos |
| Extensión | DigiNG.OrdenesRaster.dll |
| Variables relacionadas | [AA](aa.md), [AT](at.md), [AUTONUM](autonum.md), [FORMATO\_AUTONUM](formato_autonum.md), [JT](jt.md), [REPITE](repite.md) |

## Vídeo

Vea también

