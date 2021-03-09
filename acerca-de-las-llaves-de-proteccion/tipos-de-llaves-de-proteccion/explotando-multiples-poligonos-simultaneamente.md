# Explotando múltiples polígonos simultáneamente

La orden [EXPLOTAR\_COMPLEJO](6dea026c-9c1d-4daa-a059-c18aed017acb) explota tanto polígonos como entidades de tipo complejo.

Esta orden admite selección múltiple, así que puedes seleccionar múltiples entidades \(mediante órdenes que permitan seleccionar múltiples entidades, como por ejemplo [SELECCIONA\_VENTANA](selecciona_ventana.md)\) y enviárselas a la orden _EXPLOTAR\_COMPLEJO_ cuando ésta solicita que selecciones la entidad a explotar.

Otra manera es mediante la herramienta de búsqueda, localizando polígonos y enviando las entidades localizadas a la orden _EXPLOTAR\_COMPLEJO_.

Sigue las siguientes instrucciones para explotar todos los polígonos:

1. Selecciona la opción del menú **Editar/Buscar**. Aparecerá el panel **Buscar**.
2. Despliega el menú desplegable del panel Buscar y selecciona la opción **Todos los polígonos**.
3. Asegúrate de que abajo en el campo **Enviar los resultados a** está seleccionada la opción **Ventana "Resultados de la búsqueda 1"**.
4. Pulsa el botón **Buscar**.
5. Aparecerán todos los polígonos del archivo enumerados en el panel **Resultados de la búsqueda 1**.
6. Ejecuta la orden **EXPLOTAR\_COMPLEJO**. La orden solicitará que selecciones la entidad a explotar.
7. En el panel **Resultados de la búsqueda** 1 selecciona todas las entidades y pulsa el **botón derecho** del ratón. Aparecerá un menú contextual.
8. Selecciona la opción **Enviar la selección a la orden activa**. Como la orden activa es la orden _EXPLOTAR\_COMPLEJO_, se enviarán todos los polígonos a ésta y el resultado es que se explotarán todos ellos de una vez.

