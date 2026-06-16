# cv-site

CV online personal construido con [Astro](https://astro.build).
Diseño minimalista estilo terminal, orientado a perfil técnico IT.

## Setup

```bash
npm install
npm run dev        # dev server en localhost:4321
npm run build      # build estático en dist/
npm run preview    # preview del build
```

## Personalización antes de publicar

Busca y reemplaza en todos los archivos:

- `Nombre Apellido` → tu nombre real
- `tu@email.com` → tu email
- `tuusuario` → tu usuario de GitHub
- `user@lleida` → tu usuario real (opcional, es el prompt del terminal)

### Opcionales
- Descomenta el bloque de Instagram en `src/pages/index.astro` si quieres añadirlo
- Cambia `site` en `astro.config.mjs` a tu URL real para deploy
- Para añadir descarga de PDF: coloca tu CV.pdf en `/public/` y añade un link en el hero

## Deploy

Compatible con GitHub Pages, Netlify, Vercel, Cloudflare Pages.

```bash
# GitHub Pages (via gh-pages)
npm run build
npx gh-pages -d dist
```

## Estructura

```
src/
├── components/
│   ├── ExperienceCard.astro   # Card de experiencia reutilizable
│   └── Section.astro          # Wrapper de sección con label
├── layouts/
│   └── Layout.astro           # Layout principal + nav + footer
├── pages/
│   └── index.astro            # Página principal (todo el contenido)
└── styles/
    └── global.css             # Design tokens y estilos globales
public/
└── favicon.svg
```
