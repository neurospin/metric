---
layout: page_team
title: MRI INSTRUMENTATION
cat: metric
subcat: team
headline:
teasing: Our team conducts hardware developments for MRI instrumentation at Ultra-High-Field (UHF). Primarily we design and build RF head coils suited for NeuroSpin needs, mainly for humans but also for animals for fMRI studies. We put a strong emphasis on parallel transmit coils and receive arrays for our clinical 7T and 11.7T scanners. We also develop original multi-coil arrays dedicated to human and NHP brain shimming.
leader: Alexis Amadon
icon: noimage.png
added: 2025
permalink: teams/metric-instrumentation.html
---

<!-- Banner -->
<section id="banner">
<div class="content">
  <header><p>{{ page.title }} team</p></header>
  <p>
   Our team conducts hardware developments for MRI instrumentation at Ultra-High-Field (UHF). Primarily we design and build RF head coils suited for NeuroSpin needs, mainly for humans but also for animals for fMRI studies. We put a strong emphasis on parallel transmit coils and receive arrays for our clinical 7T and 11.7T scanners. We also develop original multi-coil arrays dedicated to human and NHP brain shimming.
  </p>
  <p>
    <b> Leader: </b>
    <script>mail2("{{page.leader | replace: " ", "." | downcase}}", "cea", 3, "", "{{page.leader}}")</script>
  </p>
</div>
<span class="image object">
  <img src="{{site.url}}{{site.baseurl}}/images/labs/{{page.icon}}" alt="" />
</span>
</section>

<!-- Content -->
<br>
<b>1. RF coils</b>

Parallel transmit RF coils (so-called pTx coils) are desired to bring the degrees of freedom needed to overcome the B1 field inhomogeneity issue at UHF, obtain uniform brain excitation and maintain the expected contrast across the image. This is why we started making such coils for humans at 7T as early as in 2008, based on strip-line transceiver dipoles. Our first 8-Tx human-safe head prototype allowed to validate our licensed kT-points transmission method for whole brain excitation, leading to B1-artefact-free images. To increase SNR, we then built prototypes with higher numbers of receive elements (8->24->32), featuring a circularly-polarized patch at the top of the head, two rows of shorter staggered strip-line dipoles and receive-only loops in-between. This is how we chose to build the first RF coil for our Iseult scanner, with 15 Tx- and 32 Rx-elements, all relying on specific geometry for decoupling, and bringing forth the first in-vivo human brain images ever made at 11.7 Tesla. 

On the other hand, close-fit receive arrays are essential for better signal-to-noise ratio. So more recently, we put efforts into enhancing SNR at 11.7T thanks to High-Impedance coils placed in a honeycomb pattern on a flexible cap, to be used for high-resolution fMRI of temporal lobes. We are in the process of applying this High-Impedance technology to single-row transceiver dipoles from which we expect a significant gain in both transmit efficiency and SNR for the entire human brain. Later on we will focus on a 56-HIC cap in the perspective of a 64-channel upgrade of our Iseult scanner in the coming years. Such later works are performed in the framework of the Franco-German UHF-NeuroBoost project (ANR-DFG grant). 

Another accomplishment at 7T, part of the former European M-One project, consisted in building a human receive-array based on two preamp-decoupled loop layers, the outer layer consisting in larger elements to regain signal towards the center of the head. A special feature was the making of reproducible loops from a new additive copper technology.
We have also developed a hybrid coil for macaques in the sphinx position at 7T to present fMRI stimuli and have less echo-planar imaging artefacts, featuring both Tx-Rx dipoles and Rx-loops, and are in the process of building similar coil arrays at 11.7T, with Low-Impedance and High-Impedance loops. 

<b>2. B0-shim multi-coil arrays</b>

Some of the coils above were made to fit in brain-dedicated cylindrical multicoil shim arrays, meant to homogenize the static magnetic field in the brain. Fine-shimming consists in compensating magnetic susceptibility disparities in the brain due to the presence of air cavities such as sinus or ear canals; these increase B0 inhomogeneities as the B0-strength rises, worsening image distortions and signal dropout in Echo-Planar-Imaging for instance. So we devised a patented design method for low-cost shim arrays, so-called SCOTCH, whereby the coil windings’ shape, size and location are optimized for whole brain shimming. We thus produced 48-coil prototypes on 3 cylindrical layers for 1/ human brain shimming in the supine position, and 2/ macaque brain in the sphinx position. At 7T, with a maximum of 3A per channel, we showed our shim arrays outperform all existing multicoil arrays in whole-brain shimming, being equivalent to spherical-harmonics correcting systems with unlimited power up to 7th-order. Moreover such arrays can be driven for dynamic shimming, using feedback-controlled electronics designed at MIT/MGH. We upgraded such electronics to allow 5A per channel in order to get the same performance at 11.7T as at 7T. We thus expect on average a 37% gain in the brain B0 homogeneity. Work is under way to optimize shimming in brain ROIs such as the temporal lobes or the prefrontal cortex without compromising shimming in the rest of the brain...

<b>3. Resources for our developments</b>

Before implementation, our hardware is always modeled and simulated, in particular with the Ansys electro-magnetic software package (including HFSS). From simulations of our RF coils loaded with human head models, we go all the way to predict SNR and Specific Absorption Rate (SAR), usually under Matlab.
The MRI Instrumentation team also relies on an electronic workshop for developing, maintaining and testing RF coils and other electronics hardware. It features spectrum analyzers, vector network analyzers, signal generators, oscilloscopes, LCR meters, Faraday cages and a home-made 16-Tx, 64-Rx workbench to test our pTx coils and receive arrays. 
