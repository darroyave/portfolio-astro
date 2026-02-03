# Dannover Portfolio

Portfolio personal de **Dannover**: desarrollador y fotógrafo. La página principal divide la pantalla en dos mitades: la izquierda para proyectos de **Developer** y la derecha para la galería de **Fotógrafo**, con un diseño inspirado en layouts de showcase a pantalla completa.

## Stack

- **[Astro](https://astro.build)** – Sitio estático
- **[Tailwind CSS](https://tailwindcss.com)** – Estilos (vía `@tailwindcss/vite`)
- **Google Fonts (Syne)** – Tipografía principal

## Estructura del proyecto

```
src/
├── styles/
│   └── global.css          # Estilos globales + Tailwind
└── pages/
    ├── index.astro         # Home: dos paneles (Developer | Fotógrafo)
    ├── developer/
    │   └── index.astro     # Sección Developer
    └── fotografo/
        └── index.astro     # Sección Fotógrafo
```

- **Home:** header fijo, dos paneles a pantalla completa (imagen de fondo + overlay de texto) y footer con barra de progreso.
- **Developer / Fotógrafo:** páginas de sección con navegación de vuelta al inicio.

## Comandos

| Comando        | Acción                    |
|----------------|---------------------------|
| `npm run dev`  | Servidor de desarrollo    |
| `npm run build`| Build estático            |
| `npm run preview` | Vista previa del build |

## Personalización

- **Imágenes de fondo:** sustituir las URLs en `src/pages/index.astro` (o usar imágenes en `public/`).
- **Contenido:** editar los textos y enlaces en cada panel y en las páginas `developer` y `fotografo`.
- **Colores:** las secciones usan acentos emerald (Developer) y violet (Fotógrafo); se pueden cambiar en las clases de Tailwind.
