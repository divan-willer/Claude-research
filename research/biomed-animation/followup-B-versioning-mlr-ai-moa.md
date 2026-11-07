# Follow-up: Versioning/localisation of MoA masters, MLR provenance, and AI-MoA competitors

Follow-up researcher B. Date: 7 November 2026. Method: 35 WebSearch queries (the hard cap). No page was opened, because WebFetch is blocked in this environment. Every fact below comes from a search-result summary and is marked "(snippet)". Where a summary merged several pages and I could not tell which page a number came from, I say so.

## Bottom line

- **The "32.4 days for video" figure now has a source, but it is a vendor figure.** Vodori's own blog cites it from its "2025 State of Promotional Review Benchmarks Report". It is defined as "start to approval", not review time. Animation is not broken out ([Vodori](https://www.vodori.com/blog/pharma-digital-marketing-mlr-review), snippet). This is stronger than the track-2 fact-check assumed. It is still one vendor's benchmark.
- **Veeva already does frame-level claim linking on video, and it bought an AI-MLR start-up in 2026.** PromoMats supports claim links and reference anchors placed on a chosen video frame ([Veeva support](https://support.veeva.com/hc/en-us/articles/360002742354-How-to-Annotate-a-Video-in-PromoMats-and-Medical), snippet). Veeva bought Copli on 23 June 2026 and relaunched it as Falcon MLR, with automatic claim anchoring ([Veeva](https://www.veeva.com/jp/resources/veeva-acquires-copli-launches-veeva-falcon-mlr-to-accelerate-content-review/), snippet). A Claims Agent was listed for August 2026 ([Veeva APAC](https://www.veeva.com/ap/?p=254118), snippet). Claim-level provenance for MLR is owned by Veeva.
- **An AI-MoA competitor already sells "provenance".** VarsaAI is an AI mechanism-of-action platform. It offers sentence-level referencing, a patent-pending "VeriCore" verification system and a full MLR audit trail. It is sold through a healthcare agency, GW Health (June 2026) ([PR.com](https://www.pr.com/press-release/971739), snippet). Powtoon's Visual Pharma "MOA Studio" (beta) was an LTEN 2026 finalist and is "built to align with Veeva-based workflows" ([AI Journal](https://aijourn.com/visual-pharma-by-powtoon-named-lten-excellence-awards-finalist-for-moa-studio-advancing-compliant-ai-powered-scientific-communication/), [Powtoon](https://www.powtoon.com/solution/visual-pharma), snippet). Neither shows a public price.
- **Flat-video localisation is a scaled, cheap commodity.** Synthesia is valued at USD 4B with about USD 140–150M ARR, and Inizio Medical has been a certified Synthesia provider since March 2024. HeyGen reports more than USD 200M ARR; ElevenLabs had more than USD 330M at the end of 2025. Per-language add-ons from studios and vendors run about USD 500–1,500, or 15–20% of the film's base price. So any versioning offer that works only on the finished video has no moat.
- **The large content-operations firms are growing and moving into localisation and MLR.**
  - Indegene: FY26 revenue INR 35,105m (USD 396.9m), up 23.6% in INR; Q2 FY27 up 39.5% in INR and 27.5% in USD ([NSE](https://nsearchives.nseindia.com/corporate/INDEGENE_29042026203956_Intimation_of_Press_Release.pdf), [Investywise](https://www.investywise.com/indegene-reports-strong-q2-fy27-financial-results/), snippet).
  - ZS: launched ZAIDYN Content (generation, reuse, localisation, MLR) on 19 May 2026.
  - IQVIA: launched IQVIA.ai on 16 March 2026, which it says 19 of the top 20 pharma companies are integrating.
- **Verdict, gap (a), versioning of 3D masters: weakened.** As a pharma-facing SaaS it is mostly owned or blocked. The one part no competitor I found covers is 3D-native work: re-timing from the source scene and swapping on-screen labels inside the scene. That part survives as a studio-side tool or white-label service. The evidence for it is thin:
  - Label updates mostly change text (ISI and claims), not the 3D mechanism.
  - The bottleneck is local re-review, not rendering. In Veeva's 2026 MedTech benchmark, 64% name local regulatory re-review as the main barrier.
  - Confidence: medium.
- **Verdict, gap (b), reference-annotated, provenance-tracked scenes: weakened.** The claim and document level is taken by Veeva (anchors, Claims Agent, Falcon MLR), Aprimo, Solstice (USD 21M Series A, May 2026) and VarsaAI. What is left is provenance at the asset level inside the 3D tool: which PDB entry or paper a structure, its scale or its colour came from, exported as anchors into PromoMats. That works as a feature of a validated 3D asset library (the track 3/5 library gaps), not as a standalone product. Confidence: medium.
- **Who pays first (inference, confidence low–medium):** small and mid-size medical-animation studios, and healthcare or MedComms agencies that hold the source scene files. They would pay per derivative, probably in the range of about USD 1,500–6,000 per language or format version of a 2–3 minute MoA. That is set by today's per-language add-ons and the 15–20%-of-base rule of thumb. Pharma brand teams are unlikely first buyers: they buy through agencies and Veeva.

## Findings

### Q1. Competitors and substitutes

**Powtoon Visual Pharma / MOA Studio**
- A DIA exhibitor listing calls MOA Studio a "(Beta)" capability that "visualize[s] drug interactions, MoAs and AEs in a scientifically accurate manner" ([DIA](https://live.diaglobal.org/event/medical-affairs-and-scientific-communications-forum-1/exhibitor/RXhoaWJpdG9yXzI0MjE5NTk=), snippet).
- An April 2026 release says Visual Pharma by Powtoon was a 2026 LTEN Excellence Awards finalist for MOA Studio, described as a "compliant AI-powered workflow" ([AI Journal](https://aijourn.com/visual-pharma-by-powtoon-named-lten-excellence-awards-finalist-for-moa-studio-advancing-compliant-ai-powered-scientific-communication/), snippet).
- Powtoon's pharma page places MOA Studio in its "Create" tier, next to Anything-to-Video, and says the product is "built to align with Veeva-based workflows". That is a compatibility claim; I found no Veeva-side integration ([Powtoon](https://www.powtoon.com/solution/visual-pharma), snippet).
- No Visual Pharma price was found. Generic Powtoon plans list at USD 49–199 a month, with custom enterprise pricing and no API ([SoftwareFinder](https://softwarefinder.com/design-software/powtoon), snippet).
- A summary site claims production falls "from weeks to hours" and saves "tens of thousands of dollars per video". This is unsourced ([BriefGlance](https://briefglance.com/articles/ai-tool-slashes-pharma-video-production-from-weeks-to-hours), snippet).

**VarsaAI**
- VarsaAI calls itself "an AI mechanism-of-action platform built for pharmaceutical, biotechnology, and medical affairs teams". It makes MoA presentations and videos.
- GW Health, a life-sciences communications agency, partnered with it so that GW Health's clients get "compliant… MOA and mechanism-of-disease content in minutes rather than weeks".
- The release cites a "patent-pending VeriCore™ scientific verification system, sentence-level referencing, and a full MLR audit trail". Datelines conflict: Cannes, 22 June 2026, and Jersey City, 30 June 2026, the latter marked as a paid release ([PR.com](https://www.pr.com/press-release/971739), [WebDisclosure](https://www.webdisclosure.com/press-release/gw-health-strengthens-strategic-communications-offering-with-ai-partnership-UuemjkZTxVB), snippet).
- A ChatGPT app listing says it checks text sentence by sentence against PubMed, openFDA and the client's approved reference library ([ChatGPT app listing](https://chatgpt.com/plugins/plugin_asdk_app_6a68f179b5248191b1c50b3b675e0dc4), snippet). Capterra describes it as a verification layer that checks each sentence against approved sources ([Capterra](https://www.capterra.in/software/1311677/VarsaAI), snippet).
- Track 1 already cited its "12 minutes, not 12 weeks" claim.
- I found no price, no funding, and nothing on whether its video is 3D.
- Inference (confidence: medium): VarsaAI already sells the "provenance for MLR" idea, at the level of text and script, inside the MoA niche, through agencies. It is the closest direct competitor to gap (b).

**Leadde.ai**
- Leadde has an AI "pharmacology animation" product with a free tier that needs no card ([Leadde](https://leadde.ai/solutions/pharmacology-animation), snippet).
- It claims SOC 2, ISO 42001 and GDPR compliance ([Leadde](https://leadde.ai/ko/tools/ai-pharma-video-maker), snippet).
- Paid prices were not visible.

**Synthesia and Inizio Medical**
- The search summary dates the partnership to March 2024: Inizio Medical became a "recommended Synthesia provider" ([Inizio](https://inizio.com/insights/inizio-medical-partners-with-synthesia-to-unlock-ai-powered-video-creation-for-healthcare-at-scale/), [Synthesia](https://www.synthesia.io/service-providers/inizio-medical), snippet). This fills in the date that track 4 left blank.
- Synthesia's case study on MEDiSTRAVA, an Inizio unit, covers AI video in "50+ languages for medical communication" ([Synthesia](https://www.synthesia.io/case-studies/medistrava), snippet).
- In July 2025, Inizio made 17 MS patient case-study videos for HCPs using AI avatars. The work took six weeks against a usual four months or more ([Inizio](https://inizio.com/insights/ai-avatars-for-hcp-engagement/), snippet). The tool is not named.
- Synthesia corporate facts:
  - USD 200M Series E at USD 4B (January 2026) ([TechCrunch](https://techcrunch.com/2026/01/26/synthesia-hits-4b-valuation-lets-employees-cash-in), snippet).
  - ARR about USD 146M in September 2025 (Sacra estimate), about USD 140M disclosed by the company in February 2026 ([Sacra](https://sacra.com/research/synthesia), snippet).
  - About 70% of revenue from enterprise; typical large accounts pay USD 2,000–10,000 a month (Sacra).
  - SpendHound's sample of 34 enterprise customers averages USD 208,741 a year ([SpendHound](https://www.spendhound.com/marketplace/synthesia-pricing), snippet).
  - Merck is a named customer.
- Scope caveat (as track 4 noted): this is presenter and avatar video, not 3D MoA.

**HeyGen, ElevenLabs, Rask and AI-dubbing vendors**
- HeyGen reported passing USD 200M ARR in June 2026 ([YesPress](https://yespress.io/heygen), snippet). Sacra estimated USD 95M in September 2025 ([Sacra](https://sacra.com/research/heygen/), snippet). Video translation is an add-on or a higher-tier feature.
- ElevenLabs closed 2025 with "over USD 330 million in ARR" ([ElevenLabs](https://elevenlabs.io/blog/series-d), snippet). Sacra estimates about USD 500M in April 2026 ([Sacra](https://sacra.com/research/elevenlabs), snippet). Enterprise terms include BAAs for HIPAA customers. Dubbing draws on a shared credit pool.
- I found no named healthcare dubbing customer for HeyGen or ElevenLabs, and no Rask result.
- Language-service vendors sell AI dubbing to pharma with human and MLR review on top:
  - Smartcat ([Smartcat](https://www.smartcat.com/pharmacy-translation/digital-marketing-agency))
  - VerboLabs ([VerboLabs](https://www.verbolabs.com/?p=27842))
  - Wavel ([Wavel](https://wavel.ai/industry/pharmaceutical-videos))
  - Interpro (2026: "AI drafts, humans remain accountable"; wording can change between US and EU MDR) ([Interpro](https://www.interproinc.com/video-localization-fails-healthcare-examples/))
  - Vistatec (2026 case study: AI-assisted subtitling for a device maker) ([Vistatec PDF](https://www.vistatec.com/wp-content/uploads/2026/06/Case-Studies_Vistatec-Streamlines-Global-Video-Subtitling-for-a-Medical-Device-Manufacturer.pdf))
  - translate.video (75+ languages) ([translate.video](https://translate.video/pharmaceuticals/translate-pharma-training-videos-into-75-languages))
  - All snippet.

**Veeva (PromoMats, AI agents, Copli / Falcon MLR)**
- Veeva AI Agents for Vault CRM and PromoMats were announced as available on 4 December 2025 (search summary; page attribution likely [Veeva news](https://www.veeva.com/ap/?p=253815), snippet).
- Released standard agents: Quick Check Agent (pre-MLR checks against editorial, brand, market, channel and compliance rules) and Content Agent ([Veeva KR](https://www.veeva.com/kr/products/veeva-ai-for-promomats/), snippet).
- A Claims Agent ("identify and substantiate claims and maintain the Claims Library") and custom agents were listed for August 2026 ([Veeva APAC](https://www.veeva.com/ap/?p=254118), snippet).
- Veeva bought Copli, a Danish agentic-MLR company, on 23 June 2026 and relaunched it as Veeva Falcon MLR. It claims Falcon MLR could remove "70% or more of manual MLR labor within five years". The price was not disclosed ([Veeva](https://www.veeva.com/jp/resources/veeva-acquires-copli-launches-veeva-falcon-mlr-to-accelerate-content-review/), [StreetInsider/PRN](https://www.streetinsider.com/PRNewswire/Veeva+Acquires+Copli%2C+Launches+Veeva+Falcon+MLR+to+Accelerate+Content+Review/26675730.html), [Signalbase](https://www.trysignalbase.com/news/acquisitions/copli-acquired-by-veeva-systems-acquisition), snippet).
- A third-party write-up names "automatic claim anchoring to approved references" as a key Copli feature ([BriefGlance](https://briefglance.com/articles/veevas-ai-gambit-agentic-mlr-aims-to-remake-life-sciences-compliance), snippet).
- Veeva's 2026 MLR paper says PromoMats and Falcon MLR together cover "content ideation, review, localization, and approval" ([Veeva PDF Jul 2026](https://www.veeva.com/wp-content/uploads/2026/07/Modernize-MLR-with-AI.pdf), snippet).
- I found no Veeva AI agent that generates video.

**Adobe GenStudio and Aprimo**
- I found no GenStudio material specific to life sciences.
- Adobe says it "can integrate with Veeva and other MLR tools" ([Adobe partners](https://partners.adobe.com/digitalexperience/industries/healthcare-life-sciences), snippet). The Adobe–Veeva partnership dates from 2021 ([Adobe blog](https://blog.adobe.com/en/publish/2021/07/01/adobe-veeva-partner-personalize-digital-life-sciences-experience), snippet) [pre-2024].
- Aprimo markets "claims traceability" and global-to-local adaptation "without… losing alignment to approved claims and references" ([Aprimo](https://www.aprimo.com/solutions/industries/life-sciences), [Aprimo](https://www.aprimo.com/solutions/industries/solutions-industries-life-sciences-new), snippet).

**Indegene**
- FY26 (year to 31 March 2026, reported 29 April 2026):
  - Revenue INR 35,105m (USD 396.9m), up 23.6% in INR and 18.2% in USD, from INR 28,393m.
  - Q4 INR 10,034m, up 32.8%.
  - Adjusted EBITDA INR 6,793m (19.4%).
  - Source: [NSE press release](https://nsearchives.nseindia.com/corporate/INDEGENE_29042026203956_Intimation_of_Press_Release.pdf), snippet. This confirms the track-2 figures at snippet level.
- Profit after tax fell 1.4% to INR 4,011m ([Whalesbook](https://www.whalesbook.com/corporate-news/English/tech/Indegene-FY26-Revenue-Climbs-236percent-PAT-Falls-Amid-Client-Growth/69f2351008235f0c2a1bd2ab), snippet). 53 clients each pay more than USD 1m a year ([Investywise](https://www.investywise.com/?p=77795), snippet).
- Q2 FY27 (to 30 September 2026):
  - Revenue INR 11,223m, up 39.5% in INR and 27.5% in USD (about USD 117.5m).
  - EBITDA margin 16.7%.
  - Mix: Enterprise Commercial about 71%, Enterprise Medical 25%.
  - 59 clients above USD 1m, 13 above USD 10m.
  - Management cited a "global digital content management deal for a top 30 pharma company" and wins in GenAI-enabled transformation.
  - Sources: [Investywise](https://www.investywise.com/indegene-reports-strong-q2-fy27-financial-results/), [Investywise transcript](https://www.investywise.com/indegene-q2-fy27-earnings-transcript-highlights-growth-strategic-wins/), [Sahi](https://www.sahi.com/news/indegene-reports-q2-revenue-of-11-22-billion-versus-8-04-billion-yoy), snippet.
  - Profit growth is reported as both 10% and 22.7%. The sources conflict.

**IQVIA and ZS**
- IQVIA.ai launched on 16 March 2026 with Nvidia. "19 of the top 20" pharma companies had begun integrating IQVIA agents ([Let's Data Science](https://letsdatascience.com/news/iqvia-launches-iqviaai-agentic-ai-platform-with-nvidia-b1ca210d), snippet).
- IQVIA's service pages describe agents that "rapidly create on-brand content variations and navigate the MLR review process". Its July 2026 blog says MLR teams must review more volume at the same standard ([IQVIA blog](https://www.iqvia.com/blogs/2026/07/from-automation-to-oversight), snippet).
- ZS launched ZAIDYN Content on 19 May 2026, covering "content generation, personalization, reuse, localization, and MLR review", with a Content MLR Accelerator ([ZS](https://www.zs.com/about/newsroom/zs-launches-agentic-ai-products-zaidyn-medical-and-zaidyn-content), [Consulting Report](https://www.theconsultingreport.com/zs-expands-zaidyn-platform-with-agentic-ai-applications-for-regulated-life-sciences-workflows/), snippet).
- Neither showed video-specific capability.

**AI-MLR and claims start-ups launched or funded in 2025–2026**
- Solstice raised a USD 21M Series A (28 May 2026, led by Transformation Capital; about USD 25M in total). Its workflow covers "content creation, claim substantiation, MLR pre-check, Veeva submission". It claims MLR rounds fall from 3.2 to 1.2 ([HIT Consultant](https://hitconsultant.net/2026/05/28/solstice-raises-21m-series-a-pharma-mlr-ai/), [ContentGrip](https://www.contentgrip.com/solstice-series-a-pharma-mlr/), snippet; vendor claim).
- Revisto (USD 4M seed) is named as a comparable ([NewMarketPitch](https://newmarketpitch.com/blogs/news/solstice-series-a-analysis), snippet).
- I found no funded start-up dedicated to AI video or 3D MoA beyond VarsaAI, Powtoon's unit and Leadde.
- One search returned an unrelated "Varya" video model from Avataar, priced at USD 0.005 per generated second ([TNW](https://thenextweb.com/news/avataar-ai-varya-video-model-india-cheap), snippet). It is relevant only as a sign that generic AI video is becoming a commodity.

**Signals from studios and guides**
- An AI-video guide says generated video suits MoA, disease education and HCP training. It also says "the branded launch asset that carries regulated claims still belongs with a studio" ([AITuber](https://aituber.app/blog/pharma-video-marketing/), snippet).
- AXS3D says "No AI" clauses are rising in biotech animation contracts ([AXS3D 2026](https://axs3d.com/blog/future-of-biotech-animation-2026/), snippet; studio claim, no contract text).

### Q2. How MoA films are versioned and localised today

**Facts on prices and practice (all vendor list prices, snippet)**
- Per-language add-ons:
  - An explainer studio's package sheet: translated voiceover USD 1,500 per language; translated subtitles USD 500 per language ([Explainify PDF](https://explainify.com/wp-content/uploads/2022/08/Animated_Explainer_Packages.pdf)) [pre-2024].
  - A medical-animation cost guide: budget another 15–20% of the base price for each extra language (likely [Prolific cost guide](https://prolificstudio.co/?p=30191); [Podymos](https://podymos.com/learning-center/medical-animation-cost) was in the same result set, so attribution is unconfirmed).
  - A voice-translation vendor: USD 850 per language (likely [Contra listing](https://contra.com/s/sbEEXk72-ai-video-translation-voice-cloning-across-languages); unconfirmed).
- How languages are sold:
  - Some medical-animation sellers include one language in the base package and charge for others ([Fiverr](https://fiverr.com/fcreativeteam/clear-medical-animations-for-patient-understanding)).
  - A Dublin studio's portfolio shows re-versioning of an existing film into five extra languages as a project in its own right ([Production Attic](https://www.dublin.productionattic.com/portfolio/ddimertranslation)).
- Base prices for reference: MoA films USD 25,000–75,000 for 2–3 minutes (one pricing source; page among results for [AITuber](https://aituber.app/blog/pharma-video-marketing/) and Prolific pages, unconfirmed). Studio rates USD 5,000–20,000 per finished minute ([VOKA](https://voka.io/medical-animation-cost/)).
- A vendor claims traditional localisation took "4–6 weeks per language" (source page unconfirmed among the [translate.video](https://translate.video/pharmaceuticals/translate-pharma-training-videos-into-75-languages) and [Viseven](https://viseven.com/best-practices-content-localization/) results).

**Facts on how many markets and how much reuse**
- Veeva's 2026 MedTech benchmark, which covers device companies, not pharma: 74% use "a global core with a local adaptation model"; 64% say "local regulatory re-review remains the primary barrier" ([Veeva MedTech 2026 PDF](https://www.veeva.com/medtech/wp-content/uploads/2026/07/2026-MedTech-Commercial-Content-Benchmark-Report-1.pdf), snippet).
- A LinkedIn post attributes to Veeva the figure that only 9% of global pharma assets are reused in local markets ([LinkedIn](https://es.linkedin.com/in/kieran-fairnington), snippet). This is weak, second-hand evidence.
- A Reuters Events speaker cites 60–70% of pharma content never reaching a customer and a six-month lag between global and affiliate teams ([Reuters Events](https://www.reutersevents.com/pharma/node/63059), snippet; speaker claim; page attribution between this and the [content-ops article](https://events.reutersevents.com/pharma/article/optimize-content-operations) unconfirmed).
- I found no source giving the number of languages or markets for a typical global MoA film.

**Facts on how often labels change**
- A 2017 BMJ analysis found 0.94 safety-related label changes per drug per year for expedited-pathway drugs, against 0.68 for others ([PMC5588044](https://pmc.ncbi.nlm.nih.gov/articles/PMC5588044), snippet) [pre-2024].
- A study of 278 novel drugs (2002–2014) recorded 703 label updates. Another found that 88.5% of new therapeutic biologics had at least one safety update. Snippets do not show which of [PMC8159207](https://pmc.ncbi.nlm.nih.gov/articles/PMC8159207), [PMC6013049](https://pmc.ncbi.nlm.nih.gov/articles/PMC6013049) and [Drug Safety 2021](https://link.springer.com/article/10.1007/s40264-021-01142-3) each figure comes from [pre-2024].
- FDA's Safety-related Labeling Changes database covers changes from 2016 onward ([FDA](https://www.fda.gov/drug-safety-labeling-changes), snippet).
- Promotional animations must carry footnotes citing the literature behind their claims ([Mechanism Digital](https://mechanismdigital.com/post/footnotes-and-fair-balance), snippet).

**Who does the work (synthesis of snippets plus the track reports)**
- The original studio does re-cuts.
- Language-service providers and AI-dubbing vendors do voiceover and subtitles.
- Content-operations firms (Indegene, IQVIA, ZS, Publicis Sapient Bodhi) handle global-to-local adaptation.
- Chasing Illusions (track 5) versioned one master into 12+ Indian languages with AI voice.

**Inferences**
- Confidence medium: most label-driven changes to an MoA film are text changes (indication wording, ISI or fair-balance end cards, on-screen claims, footnotes). They are composited 2D overlays, not 3D re-renders. A drug's mechanism rarely changes with a safety update. That shrinks the "label-update re-render" market.
- Confidence low–medium: in-scene 3D labels (text attached to a structure in the scene) and re-timing to a new voiceover length are the parts that need the source scene. Flat-video AI tools cannot do these well. No competitor I found addresses them. But only the studio that holds the scene files can do the work, so the natural buyer is the studio, or an agency that owns the files.

### Q3. Video in MLR review, and tools that link assets to claims

**Facts on review time**
- Vodori's blog quotes its 2025 State of Promotional Review Benchmarks Report: "Video content averages 32.4 days from start to approval". Email averages 18.8 days. Time to incorporate feedback: website 13.2 days, social 4.7 days, event materials 4.1 days ([Vodori](https://www.vodori.com/blog/pharma-digital-marketing-mlr-review), snippet).
- Another Vodori post: the 2024 average was about 13.8 days, and "some content types, like videos, tend to take longer due to their complexity". The 2025 industry average job duration was 14.8 days. Teams making more than five process changes a quarter reach a median of 5.5 days, against 9.9 days for teams making fewer than one ([Vodori](https://www.vodori.com/blog/process-iteration-the-secret-to-top-performing-mlr-processes), snippet; exact page for each figure unconfirmed).
- Vodori (May 2022): video is harder to review because reviewers must assess "the voiceover, in-video graphics, and even the in-frame action". Its Pepper Flow product has video annotation tools ([Vodori 2022](https://vodori.com/blog/4-tips-to-improve-video-feedback-during-mlr-review), snippet) [pre-2024].
- Other clocks:
  - Veeva (2023 data): US days in review fell by more than 25% to 16 ([Veeva](https://www.veeva.com/?p=93099), snippet) [pre-2024 data].
  - Klick cites Veeva's 2021 Pulse report (21 days to approval, 74% first-cycle approval) [pre-2024] and EY 2024 (24 days) ([Klick](https://idx.klick.com/articles/from-checkpoint-to-input-a-different-model-for-mlr), snippet).
- No source breaks out animation or MoA separately.
- Status of the 32.4-day claim: the attribution is now found on Vodori's own domain at snippet level. The definition is "start to approval", which includes revision time. It is a vendor benchmark, and Vodori sells review software. Not verified against the report itself.

**Tools that link video or assets to claims and references**
- **Veeva PromoMats video annotation.**
  - Three annotation types on video: comment, link, and claim link (where configured). The user pauses on a frame and places the link ([Veeva support](https://support.veeva.com/hc/en-us/articles/360002742354-How-to-Annotate-a-Video-in-PromoMats-and-Medical), snippet).
  - Reference anchors ("Link to Content") are also placed on a chosen frame ([Veeva support](https://support.veeva.com/hc/en-us/articles/29795579004059-How-to-Link-Anchors-to-the-Content-on-a-Video-in-PromoMats-and-Veeva-Medical), snippet).
  - When annotations are brought forward to a new version, they keep their timestamps. If a timestamp no longer exists because the video length changed, the annotation moves to 00:00 with an alert icon. Source: summary of the Veeva support set; the exact page is either the anchors article above or the [bring-forward article](https://support.veeva.com/hc/en-us/articles/4402585274395-Why-Bring-Forward-Annotations-is-Not-Visible-for-Video-Annotations-in-PromoMats-and-Medical).
  - Auto-created links become "Approved Link" annotations, whose references cannot be moved or edited.
  - Veeva marketing cites "80% claims auto-linked" (vendor claim; page unconfirmed, [Veeva claims management](https://www.veeva.com/products/veeva-promomats/claims-management/)).
- **Veeva Claims Agent** (listed for August 2026) and **Falcon MLR / Copli** (automatic claim anchoring), as above.
- **Aprimo**: claims traceability and global-to-local alignment (above).
- **Vodori Pepper Flow**: annotation and comments on video (above).
- **Solstice**: claim substantiation and a pre-review score before submission to Veeva (above).
- **VarsaAI**: sentence-level referencing and an MLR audit trail for MoA content (above).
- I found no tool that links a 3D scene element or asset inside the 3D software (a protein, a cell, a scale choice) to a reference and carries that link through to PromoMats.

**Inferences**
- Confidence medium: re-cutting an approved video (a 15-second cut-down, a re-timed language version) breaks the frame-based claim anchors in PromoMats. They land at 00:00 and must be placed again by hand. That is a real but small friction. A tool that exports a timed list of claims and anchors from the edit or scene, for each derivative, would fix it. But it sits on Veeva's surface, and Veeva can close the gap with a feature.
- Confidence medium: the "provenance" gap left for a small team is upstream, at the level of the asset or shot in production. It is not at the claim level, which Veeva, Aprimo, Solstice and VarsaAI cover.

### Q4. Real-time and interactive 3D MoA (rep iPads, HCP portals, congress booths)

**Facts**
- Veeva CLM's media player handles PDF detail aids, HTML5 interactive apps and video ([IntuitionLabs](https://intuitionlabs.ai/articles/veeva-clm-pharma-marketing-guide), snippet). I found no source on WebGL or 3D performance inside the CLM app.
- Viscira's vDetail for Veeva iRep advertised "real-time 3D content" more than a decade ago ([PRWeb](https://www.prweb.com/releases/viscira_enhances_veeva_irep_with_its_version_2_0_vdetail_solution/prweb10955027.htm), snippet) [pre-2024]. Interactive 3D on the rep iPad is not new.
- An industry overview says MoA visuals in interactive aids are usually "pre-rendered animations with interaction triggers; some real-time" ([TechnoLynx](https://technolynx-site.pages.dev/post/interactive-visual-aids-in-pharma-driving-engagement), snippet).
- AXS3D builds interactive apps in-house in Toronto. "One app… can be deployed to your congress booth, your website, and tablets". Prices are quoted on request ([AXS3D](https://axs3d.com/services/medical-scientific-interactive-apps-conference-experiences/), [AXS3D Interactive MOA for Booth and Browser](https://axs3d.com/?p=17081), snippet).
- Random42 (ESMO 2025) offers touchscreen or iPad interactive experiences and mixed-reality headsets ([Random42](https://random42.com/company-news/esmo-2025), snippet).
- VOKA sells touchscreen kiosks with manipulable 3D ([VOKA](https://voka.io/medical-booth-ideas-for-pharma/), snippet).
- Inizio:
  - ASCO 2025: LED walls with interactive MoA walkthroughs, and a quiz that could be reconfigured between days ([Inizio](https://inizio.com/insights/real-time-strategy-at-asco25/), snippet).
  - ASH: a rare-disease MoA installation on a 15' × 11' LED wall showing a "3D room of blood cells", with close to 1,000 unique sessions over three days ([Inizio](https://inizio.com/insights/moa-congress-engagement/), snippet).
- Viseven eWizard publishes to Veeva CRM, CLM and PromoMats. Its pricing (per account, team or seat) is on request, and I found no 3D evidence ([eWizard pricing](https://ewizard.io/pricing), [G2](https://www.g2.com/products/viseven-ewizard/pricing), snippet).
- BioDigital sells licensed 3D anatomy to pharma as "cost effective" ([BioDigital](https://www.biodigital.com/customers/pharma), snippet).
- No price for any interactive 3D MoA app, portal module or booth piece was found.

**Inference (confidence medium):** established studios and agencies (AXS3D, Random42, VOKA, Inizio, Emota from track 5) already deliver interactive MoA across booth, web and iPad. Much of it is pre-rendered video with triggers. Nothing here shows buyer pain about converting rigs to real time. Track 5's Gap 2 is neither helped nor hurt by this; it is still unpriced.

## Competitors and substitutes found

| Name | Offering | Price | Model | Date of evidence | URL |
|---|---|---|---|---|---|
| Powtoon Visual Pharma: MOA Studio | AI MoA video workflow (beta) for medical affairs; claims Veeva-aligned workflow | Not public; Powtoon generic USD 49–199/mo, enterprise custom | SaaS, enterprise | Apr 2026 (LTEN finalist) | https://aijourn.com/visual-pharma-by-powtoon-named-lten-excellence-awards-finalist-for-moa-studio-advancing-compliant-ai-powered-scientific-communication/ |
| VarsaAI | AI MoA and MoD presentations and videos; VeriCore verification, sentence-level references, MLR audit trail | Not found | SaaS, resold via agencies (GW Health) | Jun 2026 | https://www.pr.com/press-release/971739 |
| Leadde.ai | AI "pharmacology animation" and pharma video maker | Free tier; paid tiers not visible | Self-serve SaaS | 2026 (undated pages) | https://leadde.ai/solutions/pharmacology-animation |
| Synthesia (with Inizio Medical) | AI avatar and presenter video, translation; Inizio is a certified provider; MEDiSTRAVA 50+ languages | Large accounts USD 2–10k/mo (Sacra); average enterprise USD 208,741/yr (SpendHound, n=34) | SaaS; agency partner channel | Mar 2024 (partnership); Jan 2026 (USD 4B round) | https://www.synthesia.io/case-studies/medistrava |
| HeyGen | AI avatar video and video translation | Add-on or higher tier; enterprise custom | SaaS | Jun 2026 (more than USD 200M ARR, company-reported) | https://yespress.io/heygen |
| ElevenLabs | Voice, dubbing (Dubbing v2), BAAs for HIPAA | Credit pool; enterprise custom | SaaS / API | Dec 2025 (more than USD 330M ARR); Sep 2026 SKUs | https://elevenlabs.io/blog/series-d |
| Smartcat, VerboLabs, Wavel, Interpro, Vistatec, translate.video | AI dubbing and subtitles for pharma and medtech, with human or MLR review | Not found | LSP / SaaS | 2026 | https://www.interproinc.com/video-localization-fails-healthcare-examples/ |
| Veeva PromoMats + AI agents | Frame-level video claim links and anchors; Quick Check, Content, Claims (Aug 2026) agents; DAM; modular content | Enterprise licence (not found) | Platform SaaS | Dec 2025 – Aug 2026 | https://www.veeva.com/ap/?p=254118 |
| Veeva Falcon MLR (ex-Copli) | Agentic MLR review; automatic claim anchoring | Not disclosed | Add-on to PromoMats | 23 Jun 2026 (acquisition) | https://www.veeva.com/jp/resources/veeva-acquires-copli-launches-veeva-falcon-mlr-to-accelerate-content-review/ |
| Aprimo (life sciences) | DAM and content operations with claims traceability and global-to-local adaptation | Not found | SaaS | 2026 (undated page) | https://www.aprimo.com/solutions/industries/life-sciences |
| Adobe (GenStudio / Experience) | Content supply chain; integrates with Veeva | Not found | SaaS | 2021 partnership [pre-2024]; no 2026 life-sciences evidence | https://partners.adobe.com/digitalexperience/industries/healthcare-life-sciences |
| Indegene | Commercial and medical content operations; GenAI transformation | Services | Outsourcer (listed in India) | FY26 (Apr 2026), Q2 FY27 (Oct–Nov 2026) | https://nsearchives.nseindia.com/corporate/INDEGENE_29042026203956_Intimation_of_Press_Release.pdf |
| IQVIA.ai | Agentic platform; content variations; MLR navigation | Not found | Platform + services | 16 Mar 2026 | https://letsdatascience.com/news/iqvia-launches-iqviaai-agentic-ai-platform-with-nvidia-b1ca210d |
| ZS ZAIDYN Content | Content generation, reuse, localisation, MLR accelerator | Not found | Platform + consulting | 19 May 2026 | https://www.zs.com/about/newsroom/zs-launches-agentic-ai-products-zaidyn-medical-and-zaidyn-content |
| Solstice | AI-native pharma marketing: creation, claim substantiation, MLR pre-check, Veeva submission | Not found (USD 21M Series A) | SaaS | 28 May 2026 | https://hitconsultant.net/2026/05/28/solstice-raises-21m-series-a-pharma-mlr-ai/ |
| Revisto | AI MLR platform | Not found (USD 4M seed) | SaaS | 2026 (analysis blog) | https://newmarketpitch.com/blogs/news/solstice-series-a-analysis |
| Vodori Pepper Flow | Promotional review, with video annotation | Not found | SaaS | 2022 blog [pre-2024]; 2025 benchmarks | https://vodori.com/blog/4-tips-to-improve-video-feedback-during-mlr-review |
| Viseven eWizard | Modular eDetailing and CLM content authoring; publishes to Veeva | On request (per account, team or seat) | SaaS + agency | Mar 2025 release; 2026 pages | https://ewizard.io/pricing |
| AXS3D, Random42, VOKA, Inizio, Emota | Custom interactive 3D MoA for booth, web and iPad; XR | Quote on request | Studio / agency | 2025–2026 | https://axs3d.com/services/medical-scientific-interactive-apps-conference-experiences/ |
| Avataar Varya | Low-cost generic AI video model (sign of commoditisation only) | USD 0.005 per generated second | API | Jun 2026 | https://thenextweb.com/news/avataar-ai-varya-video-model-india-cheap |

## Price points

| Item | Price | Currency / year | List or deal | URL |
|---|---|---|---|---|
| Translated voiceover add-on (explainer studio) | 1,500 per language | USD, 2022 [pre-2024] | List | https://explainify.com/wp-content/uploads/2022/08/Animated_Explainer_Packages.pdf |
| Translated subtitles add-on (explainer studio) | 500 per language | USD, 2022 [pre-2024] | List | https://explainify.com/wp-content/uploads/2022/08/Animated_Explainer_Packages.pdf |
| Extra language on a medical animation | 15–20% of base price per language | USD-relative, c. 2025–26 | List rule of thumb (page attribution unconfirmed) | https://prolificstudio.co/?p=30191 |
| AI voice translation per language (vendor) | 850 per language | USD, c. 2026 | List (page attribution unconfirmed) | https://contra.com/s/sbEEXk72-ai-video-translation-voice-cloning-across-languages |
| MoA film, 2–3 minutes | 25,000–75,000 | USD, c. 2026 | List (page attribution unconfirmed) | https://aituber.app/blog/pharma-video-marketing/ |
| Studio medical animation per finished minute | 5,000–20,000 | USD, 2025–26 | List | https://voka.io/medical-animation-cost/ |
| Synthesia large-account spend | 2,000–10,000 per month | USD, 2025–26 | Analyst estimate | https://sacra.com/research/synthesia |
| Synthesia average enterprise contract | 208,741 per year (n=34) | USD, 2026 | Deal sample (procurement data) | https://www.spendhound.com/marketplace/synthesia-pricing |
| Powtoon individual plans | 49–199 per month | USD, 2026 | List | https://softwarefinder.com/design-software/powtoon |
| Generic AI video generation (Varya) | 0.005 per second | USD, Jun 2026 | List | https://thenextweb.com/news/avataar-ai-varya-video-model-india-cheap |
| Indegene FY26 revenue (market size signal) | 396.9m (INR 35,105m) | USD, FY to Mar 2026 | Reported | https://nsearchives.nseindia.com/corporate/INDEGENE_29042026203956_Intimation_of_Press_Release.pdf |
| Solstice Series A (funding signal) | 21m | USD, May 2026 | Reported | https://hitconsultant.net/2026/05/28/solstice-raises-21m-series-a-pharma-mlr-ai/ |
| Interactive 3D MoA app, booth or iPad | Not found ("quote on request") | — | — | https://axs3d.com/services/medical-scientific-interactive-apps-conference-experiences/ |

Inference (confidence low): on a USD 25–75k MoA film, the 15–20% rule gives about USD 3,750–15,000 per extra language from the original studio. Flat-video AI dubbing comes in at under USD 1,500. A 3D-native versioning service would have to price between the two, at roughly USD 1,500–6,000 per language or format derivative. It would have to win on in-scene text and timing quality, plus a claims-anchor export, not on cost alone.

## Evidence that cuts AGAINST the candidate gaps

1. **Veeva covers claim-level provenance on video and is building more.** It offers frame-level claim links and reference anchors on video, auto claim-linking ("80%", vendor claim), a Claims Agent (August 2026) and Falcon MLR via the Copli acquisition (June 2026), with automatic claim anchoring. A small team's "provenance for MLR" product would compete with the system of record its buyers already pay for.
2. **VarsaAI already sells "AI MoA with sentence-level references and an MLR audit trail" through an agency channel** (GW Health, June 2026). Powtoon's MOA Studio is a recognised (LTEN-finalist) Veeva-aligned AI-MoA product. Gap (b) and the AI side of gap (a) are contested in the exact niche.
3. **The bottleneck is review, not production.** In the Veeva MedTech 2026 benchmark, 64% name local regulatory re-review as the primary barrier. Vodori's 32.4 days is "start to approval", most of which is review and revision, not rendering. A faster render pipeline does not shorten MLR. Veeva's Falcon MLR aims directly at review labour.
4. **Flat-video localisation is cheap, scaled and already inside the large MedComms groups.** Inizio has been a certified Synthesia provider since March 2024; MEDiSTRAVA works in 50+ languages; HeyGen and ElevenLabs are at hundreds of millions of USD in ARR. Language providers sell AI dubbing to pharma with human review. Per-language add-ons at USD 500–1,500 leave little room for a premium.
5. **Content-operations giants own the pharma global-to-local budget and are growing fast.** Indegene grew 23.6% in FY26 and 39.5% in Q2 FY27 (INR). ZS ZAIDYN Content includes localisation, and IQVIA.ai reaches 19 of the top 20 pharma companies.
6. **Label updates mostly change text, not mechanism** (inference, medium). There are about 0.7–0.9 safety label changes per drug per year (2017 study, pre-2024), but these hit ISI and fair-balance text. The 3D mechanism scenes rarely change, so re-render volume per brand is small.
7. **Access to source files is a structural barrier** (inference, medium). In-scene 3D re-versioning needs the original scene files, which the original studio usually holds. That makes the studio the buyer or the competitor, not pharma.
8. **Interactive and real-time 3D MoA is already delivered by incumbent studios** (AXS3D one-app-for-booth/web/tablet; Random42; VOKA; Inizio). Many "interactive" MoAs are pre-rendered with triggers, so demand for true real-time rigs is unproven.
9. **There are no visible prices or traction numbers for AI-MoA tools.** No price and no customer counts exist for MOA Studio or VarsaAI. Either the space is early and open, or it is small. The evidence cannot tell these apart.

## Still unknown

- The number of markets and languages for a typical global MoA film. The per-language cost of a pharma MoA localisation including local MLR. Which party (studio, agency, language provider) does it, by share.
- Whether studios hand over source scene files to clients or agencies under standard contracts. This decides who can sell 3D-native versioning.
- How often an approved MoA film is re-cut (cut-downs, aspect ratios) or re-rendered after approval. The share of derivatives that need 3D work versus 2D overlay changes.
- VarsaAI: price, funding, customers, and whether its videos are 3D, 2D or template-based. Powtoon MOA Studio: general-availability date, price, named pharma customers.
- Whether Veeva's Claims Agent or Falcon MLR handles video or animation natively, or only documents and images.
- Adobe GenStudio's life-sciences offering in 2026. Rask AI or other dubbing tools in named pharma deployments.
- Any review-time figure specific to animation (number of MLR rounds at storyboard, animatic and final). Vodori's full 2025 report and its definitions.
- Deal prices for interactive 3D MoA apps, HCP-portal modules and congress installations. Whether Veeva CLM supports WebGL or glTF content well on current iPads.
- The source of the "9% of global assets reused" figure (attributed to Veeva via LinkedIn only).

## Sources

All accessed via WebSearch snippets on 7 Nov 2026; no page was opened.

1. Visual Pharma by Powtoon named LTEN Excellence Awards finalist for MOA Studio. AI Journal (press release), Apr 2026. https://aijourn.com/visual-pharma-by-powtoon-named-lten-excellence-awards-finalist-for-moa-studio-advancing-compliant-ai-powered-scientific-communication/
2. DIA Medical Affairs & Scientific Communications Forum: exhibitor listing (Powtoon). DIA, 2026 (date not shown). https://live.diaglobal.org/event/medical-affairs-and-scientific-communications-forum-1/exhibitor/RXhoaWJpdG9yXzI0MjE5NTk=
3. Next-gen visual knowledge sharing for pharma teams (Visual Pharma). Powtoon, n.d. https://www.powtoon.com/solution/visual-pharma
4. From complexity to clarity: Medical Affairs. Powtoon, n.d. https://www.powtoon.com/ai/medical-affairs
5. Powtoon review and pricing. SoftwareFinder, n.d. https://softwarefinder.com/design-software/powtoon
6. AI Tool Slashes Pharma Video Production from Weeks to Hours. BriefGlance, 2026. https://briefglance.com/articles/ai-tool-slashes-pharma-video-production-from-weeks-to-hours
7. GW Health Announces Strategic AI Partnership to Expand Communications Capabilities (VarsaAI). PR.com, 22 Jun 2026. https://www.pr.com/press-release/971739
8. GW Health strengthens strategic communications offering with AI partnership (paid release). WebDisclosure, 30 Jun 2026. https://www.webdisclosure.com/press-release/gw-health-strengthens-strategic-communications-offering-with-ai-partnership-UuemjkZTxVB
9. "Cite and verify every claim" (VarsaAI app listing). ChatGPT apps, 2026. https://chatgpt.com/plugins/plugin_asdk_app_6a68f179b5248191b1c50b3b675e0dc4
10. VarsaAI. Capterra India, n.d. https://www.capterra.in/software/1311677/VarsaAI
11. VarsaAI blog: biotech content marketing (cited by track 1). VarsaAI, 2026. https://studio.varsaai.com/blog/biotech-content-marketing
12. Pharmacology animation. Leadde.ai, n.d. https://leadde.ai/solutions/pharmacology-animation
13. AI pharma video maker (Korean). Leadde.ai, n.d. https://leadde.ai/ko/tools/ai-pharma-video-maker
14. Inizio Medical Partners with Synthesia to Unlock AI-Powered Video Creation for Healthcare at Scale. Inizio, Mar 2024 (date from search summary). https://inizio.com/insights/inizio-medical-partners-with-synthesia-to-unlock-ai-powered-video-creation-for-healthcare-at-scale/
15. Inizio Medical (service provider page). Synthesia, n.d. https://www.synthesia.io/service-providers/inizio-medical
16. How MEDiSTRAVA uses AI Videos in 50+ languages for medical communication. Synthesia, n.d. https://www.synthesia.io/case-studies/medistrava
17. Using AI avatars to create 17 MS patient case study videos for HCP engagement. Inizio, Jul 2025. https://inizio.com/insights/ai-avatars-for-hcp-engagement/
18. Inizio Medical 2026 MM+M Awards AI finalists. Inizio, 2026. https://inizio.com/our-businesses/medical/resources/inizio-medical-2026-mmm-awards-ai-finalists-medical-affairs/
19. Synthesia hits $4B valuation, lets employees cash in. TechCrunch, 26 Jan 2026. https://techcrunch.com/2026/01/26/synthesia-hits-4b-valuation-lets-employees-cash-in
20. Synthesia research profile. Sacra, 2025–26. https://sacra.com/research/synthesia
21. Actual Synthesia Pricing 2026. SpendHound, 2026. https://www.spendhound.com/marketplace/synthesia-pricing
22. HeyGen profile ($200M ARR). YesPress, Jun 2026. https://yespress.io/heygen
23. HeyGen research profile. Sacra, 2025. https://sacra.com/research/heygen/
24. HeyGen 2026 G2 summer reports. HeyGen, 2026. https://www.heygen.com/blog/heygen-2026-g2-summer-reports
25. ElevenLabs Series D. ElevenLabs, early 2026. https://elevenlabs.io/blog/series-d
26. ElevenLabs research profile. Sacra, 2026. https://sacra.com/research/elevenlabs
27. ElevenLabs 2026-09-28: v3 Conversational, Dubbing v2. UsagePricing, Sep 2026. https://www.usagepricing.com/blueprint/activity/elevenlabs-2026-09-28-v3-conversational-dubbing-v2
28. Pharmacy translation for digital marketing agencies. Smartcat, n.d. https://www.smartcat.com/pharmacy-translation/digital-marketing-agency
29. VerboLabs AI dubbing (pharma). VerboLabs, n.d. https://www.verbolabs.com/?p=27842
30. Medical and Pharmaceutical Explainer Videos. Wavel, n.d. https://wavel.ai/industry/pharmaceutical-videos
31. 5 Ways Video Localization Fails (with Healthcare Examples). Interpro, Jun 2026. https://www.interproinc.com/video-localization-fails-healthcare-examples/
32. Training videos aren't enough: localization in compliance. Perso.ai, n.d. https://perso.ai/blog/training-videos-arent-enough-localization-in-compliance
33. Vistatec streamlines global video subtitling for a medical device manufacturer. Vistatec, Jun 2026. https://www.vistatec.com/wp-content/uploads/2026/06/Case-Studies_Vistatec-Streamlines-Global-Video-Subtitling-for-a-Medical-Device-Manufacturer.pdf
34. Translate pharma training videos into 75+ languages. translate.video, n.d. https://translate.video/pharmaceuticals/translate-pharma-training-videos-into-75-languages
35. Veeva AI for PromoMats (Korean). Veeva, 2026. https://www.veeva.com/kr/products/veeva-ai-for-promomats/
36. AI for PromoMats (APAC). Veeva, 2026. https://www.veeva.com/ap/?p=254118
37. Veeva news item (AI Agents availability, 4 Dec 2025; page attribution likely). Veeva, Dec 2025. https://www.veeva.com/ap/?p=253815
38. Modernize MLR with AI. Veeva, Jul 2026. https://www.veeva.com/wp-content/uploads/2026/07/Modernize-MLR-with-AI.pdf
39. Veeva AI for PromoMats Features Brief. Veeva, Dec 2025. https://pantheon.veeva.com/wp-content/uploads/2025/12/Veeva-AI-for-PromoMats-Features-Brief.pdf
40. Veeva Acquires Copli, Launches Veeva Falcon MLR to Accelerate Content Review. Veeva (JP), 23 Jun 2026. https://www.veeva.com/jp/resources/veeva-acquires-copli-launches-veeva-falcon-mlr-to-accelerate-content-review/
41. Same release via PR Newswire. StreetInsider, 23 Jun 2026. https://www.streetinsider.com/PRNewswire/Veeva+Acquires+Copli%2C+Launches+Veeva+Falcon+MLR+to+Accelerate+Content+Review/26675730.html
42. Copli acquired by Veeva Systems. Signalbase, 2026. https://www.trysignalbase.com/news/acquisitions/copli-acquired-by-veeva-systems-acquisition
43. Veeva's AI gambit: agentic MLR aims to remake life-sciences compliance. BriefGlance, 2026. https://briefglance.com/articles/veevas-ai-gambit-agentic-mlr-aims-to-remake-life-sciences-compliance
44. How to Annotate a Video in PromoMats and Medical. Veeva Support, n.d. https://support.veeva.com/hc/en-us/articles/360002742354-How-to-Annotate-a-Video-in-PromoMats-and-Medical
45. How to Link Anchors to the Content on a Video in PromoMats and Veeva Medical. Veeva Support, n.d. https://support.veeva.com/hc/en-us/articles/29795579004059-How-to-Link-Anchors-to-the-Content-on-a-Video-in-PromoMats-and-Veeva-Medical
46. Why Bring Forward Annotations is Not Visible for Video Annotations in PromoMats and Medical. Veeva Support, n.d. https://support.veeva.com/hc/en-us/articles/4402585274395-Why-Bring-Forward-Annotations-is-Not-Visible-for-Video-Annotations-in-PromoMats-and-Medical
47. Veeva PromoMats claims management. Veeva, n.d. https://www.veeva.com/products/veeva-promomats/claims-management/
48. 2026 MedTech Commercial Content Benchmark Report. Veeva MedTech, Jul 2026. https://www.veeva.com/medtech/wp-content/uploads/2026/07/2026-MedTech-Commercial-Content-Benchmark-Report-1.pdf
49. Life sciences. Aprimo, n.d. https://www.aprimo.com/solutions/industries/life-sciences
50. Life sciences (new). Aprimo, n.d. https://www.aprimo.com/solutions/industries/solutions-industries-life-sciences-new
51. Healthcare and life sciences. Adobe Partners, n.d. https://partners.adobe.com/digitalexperience/industries/healthcare-life-sciences
52. Adobe and Veeva partner to personalize digital life sciences experience. Adobe Blog, 1 Jul 2021 [pre-2024]. https://blog.adobe.com/en/publish/2021/07/01/adobe-veeva-partner-personalize-digital-life-sciences-experience
53. Indegene: Intimation of Press Release (FY26 results). NSE filing, 29 Apr 2026. https://nsearchives.nseindia.com/corporate/INDEGENE_29042026203956_Intimation_of_Press_Release.pdf
54. Indegene FY26 Revenue Climbs 23.6%, PAT Falls. Whalesbook, Apr 2026. https://www.whalesbook.com/corporate-news/English/tech/Indegene-FY26-Revenue-Climbs-236percent-PAT-Falls-Amid-Client-Growth/69f2351008235f0c2a1bd2ab
55. Indegene reports strong FY26 performance with 23.6% revenue growth. Investywise, Apr 2026. https://www.investywise.com/?p=77795
56. Indegene: Q2 FY27 revenue surges 39.5% YoY to ₹11,223M. Investywise, Oct/Nov 2026. https://www.investywise.com/indegene-reports-strong-q2-fy27-financial-results/
57. Indegene Q2 FY27 earnings transcript highlights. Investywise, Oct/Nov 2026. https://www.investywise.com/indegene-q2-fy27-earnings-transcript-highlights-growth-strategic-wins/
58. Indegene reports Q2 revenue of ₹11.22 billion versus ₹8.04 billion YoY. Sahi, Oct/Nov 2026. https://www.sahi.com/news/indegene-reports-q2-revenue-of-11-22-billion-versus-8-04-billion-yoy
59. From automation to oversight. IQVIA blog, Jul 2026. https://www.iqvia.com/blogs/2026/07/from-automation-to-oversight
60. IQVIA launches IQVIA.ai agentic AI platform with Nvidia. Let's Data Science, Mar 2026. https://letsdatascience.com/news/iqvia-launches-iqviaai-agentic-ai-platform-with-nvidia-b1ca210d
61. Power launch excellence with generative AI. IQVIA, 2025–26. https://www.iqvia.com/library/articles/power-launch-excellence-with-generative-ai
62. ZS launches agentic AI products ZAIDYN Medical and ZAIDYN Content. ZS, 19 May 2026. https://www.zs.com/about/newsroom/zs-launches-agentic-ai-products-zaidyn-medical-and-zaidyn-content
63. ZS expands ZAIDYN platform with agentic AI applications. The Consulting Report, May 2026. https://www.theconsultingreport.com/zs-expands-zaidyn-platform-with-agentic-ai-applications-for-regulated-life-sciences-workflows/
64. Solstice raises $21M Series A (pharma MLR AI). HIT Consultant, 28 May 2026. https://hitconsultant.net/2026/05/28/solstice-raises-21m-series-a-pharma-mlr-ai/
65. Solstice raises $21M Series A for faster pharma marketing compliance cycles. ContentGrip, May/Jun 2026. https://www.contentgrip.com/solstice-series-a-pharma-mlr/
66. Solstice Series A analysis. NewMarketPitch, 1 Jun 2026. https://newmarketpitch.com/blogs/news/solstice-series-a-analysis
67. India's Avataar AI launches a video model that costs $0.005 per second. The Next Web, Jun 2026. https://thenextweb.com/news/avataar-ai-varya-video-model-india-cheap
68. Pharma video marketing guide. AITuber, 2026. https://aituber.app/blog/pharma-video-marketing/
69. Future of biotech animation 2026. AXS3D, 2026. https://axs3d.com/blog/future-of-biotech-animation-2026/
70. Pharma digital marketing MLR review (2025 benchmarks; 32.4 days). Vodori, 2025. https://www.vodori.com/blog/pharma-digital-marketing-mlr-review
71. Process iteration: the secret to top-performing MLR processes. Vodori, 2025. https://www.vodori.com/blog/process-iteration-the-secret-to-top-performing-mlr-processes
72. 4 tips to improve video feedback during MLR review. Vodori, May 2022 [pre-2024]. https://vodori.com/blog/4-tips-to-improve-video-feedback-during-mlr-review
73. Veeva benchmark page (US days in review fell to 16). Veeva, 2023 data [pre-2024]. https://www.veeva.com/?p=93099
74. From Checkpoint to Input: A Different Model for MLR. Klick IDX, 2025. https://idx.klick.com/articles/from-checkpoint-to-input-a-different-model-for-mlr
75. Animated Explainer Packages (price sheet). Explainify, Aug 2022 [pre-2024]. https://explainify.com/wp-content/uploads/2022/08/Animated_Explainer_Packages.pdf
76. Medical Animation Cost Guide: What You Should Expect to Pay. Prolific Studio, c. 2025–26. https://prolificstudio.co/?p=30191
77. Medical animation cost. Podymos, n.d. https://podymos.com/learning-center/medical-animation-cost
78. AI video translation and voice cloning across languages. Contra, n.d. https://contra.com/s/sbEEXk72-ai-video-translation-voice-cloning-across-languages
79. Clear medical animations for patient understanding. Fiverr, n.d. https://fiverr.com/fcreativeteam/clear-medical-animations-for-patient-understanding
80. DDimer translation (portfolio). Production Attic Dublin, n.d. https://www.dublin.productionattic.com/portfolio/ddimertranslation
81. Medical animation cost. VOKA, 2025–26. https://voka.io/medical-animation-cost/
82. Pharmaceutical content localization: problems, strategies, and tools. Viseven, n.d. https://viseven.com/best-practices-content-localization/
83. Kieran Fairnington (LinkedIn profile/post citing Veeva 9% reuse). LinkedIn, n.d. https://es.linkedin.com/in/kieran-fairnington
84. Global versus local: Mind the content gap. Reuters Events, n.d. https://www.reutersevents.com/pharma/node/63059
85. Optimize content operations. Reuters Events, n.d. https://events.reutersevents.com/pharma/article/optimize-content-operations
86. Safety-related label changes, expedited vs non-expedited drugs. BMJ via PMC, 2017 [pre-2024]. https://pmc.ncbi.nlm.nih.gov/articles/PMC5588044
87. PMC article on post-approval label updates. PMC, c. 2021 [pre-2024]. https://pmc.ncbi.nlm.nih.gov/articles/PMC8159207
88. PMC article on safety updates for new therapeutic biologics. PMC, c. 2018 [pre-2024]. https://pmc.ncbi.nlm.nih.gov/articles/PMC6013049
89. Sources of evidence triggering and supporting safety-related labeling changes. Drug Safety (Springer), 2021 [pre-2024]. https://link.springer.com/article/10.1007/s40264-021-01142-3
90. Drug Safety-related Labeling Changes (SrLC) database. FDA, ongoing. https://www.fda.gov/drug-safety-labeling-changes
91. Footnotes and fair balance. Mechanism Digital, n.d. https://mechanismdigital.com/post/footnotes-and-fair-balance
92. Veeva CLM: IT Guide for Pharma Marketing. IntuitionLabs, 2025–26. https://intuitionlabs.ai/articles/veeva-clm-pharma-marketing-guide
93. Viscira enhances Veeva iRep with its version 2.0 vDetail solution. PRWeb, c. 2013 [pre-2024]. https://www.prweb.com/releases/viscira_enhances_veeva_irep_with_its_version_2_0_vdetail_solution/prweb10955027.htm
94. Interactive Visual Aids in Pharma: Driving Engagement. TechnoLynx, 2026. https://technolynx-site.pages.dev/post/interactive-visual-aids-in-pharma-driving-engagement
95. Interactive Apps & Experiences. AXS3D, n.d. https://axs3d.com/services/medical-scientific-interactive-apps-conference-experiences/
96. Interactive MOA for Booth and Browser. AXS3D, n.d. https://axs3d.com/?p=17081
97. Bring Your Science to Life at ESMO 2025. Random42, 2025. https://random42.com/company-news/esmo-2025
98. Medical booth ideas for pharma. VOKA, n.d. https://voka.io/medical-booth-ideas-for-pharma/
99. Delivering an immersive interactive MOA congress engagement. Inizio, 2025–26. https://inizio.com/insights/moa-congress-engagement/
100. How smart spaces and real-time strategy transformed ASCO 2025. Inizio, 2025. https://inizio.com/insights/real-time-strategy-at-asco25/
101. Let's discuss our pricing. eWizard (Viseven), n.d. https://ewizard.io/pricing
102. Viseven eWizard pricing. G2, n.d. https://www.g2.com/products/viseven-ewizard/pricing
103. BioDigital for pharma. BioDigital, n.d. https://www.biodigital.com/customers/pharma
104. What does interactive pharma content look like in an HCP portal? Digitalya, n.d. https://digitalya.co/blog/interactive-pharma-content-for-hcp-portals/
