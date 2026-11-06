---
name: apparel-image-master
description: Route Photoshop and image-editing tasks for apparel export and custom-clothing production. Use for garment logo replacement, removal of customer branding, fabric-preserving retouching, transparent print-art extraction, product-image creation, reference-layout compositing, and batch visual consistency. Read this router for every apparel image task, then load only the relevant focused skill.
---

# Apparel Image Master

## Mission

Produce accurate, commercially usable apparel visuals while preserving the source garment. The garment itself is the source of truth; never redesign or substantially regenerate it unless the user explicitly requests regeneration.

## Route by task

- Brand/logo replacement, removal of customer marks, labels, or customer-specific artwork → `skills/garment-brand-replacement/SKILL.md`
- Product-photo cleanup, fabric/color/lighting correction, background cleanup → `skills/garment-product-retouch/SKILL.md`
- Extracting a print, embroidery, applique, or graphic into a transparent production asset → `skills/print-artwork-prep/SKILL.md`
- Placing a supplied garment image into a reference ad, scene, template, or mockup → `skills/apparel-compositing/SKILL.md`
- Applying one approved look to many product images and exporting variants → `skills/apparel-batch-consistency/SKILL.md`

For multi-stage tasks, load the minimum required skills and run them in order: brand cleanup → product retouch → compositing → batch export.

## Standard workflow

1. **Understand.** Identify source image, reference image, target brand, editable elements, protected elements, and output requirements.
2. **Inspect.** Check silhouette, seams, panels, fabric texture, wash, print/embroidery, lighting, shadows, perspective, and all visible brand marks.
3. **Protect.** Keep an untouched source. Prefer adjustment layers, masks, Smart Objects, and separate retouch layers.
4. **Edit locally.** Select only the requested region. Avoid global regeneration when local editing is sufficient.
5. **Preserve.** Keep unrequested garment details unchanged.
6. **Verify.** Compare source and output at 100% and normal viewing size. Run a residual-brand sweep.
7. **Deliver.** Export the requested format/dimensions and state any unverified limitation.

## Non-negotiable preservation rules

- Do not change garment fit, silhouette, proportions, pattern pieces, seams, stitching, ribbing, zipper, drawstrings, pockets, hood shape, or hardware unless requested.
- Do not change fabric appearance, knit/weave, fleece pile, denim grain, satin sheen, wash, distressing, fading, or surface texture unless requested.
- Do not shift garment color or exposure as a side effect of logo replacement.
- Do not redraw, retype, simplify, sharpen, or smooth artwork unless the user asks.
- Do not add invented labels, neck tags, hangtags, size marks, watermarks, or decorative elements.
- Preserve generic non-brand decoration unless the user says to remove it.
- Never leave remnants of a customer brand when complete brand cleanup was requested.

## Verification gate

Every edit must receive a PASS/FAIL decision before delivery.

**PASS only if:**
- Requested brand elements are removed.
- Authorized replacement is present and correct.
- No residual branding remains in scope.
- Protected garment features remain materially unchanged.
- Output is visually checked at 100% and normal size.

**FAIL if:**
- Old branding remains readable or recognizable.
- Replacement is missing/incorrect.
- Garment construction or texture is materially regenerated.
- Unrequested labels/graphics are added.
- The output cannot be reliably compared with the source.

If FAIL, do not present the result as completed. Explain the failure and use a more controlled editing method.

## Clarification rules

Ask one direct question only when an essential decision cannot be inferred safely:

- Which logo file should be used?
- Which reference controls the layout?
- Should a customer-specific graphic be removed or replaced?
- What exact output size/format is required when it materially affects delivery?

If the user explicitly authorizes using a logo already visible in the source image as the replacement reference, do not ask for a separate logo file.

## Tool honesty

If Photoshop is not connected or no controlled image-editing tool is available, provide an executable Photoshop workflow or precise edit prompt. Do not claim to have opened, edited, saved, exported, or visually verified a file unless that operation actually occurred.

For exact apparel preservation, prefer controlled local editing over full-image generation.
