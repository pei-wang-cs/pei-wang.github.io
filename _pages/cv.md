---
layout: archive
title: "Curriculum Vitae"
permalink: /cv/
author_profile: true
redirect_from:
  - /resume
---

{% include base_path %}

Education
------
- **2023–present:** Ph.D. student, School of Software, Tsinghua University, Beijing, China

Research Interests
------
- Formal methods and software verification
- Concurrent program verification
- Deadlock and data-race analysis
- SMT-based and partial-order-based verification

Publications
------
<ul>
{% for publication in site.publications reversed %}
  <li>
    <a href="{{ base_path }}{{ publication.url }}"><strong>{{ publication.title }}</strong></a><br>
    {{ publication.citation }}
  </li>
{% endfor %}
</ul>

Research Software
------
- **DEAGLE-DL:** Artifact for deadlock verification via ordering-constrained mutex modeling. [[DOI](https://doi.org/10.5281/zenodo.19696864)]
- **DEAGLE-DR:** Artifact for precise and efficient static data-race detection. [[DOI](https://doi.org/10.5281/zenodo.21744663)]

Contact
------
- Email: [wang-p23@mails.tsinghua.edu.cn](mailto:wang-p23@mails.tsinghua.edu.cn)
- ORCID: [0009-0007-0437-9141](https://orcid.org/0009-0007-0437-9141)
- GitHub: [pei-wang-cs](https://github.com/pei-wang-cs)
