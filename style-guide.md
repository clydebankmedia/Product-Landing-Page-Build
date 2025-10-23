# Style Guide -Product Landing Page Build 

Use this guide throughout your build when applying styling. You don’t need to memorize the values, just check back whenever you’re making layout, spacing, or typography decisions.


## Typography

- **Headings:** Montserrat, sans-serif
- **Body text:** Open Sans, sans-serif
- **Base size:** `16px`
- **Line height:** `1.6` (comfortable reading)
- **Heading sizes:**
    - H1: `2.5rem`
    - H2: `2rem`
    - H3: `1.5rem`


## Color Palette

- **Primary dark (text, dark UI):** `#2C3E50`
- **Accent blue (borders, highlights):** `#3498DB`
- **Accent orange (primary CTA):** `#E67E22`
- **Light background:** `#F9F9F9`
- **Border gray:** `#DDDDDD`
- **CTA gradient:** `linear-gradient(135deg, #2C3E50, #3b4d63)`


## Layout & Spacing

- **Max page width:** `1120px` (inside `.container`)
- **Gutters (side padding):** `1rem`
- **Vertical rhythm:** Add generous padding (`4rem 0`) to separate sections
- **Nav bar:** Full-width background; content sits inside centered `.container`


## UI Components

- **Buttons:**
    - Fill: Accent orange
    - Text: White
    - Padding: `0.75rem 1.5rem`
    - Rounded corners: `4px`
    - Hover: Darker orange or subtle opacity shift
- **Cards (Why Us/Services):**
    - Border: `1px solid #DDDDDD`
    - Padding: `1.5rem`
    - Shadow: Subtle on hover
- **Reviews:**
    - Background: White
    - Padding: `1.5rem`
    - Drop shadow for depth
    - Quote text italic with left border accent (blue)



## Imagery

- **Hero:**
    - Use a full-bleed Unsplash image (pets/cleaning theme).
      - Asset used in mockup: `https://images.unsplash.com/photo-1517849845537-4d257902454a?w=1600&q=80&auto=format&fit=crop` 
    - Use `background-size: cover;` and `background-position: center;`.
    - Overlay with semi-transparent dark layer for contrast.
- **Other images (if used):**
    - Rounded corners optional
    - Consistent sizing within a section


## Accessibility

- Always check **color contrast** (light text on dark backgrounds, dark text on light).
- Ensure **hover states** also provide visual cues (not just color).
- Don’t remove browser **focus outlines**; instead, style them clearly.