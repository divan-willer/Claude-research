# Phase 3 validation: Batch 4 (compliance kits: C16-C20)

Validator #4. Date: 2026-11-01. Rubric and anchors are from the shared validator brief. Web searches used: 20 of 20. I also used the GitHub API (free) and the Wix Help Center MCP (free).

## Score table

| id | name | demand | competition (5 = low) | wtp | buildability | distribution | growth | total | verdict |
|---|---|---|---|---|---|---|---|---|---|
| C16 | EU AI Act starter compliance pack (seed 3) | 2 | 1 | 2 | 4 | 3 | 2 | 14 | **REJECT** (fatal: saturated with mass-produced kits plus free templates; softened duty) |
| C17 | Shopify/Wix accessibility self-audit & fix kit (seed 4) | 4 | 3 | 3 | 4 | 3 | 4 | 21 | **VIABLE** (Shopify-only; Wix half absorbed by Wix's free Accessibility Wizard) |
| C18 | A2P 10DLC approval kit | 4 | 2 | 3 | 5 | 3 | 4 | 21 | **VIABLE** (agency-facing version only) |
| C19 | UK DUAA data-protection complaints procedure pack | 2 | 2 | 2 | 5 | 3 | 2 | 16 | **WEAK** (use only as a bundle line item) |
| C20 | CA/NY auto-renewal compliance kit | 1 | 2 | 2 | 5 | 2 | 2 | 14 | **REJECT** (fatal: core mechanics absorbed by billing platforms such as Stripe; zero buyer demand found) |

Bottom line: nothing in this batch reaches STRONG. C17 and C18 are the only two worth building, each with tight scoping and careful claims. C16 and C20 should be dropped. C19 is a £9 add-on at best.

---

## C16. EU AI Act starter compliance pack for small companies [SEED 3]

**Rationale:** This is the most crowded compliance niche I checked. Etsy search shows full kits from $2.95 to $499, including "117 documents" mega-packs, Art. 4 literacy kits and Art. 50 transparency kits. One AI-generated Gumroad catalogue alone has 42 products matching "AI Act". The Digital Omnibus softened Art. 4, no EU-level fine applies to it, and no enforcement was found. The SMB-relevant Art. 50 date (2 Aug 2026) has already passed. There is no buyer pain, just supply chasing a headline.

**Best-scoped version:** none as a standalone product. At most, a 2-page "AI use policy + staff AI-literacy log" as a free lead magnet or a bundle sweetener inside C30-style vertical AI-policy kits.

**Target buyer:** EU SMEs deploying off-the-shelf AI tools. They have no forcing function and a lighter Art. 50 role than providers.

**Demand evidence:**
- One Reddit-mirror anecdote that companies are "sleeping on Article 4" (Phase 1 REG#13: https://reddit.sentinel-team.org/posts/1t3gtml/snapshots/2026-05-07T16%3A03%3A41.170452Z). WEAK.
- No buyer threads were found this session. The visible activity is all seller-side.

**Competition snapshot:**
- Etsy: kits from about $2.95 (audit checklist) to $499. These include a "15 documents… AI Literacy Training… 27-Country Annex" kit, a "117 total documents" pack, a €109 five-template starter kit, Art. 4 PowerPoint/trainer kits and Art. 50 disclosure kits. Several advertise "2026 Digital Omnibus" updates. Sources: https://www.etsy.com/market/compliance_kits, https://www.etsy.com/market/eu_regulations, https://www.etsy.com/shop/ComplianceDocs. No review counts were visible in the results.
- Phase 1 also found Etsy kits at $12.99, $20.76 and $131.27 (https://www.etsy.com/market/ai_policies, https://www.etsy.com/listing/4430787946/2026-ai-compliance-bundle-for-eu-and-us).
- Gumroad: the ghostcorpnet catalogue has 42 items matching "ai act" (my count, from https://raw.githubusercontent.com/koalstingkdelaney-gif/kestrelattice/HEAD/ai/catalog.json). Also https://mininglife1.gumroad.com/l/eu-ai-act-readiness-kit.
- Free:
  - EU AI Office living repository of AI-literacy practices. These are examples, not templates, and the Commission says replicating them does not grant presumption of compliance (https://digital-strategy.ec.europa.eu/en/library/living-repository-foster-learning-and-exchange-ai-literacy).
  - Free templates and gap assessments at https://www.aiactblog.nl/en/templates, https://templates.securityscientist.net/t/eu-ai-act-gap-assessment-template/ and https://vorluxai.pages.dev/templates.
  - AIPIA's AI Pact pledge to publish free SME material, 7 Sep 2026 to 31 Dec 2027 (https://digital-skills-jobs.europa.eu/en/impact-shapers/pledges/aipia-open-ai-literacy-programme-2026-2027).
  - 59 "eu ai act template" GitHub repos (gh api, 1 Nov 2026).

**Kill reasons found:**
1. Hundreds of near-identical, mass-produced kits on Etsy and Gumroad, plus free templates.
2. The duty was softened by the Omnibus, there is no EU fine for Art. 4, and no enforcement was found (Phase 1 REG#13).
3. The next dates are provider-side (2 Dec 2026 machine-readable marking) or far away (high-risk moved to Dec 2027 / Aug 2028).

**Legal-claims risk:** medium. Competitors already use "compliant" and "audit-ready" language. The post-Omnibus legal content goes stale fast, and selling outdated legal templates to 27 jurisdictions is a liability.

**Price recommendation:** do not sell standalone. If bundled, it adds about $0-10 of perceived value.

**Launch channels:**
- Etsy search. Market pages exist, but they are saturated: https://www.etsy.com/market/compliance_kits
- Reddit: no buyer community identified. Rules NOT VERIFIED.

**Biggest risk:** zero sales among a hundred lookalikes. **Cheapest test:** none worth running. Phase 1 GitHub data shows supply plateaued in Q3 2026, and Etsy is flooded.

**Build notes:** trivially buildable (static docs, about 4h). The hard part is legal accuracy after Reg. (EU) 2026/1744. Buildability doesn't matter, because the product can't win.

---

## C17. Shopify/Wix accessibility self-audit & fix kit [SEED 4]

**Rationale:** The pain is real, with merchant-written panic threads on the Shopify Community forum. Lawsuit volume is high and flat: 2,045 ADA web suits in H1 2026, up 1.5% (Phase 1). The Wix half is dead: Wix ships a free Accessibility Wizard (WCAG 2.2-based, scans Stores pages, lists "Manual tasks", updated Oct 2026). The W3C offers a free statement generator. Etsy already has a "Shopify & WooCommerce Accessibility Kit" and an "ADA Compliant Website" bundle. The remaining gap is narrow: a Shopify-theme-specific (Dawn/Horizon) manual-fix workbook plus a "you got a demand letter: first 7 days" organiser that routes the merchant to counsel.

**Best-scoped version:** "Shopify ADA Letter Response & Fix Workbook", for Shopify only. It contains:
- a demand-letter triage checklist (what to preserve, what to send counsel, what not to say)
- a Shopify-admin click-path fix list for the common letter allegations: alt text, icon buttons, form labels, contrast, focus and keyboard traps in the cart drawer
- a dated remediation log in Google Sheets that counsel can attach
- an accessibility statement template

Never use the word "compliant".

**Target buyer:** a US Shopify store owner doing $100k-$2M/yr who has just received, or fears, a demand letter. A secondary buyer is the freelancer or agency asked to "fix it fast".

**Demand evidence:**
- Shopify Community "NEED HELP got a letter from a lawfirm stating my site is not compliance for blind poeple" (https://community.shopify.com/t/need-help-got-a-letter-from-a-lawfirm-stating-my-site-is-not-compliance-for-blind-poeple/575477). Date not shown in the search result.
- Shopify Community "ADA accessibility lawsuits" thread, page 14 or more replies deep (https://community.shopify.com/t/ada-accessibility-lawsuits/351516/14). The results summary says letters cite missing alt text, unlabeled icon buttons and form fields, contrast and keyboard issues, and that "Most are templates". Date not shown.
- "ADA Compliance Lawsuit - Company to Help?" (https://community.shopify.com/t/ada-compliance-lawsuit-company-to-help/230778) and "I have a Shopify Store and I've just been sued under the ADA" (https://community.shopify.com/c/shopify-discussions/i-have-a-shopify-store-and-i-ve-just-been-sued-under-the-ada/td-p/684774). These are older (legacy URL format). They show the problem is persistent.
- "Deep link my accessibility pop up" (https://community.shopify.com/t/deep-link-my-accessibility-pop-up/607500/2), a recent thread ID showing merchants still reach for widgets.
- Volume: EcomBack counted 2,045 ADA web suits in H1 2026 (Phase 1 REG#1: https://www.ecomback.com/ada-website-lawsuits-recap-report/2026-mid-year-ada-website-lawsuit-report). UsableNet says 79% of H1 2026 filings targeted e-commerce (Phase 1, relayed via https://accessibility.build/blog/web-accessibility-lawsuits-2026-midyear-numbers).
- Many 2026 vendor guides target exactly this buyer: https://testparty.ai/blog/ada-demand-letter-shopify-merchant-guide, https://accesscomply.pages.dev/blog/ada-demand-letter-shopify-store, https://www.consentmo.com/blog-posts/us-response-ada-website-lawsuit-surge-shopify-merchants-guide.
- No Reddit r/shopify threads were retrieved; the search returned vendor pages only.

**Competition snapshot:**
- Etsy:
  - "The Creator's Guide to an ADA Compliant Website" bundle (attorney-drafted per the listing, new for 2025, 1 year of updates): https://www.etsy.com/listing/4296587607/the-creators-guide-to-an-ada-compliant
  - a "Shopify & WooCommerce Accessibility Kit" (WCAG 2.2 checklist plus statement generator)
  - a Shopify/WooCommerce keyboard-test audit PDF
  - multiple "Website Accessibility Statement Template" listings

  Prices range from "a few dollars to about $90" (search summary; market page https://www.etsy.com/market/accessibility_audit). No review counts were visible.
- Gumroad: general WCAG material only, nothing Shopify-specific:
  - Uncover Accessibility knowledge base (https://uncover.gumroad.com/l/uncoveraccessibility)
  - Accessibility Made Human (https://mxmdigital.gumroad.com/l/ux-accessibility-guide)
  - a £99 home-page review service (https://chrisyoong.gumroad.com/l/accessibility-review)
  - a statement template (Phase 1: https://mirelaprifti.gumroad.com/l/website-accessibility-statement)
- Adjacent SaaS: overlays at $49-$149/mo (Phase 1, vendor-sourced). The FTC's $1M order against accessiBe undermines them.
- Free alternatives:
  - **Wix Accessibility Wizard**: a free, built-in scan of "Detected issues" plus "Manual tasks" based on WCAG 2.2, which also scans Stores and Blog pages. Updated 5 Oct 2026. Wix itself says it "cannot guarantee that your site will be compliant" (https://support.wix.com/en/article/accessibility-about-the-accessibility-wizard-5119725, https://support.wix.com/en/article/accessibility-using-the-accessibility-wizard). **This absorbs the Wix half of the product.**
  - W3C WAI free accessibility statement generator (https://www.w3.org/WAI/planning/statements/, per the search summary; repo https://github.com/w3c/wai-statements).
  - Shopify's own Checkout accessibility conformance report puts responsibility on the merchant (per the search summary).
  - GitHub: 122 "shopify accessibility" repos, including kgelster/ecom-a11y-audit (12★, Aug 2026; attributes failures to theme vs app) and tanujrajputdev/shopify-theme-audit-skill (44★, a Claude Code skill). Also 85 "accessibility statement" repos created in 2026 (gh api).

**Kill reasons found:**
1. The Wix half is absorbed by the free platform-native wizard.
2. Direct Shopify kits already exist on Etsy.
3. **Legal-claims risk is HIGH.** The FTC's $1M, 20-year order against accessiBe for "makes you compliant" claims (Phase 1: https://technologylaw.fkks.com/post/102jsmj/ftc-finds-website-overlay-tool-failed-to-deliver-accessibility-promises). A demand-letter guide can drift into legal advice. Mitigate by framing it as an organiser that hands off to an attorney, and by making no compliance or lawsuit-protection claims.

None of these is fatal for a Shopify-only, honest version.

**Price recommendation:** $29 on Etsy. $49 for the "letter received" edition with the remediation log and attorney hand-off pack.

**Launch channels:**
- Etsy search: market pages exist for "accessibility audit" and "accessibility checklist" (https://www.etsy.com/market/accessibility_audit, https://www.etsy.com/ie/market/accessibility_checklist). Etsy's AI-disclosure rules apply (Phase 1 REG#9); NOT VERIFIED this session.
- Shopify Community forum: forum rules discourage blatant self-promotion and limit promotional content to designated areas. This was seen via a third-party copy of the Shopify *Developer* Community code of conduct (https://cleverence.com/articles/shopify-dev-documentation/code-of-conduct-shopify-developer-community-6893); the merchant forum rules are NOT VERIFIED. Value-first answers in letter threads are the realistic approach.
- r/shopify: rules NOT VERIFIED.
- r/ecommerce: bans self-promotion "even if free", per a search summary of a mirror snapshot (https://reddit.sentinel-team.org/subreddits/ecommerce/snapshots/2025-12-20T08%3A30%3A17.413923Z).
- r/ecommercemarketing: moved to automatic removal of self-promotion (https://redlib.groet-infra.nl/r/ecommercemarketing/, Feb 2026 snapshot).

**Biggest risk:** panicked merchants buy a lawyer or an app, not a $29 PDF, and calm merchants don't search for it. **Cheapest test:** list the $29 Shopify-only version on Etsy, then answer 5 Shopify Community letter threads with genuinely useful free steps (no link) over 14 days. Kill it if there are fewer than 2 sales or fewer than 20 favourites.

**Build notes:** a static kit: a Docs/PDF workbook, a Google Sheets remediation log and a statement template. About 6h. The click paths need checking in a free Shopify dev store with the Dawn theme, which is doable but tight. Drop Wix entirely.

---

## C18. A2P 10DLC approval kit

**Rationale:** The pain is real and recurring. It shows up in Zoom and Sinch community threads (one user rejected 20+ times), a thriving Fiverr "fix my A2P rejection" gig market, and 174 GitHub repos named for SMS privacy policies created since Twilio's 30 Jun 2026 mandate. The problem is free supply. GoHighLevel's own help article gives the required statements, Hot Prospector's free generator writes six pages plus SMS consent language, and MessageDesk has a free policy checker. A paid Gumroad GHL A2P guide with an "Approval Prep Kit" already exists. A generic kit is a commodity. An agency-facing, multi-vertical pack with a current rejection-code → fix table is the only defensible version.

**Best-scoped version:** "A2P 10DLC Agency Pack (GoHighLevel/Twilio)". It contains:
- 10 vertical campaign-description and sample-message sets (HVAC, dental, salon, real estate, med-spa, gyms…)
- an SMS privacy and terms clause library
- opt-in checkbox copy plus screenshot checklist
- a current Twilio/TCR rejection-code → fix table, including the Mar/Sep 2026 granular codes
- a pre-submission brand-data consistency checklist (legal name, EIN, domain email)
- a client intake form for sub-accounts

Frame it as "no approval guaranteed; not legal advice".

**Target buyer:** a GoHighLevel/white-label agency owner registering 5-50 client sub-accounts who loses days to each rejection. The secondary buyer is the DIY SMB owner on Twilio or GHL.

**Demand evidence:**
- Zoom Community: campaign rejected 20+ times (Phase 1 REG#3: https://community.zoom.com/t5/Zoom-Phone-System/10DLC-Registration-failed-over-and-over/m-p/191089). Also a brand-name mismatch rejection thread (https://community.zoom.com/t5/Zoom-Phone-System/10DLC-SMS-Campaign-Rejected-due-to-Brand-name-not-consistent/m-p/218393).
- Sinch Community "Why was my 10DLC campaign rejected?" (https://community.sinch.com/t5/10DLC/Why-was-my-10DLC-campaign-rejected/m-p/15408). Dates for these threads not shown.
- Fiverr gig supply proves people pay for fixes:
  - https://fiverr.com/workwithahtsham/fix-gohighlevel-twilio-a2p-10dlc-sms-registration
  - https://fiverr.com/midexaa/register-your-a2p-10dlc-brand-and-campaign
  - https://fiverr.com/prada_os/setup-ghl-a2p-10dlc-fix-rejection-and-sms-compliance
  - https://fiverr.com/ayomideisaac643/do-a2p-10dlc-registration-twilio-setup-ghl-automation
  - https://www.fiverr.com/s/ljaRABj
- GitHub (gh api, 1 Nov 2026): 174 repos matching "sms privacy policy" and 80 matching "10dlc" created since 30 Jun 2026. Many are small businesses hosting their SMS policy pages, e.g.:
  - LachmanConsultants/sms-policy (2 Jul 2026, "SMS program privacy policy and terms (A2P 10DLC compliance)")
  - shawnacason/sms-policy (10 Jul 2026)
  - thomaswiedwards-source/sms-policy (20 Jul 2026)
  - jessmohler-del/sms-privacy ("SMS privacy policy for Twilio", 15 Sep 2026)

  The near-identical descriptions suggest people are already DIY-ing this with free AI tools. That is counter-evidence for willingness to pay.
- Twilio added granular rejection codes on 23 Mar 2026, per https://www.ghlscaleup.com/blog/a2p-error-codes-explained, and from 15 Sep 2026, per Phase 1. Telnyx added appeals for rejected campaigns (https://telnyx.com/release-notes/appeal-rejected-10dlc-campaigns-api-portal.md). Twilio error docs include 30971 (business email must use official domain) and 30972 (contact must be an authorised representative): https://live.docs.dev.twilio.com/docs/api/errors/30971.md, https://live.docs.dev.twilio.com/docs/api/errors/30972.md.
- No Reddit threads were retrieved; both Reddit searches returned vendors only.

**Competition snapshot:**
- Gumroad: "The No-Guesswork A2P Setup for GoHighLevel: A Beginner's Guide" includes an "Approval Prep Kit", opt-in language templates and a STOP/DND test pack (https://theapexintelligence.gumroad.com/l/whfrb). Price and ratings were not shown. This is a direct competitor.
- Etsy: one "Twilio A2P 10DLC Registration Helper" listing (https://www.etsy.com/listing/4435251968/twilio-a2p-10dlc-registration-helper-sms). Price and reviews were not shown. GHL template listings only mention A2P in passing (https://www.etsy.com/market/go_high_level_templates_agency). Thin Etsy supply, but also thin Etsy demand.
- Services: the Fiverr gigs above, plus agency setups at $799-$1,500 (Phase 1: https://autogencrm.com/?p=16408).
- Free alternatives:
  - GoHighLevel help article "A2P Opt-In Form - Privacy Policy and Terms and Conditions Guidelines", with required statements and sample pages (last modified 21 Jan 2026): https://help.gohighlevel.com/support/solutions/articles/155000001426-a2p-opt-in-form-privacy-policy-and-terms-and-conditions-guidelines
  - Hot Prospector free funnel generator: six pages plus SMS consent language for GHL forms (https://hotprospector.com/a2p-compliance-guide/funnel-generator)
  - MessageDesk free AI privacy-policy generator and checker (https://www.messagedesk.com/free-tools/privacy-policy-generator)
  - GHL Scale Up free opt-in language templates (https://www.ghlscaleup.com/blog/a2p-opt-in-language-templates)
  - Twilio's error-code docs
  - 49 "a2p 10dlc privacy policy" GitHub repos

**Kill reasons found:**
1. Strong free alternatives cover the policy and opt-in copy.
2. Carriers reject for brand-data reasons (EIN or name mismatch, free email domain, unauthorised contact) that no template fixes.
3. **Legal-claims risk is MEDIUM-HIGH.** TCPA statutory damages attach to consent language. "Guaranteed approval" claims (Phase 1 Fiverr example: https://fiverr.com/ghl_expert_atif/create-gohighlevel-workflows-email-automations-and-crm-triggers) are false by construction. Sell process templates, not outcomes.

Not fatal for the agency version.

**Price recommendation:** $29 single-business edition and $79 agency licence (unlimited client sub-accounts). Undercut Fiverr's per-registration fees, which are visible but not quoted here.

**Launch channels:**
- Gumroad: a direct competitor is present, which shows the channel works for this.
- GoHighLevel Facebook groups and the GHL community: rules NOT VERIFIED.
- r/gohighlevel: rules NOT VERIFIED; the search returned no rules page.
- Etsy: one listing only, so low buyer search traffic is likely. NOT VERIFIED.
- Fiverr: sell a "productised" registration review gig using the kit as the deliverable. Fiverr ToS NOT VERIFIED.

**Biggest risk:** agencies use the free GHL docs plus the Hot Prospector generator and never pay. **Cheapest test:** publish the rejection-code → fix table as a free Gumroad lead magnet, with an upsell to the $79 agency pack. Post it in 2 GHL Facebook groups after checking rules. Kill it if there are fewer than 50 free downloads and 0 upsells in 14 days.

**Build notes:** a static kit: a Docs clause library, Sheets code table, vertical sample-message sets and an intake form. About 6h with Claude Code. Errors must be sourced to Twilio docs pages and date-stamped "current as of Nov 2026". Approval outcomes can't be tested in a day, and none should be claimed.

---

## C19. UK data-protection complaints procedure pack (DUAA)

**Rationale:** The legal duty is real and universal. From 19 Jun 2026, every controller needs a complaints process with 30-day acknowledgement, confirmed by many law firms and the ICO. But no buyer is visibly asking for help: the reddit search returned only law firms and vendors. The ICO publishes a free small-business guide that suggests reusable template letters. Free sample procedures circulate (ComplaintsDesk, public PDFs). There is no standalone offence or penalty for lacking one. The product is a one-page procedure plus two letters, which is hard to sell on its own.

**Best-scoped version:** a £9 "UK DUAA complaints add-on" (procedure, acknowledgement and outcome letters, Sheets log with a 30-day timer, website "how to complain" snippet). Best bundled into a broader UK GDPR small-business pack that Etsy buyers already search for.

**Target buyer:** UK micro-businesses, charities and clubs that buy UK GDPR template packs on Etsy.

**Demand evidence:**
- No buyer threads were found.
- Supply-side and legal: "UK SMEs have three weeks to comply…" (https://www.comparethecloud.net/news/uk-smes-have-three-weeks-to-comply-with-new-data-complaint-rules-under-the-duaa, May/Jun 2026), DLA Piper (https://privacymatters.dlapiper.com/2026/06/uk-new-complaints-handling-rules-under-duaa-take-effect-on-19-june-2026-are-you-ready/, Jun 2026) and RPC (https://www.rpclegal.com/snapshots/data-protection/autumn-2026/new-uk-statutory-data-protection-complaints-regime-now-in-force/, autumn 2026).
- The ICO small-business blog "Five simple ways to make a data protection complaint easier to handle" (https://ico.org.uk/for-organisations/advice-for-small-organisations/news-blogs-and-events/blogs/five-simple-ways-to-make-a-data-protection-complaint-easier-to-handle/) shows the regulator expects SME confusion. This is not buyer demand.

**Competition snapshot:**
- Etsy: complaint-specific listings are "few". Most UK GDPR packs bundle a policy, SAR template and breach log, with complaints as a section. Examples: https://www.etsy.com/listing/4525291416/uk-gdpr-data-protection-policy-template, https://www.etsy.com/listing/1667069653/uk-gdpr-data-protection-policy-template and market page https://www.etsy.com/market/gdpr_template_uk. No prices or reviews were visible.
- Free alternatives:
  - ICO "How to deal with data protection complaints you receive as a small business" (https://ico.org.uk/for-organisations/sme-web-hub/how-to-deal-with-data-protection-complaints-you-receive-as-a-small-business)
  - ComplaintsDesk free template (https://complaintsdesk.pages.dev/duaa-complaints-procedure)
  - Business Wales guidance (https://businesswales.gov.wales/news-and-blog/dealing-data-protection-complaints-a-small-business)
  - A public sample procedure PDF (https://www.everywhen.co.uk/media/3uqbeyhh/data-protection-complaints-procedure.pdf)
  - iubenda and Sprintlaw guides (Phase 1)

**Kill reasons found:**
1. Free ICO guidance plus free templates cover most of the job.
2. The deadline has passed and there is no standalone penalty (per the search summary of law-firm sources), so there is no urgency.
3. No buyer demand was found.

**Legal-claims risk:** LOW. It's a procedural document, mirrors ICO guidance, and carries a "not legal advice" disclaimer.

**Price recommendation:** £7-£12 standalone, or included in a £19-£29 UK GDPR small-business bundle.

**Launch channels:**
- Etsy UK: a market page for "gdpr template uk" exists (https://www.etsy.com/market/gdpr_template_uk), so buyers search there. Ranking NOT VERIFIED.
- r/UKPersonalFinance and r/smallbusinessuk: rules NOT VERIFIED.

**Biggest risk:** nobody searches for "complaints procedure" specifically. **Cheapest test:** a £9 Etsy UK listing with "DUAA 2025 complaints procedure" in the title. Kill it after 30 days with 0 sales.

**Build notes:** about 2-3h. Docs, a Sheets log with a 30-day due-date formula and an HTML snippet. Trivial to build.

---

## C20. Auto-renewal compliance kit for small subscription sellers (CA/NY)

**Rationale:** No buyer demand surfaced: every result was a 2025 law-firm alert. The regulated mechanics are already built into the billing platforms. Stripe's own FAQ ("FTC & California subscription law changes require billing updates") documents renewal-reminder emails, "Manage Subscription" links and "a near one-click cancellation process". Creators on merchant-of-record platforms (Gumroad, Lemon Squeezy) don't control their checkout or cancel flow at all; this is my inference and was not verified per platform. A free educational ARL scanner already exists on GitHub. The disclosure-copy remainder is a few paragraphs.

**Best-scoped version:** none standalone. At most, a "subscription terms + renewal-reminder email" page inside a creator legal bundle.

**Target buyer:** creators and small membership or SaaS sellers on Stripe, Kajabi or Skool. They are not observed asking for this.

**Demand evidence:**
- None from buyers. The search for Kajabi/Skool/Stripe creators returned only law firms (e.g. https://www.cooley.com/news/insight/2025/2025-06-04-california-automatic-renewal-law-amendments-take-effect-on-july-1-2025, https://www.kelleydrye.com/viewpoints/blogs/ad-law-access/california-ag-issues-alert-on-californias-automatic-renewal-law.md).
- Phase 1 REG#8 shows the FTC restarted rulemaking (ANPRM, Jan 2026) and CA litigation is rising (https://www.mondaq.com/unitedstates/consumer-law/1769282/that-free-trial-might-cost-you-automatic-renewal-litigation-on-the-rise-in-ca). Defendants are larger companies, not creators.

**Competition snapshot:**
- Etsy: subscription agreement templates, one advertising "State-ARL-aware" cancel-by-date and price-notice terms (https://www.etsy.com/market/subscription_contract, https://www.etsy.com/listing/4493950129/subscription-service-agreement-doc-pdf). No prices or reviews were visible.
- Free and platform-native:
  - Stripe Billing renewal reminders, subscription-management links and one-click cancellation (https://support.stripe.com/questions/faq-ftc-california-subscription-law-changes-require-billing-updates, https://docs.stripe.com/billing/revenue-recovery/customer-emails?locale=en-US)
  - GitHub GerardoRdz96/reclause, "a free, educational scanner for US subscription auto-renewal (ARL / negative-option) laws" (Jun 2026)
  - checkbox-site/auto-renewal-laws (created 1 Nov 2026)

**Kill reasons found:**
1. **Fatal:** core mechanics (cancellation, reminders, management links) are absorbed by billing platforms. Stripe explicitly markets them for the CA/FTC rules.
2. No buyer demand evidence.
3. No dated forcing function: the CA and NY laws are already in force, and the FTC rule is only at the ANPRM stage.
4. **Legal-claims risk is MEDIUM.** ARL class actions are statutory, so wrong disclosure copy could hurt a buyer.

**Price recommendation:** do not sell. If bundled, $0-$10 of perceived value.

**Launch channels:** no clear channel. Creators don't browse Etsy or Gumroad for compliance. Indie Hackers or creator subreddits: rules NOT VERIFIED.

**Biggest risk:** zero demand. **Cheapest test:** not worth one.

**Build notes:** about 3h of static docs. Easy, but pointless given the above.

---

## Method & limitations

- **Searches:** 20 WebSearch calls (the full allowance).
  - Etsy, domain-restricted: EU AI Act, accessibility, 10DLC ×2, UK GDPR complaints, auto-renewal.
  - Gumroad: 10DLC, Shopify accessibility.
  - Shopify Community: ADA letters.
  - Plain queries: Reddit demand ×4, Reddit rules, ICO templates, GHL free generators, W3C generator, AI Office repository, Stripe ARL features.
- **Other free sources:** GitHub repo counts and listings via `gh api search/repositories` on 1 Nov 2026; the ghostcorpnet Gumroad catalogue JSON (keyword counts); the Wix Help Center via the Wix MCP (Accessibility Wizard articles, updated Oct 2026). The Gumroad demand CSV from Phase 1 had no rows for these niches.
- **Gaps:**
  - WebFetch was not used (blocked), so Etsy and Gumroad **prices, review counts and sales were mostly NOT visible**. Most Etsy evidence comes from search-tool summaries of listing and market pages, and individual listing prices weren't tied to URLs. The wtp scores are capped at 3 for this reason.
  - No Reddit threads were retrieved for any candidate. Reddit-based demand evidence is absent, and every subreddit self-promotion rule except r/ecommerce and r/ecommercemarketing (mirror summaries) is NOT VERIFIED.
  - Shopify Community thread dates were not shown in results. Some threads are old (legacy URLs).
  - Statements about merchant-of-record platforms controlling checkout (C20) and about Etsy's AI-disclosure rules are inferences or relayed from Phase 1, not verified here.
  - I did not research unauthorised-practice-of-law limits for selling legal templates (same gap as Phase 1).

## Sources

Etsy:
- https://www.etsy.com/market/compliance_kits
- https://www.etsy.com/market/eu_regulations
- https://www.etsy.com/shop/ComplianceDocs
- https://www.etsy.com/market/ai_policies (Phase 1)
- https://www.etsy.com/listing/4430787946/2026-ai-compliance-bundle-for-eu-and-us (Phase 1)
- https://www.etsy.com/listing/4296587607/the-creators-guide-to-an-ada-compliant
- https://www.etsy.com/market/accessibility_audit
- https://www.etsy.com/ie/market/accessibility_checklist
- https://www.etsy.com/listing/4435251968/twilio-a2p-10dlc-registration-helper-sms
- https://www.etsy.com/market/go_high_level_templates_agency
- https://www.etsy.com/market/gdpr_template_uk
- https://www.etsy.com/listing/4525291416/uk-gdpr-data-protection-policy-template
- https://www.etsy.com/listing/1667069653/uk-gdpr-data-protection-policy-template
- https://www.etsy.com/market/subscription_contract
- https://www.etsy.com/listing/4493950129/subscription-service-agreement-doc-pdf

Gumroad:
- https://theapexintelligence.gumroad.com/l/whfrb
- https://uncover.gumroad.com/l/uncoveraccessibility
- https://mxmdigital.gumroad.com/l/ux-accessibility-guide
- https://chrisyoong.gumroad.com/l/accessibility-review
- https://mininglife1.gumroad.com/l/eu-ai-act-readiness-kit (Phase 1)
- https://raw.githubusercontent.com/koalstingkdelaney-gif/kestrelattice/HEAD/ai/catalog.json

Shopify Community:
- https://community.shopify.com/t/need-help-got-a-letter-from-a-lawfirm-stating-my-site-is-not-compliance-for-blind-poeple/575477
- https://community.shopify.com/t/ada-accessibility-lawsuits/351516/14
- https://community.shopify.com/t/ada-compliance-lawsuit-company-to-help/230778
- https://community.shopify.com/c/shopify-discussions/i-have-a-shopify-store-and-i-ve-just-been-sued-under-the-ada/td-p/684774
- https://community.shopify.com/t/deep-link-my-accessibility-pop-up/607500/2

Wix and W3C:
- https://support.wix.com/en/article/accessibility-about-the-accessibility-wizard-5119725
- https://support.wix.com/en/article/accessibility-using-the-accessibility-wizard
- https://www.w3.org/WAI/news/2018-11-29/develop-accessibility-statement/
- https://github.com/w3c/wai-statements

A2P 10DLC:
- https://help.gohighlevel.com/support/solutions/articles/155000001426-a2p-opt-in-form-privacy-policy-and-terms-and-conditions-guidelines
- https://hotprospector.com/a2p-compliance-guide/funnel-generator
- https://www.messagedesk.com/free-tools/privacy-policy-generator
- https://www.ghlscaleup.com/blog/a2p-opt-in-language-templates
- https://www.ghlscaleup.com/blog/a2p-error-codes-explained
- https://telnyx.com/release-notes/appeal-rejected-10dlc-campaigns-api-portal.md
- https://live.docs.dev.twilio.com/docs/api/errors/30971.md
- https://live.docs.dev.twilio.com/docs/api/errors/30972.md
- Fiverr gigs (listed under C18)
- Zoom and Sinch community threads (Phase 1)

UK DUAA:
- https://ico.org.uk/for-organisations/sme-web-hub/how-to-deal-with-data-protection-complaints-you-receive-as-a-small-business
- https://ico.org.uk/for-organisations/advice-for-small-organisations/news-blogs-and-events/blogs/five-simple-ways-to-make-a-data-protection-complaint-easier-to-handle/
- https://complaintsdesk.pages.dev/duaa-complaints-procedure
- https://businesswales.gov.wales/news-and-blog/dealing-data-protection-complaints-a-small-business
- https://www.everywhen.co.uk/media/3uqbeyhh/data-protection-complaints-procedure.pdf
- https://www.comparethecloud.net/news/uk-smes-have-three-weeks-to-comply-with-new-data-complaint-rules-under-the-duaa
- https://privacymatters.dlapiper.com/2026/06/uk-new-complaints-handling-rules-under-duaa-take-effect-on-19-june-2026-are-you-ready/
- https://www.rpclegal.com/snapshots/data-protection/autumn-2026/new-uk-statutory-data-protection-complaints-regime-now-in-force/

EU AI Act:
- https://digital-strategy.ec.europa.eu/en/library/living-repository-foster-learning-and-exchange-ai-literacy
- https://www.aiactblog.nl/en/templates
- https://templates.securityscientist.net/t/eu-ai-act-gap-assessment-template/
- https://digital-skills-jobs.europa.eu/en/impact-shapers/pledges/aipia-open-ai-literacy-programme-2026-2027

Auto-renewal:
- https://support.stripe.com/questions/faq-ftc-california-subscription-law-changes-require-billing-updates
- https://docs.stripe.com/billing/revenue-recovery/customer-emails?locale=en-US
- https://www.cooley.com/news/insight/2025/2025-06-04-california-automatic-renewal-law-amendments-take-effect-on-july-1-2025

Reddit rules (mirrors):
- https://reddit.sentinel-team.org/subreddits/ecommerce/snapshots/2025-12-20T08%3A30%3A17.413923Z
- https://redlib.groet-infra.nl/r/ecommercemarketing/

Phase 1 citations: `research/phase1/regulation-and-platform-shifts.md` (sections #1, #3, #7, #8, #13 and the risk notes), `marketplace-saturation-scout.md` (#44, #46), `trend-scout.md` (#4, #6, #20).
