# Localización de orientaciones

El sensor cónico no sabe cargar orientaciones para las imágenes, delega esta acción a cada una de las [Extensiones del Sensor Conico](extensiones-del-sensor-conico.md) cargadas, de modo que si una de ellas proporciona orientaciones externas para una de las imágenes, se asigna a dicha imagen la orientación externa proporcionada.

Si no se localiza ninguna extensión que devuelva una orientación externa para alguna de las imágenes, se asigna una orientación externa unitaria, en la cual las Coordenadas Cámara devuelvas coinciden con las Coordenadas Modelo proporcionadas.

Vea también

