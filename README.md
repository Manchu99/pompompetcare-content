# PomPom Petcare — Content Repository

Public content assets (listing images, A+ content, Brand Story, Brand Store) for PomPom Petcare's Amazon listings. Hosted publicly so Amazon's image crawler can fetch images via raw URLs.

## Structure

```
listing-images/
  care/
    HP-SH1-250/    (2-in-1 Shampoo & Conditioner)
    HP-CO1-250/    (Conditioner)
    HP-SHX-250/    (Lux Shampoo)
    HP-SHP-250/    (Puppy Shampoo)
  sprays/
    HP-DET-250/    (Detangling Spray)
    HP-SS1-250/    (Show Shine Spray)
  flea/
    HP-SHL-250/    (Deep-Cleansing Shampoo — "Loppe" in EU)
a-plus-content/    (placeholder)
brand-story/       (placeholder)
brand-store/       (placeholder)
```

## Image naming convention

`<SKU>-<NN>.png` where NN is a two-digit position:
- `01` — Main image (white background, required for Amazon main slot)
- `02–07` — Gallery images (lifestyle, infographics, usage, trust)

Raw URL pattern:
```
https://raw.githubusercontent.com/<user>/<repo>/main/listing-images/<group>/<SKU>/<SKU>-<NN>.png
```

## Notes
- All images 2000×2000 PNG.
- Replacing an image: overwrite the file with the same name + commit. Amazon refetches on next PATCH.
- Content is marketing assets — not sensitive.
