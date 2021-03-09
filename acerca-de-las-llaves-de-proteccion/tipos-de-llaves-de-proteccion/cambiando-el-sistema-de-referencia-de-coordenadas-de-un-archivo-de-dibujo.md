# Cambiando el Sistema de Referencia de Coordenadas de un archivo de dibujo

No se puede cambiar el _sistema de referencia de coordenadas_ de un archivo de dibujo.

Si quieres cambiar el sistema de _referencia de coordenadas_ de un archivo de dibujo la única opción es exportar el archivo y crear uno nuevo en el sistema de referencia de coordenadas que nos interese.

Si estás trabajando con un archivo que tiene la información de su _sistema de referencia de coordenadas_ en un archivo externo con extensión [.prj](cambiando-el-sistema-de-referencia-de-coordenadas-de-un-archivo-de-dibujo.md) y sustituimos ese archivo _.prj_ por otro, **no esteremos cambiando** el sistema de referencia de coordenadas del archivo, sino que estaremos **engañando** al programa que cargue el archivo de dibujo, en este caso Digi3D.NET. El sustituir el archivo _.prj_ no cambia internamente las coordenadas de las geometrías de un archivo de dibujo.

