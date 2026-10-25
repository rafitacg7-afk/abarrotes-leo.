# KIO MENÚ v0.2 — Tu cocina, tu aventura

Aplicación web progresiva (PWA) con pixel art detallado y navegación tipo expedición culinaria.

## Dirección de diseño
- **Mapa del día:** cuatro paradas interactivas, una por cada momento de comida.
- **Cocina explorable:** inventario visual con cantidades editables.
- **Recetario de descubrimientos:** ingredientes, pasos, tiempos, costos estimados y faltantes.
- **Ruta del día:** cambiar un plato sin regenerar los demás y marcar misiones completas.
- **KIO VISUAL DNA:** Pixel Hybrid con elementos de Pixel Adventure.
- Diseño responsive, pensado para Android, iPhone y tabletas.

## Funciones v0.2
- Inventario local editable, búsqueda y filtros por categoría.
- Generador heurístico con modos ahorro, balance, explorador y exprés.
- Presupuesto orientativo para ingredientes faltantes.
- Ajuste para no depender de conservar sobras refrigeradas.
- Recetas y alternativas por comida.
- Lista de faltantes para compartir.
- Exportación JSON de respaldo.
- Compartir enlace y listas con el mecanismo nativo cuando esté disponible.
- Caché básica para abrir la aplicación sin conexión después de la primera carga.

## Instalación en dispositivos
### Android
1. Abre el enlace en Chrome.
2. En el menú del navegador, elige **Instalar aplicación** o **Agregar a pantalla de inicio**.

### iPhone / iPad
1. Abre el enlace en Safari.
2. Toca **Compartir**.
3. Elige **Añadir a pantalla de inicio**.
4. Activa **Abrir como app web** si aparece y toca **Añadir**.

La disponibilidad de la opción depende de la versión del sistema y del navegador. No requiere cuenta de desarrollador ni publicación en App Store para usarse de esta manera.

## Datos y privacidad
El inventario, la ruta y las preferencias se guardan en el almacenamiento local del navegador/dispositivo. No hay cuenta de usuario ni sincronización entre integrantes de la familia. Compartir el enlace no comparte el inventario.

## Límites conocidos
- El motor de menús se basa en reglas deterministas con algo de variación, no en un modelo de IA.
- Los costos son aproximados por porción, no precios de paquetes ni una cotización de tienda.
- El inventario inicial es un ejemplo: revisa y corrige cantidades reales.
- No sustituye criterios de nutrición clínica ni de inocuidad alimentaria.
- No se ha verificado todavía el comportamiento en todos los modelos de iPhone y Android.

## Tecnología
HTML, CSS y JavaScript nativos; sin dependencias ni servicios de pago.
- `kio-visual-dna.css`: tokens de diseño compartidos.
- `index.html`: interfaz y lógica de la app.
- `manifest.webmanifest`: metadatos e iconos de instalación.
- `apple-touch-icon.png`: icono de inicio para iOS.
- `sw.js`: caché offline.


## Pulido visual y créditos
- Las tarjetas de receta, el menú diario y la vista ampliada utilizan ilustraciones pixel art de platillos con más textura, volumen y color; los iconos de ingredientes permanecen simples para identificarlos rápidamente.
- La pantalla conserva la firma discreta **“Una creación de KioRafa × ChatGPT”** y, en Ajustes, explica el reparto creativo: concepto y dirección de KioRafa; diseño e implementación en colaboración con ChatGPT.
- Las ilustraciones de comida se almacenan localmente en `assets/food/` y se incluyen en la caché offline.

## KIO × RAFA — identidad y pulido v0.3
- **Marca:** KIO × RAFA; KIO representa el sistema de diseño, exploración y lógica, y Rafa aporta la visión creativa, el contexto y la dirección del proyecto.
- **Escenas:** `realm.svg` y `kitchen.svg` son ilustraciones SVG de pixel art de mayor detalle, cargadas por la aplicación y almacenadas en caché para uso offline.
- **Platillos:** la aplicación genera ilustraciones inline con textura, volumen, sombras y colores por tipo de comida; no depende de un sprite pequeño externo para las tarjetas.
- **Inventario:** los iconos de ingredientes se mantienen más simples de forma deliberada para facilitar el reconocimiento rápido.
- **Créditos:** visibles de manera discreta en la interfaz y descritos en Ajustes.

## KIO × RAFA — pulido visual v0.3
- Marca visual: **KIO × RAFA**, una firma pequeña, integrada en la identidad de la app. KIO representa lógica, estructura y exploración; Rafa, visión creativa y dirección del producto.
- `icon.svg`: emblema de pixel art para la cabecera, favicon y manifiesto PWA.
- `realm.svg` y `kitchen.svg`: escenas detalladas con montaña, bosque, río, casas, luz de ventana, utensilios y estantes.
- Los platillos se ilustran directamente en el código con capas de volumen, sombras, textura y detalles de ingredientes; los iconos de despensa conservan su forma sencilla para una lectura rápida.
- El caché del Service Worker se versiona para actualizar la interfaz y sus escenas después de publicar.
- **Límite de icono:** la cabecera, favicon y manifiesto usan la nueva marca SVG; la validación del icono de inicio en iOS debe confirmarse en un iPhone real.
