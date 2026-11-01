# Final report: 10 one-day digital products worth building (Nov 2026)

Prepared 1 Nov 2026 by the lead researcher.

Inputs:
- Phase 1: 5 research files, in `research/phase1/`
- Phase 2: 30 candidates, in `research/phase2/candidates.md`
- Phase 3: 6 validator batches, in `research/phase3/batch-*.md` and `.json`

## Read this first: the blunt summary

- **Nothing scored STRONG.** No candidate reached 22/30 on the six-criterion rubric.
  - The best five tie at 21/30, rated VIABLE.
  - Every validator went looking for reasons to reject, and most ideas died.
  - Expect **modest** sales, not a breakout. The binding constraint is **distribution**, not the build.
  - Gumroad is winner-take-most. In an Aug 2026 crawl of 8,311 products, 43% had no ratings. ([dataset](https://github.com/sujeito-operator/gumroad-market-data))
- **Most of the "AI-native" seed ideas lose to free official tools.** Anthropic's free **Claude for Small Business** plugin already does:
  - quotes from voice memos
  - month-end close in QuickBooks and Xero
  - review replies and invoice chasing
  - "turn a task into a skill"

  There are also a free official brand-voice plugin, free vendor MCP servers, Microsoft's free skill-recorder, and a free set of 44 profession plugins. ([plugin README](https://raw.githubusercontent.com/anthropics/knowledge-work-plugins/main/small-business/README.md), [44-profession set](https://raw.githubusercontent.com/alexclowe/awesome-claude-cowork-plugins/main/README.md))
  - The validators found conflicting launch dates for the small-business plugin: 13 May 2026 and a 15 Sep 2026 version. Either way, it is live and free.
- **The ideas that survive are less exciting.** They fall into two groups:
  1. **Template kits for a narrow vertical**, sold where buyers already search (Etsy, TPT).
  2. **Kits driven by a regulation or platform change**, for non-technical people facing a dated deadline or a rejection:
     - ADA demand letters
     - A2P 10DLC rejections (the US registration that business text-messaging campaigns need)
     - UK Making Tax Digital, April 2027
     - Etsy's AI-rule change of 22 Oct 2026
- **Platform risk for this founder: Etsy's 22 Oct 2026 AI policy.** Seven of the top 10 would sell on Etsy.
  - Reported content of the policy:
    - AI use must be disclosed.
    - AI prompt bundles are prohibited.
    - AI-generated "functional guides" (instructions, patterns) are banned.
    - Repeat violations can close a shop.
  - Sources: [Etsy Seller Handbook](https://www.etsy.com/seller-handbook/article/1522733284810), [Digital Commerce 360](https://www.digitalcommerce360.com/2026/10/26/etsy-ai-policy/amp/), [Value Added Resource](https://www.valueaddedresource.net/etsy-bans-ai-patterns/).
  - Caveat: we read these through search summaries, so the exact clause wording is unconfirmed.
  - **Rule for every Etsy product below:**
    - Lead with templates and spreadsheets.
    - Write and edit the instructional text yourself.
    - Disclose AI assistance.
    - Sell any prompt or skill files on Gumroad, not Etsy.

## How this was done, and what to trust

- **Phase 1:** 5 parallel research agents.
- **Phase 2:** the lead synthesised 30 candidates, including all 10 seed hypotheses.
- **Phase 3:** 6 parallel validators, 5 candidates each. Each one was told to search for competitors and free alternatives and to score down when evidence was missing.
- **Network limits:**
  - This cloud environment's network policy blocked direct page fetches to Reddit, Gumroad, Etsy, TPT, Product Hunt, HN and most blogs. Only github.com loaded.
  - Evidence therefore comes from web-search result summaries, plus the GitHub, npm and MCP-registry APIs and Gumroad scrape datasets hosted on GitHub.
  - Reddit threads appear as **mirror URLs** (reddit.sentinel-team.org), because search returned those, not reddit.com.
  - Etsy and TPT review counts come from search snippets. Some may be **shop-level, not listing-level**.
- **Search budget:** web search had a shared cap of about 200 calls per run. Three of the five Phase 1 agents ran with **zero** web searches and used GitHub and registry data instead. Phase 3 validators got 20 searches each.
- **Skipped step:** the Phase 1 completeness critic and gap-fill step was cancelled when you asked me to speed up. The Phase 3 validators closed the biggest gap, which was checking Etsy and TPT directly via search.
- **Posting rules:** most subreddit and community posting rules could **not** be verified (marked NOT VERIFIED below). Read each sidebar before posting. The rules that were confirmed came from mirror copies and are noted as such.
- **Recency:** most demand evidence is dated Jan to Oct 2026. Undated items are flagged.

**Assumptions (no questions asked, per the brief):**
- The founder has no existing audience.
- Sales are in USD or GBP through Etsy, TPT, Gumroad or Lemon Squeezy.
- "One day" means a static kit or simple Sheets/Apps Script, with no backend and no vendor partner approvals.
- Compliance-adjacent kits are sold as checklists and templates with "not legal/tax advice" wording, never as "makes you compliant". The FTC's $1M order against accessiBe for unsupported compliance claims is the precedent. ([fkks](https://technologylaw.fkks.com/post/102jsmj/ftc-finds-website-overlay-tool-failed-to-deliver-accessibility-promises))

## Full ranking (all 30 candidates)

Each criterion is scored 1-5. "Comp" is low competition, so 5 means almost no competitors. Total is out of 30. Ties are broken by demand, then willingness to pay (WTP). Any candidate with Comp = 1 (hundreds of near-identical products, or a free official tool) drops below the others on the same total, per your saturation rule.

| Rank | ID | Candidate | Dem | Comp | WTP | Build | Dist | Growth | Total | Verdict |
|---|---|---|---|---|---|---|---|---|---|---|
| 1 | C03 | Therapist progress-note kit (no client data) | 4 | 2 | 4 | 4 | 4 | 3 | **21** | VIABLE |
| 2 | C17 | Shopify ADA letter-response & fix workbook (seed 4) | 4 | 3 | 3 | 4 | 3 | 4 | **21** | VIABLE |
| 3 | C18 | A2P 10DLC agency pack | 4 | 2 | 3 | 5 | 3 | 4 | **21** | VIABLE |
| 4 | C24 | Single-trade ops spreadsheet kit (absorbs C01) | 3 | 2 | 4 | 5 | 4 | 3 | **21** | VIABLE |
| 5 | C21 | UK Making Tax Digital landlord records workbook | 3 | 2 | 3 | 4 | 4 | 5 | **21** | VIABLE |
| 6 | C07 | Voice-agent launch-safety kit for agencies (seed 6, absorbs seed 8) | 3 | 2 | 3 | 3 | 4 | 4 | **19** | VIABLE |
| 7 | C12 | FTC- and Google-safe review-request kit (absorbs seed 2) | 3 | 2 | 2 | 5 | 4 | 3 | **19** | VIABLE |
| 8 | C14 | Etsy AI-policy listing audit kit | 3 | 2 | 2 | 5 | 3 | 4 | **19** | VIABLE |
| 9 | C27 | Report-card comment bank, one curriculum (Comp = 1) | 3 | 1 | 4 | 5 | 4 | 2 | **19** | VIABLE, conditional |
| 10 | C22 | Missing-docs tracker for US tax preparers | 2 | 2 | 3 | 4 | 3 | 3 | **17** | WEAK |
| 11 | C28 | Independent tutor business kit | 2 | 1 | 3 | 5 | 4 | 3 | 18 | Excluded: saturated (validator) |
| 12 | C23 | Freelancer "get paid" kit | 4 | 1 | 2 | 5 | 3 | 2 | 17 | REJECT (free templates and built-in invoicing reminders) |
| 13 | C29 | Photographer contract & workflow pack | 3 | 1 | 3 | 4 | 4 | 2 | 17 | WEAK |
| 14 | C04 | Realtor AI listing kit (seed 1) | 3 | 1 | 2 | 5 | 3 | 3 | 17 | WEAK |
| 15 | C01 | HVAC/plumbing Claude skill pack (seed 1) | 3 | 2 | 3 | 4 | 2 | 2 | 16 | WEAK, merge into C24 |
| 16 | C19 | UK DUAA complaints procedure pack (data-protection law) | 2 | 2 | 2 | 5 | 3 | 2 | 16 | WEAK |
| 17 | C13 | Agentic-commerce readiness checklist | 3 | 2 | 2 | 4 | 2 | 2 | 15 | WEAK |
| 18 | C11 | "Get found by AI" kit (seed 2) | 2 | 1 | 2 | 4 | 3 | 3 | 15 | WEAK, fold into C12 |
| 19 | C15 | Vibe-coder launch safety kit | 3 | 1 | 2 | 4 | 3 | 2 | 15 | REJECT (Lovable's built-in pre-publish scan; free Cloudflare skill) |
| 20 | C30 | AI-use policy kit for one regulated profession | 3 | 1 | 2 | 4 | 2 | 3 | 15 | REJECT (free bar, APA and AICPA templates) |
| 21 | C16 | EU AI Act starter pack (seed 3) | 2 | 1 | 2 | 4 | 3 | 2 | 14 | REJECT |
| 22 | C08 | Chatbot QA kit (seed 8) | 1 | 2 | 2 | 5 | 2 | 2 | 14 | WEAK, fold into C07 |
| 23 | C20 | CA/NY auto-renewal kit | 1 | 2 | 2 | 5 | 2 | 2 | 14 | REJECT (Stripe built-ins) |
| 24 | C02 | Bookkeeper month-end skill pack (seed 1) | 2 | 1 | 2 | 4 | 2 | 2 | 13 | REJECT (free official close-month skill) |
| 25 | C09 | Brand voice pack (seed 7) | 1 | 1 | 2 | 5 | 3 | 1 | 13 | REJECT (free official plugin) |
| 26 | C25 | TAKE IT DOWN Act pack | 1 | 2 | 2 | 4 | 2 | 2 | 13 | REJECT |
| 27 | C26 | School/tutoring AI policy pack (seed 9) | 1 | 1 | 2 | 5 | 2 | 2 | 13 | REJECT |
| 28 | C10 | "Agent-ready local business" MCP kit | 1 | 3 | 1 | 3 | 2 | 2 | 12 | REJECT |
| 29 | C06 | Claude connector setup kit (seed 5) | 2 | 1 | 2 | 3 | 2 | 1 | 11 | REJECT |
| 30 | C05 | SOP-to-agent converter (seed 10) | 2 | 1 | 1 | 4 | 2 | 1 | 11 | REJECT |

### Seed hypotheses: final verdicts

| # | Seed | Verdict | Why (details in the batch files) |
|---|---|---|---|
| 1 | Claude Code / agent skill packs for non-developer professions | **Rejected as "skill packs"** (C01 16, C02 13, C04 17). Survives only as a template kit (C03). | The free official SMB plugin covers about 60-70% of the trades and bookkeeping workflows. A free 44-profession plugin set exists. Paid trade AI kits on Etsy show single-digit ratings. Buyers need a paid Claude plan and must get through plugin installs (batch-1). |
| 2 | "Get found by AI search" kits | **Weak (15)**; use as a bonus inside C12 | Free graders (BrightLocal, HubSpot, Ahrefs). A free claude-seo skill with about 25k stars. The official SMB plugin has an AI-visibility skill. llms.txt showed no measurable effect (batch-3, REG#4). |
| 3 | EU AI Act starter packs | **Rejected (14)** | The Digital Omnibus softened Art. 4, there are no EU fines, and there are no small-business deadlines in the next 6 months. Etsy kits run $2.95-$499, and one AI-generated Gumroad catalogue holds 42 such products (batch-4). |
| 4 | Accessibility fix kits for Shopify/Wix | **Viable, Shopify only (21)** | Real demand-letter panic. Wix has a free built-in Accessibility Wizard. High claims risk (batch-4). |
| 5 | MCP connectors / setup guides | **Rejected (11)** | Aggregators publish 700-1,900 hosted MCP servers each. Official vendor servers exist. Setup failures are vendor bugs that a guide can't fix (Phase 1 G1/G6, batch-2). |
| 6 | Voice receptionist templates | **Viable only re-scoped (19)** as a compliance and test kit for agencies | Plain per-trade prompts already sell on Etsy and come free with Skool memberships (batch-2). |
| 7 | Brand voice packs | **Rejected (13)** | A free official brand-voice plugin exists (by Tribe AI). Prices are anchored at $9. |
| 8 | Chatbot test/QA kits | **Weak (14)**; fold into C07 | No buyers or sellers found. Free vendor checklists exist. |
| 9 | AI usage policy packs for schools/tutoring | **Rejected (13)** | No tutoring mandate found. TPT sells AI agreements for $0.99 or free, and state model policies are free (batch-6). |
| 10 | SOP-to-agent instruction converters | **Rejected (11)** | Anthropic's skill-creator, the SMB plugin's "Automate this" and Microsoft's Skill Recorder already do this free (batch-1). |

---

## The top 10

Prices are one-time unless stated otherwise. "Mirror" means the evidence came through a Reddit mirror page that search returned, not reddit.com itself.

### 1. Insurance-Ready Progress Note Kit for private-practice therapists (C03, 21/30)

**Pitch.** A Google Sheets note builder plus phrase banks that let a solo therapist write a defensible DAP, SOAP or BIRP note in 3 minutes, without putting client data into any AI tool.

**Target buyer.** Solo private-practice therapists (LPC, LCSW, LMFT) who bill insurance and write notes in the evening. Pick one sub-niche for the title, such as adult anxiety and depression, or child and play therapy.

**Evidence of demand.**
- r/therapists documentation threads in Jan, Apr, May and Jun 2026 (mirror):
  - [Jan](https://reddit.sentinel-team.org/posts/1qporha/snapshots/2026-01-29T01%3A51%3A20.500236Z)
  - [Apr](https://reddit.sentinel-team.org/posts/1sdnt0u/snapshots/2026-04-09T17%3A33%3A54.651862Z)
  - [May](https://reddit.sentinel-team.org/posts/1tk7l4p/snapshots/2026-05-22T06%3A54%3A50.751336Z)
  - [Jun](https://reddit.sentinel-team.org/posts/1tvy83a/snapshots/2026-06-04T12%3A20%3A34.255191Z)
- [NPR/WFAE, May 2026](https://www.wfae.org/united-states-world/2026-05-26/therapists-are-using-ai-to-take-notes-is-it-a-useful-tool-or-a-breach-of-trust): therapists use AI for notes, with real client-trust concerns.
- Existing spend: AI scribes and the SimplePractice add-on cost about $35 per clinician per month (Phase 1 PH#1).

**Competition snapshot.**
- **Etsy is crowded, but it proves people pay.** These review counts may be shop-level:
  - [SOAP DAP BIRP Notes Builder Bundle](https://www.etsy.com/listing/4443073237/soap-dap-birp-notes-builder-bundle): $14.40, about 827-836 reviews shown.
  - [Therapy Note Taking Templates](https://www.etsy.com/listing/4333200272/therapy-note-taking-templates-soap-dap): $14.06, 614 shown.
  - A [notes generator](https://www.etsy.com/market/therapy_note_generator): $8.99, 580 shown.
- Free: alexclowe's therapist plugin, and vendor blog templates.
- **Where this is different:** one niche, insurance-ready medical-necessity phrasing, a goal and objective bank, and a client AI-use consent template. "AI" is a bonus, not the headline, because many therapists distrust AI notes.

**What to build.**

Files:
- `Progress-Note-Builder` (Google Sheets, with an Excel copy). Tabs:
  - How-to
  - DAP builder, SOAP builder and BIRP builder (dropdowns that assemble the note with TEXTJOIN)
  - Interventions by modality (CBT, DBT, ACT, MI, person-centred)
  - Client response
  - Medical-necessity phrases
  - Goals and objectives
  - Risk documentation phrases
- `Phrase-Bank.pdf`: 300+ phrases.
- `Treatment-Goals-Bank.docx`.
- `Client-AI-Use-Consent-Template.docx`, marked "have your board or attorney review".
- `Quick-Start.pdf`.
- *Gumroad edition only:* `No-PHI-AI-Workflow.pdf`, a de-identified shorthand method plus one project instruction. Keep this off Etsy because of the prompt-bundle ban.

Tech: Google Sheets formulas. Claude Code drafts the phrase banks, which you then hand-edit. Playwright renders HTML mockups to PNG for listing images.

Hour-by-hour:

| Hour | Work |
|---|---|
| 1 | Pick the niche. Check Etsy search for niche terms and note what the incumbents miss. Outline the tabs. |
| 2 | Build the Sheets skeleton, dropdowns and note-assembly formulas. |
| 3 | Draft the intervention and client-response banks with Claude. Hand-edit against payer medical-necessity language. |
| 4 | Goals and objectives bank, risk-documentation phrases. Wire them into the dropdowns. |
| 5 | Consent template, quick-start guide, disclaimers: not clinical, legal or billing advice; never put PHI into consumer AI; no "HIPAA compliant" claim. |
| 6 | QA: write 5 sample notes end to end in Google Sheets and Excel. Set up a "Make a copy" link. |
| 7 | Mockups, Etsy title and 13 tags, description with AI-assistance disclosure. Gumroad page for the AI edition. |
| 8 | Publish on Etsy and Gumroad. Start Etsy Ads at $2/day. Post in the r/therapists weekly thread. |

**Price.** $19 on Etsy (list at $24 with a launch discount). $27 on Gumroad with the AI-workflow bonus. Incumbents anchor at $9-18, so don't go above about $29.

**Launch on day one.**
- **Etsy** search: "therapy notes template", "SOAP note template", "DAP notes". This is the main channel. ([market page](https://www.etsy.com/market/therapy_soap_notes_template))
- **r/therapists:** ads are "removed WITHOUT WARNING", but there is a weekly "CEUs, Resources, Self-Promos" thread. Post only there. Seen via [mirror](https://reddit.sentinel-team.org/posts/1ttri99/snapshots/2026-06-02T09%3A49%3A38.052873Z); frequency and limits NOT VERIFIED.
- **Gumroad** for the AI edition.
- Therapist Facebook groups: rules NOT VERIFIED.

**Biggest risk.** A new zero-review Etsy listing can't outrank the 600-800-review incumbents. **Cheap test:** $19 listing plus $2/day Etsy Ads for 10 days. Kill it if there are fewer than 3 sales.

### 2. Shopify ADA Letter Response & Fix Workbook (C17, 21/30, seed 4)

**Pitch.** For the Shopify merchant who just got a law-firm accessibility letter: a calm 48-hour triage checklist, a dated fix log, and click-by-click Shopify fixes for the issues these letters usually allege. All of it hands off to a lawyer and claims no compliance outcome.

**Target buyer.** US Shopify store owners (roughly $100k-$2M/yr revenue) who received, or fear, an ADA demand letter. Secondary buyers are freelancers asked to "fix it fast".

**Evidence of demand.**
- Shopify Community threads (dates not shown in results):
  - [Merchant panic after a law-firm letter](https://community.shopify.com/t/need-help-got-a-letter-from-a-lawfirm-stating-my-site-is-not-compliance-for-blind-poeple/575477)
  - [Long ADA-lawsuit thread](https://community.shopify.com/t/ada-accessibility-lawsuits/351516/14): letters cite alt text, unlabeled buttons and forms, contrast and keyboard access; "Most are templates".
  - [Merchant sued, asking for help](https://community.shopify.com/t/ada-compliance-lawsuit-company-to-help/230778) (older)
- [EcomBack mid-2026 report](https://www.ecomback.com/ada-website-lawsuits-recap-report/2026-mid-year-ada-website-lawsuit-report): 2,045 ADA website suits in H1 2026; Phase 1 cites about 79% against e-commerce.

**Competition snapshot.**
- Etsy has generic and multi-platform kits:
  - a [Shopify & WooCommerce Accessibility Kit](https://www.etsy.com/market/accessibility_audit) and audit PDFs, priced from a few dollars to about $90
  - an attorney-drafted ["ADA Compliant Website" bundle](https://www.etsy.com/listing/4296587607/the-creators-guide-to-an-ada-compliant)
  - no visible reviews on any of them
- Gumroad has generic WCAG guides.
- Free: the [W3C statement generator](https://github.com/w3c/wai-statements), free Claude accessibility skills, and 122 "shopify accessibility" GitHub repos.
- Wix has a free built-in [Accessibility Wizard](https://support.wix.com/en/article/accessibility-about-the-accessibility-wizard-5119725), so **drop Wix entirely**.
- **Where this is different:** Shopify-only, built around the *letter* moment (triage, evidence log, attorney hand-off pack), with click paths verified in Dawn. It is not another generic WCAG guide.

**What to build.**

Files:
- `Letter-Triage-48h.pdf`: what to preserve, forward to counsel, and not say. Framed as an organiser, not legal advice.
- `Shopify-Fix-Guide-Dawn.pdf`: screenshots for:
  - alt text
  - icon-button labels
  - form labels
  - colour contrast via theme settings
  - focus traps in the cart drawer and keyboard navigation
  - video captions
- `Remediation-Log` (Google Sheets): issue, WCAG reference, page, fix, date, evidence link, status.
- `Accessibility-Statement-Template.docx`.
- `Attorney-Handoff-Pack.docx`.
- `Overlay-Warning.pdf`: why a widget is not protection, citing the FTC/accessiBe order.

Tech: a free Shopify Partner development store on Dawn, plus free axe DevTools or Lighthouse for screenshots.

Hour-by-hour:

| Hour | Work |
|---|---|
| 1 | List the common allegations from the Shopify Community threads. Set up a Partner dev store on Dawn. |
| 2-3 | Reproduce each fix in Dawn admin and screenshot it. |
| 4 | Remediation-log Sheet with conditional formatting. |
| 5 | Statement template, attorney hand-off pack, overlay warning. |
| 6 | Claims pass: delete every "compliant", "lawsuit-proof" and "protects you". Add "not legal advice" and a "current as of Nov 2026" stamp. |
| 7 | Mockups and listing copy (Etsy plus Gumroad). |
| 8 | Publish. Answer 5 Shopify Community letter threads with free, link-free steps. |

**Price.** $29 standard edition. $49 "letter received" edition with the remediation log and attorney pack.

**Launch on day one.**
- **Etsy:** "accessibility audit" and "ADA website" market pages exist; Etsy's AI-disclosure rules apply.
- **Gumroad.**
- **Shopify Community:** give help without links. A third-party copy of the developer-community code says promotion belongs only in designated areas ([source](https://cleverence.com/articles/shopify-dev-documentation/code-of-conduct-shopify-developer-community-6893)); merchant-forum rules NOT VERIFIED.
- **r/ecommerce** bans self-promotion ([mirror](https://reddit.sentinel-team.org/subreddits/ecommerce/snapshots/2025-12-20T08%3A30%3A17.413923Z)), so don't post there.
- r/shopify: NOT VERIFIED.

**Biggest risk.** Two of them:
- **Legal claims:** the FTC's $1M accessiBe order shows that compliance promises draw enforcement.
- **Buyer behaviour:** panicked merchants may hire a lawyer or buy an app instead.

**Cheap test:** 14 days on Etsy at $29. Kill it if there are fewer than 2 sales or fewer than 20 favourites.

### 3. A2P 10DLC Agency Pack for GoHighLevel and Twilio (C18, 21/30)

**Pitch.** Everything an agency needs to get client SMS campaigns approved on the first or second try. Agencies resell GoHighLevel (GHL) as a white-label CRM, and A2P 10DLC is the carrier registration US business texting requires. The pack covers 10 industries:
- campaign descriptions and sample messages
- privacy and terms clauses
- opt-in copy
- a current table mapping each rejection code to its fix
- a client intake form

**Target buyer.** GoHighLevel and white-label agency owners registering 5-50 client sub-accounts. Secondary: DIY small-business owners on Twilio or GHL.

**Evidence of demand.**
- Zoom Community: [campaign rejected 20+ times](https://community.zoom.com/t5/Zoom-Phone-System/10DLC-Registration-failed-over-and-over/m-p/191089).
- Zoom Community: [brand-name mismatch rejection](https://community.zoom.com/t5/Zoom-Phone-System/10DLC-SMS-Campaign-Rejected-due-to-Brand-name-not-consistent/m-p/218393).
- Sinch Community: ["Why was my campaign rejected"](https://community.sinch.com/t5/10DLC/Why-was-my-10DLC-campaign-rejected/m-p/15408).
- 5+ Fiverr gigs selling rejection fixes, e.g. [this one](https://fiverr.com/prada_os/setup-ghl-a2p-10dlc-fix-rejection-and-sms-compliance).
- GitHub: 174 "sms privacy policy" repos created since Twilio's 30 Jun 2026 mandate (gh api, 1 Nov 2026).
- Twilio introduced granular rejection codes on 23 Mar 2026 ([GHL Scale Up](https://www.ghlscaleup.com/blog/a2p-error-codes-explained)).

**Competition snapshot.**
- One paid Gumroad guide: ["The No-Guesswork A2P Setup for GoHighLevel"](https://theapexintelligence.gumroad.com/l/whfrb) with an "Approval Prep Kit".
- One [Etsy helper](https://www.etsy.com/listing/4435251968/twilio-a2p-10dlc-registration-helper-sms).
- Fiverr services, and agency done-for-you setups at $799-1,500.
- **Strong free alternatives:**
  - [GHL help article](https://help.gohighlevel.com/support/solutions/articles/155000001426-a2p-opt-in-form-privacy-policy-and-terms-and-conditions-guidelines)
  - [Hot Prospector's free generator](https://hotprospector.com/a2p-compliance-guide/funnel-generator)
  - [MessageDesk's free checker](https://www.messagedesk.com/free-tools/privacy-policy-generator)
- **Where this is different:** multi-vertical, an **agency licence**, and a dated, sourced rejection-code table. The free tools only cover the privacy-policy page.

**What to build.**

Files:
- `Rejection-Code-Fix-Table` (Google Sheets): code, meaning, fix, Twilio documentation link, last-checked date.
- `Clause-Library.docx`: SMS privacy and terms clauses (program name, frequency, rates, STOP/HELP, no sharing of mobile data).
- `Vertical-Campaign-Sets.docx`: 10 verticals × campaign description, 2-5 sample messages and opt-in checkbox copy.
- `Opt-in-Screenshot-Checklist.pdf`.
- `Brand-Data-Consistency-Checklist.pdf`: legal name, EIN, domain email, website.
- `Client-Intake-Form` (Google Form template).
- `Agency-SOP.pdf`.
- A free lead magnet: the top-15 rows of the code table.

Hour-by-hour:

| Hour | Work |
|---|---|
| 1 | Gather Twilio error-code docs, TCR rejection reasons and the GHL requirements. Choose the 10 verticals. |
| 2 | Build the code table, with every row sourced and dated. |
| 3 | Clause library. |
| 4 | Vertical campaign sets and opt-in copy. |
| 5 | Brand-data checklist, intake form, SOP. |
| 6 | Lead-magnet extract. Disclaimers: "no approval guaranteed", "not legal advice", TCPA consent caution. Changelog. |
| 7 | Gumroad product pages and covers. |
| 8 | Publish. Post the free table in GHL communities after reading their rules. |

**Price.** $29 single-business edition. $79 agency licence covering unlimited clients.

**Launch on day one.**
- **Gumroad.** A direct competitor already sells there, so the channel works for this.
- GHL Facebook groups and community: rules NOT VERIFIED.
- r/gohighlevel: NOT VERIFIED.
- Optional: a productised Fiverr "A2P pre-submission review" gig that uses the kit (Fiverr ToS NOT VERIFIED).

**Biggest risk.** Agencies use the free GHL docs and generators and never pay. Some rejections come from brand data, which no template fixes. **Cheap test:** free lead magnet for 14 days. Kill it at fewer than 50 downloads and 0 upsells.

### 4. One-Payment HVAC Office Workbook: estimates to invoices to maintenance-agreement renewals (C24 + C01, 21/30)

**Pitch.** A phone-friendly Google Sheets kit that replaces the parts of Jobber a 1-3-person HVAC shop actually uses: price book, estimate, job, invoice, money owed, and a maintenance-agreement renewal tracker that flags renewals 60 and 90 days out. One payment, no monthly fee.

**Target buyer.** Solo and 1-3-truck residential HVAC owner-operators who sell maintenance plans and won't pay $49-149/month for field-service software. If eRank shows an HVAC incumbent with 500+ reviews, switch to pressure washing.

**Evidence of demand.**
- Local-service owner [replaced a $200/month field-service subscription](https://reddit.sentinel-team.org/posts/1sdtcl7/snapshots/2026-04-09T20%3A34%3A38.462784Z) (Apr 2026, mirror).
- [Field-service software too complex on a phone](https://reddit.sentinel-team.org/posts/1tlc4zu/snapshots/2026-05-29T21%3A30%3A12.687798Z) (May 2026, mirror).
- [Contractor cut nightly admin from about 3h to 30 min](https://reddit.sentinel-team.org/posts/1sn2lxy/snapshots/2026-04-24T19%3A29%3A23.242902Z) (Apr 2026, mirror).
- Jobber price changes in 2026 ([PricingSaaS Q2 2026](https://pricingsaas.com/companies/jobber/diffs/2026Q2)), though price trackers conflict.
- An HVAC-R school symposium session on [AI workflows for small HVAC owners](https://www.hvacrschool.com/events/7th-annual-hvac-r-training-symposium/the-small-hvac-owners-guide-to-ai-workflows-that-actually-work/) (2026).

**Competition snapshot.**
- Etsy trades spreadsheets sell, which proves willingness to pay, but they are crowded and cheap ([market page](https://www.etsy.com/market/lawn_care_business_planner_templates)):
  - a landscaping bundle at $8.76 showing "(3.5k)" reviews, possibly shop-level
  - one at $3.99 with 185 reviews
  - a $13.78 tracker with 84 reviews
- HVAC AI prompt kits show only single-digit ratings ([market page](https://www.etsy.com/market/ai_business_toolkits)).
- **Where this is different:**
  - single trade, HVAC-specific
  - a maintenance-agreement renewal engine, which no listing found offers
  - a Jobber/Housecall Pro CSV import tab
  - phone-first layout

**What to build.**

Files:
- `HVAC-Office-Workbook` (Google Sheets). Tabs:
  - Start Here
  - Price Book
  - Estimates (auto-numbered, PDF export)
  - Jobs
  - Invoices
  - Money Owed (AR aging)
  - Maintenance Agreements (renewal flags)
  - Customers
  - CSV Import (column map taken from Jobber and HCP public help docs)
- `Text-and-Email-Templates.pdf`: renewal reminders, quote follow-ups, payment reminders. Write these yourself; templates carry less risk under Etsy's rules.
- `Quick-Start.pdf`.
- Optional: an Apps Script button that drafts the renewal texts.

Hour-by-hour:

| Hour | Work |
|---|---|
| 1 | eRank free tier and Etsy search: confirm there is no 500+-review HVAC leader, or switch trades. |
| 2-3 | Core flow: price book, estimate, job, invoice. |
| 4 | Money-owed tab, agreement tracker with conditional formatting, CSV import tab. |
| 5 | Phone test in the Google Sheets mobile app; simplify. |
| 6 | Templates and quick-start. |
| 7 | Mockups, Etsy copy with a "no monthly fee" comparison (cite the source for any price). |
| 8 | Publish. Start Etsy Ads at $1-2/day. |

**Price.** $19 (range $14-24). Anything above about $29 fights a $4-14 price anchor.

**Launch on day one.**
- **Etsy:** "HVAC spreadsheet", "contractor invoice template", "service agreement tracker".
- r/HVAC: NOT VERIFIED.
- r/hvacadvice: homeowners and end users only (2022 rules via [mirror](https://lr.eu.psf.lt/r/hvacadvice/comments/wz8vhy/subreddit_rules_august_2022/is7wgjy/?context=3)), so don't post there.
- r/sweatystartup and HVAC Facebook groups: NOT VERIFIED.

**Biggest risk.** A new listing can't outrank $4-9 incumbents with hundreds of reviews. **Cheap test:** 21 days of $1-2/day Etsy Ads. You need at least 1% conversion on 500+ views.

### 5. UK Making Tax Digital Landlord Records Workbook, 2026/27 and 2027/28 editions (C21, 21/30)

**Pitch.** A spreadsheet for UK landlords who refuse to switch to Xero. It keeps records in HMRC's property categories, handles joint owners and multiple properties, and produces a quarterly summary that imports into a named bridging tool, so there is no copy-paste. It comes with a one-page April 2027 sign-up and quarterly-deadline guide.

**Target buyer.** UK landlords with 1-4 properties and £30k-£50k qualifying income, who keep spreadsheets today and are mandated from 6 Apr 2027. Do a sole-trader edition second.

**Evidence of demand.**
- About 970k more people are mandated in Apr 2027 ([The Register](https://www.theregister.com/2026/04/10/mtd_hmrc/)); MoneyWeek puts the wave at [about 1,077,000](https://moneyweek.com/economy/small-business/what-you-need-to-know-about-making-tax-digital).
- HMRC is [contacting taxpayers who missed the first quarterly update](https://www.att.org.uk/technical/news/hmrc-contact-taxpayers-who-missed-first-mtd-quarterly-update-deadline) (ATT, 2026).
- A buyer asking about [bridging software](https://singletrackworld.com/forum/off-topic/making-tax-digital-mild-panic-is-bridging-software-a-good-idea-and-any-recommendations-pls) (date unknown).
- ["Tried using existing Make Tax Digital tools. Gave up. Built my own."](https://reddit.sentinel-team.org/posts/1qec57t/snapshots/2026-01-16T11%3A40%3A13.507681Z) (Jan 2026, mirror).

**Competition snapshot.**
- Etsy already has an MTD cluster, with no review counts visible:
  - a [landlord joint-owners sheet at $10.48](https://www.etsy.com/uk/market/landlord_excel_spreadsheet)
  - the [MTDMadeSimple shop](https://www.etsy.com/ca/shop/MTDMadeSimple)
  - a [music-teacher edition](https://www.etsy.com/listing/4600080866/music-teacher-bookkeeping-spreadsheet-uk)
  - "hmrc spreadsheet uk" [runs to at least 4 result pages](https://www.etsy.com/market/hmrc_spreadsheet_uk?page=4)
- **Free software is the bigger threat:**
  - the [GOV.UK finder](https://gov.uk/guidance/find-software-thats-compatible-with-making-tax-digital-for-income-tax) can filter for free products
  - Starling's free tool for its account holders
  - Clear Books' free plan
  - Magic Tax free bridging
  - [NRLA's free bridging template for members](https://www.nrla.org.uk/services/tax/taxd/bridging-template)
- **Where this is different:**
  - landlord-first, with joint-owner splits
  - **proven** to import into one named bridging tool (most listings don't show this)
  - includes the 2027/28 edition and the April 2027 sign-up guide

**What to build.**

Files:
- `MTD-Landlord-Workbook` (Excel and Google Sheets). Tabs:
  - Properties
  - Income
  - Expenses by HMRC property category
  - Joint-owner split
  - Quarterly summary (formatted for bridging import)
  - Year-end
- `MTD-2027-Guide.pdf`: sign-up, choosing a bridging tool, quarterly dates (7 Aug, 7 Nov, 7 Feb, 7 May per batch-5), digital-link rules.
- `Bridging-Import-Walkthrough.pdf` with screenshots.

Hour-by-hour:

| Hour | Work |
|---|---|
| 1 | Read GOV.UK MTD ITSA guidance and the property categories. Pick a free or trial bridging tool. |
| 2-3 | Build the workbook. |
| 4 | **Prove the import works with the bridging tool** (may need an HMRC sandbox or trial account). This is the riskiest hour. |
| 5 | Guide and walkthrough. |
| 6 | Check categories against GOV.UK. Disclaimers: "not HMRC-recognised software", "not tax advice". |
| 7 | Etsy UK mockups and listing. |
| 8 | Publish. Schedule Etsy Ads for Jan-Feb 2027. |

**Price.** £15 per edition (range £12-19), or a £24 landlord + sole-trader bundle. Don't go above about £25.

**Launch on day one.**
- **Etsy UK:** "hmrc spreadsheet uk", "landlord excel spreadsheet", "making tax digital".
- Not verified: r/UKLandlords, r/UKPersonalFinance, Property Tribes and NRLA forums.
- [UK Business Forums](https://www.ukbusinessforums.co.uk/threads/hmrc-making-tax-digital.430470/latest) is full of vendor spam, so contribute rather than promote.

**Biggest risk.** Free recognised software, plus zero-review listings among near-identical sheets. **Cheap test:** landlord edition only, with about £3/day of Etsy Ads over 14 days in Jan-Feb 2027. Kill it below 3 sales. Build now so the listing ages before the peak.

### 6. Voice-Agent Launch-Safety Kit for HVAC and plumbing agencies (C07, 19/30; seed 6, absorbs seed 8)

**Pitch.** Before an agency puts an AI receptionist on a plumber's phone line, this kit covers:
- the state-by-state AI-disclosure and recording-consent opening lines
- an emergency-triage rule block for gas, carbon monoxide and flooding
- 50 scripted test calls with a pass/fail scorecard
- Vapi and Retell tool-schema JSON
- a client go-live sign-off sheet

**Target buyer.** 1-5-person AI-automation agencies and freelancers selling receptionists to home-service businesses on $400-2,000/month retainers.

**Evidence of demand.**
- GitHub "ai receptionist" repos are up 8.8x year on year (Phase 1 TR#3).
- Voice-AI agency communities trade templates:
  - [AI Voice Network](https://www.skool.com/aivoicenetwork/about)
  - [Voice Offer Lab](https://www.skool.com/openautomation-collective-6267)
- Freelancers sell [HVAC/plumbing receptionist builds on Upwork](https://www.upwork.com/services/product/admin-customer-support-build-ai-receptionist-for-hvac-plumbing-electrical-ai-calling-agent-2071660623106302895).
- Phase 1 REG#6 found a fragmented legal layer: the FCC treats AI voices as "artificial", CA AB 2905, Utah, Maine, all-party-consent states, and CIPA wiretap suits.

**Competition snapshot.**
- Per-trade prompts already exist (no reviews visible on any of them):
  - an [Etsy HVAC AI Receptionist Deployment Kit](https://www.etsy.com/au/listing/4539664221/hvac-ai-receptionist-deployment-kit)
  - a [$22 Vapi/Bland/Retell script pack](https://www.etsy.com/market/ai_receptionist)
  - [Ciela](https://ciela.ai/blogs/pre-built-ai-agent-templates-for-agencies) at $49 per template or $99/month
  - a $179/$349 [dental kit](https://dental-voice-bot-kit.vercel.app/)
- Free: Vapi's prompt reference, GitHub starters, and Skool memberships.
- **Where this is different:** nobody found sells the **compliance + test-call + sign-off** layer. Lead with that, not with prompts.

**What to build.**

Files:
- `State-AI-Disclosure-and-Recording-Consent` (Google Sheets): one row per state, cited, "current as of Nov 2026", not legal advice.
- `Opening-Lines-and-Consent-Flows.docx`.
- `Emergency-Triage-Block.md`.
- `50-Test-Calls-and-Scorecard` (Sheets).
- `vapi-tools.json` and `retell-tools.json`: booking, transfer, message-taking.
- `Go-Live-Signoff.docx`.
- `README.pdf`.

Hour-by-hour:

| Hour | Work |
|---|---|
| 1-2 | State table, limited to disclosure states and all-party-consent states, each row cited. |
| 3 | Opening lines, consent flows, emergency block. |
| 4 | Test calls and scorecard. |
| 5-6 | Tool JSON for both platforms, **tested** on a pay-as-you-go Vapi account and number (under $20). |
| 7 | Sign-off sheet, README, disclaimers. Make no HIPAA or BAA claims for Vapi or Retell. |
| 8 | List on Etsy and Gumroad. Post a free "10 state opening lines" sample. |

**Price.** $39 per trade. $79 for an HVAC + plumbing + dental bundle (dental adds a BAA checklist).

**Launch on day one.**
- **Gumroad** and **Etsy**: the "ai receptionist" and "ai voice agent prompts" market pages exist.
- **Skool voice-AI communities:** promotion rules NOT VERIFIED.
- **r/automation:** a mirrored rule says to avoid using it "solely as a platform to advertise ... without genuine engagement" ([GummySearch copy](https://gummysearch.com/r/automation/)). Lead with the free sample.

**Biggest risk.** Agencies see templates as a commodity, and state-law accuracy carries liability. **Cheap test:** first open the competing Etsy listings in a normal browser to read their review counts. Then run a 14-day listing and kill it below 3 sales.

### 7. Google Review Kit for trades: FTC- and Google-policy-safe (C12, 19/30; absorbs seed 2 as a bonus)

**Pitch.** Review cards plus what the $3 cards don't include:
- request scripts for each job stage
- a two-step follow-up cadence
- a staff and family review disclosure policy
- a "never do" list (gating, incentives, in-store iPads)
- 20 response templates
- a bonus "be found in Google's AI answers" Business Profile checklist

**Target buyer.** Owners and office managers of local service businesses (HVAC, plumbing, salons, clinics) who are already searching Etsy for "Google review card".

**Evidence of demand.**
- Reddit (mirror):
  - [Reviews are harder to get than expected](https://reddit.sentinel-team.org/posts/1rq57dr/snapshots/2026-03-11T01%3A23%3A07.053576Z) (Mar 2026)
  - [Real reviews removed, possibly after bulk asks](https://reddit.sentinel-team.org/posts/1sz8u0r/snapshots/2026-05-02T04%3A50%3A06.954017Z) (May 2026)
  - [Another review-problems thread](https://reddit.sentinel-team.org/posts/1tn81br/snapshots/2026-05-26T09%3A47%3A52.470198Z) (May 2026)
- Etsy buyer search pages: ["review request"](https://www.etsy.com/market/review_request) and ["google review card templates"](https://www.etsy.com/market/google_review_card_templates).
- Why now:
  - the FTC brought its first Consumer Review Rule suit in May 2026 (Phase 1 REG#5)
  - in-store review iPads now break Google's rules ([whito](https://whito.co.uk/news/the-ipad-on-your-counter-is-now-breaking-googles-review-rules/))

**Competition snapshot.**
- Cards are a $1-6 Etsy commodity.
- Google provides a [free review link and QR code](https://support.google.com/business/answer/16816815?hl=en).
- Review SaaS blogs give scripts away.
- No standalone *compliant scripts + policy* kit was found.
- **Where this is different:** one trade, the policy-safe layer, and response templates. The cards are just the hero image.

**What to build.**

Files:
- `Review-Cards` (6 Canva share links, QR codes from Google's own link).
- `Request-Scripts.pdf`: 10 SMS and email scripts, written by hand.
- `Follow-Up-Cadence.pdf`.
- `Staff-Review-Disclosure-Policy.docx`.
- `Never-Do-Checklist.pdf`, citing 16 CFR 465 and Google policy.
- `Review-Responses` (Sheets): 20 responses.
- `Bonus-GBP-AI-Visibility-Checklist.pdf`.

Hour-by-hour:

| Hour | Work |
|---|---|
| 1 | Read the FTC rule and Google's review policy. Outline the never-do list. |
| 2 | Scripts and cadence. |
| 3 | Cards in Canva. |
| 4 | Response templates. |
| 5 | GBP/AI checklist (leave out llms.txt). |
| 6 | Hand-edit pass; "aligned with" wording plus "not legal advice". |
| 7 | Mockups and listing. |
| 8 | Publish on Etsy. Post in the r/smallbusiness weekly promotion thread. |

**Price.** $15 on Etsy (range $12-19). $29 for a 3-trade agency pack on Gumroad.

**Launch on day one.**
- **Etsy** card search pages.
- **r/smallbusiness:** self-promotion is allowed only in the weekly "Promote your business" thread (from [2024 mirror copies](https://lr.in.psf.lt/r/smallbusiness/comments/1bn1bpy/promote_your_business_week_of_march_25_2024); current sidebar NOT VERIFIED).

**Biggest risk.** Buyers anchored on $3 cards won't pay $15. **Cheap test:** use the cards as the hero image and put "FTC & Google-safe scripts included" in the title. Kill it at 0 sales after 21 days or 300 views.

### 8. Etsy AI-Policy Listing Audit Kit, Oct 2026 rules (C14, 19/30)

**Pitch.** A Google Sheet that audits each of your Etsy listings against the 22 Oct 2026 AI rules: disclosure, functional-guide risk, image rules and prompt-bundle risk. It comes with ready-to-paste disclosure sentences by product type and an appeal letter for wrongful removals.

**Target buyer.** Etsy digital-download sellers with 50-500 listings (printables, Canva templates, planners, clipart) who used AI somewhere and fear removal or shop closure.

**Evidence of demand.**
- Etsy forum removal threads (dates not shown):
  - [Removed under Creativity Standards](https://community.etsy.com/t5/Technical-Issues/My-listing-was-removed-that-doesn-t-follow-Etsy-s-Creativity/m-p/146483880)
  - [Removed "as AI"](https://community.etsy.com/t5/Technical-Issues/Listing-Removed-for-Violating-Creativity-Standards-as-AI-found/m-p/146482631/highlight/true)
  - [Canva templates the seller made themselves deactivated](https://community.etsy.com/t5/Technical-Issues/Etsy-deactivated-a-bunch-of-Canva-templates-I-made-myself/m-p/146045612/highlight/true)
- Press coverage of the 22 Oct change: [Retail Dive](https://retaildive.com/news/etsy-updates-ai-use-policies-emphasize-craftsmanship/833838) and [Digital Commerce 360](https://www.digitalcommerce360.com/2026/10/26/etsy-ai-policy/amp/).

**Competition snapshot.**
- **No paid compliance kit was found**. That could mean a gap, or no demand.
- Free: Etsy's own [Creativity Standards](https://www.etsy.com/legal/creativity) and [handbook article](https://www.etsy.com/seller-handbook/article/1522733284810), plus blog explainers that appeared within days.
- **Where this is different:** a working per-listing audit tool, disclosure templates and an appeal letter. The free material only explains the rules.

**What to build.**

Files:
- `Listing-Audit` (Google Sheets): per-listing rows, dropdown risk flags, conditional formatting, a summary dashboard.
- `Disclosure-Templates.pdf`: 10 product types, written by hand.
- `Appeal-Letter.docx`.
- `Changelog.md`, dated.

Hour-by-hour:

| Hour | Work |
|---|---|
| 1 | Read the Etsy policy pages and link to them rather than copying them. |
| 2-3 | Audit Sheet. |
| 4 | Disclosure templates. |
| 5 | Appeal letter. |
| 6 | Test on 20 sample listings. |
| 7 | Listing, with your own AI-use disclosure. |
| 8 | Publish. |

Speed matters: the change is fresh, and buyers are worried now.

**Price.** $12 (range $9-15).

**Launch on day one.**
- **Etsy** (dogfooding the rules).
- **Gumroad.**
- r/EtsySellers: NOT VERIFIED.
- Etsy Community forums: assume promotion is prohibited.

**Biggest risk.** Two of them:
- Sellers read Etsy's free page and move on.
- Etsy flags the kit itself under the AI-guide rule.

Make it mostly a tool, hand-written and disclosed. **Cheap test:** a $9 listing within 7 days. Kill it at 0 sales after 21 days.

### 9. Report-Card Comment Bank + Sheets generator for ONE curriculum and grade band (C27, 19/30, conditional)

**Condition.** TPT is saturated for Ontario banks, and Khanmigo plus several free generators handle the generic "generator" job. That is why Comp is scored 1. **Only build this if a 10-minute TPT search for your chosen jurisdiction and grade band shows fewer than about 20 banks.** Otherwise skip it. It is in the top 10 because teachers visibly pay for banks, and the season is **right now**.

**Pitch.** Curriculum-locked report-card comments by strand and achievement level, with a Google Sheets merge that handles pronouns, strengths and next steps from dropdowns. No student data ever goes into an AI tool.

**Target buyer.** Elementary teachers writing 25-30 narrative report cards in a comment-heavy jurisdiction, between now and December.

**Evidence of demand.**
- [Ontario Grades 1-3 bank](https://www.teacherspayteachers.com/Product/Ontario-Report-Card-Comment-Bank-Grades-1-2-3-1679005): 4.72/5 from 203 reviews at $10 (review dates not visible).
- [TPT search](https://www.teacherspayteachers.com/browse?search=report+card+comment+bank): many banks priced free to $20.
- [2026 comparison of AI comment tools](https://findskill.ai/blog/ai-report-card-comments-5-tool-comparison-2026/): the category is active.
- An r/Teachers thread about an AI comment tool ([mirror, Jun 2026](https://reddit.sentinel-team.org/posts/1tw7108/snapshots/2026-06-04T19%3A24%3A55.144009Z)) is a pitch, so it is weak evidence.

**Competition snapshot.**
- Ontario banks exist grade by grade with 200+ reviews. TPT already sells Sheets generators.
- [Khanmigo](https://www.khanmigo.ai/report-card-comments) is free and unlimited, and [Formswrite](https://formswrite.com/tools/report-card-comment-generator) needs no sign-up.
- **Where this is different:** an underserved jurisdiction or grade band, plus a privacy-safe offline generator.

**What to build.**

Files:
- `Comment-Bank.docx`: strands × 4 levels, learning skills, next steps.
- `Comment-Generator` (Google Sheets): dropdowns plus SUBSTITUTE/CONCATENATE pronoun merge.
- `Free-Sample-20-Comments.pdf`.

Hour-by-hour:

| Hour | Work |
|---|---|
| 1 | TPT gap check: go or no-go. |
| 2 | Read the official curriculum documents. |
| 3-4 | Draft comments with Claude and hand-edit them into curriculum language. |
| 5 | Generator Sheet. |
| 6 | Repetition and grammar QA. |
| 7 | TPT listing plus free sample. |
| 8 | Publish. Make Pinterest pins. |

**Price.** $8-10 per grade (the bottom of your band). $25-30 for a multi-grade bundle.

**Launch on day one.**
- **TPT** search for "report card comment bank" and "report card comment generator". Fee tiers NOT VERIFIED.
- A free sample as a lead magnet.
- r/Teachers: NOT VERIFIED.
- Pinterest: not checked.

**Biggest risk.** Invisible next to 200+-review incumbents, and the season ends mid-December. **Cheap test:** build one grade band in about 3 hours, list it this week, and expand only if it sells by mid-December.

### 10. Missing-Docs Tracker for US tax preparers and bookkeepers (C22, 17/30, WEAK)

**Honest note.** This is WEAK. It is #10 because the higher scorers were saturated or rejected, not because the evidence is good. Build it only after a top-5 product shows traction.

**Pitch.** A Google Sheet where each client row ticks off the documents they owe. One button drafts a Gmail email listing *only* the missing items. It comes with SMS nudges and "no organizer, no start" engagement-letter wording, ready before January.

**Target buyer.** Solo US tax preparers and bookkeepers with 30-150 individual or Schedule C clients who don't pay for TaxDome, Karbon or Liscio.

**Evidence of demand (weak).**
- NJCPA, Jan 2026: [don't start until the organizer is back](https://www.njcpa.org/about/ceo-compass/post/njcpa-focus/2026/01/20/6-engagement-letter-tips-for-busy-season).
- A [post on automating receipt-PDF chasing](https://reddit.sentinel-team.org/posts/1tfkkpn/snapshots/2026-05-22T21%3A52%3A38.863292Z) (May 2026, mirror, no body visible).
- A client asking [whether monthly document requests are normal](https://reddit.sentinel-team.org/posts/1u12tvt/snapshots/2026-06-09T23%3A36%3A18.844689Z) (Jun 2026, client side).
- Phase 1 PH#8 rests mostly on vendor sources.
- **No buyer threads asking for this exact tool were found.**

**Competition snapshot.**
- Etsy already sells:
  - a [document request list](https://www.etsy.com/listing/4465613550/bookkeeping-client-document-request-list)
  - [tax organizers](https://www.etsy.com/listing/4390500735/2025-tax-organizer-worksheet-clients-tax)
  - [email libraries at about $10-80](https://www.etsy.com/market/email_to_tax_clients)
- Portal SaaS (Liscio, DocChase) automates the chasing.
- **Where this is different:** the email drafter that lists only the missing items. That feature is hard to show in an Etsy thumbnail.

**What to build.**

Files:
- `Missing-Docs-Tracker` (Google Sheets): document lists by client type (W-2, 1099-NEC/K, Schedule C, rental) and a status grid.
- An Apps Script "Draft reminder emails" menu that creates Gmail drafts.
- `SMS-and-Email-Nudges.pdf`.
- `Engagement-Letter-Clauses.docx`.
- `Quick-Start.pdf`, including the OAuth consent walkthrough.

Hour-by-hour:

| Hour | Work |
|---|---|
| 1 | Document lists. |
| 2-3 | Tracker. |
| 4-5 | Apps Script, tested in a fresh Google account. |
| 6 | Templates. |
| 7 | Etsy listing, with a GIF of the button. |
| 8 | Publish by 1 Dec 2026. |

**Price.** $24 (range $19-29).

**Launch on day one.**
- **Etsy**: "tax client checklist template", "bookkeeper checklist".
- **r/Bookkeeping** bans self-promotion: Rule 1 "No self-promotion", Rule 2 "No commercial spam" (via [mirror](https://redlib.ssps.io/r/Bookkeeping)). Don't post there.
- r/taxpros and ProAdvisor Facebook groups: NOT VERIFIED.

**Biggest risk.** Buyers already use a portal or a $15 checklist. **Cheap test:** about $1/day of ads from 1 Dec to 31 Jan. Kill it with 0 sales by 31 Jan 2027.

---

## Cross-cutting launch notes

- **Run three cheap tests in parallel rather than building ten products.** Each Etsy test costs a $0.20 listing fee (per batch-1) plus $1-3/day in ads. Fourteen days of data beats any score in this report.
- **Etsy hygiene for the Oct 2026 rules:**
  - Disclose AI assistance.
  - Hand-write the instructional text.
  - Make templates and Sheets the product.
  - Keep prompt and skill files on Gumroad.
- **Compliance-adjacent kits (#2, #3, #5, #6, #7):**
  - Use "checklist", "organiser" and "starting point" language.
  - Date-stamp each kit ("current as of Nov 2026").
  - Say "not legal/tax advice".
  - Never promise compliance or approval.
  - Unauthorised-practice-of-law limits on selling legal templates were **not** researched. Check them before scaling #2 and #3.
- **Communities:** almost every relevant subreddit bans direct promotion. The verified pattern is a weekly self-promotion thread (r/therapists, r/smallbusiness) or nothing (r/ecommerce, r/Bookkeeping, r/hvacadvice). Marketplace search is your real day-one channel.

## If I could only build one tomorrow, build this, because...

**Build #1, the Insurance-Ready Progress Note Kit for private-practice therapists.**

1. **Buyers visibly pay for this exact format.** Etsy therapy-note templates show 580-836 reviews at $9-18, even if those counts are partly shop-level. That is the strongest willingness-to-pay evidence among all 30 candidates. Every AI-native idea we tested had none.
2. **The pain is constant, not seasonal, and well evidenced in 2026:** r/therapists threads every few months, NPR in May 2026, and existing $35/month AI-scribe spending.
3. **Distribution doesn't need an audience.** Etsy search brings the buyers. r/therapists gives you a sanctioned weekly self-promotion slot.
4. **It is safe to build in one day:** about 6 hours of Sheets and docs, no APIs, and low legal exposure if you never touch PHI and never say "HIPAA compliant".
5. **The free official Claude plugins can't take this buyer.** A therapist browsing Etsy for a note template isn't installing Cowork plugins. The AI angle is a bonus you sell separately on Gumroad, not the thing that has to work.

It is a crowded category, so the bet is a sharp sub-niche and the 10-day, about-$20 Etsy Ads test. Kill it fast if it gets fewer than 3 sales.

**Runner-up for next week:** #5, the UK MTD landlord workbook. List it now so it has reviews before the Jan-Mar 2027 sign-up rush.
