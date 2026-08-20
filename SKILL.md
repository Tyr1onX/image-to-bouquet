---
name: image-to-bouquet
description: Translate any reference image into a visually faithful, florist-buildable bouquet. Use when the user wants a photo, poster, album cover, illustration, logo, film still, game image, or other visual reference turned into a bouquet. A complete run MUST generate a bouquet image and a florist-ready build sheet; text-only analysis or prompts are incomplete.
---

# Image to Bouquet

## Purpose

Turn a reference image into **one coherent bouquet** that preserves the image's visual identity while remaining realistic for a florist to build.

A complete result has two required outputs:

1. `bouquet.png` (or equivalent image artifact)
2. `bouquet-spec.md` (or equivalent florist-ready execution sheet)

The bouquet image is the primary user-facing result. The build sheet explains how to reproduce that exact bouquet.

**Never finish with only analysis, a color palette, flower suggestions, or an image-generation prompt.**

## Product boundary

This is not a generic flower recommender and not a literal object-copying task.

The task is visual translation:

```text
Reference Image
→ Visual DNA
→ Translation Decisions
→ Buildable Bouquet Spec
→ Bouquet Image
→ Consistency Check
```

The goal is not “use flowers with similar colors.” The goal is:

> Preserve what makes the reference visually recognizable after changing the medium from image to bouquet.

## Default interaction

Do not force the user through a questionnaire.

If the user only supplies an image, produce a useful first result immediately. Infer a reasonable medium hand-held bouquet unless the reference clearly calls for another scale or the user gives size, budget, recipient, flower type, freshness, season, or material constraints.

When assumptions materially affect execution, state them briefly in the build sheet instead of blocking generation.

## Pass A — Extract the Visual DNA

Read the image as a composition, not as a list of objects.

Extract:

### 1. Palette
Identify:
- dominant colors;
- secondary colors;
- accent colors;
- approximate visual percentage of each;
- black/white/neutral balance;
- saturation;
- brightness;
- warm/cool relationship;
- gradients or iridescence when visually important.

Do not average the image into a dull palette. Preserve small but identity-critical accent colors.

### 2. Composition
Identify:
- visual center;
- left/right or top/bottom weight;
- symmetry/asymmetry;
- density versus negative space;
- directionality;
- major large, medium, and small shapes;
- whether the image feels compact, vertical, horizontal, radiating, layered, floating, or fragmented.

### 3. Texture and material impression
Identify qualities such as:
- matte / glossy;
- metallic / pearlescent;
- translucent / opaque;
- soft / hard;
- airy / dense;
- organic / geometric;
- smooth / rough;
- hazy / crisp.

### 4. Mood
Infer only what is visually supported, such as:
- dreamy;
- quiet;
- playful;
- futuristic;
- romantic;
- brutal;
- nostalgic;
- cosmic;
- minimal;
- theatrical.

Mood controls restraint and material choice. It is not decoration added on top.

### 5. Identity anchors
Find at most 1–3 visual features whose loss would make the translation feel generic.

Examples:
- a neon green portal against deep navy;
- one saturated red slash in a black image;
- a silver/blue light wash;
- a pink carousel silhouette;
- a rainbow emerging from black;
- a repeated circular form.

These anchors may become flower choices, silhouette decisions, wrapping, line elements, or restrained accents. Do not mechanically reproduce copyrighted artwork or insert the source image into the bouquet unless the user explicitly asks for that.

## Pass B — Translate Visual DNA into Bouquet Language

Use these mappings as principles, not rigid lookup tables.

### Color → flower / foliage / wrapping / ribbon

Assign colors according to visual role:
- dominant image color → dominant bouquet mass or wrapping field;
- secondary colors → supporting flower groups;
- small high-contrast accents → limited focal flowers or line accents;
- neutrals → breathing room, foliage, paper, or base flowers.

Preserve color hierarchy. Do not give every extracted color equal area.

### Composition → silhouette / height / density / focal point

Translate large-scale geometry into the bouquet:
- strong vertical image → taller stems / upward movement;
- broad horizontal image → wider fan or lateral spread;
- centered symmetry → controlled balanced bouquet;
- asymmetry → off-center focal mass with intentional counterweight;
- large negative space → fewer flowers, clearer gaps, restrained filler;
- dense image → fuller layering, but still buildable.

### Texture → materials

Use flower surface, foliage, wrapping, ribbon, dried material, metallic/pearlescent elements, transparency, and layering to carry texture.

Do not rely on color alone when texture is a major part of the source identity.

### Symbol → accent

Translate symbols indirectly when possible.

Prefer:
- one arcing stem instead of a literal printed rainbow;
- radiating line flowers instead of a pasted starburst;
- a circular floral opening instead of a copied portal graphic;
- silver structural leaves instead of a logo cutout.

Literal printed props should be used only when the user requests them or when the reference cannot remain recognizable without them.

### Mood → restraint

Mood determines how much to include:
- quiet/minimal references require fewer species, more air, lower saturation;
- theatrical references may support larger contrast and denser focal structure;
- futuristic references may use metallic, translucent, unusual gradients, or sharper structure;
- nostalgic references may prefer softer color transitions and less synthetic contrast.

## Pass C — Make It Buildable

Before generating the image, lock a florist-executable plan.

The plan must include:

### Bouquet profile
- intended size: XS / S / M / L / XL or approximate width × height;
- hand-tied / presentation bouquet / arm bouquet / other relevant structure;
- silhouette;
- focal location;
- density and negative-space target.

### Flower recipe
For every material group specify:
- flower / foliage / decorative material;
- color or treatment;
- count when practical, otherwise percentage/range;
- role: focal / secondary / filler / line / foliage / accent;
- approximate placement.

Do not invent a botanically impossible flower solely to match a digital color. When a precise color is uncommon naturally, use a realistic dyed/preserved/artificial option or shift that color into wrapping/materials and state the choice.

### Wrapping and finishing
Specify:
- outer paper;
- inner paper / translucent layer if used;
- number of visible layers when important;
- paper color and finish;
- ribbon color, width, and finish;
- optional wire, pearl, acrylic, metallic, dried, or other accent materials.

### Assembly order
Give a concise build sequence, for example:
1. establish line and height;
2. place focal flowers;
3. build secondary masses;
4. add fillers/foliage while preserving negative space;
5. wrap in stated layer order;
6. tie and rotate-check the focal face.

### Substitution rules
Give substitutions by **visual role**, not merely species.

For example:
- “If blue delphinium is unavailable, substitute another cool blue line flower of similar height; do not replace it with a compact blue rose.”

### Must preserve / must avoid
List the 3–6 visual decisions that most affect identity.

Examples:
- preserve one neon-green focal area against dark navy;
- keep the bouquet asymmetric;
- retain at least 20% visual breathing room;
- avoid warm kraft paper;
- avoid turning every accent into a separate flower species;
- avoid a conventional round rose bouquet when the reference is angular or sparse.

## Pass D — Generate the Bouquet Image

Use the host's native image-generation or image-editing capability to create the final bouquet image.

**An image-generation prompt is an internal implementation detail, not a final output.**

### Image requirements
The final image should:
- show one finished bouquet clearly;
- look physically buildable;
- follow the locked flower recipe, hierarchy, silhouette, palette, and wrapping;
- show realistic stem/flower scale and plausible material behavior;
- keep the bouquet itself as the subject;
- avoid unnecessary text, labels, watermarks, moodboard panels, or an inset copy of the reference image unless explicitly requested;
- be high enough resolution to inspect color, structure, and wrapping.

A clean studio, neutral, or contextually compatible background is acceptable, but background styling must not compensate for a weak bouquet translation.

### Spec is authoritative
The build sheet is the construction contract.

If the generated image materially violates the locked spec, regenerate or edit the image. Do **not** silently rewrite the spec afterward just to match an accidental generation result.

## Pass E — Consistency Check

Before completion, compare the image against both the reference and build sheet.

Score mentally on five axes:

1. **Identity transfer** — does it still feel like the source image after removing literal source objects?
2. **Color hierarchy** — are dominant/secondary/accent proportions preserved?
3. **Composition transfer** — did the source's balance, direction, density, and negative space survive?
4. **Buildability** — could a florist plausibly assemble this?
5. **Image/spec consistency** — does the generated bouquet match the written recipe?

If any axis is obviously poor, revise before delivering.

## Required florist build-sheet format

Use this concise structure:

```markdown
# Bouquet Build Sheet

## Design intent
One short paragraph explaining what visual identity is being preserved.

## Visual DNA
- Palette: ...
- Mood: ...
- Composition: ...
- Identity anchors: ...

## Bouquet profile
- Size: ...
- Shape: ...
- Focal point: ...
- Density / negative space: ...

## Flower recipe
| Material | Color / treatment | Amount | Role | Placement |
| --- | --- | ---: | --- | --- |

## Wrapping & finishing
- ...

## Assembly
1. ...

## Substitutions
- ...

## Must preserve
- ...

## Avoid
- ...
```

## Completion behavior

Normal completion means presenting:

1. the final bouquet image;
2. the florist build sheet.

Optional analysis may follow, but it must not displace the image as the main result.

If the host has no image-generation/editing capability, state clearly that the required image output cannot be completed in that environment. Do not claim the Skill succeeded by returning only a prompt.

## Non-goals

Do not:
- merely name flowers matching sampled colors;
- produce a generic round bouquet for every image;
- copy every object from the reference literally;
- add decorative symbols that overwhelm the flowers;
- generate a fantasy bouquet that cannot be built while calling it florist-ready;
- replace the final bouquet image with a moodboard, palette, SVG diagram, or text description;
- make the user do the visual-analysis work the Skill is supposed to perform.
