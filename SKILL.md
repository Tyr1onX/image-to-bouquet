---
name: image-to-bouquet
description: Turn any reference image into one visually faithful, florist-buildable bouquet. Use for photos, posters, album covers, illustrations, logos, film stills, game images, and other visual references. A complete run outputs the reference image for comparison, one clean bouquet image, and a separate florist build sheet. The bouquet must be physically reproducible and cost-conscious by default.
---

# Image to Bouquet

Turn a reference image into **one real bouquet**, not a fantasy illustration and not an infographic.

## Required result

Show the user:

1. **Reference image** — separately, for comparison.
2. **Bouquet image** — the primary result. It must contain only the finished bouquet and a simple photographic background.
3. **Florist build sheet** — separate text/document. Never place the build sheet, palette, labels, reference thumbnail, arrows, or design notes inside the bouquet image.

A text prompt without an actual bouquet image is incomplete.

## Core task

```text
reference image
→ extract visual identity
→ translate it into real floral language
→ lock a buildable, cost-conscious recipe
→ generate the bouquet image
→ check image against recipe and reference
```

Do **not** copy every object from the reference. Preserve its visual identity through color hierarchy, silhouette, texture, density, negative space, and 1–3 identity anchors.

## 1. Read the reference

Extract only what matters:

- dominant / secondary / accent colors and their rough proportions;
- brightness, saturation, warm/cool balance;
- composition: centered/asymmetric, tall/wide, dense/airy, directional/static;
- texture: matte, glossy, metallic, translucent, soft, rough, etc.;
- mood;
- at most **1–3 identity anchors** whose loss would make the result generic.

Small accent colors may matter more than their area. Do not average the image into a dull palette.

## 2. Translate into bouquet language

Use this mapping:

- **Color →** flowers, foliage, wrapping, ribbon.
- **Composition →** bouquet silhouette, height, width, focal position, density, negative space.
- **Texture →** flower surface, leaves, wrapping finish, transparency, preserved/dried material.
- **Symbol →** indirect floral/structural suggestion only when useful.
- **Mood →** restraint, saturation, spacing, material choice.

### Symbol rule — very important

A reference may contain planets, portals, logos, cartoon characters, prisms, stars, buildings, faces, or other objects.

**Do not place literal miniature objects, floating planets, glowing portals, crystals, figurines, logos, printed cards, or impossible props into the bouquet just because they exist in the reference.**

Translate them indirectly with ordinary florist materials when possible. If an element cannot be translated naturally, omit it rather than turning the bouquet into a prop sculpture.

Examples:
- green portal → one concentrated lime-green floral mass or circular color rhythm, **not a glowing vortex object**;
- starry sky → sparse white/yellow filler points, **not floating planets**;
- rainbow → a restrained sequence of colored flowers, **not a plastic rainbow prop**.

Only use literal props when the user explicitly asks for them.

## 3. Reality and reproducibility are hard constraints

The generated bouquet must look like something a competent florist could actually assemble from purchasable flowers and standard florist materials.

Never invent:
- impossible flower anatomy;
- flowers fused into glowing objects;
- floating decorations with no support;
- physically implausible stem arrangements;
- materials that appear to levitate;
- fantasy light sources embedded in flowers unless the build sheet explicitly uses a real, ordinary product such as florist-safe micro lights and the user asked for that effect.

When an exact digital color is rare in fresh flowers, prefer one of these, in order:

1. shift that color to wrapping/ribbon;
2. use a common dyed/preserved/artificial floral material and say so;
3. choose the nearest realistic flower color.

Do not pretend an uncommon color exists naturally.

## 4. Cost control is the default

Unless the user asks for a luxury bouquet, design a **cost-conscious S–M bouquet**.

Default targets:

- about **30–40 cm wide**;
- usually **3–5 flower/foliage types total**;
- roughly **7–12 visible main flower heads/stems**;
- small amounts of inexpensive filler/foliage are allowed but must not make the bouquet look overfilled;
- at most **1–2 premium/specialty materials**, used only when they carry important visual identity;
- use wrapping and foliage to carry large color areas instead of buying many expensive flowers;
- avoid unnecessary species variety: one flower type may perform multiple visual roles;
- avoid dense “everything everywhere” arrangements unless density is essential to the reference.

Prefer a small number of strong decisions over many different flowers.

If a visual effect can be achieved either by adding five more flowers or by changing the wrapping paper, prefer the wrapping paper.

The build sheet should state the cost level (`low / medium / high`) and offer cheaper substitutions for premium materials.

## 5. Lock the florist recipe before image generation

Create a concise internal recipe first, then generate the image from it.

The separate florist build sheet must contain:

- size and silhouette;
- flower/foliage/material list;
- count or small range for each material;
- placement/role;
- wrapping paper and ribbon;
- short assembly order;
- cost level;
- cheaper substitutions;
- `must preserve` visual decisions;
- `avoid` decisions.

The recipe is authoritative. If the generated image violates it, regenerate/edit the image. Do not rewrite the recipe afterward to excuse an accidental image.

## 6. Bouquet-image rules

The final generated image must:

- show **one finished bouquet** clearly;
- show only the bouquet plus a simple studio or natural photographic background;
- look like a real florist product photo;
- match the locked recipe;
- preserve the reference's color hierarchy and composition character;
- use plausible flower sizes and stem counts;
- remain cost-conscious unless told otherwise;
- contain **no text**;
- contain **no design panel**;
- contain **no palette**;
- contain **no reference-image inset**;
- contain **no florist checklist**;
- contain **no watermark**;
- contain **no decorative fantasy object that is not in the build recipe**.

The reference image is shown separately in the conversation/UI for comparison; it must not be composited into the bouquet image.

## 7. Final check

Before delivery, reject and revise the bouquet if any of these are true:

- it is visually generic and has lost the reference identity;
- it contains literal fantasy props that a florist could not reproduce;
- it uses too many flowers/species for the effect achieved;
- it appears unnecessarily expensive;
- it is much denser than the reference needs;
- the image contains labels, instructions, or an inset reference;
- the flower counts/structure disagree with the build sheet;
- a florist could not plausibly rebuild it from the written recipe.

Judge success on five axes:

1. visual identity transfer;
2. color/composition fidelity;
3. physical reproducibility;
4. cost efficiency;
5. image ↔ build-sheet consistency.

The best result is **not the most spectacular bouquet**. It is the simplest real bouquet that still makes the user say: “yes, this came from that image.”
