# Study Planner Backend

Backend del proyecto final **Study Planner**, una aplicacion CRUD para organizar tareas de estudio.

La API esta hecha con **Node.js**, **Express** y **MongoDB Atlas** usando **Mongoose**.

## Funcionalidades

- Crear tareas
- Ver todas las tareas
- Ver una tarea por su id
- Editar tareas
- Eliminar tareas

Cada tarea puede tener:

- `title`
- `description`
- `priority`
- `status`
- `dueDate`

## Tecnologias usadas

- Node.js
- Express
- MongoDB Atlas
- Mongoose
- dotenv
- cors

## Instalacion

1. Clonar el repositorio
2. Entrar en la carpeta del proyecto
3. Instalar dependencias

```bash
npm install
```

## Variables de entorno

Hay que crear un archivo `.env` con este formato:

```env
PORT=4000
MONGODB_URI=tu_uri_de_mongodb
```

## Ejecutar el proyecto

Modo desarrollo:

```bash
npm run dev
```

Modo normal:

```bash
npm start
```

El servidor se ejecuta por defecto en:

```txt
http://localhost:4000
```

## Endpoints principales

- `GET /api/tasks` -> obtener todas las tareas
- `GET /api/tasks/:id` -> obtener una tarea concreta
- `POST /api/tasks` -> crear una tarea
- `PUT /api/tasks/:id` -> actualizar una tarea
- `DELETE /api/tasks/:id` -> eliminar una tarea

## Ejemplo de body para crear una tarea

```json
{
  "title": "Preparar entrega final",
  "description": "Terminar backend y frontend",
  "priority": "high",
  "status": "pending",
  "dueDate": "2026-04-05"
}
```

## Estado del proyecto

Actualmente el backend funciona en local y esta conectado a MongoDB Atlas.

Cuando el proyecto este desplegado, aqui se puede añadir la URL publica del backend.
