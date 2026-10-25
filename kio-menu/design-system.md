# KIO MENÚ — Implementación de KIO VISUAL DNA

KIO MENÚ es la primera referencia práctica de KIO VISUAL DNA, en modo **Pixel Hybrid con presencia de Pixel Adventure**.

## Aplicación del estándar
- Paleta cálida con bosque, crema y ámbar.
- Tipografía de interfaz de sistema y titulares pixelados.
- Bordes definidos, cuadrícula y sombras duras.
- Sprites de comida y progreso como misiones.
- Interacción táctil y layout adaptado a móvil.
- La receta, el inventario y los costos siguen siendo el centro; el juego no oculta la información práctica.

## Biblioteca reutilizable
- `kio-visual-dna.css`: tokens y primitivas compartidas.
- `icon.svg`: icono PWA.
- `index.html`: aplicación de referencia.
- `manifest.webmanifest` y `sw.js`: instalación y caché offline.

## Reutilizar en otro proyecto
Copiar `kio-visual-dna.css`, cargarlo antes de los estilos propios, y usar solo tokens/clases que se necesiten. Para un proyecto de cliente, conservar su marca y aplicar únicamente los principios compatibles.

## Límite de esta versión
La biblioteca es v1.0 inicial y usa CSS nativo. KIO MENÚ es una implementación de referencia, no una auditoría integral de accesibilidad ni una prueba de compatibilidad con todos los navegadores.
