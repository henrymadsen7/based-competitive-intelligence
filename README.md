# Based Competitive Intelligence
**Reverse-engineered deep-dive into the AI agent / no-code automation landscape.**
**Date:** April 20, 2026
**Purpose:** Build something better, simpler, and more beautiful than all of them.

---

## Repo Structure

```
companies/                     # Individual competitive profiles (13 companies)
  lindy.md                     # AI exec assistant via iMessage
  gumloop.md                   # Visual AI automation (Series B, Benchmark)
  relay.md                     # AI-native Zapier alternative
  relevance-ai.md              # AI Workforce for GTM teams
  viktor.md                    # Engineering workflow automation
  cohesion.md                  # YC S26 public equities agent
  happyrobots.md               # AI trust/evaluation platform
  insforge.md                  # Backend PaaS for AI builders (YC)
  getmodern.md                 # AI-native ITSM (YC)
  pentagon.md                  # AI agent team workspace (YC P26)
  gojiberry.md                 # AI outbound sales/LinkedIn
  launchlemonade.md            # NOT A COMPETITOR (marketing workshop)
  poke-ai.md                   # NO ACTIVE PRODUCT FOUND

synthesis/
  comparison-matrix.md         # 11-dimension competitive matrix

architecture/
  unified-product-architecture.md   # The "Based Agent Platform" blueprint

design-reference/
  string-theory-design-system.md    # CSS-first, 60FPS, kinetic typography system
  based-website-integration.md      # How to inject String Theory into based-website
```

---

## The Landscape: 6 Patterns, 10 Players, 1 Gap

### Pattern 1: Conversational Layer
**Leaders:** Lindy (iMessage), Relevance AI (SuperGTM), GetModern (NL workflows)
**Gap:** Every implementation is siloed to one channel. No one does universal messaging.

### Pattern 2: Visual Workflow Builder
**Leaders:** Gumloop, Relay, Viktor
**Gap:** All have credit limits, complexity, and no true code escape hatch.

### Pattern 3: Multi-Agent Team Coordination
**Leaders:** Pentagon (desktop), Relevance AI (web canvas)
**Gap:** Pentagon is macOS-only. Relevance is GTM-only.

### Pattern 4: Vertical Specialization
**Leaders:** Cohesion (finance), GetModern (ITSM), Gojiberry (sales), Viktor (engineering)
**Gap:** Each is its own product. No unified platform with vertical templates.

### Pattern 5: Backend-as-a-Service for AI
**Leader:** InsForge
**Gap:** Backend is separate from agent logic. No embedded provisioning.

### Pattern 6: Trust & Evaluation
**Leader:** HappyRobots
**Gap:** Evaluation is a separate product, not embedded in the agent runtime.

### The Gap Nobody Fills
**No one combines conversational + visual + code + team coordination + vertical templates + embedded backend + trust layer in one platform with transparent pricing and self-hosting.**

That is what we are building.

---

## Based Agent Platform: Unified Architecture

See [`architecture/unified-product-architecture.md`](architecture/unified-product-architecture.md) for the full spec.

### 6 Layers

| Layer | Name | What It Does |
|-------|------|--------------|
| 0 | **String Theory** | CSS-first, 60FPS, kinetic typography design system |
| 1 | **The Wire** | Universal conversational interface (iMessage, Slack, Web, Voice) |
| 2 | **The Loom** | Visual workflow builder with natural language generation and code escape hatch |
| 3 | **The Forge** | Multi-agent runtime with persistent memory, tool use, and sandboxing |
| 4 | **The Anvil** | Auto-provisioned backend per project: Postgres, auth, storage, functions, realtime |
| 5 | **The Guilds** | Vertical agent templates: IT, Sales, Finance, Legal, HR, Engineering, Marketing |
| 6 | **The Prism** | Embedded trust layer: benchmarking, A/B testing, human feedback, audit trails |

### Pricing (Transparent, Predictable)

| Tier | Price | What You Get |
|------|-------|--------------|
| **Free** | $0 | Unlimited personal agents, 1,000 runs/mo, local runtime |
| **Pro** | $29/mo | Unlimited agents, 5 team members, 10,000 runs/mo, cloud runtime |
| **Team** | $99/mo | 20 members, 100,000 runs/mo, BYO LLM, SSO, RBAC |
| **Enterprise** | Custom | Self-hosted, private cloud, custom Guilds, SLA |

**No credits. No action limits. No vendor fees.**

---

## Design System: String Theory

See [`design-reference/string-theory-design-system.md`](design-reference/string-theory-design-system.md) for the full spec.

Inspired by [string-tune.fiddle.digital](https://string-tune.fiddle.digital):
- CSS-first, JS-light animations
- 60FPS guarantee
- Attribute-driven behavior (`data-animate="reveal"`)
- Kinetic typography: text that responds to scroll, cursor, and interaction
- Scroll progress as state (`--progress` variable)
- Zen minimalism with craft precision

See [`design-reference/based-website-integration.md`](design-reference/based-website-integration.md) for how to inject String Theory into the current Based-Website.

---

## How to Use This Repo

### For Product Strategy
Read `synthesis/comparison-matrix.md` to understand where each competitor wins and loses.

### For Feature Prioritization
Read each `companies/*.md` to see what capabilities to absorb, what weaknesses to exploit.

### For Architecture Decisions
Read `architecture/unified-product-architecture.md` for the technical blueprint.

### For Design Direction
Read `design-reference/string-theory-design-system.md` for the visual language.

---

## Research Methodology

1. **Direct site reconnaissance:** Browser-based navigation of every homepage, pricing page, docs hub, and feature page
2. **Open-source intelligence:** Hacker News, Crunchbase, YC directory, GitHub, ProductHunt
3. **Technical signal extraction:** Job postings, tech stack indicators, integration ecosystems
4. **UX pattern documentation:** Visual descriptions of interfaces, workflows, and interaction models
5. **Gap analysis:** First-principles decomposition of what each product does vs. what the market needs

---

## Next Steps

1. [ ] Build String Theory CSS/JS and deploy to Based-Website
2. [ ] Scaffold Based Agent Platform repo (Next.js + FastAPI + LangGraph)
3. [ ] Implement "The Wire" conversational layer (Slack + Web first)
4. [ ] Build "The Loom" visual workflow MVP
5. [ ] Launch with one Guild (ITSM or Sales)
6. [ ] Iterate based on user feedback and competitive moves

---

*Built with first-principles thinking and relentless competitive obsession.*
*For questions or updates, ping Hank.*
