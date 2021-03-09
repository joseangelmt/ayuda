# Localización del archivo de orientación absoluta

_Digi3D.NET_ puede cargar orientaciones absolutas de archivos con las siguientes extensiones:

* Archivos _.abs.xml_ \(que aparecieron con Digi3D.NET\).
* Archivos .abs2 \(que aparecieron con Digi3D 2007\).

Cuando se carga un modelo, _Digi3D.NET_ intenta localizar en el directorio de trabajo un archivo cuyo nombre coincide con el del modelo cualquiera de estos archivos. 

Si el modelo es monoscópico, se intentarán localizar los siguientes archivos:

* \[nombre\_de\_la\_imagen\].abs.xml
* \[nombre\_de\_la\_imagen\].abs2

Si el modelo es estereoscópico, se intentarán localizar los siguientes archivos:

* \[nombre\_de\_la\_imagen\_izquierda\]-\[nombre\_de\_la\_imagen\_derecha\].abs.xml
* \[nombre\_de\_la\_imagen\_izquierda\]-\[nombre\_de\_la\_imagen\_derecha\].abs2

Si el modelo disponde de tres imágenes \(como por ejemplo en el [Sensor ADS](sensor-ads.md)\), se intentarán localizar los siguientes archivos:

* \[nombre\_de\_la\_imagen\_back\]-\[nombre\_de\_la\_imagen\_nadir\]-\[nombre\_de\_la\_imagen\_forward\].abs.xml
* \[nombre\_de\_la\_imagen\_back\]-\[nombre\_de\_la\_imagen\_nadir\]-\[nombre\_de\_la\_imagen\_forward\].abs2

Si se localiza un archivo, se carga y se asigna al sensor y finaliza la carga de archivos de orientación absoluta, de modo que si se localiza el archivo .abs.xml asociado a un modelo, ya no se intenta localizar el archivo _.abs2_.

En caso de no localizar ningún archivo de orientación absoluta, se creará una orientación absoluta virtual que para unas determinadas _Coordenadas Terreno_ devuelva las mismas _Coordenadas Modelo_.

