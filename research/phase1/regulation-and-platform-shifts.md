# Regulation and platform shifts that force small buyers to act (status as of 1 Nov 2026)

Phase 1 research, role: regulation-and-platform-shifts. Prepared for the solo-founder "10 one-day digital products" project.

## Executive summary

- **Many headline AI-regulation deadlines have been delayed, softened or repealed.** The EU Digital Omnibus on AI (Reg. (EU) 2026/1744, in force 27 Jul 2026) pushed high-risk duties to Dec 2027 / Aug 2028 and rewrote Art. 4 AI literacy into a softer "take measures to support" duty with no EU-level fine. Colorado's AI Act was repealed and replaced before it ever applied, and enforcement is stayed. The FCC AI-caller disclosure rule is parked as a "Long-Term Action". The DOJ (ADA Title II) and HHS (Section 504) web-accessibility deadlines slipped a year, to 2027/2028. **Seed hypothesis 3 (EU AI Act starter packs) looks weak:** the duty is softer than marketed, no enforcement was found, the space is crowded (Etsy kits from $12.99, about 1,100 GitHub repos created in 2026) and free templates are plentiful.
- **The strongest forcing functions for small, non-technical buyers are not "AI laws".** They are: (1) US ADA website lawsuits against e-commerce (about 2,045 suits in H1 2026; 79% e-commerce per UsableNet), plus early EAA enforcement in France, Sweden, the Netherlands and Germany; (2) UK Making Tax Digital for Income Tax (live since Apr 2026 for over £50k; about 1 million more sole traders and landlords from Apr 2027 at over £30k); (3) A2P 10DLC SMS registration rejections (Twilio made privacy-policy and terms URLs mandatory from 30 Jun 2026); and (4) AI-search and Google Maps changes (Ask Maps replaced GBP Q&A; AI Overviews cut CTR about 58% per Ahrefs) pushing local businesses to optimise reviews and profiles. The FTC Consumer Review Rule (first lawsuit May 2026) limits how they can chase reviews.
- **Voice-agent and chatbot compliance is real but fragmented.** Outbound AI calls need TCPA consent (FCC 2024 ruling). State AI-disclosure rules apply (CA AB 2905, Utah on-ask, Maine). About a dozen all-party recording-consent states and CIPA wiretap suits against AI call-centre tools add risk. This supports a "compliance script pack" add-on to seed hypothesis 6, not a standalone legal product.
- **Other affected groups for cheap templates (all-business scope, weaker willingness to pay):** UK data-protection complaints procedures (mandatory for all UK controllers since 19 Jun 2026); CA/NY auto-renewal rules; Etsy AI-disclosure and "Designed by" rules for digital sellers; the TAKE IT DOWN Act notice-and-removal process for small UGC sites (enforced since 19 May 2026).
- **Weak or reject:** school/tutoring AI policies (mandates hit districts, which have free model policies; no tutoring-centre mandate found); US state privacy laws (thresholds exclude most micro businesses); CCPA ADMT, NIS2, HIPAA Security Rule overhaul (still proposed) and PCI SAQ A (larger or technical buyers); llms.txt (log studies show AI crawlers barely request it; no citation correlation).
- **Liability warning for compliance products:** the FTC's $1M order against accessiBe (2025) for unsupported accessibility-compliance claims is a direct precedent. Any kit must avoid "makes you compliant / lawsuit-proof / guaranteed approval" claims. It needs "not legal or tax advice" disclaimers and should be framed as checklists and templates, not outcomes.

## Ranked summary table

Ranking = (number of affected small buyers) x (urgency now) x (fit for a $10-100 one-day digital product). H = high, M = medium, L = low. Evidence labels as defined in the brief.

| Rank | Shift / rule | Verified status (Nov 2026) | Affected small buyers | Urgency | One-day product fit | Evidence | Verdict |
|---|---|---|---|---|---|---|---|
| 1 | US ADA web-accessibility lawsuits vs e-commerce (+ EU EAA) | Lawsuits flat-to-rising; EAA in force since 28 Jun 2025 with early enforcement, no published fines | US Shopify/Wix/Squarespace stores; EU non-micro shops | H | M-H (self-audit + statement + demand-letter first-steps kit) | STRONG (trackers; vendor-sourced) | Pursue, with strict no-compliance-guarantee framing; crowded with apps and overlays |
| 2 | UK Making Tax Digital for Income Tax | Live 6 Apr 2026 (over £50k); £30k from Apr 2027; £20k from Apr 2028 | ~780k now, ~970k-1.08M more in Apr 2027 | H (next wave in 5 months) | H (Sheets records template + bridging-software guide; Etsy already sells these) | STRONG | Pursue; must not claim to be HMRC-recognised software |
| 3 | A2P 10DLC / TCPA SMS rules | Twilio privacy-policy and terms URLs mandatory for new campaigns from 30 Jun 2026; TCPA "revoke-all" delayed to 31 Jan 2027, with new FCC changes pending | US SMBs texting customers; GoHighLevel/Twilio agencies | H (blocking rejections) | H (approval kit: policy clauses, opt-in copy, campaign descriptions, rejection-code fix table) | MEDIUM | Pursue; cannot promise approval |
| 4 | AI-search / Google AI Overviews / AI Mode / Ask Maps shift | Ongoing platform shift; AI Mode over 1B monthly users (I/O 2026) | All local SMBs | M | H (GBP + reviews + schema kit; drop llms.txt as a selling point) | STRONG on traffic shift; WEAK on WTP | Pursue (seed hyp. 2), re-scoped |
| 5 | FTC Consumer Review & Testimonials Rule | In force since Oct 2024; warning letters Dec 2025; first DOJ/FTC suit May 2026 | Local service businesses chasing reviews | M | H (compliant review-request templates, bundle with #4) | MEDIUM-STRONG | Bundle with #4 |
| 6 | AI voice-agent disclosure / call-recording consent | FCC AI-voice = "artificial voice" (2024); AI-disclosure NPRM stalled; CA AB 2905, Utah, Maine; CIPA suits | Trades, clinics, agencies deploying AI receptionists | M | H as add-on (state-by-state opening scripts, consent flows, BAA checklist) | MEDIUM | Bundle with seed hyp. 6 |
| 7 | UK DUAA data-protection complaints procedure | Mandatory since 19 Jun 2026, no size exemption | Every UK business processing personal data | M (low awareness) | H (procedure + letters + log) | MEDIUM-STRONG | Viable cheap Etsy/Gumroad template; unproven WTP |
| 8 | CA/NY auto-renewal laws (federal click-to-cancel vacated) | CA amendments 1 Jul 2025; NY amendments 5 Nov 2025; FTC restarted rulemaking (ANPRM 2026) | Small subscription/membership sellers | M | M (checklist + cancellation-flow copy) | MEDIUM | Niche option |
| 9 | Etsy AI-disclosure / Creativity Standards for digital downloads | Digital downloads in Creativity Standards (Jun 2025); "Designed by" enforcement reported from 14 Jan 2026 | Etsy digital sellers (incl. this founder) | M | M (seller checklist) | WEAK-MEDIUM (blogs) | Mainly a risk to manage for the founder's own listings |
| 10 | TAKE IT DOWN Act platform duties | FTC enforcing since 19 May 2026; 48-hour removal | Small forums/communities hosting UGC | M | M (policy + request form + SOP) | MEDIUM | Niche option |
| 11 | HHS Sec. 504 / ADA Title II web rules | Delayed to May 2027 / Apr 2027 (large) and 2028 (small); lawsuit vs delay | Clinics with HHS funding; local governments | L now, M in 2027 | M | STRONG | Revisit in 2027 |
| 12 | EU e-invoicing (FR Sep 2026 receive / Sep 2027 issue; PL KSeF; BE Peppol; DE 2027/28) | Live in BE, PL; FR reception live since 1 Sep 2026 | Millions of EU micro firms | M-H | L-M (buyers need software; local-language guides) | STRONG | Low fit for this founder |
| 13 | EU AI Act Art. 4 literacy + Art. 50 transparency | Art. 4 softened (no EU fine); Art. 50 applies from 2 Aug 2026 (watermark grandfathering to 2 Dec 2026) | EU SMEs using AI | L | M | STRONG (status) | Reject seed hyp. 3 as a standalone |
| 14 | US state AI laws (CO, TX, IL, CA companion bots) | CO repealed/replaced, eff. 1 Jan 2027 and stayed; TX TRAIGA narrow; IL notice law live | Few small buyers | L | L-M | MEDIUM | Reject (except a possible IL hiring-notice template) |
| 15 | School AI policy mandates (OH, TN, ID, MD, OK, VA; UK KCSIE 2026) | OH deadline passed 1 Jul 2026; free model policies | Districts (procurement), not tutoring centres | L | L | MEDIUM | Reject seed hyp. 9 for schools; no tutoring mandate found |
| 16 | Gmail/Yahoo/Microsoft bulk-sender rules | Gmail permanent rejections since Nov 2025; Microsoft since 5 May 2025 | Only senders of 5k+/day to consumer inboxes | L-M | M | STRONG | Low; free generators everywhere |
| 17 | Others checked: CCPA ADMT, NIS2, CRA reporting, PCI SAQ A, HIPAA SR, COPPA 2025 rule, state privacy laws, Consent Mode v2, EU Pay Transparency, Australia ADM, GPSR, 1099 thresholds, Chrome MV2, ChatGPT Instant Checkout | See detail | Mostly larger, technical, or relief-only | L | L | Mixed | Drop or niche |

---

## Detailed entries (ranked)

### 1. US ADA website lawsuits vs e-commerce, plus the European Accessibility Act (EAA)

**What changed:** No new US federal rule applies to private businesses. The change is litigation volume and its concentration on e-commerce. The EAA has applied to e-commerce and other services since 28 Jun 2025, and 2026 is its first real enforcement year.

**Evidence (US):**
- EcomBack counted 2,045 ADA website lawsuits in H1 2026, up 1.54% on H1 2025's 2,014 ([EcomBack mid-year report](https://www.ecomback.com/ada-website-lawsuits-recap-report/2026-mid-year-ada-website-lawsuit-report)). A secondary source citing EcomBack says 46.55% (952) of H1 2026 cases hit Shopify stores. This was not confirmed in EcomBack's own report, so it is **unverified** ([halfaccessible](https://halfaccessible.com/ada-website-lawsuit-statistics-2026/)).
- UsableNet's 2026 midyear report projects about 6,176 federal and state website/app suits for 2026. It says 79% of H1 2026 filings targeted e-commerce, up from 70% in 2025 (per search summary of [accessibility.build midyear](https://accessibility.build/blog/web-accessibility-lawsuits-2026-midyear-numbers) / [testpros](https://testpros.com/accessibility/web-accessibility-lawsuit-statistics/)).
- Seyfarth counted 5,006 federal ADA Title III filings in H1 2026 (all Title III, not just web) ([adatitleiii.com](https://www.adatitleiii.com/)).
- EcomBack reports 496 suits (24.25%) were filed against sites that already had an accessibility widget installed ([EcomBack](https://www.ecomback.com/ada-website-lawsuits-recap-report/2026-mid-year-ada-website-lawsuit-report)). This is counter-evidence that overlays protect anyone.
- Settlement ranges quoted by vendors run $5k-$75k, and response windows are about 30 days ([testparty demand-letter guide](https://testparty.ai/blog/ada-demand-letter-shopify-merchant-guide), [accesscomply](https://accesscomply.pages.dev/blog/ada-demand-letter-shopify-store)). These are vendor sources, so **WEAK**.

**Evidence (EU EAA, enforcement reality):**
- A tracker dated 19 Oct 2026 says no regulator in 14 countries has published a fine. Poland told Parliament in Aug 2026 that no fines had been imposed ([complyloft tracker](https://www.complyloft.com/accessibility/eaa/enforcement), [statutus](https://statutus.ch/en/guides/european-accessibility-act-enforcement-so-far/), [libration.io](https://libration.io/en/resources/eaa-fines-enforcement/)).
- **France:** a Caen court on 4 Jun 2026 ordered Carrefour to make its site and app accessible within six months, with daily penalties. It rejected the argument that 71% compliance was enough. The DGCCRF has examined about 50 e-commerce businesses and received almost 700 complaints by Jun 2026 ([li.solutions](https://li.solutions/blog/eaa-enforcement-2026/), [atyantik](https://atyantik.com/blog/european-accessibility-act-enforcement/)).
- **Sweden:** PTS had 28 e-commerce supervision cases by Mar 2026. **Netherlands:** ACM sent information requests, including to non-EU firms ([atyantik](https://atyantik.com/blog/european-accessibility-act-enforcement/), [statutus](https://statutus.ch/en/guides/european-accessibility-act-enforcement-so-far/)).
- **Germany:** the first BFSG Abmahnungen (competitor warning letters) arrived about six weeks after the law took effect ([Heuking, Aug 2025](https://www.heuking.de/de/news-events/newsletter-fachbeitraege/artikel/das-barrierefreiheitsstaerkungsgesetz-bfsg-teil-2-die-ersten-bfsg-abmahnungen-im-e-commerce.html)). Vendors claim a "second wave" in 2026 but give no verifiable data ([pragma-code](https://www.pragma-code.de/blog-abmahnwelle-barrierefreiheit-2026), [xictron](https://www.xictron.com/de/blog/bfsg-abmahnwelle-2026-barrierefreiheit-durchsetzen/)). Händlerbund offers a free BFSG check to members ([haendlerbund](https://www.haendlerbund.de/de/news/aktuelles/gratis-bfsg-check)).
- **Microenterprise exemption (counter-evidence for EU small buyers):** EAA service obligations exempt microenterprises (under 10 staff; the €2M turnover limit comes from the EU micro definition and was not confirmed by these results). The exemption covers the shop as a service, not certain products sold ([xictron](https://www.xictron.com/en/blog/accessibility-act-exemptions-microenterprises-2026/), [dev.to/lawebe](https://dev.to/lawebe/the-european-accessibility-act-eaa-what-online-stores-must-do-1eh5)). Vendors claiming "most Shopify merchants won't qualify" ([fudge.ai](https://www.fudge.ai/blog/european-accessibility-act-shopify/)) have a sales interest. Many tiny shops likely do qualify, which shrinks the EU small-buyer pool.

**What buyers would buy:** a self-audit checklist for their platform/theme (alt text, contrast, keyboard, forms, PDFs/emails), an accessibility statement template (EU statement / US "commitment" page), a remediation log, and a "received a demand letter" first-steps checklist that points to counsel.

**Existing paid offerings and prices:**
- Overlays: accessiBe quoted at $490-$950/yr or $59/mo; UserWay at $49-$149/mo ([testparty](https://testparty.ai/blog/is-accessibe-worth-it), [alttext.ai](https://alttext.ai/vs/accessibe)), vendor-sourced.
- A Gumroad accessibility-statement template exists (price not shown) ([mirelaprifti.gumroad.com](https://mirelaprifti.gumroad.com/l/website-accessibility-statement)).
- Free statement generators: [iubenda](https://www.iubenda.com/en/blog/european-accessibility-act-eaa-accessibility-statement-guide-template-2/), [getwcag](https://getwcag.com/en/accessibility-statement), and npm packages `eaa-kit`, `@ariada-org/statement-generator`, `curbcut` (npm registry search). A free Claude skill for WCAG audits also exists on GitHub ([creativedeals/free-claude-skill-accessibility-audit](https://github.com/creativedeals/free-claude-skill-accessibility-audit)).

**Liability risk (high):** the FTC finalised a $1M, 20-year order against accessiBe in 2025 for unsupported claims that its tool made sites compliant ([fkks](https://technologylaw.fkks.com/post/102jsmj/ftc-finds-website-overlay-tool-failed-to-deliver-accessibility-promises), [grandriversolutions](https://grandriversolutions.com/ftc-1-million-dollar-settlement-case/)). A class action was also filed against UserWay by a customer who was sued anyway ([search summary, testparty](https://testparty.ai/blog/are-accessibility-overlays-legal)).

**Verdict:** best fit for seed hypothesis 4. Large, anxious, non-technical buyer base, and buyers gather in r/shopify and Shopify community forums (no Reddit threads were retrieved; channel presence is an assumption to verify). A one-day product works as a manual-fix checklist plus statement plus remediation tracker, explicitly not a guarantee. Competition from apps is heavy, so differentiate on "honest, no-overlay, platform-specific steps". **Evidence: STRONG** (multiple trackers, though most are vendors). Dates: 2026.

---

### 2. UK Making Tax Digital for Income Tax Self Assessment (MTD ITSA)

**What changed:** from 6 Apr 2026, sole traders and landlords with qualifying gross income over £50k must keep digital records and send quarterly updates via compatible software. The threshold drops to £30k from Apr 2027 and £20k from Apr 2028 ([GOV.UK software guidance](https://www.gov.uk/guidance/choose-the-right-software-for-making-tax-digital-for-income-tax?), [GOV.UK policy paper](https://www.gov.uk/government/publications/extension-of-making-tax-digital-for-income-tax-self-assessment-to-sole-traders-and-landlords/making-tax-digital-for-income-tax-self-assessment-for-sole-traders-and-landlords), [ICAS](https://www.icas.com/news-insights-events/news/tax/further-updates-to-making-tax-digital-for-income-tax-self-assessment-announced)).

**Who and how many:**
- About 780,000 were required in the first wave, and fewer than 3 in 10 had registered by April ([The Register, 10 Apr 2026](https://www.theregister.com/2026/04/10/mtd_hmrc/), [pulse.bot](https://www.pulse.bot/finance/news/fewer-than-3-in-10-register-for-hmrcs-making-tax-digital-shake-up-b534009f-ba1a-45e1-b494-31174b5ace84/)).
- About 436,000 had filed a first quarterly update by Aug 2026 ([sterlingandwells](https://sterlingandwells.com/news/sole-traders-landlords-filed-under-mtd/)), a single blog, unverified against HMRC.
- Estimates for the Apr 2027 wave are about 970,000 ([The Register](https://www.theregister.com/2026/04/10/mtd_hmrc/)) or about 1,077,000 ([MoneyWeek](https://moneyweek.com/economy/small-business/what-you-need-to-know-about-making-tax-digital)). About 975,000 more are expected in Apr 2028 ([MoneyWeek](https://moneyweek.com/economy/small-business/what-you-need-to-know-about-making-tax-digital)).

**Penalties:** sources conflict. Some report a first-year soft landing on penalty points for late quarterly updates, others say non-sign-up is treated as non-compliance ([ICAS](https://www.icas.com/news-insights-events/news/tax/further-updates-to-making-tax-digital-for-income-tax-self-assessment-announced), [payslipchecker](https://www.payslipchecker.uk/blog/making-tax-digital-self-employed-guide)).

**What buyers would buy:** spreadsheets are allowed as the record-keeper if paired with bridging software ([getcoconut](https://www.getcoconut.com/knowledge-hub/bridging-software-for-online-marketplaces-and-mtd), [zmartly](https://zmartly.co.uk/news-insights/mtd-software-for-landlords-bridging-software)). That creates demand for a well-structured Google Sheets/Excel income-and-expense template mapped to HMRC categories, plus a "which bridging tool, how to sign up, quarterly calendar" guide. Separate editions for landlords and sole traders are possible.

**Existing paid offerings:**
- Etsy already lists MTD 2026/27 spreadsheets; one landlord version is at AU$30.30 on sale ([Etsy listing](https://www.etsy.com/listing/4567179604/), [Etsy listing](https://www.etsy.com/listing/4567155739/), [Etsy listing](https://www.etsy.com/listing/4567156121/)).
- Payhip listings exist ([payhip](https://payhip.com/b/9ZbAV)).
- Bridging tools: 123 Sheets ([123sheets](https://123sheets.com/landlords.aspx)), Abridge for Google Sheets ([Workspace Marketplace](https://workspace.google.com/marketplace/app/abridge/251470994062)) and the MTD Companion app ([App Store](https://apps.apple.com/gb/app/id6752574003)).
- NRLA offers a free bridging template to members ([NRLA](https://www.nrla.org.uk/services/tax/taxd/bridging-template)).

**Counter-evidence:** HMRC-recognised software vendors (and free tiers) compete. Etsy supply already exists, so the niche is not empty. It is growing, though, with a hard April 2027 deadline and about 1M new entrants.

**Liability:** tax content. Use "not tax advice" and do not claim HMRC recognition (the template is not software that submits). **Evidence: STRONG.** Dates: Apr 2026-Apr 2028.

**Verdict:** one of the best fits in this remit. It is a Sheets template plus guide, sold where UK buyers search (Etsy UK, landlord forums such as Property118 and the NRLA community; [property118](https://www.property118.com/landlords-urged-to-prepare-for-making-tax-digital-2027/)).

---

### 3. A2P 10DLC SMS registration and TCPA consent rules (US)

**What changed:**
- Twilio requires both a privacy-policy URL and a terms URL for new 10DLC campaign registrations from 30 Jun 2026, and rejects campaigns missing them ([Twilio changelog, 6 Apr 2026](https://www.twilio.com/en-us/changelog/a2p-10dlc-campaign-registration-will-require-privacy-policy-and-)). Error 30933 makes `PrivacyPolicyUrl` mandatory via the API from that date ([Twilio error 30933](https://www.twilio.com/docs/api/errors/30933)).
- Other common rejection codes: 30908 (policy doesn't explain mobile data use), 30932 (policy suggests sharing opt-in data with third parties) and 30920 (website is just a landing page) ([30908](https://live.docs.dev.twilio.com/docs/api/errors/30908.md), [30932](https://static0.twilio.com/docs/api/errors/30932), [30920](https://static1.twilio.com/docs/api/errors/30920)). Twilio adds new rejection error codes from 15 Sep 2026 ([Twilio changelog](https://static1.twilio.com/en-us/changelog/new-error-codes-provide-clearer-tfv-and-a2p-10dlc-registration-f)).
- Toll-free verification requires a Business Registration Number for new registrations from 1 Jan 2026 (per search summary of [conduit.ai](https://conduit.ai/blog/a2p-10dlc-registration-step-by-step-for-2026)).
- TCPA: the FCC delayed the "revoke-all" consent rule to 31 Jan 2027 ([Burr & Forman](https://www.burr.com/telephone-consumer-protection-act/the-fcc-delays-effective-date-of-tcpa-revoke-all-rule-until-january-31-2027), [Mac Murray & Shuster](https://mslawgroup.com/delayed-again-fcc-pushes-back-tcpas-revoke-all-rule-to-january-31-2027/)). A further order revising the revocation rules (7-day honour window, two-way texting) was scheduled for an FCC vote on 30 Sep 2026. Adoption was **not confirmed** ([Cullen and Dykman](https://www.cullenllp.com/blog/fcc-substantially-revises-tcpa-consent-revocation-rules-set-to-take-effect-january-2027/), [Troutman](https://www.troutman.com/insights/fcc-revises-tcpa-revocation-of-consent-rules-that-were-set-to-go-into-effect-in-january/)).

**Pain evidence:**
- A Zoom Community user reports their 10DLC campaign was rejected 20+ times since March ([community.zoom.com](https://community.zoom.com/t5/Zoom-Phone-System/10DLC-Registration-failed-over-and-over/m-p/191089)). Another thread covers rejection over brand-name inconsistency ([community.zoom.com](https://community.zoom.com/t5/Zoom-Phone-System/10DLC-SMS-Campaign-Rejected-due-to-Brand-name-not-consistent/m-p/218393)), and a Sinch community thread asks why a campaign was rejected ([community.sinch.com](https://community.sinch.com/t5/10DLC/Why-was-my-10DLC-campaign-rejected/m-p/15408)).
- Fiverr sellers advertise GoHighLevel A2P approval services, one promising "guarantee approval", which nobody can deliver ([fiverr](https://fiverr.com/ghl_expert_atif/create-gohighlevel-workflows-email-automations-and-crm-triggers)). Agency setups are listed from $799-$1,500 ([autogencrm](https://autogencrm.com/?p=16408)).
- Fees: brand $4.50 one-time, standard vetting $41.50 (per search summary, [textbolt](https://textbolt.com/blog/10dlc-compliance/) / [getterms](https://getterms.io/blog/what-is-a2p-10dlc)).
- GitHub shows 154 repos matching "10dlc" created since Jun 2025, mostly vendor code samples, so there is low "productised template" supply on GitHub (`gh api search/repositories`).

**What buyers would buy:** an "A2P 10DLC Approval Kit". It would contain:
- SMS-specific privacy-policy clauses (mobile data not shared or sold) and SMS terms page copy.
- Opt-in form and checkbox wording plus a screenshot checklist.
- Campaign descriptions and sample messages for common SMB verticals (HVAC, dental, salons, real estate).
- STOP/HELP replies.
- A rejection-code-to-fix table.

Buyers are small businesses and especially GoHighLevel / white-label agencies that register many sub-accounts.

**Counter-evidence:** free generators (e.g. GetTerms) and provider docs explain the requirements, and carriers can still reject for brand/website reasons a template can't fix.

**Liability:** TCPA exposure is high-stakes. Sell as templates plus a checklist, with "not legal advice" and "no approval guaranteed" framing. **Evidence: MEDIUM** (primary Twilio docs plus forum anecdotes; no count of rejections found). Dates: 2026.

**Verdict:** strong one-day product with a clear buyer gathering place (GHL Facebook groups and forums, r/gohighlevel, r/twilio; not verified in this session).

---

### 4. AI search and Google local changes (AI Overviews, AI Mode, Ask Maps, ChatGPT recommendations): seed hypothesis 2

**What changed:**
- AI Overviews correlate with a 58% lower CTR for top-ranking pages (Ahrefs, Feb 2026) ([thenextweb](https://thenextweb.com/news/google-ai-overviews-publisher-links-search-traffic), [seo-kreativ](https://www.seo-kreativ.de/en/blog/google-ai-overviews-updates-2026-en/)).
- Pew (Jul 2025) found users click a classic result 8% of the time with an AI Overview vs 15% without (via [searchenginejournal](https://www.searchenginejournal.com/impact-of-ai-overviews-how-publishers-need-to-adapt/556843/)).
- SparkToro measured zero-click searches at 68% in early 2026 ([Search Engine Land](https://searchengineland.com/google-zero-click-searches-2026-study-479717)).
- Google said at I/O 2026 that AI Mode passed 1B monthly users (per search summary; [omnibound](https://www.omnibound.ai/blog/google-ai-overviews-statistics)).
- Google retired GBP Q&A for "Ask Maps", a Gemini answer that reportedly returns one recommendation rather than three ([ppc.land](https://ppc.land/google-quietly-kills-q-a-for-an-ai-button-most-wont-use/), [thevalleymarketinggroup](https://thevalleymarketinggroup.com/blog/google-business-profile-qa-removed-ask-maps-2026/), [ppc.land data layer](https://ppc.land/google-business-profile-is-now-a-data-layer-that-feeds-ai-maps-and-search/)).
- BrightLocal's 2026 survey found 45% of US consumers used ChatGPT or other gen-AI tools for local business recommendations in the past 12 months, vs 6% a year earlier (via [bccinteractive](https://www.bccinteractive.com/blog/local-ai-search-statistics/), [seosandwitch](https://seosandwitch.com/chatgpt-local-business-statistics/)).
- SOCi found ChatGPT recommended about 1.2% of local businesses vs 35.9% appearing in Google's 3-pack (via [seosandwitch](https://seosandwitch.com/chatgpt-local-business-statistics/)), a vendor citation.

**llms.txt (counter-evidence):**
- About 10% of ~300k domains have the file (SE Ranking, May 2026). Large log studies found only about 408 llms.txt requests across 500M+ AI-bot visits, and no statistically significant correlation with AI citations ([richdevtools](https://richdevtools.com/articles/web/llms-txt-evidence-2026), [1clickreport](https://www.1clickreport.com/blog/llms-txt-evidence-2026), [limy.ai](https://limy.ai/blog/llms-txt-in-2026-the-full-guide)). The log data comes from a GEO vendor.
- **Do not sell llms.txt as a visibility lever.** 164 GitHub repos matching "llms.txt generator" were created in 2026, plus dozens of npm generators, so it is saturated and free anyway.

**Existing paid offerings:** a $19 GEO starter kit on Gumroad ([genxops.gumroad.com](https://genxops.gumroad.com/l/geo_for_smbs)), a €39 AEO Starter Kit ([aeo-starter-kit.pages.dev](https://aeo-starter-kit.pages.dev/)), a £39 white-label AEO audit kit on Payhip ([payhip](https://payhip.com/b/YzjDQ)) and a Framer template ([framer](https://www.framer.com/marketplace/templates/aeo-geo-seo/?via=doug)).

**Verdict:** the demand trend is real and growing (**STRONG** evidence for the traffic shift). Small-business willingness to pay is shown only by small-ticket kits (**WEAK**). Re-scope seed hypothesis 2 to "Get recommended by Google Maps and ChatGPT":
- GBP attribute completion
- review velocity and detail (FTC-compliant, see #5)
- LocalBusiness schema snippets for Wix/Squarespace/Shopify
- a monthly "ask the AI" self-test prompt sheet

Results are unprovable and AI answers vary between runs (one study found only 29% overlap between identical queries about 39 minutes apart, via [seosandwitch](https://seosandwitch.com/chatgpt-local-business-statistics/)), so avoid ranking promises.

---

### 5. FTC Consumer Review and Testimonials Rule (16 CFR 465)

**Status:** in force since 21 Oct 2024. On 22 Dec 2025 the FTC sent warning letters to 10 companies. In May 2026 DOJ (on FTC referral) and the Illinois AG sued Premium Home Service over fake listings and reviews. Penalties are up to $53,088 per violation, and no small-business exemption was found ([Benesch/Legal500](https://www.beneschlaw.com/insight/five-stars-zero-tolerance-ftc-turns-up-enforcement-under-consumer-review-rule/), [regulatoryoversight](https://www.regulatoryoversight.com/2026/01/ftc-warns-companies-over-deceptive-online-review-practices/), [insideprivacy](https://www.insideprivacy.com/united-states/federal-trade-commission/ftc-issues-warning-letters-for-violations-of-consumer-reviews-rule/)). One source misdates the rule's effective date to Oct 2026 and appears to be wrong.

**Who:** every local business soliciting reviews. The rule bans incentives conditioned on positive sentiment, review suppression and insider reviews without disclosure.

**Product:** compliant review-request SMS and email templates (neutral wording, no gating), a staff-review disclosure policy, and a "what not to do" checklist. Best bundled with #4, since Ask Maps and AI Overviews pull from review text ([ppc.land](https://ppc.land/google-business-profile-is-now-a-data-layer-that-feeds-ai-maps-and-search/)).

**Evidence: MEDIUM-STRONG.** **Verdict:** good add-on, weak as a standalone.

---

### 6. AI voice agents and receptionists: disclosure, consent and recording (supports seed hypothesis 6)

**Verified status:**
- **FCC:** the Feb 2024 declaratory ruling treats AI-generated voices as "artificial" under the TCPA, so outbound calls need prior express consent (written for telemarketing). The Aug 2024 NPRM (FCC 24-84) proposing AI-disclosure duties is listed in the Aug 2026 Unified Agenda under "Long-Term Actions" with "Next Action Undetermined". No final rule was found as of 5 Oct 2026 ([FCC 24-84](https://docs.fcc.gov/public/attachments/FCC-24-84A1.pdf), [leandiscoverygroup](https://www.leandiscoverygroup.com/post/ai-voice-agent-disclosure-consent), [justcall](https://justcall.io/blog/ai-voice-agent-disclosure-laws.html)).
- **States:**
  - California AB 2905 (eff. 1 Jan 2025) requires robocall disclosure of AI-generated voices.
  - Utah requires disclosure when asked, and proactively for regulated occupations; the 2025 amendments narrowed the original law.
  - Maine requires a clear notice where a consumer could be misled, but whether it covers phone calls is contested ([zian.ai](https://zian.ai/us-state-ai-call-disclosure-laws/), [aiemply](https://aiemply.com/blog/ai-receptionist-disclosure-laws), [pyai tracker](https://pyai.com/voice-ai-compliance/laws)).
- **Recording consent:** about 12 all-party-consent states (counts vary from 9 to 12 between sources) ([getnextphone](https://getnextphone.com/blog/call-recording-laws-by-state), [retellai](https://www.retellai.com/blog/legally-recording-phone-calls-in-the-us-how-does-it-work)).
- **Litigation:**
  - *Ambriz v. Google*: in Feb 2025, N.D. Cal. let CIPA wiretap claims proceed against Google's Contact Center AI. Commentators report "over a dozen" similar suits against AI call-centre tools ([pearlcohen](https://www.pearlcohen.com/google-may-be-unlawfully-eavesdropping-with-ai-according-to-federal-court/), [mondaq](https://www.mondaq.com/unitedstates/privacy-protection/1591946/ai-voice-products-subject-to-california-invasion-of-privacy-claims)). This is **OLD** (2025) and the 2026 status was not found.
  - California SB 690 was signed on 30 Sep 2026 per WilmerHale. It narrows pen-register/trap-and-trace website claims but not all-party recording claims ([WilmerHale](https://www.wilmerhale.com/en/insights/blogs/wilmerhale-privacy-and-cybersecurity-law/20261006-cipa-reform-signed-into-law), [Parker Poe](https://www.parkerpoe.com/news/2026/08/california-legislature-approves-senate-bill-690-narrowing-certain)).
- **Healthcare:** a BAA is a precondition for AI receptionists handling patient calls ([hellopatient](https://home.hellopatient.com/learn/ai-receptionist-hipaa-compliant)), a vendor source. No Vapi/Retell BAA documentation was found.

**Product:** a "voice-agent compliance script pack" containing:
- opening disclosure lines covering both AI and recording (with a no-record fallback)
- a per-state table
- an outbound consent-capture wording template
- a clinic BAA and vendor questionnaire

This is best bundled into seed hypothesis 6's receptionist templates.

**Counter-evidence:** builder supply is saturated (3,426 GitHub repos matching "ai receptionist" created in 2026, per `gh api` search, a fuzzy count). Vendors publish free checklists ([dialzara](https://dialzara.com/blog/ai-phone-agent-compliance-checklist), [thoughtly](https://thoughtly.com/blog/call-recording-consent-ai-voice-agents-state-guide)). **Evidence: MEDIUM** (mostly vendor blogs; FCC docs primary).

---

### 7. UK Data (Use and Access) Act 2025: data-protection complaints procedure

**Status:** from 19 Jun 2026, controllers must provide a way to make data-protection complaints and acknowledge them within 30 days (DPA 2018 s.164A, inserted by DUAA s.103) ([Mishcon](https://www.mishcon.com/news/is-your-data-protection-complaints-process-ready-for-19-june-2026), [Mayer Brown](https://www.mayerbrown.com/en/insights/publications/2026/02/preparing-for-the-data-use-and-access-act-2025-upcoming-complaints-procedure-requirement), [privacyworld](https://www.privacyworld.blog/2026/06/the-data-use-and-access-act-2025-and-the-new-right-for-individuals-to-complain-to-controllers-what-organisations-need-to-do-before-19-june-2026/), [ICO blog May 2026](https://ico.org.uk/about-the-ico/media-centre/news-and-blogs/2026/05/one-month-to-go-what-businesses-need-to-know-to-meet-new-data-law)). ICO guidance (final, Feb 2026) is cited as saying there are no exemptions ([Arnold & Porter](https://www.arnoldporter.com/en/perspectives/advisories/2026/02/ico-publishes-guidance-on-how-to-deal-with-data-protection-complaints)).

**Who:** effectively every UK business, charity, club and sole trader holding personal data. No count was found.

**Existing offerings:** a free template behind a waitlist ([complaintsdesk](https://complaintsdesk.pages.dev/duaa-complaints-procedure)); vendor guides from [iubenda](https://www.iubenda.com/en/blog/uks-six-step-guide-on-handling-data-protection-complaints/) and [sprintlaw](https://sprintlaw.co.uk/articles/handling-ico-complaints-a-stepbystep-business-guide/). No priced Etsy/Gumroad listing was found.

**Product:** a procedure document, acknowledgement and outcome letter templates, a Sheets complaint log with a 30-day timer, and a website "how to complain" snippet.

**Counter-evidence:** low awareness, no enforcement found, and ICO guidance is free. **Evidence: MEDIUM-STRONG** (law firms plus ICO). **Verdict:** cheap and quick to build; demand unproven, so test on Etsy UK with a £7-£15 price.

---

### 8. Subscription auto-renewal rules (federal click-to-cancel vacated; states active)

**Status:**
- The Eighth Circuit vacated the FTC Negative Option ("click-to-cancel") rule on 8 Jul 2025 on procedural grounds ([Cooley](https://www.cooley.com/news/insight/2025/2025-07-11-click-to-cancel-just-got-cancelled-eighth-circuit-vacates-entirety-of-ftcs-negative-option-rule)).
- The FTC restarted rulemaking with an ANPRM sent to OIRA on 30 Jan 2026 (comments were due 13 Apr 2026) and keeps enforcing ROSCA ([Jones Day](https://www.jonesday.com/en/insights/2026/05/ftc-revives-clicktocancel-rule-new-risks-for-subscription-businesses), [Gibson Dunn](https://www.gibsondunn.com/ftc-restarts-negative-option-rulemaking-after-eighth-circuit-vacatur-enforcement-under-rosca-continues/), [Crowell](https://www.crowell.com/en/insights/client-alerts/clicking-all-the-right-boxes-ftc-moves-to-revive-click-to-cancel-rule-following-eighth-circuit-vacatur)).
- California's ARL amendments (AB 2863), effective 1 Jul 2025, require online click-to-cancel and separate express consent to auto-renewal ([fkks](https://advertisinglaw.fkks.com/post/102jkbj/california-amends-its-auto-renewal-law-effective-july-1-2025), [Venable](https://www.venable.com/insights/publications/2025/07/july-1-and-july-14-autorenewal-and-negative-opt)).
- New York amendments took effect 5 Nov 2025, including an in-app cancel button and 5-business-day notice of material changes ([Hudson Cook](https://hudsoncook.com/article/keeping-your-eye-on-the-ball-federal-cancellation-policy-settlements-and-new-york-updates-to-auto-renewal-law/)).
- Litigation is rising in CA ([mondaq](https://www.mondaq.com/unitedstates/consumer-law/1769282/that-free-trial-might-cost-you-automatic-renewal-litigation-on-the-rise-in-ca)).

**Product:** a checklist plus checkout and cancellation-flow copy and renewal-reminder email templates for small membership, course and SaaS sellers (Gumroad, Lemon Squeezy, Kajabi, Shopify subscriptions).

**Verdict:** niche but well-matched to creator-economy buyers. **Evidence: MEDIUM** (law-firm sources; dates 2025 are **OLD** but still operative).

---

### 9. Etsy policy shifts for AI-assisted digital products (risk to the founder's own channel)

- Etsy added digital downloads to its Creativity Standards on 10 Jun 2025 ([promptlesspress](https://www.promptlesspress.com/blog-etsy-ai-policy-2026-digital-products)).
- Enforcement of "Designed by" attribution for AI-assisted items is reported from 14 Jan 2026 ([ngini](https://ngini.com/en-us/blog/etsy-ai-disclosure-policy-2026-explained)).
- Etsy says digital listings "should include a visual preview or excerpt of the content buyers will receive" (quoted in [inkfluenceai](https://www.inkfluenceai.com/blog/etsy-ai-disclosure-explained-2026)).
- Raw AI prompt bundles are reported as prohibited ([inkfluenceai Oct 2026](https://www.inkfluenceai.com/blog/etsy-ai-rules-update-october-2026)).
- One blog claims about 12,000 listings were removed in Q1 2026, which is **unverified** ([prcreativedigital](https://www.prcreativedigital.com/blog/etsy-ai-disclosure-policy-2026-shoppers.html)).
- GPSR: non-EU physical-goods sellers need an EU responsible person. Whether it applies to digital downloads is disputed ([stallscore](https://stallscore.pages.dev/learn/etsy-gpsr), [craftybase](https://craftybase.com/blog/what-is-gpsr)).

**Evidence: WEAK-MEDIUM** (SEO blogs, no Etsy primary source retrieved).

**Implication for the lead:** any Etsy listing for Claude-built templates must disclose AI use, show genuine creative contribution and include previews. "Prompt packs" are risky on Etsy. A cheap "Etsy AI-disclosure compliance checklist for digital sellers" is possible but evidence is thin.

---

### 10. TAKE IT DOWN Act: notice-and-removal for platforms hosting user content

**Status:** platform duties have been enforceable since 19 May 2026. Covered platforms must remove reported non-consensual intimate imagery within 48 hours. The FTC issued warning letters on day one and runs complaints via TakeItDown.ftc.gov. Penalties are up to $53,088 per violation ([FTC press release, May 2026](https://www.ftc.gov/news-events/news/press-releases/2026/05/ftc-begins-enforcing-take-it-down-act), [WilmerHale](https://wilmerhale.com/en/insights/client-alerts/20260615-the-take-it-down-act-goes-live), [Wiley](https://www.wiley.law/alert-May-19-Deadline-for-TAKE-IT-DOWN-Act-Compliance-Is-Your-Company-Prepared)).

**Who:** the definition is broad. Law firms suggest any customer-facing platform where users post content should check scope ([Wiley](https://www.wiley.law/alert-May-19-Deadline-for-TAKE-IT-DOWN-Act-Compliance-Is-Your-Company-Prepared)). No small-site exemption was found.

**Product:** a takedown policy, request form copy, a 48-hour SOP and a log template for small forums, Discord-adjacent sites and community/membership sites.

**Verdict:** niche, low price. **Evidence: MEDIUM** (FTC primary). Hosted platforms (Circle, Skool) may handle this for their users, which reduces demand.

---

### 11. Public-sector and healthcare web accessibility rules (delayed)

- **ADA Title II:** a DOJ interim final rule (20 Apr 2026) moved compliance to 26 Apr 2027 for entities serving 50k+ people and 26 Apr 2028 for smaller entities and special districts. The DOJ says it "fully anticipates implementing the regulation at the new deadline" ([Duane Morris](https://www.duanemorris.com/alerts/doj_extends_ada_title_ii_digital_accessibility_deadlines_one_year_0426.html), [adatitleiii.com](https://www.adatitleiii.com/2026/04/doj-extends-ada-title-ii-website-accessibility-deadlines-for-governmental-entities-but-litigation-and-compliance-risks-remain/), [UPCEA](https://upcea.edu/doj-extends-accessibility-deadline-to-april-2027-policy-matters-april-2026/)).
- **HHS Section 504:** an interim final rule (FR 11 May 2026) moved deadlines to 11 May 2027 (15+ employees) and 10 May 2028 (smaller). HHS plans to reconsider substance ([Federal Register via govinfo](https://www.govinfo.gov/content/pkg/FR-2026-05-11/html/2026-09266.htm), [LeadingAge](https://leadingage.org/web-accessibility-compliance-date-delayed-under-hhs-section-504-regulations/)).
- A lawsuit challenges both delays ([Disability Scoop, Jun 2026](https://www.disabilityscoop.com/2026/06/08/trump-administration-sued-over-delay-of-accessibility-rules/32033/)).

**Verdict:** low urgency now; revisit in early 2027 for a "small clinic website accessibility checklist" (HHS-funded providers, e.g. Medicaid). **Evidence: STRONG** (Federal Register primary).

---

### 12. EU e-invoicing mandates

- **Belgium:** B2B Peppol e-invoicing mandatory since 1 Jan 2026, with a Q1 2026 tolerance period ([vatcalc](https://www.vatcalc.com/belgium/belgium-b2b-e-invoicing-july-2024-update/), [truecommerce](https://www.truecommerce.com/blog/e-invoicing-in-belgium-your-guide-to-the-2026-mandate/)).
- **Poland KSeF:** largest firms from 1 Feb 2026, most from 1 Apr 2026, the smallest (≤PLN 10k monthly sales) from 1 Jan 2027. The penalty deferral to 31 Dec 2027 was announced on 16 Sep 2026 and was a draft law as of 20 Oct 2026, not yet enacted ([Sovos](https://sovos.com/regulatory-updates/vat/poland-ministry-of-finance-extends-ksef-penalty-relief-until-end-of-2027/), [KPMG PL](https://kpmg.com/pl/en/insights/taxes/tax-alert-extension-of-the-deferral-of-penalties-for-errors-in-using-ksef-until-the-end-of-2027.html)).
- **France:** all VAT-registered firms must be able to receive e-invoices from 1 Sep 2026. SMEs and micro-enterprises must issue from 1 Sep 2027, which requires choosing a "plateforme agréée" ([service-public.gouv.fr](https://entreprendre.service-public.gouv.fr/actualites/A15683?lang=en), [hayot-expertise](https://hayot-expertise.fr/blog/facturation-electronique-2026-obligation-reception-1er-septembre), [abby.fr](https://abby.fr/guide/facturation-electronique/facture-electronique-septembre-2026)). One outlier source says micro firms have until 2028 ([invoicedataextraction](https://invoicedataextraction.com/blog/france-e-invoicing-mandate-2026)).
- **Germany:** reception since 2025; issuance from 1 Jan 2027 for turnover over €800k and 2028 for others (most-specific source; [enterpryze](https://www.enterpryze.com/post/peppol-e-invoicing-mandates-2026-eu-sme-guide)).

**Verdict:** affects millions of micro firms (a STRONG forcing function), but they need software (platforms and accounting tools), not templates. A guide or checklist would have to be in French, Polish or German and sold off Gumroad/Etsy. **Low fit** for this founder.

---

### 13. EU AI Act: Art. 4 AI literacy, Art. 50 transparency, high-risk delay (seed hypothesis 3)

**Verified status:**
- The Digital Omnibus on AI (Reg. (EU) 2026/1744) was politically agreed on 7 May 2026 and adopted by Parliament (16 Jun) and Council (29 Jun). It was published on 24 Jul and entered into force on 27 Jul 2026.
- Annex III high-risk obligations move to 2 Dec 2027 and Annex I (product-embedded) to 2 Aug 2028 ([usercentrics](https://usercentrics.com/knowledge-hub/eu-ai-act-high-risk-delay-article-50-transparency-consent/), [White & Case](https://www.whitecase.com/insight-alert/eu-ai-omnibus-enters-force-amending-ai-act), [FPF](https://fpf.org/blog/the-ai-act-implementation-timeline-what-changes-under-the-ai-omnibus/), [CSA](https://labs.cloudsecurityalliance.org/research/csa-research-note-eu-ai-act-omnibus-vii-deadline-delay-20260/)).
- **Art. 4** was rewritten. Providers and deployers must "take measures" to support AI literacy, without guaranteeing any individual's level ([casys.ai](https://casys.ai/blog/digital-omnibus-article-4-what-changed), [White & Case](https://www.whitecase.com/insight-alert/eu-ai-omnibus-enters-force-amending-ai-act)). Art. 99 lists no EU-level fine for Art. 4; penalties come from national law, which may include warnings ([pk-sharma](https://www.pk-sharma.com/tools/ai-literacy-obligation), [aiprioritymap](https://aiprioritymap.com/en/insights/ai-literacy-article-4-eu-ai-act)). **No Art. 4 enforcement action was found.**
- **Art. 50** (AI-interaction disclosure, deepfake/AI-text labelling) applies from 2 Aug 2026. Generative systems already on the market get until 2 Dec 2026 for machine-readable marking. The Transparency Code of Practice was published 10 Jun 2026 (about 190 signatories by end-Jul) and the Commission's Art. 50 guidelines were approved on 20 Jul 2026 ([artificialintelligenceact.eu](https://artificialintelligenceact.eu/transparency-rules-article-50/), [EC Code page](https://digital-strategy.ec.europa.eu/en/policies/code-practice-ai-generated-content), [MoFo](https://www.mofo.com/resources/insights/260911-full-transparency-organizations-sign-eu-code), [ai-resources.eu](https://ai-resources.eu/soft-law/transparency-guidelines-art-50/)). Art. 50(1) chatbot disclosure falls mainly on providers, so SMBs embedding a vendor's bot have a lighter role (inference from the article structure; not separately verified).

**Supply (saturation evidence):**
- Etsy kits at $12.99, $20.76 and $131.27 ([Etsy market "ai policies"](https://www.etsy.com/market/ai_policies), [Etsy 2026 bundle](https://www.etsy.com/listing/4430787946/2026-ai-compliance-bundle-for-eu-and-us)).
- Vendor kits at €990 ([compliance-kit.eu](https://compliance-kit.eu/en/kits/eu-ai-act)), $99 ([governancedocs](https://governancedocs.com/product/eu-ai-act-toolkit/)) and from $229 ([trustpacket](https://www.trustpacket.app/pack)).
- Free templates from [Praxikon](https://www.praxikon.com/en/templates), [aiactblog.nl](https://www.aiactblog.nl/en/templates) and [complylayer](https://complylayer.com/guides/ai-acceptable-use-policy-template).
- GitHub: 1,125 repos matching "eu ai act compliance" created since 1 Jan 2026, including a Claude GRC skills repo with 1,025 stars ([Sushegaad/Claude-Skills-Governance-Risk-and-Compliance](https://github.com/Sushegaad/Claude-Skills-Governance-Risk-and-Compliance)). npm has 20+ EU-AI-Act MCP/compliance packages updated in 2026.

**Demand signal:** a Reddit-mirror thread claims companies are "sleeping on Article 4" ([reddit mirror 1t3gtml](https://reddit.sentinel-team.org/posts/1t3gtml/snapshots/2026-05-07T16%3A03%3A41.170452Z); exact attribution between this and [mirror 1tinc58](https://reddit.sentinel-team.org/posts/1tinc58/snapshots/2026-05-25T23%3A35%3A02.893844Z) unclear, content not opened). A single anecdote, **WEAK**.

**Verdict:** **reject as a standalone product.** The duty was softened, there is no EU fine and no enforcement, and supply is crowded and partly free. A short "AI use policy + staff AI-literacy one-pager" could be a bundle sweetener only. **Evidence on status: STRONG.**

---

### 14. US state AI laws and federal preemption

- **Colorado:** SB 24-205 was delayed to 30 Jun 2026, then repealed and replaced by SB 26-189 (signed 14 May 2026), which is narrower, disclosure-focused and effective 1 Jan 2027. A stipulated order in xAI's suit (joined by DOJ) bars enforcement ([Eckert Seamans](https://www.eckertseamans.com/legal-updates/colorado-repeals-and-replaces-its-landmark-ai-statute-what-businesses-need-to-know), [techtimes](https://www.techtimes.com/articles/319420/20260701/colorado-ai-law-reset-discrimination-duty-dropped-disclosure-takes-its-place.htm), [intellisee](https://intellisee.com/intelligence/colorado-ai-act-sb-24-205-repeal-2026-compliance-briefing/)).
- **Texas TRAIGA:** effective 1 Jan 2026. Private-sector disclosure duties mainly cover healthcare; no small-business carve-out was found ([Norton Rose Fulbright](https://www.nortonrosefulbright.com/en-us/knowledge/publications/c6c60e0c/the-texas-responsible-ai-governance-act), [Texas AG](https://oag.state.tx.us/consumer-protection/file-consumer-complaint/consumer-ai-rights)).
- **Illinois HB 3773:** effective 1 Jan 2026. Employers with 1+ Illinois employee must give notice when AI influences employment decisions. IDHR draft rules were reportedly withdrawn on 2 Jun 2026, a single-source claim ([Seyfarth](https://www.seyfarth.com/news-insights/legal-update-new-illinois-ai-law-requires-employee-notice-affirms-existing-employer-nondiscrimination-duties.html), [casrai](https://casrai.org/guides/illinois-hb-3773-ai-employment-discrimination)).
- **Companion-chatbot laws:** California SB 243 (1 Jan 2026) excludes customer-service bots ([Skadden](https://skadden.com/insights/publications/2025/10/new-california-companion-chatbot-law)). New York's companion law took effect 5 Nov 2025 and a new youth chatbot law was signed on 28 Oct 2026 (compliance 1 Jan 2027) ([Fenwick](https://www.fenwick.com/insights/publications/new-yorks-ai-companion-safeguard-law-takes-effect), [IAPP](https://iapp.org/news/a/new-york-s-governor-signs-youth-ai-chatbot-safety-bill)). About 12 states have companion-chatbot laws per Orrick ([Orrick](https://www.orrick.com/en/Insights/2026/04/2026-State-Chatbot-Laws-Key-Provisions-and-Regulatory-Trends)).
- **California AI Transparency Act** (SB 942 as delayed by AB 853): operative 2 Aug 2026 for large GenAI providers ([Morgan Lewis](https://morganlewis.com/pubs/2026/08/new-california-ai-disclosure-rules-become-operative)). Not small buyers.
- **Federal:** EO 14365 (11 Dec 2025) created a DOJ AI Litigation Task Force (stood up 9 Jan 2026) to challenge state AI laws. Congress has not enacted preemption ([Paul Hastings](https://www.paulhastings.com/insights/client-alerts/president-trump-signs-executive-order-challenging-state-ai-laws), [Ropes & Gray](https://www.ropesgray.com/en/insights/alerts/2026/03/the-white-house-legislative-recommendations-national-policy-framework-for-artificial-intelligence-an)).

**Verdict:** fluid and contested, with few small buyers affected. The only cheap-product angle is an Illinois AI-hiring notice template (WEAK). **Evidence: MEDIUM.**

---

### 15. AI in schools and tutoring (seed hypothesis 9)

- **Ohio:** HB 96 (ORC 3301.24) required every district, community school and STEM school to adopt an AI policy by 1 Jul 2026. The deadline has passed. A state model policy is available and the law does not dictate content ([KJK](https://kjk.com/2026/06/12/ohios-july-1-2026-school-ai-policy-deadline-what-districts-educators-and-parents-need-to-know/), [Ohio DEW](https://education.ohio.gov/Media/Media-Releases/2025-Media-Releases/Ohio-Department-of-Education-and-Workforce-Release)).
- **Other states:** Tennessee required policies earlier and the TSBA model policy was widely adopted. New laws in Idaho, Maryland, Oklahoma and Virginia require board policies, and Maryland adds an AI coordinator ([Yahoo/news](https://www.yahoo.com/news/politics/articles/4-more-states-require-districts-050000407.html), [truemadeai](https://www.truemadeai.com/resources/state-k12-ai-laws-and-guidance)). 34 states plus Puerto Rico had guidance by Oct 2025 ([aiforeducation](https://www.aiforeducation.io/ai-resources/state-ai-guidance)).
- **UK:** the DfE "Generative AI: product safety standards" were updated 19 Jan 2026. KCSIE 2026 (statutory, effective 1 Sep 2026) points schools to them ([edtechinnovationhub](https://www.edtechinnovationhub.com/news/dfe-publishes-kcsie-2026-with-mobile-phone-free-default-and-ai-safeguarding-rules), [GOV.UK policy paper](https://www.gov.uk/government/publications/generative-artificial-intelligence-in-education)).
- **Australia:** the national framework is voluntary guidance ([educatoronline](https://www.theeducatoronline.com.au/k12/news/ai-framework-for-schools-released/283752)).
- **US federal:** EO 14277 (Apr 2025) promotes AI education rather than restricting it ([UCSB presidency](https://www.presidency.ucsb.edu/documents/executive-order-14277-advancing-artificial-intelligence-education-for-american-youth)).
- **Tutoring centres:** no mandate found anywhere in these searches.
- **Free supply:** [Tes](https://www.tes.com/en-nz/teaching-resource/artificial-intelligence-ai-policy-template-13133971), [Third Space Learning](https://thirdspacelearning.com/blog/ai-policy-for-schools/), [Kuraplan](https://www.kuraplan.com/uk/ai-policy?year=1) (paid full pack) and state model policies.

**Verdict:** **weak.** District buyers have free model policies and procurement processes, and no rule forces tutoring centres. A parent-facing "how we use AI" letter pack for tutors would be a nice-to-have, not a must-buy. **Evidence: MEDIUM.**

---

### 16. Email sender requirements (Gmail, Yahoo, Microsoft)

- **Gmail:** moved from temporary deferrals to permanent 5xx rejections in Nov 2025 for non-compliant bulk senders (5,000+/day to personal Gmail). Requirements are SPF, DKIM, DMARC (p=none OK), one-click unsubscribe and spam rate under 0.3% ([gmass](https://www.gmass.co/blog/gmail-bulk-sender-guidelines/), [redsift](https://redsift.com/resources/blog/gmails-enforcement-ramps-up-what-bulk-senders-need-to-know), [valimail](https://www.valimail.com/blog/google-email-compliance-enforcement/)).
- **Microsoft:** since 5 May 2025, 5,000+ senders must pass SPF and DKIM and publish DMARC, with failures bounced as 550 5.7.515 ([Microsoft support](https://support.microsoft.com/outlook/fix-ndr-error-550-5-7-515-in-outlook-com), [Microsoft Tech Community](https://techcommunity.microsoft.com/blog/microsoftdefenderforoffice365blog/strengthening-email-ecosystem-outlook%E2%80%99s-new-requirements-for-high%E2%80%90volume-senders/4399730/replies/4418393)).

**Verdict:** most micro businesses send through ESPs that handle this, and free DNS generators abound. **Low.** **Evidence: STRONG** (Microsoft primary).

---

### 17. Other shifts checked (mostly drop)

| Shift | Verified status | Why it is weak for this founder | Key source |
|---|---|---|---|
| New US state privacy laws (IN, KY, RI on 1 Jan 2026; MD MODPA enforcement 1 Apr 2026) | In force; ~19-20 states | Thresholds (e.g. 100k consumers; RI 35k) exclude most micro firms; generators (Termly, iubenda) dominate | [TrustArc](https://trustarc.com/resource/new-in-2026-state-privacy-laws-in-indiana-kentucky-and-rhode-island/), [MSBA](https://msba.org/site/content/News-and-Publications/News/General-News/Maryland_Online_Data_Privacy_Act.aspx) |
| CCPA regs (ADMT 1 Jan 2027; risk assessments; cyber audits from 2028) | Effective 1 Jan 2026, phased | CCPA-sized businesses only | [Hunton](https://www.hunton.com/privacy-and-cybersecurity-law-blog/newly-approved-ccpa-regulations-have-staggered-deadlines-for-compliance), [Thompson Coburn](https://www.thompsoncoburn.com/insights/californias-2026-ccpa-regulations-summary-and-preparation-guide/) |
| COPPA Rule amendments | Compliance date 22 Apr 2026 passed; FTC Feb 2026 age-verification policy statement; no enforcement citing new rule found (single source) | Narrow pool (kids' apps, edtech) | [Davis Polk](https://www.davispolk.com/insights/client-update/ftc-prioritizes-coppa-enforcement-new-compliance-obligations-take-effect), [Hunton](https://www.hunton.com/privacy-and-cybersecurity-law-blog/coppa-rule-amendment-compliance-deadline-approaches) |
| Google Consent Mode v2 / certified CMP | Google platform requirement for EEA ads; certified CMP for AdSense/AdMob publishers | Many CMPs; technical | [measuremindsgroup](https://measuremindsgroup.com/is-consent-mode-v2-mandatory), [consentbit](https://www.consentbit.com/blog/do-you-need-a-google-certified-cmp-what-googles-requirement-actually-means) |
| EU Digital Omnibus GDPR/cookie changes | Not adopted. Council mandate 22 Oct 2026; Parliament position not before ~Feb 2027; browser-signal duty dropped by Council | Nothing changes yet; future simplification may reduce banner needs | [euinternetpolicy](https://euinternetpolicy.wordpress.com/2026/10/23/the-councils-digital-omnibus-mandate-what-it-would-change-in-the-gdpr/), [acompli](https://acompli.ie/news/digital-omnibus-gdpr-cookies-status-september-2026/) |
| EU Pay Transparency Directive | Transposition deadline 7 Jun 2026 missed by most (only 4 states fully transposed); job-ad / pre-interview pay range applies to all employers where transposed; pay-gap reports 2027 (150+) | Country-by-country fragmentation; revisit in 2027 | [Littler](https://www.littler.com/news-analysis/asap/eleventh-hour-implementation-status-eu-pay-transparency-directive), [Lewis Silkin](https://www.lewissilkin.com/insights/2026/07/01/eu-pay-transparency-directive-2026-employer-compliance), [Crowe](https://www.crowe.com/uk/insights/eu-pay-transparency-directive) |
| EU Cyber Resilience Act reporting | Art. 14 reporting from 11 Sep 2026 via ENISA platform; most duties 11 Dec 2027 | Manufacturers of digital products; legal-heavy (note: could affect EU sales of the founder's own software) | [EC CRA reporting](https://digital-strategy.ec.europa.eu/en/policies/cra-reporting), [Jones Day](https://www.jonesday.com/en/insights/2026/07/eu-cyber-resilience-act-24hour-reporting-duties-start-september-11-2026) |
| NIS2 (Germany) | In force 6 Dec 2025; ~29,500 entities; registration due 6 Mar 2026 | Mid-size and up | [Reed Smith](https://www.reedsmith.com/articles/germany-implements-nis2-immediate-effect-broad-scope-near-term-registration/), [JD Supra](https://www.jdsupra.com/legalnews/new-cybersecurity-regulations-in-2713282/) |
| PCI DSS 4.0.1 SAQ A | Jan 2025 revision removed 6.4.3/11.6.1 from SAQ A but added a script-attack eligibility criterion | Hosted-checkout SMBs largely covered by platforms | [PCI SSC blog](https://blog.pcisecuritystandards.org/faq-clarifies-new-saq-a-eligibility-criteria-for-e-commerce-merchants) |
| HIPAA Security Rule overhaul | Still proposed; final action target Jul 2027; 100+ groups asked for withdrawal | No 2026 forcing function | [HIPAA Journal](https://www.hipaajournal.com/ocr-gives-update-on-proposed-hipaa-security-rule/), [pact-one](https://www.pact-one.com/2026/09/hipaa-security-rule-2026-status/) |
| FTC Safeguards Rule (tax preparers' WISP) | Longstanding (2023), IRS still pushing (IRS issue 2026-22) | Free official template (IRS Pub 5708); no paid listing prices found | [IRS 2026-22](https://www.irs.gov/pub/opr-taxpros/issue-number-2026-22-how-to-be-a-careful-wisper.pdf), [CPA Practice Advisor Oct 2026](https://www.cpapracticeadvisor.com/2026/10/02/what-the-ftc-safeguards-rule-actually-requires-from-tax-and-accounting-firms/) |
| US 1099 thresholds | 1099-K back to $20k/200 transactions (OBBBA); 1099-NEC/MISC to $2,000 for TY2026 | Relief, not new burden | [CPA Practice Advisor](https://cpapracticeadvisor.com/2025/07/30/one-big-beautiful-bill-act-changes-1099-thresholds/165863/), [Patriot](https://www.patriotsoftware.com/blog/accounting/1099-reporting-threshold/) |
| Australia Privacy Act ADM transparency | Privacy-policy ADM disclosure from 10 Dec 2026 (some say 11 Dec); A$3M small-business exemption still in place | Excludes most micro firms | [sprintlaw AU](https://sprintlaw.com.au/articles/automated-decision-making-privacy-rules/), [colemangreig](https://colemangreig.com.au/insights/privacy-reform-in-australia-what-businesses-need-to-know-in-2026-2027/) |
| EU GPSR (Dec 2024, **OLD**) | Ongoing Etsy/eBay enforcement on EU responsible person fields | Physical goods; vendor services dominate | [craftybase](https://craftybase.com/blog/what-is-gpsr), [24hour-ar](https://www.24hour-ar.com/the-hidden-risks-of-non-compliance-with-gpsr-on-amazon-etsy-ebay) |
| Website chat/pixel CIPA suits | Large wave; SB 690 signed 30 Sep 2026, narrow (pen-register/trap-and-trace) | Disclosure banner text only; liability-heavy | [Fisher Phillips](https://www.fisherphillips.com/en/insights/insights/federal-appeals-court-hands-out-win-in-website-chat-wiretap-case), [WilmerHale](https://www.wilmerhale.com/en/insights/blogs/wilmerhale-privacy-and-cybersecurity-law/20261006-cipa-reform-signed-into-law) |
| Chatbot liability for wrong answers (seed hyp. 8) | Air Canada 2024 (**OLD**); OLG Hamm May 2026 held a clinic liable for chatbot-invented titles (not final); CA AB 316 "autonomous AI" defence bar (unverified) | Supports a "chatbot QA checklist" weakly; no rule forces testing | [legaldata.law](https://www.legaldata.law/en/insights/ai-makes-up-facts-and-the-company-pays-this-ruling-is-a-warning-to-every-chatbot-operator), [innobu](https://www.innobu.com/en/articles/ai-liability-chatbot-companies-2026.html) |
| Meta / Google ads policy | Meta health/wellness conversion-event restrictions (2025) and further 2026 changes (single-source counts); Google advertiser-verification tightening | Not a template-shaped need | [Digiday](https://digiday.com/marketing/as-health-and-wellness-brands-brace-for-ad-restrictions-on-meta-marketers-and-advertisers-seek-more-transparency/), [Search Engine Land](https://searchengineland.com/google-clarifies-policy-on-false-information-in-advertiser-verification-464395) |

---

### 18. Platform shifts relevant to how the founder builds and sells (seed hypotheses 1, 5, 10)

- **Agent Skills open standard:** released by Anthropic on 18 Dec 2025 and reportedly supported by 26-40+ clients (incl. Codex, Gemini CLI, Copilot, Cursor) ([atlan](https://atlan.com/know/ai-agent/ai-agent-skills/what-are-agent-skills/), [laurentkempe](https://laurentkempe.com/2026/01/27/Agent-Skills-From-Claude-to-Open-Standard/)).
  - Paid skill marketplaces exist. Agensi suggests $5-15 per single skill and $20-50 for comprehensive ones ([agensi](https://www.agensi.io/learn/agent-skills-marketplace-sell-your-skills)). SkillHQ pays 80-85% to creators ([skillhq](https://skillhq.dev/become-seller)) and KissMySkills 35% ([kissmyskills](https://kissmyskills.com/pages/sell-your-skills)).
  - A 167-skill marketing bundle sells at $167 on Gumroad ([inflectual.gumroad.com](https://inflectual.gumroad.com/l/master-marketing-claude-skills-bundle)).
  - Sales volumes are self-reported or unavailable (**WEAK**). Compliance-flavoured skills are heavily supplied for free on GitHub (e.g. 282+ privacy skills in [mukul975/Privacy-Data-Protection-Skills](https://github.com/mukul975/Privacy-Data-Protection-Skills)).
- **ChatGPT Apps directory:** open to verified developers, but in-ChatGPT sale of digital goods or subscriptions is not allowed; only link-outs are permitted ([VentureBeat](https://venturebeat.com/technology/openai-now-accepting-chatgpt-app-submissions-from-third-party-devs-launches), [OpenAI dev forum](https://community.openai.com/t/chatgpt-app-monetization-apps-sdk/1372343)).
- **ChatGPT Instant Checkout:** launched Sep 2025 with Etsy and Shopify ([OpenAI on X](https://x.com/OpenAI/status/1972708279043367238), [Stripe](https://stripe.com/newsroom/news/stripe-openai-instant-checkout)). It was reportedly retired in Mar 2026 in favour of merchant-side checkout, which is **conflicting and unverified** ([hypotenuse](https://www.hypotenuse.ai/blog/chatgpts-instant-checkout-the-next-phase-of-agentic-commerce)).
- **Chrome MV2:** the last MV2 extensions were removed from the Chrome Web Store on 31 Aug 2026 ([Chrome developer timeline](https://developer.chrome.com/docs/extensions/develop/migrate/mv2-deprecation-timeline)). Any new extension must be MV3. This is not a buyer forcing function.
- **Payments:** Gumroad is reported at 10% plus processing and not a merchant of record (seller handles VAT). Lemon Squeezy is reported at 5% + 50¢ as a merchant of record, with migration toward Stripe's managed products (single blog, unverified) ([wearefounders](https://www.wearefounders.uk/gumroad-fees-2026-what-sellers-actually-pay-per-sale/), [fungies](https://fungies.io/whop-vs-gumroad-vs-lemon-squeezy-2026)). This matters for EU/UK VAT on the founder's own sales.

---

## Implications for the seed hypotheses (regulatory lens only)

| # | Hypothesis | Regulatory/platform evidence | Lean |
|---|---|---|---|
| 1 | Claude Code / agent skill packs for non-dev professions | Agent Skills standard plus paid marketplaces exist; compliance-domain skills are heavily free on GitHub | Neutral; avoid compliance-domain skills |
| 2 | "Get found by AI search" kits | Strong traffic-shift evidence; Ask Maps and AI Overviews use reviews and GBP data; llms.txt shows no measurable effect | Support, re-scoped to GBP, reviews and schema (+ FTC review-rule templates) |
| 3 | EU AI Act starter packs | Softened Art. 4, no EU fine, no enforcement found, crowded and partly free | Reject as standalone |
| 4 | Accessibility fix kits (EAA/ADA) | Strongest litigation forcing function; EU micro exemption narrows EU; FTC overlay precedent limits claims | Support, with careful claims |
| 5 | MCP connectors / setup guides for niche software | Platform shift real (Agent Skills, Apps SDK); no regulatory forcing; HMRC MTD MCP already exists on npm (`hmrc-mtd-mcp`) | Out of this remit; neutral |
| 6 | Voice receptionist templates | TCPA consent, state AI-disclosure, all-party recording, CIPA suits = real compliance layer; builder supply saturated | Support only with bundled compliance scripts |
| 7 | Brand voice packs | No regulatory driver found | No evidence found (n/a) |
| 8 | Chatbot test/QA kits | Liability rulings (Air Canada 2024; OLG Hamm 2026, not final) but no rule mandates testing | Weak support |
| 9 | AI usage policy packs for schools/tutoring | District mandates use free model policies; no tutoring mandate found | Weak / reject |
| 10 | SOP-to-agent converters | No regulatory driver found | No evidence found (n/a) |

**New candidates surfaced by this remit (not in the seed list):**
- UK MTD ITSA records template plus bridging guide
- A2P 10DLC approval kit
- UK DUAA complaints-procedure pack
- FTC-compliant review-request kit
- Auto-renewal (CA/NY) compliance kit for creators
- TAKE IT DOWN Act takedown pack for small communities

## Selling compliance products: risk notes

- **Claims risk is itself regulated.** The FTC's $1M order against accessiBe for unsubstantiated accessibility claims ([fkks](https://technologylaw.fkks.com/post/102jsmj/ftc-finds-website-overlay-tool-failed-to-deliver-accessibility-promises)) shows that "makes you compliant" marketing can draw enforcement. The same logic applies to "guaranteed 10DLC approval" (as on [Fiverr](https://fiverr.com/ghl_expert_atif/create-gohighlevel-workflows-email-automations-and-crm-triggers)).
- **Use process language.** Use "checklist", "template", "starting point" and "not legal/tax advice; consult a qualified professional". Date-stamp each kit ("current as of <month year>") and plan update cycles, because statuses moved repeatedly in 2025-2026 (EU Omnibus, Colorado, DOJ/HHS delays, TCPA revoke-all).
- **Unauthorized-practice-of-law rules were not researched here.** Generic templates are commonly sold with disclaimers (e.g. Etsy AI-policy kits), but this session did not verify jurisdiction-specific limits. The lead should check this before selling legal templates.
- **Etsy's own AI-disclosure rules apply to Claude-built listings** (see #9).

## Method & limitations

- **About 70 WebSearch queries** (standard and extended), plus npm registry searches via `curl` and GitHub repository counts via `gh api search/repositories`. Pages were **not opened directly**: WebFetch is blocked for nearly all hosts in this environment. All facts come from search-result lists and the search tool's summaries/excerpts, so wording, dates and counts could carry summarisation errors. Quotation marks are used only for strings that appeared verbatim in tool results.
- **Many sources are vendor or law-firm blogs with commercial interests:**
  - accessibility trackers (EcomBack, UsableNet, TestParty)
  - GEO vendors (Limy, Profound, SOCi via blogs)
  - CMP vendors and e-invoicing platforms
  - Etsy-policy SEO blogs

  These are labelled WEAK or MEDIUM unless corroborated by primary sources (Federal Register/govinfo, FCC, FTC, ICO, GOV.UK, Microsoft, Twilio docs, PCI SSC, EC pages).
- **Several claims conflict across sources and are flagged inline:**
  - Art. 50(2) grandfathering details
  - Colorado repeal date
  - EAA microenterprise thresholds
  - MTD penalty soft-landing and wave sizes (970k vs 1.077M)
  - TCPA September 2026 order adoption
  - ChatGPT Instant Checkout retirement
  - Etsy enforcement counts
  - Shopify share of ADA suits (46.55%, unverified)
- **Reddit:** almost no Reddit threads were retrieved (the crawler is blocked). Community-pain evidence comes mainly from Zoom/Sinch community forums and two Reddit-mirror snapshots whose content was not opened. Buyer-channel claims (r/shopify, GHL groups, landlord forums) are assumptions to verify in Phase 2.
- **Gaps:**
  - No marketplace prices found for WISP templates, UK complaints templates, 10DLC kits or TAKE IT DOWN packs.
  - No counts of 10DLC rejections or of UK businesses lacking a complaints procedure.
  - No primary Etsy policy text.
  - No 2026 status for Ambriz v. Google.
  - No small-business-specific AI-search study.
  - GitHub counts are fuzzy full-text matches (indicative only).
  - Future-dated or inconsistent "as of" dates in some search results were treated cautiously.

## Sources

EU AI Act / Omnibus
- https://usercentrics.com/knowledge-hub/eu-ai-act-high-risk-delay-article-50-transparency-consent/
- https://labs.cloudsecurityalliance.org/research/csa-research-note-eu-ai-act-omnibus-vii-deadline-delay-20260/
- https://www.whitecase.com/insight-alert/eu-ai-omnibus-enters-force-amending-ai-act
- https://fpf.org/blog/the-ai-act-implementation-timeline-what-changes-under-the-ai-omnibus/
- https://casys.ai/blog/digital-omnibus-article-4-what-changed
- https://www.pk-sharma.com/tools/ai-literacy-obligation
- https://aiprioritymap.com/en/insights/ai-literacy-article-4-eu-ai-act
- https://artificialintelligenceact.eu/transparency-rules-article-50/
- https://digital-strategy.ec.europa.eu/en/policies/code-practice-ai-generated-content
- https://www.mofo.com/resources/insights/260911-full-transparency-organizations-sign-eu-code
- https://ai-resources.eu/soft-law/transparency-guidelines-art-50/
- https://www.etsy.com/market/ai_policies
- https://www.etsy.com/listing/4430787946/2026-ai-compliance-bundle-for-eu-and-us
- https://compliance-kit.eu/en/kits/eu-ai-act
- https://governancedocs.com/product/eu-ai-act-toolkit/
- https://www.trustpacket.app/pack
- https://www.praxikon.com/en/templates
- https://www.aiactblog.nl/en/templates
- https://complylayer.com/guides/ai-acceptable-use-policy-template
- https://github.com/Sushegaad/Claude-Skills-Governance-Risk-and-Compliance
- https://reddit.sentinel-team.org/posts/1t3gtml/snapshots/2026-05-07T16%3A03%3A41.170452Z
- https://reddit.sentinel-team.org/posts/1tinc58/snapshots/2026-05-25T23%3A35%3A02.893844Z

US state AI laws / federal
- https://www.eckertseamans.com/legal-updates/colorado-repeals-and-replaces-its-landmark-ai-statute-what-businesses-need-to-know
- https://www.techtimes.com/articles/319420/20260701/colorado-ai-law-reset-discrimination-duty-dropped-disclosure-takes-its-place.htm
- https://intellisee.com/intelligence/colorado-ai-act-sb-24-205-repeal-2026-compliance-briefing/
- https://www.nortonrosefulbright.com/en-us/knowledge/publications/c6c60e0c/the-texas-responsible-ai-governance-act
- https://oag.state.tx.us/consumer-protection/file-consumer-complaint/consumer-ai-rights
- https://www.seyfarth.com/news-insights/legal-update-new-illinois-ai-law-requires-employee-notice-affirms-existing-employer-nondiscrimination-duties.html
- https://casrai.org/guides/illinois-hb-3773-ai-employment-discrimination
- https://skadden.com/insights/publications/2025/10/new-california-companion-chatbot-law
- https://www.fenwick.com/insights/publications/new-yorks-ai-companion-safeguard-law-takes-effect
- https://iapp.org/news/a/new-york-s-governor-signs-youth-ai-chatbot-safety-bill
- https://www.orrick.com/en/Insights/2026/04/2026-State-Chatbot-Laws-Key-Provisions-and-Regulatory-Trends
- https://morganlewis.com/pubs/2026/08/new-california-ai-disclosure-rules-become-operative
- https://www.paulhastings.com/insights/client-alerts/president-trump-signs-executive-order-challenging-state-ai-laws
- https://www.ropesgray.com/en/insights/alerts/2026/03/the-white-house-legislative-recommendations-national-policy-framework-for-artificial-intelligence-an

Voice AI / calls / CIPA
- https://docs.fcc.gov/public/attachments/FCC-24-84A1.pdf
- https://www.leandiscoverygroup.com/post/ai-voice-agent-disclosure-consent
- https://justcall.io/blog/ai-voice-agent-disclosure-laws.html
- https://zian.ai/us-state-ai-call-disclosure-laws/
- https://aiemply.com/blog/ai-receptionist-disclosure-laws
- https://pyai.com/voice-ai-compliance/laws
- https://getnextphone.com/blog/call-recording-laws-by-state
- https://www.retellai.com/blog/legally-recording-phone-calls-in-the-us-how-does-it-work
- https://home.hellopatient.com/learn/ai-receptionist-hipaa-compliant
- https://dialzara.com/blog/ai-phone-agent-compliance-checklist
- https://thoughtly.com/blog/call-recording-consent-ai-voice-agents-state-guide
- https://www.pearlcohen.com/google-may-be-unlawfully-eavesdropping-with-ai-according-to-federal-court/
- https://www.mondaq.com/unitedstates/privacy-protection/1591946/ai-voice-products-subject-to-california-invasion-of-privacy-claims
- https://www.wilmerhale.com/en/insights/blogs/wilmerhale-privacy-and-cybersecurity-law/20261006-cipa-reform-signed-into-law
- https://www.parkerpoe.com/news/2026/08/california-legislature-approves-senate-bill-690-narrowing-certain
- https://www.fisherphillips.com/en/insights/insights/federal-appeals-court-hands-out-win-in-website-chat-wiretap-case

Accessibility
- https://www.ecomback.com/ada-website-lawsuits-recap-report/2026-mid-year-ada-website-lawsuit-report
- https://halfaccessible.com/ada-website-lawsuit-statistics-2026/
- https://accessibility.build/blog/web-accessibility-lawsuits-2026-midyear-numbers
- https://testpros.com/accessibility/web-accessibility-lawsuit-statistics/
- https://www.adatitleiii.com/
- https://www.adatitleiii.com/2026/04/doj-extends-ada-title-ii-website-accessibility-deadlines-for-governmental-entities-but-litigation-and-compliance-risks-remain/
- https://www.duanemorris.com/alerts/doj_extends_ada_title_ii_digital_accessibility_deadlines_one_year_0426.html
- https://upcea.edu/doj-extends-accessibility-deadline-to-april-2027-policy-matters-april-2026/
- https://www.govinfo.gov/content/pkg/FR-2026-05-11/html/2026-09266.htm
- https://leadingage.org/web-accessibility-compliance-date-delayed-under-hhs-section-504-regulations/
- https://www.disabilityscoop.com/2026/06/08/trump-administration-sued-over-delay-of-accessibility-rules/32033/
- https://testparty.ai/blog/ada-demand-letter-shopify-merchant-guide
- https://accesscomply.pages.dev/blog/ada-demand-letter-shopify-store
- https://testparty.ai/blog/is-accessibe-worth-it
- https://testparty.ai/blog/are-accessibility-overlays-legal
- https://alttext.ai/vs/accessibe
- https://technologylaw.fkks.com/post/102jsmj/ftc-finds-website-overlay-tool-failed-to-deliver-accessibility-promises
- https://grandriversolutions.com/ftc-1-million-dollar-settlement-case/
- https://www.complyloft.com/accessibility/eaa/enforcement
- https://statutus.ch/en/guides/european-accessibility-act-enforcement-so-far/
- https://libration.io/en/resources/eaa-fines-enforcement/
- https://li.solutions/blog/eaa-enforcement-2026/
- https://atyantik.com/blog/european-accessibility-act-enforcement/
- https://www.xictron.com/en/blog/accessibility-act-exemptions-microenterprises-2026/
- https://dev.to/lawebe/the-european-accessibility-act-eaa-what-online-stores-must-do-1eh5
- https://www.fudge.ai/blog/european-accessibility-act-shopify/
- https://www.heuking.de/de/news-events/newsletter-fachbeitraege/artikel/das-barrierefreiheitsstaerkungsgesetz-bfsg-teil-2-die-ersten-bfsg-abmahnungen-im-e-commerce.html
- https://www.pragma-code.de/blog-abmahnwelle-barrierefreiheit-2026
- https://www.xictron.com/de/blog/bfsg-abmahnwelle-2026-barrierefreiheit-durchsetzen/
- https://www.haendlerbund.de/de/news/aktuelles/gratis-bfsg-check
- https://mirelaprifti.gumroad.com/l/website-accessibility-statement
- https://www.iubenda.com/en/blog/european-accessibility-act-eaa-accessibility-statement-guide-template-2/
- https://getwcag.com/en/accessibility-statement
- https://github.com/creativedeals/free-claude-skill-accessibility-audit

Privacy / consumer protection
- https://trustarc.com/resource/new-in-2026-state-privacy-laws-in-indiana-kentucky-and-rhode-island/
- https://msba.org/site/content/News-and-Publications/News/General-News/Maryland_Online_Data_Privacy_Act.aspx
- https://www.hunton.com/privacy-and-cybersecurity-law-blog/newly-approved-ccpa-regulations-have-staggered-deadlines-for-compliance
- https://www.thompsoncoburn.com/insights/californias-2026-ccpa-regulations-summary-and-preparation-guide/
- https://www.davispolk.com/insights/client-update/ftc-prioritizes-coppa-enforcement-new-compliance-obligations-take-effect
- https://www.hunton.com/privacy-and-cybersecurity-law-blog/coppa-rule-amendment-compliance-deadline-approaches
- https://measuremindsgroup.com/is-consent-mode-v2-mandatory
- https://www.consentbit.com/blog/do-you-need-a-google-certified-cmp-what-googles-requirement-actually-means
- https://euinternetpolicy.wordpress.com/2026/10/23/the-councils-digital-omnibus-mandate-what-it-would-change-in-the-gdpr/
- https://acompli.ie/news/digital-omnibus-gdpr-cookies-status-september-2026/
- https://www.mishcon.com/news/is-your-data-protection-complaints-process-ready-for-19-june-2026
- https://www.mayerbrown.com/en/insights/publications/2026/02/preparing-for-the-data-use-and-access-act-2025-upcoming-complaints-procedure-requirement
- https://www.privacyworld.blog/2026/06/the-data-use-and-access-act-2025-and-the-new-right-for-individuals-to-complain-to-controllers-what-organisations-need-to-do-before-19-june-2026/
- https://ico.org.uk/about-the-ico/media-centre/news-and-blogs/2026/05/one-month-to-go-what-businesses-need-to-know-to-meet-new-data-law
- https://www.arnoldporter.com/en/perspectives/advisories/2026/02/ico-publishes-guidance-on-how-to-deal-with-data-protection-complaints
- https://complaintsdesk.pages.dev/duaa-complaints-procedure
- https://www.iubenda.com/en/blog/uks-six-step-guide-on-handling-data-protection-complaints/
- https://sprintlaw.co.uk/articles/handling-ico-complaints-a-stepbystep-business-guide/
- https://sprintlaw.com.au/articles/automated-decision-making-privacy-rules/
- https://colemangreig.com.au/insights/privacy-reform-in-australia-what-businesses-need-to-know-in-2026-2027/
- https://www.beneschlaw.com/insight/five-stars-zero-tolerance-ftc-turns-up-enforcement-under-consumer-review-rule/
- https://www.regulatoryoversight.com/2026/01/ftc-warns-companies-over-deceptive-online-review-practices/
- https://www.insideprivacy.com/united-states/federal-trade-commission/ftc-issues-warning-letters-for-violations-of-consumer-reviews-rule/
- https://www.cooley.com/news/insight/2025/2025-07-11-click-to-cancel-just-got-cancelled-eighth-circuit-vacates-entirety-of-ftcs-negative-option-rule
- https://www.jonesday.com/en/insights/2026/05/ftc-revives-clicktocancel-rule-new-risks-for-subscription-businesses
- https://www.gibsondunn.com/ftc-restarts-negative-option-rulemaking-after-eighth-circuit-vacatur-enforcement-under-rosca-continues/
- https://www.crowell.com/en/insights/client-alerts/clicking-all-the-right-boxes-ftc-moves-to-revive-click-to-cancel-rule-following-eighth-circuit-vacatur
- https://advertisinglaw.fkks.com/post/102jkbj/california-amends-its-auto-renewal-law-effective-july-1-2025
- https://www.venable.com/insights/publications/2025/07/july-1-and-july-14-autorenewal-and-negative-opt
- https://hudsoncook.com/article/keeping-your-eye-on-the-ball-federal-cancellation-policy-settlements-and-new-york-updates-to-auto-renewal-law/
- https://www.mondaq.com/unitedstates/consumer-law/1769282/that-free-trial-might-cost-you-automatic-renewal-litigation-on-the-rise-in-ca
- https://www.ftc.gov/news-events/news/press-releases/2026/05/ftc-begins-enforcing-take-it-down-act
- https://wilmerhale.com/en/insights/client-alerts/20260615-the-take-it-down-act-goes-live
- https://www.wiley.law/alert-May-19-Deadline-for-TAKE-IT-DOWN-Act-Compliance-Is-Your-Company-Prepared
- https://www.legaldata.law/en/insights/ai-makes-up-facts-and-the-company-pays-this-ruling-is-a-warning-to-every-chatbot-operator
- https://www.innobu.com/en/articles/ai-liability-chatbot-companies-2026.html

Email / SMS
- https://www.gmass.co/blog/gmail-bulk-sender-guidelines/
- https://redsift.com/resources/blog/gmails-enforcement-ramps-up-what-bulk-senders-need-to-know
- https://www.valimail.com/blog/google-email-compliance-enforcement/
- https://support.microsoft.com/outlook/fix-ndr-error-550-5-7-515-in-outlook-com
- https://techcommunity.microsoft.com/blog/microsoftdefenderforoffice365blog/strengthening-email-ecosystem-outlook%E2%80%99s-new-requirements-for-high%E2%80%90volume-senders/4399730/replies/4418393
- https://www.twilio.com/en-us/changelog/a2p-10dlc-campaign-registration-will-require-privacy-policy-and-
- https://www.twilio.com/docs/api/errors/30933
- https://live.docs.dev.twilio.com/docs/api/errors/30908.md
- https://static0.twilio.com/docs/api/errors/30932
- https://static1.twilio.com/docs/api/errors/30920
- https://static1.twilio.com/en-us/changelog/new-error-codes-provide-clearer-tfv-and-a2p-10dlc-registration-f
- https://conduit.ai/blog/a2p-10dlc-registration-step-by-step-for-2026
- https://textbolt.com/blog/10dlc-compliance/
- https://getterms.io/blog/what-is-a2p-10dlc
- https://community.zoom.com/t5/Zoom-Phone-System/10DLC-Registration-failed-over-and-over/m-p/191089
- https://community.zoom.com/t5/Zoom-Phone-System/10DLC-SMS-Campaign-Rejected-due-to-Brand-name-not-consistent/m-p/218393
- https://community.sinch.com/t5/10DLC/Why-was-my-10DLC-campaign-rejected/m-p/15408
- https://fiverr.com/ghl_expert_atif/create-gohighlevel-workflows-email-automations-and-crm-triggers
- https://autogencrm.com/?p=16408
- https://www.burr.com/telephone-consumer-protection-act/the-fcc-delays-effective-date-of-tcpa-revoke-all-rule-until-january-31-2027
- https://mslawgroup.com/delayed-again-fcc-pushes-back-tcpas-revoke-all-rule-to-january-31-2027/
- https://www.cullenllp.com/blog/fcc-substantially-revises-tcpa-consent-revocation-rules-set-to-take-effect-january-2027/
- https://www.troutman.com/insights/fcc-revises-tcpa-revocation-of-consent-rules-that-were-set-to-go-into-effect-in-january/

Tax / e-invoicing
- https://www.gov.uk/guidance/choose-the-right-software-for-making-tax-digital-for-income-tax?
- https://www.gov.uk/government/publications/extension-of-making-tax-digital-for-income-tax-self-assessment-to-sole-traders-and-landlords/making-tax-digital-for-income-tax-self-assessment-for-sole-traders-and-landlords
- https://www.icas.com/news-insights-events/news/tax/further-updates-to-making-tax-digital-for-income-tax-self-assessment-announced
- https://www.payslipchecker.uk/blog/making-tax-digital-self-employed-guide
- https://www.theregister.com/2026/04/10/mtd_hmrc/
- https://www.pulse.bot/finance/news/fewer-than-3-in-10-register-for-hmrcs-making-tax-digital-shake-up-b534009f-ba1a-45e1-b494-31174b5ace84/
- https://sterlingandwells.com/news/sole-traders-landlords-filed-under-mtd/
- https://moneyweek.com/economy/small-business/what-you-need-to-know-about-making-tax-digital
- https://www.property118.com/landlords-urged-to-prepare-for-making-tax-digital-2027/
- https://www.getcoconut.com/knowledge-hub/bridging-software-for-online-marketplaces-and-mtd
- https://zmartly.co.uk/news-insights/mtd-software-for-landlords-bridging-software
- https://www.etsy.com/listing/4567179604/
- https://www.etsy.com/listing/4567155739/
- https://www.etsy.com/listing/4567156121/
- https://payhip.com/b/9ZbAV
- https://123sheets.com/landlords.aspx
- https://workspace.google.com/marketplace/app/abridge/251470994062
- https://apps.apple.com/gb/app/id6752574003
- https://www.nrla.org.uk/services/tax/taxd/bridging-template
- https://entreprendre.service-public.gouv.fr/actualites/A15683?lang=en
- https://hayot-expertise.fr/blog/facturation-electronique-2026-obligation-reception-1er-septembre
- https://abby.fr/guide/facturation-electronique/facture-electronique-septembre-2026
- https://invoicedataextraction.com/blog/france-e-invoicing-mandate-2026
- https://sovos.com/regulatory-updates/vat/poland-ministry-of-finance-extends-ksef-penalty-relief-until-end-of-2027/
- https://kpmg.com/pl/en/insights/taxes/tax-alert-extension-of-the-deferral-of-penalties-for-errors-in-using-ksef-until-the-end-of-2027.html
- https://www.vatcalc.com/belgium/belgium-b2b-e-invoicing-july-2024-update/
- https://www.truecommerce.com/blog/e-invoicing-in-belgium-your-guide-to-the-2026-mandate/
- https://www.enterpryze.com/post/peppol-e-invoicing-mandates-2026-eu-sme-guide
- https://cpapracticeadvisor.com/2025/07/30/one-big-beautiful-bill-act-changes-1099-thresholds/165863/
- https://www.patriotsoftware.com/blog/accounting/1099-reporting-threshold/
- https://www.irs.gov/pub/opr-taxpros/issue-number-2026-22-how-to-be-a-careful-wisper.pdf
- https://www.cpapracticeadvisor.com/2026/10/02/what-the-ftc-safeguards-rule-actually-requires-from-tax-and-accounting-firms/

Security / other EU
- https://blog.pcisecuritystandards.org/faq-clarifies-new-saq-a-eligibility-criteria-for-e-commerce-merchants
- https://www.hipaajournal.com/ocr-gives-update-on-proposed-hipaa-security-rule/
- https://www.pact-one.com/2026/09/hipaa-security-rule-2026-status/
- https://digital-strategy.ec.europa.eu/en/policies/cra-reporting
- https://www.jonesday.com/en/insights/2026/07/eu-cyber-resilience-act-24hour-reporting-duties-start-september-11-2026
- https://www.reedsmith.com/articles/germany-implements-nis2-immediate-effect-broad-scope-near-term-registration/
- https://www.jdsupra.com/legalnews/new-cybersecurity-regulations-in-2713282/
- https://www.littler.com/news-analysis/asap/eleventh-hour-implementation-status-eu-pay-transparency-directive
- https://www.lewissilkin.com/insights/2026/07/01/eu-pay-transparency-directive-2026-employer-compliance
- https://www.crowe.com/uk/insights/eu-pay-transparency-directive
- https://craftybase.com/blog/what-is-gpsr
- https://www.24hour-ar.com/the-hidden-risks-of-non-compliance-with-gpsr-on-amazon-etsy-ebay
- https://stallscore.pages.dev/learn/etsy-gpsr

Education
- https://kjk.com/2026/06/12/ohios-july-1-2026-school-ai-policy-deadline-what-districts-educators-and-parents-need-to-know/
- https://education.ohio.gov/Media/Media-Releases/2025-Media-Releases/Ohio-Department-of-Education-and-Workforce-Release
- https://www.yahoo.com/news/politics/articles/4-more-states-require-districts-050000407.html
- https://www.truemadeai.com/resources/state-k12-ai-laws-and-guidance
- https://www.aiforeducation.io/ai-resources/state-ai-guidance
- https://www.edtechinnovationhub.com/news/dfe-publishes-kcsie-2026-with-mobile-phone-free-default-and-ai-safeguarding-rules
- https://www.gov.uk/government/publications/generative-artificial-intelligence-in-education
- https://www.theeducatoronline.com.au/k12/news/ai-framework-for-schools-released/283752
- https://www.presidency.ucsb.edu/documents/executive-order-14277-advancing-artificial-intelligence-education-for-american-youth
- https://www.tes.com/en-nz/teaching-resource/artificial-intelligence-ai-policy-template-13133971
- https://thirdspacelearning.com/blog/ai-policy-for-schools/
- https://www.kuraplan.com/uk/ai-policy?year=1

Platforms / AI search / marketplaces
- https://thenextweb.com/news/google-ai-overviews-publisher-links-search-traffic
- https://www.seo-kreativ.de/en/blog/google-ai-overviews-updates-2026-en/
- https://www.searchenginejournal.com/impact-of-ai-overviews-how-publishers-need-to-adapt/556843/
- https://searchengineland.com/google-zero-click-searches-2026-study-479717
- https://www.omnibound.ai/blog/google-ai-overviews-statistics
- https://ppc.land/google-quietly-kills-q-a-for-an-ai-button-most-wont-use/
- https://ppc.land/google-business-profile-is-now-a-data-layer-that-feeds-ai-maps-and-search/
- https://thevalleymarketinggroup.com/blog/google-business-profile-qa-removed-ask-maps-2026/
- https://www.bccinteractive.com/blog/local-ai-search-statistics/
- https://seosandwitch.com/chatgpt-local-business-statistics/
- https://richdevtools.com/articles/web/llms-txt-evidence-2026
- https://www.1clickreport.com/blog/llms-txt-evidence-2026
- https://limy.ai/blog/llms-txt-in-2026-the-full-guide
- https://genxops.gumroad.com/l/geo_for_smbs
- https://aeo-starter-kit.pages.dev/
- https://payhip.com/b/YzjDQ
- https://www.framer.com/marketplace/templates/aeo-geo-seo/?via=doug
- https://www.promptlesspress.com/blog-etsy-ai-policy-2026-digital-products
- https://ngini.com/en-us/blog/etsy-ai-disclosure-policy-2026-explained
- https://www.inkfluenceai.com/blog/etsy-ai-disclosure-explained-2026
- https://www.inkfluenceai.com/blog/etsy-ai-rules-update-october-2026
- https://www.prcreativedigital.com/blog/etsy-ai-disclosure-policy-2026-shoppers.html
- https://atlan.com/know/ai-agent/ai-agent-skills/what-are-agent-skills/
- https://laurentkempe.com/2026/01/27/Agent-Skills-From-Claude-to-Open-Standard/
- https://www.agensi.io/learn/agent-skills-marketplace-sell-your-skills
- https://skillhq.dev/become-seller
- https://kissmyskills.com/pages/sell-your-skills
- https://inflectual.gumroad.com/l/master-marketing-claude-skills-bundle
- https://github.com/mukul975/Privacy-Data-Protection-Skills
- https://venturebeat.com/technology/openai-now-accepting-chatgpt-app-submissions-from-third-party-devs-launches
- https://community.openai.com/t/chatgpt-app-monetization-apps-sdk/1372343
- https://x.com/OpenAI/status/1972708279043367238
- https://stripe.com/newsroom/news/stripe-openai-instant-checkout
- https://www.hypotenuse.ai/blog/chatgpts-instant-checkout-the-next-phase-of-agentic-commerce
- https://developer.chrome.com/docs/extensions/develop/migrate/mv2-deprecation-timeline
- https://www.wearefounders.uk/gumroad-fees-2026-what-sellers-actually-pay-per-sale/
- https://fungies.io/whop-vs-gumroad-vs-lemon-squeezy-2026
- https://digiday.com/marketing/as-health-and-wellness-brands-brace-for-ad-restrictions-on-meta-marketers-and-advertisers-seek-more-transparency/
- https://searchengineland.com/google-clarifies-policy-on-false-information-in-advertiser-verification-464395

Tool-derived (not web pages): npm registry search API (registry.npmjs.org/-/v1/search) for "10dlc", "eu ai act", "accessibility statement", "making tax digital", "llms.txt"; GitHub repository search via `gh api search/repositories` for 2026-created repos matching "eu ai act compliance" (1,125), "european accessibility act" (31), "10dlc" since Jun 2025 (154), "making tax digital" (33), "llms.txt generator" (164) and "ai receptionist" (3,426).
