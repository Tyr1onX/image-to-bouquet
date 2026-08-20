---
name: image-to-bouquet
description: Turn any reference image into one realistic, cost-conscious, florist-reproducible bouquet. Use for ordinary photos, landscapes, personal photography, posters, illustrations, album art, film stills, or any other image whose color, geometry, and visual mood should be translated into floral form. A complete run shows the reference image separately, generates one clean bouquet image, and provides a separate florist build sheet.
---

# Image to Bouquet

Turn **one image into one real bouquet**.

The reference can be anything: a landscape, sunset, street photo, architecture, portrait, personal photograph, illustration, poster, album cover, or abstract image. The source subject itself is not important. What matters is its **visual language**.

## What to preserve

Extract only four things:

1. **Color hierarchy** — dominant, secondary, accent colors and rough proportions.
2. **Geometry / composition** — tall or wide, centered or asymmetric, dense or airy, directional or static, major blocks and negative space.
3. **Texture** — soft, rough, glossy, matte, translucent, metallic, natural, geometric, etc.
4. **Visual mood** — calm, playful, cold, warm, dreamy, restrained, dramatic, nostalgic, futuristic, and similar visually grounded qualities.

Do not try to reproduce the literal objects in the source image.

A mountain does not become a mountain prop. A moon does not become a plastic moon. A portal does not become a glowing vortex. A person does not become a figurine. A building does not become a model building.

Translate the **visual relationships**, not the depicted objects.

## Translation rule

```text
Color      → flowers / foliage / wrapping / ribbon
Geometry   → bouquet silhouette / height / width / focal position / spacing
Texture    → flower surface / foliage / paper finish / transparency / material choice
Mood       → saturation / restraint / density / negative space
```

Use the **fewest floral decisions needed** to preserve the source identity.

## Reality is a hard constraint

The bouquet must look like something a normal competent florist could actually make.

Never generate:
- floating objects;
- planets, portals, crystals, figurines, logos, printed source images, or decorative props unless the user explicitly requests them;
- impossible flower anatomy;
- glowing flowers or fantasy materials with no real-world equivalent;
- physically implausible stem structures;
- an arrangement that depends on hidden CGI-like effects.

When a source color is difficult to obtain naturally, prefer:
1. wrapping or ribbon;
2. common dyed/preserved/artificial floral material, clearly stated in the build sheet;
3. the nearest realistic flower color.

## Cost is a hard constraint by default

Unless the user asks for a luxury bouquet, design a **small-to-medium, cost-conscious bouquet**.

Default target:
- about 30–40 cm wide;
- about 3–5 floral/foliage material types total;
- about 7–12 visible main flower heads/stems;
- only small amounts of filler and foliage;
- at most 1–2 premium/specialty materials;
- use wrapping, ribbon, foliage, and spacing to carry large color areas instead of adding more flowers;
- do not add a new species just to represent every small color in the source.

If the same visual effect can be achieved by changing wrapping instead of adding several flowers, choose wrapping.

## Before image generation

Lock a short florist recipe first:
- bouquet size and silhouette;
- flower/material names;
- count or small range;
- role and approximate placement;
- wrapping and ribbon;
- cost level;
- cheaper substitutions;
- 2–4 `must preserve` decisions;
- 2–4 `avoid` decisions.

The recipe is authoritative. If the generated image does not match it, regenerate/edit the image. Do not rewrite the recipe afterward to justify an accidental image.

## Final bouquet image

The final image is the primary result.

It must show:
- **one finished bouquet only**;
- a simple studio or natural photographic background;
- realistic flower scale and stem count;
- realistic florist wrapping;
- the source image's color hierarchy and geometric character;
- a result that could actually be reproduced from the build sheet.

It must contain **no**:
- text;
- palette;
- infographic panel;
- checklist;
- reference-image inset;
- watermark;
- moodboard layout;
- unrelated decorative object.

The reference image should be shown **separately** to the user for before/after comparison, never composited into the bouquet image.

## Required delivery

1. Show the original/reference image separately.
2. Generate the clean bouquet image.
3. Provide the florist build sheet separately as text/document.

A prompt, palette, analysis, or build sheet without the actual bouquet image is incomplete.

## Final test

Reject and revise the result if:
- it has become a generic bouquet with no relationship to the reference;
- it copied literal objects instead of visual language;
- it contains anything a florist cannot realistically reproduce;
- it uses too many flowers or too many species;
- it looks unnecessarily expensive;
- the bouquet image contains explanations or reference images;
- the image and recipe describe different bouquets.

The target is not the most spectacular bouquet.

The target is:

> **the simplest real bouquet that still clearly feels derived from the reference image.**