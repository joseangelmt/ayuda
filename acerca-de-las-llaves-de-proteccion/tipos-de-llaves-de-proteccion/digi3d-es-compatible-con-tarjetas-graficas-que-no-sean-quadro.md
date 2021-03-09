# ¿Digi3D es compatible con tarjetas gráficas que no sean Quadro?

La respuesta depende de si vas a visualizar estereoscopía profesional o no:

En un principio _Digi3D.NET_ es compatible con cualquier tarjeta gráfica que soporte el lenguaje gráfico [OpenGL](digi3d-es-compatible-con-tarjetas-graficas-que-no-sean-quadro.md), por lo tanto puedes utilizar cualquier tarjeta que lo soporte, ni siquiera tiene por que ser _nVidia_, puede ser una _Intel_, una _ATI, ...,_ pero no todas estar tarjetas te permiten visualizar estereoscopía profesional.

* Si no vas a visualizar estereoscopía profesional \(no vas a utilizar la ventana fotogramétrica, o vas a utilizar únicamente sensores monoscópicos como el de _Ortofoto_ o el de _Web Map Service_ o _Web Map Tile Service_\) o si vas a utilizar estereoscopía no profesional \(anaglifo o monitores auto-estereoscópicos o monitores con gafa pasiva polarizada\) puedes utilizar cualquier tarjeta gráfica que soporte _OpenGL_.
* Si por el contrario vas a visualizar estereoscopía profesional \(tienes un monitor con gafas activas _nVidia 3D Vision_ ó un monitor _Planar 3D\),_ necesitarás una tarjeta gráfica _nVidia Quadro_ por el siguiente motivo:

  **Las únicas tarjetas gráficas que admiten estereoscopía profesional son las** _**nVidia Quadro**_ **o las** _**ATI Fire GL**_**.**

  Las tarjetas gráficas de otras marcas no admiten estereoscopía, y las tarjetas gráficas _nVidia_ de la gama _GeForce_ únicamente soportan estereoscopía para el lenguaje de gráficos [DirectX](digi3d-es-compatible-con-tarjetas-graficas-que-no-sean-quadro.md) _11.1_ o superior. Este lenguaje de gráficos es compatible únicamente con _Windows 8_ o superior y tradicionalmente ha sido siempre un lenguaje gráfijo para juegos, y no para aplicaciones profesionales.

  _Digi3D.NET_ utiliza _OpenGL_ como lenguaje gráfico, por lo tanto **no puedes utilizar una tarjeta gráfica** _**nVidia GeForce**_ **para visualizar estereoscopía con Digi3D.NET**.

  Como curiosidad: el nombre _Quadro_ viene de _Quad Buffer_ que hace clara alusión a cuatro bufferes que es lo necesario para visualizar estereoscopía \(uno frontal y trasero para el ojo izquierdo y otro frontal y trasero para el derecho\).

