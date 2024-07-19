# Gestión de Clientes - Backend
Este proyecto es el backend para la aplicación de gestión de clientes, desarrollado utilizando Spring Boot. Proporciona una API RESTful para interactuar con una base de datos MySQL.

### Tecnologías Utilizadas
Spring Boot
Spring Data JPA
MySQL
Lombok
### Requisitos Previos
Java (>= 11)
Maven (>= 3.6)
MySQL (>= 5.7)

### Instalación
Clona el repositorio:

```
git clone https://github.com/tuusuario/gestion-clientes-backend.git
cd gestion-clientes-backend
```
Configura la base de datos en src/main/resources/application.properties:

### properties
```
spring.datasource.url=jdbc:mysql://localhost:3306/gestion_clientes
spring.datasource.username=tu_usuario
spring.datasource.password=tu_contraseña
spring.jpa.hibernate.ddl-auto=update
spring.jpa.show-sql=true
spring.jpa.properties.hibernate.dialect=org.hibernate.dialect.MySQL5Dialect
```
### Crea la base de datos en MySQL:

sql
```
CREATE DATABASE gestion_clientes;
```
#### Ejecuta la aplicación:
```
mvn spring-boot:run
La aplicación estará disponible en http://localhost:8080.
```

#### Estructura del Proyecto
src/main/java/com/gestion/clientes/

controller/: Controladores que manejan las solicitudes HTTP.

model/: Entidades JPA que representan las tablas de la base de datos.

repository/: Interfaces de repositorio para acceso a datos.

service/: Servicios que contienen la lógica de negocio.

src/main/resources/

application.properties: Archivo de configuración de la aplicación.


### Endpoints de la API
GET /api/v1/clientes: Lista todos los clientes.

POST /api/v1/clientes: Crea un nuevo cliente.

GET /api/v1/clientes/{id}: Obtiene un cliente por ID.

PUT /api/v1/clientes/{id}: Actualiza un cliente por ID.

DELETE /api/v1/clientes/{id}: Elimina un cliente por ID.

### Funcionalidades
#### Listado de Clientes:
Proporciona una lista de clientes almacenados en la base de datos.

#### Agregar Cliente: 
Permite la creación de un nuevo cliente.

#### Editar Cliente:
Permite la actualización de los datos de un cliente existente.

#### Eliminar Cliente: 
Permite la eliminación de un cliente de la base de datos.


https://github.com/user-attachments/assets/fa2cc3db-4bf2-423b-bc4b-a0584d78d213

