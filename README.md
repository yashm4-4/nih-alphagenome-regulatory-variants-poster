# Modeling the Regulatory Effects of Non-Coding Variants with AlphaGenome and CNN-Based Enhancer Classification

**NIH / National Library of Medicine (NLM) | Approved research poster**

**Authors:** Yash Maheshwaran, Gaetano Manzo, and Ivan Ovcharenko

## Overview

Noncoding genetic variants can alter enhancer activity, but linking their regulatory effects to downstream gene expression and identifying plausible target genes remains challenging. This research investigates whether an integrated approach combining K562 enhancer classification, AlphaGenome-predicted RNA effects, and independent gene-link evidence can help prioritize variant-to-gene hypotheses.

The accompanying NIH/NLM research poster describes the project and its results. **This repository is a public presentation of the approved poster, not a release of the underlying research code or data.**

## Approach

1. **Regulatory feature modeling:** Use AlphaGenome-derived chromatin/regulatory features and a CNN to classify K562 enhancer versus control intervals.
2. **Variant-effect scoring:** Compare reference and alternate sequence predictions to assess changes in enhancer activity, retaining continuous scores and identifying predicted enhancer-state changes at a defined threshold.
3. **Independent comparison:** Compare predicted enhancer-effect directions with K562 SuRE and MPRA reporter-assay measurements.
4. **Candidate gene prioritization:** Combine enhancer effects, AlphaGenome RNA predictions, and external eQTL, chromatin-contact, and enhancer–gene evidence to prioritize candidate target genes.

## Selected findings from the poster

| Analysis | Poster-reported result |
| --- | --- |
| K562 enhancer classifier | Validation AUROC **0.9803**, AUPRC **0.9827** |
| Variant enhancer-state changes | **29** threshold-crossing variants: **23** predicted enhancer losses and **6** gains |
| Reporter-assay direction comparisons | **76%** K562 SuRE; **74%** K562 MPRA; **70%** same direction across all three |
| Variant-to-gene evidence | **24/29** threshold-crossing variants had empirical gene-link evidence |
| Enhancer/RNA consistency | **26/28** variants showed enhancer–RNA directional coherence in the reported subset |

The gene-link analyses are used to generate and prioritize *hypotheses*, not to assert experimental proof of causal target genes.

## Authors and acknowledgments

**Yash Maheshwaran, Gaetano Manzo, Ivan Ovcharenko**  
National Library of Medicine, National Institutes of Health

The research was supported by the NIH/NLM Division of Intramural Research and DSI program and used NIH Biowulf high-performance computing resources.

## Materials and availability

The approved poster PDF is intended to be hosted in this repository. The active NIH research repository and its unpublished analyses, source code, and underlying data remain private. Public release of this poster does **not** imply that the broader research project is open source.

Please consult the poster for figures, detailed methods, and literature references.
