# Relay.app — Competitive Intelligence
## Date: 2026-04-20

### Core Value Proposition
"The easiest way to automate with AI." Modern, AI-native alternative to Zapier/Make. Turns plain language into reliable, visual workflows.

### Key Features
- Natural language workflow generation (AI agent builds workflows from description)
- Visual workflow editor with drag-and-drop
- 200+ app integrations
- Multi-step workflows with conditional paths, loops, iterators
- AI steps: data extraction, classification, summarization, translation, audio transcription, TTS, image generation
- Human-in-the-loop: approvals, manual data inputs, tasks, manual path selection
- Flow control: Paths (branching), merging, dynamic waits
- Sequences (reusable sub-workflows)
- Tables (structured data storage for stateful automations)
- MCP Server builder (expose custom tools to ChatGPT, Claude, etc.)
- Webhook triggers & HTTP requests
- Custom JavaScript code execution
- Batch triggers
- Rich text templating
- Run history & inspection

### Pricing
- Free: $0, 1 user, 500 AI credits/mo, 200 steps/mo
- Professional: $19/mo (annual), 1 user, 2,000 AI credits/mo, 750 steps/mo
- Team: $69/mo (annual), 10 users, 2,000 AI credits/mo, 2,000 steps/mo
- Enterprise: Custom usage, SOC2/GDPR, priority support

### Target Audience
Non-technical ops, marketing, sales, and product teams.

### Tech Stack Signals
- React-based marketing site
- GitBook for docs
- Uses HyperDX for monitoring (founder HN comment)
- AI models: GPT, Claude, Gemini integration

### UX/UI Patterns
- Hybrid: natural language chat interface to generate workflows + visual editor for refinement
- Visual workflow builder that "feels nothing like wiring diagrams"
- Not code-first; designed for non-technical users

### Integration Ecosystem
200+ native integrations: CRM (HubSpot, Salesforce), productivity (Notion, Airtable, Google), comms (Slack, Gmail), dev (GitHub), specialized (Apollo, Gong).

### Competitive Weaknesses/Gaps
- Step limits are relatively low on lower tiers (200-750/mo)
- AI credit system may frustrate heavy users
- No on-prem/self-hosted option
- Primarily focused on SaaS integrations, not internal APIs or complex data pipelines
- No true multi-agent team coordination

### Reverse-Engineering Notes
Relay proves "natural language → visual workflow" pattern works.
To beat them:
- Unlimited steps on all tiers (differentiator)
- Self-hosted runners for internal API access
- Multi-agent team orchestration
- Native code blocks with autocomplete
- Better error handling and debugging UI
