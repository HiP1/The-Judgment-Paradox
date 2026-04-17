# The Judgment Paradox

**Disagreement Valuation, Annotation Pipelines, Synthetic Data, and the Case for Preservation**

Ivan Phan · Independent Researcher · ORCID: [0009-0003-1095-5855](https://orcid.org/0009-0003-1095-5855)

April 2026 · CC BY 4.0 · DOI: [10.5281/zenodo.19594378](https://doi.org/10.5281/zenodo.19594378)

## Summary

Current annotation pipelines for RLHF and related training methods destroy valuable information by collapsing expert disagreement into single consensus labels. The information loss extends beyond disagreement: even when experts agree, the reasoning behind their agreement is discarded.

This paper proposes a redesigned annotation pipeline and introduces the **Rich Annotation Object (RAO)**: a structured data format replacing binary preference labels with full judgment distributions, per-annotator reasoning, cross-review matrices, and disagreement classification. The pipeline is a signal enrichment tool across the entire distribution of expert judgment.

The paper identifies RL optimisation as structurally hostile to calibrated uncertainty on contested items and recommends **supervised fine-tuning (SFT)** as the primary integration path. **Eight testable predictions** with named falsifiers are derived from established cognitive science and uncertainty-communication findings. The pipeline is not empirically tested; a pilot study design is proposed.

This paper developed two threads during writing. It began as annotation pipeline design. During integration of the April 2026 safety literature on subliminal learning (Cloud et al.), persona features (Wang et al.), alignment faking (Greenblatt et al.), and sleeper agents (Hubinger et al.), a second thread emerged about training-signal provenance. The paper now develops both. The connecting through-line is the argument that training signals must ground in one of three auditable sources: **formal systems, physical execution, or traceable human experts**. The RAO is the third grounding point and the only one that operates in contested domains where formal systems and physical execution cannot adjudicate.

This is a collaboration invitation.

## Reading the Paper

**HTML** (primary reading experience): [Read online](https://hip1.github.io/The-Judgment-Paradox/the-judgment-paradox.html)
- Floating table of contents
- Light/dark mode
- Audience-coded sections

**PDF** (for archival/print): [the-judgment-paradox.pdf](the-judgment-paradox.pdf)

**Markdown** (source): [the-judgment-paradox.md](the-judgment-paradox.md)

## Structure

The paper has 13 sections. The reading guide (§1.3) routes readers by background:

- **ML / Alignment:** §1–§4, §9 (pipeline, integration, downstream applications, predictions; §4.2 develops the safety chain and grounding framework)
- **Annotation Science:** §5–§6, §10 (evidence base, literature context, cost analysis)
- **Workforce / Ethics:** §7–§8 (expert valuation, apprenticeship layer, education extension)
- **Cognitive Science / Education:** §9 (eight predictions with falsifiers)

## Key Contributions

1. The **Rich Annotation Object** (RAO) schema with JSON specification
2. The **propagation problem** analysis and SFT recommendation
3. **RLHD** (Reinforcement Learning from Human Disagreement) as a paradigm label
4. The **three-grounding-points principle**: training signals must ground in formal systems, physical execution, or traceable human experts to escape the synthetic-data safety chain
5. **RLVR disaggregation**: distinguishes programmatic verification (grounded) from model-based verification (ungrounded), and notes that "verifiable rewards" in practice often route through models at the correctness-judgment step
6. Twelve downstream applications from a single data object
7. Eight testable predictions grounded in established literature (cognitive science, argumentation studies, uncertainty communication)
8. Cross-domain reviewer design variant
9. **Failure mode 7**: expert fallibility and disclosure reluctance, grounded in Cooke's Physicians' Reaction to Uncertainty instrument and related work
10. Signal enrichment reframe (the RAO enriches the entire 100%, not just disagreement)

## Safety Chain Integration

§4.2 engages the April 2026 alignment safety literature:

- Betley et al. (ICML 2025): emergent misalignment from narrow fine-tuning
- Cloud et al. (Nature 2026): subliminal learning through filtered data
- Wang et al. (ICLR 2026): persona features and subtle-error misalignment
- Denison et al. (2024): sycophancy generalises to reward tampering
- Greenblatt et al. (2024): alignment faking
- Hubinger et al. (2024): sleeper agents persist through safety training
- Casper et al. (2024): black-box access insufficient for rigorous audits

The common structural feature across these findings: training signals whose provenance depends on a previous model carry latent traits that semantic filtering cannot remove and behavioural evaluation cannot reliably detect. The RAO's human-expert grounding is positioned as the escape mechanism for contested domains where formal systems and physical execution cannot adjudicate.

## Related Work

This paper connects to but is independently motivated from:

- [Confidence Curriculum](https://hip1.github.io/confidence-curriculum/) (Phan 2026a–f)
- [Uncertainty Collapse](https://hip1.github.io/Uncertainty-Collapse/) (Phan 2026g, DOI: [10.5281/zenodo.19482051](https://doi.org/10.5281/zenodo.19482051))

## Methodology

Developed using an adversarial triad methodology. Three frontier AI systems (Claude, ChatGPT, Gemini) served as collaborative drafting and review partners with distinct analytical roles. The author retained sole editorial authority over all content, structure, and argumentation decisions. See the Author's Note in the paper.

## Citation

See [CITATION.cff](CITATION.cff) or cite as:

> Phan, I. (2026). The Judgment Paradox: Disagreement Valuation, Annotation Pipelines, Synthetic Data, and the Case for Preservation. DOI: [10.5281/zenodo.19594378](https://doi.org/10.5281/zenodo.19594378)

## Licence

This work is licensed under [CC BY 4.0](https://creativecommons.org/licenses/by/4.0/). See [LICENSE](LICENSE).
