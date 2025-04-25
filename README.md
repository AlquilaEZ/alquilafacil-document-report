## 4.2.X. Bounded Context: Booking Context

### 4.2.X.1. Domain Layer

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

### 4.2.X.2. Interface Layer

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


### 4.2.X.3. Application Layer

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

### 4.2.X.5. Bounded Context Software Architecture Component Level Diagrams

![Diagrama Stucturizr([URL]())](images/c4-component-level-diagrams/booking-context.png)

### 4.2.X.6. Bounded Context Software Architecture Code Level Diagrams

#### 4.2.X.6.1. Bounded Context Domain Layer Class Diagrams

![Diagrama Lucidchart([URL]())](images/c4-component-level-diagrams/booking-context.png)

#### 4.2.X.6.2. Bounded Context Database Design Diagram

![Diagrama Vertanelo([URL]())](images/c4-component-level-diagrams/booking-context.png)