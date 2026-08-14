# glpi-conocimientos
Guía: Manual de Procedimiento: Creación y Gestión de Perfiles
Este documento describe la metodología para definir, configurar y asignar perfiles de acceso en la plataforma GLPI, garantizando el principio de menor privilegio y la seguridad del inventario y la mesa de ayuda.

1. Conceptos Clave de Seguridad
Separación de funciones: Los permisos administrativos no deben otorgarse a cuentas genéricas ni a usuarios finales.

Uso del perfil Super-Admin: Reservado exclusivamente para tareas estructurales (actualizaciones, backups, reglas globales, plugins). No utilizar para la gestión diaria de tickets.

Herencia de entidades: Definir si un perfil tiene alcance únicamente sobre una subentidad o sobre toda la estructura jerárquica de la facultad.

2. Paso a Paso: Crear un Nuevo Perfil
Iniciar sesión con una cuenta con perfil Super-Admin.

Acceder al menú: Administración > Perfiles (Administration > Profiles).

Hacer clic en el botón + (Agregar) en la barra superior.

Completar los campos iniciales:

Nombre: Denominación clara del rol (ej. Técnico Redes - Nivel 1, Operador de Laboratorio, Auditor Externo).

Perfil predeterminado: Indicar si será el perfil asignado automáticamente a los nuevos usuarios.

Interfaz: Seleccionar entre Interfaz simplificada (usuarios finales/Post-Only) o Interfaz estándar (técnicos y administradores).

Hacer clic en Guardar.

3. Configuración Fina de Permisos (Pestañas)
Una vez creado el perfil, se deben ajustar las matrices de permisos ingresando a sus pestañas laterales:

Asistencia / Helpdesk:

Definir si el rol puede crear, actualizar, asignar, solucionar o eliminar tickets.

Habilitar o restringir la visualización de tickets de otros grupos o entidades.

Configurar permisos para añadir tareas y tiempos de intervención.

Inventario / Activos:

Configurar permisos de Lectura, Modificación o Eliminación para cada tipo de activo (Computadoras, Dispositivos de red, Impresoras, Software).

Recomendación: Bloquear el permiso de eliminación definitiva de activos a perfiles que no sean Administrador general.

Herramientas / Base de Conocimientos:

Habilitar acceso de lectura o escritura sobre manuales internos y públicos.

Administración:

Definir si el perfil puede gestionar usuarios, grupos, reglas de negocio o diccionarios del sistema.

4. Asignación de Perfiles a Usuarios
Ir a Administración > Usuarios (Administration > Users).

Seleccionar el usuario correspondiente de la lista.

En el menú lateral izquierdo, hacer clic en Autorizaciones (Authorizations).

Hacer clic en Agregar una autorización:

Seleccionar la Entidad correspondiente (ej. Entidad Raíz o una sede/área específica).

Asignar el Perfil adecuado.

Indicar si aplica de forma Recursiva (para subentidades).

Presionar Agregar.bicación exacta (ej. Aula 2 / Laboratorio de Sistemas).
