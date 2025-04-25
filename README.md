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