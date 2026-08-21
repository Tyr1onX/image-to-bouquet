---
name: image-to-bouquet
description: Turn one reference image into one realistic, cost-conscious, florist-reproducible bouquet. Use the source only to extract abstract color hierarchy, coarse spatial color relationships, material feel, and mood. Never preserve or recreate the source subject, silhouette, local contours, or recognizable imagery. A complete run must produce exactly two deliverables: one clean standalone bouquet image and one concise florist build sheet for that same bouquet.
---

# Image to Bouquet

Turn **one reference image into one ordinary, real, non-figurative florist bouquet**.

The reference may be a portrait, landscape, album cover, poster, architecture image, illustration, or any other picture. It is an **analysis source**, not a visual template for the generated image.

The final result must always read simply as:

> a normal hand-tied florist bouquet

It must never read as a floral portrait, floral sculpture, floral relief, mosaic, picture, symbol, character, object, building, landscape reconstruction, or themed prop.

## Required output

A complete run produces exactly two deliverables:

1. **Bouquet image** — one standalone, crisp, realistic florist product photograph.
2. **Florist build sheet** — one short Markdown document explaining how to reproduce that exact bouquet.

The image-generation call is not the end of the task. Do not finish until both deliverables exist.

---

## 1. Analyze the source, then detach from it

Read only these abstract properties:

1. **Color hierarchy** — dominant / secondary / accent colors and rough proportions.
2. **Coarse color zoning** — only broad relations such as left cooler / right warmer, center lighter / edge darker, top muted / bottom saturated.
3. **Overall density and direction** — airy / dense, calm / energetic, vertically biased / horizontally broad / balanced.
4. **Material feel and mood** — soft / crisp / matte / glossy / restrained / dramatic / nostalgic / futuristic, translated only into ordinary florist materials.

### Never extract subject geometry

Do **not** preserve or transfer:

- subject silhouette;
- face shape or facial layout;
- body pose or anatomy;
- object contour;
- building outline;
- mountain / skyline / road / window shape;
- local edges, internal linework, feature positions, or recognizable scene layout;
- any source-specific shape that could let a viewer identify what the original picture depicted.

Source **geometry is not a design target**. Only coarse, non-semantic balance may survive.

For portraits specifically, ignore the geometry of the person completely. A portrait can contribute palette, broad light/dark balance, and mood only.

For album covers, posters, and illustrations, ignore all typography, line art, symbols, graphic motifs, and recognizable artwork. They may influence broad color zoning or mood only.

### Texture is not a texture map

Do not map skin texture, fabric texture, drawing marks, brush strokes, image noise, or source surface details onto flowers or wrapping.

Translate texture only at a very high level, for example:

- soft → soft-petaled flowers / matte wrap;
- crisp → cleaner flower spacing / firmer wrap edges;
- glossy → a naturally glossy botanical such as anthurium or subtle cellophane;
- airy → more negative space and lighter filler.

---

## 2. Create a sanitized floral brief

After analysis, create a short internal **sanitized floral brief** and stop reasoning from the source image itself.

The brief may contain only:

- 3–5 color groups with rough proportions;
- broad color zones such as left / right / center / edge;
- one ordinary florist bouquet form;
- density / airiness;
- flower and foliage names;
- wrapping and ribbon;
- neutral product-photo lighting;
- cost level.

The brief must **not contain source semantics** such as the identity of a person, album, character, object, building, landscape, logo, title, facial feature, or other depicted subject.

Do not carry source nouns into the image-generation prompt.

### Bouquet form whitelist

Choose only an ordinary florist form:

- natural round hand-tied bouquet;
- loose garden-style hand-tied bouquet;
- gently asymmetric hand-tied bouquet;
- lightly vertical hand-tied bouquet.

The form must be selected for florist plausibility and broad visual balance, **not to trace the source subject**.

Do not create pictorial or representational arrangements.

---

## 3. Lock a real florist recipe

Before image generation, lock:

- size: normally S–M, around 30–40 cm wide;
- bouquet form from the whitelist above;
- 3–5 flower / foliage material types total when possible;
- roughly 7–12 visible main flower heads / stems;
- focal / support / filler roles;
- wrapping paper and ribbon;
- material colors that carry the source palette in normal daylight;
- cost level;
- cheaper substitutions;
- a visible-material inventory.

### Default visible-material inventory

The finished bouquet may visibly contain only:

- real fresh flowers;
- real foliage or botanical branches;
- real dried / preserved botanicals;
- clearly disclosed dyed botanicals when necessary;
- florist-usable artificial botanicals only when necessary and disclosed;
- ordinary florist wrapping paper / tissue / mesh / cellophane;
- ordinary ribbon or tying material.

Structural wire or tape may be used internally but should not become visible decoration.

### Not part of the default bouquet

Do not add decorative props just because they are physically possible. By default the bouquet contains no:

- visible wire frameworks, rods, frames, acrylic or plastic inserts;
- lamps, LEDs, neon tubes, light sticks, bulbs, electronics, or active light sources;
- cards, tags, labels, tickets, printed slips, message cards, or branded inserts;
- source-image prints, photos, logos, words, symbols, or artwork fragments;
- figurines, models, crystals, mirrors, sculptural props, or CGI-like effects.

Wrapping should look like ordinary flexible florist wrapping, not a poster, printed artwork, rigid panel, or display board.

---

## 4. Generate from the sanitized recipe, not from the source image

This is the most important generation rule.

### Reference detachment

After the sanitized floral brief and recipe are locked:

- generate a **new bouquet from text**;
- do not use the source image as an edit target;
- do not pass the source file, source crop, source image ID, or source image path as a generation reference when the tool allows a text-only call;
- do not composite, mask, project, texture, trace, restage, or transform the source image;
- use a fresh text-to-image generation path rather than image editing / image-to-image when possible.

The source is for the agent's analysis step only. The image model should receive the **sanitized floral recipe**, not the original subject description.

### Prompt hygiene

Keep the image-generation brief short and positive.

Describe only:

- one ordinary hand-tied florist bouquet;
- exact flowers / foliage and approximate counts;
- physical flower colors;
- broad color zoning;
- natural spacing and bouquet form;
- ordinary wrapping and ribbon;
- neutral, color-faithful studio photography.

Do **not** feed the image model a long list of source-specific negative concepts. In particular, do not repeat source semantic nouns merely to say they are forbidden. The sanitization step should remove those concepts before generation.

A good generation brief should still make complete sense if the source image is hidden.

### Non-figurative composition rule

Flowers are arranged for **floral balance only**.

They must not be positioned to collectively depict a recognizable picture, contour, relief, symbol, letter, object, scene, or living form.

Do not create a continuous petal surface, flower mosaic, pixel-like field, or sculpted floral mass whose purpose is to reproduce an image.

---

## 5. Product-photo rules

The final image must:

- show one finished bouquet only;
- look like a normal florist product photograph;
- use realistic flower scale, stem count, spacing, wrapping, and gravity;
- use a simple neutral or natural background;
- use neutral or gently warm/cool **off-camera** lighting;
- keep actual flower and wrapping colors readable;
- derive the palette from physical materials, not colored light or post-processing;
- contain no visible light source;
- contain no text or printed matter;
- remain crisp with clear petal, foliage, and wrapping detail.

A useful color test:

> If the bouquet were viewed in ordinary daylight, its main color relationships should still be present.

---

## 6. Mandatory acceptance audits

Do not accept the first attractive image automatically.

### A. Ordinary-bouquet test

Hide the reference mentally and inspect the output.

Ask:

> Would a florist describe this simply as a hand-tied bouquet, or would they say it is shaped like / depicting something?

If it depicts **anything**, reject it.

### B. Semantic-shape audit

Reject if the overall flower arrangement forms or strongly suggests:

- a recognizable living form;
- a recognizable object;
- a symbol, letter, logo, picture, scene, building, or source-specific contour;
- a portrait-like or relief-like central surface;
- any image made out of flowers.

This audit applies to the **whole composition**, not just individual materials. A composition can fail even if every individual element is a real flower.

### C. Source-copy audit

Reject if any recognizable source content survives as:

- printed imagery;
- a reconstructed shape;
- a traced contour;
- a graphic motif;
- a scene fragment;
- a source-specific object or symbol.

Only abstract palette, coarse color zoning, broad density, and mood may survive.

### D. Florist-material audit

Every conspicuous visible item must be explainable as flower, foliage, disclosed botanical material, wrapping, or ribbon.

### E. Lighting / paper audit

Reject if:

- colored light is carrying the palette;
- any light fixture is visible;
- any unnecessary tag / card / label / paper insert appears;
- wrapping looks printed, rigid, sculptural, or implausible.

### F. Reality audit

Reject if:

- the flowers have impossible morphology or color without a real disclosed treatment;
- stems / flower heads / wrapping are physically implausible;
- the bouquet is unnecessarily huge, complex, or expensive;
- the result reads as installation art or editorial prop instead of a sellable florist bouquet.

If any audit fails, regenerate from the sanitized recipe. Do not rewrite the recipe to justify an accidental result.

---

## 7. Florist Build Sheet — mandatory second deliverable

After the **final accepted image** exists, always provide the build sheet.

If the image was regenerated, describe the final accepted bouquet, not an earlier attempt.

Use this concise format:

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

The build sheet and image must describe the **same bouquet**.

Before ending the run, verify internally:

- [ ] Final accepted bouquet image delivered.
- [ ] Florist Build Sheet delivered for that exact image.

If either is missing, the run is incomplete.

---

## Batch / golden-sample testing

For every reference, generate one standalone bouquet. Do not generate test matrices or comparison collages as the final bouquet image.

Golden samples should include portraits, album covers, landscapes, architecture, abstract artwork, strong color zoning, and dramatic lighting.

A successful test preserves only:

- color hierarchy and rough proportions;
- coarse spatial color zoning;
- broad density / direction;
- high-level material feel;
- mood.

It must **not preserve what the source depicts**.

The target is:

> **a normal, non-figurative, florist-reproducible bouquet that carries the reference image's palette and atmosphere without carrying its subject, shape, symbols, or literal content — plus a matching build sheet.**
