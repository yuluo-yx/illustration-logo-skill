# Illustration Logo Skill

[![LINUX DO Community](https://img.shields.io/badge/LINUX%20DO-Community-FFB003?style=flat)](https://linux.do/)

`illustration-logo-skill` is an Agent Skill for creating and refining square illustration marks. It supports calm youthful face outlines, head-and-shoulders portraits, and compact half-body figures with clean graphic linework, varied flat palettes, and one restrained thematic cue inside a rounded-square frame.

The skill is designed for compatible AI agents that can generate raster images. It keeps the artwork simple enough to remain legible at small icon sizes while leaving room for controlled creative variation.

## Logo wall

One illustration language, six personalities: bright citrus and coral alongside botanical greens, warm terracotta, and muted plum. Each image links to its full-resolution artwork.

<table>
  <tr>
    <td align="center" width="33%">
      <a href="assets/illustration-reference.png"><img src="assets/illustration-reference.png" alt="Original blue line portrait with a light blue rounded frame" width="240"></a><br>
      <strong>Original Blue</strong><br>Clean lines · Cool blue
    </td>
    <td align="center" width="33%">
      <a href="assets/citrus-studio.png"><img src="assets/citrus-studio.png" alt="Short-haired portrait in charcoal, tangerine, and lemon" width="240"></a><br>
      <strong>Citrus Studio</strong><br>Tangerine · Lemon · Warm white
    </td>
    <td align="center" width="33%">
      <a href="assets/coral-pop.png"><img src="assets/coral-pop.png" alt="Ponytail portrait in deep wine and vivid coral" width="240"></a><br>
      <strong>Coral Pop</strong><br>Wine · Coral · Blush
    </td>
  </tr>
  <tr>
    <td align="center" width="33%">
      <a href="assets/olive-retro.png"><img src="assets/olive-retro.png" alt="Botanical bob-haired portrait in forest green, olive, and mustard" width="240"></a><br>
      <strong>Olive Retro</strong><br>Forest · Olive · Mustard
    </td>
    <td align="center" width="33%">
      <a href="assets/terracotta-reader.png"><img src="assets/terracotta-reader.png" alt="Long-haired reader holding a book in warm terracotta and umber" width="240"></a><br>
      <strong>Terracotta Reader</strong><br>Umber · Terracotta · Cream
    </td>
    <td align="center" width="33%">
      <a href="assets/plum-melody.png"><img src="assets/plum-melody.png" alt="Short-haired listener wearing headphones in plum and dusty mauve" width="240"></a><br>
      <strong>Plum Melody</strong><br>Plum · Mauve · Apricot
    </td>
  </tr>
</table>

## What it guides

- Three deliberate illustration directions before generation
- Six independent candidates by default, labeled `A1` through `C2`
- Face outlines, head-and-shoulders portraits, and compact half-body figures rather than one fixed pose
- Warm, botanical, sunset, citrus, and rose-dusk palette families instead of an all-blue batch
- One optional thematic cue for reading, making, music, study, nature, travel, or reflection
- A light rounded-square frame and white, cream, blush, ivory, or other quiet field chosen to support the palette
- Broad, confident curves that survive reduction to `32 × 32`
- Quiet editorial warmth instead of photorealistic, glossy, or ornamental rendering
- Separate full-resolution square assets rather than contact sheets
- One-pass delivery of every generated result without automatic ranking or retries
- Clear reporting of direction, palette roles, dimensions, and saved paths

## Use

Ask a compatible AI agent for an illustration direction, for example:

```text
Create six illustration candidates that preserve the current clean line language and 32 × 32 legibility, while mixing face outlines, head-and-shoulders portraits, and compact half-body figures across warm paper, botanical, sunset, citrus studio, and rose-dusk palettes with small thematic cues. Do not make every candidate blue or use the same crop.
```

When the request does not provide enough product context, the skill reads the available workspace context first and asks one consolidated round of questions only when needed. It then proposes three concise directions and waits for approval unless the request already authorizes the batch.

The bundled reference image is a visual anchor for continuity. It is not a requirement to reproduce the exact existing pixels, and it should not be copied into a generated result unless the user explicitly requests a faithful redraw.

## Repository structure

```text
SKILL.md
README.md
LICENSE
assets/illustration-reference.png
assets/citrus-studio.png
assets/coral-pop.png
assets/olive-retro.png
assets/terracotta-reader.png
assets/plum-melody.png
```

The skill has no runtime dependencies, scripts, or external style packages.

## License

MIT
