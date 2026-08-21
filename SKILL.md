---
name: image-to-bouquet
description: Turn one reference image into one visually faithful, florist-producible bouquet. Support fresh, preserved, hybrid, and art modes. Preserve palette, color relationships, rhythm, mood, material character, wrapping language, and finish without copying source content. Output one final bouquet image plus one concise Chinese florist execution sheet.
---

# Image to Bouquet

Turn one reference image into **one beautiful bouquet that a florist can actually reproduce**.

The result must read first as a professionally designed bouquet, never as the source image rebuilt with flowers.

A complete run has exactly two deliverables:

1. one standalone final bouquet image;
2. one concise **Chinese** florist execution sheet for that exact bouquet.

Do not stop after image generation.

## 1. Resolve preferences

Support optional controls. If unspecified, choose automatically.

### Material mode
- `auto` — choose the best mode
- `fresh` — fresh flowers and foliage
- `preserved` — preserved flowers/botanicals first
- `hybrid` — fresh + preserved / dried / dyed botanicals
- `art` — visual fidelity first; high-quality artificial botanicals may also be used

Recommended auto behavior:
- natural portrait / landscape / gift use → `fresh` or `hybrid`
- album cover / poster / strong graphic palette → `preserved` by default
- metallic / neon / hard-to-source natural palette → `hybrid` or `art`

Other optional controls:
- color fidelity: `natural / balanced / strict`
- design intensity: `safe / editorial / bold`
- budget: `low / medium / high`
- wrapping: `minimal / commercial / editorial / luxury / color-led`
- stem finish: `auto / open / partial / covered`

Explicit user choices override auto selection.

## 2. Extract design language, not source content

Transfer only:
- dominant / secondary / accent colors and rough proportions;
- broad color placement and visual weight;
- warm/cool, light/dark, muted/saturated relationships;
- rhythm, movement, depth, negative space;
- material feel and mood.

Never transfer:
- source subject or silhouette;
- face/body geometry;
- object/building contours or scene layout;
- graphic linework;
- text, logos, symbols, printed artwork, or recognizable source fragments.

**Composition may survive; depiction may not.**

After analysis, create a short internal floral brief with no source-specific nouns. When possible, generate from that text brief rather than using the source image as an edit reference.

## 3. Lock palette relationships first

Before choosing flowers, define 3–5 palette roles:
- dominant;
- secondary;
- bridge;
- accent;
- optional neutral / dark field.

For each role, lock:
- hue family;
- lightness;
- saturation;
- warm/cool bias;
- approximate visual share;
- broad position.

Also record the relationship:
- hard split or soft transition;
- clean block or blended overlap;
- dark-to-light lift;
- cool-to-warm drift;
- one dominant field with a small counter-color, or two near-equal poles.

Assign color work across **flowers, foliage, wrapping, and ribbon**.

Rules:
- the bouquet should remain related to the source at thumbnail size;
- vivid references must not collapse into generic pastel floristry;
- do not give every source color equal flower coverage;
- large flat fields are often better carried by wrapping than by extra flower species;
- matching isolated swatches is not enough if the relationships feel wrong.

### Selective gradient policy

Gradient is a tool, not a default style.

Use it only when the source contains meaningful color drift or one controlled transition improves fidelity.

Good uses:
- a narrow bridge where one palette genuinely drifts into another;
- one preserved/dyed flower family with believable petal-edge or center-to-edge ombré;
- hydrangea, rose, carnation, orchid, fine foliage, or wrapping with a source-aligned transition;
- layered translucent wrapping that connects two strong fields.

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

For preserved bouquets, start from mature, florist-friendly families:
- rose / garden rose;
- hydrangea;
- carnation;
- ranunculus-like flowers when genuinely available;
- mum / chrysanthemum families;
- orchids when genuinely available;
- gypsophila and fine preserved fillers;
- restrained eucalyptus and fine line botanicals.

Keep foliage subordinate unless the source is explicitly botanical. Flowers should normally occupy the clear visual majority of the bouquet face.

Do not let oversized broad leaves, spathes, tropical foliage masses, or awkward sculptural botanicals dominate merely because their shape resembles part of the source.

Prefer **3–5 strong material families** over many weak species.

For preserved / hybrid / art modes, verify unusual flower types, extreme colors, metallic finishes, gradient treatments, or specialty foliage against real florist/supplier availability when web/catalog access exists. Do not invent convenient materials.

Hidden florist wire/tape is allowed for construction, but never as a visible design element.

## 5. Design wrapping architecture

Wrapping is a **structural design system**, not merely a color choice.

Choose one primary architecture:
- `open fan` — airy, spread, casual or color-led;
- `asymmetric wing` — sharper, editorial, directional;
- `nested cone` — compact, polished, giftable;
- `layered collar` — fuller framing around the bouquet face;
- `half-enclosed` — open flowers with a more finished lower body;
- `covered base` — clean premium finish, especially suitable for preserved/editorial bouquets.

Choose wrapping by:
- hue and value;
- translucency and sheen;
- stiffness and fold behavior;
- number and direction of layers;
- edge rhythm and outer silhouette;
- relation to focal flowers and negative space.

Possible materials include matte florist paper, translucent/frosted paper, soft tissue, structured paper, organza, fine mesh, and suitable ribbon.

Use wrapping to carry large neutral, dark, or saturated fields instead of forcing flowers to do all color work.

A subtle layered fade or gradient is allowed only when it corresponds to the source and improves the transition.

Do not print source imagery, text, logos, or recognizable artwork on the wrapping.

## 6. Decide stem / handle finish

Exposed stems are optional, not mandatory.

Choose `open`, `partial`, or `covered` according to the bouquet.

Prefer open stems when:
- fresh flowers and natural garden character are important;
- visible stems add lightness or authenticity;
- stems are clean, balanced, and intentional.

Prefer partial or covered stems when:
- using preserved / hybrid / art mode;
- the bouquet is premium, editorial, compact, or gift-ready;
- exposed stems would look thin, rough, sparse, uneven, or unfinished;
- the lower silhouette benefits from a wrapped sleeve or complete base.

Rules:
- never expose stems just because bouquets often show stems;
- exposed stems must be neat and proportionate;
- concealed stems must look like believable florist wrapping, not a vase or hard pedestal;
- the lower third must feel as resolved as the bouquet face.

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
- focal — unmistakable first read;
- support — balances without mirroring;
- bridge — connects color groups without averaging them;
- line / movement — botanical only;
- depth — front / middle / upper-rear;
- negative space — enough breathing room to avoid a flower wall.

If the result can be summarized as `one pile per color`, redesign it.

## 8. Beauty gate

Reject and regenerate if any are true:
- palette relationships are noticeably weaker than the source;
- individual hues are close but cool/warm, light/dark, or overlap logic is wrong;
- gradient is missing where it matters, placed wrongly, or overused;
- main materials are bulky, awkward, leaf-heavy, or less attractive than a simpler flower-led solution;
- wrapping architecture, layering, folds, or silhouette feel generic or awkward;
- stems/base look messy, thin, unfinished, overexposed, or inconsistent with the bouquet style;
- the bouquet face feels designed but the lower section does not;
- no clear focal hierarchy, weak rhythm, flat depth, mechanical symmetry, or obvious color piles;
- the result is pleasant but interchangeable with a generic catalog bouquet;
- flowers collectively form a face, body, object, logo, picture, scene, or source-specific shape;
- visible cards, text, graphics, wire frameworks, lights, electronics, or unrelated inserts appear;
- material/color/gradient is invented, construction is implausible, or the execution sheet cannot reproduce the visible result.

Target:

> recognizable palette + correct color relationships + selective justified gradients + beautiful flower forms + deliberate wrapping architecture + resolved handle finish + memorable bouquet design + florist reproducibility + zero literal source content

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
- wrapping architecture, materials, layers, and ribbon;
- stem / handle finish;
- neutral color-faithful product/editorial photography.

Keep the generation prompt positive and florist-specific.

## 10. Final user-facing output contract

This section is mandatory.

### Language

Unless the user explicitly requests another language, **all user-visible text must be Chinese**.

Internal English keywords may be used for reasoning only. Never expose raw internal values such as `preserved`, `strict`, `editorial`, `asymmetric wing`, `covered`, `focal`, `support`, or `bridge` in the final response.

Use these Chinese equivalents when needed:
- fresh → 鲜花
- preserved → 永生花
- hybrid → 混合花材
- art → 艺术花材
- natural → 自然
- balanced → 平衡
- strict → 严格
- safe → 克制
- editorial → 编辑感
- bold → 大胆
- open → 露枝
- partial → 半包
- covered → 全包
- open fan → 开放扇形
- asymmetric wing → 非对称翼形
- nested cone → 嵌套锥形
- layered collar → 层叠围边
- half-enclosed → 半包围
- covered base → 覆盖式底部

### Output only the finished result

Do **not** output any of the following unless the user explicitly asks:
- installation/update/version status;
- test iteration labels such as “第六版”;
- “已安装最新版”“已完成测试”等 process chatter;
- local filesystem paths;
- raw output file paths or “查看图片” links to local paths;
- Git commit / branch / PR information;
- supplier verification notes or supplier links;
- web citations or sourcing links;
- internal prompt, internal recipe, audit log, or regeneration history;
- English headings, English role names, or English mode names.

If web/catalog verification was used, use it silently to choose valid materials. Only mention sourcing details if the user asks.

### Final structure

The final response contains only:

1. the final bouquet image, presented through the platform’s image/file output mechanism without printing a local path;
2. the following concise Chinese execution sheet.

Use **bullets instead of a Markdown table** for materials to avoid broken table rendering.

```markdown
# 花艺师执行单

## 设计
- 尺寸：小 / 中 / 大（可补充约宽 × 高）
- 材质模式：鲜花 / 永生花 / 混合花材 / 艺术花材
- 色彩还原：自然 / 平衡 / 严格
- 设计强度：克制 / 编辑感 / 大胆
- 核心视觉：……
- 记忆点：……
- 主花 / 支撑 / 过渡：……
- 渐变：无 / 轻微 / 适中；说明位置与作用

## 花材
- …… × 数量｜类型｜颜色或处理｜作用
- …… × 数量｜类型｜颜色或处理｜作用

## 包装
- 包装结构：开放扇形 / 非对称翼形 / 嵌套锥形 / 层叠围边 / 半包围 / 覆盖式底部
- 外层：……
- 内层：……
- 丝带：……
- 视觉作用：……
- 花杆处理：露枝 / 半包 / 全包

## 制作
1. ……
2. ……
3. ……
4. ……

## 可替代
- …… → ……

## 必须保留
- ……
- ……
```

Keep the execution sheet concise. Do not repeat design reasoning, testing history, source-analysis notes, or procurement research.

The execution sheet must match the final image exactly and disclose preserved, dyed, dried, artificial, or gradient-treated materials when used.