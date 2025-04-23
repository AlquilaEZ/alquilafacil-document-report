## 4.2.X. Bounded Context: Locals Context

### 4.2.X.1. Domain Layer

#### Aggregates

1. **Local**
   - **Descripción:** Representa un espacio físico disponible para ser arrendado, con sus características, estado y capacidad.
   - **Atributos:**
     - `Id`: Identificador único del local.
     - `Nombre`: Nombre referencial del local.
     - `Descripcion`: Descripción del espacio.
     - `Ubicacion`: Objeto de valor con dirección geográfica.
     - `CapacidadMaxima`: Número máximo de personas permitidas.
     - `Tipo`: Tipo del local (auditorio, salón, oficina).
     - `Estado`: Estado del local (publicado, no publicado, inactivo).
     - `Imagenes`: Lista de URLs de imágenes.
     - `ServiciosIncluidos`: Lista de comodidades del local.
     - `ArrendadorId`: Identificador del propietario del local.

2. **ReporteLocal**
   - **Descripción:** Informe generado por el arrendador sobre el estado operativo del local.
   - **Atributos:**
     - `Id`: Identificador único del reporte.
     - `LocalId`: Identificador del local.
     - `Fecha`: Fecha de emisión del reporte.
     - `EstadoOperativo`: Estado general (óptimo, requiere mantenimiento).
     - `Observaciones`: Comentarios relevantes.

#### Entities

1. **HistorialVisitas**
   - **Descripción:** Registro histórico de visitas o consultas realizadas sobre un local.
   - **Atributos:**
     - `Id`: Identificador único del registro.
     - `LocalId`: Identificador del local.
     - `UsuarioId`: ID del usuario que consultó.
     - `FechaConsulta`: Fecha y hora de la interacción.

#### Value Objects

1. **Ubicacion**
   - **Descripción:** Objeto de valor que representa los datos geográficos del local.
   - **Atributos:**
     - `Distrito`: Distrito donde se ubica.
     - `Direccion`: Dirección detallada.
     - `Referencia`: Punto de referencia.

2. **CaracteristicasTecnicas**
   - **Descripción:** Objeto de valor que encapsula detalles técnicos del local.
   - **Atributos:**
     - `Conectividad`: Detalles de red e internet.
     - `Equipamiento`: Lista de equipos disponibles.
     - `Iluminacion`: Tipo de iluminación.
     - `Ventilacion`: Sistema de aireación.
     - `Seguridad`: Medidas de seguridad disponibles.

#### Commands

1. **RegistrarLocalCommand**
   - **Descripción:** Permite registrar un nuevo local con sus datos completos.

2. **ActualizarLocalCommand**
   - **Descripción:** Actualiza las características del local existente.

3. **PublicarLocalCommand**
   - **Descripción:** Cambia el estado de un local para ser visible al público.

4. **EliminarLocalCommand**
   - **Descripción:** Elimina un local si no tiene reservas activas.

5. **CrearReporteLocalCommand**
   - **Descripción:** Genera un reporte sobre el estado actual del local.

#### Queries

1. **ObtenerLocalesDelArrendadorQuery**
   - **Descripción:** Devuelve todos los locales registrados por un arrendador.

2. **ListarLocalesPorDistritoQuery**
   - **Descripción:** Lista los locales disponibles en un distrito específico.

3. **BuscarLocalesPorCapacidadQuery**
   - **Descripción:** Filtra locales según capacidad mínima y máxima.

4. **ConsultarDetallesDelLocalQuery**
   - **Descripción:** Consulta todos los detalles de un local específico.

5. **ConsultarLocalesPublicadosQuery**
   - **Descripción:** Devuelve todos los locales marcados como "publicados".

#### Repositories (Interfaces)

1. **LocalRepository**
   - **Descripción:** Interfaz para interactuar con la base de datos de locales.
   - **Métodos:**
     - `findById(id)`: Buscar un local por su ID.
     - `findByArrendadorId(arrendadorId)`: Obtener los locales de un arrendador.
     - `findByDistrito(distrito)`: Listar locales por ubicación.
     - `findPublished()`: Listar todos los locales publicados.
     - `save(local)`: Guardar o actualizar un local.
     - `delete(id)`: Eliminar un local.

2. **ReporteLocalRepository**
   - **Descripción:** Interfaz para gestionar reportes de locales.
   - **Métodos:**
     - `findByLocalId(localId)`: Obtener reportes por local.
     - `findLatestByLocalId(localId)`: Obtener el último reporte de un local.
     - `save(reporte)`: Guardar o actualizar un reporte.

3. **HistorialVisitasRepository**
   - **Descripción:** Interfaz para guardar registros de visitas a locales.
   - **Métodos:**
     - `findByLocalId(localId)`: Consultar visitas por local.
     - `save(historial)`: Guardar una nueva visita.


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