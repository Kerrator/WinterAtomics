---
layout: default
title: "PyKMC Talk"
permalink: /pykmc/
description: "Companion landing page for Stephen Kerr's talk on PyKMC and the Ni–Cr–Al vacancy / segregation work — short video walkthroughs of the algorithm, TST, percolation, and Wagner's third element effect."
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
<meta property="og:title" content="PyKMC Talk — Stephen Kerr">
<meta property="og:description" content="Companion landing page with short walkthroughs of the PyKMC algorithm, TST, percolation, and Wagner's third element effect.">
<meta property="og:image" content="https://www.winteratomics.ca/assets/images/graphical-abstract-cr-vacancy.png">

<!-- Twitter -->
<meta name="twitter:card" content="summary_large_image">
<meta name="twitter:url" content="https://www.winteratomics.ca/pykmc/">
<meta name="twitter:title" content="PyKMC Talk — Stephen Kerr">
<meta name="twitter:description" content="Companion landing page with short walkthroughs of the PyKMC algorithm, TST, percolation, and Wagner's third element effect.">
<meta name="twitter:image" content="https://www.winteratomics.ca/assets/images/graphical-abstract-cr-vacancy.png">

<div class="pykmc-page">

  <div class="pykmc-hero">
    <h1>PyKMC Talk</h1>
    <p class="tagline">A short companion page for the talk. The four videos below walk through the core ideas in roughly the order they appear in the presentation.</p>
  </div>

  <nav class="pykmc-toc" aria-label="On this page">
    <strong>On this page</strong>
    <ol>
      <li><a href="#algorithm">The PyKMC algorithm</a></li>
      <li><a href="#tst">Transition state theory</a></li>
      <li><a href="#percolation">Percolation theory</a></li>
      <li><a href="#tee">Wagner's third element effect</a></li>
    </ol>
  </nav>

  <section id="algorithm" class="pykmc-section">
    <h2>The PyKMC algorithm</h2>
    <p>How PyKMC samples atomic-scale rare events on a fixed lattice — event catalogue, KMC time step, and acceptance criterion. The walkthrough zooms in on a vacancy hop in Ni–Cr–Al and shows how DFT-derived barriers feed the simulation.</p>
    <div class="video-embed">
      <!-- TODO: replace VIDEO_ID_ALGORITHM with the YouTube ID after upload -->
      <iframe src="https://www.youtube.com/embed/VIDEO_ID_ALGORITHM" title="PyKMC algorithm walkthrough" allow="accelerometer; clipboard-write; encrypted-media; picture-in-picture" allowfullscreen loading="lazy"></iframe>
    </div>
  </section>

  <section id="tst" class="pykmc-section">
    <h2>Transition state theory</h2>
    <p>TST gives us the rate constants that PyKMC consumes. This short clip covers the harmonic-TST expression, how saddle points are located with NEB, and the assumptions that matter (and the ones that don't).</p>
    <div class="video-embed">
      <!-- TODO: replace VIDEO_ID_TST with the YouTube ID after upload -->
      <iframe src="https://www.youtube.com/embed/VIDEO_ID_TST" title="Transition state theory walkthrough" allow="accelerometer; clipboard-write; encrypted-media; picture-in-picture" allowfullscreen loading="lazy"></iframe>
    </div>
  </section>

  <section id="percolation" class="pykmc-section">
    <h2>Percolation theory</h2>
    <p>Connected paths of vacancies (or of aluminium atoms) control bulk transport. The video shows why the percolation threshold is a useful lens on selective-oxidation onset, and where the threshold lands for Ni–Cr–Al.</p>
    <div class="video-embed">
      <!-- TODO: replace VIDEO_ID_PERCOLATION with the YouTube ID after upload -->
      <iframe src="https://www.youtube.com/embed/VIDEO_ID_PERCOLATION" title="Percolation theory walkthrough" allow="accelerometer; clipboard-write; encrypted-media; picture-in-picture" allowfullscreen loading="lazy"></iframe>
    </div>
  </section>

  <section id="tee" class="pykmc-section">
    <h2>Wagner's third element effect</h2>
    <p>Wagner's model explains why adding chromium changes the selective-oxidation regime in Ni–Al — and why the same alloying element can both raise vacancy concentration in the bulk and promote Al segregation to the grain boundary. The clip frames the experimental signature that motivated this work.</p>
    <div class="video-embed">
      <!-- TODO: replace VIDEO_ID_TEE with the YouTube ID after upload -->
      <iframe src="https://www.youtube.com/embed/VIDEO_ID_TEE" title="Wagner's third element effect walkthrough" allow="accelerometer; clipboard-write; encrypted-media; picture-in-picture" allowfullscreen loading="lazy"></iframe>
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
