---
name: image-to-bouquet
description: Turn one reference image into one striking, florist-producible bouquet or floral piece. Preserve abstract palette, visual weight, contrast, rhythm, movement, negative space, material character, and mood without copying the source subject, local geometry, text, or recognizable imagery. Support fresh, hybrid, and art material modes. Output one final floral image plus one concise florist build sheet for that exact result.
---

# Image to Bouquet

Turn **one reference image into one visually faithful, designed, florist-producible floral work**.

The source is for analysis only. The final image must read first as a bouquet or floral piece, never as a picture rebuilt with flowers.

A complete run has exactly two deliverables:

1. one standalone final floral image;
2. one concise florist build sheet for that exact result.

Do not stop after image generation.

## 1. Resolve user preferences

Support these optional controls. If the user does not specify them, choose automatically from the source.

### Material mode
- **auto** — choose the best strategy for the image
- **fresh** — fresh flowers and fresh foliage; natural florist look
- **hybrid** — fresh + preserved / dried / dyed materials when useful
- **art** — visual fidelity first; preserved flowers, dyed flowers, dried botanicals, treated foliage, and high-quality artificial botanicals are allowed

### Color fidelity
- **natural** — natural flower colors take priority
- **balanced** — balance realism and palette fidelity
- **strict** — match the source palette closely, using treated/preserved/artificial materials when the selected material mode allows it

### Design intensity
- **safe** — elegant, commercial, restrained
- **editorial** — stronger composition and material contrast
- **bold** — high-impact, more directional and statement-like

### Budget
- **low / medium / high**

### Wrapping
- **minimal / commercial / editorial / luxury / color-led**

Recommended auto behavior:
- ordinary portrait / landscape / gift use → `fresh` or `hybrid`, `balanced`
- stylized album cover / poster / extreme palette → `hybrid` or `art`, usually `strict`

Explicit user choices always override auto selection.

## 2. Extract design language, not source content

Transfer only:

- dominant / secondary / accent colors and rough proportions;
- broad color placement and visual weight;
- warm/cool, dark/light, muted/saturated contrast;
- rhythm and directional energy;
- negative-space character and depth;
- material feel and mood.

Never transfer:

- source subject or silhouette;
- face/body geometry;
- object/building contours or scene layout;
- local edges and graphic linework;
- text, logos, symbols, printed artwork, or recognizable source fragments.

**Composition may survive; depiction may not.**

After analysis, create a short internal floral brief with no source-specific nouns. When possible, generate from that text brief instead of using the source image as an edit/image-to-image reference.

## 3. Lock the palette before choosing flowers

Do not begin from flower availability. Begin from the visual target.

Create 3–5 palette roles:

- dominant color;
- secondary color;
- transition / bridge color;
- accent color;
- optional neutral / dark field.

For each role, record internally:

- hue family;
- lightness;
- saturation;
- warm/cool bias;
- approximate visual share;
- where it should appear broadly.

Then assign each role to **flowers, foliage, treated materials, wrapping, or ribbon**.

The final bouquet should remain recognizably related to the source palette at thumbnail size. If the source is vivid, do not wash it into generic pastel floristry. If the source is restrained, do not over-saturate it.

## 4. Choose materials by color + character

A flower is not interchangeable just because its color matches.

Choose materials using all of these:

- color accuracy;
- silhouette / petal geometry;
- surface texture;
- scale;
- visual personality;
- movement;
- availability within the selected material mode.

Examples of material character:

- anemone → graphic, high-contrast focal
- calla lily → sculptural, modern, directional
- anthurium → glossy, bold, editorial
- orchid → refined, cool, exotic
- hydrangea → broad soft color mass
- rose / garden rose → dense romantic focal/support
- delphinium / snapdragon → vertical line and lift
- preserved / dyed foliage → controlled unusual color fields

Prefer **fewer, stronger material choices** over adding a new species for every hue.

## 5. Treat wrapping as part of the design

Wrapping is a first-class visual component, not an afterthought.

Use it to carry:

- large neutral or dark areas;
- strong background color fields;
- edge contrast;
- direction and silhouette;
- material contrast with the flowers.

Match wrapping by hue, value, translucency, sheen, stiffness, and layering.

For color-led or editorial references, wrapping may carry a substantial share of the source palette so the flowers do not need to become an overloaded color pile.

Do not print the source image, text, logo, or recognizable artwork on the wrapping.

## 6. Design for impact

Do not aim for merely safe or generally pretty. The result should have **one memorable floral design move**.

Choose one, occasionally two:

- off-center focal cluster with a clear counterweight;
- one distinctive hero flower/form against smaller textures;
- strong diagonal or upward botanical movement;
- concentrated warm/cool tension with a narrow transition bridge;
- bold wrapping-led composition;
- strong scale or texture contrast;
- intentional negative space that creates a memorable bouquet silhouette.

Build around:

- **focal** — unmistakable first read;
- **support** — balances without mirroring;
- **bridge** — connects color groups without averaging them;
- **line / movement** — botanical stems only;
- **depth** — foreground, middle, upper/rear;
- **negative space** — enough breathing room to avoid a flower wall.

If the result can be summarized as `one pile per color`, redesign it.

## 7. Material rules by mode

### Fresh
Use fresh flowers, fresh foliage, ordinary wrapping, and natural/near-natural colors. Accept moderate palette compromise if needed.

### Hybrid
Mix fresh flowers with preserved, dried, dyed, or treated botanicals when they materially improve color accuracy or design character.

### Art
Prioritize visual fidelity and design. Preserved flowers, dyed flowers, dried botanicals, treated foliage, and high-quality artificial botanicals are allowed and must be disclosed in the build sheet.

In all modes, the result must be **florist-producible**. Realistic does not mean every visible botanical must be an untreated fresh flower.

Visible non-botanical content should normally be limited to wrapping and ribbon. Structural wire/tape must remain hidden.

By default, no visible wire frameworks, rods, pins, grids, lights, electronics, cards, tags, labels, printed source imagery, acrylic props, figurines, or unrelated conceptual inserts.

## 8. Generate from a short florist brief

Use a fresh text-to-image path when available.

The image-generation brief should contain only:

- bouquet / floral form;
- selected material mode;
- exact materials and approximate counts;
- material type/treatment when relevant;
- focal / support / bridge roles;
- physical colors and macro color direction;
- hero design move;
- depth, movement, negative space;
- wrapping system and ribbon;
- color-faithful product/editorial photography.

Useful prompt shape:

> Editorial-quality but florist-producible [bouquet/floral piece]; material mode [fresh/hybrid/art]; [hero move]; [materials + counts + treatments]; [dominant/secondary/accent palette and direction]; clear focal/support/bridge hierarchy; varied scale and texture; visible front/mid/rear depth; intentional negative space; [wrapping system]; color-faithful lighting; crisp believable botanical detail.

Keep the prompt positive and florist-specific. Do not repeat source-specific forbidden nouns.

## 9. Accept only a strong result

Reject and regenerate if any of these are true:

- **Color failure:** dominant/secondary/accent relationships are noticeably weaker or shifted from the source without a material-mode reason.
- **Material failure:** flower/material character does not fit the source mood, or the chosen mode is ignored.
- **Wrapping failure:** wrapping feels generic, mismatched, or disconnected from the palette/composition.
- **Design failure:** no clear focal hierarchy, no memorable design move, flat depth, mechanical symmetry, or obvious color piles.
- **Generic failure:** pleasant but interchangeable with a standard catalog bouquet.
- **Depiction failure:** flowers collectively form a recognizable face, body, object, logo, picture, scene, or source-specific shape.
- **Prop failure:** visible unrelated devices, cards, text, source graphics, wire frameworks, or conceptual inserts appear.
- **Reality failure:** impossible construction, implausible gravity, excessive species/count, or materials a florist could not reasonably reproduce/source.
- **Lighting failure:** palette depends on colored illumination instead of the actual materials.

Desired balance:

> **recognizable palette + deliberate material selection + designed wrapping + memorable floral composition + real-world reproducibility + zero literal source content**

## 10. Florist Build Sheet

After the final accepted image, output:

```markdown
# Florist Build Sheet

## Design
- Size: S / M / L (approx. width × height)
- Form: bouquet / floral piece
- Material mode: fresh / hybrid / art
- Color fidelity: natural / balanced / strict
- Design intensity: safe / editorial / bold
- Budget: low / medium / high
- Core visual idea: ...
- Hero move: ...
- Focal / support / bridge: ...

## Materials
| Material | Type | Color / treatment | Qty | Role |
| --- | --- | --- | ---: | --- |
| ... | fresh / preserved / dried / dyed / artificial | ... | ... | focal / support / bridge / line / filler / foliage |

## Wrapping
- Outer wrap: ...
- Inner layer: ...
- Ribbon: ...
- Visual role: neutral field / color field / bridge / contrast / silhouette

## Assembly
1. Establish focal, movement, and depth.
2. Add support with unequal scale/height.
3. Add the bridge without flattening palette contrast.
4. Build the wrapping as part of the composition, preserve negative space, then tie.

## Substitutions
- ... → ...

## Must preserve
- ...
- ...
```

The build sheet must match the final image exactly and disclose preserved/dyed/artificial materials when used.
