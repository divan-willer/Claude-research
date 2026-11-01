# AI ecosystem gaps: MCP connectors, skill packs, setup pain and what is already sold (status 1 Nov 2026)

Phase 1 research. Role: ai-ecosystem-gaps. Prepared for the solo-founder "10 one-day digital products" project.

> **Read this first: how the evidence was gathered.** The shared web-search budget was used up before this agent's first search (the tool said "this turn's web search budget is used up"). So **no WebSearch results are used anywhere in this file**. All evidence comes from four machine-readable sources: the GitHub search API (via `gh api`), the official MCP Registry API (registry.modelcontextprotocol.io; a full dump of 54,491 latest-version server entries), the npm registry search API, and READMEs read through raw.githubusercontent.com. Because of this, the file has **almost no demand-side evidence**: no Reddit or forum threads, no Gumroad, Etsy, Fiverr or Upwork sales counts, and no vendor press releases. Treat every "gap" below as a **supply gap**, meaning nobody has built it yet. That is not proof that anyone will pay for it.

## Executive summary

1. **"Build an MCP connector for niche SMB software" (seed 5) is mostly closed as a one-day product.** Hosted-MCP aggregators now mass-publish to the official registry: io.usefulapi has 715 servers (including Mindbody, Boulevard, Acuity, Clio, Housecall Pro, Buildium, Teachworks, Healthie, Hostaway, JobNimbus, Gingr and Follow Up Boss), pipeworx-io has 1,916 and mrfentmen has 1,079. Several vendors also ship official servers or plugins: Intuit QuickBooks, Xero, Square, ShipStation, Wix, Kajabi, Planning Center, Shopify and Synthflow.
2. **The remaining zero-MCP products are mostly blocked.** These are Dentrix, Vagaro, Jane App, Pixieset, Pic-Time, Dubsado, 17hats, TaxDome and Tutorbird. Their APIs are partner-gated or missing (Dentrix Developer Program, Vagaro Enterprise API, Jane partner API, a reverse-engineered Tutorbird API), so a connector cannot be built or tested in one day. The only cheap route seen is a **Chrome extension over the web UI**, for example an existing Jane App bulk report-download extension.
3. **Profession skill packs (seed 1): free supply is huge and growing, so "first for profession X" is hard to claim.** New GitHub repos matching "claude skills" went from 704 (Nov 2025) to 16,857 (Oct 2026). Marketing, sales, founder, academic and legal are saturated (marketingskills alone has 57.8k stars). Anthropic itself gives away plugins for legal, finance, sales, marketing, support, K-12 teachers and healthcare. A free 44-profession plugin set already covers nurses, pharmacists, vets, physical therapists, dental hygienists, mortgage brokers, photographers, event planners and tradespeople, though shallowly (31 stars).
4. **The real remaining gap is depth plus distribution, not breadth.** Examples are packs tied to a specific SMB tool and workflow (a bookkeeper's month-end on the official QuickBooks connector, a small law firm on Clio, HVAC or plumbing quoting from Jobber or Housecall Pro exports), sold to non-developers who do not browse GitHub. Anthropic's own legal and finance plugins target enterprise tools (Westlaw, iManage, FactSet, Snowflake), not SMB tools.
5. **Setup pain for non-developers is real and well documented, but a weak product.** There are 1,312 "Cowork" issues in anthropics/claude-code since May 2026 and 927 issues in anthropics/claude-ai-mcp, including OAuth, connectors showing "Connected" with no tools, and Windows `spawn npx ENOENT`. Most of these are platform bugs that a guide cannot fix, they change weekly, and free guides already exist (mcp-for-beginners has 17.6k stars).
6. **New weak signal: local trades businesses publishing their own MCP servers** to the official registry (Aug to Oct 2026), such as plumbers, electricians, HVAC firms, pest control and dental clinics. This is a possible "agent-ready local business" kit (a seed 2 variant). However, several entries share one lead-gen template, and no evidence was found that AI assistants actually call them.
7. **GEO/AEO, brand voice, SOP-to-agent and EU AI Act tooling are crowded with free open-source options.** Of the seeds, only voice receptionist templates show clearly rising builder activity (GitHub "ai receptionist" repos went from 128 a month in Nov 2025 to 539 in Oct 2026). Free templates and an official Synthflow Claude plugin already exist.
8. **Paid skill packs do exist at $9 to $149 (one-time)**, for example a $19 50-skill "Claude Code Ops Pack" on Gumroad, a $29 PrintNest Pro and the ToolGenX catalogue of 21 products. **No sales or review counts were visible.**

## Summary table

| # | Gap / hypothesis | Verdict (for a 1-day product) | Strength | Evidence date | Key evidence | Best 1-day angle |
|---|---|---|---|---|---|---|
| G1 | MCP connectors for long-tail SMB software (seed 5) | **Reject as a connector product** | STRONG (supply side) | Mar to Nov 2026 | Registry: usefulapi 715, pipeworx 1,916, mrfentmen 1,079; official vendor MCPs for QBO, Xero, Square, Wix, Kajabi, etc. | None as a connector; see G3 |
| G2 | No-API / partner-gated vertical SaaS (Dentrix, Vagaro, Jane, Pixieset, Dubsado, TaxDome, Tutorbird, Pic-Time, 17hats) | Gap exists, but connector not buildable | MEDIUM | Oct 2026 | 0 MCP repos and 0 registry entries; API Evangelist profiles show partner programs | Chrome extension (export/report/bulk actions) needs a test account; ToS risk |
| G3 | Official connector exists, SMB workflow pack missing (QBO/Xero for bookkeepers; Clio/MyCase for small firms) | **Plausible** | MEDIUM-WEAK | Sep to Oct 2026 | Intuit official plugin and MCP (440 stars); Xero MCP 110k npm downloads a month; Anthropic legal/finance plugins target enterprise tools | "Setup guide + 8-12 workflow skills" on top of the official connector |
| G4 | Profession skill packs (seed 1), crowded professions | Reject: marketing, sales, founder, academic, legal, teachers, real estate, tax | STRONG | Jan to Nov 2026 | marketingskills 57.8k stars; academic-research-skills 54.9k stars; Anthropic plugins | n/a |
| G5 | Profession skill packs, thin professions (trades, salon/spa/studio owners, photographers' business side, wedding/florist, tutoring centres, dental office managers, vet clinics) | **Plausible but unproven demand** | WEAK | Mar to Oct 2026 | 0 to 9 repos each; 0 Claude community-marketplace plugins for hvac, salon, fitness, wedding, vet, realtor | Tool-specific pack (e.g. "HVAC quotes & follow-ups from Housecall Pro exports") |
| G6 | Non-developer setup pain (MCP, Cowork, connectors, OAuth, npx) | Pain real; product weak | STRONG (pain) / WEAK (product) | May to Nov 2026 | 1,312 Cowork-titled issues; 243 OAuth-titled claude-ai-mcp issues; Windows npx ENOENT | Lead magnet or bundle add-on, not a standalone product |
| G7 | "Agent-ready local business" (MCP listing + AI-assistant page; seed 2 variant) | Early, speculative | WEAK | Aug to Nov 2026 | ~14-25 single-business registry entries (plumbers, HVAC, electricians, pest control, dental) | Template kit for local-SEO freelancers |
| G8 | GEO/AEO/llms.txt kits (seed 2) | Crowded with free tools | STRONG (supply) | 2026 | 461 registry entries match GEO/AEO terms (noisy); open-seo-mcp-skills 8.5k stars; geo-optimizer-skill 1.3k stars; GitHub "geo aeo" repos 5 to 344 a month | Only if very vertical (see G7) |
| G9 | Voice receptionist templates (seed 6) | Rising builder activity; free templates exist | MEDIUM (supply trend) | Nov 2025 to Oct 2026 | GitHub "ai receptionist" repos 128 to 539 a month; free industry templates; official Synthflow Claude plugin | Vertical prompt + tool-schema pack for agencies, with compliance scripts |
| G10 | Brand voice packs (seed 7) | Reject | MEDIUM | 2026 | Anthropic marketing plugin "enforce brand voice"; Brand-building-skills 821 stars; 10 brand-voice MCPs | n/a |
| G11 | Chatbot test/QA kits for SMBs (seed 8) | No evidence either way | WEAK | 2026 | 1 GitHub repo; dev-only eval tools (deepeval in official plugins) | Not recommended without demand proof |
| G12 | SOP-to-agent converters (seed 10) | Crowded free tools | MEDIUM | 2025-2026 | strands-agents/agent-sop 1.2k stars; agentic-sop-to-work 211 stars; procedure-ops 63 stars; Anthropic skill-creator | Vertical "SOP to skill" templates only |
| G13 | EU AI Act packs (seed 3), ecosystem view | Crowded with free tools | MEDIUM | 2026 | 99 registry entries mention AI Act / ISO 42001; GitHub kits; see sibling file | n/a |
| G14 | Accessibility fix kits (seed 4), ecosystem view | Developer tooling crowded; store-owner side not assessed here | WEAK | 2026 | ~145 registry entries (noisy) incl. free WCAG checkers; Shopify a11y fixer apps | Defer to sibling file (lawsuit-driven demand) |
| G15 | AI policy packs for schools/tutoring (seed 9) | No ecosystem evidence | WEAK | 2026 | 2 GitHub repos; Anthropic Claude for Teachers ships free skills | n/a |
| G16 | What is already sold (paid skill packs, hosted MCP) | Market exists; volumes unknown | MEDIUM (prices) / none (sales) | May to Oct 2026 | $19, $29, £7-£12, $9-$149 packs; freemium hosted MCPs | Price anchor: $19-$49 one-time |

---

## A. Gap (a): MCP coverage for 80 SMB / vertical products

### Method
- **GitHub:** `gh api search/repositories q="<product> mcp"`, top 100 by stars. Repos were kept only if the name or description contains the product name **and** "mcp" or "model context". Columns: matched repos, repos with 5 or more stars, repos pushed on or after 2026-05-01. Counts are capped at 100, so high-volume products are lower bounds. Ambiguous names (Square, Toast, Clover, Lightspeed, Podium, Wave, Circle, Google Classroom) include false positives, flagged below.
- **Official MCP Registry:** full dump of `https://registry.modelcontextprotocol.io/v0/servers?limit=100&version=latest` (545 pages, 54,491 entries, 36,341 with a remote endpoint), regex-matched on name, title and description, then hand-cleaned.
- **npm:** `https://registry.npmjs.org/-/v1/search?text=<product>+mcp&size=100`, filtered the same way. Monthly downloads come from the search API and include bot and CI traffic.
- **"Official"** means a repo in the vendor's GitHub org, a vendor-namespaced registry entry (e.g. `com.kajabi/kajabi`), or a vendor plugin in Anthropic's official plugin marketplace. Vendors may also have hosted connectors in the Claude, ChatGPT or other directories that this run could not check.

### Results (sorted roughly from no coverage to crowded)

| Product | GitHub MCP repos (>=5 stars / pushed since May-26) | Best GitHub repo (stars, last push) | Registry servers (cleaned) | npm MCP pkgs (top downloads/mo) | Official? | Read |
|---|---|---|---|---|---|---|
| Dentrix | 0 | n/a | 0 | 0 | No (partner-only "Dentrix Developer Program" per API Evangelist profile) | **Gap, blocked** |
| Vagaro | 0 | n/a | 0 | 0 | No ("Enterprise Business API") | **Gap, blocked** |
| Jane App | 0 | n/a (only a Chrome report-scraper extension) | 0 | 0 | No (partner API per profile) | **Gap, blocked** |
| Dubsado | 0 | n/a | 0 | 0 | No API profile found | Gap |
| 17hats | 0 | n/a | 0 | 0 | Unknown | Gap |
| Pixieset | 0 | n/a | 0 | 0 | Profile lists Clients/Collections/Contracts/Invoices APIs; access terms unknown | Gap, unverified API |
| Pic-Time | 0 | n/a | 0 | 0 | Unknown | Gap |
| TaxDome | 0 | n/a | 0 | 0 | Unknown | Gap |
| Tutorbird | 0 | n/a (unofficial reverse-engineered API doc) | 0 | 0 | No public OpenAPI ("Zapier-shaped" keys) | Gap, fragile |
| Teachworks | 0 | n/a | 1 (usefulapi, hosted) | 0 | No | Covered by aggregator |
| Thryv | 0 | n/a | 0 | 0 | Unknown | Gap (low priority) |
| FieldEdge | 1 (0/0) | BusyBee3333 mass-generated (0, Feb-26) | 0 | 0 | No | Toy only |
| ShootProof | 1 (0/0) | 0 stars, last push May-2025 (OLD) | 1 (mrfentmen) | 0 | No | Toy only |
| Open Dental | 2 (1/2) | sanjibani/open-dental-mcp (7, Jun-26) | 0 | 0 | No | Thin |
| Boulevard | 2 (0/0) | 0 stars | 1 (usefulapi) | 0 | No | Aggregator |
| Acuity Scheduling | 2 (0/1) | 0 stars | 1 (usefulapi) | 0 | No | Aggregator |
| Karbon | 4 (0/2) | 1 star | 1 | 0 | No | Thin |
| PracticePanther | 2 (0/2) | 1 star | 0 | 1 (19/mo) | No | Thin |
| MyCase | 2 (1/2) | oktopeak/mycase-mcp (6) | 1 | 2 (345/mo) | No | Thin |
| HoneyBook | 1 (0/1) | chrischall/honeybook-mcp (1); **client-portal side**, not the business account | 1 | 1 (2,474/mo) | No | Business-side gap |
| SimplePractice / TherapyNotes | 1 each (client-portal readers) | chrischall (1) | 1 / 1 | 1 (1,699/mo) | No | Clinician-side gap |
| Kajabi | 1 real (0) | n/a | 1: **com.kajabi/kajabi (official, remote)** | 0 | **Yes** | Closed |
| Teachable / Thinkific | 2 / 3 (all 0 stars) | n/a | 0 / 0 | 2 (757/mo) / 0 | No | Thin |
| Skool | 19 (3/15) | louiewoof2026/skool-mcp (59, Mar-26) | 1 (cotlet) | 0 | No | Covered |
| Mindbody | 8 (1/4) | vespo92/MindbodyMCP (11, Mar-26) | 2 (usefulapi, studiovector) | 1 | No | Aggregator |
| Gusto | 5 (0/2) | 1 star | 0 | 1 (12/mo) | None found | Thin |
| Buildertrend | 3 (0/2) | 0 stars | 0 | 0 | None found | Thin |
| Procore | 11 (2/7) | TylerIlunga/procore-mcp-server (17, Aug-26) | 0 | 0 | None found in GitHub org or registry | Partly covered |
| ServiceTitan | 20 (1/11) | montrellcruse/servicetitan-mcp (5, Oct-26) | 0 | 1 (315/mo) | None found | Many toys, no leader |
| Jobber | 19 (1/15) | BusyBee3333 (5); chrischall (client-hub side) | 3-6 | 3 (1,619/mo) | None found (GetJobber org has an unrelated bot repo) | Many toys, no leader |
| Housecall Pro | 14 (2/11) | BuildWithBeacon (19, **stale since Jun-2025**) | 3 incl. usefulapi | 3 (1,673/mo) | None found | Aggregator + toys |
| Clio | ~29 (5/24) | oktopeak/clio-mcp (27, Oct-26) | 3 incl. usefulapi | 3 (897/mo) | None found | Covered by third parties |
| Filevine / Lawmatics / Smokeball | 5 / 8 / 1 | RosenAdvertising, oktopeak suites (<=4) | 2 / 1 / 0 | 2 / 2 / 0 | No | Legal MCP suites emerging |
| AppFolio / Buildium | 8 / 3 | CryptoCultCurt (10) / luthersystems (6) | 2 / 1 (usefulapi) | 3 / 1 | No | Covered |
| Follow Up Boss | 6 (1/4) | mindwear-capitian (33, Oct-26) | 4-5 incl. usefulapi | 1 | No | Covered |
| kvCORE / BoldTrail | 1 (0/1) | 0 stars | 0 | 0 | None found | Thin |
| Guesty / Hostaway / OwnerRez / Lodgify / Cloudbeds | 10 / 9 / 5 / 3 / 4 | all <=4 stars | 1-4 each (usefulapi for Hostaway, OwnerRez) | Hostaway 2,383/mo | No | Short-term rental: crowded with small tools |
| Zenoti / Fresha | 2 / 10 | cotletdev/fresha-api-mcp-server (7) | 1 / 1 (cotlet) | 1 / 2 | No | Covered |
| Tebra/Kareo / Healthie / Practice Better | 3 / 0 / 0 | 1 star | 1 / 1 (usefulapi) / 1 (usefulapi) | 1 (984/mo) / 0 / 0 | No | Aggregator |
| JobNimbus / AccuLynx / CompanyCam / Contractor Foreman | 4 / 2 / 2 / 1 | <=6 stars | 1 (usefulapi) / 0 / 0 / 1 (cotlet) | 2 / 2 / 0 / 0 | No | Roofing/construction: thin |
| PowerSchool | 3 (0/1) | 2 stars | 0 | 0 | None found | Thin (district-gated) |
| Canvas LMS | 98+ (14/68) | vishalsachdev/canvas-mcp (310, Nov-26) | ~10+ | 13 | None in GitHub org | **Crowded** |
| Google Classroom | ~42 (noisy) | 7 stars | 2-7 | 6 (2,936/mo) | None found | Crowded |
| Calendly | 34 (2/18) | meAmitPatil (10) | 2-3 (pipeworx) | 3 | None found | Crowded |
| Etsy | 60 (4/44) | semihbugrasezer/seerxo (28) | 7-24 (includes Etsy-tool vendors) | 6 | None found | Crowded |
| Printful | 11 (1/8) | Purple-Horizons/printful-mcp (32) | 1 (usefulapi) | 1 | No | Covered |
| Lightroom | 36 (6/31) | Automaat/lightroom-mcp (171, Oct-26) | 2 | 2 | None found | Covered |
| Squarespace | 9 (2/8) | BusyBee3333 (9), timncox (8) | 1 | 1 | None found | Covered |
| FreshBooks | 24 (0/13) | 3 stars | 2 | 2 (2,874/mo) | None found | Many, no leader |
| Wave | 3 (1/2) | LunaParker/waveapps-mcp (6) | 0 | 0 | None found | Thin |
| Toast | ~37 (noisy) | BusyBee3333 toast (16) | 1 (consumer-side) | 1 (251/mo) | None found | Thin real coverage |
| ShipStation | 6 (1/2) | **shipstation/mcp-shipstation-api (12, official org)** | 0 | 1 | **Yes (GitHub org)** | Closed |
| Square | many (noisy) | **square/square-mcp-server (109, official org)** | 0 vendor-namespaced | 1 (3,175/mo) | **Yes** | Closed |
| Wix | 26 | **wix/wix-mcp (15); com.wix/mcp; official "wix" Claude plugin** | 1 official | 2 (3,527/mo) | **Yes** | Closed |
| QuickBooks | 90+ (10/57) | **intuit/quickbooks-online-mcp-server (440); official "intuit-quickbooks" Claude plugin** | 13-31 | 8 | **Yes** | Closed; setup-guide angle |
| Xero | 92+ (3/56) | **XeroAPI/xero-mcp-server (388)** | 12-17 | 19 (**@xeroapi/xero-mcp-server 110,071/mo**) | **Yes** | Closed; setup-guide angle |
| Planning Center | 24 | jake-ccnh/pco-mcp (11, last push Oct-2025) | **com.planningcenter/mcp (official)** | 0 | **Yes** | Closed |
| GoHighLevel | 98+ (9/62) | mastanley13/GoHighLevel-MCP (196; last push Jul-2025) | 4-14 | 18 (@elitedcs/ghl-mcp 5,306/mo) | None found in registry or GitHub | **Crowded** |
| Shopify | 60+ (31 >=5 stars) | GeLi2001/shopify-mcp (239); official Shopify-AI-Toolkit plugin | 43-168 | 33 | **Yes** | Saturated |
| Zoho | n/a | zoho/analytics-mcp-server, zoho/zoho-billing-mcp (official org) | 5 | 5 | **Partly (Zoho org)** | Partly closed |

**Mass generators to know about** (they make "be first with a connector" a race you lose):
- **io.usefulapi**: 715 hosted remote servers, "authorize once and go". Seen vertical entries: acuity-scheduling, boulevard, buildium, clio, follow-up-boss, gingr, healthie, hostaway, housecall-pro, jobnimbus, mindbody, ownerrez, practice-better, printful, teachworks, lightspeed r/x-series. Its README describes hosted MCP servers for existing tools with no local install ("No local install, no key-juggling: authorize once and go").
- **pipeworx-io**: 1,916 servers, including QuickBooks, Xero, Etsy and Calendly. Freemium: "Without a key it calls anonymously, capped at 50 calls a day."
- **mrfentmen** (1,079), **BusyBee3333** ("…-mcp-2026-complete" repos for FieldEdge, Acuity, Housecall Pro, ServiceTitan, Squarespace, Toast, Clover, Lightspeed, GoHighLevel), **cotlet** (Fresha, Booksy, Skool, Contractor Foreman, Tradify, Pirate Ship), **chrischall** (client-portal readers for Jobber, Housecall Pro, HoneyBook, SimplePractice, FreshBooks and Toast).
- Registry publishing is accelerating. By latest-version publish month: 2,036 (May 2026), 3,702 (Jul), 10,411 (Sep), 23,380 (Oct). This metric over-weights recently updated servers, so read it as activity, not as new launches.

**Buildability verdict for seed 5:** a one-day MCP connector is technically feasible only where a public, self-serve API key exists (e.g. FreshBooks, Wave, Gusto?, Buildertrend?; not verified). In every such case a free or aggregator alternative already exists or can appear within weeks. Where no MCP exists (Dentrix, Vagaro, Jane), the reason is API gating, which makes it **not** one-day. Strength: STRONG on supply; demand not measured.

### G2: The no-API / partner-gated tail, where a Chrome extension is the cheap route
- Evidence: zero MCP repos, registry entries or npm packages for Dentrix, Vagaro, Jane App, Dubsado, 17hats, Pixieset, Pic-Time, TaxDome and Tutorbird (searches above).
- API Evangelist (third-party profiles, Oct-Nov 2026) describes the access model:
  - **Dentrix:** APIs "through two dis[tinct]" channels, including a "Dentrix Developer Program" with a "commercial-only Scheduling API".
  - **Vagaro:** "Access token issuance for the Enterprise Business API".
  - **Jane:** a patients API "for the practitioner's accessible patients within a clinic" plus partner webhooks.
  - **Tutorbird:** "publishes no official OpenAPI document. The surface is Zapier-shaped" (unofficial repo).
- Existing pattern: a Manifest V3 Chrome extension that bulk-downloads all CSV reports from a Jane App clinic's Admin, Reports page in one click (tomjwc/JaneApp---Reports-Scraper, 1 star, Aug 2026).
- One-day angle: a Chrome extension that does one tedious bulk action in a no-API vertical tool (export, bulk tag, report download, copy client data into a Claude-ready summary). Sold on the Chrome Web Store with a Stripe or Lemon Squeezy licence.
- **Honest buildability:** you need a real or trial account to test it. DOM scraping breaks when the vendor changes its UI. ToS and health-data (HIPAA/PIPEDA) risk applies for Jane, Dentrix and SimplePractice. Evidence strength: WEAK (one repo; no buyer evidence).

### G3: Official connector exists, but no SMB-workflow layer
- Intuit ships an official QuickBooks MCP (440 stars) **and** an official Claude plugin, "intuit-quickbooks": "QuickBooks business insights and actions: financial health briefings across P&L, cash flow…, overdue-invoice reminders". Xero's official server shows 110,071 npm downloads a month.
- Anthropic's own finance plugin lists "Snowflake, Databricks, BigQuery, Slack, Microsoft 365" as connectors. Its financial-services repo targets "investment banking, equity research, private equity, and wealth management". Its legal repo names Westlaw, Thomson Reuters, CourtListener, iManage, Ironclad and Everlaw, but **not** Clio, MyCase, PracticePanther or Smokeball (grep of the README).
- So for **SMB bookkeepers** (QuickBooks/Xero) and **small law firms** (Clio/MyCase), the connector exists (official or third-party) but packaged workflows are thin. Existing free bookkeeping skills are small: startup-bookkeeper (20 stars), polytheseus/bookkeeper-skills (0 stars), plus the generic "bookkeeper" plugin in alexclowe's set. openaccountants (469 stars) covers tax rules, not QBO operations.
- One-day angle: "Claude + QuickBooks for bookkeepers: setup guide + 10 workflow skills (month-end checklist, uncategorised-transaction triage, A/R chase emails, client P&L narrative)". Sold as a ZIP plus PDF. Buildable in a day if you have a QBO sandbox (Intuit developer sandboxes are free; not verified in this run).
- Counter-evidence: Intuit could extend its plugin; free skills exist; and **no evidence was collected that bookkeepers buy such packs**. Strength: MEDIUM-WEAK.

---

## B. Gap (b): which professions already have packs (crowded) and which have none

Method: `gh api search/repositories q="<profession> claude skills"`, filtered on profession words plus skill/claude/plugin/agent. Matched counts are capped at 100. Also checked: Anthropic's official (315) and community (2,283) plugin marketplace JSON files, and keyword searches like "<profession> claude".

### Crowded: avoid unless you have a sharp angle

| Profession | Matched repos (>=10 stars) | Leader(s) | Free official alternative |
|---|---|---|---|
| Marketing | 1,450 total; 87 shown, all >=10 stars | coreyhaines31/marketingskills **57,831 stars** | Anthropic `marketing` plugin |
| Academic / research | 693 total | Imbad0202/academic-research-skills **54,870 stars** | n/a |
| Sales | 583 total (55 >=10 stars) | zubair-trabzada/ai-sales-team-claude (1,499) | Anthropic `sales` plugin |
| Founder / startup | 381 total (41 >=10 stars) | Jakeschincariol/founder-skill (2,313) | anthropics/launch-your-agent |
| Legal | 42 (5 >=10 stars) | evolsb/claude-legal-skill (492), skala-io/legal-skills (53) | anthropics/claude-for-legal (9,864 stars); LegalZoom official plugin |
| Accounting / tax | 98 (20 >=10 stars) | openaccountants (469; "2,250 skills across 266 jurisdictions") | Anthropic `finance` plugin; Intuit plugin |
| Teachers (K-12) | 78 (3 >=10 stars) | GarethManning/education-agent-skills (939) | anthropics/k12-teacher-skills, bundled with "Claude for Teachers" |
| Real estate | 86 (13 >=10 stars) | zubair-trabzada/ai-realestate-claude (187); miron-tech/realtor-claude-skills (15) | n/a |
| Financial advisors | few repos | n/a | **Official** BlackRock, Vanguard and Zocks advisor plugins |
| Healthcare (payer/provider coding) | n/a | n/a | anthropics/healthcare (ICD-10, CPT, prior auth) |
| Ecommerce / Amazon | 244 total (34 >=10 stars) | nexscope-ai/Amazon-Skills (822) | Shopify AI Toolkit |

### Thin or no supply (supply gaps; demand unverified)

| Profession / buyer | Evidence of supply | Notes |
|---|---|---|
| Trades (HVAC, plumbing, electrical, roofing) | miron-tech/hvac-claude-skills (6 stars), KRASA-AI/hvac-ai-skills (3), emd-ai/trades-claude-skills (3), alexclowe "tradesperson"; **0** "hvac" plugins in the Claude community marketplace | Many Jobber/HCP/ServiceTitan MCP toys exist (section A). Trades are also the main target of AI-receptionist builders (G9). Best candidate for a tool-specific pack. |
| Salon / spa / med-spa / fitness studio owners | "salon claude skills": 5 repos, mostly vendor connector plugins (hairdora, salonnow); "fitness": 66 repos are personal-fitness apps, not studio owners; **0** salon or fitness plugins in the community marketplace | Mindbody, Boulevard, Fresha and Zenoti are covered by aggregator MCPs; Vagaro is blocked |
| Dental practice / office managers | 2 repos (Tuminha/dental-ai-skills, 7 stars, clinical research focus); alexclowe "dental hygienist" | Dentrix is API-gated; Open Dental has 2 small MCPs |
| Veterinary clinics | 3 repos (Gonzih/skills-veterinary, 0 stars); veterical/claude-plugin (vendor connector); alexclowe "veterinarian" | Gingr is on usefulapi |
| Photographers (business side: galleries, contracts, client comms) | 2 repos (RAW grading, not business); alexclowe "photographer" | Pixieset and Pic-Time have no MCP; Lightroom MCP exists (171 stars) |
| Wedding / event planners, florists | wedding 8 repos (0 >=10 stars); florist 0 relevant | HoneyBook and Dubsado: business-side gap (no API for Dubsado) |
| Tutoring centres / music schools | "tutoring center claude": 2 irrelevant repos; "music teacher": 4 | Teachworks on usefulapi; Tutorbird has an unofficial API only |
| Property managers (long-term) | 3 repos; msg2ai/vacationrental-team-skills (3) | AppFolio and Buildium MCPs exist |
| Nurses, pharmacists, PTs, chiropractors | 0-2 repos each in targeted searches, **but** alexclowe/awesome-claude-cowork-plugins includes nurse, pharmacist, physical therapist, chiropractor, OT, optometrist, SLP and therapist | Clinical documentation raises HIPAA/liability concerns; low-star free packs already exist |

**The key counter-evidence for seed 1:** alexclowe/awesome-claude-cowork-plugins offers "44 profession-specific plugin suites for Claude Cowork and Claude Code", free. It covers nurse, pharmacist, vet, dental hygienist, chiropractor, therapist, attorney, paralegal, bookkeeper, financial advisor, insurance agent, mortgage broker, property manager, real estate agent, photographer, interior designer, event planner, personal trainer, dietitian, teacher, construction PM and tradesperson. It has only **31 stars**. Two readings are possible: (i) the breadth gap is already filled for free, so you must compete on depth; or (ii) even free profession packs get little traction on GitHub, because non-developer professionals are not there. **Neither demand nor distribution for non-developer buyers could be evidenced in this run.** Also note that the plugin README itself says "plugins need a paid Claude plan — Pro, Max, or Team". The buyer must already pay for Claude.

**Scale of the free skill supply (supply-side trend, STRONG):** new GitHub repos matching "claude skills" per month were 704 (Nov 2025), 3,382 (Jan 2026), 11,357 (Mar), 12,908 (May), 12,796 (Jul), 10,867 (Aug), 10,980 (Sep) and 16,857 (Oct 2026). The `skills` CLI (vercel-labs/skills, "The open agent skills ecosystem") shows 16.7M npm downloads a month. anthropics/skills has 186,310 stars. This is a fast-filling space.

---

## C. Gap (c): setup problems non-developers hit

Evidence comes from GitHub issue search (`gh api search/issues`), which captures mostly technical reporters. Counts are full-text or title matches and noisy.

| Problem | Representative issues (date, reactions, comments) | Fixable by a guide? |
|---|---|---|
| `npx`/`uvx` not found from Claude Desktop (nvm, Windows `npx.cmd`) | modelcontextprotocol/servers#64 "MCP Servers Don't Work with NVM" (2024-11-26, 182 reactions, 91 comments; **OLD** but the top-reacted one); anthropics/claude-code#58510 "Windows: plugin-shipped MCP servers using bare `npx` fail with `spawn ENOENT`" (2026-05-12); CherryHQ/cherry-studio#14966 (2026-05-09); wevm/incur#275 (2026-10-21). 559 issues contain "spawn npx ENOENT" (all time) | Partly (absolute paths, `npx.cmd`) |
| Desktop updates breaking local MCP | anthropics/claude-ai-mcp#664 "MCP tool calls never reach Filesystem-type servers after Desktop update" (2026-07-22, 52 reactions, 93 comments); mims-harvard/ToolUniverse#585 "Claude Desktop extension shows 'Failed — Server disconnected' — how to fix it now" (2026-09-15) | No (platform bug) |
| Cowork on Windows | anthropics/claude-code#92984 "Cowork (Windows): all Plan9 shares fail…" (2026-09-09, 61 reactions, 121 comments); #57371 disable bundled Cowork service (2026-05-08, 67 reactions); #66535 sandbox never ready on ARM64 (2026-06-09). 336 Cowork + Windows title issues since May 2026 | No |
| Connectors "Connected" but no tools / OAuth failures | anthropics/claude-code#61682 GitHub connector shows "Connected" but exposes no tools (2026-05-23, 25 reactions); #59854 "OAuth DCR unsupported" (2026-05-17); anthropics/claude-ai-mcp#476 custom remote connector tools never surfaced (2026-06-21, 18 reactions, 35 comments); #728 Google Sheets MCP OAuth (2026-07-30); #1204 "Server URL doesn't match expected format" (2026-10-30); #1207 authorization error after OAuth (2026-10-31). 243 OAuth-titled and 539 connector-titled claude-ai-mcp issues since May 2026 | Mostly no |
| Permission-prompt fatigue | anthropics/claude-ai-mcp#491 "Cowork (Team plan): custom remote MCP connector prompts on every tool call" (2026-06-24, 23 reactions) | Partly (settings) |
| Plugins / skills in Cowork | anthropics/claude-code#56376 plugin-upload validation errors swallowed (2026-05-05); #91394 cannot add claude-plugins-community marketplace in Cowork (2026-09-02); #87537 plugin-bundled stdio MCP servers silently dropped in cloud sessions (2026-08-18); #94321 plugin MCP OAuth not durable (2026-09-14); #103282 coordinator session cannot access Dropbox/Google Drive connectors (2026-10-18) | No |
| n8n + MCP | czlonkowski/n8n-mcp (23,187 stars); #340 "Server Disconnected - Claude Desktop" (2025-10-19, OLD-ish); #1159 "Added 1-click config generator and setup guide…" (2026-10-14) | Free config generators exist |
| Voice agents (Vapi/Retell) | No useful setup-pain signal in GitHub issues (title searches mostly returned unrelated "vapi"/"retell" words) | n/a: no evidence found |

Overall volume: 1,312 issues with "cowork" in the title in anthropics/claude-code created since 2026-05-01, and 927 issues in anthropics/claude-ai-mcp since 2026-05-01.

**Counter-evidence and alternatives:**
- One-click installs exist: modelcontextprotocol/mcpb "Desktop Extensions: One-click local MCP server installation" (2,162 stars), and `@anthropic-ai/mcpb` shows ~718k npm downloads a month.
- Hosted connectors (usefulapi, official vendor servers) remove the JSON-config step.
- Free guides exist: microsoft/mcp-for-beginners (17,579 stars), zebbern/claude-code-guide (4,691), FlorianBruniaux/claude-cowork-guide (255; "43 workflows, 70 prompts"), carlvellotti/cowork-complete-guide ("Free interactive course").

**Verdict:** the pain is STRONG and current. A paid troubleshooting guide is WEAK, because the bugs are vendor-side, the advice goes stale fast, and free guides exist. Its best use is as a free lead magnet or as a "setup chapter" bundled into a G3/G5 pack.

---

## D. Gap (d): what is already being sold, and at what price

| Offer | Price | Where | Sales / reviews visible? | Source |
|---|---|---|---|---|
| "Claude Code Ops Pack": 50 skills (business ops, dev ops, marketing) incl. a gumroad-listing-writer and an invoice generator | **$19** | Gumroad (libertybound0.gumroad.com/l/claude-ops-pack) | No | signcrypt/claude-ops-pack-sampler README (2026-10-31) |
| "PrintNest Worksheets Pro": Claude Code skill that generates sellable worksheet PDFs for Etsy, TPT and KDP (40+ types; free 5-type Lite) | **$29** | Gumroad (synishida.gumroad.com/l/printnest-worksheets-pro) | No | nishidagonyuya/printnest-worksheets-lite README (May 2026) |
| ToolGenX / agentskillpacks.com: 21 products, e.g. "Idea to App OS" ($149, for "people who have never written code"), "AI SEO Agency OS" ($149), "AI Agency Launch Kit" ($119), "AI SEO Command Suite" ($69), "AI Search Visibility Toolkit" (GEO, $49), "AI CFO Toolkit" (reads a QuickBooks CSV, $29), "Structured Data Pro Pack" (JSON-LD templates, $19), "Visa Document Translator" ($9) | **$9 to $149** one-time | Own site | No | ismailGunaydn/ToolgenX.github.io README (Oct 2026) |
| "AI Agent Buyer Pack": Claude Code Skill Pack (25 skills + hooks) £12; Hermes Audit Suite £9; NHS Nurse Planner £7 | **£7 to £12** | Not stated (Gumroad tag) | No | bv-12345/agent-buyer-pack-preview README (May-Oct 2026) |
| Hosted MCP freemium: pipeworx (50 anonymous calls/day, free key raises cap); Guesty MCP by DLJRealty ("23 free read-only tools live; 43 total (Pro+Enterprise)"); MakeBox Etsy MCP ("MakeBox Pro or Studio required"); techandtoast ("First question free, then $2 each") | Freemium / subscription | MCP Registry | No | Registry entries (Sep-Oct 2026) |
| Voice-receptionist market pricing aggregators: receptionistprices.com ("Dated AI and virtual receptionist prices…"), aireceptionistrankings.com ("prices at 100 and 200 calls") | n/a | MCP Registry | n/a | Registry (Oct 2026), a sign of a mature, comparison-shopped SaaS market |

Not found in this run (web search unavailable): Fiverr/Upwork MCP-setup gigs, Etsy listings for AI prompt or skill packs, Gumroad Discover sales or ratings counts, Vapi/Retell/Synthflow template-marketplace listings, ChatGPT GPT/app store data. **No evidence found** is not evidence of absence here; it reflects the method limit.

---

## E. Seed hypotheses: evidence for and against (from the AI-ecosystem angle)

1. **Skill packs for non-developer professions.** *For:* exploding skill supply shows the format is mainstream. Paid packs exist at $9-$149. Specific professions (trades, salon/studio owners, dental offices, photographers' business side, wedding planners, tutoring centres) have little or only shallow supply. *Against:* Anthropic and vendors give away plugins for the biggest professions (legal, finance, sales, marketing, support, K-12, healthcare, advisors). There is a free 44-profession set. Buyers must hold a paid Claude plan and cope with plugin/Cowork install bugs (section C). No sales data. **Verdict:** only a tool- and workflow-specific depth pack (G3/G5) is defensible. MEDIUM-WEAK.
2. **"Get found by AI search" kits.** *For:* builder activity is rising (GitHub "geo aeo" new repos per month: Nov-25 5, Jan-26 24, Mar 82, May 170, Jul 272, Aug 267, Sep 286, Oct 344; "llms.txt": Nov-25 39 to Oct-26 370). Local businesses have started publishing MCP servers (G7). *Against:* heavy free supply (open-seo-mcp-skills 8,534 stars, geo-optimizer-skill 1,255, fire-your-seo-agency 987, firecrawl/llmstxt-generator 539), 461 GEO/AEO-ish registry entries and paid toolkits already at $19-$49. The sibling file (regulation-and-platform-shifts.md) reports log studies doubting llms.txt. **Verdict:** crowded. Only a very vertical, done-for-you variant (G7) might differentiate. WEAK-MEDIUM.
3. **EU AI Act packs.** 99 registry entries mention AI Act or ISO 42001, many free (e.g. "Read-only EU AI Act tools… Free", euaiactlaw's eu-ai-act-explorer), plus GitHub kits (ogulcanaydogan/eu-ai-act-compliance-kit). The sibling file says the duty was softened. **Verdict:** reject from this angle.
4. **Accessibility fix kits.** About 145 registry entries match accessibility/WCAG (many are browser-automation "accessibility tree" tools). There are free WCAG MCP checkers (accesslumens, Veduis/wcag-compliance-mcp), Shopify a11y fixer plugins (AmazingPlugins) and a Shopify theme audit skill (44 stars). Developer tooling is crowded. Whether non-technical store owners would buy a checklist kit depends on the lawsuit evidence in the sibling file. **No verdict from this angle.**
5. **MCP connectors / setup guides.** Connectors: reject (section A). Setup guides: only bundled with official connectors (G3); a standalone guide is weak (section C).
6. **Voice receptionist templates.** *For:* GitHub "ai receptionist" new repos per month: 128 (Nov-25), 141 (Jan-26), 287 (Mar), 328 (May), 546 (Jul), 411 (Aug), 419 (Sep), 539 (Oct). This is builder and agency demand for templates. Trades, dental and legal are recurring targets (e.g. a dental receptionist on Open Dental's API, a law-firm receptionist on Retell). *Against:* free industry templates exist (TRivers01/ai-receptionist-templates covers dental, legal, HVAC, salon and real estate; dom-ran/voice-receptionist-ai; TomHardiman6/ai-receptionist-starter), there is an official Synthflow Claude plugin, receptionist SaaS vendors list themselves in the MCP registry (Nexwin, Larkella, Gini, VoiceDesk), and price-comparison sites exist. **Verdict:** MEDIUM for an agency-facing vertical pack (prompts + tool schemas + test-call scripts + compliance script from the sibling file). Buyers are AI-automation agencies, not the trade owners.
7. **Brand voice packs.** Anthropic's marketing plugin "enforce[s] brand voice". There are free brand-skill repos (Brand-building-skills 821 stars, cofoundy/brand-skills 68) and brand-voice MCP services (Marcora, StyleMCP, Brandcode). **Reject.**
8. **Chatbot test/QA kits.** One GitHub repo for SMB eval (0 stars). Eval tooling (deepeval, Langfuse) targets developers and appears in the official plugin marketplace. **No demand evidence found. WEAK.**
9. **AI usage policy packs for schools/tutoring.** Only 2 GitHub repos (e.g. urduaiorg/aiforedu "policy templates"). Anthropic's "Claude for Teachers" bundles free K-12 skills. The sibling file finds no tutoring-centre mandate. **Reject from this angle.**
10. **SOP-to-agent converters.** strands-agents/agent-sop (1,208 stars), s0912758806p/agentic-sop-to-work (211; "Turn human SOPs into deterministic, gated agentic workflows — a Claude Code plug[in]"), charlesdove977/procedure-ops (63), plus Anthropic's free skill-creator. **Reject as a generic tool.** Possibly fold into G3/G5 as an "add your own SOPs" template.

---

## F. Detailed entries for the most promising gaps

### G3 / G5. Tool-specific workflow packs for under-served SMB roles
- **Who would buy:** bookkeepers on QuickBooks or Xero; small law firms on Clio or MyCase; HVAC/plumbing owners on Jobber or Housecall Pro; salon or studio owners on Mindbody, Boulevard or Fresha. These are assumptions, with no buyer evidence in this run.
- **Evidence:** official QBO and Xero connectors (A); Anthropic's legal and finance plugins target enterprise tools (A, G3); thin trades, salon and studio supply (B); hosted MCPs for these tools exist (usefulapi), so a pack can reference an existing connector instead of building one.
- **Current alternatives:** free generic profession plugins (alexclowe), free vendor plugins (Intuit), aggregator connectors, and Anthropic's generic plugins.
- **One-day product:** a ZIP of 8-12 SKILL.md files plus a CLAUDE.md or "practice profile" template, a 10-page PDF setup guide (connect the official or hosted connector in Claude Desktop/Cowork, with fixes for the top 5 errors in section C), and sample prompts. Sell for $19-$49 (anchored by D) on Gumroad or Lemon Squeezy.
- **Buildability:** HIGH for skills that work from exported CSV/PDF files (no API needed). MEDIUM if you want to demo live connector use, since that requires vendor accounts or sandboxes. The risk is distribution, not the build.
- **Strength:** WEAK-MEDIUM (supply-side only).

### G7. "Agent-ready local business" listing kit
- **Evidence:** single-business entries in the official MCP registry, published Aug-Nov 2026:
  - kcplumb.com ("Book plumber in Kansas City, MO… free callback"; website path `/for-ai-assistants`).
  - kcvolts.com and austinvolts.com (same template, so likely one lead-gen operator).
  - Western Sky HVAC (2 locations), thejohnsonbros.com plumbing, delcoplumbernow.com, absolutebestair.com HVAC, kay1electric.ca, lordmechanical, wavespestcontrol, inescapable.app car detailing, Virohana and Dental Digital Center clinics.
  - Salons and barbers via platforms (belcome.app, easyweek, joinmane).
- **Against:** no evidence that ChatGPT, Claude or Perplexity route local-service queries to registry-listed MCP servers. Some entries look like SEO lead-gen sites, not businesses. The GEO tool space is crowded.
- **One-day product:** a template repo or Cloudflare Worker that serves a read-only "services, areas, prices, booking link" MCP endpoint plus JSON-LD and llms.txt, with a guide to publishing to the registry. Buyers would be local-SEO freelancers or agencies.
- **Buildability:** HIGH. Demand: unproven. **Strength: WEAK.**

### G9. Vertical voice-receptionist template pack (agency-facing)
- **Evidence:** rising repo creation (above); vertical demos (signalwire-demos/dental "uses Opendental API to be a complete dental receptionist"; Awaisali36 law-firm Retell receptionist; HVAC voice agents).
- **Against:** free templates and vendor tooling; a mature SaaS market (comparison sites). Compliance risk is covered in the sibling file.
- **One-day product:** per-vertical (HVAC, dental, legal intake) system prompt, tool/function JSON for Vapi/Retell, a test-call script and QA checklist, and a disclosure/consent script. **Buildability:** HIGH for docs/JSON; testing needs a paid Vapi or Retell account and a phone number. **Strength: MEDIUM-WEAK.**

### G2. Chrome extension for a no-API vertical tool
- See section A (G2). **Strength: WEAK.** Highest technical risk of the set. The only cheap way to "integrate" with Dentrix, Jane, Vagaro, Pixieset or Dubsado.

---

## Method & limitations

- **No web search results were used.** The shared WebSearch budget (200 per turn) was already used up by other agents when this agent started. Per the tool's instruction, no workarounds were attempted. Consequently there is no Reddit, forum, Hacker News, Product Hunt, Gumroad Discover, Etsy, Fiverr, Upwork, vendor-blog or press evidence. **Demand-side claims are therefore almost entirely missing.** The lead should re-run demand checks (Reddit r/ClaudeAI, r/bookkeeping, r/HVAC, r/smallbusiness; Gumroad and Etsy listing counts; Fiverr "MCP setup" gigs) in a follow-up session.
- Pages were **not opened in a browser**. Data came from APIs (GitHub search, MCP Registry, npm search) and raw READMEs. Quotes are verbatim from those READMEs or API descriptions.
- GitHub repository-search counts are fuzzy: they include false positives for ambiguous names, are capped at 100 items per query, and count supply, not usage. Star counts are a weak proxy for adoption. Monthly repo counts use `created:` date ranges; adjacent ranges share one boundary day.
- MCP Registry: the dump is of latest versions only (54,491 entries). "publishedAt" is the latest version's date, not first publication. Regex categorisation is noisy (e.g. "geo" matches geography).
- npm "monthly downloads" from the search API include CI and bot installs.
- "Official" status was checked only via vendor GitHub orgs, vendor-namespaced registry names and Anthropic's official plugin marketplace JSON. Vendor-hosted connectors listed only in the Claude, ChatGPT or Gemini directories were not checked. Absence of an official integration (e.g. Jobber, ServiceTitan, Clio, Procore, Gusto, Calendly, GoHighLevel) is therefore **unconfirmed**.
- API-access claims for Dentrix, Vagaro, Jane and others rely on API Evangelist third-party profiles, not vendor docs.
- Not checked at all: mcp.so, smithery.ai, glama.ai, PulseMCP, skills.sh web directory, ChatGPT GPT/app store, Vapi/Retell/Synthflow template marketplaces, Fiverr/Upwork.

## Sources

**MCP Registry (API queries actually run)**
- https://registry.modelcontextprotocol.io/v0/servers?limit=100&version=latest (paginated full dump, 545 pages, 1 Nov 2026)
- https://registry.modelcontextprotocol.io/v0/servers?search=quickbooks
- https://registry.modelcontextprotocol.io/v0/servers?search=jobber (and the same pattern for each product in section A, plus usefulapi, pipeworx, cotlet, mrfentmen, canvas, classroom, highlevel, ghl, dental, receptionist, vapi, retell, booking, com.kajabi, com.planningcenter, com.wix, com.stripe, com.notion, com.zapier, com.monday, com.atlassian, com.paypal.mcp, com.canva.mcp)
- Remote endpoints / websites appearing in registry results: https://kcplumb.com/for-ai-assistants , https://kcplumb.com/mcp , https://www.westernskyhvac.com/api/booking , https://thejohnsonbros.com/mcp , https://delcoplumbernow.com/mcp , https://www.absolutebestair.com/api/mcp , https://kay1electric.ca/mcp/ , https://austinvolts.com/mcp , https://kcvolts.com/mcp , https://inescapable.app/mcp , https://mcp.virohanadentalclinic.com/mcp , https://jgp-mcp.vercel.app , https://usefulapi.io/mindbody/ , https://mindbody.usefulapi.io/mcp , https://pipeworx.io/packs/quickbooks , https://www.receptionistprices.com/mcp/ , https://www.aireceptionistrankings.com/mcp/

**npm registry**
- https://registry.npmjs.org/-/v1/search?text=xero+mcp&size=100 (and the same pattern per product)
- https://registry.npmjs.org/-/v1/search?text=skills&size=10
- https://registry.npmjs.org/-/v1/search?text=@anthropic-ai/mcpb&size=3
- https://registry.npmjs.org/-/v1/search?text=mcp-remote&size=3
- https://registry.npmjs.org/-/v1/search?text=@modelcontextprotocol/server-filesystem&size=3

**GitHub API searches** (`gh api search/repositories` and `search/issues`; queries listed in the text)

**GitHub repositories cited**
- https://github.com/intuit/quickbooks-online-mcp-server
- https://github.com/intuit/quickbooks-claude-plugin.git (from the official marketplace JSON)
- https://github.com/XeroAPI/xero-mcp-server
- https://github.com/square/square-mcp-server
- https://github.com/shipstation/mcp-shipstation-api
- https://github.com/wix/wix-mcp
- https://github.com/oktopeak/clio-mcp
- https://github.com/vishalsachdev/canvas-mcp
- https://github.com/mastanley13/GoHighLevel-MCP
- https://github.com/Automaat/lightroom-mcp
- https://github.com/louiewoof2026/skool-mcp
- https://github.com/mindwear-capitian/followupboss-mcp-server
- https://github.com/Purple-Horizons/printful-mcp
- https://github.com/BuildWithBeacon/housecallpro-mcp
- https://github.com/TylerIlunga/procore-mcp-server
- https://github.com/montrellcruse/servicetitan-mcp
- https://github.com/BusyBee3333/jobber-mcp-2026-complete
- https://github.com/vespo92/MindbodyMCP
- https://github.com/sanjibani/open-dental-mcp
- https://github.com/CryptoCultCurt/appfolio-mcp-server
- https://github.com/jake-ccnh/pco-mcp
- https://github.com/RosenAdvertising/filevine-mcp
- https://github.com/cotletdev/fresha-api-mcp-server
- https://github.com/chrischall/honeybook-mcp
- https://github.com/m190/usefulapi-mcp
- https://github.com/pipeworx-io/mcp-quickbooks
- https://github.com/tomjwc/JaneApp---Reports-Scraper
- https://github.com/EZ-Walk/tutorbird-api
- https://github.com/coreyhaines31/marketingskills
- https://github.com/Imbad0202/academic-research-skills
- https://github.com/evolsb/claude-legal-skill
- https://github.com/skala-io/legal-skills
- https://github.com/openaccountants/openaccountants
- https://github.com/GarethManning/education-agent-skills
- https://github.com/miron-tech/hvac-claude-skills
- https://github.com/miron-tech/realtor-claude-skills
- https://github.com/KRASA-AI/hvac-ai-skills
- https://github.com/emd-ai/trades-claude-skills
- https://github.com/Tuminha/dental-ai-skills
- https://github.com/Gonzih/skills-veterinary
- https://github.com/msg2ai/vacationrental-team-skills
- https://github.com/vpodugu/startup-bookkeeper
- https://github.com/polytheseus/bookkeeper-skills
- https://github.com/alexclowe/awesome-claude-cowork-plugins
- https://github.com/anthropics/skills
- https://github.com/anthropics/knowledge-work-plugins
- https://github.com/anthropics/claude-for-legal
- https://github.com/anthropics/financial-services
- https://github.com/anthropics/k12-teacher-skills
- https://github.com/anthropics/healthcare
- https://github.com/anthropics/claude-plugins-official
- https://github.com/anthropics/claude-plugins-community
- https://github.com/SynthFlowAI/AnthropicPlugin.git (from the official marketplace JSON)
- https://github.com/signcrypt/claude-ops-pack-sampler
- https://github.com/nishidagonyuya/printnest-worksheets-lite
- https://github.com/ismailGunaydn/ToolgenX.github.io
- https://github.com/bv-12345/agent-buyer-pack-preview
- https://github.com/TRivers01/ai-receptionist-templates
- https://github.com/TomHardiman6/ai-receptionist-starter
- https://github.com/dom-ran/voice-receptionist-ai
- https://github.com/codewithmuh/ai-voice-agent
- https://github.com/signalwire-demos/dental
- https://github.com/Ryze-AI-Adgent/open-seo-mcp-skills
- https://github.com/Auriti-Labs/geo-optimizer-skill
- https://github.com/leopard627/fire-your-seo-agency
- https://github.com/firecrawl/llmstxt-generator
- https://github.com/arnabbagxd/Brand-building-skills
- https://github.com/strands-agents/agent-sop
- https://github.com/s0912758806p/agentic-sop-to-work
- https://github.com/charlesdove977/procedure-ops
- https://github.com/FlorianBruniaux/claude-cowork-guide
- https://github.com/microsoft/mcp-for-beginners
- https://github.com/zebbern/claude-code-guide
- https://github.com/modelcontextprotocol/mcpb
- https://github.com/czlonkowski/n8n-mcp
- https://github.com/ogulcanaydogan/eu-ai-act-compliance-kit
- https://github.com/urduaiorg/aiforedu
- https://github.com/AmazingPlugins/shopify-accessibility-fixer-legacy
- https://github.com/tanujrajputdev/shopify-theme-audit-skill
- https://github.com/achrafkarzit11-spec/ai-business-ops-evaluation-toolkit

**READMEs / data files read via raw.githubusercontent.com**
- https://raw.githubusercontent.com/anthropics/knowledge-work-plugins/main/README.md
- https://raw.githubusercontent.com/anthropics/claude-for-legal/main/README.md
- https://raw.githubusercontent.com/anthropics/k12-teacher-skills/main/README.md
- https://raw.githubusercontent.com/anthropics/healthcare/main/README.md
- https://raw.githubusercontent.com/anthropics/financial-services/main/README.md
- https://raw.githubusercontent.com/anthropics/skills/main/README.md
- https://raw.githubusercontent.com/anthropics/claude-plugins-official/main/.claude-plugin/marketplace.json
- https://raw.githubusercontent.com/anthropics/claude-plugins-community/main/.claude-plugin/marketplace.json
- https://raw.githubusercontent.com/api-evangelist/vagaro/main/README.md
- https://raw.githubusercontent.com/api-evangelist/dentrix/main/README.md
- https://raw.githubusercontent.com/api-evangelist/17hats/main/README.md
- https://raw.githubusercontent.com/api-evangelist/pixieset/main/README.md
- https://raw.githubusercontent.com/api-evangelist/jane-app/main/README.md
- https://raw.githubusercontent.com/api-evangelist/glofox/main/README.md
- https://raw.githubusercontent.com/api-evangelist/petexec/main/README.md
- https://raw.githubusercontent.com/api-evangelist/teachable/main/README.md
- https://raw.githubusercontent.com/api-evangelist/kajabi/main/README.md
- https://raw.githubusercontent.com/punkpeye/awesome-mcp-servers/main/README.md
- https://raw.githubusercontent.com/m190/usefulapi-mcp/main/README.md
- https://raw.githubusercontent.com/pipeworx-io/mcp-quickbooks/main/README.md
- https://raw.githubusercontent.com/signcrypt/claude-ops-pack-sampler/main/README.md
- https://raw.githubusercontent.com/bv-12345/agent-buyer-pack-preview/main/README.md
- https://raw.githubusercontent.com/ismailGunaydn/ToolgenX.github.io/main/README.md
- https://raw.githubusercontent.com/nishidagonyuya/printnest-worksheets-lite/main/README.md
- https://raw.githubusercontent.com/alexclowe/awesome-claude-cowork-plugins/main/README.md
- https://raw.githubusercontent.com/tomjwc/JaneApp---Reports-Scraper/main/README.md
- https://raw.githubusercontent.com/EZ-Walk/tutorbird-api/main/README.md

**Paid-product URLs appearing in READMEs**
- https://libertybound0.gumroad.com/l/claude-ops-pack
- https://synishida.gumroad.com/l/printnest-worksheets-pro
- https://www.agentskillpacks.com/products

**GitHub issues cited**
- https://github.com/modelcontextprotocol/servers/issues/64
- https://github.com/anthropics/claude-ai-mcp/issues/664
- https://github.com/anthropics/claude-ai-mcp/issues/476
- https://github.com/anthropics/claude-ai-mcp/issues/491
- https://github.com/anthropics/claude-ai-mcp/issues/368
- https://github.com/anthropics/claude-ai-mcp/issues/728
- https://github.com/anthropics/claude-ai-mcp/issues/1204
- https://github.com/anthropics/claude-ai-mcp/issues/1207
- https://github.com/anthropics/claude-code/issues/58510
- https://github.com/anthropics/claude-code/issues/92984
- https://github.com/anthropics/claude-code/issues/57371
- https://github.com/anthropics/claude-code/issues/66535
- https://github.com/anthropics/claude-code/issues/61682
- https://github.com/anthropics/claude-code/issues/59854
- https://github.com/anthropics/claude-code/issues/94321
- https://github.com/anthropics/claude-code/issues/56376
- https://github.com/anthropics/claude-code/issues/91394
- https://github.com/anthropics/claude-code/issues/87537
- https://github.com/anthropics/claude-code/issues/103282
- https://github.com/mims-harvard/ToolUniverse/issues/585
- https://github.com/czlonkowski/n8n-mcp/issues/340
- https://github.com/czlonkowski/n8n-mcp/issues/1159
- https://github.com/CherryHQ/cherry-studio/issues/14966
- https://github.com/wevm/incur/issues/275

**Sibling file referenced (not re-verified here):** /home/user/Claude-research/research/phase1/regulation-and-platform-shifts.md
