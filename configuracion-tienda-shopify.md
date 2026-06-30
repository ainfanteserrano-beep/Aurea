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

## Pendiente / siguientes pasos sugeridos

- La tienda aún no tiene productos cargados. Siguiente paso natural: crear los productos de la temática de jabones — **Ritual de Coco**, **Ritual de Mango** y el **Kit Áurea** — y agruparlos en una colección.
- Subir imágenes de producto (barras de jabón, espuma, coco/mango) coherentes con la estética kraft/dorada.
