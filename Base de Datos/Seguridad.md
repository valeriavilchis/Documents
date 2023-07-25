# Seguridad en la base de datos

No es recomendable que <b>TODOS</b> los administradores de la base de datos tengan acceso total a los privilegios.  
Por eso es indispensable definir cuales tareas deben ejecutar cada uno.  
Ejemplo:
- Acceso total
- Creacioón y modificación de estructuras
- Lectura y escritura
- Solo lectura

## Seguridad
### Creación de usuarios

En MYSQL existen dos tipos de usuarios:
- El usuario <b>root</b>, que tiene acceso total.
- El resto de usuarios, quienes tienen limitaciones sobre lo que puede y no hacer en la base de datos.
- Sentencia para visualizar a los usuarios dentro de la base de datos: <b>SELECT user FROM mysql.user;</b>

### Creación de usuario.
CREATE USER valeria@localhost IDENTIFIED BY "contraseña";

### Sentencia para actualizar contraseña.
ALTER USER valeria@localhost IDENTIFIED BY "nueva_contraseña";

## Permisos

Los permisos son privilegios que se tienen sobre una tarea a realizar, en este caso, acciones sobre la base de datos.  
Algunos de los permisos que se aplican son:
- CREATE: permite crear tablas y/o bases de datos.
- SELECT: permite obtener los registros de las tablas.
- UPDATE: permite actualizar los registros de las tablas.
- DELETE: permite eliminar los registros de las tablas.
- DROP: permite eliminar tantos los registros de una tabla como las bases de datos.
- ALL PRIVILEGES: otorga todos los permisos.

## Niveles de privilegios a los usuarios

En MYSQL existen 5 diferentes niveles de privilegios:
- Global: acceso total sin ningun tipo de restricciones.
- De base de datos: acceso para una base de datos, teniendo el control total de la misma.
- De tabla: solo se permite el control de tablas y con ello de todas las columnas definidas.
- De columna: acceso solo a una columna definida en una tabla.
- De rutina: permiso solo a procedimientos almacenados.

### Agregar privilegios a usuarios
GRANT permiso ON electronic_technologies.customer TO valeria@localhost;

### Elimina privilegios a un usuario
REVOKE permiso ON electronic_technologies.customer FROM valeria@localhost;

### Enlistar los permisos que tiene un usuario.
SHOW GRANTS FOR valeria@localhost;

### IMPORTANTE --> despues de actualizar se debe de ejecutar.
FLUSH PRIVILEGES;

## Roles

Los roles son un grupo de privilegios identificados con un nombre.   
Puedes agregar o eliminar privilegios a un rol en cualquier momento.

- DBA: incluye todos los permisos.
- MaintenanceAdmin: permisos para el mantenimiento del servidor.
- ProcessAdmin: permisos para evaluar, supervisar y eliminar procesos de usuarios.
- SecurityAdmin: permisos para administrar inicios de sesiones, también se puede utilizar para otorgar y revocar privilegios.
- MonitorAdmin: permisos minimos para poder supervisar el servidor.
- DBManager: permisos para hacer modificaciones en todas las bases de datos.
- BDDesigner: permisos para crear y hacer ingenieria inversa en todas las bases de datos.
- ReplicationAdmin: permisos para configurar y administrar la replicación.
- BackupAdmin: permisos minimos para realizar copias de seguridad de cualquier base de datos.

### Sentencia para crear roles.
CREATE ROLE nombre_rol_a, nombre_rol_b;

### Sentencia para enlistar los permisos que tiene un rol.
SHOW GRANTS FOR nombre_rol;

### Sentencia para agregar permisos a un rol.
GRANT permiso ON electronic_technologies.customer TO nombre_rol;

### Eliminar permisos de un rol.
REVOKE permiso ON electronic_technologies.customer FROM nombre_rol;

### Agregar un rol a un usuario.
GRANT nombre_rol TO valeria@localhost;

### Eliminar un rol de un usuario.
REVOKE nombre_rol FROM valeria@localhost;

### Activa roles en cada inicio de sesion.
SET DEFAULT ROLE ALL TO valeria@localhost;