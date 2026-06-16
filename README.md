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

## Deploy

Compatible con GitHub Pages, Netlify, Vercel, Cloudflare Pages.

```bash
# Via Netlify
npm run build
git add .
git commit -m "Comentario"
git push
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
│   └── index.astro            # Página principal
└── styles/
    └── global.css             # Design tokens y estilos globales
public/
└── favicon.svg
└── cv.pdf
```
