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
      <td>10/04/2025</td>
      <td>
        - Ames Oviedo Mariano Jose <br>
        - Avalos Santos Anthony Piero <br>
        - Lecca Choccare Christopher Bryan <br>
        - Sosa Colca Angello Rodolfo <br
      </td>
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

<table>
  <thead>
    <tr>
      <th>Criterio específico</th>
      <th>Acciones realizadas</th>
      <th>Conclusiones</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>Trabaja en equipo para proporcionar liderazgo en forma conjunta.</td>
      <td>TB1: <br>
      <td></td>
      </tr>
      <td>Comunica en forma escrita ideas y/o resultados con objetividad a público de diferentes especialidades y niveles jerarquicos, en el marco del desarrollo de un proyecto en ingeniería.
      <td>TB1: <br>
      <td></td>
      </td>

      
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
| LLENAR |
|Nombre|Lecca Choccare, Christopher Bryan (U202211399)|
|Mi nombre es Christopher, tengo 20 años y actualmente me encuentro cursando el 7mo ciclo de la carrera de Ingeniería de Software en la Universidad Peruana de Ciencias Aplicadas (UPC). Considero que mi compromiso con el equipo de trabajo designado y mi capacidad de aprendizaje rápida aportarán de buena manera al desarrollo del producto final.|
|Nombre|Sosa Colca, Angello Rodolfo (U202212077)|
|Tengo 19 años y curso el 7mo ciclo de la carrera de Ingeniería de Software en la Universidad Peruana de Ciencias Aplicadas. Soy una persona enfocada, perseverante y colaborativo. Estas cualidades me permiten ser una persona que ayudará de manera óptima el requisito que se me imponga. Además, soy una persona que apoya cuando los demás se encuentran en problemas.|
|Nombre|LLENAR (XXXXXXXXXX)|
| LLENAR |

## 1.2. Solution Profile

En esta sección se detallan los aspectos claves de nuestra solución de software, incluyendo sus características distintivas y propuestas de valor. 

**Product Name:** AlquilaFácil

**Producto Descriptivo:** AlquilaFácil es una plataforma diseñada para simplificar el proceso de búsqueda y reserva de espacios para eventos, conectando de manera eficiente a arrendadores y arrendatarios. Ofrece una experiencia fluida, permitiendo a los usuarios buscar, reservar y gestionar espacios para una amplia variedad de eventos. Además, la plataforma incluye herramientas de gestión y seguimiento en tiempo real, asegurando una experiencia optimizada tanto para arrendadores como para arrendatarios. 

**Monetización:** AlquilaFácil generará ingresos a través de un modelo de suscripción para arrendadores que deseen destacar sus propiedades y acceder a herramientas avanzadas de gestión de reservas. Estos planes premium ofrecerán beneficios adicionales, como una mayor visibilidad en los resultados de búsqueda y acceso prioritario a herramientas analíticas avanzadas. Además, monetizaremos la plataforma mediante la implementación de sensores en los locales, permitiendo a los propietarios recibir reportes detallados sobre la actividad en sus espacios. En contraste, el acceso a la plataforma será completamente gratuito para los arrendatarios, incentivando su participación y aumentando la oferta de espacios disponibles.

## 1.2.1. Antecedentes y Problematicas

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




