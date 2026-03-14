---
layout: single
title: "Chongqing at Night"
permalink: /travel/chongqing-night/
author_profile: true
---

<style>
.trip-page {
	--ink: #1f2937;
	--muted: #5f6b78;
	--line: #dbe3ea;
	--accent: #0f766e;
	--warm: #b45309;
	background:
		radial-gradient(circle at top right, rgba(15, 118, 110, 0.12), transparent 22%),
		radial-gradient(circle at bottom left, rgba(180, 83, 9, 0.08), transparent 24%),
		linear-gradient(180deg, #f8fbfd 0%, #ffffff 62%);
	border: 1px solid var(--line);
	border-radius: 22px;
	padding: 1.3rem;
	box-shadow: 0 18px 40px rgba(15, 23, 42, 0.08);
}

.trip-hero {
	position: relative;
	border-radius: 18px;
	overflow: hidden;
	border: 1px solid var(--line);
	box-shadow: 0 14px 30px rgba(15, 23, 42, 0.16);
}

.trip-hero-link,
.mini-gallery a {
	display: block;
	text-decoration: none;
	color: inherit;
}

.lightbox-trigger {
	padding: 0;
	margin: 0;
	border: 0;
	background: transparent;
	width: 100%;
	cursor: zoom-in;
	text-align: left;
}

.trip-hero img {
	display: block;
	width: 100%;
	max-height: 480px;
	object-fit: cover;
	transition: transform 0.2s ease;
}

.trip-hero-link:hover img,
.mini-gallery a:hover img {
	transform: scale(1.02);
}

.lightbox-trigger:hover img {
	transform: scale(1.02);
}

.trip-hero-note {
	position: absolute;
	left: 0.75rem;
	bottom: 0.75rem;
	color: #f9fbfd;
	background: rgba(15, 23, 42, 0.62);
	border: 1px solid rgba(255, 255, 255, 0.3);
	border-radius: 8px;
	padding: 0.42rem 0.56rem;
	font-size: 0.82rem;
	backdrop-filter: blur(2px);
}

.trip-zoom-note {
	position: absolute;
	right: 0.75rem;
	bottom: 0.75rem;
	color: #f9fbfd;
	background: rgba(15, 23, 42, 0.62);
	border: 1px solid rgba(255, 255, 255, 0.3);
	border-radius: 8px;
	padding: 0.42rem 0.56rem;
	font-size: 0.78rem;
	backdrop-filter: blur(2px);
}

.trip-headline {
	margin: 0.95rem 0 0;
	display: grid;
	grid-template-columns: 1.1fr 0.9fr;
	gap: 14px;
}

.trip-intro,
.trip-quote {
	border: 1px solid var(--line);
	border-radius: 16px;
	padding: 1rem;
	background: rgba(255, 255, 255, 0.88);
}

.trip-kicker {
	margin: 0;
	color: var(--accent);
	text-transform: uppercase;
	letter-spacing: 0.12em;
	font-size: 0.74rem;
	font-weight: 700;
}

.trip-intro h2,
.trip-quote h2 {
	margin: 0.35rem 0 0;
	color: var(--ink);
	font-size: 1.15rem;
}

.trip-intro p,
.trip-quote p {
	margin: 0.6rem 0 0;
	color: var(--muted);
}

.trip-quote {
	background: linear-gradient(180deg, #fffdf7 0%, #ffffff 100%);
}

.trip-quote-mark {
	color: var(--warm);
	font-size: 1.8rem;
	line-height: 1;
}

.trip-grid {
	margin-top: 1rem;
	display: grid;
	grid-template-columns: 1.3fr 1fr;
	gap: 14px;
}

.trip-panel {
	border: 1px solid var(--line);
	border-radius: 12px;
	background: #fff;
	padding: 0.95rem;
}

.trip-panel h2 {
	margin: 0 0 0.6rem;
	color: var(--ink);
	font-size: 1.07rem;
}

.trip-panel p,
.trip-panel li {
	color: var(--muted);
}

.coord {
	font-family: "JetBrains Mono", "SFMono-Regular", Menlo, Consolas, monospace;
	color: #4b5563;
	font-size: 0.84rem;
}

.mini-gallery {
	margin-top: 1rem;
	display: grid;
	grid-template-columns: repeat(3, minmax(0, 1fr));
	gap: 10px;
}

.mini-gallery-title {
	margin: 1.15rem 0 0.7rem;
	color: var(--ink);
	font-size: 1rem;
}

.mini-gallery figure {
	margin: 0;
	border: 1px solid var(--line);
	border-radius: 10px;
	overflow: hidden;
	background: #fff;
}

.mini-gallery img {
	width: 100%;
	height: 150px;
	object-fit: cover;
	display: block;
}

.mini-gallery figcaption {
	font-size: 0.76rem;
	color: #66727f;
	padding: 0.42rem 0.5rem;
}

.travel-details {
	margin-top: 1rem;
	display: grid;
	grid-template-columns: repeat(3, minmax(0, 1fr));
	gap: 10px;
}

.detail-card {
	border: 1px solid var(--line);
	border-radius: 12px;
	padding: 0.85rem;
	background: linear-gradient(180deg, #ffffff 0%, #f8fbfd 100%);
}

.detail-card strong {
	display: block;
	color: var(--ink);
	margin-bottom: 0.28rem;
}

.detail-card span {
	color: var(--muted);
	font-size: 0.9rem;
}

.lightbox {
	position: fixed;
	inset: 0;
	z-index: 9999;
	display: none;
	align-items: center;
	justify-content: center;
	padding: 2rem;
	background: rgba(15, 23, 42, 0.82);
	backdrop-filter: blur(6px);
}

.lightbox.is-open {
	display: flex;
}

.lightbox-backdrop {
	position: absolute;
	inset: 0;
	border: 0;
	background: transparent;
	cursor: zoom-out;
}

.lightbox-panel {
	position: relative;
	z-index: 1;
	max-width: min(1100px, 92vw);
	max-height: 88vh;
	width: auto;
}

.lightbox-image {
	display: block;
	max-width: 100%;
	max-height: 78vh;
	border-radius: 14px;
	box-shadow: 0 20px 50px rgba(0, 0, 0, 0.35);
	background: #fff;
}

.lightbox-close {
	position: absolute;
	top: -0.8rem;
	right: -0.8rem;
	width: 40px;
	height: 40px;
	border: 0;
	border-radius: 999px;
	background: rgba(255, 255, 255, 0.96);
	color: #0f172a;
	font-size: 1.2rem;
	cursor: pointer;
	box-shadow: 0 8px 24px rgba(0, 0, 0, 0.2);
}

.lightbox-caption {
	margin-top: 0.75rem;
	text-align: center;
	color: #e2e8f0;
	font-size: 0.92rem;
}

.journal {
	margin-top: 1rem;
	border-left: 3px solid var(--accent);
	padding-left: 0.9rem;
}

.credit {
	margin-top: 1rem;
	padding: 0.7rem 0.8rem;
	border: 1px dashed var(--line);
	border-radius: 10px;
	font-size: 0.85rem;
	color: #687484;
	background: #f8fbfd;
}

@media (max-width: 900px) {
	.trip-headline,
	.trip-grid {
		grid-template-columns: 1fr;
	}

	.travel-details,
	.mini-gallery {
		grid-template-columns: 1fr;
	}

	.lightbox {
		padding: 1rem;
	}

	.lightbox-close {
		top: -0.5rem;
		right: -0.2rem;
	}
}
</style>

<div class="trip-page">
	<div class="trip-hero">
		<button class="trip-hero-link lightbox-trigger" type="button" data-full="https://upload.wikimedia.org/wikipedia/commons/f/f5/Chongqing_Skyline_At_Night.png" data-caption="Chongqing skyline at night">
			<img src="https://upload.wikimedia.org/wikipedia/commons/thumb/f/f5/Chongqing_Skyline_At_Night.png/1920px-Chongqing_Skyline_At_Night.png" alt="Chongqing skyline at night">
		</button>
		<div class="trip-hero-note">Chongqing, China | Night walk by the river</div>
		<div class="trip-zoom-note">Click image to enlarge</div>
	</div>

	<div class="trip-headline">
		<section class="trip-intro">
			<p class="trip-kicker">Travel Story</p>
			<h2>Light, density, and a city that seems to rise straight out of the river.</h2>
			<p>This page is meant to feel more personal than a postcard. It is not only about where the photo was taken, but also about what the place felt like in motion: the sound of water, the weight of humidity, and the sense of scale that only appears at night.</p>
		</section>
		<aside class="trip-quote">
			<div class="trip-quote-mark">"</div>
			<h2>A sentence for the page</h2>
			<p>Some cities impress you with size. Chongqing stays with you because it turns complexity into atmosphere.</p>
		</aside>
	</div>

	<div class="trip-grid">
		<section class="trip-panel">
			<h2>Place Notes</h2>
			<ul>
				<li>City: Chongqing, China</li>
				<li>Coordinates: <span class="coord">29.5630 N, 106.5516 E</span></li>
				<li>Scene: River skyline and bridge lights at night</li>
			</ul>
			<p>
				The city looks cinematic from the river. Layers of bridges, dense towers,
				and neon reflections make every frame feel alive.
			</p>
		</section>

		<section class="trip-panel">
			<h2>My Reflection</h2>
			<p>
				This night view reminds me that complex systems are beautiful not because
				they are simple, but because they remain coherent in motion.
			</p>
			<p>
				There is noise, uncertainty, and asymmetry everywhere, yet a structure
				still emerges. That is exactly the feeling I have when doing research.
			</p>
			<div class="journal">
				<strong>One sentence I keep:</strong>
				<p>"Clarity is not the absence of complexity, but a way through it."</p>
			</div>
		</section>
	</div>

	<div class="travel-details">
		<div class="detail-card">
			<strong>Mood</strong>
			<span>Cinematic, humid, layered, electric</span>
		</div>
		<div class="detail-card">
			<strong>Best Moment</strong>
			<span>When bridge lights begin reflecting on the river surface</span>
		</div>
		<div class="detail-card">
			<strong>Memory Trigger</strong>
			<span>The contrast between heavy skyline density and flowing water</span>
		</div>
	</div>

	<h2 class="mini-gallery-title">More Photos</h2>
	<div class="mini-gallery">
		<figure>
			<button class="lightbox-trigger" type="button" data-full="https://upload.wikimedia.org/wikipedia/commons/f/f5/Chongqing_Skyline_At_Night.png" data-caption="Main skyline view">
				<img src="https://upload.wikimedia.org/wikipedia/commons/thumb/f/f5/Chongqing_Skyline_At_Night.png/1280px-Chongqing_Skyline_At_Night.png" alt="Chongqing skyline at night">
			</button>
			<figcaption>Main skyline view</figcaption>
		</figure>
		<figure>
			<button class="lightbox-trigger" type="button" data-full="https://upload.wikimedia.org/wikipedia/commons/d/d4/Chongqing_center.jpg" data-caption="City center panorama">
				<img src="https://upload.wikimedia.org/wikipedia/commons/thumb/d/d4/Chongqing_center.jpg/1280px-Chongqing_center.jpg" alt="Chongqing center skyline">
			</button>
			<figcaption>City center panorama</figcaption>
		</figure>
		<figure>
			<button class="lightbox-trigger" type="button" data-full="https://upload.wikimedia.org/wikipedia/commons/b/b2/Raffles_City_Chongqing_from_Yangtze_River.jpg" data-caption="Riverside architecture and movement">
				<img src="https://upload.wikimedia.org/wikipedia/commons/thumb/b/b2/Raffles_City_Chongqing_from_Yangtze_River.jpg/1280px-Raffles_City_Chongqing_from_Yangtze_River.jpg" alt="Raffles City Chongqing from Yangtze River">
			</button>
			<figcaption>Riverside architecture and movement</figcaption>
		</figure>
	</div>

</div>

<div class="lightbox" id="travel-lightbox" aria-hidden="true">
	<button class="lightbox-backdrop" type="button" aria-label="Close enlarged image"></button>
	<div class="lightbox-panel" role="dialog" aria-modal="true" aria-label="Enlarged travel photo">
		<button class="lightbox-close" type="button" aria-label="Close enlarged image">×</button>
		<img class="lightbox-image" src="" alt="">
		<div class="lightbox-caption"></div>
	</div>
</div>

<script>
	(function () {
		var lightbox = document.getElementById('travel-lightbox');
		if (!lightbox) return;

		var image = lightbox.querySelector('.lightbox-image');
		var caption = lightbox.querySelector('.lightbox-caption');
		var closeButton = lightbox.querySelector('.lightbox-close');
		var backdrop = lightbox.querySelector('.lightbox-backdrop');
		var triggers = document.querySelectorAll('.lightbox-trigger');

		function openLightbox(src, alt, text) {
			image.src = src;
			image.alt = alt || text || 'Travel photo';
			caption.textContent = text || '';
			lightbox.classList.add('is-open');
			lightbox.setAttribute('aria-hidden', 'false');
			document.body.style.overflow = 'hidden';
		}

		function closeLightbox() {
			lightbox.classList.remove('is-open');
			lightbox.setAttribute('aria-hidden', 'true');
			image.src = '';
			document.body.style.overflow = '';
		}

		triggers.forEach(function (trigger) {
			trigger.addEventListener('click', function () {
				var img = trigger.querySelector('img');
				openLightbox(trigger.getAttribute('data-full'), img ? img.alt : '', trigger.getAttribute('data-caption'));
			});
		});

		closeButton.addEventListener('click', closeLightbox);
		backdrop.addEventListener('click', closeLightbox);
		document.addEventListener('keydown', function (event) {
			if (event.key === 'Escape' && lightbox.classList.contains('is-open')) {
				closeLightbox();
			}
		});
	})();
</script>
