---
layout: archive
title: "Research"
permalink: /research/
author_profile: true
---

My research lies at the intersection of **probabilistic machine learning**, **computational statistics**, and **deep learning**. I am broadly interested in developing rigorous, uncertainty-aware methods that are both theoretically grounded and practically effective.

---

## Probabilistic Machine Learning

I am interested in Bayesian approaches to learning, where uncertainty is treated as a first-class citizen. Key topics include:

- **Bayesian inference** and approximate posterior methods
- **Uncertainty quantification** in neural network predictions
- **Probabilistic forecasting** for real-world time series

---

## Computational Statistics

A significant part of my work focuses on the computational aspects of statistical inference:

- **Monte Carlo methods** and sequential Monte Carlo
- **Kernel-based methods** for statistical testing and discrepancy measures
- **Stein operators** and related techniques in modern computational statistics

---

## Deep Learning

I apply and develop deep learning architectures for structured data problems:

- **Sequence modelling** — Temporal Convolutional Networks, Transformers
- **Graph Neural Networks** — CoGraphNet and co-occurrence graph representations
- **Sparse attention mechanisms** for efficient long-range dependency modelling

---

## Selected Publications

<ul>{% for post in site.publications reversed %}
  {% include archive-single.html %}
{% endfor %}</ul>
