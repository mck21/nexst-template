# 🧪 Nexst Monorepo Template

<p align="center">  
  <img src="https://github.com/mck21/nexst-template/blob/main/public/images/nexst-header.png" />
</p>


---

## 🛠️ Tech Stack

[![Next.js](https://img.shields.io/badge/Next.js-15-black?logo=next.js&style=flat-square)](https://nextjs.org)
[![NestJS](https://img.shields.io/badge/NestJS-E0234E?logo=nestjs&logoColor=white&style=flat-square)](https://nestjs.com)
[![Bun](https://img.shields.io/badge/Bun-1.2.4-ffde57?logo=bun&logoColor=black&style=flat-square)](https://bun.sh)
[![TypeScript](https://img.shields.io/badge/TypeScript-5.8-blue?logo=typescript&style=flat-square)](https://www.typescriptlang.org)
[![Turborepo](https://img.shields.io/badge/Turborepo-monorepo-5c5cff?logo=vercel&style=flat-square)](https://turbo.build)
[![Tailwind CSS](https://img.shields.io/badge/Tailwind_CSS-38B2AC?logo=tailwind-css&logoColor=white&style=flat-square)](https://tailwindcss.com)
[![Prisma](https://img.shields.io/badge/Prisma-2D3748?logo=prisma&logoColor=white&style=flat-square)](https://www.prisma.io)


---

## 📦 Estructura

```
nexst-template/
├── apps/
│   ├── web/          → Frontend (Next.js)
│   ├── api/          → Backend (NestJS)
│   └── docs/         → Documentación (Next.js)
├── packages/
│   ├── ui/           → Componentes UI compartidos
│   ├── eslint-config/→ Configuración ESLint
│   └── typescript-config/ → Configuración TypeScript
├── turbo.json        → Configuración Turborepo
└── package.json      → Configuración raíz y scripts
```

---

## 🚀 Instalación

```bash
# Clonar el repositorio
git clone https://github.com/mck21/nexst-template.git
cd nexst-template

# Instalar dependencias
bun install
```

---

## 🧪 Scripts disponibles

Desde la raíz del proyecto:

```bash
bun run dev         # Levanta frontend (Next.js) y backend (NestJS)
bun run build       # Compila todos los paquetes
bun run lint        # Ejecuta linter en todos los paquetes
bun run format      # Formatea con Prettier
bun run check-types # Verifica tipos TypeScript
```

Puedes también correr los comandos individualmente desde `apps/web` o `apps/api`:

```bash
# Frontend
cd apps/web && bun dev

# Backend (usando npm)
cd apps/api && npm run start:dev

# Documentación
cd apps/docs && bun dev
```

---

## 💡 Requisitos

- **Node.js** >= 18
- **Bun** >= 1.2.4
- **npm** >= 8 (solo si usas npm para el backend)

---

## 📁 Convenciones

- `apps/` contiene las aplicaciones Next.js y NestJS
- `packages/` contiene librerías compartidas entre front y back (ej. ui, config, utils, etc)
- Sigue principios **DDD** y **SOLID** para escalar el proyecto fácilmente

---

## 📌 Notas

- El backend está preparado para trabajar con **npm** por compatibilidad con herramientas que no soportan aún **bun**
- Frontend utiliza **bun** por velocidad y simplicidad
- La estructura está optimizada para desarrollo y producción

---

## 🧙 Autores

Hecho por [@MarcosPalomero](https://github.com/mck21)

---

## 📝 Licencia

MIT © 2025
