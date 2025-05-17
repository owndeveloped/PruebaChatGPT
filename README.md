# PruebaChatGPT — App Híbrida con Ionic + Firebase + .NET 8

Este proyecto incluye una aplicación híbrida desarrollada con **Ionic + Angular** y un backend en **.NET 8 Web API**.  
La autenticación se realiza con **Firebase (Google y Facebook)**, y los usuarios tienen roles: `administrador`, `demandante`, `ayudante`.

---

## 📁 Estructura del proyecto

```
PruebaChatGPT/
│
├── frontend/           # App móvil con Ionic + Angular
│
└── backend/            # API REST .NET 8 + Firebase JWT + SQL Server
```

---

## 🔐 Autenticación

- Login con **Google** y **Facebook** usando Firebase Authentication
- Backend .NET valida el JWT de Firebase en cada solicitud
- Validación de **roles de usuario** mediante claims en el token

---

## 🧑‍💻 Requisitos

- Node.js 18+
- Ionic CLI
- Angular CLI
- .NET SDK 8
- Firebase Console (proyecto configurado)
- SQL Server (local o Azure SQL)

---

## 🚀 Instrucciones para desarrollo local

### 1. Clonar el proyecto

```bash
git clone https://github.com/owndeveloped/PruebaChatGPT.git
cd PruebaChatGPT
```

### 2. Frontend

```bash
cd frontend
npm install
ionic serve
```

### 3. Backend

```bash
cd backend
dotnet restore
dotnet run
```

> El backend se conecta a Firebase y valida tokens JWT. Configura tu conexión a SQL Server en `appsettings.json`.

---

## ☁️ Despliegue en Azure

- **Frontend:** Puedes compilar y desplegar en un hosting estático (Firebase Hosting, Vercel, Azure Static Web Apps, etc.)
- **Backend:** Puedes publicar directamente desde Visual Studio o usar Azure CLI para subir la Web API

---

## 🧾 Licencia

MIT © 2025 – Proyecto de ejemplo creado con ChatGPT