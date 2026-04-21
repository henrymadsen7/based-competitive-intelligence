# Based-Website Design Integration Spec
## How to inject String Theory into the current Based site

### Current State
- Static HTML/CSS site on Cloudflare Pages
- Deep forest green (#102820) + warm cream (#f1ead9) palette
- Glassmorphism header pill
- Editorial, refined aesthetic
- No JavaScript animation system

### Target State
- Same color palette (it is already strong)
- Add kinetic typography to hero section
- Add scroll-driven reveal animations to all sections
- Add cursor spotlight effect on hero
- Add scroll progress indicator at top
- Keep static architecture (no framework needed for marketing site)

### Implementation Plan

#### Phase 1: Core Animation CSS (1 file, ~10KB)
Add `string-theory.css` with:
- `--scroll-progress` variable updated via minimal JS
- `@keyframes` for reveal, parallax, fade
- Utility classes: `.st-reveal`, `.st-parallax`, `.st-magnetic`, `.st-spotlight`

#### Phase 2: Hero Enhancement
- Hero headline uses split-text reveal on load
- Subtle parallax on background gradient
- Cursor spotlight reveals subtle texture in dark background
- Scroll indicator bounces gently at bottom

#### Phase 3: Section Reveals
- Each section heading uses `.st-reveal` (fade up + character stagger)
- Feature cards stagger in on scroll
- Testimonials use subtle parallax depth

#### Phase 4: Interactive Moments
- Magnetic buttons on primary CTAs
- Cards lift and glow on hover
- Navigation links have animated underline

### Code Sample: Scroll Progress + Reveal
```css
/* string-theory.css */
:root {
  --scroll-progress: 0;
  --ease-smooth: cubic-bezier(0.2, 0.8, 0.2, 1);
}

html {
  scroll-behavior: smooth;
}

/* Progress bar */
.scroll-progress {
  position: fixed;
  top: 0;
  left: 0;
  height: 2px;
  background: #8a6240;
  width: calc(var(--scroll-progress) * 100%);
  z-index: 100;
  transition: width 0.1s linear;
}

/* Reveal animation */
.st-reveal {
  opacity: 0;
  transform: translateY(24px);
  transition: opacity 0.8s var(--ease-smooth), transform 0.8s var(--ease-smooth);
}
.st-reveal.is-visible {
  opacity: 1;
  transform: translateY(0);
}

/* Stagger children */
.st-reveal.is-visible > *:nth-child(1) { transition-delay: 0ms; }
.st-reveal.is-visible > *:nth-child(2) { transition-delay: 80ms; }
.st-reveal.is-visible > *:nth-child(3) { transition-delay: 160ms; }
.st-reveal.is-visible > *:nth-child(4) { transition-delay: 240ms; }
.st-reveal.is-visible > *:nth-child(5) { transition-delay: 320ms; }
```

```javascript
// string-theory.js (minimal, ~2KB)
(function() {
  // Update scroll progress
  function updateProgress() {
    const scrollTop = window.scrollY;
    const docHeight = document.documentElement.scrollHeight - window.innerHeight;
    const progress = docHeight > 0 ? scrollTop / docHeight : 0;
    document.documentElement.style.setProperty('--scroll-progress', progress);
  }
  window.addEventListener('scroll', updateProgress, { passive: true });
  updateProgress();

  // IntersectionObserver for reveals
  const observer = new IntersectionObserver((entries) => {
    entries.forEach(entry => {
      if (entry.isIntersecting) {
        entry.target.classList.add('is-visible');
        observer.unobserve(entry.target);
      }
    });
  }, { threshold: 0.1, rootMargin: '0px 0px -50px 0px' });

  document.querySelectorAll('.st-reveal').forEach(el => observer.observe(el));
})();
```

### Risk Mitigation
- All animations respect `prefers-reduced-motion`
- CSS-only fallback for no-JS environments
- Minimal bundle impact (<15KB total)
- No framework dependencies
