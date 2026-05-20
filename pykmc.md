---
layout: default
title: "PyKMC"
permalink: /pykmc/
description: "Companion page for the PyKMC poster — full showreel and per-event animations (init / saddle / final stills) for the four elementary surface events in Ni–Cr–Al kinetic Monte Carlo."
---

<style>
.pykmc-page { max-width: 760px; margin: 0 auto; }

.pykmc-hero {
  padding: 1.5rem 0 1rem 0;
  border-bottom: 1px solid var(--border-subtle);
  margin-bottom: 1.5rem;
}
.pykmc-hero h1 { margin-top: 0; }
.pykmc-hero .tagline {
  color: var(--text-muted);
  font-size: 1.05rem;
}

.pykmc-toc {
  background-color: var(--bg-card);
  border: 1px solid var(--border-subtle);
  border-radius: 8px;
  padding: 1rem 1.25rem;
  margin-bottom: 2rem;
}
.pykmc-toc strong {
  color: var(--text-heading);
  display: block;
  margin-bottom: 0.5rem;
  font-weight: 600;
}
.pykmc-toc ol { margin: 0; padding-left: 1.25rem; }
.pykmc-toc li { margin-bottom: 0.25rem; }

.pykmc-section {
  scroll-margin-top: 1rem;
  padding-top: 1rem;
  margin-bottom: 2.5rem;
  border-top: 1px solid var(--border-subtle);
}
.pykmc-section h2 { margin-top: 0.5rem; }
.pykmc-section .event-meta {
  color: var(--text-muted);
  font-size: 0.9rem;
  margin-top: -0.25rem;
}

.video-embed {
  position: relative;
  width: 100%;
  padding-bottom: 56.25%;
  margin: 1rem 0;
  border-radius: 8px;
  overflow: hidden;
  border: 1px solid var(--border-subtle);
  background-color: var(--bg-card);
}
.video-embed iframe {
  position: absolute;
  top: 0;
  left: 0;
  width: 100%;
  height: 100%;
  border: 0;
}

.event-stills {
  display: grid;
  grid-template-columns: repeat(3, 1fr);
  gap: 0.75rem;
  margin-top: 1rem;
}
.event-still {
  display: flex;
  flex-direction: column;
  align-items: stretch;
  background-color: var(--bg-card);
  border: 1px solid var(--border-subtle);
  border-radius: 6px;
  overflow: hidden;
}
.event-still img {
  width: 100%;
  height: auto;
  display: block;
}
.event-still .caption {
  padding: 0.4rem 0.5rem;
  font-size: 0.85rem;
  color: var(--text-muted);
  text-align: center;
  border-top: 1px solid var(--border-subtle);
  background-color: var(--bg-elev);
}
.event-still .caption strong {
  color: var(--text-heading);
  font-weight: 600;
}

@media (max-width: 600px) {
  .event-stills {
    grid-template-columns: 1fr;
  }
}

.pykmc-resources {
  margin-top: 2.5rem;
  padding: 1rem 1.25rem;
  background-color: var(--bg-card);
  border: 1px solid var(--border-subtle);
  border-radius: 8px;
}
.pykmc-resources h2 {
  margin-top: 0;
  font-size: 1.15rem;
}
.pykmc-resources ul {
  margin: 0.5rem 0 0 0;
  padding-left: 1.25rem;
}
</style>

<!-- Open Graph / Facebook -->
<meta property="og:type" content="article">
<meta property="og:url" content="https://www.winteratomics.ca/pykmc/">
<meta property="og:title" content="PyKMC — Stephen Kerr">
<meta property="og:description" content="Companion page for the PyKMC poster — full showreel and per-event animations of the four elementary surface events in Ni–Cr–Al kinetic Monte Carlo.">
<meta property="og:image" content="https://www.winteratomics.ca/assets/images/graphical-abstract-cr-vacancy.png">

<!-- Twitter -->
<meta name="twitter:card" content="summary_large_image">
<meta name="twitter:url" content="https://www.winteratomics.ca/pykmc/">
<meta name="twitter:title" content="PyKMC — Stephen Kerr">
<meta name="twitter:description" content="Companion page for the PyKMC poster — full showreel and per-event animations of the four elementary surface events in Ni–Cr–Al kinetic Monte Carlo.">
<meta name="twitter:image" content="https://www.winteratomics.ca/assets/images/graphical-abstract-cr-vacancy.png">

<div class="pykmc-page">

  <div class="pykmc-hero">
    <h1>PyKMC</h1>
    <p class="tagline">Companion page for the PyKMC poster — full simulation showreel up top, then per-event animations and init / saddle / final stills for the four elementary surface events covered on the poster.</p>
  </div>

  <section id="showreel" class="pykmc-section" style="border-top: none; padding-top: 0;">
    <h2>Full showreel</h2>
    <p>End-to-end render of a representative PyKMC trajectory in Ni–Cr–Al: vacancy diffusion, surface ↔ subsurface exchange, and 1NN in-plane hops, sequenced in the order they occurred during the run.</p>
    <div class="video-embed">
      <iframe src="https://www.youtube.com/embed/ATy5YVhzN2s" title="PyKMC full showreel — Ni–Cr–Al kinetic Monte Carlo" allow="accelerometer; clipboard-write; encrypted-media; picture-in-picture" allowfullscreen loading="lazy"></iframe>
    </div>
  </section>

  <nav class="pykmc-toc" aria-label="On this page">
    <strong>Elementary events on this page</strong>
    <ol>
      <li><a href="#event-1">Surface ↔ subsurface exchange (downward)</a></li>
      <li><a href="#event-2">Surface 1NN in-plane (atom 3975)</a></li>
      <li><a href="#event-3">Surface 1NN in-plane (atom 2023)</a></li>
      <li><a href="#event-4">Surface ↔ subsurface exchange (upward, atom 3234)</a></li>
    </ol>
  </nav>

  <section id="event-1" class="pykmc-section">
    <h2>Event 1 — Surface ↔ subsurface exchange (downward)</h2>
    <p class="event-meta">Surface atom hops into a subsurface vacancy. Sets the downstream availability of vacancies for the in-plane events.</p>
    <p>An atom on the surface layer swaps with the subsurface vacancy directly below it. This event transports a vacancy upward to the surface while moving a surface atom into the bulk — the first ingredient in the chromium-driven enhancement of bulk vacancy concentration.</p>
    <div class="video-embed">
      <iframe src="https://www.youtube.com/embed/a5MsdIsdSnA" title="Event 1 — surface ↔ subsurface exchange (downward)" allow="accelerometer; clipboard-write; encrypted-media; picture-in-picture" allowfullscreen loading="lazy"></iframe>
    </div>
    <div class="event-stills" aria-label="Event 1 stills">
      <figure class="event-still">
        <img src="/assets/images/pykmc-e1-init.jpg" alt="Event 1 — initial state" loading="lazy">
        <figcaption class="caption"><strong>Initial</strong></figcaption>
      </figure>
      <figure class="event-still">
        <img src="/assets/images/pykmc-e1-saddle.jpg" alt="Event 1 — saddle point" loading="lazy">
        <figcaption class="caption"><strong>Saddle</strong></figcaption>
      </figure>
      <figure class="event-still">
        <img src="/assets/images/pykmc-e1-final.jpg" alt="Event 1 — final state" loading="lazy">
        <figcaption class="caption"><strong>Final</strong></figcaption>
      </figure>
    </div>
  </section>

  <section id="event-2" class="pykmc-section">
    <h2>Event 2 — Surface 1NN in-plane (atom 3975)</h2>
    <p class="event-meta">First-nearest-neighbour hop in the surface plane. Atom index 3975 — a particular local environment.</p>
    <p>A surface atom hops to a first-nearest-neighbour vacancy site within the same surface plane. The local chromium / aluminium configuration around atom 3975 sets this event's barrier and rate; comparing it with the same geometric event at a different atom (Event 3) shows how strongly the barrier varies with local chemistry.</p>
    <div class="video-embed">
      <iframe src="https://www.youtube.com/embed/wFuyyo_9nL0" title="Event 2 — surface 1NN in-plane, atom 3975" allow="accelerometer; clipboard-write; encrypted-media; picture-in-picture" allowfullscreen loading="lazy"></iframe>
    </div>
    <div class="event-stills" aria-label="Event 2 stills">
      <figure class="event-still">
        <img src="/assets/images/pykmc-e2-init.jpg" alt="Event 2 — initial state" loading="lazy">
        <figcaption class="caption"><strong>Initial</strong></figcaption>
      </figure>
      <figure class="event-still">
        <img src="/assets/images/pykmc-e2-saddle.jpg" alt="Event 2 — saddle point" loading="lazy">
        <figcaption class="caption"><strong>Saddle</strong></figcaption>
      </figure>
      <figure class="event-still">
        <img src="/assets/images/pykmc-e2-final.jpg" alt="Event 2 — final state" loading="lazy">
        <figcaption class="caption"><strong>Final</strong></figcaption>
      </figure>
    </div>
  </section>

  <section id="event-3" class="pykmc-section">
    <h2>Event 3 — Surface 1NN in-plane (atom 2023)</h2>
    <p class="event-meta">Same geometric event as Event 2, different atom (idx 2023) — different local chemistry, different barrier.</p>
    <p>Atom 2023 makes the same geometric move as atom 3975, but its neighbours differ — so the barrier (and the rate that PyKMC samples it at) differs too. Side-by-side with Event 2, this is the cleanest single-event illustration of the local-environment sensitivity that PyKMC has to resolve at every step.</p>
    <div class="video-embed">
      <iframe src="https://www.youtube.com/embed/QaGVe-QhRt0" title="Event 3 — surface 1NN in-plane, atom 2023" allow="accelerometer; clipboard-write; encrypted-media; picture-in-picture" allowfullscreen loading="lazy"></iframe>
    </div>
    <div class="event-stills" aria-label="Event 3 stills">
      <figure class="event-still">
        <img src="/assets/images/pykmc-e3-init.jpg" alt="Event 3 — initial state" loading="lazy">
        <figcaption class="caption"><strong>Initial</strong></figcaption>
      </figure>
      <figure class="event-still">
        <img src="/assets/images/pykmc-e3-saddle.jpg" alt="Event 3 — saddle point" loading="lazy">
        <figcaption class="caption"><strong>Saddle</strong></figcaption>
      </figure>
      <figure class="event-still">
        <img src="/assets/images/pykmc-e3-final.jpg" alt="Event 3 — final state" loading="lazy">
        <figcaption class="caption"><strong>Final</strong></figcaption>
      </figure>
    </div>
  </section>

  <section id="event-4" class="pykmc-section">
    <h2>Event 4 — Surface ↔ subsurface exchange (upward, atom 3234)</h2>
    <p class="event-meta">Reverse of Event 1: subsurface atom 3234 hops up to the surface. Closes the surface ↔ bulk vacancy cycle.</p>
    <p>The subsurface atom at index 3234 hops up into a surface vacancy, swapping the vacancy back into the bulk. Paired with Event 1, this completes the simplest surface ↔ subsurface exchange cycle and is the elementary step that lets vacancies (and segregating Al) shuttle between the surface and the interior.</p>
    <div class="video-embed">
      <iframe src="https://www.youtube.com/embed/lF9cu1FroHc" title="Event 4 — surface ↔ subsurface exchange (upward), atom 3234" allow="accelerometer; clipboard-write; encrypted-media; picture-in-picture" allowfullscreen loading="lazy"></iframe>
    </div>
    <div class="event-stills" aria-label="Event 4 stills">
      <figure class="event-still">
        <img src="/assets/images/pykmc-e4-init.jpg" alt="Event 4 — initial state" loading="lazy">
        <figcaption class="caption"><strong>Initial</strong></figcaption>
      </figure>
      <figure class="event-still">
        <img src="/assets/images/pykmc-e4-saddle.jpg" alt="Event 4 — saddle point" loading="lazy">
        <figcaption class="caption"><strong>Saddle</strong></figcaption>
      </figure>
      <figure class="event-still">
        <img src="/assets/images/pykmc-e4-final.jpg" alt="Event 4 — final state" loading="lazy">
        <figcaption class="caption"><strong>Final</strong></figcaption>
      </figure>
    </div>
  </section>

  <aside class="pykmc-resources">
    <h2>Resources</h2>
    <ul>
      <li><a href="/assets/pdfs/kerr-2025-scripta-cr-vacancy.pdf" target="_blank" rel="noopener noreferrer">Preprint PDF — Chromium raises vacancy concentration in Ni–Cr–Al</a></li>
      <li><a href="/publications/">All publications</a></li>
      <li><a href="mailto:24jrpc@queensu.ca">Email me with questions</a></li>
    </ul>
  </aside>

</div>
