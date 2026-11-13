# Página personal de Brian Gil

## Descripción

Este sitio presenta a Brian, sus habilidades, los lenguajes que está aprendiendo y su interés en el desarrollo Full Stack. El diseño usa tarjetas y una paleta oscura con tonos azules y morados.

## Archivos

- `index.html`: contiene el contenido de la página y sus estilos CSS dentro de la etiqueta `<style>`.
- `imagen/foto-perfil.png.jpg`: fotografía que aparece en la presentación.

## Cómo ver el sitio

Abre el archivo `index.html` en un navegador web. No se necesitan instalar programas ni dependencias.

## Orden del código

El HTML está organizado así: datos de la página en `<head>`, estilos en `<style>` y contenido visible en `<body>`. Dentro del contenido aparecen primero la presentación, después la información personal y las tarjetas, y al final el pie de página.

El CSS sigue un orden simple: colores compartidos, reglas generales, estilos de la presentación y las tarjetas, estados interactivos y, al final, ajustes para pantallas pequeñas y movimiento reducido.

## Etiquetas HTML utilizadas

| Etiqueta | Explicación sencilla |
| --- | --- |
| `<!DOCTYPE html>` | Indica al navegador que el documento usa HTML moderno. |
| `<html lang="es">` | Contiene toda la página e indica que su idioma es español. |
| `<head>` | Guarda información y configuraciones que no aparecen como contenido principal. |
| `<meta>` | Define datos como los caracteres, la adaptación al tamaño de pantalla y la descripción. |
| `<title>` | Define el nombre que aparece en la pestaña del navegador. |
| `<style>` | Contiene las reglas CSS que dan estilo a la página. |
| `<body>` | Contiene todo lo que se muestra en la página. |
| `<div>` | Agrupa elementos para organizarlos y aplicarles estilos. |
| `<header>` | Agrupa la presentación principal de Brian. |
| `<main>` | Agrupa el contenido principal de la página. |
| `<section>` | Separa el contenido en secciones relacionadas. |
| `<article>` | Representa una tarjeta de contenido independiente. |
| `<footer>` | Muestra el pie de página. |
| `<h1>` | Es el título principal de la página. |
| `<h2>` | Es un título para una sección o tarjeta. |
| `<p>` | Muestra un párrafo de texto. |
| `<strong>` | Resalta una palabra o frase importante. |
| `<img>` | Muestra la foto de perfil. |
| `<ul>` | Crea una lista sin números. |
| `<li>` | Representa un elemento de una lista. |
| `<span>` | Agrupa una parte corta del texto para destacarla o darle estilo. |
| `<a>` | Crea un enlace; en esta página lleva al perfil de GitHub y sus repositorios. |

## Atributos HTML importantes

- `class`: conecta un elemento con sus estilos CSS; varias tarjetas pueden compartir la misma clase.
- `id`: da un nombre único a una sección, usado aquí para relacionarla con su título.
- `src`: indica dónde está el archivo de imagen.
- `alt`: describe la imagen para lectores de pantalla o cuando la imagen no carga.
- `href`: contiene la dirección del enlace de GitHub.
- `target="_blank"`: abre el enlace en otra pestaña.
- `rel="noopener noreferrer"`: añade una protección al abrir un enlace en otra pestaña.
- `aria-labelledby` y `aria-label`: ofrecen nombres comprensibles de las secciones y otros elementos a tecnologías de asistencia.
- `aria-hidden="true"`: evita que el símbolo de flecha decorativo se lea como contenido.

## Clases CSS

Las clases se escriben en el HTML con `class="..."` y se seleccionan en CSS con un punto, por ejemplo `.card`.

| Clase | Uso |
| --- | --- |
| `.page-shell` | Centra el contenido y limita su ancho. |
| `.hero` | Da formato al bloque de presentación. |
| `.hero-copy` | Agrupa y ordena el texto de presentación. |
| `.profile-photo` | Ajusta el tamaño y la forma circular de la foto. |
| `.eyebrow` | Estiliza el texto pequeño que acompaña a un título. |
| `.hero-description` | Da estilo a la descripción bajo el nombre. |
| `.section-heading` | Da estilo a los títulos de las secciones. |
| `.about` | Ajusta el texto de presentación personal. |
| `.cards` | Organiza las tarjetas en una cuadrícula. |
| `.card` | Da formato visual a cada tarjeta. |
| `.card-label` | Estiliza la etiqueta pequeña que aparece arriba del título de una tarjeta. |
| `.skill-list` | Organiza las habilidades en una lista flexible. |
| `.languages` | Organiza las etiquetas de lenguajes. |
| `.language-tag` | Da formato a las etiquetas JavaScript y Python. |
| `.card-copy` | Da estilo al texto descriptivo de las tarjetas. |
| `.github-link` | Da estilo al enlace del perfil de GitHub. |

## CSS en palabras simples

En cada regla CSS, el **selector** indica qué elemento se va a cambiar y las **propiedades** indican qué aspecto tendrá. Por ejemplo, `.card` selecciona las tarjetas y sus propiedades controlan el fondo, el espacio interior y los bordes.

### Selectores y reglas

- `:root` define variables de colores compartidas por toda la página.
- `*` selecciona todos los elementos; se usa para que el tamaño incluya el espacio interior y los bordes.
- `body`, `a`, `h1`, `h2`, `p` y `footer` seleccionan etiquetas HTML directamente.
- `.clase` selecciona los elementos que tienen esa clase.
- `.card h2` selecciona los títulos `<h2>` que están dentro de una tarjeta.
- Las comas permiten aplicar una misma regla a varios selectores.
- `:hover` cambia el aspecto al pasar el cursor sobre un elemento.
- `:focus-visible` resalta un enlace cuando se llega a él con el teclado.
- `::after` agrega un adorno visual a la presentación sin añadir contenido al HTML.
- `@media (max-width: 640px)` adapta la distribución a pantallas pequeñas.
- `@media (prefers-reduced-motion: reduce)` reduce las transiciones para quienes prefieren menos movimiento.

### Propiedades y técnicas principales

- `--background`, `--text`, `--electric`, `--pastel`, `--intense` y `--purple` guardan los colores usados por el diseño. Se consultan con `var(--nombre)`.
- `var()`, `rgb()`, `min()` y `clamp()` son funciones CSS: reutilizan variables, definen colores con transparencia y ajustan tamaños a la pantalla.
- `color-scheme` indica al navegador que el diseño es oscuro; `color`, `background` y `border-color` definen colores de texto, fondos y bordes.
- `font-family`, `font-size`, `font-weight`, `font-style`, `line-height`, `letter-spacing` y `text-transform` controlan la apariencia y lectura del texto.
- `width`, `min-width`, `max-width`, `height` y `min-height` controlan tamaños.
- `margin` crea espacio exterior; `padding` crea espacio interior.
- `display: flex`, `flex-direction`, `flex-wrap`, `flex: 0 0 auto` y `align-items` acomodan elementos en filas o columnas y controlan su alineación.
- `display: grid` y `grid-template-columns` organizan las tarjetas en columnas; en móviles pasan a una columna.
- `gap` define el espacio entre elementos flexibles o columnas.
- `border`, `border-radius` y `box-shadow` crean bordes, esquinas redondeadas y sombras.
- `linear-gradient` y `radial-gradient` crean fondos con degradados de color.
- `object-fit: cover` ajusta la imagen al espacio sin deformarla.
- `transition` suaviza el cambio visual al interactuar con una tarjeta o un enlace.
- `transform` mueve ligeramente la tarjeta al pasar el cursor; `transition-duration` regula la duración de los cambios.
- `text-decoration` y `text-underline-offset` controlan el subrayado de los enlaces.
- `position`, `top`, `right`, `z-index`, `overflow` y `pointer-events` permiten ubicar, superponer y recortar el adorno decorativo.
- `box-sizing` hace más predecible el cálculo de tamaños; `list-style` controla las viñetas de la lista.
- `scroll-behavior` controla el desplazamiento y `!important` hace que esa regla de movimiento reducido tenga prioridad.

## JavaScript

Esta página no usa JavaScript. El contenido y el diseño están hechos con HTML y CSS.
