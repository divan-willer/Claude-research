# Track 3: Supply-side pain

Method note. WebSearch worked; WebFetch failed on every host tried (DNS resolution error in this sandbox: clarafi.com, cgchannel.com, pie.med.utoronto.ca, extensions.blender.org). I stopped retrying as the error instructed. The shared web-search budget then ran out after about 39 searches. So every citation below is a search-result snippet, marked "(snippet)". No page was opened. A fact-checker should open the load-bearing URLs first.

## Summary

**Tool layer: the Maya-side molecular and soft-tissue tools are stale or gone. Blender's equivalent is active and free.**

- Clarafi's Molecular Maya (mMaya) page lists support for "OSX & Windows: Maya 2018-2020, Linux: Maya 2020". It says Maya 2022 is not yet supported because of Python 3 integration work [source](https://clarafi.com/tools/mmaya/) (snippet). A Clarafi forum post hoped for a Maya 2022 version in Q1 2022 [source](https://clarafi.com/topic/maya-2022-version/) (snippet) [pre-2024, possibly stale]. I found no evidence that version shipped.
- Maya has been Python-3-only since Maya 2023 [source](https://www.riggingdojo.com/2022/03/31/autodesk-2023/) (snippet) [pre-2024]. Autodesk had shipped Maya 2026.3 by the time of this research [source](https://help.autodesk.com/cloudhelp/2026/ENU/Maya-ReleaseNotes/files/MAYA_RELEASENOTES_2026_3_RELEASE_NOTES_HTML.html) (snippet).
- Inference (confidence: medium): if Clarafi's compatibility list is current, mMaya has not run on any Maya release of the last four years. Maya-based molecular animators have no maintained native toolkit.
- ePMV's GitHub still lists Cinema4D 12, Blender 2.49 and Maya 2011 as hosts [source](https://github.com/corredD/ePMV) (snippet). Its website says it is being migrated and some links may be broken [source](https://epmv.scripps.edu/) (snippet).
- Molecular Nodes for Blender is active. Version 4.5.12 is dated 17 March 2026 and supports Blender 5.1 [source](https://extensions.blender.org/add-ons/molecularnodes/versions/) (snippet). It got a NumFOCUS grant in December 2024 for a scripting API [source](https://www.mdanalysis.org/2024/12/12/sdg_molecularnodes/) (snippet). Its developers say "multiple professional scientific animation studios" use it. That is a self-report [source](https://proteins-2024.p.asnevents.com.au/days/2024-02-05/abstract/101827) (snippet).
- Unity stopped selling and supporting Ziva VFX on 2 April 2024. Subscribers could convert to five-year licences, and DNEG received an exclusive perpetual licence to the IP [source](https://www.cgchannel.com/2024/04/unity-discontinues-the-ziva-products/), [source](https://3dvf.com/unity-met-fin-a-la-vente-et-au-support-de-ziva-dneg-en-acquiert-les-droits/) (snippets). In March 2026, CG Channel wrote that this "left Maya artists without a simple off-the-shelf solution" for soft tissue. It asked whether AdonisFX 2.0 could fill that gap [source](https://www.cgchannel.com/2026/03/is-adonisfx-2-0-the-new-ziva-vfx/) (snippet).

**Rigging and simulation: artists improvise.**

- On the SideFX forum, artists ask how to make a Vellum heart contract. One reply points them to a tetrahedral soft body with fibre constraints [source](https://sidefx.com/forum/topic/96072), [source](https://www.sidefx.com/forum/topic/82147/) (snippets). One heart setup came with the caveat "I claim no physical accuracy here at all, just 'does it look goopy'" (same threads, snippet).
- I found no peristalsis rig tutorial or product for Maya or Blender. The closest material was generic sine, bend and soft-mod deformer tutorials [source](https://lesterbanks.com/2020/02/how-to-create-a-rolling-or-coiling-rig-in-maya/) (snippet). That is an absence of search results, which is weak evidence.

**Assets: the market is large but generic. Rigged, documented, commercial-safe biological rigs are rare.**

- A TurboSquid "virus" search showed price-filter counts that add up to about 3,591 results [source](https://www.turbosquid.com/ko/Search/3D-Models/virus) (snippet; the cache date is unclear).
- Rigged hearts sell for $15 to $299. One $20 rigged heart is licensed for editorial use only [source](https://www.turbosquid.com/3d-models/heart-animation-human-heart-beating-2444833) (snippet). A $299 "rigged and animated" heart has a licence that excludes AI use [source](https://www.cgtrader.com/3d-models/science/medical/human-heart-rigged-and-animated) (snippet).
- A buyer review of a $29 animated lung model says the animation only works in 3ds Max [source](https://www.cgtrader.com/3d-models/character/anatomy/lungs-animated) (snippet).
- None of the listings I saw cited anatomical sources or expert review.

**Counter-evidence: studios already reuse assets in-house.**

- VOKA advertises a catalogue of more than 1,000 ready-made models and reuses assets to cut costs [source](https://voka.io/3d-scientific-animation-services/molecular-biology/) (snippet).
- Mainframe builds asset libraries so content can be reused and localised [source](https://mainframeuk.squarespace.com/medical-animation) (snippet).
- Hybrid Medical Animation rendered a tumour scene with more than 10 million cells using Houdini procedurals [source](https://www.stashmedia.tv/?p=100441) (snippet).
- Inference (confidence: medium): large studios do not "rebuild per project". Small studios and freelancers probably do. They are the likelier buyers of assets.

**Review and economics.**

- AXS Studio describes two script review rounds and two storyboard rounds before formal MLR (medical, legal and regulatory) review. It asks clients to come four months ahead [source](https://axs3d.com/locations/) (snippet).
- An MLR vendor says teams plan four to eight weeks for MLR review, and much of that time is lost to version confusion [source](https://www.informait.com/blog/the-mlr-delay-nobody-budgets-for) (snippet).
- Studio price guides put freelance work at $1.5k–$4k per finished minute and studio work at $5k–$20k [source](https://voka.io/medical-animation-cost/) (snippet).
- The Association of Illustrators' 2026 survey found that 46% of 549 illustrators had lost work to AI, up from 32% the year before. 31% said clients expect lower fees [source](https://www.resultsense.com/news/2026-11-04-aoi-illustrators-generative-ai-survey-2026/) (snippet). This survey covers general illustrators, not medical ones.
- VOKA (2026) says AI speeds up concept work, cleanup and localisation. It also says anatomy, scale and medical claims still need expert review [source](https://voka.io/?p=15477) (snippet).

**Professional bodies.** I found no "ASMI"; it is probably a variant of AMI. Inference (confidence: medium). AMI's 2026 call for proposals listed AI and 3D animation workshops as topics [source](https://www.surveymonkey.com/r/ami2026proposals) (snippet). IMI 2026 (Glasgow) mentions AI-informed workflows [source](https://www.imi.org.uk/conference2026/) (snippet).

**Overall inference (confidence: medium).** The clearest gap that fits Divan is motion-ready biological rigs with documented sources and a licence safe for pharma work: organs, cell processes and microbes. Maya users lost Ziva and Molecular Maya, so it is sharpest for them. Risks: a small buyer pool, free Molecular Nodes, and in-house studio libraries.

## Hypothesis check

| ID | Verdict | Key evidence | Strongest counter-evidence |
|---|---|---|---|
| H1 | partly supported | Rigged organs on marketplaces come as baked animation with mixed licences: a $20 heart is editorial-only ([TurboSquid](https://www.turbosquid.com/3d-models/heart-animation-human-heart-beating-2444833)); a $299 heart excludes AI use ([CGTrader](https://www.cgtrader.com/3d-models/science/medical/human-heart-rigged-and-animated)); a lung animation is 3ds-Max-only per a buyer review ([CGTrader](https://www.cgtrader.com/3d-models/character/anatomy/lungs-animated)). No listing seen cites sources or review. mMaya's molecular kits are tied to Maya 2018–2020 ([Clarafi](https://clarafi.com/tools/mmaya/)). ePMV lists hosts from about 2011 ([GitHub](https://github.com/corredD/ePMV)). All snippets. | Studios already keep internal libraries: VOKA has 1,000+ models ([VOKA](https://voka.io/3d-scientific-animation-services/molecular-biology/)); Mainframe ([Mainframe](https://mainframeuk.squarespace.com/medical-animation)); a studio's "protein cards" library ([blog](https://reindeer-haddock-glja.squarespace.com/blog/from-pdb-to-production-how-to-prep-protein-structures-for-3d-animation)). Free sources cover molecules and some cells: NIH 3D ([NIH 3D](https://3d.nih.gov/faqs)) and Molecular Nodes, active in 2026 ([Blender Extensions](https://extensions.blender.org/add-ons/molecularnodes/versions/)). There are about 3,591 generic virus models on TurboSquid ([TurboSquid](https://www.turbosquid.com/ko/Search/3D-Models/virus)). All snippets. |
| H2 | partly supported (supply-side view only) | VOKA says expert review is still needed even with AI ([VOKA](https://voka.io/?p=15477)). Frontiers retracted a paper with Midjourney figures three days after publication in February 2024 ([Gizmodo](https://gizmodo.com/science-journal-rat-dck-ai-generated-images-retracted-1851297606)). "No AI" clauses are reported as common in pharma clinical-research agreements ([Contract Network](https://thecontractnetwork.com/the-end-of-no-ai-clauses-in-clinical-research-agreements/)). Marketplace licences now exclude AI use ([CGTrader](https://www.cgtrader.com/3d-models/science/medical/human-heart-rigged-and-animated)). All snippets. | I found no evidence that studio capacity is short. The evidence points to price pressure instead: AOI 2026 says 31% of illustrators report clients expect lower fees ([Resultsense](https://www.resultsense.com/news/2026-11-04-aoi-illustrators-generative-ai-survey-2026/)), and Upwork lists a medical animator at $35/hr ([Upwork](https://www.upwork.com/hire/medical-animation-freelancers/pk/)). I found no "No AI" clause in an actual animation contract, and the source above argues such clauses are ending. |
| H3 | insufficient evidence | Weak signals only: Mainframe builds reusable systems to localise content ([Mainframe](https://mainframeuk.squarespace.com/medical-animation)); VOKA says AI speeds localisation ([VOKA](https://voka.io/?p=15477)); Random42 builds patient-education tools in Unity ([Unity](https://unity.com/en/resources/random42)). All snippets. | The localisation claims suggest studios already offer this, which cuts against "underserved". My track did not look at patient-facing demand. |
| H4 | partly supported (supply of assets only) | I found no Staphylococcus model in searches. Commercial E. coli models make unreviewed accuracy claims ([CGTrader](https://www.cgtrader.com/3d-models/science/medical/escherichia-coli-e-coli-bacterium)). One virus app ships only two 3D models ([App Store](https://apps.apple.com/ky/app/learn-viruses/id1603794565)). All snippets. | Multi-species packs exist: DOSCH has 50 bacteria ([DOSCH](https://doschdesign.com/products/3d/Medical_Bacteria.html)), Ithappy has 190+ microbe assets ([Ithappy](https://ithappystudios.com/props/viruses)), and a CGTrader pack has 17 ([CGTrader](https://www.cgtrader.com/3d-model-packs/microscopic-life-collection-01)). NIH 3D hosts CC-BY E. coli models ([NIH 3D](https://3d.nih.gov/entries/3DPX-017981)), and CellWalk covers Mycoplasma ([App Store](https://apps.apple.com/app/cellwalk/id1627776848)). I did not assess demand. All snippets. |

## Top 3 candidate gaps

### Gap 1. Validated "living anatomy" rig kits: organs, cell processes and microbes with documented sources and commercial-safe licences

**Problem.** Medical animators need organs and cell structures that move correctly. Examples: a contracting heart, lungs with the diaphragm, peristalsis, ciliary beat, membrane budding and fusion, cell division, flagellar motion. Marketplace items are mostly baked animation, locked to one program, licensed inconsistently, and come with no record of sources or expert review. Larger studios build their own; smaller ones and freelancers rebuild or improvise.

**Evidence**
- Rigged or animated hearts list at $15, $139, $275 and $299 on CGTrader, and $20 on TurboSquid. The $20 one is editorial-use only, and the $299 one excludes AI use ([TurboSquid](https://www.turbosquid.com/3d-models/heart-animation-human-heart-beating-2444833), [CGTrader $299](https://www.cgtrader.com/3d-models/science/medical/human-heart-rigged-and-animated), [CGTrader $15](https://www.cgtrader.com/3d-models/science/medical/realistic-3d-animated-human-heart), [CGTrader $139](https://www.cgtrader.com/3d-models/character/human-anatomy/human-heart-beat-animated-for-blender), [CGTrader $275](https://www.cgtrader.com/3d-models/science/medical/animated-heart-inside-ribcage)) (snippets).
- Lungs: a $69.99 animated cross-section tagged "rigged" (Maya, about 7,400 polygons) ([CGTrader](https://cgtrader.com/3d-models/science/medical/cross-section-human-lungs)). A $29 animated lung whose buyer review says the animation only works in 3ds Max ([CGTrader](https://www.cgtrader.com/3d-models/character/anatomy/lungs-animated)). A full animated thorax at about $499 ([CGTrader](https://cgtrader.com/3d-models/character/anatomy/human-anatomy-nimated-skeleton-and-internal-organs)) (snippets).
- Soft-tissue tooling gap in Maya after Ziva was discontinued ([CG Channel 2026](https://www.cgchannel.com/2026/03/is-adonisfx-2-0-the-new-ziva-vfx/)). Houdini users improvise heart contraction ([SideFX forum](https://sidefx.com/forum/topic/96072)) (snippets).
- Researchers still publish methods for "self-driven" heart, lung and kidney deformation, aimed at medical training ([arXiv 2401.11614, Jan 2024](https://www.arxiv.org/abs/2401.11614)) (snippet).
- Microbes: generic virus models are plentiful, but I found no Staphylococcus model. Accuracy claims on bacteria models come from the sellers ([CGTrader E. coli](https://www.cgtrader.com/3d-models/science/medical/escherichia-coli-e-coli-bacterium), [TurboSquid virus search](https://www.turbosquid.com/ko/Search/3D-Models/virus)) (snippets).
- Large studios keep their own libraries, which caps this market at the top end ([VOKA](https://voka.io/3d-scientific-animation-services/molecular-biology/), [Mainframe](https://mainframeuk.squarespace.com/medical-animation)) (snippets).

**Who pays.** Freelance medical animators. Small medical-animation studios (2–20 staff). Med-ed and e-learning content producers. Surgical-sim and XR developers. Technical directors at mid-size studios who would buy rigs instead of building them. Buyers inside pharma agencies are indirect.

**Rough price points.**
- List prices in USD, from search snippets captured November 2026:
  - rigged or animated hearts $15–$299
  - full animated thorax about $499
  - animated lungs $5–$69.99
  - microbe and cell packs $2.99–$30 ([Superhive](https://superhivemarket.com/products/biological-research-3dassets-pack), [CGTrader](https://www.cgtrader.com/3d-models/science/medical/medical-microscopic-infographics-pack-cells-viruses-and-dna))
- I have no deal prices.
- Context: studio work runs about $5k–$20k per finished minute ([VOKA](https://voka.io/medical-animation-cost/)) (snippet).
- Inference (confidence: low): a documented, multi-program, commercially licensed rig kit could list at USD 200–1,500 per seat, with studio site licences higher. That price is untested.

**Competitors / substitutes.**
- In-house studio libraries.
- CGTrader, TurboSquid and Fab sellers. SciePro sells "medically accurate" static anatomy via TurboSquid ([TurboSquid blog 2023](https://blog.turbosquid.com/2023/04/03/how-sciepro-created-the-most-anatomically-accurate-model-on-the-market/)) [pre-2024, possibly stale].
- Zygote. Pricing was not visible ([Zygote](https://www.zygotebody.com/pricing)).
- NIH 3D, free and CC-BY ([NIH 3D](https://3d.nih.gov/faqs)).
- Houdini procedural setups.
- Nucleus library licensing for finished animations ([Knowlify](https://knowlify.com/articles/best-medical-healthcare-animation-agencies)).

All snippets.

**Founder fit.** Direct: hyper-realistic anatomical sculpting plus Maya rigging (mGear, custom deformers). He can ship Maya and Blender versions.

**Confidence.** Medium.

### Gap 2. A maintained Maya bio-toolkit: molecular import and biological-motion deformers to replace Molecular Maya, ePMV and Ziva for this niche

**Problem.** Maya users in biomedical animation lost their native molecular toolkit (mMaya is tied to Maya 2018–2020) and their soft-tissue solver (Ziva). Blender users have Molecular Nodes. Maya users have nothing maintained for PDB import, mesoscale packing, or biological motion presets such as ciliary fields, peristaltic waves, membrane deformation and cardiac contraction.

**Evidence**
- mMaya compatibility stops at Maya 2018–2020, and Maya 2022 was "not yet supported" because of Python 3 work ([Clarafi](https://clarafi.com/tools/mmaya/), [Clarafi forum](https://clarafi.com/topic/maya-2022-version/)) (snippets) [pre-2024, possibly stale].
- An Autodesk forum user found mMaya support listed only up to 2019 ([Autodesk Community](https://forums.autodesk.com/t5/maya-forum/molecular-maya/td-p/9256999)) (snippet) [pre-2024].
- Maya has been Python 3 only since 2023 ([Rigging Dojo](https://www.riggingdojo.com/2022/03/31/autodesk-2023/)), and Maya 2026.3 is current ([Autodesk](https://help.autodesk.com/cloudhelp/2026/ENU/Maya-ReleaseNotes/files/MAYA_RELEASENOTES_2026_3_RELEASE_NOTES_HTML.html)) (snippets).
- ePMV hosts are from about 2011 ([GitHub](https://github.com/corredD/ePMV)) (snippet).
- Ziva was discontinued on 2 April 2024 ([CG Channel](https://www.cgchannel.com/2024/04/unity-discontinues-the-ziva-products/), [Unity Discussions](https://discussions.unity.com/t/ziva-products-discontinued-no-longer-part-of-unity/943600)). AdonisFX 2.0 and HézFX are emerging replacements, but they target VFX and games characters, not organs or cells ([CG Channel 2026](https://www.cgchannel.com/2026/03/is-adonisfx-2-0-the-new-ziva-vfx/), [80.lv](https://80.lv/articles/artist-shows-ziva-vfx-inspired-muscle-simulation-plug-in-for-3ds-max-maya)) (snippets).
- ChimeraX-to-Blender users struggle with over-dense meshes and bloated GLB files ([ChimeraX list](https://mail.cgl.ucsf.edu/mailman/archives/list/chimerax-users@cgl.ucsf.edu/thread/ZLFBNB32ANX7SGRB2EKJH6DKBVLMM4X5/), [Matsci forum](https://matsci.org/t/how-to-further-reduce-the-resolution-of-glb-format/54013)) (snippets).
- Counter-evidence: Molecular Nodes is free, active, and claims studio adoption ([Blender Extensions](https://extensions.blender.org/add-ons/molecularnodes/versions/), [Lorne 2024](https://proteins-2024.p.asnevents.com.au/days/2024-02-05/abstract/101827)). U of T's BMC programme teaches Blender and Houdini for molecular structures ([U of T BMC](https://bmc.med.utoronto.ca/news-events/category/BMC75)). Big studios cite 3ds Max, Redshift and Houdini, not Maya ([Unity / Random42](https://unity.com/en/resources/random42)). All snippets.

**Who pays.** Maya-based technical directors and lead animators at medical-animation studios. Freelance medical animators who already know Maya. University BMC programmes that teach Maya.

**Rough price points.** Evidence thin. I found no current price for mMaya, AdonisFX or Bio-Art Blender in the snippets. Inference (confidence: low): a per-seat subscription of about USD 100–500 per year, held down by the free Molecular Nodes. Not sourced.

**Competitors / substitutes.**
- Molecular Nodes (Blender, free).
- Bio-Art Blender add-on, which makes membranes and viruses from PDB data with geometry nodes ([Superhive](https://superhivemarket.com/products/bio-art)).
- Houdini Muscles & Tissue and Vellum ([SideFX docs](https://www.sidefx.com/docs/houdini/muscles/index.html)).
- AdonisFX.
- cellPACK and Mesoscope ([Scripps CCSB](https://ccsb.scripps.edu/cellpack/)).
- ChimeraX export.

All snippets.

**Founder fit.** Direct: a Maya TD who builds PySide tools and custom deformers. He would need a structural-biology adviser.

**Confidence.** Low. The tool gap is real, but the number of buyers who stay in Maya is unknown, and the field may be moving to Blender and Houdini.

### Gap 3. A scientific provenance and review tracker for biomedical shots (AI-assisted claim-to-source checks)

**Problem.** Every asset and shot needs scientific sign-off. Review runs over several rounds of script, storyboard and MLR. Version confusion eats weeks. Generative AI raises the risk of plausible but wrong visuals. No tool I found links each asset or shot to its sources (PDB IDs, papers, scale data) and its reviewer sign-offs in one place.

**Evidence**
- Two script rounds and two storyboard rounds come before formal MLR ([AXS](https://axs3d.com/locations/)). Teams plan four to eight weeks for MLR, much of it lost to version confusion ([Informa](https://www.informait.com/blog/the-mlr-delay-nobody-budgets-for)) (snippets).
- Medical animation takes 8–20 weeks, against 4–12 for commercial animation ([Programming Insider](https://programminginsider.com/accuracy-is-the-product-what-makes-medical-animation-different/)) (snippet; the vendor behind the figure is unclear).
- A Frontiers reviewer said checking the AI images was not his job, and the paper was retracted three days after publication ([Vice](https://www.vice.com/en/article/scientific-journal-frontiers-publishes-ai-generated-rat-with-gigantic-penis-in-worrying-incident), [Gizmodo](https://gizmodo.com/science-journal-rat-dck-ai-generated-images-retracted-1851297606)) (snippets).
- VOKA says expert review is still required even with AI in the pipeline ([VOKA](https://voka.io/?p=15477)) (snippet).
- One studio keeps "protein cards" as an internal reference library. This is a hand-made version of provenance tracking ([blog](https://reindeer-haddock-glja.squarespace.com/blog/from-pdb-to-production-how-to-prep-protein-structures-for-3d-animation)) (snippet).

**Who pays.** Producers and scientific directors at medical-animation studios. Medical-review leads at healthcare agencies. Possibly pharma medical-affairs teams.

**Rough price points.** Evidence thin. I found no pricing. Inference (confidence: low): a SaaS at USD 50–200 per seat per month for studios. Agency and pharma tiers would be custom-quoted.

**Competitors / substitutes.** Generic review tools and spreadsheets. Enterprise MLR platforms. Inference (confidence: medium): Veeva-style MLR systems dominate on the pharma side; I did not verify this in this track. In-house "reference card" habits.

**Founder fit.** Partial. It uses his RAG and Claude-tool skills, but not his sculpting and rigging strengths, and it sells to producers rather than artists.

**Confidence.** Low.

## Load-bearing claims

1. Clarafi's mMaya page states compatibility "OSX & Windows: Maya 2018-2020, Linux: Maya 2020". It states Maya 2022 is not yet supported because of Python 3 integration. https://clarafi.com/tools/mmaya/ (snippet only; page date unknown).
2. Maya 2023 and later support Python 3 only. Maya 2024.1 bundles Python 3.10.8. https://www.riggingdojo.com/2022/03/31/autodesk-2023/ and https://help.autodesk.com/view/MAYAUL/2024/ENU/?guid=Maya_SDK_Open_Source_Components_2024_1_Open_Source_Components_html (snippet only; the search summary did not cleanly attribute the "Python 3 exclusively" wording to one page).
3. Unity stopped selling and supporting Ziva VFX, Ziva Real-Time and Ziva Face Trainer, effective 2 April 2024. Active subscribers could convert to a five-year term. DNEG received an exclusive perpetual licence to the Ziva IP. https://www.cgchannel.com/2024/04/unity-discontinues-the-ziva-products/ and https://3dvf.com/unity-met-fin-a-la-vente-et-au-support-de-ziva-dneg-en-acquiert-les-droits/ (snippet only).
4. A CG Channel article of 4 March 2026 says Unity's decision "left Maya artists without a simple off-the-shelf solution" for soft tissue. It asks whether AdonisFX 2.0 is that solution. https://www.cgchannel.com/2026/03/is-adonisfx-2-0-the-new-ziva-vfx/ (snippet only).
5. Molecular Nodes 4.5.12 is dated 17 March 2026 on Blender Extensions and requires Blender 5.1 or later. https://extensions.blender.org/add-ons/molecularnodes/versions/ (snippet only).
6. The CGTrader listing "Realistic Human Heart - Rigged and Animated" is priced at $299, under a royalty-free licence that excludes AI use. https://www.cgtrader.com/3d-models/science/medical/human-heart-rigged-and-animated (snippet only).
7. The TurboSquid listing "Heart Animation - Human Heart Beating" is $20. It is a stylised Blender heart, rigged and animated, under an editorial-uses-only licence. https://www.turbosquid.com/3d-models/heart-animation-human-heart-beating-2444833 (snippet only).
8. A buyer review on the CGTrader "Lungs animated" listing ($29) says the animation only works in 3ds Max. https://www.cgtrader.com/3d-models/character/anatomy/lungs-animated (snippet only; a second URL, /character/human-anatomy/lungs-animated, also appeared, and I could not confirm which carries the review).
9. A cached TurboSquid search for "virus" showed price-filter counts of $300+ (35), $200–300 (24), $100–200 (186) and $1–100 (3,346). That sums to about 3,591. https://www.turbosquid.com/ko/Search/3D-Models/virus (snippet only; cache date unknown; the sum is mine).
10. VOKA states a catalogue of more than 1,000 ready-made models and reuses existing assets in pre-production to cut costs. https://voka.io/3d-scientific-animation-services/molecular-biology/ (snippet only).
11. AXS Studio: scripts typically get two review rounds, then two storyboard rounds, then formal MLR review. Clients should contact it at least four months before the deadline. https://axs3d.com/locations/ (snippet only).
12. An MLR vendor says pharma teams typically plan four to eight weeks for MLR review. https://www.informait.com/blog/the-mlr-delay-nobody-budgets-for (snippet only).
13. VOKA's cost guide: freelance medical animation $1.5k–$4k per minute; professional studios $5k–$20k per minute. https://voka.io/medical-animation-cost/ (snippet only; year not shown).
14. The 2026 AOI survey: 46% of 549 illustrators lost work to generative AI, up from 32%. 31% say clients expect lower fees. https://www.resultsense.com/news/2026-11-04-aoi-illustrators-generative-ai-survey-2026/ (snippet only; dated 4 November 2026).
15. Frontiers in Cell and Developmental Biology retracted a paper with Midjourney-generated figures on 16 February 2024, three days after publication. https://gizmodo.com/science-journal-rat-dck-ai-generated-images-retracted-1851297606 (snippet only).

## Where sources disagree

- **Ziva discontinuation date.** Unity's notice and CG Channel give 2 April 2024 ([CG Channel](https://www.cgchannel.com/2024/04/unity-discontinues-the-ziva-products/)). Super Renders Farm says January 2024 ([Super Renders Farm](https://www.superrendersfarm.com/article/ziva-vfx-vs-houdini-simulation)). I treat April as correct.
- **Newest Maya supported by Molecular Maya.** Clarafi's page says 2018–2020 ([Clarafi](https://clarafi.com/tools/mmaya/)). An Autodesk forum user says "up to 2019" ([Autodesk](https://forums.autodesk.com/t5/maya-forum/molecular-maya/td-p/9256999)). A 2019 blog says 2015–2018 ([Redworks](http://www.redworks.co.nz/2019/05/magic-of-molecular-maya.html)). All are older than 2024. Current status is unconfirmed.
- **Price per minute.**
  - VOKA: studios $5k–$20k per minute ([VOKA](https://voka.io/medical-animation-cost/)).
  - Another guide: MoA $25k–$75k for 2–3 minutes. A further guide: $1k–$60k per minute, mid-market $8k–$25k (both from [Prolific](https://prolificstudio.co/?p=30191) or related search results; attribution unclear).
  - Knowlify: $5k–$50k+ per minute ([Knowlify](https://knowlify.com/articles/best-medical-healthcare-animation-agencies)).
  - All of these are vendor-published.
- **Salaries.**
  - AMI-attributed medians via secondary sites: about $83.5k–$89.8k ([content-farm summary](https://ratings.koha-community.org/en/salary-for-medical-illustrator.html)).
  - Payscale: about $71k ([Payscale](https://www.payscale.com/research/US/Job=Medical_Illustrator/Salary)).
  - Salary.com: $61,562 as of April 2025 ([Salary.com](https://salary.com/research/salary/posting/medical-illustrator-salary)).
  - I did not see the primary AMI survey.
- **AI job loss.**
  - AOI: 32% rising to 46% ([Resultsense](https://www.resultsense.com/news/2026-11-04-aoi-illustrators-generative-ai-survey-2026/)).
  - Society of Authors 2024: 26% of illustrators ([80.lv](https://80.lv/articles/a-third-of-translators-a-quarter-of-illustrators-have-lost-their-jobs-to-ai)).
  - A Society of Authors 2025 figure of 6% "lost opportunities" across authors and illustrators. These ask different questions of different samples.
  - None is specific to medical illustrators.
- **Project timelines.** "12–16 weeks for a two-minute animation" versus "8–20 weeks". These cover different scopes ([AXS](https://axs3d.com/locations/), [Programming Insider](https://programminginsider.com/accuracy-is-the-product-what-makes-medical-animation-different/)).
- **Interactive engine of choice.** Random42 made a COVID film in Unreal ([Epic](https://www.unrealengine.com/spotlights/getting-under-the-microscope-with-random42-s-amazing-medical-animations), likely pre-2024). Its November 2025 case study describes interactive MoA and MoD work in Unity ([Unity](https://unity.com/en/resources/random42)).
- **Molecular Nodes adoption.** The developers report studio adoption ([Lorne 2024](https://proteins-2024.p.asnevents.com.au/days/2024-02-05/abstract/101827)). I found no independent confirmation.
- **AMI location.** It was incorporated in Illinois; another snippet places it in Lexington, Kentucky ([AMI](https://ami.org/)). Minor.

## What I could not find

- **Opened pages.** WebFetch failed with a DNS error on every host tried, so no page was opened. The shared search budget ran out after about 39 searches. Every claim here needs a fetch to confirm.
- **mMaya.** Its current price, or any Clarafi release after 2022.
- **ePMV.** Its last commit date.
- **Conference programmes.** Full AMI session lists for 2024–2026 (talk titles), and the IMI 2025 programme.
- **Practitioner forums.** Reddit threads from r/medicalillustration, r/Maya or r/vfx. No Reddit results came back. Blender Artists threads by medical animators.
- **Fab and Sketchfab.** Prices, and counts of rigged biological assets.
- **Professional bodies.** Any organisation called "ASMI".
- **Accuracy review.** Fees for subject-matter-expert consultants. Documented accuracy errors in pharma animations, as opposed to journal figures.
- **Contracts.** An actual "No AI" clause in a medical-animation contract.
- **Job market.** Data for BMC, JHU, UIC, Augusta, Dundee or Glasgow graduates in 2025–2026. Studio layoffs. Offshoring.
- **Costs and prices.** Render costs. Zygote licence prices. BioDigital export terms.
- **Rig tools.** Peristalsis or cilia rig products and tutorials. Sales counts for Superhive biology add-ons.
- **Theses.** Any medical-visualisation thesis on tool pain.

## Sources

All items were seen as search-result snippets only (not opened). "Date n/s" means no date was shown in the snippet.

1. mMaya, Clarafi, date n/s (content covers Maya 2018–2022) [pre-2024, possibly stale] — https://clarafi.com/tools/mmaya/
2. Maya 2022 version (forum), Clarafi, about 2021–22 [pre-2024, possibly stale] — https://clarafi.com/topic/maya-2022-version/
3. Solved: Molecular Maya, Autodesk Community, about 2020 [pre-2024, possibly stale] — https://forums.autodesk.com/t5/maya-forum/molecular-maya/td-p/9256999
4. Magic of Molecular Maya, Redworks, May 2019 [pre-2024, possibly stale] — http://www.redworks.co.nz/2019/05/magic-of-molecular-maya.html
5. Autodesk 2023, Rigging Dojo, 31 Mar 2022 [pre-2024, possibly stale] — https://www.riggingdojo.com/2022/03/31/autodesk-2023/
6. Maya 2024.1 Open Source Components, Autodesk, 2023 [pre-2024, possibly stale] — https://help.autodesk.com/view/MAYAUL/2024/ENU/?guid=Maya_SDK_Open_Source_Components_2024_1_Open_Source_Components_html
7. Maya 2026.3 Update Release Notes, Autodesk, 2026 — https://help.autodesk.com/cloudhelp/2026/ENU/Maya-ReleaseNotes/files/MAYA_RELEASENOTES_2026_3_RELEASE_NOTES_HTML.html
8. Maya 2025.2 adds a new ML deformer, CG Channel, 31 Jul 2024 — https://www.cgchannel.com/2024/07/maya-2025-2-adds-a-new-ml-deformer/
9. Welcome to ePMV, Scripps, date n/s — https://epmv.scripps.edu/
10. corredD/ePMV, GitHub, date n/s — https://github.com/corredD/ePMV
11. ePMV paper, Structure (PMC), 2011 [pre-2024, possibly stale] — https://pmc.ncbi.nlm.nih.gov/articles/PMC3101797
12. Molecular Nodes versions, Blender Extensions, Mar 2026 — https://extensions.blender.org/add-ons/molecularnodes/versions/
13. NumFOCUS Small Development Grant: MolecularNodes, MDAnalysis, 12 Dec 2024 — https://www.mdanalysis.org/2024/12/12/sdg_molecularnodes/
14. Poster, 49th Lorne Conference on Protein Structure and Function, Feb 2024 — https://proteins-2024.p.asnevents.com.au/days/2024-02-05/abstract/101827
15. Bio-Art Blender, Superhive, date n/s (lists Blender 2.93) — https://superhivemarket.com/products/bio-art
16. Bio-Art Blender, Blender Market, date n/s — https://blendermarket.com/products/bio-art
17. Biological Research 3D-Assets Pack, Superhive, about 2025–26 (Blender 5.0) — https://superhivemarket.com/products/biological-research-3dassets-pack
18. How to reduce subdivision of the mesh?, ChimeraX users mailing list (UCSF), date n/s — https://mail.cgl.ucsf.edu/mailman/archives/list/chimerax-users@cgl.ucsf.edu/thread/ZLFBNB32ANX7SGRB2EKJH6DKBVLMM4X5/
19. How to further reduce the resolution of glb format?, Matsci forum, date n/s — https://matsci.org/t/how-to-further-reduce-the-resolution-of-glb-format/54013
20. CellPACK, Scripps CCSB, date n/s — https://ccsb.scripps.edu/cellpack/
21. Mesoscale projects, Scripps CCSB, date n/s — https://ccsb.scripps.edu/projects/mesoscale
22. Mesoscale Explorer (PMID 39282403), NLK mirror, 2024 — https://dev.nlk.cz/mdv/doc/pmid39282403
23. Talks and posters, Allen Institute for Cell Science, 2024 — https://allencell.org/talks-posters.html
24. Unity discontinues the Ziva products, CG Channel, 3 Apr 2024 — https://www.cgchannel.com/2024/04/unity-discontinues-the-ziva-products/
25. An update about Ziva, Unity, 2024 — https://unity.com/vn/blog/news/update-about-ziva
26. Ziva products discontinued, Unity Discussions, 2024 — https://discussions.unity.com/t/ziva-products-discontinued-no-longer-part-of-unity/943600
27. Unity met fin à la vente et au support de Ziva, DNEG en acquiert les droits, 3DVF, 2024 — https://3dvf.com/unity-met-fin-a-la-vente-et-au-support-de-ziva-dneg-en-acquiert-les-droits/
28. Ziva VFX vs Houdini simulation, Super Renders Farm, date n/s — https://www.superrendersfarm.com/article/ziva-vfx-vs-houdini-simulation
29. Is AdonisFX 2.0 the new Ziva VFX?, CG Channel, 4 Mar 2026 — https://www.cgchannel.com/2026/03/is-adonisfx-2-0-the-new-ziva-vfx/
30. Artist shows Ziva VFX-inspired muscle simulation plug-in, 80.lv, date n/s — https://80.lv/articles/artist-shows-ziva-vfx-inspired-muscle-simulation-plug-in-for-3ds-max-maya
31. Vellum beating heart, SideFX forum, date n/s — https://www.sidefx.com/forum/topic/82147/
32. Vellum object with different needs, SideFX forum, date n/s — https://sidefx.com/forum/topic/96072
33. Muscles & Tissue, SideFX Houdini docs, date n/s — https://www.sidefx.com/docs/houdini/muscles/index.html
34. Houdini-made rib cage rig for breathing animation, 80.lv, date n/s — https://cdn.80.lv/articles/this-houdini-made-rib-cage-rig-allows-creating-lifelike-breathing-animations
35. Lightweight Self-Driven Deformable Organ Animations, arXiv 2401.11614, Jan 2024 — https://www.arxiv.org/abs/2401.11614
36. Rolling or coiling rig in Maya, Lester Banks, Feb 2020 [pre-2024, possibly stale] — https://lesterbanks.com/2020/02/how-to-create-a-rolling-or-coiling-rig-in-maya/
37. Flagella animation project, XVIVO, date n/s — https://xvivo.com/?p=2342
38. Hybrid's Fantastic Voyage into a Tumor Microenvironment, Stash, date n/s — https://www.stashmedia.tv/?p=100441
39. Getting under the microscope with Random42, Epic Games, date n/s (likely 2020–21) [pre-2024, possibly stale] — https://www.unrealengine.com/spotlights/getting-under-the-microscope-with-random42-s-amazing-medical-animations
40. How Random42 is revolutionizing medical visualization with Unity, Unity, Nov 2025 — https://unity.com/en/resources/random42
41. VOKA article on AI and real-time in medical animation, VOKA, 2026 — https://voka.io/?p=15477
42. 3D scientific animation: molecular biology, VOKA, date n/s — https://voka.io/3d-scientific-animation-services/molecular-biology/
43. Medical animation cost, VOKA, date n/s — https://voka.io/medical-animation-cost/
44. Medical Animation & Scientific Visualisation, Mainframe, date n/s — https://mainframeuk.squarespace.com/medical-animation
45. From PDB to Production, studio blog (Squarespace), date n/s — https://reindeer-haddock-glja.squarespace.com/blog/from-pdb-to-production-how-to-prep-protein-structures-for-3d-animation
46. Recent innovations in 3D animation technology for pharma, AXS Studio, date n/s — https://axs3d.com/recent-innovations-in-3d-animation-technology-for-pharma/
47. Global Medical Animation Services, AXS Studio, date n/s — https://axs3d.com/locations/
48. Heart Animation - Human Heart Beating, TurboSquid, date n/s — https://www.turbosquid.com/3d-models/heart-animation-human-heart-beating-2444833
49. Realistic Human Heart - Rigged and Animated, CGTrader, date n/s — https://www.cgtrader.com/3d-models/science/medical/human-heart-rigged-and-animated
50. Realistic 3D Animated Human Heart, CGTrader, date n/s — https://www.cgtrader.com/3d-models/science/medical/realistic-3d-animated-human-heart
51. Human Heart Beat Animated for Blender, CGTrader, date n/s — https://www.cgtrader.com/3d-models/character/human-anatomy/human-heart-beat-animated-for-blender
52. Animated heart inside RibCage, CGTrader, date n/s — https://www.cgtrader.com/3d-models/science/medical/animated-heart-inside-ribcage
53. Cross Section Human Lungs, CGTrader, date n/s — https://cgtrader.com/3d-models/science/medical/cross-section-human-lungs
54. Lungs animated, CGTrader, date n/s — https://www.cgtrader.com/3d-models/character/anatomy/lungs-animated
55. Human anatomy animated (skeleton and internal organs), CGTrader, date n/s — https://cgtrader.com/3d-models/character/anatomy/human-anatomy-nimated-skeleton-and-internal-organs
56. Lungs Model 1, CGTrader, date n/s — https://cgtrader.com/3d-models/various/various-models/lungs-model-1
57. Human Lungs - pulmonary system, CGTrader, date n/s — https://cgtrader.com/3d-models/science/medical/human-lungs-pulmonary-system-3d-model
58. Medical microscopic infographics pack, CGTrader, date n/s — https://www.cgtrader.com/3d-models/science/medical/medical-microscopic-infographics-pack-cells-viruses-and-dna
59. Ultimate 3D Human Organs Pack, CGTrader, date n/s — https://www.cgtrader.com/3d-models/character/anatomy/ultimate-3d-human-organs-pack
60. DNA Virus Blood Cell Bacteria microbiology model, CGTrader, date n/s — https://cgtrader.com/3d-models/science/medical/dna-virus-blood-cell-bacteria-round-cell-microbiology-model
61. Viruses props pack, Ithappy Studios, date n/s — https://ithappystudios.com/props/viruses
62. Ultimate microscopic anatomy listing, Fab, date n/s — https://www.fab.com/listings/117cf6a5-1763-4f9c-b12b-efb41e9a2d37
63. Search: virus, TurboSquid (Korean cache), date n/s — https://www.turbosquid.com/ko/Search/3D-Models/virus
64. NIH 3D entry 3DPX-017981 (E. coli), NIH, date n/s — https://3d.nih.gov/entries/3DPX-017981
65. NIH 3D entry 17980 (E. coli), NIH, date n/s — https://3d.nih.gov/entries/17980
66. Escherichia coli bacterium, CGTrader, date n/s — https://www.cgtrader.com/3d-models/science/medical/escherichia-coli-e-coli-bacterium
67. Microscopic Life Collection 01, CGTrader, date n/s — https://www.cgtrader.com/3d-model-packs/microscopic-life-collection-01
68. Medical - Bacteria, DOSCH Design, date n/s — https://doschdesign.com/products/3d/Medical_Bacteria.html
69. NIH 3D FAQs, NIH, date n/s — https://3d.nih.gov/faqs
70. Free NIH BioART 2D and NIH 3D, UW–Madison Biochemistry, 21 Nov 2024 — https://bcrf.biochem.wisc.edu/2024/11/21/free-nih-bioart-2d-and-nih-3d/
71. SARS-CoV-2 3D model, Visual Science, 2020 [pre-2024, possibly stale] — https://www.visual-science.com/projects/sars-cov-2/3d-model
72. How SciePro created the most anatomically accurate model, TurboSquid blog, 3 Apr 2023 [pre-2024, possibly stale] — https://blog.turbosquid.com/2023/04/03/how-sciepro-created-the-most-anatomically-accurate-model-on-the-market/
73. Zygote Body pricing, Zygote, date n/s — https://www.zygotebody.com/pricing
74. Best medical healthcare animation agencies, Knowlify, date n/s — https://knowlify.com/articles/best-medical-healthcare-animation-agencies
75. Creating animations with your BioRender illustrations, BioRender Help, 2026 — https://help.biorender.com/hc/en-gb/articles/17605508265629-Creating-animations-with-your-BioRender-illustrations
76. BioRender Features, BioRender, date n/s — https://www.biorender.com/features
77. Best BioRender alternatives for 3D science animation (2026), Animiotics, 2026 — https://animiotics.com/blog/best-biorender-alternatives-for-3d-science-animation-2026/
78. Medical Animation Cost Guide, Prolific Studio, date n/s — https://prolificstudio.co/?p=30191
79. Hire medical animation freelancers (Pakistan), Upwork, date n/s — https://www.upwork.com/hire/medical-animation-freelancers/pk/
80. Medical Illustrator Salary in 2026, Payscale, 2026 — https://www.payscale.com/research/US/Job=Medical_Illustrator/Salary
81. Medical illustrator salary, Salary.com, Apr 2025 — https://salary.com/research/salary/posting/medical-illustrator-salary
82. A Deep Dive into the Salary for a Medical Illustrator in 2024, content-farm site (weak), 2024 — https://ratings.koha-community.org/en/salary-for-medical-illustrator.html
83. 46% of illustrators surveyed say they have lost work to AI, Resultsense, 4 Nov 2026 — https://www.resultsense.com/news/2026-11-04-aoi-illustrators-generative-ai-survey-2026/
84. A third of translators and a quarter of illustrators lost jobs to AI, 80.lv, 2024 — https://80.lv/articles/a-third-of-translators-a-quarter-of-illustrators-have-lost-their-jobs-to-ai
85. Association of Medical Illustrators 2025 Annual Conference, TVASurg (U of T), 2025 — https://pie.med.utoronto.ca/TVASurg/association-of-medical-illustrators-2025-annual-conference/
86. AMI 2026 proposal information, AMI via SurveyMonkey, 2025–26 — https://www.surveymonkey.com/r/ami2026proposals
87. AMI home page, Association of Medical Illustrators, 2026 — https://ami.org/
88. IMI Conference 2026, Institute of Medical Illustrators, 2026 — https://www.imi.org.uk/conference2026/
89. About, Medical Artists' Association of Great Britain, 2025–26 — https://maa.org.uk/about/
90. BMC75 News & Events, U of T MScBMC, date n/s — https://bmc.med.utoronto.ca/news-events/category/BMC75
91. Accuracy is the product: what makes medical animation different, Programming Insider, date n/s — https://programminginsider.com/accuracy-is-the-product-what-makes-medical-animation-different/
92. The MLR delay nobody budgets for, Informa (informait), 2025–26 — https://www.informait.com/blog/the-mlr-delay-nobody-budgets-for
93. MLR review agency guide, Informa (informait), 2025–26 — https://www.informait.com/guides/mlr-review-agency-guide
94. Science journal retracts AI-generated rat images, Gizmodo, Feb 2024 — https://gizmodo.com/science-journal-rat-dck-ai-generated-images-retracted-1851297606
95. Frontiers publishes AI-generated rat, Vice, Feb 2024 — https://www.vice.com/en/article/scientific-journal-frontiers-publishes-ai-generated-rat-with-gigantic-penis-in-worrying-incident
96. The end of "No AI" clauses in clinical research agreements, The Contract Network, Jan 2025 — https://thecontractnetwork.com/the-end-of-no-ai-clauses-in-clinical-research-agreements/
97. Webinar on "No AI" clauses in CDAs, Florence Healthcare, date n/s — https://www.florencehc.com/?p=16686
98. ITSme Society illustration agencies introduce AI clause, The Bookseller, date n/s — https://thebookseller.com/news/itsme-society-illustration-agencies-introduce-protection-against-ai-clause-in-contracts
99. CellWalk, Apple App Store, date n/s — https://apps.apple.com/app/cellwalk/id1627776848
100. Learn Viruses, Apple App Store, date n/s — https://apps.apple.com/ky/app/learn-viruses/id1603794565
101. VR startup offers microscopic learning environment (MedMicroMaps), XR Today, Feb 2025 — https://www.xrtoday.com/?p=57106

## Independent fact-check

18 checked: 0 verified, 0 partial, 18 unverified, 0 contradicted, 0 fabricated-url.

Method note (7 November 2026). This check could not reach any source. WebFetch failed with DNS resolution errors on every host tried: clarafi.com, www.cgchannel.com (two URLs), extensions.blender.org, www.cgtrader.com and www.turbosquid.com. The sandbox gave the same error the original author hit, and its message said to stop trying further hosts. WebSearch returned "budget used up" (the shared 200-call limit for this turn) on all four corroborating queries. So no claim below could be confirmed or refuted from a source, and every row is UNVERIFIED. The notes record internal-consistency checks and the checker's prior knowledge (training data to about mid-2026). They are flags, not verification. To run a real check, allow these domains in the session's network settings and re-run with a fresh search budget.

| # | Claim (short) | Status | Note / corrected value | Source checked (URL) |
|---|---|---|---|---|
| 1 | mMaya supports Maya 2018-2020 only; 2022 "not yet supported" (Python 3) | UNVERIFIED | Fetch failed (DNS). The page is undated, so "has not run on any Maya release of the last four years" is an inference, not a fact. A later release may exist that the snippets missed. | https://clarafi.com/tools/mmaya/ |
| 2 | Maya 2023+ is Python 3 only; Maya 2024.1 bundles Python 3.10.8 | UNVERIFIED | Not fetched. This matches the checker's prior knowledge: Maya 2022 made Python 3 the default, 2023 removed Python 2, and the 2024 line ships Python 3.10.x. Low risk. | https://www.riggingdojo.com/2022/03/31/autodesk-2023/ ; Autodesk help URL (not attempted after DNS failures) |
| 3 | Ziva VFX, RT and Face Trainer discontinued 2 Apr 2024; 5-year term; DNEG perpetual licence | UNVERIFIED | Fetch failed (DNS). Matches prior knowledge of Unity's March 2024 notice. Low risk. | https://www.cgchannel.com/2024/04/unity-discontinues-the-ziva-products/ |
| 4 | CG Channel, 4 Mar 2026: Unity "left Maya artists without a simple off-the-shelf solution"; asks whether AdonisFX 2.0 fills it | UNVERIFIED | Fetch failed (DNS). The quote could not be checked. Note that AdonisFX itself is a commercial Maya soft-tissue plugin that has existed since before 2024. So "Maya users have nothing maintained" (Gap 2) overstates the case for characters, though the organ- and cell-specific angle may still hold. | https://www.cgchannel.com/2026/03/is-adonisfx-2-0-the-new-ziva-vfx/ |
| 5 | Molecular Nodes 4.5.12, 17 Mar 2026, Blender 5.1 | UNVERIFIED | Fetch failed (DNS). The report is inconsistent with itself: the Summary says it "supports Blender 5.1", while load-bearing claim 5 says it "requires Blender 5.1 or later". These are not the same claim. | https://extensions.blender.org/add-ons/molecularnodes/versions/ |
| 6 | CGTrader rigged and animated heart, $299, licence excludes AI use | UNVERIFIED | Fetch failed (DNS). Marketplace prices and licence terms change often. Treat them as a point-in-time snapshot. | https://www.cgtrader.com/3d-models/science/medical/human-heart-rigged-and-animated |
| 7 | TurboSquid heart, $20, Blender, editorial-only | UNVERIFIED | Fetch failed (DNS). | https://www.turbosquid.com/3d-models/heart-animation-human-heart-beating-2444833 |
| 8 | CGTrader "Lungs animated" $29; a buyer review says the animation is 3ds-Max-only | UNVERIFIED | Not fetched (host blocked). The author already flagged that two URLs exist and that the review was not tied to either one. | https://www.cgtrader.com/3d-models/character/anatomy/lungs-animated |
| 9 | TurboSquid "virus" search: about 3,591 results | UNVERIFIED | Not fetched (host blocked). The arithmetic is correct: 35 + 24 + 186 + 3,346 = 3,591. The cache date is unknown, and this is a Korean-locale search page. | https://www.turbosquid.com/ko/Search/3D-Models/virus |
| 10 | VOKA: more than 1,000 ready-made models; reuses assets | UNVERIFIED | Not fetched (no access, search budget out). This is vendor marketing copy. | https://voka.io/3d-scientific-animation-services/molecular-biology/ |
| 11 | AXS: 2 script rounds, then 2 storyboard rounds, then MLR; book 4 months ahead | UNVERIFIED | Not fetched. Vendor page. | https://axs3d.com/locations/ |
| 12 | MLR takes 4 to 8 weeks; time lost to version confusion | UNVERIFIED | Not fetched. The source is an MLR vendor with a commercial interest in describing the delay. | https://www.informait.com/blog/the-mlr-delay-nobody-budgets-for |
| 13 | VOKA cost guide: freelance $1.5k to $4k per minute; studio $5k to $20k per minute | UNVERIFIED | Not fetched, and the page is undated. Other vendor guides cited in the report give $1k to $60k and $5k to $50k+, so this figure is a single-vendor number, not an industry rate. | https://voka.io/medical-animation-cost/ |
| 14 | AOI 2026: 46% of 549 lost work to AI (up from 32%); 31% say clients expect lower fees | UNVERIFIED | Not fetched. The article is dated 4 Nov 2026, after the checker's knowledge cutoff, so the checker cannot assess it from memory. It is a secondary news write-up. The primary AOI report was not seen. It covers general illustrators. | https://www.resultsense.com/news/2026-11-04-aoi-illustrators-generative-ai-survey-2026/ |
| 15 | Frontiers retracted the Midjourney-figure paper on 16 Feb 2024, 3 days after publication | UNVERIFIED | Not fetched. Matches prior knowledge: published about 13 Feb 2024, retracted about 16 Feb 2024. Low risk. It is a pre-2025 journal-figure case, not a commercial medical-animation case. | https://gizmodo.com/science-journal-rat-dck-ai-generated-images-retracted-1851297606 |
| 16 | Gap 1 heart prices $15 / $139 / $275 / $299 (CGTrader) and $20 (TurboSquid) | UNVERIFIED | No listing could be opened. The prices are from search snippets of unknown date. | CGTrader and TurboSquid listing URLs in Gap 1 (host blocked) |
| 17 | Gap 1 lung and thorax prices: $69.99, $29, about $499; range "animated lungs $5-$69.99" | UNVERIFIED | No listing opened. The $5 lower bound in "Rough price points" matches no lung listing in the Gap 1 evidence ($29, $69.99). It may come from "Lungs Model 1" (source 56), which is not shown to be animated. Treat $5 as unsupported. | https://www.cgtrader.com/3d-models/character/anatomy/lungs-animated ; https://cgtrader.com/3d-models/science/medical/cross-section-human-lungs (host blocked) |
| 18 | "Maya 2026.3 is current" (Gap 2) | UNVERIFIED | Not fetched. Possibly outdated: Autodesk usually ships the next annual Maya release in spring, so by November 2026 a Maya 2027 release is likely. Rephrase as "at least through Maya 2026.3". This does not change the argument: the mMaya gap would only be wider. | https://help.autodesk.com/cloudhelp/2026/ENU/Maya-ReleaseNotes/files/MAYA_RELEASENOTES_2026_3_RELEASE_NOTES_HTML.html (not attempted after DNS failures) |

Other flags (not counted above):
- **Inference presented as fact.** Gap 2's Problem statement says Maya users "lost their native molecular toolkit" and "have nothing maintained". The Summary rightly calls this a medium-confidence inference, but Gap 2 states it flatly. It rests on an undated Clarafi page and on finding no later release. AdonisFX (a maintained Maya soft-tissue plugin) partly contradicts the soft-tissue half.
- **Pre-2024 facts used as current.** The mMaya compatibility evidence (claims 1 and 2, and the Clarafi forum and Autodesk forum posts) is all pre-2024. The author tagged it, but Gap 2 depends on it.
- **Vendor-sourced numbers.** Every price-per-minute, timeline and MLR-duration figure comes from vendor marketing (VOKA, AXS, Informa, Programming Insider). None is independent.
- **Hypothesis H2.** "Partly supported" is generous. The supporting evidence is one 2024 journal retraction, one vendor blog, and a source that argues "No AI" clauses are *ending*. The author's own counter-evidence column finds no capacity shortage. "Insufficient evidence" would fit better.

### Implications

- **Overall.** This check adds no independent confirmation. The report's evidence is still 100% search snippets, now with a second failed attempt to open them. No verdict is strengthened. Confidence ratings should be read as at most what the author gave, and lower where the gap rests on one undated page.
- **Gap 1 (living-anatomy rig kits)** is moderately weakened, not refuted. Its core observation is qualitative: marketplace organ rigs are baked, locked to one program, licensed inconsistently, and unsourced. It rests on about 8 listing snippets that nobody has opened. Prices and licence terms are volatile, and the $5 lung lower bound is unsupported. The demand side (who buys, how many) is unmeasured. Keep it at medium confidence only once someone opens the listings. Until then, low to medium.
- **Gap 2 (Maya bio-toolkit)** is weakened the most. Both pillars are unverified: mMaya being abandoned rests on an undated, pre-2024 compatibility page, and the Ziva loss is plausible (it matches prior knowledge). AdonisFX already gives Maya users a maintained soft-tissue solver, and Molecular Nodes plus the drift to Blender and Houdini shrink the buyer pool. The author's "Low" confidence is right. Downgrade further unless a 2025 or 2026 Clarafi status is confirmed.
- **Gap 3 (provenance and review tracker)** is slightly weakened. Its pain evidence (MLR weeks, review rounds) comes from vendors with a commercial interest. The Frontiers case is a 2024 journal incident, not a pharma-animation failure. Low confidence stands.
- **Hypotheses.** H1 "partly supported" stands, but only on unverified snippets. H2 should be downgraded to "insufficient evidence". H3 "insufficient evidence" and H4 "partly supported (supply only)" stand unchanged.
- **Most valuable next fetches.** In order: clarafi.com/tools/mmaya (Gap 2 depends on it), the CG Channel 2026 AdonisFX article, the CGTrader and TurboSquid heart listings, and the Molecular Nodes versions page.
