# KIO MENÚ — Cocina de aventura

Aplicación web progresiva (PWA) en español, diseñada primero para Android y con interfaz pixel art.

## Funciones v0.1
- Inventario editable de ingredientes.
- Generación heurística de desayuno, almuerzo, comida y cena.
- Modos ahorro, práctico, explorador y exprés.
- Estimación orientativa de costos por porción e ingredientes faltantes.
- Recetas breves, cambio individual de plato y progreso de misiones.
- Opción para priorizar comidas que no dependan de guardar sobras refrigeradas.
- Persistencia local y caché básica para uso sin conexión tras la primera carga.

## Tecnología
HTML, CSS y JavaScript nativos, sin dependencias, cuentas, API ni servicios de pago. Los datos de inventario y preferencias permanecen en `localStorage` del navegador.

## Límites conocidos
- El motor de menú es heurístico, no inteligencia artificial.
- Las recetas y costos son una base inicial; los precios son aproximados y no equivalen al costo de comprar paquetes completos.
- La coincidencia de ingredientes depende de cómo se escriban.
- No es un sistema de nutrición clínica ni sustituye las prácticas de inocuidad alimentaria.
- No se sincroniza entre dispositivos.

## Abrir
La app se publica en la subruta `/kio-menu/` del sitio GitHub Pages que la contiene. En Android, abre la URL en el navegador y usa el menú del navegador → **Agregar a pantalla de inicio**.
