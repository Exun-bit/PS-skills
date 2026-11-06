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
