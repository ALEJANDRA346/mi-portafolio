# Portfolio Template — Bilingual (ES/EN)

Plantilla de portafolio profesional bilingüe. Una sola página, responsive, con toggle de idioma ES/EN.

Bilingual professional portfolio template. Single page, responsive, with ES/EN language toggle.

## Demo

Ejemplo en vivo / Live example: [juantlapa.github.io](https://juantlapa.github.io)

---

## Quick Start

1. **Fork** este repo o haz clic en "Use this template"
2. Renombra el repo a `tu-usuario.github.io`
3. Edita los archivos (ver instrucciones abajo)
4. Activa GitHub Pages en Settings > Pages > Branch: `main`
5. Tu portafolio estará en `https://tu-usuario.github.io`

---

## Estructura

```
index.html              ← HTML principal + CSS inline
js/main.js              ← Toggle de idioma + navbar + mobile menu
assets/images/foto.jpg  ← Tu foto (reemplazar)
```

---

## Personalizar

### 1. Tu información

En `index.html`, busca los comentarios `<!-- PERSONALIZAR -->` para ubicar las secciones editables:

- **Nombre y tagline** — Hero, Nav, Footer
- **Links** — LinkedIn, GitHub, Email (hero y footer)
- **Foto** — Reemplaza `assets/images/foto.jpg` con tu foto
- **Color** — Cambia `--primary` en `:root` para ajustar toda la paleta

### 2. Contenido bilingüe

El sistema de idiomas funciona de dos maneras:

**Textos cortos** (headings, labels, botones): usan `data-i18n="clave"` en el HTML y se definen en `js/main.js` dentro del objeto `translations`.

```html
<h2 data-i18n="aboutTitle">Sobre mí</h2>
```

**Textos largos** (párrafos, listas): usan dos elementos con `data-lang="es"` y `data-lang="en"`.

```html
<p class="lang-block" data-lang="es">Texto en español</p>
<p class="lang-block" data-lang="en" style="display:none;">English text</p>
```

### 3. Secciones

Cada sección es un `<section>` independiente. Puedes:
- Agregar o quitar secciones completas
- Duplicar `.job-card` para agregar experiencia
- Duplicar `.project-card` para agregar proyectos
- Agregar categorías de habilidades duplicando `.skill-category`

---

## Stack

- HTML5 + CSS3 (inline en `<style>`)
- JavaScript vanilla (ES6+)
- Google Fonts (Inter)
- Sin dependencias, sin frameworks, sin build tools

---

## Licencia

MIT — usa libremente para tu portafolio personal o profesional.
