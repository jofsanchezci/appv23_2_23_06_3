
# AE-UPN App v2.3

Este proyecto es una aplicación web moderna construida con **Next.js 13+**, utilizando el nuevo enrutamiento basado en directorios (`/app`), junto con **TypeScript**, **TailwindCSS**, y API Routes para manejar solicitudes del backend. Representa un sistema de acompañamiento institucional para estudiantes universitarios.

---

## Tecnologías utilizadas

- **Next.js 13+** con `App Router`
- **TypeScript**
- **TailwindCSS**
- **API Routes (integradas)**
- **pnpm** como gestor de paquetes
- Posible integración Python (`app.py`) para funcionalidades externas

---

## Estructura del proyecto

```
├── app/                        # Sistema de rutas y vistas principales
│   ├── layout.tsx             # Layout base
│   ├── page.tsx               # Página principal (inicio)
│   ├── globals.css            # Estilos globales (TailwindCSS)
│   ├── consultar/             # Página de consulta de datos
│   ├── registrar/             # Página de registro
│   ├── ayuda/                 # Página de ayuda
│
├── app/api/                   # Rutas API para backend
│   ├── auth/                  # Módulo de autenticación
│   ├── login/logout/me/       # Rutas relacionadas con sesión
│   ├── estudiante/[id]/       # Ruta dinámica para estudiante
│   ├── buscar/atenciones/     # Consultas y acciones del sistema
│   └── reportes/              # Generación y acceso a reportes
│
├── components.json            # Configuración de componentes
├── next.config.mjs            # Configuración de Next.js
├── package.json               # Dependencias del proyecto
├── pnpm-lock.yaml             # Bloqueo de dependencias
├── postcss.config.mjs         # Configuración para PostCSS
├── tailwind.config.ts         # Configuración de TailwindCSS
├── tsconfig.json              # Configuración de TypeScript
├── middleware.ts              # Middleware para protección de rutas
├── app.py                     # Integración posible con Python
```

---

##  Cómo ejecutar la aplicación

1. Asegúrate de tener instalado:

   - Node.js (v18 o superior)
   - pnpm: [`npm install -g pnpm`](https://pnpm.io/installation)

2. Instala las dependencias:

```bash
pnpm install
```

3. Ejecuta el servidor de desarrollo:

```bash
pnpm dev
```

4. Accede a:

```
http://localhost:3000
```

---

## ✨ Funcionalidades clave

- Interfaz moderna y responsiva
- Registro y consulta de atenciones a estudiantes
- Generación de reportes institucionales
- Gestión de sesiones y autenticación integrada
- Modularidad para mantenimiento y escalabilidad

---

## Nota

El archivo `app.py` sugiere que puede existir una integración externa (por ejemplo, generación de documentos o análisis con Python), aunque no forma parte directa del entorno Next.js.

---

## Requisitos

- Node.js 18+
- pnpm
- Navegador moderno

---
## Autor
 - Cristina Rueba
 - correo: ccruedab@upn.edu.co
