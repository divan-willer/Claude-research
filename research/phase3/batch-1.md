# Phase 3 validation, batch 1: vertical AI skill packs (C01-C05; seeds 1 and 10)

Validator #1, 2026-11-01. 20 of 20 allowed WebSearch calls used. GitHub was checked through raw.githubusercontent.com and `gh api`.

## Score table

| id | name | demand | competition (5 = low) | wtp | buildability | distribution | growth | total | verdict |
|---|---|---|---|---|---|---|---|---|---|
| C01 | HVAC & plumbing "AI office manager" skill pack | 3 | 2 | 3 | 4 | 2 | 2 | **16** | WEAK |
| C02 | Bookkeeper month-end close skill pack (QBO/Xero) | 2 | 1 | 2 | 4 | 2 | 2 | **13** | REJECT |
| C03 | Therapist private-practice documentation kit (no PHI) | 4 | 2 | 4 | 4 | 4 | 3 | **21** | VIABLE (only as a template kit, not an AI kit) |
| C04 | Realtor AI listing & follow-up kit with fair-housing guardrails | 3 | 1 | 2 | 5 | 3 | 3 | **17** | WEAK (do not build) |
| C05 | SOP-to-agent instruction converter | 2 | 1 | 1 | 4 | 2 | 1 | **11** | REJECT (fatal: free official tools) |

## The four key questions

1. **Do paid profession-specific Claude kits sell for these four professions?** Barely, and not as Claude skills.
   - The Gumroad search returned **no** Claude skill pack for HVAC, plumbing, realtors, therapists or bookkeepers. It found only generic Claude packs (e.g. [Claude Skills Pack](https://thinkaiprompt.gumroad.com/l/claude-skills) and [Freelance Toolkit for Claude Code](https://ribster014.gumroad.com/l/voqthx)).
   - What does exist is cheap multi-model **prompt PDFs** on Etsy and Gumroad:
     - HVAC: $14.99 with "6 ratings".
     - Plumbing: $14.99 with "6 ratings".
     - Cleaning-business toolkit: "19 sales" and "Be the first to review this item".
     - Realtor bundles: $1.50-$28. Bookkeeping packs: mostly $5-$20, including an $8 "AI Bookkeeping Toolkit for Claude".
   - Phase 1's rated Claude kits (designers $70 with 42 ratings, lawyers $39 with 11) are for **other** professions (MS#20).
   - The one strong willingness-to-pay signal in this batch is **non-AI**: therapy note templates on Etsy with hundreds of reviews.
2. **Do free official plugins cover them?** Largely yes, for C01, C02 and C05.
   - Anthropic's free **Claude for Small Business** plugin ([README](https://raw.githubusercontent.com/anthropics/knowledge-work-plugins/main/small-business/README.md), v1.35.1, 2026-09-15) covers most of their workflows:
     - `proposal-builder` turns "a voice memo, jobsite photos … or scrappy notes" into a "costed proposal, estimate" ([SKILL.md](https://raw.githubusercontent.com/anthropics/knowledge-work-plugins/main/small-business/skills/proposal-builder/SKILL.md)).
     - `close-month` and `month-end-prep` reconcile "the ledger against every connected payment processor" and need "MYOB, NetSuite, QuickBooks, Xero, or Zoho Books", with a CSV fallback ([SKILL.md](https://raw.githubusercontent.com/anthropics/knowledge-work-plugins/main/small-business/skills/close-month/SKILL.md)).
     - Also included: `review-reputation`, `reactivate` (win-back), `invoice-chase`, `speed-to-lead`, and "Automate this — turn a task you repeat into a named skill".
   - Intuit's official `intuit-quickbooks` plugin is in the official marketplace ([marketplace.json](https://raw.githubusercontent.com/anthropics/claude-plugins-official/main/.claude-plugin/marketplace.json)).
   - The free 44-profession set ([alexclowe README](https://raw.githubusercontent.com/alexclowe/awesome-claude-cowork-plugins/main/README.md)) ships ready-made plugins for all four professions:
     - Tradesperson: `/estimate`, `/scope-of-work`, `/customer-email`
     - Bookkeeper: `/reconciliation-report`, `/client-email`
     - Therapist: `/session-note`, `/treatment-plan`, `/hipaa-check`
     - Real Estate Agent: `/listing-description`, `/cma-narrative`
3. **Where do these buyers gather, and is promotion allowed?**
   - **r/therapists:** ads are "removed WITHOUT WARNING", and a weekly self-promotion thread exists.
   - **r/Bookkeeping:** Rule 1 "No self-promotion" and Rule 2 "No commercial spam" (relayed from mirrors).
   - **r/hvacadvice:** only homeowners and end users post (2022 rules).
   - **r/HVAC** and **r/realtors** promotion rules: NOT VERIFIED.
   - **Facebook groups:** NOT VERIFIED.
   - **Etsy** is the only channel where buyer search traffic is evident. It is strong for therapy note templates and realtor prompts, and thin for trades.
4. **Is the SOP converter killed by the free tools?** Yes. All of these are free and do the job:
   - Anthropic `skill-creator` ([SKILL.md](https://raw.githubusercontent.com/anthropics/skills/main/skills/skill-creator/SKILL.md))
   - the Claude for Small Business "Automate this" feature
   - Microsoft Skill Recorder ([README](https://raw.githubusercontent.com/microsoft/skill-recorder/main/README.md): "Record yourself doing a task once, then turn it into a skill")
   - the strands-agents SOP→SKILL.md converter ([deepwiki](https://deepwiki.com/strands-agents/agent-sop/4.3-anthropic-skills))
   - 84 GitHub repos for "sop to skill"

**Seed 1 (profession skill packs):** reject the "Claude skill pack" framing for these four professions. Only C03 survives, and only as an Etsy template kit with an optional no-PHI AI workflow.

**Seed 10 (SOP converter):** reject.

---

## C01. HVAC & plumbing "AI office manager" skill pack (16, WEAK)

**Rationale.**
- The free official Claude for Small Business plugin already does quotes from voice memos and jobsite photos, review replies, win-back, invoice chasing and speed-to-lead. The free 44-profession set adds a tradesperson `/estimate`.
- That leaves only Jobber/Housecall Pro export-awareness and maintenance-agreement renewals as differentiation.
- Paid trade AI kits on Etsy are $5-$50 prompt PDFs with single-digit ratings. Trade owners are not a proven Etsy or Gumroad audience.

**Best-scoped version.** Drop "AI office manager". Build an "HVAC Service-Agreement Renewal & Quote Follow-up Kit":
- a Google Sheets agreement tracker with renewal dates 60/90 days out
- 12 SMS/email templates (renewal, tune-up booking, quote follow-up)
- one optional Claude/ChatGPT project instruction that reads a Jobber/HCP customer CSV and drafts the week's renewal texts

Sell it on Etsy as a spreadsheet kit, not an AI kit. This overlaps C24 and should probably merge into it.

**Target buyer.** Owner-operator of a 1-5 truck residential HVAC shop that sells maintenance plans and runs them from a spreadsheet or a basic Jobber tier.

**Demand evidence.**
- A Florida HVAC owner asks how others use Claude in their business (r/HVAC mirror, about Mar 2026): https://reddit.sentinel-team.org/posts/1srtoqs/snapshots/2026-04-25T02%3A30%3A13.962987Z
- Other HVAC-related snapshots were returned, including one asking what helped with estimating, dispatching and admin (only the title or opener is visible): https://reddit.sentinel-team.org/posts/1slagzc/snapshots/2026-04-17T17%3A16%3A47.061327Z
- A contractor cut nightly admin from about 3 h to 30 min with AI estimates (r/automation mirror, Apr 2026, PH#9): https://reddit.sentinel-team.org/posts/1sn2lxy/snapshots/2026-04-24T19%3A29%3A23.242902Z
- An industry symposium session, "The small HVAC owner's guide to AI workflows that actually work": https://www.hvacrschool.com/events/7th-annual-hvac-r-training-symposium/the-small-hvac-owners-guide-to-ai-workflows-that-actually-work/
- A ServiceTitan community thread on "ChatGPT - Estimates/Quotes" (date unknown): https://community.servicetitan.com/t5/Estimates/ChatGPT-Estimates-Quotes/m-p/40122
- The maintenance-agreement pain (PH#31) has vendor-only evidence. No r/HVAC thread was found.

**Competition snapshot.**

Paid, on Etsy:
- "HVAC Business AI Toolkit | 90 ChatGPT Prompts, 5 Automations": $14.99, "6 ratings".
- Plumbing twin: $14.99, "6 ratings".
- "AI Office Starter Package for HVAC Companies – 60 Prompts, 6 Workflows": $37-$49.78, no sales seen.
- A multi-trade kit with 60 ChatGPT and Claude prompts: $10.
- A 120-prompt home-service pack: $5.59.
- 150 prompts for builders, electricians and plumbers: $31.83.
- [AI for Contractors Prompt Guide](https://www.etsy.com/listing/4357247077/ai-for-contractors-prompt-guide-roofing).
- [Home Services AI Manager Tool](https://www.etsy.com/listing/4513471732/home-services-ai-manager-tool-59-sales). The URL slug says "59-sales"; this is unverified.
- The cleaning-business analogue shows "19 sales" ([listing](https://www.etsy.com/listing/4489958284/cleaning-business-email-templates)).
- The specific HVAC and plumbing listings above appeared in Etsy search results ([ai_business_toolkits](https://www.etsy.com/market/ai_business_toolkits), [construction_ai_prompts](https://www.etsy.com/market/construction_ai_prompts)).

Free:
- Claude for Small Business: `proposal-builder`, `review-reputation`, `reactivate`, `invoice-chase`, `speed-to-lead`.
- alexclowe `tradesperson` plugin.
- GitHub: [miron-tech/hvac-claude-skills](https://github.com/miron-tech/hvac-claude-skills) (6 stars), [KRASA-AI/plumbing-ai-skills](https://github.com/KRASA-AI/plumbing-ai-skills) (0 stars). The "hvac claude" query returns 59 repos.
- Free SEO content: [claudecoworkcourse HVAC](https://claudecoworkcourse.com/blog/chatgpt-for-hvac-businesses), [techpresso HVAC prompt library](https://academy.techpresso.co/prompts/hvac-companies), [ACHR News "10 free ways"](https://achrnews.com/articles/152896-10-free-ways-to-boost-your-hvac-business-with-chatgpt).

**Kill reasons.**
1. The free official SMB plugin covers about 60-70% of the listed workflows.
2. Claude skills need a paid Claude plan, and installing them is a hurdle for non-technical trade owners (Phase 1 G6).
3. Etsy trade-AI listings show single-digit ratings.
4. No buyer community with verified promotion rules.

**Price.** $19-$29 as a Sheets plus templates kit. Don't price above $29 given the $10-$15 anchors.

**Launch channels.**
- Etsy (spreadsheet kit): listings exist, so search traffic is plausible but thin.
- r/HVAC: promotion rules NOT VERIFIED.
- r/hvacadvice: "mods, homeowners, and end users should be the only people making posts" (2022 rules), so it is the wrong audience: https://lr.eu.psf.lt/r/hvacadvice/comments/wz8vhy/subreddit_rules_august_2022/is7wgjy/?context=3
- HVAC owner Facebook groups: NOT VERIFIED.

**Biggest risk.** Trade owners don't buy "AI kits" on Etsy or Gumroad, and the free official plugin absorbs what's left. **Cheapest test:**
- Publish one $19 Etsy listing (about $0.20 fee) with the agreement tracker and texts, and run Etsy Ads at $1-2/day for 7 days.
- Kill the idea if it gets fewer than 300 views or 0 sales.

**Build notes.**
- Sheets tracker with conditional-format renewal flags, templates in Google Docs, one SKILL.md and a 5-page setup PDF. About 5 h.
- Jobber/HCP CSV column names must be taken from public help docs; no test account is needed for a CSV-based skill.

## C02. Bookkeeper month-end close skill pack (13, REJECT)

**Rationale.**
- The core job is already free and official. Claude for Small Business `close-month`/`month-end-prep` reconciles QBO, Xero, MYOB or Zoho ledgers against payment processors and writes the P&L narrative.
- Intuit ships its own Claude plugin and connector. It went live in Claude on about 23 Apr 2026, and invoice write actions were announced at Intuit Connect on 27 Oct 2026 (secondary sources).
- The free alexclowe `bookkeeper` plugin adds `/reconciliation-report` and `/client-email`.
- Etsy already sells month-end close checklists with Claude prompts, and $8 Claude bookkeeping toolkits.
- Bookkeeper buyer demand for a Claude pack is unevidenced, and r/Bookkeeping bans self-promotion.

**Best-scoped version.** None as a Claude pack. The only gap left is multi-client bookkeeper work: client query emails about uncategorised transactions, and document chasing. That belongs in C22 (doc-chasing Sheets kit), not here.

**Target buyer.** A solo bookkeeper with 10-40 QBO/Xero clients.

**Demand evidence.**
- A thread on replacing a VA by connecting Claude to QuickBooks via MCP (May 2026; an r/automation-style thread, not r/Bookkeeping): https://reddit.sentinel-team.org/posts/1t6a6ic/snapshots/2026-05-08T21%3A35%3A13.515039Z
- Receipt-chasing threads (May 2026, PH#8): https://reddit.sentinel-team.org/posts/1tfkkpn/snapshots/2026-05-22T21%3A52%3A38.863292Z
- Vendor and tutorial content only: https://findskill.ai/blog/claude-quickbooks-month-end-close-bookkeeper/ and https://www.claudecodehq.com/blog/claude-accountants-month-end-close-stack (Oct 23 2026; says the connector suits report questions, not line-level month-end matching).
- No r/Bookkeeping thread found.

**Competition snapshot.**

Paid, on Etsy ([bookkeeper_templates](https://www.etsy.com/market/bookkeeper_templates), [ai_for_accounting](https://www.etsy.com/fr/market/ai_for_accounting?page=2), [marketing_and_finance_ai_prompts](https://www.etsy.com/market/marketing_and_finance_ai_prompts)):
- A month-end close kit: "22-step checklist, an Excel workbook with 5 tabs, 7 AI prompts for Claude and ChatGPT".
- "AI Bookkeeping Toolkit for Claude | Small Business Finance Agents" at $8.00.
- 100- and 110-prompt bookkeeper packs. Most cost $5-$20; no sales counts were visible.

Free:
- Claude for Small Business `close-month`, `month-end-prep`, `invoice-chase`, `tax-season-organizer`.
- Intuit `intuit-quickbooks` official plugin and connector ([marketplace.json](https://raw.githubusercontent.com/anthropics/claude-plugins-official/main/.claude-plugin/marketplace.json); [Insightful Accountant](https://insightfulaccountant.com/accounting-tech/general-ledger/intuit-announces-expansion-of-claude-and-chatgpt-connectivity/); [nexairi](https://nexairi-mentis.pages.dev/article/Accounting/quickbooks-turbotax-claude-intuit-cpa-guide/)).
- alexclowe `bookkeeper` plugin.
- GitHub: vpodugu/startup-bookkeeper (20 stars). The "bookkeeping claude skills" query returns 51 repos.

**Kill reasons.**
1. A free official tool does the same core job: `close-month` plus the Intuit plugin.
2. r/Bookkeeping Rule 1 "No self-promotion" and Rule 2 "No commercial spam", plus a mod post about the "uptick" in tool announcements (mirrors: https://lr.eu.psf.lt/r/bookkeeping, https://reddit.sudovanilla.org/r/Bookkeeping, https://reddit.sentinel-team.org/posts/1q6byd3/snapshots/2026-01-12T01%3A40%3A27.562937Z).
3. The price anchor is $5-$20.

**Price.** Do not build. If folded into C22, $29-$39.

**Launch channels.**
- r/Bookkeeping: no self-promotion (rules relayed via a user comment on a mirror; full current text NOT VERIFIED).
- QuickBooks ProAdvisor groups: NOT VERIFIED.
- Etsy: listings exist; no sales seen.

**Biggest risk.** Intuit and Anthropic keep extending the free layer: invoice writes were added in Oct 2026. **Cheapest test:** none worth running. Test C22 instead.

**Build notes.** Buildable in a day from CSV exports. Live-connector testing needs a QBO sandbox (not verified as free in this run).

## C03. Therapist private-practice documentation kit, no PHI (21, VIABLE)

**Rationale.**
- This is the only candidate in the batch with real willingness-to-pay evidence. Etsy therapy-note template bundles sell at $9-$18 and show 580-836 reviews.
- The pain is constant: evening note-writing, and AI scribes at about $35 per clinician per month (PH#1).
- The market is crowded, though, and "AI" is not the differentiator. Etsy already has "AI Progress Notes Prompt Guide for Therapists", "No PHI" and "HIPAA Compliant Templates" listings, and the free alexclowe `therapist` plugin has `/session-note` and `/hipaa-check`.
- It wins only as a better template kit for a sharper niche, with the AI workflow as a bonus.

**Best-scoped version.** An "Insurance-Ready Progress Note Kit for [one niche]", e.g. LPCs/LCSWs billing insurance for anxiety and depression, or child/play therapy:
- a Google Sheets note builder (dropdown → DAP/SOAP/BIRP narrative)
- a medical-necessity and intervention phrase bank
- a treatment-goal bank
- a 1-page "de-identified shorthand → note" Claude/ChatGPT project instruction, with an explicit no-PHI rule
- a client AI-use consent template

Sell on Etsy.

**Target buyer.** A solo private-practice LPC, LCSW or LMFT who bills insurance and writes notes in the evening.

**Demand evidence.**
- r/therapists mirror threads, Jan-Jun 2026 (PH#1): https://reddit.sentinel-team.org/posts/1qporha/snapshots/2026-01-29T01%3A51%3A20.500236Z, https://reddit.sentinel-team.org/posts/1sdnt0u/snapshots/2026-04-09T17%3A33%3A54.651862Z, https://reddit.sentinel-team.org/posts/1tk7l4p/snapshots/2026-05-22T06%3A54%3A50.751336Z, https://reddit.sentinel-team.org/posts/1tvy83a/snapshots/2026-06-04T12%3A20%3A34.255191Z
- NPR/WFAE, 2026-05-26: https://www.wfae.org/united-states-world/2026-05-26/therapists-are-using-ai-to-take-notes-is-it-a-useful-tool-or-a-breach-of-trust
- Vendor content about therapists using ChatGPT or Claude for notes and the HIPAA risk: https://findskill.ai/blog/chatgpt-therapy-notes-hipaa/, https://www.icanotes.com/?p=37547, https://mentalyc.com/blog/using-chatgpt-for-therapy-notes

**Competition snapshot.**

Paid, on Etsy. Review counts are as shown on the listing page and may be shop-wide, not per-item:
- [SOAP DAP BIRP Notes Builder Bundle](https://www.etsy.com/listing/4443073237/soap-dap-birp-notes-builder-bundle): $14.40 (from $18), 827-836 reviews, a Sheets builder.
- [Therapy Note Taking Templates](https://www.etsy.com/listing/4333200272/therapy-note-taking-templates-soap-dap): $14.06 (from $35.14), 614 reviews.
- A Therapy Session Notes Generator: $8.99 (from $14.99), 580 reviews.
- A $2.99 template with a medical-necessity phrase bank.
- [Couples Therapy Progress Notes](https://www.etsy.com/listing/4457555827/couples-therapy-progress-notes-therapy).
- AI prompt guides for therapists ([AI Prompt Pack for Therapists & Coaches](https://www.etsy.com/listing/4504821073/ai-prompt-pack-for-therapists-coaches), [chatgpt_prompts_for_therapist](https://www.etsy.com/market/chatgpt_prompts_for_therapist), [therapy_note_generator](https://www.etsy.com/market/therapy_note_generator)).
- On Gumroad, only generic psychologist prompt packs ([ismailsaleem](https://ismailsaleem.gumroad.com/l/ChatGPT-Prompts-for-Psychologist)). No therapist progress-note Claude pack was found.

Free:
- alexclowe `therapist` plugin.
- GitHub: carrie-lypp/claude-therapist (24 stars). The "therapist claude skills" query returns 8 repos.
- Free SOAP/DAP templates on vendor blogs.

Paid SaaS:
- BAA-covered scribes (Mentalyc, Upheal), and SimplePractice's AI add-on at about $35/month (PH#1).

**Kill reasons.** Not fatal, but serious:
1. A crowded Etsy category with entrenched high-review leaders.
2. Liability: a template must never claim "HIPAA compliant". Consumer ChatGPT and Claude are not HIPAA-covered without a BAA, per the vendor sources above.
3. Many therapists distrust AI notes (NPR).

**Price.** $17-$24 one-time on Etsy, with list prices at about $29 and launch sales. Incumbents anchor at $9-$18 after discount.

**Launch channels.**
- Etsy: strong buyer search. Many listings with hundreds of reviews exist.
- r/therapists: ads are "removed WITHOUT WARNING", and there is a weekly "CEUs, Resources, Self-Promos" thread (mirrors: https://reddit.sentinel-team.org/posts/1ttri99/snapshots/2026-06-02T09%3A49%3A38.052873Z, https://reddit.sentinel-team.org/posts/1rrw7qx/snapshots/2026-03-13T10%3A12%3A09.430076Z). Frequency and limits are NOT VERIFIED.
- Therapist Facebook groups: NOT VERIFIED.

**Biggest risk.** A new zero-review listing can't outrank the 600-800-review incumbents. **Cheapest test:**
- List the niche kit on Etsy at $19 with $2/day Etsy Ads for 10 days. Target fewer than 3 sales before deciding whether to expand.
- Post once in the r/therapists weekly self-promo thread.

**Build notes.** Doable in about 6 h:
- Sheets builder with data-validation dropdowns and concatenation formulas
- Docs templates and the phrase bank
- one project-instruction file and the disclaimers

Clinical phrasing must be checked against payer medical-necessity language. Add a "not clinical, legal or billing advice" disclaimer and a no-PHI instruction.

## C04. Realtor AI listing & follow-up kit with fair-housing guardrails (17, WEAK; do not build)

**Rationale.**
- This is the most saturated niche in the batch. Etsy and Gumroad carry dozens of realtor ChatGPT/Claude prompt bundles priced from $1.50 to about $28, including 100-500+ prompt libraries.
- Free fair-housing AI guides exist, and the free alexclowe `real-estate` plugin includes `/listing-description` and `/cma-narrative`.
- Demand rests on one NAR survey. Phase 1 already flagged real estate as crowded (G4).

**Best-scoped version.** None worth a build day. If forced: a $9-$12 "Fair-Housing Listing Word Check" Google Sheet that flags risky phrases in pasted listing copy. It is a lead magnet at best.

**Target buyer.** An individual residential agent who uses ChatGPT for listings.

**Demand evidence.**
- NAR 2026 tech report: 63% cite the learning curve (PH#7): https://www.nar.realtor/newsroom/realtors-adopt-technology-to-save-time-and-improve-the-client-experience-nar-report-finds and https://www.nar.realtor/news/real-estate-news/technology/the-tech-real-estate-agents-rely-on-most-in-2026
- No r/realtors threads were found in this run.

**Competition snapshot.**

Paid, on Etsy:
- [real_estate_chatgpt_prompts](https://www.etsy.com/market/real_estate_chatgpt_prompts)
- [100 ChatGPT Prompts for Realtors](https://www.etsy.com/listing/4316721928/100-chatgpt-prompts-for-realtors-real)
- [Real Estate AI Prompt Library Bundle 100+](https://www.etsy.com/au/listing/4350932972/real-estate-ai-prompt-library-bundle-100)
- [ChatGPT Package for Real Estate Agents](https://www.etsy.com/listing/4370531065/chatgpt-package-for-real-estate-agents)
- [75 AI Prompts for Real Estate Agents](https://www.etsy.com/se-en/listing/4489720803/75-ai-prompts-for-real-estate-agents)
- Prices run from about $1.50 to about $28 (400+ prompt bundles exist). No reviews were visible in the snippets.

Paid, on Gumroad:
- [True Prompts real estate kit](https://trueprompts.gumroad.com/l/realestateprompts)
- [VortexDev 500+ prompts](https://vortexdev0.gumroad.com/l/ai-prompts-real-estate)
- [ismailsaleem](https://ismailsaleem.gumroad.com/l/ChatGPT-Prompts-for-Real-Estate-Sales-Agent)
- [Aivenue Master Prompt Vault](https://aivenuelabs.gumroad.com/l/ujibd)
- [AI Workshop Prompt Vault](https://theaiworkhop.gumroad.com/l/klxpsq)
- [AI Real Estate Marketing Kit 2.0](https://digitalwealthwithsa.gumroad.com/l/airealstate)
- Gumroad has a dedicated [realtor tag](https://gumroad.com/business-and-money/real-estate?tags=realtor).

Free:
- alexclowe `real-estate` plugin.
- GitHub: [zubair-trabzada/ai-realestate-claude](https://github.com/zubair-trabzada/ai-realestate-claude) (187 stars). The "real estate agent claude skills" query returns 40 repos.
- Free fair-housing AI guides: [howaiworks](https://howaiworks.ai/use-cases/ai-for-real-estate-listings), [theaicareerlab](https://theaicareerlab.com/professions/real-estate).

**Kill reasons.**
1. Dozens of near-identical products at $1.50-$28.
2. Free profession plugins and free guides.
3. Fair-housing claims carry liability that lands on the agent's license, so the guardrail can't be sold as a guarantee.

**Price.** $9-$12 if built at all.

**Launch channels.**
- Etsy and Gumroad: heavy buyer search, but saturated.
- r/realtors: the sidebar says "Follow the rules"; self-promotion rules NOT VERIFIED (https://reddit.sentinel-team.org/posts/1th24mr/snapshots/2026-05-20T07%3A13%3A12.584101Z).
- Realtor Facebook groups: NOT VERIFIED.

**Biggest risk.** The listing gets buried among 100+ near-identical listings. **Cheapest test:** don't spend the build day. If curious, look at the review counts of the top 10 Etsy "real estate chatgpt prompts" listings; this was not visible in search snippets.

**Build notes.** Trivial (about 3 h). The difficulty is entirely distribution.

## C05. SOP-to-agent instruction converter (11, REJECT, fatal)

**Rationale.**
- A free official tool does exactly this job:
  - Anthropic's `skill-creator` ("Create new skills … from scratch").
  - Claude for Small Business ships "Automate this — turn a task you repeat into a named skill" and `build-agent`.
  - Microsoft Skill Recorder turns a recorded session into a SKILL.md.
  - strands-agents has an SOP→SKILL.md converter.
- No paid converter with sales was found. Buyers have no reason to pay for something Claude does natively when told "turn this SOP into a skill".

**Best-scoped version.** None as a converter. Pre-written vertical SOP skills (e.g. "12 front-office SOPs for a dental office") can be a section inside a vertical kit.

**Target buyer.** An SMB owner documenting processes. Already served for free.

**Demand evidence.**
- Owners complain about undocumented processes (PH#19): https://reddit.sentinel-team.org/posts/1sxq3ki/snapshots/2026-04-28T10%3A30%3A37.832533Z (Apr 2026) and https://reddit.sentinel-team.org/posts/1pn8tys/snapshots/2025-12-16T04%3A11%3A49.657895Z (Dec 2025).
- That pain is about writing SOPs, not converting them to agents. No buyer demand for conversion was found.

**Competition snapshot.**

Free:
- [anthropics skill-creator](https://raw.githubusercontent.com/anthropics/skills/main/skills/skill-creator/SKILL.md)
- Claude for Small Business "Automate this" / `build-agent` ([README](https://raw.githubusercontent.com/anthropics/knowledge-work-plugins/main/small-business/README.md))
- [microsoft/skill-recorder](https://raw.githubusercontent.com/microsoft/skill-recorder/main/README.md)
- [strands-agents SOP→skills converter](https://deepwiki.com/strands-agents/agent-sop/4.3-anthropic-skills)
- [skills.sh "Skills Maker"](https://www.skills.sh/diegosouzapw/awesome-omni-skill/agent-33-skills-maker) ("convert any workflow description, SOP document … into a Claude Desktop skill package")
- Free how-tos: [MindStudio](https://www.mindstudio.ai/blog/skill-creator-workflow-claude-code-sop-to-skill), [Elite AI Advantage](https://eliteaiadvantage.com/how-to/claude-skill-sop-for-team)
- GitHub search counts: "sop to skill" 84 repos, "sop skill claude" 133 (e.g. charlesdove977/procedure-ops, 63 stars).

Paid, on Etsy:
- Only generic "Custom GPT Instructions Builder" and Claude-skill packs ([ai_agent_template](https://www.etsy.com/market/ai_agent_template), [chatgpt_custom_instructions](https://www.etsy.com/market/chatgpt_custom_instructions)). No SOP converter, and no sales seen.

**Kill reasons.**
1. Fatal: free official and platform-native tools from Anthropic and Microsoft.
2. No willingness-to-pay evidence.
3. A web-tool version would need a paid LLM API backend.

**Price.** n/a. At most a free lead magnet.

**Launch channels.** None credible. Etsy shows only adjacent "AI agent template" searches; promotion rules NOT VERIFIED.

**Biggest risk.** It is already absorbed. **Cheapest test:** none recommended.

**Build notes.** A SKILL.md version takes under 1 h, which is itself the problem. A web version needs API keys and cost control.

---

## Method & limitations

**WebSearch: 20 calls, all used.**
- Etsy, scoped to `allowed_domains`: HVAC, therapist, realtor, bookkeeper, SOP and therapy-template queries.
- Gumroad: profession skill packs, therapist, realtor.
- Reddit mirrors: demand threads and subreddit rules.
- Plain web: Intuit connector, SOP converters.

**GitHub, free:**
- raw.githubusercontent.com for the Anthropic SMB plugin README, its skills and `.mcp.json`, the official marketplace.json, alexclowe's README, skill-creator and skill-recorder.
- `gh api search/repositories` for profession repo counts.
- api.github.com repo metadata was blocked for non-attached repos, so star counts come from search results only.

**Caveats:**
- Etsy review counts come from search-tool summaries of listing pages. They may be shop-level, not per-listing. Sales counts were visible for only one listing (cleaning, 19 sales).
- Etsy and Gumroad prices are snapshots and may be in mixed currencies.
- Subreddit rules come from third-party mirrors and are partial:
  - r/HVAC and r/realtors self-promotion rules: NOT VERIFIED.
  - Facebook groups: not checkable.
- Intuit launch dates (23 Apr 2026; 27 Oct 2026 write actions) come from secondary sites, not Intuit's newsroom.
- The Claude for Small Business launch date: SiliconANGLE says 13 May 2026, and the README is v1.35.1 dated 15 Sep 2026.
- No WebFetch was possible, so no listing page was opened directly.

## Sources

Free official and open-source:
- https://raw.githubusercontent.com/anthropics/knowledge-work-plugins/main/small-business/README.md
- https://raw.githubusercontent.com/anthropics/knowledge-work-plugins/main/small-business/skills/proposal-builder/SKILL.md
- https://raw.githubusercontent.com/anthropics/knowledge-work-plugins/main/small-business/skills/close-month/SKILL.md
- https://raw.githubusercontent.com/anthropics/knowledge-work-plugins/main/small-business/skills/review-reputation/SKILL.md
- https://raw.githubusercontent.com/anthropics/knowledge-work-plugins/main/small-business/skills/reactivate/SKILL.md
- https://raw.githubusercontent.com/anthropics/knowledge-work-plugins/main/small-business/.mcp.json
- https://raw.githubusercontent.com/anthropics/claude-plugins-official/main/.claude-plugin/marketplace.json
- https://raw.githubusercontent.com/alexclowe/awesome-claude-cowork-plugins/main/README.md
- https://raw.githubusercontent.com/anthropics/skills/main/skills/skill-creator/SKILL.md
- https://raw.githubusercontent.com/microsoft/skill-recorder/main/README.md
- https://deepwiki.com/strands-agents/agent-sop/4.3-anthropic-skills
- https://www.skills.sh/diegosouzapw/awesome-omni-skill/agent-33-skills-maker
- https://www.mindstudio.ai/blog/skill-creator-workflow-claude-code-sop-to-skill
- https://eliteaiadvantage.com/how-to/claude-skill-sop-for-team
- https://siliconangle.com/2026/05/13/anthropic-launches-claude-small-business-new-automation-workflows/
- https://insightfulaccountant.com/accounting-tech/general-ledger/intuit-announces-expansion-of-claude-and-chatgpt-connectivity/
- https://nexairi-mentis.pages.dev/article/Accounting/quickbooks-turbotax-claude-intuit-cpa-guide/

Etsy:
- https://www.etsy.com/listing/4357247077/ai-for-contractors-prompt-guide-roofing
- https://www.etsy.com/listing/4513471732/home-services-ai-manager-tool-59-sales
- https://www.etsy.com/listing/4489958284/cleaning-business-email-templates
- https://www.etsy.com/market/construction_ai_prompts
- https://www.etsy.com/market/ai_business_toolkits
- https://www.etsy.com/listing/4443073237/soap-dap-birp-notes-builder-bundle
- https://www.etsy.com/listing/4333200272/therapy-note-taking-templates-soap-dap
- https://www.etsy.com/listing/4457555827/couples-therapy-progress-notes-therapy
- https://www.etsy.com/listing/4504821073/ai-prompt-pack-for-therapists-coaches
- https://www.etsy.com/market/chatgpt_prompts_for_therapist
- https://www.etsy.com/market/therapy_note_generator
- https://www.etsy.com/market/real_estate_chatgpt_prompts
- https://www.etsy.com/listing/4316721928/100-chatgpt-prompts-for-realtors-real
- https://www.etsy.com/au/listing/4350932972/real-estate-ai-prompt-library-bundle-100
- https://www.etsy.com/listing/4370531065/chatgpt-package-for-real-estate-agents
- https://www.etsy.com/se-en/listing/4489720803/75-ai-prompts-for-real-estate-agents
- https://www.etsy.com/market/bookkeeper_templates
- https://www.etsy.com/fr/market/ai_for_accounting?page=2
- https://www.etsy.com/market/marketing_and_finance_ai_prompts
- https://www.etsy.com/market/ai_agent_template
- https://www.etsy.com/market/chatgpt_custom_instructions

Gumroad:
- https://thinkaiprompt.gumroad.com/l/claude-skills
- https://ribster014.gumroad.com/l/voqthx
- https://ismailsaleem.gumroad.com/l/ChatGPT-Prompts-for-Psychologist
- https://trueprompts.gumroad.com/l/realestateprompts
- https://vortexdev0.gumroad.com/l/ai-prompts-real-estate
- https://ismailsaleem.gumroad.com/l/ChatGPT-Prompts-for-Real-Estate-Sales-Agent
- https://aivenuelabs.gumroad.com/l/ujibd
- https://theaiworkhop.gumroad.com/l/klxpsq
- https://digitalwealthwithsa.gumroad.com/l/airealstate
- https://gumroad.com/business-and-money/real-estate?tags=realtor

Demand and community (Reddit mirrors and other):
- https://reddit.sentinel-team.org/posts/1srtoqs/snapshots/2026-04-25T02%3A30%3A13.962987Z
- https://reddit.sentinel-team.org/posts/1slagzc/snapshots/2026-04-17T17%3A16%3A47.061327Z
- https://reddit.sentinel-team.org/posts/1sn2lxy/snapshots/2026-04-24T19%3A29%3A23.242902Z
- https://reddit.sentinel-team.org/posts/1t6a6ic/snapshots/2026-05-08T21%3A35%3A13.515039Z
- https://reddit.sentinel-team.org/posts/1tfkkpn/snapshots/2026-05-22T21%3A52%3A38.863292Z
- https://reddit.sentinel-team.org/posts/1ttri99/snapshots/2026-06-02T09%3A49%3A38.052873Z
- https://reddit.sentinel-team.org/posts/1rrw7qx/snapshots/2026-03-13T10%3A12%3A09.430076Z
- https://reddit.sentinel-team.org/posts/1q6byd3/snapshots/2026-01-12T01%3A40%3A27.562937Z
- https://reddit.sentinel-team.org/posts/1th24mr/snapshots/2026-05-20T07%3A13%3A12.584101Z
- https://lr.eu.psf.lt/r/bookkeeping
- https://reddit.sudovanilla.org/r/Bookkeeping
- https://lr.eu.psf.lt/r/hvacadvice/comments/wz8vhy/subreddit_rules_august_2022/is7wgjy/?context=3
- https://www.hvacrschool.com/events/7th-annual-hvac-r-training-symposium/the-small-hvac-owners-guide-to-ai-workflows-that-actually-work/
- https://community.servicetitan.com/t5/Estimates/ChatGPT-Estimates-Quotes/m-p/40122
- https://claudecoworkcourse.com/blog/chatgpt-for-hvac-businesses
- https://academy.techpresso.co/prompts/hvac-companies
- https://achrnews.com/articles/152896-10-free-ways-to-boost-your-hvac-business-with-chatgpt
- https://findskill.ai/blog/claude-quickbooks-month-end-close-bookkeeper/
- https://www.claudecodehq.com/blog/claude-accountants-month-end-close-stack
- https://findskill.ai/blog/chatgpt-therapy-notes-hipaa/
- https://www.icanotes.com/?p=37547
- https://mentalyc.com/blog/using-chatgpt-for-therapy-notes
- https://howaiworks.ai/use-cases/ai-for-real-estate-listings
- https://theaicareerlab.com/professions/real-estate

Relayed from Phase 1 (PH#1, #7, #8, #9, #19; MS#20; G3-G5, G12; TR#1, #19). URLs as cited above, from `research/phase1/pain-hunter.md`, `marketplace-saturation-scout.md`, `ai-ecosystem-gaps.md` and `trend-scout.md`.
