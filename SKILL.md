---
name: image-to-bouquet
description: Turn one reference image into one realistic, cost-conscious, florist-reproducible bouquet. Translate only the source image's color hierarchy, geometry, texture, and visual mood. A complete run must produce exactly two deliverables: one clean bouquet image generated directly by the host's native image tool, and one concise florist build sheet describing how to reproduce that same bouquet.
---

# Image to Bouquet

Turn **one reference image into one real bouquet**.

The input may be a personal photo, landscape, architecture, portrait, illustration, poster, album art, film still, or any other image. Treat it as a source of **visual language**, never as literal content to copy.

## Required output

A complete run produces exactly two deliverables:

1. **Bouquet image** — one clean, high-quality florist product image.
2. **Florist build sheet** — one short Markdown document explaining how to physically reproduce that same bouquet.

The reference image is analysis input only. It may be shown separately by the host for comparison, but it must never appear inside the generated bouquet image.

Do not finish with only analysis, a palette, a prompt, or a build sheet.

## 1. Read only four visual layers

Extract:

1. **Color hierarchy** — dominant, secondary, accent colors and rough proportions.
2. **Geometry** — tall/wide, centered/asymmetric, dense/airy, focal position, direction, negative space.
3. **Texture** — soft, rough, glossy, matte, translucent, metallic, natural, geometric, etc.
4. **Mood** — calm, playful, cold, warm, dreamy, restrained, dramatic, nostalgic, futuristic, etc.

Do not reconstruct the source scene, characters, faces, typography, logos, buildings, props, signature objects, or any other recognizable source content.

### Safe abstraction

For third-party artwork or branded media, first reduce the image internally to a neutral visual description such as:

> deep navy field + concentrated lime-green mass + small warm-yellow accents + energetic asymmetric composition

Design from that abstraction only. Do not ask the image model to recreate, trace, extend, restage, or closely imitate the protected work.

### Source-content firewall — absolute rule

The source image is **analysis-only**. The final bouquet may preserve abstract visual relationships, but it must contain **zero literal or recognizable source-image content**.

Never reproduce, print, redraw, collage, embed, or restage any of the following inside the bouquet, wrapping, ribbon, background, or accessories:

- faces or facial parts — eyes, lips, noses, ears, skin, hair, facial outlines, portraits;
- human bodies, silhouettes, hands, clothing shapes, poses, or recognizable anatomy;
- text, typography, album titles, captions, signatures, logos, labels, watermarks, or symbols;
- photographs, screenshots, source-image crops, printed portraits, printed cover art, or image fragments;
- recognizable characters, buildings, products, props, objects, scenery, or signature motifs from the source;
- line art, diagrams, circuit marks, graphic overlays, borders, UI elements, or decorative patterns copied from the source.

This rule applies even when the copied element would be physically printable or technically reproducible. **Physical reproducibility does not make literal source copying acceptable.**

For a portrait, a skin tone may become a peach, champagne, blush, beige, or warm neutral floral color, but no facial feature, face shape, body part, or portrait image may survive.

For an album cover, poster, or film still, the final bouquet must not contain any crop, reprint, portrait, title, logo, artwork fragment, or recognizable object from that source.

For a landscape or architecture image, the final bouquet must not reconstruct the mountain, building, skyline, road, window, tree silhouette, or other recognizable scene object. Translate only their abstract color zones, balance, direction, density, and mood.

**No source-image pixels or printed source imagery should appear in the final bouquet image.**

If the output contains any recognizable literal source element, reject it immediately and regenerate from the abstract floral recipe.

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
- printed graphics, text cards, logos, source-image fragments, printed portraits, or symbolic inserts;
- figurines, planets, portals, lights, electronics, floating objects, or CGI-like effects;
- abstract sculptural elements whose material cannot be clearly named and purchased by a florist;
- impossible flowers or invented botanical species.

A real botanical branch is allowed only when it is visibly a natural plant material, not when it functions as a substitute for graphic line art.

### Build-sheet accountability rule

Every major visible element in the generated image must be explainable by the florist build sheet.

If the image contains a visible object that cannot be clearly named, sourced, quantified, and assigned a florist role, the image is invalid and must be regenerated or edited.

A useful test is:

> If a florist would point at a visible object and ask “what exactly is this, and where do I buy it?”, the generation has failed unless the build sheet already has a realistic answer.

The reverse is also important: even if an element **can** be purchased or printed, it is still forbidden if it literally repeats source-image content.

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

Do not solve a color problem by inventing a non-floral prop or by printing the source image onto wrapping.

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

### Generation isolation rule

After the visual analysis is complete, the image-generation step must be driven by the **locked floral recipe**, not by literal source content.

When instructing the image generator:

- describe the bouquet as a new standalone florist product;
- describe flowers, foliage, wrapping, ribbon, color zoning, scale, silhouette, and lighting;
- do **not** ask it to preserve, recreate, include, print, or restage a face, person, album cover, text, logo, source object, source scene, or graphic motif;
- do **not** use the reference image as an edit target, collage layer, texture, print, or compositing source;
- if the host automatically exposes the reference image to the image model, explicitly state that it is **analysis-only** and that no recognizable source content may appear in the output.

The image should be generated **from scratch as a bouquet**, using only the abstracted recipe.

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
- contain no face, facial feature, human body, portrait, skin image, clothing image, or human silhouette;
- contain no printed source image, source-image crop, album-cover fragment, screenshot, logo, title, or recognizable source object;
- contain no visible decorative wire, abstract framework, geometric insert, or other non-floral conceptual object by default.

Plain wrapping paper may use solid colors, gradients, translucency, or ordinary non-referential texture. It must never carry a recognizable reproduction of the source image.

### Image provenance and quality

The final bouquet image must be a direct standalone output from the native image tool.

Never use as the final image:

- a crop from a collage/contact sheet/infographic/comparison board/screenshot;
- a crop or fragment of the source image;
- an enlarged thumbnail;
- an upscaled low-resolution crop;
- a recompressed preview when the original direct generation exists;
- a Python/graphics reconstruction used instead of native image generation;
- a composite in which the source image is printed, pasted, masked, projected, or blended into the bouquet.

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

Do not use the build sheet to retroactively justify an accidental abstract object or literal source-image reproduction. If an object violates the florist-real or source-content-firewall rules, remove it from the image instead.

## 8. Final check

Reject and revise if any of these are true:

- the bouquet looks generic and has lost the source identity;
- dominant/secondary/accent roles were flattened;
- large color zones were mixed together even though their spatial separation is important to the source;
- important dark mass, contrast, transition, or accent color disappeared;
- literal source content or graphic motifs were copied instead of abstracted;
- any face, facial feature, portrait, human anatomy, body silhouette, clothing image, or recognizable person appears;
- any text, title, logo, signature, source-image fragment, printed cover art, screenshot, recognizable source object, or recognizable source scene appears;
- the wrapping or ribbon contains printed imagery derived from the source;
- visible wires, black rods, line frameworks, metal structures, acrylic shapes, geometric inserts, or conceptual props appeared without an explicit user request;
- a visible element is not a real florist-usable material or cannot be named and sourced in the build sheet;
- a flower uses an implausible color or impossible morphology without a disclosed real-world treatment/material;
- anything is physically unreproducible;
- flower/species count is excessive for the achieved effect;
- it looks unnecessarily expensive;
- it reads as a conceptual installation rather than a sellable florist bouquet;
- the image and build sheet disagree;
- the delivered image is not a crisp direct native generation.

### Mandatory literal-copy audit before delivery

Compare the generated bouquet against the source one last time.

Ask:

1. Does any part of the output look like a cropped, printed, redrawn, traced, or reconstructed piece of the source?
2. Can I recognize a face, person, object, building, character, logo, word, symbol, or scene from the source?
3. Does the wrapping contain an image rather than just abstract color/material treatment?
4. Is any source-specific motif surviving as a literal object instead of a floral decision?

If **yes** to any question, reject the image and regenerate from the abstract floral recipe.

Only these source relationships may survive:

- color hierarchy and rough proportions;
- spatial color zoning;
- bouquet-scale geometry and balance;
- texture translated into real floral/material texture;
- overall mood.

### Mandatory object audit before delivery

Inspect every conspicuous visible object and classify it as one of:

- flower;
- foliage / botanical branch;
- dried / preserved / dyed / artificial botanical material disclosed in the sheet;
- wrapping;
- ribbon / tie.

If a conspicuous object cannot be placed in one of those categories, reject the image and regenerate or edit it.

Passing the object audit does **not** override the literal-copy audit. A printed portrait on wrapping is still forbidden even though the paper itself is a valid florist material.

## Batch / golden-sample testing

For multiple references, still generate **one bouquet per native image call**. Never ask the image model for a test matrix, before/after board, contact sheet, or multi-case infographic. Comparison sheets may be assembled afterward only for review.

Golden samples should intentionally include portraits, album covers, posters, graphic overlays, line art, strong color zoning, and difficult colors.

A successful portrait test preserves palette, light/dark balance, spatial emphasis, and mood **without reproducing the person or any facial/body feature**.

A successful album-cover test preserves color hierarchy and composition **without reproducing cover art, portraits, text, logos, graphics, or printed source fragments**.

A successful result must preserve visual identity **without importing literal source content into the bouquet**.

The target is:

> **the simplest real bouquet that clearly carries only the reference image's color hierarchy, spatial color relationships, geometry, texture, and mood — using florist-real visible materials, with zero literal source-image content — plus a short build sheet that lets a florist reproduce it.**
