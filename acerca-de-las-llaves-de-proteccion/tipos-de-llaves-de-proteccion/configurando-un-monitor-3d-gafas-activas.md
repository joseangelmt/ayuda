# Configurando un Monitor 3D Gafas Activas

El instalador de Digi3D.NET ha configurado el programa para esta configuración, pero es posible que tu ordenador no esté configurado correctamente para esta configuración.

Sigue los siguientes pasos para configurar tanto tu ordenador como Digi3D.NET para visualizar estereoscopía en un monitor _3D_.

Existen tres configuraciones de monitor _3D_ con _nVidia 3DVision_:

1. Gafas inalámbricas con monitor sin emisor incorporado. En este caso, asegúrate de que el emisor está conectado correctamente al puerto USB correspondiente. Si tu tarjeta gráfica dispone de conector estereoscópico y dispones del cable de sincronismo, conecta tambien el emisor a la tarjeta gráfica.
2. Gafas inalámbricas con monitor con emisor incorporado.
3. Gafas con cable. En este caso asegúrate de que el emisor está conectado correctamente al puerto _USB_.

Configuración del controlador de la tarjeta gráfica:

1. Pulsa con el botón derecho del ratón en el escritorio. Aparecerá un menú contextual.
2. Selecciona la opción **Panel de control de NVIDIA**.
3. Localiza y selecciona la sección **3D estereoscópica/Establecer la configuración 3D estereoscópica**.
4. **Desactiva** la opción **Activar 3D estereoscópica**
5. Localiza y selecciona la sección **Configuración 3D/Controlar la configuración 3D**.
6. Aparecerá la página **Controlar la configuración 3D**.
7. Selecciona la pestaña **Configuración global**.
8. En el desplegable **Valores globales preestablecidos** selecciona la opción **Perfil base**.
9. Activa la opción **Estéreo - Habilitar**
10. Cambia el valor de la opción **Estéreo - Modo de pantalla** a la opción correspondiente según la siguiente tabla:

    | Tipo de monitor | Tipo de tarjeta gráfica | Disponibilidad de cable sincronismo | Opción a configurar |
    | :--- | :--- | :--- | :--- |
    | Monitor _3D_ sin emisor incorporado | Tarjeta gráfica profesional con conector estereoscópico | Si | Conector DIN interno \(con emisor 3D Vision de NVIDIA\) |
    | Monitor _3D_ sin emisor incorporado | Tarjeta gráfica profesional con conector estereoscópico | No | Estereo activo genérico \(con 3D Vision de NVIDIA\) |
    | Monitor _3D_ sin emisor incorporado | Tarjeta gráfica de gama de entrada | N/A | Estereo activo genérico \(con 3D Vision de NVIDIA\) |
    | Monitor _3D_ con emisor incorporado | N/A | N/A | Estereo activo genérico \(con 3D Vision de NVIDIA\) |

11. Si has tenido que cambiar alguna opción en los pasos anteriores, pulsa el botón **Aplicar**.
12. Localiza y selecciona la sección **Pantalla/Cambiar la resolución**.
13. Aparecerá la pantalla **Cambiar la resolución**.
14. Selecciona tu monitor _3D_ de entre la lista de monitores disponibles.
15. Asegúrate de que la **Frecuencia de actualización** del monitor _3D_ es _120Hz_.
16. Si has tenido que cambiar la _frecuencia de actualización_ en el paso anterior, pulsa el botón **Aplicar**.
17. Cierra el **Panel de control de NVIDIA**.

Configuración de Digi3D.NET para utilizar la configuración estereoscópica de la tarjeta gráfica:

1. Ejecuta **Digi3D.NET**.
2. Aparecerá el cuadro de diálogo **Nuevo proyecto**.
3. Pulsa el botón **Cancelar** para cerrar el cuadro de diálogo **Nuevo proyecto**.
4. Selecciona la opción del menú **Herramientas/Configuración**.
5. Despliega la sección **Ventana fotogramétrica**.
6. Selecciona la opción **Controlado por el driver** en campo **Estereoscopía**.
7. Pulsa el botón **Aceptar** del cuadro de diálogo **Configuración**.

## Vídeo

