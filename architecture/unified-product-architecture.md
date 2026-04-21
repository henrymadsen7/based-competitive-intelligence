# Based Agent Platform — Unified Architecture
## Date: 2026-04-20
## Classification: Product Blueprint / Competitive Synthesis

### Philosophy
First principles from Elon Musk: strip every feature to its atomic necessity. Then rebuild with relentless optimization.
Product sense from Steve Jobs: the interface IS the product. Every pixel, every transition, every micro-interaction must feel inevitable.

We are not building "another AI automation tool." We are building the **universal operating system for digital labor**.

---

## Core Thesis
**The future of work is not humans using AI tools. It is humans orchestrating AI workers.**

Every company in our competitive set solves ONE piece of this:
- Lindy: individual delegation
- Gumloop: visual automation
- Relevance: GTM teams
- Pentagon: agent chat rooms
- InsForge: backend infra
- GetModern: IT service desk
- Gojiberry: sales outbound

**Based Agent Platform unifies all of these into one coherent system.**

---

## Architectural Layers

### Layer 0: Design System — "String Theory"
Borrowed and evolved from string-tune.fiddle.digital principles:
- **CSS-first, JS-light:** Animations via CSS transforms and custom properties. JS only for orchestration.
- **60FPS guarantee:** Every scroll, hover, and transition is composited. Zero layout shifts.
- **Attribute-driven:** Behavior activated via HTML data attributes. No JS ceremony.
- **Kinetic typography:** Text that responds to scroll progress, cursor position, and interaction.
- **Scroll progress as state:** `--progress` variable drives animations across the page.
- **Zen minimalism:** Japanese craft aesthetic. "To master the string is to master the code."
- **Dark forest + warm cream palette** from current Based brand, elevated with kinetic motion.

### Layer 1: Conversational Interface — "The Wire"
- **Universal messaging layer:** iMessage, WhatsApp, Slack, Telegram, Email, Web chat, Voice
- **Contextual awareness:** The agent knows what you are working on, what you have delegated, what is pending
- **Voice-first option:** Speak to your agents like a human assistant
- **Thread persistence:** Every conversation is a thread with full history, decisions, and outcomes
- **Smart handoff:** Seamless transition from chat to visual editor to code

### Layer 2: Visual Workflow Engine — "The Loom"
- **Natural language → workflow:** Describe what you want, AI generates the flow
- **Visual canvas:** Drag, drop, connect. But not ugly wiring diagrams — clean, glanceable nodes
- **Code escape hatch:** Every visual flow generates editable Python/TypeScript. One-click open in editor.
- **Real-time collaboration:** Multiple users editing the same workflow with cursors and comments
- **Version control:** Git-native. Branch, merge, diff workflows.
- **Templates:** Start from 100+ pre-built workflows for common tasks

### Layer 3: Agent Runtime — "The Forge"
- **Multi-agent orchestration:** Agents communicate, delegate, and coordinate like a human team
- **Persistent memory:** Every agent remembers context, decisions, failures, and patterns
- **Tool use:** MCP servers, custom APIs, browser automation, code execution, file system access
- **Human-in-the-loop:** Approvals, reviews, escalations at any step. Not bolted on — architected in.
- **Sandboxed execution:** Every agent runs in an isolated environment (VM/container)
- **Observability:** Real-time logs, traces, and cost tracking for every agent run

### Layer 4: Backend Provisioning — "The Anvil"
Every agent project auto-provisions:
- **Postgres database** with schema inferred from agent needs
- **Authentication** (OAuth, SSO, SAML) — configurable in one click
- **File storage** with signed URLs and access controls
- **Serverless functions** for custom logic
- **Realtime sync** for live data updates
- **API gateway** with rate limiting and versioning
- **One-command local dev:** `based dev` spins up the entire stack locally

### Layer 5: Vertical Templates — "The Guilds"
Pre-built agent teams for specific domains:
- **ITSM Guild:** Ticket resolution, access management, onboarding/offboarding (absorbs GetModern)
- **Sales Guild:** Lead enrichment, outbound sequences, demo booking (absorbs Gojiberry)
- **Finance Guild:** Earnings tracking, signal detection, report generation (absorbs Cohesion)
- **Engineering Guild:** Code review, deployment, incident response, documentation
- **Legal Guild:** Contract review, compliance checks, policy enforcement
- **HR Guild:** Recruitment, onboarding, performance tracking
- **Marketing Guild:** Content generation, campaign orchestration, analytics

Each Guild is a deployable template with:
- Pre-trained domain knowledge
- Industry-specific integrations
- Compliance presets (HIPAA, SOC2, GDPR)
- Best-practice workflows

### Layer 6: Trust & Evaluation — "The Prism"
Embedded evaluation framework (absorbs HappyRobots):
- **Automatic benchmarking:** Every agent is scored on accuracy, latency, cost, and safety
- **A/B testing:** Run two agent versions side-by-side with statistical significance
- **Human feedback loops:** One-click thumbs up/down with optional comment
- **Failure-mode library:** Track every failure, categorize it, and auto-suggest fixes
- **Audit trails:** Every action, decision, and data access is logged immutably
- **Compliance reports:** Auto-generate SOC2, GDPR, and HIPAA evidence packs

---

## Technical Stack

### Frontend
- Next.js 15 (App Router, React Server Components)
- TypeScript throughout
- Tailwind CSS + custom design tokens
- String Theory animation system (CSS-first, attribute-driven)
- Real-time collaboration via Yjs + WebRTC
- Monaco editor for code escape hatch

### Backend
- FastAPI (Python) for agent runtime
- LangGraph for multi-agent orchestration
- Postgres + Prisma for data
- Redis for queues and caching
- Temporal.io for durable workflow execution
- Ollama + vLLM for local inference
- LiteLLM proxy for cloud fallback routing

### Infrastructure
- Docker Compose for local dev
- Kubernetes for production
- Terraform for cloud provisioning
- Support AWS, GCP, Azure, and on-prem
- Self-hosted option: one-command install on any Linux box

---

## Pricing Strategy

### Free
- Unlimited personal agents
- 1,000 workflow runs/mo
- Community support
- Local runtime only

### Pro ($29/mo)
- Unlimited agents and workflows
- Team collaboration (up to 5)
- Cloud runtime included
- 10,000 workflow runs/mo
- All integrations
- Standard support

### Team ($99/mo)
- Everything in Pro
- Up to 20 team members
- 100,000 workflow runs/mo
- Custom LLM bring-your-own-key
- SSO and RBAC
- Priority support

### Enterprise (Custom)
- Unlimited everything
- Self-hosted or private cloud
- Dedicated infrastructure
- Custom vertical guilds
- White-glove onboarding
- SLA guarantees

**Why this wins:** Transparent, predictable pricing. No "credits," no "actions," no "vendor fees." Just flat tiers that scale with value.

---

## Differentiation Summary

| Competitor | Their Strength | Our Counter |
|------------|---------------|-------------|
| Lindy | iMessage exec assistant | Multi-platform + visual builder + team sharing |
| Gumloop | Visual reasoning chains | Simpler pricing + code escape hatch + self-host |
| Relay | Easy visual automation | Unlimited steps + multi-agent + backend provisioning |
| Relevance AI | GTM workforce | General purpose + flat pricing + BYO cloud |
| Pentagon | Agent team workspace | Cross-platform + SaaS integrations + visual workflows |
| InsForge | Backend for AI builders | Embedded in agent platform, not separate tool |
| GetModern | AI ITSM | One vertical guild among many + self-serve |
| Gojiberry | LinkedIn outbound | Multi-channel + visual campaign builder |
| Cohesion | Equities research | Template marketplace enables any vertical |
| HappyRobots | Trust/evaluation | Embedded prism layer, not separate product |
