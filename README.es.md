# Closed Sidebar by default

[ENGLISH](README.md) | **ESPAÑOL**

Componente de tema de Discourse que, en viewports móviles (≤767px), mantiene la barra lateral
cerrada por defecto y permite abrirla deslizando desde el borde izquierdo y cerrarla
deslizando hacia la izquierda. En una lista configurable de categorías la barra lateral se abre
automáticamente.

## Cómo funciona

- Abrir/cerrar reutiliza el propio interruptor de barra lateral de Discourse (el
  botón hamburguesa de la cabecera) en lugar de sobrescribir el CSS del núcleo, así que sigue siendo compatible entre
  actualizaciones y se anima con el panel deslizante nativo y su fondo.
- El comportamiento en escritorio/tableta no se toca.
- El inicializador vive en `javascripts/discourse/api-initializers/`, la ruta que
  Discourse carga automáticamente.

## Ajustes

- **exempt_categories**: slugs de categorías (como aparecen en la URL) donde la
  barra lateral debe abrirse automáticamente en móvil. Se edita desde la pestaña
  Ajustes del componente en el panel de administración. Por defecto: `glosario`, `trading-curso`, `wiki`.

Texto de este README bajo [CC BY-NC-SA 4.0](CC-BY-NC-SA-4.0.txt).
