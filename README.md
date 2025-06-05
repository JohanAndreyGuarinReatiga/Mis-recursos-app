# MisRecursosApp

## Descripción

MisRecursosApp permite a los usuarios llevar un registro personalizado de sus series, películas y libros. Los usuarios pueden agregar, modificar, eliminar y consultar sus recursos favoritos, así como filtrarlos y buscar por nombre. La aplicación está diseñada para organizar y hacer seguimiento del progreso y valoración de cada recurso.

---

## Generalidades

- La base de datos está diseñada en MongoDB y consta de dos colecciones principales:
  - `Clientes`: almacena información de los usuarios registrados.
  - `Recursos`: contiene los registros de series, películas y libros asociados a cada usuario.
  
- Cada recurso está relacionado con un usuario mediante el campo `IdUsuario`.

- Se implementan operaciones CRUD (Crear, Leer, Actualizar, Eliminar).

- Se pueden aplicar filtros por estado, formato y plataforma, además de una búsqueda por nombre del recurso.

---

## Comandos para crear la base de datos y colecciones en MongoDB

Ejecutar los siguientes comandos:

```js
// Seleccionar o crear la base de datos MisRecursosApp
use MisRecursosApp

// Crear la colección Clientes
db.createCollection("Clientes")

// Crear la colección Recursos
db.createCollection("Recursos")
