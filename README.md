## 4.2.X. Bounded Context: IAM Context

### 4.2.X.1. Domain Layer

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

### 4.2.X.2. Interface Layer

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

### 4.2.X.3. Application Layer

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