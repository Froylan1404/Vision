

## UC#07- Registrar valoración

## Descripción:
Este caso de uso describe el proceso de ingresar una valoración o una retroalimentación a un producto o servicio en la aplicación Adopets.
En este caso de uso el usuario puede dar retroalimentación sobre el producto o servicio adquirido con el propósito de que los demás usuarios de la aplicación puedan tener una visión clara de lo que desean adquirir en la aplicación.

## Actores
Usuarios primarios
## Precondiciones
El usuario registrado debe haber iniciado sesión en su cuenta.
Debe haber una transacción previa relacionada con el servicio o producto que el usuario desea valorar.
## Postcondiciones
La valoración del usuario se registra en la aplicación y está disponible para que otros usuarios la consulten.
La puntuación y el comentario del usuario se utilizan para calcular la calificación promedio del elemento valorado.
## Relaciones
## Flujo básico
**1.**  El usuario inicia sesión en la aplicación Adopets utilizando su nombre de usuario y contraseña.

**2.** Una vez dentro de la aplicación, el usuario explora las distintas secciones y busca el producto o servicio que desea valorar. Esto podría incluir refugios de animales, productos para mascotas, servicios de adopción y veterinarias.

**3.** Una vez que el usuario encuentra el elemento que desea valorar, selecciona la opción "Valorar" o "Dejar una opinión" asociada a ese elemento.
La aplicación muestra un formulario de valoración que incluye los siguientes campos: título de la valoración, puntuación y comentario detallado.

**4.** El usuario completa el formulario de valoración proporcionando la información requerida.

**5.** Después de completar el formulario, el usuario confirma su valoración y la envía.

**6.** La aplicación registra la valoración y la asocia al elemento correspondiente, de modo que esté disponible para que otros usuarios la vean.

## Flujos Alternos
Si el usuario decide cancelar la valoración en cualquier punto del proceso, la aplicación lo redirige de vuelta a la página del elemento sin registrar la valoración.

## Requerimientos especiales
**Fórmula matemática:** El cálculo de la calificación promedio se realizará sumando todas las puntuaciones y dividiéndolas por el número total de valoraciones.

**Regla de negocio:**  Solo los usuarios registrados pueden dejar valoraciones.

**Requerimiento de usabilidad:** El formulario de valoración debe ser fácil de usar y estar diseñado de manera intuitiva para fomentar la participación de los usuarios.

**Definiciones de datos:**  Para la puntuación solo se acepta que escojan una valoración del uno al cinco, cada una representando una estrella, siendo cinco estrellas la máxima calificación.




