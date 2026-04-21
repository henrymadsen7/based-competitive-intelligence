# Poke.com — Deep-Dive Competitive Intelligence
## Date: April 20, 2026
## Researcher: Hermes (direct browser reconnaissance)

---

## Executive Summary

**Poke** is an AI SMS assistant built by **Interaction Co.** (interaction.co), based in Palo Alto, California. It operates entirely through text messaging — users sign up with a phone number and interact with Poke via SMS. The product centers on a "recipe" marketplace: pre-built integrations and automations that users activate with one tap.

**Key insight:** Poke is not trying to be a general-purpose AI workspace. It is deliberately narrow: SMS-first, phone-native, recipe-driven. This is both its strength (extreme simplicity, no app download) and its ceiling (SMS is a constrained interface for complex multi-step work).

---

## Company Identity

| Attribute | Detail |
|-----------|--------|
| **Product name** | Poke |
| **Company** | Interaction Co. |
| **Domain** | poke.com |
| **Company site** | interaction.co |
| **Location** | Palo Alto, California |
| **Social** | x.com/interaction |
| **Contact** | hi@interaction.co, poke@interaction.co |
| **Founded** | Unknown (site shows copyright 2026) |
| **Funding** | Not disclosed |
| **Team size** | Unknown (hiring at interaction.co/jobs) |

**Critical correction from previous research:** The company is NOT "poke.ai" or "pokeai.com". It is **poke.com**. The previous session searched for the wrong domain and concluded the company was defunct. This was a TLD assumption error.

---

## Core Value Proposition

> "Say hey to Poke. Ask or get anything done, right from your texts."

Poke's thesis is simplicity through constraint:
- **No app to download** — everything happens in iMessage/SMS
- **No visual builder** — recipes are pre-configured; users just tap "Get Started"
- **No learning curve** — natural language in, results out
- **One-tap setup** — recipes activate instantly

---

## Recipe Marketplace (Integration Ecosystem)

Poke organizes capabilities as "recipes" — pre-built integrations with specific tools or workflows. The marketplace has 20+ recipes across 11 categories.

### Verified Recipes (from direct browser reconnaissance)

**Productivity**
- Todoist — Manage tasks and projects with priorities, labels, and progress tracking
- Linear — Streamline issue tracking, project management, and cycles from your texts
- Notion — Access and organize your pages, databases, and docs from your texts
- Asana — Organize work across projects with task management, tracking, and collaboration
- GitHub — Review pull requests, track issues, and collaborate across repositories
- Granola — Capture meeting notes, summaries, and action items automatically from calls
- Journal — Daily prompts and past reflections
- Weekly Productivity Check-in — Review accomplishments every Friday

**Developer Tools**
- Devin — Start sessions, check progress, and collaborate with the AI software engineer
- Cursor Cloud Agents — Manage Cursor cloud agents
- Vercel — Ship and monitor web apps with deployment insights and build log analysis
- PostHog — Query event data, manage feature flags, and analyze product usage patterns
- Parallel Web Systems — Search the web and extract content from URLs with ranked, LLM-optimized results

**Health & Wellness**
- Oura — Track sleep stages, readiness scores, and daily activity insights
- Fit — Log meals via text and see daily totals, weekly trends, and macro breakdowns
- Hydration Reminders — Friendly water reminders throughout the day
- Strava — Track runs, rides, and workouts with pace, distance, and training insights

**Creative / Media**
- Canva — Design presentations, social posts, and graphics
- Pics — Edit, enhance, and create images right in your texts

**Smart Home**
- Sonos — Control speakers, adjust volume, and manage music playback across rooms
- Philips Hue — Control smart lights, adjust colors, and activate scenes

**Finance / Operations**
- Forward Receipts to Navan — Automatically detect invoices and expense emails and route them to Navan

**Information / Lifestyle**
- Daily Weather — Local forecast with temperature, rain chances, and outfit tips
- Daily Horoscope — Personalized zodiac reading, themes, and guidance
- Bible — Daily scripture passage via text with ability to explore and ask questions
- Nightly Gratitude — Thoughtful reflection prompt every evening

**Students** (category exists, specific recipes not enumerated in this session)

### Recipe Architecture

Each recipe has:
- **Description** — What it does
- **Integrations** — Which APIs/services it connects to
- **Chef** — Author (most are "Poke Team")
- **Tags** — Category filters
- **"Often Used Together"** — Cross-sell suggestions
- **"Create my own"** — Users can build custom recipes at /kitchen

**Custom integrations supported via MCP** (Model Context Protocol). Guide at poke.com/mcp.

---

## Product UI & UX Patterns

### Onboarding Flow
1. User visits poke.com/get-started
2. Enters phone number (country selector + number input)
3. No email required. No password. No download.
4. SMS confirmation presumably follows

### Interaction Model
- **Primary channel:** SMS/iMessage
- **Trigger:** User texts Poke a request
- **Response:** Poke texts back results or confirms actions
- **Recipes:** One-tap activation from web catalog

### Web Interface
- **Homepage:** Single hero with "Say hey to Poke" + two CTAs (Get Started, Explore)
- **Recipes catalog:** Searchable, filterable grid with category tabs (All, Automate, Integrate)
- **Recipe detail:** Minimal — description, integrations, chef, tags, related recipes
- **No dashboard** — the product lives in SMS, not a web app

---

## Pricing

**No pricing page exists.** The /pricing URL returns 404.

The FAQ includes the question: "Can I get a discount on the price set by Poke?"

This implies:
1. Poke has set pricing (not free)
2. Pricing may be per-recipe or subscription-based
3. Pricing is not publicly advertised
4. It may be revealed after signup or through SMS

**Assessment:** Poke is likely in a closed beta or early-access phase where pricing is handled individually or via SMS after onboarding. The absence of a pricing page is notable for a consumer-facing product.

---

## Privacy & Security

Poke's privacy posture is aggressive and well-communicated:

> "By default, your conversations with Poke are as private as your thoughts. When you sign up, we automatically set you to 'Maximum Privacy,' meaning not even we can see your chats. We will **never** change this on your behalf. In this mode, we also **do not** train on user data."

This is a direct competitive differentiator against OpenAI, Claude, and most cloud AI assistants.

---

## Competitive Positioning

### What Poke Does Well
1. **Zero-friction onboarding** — Phone number only, no app download
2. **Privacy-first by default** — "Maximum Privacy" mode, no training on data
3. **Recipe marketplace** — Pre-built integrations reduce setup to one tap
4. **SMS-native** — Meets users where they already are (iMessage)
5. **MCP support** — Extensible for power users without complicating the core product
6. **Warm, approachable brand** — "Say hey to Poke" vs. enterprise jargon

### Where Poke Is Vulnerable
1. **SMS is a ceiling** — Complex multi-step workflows, rich media, and team collaboration are awkward in text messages
2. **No team features visible** — Everything appears individual-user focused
3. **No pricing transparency** — Users cannot evaluate cost before signing up
4. **Limited workflow depth** — Recipes are single-purpose; no chaining, branching, or conditional logic visible
5. **No desktop/web workspace** — For serious work, users still need their actual tools
6. **Enterprise adoption unlikely** — SMS-based access control, audit trails, and compliance are undefined

### The Gap Poke Reveals

Poke proves that users want **instantly useful AI** without configuration burden. But it also proves that SMS is too thin for serious operational work. The whitespace is:

> **A product with Poke's simplicity but Based's depth.** Natural language in, but with a real workspace behind it — multi-step workflows, team collaboration, reviewable output, and controlled access.

---

## Reverse-Engineering Notes

### Tech Stack Signals
- Modern React/Next.js site (based on DOM structure and routing)
- SMS infrastructure likely via Twilio or similar
- MCP support suggests they use an AI orchestration layer that exposes tools via standard protocol
- Recipe marketplace implies a plugin architecture

### Design Patterns
- Clean, minimal aesthetic
- Warm earth tones (browns, creams)
- Card-based recipe grid
- Mobile-first (makes sense for an SMS product)
- Simple iconography for each integration

### What We Can Learn
1. **Recipe model works** — Pre-built, one-tap configurations reduce activation friction dramatically
2. **Privacy as a feature** — Leading with "we can't see your chats" builds trust instantly
3. **SMS as a channel** — There is a segment of users who prefer text over apps
4. **MCP is emerging as standard** — Supporting Model Context Protocol makes integrations extensible without building them all

---

## Verification Log

| Claim | Source | Status |
|-------|--------|--------|
| Poke is at poke.com (not poke.ai) | Direct browser navigation | **VERIFIED** |
| 20+ recipe integrations | Direct browser snapshot of /recipes | **VERIFIED** |
| MCP custom integration support | FAQ expanded content | **VERIFIED** |
| "Maximum Privacy" by default | FAQ expanded content | **VERIFIED** |
| No training on user data | FAQ expanded content | **VERIFIED** |
| No pricing page | Direct navigation to /pricing (404) | **VERIFIED** |
| Parent company is Interaction Co. | Footer links, about redirect | **VERIFIED** |
| Based in Palo Alto | Footer "Designed in Palo Alto" | **VERIFIED** |
| Phone-only onboarding | /get-started page inspection | **VERIFIED** |
| Custom recipes via /kitchen | Homepage CTA + FAQ | **VERIFIED** |

---

## Previous Errors Corrected

1. **Wrong domain:** Previous session searched "poke.ai" and found nothing. Correct domain is **poke.com**.
2. **Defunct conclusion:** Previous session incorrectly concluded Poke AI was defunct. It is actively operated by Interaction Co.
3. **Integration count:** Previous session estimated "15+ recipe integrations." Verified count is **20+** with 11 categories.
4. **Product category:** Previous session had no category. Verified: SMS-native AI assistant with recipe marketplace.
