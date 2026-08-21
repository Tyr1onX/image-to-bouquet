---
name: image-to-bouquet
description: Turn one reference image into one visually faithful, florist-producible bouquet. Support fresh, preserved, hybrid, and art modes. Preserve palette, visual weight, rhythm, mood, material character, and color relationships without copying the source subject. Output one final bouquet image plus one concise florist build sheet.
---

# Image to Bouquet

Turn **one reference image into one beautiful bouquet that a florist can actually make**.

The result must read first as a professionally designed bouquet, never as the source image rebuilt with flowers.

A complete run has exactly two deliverables:

1. one standalone bouquet image;
2. one concise florist build sheet for that exact bouquet.

Do not stop after image generation.

## 1. Resolve preferences

Support these optional controls. If unspecified, choose automatically.

### Material mode
- **auto** — choose the best mode
- **fresh** — fresh flowers and fresh foliage
- **preserved** — preserved flowers/botanicals as the main material system
- **hybrid** — fresh + preserved / dried / dyed botanicals
- **art** — visual fidelity first; high-quality artificial botanicals may also be used

Recommended auto behavior:
- natural portrait / landscape / gift use → `fresh` or `hybrid`
- album cover / poster / strong graphic palette → `preserved` by default
- extreme metallic / neon / impossible natural palette → `hybrid` or `art`

### Color fidelity
- **natural** — natural flower colors first
- **balanced** — realism and palette fidelity balanced
- **strict** — source palette first; use preserved/dyed materials when needed

### Design intensity
- **safe** — elegant and restrained
- **editorial** — stronger focal, wrapping, and material contrast
- **bold** — high-impact and directional

Optional: `budget: low / medium / high`, `wrapping: minimal / commercial / editorial / luxury / color-led`.

Explicit user choices always override auto selection.

## 2. Extract design language, not source content

Transfer only:
- dominant / secondary / accent colors and rough proportions;
- broad color placement and visual weight;
- warm/cool, light/dark, muted/saturated contrast;
- rhythm, movement, depth, negative space;
- material feel and mood.

Never transfer:
- source subject or silhouette;
- face/body geometry;
- object/building contours or scene layout;
- local graphic linework;
- text, logos, symbols, printed artwork, or recognizable source fragments.

**Composition may survive; depiction may not.**

After analysis, create a short internal floral brief with no source-specific nouns. When possible, generate from that text brief rather than using the source image as an edit reference.

## 3. Lock the palette and its relationships first

Before choosing flowers, define 3–5 palette roles:
- dominant;
- secondary;
- bridge;
- accent;
- optional neutral/dark field.

For each role, lock:
- hue family;
- lightness;
- saturation;
- warm/cool bias;
- approximate visual share;
- broad position.

Then record how the roles interact:
- hard split or soft transition;
- clean block or blended overlap;
- dark-to-light lift;
- cool-to-warm drift;
- dominant field with a small counter-color, or two near-equal poles.

Then assign the color work to **flowers, foliage, wrapping, or ribbon**.

Rules:
- the bouquet should still feel related to the source at thumbnail size;
- vivid references must not collapse into generic pastel floristry;
- do not give every source color equal flower coverage;
- large flat color fields are often better carried by wrapping than by adding more flower species;
- matching individual swatches is not enough if the relationship between them feels wrong.

### Selective gradient policy

Gradient is a tool, not a default style.

Use it only when the source contains a meaningful color drift or when one controlled transition materially improves the bouquet.

Good uses:
- a narrow bridge where cool genuinely drifts into warm;
- one preserved/dyed flower family with believable petal-edge or center-to-edge ombré;
- hydrangea, rose, carnation, orchid, fine foliage, or wrapping with a source-aligned transition;
- a layered wrapping fade that connects two strong fields without flattening them.

Rules:
- default to **1–2 gradient moments at most**;
- keep solid-color anchor flowers so the bouquet still has structure;
- gradient direction and color order must match the source;
- do not make every bloom gradient;
- do not add gradient simply because it looks decorative;
- if the source is mostly solid-color, keep the bouquet mostly solid-color.

## 4. Flower-first material selection

The bouquet subject should be **beautiful flower forms first**.

Choose materials by:
- color accuracy;
- flower shape;
- texture;
- scale;
- visual personality;
- movement;
- real availability in the selected mode.

### Preferred preserved vocabulary
Start from mature, commonly used preserved-flower families before reaching for unusual sculptural materials:

**Hero / focal**
- preserved rose / garden rose
- ranunculus-style preserved flower
- carnation
- hydrangea cluster
- mum / chrysanthemum families
- orchid / dendrobium when genuinely available

**Bridge / texture**
- gypsophila
- small preserved flowers
- lavender-like materials
- hydrangea fragments
- fine dried or preserved fillers

**Line / foliage**
- restrained eucalyptus
- ivy / pittosporum-like preserved greens
- fine preserved or dried line botanicals

Keep foliage subordinate unless the reference is explicitly botanical or forest-led. As a default, flowers should occupy the clear visual majority of the bouquet face.

Do not let one oversized broad leaf, spathe, tropical foliage mass, or sculptural botanical dominate merely because its shape matches part of the source. Anthurium, calla, large leaves, and similar materials are optional accents, not default hero choices.

Prefer **3–5 strong material families** over many small species.

## 5. Verify unusual materials instead of inventing them

For `preserved`, `hybrid`, and `art` modes, use florist-sourceable materials.

When web/catalog access is available:
- verify unusual preserved flower types, extreme colors, metallic finishes, gradient treatments, or specialty foliage against a current supplier catalog before relying on them;
- prefer established preserved-flower supplier families such as Florever, RoseAmor, Verdissimo, or equivalent regional suppliers;
- do not invent a preserved variety, color, or gradient treatment just because it would be convenient.

If a desired exact material is uncertain, use a verified substitute and state it in the build sheet.

Hidden florist wire/tape may be used for preserved-flower assembly, but it must not become a visible design element.

## 6. Wrapping is part of the design

Wrapping is not an afterthought. It may carry a substantial share of the source palette.

Design it by:
- hue and value;
- translucency;
- matte vs sheen;
- stiffness;
- number and direction of layers;
- edge contrast;
- relation to the focal flowers.

Use wrapping to carry large neutral, dark, or saturated fields instead of forcing flowers to do all color work.

A subtle layered fade or gradient is allowed only when it corresponds to the source and improves the transition between major color fields.

Do not print the source image, text, logo, or recognizable artwork on the wrapping.

## 7. Design the bouquet, not a color pile

Every bouquet needs one memorable floral decision, such as:
- off-center focal cluster with counterweight;
- one hero flower family against smaller textures;
- clear diagonal / upward botanical movement;
- concentrated warm/cool tension with a narrow bridge;
- strong scale contrast;
- wrapping-led silhouette;
- deliberate negative space.

Build around:
- **focal** — unmistakable first read;
- **support** — balances without mirroring;
- **bridge** — connects color groups without averaging them;
- **line / movement** — botanical only;
- **depth** — front / middle / upper-rear;
- **negative space** — enough breathing room to avoid a flower wall.

If the result can be summarized as `one pile per color`, redesign it.

## 8. Beauty gate

Reject and regenerate if any are true:
- **Color failure:** dominant / secondary / accent relationships are noticeably weaker than the source.
- **Relationship failure:** individual hues may be close, but the source's cool/warm, light/dark, or overlap logic is missing.
- **Gradient failure:** gradient is missing where it matters, placed in the wrong area/direction, or overused as decoration.
- **Flower-form failure:** the main visible materials are bulky, awkward, leaf-heavy, or less attractive than a simpler flower-led solution.
- **Design failure:** no clear focal hierarchy, weak rhythm, flat depth, mechanical symmetry, or obvious color piles.
- **Wrapping failure:** wrapping feels generic or disconnected from the palette.
- **Generic failure:** pleasant but interchangeable with a standard catalog bouquet.
- **Depiction failure:** flowers collectively form a face, body, object, logo, picture, scene, or source-specific shape.
- **Prop failure:** visible cards, text, graphics, wire frameworks, lights, electronics, or unrelated inserts appear.
- **Reality failure:** material/color/gradient is invented, construction is implausible, or the florist build sheet cannot source/reproduce the visible result.

The target is:

> **recognizable palette + correct color relationships + selective justified gradients + beautiful flower forms + deliberate wrapping + memorable bouquet design + florist reproducibility + zero literal source content**

## 9. Generate from a short florist brief

Use a fresh text-to-image path when available.

The generation brief should contain only:
- bouquet form;
- material mode;
- verified materials and approximate counts;
- focal / support / bridge roles;
- physical palette and macro color direction;
- gradient moments, if any;
- hero design move;
- depth, movement, negative space;
- wrapping system and ribbon;
- color-faithful product/editorial photography.

Useful prompt shape:

> Editorial-quality, florist-producible hand-tied bouquet; [mode]; flower-led composition with [hero move]; [materials + counts + treatments]; [palette roles and direction]; [one or two selective gradient moments only if justified]; clear focal/support/bridge hierarchy; varied flower scale and depth; restrained foliage; intentional negative space; designed [wrapping]; neutral color-faithful lighting; believable botanical detail.

Keep the prompt positive and florist-specific.

## 10. Florist Build Sheet

After the final accepted image, output:

```markdown
# Florist Build Sheet

## Design
- Size: S / M / L
- Material mode: fresh / preserved / hybrid / art
- Color fidelity: natural / balanced / strict
- Design intensity: safe / editorial / bold
- Core visual idea: ...
- Hero move: ...
- Focal / support / bridge: ...
- Gradient use: none / subtle / moderate; where and why

## Materials
| Material | Type | Color / treatment | Qty | Role |
| --- | --- | --- | ---: | --- |
| ... | fresh / preserved / dried / dyed / artificial | ... | ... | focal / support / bridge / line / filler / foliage |

## Wrapping
- Outer wrap: ...
- Inner layer: ...
- Ribbon: ...
- Visual role: ...

## Assembly
1. Establish focal, movement, and depth.
2. Add support with unequal scale and height.
3. Add bridge materials and any selective gradient moment without flattening palette contrast.
4. Build wrapping as part of the composition, preserve negative space, then tie.

## Substitutions
- ... → ...

## Must preserve
- ...
- ...
```

The build sheet must match the final image exactly and disclose preserved, dyed, dried, artificial, and gradient-treated materials when used.