---
title: "Deadlock Verification via Ordering-Constrained Mutex Modeling"
collection: publications
category: conferences
permalink: /publication/deadlock-verification-ordering-constrained-mutex-modeling/
excerpt: >-
  Mutexes are widely used to synchronize concurrent programs, but incorrect
  locking can cause deadlocks. Conventional assume-based encodings support
  safety checking while abstracting away waiting behavior, which can make
  deadlock results inaccurate. This paper introduces ordering constraints that
  distinguish eventual lock acquisition from indefinite blocking within a
  partial-order-based verification framework. We prove the method correct and
  implement it in the DEAGLE-DL prototype. Experiments against ESBMC with
  conventional mutex modeling and a state-of-the-art static deadlock analyzer
  show markedly better precision while retaining practical efficiency.
date: 2026-07-24
venue: "38th International Conference on Computer Aided Verification (CAV 2026)"
paperurl: "https://doi.org/10.1007/978-3-032-32519-8_3"
artifacturl: "https://doi.org/10.5281/zenodo.19696864"
citation: "Pei Wang, Zhilei Han, Zhihang Sun, and Fei He. (2026). &quot;Deadlock Verification via Ordering-Constrained Mutex Modeling.&quot; <i>Computer Aided Verification (CAV 2026)</i>, LNCS 16682, pp. 42–66."
---

Abstract
--------

Mutexes are widely used to synchronize concurrent programs, but incorrect locking can cause deadlocks. Conventional assume-based encodings support safety checking while abstracting away waiting behavior, which can make deadlock results inaccurate. This paper introduces ordering constraints that distinguish eventual lock acquisition from indefinite blocking within a partial-order-based verification framework. We prove the method correct and implement it in the **DEAGLE-DL** prototype. Experiments against ESBMC with conventional mutex modeling and a state-of-the-art static deadlock analyzer show markedly better precision while retaining practical efficiency.

Links
-----

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
