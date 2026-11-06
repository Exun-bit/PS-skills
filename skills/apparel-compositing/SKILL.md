---
name: apparel-compositing
description: Composite a supplied apparel product image into a reference advertisement, e-commerce layout, scene, or mockup while preserving the garment itself. Use when the user provides a reference image and a separate product image to embed.
---

# Apparel Compositing

## Source roles

- **Reference image:** controls layout, composition, typography hierarchy, background treatment, lighting direction, and placement.
- **Product image:** controls the garment's actual appearance. Never copy garment details from the reference over the supplied product.

If the user says "embed my product into this reference", preserve the reference's layout while replacing only the product area with the supplied garment.

## Preserve the garment

Do not alter garment design, color, fabric, silhouette, construction, texture, logos authorized by the user, or print details unless separately requested. Do not generate missing garment portions in a way that changes product specifications.

## Composition workflow

1. Identify the reference canvas size, aspect ratio, margins, product area, text areas, background, and key alignment lines.
2. Inspect product image orientation, perspective, garment boundaries, and lighting.
3. Remove the product background only as needed. Preserve fine garment edges, drawstrings, fringes, and shadows.
4. Scale proportionally. Never stretch width and height independently.
5. Position and warp only to match the reference plane. Do not distort the garment's design.
6. Match the reference lighting and shadow direction without changing the garment's base color or fabric appearance.
7. Keep text, logos, and graphic overlays separate and editable where possible.
8. Verify margins, overlap, clipping, edge quality, and visual hierarchy against the reference.

## Layout lock

When a user has approved a recurring layout, treat it as a locked template:
- Keep canvas ratio, major zones, divider angle, text hierarchy, and product placement consistent.
- Change only the product image and product-specific copy that the user authorizes.
- Do not improvise a new layout on each iteration.

## Delivery

Export at the reference aspect ratio and requested resolution. Keep a layered PSD when future product swaps are expected. Also provide a flattened preview if requested.


## Fixed-master product replacement (critical default)

When the user supplies an approved advertising template and a separate garment photo, interpret “replace the product” as **object-level garment replacement**, never as replacing or filling the entire right-hand panel.

### Lock the master template
1. Use the approved reference artwork as the immutable master.
2. Preserve its canvas dimensions, crop, left information panel, typography, icons, badges, buttons, background, diagonal divider, and all layout pixels outside the original garment footprint.
3. Do not redraw, approximate, recalculate, shift, straighten, or regenerate the diagonal divider.
4. Do not scale the full product photograph to fill the right panel.

### Transfer the garment, not its source photograph
1. Locate the original garment in the master and determine its visible silhouette/bounding box, center, scale, orientation, visual mass, and margins relative to the right panel.
2. Segment the garment from the supplied product photo. Remove the supplied photo's background when necessary; retain fine edges, hood/drawstrings, cuffs, hems, loose fibers, and natural garment shadows where useful.
3. Remove only the original garment from the master. Reconstruct the small exposed background area from adjacent background texture/light; do not touch the left panel or divider.
4. Fit the new garment to the **original garment's visual footprint**, not to the whole right-side panel. Match the reference garment's center, approximate bounding-box width/height, scale, top/bottom position, and surrounding negative space.
5. Preserve the new garment's own aspect ratio and construction. Use proportional scaling; if its silhouette differs, adjust placement and scale rather than stretching it. Do not force the new garment into the old garment's exact outline.
6. Match scene perspective and lighting only as needed for a believable composite. Keep the new garment's actual color, fabric, wash, logo, print/embroidery, and construction faithful to its source.
7. Keep the original template's diagonal boundary and background intact. The replacement garment must sit naturally within the right product scene without crossing into the left information panel unless the approved template already does so.

### Hard prohibitions
- Never paste the entire source product photo over the right panel.
- Never crop the product photo to the panel aspect ratio as a shortcut.
- Never invent a new divider or rebuild the ad layout.
- Never enlarge the garment merely to fill empty space; match the reference garment's visual scale and margins.
- Never alter the left-side text, graphics, or information to make room for the product.
- Never claim a pixel-identical result if the original garment removal required background reconstruction.

### Verification checklist
Compare output side-by-side with the master:
- Left information panel and divider are unchanged.
- Canvas size and aspect ratio are unchanged.
- Only the original garment/object area has been replaced (plus the minimum background reconstruction needed to remove it).
- New garment's visual center, scale, and negative-space margins follow the reference garment.
- New garment is not stretched, clipped, or unnaturally cut out.
- Garment identity and details match the supplied product photo.

If a clean garment mask or background reconstruction is not reliable, do not fake a panel swap. Report the limitation and request a cleaner product photo or use a dedicated image-editing/generative-fill step with the master locked.
