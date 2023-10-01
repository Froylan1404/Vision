

## UC#07- Registrar valoración

### Descripción:
Este caso de uso describe el proceso de ingresar una valoración o una retroalimentación a un producto o servicio en la aplicación Adopets.
En este caso de uso el usuario puede dar retroalimentación sobre el producto o servicio adquirido con el propósito de que los demás usuarios de la aplicación puedan tener una visión clara de lo que desean adquirir en la aplicación.

### Actores
Usuarios primarios
### Precondiciones
El usuario registrado debe haber iniciado sesión en su cuenta.
Debe haber una transacción previa relacionada con el servicio o producto que el usuario desea valorar.
### Postcondiciones
La valoración del usuario se registra en la aplicación y está disponible para que otros usuarios la consulten.
La puntuación y el comentario del usuario se utilizan para calcular la calificación promedio del elemento valorado.
### Relaciones
### Flujo básico
**1.**  El usuario inicia sesión en la aplicación Adopets utilizando su nombre de usuario y contraseña.

**2.** Una vez dentro de la aplicación, el usuario explora las distintas secciones y busca el producto o servicio que desea valorar. Esto podría incluir refugios de animales, productos para mascotas, servicios de adopción y veterinarias.

**3.** Una vez que el usuario encuentra el elemento que desea valorar, selecciona la opción "Valorar" o "Dejar una opinión" asociada a ese elemento.
La aplicación muestra un formulario de valoración que incluye los siguientes campos: título de la valoración, puntuación y comentario detallado.

**4.** El usuario completa el formulario de valoración proporcionando la información requerida.

**5.** Después de completar el formulario, el usuario confirma su valoración y la envía.

**6.** La aplicación registra la valoración y la asocia al elemento correspondiente, de modo que esté disponible para que otros usuarios la vean.

### Flujos Alternos
Si el usuario decide cancelar la valoración en cualquier punto del proceso, la aplicación lo redirige de vuelta a la página del elemento sin registrar la valoración.

### Requerimientos especiales
**Fórmula matemática:** El cálculo de la calificación promedio se realizará sumando todas las puntuaciones y dividiéndolas por el número total de valoraciones.

**Regla de negocio:**  Solo los usuarios registrados pueden dejar valoraciones.

**Requerimiento de usabilidad:** El formulario de valoración debe ser fácil de usar y estar diseñado de manera intuitiva para fomentar la participación de los usuarios.

**Definiciones de datos:**  Para la puntuación solo se acepta que escojan una valoración del uno al cinco, cada una representando una estrella, siendo cinco estrellas la máxima calificación.

## UC#08 - Administrar comentarios
### Descripción:
Este caso de uso describe el proceso mediante el cual los administradores de la aplicación Adopets pueden administrar los comentarios y valoraciones proporcionados por los usuarios sobre productos y servicios relacionados con animales. Los administradores tienen la capacidad de revisar, aprobar, modificar y eliminar comentarios para garantizar que cumplan con las políticas y estándares de la plataforma.

### Actores:
 Administrador

### Precondiciones:
El administrador debe haber iniciado sesión en su cuenta de administrador.
Deben existir comentarios y valoraciones que requieran revisión o administración.

### Postcondiciones:
Los comentarios se administran de acuerdo con las políticas de la plataforma.
Los comentarios aprobados y modificados se hacen visibles para los usuarios.
Los comentarios eliminados se eliminan de la plataforma.

### Flujo Básico:
**1.** El administrador inicia sesión en la aplicación Adopets utilizando sus credenciales de administrador.

**2.** Una vez dentro de la aplicación, el administrador accede a la sección de administración de comentarios y valoraciones.
La aplicación presenta una lista de comentarios y valoraciones pendientes de revisión.

**3.** El administrador selecciona un comentario para revisar y administrar.
El administrador tiene las siguientes opciones:

**a.** Aprobar el comentario, permitiendo que sea visible para otros usuarios.

**b.** Modificar el contenido del comentario si es necesario y luego aprobarlo.

**c.** Eliminar el comentario si incumple las políticas de la plataforma.

**6.** El administrador guarda los cambios realizados y repite el proceso para otros comentarios si es necesario.


### Flujos Alternos:
Si un comentario no cumple con las políticas de la plataforma, el administrador puede eliminarlo directamente en lugar de modificarlo y aprobarlo.

### Requerimientos Especiales:
Los administradores deben tener la capacidad de realizar un seguimiento y generar informes sobre las acciones de administración de comentarios realizadas en la plataforma.

La plataforma debe mantener un registro de las acciones de administración de comentarios realizadas por los administradores para fines de auditoría y seguimiento.



## UC#09 - Visualizar  comentarios

### Descripción:
Este caso de uso describe cómo los usuarios primarios, los administradores y empresas visualizan los comentarios y valoraciones proporcionados por los usuarios sobre productos y servicios relacionados con animales en la aplicación Adopets. La visualización varía según el rol del usuario para garantizar la privacidad y la administración adecuada de los comentarios.

### Actores:
Usuarios primarios, administradores y organizaciones o empresas.

### Precondiciones:

Tanto los usuario primarios, organizaciones o empresas deben haber iniciado sesión en su cuenta.
Deben existir comentarios y valoraciones que sean visibles para el usuario.
El administrador debe haber iniciado sesión en su cuenta de administrador.


### Postcondiciones:

Tanto los usuarios primarios, como organizaciones o empresas visualizan los comentarios y valoraciones de los demás de acuerdo con su rol y la configuración de privacidad.
Los administradores tienen acceso a la visualización completa de los comentarios para su administración.

### Flujo Básico:

**1.** El usuario primario, el administrador y las organizaciones inician sesión en la aplicación Adopets utilizando sus credenciales respectivas.

**2.** Una vez dentro de la aplicación, el usuario primario, el administrador y las organizaciones acceden a la sección correspondiente para explorar productos o servicios relacionados con animales.

**3.** Cuando selecciona un elemento (por ejemplo, un producto o un refugio), puede ver las valoraciones y comentarios asociados a ese elemento.

**4.** La aplicación muestra los comentarios y valoraciones visibles para los usuarios primarios o la vista completa para los administradores, que pueden incluir calificaciones, comentarios detallados y la información del usuario que los proporcionó.

**5.** El usuario primario, el administrador y empresas pueden leer y considerar esta retroalimentación para tomar decisiones informadas.

### Flujo Alternativo:

Si un comentario ha sido marcado como inapropiado o incumple las políticas de la plataforma, el administrador puede tomar medidas directas de administración desde esta vista completa, incluyendo la eliminación del comentario.

### Requerimientos Especiales:

Los usuarios primarios solo pueden ver los comentarios y valoraciones que son visibles para ellos según la configuración de privacidad.
Los administradores deben tener acceso completo a todos los comentarios para su revisión y administración.




