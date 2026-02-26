# 🏗️ VATEV RÉNOVATION — WEBSITE BUILD PLAN
## Complete specification for Claude Code agent

---

## 📋 PROJECT OVERVIEW

**Client:** Vatev Rénovation  
**Location:** Paris, France  
**Type:** Premium interior renovation company  
**Tech Stack:** Single HTML file (HTML + CSS + JS, no frameworks needed)  
**Output:** `index.html` — fully self-contained, production-ready website  
**Language:** French (primary), with subtle multilingual awareness  

---

## 🎯 BRAND POSITIONING

Vatev Rénovation is a **premium Paris-based renovation artisan** built entirely on reputation and referrals — zero paid advertising. This is the core brand story and must be felt immediately.

**Key differentiators:**
- 6 years of Parisian interior expertise
- Zero paid advertising — 100% word-of-mouth reputation
- Luxury finishes at competitive rates
- Professional-grade machines and materials
- Works with architects and demanding private clients

**Emotional promise:**  
*"Chaque projet est réalisé comme si c'était notre propre intérieur."*

---

## 🎨 DESIGN DIRECTION

### Aesthetic: **Refined Parisian Luxury**
Think Haussman apartment meets contemporary atelier. NOT cold minimalism. NOT corporate. Think **warm, tactile, artisanal prestige**.

### Color Palette (CSS variables)
```css
--cream: #F5F0E8;
--warm-white: #FAFAF7;
--charcoal: #1C1C1A;
--dark-grey: #2E2D2B;
--medium-grey: #6B6860;
--light-grey: #D4D0C8;
--wood-warm: #8B6F47;
--wood-light: #C4A882;
--gold-accent: #B8965A;
--gold-light: #D4AF7A;
```

### Typography
- **Display / Headings:** `Cormorant Garamond` (Google Fonts) — elegant, editorial, Parisian
- **Body:** `Jost` (Google Fonts) — clean, modern, readable
- **Accent/Labels:** `Cormorant Garamond` italic for pull quotes

### Visual Language
- Generous white space (premium feels spacious)
- Thin horizontal lines as dividers
- Subtle grain texture overlay on hero section
- Smooth scroll behavior
- Fade-in animations on scroll (IntersectionObserver)
- Hover micro-interactions on buttons and nav
- NO drop shadows everywhere — use negative space instead
- Photography-first design — large images, minimal text overlay

---

## 🏗️ WEBSITE STRUCTURE

### Navigation (Fixed, transparent → solid on scroll)
```
Logo: "VATEV" (top left, elegant serif)
Nav links: Accueil | Services | Réalisations | À Propos | Contact
CTA button: "Demander un devis" (gold accent, top right)
```
On mobile: hamburger menu with full-screen overlay.

---

### SECTION 1 — HERO (Full viewport)

**Layout:** Full-screen with large background image + text overlay

**Background image:** Use this URL:
`https://hips.hearstapps.com/hmg-prod/images/uchronia-paris-apartment-living-room-64e4888ea1eb6.jpg`

**Content:**
```
[small uppercase label] ARTISAN RÉNOVATEUR · PARIS

[H1 — large, Cormorant Garamond]
Rénovation Intérieure
Haut de Gamme à Paris

[subtitle — Jost, light weight]
Finitions Parfaites. Détails Maîtrisés. Résultat Durable.

[two CTA buttons]
→ "Demander un devis" (filled, gold)
→ "Voir nos réalisations" (outline, white)

[bottom of hero — scroll indicator with animated arrow]
```

**Overlay:** Semi-transparent dark gradient from bottom — so text is readable but photo shines.

---

### SECTION 2 — STATS / TRUST BAR

**Layout:** 4 columns, centered, clean

```
| 6 ans        | 100%           | 0€           | Paris         |
| d'expertise  | recommandations| publicité    | & Île-de-France|
| à Paris      | clients        | bouche à oreille | Exclusivement |
```

Style: thin top/bottom borders, gold numbers, grey labels.

---

### SECTION 3 — SERVICES

**Section title:** 
```
Nos Prestations
— Services haut de gamme pour votre intérieur —
```

#### Service Card 1: Peinture & Enduits
**Image:** `https://hips.hearstapps.com/hmg-prod/images/uchronia-paris-apartment-living-room-64e4888ea1eb6.jpg`  
**Title:** Peinture & Finitions  
**Description:** Préparation complète des surfaces, enduits et lissage parfait, peintures premium avec finitions mates, satinées ou velours. Chaque mur devient une toile.  
**Services list:**
- Enduits et lissage parfait
- Peintures premium (mate, satinée, velours)
- Préparation complète des surfaces
- Finitions décoratives sur mesure

#### Service Card 2: Parquet & Sols
**Image:** `https://mcmillanfloors.com/cdn/shop/articles/getty-images-GjLnhJgS_kc-unsplash.jpg?v=1755842465&width=2000`  
**Title:** Parquet & Sols  
**Description:** De la pose à la rénovation, nous maîtrisons tous les aspects du parquet — massif, contrecollé, ponçage et vitrification pour redonner vie à vos sols anciens.  
**Services list:**
- Pose parquet massif & contrecollé
- Ponçage et vitrification
- Réparation parquet ancien
- Préparation et ragréage des sols

**Layout:** Two large cards, side by side. Each card: image top (60% height), content bottom. Hover: subtle image zoom + gold border-left appears.

---

### SECTION 4 — PHILOSOPHY / ABOUT

**Layout:** Split — left image, right text (alternating)

**Image (left):** `https://egerton-place-no297_walls_living-room_portrait_archive-collection_mylands_2021.jpg` — use: `https://cdn.shopify.com/s/files/1/2983/8386/t/20/assets/egerton-place-no297_walls_living-room_portrait_archive-collection_mylands_2021-1633950259429.jpg`

**Text (right):**
```
[small label] NOTRE PHILOSOPHIE

[H2] L'Excellence
par le Détail

[body text]
Depuis 6 ans, nous intervenons dans les intérieurs les plus exigeants de Paris.
Notre réputation s'est construite uniquement sur la qualité de notre travail et 
les recommandations de nos clients satisfaits — jamais sur la publicité.

Nous croyons qu'une rénovation réussie commence bien avant le premier coup de 
pinceau : par une préparation rigoureuse, des matériaux sélectionnés et une 
attention absolue aux détails.

[italic pull quote — Cormorant Garamond]
"Chaque projet est réalisé comme si c'était notre propre intérieur."

[small text — stats]
✦ Machines professionnelles dernière génération
✦ Matériaux premium sélectionnés
✦ Respect des délais garanti
✦ Devis détaillé et transparent
```

---

### SECTION 5 — SOCIAL PROOF / TESTIMONIALS

**Section title:** Ils Nous Font Confiance

**Layout:** 3 testimonial cards in a row

**Testimonial 1:**
```
★★★★★
"Travail impeccable, finitions parfaites. Je recommande sans hésiter 
à tous mes amis qui cherchent un artisan sérieux à Paris."
— Marie L., 16ème arrondissement
```

**Testimonial 2:**
```
★★★★★  
"Notre architecte nous a recommandé Vatev pour la peinture de notre 
appartement haussmannien. Le résultat est au-delà de nos espérances."
— Pierre & Sophie D., 8ème arrondissement
```

**Testimonial 3:**
```
★★★★★
"Professionnalisme exemplaire. Les enduits sont parfaits, on ne voit 
aucune irrégularité. Je referai appel à eux sans hésiter."
— Jean-Marc B., Neuilly-sur-Seine
```

**Style:** Light card with cream background, gold stars, italic quote text, small divider line before attribution.

**Below testimonials — trust badges row:**
```
[Google Logo] 5.0 ★★★★★  |  Recommandé par des architectes  |  6 ans d'expérience
```

---

### SECTION 6 — PROCESS / HOW WE WORK

**Section title:** Notre Processus

**Layout:** 4 steps in horizontal timeline

```
01              02              03              04
Devis           Préparation     Réalisation     Livraison
Gratuit         Rigoureuse      Haut de Gamme   Parfaite

Visite sur      Protection      Travaux avec    Nettoyage
place et        complète du     matériaux       complet et
estimation      chantier        premium         remise des clés
détaillée
```

**Style:** Numbers in gold circles, connected by thin line, clean minimal layout.

---

### SECTION 7 — CONTACT / QUOTE REQUEST

**Layout:** Split — left info, right form

**Left side:**
```
[H2] Demandez Votre Devis Gratuit

[body]
Contactez-nous pour une visite sur place et 
une estimation détaillée, sans engagement.

[contact details]
📍 Paris & Île-de-France
📞 [PHONE — to be filled by client]
✉ [EMAIL — to be filled by client]

Délai de réponse : sous 24h
```

**Right side — Contact Form:**
```
Fields:
- Nom complet (text)
- Téléphone (tel)  
- Email (email)
- Arrondissement / Ville (text)
- Type de travaux (select: Peinture | Parquet | Les deux | Autre)
- Description du projet (textarea)
- [Submit button: "Envoyer ma demande" — gold, full width]
```

**Note for agent:** The form should use `mailto:` action or show a success message on submit. Add `netlify` attribute if deploying to Netlify, otherwise use `action="mailto:contact@vatev-renovation.fr"`.

---

### SECTION 8 — FOOTER

**Layout:** 4 columns

```
Col 1: Logo + tagline
"VATEV RÉNOVATION"
Artisan Rénovateur à Paris
Finitions Haut de Gamme

Col 2: Navigation
Accueil
Services  
Réalisations
À Propos
Contact

Col 3: Services
Peinture & Enduits
Parquet & Sols
Rénovation complète
Conseil et expertise

Col 4: Contact
Paris & Île-de-France
[phone placeholder]
[email placeholder]
```

**Bottom bar:**
```
© 2024 Vatev Rénovation · Tous droits réservés · Artisan rénovateur Paris
```

---

## 📱 RESPONSIVE BREAKPOINTS

```
Mobile: < 768px
  - Single column layout
  - Hamburger navigation
  - Stack all split sections
  - Reduce hero text size
  - Cards in single column

Tablet: 768px - 1200px  
  - Services: 2 columns
  - Testimonials: 2 columns
  - Stats: 2x2 grid

Desktop: > 1200px
  - Full layout as described above
  - Max-width: 1400px, centered
```

---

## ⚡ ANIMATIONS & INTERACTIONS

```javascript
// Implement these:

1. Scroll-triggered fade-in:
   - All sections fade up on enter (opacity 0 → 1, translateY 30px → 0)
   - Use IntersectionObserver
   - Stagger children with animation-delay

2. Navigation:
   - Transparent on hero → white/cream background on scroll
   - Smooth transition (background + box-shadow)

3. Service cards hover:
   - Image: scale(1.05) with overflow hidden
   - Gold left border appears
   - Slight translateY(-4px)

4. Buttons hover:
   - Gold button: darken background + subtle scale
   - Outline button: fill with gold color

5. Hero scroll indicator:
   - Animated bouncing arrow / chevron
   - Fade out on scroll

6. Stats counter:
   - Animate numbers counting up when in view
   - "6" counts to 6, etc.
```

---

## 🔤 GOOGLE FONTS TO IMPORT

```html
<link rel="preconnect" href="https://fonts.googleapis.com">
<link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
<link href="https://fonts.googleapis.com/css2?family=Cormorant+Garamond:ital,wght@0,300;0,400;0,500;0,600;1,300;1,400&family=Jost:wght@300;400;500&display=swap" rel="stylesheet">
```

---

## 🔍 SEO META TAGS

```html
<title>Vatev Rénovation | Artisan Peinture & Parquet Haut de Gamme Paris</title>
<meta name="description" content="Artisan rénovateur à Paris spécialisé en peinture décorative, enduits, pose et rénovation de parquet. 6 ans d'expertise. Devis gratuit.">
<meta name="keywords" content="rénovation intérieure Paris, peinture haut de gamme Paris, pose parquet Paris, enduits décoration Paris, artisan rénovation Paris">
<meta property="og:title" content="Vatev Rénovation | Peinture & Parquet Haut de Gamme Paris">
<meta property="og:description" content="6 ans d'expertise en rénovation intérieure à Paris. Peinture, enduits, parquet. Recommandé uniquement par la qualité.">
```

---

## 📁 FILE OUTPUT

The agent must produce **one single file:**
```
index.html
```

All CSS must be in `<style>` tags inside the HTML.
All JavaScript must be in `<script>` tags at the bottom of the HTML.
No external dependencies except Google Fonts (CDN) and the image URLs provided.

---

## ✅ QUALITY CHECKLIST FOR AGENT

Before finishing, verify:
- [ ] All 8 sections are present
- [ ] Navigation works (smooth scroll to sections)
- [ ] Mobile responsive (test with CSS breakpoints)
- [ ] All images load (use provided URLs)
- [ ] Animations work on scroll
- [ ] Contact form is styled and functional
- [ ] Google Fonts load correctly
- [ ] Color palette matches spec
- [ ] Typography uses Cormorant Garamond for headings
- [ ] Footer has all 4 columns
- [ ] No Lorem Ipsum — all text is final French content
- [ ] Hero CTA buttons both work (scroll to sections)
- [ ] Meta tags for SEO are present

---

## 🚀 CLAUDE CODE COMMAND TO USE

When running with Claude Code, use this prompt:

```
Build a complete, production-ready single HTML file website for "Vatev Rénovation" 
following every specification in VATEV_WEBSITE_PLAN.md exactly. 
Create index.html with all HTML, CSS and JS in one file. 
Prioritize visual excellence — this is a luxury brand and the design must feel premium.
```

---

*Plan created for Claude Code agent — Vatev Rénovation website v1.0*
