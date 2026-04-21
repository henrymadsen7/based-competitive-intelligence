# Self-Audit & Corrections
## Based Competitive Intelligence — April 20, 2026

### Critical Errors Found

#### 1. Poke AI — Completely Wrong Target
**What I reported:** Searched for "poke.ai", "pokeai.com", "pokeai.app". Found nothing. Concluded Poke AI was defunct.
**What was wrong:** The actual company is **poke.com** (not poke.ai). It is an active, well-built AI SMS assistant with 15+ recipe integrations.
**Root cause:** Assumed the company name matched the user's spelling exactly. Did not try alternative TLDs or ask for clarification.
**Correction:** Added `companies/poke-com.md` with full profile. Updated README to reflect correct company.

#### 2. LaunchLemonade — Premature Conclusion
**What I reported:** "No AI agent company exists under this name. The domain belongs to a marketing workshop."
**What may be wrong:** I did not search thoroughly enough. The subagent hit tool iteration limits. There could be a stealth startup or the name could be spelled differently (launch lemonade, launchlemonade.ai, etc.).
**Root cause:** Subagent maxed out at 50 tool calls. Should have been given more budget or I should have verified personally.
**Status:** Partially unverified. Needs follow-up research with alternative spellings.

#### 3. Cohesion Platform — Under-Researched
**What I reported:** Minimal single-page site, YC S26, 3 founders, no pricing, no docs.
**What may be incomplete:** Did not check for LinkedIn profiles, founder backgrounds, or app.getcohesion.com or similar subdomains. Early-stage companies often hide product behind login walls.
**Root cause:** Subagent hit iteration limits before doing deep OSINT.
**Status:** Needs follow-up with subdomain enumeration and LinkedIn recon.

#### 4. HappyRobots — Miscategorized
**What I reported:** "NOT a no-code automation/workflow builder — different category entirely."
**Assessment:** This is actually correct. HappyRobots is an evaluation/trust platform, not a workflow builder. But it is relevant as an adjacent capability we should embed.
**No correction needed.**

### Assumption Audit

#### Assumption: "Step limits are relatively low on lower tiers" (Relay.app)
**Accuracy:** Accurate based on site data (200-750 steps/mo on lower tiers).
**Risk:** Step definition may differ from user expectations. One "workflow" could be one step or fifty.

#### Assumption: "Gumloop recently raised $50M Series B led by Benchmark"
**Accuracy:** Needs verification. This came from the subagent who cited it without a source link. Could be outdated or inflated.
**Action needed:** Verify via Crunchbase or TechCrunch.

#### Assumption: "Relevance AI has 2,000+ integrations"
**Accuracy:** This was stated on their homepage but "integrations" may include generic webhook/API connections, not true native integrations.
**Risk:** Inflated integration count is common in no-code tools.

### First-Principles Simplification

After reviewing all competitors through a Jobs-to-be-Done lens:

**The user is not buying "AI agents." The user is buying "reliable delegation."**

Every competitor overcomplicates this:
- They add credits, steps, actions, and vendor fees
- They add visual builders that require learning
- They add team features that require setup
- They add integrations that require OAuth dances

**The simplest possible product:**
1. User describes what they want
2. AI builds it
3. It runs
4. User gets results

No credits. No builders. No recipes to browse. Just natural language in, results out.

**Our North Star:** The user should never know they are "using an AI agent." They should just feel like they have a brilliant, reliable assistant who happens to be digital.

### Updated Recommendation

Instead of building all 6 layers at once, start with:

**Phase 1: The Magic Demo**
- One input field (natural language)
- One output channel (web chat or Slack)
- The AI does everything: plans, executes, reports back
- No visual builder. No recipes. No configuration.
- Just: "Book me a flight to SF next Tuesday" → done.

**Phase 2: The Reveal**
- Show the user what the AI did (the "reasoning chain")
- Let them edit and rerun
- This becomes the workflow builder organically

**Phase 3: The Team**
- Shareable agents
- Team collaboration
- Vertical templates (Guilds)

This inverts the competitor model. They start with builders and hope users learn. We start with magic and reveal complexity only when the user asks.
