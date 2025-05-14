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

## Project Report Collaboration Insights

<p>URL del repositorio: https://github.com/AlquilaEZ/alquilafacil-document-report</p>

<strong>TB1</strong> 

<p> El equipo participó de forma activa en el repositorio de GitHub, registrando un total de 74 commits durante el desarrollo del primer entregable del informe.</p>

![image]( /images/collaborator_TB1.png)


<p> El trabajo con ramas paralelas permitió que los integrantes del equipo avanzaran en distintas secciones del informe de forma simultánea, integrando sus cambios de manera ágil y minimizando conflictos. Esta estrategia colaborativa aseguró una participación equilibrada de todos los miembros en la construcción del entregable.</p>

![image]( /images/network_TB1.png)
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

# Capítulo II: Requirements Elicitation & Analysis

## 2.1. Competidores

<div align="justify">

Después de realizar una investigación de mercado, hemos identificado tres plataformas que ofrecen características similares a las de nuestra aplicación para conectar arrendadores con arrendatarios de eventos. Estas son: 
</div>

**Competidores:**

<div align="justify">

* ***Airbnb:***
  Es una plataforma en línea fundada en 2008 que revolucionó la industria hotelera al ofrecer una alternativa a los hoteles tradicionales. Permite a los usuarios alquilar alojamientos a corto plazo, desde habitaciones individuales hasta casas completas, en más de 191 países. Facilita la conexión entre anfitriones que desean alquilar sus propiedades y huéspedes en busca de alojamiento temporal.  

</div>

  ![Imagen extraída de Airbnb([URL]())](images/competitors/Airbnb.png)

<br>
<div align="justify">

* ***Vrbo:***
   Es una plataforma en línea fundada en 1995 que facilita el alquiler de alojamientos vacacionales directamente a través de los propietarios. El nombre significa "Vacation Rentals by Owner" (Alquileres Vacacionales por Propietario). Es uno de los principales sitios web para alquileres vacacionales en todo el mundo, donde los usuarios pueden buscar y reservar casas, apartamentos, cabañas y villas en una variedad de destinos. Esto les permite encontrar opciones que se adapten a sus necesidades y preferencias. 

</div>

  ![Imagen extraída de Vrbo([URL]())](images/competitors/Vrbo.png)
<br><br>
<div align="justify">

* ***Booking:***
 Es una plataforma que permite a los usuarios reservar alojamiento en hoteles, hostales, apartamentos y otros tipos de alojamiento en todo el mundo. También ofrece la posibilidad de reservar vuelos, alquilar coches y reservar actividades turísticas. Booking.com es una de las mayores plataformas de reserva de alojamiento en línea y ofrece una amplia variedad de opciones para viajeros de todo tipo. Los usuarios pueden buscar alojamientos según sus preferencias y presupuesto, y realizar reservas de manera rápida y conveniente a través de la plataforma. 

</div>

  ![Imagen extraída de Booking([URL]())](images/competitors/Booking.png)

<br>

### 2.1.1. Análisis competitivo

<table>
    <thead>
        <tr>
            <th colspan="6">Competitive Analysis Landscape</th>
        </tr>
        <tr>
            <th colspan="6">Escriba en el recuadro la pregunta que busca responder o el objetivo de este análisis.</th>
        </tr>
        <tr>
            <th colspan="6">Este análisis se realizó con la finalidad de poder identificar a nuestros potenciales competidores e idear estrategias y tácticas para diferenciarnos de estos.</th>
        </tr>
        <tr>
            <th colspan="2"></th>
            <th>AlquilaFácil</th>
            <th>Airbnb</th>
            <th>Vrbo</th>
            <th>Booking.com</th>
        </tr>
    </thead>
    <tbody>
        <tr>
            <td rowspan="2" align="center">Perfil</td>
            <td align="center">Overview</td>
            <td align="center">Es una plataforma en línea que facilita el alquiler de una amplia gama de espacios para eventos, desde salones de eventos hasta casas y alojamientos temporales. Con una interfaz fácil de usar, conecta a arrendadores con arrendatarios, ofreciendo una solución conveniente y eficiente para satisfacer las necesidades de ambos. Asimismo, presenta una interfaz para poder recibir reportes de eventos ocurridos en el local.</td>
            <td align="center">Plataforma en línea que revoluciona el alquiler de alojamientos a corto plazo, conectando anfitriones y huéspedes en todo el mundo. Ofrece una amplia variedad de opciones de alojamiento, desde habitaciones individuales hasta casas completas.</td>
            <td align="center">Plataforma en línea que permite a los usuarios buscar y reservar alojamientos vacacionales directamente a través de arrendadores. Ofrece una variedad de opciones de alojamiento, como casas, apartamentos, cabañas y villas, en diferentes destinos, adaptándose a las necesidades y preferencias de los viajeros.</td>
            <td align="center">Booking.com es una plataforma líder para reservar alojamiento y actividades turísticas en todo el mundo. Ofrece una amplia variedad de opciones, desde hoteles hasta apartamentos, y facilita la búsqueda y reserva según las preferencias y presupuesto de los usuarios.</td>
        </tr>
        <tr>
            <td align="center">Ventaja competitiva ¿Qué valor ofrece a los clientes?</td>
            <td align="center">Proporciona una solución completa para la planificación de eventos, ofreciendo una amplia gama de espacios para eventos y una plataforma intuitiva para gestionar reservas y espacios. Con características como registro gratuito de espacios, búsqueda avanzada y servicio al cliente dedicado, ArrendaFácil simplifica el proceso de planificación de eventos para arrendatarios y arrendadores.</td>
            <td align="center">Ofrece una amplia variedad de alojamientos en todo el mundo, desde habitaciones individuales hasta casas completas, junto con experiencias locales únicas organizadas por anfitriones. Esto permite a los viajeros personalizar su experiencia y sumergirse en la cultura local.	</td>
            <td align="center">Se especializa en alquileres vacacionales directamente a través de arrendadores, brindando a los viajeros la oportunidad de disfrutar de una experiencia más auténtica y personalizada. Con una amplia selección de alojamientos vacacionales, Vrbo ofrece opciones para todos los gustos y presupuestos.</td>
            <td align="center">Destaca por su amplia oferta de alojamiento y servicios, que incluyen hoteles, vuelos, alquiler de coches y actividades turísticas. La plataforma fácil de usar permite a los usuarios encontrar y reservar alojamiento de manera rápida y sencilla, ofreciendo una solución integral para los viajeros.</td>
        </tr>
        <tr>
            <td rowspan="5" align="center">Perfil de Marketing</td>
            <td align="center">Mercado Objetivo</td>
            <td align="center">Dirigido a arrendatarios adultos de 18 años en adelante que buscan espacios para eventos sociales, corporativos o especiales, como bodas, conferencias, fiestas de empresa, entre otros. Además, atrae a empresas y organizaciones que buscan espacios para eventos corporativos y reuniones profesionales dirigidas a un público adulto.</td>
            <td align="center">Se centra en viajeros adultos de 18 años en adelante, ofreciendo una amplia variedad de alojamientos en todo el mundo, desde habitaciones individuales hasta casas completas, para adaptarse a diferentes necesidades y preferencias de viaje. Además, apunta a grupos de amigos, parejas y familias adultas que buscan opciones de alojamiento que se ajusten a sus requerimientos y presupuestos durante sus vacaciones o escapadas.</td>
            <td align="center">Está dirigido a familias y grupos de amigos adultos de 18 años en adelante que buscan alquilar casas, villas o cabañas para vacaciones o escapadas grupales. Además, atrae a parejas y grupos de amigos adultos que buscan alquilar alojamientos vacacionales para eventos especiales, como bodas, reuniones familiares o celebraciones de cumpleaños.</td>
            <td align="center">Orientado a viajeros adultos de 18 años en adelante, busca ofrecer una amplia gama de opciones de alojamiento para adaptarse a diversas necesidades y preferencias durante sus viajes. También se dirige a personas que viajan por negocios, parejas en escapadas románticas, grupos de amigos en vacaciones y familias en busca de opciones de alojamiento cómodas y convenientes.</td>
        </tr>
        <tr>
            <td align="center">Estrategias de Marketing</td>
            <td align="center">ArrendaFácil destaca con marketing de contenidos, participación en eventos de la industria y alianzas con proveedores de servicios de eventos para ofrecer soluciones completas a arrendatarios.</td>
            <td align="center">Airbnb emplea campañas publicitarias en redes sociales y colaboraciones con influencers para promocionar destinos y experiencias únicas. También utiliza programas de referidos para aumentar su base de usuarios.</td>
            <td align="center">Vrbo se centra en contenido educativo en su sitio web, colaboraciones con agencias de viajes y ofertas exclusivas para atraer a familias y grupos de amigos a reservar a través de su plataforma.</td>
            <td align="center">Booking.com utiliza estrategias de SEO y SEM, junto con programas de fidelización, para atraer tráfico y fomentar la lealtad del cliente a través de una experiencia personalizada.</td>
        </tr>
        <tr>
            <td align="center">Productos & servicios</td>
            <td align="center">Aplicación web que conecta a arrendadores de diversos espacios, como salones de eventos, jardines y locales comerciales, con arrendatarios que buscan alquilar estos espacios para celebrar eventos sociales, corporativos o especiales. Proporciona una variedad de herramientas y servicios para facilitar la búsqueda, reserva y gestión de espacios para eventos.</td>
            <td align="center">Plataforma en línea donde los usuarios pueden alquilar una variedad de alojamientos a corto plazo, desde habitaciones individuales hasta casas completas, en todo el mundo. Además de alojamiento, Airbnb también proporciona experiencias locales únicas organizadas por anfitriones, como recorridos gastronómicos, clases de cocina y excursiones.	</td>
            <td align="center">Plataforma para alquilar alojamientos vacacionales directamente a través de los arrendadores. Los usuarios pueden encontrar y reservar una amplia gama de propiedades, que van desde casas y apartamentos hasta cabañas y villas, para sus vacaciones o escapadas en todo el mundo.</td>
            <td align="center">Plataforma en línea que permite a los usuarios reservar una variedad de alojamientos, incluyendo hoteles, hostales, apartamentos y otros tipos de hospedaje en todo el mundo. Además de alojamiento, Booking.com ofrece la posibilidad de reservar vuelos, alquilar coches y reservar actividades turísticas para completar la experiencia de viaje del usuario.</td>
        </tr>
        <tr>
            <td align="center">Precios & Costos</td>
            <td align="center">Los precios de ArrendaFácil varían dependiendo del lugar, el tamaño de la propiedad, servicios, y el tiempo de uso.</td>
            <td align="center">El costo promedio puede variar significativamente dependiendo de varios factores, como la ubicación, el tipo de alojamiento, la época del año y la demanda local.</td>
            <td align="center">Los precios en VRBO pueden variar significativamente dependiendo de la ubicación, el tamaño de la propiedad, las comodidades ofrecidas y la temporada del año.</td>
            <td align="center">Los precios pueden variar significativamente según la ubicación, la temporada, la demanda y el tipo de alojamiento.</td>
        </tr>
        <tr>
            <td align="center">Canales de distribución (Web y/o móvil)</td>
            <td align="center">Redes sociales y aplicación web donde los usuarios pueden poner en renta su espacio o alquilar un espacio para eventos.</td>
            <td align="center">Sitio web de Airbnb, aplicación móvil de Airbnb, socios afiliados y asociaciones, redes sociales y marketing digital.</td>
            <td align="center">Principalmente su sitio web y su aplicación móvil, así como acuerdos de distribución con otros sitios web de viajes o agencias de viajes en línea.</td>
            <td align="center">Sitio web de Booking.com, aplicación móvil de Booking, agencias de viajes en línea, alianzas con compañías de viajes, afiliados y asociados.</td>
        </tr>
        <tr>
            <td rowspan="4" align="center">Análisis SWOT</td>
            <td align="center">Fortalezas</td>
            <td align="center">Solución completa para la planificación de eventos.</td>
            <td align="center">Gran comunidad de anfitriones y usuarios.</td>
            <td align="center">Variedad de alojamientos en todo el mundo.</td>
            <td align="center">Interfaz fácil de usar y experiencia intuitiva del usuario.</td>
        </tr>
        <tr>
            <td align="center">Debilidades</td>
            <td align="center">Dependencia de la disponibilidad de espacios para eventos.</td>
            <td align="center">Dependencia de la reputación y opiniones de los usuarios.</td>
            <td align="center">Posible saturación del mercado de alquiler vacacional.</td>
            <td align="center">Competencia intensa con otras plataformas de alquiler de alojamiento.</td>
        </tr>
        <tr>
            <td align="center">Oportunidades</td>
            <td align="center">Expansión mediante aplicaciones integradas para mejorar la comunicación entre sus usuarios.</td>
            <td align="center">Desarrollo de nuevas características y servicios para mejorar la experiencia del usuario.</td>
            <td align="center">Alianzas estratégicas con proveedores de servicios de eventos.</td>
            <td align="center">Aprovechamiento de la tendencia creciente del turismo y los viajes.</td>
        </tr>
        <tr>
            <td align="center">Amenazas</td>
            <td align="center">Cambios en la regulación de alquileres vacacionales y eventos.</td>
            <td align="center">Posible disminución de la demanda de viajes debido a crisis económicas o sanitarias.</td>
            <td align="center">Innovaciones tecnológicas que podrían ser adoptadas por competidores.</td>
            <td align="center">Posible pérdida de confianza del usuario debido a problemas de seguridad o calidad del servicio.</td>
        </tr>
    </tbody>
</table>

### 2.1.2. Estrategias y tácticas frente a competidores

<div align="justify">

En esta sección se analizarán las estrategias y tácticas que se implementarán para aprovechar las debilidades de la competencia y enfrentar sus fortalezas, así como para abordar las amenazas y oportunidades del mercado. Para ello, hemos empleado un análisis FODA que nos ha permitido identificar nuestras fortalezas y debilidades internas, así como las oportunidades y amenazas externas, todo en función de nuestros dos segmentos objetivos: arrendadores y arrendatarios.

**Estrategia de diferenciación:**

**Para los arrendadores:** A diferencia de otras plataformas de alquiler de espacios para eventos, AlquilaFácil ofrecerá herramientas innovadoras para la gestión de reservas y un sistema de promoción destacada para que sus espacios tengan mayor visibilidad. Además, contarán con opciones para integrar servicios adicionales como catering o entretenimiento, facilitando así una oferta más completa para los clientes.

**Para los arrendatarios:** Nuestra interfaz será fácil de usar y estará diseñada para simplificar todo el proceso de búsqueda, comparación y reserva de espacios. AlquilaFácil también permitirá la personalización de eventos y la contratación de servicios complementarios desde la misma plataforma, brindando una experiencia integral y diferenciada.

**Estrategia de liderazgo en Costos:**

AlquilaFácil buscará ofrecer un modelo flexible y competitivo en costos. Si bien se mantendrán tarifas estándar por el uso de la plataforma, se explorarán modelos de monetización creativa que permitan diversificar los ingresos sin afectar la accesibilidad. Se ofrecerán servicios premium opcionales para arrendadores que deseen destacar sus listados o acceder a herramientas avanzadas de gestión. También se considerará la inclusión de servicios adicionales bajo demanda, así como publicidad no intrusiva y patrocinios de eventos como fuentes complementarias de ingreso.

**Estrategia de marketing:**

El marketing de AlquilaFácil estará enfocado en construir una comunidad activa y comprometida de arrendadores y arrendatarios. Se buscará destacar los beneficios de la plataforma no solo desde el punto de vista funcional, sino también como un espacio para compartir experiencias, generar confianza y fidelizar usuarios.

**Tácticas:**

- **Campañas segmentadas:** Se lanzarán campañas digitales específicas para arrendadores y otras para arrendatarios, empleando publicidad en redes sociales, colaboraciones con influencers del sector de eventos y alianzas con proveedores de servicios relacionados.
- **Fomento de comunidad:** Se habilitarán espacios dentro de la plataforma para que los usuarios compartan sus experiencias, recomienden espacios o servicios, e interactúen entre sí, fortaleciendo así el sentido de comunidad.
- **Eventos y participación activa:** AlquilaFácil participará en ferias comerciales, eventos del sector y actividades colaborativas que aumenten la visibilidad de la marca y fomenten la interacción directa con los usuarios.
- **Modelos de referidos:** Se incentivará a los usuarios actuales a invitar a nuevos miembros mediante recompensas como descuentos, servicios premium o visibilidad destacada.

</div>

## 2.2. Entrevistas

### 2.2.1. Diseño de entrevistas

<div align="justify">

Se ha definido una cierta cantidad de preguntas para cada uno de nuestros segmentos objetivo, con la finalidad de obtener información cualitativa como opiniones o descripciones. Esta información nos será de gran ayuda en el desarrollo de nuestra solución.

**Preguntas generales:**

1. ¿Cuál es tu nombre?  
2. ¿Qué edad tienes?  
3. ¿Dónde vives actualmente?  
4. ¿A qué te dedicas?  

**Preguntas segmento de arrendadores de espacios para eventos:**

1. ¿Qué tan útil te parecería tener una sola plataforma como AlquilaFácil para gestionar reservas, pagos y comunicación con los usuarios?

2. ¿Te gustaría que los usuarios puedan dejar calificaciones y comentarios sobre tu espacio? ¿Por qué?

3. ¿Qué tan importante es para vos poder aprobar o rechazar reservas según el perfil o reputación del usuario?

4. ¿Te serviría ver reportes o estadísticas sobre las reservas y uso de tu espacio?

5. ¿Cómo te gustaría recibir los pagos de tus alquileres? ¿Todo desde la misma plataforma?

6. ¿Cuánto valorás tener una app que te ayude a resolver reclamos o problemas con arrendatarios de forma rápida?

7. ¿Qué tan importante es para vos poder tener visibilidad de lo que ocurre en tu espacio durante un evento?

8. ¿Te gustaría recibir alertas si algo inusual sucede mientras alguien está usando tu espacio?

9. ¿Qué tipo de herramientas o soluciones tecnológicas creés que te ayudarían a gestionar mejor tu propiedad?

10. ¿Te interesaría usar tecnología que te permita tener más control sobre el uso de tu espacio sin necesidad de estar presente?

**Preguntas segmento de arrendatarios sociales / usuarios frecuentes de espacios para eventos:**

1. ¿Qué tan útil te parecería una app como AlquilaFácil que te permita ver espacios disponibles, comparar precios y reservar en el mismo lugar?

2. ¿Qué tanto valoras poder leer opiniones y calificaciones de otros usuarios antes de alquilar un espacio?

3. ¿Cómo te gustaría que sea el proceso de reserva: rápido, seguro, desde la misma plataforma?

4. ¿Qué tan importante sería para vos poder reportar problemas o hacer reclamos directamente desde la app?

5. ¿Qué tan fácil te resulta hoy en día encontrar espacios adecuados para tus eventos?

6. ¿Te sentirías más cómodo/a alquilando si la app tuviera un sistema de reputación tanto para arrendadores como para arrendatarios?

7. ¿Te interesaría recibir notificaciones sobre el estado del lugar durante tu evento? (por ejemplo, si algo se sale de control)

8. ¿Qué tan importante es para ti saber que el espacio cuenta con herramientas que ayuden a garantizar tu seguridad durante el evento?

9. ¿Prefieres lugares que cuenten con tecnología que permita controlar ciertas situaciones mientras se alquila?

10. ¿Qué tipo de herramientas tecnológicas te gustaría que tuvieran los espacios que alquilás para sentirte más tranquilo/a?

</div>


### 2.2.2. Registro de entrevistas

<div align="justify">

Para el registro de entrevistas se realizará 3 entrevista por segmento, dando un total de 6 entrevistas. Además, el formato de las entrevistas es mp4, cada entrevista es independiente debido a las diferentes preguntas y respuestas dadas por los entrevistados de cada segmento.

**Segmento 1: Arrendadores de espacios para eventos**
<br>
<table>
<colgroup>
</colgroup>
<thead>
  <tr>
    <th colspan="2"> <div align="center">Entrevista #1<br></div></th>
  </tr>
</thead>
<tbody>
  <tr>
    <td>Nombre</td>
    <td>Mauricio Abraham</td>
  </tr>
  <tr>
    <td>Apellidos</td>
    <td>Rojas Ugarte</td>
  </tr>
  <tr>
    <td>Edad</td>
    <td>25</td>
  </tr>
  <tr>
    <td>Distrito</td>
    <td>Jesús María</td>
  </tr>
  <tr>
    <td>Aplicaciones usadas</td>
    <td>Facebook, WhatsApp, Excel.</td>
  </tr>
  <tr>
    <td>Motivación</td>
    <td>Proporcionar experiencias memorables a sus clientes, contribuyendo a la felicidad y la celebración de momentos importantes.</td>
  </tr>
  <tr>
    <td>Frustración</td>
    <td>Desafíos en la gestión de reservas y coordinación de eventos.</td>
  </tr>
  <tr>
    <td>Tecnologías</td>
    <td>Android, Windows</td>
  </tr>
	<tr>
    <td>Browsers</td>
    <td>Brave</td>
  </tr>
  <tr>
    <td>Entrevistador</td>
    <td>Angello Sosa</td>
  </tr>
  <tr>
    <td>Evidencia</td>
    <td><div align="center"><img src="images/interviews/arrendador-1.png" alt="Entrevista a Mauricio Rojas"></div></td>
  </tr>
  <tr>
    <td>Enlace</td>
    <td><p><a target="_blank"  href="https://" title="Title">Microsoft Stream</a></p></td>
  </tr>
  <tr>
    <td>Duración<br></td>
    <td>00:00 min - 00:00 min </td>
  </tr>
  <tr>
    <td>Resumen</td>
    <td style="text-align: justify;">
    El entrevistado Mauricio Ugarte tiene 25 años y reside en Pueblo Libre, él es un arrendador con 3 años en el negocio. Durante la entrevista nos reveló diversos datos sobre cómo lleva a cabo el proceso de gestionar sus locales, dentro de esta información se encuentra que maneja el sistema de disponibilidad de sus locales de forma manual, mediante el uso de aplicativos como Excel.
    Asimismo, indicó que últimamente tuvo problemas con el alquiler de sus espacios debido a la falta de herramientas de gestión del local que le notifiquen lo que está sucediendo en el momento.
    </td>
  </tr>
</tbody>
</table>

<br>

<table>
<colgroup>
</colgroup>
<thead>
  <tr>
    <th colspan="2"> <div align="center">Entrevista #2<br></div></th>
  </tr>
</thead>
<tbody>
  <tr>
    <td>Nombre</td>
    <td>Lucero</td>
  </tr>
  <tr>
    <td>Apellidos</td>
    <td>Smith Cardenas</td>
  </tr>
  <tr>
    <td>Edad</td>
    <td>40 años</td>
  </tr>
  <tr>
    <td>Distrito</td>
    <td>San Isidro</td>
  </tr>
  <tr>
    <td>Aplicaciones usadas</td>
    <td>Instagram, X.</td>
  </tr>
  <tr>
    <td>Motivación</td>
    <td>Explorar nuevas oportunidades de negocio y expandir su presencia en el mercado de eventos sociales</td>
  </tr>
  <tr>
    <td>Frustración</td>
    <td>Dificultades para promocionar eficazmente su local y atraer nuevos clientes.</td>
  </tr>
  <tr>
    <td>Tecnologías</td>
    <td>iOS, Android, Windows.</td>
  </tr>
	<tr>
    <td>Browsers</td>
    <td>Google Chrome</td>
  </tr>
  <tr>
    <td>Entrevistador</td>
    <td>Anthony Avalos</td>
  </tr>
  <tr>
    <td>Evidencia</td>
    <td><div align="center"><img src="images/interviews/arrendador-2.png" alt="Entrevista a Lucero Smith"></div></td>
  </tr>
  <tr>
    <td>Enlace</td>
    <td><p><a target="_blank"  href="https://" title="Title">Microsoft Stream</a></p></td>
  </tr>
  <tr>
    <td>Duración<br></td>
    <td>00:00 min - 00:00 min </td>
  </tr>
  <tr>
    <td>Resumen</td>
    <td style="text-align: justify;">
    Lucero es una profesional la cual dispone de muchas propiedades, donde frecuentemente los pode a disposición de amigos o conocidos para que puedan hacer sus reuniones y/o eventos. Ella nos comenta que AlquilaFacil sería una excelente opciones par agestión reservas de sus espacios, mantener una comunicación con los usuarios, y gestionar adecuadamente el cuidado o reglas que este tenga durante el evento. Le gustaría que se maneje un sistema de calificaciones para ayudar a otros usuarios y también para ella misma tener conocimiento de que clase de usuario esta por alquilar su espacio. Nos comenta también que le parece una super idea el tener control total de lo que esté ocurriendo en el evento, como por ejemplo ver que el arrendatario este cumpliendo con las reglas que se le a establecido. También le parecería interesante el poder recibir alertas cuando se incumpla ciertos acuerdos establecidos. Ella cree que sensores de diversos tipos serían los adecuados para llevar un control total de lo que esté ocurriendo en el espacio que está dando a disposición de los usuarios. Le gustaría que todo se haga desde una interfaz sencilla y adaptable a todo tipo de dispositivos.
    </td>
  </tr>
</tbody>
</table>

<br>


<table>
<colgroup>
</colgroup>
<thead>
  <tr>
    <th colspan="2"> <div align="center">Entrevista #3<br></div></th>
  </tr>
</thead>
<tbody>
  <tr>
    <td>Nombre</td>
    <td>Luis David</td>
  </tr>
  <tr>
    <td>Apellidos</td>
    <td>Garcia Días</td>
  </tr>
  <tr>
    <td>Edad</td>
    <td>21 años</td>
  </tr>
  <tr>
    <td>Distrito</td>
    <td>Magdalena</td>
  </tr>
  <tr>
    <td>Aplicaciones usadas</td>
    <td>Instagram, Excel.</td>
  </tr>
  <tr>
    <td>Motivación</td>
    <td>Ver crecer su negocio y convertir su local en un lugar de referencia para eventos en su comunidad.</td>
  </tr>
  <tr>
    <td>Frustración</td>
    <td>Posibles accidentes dentro de su local por falta de herramientas para gestionarlo.</td>
  </tr>
  <tr>
    <td>Tecnologías</td>
    <td>Android, Windows.</td>
  </tr>
	<tr>
    <td>Browsers</td>
    <td>Opera GX</td>
  </tr>
  <tr>
    <td>Entrevistador</td>
    <td>Mariano Ames</td>
  </tr>
  <tr>
    <td>Evidencia</td>
    <td><div align="center"><img src="images/interviews/arrendador-3.png" alt="Entrevista a Luis Garcia"></div></td>
  </tr>
  <tr>
    <td>Enlace</td>
    <td><p><a target="_blank"  href="https://" title="Title">Microsoft Stream</a></p></td>
  </tr>
  <tr>
    <td>Duración<br></td>
    <td>00:00 min - 00:00 min </td>
  </tr>
  <tr>
    <td>Resumen</td>
    <td style="text-align: justify;">
    El entrevistado mencionó que, si se encuentra interesado en la aplicación, lo que mejoraría su negocio al poder gestionar de manera más sencillas sus locales y los arrendatarios.
    Mencionó que anteriormente ha tenido problemas a la hora de organizar reservas mientras no contaba con una herramienta especializada para llevar un recuento de sus reservaciones. También se mencionó que tuvo problemas con diferentes clientes, que de haber tenido un perfil de ellos de antemano se podrían haber evitado.
    Por último, se mostró interesado en poder integrar todo su proceso desde la promoción del local, la reserva y el pago, hasta la gestión y manejo del mismo desde una misma aplicación.
    </td>
  </tr>
</tbody>
</table>
<br>

**Segmento 2: Arrendatarios sociales frecuentes de espacios para eventos**

<br>
<table>
<colgroup>
</colgroup>
<thead>
  <tr>
    <th colspan="2"> <div align="center">Entrevista #1<br></div></th>
  </tr>
</thead>
<tbody>
  <tr>
    <td>Nombre</td>
    <td>Manuel Jesús</td>
  </tr>
  <tr>
    <td>Apellidos</td>
    <td>Chávez Cuba</td>
  </tr>
  <tr>
    <td>Edad</td>
    <td>21</td>
  </tr>
  <tr>
    <td>Distrito</td>
    <td>San Martín de Porres</td>
  </tr>
  <tr>
    <td>Aplicaciones usadas</td>
    <td>Facebook Marketplace</td>
  </tr>
  <tr>
    <td>Motivación</td>
    <td>Ofrecer experiencias únicas y memorables para sus clientes.</td>
  </tr>
  <tr>
    <td>Frustración</td>
    <td>Limitaciones presupuestarias que puedan afectar la calidad de los eventos.</td>
  </tr>
  <tr>
    <td>Tecnologías</td>
    <td>iOS, Android, Windows.</td>
  </tr>
	<tr>
    <td>Browsers</td>
    <td>Google Chrome, Brave</td>
  </tr>
  <tr>
    <td>Entrevistador</td>
    <td>Christopher Lecca</td>
  </tr>
  <tr>
    <td>Evidencia</td>
    <td><div align="center"><img src="images/interviews/arrendatario-1.png" alt="Entrevista a Manuel Chavez"></div></td>
  </tr>
  <tr>
    <td>Enlace</td>
    <td><p><a target="_blank"  href="https://" title="Title">Microsoft Stream</a></p></td>
  </tr>
  <tr>
    <td>Duración<br></td>
    <td>00:00 min - 00:00 min </td>
  </tr>
  <tr>
    <td>Resumen</td>
    <td style="text-align: justify;">
    El entrevistado se presenta como Manuel Chavez, un estudiante de Ingeniería de 21 años. Manuel nos comentó que se encuentra viendo la manera de generar ingresos, por lo que se lo ocurrió adentrarse al mercado de alquiler de espacios para organizar eventos.
    Durante la entrevista, resaltó la necesidad de una aplicación que facilite la reserva de este tipo de espacios, enfocándose en la gestión del local por parte del arrendador, de modo que pueda estar al tanto de aquellas ocurrencias que puedan perjudicar el desarrollo de su evento.
    Para finalizar, nos comentó su experiencia previa con otras herramientas similares y cómo es que estas no cuentan con herramientas de gestión inteligentes que faciliten el control del aforo o detección de riesgos.
    </td>
  </tr>
</tbody>
</table>

<br>


<table>
<colgroup>
</colgroup>
<thead>
  <tr>
    <th colspan="2"> <div align="center">Entrevista #2<br></div></th>
  </tr>
</thead>
<tbody>
  <tr>
    <td>Nombre</td>
    <td>Fabio Ernesto</td>
  </tr>
  <tr>
    <td>Apellidos</td>
    <td>Horna Silva</td>
  </tr>
  <tr>
    <td>Edad</td>
    <td>23</td>
  </tr>
  <tr>
    <td>Distrito</td>
    <td>Surco</td>
  </tr>
  <tr>
    <td>Aplicaciones usadas</td>
    <td>Instagram</td>
  </tr>
  <tr>
    <td>Motivación</td>
    <td>Establecerse como un organizador de eventos reconocido en su área.</td>
  </tr>
  <tr>
    <td>Frustración</td>
    <td>Dificultades para encontrar espacios con características específicas.</td>
  </tr>
  <tr>
    <td>Tecnologías</td>
    <td>Android, Windows.</td>
  </tr>
	<tr>
    <td>Browsers</td>
    <td>Google Chrome, Brave</td>
  </tr>
  <tr>
    <td>Entrevistador</td>
    <td>Carlos Casimiro</td>
  </tr>
  <tr>
    <td>Evidencia</td>
    <td><div align="center"><img src="images/interviews/arrendatario-2.png" alt="Entrevista a XXX"></div></td>
  </tr>
  <tr>
    <td>Enlace</td>
    <td><p><a target="_blank"  href="https://" title="Title">Microsoft Stream</a></p></td>
  </tr>
  <tr>
    <td>Duración<br></td>
    <td>00:00 min - 00:00 min </td>
  </tr>
  <tr>
    <td>Resumen</td>
    <td style="text-align: justify;">
    Fabio Orna Silva, consultor de ingeniería, respondió sobre su experiencia como usuario y proveedor de espacios para eventos, resaltando los desafíos que enfrenta al alquilar y ofrecer inmuebles. Considera muy útil una app como Alquilar Fácil, ya que facilitaría la búsqueda, comparación de precios y reservas en un solo lugar. Destacó la importancia de contar con calificaciones y opiniones de otros usuarios, procesos rápidos y seguros, así como la posibilidad de hacer reclamos directamente desde la plataforma. Además, valoró la existencia de un sistema de reputación para arrendadores y arrendatarios, y sugirió integrar herramientas tecnológicas como cerraduras electrónicas y sistemas de gestión de reservas para mejorar la experiencia y confianza en el servicio.
    </td>
  </tr>
</tbody>
</table>

<br>


<table>
<colgroup>
</colgroup>
<thead>
  <tr>
    <th colspan="2"> <div align="center">Entrevista #3<br></div></th>
  </tr>
</thead>
<tbody>
  <tr>
    <td>Nombre</td>
    <td>Flavia</td>
  </tr>
  <tr>
    <td>Apellidos</td>
    <td>Cáceres Bustamente</td>
  </tr>
  <tr>
    <td>Edad</td>
    <td>23 años</td>
  </tr>
  <tr>
    <td>Distrito</td>
    <td>San Isidro</td>
  </tr>
  <tr>
    <td>Aplicaciones usadas</td>
    <td>Instagram, TikTok.</td>
  </tr>
  <tr>
    <td>Motivación</td>
    <td>Ofrecer experiencias únicas y satisfactorias a sus clientes.</td>
  </tr>
  <tr>
    <td>Frustración</td>
    <td>Falta de herramientas de gestión durante el desarrollo de sus eventos.</td>
  </tr>
  <tr>
    <td>Tecnologías</td>
    <td>iOS, macOS.</td>
  </tr>
	<tr>
    <td>Browsers</td>
    <td>Safari</td>
  </tr>
  <tr>
    <td>Entrevistador</td>
    <td>Anthony Avalos</td>
  </tr>
  <tr>
    <td>Evidencia</td>
    <td><div align="center"><img src="images/interviews/arrendatario-3.png" alt="Entrevista a Flavia Cáceres"></div></td>
  </tr>
  <tr>
    <td>Enlace</td>
    <td><p><a target="_blank"  href="https://" title="Title">Microsoft Stream</a></p></td>
  </tr>
  <tr>
    <td>Duración<br></td>
    <td>00:00 min - 00:00 min </td>
  </tr>
  <tr>
    <td>Resumen</td>
    <td style="text-align: justify;">
    Flavia es una estudiante de los últimos ciclos de su carrera. Su familia suele realizar eventos masivos frecuentemente, y le encargan a ella poder encontrar un lugar adecuado para llevarlo  a cabo. Nos comenta que eta tarea se ve simplificada con una app como AlquilaFacil. Le gustaría que dentro de esta app se pueda ver reseñas de los lugares que posiblemente alquilara. Le parecería genial una plataforma super intuitiva y con una experiencia de usuario fluida. Nos comenta que muchas veces no puede llevar el control del cumplimento de las reglas que se le puso al alquilar ciertos locales. Le gustaría que el local tenga tecnología como sensores de humo, si es que no se puede fumar en el local, o también nel control de aforo, que es uno de los problemas más frecuentes que tiene con sus arrendadores. Y más allá de eso, le gustará que estas herramientas velen por su seguridad y la de sus invitados durante el evento. Le gustaría una aplicación móvil donde pueda recibir alertas si es que alguno de estos limite establecidos dentro del local se está saliendo de control. Una aplicación que te facilite todo este trabajo y te genere tranquilidad, le parecería de mucha utilidad.
    </td>
  </tr>
</tbody>
</table>
</div>

### 2.2.3. Análisis de entrevistas

<div align="justify">

Las entrevistas realizadas proporcionan una visión detallada y matizada sobre las expectativas y requisitos de los distintos actores involucrados en el ámbito de las plataformas de alquiler de espacios para eventos. En general, tanto los arrendadores como los arrendatarios y los usuarios finales destacan la necesidad imperiosa de contar con sistemas que aseguren la integridad de las transacciones financieras, la claridad en los acuerdos contractuales y una comunicación fluida y eficaz. 

**Arrendadores de espacios para eventos**

Para los arrendadores, la seguridad en las transacciones financieras y la integridad de los contratos son aspectos fundamentales. También valoran una promoción efectiva de sus propiedades, buscando una plataforma que les permita llegar a un público amplio y relevante. Además, aprecian una comunicación clara y eficiente con los arrendatarios para evitar malentendidos y conflictos. Algunos arrendadores están dispuestos a invertir en servicios premium que les brinden ventajas adicionales, como una mayor visibilidad de sus espacios en la plataforma. En resumen, los arrendadores buscan una plataforma que les ofrezca seguridad, visibilidad, comunicación eficiente y opciones para maximizar el rendimiento de sus espacios. 


| **Característica objetiva**    | **Frecuencia** | **Porcentaje** | **Sustento desde entrevistas** |
|--------------------------------|----------------|----------------|--------------------------------|
| **Utiliza redes sociales para captar clientes** | 3 de 3. | 100% | Menciona Instagram y Facebook como fuentes principales de clientes |
| **Gestiona reservas manualmente** | 3 de 3. | 100% | Gestiona la disponibilidad con agenda física y Excel |
| **Recibe consultas por WhatsApp**  | 3 de 3. | 100% | Coordina todo el proceso por WhatsApp |
| **Necesita un sistema de agenda para evitar dobles reservas** | 3 de 3. | 100% | Tuvo una doble reserva por falta de sistema automatizado |


**Arrendatarios para eventos**

Por otro lado, los arrendatarios tienen necesidades específicas al utilizar plataformas de alquiler de locales. Para ellos, la facilidad de encontrar y reservar espacios adecuados es crucial, especialmente en situaciones de emergencia o cambios de último momento. Valoran la transparencia en los contratos y una comunicación eficiente con los arrendadores para evitar malentendidos y asegurar una experiencia sin contratiempos. Además, buscan plataformas que ofrezcan una amplia variedad de opciones de espacios que se ajusten a sus necesidades específicas y horarios. La posibilidad de utilizar herramientas de búsqueda avanzada y filtrado también es importante para encontrar el lugar perfecto. En resumen, los arrendatarios de eventos buscan plataformas que les brinden facilidad de uso, transparencia en los procesos, comunicación eficiente y una amplia gama de opciones de espacios para eventos. 


| **Característica objetiva**    | **Frecuencia** | **Porcentaje** | **Sustento desde entrevistas** |
|--------------------------------|----------------|----------------|--------------------------------|
| **Uso de redes sociales o sitios web para buscar espacios** | 3 de 3. | 100% | Todos los entrevistados mencionan usar redes o sitios web |
| **Realiza reservas con regularidad** | 3 de 3. | 100% | Todos mencionan alquilar espacios de forma habitual |
| **Busca espacios para eventos familiares o recreativos**  | 3 de 3. | 100% | Todos organizan o buscan espacios para actividades recreativas o familiares |
| **Valora herramientas que faciliten la organización del tiempo (agenda)** | 3 de 3. | 100% | Mencionan la utilidad de una agenda o calendario para organizarse mejor |


**Determinación de Personas**

Basado en el análisis de las entrevistas, se ha determinado lo siguiente:

**Persona Principal: Arrendatarios**  
**Razón:** Los arrendatarios son los usuarios finales que interactúan directamente con la plataforma para encontrar y reservar espacios. Sus necesidades de facilidad de uso, transparencia, comunicación eficiente y una amplia gama de opciones son cruciales para el éxito del producto. Además, la facilidad de encontrar y reservar espacios adecuados es fundamental para ellos, lo que hace que sus requerimientos sean el enfoque principal del desarrollo.  

**Persona Secundaria: Arrendadores**  
**Razón:** Aunque los arrendadores también son esenciales para el funcionamiento de la plataforma, su papel es secundario en comparación con los arrendatarios. Los arrendadores buscan seguridad, visibilidad y herramientas para la promoción y gestión de sus espacios. Estos aspectos son importantes, pero el enfoque primario debe estar en las necesidades y experiencias de los arrendatarios, que son quienes utilizan la plataforma de manera más activa y recurrente.

</div>

## 2.3. Needfinding

### 2.3.1. User Personas

<p align="justify">
Presentaremos los User Persona por cada segmento objetivo, en los cuales nos basamos en los usuarios ideales de cada segmento: Sergio Aguirre (Arrendatario), Claudia Camareño (Arrendador).
</p>

**Segmento 1: Arrendatario**

![Artefacto creado en UXPressia](images/needfinding/userpersona-1.png)

<br>

**Segmento 2: Arrendador**

![Artefacto creado en UXPressia](images/needfinding/userpersona-2.png)

### 2.3.2. User Task Matrix

<br>

**User Persona Principal**

**Nombre:** Sergio Aguirre  
**Rol:** Arrendatario

<table align="center">
  <thead>
    <tr>
      <th>Task</th>
      <th>Frequency</th>
      <th>Importance</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>Buscar y reservar espacios para eventos</td>
      <td>High</td>
      <td>High</td>
    </tr>
    <tr>
      <td>Comunicarse con los arrendadores de los espacios</td>
      <td>High</td>
      <td>High</td>
    </tr>
    <tr>
      <td>Buscar variedad en los tipos de espacios disponibles</td>
      <td>High</td>
      <td>High</td>
    </tr>
    <tr>
      <td>Reservar espacios para diferentes tipos de eventos</td>
      <td>High</td>
      <td>High</td>
    </tr>
    <tr>
      <td>Estar dispuesto a pagar por una mejor experiencia</td>
      <td>Medium</td>
      <td>Medium</td>
    </tr>
    <tr>
      <td>Utilizar una plataforma fácil de usar e intuitiva</td>
      <td>High</td>
      <td>High</td>
    </tr>
  </tbody>
</table>

<br>

**User Persona Secundaria**

**Nombre:** Claudia Cañamero  
**Rol:** Arrendadora

<table align="center">
  <thead>
    <tr>
      <th>Task</th>
      <th>Frequency</th>
      <th>Importance</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>Gestionar reservas y coordinar eventos</td>
      <td>High</td>
      <td>High</td>
    </tr>
    <tr>
      <td>Promocionar el local en redes sociales y otros canales de marketing</td>
      <td>High</td>
      <td>High</td>
    </tr>
    <tr>
      <td>Mantener el local en óptimas condiciones de limpieza y mantenimiento</td>
      <td>High</td>
      <td>High</td>
    </tr>
    <tr>
      <td>Establecer comunicación efectiva con clientes y proveedores</td>
      <td>High</td>
      <td>High</td>
    </tr>
    <tr>
      <td>Explorar nuevas oportunidades de negocio y crecimiento</td>
      <td>Medium</td>
      <td>Medium</td>
    </tr>
  </tbody>
</table> 
<br>

### 2.3.3. User Journey Mapping

**Persona Principal: Arrendatarios de eventos sociales** 

![Artefacto creado en UXPressia](images/needfinding/journey-1.jpg)

**Persona Secundaria: Arrendadores de espacios para eventos**

![Artefacto creado en UXPressia](images/needfinding/journey-2.jpg)

### 2.3.4. Empathy Mapping

**Persona Principal: Arrendatarios de eventos sociales**

![Artefacto creado en UXPressia](images/needfinding/empathy-1.jpg)

**Persona Secundaria: Arrendadores de espacios para eventos**

![Artefacto creado en UXPressia](images/needfinding/empathy-2.jpg)


### 2.3.5. As-is Scenario Mapping

**Persona Principal: Arrendatarios**

![Artefacto creado en UXPressia](images/needfinding/asis-1.png)

**Persona Secundaria: Arrendadores**

![Artefacto creado en UXPressia](images/needfinding/asis-2.png)

## 2.4. Ubiquitous Language

<table align="center">
  <thead>
    <tr>
      <th><strong>Término</strong></th>
      <th><strong>Definición</strong></th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>Tenant</td>
      <td>Arrendatario, quien realiza la reserva de un espacio.</td>
    </tr>
    <tr>
      <td>Landlord</td>
      <td>Arrendador, quien publica sus espacios para ser reservados.</td>
    </tr>
    <tr>
      <td>Local</td>
      <td>Espacio para eventos que contiene diferentes características de acuerdo con el arrendador.</td>
    </tr>
    <tr>
      <td>Booking</td>
      <td>Reserva de un espacio, con identificación de arrendatario, fecha y hora de inicio y fin.</td>
    </tr>
    <tr>
      <td>Comment</td>
      <td>Comentario acerca de un local anexado a su reseña con calificación.</td>
    </tr>
    <tr>
      <td>Calendar</td>
      <td>Agenda de reservas presentadas tanto para arrendador como arrendatario.</td>
    </tr>
    <tr>
      <td>Report</td>
      <td>Denuncia hacia algún espacio publicada por un arrendatario de este mismo.</td>
    </tr>
    <tr>
      <td>District</td>
      <td>Distrito de locación del espacio publicado.</td>
    </tr>
    <tr>
      <td>Features</td>
      <td>Características adicionales del espacio publicado.</td>
    </tr>
  </tbody>
</table>
  
  
# Capitulo III: Requirements Specification

## 3.1 To-Be Scenario Mapping

![To-be Mapping](resources/To-be-iot.jpeg)

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

**Arrendatarios:** 

![Impact Mapping](resources/Impact-map-arrendatario.png)

**Arrendadores:**

![Impact Mapping](resources/Impact-map-arrendador.png)


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

Link de trello: https://trello.com/b/63Zub4fa/product-backlog-iot

# Capítulo IV: Solution Software Design

## 4.1. Strategic-Level Domain-Driven Design

### 4.1.1. Event Storming
<p>
EventStorming es una técnica de modelado colaborativo e iterativo que permite analizar a fondo problemas complejos y de gran escala, ayudando a descubrir una amplia variedad de detalles y desafíos involucrados.</p>

![Event Storming](/images/imagen_1.png)

Enlace del Miroo para verlo completo:[ https://miro.com/app/board/uXjVKldWbQI=/?share_link_id=811519345320](https://miro.com/app/board/uXjVIBJ9674=/)

#### 4.1.1.1 Candidate Context Discovery

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
Se identificaron siete contextos principales:

IAM (Identity and Access Management): Encargado de la gestión de identidad, registro, autenticación y control de acceso de los usuarios al sistema.

Locals: Responsable del registro, actualización, visualización y reporte de los locales disponibles para reserva.

Booking: Gestiona todo el ciclo de vida de las reservas, incluyendo su creación, modificación, finalización y calificación posterior.

Monitoring: Controla la recolección de datos desde sensores IoT (como aforo, humo o ruido), valida reglas del local y registra infracciones.

Notifications: Administra el envío de alertas a usuarios o arrendadores cuando se detectan condiciones críticas o eventos relevantes.

Profiles: Administra la información personal del usuario para compartirla con otros usuarios

Subscriptions: Gestiona las suscripciones de los usuarios para acceder a beneficios en la aplicación.

Cada uno de estos contextos delimita claramente su modelo de datos, comandos y eventos, lo que permite mantener una arquitectura modular, trazable y preparada para escalar según las necesidades del sistema.
</p>





#### 4.1.1.2 Domain Message Flows Modeling



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







#### 4.1.1.3 Bounded Context Canvases
![Event Storming](/images/imagen_16.jpeg)
![Event Storming](/images/imagen_17.jpeg)
![Event Storming](/images/imagen_18.jpeg)
![Event Storming](/images/imagen_18a.jpeg)


### 4.1.2. Context Mapping

##### 1. Pasos para Crear el Context Mapping
###### 1.1. Identificación de los Bounded Contexts
- IAM (Identity and Access Management)
- Locals
- Booking
- Monitoring
- Notifications
- Profiles
- Subscriptions
###### 1.2. Identificación de Relaciones Iniciales
- IAM ⭤  Booking: Relación de Customer/Supplier.
- IAM proporciona la autenticación y control de acceso, mientras Booking consume la identidad para permitir la creación de reservas.
- IAM ⭤  Locals: Relación de Customer/Supplier.
- IAM proporciona la autenticación y control de acceso, mientras Locals consume la identidad para permitir la publicación de espacios.
- IAM ⭤  Profiles: Relación de Customer/Supplier.
- IAM proporciona la autenticación y control de acceso, mientras Profiles consume la identidad para permitir la visualización de información del usuario.
- IAM ⭤  Subscriptions: Relación de Customer/Supplier.
- IAM proporciona la autenticación y control de acceso, mientras Subscriptions consume la identidad para gestionar los beneficios del usuario.
- Locals ⭤  Booking: Relación de Customer/Supplier.
- Locals administra la disponibilidad y características de los espacios, Booking consulta esa información para registrar una reserva.
- Booking ⭤  Monitoring: Relación de Customer/Supplier.
- Booking genera el inicio y fin de la reserva, mientras Monitoring supervisa el cumplimiento de normas durante ese periodo.
- Monitoring ⭤ Notifications: Relación de Conformist.
- Notifications se adapta a los eventos generados por Monitoring para emitir alertas sin modificar la estructura de los datos.
- Booking ⭤ Notifications: Relación de Conformist.
- Booking puede generar eventos que Notifications transforma en mensajes para usuarios.


##### 2. Análisis de Alternativas y Preguntas Clave
###### 2.1. ¿Qué pasaria si movemos la gestión de reportes de locales desde Locals a Monitoring?
###### Impacto:
Monitoring tendría control total del estado operacional del local.
Se perdería la separación entre información estática del local (Locals) y condiciones temporales (Monitoring).
Discusión:
No se recomienda el cambio. Mantener reportes en Locals permite independencia de la información operativa.

###### 2.2. ¿Y si separáramos Monitoring en dos contexts: SensorEvents y RuleValidation?
Impacto:
Permitiría escalar el procesamiento de eventos por separado del motor de reglas.
Mayor complejidad y necesidad de sincronización.
Discusión:
Podría evaluarse si los volúmenes de datos lo justifican, pero por ahora es preferible mantenerlo unificado.

###### 2.3. ¿Podría Notifications compartir un kernel con Booking?
Impacto:
Se podría optimizar el modelo de eventos compartidos.
Riesgo de acoplamiento excesivo.
Discusión:
Mejor mantener el contrato como evento público. No se recomienda un shared kernel.


###### 2.4. ¿Sería viable mover la asignación de pulseras NFC de Booking a IAM?
Impacto:
IAM controlaría identidad + dispositivo asignado.
Aumenta la carga de IAM, mezcla responsabilidades de autenticación con gestión de dispositivos.
Discusión:
Se recomienda mantener la asignación en Booking para no contaminar IAM con lógica operacional.

##### 3. Alternativas Recomendadas de Context Mapping
Mantener la separación entre datos estáticos (Locals) y monitoreo operacional (Monitoring).
No dividir Monitoring aún, salvo que se presenten cuellos de botella o necesidades de escalabilidad por volumen de eventos.
Evitar compartir kernels entre contexts; priorizar integración por eventos públicos.
Mantener la asignación de dispositivos dentro de Booking.
##### 4. Patrones de Relaciones Sugeridos
- Customer/Supplier: IAM ⭤ Booking, Locals ⭤ Booking, Booking ⭤ Monitoring, IAM ⭤ Subscription, IAM ⭤ Profiles
- Conformist: Monitoring ⭤ Notifications, Booking ⭤ Notifications
- Published Language: Monitoring publica eventos con estructura conocida para consumo externo (ej. por Notifications)
- Anti-Corruption Layer (ACL): Podría evaluarse entre Monitoring y cualquier motor externo de validación de reglas en el futuro

![Event Storming](/images/imagen_19.png)

### 4.1.3. Software Architecture
#### 4.1.3.1. Software Architecture System Landscape Diagram

![Event Storming](/images/imagen_22.png)


#### 4.1.3.2. Software Architecture Context Level Diagrams

![Event Storming](/images/imagen_20.png)

#### 4.1.3.3. Software Architecture Container Level Diagrams

![Event Storming](/images/imagen_21.jpeg)

#### 4.1.3.4. Software Architecture Deployment Diagrams

![Event Storming](/images/imagen_23.png)
  
  
 
## 4.2.1. Bounded Context: IAM Context

### 4.2.1.1. Domain Layer

#### Aggregates

1. **User**
    - **Descripción:** Representa un usuario en la aplicación.
    - **Atributos:**
        - `Id`: Identificador unico para el usuario.
        - `Username`: Nombre del usuario.
        - `Email`: Correo electronico del usuario.
        - `RoleId`: El rol de acceso del usuario.

#### Entities

1. **UserRole**
    - **Descripción:** Representa el rol de acceso que puede tener un usuario (Tester, admin, usuario)
    - **Atributos:**
        - `Id`: Identificador unico para el rol
        - `Role`: Nombre del rol

#### Value Objects

1. **EUserRoles**
    - **Descripción:** Enumerable que contiene todos los tipos de roles que puede tener un usuario.

#### Commands

1. **SeedUserRolesCommand:**
    - **Descripción:** Genera los roles de acceso para poder ser usados.

2. **SignInCommand:**
    - **Descripción:** Inicio de sesión de un usuario ya registrado.

3. **SignUpCommand:**
    - **Descripción:** Registro de un nuevo usuario en la aplicación.

4. **UpdateUsernameCommand:**
    - **Descripción:** Permite el cambio del nombre de un usuario.

#### Queries

1. **GetAllUsersQuery:**
    - **Descripción:** Obtener todos los usuarios registrados.

2. **GetUserByEmailQuery:**
    - **Descripción:** Obtener un usuario en base a su correo electronico.

3. **GetUserByIdQuery:**
    - **Descripción:** Obtener un usuario en base a su Id.

4. **GetUsernameByIdQuery:**
    - **Descripción:** Obtener el nombre de un usuario en base a su Id.

5. **UserExistsQuery:**
    - **Descripción:** Verificar si el usuario ya existe.

#### Repositories

1. **UserRepositroy:**
    - **Descripción:** Interfaz que permite interactuar con la base de datos de usuarios.
    - **Métodos:**
        - `FindByEmailAsync(string email)`: Devuelve un usuario en base al email proporcionado
        - `ExistByUsername(string username)`: Devuelve un valor positivo si el nombre de usuario se encuentra en otro usuario
        - `GetUsernameByIdAsync(int userId)`: Devuelve el nombre de usuario con en base a un id proporcionado
        - `ExistsById(int userId)`: Devuelve un valor positivo si hay un usuario con el id proporcionado

2. **UserRoleRepository:** 
    - **Descripción:** Interfaz que permite interactuar con la base de datos de roles de usuario
    - **Métodos:**
        - `ExistsUserRole(EUserRoles role)`: Devuelve positivo si el rol de usuario ya existe.

### 4.2.1.2. Interface Layer

#### Facades

1. **IamContextFacade:**
    - **Descripción:** Permite que otros bounded context accedan a este contexto a traves del patrón facade
    - **Métodos:**
        - `CreateUser(string username, string password, string email)`: Permite crear un usuario desde fuera del bounded context.
        - `FetchUserIdByUsername(string username)`: Permite extrar el id de un usuario a traves de su nombre de usuario.
        - `FetchUsernameById(int userId)`: Devuelve un nombre de usuario en base a un id proporcionado

#### Controllers

1. **AuthenticationController:**
    - **Descripción:** Expone endpoints para autenticación de usuarios.
    - **Métodos:**
        - `SignIn(SignInResource signInResource)`: Endpoint para el inicio de sesión.
        - `SignUp(SignUpResource signUpResource)`: Endpoint para el registro de un nuevo usuario.

2. **UsersController:** 
    - **Descripción:** Expone endpoints para la gestión de usuarios
    - **Métodos:**
        - `GetUserById(int userId)`: Enpoint que permite obtener un usuario a traves de su id
        - `GetAllUsers()`: Endpoint que permite obtener a todos los usuarios.
        - `GetUserNameById`: Endpoint que permite obtener un nombre de usuario a traves del id del usuario.
        - `UpdateUser(int userId, UpdateUsernameResource updateUsernameResource)`: Endpoint que permite actualizar el nombre de usuario de un usuario

### 4.2.1.3. Application Layer

#### Command Services

1. **SeedUserRoleCommandService:**
    - **Descripción:** Inicializa la tabla de roles de usuarios con los valores preestablecidos
    - **Métodos:**
        - `Handle(SeedUserRolesCommand command)`: Valida y aplica el comando para generar los roles de usuario

2. **UserCommandService:**
    - **Descripción:** Maneja comandos para crear, actualizar o validar usuarios.
    - **Métodos:**
        - `Handle(SignInCommand command)`: Valida y aplica el comando para iniciar la sesión del usuario.
        - `Handle(SignUpCommand command)`: Valida y aplica el comando para registrar un nuevo usuario.
        - `Handle(UpdateUsernameCommand command)`: Valida y aplica el comando para cambiar el nombre a un usuario existente.

#### Query Services

1. **UserQueryService:**
    - **Descripción:** Ofrece consultas para obtener información de los usuarios.
    - **Métodos:**
        - `Handle(GetUserByIdQuery query)`: Valida y aplica la consulta para obtener un usuario dado su id.
        - `Handle(GetAllUsersQuery query)`: Valida y aplica la consulta para obtener todos los usuarios.
        - `Handle(GetUserByEmailQuery)`: Valida y aplica la consulta para obtener un usuario dado su email.
        - `Handle(GetUsernameByIdQuery)`: Valida y aplica la consulta para obtener el nombre de usuario dado el id de un usuario.
        - `Handle(UserExistsQuery)`: Valida y aplica la consulta para verificar que un usuario exista.

#### Outbound Services

1. **Hashing Service:** 
    - **Descripción:** Maneja metodos para encriptar contraseñas y verificarlas.
    - **Métodos:**
        - `HashPassword(string password)`: Permite hashear o encriptar una contraseña
        - `VerifyPassword(string password, string passwordHash)`: Permite validar una contraseña hasheada o encriptada con una original

2. **Token Service:**
    - **Descripción:** Maneja los tokens para poder manejar la sesión de los usuarios.
    - **Métodos:**
        - `GenerateToken(User user)`: Permite generar un token unico asociado a un usuario.
        - `ValidateToken(string token)`: Permite validar el token de un usuario.

### 4.2.1.4. Infrastructure Layer

#### Repositories (Implementacion)

1. **UserRepository:**
    - **Descripción:** Implementación que permite interactuar con la base de datos de usuarios.
    - **Métodos:**
        - `FindByEmailAsync(string email)`: Devuelve un usuario en base al email proporcionado
        - `ExistByUsername(string username)`: Devuelve un valor positivo si el nombre de usuario se encuentra en otro usuario
        - `GetUsernameByIdAsync(int userId)`: Devuelve el nombre de usuario con en base a un id proporcionado
        - `ExistsById(int userId)`: Devuelve un valor positivo si hay un usuario con el id proporcionado

2. **UserRoleRepository:** 
    - **Descripción:** Implementación que permite interactuar con la base de datos de roles de usuario
    - **Métodos:**
        - `ExistsUserRole(EUserRoles role)`: Devuelve positivo si el rol de usuario ya existe.

### 4.2.1.5. Bounded Context Software Architecture Component Level Diagrams

![Diagrama Stucturizr([URL]())](images/c4-component-level-diagrams/iam-context.png)

### 4.2.1.6. Bounded Context Software Architecture Code Level Diagrams

#### 4.2.1.6.1. Bounded Context Domain Layer Class Diagrams

![Diagrama LucidChart([URL]())](images/class-diagrams/iam-class-diagram.png)

#### 4.2.1.6.2. Bounded Context Database Design Diagram

![Diagrama Vertabello([URL]())](images/database-diagrams/iam-database-diagram.png)
  
## 4.2.2. Bounded Context: Locals Context

### 4.2.X.1. Domain Layer

#### Aggregates

1. **Local**
   - **Descripción:** Representa un espacio físico disponible para ser arrendado, incluyendo características como ubicación, precio, tipo y capacidad.
   - **Atributos:**
     - `Id`: Identificador único del local.
     - `Features`: Características especiales del local.
     - `Capacity`: Capacidad máxima de personas.
     - `LocalName`: Tipo o nombre del local (objeto de valor `LocalName`).
     - `NightPrice`: Precio por noche (objeto de valor `NightPrice`).
     - `PhotoUrl`: URL de la foto principal del local (objeto de valor `PhotoUrl`).
     - `StreetAddress`: Dirección completa (objeto de valor `StreetAddress`).
     - `CityPlace`: Ciudad y país (objeto de valor `CityPlace`).
     - `DescriptionMessage`: Descripción del local (objeto de valor `DescriptionMessage`).
     - `LocalCategoryId`: Identificador de categoría del local.
     - `UserId`: Identificador del propietario del local.


2. **Comment**
   - **Descripción:** Representa un comentario realizado por un usuario sobre un local, incluyendo la valoración y el texto del comentario.
   - **Atributos:**
     - `Id`: Identificador único del comentario.
     - `UserId`: ID del usuario que realiza el comentario.
     - `LocalId`: ID del local sobre el que se comenta.
     - `Text`: Texto del comentario (objeto de valor `TextComment`).
     - `Rating`: Valoración del local (objeto de valor `RatingComment`).
     - `CommentText`: Texto plano del comentario.
     - `CommentRating`: Valor numérico de la calificación.

3. **Report**
   - **Descripción:** Representa un reporte o queja generado sobre un local, realizado por un usuario.
   - **Atributos:**
     - `Id`: Identificador único del reporte.
     - `LocalId`: ID del local reportado.
     - `Title`: Título del reporte.
     - `UserId`: ID del usuario que genera el reporte.
     - `Description`: Descripción del problema o situación reportada.
     - `CreatedAt`: Fecha de creación del reporte.

#### Entities

1. **LocalCategory**
   - **Descripción:** Representa una categoría de locales, como auditorio, salón de eventos, oficina, etc.
   - **Atributos:**
     - `Id`: Identificador único de la categoría.
     - `Name`: Nombre de la categoría (por ejemplo, \"Auditorio\", \"Coworking\", \"Salón de Eventos\").
     - `PhotoUrl`: URL de una imagen representativa de la categoría.


#### Value Objects

1. **CityPlace**
   - **Descripción:** Representa el país y la ciudad donde se ubica un local.
   - **Atributos:**
     - `Country`: País del local.
     - `City`: Ciudad del local.
     - `FullCityPlace`: Representación completa como texto (`"País, Ciudad"`).

2. **DescriptionMessage**
   - **Descripción:** Representa el mensaje descriptivo o detalle del local.
   - **Atributos:**
     - `MessageDescription`: Texto descriptivo del local.

3. **LocalName**
   - **Descripción:** Representa el tipo o nombre asignado a un local.
   - **Atributos:**
     - `TypeLocal`: Nombre o tipo del local (ej: \"Auditorio\", \"Sala de Reuniones\").

4. **NightPrice**
   - **Descripción:** Representa el precio por noche de alquiler del local.
   - **Atributos:**
     - `PriceNight`: Valor numérico del precio.

5. **PhotoUrl**
   - **Descripción:** Representa la URL de la foto principal del local.
   - **Atributos:**
     - `PhotoUrlLink`: Enlace de la imagen.

6. **RatingComment**
   - **Descripción:** Representa la calificación numérica otorgada a un local en un comentario.
   - **Atributos:**
     - `Rating`: Puntuación del comentario (ej: de 1 a 5 estrellas).

7. **StreetAddress**
   - **Descripción:** Representa la dirección geográfica del local.
   - **Atributos:**
     - `District`: Distrito donde se ubica el local.
     - `Street`: Calle específica del local.
     - `FullAddress`: Representación completa como texto (`"Distrito, Calle"`).

8. **TextComment**
   - **Descripción:** Representa el texto escrito de un comentario sobre un local.
   - **Atributos:**
     - `Text`: Contenido textual del comentario.


#### Commands

1. **CreateLocalCommand**
   - **Descripción:** Permite registrar un nuevo local con todos sus datos estructurados.
   - **Parámetros:**
     - `District`: Distrito donde se ubica el local.
     - `Street`: Calle del local.
     - `LocalType`: Tipo o categoría del local.
     - `Country`: País.
     - `City`: Ciudad.
     - `Price`: Precio por noche.
     - `PhotoUrl`: Enlace de la imagen principal.
     - `DescriptionMessage`: Descripción del local.
     - `LocalCategoryId`: ID de la categoría.
     - `UserId`: ID del arrendador que registra el local.
     - `Features`: Características adicionales del local.
     - `Capacity`: Capacidad máxima de personas.

2. **UpdateLocalCommand**
   - **Descripción:** Actualiza los atributos de un local existente.
   - **Parámetros:**
     - `Id`: ID del local a actualizar.
     - (Resto de parámetros iguales a `CreateLocalCommand`)

3. **CreateCommentCommand**
   - **Descripción:** Registra un nuevo comentario para un local.
   - **Parámetros:**
     - `UserId`: ID del usuario que comenta.
     - `LocalId`: ID del local.
     - `Text`: Texto del comentario.
     - `Rating`: Puntuación asignada al local.

4. **CreateReportCommand**
   - **Descripción:** Permite crear un reporte operativo o queja sobre un local.
   - **Parámetros:**
     - `LocalId`: ID del local reportado.
     - `Title`: Título del reporte.
     - `UserId`: ID del usuario que genera el reporte.
     - `Description`: Contenido del reporte.

5. **DeleteReportCommand**
   - **Descripción:** Elimina un reporte existente en base a su ID.
   - **Parámetros:**
     - `Id`: ID del reporte a eliminar.

6. **SeedLocalCategoriesCommand**
   - **Descripción:** Permite poblar la base de datos con un conjunto inicial de categorías de locales.
   - **Parámetros:** *(Ninguno)*



#### Queries

1. **GetAllCommentsByLocalIdQuery**
   - **Descripción:** Obtiene todos los comentarios asociados a un local específico.
   - **Parámetros:**
     - `LocalId`: ID del local.

2. **GetAllLocalCategoriesQuery**
   - **Descripción:** Obtiene todas las categorías de locales disponibles.
   - **Parámetros:** *(Ninguno)*

3. **GetAllLocalDistrictsQuery**
   - **Descripción:** Obtiene todos los distritos donde existen locales registrados.
   - **Parámetros:** *(Ninguno)*

4. **GetAllLocalsByLocalCategoryIdQuery**
   - **Descripción:** Obtiene todos los locales filtrados por una categoría específica.
   - **Parámetros:**
     - `LocalCategoryId`: ID de la categoría.

5. **GetAllLocalsQuery**
   - **Descripción:** Obtiene todos los locales registrados en el sistema.
   - **Parámetros:** *(Ninguno)*

6. **GetLocalByIdQuery**
   - **Descripción:** Consulta los detalles de un local específico por su ID.
   - **Parámetros:**
     - `LocalId`: ID del local.

7. **GetLocalCategoryByIdQuery**
   - **Descripción:** Consulta los detalles de una categoría específica de locales.
   - **Parámetros:**
     - `Id`: ID de la categoría.

8. **GetLocalsByCategoryIdAndCapacityRangeQuery**
   - **Descripción:** Obtiene locales que pertenecen a una categoría específica y cuyo rango de capacidad está dentro de los límites indicados.
   - **Parámetros:**
     - `LocalCategoryId`: ID de la categoría.
     - `MinCapacity`: Capacidad mínima.
     - `MaxCapacity`: Capacidad máxima.

9. **GetLocalsByUserIdQuery**
   - **Descripción:** Obtiene todos los locales registrados por un usuario específico (arrendador).
   - **Parámetros:**
     - `UserId`: ID del usuario.

10. **GetReportsByLocalIdQuery**
    - **Descripción:** Obtiene todos los reportes asociados a un local específico.
    - **Parámetros:**
      - `LocalId`: ID del local.

11. **GetReportsByUserIdQuery**
    - **Descripción:** Obtiene todos los reportes generados por un usuario específico.
    - **Parámetros:**
      - `UserId`: ID del usuario.

12. **IsLocalOwnerQuery**
    - **Descripción:** Verifica si un usuario específico es propietario de un local.
    - **Parámetros:**
      - `UserId`: ID del usuario.
      - `LocalId`: ID del local.





#### Repositories (Interfaces)

1. **ICommentRepository**
   - **Descripción:** Interfaz para gestionar los comentarios asociados a locales.
   - **Métodos:**
     - `GetAllCommentsByLocalId(int localId)`: Obtiene todos los comentarios de un local específico.

2. **ILocalCategoryRepository**
   - **Descripción:** Interfaz para gestionar las categorías de locales.
   - **Métodos:**
     - `ExistsLocalCategory(EALocalCategoryTypes type)`: Verifica si existe una categoría específica.
     - `GetAllLocalCategories()`: Obtiene todas las categorías de locales.

3. **ILocalRepository**
   - **Descripción:** Interfaz para la gestión de locales registrados en el sistema.
   - **Métodos:**
     - `GetAllDistrictsAsync()`: Obtiene un listado de todos los distritos donde hay locales.
     - `GetLocalsByCategoryIdAndCapacityrange(int categoryId, int minCapacity, int maxCapacity)`: Filtra locales por categoría y rango de capacidad.
     - `GetLocalsByUserIdAsync(int userId)`: Obtiene los locales de un usuario específico (arrendador).
     - `IsOwnerAsync(int userId, int localId)`: Verifica si un usuario es dueño de un local.

4. **IReportRepository**
   - **Descripción:** Interfaz para la gestión de reportes generados sobre locales.
   - **Métodos:**
     - `GetReportsByLocalId(int localId)`: Obtiene los reportes asociados a un local.
     - `GetReportsByUserId(int userId)`: Obtiene los reportes generados por un usuario específico.




### 4.2.2.2. Interface Layer

#### Controllers

1. **CommentController**
   - **Descripción:** Maneja operaciones relacionadas con los comentarios de locales.
   - **Métodos:**
     - `GetAllCommentsByLocalId(int localId)`: Obtiene todos los comentarios realizados sobre un local específico.
     - `CreateComment(CreateCommentResource resource)`: Registra un nuevo comentario para un local.

2. **LocalCategoriesController**
   - **Descripción:** Expone operaciones para consultar las categorías de locales disponibles.
   - **Métodos:**
     - `GetAllLocalCategories()`: Obtiene todas las categorías de locales.

3. **LocalsController**
   - **Descripción:** Maneja las operaciones CRUD principales sobre locales.
   - **Métodos:**
     - `CreateLocal(CreateLocalResource resource)`: Registra un nuevo local.
     - `GetAllLocals()`: Obtiene todos los locales registrados en el sistema.
     - `GetLocalById(int localId)`: Consulta los detalles de un local específico.
     - `UpdateLocal(int localId, UpdateLocalResource resource)`: Actualiza la información de un local existente.
     - `SearchByCategoryIdAndCapacityRange(int categoryId, int minCapacity, int maxCapacity)`: Filtra locales por categoría y rango de capacidad.
     - `GetAllDistricts()`: Obtiene todos los distritos donde hay locales registrados.
     - `GetUserLocals(int userId)`: Obtiene todos los locales registrados por un arrendador específico.

4. **ReportController**
   - **Descripción:** Maneja operaciones relacionadas con la creación, consulta y eliminación de reportes de locales.
   - **Métodos:**
     - `CreateReport(CreateReportResource createReportResource)`: Registra un nuevo reporte de estado o queja sobre un local.
     - `GetReportsByUserId(int userId)`: Obtiene todos los reportes generados por un usuario.
     - `GetReportsByLocalId(int localId)`: Obtiene todos los reportes asociados a un local específico.
     - `DeleteReport(int reportId)`: Elimina un reporte existente por su ID.
  




### 4.2.2.3. Application Layer
#### Command Services

1. **CommentCommandService**
   - **Descripción:** Maneja la lógica de negocio para registrar comentarios en locales.
   - **Dependencias:** `ICommentRepository`, `ILocalRepository`, `IUserCommentExternalService`, `IUnitOfWork`.
   - **Métodos:**
     - `Handle(CreateCommentCommand command)`: Valida existencia del local y usuario, crea el comentario y lo persiste.

2. **LocalCommandService**
   - **Descripción:** Maneja la creación y actualización de locales por parte de los arrendadores.
   - **Dependencias:** `ILocalRepository`, `ILocalCategoryRepository`, `IUnitOfWork`.
   - **Métodos:**
     - `Handle(CreateLocalCommand command)`: Crea un nuevo local validando categoría y precio.
     - `Handle(UpdateLocalCommand command)`: Actualiza un local existente validando entidad y datos.

3. **LocalCategoryCommandService**
   - **Descripción:** Inicializa las categorías de locales disponibles en el sistema.
   - **Dependencias:** `ILocalCategoryRepository`, `IUnitOfWork`.
   - **Métodos:**
     - `Handle(SeedLocalCategoriesCommand command)`: Registra categorías predefinidas si no existen.

4. **ReportCommandService**
   - **Descripción:** Maneja la creación y eliminación de reportes asociados a locales.
   - **Dependencias:** `IReportRepository`, `IUnitOfWork`.
   - **Métodos:**
     - `Handle(CreateReportCommand command)`: Crea y guarda un nuevo reporte.
     - `Handle(DeleteReportCommand command)`: Elimina un reporte existente validando su existencia.


#### Query Services

1. **CommentQueryService**
   - **Descripción:** Permite consultar los comentarios hechos sobre un local.
   - **Dependencias:** `ICommentRepository`.
   - **Métodos:**
     - `Handle(GetAllCommentsByLocalIdQuery query)`: Devuelve todos los comentarios asociados a un local.

2. **LocalQueryService**
   - **Descripción:** Permite consultar información de locales y sus filtros asociados.
   - **Dependencias:** `ILocalRepository`.
   - **Métodos:**
     - `Handle(GetAllLocalsQuery query)`: Lista todos los locales del sistema.
     - `Handle(GetLocalByIdQuery query)`: Devuelve los detalles de un local específico.
     - `Handle(GetAllLocalDistrictsQuery query)`: Devuelve todos los distritos donde hay locales registrados.
     - `Handle(GetLocalsByUserIdQuery query)`: Lista los locales registrados por un arrendador.
     - `Handle(GetLocalsByCategoryIdAndCapacityRangeQuery query)`: Devuelve locales filtrados por categoría y rango de capacidad.
     - `Handle(IsLocalOwnerQuery query)`: Verifica si un usuario es dueño del local.

3. **LocalCategoryQueryService**
   - **Descripción:** Permite consultar la lista de categorías de locales.
   - **Dependencias:** `ILocalCategoryRepository`.
   - **Métodos:**
     - `Handle(GetAllLocalCategoriesQuery query)`: Retorna todas las categorías existentes.

4. **ReportQueryService**
   - **Descripción:** Permite obtener reportes asociados a locales o usuarios.
   - **Dependencias:** `IReportRepository`.
   - **Métodos:**
     - `Handle(GetReportsByLocalIdQuery query)`: Lista los reportes generados para un local.
     - `Handle(GetReportsByUserIdQuery query)`: Lista los reportes generados por un usuario.



### 4.2.2.4. Infrastructure Layer

#### Repositories (Implementaciones)

1. **CommentRepository**
   - **Descripción:** Implementación del repositorio para gestionar comentarios sobre locales.
   - **Hereda de:** `BaseRepository<Comment>`
   - **Métodos implementados:**
     - `GetAllCommentsByLocalId(int localId)`: Devuelve todos los comentarios asociados a un local específico.

2. **LocalCategoryRepository**
   - **Descripción:** Implementación del repositorio para gestionar categorías de locales.
   - **Hereda de:** `BaseRepository<LocalCategory>`
   - **Métodos implementados:**
     - `ExistsLocalCategory(EALocalCategoryTypes type)`: Verifica si existe una categoría específica.
     - `GetAllLocalCategories()`: Devuelve todas las categorías de locales disponibles.

3. **LocalRepository**
   - **Descripción:** Implementación del repositorio para gestionar entidades `Local`.
   - **Hereda de:** `BaseRepository<Local>`
   - **Métodos implementados:**
     - `GetAllDistrictsAsync()`: Obtiene todos los distritos registrados donde hay locales, combinando ubicación con dirección.
     - `GetLocalsByCategoryIdAndCapacityrange(int categoryId, int minCapacity, int maxCapacity)`: Devuelve locales filtrados por categoría y rango de capacidad.
     - `GetLocalsByUserIdAsync(int userId)`: Obtiene todos los locales de un usuario específico.
     - `IsOwnerAsync(int userId, int localId)`: Verifica si un usuario es dueño de un local determinado.
     - `GetLocalByUserId(int userId, int localId)`: Obtiene un local específico por ID si pertenece al usuario.

4. **ReportRepository**
   - **Descripción:** Implementación del repositorio para gestionar reportes relacionados a locales.
   - **Hereda de:** `BaseRepository<Report>`
   - **Métodos implementados:**
     - `GetReportsByLocalId(int localId)`: Devuelve todos los reportes asociados a un local.
     - `GetReportsByUserId(int userId)`: Devuelve todos los reportes realizados por un usuario específico.




### 4.2.2.5. Bounded Context Software Architecture Component Level Diagrams
![Diagrama Stucturizr([URL]())](images/c4-component-level-diagrams/locals_bounded_context.png)

### 4.2.2.6. Bounded Context Software Architecture Code Level Diagrams
#### 4.2.X.6.1. Bounded Context Domain Layer Class Diagrams
![Diagrama Stucturizr([URL]())](images/class-diagrams/class_diagrams_1.png)

#### 4.2.2.6.2. Bounded Context Database Design Diagram
![Diagrama Stucturizr([URL]())](images/database-diagrams/database_diagram.png)
  
## 4.2.3. Bounded Context: Booking Context

### 4.2.3.1. Domain Layer

#### Aggregates

1. **Reservation**
     - `Id`: Identificador único de la reserva.
     - `StartDate`: Fecha y hora de inicio de la reserva
     - `EndDate`: Fecha y hora del fin de la reserva.
     - `UserId`: Identificador único del usuario.
     - `LocalId`: Identificador único del local.

#### Commands

1. **CreateReservationCommand:**
   - **Descripción:** Crear una nueva reserva con la fecha y hora de inicio, fecha y hora de fin, userId y LocalId.

2. **DeleteReservationCommand:**
   - **Descripción:** Elimina una reserva con el Id de la misma.

3. **UpdateReservationDateCommand:**
   - **Descripción:** Permite cambiar la fecha y hora de inicio y la fecha y hora de fin.


#### Queries


1. **GetReservationByEndDate:**
   - **Descripción:** Obtener todas las reservas que finalizan en una fecha específica.

2. **GetReservationByStartDate:**
   - **Descripción:** Obtener todas las reservas que inician en una fecha específica.

3. **GetReservationByLocalIdQuery:**
   - **Descripción:** Obtener todas las reservas asociadas a un local específico.

4. **GetReservationByOwnerIdQuery:**
   - **Descripción:** Obtener todas las reservas realizadas en locales pertenecientes a un propietario específico.

5. **GetReservationByUserId:**
   - **Descripción:** Obtener todas las reservas realizadas por un usuario específico.


#### Repositories (interfaces)

1. **ReservationRepository:**
   - **Descripción:** Interfaz para interactuar con la base de datos de reservas.
   - **Métodos:**
     - `GetReservationsByUserIdAsync(int userId)`: Obtiene todas las reservas realizadas por un usuario específico.
     - `GetReservationByStartDateAsync(DateTime startDate)`: Obtiene todas las reservas que inician en una fecha específica.
     - `GetReservationByEndDateAsync(DateTime endDate)`: Obtiene todas las reservas que finalizan en una fecha específica.
     - `GetReservationsByLocalIdAsync(List<int> localId)`: Obtiene todas las reservas asociadas a uno o más locales específicos.

### 4.2.3.2. Interface Layer

#### Controllers

1. **ReservationController:**
   - **Descripción:** Expone endpoints para la gestión de reservas, incluyendo su creación, actualización, eliminación y consultas por distintos criterios.
   - **Métodos:**
     - `CreateReservationAsync(CreateReservationResource resource)`: Endpoint para crear una nueva reserva.
     - `UpdateReservationAsync(int id, UpdateReservationResource resource)`: Endpoint para actualizar las fechas de una reserva existente.
     - `DeleteReservationAsync(int id)`: Endpoint para eliminar una reserva por su ID.
     - `GetReservationsByUserIdAsync(int userId)`: Endpoint para obtener todas las reservas hechas por un usuario específico.
     - `GetReservationUserDetailsAsync(int userId)`: Endpoint que obtiene reservas y detalles de suscriptores asociadas al usuario dueño del local.
     - `GetReservationByStartDateAsync(DateTime startDate)`: Endpoint para obtener todas las reservas que comienzan en una fecha específica.
     - `GetReservationByEndDateAsync(DateTime endDate)`: Endpoint para obtener todas las reservas que terminan en una fecha específica.


### 4.2.3.3. Application Layer

#### Command Services

1. **ReservationCommandService:**
   - **Descripción:** Servicio encargado de manejar los comandos relacionados a la creación, actualización y eliminación de reservas, aplicando reglas de negocio y validaciones necesarias.
   - **Métodos:**
     - `Handle(CreateReservationCommand reservation)`: Crea una nueva reserva validando existencia de usuario, local, fechas correctas y propiedad del local.
     - `Handle(UpdateReservationDateCommand reservation)`: Actualiza las fechas de una reserva existente tras validar que las fechas sean válidas y futuras.
     - `Handle(DeleteReservationCommand reservation)`: Elimina una reserva por su ID si esta existe.


#### Query Services

2. **ReservationQueryService:**
   - **Descripción:** Servicio encargado de consultar reservas desde la base de datos, permitiendo filtros por usuario, fechas o propiedad del local.
   - **Métodos:**
     - `GetReservationsByUserIdAsync(GetReservationsByUserId query)`: Obtiene todas las reservas asociadas a un usuario dado su ID.
     - `GetReservationByStartDateAsync(GetReservationByStartDate query)`: Obtiene todas las reservas que comienzan en una fecha específica.
     - `GetReservationByEndDateAsync(GetReservationByEndDate query)`: Obtiene todas las reservas que finalizan en una fecha específica.
     - `GetReservationsByOwnerIdAsync(GetReservationsByOwnerIdQuery query)`: Obtiene todas las reservas de los locales propiedad de un usuario específico.

### 4.2.3.4. Application Layer

#### Repositories (implementaciones)

### ReservationRepository

**Descripción:**  
Implementación del repositorio para interactuar con la base de datos de reservas, utilizando Entity Framework Core.

**Métodos:**

- `GetReservationsByUserIdAsync(int userId)`  
  Obtiene todas las reservas realizadas por un usuario específico.

- `GetReservationByStartDateAsync(DateTime startDate)`  
  Obtiene todas las reservas que comienzan en una fecha específica.

- `GetReservationByEndDateAsync(DateTime endDate)`  
  Obtiene todas las reservas que terminan en una fecha específica.

- `GetReservationsByLocalIdAsync(List<int> localId)`  
  Obtiene todas las reservas asociadas a una lista de IDs de locales.


### 4.2.3.5. Bounded Context Software Architecture Component Level Diagrams

![Diagrama Stucturizr([URL]())](images/c4-component-diagrams/booking-context.png)

### 4.2.3.6. Bounded Context Software Architecture Code Level Diagrams

#### 4.2.3.6.1. Bounded Context Domain Layer Class Diagrams

![Diagrama Lucidchart([URL]())](images/class-diagrams/booking-context.png)

#### 4.2.3.6.2. Bounded Context Database Design Diagram

![Diagrama Vertanelo([URL]())](images/database-diagrams/booking-context.png)
  
## 4.2.4. Bounded Context: Management Context

### 4.2.4.1. Domain Layer

#### Aggregates

1. **Sensor:**
   - **Descripción:** Representa un sensor IoT desplegado dentro de un espacio monitoreado (por ejemplo, para ruido o humo).
   - **Atributos:**
     - `Id`: Identificador único del sensor.
     - `Code`: Código físico o serial único del sensor.
     - `Type`: Tipo dek sensor: NOISE, SMOKE, TEMP, etc.
     - `State`: Estado del sensor (ACTIVE, INACTIVE, MAINTENANCE).
     - `Location`: Ubicación física dentro de la propiedad.
     - `LocalId`: Identificador del local al que pertenece.
     - `Readings`: Colección de lecturas registradas por el sensor.

2. **NFCTag**
   - **Descripción:** Representa una tarjeta NFC registrada y asociada a un usuario o propósito.
   - **Atributos:**
     - `Id`: Identificador único del tag.
     - `Code`: Código físico del tag NFC.
     - `Alias`: Nombre opcional para identificar la tarjeta.
     - `IsActive`: Si está activa o desactivada.
     - `ExpirationDate`: Fecha opcional de expiración del tag.

#### Entities

1. **Reading:**
   - **Descripción:** Representa un dato capturado por un sensor en un momento específico.
   - **Atributos:**
     - `Id`: Identificador único de la lectura.
     - `SensorId`: ID del sensor que envió la lectura.
     - `Timestamp`: Fecha y hora de la lectura.
     - `Value`: Valor medidor por el sensor.
     - `Unit`: Unidad de medida (°C, %, etc.).

2. **NFCDetectionEvent:**
   - **Descripción:** Representa un evento de detección de un tag NFC en un lector.
   - **Atributos:**
     - `Id`: Identificador único de la configuración.
     - `DetectedAt`: Momento de la detección.
     - `TagId`: Identificador del NFCTag detectado.
     - `SensorId`: Identificador de sensor que detecta.

#### Value Objects

1. **SensorType:**
   - **Descripción:** Objeto de valor que representa el tipo de un sensor. Asegura el control del tipo de infracción respectivo.
   - **Atributos:**
     - `SensorType`: 	Tipo del sensor: (NOISE, SMOKE, TEMP, etc).

2. **SensorStatus:**
   - **Descripción:** Objeto de valor que representa el estado de un sensor. Asegura que el estado cumpla con ciertas reglas de negocio (por ejemplo, solo valores como 'activo' o 'inactivo').
   - **Atributos:**
     - `Status`: Estado del dispositivo (activo, inactivo, mantenimiento).

3. **Unit:**
   - **Descripción:** Objeto de valor que representa la unidad de valor de una lectura en el sensor.
   - **Atributos:**
     - `Unit`: 	Unidad del valor (ej: dB, ppm, °C).


#### Commands

##### Sensor

1. **CreateSensorCommand:**
   - **Descripción:** Crear un nuevo sensor con tipo, ubicación y estado inicial

2. **CreateReadingCommand:**
   - **Descripción:** Crear una lectura individual desde un sensor para registrarla

3. **UpdateSensorCommand:**
   - **Descripción:** Activar o desactivar un sensor específico

##### NFCTag

1. **CreateNFCTagCommand:**
   - **Descripción:** Registra una nueva tarjeta NFC con UID y alias opcional

2. **UpdateNFCTagCommand:**
   - **Descripción:** Desactiva una tarjeta NFC existente

3. **CreateNFCDetectionEvent:**
   - **Descripción:** Registra un evento de detección de un tag NFC en un lector

#### Queries

##### Sensor

1. **GetAllSensorsByLocalIdQuery:**
   - **Descripción:** Obtener todos los sensores registrados para un id de local dado.

2. **GetSensorByIdQuery:**
   - **Descripción:** Obtener detalles de un sensor específico

3. **GetReadingsBySensorIdQuery:**
   - **Descripción:** Obtener todas las lecturas de un sensor

##### NFCTag

1. **GetNFCTagByIdQuery:**
   - **Descripción:** Obtener detalles de un tag NFC específico

2. **GetAllTagDetectionEventsBySensorIdQuery:**
   - **Descripción:** Obtener eventos de detección para un sensor específico

#### Repositories (Interfaces)

1. **SensorRepository:**
   - **Descripción:** Interfaz para interactuar con la base de datos de sensores.
   - **Métodos:**
     - `FindAllByLocalId(int id)`: Busca todos los sensores por ID de local.
     - `FindById(int id)`: Busca un sensor por su ID.
     - `Save(Sensor sensor)`: Guarda o actualiza un sensor en la base de datos.

2. **ReadingRepository:**
   - **Descripción:** Interfaz para interactuar con la base de datos de lecturas de sensores.
   - **Métodos:**
     - `FindAllBySensorId(int id)`: Busca todas las lecturas por ID de sensor.
     - `Save(Reading reading)`: Guarda o actualiza una lectura en la base de datos.

3. **NFCTagRepository:**
   - **Descripción:** Interfaz para interactuar con la base de datos de tags NFC.
   - **Métodos:**
     - `FindById(int id)`: Busca un tag NFC por su ID.
     - `Save(NFCTag nfcTag)`: Guarda o actualiza un tag NFC en la base de datos.

4. **NFCDetectionEventRepository:**
   - **Descripción:** Interfaz para interactuar con la base de datos de detecciones NFC.
   - **Métodos:**
     - `FindAllBySensorId(int id)`: Busca todas las detecciones por ID de sensor.
     - `Save(NFCDetectionEvent nfcDetectionEvent)`: Guarda o actualiza una deteccion en la base de datos.

### 4.2.4.2. Interface Layer

#### Controllers

1. **SensorsController:**
   - **Descripción:** Expone endpoints para la gestión de sensores, incluyendo la creación, actualización y recuperación de lecturas.
   - **Métodos:**
     - `RegisterSensor(Sensor sensor)`: Endpoint para registrar un nuevo sensor.
     - `RegisterReading(Reading reading)`: Endpoint para registrar una lectura de sensor.
     - `UpdateSensorStatus(int id, String status)`: Endpoint para actualizar el estado de un dispositivo.
     - `GetAllSensorsByLocalId(int id)`: Endpoint para obtener todos los sensores dado un ID de local.
     - `GetSensorById(int id)`: Endpoint para obtener los detalles de un sensor por su ID.
     - `GetAllReadingsBySensorId(int id)`: Endpoint para obtener todos las lecturas dado un ID de sensor.

2. **NFCTagsController:**
   - **Descripción:** Expone endpoints para la gestión de sensores, incluyendo la creación, actualización y recuperación de dispositivos.
   - **Métodos:**
     - `RegisterNFCTag(NFCTag nfcTag)`: Endpoint para registrar un nuevo tag NFC.
     - `RegisterNFCDetectionEvent(NFCDetectionEvent nfcDetectionEvent)`: Endpoint para registrar una detección de evento NFC.
     - `UpdateNFCTagStatus(int id, String status)`: Endpoint para actualizar el estado de un tag NFC.
     - `GetNFCTagById(int id)`: Endpoint para obtener los detalles de un tag NFC por su ID.
     - `GetAllNFCDetectionEventsBySensorId(int id)`: Endpoint para obtener todas las detecciones de eventos NFC dado un ID de sensor.

### 4.2.4.3. Application Layer

#### Command Services

1. **SensorCommandService:**
   - **Descripción:** Maneja comandos para crear y actualizar sensores con sus lecturas.
   - **Métodos:**
     - `Handle(CreateSensorCommand command)`: Valida y aplica el comando para crear un sensor.
     - `Handle(CreateReadingCommand command)`: Valida y aplica el comando para crear una lectura.
     - `Handle(UpdateSensorCommand command)`: Valida y aplica el comando para actualizar el estado de un sensor.

2. **NFCTagCommandService:**
   - **Descripción:** Maneja comandos para crear y actualizar tags NFC con sus detecciones de eventos.
   - **Métodos:**
     - `Handle(CreateNFCTagCommand command)`: Valida y aplica el comando para crear un tag NFC.
     - `Handle(CreateNFCDetectionEventCommand command)`: Valida y aplica el comando para crear una deteccion de evento NFC.
     - `Handle(UpdateNFCTagCommand command)`: Valida y aplica el comando para actualizar el estado de un tag NFC.


#### Query Services

1. **SensorQueryService:**
   - **Descripción:** Ofrece consultas para obtener información sobre los sensores y sus lecturas.
   - **Métodos:**
     - `Handle(GetAllSensorsByLocalIdQuery query)`: Valida y aplica el query para obtener todos los sensores dado un ID de local.
     - `Handle(GetSensorByIdQuery query)`: Valida y aplica el query para obtener la información de un sensor dado su ID.
     - `Handle(GetReadingsBySensorIdQuery query)`: Valida y aplica el query para obtener las lecturas dado un ID de sensor.

2. **NFCTagQueryService:**
   - **Descripción:** Ofrece consultas para obtener información sobre los tag NFC y sus detecciones de eventos.
   - **Métodos:**
     - `Handle(GetNFCTagByIdQuery query)`: Valida y aplica el query para obtener la información de un tag NFC.
     - `Handle(GetAllTagDetectionEventsBySensorIdQuery query)`: Valida y aplica el query para obtener todas las detecciones de eventos dado un ID de sensor.

### 4.2.4.4. Infrastructure Layer

#### Repositories (Implementaciones)

1. **SensorRepository:**
   - **Descripción:** Implementación para interactuar con la base de datos de sensores.
   - **Métodos:**
     - `FindAllByLocalId(int id)`: Busca todos los sensores por ID de local.
     - `FindById(int id)`: Busca un sensor por su ID.
     - `Save(Sensor sensor)`: Guarda o actualiza un sensor en la base de datos.

2. **ReadingRepository:**
   - **Descripción:** Implementación para interactuar con la base de datos de lecturas de sensores.
   - **Métodos:**
     - `FindAllBySensorId(int id)`: Busca todas las lecturas por ID de sensor.
     - `Save(Reading reading)`: Guarda o actualiza una lectura en la base de datos.

3. **NFCTagRepository:**
   - **Descripción:** Implementación para interactuar con la base de datos de tags NFC.
   - **Métodos:**
     - `FindById(int id)`: Busca un tag NFC por su ID.
     - `Save(Sensor sensor)`: Guarda o actualiza un tag NFC en la base de datos.

4. **NFCDetectionEventRepository:**
   - **Descripción:** Implementación para interactuar con la base de datos de detecciones NFC.
   - **Métodos:**
     - `FindAllBySensorId(int id)`: Busca todas las detecciones por ID de sensor.
     - `Save(NFCDetectionEvent nfcDetectionEvent)`: Guarda o actualiza una deteccion en la base de datos.


### 4.2.4.5. Bounded Context Software Architecture Component Level Diagrams

![Diagrama Stucturizr([URL]())](images/c4-component-level-diagrams/management-context.jpg)

### 4.2.4.6. Bounded Context Software Architecture Code Level Diagrams

#### 4.2.4.6.1. Bounded Context Domain Layer Class Diagrams

![Diagrama LucidChart([URL]())](images/class-diagrams/management-context.png)

#### 4.2.4.6.2. Bounded Context Database Design Diagram

![Diagrama Vertabelo([URL]())](images/database-diagrams/management-context.png)
  
  
## 4.2.5. Bounded Context: Notifications Context

### 4.2.5.1. Domain Layer

#### **Aggregates**

**🔹 Notification**

- **Descripción**: Representa una notificación enviada a un usuario dentro del sistema.
- **Atributos**:
  - `Id`: Identificador único de la notificación.
  - `UserId`: Usuario destinatario.
  - `Title`: Título de la notificación.
  - `Message`: Contenido textual.
  - `Type`: Tipo de notificación (sistema, alerta, información).
  - `CreationDate`: Fecha y hora de creación.
  - `State`: Estado de la notificación (`pendiente`, `enviada`, `leída`).

---

### 4.2.5.2. Interface Layer

#### **Controllers**

**🔹 NotificationController**

- **Descripción**: Expone endpoints para gestionar las notificaciones del sistema.
- **Métodos**:
  - `SendNotification(SendNotificationRequestDTO dto)`: Envía una nueva notificación.
  - `GetAllNotificationsByUserId(int userId)`: Retorna todas las notificaciones asociadas a un usuario.
  - `GetUnreadNotificationsByUserId(int userId)`: Lista las notificaciones no leídas del usuario.
  - `MarkAsRead(int notificationId)`: Marca una notificación como leída.

---

### 4.2.5.3. Application Layer

#### **Command Services**

**🔹 NotificationCommandService**

- **Descripción**: Contiene la lógica para gestionar comandos relacionados con el envío de notificaciones.
- **Métodos**:
  - `Handle(SendNotificationCommand command)`: Valida y envía una nueva notificación.

#### **Query Services**

**🔹 NotificationQueryService**

- **Descripción**: Permite consultar notificaciones relacionadas a un usuario.
- **Métodos**:
  - `Handle(GetAllNotificationsByUserIdQuery query)`: Devuelve todas las notificaciones del usuario.
  - `Handle(GetUnreadNotificationsByUserIdQuery query)`: Devuelve notificaciones no leídas.

---

### 4.2.5.4. Infrastructure Layer

#### **Repositories (Implementaciones)**

**🔹 NotificationRepository**

- **Descripción**: Implementa acceso a la base de datos de notificaciones.
- **Métodos**:
  - `findByUserId(userId)`: Lista de notificaciones por usuario.
  - `findUnreadByUserId(userId)`: Lista de notificaciones no leídas.
  - `markAsRead(notificationId)`: Marca una notificación como leída.
  - `save(notification)`: Guarda una nueva notificación.

### 4.2.5.5. Bounded Context Software Architecture Component Level Diagrams

![Diagrama Stucturizr([URL]())](images/c4-component-diagrams/notification-context.png)

### 4.2.5.6. Bounded Context Software Architecture Code Level Diagrams

#### 4.2.5.6.1. Bounded Context Domain Layer Class Diagrams

![Diagrama Lucidchart([URL]())](images/class-diagrams/notification-context.png)

#### 4.2.5.6.2. Bounded Context Database Design Diagram

![Diagrama Vertanelo([URL]())](images/database-diagrams/notification-context.png)

# Conclusiones

<div align="justify">

* AlquilaFácil se consolida como una solución innovadora en el mercado de alquiler de espacios para eventos, ofreciendo una plataforma que simplifica y optimiza el proceso de búsqueda, reserva y gestión de lugares. Su enfoque integral no solo facilita las operaciones tradicionales, sino que también transforma la experiencia de arrendadores y arrendatarios, garantizando una interacción fluida, rápida y eficiente en cada etapa del proceso.

* La propuesta de valor de AlquilaFácil se centra en la eficiencia y en la experiencia del usuario, incorporando herramientas avanzadas de gestión y seguimiento en tiempo real. Estas características distintivas permiten que tanto arrendadores como arrendatarios gestionen sus eventos de manera más organizada y profesional, reduciendo tiempos de respuesta y mejorando significativamente la satisfacción general en la utilización de la plataforma.

* En cuanto a su estrategia de monetización, AlquilaFácil opta por un modelo inteligente y equilibrado: los arrendadores pueden acceder a planes de suscripción premium que les brindan ventajas competitivas, como mayor visibilidad y acceso a analíticas avanzadas, mientras que los arrendatarios disfrutan de un acceso gratuito a la plataforma. Esta estructura fomenta el crecimiento de la oferta de espacios disponibles y asegura un flujo constante de usuarios, fortaleciendo la comunidad dentro del ecosistema de AlquilaFácil.

* Finalmente, AlquilaFácil no solo apunta a consolidarse en el mercado local, sino que tiene una visión ambiciosa de posicionarse como líder global en el sector de alquiler de espacios para eventos. Su compromiso con la innovación, la optimización de procesos y la excelencia en la experiencia de usuario sienta las bases para una expansión sostenida, diferenciándose como un referente en eficiencia, confiabilidad y servicio en la industria.

</div>


# Bibliografía

<div align="justify">

* A Clean Approach to Flutter Development through the Flutter Clean Architecture Package. (2023). *IEEE Conference Publication*. IEEE Xplore. Recuperado de [https://ieeexplore.ieee.org/document/9071367](https://ieeexplore.ieee.org/document/9071367)

* Airbnb. (2024). *Airbnb – Sitio Oficial*. Recuperado de [https://www.airbnb.com.pe/](https://www.airbnb.com.pe/)

* Booking.com. (2024). *Booking.com: La mayor selección de hoteles, casas y alquileres*. Recuperado de [https://www.booking.com/index.es.html](https://www.booking.com/index.es.html)

* Cvent. (2023). *Cvent's Fourth Annual Benchmark Report: The Future of Event Technology in a Post-Pandemic World*. Cvent. Recuperado de [https://marketing.conference-news.co.uk/en-gb/cvent-event-tech-report-2024](https://marketing.conference-news.co.uk/en-gb/cvent-event-tech-report-2024)

* Hybrid Development in Flutter and its Widgits. (2022). *IEEE Conference Publication*. IEEE Xplore. Recuperado de [https://ieeexplore.ieee.org/document/9995973](https://ieeexplore.ieee.org/document/9995973)

* Forrester Research, Inc. (2024). *The Global State of B2B Events, 2024: Marketers Continue to Ride a Wave of Transformation*. Forrester. Recuperado de [https://www.forrester.com/report/the-global-state-of-b2b-events-2024-marketers-continue-to-ride-a-wave-of-transformation/RES181128](https://www.forrester.com/report/the-global-state-of-b2b-events-2024-marketers-continue-to-ride-a-wave-of-transformation/RES181128)

* Inmuebles de Lima. (2024). *Encuentra el inmueble de tus sueños en Lima*. Recuperado de [https://inmueblesdelima.com.pe/](https://inmueblesdelima.com.pe/)

* Jasin, N. (2023, 11 de julio). *Acceso a internet en Perú: Los aspectos clave para reducir la brecha entre el mundo laboral y el educativo*. Business Empresarial. Recuperado de [https://www.businessempresarial.com.pe/acceso-a-internet-en-peru-los-aspectos-clave-para-reducir-la-brecha-entre-el-mundo-laboral-y-el-educativo/](https://www.businessempresarial.com.pe/acceso-a-internet-en-peru-los-aspectos-clave-para-reducir-la-brecha-entre-el-mundo-laboral-y-el-educativo/)

* Mañas, L. (2024). *Agencia de eventos Olympia= Olympia events agency*. Recuperado de [https://repositori.uji.es/xmlui/handle/10234/208284](https://repositori.uji.es/xmlui/handle/10234/208284)

* Vrbo. (2024). *Sitio oficial de Vrbo®*. Recuperado de [https://www.vrbo.com/es-mx/](https://www.vrbo.com/es-mx/)

</div>


# Anexos

<div align="justify">

+ Video de exposición: https://upcedupe-my.sharepoint.com/:f:/g/personal/u202212077_upc_edu_pe/EsajcJikO3pChqWobVLM7LsBUxbNd-ZJkHe5819nZ3CYpQ?e=xmGXjS

</div>
