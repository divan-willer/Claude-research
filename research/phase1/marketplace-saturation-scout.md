# Marketplace saturation scout: where the one-day digital products already compete (status as of 1 Nov 2026)

Phase 1 research, role: marketplace-saturation-scout. Prepared for the solo-founder "10 one-day digital products" project.

> **Read this first: method problem.** The shared WebSearch budget (200 calls per turn, shared by all agents) was already used up when this agent started, so **this agent ran zero web searches.** Every marketplace host tried directly also failed with ENOTFOUND: chromewebstore.google.com, www.notion.com, www.framer.com and www.teacherspayteachers.com. Gumroad, Etsy and Product Hunt were already known to be blocked.
>
> The evidence here therefore comes from five sources:
> 1. **Third-party Gumroad scrape datasets hosted on GitHub**, read as raw CSV: two independent crawls from Aug 2026 and one vendor dataset from Mar 2026.
> 2. **A Chrome Web Store dataset of AI extensions** (Crawlora, Jul 2026 crawl).
> 3. **GitHub search counts**, used as a proxy for free competition.
> 4. **npm registry counts** for MCP servers.
> 5. **Gumroad product links found in GitHub code**, plus marketplace facts **relayed** from the two sibling Phase 1 files (marked "relayed").
>
> **Etsy, Notion's marketplace, Framer's marketplace, TPT, Product Hunt and non-AI Chrome Web Store categories were NOT measured directly.** Verdicts for them are labelled UNVERIFIED or WEAK.

## Executive summary

- **Gumroad is a winner-take-most market, and most listings sell nothing.** An Aug 2026 crawl of 8,311 Gumroad products found **43% have no ratings at all**. The **top 1% of sellers (45 of 4,532) hold 53.1% of all 201,554 ratings**, and the top 10% hold 89.2% ([sujeito-operator dataset](https://github.com/sujeito-operator/gumroad-market-data)). A new seller with no audience should expect zero sales in any crowded term.
- **Saturated on Gumroad (reject as generic products):**
  - Notion templates: 19,818 listings for "notion template", and top results are free products with 27,701 downloads
  - ChatGPT and AI prompt packs: 4,780 listings; the top items are free
  - Canva templates: 3,627 listings, only 88 ratings across the top 10
  - Digital and printable planners, resume templates, budget trackers
  - AI agent templates, CLAUDE.md and Cursor rules, n8n workflows: massive free GitHub supply (e.g. Zie619/n8n-workflows at 57k stars; awesome-cursorrules at 41k stars)
- **AI Chrome extensions are saturated:** 39,241 AI-labelled extensions as of Jul 2026, and only 215 have 100k+ users. AI writing helpers are owned by Grammarly (35M users), Quillbot, DeepL and LanguageTool ([Crawlora](https://github.com/Crawlora-org/ai-browser-extensions-data)).
- **"Thin" on Gumroad often means "dead", not "open".** Spreadsheet niches (bookkeeping, rental property, Airbnb, construction job costing, Etsy-seller bookkeeping) have 2-46 listings but 0-2 ratings in the top 10. Sibling evidence suggests such spreadsheets sell on **Etsy** instead (relayed: 100+-review Etsy bookkeeping sheets at $12-19). **The marketplace must match the format.**
- **Seed 1 (profession-specific Claude kits) shows the best mix of thin supply and proven buyers:**
  - Paid Gumroad kits that have ratings: "Claude Code for Designers" ($70, 42 ratings), "Claude For Lawyers - 360 Claude Prompts" ($39, 11), "PM Operating System in Claude Code" ($49, 6), "50 Claude Use Cases for Architects" ($29, 5).
  - Each profession has only 1-4 paid titles.
  - Several $129-$199.99 Cowork kits for HR, accountants and CFOs have 0 ratings, so price and audience matter.
  - Free GitHub skill packs crowd marketing, legal, education and PM, but are very thin for trades (HVAC, plumbing), insurance and dental.
- **Seeds with thin paid supply but no proof that anyone buys:**
  - chatbot QA kits (2 GitHub repos; no paid listing found)
  - SOP-to-agent converters
  - MCP setup guides for software with near-zero MCP coverage (Dentrix, Dubsado, Vagaro, Podia, HoneyBook, SimplePractice, Acuity)
  - voice-receptionist templates
- **Seeds that are crowded or saturated:**
  - EU AI Act packs: one Gumroad seller alone lists 29 EU-AI-Act-tagged products at $19-49 in a 299-product, apparently AI-generated catalogue, on top of Etsy kits and free templates
  - AI policy packs
  - llms.txt (2,544 GitHub repos)
  - GEO/AI-search kits: free Claude SEO/GEO skills with 25k+ stars
  - brand-voice packs: price anchor $9
- **Seed 4 (accessibility kits) is MODERATE.** Paid template supply is thin, but the category is fenced by free statement generators and overlay/app incumbents.
- **Pricing benchmarks (Gumroad):**
  - Median paid ranking product: $45 (quartiles $24 and $99) per [gumroad-demand-dataset](https://github.com/marcosgcuenta1/gumroad-demand-dataset).
  - Median paid asking price: $18.03 across the whole category tree vs $36.99 across popular searches (sujeito).
  - Claude kits that sell cluster at $29-$70.

## Summary table

Legend:
- **Count method:** "G-scan" = Gumroad's own result count for the search term in the 6 Aug 2026 scan ([marcosgcuenta1](https://github.com/marcosgcuenta1/gumroad-demand-dataset)). Gumroad search is loose, so many hits are off-topic. "G-36" = 36-listing Discover sample, Aug 2026 ([sujeito-operator](https://github.com/sujeito-operator/gumroad-market-data)). "GH" = GitHub repository search total_count on 1 Nov 2026 (fuzzy). "Relayed" = from sibling Phase 1 files, not re-verified.
- **Evidence:** "Top-10 ratings" = sum of rating counts on the first 10 Gumroad results. Ratings require a buyer, so this is the best demand proxy available.

| # | Category | Marketplaces with evidence | Competing products (estimate, method) | Price range seen | Top-seller proof | Main quality gap | Verdict | Evidence | Date |
|---|---|---|---|---|---|---|---|---|---|
| 1 | Notion templates, generic productivity | Gumroad | 19,818 ("notion template", G-scan); 6,889 "notion dashboard"; 4,073 "productivity system" | $0 to $4,999.99; G-36 median paid $76.38 | Free "Second Brain Template": 373 ratings, 27,701 sales; "Headquarters" A$79: 194 ratings | Top slots held by free or incumbent products | SATURATED | STRONG (2 independent scans agree) | Aug 2026 |
| 2 | Notion freelancer OS | Gumroad | Hundreds (inferred from "freelance contract" 165, "proposal template" 583, "invoice template" 892, G-scan) | $47-$149.99 | "Solopreneur Operating System" $149.99: 12 ratings, 272 sales; "Freelancer Business Dashboard" $47: 11 ratings, 31 sales | Generic, not trade-specific | CROWDED | MEDIUM | Aug 2026 |
| 3 | Notion / Sheets CRM | Gumroad | 97 ("crm spreadsheet", G-scan); Notion CRM not measured | $19-$1,800 | Top-10 ratings belong to lead lists, not CRMs (29 total) | Searchers find lead databases, not CRMs | THIN on Gumroad but low demand; Notion marketplace UNVERIFIED | WEAK | Aug 2026 |
| 4 | Notion / Sheets personal finance | Gumroad | 2,280 "personal finance"; 2,114 "budget tracker"; 257 "net worth tracker"; 193 "debt payoff" (G-scan) | $0-$149 | "Ultimate Annual Budget Spreadsheet" ~$21: 66 ratings (G-36) | Demand concentrated in courses, not trackers | SATURATED | STRONG | Aug 2026 |
| 5 | Teacher / study planners | Gumroad | 984 "study planner" (G-scan); TPT not measured | $0-$19 | "Student Life OS" $19: 19 ratings | Unknown | CROWDED (Gumroad); TPT UNVERIFIED | WEAK | Aug 2026 |
| 6 | Wedding planners | Gumroad | 314 (G-scan), but top hits are off-topic | $10-$300 | 20 ratings total across the top 10, none for a wedding planner | Gumroad buyers don't come for this | THIN but dead on Gumroad; Etsy UNVERIFIED | MEDIUM (dead on Gumroad) | Aug 2026 |
| 7 | Therapist practice templates (Notion/Docs) | Etsy (relayed) | Etsy progress-note listing exists (relayed); no count | n/a | n/a | n/a | UNVERIFIED | WEAK | 2026 |
| 8 | Canva social-media templates | Gumroad (+ Etsy relayed) | 3,627 "canva template"; 3,514 "social media templates"; 3,721 "instagram templates" (G-scan) | $4-$97; Canva-mockup median $4.80 | Top Canva item is free (1.2K ratings); paid items mostly fewer than 25 ratings | Race to $5; free dominates | SATURATED | STRONG | Aug 2026 |
| 9 | Budget spreadsheets | Gumroad + Etsy (relayed) | 2,114 "budget tracker" (G-scan); G-36: 16 of 36 zero-rated | $0-$149 | 66 ratings max for a paid sheet | Commodity | SATURATED | STRONG | Aug 2026 |
| 10 | Google Sheets business templates (bookkeeping, inventory, job costing) | Gumroad; Etsy (relayed) | 46 "bookkeeping spreadsheet", 658 "inventory management", 7 "construction job costing", 23 "rental property spreadsheet" (G-scan) | $3-$349 | Gumroad top 10: 0-2 ratings (dead). Etsy: relayed claim of 100+-review sheets at $12-19 | Wrong marketplace on Gumroad | Gumroad THIN and DEAD; Etsy CROWDED (relayed) | MEDIUM | Aug 2026 |
| 11 | Printable / digital planners | Gumroad | 5,460 "digital planner" (G-scan); G-36 "planner printable": 20 of 36 zero-rated, max 16 ratings | $3-$1,500 | Max 16 ratings among printables | Commodity | SATURATED | STRONG | Aug 2026 |
| 12 | Resume / cover-letter templates | Gumroad | 1,892 resume; 753 cover letter (G-scan) | $3-$85 | $20 tech-resume book: 125 ratings; templates single-digit | Lowest-demand categories in sujeito (42% rated) | SATURATED | STRONG | Aug 2026 |
| 13 | SOP templates (generic / vertical) | Gumroad | Only ~6 SOP titles in all three Gumroad samples combined | $0-$49 | Free "House Manager SOP Vault": 12 ratings; "Local SEO SOP" $9: 8 ratings | Few vertical SOP kits | THIN | WEAK (no direct "SOP" search in either crawl) | Aug 2026 |
| 14 | Contract templates (freelance / creative) | Gumroad | 165 "freelance contract" (G-scan); G-36 "legal contract template": 21 of 36 zero-rated | $0-$680; G-36 median paid $72 | "Freelance Design Contract Template" ~$11.55: 106 ratings | Most listings unrated; one dominant seller | MODERATE | MEDIUM | Aug 2026 |
| 15 | AI prompt packs / bundles (Gumroad + Etsy) | Gumroad, Etsy (relayed), GitHub | 4,780 "chatgpt prompts"; 1,261 "midjourney prompts"; 1,458 "prompt engineering" (G-scan); f/prompts.chat free at 175,518 stars | $0-$99 | Top items free: "10k Premium Chatgpt Prompts" 436 ratings at £0; "GPT-4 Engineering Mastery" 1,005 ratings at $0+ | Free beats paid; Etsy reportedly bans raw prompt bundles (relayed) | SATURATED | STRONG | Aug-Oct 2026 |
| 16 | Small-business starter kits / business plans | Gumroad | 2,855 "business plan template"; 106 "ecommerce checklist" (G-scan) | $0-$4,999.99 | 122 ratings total across the top 10 | Generic | CROWDED, low demand | MEDIUM | Aug 2026 |
| 17 | Lesson plans / homeschool curriculum | Gumroad; TPT not measured | 398 "lesson plans", 244 "homeschool curriculum" (G-scan) | $19-$749 | "Blossom & Root Kindergarten" $67: 107 ratings; first-grade bundle $133: 83 ratings | Buyers want full curricula, not one-day products | MODERATE (Gumroad), poor one-day fit; TPT UNVERIFIED | MEDIUM | Aug 2026 |
| 18 | Cursor rules packs | Gumroad links (GitHub code), GitHub | GH topic:cursor-rules 653; "cursorrules" 523; PatrickJS/awesome-cursorrules 41,080 stars; 0 "cursor" titles in rated Gumroad samples | Not visible | None found | Free and abundant; dev buyers | SATURATED (free) | MEDIUM | Nov 2026 |
| 19 | Claude Code skills / plugins (generic, dev) | Gumroad, GitHub, skill marketplaces | GH topic:claude-skills 13,838; topic:agent-skills 40,050; 1,115 Gumroad hits for "claude code" (G-scan) | $0-$60 typical | "MY PREMIUM CLAUDE SKILLS COLLECTION" $60: 12 ratings; "Claude Skills Pack" $39: 5 | Free official/awesome repos (anthropics/skills 186k stars) | SATURATED | STRONG | Aug-Nov 2026 |
| 20 | **Claude/Cowork kits for one named non-dev profession (seed 1)** | Gumroad, GitHub | 1-4 paid Gumroad titles per profession in samples (lawyers 4, architects 2, PM 1, HR 1, accountants/CFO 2, Amazon sellers 1); free GH packs vary (see entry) | $19.99-$199.99 | Designers $70: 42 ratings; lawyers $39: 11; PM $49: 6; architects $29: 5; HR $129, accountant $199.99, Amazon $19.99: 0 | Many are prompt lists, not installable skills; high prices get 0 ratings | THIN-MODERATE with buyers (best seed) | MEDIUM | Aug 2026 |
| 21 | CLAUDE.md templates | Gumroad link, GitHub | GH 680 repos; one free "single CLAUDE.md file" repo at 227,941 stars | Not visible | None found | Free beats paid | SATURATED (free) | MEDIUM | Nov 2026 |
| 22 | n8n workflow templates | Gumroad, GitHub | GH: Zie619/n8n-workflows 57,156 stars; enescingoz (280+ free) 26,217 stars; n8n-as-code lists 7,700+ templates; topic:n8n-workflow 1,908 | ~$7-$99 | Max 2 ratings among n8n titles in Gumroad samples | Free libraries; YouTubers give packs away free | SATURATED | STRONG | Aug-Nov 2026 |
| 23 | Make.com / Zapier templates | Gumroad, GitHub | GH 5 (Make), 54 (Zapier); 1 Gumroad title in samples (0 ratings) | ~$10 | None | Low supply and no demand proof | THIN, no buyers seen | WEAK | Aug-Nov 2026 |
| 24 | Framer templates | Gumroad; Framer marketplace not measured | 590 "framer template" (G-scan), top hits mostly non-Framer | $20-$179; median $94 | 51 ratings total across the top 10 | Framer buyers buy on Framer's own marketplace | Gumroad low demand; Framer UNVERIFIED | WEAK | Aug 2026 |
| 25 | Figma UI kits | Gumroad | 1,499 "figma ui kit" (G-scan); "Design > UI & Web > Figma" 27 of 44 rated | $0-$1,299; median ~$99-$117 | Untitled UI $129: 1,558 ratings; Nucleus UI $99: 62 ratings, 583 sales | Incumbents; needs real design skill | CROWDED (alive but owned) | STRONG | Aug 2026 |
| 26 | AI agent templates | Gumroad, GitHub | 1,772 "ai agents" (G-scan); GH 4,618 "ai agent templates" repos since Nov 2025 | $9-$199.99 | 98 ratings total across the top 10, mostly off-topic | Abstract, dev-oriented | SATURATED, low demand | MEDIUM | Aug-Nov 2026 |
| 27 | **Voice receptionist / voice-agent templates (seed 6)** | Gumroad links, GitHub | GH: 36 "vapi template", 9 "retell ai template", 1,352 "voice receptionist" since Nov 2025; Gumroad: several build guides plus 11 voice-governance packs from one seller | $17-$49 | "AI Voice Assistant - Complete Setup & Build Guide" $17: 1 rating; no rated receptionist template found | Builder-focused; nothing per trade or clinic | THIN paid supply, no buyer proof | WEAK | 2026 |
| 28 | **MCP connectors / setup guides (seed 5)** | GitHub, npm, Gumroad links | Varies by software: QuickBooks 152 GH / 6 npm; Xero 97 / 11 (incl. official); Shopify 776; GoHighLevel 96; Dentrix, Dubsado, Vagaro, Podia 0; HoneyBook, SimplePractice, kvCORE 1 | Not visible | 1 MCP title in Gumroad samples: 1 rating | No setup guides for non-technical owners | SATURATED for big platforms; THIN for niche ones, demand unproven | MEDIUM (supply), WEAK (demand) | Nov 2026 |
| 29 | **GEO / AI-search kits (seed 2)** | Gumroad, Payhip, Framer (relayed), GitHub | GH 748 "generative engine optimization"; 1,377 "GEO audit" since Nov 2025; free claude-seo skill 25,454 stars | $9-$39 (paid kits) | No rated GEO kit in Gumroad samples | Results unprovable; free skills | CROWDED | MEDIUM | 2026 |
| 30 | Accessibility checker extensions | GitHub only | GH 15 open-source repos; CWS not measured | n/a | n/a | n/a | UNVERIFIED | WEAK | 2026 |
| 31 | AI writing helper extensions | Chrome Web Store (Crawlora data) | 39,241 AI-labelled extensions; 215 with 100k+ users | n/a | Grammarly 35M users, 43,097 ratings; Quillbot 5M; DeepL 4M; LanguageTool 2M | Incumbents | SATURATED | MEDIUM-STRONG | Jul 2026 |
| 32 | SEO / AI-SEO extensions | GitHub, Gumroad | GH 235 "seo chrome extension" since Nov 2025; G-36 "seo tool": 20 of 36 rated | ~$13-$289 | "GeoImgr Pro" $12.90/mo: 184 ratings | Crowded with free tools | CROWDED | WEAK | 2026 |
| 33 | LinkedIn AI extensions | GitHub | GH 280 since Nov 2025 | n/a | n/a | n/a | CROWDED (lean) | WEAK | 2026 |
| 34 | Etsy seller extensions / tools | GitHub, Gumroad, relayed | GH 71; Gumroad "Super Spy HeyEtsy" $19: 80 ratings; relayed: eRank, Marmalead, Alura, and Etsy's own AI | $19+ | 80 ratings (Super Spy) | Platform building it natively (relayed) | SATURATED | MEDIUM | 2026 |
| 35 | Shopify helper extensions | GitHub | GH 79 since Nov 2025 | n/a | n/a | n/a | CROWDED (lean) | WEAK | 2026 |
| 36 | ChatGPT / AI chat exporters | GitHub, Gumroad | GH 214; Gumroad "AI Chat Exporter" $7: 2 ratings | ~$7 | 2 ratings | Free everywhere | SATURATED | MEDIUM | 2026 |
| 37 | AI detector extensions | GitHub | GH 213 | n/a | n/a | Accuracy disputes | CROWDED (lean) | WEAK | 2026 |
| 38 | Review-reply extensions / tools (GBP) | GitHub | GH 133 "google review reply ai"; a free MV3 extension and a GBP MCP server exist | n/a | n/a | n/a | MODERATE (lean) | WEAK | 2026 |
| 39 | Invoice extensions / templates | GitHub, Gumroad | GH 70 (mostly order exporters); 892 "invoice template" (G-scan), 44 ratings across the top 10 | $49-$349 | None strong | Low demand on Gumroad | CROWDED, low demand | WEAK | Aug 2026 |
| 40 | Chrome extensions sold on Gumroad (any) | Gumroad | G-36 "chrome extension": 28 of 36 rated, median paid $19.99 | $0-$60 | "CSS Scan" ~$49: 205 ratings; "PhotoSolve PRO" $60/yr: 178 | Alive but owned by dev-tool sellers | CROWDED | MEDIUM | Aug 2026 |
| 41 | **School AI policy packs (seed 9)** | GitHub, Gumroad links, relayed TPT/Tes | GH 74; free model policies (relayed: Tes, Third Space Learning, Kuraplan, state models); one Gumroad seller's school governance packs at $29-$49 | $29-$49 | None found | Free official templates | CROWDED by free; TPT UNVERIFIED | MEDIUM (relayed) | 2026 |
| 42 | AI lesson plans | GitHub; TPT not measured | GH 237 "lesson plan generator" since Nov 2025; GarethManning/education-agent-skills: 165 free teacher skills, 939 stars | n/a | n/a | n/a | UNVERIFIED (lean CROWDED) | WEAK | 2026 |
| 43 | AI literacy units / kits | Gumroad link; TPT not measured | ≥1 Gumroad kit (probiex ai-literacy-kit) | n/a | n/a | n/a | UNVERIFIED | WEAK | 2026 |
| 44 | **EU AI Act templates (seed 3)** | Etsy (relayed), Gumroad, GitHub | Etsy kits $12.99-$131.27 (relayed); one Gumroad seller has 29 EU-AI-Act-tagged products; GH 59 "eu ai act template"; 1,125 repos since Jan 2026 (relayed) | $12.99-€990 | None visible | Mass-generated; duty softened (relayed) | SATURATED | STRONG | Oct 2026 |
| 45 | SMB AI acceptable-use policy templates | Etsy (relayed), Gumroad, GitHub | One Gumroad catalogue alone has 59 policy-tagged products; GH 9 free templates; Etsy "ai policies" market (relayed) | $19-$49 | None visible | Generic, not vertical | CROWDED | MEDIUM | Oct 2026 |
| 46 | **Accessibility statement / fix kits (seed 4)** | Gumroad, GitHub, npm, relayed | Gumroad statement template (relayed); "Accessibility Compliance Quickstart" $19; GH 17 statement generators, 88 "shopify accessibility" repos; free generators (relayed) | $19+ | None visible | Platform-specific manual-fix guides scarce | MODERATE | MEDIUM | 2026 |
| 47 | llms.txt files / generators | GitHub, Gumroad link | GH 2,544 llms.txt repos; 173 generators since Nov 2025; paid "llmstxt-pro" on Gumroad | n/a | n/a | No measurable effect (relayed) | SATURATED (free) | STRONG | Nov 2026 |
| 48 | **Brand voice packs / prompts (seed 7)** | Gumroad, Claw Mart, GitHub | GH 216 "brand voice skill" since Nov 2025; Brand-building-skills free (821 stars); paid "Brand Voice Extractor" $9 on Gumroad and $9 on Claw Mart | $9 | 0 brand-voice titles in rated Gumroad samples | Price anchored at $9 | CROWDED, low ceiling | MEDIUM | 2026 |
| 49 | **Chatbot test / QA kits (seed 8)** | GitHub | GH 2 "chatbot testing checklist" repos (both free); 70 "chatbot test cases" since Nov 2025; no paid listing found | n/a | none | Dev tools exist; nothing for SMB owners | THIN, no buyer proof | WEAK | 2026 |
| 50 | **SOP-to-agent converters (seed 10)** | GitHub, Gumroad (free lead magnet) | GH 81 "sop to skill"; 11 "sop agent instructions" since Nov 2025; a free "One-Shot Skill Creation Prompt" (SOP from screen recording) on Gumroad | $0 | none | Free lead magnets | THIN paid, no buyer proof | WEAK | 2026 |
| 51 | Niche business-model templates (OKR, SaaS metrics, real-estate model, retirement calculator, Zettelkasten) | Gumroad | 135 OKR; 206 SaaS metrics; 239 real-estate model; 36 retirement calculator; 82 Zettelkasten (G-scan) | varies | Top-10 ratings: 120 / 95 / 78 / 152 / 87 | Ratings often come from 1-3 products | MODERATE with buyers | MEDIUM | Aug 2026 |
| 52 | Copywriting swipe files | Gumroad | 98 listings (G-scan) | varies | 28 ratings total across the top 10; 7 of 10 rated | Unknown | THIN-MODERATE with buyers | WEAK-MEDIUM | Aug 2026 |

---

## Detailed entries

### A. Cross-cutting marketplace facts (read before any single category)

1. **Gumroad demand is extremely concentrated.**
   - Of 8,311 products crawled across Gumroad's category tree in Aug 2026, 3,562 (43%) had no ratings.
   - 3,251 of 4,532 sellers (71.7%) had a single product.
   - 1,710 sellers (38%) had no ratings across their whole catalogue.
   - The top 1% of sellers held 53.1% of all ratings and the top 10% held 89.2% ([sujeito-operator/gumroad-market-data](https://github.com/sujeito-operator/gumroad-market-data)).
   - A vendor dataset (InsightRaider, Mar 2026) claims the top 1% of products capture 77.3% of estimated revenue, and that unrated products average 18 sales vs 1,197 for 4.5-4.9-star products ([Pinous/gumroad-market-data](https://github.com/Pinous/gumroad-market-data)). That is a WEAK, vendor revenue estimate.
   - **Implication:** "few competitors" is not enough. The founder needs a channel that brings buyers, because Gumroad Discover alone will not.
2. **Ratings vs sales.** In the 229 listings showing both, the median paid listing sold about ×25.5 its rating count (middle half ×11.7 to ×54.2), with rank correlation 0.784 ([sujeito-operator](https://github.com/sujeito-operator/gumroad-market-data)). That sample is 57% 3D assets, and the author warns against generalising. Use it only as a rough order of magnitude: a product with 5 ratings has plausibly sold dozens of units, not thousands.
3. **Price benchmarks:**
   - The median price of a paid product ranking on a first page was $45 (quartiles $24 and $99). Only 31 of 715 ranking products were free or pay-what-you-want ($0+), but those dominate downloads ([marcosgcuenta1](https://github.com/marcosgcuenta1/gumroad-demand-dataset)).
   - Median paid asking price was $18.03 across the category tree and $36.99 across popular searches ([sujeito-operator](https://github.com/sujeito-operator/gumroad-market-data)).
   - The scan author's conclusion: "The live niches need a skill, not a template... The dead ones are the ones where producing something means opening a blank spreadsheet" ([marcosgcuenta1](https://github.com/marcosgcuenta1/gumroad-demand-dataset)).
4. **Gumroad search is loose.** The scan counted 1,115 Gumroad results for "claude code", but the top three were ZimmWriter, a Houdini AI assistant and a macOS window tool. Treat G-scan listing counts as an upper-bound noise measure, not a competitor count ([gumroad-demand.csv](https://raw.githubusercontent.com/marcosgcuenta1/gumroad-demand-dataset/HEAD/gumroad-demand.csv)).
5. **AI-generated catalogue flooding is real.** A single Gumroad seller ("ghostcorpnet") published a 299-product catalogue (generated 2 Oct 2026) with a median price of $19 and a range of $0-$299. It is heavy on AI governance: 29 products match "EU AI Act" by name or tag, 11 match voice agents, 2 school, 2 accessibility ([catalog.json](https://raw.githubusercontent.com/koalstingkdelaney-gif/kestrelattice/HEAD/ai/catalog.json)). Expect compliance-template niches to fill quickly with similar mass-produced supply. Sales for this catalogue are unknown.
6. **YouTube creators give away what others try to sell.** The Early AI-dopters repo mirrors "Every free resource from the Early AI-dopters Gumroad" (198 published resources, synced 1 Nov 2026). These include Claude skills, n8n workflows, MCP guides and a skill-from-SOP prompt ([earlyaidopters/gumroad-resources](https://github.com/earlyaidopters/gumroad-resources)). In AI-tooling categories, much of the Gumroad "supply" is $0 lead magnets.

### B. Notion templates

**1. Generic productivity (SATURATED, STRONG, Aug 2026).**
- "notion template" returned 19,818 Gumroad products, with 685 ratings across the top 10 (3.5 per 100 listings).
- "notion dashboard" returned 6,889 and "productivity system" 4,073.
- The #1 result is the free "Second Brain Template" (373 ratings, 27,701 sales), and the free "Notion Life OS" has 167 ratings and 11,857 sales ([gumroad-demand.csv](https://raw.githubusercontent.com/marcosgcuenta1/gumroad-demand-dataset/HEAD/gumroad-demand.csv)).
- The independent G-36 sample: 26 of 36 rated, 1,422 total ratings, median paid $76.38, top paid "Business Hub for Notion" at $99 with 145 ratings ([sujeito gumroad-latest.csv](https://github.com/sujeito-operator/gumroad-market-data)).
- **Gap:** none worth chasing; free incumbents own it.
- **Not measured:** Notion's own template marketplace (host blocked).

**2. Freelancer OS (CROWDED, MEDIUM).**
- Freelancer dashboards sit among hundreds of generic hits.
- "The Solopreneur Operating System" ($149.99) has 12 ratings and 272 sales; "Freelancer Business Dashboard" ($47) has 11 ratings and 31 sales ([gumroad-demand.csv](https://raw.githubusercontent.com/marcosgcuenta1/gumroad-demand-dataset/HEAD/gumroad-demand.csv)).
- **Gap:** generic "freelancer" positioning. Trade-specific OS kits (e.g. cleaner or photographer) were not measured here. The sibling pain-hunter file relays competing Etsy/Gumroad cleaning-business templates ([Etsy cleaning CRM](https://www.etsy.com/listing/1733890901/cleaning-business-crm-client-task), [Gumroad cleaning toolkit](https://cleanstrong.gumroad.com/l/ecfyg)), relayed.

**3. CRM (THIN on Gumroad, low demand; Notion marketplace UNVERIFIED; WEAK).**
- "crm spreadsheet" returned 97 products. The top-10 ratings (29) belong to lead lists and investor databases, not CRM templates ([gumroad-demand.csv](https://raw.githubusercontent.com/marcosgcuenta1/gumroad-demand-dataset/HEAD/gumroad-demand.csv)).

**4. Finance (SATURATED, STRONG).**
- Listings: "personal finance" 2,280 (946 top-10 ratings), "budget tracker" 2,114 (87), "net worth tracker" 257 (24), "debt payoff" 193 (55) ([gumroad-demand.csv](https://raw.githubusercontent.com/marcosgcuenta1/gumroad-demand-dataset/HEAD/gumroad-demand.csv)).
- In G-36 "budget spreadsheet", 16 of 36 listings were unrated. The best paid sheet ("Ultimate Annual Budget Spreadsheet", ~$21) had 66 ratings ([sujeito](https://github.com/sujeito-operator/gumroad-market-data)).

**5. Teacher planner (UNVERIFIED, WEAK).**
- "study planner" had 984 Gumroad listings and 85 top-10 ratings. TPT was not reachable.

**6. Wedding planner (THIN but dead on Gumroad, MEDIUM).**
- 314 listings, but the top-10 hits are off-topic (an AI prompt mega-pack, wedding-march sheet music), with 20 ratings total ([gumroad-demand.csv](https://raw.githubusercontent.com/marcosgcuenta1/gumroad-demand-dataset/HEAD/gumroad-demand.csv)). Etsy is the likely venue; not measured.

**7. Therapist practice (UNVERIFIED, WEAK).**
- The only marketplace datum is a relayed Etsy progress-note listing ([Etsy](https://www.etsy.com/listing/4432325264/progress-note-samples-documentation)). No count.

### C. Etsy-style digital downloads (Etsy itself not measured; Gumroad as proxy)

**8. Canva social templates (SATURATED, STRONG).**
- Gumroad listings: "canva template" 3,627 (88 top-10 ratings, 2.4 per 100), "social media templates" 3,514, "instagram templates" 3,721 ([gumroad-demand.csv](https://raw.githubusercontent.com/marcosgcuenta1/gumroad-demand-dataset/HEAD/gumroad-demand.csv)).
- In G-36, the top Canva item is free with 1.2K ratings. In the category tree, "Design > Graphics > Mockups > Canva" has a median price of $4.80 and "Print & Packaging > Canva" $6.00 ([sujeito](https://github.com/sujeito-operator/gumroad-market-data)).
- The sibling file also judged Canva packs "very crowded" (relayed).

**9. Budget spreadsheets (SATURATED, STRONG):** see #4.

**10. Google Sheets business templates (Gumroad: THIN and DEAD; Etsy: CROWDED, relayed; MEDIUM).**
- "Measured, and dead" terms, meaning 5 or fewer ratings across the whole first page ([marcosgcuenta1](https://github.com/marcosgcuenta1/gumroad-demand-dataset)):

  | Term | Listings | Top-10 ratings |
  |---|---|---|
  | bookkeeping spreadsheet | 46 | 1 |
  | rental property spreadsheet | 23 | 2 |
  | Airbnb spreadsheet | 9 | 1 |
  | construction job costing | 7 | 2 |
  | Etsy seller bookkeeping | 2 | 0 |

- G-36 "excel dashboard": 22 of 36 unrated ([sujeito](https://github.com/sujeito-operator/gumroad-market-data)).
- The scan's author built products for four of these dead terms and "sold nothing" ([marcosgcuenta1](https://github.com/marcosgcuenta1/gumroad-demand-dataset)).
- **Counter:** an Indie Hackers commenter (relayed by pain-hunter) says similar Etsy bookkeeping sheets carry 100+ reviews at $12-19 ([IH](https://www.indiehackers.com/post/built-a-finance-kit-for-freelancers-three-weeks-live-0-revenue-3c667a7111)). UK MTD spreadsheets are already listed on Etsy (relayed: [Etsy 4567179604](https://www.etsy.com/listing/4567179604/)).
- **Takeaway:** spreadsheets belong on Etsy, not Gumroad.

**11. Printable planners (SATURATED, STRONG).**
- "digital planner" had 5,460 Gumroad listings.
- In G-36 "planner printable", 20 of 36 were unrated and the best had 16 ratings ([sujeito](https://github.com/sujeito-operator/gumroad-market-data)).

**12. Resume templates (SATURATED, STRONG).**
- 1,892 listings. The only well-rated item is a $20 book (125 ratings), and template listings have single-digit ratings ([gumroad-demand.csv](https://raw.githubusercontent.com/marcosgcuenta1/gumroad-demand-dataset/HEAD/gumroad-demand.csv)).
- The category tree ranks resume template among the lowest-demand categories (42% rated) ([sujeito](https://github.com/sujeito-operator/gumroad-market-data)).
- Free GitHub resume builders also abound (3,503 "resume template" repos created since Nov 2025; GH search).

**13. SOP templates (THIN, WEAK).**
- Only about 6 SOP-titled products appeared across both crawls. The best were the free "House Manager SOP Vault" (12 ratings), "Complete Local SEO SOP" at $9 (8 ratings) and "Complete E-Commerce SEO SOP" at $9+ (2) ([gumroad-demand.csv](https://raw.githubusercontent.com/marcosgcuenta1/gumroad-demand-dataset/HEAD/gumroad-demand.csv)).
- Neither crawl searched "SOP" directly, so supply is under-sampled.
- Trainual sells SOP templates (relayed, [Trainual](https://trainual.com/solution/sop-templates)).

**14. Contract templates (MODERATE, MEDIUM).**
- "freelance contract" returned 165 listings with 66 top-10 ratings.
- In G-36 "legal contract template", 21 of 36 were unrated, but one "Freelance Design Contract Template" (~$11.55) had 106 ratings ([sujeito](https://github.com/sujeito-operator/gumroad-market-data)).
- **Gap:** most listings sell nothing, while one cheap, specific one sells well.
- **Risks:** legal liability and unauthorized-practice issues (not researched). Pain-hunter relays a founder whose contract templates were displaced by Claude itself ([IH](https://www.indiehackers.com/post/claude-ate-my-products-main-feature-i-kept-the-part-it-can-t-eat-b2596a6a36)).

**15. ChatGPT / AI prompt bundles (SATURATED, STRONG).**
- Gumroad listings: "chatgpt prompts" 4,780, "midjourney prompts" 1,261, "prompt engineering" 1,458, "ai prompts" (G-36) 32 of 36 rated.
- The most-rated items are free: "GPT-4 Engineering Mastery 2.0" (1,005 ratings, $0+), "10k Premium Chatgpt Prompts" (436 ratings, £0) and "Claude Mastery Guide" (168 ratings, $0, 10,668 sales) ([gumroad-demand.csv](https://raw.githubusercontent.com/marcosgcuenta1/gumroad-demand-dataset/HEAD/gumroad-demand.csv), [sujeito](https://github.com/sujeito-operator/gumroad-market-data)).
- The free f/prompts.chat (formerly Awesome ChatGPT Prompts) has 175,518 GitHub stars (GH search).
- Etsy reportedly prohibits raw AI prompt bundles (relayed: [inkfluenceai Oct 2026](https://www.inkfluenceai.com/blog/etsy-ai-rules-update-october-2026)).
- Pain-hunter relays $57 and $54 outcomes for generic Claude/prompt packs ([IH $57](https://www.indiehackers.com/post/i-made-57-in-48-hours-selling-claude-cheat-codes-here-s-what-worked-and-what-didn-t-01d7f1f61c), [IH $54](https://www.indiehackers.com/post/i-am-an-autonomous-ai-agent-10-weeks-2-sales-54-here-is-what-i-actually-learned-300698bdfe)).

**16. Small-business starter kits (CROWDED, low demand, MEDIUM).**
- "business plan template" returned 2,855 listings with only 122 top-10 ratings; "ecommerce checklist" returned 106 with 16 ([gumroad-demand.csv](https://raw.githubusercontent.com/marcosgcuenta1/gumroad-demand-dataset/HEAD/gumroad-demand.csv)).

**17. Lesson plans (Gumroad MODERATE, poor one-day fit; TPT UNVERIFIED).**
- "lesson plans" returned 398 listings with 261 top-10 ratings, dominated by full curricula ("Blossom & Root Kindergarten" $67, 107 ratings; "First Grade Full Bundle" $133, 83 ratings). "homeschool curriculum" returned 244 listings with 170 ratings ([gumroad-demand.csv](https://raw.githubusercontent.com/marcosgcuenta1/gumroad-demand-dataset/HEAD/gumroad-demand.csv)).
- "Education > Classroom" in the category tree: 27 of 44 rated, median $18.45 ([sujeito](https://github.com/sujeito-operator/gumroad-market-data)).
- TPT comment banks are typically under $15 per grade (relayed: [TPT search](https://www.teacherspayteachers.com/Browse/Search:report%20card%20comment%20bank)).

### D. Gumroad developer / AI-tooling categories

**18. Cursor rules (SATURATED by free supply, MEDIUM).**
- GitHub: topic:cursor-rules has 653 repos, "cursorrules" matches 523, and PatrickJS/awesome-cursorrules has 41,080 stars (GH search, 1 Nov 2026).
- Paid Gumroad listings exist (found in GitHub code): [goodepochhq cursor-rules](https://goodepochhq.gumroad.com/l/cursor-rules), [nedcodes cursor-doctor-pro](https://nedcodes.gumroad.com/l/cursor-doctor-pro), [blncraft vibe-coder-kit](https://blncraft.gumroad.com/l/vibe-coder-kit).
- No Cursor product appeared among rated titles in either Gumroad crawl. Buyers are developers, not the target buyer.

**19. Claude Code skills / plugins, generic (SATURATED, STRONG).**
- GitHub: topic:claude-skills has 13,838 repos and topic:agent-skills 40,050. Plugin repos created since Nov 2025 number 34,053.
- Free aggregators include:
  - anthropics/skills (186,297 stars)
  - anthropics/claude-plugins-official (45,699)
  - ComposioHQ/awesome-claude-skills (78,512)
  - sickn33/agentic-awesome-skills ("2,884+ reusable AI agent skills")
  - VoltAgent/awesome-openclaw-skills ("5,400+ skills")
- Gumroad paid examples: "MY PREMIUM CLAUDE SKILLS COLLECTION" $60 (12 ratings) ([usamaakrm](https://usamaakrm.gumroad.com/l/premium-claude-skills)), "Claude Skills Pack" $39 (5) ([thinkaiprompt](https://thinkaiprompt.gumroad.com/l/claude-skills)), "Claude OS" $47 (33) ([yourchatgptguide](https://yourchatgptguide.gumroad.com/l/ClaudeOS)) ([gumroad-demand.csv](https://raw.githubusercontent.com/marcosgcuenta1/gumroad-demand-dataset/HEAD/gumroad-demand.csv)).
- Dedicated skill marketplaces exist:
  - Claw Mart ([BrianRWagner README](https://github.com/BrianRWagner/ai-marketing-claude-code-skills) links a $9 listing)
  - Agensi, SkillHQ and KissMySkills (relayed by the regulation file)
  - a 167-skill $167 bundle on Gumroad (relayed: [inflectual](https://inflectual.gumroad.com/l/master-marketing-claude-skills-bundle))

**20. Claude / Cowork kits for one named non-developer profession: seed 1 (THIN-MODERATE with buyers; MEDIUM; Aug 2026).**

Paid Gumroad titles in the two crawls (ratings in parentheses) ([gumroad-demand.csv](https://raw.githubusercontent.com/marcosgcuenta1/gumroad-demand-dataset/HEAD/gumroad-demand.csv), [sujeito](https://github.com/sujeito-operator/gumroad-market-data)):

| Profession | Product | Price | Ratings |
|---|---|---|---|
| Designers | "Claude Code for Designers" ([link](https://aidesignlab.gumroad.com/l/claude-code-for-designers)) | ~$70 | 42 |
| Lawyers | "Claude For Lawyers - 360 Claude Prompts" ([link](https://kumail.gumroad.com/l/360l)) | $39 | 11 |
| Lawyers | "The Lawyer's Guide to Claude Fable 5" | ~$39 | 3 |
| Lawyers | "The Biglaw Guide To Claude" | ~$39 | 1 |
| Lawyers | multi-model "Prompts for Lawyers" | ~$100 | 0 |
| Product managers | "PM Operating System in Claude Code" ([link](https://growthpioneer.gumroad.com/l/pmos)) | $49 | 6 |
| Job seekers | "Job Search OS in Claude Code" ([link](https://growthpioneer.gumroad.com/l/jobsearchos)) | $49 | 5 |
| Architects | "50 Claude Use Cases for Architects" ([link](https://arjunechow.gumroad.com/l/claude)) | $29 | 5 |
| Architects | "Claude for Architects" masterclass + skills | ~$99 | 0 |
| Consultants | "The Consultant's Guide To Claude Skills" | $39 | 2 |
| HR | "Onboarding Claude Cowork for HR A-Z" | ~$129 | 0 |
| Accountants | "Claude Cowork for Accountant" ([link](https://ismailsaleem.gumroad.com/l/How-Accountant-Can-Use-Claude-Cowork-Powerful-Use-Cases)) | $199.99 | 0 |
| CFOs | "Claude Cowork for Chief Financial Officer (CFO)" | $199.99 | 0 |
| Amazon sellers | "8 Claude Skills for Amazon Sellers" | ~$19.99 | 0 |
| eLearning | "Claude Code for eLearning" | ~$48.70 | 0 |
| Substack writers | "Claude AI Bundle for Substack" | ~$69 | 0 |

- **Reading:**
  - There are 1-4 paid titles per profession, so supply is thin.
  - Rated titles sit at $29-$70.
  - The $129-$199.99 Cowork kits have zero ratings.
  - The two growthpioneer kits appear to belong to a creator with an existing audience (seller display name "Aakash Gupta" in the crawl). Audience, not search, probably drove those sales (inference).
- **Free competition by profession** (GitHub search, 1 Nov 2026; fuzzy):

  | Profession | Free GitHub supply |
  |---|---|
  | Marketing | "claude skills marketing" 1,202 repos; coreyhaines31/marketingskills 57,829 stars |
  | Legal | "legal skills claude" 345; evolsb/claude-legal-skill 492 stars |
  | Teachers | 77 repos; GarethManning/education-agent-skills, "165 evidence-grounded AI skills for teachers", 939 stars |
  | Recruiters | 115 |
  | Shopify | 151 |
  | Corporate roles | polar-bear-org/claude-skills: "37 free Claude Skill packs, 1073 skills" covering HR, recruiting, customer service and PM, licensed not for resale ([README](https://github.com/polar-bear-org/claude-skills)); its repo description says 51 packs and 1,178 skills, so the numbers conflict |
  | Real estate | "realtor skills claude" 6 repos (top miron-tech/realtor-claude-skills, 15 stars) |
  | HVAC | "hvac claude" 49 fuzzy hits; the actual HVAC skill repos have 3-6 stars (miron-tech/hvac-claude-skills, KRASA-AI/hvac-ai-skills) |
  | Insurance agents | 2 |
  | Accountants | "accountant skills claude" 14 |
  | Therapists | 36 hits, mostly unrelated "therapist for Claude" toys |
  | Dental | 114 fuzzy hits; Tuminha/dental-ai-skills has 7 stars |
  | Etsy sellers | 8 |

- **Verdict:** white-collar knowledge professions (marketing, legal, education, PM, HR) are CROWDED by free GitHub packs. **Trades, insurance, dental and bookkeeping offices are THIN**, but no paid kit for them showed ratings in these crawls, so demand there is unproven.

**21. CLAUDE.md templates (SATURATED by free supply, MEDIUM).**
- GitHub: 680 repos match "CLAUDE.md template". multica-ai/andrej-karpathy-skills ("A single CLAUDE.md file...") has 227,941 stars (GH search).
- Paid example: [echochime3 claudemd-bible](https://echochime3.gumroad.com/l/claudemd-bible) (found in GitHub code).

**22. n8n workflow templates (SATURATED, STRONG).**
- Free supply (GH search):
  - Zie619/n8n-workflows: 57,156 stars
  - enescingoz/awesome-n8n-templates ("280+ free n8n automation templates"): 26,217 stars
  - wassupjay/n8n-free-templates ("200+"): 6,243 stars
  - Danitilahun ("2,053 n8n workflows")
  - EtienneLescot/n8n-as-code ("7,700+ templates")
- Paid demand is weak: the three n8n titles in the Gumroad crawls had 0-2 ratings ([gumroad-demand.csv](https://raw.githubusercontent.com/marcosgcuenta1/gumroad-demand-dataset/HEAD/gumroad-demand.csv), [sujeito](https://github.com/sujeito-operator/gumroad-market-data)).
- Paid packs seen via GitHub code: [studioddx n8n-workflow-mega-pack](https://studioddx.gumroad.com/l/n8n-workflow-mega-pack), [viktorgubanov telegram template](https://viktorgubanov.gumroad.com/l/n8n-telegram-bot-template).
- Many of markkashef's n8n items are free lead magnets ([earlyaidopters/gumroad-resources](https://github.com/earlyaidopters/gumroad-resources)).

**23. Make.com / Zapier templates (THIN, no buyers seen, WEAK).**
- GitHub: 5 "make.com scenario templates" repos and 54 "zapier templates" (GH search).
- One Gumroad crawl title, "350 n8n AI Agents and make.com automations" (~$10), had 0 ratings.
- Make's and Zapier's own template galleries were not checked.

**24. Framer templates (Gumroad low demand; Framer marketplace UNVERIFIED; WEAK).**
- Gumroad: 590 listings and 51 top-10 ratings; median paid $94; top hits are not Framer sites ([gumroad-demand.csv](https://raw.githubusercontent.com/marcosgcuenta1/gumroad-demand-dataset/HEAD/gumroad-demand.csv)).
- A Framer AEO/GEO template exists on Framer's marketplace (relayed: [framer](https://www.framer.com/marketplace/templates/aeo-geo-seo/?via=doug)).

**25. Figma UI kits (CROWDED, alive but owned, STRONG).**
- Gumroad: 1,499 listings, 636 top-10 ratings, median ~$117. "Untitled UI" ($129) has 1,558 ratings, and "Nucleus UI PRO" ($99) has 62 ratings and 583 sales ([gumroad-demand.csv](https://raw.githubusercontent.com/marcosgcuenta1/gumroad-demand-dataset/HEAD/gumroad-demand.csv)).
- Category tree: "Design > UI & Web > Figma" 27 of 44 rated, median $99.14 ([sujeito](https://github.com/sujeito-operator/gumroad-market-data)).
- Needs real design skill; a poor one-day fit.

**26. AI agent templates (SATURATED, low demand, MEDIUM).**
- Gumroad "ai agents": 1,772 listings but only 98 top-10 ratings (5.5 per 100), mostly off-topic ([gumroad-demand.csv](https://raw.githubusercontent.com/marcosgcuenta1/gumroad-demand-dataset/HEAD/gumroad-demand.csv)).
- GitHub: 4,618 "ai agent templates" repos created since Nov 2025; mergisi/awesome-openclaw-agents lists "196 production-ready AI agent templates" (GH search).

**27. Voice receptionist / voice-agent templates: seed 6 (THIN paid supply, no buyer proof, WEAK).**
- GitHub (GH search):
  - 36 "vapi template" repos and 9 "retell ai template" repos
  - 1,352 "voice receptionist" repos created since Nov 2025 (top: kirklandsig/AIReceptionist, 153 stars)
  - free starter templates such as dom-ran/voice-receptionist-ai and TomHardiman6/ai-receptionist-starter
  - the regulation file counted 3,426 "ai receptionist" repos in 2026 (relayed)
- Paid listings found via GitHub code:
  - [dialdaddy how-to-build-a-vapi-voice-agent](https://dialdaddy.gumroad.com/l/how-to-build-a-vapi-voice-agent)
  - [tuguidragos ghl-n8n-vapi-ai-calling-agent](https://tuguidragos.gumroad.com/l/ghl-n8n-vapi-ai-calling-agent)
  - [chronoai aireceptionist](https://chronoai.gumroad.com/l/aireceptionist)
  - a "vendor comparison scorecard" for AI receptionist platforms
  - $49 voice-governance packs from ghostcorpnet: "TCPA Consent Playbook for AI Voice Agents", "Call Recording Consent & Retention Pack", "AI Identity Disclosure Pack for Voice Agents" ([catalog.json](https://raw.githubusercontent.com/koalstingkdelaney-gif/kestrelattice/HEAD/ai/catalog.json))
- In the Gumroad crawls, the only voice item was "AI Voice Assistant - Complete Setup & Build Guide" ($17, 1 rating).
- **Gaps:** nothing per trade or clinic (HVAC/dental scripts), nothing for owners rather than builders, and Vapi/Retell native template galleries were not checked.
- **Note:** the compliance-script add-on suggested by the regulation file already has a mass-produced $49 competitor.

**28. MCP connectors / setup guides for niche business software: seed 5 (SATURATED for big platforms, THIN for niche ones; MEDIUM on supply, WEAK on demand).**
- GitHub repos matching "<name> mcp" in name or description (all time / created since 1 May 2026), with npm packages whose name contains the product and mention MCP. Counts are fuzzy; "square", "toast", "monday" and "teachable" are polluted by common words.

  | Software | GitHub (all time / since May 2026) | npm | Supply read |
  |---|---|---|---|
  | Shopify | 776 / 509 | — | Saturated |
  | ClickUp | 211 / 81 | — | Saturated |
  | QuickBooks | 152 / 81 | 6 | Saturated |
  | Airtable | 117 | — | Saturated |
  | Etsy | 115 / 97 | 3 | Saturated |
  | Xero | 97 / 46 | 11, incl. official `@xeroapi/xero-mcp-server` | Saturated |
  | GoHighLevel | 96 / 53 | 3 | Saturated |
  | Pipedrive | 70 | — | Saturated |
  | Calendly | 35 | 4 | Crowded |
  | Clio | 31 | 2 | Crowded |
  | Wix | 27 | 1 (official `@wix/mcp`) | Crowded |
  | FreshBooks | 24 | — | Crowded |
  | ServiceTitan | 20 | 1 | Crowded |
  | Jobber | 19 | 4 | Crowded |
  | Housecall Pro | 14 | 3 | Crowded |
  | Procore | 11 | 0 | Middle |
  | Follow Up Boss | 11 | 0 | Middle |
  | Fresha | 10 | — | Middle |
  | Squarespace | 9 | 0 | Middle |
  | Mindbody | 8 | 3 | Middle |
  | Lawmatics | 8 | — | Middle |
  | AppFolio | 8 | 2 | Middle |
  | Kajabi | 3 | 0 | Thin |
  | Acuity | 3 | 0 | Thin |
  | Buildertrend | 3 | 0 | Thin |
  | Open Dental | 3 | — | Thin |
  | Buildium | 3 | — | Thin |
  | MyCase | 2 | — | Thin |
  | PracticePanther | 2 | — | Thin |
  | Jane | 2 | — | Thin |
  | Boulevard | 2 | — | Thin |
  | HoneyBook | 1 | 1 | Thin |
  | SimplePractice | 1 | 1 | Thin |
  | kvCORE | 1 | — | Thin |
  | Dentrix | 0 | 0 | Thin |
  | Dubsado | 0 | 0 | Thin |
  | Vagaro | 0 | 0 | Thin |
  | Podia | 0 | 0 | Thin |

- Some thin-coverage tools may simply lack public APIs, which would make an MCP impossible. This was not checked.
- Paid MCP guides exist ([markkashef mcpclaude](https://markkashef.gumroad.com/l/mcpclaude), found in GitHub code), but only one MCP title (1 rating) appeared in the Gumroad crawls.
- **Verdict:** supply is thin for niche vertical SaaS, but **no buyer signal was found**.

**29. GEO / AI-search kits: seed 2 (CROWDED, MEDIUM).**
- Free tooling (GH search):
  - 748 repos match "generative engine optimization"
  - 1,377 "GEO audit" repos created since Nov 2025
  - 210 AEO repos
  - AgriciDaniel/claude-seo: 25,454 stars
  - Ryze-AI-Adgent/open-seo-mcp-skills: 8,530
  - Auriti-Labs/geo-optimizer-skill: 1,255
  - onvoyage-ai/gtm-engineer-skills: 1,345
  - only 6 repos for a "local business schema markup generator"
- Paid kits:
  - "AI Discoverability Audit v2" $19 ([brianrwagner](https://brianrwagner.gumroad.com/l/ai-discoverability-audit), price from [README](https://github.com/BrianRWagner/ai-marketing-claude-code-skills))
  - [probiex geo-operations-system](https://probiex.gumroad.com/l/geo-operations-system)
  - relayed: $19 GEO starter kit ([genxops](https://genxops.gumroad.com/l/geo_for_smbs)), €39 AEO Starter Kit ([aeo-starter-kit.pages.dev](https://aeo-starter-kit.pages.dev/)), £39 Payhip AEO audit kit ([payhip](https://payhip.com/b/YzjDQ))
- No GEO kit appeared among rated titles in either Gumroad crawl.
- **Gaps:** almost all supply targets marketers and SEO agencies, not a named local trade. Local-business schema snippets look thin.

### E. Chrome Web Store (direct store access blocked)

**31. AI writing helpers (SATURATED, MEDIUM-STRONG; Jul 2026).**
- A Jul 2026 crawl found 39,241 AI-labelled Chrome extensions, only 215 with 100k+ users. The biggest categories are productivity/tools (19,038), productivity/workflow (6,037) and productivity/education (2,581).
- Leaders: Grammarly 35M users (4.5 stars, 43,097 ratings), Quillbot 5M, DeepL 4M, LanguageTool 2M, Sider 5M (4.92 stars, 113,374 ratings), Monica 3M ([Crawlora dataset](https://github.com/Crawlora-org/ai-browser-extensions-data), [summary.json](https://raw.githubusercontent.com/Crawlora-org/ai-browser-extensions-data/HEAD/data/summary.json)).
- Crawlora is a scraping vendor (conflict of interest: low; aggregate data only).

**30, 32-39. Other extension categories (WEAK; GitHub open-source counts only).**
- GitHub repository counts (GH search, 1 Nov 2026):
  - accessibility checker: 15
  - SEO extensions: 235 created since Nov 2025
  - LinkedIn AI extensions: 280 since Nov 2025
  - Etsy extensions: 71
  - Shopify extensions: 79 since Nov 2025
  - ChatGPT exporters: 214
  - AI detectors: 213
  - Google review-reply AI: 133
  - invoice extensions: 70
- These show free-builder activity, not store competition.
- Gumroad-sold extensions are alive but owned by dev-tool sellers: G-36 "chrome extension" 28 of 36 rated, median $19.99. "CSS Scan" (~$49, 205 ratings) and "Super Spy HeyEtsy" ($19, 80 ratings) show an Etsy-seller extension can sell off-store ([sujeito](https://github.com/sujeito-operator/gumroad-market-data)).
- Etsy SEO tooling is saturated and Etsy is adding native AI (relayed: [SellerMarketingTool](https://sellermarketingtool.com/etsy-seo-tools), [Etsy announcements](https://community.etsy.com/forum/announcements-290/)).
- A free MV3 Google-review reply extension exists (Jamaalx/zed-zen-ai-review-extensions), plus a Google Business Profile MCP (A1-x-Tech/mcp-google-business) (GH search).
- **Not verified:** CWS listing counts, user counts and ratings for every non-AI-tagged category.

### F. TPT / education seeds

**41. School AI policy packs: seed 9 (CROWDED by free supply; MEDIUM, relayed).**
- Free templates (relayed): [Tes](https://www.tes.com/en-nz/teaching-resource/artificial-intelligence-ai-policy-template-13133971), [Third Space Learning](https://thirdspacelearning.com/blog/ai-policy-for-schools/), [Kuraplan](https://www.kuraplan.com/uk/ai-policy?year=1), plus state model policies.
- GitHub: 74 repos match "ai policy school" (GH search).
- Paid packs from ghostcorpnet: "School Pilot Program Playbook" $29 and "Multi-School Governance Bundle" $49 ([catalog.json](https://raw.githubusercontent.com/koalstingkdelaney-gif/kestrelattice/HEAD/ai/catalog.json)).
- A teacher prompt pack exists ([clowealex teacher-ai-prompts](https://clowealex.gumroad.com/l/teacher-ai-prompts), found in GitHub code).
- TPT counts are unknown.

**42-43. AI lesson plans and AI literacy (UNVERIFIED, WEAK).**
- GitHub: 237 "lesson plan generator" repos created since Nov 2025, plus the free 165-skill teacher repo (GH search).
- A Gumroad AI literacy kit exists ([probiex ai-literacy-kit](https://probiex.gumroad.com/l/ai-literacy-kit), found in GitHub code).

### G. Remaining seed categories

**44. EU AI Act templates: seed 3 (SATURATED, STRONG).**
- Etsy kits at $12.99, $20.76 and $131.27 (relayed: [Etsy market](https://www.etsy.com/market/ai_policies), [Etsy bundle](https://www.etsy.com/listing/4430787946/2026-ai-compliance-bundle-for-eu-and-us)).
- Vendor kits at €990, $99 and $229+ (relayed).
- GitHub: 1,125 repos created since Jan 2026 (relayed) and 59 "eu ai act template" repos (GH search).
- On Gumroad, a single seller has 29 EU-AI-Act-tagged products at $19-$49 (e.g. "AI Act Obligation Matrix" $29, "AI Act Gap Assessment Deck" $49) ([catalog.json](https://raw.githubusercontent.com/koalstingkdelaney-gif/kestrelattice/HEAD/ai/catalog.json)), alongside [mininglife1 eu-ai-act-readiness-kit](https://mininglife1.gumroad.com/l/eu-ai-act-readiness-kit) and fortressaudit packs (found in GitHub code).
- The regulation file reports Art. 4 was softened, with no EU fine (relayed).

**45. SMB AI acceptable-use policies (CROWDED, MEDIUM).**
- ghostcorpnet alone has 59 policy-tagged products ([catalog.json](https://raw.githubusercontent.com/koalstingkdelaney-gif/kestrelattice/HEAD/ai/catalog.json)).
- 9 free GitHub templates exist, including brandquill/small-business-ai-policy-template and nosistech/governance-templates (GH search).
- A UK bundle ([aicomplianceuk](https://aicomplianceuk.gumroad.com/l/ai-compliance-bundle), found in GitHub code).
- **Gap:** vertical policies (solo law, therapy, bookkeeping) were not seen in these sources. Pain-hunter suggested them; demand is unverified.

**46. Accessibility statement / fix kits: seed 4 (MODERATE, MEDIUM).**
- Paid: a Gumroad statement template (relayed: [mirelaprifti](https://mirelaprifti.gumroad.com/l/website-accessibility-statement)), "Accessibility Compliance Quickstart" $19 ([catalog.json](https://raw.githubusercontent.com/koalstingkdelaney-gif/kestrelattice/HEAD/ai/catalog.json)), and a website accessibility handoff kit ([itsupportgroup](https://itsupportgroup.gumroad.com/l/website-handoff-kit), found in GitHub code).
- Free:
  - 17 statement-generator repos on GitHub (GH search)
  - free generators from iubenda and getwcag, and npm packages `eaa-kit` and `@ariada-org/statement-generator` (relayed)
  - 88 "shopify accessibility" repos, including kgelster/ecom-a11y-audit, which attributes failures to theme vs app
  - zivtech/accessibility-skills and a free Claude accessibility-audit skill (relayed)
- Overlays and apps are priced $49-$149/mo (relayed, vendor-sourced).
- **Gap:** platform-specific, non-overlay manual-fix checklists for Shopify, Wix or Squarespace owners, written for non-developers, look thin. **Buyer proof on Gumroad: none visible.**

**47. llms.txt (SATURATED by free supply, STRONG).**
- GitHub: 2,544 repos match "llms.txt" and 173 generators were created since Nov 2025 (GH search).
- A paid product exists ([grantshatz llmstxt-pro](https://grantshatz.gumroad.com/l/llmstxt-pro), found in GitHub code).
- The regulation file relays that AI crawlers barely request the file and that there is no citation correlation.

**48. Brand voice packs: seed 7 (CROWDED, low ceiling, MEDIUM).**
- GitHub: 216 "brand voice skill" repos created since Nov 2025; arnabbagxd/Brand-building-skills has 821 stars and cofoundy/brand-skills is free (GH search).
- Paid: "Brand Voice Extractor" at $9 on Gumroad, with a "$9 premium version on Claw Mart" ([BrianRWagner README](https://github.com/BrianRWagner/ai-marketing-claude-code-skills)).
- No brand-voice title appeared among rated products in either Gumroad crawl.

**49. Chatbot test / QA kits: seed 8 (THIN, no buyer proof, WEAK).**
- GitHub: only 2 repos match "chatbot testing checklist", both free (Synorthos/chatbot-golive-checklist, Autonoma-Tools/chatbot-testing-checklist). 70 "chatbot test cases" repos were created since Nov 2025, mostly QA-student portfolios (GH search).
- No Gumroad listing was found in GitHub code search: the hits for "gumroad.com/l" plus chatbot testing were all unrelated.
- **Thin because nobody sells it, and nobody has shown anyone buys it.**

**50. SOP-to-agent converters: seed 10 (THIN paid, no buyer proof, WEAK).**
- GitHub: 81 "sop to skill" repos (e.g. bruiandy/experience-to-asset, darthjaja6/distill, qingxuantang Lennys-to-sop-and-skills), 11 "sop agent instructions" repos since Nov 2025 and a commercial "SOP compiler" (sopops-dev) (GH search).
- Free lead magnet: the "One-Shot Skill Creation Prompt" on Gumroad, described as extracting "a comprehensive SOP from any screen recording" ([earlyaidopters/gumroad-resources](https://github.com/earlyaidopters/gumroad-resources)).

### H. Other thin-but-alive Gumroad terms (useful pattern data)

**51. Niche business templates (MODERATE with buyers, MEDIUM).**

From the 6 Aug 2026 scan ([gumroad-demand.csv](https://raw.githubusercontent.com/marcosgcuenta1/gumroad-demand-dataset/HEAD/gumroad-demand.csv)):

| Term | Listings | Top-10 ratings |
|---|---|---|
| okr template | 135 | 120 |
| saas metrics | 206 | 95 |
| real estate model | 239 | 78 |
| retirement calculator | 36 | 152 |
| zettelkasten | 82 | 87 |
| meeting notes | 890 | 664 |
| pitch deck | 486 | 286 |
| financial model | 955 | 331 |

Caveats:
- The top-10 ratings often come from one or two products, sometimes off-topic.
- These suit finance and knowledge workers, not trades.
- Financial models command $149 with up to 53 ratings ([sujeito](https://github.com/sujeito-operator/gumroad-market-data)).

**52. Copywriting swipe files (THIN-MODERATE with buyers, WEAK-MEDIUM).**
- 98 listings, 28 top-10 ratings, 7 of 10 rated ([gumroad-demand.csv](https://raw.githubusercontent.com/marcosgcuenta1/gumroad-demand-dataset/HEAD/gumroad-demand.csv)).

---

## Ranked shortlist: thinnest categories that still show buyer activity

"Buyer activity" means rated or sold products exist at a non-zero price. All evidence is from Aug 2026 Gumroad crawls unless noted.

| Rank | Category | Why thin | Buyer proof | Main risk | Evidence |
|---|---|---|---|---|---|
| 1 | **Claude/Cowork kits for one named non-dev profession, at $29-$69, as installable skills (not prompt lists)** | 1-4 paid Gumroad titles per profession; free GitHub packs are thin for trades, insurance and dental offices | $70 designers (42 ratings), $39 lawyers (11), $49 PM (6), $29 architects (5) | Free GitHub packs for white-collar roles; sales follow creator audience; $129-$199 kits got 0 ratings | MEDIUM |
| 2 | **Freelance / creative-services contract templates (specific discipline)** | 165 Gumroad listings; 21 of 36 in one sample unrated | One ~$11.55 template has 106 ratings | Legal liability; Claude now drafts contracts (relayed IH) | MEDIUM |
| 3 | **Niche business-model templates (OKR, SaaS metrics, real-estate model, retirement calculator)** | 36-239 Gumroad listings | 78-152 top-10 ratings | Ratings concentrated in 1-2 incumbents; finance-literate buyers | MEDIUM |
| 4 | **Etsy-seller / marketplace-seller tools sold off-store** | Few off-store sellers seen | "Super Spy HeyEtsy" $19: 80 ratings | Etsy SEO tools saturated (relayed); Etsy adding native AI | WEAK-MEDIUM |
| 5 | **Copywriting swipe files (vertical)** | 98 listings | 28 ratings, 7 of 10 rated | Small absolute demand | WEAK-MEDIUM |
| 6 | **Lesson plans / homeschool units** | 244-398 listings | 107 and 83 ratings on curriculum bundles | Buyers want full curricula, not a one-day product; TPT unmeasured | MEDIUM (poor fit) |

**Thin but no buyer proof yet (test cheaply or drop):**
- chatbot QA checklist kits for SMBs (#49)
- SOP-to-agent kits (#50)
- MCP setup guides for zero-coverage software such as Dentrix, Dubsado, Vagaro, Podia, HoneyBook, SimplePractice and Acuity (#28)
- per-trade voice-receptionist script and setup kits (#27)
- platform-specific accessibility manual-fix kits (#46)
- Make.com templates (#23)
- vertical SOP libraries (#13)

**Thin because dead on Gumroad, but possibly alive on Etsy (switch marketplace, don't drop the idea):**
- bookkeeping, rental-property, Airbnb and construction job-costing spreadsheets
- Etsy-seller bookkeeping
- wedding planners

## Implications for the seed hypotheses (marketplace-saturation lens only)

| # | Hypothesis | Supply picture | Buyer proof | Lean |
|---|---|---|---|---|
| 1 | Claude Code / agent skill packs for non-dev professions | Generic: SATURATED. Per-profession: THIN (trades, insurance, dental) to CROWDED (marketing, legal, education, PM) | Yes, small (5-42 ratings at $29-$70) | **Support, narrowly:** one profession, installable skills, $29-$69, plus an audience channel |
| 2 | GEO / AI-search kits | CROWDED by free skills; paid kits at $9-$39 | None visible | Weak; only as a local-trade-specific bundle |
| 3 | EU AI Act starter packs | SATURATED (mass-generated plus free) | None visible | **Reject** |
| 4 | Accessibility fix kits | MODERATE (thin paid templates, free generators, app incumbents) | None visible on Gumroad | Neutral; needs a buyer test |
| 5 | MCP connectors / guides | SATURATED for big SaaS; THIN for niche vertical SaaS | None visible | Weak; test one zero-coverage vertical only if it has an API |
| 6 | Voice receptionist templates | Builder repos SATURATED; paid owner-facing templates THIN; $49 compliance packs exist | None visible | Weak |
| 7 | Brand voice packs | CROWDED; $9 anchor | None visible | **Reject** as standalone |
| 8 | Chatbot test / QA kits | THIN | None visible | Unproven; cheap test only |
| 9 | AI policy packs for schools / tutoring | CROWDED by free official templates; one $29-$49 seller | None visible | **Reject** for schools |
| 10 | SOP-to-agent converters | THIN paid; free lead magnets exist | None visible | Unproven; better as a feature of #1 |

## Method & limitations

- **Zero WebSearch calls succeeded.** The shared 200-call WebSearch budget was exhausted before this agent's first query. Per the tool's instruction, no workaround through search engines was attempted. **If the lead needs Etsy, TPT, Notion, Framer, Product Hunt or Chrome Web Store result counts, the user must raise `CLAUDE_CODE_MAX_WEB_SEARCHES_PER_SESSION` or re-run this role.**
- **Direct marketplace access failed:** WebFetch returned ENOTFOUND for chromewebstore.google.com, www.notion.com, www.framer.com and www.teacherspayteachers.com. No marketplace page was opened directly.
- **Primary evidence used:**
  - Two independent third-party Gumroad crawls hosted on GitHub, downloaded as raw CSV and analysed locally:
    - [marcosgcuenta1/gumroad-demand-dataset](https://github.com/marcosgcuenta1/gumroad-demand-dataset): 101 terms, top 10 per term, snapshot 6 Aug 2026, CC0. Listing counts are Gumroad's loose search-hit counts. Its README warns "Re-run it rather than cite it".
    - [sujeito-operator/gumroad-market-data](https://github.com/sujeito-operator/gumroad-market-data): 8,311-product category walk plus 42 search terms × 36 listings, Aug 2026. Its category counts are crawl-depth-capped at 44.
  - One vendor dataset (InsightRaider, [Pinous/gumroad-market-data](https://github.com/Pinous/gumroad-market-data), Mar 2026, estimated revenue; WEAK).
  - One Chrome AI-extension dataset ([Crawlora](https://github.com/Crawlora-org/ai-browser-extensions-data), crawled 14 Jul 2026; vendor, aggregate only).
- **Proxy evidence used:**
  - GitHub repository search `total_count` (fuzzy keyword matches; counts free builder supply, not marketplace competition).
  - npm registry search, counting only packages whose name contains the product and mentions MCP.
  - GitHub code search for `gumroad.com/l/` links next to category keywords. This proves a paid listing existed at some point; price, sales and status were not visible unless a README stated them.
- **Relayed evidence** (marked "relayed") comes from the sibling files `pain-hunter.md` and `regulation-and-platform-shifts.md`. It was not re-verified by this agent.
- **Known biases:**
  - Both Gumroad crawls are single snapshots, and Discover reorders.
  - Ratings lag sales, and most buyers never rate.
  - The sales-per-rating multiplier comes from a 3D-heavy sample.
  - Neither crawl searched several seed terms ("voice agent", "MCP", "brand voice", "chatbot", "SOP", "accessibility"), so "absent from crawls" is weak evidence of absent demand.
  - Seller display names (e.g. "Aakash Gupta") are as they appeared in crawl text. The audience inference about them is this agent's, not a sourced fact.
- **Not measured at all:** Etsy result counts and review counts; Notion marketplace and gallery; Framer marketplace; TPT; Product Hunt; Lemon Squeezy storefronts; non-AI Chrome Web Store categories; Make, Zapier and Vapi native template galleries.

## Sources

Datasets (primary for this file):
- https://github.com/marcosgcuenta1/gumroad-demand-dataset
- https://raw.githubusercontent.com/marcosgcuenta1/gumroad-demand-dataset/HEAD/gumroad-demand.csv
- https://github.com/sujeito-operator/gumroad-market-data
- https://github.com/Pinous/gumroad-market-data
- https://github.com/Crawlora-org/ai-browser-extensions-data
- https://raw.githubusercontent.com/Crawlora-org/ai-browser-extensions-data/HEAD/data/summary.json
- https://raw.githubusercontent.com/koalstingkdelaney-gif/kestrelattice/HEAD/ai/catalog.json

GitHub repos (READMEs read or cited from search results):
- https://github.com/BrianRWagner/ai-marketing-claude-code-skills
- https://github.com/earlyaidopters/gumroad-resources
- https://github.com/polar-bear-org/claude-skills
- https://github.com/miron-tech/realtor-claude-skills
- https://github.com/miron-tech/hvac-claude-skills
- https://github.com/alexclowe/awesome-claude-cowork-plugins
- GitHub search API (api.github.com/search/repositories and /search/code), queried 1 Nov 2026. Repos named inline (anthropics/skills, PatrickJS/awesome-cursorrules, Zie619/n8n-workflows, enescingoz/awesome-n8n-templates, f/prompts.chat, AgriciDaniel/claude-seo, GarethManning/education-agent-skills, etc.) are from these result lists.
- npm registry search API (registry.npmjs.org/-/v1/search), queried 1 Nov 2026

Gumroad product URLs (from datasets or GitHub code; not opened):
- https://aidesignlab.gumroad.com/l/claude-code-for-designers
- https://kumail.gumroad.com/l/360l
- https://growthpioneer.gumroad.com/l/pmos
- https://growthpioneer.gumroad.com/l/jobsearchos
- https://arjunechow.gumroad.com/l/claude
- https://ismailsaleem.gumroad.com/l/How-Accountant-Can-Use-Claude-Cowork-Powerful-Use-Cases
- https://usamaakrm.gumroad.com/l/premium-claude-skills
- https://thinkaiprompt.gumroad.com/l/claude-skills
- https://yourchatgptguide.gumroad.com/l/ClaudeOS
- https://brianrwagner.gumroad.com/l/ai-discoverability-audit
- https://probiex.gumroad.com/l/geo-operations-system
- https://probiex.gumroad.com/l/ai-literacy-kit
- https://grantshatz.gumroad.com/l/llmstxt-pro
- https://dialdaddy.gumroad.com/l/how-to-build-a-vapi-voice-agent
- https://tuguidragos.gumroad.com/l/ghl-n8n-vapi-ai-calling-agent
- https://chronoai.gumroad.com/l/aireceptionist
- https://goodepochhq.gumroad.com/l/cursor-rules
- https://nedcodes.gumroad.com/l/cursor-doctor-pro
- https://blncraft.gumroad.com/l/vibe-coder-kit
- https://echochime3.gumroad.com/l/claudemd-bible
- https://studioddx.gumroad.com/l/n8n-workflow-mega-pack
- https://viktorgubanov.gumroad.com/l/n8n-telegram-bot-template
- https://markkashef.gumroad.com/l/mcpclaude
- https://mininglife1.gumroad.com/l/eu-ai-act-readiness-kit
- https://aicomplianceuk.gumroad.com/l/ai-compliance-bundle
- https://clowealex.gumroad.com/l/teacher-ai-prompts
- https://itsupportgroup.gumroad.com/l/website-handoff-kit

Relayed from sibling Phase 1 files (not re-verified here):
- https://www.etsy.com/market/ai_policies
- https://www.etsy.com/listing/4430787946/2026-ai-compliance-bundle-for-eu-and-us
- https://www.etsy.com/listing/4567179604/
- https://www.etsy.com/listing/1733890901/cleaning-business-crm-client-task
- https://www.etsy.com/listing/4432325264/progress-note-samples-documentation
- https://cleanstrong.gumroad.com/l/ecfyg
- https://genxops.gumroad.com/l/geo_for_smbs
- https://aeo-starter-kit.pages.dev/
- https://payhip.com/b/YzjDQ
- https://www.framer.com/marketplace/templates/aeo-geo-seo/?via=doug
- https://mirelaprifti.gumroad.com/l/website-accessibility-statement
- https://inflectual.gumroad.com/l/master-marketing-claude-skills-bundle
- https://www.indiehackers.com/post/built-a-finance-kit-for-freelancers-three-weeks-live-0-revenue-3c667a7111
- https://www.indiehackers.com/post/i-made-57-in-48-hours-selling-claude-cheat-codes-here-s-what-worked-and-what-didn-t-01d7f1f61c
- https://www.indiehackers.com/post/i-am-an-autonomous-ai-agent-10-weeks-2-sales-54-here-is-what-i-actually-learned-300698bdfe
- https://www.indiehackers.com/post/claude-ate-my-products-main-feature-i-kept-the-part-it-can-t-eat-b2596a6a36
- https://www.inkfluenceai.com/blog/etsy-ai-rules-update-october-2026
- https://www.teacherspayteachers.com/Browse/Search:report%20card%20comment%20bank
- https://www.tes.com/en-nz/teaching-resource/artificial-intelligence-ai-policy-template-13133971
- https://thirdspacelearning.com/blog/ai-policy-for-schools/
- https://www.kuraplan.com/uk/ai-policy?year=1
- https://sellermarketingtool.com/etsy-seo-tools
- https://community.etsy.com/forum/announcements-290/
- https://trainual.com/solution/sop-templates
