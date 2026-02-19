# Processed Images Directory

This directory contains 8-bit Oracle styled images generated from raw reference images.

## Purpose

Images here are the output of OpenRouter Gemini Flash image-to-image transformation, applying the tech-noir aesthetic:
- Phosphor green (#2EBD2E) monochrome with amber/orange highlights
- CRT monitor scan lines and phosphor glow effects
- 1970s computer terminal aesthetic
- High contrast, dramatic lighting
- Retro-futuristic digital atmosphere

## Directory Structure

This directory mirrors the structure of `public/images/raw/`:

```
processed/
├── heavy-metal/
│   └── sorayama-july-1981-cover.png
├── lord-bbs/
│   └── lord-dragon-banner.png
├── star-trek/
│   └── transporter-three-figure-dissolution.png
└── ...
```

Each processed image corresponds to a raw reference image with the same directory structure and filename (but with `.png` extension for consistency).

## Workflow

1. **Source:** Raw reference images in `public/images/raw/{category}/{filename}`
2. **Processing:** Run image generation script with hexagram's `imagePrompt` from JSON
3. **Output:** Saved here as `public/images/processed/{category}/{filename}.png`
4. **Reference:** Hexagram JSON files point to processed images, not raw ones
5. **Reusability:** Same processed image can be referenced by multiple hexagrams if needed

## Current Status

This directory will be populated as images are generated. Track progress in `docs/hexagram-image-status.md`.

**Active hexagrams awaiting generation:** 6
**Draft hexagrams awaiting generation:** 5
**Total needed:** 11 processed images (0 currently exist)

See `docs/hexagram-image-status.md` for detailed status and generation queue.
