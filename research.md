---
layout: default
title: Research
---

# Research

My research connects atomic-scale defect mechanisms to the macroscopic performance of structural alloys and catalytic surfaces, using density-functional theory, machine-learning interatomic potentials, and kinetic modelling to bridge from electronic structure to engineering-relevant microstructural evolution.

Two threads unify this work. Physically, vacancy–solute coupling and grain-boundary chemistry govern performance across all three material systems I study — nickel superalloys, zirconium fuel-cladding alloys, and transition-metal catalyst surfaces. Methodologically, ML interatomic potentials (MACE, ACE) trained on DFT data enable systematic exploration of compositional and configurational space at near-DFT accuracy, feeding directly into k-ART kinetic simulations that access experimentally relevant timescales.

<div class="pipeline-diagram" role="figure" aria-label="Multi-scale simulation pipeline: DFT to ML potential to k-ART to observable kinetics">
  <div class="pipeline-step">
    <span class="pipeline-label">Electronic</span>
    <span class="pipeline-name">DFT</span>
    <span class="pipeline-scale">QE · NWChem</span>
  </div>
  <div class="pipeline-step">
    <span class="pipeline-label">Surrogate</span>
    <span class="pipeline-name">ML potential</span>
    <span class="pipeline-scale">MACE · ACE</span>
  </div>
  <div class="pipeline-step">
    <span class="pipeline-label">Kinetics</span>
    <span class="pipeline-name">k-ART</span>
    <span class="pipeline-scale">ARTn + KMC</span>
  </div>
  <div class="pipeline-step">
    <span class="pipeline-label">Observable</span>
    <span class="pipeline-name">Microstructure</span>
    <span class="pipeline-scale">segregation · clustering</span>
  </div>
</div>

Each project shares this core DFT → ML potential → kinetic modelling pipeline, and insights flow between systems: the vacancy–solute framework from Ni–Cr–Al now guides defect calculations in the Zr-alloy project, while surface-energetics tools developed for grain-boundary segregation studies underpin the CO₂ catalysis screening on alloyed Cu surfaces. Universal foundation models (MACE-MP-0, CHGNet) are increasingly reducing the DFT data generation burden, enabling rapid hypothesis testing across new alloy chemistries before committing to full active-learning cycles.

## Current Research

<div class="research-card">
<h3>Vacancy–Solute Coupling in Ni–Fe–Cr–Al Alloys <span class="status-badge active">Active</span></h3>
<p><em>PhD, Queen's University, 2024–present</em></p>
<p>DFT and molecular dynamics show that Cr additions systematically raise the equilibrium vacancy concentration in Ni–Cr–Al and promote Al enrichment at grain boundaries — mechanisms with direct implications for oxidation resistance in high-temperature superalloys. A first-author manuscript has been submitted to <em>Scripta Materialia</em> (<a href="/assets/pdfs/kerr-2025-scripta-cr-vacancy.pdf">preprint, SSRN 5759303</a>). This project anchors the broader programme: the vacancy–solute coupling framework developed here directly motivates parallel studies in Zr cladding alloys and informs how vacancy-mediated surface composition controls catalytic selectivity on alloyed Cu. Current work extends these calculations to Fe-containing quaternary compositions and larger supercells for finite-temperature validation with MACE-driven k-ART trajectories — closing the loop between formation energetics from static DFT and the segregation profiles seen in atom-probe tomography of model superalloys.</p>
</div>

<div class="research-card">
<h3>Defect Kinetics via k-ART <span class="status-badge active">Active</span></h3>
<p><em>PhD, Queen's University, 2025–present</em></p>
<p>k-ART couples the Activation-Relaxation Technique nouveau (ARTn) with kinetic Monte Carlo to access defect clustering, segregation, and microstructural evolution at seconds-to-hours timescales — providing the temporal bridge between DFT energetics and experimentally observable outcomes. k-ART is now parameterised with MACE and ACE potentials trained on DFT data, expanding the range of alloy compositions and defect configurations accessible while maintaining near-DFT fidelity for saddle-point energetics. Production trajectories in Ni–Cr–Al are revealing vacancy-mediated clustering pathways inaccessible to conventional MD, with barrier-statistics benchmarking against NEB reference calculations validating the ML-potential accuracy for transition-state searches. The same workflow is being adapted for hcp Zr, where the lower symmetry and anisotropic migration barriers stress-test the saddle-search infrastructure.</p>
</div>

<div class="research-card">
<h3>CO₂ Catalysis on Metal Surfaces <span class="status-badge active">Active</span></h3>
<p><em>PhD, Queen's University, 2025–present</em></p>
<p>DFT screening of electrochemical CO₂ reduction on transition-metal and alloy surfaces, leveraging the surface-energetics expertise from Ni-alloy grain-boundary work. Current screening covers flat, stepped, and defected facets of alloyed Cu, mapping how vacancy and adatom sites modulate CO₂ binding energies, reaction pathways, and product selectivity toward C₂+ products. The same vacancy-mediated segregation framework used in the Ni–Cr–Al project predicts which alloy surface compositions are thermodynamically accessible under reaction conditions — connecting structural-alloy research to sustainability-driven catalysis. Foundation-model screening (MACE-MP-0) accelerates exploration of the combinatorial composition space before targeted DFT validation.</p>
</div>

<div class="research-card">
<h3>Radiation Damage in Zirconium Alloys <span class="status-badge active">Active</span></h3>
<p><em>PhD, Queen's University, 2025–present</em></p>
<p>Point-defect formation and clustering in Zr-based fuel-cladding alloys, combining MD with empirical and ML potentials alongside DFT validation. Focus: how Nb, Sn, and Fe additions affect defect stability and irradiation-induced microstructural evolution in hcp Zr. Hybrid ML/EAM benchmarking against DFT is establishing the accuracy floor needed for reliable k-ART simulations in these systems — a prerequisite for extending the long-timescale kinetic modelling capabilities proven in fcc Ni alloys to the hcp crystal structure of reactor-grade Zr.</p>
</div>

## Previous Research

<div class="research-card">
<h3>Ion-Pair Trapping in Functionalized Organic Systems <span class="status-badge past">Completed</span></h3>
<p><em>MSc, Ontario Tech, 2021–2023</em></p>
<p>Applied quantum chemistry methods (DFT, Hartree-Fock, MP2) to model noncovalently bound molecular complexes and ion-pair trapping mechanisms in functionalized cyclic hydrocarbons. Explored potential applications in energy storage and light detection.</p>
</div>

<div class="research-card">
<h3>Synthetic Chemistry <span class="status-badge past">Completed</span></h3>
<p><em>Ontario Tech, 2016–2018</em></p>
<p>Laboratory experience with organic synthesis, NMR spectroscopy, UV-Vis characterization, and GC-MS analysis supporting research in molecular systems and functionalized materials.</p>
</div>

## Methods & Tools {#methods--tools}

<div class="methods-grid">
<div class="method-group">
<h4>Simulation Methods</h4>
<ul>
<li>Density-functional theory (DFT)</li>
<li>Molecular dynamics (MD)</li>
<li>Kinetic Activation-Relaxation Technique (k-ART)</li>
<li>Hartree-Fock and post-HF methods (MP2)</li>
<li>Monte Carlo sampling</li>
<li>Machine-learning interatomic potentials (MACE, ACE, foundation models)</li>
</ul>
</div>

<div class="method-group">
<h4>Software</h4>
<ul>
<li>Quantum ESPRESSO</li>
<li>LAMMPS</li>
<li>NWChem</li>
<li>ASE (Atomic Simulation Environment)</li>
<li>pymatgen</li>
<li>VESTA &amp; XCrySDen</li>
</ul>
</div>

<div class="method-group">
<h4>Data Analysis &amp; Workflow</h4>
<ul>
<li>Python (NumPy, SciPy, Pandas, Matplotlib)</li>
<li>Bash &amp; SLURM job orchestration</li>
<li>Jupyter notebooks</li>
<li>Docker for reproducible environments</li>
<li>Git version control</li>
<li>Linux/HPC at scale</li>
<li>LaTeX for technical writing</li>
</ul>
</div>
</div>

## Emerging Directions

<div class="research-card">
<h3>Foundation Models for Atomistic Simulation <span class="status-badge emerging">Emerging</span></h3>
<p>Universal neural-network potentials (MACE-MP-0, CHGNet, M3GNet) are now viable for screening applications, reducing the DFT data generation burden for new alloy compositions. These pre-trained foundation models enter the DFT → ML potential pipeline at two points: upstream, for rapid hypothesis testing across chemical spaces before committing to full active-learning cycles; and downstream, as zero-shot baselines for k-ART saddle-point searches in new chemistries. This directly supports the Zr-alloy project, where hcp training sets remain expensive to build, and the CO₂ catalysis screening, where the combinatorial space of alloy surface compositions exceeds what targeted DFT campaigns can cover. Fine-tuning protocols that adapt foundation models to domain-specific configurations with minimal additional DFT data are an active area of development.</p>
</div>

<div class="research-card">
<h3>Autonomous Simulation Workflows <span class="status-badge emerging">Emerging</span></h3>
<p>LLM-driven agents integrated with high-throughput DFT and MD workflows to automate convergence testing, error detection, and adaptive sampling. Current applications include automated CO₂ adsorption screening across facet–composition space and self-correcting SLURM pipelines for the Ni–Cr–Al k-ART production runs. Longer-term, these agents will close the loop between k-ART kinetic trajectories and active-learning potential refinement, enabling autonomous exploration of defect-evolution pathways in alloy systems too complex for manual campaign design. This direction reflects a broader shift toward AI-accelerated materials discovery, where simulation workflows become increasingly self-directed.</p>
</div>

## Research Interests

<div class="interest-tags">
<span class="interest-tag">Point defects in metallic alloys</span>
<span class="interest-tag">Vacancy formation &amp; stability</span>
<span class="interest-tag">Grain-boundary segregation</span>
<span class="interest-tag">Diffusion &amp; transport</span>
<span class="interest-tag">Long-timescale kinetics (k-ART, KMC)</span>
<span class="interest-tag">Saddle-point search &amp; NEB</span>
<span class="interest-tag">Radiation damage in nuclear alloys</span>
<span class="interest-tag">Ni–Fe–Cr–Al alloys</span>
<span class="interest-tag">Zr alloys &amp; fuel cladding</span>
<span class="interest-tag">CO₂ reduction catalysis</span>
<span class="interest-tag">Surface energetics &amp; adsorption</span>
<span class="interest-tag">Stepped &amp; defected facets</span>
<span class="interest-tag">Oxidation resistance</span>
<span class="interest-tag">Structure–property relationships</span>
<span class="interest-tag">Machine-learning interatomic potentials</span>
<span class="interest-tag">Foundation models for materials</span>
<span class="interest-tag">Active-learning potential training</span>
<span class="interest-tag">Autonomous simulation workflows</span>
<span class="interest-tag">High-throughput DFT screening</span>
<span class="interest-tag">Multi-scale modelling</span>
<span class="interest-tag">Reproducible computational science</span>
</div>
