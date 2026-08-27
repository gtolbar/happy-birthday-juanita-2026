# happy-birthday-juanita-2026

Página de cumpleaños e invitación a cena. Un solo archivo, sin dependencias ni build.

## Cómo verla

Abre `index.html` en cualquier navegador, o publícala con GitHub Pages
(*Settings → Pages → Source: Deploy from a branch → main / root*).

## Cómo cambiar la hora de la cena

La hora por defecto es el **1 de septiembre de 2026 a las 8:00 p. m.** (hora de Bogotá, UTC−5).

- **Por URL, sin tocar código:** agrega `?hora=21:30` al final del link.
- **En el código:** en `index.html`, busca `var HOUR = 20, MIN = 0;` y cámbialo.

## Detalles

- Diseño mobile-first; los `@media (min-width)` agrandan para tablet y escritorio.
- La cuenta regresiva marca horas, minutos y segundos. Al llegar a cero se
  revela el mensaje de cumpleaños con confeti.
- **Modo prueba:** 5 toques seguidos al gif adelantan la página al estado
  "ya es la hora". Otros 5 la devuelven a la cuenta regresiva.
- Se adapta al tema claro u oscuro del celular.
- El espacio del gif se llena poniendo la ruta en `GIF_SRC`, al inicio del `<script>`.
- La carta vive dentro de un cuaderno de aventuras que se abre al tocar la
  portada y se escribe línea por línea. Sus fotos van en `BOOK_PHOTOS`
  (entre 2 y 4; con `src` vacío queda el espacio marcado).
- Hay una galería de fotos lista pero desactivada: se activa llenando el
  arreglo `PHOTOS`, al lado de `GIF_SRC`.
