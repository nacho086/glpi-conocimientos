# glpi-conocimientos
Guía: Instalación del Agente GLPI para Inventario Automático (Windows)
Esta guía detalla el procedimiento que el personal técnico debe ejecutar en cada PC o notebook de la facultad para habilitar el reporte e inventario automático en el servidor GLPI.

1. Descarga del Agente GLPI
Abrir el navegador en la computadora a inventariar y acceder al repositorio de descargas de GLPI Agent en GitHub:

[https://github.com/glpi-project/glpi-agent/releases](https://github.com/glpi-project/glpi-agent/releases)

Descargar el archivo instalador oficial para Windows según la arquitectura (por lo general, la versión de 64 bits: glpi-agent-1.x-x64.msi).

2. Instalación Paso a Paso
Ejecutar el archivo .msi descargado con permisos de administrador.

Avanzar en el asistente haciendo clic en Next e indicar el tipo de instalación Typical.

En la pantalla de Server Configuration Target:

En la opción Service URL, ingresar la URL completa del servidor GLPI apuntando al punto de inventario:

[http://192.168.27.217/front/inventory.php](http://192.168.27.217/front/inventory.php)

(Nota: Si el servidor usa un subdirectorio o la carpeta /public, asegurar la ruta exacta al script de recepción).

(Opcional) En la ventana de configuración del agente, desmarcar la opción Quick Install si se requiere personalizar opciones avanzadas.

Avanzar con Next hasta llegar a las opciones de ejecución.

En la pantalla de tareas, asegurarse de marcar Run inventory after installation (Ejecutar inventario tras instalar).

Hacer clic en Install y aguardar a que el proceso finalice en pantalla.

Presionar Finish.

3. Forzar el Primer Inventario y Verificación
Abrir la barra de búsqueda de Windows y buscar GLPI Agent Monitor.

En el panel o menú emergente del agente, hacer clic en la opción Force Inventory.

El estado del agente cambiará a Running inventory mientras recolecta la información del equipo.

4. Confirmación dentro de GLPI (Panel Administrativo)
Ingresar al panel de administración de GLPI ([http://192.168.27.217/](http://192.168.27.217/)).

Ir a Activos > Computadoras.

Si el equipo no figura de inmediato, hacer clic en la opción de Recargar página.

La computadora aparecerá registrada automáticamente con la siguiente información relevada:

Hardware: Nombre del equipo, fabricante, modelo, número de serie, procesador y memoria RAM.

Red: Direcciones IP, direcciones MAC y placas de red detectadas (LAN/Wi-Fi).

Almacenamiento y Discos: Unidades de disco, capacidad y volúmenes.

Sistema Operativo: Versión, arquitectura y parches instalados.

Software: Lista completa de aplicaciones e insumos instalados.

Histórico: Detalle con fecha/hora de la importación realizada por el agente.

⚠️ Notas y Recomendaciones para Técnicos
Red local obligatoria: Para que el agente pueda enviar los datos al servidor en el primer escaneo, la PC debe estar conectada a la misma red física/Wi-Fi de la facultad.

Asignación manual posterior: Una vez que la computadora aparezca en el inventario de GLPI, ingresar a su ficha para asignarle el Estado (ej. En uso), el Técnico a cargo, el Usuario principal y la Ubicación exacta (ej. Aula 2 / Laboratorio de Sistemas).
