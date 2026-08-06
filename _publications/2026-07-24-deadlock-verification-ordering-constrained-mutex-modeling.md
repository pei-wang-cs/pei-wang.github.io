---
title: "Deadlock Verification via Ordering-Constrained Mutex Modeling"
collection: publications
category: conferences
permalink: /publication/deadlock-verification-ordering-constrained-mutex-modeling/
excerpt: "An ordering-constrained mutex model for precise deadlock verification in partial-order-based concurrent verification frameworks."
date: 2026-07-24
venue: "38th International Conference on Computer Aided Verification (CAV 2026)"
paperurl: "https://doi.org/10.1007/978-3-032-32519-8_3"
artifacturl: "https://doi.org/10.5281/zenodo.19696864"
citation: "Pei Wang, Zhilei Han, Zhihang Sun, and Fei He. (2026). &quot;Deadlock Verification via Ordering-Constrained Mutex Modeling.&quot; <i>Computer Aided Verification (CAV 2026)</i>, LNCS 16682, pp. 42–66."
---

Mutex abstractions based on assumptions work well for conventional safety verification, but they do not preserve enough mutex semantics for accurate deadlock verification. This work models mutex operations with ordering constraints, allowing deadlocks to be verified within partial-order-based concurrent verification frameworks.

We formalize the approach, prove its correctness, and implement it in **DEAGLE-DL**. The evaluation shows improved precision over a bounded model checker using conventional mutex modeling and a state-of-the-art static deadlock analyzer, while retaining practical efficiency.

- [Publisher version](https://doi.org/10.1007/978-3-032-32519-8_3)
- [Reproducibility artifact](https://doi.org/10.5281/zenodo.19696864)

BibTeX
------

```bibtex
@inproceedings{wang2026deadlock,
  author    = {Pei Wang and Zhilei Han and Zhihang Sun and Fei He},
  title     = {Deadlock Verification via Ordering-Constrained Mutex Modeling},
  booktitle = {Computer Aided Verification},
  series    = {Lecture Notes in Computer Science},
  volume    = {16682},
  pages     = {42--66},
  publisher = {Springer Nature Switzerland},
  year      = {2026},
  doi       = {10.1007/978-3-032-32519-8_3}
}
```
