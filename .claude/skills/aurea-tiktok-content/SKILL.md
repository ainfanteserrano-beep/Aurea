---
name: aurea-tiktok-content
description: Generate on-brand TikTok/IG content (video briefs, captions, hooks and Canva visuals) for Áurea artisan soaps. Use when asked to create, plan, or design TikTok/social content, pre-launch teasers, or marketing assets for Áurea.
---

# Áurea — Contenido TikTok

Genera piezas de contenido (guiones, captions y diseños de Canva) para la marca de
jabones artesanales **Áurea**, manteniendo consistencia de marca en todas las piezas.

## Voz e identidad de marca

- **Esencia:** "Áurea es el ritual de volver a ti. No vendemos jabones; creamos momentos de pausa."
- **Cliente:** mujeres 19–44 años que "pueden con todo" y necesitan permiso para bajar el ritmo.
- **USP:** "Un kit en uno, diseñado para un encuentro conmigo misma."
- **Tono:** natural, minimalista, divertido — cercano, sin pretensiones, entiende el caos de la
  vida adulta. Textos en pantalla y captions van en **minúsculas**, una idea por plano, mucho aire.
- **Estética visual:** kraft natural, papel seda, fondos limpios, luz natural y dorada
  ("Áurea" = dorada), props reales de coco y mango. Cero ruido visual.
- **Formato video:** vertical 9:16, faceless (manos, espuma, agua, barra de jabón, fruta — nunca
  rostro), voz en off femenina cálida y cercana. ASMR de agua/espuma + lo-fi cálido de fondo.
- **Productos base:** Ritual de Coco (pausa), Ritual de Mango (despertar/energía), Kit Áurea
  (los dos juntos).

La referencia completa de guiones, hooks A/B y captions con hashtags vive en
`guiones-rituales-faceless.md` en la raíz de este repo — léelo antes de escribir contenido nuevo
para reusar el tono y no repetir hooks ya probados.

## Flujo de trabajo

1. **Definir la pieza**: confirma con el usuario qué se necesita (guion de video, caption,
   portada/cover para TikTok, carrusel de anuncio, teaser de pre-lanzamiento, etc.) y qué
   producto/ángulo aplica (Coco / Mango / Kit / lanzamiento general).
2. **Escribir el brief** siguiendo la estructura de `guiones-rituales-faceless.md`: tabla de
   tiempo/toma visual/VO-texto para video, o bloque de caption + hashtags para posts.
   - Guarda guiones nuevos como secciones adicionales en `guiones-rituales-faceless.md` (o un
     archivo nuevo si es una campaña distinta) para mantener un histórico de contenido.
3. **Generar el visual en Canva** (si se pide un diseño, cover o carrusel):
   - Usa `mcp__Canva__list-brand-kits` para ver si hay un brand kit de Áurea disponible; si el
     usuario quiere on-brand, aplícalo con `brand_kit_id`.
   - Usa `mcp__Canva__generate-design` con `design_type: "your_story"` para piezas verticales
     9:16 (covers/teasers de TikTok e Instagram Stories), o `"instagram_post"` /
     `"facebook_post"` para carruseles y posts cuadrados.
   - Incluye siempre en el `query`: estética (kraft, papel seda, dorado, minimalista), props
     reales (coco/mango, espuma, agua), tipografía en minúsculas para el mensaje principal, y el
     mensaje/CTA específico de la pieza.
   - Presenta las miniaturas/URLs de los candidatos generados al usuario para que elija.
   - Al elegir, usa `mcp__Canva__create-design-from-candidate` con el `job_id` y `candidate_id`
     correspondientes para guardar el diseño final y editable en su cuenta.
4. **Entregar**: comparte el guion/caption en texto y los links de edición/vista de Canva.

## Notas de producción (aplican siempre)

- Faceless real: encuadre de hombros hacia abajo, nunca rostro.
- El héroe visual es la barra de jabón y su espuma/agua (ASMR).
- Cierre estándar de video: logo Áurea sobre kraft + 1 línea de VO; opcional QR a la playlist
  "Áurea: Tu momento de paz".
- CTA en caption (no en video): tono cercano, tipo "Date tu momento de pausa → link en bio."
- Hashtags discretos y consistentes: `#áurea #ritualdevolverati #autocuidado` + 2-3 específicos
  del ángulo (producto, momento del día, etc.).
