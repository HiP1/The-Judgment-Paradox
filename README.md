# The Judgment Paradox

**Disagreement Valuation, Annotation Pipelines, and the Case for Preservation**

Ivan Phan · Independent Researcher · ORCID: [0009-0003-1095-5855](https://orcid.org/0009-0003-1095-5855)

April 2026 · CC BY 4.0

## Summary

Current annotation pipelines for RLHF and related training methods destroy valuable information by collapsing expert disagreement into single consensus labels. The information loss extends beyond disagreement: even when experts agree, the reasoning behind their agreement is discarded.

This paper proposes a redesigned annotation pipeline and introduces the **Rich Annotation Object (RAO)**: a structured data format replacing binary preference labels with full judgment distributions, per-annotator reasoning, cross-review matrices, and disagreement classification. The pipeline is a signal enrichment tool across the entire distribution of expert judgment.

The paper identifies RL optimisation as structurally hostile to calibrated uncertainty on contested items and recommends **supervised fine-tuning (SFT)** as the primary integration path. Seven testable predictions with named falsifiers are derived from established cognitive science findings. The pipeline is not empirically tested; a pilot study design is proposed.

This is a collaboration invitation.

## Reading the Paper

**HTML** (primary reading experience): [the-judgment-paradox.html](the-judgment-paradox.html)
- Floating table of contents
- Light/dark mode
- Audience-coded sections

**PDF** (for archival/print): [the-judgment-paradox.pdf](the-judgment-paradox.pdf)

**Markdown** (source): [the-judgment-paradox.md](the-judgment-paradox.md)

## Structure

The paper has 13 sections. The reading guide (§1.3) routes readers by background:

- **ML / Alignment:** §1–§4, §9
- **Annotation Science:** §5–§6, §10
- **Workforce / Ethics:** §7–§8
- **Cognitive Science / Education:** §9

## Key Contributions

1. The **Rich Annotation Object** (RAO) schema with JSON specification
2. The **propagation problem** analysis and SFT recommendation
3. **RLHD** (Reinforcement Learning from Human Disagreement) as a paradigm label
4. Twelve downstream applications from a single data object
5. Seven testable predictions grounded in established psychology (Nisbett, Kuhn, Schwartz, Wiley, Nathan)
6. Cross-domain reviewer design variant
7. Signal enrichment reframe (the RAO enriches the entire 100%, not just disagreement)

## Related Work

This paper connects to but is independently motivated from:

- [Confidence Curriculum](https://hip1.github.io/confidence-curriculum/) (Phan 2026a–f)
- [Uncertainty Collapse](https://hip1.github.io/Uncertainty-Collapse/) (Phan 2026g, DOI: [10.5281/zenodo.19482051](https://doi.org/10.5281/zenodo.19482051))

## Methodology

Developed using an adversarial triad methodology. Three frontier AI systems (Claude, ChatGPT, Gemini) served as collaborative drafting and review partners. The author retained sole editorial authority. See the Author's Note in the paper.

## Citation

See [CITATION.cff](CITATION.cff) or cite as:

> Phan, I. (2026). The Judgment Paradox: Disagreement Valuation, Annotation Pipelines, and the Case for Preservation. DOI: [10.5281/zenodo.19594378](https://doi.org/10.5281/zenodo.19594378)

## Licence

This work is licensed under [CC BY 4.0](https://creativecommons.org/licenses/by/4.0/). See [LICENSE](LICENSE).
