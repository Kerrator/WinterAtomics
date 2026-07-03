---
layout: default
title: Home
---

# About

<p class="intro-highlight">I am a PhD candidate in computational materials science at Queen's University, working with <a href="https://me.queensu.ca/People/Beland/" target="_blank">Laurent Karim Béland</a> in the Department of Mechanical and Materials Engineering. I use first-principles simulation, machine-learning interatomic potentials, and kinetic modelling to understand how atomic-scale defects govern the performance of structural alloys and catalytic surfaces — connecting vacancy chemistry in nuclear materials to product selectivity in CO₂ conversion.</p>

<div class="bio-section">
<h2>Currently working on</h2>

<ul class="focus-list">
<li><strong>Ni–Cr–Al k-ART production runs.</strong> MACE-driven kinetic trajectories are now resolving vacancy–solute clustering and Al segregation to grain boundaries on second-to-hour timescales — the regime where oxide-scale chemistry is actually decided.</li>
<li><strong>CO₂ on stepped &amp; defected Cu.</strong> Mapping how step-edge vacancies and Zn / Ag dopants reshape CO₂ binding energetics and the &#42;CO – &#42;COH branching point that gates C₂⁺ selectivity.</li>
<li><strong>Zr–Nb radiation damage in hcp.</strong> Hybrid ML / EAM benchmarking against DFT to establish the accuracy floor needed before pushing k-ART into the hcp regime relevant to CANDU fuel cladding.</li>
<li><strong>Foundation-model screening.</strong> Stress-testing MACE-MP-0 as a zero-shot baseline for new alloy chemistries, with light fine-tuning where it matters for saddle-point energetics.</li>
</ul>

<h2 style="margin-top:2rem;">Recent updates</h2>

<div class="update-item">
<span class="update-date">May 2026</span>
<p>Ni–Cr–Al k-ART production trajectories with MACE potentials are now resolving multi-vacancy clustering and Al grain-boundary enrichment over experimentally meaningful timescales — the temporal window where conventional MD runs out. CO₂ binding screening has expanded to stepped and defected Cu facets, applying the same vacancy-mediated segregation framework developed for the Ni-alloy work to predict the surface compositions actually accessible under reaction conditions.</p>
</div>

<div class="update-item">
<span class="update-date">Winter 2026</span>
<p>Zr–Nb radiation-damage modelling underway with hybrid ML/EAM benchmarking against DFT references — pushing the long-timescale kinetic framework from fcc Ni alloys into the hcp regime relevant to reactor-grade Zr. Co-instructed and TA'd MECH 479 (Nanomaterials) for the second consecutive year, with a new computational module on reproducible MD workflows.</p>
</div>

<div class="update-item">
<span class="update-date">2025</span>
<p>First-author manuscript on Cr–vacancy interactions submitted to <em>Scripta Materialia</em> (<a href="/assets/pdfs/kerr-2025-scripta-cr-vacancy.pdf">preprint</a>, SSRN 5759303). Completed k-ART parameterisation with MACE potentials for fcc Ni alloys. Began CO₂ catalysis DFT screening on alloyed Cu and Zr-alloy point-defect calculations.</p>
</div>

</div>

<div class="bio-section">
<h2>Research</h2>

My work centres on a single question: how do point defects interact with alloying elements to control composition, structure, and properties at interfaces? Vacancy–solute coupling is the common thread — governing oxidation resistance in Ni-based superalloys, radiation tolerance in Zr fuel cladding, and product selectivity on catalytic surfaces for CO₂ conversion. Machine-learning interatomic potentials (MACE, ACE) and the kinetic Activation-Relaxation Technique (k-ART) bridge electronic-structure calculations to experimentally relevant timescales. Four interconnected projects share a core DFT → ML potential → kinetic modelling pipeline:

<div class="project-list">
<div class="project-item">
<strong>Vacancy–solute coupling in Ni–Cr–Al</strong> — How Cr raises vacancy concentrations and drives Al to grain boundaries, connecting electronic structure to oxidation resistance.
</div>
<div class="project-item">
<strong>k-ART for long-timescale defect kinetics</strong> — Parameterising k-ART with MACE and ACE potentials to bridge DFT energetics to observable microstructural evolution.
</div>
<div class="project-item">
<strong>Radiation damage in Zr alloys</strong> — Extending the vacancy–solute framework to Zr-based fuel cladding under irradiation, with hybrid ML/EAM potentials for hcp systems.
</div>
<div class="project-item">
<strong>CO₂ catalysis on metal surfaces</strong> — Surface-defect energetics on alloyed Cu controlling binding, selectivity, and reaction pathways for electrochemical CO₂ conversion.
</div>
</div>

<div class="pipeline-connector">Shared multi-scale pipeline</div>

<div class="pipeline-diagram" role="figure" aria-label="Multi-scale simulation pipeline: DFT to ML potential to k-ART to observable kinetics">
  <div class="pipeline-step">
    <span class="pipeline-label">Electronic</span>
    <span class="pipeline-name">DFT</span>
    <span class="pipeline-scale">Å · ps</span>
  </div>
  <div class="pipeline-step">
    <span class="pipeline-label">Surrogate</span>
    <span class="pipeline-name">ML potential</span>
    <span class="pipeline-scale">MACE · ACE</span>
  </div>
  <div class="pipeline-step">
    <span class="pipeline-label">Long timescale</span>
    <span class="pipeline-name">k-ART</span>
    <span class="pipeline-scale">nm · s–h</span>
  </div>
  <div class="pipeline-step">
    <span class="pipeline-label">Observable</span>
    <span class="pipeline-name">Microstructure</span>
    <span class="pipeline-scale">segregation · barriers</span>
  </div>
</div>

All four projects feed into the same multi-scale workflow: DFT reference data trains ML potentials, which enable k-ART kinetics at experimentally relevant timescales. Universal foundation models (MACE-MP-0, CHGNet) are increasingly enabling zero-shot screening across new chemistries before committing to full active-learning cycles. See <a href="/research">Research</a> for project details and emerging work on autonomous simulation workflows.

</div>

<div class="bio-section">
<h2>Methods</h2>

Multi-scale workflow: Quantum ESPRESSO and NWChem for DFT, MACE / ACE machine-learning potentials, LAMMPS for MD, and k-ART for long-timescale kinetics — orchestrated with Python (ASE, pymatgen, NumPy, SciPy, matplotlib) and bash on SLURM-managed HPC clusters. Universal foundation models (MACE-MP-0, CHGNet) provide zero-shot baselines for new chemistries, and LLM-driven agents are beginning to automate convergence testing and adaptive sampling around the loop. See <a href="/research#methods--tools">Research</a> for the full toolkit.

</div>

<div class="bio-section">
<h2>Teaching</h2>

I teach undergraduate courses in materials science and chemistry at Queen's University, with prior experience coordinating laboratory sections at Ontario Tech. My teaching emphasises reproducible computation, hands-on problem-solving, and responsible integration of AI tools in scientific workflows. See <a href="/teaching">Teaching</a> for course details.

</div>

<div class="bio-section">
<h2>Background</h2>

MSc in Materials Science (2023) and BSc in Chemistry (2021) from Ontario Tech University. Earlier research applied quantum chemistry methods to ion-pair trapping mechanisms in functionalised organic systems, developing the computational surface-chemistry intuition that now informs my work on alloy grain boundaries and catalytic surfaces.

</div>
