---
name: image-to-bouquet
description: Turn one reference image into one visually faithful, florist-producible bouquet. Support fresh, preserved, hybrid, and art modes. Preserve palette, visual weight, rhythm, mood, material character, color relationships, and wrapping language without copying the source subject. Output one final bouquet image plus one concise florist build sheet.
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

Optional:
- `budget: low / medium / high`
- `wrapping: minimal / commercial / editorial / luxury / color-led`
- `stem_finish: auto / open / partial / covered`

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

Assign color work across **flowers, foliage, wrapping, and ribbon**.

Rules:
- the bouquet should still feel related to the source at thumbnail size;
- vivid references must not collapse into generic pastel floristry;
- do not give every source color equal flower coverage;
- large flat color fields are often better carried by wrapping than by extra flower species;
- matching isolated swatches is not enough if the relationship between them feels wrong.

### Selective gradient policy

Gradient is a tool, not a default style.

Use it only when the source contains a meaningful color drift or one controlled transition materially improves the bouquet.

Good uses:
- a narrow bridge where cool genuinely drifts into warm;
- one preserved/dyed flower family with believable petal-edge or center-to-edge ombré;
- hydrangea, rose, carnation, orchid, fine foliage, or wrapping with a source-aligned transition;
- layered translucent wrapping that connects two strong color fields.

Rules:
- default to **1–2 gradient moments at most**;
- keep solid-color anchor flowers;
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
Start from mature, commonly used preserved-flower families before unusual sculptural materials.

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

Keep foliage subordinate unless the reference is explicitly botanical or forest-led. Flowers should normally occupy the clear visual majority of the bouquet face.

Do not let one oversized broad leaf, spathe, tropical foliage mass, or sculptural botanical dominate merely because its shape resembles part of the source. Anthurium, calla, large leaves, and similar materials are optional accents, not default hero choices.

Prefer **3–5 strong material families** over many small species.

## 5. Verify unusual materials instead of inventing them

For `preserved`, `hybrid`, and `art` modes, use florist-sourceable materials.

When web/catalog access is available:
- verify unusual preserved types, extreme colors, metallic finishes, gradient treatments, or specialty foliage against a current supplier catalog;
- prefer established supplier families such as Florever, RoseAmor, Verdissimo, or equivalent regional suppliers;
- do not invent a variety, color, or treatment simply because it would be convenient.

If an exact material is uncertain, use a verified substitute and state it in the build sheet.

Hidden florist wire/tape may be used for preserved-flower assembly, but it must not become a visible design element.

## 6. Design the wrapping architecture

Wrapping is a **structural design system**, not merely a color choice.

Choose one primary wrapping architecture that suits the bouquet:
- **open fan** — airy, spread, casual or color-led;
- **asymmetric wing** — sharper, editorial, directional;
- **nested cone** — compact, polished, giftable;
- **layered collar** — fuller edge framing around the bouquet face;
- **half-enclosed** — flowers stay open while the lower body is visually finished;
- **covered base / handle sleeve** — clean premium finish, especially suitable for preserved or editorial bouquets.

Choose material by both appearance and behavior:
- matte florist paper;
- translucent / frosted paper;
- soft tissue;
- structured paper;
- organza or fine mesh when appropriate;
- ribbon with suitable width, sheen, and stiffness.

Design the wrap by:
- hue and value;
- translucency and sheen;
- stiffness and fold behavior;
- number and direction of layers;
- edge rhythm and silhouette;
- relation to focal flowers and negative space.

Use wrapping to carry large neutral, dark, or saturated source fields instead of forcing flowers to do all color work.

A subtle layered fade or gradient is allowed only when it corresponds to the source and improves the transition.

Avoid generic default wrapping when a deliberate silhouette would materially improve the bouquet. Do not print the source image, text, logo, or recognizable artwork on the wrapping.

## 7. Decide the stem / handle finish

Exposed stems are **optional**, not mandatory.

Choose `open`, `partial`, or `covered` according to the bouquet rather than using the same finish every time.

Prefer **open stems** when:
- fresh flowers and natural garden character are important;
- visible stems add authenticity, lightness, or casual elegance;
- the stems are clean, balanced, and visually intentional.

Prefer **partial or covered stems** when:
- using preserved / hybrid / art mode;
- the bouquet is premium, editorial, compact, or gift-ready;
- exposed stems would look thin, rough, sparse, uneven, or unfinished;
- the lower silhouette benefits from a wrapped sleeve or complete base.

Rules:
- never expose stems merely because bouquets often show stems;
- exposed stems must be neat and proportionate;
- concealed stems must look like believable florist wrapping, not a vase or solid pedestal;
- the lower third must feel as resolved as the bouquet face.

## 8. Design the bouquet, not a color pile

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

## 9. Beauty gate

Reject and regenerate if any are true:
- **Color failure:** dominant / secondary / accent relationships are noticeably weaker than the source.
- **Relationship failure:** individual hues may be close, but the source's cool/warm, light/dark, or overlap logic is missing.
- **Gradient failure:** gradient is missing where it matters, placed in the wrong area/direction, or overused as decoration.
- **Flower-form failure:** main visible materials are bulky, awkward, leaf-heavy, or less attractive than a simpler flower-led solution.
- **Wrapping-shape failure:** the wrap color is acceptable but its architecture, layering, folds, or silhouette feel generic or awkward.
- **Handle failure:** stems/base look messy, thin, unfinished, overexposed, or inconsistent with the bouquet style.
- **Finish failure:** the bouquet face feels designed but the lower section does not.
- **Design failure:** no clear focal hierarchy, weak rhythm, flat depth, mechanical symmetry, or obvious color piles.
- **Generic failure:** pleasant but interchangeable with a standard catalog bouquet.
- **Depiction failure:** flowers collectively form a face, body, object, logo, picture, scene, or source-specific shape.
- **Prop failure:** visible cards, text, graphics, wire frameworks, lights, electronics, or unrelated inserts appear.
- **Reality failure:** material/color/gradient is invented, construction is implausible, or the build sheet cannot source/reproduce the visible result.

The target is:

> **recognizable palette + correct color relationships + selective justified gradients + beautiful flower forms + deliberate wrapping architecture + resolved handle finish + memorable bouquet design + florist reproducibility + zero literal source content**

## 10. Generate from a short florist brief

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
- wrapping architecture, materials, layers, and ribbon;
- stem / handle finish;
- color-faithful product/editorial photography.

Useful prompt shape:

> Editorial-quality, florist-producible hand-tied bouquet; [mode]; flower-led composition with [hero move]; [materials + counts + treatments]; [palette roles and direction]; [selective gradient moment only if justified]; clear focal/support/bridge hierarchy; varied flower scale and depth; restrained foliage; intentional negative space; [wrapping architecture + materials + layering]; [open/partial/covered handle finish]; neutral color-faithful lighting; believable botanical detail.

Keep the prompt positive and florist-specific.

## 11. Florist Build Sheet

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
- Architecture: open fan / asymmetric wing / nested cone / layered collar / half-enclosed / covered base
- Outer wrap: ...
- Inner layer: ...
- Ribbon: ...
- Visual role: ...
- Stem finish: open / partial / covered

## Assembly
1. Establish focal, movement, and depth.
2. Add support with unequal scale and height.
3. Add bridge materials and any selective gradient moment without flattening palette contrast.
4. Build the chosen wrapping architecture and finish the stems/base intentionally.

## Substitutions
- ... → ...

## Must preserve
- ...
- ...
```

The build sheet must match the final image exactly and disclose preserved, dyed, dried, artificial, and gradient-treated materials when used.