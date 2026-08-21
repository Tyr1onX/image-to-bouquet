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

### Graphic motifs are never bouquet objects

For album covers, posters, illustrations, interface-like artwork, and graphic design, text, line art, symbols, circuit-like marks, grids, diagrams, geometric overlays, borders, and similar graphic motifs are **not physical bouquet materials**.

Translate them only into abstract floral decisions such as:

- left/right or top/bottom color zoning;
- focal position and visual balance;
- spacing and negative space;
- rhythm, density, verticality, or asymmetry;
- restrained versus energetic overall mood.

Never turn source-image linework or graphic motifs into visible wires, black rods, metal frames, acrylic pieces, geometric inserts, sculptural supports, or other conceptual props.

## 2. Translate visual language into floral language

```text
Color    → flowers / foliage / wrapping / ribbon
Geometry → bouquet silhouette / height / width / focal position / spacing
Texture  → flower surface / foliage / paper finish / transparency
Mood     → saturation / restraint / density / negative space
```

Use the **fewest floral decisions needed** to preserve the visual identity.

### Preserve color roles, positions, and proportions

Do not merely collect the source colors. Preserve how they function in the image.

Prioritize, in order:

1. **large color zones and their spatial positions** — left/right, top/bottom, center/edge;
2. **dominant / secondary / accent proportions**;
3. **contrast structure** — cold/warm, dark/light, muted/saturated;
4. **transition colors** that prevent the bouquet from looking split or synthetic;
5. silhouette, texture, and mood.

Examples:

- If the source is cool on the left and warm on the right, keep that directional split in the bouquet rather than mixing every color evenly.
- If a dark neutral field occupies most of the source, carry that mass through wrapping, foliage, or negative space rather than overloading the bouquet with dark flowers.
- If a tiny bright accent creates the source identity, keep it small and deliberate instead of repeating it everywhere.

### Preserve color roles, not just colors

- Large dark areas should usually survive through wrapping, foliage, or negative space.
- Keep meaningful secondary/accent colors when they carry the source identity.
- Do not flatten a nuanced image into generic green-and-white or pink-and-white.
- For multi-color references, do not add a new flower species for every hue. Reuse one species in multiple available colors, use wrapping/ribbon, or reduce to the strongest color groups.
- Prefer believable florist colors. A flower color must plausibly exist as a fresh, naturally colored, dyed, preserved, or artificial botanical material. If a special treatment is needed, name it in the build sheet.
- Do not invent metallic, glowing, fluorescent, transparent, or otherwise impossible petals merely to copy a source color. Use wrapping, ribbon, a real treated botanical material, or the nearest believable hue instead.

## 3. Florist-real visible materials are a hard constraint

The finished bouquet must look like something a normal florist could physically assemble and sell.

### Default visible-material whitelist

Every major visible element must belong to one of these categories:

- real fresh flowers;
- real foliage or botanical branches;
- real dried or preserved botanicals;
- clearly disclosed dyed botanicals when needed;
- florist-usable artificial botanicals only when a difficult color cannot be achieved otherwise and the build sheet says so;
- wrapping paper, tissue, mesh, cellophane, or other ordinary bouquet wrapping;
- ribbon or ordinary tying material.

Structural florist supplies such as tape or wire may be used **only when they are normally hidden inside the construction**. They must not become a visible graphic or decorative element.

### Default forbidden visible elements

Unless the user explicitly asks for an installation-style or mixed-media bouquet, do not generate:

- exposed floral wire used as decoration;
- black rods, sticks, pins, or line frameworks;
- metal frames or geometric supports;
- acrylic sheets, plastic shapes, mirrors, crystals, resin pieces, or glass-like props;
- printed graphics, text cards, logos, source-image fragments, or symbolic inserts;
- figurines, planets, portals, lights, electronics, floating objects, or CGI-like effects;
- abstract sculptural elements whose material cannot be clearly named and purchased by a florist;
- impossible flowers or invented botanical species.

A real botanical branch is allowed only when it is visibly a natural plant material, not when it functions as a substitute for graphic line art.

### Build-sheet accountability rule

Every major visible element in the generated image must be explainable by the florist build sheet.

If the image contains a visible object that cannot be clearly named, sourced, quantified, and assigned a florist role, the image is invalid and must be regenerated or edited.

A useful test is:

> If a florist would point at a visible object and ask “what exactly is this, and where do I buy it?”, the generation has failed unless the build sheet already has a realistic answer.

## 4. Reality and cost are hard constraints

Unless the user asks for luxury, default to a **cost-conscious S–M bouquet**:

- about 30–40 cm wide;
- usually 3–5 floral/foliage material types total;
- roughly 7–12 visible main flower heads/stems;
- small amounts of filler/foliage only;
- at most 1–2 premium/specialty materials;
- use wrapping, ribbon, foliage, and spacing to carry large color areas instead of adding unnecessary flowers.

The bouquet should read first as a **real florist product**, not as a conceptual art installation.

If a source color is difficult in fresh flowers, prefer:

1. wrapping or ribbon;
2. a real dyed/preserved botanical material, disclosed in the build sheet;
3. florist-usable artificial botanical material, disclosed in the build sheet;
4. the nearest realistic flower color.

Do not solve a color problem by inventing a non-floral prop.

## 5. Lock the bouquet recipe before generating the image

Before calling the image tool, decide a short internal recipe:

- bouquet size and silhouette;
- flower/foliage/material types;
- count or small range for each;
- focal/support/filler roles;
- wrapping paper and ribbon;
- cost level;
- cheaper substitutions;
- 2–4 visual decisions that must survive;
- a short **visible-material inventory** containing every type of object that is allowed to appear in the image.

The recipe is authoritative. If the generated image does not match it, regenerate or edit the image. Do not rewrite the recipe afterward merely to justify an accidental generation result.

No visible object outside the locked inventory may be accepted simply because it looks visually interesting.

## 6. Generate the bouquet image

Use the host's **native image-generation tool**.

**One reference → one native image-generation call → one original bouquet image.**

The final image must:

- show one finished bouquet only;
- look like a real florist product photograph;
- use realistic flower scale, stem count, wrapping, and physical structure;
- match the locked recipe and visible-material inventory;
- preserve the source's color hierarchy, spatial color zoning, and geometric character;
- use a simple studio or natural background;
- contain no text, palette, checklist, reference inset, watermark, moodboard, or infographic;
- contain no visible decorative wire, abstract framework, geometric insert, or other non-floral conceptual object by default.

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

## 7. Produce the florist build sheet

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

Do not use the build sheet to retroactively justify an accidental abstract object. If an object violates the florist-real rules, remove it from the image instead.

## 8. Final check

Reject and revise if any of these are true:

- the bouquet looks generic and has lost the source identity;
- dominant/secondary/accent roles were flattened;
- large color zones were mixed together even though their spatial separation is important to the source;
- important dark mass, contrast, transition, or accent color disappeared;
- literal source content or graphic motifs were copied instead of abstracted;
- visible wires, black rods, line frameworks, metal structures, acrylic shapes, geometric inserts, or conceptual props appeared without an explicit user request;
- a visible element is not a real florist-usable material or cannot be named and sourced in the build sheet;
- a flower uses an implausible color or impossible morphology without a disclosed real-world treatment/material;
- anything is physically unreproducible;
- flower/species count is excessive for the achieved effect;
- it looks unnecessarily expensive;
- it reads as a conceptual installation rather than a sellable florist bouquet;
- the image and build sheet disagree;
- the delivered image is not a crisp direct native generation.

### Mandatory object audit before delivery

Before accepting the image, inspect every conspicuous visible object and classify it as one of:

- flower;
- foliage / botanical branch;
- dried / preserved / dyed / artificial botanical material disclosed in the sheet;
- wrapping;
- ribbon / tie.

If a conspicuous object cannot be placed in one of those categories, reject the image and regenerate or edit it.

## Batch / golden-sample testing

For multiple references, still generate **one bouquet per native image call**. Never ask the image model for a test matrix, before/after board, contact sheet, or multi-case infographic. Comparison sheets may be assembled afterward only for review.

Golden samples should intentionally include inputs with graphic overlays, line art, strong color zoning, and difficult colors. A successful result must preserve their visual identity **without importing their graphic objects into the bouquet**.

The target is:

> **the simplest real bouquet that clearly carries the reference image's color hierarchy, spatial color relationships, geometry, texture, and mood — using only florist-real visible materials — plus a short build sheet that lets a florist reproduce it.**
