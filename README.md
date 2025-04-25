## 4.2.X. Bounded Context: Locals Context

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
     - `CreatedDate`: Fecha de creación del registro.
     - `UpdatedDate`: Fecha de última actualización del registro.

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




### 4.2.X.2. Interface Layer

#### Controllers

1. **LocalController:**
   - **Descripción:** Expone endpoints para la gestión de locales, incluyendo creación, actualización, publicación, eliminación, consulta y verificación de disponibilidad.
   - **Métodos:**
     - `RegisterLocal(CreateLocalRequestDTO dto)`: Endpoint para registrar un nuevo local.
     - `UpdateLocal(int id, UpdateLocalRequestDTO dto)`: Endpoint para actualizar los datos de un local existente.
     - `PublishLocal(int id)`: Endpoint para cambiar el estado del local a "publicado".
     - `DeleteLocal(int id)`: Endpoint para eliminar un local (solo si no tiene reservas activas).
     - `GetAllLocalsByArrendador()`: Endpoint para obtener todos los locales del arrendador autenticado.
     - `GetPublishedLocals()`: Endpoint para obtener todos los locales publicados.
     - `GetLocalById(int id)`: Endpoint para consultar los detalles de un local por su ID.
     - `CheckAvailability(int id, DateTime fechaInicio, DateTime fechaFin)`: Endpoint para verificar si el local está disponible entre dos fechas.

2. **ReporteLocalController:**
   - **Descripción:** Expone endpoints para la gestión de reportes de estado sobre los locales.
   - **Métodos:**
     - `CreateReporte(int localId, CreateReporteRequestDTO dto)`: Endpoint para generar un nuevo reporte de un local.
     - `GetAllReportesByLocalId(int localId)`: Endpoint para obtener todos los reportes de un local.
     - `GetLatestReporteByLocalId(int localId)`: Endpoint para obtener el último reporte registrado de un local.
  


### 4.2.X.3. Application Layer

#### Command Services

1. **LocalCommandService:**
   - **Descripción:** Maneja comandos relacionados con la creación, modificación, publicación y eliminación de locales.
   - **Métodos:**
     - `Handle(RegistrarLocalCommand command)`: Valida y aplica el comando para registrar un nuevo local.
     - `Handle(ActualizarLocalCommand command)`: Valida y aplica el comando para actualizar un local existente.
     - `Handle(PublicarLocalCommand command)`: Valida y aplica el comando para marcar el local como publicado.
     - `Handle(EliminarLocalCommand command)`: Valida y aplica el comando para eliminar un local, si no tiene reservas activas.

2. **ReporteLocalCommandService:**
   - **Descripción:** Maneja comandos relacionados con la generación de reportes operativos de locales.
   - **Métodos:**
     - `Handle(CrearReporteLocalCommand command)`: Valida y aplica el comando para crear un nuevo reporte de estado del local.

#### Query Services

1. **LocalQueryService:**
   - **Descripción:** Ofrece consultas para obtener información sobre locales registrados, publicados y por ubicación.
   - **Métodos:**
     - `Handle(ObtenerLocalesDelArrendadorQuery query)`: Devuelve todos los locales del arrendador autenticado.
     - `Handle(ListarLocalesPorDistritoQuery query)`: Devuelve los locales disponibles en un distrito determinado.
     - `Handle(BuscarLocalesPorCapacidadQuery query)`: Devuelve los locales filtrados por capacidad mínima y máxima.
     - `Handle(ConsultarDetallesDelLocalQuery query)`: Devuelve los datos detallados de un local específico.
     - `Handle(ConsultarLocalesPublicadosQuery query)`: Devuelve todos los locales publicados en la plataforma.
     - `Handle(CheckAvailabilityQuery query)`: Verifica si un local está disponible para un rango de fechas.

2. **ReporteLocalQueryService:**
   - **Descripción:** Ofrece consultas para obtener reportes asociados a un local.
   - **Métodos:**
     - `Handle(GetAllReportesByLocalIdQuery query)`: Devuelve todos los reportes emitidos para un local.
     - `Handle(GetLatestReporteByLocalIdQuery query)`: Devuelve el reporte más reciente de un local.



### 4.2.X.4. Infrastructure Layer

#### Repositories (Implementaciones)

1. **LocalRepository:**
   - **Descripción:** Implementación para interactuar con la base de datos de locales.
   - **Métodos:**
     - `FindById(int id)`: Busca un local por su ID.
     - `FindByArrendadorId(int arrendadorId)`: Obtiene los locales registrados por un arrendador.
     - `FindByDistrito(String distrito)`: Filtra los locales por ubicación geográfica.
     - `FindPublished()`: Devuelve los locales marcados como publicados.
     - `Save(Local local)`: Guarda o actualiza un local en la base de datos.
     - `Delete(int id)`: Elimina un local de la base de datos.

2. **ReporteLocalRepository:**
   - **Descripción:** Implementación para gestionar los reportes operativos generados por los arrendadores.
   - **Métodos:**
     - `FindByLocalId(int localId)`: Obtiene todos los reportes de un local.
     - `FindLatestByLocalId(int localId)`: Devuelve el reporte más reciente de un local.
     - `Save(ReporteLocal reporte)`: Guarda o actualiza un reporte de estado.

3. **HistorialVisitasRepository:**
   - **Descripción:** Implementación para almacenar y consultar registros de visitas o consultas de locales.
   - **Métodos:**
     - `FindByLocalId(int localId)`: Devuelve todos los registros de visitas para un local.
     - `Save(HistorialVisitas visita)`: Guarda una nueva visita realizada por un usuario.


### 4.2.X.5. Bounded Context Software Architecture Component Level Diagrams
![Diagrama Stucturizr([URL]())](images/c4-component-level-diagrams/locals-context.png)