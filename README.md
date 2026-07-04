# El Sitio Del Blog

Ejercicio de curso (AD-07-1) que consiste en construir un sitio de blog estático de 3 páginas enlazadas (Home, About Us, Contact Us) usando solo HTML y CSS, siguiendo el "Bad Template" dado como guía de diseño (ver [instructions.md](instructions.md) y [Pic/Bad_Template.jpg](Pic/Bad_Template.jpg)).

Este proyecto es la base sobre la que luego se hizo el refactor a Bootstrap en el repositorio [Refactorizacion-SitioDelBlog](https://github.com/rtkaleb/Refactorizacion-SitioDelBlog).

## Tech stack

- HTML5 / CSS3 puro (sin frameworks ni dependencias)

## Estructura del proyecto

```
elSitioDelBlog/
├── homePage.html      # Home — navbar sticky, imagen, texto de ejemplo
├── aboutMe.html         # About Us — información del equipo
├── contactMe.html        # Contact Us — formulario de contacto e info
├── style.css              # Hoja de estilos única usada por las 3 páginas
├── script.js               # Vacío (sin lógica de JS)
└── Pic/Bad_Template.jpg    # Wireframe/plantilla de referencia para el diseño
```

## Cómo verlo localmente

No requiere instalación ni build: son archivos estáticos.

```bash
open homePage.html
```

O ábrelo con un servidor local (por ejemplo, la extensión Live Server de VS Code).

## Problema conocido

`aboutMe.html` y `contactMe.html` usan clases de **Bootstrap** (`container`, `row`, `col-md-6`, `btn btn-dark`, `img-fluid`, etc.) pero el proyecto no incluye el CDN de Bootstrap ni esas clases están definidas en `style.css`. Por lo tanto esas dos páginas no se ven como se espera; solo `homePage.html` usa exclusivamente las clases propias definidas en `style.css`.

## Autor

**Kaleb Torres**
