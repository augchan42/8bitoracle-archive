# 8bitoracle-archive

Archive of large static assets from [8bitoracle-next](https://github.com/auchan/8bitoracle-next) that are not needed in production builds.

## Purpose

These files were moved out of the main project's `public/` directory to reduce Vercel build and deploy times. The main project's `public/` folder was ~585MB, with most of that being archived/raw images never served in production.

## Contents

- `public/images/archive/` — Archived hexagram images from previous generation runs (~318MB)
- `public/images/raw/` — Raw source images before processing (~87MB)
- `public/images/processed-archive/` — Archived processed images (~30MB)

## Usage

These assets are for reference and local development only. If you need to reprocess or regenerate hexagram images, copy the relevant files back to the main project.
