# Documentación Configuración Base de Datos y Gradle con Microservicio Eventos

## Paso a paso para la configuración con la base de datos MySQL:

#### Primera parte: Añadiendo tablas y editando el proyecto (Al hacer pull, ya lo van a tener)

1. Tenemos como punto de partida el modificar [basic-service] y renombrarlo con [events-service] (Tener en cuenta que tienen que reemplazar el nombre en settings.gradle.kts)

2. Luego añadimos en la carpeta ‘resources’, la carpeta ‘db’ y dentro de ella la carpeta ‘changelog’, dentro de esta última añadimos un file sql para añadir el script de la base de datos del proyecto y se añade un .xml con el nombre ‘db.changelog-master’

![1](https://i.imgur.com/zrgSHnb.png)

(Dentro de nuestro script .sql añadimos nuestras tablas de base de datos)

A continuación la configuración del .xml:

![1](https://i.imgur.com/tnvpBIy.png)

#### Segunda Parte: Configuración del gradle (TODOS deben de hacerlo para su proyecto individual)

1. El gitignore no deja hacer hacer push al .env, por lo que deben de añadir dentro del proyecto ‘events-service’ las siguientes carpetas: ‘.env’ y .env-local-template’ y dentro de ellas se debe de poner lo siguiente:

 ```java
DB_URL=jdbc:mysql://localhost:3306/events
DB_USERNAME=events
DB_PASSWORD=password
DB_SHOW_SQL=true
 ```

![1](https://i.imgur.com/aUZOQ5K.png)

2. Ahora en ‘opciones’ de intellij debemos acceder a la parte de ‘Project Structure’:


![1](https://i.imgur.com/RLDqXkB.png)

3. Debemos darle al botón ‘+’ para añadir un nuevo módulo, y le damos ‘New Module’ 


![1](https://i.imgur.com/kexzO5j.png)

4. Ahora definimos el nombre ‘events-service’ en name, buscamos en carpeta nuestro proyecto rde-backend para localizarlo en location, asegurense de estar usando el JDK 17 y le damos ‘create’.

![1](https://i.imgur.com/neKGnGZ.png)

**IMPORTANTE: Asegurarse de que la actualización gradle se haga en el proyecto ya existente ‘events-service’ y que no cree uno con el mismo nombre dentro de este proyecto, de lo contrario, a la derecha del IDE, en el elefante, se debe de desligar y a la izquierda en la solución se debe de eliminar la copia y hacerlo de nuevo.**

5. Cuando hagamos esta configuración se debe reemplazar lo del archivo ‘build.gradle.kts’ y ponemos el siguiente código:

```java
plugins {
   java
   id("org.springframework.boot") version "3.2.3"
   id("io.spring.dependency-management") version "1.1.4"
}


group = "ucr.sa"
version = "0.0.1-SNAPSHOT"


java {
   sourceCompatibility = JavaVersion.VERSION_17
}

repositories {
   mavenCentral()
}


extra["springCloudVersion"] = "2023.0.0"


dependencies {
   implementation("org.springframework.boot:spring-boot-starter-data-jpa")
  implementation("org.springframework.boot:spring-boot-starter-web")
  implementation("org.springframework.cloud:spring-cloud-starter-netflix-eureka-client")
   implementation("org.liquibase:liquibase-core")
   implementation("com.mysql:mysql-connector-j")
  testImplementation("org.springframework.boot:spring-boot-starter-test")
}


dependencyManagement {
   imports {
    mavenBom("org.springframework.cloud:spring-cloud-dependencies:${property("springCloudVersion")}")
   }
}


tasks.withType<Test> {
   useJUnitPlatform()
}


```
**IMPORTANTE: Asegurarse de darle al elefante para actualizar los cambios**

6. Ahora nos dirigimos a la parte superior de intellij ‘Run/Debug’ y le damos en ‘edit configurations’


![1](https://i.imgur.com/rwkp5QA.png)

7. Le damos en ‘+’ para crear una nueva configuración

![1](https://i.imgur.com/BtPgnVU.png)

8. Escogemos la que dice ‘Gradle’:

![1](https://i.imgur.com/fdDAChu.png)

9. Ponemos las siguientes características para cada campo, las variables de ambiente son las que están en el ‘.env’ y en gradle project escogemos el que dice ‘events-service’, le damos aplicar y ‘OK’

![1](https://i.imgur.com/O31Efeg.png)

#### Tercera parte: Configuración del MySQL en DBeaver (se debe tener en cuenta la contraseña de MySQL que se estableció inicialmente.

1. Primero abrimos la terminal de MySQL y ponemos el siguiente comando: 
 ```sql
CREATE DATABASE IF NOT EXISTS events;
```
![1](https://i.imgur.com/Z7x3jTY.png)

2. Ahora en un nuevo script corremos uno por uno los siguientes comandos:

```sql
CREATE USER 'events'@'%' IDENTIFIED BY 'password';
-- Otorga todos los permisos al usuario en la base de datos
GRANT ALL PRIVILEGES ON events.* TO 'events'@'%' WITH GRANT OPTION;
-- Aplica los cambios de permisos
FLUSH PRIVILEGES;
```
3. Luego abrimos DBeaver y le damos en el enchufe para hacer una conexión de MySQL:


![1](https://i.imgur.com/KS9s6q6.png)

4. Ahora seleccionamos URL y ponemos el siguiente comando: jdbc:mysql://localhost:3306?allowPublicKeyRetrieval=true&useSSL=false
Asegure de poner el nombre de ‘events’ en el campo Database, ponen su contraseña y le dan ‘Finalizar’.
Es preferible que la conexión sea por url, ya que nos permite poner esa dirección, haciendo que permite el Public Key Retrieval, ya que en ocasiones da errores relacionados a esto, y con dicha dirección nos ahorramos dicho problema.



![1](https://i.imgur.com/p7rd0GR.png)

5. Ya solo quedaría correr la aplicación con la configuración de Gradle [bootRun].

 
**Consideraciones extra: Siempre aparecerá un error de Eureka a este punto porque aún no está implementado esa parte, pero se puede usar perfectamente la aplicación (mientras siga levantado) para guardar datos.**






