# Modeling the Regulatory Effects of Non-Coding Variants with AlphaGenome and CNN-Based Enhancer Classification

**NIH / National Library of Medicine (NLM) | Approved research poster**  
**Poster authors:** Yash Maheshwaran, Gaetano Manzo, and Ivan Ovcharenko

**[View the approved NIH research poster (PDF)](NIH_AlphaGenome_Poster_Yash_Maheshwaran.pdf)**

## Research leadership and contributions

**Yash Maheshwaran — lead computational researcher and first author of the poster.** I conducted the primary computational research and created the poster, including its scientific narrative, figures, and presentation of the results. My principal contributions include:

- Developing and evaluating the K562 enhancer-classification workflow using AlphaGenome-derived regulatory features and CNN modeling.
- Implementing and analyzing REF/ALT regulatory variant-effect predictions and comparisons with independent K562 SuRE and MPRA measurements.
- Integrating predicted RNA effects with independent eQTL, chromatin-contact, and enhancer–gene evidence to prioritize candidate variant-to-gene relationships.
- Running the computational analyses, interpreting the results and their limitations, and preparing the research poster.

**Manuscript status:** A **first-author manuscript is in preparation** based on this ongoing research. It is not yet published or accepted.

This is collaborative research at NIH/NLM. **Gaetano Manzo** contributed research mentorship and scientific collaboration, and **Ivan Ovcharenko** is the supervising principal investigator. Both are credited as coauthors of the approved poster.

## Research question

Noncoding genetic variants can alter enhancer activity, but connecting those changes to downstream gene expression and identifying plausible target genes remains challenging. This project asks whether K562 enhancer classification, AlphaGenome-predicted RNA effects, and independent gene-link evidence can help prioritize regulatory variant-to-gene hypotheses.

## Approach

1. **Enhancer classification:** Integrate AlphaGenome-derived multimodal regulatory features and train a CNN to distinguish K562 enhancer and control intervals.
2. **Variant-effect scoring:** Compare reference and alternate sequence predictions, using both continuous scores and threshold-based enhancer-state changes.
3. **Independent experimental comparison:** Assess predicted effect directions using published K562 SuRE and MPRA reporter-assay measurements.
4. **Target-gene prioritization:** Combine enhancer effects, AlphaGenome RNA predictions, and independently sourced eQTL, 3D-contact, and enhancer–gene link evidence.

## Selected findings from the approved poster

| Analysis | Poster-reported result |
| --- | --- |
| K562 enhancer classifier | Validation AUROC **0.9803** and AUPRC **0.9827** |
| Enhancer-state changes | **29** threshold-crossing variants: **23** predicted enhancer losses and **6** gains |
| Reporter-assay direction comparisons | **76%** K562 SuRE; **74%** K562 MPRA; **70%** same direction across all three |
| Empirical variant–gene links | **24/29** threshold-crossing variants had empirical gene-link evidence |
| Enhancer–RNA coherence | **26/28** variants showed directional coherence in the reported subset |

These results support **evidence-guided candidate variant-to-gene prioritization**, not independent experimental proof of causal gene regulation.

## Materials and research status

- **[Approved NIH poster (PDF)](NIH_AlphaGenome_Poster_Yash_Maheshwaran.pdf)**: Publicly shared with authorization.
- **Underlying research code and data**: Not publicly available. The active NIH project, ongoing analyses, and unpublished manuscript materials remain private.

This repository hosts an approved scientific poster and its contextual summary; it is **not** the full NIH research codebase.

## Acknowledgments

Research performed at the National Library of Medicine, National Institutes of Health, with Gaetano Manzo and Ivan Ovcharenko. Supported by NIH/NLM's Division of Intramural Research and DSI program; computations used NIH Biowulf HPC resources. See the poster for figures, scientific references, and further details.
