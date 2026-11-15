# Illustration Logo Skill

`illustration-logo-skill` is an Agent Skill for creating and refining square illustration marks. It supports a calm youthful over-the-shoulder portrait, clean cobalt-blue linework, a pale blue rounded-square frame, and a quiet white field.

The skill is designed for compatible AI agents that can generate raster images. It keeps the artwork simple enough to remain legible at small icon sizes while leaving room for controlled creative variation.

![Illustration reference](assets/illustration-reference.png)

## What it guides

- Three deliberate illustration directions before generation
- Six independent candidates by default, labeled `A1` through `C2`
- A youthful over-the-shoulder portrait with long flowing hair
- Cobalt portrait lines, a pale sky-blue rounded-square frame, and a white or near-white field
- Broad, confident curves that survive reduction to `32 × 32`
- Quiet editorial warmth instead of photorealistic, glossy, or ornamental rendering
- Separate full-resolution square assets rather than contact sheets
- One-pass delivery of every generated result without automatic ranking or retries
- Clear reporting of direction, palette roles, dimensions, and saved paths

## Use

Ask a compatible AI agent for an illustration direction, for example:

```text
Create six illustration candidates that preserve the current over-the-shoulder portrait, cobalt linework, pale blue rounded-square frame, and white field, while simplifying the hair and face for 32 × 32 legibility.
```

When the request does not provide enough product context, the skill reads the available workspace context first and asks one consolidated round of questions only when needed. It then proposes three concise directions and waits for approval unless the request already authorizes the batch.

The bundled reference image is a visual anchor for continuity. It is not a requirement to reproduce the exact existing pixels, and it should not be copied into a generated result unless the user explicitly requests a faithful redraw.

## Repository structure

```text
SKILL.md
README.md
LICENSE
assets/illustration-reference.png
```

The skill has no runtime dependencies, scripts, or external style packages.

## License

MIT
