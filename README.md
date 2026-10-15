# Blog con Jekyll y GitHub Pages

## Qué incluye
- Portada con 10 artículos por página y paginación.
- Página HTML independiente por artículo.
- Archivo cronológico completo.
- Categorías visibles en cada publicación.
- Feed Atom, metadatos SEO y diseño adaptable a móviles.
- Plantillas reutilizables.

## Publicar un artículo
Crea un archivo en `_posts/` con el formato `AAAA-MM-DD-titulo-del-articulo.md`. Incluye al principio:

---
title: "Título del artículo"
date: 2026-10-16 09:00:00 -0400
categories: [cultura, historia]
author: "Redacción"
description: "Resumen breve para buscadores."
---

Después escribe el contenido en Markdown y sube el archivo al repositorio.

## Configurar GitHub Pages
1. Sube el contenido de esta carpeta a la raíz del repositorio.
2. Edita `_config.yml`: cambia `title`, `description` y `url` por los datos reales. Mantén `baseurl: ""` si usas un subdominio o dominio propio.
3. En Settings → Pages, selecciona la fuente GitHub Actions si vas a usar el workflow oficial de Jekyll, o la rama `main` si GitHub Pages admite la construcción elegida.
4. GitHub Pages admite Jekyll y `jekyll-paginate`. Si seleccionas GitHub Actions, configura un workflow de Jekyll con `actions/jekyll-build-pages` y `actions/deploy-pages`.

## Nota
El archivo de ejemplo sirve para comprobar el diseño; elimínalo cuando publiques contenido real. La paginación requiere el plugin `jekyll-paginate`, compatible con la construcción de GitHub Pages.
