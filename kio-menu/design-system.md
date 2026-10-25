# KIO MENÚ v0.2 — KIO VISUAL DNA en práctica

KIO MENÚ es la primera referencia práctica de KIO VISUAL DNA. Esta versión usa **Pixel Hybrid** para controles y lectura, con **Pixel Adventure** para el mundo, las misiones y la exploración.

## Dirección visual adoptada
- **Mapa del día:** un valle ilustrado conecta desayuno, almuerzo, comida y cena. Los nodos son botones reales, no parte de una captura decorativa.
- **Cocina explorable:** escena de cocina detallada antes del inventario de objetos/ingredientes.
- **Recetario:** ilustraciones pixeladas de alimentos, ingredientes disponibles/faltantes y pasos legibles.
- **Ruta del día:** muestra progreso real, cambio individual de receta y una lista de faltantes.
- **Paleta:** bosque, crema, ámbar, cielo y coral. Los colores son tokens, no reglas inamovibles.
- **Composición:** escenarios con detalle visual, pero los controles conservan jerarquía, contraste y áreas táctiles cómodas.
- **Multiplataforma:** interfaz responsive y PWA para Android, iPhone e iPad.

## Reglas de interacción
1. El mapa funciona como navegación visual: cada parada abre o descubre una comida.
2. Cambiar una misión no debe borrar las demás.
3. Los controles con gestos deben tener equivalentes visibles.
4. Las cantidades de inventario se editan explícitamente; la aplicación no supone que una lista de compras equivale a existencia real.
5. Una misión marcada como completa representa una acción del usuario, no una estimación del sistema.
6. La app puede compartirse por enlace, pero las despensas permanecen locales y no se sincronizan entre familiares.
7. Los costos son aproximaciones por porción y deben rotularse como tales.

## Biblioteca reutilizable
- `kio-visual-dna.css`: tokens de color, tipografía, espacio y primitivas.
- `index.html`: mapa, cocina, despensa, recetario, ajustes y lógica local.
- `apple-touch-icon.png`: icono dedicado para la pantalla de inicio de iOS.
- `icon.svg`: favicon / icono vectorial de la PWA.
- `manifest.webmanifest`: identidad e iconos de instalación.
- `sw.js`: caché offline versionada.
- `README.md`: funciones, límites e instrucciones de instalación.

## Instalación
- **Android:** abrir el enlace en Chrome y usar “Instalar aplicación” o “Agregar a pantalla de inicio”.
- **iPhone/iPad:** abrir en Safari, pulsar “Compartir” → “Añadir a pantalla de inicio” y habilitar “Abrir como app web” si aparece.
- Cada dispositivo mantiene su propio inventario. Compartir la URL no comparte datos ni crea sincronización.

## Criterios de revisión
- El mapa debe leerse como paisaje y ruta, no como una cuadrícula de tarjetas.
- El pixel art debe tener profundidad, luz y detalles; el detalle nunca debe reducir legibilidad.
- Debe ser fácil generar el menú y reemplazar una sola comida.
- El presupuesto y las existencias deben estar claramente diferenciados.
- El flujo principal debe revisarse en teléfonos reales; el código o un simulador no sustituyen esa prueba.
- Confirmar carga de hoja CSS, icono de iOS y caché actualizada tras publicar.

## Límite
El motor culinario de v0.2 usa reglas locales y recetas predeterminadas, no IA generativa. El costo es orientativo. La PWA está diseñada para ambas plataformas, pero su comportamiento debe confirmarse en iPhone y Android reales antes de considerarla validada en todos los dispositivos.

## Detalle de ilustración y autoría
- Las recetas y el resumen del día usan ilustraciones pixel art de platos, con textura, contraste y detalle mayores que los pictogramas pequeños de ingredientes.
- Los pictogramas del inventario siguen siendo más simples a propósito: su objetivo es reconocimiento rápido y control de cantidades, no decoración.
- Firma visual discreta: **“Una creación de KioRafa × ChatGPT”**; los créditos ampliados de Ajustes explican que KioRafa aporta concepto y dirección creativa, y ChatGPT participa en diseño e implementación.


## KIO VISUAL DNA v1.2 — Ilustración culinaria con detalle
- **Emblema:** el icono de KIO MENÚ muestra un plato ilustrado con distintos alimentos, brillos, capas y textura pixelada; el PNG de 180×180 es el icono de inicio de iOS y el SVG se utiliza en navegador/PWA.
- **Ingrediente reconocible:** cada alimento de despensa debe tener una silueta y un conjunto de detalles propios (piel, hojas, granos, cáscara, etiqueta, corte o textura). No reciclar un glifo genérico para distintos productos salvo ingredientes desconocidos, que usan la ilustración de temporada como respaldo.
- **Platos:** se muestran ilustraciones por familia de receta; arroz, quesadillas, pasta, papa, tostadas y enfrijoladas tienen escenas propias, y las ilustraciones existentes se reutilizan cuando son semánticamente adecuadas.
- **Cocina y mapa:** las escenas deben parecer espacios habitables de un juego 16/32-bit, con planos de profundidad, luz, sombras, objetos pequeños y materiales identificables.
- **Color:** verdes profundos de entorno; crema para porcelana/masa; ámbar para dorado y bordes; rojo tomate; verdes claros para hojas. Usar contraste suficiente para que el alimento siga siendo reconocible en tarjetas pequeñas.
- **Interfaz:** conservar tamaños táctiles, texto legible y jerarquía de navegación. La ilustración puede ser rica sin convertir cada control en un objeto visual recargado.
- **Créditos:** la firma se presenta como **KIO × RAFA**, visible pero discreta. Evitar promocionar nombres de herramientas como si fueran autores del producto.
