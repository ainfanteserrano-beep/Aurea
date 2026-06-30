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
| Ritual de Coco | ✅ Subida (jabón de coco sobre fondo terracota, coco real + hoja natural) |
| Ritual de Mango | ⏳ Pendiente — Canva agotó la cuota de generación |
| Kit Áurea | ⏳ Pendiente — Canva agotó la cuota de generación |

> Nota: las imágenes generadas incluyen un rótulo de marketing y la etiqueta del jabón puede salir con texto distorsionado (artefacto de IA). Para fotos de producto 100% limpias, lo ideal es subir fotografías reales.

## Pendiente / siguientes pasos sugeridos

- **Generar imágenes de Mango y Kit** cuando se reinicie la cuota de Canva (mismo estilo que Coco).
- **Ajustar precios reales** y pasar los productos de DRAFT a **ACTIVE** cuando estén listos.
- **Cargar inventario** (cantidades) en cada variante.
- Publicar el tema **Atelier** desde el admin para activar el look terracota.
