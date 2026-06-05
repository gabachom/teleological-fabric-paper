# Teleological Fabric

**Knowledge systems that match purpose, not words.**

This repository hosts the manuscript, supplementary materials, and citation information for *Teleological Fabric (TF)* — a framework for organizing expert domain knowledge as reusable judgment patterns ("Noema") bound to purpose, context, and procedure, evaluated against four novel metrics that target properties invisible to standard information-retrieval evaluation.

---

## Paper

**Title:** *From Text Similarity to Teleology: Knowledge Systems That Match Purpose, Not Words*

**Author:** Masayuki Tomoyasu (友安 昌幸), Amiko Consulting, LLC

**Status:**

| Channel | State |
| --- | --- |
| arXiv (cs.AI / cs.IR / cs.HC) | endorsement in progress |
| Zenodo (knowledge-management framing) | ✅ **v2**: [DOI: 10.5281/zenodo.20554806](https://doi.org/10.5281/zenodo.20554806) (150 queries × 406 Noemas, 2026-06-05) — v1 archived at [10.5281/zenodo.20500954](https://doi.org/10.5281/zenodo.20500954) |
| Substack series (4 posts) | rolling launch, July 30 2026 |

**One-paragraph abstract.** Current retrieval-augmented generation (RAG) and dense-retrieval systems retrieve passages by text similarity, but expert decision making requires matching to *purpose* — the goal under which a piece of knowledge becomes usable — and to *wearer constraints* (role, authority, and context of the practitioner who will act on the retrieved knowledge). This paper introduces **Teleological Fabric (TF)**, a framework that organizes domain knowledge as **Noema** — reusable judgment patterns binding purpose, context, and procedure — and operates via six core mechanisms supported by a Purpose Tree, Grounding Chain, Wearer Constraint, and Inconsistency Detection structures. We propose four novel evaluation metrics — **Purpose Alignment Recall (PAR)**, **Grounding Chain Score (GCS)**, **Wearer Compatibility Score (WCS)**, and **Cross-Source Reconciliation (CSR)** — that target properties invisible to standard IR evaluation. A pilot empirical study (30 queries × 173 compiled Noemas × 3 retrieval systems) shows TF outperforms BM25 and TF-IDF baselines on all four novel metrics, while TF-IDF retains the edge on standard P@5 and MRR. We argue this asymmetry is consistent with the framework's thesis rather than against it: different metrics measure different properties, and standard IR metrics are not designed to capture purpose alignment or grounding integrity.

---

## Repository contents

```
.
├── README.md                  ← this file
├── LICENSE                    ← CC BY 4.0
├── CITATION.cff               ← machine-readable citation
└── paper/
    └── tf-paper-v1.pdf        ← full manuscript (24 pages)
```

Supplementary code and data for the pilot empirical study (BrainBench-TF, 30 queries / 173 Noemas / 3 systems / 8 metrics) are maintained in a separate directory in the project workspace; reproduction instructions will be added in a future revision of this repository.

---

## Key contributions

1. **The level question.** TF organizes knowledge at the level of *judgment patterns* — distinct from data, information, knowledge, skill, and workflow. Prior systems (knowledge graphs, RAG, PKM tools, workflow engines) operate one or more levels below.

2. **Four novel metrics.** PAR, GCS, WCS, and CSR target properties that classical IR metrics (precision, recall, MRR, F1) were never designed to measure. PAR has roots in intent-aware IR (Broder 2002; Jansen et al. 2008); GCS draws on provenance and faithfulness work (Buneman et al. 2001; Min et al. 2023; Es et al. 2024); CSR is informed by triangulation and data fusion (Denzin 1978; Bleiholder & Naumann 2008; Pasternack & Roth 2010); WCS is, to our knowledge, novel.

3. **Empirical asymmetry as evidence.** In a pilot study, TF wins all four novel metrics; TF-IDF wins standard P@5 and MRR. We argue this is the expected pattern when distinct measurement properties are being captured — the asymmetry supports the framework rather than refuting it.

4. **A computational successor in spirit, not in substance.** TF draws inspiration from Nonaka's SECI model and Polanyi's tacit dimension, yet advances beyond them in scope and form, drawing additionally on phenomenology (Husserl), active inference (Friston), and three decades of organizational learning research.

---

## Citation

If you use TF, Noema, or any of the four metrics in your work, please cite:

```bibtex
@article{tomoyasu2026teleological,
  title   = {From Text Similarity to Teleology:
             Knowledge Systems That Match Purpose, Not Words},
  author  = {Tomoyasu, Masayuki},
  year    = {2026},
  journal = {arXiv preprint},
  note    = {Endorsement and submission in progress;
             Zenodo version forthcoming},
  url     = {https://github.com/gabachom/teleological-fabric-paper}
}
```

A machine-readable citation is available in [`CITATION.cff`](CITATION.cff). GitHub will render a "Cite this repository" button automatically.

---

## Related resources

- **Book (Japanese).** *拡張脳：脳の続きは、纏う者とともに成長する* — a long-form treatment of the same framework for a general professional audience. Forthcoming.
- **Substack series (English).** Four posts unpacking the paper for non-academic readers: (1) the purpose gap; (2) Noema as the unit of expert judgment; (3) four new metrics; (4) the six mechanisms and what they imply for KM practice.
- **Workshops.** Practitioner workshops on building one's own Augmented Brain are delivered through Amiko Consulting, LLC.

---

## License

This work is licensed under [Creative Commons Attribution 4.0 International (CC BY 4.0)](https://creativecommons.org/licenses/by/4.0/). You are free to share and adapt the material for any purpose, including commercial use, as long as appropriate credit is given. See [`LICENSE`](LICENSE) for the full text.

---

## Acknowledgments

This work is respectfully dedicated to the memory of **Professor Ikujiro Nonaka (1935–2025)**, whose SECI model has been the starting point of my professional reflection on knowledge for three decades. Thanks are also due to **Professor Hirotaka Takeuchi (Harvard Business School)** for the foundational work on which decades of research on organizational knowledge rest; to colleagues at Tokyo Electron and Samsung Electronics whose tacit practice over thirty-eight years constitutes the empirical foundation of this work; and to the Anthropic team for the Claude platform on which much of this research was conducted.

---

## Contact

- **Author:** Masayuki Tomoyasu (友安 昌幸)
- **Affiliation:** Amiko Consulting, LLC, Tokyo, Japan
- **Email:** masa.tomoyasu@amiko.consulting

Issues, corrections, and proposals for collaboration are welcome via GitHub Issues.
