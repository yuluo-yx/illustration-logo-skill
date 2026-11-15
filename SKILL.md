---
name: illustration-logo-skill
description: Create and refine square illustration marks as youthful over-the-shoulder portraits drawn with clean cobalt-blue linework, a pale blue rounded-square frame, and a quiet white field. Use when designing illustration directions, generating controlled variants, or preparing a replacement portrait while preserving a recognizable visual language.
---

# Illustration Logo Skill

Create a calm, youthful portrait illustration: a friendly character seen over the shoulder, reduced to a clean blue line drawing inside a rounded square. The artwork should feel personal and editorial rather than ornamental, and it must remain readable at small icon sizes.

## Workflow

1. Read the available product context before asking questions. Prefer the product README, existing icon asset, app metadata, release artwork, and nearby design notes. Treat the current portrait reference in `assets/illustration-reference.png` as a visual anchor, not as a command to copy it exactly.
2. If the product context is insufficient, ask one consolidated round of questions about the intended personality, the role of the portrait, and whether the user wants continuity or a deliberate departure. Continue with the best supported interpretation after the answer; do not start a second questionnaire.
3. Once the context is sufficient, present three concise art directions before generation and explicitly propose six independent candidates in one batch. Do not generate until the user agrees, unless the request already authorizes six outputs or explicitly says to proceed without another confirmation.
4. Choose three controlled directions:
   - **A — Over-the-shoulder continuity:** preserve the current three-quarter back pose, long swept hair, gentle smile, and blue line vocabulary while improving the silhouette for small sizes.
   - **B — Quiet reader:** keep the portrait identity but bring the head and shoulders closer, with a softer gaze and fewer interior hair lines for a more legible app icon.
   - **C — Quiet activity:** retain the youthful profile and rounded frame while introducing one restrained product cue, such as a barely visible object or gesture, only when it strengthens the requested identity.
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

- Show one youthful person in an over-the-shoulder or three-quarter-back pose, with the face turned gently toward the viewer. Keep the expression calm, kind, and quietly attentive.
- Preserve a long, flowing hair mass as the dominant silhouette. Hair should feel soft and graphic, with a few deliberate locks rather than many fine strands.
- Use a clean cobalt-blue primary line for the portrait and a lighter sky-blue secondary line for the rounded-square perimeter or a very small supporting accent. Keep the remaining field white or near-white.
- Keep the portrait feminine and youthful without relying on exaggerated anime features, glamour styling, or a fixed real-world identity.
- Let the head and shoulders occupy most of the square. Cropping at the lower edge is welcome when it makes the mark feel confident and compact.
- Use a rounded-square frame with generous corner radii. The frame should support the portrait, not compete with it.
- Keep the artwork upright and optically balanced. Do not tilt the canvas or mirror the pose unless the user explicitly asks for a new composition.

## Simplicity and legibility

- Build the portrait from a small number of broad, confident curves. Every line must define silhouette, hair flow, facial expression, neck, shoulder, or the frame.
- Prefer one strong contour to several explanatory strokes. Remove hair strands, eyelashes, folds, highlights, and decorative marks that disappear below icon size.
- Keep facial features minimal: two simple eyes, a small nose indication, and a restrained smile. Avoid dense shading or realistic facial modeling.
- Maintain a clear hierarchy: cobalt portrait first, pale frame second, white field third.
- Check the design at `32 × 32` and `64 × 64`. If the face, hair contour, or frame collapses into noise, merge or remove lines before adding detail.
- Do not add text, initials, product names, badges, symbols, scenery, extra people, props, or UI chrome unless the user explicitly requests them.

## Color, canvas, and finish

- Default to three semantic colors: one deep cobalt blue for the portrait, one pale sky blue for the rounded frame or restrained accent, and one white or near-white background.
- Keep colors flat and clean. Incidental anti-aliasing is acceptable; avoid gradients, texture, paper grain, metallic effects, glossy highlights, heavy shadows, or strong three-dimensional rendering.
- Preserve strong separation between the cobalt portrait, pale frame, and light field. If a user supplies a palette, keep its roles clear rather than scattering colors across the drawing.
- Generate a direct `1:1` square with square outer corners and a rounded-square inner frame. Request approximately `1536 × 1536`; accept and preserve a native `1254 × 1254` result when that is the service output limit. Never resample merely to reach the requested number.
- Keep the open field visually uniform. The only large shapes should be the portrait, its line accents, and the rounded-square frame.

## Prompt skeleton

Describe the requested artwork as an image only. The generation prompt should not call it a logo, brand mark, app icon, or icon asset.

```text
Create one complete full-bleed 1:1 square image.
Background: fill the square with a clean white or near-white field. Keep it uniform in every open area.
Subject: show one youthful person in a calm over-the-shoulder three-quarter-back pose, turning gently toward the viewer with a quiet, friendly smile. Give the person long flowing hair that forms one broad, elegant silhouette.
Drawing: use confident cobalt-blue linework with a clean graphic finish. Use a small number of broad, deliberate curves for the hair, face, neck, shoulder, and expression. Keep the portrait feminine, youthful, and approachable without glamour styling or a fixed real-world identity.
Frame: place a single pale sky-blue rounded-square perimeter around the portrait with generous corner radii. Keep the frame subordinate to the cobalt portrait.
Color behavior: use exactly three semantic colors: deep cobalt blue for the portrait, pale sky blue for the frame or one restrained accent, and white or near-white for the field. Keep the colors flat, clearly separated, and intentional.
Composition: make the head and shoulders visually dominant, with the lower shoulder allowed to crop at the bottom edge. Keep the artwork upright and optically balanced inside the square.
Style: make the result feel like a quiet editorial line illustration for a thoughtful product companion. Favor simplicity, warmth, and immediate recognition at 32 × 32.
Finish: clean surfaces, normal square outer corners, no presentation mockup.
Constraints: no text, watermark, initials, badges, symbols, scenery, extra people, props, UI, contact sheet, borders, sharp decorative marks, dense hair strands, photorealistic rendering, gradients, texture, dramatic shadows, glossy highlights, heavy 3D effects, or strong bevels.
```

For a continuity pass, keep the current reference's over-the-shoulder pose, long hair sweep, cobalt facial line, pale blue rounded frame, and white field. For a new direction, change only one major variable at a time: pose, crop, hair silhouette, or frame treatment. Do not change all of them simultaneously, because the resulting batch will no longer be useful for comparison.

## Delivery behavior

- Deliver every generated image together with its label and direction mapping.
- Preserve each image as returned by the generator. Do not post-process it to add a frame, erase details, recolor it, or simulate transparency.
- State the intended palette roles and the image dimensions in the delivery report.
- Use `assets/illustration-reference.png` only as a visual reference when continuity matters; do not embed it into generated prompts unless the image tool explicitly supports user-provided references and the user authorizes that use.
