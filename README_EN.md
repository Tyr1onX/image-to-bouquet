# Image to Bouquet

> Give it an image. Get a bouquet.

`image-to-bouquet` is an Agent / Codex Skill that translates the **color, composition, texture, mood, and visual identity** of a reference image into a bouquet that can actually be made by a florist.

## Input

Any reference image: a photo, album cover, poster, illustration, film still, logo, game screenshot, and more.

## Output

A complete run must always deliver both:

1. **Bouquet image** — a visual render of the final bouquet design.
2. **Florist build sheet** — flowers, counts/proportions, wrapping, dimensions, structure, assembly order, substitutions, and visual constraints.

**Text-only analysis, a prompt, or a palette is not a finished result.**

## Core idea

```text
Reference Image
→ Visual DNA
→ Bouquet Translation
→ Buildable Bouquet Spec
→ Bouquet Image
```

Do not literally copy objects from the image. Preserve its visual identity:

- `Color → flowers / wrapping / ribbon`
- `Composition → silhouette / height / density / visual weight`
- `Texture → materials and floral texture`
- `Symbol → restrained identifying accents`
- `Mood → saturation / negative space / restraint`

The rendered image and the florist build sheet must describe **the same bouquet**, with real-world buildability taking priority over visual gimmicks.

## Usage

Install the repository's `SKILL.md`, then give the Agent an image and ask, for example:

> Turn this image into a bouquet. Generate the bouquet image and a florist-ready build plan.

The Skill should infer the design from the image instead of forcing the user through a long questionnaire.

## Status

Early version. The current focus is the visual translation model, mandatory image output, and reliable florist-executable constraints.

---

[中文](README.md)
