---
layout: archive
title: "Gallery"
permalink: /gallery/
author_profile: true
---

<style>
.travel-wrap {
  --ink: #1f2a36;
  --muted: #6b7785;
  --line: #dbe4eb;
  --accent: #0e7490;
  --card: #ffffff;
  background: linear-gradient(180deg, #f5f8fb 0%, #ffffff 55%);
  border: 1px solid var(--line);
  border-radius: 16px;
  padding: 1.4rem;
  margin: 0.5rem 0 1.6rem;
}

.travel-intro {
  color: var(--muted);
  margin: 0.35rem 0 0;
  font-size: 1rem;
}

.gallery-section {
  margin-top: 1.8rem;
}

.section-title {
  display: flex;
  align-items: center;
  gap: 0.5rem;
  font-size: 1.18rem;
  color: var(--ink);
  margin: 0 0 0.8rem;
  padding-bottom: 0.45rem;
  border-bottom: 2px solid var(--accent);
}

.photo-grid {
  display: grid;
  grid-template-columns: repeat(auto-fit, minmax(260px, 320px));
  gap: 14px;
}

.story-card {
  text-decoration: none;
  color: inherit;
  background: var(--card);
  border: 1px solid var(--line);
  border-radius: 12px;
  overflow: hidden;
  box-shadow: 0 8px 22px rgba(15, 23, 42, 0.08);
  transition: transform 0.18s ease, box-shadow 0.18s ease;
}

.story-card:hover {
  transform: translateY(-4px);
  box-shadow: 0 14px 30px rgba(15, 23, 42, 0.14);
}

.story-card img {
  width: 100%;
  height: 210px;
  object-fit: cover;
  display: block;
}

.story-body {
  padding: 0.72rem 0.8rem 0.86rem;
}

.story-title {
  font-size: 1.02rem;
  font-weight: 700;
  color: var(--ink);
  margin: 0;
}

.story-meta {
  margin-top: 0.28rem;
  font-family: "JetBrains Mono", "SFMono-Regular", Menlo, Consolas, monospace;
  font-size: 0.76rem;
  color: #5b6775;
}

.story-note {
  margin-top: 0.35rem;
  color: var(--muted);
  font-size: 0.86rem;
}

.empty-box {
  border: 1px dashed var(--line);
  border-radius: 10px;
  padding: 0.9rem;
  color: #8a95a2;
  font-size: 0.9rem;
  background: #fcfdff;
}

.credit-line {
  color: #8391a0;
  font-size: 0.84rem;
  margin-top: 1.5rem;
  text-align: center;
}

@media (max-width: 640px) {
  .travel-wrap {
    padding: 1rem;
  }

  .photo-grid {
    grid-template-columns: 1fr;
  }
}
</style>

<div class="travel-wrap">
<p class="travel-intro">Life beyond research - moments from travels, city walks, and personal reflections.</p>

---

<div class="gallery-section">
<h2 class="section-title">GB United Kingdom</h2>
<div class="photo-grid">
<div class="empty-box">No story yet. Add your UK travel story card here.</div>

</div>
</div>

<div class="gallery-section">
<h2 class="section-title">CN China</h2>
<div class="photo-grid">

<a class="story-card" href="/travel/chongqing-night/">
  <img src="https://upload.wikimedia.org/wikipedia/commons/thumb/f/f5/Chongqing_Skyline_At_Night.png/1280px-Chongqing_Skyline_At_Night.png" alt="Chongqing skyline at night">
  <div class="story-body">
    <p class="story-title">Chongqing, China</p>
    <div class="story-meta">29.5630 N, 106.5516 E</div>
    <div class="story-note">Night skyline diary, river walk, and personal reflections.</div>
  </div>
</a>

</div>
</div>

<div class="gallery-section">
<h2 class="section-title">Elsewhere</h2>
<div class="photo-grid">
<div class="empty-box">More destinations coming soon.</div>

</div>
</div>

<p class="credit-line">
  Photo source for Chongqing card: Wikimedia Commons (CC BY-SA 4.0, Maple Doctor)
</p>
</div>
