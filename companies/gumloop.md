# Gumloop — Competitive Intelligence
## Date: 2026-04-20

### Core Value Proposition
"AI Automation Framework" — understanding a task should be the only prerequisite to automating it. Team-built specialized agents.

### Key Features
- Pre-built specialized agents: Data Analysis, Support, CRM, Meeting Prep, Call Analysis
- Each agent shows named builders (e.g., "Built by Aron, Katherine, Max")
- Visible reasoning chain with tool calls (e.g., "Querying BigQuery → Building funnel → Chart")
- Credit-based execution system
- Agent marketplace/model where teams share agents
- Unlimited agents and flows (even on Free tier)
- MCP server hosting/proxying (Enterprise)

### Pricing
- Free: 5k credits/mo, 1 seat, 1 active trigger, 2 concurrent runs, 5 concurrent agent interactions
- Pro: $37/mo (20k+ credits), unlimited seats, 5 concurrent runs, 25 concurrent agent interactions
- Enterprise: Custom (RBAC, SCIM/SAML, admin dashboard, audit logs, VPC, workflow queuing, MCP server hosting/proxying)

### Target Audience
Data teams, support teams, sales ops, technical and non-technical users building automations.

### Tech Stack Signals
- Recently raised $50M Series B led by Benchmark
- Uses BigQuery integrations shown in demos
- MCP (Model Context Protocol) server hosting/proxying
- Multi-model support implied
- Customers: Gusto, Instacart, Shopify, Ramp

### UX/UI Patterns
- Visual chat + reasoning transparency — users see tool calls and reasoning steps
- Agent "cards" showcasing use cases with builder attribution
- Interactive demo on homepage showing actual BigQuery analysis conversation
- Clean, modern SaaS aesthetic with purple/blue tones
- Monthly/annual toggle with slider for credit estimation

### Integration Ecosystem
BigQuery, CRM, calendar, support ticket systems. MCP server support indicates broad integration potential.

### Competitive Weaknesses/Gaps
- Credit-based pricing can be unpredictable at scale
- Agent builder attribution suggests complexity
- Enterprise features heavily gated (RBAC, SCIM only on custom tier)
- Brand recognition lower than Lindy
- No clear local/self-host option

### Reverse-Engineering Notes
Gumloop is the strongest no-code automation competitor with visible reasoning chains.
To beat them:
- Flat-rate or usage-transparent pricing (no confusing credits)
- One-click deploy to own infrastructure
- Simpler agent sharing without requiring "builder" expertise
- Native code extensibility (not just no-code)
- Real-time collaboration on workflows
