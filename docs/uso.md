# Uso de la API

La API permite consultar el catálogo de libros.

## Endpoints disponibles

| Método | Ruta             | Descripción                 |
|--------|------------------|-----------------------------|
| GET    | `/api/libros`    | Lista de libros             |
| GET    | `/api/libros/:id`| Libro por identificador     |


## Ejemplos de consulta

**Listar todos los libros**

Consulta que lista todos los libros dentro del JSON.

```
http://localhost:3000/api/libros
```
Respuesta esperada: `202 Ok`

**Obtener un libro por id**

Consulta que lista un libro en concreto por su id.

```
http://localhost:3000/api/libros/1
```
Respuesta esperada: `202 Ok`

**Libro inexistente**

Si el libro no existe, el servidor devuelve HTTP 404.

```
http://localhost:3000/api/libros/999
```
Respuesta esperada: `404 Not found`
