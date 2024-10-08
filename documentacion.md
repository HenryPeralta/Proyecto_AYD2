# REQUERIMIENTOS FUNCIONALES.

| **Categoría**                  | **ID**  | **Requerimiento Funcional**                                                                                                                                                 |
|--------------------------------|---------|------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| 1. Registro de Usuarios        | RF-001  | Los usuarios deben tener la posibilidad de registrarse proporcionando datos como nombre completo, fecha de nacimiento, género, correo electrónico, foto del DPI, número de celular, contraseña y confirmación de contraseña. |
|                                | RF-002  | Los usuarios deben poder añadir métodos de pago opcionales, tales como tarjetas de crédito/débito o el pago en efectivo al finalizar el viaje.                             |
|                                | RF-003  | Se debe enviar un correo electrónico de confirmación a los usuarios para verificar su cuenta.                                                                              |
| 2. Registro de Conductores     | RF-004  | Los conductores deben registrarse proporcionando información detallada como nombre completo, número de teléfono, edad, número de DPI, correo electrónico, CV en PDF, fotografía, foto del vehículo, número de placa, marca y año del vehículo, género, estado civil, cuenta bancaria y dirección. |
|                                | RF-005  | Tras el registro, se debe generar un código de empleado y una contraseña temporal para cada conductor, enviándolos por correo electrónico. La contraseña debe ser cambiada en el primer inicio de sesión. |
|                                | RF-006  | El administrador y los asistentes deben tener la capacidad de visualizar los CV en PDF de los conductores registrados.                                                       |
| 3. Registro de Asistentes      | RF-007  | El administrador debe poder registrar asistentes proporcionando información como nombre completo, número de teléfono, edad, número de DPI, correo electrónico, CV en PDF, fotografía, género, estado civil, cuenta bancaria y dirección. |
|                                | RF-008  | Para cada asistente registrado, se debe crear un código de empleado y una contraseña temporal, los cuales serán enviados por correo electrónico. La contraseña debe ser cambiada al primer inicio de sesión. |
| 4. Inicio de Sesión y Seguridad| RF-009  | Los usuarios, conductores y asistentes deben poder iniciar sesión utilizando su correo electrónico y contraseña.                                                             |
|                                | RF-010  | La cuenta debe bloquearse tras cinco intentos fallidos de inicio de sesión, y se debe enviar una notificación por correo electrónico.                                     |
|                                | RF-011  | Se debe habilitar un proceso para recuperar contraseñas que envíe un enlace de restablecimiento al correo electrónico registrado.                                           |
|                                | RF-012  | Al iniciar sesión, el administrador debe cargar un archivo de texto plano con una segunda contraseña encriptada para verificar su identidad.                               |
| 5. Gestión de Información      | RF-013  | Los usuarios deben poder actualizar su información personal, como nombre, correo electrónico, número de celular y añadir métodos de pago adicionales.                    |
|                                | RF-014  | Los conductores deben poder actualizar sus datos y los del vehículo a través de un documento en PDF, que será revisado y aprobado por un asistente.                       |
| 6. Solicitud de Viajes         | RF-015  | Los usuarios deben tener la opción de solicitar un viaje indicando punto de partida y destino, y el sistema debe mostrar las tarifas según una tabla de zonas predefinida. |
|                                | RF-016  | Al solicitar un viaje, el sistema debe notificar a todos los conductores disponibles.                                                                                     |
|                                | RF-017  | El sistema debe permitir que solo un conductor acepte cada solicitud de viaje.                                                                                            |
|                                | RF-018  | Los usuarios y conductores deben poder cancelar un viaje y proporcionar una razón para la cancelación.                                                                     |
|                                | RF-019  | Los usuarios deben ver información sobre el conductor asignado, como nombre, calificación y detalles del vehículo.                                                          |
|                                | RF-020  | Los conductores deben poder ver información básica sobre el usuario antes de aceptar un viaje.                                                                             |
| 7. Calificación y Comentarios  | RF-021  | Después de un viaje, los usuarios deben poder calificar a los conductores mediante un sistema de estrellas.                                                                  |
|                                | RF-022  | Los conductores deben poder calificar a los usuarios una vez completado el viaje.                                                                                         |
|                                | RF-023  | Los usuarios y conductores deben poder reportar problemas ocurridos durante el viaje, proporcionando una descripción detallada del incidente.                              |
| 8. Gestión de Conductores      | RF-024  | Los asistentes deben poder aceptar o rechazar solicitudes de empleo para conductores, revisando la información y documentos proporcionados.                                |
|                                | RF-025  | El sistema debe permitir a los asistentes desactivar conductores si es necesario.                                                                                          |
|                                | RF-026  | Los conductores deben recibir un resumen diario de sus ingresos, con un total acumulado disponible en su historial.                                                        |
| 9. Seguridad de Datos          | RF-027  | Todos los datos sensibles de usuarios, conductores y asistentes deben ser encriptados para asegurar la protección de la información.                                        |
| 10. Validaciones               | RF-028  | El sistema debe asegurarse de que no se permita el registro múltiple de una misma persona con la misma información.                                                        |

# STAKEHOLDERS.

| **Categoría**                | **Descripción**                                                                                          |
|------------------------------|----------------------------------------------------------------------------------------------------------|
| **Usuarios**                 | Personas que utilizan la aplicación para solicitar y gestionar viajes, así como para realizar pagos y calificaciones. |
| **Conductores**              | Personas que ofrecen servicios de transporte a través de la aplicación, gestionando viajes y actualizando su información. |
| **Asistentes**               | Personal que gestiona el registro de conductores y usuarios, revisa CVs y realiza tareas administrativas. |
| **Administradores**          | Encargados de supervisar todas las operaciones de la plataforma, gestionar la seguridad, y tomar decisiones estratégicas. |
| **Desarrolladores**          | Equipos técnicos responsables de crear, mantener y actualizar el software de la aplicación.              |
| **Equipo de Soporte Técnico**| Proporciona asistencia a usuarios, conductores y otros stakeholders en caso de problemas técnicos o consultas. |
| **Equipo de Marketing**      | Encargado de promover la aplicación, gestionar la comunicación con los usuarios y aumentar la visibilidad de la plataforma. |
| **Proveedores de Servicios** | Entidades que ofrecen servicios de infraestructura, como servidores y servicios de pago en línea.       |
| **Reguladores**              | Autoridades encargadas de asegurar que la aplicación cumpla con las leyes y regulaciones pertinentes.    |

# MATRIZ DE TRAZABILIDAD DE STAKEHOLDERS vs REQUERIMIENTOS.

| **Requerimiento Funcional**              | **Usuarios** | **Conductores** | **Asistentes** | **Administradores** | **Desarrolladores** | **Equipo de Soporte Técnico** | **Equipo de Marketing** | **Proveedores de Servicios** | **Reguladores** |
|------------------------------------------|--------------|-----------------|----------------|---------------------|----------------------|------------------------------|------------------------|-----------------------------|------------------|
| **Registro de Usuario**                  | X            |                 |                |                     | X                    | X                            | X                      | X                           | X                |
| **Registro de Conductores**              |              | X               | X              | X                   | X                    | X                            |                        | X                           | X                |
| **Registro de Asistentes**               |              |                 | X              | X                   | X                    | X                            |                        |                             | X                |
| **Inicio de Sesión**                     | X            | X               | X              | X                   | X                    | X                            |                        |                             | X                |
| **Modificar Información**                | X            | X               | X              | X                   | X                    | X                            |                        |                             | X                |
| **Calificar Conductor**                  | X            |                 |                |                     |                      |                              |                        |                             |                  |
| **Ver Información del Conductor**        | X            |                 |                |                     |                      |                              |                        |                             |                  |
| **Reportar Problemas**                   | X            | X               | X              | X                   | X                    | X                            |                        |                             |                  |
| **Métodos de Pago**                      | X            |                 |                |                     | X                    |                              |                        | X                           | X                |
| **Guardar Ubicación de Viaje**           | X            |                 |                |                     | X                    |                              |                        |                             |                  |
| **Cancelar Viaje**                       | X            |                 |                |                     | X                    |                              |                        |                             |                  |
| **Pedir Viaje**                          | X            |                 |                |                     | X                    |                              | X                      |                             | X                |
| **Aceptar Viaje**                        |              | X               |                |                     | X                    |                              |                        |                             | X                |
| **Cancelar Viaje (por el Conductor)**    |              | X               |                |                     | X                    |                              |                        |                             |                  |
| **Resumen de Ganancias**                 |              | X               |                |                     | X                    |                              |                        |                             |                  |
| **Generar Reportes**                     |              |                 |                | X                   | X                    |                              |                        |                             |                  |
| **Ver Calificaciones**                   |              |                 |                | X                   | X                    |                              |                        |                             |                  |
| **Estadísticas de Registro**             |              |                 |                | X                   | X                    |                              |                        |                             |                  |
| **Estadísticas de Uso**                  |              |                 |                | X                   | X                    |                              |                        |                             |                  |
| **Reporte de Ganancia**                  |              |                 |                | X                   | X                    |                              |                        |                             |                  |
| **Contratar Asistentes**                 |              |                 |                | X                   | X                    |                              |                        |                             |                  |
| **Dar de Baja a Asistentes**             |              |                 |                | X                   | X                    |                              |                        |                             |                  |

# MATRIZ DE TRAZABILIDAD DE STAKEHOLDERS vs CDU.

| **Casos de Uso / Stakeholders** | **Usuarios** | **Conductores** | **Asistentes** | **Administradores** | **Desarrolladores** | **Equipo de Soporte Técnico** | **Equipo de Marketing** | **Proveedores de Servicios** | **Reguladores** |
|--------------------------------|--------------|-----------------|----------------|----------------------|----------------------|------------------------------|------------------------|------------------------------|-----------------|
| **Inicio de Sesión**            | X            | X               |                | X                    | X                    | X                            |                        |                              |                 |
| **Envío de Mensajes**           | X            | X               |                |                      | X                    | X                            |                        |                              |                 |
| **Recepción de Mensajes**       | X            | X               |                |                      | X                    | X                            |                        |                              |                 |
| **Solicitar Viaje**             | X            |                 |                |                      | X                    | X                            |                        |                              |                 |
| **Gestionar Viajes**            |              | X               |                |                      | X                    | X                            |                        |                              |                 |
| **Realizar Pagos**              | X            |                 |                |                      | X                    | X                            |                        | X                            |                 |
| **Calificaciones y Comentarios**| X            | X               |                |                      | X                    | X                            |                        |                              |                 |
| **Registrar Conductores**       |              |                 | X              |                      | X                    |                              |                        |                              |                 |
| **Revisar CVs**                 |              |                 | X              |                      |                      |                              |                        |                              |                 |
| **Administrar Plataforma**      |              |                 |                | X                    | X                    |                              |                        |                              | X               |
| **Mantenimiento de Software**   |              |                 |                |                      | X                    |                              |                        |                              |                 |
| **Gestión de Incidencias**      | X            | X               |                |                      |                      | X                            |                        |                              |                 |
| **Promoción y Comunicación**    |              |                 |                |                      |                      |                              | X                      |                              |                 |
| **Servicios de Infraestructura**|              |                 |                |                      |                      |                              |                        | X                            |                 |
| **Cumplimiento de Regulaciones**|              |                 |                |                      |                      |                              |                        |                              | X               |

# MATRIZ DE TRAZABILIDAD: REQUERIMIENTOS FUNCIONALES vs CASOS DE USO.

| **Requerimiento Funcional / Caso de Uso** | **Registro de Usuario** | **Registro de Conductor** | **Registro de Asistente** | **Inicio de Sesión** | **Recuperación de Contraseña** | **Actualización de Información Personal** | **Solicitud de Viaje** | **Gestión de Viajes** | **Calificación y Comentarios** | **Gestión de Conductores** | **Seguridad de Datos** |
|-------------------------------------------|-------------------------|---------------------------|---------------------------|----------------------|-------------------------------|------------------------------------------|-------------------------|-----------------------|------------------------------|---------------------------|-------------------------|
| **RF-001**                               | X                       |                           |                           |                      |                               |                                          |                         |                       |                              |                           |                         |
| **RF-002**                               | X                       |                           |                           |                      |                               | X                                        |                         |                       |                              |                           |                         |
| **RF-003**                               | X                       |                           |                           |                      |                               |                                          |                         |                       |                              |                           |                         |
| **RF-004**                               |                         | X                         |                           |                      |                               |                                          |                         |                       |                              |                           |                         |
| **RF-005**                               |                         | X                         |                           |                      |                               |                                          |                         |                       |                              |                           |                         |
| **RF-006**                               |                         | X                         |                           |                      |                               |                                          |                         |                       |                              | X                         |                         |
| **RF-007**                               |                         |                           | X                         |                      |                               |                                          |                         |                       |                              |                           |                         |
| **RF-008**                               |                         |                           | X                         |                      |                               |                                          |                         |                       |                              |                           |                         |
| **RF-009**                               | X                       | X                         | X                         | X                    |                               |                                          |                         |                       |                              |                           |                         |
| **RF-010**                               | X                       | X                         | X                         |                      |                               |                                          |                         |                       |                              |                           |                         |
| **RF-011**                               | X                       | X                         | X                         | X                    | X                             |                                          |                         |                       |                              |                           |                         |
| **RF-012**                               |                         |                           |                           | X                    |                               |                                          |                         |                       |                              |                           |                         |
| **RF-013**                               | X                       |                           |                           |                      |                               | X                                        |                         |                       |                              |                           |                         |
| **RF-014**                               |                         | X                         |                           |                      |                               | X                                        |                         |                       |                              |                           |                         |
| **RF-015**                               |                         |                           |                           |                      |                               |                                          | X                       |                       |                              |                           |                         |
| **RF-016**                               |                         |                           |                           |                      |                               |                                          | X                       |                       |                              |                           |                         |
| **RF-017**                               |                         |                           |                           |                      |                               |                                          | X                       |                       |                              |                           |                         |
| **RF-018**                               | X                       | X                         |                           |                      |                               |                                          | X                       |                       |                              |                           |                         |
| **RF-019**                               | X                       |                           |                           |                      |                               |                                          | X                       |                       |                              |                           |                         |
| **RF-020**                               |                         | X                         |                           |                      |                               |                                          |                         |                       |                              |                           |                         |
| **RF-021**                               | X                       |                           |                           |                      |                               |                                          |                         |                       | X                            |                           |                         |
| **RF-022**                               |                         | X                         |                           |                      |                               |                                          |                         |                       | X                            |                           |                         |
| **RF-023**                               | X                       | X                         |                           |                      |                               |                                          |                         |                       | X                            |                           |                         |
| **RF-024**                               |                         | X                         |                           |                      |                               |                                          |                         |                       |                              | X                         |                         |
| **RF-025**                               |                         | X                         |                           |                      |                               |                                          |                         |                       |                              | X                         |                         |
| **RF-026**                               |                         | X                         |                           |                      |                               |                                          |                         | X                     |                              |                           |                         |
| **RF-027**                               | X                       | X                         | X                         | X                    |                               | X                                        |                         |                       |                              |                           | X                       |
| **RF-028**                               | X                       |                           |                           |                      |                               |                                          |                         |                       |                              |                           |                         |


# DIAGRAMA DE DESPLIEGUE

![Diagrama de Despliegue](/Diagramas/Diagrama%20de%20Despliegue.png)

# ESTILO ARQUITECTONICO

La arquitectura seleccionada es una arquitectura de n niveles (también conocida como arquitectura de capas o "multi-tier architecture"), específicamente una arquitectura de 3 niveles. Los tres niveles principales en esta arquitectura son:

## 1. Nivel de Presentación (Frontend)

Compuesto por los servidores web que manejan la interacción con el usuario a través de la interfaz web (en este caso, utilizando React). Estos servidores reciben las solicitudes de los clientes y envían las respuestas de vuelta después de que se hayan procesado.

## 2. Nivel de Lógica de Negocio (Backend)

Representado por los servidores backend que ejecutan Node.js. Este nivel maneja la lógica de la aplicación, procesando las reglas de negocio y controlando el flujo de la información entre la capa de presentación y la capa de datos.

## 3. Nivel de Datos

Compuesto por el servidor de base de datos MySQL y el almacenamiento en AWS S3. Esta capa se encarga de gestionar y almacenar los datos que utiliza la aplicación, así como de recuperar y actualizar la información según las necesidades de la aplicación.

# Justificación de la Arquitectura de n Capas

### 1. Escalabilidad

Cada nivel se puede escalar de manera independiente según las necesidades de la aplicación, lo que permite gestionar mejor el crecimiento del tráfico y los volúmenes de datos.

### 2. Mantenibilidad

Separar la aplicación en capas distintas facilita el mantenimiento y la actualización del sistema, ya que se puede modificar un nivel sin afectar significativamente a los otros.

### 3. Seguridad

Al tener diferentes capas, es posible implementar políticas de seguridad específicas para cada nivel, protegiendo los datos y el acceso según corresponda.

### Diagrama n-capas

![Diagrama de Despliegue](/Diagramas/Diagrama%20capas.jpg)

