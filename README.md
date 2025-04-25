
## 4.2.X. Bounded Context: Notifications Context

---

### 4.2.X.1. Domain Layer

#### **Aggregates**

**🔹 Notification**

- **Descripción**: Representa una notificación enviada a un usuario dentro del sistema.
- **Atributos**:
  - `Id`: Identificador único de la notificación.
  - `UsuarioId`: Usuario destinatario.
  - `Titulo`: Título de la notificación.
  - `Mensaje`: Contenido textual.
  - `Tipo`: Tipo de notificación (sistema, alerta, información).
  - `FechaCreacion`: Fecha y hora de creación.
  - `Estado`: Estado de la notificación (`pendiente`, `enviada`, `leída`).

---

### 4.2.X.2. Interface Layer

#### **Controllers**

**🔹 NotificationController**

- **Descripción**: Expone endpoints para gestionar las notificaciones del sistema.
- **Métodos**:
  - `SendNotification(SendNotificationRequestDTO dto)`: Envía una nueva notificación.
  - `GetAllNotificationsByUserId(int userId)`: Retorna todas las notificaciones asociadas a un usuario.
  - `GetUnreadNotificationsByUserId(int userId)`: Lista las notificaciones no leídas del usuario.
  - `MarkAsRead(int notificationId)`: Marca una notificación como leída.

---

### 4.2.X.3. Application Layer

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

### 4.2.X.4. Infrastructure Layer

#### **Repositories (Implementaciones)**

**🔹 NotificationRepository**

- **Descripción**: Implementa acceso a la base de datos de notificaciones.
- **Métodos**:
  - `findByUserId(userId)`: Lista de notificaciones por usuario.
  - `findUnreadByUserId(userId)`: Lista de notificaciones no leídas.
  - `markAsRead(notificationId)`: Marca una notificación como leída.
  - `save(notification)`: Guarda una nueva notificación.

### 4.2.X.5. Bounded Context Software Architecture Component Level Diagrams

![Diagrama Stucturizr([URL]())](images/c4-component-diagrams/notification-context.png)

### 4.2.X.6. Bounded Context Software Architecture Code Level Diagrams

#### 4.2.X.6.1. Bounded Context Domain Layer Class Diagrams

![Diagrama Lucidchart([URL]())](images/class-diagrams/notification-context.png)

#### 4.2.X.6.2. Bounded Context Database Design Diagram

![Diagrama Vertanelo([URL]())](images/database-diagrams/notification-context.png)