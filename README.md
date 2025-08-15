# TodoApp Fullstack — Express + MySQL + React
Proyecto técnico para CRUD de tareas con backend y frontend separados, cumpliendo los requisitos del enunciado.

## Tecnologías
- Backend: Node.js, Express, MySQL, express-validator, CORS, dotenv
- Frontend: React + Vite, Axios
- BD: MySQL

## Estructura
- backend/ — API REST
- frontend/ — UI React
- backend/tasks.sql — Script de BD

## Cómo ejecutar
### 1) Base de datos
- Instala MySQL y ejecuta `backend/tasks.sql` (crea DB `todoapp` y tabla `tasks`).

### 2) Backend
```bash
cd backend
cp .env.example .env   # ajusta credenciales MySQL
npm install
npm run dev            # o npm start
```

### 3) Frontend
```bash
cd frontend
cp .env.example .env   # apunta VITE_API_URL al backend (http://localhost:3000)
npm install
npm run dev
```

### Endpoints REST
- POST /tasks
- GET /tasks
- GET /tasks/:id
- PUT /tasks/:id
- DELETE /tasks/:id
