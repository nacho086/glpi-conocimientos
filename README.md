# glpi-conocimientos
GLPI divide sus accesos según el tipo de interfaz:

Interfaz Simplificada (Self-Service): Diseñada para la interacción directa del usuario final sin acceso a la administración ni al inventario global.

Interfaz Estándar: Diseñada para el personal operativo, técnico, supervisores y administradores del sistema.

1. Self-Service / Post-Only (Peticionario / Usuario Final)
Interfaz: Simplificada.

Destinatarios: Alumnos, docentes, personal administrativo y no docentes.

Funciones principales:

Crear tickets de incidencias (fallas) o requerimientos de servicio.

Consultar el estado y evolución de sus propias solicitudes.

Leer artículos públicos y manuales en la Base de Conocimiento (FAQ).

Validar, aprobar o rechazar soluciones propuestas por los técnicos.

Solicitar reserva de recursos (proyectores, salas, notebooks) si está habilitado.

Restricciones: No tiene visibilidad sobre el inventario general ni sobre los tickets de otros usuarios.

2. Hotliner (Mesa de Entradas / Operador de Primera Línea)
Interfaz: Estándar.

Destinatarios: Personal de recepción, telefonistas o soporte de nivel 1.

Funciones principales:

Recepción y registro formal de solicitudes recibidas por canales externos (teléfono, presencial o correo).

Clasificación inicial de incidentes: definición de categoría, urgencia e impacto.

Derivación y asignación de tickets a los grupos técnicos pertinentes.

Restricciones: Generalmente no ejecuta la resolución técnica ni modifica configuraciones avanzadas del parque informático.

3. Technician (Técnico de Soporte)
Interfaz: Estándar.

Destinatarios: Equipo técnico de soporte en sitio, administradores de red de campo y pasantes de TI.

Funciones principales:

Gestión, diagnóstico y resolución de tickets asignados de forma individual o a su grupo.

Registro de tareas realizadas, consumos de tiempo e insumos utilizados.

Consulta, vinculación y actualización de activos en el módulo de Inventario (PCs, switches, impresoras, servidores).

Publicación de soluciones y conversión de resoluciones en artículos de la Base de Conocimiento.

Restricciones: No puede modificar configuraciones globales del servidor, esquemas de permisos ni eliminar registros maestros de inventario.

4. Normal
Interfaz: Estándar.

Destinatarios: Personal en etapa de inducción, directores de área o auditores operativos.

Funciones principales:

Navegación completa por el menú estándar de GLPI.

Visualización del inventario de activos en modo solo lectura.

Creación y seguimiento de tickets.

Restricciones: No tiene permisos para asignar o dar por resueltos tickets técnicos ni alterar fichas de hardware/redes.

5. Supervisor (Jefe de Área / Coordinador de Soporte)
Interfaz: Estándar.

Destinatarios: Jefes del Centro de Comunicaciones, coordinadores de infraestructura y líderes de soporte.

Funciones principales:

Supervisión y reasignación de la carga de trabajo entre los técnicos del área.

Aprobación formal de solicitudes sujetas a validación (compras, cambios de infraestructura).

Gestión de acuerdos de nivel de servicio (SLAs), escalamiento de incidentes críticos y prioridades.

Visualización de estadísticas de rendimiento, métricas de tiempos de resolución y satisfacción de usuarios.

6. Admin (Administrador Funcional)
Interfaz: Estándar.

Destinatarios: Administradores generales de la plataforma y encargados de gestión de TI.

Funciones principales:

Alta, baja y modificación de usuarios, grupos y entidades.

Configuración de componentes generales, categorías de tickets, ubicaciones y modelos de hardware.

Gestión total sobre los elementos del inventario físico y lógico.

Restricciones: No interviene sobre configuraciones críticas del núcleo del sistema ni conexiones de bajo nivel reservadas al Super-Admin.

7. Super-Admin (Administrador del Sistema / Servidor)
Interfaz: Estándar.

Destinatarios: Responsables directos del servidor GLPI y administradores de infraestructura base.

Funciones principales:

Control total e irrestricto sobre la plataforma y la base de datos.

Instalación y parametrización de plugins (como agentes de inventario nativo).

Definición de reglas automáticas de negocio, diccionarios de importación y conectores externos (LDAP, servidores de correo SMTP/IMAP).

Configuración de seguridad, logs de auditoría y mantenimiento general.

8. Observer (Observador / Auditor)
Interfaz: Estándar.

Destinatarios: Auditores internos/externos, autoridades o personal de control de gestión.

Funciones principales:

Acceso de solo lectura a la totalidad del inventario, tickets y reportes estadísticos.

Extracción de datos para auditorías o balances de gestión técnica.

Restricciones: Bloqueo total para crear, editar, reasignar o eliminar cualquier elemento dentro de la plataforma.
Inactivación por baja o receso: Cuando un técnico, docente o pasante deja de prestar funciones, cambiar el estado del campo Activo a No.

Regla de integridad: Nunca eliminar definitivamente un usuario que haya participado en tickets o figure como responsable de equipamiento en el inventario. La desactivación de la cuenta bloquea el acceso al sistema mientras mantiene intacto el historial técnico.
