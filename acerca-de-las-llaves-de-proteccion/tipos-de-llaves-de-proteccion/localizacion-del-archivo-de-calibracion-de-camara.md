# Localización del archivo de calibración de cámara

El sensor cónico no sabe cargar calibraciones de cámaras, delega esta acción a cada una de las [Extensiones del Sensor Conico](extensiones-del-sensor-conico.md) cargadas, de modo que si una de ellas proporciona una calibración de cámara para una de las imágenes, se asigna a dicha imagen la calibración de cámara proporcionada.

Si no se localiza ninguna extensión que devuelva una calibración de cámara para alguna de las imágenes, se mostrará un cuadro de diálogo indicando que no se ha localizado un archivo de calibración para dicha cámara, e invitando al usuario a localizar un archivo de calibración de cámara válido. Si no se proporciona ninguno, se cancelará la carga del modelo, pues no se puede cargar un modelo sin un archivo de calibración de cámara válido.

