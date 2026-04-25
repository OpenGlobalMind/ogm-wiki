**On image optimization:**

Squoosh (squoosh.app) is the best no-code tool for this — it's a browser app made by Google, free, and lets you see the quality difference side by side before saving. For your images:

- **Format:** Convert everything from PNG to WebP. WebP gives you roughly 70-80% smaller files at equivalent visual quality. Your 7-10MB PNGs will typically drop to 500KB-1.5MB.
- **Target size:** Aim for **under 500KB per hero image, under 200KB for thumbnails and avatars**. For a full-bleed hero on a 1440px wide screen, 1600px wide at WebP quality 80 is plenty — you won't see a difference.
- **Workflow in Squoosh:** drag image in → choose WebP on the right → set quality to 80 → compare the two sides → download. Repeat for each image.
- **Rename:** keep the same filename but change `.png` to `.webp`, then update the HTML references. I can do that in one pass on the `index.html` once you've converted them all.

Realistically you can get your 150MB image folder down to under 15MB total, which will make the site feel instant.