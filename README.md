# 🐒 III Congreso Peruano de Primatología 2026

Sitio web oficial del **I Congreso Peruano de Primatología 2026**, construido con Astro + TailwindCSS y desplegado en GitHub Pages.

[![Deploy to GitHub Pages](https://github.com/tuusuario/congreso-primatologia-2026/actions/workflows/deploy.yml/badge.svg)](https://github.com/tuusuario/congreso-primatologia-2026/actions/workflows/deploy.yml)

🌐 **Demo:** https://tuusuario.github.io/congreso-primatologia-2026/

---

## 🌿 Stack Tecnológico

| Componente | Tecnología |
|---|---|
| Framework | Astro 4.x |
| Estilos | TailwindCSS 4.x |
| Contenido | JSON + Markdown |
| Deploy | GitHub Pages via Actions |
| Fuentes | Google Fonts (Playfair Display + Manrope + Inter) |

---

## 🚀 Inicio rápido

### Requisitos
- Node.js v22+
- npm v10+

### Instalación y desarrollo local

```bash
# Instalar dependencias
npm install

# Iniciar servidor de desarrollo
npm run dev
```

El sitio estará disponible en `http://localhost:4321/congreso-primatologia-2026/`

---

## 📁 Estructura del Proyecto

```
/
├── .github/workflows/deploy.yml   # Deploy automático GitHub Pages
├── public/favicon.svg
├── src/
│   ├── components/layout/         # Header, Footer
│   ├── components/home/           # Hero, Welcome, Objectives, etc.
│   ├── data/                      # Archivos JSON editables ✏️
│   │   ├── site.json              # Config global
│   │   ├── objectives.json        # Objetivos
│   │   ├── thematic-axes.json     # Ejes temáticos
│   │   ├── important-dates.json   # Fechas importantes
│   │   ├── partners.json          # Aliados
│   │   └── pricing.json           # Inscripciones y precios
│   ├── layouts/                   # BaseLayout, PageLayout
│   ├── pages/                     # 9 páginas
│   └── styles/global.css          # Design system
├── astro.config.mjs
└── README.md
```

---

## ✏️ Editar contenido (sin código)

### Datos del congreso → `src/data/site.json`
Nombre, fechas, ciudad, email de contacto, redes sociales.

### Fechas importantes → `src/data/important-dates.json`
Agrega objetos con: `date`, `label`, `title`, `description`, `type` (open/deadline/notification/event).

### Aliados → `src/data/partners.json`
Cada aliado: `name`, `acronym`, `type` (organizer/academic/government/partner), `url`.

### Precios → `src/data/pricing.json`
Categorías con precios early bird, regular y en sede.

---

## 🚢 Deploy en GitHub Pages

1. **Edita `astro.config.mjs`** con tu usuario:
```js
site: 'https://TU-USUARIO.github.io',
base: '/congreso-primatologia-2026',
```

2. En GitHub → **Settings → Pages → Source: GitHub Actions**

3. Push a `main` → deploy automático ✅

---

## 🎨 Personalizar colores

En `src/styles/global.css`, cambia las variables:

```css
:root {
  --forest-leaf:   #52b788;   /* Color principal */
  --gold:          #c9a84c;   /* Acento dorado */
  --forest-dark:   #1a3a2e;   /* Fondo oscuro hero */
}
```

---

## 📧 Formulario de contacto

Edita la action en `src/pages/contacto.astro`:
```html
<form action="https://formsubmit.co/TU@EMAIL.COM" method="POST">
```

---

*"Conectando ciencia, conservación y comunidades para el futuro de los primates del Perú"* 🌿🐒
