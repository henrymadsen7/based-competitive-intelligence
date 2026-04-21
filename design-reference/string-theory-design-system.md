# String Theory Design System
## For Based Agent Platform
## Inspired by string-tune.fiddle.digital + Based brand evolution

### Core Principles
1. **CSS-first, JS-light:** Animations via CSS custom properties and transforms. JS orchestrates, CSS executes.
2. **60FPS or nothing:** Every interaction must be composited. No layout thrashing.
3. **Attribute-driven behavior:** `data-animate="reveal"`, `data-scroll="parallax"`, `data-cursor="magnetic"`
4. **Typography as interface:** Text is not static. It breathes, responds, guides.
5. **Zen density:** Maximum information, minimum clutter. Every pixel earns its place.
6. **Scroll as narrative:** The page unfolds like a story. Progress is visible and rewarding.

---

## Color Palette

### Primary (Based Forest)
- `bg-primary`: `#0a1f18` (deeper than current #102820 for more depth)
- `bg-secondary`: `#102820` (current Based green)
- `bg-elevated`: `rgba(16, 40, 32, 0.88)`
- `bg-panel`: `rgba(10, 25, 20, 0.72)`

### Text (Warm Cream)
- `text-primary`: `#f1ead9`
- `text-soft`: `rgba(241, 234, 217, 0.72)`
- `text-faint`: `rgba(241, 234, 217, 0.46)`
- `text-muted`: `rgba(241, 234, 217, 0.28)`

### Accent (Warm Earth)
- `accent`: `#8a6240` (current Based brown)
- `accent-light`: `#a67c52`
- `accent-glow`: `rgba(138, 98, 64, 0.4)`
- `tertiary`: `#caba9c`

### Semantic
- `success`: `#91b49b`
- `warning`: `#d4a574`
- `error`: `#c4746e`
- `info`: `#7daeb5`

### Effects
- `line`: `rgba(202, 186, 156, 0.12)`
- `line-strong`: `rgba(202, 186, 156, 0.22)`
- `shadow-sm`: `0 4px 16px rgba(0, 0, 0, 0.2)`
- `shadow-md`: `0 8px 32px rgba(0, 0, 0, 0.28)`
- `shadow-lg`: `0 24px 80px rgba(0, 0, 0, 0.4)`
- `glow-accent`: `0 0 28px rgba(138, 98, 64, 0.3)`

---

## Typography

### Font Stack
- Primary: `-apple-system, BlinkMacSystemFont, "SF Pro Display", "SF Pro Text", "Helvetica Neue", Helvetica, Arial, sans-serif`
- Mono: `"SF Mono", SFMono-Regular, ui-monospace, "Cascadia Code", "Fira Code", monospace`
- Display (optional): `"Instrument Serif", Georgia, serif` for editorial moments

### Scale
- `display`: `clamp(3rem, 8vw, 6rem)` / weight 700 / letter-spacing -0.02em
- `h1`: `clamp(2.5rem, 5vw, 4rem)` / weight 600 / letter-spacing -0.01em
- `h2`: `clamp(1.75rem, 3vw, 2.5rem)` / weight 600 / letter-spacing -0.005em
- `h3`: `clamp(1.25rem, 2vw, 1.75rem)` / weight 500
- `body`: `1rem` (16px) / weight 400 / line-height 1.6
- `body-sm`: `0.875rem` / weight 400 / line-height 1.5
- `caption`: `0.75rem` / weight 500 / letter-spacing 0.02em / uppercase
- `micro`: `0.6875rem` / weight 500 / letter-spacing 0.04em / uppercase

### Kinetic Typography Patterns
1. **Reveal on scroll:** Text characters split and fade in with staggered delay based on scroll position
2. **Text with progress:** Headline opacity/tracking tied to `--scroll-progress`
3. **Kinetic text:** Words shuffle and resolve on hover or scroll intersection
4. **Split and lerp:** Characters separate and recombine with smooth interpolation
5. **Cursor proximity:** Text weight or tracking subtly shifts as cursor approaches

---

## Layout & Grid

### Container
- `max-width`: `1240px`
- `padding`: `clamp(1.5rem, 5vw, 3rem)`
- Centered with auto margins

### Grid
- 12-column implicit grid
- `gap`: `clamp(1rem, 2vw, 2rem)`
- Breakpoints: `sm: 640px`, `md: 768px`, `lg: 1024px`, `xl: 1280px`, `2xl: 1536px`

### Spacing Scale
- Based on `0.25rem` (4px) increments
- Key values: `4, 8, 12, 16, 24, 32, 48, 64, 96, 128`

---

## Components

### Header Pill
- Fixed position, centered
- Height: `48px`
- Background: `rgba(10, 25, 20, 0.72)`
- Border: `1px solid rgba(202, 186, 156, 0.55)`
- Backdrop-filter: `blur(20px) saturate(150%)`
- Border-radius: `14px`
- Shadow: `0 0 0 1px rgba(202, 186, 156, 0.08), 0 0 24px rgba(202, 186, 156, 0.08)`
- On scroll: background darkens, border strengthens, shadow deepens

### Buttons
- **Primary:** `bg-accent`, `text-primary`, `px-6 py-3`, `rounded-xl`, `font-medium`
  - Hover: `translateY(-1px)`, `shadow-glow`, `brightness(1.1)`
  - Active: `translateY(0)`, `brightness(0.95)`
- **Secondary:** `bg-transparent`, `border line-strong`, `text-primary`
  - Hover: `bg-panel`, `border-accent`
- **Ghost:** No background/border, `text-soft`
  - Hover: `text-primary`, subtle underline animation

### Cards
- Background: `bg-panel`
- Border: `1px solid line`
- Border-radius: `16px`
- Padding: `24px`
- Shadow: `shadow-sm`
- Hover: `border-color line-strong`, `shadow-md`, `translateY(-2px)`

### Input Fields
- Background: `rgba(10, 25, 20, 0.5)`
- Border: `1px solid line`
- Border-radius: `12px`
- Height: `44px`
- Focus: `border-accent`, `shadow-glow`
- Placeholder: `text-faint`

### Scroll Progress Indicator
- Fixed top or bottom of viewport
- Thin line (`2px`) in `accent` color
- Width tied to `--scroll-progress`
- Smooth transition, no JS frame loops (CSS animation-timeline or scroll-driven)

---

## Animation System

### Easing
- `--ease-smooth`: `cubic-bezier(0.2, 0.8, 0.2, 1)` (primary)
- `--ease-snap`: `cubic-bezier(0.16, 1, 0.3, 1)`
- `--ease-bounce`: `cubic-bezier(0.34, 1.56, 0.64, 1)`

### Core Effects
1. **Smooth scroll:** Native scroll with CSS `scroll-behavior: smooth` + precision smoothing formula for JS-enhanced
2. **Reveal on scroll:** Elements fade up and in as they enter viewport. Staggered children.
3. **Parallax:** Multi-layer depth. Background moves at 0.2x, content at 1x, foreground accents at 1.5x.
4. **Progress-driven:** Any property tied to scroll progress via CSS `animation-timeline: scroll()` or `--progress` variable.
5. **Cursor tracking:** Subtle elements that follow cursor with lerp (linear interpolation) smoothing.
6. **Magnetic buttons:** Buttons that subtly attract toward cursor on proximity.
7. **Spotlight:** Radial gradient following cursor, revealing content in darkness.
8. **Impulse:** Quick, sharp micro-animations for state changes (success, error, loading).

### Performance Rules
- Use `transform` and `opacity` only for animations
- Apply `will-change` sparingly, remove after animation
- Use `contain: layout style paint` on animated containers
- Prefer CSS transitions over JS animation loops
- Use `IntersectionObserver` for scroll triggers, not scroll event listeners
- Throttle any necessary JS to RAF (requestAnimationFrame)

---

## Unique Design Signatures

### 1. The "Scroll Narrative"
The page is not a document. It is a journey. Each section reveals like a chapter. Progress is always visible.

### 2. Kinetic Typography
Text is alive. It responds to scroll, cursor, and interaction. Not decorative — functional and delightful.

### 3. Zen Density
So much white space it feels luxurious. Then, when density is needed, it is precise and scannable.

### 4. Crafted Corners
Border radii are intentional. Not everything is rounded. Some elements are sharp to create contrast and hierarchy.

### 5. Warm Glow
The accent brown glows softly. Never harsh neon. It feels like candlelight in a forest.

### 6. Glass That Breathes
Glassmorphism is used sparingly — header pill, modals, dropdowns. It darkens and sharpens on scroll.

---

## Implementation Notes

### CSS Architecture
- Use CSS custom properties for all tokens
- Utility-first with Tailwind, but custom components for complex patterns
- String Theory animations as a separate CSS layer that can be disabled for accessibility

### Accessibility
- Respect `prefers-reduced-motion`: disable kinetic effects, keep fades only
- All text meets WCAG AA contrast ratios
- Keyboard-navigable throughout
- Focus states are visible and beautiful

### Responsive
- Mobile-first, but desktop is the primary experience for the app
- Kinetic typography simplifies on mobile (fewer particles, simpler reveals)
- Touch interactions replace cursor effects
