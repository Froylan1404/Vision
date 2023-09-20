# Visión

## Autores

- @Froylán Berrocal Masis
- @Esteban Madriz Astorga
- @Adrian Ureña Moraga

## Introducción

El propósito de este documento es recopilar, analizar y definir las necesidades y características de alto nivel del sistema "Finding Pets". Se enfoca en las capacidades necesarias para abordar una demanda crítica: la necesidad de proporcionar retroalimentación de los servicios que se ofrecen en la red. Esta necesidad surge en un entorno en el que la retroalimentación y la satisfacción de los usuarios desempeñan un papel fundamental en la mejora continua de los servicios en línea.

La retroalimentación de los servicios es esencial para la calidad, la confiabilidad y la mejora constante de cualquier plataforma en línea. Los usuarios desean compartir sus experiencias, expresar sus inquietudes y sugerir mejoras. La falta de un mecanismo eficiente de retroalimentación puede llevar a una desconexión entre los usuarios y el sistema, lo que a su vez puede afectar negativamente la reputación y la eficacia de la plataforma "Finding Pets".

Este documento de Visión proporciona una visión general de todo el proyecto y se centra en cómo el sistema "Finding Pets" abordará la necesidad crítica de brindar una plataforma eficaz de retroalimentación de servicios en línea, garantizando la satisfacción de los usuarios y la mejora continua de la plataforma.



### Alcance

Este documento de Visión tiene como objetivo definir y establecer el alcance del proyecto "Finding Pets". Este proyecto está relacionado con otros dos proyectos que desarrollan  necesidades críticas :

Ausencia de un medio centralizado para la oferta de servicios o productos referentes a temas de animales: Nuestro proyecto se interrelacionan en la medida que calificar entidades, empresa o usuario se vuelve imperativo para que otros puedan notar la calidad del servicio, producto ofrecido.

Ausencia de un medio centralizado para la adopción de mascotas: El proyecto que desarrolle esta necesidad dotará de la aplicación de una funcionalidad principal, y de la misma manera que comprar producto, calificar al usuario que da a la mascota en adopción dará a los usuarios una herramienta con la que podrán hacer una decisión con más confianza. 

Este documento de Visión no solo se relaciona con la definición y el alcance de "Finding Pets" como un proyecto independiente, sino que también reconoce su interacción con otros proyectos que abordan estas necesidades complementarias.


### Acrónimos y abreviaturas

**FP - Finding Pets:** El acrónimo principal del proyecto "Finding Pets". (*)

**UP - Usuarios Principales:** Para referirse a los usuarios finales que utilizan la aplicación para encontrar servicios, productos o adoptar mascotas.

**EB - Empresas y Anunciantes:**   Representa las empresas y proveedores de servicios que utilizan la plataforma para ofrecer servicios o productos relacionados con animales.

**DEV - Desarrolladores:**  El equipo encargado de diseñar, desarrollar y mantener la aplicación "Finding Pets".

**UI/UX - Interfaz de Usuario/Experiencia de Usuario:**  Para referirse al diseño y la usabilidad de la aplicación.

**API - Interfaz de Programación de Aplicaciones:**  Componentes que permiten la interacción entre la aplicación y otras plataformas o servicios.

**CRM - Gestión de Relaciones con el Cliente:**  Si se implementa un sistema para administrar la retroalimentación y las interacciones con los usuarios y las empresas.

**OAA - Organización de Adopción de Animales:**  Para referirse a organizaciones que se dedican a la adopción de mascotas.

**RA - Reseñador de Animales:**  Para las personas que escriben reseñas y comentarios sobre servicios ,adopciones de mascotas y productos.

**ADM - Administrador de la Plataforma:**  Aquellos responsables de gestionar y mantener la plataforma "Finding Pets".

**EMP - Empresas Anunciantes:**  Empresas que utilizan la plataforma para anunciar sus servicios o productos relacionados con animales.

**VET - Veterinarios:**  Para los profesionales de la salud animal que pueden estar involucrados en la plataforma.

**PRP - Personas Responsables de las Mascotas:**  Usuarios que adoptan o tienen mascotas y utilizan la plataforma.

**AC- Atributo de Calidad:**  Características o propiedades que se utilizan para evaluar la calidad de un producto, servicio o sistema.


## Posicionamiento

### Oportunidad de negocio

La necesidad de desarrollar un sistema que facilite la retroalimentación de los servicios en línea relacionados con temas de animales representa una sólida oportunidad de negocios. Esto se debe a la demanda del mercado insatisfecha, la competencia limitada y el potencial para ofrecer un modelo de negocio sostenible a través de monetización y asociaciones estratégicas. Además, la creación de una comunidad comprometida y el enfoque en la mejora continua pueden generar un impacto social positivo y permitir la escalabilidad del proyecto.

### Sentencia del problema


- **El problema:** Falta de un mecanismo eficiente de retroalimentación en línea para los diferentes servicios o productos ofrecidos en relación a las mascotas.
- **Afecta a:** Usuarios primarios, tiendas, veterinarias, refugios.
- **El impacto del cual es:** El impacto de este problema se visualiza en la calidad de los servicios dados, satisfacción del usuario como una desconexión entre proveedores y usuarios en el ámbito del cuidado animal. 
- **Una solución exitosa sería:** Implementar un sistema de valoración basado en estrellas o calificaciones numéricas para cada servicio o producto. Los usuarios deben poder calificar y dejar comentarios detallados sobre sus experiencias.


## Descripción de las personas interesadas

### Resumen de personas interesadas

---

#### Persona 1

#### Persona 1

- **Nombre:** Usuarios primarios
- **Descripción:** Los Usuarios Primarios desempeñan un papel crucial, ya que son uno de los principales beneficiarios y afectados por los servicios y productos que se  ofrecen en la aplicación. 
- **Responsabilidades:** Los Usuarios Primarios tienen la capacidad de dar retroalimentación valiosa y valorar los servicios y productos disponibles en la aplicación, lo que contribuye directamente a la toma de decisiones informadas por parte de otros usuarios. Los usuarios primarios pueden contribuir a la comunidad compartiendo sus experiencias, consejos y recomendaciones con otros usuarios. Su participación activa y sus interacciones con la aplicación son fundamentales para el éxito y la utilidad continua de la plataforma.
- **Rol:** Usuario

#### Persona 2

- **Nombre:** Refugios de animales
- **Descripción:** Éste involucrado asegura la solución de proveer acceso a los interesados en las mascotas que aún no tienen un hogar. 
- **Responsabilidades:** La principal responsabilidad es garantizar el cuidado y el bienestar de los animales que vende. Esto implica proporcionarles un ambiente limpio y seguro, una dieta adecuada, atención veterinaria cuando sea necesario y asegurarse de que los animales sean manejados con cuidado y respeto. Debe brindar a sus clientes información precisa y completa sobre el cuidado y las necesidades de los animales que venden.
- **Rol:** Stakeholder

#### Persona 3

- **Nombre:** Tiendas 
- **Descripción:** Éste involucrado dota a la aplicación diversidad de productos relacionados al cuidado animal. 

- **Responsabilidades:** La tienda debe ofrecer una amplia gama de productos de alta calidad para mascotas, incluyendo alimentos, juguetes, accesorios, ropa y productos de cuidado. Deben asegurarse de que los productos sean seguros y adecuados para las diferentes especies y tamaños de mascotas. La tienda debe mantener un ambiente limpio y ordenado para garantizar la seguridad y la salud de los clientes y las mascotas que la visitan.

- **Rol:** Stakeholder

#### Persona 4

- **Nombre:** Veterinarias 
- **Descripción:** Éste involucrado se encarga de ofrecer cuidado y atención médica a las mascotas y animales.
- **Responsabilidades:** Las veterinarias deben abarcar la prestación de atención médica de alta calidad, el diagnóstico y el tratamiento de enfermedades, la cirugía, la asesoría sobre el cuidado preventivo y, en última instancia, el bienestar de las mascotas y animales bajo su cuidado. La retroalimentación y las valoraciones proporcionadas por los usuarios son una parte valiosa de su colaboración, ya que les permiten recibir comentarios directos sobre su desempeño y la satisfacción de los clientes.
- **Rol:** Stakeholder


---
## Descripción del Producto
Permite a los usuarios de la aplicación dar su opinión acerca de un producto adquirido por las entidades, empresa o usuario. Producto, ya sea una mascota, un alimento, una atención veterinaria, un producto decorativo..
 Ayuda al usuario a conocer la valoración, de manera gráfica, que ha recibido por los demás usuarios, de la aplicación, el producto que va a comprar así como a las entidades a darse a conocer entre las personas y competir de manera más visual con las demás entidades de la aplicación.

---
### Necesidad 1
- **Necesidad:** Valorar un producto ofrecido por una entidad empresa o usuario
- **Persona Interesada:** Usuarios que compran productos en la aplicación.
- **Prioridad:** Alta.
- **Característica:** 
  - **FEA1:** Permitir al usuario dar su opinión sobre el producto adquirido.
  - **FEA2:** Permitir a la entidad cambiar de ser necesario su imagen, descrita por usuarios que compran sus productos.
  - **FEA3:** Permitir a la aplicación un manejo de control sobre qué productos y entidades desean mostrar a sus usuarios para una mayor satisfacción de uso.

### Necesidad 2
- **Necesidad:** Mostrar la valoración realizada por otros usuarios a una entidad que ofrece un producto.
- **Persona Interesad:** Usuarios que venden un producto, entidades que quieren darse a conocer.
- **Prioridad:** Media.
- **Característica:** 
  - **FEA1:** Permitir al usuario informarse sobre lo que puede encontrar en la adquisición de un producto por parte de una empresa.
  - **FEA2:** Permitir a la entidad dar a conocer la calidad de sus productos ofrecidos y ellos mismos como empresa o usuarios.
  - **FEA3:** Permitir a la aplicación interactividad entre usuarios y entidades.
---

## Restricciones y atributos de calidad

- **AC: Rapidez:** Permite a los usuarios interesados encontrar de manera más rápida sus productos deseados.
- **AC: Satisfacción:** Permite al usuario la seguridad de comprar un producto bien valorado.
- **AC: Mantenimiento:** Permite a la aplicación ordenar de manera asertiva, entidades y productos ofrecidos por estos.
- **AC: Inclusión:** Permite al usuario ser parte de la valoración de un producto que ha utilizado.
- **AC:** Promoción: Permite a la entidad conocer la valoración de un producto ofrecido.

- **R:** Personas que no den retroalimentación correcta sobre un producto adquirido.
- **R:** Entidades que no terminan vendiendo el producto ofrecido o de la calidad esperada.
- **R:** Acumulación de comentarios sin aporte alguno a la retroalimentación de un producto o entidad.
- **R:** Posibilidad de dar retroalimentación por parte de los usuarios que no han adquirido un producto.
