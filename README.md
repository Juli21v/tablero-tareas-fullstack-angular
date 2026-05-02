# Proyecto final BIT — Tablero de tareas (full stack)

Aplicación de **gestión de tareas tipo tablero** desarrollada como proyecto integrador de bootcamp: autenticación, roles, tableros y archivos. Combina un **frontend en Angular** con **backend en Node.js** y **MongoDB**.

**Autora del repositorio:** [@Juli21v](https://github.com/Juli21v)

## Stack

| Capa | Tecnologías |
|------|-------------|
| Frontend | Angular 13, Angular Material, Angular Flex Layout, RxJS |
| Backend | Node.js, Express, Mongoose, JWT, bcrypt, Nodemailer |
| Datos | MongoDB |

## Funcionalidades (resumen)

- Registro e inicio de sesión de usuarios con JWT
- Gestión de **roles** y **usuarios** (rutas de administración)
- **Tableros / tareas** (boards) con operaciones vía API
- Carga de archivos (multipart) y carpeta estática `uploads`
- Colección **Postman** incluida para probar el API: `TeamBoardBackFinish.postman_collection.json`

## Estructura del repositorio

```
Proyecto-Final-BIT/
├── frontend/                 # Aplicación Angular
│   ├── src/app/
│   │   ├── home/            # Login, registro, cabecera, pie
│   │   ├── board/           # Alta y listado de tareas
│   │   └── admin/           # Roles y usuarios
│   └── package.json
├── backend/
│   ├── index.js             # Servidor Express y rutas /api/*
│   ├── routes/              # role, user, board
│   ├── models/              # Mongoose
│   ├── middlewares/         # auth, admin, validación, archivos
│   ├── db/db.js             # Conexión MongoDB
│   └── package.json
└── TeamBoardBackFinish.postman_collection.json
```

## Requisitos

- Node.js y npm
- MongoDB en ejecución
- Angular CLI (para el frontend), alineado con la versión del `package.json` del frontend

## Puesta en marcha

### Backend

```bash
cd backend
cp .env.example .env
# Edita .env: PORT, DB_CONNECTION, SK_JWT (secreto para firmar tokens)
npm install
npm start
```

### Frontend

```bash
cd frontend
npm install
ng serve
```

Abre el navegador en la URL que indique Angular (habitualmente `http://localhost:4200`).

## Enlace útil

- [Perfil de GitHub — Juli21v](https://github.com/Juli21v)
