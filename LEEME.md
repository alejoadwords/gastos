# Mis Gastos — PWA

Cuatro archivos: `index.html`, `manifest.json`, `sw.js`, `icon.svg`. Deben quedar juntos en la misma carpeta.

## Publicarla (5 minutos, gratis)

**Opción A — Netlify Drop (la más rápida)**
1. Entra a https://app.netlify.com/drop
2. Arrastra la carpeta `gastos` completa.
3. Te da una URL tipo `https://algo.netlify.app`. Listo.

**Opción B — GitHub Pages**
1. Crea un repositorio nuevo en GitHub (puede ser privado con plan pago; público es gratis).
2. Sube los cuatro archivos a la raíz.
3. Settings → Pages → Source: Deploy from branch → main → / (root) → Save.
4. La URL queda en `https://TU_USUARIO.github.io/NOMBRE_REPO/`.

La app necesita HTTPS para instalarse como PWA; ambas opciones lo dan por defecto.

## Instalarla en el celular
- **Android (Chrome):** abre la URL → aparece el botón "Instalar" dentro de la app, o menú ⋮ → "Instalar aplicación".
- **iPhone (Safari):** abre la URL → botón Compartir → "Agregar a pantalla de inicio".

Funciona sin conexión después de la primera carga.

## Cierre de mes
Ajustes → "Exportar JSON" (o Movimientos → "CSV"). Sube ese archivo al proyecto de Claude para el análisis con datos reales.

## Importante
Los datos viven en el navegador del teléfono. Si borras datos del navegador o cambias de celular, los pierdes: exporta el respaldo cada mes y guárdalo en Drive.
