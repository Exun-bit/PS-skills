# PS Skills — Apparel & Garment Image Production

A practical Photoshop skill library for apparel export, custom-clothing product images, print artwork preparation, brand-safe image editing, and repeatable e-commerce assets.

## Design goal

Protect the original garment. Change only the elements the user explicitly asks to change. Preserve construction, fabric, color, wash, print texture, lighting, shadows, perspective, and proportions unless the task says otherwise.

## Skills

| Skill | Use it for |
|---|---|
| [apparel-image-master](skills/apparel-image-master/SKILL.md) | Main router for apparel Photoshop tasks |
| [garment-brand-replacement](skills/garment-brand-replacement/SKILL.md) | Remove customer branding and apply the currently authorized brand |
| [garment-product-retouch](skills/garment-product-retouch/SKILL.md) | Clean product photos without redesigning the garment |
| [print-artwork-prep](skills/print-artwork-prep/SKILL.md) | Extract and prepare print graphics as transparent production assets |
| [apparel-compositing](skills/apparel-compositing/SKILL.md) | Place product images into reference layouts and mockups |
| [apparel-batch-consistency](skills/apparel-batch-consistency/SKILL.md) | Apply consistent visual treatment and export rules across a set |

## Installation

Copy the required skill folder into the skills directory used by your agent. For a skills.sh-compatible workflow, install the repository and select the skill folder. The master skill can be used as the entry point.

## Operating rules

1. Inspect the source image and identify the requested edit before changing pixels.
2. Preserve an untouched original and use non-destructive layers/masks where possible.
3. Do not invent missing logos, artwork, garment details, or production specifications.
4. Do not claim an edit is complete until the output has been visually checked.
5. Keep the requested output format, dimensions, transparency, and crop margins.
6. Treat customer assets and brand details as confidential; do not reuse them in unrelated work.

## Brand profile

The current default profile is stored separately in [profiles/current-brand.md](profiles/current-brand.md). It is configuration, not a permanent assumption. When the user supplies a new company website, logo, or brand details, update the profile and use the newest confirmed information.

## References that informed the workflow

The structure borrows general workflow patterns from public Photoshop agent skills and Adobe's batch-editing skill: task routing, state/backup/operate/verify, non-destructive editing, batch consistency, and explicit export checks. This repository is an independent apparel-focused implementation, not a copy of those projects.
