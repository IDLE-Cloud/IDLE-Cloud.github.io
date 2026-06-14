---
layout: archive
title: "CV"
permalink: /cv/
author_profile: true
redirect_from:
  - /resume
---

{% include base_path %}

Jianqiao Zeng (曾健桥)
======
Shanghai, China · zengjianqiao5@gmail.com · [GitHub](https://github.com/IDLE-Cloud)

Incoming Ph.D. student working on **deep learning architectures**, **representation learning**, and **AI agents**.

Education
======
* **Ph.D. in Computer Science**, AI³ Institute, Fudan University, Shanghai Academy of AI for Science, 2026.09 – present *(incoming)*
  * Advisors: Prof. Hao Xiong (Fudan), Prof. Junchi Yan (SJTU)
* **B.E. in Artificial Intelligence**, Sun Yat-sen University (中山大学), 2022.09 – 2026.06

Publications
======
  <ul>{% for post in site.publications reversed %}
    {% include archive-single-cv.html %}
  {% endfor %}</ul>

Research Experience
======

* **CoEvol-NO: Co-Evolutionary Neural Operator with Error-Driven Predictor-Corrector Framework**
  *First author · Advisors: Prof. Junchi Yan, Prof. Hao Xiong · ICML 2026 (CCF-A) Oral · 2025.10 – 2026.05*
  * **Paradigm innovation:** Identified the structural trade-off between *geometric sensitivity* and *dynamic memory* in existing neural operators; proposed **Co-Evolution** as a third paradigm — latent state and mesh sequence evolve jointly through bidirectional updates.
  * **Theoretical unification:** Proved that residual connections and direct substitution are first-order approximations of a single Error-Driven Correction framework under different loss assumptions; introduced **exact Jacobian gradient** to upgrade updates to full optimization. Formalized the symmetry-induced stability advantage and condition-number cost.
  * **Empirical validation:** Achieved SOTA on 5 standard PDE benchmarks and 2 industrial tasks. 40-layer deep extension shows Navier-Stokes error decreases monotonically (48% drop). PC framework transfers consistently to Transolver and LNO. [Code](https://github.com/IDLE-Cloud/CoEvol-NO)

* **FreqONet: Frequency-Domain Operator Learning via Dimensional Decomposition**
  *First author · Advisor: Prof. Junchi Yan · Manuscript under review · 2025.01 – 2025.07*
  * **Decoupled-Composed framework:** Reformulated high-dimensional PDE solving as a two-stage process — independent 1D coordinate encoding followed by strict composition. Systematically analyzed four composition strategies (Cat / Add / Hadamard / Outer Product); proved **tensor product** is the unique composition preserving both orthogonality and translation-invariant kernel properties.
  * **Universal approximation:** Based on Stone-Weierstrass theorem, proved that if each 1D encoding subspace is dense in $C(K_i)$, then the tensor-product span is dense in $C(K_1 \times \cdots \times K_d)$.
  * **Hybrid encoding (FreqPE):** Decomposed encoding space into fixed-orthogonal basis (high-frequency structure prior) plus learnable basis (low-frequency data-driven) with a complementary loss enforcing orthogonality.

* **AMQuestioner: Training Critical Thinking with Question-Driven Interactive Argument Maps in Online Discussion**
  *Co-first author · Advisor: Prof. Zhenhui Peng · [CSCW 2025](https://dl.acm.org/doi/10.1145/3757551) · 2023.11 – 2024.10*
  * Designed and developed a critical-thinking training system combining argument maps with LLMs.
  * Frontend (Vue.js) for mind-map visualization and question-driven interaction; backend (Flask RESTful) for LLM role-play prompt design and adaptive opinion exploration.
  * Led user-experiment design, execution, and data analysis; wrote the core paper sections.

* **Learning Agent: Problem-DAG-Driven Personal Knowledge Tracking and Adaptive Learning**
  *Independent project · 2026.04 – present*
  * **Core insight:** "Mastering a domain = answering its core question set." Models knowledge as a DAG (multi-parent + cross-domain links); learning progress measured by question-decomposition depth, not reading volume.
  * **Methodology & feedback loop:** Designed 5 question decomposition methods (prerequisite / component / contrast / causal chain / assumption clarification); AI generates questions only, not answers. CHECK-DECIDE mechanism propagates answer updates via the DAG, marking downstream nodes as STALE for consistency cascade.
  * **Engineering:** React + Vite + Tailwind static frontend with infinite SVG canvas, three views (radial / text tree / focus navigator), global knowledge graph, statistics dashboard. 9 Claude Code skills + Python CLI for node lifecycle management.

Selected Open-Source Projects
======
* **Skill-Manager** — Skill lifecycle management tool (registration, call counts, user feedback collection, A/B evaluation).
* **CoEvol-NO** — Co-evolutionary neural operator framework. [GitHub](https://github.com/IDLE-Cloud/CoEvol-NO)
* **Learning Agent** — Graph-driven dialogue-based learning system.

Skills
======
* **Programming:** Python (expert), C/C++, CUDA, Bash, LaTeX
* **Deep Learning:** PyTorch (expert), JAX, Hugging Face Transformers
* **Tools:** Claude Code, Git, Linux, Docker
* **Theory:** Matrix theory, functional analysis, convex optimization
* **Reproductions:** PINN, FNO, CNO, DeepONet, DDPM, DiT

Professional Service
======
* (To be added — conference reviewing, mentoring, open-source contributions)
