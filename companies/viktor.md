# Viktor.ai — Competitive Intelligence
## Date: 2026-04-20

### Core Value Proposition
"Automate engineering workflows with AI." Platform for engineers to build AI-powered apps, workflows, and agents for engineering disciplines (structural, geotechnical, MEP, process, etc.).

### Key Features
- Python-based app development (200+ building blocks)
- No-code app builder (drag-and-drop) + AI-assisted building
- Engineering software integrations (Autodesk, Bentley, Trimble, Hexagon, Nemetschek)
- Interactive visualizations: 3D models, graphs, maps, reports
- Multi-step user interfaces with pages, tabs, sections
- Data revision control
- Git support & CI/CD pipelines
- Local development capability
- Workflow builder
- Validation Assistant
- OAuth2 and organization-level integrations
- App templates gallery
- Excel-to-App converter
- Batch processing / parametric design

### Pricing
- Free: 1 free user seat, public apps only, community support
- Individual: 1 core user, private apps, integrations, workflow builder, email support (contact for price)
- Small Business: 2 core + 5 basic users, build together, hosting region choice, 7 support hrs/yr
- Business: 5 core + 30 basic users, audit trails, 24 support hrs/yr
- Enterprise: 20+ core + 100+ basic users, SSO, multi-region, custom compute

### Target Audience
Engineering firms (Jacobs, etc.), structural/geotechnical/process engineers, infrastructure designers.

### Tech Stack Signals
- Docs: Docusaurus (v14)
- Frontend: Angular (marketing site)
- Backend: Python SDK (pure Python apps)
- Cloud hosting with region selection

### UX/UI Patterns
- Code-first for builders (Python SDK) but with no-code options
- Web-based app interfaces for end users
- Parametric input forms driving engineering calculations and 3D visualizations
- Git-based version control for developers

### Integration Ecosystem
Deep integrations with engineering software: Autodesk, Bentley, Trimble, Hexagon, Nemetschek.

### Competitive Weaknesses/Gaps
- Extremely niche (engineering-only)
- Requires Python knowledge for serious customization
- European-focused (HQ Rotterdam)
- Pricing not transparent for paid tiers
- Very different market from general no-code automation

### Reverse-Engineering Notes
Viktor shows vertical specialization works but requires code.
To generalize their pattern:
- Vertical templates for any industry (not just engineering)
- No-code first, code optional
- App marketplace for reusable workflows
- Local development + cloud deploy hybrid
