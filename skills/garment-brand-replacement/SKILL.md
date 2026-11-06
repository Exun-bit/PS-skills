---
name: garment-brand-replacement
description: Remove customer logos, brand names, proprietary marks, and customer-specific graphics from apparel images, then apply the user's currently authorized brand identity while preserving the garment and the original visual treatment. Use whenever the user requests logo replacement or brand cleanup on clothing.
---

# Garment Brand Replacement

## Default interpretation

When the user asks to replace a garment brand/logo:
1. Remove the original customer brand name, logo, monogram, proprietary symbol, and other customer-identifying graphic elements from the requested garment areas.
2. Apply the currently authorized brand identity from the current brand profile, unless the user names another brand or supplies another logo.
3. Preserve the garment design and all unrelated generic decoration.

Do not interpret "replace the logo" as permission to redesign the garment.

## Brand source priority

Use this order:
1. Logo/artwork file supplied in the current task.
2. Explicit brand and logo choice in the current conversation.
3. Latest confirmed brand profile in `profiles/current-brand.md`.

A brand name typed in text is not a substitute for the actual logo artwork when visual fidelity matters. If the logo file is unavailable, ask the user to upload it or ask whether a clean text-only treatment is acceptable. Never invent a logo.

The brand profile is configurable. Do not hard-code YuMu or any other company into the reusable workflow.

## What to remove

Remove all customer-specific brand identifiers visible in the requested scope, including:
- Original logo, wordmark, monogram, slogan, and branded emblem.
- Customer brand text and proprietary symbols.
- Customer-specific print/graphic artwork when the user has asked for complete removal or replacement.
- Branded labels and tags if they are visible and included in the requested cleanup.

Do not leave partial letters, ghosting, color halos, stitch remnants, or recognizable fragments.

## What may remain

Preserve generic design elements that are not customer identifiers, unless instructed otherwise:
- Generic stars, stripes, flames, abstract shapes, numbers used decoratively, distressing, and non-branded motifs.
- Garment construction details, seams, topstitching, panels, pockets, hardware, and fabric effects.
- Generic decorative artwork that the user has not asked to remove.

If a motif could reasonably be a customer-specific logo or proprietary graphic, ask or remove it according to the user's explicit scope. Do not assume every graphic is generic.

## Placement and material matching

Before placing the new mark, determine:
- Garment surface orientation and perspective.
- Fabric type and texture (jersey, fleece, denim, satin, leather, etc.).
- Print/embroidery technique (screen print, DTG, puff print, flat embroidery, applique, etc.).
- Scale, rotation, distortion, edge character, color, opacity, and position.

Match the original production appearance only when the user wants a like-for-like replacement. Otherwise follow the supplied logo and placement reference. For embroidery, simulate thread direction, stitch relief, edge density, and shadow only to the extent supported by the source/reference. Do not falsely describe a visual simulation as a real production file.

## Special label rule

Do not add or retain a main label or neck label unless the user explicitly requests it. Do not invent size labels or care labels.

## Photoshop procedure

1. Duplicate the source layer/document and name the copy clearly.
2. Inspect every visible brand-bearing region.
3. Use selections and masks to isolate each mark.
4. Remove the old mark with the least destructive suitable method: clone/heal/content-aware fill or a generative tool where necessary. Rebuild folds, texture, and grain from nearby valid source areas.
5. Inspect the cleaned region before adding the new mark. If removal damages seams or fabric structure, repair that first.
6. Place the supplied replacement logo as a Smart Object where possible.
7. Transform and warp it to the garment plane. Match local perspective and curvature; avoid stretching the logo disproportionately.
8. Match the material/print treatment with appropriate blend modes, displacement, texture, and restrained lighting effects.
9. Inspect at 100% for halos, repeated texture, hard edges, incorrect perspective, and residual original branding.
10. Toggle the original and edited layers to compare. Confirm that all non-target garment features remain stable.

## Completion checklist

- [ ] Original customer brand marks removed from the requested scope.
- [ ] No partial text, ghosting, or recognizable logo fragments remain.
- [ ] Correct current logo used; no invented logo.
- [ ] Logo placement, scale, perspective, and material appearance are plausible.
- [ ] Garment color, silhouette, seams, folds, fabric texture, wash, and construction preserved.
- [ ] Generic motifs retained unless explicitly excluded.
- [ ] No unrequested main/neck label added.
- [ ] Output visually checked at 100% and normal viewing size.
