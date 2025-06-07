# Pruebas de la API REST con Postman

### Crear un nuevo video
- **Metodo:** PUT
- **URL de la peteción:** http://localhost:5000/api/videos/30
- **Petición:**
```Json
{
  "name": "Prueba de metodo PUT",
  "views": 0,
  "likes": 0
}
```
- **Respuesta esperada:**
```Json
{
    "id": 30,
    "name": "Prueba de metodo PUT",
    "views": 0,
    "likes": 0
}
```
- **Código de estado:** 200 OK

#

### Obtener un video
- **Metodo:** GET
- **URL:** http://localhost:5000/api/videos/30
- **Respuesta esperada:** 
```Json
{
    "id": 30,
    "name": "Prueba de metodo PUT",
    "views": 0,
    "likes": 0
}
```
- **Código de estado:** 200 OK

#

### Actualizar un video
- **Metodo:** PATCH
- **URL:** http://localhost:5000/api/videos/30
- **Actualización:** 
```Json
{
  "views": 100,
  "likes": 20
}
```
- **Respuesta esperada:**
```Json
{
    "id": 30,
    "name": "Prueba de metodo PUT",
    "views": 100,
    "likes": 20
}
```
- **Código de estado:** 200 OK

#

### Eliminar un video
- **Metodo:** DELETE
- **URL:** http://localhost:5000/api/videos/30
- **Respuesta esperada:** Nada
- **Código de estado:** 204 No Content (Sin cuerpo de respuesta).
