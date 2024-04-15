
# Aplicación CRUD de PHP

Este repositorio contiene una aplicación PHP CRUD (Create, Read, Update, Delete) simple. Es una demostración básica de cómo integrar PHP con una base de datos MySQL para gestionar datos de usuarios. La aplicación permite a los usuarios agregar, ver, editar y eliminar información de usuario.

CRUD es un acrónimo que representa las cuatro operaciones básicas utilizadas en el manejo de datos en la mayoría de las aplicaciones web y sistemas de gestión de bases de datos. Cada letra representa una acción específica que se realiza sobre los datos:

Crear (Create):
La operación de crear implica agregar nuevos datos al sistema. Esto podría incluir la creación de nuevos registros en una base de datos, la creación de nuevos archivos en el sistema de archivos o la generación de nuevos elementos en una aplicación.
Por ejemplo, en una aplicación de gestión de clientes, la operación de crear se utilizaría para agregar un nuevo cliente al sistema, ingresando su nombre, dirección, número de teléfono, etc.

Leer (Read):
La operación de leer implica recuperar datos del sistema para su visualización o procesamiento. Esto incluye la recuperación de registros de una base de datos, la lectura de archivos de datos almacenados o la obtención de información de una fuente externa.
Por ejemplo, en una aplicación de redes sociales, la operación de leer se utilizaría para mostrar publicaciones de usuarios en el feed de noticias, obtener información del perfil de un usuario o mostrar comentarios en una publicación.

Actualizar (Update):
La operación de actualizar implica modificar datos existentes en el sistema. Esto podría incluir la modificación de registros en una base de datos, la actualización de archivos de datos almacenados o la modificación de información en una aplicación.
Por ejemplo, en un sistema de gestión de inventario, la operación de actualizar se utilizaría para cambiar la cantidad disponible de un producto después de una venta o actualizar la descripción de un artículo.

Eliminar (Delete):
La operación de eliminar implica eliminar datos del sistema. Esto podría incluir la eliminación de registros de una base de datos, la eliminación de archivos de datos almacenados o la eliminación de elementos de una aplicación.
Por ejemplo, en una aplicación de gestión de tareas, la operación de eliminar se utilizaría para eliminar una tarea completada o cancelada del sistema.

## Importancia en el Desarrollo de Aplicaciones Web
Las operaciones CRUD son fundamentales en el desarrollo de aplicaciones web por varias razones:

Facilidad de gestión de datos: Las operaciones CRUD proporcionan una forma estandarizada de gestionar datos en aplicaciones web, lo que simplifica el proceso de creación, lectura, actualización y eliminación de información.

Interactividad del usuario: Las aplicaciones web suelen permitir a los usuarios interactuar con los datos mediante formularios, botones y otros elementos de la interfaz de usuario. Las operaciones CRUD son la base sobre la cual se construyen estas interacciones, permitiendo a los usuarios crear, ver, actualizar y eliminar datos según sea necesario.

Mantenimiento de la integridad de los datos: Al proporcionar una forma estructurada de interactuar con los datos, las operaciones CRUD ayudan a garantizar que los datos se mantengan consistentes y que la integridad de la base de datos se mantenga en todo momento.

Flexibilidad y escalabilidad: Las aplicaciones web que utilizan operaciones CRUD son más flexibles y escalables, ya que pueden adaptarse fácilmente a cambios en los requisitos comerciales o a un mayor volumen de datos sin necesidad de reescribir grandes porciones del código.

## Tecnologías Utilizadas

- **PHP:** Lenguaje de script del lado del servidor utilizado para el desarrollo web.
- **MySQL:** Sistema de gestión de base de datos utilizado para almacenar datos de usuario.
- **HTML & CSS:** Utilizados para estructurar y dar estilo a las páginas web.
- **Tailwind CSS:** Un framework de CSS utilitario para el desarrollo rápido de interfaces de usuario.

## Páginas y Funcionalidades

### 1. Página de Inicio (`display.php`)

![Página de Inicio](images/display.png)

- **Funcionalidad:** Muestra todos los usuarios de la base de datos en un formato de tabla.
- **Características:** 
  - Ver todos los usuarios.
  - Enlaces de navegación para agregar, editar o eliminar información de usuario.

### 2. Agregar Usuario (`user.php`)

![Agregar Usuario](images/add.png)

- **Funcionalidad:** Permite agregar un nuevo usuario a la base de datos.
- **Características:** 
  - Formulario para ingresar detalles del usuario (nombre, correo electrónico, teléfono móvil, contraseña).
  - Validación de datos y envío a la base de datos.

### 3. Editar Usuario (`edit.php`)

![Editar Usuario](images/edit.png)

- **Funcionalidad:** Permite editar detalles de usuarios existentes.
- **Características:** 
  - Formulario prellenado con la información actual del usuario.
  - Actualización de detalles del usuario en la base de datos.

### 4. Eliminar Usuario (`delete.php`)

- **Funcionalidad:** Facilita la eliminación de un usuario de la base de datos.
- **Características:** 
  - Eliminación de información de usuario basada en el ID de usuario.

## Conexión a la Base de Datos (`connect.php`)

- **Propósito:** Establece una conexión con la base de datos MySQL.
- **Credenciales:** Utiliza nombre de host, nombre de usuario, contraseña y nombre de la base de datos para la conexión.

## Cómo Ejecutar

1. Clona el repositorio en tu máquina local.
2. Configura un entorno PHP y MySQL (como XAMPP).
3. Crea la base de datos usando phpmyadmin.
4. Ejecuta la aplicación en un servidor local.

## Nota de Seguridad

Esta aplicación es una demostración básica y no implementa medidas avanzadas de seguridad. Es recomendable utilizar declaraciones preparadas (prepared statements) u ORM para las interacciones con la base de datos para prevenir ataques de inyección SQL.

## Validación de entrada de datos:
La validación de entrada de datos es una medida fundamental para prevenir ataques de seguridad como la inyección de SQL, XSS (Cross-Site Scripting) y otros tipos de vulnerabilidades. Algunas prácticas comunes de validación incluyen:

**Validación del lado del cliente:**  Utiliza HTML5 para establecer tipos de datos y atributos de validación en los campos de entrada del formulario, como required, maxlength, minlength, pattern, etc. Esto ayuda a garantizar que los datos ingresados por el usuario cumplan con ciertos criterios antes de enviarlos al servidor.

**Validación del lado del servidor:** Implementa validación adicional en el lado del servidor utilizando lenguajes de programación como PHP. Verifica que los datos recibidos del cliente cumplan con ciertos criterios de formato, longitud y tipo antes de procesarlos o almacenarlos en la base de datos. Esto ayuda a prevenir la inserción de datos maliciosos o inválidos en la aplicación.

**Filtrado y saneamiento de datos:** Además de la validación, aplica técnicas de filtrado y saneamiento de datos para eliminar caracteres especiales, etiquetas HTML o comandos SQL potencialmente peligrosos de los datos ingresados por el usuario. Esto ayuda a prevenir ataques de inyección de código malicioso.

---

Siéntete libre de contribuir a este proyecto o sugerir mejoras. Para cualquier consulta o problema, por favor abre un issue en este repositorio.

