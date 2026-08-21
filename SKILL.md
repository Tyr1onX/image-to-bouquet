---
name: image-to-bouquet
description: Turn one reference image into one realistic, cost-conscious, florist-reproducible bouquet. Translate only the source image's color hierarchy, geometry, texture, and visual mood. A complete run must produce exactly two deliverables: one clean bouquet image generated directly by the host's native image tool, and one concise florist build sheet describing how to reproduce that same bouquet.
---

# Image to Bouquet

Turn **one reference image into one real bouquet**.

The input may be a personal photo, landscape, architecture, portrait, illustration, poster, album art, film still, or any other image. Treat it as a source of **visual language**, not literal content to copy.

## Required output

A complete run produces exactly two deliverables:

1. **Bouquet image** — one clean, high-quality florist product image.
2. **Florist build sheet** — one short Markdown document explaining how to physically reproduce that same bouquet.

The reference image is the input and may be shown separately for comparison, but it is not part of the generated bouquet image.

Do not finish with only analysis, a palette, a prompt, or a build sheet.

## 1. Read only four visual layers

Extract:

1. **Color hierarchy** — dominant, secondary, accent colors and rough proportions.
2. **Geometry** — tall/wide, centered/asymmetric, dense/airy, focal position, direction, negative space.
3. **Texture** — soft, rough, glossy, matte, translucent, metallic, natural, geometric, etc.
4. **Mood** — calm, playful, cold, warm, dreamy, restrained, dramatic, nostalgic, futuristic, etc.

Do not reconstruct the source scene, characters, faces, typography, logos, buildings, props, or signature objects.

### Safe abstraction

For third-party artwork or branded media, first reduce the image internally to a neutral visual description such as:

> deep navy field + concentrated lime-green mass + small warm-yellow accents + energetic asymmetric composition

Design from that abstraction only. Do not ask the image model to recreate, trace, extend, restage, or closely imitate the protected work.

## 2. Translate visual language into floral language

```text
Color    → flowers / foliage / wrapping / ribbon
Geometry → bouquet silhouette / height / width / focal position / spacing
Texture  → flower surface / foliage / paper finish / transparency
Mood     → saturation / restraint / density / negative space
```

Use the **fewest floral decisions needed** to preserve the visual identity.

### Preserve color roles, not just colors

- Large dark areas should usually survive through wrapping, foliage, or negative space.
- Keep meaningful secondary/accent colors when they carry the source identity.
- Do not flatten a nuanced image into generic green-and-white or pink-and-white.
- For multi-color references, do not add a new flower species for every hue. Reuse one species in multiple available colors, use wrapping/ribbon, or reduce to the strongest color groups.

## 3. Reality and cost are hard constraints

Unless the user asks for luxury, default to a **cost-conscious S–M bouquet**:

- about 30–40 cm wide;
- usually 3–5 floral/foliage material types total;
- roughly 7–12 visible main flower heads/stems;
- small amounts of filler/foliage only;
- at most 1–2 premium/specialty materials;
- use wrapping, ribbon, foliage, and spacing to carry large color areas instead of adding unnecessary flowers.

Never generate floating objects, planets, portals, crystals, figurines, logos, printed source images, impossible flowers, unsupported decorations, or CGI-like effects.

If a source color is difficult in fresh flowers, prefer:

1. wrapping or ribbon;
2. common dyed/preserved/artificial floral material, disclosed in the build sheet;
3. the nearest realistic flower color.

## 4. Lock the bouquet recipe before generating the image

Before calling the image tool, decide a short internal recipe:

- bouquet size and silhouette;
- flower/foliage/material types;
- count or small range for each;
- focal/support/filler roles;
- wrapping paper and ribbon;
- cost level;
- cheaper substitutions;
- 2–4 visual decisions that must survive.

The recipe is authoritative. If the generated image does not match it, regenerate or edit the image. Do not rewrite the recipe afterward merely to justify an accidental generation result.

## 5. Generate the bouquet image

Use the host's **native image-generation tool**.

**One reference → one native image-generation call → one original bouquet image.**

The final image must:

- show one finished bouquet only;
- look like a real florist product photograph;
- use realistic flower scale, stem count, wrapping, and physical structure;
- match the locked recipe;
- preserve the source's color hierarchy and geometric character;
- use a simple studio or natural background;
- contain no text, palette, checklist, reference inset, watermark, moodboard, or infographic.

### Image provenance and quality

The final bouquet image must be a direct standalone output from the native image tool.

Never use as the final image:

- a crop from a collage/contact sheet/infographic/comparison board/screenshot;
- an enlarged thumbnail;
- an upscaled low-resolution crop;
- a recompressed preview when the original direct generation exists;
- a Python/graphics reconstruction used instead of native image generation.

Cropping or assembling images is allowed only for secondary review sheets after the standalone bouquet image already exists.

Regenerate if petals, foliage, wrapping texture, or edges are visibly soft because of cropping, compression, or upscaling.

## 6. Produce the florist build sheet

Keep it **brief and directly usable by a florist**. Do not turn it into a long design report.

Use this format:

```markdown
# Florist Build Sheet

## Design
- Size: S / M (approx. width × height)
- Shape: ...
- Cost level: low / medium / high
- Core visual idea: one short sentence

## Flowers & foliage
| Material | Color / treatment | Qty | Role |
| --- | --- | ---: | --- |
| ... | ... | ... | focal / support / filler / foliage |

## Wrapping & external materials
- Outer wrap: ...
- Inner layer: ...
- Ribbon: ...
- Other real florist materials: ...

## Assembly
1. ...
2. ...
3. ...
4. ...

## Substitutions
- ... → ...

## Must preserve
- ...
- ...
```

Only list materials actually visible or required in the generated bouquet.

The document and image must describe **the same bouquet**.

## 7. Final check

Reject and revise if any of these are true:

- the bouquet looks generic and has lost the source identity;
- dominant/secondary/accent roles were flattened;
- important dark mass, contrast, or accent color disappeared;
- literal source content was copied instead of abstracted;
- anything is physically unreproducible;
- flower/species count is excessive for the achieved effect;
- it looks unnecessarily expensive;
- the image and build sheet disagree;
- the delivered image is not a crisp direct native generation.

## Batch / golden-sample testing

For multiple references, still generate **one bouquet per native image call**. Never ask the image model for a test matrix, before/after board, contact sheet, or multi-case infographic. Comparison sheets may be assembled afterward only for review.

The target is:

> **the simplest real bouquet that clearly carries the reference image's color hierarchy, geometry, texture, and mood — plus a short build sheet that lets a florist reproduce it.**
