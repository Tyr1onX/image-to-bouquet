---
name: image-to-bouquet
description: Turn any reference image into one realistic, cost-conscious, florist-reproducible bouquet. Use for ordinary photos, landscapes, personal photography, posters, illustrations, album art, film stills, or any other image whose color, geometry, texture, and visual mood should be translated into floral form. A complete run shows the reference separately, generates one clean bouquet image, and provides a separate florist build sheet.
---

# Image to Bouquet

Turn **one image into one real bouquet**.

The source may be anything. Treat it as a source of **high-level visual language**, not content to reproduce.

## Read only four layers

1. **Color hierarchy** — dominant / secondary / accent colors and rough proportions.
2. **Geometry** — tall/wide, centered/asymmetric, dense/airy, major blocks, direction and negative space.
3. **Texture** — soft, rough, glossy, matte, translucent, metallic, natural, geometric, etc.
4. **Mood** — calm, playful, cold, warm, dreamy, restrained, dramatic, nostalgic, futuristic, etc.

Do not reconstruct the scene, characters, typography, logos, buildings, objects or artwork details.

## Safe abstraction

For third-party artwork, branded media, posters, album art, film stills, illustrations or logos, use the source **only as high-level inspiration**.

First reduce it internally to a neutral description, for example:

> deep navy dominant field + one concentrated lime-green mass + tiny warm-yellow accents + energetic asymmetric composition

Design from that abstraction. Do not ask the image model to recreate, trace, restage, extend or closely imitate the protected work. Do not reproduce recognizable characters, logos, text or signature objects.

Use the same abstraction method for ordinary photos and user-created images; this keeps the Skill general rather than dependent on copyrighted media.

## Translate

```text
Color    → flowers / foliage / wrapping / ribbon
Geometry → silhouette / height / width / focal position / spacing
Texture  → flower surface / foliage / paper finish / transparency
Mood     → saturation / restraint / density / negative space
```

Use the **fewest floral decisions needed**.

### Color hierarchy must survive

Do not merely extract colors; preserve their roles.

- A large dark/background field should usually be carried by wrapping, foliage or negative space instead of being lost.
- Preserve at least one meaningful secondary or accent color when it is important to the source identity.
- Do not turn a green-dominant photo into generic green-and-white if a dark mass or warm accent is what gives the image its identity.
- For many-color references, do not add a different flower species for every hue. Reuse one species in multiple available colors, use ribbon/wrapping, or reduce to the few strongest color groups.

## Reality + cost are hard constraints

Unless the user asks for luxury, default to a **cost-conscious S–M bouquet**:

- about 30–40 cm wide;
- about 3–5 floral/foliage material types total;
- about 7–12 visible main flower heads/stems;
- small amounts of filler/foliage only;
- at most 1–2 premium/specialty materials;
- prefer wrapping/ribbon/foliage over buying many extra flowers to carry a color.

Never generate floating objects, planets, portals, crystals, figurines, logos, printed source images, impossible flowers, unsupported decorations or CGI-like effects.

If a color is difficult in fresh flowers, prefer:
1. wrapping/ribbon;
2. common dyed/preserved/artificial floral material, disclosed in the build sheet;
3. nearest realistic flower color.

## Lock the recipe first

Before generation, decide:
- size and silhouette;
- 3–5 material types and counts/ranges;
- placement roles;
- wrapping and ribbon;
- cost level and cheaper substitutes;
- 2–4 `must preserve` decisions;
- 2–4 `avoid` decisions.

The recipe is authoritative. If the image violates it, regenerate/edit the image rather than changing the recipe afterward.

## Final image

Generate **one real florist product photo**:
- one finished bouquet only;
- simple studio/natural background;
- realistic flower scale and stem count;
- realistic florist wrapping;
- no text, palette, checklist, reference inset, moodboard, watermark or infographic;
- no recognizable source artwork, character, logo or typography.

Show the reference separately in the conversation/UI. Never composite it into the final bouquet image.

## Image quality and provenance — hard constraint

The final bouquet image must be the **direct standalone output of the host's native image-generation tool** for that one reference.

Do not use any of the following as the final bouquet image:
- a crop from a collage, contact sheet, infographic, comparison board or screenshot;
- an enlarged crop from another generated image;
- a thumbnail extracted from a multi-case render;
- a recompressed preview when the original direct generation is available;
- a Python/graphics reconstruction used as a substitute for native image generation.

Cropping, resizing or assembling images is allowed only for **secondary review/comparison sheets after the standalone bouquet images already exist**. Those secondary sheets must never replace the underlying direct outputs.

Before delivery, inspect image quality. Reject and regenerate if:
- flower-petal edges or wrapping textures are visibly soft because of cropping/upscaling/compression;
- the image is noticeably lower-detail than a normal direct generation;
- there are screenshot/UI borders or remnants of another layout;
- the result is not traceable to one direct image-generation call for one reference.

**One reference → one native image-generation call → one original bouquet image.**

## Batch / evaluation rule

Even when testing many references, **image generation is one reference per call**.

Never ask the image model to render a test matrix, contact sheet, before/after board, numbered gallery or evaluation infographic. Those may be assembled afterward outside the generator for review, but every underlying generated artifact must first be a clean standalone bouquet image.

When running golden-sample evaluations, keep the original direct bouquet files and compare them against the corresponding reference images. Never score a cropped or upscaled derivative as if it were the model's original result.

## Final check

Reject/revise if:
- the bouquet is generic and only vaguely matches the source palette;
- dominant/secondary/accent roles were flattened;
- an important dark mass, contrast anchor or small accent was lost;
- literal source content was copied instead of abstracted;
- anything is physically unreproducible;
- flower/species count is excessive for the visual effect;
- it looks unnecessarily expensive;
- image and build sheet disagree;
- the delivered bouquet image is not a crisp direct native generation.

The target is:

> **the simplest real bouquet that carries the reference image's color hierarchy, geometry, texture and mood without reproducing its protected content.**