# InsForge — Competitive Intelligence
## Date: 2026-04-20

### Core Value Prop
"The backend for AI-native builders." YC-backed. Go from prompt to production backend in minutes. Coding agent builds the database, wires up auth, and runs it for you.

### Key Features
- Postgres Database for every project
- Cloud Storage (images, files)
- Authentication (OAuth built-in: Google, GitHub)
- Functions (deploy and run backend logic serverless)
- Realtime updates for data sync
- AI Integration (connect and configure AI models)
- Deployment (one-click deploy)
- MCP server setup for all major AI coding agents
- CLI: `npx @insforge/cli create`

### Pricing
- Free: $0/mo — $1 AI credits, 50k MAU, 500MB DB, 5GB bandwidth, 1GB storage. Paused after 1 week inactivity.
- Pro: $25/mo — $10 compute credits included, $10 AI credits/mo then $0.1/credit, 100k MAU then $0.00325/MAU, 8GB DB, 250GB bandwidth, 100GB storage
- Enterprise: Custom — SOC2, HIPAA available, SSO, unlimited projects, dedicated support

### Target Audience
AI-native developers, coding agent users, rapid prototypers.

### Tech Stack Signals
- YC-backed
- 7.6k GitHub stars
- MCP integrations: Cursor, Claude Code, Copilot, Google Antigravity, Codex, Cline, Kiro, Trae, Qoder, Roo Code, Windsurf
- Benchmark claim: 1.6x faster backend tasks vs alternatives

### UX/UI Patterns
- Developer-first, CLI-centric
- Clean docs-heavy site
- Benchmark/performance-focused marketing

### Integration Ecosystem
All major AI coding agents via MCP. Postgres, storage, auth, functions, realtime.

### Competitive Weaknesses/Gaps
- Narrow scope (backend only, not full-stack agents)
- No visual workflow builder
- No multi-agent orchestration
- Credit/usage-based pricing can be unpredictable
- No on-prem/self-hosted option

### Reverse-Engineering Notes
InsForge is a backend PaaS for AI builders, not an agent platform.
To absorb their value:
- Embedded backend-as-a-service inside our agent platform
- One-click database + auth + storage for every agent project
- MCP server auto-generation from agent tools
- Support all major AI coding agents natively
