# Image replacement guide

Research images are now extension-flexible. You do not need to convert PNG to JPG.

## Research image slots

Put one image file into:

```text
assets/images/research/
```

Use these base names:

```text
01-nir-oled
02-multifunctional-diodes
03-blue-uc-oled
04-evaporable-fullerenes
05-cofs
```

Supported formats:

```text
.png
.jpg
.jpeg
.webp
.avif
.gif
.svg
```

Examples that all work:

```text
assets/images/research/01-nir-oled.png
assets/images/research/01-nir-oled.jpg
assets/images/research/01-nir-oled.webp
```

Important: keep only one file with the same base name. For example, do not keep both:

```text
01-nir-oled.jpg
01-nir-oled.png
```

If both exist, the website may choose the first matching file and not the one you expect.

## Recommended dimensions

For research cards, horizontal images work best:

```text
1600 x 1000 px
1200 x 800 px
```

The site now uses `object-fit: contain`, so the full image is shown instead of being cropped.
