---
name: image-to-bouquet
description: Turn one reference image into one realistic, florist-reproducible bouquet. Preserve the source's color hierarchy, broad visual weight, contrast, rhythm, and mood without preserving its subject, silhouette, local contours, text, or recognizable imagery. The result must be a designed but non-figurative hand-tied bouquet plus a concise florist build sheet for that exact bouquet.
---

# Image to Bouquet

Turn **one reference image into one designed, real, non-figurative florist bouquet**.

The reference is an **analysis source**, not a template for the bouquet image.

The final result must read simply as a well-designed hand-tied bouquet. It must not depict, trace, imitate, print, or reconstruct what the source image shows.

A complete run has exactly two deliverables:

1. one standalone bouquet image;
2. one concise florist build sheet for that exact bouquet.

Do not stop after image generation. The task is incomplete until both exist.

---

## 1. Separate visual design from source subject

Analyze the source in two layers.

### Layer A — transferable visual relationships

These may influence the bouquet:

- **color hierarchy** — dominant / secondary / accent colors and rough proportions;
- **macro color placement** — broad relations such as left cooler / right warmer, center lighter / edge darker, upper area quieter / lower area denser;
- **visual weight** — where the image feels heavy, light, open, or concentrated at a coarse level;
- **contrast** — warm/cool, dark/light, muted/saturated, soft/sharp;
- **rhythm** — calm repetition, scattered accents, gradual transition, clustered energy;
- **directional energy** — broadly vertical, horizontal, diagonal, upward, spreading, or balanced;
- **negative-space character** — compact, airy, open, restrained;
- **material feel and mood** — soft, crisp, matte, glossy, quiet, dramatic, nostalgic, futuristic, romantic, restrained.

### Layer B — non-transferable source content

These must not survive:

- subject silhouette;
- face shape, facial layout, anatomy, body pose;
- object contour or recognizable object arrangement;
- building, skyline, mountain, road, window, character, product, or scene shape;
- local edges, internal linework, graphic overlays, symbols, typography, logos;
- texture maps such as skin, fabric, drawing strokes, screenshots, printed artwork;
- any source-specific geometry fine enough to reveal what the original image depicted.

**Composition may survive; depiction may not.**

A portrait may contribute a cool/warm split, value balance, focal intensity, and mood, but never the geometry of a face or body.

An album cover may contribute palette, broad weight, contrast, and rhythm, but never cover art, line graphics, typography, or subject shape.

---

## 2. Build an abstract composition map, not a picture map

Do not reduce the reference to colors alone. That creates dull color piles.

Instead, make a coarse internal composition map using only florist-safe design variables:

- dominant color mass;
- secondary color mass;
- accent color;
- one primary visual-weight zone;
- one supporting visual-weight zone;
- one transition / bridge zone;
- broad direction of movement;
- desired amount of negative space;
- desired depth and density.

Keep this map coarse. Do not encode facial features, object edges, or source contours.

### Break literal correspondence

The bouquet must not preserve one-to-one positions from the source.

After extracting the macro relationships:

- simplify small source regions into larger color families;
- merge nearby details;
- move focal material slightly when needed for floral balance;
- soften hard image boundaries into overlapping floral transitions;
- convert exact source edges into ordinary florist spacing and stem movement.

The goal is to preserve **visual logic**, not spatial tracing.

---

## 3. Create a sanitized floral brief

After source analysis, stop using source semantics and create a short internal floral brief.

The brief may contain only:

- 3–5 color families and rough proportions;
- macro color placement;
- focal / support / bridge roles;
- broad movement and negative space;
- bouquet form;
- botanical materials and approximate counts;
- wrapping and ribbon;
- neutral product-photo lighting;
- cost level.

Do not carry names of people, albums, characters, buildings, products, facial features, objects, scenes, titles, logos, or source motifs into the image-generation brief.

### Bouquet-form whitelist

Choose one ordinary florist form:

- natural round hand-tied bouquet;
- loose garden-style hand-tied bouquet;
- gently asymmetric hand-tied bouquet;
- lightly vertical hand-tied bouquet.

The form is chosen for floral design quality, not to trace the source subject.

---

## 4. Design the bouquet — do not merely stack colors

A successful result needs **floral composition**, not just color correspondence.

### Required design architecture

Unless the reference strongly calls for another florist-safe solution, design with these roles:

1. **Primary focal cluster** — the strongest 20–30% of visual weight. It should feel intentional, not like the center of a color wall.
2. **Supporting cluster** — a secondary mass that balances the focal cluster without mirroring it mechanically.
3. **Transition bridge** — flowers or foliage that visually connect major color zones.
4. **Directional line** — created only by real line flowers or natural botanical stems, never wire, rods, pins, frames, or artificial geometry.
5. **Negative space** — enough breathing room to separate layers and keep the bouquet from becoming a flat floral carpet.
6. **Depth layers** — foreground, middle, and rear/upper material should be visibly different in height or overlap.

### Color-transition rule

Do not make a bouquet that is simply:

> blue pile | beige separator | red pile

When two strong color zones meet:

- overlap them softly rather than creating a hard vertical border;
- use one or two bridge colors or shared materials across the boundary;
- let a small amount of the left-side color echo into the right side and vice versa when it improves cohesion;
- preserve the dominant direction without making the bouquet look cut in half;
- use wrapping or foliage to carry large dark/neutral masses instead of adding more flower heads.

The bouquet should feel **integrated but still clearly color-directed**.

### Material hierarchy

Prefer a small, intentional material vocabulary:

- 1 hero flower family or focal material;
- 1 supporting flower family;
- 1 line / movement material when useful;
- 1 filler or foliage material when useful;
- optional 1 specialty material only if it materially improves the design.

Avoid adding a new species for every hue.

### Anti-pile rules

Reject the design before generation if the recipe can be described mainly as:

- one dense block per color;
- equal-sized flower heads distributed uniformly;
- a flat wall of blooms with no depth;
- a centered separator strip between two color halves;
- many flower species used only to increase color coverage;
- dozens of repeated blooms with no focal hierarchy;
- perfectly mirrored left/right masses unless the user explicitly requests formal symmetry.

---

## 5. Lock a physically realistic florist recipe

Before image generation, lock the recipe.

Default target:

- S–M bouquet, roughly 30–40 cm wide;
- 3–5 botanical material types total;
- roughly 8–14 visually prominent stems / main heads, plus restrained filler;
- 1 clear focal hierarchy;
- 2–3 depth levels;
- visible negative space;
- ordinary florist wrapping and ribbon;
- colors that remain valid in normal daylight;
- cost-conscious unless the user asks for luxury.

The generated bouquet must visually respect these counts. If the image obviously shows dozens of main heads despite a small recipe, reject it.

### Visible-material whitelist

Visible content may contain only:

- fresh flowers;
- real foliage or natural botanical branches;
- disclosed dried / preserved / dyed botanical material when needed;
- disclosed florist-usable artificial botanical material only when necessary;
- ordinary florist wrapping paper / tissue / mesh / cellophane;
- ordinary ribbon or tying material.

### Structural materials are hidden only

Floral wire, tape, cable ties, pins, grids, cages, frames, rods, and mechanics may never be visible decorative language.

Do not use wire or pins to draw lines, connect points, imitate diagrams, create a network, or build a geometric skeleton.

If the build sheet contains a visible wire frame, geometric wire structure, bead pin system, rod framework, or similar decorative mechanic, the design is invalid.

Natural line flowers and branches are allowed only when they look botanical and organic. They must not form a deliberate diagram or polygon network.

### No decorative props by default

Do not add:

- lamps, LEDs, neon tubes, bulbs, light sticks, electronics;
- cards, tags, labels, tickets, printed slips, branded inserts;
- source prints, photos, logos, text, symbols, artwork fragments;
- acrylic, plastic inserts, mirrors, crystals, figurines, sculptural props;
- any non-floral object whose main purpose is to make the bouquet look more conceptual or futuristic.

Wrapping must look like flexible florist wrapping, not a poster, printed artwork, rigid panel, or display board.

---

## 6. Generate from the floral brief, not the source image

After the floral brief and recipe are locked:

- generate a **fresh bouquet from text**;
- use text-to-image rather than image editing / image-to-image when the host permits it;
- do not pass the source file, source crop, image ID, image path, or source pixels as a generation reference when a text-only path exists;
- do not composite, trace, project, texture, mask, or transform the source image.

The image model should receive the floral design, not the source subject.

### Prompt hygiene

The generation brief should be short, positive, and florist-specific.

Describe:

- bouquet form;
- exact botanical materials and approximate counts;
- focal / support / bridge roles;
- physical colors;
- broad color direction;
- depth and negative space;
- wrapping and ribbon;
- neutral, color-faithful product photography.

Do not fill the generation brief with a long list of source-specific forbidden nouns. Remove source semantics before generation instead.

---

## 7. Product-photo rules

The final image must:

- show one finished hand-tied bouquet only;
- look like a real florist product photograph;
- show believable stem count, flower scale, spacing, gravity, and wrapping;
- preserve visible depth rather than a flat floral surface;
- use neutral or gently warm/cool off-camera lighting;
- keep actual flower and wrapping colors readable;
- derive the palette from physical materials, not colored light or post-processing;
- contain no visible light source, printed matter, decorative hardware, or conceptual prop;
- remain crisp enough to inspect petals, foliage, wrapping, and material count.

If ordinary daylight would destroy the apparent palette, the design is invalid.

---

## 8. Mandatory acceptance audits

Do not accept the first attractive generation automatically.

### A. Ordinary bouquet test

Hide the reference and ask:

> Does this look first and only like a professionally designed hand-tied bouquet?

If it looks like a portrait, sculpture, picture, diagram, prop, stage object, or floral installation, reject it.

### B. Semantic-shape audit

Reject if the whole composition forms or strongly suggests any recognizable living form, object, symbol, letter, logo, scene, building, picture, relief, mosaic, or source-specific contour.

This applies to the **whole arrangement**, even if every individual element is a real flower.

### C. Floral-design audit

Reject if any of these are true:

- the design is mainly large blocks of different colors placed side by side;
- there is no clear focal / support hierarchy;
- major color zones have no transition bridge;
- the bouquet is a flat, dense wall with little depth or breathing room;
- flower-head sizes and heights are too uniform;
- there is no deliberate rhythm, movement, or negative space;
- too many species or blooms are used for the visual effect achieved;
- the arrangement feels mechanically symmetrical or grid-like without a good floral reason;
- the result looks like colors were merely filled into regions instead of composed as a bouquet.

### D. Source-copy audit

Reject if recognizable source content survives as a print, reconstructed shape, traced contour, graphic motif, scene fragment, object, or symbol.

Only abstract palette, broad visual weight, macro color placement, contrast, rhythm, direction, negative-space character, and mood may survive.

### E. Florist-material audit

Every conspicuous visible element must be flower, foliage, disclosed botanical material, wrapping, or ribbon.

Reject visible wire, rods, pins, line frameworks, geometric skeletons, lamps, cards, tags, acrylic, or other props.

### F. Reality and quantity audit

Reject if:

- flowers have impossible morphology or color without a disclosed real treatment;
- wrapping or stems behave implausibly;
- the visible flower count grossly exceeds the locked recipe;
- the bouquet is unnecessarily huge, complex, or expensive;
- the result reads as editorial spectacle instead of a sellable florist bouquet.

If any audit fails, revise the **floral recipe** and regenerate. Do not add props to rescue a weak design.

---

## 9. Florist Build Sheet — mandatory second deliverable

After the final accepted image exists, always provide a concise build sheet for that exact bouquet.

Use:

```markdown
# Florist Build Sheet

## Design
- Size: S / M (approx. width × height)
- Shape: ...
- Cost level: low / medium / high
- Core visual idea: ...
- Focal / support / bridge: ...

## Flowers & foliage
| Material | Color / treatment | Qty | Role |
| --- | --- | ---: | --- |
| ... | ... | ... | focal / support / bridge / line / filler / foliage |

## Wrapping
- Outer wrap: ...
- Inner layer: ...
- Ribbon: ...

## Assembly
1. Establish the focal cluster and depth.
2. Add support material without creating a flat color block.
3. Add the transition bridge and directional line.
4. Preserve negative space, then wrap and tie.

## Substitutions
- ... → ...

## Must preserve
- ...
- ...
```

The build sheet must never introduce a visible object that is absent from or forbidden in the accepted bouquet.

Before ending, verify internally:

- [ ] final accepted bouquet image delivered;
- [ ] matching florist build sheet delivered.

---

## 10. Golden-sample target

A strong result should make viewers recognize the **palette and atmosphere** of the reference while seeing only a sophisticated real bouquet.

It should preserve:

- color hierarchy;
- broad visual weight;
- macro color direction;
- contrast;
- rhythm and movement;
- negative-space character;
- mood.

It must not preserve:

- source subject;
- recognizable source geometry;
- graphic motifs or literal content.

The target is:

> **a cohesive, designed, non-figurative florist bouquet — not a picture made of flowers and not a set of color piles — plus a build sheet a florist can actually execute.**
