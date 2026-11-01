# Trend scout: fast-growing topics for one-day $10-100 digital products (status as of 1 Nov 2026)

Phase 1 research, role: trend-scout. Prepared for the solo-founder "10 one-day digital products" project.

> **Read this first: method problem.** The shared WebSearch budget (200 calls per turn, shared by all agents) was already used up before this agent started, so **this agent ran zero web searches.** Google Trends, Exploding Topics, Glimpse, job boards, subreddit sizes, newsletter counts and funding news could **not** be measured directly. To compensate, this report builds its own primary trend data from sources that stayed reachable:
> 1. **A GitHub repo-creation time series**: 30 topic queries x 8 periods (Q1 2025 to Oct 2026), 240 GitHub search API calls on 1 Nov 2026, with two neutral baselines.
> 2. **The full Y Combinator company directory** (6,361 companies, updated 31 Oct 2026, via [yc-oss/api](https://github.com/yc-oss/api)). Recent batches were classified to see where seed money is going in 2026 vs 2025.
> 3. **Anthropic's official plugin marketplaces** (read as raw JSON) and plugin READMEs and commit history on github.com.
> 4. **Curated "awesome" lists on GitHub**, used for first-party launch links (Google, Bing, Shopify, Etsy). Links taken from these lists are marked "(via list)".
> 5. **Sibling Phase 1 files** (pain-hunter, regulation-and-platform-shifts, marketplace-saturation-scout). Their facts are marked "**relayed**" and were not re-verified here.
>
> GitHub counts measure **builder and supply-side** activity, not small-business buyer demand. High GitHub growth often means **more free competition**, not more buyers. Each entry reads it both ways.

## Executive summary

- **The "skill" packaging format is the strongest growth signal anywhere in this dataset.**
  - Repos mentioning Claude or agent skills went from 70 (Q2+Q3 2025) to 60,038 (Q2+Q3 2026), and October 2026 ran about 1.45x Q3's monthly pace.
  - About 77 of the 366 repos created since 1 May 2026 that already have more than 4,000 stars are skills.
  - Anthropic launched "Claude for Small Business" on 15 Sep 2026 ([PR #1144](https://github.com/anthropics/knowledge-work-plugins/pull/1144)). It is a **free** official plugin with 44 skills and 35 official connectors, including QuickBooks, Xero, Square, Shopify, Wix, Stripe, Gusto and HubSpot.
  - **Implication:** non-technical buyers are now being onboarded to skills, but generic small-business and role packs are being absorbed for free. Only **narrow vertical packs** stay open: trades, dental, therapy, bookkeeping, real estate, and vertical software that the official plugin does not cover.
- **Seeds absorbed by free platform features in 2026:**
  - **Brand voice (7):** an official free Brand Voice plugin from a Cowork launch partner.
  - **SOP-to-agent (10):** Microsoft's free [skill-recorder](https://github.com/microsoft/skill-recorder) (29 Jul 2026) records a work session and outputs a SKILL.md.
  - **MCP connectors for mainstream SMB software (5):** vendors now ship official connectors and plugins.
- **Topics still accelerating on GitHub (Q3/Q2 2026 above 1.3):**
  - agentic commerce (2.20)
  - browser agents (1.69)
  - A2P 10DLC (1.63)
  - e-invoicing (1.51)
  - accessibility (1.49)
  - AI receptionists (1.44)
  - Claude skills (1.36)
  - teacher AI (1.33)
  - LLM evals (1.31)
  - voice agents (1.31)
- **Topics plateauing or cooling:**
  - **EU AI Act:** flat (0.99). YC's "Compliance" tag fell from 13 companies in 2025 batches to 5 in 2026.
  - **School AI policy:** 0.93. YC "Education" fell 14 → 3.
  - **Brand voice:** 0.89.
  - **Vibe coding:** 0.82 in Q3, rebounding in October.
  - **OpenClaw:** peaked in Q1 2026 at 44,750 new repos and fell to 6,513 in Q3, a clear post-hype decline.
  - **Conversational/voice AI at YC:** "Conversational AI" fell 14 → 6 and "AI Assistant" 27 → 15.
- **Where VC money flows toward small buyers in 2026 (YC):**
  - AI front offices for **home-service trades**: about 1-2 companies per batch, e.g. Cactus, CentralComs, Bernard, Fleety.
  - **Small medical, dental and therapy practices**: Patientdesk.ai, Klarify, Kairos Health, Tepali, ClaimGlide. YC's "Healthcare" tag rose 47 → 70.
  - These companies sell SaaS, not templates. They validate the pain and the vertical, and show the buyers are reachable.
- **"Get found by AI" (seed 2) is a real platform shift with crowded tooling.**
  - Search Console added generative-AI performance reports (Jun 2026) and Bing added AI Performance (Feb 2026) (via list).
  - GEO repos are up 18.9x year on year.
  - But at least 29 paid monitoring platforms, several free graders, free GEO skills (one at 8.5k stars) and an "seo-ai-visibility" skill inside Anthropic's free SMB plugin crowd the space.
  - **Opening:** a vertical, plain-English "read your new AI reports and fix your Google Business Profile, reviews and schema" kit. Not monitoring software, and not llms.txt.
- **Job titles, newsletter and community growth, and non-YC funding rounds: no first-hand evidence** (search was unavailable). See "Method & limitations".

## Summary table (ranked by growth strength x relevance to $10-100 one-day products)

Legend:
- **GH yoy** = repos created Q2+Q3 2026 / Q2+Q3 2025. The neutral baselines grew 0.9x ("todo app") and 1.7x ("portfolio website").
- **Mom.** = Q3 2026 / Q2 2026 (baselines 0.86 and 1.11).
- **Reach** = does the growth reach non-technical small buyers yet?
- **Crowd** = crowded, saturated or absorbed?

| Rank | Topic | Seed | Growth signal (headline) | GH yoy / Mom. | Reach (non-tech) | Crowd | Evidence | Date | Lean |
|---|---|---|---|---|---|---|---|---|---|
| 1 | Vertical skill packs and "company context" kits for Claude Cowork and other agents | 1 | Skills repos 70 → 60,038; Claude for Small Business launched 15 Sep 2026; 315 plugins in the official directory | 551x / 1.36 | **Yes, starting** (Cowork + SMB plugin aimed at plain-English owners) | Generic packs **absorbed** (free official plugins); trades, dental, therapy thin | STRONG (growth), MEDIUM (WTP) | Sep-Nov 2026 | **Pursue, narrow verticals only** |
| 2 | "Get found by AI" for local businesses (GBP, reviews, schema, new AI reports) | 2 | GEO repos 18.9x; GSC gen-AI reports (Jun 2026); Bing AI Performance (Feb 2026); YC Theo (F26) | 18.9x / 1.21 | Yes (owners hear about it); WTP unproven | **Crowded** (29+ paid platforms, free graders, free skills) | STRONG (shift), WEAK (WTP) | Feb-Oct 2026 | Pursue re-scoped, vertical and plain-English |
| 3 | AI front office for home-service trades (receptionist, missed call, dispatch) | 6 | AI-receptionist repos 8.8x; 10+ YC trades-AI startups 2025-26 | 8.8x / 1.44 | Owners buy SaaS; **agencies** buy templates | Builder supply saturated; YC conversational-AI cooling | STRONG (vertical), MEDIUM (template WTP) | 2025-Oct 2026 | Pursue as agency-facing per-trade "brain + compliance + test" pack |
| 4 | Accessibility fix kits for Shopify/Wix stores | 4 | Accessibility repos 4.8x and **accelerating**; ADA/EAA pressure (relayed) | 4.8x / 1.49 | Yes (demand letters) | Overlays, apps, free generators; no VC heat | MEDIUM-STRONG | 2026 | Pursue with no-compliance-claim framing |
| 5 | AI admin kits for small medical, dental and therapy practices | (new) | YC clinic/dental/therapy companies 12 → 22; Healthcare tag 47 → 70 | AI-scribe repos only 2.2x / 1.05 | Yes (pain-hunter #1, relayed) | AI scribes plentiful; HIPAA limits | MEDIUM | 2026 | Pursue (no-PHI templates, consent, BAA checklist) |
| 6 | A2P 10DLC / SMS compliance kit | (new) | 10DLC repos 3.3x; Twilio rules from 30 Jun 2026 (relayed) | 3.3x / 1.63 | Yes | Moderate | MEDIUM | Jun-Oct 2026 | Pursue (from regulation sibling) |
| 7 | UK Making Tax Digital records kit | (new) | Live Apr 2026, next wave Apr 2027 (relayed); GitHub tiny but rising | n/a (tiny base) | Yes | Etsy kits exist (relayed) | STRONG (relayed) | 2026 | Pursue (from regulation sibling) |
| 8 | Connector setup guides for vertical software (MCP) | 5 | MCP repos 2.4x on a huge base; October pace up 1.5x | 2.4x / 1.03 | Partly (Cowork users) | **Absorbed** for mainstream SMB tools; vertical gaps | STRONG (growth), WEAK (WTP) | May-Oct 2026 | Bundle only; standalone weak |
| 9 | AI-shopping readiness for Etsy/Shopify sellers (agentic commerce) | (new) | Fastest-accelerating topic: 21 → 2,362 repos; UCP backed by Google, Shopify, Etsy, Target, Walmart (via list) | 40.7x / 2.20 | Indirect (platforms switch it on) | Thin, but platforms automate | MEDIUM (dev), WEAK (seller WTP) | Dec 2025-Oct 2026 | Watch; a cheap checklist at most |
| 10 | Personal-agent skill packs (OpenClaw, DeepSeek Harness registries) | 1 | OpenClaw 393.6k stars; ClawHub registry; DeepSeek Harness 268k stars (Aug 2026) | 342x / **0.26** | Prosumers only | Free; **cooling** after the Q1 2026 spike | MEDIUM | Jan-Oct 2026 | Secondary channel only |
| 11 | Safety and launch kits for non-developers who vibe-code tools | (new) | Vibe-coding repos 3.4x; YC Floracene (S26) | 3.4x / 0.82 (Oct rebound 1.38) | Yes (non-coders shipping tools, relayed) | Free viral skills (Cloudflare security-audit-skill 56k stars) | MEDIUM-WEAK | 2026 | Maybe |
| 12 | E-invoicing (EU) | (new) | E-invoicing repos 6.0x and accelerating (Oct 1.71) | 6.0x / 1.51 | Yes, but they need software | Software vendors | MEDIUM | 2026 | Low fit (relayed) |
| 13 | Teacher AI workflow kits | 9-adj. | Teacher-AI repos 3.3x / 1.33; teacher Claude-skill repos 17 → 61 | 3.3x / 1.33 | Yes | Free skill packs; YC Education 14 → 3 | MEDIUM-WEAK | 2026 | Maybe (TPT unverified) |
| 14 | Chatbot / agent test and QA kits | 8 | LLM-eval repos 6.2x; YC eval startups 6 → 10 | 6.2x / 1.31 | **No** (dev/enterprise) | Dev tools | MEDIUM (dev), WEAK (SMB) | 2026 | Add-on to #3 only |
| 15 | AI acceptable-use policies for small firms | 3/9-adj. | Surveys show no policy (relayed); AI-Act repos plateau | 17.2x / 0.99 | Yes | **Crowded** | MEDIUM | 2026 | Vertical add-on only |
| 16 | Browser / computer-use agents | (new) | 5.7x / 1.69 | 5.7x / 1.69 | No (dev) | n/a | MEDIUM (dev) | 2026 | Ignore for now |
| 17 | n8n / automation templates | (new) | 2.0x (near baseline) | 2.0x / 1.18 | Agencies | **Saturated** (relayed) | STRONG (saturation) | 2026 | Reject |
| 18 | Brand voice packs | 7 | 12.8x on a tiny base; flattening | 12.8x / 0.89 | Yes | **Absorbed** (official free plugin) | STRONG (absorption) | 2026 | Reject standalone |
| 19 | SOP-to-agent converters | 10 | SOP repos 2.7x (near baseline) | 2.7x / 1.11 | Partly | **Absorbed** (Microsoft skill-recorder, book-to-skill, Anthropic plugin builder) | STRONG (absorption) | May-Oct 2026 | Reject converter; vertical SOP libraries maybe |
| 20 | EU AI Act starter packs | 3 | Plateau on GitHub; YC Compliance 13 → 5 | 17.2x / 0.99 | Weak | **Saturated** (relayed) | STRONG (status) | 2026 | Reject |
| 21 | School AI-policy packs | 9 | Plateau; YC Education 14 → 3 | 4.6x / 0.93 | Districts only | Free model policies (relayed) | MEDIUM | 2026 | Reject |
| 22 | llms.txt kits | 2-adj. | Supply still growing (1.28) but no effect; Google says not required (via list) | 3.8x / 1.28 | Yes (hype) | **Saturated**, free | STRONG (counter) | Sep 2026 | Reject as a lever |
| 23 | ChatGPT Apps | (new) | 3.6x on a small base | 3.6x / 1.42 | No | n/a | WEAK | 2026 | Ignore |

---

## Data appendix A: GitHub repo-creation time series (pulled 1 Nov 2026)

**How it was pulled:**
- Method: `gh api search/repositories` with `q="<terms> created:<range>"`, returning `total_count`.
- Matching covers name, description and topics. Counts are fuzzy: GitHub search is loose, spam and AI-generated repos inflate recent periods, and deleted repos deflate old periods.
- **Use ratios, not absolutes.** Two neutral baselines are included.
- "Oct pace vs Q3" = Oct count x 92/31 / Q3 count. Baselines show 0.84-0.94 here, so a value near 0.9 is "flat".

**Query terms:**
- `claude_skills` = "claude skill" OR "claude skills" OR "agent skills" OR "agent skill"
- `claude_plugin` = "claude code plugin" OR "claude plugin" OR "cowork plugin"
- `geo_aeo` = "generative engine optimization" OR "answer engine optimization" OR "ai visibility" OR "ai search visibility"
- `ai_receptionist` = "ai receptionist" OR "voice receptionist" OR "ai phone agent"
- `accessibility` = wcag OR "web accessibility" OR "accessibility checker"
- `agentic_commerce` = "agentic commerce" OR "agent payments" OR "agentic checkout" OR "universal commerce protocol"
- `openclaw` = openclaw OR clawdbot OR moltbot
- `cowork` = "claude cowork" OR "cowork". **Noisy:** this also matches coworking-space projects.
- `sop` = "sop" agent OR "standard operating procedure"
- `ai_school` = "ai policy" school OR "ai literacy" OR "ai in education"
- `teacher_ai` = "lesson plan" OR "teacher assistant" OR "ai grading"
- `ai_scribe` = "ai scribe" OR "clinical notes" OR "therapy notes" OR "progress notes"
- `gbp_local` = "google business profile" OR "local seo"
- `sms_10dlc` = 10dlc OR "a2p"
- `mtd` = "making tax digital"
- `einvoice` = peppol OR "e-invoicing" OR einvoicing
- Others are self-explanatory.

| Topic (query label) | 2025Q1 | 2025Q2 | 2025Q3 | 2025Q4 | 2026Q1 | 2026Q2 | 2026Q3 | 2026Oct | Q2+Q3 2026 vs Q2+Q3 2025 | Q3/Q2 2026 | Oct pace vs Q3 |
|---|---|---|---|---|---|---|---|---|---|---|---|
| baseline_todo | 21,618 | 23,988 | 27,696 | 23,403 | 24,552 | 24,416 | 20,959 | 5,927 | 0.9x | 0.86 | 0.84 |
| baseline_portfolio | 24,750 | 31,158 | 41,187 | 36,805 | 45,812 | 57,511 | 63,887 | 20,249 | 1.7x | 1.11 | 0.94 |
| claude_skills | 30 | 40 | 69 | 1,491 | 15,217 | 25,448 | 34,590 | 16,889 | 550.8x | 1.36 | 1.45 |
| claude_plugin | 5 | 6 | 25 | 1,090 | 5,485 | 7,236 | 7,129 | 5,594 | 463.4x | 0.99 | 2.33 |
| mcp_server | 3,919 | 15,617 | 13,802 | 13,545 | 27,810 | 35,309 | 36,269 | 18,429 | 2.4x | 1.03 | 1.51 |
| llms_txt | 96 | 149 | 189 | 145 | 339 | 569 | 728 | 364 | 3.8x | 1.28 | 1.48 |
| geo_aeo | 5 | 31 | 66 | 112 | 440 | 828 | 1,004 | 461 | 18.9x | 1.21 | 1.36 |
| ai_receptionist | 55 | 79 | 162 | 310 | 596 | 865 | 1,245 | 519 | 8.8x | 1.44 | 1.24 |
| voice_agent | 437 | 1,169 | 1,912 | 2,672 | 3,682 | 4,660 | 6,093 | 2,437 | 3.5x | 1.31 | 1.19 |
| vapi_retell | 228 | 568 | 553 | 489 | 660 | 814 | 890 | 326 | 1.5x | 1.09 | 1.09 |
| accessibility | 241 | 366 | 514 | 642 | 1,179 | 1,686 | 2,508 | 1,088 | 4.8x | 1.49 | 1.29 |
| eu_ai_act | 20 | 42 | 50 | 78 | 431 | 791 | 787 | 261 | 17.2x | 0.99 | 0.98 |
| llm_eval | 341 | 376 | 541 | 727 | 1,306 | 2,450 | 3,200 | 1,303 | 6.2x | 1.31 | 1.21 |
| brand_voice | 5 | 15 | 18 | 45 | 117 | 223 | 199 | 75 | 12.8x | 0.89 | 1.12 |
| sop | 2,005 | 2,424 | 2,677 | 3,169 | 4,479 | 6,524 | 7,271 | 2,868 | 2.7x | 1.11 | 1.17 |
| ai_school | 31 | 58 | 86 | 115 | 238 | 342 | 317 | 124 | 4.6x | 0.93 | 1.16 |
| n8n | 2,551 | 8,645 | 15,964 | 16,764 | 19,024 | 22,615 | 26,679 | 9,041 | 2.0x | 1.18 | 1.01 |
| agentic_commerce | 6 | 15 | 43 | 163 | 575 | 738 | 1,624 | 588 | 40.7x | 2.20 | 1.07 |
| chatgpt_apps | 53 | 66 | 67 | 422 | 210 | 198 | 282 | 119 | 3.6x | 1.42 | 1.25 |
| vibe_coding | 804 | 3,837 | 6,365 | 7,828 | 15,774 | 19,074 | 15,677 | 7,272 | 3.4x | 0.82 | 1.38 |
| agents_md | 7 | 25 | 95 | 196 | 920 | 1,962 | 2,395 | 1,311 | 36.3x | 1.22 | 1.62 |
| gbp_local | 32 | 57 | 89 | 107 | 270 | 716 | 721 | 249 | 9.8x | 1.01 | 1.02 |
| mtd | 0 | 1 | 2 | 3 | 7 | 4 | 11 | 11 | 5.0x | 2.75 | 2.97 |
| sms_10dlc | 31 | 39 | 45 | 38 | 106 | 106 | 173 | 42 | 3.3x | 1.63 | 0.72 |
| openclaw | 29 | 40 | 53 | 99 | 44,750 | 25,344 | 6,513 | 1,867 | 342.5x | 0.26 | 0.85 |
| cowork | 345 | 380 | 411 | 488 | 1,899 | 3,377 | 2,786 | 927 | 7.8x | 0.82 | 0.99 |
| ai_scribe | 73 | 163 | 217 | 266 | 311 | 417 | 438 | 165 | 2.2x | 1.05 | 1.12 |
| teacher_ai | 233 | 209 | 399 | 430 | 572 | 856 | 1,138 | 401 | 3.3x | 1.33 | 1.05 |
| einvoice | 56 | 78 | 95 | 150 | 245 | 416 | 627 | 361 | 6.0x | 1.51 | 1.71 |
| browser_agent | 111 | 168 | 259 | 308 | 605 | 911 | 1,539 | 498 | 5.7x | 1.69 | 0.96 |

**Profession-specific skill repos.** Query "claude skills" "<profession>", same GitHub method. Last 6 months (May-Oct 2026) vs the 6 months before (Nov 2025-Apr 2026):

| Profession term | Nov 2025-Apr 2026 | May-Oct 2026 | Read |
|---|---|---|---|
| legal | 91 | 280 | crowded with free packs |
| shopify | 51 | 136 | crowded |
| real estate | 23 | 73 | filling fast |
| teacher | 17 | 61 | filling |
| bookkeeping | 8 | 43 | filling fast |
| small business | 10 | 43 | filling (plus Anthropic's official plugin) |
| restaurant | 14 | 33 | moderate |
| nonprofit | 6 | 26 | thin-moderate |
| etsy | 1 | 20 | thin but rising |
| insurance | 10 | 16 | thin |
| accountant | 3 | 13 | thin |
| contractor | 5 | 13 | thin |
| dental | 5 | 11 | thin |
| hvac | 3 | 8 | **very thin** |
| plumbing | 1 | 7 | **very thin** |
| therapist | 5 | 3 | **very thin** |

## Data appendix B: Y Combinator batches, 2025 vs 2026

- **Source:** [yc-oss/api](https://github.com/yc-oss/api) `companies/all.json` (raw.githubusercontent.com). The repo was last pushed 1 Nov 2026, and the latest `launched_at` is 31 Oct 2026.
- **Batch sizes:**
  - 2025 batches (W25, Spring 25, S25, F25): 621 companies.
  - 2026 batches (W26, Spring 26, S26, F26): 816 companies.
- **YC self-assigned tags (count 2025 → 2026, share 2025 → 2026):**
  - Education 14 → 3 (2.3% → 0.4%)
  - Compliance 13 → 5 (2.1% → 0.6%)
  - Conversational AI 14 → 6 (2.3% → 0.7%)
  - AI Assistant 27 → 15
  - Sales 29 → 10
  - Generative AI 33 → 19
  - Healthcare 47 → 70 (7.6% → 8.6%)
  - Construction 7 → 15
  - Home Services 3 → 5
  - Insurance 13 → 23
  - Fintech 43 → 85
  - SEO 0 → 2
  - Legal 14 → 14
  - Biggest risers overall: Industrials 64 → 156, Infrastructure 61 → 112, Robotics 27 → 60, Defense 8 → 28
- **Read:** YC's 2026 money moved toward hard tech, fintech and healthcare, and away from horizontal AI assistants, education and compliance. Inside the SMB-facing slice, **trades and small medical practices** keep getting funded.

---

## Detailed entries (ranked)

### 1. Vertical skill packs and "company context" kits for Claude Cowork and other agents (seed 1)

**What's growing:**
- **Skill repo creation exploded after the Agent Skills standard** (Dec 2025, relayed from the regulation file).
  - Quarterly counts: Q4 2025 1,491; Q1 2026 15,217; Q2 25,448; Q3 34,590.
  - October 2026 alone had 16,889, about 1.45x Q3's monthly pace (Appendix A).
  - Claude-plugin repos jumped in October to 5,594 in one month, about 2.3x Q3's monthly pace. This is consistent with the September Small Business launch, but the cause is not proven.
- **Skills now dominate viral GitHub.** About 77 of the 366 repos created since 1 May 2026 with more than 4,000 stars are skills (GitHub search, keyword match, a few false positives). Examples:
  - [ponytail](https://github.com/DietrichGebert/ponytail): 182k stars, created 12 Jun 2026
  - [cloudflare/security-audit-skill](https://github.com/cloudflare/security-audit-skill): 56k, 18 Jun 2026
  - [book-to-skill](https://github.com/virgiliojr94/book-to-skill): 36.7k, 1 May 2026
  - [instagram-agent-skill](https://github.com/Jakeschincariol/instagram-agent-skill): 4.3k, 13 Sep 2026, described as "Thirteen Claude skills that run an Instagram account"
- **The platform is moving to non-developers:**
  - [anthropics/skills](https://github.com/anthropics/skills) has 186.3k stars.
  - [anthropics/knowledge-work-plugins](https://github.com/anthropics/knowledge-work-plugins) has 34.3k stars, described as an "Open source repository of plugins primarily intended for knowledge workers to use in Claude Cowork". The README says "Every component is file-based — markdown and JSON, no code, no infrastructure, no build steps."
  - The `small-business` plugin was first committed on 12 May 2026 and relaunched as **"Claude for Small Business"** on 15 Sep 2026 ([commits](https://github.com/anthropics/knowledge-work-plugins/commits/main/small-business), [PR #1144](https://github.com/anthropics/knowledge-work-plugins/pull/1144)).
  - Its [README](https://raw.githubusercontent.com/anthropics/knowledge-work-plugins/main/small-business/README.md) says it gives Claude "44 skills spanning finance, sales, marketing, operations, and hiring, plus a router that understands plain English" and "You don't need to memorize anything."
- **Official marketplaces are large and growing:**
  - The official plugin directory ([claude-plugins-official marketplace.json](https://raw.githubusercontent.com/anthropics/claude-plugins-official/main/.claude-plugin/marketplace.json)) lists **315 plugins**.
  - The knowledge-work marketplace ([marketplace.json](https://raw.githubusercontent.com/anthropics/knowledge-work-plugins/main/.claude-plugin/marketplace.json)) lists **123**.
  - Both include vertical, profession-specific plugins: `claude-for-financial-advisors` (Anthropic), BlackRock, Vanguard and Zocks advisor plugins, LegalZoom, Amazon Selling Partner, and Intuit QuickBooks.
- **Profession-specific free skill repos roughly tripled in six months** (Appendix A: legal 91 → 280, real estate 23 → 73, bookkeeping 8 → 43). Trades and therapy stay very thin: HVAC 8, plumbing 7, therapist 3.

**Who the small buyers are:**
- Non-developer owners and professionals on Claude paid plans using Cowork.
- Relayed from marketplace-saturation-scout: paid Gumroad kits with ratings exist, e.g. "Claude Code for Designers" at $70 with 42 ratings and "Claude For Lawyers" at $39 with 11 ratings.

**Reaches non-technical buyers?** **Yes, as of Sep 2026.** The official SMB plugin is explicitly plain-English, and Cowork plugins need "no code".

**Cooling or crowded?**
- **Absorption is the main risk.** Free official plugins now cover generic small business, finance, legal, marketing, sales, HR, operations, design, customer support and brand voice.
- Free GitHub supply per profession is tripling.
- Relayed (pain-hunter): generic prompt and skill packs sell poorly, e.g. "$57 in 48 hours" for a Claude pack on Indie Hackers.

**What stays open:**
- **(a) Narrow verticals.** Trades, dental, therapy, bookkeeping and Etsy sellers are thin on GitHub, and the official SMB plugin names no vertical.
- **(b) "Company context" setup kits.** Anthropic's own README says its plugins "are generic starting points. They become much more useful when you customize them for how your company actually works". A $29-49 vertical "fill-in-the-blanks business context + 10 workflows" kit sells exactly that customization.

**Evidence:** STRONG (growth, platform launch: primary sources); MEDIUM (willingness to pay, relayed). **Date:** May-Nov 2026.

### 2. "Get found by AI" for local businesses (seed 2, re-scoped)

**What's growing:**
- GEO/AEO/AI-visibility repos: 36 in H1 2025 → 1,832 in Q2+Q3 2026 (18.9x year on year, momentum 1.21, October 1.36).
- Google Business Profile / local-SEO repos: 9.8x (but flat in Q3).
- **First-party measurement launches (via [estevecastells/awesome-ai-search](https://github.com/estevecastells/awesome-ai-search)):**
  - [Google Search Console generative AI performance reports](https://developers.google.com/search/blog/2026/06/gen-ai-performance-reports) (June 2026), listed as "Reporting for impressions from AI Overviews, AI Mode and generative features in Discover".
  - [Bing Webmaster Tools AI Performance](https://blogs.bing.com/webmaster/February-2026/Introducing-AI-Performance-in-Bing-Webmaster-Tools-Public-Preview) (Feb 2026 public preview).
  - These create **new numbers small-business owners will see and not understand.**
- **YC:**
  - [AthenaHQ](https://www.ycombinator.com/companies/athenahq) and [Wildcard](https://www.ycombinator.com/companies/wildcard) (W25)
  - [Sitefire](https://www.ycombinator.com/companies/sitefire) (W26)
  - [Theo](https://www.ycombinator.com/companies/theo) (F26), the first clearly SMB-focused one: "an AI agent that builds your small business website in minutes, then works on it every week so customers find you, whether they search Google themselves or ask an AI."
- **Relayed (regulation file):**
  - BrightLocal: 45% of US consumers used gen-AI for local recommendations vs 6% a year earlier.
  - AI Mode passed 1B monthly users (I/O 2026).
  - Ask Maps replaced GBP Q&A.
  - Ahrefs: AI Overviews correlate with about 58% lower CTR.

**Who the small buyers are:** local service businesses and the solo marketers or agencies serving them.

**Reaches non-technical buyers?** Awareness yes; paid demand only shown by small $19-39 kits (relayed: Gumroad $19 GEO kit, €39 AEO kit, £39 Payhip kit). No ratings evidence was found.

**Cooling or crowded?** **Crowded at the tool layer:**
- One list names 29 paid AI-visibility monitoring platforms, including Profound, Peec AI, AthenaHQ, Otterly, Semrush AI Visibility Toolkit and Ahrefs Brand Radar.
- Free checkers: [HubSpot AI Search Grader](https://www.hubspot.com/ai-search-grader), [Ahrefs AI Visibility Checker](https://ahrefs.com/ai-visibility-checker), [Am I on AI?](https://amionai.com/) (via list).
- Free skills: [open-seo-mcp-skills](https://github.com/Ryze-AI-Adgent/open-seo-mcp-skills) (8.5k stars, created 29 Aug 2026), described as "Free SEO MCP server + open-source SEO and GEO skills for Claude". The official directory also has a free `searchfit-seo` plugin.
- **Anthropic's own small-business plugin ships a `seo-ai-visibility` skill.**
- YC's "SEO" tag went 0 → 2 only, so VCs are not piling into SMB GEO.

**One-day angle that survives:**
- A vertical, plain-English kit, e.g. "Get recommended by Google Maps and ChatGPT: for HVAC companies".
- It would cover reading the new GSC/Bing AI reports, a GBP attribute checklist, FTC-safe review-request scripts (relayed) and LocalBusiness schema snippets for Wix/Squarespace.
- No llms.txt, no ranking promises.

**Evidence:** STRONG (shift, first-party launches); WEAK (WTP). **Date:** Feb-Oct 2026.

### 3. AI front office for home-service trades: receptionist, missed calls, dispatch (seed 6)

**What's growing:**
- AI-receptionist repos 8.8x year on year, momentum 1.44 (the second-fastest acceleration among SMB topics). Voice-agent repos 3.5x.
- Repos naming Vapi/Retell/Synthflow grew only 1.5x. The **build tooling is maturing**; growth is in applications.
- **YC funds a trades front-office company in almost every batch:**
  - [Hey Telo](https://www.ycombinator.com/companies/hey-telo) (W25, "Voice AI for Home Services")
  - [Cactus](https://www.ycombinator.com/companies/oncactus) (Spring 25): "Every call answered in under 60 seconds, 24/7 qualified and booked directly into Housecall Pro, Jobber, FieldEdge, or ServiceTitan."
  - [Cohesive](https://www.ycombinator.com/companies/cohesive) (Spring 25)
  - [Stormy](https://www.ycombinator.com/companies/stormy), [NOSO LABS](https://www.ycombinator.com/companies/noso-labs) and [Bizzy AI](https://www.ycombinator.com/companies/geo-ai) (S25)
  - [Robby](https://www.ycombinator.com/companies/robby) and [Foreman](https://www.ycombinator.com/companies/foreman) (W26)
  - [CentralComs](https://www.ycombinator.com/companies/centralcoms) (Spring 26): "AI agents that answer every call, route each job to the right technician, and keep the calendar full."
  - [Bernard](https://www.ycombinator.com/companies/bernard) (S26)
  - [Fleety](https://www.ycombinator.com/companies/fleety) (F26), an AI dispatcher for plumbing and HVAC
- **Platform:** a Synthflow plugin (hosted MCP plus voice-agent skills) is listed in both official Claude marketplaces.
- **Relayed (pain-hunter #3):** missed calls are a constant pain in r/AiForSmallBusiness, and one contractor pays about $450/month for an answering stack.

**Who the small buyers are:**
- **Owners buy SaaS**, not templates.
- The realistic $10-100 buyer is the **AI automation freelancer or agency** building receptionists for trades, plus a few tech-comfortable owners on Vapi/Retell/Synthflow.

**Reaches non-technical buyers?** The pain does; template products mostly do not. This is an inference: no evidence was found of owners buying templates.

**Cooling or crowded?**
- At YC, "Conversational AI" fell 14 → 6 and "AI Assistant" 27 → 15 (2025 → 2026 batches). My crude "voice receptionist" match fell from 24 to 14 companies, which points to VC consolidation.
- Relayed: builder supply is saturated, with 3,426 "ai receptionist" repos created in 2026 per the regulation file.
- Relayed skeptic: owners want fewer dropped leads, not an "AI receptionist" category.

**One-day angle:**
- A per-trade "receptionist brain" pack: call flows, emergency triage rules, FAQ knowledge base, booking rules for Jobber/Housecall Pro, state disclosure and consent scripts (relayed), and 30 pre-launch test calls.
- Importable into Vapi, Retell and Synthflow; sold to agencies at $29-79.

**Evidence:** STRONG (vertical funding, pain); MEDIUM-WEAK (template WTP). **Date:** 2025-Oct 2026.

### 4. Accessibility fix kits for Shopify and Wix stores (seed 4)

**What's growing:**
- WCAG/accessibility repos: 607 in H1 2025 → 4,194 in Q2+Q3 2026 (4.8x), and **still accelerating** (momentum 1.49, October 1.29).
- Relayed (regulation file): about 2,045 ADA web suits in H1 2026, 79% against e-commerce (UsableNet), plus early EAA enforcement in FR, SE, NL and DE.

**Platform signals:**
- Shopify's official `liquid-skills` plugin in the Claude directory covers "Liquid language fundamentals, CSS/JS/HTML coding standards, and WCAG accessibility patterns for Shopify themes". It is developer-oriented.
- Anthropic's `design` plugin includes "accessibility audits".

**VC heat:** essentially none. The 2025-2026 YC batches contain no accessibility-compliance startup; the one F26 match is a mobile-app testing tool. Fewer funded incumbents is good for a small product, but it may also mean a small software market.

**Who the small buyers are:** Shopify, Wix and Squarespace store owners who received a demand letter or fear one; EU shops above the micro-enterprise threshold.

**Reaches non-technical buyers?** Yes, through lawsuits and letters (relayed).

**Cooling or crowded?** Overlays and apps, free statement generators (relayed), and fast-growing free AI accessibility checkers on GitHub. Liability: FTC's $1M order against accessiBe (relayed), so **never claim compliance.**

**One-day angle:** a platform-specific manual-fix checklist (theme settings, alt text, contrast, form labels), an accessibility statement template, and "you got a demand letter: first 7 days" steps.

**Evidence:** MEDIUM-STRONG. **Date:** 2026.

### 5. AI admin kits for small medical, dental and therapy practices (new)

**What's growing:**
- My crude YC match for clinic/dental/therapy companies went from 12 (2025 batches) to 22 (2026 batches), and YC's "Healthcare" tag from 47 to 70. Examples:
  - [Patientdesk.ai](https://www.ycombinator.com/companies/patientdeskai) (W26, "AI front & back office agent for dental practices")
  - [ClaimGlide](https://www.ycombinator.com/companies/claimglide) (W26, prior-auths for private practices)
  - [Tepali](https://www.ycombinator.com/companies/tepali) (W26, AI EMR for medspas)
  - [Klarify](https://www.ycombinator.com/companies/klarify) (Spring 26, "AI Agent for Therapists")
  - [Plena Health](https://www.ycombinator.com/companies/plena-health) (Spring 26)
  - [Kairos Health](https://www.ycombinator.com/companies/kairos-health) (F26, "AI front desk that fills every chair for dental practices")
- GitHub AI-scribe/clinical-notes repos grew only 2.2x (momentum 1.05), near baseline. Builders are not flooding this niche, maybe because of HIPAA.
- Relayed (pain-hunter #1): therapists' progress notes eat evenings, and SimplePractice's AI note add-on costs about $35/clinician/month.

**Who the small buyers are:** solo therapists, small dental offices, med spas, chiropractors.

**Reaches non-technical buyers?** Yes (relayed Reddit evidence).

**Cooling or crowded?** Many AI scribes and front-desk SaaS products. HIPAA and BAA constraints limit what a template may do.

**One-day angle:** a no-PHI note-template and phrase-bank kit; client AI-use consent and disclosure forms; an AI-vendor/BAA questionnaire; a front-desk call script pack.

**Evidence:** MEDIUM (YC primary data plus relayed pain). **Date:** 2026.

### 6. A2P 10DLC / SMS compliance kit (new; regulation-driven)

**What's growing:**
- 10DLC/A2P repos 3.3x year on year, momentum 1.63. October dropped (0.72), and the base is small (173 in Q3).
- Relayed (regulation file): Twilio made privacy-policy and terms URLs mandatory for new campaigns from 30 Jun 2026; registration rejections block small senders.

**Buyers and reach:** US SMBs and GoHighLevel/Twilio agencies. Reach is yes.

**Crowded?** Moderate (relayed). The guaranteed-approval claims on Fiverr show both demand and claims risk.

**Evidence:** MEDIUM (GitHub is a thin signal; status relayed). **Date:** Jun-Oct 2026.

### 7. UK Making Tax Digital records kit (new; regulation-driven)

**What's growing:**
- GitHub is too small to read: 1 → 15 repos, though October's 11 matched all of Q3.
- Relayed (regulation file): MTD ITSA has been live since Apr 2026 for income over £50k. About 1 million more sole traders and landlords join in Apr 2027.

**Buyers and reach:** sole traders and landlords. Reach is yes.

**Crowded?** Etsy sheets exist and NRLA offers a free bridging template (relayed). Never claim HMRC recognition.

**Evidence:** STRONG (relayed). Included here because the next wave is 5 months away, a clean growth driver.

### 8. Connector setup guides for vertical business software (seed 5)

**What's growing:**
- MCP-server repos: 19,536 in H1 2025 → 71,578 in Q2+Q3 2026, with October at 1.5x Q3's monthly pace.
- YC MCP-related companies 10 → 17, e.g. [Pomerado](https://www.ycombinator.com/companies/pomerado) (F26, "Turn any website into an MCP for your agents, in minutes").

**Absorbed for mainstream SMB tools:**
- The official small-business plugin's [.mcp.json](https://raw.githubusercontent.com/anthropics/knowledge-work-plugins/main/small-business/.mcp.json) ships **35 remote connectors**. They include intuit-quickbooks, xero, myob, zoho-books, square, shopify, stripe, paypal, wix, gusto, hubspot, intuit-mailchimp, canva, notion, docusign, expensify, ramp, monday-com and zapier.
- Vendors ship official plugins: Intuit QuickBooks, Amazon Selling Partner, HubSpot Sales, Wingspan, Hostinger, monday.
- The Zapier plugin advertises "Connect 8,000+ apps to your AI workflow."

**What is not in that list (inferred from absence):** field-service and practice-management software such as Jobber, ServiceTitan, Housecall Pro, Clio, SimplePractice, Dentrix, Vagaro and Mindbody. Relayed: Dentrix, Dubsado, Vagaro and Podia have 0 MCP repos.

**Buyers and reach:** Cowork users in those verticals, so partial reach.

**Cooling or crowded?** The long tail is getting covered through Zapier and vendors. Building a real connector is not a non-technical $10-100 product.

**One-day angle:** "Connect Claude to your [Jobber/Clio] via Zapier: step-by-step plus 15 workflows", as a bundle inside entry #1. Shelf life is short.

**Evidence:** STRONG (growth, absorption: primary); WEAK (WTP). **Date:** May-Oct 2026.

### 9. AI-shopping readiness for Etsy and Shopify sellers (agentic commerce, new)

**What's growing:**
- **Fastest acceleration in the dataset:** 21 repos in H1 2025 → 2,362 in Q2+Q3 2026, with Q3/Q2 at 2.20.
- The [UCP spec repo](https://github.com/Universal-Commerce-Protocol/ucp) was created 31 Dec 2025 (3.5k stars). The [awesome-ucp list](https://github.com/Upsonic/awesome-ucp) names Google, Shopify, Etsy, Wayfair, Target and Walmart, and links:
  - [Google UCP merchant docs](https://developers.google.com/merchant/ucp)
  - Etsy's partnership with Google ([Etsy news](https://www.etsy.com/news/etsy-partners-with-google-on-ai-powered-shopping))
  - Shopify's agentic commerce announcement ([Shopify news](https://www.shopify.com/news/ai-commerce-at-scale))
  - Target's Jan 2026 fact sheet ([Target](https://corporate.target.com/press/fact-sheet/2026/01/google-gemini-2026))
- The [ACP repo](https://github.com/agentic-commerce-protocol/agentic-commerce-protocol) dates from 29 Sep 2025.
- **YC:** [Agentcard](https://www.ycombinator.com/companies/agentcard) (S26, "let agents buy anything online"), [ORO AI](https://www.ycombinator.com/companies/oro-ai) (F26, evals for agentic commerce), [Wildcard](https://www.ycombinator.com/companies/wildcard) (W25, AEO for e-commerce).

**Reaches non-technical buyers?** Only indirectly: Etsy and Shopify turn it on at platform level.

**Cooling or crowded?** Relayed: ChatGPT Instant Checkout was reportedly retired in Mar 2026 (conflicting). Platforms automate the plumbing.

**Possible product:** a $15-25 "make your listings AI-shopping-ready" checklist (titles, attributes, GTINs, policies, reviews). Demand is unproven.

**Evidence:** MEDIUM (dev growth, primary platform links via list); WEAK (seller WTP). **Date:** Dec 2025-Oct 2026.

### 10. Personal-agent skill packs (OpenClaw, DeepSeek Harness registries)

**What's growing:**
- [OpenClaw](https://github.com/openclaw/openclaw) has 393.6k stars. On npm, `openclaw` was created 29 Jan 2026 and has 290 versions.
- [ClawHub](https://github.com/openclaw/clawhub) ("Skill + Plugin Registry for OpenClaw") has 9.5k stars.
- [DeepSeek Harness](https://github.com/deepseek-ai/deepseek-harness) (created 13 Aug 2026, 268k stars) is billed as "Everything is a Plugin". Skills are now portable across agent hosts.

**Cooling:** GitHub repos mentioning OpenClaw/Clawdbot/Moltbot went 44,750 (Q1 2026) → 25,344 (Q2) → 6,513 (Q3) → 1,867 (Oct). This is a textbook post-hype decline.

**Buyers and reach:** prosumers and solo founders. Install is terminal or Node-based, so non-technical reach is low.

**Crowded?** Relayed: Claw Mart sells skills at about $9.

**Lean:** use as a secondary distribution channel for entry #1 packs, not a niche.

**Evidence:** MEDIUM. **Date:** Jan-Oct 2026.

### 11. Safety and launch kits for non-developers who vibe-code tools (new)

**What's growing:**
- Vibe-coding repos 3.4x year on year. Q3 dipped (0.82), then October rebounded (1.38).
- YC [Floracene](https://www.ycombinator.com/companies/floracene) (S26): "Vibecode + deploy HIPAA-compliant internal tools, no eng team needed".
- Relayed (pain-hunter): r/ClaudeAI non-coders ship internal business tools.

**Crowded?** Free viral skills: [cloudflare/security-audit-skill](https://github.com/cloudflare/security-audit-skill) (56k stars), [unslop](https://github.com/heydamir/unslop), [anti-slop](https://github.com/miqdadbadjuber/anti-slop).

**Lean:** maybe, as a "before you share your vibe-coded tool with clients" checklist for owners (data, auth, backups). WTP is unknown.

**Evidence:** MEDIUM-WEAK. **Date:** 2026.

### 12. EU e-invoicing (new)

**What's growing:** e-invoicing/Peppol repos 6.0x year on year and accelerating (Q3/Q2 1.51, October 1.71). This fits the French reception mandate from 1 Sep 2026 (relayed).

**Fit:** low. Buyers need software, and guides must be local-language (relayed).

**Evidence:** MEDIUM. **Lean:** drop for this founder.

### 13. Teacher AI workflow kits (adjacent to seed 9)

**What's growing:**
- Lesson-plan / teacher-assistant / AI-grading repos 3.3x, momentum 1.33.
- Teacher-specific Claude-skill repos 17 → 61 in six months.

**Cooling:**
- YC "Education" tag fell 14 → 3 (2025 → 2026 batches).
- Relayed: a free 165-skill teacher pack (education-agent-skills).
- Relayed pain-hunter: report-card comments and grading are constant teacher pains.

**Unverified:** TPT demand could not be measured.

**Evidence:** MEDIUM-WEAK. **Lean:** maybe, as narrow TPT products (report-card comment banks with an AI workflow), not policy packs.

### 14. Chatbot and agent test/QA kits (seed 8)

**What's growing:**
- LLM-eval repos 6.2x year on year, momentum 1.31.
- YC eval and testing startups rose from 6 to 10 (crude count): [Roark](https://www.ycombinator.com/companies/roark) (W25, "Test, monitor, and improve your voice agents"), [Confident AI](https://www.ycombinator.com/companies/confident-ai) (W25), [Hue](https://www.ycombinator.com/companies/hue) (F26), [Rystic](https://www.ycombinator.com/companies/rystic) (F26).

**Reach:** **No.** This is developer and enterprise demand.

**Lean:** a "30 test calls before you go live" sheet inside entry #3, not standalone. Relayed: only 2 free repos and no paid listings exist.

**Evidence:** MEDIUM (dev), WEAK (SMB).

### 15. AI acceptable-use policies for small firms (adjacent to seeds 3 and 9)

**Signals:**
- Relayed pain-hunter: Clio 2026 found that 57% of solo law firms have no AI policy; Bluevine reports trust barriers.
- On GitHub, the AI-Act/compliance queries plateaued in Q3 2026 (0.99).
- YC "Compliance" fell 13 → 5.

**Crowded:** relayed saturation (one Gumroad catalogue has 59 policy-tagged products; Etsy kits).

**Lean:** sell only as a vertical add-on (therapy, solo law, bookkeeping).

**Evidence:** MEDIUM.

### 16. Browser and computer-use agents (new)

**Signals:** 5.7x year on year, Q3/Q2 1.69 (Oct 0.96). Examples: [browser-use](https://github.com/browser-use) has an official Claude plugin; Google released ARTEMIS for Android automation (GitHub, Aug 2026).

**Lean:** developer-only for now. **Evidence:** MEDIUM (dev).

### 17. n8n and automation templates

**Signals:** 2.0x year on year, roughly the baseline. Relayed: saturated by free libraries (Zie619/n8n-workflows, 57k stars).

**Lean:** reject. **Evidence:** STRONG (saturation, relayed).

### 18. Brand voice packs (seed 7)

**Signals:**
- 12.8x on a tiny base (20 → 422) and flattening (Q3/Q2 0.89).
- **Absorbed:** the official free [Brand Voice plugin](https://raw.githubusercontent.com/anthropics/knowledge-work-plugins/main/partner-built/brand-voice/README.md) by Tribe AI was "Built as a Cowork launch partner". It discovers voice from Notion, Confluence, Drive, Gong and others, then generates and enforces guidelines.
- The SMB plugin includes `brand-style`.
- Viral free "de-AI tone" skills: [lieflat-less-ai-tone](https://github.com/larashero3-dotcom/lieflat-less-ai-tone) (4.7k stars), [anti-slop](https://github.com/miqdadbadjuber/anti-slop).
- YC [Rainbrand](https://www.ycombinator.com/companies/rainbrand) (Spring 26, "The brand layer for agents").
- Relayed price anchor: $9.

**Lean:** reject standalone. **Evidence:** STRONG (absorption).

### 19. SOP-to-agent converters (seed 10)

**Signals:**
- SOP repos 2.7x (near baseline).
- **Absorbed:**
  - [microsoft/skill-recorder](https://github.com/microsoft/skill-recorder) (created 29 Jul 2026, 5.6k stars): "Record yourself doing a task once, then turn it into a skill your AI agent can repeat."
  - [book-to-skill](https://github.com/virgiliojr94/book-to-skill) (36.7k stars) converts PDFs to skills.
  - Anthropic's `cowork-plugin-management` creates and customizes plugins.
  - The SMB plugin has `build-agent` and `build-connector` skills.

**Lean:** reject the converter. A vertical, pre-written SOP library delivered as skills ("12 front-office SOPs for a dental office") folds into entry #1.

**Evidence:** STRONG (absorption).

### 20. EU AI Act starter packs (seed 3)

**Signals:**
- GitHub surged in early 2026, then plateaued: 787 in Q3 vs 791 in Q2, with October flat.
- YC Compliance 13 → 5.
- Relayed: Art. 4 was softened with no EU fine, and the market is saturated (one seller has 29 products; Etsy kits from $12.99).

**Lean:** reject. **Evidence:** STRONG (relayed status, primary GitHub plateau).

### 21. School AI-policy packs (seed 9)

**Signals:**
- Plateau (Q3/Q2 0.93); YC Education 14 → 3.
- Relayed: district mandates are met with free state model policies, and no mandate for tutoring centres was found.

**Lean:** reject. **Evidence:** MEDIUM.

### 22. llms.txt kits (hype trap within seed 2)

**Signals:**
- Supply is still growing (3.8x, momentum 1.28).
- Google's guidance, as summarised in the list, says Google Search "does not require special AI markup or `llms.txt`" ([Google guide](https://developers.google.com/search/docs/fundamentals/ai-optimization-guide), via list).
- A Sep 2026 census found "11.8% serve the file" ([stackscan](https://www.stackscan.com/blog/llms-txt-statistics), via list).
- Relayed: AI crawlers barely request it.

**Lean:** reject as a selling point. **Evidence:** STRONG (counter).

### 23. ChatGPT Apps

**Signals:** 3.6x on a small base. Relayed: no in-ChatGPT sale of digital goods.

**Lean:** ignore (developer-only, no selling channel). **Evidence:** WEAK.

---

## Seed hypotheses: trend-lens verdicts

| # | Seed | Growth signal | Absorption / crowding | Verdict |
|---|---|---|---|---|
| 1 | Skill packs for non-dev professions | Strongest in dataset; platform now targets SMB owners | Generic SMB/role packs absorbed by free official plugins; trades, dental, therapy thin | **Support, narrowly vertical + "company context" setup** |
| 2 | Get-found-by-AI kits | Strong (GSC/Bing AI reports; GEO 18.9x) | Tooling crowded; free graders and skills; SMB plugin has `seo-ai-visibility` | **Support, re-scoped** (vertical, plain-English, GBP/reviews/schema; no llms.txt) |
| 3 | EU AI Act packs | Plateau | Saturated | **Reject** |
| 4 | Accessibility fix kits | Accelerating (1.49) | Overlays, free generators | **Support** (careful claims) |
| 5 | MCP connectors / guides | Strong growth | Mainstream SMB tools absorbed (35 official connectors) | **Weak**: bundle-only guides for vertical software |
| 6 | Voice receptionist templates | Strong vertical (YC trades) | Builder supply saturated; VC conversational-AI cooling | **Support for agency buyers**, per trade, with compliance + test scripts |
| 7 | Brand voice packs | Flattening | Absorbed (official plugin) | **Reject** |
| 8 | Chatbot QA kits | Dev-only growth | n/a | **Add-on only** |
| 9 | School AI policy packs | Plateau; YC Education down | Free model policies | **Reject** |
| 10 | SOP-to-agent converters | Near baseline | Absorbed (Microsoft, Anthropic) | **Reject** converter |

**New candidates this lens adds:** AI admin kits for small practices (#5); AI-shopping readiness for Etsy/Shopify (#9, watch). The regulation-driven A2P 10DLC and MTD kits (#6, #7) are reinforced by GitHub momentum.

## Method & limitations

- **No web searches were possible** (shared budget exhausted before this agent started). WebFetch worked only for github.com. curl worked only for raw.githubusercontent.com, api.github.com search, and registry.npmjs.org. **api.github.com/repos/** endpoints for repos not attached to the session were refused, so star histories could not be pulled. Wikimedia pageviews and npm download stats were unreachable.
- **Not measured at all:** Google Trends, Exploding Topics, Glimpse, Ahrefs/Semrush keyword volumes, job-title counts (e.g. "GEO specialist", "AI automation specialist"), subreddit/Skool/Discord sizes, newsletter subscribers, and non-YC funding rounds (e.g. Profound, Peec AI). **No evidence found** for these in this run; the lead should get them from a session with search budget.
- **GitHub time series caveats:**
  - Counts come from loose keyword search across name, description and topics. Common words cause false positives (`cowork`, `sop`, `skills`).
  - AI-generated and spam repos inflate recent periods. Use the two baselines: anything under about 2x year on year is not meaningful growth.
  - GitHub activity is builder and supply-side. It indicates platform adoption and free competition, **not** small-business buyer demand.
- **YC dataset caveats:** categories came from regex matching on one-liners, descriptions and tags, then were hand-checked on samples. Counts are approximate (examples printed and cited). YC is one accelerator, about $500k cheques, so it is a proxy for where early-stage money goes, not the whole funding market.
- **Pages were mostly not opened directly.** Official Google, Bing, Shopify, Etsy and Target links are cited "(via list)": they appeared in GitHub awesome-list READMEs and were not opened. Sibling facts are "relayed" and not re-verified.
- Star counts shown on GitHub pages and in search results were read on 1 Nov 2026. Some very high counts on new repos (e.g. 182k in 4 months) may include inorganic stars.

## Sources

**GitHub search API (time series, top-repo lists).** Queried 1 Nov 2026 via `gh api search/repositories`; repos cited from those results:
- https://github.com/DietrichGebert/ponytail
- https://github.com/cloudflare/security-audit-skill
- https://github.com/virgiliojr94/book-to-skill
- https://github.com/Ryze-AI-Adgent/open-seo-mcp-skills
- https://github.com/miqdadbadjuber/anti-slop
- https://github.com/heydamir/unslop
- https://github.com/larashero3-dotcom/lieflat-less-ai-tone
- https://github.com/Jakeschincariol/instagram-agent-skill
- https://github.com/microsoft/skill-recorder
- https://github.com/deepseek-ai/deepseek-harness
- https://github.com/Universal-Commerce-Protocol/ucp
- https://github.com/agentic-commerce-protocol/agentic-commerce-protocol
- https://github.com/Upsonic/awesome-ucp
- https://github.com/estevecastells/awesome-ai-search
- https://github.com/yc-oss/api

**Anthropic platform (primary):**
- https://github.com/anthropics/skills
- https://github.com/anthropics/knowledge-work-plugins
- https://github.com/anthropics/knowledge-work-plugins/tree/main/small-business
- https://github.com/anthropics/knowledge-work-plugins/tree/main/partner-built
- https://github.com/anthropics/knowledge-work-plugins/commits/main/small-business
- https://github.com/anthropics/knowledge-work-plugins/commits/main
- https://github.com/anthropics/knowledge-work-plugins/pull/1144
- https://raw.githubusercontent.com/anthropics/knowledge-work-plugins/main/small-business/.mcp.json
- https://raw.githubusercontent.com/anthropics/knowledge-work-plugins/main/small-business/README.md
- https://raw.githubusercontent.com/anthropics/knowledge-work-plugins/main/partner-built/brand-voice/README.md
- https://raw.githubusercontent.com/anthropics/knowledge-work-plugins/main/.claude-plugin/marketplace.json
- https://raw.githubusercontent.com/anthropics/claude-plugins-official/main/.claude-plugin/marketplace.json

**Other GitHub / npm:**
- https://github.com/openclaw/openclaw
- https://github.com/openclaw/clawhub
- https://github.com/AnswerDotAI/llms-txt
- https://registry.npmjs.org/openclaw
- https://registry.npmjs.org/clawhub
- https://registry.npmjs.org/skills
- https://raw.githubusercontent.com/yc-oss/api/main/companies/all.json
- https://raw.githubusercontent.com/Upsonic/awesome-ucp/master/README.md
- https://raw.githubusercontent.com/estevecastells/awesome-ai-search/main/README.md (also read: luka2chat/awesome-geo, izak-fisher/generative-engine-optimization-tools, tentenco/awesome-geo, aldegad/awesome-geo READMEs; no funding data found in them)
- https://github.com/sujeito-operator/gumroad-market-data (sales rescan inspected; not used for conclusions)

**YC company pages (from the yc-oss dataset):**
- Trades and home services:
  - https://www.ycombinator.com/companies/hey-telo
  - https://www.ycombinator.com/companies/oncactus
  - https://www.ycombinator.com/companies/cohesive
  - https://www.ycombinator.com/companies/stormy
  - https://www.ycombinator.com/companies/noso-labs
  - https://www.ycombinator.com/companies/geo-ai
  - https://www.ycombinator.com/companies/robby
  - https://www.ycombinator.com/companies/foreman
  - https://www.ycombinator.com/companies/centralcoms
  - https://www.ycombinator.com/companies/bernard
  - https://www.ycombinator.com/companies/fleety
- Medical, dental and therapy practices:
  - https://www.ycombinator.com/companies/patientdeskai
  - https://www.ycombinator.com/companies/claimglide
  - https://www.ycombinator.com/companies/tepali
  - https://www.ycombinator.com/companies/klarify
  - https://www.ycombinator.com/companies/plena-health
  - https://www.ycombinator.com/companies/kairos-health
- AI search and brand:
  - https://www.ycombinator.com/companies/athenahq
  - https://www.ycombinator.com/companies/wildcard
  - https://www.ycombinator.com/companies/sitefire
  - https://www.ycombinator.com/companies/theo
  - https://www.ycombinator.com/companies/rainbrand
- Agents, evals and commerce:
  - https://www.ycombinator.com/companies/pomerado
  - https://www.ycombinator.com/companies/agentcard
  - https://www.ycombinator.com/companies/oro-ai
  - https://www.ycombinator.com/companies/roark
  - https://www.ycombinator.com/companies/confident-ai
  - https://www.ycombinator.com/companies/hue
  - https://www.ycombinator.com/companies/rystic
  - https://www.ycombinator.com/companies/floracene

**First-party links seen inside GitHub lists (not opened, "via list"):**
- https://developers.google.com/search/blog/2026/06/gen-ai-performance-reports
- https://blogs.bing.com/webmaster/February-2026/Introducing-AI-Performance-in-Bing-Webmaster-Tools-Public-Preview
- https://developers.google.com/search/docs/fundamentals/ai-optimization-guide
- https://www.stackscan.com/blog/llms-txt-statistics
- https://www.hubspot.com/ai-search-grader
- https://ahrefs.com/ai-visibility-checker
- https://amionai.com/
- https://developers.google.com/merchant/ucp
- https://www.etsy.com/news/etsy-partners-with-google-on-ai-powered-shopping
- https://www.shopify.com/news/ai-commerce-at-scale
- https://corporate.target.com/press/fact-sheet/2026/01/google-gemini-2026

**Relayed from sibling Phase 1 files (not re-verified; see those files for full citations):**
- /home/user/Claude-research/research/phase1/regulation-and-platform-shifts.md: ADA/EAA lawsuit counts, MTD ITSA, Twilio 10DLC, AI-search statistics (BrightLocal, Ahrefs, I/O 2026), EU AI Act Omnibus, school AI mandates, Agent Skills standard date, ChatGPT Apps and Instant Checkout status
- /home/user/Claude-research/research/phase1/pain-hunter.md: missed-call pain, Goldman Sachs survey, r/AiForSmallBusiness, therapists' notes, Clio/Bluevine AI-policy surveys, Indie Hackers sales anecdotes
- /home/user/Claude-research/research/phase1/marketplace-saturation-scout.md: Gumroad paid Claude-kit ratings, GEO/brand-voice/AI-policy/EU-AI-Act saturation, n8n free libraries, Claw Mart pricing
