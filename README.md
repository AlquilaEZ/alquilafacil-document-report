## 4.2.X. Bounded Context: Management Context

### 4.2.X.1. Domain Layer

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

### 4.2.X.2. Interface Layer

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

### 4.2.X.3. Application Layer

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


### 4.2.X.5. Bounded Context Software Architecture Component Level Diagrams

![Diagrama Stucturizr([URL]())](images/c4-component-level-diagrams/management-context.jpg)

### 4.2.X.6. Bounded Context Software Architecture Code Level Diagrams

#### 4.2.X.6.1. Bounded Context Domain Layer Class Diagrams

![Diagrama LucidChart([URL]())](images/class-diagrams/management-context.png)

#### 4.2.X.6.2. Bounded Context Database Design Diagram

![Diagrama Vertabelo([URL]())](images/database-diagrams/management-context.png)