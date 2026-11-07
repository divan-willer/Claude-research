# Follow-up: Licensing validated biomedical 3D data to AI, ed-tech and simulation firms

> **Method and limits.** I ran 30 WebSearch queries, the full cap. WebFetch was blocked, so I opened no page. Every citation is a search-result snippet or summary, marked "(snippet)". Some summaries merged several results, so I could not always tie a number to one URL; those are marked "attribution uncertain". I did not repeat follow-up A's marketplace price searches; I reuse its figures and say so. Today is 7 Nov 2026.

## Bottom line

- **Paying for licensed AI training data is a real, large market, but the money sits with huge libraries and a few buyers.**
  - Shutterstock's Data, Distribution and Services line made $203.3M in 2025, up 16%.
  - Reddit's data-licensing ("Other") revenue was about $140M in 2025.
  - News publishers' deals run from $1-5M (Le Monde/Prisa) to about $50M a year (News Corp-OpenAI).
  - Shutterstock's licensing deals came from just 20 customers, worth $238M in lifetime value (July 2025).
- **3D-specific licensing exists and is growing. No one publishes a per-asset price.**
  - TurboSquid's 1.5M+ models trained NVIDIA's Edify 3D.
  - Shutterstock sells "3D & Spatial" datasets for generative 3D and robotics.
  - Deemos (maker of Hyper3D/Rodin) bought a commercial Shutterstock 3D licence for model training (16 Dec 2025).
  - CGTrader has sold AI-training rights only through enterprise deals since 15 May 2026.
  - Daz 3D and A23D (500k+ human-authored models) sell datasets by quote.
- **Volume prices are tiny for a small specialist library.**
  - Video sells for $1-4 per minute, and animation for $2-3 per minute.
  - Adobe paid about $2.62 per minute of video and $0.06-0.16 per image.
  - At those rates, a catalogue of a few hundred biomedical assets earns hundreds to low thousands of dollars. It only makes real money if priced as a specialist dataset, an evaluation set or a custom build.
- **I found no evidence that any named buyer has bought anatomical 3D data or synthetic anatomy from an artist or studio.** The named buyers are the AI 3D/video firms, BioRender, Fundamental XR, NVIDIA, and surgical and imaging AI firms.
  - Medical AI builds anatomy from patient imaging. NVIDIA MAISI was trained on 10,277 CT volumes and outputs 127 anatomical classes. Fundamental XR's engine is trained on imaging, surgical video and pathology. Inner Logic builds virtual patients from clinical imaging.
  - Free sets also exist: MedShapeNet has 100,000+ medical shapes.
- **The accuracy problem is real, but it is not mainly a mesh problem.**
  - Surgeons rated Veo-3 surgical clips high on realism but low on medical plausibility. Only 2.8-6.2% of the errors traced to image quality.
  - Inference (medium): buyers' gap is anatomy and procedure *reasoning*. That points to expert-labelled evaluation sets and expert review, more than to extra meshes.
  - Vendors claim a premium for "rights-cleared, human-authored" data, but no one has priced it.
- **The risks are serious:**
  - **Lumpy one-off revenue.** Getty booked deal revenue early. Shutterstock's Q4 2025 data line fell 19%.
  - **Buyer concentration.**
  - **Opaque payouts to contributors.** TurboSquid artists have petitioned over obscure payouts.
  - **Substitution** by synthetic, free or scraped data.
- **Verdict: a real but small and lumpy revenue line. It is an add-on to a validated asset library, not a standalone business in 6-12 months.**
  - First revenue is most likely to come from three sources:
    - custom dataset or evaluation-set builds for one or two AI 3D firms or sim/ed-tech platforms (about $10k-75k per deal; low confidence);
    - opting the library into Shutterstock or CGTrader enterprise data deals (small, with a revenue share);
    - expert-annotation contract work ($24-100/hr benchmarks).
  - Licensing a back catalogue to AI labs is the least likely of the four routes.

## Findings

### Q1. Comparables: AI training data licensing revenue and deal terms

**Facts**

- **Shutterstock (2025 results)**
  - Total revenue was $989.9M, up 6%. "Data, Distribution, and Services" was $203.3M, up 16%, or 21% of revenue ([Yahoo Finance](https://finance.yahoo.com/news/shutterstock-sstk-reports-989-9m-114655765.html); [Shutterstock IR](https://shutterstock.gcs-web.com/node/14551)) (snippet).
  - The line is not pure AI licensing: it also bundles metadata sales, distribution and services.
  - In Q4 2025 this line fell 19% year on year, to $30.7M (same sources) (snippet).
- **Shutterstock (July 2025 data-business update):** licensing deals are its most common data deal, with 20 customers and $238M in lifetime deal value ([Quartr](https://quartr.com/events/shutterstock-inc-sstk-data-business-update-presentation_3PWD6t1U)) (snippet; attribution uncertain).
- **Shutterstock deal terms**
  - Lightricks (Jan 2025) trains its LTXV video model on Shutterstock HD/4K video. Buyers can start on a smaller research licence and upgrade to a commercial one. Contributors get 20% of data-licensing revenue ([CO/AI](https://getcoai.com/news/shutterstock-lightricks-partnership-offers-example-of-how-to-ethically-source-training-data-for-ai-video)) (snippet).
  - In Oct 2025 Shutterstock widened its offer from data supplier to "active partner in model construction, training and assessment", across 3D, images, text and video ([Nasdaq/Shutterstock PR](https://www.nasdaq.com/press-release/shutterstock-builds-data-licensing-strength-new-ai-services-model-training-and)) (snippet).
  - In March 2026 it cited "accelerating demand" and expanded its licensed datasets ([Shutterstock IR](https://investor.shutterstock.com/node/14596)) (snippet).
  - In June 2026 a trade piece said clients increasingly ask for custom datasets, with "highly technical" specs (angles, variations, metadata) ([LBB](https://lbbonline.com/news/AI-Model-Development-Training-Data-Scarcity-Shutterstock-Studios)) (snippet).
- **TurboSquid / NVIDIA Edify 3D**
  - The deal was announced in March 2023 and launched at SIGGRAPH 2024. Models were trained on TurboSquid's 1.5M+ 3D models, and about 10% of artists opted out ([CG Channel 2023](https://www.cgchannel.com/2023/03/nvidia-and-shutterstock-to-launch-ai-based-text-to-3d-service) [pre-2024]; [NVIDIA model card](https://build.nvidia.com/shutterstock/edify-3d/modelcard)) (snippet).
  - A share of each data deal goes into a "Contributor Fund", paid out every 3-6 months ([TurboSquid/Squid](https://resources.squid.io/artist-blog/update-on-our-generative-3d-partnership-with-nvidia); [TurboSquid FAQ](https://resources.turbosquid.com/?p=19881)) (snippet).
  - No per-model payout is published.
- **Shutterstock "3D & Spatial" datasets**
  - Pitched for generative 3D and robotics vision.
  - Formats: FBX, OBJ, USD, DAE, glTF and others, with renders at 600px and 2K.
  - Shutterstock describes them as "rights-cleared and contributor-permissioned", including rights to commercialise trained models and outputs ([Shutterstock](https://www.shutterstock.com/data-licensing/3d-&-spatial)) (snippet; vendor claim).
- **Getty Images**
  - Q4 2025 revenue was $282.3M, up 14.1%. It was lifted by two multi-year deals: one with a social media company for display rights, one with an AI company for creative content.
  - The CFO said these are "not pure data licensing". Revenue was recognised early, and only recurring revenue is in forecasts. 2026 faces a hard comparison ([Barchart](https://www.barchart.com/story/news/787390/gety-q4-deep-dive-one-time-licensing-deals-drive-revenue-growth-amidst-cautious-guidance)) (snippet).
  - Perplexity signed a multi-year licensing deal on 31 Oct 2025; terms were not disclosed ([The Star/Reuters](https://www.thestar.com.my/tech/tech-news/2025/10/31/getty-perplexity-sign-multi-year-licensing-deal-to-boost-ai-powered-search-visuals)) (snippet).
  - In Jan 2026 Getty and nfiniteAI agreed to turn Getty's 2D content into 3D scenes for embodied AI and robotics simulation ([Getty newsroom](https://newsroom.gettyimages.com/en/getty-images/nfiniteai-collaborates-with-getty-images-to-bring-2d-visual-content-into-the-3d-physical-ai-era)) (snippet).
  - Getty and Shutterstock are merging into a reported $3.7B firm ([CG Channel tag page](https://www.cgchannel.com/tag/getty-images)) (snippet).
- **CGTrader**
  - From 15 May 2026, standard listings are not eligible for AI training. AI-training licences go only through enterprise agreements that CGTrader negotiates "on your behalf" ([CGTrader help](https://help.cgtrader.com/hc/en-us/articles/46191349842705-Can-my-models-still-be-licensed-for-AI-training)) (snippet).
  - "Custom Enterprise Deals" were added to its General Terms (§18.12-18.13) in April 2026. Sellers are opted in by default from 15 May 2026 and can opt out ([CGTrader help](https://help.cgtrader.com/hc/en-us/articles/46191760965137-What-is-a-Custom-Enterprise-Deal-and-how-does-it-affect-my-earnings-as-a-seller)) (snippet). I did not see the royalty share.
  - Its datasets pages offer "tailor-made datasets", ready-made or "custom assets built to order", with a free sample and no price ([CGTrader datasets](https://admin.cgtrader.com/datasets); [CGTrader Arsenal](https://arsenal.cgtrader.com/3d-model-datasets-for-generative-ai)) (snippet).
  - An older CGTrader Analytics AI page required content to stay available for 12 months after signing, with six months' notice to opt out ([CGTrader](https://cgtrader.com/pages/cgtrader-analytics-terms-of-service)) (snippet; may not apply to the 2026 deals).
- **Other 3D dataset vendors**
  - Daz 3D sells "fully licensed, commercially safe" character datasets. It says every model is Daz-owned or licensed with artist permission. Access is by enterprise request, with no public price ([Daz 3D](https://daz3d.com/ai-training-data); [Daz AI datasets](https://www.daz3d.com/ai-datasets)) (snippet; vendor claim).
  - A23D says it has 500,000+ 3D models, PBR textures, decals and IES profiles, "entirely human-authored in-house", licensed for AI training through enterprise@a23d.co ([A23D README](https://a23d-readme.static.hf.space/README.md); [Hugging Face](https://huggingface.co/A23D)) (snippet; vendor claim).
- **Free / scraped substitute: Objaverse**
  - Its objects came from Sketchfab under mixed Creative Commons licences, some non-commercial, and creators were not told ([The Decoder](https://the-decoder.com/sketchfab-objaverse-ai-copyright-dispute-enters-third-dimension/); [FlippedNormals](https://blog.flippednormals.com/objaverse-raises-concerns-about-ethics-of-scraping-3d-content/)) (snippet; likely 2023 [pre-2024, possibly stale]).
  - Objaverse-XL's ODC-By licence covers the compilation, not each object ([Hugging Face README](https://huggingface.co/datasets/allenai/objaverse-xl/raw/main/README.md)) (snippet).
- **Reddit**
  - "Other" (mainly data-licensing) revenue was about $140M in 2025, up 22%.
  - Google reportedly pays about $60M a year, under a deal expiring in H1 2027. OpenAI is estimated at about $70M a year.
  - A recent quarter showed $43M, up 24%, about 5% of revenue.
  - The CEO wants higher, usage-based pricing at renewal ([Crypto Briefing](https://cryptobriefing.com/reddit-data-licensing-revenue-openai-google/); [Motley Fool, Aug 2026](https://www.fool.com/investing/2026/08/17/reddits-data-revenue-openai-google-buyers/); [FourWeekMBA](https://fourweekmba.com/ai-reddit-ai-curse-q2-2026-earnings/)) (snippet; the Google/OpenAI splits are press estimates).
- **News publishers**
  - News Corp-OpenAI: more than $250M over five years (May 2024).
  - NYT-Amazon: $20-25M a year (2025) ([Engadget](https://www.engadget.com/ai/the-new-york-times-and-amazons-ai-licensing-deal-is-reportedly-worth-up-to-25-million-per-year-135523853/)) (snippet).
  - Axel Springer: about $13M a year. FT: $5-10M a year ([LLM Pulse tracker](https://llmpulse.ai/blog/ai-content-licensing-deals/)) (snippet; attribution uncertain).
  - Neudata (June 2025) counted 52 deals. OpenAI reportedly offered Le Monde and Prisa only $1-5M for training plus retrieval ([Neudata](https://www.neudata.co/blog/ai-data-licensing-market-analysis)) (snippet).
  - Quartz (May 2026) reports that early deals were flat annual fees, and are now moving towards usage-based terms as the information gap narrows ([Quartz](https://qz.com/ai-training-data-pricing-licensing-deals-market-052126)) (snippet).
- **Video per-minute and per-hour prices**
  - Bloomberg (Jan 2025) reported that OpenAI, Google and others pay $1-4 per minute for unused creator video. Standard footage gets $1-2; premium formats (4K, drone, 3D animation) get more ([Bloomberg Law](https://news.bloomberglaw.com/ip-law/youtubers-are-selling-their-unused-video-footage-to-ai-companies); [The Decoder](https://the-decoder.com/openai-and-google-are-buying-youtubers-unpublished-videos-for-up-to-4-per-minute/); [PetaPixel](https://petapixel.com/2025/01/13/ai-companies-are-paying-content-creators-for-their-unpublished-videos)) (snippet).
  - Kidscreen: live action $1-2 per usable minute; animation $2-3 per minute ([Kidscreen](https://kidscreen.com/?p=221834)) (snippet).
  - Defined.ai reportedly cites up to $2 per image, $2-4 per short video, and $100-300 per hour of longer video ([AI News](https://www.artificialintelligence-news.com/news/ai-giants-pay-thousands-for-creators-unused-footage-to-train-models/)) (snippet; attribution uncertain).
- **Adobe (Apr 2024)**
  - Paid about $2.62 per minute of video on average, up to about $7.25, and $0.06-0.16 per image. It paid no royalties ([PetaPixel](https://petapixel.com/2024/04/11/adobe-will-buy-your-videos-for-up-to-7-25-per-minute-to-train-ai-report); [The Register](https://www.theregister.com/2024/04/12/adobe_buying_videos_ai); [ZDNet](https://www.zdnet.com.au/article/adobe-is-buying-videos-to-train-its-new-ai-generator-but-are-they-paying-enough/)) (snippet).
- **Medical imaging data prices:** none found. Marketplaces such as AWS list DICOM corpora with "enterprise licensing upon request" ([AWS Marketplace](https://aws.amazon.com/marketplace/pp/prodview-qcoatqz6wf7n6)) (snippet).
- **Market size**
  - Fortune Business Insights: AI training dataset market $3.59B in 2025, rising to $4.44B in 2026 (via [Quartz](https://qz.com/ai-training-data-pricing-licensing-deals-market-052126)) (snippet).
  - Vermillio: AI content licensing about $10B in 2025, rising to $67.5B by 2030 ([CO/AI](https://getcoai.com/news/a-67-5b-market-emerges-for-licensing-creative-work-to-train-ai)) (snippet; vendor forecast).

**Inferences**

- *High:* buyers pay real money for licensed data, but the biggest cheques go to scale (millions of assets) or unique live data (Reddit, news). A niche 3D library has neither.
- *Medium:* for 3D, the standard route is through aggregators: Shutterstock/TurboSquid, CGTrader, Getty. Contributors get a pooled share (Shutterstock-Lightricks: 20%). A small vendor going through them would earn little per asset.
- *Medium:* volume pricing ($1-4 per minute of video, cents per image) implies very low per-asset value. Premium pricing needs a "dataset with a purpose": custom specs, labels or evaluation use. This matches Shutterstock's report of "highly technical" custom requests and CGTrader's "custom assets built to order".

### Q2. Buyers: do AI 3D/video, BioRender, Fundamental XR, NVIDIA and med-AI firms buy anatomical 3D data?

**Facts: general 3D buyers (not anatomy)**

- **Deemos / Hyper3D (Rodin)** bought a commercial 3D asset licence from Shutterstock on 16 Dec 2025, "being incorporated into ongoing model training". It frames this as building a "rights-cleared ecosystem" ([Hyper3D blog](https://hyper3d.ai/blog/hyper3d-shutterstock); [PressAdvantage](https://business.ricentral.com/ricentral/article/pressadvantage-2025-12-16-hyper3d-acquires-commercial-3d-asset-license-from-shutterstock-and-announces-cooperation-with-blender)) (snippet). Scope and price were not disclosed.
- **NVIDIA** trained Edify 3D on TurboSquid and Shutterstock data (above).
- **Meshy**
  - It raised about $400M at a $1.5B valuation in July 2026 (follow-up A; [3Dnatives](https://www.3dnatives.com/en/meshy-400-million-in-series-b-21072026/)) (snippet).
  - A Meshy "Data Artist" posting includes "monitoring the quality of models from outsourcing vendors and giving them feedback" ([Chopping Block](https://www.choppingblock.ai/jobs/data-artist-at-meshy)) (snippet; date not shown).
- **Tripo** raised 3B yuan (Series B/B+, Sept 2026) partly for "3D-native foundation models and 3D data infrastructure" ([3Dnatives](https://www.3dnatives.com/en/tripo-ai-raises-3-billion-yuan-04092026/amp/)) (snippet).
- **Stability AI** posted an ML Data Engineer role on 18 Nov 2025 to curate large-scale unstructured data, including 3D ([Simplify](https://simplify.jobs/p/0cf76fa8-22f8-458b-94ad-b5b35e706d08/Machine-Learning-Data-Engineer)) (snippet).
- **Mercor (labour, not data)**
  - It hires 3D artists, generalists and TDs to "improve AI tools for 3D content creation" at $24-60/hr ([Mercor](https://work.mercor.com/jobs/list_AAABlYGD8f6kNvV2OWRBPJw6/3-d-artist)) (snippet).
  - Fine-art and illustration expert tasks pay $60-100/hr ([Mercor](https://work.mercor.com/jobs/list_AAABm5NePFoYr4KV3olKurwc/fine-artists-including-painters-sculptors-and-illustrators)) (snippet).
  - A "Biomedical Scientist – AI Trainer" role asks for anatomy and physiology fluency, and for reading "anatomic diagrams" ([Career.com](https://www.career.com/job/mercor/biomedical-scientist-ai-trainer/j202604281006073001191)) (snippet).
- **Search gaps:** no deal or job post found for Luma, Runway, Google or OpenAI buying 3D or anatomy data. Their known data buying is video by the minute (above).

**Facts: biomedical buyers**

- **BioRender**
  - In Oct 2026 it launched Leo, an AI figure agent. Leo's stated edge is "scientist-vetted icons and templates" ([BetaKit](https://betakit.com/biorender-launches-ai-agent-for-building-scientific-research-images/)) (snippet).
  - It was valued at $900M in Dec 2025 (same).
  - No 3D animation product or 3D data purchase was found. Follow-up A found only a "3D" restyle of icons.
- **Fundamental XR, Anatomy Inference Engine (beta)**
  - Trained on "imaging data, surgical videos, and pathology datasets". No providers or pricing are named ([Pharmaceutical Manufacturer](https://pharmaceuticalmanufacturer.media/pharma-manufacturing-news/digital-health-in-pharma-news/fundamental-xr-launches-ai-powered-anatomy-inference-engine/)) (snippet).
  - Its partners include Mayo Clinic, Teleflex, Orbis and CMR Surgical (same search; [IntuitionLabs](https://intuitionlabs.ai/companies/digital-health/fundamentalxr)) (snippet).
  - It runs a mixed-reality programme with Elsevier (Nov 2025) ([HIT Consultant](https://hitconsultant.net/2025/11/13/fundamental-xr-and-elsevier-launch-mixed-reality-innovation-program-for-enterprise-ai)) (snippet).
- **NVIDIA MAISI**
  - A diffusion model generating synthetic 3D CT plus masks for up to 127 anatomical classes. It was trained on 10,277 CT volumes ([arXiv 2409.11169](https://arxiv.org/html/2409.11169v1); [NVIDIA NIM docs](https://docs.nvidia.com/nim/medical/maisi/1.0.0/model-details.md)) (snippet).
  - NVIDIA reports that synthetic data improved tumour segmentation by about 2.5-4.5% ([NVIDIA blog](https://developer.nvidia.com/blog/?p=83468)) (snippet; vendor-reported).
  - It ships under an NVIDIA evaluation licence (same docs) (snippet).
- **Surgical and simulation AI**
  - Inner Logic raised $11.5M (2026). It builds "high-fidelity virtual patients built from real clinical imaging and procedural datasets" ([HIT Consultant](https://hitconsultant.net/2026/07/27/inner-logic-simulation-infrastructure-procedural-devices/); [Dealroom](https://dealroom.co/news/145393-inner-logic-raises-11-5m-to-simulate-surgery-on-thousands-of-virtual-pat)) (snippet).
  - XRlabs ($8.4M seed) turns CT and MRI scans into 3D anatomy ([MobiHealthNews](https://www.mobihealthnews.com/news/xrlabs-raises-84m-ai-surgical-platform)) (snippet).
  - AnthroTek raised £950k (June 2025) for physical synthetic anatomy plus AI 3D models ([StartupRise](https://startuprise.co.uk/cambridge-based-anthrotek-closes-950k-seed-funding/)) (snippet).
  - Redefine Surgery raised a $10M pre-seed for immersive 3D surgical training ([Signalbase](https://www.trysignalbase.com/news/funding/redefine-surgery-raises-10m-pre-seed-round)) (snippet).
- **Ed-tech / simulation content licensors (existing sellers, not buyers)**
  - BioDigital sells a Content API and Web API by quote. Custom 3D models come through Professional Services "for a one-time fee" ([BioDigital pricing](https://pricing.biodigital.com/business.html)) (snippet).
  - Zygote licenses its anatomy library for "animation, simulation… engineering and analysis" ([SolidWorks partner page](https://solidworks.com/partner-product/zygote-human-anatomy-and-skeletal-data)) (snippet; date not shown).
  - IT'IS / ZMT license the Virtual Population (ViP) simulation anatomy. Research use is free; commercial use carries a licence fee, with no public price ([IT'IS FAQ](https://itis.swiss/virtual-population/virtual-population/faq/); [IT'IS ViP brochure](https://itis.swiss/assets/Downloads/VirtualPopulation/1706-virtual-population-web.pdf) [pre-2024]) (snippet).
- **Anatomy vendors pitching AI use**
  - Atomedge's site says its cadaver-scan-based model is useful for AI training ([Atomedge](https://keyboard-poodle-zzyx.squarespace.com)) (snippet; vendor claim).
  - Virtual Body published a CC-licensed anatomy model described as "a prime resource for AI training in medical image computing" ([Virtual Body](https://www.virtual-body.org/news/3d-anatomy-model-published-under-cc-license/)) (snippet).
- **Free medical shapes:** MedShapeNet has 23 datasets and 100,000+ annotated shapes, "freely accessible" via web and Python API ([arXiv 2308.16139](https://arxiv.org/abs/2308.16139)) (snippet; first version 2023 [pre-2024]; the shapes' licences vary by source).
- **No deals found:** no 2024-2026 deal or job post turned up for an "anatomy dataset" or anatomical 3D data purchase by any named firm. Evidence thin.

**Inferences**

- *High:* imaging AI, surgical AI and simulation firms get anatomy from patient scans (CT/MRI) or from their own generators. Artist-sculpted meshes do not match their data domain (volumes, labels, real variation). They are unlikely buyers of "training data". They may buy *content* (visual layers, education assets), and that is ordinary licensing, not data licensing.
- *Medium:* general AI 3D firms (Deemos, Meshy, Tripo, Stability) do buy rights-cleared 3D data, and Meshy uses outsourcing vendors. Anatomy is a tiny slice of their demand. A biomedical set would be a niche category inside a much larger purchase, unless it is sold as an evaluation or benchmark set.
- *Low-medium:* BioRender is the most natural biomedical buyer, with its "scientist-vetted" positioning and 3D restyle. There is no evidence it buys outside content. It builds in-house.
- *Low:* the founder may already be close to Atomedge. This session's tools include an Atomedge anatomy-brief skill for its female anatomy model, but I have not verified the relationship. If he is, Atomedge is both a comparable and a possible channel for AI-data deals.

### Q3. Value drivers: validation, provenance, clean licensing; anatomy accuracy problems

**Facts**

- **Provenance is part of the sales pitch:**
  - Deemos calls its Shutterstock licence part of a "rights-cleared ecosystem" and says it ensures every part is "legitimate and trustworthy" ([Hyper3D](https://hyper3d.ai/blog/hyper3d-shutterstock)) (snippet).
  - Shutterstock says its data is "rights-cleared and contributor-permissioned" ([Shutterstock](https://www.shutterstock.com/data-licensing/3d-&-spatial)) (snippet).
  - Daz says "commercially safe" and A23D says "human-authored" (above).
  - TurboSquid sells an Enhanced Licence that adds $10k indemnification (follow-up A; [TurboSquid](https://www.turbosquid.com/3d-model/enhanced-licenses/anatomy/rig/gltf)) (snippet).
- **Human Native** was a licensed-data marketplace with subscription, revenue-share and per-use pricing. Cloudflare acquired it on 15 Jan 2026 ([SiliconANGLE](https://siliconangle.com/?p=727953)) (snippet).
  - One anecdote: a UK video-AI company "threw away" its existing training data after licensed data gave better results ([LAVX News](https://news.lavx.hu/article/cloudflare-acquires-human-native-to-build-compensated-ai-training-data-ecosystem)) (snippet; single unnamed case).
  - An analyst notes the open question of "proving that the data quality justifies the premium" ([Kaptur](https://kaptur.co/cloudflares-play-warehouse-or-toll-booth-or-both/)) (snippet).
- **Data is getting scarcer:** Epoch AI projects that public human text will be used up between 2026 and 2032 (via [Quartz](https://qz.com/ai-training-data-pricing-licensing-deals-market-052126)) (snippet).
- **Accuracy failures:**
  - SurgVeo study: surgeons rated Veo-3 surgical clips high on visual realism, but plausibility fell when medical accuracy was required. Only 6.2% (abdominal) and 2.8% (brain) of errors were image-quality errors; most were reasoning and instrument handling ([The Decoder](https://the-decoder.com/googles-veo-3-can-fake-surgical-videos-but-misses-every-hint-of-medical-sense/)) (snippet).
  - JMIR Medical Education (2025) reports that AI-generated anatomical diagrams often contain gross inaccuracies ([JMIR Med Educ](https://mededu.jmir.org/2025/1/e80084)) (snippet).
  - A CMEJ commentary (2024) says Sora-type video needs expert oversight, and that accuracy is hard for complex anatomy such as brain vasculature ([CMEJ](https://journalhosting.ucalgary.ca/index.php/cmej/article/download/79065/57851/258885)) (snippet).
  - Track 5 found "alien anatomy" in a practitioner study, and Sora-2/Veo-3 at about 64% and 58.7% on phenomenon congruency.
- **Nothing priced:** I found no published price comparison between licensed and scraped data, and no buyer statement that it pays more for *scientifically validated* data.

**Inferences**

- *Medium:* clean licensing is now table stakes for selling to commercial AI firms (Deemos, Lightricks, Edify). It is a requirement, not a premium. A biomedical library with documented authorship and no scraped inputs clears the bar but does not command a markup for that alone.
- *Medium:* scientific validation is valued most where it can *measure* a model. Examples: an anatomy and mechanism evaluation set with expert labels and source dossiers, and expert review of model outputs. Evaluation sets are small, not commoditised by volume, and re-run with every model release. Validation does not add much to raw training volume.
- *Low:* AI video firms will fix anatomy with targeted data only once medical and education use cases make money for them. I found no sign of that yet.

### Q4. Risks

**Facts**

- **One-off and lumpy revenue:**
  - Getty booked its Q4 2025 AI and social deals early and warned of a hard 2026 comparison ([Barchart](https://www.barchart.com/story/news/787390/gety-q4-deep-dive-one-time-licensing-deals-drive-revenue-growth-amidst-cautious-guidance)) (snippet).
  - Shutterstock's data line fell 19% in Q4 2025 ([Yahoo Finance](https://finance.yahoo.com/news/shutterstock-sstk-reports-989-9m-114655765.html)) (snippet).
- **Buyer concentration:**
  - Shutterstock has 20 licensing customers ([Quartr](https://quartr.com/events/shutterstock-inc-sstk-data-business-update-presentation_3PWD6t1U)) (snippet).
  - Reddit's data revenue is mostly Google plus OpenAI (above).
- **Prices and payouts are falling or opaque:**
  - OpenAI offered $1-5M for two major news archives ([Neudata](https://www.neudata.co/blog/ai-data-licensing-market-analysis)) (snippet).
  - TurboSquid artists petition that Contributor Fund payouts "have fallen into complete obscurity" ([Change.org](https://www.change.org/p/shutterstock-turbosquid-stop-exploiting-3d-artists-demand-transparency-and-fair-pay)) (snippet).
  - Artists report falling sales and missing payments ([80.lv](https://80.lv/articles/artists-threaten-to-leave-turbosquid-because-of-plummeting-sales-missing-payments)) (snippet), and blame AI for falling TurboSquid sales (July 2026) ([Foro3D](https://foro3d.com/2026/julio/artistas-de-turbosquid-denuncian-caida-de-ventas-por-culpa-de-la-ia.html)) (snippet).
- **Substitution:**
  - Objaverse shows that scraped 3D was used at scale (above).
  - MAISI generates synthetic anatomy, and MedShapeNet is free.
  - Fundamental XR generates anatomy itself.
- **Counter-trend:** new sites have blocked AI crawlers by default since mid-2025 ([Kaptur](https://kaptur.co/cloudflares-play-warehouse-or-toll-booth-or-both/)) (snippet; attribution uncertain). Most AI training-data lawsuits are still unresolved (track 5).

**Inferences**

- *High:* a data licence is usually paid once per model generation, or as an annual flat fee. Recurring revenue needs refresh obligations, new content each year, or evaluation-set subscriptions.
- *Medium-high:* the price per asset trends down as generators improve and synthetic data spreads. For a static anatomy mesh, an AI 3D firm can reach "good enough" visually from Objaverse-type data. Only correctness and labels resist that.
- *Medium:* channel risk. Selling through Shutterstock or CGTrader means opaque pooled payouts and default opt-ins. Selling direct means long enterprise sales cycles with a handful of buyers.

## Competitors and substitutes

| Name | Offering | Price | Model | Evidence date | URL |
|---|---|---|---|---|---|
| Shutterstock / TurboSquid | 3D & Spatial AI datasets (1.5M+ models); custom datasets; model training/eval services | Not published; 20 customers, $238M lifetime (all data deals) | Enterprise data deals; 20% contributor share (Lightricks deal); pooled Contributor Fund | 2025-26 | [1](https://www.shutterstock.com/data-licensing/3d-&-spatial), [2](https://quartr.com/events/shutterstock-inc-sstk-data-business-update-presentation_3PWD6t1U) |
| Getty Images (+ nfiniteAI) | Creative content licensing to AI; 2D→3D scenes for physical AI | Not disclosed | Multi-year deals, revenue booked early | Q4 2025; Jan 2026 | [1](https://www.barchart.com/story/news/787390/gety-q4-deep-dive-one-time-licensing-deals-drive-revenue-growth-amidst-cautious-guidance), [2](https://newsroom.gettyimages.com/en/getty-images/nfiniteai-collaborates-with-getty-images-to-bring-2d-visual-content-into-the-3d-physical-ai-era) |
| CGTrader | Tailor-made 3D datasets; custom assets built to order; enterprise AI-training licences | Quote; free sample | Enterprise deals negotiated for sellers (opted in by default) | May 2026 | [1](https://help.cgtrader.com/hc/en-us/articles/46191349842705-Can-my-models-still-be-licensed-for-AI-training), [2](https://admin.cgtrader.com/datasets) |
| Daz 3D | Licensed character/human-figure datasets | Quote | Enterprise access | n/s (2025-26) | [1](https://daz3d.com/ai-training-data) |
| A23D | 500k+ human-authored 3D models, textures, decals | Quote | Enterprise dataset licence | 2026 | [1](https://a23d-readme.static.hf.space/README.md) |
| Objaverse / Objaverse-XL | Millions of scraped Sketchfab/web 3D objects | Free | ODC-By compilation; mixed per-object licences | 2022-23 [pre-2024] | [1](https://huggingface.co/datasets/allenai/objaverse-xl/raw/main/README.md) |
| MedShapeNet | 100k+ annotated medical shapes, 23 datasets | Free | Open access; per-source licences | 2023+ [pre-2024 origin] | [1](https://arxiv.org/abs/2308.16139) |
| NVIDIA MAISI | Synthetic 3D CT + 127-class masks | Free under evaluation licence (commercial terms unclear) | Model/NIM | 2024-25 | [1](https://docs.nvidia.com/nim/medical/maisi/1.0.0/model-details.md) |
| Fundamental XR AIE | AI-generated, simulation-ready anatomy with pathology | Not found | Platform (beta) | 2025-26 | [1](https://pharmaceuticalmanufacturer.media/pharma-manufacturing-news/digital-health-in-pharma-news/fundamental-xr-launches-ai-powered-anatomy-inference-engine/) |
| IT'IS / ZMT Virtual Population | Validated whole-body simulation anatomy | Commercial fee, quote | Licence; free for research | n/s | [1](https://itis.swiss/virtual-population/virtual-population/faq/) |
| Zygote | Licensed 3D human anatomy library | Quote | Licence for animation, simulation, engineering | n/s | [1](https://solidworks.com/partner-product/zygote-human-anatomy-and-skeletal-data) |
| BioDigital | 3D anatomy platform; Content API; custom models | Quote; custom models one-time fee | SaaS/API licence + services | 2026 | [1](https://pricing.biodigital.com/business.html) |
| Atomedge | Cadaver-scan-based hyper-real anatomy model, pitched for AI training | Not seen | n/s | n/s | [1](https://keyboard-poodle-zzyx.squarespace.com) |
| Human Native (Cloudflare) | Licensed-data marketplace | n/s | Subscription, revenue share, per-use | Jan 2026 | [1](https://siliconangle.com/?p=727953) |
| Defined.ai / Troveo / Calliope | Video and image training-data brokers | $1-4/min video; $100-300/hr long video | Brokered licences | Jan 2025 | [1](https://news.bloomberglaw.com/ip-law/youtubers-are-selling-their-unused-video-footage-to-ai-companies), [2](https://www.artificialintelligence-news.com/news/ai-giants-pay-thousands-for-creators-unused-footage-to-train-models/) |
| Mercor (labour substitute or channel) | 3D artists and biomedical experts for AI training and evaluation | $24-60/hr (3D); $60-100/hr (expert art) | Hourly contract | 2025-26 | [1](https://work.mercor.com/jobs/list_AAABlYGD8f6kNvV2OWRBPJw6/3-d-artist) |

## Price points

| Item | Price | Unit / date | Type | Source |
|---|---|---|---|---|
| Unused creator video to AI firms | $1-2 standard; up to $4 premium | per minute, Jan 2025 | Reported range | [Bloomberg Law](https://news.bloomberglaw.com/ip-law/youtubers-are-selling-their-unused-video-footage-to-ai-companies) |
| Animation footage to AI firms | $2-3 | per minute, 2025 | Reported range | [Kidscreen](https://kidscreen.com/?p=221834) |
| Defined.ai buyer prices | $2/image; $2-4/short video; $100-300/hr long video | 2025 | Reported (attribution uncertain) | [AI News](https://www.artificialintelligence-news.com/news/ai-giants-pay-thousands-for-creators-unused-footage-to-train-models/) |
| Adobe Firefly video and images | avg $2.62/min (max about $7.25); $0.06-0.16/image | Apr 2024 | Reported | [PetaPixel](https://petapixel.com/2024/04/11/adobe-will-buy-your-videos-for-up-to-7-25-per-minute-to-train-ai-report) |
| Shutterstock contributor share of data deals | 20% of revenue | Jan 2025 | Reported term | [CO/AI](https://getcoai.com/news/shutterstock-lightricks-partnership-offers-example-of-how-to-ethically-source-training-data-for-ai-video) |
| Shutterstock data licensing book | $238M lifetime, 20 customers (≈$12M avg) | Jul 2025 | Company update (attribution uncertain); average is my arithmetic | [Quartr](https://quartr.com/events/shutterstock-inc-sstk-data-business-update-presentation_3PWD6t1U) |
| Shutterstock Data, Distribution & Services | $203.3M | FY2025 | Reported | [Yahoo Finance](https://finance.yahoo.com/news/shutterstock-sstk-reports-989-9m-114655765.html) |
| Reddit data licensing | about $140M; Google about $60M/yr; OpenAI about $70M/yr (est.) | FY2025 | Reported/estimated | [Crypto Briefing](https://cryptobriefing.com/reddit-data-licensing-revenue-openai-google/) |
| News Corp-OpenAI | >$250M / 5 yrs | May 2024 | Reported | [Quartz](https://qz.com/ai-training-data-pricing-licensing-deals-market-052126) |
| NYT-Amazon | $20-25M/yr | 2025 | Reported | [Engadget](https://www.engadget.com/ai/the-new-york-times-and-amazons-ai-licensing-deal-is-reportedly-worth-up-to-25-million-per-year-135523853/) |
| Le Monde + Prisa (OpenAI offer) | $1-5M | 2024-25 | Reported | [Neudata](https://www.neudata.co/blog/ai-data-licensing-market-analysis) |
| Mercor 3D artist / expert artist | $24-60/hr; $60-100/hr | 2025-26 | Posted rates | [Mercor](https://work.mercor.com/jobs/list_AAABlYGD8f6kNvV2OWRBPJw6/3-d-artist), [Mercor](https://work.mercor.com/jobs/list_AAABm5NePFoYr4KV3olKurwc/fine-artists-including-painters-sculptors-and-illustrators) |
| Rigged anatomy, retail marketplace (not AI rights) | $149-2,399 | per asset, 2026 | List (follow-up A) | [TurboSquid](https://www.turbosquid.com/3d-models/male-female-anatomy-set-3d-model-1594415) |
| TurboSquid Enhanced Licence | +$10,000 indemnification | 2026 | Licence tier (follow-up A) | [TurboSquid](https://www.turbosquid.com/3d-model/enhanced-licenses/anatomy/rig/gltf) |
| **Inference:** non-exclusive AI-training licence for a validated biomedical set (about 100-300 assets with labels and dossiers) | $10k-75k per buyer | one-off or annual | Low confidence; no direct comparable | n/a |
| **Inference:** custom biomedical dataset or eval-set build to spec | $20k-150k per project | project | Low confidence; anchored on CGTrader/Shutterstock "custom" offers and studio day rates | n/a |
| **Inference:** anatomy/mechanism evaluation-set subscription | $5k-30k per year per buyer | annual | Low confidence | n/a |
| **Inference:** same library sold at video-style volume rates | hundreds to low thousands of dollars in total | one-off | Medium confidence that this is the floor | n/a |

## Evidence against

1. **No anatomical buyer found.** None of the named buyers showed any 2024-2026 purchase of anatomical 3D data: the AI 3D/video firms, BioRender, Fundamental XR, NVIDIA, and the surgical and imaging AI firms. The gap rests on analogy, not observed demand.
2. **Medical AI uses patient-derived data.** MAISI, Fundamental XR AIE and Inner Logic all train on CT, MRI, surgical video or pathology, not sculpted meshes. Artist anatomy sits in the wrong data domain for them.
3. **Free and synthetic substitutes exist:** MedShapeNet (100k+ shapes), the Virtual Body CC model, MAISI and Objaverse.
4. **Value sits with scale and aggregators.** Shutterstock and Getty, now merging, already sell "rights-cleared" 3D at scale. CGTrader has pulled AI rights into its own enterprise deals. A small library is a supplier to them, not a peer.
5. **Payouts are poor or opaque.** TurboSquid's pooled fund draws petitions and complaints of missing payments.
6. **Revenue is lumpy:** Getty booked early and warned of a hard comparison; Shutterstock's Q4 data line fell 19%.
7. **Accuracy errors are about reasoning, not geometry.** The SurgVeo errors were mostly reasoning and procedure. Better meshes alone may not move buyers.
8. **Competing studio libraries already exist** (SciePro, VOKA, Zygote, ViP: follow-up A, track 4) and can opt into AI deals faster.

## Still unknown

- Actual per-asset or per-dataset prices in any 3D AI-training deal: Shutterstock 3D & Spatial, CGTrader enterprise, Deemos-Shutterstock, Daz, A23D.
- CGTrader's seller royalty share for Custom Enterprise Deals (General Terms §18.12-18.13 not seen).
- Whether Meshy, Tripo, Deemos, Luma, Runway, Google or OpenAI have any biomedical or anatomy data programme, evaluation set or vendor.
- Whether BioRender buys any outside content, and whether its 3D or animation plans need 3D source data.
- Fundamental XR AIE's data sources, pricing and accuracy.
- Whether AI 3D firms would pay for an anatomy evaluation set. No benchmark sales were found in any domain.
- Commercial terms for NVIDIA MAISI outputs, and per-source licences for MedShapeNet.
- The relationship, if any, between the founder and Atomedge, and Atomedge's AI-licensing terms.
- Medical imaging dataset per-scan prices. None were found, so there is no anchor from adjacent medical data markets.

## Sources

1. Shutterstock (SSTK) Reports $989.9M Revenue in 2025, Yahoo Finance, Feb 2026. https://finance.yahoo.com/news/shutterstock-sstk-reports-989-9m-114655765.html
2. Shutterstock Reports Full Year 2025 and Fourth Quarter Financial Results, Shutterstock IR, Feb 2026. https://shutterstock.gcs-web.com/node/14551
3. Shutterstock Data Business Update Presentation summary, Quartr, Jul 2025. https://quartr.com/events/shutterstock-inc-sstk-data-business-update-presentation_3PWD6t1U
4. Shutterstock Builds on Data Licensing Strength with New AI Services, Nasdaq/Shutterstock PR, Oct 2025. https://www.nasdaq.com/press-release/shutterstock-builds-data-licensing-strength-new-ai-services-model-training-and
5. Shutterstock Announces Major Expansion of Licensed Training Datasets, Shutterstock IR, Mar 2026. https://investor.shutterstock.com/node/14596
6. AI Model Development Training Data Scarcity (Shutterstock Studios), LBB Online, Jun 2026. https://lbbonline.com/news/AI-Model-Development-Training-Data-Scarcity-Shutterstock-Studios
7. 3D & Spatial data licensing, Shutterstock, n/s. https://www.shutterstock.com/data-licensing/3d-&-spatial
8. Shutterstock-Lightricks partnership, CO/AI, Jan 2025. https://getcoai.com/news/shutterstock-lightricks-partnership-offers-example-of-how-to-ethically-source-training-data-for-ai-video
9. NVIDIA and Shutterstock to launch AI-based text-to-3D service, CG Channel, 21 Mar 2023 [pre-2024]. https://www.cgchannel.com/2023/03/nvidia-and-shutterstock-to-launch-ai-based-text-to-3d-service
10. Edify 3D model card, NVIDIA, 2024. https://build.nvidia.com/shutterstock/edify-3d/modelcard
11. Update on our generative 3D partnership with NVIDIA, TurboSquid/Squid, n/s. https://resources.squid.io/artist-blog/update-on-our-generative-3d-partnership-with-nvidia
12. What are Shutterstock datasets / data deals?, TurboSquid, n/s. https://resources.turbosquid.com/?p=19881
13. GETY Q4 deep dive: one-time licensing deals drive revenue growth, Barchart, Mar 2026. https://www.barchart.com/story/news/787390/gety-q4-deep-dive-one-time-licensing-deals-drive-revenue-growth-amidst-cautious-guidance
14. Getty, Perplexity sign multi-year licensing deal, The Star (Reuters), 31 Oct 2025. https://www.thestar.com.my/tech/tech-news/2025/10/31/getty-perplexity-sign-multi-year-licensing-deal-to-boost-ai-powered-search-visuals
15. nfiniteAI collaborates with Getty Images (3D physical AI), Getty newsroom, Jan 2026. https://newsroom.gettyimages.com/en/getty-images/nfiniteai-collaborates-with-getty-images-to-bring-2d-visual-content-into-the-3d-physical-ai-era
16. Getty Images tag page (Getty-Shutterstock merger), CG Channel, n/s. https://www.cgchannel.com/tag/getty-images
17. Can my models still be licensed for AI training?, CGTrader Help, 2026. https://help.cgtrader.com/hc/en-us/articles/46191349842705-Can-my-models-still-be-licensed-for-AI-training
18. What is a Custom Enterprise Deal?, CGTrader Help, 2026. https://help.cgtrader.com/hc/en-us/articles/46191760965137-What-is-a-Custom-Enterprise-Deal-and-how-does-it-affect-my-earnings-as-a-seller
19. Optimized 3D Model Datasets for Next-Gen AI, CGTrader, n/s. https://admin.cgtrader.com/datasets
20. 3D model datasets for generative AI, CGTrader Arsenal, n/s. https://arsenal.cgtrader.com/3d-model-datasets-for-generative-ai
21. CGTrader Analytics Terms of Service, CGTrader, n/s. https://cgtrader.com/pages/cgtrader-analytics-terms-of-service
22. Responsible 3D AI Training Data at Scale, Daz 3D, n/s. https://daz3d.com/ai-training-data
23. AI Datasets for Characters, Daz 3D, n/s. https://www.daz3d.com/ai-datasets
24. A23D README, A23D (Hugging Face), 2026. https://a23d-readme.static.hf.space/README.md
25. A23D organisation, Hugging Face, n/s. https://huggingface.co/A23D
26. Sketchfab & Objaverse: AI copyright dispute enters third dimension, The Decoder, n/s (likely 2023) [pre-2024]. https://the-decoder.com/sketchfab-objaverse-ai-copyright-dispute-enters-third-dimension/
27. Objaverse raises concerns about ethics of scraping 3D content, FlippedNormals, n/s (likely 2023) [pre-2024]. https://blog.flippednormals.com/objaverse-raises-concerns-about-ethics-of-scraping-3d-content/
28. Objaverse-XL README, Allen AI (Hugging Face), 2023 [pre-2024]. https://huggingface.co/datasets/allenai/objaverse-xl/raw/main/README.md
29. Reddit's data licensing revenue grows 24% to $43M, Crypto Briefing, 2026. https://cryptobriefing.com/reddit-data-licensing-revenue-openai-google/
30. Reddit's data revenue: OpenAI, Google buyers, Motley Fool, 17 Aug 2026. https://www.fool.com/investing/2026/08/17/reddits-data-revenue-openai-google-buyers/
31. Reddit's AI Curse (Q2 2026 earnings), FourWeekMBA, 2026. https://fourweekmba.com/ai-reddit-ai-curse-q2-2026-earnings/
32. NYT and Amazon AI licensing deal reportedly worth up to $25M per year, Engadget, 2025. https://www.engadget.com/ai/the-new-york-times-and-amazons-ai-licensing-deal-is-reportedly-worth-up-to-25-million-per-year-135523853/
33. Every AI Content Licensing Deal, Mapped (2023-2026), LLM Pulse, 2026. https://llmpulse.ai/blog/ai-content-licensing-deals/
34. Feeding the machines (AI data licensing market analysis), Neudata, Jun 2025. https://www.neudata.co/blog/ai-data-licensing-market-analysis
35. AI training data pricing and licensing deals market, Quartz, May 2026. https://qz.com/ai-training-data-pricing-licensing-deals-market-052126
36. A $67.5B market emerges for licensing creative work to train AI, CO/AI, 2025. https://getcoai.com/news/a-67-5b-market-emerges-for-licensing-creative-work-to-train-ai
37. YouTubers Are Selling Their Unused Video Footage to AI Companies, Bloomberg Law, Jan 2025. https://news.bloomberglaw.com/ip-law/youtubers-are-selling-their-unused-video-footage-to-ai-companies
38. OpenAI and Google are buying YouTubers' unpublished videos for up to $4 per minute, The Decoder, Jan 2025. https://the-decoder.com/openai-and-google-are-buying-youtubers-unpublished-videos-for-up-to-4-per-minute/
39. AI Companies Are Paying Content Creators For Their Unpublished Videos, PetaPixel, 13 Jan 2025. https://petapixel.com/2025/01/13/ai-companies-are-paying-content-creators-for-their-unpublished-videos
40. Decoding the opportunity for selling content to AI firms, Kidscreen, 2025. https://kidscreen.com/?p=221834
41. AI giants pay thousands for creators' unused footage, AI News, 2025. https://www.artificialintelligence-news.com/news/ai-giants-pay-thousands-for-creators-unused-footage-to-train-models/
42. Adobe Will Buy Your Videos for Up to $7.25 Per Minute, PetaPixel, 11 Apr 2024. https://petapixel.com/2024/04/11/adobe-will-buy-your-videos-for-up-to-7-25-per-minute-to-train-ai-report
43. Adobe buying videos for AI, The Register, 12 Apr 2024. https://www.theregister.com/2024/04/12/adobe_buying_videos_ai
44. Adobe is buying videos to train its new AI tool, ZDNet, Apr 2024. https://www.zdnet.com.au/article/adobe-is-buying-videos-to-train-its-new-ai-generator-but-are-they-paying-enough/
45. Medical imaging dataset listing, AWS Marketplace, n/s. https://aws.amazon.com/marketplace/pp/prodview-qcoatqz6wf7n6
46. Hyper3D.AI Secures Commercial License For 3D Assets From Shutterstock, Hyper3D blog, Dec 2025. https://hyper3d.ai/blog/hyper3d-shutterstock
47. Hyper3D acquires commercial 3D asset license from Shutterstock, PressAdvantage, 16 Dec 2025. https://business.ricentral.com/ricentral/article/pressadvantage-2025-12-16-hyper3d-acquires-commercial-3d-asset-license-from-shutterstock-and-announces-cooperation-with-blender
48. Meshy raises nearly $400 million in Series B, 3Dnatives, 21 Jul 2026. https://www.3dnatives.com/en/meshy-400-million-in-series-b-21072026/
49. Data Artist at Meshy, Chopping Block, n/s. https://www.choppingblock.ai/jobs/data-artist-at-meshy
50. Tripo AI raises 3 billion yuan in Series B and B+, 3Dnatives, Sep 2026. https://www.3dnatives.com/en/tripo-ai-raises-3-billion-yuan-04092026/amp/
51. Machine Learning Data Engineer (Stability AI), Simplify, 18 Nov 2025. https://simplify.jobs/p/0cf76fa8-22f8-458b-94ad-b5b35e706d08/Machine-Learning-Data-Engineer
52. 3D Artist (AI project), Mercor, 2025-26. https://work.mercor.com/jobs/list_AAABlYGD8f6kNvV2OWRBPJw6/3-d-artist
53. Fine Artists, Including Painters, Sculptors, and Illustrators, Mercor, 2026. https://work.mercor.com/jobs/list_AAABm5NePFoYr4KV3olKurwc/fine-artists-including-painters-sculptors-and-illustrators
54. Biomedical Scientist – AI Trainer (Mercor), Career.com, Apr 2026. https://www.career.com/job/mercor/biomedical-scientist-ai-trainer/j202604281006073001191
55. BioRender launches AI agent for building scientific research images, BetaKit, Oct 2026. https://betakit.com/biorender-launches-ai-agent-for-building-scientific-research-images/
56. Fundamental XR launches AI-powered Anatomy Inference Engine, Pharmaceutical Manufacturer, n/s (2025-26). https://pharmaceuticalmanufacturer.media/pharma-manufacturing-news/digital-health-in-pharma-news/fundamental-xr-launches-ai-powered-anatomy-inference-engine/
57. FundamentalXR company profile, IntuitionLabs, n/s. https://intuitionlabs.ai/companies/digital-health/fundamentalxr
58. Fundamental XR and Elsevier launch mixed reality innovation program, HIT Consultant, 13 Nov 2025. https://hitconsultant.net/2025/11/13/fundamental-xr-and-elsevier-launch-mixed-reality-innovation-program-for-enterprise-ai
59. MAISI: Medical AI for Synthetic Imaging, arXiv 2409.11169, Sep 2024. https://arxiv.org/html/2409.11169v1
60. MAISI NIM model details, NVIDIA docs, 2024-25. https://docs.nvidia.com/nim/medical/maisi/1.0.0/model-details.md
61. NVIDIA developer blog on MAISI synthetic data, NVIDIA, 2024-25. https://developer.nvidia.com/blog/?p=83468
62. Inner Logic simulation infrastructure, HIT Consultant, 27 Jul 2026. https://hitconsultant.net/2026/07/27/inner-logic-simulation-infrastructure-procedural-devices/
63. Inner Logic raises $11.5M, Dealroom, 2026. https://dealroom.co/news/145393-inner-logic-raises-11-5m-to-simulate-surgery-on-thousands-of-virtual-pat
64. XRlabs raises $8.4M, MobiHealthNews, 2025-26. https://www.mobihealthnews.com/news/xrlabs-raises-84m-ai-surgical-platform
65. Cambridge-based AnthroTek closes £950k seed, StartupRise, Jun 2025. https://startuprise.co.uk/cambridge-based-anthrotek-closes-950k-seed-funding/
66. Redefine Surgery raises $10M pre-seed, Signalbase, n/s. https://www.trysignalbase.com/news/funding/redefine-surgery-raises-10m-pre-seed-round
67. BioDigital business pricing, BioDigital, 2026. https://pricing.biodigital.com/business.html
68. Zygote Human Anatomy and Skeletal Data, SolidWorks partner page, n/s. https://solidworks.com/partner-product/zygote-human-anatomy-and-skeletal-data
69. Virtual Population FAQ, IT'IS Foundation, n/s. https://itis.swiss/virtual-population/virtual-population/faq/
70. Virtual Population brochure, IT'IS Foundation, ~2017 [pre-2024]. https://itis.swiss/assets/Downloads/VirtualPopulation/1706-virtual-population-web.pdf
71. Hyper-Realistic 3D Anatomy Model (Atomedge), Atomedge, n/s. https://keyboard-poodle-zzyx.squarespace.com
72. 3D anatomy model published under CC licence, Virtual Body, n/s. https://www.virtual-body.org/news/3d-anatomy-model-published-under-cc-license/
73. MedShapeNet: a large-scale dataset of 3D medical shapes, arXiv 2308.16139, Aug 2023 onwards [pre-2024 origin]. https://arxiv.org/abs/2308.16139
74. TurboSquid Enhanced Licence anatomy rigs, TurboSquid, n/s (via follow-up A). https://www.turbosquid.com/3d-model/enhanced-licenses/anatomy/rig/gltf
75. Full Male and Female Anatomy Set (Blender Rigged), TurboSquid, n/s (via follow-up A). https://www.turbosquid.com/3d-models/male-female-anatomy-set-3d-model-1594415
76. Cloudflare acquires Human Native, SiliconANGLE, 15 Jan 2026. https://siliconangle.com/?p=727953
77. Cloudflare Acquires Human Native, LAVX News, Jan 2026. https://news.lavx.hu/article/cloudflare-acquires-human-native-to-build-compensated-ai-training-data-ecosystem
78. Cloudflare's play: warehouse or toll booth or both, Kaptur, 2026. https://kaptur.co/cloudflares-play-warehouse-or-toll-booth-or-both/
79. Google's Veo 3 can fake surgical videos but misses every hint of medical sense, The Decoder, 2025. https://the-decoder.com/googles-veo-3-can-fake-surgical-videos-but-misses-every-hint-of-medical-sense/
80. JMIR Medical Education Vol 11 article e80084, JMIR, 2025. https://mededu.jmir.org/2025/1/e80084
81. Sora and medical education commentary, Canadian Medical Education Journal, 2024. https://journalhosting.ucalgary.ca/index.php/cmej/article/download/79065/57851/258885
82. Shutterstock/TurboSquid: stop exploiting 3D artists (petition), Change.org, n/s. https://www.change.org/p/shutterstock-turbosquid-stop-exploiting-3d-artists-demand-transparency-and-fair-pay
83. Artists threaten to leave TurboSquid because of plummeting sales, missing payments, 80.lv, n/s. https://80.lv/articles/artists-threaten-to-leave-turbosquid-because-of-plummeting-sales-missing-payments
84. Artistas de TurboSquid denuncian caída de ventas por culpa de la IA, Foro3D, 15 Jul 2026. https://foro3d.com/2026/julio/artistas-de-turbosquid-denuncian-caida-de-ventas-por-culpa-de-la-ia.html
