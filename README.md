# El Point del Shawarma · Menú digital interactivo (demo)

Un solo archivo autocontenido: `index.html` (Tailwind, FontAwesome y Google Fonts por CDN). Variante **SIN IMÁGENES**, paleta naranja `#F26A1B` / ámbar `#FFB020` / base `#0B0B0C`. 25 productos en 6 categorías, con precios iguales a su menú actual.

## Cómo funciona
- Los productos se cargan desde una hoja de Google publicada como CSV (`PRODUCTS_CSV_URL`). Si falla o aún no está configurada, usa el respaldo local `fallbackRaw` y el menú nunca queda vacío. Los avisos salen solo por `console.warn`.
- `menu.csv` es el contenido de la hoja (`categoria,nombre,descripcion,precio,disponible`). Importarlo en Google Sheets, `Archivo > Compartir > Publicar en la web > CSV`, y pegar la URL en `PRODUCTS_CSV_URL`.
- Para marcar un producto agotado: `disponible = no`.
- Personalización con slots en cascada, configurada en `CUSTOM_BY_PRODUCT`: sin cebolla, sin lechuga, sin salsa de ajonjolí y proteína carne / pollo / mixto.
- Proteína: "con todo" equivale a Mixto al precio de la hoja. Carne suma $1 y Pollo resta $1 (`delta`), así que si cambias el precio en la hoja todo se ajusta junto.

## WhatsApp (DEMO)
- `WHATSAPP` y `EFECTO_LANDING_WA` usan el número del prospector (**0412-8995687**, `584128995687`), no el del cliente.
- Al entregar la versión final, cambiar `WHATSAPP` por el número de El Point (formato internacional, sin `+`). El footer de conversión de demo se elimina en el entregable final.

## Pendientes antes de entregar
- Horario, dirección exacta y enlaces de TikTok y Facebook del negocio.
- URL real del CSV publicado de su hoja de Google.

Texto comercial: `OFERTA.md`.
