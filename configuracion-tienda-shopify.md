# Áurea · Configuración de tienda Shopify (terracota + jabones)

> Configuración de marca aplicada a la tienda **Aurea Studios** (`1smhu3-hs.myshopify.com`).
> Paleta terracota/kraft alineada con la temática de los jabones artesanales (rituales de Coco y Mango).

## Paleta de color aplicada

Estética de marca: Kraft natural, papel seda, luz dorada/cálida, terracota como acento héroe.

| Rol en el tema | Token | HEX | Uso |
|---|---|---|---|
| Fondo (`background`) | `color_palette.background` | `#F6EEE3` | Crema kraft cálido — fondo de página, drawers, inputs, tarjetas |
| Texto (`foreground`) | `color_palette.foreground` | `#3E2A22` | Marrón cacao profundo — texto, badges "agotado" |
| Acento (`color1`) | `color_palette.color1` | `#C2674A` | **Terracota** — botones primarios (CTA), badge de rebaja, variante seleccionada |
| Bordes (`color2`) | `color_palette.color2` | `#E2D1B9` | Arena cálida — bordes sutiles de inputs, drawer y variantes |

### Mapeos clave
- **Botón primario (CTA "Comprar"):** fondo y borde en terracota (`color1`), texto en crema (`background`).
- **Variante seleccionada:** fondo y borde en terracota (`color1`), texto en crema.
- **Badge de rebaja:** fondo terracota (`color1`), texto crema.
- El resto de elementos (fondos, texto, drawers, popovers, inputs) heredan la paleta vía Liquid (`{{ settings.color_palette.* }}`).

## Dónde se aplicó

- **Tema:** `Atelier` (sin publicar) — `gid://shopify/OnlineStoreTheme/165473058905`
- **Archivo:** `config/settings_data.json` (bloques `current` y preset `Atelier`)
- El tema en vivo **Horizon** (MAIN) no se modifica porque la API de Shopify bloquea escrituras al tema publicado.

## Para activarlo en la tienda en vivo

1. En el admin de Shopify: **Tienda online → Temas**.
2. En el tema **Atelier**, usa **Vista previa** para revisar el look terracota.
3. Cuando estés conforme, pulsa **Publicar** para hacerlo el tema en vivo.

> Nota: la publicación de temas debe hacerse desde el admin (la API la bloquea por seguridad).

## Productos creados (temática de jabones)

Creados como **borrador (DRAFT)** con precios **provisionales** — ajústalos antes de publicar.

| Producto | SKU | Precio provisional | Estado |
|---|---|---|---|
| Ritual de Coco — Jabón Artesanal | `AUREA-COCO-01` | $9.00 | DRAFT |
| Ritual de Mango — Jabón Artesanal | `AUREA-MANGO-01` | $9.00 | DRAFT |
| Kit Áurea — Coco + Mango | `AUREA-KIT-01` | $16.00 | DRAFT |

- Todos con `vendor: Áurea`, inventario rastreado (cantidad 0) y descripciones de marca.
- Agrupados en la colección **Rituales Áurea** (`handle: rituales-aurea`).

## Imágenes de producto (generadas con Canva)

Imágenes de marca generadas con IA (estética terracota/kraft), formato 1080×1350.

| Producto | Imagen |
|---|---|
| Ritual de Coco | ✅ Subida — coco sobre fondo terracota (incluye rótulo de marketing y etiqueta con texto distorsionado) |
| Ritual de Mango | ✅ Subida — flat lay limpio en caja kraft, grabado "ÁUREA" correcto |
| Kit Áurea | ✅ Subida — imagen "hero" con las dos cajas + rituales de Coco y Mango juntos |

> Nota: algunas imágenes generadas por IA incluyen rótulo de marketing o texto distorsionado en la etiqueta del jabón. Para fotos de producto 100% limpias, lo ideal es subir fotografías reales.

## Pendiente / siguientes pasos sugeridos

- (Opcional) **Regenerar la imagen de Coco** en el estilo limpio de Mango para dar consistencia al set.
- **Ajustar precios reales** y pasar los productos de DRAFT a **ACTIVE** cuando haya stock.
- **Cargar inventario** cuando llegue el stock (por ahora en 0, sin existencias).
- Publicar el tema **Atelier** desde el admin para activar el look terracota.
