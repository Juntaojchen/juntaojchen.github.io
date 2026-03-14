---
layout: archive
title: "Gallery"
permalink: /gallery/
author_profile: true
---

<style>
.travel-wrap {
  --ink: #1e2937;
  --muted: #647282;
  --line: #d7e2ea;
  --accent: #0f766e;
  --accent-soft: #f2fbf8;
  --warm: #b45309;
  --card: #ffffff;
  position: relative;
  overflow: hidden;
  background:
    radial-gradient(circle at top right, rgba(15, 118, 110, 0.14), transparent 24%),
    radial-gradient(circle at left bottom, rgba(180, 83, 9, 0.08), transparent 24%),
    linear-gradient(180deg, #f7fafc 0%, #ffffff 58%);
  border: 1px solid var(--line);
  border-radius: 22px;
  padding: 1.5rem;
  margin: 0.45rem 0 1.8rem;
  box-shadow: 0 18px 40px rgba(15, 23, 42, 0.08);
}

.travel-wrap::after {
  content: "";
  position: absolute;
  top: -30px;
  right: -40px;
  width: 180px;
  height: 180px;
  border: 1px solid rgba(15, 118, 110, 0.1);
  border-radius: 999px;
}

.gallery-hero {
  display: grid;
  grid-template-columns: 1.05fr 0.95fr;
  gap: 16px;
  align-items: stretch;
}

.hero-copy {
  padding: 0.2rem 0.2rem 0 0;
}

.eyebrow {
  margin: 0;
  color: var(--accent);
  text-transform: uppercase;
  letter-spacing: 0.14em;
  font-size: 0.74rem;
  font-weight: 700;
}

.travel-title {
  margin: 0.35rem 0 0;
  color: var(--ink);
  font-size: 2rem;
  line-height: 1.06;
}

.travel-intro {
  color: var(--muted);
  margin: 0.7rem 0 0;
  font-size: 1rem;
  max-width: 560px;
}

.micro-row {
  display: flex;
  flex-wrap: wrap;
  gap: 0.55rem;
  margin-top: 1rem;
}

.micro-pill {
  display: inline-flex;
  align-items: center;
  gap: 0.4rem;
  padding: 0.42rem 0.7rem;
  border-radius: 999px;
  border: 1px solid var(--line);
  background: rgba(255, 255, 255, 0.8);
  color: #344454;
  font-size: 0.83rem;
}

.hero-note-card {
  border: 1px solid var(--line);
  border-radius: 18px;
  padding: 1rem;
  background: linear-gradient(180deg, rgba(255,255,255,0.95) 0%, rgba(242,251,248,0.9) 100%);
}

.note-kicker {
  color: var(--warm);
  font-size: 0.76rem;
  text-transform: uppercase;
  letter-spacing: 0.12em;
  font-weight: 700;
}

.note-title {
  margin: 0.45rem 0 0;
  color: var(--ink);
  font-size: 1.08rem;
}

.note-text {
  margin: 0.55rem 0 0;
  color: var(--muted);
  font-size: 0.92rem;
}

.note-list {
  margin: 0.9rem 0 0;
  padding: 0;
  list-style: none;
}

.note-list li {
  color: #506072;
  margin-top: 0.4rem;
}

.gallery-section {
  margin-top: 2rem;
}

.section-title {
  display: flex;
  align-items: center;
  justify-content: space-between;
  gap: 0.8rem;
  font-size: 1.18rem;
  color: var(--ink);
  margin: 0 0 0.8rem;
  padding-bottom: 0.65rem;
  border-bottom: 1px solid var(--line);
}

.section-title strong {
  display: flex;
  align-items: center;
  gap: 0.48rem;
}

.section-title span {
  color: var(--muted);
  font-size: 0.84rem;
}

.photo-grid {
  display: grid;
  grid-template-columns: repeat(2, minmax(0, 1fr));
  gap: 16px;
}

.featured-story {
  display: grid;
  grid-template-columns: 1.05fr 0.95fr;
  min-height: 330px;
  text-decoration: none;
  color: inherit;
  border: 1px solid var(--line);
  border-radius: 18px;
  overflow: hidden;
  background: var(--card);
  box-shadow: 0 16px 30px rgba(15, 23, 42, 0.1);
  transition: transform 0.2s ease, box-shadow 0.2s ease;
}

.featured-story:hover,
.story-card:hover {
  transform: translateY(-4px);
  box-shadow: 0 20px 34px rgba(15, 23, 42, 0.14);
}

.featured-media {
  position: relative;
}

.featured-media img {
  width: 100%;
  height: 100%;
  min-height: 330px;
  object-fit: cover;
  display: block;
}

.featured-stamp {
  position: absolute;
  left: 1rem;
  top: 1rem;
  padding: 0.38rem 0.62rem;
  border-radius: 999px;
  color: #f8fafc;
  background: rgba(15, 23, 42, 0.62);
  border: 1px solid rgba(255, 255, 255, 0.26);
  font-size: 0.76rem;
  letter-spacing: 0.08em;
  text-transform: uppercase;
}

.featured-body {
  display: flex;
  flex-direction: column;
  justify-content: space-between;
  padding: 1.1rem;
}

.story-card {
  text-decoration: none;
  color: inherit;
  background: var(--card);
  border: 1px solid var(--line);
  border-radius: 14px;
  overflow: hidden;
  box-shadow: 0 10px 22px rgba(15, 23, 42, 0.07);
  transition: transform 0.18s ease, box-shadow 0.18s ease;
}

.story-card img {
  width: 100%;
  height: 210px;
  object-fit: cover;
  display: block;
}

.story-body {
  padding: 0.9rem;
}

.story-title {
  font-size: 1.08rem;
  font-weight: 700;
  color: var(--ink);
  margin: 0;
}

.story-meta {
  margin-top: 0.34rem;
  font-family: "JetBrains Mono", "SFMono-Regular", Menlo, Consolas, monospace;
  font-size: 0.76rem;
  color: #5b6775;
}

.story-note {
  margin-top: 0.48rem;
  color: var(--muted);
  font-size: 0.86rem;
}

.story-cta {
  margin-top: 0.8rem;
  color: var(--accent);
  font-size: 0.82rem;
  font-weight: 700;
  letter-spacing: 0.06em;
  text-transform: uppercase;
}

.empty-box {
  border: 1px dashed var(--line);
  border-radius: 14px;
  padding: 1rem;
  color: #8090a0;
  font-size: 0.9rem;
  background: linear-gradient(180deg, #fcfdff 0%, #f7fafc 100%);
}

.credit-line {
  color: #8391a0;
  font-size: 0.84rem;
  margin-top: 1.7rem;
  text-align: center;
}

@media (max-width: 900px) {
  .gallery-hero,
  .featured-story,
  .photo-grid {
    grid-template-columns: 1fr;
  }

  .featured-media img {
    min-height: 240px;
  }
}

@media (max-width: 640px) {
  .travel-wrap {
    padding: 1rem;
  }

  .travel-title {
    font-size: 1.65rem;
  }
}
</style>

<div class="travel-wrap">
<div class="gallery-hero">
  <div class="hero-copy">
    <p class="eyebrow">Travel Notes</p>
    <h2 class="travel-title">A softer archive of cities, light, weather, and memory.</h2>
    <p class="travel-intro">Beyond research, this page collects travel fragments: places that stayed in mind, small observations, and the kind of sentences worth keeping after the trip ends.</p>
    <div class="micro-row">
      <span class="micro-pill">◦ city walks</span>
      <span class="micro-pill">◦ night views</span>
      <span class="micro-pill">◦ reflections</span>
    </div>
  </div>
  <aside class="hero-note-card">
    <div class="note-kicker">Curator's Note</div>
    <h3 class="note-title">Each image opens into a story page.</h3>
    <p class="note-text">Instead of sending visitors to an external image source, each card leads to your own page with more photos, place notes, and personal reflections.</p>
    <ul class="note-list">
      <li>✦ More than one photo</li>
      <li>✦ Short travel writing</li>
      <li>✦ Mood, memory, and context</li>
    </ul>
  </aside>
</div>

<div class="gallery-section">
<h2 class="section-title"><strong>GB United Kingdom</strong><span>Future city stories</span></h2>
<div class="photo-grid">
<div class="empty-box">No story yet. Add your UK travel story card here.</div>
<div class="empty-box">A second card could be Newcastle, Edinburgh, or London.</div>

</div>
</div>

<div class="gallery-section">
<h2 class="section-title"><strong>CN China</strong><span>Featured story</span></h2>
<div class="photo-grid">

<a class="featured-story" href="/travel/chongqing-night/">
  <div class="featured-media">
    <img src="https://upload.wikimedia.org/wikipedia/commons/thumb/f/f5/Chongqing_Skyline_At_Night.png/1280px-Chongqing_Skyline_At_Night.png" alt="Chongqing skyline at night">
    <div class="featured-stamp">Featured</div>
  </div>
  <div class="featured-body">
    <div>
      <p class="story-title">Chongqing, China</p>
      <div class="story-meta">29.5630 N, 106.5516 E</div>
      <div class="story-note">A night skyline shaped by bridges, river light, and a dense vertical rhythm that feels both cinematic and intimate.</div>
    </div>
    <div class="story-cta">Open story ↗</div>
  </div>
</a>

</div>
</div>

<div class="gallery-section">
<h2 class="section-title"><strong>Elsewhere</strong><span>More destinations soon</span></h2>
<div class="photo-grid">
<div class="empty-box">More destinations coming soon.</div>
<div class="empty-box">This area works well for short essays from future trips.</div>

</div>
</div>

</div>
