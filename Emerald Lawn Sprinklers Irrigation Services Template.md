---
version: alpha
name: Emerald Lawn Sprinklers
description: A professional irrigation services design system utilizing a high-contrast 'nature-tech' aesthetic with deep forest greens, cream surfaces, and technical diagrammatic elements.
colors:
  bg-ink: "#0C1208"
  bg-deep: "#141C0F"
  surface-cream: "#F0F4EC"
  surface-stone: "#DDE8D4"
  accent-green: "#4A8C2A"
  accent-lime: "#6DB33F"
  text-dark: "#111A0C"
  text-light: "#F4FAF0"
typography:
  headings:
    family: "Sora"
    weight: 500-800
    letterSpacing: "-0.085em"
  body:
    family: "Inter"
    weight: 400-800
    lineHeight: 1.7
spacing:
  section-padding: "8rem"
  inner-gap: "1.5rem"
rounded:
  md: "20px"
  lg: "28px"
  full: "999px"
components:
  buttons:
    primary:
      bg: "linear-gradient(135deg, #9FD96A, {colors.accent-green})"
      shadow: "0 14px 40px rgba(74, 140, 42, 0.28)"
  cards:
    glass:
      bg: "rgba(255, 255, 255, 0.055)"
      border: "rgba(244, 250, 240, 0.12)"
---

## Overview
The visual identity for Emerald Lawn Sprinklers is characterized by a "Modern Organic" tone. It combines deep, high-density backgrounds (Ink and Deep Green) with light, breathable surfaces (Cream and Stone). The density is high, featuring data-rich cards, technical metrics, and structured lists. Layouts often utilize diagonal slants (clip-paths) to suggest movement and professional precision. The personality is authoritative, reliable, and technically savvy, moving away from generic landscaping into specialized irrigation engineering.

## Colors
The palette is divided into two primary modes: Dark (Ink/Deep Green) and Light (Cream/Stone).

*   **Primary Brands**: Accent Green (#4A8C2A) and Accent Lime (#6DB33F) are used for interactive elements and highlights.
*   **Backgrounds**: The core dark background is #0C1208 (Ink). The primary light background is a gradient from #F0F4EC to #DDE8D4.
*   **Text**: High-contrast pairing with #F4FAF0 for dark modes and #111A0C for light modes.
*   **Overlays**: A grain overlay using a subtle radial gradient dot pattern (18px size) is applied to sections to add texture and depth.

## Typography
*   **Headings**: Sora is the primary choice for display text, set with extremely tight letter-spacing (-0.045em to -0.09em) and thin line heights (1.05).
*   **Body**: Inter provides high legibility for technical lists and descriptions, typically set at 1.05rem for standard text.
*   **Technical Labels**: Over-sized tracking (0.12em to 0.18em) and all-caps styling are used for eyebrows and kicker text to emphasize the engineering aspect.

## Layout
*   **Sectioning**: Sections utilize `clip-path: polygon()` to create 4vw slants. This creates a staggered, "serrated" vertical flow between light and dark thematic blocks.
*   **Grids**: Most content resides in a 1280px or 1440px shell. Responsive behavior transitions from 2-column or 3-column grids to a single-column stack at 1100px width.
*   **Navigation**: A fixed 78px height bar with a backdrop-blur (18px) and a centralized logo layout.

## Elevation & Depth
*   **Shadows**: Deep, colored drop shadows are used on buttons and active states (e.g., `rgba(74, 140, 42, 0.28)`).
*   **Glassmorphism**: Components in dark sections use a semi-transparent white background (rgba 255, 255, 255, 0.06) with a 1px border to simulate elevated glass surfaces.
*   **Layering**: Content layers are explicitly managed with z-index (up to z-80 for nav) to maintain the separation between background textures and interactive UI.

## Shapes
*   **Radii**: Large, friendly corner radii of 20px (md), 28px (lg), and 32px for main content containers.
*   **Interactive Elements**: Buttons and "chips" (badges) are fully pill-shaped (999px).
*   **Icons**: Wrapped in rounded-square (12px to 16px) or circular frames with subtle border strokes.

## Components
*   **Nav Bar**: Glass-effect container with centered brand lockup and split navigation links (left/right).
*   **Primary Button**: High-visibility green gradient with a slight lift (2px translate) on hover.
*   **Status Chip**: Small, pill-shaped badge containing an Iconify icon and uppercase text used for categories like "Fall" or "Spring".
*   **Impact List**: A horizontal data display with a label on the left and a specific metric (e.g., "48%") on the right, separated by thin borders.
*   **Metric Card**: Feature cards containing a header image, a descriptive body, and a dedicated metrics footer section.

## Page Sections

### Navigation
Fixed-position header with an Inter-weight font. Uses a backdrop-blur for visibility over the hero image. Contains a centered logo and a high-contrast "Get a Quote" CTA on the far right.

### Hero Section
High-impact entry with a full-bleed background image (`hero-bg-layer`). Content is split into a top-line informational bar (Serving area/Service types) and a bottom-aligned title section. The title uses Sora at massive scale (up to 8.4rem) with -0.085em tracking.

### Common Problems (Pain Points)
A light-themed section (#F3F7EE) using a 2-column grid. Each card details a failure point (e.g., Winter Damage) and contains a sub-list of symptoms and a highlighted technical icon.

### Service Scenarios (Systems)
A dark-themed technical breakdown. The left column features a "Scenario List" with a vertical connecting line (timeline/process feel) and glowing green dots. The right column contains overlapping workflow cards with specific category tags.

### Results & Impact
A hybrid section displaying a feature project card next to a benefit list. This area focuses on data quantification (e.g., "Up to 50% less water") and uses high-density layout to prove service value.

### Audit CTA
A full-bleed, high-contrast block using a dark green aesthetic. It features a "Side Card" that summarizes specific audit items with iconography and a statistics row at the bottom.

## Motion & Interaction
*   **Reveal Animations**: A custom `@keyframes revealFlow` is evidenced, applying an opacity/translateY/blur transition (1.1s duration) to items with the `.reveal-item` class.
*   **Hover States**: Buttons translate -2px vertically and increase shadow spread. Feature images (within `impact-card`) scale to 1.04 on container hover.
*   **Scroll Behavior**: Smooth scrolling is globally enabled via CSS.
*   **Technical Glow**: A `diagnostic-rail-glow` animation creates a moving light pulse through technical diagrams to simulate "flow."

## Do's and Don'ts
*   **Do**: Use high-contrast headings with tight tracking. Ensure all icons are from the Solar Iconify set. Use slants to separate major thematic shifts.
*   **Don't**: Use standard square corners or low-radius cards. Avoid using generic blacks; prefer the deep #0C1208 green-black. Do not remove the grain texture from dark backgrounds.

## Accessibility
*   **Contrast**: High-contrast text pairings are enforced for both light and dark modes.
*   **Aria Labels**: Site-nav and mobile-menu buttons include explicit aria-labels.
*   **Semantic HTML**: Header levels (h1-h4) are used sequentially to define content hierarchy.

## Assets
1.  other: https://cdn.tailwindcss.com
2.  other: https://code.iconify.design/iconify-icon/1.0.8/iconify-icon.min.js
3.  embed: https://fonts.googleapis.com/css2?family=Inter:wght@400;500;600;700;800&family=Sora:wght@500;600;700;800&display=swap
4.  other: https://www.googletagmanager.com/gtag/js?id=G-2M6V79H761
5.  image: https://emeraldlawnsprinklers.com/wp-content/uploads/2011/03/logo.png
6.  image: https://hoirqrkdgbmvpwutwuwj.supabase.co/storage/v1/object/public/assets/assets/b5413203-6577-42c0-954e-3811b69415b0_3840w.png
7.  image: https://hoirqrkdgbmvpwutwuwj.supabase.co/storage/v1/object/public/assets/assets/43b80983-9fa2-4c0d-9cbc-19fcb75ccbea_1600w.png?w=800&q=80
8.  other: https://images.unsplash.com/photo-1770664945615-52203ab54c88?w=800&q=80
9.  other: https://images.unsplash.com/photo-1622122123829-e0490a288d04?w=800&q=80
10. image: https://hoirqrkdgbmvpwutwuwj.supabase.co/storage/v1/object/public/assets/assets/3ac110ad-4dc4-4e37-ad7b-367feb87ed83_1600w.jpg?w=800&q=80

### Exported Codebase Asset Inventory
1. embed: https://fonts.googleapis.com/css2?family=Inter:wght@400;500;600;700;800&amp;family=Sora:wght@500;600;700;800&amp;display=swap
   Context: index.html: markup attribute; index.html: absolute url literal
2. image: https://hoirqrkdgbmvpwutwuwj.supabase.co/storage/v1/object/public/assets/assets/43b80983-9fa2-4c0d-9cbc-19fcb75ccbea_1600w.png?w=800&amp;q=80
   Context: index.html: markup attribute; index.html: absolute url literal; index.html: asset string literal
3. other: https://images.unsplash.com/photo-1770664945615-52203ab54c88?w=800&amp;q=80
   Context: index.html: markup attribute; index.html: absolute url literal
4. other: https://images.unsplash.com/photo-1622122123829-e0490a288d04?w=800&amp;q=80
   Context: index.html: markup attribute; index.html: absolute url literal
5. image: https://hoirqrkdgbmvpwutwuwj.supabase.co/storage/v1/object/public/assets/assets/3ac110ad-4dc4-4e37-ad7b-367feb87ed83_1600w.jpg?w=800&amp;q=80
   Context: index.html: markup attribute; index.html: absolute url literal; index.html: asset string literal
