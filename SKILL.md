---
name: image-to-bouquet
description: Turn one reference image into one striking, realistic, florist-reproducible bouquet. Preserve abstract color hierarchy, visual weight, contrast, rhythm, movement, negative space, and mood without preserving the source subject, local geometry, text, or recognizable imagery. Output one bouquet image plus one concise florist build sheet for that exact bouquet.
---

# Image to Bouquet

Turn **one reference image into one striking, real, non-figurative florist bouquet**.

The source is for visual analysis only. The final image must read first as a professionally designed hand-tied bouquet, not as a picture made from flowers.

A complete run has exactly two deliverables:

1. one standalone bouquet image;
2. one concise florist build sheet for that exact bouquet.

Do not stop after image generation.

## 1. Extract design language, not source content

Transfer only:

- color hierarchy and rough proportions;
- broad visual weight and macro color direction;
- warm/cool, dark/light, muted/saturated contrast;
- rhythm and directional energy;
- negative-space character and depth;
- high-level material feel and mood.

Never transfer the source subject, silhouette, face/body geometry, object/building contours, local edges, typography, logos, graphics, or recognizable scene structure.

**Composition may survive; depiction may not.**

After analysis, create a short internal floral brief with no source-specific nouns. When possible, generate the final bouquet from that text brief rather than using the source image as an edit or image-to-image reference.

## 2. Design for impact

Do not aim for merely safe or generally pretty. The bouquet should contain **one memorable botanical design move** while remaining realistic.

Choose one, occasionally two:

- an off-center focal cluster with a clear counterweight;
- one distinctive hero flower/form against smaller supporting textures;
- a strong diagonal or upward movement created by real line flowers or natural stems;
- concentrated warm/cool tension with a restrained transition bridge;
- an intentional opening of negative space that gives the bouquet a recognizable silhouette.

The impact must come from flowers, foliage, spacing, color, scale, and wrapping — never from props.

### Floral hierarchy

Build around:

- **focal** — one unmistakable first read;
- **support** — balances the focal without mirroring it;
- **bridge** — connects major color groups without washing them into one average color;
- **line / movement** — real botanical stems only;
- **depth** — foreground, middle, and upper/rear layers;
- **negative space** — enough breathing room to keep the bouquet from becoming a flower wall.

Use visible differences in flower size, height, texture, and density. Avoid distributing all important flowers evenly.

### Color architecture

Preserve dominant / secondary / accent roles. Do not turn every source color into equal flower coverage.

When strong color zones meet:

- keep their contrast readable;
- overlap them selectively instead of making a hard border;
- use a narrow bridge color/material rather than filling the whole bouquet with transition tones;
- let a small echo of one side appear on the other only when it improves cohesion;
- use wrapping or foliage for large neutral/dark masses instead of adding more flowers.

If the result can be summarized as `one pile per color`, redesign it.

### Avoid generic florist-template results

A technically correct bouquet can still fail if it feels interchangeable with a standard catalog arrangement.

Before generation, ask:

> What is the one botanical decision that makes this bouquet memorable?

If there is no clear answer, strengthen the focal material, asymmetry, movement, scale contrast, texture contrast, or negative space — without adding more species or props.

## 3. Keep the material vocabulary disciplined

Default target unless the source clearly needs otherwise:

- S–M bouquet, about 30–45 cm wide;
- 3–5 botanical material families;
- about 10–18 visually prominent stems / heads plus restrained filler;
- 1 hero/focal family;
- 1 supporting family;
- 1 bridge or line family;
- foliage/filler only when it improves structure;
- ordinary florist wrapping and ribbon;
- cost-conscious unless luxury is requested.

Prefer fewer, stronger choices over many small ones. Do not add a new species just to match another hue.

Visible elements may be only real/disclosed botanical materials, florist wrapping, and ribbon. Structural wire/tape must stay hidden.

By default, no visible wire frameworks, rods, pins, grids, lights, electronics, cards, tags, labels, printed source imagery, acrylic, crystals, figurines, or conceptual props.

Colors must come from actual materials under normal daylight, not from strong colored lighting or glow effects.

## 4. Generate from a short florist brief

Use a fresh text-to-image generation path when available.

The image-generation brief should describe only:

- bouquet form;
- exact materials and approximate counts;
- focal / support / bridge roles;
- physical colors and macro color direction;
- hero design move;
- depth, movement, and negative space;
- wrapping and ribbon;
- neutral, color-faithful product photography.

A useful prompt shape is:

> Editorial-quality but physically realistic florist product photograph of one hand-tied bouquet; [form]; [hero move]; [materials + counts]; [color hierarchy and direction]; clear focal/support/bridge hierarchy; varied height and scale; visible front/mid/rear depth; intentional negative space; ordinary [wrapping]; neutral studio lighting; crisp natural flower morphology.

Keep the prompt positive and florist-specific. Do not repeat the source subject in a long negative list.

## 5. Accept only a strong real bouquet

Reject and regenerate if any of these are true:

- **Depiction failure:** the flowers collectively form a recognizable face, body, object, symbol, picture, scene, logo, or source-specific shape.
- **Prop failure:** visible non-floral devices, cards, text, graphics, wire frameworks, lights, or conceptual inserts appear.
- **Design failure:** no clear focal hierarchy, no memorable botanical decision, flat depth, uniform flower heads, mechanical symmetry, or obvious color piles.
- **Generic failure:** the bouquet is pleasant but could represent almost any reference because its palette, tension, movement, and focal choice are too generic.
- **Reality failure:** impossible flower morphology/color, implausible wrapping/gravity, excessive species/count, or visible materials that a florist cannot reproduce.
- **Lighting failure:** the palette depends on colored illumination rather than actual flower/wrapping colors.

The desired balance is:

> **recognizable palette and atmosphere + memorable floral design + real-world reproducibility + zero literal source content.**

## 6. Florist Build Sheet

After the final accepted image, output this concise sheet:

```markdown
# Florist Build Sheet

## Design
- Size: S / M (approx. width × height)
- Shape: ...
- Cost level: low / medium / high
- Core visual idea: ...
- Hero move: ...
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
1. Establish the focal and depth.
2. Add support with unequal height/scale.
3. Add bridge and botanical movement without flattening the color contrast.
4. Preserve negative space, then wrap and tie.

## Substitutions
- ... → ...

## Must preserve
- ...
- ...
```

The build sheet must describe the final image exactly and must not introduce any forbidden visible element.
