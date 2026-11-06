---
name: print-artwork-prep
description: Extract, clean, crop, and prepare apparel print or graphic artwork as transparent PNG assets for DTG, screen-print reference, embroidery reference, and design software. Preserve original lettering, distressed texture, colors, and fine details.
---

# Print Artwork Preparation

## Goal

Prepare a usable artwork asset without silently redesigning the supplied graphic. The source artwork is authoritative.

## Preserve

- Exact wording, spelling, letterforms, layout, spacing, and orientation.
- Original colors, gradients, distressing, halftones, grain, cracks, and worn edges.
- Fine outlines, small details, intentional gaps, and irregularities.
- Original aspect ratio.

Never retype or recreate text when the source pixels can be retained. Do not substitute a similar font or redraw the artwork unless explicitly requested.

## Extraction workflow

1. Inspect the source dimensions, resolution, color mode, background, and artwork boundaries.
2. Determine whether the background is truly transparent, solid, textured, or part of the design.
3. Isolate the artwork with a suitable selection/mask. Refine edges without erasing intentional distressing or thin strokes.
4. Remove only the unwanted background. Do not mistake white highlights, holes, or distressed transparent gaps for background if they belong to the design.
5. Preserve alpha transparency. Do not use a checkerboard pattern, white fill, or gray fill as a fake transparent background.
6. Crop tightly around the artwork with the requested margin. If no margin is specified, use a modest 10–20 px margin when canvas resolution supports it.
7. Keep original pixel dimensions when sufficient. Do not upscale and invent detail. If resolution is inadequate, report that limitation.
8. Inspect the exported PNG over both a dark and a light background to detect halos and lost details.

## Delivery

Default editable/production-friendly output when appropriate:
- Transparent PNG.
- Original artwork colors and texture.
- Tight crop with 10–20 px margin unless specified otherwise.
- No checkerboard or solid background baked into the pixels.

For print production, distinguish a visual reference PNG from a true production-ready vector/separation file. Do not claim a PNG is vector artwork or that it contains spot-color separations.

## Quality checklist

- [ ] Text and artwork not redrawn or altered.
- [ ] Distressed texture and original colors preserved.
- [ ] Alpha channel is real transparency.
- [ ] No white/gray fringe or checkerboard pixels.
- [ ] No important details clipped.
- [ ] Crop and margin match the request.
- [ ] Resolution limitations disclosed.
