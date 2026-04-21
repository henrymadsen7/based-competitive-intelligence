# Poke (poke.com) — Competitive Intelligence
## Date: 2026-04-20
## Correction Note: Previous research searched for "poke.ai" which was incorrect. The actual company is poke.com.
## Deep-dive reference: `poke-com-deep-dive.md` (this session)

### Company Identity
| Attribute | Detail |
|-----------|--------|
| **Product** | Poke |
| **Company** | Interaction Co. |
| **Domain** | poke.com |
| **Company site** | interaction.co |
| **Location** | Palo Alto, California |
| **Social** | x.com/interaction |
| **Contact** | hi@interaction.co, poke@interaction.co, press@interaction.co |
| **Founded** | Unknown (copyright 2026) |
| **Funding** | Not disclosed |

### Core Value Proposition
"Say hey to Poke" — Ask or get anything done, right from your texts. AI assistant via SMS/text messaging with a "recipe" system for integrations.

### Key Features
- **Text-first interface:** Primary UX is SMS/text messaging (not iMessage-specific like Lindy)
- **Recipe marketplace:** Pre-built integrations called "recipes" for popular tools
- **Custom recipes:** Users can build their own at /kitchen
- **MCP support:** Custom integrations via Model Context Protocol (poke.com/mcp)
- **Privacy-first:** "Maximum Privacy" mode by default; no training on user data
- **One-tap setup:** Recipes activate instantly with a "Get Started" button

### Verified Recipes (20+ across 11 categories)
**Productivity:** Todoist, Linear, Notion, Asana, GitHub, Granola, Journal, Weekly Productivity Check-in
**Developer Tools:** Devin, Cursor Cloud Agents, Vercel, PostHog, Parallel Web Systems
**Health & Wellness:** Oura, Fit, Hydration Reminders, Strava
**Creative / Media:** Canva, Pics
**Smart Home:** Sonos, Philips Hue
**Finance / Operations:** Forward Receipts to Navan
**Information / Lifestyle:** Daily Weather, Daily Horoscope, Bible, Nightly Gratitude
**Students:** Category exists (specific recipes not enumerated)

### Pricing
**No pricing page exists.** /pricing returns 404.
FAQ mentions "the price set by Poke" and asks about discounts, implying:
- Pricing is set but not publicly advertised
- May be revealed post-signup or via SMS
- Likely in early-access / closed beta phase

### Target Audience
General productivity users, developers, health-conscious individuals. Very broad appeal via recipe marketplace. Individual-use focused; no visible team features.

### Tech Stack Signals
- Modern web app (React/Next.js patterns in DOM)
- SMS/phone infrastructure (Twilio or equivalent)
- OAuth integrations with SaaS tools
- LLM-powered natural language understanding
- MCP (Model Context Protocol) for extensibility

### UX/UI Patterns
- Clean, minimal homepage with friendly tone ("Say hey to Poke")
- Recipe cards showing tool icon, name, description, and "Get Started" CTA
- Searchable, paginated recipe catalog with category tabs (All, Automate, Integrate)
- Tag filters: Productivity, Developer, Health, Finance, Scheduling, Travel, Community, Home, Calendar, Email, Students
- Simple two-button hero: "Get Started" + "Explore"
- Light/bright aesthetic (not dark mode)
- Phone number-only onboarding at /get-started

### Privacy & Security
> "By default, your conversations with Poke are as private as your thoughts. When you sign up, we automatically set you to 'Maximum Privacy,' meaning not even we can see your chats. We will **never** change this on your behalf. In this mode, we also **do not** train on user data."

This is a direct competitive differentiator against most cloud AI assistants.

### Integration Ecosystem
Todoist, Linear, Notion, Asana, GitHub, Vercel, Oura, Devin, Granola, Parallel Web Systems, PostHog, Cursor, Canva, Strava, Sonos, Philips Hue, Navan, Fit, and more via recipe system plus MCP custom builds.

### Competitive Weaknesses/Gaps
- **SMS is a ceiling** — Complex multi-step workflows, rich media, and team collaboration are awkward in text messages
- **No team features visible** — Everything appears individual-user focused
- **No pricing transparency** — Users cannot evaluate cost before signing up
- **Limited workflow depth** — Recipes are single-purpose; no chaining, branching, or conditional logic visible
- **No desktop/web workspace** — For serious work, users still need their actual tools
- **Enterprise adoption unlikely** — SMS-based access control, audit trails, and compliance are undefined
- **Recipe system is mostly closed** — While custom recipes exist via /kitchen, the marketplace is dominated by "Poke Team" recipes

### Reverse-Engineering Notes
Poke validates the "AI assistant via text/SMS" model with a recipe/plugin architecture.
To beat them:
- Open recipe marketplace (user-generated, not just Poke Team)
- Visual recipe builder (no-code)
- Team-shared recipes and agents
- Multi-platform (not just SMS — Slack, WhatsApp, Email, Web)
- Transparent pricing
- Code extensibility for power users
- Real workspace for complex work ( Based's strength )

### Verified Claims Log
| Claim | Source | Status |
|-------|--------|--------|
| Domain is poke.com | Direct nav | VERIFIED |
| 20+ recipes | /recipes snapshot | VERIFIED |
| MCP support | FAQ expanded | VERIFIED |
| Maximum Privacy default | FAQ expanded | VERIFIED |
| No training on user data | FAQ expanded | VERIFIED |
| No pricing page | /pricing 404 | VERIFIED |
| Parent is Interaction Co. | Footer + about redirect | VERIFIED |
| Phone-only onboarding | /get-started page | VERIFIED |
| Custom recipes via /kitchen | Homepage CTA | VERIFIED |
