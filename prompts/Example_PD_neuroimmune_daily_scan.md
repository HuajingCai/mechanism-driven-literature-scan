Generate a daily Parkinson's disease neuroimmunology and mechanism-inspiration paper scan for rapid filtering, then send it to the configured email address. Default recipient: configured recipient.

Search scope and intent:
Search papers/preprints published or posted in the past 24 hours from PubMed, Nature Press/Springer Nature, Science Press/AAAS, Cell Press, bioRxiv, and medRxiv. Prioritize breadth during screening, but the final report must be selective, mechanistic, and useful for rapid filtering. Avoid hallucination by using verifiable sources only.

Primary output requirement:
- Save the report as a Word document (.docx) in the workspace.
- Email the .docx report to configured recipient.
- Do not send a Markdown file as the email attachment.
- If .docx creation is unavailable, save the best local fallback and notify the user; do not pretend that a Word report was sent.

Quantity rule:
- Screen all candidates from the search window, de-duplicate across databases/sources, and exclude clearly irrelevant/noisy hits.
- The final report must include no more than 50 papers total.
- If more than 50 relevant papers are found, retain the top 50 by priority: direct PD/synucleinopathy relevance first, then strongest neuroimmune mechanisms, then the most transferable tumor/infection/barrier/systems immunology ideas.
- Do not pad to 50; include fewer when fewer are truly useful.
- Keep each entry short and make the document easy to skim.
- Add a source/count note at the top showing approximate hits screened, relevant hits considered, retained count, and when applicable that additional relevant hits were omitted because of the 50-paper cap.

Journal categories to prioritize:
1. High-impact journals: Nature, Science, Cell, Nature Medicine, Nature Immunology, Nature Neuroscience, Nature Aging, Nature Communications, Science Translational Medicine, Cell Reports, Cell Reports Medicine.
2. Neuroscience / neurology: Neuron, Nature Neuroscience, Brain, Annals of Neurology, Movement Disorders, Acta Neuropathologica, npj Parkinson's Disease, Parkinsonism & Related Disorders.
3. Immunology: Immunity, Nature Immunology, Science Immunology, Cell Host & Microbe, Journal of Experimental Medicine, Journal of Clinical Investigation, JCI Insight, Nature Reviews Immunology, Frontiers in Immunology.
4. Neuroinflammation / glia: Glia, Journal of Neuroinflammation, Brain Behavior and Immunity, Molecular Neurodegeneration, Neurobiology of Disease.
5. Methods / single-cell / spatial: Nature Methods, Nature Biotechnology, Genome Biology, Cell Systems, Nature Genetics, Science Advances, eLife.
6. Mechanism-inspiration sources: strong cancer immunology, infection/immunity, barrier biology, vascular biology, gut microbiome, myeloid biology, T-cell biology, single-cell/spatial papers if they offer transferable ideas for Parkinson's disease neuroimmunology.

Expanded search strategy represented in the collector:
A. Direct PD search: Parkinson*, alpha-synuclein, Lewy body, synucleinopathy, PINK1, Parkin, LRRK2, GBA.
B. Direct PD plus immune/neuroimmune terms: monocyte, macrophage, microglia, T cell, lymphocyte, meninges, neuroinflammation, immune, gut, microbiome, endothelial, BBB, chemokine, cytokine, interferon, inflammasome, complement, antigen presentation, cGAS-STING.
C. Broad neuroimmune mechanism search: myeloid/T-cell/barrier/chemokine/interferon/inflammasome/complement/TREM2/APOE/gut-brain terms crossed with neurodegeneration, brain, CNS, neuron, dopaminergic, glia, aging, proteostasis, autophagy, lysosome, or mitochondria.

Filtering and ranking:
- Prioritize mechanism and idea value over strict disease match.
- Include direct PD hits when they are mechanistically useful, especially immune, gut, lysosome/autophagy, mitochondria, alpha-synuclein handling, barrier, or glial biology.
- Exclude generic clinical management, unrelated imaging, corrections/errata unless scientifically important, AI-only reports, and purely peripheral immune papers with no clear mechanism link.
- Rank papers by relevance within each section while respecting the 50-paper total cap.

Word report title: Daily Parkinson Neuroimmune Paper Scan.
Organize papers under these concise sections:
1. Direct PD / synucleinopathy relevance
2. Neuroimmune mechanism relevance

For each paper include:
- English Title
- Chinese Translation of Title
- Journal or bioRxiv/medRxiv
- One-sentence novelty summary in English
- One short 'Why useful' note, focused on how it may inspire Parkinson's/neuroimmune research
- Link or DOI

Translation and quality gate:
- Chinese titles must be natural, field-aware Chinese translations, not word-by-word dictionary replacement.
- Preserve standard technical terms when appropriate, e.g. alpha-synuclein, AADC, PINK1, T cell, single-cell, spatial omics.
- Do not run or reuse build_daily_report_from_candidates.py; that legacy builder is disabled because it used a bad literal translation path.
- If the Chinese-title quality check fails, fix the DOCX before sending. Do not email a report that fails this check.
- If Documents rendering is available, render the DOCX and inspect the PNG pages before sending; otherwise at minimum perform the text quality check and report the limitation.

Style rules:
- No long summaries.
- One novelty sentence only.
- Max 4-5 short lines per paper.
- Be concise, precise, and useful for fast filtering.
- Clearly mark preprints.
- Clearly say when no strong hits are found in a source category.

Continue running until the task is fully completed.
