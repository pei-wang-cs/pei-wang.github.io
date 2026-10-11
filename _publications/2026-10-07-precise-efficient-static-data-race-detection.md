---
title: "Precise and Efficient Static Data Race Detection"
collection: publications
category: conferences
authors:
  - Pei Wang
  - Zhihang Sun
  - Fei He
venue_short: "ASE 2026"
permalink: /publication/precise-efficient-static-data-race-detection/
excerpt: >-
  Deagle-DR detects data races in concurrent programs by constraining the order
  of individual events, without instrumenting the program. The approach is
  precise within a bounded scope and comes with a correctness proof. Extensions
  to ordering-consistency solvers support race reasoning, while value-critical
  events help remove unnecessary constraints. Experiments compare the prototype
  with five existing race detectors and demonstrate competitive performance.
date: 2026-10-07
venue: "41st IEEE/ACM International Conference on Automated Software Engineering (ASE 2026)"
paperurl: "https://doi.org/10.1145/3832783.3837438"
artifacturl: "https://doi.org/10.5281/zenodo.21775785"
citation: "Pei Wang, Zhihang Sun, and Fei He. (2026). &quot;Precise and Efficient Static Data Race Detection.&quot; <i>Proceedings of the 41st IEEE/ACM International Conference on Automated Software Engineering (ASE ’26)</i>, pp. 1793–1805."
---

Abstract
--------

Data races pose a serious threat to the correctness of concurrent programs.
Traditional model-checking-based race detection techniques typically encode race detection as assertion verification, but this introduces substantial overhead due to numerous auxiliary variables and statements.
In this paper, we present a precise modeling of data races based on event-level ordering constraints, which avoids any instrumentation while capturing the exact semantics and covering all potential race occurrences within the given bounded scope.
We integrate it into a concurrent program verification framework and prove its correctness.
Moreover, we enhance the existing theory solvers for ordering consistency theory with two new components, enabling effective reasoning about data races.
Finally, we introduce an encoding optimization that leverages the novel concept of value-critical events to eliminate redundant value constraints.
We implement our approach in a prototype tool, Deagle-DR, and compare it against state-of-the-art tools, including Dartagnan, Ugemcutter, Cseq-DR, LaDR, and Iekke.
Experiments show that our approach is competitive with state-of-the-art methods.

Links
-----

- [Publisher version](https://doi.org/10.1145/3832783.3837438)
- [Reproducibility artifact](https://doi.org/10.5281/zenodo.21775785)
- [Conference page and abstract](https://conf.researchr.org/details/ase-2026/ase-2026-research-track/142/Precise-and-Efficient-Static-Data-Race-Detection)

BibTeX
------

```bibtex
@inproceedings{wang2026precise,
  author    = {Pei Wang and Zhihang Sun and Fei He},
  title     = {Precise and Efficient Static Data Race Detection},
  booktitle = {Proceedings of the 41st IEEE/ACM International Conference on Automated Software Engineering},
  series    = {ASE '26},
  pages     = {1793--1805},
  publisher = {Association for Computing Machinery},
  year      = {2026},
  doi       = {10.1145/3832783.3837438},
  url       = {https://doi.org/10.1145/3832783.3837438}
}
```
