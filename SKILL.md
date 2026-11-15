---
name: illustration-logo-skill
description: Create and refine square illustration marks as youthful face outlines, head-and-shoulder portraits, or half-body figures with clean graphic linework, expressive flat palettes, and a small thematic cue. Use when designing illustration directions, generating controlled variants, or preparing a replacement portrait while preserving a recognizable visual language without locking every result to one pose or blue palette.
---

# Illustration Logo Skill

Create a calm, youthful portrait illustration: a friendly character represented as a face outline, head-and-shoulder portrait, or compact half-body figure inside a rounded square. Keep the artwork personal and editorial, then vary the palette, composition, and one restrained thematic cue so a batch feels rich without becoming noisy. Every candidate must remain readable at small icon sizes.

## Workflow

1. Read the available product context before asking questions. Prefer the product README, existing icon asset, app metadata, release artwork, and nearby design notes. Treat the current portrait reference in `assets/illustration-reference.png` as a visual anchor, not as a command to copy it exactly.
2. If the product context is insufficient, ask one consolidated round of questions about the intended personality, the role of the portrait, and whether the user wants continuity or a deliberate departure. Continue with the best supported interpretation after the answer; do not start a second questionnaire.
3. Once the context is sufficient, present three concise art directions before generation and explicitly propose six independent candidates in one batch. Do not generate until the user agrees, unless the request already authorizes six outputs or explicitly says to proceed without another confirmation.
4. Choose three controlled directions with distinct palette and theme roles:
   - **A — Face outline:** reduce the subject to a confident profile or three-quarter facial contour with one or two interior features, using warm paper, rose dusk, or citrus studio colors for a graphic editorial mood.
   - **B — Head-and-shoulders portrait:** keep the face, hair, neck, and upper shoulders in frame, using forest, teal, sage, marigold, or another botanical family; add one tiny leaf, sprig, or organic shape only when it helps the theme.
   - **C — Compact half-body story:** show the upper torso and one simple gesture or object for reading, making, music, study, travel, or reflection; select a palette that supports the cue, such as plum and apricot, indigo and lavender, or charcoal and rose.
   - Do not force every candidate into the same crop. Across the six-image proposal, include at least two composition types when the product context allows it.
   - Across the six-image proposal, distribute at least three clearly different palette families and at least two different thematic moods. Do not make every candidate blue.
5. Interpret the response exactly:
   - If all three directions and the six-image proposal are accepted, generate two independent variants per direction and label them `A1`, `A2`, `B1`, `B2`, `C1`, and `C2`.
   - If one direction is selected and six images are accepted, generate six controlled variants of that direction and label them `A1` through `A6`.
   - If the user changes the quantity, direction, or distribution, follow the replacement instructions exactly.
   - Keep every candidate as a separate square asset. Never ask the image model for a contact sheet or comparison grid.
6. Before generation, verify that a capable image model is available. Prefer the best available instruction-following image model. Do not fabricate results, silently substitute a low-quality fallback, or convert the artwork to SVG unless the user explicitly requests a vector deliverable.
7. Treat each batch as one creative draw. Generate each requested candidate once, preserve the returned result, and deliver every result. Do not rank candidates, reject them for minor rendering variation, or automatically retry them. Generate refinements only after the user explicitly asks for another draw.
8. Report every label, direction, rationale, pose, palette role, model/provider, saved path, and dimensions. Mention when the current reference was used as a visual anchor.

When proposing directions, use one compact line per direction: `<direction name> — <product connection> — <pose or line treatment>`. End with a direct proposal to generate six independent square images.

## Identity and art direction

- Show one youthful person as a face outline, head-and-shoulders portrait, half-body figure, or over-the-shoulder pose. Keep the expression calm, kind, and quietly attentive whenever facial features are visible.
- When hair is present, keep it as a soft graphic mass with a few deliberate locks rather than many fine strands. Short hair, tied hair, or a clean bald contour are also valid when they support the selected composition.
- Use one coherent flat palette per candidate. The portrait may use deep teal, cobalt, plum, forest, charcoal, terracotta, or another dark anchor; pair it with one lighter frame color and one restrained accent. Keep the remaining field light and quiet.
- Keep the portrait feminine and youthful without relying on exaggerated anime features, glamour styling, or a fixed real-world identity.
- Choose the crop deliberately: a face outline may use most of the square, a head-and-shoulders portrait may crop below the collarbone, and a half-body figure may show the torso and one simple gesture. Cropping at the lower edge is welcome when it makes the mark feel confident and compact.
- Use a rounded-square frame with generous corner radii. The frame should support the portrait, not compete with it.
- Keep the artwork upright and optically balanced. Do not tilt the canvas or mirror the pose unless the user explicitly asks for a new composition.

## Simplicity and legibility

- Build the figure from a small number of broad, confident curves. Every line must define the facial contour, silhouette, hair flow, expression, clothing, gesture, thematic cue, or frame.
- Prefer one strong contour to several explanatory strokes. Remove hair strands, eyelashes, folds, highlights, and decorative marks that disappear below icon size.
- Keep facial features minimal: two simple eyes, a small nose indication, and a restrained smile. Avoid dense shading or realistic facial modeling.
- Maintain a clear hierarchy: dark figure or contour first, lighter frame and accent second, quiet field third.
- Check the design at `32 × 32` and `64 × 64`. If the face, hair contour, or frame collapses into noise, merge or remove lines before adding detail.
- Add at most one small thematic cue when the selected direction calls for it: a leaf, book edge, pencil, cup, note, star, window shape, or similar simple motif. Do not add text, initials, product names, badges, extra people, detailed scenery, or UI chrome.

## Color, canvas, and finish

- Use three to five semantic colors: a dark portrait anchor, a lighter frame or secondary line, one optional accent, and a light background. Keep each candidate internally consistent instead of scattering unrelated colors across the drawing.
- Rotate among curated palette families across a batch. Good starting points are **warm paper** (plum, terracotta, coral, cream), **botanical** (forest, teal, sage, marigold, ivory), **sunset** (indigo, coral, apricot, blush), **citrus studio** (charcoal, lemon, tangerine, warm white), and **rose dusk** (wine, mauve, dusty pink, lavender). Blue may appear, but it must not be the default for every candidate.
- Let the palette support the theme: botanical cues should feel organic, reading and study can use paper and amber, music can use plum and coral, and night or reflection can use indigo and lavender. Keep the mood varied while preserving the same simple portrait language.
- Keep colors flat and clean. Incidental anti-aliasing is acceptable; avoid gradients, texture, paper grain, metallic effects, glossy highlights, heavy shadows, or strong three-dimensional rendering.
- Preserve strong separation between the portrait, frame, accent, and light field. If a user supplies a palette, keep its roles clear rather than scattering colors across the drawing.
- Generate a direct `1:1` square with square outer corners and a rounded-square inner frame. Request approximately `1536 × 1536`; accept and preserve a native `1254 × 1254` result when that is the service output limit. Never resample merely to reach the requested number.
- Keep the open field visually uniform. The only large shapes should be the portrait, its line accents, and the rounded-square frame.

## Prompt skeleton

Describe the requested artwork as an image only. The generation prompt should not call it a logo, brand mark, app icon, or icon asset.

```text
Create one complete full-bleed 1:1 square image.
Background: fill the square with a light, quiet field selected from the palette. Keep it uniform in every open area.
Subject: show one youthful person using the selected composition: a face outline, head-and-shoulders portrait, compact half-body figure, or over-the-shoulder pose. Keep the expression calm, kind, and quietly attentive when facial features are shown. Give the person a clear hair or head silhouette without requiring long hair.
Drawing: use confident graphic linework in the palette's dark portrait anchor. Use a small number of broad, deliberate curves for the facial contour, hair, neck, clothing, gesture, and expression. Keep the figure youthful and approachable without glamour styling or a fixed real-world identity.
Theme cue: add at most one small, simple motif that communicates the selected mood, such as a leaf for botanical, a book edge for reading, a pencil for making, a music note for music, a window shape for reflection, or a tiny star for night. Omit the cue when it would reduce legibility.
Frame: place a single rounded-square perimeter around the portrait using the palette's lighter frame color with generous corner radii. Keep the frame subordinate to the portrait.
Color behavior: use one named palette family for this candidate, with three to five flat semantic colors: dark portrait anchor, lighter frame or secondary line, optional accent, and light field. Keep the colors clearly separated and intentional. Do not default to blue when another palette better expresses the theme.
Composition: make the selected crop immediately legible at 32 × 32. A face outline may fill the square; a head-and-shoulders portrait may crop below the collarbone; a half-body figure may include one simple gesture or object. Keep the artwork upright and optically balanced inside the square.
Style: make the result feel like a quiet editorial line illustration for a thoughtful product companion. Favor simplicity, warmth, and immediate recognition at 32 × 32.
Finish: clean surfaces, normal square outer corners, no presentation mockup.
Constraints: no text, watermark, initials, badges, unrelated symbols, detailed scenery, extra people, repeated props, UI, contact sheet, borders, sharp decorative marks, dense hair strands, photorealistic rendering, gradients, texture, dramatic shadows, glossy highlights, heavy 3D effects, or strong bevels. Include only the one previously selected thematic cue when it improves the composition.
```

For a continuity pass, keep the current reference's clean rounded frame, white-space discipline, and restrained line vocabulary while allowing the composition to become a face outline, head-and-shoulders portrait, or half-body figure. For a new direction, change only one major structural variable at a time: pose, crop, hair silhouette, frame treatment, or theme cue. Palette and mood may change between candidates, but each individual candidate must use one coherent palette. Do not change every structural variable simultaneously, because the resulting batch will no longer be useful for comparison.

## Delivery behavior

- Deliver every generated image together with its label and direction mapping.
- Preserve each image as returned by the generator. Do not post-process it to add a frame, erase details, recolor it, or simulate transparency.
- State the intended palette roles and the image dimensions in the delivery report.
- Use `assets/illustration-reference.png` only as a visual reference when continuity matters; do not embed it into generated prompts unless the image tool explicitly supports user-provided references and the user authorizes that use.
