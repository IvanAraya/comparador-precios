# Comparador de Precios

Aplicación web progresiva (PWA) para comparar precios de productos según su valor unitario (precio dividido entre cantidad de unidades por el contenido de cada unidad).

## Uso

Abre `index.html` en un navegador, o instala la app desde el sitio publicado en GitHub Pages. Al instalarla funciona sin conexión gracias al Service Worker (`sw.js`), que guarda en caché los archivos de la aplicación.

Los datos ingresados se guardan automáticamente en el almacenamiento local del navegador (`localStorage`), por lo que se conservan al cerrar y volver a abrir la app.

## Estructura

- `index.html`: interfaz y lógica de la aplicación.
- `manifest.json`: metadatos de la PWA (nombre, íconos, colores, modo de visualización).
- `sw.js`: Service Worker con estrategia de caché para funcionamiento offline.
- `icons/`: íconos de la aplicación en distintos tamaños.
- `.github/workflows/deploy.yml`: despliegue automático a GitHub Pages en cada push a `main`.

## Despliegue en GitHub Pages

El sitio se despliega automáticamente mediante GitHub Actions al hacer push a la rama `main`. Para habilitarlo (una sola vez), en el repositorio ve a **Settings → Pages → Build and deployment → Source** y selecciona **GitHub Actions**.
