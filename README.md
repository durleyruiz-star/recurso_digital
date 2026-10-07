# Los Animales de la Granja

Recurso digital para preescolar, adaptado para estudiantes con baja visión: canción cantada por partes, imágenes grandes, alto contraste, tamaño de letra ajustable, lectura en voz alta de los movimientos y el juego «¿Quién suena?».

## Ver el recurso

Enlace público: https://durleyruiz-star.github.io/recurso_digital/
Al abrirlo directamente desde el computador (doble clic), el navegador puede bloquear los audios; usa el enlace de GitHub Pages.

## Estructura

```
index.html              Página del recurso
assets/img/             Ilustraciones (figuras 1 a 6)
assets/audio/cancion.mp3  Canción cantada completa
assets/audio/*.mp3      Sonidos de gallo, cerdo, vaca y oveja
```

## Ajustar dónde empieza cada parte de la canción

En `index.html`, busca `const TRAMOS`. Cada parte tiene tres números en segundos:

- `ini`: dónde empieza la parte.
- `voz`: dónde empieza a cantar (sirve para resaltar la letra).
- `fin`: dónde termina.

Ejemplo: si el verso del cerdo empieza en el segundo 17,5, cambia `v2: {ini:17.2, ...}` por `v2: {ini:17.5, ...}` y el `fin` de `v1` también a `17.5`.
