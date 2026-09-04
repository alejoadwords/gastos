# Mis Gastos — actualización v2

Reemplaza los cuatro archivos del repositorio: `index.html`, `manifest.json`, `sw.js`, `icon.svg`.

## Antes de subir
Ya tienes el respaldo `gastos-respaldo-2026-09-04.json`. Guárdalo en Drive. No deberías necesitarlo, pero es tu red.

## Qué pasa al abrir la app nueva
Los datos siguen guardados bajo la misma clave (`gastos:v1`), así que cargan solos. La primera vez que abras la versión nueva corre una migración automática que:

1. Crea 6 categorías: Ropa y calzado, Cuidado personal, Salud y bienestar, Hogar y mercado, Regalos y donaciones, Deudas.
2. Reclasifica 25 movimientos que estaban mal ubicados, leyendo la nota de cada uno.
3. Convierte "Abono tarjeta de crédito" en un pago, no en un gasto.
4. Crea las fuentes de ingreso: Salario, Freelance, Otro.

La migración solo corre una vez (marca `v: 2` en los datos). Volver a abrir la app no la repite.

## Si el celular sigue mostrando la versión vieja
Cierra la app del todo y vuelve a abrirla. El service worker nuevo se actualiza solo en uno o dos minutos.

## Cierre de mes
Ajustes → Exportar JSON. Sube ese archivo al proyecto para el análisis.
