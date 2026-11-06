---
name: garment-brand-replacement
description: Remove customer logos, brand names, proprietary marks, and customer-specific graphics from apparel images, then apply an authorized replacement identity while preserving the garment and the original visual treatment. Use whenever the user requests logo replacement, brand cleanup, or source-logo transfer on clothing.
---

# Garment Brand Replacement

## Core objective

Treat the garment photo as the source of truth.

The task is **local pixel editing**, not a redesign or image regeneration. Change only the requested brand-bearing regions. Preserve every unrelated garment detail.

## Brand source priority

Use the following order:

1. Replacement logo/artwork file supplied in the current task.
2. An explicit logo/brand choice stated in the current conversation.
3. The latest confirmed brand profile in `profiles/current-brand.md`.

### Source-image logo fallback

If the user explicitly says to use a logo already visible in the product/source image as the replacement reference, this is allowed.

In that case:

- Isolate the visible logo artwork from the source image.
- Treat it as a **reference/transfer source**, not as permission to invent a new logo.
- Preserve its letterform, proportions, color, distressing, and production appearance as closely as the source permits.
- If the requested operation would place the exact same logo back in exactly the same location, do not pretend that a replacement occurred. Report that the source logo is unchanged and that the test cannot validate brand-removal behavior from that image alone.
- If the user wants to test the replacement pipeline, apply the source-derived logo to a different target region/image where an actual replacement can be verified.

A typed brand name is not automatically a substitute for logo artwork when visual fidelity matters. Never invent a proprietary logo.

## Scope of removal

When the user requests complete brand cleanup, remove all customer-specific identifiers in the requested scope:

- Wordmarks and brand names.
- Logos, monograms, emblems, symbols and slogans.
- Customer-specific branded graphics.
- Branded labels/tags when included in the requested area.

Do not leave:

- Partial letters.
- Ghosted shapes.
- Color halos.
- Stitch remnants.
- Shadow remnants that reveal the old mark.
- Recognizable fragments.

## Elements that remain

Preserve unrelated generic design elements unless the user explicitly asks for removal:

- Generic stars, stripes, flames, abstract shapes and decorative numbers.
- Distressing, cracks, fading and wash effects.
- Seams, topstitching, panels, pockets and hardware.
- Fabric grain, weave, knit/fleece texture and local lighting.

If a graphic could reasonably be a proprietary brand element, follow the user's stated scope instead of guessing.

## Protected garment features

Unless explicitly requested, do not alter:

- Silhouette, fit, proportions or pattern pieces.
- Hood, sleeves, cuffs, hem and ribbing.
- Zipper, drawcords, snaps, buttons and hardware.
- Pocket geometry and stitching.
- Fabric color, wash, distressing and texture.
- Existing non-target prints or embroidery.
- Background, camera angle, perspective and shadows.

## Replacement procedure

### Phase 1 — Inspect

Before editing, identify:

1. Every brand-bearing region.
2. The exact target area.
3. The garment surface orientation.
4. The production technique: screen print, DTG, puff print, embroidery, applique, etc.
5. The local texture, grain, folds, lighting and shadow.

Do not begin replacement until the target region is isolated conceptually.

### Phase 2 — Remove

Use a separate retouch layer or duplicated source.

1. Mask/select only the old brand area.
2. Remove the old mark using the least destructive suitable method.
3. Reconstruct the underlying fabric/print surface from valid nearby pixels.
4. Preserve seams, folds, texture and garment construction crossing the target area.
5. Inspect the cleaned area **before** placing the replacement.

### Phase 3 — Place

Place the authorized replacement as a separate layer or Smart Object where possible.

Match:

- Position.
- Scale.
- Rotation.
- Perspective/warp.
- Surface curvature.
- Opacity.
- Edge softness.
- Color.
- Distressing.
- Print/embroidery character.

Do not flatten the replacement into the source until verification is complete.

### Phase 4 — Material integration

The replacement must visually belong to the garment.

For printed artwork, match the source's:

- Ink density.
- Fabric interaction.
- Cracking/distressing.
- Local folds.
- Grain and texture.
- Lighting and shadow.

For embroidery, match only what can be supported by the reference:

- Thread direction.
- Stitch density.
- Relief.
- Edge structure.
- Local shadow.

Do not claim a simulated effect is a production-ready embroidery file.

## Mandatory verification gate

A replacement is **NOT complete** until all checks pass.

### A. Brand-removal check

At 100% zoom:

- No original letters remain.
- No original logo fragments remain.
- No ghosting/halo remains.
- No old brand color remains in the cleaned region.
- No original outline is visible beneath the replacement.

### B. Replacement check

- Correct authorized logo/reference was used.
- Correct placement.
- Correct scale and perspective.
- Correct material/print treatment.
- No accidental duplication or deformation.

### C. Garment-preservation check

Compare source vs output:

- Silhouette unchanged.
- Seams unchanged.
- Pockets unchanged.
- Hardware unchanged.
- Fabric texture unchanged outside the edit.
- Color/wash unchanged.
- Lighting/shadows unchanged except where the replacement naturally affects them.

### D. Residual-brand sweep

Inspect the whole image, not only the main chest area:

- Front.
- Back.
- Sleeves.
- Hood.
- Pockets.
- Hem.
- Neck/labels.
- Any visible secondary graphics.

If a customer brand remains within the user's requested cleanup scope, the result is **FAIL**.

## Pass / Fail criteria

### PASS

All four verification gates pass and the output preserves the source garment.

### FAIL

Any of these is an automatic failure:

1. Original brand remains readable.
2. Original logo is still visible underneath the replacement.
3. Replacement logo is missing or clearly incorrect.
4. Garment construction is materially changed.
5. Texture/lighting is obviously regenerated or inconsistent.
6. Unrequested graphics or labels are added.
7. The output cannot be compared reliably with the source because the garment was substantially regenerated.

When a generated image fails, do not describe it as a successful edit. Return to the source and use a more controlled local-edit workflow.

## Photoshop procedure

1. Duplicate the source document/layer.
2. Create a dedicated group named `BRAND_REPLACEMENT`.
3. Keep `SOURCE_ORIGINAL` untouched.
4. Create one mask/retouch layer per brand-bearing region.
5. Clean the old mark first.
6. Place the replacement on its own layer/Smart Object.
7. Warp/transform to the garment surface.
8. Add only the minimum material integration required.
9. Toggle source/output visibility to compare.
10. Inspect at 100%.
11. Inspect at normal viewing size.
12. Run the residual-brand sweep.
13. Save an editable PSD when requested or useful.
14. Export the requested final format.

## Generative-image limitation

Generative image tools may change unrelated garment details, typography, seams, fabric texture or proportions. Therefore:

- Do not treat a regenerated image as equivalent to a Photoshop local edit.
- Use generative tools only when the task explicitly permits regeneration or when no controlled editor is available.
- For exact apparel preservation, prefer masks, clone/heal, content-aware fill, Smart Objects and local transforms.
- If a generated result changes protected garment features or retains the old brand, mark it **FAIL** rather than accepting it because it looks plausible.

## Special label rule

Do not add or retain a main label or neck label unless explicitly requested. Do not invent size labels, care labels or hangtags.

## Completion report

After editing, report only:

- What brand-bearing elements were removed.
- What replacement reference was used.
- Whether garment-preservation checks passed.
- Any limitation that could not be verified.

Never claim Photoshop operations, file saves, exports or visual checks that were not actually performed.
