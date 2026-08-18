# glpi-conocimientos
1. Gestión de Grupos de Trabajo
Los grupos permiten organizar al personal por áreas funcionales o técnicas (ej. Soporte Nivel 1, Redes y Conectividad, Docentes Departamento Sistemas) para facilitar la asignación colectiva de tickets y activos.

Paso a paso para crear un grupo:

Iniciar sesión como Admin o Super-Admin.

Ir a Administración > Grupos (Administration > Groups).

Hacer clic en el botón + (Agregar) en la barra superior.

Completar los campos requeridos:

Nombre: Denominación clara del grupo (ej. Soporte Técnico - Centro de Comunicaciones).

Es visible en tickets / Puede ser asignado: Seleccionar Sí si el grupo recibirá derivaciones de tickets de soporte.

Puede ser solicitante: Seleccionar Sí si se van a abrir tickets a nombre de todo el equipo.

Puede contener: Habilitar si contendrá Elementos (inventario) o Usuarios.

Hacer clic en Guardar.

En la pestaña lateral Usuarios, asociar a los integrantes del grupo.

2. Creación Manual de Usuarios
Navegar a Administración > Usuarios (Administration > Users).

Hacer clic en el botón + (Agregar).

Completar los datos principales de la ficha:

Nombre de inicio de sesión (Login): Identificador del usuario (ej. formato estándar institucional: nombre.apellido).

Contraseña / Confirmar contraseña: Clave temporal que se entregará al usuario.

Nombre y Apellido: Datos personales completos.

Correo electrónico: Dirección de correo institucional donde se enviarán las notificaciones de tickets.

Ubicación: Oficina, aula o laboratorio habitual donde se desempeña.

Activo: Mantener en Sí.

Hacer clic en Guardar.

3. Asignación de Perfil, Entidad y Grupo al Usuario
Una vez creado el usuario, es obligatorio definir su nivel de acceso para que pueda ingresar al sistema:

Dentro de la ficha del usuario recién creado, ir a la pestaña Autorizaciones (Authorizations) en el menú lateral izquierdo.

Hacer clic en Agregar una autorización:

Entidad: Seleccionar la entidad correspondiente (ej. Entidad Raíz o subentidad regional).

Perfil: Elegir el rol adecuado (Self-Service/Post-Only para usuarios finales; Technician para operadores de mesa de ayuda; Supervisor para jefes de área).

Recursivo: Indicar Sí si el usuario debe mantener los permisos en todas las subentidades dependientes.

Presionar Agregar.

Ir a la pestaña Grupos y vincular al usuario a los grupos de trabajo a los que pertenezca.

4. Modificación, Inactivación y Bajas de Cuentas
Restablecimiento de contraseñas: Desde la pestaña principal del usuario, escribir la nueva contraseña en los campos correspondientes y presionar Guardar.

Inactivación por baja o receso: Cuando un técnico, docente o pasante deja de prestar funciones, cambiar el estado del campo Activo a No.

Regla de integridad: Nunca eliminar definitivamente un usuario que haya participado en tickets o figure como responsable de equipamiento en el inventario. La desactivación de la cuenta bloquea el acceso al sistema mientras mantiene intacto el historial técnico.
