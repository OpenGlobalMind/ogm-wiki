# STUMP JERRY'S BRAINS — Framer Build Guide
## Everything you need to go from blank canvas to live site

---

## STARTING POINT: Which Template?

**Use a blank canvas. Not a template.**

Here's why: every Framer template comes with its own component library,
spacing conventions, and color system that you'll spend more time fighting
than using. This site has a very specific visual identity — Bebas Neue
display type, the warm paper/ink palette, the editorial layout. Starting
blank takes 20 minutes of setup and saves hours of fighting someone else's
opinions.

The one exception: if you want Framer's CMS for future blog posts or
case studies, start with their blank "CMS Starter" — it adds CMS
scaffolding without imposing a design.

---

## PHASE 1: PROJECT SETUP (20 min)

### 1.1 Create the project
- Framer dashboard → New Project → Blank Canvas
- Name: StumpJerrysBrains
- Connect your domain immediately: Site Settings → Domains →
  Add stumpjerrysbrain.com (and www redirect)

### 1.2 Add fonts
Site Settings → Fonts → Add Google Font. Add these four:
- **Bebas Neue** (no weight options — it only comes in one)
- **Syne** — select weights: 400, 700, 800
- **IBM Plex Mono** — select weights: 400, 500
- **Playfair Display** — select: italic 400, italic 700

### 1.3 Add color variables
Site Settings → Variables → Colors. Create these tokens
(name them exactly — you'll reference them throughout):

| Token name | Hex value | Role                            |
| ---------- | --------- | ------------------------------- |
| ink        | #0A0A0A   | Primary background, text        |
| paper      | #FAF7F2   | Page background                 |
| cream      | #F5F0E8   | Text on dark                    |
| canary     | #F7C948   | Accent, CTAs, ticker            |
| ember      | #E8531A   | CTA hover, logo 's', booking bg |
| navy       | #1A3A5C   | Story section, How It Works bg  |
| teal       | #2A9D8F   | TheBrain color, labels          |
| mid        | #8A7F70   | Secondary text, metadata        |

### 1.4 Add global custom code
Site Settings → Custom Code → Head Tag. Paste this:

```html
<link rel="preconnect" href="https://fonts.googleapis.com">
<link href="https://fonts.googleapis.com/css2?family=Bebas+Neue&family=Syne:wght@400;700;800&family=IBM+Plex+Mono:wght@400;500&family=Playfair+Display:ital,wght@1,400;1,700&display=swap" rel="stylesheet">
<style>
body { cursor: none; }
.cursor { position:fixed; width:12px; height:12px; background:#e8531a; border-radius:50%; pointer-events:none; z-index:9999; transition:transform 0.1s; mix-blend-mode:multiply; top:0; left:0; }
.cursor-ring { position:fixed; width:36px; height:36px; border:1.5px solid #e8531a; border-radius:50%; pointer-events:none; z-index:9998; opacity:0.5; top:0; left:0; }
@keyframes ticker-scroll { from { transform:translateX(0); } to { transform:translateX(-50%); } }
</style>
```

Site Settings → Custom Code → End of Body. Paste this:

```html
<div class="cursor" id="sjb-cursor"></div>
<div class="cursor-ring" id="sjb-ring"></div>
<script>
(function(){
  var c=document.getElementById('sjb-cursor'),r=document.getElementById('sjb-ring');
  if(!c||!r)return;
  var mx=0,my=0,rx=0,ry=0;
  document.addEventListener('mousemove',function(e){mx=e.clientX;my=e.clientY;});
  (function tick(){
    c.style.transform='translate('+(mx-6)+'px,'+(my-6)+'px)';
    rx+=(mx-rx-18)*0.12;ry+=(my-ry-18)*0.12;
    r.style.transform='translate('+rx+'px,'+ry+'px)';
    requestAnimationFrame(tick);
  })();
})();
</script>
```

### 1.5 Set up canvas breakpoints
In Framer's toolbar, set breakpoints:
- Desktop: 1440px (design primary here)
- Tablet:  768px
- Mobile:  390px

---

## PHASE 2: IMPORT THE SVG ASSETS (5 min)

All SVGs are in the /svgs folder of this kit. Import them into Framer:

**Method A (drag & drop):** Open your Framer canvas. Drag SVG files
directly from Finder/Explorer onto the canvas. Framer imports them
as editable vector layers.

**Method B (insert menu):** Press I (insert) → Image → select SVG file.

**What to do with each SVG:**

| File | Where to use | Notes |
|------|-------------|-------|
| brain-web-hero.svg | Hero section background | Set opacity to 7-8%. Position: absolute, cover the hero frame. |
| node-diagram.svg | "The Story" section | Place in right column alongside body copy. |
| thebrain-mockup.svg | Brain Demo section | Place in right column. Add a dark frame around it to simulate the app window chrome. |
| wordmark.svg | Anywhere you need the logo at large sizes | The HTML/CSS file renders this in type; SVG version is for export/print. |

---

## PHASE 3: BUILD THE PAGE SECTIONS

Work top to bottom. Each section is a full-width Frame with
Auto Layout (vertical). Here's the build order and key settings:

### NAV
- Frame: 100% width, fixed position (pin to top), z-index 100
- Background: #0A0A0A at 92% opacity, backdrop blur 10px
- Layout: horizontal flex, space-between, align center
- Padding: 1.2rem 4rem
- Border bottom: 1px, #FFFFFF at 6% opacity
- Brand text: Bebas Neue, 1.4rem, cream. "Jerry's" = canary, final "s" = ember
- Nav links: IBM Plex Mono, 0.72rem, uppercase, letter-spacing 15%, mid color
- CTA: same as primary button (canary background)

### HERO
- Frame: 100vw, min-height 100vh, background: ink
- Layout: 2-column grid (1fr 1fr), padding 8rem 4rem 5rem, gap 4rem
- Import brain-web-hero.svg as absolute background layer, opacity 7%

Left column:
- "Do you miss thinking?" → Playfair Display italic, canary, ~2.8rem
- "STUMP / JERRY'S / BRAINS" → Bebas Neue, cream, clamp(4.5rem, 11vw, 10rem), line-height 0.88
  → The 's' at end: separate text element in ember, same font/size
- Tagline: IBM Plex Mono, mid, 1rem, line-height 1.7
- CTA row: primary button + ghost text link, flex row, gap 2rem
- Add Framer scroll animations to each element (staggered fadeUp)

Right column (Provenance Card):
- Frame with border: 1px solid rgba(255,255,255,0.1)
- Background: rgba(26,58,92,0.4), backdrop blur 4px
- Left accent: 4px wide Frame, full height, gradient canary→ember
- Label: IBM Plex Mono, teal, 0.65rem
- Quote: Playfair Display italic, cream, 1.3rem
- Stats row: 3-column, Bebas Neue numbers in canary, IBM Plex Mono labels in mid

### TICKER
- Frame: 100% width, overflow hidden
- Background: canary
- Border top + bottom: 2px solid ink
- Inner content: Use the Ticker Code Component from components/framer-code-snippets.js
  OR manually: create a horizontal flex row, duplicate items 2x,
  apply CSS animation: ticker-scroll 36s linear infinite

### THE STORY (Provenance Section)
- Frame: 100vw, background: ink, padding 7rem 4rem
- Layout: 2-column grid (1fr 1fr), gap 6rem

Left column:
- Section label: IBM Plex Mono, 0.68rem, ember, uppercase, letter-spacing 0.3em
- Large heading: Bebas Neue, cream, ~5rem, line-height 0.95
  The word "Ideas" should be canary color

Right column:
- Body paragraphs: Syne, 1.05rem, cream at 68% opacity, line-height 1.8
- Manifesto stack: 4 rows, each with a border-bottom 1px rgba(255,255,255,0.08)
  Row structure: number (IBM Plex Mono, ember, small) + title (Syne 700, cream, 1.25rem)
  Sub-text: Syne 400, mid, 0.85em, block

### HOW IT WORKS
- Frame: 100vw, background: navy, padding 6rem 4rem
- Section label: IBM Plex Mono, teal
- Heading: Bebas Neue, cream, ~5rem
- Steps: 4-column grid (last step spans full width)
  Each step: padding 2.5rem 2rem, border-right 1px rgba(255,255,255,0.08)
  Glyph: Bebas Neue, 3rem, ember
  Title: Syne 800, cream, 1.05rem
  Description: Syne 400, 0.88rem, cream at 50% opacity

### BRAIN DEMO
- Frame: 100vw, background: navy, padding 6rem 4rem
- Layout: 2-column (1fr 1.5fr), gap 5rem
- Left: copy (section label teal, heading Bebas cream, body Syne)
- Right: import thebrain-mockup.svg
  Wrap in a dark frame with:
  - Background: #0d1117
  - Border: 1px rgba(255,255,255,0.1)
  - Border radius: 4px
  Add a titlebar strip at top: background #1c2128, flex row,
  three dot circles (red/yellow/green), monospace filename text

### OFFERS
- Frame: 100vw, background: paper, padding 7rem 4rem

Tier rows (NOT cards — use horizontal rows):
- Each row: 2-column grid (180px left / 1fr right)
- Full-width border top+bottom: 1.5px solid ink
- Rows share bottom borders (margin-bottom: -1.5px to merge them)
- Hover: transform translate(-3px, -3px) + box-shadow 3px 3px 0 ink

Left cell (price column):
- Background: rgba(0,0,0,0.04), border-right 1.5px ink
- Tier tag: IBM Plex Mono, 0.6rem, ember, uppercase
- Price: Bebas Neue, 2.5rem, ink (canary on featured dark row)
- Note: IBM Plex Mono, 0.62rem, mid

Right cell:
- Name: Syne 800, 1.2rem, ink
- Essence: IBM Plex Mono, 0.72rem, teal, italic
- Description: Syne 400, 0.9rem, #444
- Teams pill: IBM Plex Mono 0.65rem, ember, border 1px dashed ember, padding 0.25rem 0.55rem

Featured (Core) row: background ink, text cream, adjust colors accordingly

Brain on Call box:
- Background: cream
- Border: 1px rgba(0,0,0,0.12)
- Horizontal layout: label (Bebas navy, 1.4rem) + body text + CTA button
- Padding: 1.5rem 2rem

### TESTIMONIALS
- Frame: 100vw, background: cream
- Border top + bottom: 2px solid ink
- 3-column card grid
- Each card: border 1.5px ink, white background, padding 2rem
- Large decorative quote mark: Playfair Display, 5.5rem, canary, positioned absolute
- Quote text: Playfair italic, 1rem, line-height 1.65
- Attribution: IBM Plex Mono, 0.72rem, mid; name in ink

### FAQ
- Frame: 100vw, background: paper, padding 6rem 4rem
- Layout: 2-column (1fr 2fr), gap 5rem
- Left: sidebar with section label, large Bebas heading, body note
- Right: Use the FAQ Code Component from framer-code-snippets.js
  OR build manually with Framer's built-in accordion interaction

### BOOKING
- Frame: 100vw, background: ember, padding 7rem 4rem
- Layout: 2-column (1.2fr 1fr), gap 5rem
- Left: Bebas Neue title in white, body copy in white at 78%
- Right: white form box
  Clip path on form box: polygon(0 0, calc(100% - 16px) 0, 100% 16px, 100% 100%, 16px 100%, 0 calc(100% - 16px))
  Note: Framer doesn't support clip-path natively.
  Either: (a) use a Code Override, or (b) skip the chamfer and use a plain rectangle

### FOOTER
- Frame: 100vw, background: ink, padding 3rem 4rem
- Horizontal flex, space-between, wrap
- Brand wordmark text (same color rules as nav)
- Links: IBM Plex Mono, 0.72rem, mid, uppercase, hover canary
- Copyright: full-width row below, border-top 1px rgba(255,255,255,0.07), IBM Plex Mono 0.68rem mid

---

## PHASE 4: SCROLL ANIMATIONS

For every major section element:
1. Select the Frame or text layer
2. Right panel → Appearance → Scroll Effects
3. Set: Initial opacity 0, Final opacity 1
4. Set: Initial Y offset 24px, Final Y offset 0px
5. Trigger: "When enters viewport" at 10% threshold
6. Duration: 0.7s, Ease: ease-out
7. For staggered reveals (e.g. manifesto lines), add increasing delay:
   line 1: 0s, line 2: 0.1s, line 3: 0.2s, line 4: 0.3s

Hero elements use entrance animations (not scroll), set in the Framer
Animate panel with a page-load trigger.

---

## PHASE 5: CODE COMPONENTS

For the three components that need code:

**Ticker:** Assets panel → + → New Code File → Ticker.tsx
Paste the TICKER_COMPONENT code from framer-code-snippets.js
Drag onto canvas in the ticker section.

**FAQ Accordion:** Same process → FAQ.tsx → paste FAQ_COMPONENT
Drag into the right column of the FAQ section.

**Chamfered Button:** Same → ButtonPrimary.tsx → paste BUTTON_COMPONENT
Use wherever you need the primary CTA button.

**Animated Brain Web:** BrainWeb.tsx → paste BRAINWEB_COMPONENT
Place inside hero frame as absolute layer.

---

## PHASE 6: FORM SETUP

Framer has a built-in Form component. Use it for the booking form:

1. Insert → Form → drag into the booking section right column
2. Add fields: name, email, text (conference), select (format), textarea
3. Connect to: either Framer's built-in form submissions (Site Settings → Forms)
   or use a Typeform/Tally embed for more control
4. Redirect on submit: a simple "Thanks — I'll be in touch" message is fine.
   No need for a separate page.

**Recommended:** Use Tally.so for the form. It's free, looks clean,
can be embedded as an iframe, and sends to email + Notion/Airtable.
It keeps the form functional even if Framer's hosting changes.

---

## PHASE 7: SEO + META

Site Settings → SEO:
- Title: Stump Jerry's Brains — Ask Something That Matters
- Description: Live, virtual sensemaking sessions for conferences.
  Jerry Michalski brings 28 years of connected thinking to your
  hardest questions. Ask something that matters.

For the OG image (social share preview — 1200×630px):
Create in Figma (free):
- Background: #0A0A0A
- "STUMP JERRY'S BRAINS" in Bebas Neue, ~130pt, cream
  Final 's' in ember
- Subtitle: "Ask Something That Matters" in IBM Plex Mono, 24pt, canary
- Small brain-web SVG in bottom-right corner
- Export as PNG → upload to Site Settings → SEO → Social Image

---

## PHASE 8: PUBLISH

1. Framer toolbar → Publish → Connect stumpjerrysbrain.com
2. SSL is handled automatically by Framer
3. Set up the www redirect in your domain registrar's DNS settings
   (Framer's help docs cover this for every major registrar)

First publish checklist:
[ ] Fonts loading correctly in preview
[ ] Ticker animating smoothly
[ ] FAQ accordion opening/closing
[ ] Scroll reveals triggering
[ ] Form submitting (test with a real submission)
[ ] OG image showing correctly (use opengraph.xyz to preview)
[ ] Mobile layout not broken at 390px
[ ] Custom cursor not showing on mobile (add media query to disable)

---

## QUICK REFERENCE: HTML PROTOTYPE → FRAMER MAPPING

The HTML prototype (index.html) is your design source of truth.
If you're ever unsure how something should look, open it in Chrome
and use DevTools to inspect the exact values.

Key things to check in DevTools:
- Right-click any element → Inspect → Computed tab → see all CSS values
- The Elements panel shows the exact HTML structure
- Network tab → Fonts → confirms which fonts are loading

The HTML file can also be hosted as-is on Netlify (drag the file to
netlify.com/drop) as a live preview while the Framer build is in progress.
This gives you something real to share with collaborators or clients
before the Framer site is complete.

---

## ESTIMATED BUILD TIME

| Phase | Time |
|-------|------|
| Setup (fonts, colors, code) | 20 min |
| Import SVG assets | 10 min |
| Nav + Hero | 45 min |
| Ticker + Story section | 30 min |
| How It Works + Brain Demo | 30 min |
| Offers tier stack | 40 min |
| Testimonials + FAQ + Booking + Footer | 45 min |
| Scroll animations | 20 min |
| Code components | 30 min |
| Form setup + SEO + OG image | 20 min |
| Mobile responsive fixes | 30 min |
| **Total** | **~5.5 hours** |

This assumes you're comfortable with Framer's canvas. If it's your
first Framer project, add 2 hours for getting oriented.

---

## ONE LAST THING

The HTML prototype is production-quality and fully self-contained.
If you want to launch immediately while building the Framer version
properly: drop index.html on Netlify Drop (netlify.com/drop) right
now. It will be live in 60 seconds at a Netlify subdomain.
Point your domain at it while you build in Framer.
No shame in shipping the HTML version first.
