# Phase 2: Candidate products (synthesis by lead)

Date: 2026-11-01. Built from the five Phase 1 files in `research/phase1/`. "PH#" = pain-hunter item, "REG#" = regulation-and-platform-shifts rank, "G#" = ai-ecosystem-gaps item, "MS#" = marketplace-saturation-scout row, "TR#" = trend-scout rank.

## How Phase 1 actually went (read before trusting anything below)

- WebFetch was blocked for almost every host in this cloud environment, including Reddit, Gumroad, Etsy, Product Hunt, HN and most blogs. Only github.com was reachable. Agents worked from WebSearch result lists and excerpts, plus the GitHub, npm and MCP-registry APIs.
- WebSearch has a shared budget of about 200 calls. **pain-hunter** and **regulation-and-platform-shifts** used it up. **ai-ecosystem-gaps**, **marketplace-saturation-scout** and **trend-scout** ran with zero web searches and fell back on other data:
  - GitHub repo counts and time series
  - the official MCP Registry dump
  - two Aug 2026 Gumroad scrape datasets hosted on GitHub
  - a Jul 2026 Chrome Web Store AI-extension dataset
  - the YC company directory
- **Consequences:**
  - Demand evidence for AI-tooling ideas is mostly supply-side: GitHub activity, not buyers.
  - Etsy, TPT, the Notion/Framer marketplaces and non-AI Chrome Web Store categories were **not** measured directly.
  - Reddit evidence comes from search-tool summaries of mirror pages.
- The completeness critic and gap-fill step was cancelled to save time (the user asked to speed up). Phase 3 validators are told to fill these gaps.

## Cross-cutting conclusions from Phase 1

1. **Generic AI packs are a trap.** Generic prompt packs, n8n templates, CLAUDE.md files, Cursor rules, Notion templates and Canva templates are saturated or dominated by free products (MS#1, #8, #15, #18, #21, #22). Indie Hackers reports $3-$57 outcomes for generic Claude/prompt packs (pain-hunter, executive summary).
2. **Anthropic and vendors now give away the broad layer for free.** Claude for Small Business, launched 15 Sep 2026, is a free plugin with 44 skills and 35 connectors (TR#1). It sits alongside official legal, finance, sales, marketing, K-12 and healthcare plugins, official QuickBooks, Xero, Square and Wix MCP servers, a free brand-voice plugin, and Microsoft's free skill-recorder (TR, G1). What's left open is **depth in narrow verticals that the free layer skips** (trades, therapy, dental, bookkeeping workflows, salons) and **regulation-driven kits for non-technical buyers**.
3. **The strongest forcing functions are not AI laws.** They are:
   - ADA/EAA accessibility lawsuits (REG#1)
   - UK Making Tax Digital for Income Tax, with the Apr 2027 wave (REG#2)
   - A2P 10DLC SMS registration rejections (REG#3)
   - AI-search and Google Maps changes (REG#4)
   - the FTC review rule (REG#5)

   EU AI Act duties were softened by the Digital Omnibus (REG#13). School AI-policy mandates hit districts, which get free model policies (REG#15).
4. **Paid profession-specific Claude kits do sell, modestly.** Examples: $70 Claude Code for Designers (42 ratings), $39 lawyers (11), $49 PM (6), $29 architects (5). $129-$199 kits got 0 ratings (MS#20). Gumroad is winner-take-most: 43% of products have zero ratings (MS executive summary). **Distribution, not the build, is the binding constraint.**
5. **Match the format to the marketplace.** Spreadsheets and templates sell on Etsy, not Gumroad (MS ranked shortlist). Teacher products sell on TPT. Skill packs sell on Gumroad and Lemon Squeezy.

## Assumptions (no questions asked, per brief)

- The founder is US- or EU-based and can sell globally via Gumroad, Lemon Squeezy and Etsy. US and UK buyers are the main markets (largest English-speaking marketplaces).
- The founder has no existing audience. Distribution must come from marketplace search plus communities that tolerate launches.
- "Build in one day" means a downloadable kit or a static web tool. No backend with auth, no vendor partner approvals, no paid-API testing beyond about $20.
- Compliance-adjacent products are sold as checklists and templates with "not legal/tax advice" disclaimers, never as "makes you compliant" (FTC v. accessiBe precedent, REG risk notes).

## Candidates (30)

Format: **ID. Name.** What it is · Who buys · Why now · (sources). Seed hypotheses are marked **[SEED n]**. All 10 seeds are included as candidates so Phase 3 can validate or reject them on the same rubric.

### Batch 1: Vertical AI skill packs
- **C01. HVAC & plumbing "AI office manager" skill pack [SEED 1]**
  - What: 8-12 Claude/Cowork skills (quote write-ups, quote follow-ups, maintenance-agreement renewals, review requests, job-recap texts), working from Jobber/Housecall Pro CSV exports, plus a setup PDF.
  - Who buys: owner-operators of 1-10-truck HVAC/plumbing shops who already pay for Claude.
  - Why now: Cowork and Claude for Small Business are onboarding non-technical owners (Sep 2026), and the official marketplace has 0 trades plugins.
  - Sources: G5, TR#1, PH#9, #23, #31.
- **C02. Bookkeeper month-end close skill pack on the official QuickBooks/Xero connectors [SEED 1]**
  - What: skills for reconciliation review, uncategorised-transaction cleanup, client-query emails and month-end checklists.
  - Who buys: solo and small-firm bookkeepers.
  - Why now: official Intuit/Xero MCP servers shipped in 2026; Anthropic's finance plugin targets enterprise tools.
  - Sources: G3, PH#8.
- **C03. Therapist private-practice documentation kit (no-PHI) [SEED 1]**
  - What: progress-note templates (SOAP/DAP/BIRP), an intervention phrase bank, Claude project instructions that work on de-identified shorthand, and a HIPAA-safe AI-use checklist.
  - Who buys: solo and small-group private-practice therapists.
  - Why now: notes eat their evenings; AI scribes cost about $35 per clinician per month and raise HIPAA anxiety.
  - Sources: PH#1, TR#5.
- **C04. Realtor AI listing & follow-up kit with fair-housing guardrails [SEED 1]**
  - What: Claude/ChatGPT project instructions plus skills for listing descriptions, social posts and lead follow-ups, with a fair-housing word-check list.
  - Who buys: individual real estate agents.
  - Why now: heavy AI use, and NAR 2026 cites the learning curve as the #1 barrier.
  - Sources: PH#7, G4 (real estate is semi-crowded).
- **C05. SOP-to-agent instruction converter [SEED 10]**
  - What: a web tool or Claude skill that turns a written SOP into a SKILL.md or agent instructions.
  - Who buys: SMB owners documenting processes.
  - Why now: skills became mainstream in 2026.
  - Sources: PH#19, G12, TR#19. Counter-evidence: Microsoft's skill-recorder and Anthropic's skill-creator are free.

### Batch 2: AI tooling and setup
- **C06. "Connect Claude to your business tools" setup kit for non-developers [SEED 5]**
  - What: an illustrated guide plus config files for connecting Claude Desktop/Cowork to QuickBooks, Square, Google Drive, Jobber and similar tools, with fixes for the top 10 errors.
  - Who buys: SMB owners on Claude Pro.
  - Why now: there are 1,312 Cowork issues and 927 MCP-connector issues since May 2026.
  - Sources: G6. Counter-evidence: vendor bugs, free guides, one-click installs.
- **C07. Per-trade voice-receptionist template pack for AI-automation agencies [SEED 6]**
  - What: Vapi/Retell system prompts, function/tool JSON, test-call scripts, a QA checklist, and state-by-state AI-disclosure and recording-consent scripts for HVAC, plumbing, dental and legal intake.
  - Who buys: small AI-automation agencies and freelancers building receptionists.
  - Why now: "ai receptionist" repo creation is up 8.8x, and the compliance layer is fragmented.
  - Sources: G9, TR#3, REG#6.
- **C08. Chatbot & AI-receptionist QA test kit for SMBs [SEED 8]**
  - What: 150 test prompts by category (pricing, refunds, hallucination traps, prompt injection, escalation), a scorecard sheet and a go-live checklist.
  - Who buys: SMBs or agencies deploying website chatbots or receptionists.
  - Why now: liability rulings on chatbot answers (Air Canada; OLG Hamm 2026).
  - Sources: G11, MS#49, REG seed table.
- **C09. Brand voice pack for AI tools [SEED 7]**
  - What: a voice-discovery worksheet plus generated Claude/ChatGPT/Gemini project instructions and a style guide.
  - Who buys: small business owners and solo marketers.
  - Why now: generic AI copy drifts off-brand.
  - Sources: PH#29, G10, MS#48, TR#18. Counter-evidence: official free brand-voice plugin; price anchored at $9.
- **C10. "Agent-ready local business" kit**
  - What: a Cloudflare Worker template serving a read-only services/areas/prices/booking MCP endpoint, plus JSON-LD and a registry-publishing guide.
  - Who buys: local-SEO freelancers and agencies.
  - Why now: plumbers and HVAC firms started publishing MCP servers to the official registry (Aug-Oct 2026).
  - Sources: G7. Speculative.

### Batch 3: Local search, reviews and seller platforms
- **C11. "Get found by AI" kit for local service businesses [SEED 2, re-scoped]**
  - What: a plain-English Google Business Profile, reviews and schema playbook, a JSON-LD generator, and a walkthrough of the new Search Console generative-AI and Bing AI Performance reports. llms.txt is deliberately left out.
  - Who buys: owners of local service businesses, or the freelancers who serve them.
  - Why now: AI Overviews and AI Mode have over 1B users, Ask Maps replaced Google Business Profile Q&A, and new AI reports launched in Search Console (Jun 2026) and Bing (Feb 2026).
  - Sources: REG#4, TR#2, G8.
- **C12. FTC-compliant review-request kit**
  - What: SMS, email and card templates plus a QR-card generator that avoid review gating and incentives, and review-response templates.
  - Who buys: local service businesses (trades, clinics, salons).
  - Why now: the FTC Consumer Review Rule brought its first suit in May 2026, and Ask Maps leans on reviews.
  - Sources: REG#5, PH#26.
- **C13. Agentic-commerce readiness checklist for Shopify/Etsy sellers**
  - What: product-data, feed and policy checklist plus fixes so listings show up in ChatGPT, Gemini and Google AI shopping.
  - Who buys: small Shopify and Etsy sellers.
  - Why now: "agentic commerce" repos are up 40x, and UCP launched with Google, Shopify and Etsy.
  - Sources: TR#9. Seller demand unproven.
- **C14. Etsy digital-seller compliance kit**
  - What: an AI-disclosure, "Designed by" and Creativity Standards checklist, listing-copy templates and a policy-change tracker.
  - Who buys: Etsy digital-download sellers.
  - Why now: digital downloads came under Creativity Standards (Jun 2025), and "Designed by" enforcement has been reported since Jan 2026.
  - Sources: REG#9.
- **C15. Vibe-coder launch safety kit**
  - What: a Claude skill plus checklist for non-developers shipping AI-built apps: secrets, auth, RLS, privacy policy, Stripe webhooks, backups.
  - Who buys: non-developer founders using Lovable, Bolt or Claude Code.
  - Why now: vibe-coding repos are up 3.4x, with an October rebound.
  - Sources: TR#11. Counter-evidence: free security skills, one with 56k stars.

### Batch 4: Compliance kits
- **C16. EU AI Act starter compliance pack for small companies [SEED 3]**
  - What: an AI inventory, an Art. 4 AI-literacy plan, Art. 50 transparency notices and an AI-use policy.
  - Who buys: EU SMEs using AI tools.
  - Why now: Art. 50 applied from 2 Aug 2026.
  - Sources: REG#13, MS#44, TR#20. Counter-evidence: softened duty, no fines found, saturated.
- **C17. Shopify/Wix accessibility self-audit & fix kit [SEED 4]**
  - What: a platform-specific manual-fix checklist (theme, alt text, contrast, forms, focus), an accessibility statement template and a "received a demand letter: first 48 hours" guide.
  - Who buys: small US and EU e-commerce store owners.
  - Why now: about 2,045 ADA website suits were filed in H1 2026, 79% against e-commerce, and EAA enforcement has started.
  - Sources: REG#1, TR#4, MS#46.
- **C18. A2P 10DLC approval kit**
  - What: privacy-policy and terms clauses, opt-in form copy, campaign-description and sample-message templates, and a rejection-code fix table.
  - Who buys: US SMBs that text customers, and GoHighLevel/Twilio agencies.
  - Why now: Twilio made privacy and terms URLs mandatory from 30 Jun 2026, and TCPA changes are pending.
  - Sources: REG#3, TR#6.
- **C19. UK data-protection complaints procedure pack (DUAA)**
  - What: a complaints procedure, acknowledgement and response letters, and a complaints log.
  - Who buys: UK small businesses, charities and clubs.
  - Why now: the procedure has been mandatory under the Data (Use and Access) Act since 19 Jun 2026, with no size exemption.
  - Sources: REG#7.
- **C20. Auto-renewal compliance kit for small subscription sellers (CA/NY)**
  - What: a checklist, disclosure copy, a cancellation-flow script and reminder-email templates.
  - Who buys: creators and small subscription/membership sellers (Kajabi, Skool, Shopify subscriptions).
  - Why now: CA amendments took effect in Jul 2025 and NY amendments in Nov 2025, the federal click-to-cancel rule was vacated, and the FTC restarted rulemaking.
  - Sources: REG#8.

### Batch 5: Money, tax and operations templates
- **C21. UK Making Tax Digital (ITSA) digital-records spreadsheet + bridging guide**
  - What: a Google Sheets/Excel quarterly-records template for sole traders and landlords, with a step-by-step guide to bridging software.
  - Who buys: UK sole traders and landlords with £30k-£50k income.
  - Why now: about 1M more people are mandated from Apr 2027, and the over-£50k wave has been live since Apr 2026.
  - Sources: REG#2, TR#7.
- **C22. Bookkeeper client document-chasing kit**
  - What: a missing-documents tracker (Sheets), request and reminder email/SMS sequences, and a client checklist portal template.
  - Who buys: solo bookkeepers and tax preparers.
  - Why now: tax season (Jan-Apr) is approaching, and document chasing is a constant pain.
  - Sources: PH#8.
- **C23. Freelancer and small-agency "get paid" kit**
  - What: a polite-to-firm late-payment email sequence, late-fee and contract clauses, an AR tracker sheet and payment-terms templates.
  - Who buys: freelancers and micro-agencies.
  - Why now: QuickBooks 2026 reports 59% have invoices 30+ days overdue.
  - Sources: PH#5.
- **C24. One-time-price trades ops kit (anti-subscription)**
  - What: a Google Sheets kit covering estimates, invoices, job tracker, maintenance-agreement renewals and a price book.
  - Who buys: solo and small trades owners resenting Jobber/HCP price hikes.
  - Why now: subscription fatigue (PH#2, #9, #31).
- **C25. TAKE IT DOWN Act compliance pack for small online communities**
  - What: a notice-and-removal policy, request form, 48-hour SOP and log.
  - Who buys: small forums, Discord/Circle/Skool communities and niche UGC sites.
  - Why now: FTC enforcement since 19 May 2026.
  - Sources: REG#10.

### Batch 6: Education and professional services
- **C26. AI usage policy pack for tutoring centres and small private schools [SEED 9]**
  - What: an AI-use policy, parent and student agreements, a staff guide and an academic-integrity process.
  - Who buys: owners of tutoring centres and micro-schools.
  - Why now: state and UK guidance, plus parent questions.
  - Sources: REG#15, TR#21. Counter-evidence: districts get free model policies, and no tutoring mandate was found.
- **C27. Report-card comment bank + generator for one curriculum/grade band**
  - What: 500+ editable comments by subject and skill level, plus a Sheets/Claude generator that personalises them from a short grade table.
  - Who buys: K-12 teachers (e.g. US elementary, or one Canadian province's curriculum).
  - Why now: report-card season peaks Nov-Dec, Mar and Jun, and it is happening now.
  - Sources: PH#10.
- **C28. Independent tutor business kit**
  - What: Sheets/Notion for sessions, prepaid packages, invoices and parent progress reports.
  - Who buys: independent tutors.
  - Sources: PH#18 (crowded per pain-hunter).
- **C29. Wedding/portrait photographer contract & client-workflow template pack**
  - What: discipline-specific contract templates, model releases, inquiry-to-booking email sequences and a timeline questionnaire.
  - Who buys: independent wedding and portrait photographers.
  - Why now: freelance contract templates show buyer proof (a ~$11.55 template has 106 ratings), and photographers resent HoneyBook price hikes.
  - Sources: MS shortlist #2, PH#2.
- **C30. AI acceptable-use policy kit for one regulated profession**
  - What: an AI-use policy, client-disclosure language, a tool-vetting checklist and a staff training sheet tailored to solo/small law firms, therapy practices or accounting firms.
  - Who buys: owners of solo and small regulated practices.
  - Why now: Bluevine and Clio 2026 surveys show most have no AI policy and distrust AI, and bar and licensing boards keep issuing AI guidance.
  - Sources: PH#6, TR#15.

## Seed hypotheses: Phase 2 view, before validation

| Seed | Candidate(s) | Phase 1 lean |
|---|---|---|
| 1 Skill packs for non-dev professions | C01-C04 | Support **narrowly** (one vertical, installable, $29-$69); generic absorbed by free official plugins |
| 2 Get found by AI search | C11 (+C10, C12) | Real shift, crowded tooling; only a vertical, plain-English, GBP/reviews/schema re-scope survives |
| 3 EU AI Act starter packs | C16 | Likely reject (softened duty, saturated) |
| 4 Accessibility fix kits | C17 | Support with careful claims |
| 5 MCP connectors / setup guides | C06 (+C10) | Connectors rejected (aggregators publish 700-1,900 servers each); guides weak |
| 6 Voice receptionist templates | C07 | Support only as an agency-facing, per-trade pack with compliance scripts |
| 7 Brand voice packs | C09 | Likely reject (absorbed, $9 anchor) |
| 8 Chatbot QA kits | C08 | Unproven |
| 9 School AI policy packs | C26 | Likely reject |
| 10 SOP-to-agent converters | C05 | Likely reject (free Microsoft/Anthropic tools) |
