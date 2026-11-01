# Phase 3 validation: batch 2 (C06-C10, AI tooling and setup)

Validator #2. Date: 2026-11-01. Rubric and verdict thresholds: `validator-brief.md`. 20 of 20 WebSearch calls used, plus GitHub API and MCP Registry API calls (free).

## Score table

| id | name | demand | competition | wtp | build | distribution | growth | total | verdict |
|---|---|---|---|---|---|---|---|---|---|
| C06 | "Connect Claude to your business tools" setup kit [SEED 5] | 2 | 1 | 2 | 3 | 2 | 1 | **11** | **REJECT** (fatal: free official plugin with one-click OAuth) |
| C07 | Per-trade voice-receptionist template pack for agencies [SEED 6] | 3 | 2 | 3 | 3 | 4 | 4 | **19** | **VIABLE** (only as a compliance + QA layer, not as prompts) |
| C08 | Chatbot & AI-receptionist QA test kit [SEED 8] | 1 | 2 | 2 | 5 | 2 | 2 | **14** | **WEAK** (fold into C07) |
| C09 | Brand voice pack for AI tools [SEED 7] | 1 | 1 | 2 | 5 | 3 | 1 | **13** | **REJECT** (fatal: free official Brand Voice plugin) |
| C10 | "Agent-ready local business" MCP kit | 1 | 3 | 1 | 3 | 2 | 2 | **12** | **REJECT** (no evidence assistants call these servers) |

Bottom line: only C07 survives, and only once it is re-scoped. Plain per-trade prompt packs already sell on Etsy for about $22 and are bundled free in Skool communities. What's still open is the state-by-state disclosure/consent layer plus a pre-launch test-call QA kit (C08 folded in). Everything else in this batch has been absorbed by free official tools or lacks any buyer evidence.

---

## C06. "Connect Claude to your business tools" setup kit [SEED 5]: 11, REJECT

- **Rationale:** The pain is real, but most of it is vendor bugs (OAuth failures, Cowork on Windows, connectors showing "Connected" with no tools) that a guide cannot fix. Anthropic's free Claude for Small Business plugin already turns QuickBooks, Square, Google Workspace and others into OAuth sign-ins from a plugin directory, and a dozen free blog walkthroughs of exactly this setup exist. Paid Cowork guides on Gumroad show no visible sales. The content would go stale with each Cowork release.
- **Best-scoped version:** None standalone. At most, a 2-page "connect QuickBooks/Jobber to Claude: the 5 gotchas" PDF used as a free lead magnet or a chapter inside a vertical pack (C01/C02). Example gotcha: a developer sandbox does not work, so you need a paid or trial QBO file.
- **Target buyer:** an SMB owner on Claude Pro trying Cowork connectors for the first time.
- **Demand evidence:**
  - Phase 1 G6 (ai-ecosystem-gaps.md, section C): 1,312 Cowork-titled issues in anthropics/claude-code and 927 issues in anthropics/claude-ai-mcp since May 2026. These come from technical reporters, not non-dev buyers.
  - Reddit mirror (2026-05-29): a user couldn't finish QuickBooks OAuth with an Intuit sandbox (403) and had to switch to a QBO trial. https://reddit.sentinel-team.org/posts/1tmpeq5/snapshots/2026-05-29T18%3A50%3A49.032229Z
  - A free guide already documents the same gotcha: "Developer sandboxes do not work — this is the single biggest setup gotcha". https://findskill.ai/blog/claude-for-small-business-setup-walkthrough/
- **Competition snapshot:**
  - Paid: "Cowork Mastery: The Ultimate Claude Cowork Guide for Mac Users" (https://theusefultech.gumroad.com/l/cowork-mastery-guide, price and sales not visible). "Claude Cowork Guide 2026" (https://intelligentsam5.gumroad.com/l/gvnzfh, includes "Connector setup cheatsheets", price not visible). "N8n MCP Integration Handbook" on Etsy (https://www.etsy.com/listing/4518427513/n8n-mcp-integration-handbook-claude-n8n).
  - Free:
    - Claude for Small Business plugin. Search results describe it as bundling QuickBooks, PayPal, HubSpot, Canva, Docusign, Google Workspace, Microsoft 365, Square and Stripe connectors, "included with any Claude subscription at no additional cost" (https://siliconangle.com/2026/05/13/anthropic-launches-claude-small-business-new-automation-workflows/, https://www.digitalapplied.com/blog/claude-for-small-business-quickbooks-hubspot).
    - Free setup guides: https://findskill.ai/blog/claude-for-small-business-setup-walkthrough/, https://www.pulse.bot/ai/blogs/claude-for-small-business-the-practical-setup-guide-d39a3c45-9cbc-40f2-8de0-7f332b23732c/, https://mikareyes.com/ai/how-to-setup-claude-for-small-business.md, https://consulting.sva.com/insights/claude-for-small-business-how-to-connect-it-to-the-tools-you-already-use, https://dev.to/akaranjkar08/claude-for-small-business-15-workflows-setup-guide-2026-4kak
    - From Phase 1 G6: mcpb one-click installs (~718k npm downloads a month) and microsoft/mcp-for-beginners (17.6k stars).
  - **Date conflict:** candidates.md says Claude for Small Business launched on 15 Sep 2026. Search results (SiliconANGLE URL dated 2026/05/13) say 13 May 2026. Either way, it is live and free.
- **Kill reasons:**
  - The free official plugin and connector directory do the job, with OAuth sign-in and no JSON config.
  - The top errors are platform bugs that a guide can't fix.
  - The advice goes stale weekly.
  - Many free walkthroughs exist.
- **Price recommendation:** none ($0 lead magnet only).
- **Launch channels:**
  - r/ClaudeAI: self-promotion rules NOT VERIFIED.
  - Gumroad: no evidence that buyers browse for this.
- **Biggest risk + cheapest test:** Nobody pays for what's free and official. Test: publish the 2-page gotchas PDF free and count opt-ins over 7 days. If it can't pull free downloads, a paid version is dead.
- **Build notes:** Credible screenshots need paid or trial QuickBooks Online, Square and Jobber accounts, on both Mac and Windows. Every Cowork update risks breaking the steps. That rules out a one-day build at quality.

---

## C07. Per-trade voice-receptionist template pack for AI-automation agencies [SEED 6]: 19, VIABLE

- **Rationale:** Agencies clearly buy templates. Ciela's whole business is $49-per-template or $99/month Vapi templates, a dental voice-bot kit sells at $179/$349, and Etsy has receptionist script packs from $9-$22 up to about $47. But the plain "per-trade prompts" idea is **already done**: Etsy lists an HVAC AI Receptionist Deployment Kit (call flows, intake schema, escalation scripts, QA workbook), a 25-script HVAC GHL prompt pack and a $22 Vapi/Bland/Retell script pack. Ciela covers HVAC, dental, fence, cleaning, moving, accounting and more, and voice-AI Skool communities give templates away with membership. The open gap is narrower: state AI-disclosure and recording-consent scripts plus a pre-launch test-call QA kit, which none of the listings I found leads with. No sales or review counts were visible anywhere, so WTP stays at 3.
- **Best-scoped version:** "Voice Agent Launch-Safety Kit for HVAC & Plumbing agencies". Contents:
  - (1) state-by-state AI-disclosure and call-recording-consent opening lines and consent flows, as a Sheet with sources and a "not legal advice" note
  - (2) an emergency-triage rule block (gas/CO/flooding) to paste into any system prompt
  - (3) 50 scripted test calls and a pass/fail scorecard (C08 folded in)
  - (4) a Vapi and Retell tool-schema JSON for booking/transfer
  - (5) a client go-live sign-off sheet

  Sell per trade, and add dental (with a BAA checklist) as a second SKU.
- **Target buyer:** a 1-5-person AI-automation agency or freelancer selling receptionists to home-service businesses for $400-$2,000/month retainers (Ciela's claimed client pricing: https://ciela.ai/blogs/pre-built-ai-agent-templates-for-agencies).
- **Demand evidence:**
  - Phase 1 TR#3 (trend-scout.md): "ai receptionist" GitHub repos up 8.8x year on year, momentum 1.44. Repos naming Vapi/Retell only up 1.5x, so growth is in applications.
  - At least 5 Skool communities target voice-AI agency builders: AI Voice Network (https://www.skool.com/aivoicenetwork/about), The AI Reseller Club (https://www.skool.com/voice-ai-mastery-5847), Voice Self-Hosters (https://chat.skool.com/voice-self-hosters), Voice Offer Lab (https://www.skool.com/openautomation-collective-6267), Voice AI Wrapper Academy (https://www.skool.com/voice-ai-wrapper-academy-3838). This shows a buyer population; it does not show buyers asking for templates.
  - Agency-side supply on Fiverr and Upwork for HVAC/plumbing receptionists (https://www.upwork.com/services/product/admin-customer-support-build-ai-receptionist-for-hvac-plumbing-electrical-ai-calling-agent-2071660623106302895, https://fiverr.com/simon_benedic/create-ai-receptionist-using-vapi-and-retell-ai).
  - Phase 1 pain-hunter #3: home-service owners on Reddit complain about missed calls (mirror 1tgvx7m, 2026-05-22). That's end-client demand, not agency template demand.
  - **No thread found of an agency explicitly asking to buy templates.**
- **Competition snapshot:**

  | Product | Price | Sales/quality signal | URL |
  |---|---|---|---|
  | AI Receptionist Script Pack (Vapi, Bland, Retell call prompts), Etsy | $22 | No reviews visible in snippet | https://www.etsy.com/market/ai_receptionist |
  | HVAC AI Receptionist Deployment Kit (TradeKitWorks), Etsy AU | not visible | Master prompt, HVAC call flows, intake schema, emergency scripts, n8n starter, QA workbook | https://www.etsy.com/au/listing/4539664221/hvac-ai-receptionist-deployment-kit |
  | GHL AI Voice Agent Prompt Pack (25 HVAC scripts), Etsy | not visible (Etsy results for this search ranged ~$22-$47) | Repeats across Etsy search pages | https://www.etsy.com/market/ai_voice_agent_prompts |
  | Plumbing AI Receptionist Bot, Etsy | not visible | n/a | https://www.etsy.com/listing/4300593201/plumbing-ai-receptionist-bot-virtual |
  | Contractor Inbound Service Call Script & Safety Triage Sheet, Etsy | $9 | gas/CO/electrical/water safety scripts | https://www.etsy.com/market/ai_receptionist |
  | Dental voice bot kit (EN/DE/ES prompts, Vapi/Retell/ElevenLabs setup) | $179 Pro / $349 Agency, Gumroad checkout | no sales visible | https://dental-voice-bot-kit.vercel.app/ |
  | Ciela templates (HVAC, dental, 50-350+ verticals, Vapi + n8n) | $49 one-time per template, or $99/mo library (pages conflict) | vendor claims only | https://ciela.ai/agents/hvac-voice-receptionist, https://ciela.ai/blogs/pre-built-ai-agent-templates-for-agencies |
  | Retell dental clinic blueprint (Retell + n8n + Open Dental) | not visible | n/a | https://zainulabideenbaloch.gumroad.com/l/cjnmds?layout=profile |
  | Voice agent prompts / Retell prompt masterclass | not visible | n/a | https://yashica.gumroad.com/l/voice-agent-prompts |
  | Phase 1: "AI Voice Assistant - Complete Setup & Build Guide" | $17 | 1 rating | marketplace-saturation-scout.md row 27 |

  **Free alternatives:**
  - Vapi's official Voice Agent Prompt Reference (https://docs.vapi.ai/_fern-files/vapi.docs.buildwithfern.com/cf133005c62df7efa56a080a60422cbbf38e3d26974594187db228dccf935bd1/static/vapi-prompt-reference.md).
  - TomHardiman6/ai-receptionist-starter ("Starter templates for building an AI receptionist with Claude Code + Vapi", GitHub API).
  - Phase 1 G9: TRivers01/ai-receptionist-templates (dental, legal, HVAC, salon, real estate). It could not be re-checked; the GitHub API was not enabled for this repo.
  - ashtonvossai Retell x Make home-services template (listed at A$0, https://ashtonvossai.gumroad.com/l/ipjjqy).
  - Josue Hernandez "Voice AI Receptionist: VAPI MCP" at $0 (https://scalehatch.gumroad.com/).
  - Free compliance checklists from vendors (Phase 1 REG#6: dialzara, thoughtly).
  - Templates bundled with Skool memberships (above).
- **Kill reasons (none fatal):**
  - The per-trade prompt idea is already on Etsy and in Ciela.
  - Templates come free with Skool memberships.
  - A Ciela comparison notes "sophisticated agents typically require programmatic configuration", which caps the value of a template (https://ciela.ai/vs/vapi).
  - Compliance scripts carry legal-accuracy risk: state AI-disclosure laws are contested (Phase 1 REG#6), so sell them as "researched starting points, not legal advice".
  - VC consolidation in voice receptionists (Phase 1 TR#3: YC "voice receptionist" match fell from 24 to 14).
- **Price recommendation:** $39 per trade kit; $79 for an HVAC + plumbing + dental bundle. Anchors: Etsy $22 for generic prompts and Ciela $49 per template. Stay under $100, since the $179 dental kit shows no proof of sales.
- **Launch channels:**
  - Etsy: buyer search pages exist for the exact terms ("ai receptionist", "ai voice agent prompts", "ai voice agent template": https://www.etsy.com/market/ai_receptionist, https://www.etsy.com/market/ai_voice_agent_prompts, https://www.etsy.com/market/ai_voice_agent_template). Etsy listing rules for AI-generated digital goods (Creativity Standards) were NOT VERIFIED in this run.
  - Gumroad Discover: no traffic data.
  - Skool voice-AI communities: promotion rules NOT VERIFIED.
  - r/automation: a third-party mirror says to "avoid using r/automation solely as a platform to advertise your products, services, or personal websites without genuine engagement" (https://gummysearch.com/r/automation/; not the live rules).
  - r/AI_Agents: rules NOT VERIFIED (https://gummysearch.com/r/AI_Agents).
- **Biggest risk + cheapest test:** Agencies treat this as a commodity they already get free or for $22. Test: list the HVAC kit on Etsy and Gumroad at $39, with a free "10 state AI-disclosure opening lines" sample posted to one Skool community and to r/automation as a value post. Kill it if there are fewer than 3 sales in 14 days. Before building, the founder should open the Etsy HVAC kit and the $22 script pack in a browser and check their review counts (we couldn't fetch Etsy).
- **Build notes:** Docs, the Sheet and JSON fit in 8 hours. State-law research is the slow part: keep it to disclosure and all-party-consent states, cite every row, and date-stamp it. Validating the tool-schema JSON needs a pay-as-you-go Vapi account plus a phone number (budget under $20). Don't ship untested JSON. A BAA statement for dental must not claim Vapi/Retell HIPAA status; Phase 1 found no BAA documentation.

---

## C08. Chatbot & AI-receptionist QA test kit for SMBs [SEED 8]: 14, WEAK

- **Rationale:** I found nobody selling or asking to buy a chatbot QA checklist for SMBs. The only discussions are QA engineers (r/softwaretesting) and vendor content-marketing blogs. Free 2026 checklists are everywhere, and chatbot platforms build testing and evals into their own products. The "why now" liability rulings are thin: Air Canada is from 2024, OLG Hamm is not final, and nothing mandates testing.
- **Best-scoped version:** No standalone version. Fold it into C07 as the "50 test calls + scorecard" module, where QA is already a selling feature (the Etsy HVAC kit ships a "QA workbook").
- **Target buyer:** an agency launching a client chatbot or receptionist (not the SMB owner).
- **Demand evidence:**
  - r/softwaretesting thread on testing "AI that talks back" (QA engineers, not SMBs): https://redlib.hackliberty.org/r/softwaretesting/comments/1la9uc2/how_were_testing_ai_that_talks_back_and_sometimes
  - Vendor blogs only beyond that: https://insertchat.com/blog/ai-chatbot-testing-checklist-for-client-launch, https://chatimize.com/chatbot-testing/ ("How to Test a Chatbot Before Going Live: A Practical Checklist (2026)"), https://getautonoma.com/blog/chatbot-testing-checklist
  - Phase 1 MS#49: only 2 free GitHub checklist repos, and no paid listing.
- **Competition snapshot:**
  - Paid chatbot-specific: none found on Etsy or Gumroad. Adjacent paid items:
    - Etsy generic software QA templates (https://www.etsy.com/listing/4514447072/qa-test-plan-cases-checklist-templates, https://www.etsy.com/listing/4391081115/software-go-live-checklist-template)
    - Gumroad "AI Jailbreak Toolkit" (https://eye2on1ai.gumroad.com/l/ai-jailbreak-toolkit?layout=profile)
    - "Safeguard Pro Prompt Checker", which has a "Red-Team Injection Test mode" (https://mbakry.gumroad.com/l/SafeguardPromptChecker-ContentComplianceAuditor)
  - Free:
    - Free checklists from chatimize, getautonoma, insertchat, fin.ai (https://fin.ai/learn/how-to-test-ai-agent-before-deployment) and TestMu (https://www.testmuai.com/learning-hub/chatbot-hallucination/).
    - Platform-native evals: Chipp (https://chipp.ai/docs/guides/understanding-evals.md) and Hyperleap (https://hyperleap.ai/help/bot-studio/testing).
    - The OWASP LLM Top 10.
- **Kill reasons:**
  - No buyer demand found.
  - Free checklists are abundant.
  - Chatbot platforms are absorbing testing into their own products.
  - The "liability" why-now is not a mandate.
- **Price recommendation:** $0 standalone; worth +$10-20 of perceived value inside C07.
- **Launch channels:**
  - Etsy "website qa checklist" search page exists (https://www.etsy.com/market/website_qa_checklist), but it serves software-QA buyers.
  - No SMB channel found.
  - Subreddit rules NOT VERIFIED.
- **Biggest risk + cheapest test:** Nobody searches for it. Test: offer the QA module as a separately priced $15 add-on beside C07 and compare attach rate.
- **Build notes:** It's trivially buildable (a test-prompt Sheet plus a scorecard). Effort isn't the problem; buyers are.

---

## C09. Brand voice pack for AI tools [SEED 7]: 13, REJECT

- **Rationale:** An official, free Brand Voice plugin for Claude Cowork (by Tribe AI, a Cowork launch partner) already discovers voice from your documents, generates "LLM-ready brand guidelines" with a "We Are / We Are Not" framework, and enforces them. That is this product. Etsy is full of brand-voice guide templates and Claude/ChatGPT project kits, and Phase 1 found a $9 price anchor. The only demand evidence is vendor blogs.
- **Best-scoped version:** none. At most, it's a 1-page "voice interview" bonus inside a vertical pack.
- **Target buyer:** a solo marketer or small business owner using ChatGPT or Claude.
- **Demand evidence:** vendor blogs only (Phase 1 PH#29: lilachbullock.com, marqeable.com, backstory.work). No buyer threads found.
- **Competition snapshot:**
  - Paid:
    - Etsy search pages for "brand voice guide", "brand voice template" and "ai brand voice tool" exist (https://www.etsy.com/market/brand_voice_guide, https://www.etsy.com/market/brand_voice_template, https://www.etsy.com/mx/market/ai_brand_voice_tool).
    - Claude AI Project Kit for Content Creators (https://www.etsy.com/listing/4505875061/claude-ai-project-kit-for-content).
    - BrandingOS, 13 Claude skills including tone of voice (https://thesagocreator.gumroad.com/l/brandingos-claude).
    - Claude Skill Bundle: Content & Copywriting 50+, with a "Content Style Guide" skill (https://aimastering.gumroad.com/l/claude-skill-bundle-content-and-Copywriting).
    - "Brand Voice Extractor" at $9 (Phase 1 MS#48).
    - No sales or review counts were visible.
  - Free:
    - Official Brand Voice plugin (https://raw.githubusercontent.com/anthropics/knowledge-work-plugins/main/partner-built/brand-voice/README.md, fetched and read).
    - Anthropic marketing plugin "enforce brand voice" (Phase 1 G10).
    - Brand-building-skills (821 stars) and 216 "brand voice skill" repos (Phase 1 MS#48).
    - Native Claude Projects and ChatGPT custom instructions.
- **Kill reasons:**
  - A free official plugin does the same job (fatal).
  - The market is saturated, with a $9 anchor.
  - Growth is flattening (Phase 1 TR#18).
- **Price recommendation:** none.
- **Launch channels:** Etsy search pages exist (above), but they are crowded. Rules NOT VERIFIED.
- **Biggest risk + cheapest test:** It's absorbed by free tools. No test is worth running.
- **Build notes:** Trivial to build, which is part of why the shelf is full.

---

## C10. "Agent-ready local business" MCP kit: 12, REJECT

- **Rationale:** The registry entries are real. A live query shows single-business servers such as com.kcplumb/booking ("Book plumber in Kansas City, MO…"), com.thejohnsonbros/plumbing-booking, com.delcoplumbernow/plumber, com.joeygeorgeplumbing, com.westernskyhvac.www/booking and com.absolutebestair/hvac. But a cluster of near-identical "the site's own MCP server" entries on lead-gen sites (californiahvacreplacementcost, floridahvacreplacementcost, texashvacreplacementcost, comparehvacsoftware, hvacsoftwarepicker) shows this is an SEO play by operators who already have a generator. **I found no evidence that ChatGPT, Claude, Perplexity or Google consume single-business MCP servers from the registry.** Local booking in AI is going through aggregators instead: Google AI Mode agentic booking with partners such as OpenTable, Resy and Booksy (home services announced for summer 2026), Thumbtack in ChatGPT and Claude per one search summary (unverified), and booking-aggregator MCPs (Sunrays, Qasper, Lokuli, HireNimbus).
- **Best-scoped version:** none as a product. If anything, fold "Schema.org/JSON-LD + booking-link hygiene for AI Mode" into C11.
- **Target buyer:** local-SEO freelancers and agencies.
- **Demand evidence:**
  - Supply-side only. MCP Registry API queries (https://registry.modelcontextprotocol.io/v0/servers?search=plumb, https://registry.modelcontextprotocol.io/v0/servers?search=hvac, run 2026-11-01).
  - Phase 1 G7.
  - No buyer threads.
- **Competition snapshot:**
  - Direct kits: none found.
  - Substitutes:
    - Sunrays local service booking MCP (https://glama.ai/mcp/connectors/dev.sunrays.mcp/sunrays-local-service-booking)
    - Qasper MCP (https://mcpservers.org/servers/qasper-ai-mcp, 0 stars)
    - Lokuli skills (https://implexa.ai/s/clawhub/lokuli-skills)
    - Custom MCP server agencies (https://studiomeyer.io/en/services/custom-mcp-server)
    - Google AI Mode agentic booking (https://www.searchenginejournal.com/google-ai-mode-adds-agentic-booking-expands-to-more-countries/554345/, https://www.nearmedia.co/local-agents-alexas-do-over-google-dark-ad-patterns-reviewpocalypse/)
- **Kill reasons:**
  - No evidence that any assistant routes local queries to these servers (fatal for a paid kit).
  - Platforms are choosing aggregator partners.
  - The registry niche is already being mass-produced by lead-gen operators.
  - Publishing to the registry needs a domain-namespace verification step, which non-technical buyers struggle with.
- **Price recommendation:** none.
- **Launch channels:** local-SEO communities: rules NOT VERIFIED. No marketplace where buyers browse for this.
- **Biggest risk + cheapest test:** It's a product for a channel that may never send traffic. Cheapest test, for later: ask kcplumb/Johnson Bros-style operators whether they've had any AI-originated bookings. It can't be done in a day.
- **Build notes:** A Cloudflare Worker plus JSON-LD template is buildable in a day. Registry publishing needs DNS/HTTP namespace verification, and testing it against ChatGPT/Claude means connecting it as a custom connector, which proves nothing about organic discovery.

---

## Method & limitations

- I used 20 WebSearch calls: Gumroad- and Etsy-scoped competitor checks, Skool, Reddit-mirror demand searches, a subreddit-rules search, and AI-Mode and MCP-discovery searches. Free checks: the GitHub API (repo search; individual repo lookups for TRivers01, Synorthos and Autonoma were **blocked** by session GitHub access), raw.githubusercontent.com (Brand Voice plugin README, read directly), and the MCP Registry API (live queries; this endpoint was reachable by curl).
- I didn't try WebFetch, since the brief says it's blocked. As a result, **no Etsy or Gumroad review or sales counts could be read**. Prices come from search-result snippets and some vary by regional storefront. Skool membership prices and promotion rules were not visible.
- Subreddit rules: only r/automation, via a third-party mirror (gummysearch), not the live sidebar. Everything else is NOT VERIFIED.
- Reddit evidence comes from mirror snapshots (reddit.sentinel-team.org, redlib).
- The Thumbtack-in-ChatGPT/Claude claim came from a search summary without a clearly attributed URL. It is treated as unverified and used only as context, not for scoring.
- There's a date conflict on the Claude for Small Business launch: 13 May 2026 in search results vs 15 Sep 2026 in candidates.md.

## Sources

- https://docs.vapi.ai/_fern-files/vapi.docs.buildwithfern.com/cf133005c62df7efa56a080a60422cbbf38e3d26974594187db228dccf935bd1/static/vapi-prompt-reference.md
- https://dental-voice-bot-kit.vercel.app/
- https://ciela.ai/agents/hvac-voice-receptionist
- https://ciela.ai/agents/dental-voice-receptionist
- https://ciela.ai/blogs/pre-built-ai-agent-templates-for-agencies
- https://ciela.ai/vs/vapi
- https://ciela.ai/vs/synthflow
- https://ciela.ai/blogs/vapi-vs-retell-reddit
- https://yashica.gumroad.com/l/voice-agent-prompts
- https://ashtonvossai.gumroad.com/l/ipjjqy
- https://zainulabideenbaloch.gumroad.com/l/cjnmds?layout=profile
- https://scalehatch.gumroad.com/
- https://franknillard.gumroad.com/l/ehovvt
- https://www.etsy.com/market/ai_receptionist
- https://www.etsy.com/market/ai_voice_agent_prompts
- https://www.etsy.com/market/ai_voice_agent_template
- https://www.etsy.com/au/listing/4539664221/hvac-ai-receptionist-deployment-kit
- https://www.etsy.com/listing/4300593201/plumbing-ai-receptionist-bot-virtual
- https://www.etsy.com/ca/listing/4373990675/ai-voice-agent-setup-guide-step-by-step
- https://www.skool.com/aivoicenetwork/about
- https://www.skool.com/voice-ai-mastery-5847
- https://chat.skool.com/voice-self-hosters
- https://www.skool.com/openautomation-collective-6267
- https://www.skool.com/voice-ai-wrapper-academy-3838
- https://www.upwork.com/services/product/admin-customer-support-build-ai-receptionist-for-hvac-plumbing-electrical-ai-calling-agent-2071660623106302895
- https://fiverr.com/simon_benedic/create-ai-receptionist-using-vapi-and-retell-ai
- https://gummysearch.com/r/automation/
- https://gummysearch.com/r/AI_Agents
- https://reddit.sentinel-team.org/posts/1tmpeq5/snapshots/2026-05-29T18%3A50%3A49.032229Z
- https://findskill.ai/blog/claude-for-small-business-setup-walkthrough/
- https://siliconangle.com/2026/05/13/anthropic-launches-claude-small-business-new-automation-workflows/
- https://www.digitalapplied.com/blog/claude-for-small-business-quickbooks-hubspot
- https://www.pulse.bot/ai/blogs/claude-for-small-business-the-practical-setup-guide-d39a3c45-9cbc-40f2-8de0-7f332b23732c/
- https://mikareyes.com/ai/how-to-setup-claude-for-small-business.md
- https://consulting.sva.com/insights/claude-for-small-business-how-to-connect-it-to-the-tools-you-already-use
- https://dev.to/akaranjkar08/claude-for-small-business-15-workflows-setup-guide-2026-4kak
- https://theusefultech.gumroad.com/l/cowork-mastery-guide
- https://intelligentsam5.gumroad.com/l/gvnzfh
- https://www.etsy.com/listing/4518427513/n8n-mcp-integration-handbook-claude-n8n
- https://redlib.hackliberty.org/r/softwaretesting/comments/1la9uc2/how_were_testing_ai_that_talks_back_and_sometimes
- https://insertchat.com/blog/ai-chatbot-testing-checklist-for-client-launch
- https://chatimize.com/chatbot-testing/
- https://getautonoma.com/blog/chatbot-testing-checklist
- https://fin.ai/learn/how-to-test-ai-agent-before-deployment
- https://www.testmuai.com/learning-hub/chatbot-hallucination/
- https://chipp.ai/docs/guides/understanding-evals.md
- https://hyperleap.ai/help/bot-studio/testing
- https://www.etsy.com/listing/4514447072/qa-test-plan-cases-checklist-templates
- https://www.etsy.com/listing/4391081115/software-go-live-checklist-template
- https://www.etsy.com/market/website_qa_checklist
- https://eye2on1ai.gumroad.com/l/ai-jailbreak-toolkit?layout=profile
- https://mbakry.gumroad.com/l/SafeguardPromptChecker-ContentComplianceAuditor
- https://raw.githubusercontent.com/anthropics/knowledge-work-plugins/main/partner-built/brand-voice/README.md
- https://www.etsy.com/market/brand_voice_guide
- https://www.etsy.com/market/brand_voice_template
- https://www.etsy.com/mx/market/ai_brand_voice_tool
- https://www.etsy.com/listing/4505875061/claude-ai-project-kit-for-content
- https://thesagocreator.gumroad.com/l/brandingos-claude
- https://aimastering.gumroad.com/l/claude-skill-bundle-content-and-Copywriting
- https://registry.modelcontextprotocol.io/v0/servers?search=plumb
- https://registry.modelcontextprotocol.io/v0/servers?search=hvac
- https://glama.ai/mcp/connectors/dev.sunrays.mcp/sunrays-local-service-booking
- https://mcpservers.org/servers/qasper-ai-mcp
- https://implexa.ai/s/clawhub/lokuli-skills
- https://studiomeyer.io/en/services/custom-mcp-server
- https://www.searchenginejournal.com/google-ai-mode-adds-agentic-booking-expands-to-more-countries/554345/
- https://www.nearmedia.co/local-agents-alexas-do-over-google-dark-ad-patterns-reviewpocalypse/
- Phase 1 files: research/phase1/ai-ecosystem-gaps.md (G6, G7, G9, G10, G11), marketplace-saturation-scout.md (rows 27, 48, 49), trend-scout.md (#3, #14, #18), regulation-and-platform-shifts.md (#6, chatbot-liability row), pain-hunter.md (#3, #29)
