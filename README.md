**Universidad Peruana de Ciencias Aplicadas**
**Ingeniería de Software**
**Ciclo 2025-10**

# Course Project

### Profesor: Marco Antonio Leon Baca
### Curso: Desarrollo de Soluciones IoT

# FINAL REPORT

## Startup: AlquilaEZ
## Propuesta: AlquilaFacil

**Team Members**

- Ames Oviedo Mariano Jose
- Avalos Santos Anthony Piero
- Lecca Choccare Christopher Bryan
- Sosa Colca Angello Rodolfo
- Carlos Oswaldo Casimiro Fernandez

**Abril 2025**

---

## Registro de Versiones 

<table>
  <thead>
    <tr>
      <th>Versión</th>
      <th>Fecha</th>
      <th>Autor</th>
      <th>Descripción de modificación</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>1era</td>
      <td>22/04/2025</td>
      <td>
        - Ames Oviedo Mariano Jose <br>
        - Avalos Santos Anthony Piero <br>
        - Lecca Choccare Christopher Bryan <br>
        - Sosa Colca Angello Rodolfo <br>
        - Carlos Oswaldo Casimiro Fernandez <br>
      </td>
      <td>Se creo la ramificacion del repositorio. Se concluyo con los capitulos 1, 2, 3 y 4, realizando la presentacion respectiva de la documentacion. Tambien se realizo el video donde cada miembro del equipo expone ciertas partes del trabajo</td>
   </tr>
</table>

## Contenido

**Tabla de contenidos**

| Tabla de contenidos                                                                                                 |
| ------------------------------------------------------------------------------------------------------------------- |
| [Capítulo I: Introducción](#capítulo-i-introducción)                                                                |
| [1.1. Startup Profile](#11-startup-profile)                                                                         |
| [1.1.1. Descripción de la Startup](#111-descripción-de-la-startup)                                                  |
| [1.1.2. Perfiles de integrantes del equipo](#112-perfiles-de-integrantes-del-equipo)                                |
| [1.2. Solution Profile](#12-solution-profile)                                                                       |
| [1.2.1 Antecedentes y problemática](#121-antecedentes-y-problemática)                                               |
| [1.2.2. Lean UX Process](#122-lean-ux-process)                                                                      |
| [1.2.2.1. Lean UX Problem Statements](#1221-lean-ux-problem-statements)                                             |
| [1.2.2.2. Lean UX Assumptions](#1222-lean-ux-assumptions)                                                           |
| [1.2.2.3. Lean UX Hypothesis Statements](#1223-lean-ux-hypothesis-statements)                                       |
| [1.2.2.4. Lean UX Canvas](#1224-lean-ux-canvas)                                                                     |
| [1.3. Segmentos objetivo](#13-segmentos-objetivo)                                                                   |
| [Capítulo II: Requirements Elicitation & Analysis](#capítulo-ii-requirements-elicitation--analysis)                 |
| [2.1. Competidores](#21-competidores)                                                                               |
| [2.1.1. Análisis competitivo](#211-análisis-competitivo)                                                            |
| [2.1.2. Estrategias y tácticas frente a competidores](#212-estrategias-y-tácticas-frente-a-competidores)            |
| [2.2. Entrevistas](#22-entrevistas)                                                                                 |
| [2.2.1. Diseño de entrevistas](#221-diseño-de-entrevistas)                                                          |
| [2.2.2. Registro de entrevistas](#222-registro-de-entrevistas)                                                      |
| [2.2.3. Análisis de entrevistas](#223-análisis-de-entrevistas)                                                      |
| [2.3. Needfinding](#23-needfinding)                                                                                 |
| [2.3.1. User Personas](#231-user-personas)                                                                          |
| [2.3.2. User Task Matrix](#232-user-task-matrix)                                                                    |
| [2.3.3. User Journey Mapping](#233-user-journey-mapping)                                                            |
| [2.3.4. Empathy Mapping](#234-empathy-mapping)                                                                      |
| [2.3.5. As-is Scenario Mapping](#235-as-is-scenario-mapping)                                                        |
| [2.4. Ubiquitous Language](#24-ubiquitous-language)  
| [Capítulo III: Requirements Specification](#capítulo-iii-requirements-specification)                                |
| [3.1. To-Be Scenario Mapping](#31-to-be-scenario-mapping)                                                           |
| [3.2. User Stories](#32-user-stories)                                                                               |
| [3.3. Impact Mapping](#33-impact-mapping)                                                                           |
| [3.4. Product Backlog](#34-product-backlog)     
| [Capítulo IV: Solution Software Design](#capítulo-iv-product-design)                                                          |
| [4.1. Strategic-Level Domain-Driven Design](#41-strategic-level-domain-driven-design)                               |
| [4.1.1. Event Storming](#411-event-storming) |
| [4.1.1.1 Candidate Context Discovery](#4111-candidate-context-discovery) |
| [4.1.1.2 Domain Message Flows Modeling](#4112-domain-message-flows-modeling) |
| [4.1.1.3 Bounded Context Canvases](#4113-bounded-context-canvases) |
| [4.1.2. Context Mapping](#412-context-mapping) |
| [4.1.3. Software Architecture](#413-software-architecture) |
| [4.1.3.1. Software Architecture System Landscape Diagram](#4131-software-architecture-system-landscape-diagram) |
| [4.1.3.2. Software Architecture Context Level Diagrams](#4132-software-architecture-context-level-diagrams) |
| [4.1.3.3. Software Architecture Container Level Diagrams](#4133-software-architecture-container-level-diagrams) |
| [4.1.3.4. Software Architecture Deployment Diagrams](#4134-software-architecture-deployment-diagrams) |
| [4.2. Tactical-Level Domain-Driven Design](#42-tactical-level-domain-driven-design) |
| [4.2.1. Bounded Context: <Bounded Context Name>](#421-bounded-context-bounded-context-name) |
| [4.2.1.1. Domain Layer](#4211-domain-layer) |
| [4.2.1.2. Interface Layer](#4212-interface-layer) |
| [4.2.1.3. Application Layer](#4213-application-layer) |
| [4.2.1.4. Infrastructure Layer](#4214-infrastructure-layer) |
| [4.2.1.5. Bounded Context Software Architecture Component Level Diagrams](#4215-bounded-context-software-architecture-component-level-diagrams) |
| [4.2.1.6. Bounded Context Software Architecture Code Level Diagrams](#4216-bounded-context-software-architecture-code-level-diagrams) |
| [4.2.1.6.1. Bounded Context Domain Layer Class Diagrams](#42161-bounded-context-domain-layer-class-diagrams) |
| [4.2.1.6.2. Bounded Context Database Design Diagram](#42162-bounded-context-database-design-diagram) |

 


# Student Outcome

**ABET – EAC – Student Outcome 5**
Criterio: La capacidad de funcionar efectivamente en un equipo cuyos miembros
juntos proporcionan liderazgo, crean un entorno de colaboración e inclusivo,
establecen objetivos, planifican tareas y cumplen objetivos

En el siguiente cuadro se describe las acciones realizadas y enunciados de
conclusiones por parte del grupo, que permiten sustentar el haber alcanzado el logro
del ABET – EAC - Student Outcome 5.

<table border="1" cellspacing="0" cellpadding="8">
  <thead>
    <tr>
      <th><strong>Criterio específico</strong></th>
      <th><strong>Acciones realizadas</strong></th>
      <th><strong>Conclusiones</strong></th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>Trabaja en equipo para proporcionar liderazgo en forma conjunta.</td>
      <td>
        <strong>Christopher Bryan Lecca Choccare (TB1):</strong> Me encargué de liderar el diseño estratégico, guiando al equipo en la identificación de bounded contexts y en la elaboración del Event Storming y Context Mapping. Coordiné la conexión lógica entre eventos y políticas, y aseguré la consistencia general en los flujos del sistema.<br><br>
        <strong>Angello Rodolfo Sosa Colca (TB1):</strong> Lideré el diseño táctico del contexto "Locals", definiendo sus capas y componentes. Me aseguré de que la estructura entre entidades, comandos, servicios y repositorios fuera coherente y alineada con los principios de DDD.<br><br>
        <strong>Anthony Piero Avalos Santos (TB1):</strong> Participé activamente en la fase de descubrimiento del usuario. Me enfoqué en aplicar técnicas como Empathy Mapping, User Personas y User Journey para captar de manera precisa las necesidades reales y plasmarlas en el sistema.<br><br>
        <strong>Mariano José Ames Oviedo (TB1):</strong> Me encargué de elaborar la introducción de la solución, definiendo el perfil de la startup, los desafíos que busca resolver y su aporte a la sostenibilidad urbana. También consolidé los antecedentes para contextualizar el problema.<br><br>
        <strong>Carlos Oswaldo Casimiro Fernández (TB1):</strong> Me responsabilicé por la implementación de la capa de infraestructura del contexto, construyendo los repositorios, asegurando persistencia adecuada y validando integraciones con bases de datos.
      </td>
      <td>
        El equipo demostró una colaboración efectiva al asumir roles estratégicos que permitieron el avance fluido del proyecto. Cada miembro aportó liderazgo desde sus fortalezas, logrando construir una solución bien estructurada a través de trabajo conjunto y comunicación constante.
      </td>
    </tr>
    <tr>
      <td>Comunica en forma escrita ideas y/o resultados con objetividad a público de diferentes especialidades y niveles jerárquicos.</td>
      <td>
        <strong>Mariano José Ames Oviedo (TB1):</strong> Me encargué de redactar las secciones introductorias del entregable, comunicando los objetivos y fundamentos del sistema de forma clara para cualquier lector.<br><br>
        <strong>Anthony Piero Avalos Santos (TB1):</strong> Redacté resultados del análisis de usuarios, presentando mapas y perfiles de forma comprensible para distintos perfiles técnicos y no técnicos.<br><br>
        <strong>Christopher Bryan Lecca Choccare (TB1):</strong> Elaboré la descripción del diseño estratégico, cuidando que el lenguaje técnico pudiera ser entendido también por miembros no especializados del equipo.<br><br>
        <strong>Angello Rodolfo Sosa Colca (TB1):</strong> Documenté los diagramas tácticos y estructuras de clases, asegurando una redacción técnica precisa pero accesible para otros desarrolladores o evaluadores.<br><br>
        <strong>Carlos Oswaldo Casimiro Fernández (TB1):</strong> Expliqué el funcionamiento de los repositorios en lenguaje claro y estructurado, facilitando la revisión y el entendimiento por parte de terceros.
      </td>
      <td>
        Se logró una comunicación escrita efectiva a lo largo del entregable, permitiendo que las ideas fueran comprendidas por distintas audiencias. El uso claro del lenguaje, apoyado por gráficos y ejemplos, facilitó la transmisión de resultados y decisiones de diseño.
      </td>
    </tr>
  </tbody>
</table>


# Capítulo I: Introducción

## 1.1. Startup Profile

### 1.1.1 Descripción de la Startup

AlquilaFácil es un startup fundado en el 2025, por un grupo de estudiantes de la carrera de Ingeniería de Software de la Universidad Peruana de Ciencias Aplicadas (UPC). Nuestra empresa emergente se enfoca en la simplificación del proceso de búsqueda de alquiler de espacios para eventos, así como la administración de los mismos.

**Misión:** Revolucionar el alquiler de espacios para eventos con una plataforma intuitiva que une a arrendadores y arrendatarios de manera rápida y sencilla. 

**Visión:** Consolidarnos como la referencia global en alquiler de espacios para eventos, redefiniendo el sector con soluciones inteligentes y una experiencia excepcional.

### 1.1.2 Perfiles de integrantes del equipo

|<!-- -->|<!-- -->|
|--------|--------|
|Nombre|Ames Oviedo, Mariano José (U202211371)|
|Soy Mariano, tengo 19 años actualmente curso mi 6to ciclo de la carrera de Ingeniería de Software. Me considero una persona responsable y dispuesta a afrontar desafíos. Considero que estas cualidades beneficiaran a mi equipo para poder completar un trabajo de calidad.||
|Nombre|Avalos Santos, Anthony Piero (U20211C596)|
| Soy Anthony Avalos, tengo 21 años, actualmente me encuentro en el 9no ciclo de mi carrera de Ingeniería de Software. Soy un apasionado por el desarrollo Fullstack, me considero una persona super proactiva y con ganas de seguir aprendiendo una nueva tecnología emergente. Me gusta el trabajo en equipo y colaborar con grande profesionales |
|Nombre|Lecca Choccare, Christopher Bryan (U202211399)|
|Mi nombre es Christopher, tengo 20 años y actualmente me encuentro cursando el 7mo ciclo de la carrera de Ingeniería de Software en la Universidad Peruana de Ciencias Aplicadas (UPC). Considero que mi compromiso con el equipo de trabajo designado y mi capacidad de aprendizaje rápida aportarán de buena manera al desarrollo del producto final.|
|Nombre|Sosa Colca, Angello Rodolfo (U202212077)|
|Tengo 19 años y curso el 7mo ciclo de la carrera de Ingeniería de Software en la Universidad Peruana de Ciencias Aplicadas. Soy una persona enfocada, perseverante y colaborativo. Estas cualidades me permiten ser una persona que ayudará de manera óptima el requisito que se me imponga. Además, soy una persona que apoya cuando los demás se encuentran en problemas.|
|Nombre|Carlos Oswaldo Casimiro Fernandez (U202115412)|
| Tengo 21 años y soy estudiante de Ingeniería de Software de la Universidad Peruana de Ciencias Aplicadas. Me considero una persona proactiva, educada y sociable con los que me rodean. Además, cuento con habilidades peculiares como la animación en 3D, edición de videos cinematográficos y conocimiento en lenguajes como C++, Python. |

## 1.2. Solution Profile

En esta sección se detallan los aspectos claves de nuestra solución de software, incluyendo sus características distintivas y propuestas de valor. 

**Product Name:** AlquilaFácil

**Producto Descriptivo:** AlquilaFácil es una plataforma diseñada para simplificar el proceso de búsqueda y reserva de espacios para eventos, conectando de manera eficiente a arrendadores y arrendatarios. Ofrece una experiencia fluida, permitiendo a los usuarios buscar, reservar y gestionar espacios para una amplia variedad de eventos. Además, la plataforma incluye herramientas de gestión y seguimiento en tiempo real, asegurando una experiencia optimizada tanto para arrendadores como para arrendatarios. 

**Monetización:** AlquilaFácil generará ingresos a través de un modelo de suscripción para arrendadores que deseen destacar sus propiedades y acceder a herramientas avanzadas de gestión de reservas. Estos planes premium ofrecerán beneficios adicionales, como una mayor visibilidad en los resultados de búsqueda y acceso prioritario a herramientas analíticas avanzadas. Además, monetizaremos la plataforma mediante la implementación de sensores en los locales, permitiendo a los propietarios recibir reportes detallados sobre la actividad en sus espacios. En contraste, el acceso a la plataforma será completamente gratuito para los arrendatarios, incentivando su participación y aumentando la oferta de espacios disponibles.

### 1.2.1. Antecedentes y Problematicas

Actualmente, las personas tienen fácil acceso a herramientas tecnológicas para reservar y alquilar locales de eventos, en páginas web o mediante un aplicativo móvil. Esto genera una mayor demanda en nuestro país sobre el creciente mercado de las reservas online. Además, con el incremento de usuarios que tienen acceso a internet, uso de dispositivos para facilitar el proceso de reserva espacios para eventos. Según el INEI, en los primeros tres meses del año 2022, 73 de cada 100 personas de 6 y más años accedieron a Internet en el país, cifra que muestra un crecimiento de 5,1 y 17,7 puntos porcentuales comparado con igual trimestre de 2021 (67,4%) y 2019 (54,8%), respectivamente (Jasin, 2023). 

También es importante mencionar la creciente demanda por la elaboración de eventos por parte de las marcas. Según Mañas (2024), las marcas apuestan cada vez más por los eventos para darse a conocer e interactuar directamente con su audiencia, pues muchas consideran que estas experiencias ayudan a mostrar sus valores y a construir relaciones sólidas con sus clientes. 

Ante ello, podemos demostrar que en el Perú el número de personas con acceso a internet a incrementado considerablemente en los últimos dos años, por otro lado, también justificamos la necesidad de una plataforma para facilitar la búsqueda en alquiler de espacios ante la creciente demanda de estas por parte de las empresas.



**Problemáticas - Técnica de las 5 'W's y 2 'H's**

**What?**

**¿Cuál es el problema?**

El problema es la falta de una plataforma centralizada y enfocada en el alquiler de espacios para eventos. Actualmente, arrendadores y arrendatarios enfrentan dificultades al buscar y reservar espacios adecuados para sus necesidades. 

**¿Cuál es la relación con la persona en cuestión?**

La persona en cuestión es que, si es arrendador de un espacio para eventos, puede enfrentar dificultades al encontrar y atraer a potenciales clientes para alquilar su espacio. Del mismo modo, si es arrendatario, puede enfrentar desafíos al buscar y reservar un espacio adecuado para sus eventos.	 

**When?**

**¿Cuánto sucede el problema?** 

El problema ocurre cada vez que arrendadores desean alquilar sus instalaciones para eventos o arrendatarios buscan espacios para celebrar sus actividades. Esta necesidad surge de manera recurrente y en diferentes momentos, ya sea para eventos planificados con anticipación o para aquellos que requieran una búsqueda rápida de un espacio disponible. 

**¿Cuándo utiliza el cliente el producto?** 

Cuando organizaciones o personas necesitan encontrar y reservar un espacio para un evento, ya sea con anticipación o de manera urgente. También, para aquellas personas que poseen instalaciones para realizar eventos y deseen promocionar su espacio, conectándose así con clientes potenciales. 

**Where?** 
**¿Dónde está el cliente cuando usa el producto?**

El cliente utiliza AlquilaFácil a través de su aplicación móvil. 

 
**¿A dónde se dirige?** 

Se dirige a una plataforma en línea o a una aplicación móvil, donde puede buscar, comparar y reservar espacios para eventos de manera conveniente y eficiente. 

**¿Dónde surge el problema?** 

El problema surge en la dificultad para encontrar y reservar espacios adecuados para eventos, ya sea durante la planificación anticipada de un evento o en situaciones donde se requiere una búsqueda rápida. 

**Why?**

**¿Cuál es la causa del problema?**

La falta de una plataforma centralizada y eficiente que conecte a arrendadores con personas que buscan alquilar un espacio para eventos. La ausencia de un sistema unificado dificulta la búsqueda y reserva de espacios adecuados, lo que puede generar frustración y pérdida de oportunidades tanto para arrendadores como para arrendatarios. 

**How?** 

**¿En qué condiciones los clientes usan nuestro producto?** 

Los clientes utilizan AlquilaFácil para buscar y reservar espacios para una variedad de eventos, ya sea para eventos sociales o corporativos. 

**¿Cómo prefieren los clientes acceder a nuestro producto?**

Los clientes prefieren acceder a nuestro producto, a través de una plataforma web o móvil. 

**¿Que llevó al cliente a llegar a esta situación?**

La falta de una plataforma para el alquiler de espacios para eventos llevó tanto a los clientes que buscan espacios como a los arrendadores a esta situación. 

 
**How much?** 

Los costos de AlquilaFácil varían según el plan de suscripción seleccionada. Ofrecemos opciones gratuitas para los usuarios básicos, así como planes de suscripción mensual o anual con tarifas moderadas para aquellos que deseen optar por un plan premium y beneficios adicionales. 

### 1.2.2. Lean UX Process

En esta parte, llevaremos a cabo el proceso de Lean UX, que abarca la visión del modelo de negocio que respaldará nuestro producto de software. Este enfoque metodológico nos permite concentrarnos en el diseño de nuestra solución y en la resolución de los problemas identificados a través del pensamiento de diseño. 

#### 1.2.2.1. Lean UX Problem Statement

Nuestro contexto se enmarca en el mercado de alquiler de espacios para eventos en Perú, un sector que ha experimentado un crecimiento sostenido en los últimos años. Con el aumento de la demanda por espacios flexibles y adaptables para diferentes tipos de eventos, también surgen desafíos en la manera en que los usuarios, tanto arrendadores como arrendatarios, interactúan dentro de este ecosistema. 

Hemos identificado que, en el mercado de alquiler de espacios, los usuarios enfrentan dificultades por la falta de integración en el proceso. La fragmentación en la búsqueda, gestión de reservas y organización genera ineficiencias y una experiencia insatisfactoria. 

¿Cómo podemos mejorar la conexión entre arrendadores y arrendatarios, optimizando el proceso de alquiler de espacios para eventos y ofreciendo una experiencia más fluida y eficiente?

#### 1.2.2.2. Lean UX Assumptions



**Business Outcomes:** 

- Asegurar que la plataforma procese al menos 1,000 reservas de eventos en el primer año, optimizando la gestión y la comunicación entre arrendadores y arrendatarios. 

- Lograr una tasa de satisfacción del usuario del 90% o más mediante la implementación de herramientas que permitan verificar clasificaciones e historial de espacios, ayudando a los arrendatarios a tomar decisiones informadas.  

- Renovación de suscripciones del 80% al final del primer año, indicando la satisfacción y la retención de clientes. 

 

**User Assumptions:**

- ¿Quién es el usuario?

  - Arrendatarios 

  - Arrendadores 

- ¿Dónde entra nuestro producto en su trabajo o su vida? 

  - **Arrendatarios:** AlquilaFácil simplifica la búsqueda y reserva de espacios, optimizando la planificación de eventos y ahorrando tiempo y esfuerzo. 

  - **Arrendadores:** AlquilaFácil facilita la promoción y gestión eficiente de sus espacios, aumentando su visibilidad y el número de reservas. 

<br>

- ¿Cuál es el problema que nuestro producto soluciona? 

  - Comunicación ineficiente entre arrendatarios y arrendadores. 

  - Dificultad para encontrar y reservar espacios adecuados. 

  - Falta de transparencia y confianza en la calidad y disponibilidad de los espacios. 

  - Necesidad de una herramienta centralizada para gestionar reservas y promover espacios. 

<br>

- ¿Cómo y cuándo nuestro producto es usado? 

  - **Arrendatarios:** Usan la plataforma para buscar, filtrar y reservar espacios para sus eventos, tanto durante la planificación como en la fase de ejecución. 

  - **Arrendadores:** Usan la plataforma para promocionar sus espacios y gestionar reservas. 

 <br>

- ¿Qué características son importantes? 

  - Interfaz intuitiva y fácil de usar para búsqueda y reserva de espacios. 

  - Sistema de promoción y visibilidad para los espacios. 

  - Herramientas para gestionar reservas y comunicarse eficientemente. 

  - Acceso a clasificaciones y reseñas para tomar decisiones informadas. 

 <br>

- **User Outcomes:** 

  - Los arrendatarios de eventos lograrán una reducción del 20% en el tiempo promedio dedicado a la búsqueda y reserva de espacios para eventos dentro de los primeros seis meses de uso de la plataforma. 

 

  - Los arrendadores de espacios aumentarán en un 25% el número de reservas y consultas recibidas en sus espacios durante el primer año de implementación de la plataforma. 

 

  - Los arrendatarios de eventos experimentarán una mejora del 30% en la satisfacción con la calidad y adecuación de los espacios reservados, medida a través de reseñas y calificaciones en la plataforma durante el primer año. 


#### 1.2.2.3. Lean UX Hypothesis Statements

Para la elaboración de los Hypothesis Statements se utilizó el formato Lean UX: [We believe that], [This will achieve] y [We will have demostrated this when] 

**Hipótesis 1**

Creemos que, al simplificar el proceso de búsqueda y comparación de espacios para eventos en nuestra plataforma, aumentaremos la cantidad de clientes recurrentes. 

Sabremos que estamos en lo correcto cuando observemos un incremento en la cantidad de reservas realizadas por clientes recurrentes, proyectando un aumento del 25% dentro de los primeros seis meses de la implementación de esta mejora. 

<br>
 
**Hipótesis 2** 

Creemos que, al mejorar la función de búsqueda avanzada en nuestra plataforma, permitiendo a los usuarios filtrar por características específicas de los espacios (como capacidad, ubicación y servicios incluidos), aumentaremos la satisfacción del usuario y mejoraremos la precisión en la selección de espacios. 

Sabremos que estamos en lo correcto cuando observemos una disminución del 25% en las consultas de soporte relacionadas con la búsqueda de espacios y un aumento en el tiempo promedio que los usuarios pasan en la plataforma explorando opciones. 

<br>

**Hipótesis 3**

Creemos que, al ofrecer descuentos exclusivos en tarifas de alquiler de espacios seleccionados para los usuarios con suscripción premium, lograremos aumentar la conversión de usuarios de planes básicos a planes premium. 

Sabremos que estamos en lo correcto cuando observemos un aumento del 30% en la cantidad de usuarios que actualizan su suscripción a premium y un incremento en el volumen de reservas realizadas por estos usuarios, dentro de los primeros seis meses de la implementación de esta estrategia. 

<br>

**Hipótesis 4**

Creemos que, al implementar un sistema de calificación y comentarios para los espacios disponibles en nuestra plataforma, aumentaremos la confianza de los usuarios y mejoraremos la percepción de calidad de los espacios, lo que impulsará un mayor número de reservas. 

Sabremos que estamos en lo correcto cuando observemos un aumento del 20% en la cantidad de reservas completadas, junto con una mejora en las calificaciones y comentarios proporcionados por los usuarios, dentro de los primeros tres meses de la implementación.

<br>

**Hipótesis 5**

Creemos que, al implementar un programa de referidos que recompense a los usuarios por traer nuevos arrendadores o arrendatarios a nuestra plataforma, aumentaremos la adquisición de usuarios y fomentaremos el crecimiento orgánico de nuestra base de clientes. 

Sabremos que estamos en lo correcto cuando observemos un aumento del 35% en la cantidad de nuevos registros y un incremento en el número de referidos realizados por los usuarios existentes, dentro de los primeros tres meses de implementación del programa. 

#### 1.2.2.4. Lean UX Canvas



## 1.3. Segmentos objetivo

En esta sección, identificamos los segmentos de clientes específicos a los que se dirige AlquilaFácil, basándonos en características demográficas, comportamientos y necesidades compartidas. 

**Arrendatarios:** 

- Descripción: Individuos que planifican eventos sociales como bodas, fiestas de cumpleaños, reuniones familiares, entre otros, y aquellos que organizan eventos regularmente, ya sea social o corporativo. 

- Características: Buscan espacios que se adapten a sus necesidades específicas, como capacidad, ubicación y servicios disponibles. Realizan múltiples reservas de espacios a lo largo del año. 

- Necesidades: Facilidad de búsqueda y reserva de espacios, acceso a información detallada sobre las instalaciones y servicios ofrecidos, programas de fidelización y alertas de acontecimientos que puedan afectar el desarrollo de su evento. 

**Arrendadores:**

- Descripción: Individuos o empresas que poseen espacios aptos para eventos, como salones de banquetes, jardines, locales comerciales, etc. 

- Características: Ofrecen una variedad de espacios con diferentes capacidades y servicios. 

- Necesidades: Promoción efectiva de sus espacios, gestión eficiente de reservas, acceso a herramientas para administrar sus listados y proyectos de eventos. 


