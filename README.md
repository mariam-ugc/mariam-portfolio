# Portfolio Mariam — versión maestra para GitHub

Esta carpeta contiene la web completa preparada para GitHub Pages. No necesita npm, compilación ni servidor: es HTML/CSS/JavaScript estático.

## Qué editar y dónde

- `index.html`: estructura y textos largos de cada acto, servicios, Backstage y formulario.
- `css/styles.css`: todo el diseño, responsive y animaciones.
- `js/content.js`: **primer sitio que debes mirar**. Aquí están los tres proyectos destacados, los tres universos de Creative Storytelling, Utilería y rutas principales de marca.
- `js/main.js`: comportamiento (telón, navegación, carruseles, Backstage, tarifas, bombilla, filtros). Normalmente no hace falta tocarlo para cambiar contenido.
- `assets/`: imágenes actuales. Las carpetas `assets/images/...` y `assets/videos/...` están preparadas para añadir tus fotos y vídeos.

## Añadir fotos reales a Utilería

1. Sube, por ejemplo, `assets/images/utileria/rode.png`.
2. Abre `js/content.js`.
3. En Micrófonos RØDE cambia `image:""` por `image:"assets/images/utileria/rode.png"`.
4. El icono desaparece automáticamente y se muestra la foto.

## Cambiar un proyecto destacado

En `js/content.js`, edita `featuredProductions`. Cada elemento tiene `title`, `type`, `description` y `video`. La estructura visual de los tres teléfonos no se toca.

## Logo y tarifas

Los archivos actuales son `assets/logo-mariam.png` y `assets/tarifas-mariam.png`. Puedes reemplazarlos manteniendo el mismo nombre, o cambiar su ruta en `js/content.js` y en el HTML si corresponde.

## Publicar en GitHub Pages

1. Crea un repositorio nuevo en GitHub (por ejemplo `mariam-portfolio`).
2. Sube **el contenido de esta carpeta**, de forma que `index.html` quede en la raíz del repositorio.
3. En GitHub: **Settings → Pages**.
4. En *Build and deployment*, selecciona **Deploy from a branch**.
5. Branch: `main`; carpeta: `/ (root)`; guarda.
6. GitHub mostrará la URL pública cuando termine el despliegue.

## Cómo trabajar conmigo después

Puedes pasarme el ZIP actualizado o el archivo concreto que quieras cambiar. Para cambios de contenido normalmente bastará `js/content.js`; para diseño, `css/styles.css`; para funcionamiento, `js/main.js`. Así evitamos reescribir toda la web por cada ajuste.

## Nota del formulario

El formulario visual todavía no envía mensajes reales. Hay que conectarlo posteriormente a un servicio de formularios o backend. No se ha simulado un envío real.

## Ajustes finales ya incorporados

- El primer texto del prólogo permanece 1,5 s más antes de transformarse.
- La bombilla decorativa queda en una capa inferior a los teléfonos de «Mis producciones», para que no tape los vídeos ni bloquee interacción.
