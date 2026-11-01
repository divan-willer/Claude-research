# Phase 3 validation: batch 3 (C11-C15)

Validator #3. Date: 2026-11-01. Rubric and verdict bands are from the shared validator brief. Scores were set with a skeptical default: missing evidence lowered a score and never raised it.

## Score table

| id | name | demand | competition (5 = low) | wtp | buildability | distribution | growth | total | verdict |
|---|---|---|---|---|---|---|---|---|---|
| C11 | "Get found by AI" kit for local service businesses | 2 | 1 | 2 | 4 | 3 | 3 | 15 | WEAK |
| C12 | FTC-compliant review-request kit | 3 | 2 | 2 | 5 | 4 | 3 | 19 | VIABLE |
| C13 | Agentic-commerce readiness checklist (Shopify/Etsy) | 3 | 2 | 2 | 4 | 2 | 2 | 15 | WEAK |
| C14 | Etsy digital-seller compliance kit | 3 | 2 | 2 | 5 | 3 | 4 | 19 | VIABLE |
| C15 | Vibe-coder launch safety kit | 3 | 1 | 2 | 4 | 3 | 2 | 15 | REJECT (fatal kill reason) |

**Cross-cutting finding for the lead (affects every batch): Etsy's 22 Oct 2026 AI-policy update is a channel risk for any Claude-written guide.**
- Etsy's own Seller Handbook and help pages now say:
  - AI use must be disclosed in the listing.
  - AI prompt bundles are prohibited.
  - Mass-automated listing generation is prohibited.
  - AI-generated functional guides (patterns, recipes, instructions) are no longer allowed.

  Sources: [Etsy Seller Handbook, "Important updates to AI use on Etsy"](https://www.etsy.com/seller-handbook/article/1522733284810), [Etsy Creativity Standards](https://www.etsy.com/legal/creativity), and press coverage ([Digital Commerce 360, 26 Oct 2026](https://www.digitalcommerce360.com/2026/10/26/etsy-ai-policy/amp/), [Value Added Resource](https://www.valueaddedresource.net/etsy-bans-ai-patterns/), [Retail Dive](https://retaildive.com/news/etsy-updates-ai-use-policies-emphasize-craftsmanship/833838)).
- What it means: any "how-to" kit listed on Etsy must be visibly human-authored and must disclose AI assistance. Templates and spreadsheets are lower risk than instruction guides.
- I am relying on the search tool's summary of those pages (WebFetch is blocked), so I could not read the exact wording of the functional-guide clause. Treat it as **high-confidence direction, unverified exact wording.**

---

## C11. "Get found by AI" kit for local service businesses (seed 2, re-scoped): 15, WEAK

**Rationale:** The traffic shift is real, but this is one of the most crowded corners of the 2026 info-product market.
- **Paid competition:**
  - Etsy already has GEO and "get found by AI" guides from about $1 to $30, many heavily discounted.
  - Gumroad has playbooks, dashboards and agency kits.
- **Free competition:**
  - At least six free AI-visibility checkers, including BrightLocal's location-level one.
  - A 25k-star free Claude SEO/GEO skill.
  - Anthropic's own free small-business plugin, which ships an `seo-ai-visibility` skill.
- **Buyer demand:** I found no thread of a local owner asking for this. The results were almost entirely agency and vendor blogs.

**Best-scoped version:** Don't sell this standalone. Fold it into C12 as a bonus module: "Get recommended on Google Maps & ChatGPT: reviews + profile checklist for [one trade]". That means a GBP attribute checklist, NAP-consistency sheet, LocalBusiness JSON-LD snippet and a monthly "ask the AI" self-test sheet. No llms.txt and no ranking promises.

**Target buyer:** owner-operator of a 1-10-person HVAC, plumbing or electrical company who does their own Google Business Profile. A secondary buyer is the freelancer who manages a few such profiles.

**Demand evidence:**
- Consumer-side shift, a survey relayed in Phase 1: BrightLocal 2026 found 45% of US consumers used gen-AI for local recommendations ([bccinteractive](https://www.bccinteractive.com/blog/local-ai-search-statistics/), [seosandwitch](https://seosandwitch.com/chatgpt-local-business-statistics/)). This shows consumer behaviour, not owners wanting a kit.
- One Reddit mirror post (25 Apr 2026) notes that most small businesses checked were invisible in ChatGPT ([1stc10m](https://reddit.sentinel-team.org/posts/1stc10m/snapshots/2026-04-25T00%3A47%3A11.009274Z)). The author is probably a marketer, not a buyer.
- The search for "how do I get my business recommended by ChatGPT" returned **only** agency/vendor blogs and no r/smallbusiness threads, e.g. [humblehelp.studio](https://www.humblehelp.studio/blog/chatgpt-wont-recommend-your-business-fix), [frostbitemarketing](https://frostbitemarketing.com/?p=104060), [webzum](https://webzum.com/blog/how-to-get-recommended-by-chatgpt). Per the rubric, vendor blogs only count for 1-2.

**Competition snapshot:**
- **Paid, Etsy:**
  - Etsy has market pages for [chatgpt_seo](https://www.etsy.com/market/chatgpt_seo), [local_seo](https://www.etsy.com/market/local_seo) and [google_business_profile](https://www.etsy.com/market/google_business_profile).
  - Listings include an "AI SEO/GEO Course for Small Business, Get Found in AI Search, Local SEO/GEO Guide and Workbook", a 50+ page GEO/AEO checklist, a ~$15.99 Local SEO Workbook and a ~$5 "Get Found by ChatGPT + Claude" prompt pack.
  - Prices run ~$1-$30 and are often discounted.
  - Review and sales counts were not visible in search results.
- **Paid, Gumroad:**
  - [GEO Playbook, 167 tactics](https://tanguykeyzer.gumroad.com/l/ssjwve)
  - [GEO Performance Dashboard](https://datmark.gumroad.com/l/ai-traffic-dashboard)
  - [AI Agency Launch Kit](https://modernwebseo.gumroad.com/l/ai-agency-launch-kit) (11 geo-* skills plus a LocalBusiness JSON-LD template)
  - [AI GEO/AEO/SEO OS](https://growthwithalex.gumroad.com/l/aisearchagent)
  - Relayed from Phase 1: a $19 [genxops GEO kit](https://genxops.gumroad.com/l/geo_for_smbs), the €39 [AEO Starter Kit](https://aeo-starter-kit.pages.dev/) and a £39 [Payhip AEO audit](https://payhip.com/b/YzjDQ).
  - Phase 1 found **no GEO kit among rated titles** in two Gumroad crawls.
- **Free checkers:**
  - [BrightLocal Local AI Visibility Checker](https://www.brightlocal.com/free-local-seo-tools/local-ai-visibility-checker/) (location-level, Google AI Mode plus ChatGPT)
  - [Birdeye AI Visibility Checker](https://birdeye.com/ai-visibility-checker/)
  - [Insites free AI visibility audit](https://insites.com/resources/free-ai-visibility-audit/)
  - [Zarla](https://www.zarla.com/whats-new/2026-08-24-see-what-ai-assistants-say-about-your-business) (24 Aug 2026)
  - Relayed: [HubSpot AI Search Grader](https://www.hubspot.com/ai-search-grader) and [Ahrefs AI Visibility Checker](https://ahrefs.com/ai-visibility-checker)
- **Free Google tooling:** GSC generative-AI reports ([Google, Jun 2026](https://developers.google.com/search/blog/2026/06/gen-ai-performance-reports)) and Bing AI Performance ([Bing, Feb 2026](https://blogs.bing.com/webmaster/February-2026/Introducing-AI-Performance-in-Bing-Webmaster-Tools-Public-Preview)), with official docs.
- **Free skills and repos (GitHub search API, 1 Nov 2026):**
  - AgriciDaniel/claude-seo: 25,479 stars
  - Ryze-AI-Adgent/open-seo-mcp-skills: 8,538 stars
  - onvoyage-ai/gtm-engineer-skills: 1,345 stars
  - Auriti-Labs/geo-optimizer-skill: 1,255 stars
  - leopard627/fire-your-seo-agency: 987 stars
  - At least 5 free LocalBusiness JSON-LD generators created Jul-Oct 2026 (e.g. ahmettasdemirusa/local-business-schema-generator)
  - Local-SEO/GBP Claude skills (milad-ahmd/google-business-profile-manager, ahmettasdemirusa/local-seo-skills)
- **Free official plugin:** Anthropic's small-business plugin includes a `seo-ai-visibility` skill (Phase 1, trend-scout #2).

**Kill reasons found:**
1. Free graders plus a free official Anthropic skill cover "check and fix my AI visibility".
2. Etsy/Gumroad price anchors sit at $1-$19 with no visible ratings.
3. Results are unprovable: AI answers vary between runs, with 29% overlap between identical queries, relayed from [seosandwitch](https://seosandwitch.com/chatgpt-local-business-statistics/).
4. Etsy's Oct 2026 ban on AI-generated instructional guides puts a Claude-written playbook at risk on Etsy.

Not fatal on its own: no single free tool gives a non-technical plumber a plain-English, trade-specific to-do list. But nothing here shows owners will pay for that.

**Price recommendation:** $15-19 as a standalone. Better as a bonus inside C12 to justify $19-29.

**Launch channels:**
- **Etsy.** Market pages exist for local_seo, chatgpt_seo and google_business_profile, so there is buyer search traffic. Rules: AI use must be disclosed, and AI-generated functional guides and prompt bundles are prohibited ([Etsy Seller Handbook](https://www.etsy.com/seller-handbook/article/1522733284810)).
- **r/smallbusiness.** Self-promotion is limited to a weekly "Promote your business" thread, and the subreddit is Q&A, per mirror copies of 2024 promo threads ([Mar 2024](https://lr.in.psf.lt/r/smallbusiness/comments/1bn1bpy/promote_your_business_week_of_march_25_2024), [Apr 2024](https://lr.in.psf.lt/r/smallbusiness/comments/1cfnz3o/promote_your_business_week_of_april_29_2024)). The current sidebar is NOT VERIFIED.
- **Trade-owner Facebook groups and r/HVAC:** NOT VERIFIED.

**Biggest risk:** nobody pays for a guide when free graders and free AI give the same advice. **Cheapest test:** fold it into C12 and see whether the bundle sells. If it must stand alone, list a $15 Etsy version for one trade and kill it if it gets fewer than about 150 views and no sale in 14 days.

**Build notes:**
- Deliverables: PDF playbook, Google Sheets checklist, single-file HTML JSON-LD generator, and a GSC/Bing AI-report walkthrough.
- The walkthrough needs screenshots from a property that actually shows AI impressions. The founder may not have one, which is hard to fit into a day.
- The guide must be human-edited and carry an AI disclosure on Etsy.

---

## C12. FTC-compliant review-request kit: 19, VIABLE

**Rationale:** This is the only product in the batch that rides existing Etsy buyer search. Etsy has market pages for [google_review_card_templates](https://www.etsy.com/market/google_review_card_templates), [review_request](https://www.etsy.com/market/review_request), [request_review_card](https://www.etsy.com/market/request_review_card) and [google_review_printable](https://www.etsy.com/market/google_review_printable).
- **Against it:**
  - That card category is a commodity at about $1-$6.
  - Google itself now gives every business a free review link and QR code, with policy text ([Google help 16816815](https://support.google.com/business/answer/16816815?hl=en)).
- **The opening:** the compliant scripts and policy layer. That covers:
  - SMS and email wording that asks every customer, with no gating
  - no incentives
  - a staff-review disclosure rule
  - "don't pressure in-store"

  Etsy and Gumroad results surfaced none of that as a standalone product.
- **Limits:** this is a modest, low-ticket product. It is not a breakout.

**Best-scoped version:** "Google Review Kit for [HVAC/plumbing], FTC- and Google-policy-safe". It includes:
- 6 editable Canva cards (QR from Google's own link)
- 10 SMS/email request scripts by job stage
- a 2-step follow-up cadence
- a staff/family review disclosure policy
- a "never do" checklist (gating, incentives, review stations/iPads in store)
- 20 review-response templates
- C11's GBP/AI checklist as a bonus

**Target buyer:** owner or office manager of a local service business (trades, clinics, salons) who is already searching Etsy for "Google review card".

**Demand evidence:**
- Three Reddit mirror threads (Mar-May 2026, Phase 1 PH#26) on reviews being hard to get and real reviews being removed: [1rq57dr](https://reddit.sentinel-team.org/posts/1rq57dr/snapshots/2026-03-11T01%3A23%3A07.053576Z), [1sz8u0r](https://reddit.sentinel-team.org/posts/1sz8u0r/snapshots/2026-05-02T04%3A50%3A06.954017Z), [1tn81br](https://reddit.sentinel-team.org/posts/1tn81br/snapshots/2026-05-26T09%3A47%3A52.470198Z).
- Etsy has 4+ market pages for review-request cards, which means buyer search demand exists.
- There is confusion about the rules: sources disagree on whether the FTC bans incentives ([fitsmallbusiness](https://fitsmallbusiness.com/marketing/ask-for-google-reviews/), [shiftflow](https://www.shiftflow.app/playbook/can-i-offer-discount-or-gift-card-for-review), [clovvy](https://clovvy.pages.dev/google-review-guidelines/), [whito.co.uk on in-store iPads](https://whito.co.uk/news/the-ipad-on-your-counter-is-now-breaking-googles-review-rules/), [beancount FTC guide, 16 Jul 2026](https://beancount.io/blog/2026/07/16/ftc-fake-reviews-crackdown-consumer-review-rule-guide)). That confusion is the hook.
- Enforcement, relayed from Phase 1 REG#5: FTC warning letters on 22 Dec 2025 and a DOJ/Illinois AG suit in May 2026 ([Benesch](https://www.beneschlaw.com/insight/five-stars-zero-tolerance-ftc-turns-up-enforcement-under-consumer-review-rule/)).

**Competition snapshot:**
- **Paid, Etsy:** many editable Canva review cards at ~$1-$6, e.g. listings [4480710918](https://www.etsy.com/listing/4480710918/google-review-card-template-editable-qr), [1727191495](https://www.etsy.com/listing/1727191495/google-review-canva-template-leave-us-a), [1588306343](https://www.etsy.com/listing/1588306343/google-square-review-card-template), [1754614558](https://www.etsy.com/listing/1754614558/google-review-sign-review-card-template). Sales counts were not visible.
- **Paid, Gumroad:**
  - [Google Review Card](https://enlightprints.gumroad.com/l/Greview)
  - [LocalRankAI](https://promarketing10.gumroad.com/l/LocalRankAI), which includes a bonus "SMS Review Request Template Kit"
  - [Automated Google Reviews blueprint](https://automatewithbishal.gumroad.com/l/AutomatedGoogleReviews)
  - [AI GBP review response system](https://hashirmalick.gumroad.com/l/aireplygooglemybusiness)
  - No ratings were visible.
- **Free alternatives:**
  - Google's native review link and QR ([16816815](https://support.google.com/business/answer/16816815?hl=en), [16334724](https://support.google.com/business/answer/16334724?hl=en-GB)) and "Tips to get more reviews" ([3474122](https://support.google.com/business/answer/3474122?hl=en-GH))
  - Vendor blogs from review SaaS (AskNicely, GatherUp, Famewall)
  - Free card makers in Canva

**Kill reasons found:**
- The card layer is a $1-$6 commodity, and Google gives away the QR.
- The scripts are freely written up by review-SaaS blogs.

No fatal reason: nothing free bundles trade-specific scripts, a compliance checklist and printable cards. **Legal-risk note:** sell as "templates aligned with Google policy and the FTC rule (16 CFR 465), not legal advice". Never claim "makes you compliant" (see the FTC v. accessiBe precedent noted in Phase 1).

**Price recommendation:** $12-19 on Etsy (the cards anchor low, so the bundle must look clearly bigger). A $29 "3-trade agency pack" upsell on Gumroad.

**Launch channels:**
- **Etsy.** There is search traffic on the review-card market pages. Rules: AI use must be disclosed. Templates are a lower-risk format than AI-written guides ([Etsy Seller Handbook](https://www.etsy.com/seller-handbook/article/1522733284810)).
- **r/smallbusiness weekly promo thread only.** Rules per the 2024 mirror threads above; current sidebar NOT VERIFIED.
- **Gumroad** for the agency pack: no buyer traffic verified.

**Biggest risk:** buyers anchored at $3 cards won't pay $15 for scripts and policy. **Cheapest test:** list on Etsy with the cards as the hero image and "FTC & Google-safe scripts included" in the title. Kill it if there is no sale within 21 days or 300 views. Optionally add $1/day Etsy Ads.

**Build notes:** 4-5 hours.
- Canva templates: free Canva account, delivered as share-template links in a PDF.
- Scripts and policy in Google Docs/PDF, response templates in Sheets.
- No QR generator needed: point buyers to Google's native QR. This removes a build item that adds no value.
- Write the scripts by hand-editing, so Etsy doesn't treat the kit as an AI-generated guide.

---

## C13. Agentic-commerce readiness checklist for Shopify/Etsy sellers: 15, WEAK

**Rationale:** The platforms do the plumbing for free.
- **Shopify:** "Agentic Storefronts" is on by default for eligible stores. Products reach ChatGPT, Copilot, Google AI Mode and Gemini through Shopify Catalog "with no separate integrations, no apps" ([Shopify Help](https://help.shopify.com/en/manual/online-sales-channels/agentic-storefronts), [Shopify news](https://www.shopify.com/news/agentic-commerce-momentum)).
- **Etsy:** it integrates with Google at platform level ([Etsy news](https://www.etsy.com/news/etsy-partners-with-google-on-ai-powered-shopping), Phase 1).
- **What's left:** product-data quality (titles, attributes, Merchant Center feed, reviews). That is ordinary listing SEO, already covered by free vendor guides and free GitHub audit skills.
- **Demand:** real Shopify-community confusion exists, but no Etsy-seller demand surfaced.

**Best-scoped version:** a Shopify-only "Why aren't my products showing in ChatGPT/AI Mode?" diagnostic. It would cover:
- an eligibility check
- Catalog and Merchant Center feed errors
- a title/attribute rewrite sheet
- a policy/returns page checklist

Price it as a $15-19 Google Sheet. Drop Etsy, since Etsy sellers have no lever beyond the listing itself.

**Target buyer:** a small US Shopify merchant (under $500k GMV) who noticed AI-chat traffic or heard about Agentic Storefronts and can't tell whether their products appear.

**Demand evidence:**
- Shopify Community threads:
  - [ChatGPT & Copilot Agentic Shopping: Is It Live for All Shopify Stores?](https://community.shopify.com/t/chatgpt-copilot-agentic-shopping-is-it-live-for-all-shopify-stores/585319)
  - [ChatGPT is becoming a sales channel](https://community.shopify.com/t/chatgpt-is-becoming-a-sales-channel/591794)
  - [Agentic Shopping Q&A: What Every Shopify Store Needs to Know](https://community.shopify.com/t/agentic-shopping-q-a-what-every-shopify-store-needs-to-know-right-now/599243)
  - Dates were not shown. The topic IDs suggest 2026.
- Vendor posts on "products not showing" ([paz.ai](https://www.paz.ai/blog/shopify-agentic-storefronts-chatgpt-products-not-showing)).
- Two Reddit mirror snapshots (18 Feb 2026 [1r7c9fd](https://reddit.sentinel-team.org/posts/1r7c9fd/snapshots/2026-02-18T03%3A43%3A29.412351Z), 27 Mar 2026 [1s4zdbz](https://reddit.sentinel-team.org/posts/1s4zdbz/snapshots/2026-03-27T21%3A08%3A12.710659Z)). The search tool described them as low-substance.
- No Etsy-seller demand was found.

**Competition snapshot:**
- **Free official:** Shopify Help and blog ([how agentic commerce works](https://www.shopify.com/blog/how-agentic-commerce-works)), [Google UCP merchant docs](https://developers.google.com/merchant/ucp).
- **Free vendor guides:**
  - [ecommercefastlane readiness guide](https://ecommercefastlane.com/shopify-agentic-commerce-readiness-guide/)
  - [storerank.ai complete guide](https://www.storerank.ai/shopify-agentic-commerce-the-complete-guide-for-2026/)
  - [askphill](https://askphill.com/blogs/blog/agentic-commerce-for-shopify-protocols-platforms-and-what-to-prioritize-in-2026)
  - [shugert product-data guide](https://shugert.com.mx/resources/shopify-agentic-storefronts-product-data)
- **Free repos (GitHub search, 16 results):** monkydot/ucp-ready, zhao-hanbo/agentic-commerce-kit (a Claude Code readiness-audit skill), hongruzoe/shopify-geo-product-auditor, nick-liyao/agentic-commerce-kit.
- **Paid:** SaaS such as Paz.ai and StoreRank (prices not checked). I spent no search on Gumroad/Etsy paid checklists, so paid-kit count is UNKNOWN.

**Kill reasons found:**
- Platform-native default-on discovery (Shopify), with Etsy integrating at platform level.
- The remaining work is generic product-SEO with abundant free guides.
- The ground keeps moving: ChatGPT Instant Checkout was reportedly retired in Mar 2026 (Phase 1, conflicting reports), and checkout differs by channel.

Not quite fatal, because "why am I not showing" is a real diagnostic question, but close.

**Price recommendation:** $15-19.

**Launch channels:**
- **Shopify Community forums:** promotion rules NOT VERIFIED.
- **r/shopify:** rules NOT VERIFIED.
- **Gumroad:** no buyer traffic verified.
- **Etsy:** the wrong channel for Shopify merchants.

**Biggest risk:** Shopify/Google ship a native "AI visibility" diagnostic in the admin, and sellers simply wait. **Cheapest test:** answer 5 Shopify Community "not showing in ChatGPT" questions with genuine help. If people ask follow-ups or DM, list a $15 Sheet on Gumroad. Otherwise drop it.

**Build notes:**
- A Sheets checklist plus PDF is easy.
- Accuracy is the hard part: it needs current Shopify/Google/OpenAI docs, and the rules change monthly.
- Testing it properly requires a live Shopify store, which makes it buildability 4.

---

## C14. Etsy digital-seller compliance kit: 19, VIABLE

**Rationale:** The "why now" just got much stronger.
- **The policy change:** On 22 Oct 2026 Etsy tightened AI rules:
  - disclosure required
  - AI prompt bundles prohibited
  - bot/mass-automated listings prohibited
  - AI-generated functional guides banned
  - stricter image requirements
  - removals and possible shop closure for repeat violations

  Sources: [Etsy Seller Handbook](https://www.etsy.com/seller-handbook/article/1522733284810), [Digital Commerce 360, 26 Oct 2026](https://www.digitalcommerce360.com/2026/10/26/etsy-ai-policy/amp/), [eMarketer](https://www.emarketer.com/content/etsy-cracks-down-on-ai-listings-rebuild-buyer-seller-trust), [ppc.land](https://ppc.land/etsy-forces-sellers-to-show-one-unaltered-photo-in-every-listing/).
- **Seller pain:** removal threads exist on Etsy's own forum.
- **Against it:**
  - Etsy publishes the rules itself, for free, in plain language.
  - Within days, a wave of free blog explainers appeared (findskill.ai, inkfluenceai, explainx, kompozy, rewarx).
  - I found no paid compliance kit with sales, so willingness to pay is unproven.

**Best-scoped version:** "Etsy AI-Policy Listing Audit Kit (Oct 2026 rules)". It includes:
- a Google Sheet that audits each listing (disclosure present? functional guide? image requirements? prompt-bundle risk?)
- 10 human-written disclosure-sentence templates by product type (printables, Canva templates, clipart, planners)
- an appeal-letter template for wrongful removals
- a dated changelog page

Do not include an "ongoing policy tracker" promise; it can't be maintained solo.

**Target buyer:** an Etsy digital-download seller with 50-500 listings (printables, Canva templates, planners, clipart) who used AI somewhere in their workflow and fears removal or shop closure.

**Demand evidence:**
- Etsy Community removal threads (dates not shown in results):
  - ["My listing was removed that doesn't follow Etsy's Creativity Standards"](https://community.etsy.com/t5/Technical-Issues/My-listing-was-removed-that-doesn-t-follow-Etsy-s-Creativity/m-p/146483880)
  - ["Listing Removed for Violating Creativity Standards as AI found"](https://community.etsy.com/t5/Technical-Issues/Listing-Removed-for-Violating-Creativity-Standards-as-AI-found/m-p/146482631/highlight/true)
  - ["My Listing Removed by Mistake"](https://community.etsy.com/t5/Technical-Issues/My-Listing-Removed-by-Mistake/m-p/148836738)
  - ["Etsy deactivated a bunch of Canva templates I made myself"](https://community.etsy.com/t5/Technical-Issues/Etsy-deactivated-a-bunch-of-Canva-templates-I-made-myself/m-p/146045612/highlight/true)
- Press coverage of the Oct 2026 update:
  - [Retail Dive](https://retaildive.com/news/etsy-updates-ai-use-policies-emphasize-craftsmanship/833838)
  - [Value Added Resource](https://www.valueaddedresource.net/etsy-bans-ai-patterns/)
  - [Crowdfund Insider](https://www.crowdfundinsider.com/?p=320422)
  - [letsdatascience](https://letsdatascience.com/news/etsy-bans-ai-generated-recipes-and-patterns-tightens-photo-r-b8c546e9)
- No r/EtsySellers thread surfaced; Reddit is blocked to the crawler.
- Removal-count claims (12,000 in Q1 2026; 17,000 in early 2025) come from vendor blogs and conflict. **Unverified.**

**Competition snapshot:**
- **Free official:**
  - [Creativity Standards](https://www.etsy.com/legal/creativity)
  - [Important updates to AI use on Etsy](https://www.etsy.com/seller-handbook/article/1522733284810)
  - [What is Etsy's stance on AI creations?](https://www.etsy.com/seller-handbook/article/1275449912004)
  - [Listing Image Requirements](https://www.etsy.com/legal/policy/listing-image-requirements/253962679005)
  - [Help: image requirements](https://help.etsy.com/hc/en-us/articles/44297885802647-How-Do-Etsy-s-Listing-Image-Requirements-Apply-to-My-Listings?segment=selling)
- **Free blogs:**
  - [findskill.ai](https://findskill.ai/blog/etsy-ai-rules-october-2026-seller-guide/)
  - [inkfluenceai](https://www.inkfluenceai.com/blog/etsy-ai-rules-update-october-2026)
  - [explainx](https://explainx.ai/blog/etsy-ai-policy-update-unedited-photo-ban-ai-guides-bot-listings-2026)
  - [kompozy](https://kompozy.io/news/etsy-ai-use-policy-update-october-2026)
  - [rewarx compliance guide](https://www.rewarx.com/blogs/etsy-ai-transparency-standard-compliance-guide)
  - [listadum](https://www.listadum.com/blog/etsy-creativity-standards)
  - [lineart-ink compliance guide](https://lineart-ink-core.pages.dev/blog/etsy-ai-compliance-guide)
- **Free repo:** JanPienaar/keepr-etsy-ops, a Claude Code Etsy skill pack "with compliance gates".
- **Paid:** none found on Etsy or Gumroad in my searches. That is either a gap or a sign of no demand. Adjacent paid Etsy tools (eRank, Marmalead, Alura; "Super Spy HeyEtsy" $19 with 80 ratings, relayed from Phase 1 MS#34) show sellers pay for tools.

**Kill reasons found:**
- Etsy's own free, plain-language policy pages cover the rules.
- Free explainer blogs appeared within days.
- **Irony risk:** a Claude-written compliance guide sold on Etsy could itself breach the AI-generated functional-guide rule. It must be human-authored, disclosed and template-heavy.

No fatal reason: the free sources explain the rules but don't audit your 300 listings.

**Price recommendation:** $9-15 on Etsy.

**Launch channels:**
- **Etsy.** Sellers buy seller resources there (Phase 1 relayed 8 Etsy-seller products in the Gumroad crawl; Etsy search volume for "etsy ai disclosure" NOT VERIFIED). Rules: AI disclosure required, no prompt bundles, no AI-generated functional guides ([Etsy Seller Handbook](https://www.etsy.com/seller-handbook/article/1522733284810)).
- **Gumroad** as a secondary channel.
- **r/EtsySellers:** self-promotion rules NOT VERIFIED.
- **Etsy Community forums:** promotion rules NOT VERIFIED (assume prohibited).

**Biggest risk:** sellers read Etsy's free page and move on. A smaller risk is Etsy flagging the kit itself. **Cheapest test:** a $9 Etsy listing within 7 days, while the 22 Oct change is fresh. Kill it if there is no sale in 21 days. Check eRank/Etsy autocomplete for "ai disclosure" first.

**Build notes:** 4-5 hours.
- Google Sheet audit with dropdowns and conditional formatting, a PDF of templates, and an appeal letter.
- Cite Etsy's pages by link; don't copy them.
- Write and hand-edit in the founder's own voice, and add an AI-use disclosure to the listing.

---

## C15. Vibe-coder launch safety kit: 15, REJECT (fatal kill reason)

**Rationale:** The pain is real and well documented: Moltbook, the Lovable RLS CVE affecting about 170 apps, audits finding RLS off. But free official and platform-native tools now do the core job.
- **Lovable:** it scans automatically for security issues before every publish and has integrated Supabase's Security Advisor ([Lovable blog](https://lovable.dev/blog/secure-vibe-coding), [createwith](https://www.createwith.com/tool/lovable/updates/lovable-launches-automatic-security-scanning-before-every-publish)).
- **Claude Code users:** they get cloudflare/security-audit-skill free (56,272 stars, created 18 Jun 2026).
- **More free checklists, skills and scanners:** benavlabs/vibe-check, slopsec, rlsgate, VibeRaven, boxed-dev 69-check list. GitHub search returned 35 repos for "vibe coding security checklist" and 23 for "supabase security scanner vibe".
- **Paid:** Gumroad has several paid checklists already, with no visible traction.

**Best-scoped version:** none as a standalone product. A non-security "launch admin" checklist (privacy policy, terms, backups, Stripe webhook verification, data-deletion process) is a thin remainder. It could be a free lead magnet, not a $19 product.

**Target buyer:** a non-developer founder shipping a Lovable, Bolt or Claude Code app that handles customer data.

**Demand evidence:**
- [Moltbook flaw exposed AI chats and keys](https://securitybrief.co.uk/story/moltbook-vibe-coded-flaw-exposed-ai-chats-keys) (SecurityBrief)
- [I audited 50 vibe-coded apps](https://dev.to/rishabh_kumar_6d865c83a4d/i-audited-50-vibe-coded-apps-heres-what-broke-1pb6): "70% of audited Lovable apps had RLS completely off" (small sample)
- [Your vibe-coded app might be wide open](https://dev.to/noa-agent/your-vibe-coded-app-might-be-wide-open-heres-how-to-check-4ihe)
- [rockingtech production-ready checklist, 2 Jul 2026](https://rockingtech.co.uk/blog/is-your-vibe-coded-app-production-ready-checklist)
- [Lovable/Bolt/v0 security crisis for non-technical founders](https://dev.to/varsha_ojha_5b45cb023937b/the-lovableboltv0-security-crisis-what-non-technical-founders-must-fix-before-going-live-9i5)
- One search-result article says a pre-launch checklist went viral on r/vibecoding with replies like "I shipped without doing any of this". The tool did not attribute it to a specific URL, so the thread is NOT VERIFIED.

**Competition snapshot:**
- **Free official/platform:** Lovable's pre-publish scan, Supabase Security Advisor and Lovable's AI Security Reviewer.
- **Free repos (GitHub search, 1 Nov 2026):**
  - cloudflare/security-audit-skill: 56,272 stars
  - astoj/vibe-security: 165 stars
  - benavlabs/vibe-check: 142 stars
  - finehq/vibe-coding-checklist: 37 stars
  - lachydotmcg/slopsec (Claude Code skill): 25 stars
  - boxed-dev/vibe-coding-security: 15 stars
  - ohad6k/VibeRaven: 61 stars, "Free, local, no login"
  - SymbioticSec/vibe-scanner: 23 stars
  - GerardoRdz96/rlsgate
  - AlonAI4/code-armour, which also covers legal/privacy
- **Paid, Gumroad:**
  - [vibe code security checklist](https://givigier.gumroad.com/l/vibe-code-security-checklist)
  - [Pre-Push Review Prompt](https://buildtolaunch.gumroad.com/l/pre-push-review) (has a Supabase RLS add-on)
  - [Smoke Testing checklist](https://buildtolaunch.gumroad.com/l/best-vibe-coding-testing-checklist)
  - [Secure Coding ebook](https://uigerhana.gumroad.com/l/vibe-coding-security)
  - Relayed: [blncraft vibe-coder-kit](https://blncraft.gumroad.com/l/vibe-coder-kit)
  - No ratings were visible.
- **Paid, Product Hunt:** ["The Security Guide for Vibe Coders"](https://www.producthunt.com/products/the-security-guide-for-vibe-coders?page=2).

**Kill reasons found:**
1. **Fatal:** a free platform-native scanner (Lovable plus Supabase Security Advisor) and a 56k-star free official-vendor skill (Cloudflare) do the core security job.
2. There are dozens of free checklists and paid Gumroad clones.
3. **Liability:** selling "launch safety" to non-developers implies an assurance that a checklist can't give.

**Price recommendation:** do not sell. At most, give it away free as a lead magnet.

**Launch channels:**
- **r/vibecoding and r/lovable:** self-promotion rules NOT VERIFIED.
- **Product Hunt:** similar guides are listed; rules NOT VERIFIED.
- **Gumroad:** search shows many vibe-coding listings, so supply-side traffic exists.

**Biggest risk:** n/a (rejected). If the lead wants a test anyway: post the free checklist to r/vibecoding and count email sign-ups before building anything paid.

**Build notes:** the skill and checklist would be easy. Credibility would need testing against a sample Supabase app, which takes a few hours.

---

## Method & limitations
- **Searches:** I used exactly 20 WebSearch calls (the hard cap).
  - Etsy-domain searches: 4
  - Gumroad-domain searches: 3
  - support.google.com: 1
  - shopify.com: 1
  - Plain queries for Reddit/demand/rules/free tools: 11
- **WebFetch** was not used; per the brief it is blocked.
- **GitHub:** the `repos/` endpoint returned 403 in this session, but the `search/repositories` endpoint worked. All star counts come from search results pulled on 1 Nov 2026.
- **Etsy and Gumroad:** review counts and sales counts were **not visible** in search-result summaries. I could not confirm sales for any GEO, review-card, compliance or vibe-coding kit. That is why every wtp score is 2.
- **Reddit:** no first-hand Reddit threads were retrieved for this batch (crawler blocked). Reddit evidence is from Phase 1 mirror links or search summaries.
- **Etsy policy text:** quotes come from the search tool's summaries of Etsy pages. I could not read the pages directly, so the exact clause wording is unverified.
- **Subreddit rules:** only the r/smallbusiness weekly-promo-thread rule was partially verified, from 2024 mirrors. All other community rules are NOT VERIFIED.
- **Gaps:** I did not check paid agentic-commerce checklists on Gumroad/Etsy (C13), Etsy search volumes, or TPT/Chrome Web Store, which are not relevant to this batch.

## Sources
- https://www.etsy.com/market/chatgpt_seo
- https://www.etsy.com/market/local_seo
- https://www.etsy.com/market/google_business_profile
- https://www.etsy.com/listing/4352991947/ai-seo-automation-workflow-keyword
- https://www.etsy.com/market/google_review_card_templates
- https://www.etsy.com/market/review_request
- https://www.etsy.com/market/request_review_card
- https://www.etsy.com/market/google_review_printable
- https://www.etsy.com/listing/4480710918/google-review-card-template-editable-qr
- https://www.etsy.com/listing/1727191495/google-review-canva-template-leave-us-a
- https://www.etsy.com/listing/1588306343/google-square-review-card-template
- https://www.etsy.com/listing/1754614558/google-review-sign-review-card-template
- https://www.etsy.com/seller-handbook/article/1522733284810
- https://www.etsy.com/seller-handbook/article/1275449912004
- https://www.etsy.com/legal/creativity
- https://www.etsy.com/legal/policy/listing-image-requirements/253962679005
- https://help.etsy.com/hc/en-us/articles/44297885802647-How-Do-Etsy-s-Listing-Image-Requirements-Apply-to-My-Listings?segment=selling
- https://community.etsy.com/t5/Technical-Issues/My-listing-was-removed-that-doesn-t-follow-Etsy-s-Creativity/m-p/146483880
- https://community.etsy.com/t5/Technical-Issues/Listing-Removed-for-Violating-Creativity-Standards-as-AI-found/m-p/146482631/highlight/true
- https://community.etsy.com/t5/Technical-Issues/My-Listing-Removed-by-Mistake/m-p/148836738
- https://community.etsy.com/t5/Technical-Issues/Etsy-deactivated-a-bunch-of-Canva-templates-I-made-myself/m-p/146045612/highlight/true
- https://www.digitalcommerce360.com/2026/10/26/etsy-ai-policy/amp/
- https://retaildive.com/news/etsy-updates-ai-use-policies-emphasize-craftsmanship/833838
- https://www.valueaddedresource.net/etsy-bans-ai-patterns/
- https://www.emarketer.com/content/etsy-cracks-down-on-ai-listings-rebuild-buyer-seller-trust
- https://ppc.land/etsy-forces-sellers-to-show-one-unaltered-photo-in-every-listing/
- https://www.crowdfundinsider.com/?p=320422
- https://letsdatascience.com/news/etsy-bans-ai-generated-recipes-and-patterns-tightens-photo-r-b8c546e9
- https://findskill.ai/blog/etsy-ai-rules-october-2026-seller-guide/
- https://www.inkfluenceai.com/blog/etsy-ai-rules-update-october-2026
- https://explainx.ai/blog/etsy-ai-policy-update-unedited-photo-ban-ai-guides-bot-listings-2026
- https://kompozy.io/news/etsy-ai-use-policy-update-october-2026
- https://www.rewarx.com/blogs/etsy-ai-transparency-standard-compliance-guide
- https://www.listadum.com/blog/etsy-creativity-standards
- https://lineart-ink-core.pages.dev/blog/etsy-ai-compliance-guide
- https://tanguykeyzer.gumroad.com/l/ssjwve
- https://datmark.gumroad.com/l/ai-traffic-dashboard
- https://modernwebseo.gumroad.com/l/ai-agency-launch-kit
- https://growthwithalex.gumroad.com/l/aisearchagent
- https://genxops.gumroad.com/l/geo_for_smbs (Phase 1)
- https://aeo-starter-kit.pages.dev/ (Phase 1)
- https://payhip.com/b/YzjDQ (Phase 1)
- https://enlightprints.gumroad.com/l/Greview
- https://promarketing10.gumroad.com/l/LocalRankAI
- https://automatewithbishal.gumroad.com/l/AutomatedGoogleReviews
- https://hashirmalick.gumroad.com/l/aireplygooglemybusiness
- https://givigier.gumroad.com/l/vibe-code-security-checklist
- https://buildtolaunch.gumroad.com/l/pre-push-review
- https://buildtolaunch.gumroad.com/l/best-vibe-coding-testing-checklist
- https://uigerhana.gumroad.com/l/vibe-coding-security
- https://blncraft.gumroad.com/l/vibe-coder-kit (Phase 1)
- https://www.producthunt.com/products/the-security-guide-for-vibe-coders?page=2
- https://www.brightlocal.com/free-local-seo-tools/local-ai-visibility-checker/
- https://birdeye.com/ai-visibility-checker/
- https://insites.com/resources/free-ai-visibility-audit/
- https://www.zarla.com/whats-new/2026-08-24-see-what-ai-assistants-say-about-your-business
- https://www.hubspot.com/ai-search-grader (Phase 1)
- https://ahrefs.com/ai-visibility-checker (Phase 1)
- https://developers.google.com/search/blog/2026/06/gen-ai-performance-reports (Phase 1)
- https://blogs.bing.com/webmaster/February-2026/Introducing-AI-Performance-in-Bing-Webmaster-Tools-Public-Preview (Phase 1)
- https://reddit.sentinel-team.org/posts/1stc10m/snapshots/2026-04-25T00%3A47%3A11.009274Z
- https://www.humblehelp.studio/blog/chatgpt-wont-recommend-your-business-fix
- https://frostbitemarketing.com/?p=104060
- https://webzum.com/blog/how-to-get-recommended-by-chatgpt
- https://www.bccinteractive.com/blog/local-ai-search-statistics/ (Phase 1)
- https://seosandwitch.com/chatgpt-local-business-statistics/ (Phase 1)
- https://support.google.com/business/answer/16816815?hl=en
- https://support.google.com/business/answer/16334724?hl=en-GB
- https://support.google.com/business/answer/3474122?hl=en-GH
- https://fitsmallbusiness.com/marketing/ask-for-google-reviews/
- https://www.shiftflow.app/playbook/can-i-offer-discount-or-gift-card-for-review
- https://clovvy.pages.dev/google-review-guidelines/
- https://whito.co.uk/news/the-ipad-on-your-counter-is-now-breaking-googles-review-rules/
- https://beancount.io/blog/2026/07/16/ftc-fake-reviews-crackdown-consumer-review-rule-guide
- https://www.beneschlaw.com/insight/five-stars-zero-tolerance-ftc-turns-up-enforcement-under-consumer-review-rule/ (Phase 1)
- https://reddit.sentinel-team.org/posts/1rq57dr/snapshots/2026-03-11T01%3A23%3A07.053576Z (Phase 1)
- https://reddit.sentinel-team.org/posts/1sz8u0r/snapshots/2026-05-02T04%3A50%3A06.954017Z (Phase 1)
- https://reddit.sentinel-team.org/posts/1tn81br/snapshots/2026-05-26T09%3A47%3A52.470198Z (Phase 1)
- https://lr.in.psf.lt/r/smallbusiness/comments/1bn1bpy/promote_your_business_week_of_march_25_2024
- https://lr.in.psf.lt/r/smallbusiness/comments/1cfnz3o/promote_your_business_week_of_april_29_2024
- https://help.shopify.com/en/manual/online-sales-channels/agentic-storefronts
- https://www.shopify.com/news/agentic-commerce-momentum
- https://www.shopify.com/blog/how-agentic-commerce-works
- https://community.shopify.com/t/chatgpt-copilot-agentic-shopping-is-it-live-for-all-shopify-stores/585319
- https://community.shopify.com/t/chatgpt-is-becoming-a-sales-channel/591794
- https://community.shopify.com/t/agentic-shopping-q-a-what-every-shopify-store-needs-to-know-right-now/599243
- https://www.paz.ai/blog/shopify-agentic-storefronts-chatgpt-products-not-showing
- https://ecommercefastlane.com/shopify-agentic-commerce-readiness-guide/
- https://www.storerank.ai/shopify-agentic-commerce-the-complete-guide-for-2026/
- https://askphill.com/blogs/blog/agentic-commerce-for-shopify-protocols-platforms-and-what-to-prioritize-in-2026
- https://shugert.com.mx/resources/shopify-agentic-storefronts-product-data
- https://reddit.sentinel-team.org/posts/1r7c9fd/snapshots/2026-02-18T03%3A43%3A29.412351Z
- https://reddit.sentinel-team.org/posts/1s4zdbz/snapshots/2026-03-27T21%3A08%3A12.710659Z
- https://developers.google.com/merchant/ucp (Phase 1)
- https://www.etsy.com/news/etsy-partners-with-google-on-ai-powered-shopping (Phase 1)
- https://lovable.dev/blog/secure-vibe-coding
- https://www.createwith.com/tool/lovable/updates/lovable-launches-automatic-security-scanning-before-every-publish
- https://securitybrief.co.uk/story/moltbook-vibe-coded-flaw-exposed-ai-chats-keys
- https://dev.to/rishabh_kumar_6d865c83a4d/i-audited-50-vibe-coded-apps-heres-what-broke-1pb6
- https://dev.to/noa-agent/your-vibe-coded-app-might-be-wide-open-heres-how-to-check-4ihe
- https://dev.to/varsha_ojha_5b45cb023937b/the-lovableboltv0-security-crisis-what-non-technical-founders-must-fix-before-going-live-9i5
- https://rockingtech.co.uk/blog/is-your-vibe-coded-app-production-ready-checklist
- GitHub search API (api.github.com/search/repositories, pulled 1 Nov 2026): cloudflare/security-audit-skill, AgriciDaniel/claude-seo, Ryze-AI-Adgent/open-seo-mcp-skills, onvoyage-ai/gtm-engineer-skills, Auriti-Labs/geo-optimizer-skill, leopard627/fire-your-seo-agency, astoj/vibe-security, benavlabs/vibe-check, lachydotmcg/slopsec, boxed-dev/vibe-coding-security, ohad6k/VibeRaven, SymbioticSec/vibe-scanner, GerardoRdz96/rlsgate, AlonAI4/code-armour, monkydot/ucp-ready, zhao-hanbo/agentic-commerce-kit, hongruzoe/shopify-geo-product-auditor, JanPienaar/keepr-etsy-ops, ahmettasdemirusa/local-business-schema-generator, milad-ahmd/google-business-profile-manager, ahmettasdemirusa/local-seo-skills
