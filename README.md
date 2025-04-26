#Capítulo IV: Solution Software Design

##4.1. Strategic-Level Domain-Driven Design

###4.1.1. Event Storming
<p>
EventStorming es una técnica de modelado colaborativo e iterativo que permite analizar a fondo problemas complejos y de gran escala, ayudando a descubrir una amplia variedad de detalles y desafíos involucrados.</p>

![Event Storming](/images/imagen_1.png)

Enlace del Miroo para verlo completo:[ https://miro.com/app/board/uXjVKldWbQI=/?share_link_id=811519345320](https://miro.com/app/board/uXjVIBJ9674=/)

####4.1.1.1 Candidate Context Discovery

<strong>Step 1: Unstructured Exploration</strong>:<br>
<p>En la etapa inicial del EventStorming, se lleva a cabo una sesión de lluvia de ideas destinada a descubrir los eventos clave del dominio vinculados al negocio analizado. Es importante redactar estos eventos utilizando verbos en pasado, ya que deben reflejar acciones que ya han sucedido dentro del sistema o proceso.</p>

![Event Storming](/images/imagen_2.png)


<p>Realizamos una sesión de lluvia de ideas para identificar todos los eventos relevantes que el sistema de reservas de locales con tecnología IoT debe manejar. En esta etapa inicial del Event Storming se mapearon eventos clave como la creación de cuentas, registro y actualización de locales, postulaciones y confirmación de reservas, así como la entrada y salida del arrendatario mediante pulsera NFC. También se incluyeron eventos generados por sensores, como detección de humo, sobreaforo y accesos no autorizados, fundamentales para garantizar el cumplimiento de las normas del local. Se consideraron alertas automáticas enviadas tanto al arrendador como al arrendatario en caso de infracciones, así como acciones relacionadas con la gestión de reportes, historial de asistencia e interacciones con la app móvil. Este mapeo inicial permite tener una visión integral de todos los comportamientos que el sistema debe registrar y reaccionar para brindar una solución de monitoreo y control eficaz para ambas partes involucradas</p>


<strong>Step 2: Timelines</strong>:<br>
<p>En esta segunda etapa, se toman los eventos de dominio identificados y se ordenan cronológicamente según su secuencia natural dentro del proceso. El primer enfoque consiste en construir un "camino feliz" (happy path), es decir, una secuencia ideal en la que todas las acciones se ejecutan correctamente y el flujo del sistema se desarrolla sin inconvenientes. Una vez definido este escenario óptimo, se incorporan variaciones o situaciones alternativas que representen posibles errores, fallos o condiciones excepcionales dentro del flujo operativo.</p>


![Event Storming](/images/imagen_3.png)


<p>En esta segunda fase del Event Storming, organizamos los eventos de dominio identificados previamente en flujos secuenciales que reflejan cómo se comporta el sistema ante diferentes escenarios relacionados con el proceso de reserva, ingreso y monitoreo del uso del local. El flujo principal sigue un "camino feliz" donde el usuario inicia sesión, selecciona un local, crea una reserva, asiste con su pulsera NFC, y completa la experiencia sin incidentes, incluyendo la generación de reportes y la calificación del local.
Además, se contemplan trayectorias alternativas que incluyen detecciones de humo, ruido o exceso de aforo, así como ingresos fuera de horario o con pulseras no autorizadas. Estas situaciones activan mecanismos de control como el registro de infracciones, el envío de notificaciones al arrendador o arrendatario, y la actualización del historial de eventos. Esta organización permite visualizar cómo el sistema reacciona ante distintos contextos operativos, sentando las bases para diseñar una lógica robusta, trazable y automatizada tanto en la app móvil como en la plataforma web.</p>


<strong>Step 3: Paint Points</strong>:<br>
<p>Una vez que los eventos fueron organizados en una secuencia temporal, utilizamos esta visión global del proceso para detectar áreas clave que requieren atención. Estos puntos críticos pueden manifestarse como cuellos de botella operativos, tareas manuales susceptibles de automatización, ausencia de documentación relevante o vacíos en el entendimiento del dominio. Esta revisión permite anticipar mejoras y definir prioridades para el diseño del sistema.</p>


![Event Storming](/images/imagen_4.png)


<p>En esta fase del Event Storming, se identificaron los puntos críticos del sistema y se documentaron preguntas clave que deben ser respondidas para garantizar el correcto funcionamiento del proceso de reservas, ingreso y monitoreo de locales. Estas preguntas se integran directamente en los flujos de eventos y permiten explorar escenarios como la verificación de acceso mediante pulseras NFC, la validación del cronograma de reservas o la forma en que se detectan eventos de sobreaforo, humo o ruido durante el uso del local.
</p>






<strong>Step 4: Pivotal Points</strong>:<br>
<p>Una vez que se ha construido la línea de eventos completa, incluyendo los puntos de dolor, se procede a identificar aquellos eventos relevantes que representan un cambio significativo en el contexto o en la etapa del proceso. Estos se conocen como eventos principales, y se utilizan como puntos de corte dentro del flujo, marcando una transición clara entre lo que ocurre antes y lo que sucede después. Para visualizarlos, se incorpora una barra vertical que divide los eventos previos de los posteriores a dicho hito</p>


![Event Storming](/images/imagen_5.png)


<p>Hemos identificado los eventos principales (pivotal points) que marcan transiciones clave dentro del sistema de reservas y monitoreo de locales con tecnología IoT. Estos eventos delimitan fases importantes del proceso y permiten establecer momentos en los que es necesario validar decisiones fundamentales para garantizar el correcto funcionamiento del sistema.
</p>




<strong>Step 5: Commands</strong>:<br>
<p>En esta etapa también incorporamos los comandos, los cuales representan las acciones que desencadenan uno o varios eventos dentro del sistema. A diferencia de los eventos de dominio, que describen hechos ya ocurridos, los comandos se expresan en forma imperativa, indicando las operaciones que deben llevarse a cabo en el sistema para provocar un cambio en su estado o avanzar en el flujo del proceso</p>


![Event Storming](/images/imagen_6.png)






<strong>Step 6: Policies</strong>:<br>
<p>En esta etapa se identifican las políticas de automatización, es decir, reglas que permiten que ciertos comandos se ejecuten automáticamente en respuesta a eventos del dominio. Esto implica que, al producirse un evento específico dentro del sistema, se dispare de forma inmediata la acción correspondiente, sin intervención manual. En otras palabras, se establece una relación directa entre eventos y comandos, permitiendo que el sistema reaccione de forma autónoma ante situaciones previamente definidas.</p>


![Event Storming](/images/imagen_7.png)


<p>Definimos y organizamos las políticas de automatización que permiten ejecutar comandos de forma automática ante la ocurrencia de eventos clave dentro del sistema. Estas políticas cubren la recolección y envío de datos, la asignación de pulseras NFC, la validación de accesos, la generación de reportes del local, y el monitoreo de condiciones críticas como sobreaforo, humo o ruido en el recinto.
También se estructuraron reglas para el disparo automático de alertas al detectar eventos que representan infracciones, asegurando que el sistema reaccione de manera inmediata sin intervención manual.
</p>


<strong>Step 7: Read models</strong>:<br>
<p>En esta etapa, incorporamos los modelos de lectura, que representan las vistas de datos del sistema que los agentes (ya sean usuarios o componentes del sistema) utilizan para decidir si deben ejecutar un comando. Esto implica definir visualizaciones específicas como reportes de locales, paneles de monitoreo de aforo, alertas en tiempo real por infracciones, estado de las reservas, historial de asistencia y validación de acceso mediante NFC.</p>


![Event Storming](/images/imagen_7.png)







<strong>Step 8: External Systems</strong>:<br>
<p>En este paso, integramos al modelo los sistemas externos, es decir, aquellos que están fuera del dominio principal del sistema que estamos diseñando. Estos sistemas pueden intervenir ejecutando comandos hacia nuestro sistema (como entradas) o bien recibir información generada por eventos del dominio (como salidas).</p>


![Event Storming](/images/imagen_8.png)


<p>Incorporamos los sistemas externos que interactúan con el dominio principal, representados con etiquetas rojas. Se identificaron elementos clave como el lector NFC y los sensores IoT (aforo, humo, ruido), los cuales permiten recolectar datos del entorno físico y activan eventos automatizados dentro del sistema. Además, se detallaron las políticas de envío de datos, representadas en color morado, las cuales se encargan de transmitir información relevante a la nube o al backend en tiempo real.
</p>



<strong>Step 9: Aggregates</strong>:<br>
<p>Después de haber definido todos los eventos y comandos del sistema, procedemos a agrupar aquellos conceptos que guardan una relación directa dentro de unidades llamadas agregados. Estos agregados representan componentes clave del dominio, ya que son los encargados de recibir comandos y, a partir de ellos, generar los eventos correspondientes que reflejan los cambios en el estado del sistema</p>


![Event Storming](/images/imagen_9.png)


<p>Identificamos los agregados del dominio que encapsulan la lógica de negocio principal del sistema de reservas con IoT. Cada aggregate agrupa los comandos y eventos que afectan una misma unidad lógica, asegurando la coherencia de los datos y el cumplimiento de las reglas definidas. Se establecieron agregados como User, para el control de identidad y autenticación; Locale, encargado del ciclo de vida de los locales; Reservation, que gestiona las reservas y su estado; AccessControl, que regula el ingreso mediante pulseras NFC; y Monitoring, responsable de registrar condiciones detectadas por sensores IoT. Esta estructura permite organizar el dominio de forma modular y consistente, facilitando el mantenimiento y escalabilidad del sistema
</p>


<strong>Step 10: Bounded Context</strong>:<br>
<p>Finalmente, agrupamos los agregados que mantienen una relación directa entre sí, ya sea porque comparten funciones estrechamente relacionadas o porque están conectados a través de ciertas políticas de negocio. Estos conjuntos de agregados constituyen candidatos naturales para establecer los contextos delimitados (Bounded Contexts) del sistema, permitiendo organizar el dominio en módulos coherentes y bien definidos según sus responsabilidades y reglas específicas.</p>


![Event Storming](/images/imagen_10.png)



<p>En esta etapa final, estructuramos el sistema en Bounded Contexts claramente definidos, agrupando los agregados que comparten responsabilidades, reglas de negocio o interacciones comunes. Esta segmentación permite organizar el dominio en módulos independientes, cada uno con un propósito específico y una lógica coherente.
Se identificaron cinco contextos principales:
IAM (Identity and Access Management): encargado de la gestión de identidad, registro, autenticación y control de acceso de los usuarios al sistema.
Locals: responsable del registro, actualización, visualización y reporte de los locales disponibles para reserva.
Booking: gestiona todo el ciclo de vida de las reservas, incluyendo su creación, modificación, finalización y calificación posterior.
Monitoring: controla la recolección de datos desde sensores IoT (como aforo, humo o ruido), valida reglas del local y registra infracciones.
Notifications: administra el envío de alertas a usuarios o arrendadores cuando se detectan condiciones críticas o eventos relevantes.
Cada uno de estos contextos delimita claramente su modelo de datos, comandos y eventos, lo que permite mantener una arquitectura modular, trazable y preparada para escalar según las necesidades del sistema.
</p>





####4.1.1.2 Domain Message Flows Modeling



<strong>Scenario 1: Local reservation</strong>:<br>
![Event Storming](/images/imagen_11.jpeg)

<strong>Scenario 2: Local comment creation</strong>:<br>
![Event Storming](/images/imagen_12.jpeg)

<strong>Scenario 3: Tenant exceeds local capacity</strong>:<br>
![Event Storming](/images/imagen_13.jpeg)

<strong>Scenario 4: Tenant exceeds noise level</strong>:<br>
![Event Storming](/images/imagen_14.jpeg)

<strong>Scenario 5: Tenant tries to enter the premises outside of reservation hours
</strong>:<br>
![Event Storming](/images/imagen_15.jpeg)







####4.1.1.3 Bounded Context Canvases
![Event Storming](/images/imagen_16.jpeg)
![Event Storming](/images/imagen_17.jpeg)
![Event Storming](/images/imagen_18.jpeg)



###4.1.2. Context Mapping

#####1. Pasos para Crear el Context Mapping
######1.1. Identificación de los Bounded Contexts
- IAM (Identity and Access Management)
- Locals
- Booking
- Monitoring
- Notifications
######1.2. Identificación de Relaciones Iniciales
- IAM ⭤ Booking: Relación de Customer/Supplier.
- IAM proporciona la autenticación y control de acceso, mientras Booking consume la identidad para permitir la creación de reservas.
- Locals ⭤ Booking: Relación de Customer/Supplier.
- Locals administra la disponibilidad y características de los espacios, Booking consulta esa información para registrar una reserva.
- Booking ⭤ Monitoring: Relación de Customer/Supplier.
- Booking genera el inicio y fin de la reserva, mientras Monitoring supervisa el cumplimiento de normas durante ese periodo.
- Monitoring ⭤ Notifications: Relación de Conformist.
- Notifications se adapta a los eventos generados por Monitoring para emitir alertas sin modificar la estructura de los datos.
- Booking ⭤ Notifications: Relación de Conformist.
- Booking puede generar eventos que Notifications transforma en mensajes para usuarios.


#####2. Análisis de Alternativas y Preguntas Clave
######2.1. ¿Qué pasaria si movemos la gestión de reportes de locales desde Locals a Monitoring?
######Impacto:
Monitoring tendría control total del estado operacional del local.
Se perdería la separación entre información estática del local (Locals) y condiciones temporales (Monitoring).
Discusión:
No se recomienda el cambio. Mantener reportes en Locals permite independencia de la información operativa.

######2.2. ¿Y si separáramos Monitoring en dos contexts: SensorEvents y RuleValidation?
Impacto:
Permitiría escalar el procesamiento de eventos por separado del motor de reglas.
Mayor complejidad y necesidad de sincronización.
Discusión:
Podría evaluarse si los volúmenes de datos lo justifican, pero por ahora es preferible mantenerlo unificado.

######2.3. ¿Podría Notifications compartir un kernel con Booking?
Impacto:
Se podría optimizar el modelo de eventos compartidos.
Riesgo de acoplamiento excesivo.
Discusión:
Mejor mantener el contrato como evento público. No se recomienda un shared kernel.


######2.4. ¿Sería viable mover la asignación de pulseras NFC de Booking a IAM?
Impacto:
IAM controlaría identidad + dispositivo asignado.
Aumenta la carga de IAM, mezcla responsabilidades de autenticación con gestión de dispositivos.
Discusión:
Se recomienda mantener la asignación en Booking para no contaminar IAM con lógica operacional.

#####3. Alternativas Recomendadas de Context Mapping
Mantener la separación entre datos estáticos (Locals) y monitoreo operacional (Monitoring).
No dividir Monitoring aún, salvo que se presenten cuellos de botella o necesidades de escalabilidad por volumen de eventos.
Evitar compartir kernels entre contexts; priorizar integración por eventos públicos.
Mantener la asignación de dispositivos dentro de Booking.
#####4. Patrones de Relaciones Sugeridos
- Customer/Supplier: IAM ⭤ Booking, Locals ⭤ Booking, Booking ⭤ Monitoring
- Conformist: Monitoring ⭤ Notifications, Booking ⭤ Notifications
- Published Language: Monitoring publica eventos con estructura conocida para consumo externo (ej. por Notifications)
- Anti-Corruption Layer (ACL): Podría evaluarse entre Monitoring y cualquier motor externo de validación de reglas en el futuro

![Event Storming](/images/imagen_19.png)

###4.1.3. Software Architecture
####4.1.3.1. Software Architecture System Landscape Diagram

![Event Storming](/images/imagen_22.png)


####4.1.3.2. Software Architecture Context Level Diagrams

![Event Storming](/images/imagen_20.png)

####4.1.3.3. Software Architecture Container Level Diagrams

![Event Storming](/images/imagen_21.jpeg)

####4.1.3.4. Software Architecture Deployment Diagrams

![Event Storming](/images/imagen_23.png)



