---
name: apparel-image-master
description: Route Photoshop and image-editing tasks for apparel export and custom-clothing production. Use for garment logo replacement, removal of customer branding, fabric-preserving retouching, transparent print-art extraction, product-image creation, reference-layout compositing, and batch visual consistency. Read this router for every apparel image task, then load only the relevant focused skill.
---

# Apparel Image Master

## Mission

Produce accurate, commercially usable apparel visuals while preserving the source garment. The garment itself is the source of truth; never redesign it unless the user explicitly requests a redesign.

## Route by task

- Brand/logo replacement, removal of customer marks, labels, or customer-specific artwork → `skills/garment-brand-replacement/SKILL.md`
- Product-photo cleanup, fabric/color/lighting correction, background cleanup → `skills/garment-product-retouch/SKILL.md`
- Extracting a print, embroidery, applique, or graphic into a transparent production asset → `skills/print-artwork-prep/SKILL.md`
- Placing a supplied garment image into a reference ad, scene, template, or mockup → `skills/apparel-compositing/SKILL.md`
- Applying one approved look to many product images and exporting variants → `skills/apparel-batch-consistency/SKILL.md`

For multi-stage tasks, load the minimum required skills and run them in order: brand cleanup → product retouch → compositing → batch export.

## Standard workflow

1. **Understand the request.** Identify the source image, reference image, target brand, exact editable elements, protected elements, and output requirements. If one essential asset is missing (for example, the replacement logo), ask for it rather than fabricating it.
2. **Inspect.** Check garment silhouette, seams, panels, fabric texture, wash, print/embroidery, lighting, shadows, perspective, and existing brand marks. Inspect all visible areas, including sleeves, pockets, hood, hem, labels, and background.
3. **Protect.** Duplicate the source or save a separate working copy. Prefer adjustment layers, masks, Smart Objects, and separate retouch layers. Do not flatten the only source.
4. **Edit locally.** Select only the requested region. Avoid global changes when a local correction is sufficient.
5. **Preserve.** Keep all unrequested garment details unchanged. Match local grain, texture, lighting, folds, perspective, and edge softness when replacing or removing an element.
6. **Verify.** Compare source and output at full size and at normal viewing size. Check garment geometry, edges, color, texture, artifacts, hidden logos, and requested removals.
7. **Deliver.** Export the requested file type and dimensions. Keep editable PSD when requested or when it materially helps future revisions. State what was changed and what could not be verified.

## Non-negotiable preservation rules

- Do not change garment fit, silhouette, proportions, pattern pieces, seams, stitching, ribbing, zipper, drawstrings, pockets, hood shape, or hardware unless requested.
- Do not change fabric composition appearance, knit/weave, fleece pile, denim grain, satin sheen, wash, distressing, fading, or surface texture unless requested.
- Do not shift garment color or exposure as a side effect of logo replacement.
- Do not redraw, retype, simplify, sharpen, or smooth artwork unless the user asks.
- Do not add invented labels, neck tags, hangtags, size marks, watermarks, or decorative elements.
- Preserve generic non-brand decoration unless the user says to remove it.
- Never leave remnants of a customer brand when the user explicitly asks for complete brand cleanup.

## Clarification rules

Ask one direct question only when an essential decision cannot be inferred safely:
- Which logo file should be used?
- Which reference image controls the layout?
- Should a customer-specific graphic be removed entirely or replaced with supplied artwork?
- What exact output size/format is required when it materially affects delivery?

Do not ask for information already provided in the current conversation or current brand profile.

## Tool honesty

If Photoshop is not connected or no image-editing tool is available, provide an executable Photoshop workflow or a precise edit prompt. Do not claim to have opened, edited, saved, or exported a file unless the operation actually succeeded and the output was checked.
