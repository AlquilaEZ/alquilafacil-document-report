# Capitulo III: Requirements Specification

## 3.1 To-Be Scenario Mapping

![To-be Mapping](Resources/To-be-iot.jpeg)

## 3.2 User Stories

**Epics**

| Epic / Story ID | Título                                 | Descripción                                                                                                                                                                   | Historias de Usuario Relacionadas       |
|-----------------|----------------------------------------|-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|-----------------------------------------|
| EP01            | Gestión de usuarios y autenticación    | Como usuario de AlquilaFácil, quiero poder registrarme fácilmente en la aplicación y acceder a mi cuenta, para poder utilizar las funcionalidades principales sin complicaciones. | US01, US02, US14, US17                  |
| EP02            | Registro y gestión de espacios         | Como arrendador de AlquilaFácil, quiero poder registrar, modificar y promocionar mis espacios en la plataforma para asegurarme de que los arrendatarios puedan ver y reservar mis propiedades de manera fácil y rápida. | US03, US12, US13                        |
| EP03            | Búsqueda y reserva de espacios         | Como arrendatario de AlquilaFácil, quiero poder buscar y reservar espacios de acuerdo con mis necesidades (por capacidad, categoría, y ubicación), para encontrar el lugar perfecto para mi evento y asegurar su disponibilidad. | US04, US05, US06, US07, US11, US15, US16 |
| EP04            | Gestión de agenda de usuario           | Como usuario de AlquilaFácil, quiero poder gestionar mis reservas y recibir notificaciones sobre cambios y actividades relacionadas con mis espacios, para mantenerme organizado y al tanto de todo en tiempo real. | US08, US09, US10                        |

**User Stories**

| ID de la user story | Título| Descripción|Criterios de aceptación|
|---------------------|-------------------------------------------|---------------------------------------------------------------------------------------------------------------------------------------------------|--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| US01                | Registrar usuario                         | Como usuario de la aplicación móvil de AlquilaFácil de un espacio para eventos, quiero poder registrarme fácilmente en AlquilaFácil para ofrecer mi espacio en alquiler y llegar a más clientes potenciales. | Escenario 01: Registro exitoso  <br> **Dado** que un usuario desea registrar su espacio en AlquilaFácil. **Cuando** el usuario completa el formulario de registro con la información requerida. **Entonces** el usuario recibe una confirmación de registro y puede acceder a su cuenta. <br><br> Escenario 02: Validación de datos <br> **Dado** que un usuario completa el formulario de registro en AlquilaFácil. **Cuando** el usuario envía el formulario. **Entonces** los datos proporcionados se validan para garantizar la precisión y la autenticidad. |
| US02                | Iniciar sesión                            | Como usuario registrado de la aplicación móvil de AlquilaFácil, quiero poder iniciar sesión fácilmente en mi cuenta, para gestionar mi espacio en alquiler y acceder a mis mensajes y notificaciones. | Escenario 01: Inicio de sesión exitoso <br> **Dado** que un usuario registrado desea acceder a su cuenta en AlquilaFácil. **Cuando** el usuario ingresa su correo electrónico y contraseña correctos en el formulario de inicio de sesión. **Entonces** el usuario es autenticado exitosamente y se le otorga acceso a su cuenta. <br><br> Escenario 02: Error en el inicio de sesión por credenciales incorrectas <br> **Dado** que un usuario registrado intenta acceder a su cuenta en AlquilaFácil. **Cuando** el usuario ingresa una combinación incorrecta de correo electrónico o contraseña. **Entonces** se le muestra un mensaje de error indicando que las credenciales son incorrectas y se le solicita que intente nuevamente. |
| US03                | Registrar espacios                        | Como arrendador de un espacio para eventos en AlquilaFácil, quiero poder registrar mi espacio para comenzar a recibir solicitudes de reserva lo antes posible. | Escenario 01: Registro de datos básicos <br> **Dado** que un arrendador desea registrar su espacio en AlquilaFácil. **Cuando** completa distintos campos organizados en varios pasos detallados que incluyen información detallada sobre la propiedad. **Entonces** puede enviar el registro con éxito y recibir confirmación de su inclusión en la plataforma. <br><br> Escenario 02: Validación de datos requeridos en cada paso del registro <br> **Dado** que un arrendador está completando el registro de su espacio en AlquilaFácil. **Cuando** rellena todos los campos correspondientes a un paso en específico. **Entonces** se activa el botón que le permite continuar al siguiente paso. |
| US04                | Buscar espacios disponibles               | Como arrendatario, quiero poder buscar fácilmente espacios disponibles en AlquilaFácil para encontrar el lugar perfecto para mi evento.            | Escenario 01: Búsqueda principal por ubicación <br> **Dado** que un arrendatario busca un espacio para eventos en una ubicación específica. **Cuando** el arrendatario ingresa la ubicación deseada en el campo de búsqueda. **Entonces** se muestran los espacios disponibles en esa ubicación. <br><br> Escenario 02: Búsqueda general de espacios <br> **Dado** que un arrendatario no ingresa algún texto en la barra de búsqueda. **Cuando** presiona sobre el ícono para buscar espacios. **Entonces** se muestran todos los espacios disponibles. |
| US05                | Filtrar espacios disponibles              | Como arrendatario, quiero poder filtrar los espacios disponibles por capacidad y categoría, para encontrar uno que cumpla con mis criterios específicos. | Escenario 01: Filtrado por capacidad <br> **Dado** que un arrendatario desea un espacio con capacidad para un número específico de personas. **Cuando** el arrendatario aplica un filtro de capacidad en la búsqueda. **Entonces** se muestran solo los espacios que cumplen con ese criterio. <br><br> Escenario 02: Filtrado por categoría <br> **Dado** que un arrendatario desea un espacio de una categoría en específico. **Cuando** el arrendatario aplica un filtro de categoría en la búsqueda. **Entonces** se muestran solo los espacios que cumplen con ese criterio. |
| US06                | Visualizar información del espacio        | Como arrendatario, quiero poder visualizar información detallada del espacio, para evaluar si cumple con los requisitos de mi evento antes de hacer una reserva. | Escenario 01: Visualización de información <br> **Dado** que el arrendatario selecciona un espacio en AlquilaFácil. **Cuando** accede a la página de detalles del espacio. **Entonces** puede visualizar información detallada como el aforo máximo, descripción del espacio y servicios disponibles. <br><br> Escenario 02: Visualización de reseñas del espacio <br> **Dado** que el arrendatario está revisando un espacio. **Cuando** accede a la página de comentarios. **Entonces** puede visualizar las reseñas y calificaciones dejadas por otros usuarios sobre ese espacio. |
| US07                | Reservar espacios                         | Como arrendatario, quiero poder reservar un espacio para mi evento en AlquilaFácil para garantizar su disponibilidad en la fecha deseada. | Escenario 01: Proceso de Reserva <br> Dado que un arrendatario ha encontrado el espacio ideal en AlquilaFácil. Cuando selecciona un espacio y una fecha. Entonces se muestra un formulario de para completar los detalles de reserva. <br><br> Escenario 02: Pago de la reserva con PayPal <br> **Dado** que el usuario está a punto de culminar el proceso de reserva de un espacio. **Cuando** el usuario presione el botón de realizar reserva. **Entonces** el usuario realizará el pago de la reserva a través de PayPal. <br><br> Escenario 03: Confirmación de Reserva <br> Dado que un arrendatario ha realizado el pago de la reserva en AlquilaFácil. Cuando el arrendatario es redirigido a la aplicación. Entonces recibe una confirmación de reserva y los detalles se actualizan en su cuenta. |
| US08                | Gestionar calendario de reservas          | Como usuario de AlquilaFácil, quiero poder controlar una agenda de reservas para tener un horario organizado y evitar conflictos futuros. | Escenario 01: Existencia de reserva de usuario normal <br> Dado que un arrendatario ha realizado una reserva   de uno de mis espacios. Cuando el propietario accede al calendario. Entonces puede ver el día de la reserva resaltada en color rojo. <br><br> Escenario 02: Existencia de reserva de usuario premium <br> Dado que un arrendatario con suscripción premium ha realizado una reserva   de uno de mis espacios. Cuando el propietario accede al calendario. Entonces puede ver el día de la reserva resaltada en color amarillo. <br><br> Escenario 03: Existencia de reserva de espacio ajeno <br> Dado que un arrendatario ha realizado una reserva de espacio. Cuando este accede al calendario. Entonces puede ver el día de su reserva resaltada en color azul. |
| US09                | Calificar y comentar sobre espacios       | Como arrendatario, quiero poder publicar mi reseña sobre un espacio que he reservado para que otros usuarios puedan conocer mi experiencia sobre este. | Escenario 01: Permiso para opinar sobre un espacio <br> Dado que un arrendatario tiene una reserva culminada de un espacio. Cuando accede a su información a través del calendario. Entonces se presenta la opción habilitada para que pueda publicar su reseña sobre este. <br><br> Escenario 02: Aporte de reseña <br> Dado que un arrendatario ha rellenado todos los campos de reseña. Cuando presiona el campo de realizar reseña. Entonces esta se publica para que todos los usuarios la puedan ver. |
| US10                | Notificar sobre actividades de arrendatarios | Como arrendador de un espacio para eventos en AlquilaFácil, quiero recibir notificaciones **Cuando** un arrendatario ha realizado cierta acción sobre mi espacio para estar al tanto de su estado y tomar las acciones pertinentes.  | Escenario 01: Notificación de reserva <br> **Dado** que el arrendador ha publicado un espacio en AlquilaFácil. **Cuando** un arrendatario realiza una reserva para dicho espacio. **Entonces** el arrendador recibe una notificación en la aplicación indicando que el espacio ha sido reservado, con detalles de la fecha y el nombre del arrendatario.  <br><br> Escenario 02: Notificación de reseña <br> **Dado** que el arrendador ha publicado un espacio en AlquilaFácil. **Cuando** un arrendatario realiza una reseña sobre dicho espacio. **Entonces** el arrendador recibe una notificación en la aplicación que le permite ver el comentario y la calificación otorgada, ayudándole a monitorear la satisfacción del cliente.  |
| US11                | Controlar espacios favoritos              | Como arrendatario en AlquilaFácil, quiero poder agregar un espacio a mis favoritos para guardar y acceder rápidamente a los lugares de interés para futuras reservas. | Escenario 01: Agregar a favoritos <br> **Dado** que el arrendatario está visualizando la página de detalles de un espacio. **Cuando** selecciona la opción de "Agregar a favoritos". **Entonces** el espacio se guarda en la lista de favoritos de forma local. <br><br> Escenario 02: Eliminar de favoritos <br> **Dado** que el arrendatario ha guardado un espacio como favorito. **Cuando** selecciona la opción de "Eliminar de favoritos" en dicho espacio. **Entonces** el espacio se elimina de la lista de favoritos, y ya no se mostrará al realizar el filtrado.  |
| US12                | Visualizar espacios propios publicados    | Como arrendador en AlquilaFácil, quiero poder visualizar todos los espacios que he publicado en la plataforma, para gestionar fácilmente la información de mis propiedades.  | Escenario 01: Listado de espacios publicados <br> **Dado** que el arrendador ha iniciado sesión en su cuenta de AlquilaFácil. **Cuando** accede a la sección "Mis espacios". **Entonces** puede ver una lista de todos los espacios que ha publicado, incluyendo información básica como nombre del espacio, ubicación. <br><br> Escenario 02: Acceso a detalles y edición <br> **Dado** que el arrendador visualiza la lista de espacios publicados. **Cuando** selecciona un espacio específico. **Entonces** puede acceder a la página de detalles de ese espacio donde tiene la opción de editar la información. |
| US13                | Modificar espacios publicados             | Como arrendador de un espacio en AlquilaFácil, quiero poder modificar la información de los espacios que he publicado, incluyendo detalles como la descripción, aforo, servicios disponibles, tarifas y visibilidad temporal, para asegurar que los datos sean precisos y estén actualizados.  | Escenario 01: Edición de detalles del espacio <br> **Dado** que el arrendador desea actualizar la información de su espacio. **Cuando** accede a la sección de edición de su espacio y realiza modificaciones en campos como descripción, aforo, servicios disponibles y tarifas. **Entonces** puede guardar los cambios, y estos se reflejan en la página de detalles del espacio para todos los usuarios una vez finalizada la edición. <br><br> Escenario 02: Modificación de visibilidad Temporal del espacio <br> **Dado** que el arrendador está realizando modificaciones en su espacio. **Cuando** activa la opción de "No disponible temporalmente" para realizar cambios. **Entonces** el espacio se muestra como no disponible para reservas. |
| US14                | Actualizar perfil y sesión de usuario     | Como usuario de AlquilaFácil, quiero poder modificar mi perfil, incluyendo la opción de cambiar mi nombre de usuario y cerrar sesión, para mantener actualizada mi información personal y gestionar mi acceso a la aplicación de manera conveniente. | Escenario 01: Modificación del nombre de usuario <br> **Dado** que el usuario ha iniciado sesión en su cuenta de AlquilaFácil. **Cuando** accede a la sección de configuración de perfil y edita el campo "Nombre de usuario". **Entonces** puede guardar los cambios, y el nuevo nombre de usuario se refleja en su perfil y en todas las interacciones futuras en la plataforma. <br><br> Escenario 02: Cierre de sesión <br> **Dado** que el usuario desea salir de su cuenta en AlquilaFácil. **Cuando** selecciona la opción "Cerrar sesión" en la configuración de perfil. **Entonces** es desconectado de su cuenta y redirigido a la pantalla de inicio de sesión, asegurando que su sesión se haya cerrado de manera segura.|
| US15                | Reportar espacios inseguros               | Como usuario de AlquilaFácil, quiero poder reportar espacios inseguros, para contribuir a la seguridad de la comunidad y alertar sobre situaciones que puedan poner en riesgo a otros usuarios.  |Escenario 01: Selección del espacio inseguro <br> **Dado** que el usuario ha iniciado sesión en su cuenta de AlquilaFácil. **Cuando** accede a la sección de "Reportar espacio" y selecciona el espacio desde la lista de reservas activas o buscando un espacio específico. **Entonces** puede ingresar un asunto y descripción del problema. <br><br> Escenario 02: Confirmación del reporte <br> **Dado** que el usuario ha completado el formulario de reporte con todos los detalles requeridos. **Cuando** envía el reporte mediante el botón "Enviar". **Entonces** el reporte será registrado y revisado por el equipo de soporte de AlquilaFácil. |
| US16                | Visualizar espacios reportados por el usuario | Como usuario de AlquilaFácil, quiero poder visualizar los espacios que he reportado, para realizar un seguimiento de mis reportes y gestionarlos.  | Escenario 01: Navegar a la sección de "Ver Espacios Reportados" <br> **Dado** que el usuario ha iniciado sesión en su cuenta de AlquilaFácil. **Cuando** accede a la sección de "Ver Espacios Reportados" desde el panel de control. **Entonces** puede ver una lista de los espacios que ha reportado, incluyendo información como el nombre del espacio, la fecha del reporte, y el motivo del reporte. <br><br> Escenario 02: Eliminar un reporte deslizando hacia la izquierda <br> **Dado** que el usuario se encuentra en la lista de espacios reportados. **Cuando** desliza uno de los reportes hacia la izquierda. **Entonces** aparece una opción para confirmar la eliminación del reporte. Y si confirma, el reporte se elimina de la lista. |
| US17                | Iniciar sesión con servicios externos     | Como usuario de AlquilaFácil, quiero poder iniciar sesión utilizando servicios externos como Google o Outlook, para ahorrar tiempo y evitar tener que crear una cuenta desde cero. | Escenario 01: Inicio de sesión con Google <br> **Dado** que un usuario está en la pantalla de inicio de sesión de AlquilaFácil, **Cuando** hace clic en "Iniciar sesión con Google", **Entonces** el sistema redirige al usuario a la pantalla de autenticación de Google, donde ingresa sus credenciales y otorga permisos. <br><br> Escenario 02: Inicio de sesión con Facebook <br> **Dado** que un usuario está en la pantalla de inicio de sesión de AlquilaFácil, **Cuando** hace clic en "Iniciar sesión con Facebook", **Entonces** el sistema redirige al usuario a la pantalla de autenticación de Google, donde ingresa sus credenciales y otorga permisos. |
| US18                | Acceder a información de ayuda            | Como usuario de AlquilaFácil, quiero poder acceder fácilmente a una sección de preguntas frecuentes e información de contacto para resolver mis dudas o comunicarme con el soporte **Cuando** lo necesite. | Escenario 01: Consultar preguntas frecuentes <br> **Dado** que un usuario tiene una duda común sobre el funcionamiento de la plataforma. **Cuando** selecciona la opción de "Preguntas frecuentes" en el menú de ayuda. **Entonces** se muestra una lista de preguntas con sus respuestas para ayudar al usuario. <br><br> Escenario 02: Acceder a información de contacto <br> **Dado** que un usuario necesita comunicarse con el soporte. **Cuando** selecciona la opción de "Información de contacto" en el menú de ayuda. **Entonces** se muestra la información de contacto, incluyendo el correo electrónico y número de teléfono del soporte. |
| US19                | Control de Aforo                          | Como arrendador, quiero recibir información en tiempo real sobre el número de personas presentes en mi local durante un evento, para asegurarme de que no se exceda el aforo permitido. | - **Dado** que hay un evento activo, **cuando** se detecta que el número de personas se acerca al límite permitido, **entonces** se muestra una alerta en la app del arrendador.<br> - **Dado** que se ha superado el aforo máximo permitido, **cuando** esto ocurre, **entonces** el sistema debe notificar al arrendador inmediatamente por notificación push **y** correo electrónico. |
| US20                | Monitoreo de Niveles de Ruido             | Como arrendador, quiero que el sistema me notifique si el nivel de ruido supera un umbral establecido, para poder tomar acciones preventivas. | - **Dado** que se ha configurado un umbral de ruido, **cuando** los decibeles exceden ese límite, **entonces** el sistema envía una notificación al arrendador.<br> - **Dado** que el evento sigue en curso, **cuando** los niveles de ruido vuelven a la normalidad, **entonces** el sistema registra automáticamente el tiempo total del exceso. |
| US21                | Detección de Humo                         | Como arrendador, quiero que se active una alerta automática si se detecta humo en el local durante un evento, para verificar si hay una situación de riesgo. | - **Dado** que hay sensores de humo activos, **cuando** se detecta presencia de humo, **entonces** se envía una notificación crítica al arrendador.<br> - **Dado** que se ha enviado una alerta de humo, **cuando** el usuario accede a la app, **entonces** debe visualizar el evento en un panel de incidentes con la hora exacta de detección. |
| US22                | Movimiento en Áreas No Autorizadas        | Como arrendador, quiero recibir notificaciones si se detecta movimiento en zonas restringidas, para asegurar que los arrendatarios respeten los espacios delimitados. | - **Dado** que se ha definido una zona como restringida, **cuando** se detecta movimiento en esa área, **entonces** el arrendador recibe una alerta inmediata con la ubicación del incidente.<br> - **Dado** que ocurre una intrusión, **cuando** el evento es registrado, **entonces** debe quedar un historial con fecha, hora **y** duración del movimiento. |
| US23                | Registro de Incidentes                    | Como arrendador, quiero acceder a un historial con todos los eventos registrados por sensores, para tener evidencia y mejorar la gestión. | - **Dado** que han ocurrido incidentes durante un evento, **cuando** el arrendador accede al panel de historial, **entonces** puede ver un listado con fecha, tipo de incidente **y** duración.<br> - **Dado** que se selecciona un evento del historial, **cuando** el usuario lo abre, **entonces** debe poder ver detalles como gráfico de actividad, sensores involucrados **y** ubicación dentro del local. |

## 3.3 Impact Mapping

## 3.4 Product Backlog

<div align="center">
    <table>
        <thead>
            <tr>
                <th>User Stories ID</th>
                <th>Título</th>
                <th>Descripción</th>
                <th>Story Points (1/2/3/5/8)</th>
            </tr>
        </thead>
        <tbody>
            <tr>
                <td>US03</td>
                <td>Registrar espacios</td>
                <td>Como arrendador de un espacio para eventos en AlquilaFácil, quiero poder registrar mi espacio para comenzar a recibir solicitudes de reserva lo antes posible.</td>
                <td>8</td>
            </tr>
            <tr>
                <td>US04</td>
                <td>Buscar espacios disponibles</td>
                <td>Como arrendatario, quiero poder buscar fácilmente espacios disponibles en AlquilaFácil para encontrar el lugar perfecto para mi evento.</td>
                <td>5</td>
            </tr>
            <tr>
                <td>US05</td>
                <td>Filtrar espacios disponibles</td>
                <td>Como arrendatario, quiero poder filtrar los espacios disponibles por capacidad y categoría, para encontrar uno que cumpla con mis criterios específicos.</td>
                <td>5</td>
            </tr>
            <tr>
                <td>US06</td>
                <td>Visualizar información del espacio</td>
                <td>Como arrendatario, quiero poder visualizar información detallada del espacio, para evaluar si cumple con los requisitos de mi evento antes de hacer una reserva.</td>
                <td>5</td>
            </tr>
            <tr>
                <td>US07</td>
                <td>Reservar espacios</td>
                <td>Como arrendatario, quiero poder reservar un espacio para mi evento en AlquilaFácil para garantizar su disponibilidad en la fecha deseada.</td>
                <td>8</td>
            </tr>
            <tr>
                <td>US12</td>
                <td>Visualizar espacios propios publicados</td>
                <td>Como arrendador en AlquilaFácil, quiero poder visualizar todos los espacios que he publicado en la plataforma, para gestionar fácilmente la información de mis propiedades.</td>
                <td>3</td>
            </tr>
            <tr>
                <td>US13</td>
                <td>Modificar espacios publicados</td>
                <td>Como arrendador de un espacio en AlquilaFácil, quiero poder modificar la información de los espacios que he publicado, incluyendo detalles como la descripción, aforo, servicios disponibles, tarifas y visibilidad temporal, para asegurar que los datos sean precisos y estén actualizados.</td>
                <td>3</td>
            </tr>
            <tr>
                <td>US08</td>
                <td>Gestionar calendario de reservas</td>
                <td>Como usuario de AlquilaFácil, quiero poder controlar una agenda de reservas para tener un horario organizado y evitar conflictos futuros.</td>
                <td>5</td>
            </tr>
            <tr>
                <td>US19</td>
                <td>Control de aforo</td>
                <td>Como arrendador, quiero recibir información en tiempo real sobre el número de personas presentes en mi local durante un evento, para asegurarme de que no se exceda el aforo permitido.</td>
                <td>3</td>
            </tr>
            <tr>
                <td>US20</td>
                <td>Monitoreo de niveles de ruido</td>
                <td>Como arrendador, quiero que el sistema me notifique si el nivel de ruido supera un umbral establecido, para poder tomar acciones preventivas.</td>
                <td>3</td>
            </tr>
            <tr>
                <td>US21</td>
                <td>Detección de humo</td>
                <td>Como arrendador, quiero que se active una alerta automática si se detecta humo en el local durante un evento, para verificar si hay una situación de riesgo.</td>
                <td>5</td>
            </tr>
            <tr>
                <td>US22</td>
                <td>Movimiento en áreas No autorizadas</td>
                <td>Como arrendador, quiero recibir notificaciones si se detecta movimiento en zonas restringidas, para asegurar que los arrendatarios respeten los espacios delimitados.</td>
                <td>5</td>
            </tr>
            <tr>
                <td>US23</td>
                <td>Registro de incidentes</td>
                <td>Como arrendador, quiero acceder a un historial con todos los eventos registrados por sensores, para tener evidencia y mejorar la gestión.</td>
                <td>5</td>
            </tr>
            <tr>
                <td>US09</td>
                <td>Calificar y comentar sobre espacios</td>
                <td>Como arrendatario, quiero poder publicar mi reseña sobre un espacio que he reservado para que otros usuarios puedan conocer mi experiencia sobre este.</td>
                <td>3</td>
            </tr>
            <tr>
                <td>US11</td>
                <td>Controlar espacios favoritos</td>
                <td>Como arrendatario en AlquilaFácil, quiero poder agregar un espacio a mis favoritos para guardar y acceder rápidamente a los lugares de interés para futuras reservas.</td>
                <td>3</td>
            </tr>
            <tr>
                <td>US15</td>
                <td>Reportar espacios inseguros</td>
                <td>Como usuario de AlquilaFácil, quiero poder reportar espacios inseguros, para contribuir a la seguridad de la comunidad y alertar sobre situaciones que puedan poner en riesgo a otros usuarios.</td>
                <td>3</td>
            </tr>
            <tr>
                <td>US16</td>
                <td>Visualizar espacios reportados</td>
                <td>Como usuario de AlquilaFácil, quiero poder visualizar los espacios que he reportado, para realizar un seguimiento de mis reportes y gestionarlos.</td>
                <td>3</td>
            </tr>
            <tr>
                <td>US01</td>
                <td>Registrar usuario</td>
                <td>Como usuario de la aplicación móvil de AlquilaFácil de un espacio para eventos, quiero poder registrarme fácilmente en AlquilaFácil para ofrecer mi espacio en alquiler y llegar a más clientes potenciales.</td>
                <td>3</td>
            </tr>
            <tr>
                <td>US02</td>
                <td>Iniciar sesión</td>
                <td>Como usuario registrado de la aplicación móvil de AlquilaFácil, quiero poder iniciar sesión fácilmente en mi cuenta, para gestionar mi espacio en alquiler y acceder a mis mensajes y notificaciones.</td>
                <td>3</td>
            </tr>
            <tr>
                <td>US10</td>
                <td>Notificar sobre actividades de arrendatarios</td>
                <td>Como arrendador de un espacio para eventos en AlquilaFácil, quiero recibir notificaciones Cuando un arrendatario ha realizado cierta acción sobre mi espacio para estar al tanto de su estado y tomar las acciones pertinentes.</td>
                <td>3</td>
            </tr>
            <tr>
                <td>US17</td>
                <td>Permitir iniciar sesión con servicios externos</td>
                <td>Como usuario de AlquilaFácil, quiero poder iniciar sesión utilizando servicios externos como Google o Outlook, para ahorrar tiempo y evitar tener que crear una cuenta desde cero.</td>
                <td>2</td>
            </tr>
            <tr>
                <td>US14</td>
                <td>Actualizar perfil y sesión de usuario</td>
                <td>Como usuario de AlquilaFácil, quiero poder modificar mi perfil, incluyendo la opción de cambiar mi nombre de usuario y cerrar sesión, para mantener actualizada mi información personal y gestionar mi acceso a la aplicación de manera conveniente.</td>
                <td>2</td>
            </tr>
            <tr>
                <td>US18</td>
                <td>Acceder a información de ayuda</td>
                <td>Como usuario de AlquilaFácil, quiero poder acceder fácilmente a una sección de preguntas frecuentes e información de contacto para resolver mis dudas o comunicarme con el soporte Cuando lo necesite.</td>
                <td>5</td>
            </tr>
        </tbody>
    </table>
</div>