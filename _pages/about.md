---
permalink: /
title: "About Me"
author_profile: true
redirect_from:
  - /about/
  - /about.html
---
<style>
.home-wrap {
  --ink: #1f2933;
  --muted: #61707f;
  --line: #d8e2ea;
  --card: #ffffff;
  --soft: #f6f9fc;
  --accent: #0f766e;
  --accent-2: #d97706;
}

.hero-panel {
  position: relative;
  overflow: hidden;
  padding: 1.5rem;
  border: 1px solid var(--line);
  border-radius: 18px;
  background:
    radial-gradient(circle at top right, rgba(15, 118, 110, 0.12), transparent 28%),
    radial-gradient(circle at bottom left, rgba(217, 119, 6, 0.08), transparent 26%),
    linear-gradient(180deg, #ffffff 0%, #f8fbfd 100%);
  box-shadow: 0 14px 36px rgba(15, 23, 42, 0.08);
}

.hero-panel::after {
  content: "";
  position: absolute;
  top: -24px;
  right: -24px;
  width: 140px;
  height: 140px;
  border: 1px solid rgba(15, 118, 110, 0.12);
  border-radius: 999px;
}

.eyebrow {
  margin: 0;
  color: var(--accent);
  text-transform: uppercase;
  letter-spacing: 0.14em;
  font-size: 0.74rem;
  font-weight: 700;
}

.hero-name {
  margin: 0.28rem 0 0;
  color: var(--ink);
  font-size: 2rem;
  line-height: 1.08;
}

.hero-lead {
  margin: 0.75rem 0 0;
  color: var(--ink);
  font-size: 1.02rem;
}

.hero-text {
  margin: 0.85rem 0 0;
  color: var(--muted);
  font-size: 0.98rem;
  max-width: 720px;
}

.tag-row {
  margin-top: 1rem;
  display: flex;
  flex-wrap: wrap;
  gap: 0.55rem;
}

.tag {
  display: inline-flex;
  align-items: center;
  gap: 0.35rem;
  padding: 0.38rem 0.7rem;
  border-radius: 999px;
  background: rgba(255, 255, 255, 0.88);
  border: 1px solid var(--line);
  color: #304152;
  font-size: 0.84rem;
}

.tag::before {
  content: "✦";
  color: var(--accent-2);
  font-size: 0.72rem;
}

.fact-grid {
  margin-top: 1.1rem;
  display: grid;
  grid-template-columns: repeat(3, minmax(0, 1fr));
  gap: 12px;
}

.fact-card {
  border: 1px solid var(--line);
  border-radius: 14px;
  padding: 0.9rem;
  background: rgba(255, 255, 255, 0.78);
  backdrop-filter: blur(4px);
}

.fact-label {
  color: #7b8794;
  text-transform: uppercase;
  letter-spacing: 0.08em;
  font-size: 0.7rem;
}

.fact-value {
  margin-top: 0.22rem;
  color: var(--ink);
  font-weight: 700;
  font-size: 0.95rem;
}

.section-block {
  margin-top: 1.4rem;
  border: 1px solid var(--line);
  border-radius: 18px;
  background: var(--card);
  box-shadow: 0 8px 24px rgba(15, 23, 42, 0.06);
  padding: 1.2rem;
}

.section-title {
  display: flex;
  align-items: center;
  gap: 0.55rem;
  margin: 0 0 0.95rem;
  color: var(--ink);
  font-size: 1.05rem;
}

.section-icon {
  width: 28px;
  height: 28px;
  display: inline-flex;
  align-items: center;
  justify-content: center;
  border-radius: 999px;
  background: #eff7f6;
  color: var(--accent);
  font-size: 0.85rem;
}

.interest-grid {
  display: grid;
  grid-template-columns: repeat(3, minmax(0, 1fr));
  gap: 12px;
}

.interest-card {
  border: 1px solid var(--line);
  border-radius: 14px;
  padding: 1rem;
  background: linear-gradient(180deg, #ffffff 0%, var(--soft) 100%);
}

.interest-num {
  color: #94a3b8;
  font-family: "JetBrains Mono", "SFMono-Regular", Menlo, Consolas, monospace;
  font-size: 0.76rem;
}

.interest-card h3 {
  margin: 0.32rem 0 0.4rem;
  color: var(--ink);
  font-size: 0.96rem;
}

.interest-card p {
  margin: 0;
  color: var(--muted);
  font-size: 0.9rem;
}

.timeline {
  display: grid;
  gap: 12px;
}

.timeline-item {
  display: grid;
  grid-template-columns: 86px 1fr;
  gap: 12px;
  padding: 0.85rem 0.9rem;
  border: 1px solid var(--line);
  border-radius: 12px;
  background: linear-gradient(180deg, #ffffff 0%, #fbfdff 100%);
}

.timeline-date {
  color: var(--accent);
  font-weight: 700;
  font-size: 0.84rem;
}

.timeline-text {
  color: var(--muted);
}

.award-grid {
  display: grid;
  grid-template-columns: repeat(2, minmax(0, 1fr));
  gap: 12px;
}

.award-card {
  border: 1px solid var(--line);
  border-radius: 14px;
  padding: 0.95rem;
  background: linear-gradient(180deg, #fffdf8 0%, #ffffff 100%);
}

.award-year {
  color: var(--accent-2);
  font-weight: 700;
  font-size: 0.82rem;
}

.award-text {
  margin-top: 0.25rem;
  color: var(--ink);
}

.map-box {
  border: 1px dashed var(--line);
  border-radius: 14px;
  padding: 1rem;
  background: linear-gradient(180deg, #fbfdff 0%, #f5f9fc 100%);
}

.map-note {
  margin: 0 0 0.8rem;
  color: var(--muted);
  font-size: 0.9rem;
}

@media (max-width: 900px) {
  .fact-grid,
  .interest-grid,
  .award-grid {
    grid-template-columns: 1fr;
  }

  .timeline-item {
    grid-template-columns: 1fr;
  }
}
</style>

<div class="home-wrap">
  <section class="hero-panel">
    <p class="eyebrow">Academic Profile</p>
    <h1 class="hero-name">Juntao (Jason) Chen</h1>
    <p class="hero-lead">MPhil candidate in the School of Mathematics, Statistics and Physics at Newcastle University, supervised by <a href="https://www.ncl.ac.uk/maths-physics/people/profile/chrisoates.html">Prof. Chris Oates</a>.</p>
    <p class="hero-text">I work at the intersection of probabilistic machine learning, computational statistics, and deep learning, with a focus on principled and uncertainty-aware methods for real-world problems.</p>

    <div class="tag-row">
      <span class="tag">Probabilistic ML</span>
      <span class="tag">Computational Statistics</span>
      <span class="tag">Deep Learning</span>
      <span class="tag">Uncertainty Quantification</span>
    </div>

    <div class="fact-grid">
      <div class="fact-card">
        <div class="fact-label">Current Base</div>
        <div class="fact-value">Newcastle upon Tyne, UK</div>
      </div>
      <div class="fact-card">
        <div class="fact-label">Research Style</div>
        <div class="fact-value">Theory-informed, application-aware</div>
      </div>
      <div class="fact-card">
        <div class="fact-label">Current Themes</div>
        <div class="fact-value">Bayesian methods, Monte Carlo, structured deep models</div>
      </div>
    </div>
  </section>

  <section class="section-block">
    <h2 class="section-title"><span class="section-icon">01</span>Research Interests</h2>
    <div class="interest-grid">
      <article class="interest-card">
        <div class="interest-num">Focus A</div>
        <h3>Probabilistic Machine Learning</h3>
        <p>Bayesian inference, uncertainty quantification, and reliable predictive modeling.</p>
      </article>
      <article class="interest-card">
        <div class="interest-num">Focus B</div>
        <h3>Computational Statistics</h3>
        <p>Monte Carlo methods, statistical learning theory, and modern discrepancy tools.</p>
      </article>
      <article class="interest-card">
        <div class="interest-num">Focus C</div>
        <h3>Deep Learning</h3>
        <p>Sequence modeling, graph neural networks, and transformer-based architectures.</p>
      </article>
    </div>
  </section>

  <section class="section-block">
    <h2 class="section-title"><span class="section-icon">02</span>Recent News</h2>
    <div class="timeline">
      <div class="timeline-item">
        <div class="timeline-date">Jan 2025</div>
        <div class="timeline-text">Paper accepted at <em>Scientific Reports</em>: CoGraphNet for enhanced text classification.</div>
      </div>
      <div class="timeline-item">
        <div class="timeline-date">Nov 2024</div>
        <div class="timeline-text">Paper published in <em>Energy</em>: offshore wind power prediction with TCN-DANet-Sparse Transformer.</div>
      </div>
    </div>
  </section>

  <section class="section-block">
    <h2 class="section-title"><span class="section-icon">03</span>Selected Awards</h2>
    <div class="award-grid">
      <article class="award-card">
        <div class="award-year">2023</div>
        <div class="award-text">International Mathematical Contest in Modeling (MCM/ICM) - <strong>Meritorious Winner</strong></div>
      </article>
      <article class="award-card">
        <div class="award-year">2023</div>
        <div class="award-text">National College Student Mathematical Modeling Competition (CUMCM) - <strong>Second Prize</strong></div>
      </article>
      <article class="award-card">
        <div class="award-year">2022 &amp; 2023</div>
        <div class="award-text">National College Student Statistical Modeling Competition - <strong>Second Prize</strong></div>
      </article>
      <article class="award-card">
        <div class="award-year">2021-2023</div>
        <div class="award-text">University-level Special Scholarship and Department First-Class Scholarship for three consecutive years.</div>
      </article>
    </div>
  </section>

  <section class="section-block">
    <h2 class="section-title"><span class="section-icon">04</span>Visitor Map</h2>
    <div class="map-box">
      <p class="map-note">A small trace of where visitors come from. It adds a quiet travelogue feel to the homepage.</p>
      <div style="text-align: center; margin-top: 0.4rem;">
        <script type="text/javascript" id="mmvst_globe" src="//mapmyvisitors.com/globe.js?d=JaAvWtEeczc9P-6tKzPgSbuvHFP5j7m3PltnLpLiPT8"></script>
      </div>
    </div>
  </section>
</div>
