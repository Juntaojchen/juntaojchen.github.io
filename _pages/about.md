---
permalink: /
title: "About Me"
author_profile: true
redirect_from:
  - /about/
  - /about.html
---
I am **Juntao (Jason) Chen**, an MPhil candidate in the School of Mathematics, Statistics and Physics at Newcastle University, and I am fortunate to be supervised by [Prof. Chris Oates](https://www.ncl.ac.uk/maths-physics/people/profile/chrisoates.html).

My research sits at the intersection of **probabilistic machine learning**, **computational statistics**, and **deep learning** — with a focus on developing principled, uncertainty-aware methods for real-world problems.

---

## Research Interests

- **Probabilistic Machine Learning** — Bayesian inference, uncertainty quantification
- **Computational Statistics** — Monte Carlo methods, statistical learning theory
- **Deep Learning** — Sequence modelling, graph neural networks, transformers

---

## News

- **Jan 2025** — Paper accepted at *Scientific Reports*: CoGraphNet for enhanced text classification.
- **Nov 2024** — Paper published in *Energy*: Offshore wind power prediction with TCN-DANet-Sparse Transformer.

---

## Selected Awards

| Year | Award |
|------|-------|
| 2023 | International Mathematical Contest in Modeling (MCM/ICM) — **Meritorious Winner** |
| 2023 | National College Student Mathematical Modeling Competition (CUMCM) — **Second Prize** |
| 2022 & 2023 | National College Student Statistical Modeling Competition — **Second Prize** |
| 2021–2023 | University-level **Special Scholarship** (3 consecutive years) |
| 2021–2023 | Department **First-Class Scholarship** (3 consecutive years) |

---

## Visitor Map

<style>
.visitor-map-wrap {
  margin-top: 1rem;
  text-align: center;
}

.visitor-map-fallback {
  display: none;
  max-width: 520px;
  margin: 0 auto;
  padding: 0.9rem 1rem;
  border: 1px solid #d8e2ea;
  border-radius: 12px;
  background: #f8fbfd;
  color: #5f6b78;
  font-size: 0.92rem;
  line-height: 1.6;
}
</style>

<div class="visitor-map-wrap">
  <div id="visitor-map-container"></div>
  <div id="visitor-map-fallback" class="visitor-map-fallback">
    The visitor globe sometimes fails to load because the external script can be blocked by network conditions, privacy extensions, or browser protections. If it does not appear, please try refreshing the page.
  </div>
</div>

<script>
  (function () {
    var container = document.getElementById('visitor-map-container');
    var fallback = document.getElementById('visitor-map-fallback');
    if (!container || !fallback) return;

    var script = document.createElement('script');
    script.type = 'text/javascript';
    script.id = 'mmvst_globe';
    script.src = 'https://mapmyvisitors.com/globe.js?d=JaAvWtEeczc9P-6tKzPgSbuvHFP5j7m3PltnLpLiPT8';
    script.async = true;

    var resolved = false;

    script.onload = function () {
      resolved = true;
      fallback.style.display = 'none';
    };

    script.onerror = function () {
      resolved = true;
      fallback.style.display = 'block';
    };

    container.appendChild(script);

    window.setTimeout(function () {
      if (!resolved && container.children.length <= 1) {
        fallback.style.display = 'block';
      }
    }, 4000);
  })();
</script>
